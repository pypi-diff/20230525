# Comparing `tmp/light_size_constrained_clustering-0.0.3.tar.gz` & `tmp/light_size_constrained_clustering-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "light_size_constrained_clustering-0.0.3.tar", last modified: Wed May 24 21:05:34 2023, max compression
+gzip compressed data, was "light_size_constrained_clustering-0.0.4.tar", last modified: Thu May 25 13:21:46 2023, max compression
```

## Comparing `light_size_constrained_clustering-0.0.3.tar` & `light_size_constrained_clustering-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 i0365030   (502) staff       (20)        0 2023-05-24 21:05:34.964714 light_size_constrained_clustering-0.0.3/
--rw-r--r--   0 i0365030   (502) staff       (20)     1074 2023-05-24 18:28:58.000000 light_size_constrained_clustering-0.0.3/LICENSE
--rw-r--r--   0 i0365030   (502) staff       (20)     3528 2023-05-24 21:05:34.964560 light_size_constrained_clustering-0.0.3/PKG-INFO
--rw-r--r--   0 i0365030   (502) staff       (20)     3181 2023-05-24 21:03:08.000000 light_size_constrained_clustering-0.0.3/README.md
-drwxr-xr-x   0 i0365030   (502) staff       (20)        0 2023-05-24 21:05:34.963259 light_size_constrained_clustering-0.0.3/light_size_constrained_clustering/
--rw-r--r--   0 i0365030   (502) staff       (20)      106 2023-05-24 20:33:58.000000 light_size_constrained_clustering-0.0.3/light_size_constrained_clustering/__init__.py
--rw-r--r--   0 i0365030   (502) staff       (20)     6178 2023-05-24 20:40:01.000000 light_size_constrained_clustering-0.0.3/light_size_constrained_clustering/base.py
--rw-r--r--   0 i0365030   (502) staff       (20)     6668 2023-05-24 20:18:18.000000 light_size_constrained_clustering-0.0.3/light_size_constrained_clustering/da.py
-drwxr-xr-x   0 i0365030   (502) staff       (20)        0 2023-05-24 21:05:34.964061 light_size_constrained_clustering-0.0.3/light_size_constrained_clustering.egg-info/
--rw-r--r--   0 i0365030   (502) staff       (20)     3528 2023-05-24 21:05:34.000000 light_size_constrained_clustering-0.0.3/light_size_constrained_clustering.egg-info/PKG-INFO
--rw-r--r--   0 i0365030   (502) staff       (20)      455 2023-05-24 21:05:34.000000 light_size_constrained_clustering-0.0.3/light_size_constrained_clustering.egg-info/SOURCES.txt
--rw-r--r--   0 i0365030   (502) staff       (20)        1 2023-05-24 21:05:34.000000 light_size_constrained_clustering-0.0.3/light_size_constrained_clustering.egg-info/dependency_links.txt
--rw-r--r--   0 i0365030   (502) staff       (20)      106 2023-05-24 21:05:34.000000 light_size_constrained_clustering-0.0.3/light_size_constrained_clustering.egg-info/requires.txt
--rw-r--r--   0 i0365030   (502) staff       (20)       34 2023-05-24 21:05:34.000000 light_size_constrained_clustering-0.0.3/light_size_constrained_clustering.egg-info/top_level.txt
--rw-r--r--   0 i0365030   (502) staff       (20)       38 2023-05-24 21:05:34.964757 light_size_constrained_clustering-0.0.3/setup.cfg
--rw-r--r--   0 i0365030   (502) staff       (20)     1312 2023-05-24 21:05:00.000000 light_size_constrained_clustering-0.0.3/setup.py
-drwxr-xr-x   0 i0365030   (502) staff       (20)        0 2023-05-24 21:05:34.964210 light_size_constrained_clustering-0.0.3/tests/
--rw-r--r--   0 i0365030   (502) staff       (20)     1341 2023-05-24 20:41:53.000000 light_size_constrained_clustering-0.0.3/tests/test_da.py
+drwxr-xr-x   0 i0365030   (502) staff       (20)        0 2023-05-25 13:21:46.473019 light_size_constrained_clustering-0.0.4/
+-rw-r--r--   0 i0365030   (502) staff       (20)     1074 2023-05-24 18:28:58.000000 light_size_constrained_clustering-0.0.4/LICENSE
+-rw-r--r--   0 i0365030   (502) staff       (20)     3439 2023-05-25 13:21:46.472885 light_size_constrained_clustering-0.0.4/PKG-INFO
+-rw-r--r--   0 i0365030   (502) staff       (20)     3092 2023-05-24 21:10:13.000000 light_size_constrained_clustering-0.0.4/README.md
+drwxr-xr-x   0 i0365030   (502) staff       (20)        0 2023-05-25 13:21:46.471785 light_size_constrained_clustering-0.0.4/light_size_constrained_clustering/
+-rw-r--r--   0 i0365030   (502) staff       (20)      106 2023-05-24 20:33:58.000000 light_size_constrained_clustering-0.0.4/light_size_constrained_clustering/__init__.py
+-rw-r--r--   0 i0365030   (502) staff       (20)     6178 2023-05-24 20:40:01.000000 light_size_constrained_clustering-0.0.4/light_size_constrained_clustering/base.py
+-rw-r--r--   0 i0365030   (502) staff       (20)     6668 2023-05-24 20:18:18.000000 light_size_constrained_clustering-0.0.4/light_size_constrained_clustering/da.py
+drwxr-xr-x   0 i0365030   (502) staff       (20)        0 2023-05-25 13:21:46.472506 light_size_constrained_clustering-0.0.4/light_size_constrained_clustering.egg-info/
+-rw-r--r--   0 i0365030   (502) staff       (20)     3439 2023-05-25 13:21:46.000000 light_size_constrained_clustering-0.0.4/light_size_constrained_clustering.egg-info/PKG-INFO
+-rw-r--r--   0 i0365030   (502) staff       (20)      455 2023-05-25 13:21:46.000000 light_size_constrained_clustering-0.0.4/light_size_constrained_clustering.egg-info/SOURCES.txt
+-rw-r--r--   0 i0365030   (502) staff       (20)        1 2023-05-25 13:21:46.000000 light_size_constrained_clustering-0.0.4/light_size_constrained_clustering.egg-info/dependency_links.txt
+-rw-r--r--   0 i0365030   (502) staff       (20)      106 2023-05-25 13:21:46.000000 light_size_constrained_clustering-0.0.4/light_size_constrained_clustering.egg-info/requires.txt
+-rw-r--r--   0 i0365030   (502) staff       (20)       34 2023-05-25 13:21:46.000000 light_size_constrained_clustering-0.0.4/light_size_constrained_clustering.egg-info/top_level.txt
+-rw-r--r--   0 i0365030   (502) staff       (20)       38 2023-05-25 13:21:46.473055 light_size_constrained_clustering-0.0.4/setup.cfg
+-rw-r--r--   0 i0365030   (502) staff       (20)     1140 2023-05-25 13:21:30.000000 light_size_constrained_clustering-0.0.4/setup.py
+drwxr-xr-x   0 i0365030   (502) staff       (20)        0 2023-05-25 13:21:46.472663 light_size_constrained_clustering-0.0.4/tests/
+-rw-r--r--   0 i0365030   (502) staff       (20)     1341 2023-05-24 20:41:53.000000 light_size_constrained_clustering-0.0.4/tests/test_da.py
```

### Comparing `light_size_constrained_clustering-0.0.3/LICENSE` & `light_size_constrained_clustering-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `light_size_constrained_clustering-0.0.3/PKG-INFO` & `light_size_constrained_clustering-0.0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: light_size_constrained_clustering
-Version: 0.0.3
+Version: 0.0.4
 Summary: Size Constrained Clustering solver
 Home-page: https://github.com/AlbertPlaPlanas/size_constrained_clustering
 Author: Albert Pla
 Author-email: plaalbert@gmail.com
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -53,15 +53,15 @@
 print("Labels:")
 print(labels)
 print("Elements in cluster 0: ", np.count_nonzero(labels == 0))
 print("Elements in cluster 1: ", np.count_nonzero(labels == 1))
 print("Elements in cluster 2: ", np.count_nonzero(labels == 2))
 print("Elements in cluster 3: ", np.count_nonzero(labels == 3))
 ```
