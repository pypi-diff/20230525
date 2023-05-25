# Comparing `tmp/fmsne-0.6.4.tar.gz` & `tmp/fmsne-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fmsne-0.6.4.tar", last modified: Thu May 25 06:01:05 2023, max compression
+gzip compressed data, was "fmsne-0.6.5.tar", last modified: Thu May 25 13:44:58 2023, max compression
```

## Comparing `fmsne-0.6.4.tar` & `fmsne-0.6.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 lgatto    (1001) lgatto    (1001)        0 2023-05-25 06:01:05.422820 fmsne-0.6.4/
--rw-rw-r--   0 lgatto    (1001) lgatto    (1001)     1195 2023-05-17 17:30:25.000000 fmsne-0.6.4/LICENCE.md
--rw-rw-r--   0 lgatto    (1001) lgatto    (1001)       67 2023-05-17 17:30:25.000000 fmsne-0.6.4/MANIFEST.in
--rw-rw-r--   0 lgatto    (1001) lgatto    (1001)     8788 2023-05-25 06:01:05.422820 fmsne-0.6.4/PKG-INFO
--rw-rw-r--   0 lgatto    (1001) lgatto    (1001)     8200 2023-05-17 17:30:25.000000 fmsne-0.6.4/README.md
-drwxrwxr-x   0 lgatto    (1001) lgatto    (1001)        0 2023-05-25 06:01:05.422820 fmsne-0.6.4/fmsne/
--rw-rw-r--   0 lgatto    (1001) lgatto    (1001)       44 2023-05-24 06:08:00.000000 fmsne-0.6.4/fmsne/__init__.py
--rw-rw-r--   0 lgatto    (1001) lgatto    (1001)     3380 2023-05-17 17:30:25.000000 fmsne-0.6.4/fmsne/arithmetic_ansi.h
--rw-rw-r--   0 lgatto    (1001) lgatto    (1001)     8830 2023-05-17 17:30:25.000000 fmsne-0.6.4/fmsne/arithmetic_sse_double.h
--rw-rw-r--   0 lgatto    (1001) lgatto    (1001)     9070 2023-05-17 17:30:25.000000 fmsne-0.6.4/fmsne/arithmetic_sse_float.h
--rw-rw-r--   0 lgatto    (1001) lgatto    (1001)    41394 2023-05-24 06:33:59.000000 fmsne-0.6.4/fmsne/fmsne.py
--rw-rw-r--   0 lgatto    (1001) lgatto    (1001)  2008886 2023-05-21 12:37:39.000000 fmsne-0.6.4/fmsne/fmsne_implem.cpp
--rw-rw-r--   0 lgatto    (1001) lgatto    (1001)   171438 2023-05-17 17:30:25.000000 fmsne-0.6.4/fmsne/fmsne_implem.pyx
--rw-rw-r--   0 lgatto    (1001) lgatto    (1001)    41095 2023-05-17 17:30:25.000000 fmsne-0.6.4/fmsne/lbfgs.c
--rw-rw-r--   0 lgatto    (1001) lgatto    (1001)    32648 2023-05-17 17:30:25.000000 fmsne-0.6.4/fmsne/lbfgs.h
--rw-rw-r--   0 lgatto    (1001) lgatto    (1001)    19367 2023-05-17 17:30:25.000000 fmsne-0.6.4/fmsne/vptree.h
-drwxrwxr-x   0 lgatto    (1001) lgatto    (1001)        0 2023-05-25 06:01:05.422820 fmsne-0.6.4/fmsne.egg-info/
--rw-rw-r--   0 lgatto    (1001) lgatto    (1001)     8788 2023-05-25 06:01:05.000000 fmsne-0.6.4/fmsne.egg-info/PKG-INFO
--rw-rw-r--   0 lgatto    (1001) lgatto    (1001)      400 2023-05-25 06:01:05.000000 fmsne-0.6.4/fmsne.egg-info/SOURCES.txt
--rw-rw-r--   0 lgatto    (1001) lgatto    (1001)        1 2023-05-25 06:01:05.000000 fmsne-0.6.4/fmsne.egg-info/dependency_links.txt
--rw-rw-r--   0 lgatto    (1001) lgatto    (1001)       49 2023-05-25 06:01:05.000000 fmsne-0.6.4/fmsne.egg-info/requires.txt
--rw-rw-r--   0 lgatto    (1001) lgatto    (1001)       19 2023-05-25 06:01:05.000000 fmsne-0.6.4/fmsne.egg-info/top_level.txt
--rw-rw-r--   0 lgatto    (1001) lgatto    (1001)      579 2023-05-25 06:01:05.426820 fmsne-0.6.4/setup.cfg
--rw-rw-r--   0 lgatto    (1001) lgatto    (1001)     1017 2023-05-21 13:08:54.000000 fmsne-0.6.4/setup.py
+drwxrwxr-x   0 lgatto    (1001) lgatto    (1001)        0 2023-05-25 13:44:58.590957 fmsne-0.6.5/
+-rw-rw-r--   0 lgatto    (1001) lgatto    (1001)     1195 2023-05-17 17:30:25.000000 fmsne-0.6.5/LICENCE.md
+-rw-rw-r--   0 lgatto    (1001) lgatto    (1001)       67 2023-05-17 17:30:25.000000 fmsne-0.6.5/MANIFEST.in
+-rw-rw-r--   0 lgatto    (1001) lgatto    (1001)     8788 2023-05-25 13:44:58.590957 fmsne-0.6.5/PKG-INFO
+-rw-rw-r--   0 lgatto    (1001) lgatto    (1001)     8200 2023-05-17 17:30:25.000000 fmsne-0.6.5/README.md
+drwxrwxr-x   0 lgatto    (1001) lgatto    (1001)        0 2023-05-25 13:44:58.590957 fmsne-0.6.5/fmsne/
+-rw-rw-r--   0 lgatto    (1001) lgatto    (1001)       44 2023-05-25 13:44:49.000000 fmsne-0.6.5/fmsne/__init__.py
+-rw-rw-r--   0 lgatto    (1001) lgatto    (1001)     3380 2023-05-17 17:30:25.000000 fmsne-0.6.5/fmsne/arithmetic_ansi.h
+-rw-rw-r--   0 lgatto    (1001) lgatto    (1001)     8830 2023-05-17 17:30:25.000000 fmsne-0.6.5/fmsne/arithmetic_sse_double.h
+-rw-rw-r--   0 lgatto    (1001) lgatto    (1001)     9070 2023-05-17 17:30:25.000000 fmsne-0.6.5/fmsne/arithmetic_sse_float.h
+-rw-rw-r--   0 lgatto    (1001) lgatto    (1001)    41404 2023-05-25 13:44:49.000000 fmsne-0.6.5/fmsne/fmsne.py
+-rw-rw-r--   0 lgatto    (1001) lgatto    (1001)  2008886 2023-05-21 12:37:39.000000 fmsne-0.6.5/fmsne/fmsne_implem.cpp
+-rw-rw-r--   0 lgatto    (1001) lgatto    (1001)   171438 2023-05-17 17:30:25.000000 fmsne-0.6.5/fmsne/fmsne_implem.pyx
+-rw-rw-r--   0 lgatto    (1001) lgatto    (1001)    41095 2023-05-17 17:30:25.000000 fmsne-0.6.5/fmsne/lbfgs.c
+-rw-rw-r--   0 lgatto    (1001) lgatto    (1001)    32648 2023-05-17 17:30:25.000000 fmsne-0.6.5/fmsne/lbfgs.h
+-rw-rw-r--   0 lgatto    (1001) lgatto    (1001)    19367 2023-05-17 17:30:25.000000 fmsne-0.6.5/fmsne/vptree.h
+drwxrwxr-x   0 lgatto    (1001) lgatto    (1001)        0 2023-05-25 13:44:58.590957 fmsne-0.6.5/fmsne.egg-info/
+-rw-rw-r--   0 lgatto    (1001) lgatto    (1001)     8788 2023-05-25 13:44:58.000000 fmsne-0.6.5/fmsne.egg-info/PKG-INFO
+-rw-rw-r--   0 lgatto    (1001) lgatto    (1001)      400 2023-05-25 13:44:58.000000 fmsne-0.6.5/fmsne.egg-info/SOURCES.txt
+-rw-rw-r--   0 lgatto    (1001) lgatto    (1001)        1 2023-05-25 13:44:58.000000 fmsne-0.6.5/fmsne.egg-info/dependency_links.txt
+-rw-rw-r--   0 lgatto    (1001) lgatto    (1001)       49 2023-05-25 13:44:58.000000 fmsne-0.6.5/fmsne.egg-info/requires.txt
+-rw-rw-r--   0 lgatto    (1001) lgatto    (1001)       19 2023-05-25 13:44:58.000000 fmsne-0.6.5/fmsne.egg-info/top_level.txt
+-rw-rw-r--   0 lgatto    (1001) lgatto    (1001)      579 2023-05-25 13:44:58.590957 fmsne-0.6.5/setup.cfg
+-rw-rw-r--   0 lgatto    (1001) lgatto    (1001)     1017 2023-05-21 13:08:54.000000 fmsne-0.6.5/setup.py
```

### Comparing `fmsne-0.6.4/LICENCE.md` & `fmsne-0.6.5/LICENCE.md`

 * *Files identical despite different names*

### Comparing `fmsne-0.6.4/PKG-INFO` & `fmsne-0.6.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fmsne
-Version: 0.6.4
+Version: 0.6.5
 Summary: Fast Multi-Scale Neighbour Embedding
 Home-page: https://github.com/cdebodt/Fast_Multi-scale_NE
 Author: Cyril de Bodt
 Author-email: cyril.debodt@uclouvain.be
 Maintainer: Laurent Gatto
 Maintainer-email: laurent.gatto@uclouvain.be
 License: MIT
