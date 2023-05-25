# Comparing `tmp/HomoglyphsCJK-0.1.0.tar.gz` & `tmp/HomoglyphsCJK-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HomoglyphsCJK-0.1.0.tar", last modified: Thu May 25 02:47:12 2023, max compression
+gzip compressed data, was "HomoglyphsCJK-0.1.1.tar", last modified: Thu May 25 03:10:08 2023, max compression
```

## Comparing `HomoglyphsCJK-0.1.0.tar` & `HomoglyphsCJK-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 yangxinmei   (501) staff       (20)        0 2023-05-25 02:47:12.856681 HomoglyphsCJK-0.1.0/
-drwxr-xr-x   0 yangxinmei   (501) staff       (20)        0 2023-05-25 02:47:12.851896 HomoglyphsCJK-0.1.0/HomoglyphsCJK/
--rw-r--r--   0 yangxinmei   (501) staff       (20)       93 2023-05-22 03:32:58.000000 HomoglyphsCJK-0.1.0/HomoglyphsCJK/__init__.py
--rw-r--r--   0 yangxinmei   (501) staff       (20)     9586 2023-05-25 02:44:44.000000 HomoglyphsCJK-0.1.0/HomoglyphsCJK/hg_functions.py
--rw-r--r--   0 yangxinmei   (501) staff       (20)     2422 2023-05-13 13:49:58.000000 HomoglyphsCJK-0.1.0/HomoglyphsCJK/test_run.py
-drwxr-xr-x   0 yangxinmei   (501) staff       (20)        0 2023-05-25 02:47:12.856082 HomoglyphsCJK-0.1.0/HomoglyphsCJK.egg-info/
--rw-r--r--   0 yangxinmei   (501) staff       (20)     3752 2023-05-25 02:47:12.000000 HomoglyphsCJK-0.1.0/HomoglyphsCJK.egg-info/PKG-INFO
--rw-r--r--   0 yangxinmei   (501) staff       (20)      284 2023-05-25 02:47:12.000000 HomoglyphsCJK-0.1.0/HomoglyphsCJK.egg-info/SOURCES.txt
--rw-r--r--   0 yangxinmei   (501) staff       (20)        1 2023-05-25 02:47:12.000000 HomoglyphsCJK-0.1.0/HomoglyphsCJK.egg-info/dependency_links.txt
--rw-r--r--   0 yangxinmei   (501) staff       (20)       44 2023-05-25 02:47:12.000000 HomoglyphsCJK-0.1.0/HomoglyphsCJK.egg-info/requires.txt
--rw-r--r--   0 yangxinmei   (501) staff       (20)       14 2023-05-25 02:47:12.000000 HomoglyphsCJK-0.1.0/HomoglyphsCJK.egg-info/top_level.txt
--rw-r--r--   0 yangxinmei   (501) staff       (20)     3752 2023-05-25 02:47:12.856453 HomoglyphsCJK-0.1.0/PKG-INFO
--rw-r--r--   0 yangxinmei   (501) staff       (20)     3208 2023-05-25 02:46:46.000000 HomoglyphsCJK-0.1.0/README.md
--rw-r--r--   0 yangxinmei   (501) staff       (20)       38 2023-05-25 02:47:12.856730 HomoglyphsCJK-0.1.0/setup.cfg
--rw-r--r--   0 yangxinmei   (501) staff       (20)      950 2023-05-25 02:44:47.000000 HomoglyphsCJK-0.1.0/setup.py
+drwxr-xr-x   0 yangxinmei   (501) staff       (20)        0 2023-05-25 03:10:08.447877 HomoglyphsCJK-0.1.1/
+drwxr-xr-x   0 yangxinmei   (501) staff       (20)        0 2023-05-25 03:10:08.446570 HomoglyphsCJK-0.1.1/HomoglyphsCJK/
+-rw-r--r--   0 yangxinmei   (501) staff       (20)       93 2023-05-22 03:32:58.000000 HomoglyphsCJK-0.1.1/HomoglyphsCJK/__init__.py
+-rw-r--r--   0 yangxinmei   (501) staff       (20)     9649 2023-05-25 03:06:03.000000 HomoglyphsCJK-0.1.1/HomoglyphsCJK/hg_functions.py
+-rw-r--r--   0 yangxinmei   (501) staff       (20)     2422 2023-05-13 13:49:58.000000 HomoglyphsCJK-0.1.1/HomoglyphsCJK/test_run.py
+drwxr-xr-x   0 yangxinmei   (501) staff       (20)        0 2023-05-25 03:10:08.447534 HomoglyphsCJK-0.1.1/HomoglyphsCJK.egg-info/
+-rw-r--r--   0 yangxinmei   (501) staff       (20)     3989 2023-05-25 03:10:08.000000 HomoglyphsCJK-0.1.1/HomoglyphsCJK.egg-info/PKG-INFO
+-rw-r--r--   0 yangxinmei   (501) staff       (20)      284 2023-05-25 03:10:08.000000 HomoglyphsCJK-0.1.1/HomoglyphsCJK.egg-info/SOURCES.txt
+-rw-r--r--   0 yangxinmei   (501) staff       (20)        1 2023-05-25 03:10:08.000000 HomoglyphsCJK-0.1.1/HomoglyphsCJK.egg-info/dependency_links.txt
+-rw-r--r--   0 yangxinmei   (501) staff       (20)       44 2023-05-25 03:10:08.000000 HomoglyphsCJK-0.1.1/HomoglyphsCJK.egg-info/requires.txt
+-rw-r--r--   0 yangxinmei   (501) staff       (20)       14 2023-05-25 03:10:08.000000 HomoglyphsCJK-0.1.1/HomoglyphsCJK.egg-info/top_level.txt
+-rw-r--r--   0 yangxinmei   (501) staff       (20)     3989 2023-05-25 03:10:08.447718 HomoglyphsCJK-0.1.1/PKG-INFO
+-rw-r--r--   0 yangxinmei   (501) staff       (20)     3445 2023-05-25 03:09:44.000000 HomoglyphsCJK-0.1.1/README.md
+-rw-r--r--   0 yangxinmei   (501) staff       (20)       38 2023-05-25 03:10:08.447923 HomoglyphsCJK-0.1.1/setup.cfg
+-rw-r--r--   0 yangxinmei   (501) staff       (20)      950 2023-05-25 03:10:01.000000 HomoglyphsCJK-0.1.1/setup.py
```

### Comparing `HomoglyphsCJK-0.1.0/HomoglyphsCJK/hg_functions.py` & `HomoglyphsCJK-0.1.1/HomoglyphsCJK/hg_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from multiprocess import cpu_count
 from multiprocess import Pool
 # from concurrent.futures import ProcessPoolExecutor as PoolExecutor
 # from .proxy import entry_point
 import numpy as np
 # from numba import njit, types, prange,jit
 # from numba.typed import Dict, List
