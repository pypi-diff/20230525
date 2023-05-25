# Comparing `tmp/PyXAB-0.2.1.tar.gz` & `tmp/PyXAB-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/PyXAB-0.2.1.tar", last modified: Wed Apr 26 03:18:03 2023, max compression
+gzip compressed data, was "dist/PyXAB-0.2.2.tar", last modified: Thu May 25 00:38:32 2023, max compression
```

## Comparing `PyXAB-0.2.1.tar` & `PyXAB-0.2.2.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 william    (501) staff       (20)        0 2023-04-26 03:18:03.051119 PyXAB-0.2.1/
--rw-r--r--   0 william    (501) staff       (20)     1066 2022-03-24 15:30:00.000000 PyXAB-0.2.1/LICENSE
--rw-r--r--   0 william    (501) staff       (20)    15987 2023-04-26 03:18:03.051351 PyXAB-0.2.1/PKG-INFO
-drwxr-xr-x   0 william    (501) staff       (20)        0 2023-04-26 03:18:03.031588 PyXAB-0.2.1/PyXAB/
--rw-r--r--   0 william    (501) staff       (20)        0 2022-03-22 23:40:33.000000 PyXAB-0.2.1/PyXAB/__init__.py
-drwxr-xr-x   0 william    (501) staff       (20)        0 2023-04-26 03:18:03.038325 PyXAB-0.2.1/PyXAB/algos/
--rw-r--r--   0 william    (501) staff       (20)     1415 2023-04-26 03:17:41.000000 PyXAB-0.2.1/PyXAB/algos/Algo.py
--rw-r--r--   0 william    (501) staff       (20)     6130 2023-04-26 03:17:41.000000 PyXAB-0.2.1/PyXAB/algos/DOO.py
--rw-r--r--   0 william    (501) staff       (20)     5335 2023-04-26 03:17:41.000000 PyXAB-0.2.1/PyXAB/algos/GPO.py
--rw-r--r--   0 william    (501) staff       (20)    10126 2023-04-26 03:17:41.000000 PyXAB-0.2.1/PyXAB/algos/HCT.py
--rw-r--r--   0 william    (501) staff       (20)     8909 2023-04-26 03:17:41.000000 PyXAB-0.2.1/PyXAB/algos/HOO.py
--rw-r--r--   0 william    (501) staff       (20)     2358 2023-04-26 03:17:41.000000 PyXAB-0.2.1/PyXAB/algos/PCT.py
--rw-r--r--   0 william    (501) staff       (20)     5670 2023-04-26 03:17:41.000000 PyXAB-0.2.1/PyXAB/algos/POO.py
--rw-r--r--   0 william    (501) staff       (20)     5390 2023-04-26 03:17:41.000000 PyXAB-0.2.1/PyXAB/algos/SOO.py
--rw-r--r--   0 william    (501) staff       (20)     7170 2023-04-26 03:17:41.000000 PyXAB-0.2.1/PyXAB/algos/SequOOL.py
--rw-r--r--   0 william    (501) staff       (20)     7337 2023-03-13 03:58:11.000000 PyXAB-0.2.1/PyXAB/algos/StoSOO.py
--rw-r--r--   0 william    (501) staff       (20)    10994 2023-04-26 03:17:41.000000 PyXAB-0.2.1/PyXAB/algos/StroquOOL.py
--rw-r--r--   0 william    (501) staff       (20)    11938 2023-04-26 03:17:41.000000 PyXAB-0.2.1/PyXAB/algos/VHCT.py
--rw-r--r--   0 william    (501) staff       (20)     2360 2023-04-26 03:17:41.000000 PyXAB-0.2.1/PyXAB/algos/VPCT.py
--rw-r--r--   0 william    (501) staff       (20)     5218 2023-04-26 03:17:41.000000 PyXAB-0.2.1/PyXAB/algos/Zooming.py
--rw-r--r--   0 william    (501) staff       (20)      331 2023-04-26 03:17:41.000000 PyXAB-0.2.1/PyXAB/algos/__init__.py
-drwxr-xr-x   0 william    (501) staff       (20)        0 2023-04-26 03:18:03.043475 PyXAB-0.2.1/PyXAB/partition/
--rw-r--r--   0 william    (501) staff       (20)     2806 2023-03-13 03:58:11.000000 PyXAB-0.2.1/PyXAB/partition/BinaryPartition.py
--rw-r--r--   0 william    (501) staff       (20)     3131 2023-03-13 03:58:11.000000 PyXAB-0.2.1/PyXAB/partition/DimensionBinaryPartition.py
--rw-r--r--   0 william    (501) staff       (20)     2807 2023-03-13 03:58:11.000000 PyXAB-0.2.1/PyXAB/partition/KaryPartition.py
--rw-r--r--   0 william    (501) staff       (20)     2298 2023-02-16 03:14:10.000000 PyXAB-0.2.1/PyXAB/partition/Node.py
--rw-r--r--   0 william    (501) staff       (20)     3019 2023-03-13 03:58:11.000000 PyXAB-0.2.1/PyXAB/partition/Partition.py
--rw-r--r--   0 william    (501) staff       (20)     2861 2023-03-13 03:58:11.000000 PyXAB-0.2.1/PyXAB/partition/RandomBinaryPartition.py
--rw-r--r--   0 william    (501) staff       (20)     3068 2023-03-13 03:58:11.000000 PyXAB-0.2.1/PyXAB/partition/RandomKaryPartition.py
--rw-r--r--   0 william    (501) staff       (20)       83 2023-03-13 03:58:11.000000 PyXAB-0.2.1/PyXAB/partition/__init__.py
-drwxr-xr-x   0 william    (501) staff       (20)        0 2023-04-26 03:18:03.048445 PyXAB-0.2.1/PyXAB/synthetic_obj/
--rw-r--r--   0 william    (501) staff       (20)     2534 2023-03-13 03:58:11.000000 PyXAB-0.2.1/PyXAB/synthetic_obj/Ackley.py
--rw-r--r--   0 william    (501) staff       (20)     1027 2023-03-13 03:58:11.000000 PyXAB-0.2.1/PyXAB/synthetic_obj/Cexample.py
--rw-r--r--   0 william    (501) staff       (20)     1224 2023-03-13 03:58:11.000000 PyXAB-0.2.1/PyXAB/synthetic_obj/DifficultFunc.py
--rw-r--r--   0 william    (501) staff       (20)     4145 2023-03-13 03:58:11.000000 PyXAB-0.2.1/PyXAB/synthetic_obj/DoubleSine.py
--rw-r--r--   0 william    (501) staff       (20)     2118 2023-03-13 03:58:11.000000 PyXAB-0.2.1/PyXAB/synthetic_obj/Garland.py
--rw-r--r--   0 william    (501) staff       (20)     2095 2023-03-13 03:58:11.000000 PyXAB-0.2.1/PyXAB/synthetic_obj/Himmelblau.py
--rw-r--r--   0 william    (501) staff       (20)      484 2023-02-16 02:41:47.000000 PyXAB-0.2.1/PyXAB/synthetic_obj/Objective.py
--rw-r--r--   0 william    (501) staff       (20)     2116 2023-03-13 03:58:11.000000 PyXAB-0.2.1/PyXAB/synthetic_obj/Rastrigin.py
--rw-r--r--   0 william    (501) staff       (20)      380 2023-02-16 02:41:47.000000 PyXAB-0.2.1/PyXAB/synthetic_obj/__init__.py
-drwxr-xr-x   0 william    (501) staff       (20)        0 2023-04-26 03:18:03.050511 PyXAB-0.2.1/PyXAB/utils/
--rw-r--r--   0 william    (501) staff       (20)        0 2022-03-22 23:40:33.000000 PyXAB-0.2.1/PyXAB/utils/__init__.py
--rw-r--r--   0 william    (501) staff       (20)     1467 2023-02-16 03:14:10.000000 PyXAB-0.2.1/PyXAB/utils/plot.py
--rw-r--r--   0 william    (501) staff       (20)     2477 2023-04-26 03:17:41.000000 PyXAB-0.2.1/PyXAB/utils/run_synthetic.py
--rw-r--r--   0 william    (501) staff       (20)     4350 2023-03-13 03:58:11.000000 PyXAB-0.2.1/PyXAB/utils/visualize_gif.py
-drwxr-xr-x   0 william    (501) staff       (20)        0 2023-04-26 03:18:03.032963 PyXAB-0.2.1/PyXAB.egg-info/
--rw-r--r--   0 william    (501) staff       (20)    15987 2023-04-26 03:18:02.000000 PyXAB-0.2.1/PyXAB.egg-info/PKG-INFO
--rw-r--r--   0 william    (501) staff       (20)     1179 2023-04-26 03:18:02.000000 PyXAB-0.2.1/PyXAB.egg-info/SOURCES.txt
--rw-r--r--   0 william    (501) staff       (20)        1 2023-04-26 03:18:02.000000 PyXAB-0.2.1/PyXAB.egg-info/dependency_links.txt
--rw-r--r--   0 william    (501) staff       (20)       25 2023-04-26 03:18:02.000000 PyXAB-0.2.1/PyXAB.egg-info/requires.txt
--rw-r--r--   0 william    (501) staff       (20)        6 2023-04-26 03:18:02.000000 PyXAB-0.2.1/PyXAB.egg-info/top_level.txt
--rw-r--r--   0 william    (501) staff       (20)    13664 2023-04-26 03:17:41.000000 PyXAB-0.2.1/README.md
--rw-r--r--   0 william    (501) staff       (20)      103 2023-04-26 03:18:03.051821 PyXAB-0.2.1/setup.cfg
--rw-r--r--   0 william    (501) staff       (20)     3881 2023-04-26 03:17:54.000000 PyXAB-0.2.1/setup.py
+drwxr-xr-x   0 william    (501) staff       (20)        0 2023-05-25 00:38:32.396742 PyXAB-0.2.2/
+-rw-r--r--   0 william    (501) staff       (20)     1066 2022-03-24 15:30:00.000000 PyXAB-0.2.2/LICENSE
+-rw-r--r--   0 william    (501) staff       (20)    16395 2023-05-25 00:38:32.397036 PyXAB-0.2.2/PKG-INFO
+drwxr-xr-x   0 william    (501) staff       (20)        0 2023-05-25 00:38:32.370209 PyXAB-0.2.2/PyXAB/
+-rw-r--r--   0 william    (501) staff       (20)        0 2022-03-22 23:40:33.000000 PyXAB-0.2.2/PyXAB/__init__.py
+drwxr-xr-x   0 william    (501) staff       (20)        0 2023-05-25 00:38:32.380143 PyXAB-0.2.2/PyXAB/algos/
+-rw-r--r--   0 william    (501) staff       (20)     1415 2023-05-24 05:55:11.000000 PyXAB-0.2.2/PyXAB/algos/Algo.py
+-rw-r--r--   0 william    (501) staff       (20)     6201 2023-05-24 05:55:19.000000 PyXAB-0.2.2/PyXAB/algos/DOO.py
+-rw-r--r--   0 william    (501) staff       (20)     5406 2023-05-24 05:55:19.000000 PyXAB-0.2.2/PyXAB/algos/GPO.py
+-rw-r--r--   0 william    (501) staff       (20)    10197 2023-05-24 05:55:19.000000 PyXAB-0.2.2/PyXAB/algos/HCT.py
+-rw-r--r--   0 william    (501) staff       (20)     8980 2023-05-24 05:55:19.000000 PyXAB-0.2.2/PyXAB/algos/HOO.py
+-rw-r--r--   0 william    (501) staff       (20)     2428 2023-05-24 05:55:19.000000 PyXAB-0.2.2/PyXAB/algos/PCT.py
+-rw-r--r--   0 william    (501) staff       (20)     5740 2023-05-24 05:55:19.000000 PyXAB-0.2.2/PyXAB/algos/POO.py
+-rw-r--r--   0 william    (501) staff       (20)     5461 2023-05-24 05:55:19.000000 PyXAB-0.2.2/PyXAB/algos/SOO.py
+-rw-r--r--   0 william    (501) staff       (20)     7241 2023-05-24 05:55:19.000000 PyXAB-0.2.2/PyXAB/algos/SequOOL.py
+-rw-r--r--   0 william    (501) staff       (20)     7408 2023-05-24 05:55:19.000000 PyXAB-0.2.2/PyXAB/algos/StoSOO.py
+-rw-r--r--   0 william    (501) staff       (20)    11065 2023-05-24 05:55:19.000000 PyXAB-0.2.2/PyXAB/algos/StroquOOL.py
+-rw-r--r--   0 william    (501) staff       (20)    12008 2023-05-24 05:55:19.000000 PyXAB-0.2.2/PyXAB/algos/VHCT.py
+-rw-r--r--   0 william    (501) staff       (20)     2430 2023-05-24 05:55:19.000000 PyXAB-0.2.2/PyXAB/algos/VPCT.py
+-rw-r--r--   0 william    (501) staff       (20)     5288 2023-05-24 05:55:19.000000 PyXAB-0.2.2/PyXAB/algos/Zooming.py
+-rw-r--r--   0 william    (501) staff       (20)      331 2023-05-24 05:55:11.000000 PyXAB-0.2.2/PyXAB/algos/__init__.py
+drwxr-xr-x   0 william    (501) staff       (20)        0 2023-05-25 00:38:32.385873 PyXAB-0.2.2/PyXAB/partition/
+-rw-r--r--   0 william    (501) staff       (20)     2806 2023-03-13 03:58:11.000000 PyXAB-0.2.2/PyXAB/partition/BinaryPartition.py
+-rw-r--r--   0 william    (501) staff       (20)     3131 2023-03-13 03:58:11.000000 PyXAB-0.2.2/PyXAB/partition/DimensionBinaryPartition.py
+-rw-r--r--   0 william    (501) staff       (20)     2807 2023-03-13 03:58:11.000000 PyXAB-0.2.2/PyXAB/partition/KaryPartition.py
+-rw-r--r--   0 william    (501) staff       (20)     2298 2023-02-16 03:14:10.000000 PyXAB-0.2.2/PyXAB/partition/Node.py
+-rw-r--r--   0 william    (501) staff       (20)     3019 2023-03-13 03:58:11.000000 PyXAB-0.2.2/PyXAB/partition/Partition.py
+-rw-r--r--   0 william    (501) staff       (20)     2861 2023-03-13 03:58:11.000000 PyXAB-0.2.2/PyXAB/partition/RandomBinaryPartition.py
+-rw-r--r--   0 william    (501) staff       (20)     3068 2023-03-13 03:58:11.000000 PyXAB-0.2.2/PyXAB/partition/RandomKaryPartition.py
+-rw-r--r--   0 william    (501) staff       (20)       83 2023-03-13 03:58:11.000000 PyXAB-0.2.2/PyXAB/partition/__init__.py
+drwxr-xr-x   0 william    (501) staff       (20)        0 2023-05-25 00:38:32.393239 PyXAB-0.2.2/PyXAB/synthetic_obj/
+-rw-r--r--   0 william    (501) staff       (20)     2534 2023-03-13 03:58:11.000000 PyXAB-0.2.2/PyXAB/synthetic_obj/Ackley.py
+-rw-r--r--   0 william    (501) staff       (20)     1027 2023-03-13 03:58:11.000000 PyXAB-0.2.2/PyXAB/synthetic_obj/Cexample.py
+-rw-r--r--   0 william    (501) staff       (20)     1224 2023-03-13 03:58:11.000000 PyXAB-0.2.2/PyXAB/synthetic_obj/DifficultFunc.py
+-rw-r--r--   0 william    (501) staff       (20)     4145 2023-03-13 03:58:11.000000 PyXAB-0.2.2/PyXAB/synthetic_obj/DoubleSine.py
+-rw-r--r--   0 william    (501) staff       (20)     2118 2023-03-13 03:58:11.000000 PyXAB-0.2.2/PyXAB/synthetic_obj/Garland.py
+-rw-r--r--   0 william    (501) staff       (20)     2095 2023-03-13 03:58:11.000000 PyXAB-0.2.2/PyXAB/synthetic_obj/Himmelblau.py
+-rw-r--r--   0 william    (501) staff       (20)      484 2023-02-16 02:41:47.000000 PyXAB-0.2.2/PyXAB/synthetic_obj/Objective.py
+-rw-r--r--   0 william    (501) staff       (20)     2116 2023-03-13 03:58:11.000000 PyXAB-0.2.2/PyXAB/synthetic_obj/Rastrigin.py
+-rw-r--r--   0 william    (501) staff       (20)      380 2023-02-16 02:41:47.000000 PyXAB-0.2.2/PyXAB/synthetic_obj/__init__.py
+drwxr-xr-x   0 william    (501) staff       (20)        0 2023-05-25 00:38:32.395729 PyXAB-0.2.2/PyXAB/utils/
+-rw-r--r--   0 william    (501) staff       (20)        0 2022-03-22 23:40:33.000000 PyXAB-0.2.2/PyXAB/utils/__init__.py
+-rw-r--r--   0 william    (501) staff       (20)     1467 2023-02-16 03:14:10.000000 PyXAB-0.2.2/PyXAB/utils/plot.py
+-rw-r--r--   0 william    (501) staff       (20)     2477 2023-05-24 05:55:11.000000 PyXAB-0.2.2/PyXAB/utils/run_synthetic.py
+-rw-r--r--   0 william    (501) staff       (20)     4350 2023-03-13 03:58:11.000000 PyXAB-0.2.2/PyXAB/utils/visualize_gif.py
+drwxr-xr-x   0 william    (501) staff       (20)        0 2023-05-25 00:38:32.371773 PyXAB-0.2.2/PyXAB.egg-info/
+-rw-r--r--   0 william    (501) staff       (20)    16395 2023-05-25 00:38:32.000000 PyXAB-0.2.2/PyXAB.egg-info/PKG-INFO
+-rw-r--r--   0 william    (501) staff       (20)     1179 2023-05-25 00:38:32.000000 PyXAB-0.2.2/PyXAB.egg-info/SOURCES.txt
+-rw-r--r--   0 william    (501) staff       (20)        1 2023-05-25 00:38:32.000000 PyXAB-0.2.2/PyXAB.egg-info/dependency_links.txt
+-rw-r--r--   0 william    (501) staff       (20)       25 2023-05-25 00:38:32.000000 PyXAB-0.2.2/PyXAB.egg-info/requires.txt
+-rw-r--r--   0 william    (501) staff       (20)        6 2023-05-25 00:38:32.000000 PyXAB-0.2.2/PyXAB.egg-info/top_level.txt
+-rw-r--r--   0 william    (501) staff       (20)    14056 2023-05-25 00:37:31.000000 PyXAB-0.2.2/README.md
+-rw-r--r--   0 william    (501) staff       (20)      103 2023-05-25 00:38:32.397677 PyXAB-0.2.2/setup.cfg
+-rw-r--r--   0 william    (501) staff       (20)     3881 2023-05-24 05:55:19.000000 PyXAB-0.2.2/setup.py
```

### Comparing `PyXAB-0.2.1/LICENSE` & `PyXAB-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `PyXAB-0.2.1/PKG-INFO` & `PyXAB-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyXAB
-Version: 0.2.1
+Version: 0.2.2
 Summary: PyXAB - A Python Library for X-Armed Bandit and Online Blackbox Optimization Algorithms.
 Home-page: https://github.com/WilliamLwj/PyXAB
 Author: Wenjie Li, Haoze Li
 Author-email: lil3549@purdue.edu
 License: MIT
 Description: 
         
@@ -50,58 +50,60 @@
         
         
         <p align='center'>
           <img src="https://raw.githubusercontent.com/WilliamLwj/PyXAB/main/figs/HCT_trajectory.gif" alt="trajectory" width="48%"/>  
           <img src="https://raw.githubusercontent.com/WilliamLwj/PyXAB/main/figs/HCT_heatmap.gif" alt="heatmap" width="48%"/>  
         </p>
         
-        PyXAB includes implementations of different *X*-armed bandit algorithms, including the classic ones such as [HOO (Bubeck et al., 2011)](https://jmlr.org/papers/v12/bubeck11a.html), 
+        PyXAB contains the implementations of **more than 10 optimization algorithms**, including the classic ones such as [HOO (Bubeck et al., 2011)](https://jmlr.org/papers/v12/bubeck11a.html), 
          [StoSOO (Valko et al., 2013)](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/StoSOO.py), and [HCT (Azar et al., 2014)](https://proceedings.mlr.press/v32/azar14.html), and the most
-        recent works such as [GPO (Shang et al., 2019)](https://proceedings.mlr.press/v98/xuedong19a.html) and [VHCT (Li et al, 2021)](https://arxiv.org/abs/2106.09215).
+        recent works such as [GPO (Shang et al., 2019)](https://proceedings.mlr.press/v98/xuedong19a.html), [StroquOOL  (Bartlett et al.,2019)](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/StroquOOL.py) and [VHCT (Li et al, 2021)](https://arxiv.org/abs/2106.09215).
         PyXAB also provides the most commonly-used synthetic objectives to evaluate the performance of different algorithms and the implementations for different hierarchical partitions
         
+        **The algorithms are maximization algorithms!**
         
         ## Quick Links
         
         - [Quick Example](#Quick-Example)
         - [Documentations](#Documentations)
         - [Installation](#Installation)
         - [Features](#Features)
           * [*X*-armed bandit algorithms](#Stochastic-X-armed-bandit-algorithms)
           * [Hierarchical partition ](#Hierarchical-partition)
           * [Synthetic objectives](#Synthetic-objectives)
         - [Contributing](#Contributing)
         - [Citations](#Citations)
         
         ## Quick Example
-        First define the blackbox objective, the parameter domain, the partition of the space, and the algorithm, e.g.
+        PyXAB follows a natural and straightforward API design completely aligned with the online blackbox
+        optimization paradigm. The following is a simple 6-line usage example.
         
-        ```python3
-        target = Garland()
-        domain = [[0, 1]]
-        partition = BinaryPartition
-        algo = T_HOO(rounds=1000, domain=domain, partition=partition)
+        First, we define the parameter domain and the algorithm to run. 
+        At every round  `t`, call `algo.pull(t)` to get a point and call 
+        `algo.receive_reward(t, reward)` to give the algorithm the objective evaluation (reward)
         ```
         
-        At every round  `t`, call `algo.pull(t)` to get a point. After receiving the (stochastic) reward for the point, call 
-        `algo.receive_reward(t, reward)` to give the algorithm the feedback
-        
         ```python3