```

### Comparing `fmsne-0.6.4/README.md` & `fmsne-0.6.5/README.md`

 * *Files identical despite different names*

### Comparing `fmsne-0.6.4/fmsne/arithmetic_ansi.h` & `fmsne-0.6.5/fmsne/arithmetic_ansi.h`

 * *Files identical despite different names*

### Comparing `fmsne-0.6.4/fmsne/arithmetic_sse_double.h` & `fmsne-0.6.5/fmsne/arithmetic_sse_double.h`

 * *Files identical despite different names*

### Comparing `fmsne-0.6.4/fmsne/arithmetic_sse_float.h` & `fmsne-0.6.5/fmsne/arithmetic_sse_float.h`

 * *Files identical despite different names*

### Comparing `fmsne-0.6.4/fmsne/fmsne.py` & `fmsne-0.6.5/fmsne/fmsne.py`

 * *Files 1% similar despite different names*

```diff
@@ -919,15 +919,15 @@
     Computes the pairwise Euclidean distances of HD and several LD
     embeddings X and Ys and then computes the DR quality assessment
     criteria R_{NX}(K) and AUC for each (X, Yi).
     """
     rnx = []
     d_hd = eucl_dist_matr(X)
     for Y in Ys:
-        d_ld = eucl_dist_matr(Y)
+        d_ld = eucl_dist_matr(np.array(Y))
         rnx.append(eval_dr_quality(d_hd = d_hd,
                                    d_ld = d_ld))
     return(rnx)
 
 def eval_red_rnx_auc_from_data(X, Y, Kup = 10000):
     """
     Computes the reduced DR quality assessment criteria R_{NX}(K)