+import copy
 
 def download_dict(lang):
     '''
     This function is like if it does not exist, then download, otherwise just load from local machine
     '''
     if lang not in ['ko','ja','zhs','zht']:
         raise Exception("language must be specified as ko, ja, zhs or zht")
@@ -113,21 +114,22 @@
         if ele == b: # If any of the ele in a equals b, return 1, after the iter, if nothing returns, just return 0
             return 1
     return 0
 
 def homoglyph_merge(lang, df_1,df_2,key_1,key_2,homo_lambda=1, insertion=1, deletion=1, parallel=False,num_workers=None):
     #cluster_dict = download_dict('ko')
     # Initialize the list 2
-    list2 = df_2[key_2].tolist()
+    df_2_aux = copy.deepcopy(df_2)
+    list2 = df_2_aux[key_2].tolist()
     # key_2 to other variables
-    df_2_columns = df_2.columns.values.tolist()
-    df_2.set_index(key_2,inplace=True)
+    df_2_columns = df_2_aux.columns.values.tolist()
+    df_2_aux.set_index(key_2,inplace=True)
     for df_2_col in df_2_columns:
         if df_2_col!=key_2:
-            globals()['col%s' % df_2_col] = df_2.to_dict()[df_2_col]
+            globals()['col%s' % df_2_col] = df_2_aux.to_dict()[df_2_col]
 
     # Initialize the list 1
     result_list = df_1[key_1].tolist() # The result_list is list 1
     # assert len(list2) == len(result_list)
     list1 = [] # initialize the list1
     for res, truth in zip(result_list,list2):
         res_dict = {}