-        point = algo.pull(t)
-        reward = target.f(point) + np.random.uniform(-0.1, 0.1) # Uniform noise example
-        algo.receive_reward(t, reward)
+        domain = [[0, 1]]               # Parameter is 1-D and between 0 and 1
+        algo = T_HOO(rounds=1000, domain=domain) 
+        for t in range(1000):
+            point = algo.pull(t)
+            reward = 1                  #TODO: User-defined objective returns the reward
+            algo.receive_reward(t, reward)
         ```
         
+        More detailed examples can be found [here](https://pyxab.readthedocs.io/en/latest/getting_started/auto_examples/index.html)
+        
         ## Documentations
         
           * The most up-to-date [documentations](https://pyxab.readthedocs.io/) 
         
           * The [roadmap](https://github.com/users/WilliamLwj/projects/1) for our project    
           
-          * Our [paper](https://arxiv.org/abs/2303.04030) for the library
+          * Our [manuscript](https://arxiv.org/abs/2303.04030) for the library
         
         ## Installation
         
         To install via pip, run the following lines of code
         ```bash
         pip install PyXAB                 # normal install
         pip install --upgrade PyXAB       # or update if needed
```

#### html2text {}

```diff
@@ -1,75 +1,81 @@
-Metadata-Version: 2.1 Name: PyXAB Version: 0.2.1 Summary: PyXAB - A Python
+Metadata-Version: 2.1 Name: PyXAB Version: 0.2.2 Summary: PyXAB - A Python
 Library for X-Armed Bandit and Online Blackbox Optimization Algorithms. Home-
 page: https://github.com/WilliamLwj/PyXAB Author: Wenjie Li, Haoze Li Author-
 email: lil3549@purdue.edu License: MIT Description: # PyXAB - Python *X*-Armed
 Bandit
 [PyPI_version] [https://codecov.io/gh/WilliamLwj/PyXAB/branch/main/graph/
 badge.svg?token=VACRX9AQBM] [Documentation_Status] [Code_style:_black]
 [testing] [github-PyXAB_forks] [github-PyXAB_stars] [downloads] [github-PyXAB
 license] [Code_style:_black]
 PyXAB is a Python open-source library for *X*-armed bandit algorithms, a
 prestigious set of optimizers for online black-box optimization, i.e., optimize
 an objective without gradients, also known as the continuous-arm bandit (CAB),
 Lipschitz bandit, global optimization (GO) and bandit-based black-box
 optimization problems.
                             [trajectory] [heatmap]