```

### Comparing `fmsne-0.6.4/fmsne/fmsne_implem.cpp` & `fmsne-0.6.5/fmsne/fmsne_implem.cpp`

 * *Files identical despite different names*

### Comparing `fmsne-0.6.4/fmsne/fmsne_implem.pyx` & `fmsne-0.6.5/fmsne/fmsne_implem.pyx`

 * *Files identical despite different names*

### Comparing `fmsne-0.6.4/fmsne/lbfgs.c` & `fmsne-0.6.5/fmsne/lbfgs.c`

 * *Files identical despite different names*

### Comparing `fmsne-0.6.4/fmsne/lbfgs.h` & `fmsne-0.6.5/fmsne/lbfgs.h`

 * *Files identical despite different names*

### Comparing `fmsne-0.6.4/fmsne/vptree.h` & `fmsne-0.6.5/fmsne/vptree.h`

 * *Files identical despite different names*

### Comparing `fmsne-0.6.4/fmsne.egg-info/PKG-INFO` & `fmsne-0.6.5/fmsne.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fmsne
-Version: 0.6.4
+Version: 0.6.5
 Summary: Fast Multi-Scale Neighbour Embedding
 Home-page: https://github.com/cdebodt/Fast_Multi-scale_NE
 Author: Cyril de Bodt
 Author-email: cyril.debodt@uclouvain.be
 Maintainer: Laurent Gatto
 Maintainer-email: laurent.gatto@uclouvain.be
 License: MIT
```

### Comparing `fmsne-0.6.4/setup.cfg` & `fmsne-0.6.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `fmsne-0.6.4/setup.py` & `fmsne-0.6.5/setup.py`

 * *Files identical despite different names*