```

### Comparing `HomoglyphsCJK-0.1.0/HomoglyphsCJK/test_run.py` & `HomoglyphsCJK-0.1.1/HomoglyphsCJK/test_run.py`

 * *Files identical despite different names*

### Comparing `HomoglyphsCJK-0.1.0/HomoglyphsCJK.egg-info/PKG-INFO` & `HomoglyphsCJK-0.1.1/HomoglyphsCJK.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HomoglyphsCJK
-Version: 0.1.0
+Version: 0.1.1
 Summary: An easy Python package for fuzzy matching Chinese(simplified and traditional), Japanese and Korean, using character similarity trained from ViT transformer
 Home-page: https://github.com/dell-research-harvard/HomoglyphsCJK.git
 Author: HomoglyphsCJK Team
 Author-email: homoglyphscjk@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -65,13 +65,16 @@
 download_dict('zhs')
 homoglyph_distance('苏萃乡','小苏莽乡',homo_lambda=1, insertion=1, deletion=1)
 # 1.88
 ```
 ## Contributing
 We encourage you to contribute to HomoglyphsCJK!
 
+## Questions
+If you have any questions using this package, you can open an issue under our [GitHub repository](https://github.com/dell-research-harvard/HomoglyphsCJK/issues). We are maintaining and updating this package, so stay tuned!
+
 ## Citation
 
 Coming Soon
 ```bibtex
 
 ```
```

### Comparing `HomoglyphsCJK-0.1.0/PKG-INFO` & `HomoglyphsCJK-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HomoglyphsCJK
-Version: 0.1.0
+Version: 0.1.1
 Summary: An easy Python package for fuzzy matching Chinese(simplified and traditional), Japanese and Korean, using character similarity trained from ViT transformer
 Home-page: https://github.com/dell-research-harvard/HomoglyphsCJK.git
 Author: HomoglyphsCJK Team
 Author-email: homoglyphscjk@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -65,13 +65,16 @@
 download_dict('zhs')
 homoglyph_distance('苏萃乡','小苏莽乡',homo_lambda=1, insertion=1, deletion=1)
 # 1.88
 ```
 ## Contributing
 We encourage you to contribute to HomoglyphsCJK!
 
+## Questions
+If you have any questions using this package, you can open an issue under our [GitHub repository](https://github.com/dell-research-harvard/HomoglyphsCJK/issues). We are maintaining and updating this package, so stay tuned!
+
 ## Citation
 
 Coming Soon
 ```bibtex
 
 ```
```

### Comparing `HomoglyphsCJK-0.1.0/README.md` & `HomoglyphsCJK-0.1.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -53,13 +53,16 @@
 download_dict('zhs')
 homoglyph_distance('苏萃乡','小苏莽乡',homo_lambda=1, insertion=1, deletion=1)
 # 1.88
 ```
 ## Contributing
 We encourage you to contribute to HomoglyphsCJK!
 
+## Questions
+If you have any questions using this package, you can open an issue under our [GitHub repository](https://github.com/dell-research-harvard/HomoglyphsCJK/issues). We are maintaining and updating this package, so stay tuned!
+
 ## Citation
 
 Coming Soon
 ```bibtex
 
 ```
```

### Comparing `HomoglyphsCJK-0.1.0/setup.py` & `HomoglyphsCJK-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open("README.md","r") as fh:
     long_des = fh.read()
 
 setup(
     name="HomoglyphsCJK",
     packages=["HomoglyphsCJK"],
-    version="0.1.0",
+    version="0.1.1",
     author="HomoglyphsCJK Team",
     author_email="homoglyphscjk@gmail.com",
     description="An easy Python package for fuzzy matching Chinese(simplified and traditional), Japanese and Korean, using character similarity trained from ViT transformer",
     long_description=long_des,
     long_description_content_type="text/markdown",
     url="https://github.com/dell-research-harvard/HomoglyphsCJK.git",
     classifiers=[
```