-![alt text](https://github.com/jingw2/size_constrained_clustering/blob/master/pic/da.png)
+
 
 Cluster size: 1200, 600 and 200 in the figure above, corresponding to distribution [0.6, 0.3, 0.1]
 
 
 ## Copyright
 Copyright (c) 2023 Jing Wang & Albert Pla. Released under the MIT License.
```

### Comparing `light_size_constrained_clustering-0.0.3/README.md` & `light_size_constrained_clustering-0.0.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 print("Labels:")
 print(labels)
 print("Elements in cluster 0: ", np.count_nonzero(labels == 0))
 print("Elements in cluster 1: ", np.count_nonzero(labels == 1))
 print("Elements in cluster 2: ", np.count_nonzero(labels == 2))
 print("Elements in cluster 3: ", np.count_nonzero(labels == 3))
 ```
-![alt text](https://github.com/jingw2/size_constrained_clustering/blob/master/pic/da.png)
+
 
 Cluster size: 1200, 600 and 200 in the figure above, corresponding to distribution [0.6, 0.3, 0.1]
 
 
 ## Copyright
 Copyright (c) 2023 Jing Wang & Albert Pla. Released under the MIT License.
```

### Comparing `light_size_constrained_clustering-0.0.3/light_size_constrained_clustering/base.py` & `light_size_constrained_clustering-0.0.4/light_size_constrained_clustering/base.py`

 * *Files identical despite different names*

### Comparing `light_size_constrained_clustering-0.0.3/light_size_constrained_clustering/da.py` & `light_size_constrained_clustering-0.0.4/light_size_constrained_clustering/da.py`

 * *Files identical despite different names*

### Comparing `light_size_constrained_clustering-0.0.3/light_size_constrained_clustering.egg-info/PKG-INFO` & `light_size_constrained_clustering-0.0.4/light_size_constrained_clustering.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: light-size-constrained-clustering
-Version: 0.0.3
+Version: 0.0.4
 Summary: Size Constrained Clustering solver
 Home-page: https://github.com/AlbertPlaPlanas/size_constrained_clustering
 Author: Albert Pla
 Author-email: plaalbert@gmail.com
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -53,15 +53,15 @@
 print("Labels:")
 print(labels)
 print("Elements in cluster 0: ", np.count_nonzero(labels == 0))
 print("Elements in cluster 1: ", np.count_nonzero(labels == 1))
 print("Elements in cluster 2: ", np.count_nonzero(labels == 2))
 print("Elements in cluster 3: ", np.count_nonzero(labels == 3))
 ```
-![alt text](https://github.com/jingw2/size_constrained_clustering/blob/master/pic/da.png)
+
 
 Cluster size: 1200, 600 and 200 in the figure above, corresponding to distribution [0.6, 0.3, 0.1]
 
 
 ## Copyright
 Copyright (c) 2023 Jing Wang & Albert Pla. Released under the MIT License.
```

### Comparing `light_size_constrained_clustering-0.0.3/setup.py` & `light_size_constrained_clustering-0.0.4/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,31 +10,21 @@
 
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 dist.Distribution().fetch_build_eggs(["numpy>=1.13"])
 
-
-try:
-    from numpy import get_include
-except:
-    def get_include():
-        # Defer import to later
-        from numpy import get_include
-
-        return get_include()
-
 path = os.path.dirname(os.path.abspath(__file__))
 
 with open(os.path.join(path, "requirements.txt")) as fp:
     install_requires = fp.read().strip().split("\n")
 
 
-VERSION = "0.0.3"
+VERSION = "0.0.4"
 LICENSE = "MIT"
 setup(
     #ext_modules=extensions,
     version=VERSION,
     setup_requires=["numpy"],
     install_requires=install_requires,
     name="light_size_constrained_clustering",
```

### Comparing `light_size_constrained_clustering-0.0.3/tests/test_da.py` & `light_size_constrained_clustering-0.0.4/tests/test_da.py`

 * *Files identical despite different names*