-PyXAB includes implementations of different *X*-armed bandit algorithms,
+PyXAB contains the implementations of **more than 10 optimization algorithms**,
 including the classic ones such as [HOO (Bubeck et al., 2011)](https://
 jmlr.org/papers/v12/bubeck11a.html), [StoSOO (Valko et al., 2013)](https://
 github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/StoSOO.py), and [HCT (Azar et
 al., 2014)](https://proceedings.mlr.press/v32/azar14.html), and the most recent
 works such as [GPO (Shang et al., 2019)](https://proceedings.mlr.press/v98/
-xuedong19a.html) and [VHCT (Li et al, 2021)](https://arxiv.org/abs/2106.09215).
-PyXAB also provides the most commonly-used synthetic objectives to evaluate the
-performance of different algorithms and the implementations for different
-hierarchical partitions ## Quick Links - [Quick Example](#Quick-Example) -
-[Documentations](#Documentations) - [Installation](#Installation) - [Features]
-(#Features) * [*X*-armed bandit algorithms](#Stochastic-X-armed-bandit-
-algorithms) * [Hierarchical partition ](#Hierarchical-partition) * [Synthetic
-objectives](#Synthetic-objectives) - [Contributing](#Contributing) -
-[Citations](#Citations) ## Quick Example First define the blackbox objective,
-the parameter domain, the partition of the space, and the algorithm, e.g.
-```python3 target = Garland() domain = [[0, 1]] partition = BinaryPartition
-algo = T_HOO(rounds=1000, domain=domain, partition=partition) ``` At every
-round `t`, call `algo.pull(t)` to get a point. After receiving the (stochastic)
-reward for the point, call `algo.receive_reward(t, reward)` to give the
-algorithm the feedback ```python3 point = algo.pull(t) reward = target.f(point)
-+ np.random.uniform(-0.1, 0.1) # Uniform noise example algo.receive_reward(t,
-reward) ``` ## Documentations * The most up-to-date [documentations](https://
+xuedong19a.html), [StroquOOL (Bartlett et al.,2019)](https://github.com/
+WilliamLwj/PyXAB/blob/main/PyXAB/algos/StroquOOL.py) and [VHCT (Li et al,
+2021)](https://arxiv.org/abs/2106.09215). PyXAB also provides the most
+commonly-used synthetic objectives to evaluate the performance of different
+algorithms and the implementations for different hierarchical partitions **The
+algorithms are maximization algorithms!** ## Quick Links - [Quick Example]
+(#Quick-Example) - [Documentations](#Documentations) - [Installation]
+(#Installation) - [Features](#Features) * [*X*-armed bandit algorithms]
+(#Stochastic-X-armed-bandit-algorithms) * [Hierarchical partition ]
+(#Hierarchical-partition) * [Synthetic objectives](#Synthetic-objectives) -
+[Contributing](#Contributing) - [Citations](#Citations) ## Quick Example PyXAB
+follows a natural and straightforward API design completely aligned with the
+online blackbox optimization paradigm. The following is a simple 6-line usage
+example. First, we define the parameter domain and the algorithm to run. At
+every round `t`, call `algo.pull(t)` to get a point and call
+`algo.receive_reward(t, reward)` to give the algorithm the objective evaluation
+(reward) ``` ```python3 domain = [[0, 1]] # Parameter is 1-D and between 0 and
+1 algo = T_HOO(rounds=1000, domain=domain) for t in range(1000): point =
+algo.pull(t) reward = 1 #TODO: User-defined objective returns the reward
+algo.receive_reward(t, reward) ``` More detailed examples can be found [here]
+(https://pyxab.readthedocs.io/en/latest/getting_started/auto_examples/
+index.html) ## Documentations * The most up-to-date [documentations](https://
 pyxab.readthedocs.io/) * The [roadmap](https://github.com/users/WilliamLwj/
-projects/1) for our project * Our [paper](https://arxiv.org/abs/2303.04030) for
-the library ## Installation To install via pip, run the following lines of code
-```bash pip install PyXAB # normal install pip install --upgrade PyXAB # or
-update if needed ``` To install via git, run the following lines of code
-```bash git clone https://github.com/WilliamLwj/PyXAB.git cd PyXAB pip install
-. ``` ## Features: ### *X*-armed bandit algorithms * Algorithm starred are
-meta-algorithms (wrappers) | Algorithm | Research Paper | Year | |-------------
-------------------------------------------------------------------------|------
+projects/1) for our project * Our [manuscript](https://arxiv.org/abs/
+2303.04030) for the library ## Installation To install via pip, run the
+following lines of code ```bash pip install PyXAB # normal install pip install
+--upgrade PyXAB # or update if needed ``` To install via git, run the following
+lines of code ```bash git clone https://github.com/WilliamLwj/PyXAB.git cd
+PyXAB pip install . ``` ## Features: ### *X*-armed bandit algorithms *
+Algorithm starred are meta-algorithms (wrappers) | Algorithm | Research Paper |
+Year | |-----------------------------------------------------------------------
+--------------|----------------------------------------------------------------
 -------------------------------------------------------------------------------
--------------------------------------------------------------------------------
-----------------------|------| | [Zooming](https://github.com/WilliamLwj/PyXAB/
-blob/main/PyXAB/algos/Zooming.py) | [Multi-Armed Bandits in Metric Spaces]
-(https://arxiv.org/pdf/0809.4882.pdf) | 2008 | | [T-HOO](https://github.com/
-WilliamLwj/PyXAB/blob/main/PyXAB/algos/HOO.py) | [*X*-Armed Bandit](https://
-jmlr.org/papers/v12/bubeck11a.html) | 2011 | | [DOO](https://github.com/
-WilliamLwj/PyXAB/blob/main/PyXAB/algos/DOO.py) | [Optimistic Optimization of a
-Deterministic Function without the Knowledge of its Smoothness](https://
-proceedings.neurips.cc/paper/2011/file/7e889fb76e0e07c11733550f2a6c7a5a-
-Paper.pdf) | 2011 | | [SOO](https://github.com/WilliamLwj/PyXAB/blob/main/
-PyXAB/algos/SOO.py) | [Optimistic Optimization of a Deterministic Function
-without the Knowledge of its Smoothness](https://proceedings.neurips.cc/paper/
-2011/file/7e889fb76e0e07c11733550f2a6c7a5a-Paper.pdf) | 2011 | | [StoSOO]
-(https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/StoSOO.py) |
-[Stochastic Simultaneous Optimistic Optimization](http://proceedings.mlr.press/
-v28/valko13.pdf) | 2013 | | [HCT](https://github.com/WilliamLwj/PyXAB/blob/
-main/PyXAB/algos/HCT.py) | [Online Stochastic Optimization Under Correlated
-Bandit Feedback](https://proceedings.mlr.press/v32/azar14.html) | 2014 | |
-[POO*](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/POO.py) |
-[Black-box optimization of noisy functions with unknown smoothness](https://
+-------------------------------------------|------| | [Zooming](https://
+github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/Zooming.py) | [Multi-Armed
+Bandits in Metric Spaces](https://arxiv.org/pdf/0809.4882.pdf) | 2008 | | [T-
+HOO](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/HOO.py) | [*X*-
+Armed Bandit](https://jmlr.org/papers/v12/bubeck11a.html) | 2011 | | [DOO]
+(https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/DOO.py) |
+[Optimistic Optimization of a Deterministic Function without the Knowledge of
+its Smoothness](https://proceedings.neurips.cc/paper/2011/file/
+7e889fb76e0e07c11733550f2a6c7a5a-Paper.pdf) | 2011 | | [SOO](https://
+github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/SOO.py) | [Optimistic
+Optimization of a Deterministic Function without the Knowledge of its
+Smoothness](https://proceedings.neurips.cc/paper/2011/file/
+7e889fb76e0e07c11733550f2a6c7a5a-Paper.pdf) | 2011 | | [StoSOO](https://
+github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/StoSOO.py) | [Stochastic
+Simultaneous Optimistic Optimization](http://proceedings.mlr.press/v28/
+valko13.pdf) | 2013 | | [HCT](https://github.com/WilliamLwj/PyXAB/blob/main/
+PyXAB/algos/HCT.py) | [Online Stochastic Optimization Under Correlated Bandit
+Feedback](https://proceedings.mlr.press/v32/azar14.html) | 2014 | | [POO*]
+(https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/POO.py) | [Black-box
+optimization of noisy functions with unknown smoothness](https://
 papers.nips.cc/paper/2015/hash/ab817c9349cf9c4f6877e1894a1faa00-Abstract.html)
 | 2015 | | [GPO*](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/
 GPO.py) | [General Parallel Optimization Without A Metric](https://
 proceedings.mlr.press/v98/xuedong19a.html) | 2019 | | [PCT](https://github.com/
 WilliamLwj/PyXAB/blob/main/PyXAB/algos/PCT.py) | [General Parallel Optimization
 Without A Metric](https://proceedings.mlr.press/v98/xuedong19a.html) | 2019 | |
 [SequOOL](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/SequOOL.py)
```

### Comparing `PyXAB-0.2.1/PyXAB/algos/Algo.py` & `PyXAB-0.2.2/PyXAB/algos/Algo.py`

 * *Files identical despite different names*

### Comparing `PyXAB-0.2.1/PyXAB/algos/DOO.py` & `PyXAB-0.2.2/PyXAB/algos/DOO.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 # License: MIT
 
 
 import math
 import numpy as np
 from PyXAB.algos.Algo import Algorithm
 from PyXAB.partition.Node import P_node
+from PyXAB.partition.BinaryPartition import BinaryPartition
 import pdb
 
 
 class DOO_node(P_node):
     """
     Implementation of the node in the DOO algorithm
     """
@@ -100,15 +101,15 @@
 
 
 class DOO(Algorithm):
     """
     The implementation of the DOO algorithm (Munos, 2011)
     """
 
-    def __init__(self, n=100, delta=None, domain=None, partition=None):
+    def __init__(self, n=100, delta=None, domain=None, partition=BinaryPartition):
         """
         The initialization of the DOO algorithm
 
         Parameters
         ----------
         n: int
             The total number of rounds (budget)
```

### Comparing `PyXAB-0.2.1/PyXAB/algos/GPO.py` & `PyXAB-0.2.2/PyXAB/algos/GPO.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,23 +3,24 @@
 """
 # Author: Wenjie Li <li3549@purdue.edu>
 # License: MIT
 import pdb
 
 import numpy as np
 from PyXAB.algos.Algo import Algorithm
+from PyXAB.partition.BinaryPartition import BinaryPartition
 
 
 class GPO(Algorithm):
     """
     Implementation of the General Parallel Optimization (GPO) algorithm (Shang et al., 2019)
     """
 
     def __init__(
-        self, numax=1.0, rhomax=0.9, rounds=1000, domain=None, partition=None, algo=None
+        self, numax=1.0, rhomax=0.9, rounds=1000, domain=None, partition=BinaryPartition, algo=None
     ):
         """
         Initialization of the wrapper algorithm
 
         Parameters
         ----------
         numax: float
```

### Comparing `PyXAB-0.2.1/PyXAB/algos/HCT.py` & `PyXAB-0.2.2/PyXAB/algos/HCT.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 # Author: Wenjie Li <li3549@purdue.edu>
 # License: MIT
 
 import math
 import numpy as np
 from PyXAB.algos.Algo import Algorithm
 from PyXAB.partition.Node import P_node
+from PyXAB.partition.BinaryPartition import BinaryPartition
 import pdb
 
 
 def compute_t_plus(x):
     return np.power(2, np.ceil(np.log(x) / np.log(2)))
 
 
@@ -145,15 +146,15 @@
 
 
 class HCT(Algorithm):
     """
     Implementation of the HCT algorithm
     """
 
-    def __init__(self, nu=1, rho=0.5, c=0.1, delta=0.01, domain=None, partition=None):
+    def __init__(self, nu=1, rho=0.5, c=0.1, delta=0.01, domain=None, partition=BinaryPartition):
         """
         Initialization of the HCT algorithm
 
         Parameters
         ----------
         nu: float
             parameter nu of the HCT algorithm
```

### Comparing `PyXAB-0.2.1/PyXAB/algos/HOO.py` & `PyXAB-0.2.2/PyXAB/algos/HOO.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 # Author: Wenjie Li <li3549@purdue.edu>
 # License: MIT
 
 import math
 import numpy as np
 from PyXAB.algos.Algo import Algorithm
 from PyXAB.partition.Node import P_node
+from PyXAB.partition.BinaryPartition import BinaryPartition
 import pdb
 
 
 class HOO_node(P_node):
     """
     Implementation of the HOO_node
     """
@@ -138,15 +139,15 @@
 
 
 class T_HOO(Algorithm):
     """
     Implementation of the T_HOO algorithm
     """
 
-    def __init__(self, nu=1, rho=0.5, rounds=1000, domain=None, partition=None):
+    def __init__(self, nu=1, rho=0.5, rounds=1000, domain=None, partition=BinaryPartition):
         """
         Initialization of the T_HOO algorithm
 
         Parameters
         ----------
         nu: float
             parameter nu of the T_HOO algorithm
```

### Comparing `PyXAB-0.2.1/PyXAB/algos/PCT.py` & `PyXAB-0.2.2/PyXAB/algos/PCT.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 # Author: Wenjie Li <li3549@purdue.edu>
 # License: MIT
 
 import numpy as np
 from PyXAB.algos.Algo import Algorithm
 from PyXAB.algos.HCT import HCT
 from PyXAB.algos.GPO import GPO
-
+from PyXAB.partition.BinaryPartition import BinaryPartition
 
 class PCT(Algorithm):
     """
     Implementation of Parallel Confidence Tree (Shang et al., 2019) algorithm
     """
 
-    def __init__(self, numax=1, rhomax=0.9, rounds=1000, domain=None, partition=None):
+    def __init__(self, numax=1, rhomax=0.9, rounds=1000, domain=None, partition=BinaryPartition):
         """
         Initialization of the PCT algorithm
 
         Parameters
         ----------
         numax: float
             parameter nu_max in the algorithm
```

### Comparing `PyXAB-0.2.1/PyXAB/algos/POO.py` & `PyXAB-0.2.2/PyXAB/algos/POO.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 """
 # Author: Wenjie Li <li3549@purdue.edu>
 # License: MIT
 import pdb
 
 import numpy as np
 from PyXAB.algos.Algo import Algorithm
-
+from PyXAB.partition.BinaryPartition import BinaryPartition
 
 class POO(Algorithm):
     """
     Implementation of the Parallel Optimistic Optimization (POO) algorithm (Grill et al., 2015), with the general
     definition in Shang et al., 2019.
     """
 
     def __init__(
-        self, numax=1, rhomax=0.9, rounds=1000, domain=None, partition=None, algo=None
+        self, numax=1, rhomax=0.9, rounds=1000, domain=None, partition=BinaryPartition, algo=None
     ):
         """
 
         Parameters
         ----------
         numax: float
             parameter nu_max in the algorithm
```

### Comparing `PyXAB-0.2.1/PyXAB/algos/SOO.py` & `PyXAB-0.2.2/PyXAB/algos/SOO.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 # License: MIT
 
 
 import math
 import numpy as np
 from PyXAB.algos.Algo import Algorithm
 from PyXAB.partition.Node import P_node
+from PyXAB.partition.BinaryPartition import BinaryPartition
 import pdb
 
 
 class SOO_node(P_node):
     """
     Implementation of the node in the SOO algorithm
     """
@@ -75,15 +76,15 @@
 
 
 class SOO(Algorithm):
     """
     The implementation of the SOO algorithm (Munos, 2011)
     """
 
-    def __init__(self, n=100, h_max=100, domain=None, partition=None):
+    def __init__(self, n=100, h_max=100, domain=None, partition=BinaryPartition):
         """
         The initialization of the SOO algorithm
         
         Parameters
         ----------
         n: int
             The total number of rounds (budget)
```

### Comparing `PyXAB-0.2.1/PyXAB/algos/SequOOL.py` & `PyXAB-0.2.2/PyXAB/algos/SequOOL.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 # License: MIT
 
 import math
 import random
 import numpy as np
 from PyXAB.algos.Algo import Algorithm
 from PyXAB.partition.Node import P_node
+from PyXAB.partition.BinaryPartition import BinaryPartition
 import pdb
 
 
 class SequOOL_node(P_node):
     """
     Implementation of the SequOOL node
     """
@@ -84,15 +85,15 @@
 
 
 class SequOOL(Algorithm):
     """
     The implementation of the SequOOL algorithm (Barlett, 2019)
     """
 
-    def __init__(self, n=1000, domain=None, partition=None):
+    def __init__(self, n=1000, domain=None, partition=BinaryPartition):
         """
         The initialization of the SequOOL algorithm
         
         Parameters
         ----------
         n: int
             The totdal number of rounds (budget)
```

### Comparing `PyXAB-0.2.1/PyXAB/algos/StoSOO.py` & `PyXAB-0.2.2/PyXAB/algos/StoSOO.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 # License: MIT
 
 
 import math
 import numpy as np
 from PyXAB.algos.Algo import Algorithm
 from PyXAB.partition.Node import P_node
+from PyXAB.partition.BinaryPartition import BinaryPartition
 import pdb
 
 
 class StoSOO_node(P_node):
     """
     Implementation of the node in the StoSOO algorithm
     """
@@ -114,15 +115,15 @@
 
 class StoSOO(Algorithm):
     """
     The implementation of the StoSOO algorithm (Valko et al., 2013)
     """
 
     def __init__(
-        self, n=100, k=None, h_max=100, delta=None, domain=None, partition=None
+        self, n=100, k=None, h_max=100, delta=None, domain=None, partition=BinaryPartition
     ):
         """
         The initialization of the StoSOO algorithm
 
         Parameters
         ----------
         n: int
```

### Comparing `PyXAB-0.2.1/PyXAB/algos/StroquOOL.py` & `PyXAB-0.2.2/PyXAB/algos/StroquOOL.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 # Author: Haoze Li <li4456@purdue.edu>
 # License: MIT
 
 import math
 import numpy as np
 from PyXAB.algos.Algo import Algorithm
 from PyXAB.partition.Node import P_node
+from PyXAB.partition.BinaryPartition import BinaryPartition
 import pdb
 
 
 class StroquOOL_node(P_node):
     """
     Implementation of the node in the StroquOOL algorithm
     """
@@ -118,15 +119,15 @@
 
 
 class StroquOOL(Algorithm):
     """
     The implementation of the StroquOOL algorithm (Bartlett, 2019)
     """
 
-    def __init__(self, n=1000, domain=None, partition=None):
+    def __init__(self, n=1000, domain=None, partition=BinaryPartition):
         """
         The initialization of the StroquOOL algorithm
 
         Parameters
         ----------
         n: int
             The total number of rounds (budget)
```

### Comparing `PyXAB-0.2.1/PyXAB/algos/VHCT.py` & `PyXAB-0.2.2/PyXAB/algos/VHCT.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # License: MIT
 
 
 import math
 import numpy as np
 from PyXAB.algos.Algo import Algorithm
 from PyXAB.partition.Node import P_node
-
+from PyXAB.partition.BinaryPartition import BinaryPartition
 
 def compute_t_plus(x):
     return np.power(2, np.ceil(np.log(x) / np.log(2)))
 
 
 class VHCT_node(P_node):
     """
@@ -204,15 +204,15 @@
 
 class VHCT(Algorithm):
     """
     The implementation of the Variance High Confidence Tree algorithm
     """
 
     def __init__(
-        self, nu=1, rho=0.5, c=0.1, delta=0.01, bound=1, domain=None, partition=None
+        self, nu=1, rho=0.5, c=0.1, delta=0.01, bound=1, domain=None, partition=BinaryPartition
     ):
         """
         Initialization of the VHCT algorithm
 
         Parameters
         ----------
         nu: float
```

### Comparing `PyXAB-0.2.1/PyXAB/algos/VPCT.py` & `PyXAB-0.2.2/PyXAB/algos/VPCT.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 # Author: Wenjie Li <li3549@purdue.edu>
 # License: MIT
 
 import numpy as np
 from PyXAB.algos.Algo import Algorithm
 from PyXAB.algos.VHCT import VHCT
 from PyXAB.algos.GPO import GPO
-
+from PyXAB.partition.BinaryPartition import BinaryPartition
 
 class VPCT(Algorithm):
     """
     Implementation of Variance-reduced Parallel Confidence Tree  algorithm (VHCT + GPO)
     """
 
-    def __init__(self, numax=1, rhomax=0.9, rounds=1000, domain=None, partition=None):
+    def __init__(self, numax=1, rhomax=0.9, rounds=1000, domain=None, partition=BinaryPartition):
         """
         Initialization of the VPCT algorithm
 
         Parameters
         ----------
         numax: float
             parameter nu_max in the algorithm
```

### Comparing `PyXAB-0.2.1/PyXAB/algos/Zooming.py` & `PyXAB-0.2.2/PyXAB/algos/Zooming.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 import math
 import pdb
 
 import numpy as np
 from PyXAB.algos.Algo import Algorithm
 from PyXAB.partition.Node import P_node
-
+from PyXAB.partition.BinaryPartition import BinaryPartition
 
 class point:
     """
     A helper class to use points as references
     """
 
     def __init__(self, p):
@@ -26,15 +26,15 @@
 
 
 class Zooming(Algorithm):
     """
     The implementation of the Zooming algorithm
     """
 
-    def __init__(self, nu=1, rho=0.9, domain=None, partition=None):
+    def __init__(self, nu=1, rho=0.9, domain=None, partition=BinaryPartition):
         """
         Initialization of the Zooming algorithm
 
         Parameters
         ----------
         nu: float
             smoothness parameter nu of the Zooming algorithm
```

### Comparing `PyXAB-0.2.1/PyXAB/partition/BinaryPartition.py` & `PyXAB-0.2.2/PyXAB/partition/BinaryPartition.py`

 * *Files identical despite different names*

### Comparing `PyXAB-0.2.1/PyXAB/partition/DimensionBinaryPartition.py` & `PyXAB-0.2.2/PyXAB/partition/DimensionBinaryPartition.py`

 * *Files identical despite different names*

### Comparing `PyXAB-0.2.1/PyXAB/partition/KaryPartition.py` & `PyXAB-0.2.2/PyXAB/partition/KaryPartition.py`

 * *Files identical despite different names*

### Comparing `PyXAB-0.2.1/PyXAB/partition/Node.py` & `PyXAB-0.2.2/PyXAB/partition/Node.py`

 * *Files identical despite different names*

### Comparing `PyXAB-0.2.1/PyXAB/partition/Partition.py` & `PyXAB-0.2.2/PyXAB/partition/Partition.py`

 * *Files identical despite different names*

### Comparing `PyXAB-0.2.1/PyXAB/partition/RandomBinaryPartition.py` & `PyXAB-0.2.2/PyXAB/partition/RandomBinaryPartition.py`

 * *Files identical despite different names*

### Comparing `PyXAB-0.2.1/PyXAB/partition/RandomKaryPartition.py` & `PyXAB-0.2.2/PyXAB/partition/RandomKaryPartition.py`

 * *Files identical despite different names*

### Comparing `PyXAB-0.2.1/PyXAB/synthetic_obj/Ackley.py` & `PyXAB-0.2.2/PyXAB/synthetic_obj/Ackley.py`

 * *Files identical despite different names*

### Comparing `PyXAB-0.2.1/PyXAB/synthetic_obj/Cexample.py` & `PyXAB-0.2.2/PyXAB/synthetic_obj/Cexample.py`

 * *Files identical despite different names*

### Comparing `PyXAB-0.2.1/PyXAB/synthetic_obj/DifficultFunc.py` & `PyXAB-0.2.2/PyXAB/synthetic_obj/DifficultFunc.py`

 * *Files identical despite different names*

### Comparing `PyXAB-0.2.1/PyXAB/synthetic_obj/DoubleSine.py` & `PyXAB-0.2.2/PyXAB/synthetic_obj/DoubleSine.py`

 * *Files identical despite different names*

### Comparing `PyXAB-0.2.1/PyXAB/synthetic_obj/Garland.py` & `PyXAB-0.2.2/PyXAB/synthetic_obj/Garland.py`

 * *Files identical despite different names*

### Comparing `PyXAB-0.2.1/PyXAB/synthetic_obj/Himmelblau.py` & `PyXAB-0.2.2/PyXAB/synthetic_obj/Himmelblau.py`

 * *Files identical despite different names*

### Comparing `PyXAB-0.2.1/PyXAB/synthetic_obj/Rastrigin.py` & `PyXAB-0.2.2/PyXAB/synthetic_obj/Rastrigin.py`

 * *Files identical despite different names*

### Comparing `PyXAB-0.2.1/PyXAB/utils/plot.py` & `PyXAB-0.2.2/PyXAB/utils/plot.py`

 * *Files identical despite different names*

### Comparing `PyXAB-0.2.1/PyXAB/utils/run_synthetic.py` & `PyXAB-0.2.2/PyXAB/utils/run_synthetic.py`

 * *Files identical despite different names*

### Comparing `PyXAB-0.2.1/PyXAB/utils/visualize_gif.py` & `PyXAB-0.2.2/PyXAB/utils/visualize_gif.py`

 * *Files identical despite different names*

### Comparing `PyXAB-0.2.1/PyXAB.egg-info/PKG-INFO` & `PyXAB-0.2.2/PyXAB.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyXAB
-Version: 0.2.1
+Version: 0.2.2
 Summary: PyXAB - A Python Library for X-Armed Bandit and Online Blackbox Optimization Algorithms.
 Home-page: https://github.com/WilliamLwj/PyXAB
 Author: Wenjie Li, Haoze Li
 Author-email: lil3549@purdue.edu
 License: MIT
 Description: 
         
@@ -50,58 +50,60 @@
         
         
         <p align='center'>
           <img src="https://raw.githubusercontent.com/WilliamLwj/PyXAB/main/figs/HCT_trajectory.gif" alt="trajectory" width="48%"/>  
           <img src="https://raw.githubusercontent.com/WilliamLwj/PyXAB/main/figs/HCT_heatmap.gif" alt="heatmap" width="48%"/>  
         </p>
         
-        PyXAB includes implementations of different *X*-armed bandit algorithms, including the classic ones such as [HOO (Bubeck et al., 2011)](https://jmlr.org/papers/v12/bubeck11a.html), 
+        PyXAB contains the implementations of **more than 10 optimization algorithms**, including the classic ones such as [HOO (Bubeck et al., 2011)](https://jmlr.org/papers/v12/bubeck11a.html), 
          [StoSOO (Valko et al., 2013)](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/StoSOO.py), and [HCT (Azar et al., 2014)](https://proceedings.mlr.press/v32/azar14.html), and the most
-        recent works such as [GPO (Shang et al., 2019)](https://proceedings.mlr.press/v98/xuedong19a.html) and [VHCT (Li et al, 2021)](https://arxiv.org/abs/2106.09215).
+        recent works such as [GPO (Shang et al., 2019)](https://proceedings.mlr.press/v98/xuedong19a.html), [StroquOOL  (Bartlett et al.,2019)](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/StroquOOL.py) and [VHCT (Li et al, 2021)](https://arxiv.org/abs/2106.09215).
         PyXAB also provides the most commonly-used synthetic objectives to evaluate the performance of different algorithms and the implementations for different hierarchical partitions
         
+        **The algorithms are maximization algorithms!**
         
         ## Quick Links
         
         - [Quick Example](#Quick-Example)
         - [Documentations](#Documentations)
         - [Installation](#Installation)
         - [Features](#Features)
           * [*X*-armed bandit algorithms](#Stochastic-X-armed-bandit-algorithms)
           * [Hierarchical partition ](#Hierarchical-partition)
           * [Synthetic objectives](#Synthetic-objectives)
         - [Contributing](#Contributing)
         - [Citations](#Citations)
         
         ## Quick Example
-        First define the blackbox objective, the parameter domain, the partition of the space, and the algorithm, e.g.
+        PyXAB follows a natural and straightforward API design completely aligned with the online blackbox
+        optimization paradigm. The following is a simple 6-line usage example.
         
-        ```python3
-        target = Garland()
-        domain = [[0, 1]]
-        partition = BinaryPartition
-        algo = T_HOO(rounds=1000, domain=domain, partition=partition)
+        First, we define the parameter domain and the algorithm to run. 
+        At every round  `t`, call `algo.pull(t)` to get a point and call 
+        `algo.receive_reward(t, reward)` to give the algorithm the objective evaluation (reward)
         ```
         
-        At every round  `t`, call `algo.pull(t)` to get a point. After receiving the (stochastic) reward for the point, call 
-        `algo.receive_reward(t, reward)` to give the algorithm the feedback
-        
         ```python3
-        point = algo.pull(t)
-        reward = target.f(point) + np.random.uniform(-0.1, 0.1) # Uniform noise example
-        algo.receive_reward(t, reward)
+        domain = [[0, 1]]               # Parameter is 1-D and between 0 and 1
+        algo = T_HOO(rounds=1000, domain=domain) 
+        for t in range(1000):
+            point = algo.pull(t)
+            reward = 1                  #TODO: User-defined objective returns the reward
+            algo.receive_reward(t, reward)
         ```
         
+        More detailed examples can be found [here](https://pyxab.readthedocs.io/en/latest/getting_started/auto_examples/index.html)
+        
         ## Documentations
         
           * The most up-to-date [documentations](https://pyxab.readthedocs.io/) 
         
           * The [roadmap](https://github.com/users/WilliamLwj/projects/1) for our project    
           
-          * Our [paper](https://arxiv.org/abs/2303.04030) for the library
+          * Our [manuscript](https://arxiv.org/abs/2303.04030) for the library
         
         ## Installation
         
         To install via pip, run the following lines of code
         ```bash
         pip install PyXAB                 # normal install
         pip install --upgrade PyXAB       # or update if needed
```

#### html2text {}

```diff
@@ -1,75 +1,81 @@
-Metadata-Version: 2.1 Name: PyXAB Version: 0.2.1 Summary: PyXAB - A Python
+Metadata-Version: 2.1 Name: PyXAB Version: 0.2.2 Summary: PyXAB - A Python
 Library for X-Armed Bandit and Online Blackbox Optimization Algorithms. Home-
 page: https://github.com/WilliamLwj/PyXAB Author: Wenjie Li, Haoze Li Author-
 email: lil3549@purdue.edu License: MIT Description: # PyXAB - Python *X*-Armed
 Bandit
 [PyPI_version] [https://codecov.io/gh/WilliamLwj/PyXAB/branch/main/graph/
 badge.svg?token=VACRX9AQBM] [Documentation_Status] [Code_style:_black]
 [testing] [github-PyXAB_forks] [github-PyXAB_stars] [downloads] [github-PyXAB
 license] [Code_style:_black]
 PyXAB is a Python open-source library for *X*-armed bandit algorithms, a
 prestigious set of optimizers for online black-box optimization, i.e., optimize
 an objective without gradients, also known as the continuous-arm bandit (CAB),
 Lipschitz bandit, global optimization (GO) and bandit-based black-box
 optimization problems.
                             [trajectory] [heatmap]
-PyXAB includes implementations of different *X*-armed bandit algorithms,
+PyXAB contains the implementations of **more than 10 optimization algorithms**,
 including the classic ones such as [HOO (Bubeck et al., 2011)](https://
 jmlr.org/papers/v12/bubeck11a.html), [StoSOO (Valko et al., 2013)](https://
 github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/StoSOO.py), and [HCT (Azar et
 al., 2014)](https://proceedings.mlr.press/v32/azar14.html), and the most recent
 works such as [GPO (Shang et al., 2019)](https://proceedings.mlr.press/v98/
-xuedong19a.html) and [VHCT (Li et al, 2021)](https://arxiv.org/abs/2106.09215).
-PyXAB also provides the most commonly-used synthetic objectives to evaluate the
-performance of different algorithms and the implementations for different
-hierarchical partitions ## Quick Links - [Quick Example](#Quick-Example) -
-[Documentations](#Documentations) - [Installation](#Installation) - [Features]
-(#Features) * [*X*-armed bandit algorithms](#Stochastic-X-armed-bandit-
-algorithms) * [Hierarchical partition ](#Hierarchical-partition) * [Synthetic
-objectives](#Synthetic-objectives) - [Contributing](#Contributing) -
-[Citations](#Citations) ## Quick Example First define the blackbox objective,
-the parameter domain, the partition of the space, and the algorithm, e.g.
-```python3 target = Garland() domain = [[0, 1]] partition = BinaryPartition
-algo = T_HOO(rounds=1000, domain=domain, partition=partition) ``` At every
-round `t`, call `algo.pull(t)` to get a point. After receiving the (stochastic)
-reward for the point, call `algo.receive_reward(t, reward)` to give the
-algorithm the feedback ```python3 point = algo.pull(t) reward = target.f(point)
-+ np.random.uniform(-0.1, 0.1) # Uniform noise example algo.receive_reward(t,
-reward) ``` ## Documentations * The most up-to-date [documentations](https://
+xuedong19a.html), [StroquOOL (Bartlett et al.,2019)](https://github.com/
+WilliamLwj/PyXAB/blob/main/PyXAB/algos/StroquOOL.py) and [VHCT (Li et al,
+2021)](https://arxiv.org/abs/2106.09215). PyXAB also provides the most
+commonly-used synthetic objectives to evaluate the performance of different
+algorithms and the implementations for different hierarchical partitions **The
+algorithms are maximization algorithms!** ## Quick Links - [Quick Example]
+(#Quick-Example) - [Documentations](#Documentations) - [Installation]
+(#Installation) - [Features](#Features) * [*X*-armed bandit algorithms]
+(#Stochastic-X-armed-bandit-algorithms) * [Hierarchical partition ]
+(#Hierarchical-partition) * [Synthetic objectives](#Synthetic-objectives) -
+[Contributing](#Contributing) - [Citations](#Citations) ## Quick Example PyXAB
+follows a natural and straightforward API design completely aligned with the
+online blackbox optimization paradigm. The following is a simple 6-line usage
+example. First, we define the parameter domain and the algorithm to run. At
+every round `t`, call `algo.pull(t)` to get a point and call
+`algo.receive_reward(t, reward)` to give the algorithm the objective evaluation
+(reward) ``` ```python3 domain = [[0, 1]] # Parameter is 1-D and between 0 and
+1 algo = T_HOO(rounds=1000, domain=domain) for t in range(1000): point =
+algo.pull(t) reward = 1 #TODO: User-defined objective returns the reward
+algo.receive_reward(t, reward) ``` More detailed examples can be found [here]
+(https://pyxab.readthedocs.io/en/latest/getting_started/auto_examples/
+index.html) ## Documentations * The most up-to-date [documentations](https://
 pyxab.readthedocs.io/) * The [roadmap](https://github.com/users/WilliamLwj/
-projects/1) for our project * Our [paper](https://arxiv.org/abs/2303.04030) for
-the library ## Installation To install via pip, run the following lines of code
-```bash pip install PyXAB # normal install pip install --upgrade PyXAB # or
-update if needed ``` To install via git, run the following lines of code
-```bash git clone https://github.com/WilliamLwj/PyXAB.git cd PyXAB pip install
-. ``` ## Features: ### *X*-armed bandit algorithms * Algorithm starred are
-meta-algorithms (wrappers) | Algorithm | Research Paper | Year | |-------------
-------------------------------------------------------------------------|------
+projects/1) for our project * Our [manuscript](https://arxiv.org/abs/
+2303.04030) for the library ## Installation To install via pip, run the
+following lines of code ```bash pip install PyXAB # normal install pip install
+--upgrade PyXAB # or update if needed ``` To install via git, run the following
+lines of code ```bash git clone https://github.com/WilliamLwj/PyXAB.git cd
+PyXAB pip install . ``` ## Features: ### *X*-armed bandit algorithms *
+Algorithm starred are meta-algorithms (wrappers) | Algorithm | Research Paper |
+Year | |-----------------------------------------------------------------------
+--------------|----------------------------------------------------------------
 -------------------------------------------------------------------------------
--------------------------------------------------------------------------------
-----------------------|------| | [Zooming](https://github.com/WilliamLwj/PyXAB/
-blob/main/PyXAB/algos/Zooming.py) | [Multi-Armed Bandits in Metric Spaces]
-(https://arxiv.org/pdf/0809.4882.pdf) | 2008 | | [T-HOO](https://github.com/
-WilliamLwj/PyXAB/blob/main/PyXAB/algos/HOO.py) | [*X*-Armed Bandit](https://
-jmlr.org/papers/v12/bubeck11a.html) | 2011 | | [DOO](https://github.com/
-WilliamLwj/PyXAB/blob/main/PyXAB/algos/DOO.py) | [Optimistic Optimization of a
-Deterministic Function without the Knowledge of its Smoothness](https://
-proceedings.neurips.cc/paper/2011/file/7e889fb76e0e07c11733550f2a6c7a5a-
-Paper.pdf) | 2011 | | [SOO](https://github.com/WilliamLwj/PyXAB/blob/main/
-PyXAB/algos/SOO.py) | [Optimistic Optimization of a Deterministic Function
-without the Knowledge of its Smoothness](https://proceedings.neurips.cc/paper/
-2011/file/7e889fb76e0e07c11733550f2a6c7a5a-Paper.pdf) | 2011 | | [StoSOO]
-(https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/StoSOO.py) |
-[Stochastic Simultaneous Optimistic Optimization](http://proceedings.mlr.press/
-v28/valko13.pdf) | 2013 | | [HCT](https://github.com/WilliamLwj/PyXAB/blob/
-main/PyXAB/algos/HCT.py) | [Online Stochastic Optimization Under Correlated
-Bandit Feedback](https://proceedings.mlr.press/v32/azar14.html) | 2014 | |
-[POO*](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/POO.py) |
-[Black-box optimization of noisy functions with unknown smoothness](https://
+-------------------------------------------|------| | [Zooming](https://
+github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/Zooming.py) | [Multi-Armed
+Bandits in Metric Spaces](https://arxiv.org/pdf/0809.4882.pdf) | 2008 | | [T-
+HOO](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/HOO.py) | [*X*-
+Armed Bandit](https://jmlr.org/papers/v12/bubeck11a.html) | 2011 | | [DOO]
+(https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/DOO.py) |
+[Optimistic Optimization of a Deterministic Function without the Knowledge of
+its Smoothness](https://proceedings.neurips.cc/paper/2011/file/
+7e889fb76e0e07c11733550f2a6c7a5a-Paper.pdf) | 2011 | | [SOO](https://
+github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/SOO.py) | [Optimistic
+Optimization of a Deterministic Function without the Knowledge of its
+Smoothness](https://proceedings.neurips.cc/paper/2011/file/
+7e889fb76e0e07c11733550f2a6c7a5a-Paper.pdf) | 2011 | | [StoSOO](https://
+github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/StoSOO.py) | [Stochastic
+Simultaneous Optimistic Optimization](http://proceedings.mlr.press/v28/
+valko13.pdf) | 2013 | | [HCT](https://github.com/WilliamLwj/PyXAB/blob/main/
+PyXAB/algos/HCT.py) | [Online Stochastic Optimization Under Correlated Bandit
+Feedback](https://proceedings.mlr.press/v32/azar14.html) | 2014 | | [POO*]
+(https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/POO.py) | [Black-box
+optimization of noisy functions with unknown smoothness](https://
 papers.nips.cc/paper/2015/hash/ab817c9349cf9c4f6877e1894a1faa00-Abstract.html)
 | 2015 | | [GPO*](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/
 GPO.py) | [General Parallel Optimization Without A Metric](https://
 proceedings.mlr.press/v98/xuedong19a.html) | 2019 | | [PCT](https://github.com/
 WilliamLwj/PyXAB/blob/main/PyXAB/algos/PCT.py) | [General Parallel Optimization
 Without A Metric](https://proceedings.mlr.press/v98/xuedong19a.html) | 2019 | |
 [SequOOL](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/SequOOL.py)
```

### Comparing `PyXAB-0.2.1/PyXAB.egg-info/SOURCES.txt` & `PyXAB-0.2.2/PyXAB.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyXAB-0.2.1/README.md` & `PyXAB-0.2.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -41,58 +41,60 @@
 
 
 <p align='center'>
   <img src="https://raw.githubusercontent.com/WilliamLwj/PyXAB/main/figs/HCT_trajectory.gif" alt="trajectory" width="48%"/>  
   <img src="https://raw.githubusercontent.com/WilliamLwj/PyXAB/main/figs/HCT_heatmap.gif" alt="heatmap" width="48%"/>  
 </p>
 
-PyXAB includes implementations of different *X*-armed bandit algorithms, including the classic ones such as [HOO (Bubeck et al., 2011)](https://jmlr.org/papers/v12/bubeck11a.html), 
+PyXAB contains the implementations of **more than 10 optimization algorithms**, including the classic ones such as [HOO (Bubeck et al., 2011)](https://jmlr.org/papers/v12/bubeck11a.html), 
  [StoSOO (Valko et al., 2013)](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/StoSOO.py), and [HCT (Azar et al., 2014)](https://proceedings.mlr.press/v32/azar14.html), and the most
-recent works such as [GPO (Shang et al., 2019)](https://proceedings.mlr.press/v98/xuedong19a.html) and [VHCT (Li et al, 2021)](https://arxiv.org/abs/2106.09215).
+recent works such as [GPO (Shang et al., 2019)](https://proceedings.mlr.press/v98/xuedong19a.html), [StroquOOL  (Bartlett et al.,2019)](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/StroquOOL.py) and [VHCT (Li et al, 2021)](https://arxiv.org/abs/2106.09215).
 PyXAB also provides the most commonly-used synthetic objectives to evaluate the performance of different algorithms and the implementations for different hierarchical partitions
 
+**The algorithms are maximization algorithms!**
 
 ## Quick Links
 
 - [Quick Example](#Quick-Example)
 - [Documentations](#Documentations)
 - [Installation](#Installation)
 - [Features](#Features)
   * [*X*-armed bandit algorithms](#Stochastic-X-armed-bandit-algorithms)
   * [Hierarchical partition ](#Hierarchical-partition)
   * [Synthetic objectives](#Synthetic-objectives)
 - [Contributing](#Contributing)
 - [Citations](#Citations)
 
 ## Quick Example
-First define the blackbox objective, the parameter domain, the partition of the space, and the algorithm, e.g.
+PyXAB follows a natural and straightforward API design completely aligned with the online blackbox
+optimization paradigm. The following is a simple 6-line usage example.
 
-```python3
-target = Garland()
-domain = [[0, 1]]
-partition = BinaryPartition
-algo = T_HOO(rounds=1000, domain=domain, partition=partition)
+First, we define the parameter domain and the algorithm to run. 
+At every round  `t`, call `algo.pull(t)` to get a point and call 
+`algo.receive_reward(t, reward)` to give the algorithm the objective evaluation (reward)
 ```
 
-At every round  `t`, call `algo.pull(t)` to get a point. After receiving the (stochastic) reward for the point, call 
-`algo.receive_reward(t, reward)` to give the algorithm the feedback
-
 ```python3
-point = algo.pull(t)
-reward = target.f(point) + np.random.uniform(-0.1, 0.1) # Uniform noise example
-algo.receive_reward(t, reward)
+domain = [[0, 1]]               # Parameter is 1-D and between 0 and 1
+algo = T_HOO(rounds=1000, domain=domain) 
+for t in range(1000):
+    point = algo.pull(t)
+    reward = 1                  #TODO: User-defined objective returns the reward
+    algo.receive_reward(t, reward)
 ```
 
+More detailed examples can be found [here](https://pyxab.readthedocs.io/en/latest/getting_started/auto_examples/index.html)
+
 ## Documentations
 
   * The most up-to-date [documentations](https://pyxab.readthedocs.io/) 
 
   * The [roadmap](https://github.com/users/WilliamLwj/projects/1) for our project    
   
-  * Our [paper](https://arxiv.org/abs/2303.04030) for the library
+  * Our [manuscript](https://arxiv.org/abs/2303.04030) for the library
 
 ## Installation
 
 To install via pip, run the following lines of code
 ```bash
 pip install PyXAB                 # normal install
 pip install --upgrade PyXAB       # or update if needed
```

#### html2text {}

```diff
@@ -5,67 +5,73 @@
 license] [Code_style:_black]
 PyXAB is a Python open-source library for *X*-armed bandit algorithms, a
 prestigious set of optimizers for online black-box optimization, i.e., optimize
 an objective without gradients, also known as the continuous-arm bandit (CAB),
 Lipschitz bandit, global optimization (GO) and bandit-based black-box
 optimization problems.
                             [trajectory] [heatmap]
-PyXAB includes implementations of different *X*-armed bandit algorithms,
+PyXAB contains the implementations of **more than 10 optimization algorithms**,
 including the classic ones such as [HOO (Bubeck et al., 2011)](https://
 jmlr.org/papers/v12/bubeck11a.html), [StoSOO (Valko et al., 2013)](https://
 github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/StoSOO.py), and [HCT (Azar et
 al., 2014)](https://proceedings.mlr.press/v32/azar14.html), and the most recent
 works such as [GPO (Shang et al., 2019)](https://proceedings.mlr.press/v98/
-xuedong19a.html) and [VHCT (Li et al, 2021)](https://arxiv.org/abs/2106.09215).
-PyXAB also provides the most commonly-used synthetic objectives to evaluate the
-performance of different algorithms and the implementations for different
-hierarchical partitions ## Quick Links - [Quick Example](#Quick-Example) -
-[Documentations](#Documentations) - [Installation](#Installation) - [Features]
-(#Features) * [*X*-armed bandit algorithms](#Stochastic-X-armed-bandit-
-algorithms) * [Hierarchical partition ](#Hierarchical-partition) * [Synthetic
-objectives](#Synthetic-objectives) - [Contributing](#Contributing) -
-[Citations](#Citations) ## Quick Example First define the blackbox objective,
-the parameter domain, the partition of the space, and the algorithm, e.g.
-```python3 target = Garland() domain = [[0, 1]] partition = BinaryPartition
-algo = T_HOO(rounds=1000, domain=domain, partition=partition) ``` At every
-round `t`, call `algo.pull(t)` to get a point. After receiving the (stochastic)
-reward for the point, call `algo.receive_reward(t, reward)` to give the
-algorithm the feedback ```python3 point = algo.pull(t) reward = target.f(point)
-+ np.random.uniform(-0.1, 0.1) # Uniform noise example algo.receive_reward(t,
-reward) ``` ## Documentations * The most up-to-date [documentations](https://
+xuedong19a.html), [StroquOOL (Bartlett et al.,2019)](https://github.com/
+WilliamLwj/PyXAB/blob/main/PyXAB/algos/StroquOOL.py) and [VHCT (Li et al,
+2021)](https://arxiv.org/abs/2106.09215). PyXAB also provides the most
+commonly-used synthetic objectives to evaluate the performance of different
+algorithms and the implementations for different hierarchical partitions **The
+algorithms are maximization algorithms!** ## Quick Links - [Quick Example]
+(#Quick-Example) - [Documentations](#Documentations) - [Installation]
+(#Installation) - [Features](#Features) * [*X*-armed bandit algorithms]
+(#Stochastic-X-armed-bandit-algorithms) * [Hierarchical partition ]
+(#Hierarchical-partition) * [Synthetic objectives](#Synthetic-objectives) -
+[Contributing](#Contributing) - [Citations](#Citations) ## Quick Example PyXAB
+follows a natural and straightforward API design completely aligned with the
+online blackbox optimization paradigm. The following is a simple 6-line usage
+example. First, we define the parameter domain and the algorithm to run. At
+every round `t`, call `algo.pull(t)` to get a point and call
+`algo.receive_reward(t, reward)` to give the algorithm the objective evaluation
+(reward) ``` ```python3 domain = [[0, 1]] # Parameter is 1-D and between 0 and
+1 algo = T_HOO(rounds=1000, domain=domain) for t in range(1000): point =
+algo.pull(t) reward = 1 #TODO: User-defined objective returns the reward
+algo.receive_reward(t, reward) ``` More detailed examples can be found [here]
+(https://pyxab.readthedocs.io/en/latest/getting_started/auto_examples/
+index.html) ## Documentations * The most up-to-date [documentations](https://
 pyxab.readthedocs.io/) * The [roadmap](https://github.com/users/WilliamLwj/
-projects/1) for our project * Our [paper](https://arxiv.org/abs/2303.04030) for
-the library ## Installation To install via pip, run the following lines of code
-```bash pip install PyXAB # normal install pip install --upgrade PyXAB # or
-update if needed ``` To install via git, run the following lines of code
-```bash git clone https://github.com/WilliamLwj/PyXAB.git cd PyXAB pip install
-. ``` ## Features: ### *X*-armed bandit algorithms * Algorithm starred are
-meta-algorithms (wrappers) | Algorithm | Research Paper | Year | |-------------
-------------------------------------------------------------------------|------
+projects/1) for our project * Our [manuscript](https://arxiv.org/abs/
+2303.04030) for the library ## Installation To install via pip, run the
+following lines of code ```bash pip install PyXAB # normal install pip install
+--upgrade PyXAB # or update if needed ``` To install via git, run the following
+lines of code ```bash git clone https://github.com/WilliamLwj/PyXAB.git cd
+PyXAB pip install . ``` ## Features: ### *X*-armed bandit algorithms *
+Algorithm starred are meta-algorithms (wrappers) | Algorithm | Research Paper |
+Year | |-----------------------------------------------------------------------
+--------------|----------------------------------------------------------------
 -------------------------------------------------------------------------------
--------------------------------------------------------------------------------
-----------------------|------| | [Zooming](https://github.com/WilliamLwj/PyXAB/
-blob/main/PyXAB/algos/Zooming.py) | [Multi-Armed Bandits in Metric Spaces]
-(https://arxiv.org/pdf/0809.4882.pdf) | 2008 | | [T-HOO](https://github.com/
-WilliamLwj/PyXAB/blob/main/PyXAB/algos/HOO.py) | [*X*-Armed Bandit](https://
-jmlr.org/papers/v12/bubeck11a.html) | 2011 | | [DOO](https://github.com/
-WilliamLwj/PyXAB/blob/main/PyXAB/algos/DOO.py) | [Optimistic Optimization of a
-Deterministic Function without the Knowledge of its Smoothness](https://
-proceedings.neurips.cc/paper/2011/file/7e889fb76e0e07c11733550f2a6c7a5a-
-Paper.pdf) | 2011 | | [SOO](https://github.com/WilliamLwj/PyXAB/blob/main/
-PyXAB/algos/SOO.py) | [Optimistic Optimization of a Deterministic Function
-without the Knowledge of its Smoothness](https://proceedings.neurips.cc/paper/
-2011/file/7e889fb76e0e07c11733550f2a6c7a5a-Paper.pdf) | 2011 | | [StoSOO]
-(https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/StoSOO.py) |
-[Stochastic Simultaneous Optimistic Optimization](http://proceedings.mlr.press/
-v28/valko13.pdf) | 2013 | | [HCT](https://github.com/WilliamLwj/PyXAB/blob/
-main/PyXAB/algos/HCT.py) | [Online Stochastic Optimization Under Correlated
-Bandit Feedback](https://proceedings.mlr.press/v32/azar14.html) | 2014 | |
-[POO*](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/POO.py) |
-[Black-box optimization of noisy functions with unknown smoothness](https://
+-------------------------------------------|------| | [Zooming](https://
+github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/Zooming.py) | [Multi-Armed
+Bandits in Metric Spaces](https://arxiv.org/pdf/0809.4882.pdf) | 2008 | | [T-
+HOO](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/HOO.py) | [*X*-
+Armed Bandit](https://jmlr.org/papers/v12/bubeck11a.html) | 2011 | | [DOO]
+(https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/DOO.py) |
+[Optimistic Optimization of a Deterministic Function without the Knowledge of
+its Smoothness](https://proceedings.neurips.cc/paper/2011/file/
+7e889fb76e0e07c11733550f2a6c7a5a-Paper.pdf) | 2011 | | [SOO](https://
+github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/SOO.py) | [Optimistic
+Optimization of a Deterministic Function without the Knowledge of its
+Smoothness](https://proceedings.neurips.cc/paper/2011/file/
+7e889fb76e0e07c11733550f2a6c7a5a-Paper.pdf) | 2011 | | [StoSOO](https://
+github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/StoSOO.py) | [Stochastic
+Simultaneous Optimistic Optimization](http://proceedings.mlr.press/v28/
+valko13.pdf) | 2013 | | [HCT](https://github.com/WilliamLwj/PyXAB/blob/main/
+PyXAB/algos/HCT.py) | [Online Stochastic Optimization Under Correlated Bandit
+Feedback](https://proceedings.mlr.press/v32/azar14.html) | 2014 | | [POO*]
+(https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/POO.py) | [Black-box
+optimization of noisy functions with unknown smoothness](https://
 papers.nips.cc/paper/2015/hash/ab817c9349cf9c4f6877e1894a1faa00-Abstract.html)
 | 2015 | | [GPO*](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/
 GPO.py) | [General Parallel Optimization Without A Metric](https://
 proceedings.mlr.press/v98/xuedong19a.html) | 2019 | | [PCT](https://github.com/
 WilliamLwj/PyXAB/blob/main/PyXAB/algos/PCT.py) | [General Parallel Optimization
 Without A Metric](https://proceedings.mlr.press/v98/xuedong19a.html) | 2019 | |
 [SequOOL](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/SequOOL.py)
```

### Comparing `PyXAB-0.2.1/setup.py` & `PyXAB-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'PyXAB'
 DESCRIPTION = 'PyXAB - A Python Library for X-Armed Bandit and Online Blackbox Optimization Algorithms.'
 URL = 'https://github.com/WilliamLwj/PyXAB'
 EMAIL = 'lil3549@purdue.edu'
 AUTHOR = 'Wenjie Li, Haoze Li'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.2.1'
+VERSION = '0.2.2'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'numpy>=1.20.3',
     'matplotlib',
     # 'requests', 'maya', 'records',
 ]
```

