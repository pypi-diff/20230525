# Comparing `tmp/freerec-0.3.1.tar.gz` & `tmp/freerec-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freerec-0.3.1.tar", last modified: Sun Apr  9 03:11:27 2023, max compression
+gzip compressed data, was "freerec-0.3.5.tar", last modified: Wed Apr 26 07:39:53 2023, max compression
```

## Comparing `freerec-0.3.1.tar` & `freerec-0.3.5.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxrwxrwx   0        0        0        0 2023-04-09 03:11:27.795427 freerec-0.3.1/
--rw-rw-rw-   0        0        0     1085 2022-09-12 08:50:27.000000 freerec-0.3.1/LICENSE
--rw-rw-rw-   0        0        0     1814 2023-04-09 03:11:27.794838 freerec-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     1349 2023-03-24 04:09:10.000000 freerec-0.3.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-09 03:11:27.537852 freerec-0.3.1/freerec/
--rw-rw-rw-   0        0        0      506 2023-04-09 03:10:25.000000 freerec-0.3.1/freerec/__init__.py
--rw-rw-rw-   0        0        0     4188 2023-03-27 11:31:30.000000 freerec-0.3.1/freerec/__main__.py
--rw-rw-rw-   0        0        0     3379 2023-03-16 13:10:00.000000 freerec-0.3.1/freerec/criterions.py
-drwxrwxrwx   0        0        0        0 2023-04-09 03:11:27.580699 freerec-0.3.1/freerec/data/
--rw-rw-rw-   0        0        0       90 2023-02-24 08:54:11.000000 freerec-0.3.1/freerec/data/__init__.py
--rw-rw-rw-   0        0        0      998 2023-03-22 12:08:02.000000 freerec-0.3.1/freerec/data/dataloader.py
-drwxrwxrwx   0        0        0        0 2023-04-09 03:11:27.598971 freerec-0.3.1/freerec/data/datasets/
--rw-rw-rw-   0        0        0      239 2023-03-08 11:54:05.000000 freerec-0.3.1/freerec/data/datasets/__init__.py
--rw-rw-rw-   0        0        0    18023 2023-02-27 06:25:40.000000 freerec-0.3.1/freerec/data/datasets/base.py
-drwxrwxrwx   0        0        0        0 2023-04-09 03:11:27.606534 freerec-0.3.1/freerec/data/datasets/context/
--rw-rw-rw-   0        0        0        0 2023-02-26 02:12:53.000000 freerec-0.3.1/freerec/data/datasets/context/__init__.py
--rw-rw-rw-   0        0        0      209 2023-02-24 08:54:11.000000 freerec-0.3.1/freerec/data/datasets/context/base.py
-drwxrwxrwx   0        0        0        0 2023-04-09 03:11:27.660108 freerec-0.3.1/freerec/data/datasets/general/
--rw-rw-rw-   0        0        0       91 2023-02-24 08:54:11.000000 freerec-0.3.1/freerec/data/datasets/general/__init__.py
--rw-rw-rw-   0        0        0    13760 2023-02-28 12:22:06.000000 freerec-0.3.1/freerec/data/datasets/general/amazon.py
--rw-rw-rw-   0        0        0     3872 2023-03-16 13:18:06.000000 freerec-0.3.1/freerec/data/datasets/general/base.py
--rw-rw-rw-   0        0        0     2861 2023-04-08 05:39:36.000000 freerec-0.3.1/freerec/data/datasets/general/gowalla.py
--rw-rw-rw-   0        0        0     4729 2023-02-28 12:23:17.000000 freerec-0.3.1/freerec/data/datasets/general/movielens.py
--rw-rw-rw-   0        0        0     2845 2023-02-28 12:22:37.000000 freerec-0.3.1/freerec/data/datasets/general/yelp.py
-drwxrwxrwx   0        0        0        0 2023-04-09 03:11:27.671157 freerec-0.3.1/freerec/data/datasets/knowledge/
--rw-rw-rw-   0        0        0        0 2023-02-26 02:12:46.000000 freerec-0.3.1/freerec/data/datasets/knowledge/__init__.py
--rw-rw-rw-   0        0        0      215 2023-02-24 08:54:11.000000 freerec-0.3.1/freerec/data/datasets/knowledge/base.py
-drwxrwxrwx   0        0        0        0 2023-04-09 03:11:27.715396 freerec-0.3.1/freerec/data/datasets/sequential/
--rw-rw-rw-   0        0        0       69 2023-02-28 12:12:56.000000 freerec-0.3.1/freerec/data/datasets/sequential/__init__.py
--rw-rw-rw-   0        0        0     3716 2023-02-28 12:30:03.000000 freerec-0.3.1/freerec/data/datasets/sequential/amazon.py
--rw-rw-rw-   0        0        0     2818 2023-02-28 12:32:59.000000 freerec-0.3.1/freerec/data/datasets/sequential/base.py
--rw-rw-rw-   0        0        0     1792 2023-02-28 12:30:30.000000 freerec-0.3.1/freerec/data/datasets/sequential/movielens.py
--rw-rw-rw-   0        0        0     1794 2023-02-28 12:31:02.000000 freerec-0.3.1/freerec/data/datasets/sequential/steam.py
-drwxrwxrwx   0        0        0        0 2023-04-09 03:11:27.726441 freerec-0.3.1/freerec/data/datasets/session/
--rw-rw-rw-   0        0        0        0 2023-02-26 02:12:38.000000 freerec-0.3.1/freerec/data/datasets/session/__init__.py
--rw-rw-rw-   0        0        0      209 2023-02-24 08:54:11.000000 freerec-0.3.1/freerec/data/datasets/session/base.py
--rw-rw-rw-   0        0        0    29454 2023-03-10 09:09:02.000000 freerec-0.3.1/freerec/data/fields.py
-drwxrwxrwx   0        0        0        0 2023-04-09 03:11:27.779778 freerec-0.3.1/freerec/data/postprocessing/
--rw-rw-rw-   0        0        0      111 2023-02-24 08:54:11.000000 freerec-0.3.1/freerec/data/postprocessing/__init__.py
--rw-rw-rw-   0        0        0     2713 2023-02-24 08:54:11.000000 freerec-0.3.1/freerec/data/postprocessing/base.py
--rw-rw-rw-   0        0        0     2177 2023-02-24 08:54:11.000000 freerec-0.3.1/freerec/data/postprocessing/column.py
--rw-rw-rw-   0        0        0    10232 2023-02-24 08:54:11.000000 freerec-0.3.1/freerec/data/postprocessing/row.py
--rw-rw-rw-   0        0        0    17697 2023-02-24 08:54:11.000000 freerec-0.3.1/freerec/data/postprocessing/sampler.py
--rw-rw-rw-   0        0        0     2737 2023-02-24 08:54:11.000000 freerec-0.3.1/freerec/data/postprocessing/source.py
-drwxrwxrwx   0        0        0        0 2023-04-09 03:11:27.792838 freerec-0.3.1/freerec/data/preprocessing/
--rw-rw-rw-   0        0        0       62 2023-03-24 02:17:25.000000 freerec-0.3.1/freerec/data/preprocessing/__init__.py
--rw-rw-rw-   0        0        0    18771 2023-03-26 11:55:18.000000 freerec-0.3.1/freerec/data/preprocessing/base.py
--rw-rw-rw-   0        0        0     7748 2023-04-06 04:06:45.000000 freerec-0.3.1/freerec/data/preprocessing/datasets.py
--rw-rw-rw-   0        0        0      807 2023-03-23 07:09:59.000000 freerec-0.3.1/freerec/data/tags.py
--rw-rw-rw-   0        0        0     4533 2023-02-26 11:58:59.000000 freerec-0.3.1/freerec/data/transformation.py
--rw-rw-rw-   0        0        0     7457 2023-03-17 12:50:23.000000 freerec-0.3.1/freerec/data/utils.py
--rw-rw-rw-   0        0        0     3101 2023-02-24 08:54:11.000000 freerec-0.3.1/freerec/dict2obj.py
--rw-rw-rw-   0        0        0    31008 2023-04-09 01:47:49.000000 freerec-0.3.1/freerec/launcher.py
--rw-rw-rw-   0        0        0    22071 2023-03-27 11:15:13.000000 freerec-0.3.1/freerec/metrics.py
-drwxrwxrwx   0        0        0        0 2023-04-09 03:11:27.793837 freerec-0.3.1/freerec/models/
--rw-rw-rw-   0        0        0       23 2023-02-24 08:54:11.000000 freerec-0.3.1/freerec/models/__init__.py
--rw-rw-rw-   0        0        0     3289 2023-02-24 08:54:11.000000 freerec-0.3.1/freerec/models/base.py
--rw-rw-rw-   0        0        0    16542 2023-03-24 05:56:11.000000 freerec-0.3.1/freerec/parser.py
--rw-rw-rw-   0        0        0    14588 2023-03-16 13:10:40.000000 freerec-0.3.1/freerec/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-09 03:11:27.562370 freerec-0.3.1/freerec.egg-info/
--rw-rw-rw-   0        0        0     1814 2023-04-09 03:11:27.000000 freerec-0.3.1/freerec.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1675 2023-04-09 03:11:27.000000 freerec-0.3.1/freerec.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-09 03:11:27.000000 freerec-0.3.1/freerec.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-04-09 03:11:27.000000 freerec-0.3.1/freerec.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      111 2023-04-09 03:11:27.000000 freerec-0.3.1/freerec.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-09 03:11:27.000000 freerec-0.3.1/freerec.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-09 03:11:27.795427 freerec-0.3.1/setup.cfg
--rw-rw-rw-   0        0        0     1180 2023-03-24 05:54:08.000000 freerec-0.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-26 07:39:53.330674 freerec-0.3.5/
+-rw-rw-rw-   0        0        0     1085 2022-09-12 08:50:27.000000 freerec-0.3.5/LICENSE
+-rw-rw-rw-   0        0        0     2598 2023-04-26 07:39:53.330674 freerec-0.3.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2133 2023-04-09 09:14:38.000000 freerec-0.3.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-26 07:39:53.229422 freerec-0.3.5/freerec/
+-rw-rw-rw-   0        0        0      505 2023-04-26 07:36:47.000000 freerec-0.3.5/freerec/__init__.py
+-rw-rw-rw-   0        0        0     4188 2023-03-27 11:31:30.000000 freerec-0.3.5/freerec/__main__.py
+-rw-rw-rw-   0        0        0     3379 2023-03-16 13:10:00.000000 freerec-0.3.5/freerec/criterions.py
+drwxrwxrwx   0        0        0        0 2023-04-26 07:39:53.268646 freerec-0.3.5/freerec/data/
+-rw-rw-rw-   0        0        0       90 2023-02-24 08:54:11.000000 freerec-0.3.5/freerec/data/__init__.py
+-rw-rw-rw-   0        0        0      998 2023-03-22 12:08:02.000000 freerec-0.3.5/freerec/data/dataloader.py
+drwxrwxrwx   0        0        0        0 2023-04-26 07:39:53.270651 freerec-0.3.5/freerec/data/datasets/
+-rw-rw-rw-   0        0        0      239 2023-03-08 11:54:05.000000 freerec-0.3.5/freerec/data/datasets/__init__.py
+-rw-rw-rw-   0        0        0    18023 2023-02-27 06:25:40.000000 freerec-0.3.5/freerec/data/datasets/base.py
+drwxrwxrwx   0        0        0        0 2023-04-26 07:39:53.271651 freerec-0.3.5/freerec/data/datasets/context/
+-rw-rw-rw-   0        0        0        0 2023-02-26 02:12:53.000000 freerec-0.3.5/freerec/data/datasets/context/__init__.py
+-rw-rw-rw-   0        0        0      209 2023-02-24 08:54:11.000000 freerec-0.3.5/freerec/data/datasets/context/base.py
+drwxrwxrwx   0        0        0        0 2023-04-26 07:39:53.278784 freerec-0.3.5/freerec/data/datasets/general/
+-rw-rw-rw-   0        0        0       91 2023-02-24 08:54:11.000000 freerec-0.3.5/freerec/data/datasets/general/__init__.py
+-rw-rw-rw-   0        0        0    13580 2023-04-26 06:46:20.000000 freerec-0.3.5/freerec/data/datasets/general/amazon.py
+-rw-rw-rw-   0        0        0     3872 2023-03-16 13:18:06.000000 freerec-0.3.5/freerec/data/datasets/general/base.py
+-rw-rw-rw-   0        0        0     2825 2023-04-26 06:46:27.000000 freerec-0.3.5/freerec/data/datasets/general/gowalla.py
+-rw-rw-rw-   0        0        0     4657 2023-04-26 06:54:50.000000 freerec-0.3.5/freerec/data/datasets/general/movielens.py
+-rw-rw-rw-   0        0        0     2809 2023-04-26 06:52:08.000000 freerec-0.3.5/freerec/data/datasets/general/yelp.py
+drwxrwxrwx   0        0        0        0 2023-04-26 07:39:53.279793 freerec-0.3.5/freerec/data/datasets/knowledge/
+-rw-rw-rw-   0        0        0        0 2023-02-26 02:12:46.000000 freerec-0.3.5/freerec/data/datasets/knowledge/__init__.py
+-rw-rw-rw-   0        0        0      215 2023-02-24 08:54:11.000000 freerec-0.3.5/freerec/data/datasets/knowledge/base.py
+drwxrwxrwx   0        0        0        0 2023-04-26 07:39:53.292393 freerec-0.3.5/freerec/data/datasets/sequential/
+-rw-rw-rw-   0        0        0       69 2023-02-28 12:12:56.000000 freerec-0.3.5/freerec/data/datasets/sequential/__init__.py
+-rw-rw-rw-   0        0        0    10772 2023-04-26 07:32:55.000000 freerec-0.3.5/freerec/data/datasets/sequential/amazon.py
+-rw-rw-rw-   0        0        0     2818 2023-02-28 12:32:59.000000 freerec-0.3.5/freerec/data/datasets/sequential/base.py
+-rw-rw-rw-   0        0        0     1756 2023-04-26 07:33:17.000000 freerec-0.3.5/freerec/data/datasets/sequential/movielens.py
+-rw-rw-rw-   0        0        0     1751 2023-04-26 07:33:37.000000 freerec-0.3.5/freerec/data/datasets/sequential/steam.py
+drwxrwxrwx   0        0        0        0 2023-04-26 07:39:53.294411 freerec-0.3.5/freerec/data/datasets/session/
+-rw-rw-rw-   0        0        0        0 2023-02-26 02:12:38.000000 freerec-0.3.5/freerec/data/datasets/session/__init__.py
+-rw-rw-rw-   0        0        0      209 2023-02-24 08:54:11.000000 freerec-0.3.5/freerec/data/datasets/session/base.py
+-rw-rw-rw-   0        0        0    29845 2023-04-25 10:57:51.000000 freerec-0.3.5/freerec/data/fields.py
+drwxrwxrwx   0        0        0        0 2023-04-26 07:39:53.311010 freerec-0.3.5/freerec/data/postprocessing/
+-rw-rw-rw-   0        0        0      111 2023-02-24 08:54:11.000000 freerec-0.3.5/freerec/data/postprocessing/__init__.py
+-rw-rw-rw-   0        0        0     2713 2023-02-24 08:54:11.000000 freerec-0.3.5/freerec/data/postprocessing/base.py
+-rw-rw-rw-   0        0        0     2177 2023-02-24 08:54:11.000000 freerec-0.3.5/freerec/data/postprocessing/column.py
+-rw-rw-rw-   0        0        0    10217 2023-04-25 11:14:13.000000 freerec-0.3.5/freerec/data/postprocessing/row.py
+-rw-rw-rw-   0        0        0    17962 2023-04-25 11:11:28.000000 freerec-0.3.5/freerec/data/postprocessing/sampler.py
+-rw-rw-rw-   0        0        0     3228 2023-04-10 09:00:22.000000 freerec-0.3.5/freerec/data/postprocessing/source.py
+drwxrwxrwx   0        0        0        0 2023-04-26 07:39:53.317578 freerec-0.3.5/freerec/data/preprocessing/
+-rw-rw-rw-   0        0        0       62 2023-03-24 02:17:25.000000 freerec-0.3.5/freerec/data/preprocessing/__init__.py
+-rw-rw-rw-   0        0        0    19241 2023-04-26 06:53:36.000000 freerec-0.3.5/freerec/data/preprocessing/base.py
+-rw-rw-rw-   0        0        0     8970 2023-04-26 06:52:50.000000 freerec-0.3.5/freerec/data/preprocessing/datasets.py
+-rw-rw-rw-   0        0        0      807 2023-03-23 07:09:59.000000 freerec-0.3.5/freerec/data/tags.py
+-rw-rw-rw-   0        0        0     4533 2023-02-26 11:58:59.000000 freerec-0.3.5/freerec/data/transformation.py
+-rw-rw-rw-   0        0        0     7457 2023-03-17 12:50:23.000000 freerec-0.3.5/freerec/data/utils.py
+-rw-rw-rw-   0        0        0     3101 2023-02-24 08:54:11.000000 freerec-0.3.5/freerec/dict2obj.py
+-rw-rw-rw-   0        0        0    31338 2023-04-26 05:42:39.000000 freerec-0.3.5/freerec/launcher.py
+-rw-rw-rw-   0        0        0    22071 2023-03-27 11:15:13.000000 freerec-0.3.5/freerec/metrics.py
+drwxrwxrwx   0        0        0        0 2023-04-26 07:39:53.329280 freerec-0.3.5/freerec/models/
+-rw-rw-rw-   0        0        0       23 2023-02-24 08:54:11.000000 freerec-0.3.5/freerec/models/__init__.py
+-rw-rw-rw-   0        0        0     3289 2023-02-24 08:54:11.000000 freerec-0.3.5/freerec/models/base.py
+-rw-rw-rw-   0        0        0    16575 2023-04-11 11:36:37.000000 freerec-0.3.5/freerec/parser.py
+-rw-rw-rw-   0        0        0    14588 2023-03-16 13:10:40.000000 freerec-0.3.5/freerec/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-26 07:39:53.246449 freerec-0.3.5/freerec.egg-info/
+-rw-rw-rw-   0        0        0     2598 2023-04-26 07:39:53.000000 freerec-0.3.5/freerec.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1675 2023-04-26 07:39:53.000000 freerec-0.3.5/freerec.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 07:39:53.000000 freerec-0.3.5/freerec.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-04-26 07:39:53.000000 freerec-0.3.5/freerec.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      144 2023-04-26 07:39:53.000000 freerec-0.3.5/freerec.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-26 07:39:53.000000 freerec-0.3.5/freerec.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-26 07:39:53.330674 freerec-0.3.5/setup.cfg
+-rw-rw-rw-   0        0        0     1228 2023-04-11 12:23:57.000000 freerec-0.3.5/setup.py
```

### Comparing `freerec-0.3.1/LICENSE` & `freerec-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `freerec-0.3.1/PKG-INFO` & `freerec-0.3.5/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,46 @@
-Metadata-Version: 2.1
-Name: freerec
-Version: 0.3.1
-Summary: PyTorch library for recommender systems
-Home-page: https://github.com/MTandHJ/freerec
-Author: MTandHJ
-Author-email: congxueric@gmail.com
-License: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 
 
 FreeRec is a personal repository designed for fast data pre-processing and model training.
 I am a beginner in the field of recommender systems, so much of FreeRec's design may not be as effective. In addition, you are free to specify your own framework based on FreeRec.
 
 
 ## Requirements: 
 
 Python == 3.9 | [PyTorch == 1.12.1](https://pytorch.org/) | [TorchData == 0.4.1](https://github.com/pytorch/data) | [PyG](https://pytorch-geometric.readthedocs.io/en/latest/notes/installation.html#)
 
 
+```
+conda create --name=PyT12 python=3.9
+conda activate PyT12
+```
+
+```
+pip install torch==1.12.1+cu113 --extra-index-url https://download.pytorch.org/whl/cu113
+pip install torchdata==0.4.1
+```
+
+- Linux
+
+```
+pip install torch_geometric==2.1.0.post1
+pip install https://data.pyg.org/whl/torch-1.12.0%2Bcu116/torch_scatter-2.0.9-cp39-cp39-linux_x86_64.whl
+pip install https://data.pyg.org/whl/torch-1.12.0%2Bcu116/torch_sparse-0.6.15%2Bpt112cu116-cp39-cp39-linux_x86_64.whl
+```
+
+- Windows
+
+```
+pip install torch_geometric==2.1.0.post1
+pip install https://data.pyg.org/whl/torch-1.12.0%2Bcu116/torch_scatter-2.0.9-cp39-cp39-win_amd64.whl
+pip install https://data.pyg.org/whl/torch-1.12.0%2Bcu116/torch_sparse-0.6.15%2Bpt112cu116-cp39-cp39-win_amd64.whl
+```
+
+
+
 ## Installation
 
     pip install freerec
 
 or (for latest)
 
     pip install git+https://github.com/MTandHJ/freerec.git
```

### Comparing `freerec-0.3.1/freerec/__main__.py` & `freerec-0.3.5/freerec/__main__.py`

 * *Files identical despite different names*

### Comparing `freerec-0.3.1/freerec/criterions.py` & `freerec-0.3.5/freerec/criterions.py`

 * *Files identical despite different names*

### Comparing `freerec-0.3.1/freerec/data/dataloader.py` & `freerec-0.3.5/freerec/data/dataloader.py`

 * *Files identical despite different names*

### Comparing `freerec-0.3.1/freerec/data/datasets/base.py` & `freerec-0.3.5/freerec/data/datasets/base.py`

 * *Files identical despite different names*

### Comparing `freerec-0.3.1/freerec/data/datasets/general/amazon.py` & `freerec-0.3.5/freerec/data/datasets/general/amazon.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,15 +29,14 @@
     -------
     filename: Amazon_Books
     dataset: AmazonBooks
     kcore4user: 10
     kcore4item: 10
     star4pos: 4
     ratios: (8, 1, 1)
-    strict: True
 
     Statistics:
     -----------
     +--------+-------+---------------+---------+--------+--------+------------------------+
     | #User  | #Item | #Interactions |  #Train | #Valid | #Test  |        Density         |
     +--------+-------+---------------+---------+--------+--------+------------------------+
     | 109730 | 96421 |    3181759    | 2502323 | 308885 | 370551 | 0.00030072551044609626 |
@@ -54,15 +53,14 @@
     -------
     filename: Amazon_Books
     dataset: AmazonBooks
     kcore4user: 10
     kcore4item: 10
     star4pos: 4
     ratios: (7, 1, 2)
-    strict: True
 
     Statistics:
     -----------
     +--------+-------+---------------+---------+--------+--------+------------------------+
     | #User  | #Item | #Interactions |  #Train | #Valid | #Test  |        Density         |
     +--------+-------+---------------+---------+--------+--------+------------------------+
     | 109730 | 96421 |    3181759    | 2181889 | 320434 | 679436 | 0.00030072551044609626 |
@@ -79,15 +77,14 @@
     -------
     filename: Amazon_CDs_and_Vinyl
     dataset: AmazonCDs
     kcore4user: 10
     kcore4item: 10
     star4pos: 4
     ratios: (8, 1, 1)
-    strict: True
 
     Statistics:
     -----------
     +-------+-------+---------------+--------+--------+-------+----------------------+
     | #User | #Item | #Interactions | #Train | #Valid | #Test |       Density        |
     +-------+-------+---------------+--------+--------+-------+----------------------+
     |  9954 | 10877 |     272086    | 213755 | 26342  | 31989 | 0.002513040172344499 |
@@ -104,15 +101,14 @@
     -------
     filename: Amazon_CDs_and_Vinyl
     dataset: AmazonCDs
     kcore4user: 10
     kcore4item: 10
     star4pos: 4
     ratios: (7, 1, 2)
-    strict: True
 
     Statistics:
     -----------
     +-------+-------+---------------+--------+--------+-------+----------------------+
     | #User | #Item | #Interactions | #Train | #Valid | #Test |       Density        |
     +-------+-------+---------------+--------+--------+-------+----------------------+
     |  9954 | 10877 |     272086    | 186347 | 27408  | 58331 | 0.002513040172344499 |
@@ -129,15 +125,14 @@
     -------
     filename: Amazon_Movies_and_TV
     dataset: AmazonMovies
     kcore4user: 10
     kcore4item: 10
     star4pos: 4
     ratios: (8, 1, 1)
-    strict: True
 
     Statistics:
     -----------
     +-------+-------+---------------+--------+--------+-------+-----------------------+
     | #User | #Item | #Interactions | #Train | #Valid | #Test |        Density        |
     +-------+-------+---------------+--------+--------+-------+-----------------------+
     | 21506 | 15269 |     580420    | 455956 | 56162  | 68302 | 0.0017675517274430242 |
@@ -154,15 +149,14 @@
     -------
     filename: Amazon_Movies_and_TV
     dataset: AmazonMovies
     kcore4user: 10
     kcore4item: 10
     star4pos: 4
     ratios: (7, 1, 2)
-    strict: True
 
     Statistics:
     -----------
     +-------+-------+---------------+--------+--------+-------+-----------------------+
     | #User | #Item | #Interactions | #Train | #Valid | #Test  |        Density        |
     +-------+-------+---------------+--------+--------+--------+-----------------------+
     | 21506 | 15269 |     580420    | 397557 | 58399  | 124464 | 0.0017675517274430242 |
@@ -179,15 +173,14 @@
     -------
     filename: Amazon_Beauty
     dataset: AmazonBeauty
     kcore4user: 10
     kcore4item: 10
     star4pos: 4
     ratios: (8, 1, 1)
-    strict: True
 
     Statistics:
     -----------
     +-------+-------+---------------+--------+--------+-------+----------------------+
     | #User | #Item | #Interactions | #Train | #Valid | #Test |       Density        |
     +-------+-------+---------------+--------+--------+-------+----------------------+
     |  973  |  645  |     19263     | 15008  |  1845  |  2410 | 0.030693850235426277 |
@@ -204,15 +197,14 @@
     -------
     filename: Amazon_Beauty
     dataset: AmazonBeauty
     kcore4user: 10
     kcore4item: 10
     star4pos: 4
     ratios: (8, 1, 1)
-    strict: True
 
     Statistics:
     -----------
     +-------+-------+---------------+--------+--------+-------+----------------------+
     | #User | #Item | #Interactions | #Train | #Valid | #Test |       Density        |
     +-------+-------+---------------+--------+--------+-------+----------------------+
     |  973  |  645  |     19263     | 13063  |  1945  |  4255 | 0.030693850235426277 |
@@ -229,15 +221,14 @@
     -------
     filename: Amazon_Electronics
     dataset: AmazonElectronics
     kcore4user: 10
     kcore4item: 10
     star4pos: 4
     ratios: (8, 1, 1)
-    strict: True
 
     Statistics:
     -----------
     +-------+-------+---------------+--------+--------+-------+----------------------+
     | #User | #Item | #Interactions | #Train | #Valid | #Test |       Density        |
     +-------+-------+---------------+--------+--------+-------+----------------------+
     |  9279 |  6065 |     158979    | 123648 | 14988  | 20343 | 0.002824930586818252 |
@@ -254,15 +245,14 @@
     -------
     filename: Amazon_Electronics
     dataset: AmazonElectronics
     kcore4user: 10
     kcore4item: 10
     star4pos: 4
     ratios: (7, 1, 2)
-    strict: True
 
     Statistics:
     -----------
     +-------+-------+---------------+--------+--------+-------+----------------------+
     | #User | #Item | #Interactions | #Train | #Valid | #Test |       Density        |
     +-------+-------+---------------+--------+--------+-------+----------------------+
     |  9279 |  6065 |     158979    | 107674 | 15974  | 35331 | 0.002824930586818252 |
```

### Comparing `freerec-0.3.1/freerec/data/datasets/general/base.py` & `freerec-0.3.5/freerec/data/datasets/general/base.py`

 * *Files identical despite different names*

### Comparing `freerec-0.3.1/freerec/data/datasets/general/gowalla.py` & `freerec-0.3.5/freerec/data/datasets/general/gowalla.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,14 @@
     -------
     filename: gowalla
     dataset: Gowalla
     kcore4user: 10
     kcore4item: 10
     star4pos: 0
     ratios: (8, 1, 1)
-    strict: True
 
     Statistics:
     -----------
     +-------+-------+---------------+--------+--------+--------+-----------------------+
     | #User | #Item | #Interactions | #Train | #Valid | #Test  |        Density        |
     +-------+-------+---------------+--------+--------+--------+-----------------------+
     | 29858 | 40988 |    1027464    | 810128 | 100508 | 116828 | 0.0008395550395550749 |
@@ -50,15 +49,14 @@
     -------
     filename: gowalla
     dataset: Gowalla
     kcore4user: 10
     kcore4item: 10
     star4pos: 0
     ratios: (8, 1, 1)
-    strict: True
 
     Statistics:
     -----------
     +-------+-------+---------------+--------+--------+--------+-----------------------+
     | #User | #Item | #Interactions | #Train | #Valid | #Test  |        Density        |
     +-------+-------+---------------+--------+--------+--------+-----------------------+
     | 29858 | 40988 |    1027464    | 706338 | 103790 | 217336 | 0.0008395550395550749 |
```

### Comparing `freerec-0.3.1/freerec/data/datasets/general/movielens.py` & `freerec-0.3.5/freerec/data/datasets/general/movielens.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,14 @@
     -------
     filename: ml-100k
     dataset: MovieLens100K
     kcore4user: 10
     kcore4item: 10
     star4pos: 1
     ratios: (8, 1, 1)
-    strict: True
 
     Statistics:
     -----------
     +-------+-------+---------------+--------+--------+-------+---------------------+
     | #User | #Item | #Interactions | #Train | #Valid | #Test |       Density       |
     +-------+-------+---------------+--------+--------+-------+---------------------+
     |  943  |  1152 |     97953     | 77980  |  9744  | 10229 | 0.09016823524213503 |
@@ -51,15 +50,14 @@
     -------
     filename: ml-100k
     dataset: MovieLens100K
     kcore4user: 10
     kcore4item: 10
     star4pos: 1
     ratios: (8, 1, 1)
-    strict: True
 
     Statistics:
     -----------
     +-------+-------+---------------+--------+--------+-------+---------------------+
     | #User | #Item | #Interactions | #Train | #Valid | #Test |       Density       |
     +-------+-------+---------------+--------+--------+-------+---------------------+
     |  943  |  1152 |     97953     | 68156  |  9824  | 19973 | 0.09016823524213503 |
@@ -76,15 +74,14 @@
     -------
     filename: ml-1m
     dataset: MovieLens1M
     kcore4user: 10
     kcore4item: 10
     star4pos: 1
     ratios: (8, 1, 1)
-    strict: True
 
     Statistics:
     -----------
     +-------+-------+---------------+--------+--------+--------+---------------------+
     | #User | #Item | #Interactions | #Train | #Valid | #Test  |       Density       |
     +-------+-------+---------------+--------+--------+--------+---------------------+
     |  6040 |  3260 |     998539    | 796389 | 99549  | 102601 | 0.05071197131597124 |
@@ -101,15 +98,14 @@
     -------
     filename: ml-1m
     dataset: MovieLens1M
     kcore4user: 10
     kcore4item: 10
     star4pos: 1
     ratios: (7, 1, 2)
-    strict: True
 
     Statistics:
     -----------
     +-------+-------+---------------+--------+--------+--------+---------------------+
     | #User | #Item | #Interactions | #Train | #Valid | #Test  |       Density       |
     +-------+-------+---------------+--------+--------+--------+---------------------+
     |  6040 |  3260 |     998539    | 696267 | 100122 | 202150 | 0.05071197131597124 |
```

### Comparing `freerec-0.3.1/freerec/data/datasets/general/yelp.py` & `freerec-0.3.5/freerec/data/datasets/general/yelp.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,14 @@
     -------
     filename: yelp2018
     dataset: Yelp2018
     kcore4user: 10
     kcore4item: 10
     star4pos: 4
     ratios: (8, 1, 1)
-    strict: True
 
     Statistics:
     -----------
     +-------+-------+---------------+--------+--------+--------+-----------------------+
     | #User | #Item | #Interactions | #Train | #Valid | #Test  |        Density        |
     +-------+-------+---------------+--------+--------+--------+-----------------------+
     | 41801 | 26512 |    1022604    | 801621 | 98722  | 122261 | 0.0009227378271017908 |
@@ -50,15 +49,14 @@
     -------
     filename: yelp2018
     dataset: Yelp2018
     kcore4user: 10
     kcore4item: 10
     star4pos: 4
     ratios: (7, 1, 2)
-    strict: True
 
     Statistics:
     -----------
     +-------+-------+---------------+--------+--------+--------+-----------------------+
     | #User | #Item | #Interactions | #Train | #Valid | #Test  |        Density        |
     +-------+-------+---------------+--------+--------+--------+-----------------------+
     | 41801 | 26512 |    1022604    | 698623 | 102998 | 220983 | 0.0009227378271017908 |
```

### Comparing `freerec-0.3.1/freerec/data/datasets/sequential/base.py` & `freerec-0.3.5/freerec/data/datasets/sequential/base.py`

 * *Files identical despite different names*

### Comparing `freerec-0.3.1/freerec/data/datasets/sequential/movielens.py` & `freerec-0.3.5/freerec/data/datasets/sequential/movielens.py`

 * *Files 18% similar despite different names*

```diff
@@ -21,43 +21,41 @@
     Config:
     -------
     filename: ml-1m
     dataset: MovieLens1M
     kcore4user: 5
     kcore4item: 5
     star4pos: 0
-    strict: False
 
     Statistics:
     -----------
     +-------+-------+---------------+--------+--------+-------+----------------------+
     | #User | #Item | #Interactions | #Train | #Valid | #Test |       Density        |
     +-------+-------+---------------+--------+--------+-------+----------------------+
     |  6040 |  3416 |     999611    | 987531 |  6040  |  6040 | 0.048448041549699894 |
     +-------+-------+---------------+--------+--------+-------+----------------------+
     """
-    URL = "https://zenodo.org/record/7684496/files/MovieLens1M_550_Chron.zip"
+    URL = "https://zenodo.org/record/7866203/files/MovieLens1M_550_Chron.zip"
 
 
 class MovieLens1M_500_Chron(UserItemTimeTriplet):
     r"""
     Chronologically-ordered MovieLens1M dataset.
 
     Config:
     -------
     filename: ml-1m
     dataset: MovieLens1M
     kcore4user: 5
     kcore4item: 0
     star4pos: 0
-    strict: False
 
     Statistics:
     -----------
     +-------+-------+---------------+--------+--------+-------+----------------------+
     | #User | #Item | #Interactions | #Train | #Valid | #Test |       Density        |
     +-------+-------+---------------+--------+--------+-------+----------------------+
     |  6040 |  3706 |    1000209    | 988129 |  6040  |  6040 | 0.044683625622312845 |
     +-------+-------+---------------+--------+--------+-------+----------------------+
     """
-    URL = "https://zenodo.org/record/7684496/files/MovieLens1M_500_Chron.zip"
+    URL = "https://zenodo.org/record/7866203/files/MovieLens1M_500_Chron.zip"
```

### Comparing `freerec-0.3.1/freerec/data/datasets/sequential/steam.py` & `freerec-0.3.5/freerec/data/datasets/sequential/steam.py`

 * *Files 13% similar despite different names*

```diff
@@ -20,43 +20,41 @@
     Config:
     -------
     filename: steam
     dataset: Steam
     kcore4user: 5
     kcore4item: 5
     star4pos: 0
-    strict: False
 
     Statistics:
     -----------
-    +-------+-------+---------------+--------+--------+-------+-----------------------+
-    | #User | #Item | #Interactions | #Train | #Valid | #Test |        Density        |
-    +-------+-------+---------------+--------+--------+-------+-----------------------+
-    | 26247 |  8479 |     340353    | 287863 | 26245  | 26245 | 0.0015293443271349354 |
-    +-------+-------+---------------+--------+--------+-------+-----------------------+
+    +-------+-------+---------------+--------+--------+-------+----------------------+
+    | #User | #Item | #Interactions | #Train | #Valid | #Test |       Density        |
+    +-------+-------+---------------+--------+--------+-------+----------------------+
+    | 25389 |  4089 |     328278    | 277500 | 25389  | 25389 | 0.003162125283631449 |
+    +-------+-------+---------------+--------+--------+-------+----------------------+
     """
-    URL = "https://zenodo.org/record/7684496/files/Steam_550_Chron.zip"
+    URL = "https://zenodo.org/record/7866203/files/Steam_550_Chron.zip"
 
 
 class Steam_500_Chron(UserItemTimeTriplet):
     r"""
     Chronologically-ordered MovieLens1M dataset.
 
     Config:
     -------
     filename: steam
     dataset: Steam
     kcore4user: 5
     kcore4item: 0
     star4pos: 0
-    strict: False
 
     Statistics:
     -----------
     +-------+-------+---------------+--------+--------+-------+----------------------+
     | #User | #Item | #Interactions | #Train | #Valid | #Test |       Density        |
     +-------+-------+---------------+--------+--------+-------+----------------------+
     | 26247 |  9327 |     341270    | 288776 | 26247  | 26247 | 0.001394043945100003 |
     +-------+-------+---------------+--------+--------+-------+----------------------+
     """
-    URL = "https://zenodo.org/record/7684496/files/Steam_500_Chron.zip"
+    URL = "https://zenodo.org/record/7866203/files/Steam_500_Chron.zip"
```

### Comparing `freerec-0.3.1/freerec/data/fields.py` & `freerec-0.3.5/freerec/data/fields.py`

 * *Files 1% similar despite different names*

```diff
@@ -182,32 +182,40 @@
         dtype: Optional[Union[torch.dtype, str]] = None,
         non_blocking: bool = False
     ):
         if isinstance(self.data, torch.Tensor):
             self.data = self.data.to(device, dtype, non_blocking)
         return self
 
-    def to_csr(self) -> torch.Tensor:
+    def to_csr(self, length: Optional[int] = None) -> torch.Tensor:
         r"""
         Convert List to CSR Tensor.
 
         Notes:
         ------
         Each row in self.data should be the col indices !
         """
+        data = self.data
+        if isinstance(data, torch.Tensor):
+            data = data.tolist()
+        elif isinstance(data, np.ndarray):
+            data = data.tolist()
+        assert isinstance(data[0], (list, tuple)), f"Each row of data should be `list'|`tuple' but `{type(data[0])}' received ..."
+
+        length = self.count if length is None else length
         crow_indices = np.cumsum([0] + list(map(len, self.data)), dtype=np.int64)
         col_indices = reduce(
-            lambda x, y: x + y, self.data
+            lambda x, y: x + y, data
         )
         values = np.ones_like(col_indices, dtype=np.int64)
         return torch.sparse_csr_tensor(
             crow_indices=crow_indices,
             col_indices=col_indices,
             values=values,
-            size=(len(self.data), self.count) # B x Num of Items
+            size=(len(data), length) # B x Num of Items
         )
 
 
 class FieldModule(Field, torch.nn.Module):
     r"""
     A module that represents a field of data.
```

### Comparing `freerec-0.3.1/freerec/data/postprocessing/base.py` & `freerec-0.3.5/freerec/data/postprocessing/base.py`

 * *Files identical despite different names*

### Comparing `freerec-0.3.1/freerec/data/postprocessing/column.py` & `freerec-0.3.5/freerec/data/postprocessing/column.py`

 * *Files identical despite different names*

### Comparing `freerec-0.3.1/freerec/data/postprocessing/row.py` & `freerec-0.3.5/freerec/data/postprocessing/row.py`

 * *Files 0% similar despite different names*

```diff
@@ -168,15 +168,14 @@
         return row
 
     def __iter__(self):
         for row in self.source:
             yield self._apply_fn(row)
 
 
-dp.iter.Mapper
 @dp.functional_datapipe("lprune_")
 class LeftPruningRow(RowMapper):
     r"""
     A functional datapipe that prunes the left side of a given datapipe to a specified maximum length.
 
     Parameters:
     -----------
```

### Comparing `freerec-0.3.1/freerec/data/postprocessing/sampler.py` & `freerec-0.3.5/freerec/data/postprocessing/sampler.py`

 * *Files 1% similar despite different names*

```diff
@@ -334,14 +334,21 @@
         for chunk in dataset.valid():
             self.listmap(
                 lambda user, item: self.posItems[user].append(item),
                 chunk[USER, ID], chunk[ITEM, ID]
             )
         self.posItems = [tuple(items) for items in self.posItems]
 
+    def __iter__(self):
+        for user in self.source:
+            if self._check(user):
+                posItems = self.posItems[user]
+                # (user, seqs, unseen, seen)
+                yield [user, posItems[:-1], posItems[-1:], posItems[:-1]]
+
 
 @dp.functional_datapipe("seq_test_yielding_")
 class SeqTestYielder(SeqValidYielder):
     r"""
     A functional datapipe for yielding (user, positives, targets).
 
     Parameters:
```

### Comparing `freerec-0.3.1/freerec/data/postprocessing/source.py` & `freerec-0.3.5/freerec/data/postprocessing/source.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from functools import partial
 
 from .base import BaseProcessor
 from ..fields import SparseField
 
 
 __all__ = [
-    'RandomSource', 'OrderedSource',
+    'RandomSource', 'RandomShuffledSource', 'OrderedSource',
     'RandomIDs', 'OrderedIDs', 'DummySource'
 ]
 
 
 class RandomSource(BaseProcessor):
     r"""
     DataPipe that generates random items from given source.
@@ -39,14 +39,37 @@
         self.datasize = datasize
 
     def __iter__(self):
         for _ in range(self.datasize):
             yield self._rng()
 
 
+class RandomShuffledSource(BaseProcessor):
+    r"""
+    DataPipe that generates shuffled source.
+
+    Parameters:
+    -----------
+    source: Iterable 
+        The source data to start.
+    """
+
+    def __init__(self, source) -> None:
+        super().__init__(None)
+
+        self.source = list(source)
+        self._rng = partial(
+            random.shuffle, x=self.source
+        )
+
+    def __iter__(self):
+        self._rng()
+        yield from iter(self.source)
+
+
 class OrderedSource(BaseProcessor):
     r"""
     DataPipe that generates ordered items from given source.
 
     Parameters:
     -----------
     source: Sequence
```

### Comparing `freerec-0.3.1/freerec/data/preprocessing/base.py` & `freerec-0.3.5/freerec/data/preprocessing/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import os, random
 import numpy as np
 import pandas as pd
 from math import floor, ceil
 
 from ..tags import USER, ITEM, RATING, TIMESTAMP
 
-from ...utils import infoLogger, mkdirs
+from ...utils import infoLogger, warnLogger, mkdirs
 
 
 __all__ = ['AtomicConverter']
 
 
 NAME_FORMAT_DICT = {
     'user_id': USER.name,
@@ -69,28 +69,38 @@
         self.path = os.path.join(root, filename)
         if not os.path.exists(self.path) or not any(True for _ in os.scandir(self.path)):
             raise FileNotFoundError(f"No such file of {self.path}, or this dir is empty ...")
 
         self.root = root
         self.dataset = dataset if dataset else self.__class__.__name__
 
-        self._name_format_dict.update(NAME_FORMAT_DICT)
-        self._type_format_dict.update(TYPE_FORMAT_DICT)
+        for key, val in NAME_FORMAT_DICT.items():
+            if self._name_format_dict.get(key, None) is None:
+                self._name_format_dict[key] = val
+        for key, val in TYPE_FORMAT_DICT.items():
+            if self._type_format_dict.get(key, None) is None:
+                self._type_format_dict[key] = val
 
     def convert_by_column(self, df: pd.DataFrame):
         old_columns = df.columns
         new_columns = []
 
         for col in old_columns:
             col = col.lower()
             name_, type_ = col.split(":")
             name_ =  self._name_format_dict.get(name_, name_.capitalize())
             type_ = self._type_format_dict[type_]
-            df[col] = df[col].astype(type_)
-
+            try:
+                df[col] = df[col].astype(type_)
+            except ValueError as e:
+                warnLogger(
+                    f"`{type_}' cannot address field `{col}': \n"
+                    f"\t {e} \n"
+                    f"Skip it ..."
+                )
             new_columns.append(name_)
         
         df.columns = new_columns
         return df
 
     def load_inter_file(self):
         for file_ in os.scandir(self.path):
@@ -222,16 +232,16 @@
         infoLogger(
             f"[Converter] >>> Filter dataframe: "
             f"User in [{low4user}, {high4user}]; "
             f"Item in [{low4item}, {high4item}] ..."
         )
         infoLogger(f"[Converter] >>> Current datasize: {len(df)} ...")
         while dsz != len(df):
-            # filter by user
             dsz = len(df)
+            # filter by user
             users = df[USER.name]
             counts = users.value_counts()
             bool_indices = users.isin(
                 counts[(low4user <= counts) & (counts <= high4user)].index
             )
             df = df[bool_indices]
```

### Comparing `freerec-0.3.1/freerec/data/preprocessing/datasets.py` & `freerec-0.3.5/freerec/data/preprocessing/datasets.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,30 +40,70 @@
         user_id:token	item_id:token	rating:float	timestamp:float
     item:
         item_id:token	categories:token_seq	title:token 	price:float	    sales_type:token	sales_rank:float	brand:token
     """
     filename = "Amazon_Electronics"
 
 
+class AmazonHome(AtomicConverter):
+    r"""
+    inter:
+        user_id:token	item_id:token	rating:float	timestamp:float
+    item:
+        item_id:token	sales_type:token	sales_rank:float	categories:token_seq	title:token	price:float	brand:token
+    """
+    filename = "Amazon_Home_and_Kitchen"
+
+
 class AmazonMovies(AtomicConverter):
     r"""
     inter:
         user_id:token	item_id:token	rating:float	timestamp:float
     item:
         item_id:token	categories:token_seq	title:token	    price:float	    sales_type:token	sales_rank:float	brand:token
     """
     filename = "Amazon_Movies_and_TV"
 
 
+class AmazonOffice(AtomicConverter):
+    r"""
+    inter:
+        user_id:token	item_id:token	rating:float	timestamp:float
+    item:
+        item_id:token	price:float	sales_type:token	sales_rank:float	categories:token_seq	title:token	brand:token
+    """
+    filename = "Amazon_Office_Products"
+
+
+class AmazonTools(AtomicConverter):
+    r"""
+    inter:
+        user_id:token	item_id:token	rating:float	timestamp:float
+    item:
+        item_id:token	categories:token_seq	title:token	price:float	brand:token	sales_type:token	sales_rank:float
+    """
+    filename = "Amazon_Tools_and_Home_Improvement"
+
+
+class AmazonToys(AtomicConverter):
+    r"""
+    inter:
+        user_id:token	item_id:token	rating:float	timestamp:float
+    item:
+        item_id:token	title:token	price:float	sales_type:token	sales_rank:float	brand:token	categories:token_seq
+    """
+    filename = "Amazon_Toys_and_Games"
+
+
 class AmazonGames(AtomicConverter):
     r"""
     inter:
         user_id:token	item_id:token	rating:float	timestamp:float
     item:
-        item_id:token	price:float	    sales_type:token	sales_rank:float	categories:token_seq	title:token	brand:token
+        item_id:token	price:float	sales_type:token	sales_rank:float	categories:token_seq	title:token	brand:token
     """
     filename = "Amazon_Video_Games"
 
 
 class FourSquareNYC(AtomicConverter):
     r"""
     inter:
```

### Comparing `freerec-0.3.1/freerec/data/tags.py` & `freerec-0.3.5/freerec/data/tags.py`

 * *Files identical despite different names*

### Comparing `freerec-0.3.1/freerec/data/transformation.py` & `freerec-0.3.5/freerec/data/transformation.py`

 * *Files identical despite different names*

### Comparing `freerec-0.3.1/freerec/data/utils.py` & `freerec-0.3.5/freerec/data/utils.py`

 * *Files identical despite different names*

### Comparing `freerec-0.3.1/freerec/dict2obj.py` & `freerec-0.3.5/freerec/dict2obj.py`

 * *Files identical despite different names*

### Comparing `freerec-0.3.1/freerec/launcher.py` & `freerec-0.3.5/freerec/launcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -282,1657 +282,1678 @@
 00001190: 2073 656c 662e 6669 656c 6473 3a20 4669   self.fields: Fi
 000011a0: 656c 6454 7570 6c65 5b46 6965 6c64 4d6f  eldTuple[FieldMo
 000011b0: 6475 6c65 5d20 3d20 4669 656c 6454 7570  dule] = FieldTup
 000011c0: 6c65 2866 6965 6c64 7329 0d0a 2020 2020  le(fields)..    
 000011d0: 2020 2020 7365 6c66 2e64 6576 6963 6520      self.device 
 000011e0: 3d20 746f 7263 682e 6465 7669 6365 2864  = torch.device(d
 000011f0: 6576 6963 6529 0d0a 2020 2020 2020 2020  evice)..        
-00001200: 746f 7263 682e 6375 6461 2e73 6574 5f64  torch.cuda.set_d
-00001210: 6576 6963 6528 7365 6c66 2e64 6576 6963  evice(self.devic
-00001220: 6529 0d0a 0d0a 2020 2020 2020 2020 7365  e)....        se
-00001230: 6c66 2e5f 7365 745f 6461 7461 7069 7065  lf._set_datapipe
-00001240: 2874 7261 696e 7069 7065 2c20 7661 6c69  (trainpipe, vali
-00001250: 6470 6970 652c 2074 6573 7470 6970 6529  dpipe, testpipe)
-00001260: 0d0a 2020 2020 2020 2020 7365 6c66 2e5f  ..        self._
-00001270: 7365 745f 6f74 6865 7228 6d6f 6465 6c2c  set_other(model,
-00001280: 2063 7269 7465 7269 6f6e 2c20 6f70 7469   criterion, opti
-00001290: 6d69 7a65 722c 206c 725f 7363 6865 6475  mizer, lr_schedu
-000012a0: 6c65 7229 0d0a 0d0a 2020 2020 2020 2020  ler)....        
-000012b0: 7365 6c66 2e5f 5f6d 6f64 6520 3d20 2774  self.__mode = 't
-000012c0: 7261 696e 270d 0a0d 0a20 2020 2020 2020  rain'....       
-000012d0: 2064 6566 2063 6c65 616e 2829 3a0d 0a20   def clean():.. 
-000012e0: 2020 2020 2020 2020 2020 2070 6172 656e             paren
-000012f0: 7420 3d20 7073 7574 696c 2e50 726f 6365  t = psutil.Proce
-00001300: 7373 286f 732e 6765 7470 6964 2829 290d  ss(os.getpid()).
-00001310: 0a20 2020 2020 2020 2020 2020 2063 6869  .            chi
-00001320: 6c64 7265 6e20 3d20 7061 7265 6e74 2e63  ldren = parent.c
-00001330: 6869 6c64 7265 6e28 7265 6375 7273 6976  hildren(recursiv
-00001340: 653d 5472 7565 290d 0a20 2020 2020 2020  e=True)..       
-00001350: 2020 2020 2066 6f72 2070 726f 6365 7373       for process
-00001360: 2069 6e20 6368 696c 6472 656e 3a0d 0a20   in children:.. 
-00001370: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00001380: 726f 6365 7373 2e73 656e 645f 7369 676e  rocess.send_sign
-00001390: 616c 2873 6967 6e61 6c2e 5349 4754 4552  al(signal.SIGTER
-000013a0: 4d29 0d0a 2020 2020 2020 2020 2020 2020  M)..            
-000013b0: 7073 7574 696c 2e77 6169 745f 7072 6f63  psutil.wait_proc
-000013c0: 7328 6368 696c 6472 656e 2c20 7469 6d65  s(children, time
-000013d0: 6f75 743d 3529 0d0a 0d0a 2020 2020 2020  out=5)....      
-000013e0: 2020 6174 6578 6974 2e72 6567 6973 7465    atexit.registe
-000013f0: 7228 636c 6561 6e29 0d0a 0d0a 2020 2020  r(clean)....    
-00001400: 6465 6620 5f73 6574 5f64 6174 6170 6970  def _set_datapip
-00001410: 6528 0d0a 2020 2020 2020 2020 7365 6c66  e(..        self
-00001420: 2c0d 0a20 2020 2020 2020 2074 7261 696e  ,..        train
-00001430: 7069 7065 2c0d 0a20 2020 2020 2020 2076  pipe,..        v
-00001440: 616c 6964 7069 7065 3d4e 6f6e 652c 0d0a  alidpipe=None,..
-00001450: 2020 2020 2020 2020 7465 7374 7069 7065          testpipe
-00001460: 3d4e 6f6e 652c 0d0a 2020 2020 293a 0d0a  =None,..    ):..
-00001470: 2020 2020 2020 2020 2222 2253 6574 2074          """Set t
-00001480: 6865 2064 6174 6120 7069 7065 2066 6f72  he data pipe for
-00001490: 2074 7261 696e 696e 672c 2076 616c 6964   training, valid
-000014a0: 6174 696f 6e20 616e 6420 7465 7374 2e22  ation and test."
-000014b0: 2222 0d0a 2020 2020 2020 2020 7365 6c66  ""..        self
-000014c0: 2e74 7261 696e 7069 7065 203d 2074 7261  .trainpipe = tra
-000014d0: 696e 7069 7065 0d0a 2020 2020 2020 2020  inpipe..        
-000014e0: 7365 6c66 2e76 616c 6964 7069 7065 203d  self.validpipe =
-000014f0: 2073 656c 662e 7472 6169 6e70 6970 6520   self.trainpipe 
-00001500: 6966 2076 616c 6964 7069 7065 2069 7320  if validpipe is 
-00001510: 4e6f 6e65 2065 6c73 6520 7661 6c69 6470  None else validp
-00001520: 6970 650d 0a20 2020 2020 2020 2073 656c  ipe..        sel
-00001530: 662e 7465 7374 7069 7065 203d 2073 656c  f.testpipe = sel
-00001540: 662e 7661 6c69 6470 6970 6520 6966 2074  f.validpipe if t
-00001550: 6573 7470 6970 6520 6973 204e 6f6e 6520  estpipe is None 
-00001560: 656c 7365 2074 6573 7470 6970 650d 0a0d  else testpipe...
-00001570: 0a20 2020 2064 6566 205f 7365 745f 6f74  .    def _set_ot
-00001580: 6865 7228 0d0a 2020 2020 2020 2020 7365  her(..        se
-00001590: 6c66 2c0d 0a20 2020 2020 2020 206d 6f64  lf,..        mod
-000015a0: 656c 3d4e 6f6e 652c 2063 7269 7465 7269  el=None, criteri
-000015b0: 6f6e 3d4e 6f6e 652c 206f 7074 696d 697a  on=None, optimiz
-000015c0: 6572 3d4e 6f6e 652c 206c 725f 7363 6865  er=None, lr_sche
-000015d0: 6475 6c65 723d 4e6f 6e65 2c0d 0a20 2020  duler=None,..   
-000015e0: 2029 3a0d 0a20 2020 2020 2020 2022 2222   ):..        """
-000015f0: 5365 7420 7468 6520 6f74 6865 7220 6e65  Set the other ne
-00001600: 6365 7373 6172 7920 636f 6d70 6f6e 656e  cessary componen
-00001610: 7473 2e22 2222 0d0a 2020 2020 2020 2020  ts."""..        
-00001620: 7365 6c66 2e63 7269 7465 7269 6f6e 203d  self.criterion =
-00001630: 2063 7269 7465 7269 6f6e 0d0a 2020 2020   criterion..    
-00001640: 2020 2020 7365 6c66 2e6d 6f64 656c 203d      self.model =
-00001650: 206d 6f64 656c 2e74 6f28 7365 6c66 2e64   model.to(self.d
-00001660: 6576 6963 6529 2069 6620 6d6f 6465 6c20  evice) if model 
-00001670: 656c 7365 205f 4475 6d6d 794d 6f64 756c  else _DummyModul
-00001680: 6528 290d 0a20 2020 2020 2020 2073 656c  e()..        sel
-00001690: 662e 6f70 7469 6d69 7a65 7220 3d20 6f70  f.optimizer = op
-000016a0: 7469 6d69 7a65 7220 6966 206f 7074 696d  timizer if optim
-000016b0: 697a 6572 2065 6c73 6520 5f44 756d 6d79  izer else _Dummy
-000016c0: 4d6f 6475 6c65 2829 0d0a 2020 2020 2020  Module()..      
-000016d0: 2020 7365 6c66 2e6c 725f 7363 6865 6475    self.lr_schedu
-000016e0: 6c65 7220 3d20 6c72 5f73 6368 6564 756c  ler = lr_schedul
-000016f0: 6572 2069 6620 6c72 5f73 6368 6564 756c  er if lr_schedul
-00001700: 6572 2065 6c73 6520 5f44 756d 6d79 4d6f  er else _DummyMo
-00001710: 6475 6c65 2829 0d0a 0d0a 2020 2020 4070  dule()....    @p
-00001720: 726f 7065 7274 790d 0a20 2020 2064 6566  roperty..    def
-00001730: 206d 6f64 6528 7365 6c66 293a 0d0a 2020   mode(self):..  
-00001740: 2020 2020 2020 2222 2247 6574 2074 6865        """Get the
-00001750: 2063 7572 7265 6e74 206d 6f64 6520 6f66   current mode of
-00001760: 2074 6865 2063 6869 6566 2063 6f61 6368   the chief coach
-00001770: 2e22 2222 0d0a 2020 2020 2020 2020 7265  ."""..        re
-00001780: 7475 726e 2073 656c 662e 5f5f 6d6f 6465  turn self.__mode
-00001790: 0d0a 0d0a 2020 2020 4074 696d 656d 6574  ....    @timemet
-000017a0: 6572 2822 436f 6163 682f 7472 6169 6e22  er("Coach/train"
-000017b0: 290d 0a20 2020 2064 6566 2074 7261 696e  )..    def train
-000017c0: 2873 656c 662c 2065 706f 6368 3a20 696e  (self, epoch: in
-000017d0: 7429 3a0d 0a20 2020 2020 2020 2022 2222  t):..        """
-000017e0: 5374 6172 7420 7472 6169 6e69 6e67 2061  Start training a
-000017f0: 6e64 2072 6574 7572 6e20 7468 6520 7472  nd return the tr
-00001800: 6169 6e69 6e67 206c 6f73 732e 2222 220d  aining loss.""".
-00001810: 0a20 2020 2020 2020 2073 656c 662e 5f5f  .        self.__
-00001820: 6d6f 6465 203d 2027 7472 6169 6e27 0d0a  mode = 'train'..
-00001830: 2020 2020 2020 2020 7365 6c66 2e6d 6f64          self.mod
-00001840: 656c 2e74 7261 696e 2829 0d0a 2020 2020  el.train()..    
-00001850: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-00001860: 7472 6169 6e5f 7065 725f 6570 6f63 6828  train_per_epoch(
-00001870: 6570 6f63 6829 0d0a 0d0a 2020 2020 4074  epoch)....    @t
-00001880: 696d 656d 6574 6572 2822 436f 6163 682f  imemeter("Coach/
-00001890: 7661 6c69 6422 290d 0a20 2020 2040 746f  valid")..    @to
-000018a0: 7263 682e 6e6f 5f67 7261 6428 290d 0a20  rch.no_grad().. 
-000018b0: 2020 2064 6566 2076 616c 6964 2873 656c     def valid(sel
-000018c0: 662c 2065 706f 6368 3a20 696e 7429 3a0d  f, epoch: int):.
-000018d0: 0a20 2020 2020 2020 2022 2222 5374 6172  .        """Star
-000018e0: 7420 7661 6c69 6461 7469 6f6e 2061 6e64  t validation and
-000018f0: 2072 6574 7572 6e20 7468 6520 7661 6c69   return the vali
-00001900: 6461 7469 6f6e 206d 6574 7269 6373 2e22  dation metrics."
-00001910: 2222 0d0a 2020 2020 2020 2020 7365 6c66  ""..        self
-00001920: 2e5f 5f6d 6f64 6520 3d20 2776 616c 6964  .__mode = 'valid
-00001930: 270d 0a20 2020 2020 2020 2073 656c 662e  '..        self.
-00001940: 6d6f 6465 6c2e 6576 616c 2829 0d0a 2020  model.eval()..  
-00001950: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-00001960: 662e 6576 616c 7561 7465 2865 706f 6368  f.evaluate(epoch
-00001970: 3d65 706f 6368 2c20 7072 6566 6978 3d27  =epoch, prefix='
-00001980: 7661 6c69 6427 290d 0a0d 0a20 2020 2040  valid')....    @
-00001990: 7469 6d65 6d65 7465 7228 2243 6f61 6368  timemeter("Coach
-000019a0: 2f74 6573 7422 290d 0a20 2020 2040 746f  /test")..    @to
-000019b0: 7263 682e 6e6f 5f67 7261 6428 290d 0a20  rch.no_grad().. 
-000019c0: 2020 2064 6566 2074 6573 7428 7365 6c66     def test(self
-000019d0: 2c20 6570 6f63 683a 2069 6e74 293a 0d0a  , epoch: int):..
-000019e0: 2020 2020 2020 2020 2222 2253 7461 7274          """Start
-000019f0: 2074 6573 7469 6e67 2061 6e64 2072 6574   testing and ret
-00001a00: 7572 6e20 7468 6520 7465 7374 206d 6574  urn the test met
-00001a10: 7269 6373 2e22 2222 0d0a 2020 2020 2020  rics."""..      
-00001a20: 2020 7365 6c66 2e5f 5f6d 6f64 6520 3d20    self.__mode = 
-00001a30: 2774 6573 7427 0d0a 2020 2020 2020 2020  'test'..        
-00001a40: 7365 6c66 2e6d 6f64 656c 2e65 7661 6c28  self.model.eval(
-00001a50: 290d 0a20 2020 2020 2020 2072 6574 7572  )..        retur
-00001a60: 6e20 7365 6c66 2e65 7661 6c75 6174 6528  n self.evaluate(
-00001a70: 6570 6f63 683d 6570 6f63 682c 2070 7265  epoch=epoch, pre
-00001a80: 6669 783d 2774 6573 7427 290d 0a0d 0a20  fix='test').... 
-00001a90: 2020 2040 6162 632e 6162 7374 7261 6374     @abc.abstract
-00001aa0: 6d65 7468 6f64 0d0a 2020 2020 6465 6620  method..    def 
-00001ab0: 7472 6169 6e5f 7065 725f 6570 6f63 6828  train_per_epoch(
-00001ac0: 7365 6c66 2c20 6570 6f63 683a 2069 6e74  self, epoch: int
-00001ad0: 293a 0d0a 2020 2020 2020 2020 7261 6973  ):..        rais
-00001ae0: 6520 4e6f 7449 6d70 6c65 6d65 6e74 6564  e NotImplemented
-00001af0: 4572 726f 7228 0d0a 2020 2020 2020 2020  Error(..        
-00001b00: 2020 2020 6622 7b73 656c 662e 5f5f 636c      f"{self.__cl
-00001b10: 6173 735f 5f2e 5f5f 6e61 6d65 5f5f 7d2e  ass__.__name__}.
-00001b20: 7472 6169 6e5f 7065 725f 6570 6f63 6828  train_per_epoch(
-00001b30: 2920 7368 6f75 6c64 2062 6520 696d 706c  ) should be impl
-00001b40: 656d 656e 7465 6420 2e2e 2e22 0d0a 2020  emented ..."..  
-00001b50: 2020 2020 2020 290d 0a0d 0a20 2020 2040        )....    @
-00001b60: 6162 632e 6162 7374 7261 6374 6d65 7468  abc.abstractmeth
-00001b70: 6f64 0d0a 2020 2020 6465 6620 6576 616c  od..    def eval
-00001b80: 7561 7465 2873 656c 662c 2065 706f 6368  uate(self, epoch
-00001b90: 3a20 696e 742c 2070 7265 6669 783a 2073  : int, prefix: s
-00001ba0: 7472 203d 2027 7661 6c69 6427 293a 0d0a  tr = 'valid'):..
-00001bb0: 2020 2020 2020 2020 7261 6973 6520 4e6f          raise No
-00001bc0: 7449 6d70 6c65 6d65 6e74 6564 4572 726f  tImplementedErro
-00001bd0: 7228 0d0a 2020 2020 2020 2020 2020 2020  r(..            
-00001be0: 6622 7b73 656c 662e 5f5f 636c 6173 735f  f"{self.__class_
-00001bf0: 5f2e 5f5f 6e61 6d65 5f5f 7d2e 6576 616c  _.__name__}.eval
-00001c00: 7561 7465 2829 2073 686f 756c 6420 6265  uate() should be
-00001c10: 2069 6d70 6c65 6d65 6e74 6564 202e 2e2e   implemented ...
-00001c20: 220d 0a20 2020 2020 2020 2029 0d0a 0d0a  "..        )....
-00001c30: 2020 2020 6465 6620 7265 6769 7374 6572      def register
-00001c40: 5f6d 6574 7269 6328 0d0a 2020 2020 2020  _metric(..      
-00001c50: 2020 7365 6c66 2c20 6e61 6d65 3a20 7374    self, name: st
-00001c60: 722c 2066 756e 633a 2043 616c 6c61 626c  r, func: Callabl
-00001c70: 652c 200d 0a20 2020 2020 2020 2066 6d74  e, ..        fmt
-00001c80: 3a20 7374 7220 3d20 272e 3466 272c 2062  : str = '.4f', b
-00001c90: 6573 745f 6361 7374 6572 3a20 4361 6c6c  est_caster: Call
-00001ca0: 6162 6c65 203d 206d 6178 0d0a 2020 2020  able = max..    
-00001cb0: 2920 2d3e 204e 6f6e 653a 0d0a 2020 2020  ) -> None:..    
-00001cc0: 2020 2020 7222 2222 0d0a 2020 2020 2020      r"""..      
-00001cd0: 2020 5265 6769 7374 6572 2061 206d 6574    Register a met
-00001ce0: 7269 632e 0d0a 0d0a 2020 2020 2020 2020  ric.....        
-00001cf0: 5061 7261 6d65 7465 7273 0d0a 2020 2020  Parameters..    
-00001d00: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a      ----------..
-00001d10: 2020 2020 2020 2020 6e61 6d65 203a 2073          name : s
-00001d20: 7472 0d0a 2020 2020 2020 2020 2020 2020  tr..            
-00001d30: 5468 6520 636f 6d70 6c65 7465 206e 616d  The complete nam
-00001d40: 6520 6f66 2074 6865 206d 6574 7269 632c  e of the metric,
-00001d50: 2073 7563 6820 6173 2060 4c4f 5353 3260   such as `LOSS2`
-00001d60: 2e0d 0a20 2020 2020 2020 2020 2020 2054  ...            T
-00001d70: 6865 206e 6f74 6174 696f 6e20 6040 6020  he notation `@` 
-00001d80: 7368 6f75 6c64 206e 6f74 2062 6520 696e  should not be in
-00001d90: 636c 7564 6564 2c20 692e 652e 2c20 274c  cluded, i.e., 'L
-00001da0: 4f53 5340 3227 2069 7320 696e 7661 6c69  OSS@2' is invali
-00001db0: 642e 0d0a 2020 2020 2020 2020 6675 6e63  d...        func
-00001dc0: 203a 2043 616c 6c61 626c 650d 0a20 2020   : Callable..   
-00001dd0: 2020 2020 2020 2020 2054 6865 2066 756e           The fun
-00001de0: 6374 696f 6e20 746f 2070 726f 6365 7373  ction to process
-00001df0: 2074 6865 2064 6174 6120 666f 7220 7468   the data for th
-00001e00: 6520 6d65 7472 6963 2e0d 0a20 2020 2020  e metric...     
-00001e10: 2020 2066 6d74 203a 2073 7472 2c20 6f70     fmt : str, op
-00001e20: 7469 6f6e 616c 0d0a 2020 2020 2020 2020  tional..        
-00001e30: 2020 2020 5468 6520 666f 726d 6174 2074      The format t
-00001e40: 6f20 7573 6520 7768 656e 2070 7269 6e74  o use when print
-00001e50: 696e 6720 7468 6520 6d65 7472 6963 2c20  ing the metric, 
-00001e60: 6465 6661 756c 7473 2074 6f20 6027 2e34  defaults to `'.4
-00001e70: 6627 602e 0d0a 2020 2020 2020 2020 6265  f'`...        be
-00001e80: 7374 5f63 6173 7465 7220 3a20 4361 6c6c  st_caster : Call
-00001e90: 6162 6c65 2c20 6f70 7469 6f6e 616c 0d0a  able, optional..
-00001ea0: 2020 2020 2020 2020 2020 2020 4120 6675              A fu
-00001eb0: 6e63 7469 6f6e 2075 7365 6420 746f 2063  nction used to c
-00001ec0: 6173 7420 7468 6520 6265 7374 2076 616c  ast the best val
-00001ed0: 7565 206f 6620 7468 6520 6d65 7472 6963  ue of the metric
-00001ee0: 2c20 6465 6661 756c 7473 2074 6f20 606d  , defaults to `m
-00001ef0: 6178 602e 0d0a 2020 2020 2020 2020 2020  ax`...          
-00001f00: 2020 0d0a 2020 2020 2020 2020 5265 7475    ..        Retu
-00001f10: 726e 730d 0a20 2020 2020 2020 202d 2d2d  rns..        ---
-00001f20: 2d2d 2d2d 0d0a 2020 2020 2020 2020 4e6f  ----..        No
-00001f30: 6e65 0d0a 2020 2020 2020 2020 0d0a 2020  ne..        ..  
-00001f40: 2020 2020 2020 5261 6973 6573 0d0a 2020        Raises..  
-00001f50: 2020 2020 2020 2d2d 2d2d 2d2d 0d0a 2020        ------..  
-00001f60: 2020 2020 2020 4173 7365 7274 696f 6e45        AssertionE
-00001f70: 7272 6f72 0d0a 2020 2020 2020 2020 2020  rror..          
-00001f80: 2020 5768 656e 2060 6e61 6d65 6020 6861    When `name` ha
-00001f90: 7320 616c 7265 6164 7920 6265 656e 2072  s already been r
-00001fa0: 6567 6973 7465 7265 6420 6f72 2063 6f6e  egistered or con
-00001fb0: 7461 696e 7320 7468 6520 6e6f 7461 7469  tains the notati
-00001fc0: 6f6e 2060 4060 2e0d 0a20 2020 2020 2020  on `@`...       
-00001fd0: 2022 2222 0d0a 0d0a 2020 2020 2020 2020   """....        
-00001fe0: 6e61 6d65 203d 206e 616d 652e 7570 7065  name = name.uppe
-00001ff0: 7228 290d 0a20 2020 2020 2020 2061 7373  r()..        ass
-00002000: 6572 7420 4445 4641 554c 545f 4d45 5452  ert DEFAULT_METR
-00002010: 4943 532e 6765 7428 6e61 6d65 2c20 4e6f  ICS.get(name, No
-00002020: 6e65 2920 6973 204e 6f6e 652c 2066 2254  ne) is None, f"T
-00002030: 6865 206d 6574 7269 6320 7b6e 616d 657d  he metric {name}
-00002040: 2061 6c72 6561 6479 2065 7869 7374 7320   already exists 
-00002050: 2e2e 2e22 0d0a 2020 2020 2020 2020 6173  ..."..        as
-00002060: 7365 7274 2027 4027 206e 6f74 2069 6e20  sert '@' not in 
-00002070: 6e61 6d65 2c20 6622 5468 6520 6d65 7472  name, f"The metr
-00002080: 6963 206e 616d 6520 6861 7320 696e 7661  ic name has inva
-00002090: 6c69 6420 6e6f 7461 7469 6f6e 206f 6620  lid notation of 
-000020a0: 6040 2720 2e2e 2e22 0d0a 2020 2020 2020  `@' ..."..      
-000020b0: 2020 4445 4641 554c 545f 4d45 5452 4943    DEFAULT_METRIC
-000020c0: 535b 6e61 6d65 5d20 3d20 6675 6e63 0d0a  S[name] = func..
-000020d0: 2020 2020 2020 2020 4445 4641 554c 545f          DEFAULT_
-000020e0: 464d 5453 5b6e 616d 655d 203d 2066 6d74  FMTS[name] = fmt
-000020f0: 0d0a 2020 2020 2020 2020 4445 4641 554c  ..        DEFAUL
-00002100: 545f 4245 5354 5f43 4153 5445 525b 6e61  T_BEST_CASTER[na
-00002110: 6d65 5d20 3d20 6265 7374 5f63 6173 7465  me] = best_caste
-00002120: 720d 0a0d 0a0d 0a63 6c61 7373 2043 6f61  r......class Coa
-00002130: 6368 2843 6869 6566 436f 6163 6829 3a0d  ch(ChiefCoach):.
-00002140: 0a20 2020 2022 2222 5468 6520 6672 616d  .    """The fram
-00002150: 6577 6f72 6b20 666f 7220 7472 6169 6e69  ework for traini
-00002160: 6e67 2e22 2222 0d0a 0d0a 2020 2020 6465  ng."""....    de
-00002170: 6620 7072 6570 6172 655f 6461 7461 6c6f  f prepare_datalo
-00002180: 6164 6572 2873 656c 6629 202d 3e20 4e6f  ader(self) -> No
-00002190: 6e65 3a0d 0a20 2020 2020 2020 2022 2222  ne:..        """
-000021a0: 5072 6570 6172 6520 6461 7461 206c 6f61  Prepare data loa
-000021b0: 6465 7273 2066 6f72 2074 7261 696e 696e  ders for trainin
-000021c0: 672c 2076 616c 6964 6174 696f 6e2c 2061  g, validation, a
-000021d0: 6e64 2074 6573 7469 6e67 2064 6174 612e  nd testing data.
-000021e0: 2222 220d 0a20 2020 2020 2020 2073 656c  """..        sel
-000021f0: 662e 7472 6169 6e6c 6f61 6465 7220 3d20  f.trainloader = 
-00002200: 4461 7461 4c6f 6164 6572 280d 0a20 2020  DataLoader(..   
-00002210: 2020 2020 2020 2020 2064 6174 6170 6970           datapip
-00002220: 653d 7365 6c66 2e74 7261 696e 7069 7065  e=self.trainpipe
-00002230: 2c20 0d0a 2020 2020 2020 2020 2020 2020  , ..            
-00002240: 6e75 6d5f 776f 726b 6572 733d 7365 6c66  num_workers=self
-00002250: 2e63 6667 2e6e 756d 5f77 6f72 6b65 7273  .cfg.num_workers
-00002260: 2c0d 0a20 2020 2020 2020 2020 2020 2070  ,..            p
-00002270: 696e 5f6d 656d 6f72 793d 7365 6c66 2e63  in_memory=self.c
-00002280: 6667 2e70 696e 5f6d 656d 6f72 790d 0a20  fg.pin_memory.. 
-00002290: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
-000022a0: 2020 7365 6c66 2e76 616c 6964 6c6f 6164    self.validload
-000022b0: 6572 203d 2044 6174 614c 6f61 6465 7228  er = DataLoader(
-000022c0: 0d0a 2020 2020 2020 2020 2020 2020 6461  ..            da
-000022d0: 7461 7069 7065 3d73 656c 662e 7661 6c69  tapipe=self.vali
-000022e0: 6470 6970 652c 200d 0a20 2020 2020 2020  dpipe, ..       
-000022f0: 2020 2020 206e 756d 5f77 6f72 6b65 7273       num_workers
-00002300: 3d73 656c 662e 6366 672e 6e75 6d5f 776f  =self.cfg.num_wo
-00002310: 726b 6572 732c 0d0a 2020 2020 2020 2020  rkers,..        
-00002320: 2020 2020 7069 6e5f 6d65 6d6f 7279 3d73      pin_memory=s
-00002330: 656c 662e 6366 672e 7069 6e5f 6d65 6d6f  elf.cfg.pin_memo
-00002340: 7279 0d0a 2020 2020 2020 2020 290d 0a20  ry..        ).. 
-00002350: 2020 2020 2020 2073 656c 662e 7465 7374         self.test
-00002360: 6c6f 6164 6572 203d 2044 6174 614c 6f61  loader = DataLoa
-00002370: 6465 7228 0d0a 2020 2020 2020 2020 2020  der(..          
-00002380: 2020 6461 7461 7069 7065 3d73 656c 662e    datapipe=self.
-00002390: 7465 7374 7069 7065 2c20 0d0a 2020 2020  testpipe, ..    
-000023a0: 2020 2020 2020 2020 6e75 6d5f 776f 726b          num_work
-000023b0: 6572 733d 7365 6c66 2e63 6667 2e6e 756d  ers=self.cfg.num
-000023c0: 5f77 6f72 6b65 7273 2c0d 0a20 2020 2020  _workers,..     
-000023d0: 2020 2020 2020 2070 696e 5f6d 656d 6f72         pin_memor
-000023e0: 793d 7365 6c66 2e63 6667 2e70 696e 5f6d  y=self.cfg.pin_m
-000023f0: 656d 6f72 790d 0a20 2020 2020 2020 2029  emory..        )
-00002400: 0d0a 2020 2020 0d0a 2020 2020 4070 726f  ..    ..    @pro
-00002410: 7065 7274 790d 0a20 2020 2064 6566 2064  perty..    def d
-00002420: 6174 616c 6f61 6465 7228 7365 6c66 293a  ataloader(self):
-00002430: 0d0a 2020 2020 2020 2020 2222 2252 6574  ..        """Ret
-00002440: 7572 6e20 7468 6520 636f 7272 6573 706f  urn the correspo
-00002450: 6e64 696e 6720 6461 7461 206c 6f61 6465  nding data loade
-00002460: 7220 6465 7065 6e64 696e 6720 6f6e 2074  r depending on t
-00002470: 6865 2063 7572 7265 6e74 206d 6f64 652e  he current mode.
-00002480: 2222 220d 0a20 2020 2020 2020 2069 6620  """..        if 
-00002490: 7365 6c66 2e6d 6f64 6520 3d3d 2027 7472  self.mode == 'tr
-000024a0: 6169 6e27 3a0d 0a20 2020 2020 2020 2020  ain':..         
-000024b0: 2020 2072 6574 7572 6e20 7365 6c66 2e74     return self.t
-000024c0: 7261 696e 6c6f 6164 6572 0d0a 2020 2020  rainloader..    
-000024d0: 2020 2020 656c 6966 2073 656c 662e 6d6f      elif self.mo
-000024e0: 6465 203d 3d20 2776 616c 6964 273a 0d0a  de == 'valid':..
-000024f0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00002500: 726e 2073 656c 662e 7661 6c69 646c 6f61  rn self.validloa
-00002510: 6465 720d 0a20 2020 2020 2020 2065 6c73  der..        els
-00002520: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-00002530: 7265 7475 726e 2073 656c 662e 7465 7374  return self.test
-00002540: 6c6f 6164 6572 0d0a 0d0a 2020 2020 4070  loader....    @p
-00002550: 726f 7065 7274 790d 0a20 2020 2064 6566  roperty..    def
-00002560: 206d 6f6e 6974 6f72 7328 7365 6c66 2920   monitors(self) 
-00002570: 2d3e 204d 6f6e 6974 6f72 3a0d 0a20 2020  -> Monitor:..   
-00002580: 2020 2020 2022 2222 5265 7475 726e 2074       """Return t
-00002590: 6865 206d 6f6e 6974 6f72 2064 6963 7469  he monitor dicti
-000025a0: 6f6e 6172 7920 666f 7220 7468 6520 6469  onary for the di
-000025b0: 6666 6572 656e 7420 6d6f 6465 7320 2827  fferent modes ('
-000025c0: 7472 6169 6e27 2c20 2776 616c 6964 272c  train', 'valid',
-000025d0: 2027 7465 7374 2729 2e22 2222 0d0a 2020   'test')."""..  
-000025e0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-000025f0: 662e 5f5f 6d6f 6e69 746f 7273 0d0a 0d0a  f.__monitors....
-00002600: 2020 2020 4070 726f 7065 7274 790d 0a20      @property.. 
-00002610: 2020 2064 6566 206d 6574 6572 3462 6573     def meter4bes
-00002620: 7428 7365 6c66 293a 0d0a 2020 2020 2020  t(self):..      
-00002630: 2020 7265 7475 726e 2073 656c 662e 5f5f    return self.__
-00002640: 6265 7374 5f6d 6574 6572 0d0a 0d0a 2020  best_meter....  
-00002650: 2020 406d 6574 6572 3462 6573 742e 7365    @meter4best.se
-00002660: 7474 6572 0d0a 2020 2020 6465 6620 6d65  tter..    def me
-00002670: 7465 7234 6265 7374 2873 656c 662c 206d  ter4best(self, m
-00002680: 6574 6572 3a20 4176 6572 6167 654d 6574  eter: AverageMet
-00002690: 6572 293a 0d0a 2020 2020 2020 2020 7365  er):..        se
-000026a0: 6c66 2e5f 5f62 6573 745f 6d65 7465 7220  lf.__best_meter 
-000026b0: 3d20 6d65 7465 720d 0a20 2020 2020 2020  = meter..       
-000026c0: 2069 6e66 6f4c 6f67 6765 7228 6622 5b43   infoLogger(f"[C
-000026d0: 6f61 6368 5d20 3e3e 3e20 5365 7420 6265  oach] >>> Set be
-000026e0: 7374 206d 6574 6572 3a20 7b6d 6574 6572  st meter: {meter
-000026f0: 2e6e 616d 657d 2022 290d 0a0d 0a20 2020  .name} ")....   
-00002700: 2040 7469 6d65 6d65 7465 7228 2243 6f61   @timemeter("Coa
-00002710: 6368 2f63 6f6d 7069 6c65 2229 0d0a 2020  ch/compile")..  
-00002720: 2020 6465 6620 636f 6d70 696c 6528 0d0a    def compile(..
-00002730: 2020 2020 2020 2020 7365 6c66 2c20 6366          self, cf
-00002740: 673a 2043 6f6e 6669 672c 206d 6f6e 6974  g: Config, monit
-00002750: 6f72 733a 204c 6973 745b 7374 725d 2c20  ors: List[str], 
-00002760: 0d0a 2020 2020 2020 2020 7768 6963 6834  ..        which4
-00002770: 6265 7374 3a20 7374 7220 3d20 274c 4f53  best: str = 'LOS
-00002780: 5327 0d0a 2020 2020 293a 0d0a 2020 2020  S'..    ):..    
-00002790: 2020 2020 7222 2222 0d0a 2020 2020 2020      r"""..      
-000027a0: 2020 4c6f 6164 2074 6865 2063 6f6e 6669    Load the confi
-000027b0: 6775 7261 7469 6f6e 2061 6e64 2073 6574  guration and set
-000027c0: 2075 7020 6d6f 6e69 746f 7273 2066 6f72   up monitors for
-000027d0: 2074 7261 696e 696e 672e 0d0a 0d0a 2020   training.....  
-000027e0: 2020 2020 2020 5061 7261 6d65 7465 7273        Parameters
-000027f0: 0d0a 2020 2020 2020 2020 2d2d 2d2d 2d2d  ..        ------
-00002800: 2d2d 2d2d 0d0a 2020 2020 2020 2020 6366  ----..        cf
-00002810: 6720 3a20 436f 6e66 6967 0d0a 2020 2020  g : Config..    
-00002820: 2020 2020 2020 2020 4120 636f 6e66 6967          A config
-00002830: 7572 6174 696f 6e20 6f62 6a65 6374 2077  uration object w
-00002840: 6974 6820 7468 6520 7472 6169 6e69 6e67  ith the training
-00002850: 2064 6574 6169 6c73 2e0d 0a20 2020 2020   details...     
-00002860: 2020 206d 6f6e 6974 6f72 7320 3a20 4c69     monitors : Li
-00002870: 7374 5b73 7472 5d0d 0a20 2020 2020 2020  st[str]..       
-00002880: 2020 2020 2041 206c 6973 7420 6f66 206d       A list of m
-00002890: 6574 7269 6320 6e61 6d65 7320 746f 2062  etric names to b
-000028a0: 6520 6d6f 6e69 746f 7265 6420 6475 7269  e monitored duri
-000028b0: 6e67 2074 7261 696e 696e 672e 0d0a 2020  ng training...  
-000028c0: 2020 2020 2020 7768 6963 6834 6265 7374        which4best
-000028d0: 203a 2073 7472 2c20 6465 6661 756c 7473   : str, defaults
-000028e0: 2060 4c4f 5353 270d 0a20 2020 2020 2020   `LOSS'..       
-000028f0: 2020 2020 2054 6865 206d 6574 7269 6320       The metric 
-00002900: 7573 6564 2066 6f72 2073 656c 6563 7469  used for selecti
-00002910: 6e67 2074 6865 2062 6573 7420 6368 6563  ng the best chec
-00002920: 6b70 6f69 6e74 2e0d 0a0d 0a20 2020 2020  kpoint.....     
-00002930: 2020 2045 7861 6d70 6c65 730d 0a20 2020     Examples..   
-00002940: 2020 2020 202d 2d2d 2d2d 2d2d 2d0d 0a20       --------.. 
-00002950: 2020 2020 2020 203e 3e3e 2063 6f61 6368         >>> coach
-00002960: 3a20 436f 6163 680d 0a20 2020 2020 2020  : Coach..       
-00002970: 203e 3e3e 2063 6f61 6368 2e63 6f6d 7069   >>> coach.compi
-00002980: 6c65 2863 6667 2c20 6d6f 6e69 746f 7273  le(cfg, monitors
-00002990: 3d5b 276c 6f73 7327 2c20 2772 6563 616c  =['loss', 'recal
-000029a0: 6c40 3130 272c 2027 7265 6361 6c6c 4032  l@10', 'recall@2
-000029b0: 3027 2c20 276e 6463 6740 3130 272c 2027  0', 'ndcg@10', '
-000029c0: 6e64 6367 4032 3027 5d29 0d0a 2020 2020  ndcg@20'])..    
-000029d0: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
-000029e0: 2073 656c 662e 6366 6720 3d20 6366 670d   self.cfg = cfg.
-000029f0: 0a20 2020 2020 2020 2023 206d 6574 6572  .        # meter
-00002a00: 7320 666f 7220 7472 6169 6e7c 7661 6c69  s for train|vali
-00002a10: 647c 7465 7374 0d0a 2020 2020 2020 2020  d|test..        
-00002a20: 7365 6c66 2e5f 5f6d 6f6e 6974 6f72 7320  self.__monitors 
-00002a30: 3d20 4d6f 6e69 746f 7228 290d 0a20 2020  = Monitor()..   
-00002a40: 2020 2020 2073 656c 662e 5f5f 6d6f 6e69       self.__moni
-00002a50: 746f 7273 5b27 7472 6169 6e27 5d20 3d20  tors['train'] = 
-00002a60: 6465 6661 756c 7464 6963 7428 6c69 7374  defaultdict(list
-00002a70: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00002a80: 5f5f 6d6f 6e69 746f 7273 5b27 7661 6c69  __monitors['vali
-00002a90: 6427 5d20 3d20 6465 6661 756c 7464 6963  d'] = defaultdic
-00002aa0: 7428 6c69 7374 290d 0a20 2020 2020 2020  t(list)..       
-00002ab0: 2073 656c 662e 5f5f 6d6f 6e69 746f 7273   self.__monitors
-00002ac0: 5b27 7465 7374 275d 203d 2064 6566 6175  ['test'] = defau
-00002ad0: 6c74 6469 6374 286c 6973 7429 0d0a 0d0a  ltdict(list)....
-00002ae0: 2020 2020 2020 2020 6465 6620 7365 745f          def set_
-00002af0: 6d6f 6e69 746f 7228 0d0a 2020 2020 2020  monitor(..      
-00002b00: 2020 2020 2020 6e61 6d65 3a20 7374 722c        name: str,
-00002b10: 206c 6173 746e 616d 653a 2073 7472 2c20   lastname: str, 
-00002b20: 7072 6566 6978 3a20 7374 7220 3d20 2774  prefix: str = 't
-00002b30: 7261 696e 272c 202a 2a6b 7761 7267 730d  rain', **kwargs.
-00002b40: 0a20 2020 2020 2020 2029 3a0d 0a20 2020  .        ):..   
-00002b50: 2020 2020 2020 2020 2022 2222 4164 6420           """Add 
-00002b60: 6120 6d6f 6e69 746f 7220 666f 7220 7468  a monitor for th
-00002b70: 6520 7370 6563 6966 6965 6420 6d65 7472  e specified metr
-00002b80: 6963 2e22 2222 0d0a 2020 2020 2020 2020  ic."""..        
-00002b90: 2020 2020 7472 793a 0d0a 2020 2020 2020      try:..      
-00002ba0: 2020 2020 2020 2020 2020 6d65 7465 7220            meter 
-00002bb0: 3d20 4176 6572 6167 654d 6574 6572 280d  = AverageMeter(.
-00002bc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002bd0: 2020 2020 2020 2020 206e 616d 653d 6e61           name=na
-00002be0: 6d65 2c0d 0a20 2020 2020 2020 2020 2020  me,..           
-00002bf0: 2020 2020 2020 2020 2020 2020 206d 6574               met
-00002c00: 7269 633d 7061 7274 6961 6c28 4445 4641  ric=partial(DEFA
-00002c10: 554c 545f 4d45 5452 4943 535b 6c61 7374  ULT_METRICS[last
-00002c20: 6e61 6d65 5d2c 202a 2a6b 7761 7267 7329  name], **kwargs)
-00002c30: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00002c40: 2020 2020 2020 2020 2020 2066 6d74 3d44             fmt=D
-00002c50: 4546 4155 4c54 5f46 4d54 535b 6c61 7374  EFAULT_FMTS[last
-00002c60: 6e61 6d65 5d2c 0d0a 2020 2020 2020 2020  name],..        
-00002c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002c80: 6265 7374 5f63 6173 7465 723d 4445 4641  best_caster=DEFA
-00002c90: 554c 545f 4245 5354 5f43 4153 5445 525b  ULT_BEST_CASTER[
-00002ca0: 6c61 7374 6e61 6d65 5d0d 0a20 2020 2020  lastname]..     
-00002cb0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-00002cc0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00002cd0: 2020 7365 6c66 2e5f 5f6d 6f6e 6974 6f72    self.__monitor
-00002ce0: 735b 7072 6566 6978 5d5b 6c61 7374 6e61  s[prefix][lastna
-00002cf0: 6d65 5d2e 6170 7065 6e64 286d 6574 6572  me].append(meter
-00002d00: 290d 0a20 2020 2020 2020 2020 2020 2065  )..            e
-00002d10: 7863 6570 7420 4b65 7945 7272 6f72 3a0d  xcept KeyError:.
-00002d20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002d30: 2072 6169 7365 204b 6579 4572 726f 7228   raise KeyError(
-00002d40: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00002d50: 2020 2020 2020 6622 5468 6520 6d65 7472        f"The metr
-00002d60: 6963 206f 6620 7b6c 6173 746e 616d 657d  ic of {lastname}
-00002d70: 2069 7320 6e6f 7420 696e 636c 7564 6564   is not included
-00002d80: 2e20 220d 0a20 2020 2020 2020 2020 2020  . "..           
-00002d90: 2020 2020 2020 2020 2066 2259 6f75 2063           f"You c
-00002da0: 616e 2072 6567 6973 7465 7220 6279 2063  an register by c
-00002db0: 616c 6c69 6e67 2060 7265 6769 7374 6572  alling `register
-00002dc0: 5f6d 6574 7269 6328 2e2e 2e29 2720 2e2e  _metric(...)' ..
-00002dd0: 2e22 0d0a 2020 2020 2020 2020 2020 2020  ."..            
-00002de0: 2020 2020 290d 0a20 2020 2020 2020 2020      )..         
-00002df0: 2020 2072 6574 7572 6e20 6d65 7465 720d     return meter.
-00002e00: 0a0d 0a20 2020 2020 2020 2023 2055 5050  ...        # UPP
-00002e10: 4552 0d0a 2020 2020 2020 2020 7768 6963  ER..        whic
-00002e20: 6834 6265 7374 203d 2077 6869 6368 3462  h4best = which4b
-00002e30: 6573 742e 7570 7065 7228 290d 0a20 2020  est.upper()..   
-00002e40: 2020 2020 206d 6f6e 6974 6f72 7320 3d20       monitors = 
-00002e50: 5b27 4c4f 5353 275d 202b 205b 6e61 6d65  ['LOSS'] + [name
-00002e60: 2e75 7070 6572 2829 2066 6f72 206e 616d  .upper() for nam
-00002e70: 6520 696e 206d 6f6e 6974 6f72 735d 202b  e in monitors] +
-00002e80: 205b 7768 6963 6834 6265 7374 5d0d 0a20   [which4best].. 
-00002e90: 2020 2020 2020 206d 6f6e 6974 6f72 7320         monitors 
-00002ea0: 3d20 736f 7274 6564 2873 6574 286d 6f6e  = sorted(set(mon
-00002eb0: 6974 6f72 7329 2c20 6b65 793d 6d6f 6e69  itors), key=moni
-00002ec0: 746f 7273 2e69 6e64 6578 290d 0a0d 0a20  tors.index).... 
-00002ed0: 2020 2020 2020 2066 6f72 206e 616d 6520         for name 
-00002ee0: 696e 206d 6f6e 6974 6f72 733a 0d0a 2020  in monitors:..  
-00002ef0: 2020 2020 2020 2020 2020 666f 7220 7072            for pr
-00002f00: 6566 6978 2069 6e20 2827 7472 6169 6e27  efix in ('train'
-00002f10: 2c20 2776 616c 6964 272c 2027 7465 7374  , 'valid', 'test
-00002f20: 2729 3a0d 0a20 2020 2020 2020 2020 2020  '):..           
-00002f30: 2020 2020 2069 6620 2740 2720 696e 206e       if '@' in n
-00002f40: 616d 653a 0d0a 2020 2020 2020 2020 2020  ame:..          
-00002f50: 2020 2020 2020 2020 2020 6c61 7374 6e61            lastna
-00002f60: 6d65 2c20 4b20 3d20 6e61 6d65 2e73 706c  me, K = name.spl
-00002f70: 6974 2827 4027 290d 0a20 2020 2020 2020  it('@')..       
-00002f80: 2020 2020 2020 2020 2020 2020 206d 6574               met
-00002f90: 6572 203d 2073 6574 5f6d 6f6e 6974 6f72  er = set_monitor
-00002fa0: 280d 0a20 2020 2020 2020 2020 2020 2020  (..             
-00002fb0: 2020 2020 2020 2020 2020 206e 616d 653d             name=
-00002fc0: 6e61 6d65 2c0d 0a20 2020 2020 2020 2020  name,..         
-00002fd0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-00002fe0: 6173 746e 616d 653d 6c61 7374 6e61 6d65  astname=lastname
-00002ff0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00003000: 2020 2020 2020 2020 2020 2070 7265 6669             prefi
-00003010: 783d 7072 6566 6978 2c0d 0a20 2020 2020  x=prefix,..     
-00003020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003030: 2020 206b 3d69 6e74 284b 290d 0a20 2020     k=int(K)..   
-00003040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003050: 2029 0d0a 2020 2020 2020 2020 2020 2020   )..            
-00003060: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
-00003070: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-00003080: 6173 746e 616d 6520 3d20 6e61 6d65 0d0a  astname = name..
-00003090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000030a0: 2020 2020 6d65 7465 7220 3d20 7365 745f      meter = set_
-000030b0: 6d6f 6e69 746f 7228 0d0a 2020 2020 2020  monitor(..      
-000030c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000030d0: 2020 6e61 6d65 3d6e 616d 652c 0d0a 2020    name=name,..  
-000030e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000030f0: 2020 2020 2020 6c61 7374 6e61 6d65 3d6c        lastname=l
-00003100: 6173 746e 616d 652c 0d0a 2020 2020 2020  astname,..      
-00003110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003120: 2020 7072 6566 6978 3d70 7265 6669 780d    prefix=prefix.
-00003130: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003140: 2020 2020 2029 0d0a 2020 2020 2020 2020       )..        
-00003150: 2020 2020 2020 2020 6966 2070 7265 6669          if prefi
-00003160: 7820 3d3d 2027 7661 6c69 6427 2061 6e64  x == 'valid' and
-00003170: 206e 616d 6520 3d3d 2077 6869 6368 3462   name == which4b
-00003180: 6573 743a 0d0a 2020 2020 2020 2020 2020  est:..          
-00003190: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
-000031a0: 6574 6572 3462 6573 7420 3d20 6d65 7465  eter4best = mete
-000031b0: 720d 0a20 2020 2020 2020 2020 2020 2020  r..             
-000031c0: 2020 2020 2020 2073 656c 662e 5f62 6573         self._bes
-000031d0: 7420 3d20 2d66 6c6f 6174 2827 696e 6627  t = -float('inf'
-000031e0: 2920 6966 206d 6574 6572 2e63 6173 7465  ) if meter.caste
-000031f0: 7220 6973 206d 6178 2065 6c73 6520 666c  r is max else fl
-00003200: 6f61 7428 2769 6e66 2729 0d0a 2020 2020  oat('inf')..    
-00003210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003220: 7365 6c66 2e5f 6265 7374 5f65 706f 6368  self._best_epoch
-00003230: 203d 2030 0d0a 0d0a 2020 2020 2020 2020   = 0....        
-00003240: 2320 5072 6570 6172 6520 6461 7461 206c  # Prepare data l
-00003250: 6f61 6465 7273 0d0a 2020 2020 2020 2020  oaders..        
-00003260: 7365 6c66 2e70 7265 7061 7265 5f64 6174  self.prepare_dat
-00003270: 616c 6f61 6465 7228 290d 0a0d 0a20 2020  aloader()....   
-00003280: 2064 6566 2073 6176 6528 7365 6c66 2920   def save(self) 
-00003290: 2d3e 204e 6f6e 653a 0d0a 2020 2020 2020  -> None:..      
-000032a0: 2020 2222 2253 6176 6520 7468 6520 6d6f    """Save the mo
-000032b0: 6465 6c22 2222 0d0a 2020 2020 2020 2020  del"""..        
-000032c0: 746f 7263 682e 7361 7665 2873 656c 662e  torch.save(self.
-000032d0: 6d6f 6465 6c2e 7374 6174 655f 6469 6374  model.state_dict
-000032e0: 2829 2c20 6f73 2e70 6174 682e 6a6f 696e  (), os.path.join
-000032f0: 2873 656c 662e 6366 672e 4c4f 475f 5041  (self.cfg.LOG_PA
-00003300: 5448 2c20 7365 6c66 2e63 6667 2e53 4156  TH, self.cfg.SAV
-00003310: 4544 5f46 494c 454e 414d 4529 290d 0a0d  ED_FILENAME))...
-00003320: 0a20 2020 2064 6566 206c 6f61 6428 7365  .    def load(se
-00003330: 6c66 2c20 7061 7468 3a20 7374 722c 2066  lf, path: str, f
-00003340: 696c 656e 616d 653a 204f 7074 696f 6e61  ilename: Optiona
-00003350: 6c5b 7374 725d 203d 204e 6f6e 652c 202a  l[str] = None, *
-00003360: 2a6b 7761 7267 7329 202d 3e20 4e6f 6e65  *kwargs) -> None
-00003370: 3a0d 0a20 2020 2020 2020 2066 696c 656e  :..        filen
-00003380: 616d 6520 3d20 7365 6c66 2e63 6667 2e53  ame = self.cfg.S
-00003390: 4156 4544 5f46 494c 454e 414d 4520 6966  AVED_FILENAME if
-000033a0: 2066 696c 656e 616d 6520 6973 204e 6f6e   filename is Non
-000033b0: 6520 656c 7365 2066 696c 656e 616d 650d  e else filename.
-000033c0: 0a20 2020 2020 2020 2073 656c 662e 6d6f  .        self.mo
-000033d0: 6465 6c2e 6c6f 6164 5f73 7461 7465 5f64  del.load_state_d
-000033e0: 6963 7428 746f 7263 682e 6c6f 6164 286f  ict(torch.load(o
-000033f0: 732e 7061 7468 2e6a 6f69 6e28 7061 7468  s.path.join(path
-00003400: 2c20 6669 6c65 6e61 6d65 292c 202a 2a6b  , filename), **k
-00003410: 7761 7267 7329 290d 0a0d 0a20 2020 2064  wargs))....    d
-00003420: 6566 2073 6176 655f 6368 6563 6b70 6f69  ef save_checkpoi
-00003430: 6e74 2873 656c 662c 2065 706f 6368 3a20  nt(self, epoch: 
-00003440: 696e 7429 202d 3e20 4e6f 6e65 3a0d 0a20  int) -> None:.. 
-00003450: 2020 2020 2020 2072 2222 220d 0a20 2020         r"""..   
-00003460: 2020 2020 2053 6176 6520 6375 7272 656e       Save curren
-00003470: 7420 6368 6563 6b70 6f69 6e74 2061 7420  t checkpoint at 
-00003480: 6570 6f63 682e 0d0a 0d0a 2020 2020 2020  epoch.....      
-00003490: 2020 5061 7261 6d65 7465 7273 3a0d 0a20    Parameters:.. 
-000034a0: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
-000034b0: 2d2d 0d0a 2020 2020 2020 2020 2020 2020  --..            
-000034c0: 6570 6f63 6820 3a69 6e74 2043 7572 7265  epoch :int Curre
-000034d0: 6e74 2065 706f 6368 206e 756d 6265 722e  nt epoch number.
-000034e0: 0d0a 0d0a 2020 2020 2020 2020 5265 7475  ....        Retu
-000034f0: 726e 733a 0d0a 2020 2020 2020 2020 2d2d  rns:..        --
-00003500: 2d2d 2d2d 2d2d 0d0a 2020 2020 2020 2020  ------..        
-00003510: 2020 2020 4e6f 6e65 0d0a 2020 2020 2020      None..      
-00003520: 2020 2222 220d 0a20 2020 2020 2020 2070    """..        p
-00003530: 6174 6820 3d20 6f73 2e70 6174 682e 6a6f  ath = os.path.jo
-00003540: 696e 2873 656c 662e 6366 672e 4348 4543  in(self.cfg.CHEC
-00003550: 4b50 4f49 4e54 5f50 4154 482c 2073 656c  KPOINT_PATH, sel
-00003560: 662e 6366 672e 4348 4543 4b50 4f49 4e54  f.cfg.CHECKPOINT
-00003570: 5f46 494c 454e 414d 4529 0d0a 2020 2020  _FILENAME)..    
-00003580: 2020 2020 6368 6563 6b70 6f69 6e74 203d      checkpoint =
-00003590: 2064 6963 7428 290d 0a20 2020 2020 2020   dict()..       
-000035a0: 2063 6865 636b 706f 696e 745b 2765 706f   checkpoint['epo
-000035b0: 6368 275d 203d 2065 706f 6368 0d0a 2020  ch'] = epoch..  
-000035c0: 2020 2020 2020 666f 7220 6d6f 6475 6c65        for module
-000035d0: 2069 6e20 7365 6c66 2e63 6667 2e43 4845   in self.cfg.CHE
-000035e0: 434b 504f 494e 545f 4d4f 4455 4c45 533a  CKPOINT_MODULES:
-000035f0: 0d0a 2020 2020 2020 2020 2020 2020 6368  ..            ch
-00003600: 6563 6b70 6f69 6e74 5b6d 6f64 756c 655d  eckpoint[module]
-00003610: 203d 2067 6574 6174 7472 2873 656c 662c   = getattr(self,
-00003620: 206d 6f64 756c 6529 2e73 7461 7465 5f64   module).state_d
-00003630: 6963 7428 290d 0a20 2020 2020 2020 2063  ict()..        c
-00003640: 6865 636b 706f 696e 745b 276d 6f6e 6974  heckpoint['monit
-00003650: 6f72 7327 5d20 3d20 7365 6c66 2e6d 6f6e  ors'] = self.mon
-00003660: 6974 6f72 732e 7374 6174 655f 6469 6374  itors.state_dict
-00003670: 2829 0d0a 2020 2020 2020 2020 746f 7263  ()..        torc
-00003680: 682e 7361 7665 2863 6865 636b 706f 696e  h.save(checkpoin
-00003690: 742c 2070 6174 6829 0d0a 0d0a 2020 2020  t, path)....    
-000036a0: 6465 6620 6c6f 6164 5f63 6865 636b 706f  def load_checkpo
-000036b0: 696e 7428 7365 6c66 2920 2d3e 2069 6e74  int(self) -> int
-000036c0: 3a0d 0a20 2020 2020 2020 2072 2222 220d  :..        r""".
-000036d0: 0a20 2020 2020 2020 204c 6f61 6420 6c61  .        Load la
-000036e0: 7374 2073 6176 6564 2063 6865 636b 706f  st saved checkpo
-000036f0: 696e 742e 0d0a 0d0a 2020 2020 2020 2020  int.....        
-00003700: 5265 7475 726e 733a 0d0a 2020 2020 2020  Returns:..      
-00003710: 2020 2d2d 2d2d 2d2d 2d2d 0d0a 2020 2020    --------..    
-00003720: 2020 2020 6570 6f63 683a 2069 6e74 200d      epoch: int .
-00003730: 0a20 2020 2020 2020 2020 2020 2054 6865  .            The
-00003740: 2065 706f 6368 206e 756d 6265 7220 6c6f   epoch number lo
-00003750: 6164 6564 2066 726f 6d20 7468 6520 6368  aded from the ch
-00003760: 6563 6b70 6f69 6e74 2e0d 0a20 2020 2020  eckpoint...     
-00003770: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
-00003780: 7061 7468 203d 206f 732e 7061 7468 2e6a  path = os.path.j
-00003790: 6f69 6e28 7365 6c66 2e63 6667 2e43 4845  oin(self.cfg.CHE
-000037a0: 434b 504f 494e 545f 5041 5448 2c20 7365  CKPOINT_PATH, se
-000037b0: 6c66 2e63 6667 2e43 4845 434b 504f 494e  lf.cfg.CHECKPOIN
-000037c0: 545f 4649 4c45 4e41 4d45 290d 0a20 2020  T_FILENAME)..   
-000037d0: 2020 2020 2063 6865 636b 706f 696e 7420       checkpoint 
-000037e0: 3d20 746f 7263 682e 6c6f 6164 2870 6174  = torch.load(pat
-000037f0: 6829 0d0a 2020 2020 2020 2020 666f 7220  h)..        for 
-00003800: 6d6f 6475 6c65 2069 6e20 7365 6c66 2e63  module in self.c
-00003810: 6667 2e43 4845 434b 504f 494e 545f 4d4f  fg.CHECKPOINT_MO
-00003820: 4455 4c45 533a 0d0a 2020 2020 2020 2020  DULES:..        
-00003830: 2020 2020 6765 7461 7474 7228 7365 6c66      getattr(self
-00003840: 2c20 6d6f 6475 6c65 292e 6c6f 6164 5f73  , module).load_s
-00003850: 7461 7465 5f64 6963 7428 6368 6563 6b70  tate_dict(checkp
-00003860: 6f69 6e74 5b6d 6f64 756c 655d 290d 0a20  oint[module]).. 
-00003870: 2020 2020 2020 2073 656c 662e 6d6f 6e69         self.moni
-00003880: 746f 7273 2e6c 6f61 645f 7374 6174 655f  tors.load_state_
-00003890: 6469 6374 2863 6865 636b 706f 696e 745b  dict(checkpoint[
-000038a0: 276d 6f6e 6974 6f72 7327 5d29 0d0a 2020  'monitors'])..  
-000038b0: 2020 2020 2020 7265 7475 726e 2063 6865        return che
-000038c0: 636b 706f 696e 745b 2765 706f 6368 275d  ckpoint['epoch']
-000038d0: 0d0a 0d0a 2020 2020 6465 6620 7361 7665  ....    def save
-000038e0: 5f62 6573 7428 7365 6c66 2920 2d3e 204e  _best(self) -> N
-000038f0: 6f6e 653a 0d0a 2020 2020 2020 2020 746f  one:..        to
-00003900: 7263 682e 7361 7665 2873 656c 662e 6d6f  rch.save(self.mo
-00003910: 6465 6c2e 7374 6174 655f 6469 6374 2829  del.state_dict()
-00003920: 2c20 6f73 2e70 6174 682e 6a6f 696e 2873  , os.path.join(s
-00003930: 656c 662e 6366 672e 4c4f 475f 5041 5448  elf.cfg.LOG_PATH
-00003940: 2c20 7365 6c66 2e63 6667 2e42 4553 545f  , self.cfg.BEST_
-00003950: 4649 4c45 4e41 4d45 2929 0d0a 0d0a 2020  FILENAME))....  
-00003960: 2020 6465 6620 6c6f 6164 5f62 6573 7428    def load_best(
-00003970: 7365 6c66 2920 2d3e 204e 6f6e 653a 0d0a  self) -> None:..
-00003980: 2020 2020 2020 2020 696e 666f 4c6f 6767          infoLogg
-00003990: 6572 2866 225b 436f 6163 685d 203e 3e3e  er(f"[Coach] >>>
-000039a0: 204c 6f61 6420 6265 7374 206d 6f64 656c   Load best model
-000039b0: 2040 4570 6f63 6820 7b73 656c 662e 5f62   @Epoch {self._b
-000039c0: 6573 745f 6570 6f63 683a 3c34 647d 2022  est_epoch:<4d} "
-000039d0: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-000039e0: 6d6f 6465 6c2e 6c6f 6164 5f73 7461 7465  model.load_state
-000039f0: 5f64 6963 7428 746f 7263 682e 6c6f 6164  _dict(torch.load
-00003a00: 286f 732e 7061 7468 2e6a 6f69 6e28 7365  (os.path.join(se
-00003a10: 6c66 2e63 6667 2e4c 4f47 5f50 4154 482c  lf.cfg.LOG_PATH,
-00003a20: 2073 656c 662e 6366 672e 4245 5354 5f46   self.cfg.BEST_F
-00003a30: 494c 454e 414d 4529 2929 0d0a 0d0a 2020  ILENAME)))....  
-00003a40: 2020 6465 6620 6368 6563 6b5f 6265 7374    def check_best
-00003a50: 2873 656c 662c 2065 706f 6368 3a20 696e  (self, epoch: in
-00003a60: 7429 202d 3e20 4e6f 6e65 3a0d 0a20 2020  t) -> None:..   
-00003a70: 2020 2020 2022 2222 5570 6461 7465 2062       """Update b
-00003a80: 6573 7420 7661 6c75 652e 2222 220d 0a20  est value.""".. 
-00003a90: 2020 2020 2020 2069 6620 7365 6c66 2e6d         if self.m
-00003aa0: 6574 6572 3462 6573 742e 6163 7469 7665  eter4best.active
-00003ab0: 3a0d 0a20 2020 2020 2020 2020 2020 2062  :..            b
-00003ac0: 6573 745f 203d 2073 656c 662e 6d65 7465  est_ = self.mete
-00003ad0: 7234 6265 7374 2e77 6869 6368 5f69 735f  r4best.which_is_
-00003ae0: 6265 7474 6572 2873 656c 662e 5f62 6573  better(self._bes
-00003af0: 7429 0d0a 2020 2020 2020 2020 2020 2020  t)..            
-00003b00: 6966 2062 6573 745f 2021 3d20 7365 6c66  if best_ != self
-00003b10: 2e5f 6265 7374 3a0d 0a20 2020 2020 2020  ._best:..       
-00003b20: 2020 2020 2020 2020 2073 656c 662e 5f62           self._b
-00003b30: 6573 7420 3d20 6265 7374 5f0d 0a20 2020  est = best_..   
-00003b40: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00003b50: 662e 5f62 6573 745f 6570 6f63 6820 3d20  f._best_epoch = 
-00003b60: 6570 6f63 680d 0a20 2020 2020 2020 2020  epoch..         
-00003b70: 2020 2020 2020 2069 6e66 6f4c 6f67 6765         infoLogge
-00003b80: 7228 6622 5b43 6f61 6368 5d20 3e3e 3e20  r(f"[Coach] >>> 
-00003b90: 4265 7474 6572 202a 2a2a 7b73 656c 662e  Better ***{self.
-00003ba0: 6d65 7465 7234 6265 7374 2e6e 616d 657d  meter4best.name}
-00003bb0: 2a2a 2a20 6f66 202a 2a2a 7b73 656c 662e  *** of ***{self.
-00003bc0: 5f62 6573 743a 2e34 667d 2a2a 2a20 2229  _best:.4f}*** ")
-00003bd0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00003be0: 2020 7365 6c66 2e73 6176 655f 6265 7374    self.save_best
-00003bf0: 2829 0d0a 0d0a 2020 2020 6465 6620 6576  ()....    def ev
-00003c00: 616c 5f61 745f 6265 7374 2873 656c 6629  al_at_best(self)
-00003c10: 3a0d 0a20 2020 2020 2020 2074 7279 3a0d  :..        try:.
-00003c20: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00003c30: 662e 6c6f 6164 5f62 6573 7428 290d 0a20  f.load_best().. 
-00003c40: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00003c50: 7661 6c69 6428 7365 6c66 2e5f 6265 7374  valid(self._best
-00003c60: 5f65 706f 6368 290d 0a20 2020 2020 2020  _epoch)..       
-00003c70: 2020 2020 2073 656c 662e 7465 7374 2873       self.test(s
-00003c80: 656c 662e 5f62 6573 745f 6570 6f63 6829  elf._best_epoch)
-00003c90: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-00003ca0: 6c66 2e73 7465 7028 7365 6c66 2e5f 6265  lf.step(self._be
-00003cb0: 7374 5f65 706f 6368 290d 0a20 2020 2020  st_epoch)..     
-00003cc0: 2020 2020 2020 2073 656c 662e 6c6f 6164         self.load
-00003cd0: 2873 656c 662e 6366 672e 4c4f 475f 5041  (self.cfg.LOG_PA
-00003ce0: 5448 2c20 7365 6c66 2e63 6667 2e53 4156  TH, self.cfg.SAV
-00003cf0: 4544 5f46 494c 454e 414d 4529 0d0a 2020  ED_FILENAME)..  
-00003d00: 2020 2020 2020 6578 6365 7074 2046 696c        except Fil
-00003d10: 654e 6f74 466f 756e 6445 7272 6f72 3a0d  eNotFoundError:.
-00003d20: 0a20 2020 2020 2020 2020 2020 2069 6e66  .            inf
-00003d30: 6f4c 6f67 6765 7228 6622 5b43 6f61 6368  oLogger(f"[Coach
-00003d40: 5d20 3e3e 3e20 4e6f 2062 6573 7420 6d6f  ] >>> No best mo
-00003d50: 6465 6c20 7761 7320 7265 636f 7264 6564  del was recorded
-00003d60: 2e20 536b 6970 2069 7420 2e2e 2e22 290d  . Skip it ...").
-00003d70: 0a0d 0a20 2020 2064 6566 2072 6573 756d  ...    def resum
-00003d80: 6528 7365 6c66 2920 2d3e 2069 6e74 3a0d  e(self) -> int:.
-00003d90: 0a20 2020 2020 2020 2072 2222 220d 0a20  .        r""".. 
-00003da0: 2020 2020 2020 2052 6573 756d 6520 7472         Resume tr
-00003db0: 6169 6e69 6e67 2066 726f 6d20 7468 6520  aining from the 
-00003dc0: 6c61 7374 2063 6865 636b 706f 696e 742e  last checkpoint.
-00003dd0: 0d0a 0d0a 2020 2020 2020 2020 5265 7475  ....        Retu
-00003de0: 726e 733a 0d0a 2020 2020 2020 2020 2d2d  rns:..        --
-00003df0: 2d2d 2d2d 2d2d 0d0a 2020 2020 2020 2020  ------..        
-00003e00: 7374 6172 745f 6570 6f63 683a 2069 6e74  start_epoch: int
-00003e10: 0d0a 2020 2020 2020 2020 2020 2020 5468  ..            Th
-00003e20: 6520 6570 6f63 6820 6e75 6d62 6572 2074  e epoch number t
-00003e30: 6f20 7265 7375 6d65 2074 7261 696e 696e  o resume trainin
-00003e40: 6720 6672 6f6d 2e0d 0a20 2020 2020 2020  g from...       
-00003e50: 2022 2222 0d0a 2020 2020 2020 2020 7374   """..        st
-00003e60: 6172 745f 6570 6f63 683a 2069 6e74 203d  art_epoch: int =
-00003e70: 2030 0d0a 2020 2020 2020 2020 6966 2073   0..        if s
-00003e80: 656c 662e 6366 672e 7265 7375 6d65 3a0d  elf.cfg.resume:.
-00003e90: 0a20 2020 2020 2020 2020 2020 2073 7461  .            sta
-00003ea0: 7274 5f65 706f 6368 203d 2073 656c 662e  rt_epoch = self.
-00003eb0: 6c6f 6164 5f63 6865 636b 706f 696e 7428  load_checkpoint(
-00003ec0: 290d 0a20 2020 2020 2020 2020 2020 2069  )..            i
-00003ed0: 6e66 6f4c 6f67 6765 7228 6622 5b43 6f61  nfoLogger(f"[Coa
-00003ee0: 6368 5d20 3e3e 3e20 4c6f 6164 206c 6173  ch] >>> Load las
-00003ef0: 7420 6368 6563 6b70 6f69 6e74 2061 6e64  t checkpoint and
-00003f00: 2074 7261 696e 2066 726f 6d20 6570 6f63   train from epoc
-00003f10: 683a 207b 7374 6172 745f 6570 6f63 687d  h: {start_epoch}
-00003f20: 2229 0d0a 2020 2020 2020 2020 7265 7475  ")..        retu
-00003f30: 726e 2073 7461 7274 5f65 706f 6368 0d0a  rn start_epoch..
-00003f40: 0d0a 2020 2020 4074 6f72 6368 2e6e 6f5f  ..    @torch.no_
-00003f50: 6772 6164 2829 0d0a 2020 2020 6465 6620  grad()..    def 
-00003f60: 6d6f 6e69 746f 7228 0d0a 2020 2020 2020  monitor(..      
-00003f70: 2020 7365 6c66 2c20 2a76 616c 7565 732c    self, *values,
-00003f80: 0d0a 2020 2020 2020 2020 6e3a 2069 6e74  ..        n: int
-00003f90: 203d 2031 2c20 6d6f 6465 3a20 7374 7220   = 1, mode: str 
-00003fa0: 3d20 276d 6561 6e27 2c20 0d0a 2020 2020  = 'mean', ..    
-00003fb0: 2020 2020 7072 6566 6978 3a20 7374 7220      prefix: str 
-00003fc0: 3d20 2774 7261 696e 272c 2070 6f6f 6c3a  = 'train', pool:
-00003fd0: 204f 7074 696f 6e61 6c5b 4974 6572 6162   Optional[Iterab
-00003fe0: 6c65 5d20 3d20 4e6f 6e65 0d0a 2020 2020  le] = None..    
-00003ff0: 293a 0d0a 0d0a 2020 2020 2020 2020 7222  ):....        r"
-00004000: 2222 0d0a 2020 2020 2020 2020 4c6f 6720  ""..        Log 
-00004010: 6461 7461 2076 616c 7565 7320 746f 2073  data values to s
-00004020: 7065 6369 6669 6320 6d6f 6e69 746f 7273  pecific monitors
-00004030: 2e0d 0a0d 0a20 2020 2020 2020 2050 6172  .....        Par
-00004040: 616d 6574 6572 733a 0d0a 2020 2020 2020  ameters:..      
-00004050: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d0d 0a20    -----------.. 
-00004060: 2020 2020 2020 202a 7661 6c75 6573 203a         *values :
-00004070: 2064 6174 610d 0a20 2020 2020 2020 2020   data..         
-00004080: 2020 2054 6865 2064 6174 6120 7661 6c75     The data valu
-00004090: 6573 2074 6f20 6265 206c 6f67 6765 642e  es to be logged.
-000040a0: 0d0a 2020 2020 2020 2020 6e20 3a20 696e  ..        n : in
-000040b0: 740d 0a20 2020 2020 2020 2020 2020 2054  t..            T
-000040c0: 6865 2062 6174 6368 2073 697a 6520 696e  he batch size in
-000040d0: 2067 656e 6572 616c 2e0d 0a20 2020 2020   general...     
-000040e0: 2020 206d 6f64 6520 3a20 7374 722c 206f     mode : str, o
-000040f0: 7074 696f 6e61 6c0d 0a20 2020 2020 2020  ptional..       
-00004100: 2020 2020 2054 6865 206d 6f64 6520 746f       The mode to
-00004110: 2063 6f6d 7075 7465 2074 6865 206d 6574   compute the met
-00004120: 7269 632e 2043 616e 2062 6520 2773 756d  ric. Can be 'sum
-00004130: 2720 6f72 2027 6d65 616e 2720 2864 6566  ' or 'mean' (def
-00004140: 6175 6c74 292e 0d0a 2020 2020 2020 2020  ault)...        
-00004150: 7072 6566 6978 203a 2073 7472 2c20 6f70  prefix : str, op
-00004160: 7469 6f6e 616c 0d0a 2020 2020 2020 2020  tional..        
-00004170: 2020 2020 5468 6520 7072 6566 6978 2073      The prefix s
-00004180: 7472 696e 6720 696e 6469 6361 7469 6e67  tring indicating
-00004190: 2077 6869 6368 206d 6f64 6520 7468 6520   which mode the 
-000041a0: 7661 6c75 6573 2062 656c 6f6e 6720 746f  values belong to
-000041b0: 2e20 4361 6e20 6265 2027 7472 6169 6e27  . Can be 'train'
-000041c0: 2c20 2774 6573 7427 206f 7220 2776 616c  , 'test' or 'val
-000041d0: 6964 272e 0d0a 2020 2020 2020 2020 706f  id'...        po
-000041e0: 6f6c 203a 204c 6973 745b 7374 725d 2c20  ol : List[str], 
-000041f0: 6f70 7469 6f6e 616c 0d0a 2020 2020 2020  optional..      
-00004200: 2020 2020 2020 4120 6c69 7374 206f 6620        A list of 
-00004210: 6d65 7472 6963 206e 616d 6573 2074 6f20  metric names to 
-00004220: 6c6f 672e 2049 6620 4e6f 6e65 2c20 616c  log. If None, al
-00004230: 6c20 6d65 7472 6963 7320 696e 2074 6865  l metrics in the
-00004240: 2070 6f6f 6c20 6f66 2060 7072 6566 6978   pool of `prefix
-00004250: 6020 7769 6c6c 2062 6520 6c6f 6767 6564  ` will be logged
-00004260: 2e0d 0a20 2020 2020 2020 2022 2222 0d0a  ...        """..
-00004270: 0d0a 2020 2020 2020 2020 6d65 7472 6963  ..        metric
-00004280: 733a 2044 6963 745b 4c69 7374 5d20 3d20  s: Dict[List] = 
-00004290: 7365 6c66 2e6d 6f6e 6974 6f72 735b 7072  self.monitors[pr
-000042a0: 6566 6978 5d0d 0a20 2020 2020 2020 2070  efix]..        p
-000042b0: 6f6f 6c20 3d20 6d65 7472 6963 7320 6966  ool = metrics if
-000042c0: 2070 6f6f 6c20 6973 204e 6f6e 6520 656c   pool is None el
-000042d0: 7365 2070 6f6f 6c0d 0a20 2020 2020 2020  se pool..       
-000042e0: 2066 6f72 206c 6173 746e 616d 6520 696e   for lastname in
-000042f0: 2070 6f6f 6c3a 0d0a 2020 2020 2020 2020   pool:..        
-00004300: 2020 2020 666f 7220 6d65 7465 7220 696e      for meter in
-00004310: 206d 6574 7269 6373 2e67 6574 286c 6173   metrics.get(las
-00004320: 746e 616d 652e 7570 7065 7228 292c 205b  tname.upper(), [
-00004330: 5d29 3a0d 0a20 2020 2020 2020 2020 2020  ]):..           
-00004340: 2020 2020 206d 6574 6572 282a 7661 6c75       meter(*valu
-00004350: 6573 2c20 6e3d 6e2c 206d 6f64 653d 6d6f  es, n=n, mode=mo
-00004360: 6465 290d 0a0d 0a20 2020 2064 6566 2073  de)....    def s
-00004370: 7465 7028 7365 6c66 2c20 6570 6f63 683a  tep(self, epoch:
-00004380: 2069 6e74 293a 0d0a 2020 2020 2020 2020   int):..        
-00004390: 7222 2222 0d0a 2020 2020 2020 2020 5072  r"""..        Pr
-000043a0: 696e 7473 2074 7261 696e 696e 6720 7374  ints training st
-000043b0: 6174 7573 2061 6e64 2065 7661 6c75 6174  atus and evaluat
-000043c0: 696f 6e20 7265 7375 6c74 7320 666f 7220  ion results for 
-000043d0: 6561 6368 2065 706f 6368 2c20 0d0a 2020  each epoch, ..  
-000043e0: 2020 2020 2020 616e 6420 7265 7365 7473        and resets
-000043f0: 2074 6865 2063 6f72 7265 7370 6f6e 6469   the correspondi
-00004400: 6e67 2060 4176 6572 6167 654d 6574 6572  ng `AverageMeter
-00004410: 6020 696e 7374 616e 6365 732e 0d0a 0d0a  ` instances.....
-00004420: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
-00004430: 7273 3a0d 0a20 2020 2020 2020 202d 2d2d  rs:..        ---
-00004440: 2d2d 2d2d 2d2d 2d2d 0d0a 2020 2020 2020  --------..      
-00004450: 2020 6570 6f63 6820 3a20 696e 740d 0a20    epoch : int.. 
-00004460: 2020 2020 2020 2020 2020 2054 6865 2065             The e
-00004470: 706f 6368 206e 756d 6265 722e 0d0a 0d0a  poch number.....
-00004480: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
-00004490: 0d0a 2020 2020 2020 2020 2d2d 2d2d 2d2d  ..        ------
-000044a0: 2d2d 0d0a 2020 2020 2020 2020 4e6f 6e65  --..        None
-000044b0: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
-000044c0: 2020 2020 2020 206d 6574 7269 6373 3a20         metrics: 
-000044d0: 4469 6374 5b73 7472 2c20 4c69 7374 5b41  Dict[str, List[A
-000044e0: 7665 7261 6765 4d65 7465 725d 5d0d 0a20  verageMeter]].. 
-000044f0: 2020 2020 2020 2066 6f72 2070 7265 6669         for prefi
-00004500: 782c 206d 6574 7269 6373 2069 6e20 7365  x, metrics in se
-00004510: 6c66 2e6d 6f6e 6974 6f72 732e 6974 656d  lf.monitors.item
-00004520: 7328 293a 0d0a 2020 2020 2020 2020 2020  s():..          
-00004530: 2020 696e 666f 7320 3d20 5b66 225b 436f    infos = [f"[Co
-00004540: 6163 685d 203e 3e3e 207b 7072 6566 6978  ach] >>> {prefix
-00004550: 2e75 7070 6572 2829 3a35 7d20 4045 706f  .upper():5} @Epo
-00004560: 6368 3a20 7b65 706f 6368 3a3c 3464 7d20  ch: {epoch:<4d} 
-00004570: 3e3e 3e20 225d 0d0a 2020 2020 2020 2020  >>> "]..        
-00004580: 2020 2020 666f 7220 6d65 7465 7273 2069      for meters i
-00004590: 6e20 6d65 7472 6963 732e 7661 6c75 6573  n metrics.values
-000045a0: 2829 3a0d 0a20 2020 2020 2020 2020 2020  ():..           
-000045b0: 2020 2020 2069 6e66 6f73 202b 3d20 5b6d       infos += [m
-000045c0: 6574 6572 2e73 7465 7028 2920 666f 7220  eter.step() for 
-000045d0: 6d65 7465 7220 696e 206d 6574 6572 7320  meter in meters 
-000045e0: 6966 206d 6574 6572 2e61 6374 6976 655d  if meter.active]
-000045f0: 0d0a 2020 2020 2020 2020 2020 2020 696e  ..            in
-00004600: 666f 4c6f 6767 6572 2827 207c 7c20 272e  foLogger(' || '.
-00004610: 6a6f 696e 2869 6e66 6f73 2929 0d0a 0d0a  join(infos))....
-00004620: 2020 2020 4074 696d 656d 6574 6572 2822      @timemeter("
-00004630: 436f 6163 682f 7375 6d6d 6172 7922 290d  Coach/summary").
-00004640: 0a20 2020 2064 6566 2073 756d 6d61 7279  .    def summary
-00004650: 2873 656c 6629 3a0d 0a20 2020 2020 2020  (self):..       
-00004660: 2072 2222 220d 0a20 2020 2020 2020 2053   r"""..        S
-00004670: 756d 6d61 7279 2074 6865 2077 686f 6c65  ummary the whole
-00004680: 2074 7261 696e 696e 6720 7072 6f63 6573   training proces
-00004690: 732e 0d0a 0d0a 2020 2020 2020 2020 4765  s.....        Ge
-000046a0: 6e65 7261 7465 2061 2073 756d 6d61 7279  nerate a summary
-000046b0: 206f 6620 7468 6520 656e 7469 7265 2074   of the entire t
-000046c0: 7261 696e 696e 6720 7072 6f63 6573 732c  raining process,
-000046d0: 2069 6e63 6c75 6469 6e67 2074 6865 2068   including the h
-000046e0: 6973 746f 7269 6361 6c20 6576 616c 7561  istorical evalua
-000046f0: 7469 6f6e 2072 6573 756c 7473 2c20 7468  tion results, th
-00004700: 6520 6265 7374 0d0a 2020 2020 2020 2020  e best..        
-00004710: 6869 7374 6f72 6963 616c 2072 6573 756c  historical resul
-00004720: 7473 2c20 616e 6420 7468 6520 6375 7276  ts, and the curv
-00004730: 6573 206f 6620 6869 7374 6f72 6963 616c  es of historical
-00004740: 2072 6573 756c 7473 2e20 5468 6520 7265   results. The re
-00004750: 7375 6c74 696e 6720 7375 6d6d 6172 7920  sulting summary 
-00004760: 6973 2073 6176 6564 2074 6f20 6120 4d61  is saved to a Ma
-00004770: 726b 646f 776e 2066 696c 6520 6e61 6d65  rkdown file name
-00004780: 640d 0a20 2020 2020 2020 2022 5375 6d6d  d..        "Summ
-00004790: 6172 792e 6d64 2220 696e 2074 6865 2060  ary.md" in the `
-000047a0: 7365 6c66 2e63 6667 2e4c 4f47 5f50 4154  self.cfg.LOG_PAT
-000047b0: 4860 2064 6972 6563 746f 7279 2e0d 0a0d  H` directory....
-000047c0: 0a20 2020 2020 2020 2041 6464 6974 696f  .        Additio
-000047d0: 6e61 6c6c 792c 2074 6865 2062 6573 7420  nally, the best 
-000047e0: 6869 7374 6f72 6963 616c 2072 6573 756c  historical resul
-000047f0: 7473 2061 7265 2073 6176 6564 2074 6f20  ts are saved to 
-00004800: 6120 6269 6e61 7279 2066 696c 6520 6e61  a binary file na
-00004810: 6d65 6420 6073 656c 662e 6366 672e 4d4f  med `self.cfg.MO
-00004820: 4e49 544f 525f 4245 5354 5f46 494c 454e  NITOR_BEST_FILEN
-00004830: 414d 4560 2e0d 0a20 2020 2020 2020 2022  AME`...        "
-00004840: 2222 0d0a 2020 2020 2020 2020 7320 3d20  ""..        s = 
-00004850: 227c 2020 7b70 7265 6669 787d 2020 7c20  "|  {prefix}  | 
-00004860: 2020 7b6e 616d 657d 2020 207c 2020 207b    {name}   |   {
-00004870: 7661 6c7d 2020 207c 2020 207b 6570 6f63  val}   |   {epoc
-00004880: 687d 2020 207c 2020 207b 696d 677d 2020  h}   |   {img}  
-00004890: 207c 5c6e 220d 0a20 2020 2020 2020 2069   |\n"..        i
-000048a0: 6e66 6f20 3d20 2222 0d0a 2020 2020 2020  nfo = ""..      
-000048b0: 2020 696e 666f 202b 3d20 227c 2020 5072    info += "|  Pr
-000048c0: 6566 6978 2020 7c20 2020 4d65 7472 6963  efix  |   Metric
-000048d0: 2020 207c 2020 2042 6573 7420 2020 7c20     |   Best   | 
-000048e0: 2020 4045 706f 6368 2020 207c 2020 2049    @Epoch   |   I
-000048f0: 6d67 2020 207c 5c6e 220d 0a20 2020 2020  mg   |\n"..     
-00004900: 2020 2069 6e66 6f20 2b3d 2022 7c20 3a2d     info += "| :-
-00004910: 2d2d 2d2d 2d2d 3a20 7c20 3a2d 2d2d 2d2d  ------: | :-----
-00004920: 2d2d 3a20 7c20 3a2d 2d2d 2d2d 2d2d 3a20  --: | :-------: 
-00004930: 7c20 3a2d 2d2d 2d2d 2d2d 3a20 7c20 3a2d  | :-------: | :-
-00004940: 2d2d 2d2d 2d2d 3a20 7c5c 6e22 0d0a 2020  ------: |\n"..  
-00004950: 2020 2020 2020 6461 7461 203d 205b 5d0d        data = [].
-00004960: 0a20 2020 2020 2020 2062 6573 7420 3d20  .        best = 
-00004970: 6465 6661 756c 7464 6963 7428 6469 6374  defaultdict(dict
-00004980: 290d 0a0d 0a20 2020 2020 2020 2066 6f72  )....        for
-00004990: 2070 7265 6669 782c 206d 6574 7269 6373   prefix, metrics
-000049a0: 2069 6e20 7365 6c66 2e6d 6f6e 6974 6f72   in self.monitor
-000049b0: 732e 6974 656d 7328 293a 0d0a 2020 2020  s.items():..    
-000049c0: 2020 2020 2020 2020 6d65 7472 6963 733a          metrics:
-000049d0: 2064 6566 6175 6c74 6469 6374 5b73 7472   defaultdict[str
-000049e0: 2c20 4c69 7374 5b41 7665 7261 6765 4d65  , List[AverageMe
-000049f0: 7465 725d 5d0d 0a20 2020 2020 2020 2020  ter]]..         
-00004a00: 2020 2066 7265 7120 3d20 3120 6966 2070     freq = 1 if p
-00004a10: 7265 6669 7820 3d3d 2027 7472 6169 6e27  refix == 'train'
-00004a20: 2065 6c73 6520 7365 6c66 2e63 6667 2e45   else self.cfg.E
-00004a30: 5641 4c5f 4652 4551 0d0a 2020 2020 2020  VAL_FREQ..      
-00004a40: 2020 2020 2020 666f 7220 6c61 7374 6e61        for lastna
-00004a50: 6d65 2c20 6d65 7465 7273 2069 6e20 6d65  me, meters in me
-00004a60: 7472 6963 732e 6974 656d 7328 293a 0d0a  trics.items():..
-00004a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004a80: 666f 7220 6d65 7465 7220 696e 206d 6574  for meter in met
-00004a90: 6572 733a 0d0a 2020 2020 2020 2020 2020  ers:..          
-00004aa0: 2020 2020 2020 2020 2020 2320 536b 6970            # Skip
-00004ab0: 2074 686f 7365 206d 6574 6572 7320 6e65   those meters ne
-00004ac0: 7665 7220 6163 7469 7661 7465 642e 0d0a  ver activated...
-00004ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004ae0: 2020 2020 6966 206c 656e 286d 6574 6572      if len(meter
-00004af0: 2e68 6973 746f 7279 2920 3d3d 2030 3a0d  .history) == 0:.
-00004b00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004b10: 2020 2020 2020 2020 2063 6f6e 7469 6e75           continu
-00004b20: 650d 0a20 2020 2020 2020 2020 2020 2020  e..             
-00004b30: 2020 2020 2020 206d 6574 6572 2e70 6c6f         meter.plo
-00004b40: 7428 6672 6571 3d66 7265 7129 0d0a 2020  t(freq=freq)..  
-00004b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004b60: 2020 696d 676e 616d 6520 3d20 6d65 7465    imgname = mete
-00004b70: 722e 7361 7665 2870 6174 683d 6f73 2e70  r.save(path=os.p
-00004b80: 6174 682e 6a6f 696e 2873 656c 662e 6366  ath.join(self.cf
-00004b90: 672e 4c4f 475f 5041 5448 2c20 7365 6c66  g.LOG_PATH, self
-00004ba0: 2e63 6667 2e53 554d 4d41 5259 5f44 4952  .cfg.SUMMARY_DIR
-00004bb0: 292c 2070 7265 6669 783d 7072 6566 6978  ), prefix=prefix
-00004bc0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00004bd0: 2020 2020 2020 2065 706f 6368 2c20 7661         epoch, va
-00004be0: 6c20 3d20 6d65 7465 722e 6172 6762 6573  l = meter.argbes
-00004bf0: 7428 6672 6571 290d 0a20 2020 2020 2020  t(freq)..       
-00004c00: 2020 2020 2020 2020 2020 2020 2069 6e66               inf
-00004c10: 6f20 2b3d 2073 2e66 6f72 6d61 7428 0d0a  o += s.format(..
-00004c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004c30: 2020 2020 2020 2020 7072 6566 6978 3d70          prefix=p
-00004c40: 7265 6669 782c 206e 616d 653d 6d65 7465  refix, name=mete
-00004c50: 722e 6e61 6d65 2c0d 0a20 2020 2020 2020  r.name,..       
+00001200: 7472 793a 0d0a 2020 2020 2020 2020 2020  try:..          
+00001210: 2020 746f 7263 682e 6375 6461 2e73 6574    torch.cuda.set
+00001220: 5f64 6576 6963 6528 7365 6c66 2e64 6576  _device(self.dev
+00001230: 6963 6529 0d0a 2020 2020 2020 2020 6578  ice)..        ex
+00001240: 6365 7074 2056 616c 7565 4572 726f 723a  cept ValueError:
+00001250: 0d0a 2020 2020 2020 2020 2020 2020 7061  ..            pa
+00001260: 7373 0d0a 0d0a 2020 2020 2020 2020 7365  ss....        se
+00001270: 6c66 2e5f 7365 745f 6461 7461 7069 7065  lf._set_datapipe
+00001280: 2874 7261 696e 7069 7065 2c20 7661 6c69  (trainpipe, vali
+00001290: 6470 6970 652c 2074 6573 7470 6970 6529  dpipe, testpipe)
+000012a0: 0d0a 2020 2020 2020 2020 7365 6c66 2e5f  ..        self._
+000012b0: 7365 745f 6f74 6865 7228 6d6f 6465 6c2c  set_other(model,
+000012c0: 2063 7269 7465 7269 6f6e 2c20 6f70 7469   criterion, opti
+000012d0: 6d69 7a65 722c 206c 725f 7363 6865 6475  mizer, lr_schedu
+000012e0: 6c65 7229 0d0a 0d0a 2020 2020 2020 2020  ler)....        
+000012f0: 7365 6c66 2e5f 5f6d 6f64 6520 3d20 2774  self.__mode = 't
+00001300: 7261 696e 270d 0a0d 0a20 2020 2020 2020  rain'....       
+00001310: 2064 6566 2063 6c65 616e 2829 3a0d 0a20   def clean():.. 
+00001320: 2020 2020 2020 2020 2020 2070 6172 656e             paren
+00001330: 7420 3d20 7073 7574 696c 2e50 726f 6365  t = psutil.Proce
+00001340: 7373 286f 732e 6765 7470 6964 2829 290d  ss(os.getpid()).
+00001350: 0a20 2020 2020 2020 2020 2020 2063 6869  .            chi
+00001360: 6c64 7265 6e20 3d20 7061 7265 6e74 2e63  ldren = parent.c
+00001370: 6869 6c64 7265 6e28 7265 6375 7273 6976  hildren(recursiv
+00001380: 653d 5472 7565 290d 0a20 2020 2020 2020  e=True)..       
+00001390: 2020 2020 2066 6f72 2070 726f 6365 7373       for process
+000013a0: 2069 6e20 6368 696c 6472 656e 3a0d 0a20   in children:.. 
+000013b0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+000013c0: 726f 6365 7373 2e73 656e 645f 7369 676e  rocess.send_sign
+000013d0: 616c 2873 6967 6e61 6c2e 5349 4754 4552  al(signal.SIGTER
+000013e0: 4d29 0d0a 2020 2020 2020 2020 2020 2020  M)..            
+000013f0: 7073 7574 696c 2e77 6169 745f 7072 6f63  psutil.wait_proc
+00001400: 7328 6368 696c 6472 656e 2c20 7469 6d65  s(children, time
+00001410: 6f75 743d 3529 0d0a 0d0a 2020 2020 2020  out=5)....      
+00001420: 2020 6174 6578 6974 2e72 6567 6973 7465    atexit.registe
+00001430: 7228 636c 6561 6e29 0d0a 0d0a 2020 2020  r(clean)....    
+00001440: 6465 6620 5f73 6574 5f64 6174 6170 6970  def _set_datapip
+00001450: 6528 0d0a 2020 2020 2020 2020 7365 6c66  e(..        self
+00001460: 2c0d 0a20 2020 2020 2020 2074 7261 696e  ,..        train
+00001470: 7069 7065 2c0d 0a20 2020 2020 2020 2076  pipe,..        v
+00001480: 616c 6964 7069 7065 3d4e 6f6e 652c 0d0a  alidpipe=None,..
+00001490: 2020 2020 2020 2020 7465 7374 7069 7065          testpipe
+000014a0: 3d4e 6f6e 652c 0d0a 2020 2020 293a 0d0a  =None,..    ):..
+000014b0: 2020 2020 2020 2020 2222 2253 6574 2074          """Set t
+000014c0: 6865 2064 6174 6120 7069 7065 2066 6f72  he data pipe for
+000014d0: 2074 7261 696e 696e 672c 2076 616c 6964   training, valid
+000014e0: 6174 696f 6e20 616e 6420 7465 7374 2e22  ation and test."
+000014f0: 2222 0d0a 2020 2020 2020 2020 7365 6c66  ""..        self
+00001500: 2e74 7261 696e 7069 7065 203d 2074 7261  .trainpipe = tra
+00001510: 696e 7069 7065 0d0a 2020 2020 2020 2020  inpipe..        
+00001520: 7365 6c66 2e76 616c 6964 7069 7065 203d  self.validpipe =
+00001530: 2073 656c 662e 7472 6169 6e70 6970 6520   self.trainpipe 
+00001540: 6966 2076 616c 6964 7069 7065 2069 7320  if validpipe is 
+00001550: 4e6f 6e65 2065 6c73 6520 7661 6c69 6470  None else validp
+00001560: 6970 650d 0a20 2020 2020 2020 2073 656c  ipe..        sel
+00001570: 662e 7465 7374 7069 7065 203d 2073 656c  f.testpipe = sel
+00001580: 662e 7661 6c69 6470 6970 6520 6966 2074  f.validpipe if t
+00001590: 6573 7470 6970 6520 6973 204e 6f6e 6520  estpipe is None 
+000015a0: 656c 7365 2074 6573 7470 6970 650d 0a0d  else testpipe...
+000015b0: 0a20 2020 2064 6566 205f 7365 745f 6f74  .    def _set_ot
+000015c0: 6865 7228 0d0a 2020 2020 2020 2020 7365  her(..        se
+000015d0: 6c66 2c0d 0a20 2020 2020 2020 206d 6f64  lf,..        mod
+000015e0: 656c 3d4e 6f6e 652c 2063 7269 7465 7269  el=None, criteri
+000015f0: 6f6e 3d4e 6f6e 652c 206f 7074 696d 697a  on=None, optimiz
+00001600: 6572 3d4e 6f6e 652c 206c 725f 7363 6865  er=None, lr_sche
+00001610: 6475 6c65 723d 4e6f 6e65 2c0d 0a20 2020  duler=None,..   
+00001620: 2029 3a0d 0a20 2020 2020 2020 2022 2222   ):..        """
+00001630: 5365 7420 7468 6520 6f74 6865 7220 6e65  Set the other ne
+00001640: 6365 7373 6172 7920 636f 6d70 6f6e 656e  cessary componen
+00001650: 7473 2e22 2222 0d0a 2020 2020 2020 2020  ts."""..        
+00001660: 7365 6c66 2e63 7269 7465 7269 6f6e 203d  self.criterion =
+00001670: 2063 7269 7465 7269 6f6e 0d0a 2020 2020   criterion..    
+00001680: 2020 2020 7365 6c66 2e6d 6f64 656c 203d      self.model =
+00001690: 206d 6f64 656c 2e74 6f28 7365 6c66 2e64   model.to(self.d
+000016a0: 6576 6963 6529 2069 6620 6d6f 6465 6c20  evice) if model 
+000016b0: 656c 7365 205f 4475 6d6d 794d 6f64 756c  else _DummyModul
+000016c0: 6528 290d 0a20 2020 2020 2020 2073 656c  e()..        sel
+000016d0: 662e 6f70 7469 6d69 7a65 7220 3d20 6f70  f.optimizer = op
+000016e0: 7469 6d69 7a65 7220 6966 206f 7074 696d  timizer if optim
+000016f0: 697a 6572 2065 6c73 6520 5f44 756d 6d79  izer else _Dummy
+00001700: 4d6f 6475 6c65 2829 0d0a 2020 2020 2020  Module()..      
+00001710: 2020 7365 6c66 2e6c 725f 7363 6865 6475    self.lr_schedu
+00001720: 6c65 7220 3d20 6c72 5f73 6368 6564 756c  ler = lr_schedul
+00001730: 6572 2069 6620 6c72 5f73 6368 6564 756c  er if lr_schedul
+00001740: 6572 2065 6c73 6520 5f44 756d 6d79 4d6f  er else _DummyMo
+00001750: 6475 6c65 2829 0d0a 0d0a 2020 2020 4070  dule()....    @p
+00001760: 726f 7065 7274 790d 0a20 2020 2064 6566  roperty..    def
+00001770: 206d 6f64 6528 7365 6c66 293a 0d0a 2020   mode(self):..  
+00001780: 2020 2020 2020 2222 2247 6574 2074 6865        """Get the
+00001790: 2063 7572 7265 6e74 206d 6f64 6520 6f66   current mode of
+000017a0: 2074 6865 2063 6869 6566 2063 6f61 6368   the chief coach
+000017b0: 2e22 2222 0d0a 2020 2020 2020 2020 7265  ."""..        re
+000017c0: 7475 726e 2073 656c 662e 5f5f 6d6f 6465  turn self.__mode
+000017d0: 0d0a 0d0a 2020 2020 4074 696d 656d 6574  ....    @timemet
+000017e0: 6572 2822 436f 6163 682f 7472 6169 6e22  er("Coach/train"
+000017f0: 290d 0a20 2020 2064 6566 2074 7261 696e  )..    def train
+00001800: 2873 656c 662c 2065 706f 6368 3a20 696e  (self, epoch: in
+00001810: 7429 3a0d 0a20 2020 2020 2020 2022 2222  t):..        """
+00001820: 5374 6172 7420 7472 6169 6e69 6e67 2061  Start training a
+00001830: 6e64 2072 6574 7572 6e20 7468 6520 7472  nd return the tr
+00001840: 6169 6e69 6e67 206c 6f73 732e 2222 220d  aining loss.""".
+00001850: 0a20 2020 2020 2020 2073 656c 662e 5f5f  .        self.__
+00001860: 6d6f 6465 203d 2027 7472 6169 6e27 0d0a  mode = 'train'..
+00001870: 2020 2020 2020 2020 7365 6c66 2e6d 6f64          self.mod
+00001880: 656c 2e74 7261 696e 2829 0d0a 2020 2020  el.train()..    
+00001890: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+000018a0: 7472 6169 6e5f 7065 725f 6570 6f63 6828  train_per_epoch(
+000018b0: 6570 6f63 6829 0d0a 0d0a 2020 2020 4074  epoch)....    @t
+000018c0: 696d 656d 6574 6572 2822 436f 6163 682f  imemeter("Coach/
+000018d0: 7661 6c69 6422 290d 0a20 2020 2040 746f  valid")..    @to
+000018e0: 7263 682e 6e6f 5f67 7261 6428 290d 0a20  rch.no_grad().. 
+000018f0: 2020 2064 6566 2076 616c 6964 2873 656c     def valid(sel
+00001900: 662c 2065 706f 6368 3a20 696e 7429 3a0d  f, epoch: int):.
+00001910: 0a20 2020 2020 2020 2022 2222 5374 6172  .        """Star
+00001920: 7420 7661 6c69 6461 7469 6f6e 2061 6e64  t validation and
+00001930: 2072 6574 7572 6e20 7468 6520 7661 6c69   return the vali
+00001940: 6461 7469 6f6e 206d 6574 7269 6373 2e22  dation metrics."
+00001950: 2222 0d0a 2020 2020 2020 2020 7365 6c66  ""..        self
+00001960: 2e5f 5f6d 6f64 6520 3d20 2776 616c 6964  .__mode = 'valid
+00001970: 270d 0a20 2020 2020 2020 2073 656c 662e  '..        self.
+00001980: 6d6f 6465 6c2e 6576 616c 2829 0d0a 2020  model.eval()..  
+00001990: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+000019a0: 662e 6576 616c 7561 7465 2865 706f 6368  f.evaluate(epoch
+000019b0: 3d65 706f 6368 2c20 7072 6566 6978 3d27  =epoch, prefix='
+000019c0: 7661 6c69 6427 290d 0a0d 0a20 2020 2040  valid')....    @
+000019d0: 7469 6d65 6d65 7465 7228 2243 6f61 6368  timemeter("Coach
+000019e0: 2f74 6573 7422 290d 0a20 2020 2040 746f  /test")..    @to
+000019f0: 7263 682e 6e6f 5f67 7261 6428 290d 0a20  rch.no_grad().. 
+00001a00: 2020 2064 6566 2074 6573 7428 7365 6c66     def test(self
+00001a10: 2c20 6570 6f63 683a 2069 6e74 293a 0d0a  , epoch: int):..
+00001a20: 2020 2020 2020 2020 2222 2253 7461 7274          """Start
+00001a30: 2074 6573 7469 6e67 2061 6e64 2072 6574   testing and ret
+00001a40: 7572 6e20 7468 6520 7465 7374 206d 6574  urn the test met
+00001a50: 7269 6373 2e22 2222 0d0a 2020 2020 2020  rics."""..      
+00001a60: 2020 7365 6c66 2e5f 5f6d 6f64 6520 3d20    self.__mode = 
+00001a70: 2774 6573 7427 0d0a 2020 2020 2020 2020  'test'..        
+00001a80: 7365 6c66 2e6d 6f64 656c 2e65 7661 6c28  self.model.eval(
+00001a90: 290d 0a20 2020 2020 2020 2072 6574 7572  )..        retur
+00001aa0: 6e20 7365 6c66 2e65 7661 6c75 6174 6528  n self.evaluate(
+00001ab0: 6570 6f63 683d 6570 6f63 682c 2070 7265  epoch=epoch, pre
+00001ac0: 6669 783d 2774 6573 7427 290d 0a0d 0a20  fix='test').... 
+00001ad0: 2020 2040 6162 632e 6162 7374 7261 6374     @abc.abstract
+00001ae0: 6d65 7468 6f64 0d0a 2020 2020 6465 6620  method..    def 
+00001af0: 7472 6169 6e5f 7065 725f 6570 6f63 6828  train_per_epoch(
+00001b00: 7365 6c66 2c20 6570 6f63 683a 2069 6e74  self, epoch: int
+00001b10: 293a 0d0a 2020 2020 2020 2020 7261 6973  ):..        rais
+00001b20: 6520 4e6f 7449 6d70 6c65 6d65 6e74 6564  e NotImplemented
+00001b30: 4572 726f 7228 0d0a 2020 2020 2020 2020  Error(..        
+00001b40: 2020 2020 6622 7b73 656c 662e 5f5f 636c      f"{self.__cl
+00001b50: 6173 735f 5f2e 5f5f 6e61 6d65 5f5f 7d2e  ass__.__name__}.
+00001b60: 7472 6169 6e5f 7065 725f 6570 6f63 6828  train_per_epoch(
+00001b70: 2920 7368 6f75 6c64 2062 6520 696d 706c  ) should be impl
+00001b80: 656d 656e 7465 6420 2e2e 2e22 0d0a 2020  emented ..."..  
+00001b90: 2020 2020 2020 290d 0a0d 0a20 2020 2040        )....    @
+00001ba0: 6162 632e 6162 7374 7261 6374 6d65 7468  abc.abstractmeth
+00001bb0: 6f64 0d0a 2020 2020 6465 6620 6576 616c  od..    def eval
+00001bc0: 7561 7465 2873 656c 662c 2065 706f 6368  uate(self, epoch
+00001bd0: 3a20 696e 742c 2070 7265 6669 783a 2073  : int, prefix: s
+00001be0: 7472 203d 2027 7661 6c69 6427 293a 0d0a  tr = 'valid'):..
+00001bf0: 2020 2020 2020 2020 7261 6973 6520 4e6f          raise No
+00001c00: 7449 6d70 6c65 6d65 6e74 6564 4572 726f  tImplementedErro
+00001c10: 7228 0d0a 2020 2020 2020 2020 2020 2020  r(..            
+00001c20: 6622 7b73 656c 662e 5f5f 636c 6173 735f  f"{self.__class_
+00001c30: 5f2e 5f5f 6e61 6d65 5f5f 7d2e 6576 616c  _.__name__}.eval
+00001c40: 7561 7465 2829 2073 686f 756c 6420 6265  uate() should be
+00001c50: 2069 6d70 6c65 6d65 6e74 6564 202e 2e2e   implemented ...
+00001c60: 220d 0a20 2020 2020 2020 2029 0d0a 0d0a  "..        )....
+00001c70: 2020 2020 6465 6620 7265 6769 7374 6572      def register
+00001c80: 5f6d 6574 7269 6328 0d0a 2020 2020 2020  _metric(..      
+00001c90: 2020 7365 6c66 2c20 6e61 6d65 3a20 7374    self, name: st
+00001ca0: 722c 2066 756e 633a 2043 616c 6c61 626c  r, func: Callabl
+00001cb0: 652c 200d 0a20 2020 2020 2020 2066 6d74  e, ..        fmt
+00001cc0: 3a20 7374 7220 3d20 272e 3466 272c 2062  : str = '.4f', b
+00001cd0: 6573 745f 6361 7374 6572 3a20 4361 6c6c  est_caster: Call
+00001ce0: 6162 6c65 203d 206d 6178 0d0a 2020 2020  able = max..    
+00001cf0: 2920 2d3e 204e 6f6e 653a 0d0a 2020 2020  ) -> None:..    
+00001d00: 2020 2020 7222 2222 0d0a 2020 2020 2020      r"""..      
+00001d10: 2020 5265 6769 7374 6572 2061 206d 6574    Register a met
+00001d20: 7269 632e 0d0a 0d0a 2020 2020 2020 2020  ric.....        
+00001d30: 5061 7261 6d65 7465 7273 0d0a 2020 2020  Parameters..    
+00001d40: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a      ----------..
+00001d50: 2020 2020 2020 2020 6e61 6d65 203a 2073          name : s
+00001d60: 7472 0d0a 2020 2020 2020 2020 2020 2020  tr..            
+00001d70: 5468 6520 636f 6d70 6c65 7465 206e 616d  The complete nam
+00001d80: 6520 6f66 2074 6865 206d 6574 7269 632c  e of the metric,
+00001d90: 2073 7563 6820 6173 2060 4c4f 5353 3260   such as `LOSS2`
+00001da0: 2e0d 0a20 2020 2020 2020 2020 2020 2054  ...            T
+00001db0: 6865 206e 6f74 6174 696f 6e20 6040 6020  he notation `@` 
+00001dc0: 7368 6f75 6c64 206e 6f74 2062 6520 696e  should not be in
+00001dd0: 636c 7564 6564 2c20 692e 652e 2c20 274c  cluded, i.e., 'L
+00001de0: 4f53 5340 3227 2069 7320 696e 7661 6c69  OSS@2' is invali
+00001df0: 642e 0d0a 2020 2020 2020 2020 6675 6e63  d...        func
+00001e00: 203a 2043 616c 6c61 626c 650d 0a20 2020   : Callable..   
+00001e10: 2020 2020 2020 2020 2054 6865 2066 756e           The fun
+00001e20: 6374 696f 6e20 746f 2070 726f 6365 7373  ction to process
+00001e30: 2074 6865 2064 6174 6120 666f 7220 7468   the data for th
+00001e40: 6520 6d65 7472 6963 2e0d 0a20 2020 2020  e metric...     
+00001e50: 2020 2066 6d74 203a 2073 7472 2c20 6f70     fmt : str, op
+00001e60: 7469 6f6e 616c 0d0a 2020 2020 2020 2020  tional..        
+00001e70: 2020 2020 5468 6520 666f 726d 6174 2074      The format t
+00001e80: 6f20 7573 6520 7768 656e 2070 7269 6e74  o use when print
+00001e90: 696e 6720 7468 6520 6d65 7472 6963 2c20  ing the metric, 
+00001ea0: 6465 6661 756c 7473 2074 6f20 6027 2e34  defaults to `'.4
+00001eb0: 6627 602e 0d0a 2020 2020 2020 2020 6265  f'`...        be
+00001ec0: 7374 5f63 6173 7465 7220 3a20 4361 6c6c  st_caster : Call
+00001ed0: 6162 6c65 2c20 6f70 7469 6f6e 616c 0d0a  able, optional..
+00001ee0: 2020 2020 2020 2020 2020 2020 4120 6675              A fu
+00001ef0: 6e63 7469 6f6e 2075 7365 6420 746f 2063  nction used to c
+00001f00: 6173 7420 7468 6520 6265 7374 2076 616c  ast the best val
+00001f10: 7565 206f 6620 7468 6520 6d65 7472 6963  ue of the metric
+00001f20: 2c20 6465 6661 756c 7473 2074 6f20 606d  , defaults to `m
+00001f30: 6178 602e 0d0a 2020 2020 2020 2020 2020  ax`...          
+00001f40: 2020 0d0a 2020 2020 2020 2020 5265 7475    ..        Retu
+00001f50: 726e 730d 0a20 2020 2020 2020 202d 2d2d  rns..        ---
+00001f60: 2d2d 2d2d 0d0a 2020 2020 2020 2020 4e6f  ----..        No
+00001f70: 6e65 0d0a 2020 2020 2020 2020 0d0a 2020  ne..        ..  
+00001f80: 2020 2020 2020 5261 6973 6573 0d0a 2020        Raises..  
+00001f90: 2020 2020 2020 2d2d 2d2d 2d2d 0d0a 2020        ------..  
+00001fa0: 2020 2020 2020 4173 7365 7274 696f 6e45        AssertionE
+00001fb0: 7272 6f72 0d0a 2020 2020 2020 2020 2020  rror..          
+00001fc0: 2020 5768 656e 2060 6e61 6d65 6020 6861    When `name` ha
+00001fd0: 7320 616c 7265 6164 7920 6265 656e 2072  s already been r
+00001fe0: 6567 6973 7465 7265 6420 6f72 2063 6f6e  egistered or con
+00001ff0: 7461 696e 7320 7468 6520 6e6f 7461 7469  tains the notati
+00002000: 6f6e 2060 4060 2e0d 0a20 2020 2020 2020  on `@`...       
+00002010: 2022 2222 0d0a 0d0a 2020 2020 2020 2020   """....        
+00002020: 6e61 6d65 203d 206e 616d 652e 7570 7065  name = name.uppe
+00002030: 7228 290d 0a20 2020 2020 2020 2061 7373  r()..        ass
+00002040: 6572 7420 4445 4641 554c 545f 4d45 5452  ert DEFAULT_METR
+00002050: 4943 532e 6765 7428 6e61 6d65 2c20 4e6f  ICS.get(name, No
+00002060: 6e65 2920 6973 204e 6f6e 652c 2066 2254  ne) is None, f"T
+00002070: 6865 206d 6574 7269 6320 7b6e 616d 657d  he metric {name}
+00002080: 2061 6c72 6561 6479 2065 7869 7374 7320   already exists 
+00002090: 2e2e 2e22 0d0a 2020 2020 2020 2020 6173  ..."..        as
+000020a0: 7365 7274 2027 4027 206e 6f74 2069 6e20  sert '@' not in 
+000020b0: 6e61 6d65 2c20 6622 5468 6520 6d65 7472  name, f"The metr
+000020c0: 6963 206e 616d 6520 6861 7320 696e 7661  ic name has inva
+000020d0: 6c69 6420 6e6f 7461 7469 6f6e 206f 6620  lid notation of 
+000020e0: 6040 2720 2e2e 2e22 0d0a 2020 2020 2020  `@' ..."..      
+000020f0: 2020 4445 4641 554c 545f 4d45 5452 4943    DEFAULT_METRIC
+00002100: 535b 6e61 6d65 5d20 3d20 6675 6e63 0d0a  S[name] = func..
+00002110: 2020 2020 2020 2020 4445 4641 554c 545f          DEFAULT_
+00002120: 464d 5453 5b6e 616d 655d 203d 2066 6d74  FMTS[name] = fmt
+00002130: 0d0a 2020 2020 2020 2020 4445 4641 554c  ..        DEFAUL
+00002140: 545f 4245 5354 5f43 4153 5445 525b 6e61  T_BEST_CASTER[na
+00002150: 6d65 5d20 3d20 6265 7374 5f63 6173 7465  me] = best_caste
+00002160: 720d 0a0d 0a0d 0a63 6c61 7373 2043 6f61  r......class Coa
+00002170: 6368 2843 6869 6566 436f 6163 6829 3a0d  ch(ChiefCoach):.
+00002180: 0a20 2020 2022 2222 5468 6520 6672 616d  .    """The fram
+00002190: 6577 6f72 6b20 666f 7220 7472 6169 6e69  ework for traini
+000021a0: 6e67 2e22 2222 0d0a 0d0a 2020 2020 6465  ng."""....    de
+000021b0: 6620 7072 6570 6172 655f 6461 7461 6c6f  f prepare_datalo
+000021c0: 6164 6572 2873 656c 6629 202d 3e20 4e6f  ader(self) -> No
+000021d0: 6e65 3a0d 0a20 2020 2020 2020 2022 2222  ne:..        """
+000021e0: 5072 6570 6172 6520 6461 7461 206c 6f61  Prepare data loa
+000021f0: 6465 7273 2066 6f72 2074 7261 696e 696e  ders for trainin
+00002200: 672c 2076 616c 6964 6174 696f 6e2c 2061  g, validation, a
+00002210: 6e64 2074 6573 7469 6e67 2064 6174 612e  nd testing data.
+00002220: 2222 220d 0a20 2020 2020 2020 2073 656c  """..        sel
+00002230: 662e 7472 6169 6e6c 6f61 6465 7220 3d20  f.trainloader = 
+00002240: 4461 7461 4c6f 6164 6572 280d 0a20 2020  DataLoader(..   
+00002250: 2020 2020 2020 2020 2064 6174 6170 6970           datapip
+00002260: 653d 7365 6c66 2e74 7261 696e 7069 7065  e=self.trainpipe
+00002270: 2c20 0d0a 2020 2020 2020 2020 2020 2020  , ..            
+00002280: 6e75 6d5f 776f 726b 6572 733d 7365 6c66  num_workers=self
+00002290: 2e63 6667 2e6e 756d 5f77 6f72 6b65 7273  .cfg.num_workers
+000022a0: 2c0d 0a20 2020 2020 2020 2020 2020 2070  ,..            p
+000022b0: 696e 5f6d 656d 6f72 793d 7365 6c66 2e63  in_memory=self.c
+000022c0: 6667 2e70 696e 5f6d 656d 6f72 790d 0a20  fg.pin_memory.. 
+000022d0: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
+000022e0: 2020 7365 6c66 2e76 616c 6964 6c6f 6164    self.validload
+000022f0: 6572 203d 2044 6174 614c 6f61 6465 7228  er = DataLoader(
+00002300: 0d0a 2020 2020 2020 2020 2020 2020 6461  ..            da
+00002310: 7461 7069 7065 3d73 656c 662e 7661 6c69  tapipe=self.vali
+00002320: 6470 6970 652c 200d 0a20 2020 2020 2020  dpipe, ..       
+00002330: 2020 2020 206e 756d 5f77 6f72 6b65 7273       num_workers
+00002340: 3d73 656c 662e 6366 672e 6e75 6d5f 776f  =self.cfg.num_wo
+00002350: 726b 6572 732c 0d0a 2020 2020 2020 2020  rkers,..        
+00002360: 2020 2020 7069 6e5f 6d65 6d6f 7279 3d73      pin_memory=s
+00002370: 656c 662e 6366 672e 7069 6e5f 6d65 6d6f  elf.cfg.pin_memo
+00002380: 7279 0d0a 2020 2020 2020 2020 290d 0a20  ry..        ).. 
+00002390: 2020 2020 2020 2073 656c 662e 7465 7374         self.test
+000023a0: 6c6f 6164 6572 203d 2044 6174 614c 6f61  loader = DataLoa
+000023b0: 6465 7228 0d0a 2020 2020 2020 2020 2020  der(..          
+000023c0: 2020 6461 7461 7069 7065 3d73 656c 662e    datapipe=self.
+000023d0: 7465 7374 7069 7065 2c20 0d0a 2020 2020  testpipe, ..    
+000023e0: 2020 2020 2020 2020 6e75 6d5f 776f 726b          num_work
+000023f0: 6572 733d 7365 6c66 2e63 6667 2e6e 756d  ers=self.cfg.num
+00002400: 5f77 6f72 6b65 7273 2c0d 0a20 2020 2020  _workers,..     
+00002410: 2020 2020 2020 2070 696e 5f6d 656d 6f72         pin_memor
+00002420: 793d 7365 6c66 2e63 6667 2e70 696e 5f6d  y=self.cfg.pin_m
+00002430: 656d 6f72 790d 0a20 2020 2020 2020 2029  emory..        )
+00002440: 0d0a 2020 2020 0d0a 2020 2020 4070 726f  ..    ..    @pro
+00002450: 7065 7274 790d 0a20 2020 2064 6566 2064  perty..    def d
+00002460: 6174 616c 6f61 6465 7228 7365 6c66 293a  ataloader(self):
+00002470: 0d0a 2020 2020 2020 2020 2222 2252 6574  ..        """Ret
+00002480: 7572 6e20 7468 6520 636f 7272 6573 706f  urn the correspo
+00002490: 6e64 696e 6720 6461 7461 206c 6f61 6465  nding data loade
+000024a0: 7220 6465 7065 6e64 696e 6720 6f6e 2074  r depending on t
+000024b0: 6865 2063 7572 7265 6e74 206d 6f64 652e  he current mode.
+000024c0: 2222 220d 0a20 2020 2020 2020 2069 6620  """..        if 
+000024d0: 7365 6c66 2e6d 6f64 6520 3d3d 2027 7472  self.mode == 'tr
+000024e0: 6169 6e27 3a0d 0a20 2020 2020 2020 2020  ain':..         
+000024f0: 2020 2072 6574 7572 6e20 7365 6c66 2e74     return self.t
+00002500: 7261 696e 6c6f 6164 6572 0d0a 2020 2020  rainloader..    
+00002510: 2020 2020 656c 6966 2073 656c 662e 6d6f      elif self.mo
+00002520: 6465 203d 3d20 2776 616c 6964 273a 0d0a  de == 'valid':..
+00002530: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00002540: 726e 2073 656c 662e 7661 6c69 646c 6f61  rn self.validloa
+00002550: 6465 720d 0a20 2020 2020 2020 2065 6c73  der..        els
+00002560: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+00002570: 7265 7475 726e 2073 656c 662e 7465 7374  return self.test
+00002580: 6c6f 6164 6572 0d0a 0d0a 2020 2020 4070  loader....    @p
+00002590: 726f 7065 7274 790d 0a20 2020 2064 6566  roperty..    def
+000025a0: 206d 6f6e 6974 6f72 7328 7365 6c66 2920   monitors(self) 
+000025b0: 2d3e 204d 6f6e 6974 6f72 3a0d 0a20 2020  -> Monitor:..   
+000025c0: 2020 2020 2022 2222 5265 7475 726e 2074       """Return t
+000025d0: 6865 206d 6f6e 6974 6f72 2064 6963 7469  he monitor dicti
+000025e0: 6f6e 6172 7920 666f 7220 7468 6520 6469  onary for the di
+000025f0: 6666 6572 656e 7420 6d6f 6465 7320 2827  fferent modes ('
+00002600: 7472 6169 6e27 2c20 2776 616c 6964 272c  train', 'valid',
+00002610: 2027 7465 7374 2729 2e22 2222 0d0a 2020   'test')."""..  
+00002620: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+00002630: 662e 5f5f 6d6f 6e69 746f 7273 0d0a 0d0a  f.__monitors....
+00002640: 2020 2020 4070 726f 7065 7274 790d 0a20      @property.. 
+00002650: 2020 2064 6566 206d 6574 6572 3462 6573     def meter4bes
+00002660: 7428 7365 6c66 293a 0d0a 2020 2020 2020  t(self):..      
+00002670: 2020 7265 7475 726e 2073 656c 662e 5f5f    return self.__
+00002680: 6265 7374 5f6d 6574 6572 0d0a 0d0a 2020  best_meter....  
+00002690: 2020 406d 6574 6572 3462 6573 742e 7365    @meter4best.se
+000026a0: 7474 6572 0d0a 2020 2020 6465 6620 6d65  tter..    def me
+000026b0: 7465 7234 6265 7374 2873 656c 662c 206d  ter4best(self, m
+000026c0: 6574 6572 3a20 4176 6572 6167 654d 6574  eter: AverageMet
+000026d0: 6572 293a 0d0a 2020 2020 2020 2020 7365  er):..        se
+000026e0: 6c66 2e5f 5f62 6573 745f 6d65 7465 7220  lf.__best_meter 
+000026f0: 3d20 6d65 7465 720d 0a20 2020 2020 2020  = meter..       
+00002700: 2069 6e66 6f4c 6f67 6765 7228 6622 5b43   infoLogger(f"[C
+00002710: 6f61 6368 5d20 3e3e 3e20 5365 7420 6265  oach] >>> Set be
+00002720: 7374 206d 6574 6572 3a20 7b6d 6574 6572  st meter: {meter
+00002730: 2e6e 616d 657d 2022 290d 0a0d 0a20 2020  .name} ")....   
+00002740: 2040 7469 6d65 6d65 7465 7228 2243 6f61   @timemeter("Coa
+00002750: 6368 2f63 6f6d 7069 6c65 2229 0d0a 2020  ch/compile")..  
+00002760: 2020 6465 6620 636f 6d70 696c 6528 0d0a    def compile(..
+00002770: 2020 2020 2020 2020 7365 6c66 2c20 6366          self, cf
+00002780: 673a 2043 6f6e 6669 672c 206d 6f6e 6974  g: Config, monit
+00002790: 6f72 733a 204c 6973 745b 7374 725d 2c20  ors: List[str], 
+000027a0: 0d0a 2020 2020 2020 2020 7768 6963 6834  ..        which4
+000027b0: 6265 7374 3a20 7374 7220 3d20 274c 4f53  best: str = 'LOS
+000027c0: 5327 0d0a 2020 2020 293a 0d0a 2020 2020  S'..    ):..    
+000027d0: 2020 2020 7222 2222 0d0a 2020 2020 2020      r"""..      
+000027e0: 2020 4c6f 6164 2074 6865 2063 6f6e 6669    Load the confi
+000027f0: 6775 7261 7469 6f6e 2061 6e64 2073 6574  guration and set
+00002800: 2075 7020 6d6f 6e69 746f 7273 2066 6f72   up monitors for
+00002810: 2074 7261 696e 696e 672e 0d0a 0d0a 2020   training.....  
+00002820: 2020 2020 2020 5061 7261 6d65 7465 7273        Parameters
+00002830: 0d0a 2020 2020 2020 2020 2d2d 2d2d 2d2d  ..        ------
+00002840: 2d2d 2d2d 0d0a 2020 2020 2020 2020 6366  ----..        cf
+00002850: 6720 3a20 436f 6e66 6967 0d0a 2020 2020  g : Config..    
+00002860: 2020 2020 2020 2020 4120 636f 6e66 6967          A config
+00002870: 7572 6174 696f 6e20 6f62 6a65 6374 2077  uration object w
+00002880: 6974 6820 7468 6520 7472 6169 6e69 6e67  ith the training
+00002890: 2064 6574 6169 6c73 2e0d 0a20 2020 2020   details...     
+000028a0: 2020 206d 6f6e 6974 6f72 7320 3a20 4c69     monitors : Li
+000028b0: 7374 5b73 7472 5d0d 0a20 2020 2020 2020  st[str]..       
+000028c0: 2020 2020 2041 206c 6973 7420 6f66 206d       A list of m
+000028d0: 6574 7269 6320 6e61 6d65 7320 746f 2062  etric names to b
+000028e0: 6520 6d6f 6e69 746f 7265 6420 6475 7269  e monitored duri
+000028f0: 6e67 2074 7261 696e 696e 672e 0d0a 2020  ng training...  
+00002900: 2020 2020 2020 7768 6963 6834 6265 7374        which4best
+00002910: 203a 2073 7472 2c20 6465 6661 756c 7473   : str, defaults
+00002920: 2060 4c4f 5353 270d 0a20 2020 2020 2020   `LOSS'..       
+00002930: 2020 2020 2054 6865 206d 6574 7269 6320       The metric 
+00002940: 7573 6564 2066 6f72 2073 656c 6563 7469  used for selecti
+00002950: 6e67 2074 6865 2062 6573 7420 6368 6563  ng the best chec
+00002960: 6b70 6f69 6e74 2e0d 0a0d 0a20 2020 2020  kpoint.....     
+00002970: 2020 2045 7861 6d70 6c65 730d 0a20 2020     Examples..   
+00002980: 2020 2020 202d 2d2d 2d2d 2d2d 2d0d 0a20       --------.. 
+00002990: 2020 2020 2020 203e 3e3e 2063 6f61 6368         >>> coach
+000029a0: 3a20 436f 6163 680d 0a20 2020 2020 2020  : Coach..       
+000029b0: 203e 3e3e 2063 6f61 6368 2e63 6f6d 7069   >>> coach.compi
+000029c0: 6c65 2863 6667 2c20 6d6f 6e69 746f 7273  le(cfg, monitors
+000029d0: 3d5b 276c 6f73 7327 2c20 2772 6563 616c  =['loss', 'recal
+000029e0: 6c40 3130 272c 2027 7265 6361 6c6c 4032  l@10', 'recall@2
+000029f0: 3027 2c20 276e 6463 6740 3130 272c 2027  0', 'ndcg@10', '
+00002a00: 6e64 6367 4032 3027 5d29 0d0a 2020 2020  ndcg@20'])..    
+00002a10: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
+00002a20: 2073 656c 662e 6366 6720 3d20 6366 670d   self.cfg = cfg.
+00002a30: 0a20 2020 2020 2020 2023 206d 6574 6572  .        # meter
+00002a40: 7320 666f 7220 7472 6169 6e7c 7661 6c69  s for train|vali
+00002a50: 647c 7465 7374 0d0a 2020 2020 2020 2020  d|test..        
+00002a60: 7365 6c66 2e5f 5f6d 6f6e 6974 6f72 7320  self.__monitors 
+00002a70: 3d20 4d6f 6e69 746f 7228 290d 0a20 2020  = Monitor()..   
+00002a80: 2020 2020 2073 656c 662e 5f5f 6d6f 6e69       self.__moni
+00002a90: 746f 7273 5b27 7472 6169 6e27 5d20 3d20  tors['train'] = 
+00002aa0: 6465 6661 756c 7464 6963 7428 6c69 7374  defaultdict(list
+00002ab0: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00002ac0: 5f5f 6d6f 6e69 746f 7273 5b27 7661 6c69  __monitors['vali
+00002ad0: 6427 5d20 3d20 6465 6661 756c 7464 6963  d'] = defaultdic
+00002ae0: 7428 6c69 7374 290d 0a20 2020 2020 2020  t(list)..       
+00002af0: 2073 656c 662e 5f5f 6d6f 6e69 746f 7273   self.__monitors
+00002b00: 5b27 7465 7374 275d 203d 2064 6566 6175  ['test'] = defau
+00002b10: 6c74 6469 6374 286c 6973 7429 0d0a 0d0a  ltdict(list)....
+00002b20: 2020 2020 2020 2020 6465 6620 7365 745f          def set_
+00002b30: 6d6f 6e69 746f 7228 0d0a 2020 2020 2020  monitor(..      
+00002b40: 2020 2020 2020 6e61 6d65 3a20 7374 722c        name: str,
+00002b50: 206c 6173 746e 616d 653a 2073 7472 2c20   lastname: str, 
+00002b60: 7072 6566 6978 3a20 7374 7220 3d20 2774  prefix: str = 't
+00002b70: 7261 696e 272c 202a 2a6b 7761 7267 730d  rain', **kwargs.
+00002b80: 0a20 2020 2020 2020 2029 3a0d 0a20 2020  .        ):..   
+00002b90: 2020 2020 2020 2020 2022 2222 4164 6420           """Add 
+00002ba0: 6120 6d6f 6e69 746f 7220 666f 7220 7468  a monitor for th
+00002bb0: 6520 7370 6563 6966 6965 6420 6d65 7472  e specified metr
+00002bc0: 6963 2e22 2222 0d0a 2020 2020 2020 2020  ic."""..        
+00002bd0: 2020 2020 7472 793a 0d0a 2020 2020 2020      try:..      
+00002be0: 2020 2020 2020 2020 2020 6d65 7465 7220            meter 
+00002bf0: 3d20 4176 6572 6167 654d 6574 6572 280d  = AverageMeter(.
+00002c00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002c10: 2020 2020 2020 2020 206e 616d 653d 6e61           name=na
+00002c20: 6d65 2c0d 0a20 2020 2020 2020 2020 2020  me,..           
+00002c30: 2020 2020 2020 2020 2020 2020 206d 6574               met
+00002c40: 7269 633d 7061 7274 6961 6c28 4445 4641  ric=partial(DEFA
+00002c50: 554c 545f 4d45 5452 4943 535b 6c61 7374  ULT_METRICS[last
+00002c60: 6e61 6d65 5d2c 202a 2a6b 7761 7267 7329  name], **kwargs)
+00002c70: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00002c80: 2020 2020 2020 2020 2020 2066 6d74 3d44             fmt=D
+00002c90: 4546 4155 4c54 5f46 4d54 535b 6c61 7374  EFAULT_FMTS[last
+00002ca0: 6e61 6d65 5d2c 0d0a 2020 2020 2020 2020  name],..        
+00002cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002cc0: 6265 7374 5f63 6173 7465 723d 4445 4641  best_caster=DEFA
+00002cd0: 554c 545f 4245 5354 5f43 4153 5445 525b  ULT_BEST_CASTER[
+00002ce0: 6c61 7374 6e61 6d65 5d0d 0a20 2020 2020  lastname]..     
+00002cf0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+00002d00: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00002d10: 2020 7365 6c66 2e5f 5f6d 6f6e 6974 6f72    self.__monitor
+00002d20: 735b 7072 6566 6978 5d5b 6c61 7374 6e61  s[prefix][lastna
+00002d30: 6d65 5d2e 6170 7065 6e64 286d 6574 6572  me].append(meter
+00002d40: 290d 0a20 2020 2020 2020 2020 2020 2065  )..            e
+00002d50: 7863 6570 7420 4b65 7945 7272 6f72 3a0d  xcept KeyError:.
+00002d60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002d70: 2072 6169 7365 204b 6579 4572 726f 7228   raise KeyError(
+00002d80: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00002d90: 2020 2020 2020 6622 5468 6520 6d65 7472        f"The metr
+00002da0: 6963 206f 6620 7b6c 6173 746e 616d 657d  ic of {lastname}
+00002db0: 2069 7320 6e6f 7420 696e 636c 7564 6564   is not included
+00002dc0: 2e20 220d 0a20 2020 2020 2020 2020 2020  . "..           
+00002dd0: 2020 2020 2020 2020 2066 2259 6f75 2063           f"You c
+00002de0: 616e 2072 6567 6973 7465 7220 6279 2063  an register by c
+00002df0: 616c 6c69 6e67 2060 7265 6769 7374 6572  alling `register
+00002e00: 5f6d 6574 7269 6328 2e2e 2e29 2720 2e2e  _metric(...)' ..
+00002e10: 2e22 0d0a 2020 2020 2020 2020 2020 2020  ."..            
+00002e20: 2020 2020 290d 0a20 2020 2020 2020 2020      )..         
+00002e30: 2020 2072 6574 7572 6e20 6d65 7465 720d     return meter.
+00002e40: 0a0d 0a20 2020 2020 2020 2023 2055 5050  ...        # UPP
+00002e50: 4552 0d0a 2020 2020 2020 2020 7768 6963  ER..        whic
+00002e60: 6834 6265 7374 203d 2077 6869 6368 3462  h4best = which4b
+00002e70: 6573 742e 7570 7065 7228 290d 0a20 2020  est.upper()..   
+00002e80: 2020 2020 206d 6f6e 6974 6f72 7320 3d20       monitors = 
+00002e90: 5b27 4c4f 5353 275d 202b 205b 6e61 6d65  ['LOSS'] + [name
+00002ea0: 2e75 7070 6572 2829 2066 6f72 206e 616d  .upper() for nam
+00002eb0: 6520 696e 206d 6f6e 6974 6f72 735d 202b  e in monitors] +
+00002ec0: 205b 7768 6963 6834 6265 7374 5d0d 0a20   [which4best].. 
+00002ed0: 2020 2020 2020 206d 6f6e 6974 6f72 7320         monitors 
+00002ee0: 3d20 736f 7274 6564 2873 6574 286d 6f6e  = sorted(set(mon
+00002ef0: 6974 6f72 7329 2c20 6b65 793d 6d6f 6e69  itors), key=moni
+00002f00: 746f 7273 2e69 6e64 6578 290d 0a0d 0a20  tors.index).... 
+00002f10: 2020 2020 2020 2066 6f72 206e 616d 6520         for name 
+00002f20: 696e 206d 6f6e 6974 6f72 733a 0d0a 2020  in monitors:..  
+00002f30: 2020 2020 2020 2020 2020 666f 7220 7072            for pr
+00002f40: 6566 6978 2069 6e20 2827 7472 6169 6e27  efix in ('train'
+00002f50: 2c20 2776 616c 6964 272c 2027 7465 7374  , 'valid', 'test
+00002f60: 2729 3a0d 0a20 2020 2020 2020 2020 2020  '):..           
+00002f70: 2020 2020 2069 6620 2740 2720 696e 206e       if '@' in n
+00002f80: 616d 653a 0d0a 2020 2020 2020 2020 2020  ame:..          
+00002f90: 2020 2020 2020 2020 2020 6c61 7374 6e61            lastna
+00002fa0: 6d65 2c20 4b20 3d20 6e61 6d65 2e73 706c  me, K = name.spl
+00002fb0: 6974 2827 4027 290d 0a20 2020 2020 2020  it('@')..       
+00002fc0: 2020 2020 2020 2020 2020 2020 206d 6574               met
+00002fd0: 6572 203d 2073 6574 5f6d 6f6e 6974 6f72  er = set_monitor
+00002fe0: 280d 0a20 2020 2020 2020 2020 2020 2020  (..             
+00002ff0: 2020 2020 2020 2020 2020 206e 616d 653d             name=
+00003000: 6e61 6d65 2c0d 0a20 2020 2020 2020 2020  name,..         
+00003010: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+00003020: 6173 746e 616d 653d 6c61 7374 6e61 6d65  astname=lastname
+00003030: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00003040: 2020 2020 2020 2020 2020 2070 7265 6669             prefi
+00003050: 783d 7072 6566 6978 2c0d 0a20 2020 2020  x=prefix,..     
+00003060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003070: 2020 206b 3d69 6e74 284b 290d 0a20 2020     k=int(K)..   
+00003080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003090: 2029 0d0a 2020 2020 2020 2020 2020 2020   )..            
+000030a0: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
+000030b0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+000030c0: 6173 746e 616d 6520 3d20 6e61 6d65 0d0a  astname = name..
+000030d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000030e0: 2020 2020 6d65 7465 7220 3d20 7365 745f      meter = set_
+000030f0: 6d6f 6e69 746f 7228 0d0a 2020 2020 2020  monitor(..      
+00003100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003110: 2020 6e61 6d65 3d6e 616d 652c 0d0a 2020    name=name,..  
+00003120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003130: 2020 2020 2020 6c61 7374 6e61 6d65 3d6c        lastname=l
+00003140: 6173 746e 616d 652c 0d0a 2020 2020 2020  astname,..      
+00003150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003160: 2020 7072 6566 6978 3d70 7265 6669 780d    prefix=prefix.
+00003170: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003180: 2020 2020 2029 0d0a 2020 2020 2020 2020       )..        
+00003190: 2020 2020 2020 2020 6966 2070 7265 6669          if prefi
+000031a0: 7820 3d3d 2027 7661 6c69 6427 2061 6e64  x == 'valid' and
+000031b0: 206e 616d 6520 3d3d 2077 6869 6368 3462   name == which4b
+000031c0: 6573 743a 0d0a 2020 2020 2020 2020 2020  est:..          
+000031d0: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
+000031e0: 6574 6572 3462 6573 7420 3d20 6d65 7465  eter4best = mete
+000031f0: 720d 0a20 2020 2020 2020 2020 2020 2020  r..             
+00003200: 2020 2020 2020 2073 656c 662e 5f62 6573         self._bes
+00003210: 7420 3d20 2d66 6c6f 6174 2827 696e 6627  t = -float('inf'
+00003220: 2920 6966 206d 6574 6572 2e63 6173 7465  ) if meter.caste
+00003230: 7220 6973 206d 6178 2065 6c73 6520 666c  r is max else fl
+00003240: 6f61 7428 2769 6e66 2729 0d0a 2020 2020  oat('inf')..    
+00003250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003260: 7365 6c66 2e5f 6265 7374 5f65 706f 6368  self._best_epoch
+00003270: 203d 2030 0d0a 0d0a 2020 2020 2020 2020   = 0....        
+00003280: 2320 5072 6570 6172 6520 6461 7461 206c  # Prepare data l
+00003290: 6f61 6465 7273 0d0a 2020 2020 2020 2020  oaders..        
+000032a0: 7365 6c66 2e70 7265 7061 7265 5f64 6174  self.prepare_dat
+000032b0: 616c 6f61 6465 7228 290d 0a0d 0a20 2020  aloader()....   
+000032c0: 2064 6566 2073 6176 6528 7365 6c66 2920   def save(self) 
+000032d0: 2d3e 204e 6f6e 653a 0d0a 2020 2020 2020  -> None:..      
+000032e0: 2020 2222 2253 6176 6520 7468 6520 6d6f    """Save the mo
+000032f0: 6465 6c22 2222 0d0a 2020 2020 2020 2020  del"""..        
+00003300: 746f 7263 682e 7361 7665 2873 656c 662e  torch.save(self.
+00003310: 6d6f 6465 6c2e 7374 6174 655f 6469 6374  model.state_dict
+00003320: 2829 2c20 6f73 2e70 6174 682e 6a6f 696e  (), os.path.join
+00003330: 2873 656c 662e 6366 672e 4c4f 475f 5041  (self.cfg.LOG_PA
+00003340: 5448 2c20 7365 6c66 2e63 6667 2e53 4156  TH, self.cfg.SAV
+00003350: 4544 5f46 494c 454e 414d 4529 290d 0a0d  ED_FILENAME))...
+00003360: 0a20 2020 2064 6566 206c 6f61 6428 7365  .    def load(se
+00003370: 6c66 2c20 7061 7468 3a20 7374 722c 2066  lf, path: str, f
+00003380: 696c 656e 616d 653a 204f 7074 696f 6e61  ilename: Optiona
+00003390: 6c5b 7374 725d 203d 204e 6f6e 652c 202a  l[str] = None, *
+000033a0: 2a6b 7761 7267 7329 202d 3e20 4e6f 6e65  *kwargs) -> None
+000033b0: 3a0d 0a20 2020 2020 2020 2066 696c 656e  :..        filen
+000033c0: 616d 6520 3d20 7365 6c66 2e63 6667 2e53  ame = self.cfg.S
+000033d0: 4156 4544 5f46 494c 454e 414d 4520 6966  AVED_FILENAME if
+000033e0: 2066 696c 656e 616d 6520 6973 204e 6f6e   filename is Non
+000033f0: 6520 656c 7365 2066 696c 656e 616d 650d  e else filename.
+00003400: 0a20 2020 2020 2020 2073 656c 662e 6d6f  .        self.mo
+00003410: 6465 6c2e 6c6f 6164 5f73 7461 7465 5f64  del.load_state_d
+00003420: 6963 7428 746f 7263 682e 6c6f 6164 286f  ict(torch.load(o
+00003430: 732e 7061 7468 2e6a 6f69 6e28 7061 7468  s.path.join(path
+00003440: 2c20 6669 6c65 6e61 6d65 292c 202a 2a6b  , filename), **k
+00003450: 7761 7267 7329 290d 0a0d 0a20 2020 2064  wargs))....    d
+00003460: 6566 2073 6176 655f 6368 6563 6b70 6f69  ef save_checkpoi
+00003470: 6e74 2873 656c 662c 2065 706f 6368 3a20  nt(self, epoch: 
+00003480: 696e 7429 202d 3e20 4e6f 6e65 3a0d 0a20  int) -> None:.. 
+00003490: 2020 2020 2020 2072 2222 220d 0a20 2020         r"""..   
+000034a0: 2020 2020 2053 6176 6520 6375 7272 656e       Save curren
+000034b0: 7420 6368 6563 6b70 6f69 6e74 2061 7420  t checkpoint at 
+000034c0: 6570 6f63 682e 0d0a 0d0a 2020 2020 2020  epoch.....      
+000034d0: 2020 5061 7261 6d65 7465 7273 3a0d 0a20    Parameters:.. 
+000034e0: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
+000034f0: 2d2d 0d0a 2020 2020 2020 2020 2020 2020  --..            
+00003500: 6570 6f63 6820 3a69 6e74 2043 7572 7265  epoch :int Curre
+00003510: 6e74 2065 706f 6368 206e 756d 6265 722e  nt epoch number.
+00003520: 0d0a 0d0a 2020 2020 2020 2020 5265 7475  ....        Retu
+00003530: 726e 733a 0d0a 2020 2020 2020 2020 2d2d  rns:..        --
+00003540: 2d2d 2d2d 2d2d 0d0a 2020 2020 2020 2020  ------..        
+00003550: 2020 2020 4e6f 6e65 0d0a 2020 2020 2020      None..      
+00003560: 2020 2222 220d 0a20 2020 2020 2020 2070    """..        p
+00003570: 6174 6820 3d20 6f73 2e70 6174 682e 6a6f  ath = os.path.jo
+00003580: 696e 2873 656c 662e 6366 672e 4348 4543  in(self.cfg.CHEC
+00003590: 4b50 4f49 4e54 5f50 4154 482c 2073 656c  KPOINT_PATH, sel
+000035a0: 662e 6366 672e 4348 4543 4b50 4f49 4e54  f.cfg.CHECKPOINT
+000035b0: 5f46 494c 454e 414d 4529 0d0a 2020 2020  _FILENAME)..    
+000035c0: 2020 2020 6368 6563 6b70 6f69 6e74 203d      checkpoint =
+000035d0: 2064 6963 7428 290d 0a20 2020 2020 2020   dict()..       
+000035e0: 2063 6865 636b 706f 696e 745b 2765 706f   checkpoint['epo
+000035f0: 6368 275d 203d 2065 706f 6368 0d0a 2020  ch'] = epoch..  
+00003600: 2020 2020 2020 666f 7220 6d6f 6475 6c65        for module
+00003610: 2069 6e20 7365 6c66 2e63 6667 2e43 4845   in self.cfg.CHE
+00003620: 434b 504f 494e 545f 4d4f 4455 4c45 533a  CKPOINT_MODULES:
+00003630: 0d0a 2020 2020 2020 2020 2020 2020 6368  ..            ch
+00003640: 6563 6b70 6f69 6e74 5b6d 6f64 756c 655d  eckpoint[module]
+00003650: 203d 2067 6574 6174 7472 2873 656c 662c   = getattr(self,
+00003660: 206d 6f64 756c 6529 2e73 7461 7465 5f64   module).state_d
+00003670: 6963 7428 290d 0a20 2020 2020 2020 2063  ict()..        c
+00003680: 6865 636b 706f 696e 745b 276d 6f6e 6974  heckpoint['monit
+00003690: 6f72 7327 5d20 3d20 7365 6c66 2e6d 6f6e  ors'] = self.mon
+000036a0: 6974 6f72 732e 7374 6174 655f 6469 6374  itors.state_dict
+000036b0: 2829 0d0a 2020 2020 2020 2020 746f 7263  ()..        torc
+000036c0: 682e 7361 7665 2863 6865 636b 706f 696e  h.save(checkpoin
+000036d0: 742c 2070 6174 6829 0d0a 0d0a 2020 2020  t, path)....    
+000036e0: 6465 6620 6c6f 6164 5f63 6865 636b 706f  def load_checkpo
+000036f0: 696e 7428 7365 6c66 2920 2d3e 2069 6e74  int(self) -> int
+00003700: 3a0d 0a20 2020 2020 2020 2072 2222 220d  :..        r""".
+00003710: 0a20 2020 2020 2020 204c 6f61 6420 6c61  .        Load la
+00003720: 7374 2073 6176 6564 2063 6865 636b 706f  st saved checkpo
+00003730: 696e 742e 0d0a 0d0a 2020 2020 2020 2020  int.....        
+00003740: 5265 7475 726e 733a 0d0a 2020 2020 2020  Returns:..      
+00003750: 2020 2d2d 2d2d 2d2d 2d2d 0d0a 2020 2020    --------..    
+00003760: 2020 2020 6570 6f63 683a 2069 6e74 200d      epoch: int .
+00003770: 0a20 2020 2020 2020 2020 2020 2054 6865  .            The
+00003780: 2065 706f 6368 206e 756d 6265 7220 6c6f   epoch number lo
+00003790: 6164 6564 2066 726f 6d20 7468 6520 6368  aded from the ch
+000037a0: 6563 6b70 6f69 6e74 2e0d 0a20 2020 2020  eckpoint...     
+000037b0: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
+000037c0: 7061 7468 203d 206f 732e 7061 7468 2e6a  path = os.path.j
+000037d0: 6f69 6e28 7365 6c66 2e63 6667 2e43 4845  oin(self.cfg.CHE
+000037e0: 434b 504f 494e 545f 5041 5448 2c20 7365  CKPOINT_PATH, se
+000037f0: 6c66 2e63 6667 2e43 4845 434b 504f 494e  lf.cfg.CHECKPOIN
+00003800: 545f 4649 4c45 4e41 4d45 290d 0a20 2020  T_FILENAME)..   
+00003810: 2020 2020 2063 6865 636b 706f 696e 7420       checkpoint 
+00003820: 3d20 746f 7263 682e 6c6f 6164 2870 6174  = torch.load(pat
+00003830: 6829 0d0a 2020 2020 2020 2020 666f 7220  h)..        for 
+00003840: 6d6f 6475 6c65 2069 6e20 7365 6c66 2e63  module in self.c
+00003850: 6667 2e43 4845 434b 504f 494e 545f 4d4f  fg.CHECKPOINT_MO
+00003860: 4455 4c45 533a 0d0a 2020 2020 2020 2020  DULES:..        
+00003870: 2020 2020 6765 7461 7474 7228 7365 6c66      getattr(self
+00003880: 2c20 6d6f 6475 6c65 292e 6c6f 6164 5f73  , module).load_s
+00003890: 7461 7465 5f64 6963 7428 6368 6563 6b70  tate_dict(checkp
+000038a0: 6f69 6e74 5b6d 6f64 756c 655d 290d 0a20  oint[module]).. 
+000038b0: 2020 2020 2020 2073 656c 662e 6d6f 6e69         self.moni
+000038c0: 746f 7273 2e6c 6f61 645f 7374 6174 655f  tors.load_state_
+000038d0: 6469 6374 2863 6865 636b 706f 696e 745b  dict(checkpoint[
+000038e0: 276d 6f6e 6974 6f72 7327 5d29 0d0a 2020  'monitors'])..  
+000038f0: 2020 2020 2020 7265 7475 726e 2063 6865        return che
+00003900: 636b 706f 696e 745b 2765 706f 6368 275d  ckpoint['epoch']
+00003910: 0d0a 0d0a 2020 2020 6465 6620 7361 7665  ....    def save
+00003920: 5f62 6573 7428 7365 6c66 2920 2d3e 204e  _best(self) -> N
+00003930: 6f6e 653a 0d0a 2020 2020 2020 2020 746f  one:..        to
+00003940: 7263 682e 7361 7665 2873 656c 662e 6d6f  rch.save(self.mo
+00003950: 6465 6c2e 7374 6174 655f 6469 6374 2829  del.state_dict()
+00003960: 2c20 6f73 2e70 6174 682e 6a6f 696e 2873  , os.path.join(s
+00003970: 656c 662e 6366 672e 4c4f 475f 5041 5448  elf.cfg.LOG_PATH
+00003980: 2c20 7365 6c66 2e63 6667 2e42 4553 545f  , self.cfg.BEST_
+00003990: 4649 4c45 4e41 4d45 2929 0d0a 0d0a 2020  FILENAME))....  
+000039a0: 2020 6465 6620 6c6f 6164 5f62 6573 7428    def load_best(
+000039b0: 7365 6c66 2920 2d3e 204e 6f6e 653a 0d0a  self) -> None:..
+000039c0: 2020 2020 2020 2020 696e 666f 4c6f 6767          infoLogg
+000039d0: 6572 2866 225b 436f 6163 685d 203e 3e3e  er(f"[Coach] >>>
+000039e0: 204c 6f61 6420 6265 7374 206d 6f64 656c   Load best model
+000039f0: 2040 4570 6f63 6820 7b73 656c 662e 5f62   @Epoch {self._b
+00003a00: 6573 745f 6570 6f63 683a 3c34 647d 2022  est_epoch:<4d} "
+00003a10: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00003a20: 6d6f 6465 6c2e 6c6f 6164 5f73 7461 7465  model.load_state
+00003a30: 5f64 6963 7428 746f 7263 682e 6c6f 6164  _dict(torch.load
+00003a40: 286f 732e 7061 7468 2e6a 6f69 6e28 7365  (os.path.join(se
+00003a50: 6c66 2e63 6667 2e4c 4f47 5f50 4154 482c  lf.cfg.LOG_PATH,
+00003a60: 2073 656c 662e 6366 672e 4245 5354 5f46   self.cfg.BEST_F
+00003a70: 494c 454e 414d 4529 2929 0d0a 0d0a 2020  ILENAME)))....  
+00003a80: 2020 6465 6620 6368 6563 6b5f 6265 7374    def check_best
+00003a90: 2873 656c 662c 2065 706f 6368 3a20 696e  (self, epoch: in
+00003aa0: 7429 202d 3e20 4e6f 6e65 3a0d 0a20 2020  t) -> None:..   
+00003ab0: 2020 2020 2022 2222 5570 6461 7465 2062       """Update b
+00003ac0: 6573 7420 7661 6c75 652e 2222 220d 0a20  est value.""".. 
+00003ad0: 2020 2020 2020 2069 6620 7365 6c66 2e6d         if self.m
+00003ae0: 6574 6572 3462 6573 742e 6163 7469 7665  eter4best.active
+00003af0: 3a0d 0a20 2020 2020 2020 2020 2020 2062  :..            b
+00003b00: 6573 745f 203d 2073 656c 662e 6d65 7465  est_ = self.mete
+00003b10: 7234 6265 7374 2e77 6869 6368 5f69 735f  r4best.which_is_
+00003b20: 6265 7474 6572 2873 656c 662e 5f62 6573  better(self._bes
+00003b30: 7429 0d0a 2020 2020 2020 2020 2020 2020  t)..            
+00003b40: 6966 2062 6573 745f 2021 3d20 7365 6c66  if best_ != self
+00003b50: 2e5f 6265 7374 3a0d 0a20 2020 2020 2020  ._best:..       
+00003b60: 2020 2020 2020 2020 2073 656c 662e 5f62           self._b
+00003b70: 6573 7420 3d20 6265 7374 5f0d 0a20 2020  est = best_..   
+00003b80: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00003b90: 662e 5f62 6573 745f 6570 6f63 6820 3d20  f._best_epoch = 
+00003ba0: 6570 6f63 680d 0a20 2020 2020 2020 2020  epoch..         
+00003bb0: 2020 2020 2020 2069 6e66 6f4c 6f67 6765         infoLogge
+00003bc0: 7228 6622 5b43 6f61 6368 5d20 3e3e 3e20  r(f"[Coach] >>> 
+00003bd0: 4265 7474 6572 202a 2a2a 7b73 656c 662e  Better ***{self.
+00003be0: 6d65 7465 7234 6265 7374 2e6e 616d 657d  meter4best.name}
+00003bf0: 2a2a 2a20 6f66 202a 2a2a 7b73 656c 662e  *** of ***{self.
+00003c00: 5f62 6573 743a 2e34 667d 2a2a 2a20 2229  _best:.4f}*** ")
+00003c10: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00003c20: 2020 7365 6c66 2e73 6176 655f 6265 7374    self.save_best
+00003c30: 2829 0d0a 0d0a 2020 2020 6465 6620 6576  ()....    def ev
+00003c40: 616c 5f61 745f 6265 7374 2873 656c 6629  al_at_best(self)
+00003c50: 3a0d 0a20 2020 2020 2020 2074 7279 3a0d  :..        try:.
+00003c60: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00003c70: 662e 6c6f 6164 5f62 6573 7428 290d 0a20  f.load_best().. 
+00003c80: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00003c90: 7661 6c69 6428 7365 6c66 2e5f 6265 7374  valid(self._best
+00003ca0: 5f65 706f 6368 290d 0a20 2020 2020 2020  _epoch)..       
+00003cb0: 2020 2020 2073 656c 662e 7465 7374 2873       self.test(s
+00003cc0: 656c 662e 5f62 6573 745f 6570 6f63 6829  elf._best_epoch)
+00003cd0: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+00003ce0: 6c66 2e73 7465 7028 7365 6c66 2e5f 6265  lf.step(self._be
+00003cf0: 7374 5f65 706f 6368 290d 0a20 2020 2020  st_epoch)..     
+00003d00: 2020 2020 2020 2073 656c 662e 6c6f 6164         self.load
+00003d10: 2873 656c 662e 6366 672e 4c4f 475f 5041  (self.cfg.LOG_PA
+00003d20: 5448 2c20 7365 6c66 2e63 6667 2e53 4156  TH, self.cfg.SAV
+00003d30: 4544 5f46 494c 454e 414d 4529 0d0a 2020  ED_FILENAME)..  
+00003d40: 2020 2020 2020 6578 6365 7074 2046 696c        except Fil
+00003d50: 654e 6f74 466f 756e 6445 7272 6f72 3a0d  eNotFoundError:.
+00003d60: 0a20 2020 2020 2020 2020 2020 2069 6e66  .            inf
+00003d70: 6f4c 6f67 6765 7228 6622 5b43 6f61 6368  oLogger(f"[Coach
+00003d80: 5d20 3e3e 3e20 4e6f 2062 6573 7420 6d6f  ] >>> No best mo
+00003d90: 6465 6c20 7761 7320 7265 636f 7264 6564  del was recorded
+00003da0: 2e20 536b 6970 2069 7420 2e2e 2e22 290d  . Skip it ...").
+00003db0: 0a0d 0a20 2020 2064 6566 2072 6573 756d  ...    def resum
+00003dc0: 6528 7365 6c66 2920 2d3e 2069 6e74 3a0d  e(self) -> int:.
+00003dd0: 0a20 2020 2020 2020 2072 2222 220d 0a20  .        r""".. 
+00003de0: 2020 2020 2020 2052 6573 756d 6520 7472         Resume tr
+00003df0: 6169 6e69 6e67 2066 726f 6d20 7468 6520  aining from the 
+00003e00: 6c61 7374 2063 6865 636b 706f 696e 742e  last checkpoint.
+00003e10: 0d0a 0d0a 2020 2020 2020 2020 5265 7475  ....        Retu
+00003e20: 726e 733a 0d0a 2020 2020 2020 2020 2d2d  rns:..        --
+00003e30: 2d2d 2d2d 2d2d 0d0a 2020 2020 2020 2020  ------..        
+00003e40: 7374 6172 745f 6570 6f63 683a 2069 6e74  start_epoch: int
+00003e50: 0d0a 2020 2020 2020 2020 2020 2020 5468  ..            Th
+00003e60: 6520 6570 6f63 6820 6e75 6d62 6572 2074  e epoch number t
+00003e70: 6f20 7265 7375 6d65 2074 7261 696e 696e  o resume trainin
+00003e80: 6720 6672 6f6d 2e0d 0a20 2020 2020 2020  g from...       
+00003e90: 2022 2222 0d0a 2020 2020 2020 2020 7374   """..        st
+00003ea0: 6172 745f 6570 6f63 683a 2069 6e74 203d  art_epoch: int =
+00003eb0: 2030 0d0a 2020 2020 2020 2020 6966 2073   0..        if s
+00003ec0: 656c 662e 6366 672e 7265 7375 6d65 3a0d  elf.cfg.resume:.
+00003ed0: 0a20 2020 2020 2020 2020 2020 2073 7461  .            sta
+00003ee0: 7274 5f65 706f 6368 203d 2073 656c 662e  rt_epoch = self.
+00003ef0: 6c6f 6164 5f63 6865 636b 706f 696e 7428  load_checkpoint(
+00003f00: 290d 0a20 2020 2020 2020 2020 2020 2069  )..            i
+00003f10: 6e66 6f4c 6f67 6765 7228 6622 5b43 6f61  nfoLogger(f"[Coa
+00003f20: 6368 5d20 3e3e 3e20 4c6f 6164 206c 6173  ch] >>> Load las
+00003f30: 7420 6368 6563 6b70 6f69 6e74 2061 6e64  t checkpoint and
+00003f40: 2074 7261 696e 2066 726f 6d20 6570 6f63   train from epoc
+00003f50: 683a 207b 7374 6172 745f 6570 6f63 687d  h: {start_epoch}
+00003f60: 2229 0d0a 2020 2020 2020 2020 7265 7475  ")..        retu
+00003f70: 726e 2073 7461 7274 5f65 706f 6368 0d0a  rn start_epoch..
+00003f80: 0d0a 2020 2020 4074 6f72 6368 2e6e 6f5f  ..    @torch.no_
+00003f90: 6772 6164 2829 0d0a 2020 2020 6465 6620  grad()..    def 
+00003fa0: 6d6f 6e69 746f 7228 0d0a 2020 2020 2020  monitor(..      
+00003fb0: 2020 7365 6c66 2c20 2a76 616c 7565 732c    self, *values,
+00003fc0: 0d0a 2020 2020 2020 2020 6e3a 2069 6e74  ..        n: int
+00003fd0: 203d 2031 2c20 6d6f 6465 3a20 7374 7220   = 1, mode: str 
+00003fe0: 3d20 276d 6561 6e27 2c20 0d0a 2020 2020  = 'mean', ..    
+00003ff0: 2020 2020 7072 6566 6978 3a20 7374 7220      prefix: str 
+00004000: 3d20 2774 7261 696e 272c 2070 6f6f 6c3a  = 'train', pool:
+00004010: 204f 7074 696f 6e61 6c5b 4974 6572 6162   Optional[Iterab
+00004020: 6c65 5d20 3d20 4e6f 6e65 0d0a 2020 2020  le] = None..    
+00004030: 293a 0d0a 0d0a 2020 2020 2020 2020 7222  ):....        r"
+00004040: 2222 0d0a 2020 2020 2020 2020 4c6f 6720  ""..        Log 
+00004050: 6461 7461 2076 616c 7565 7320 746f 2073  data values to s
+00004060: 7065 6369 6669 6320 6d6f 6e69 746f 7273  pecific monitors
+00004070: 2e0d 0a0d 0a20 2020 2020 2020 2050 6172  .....        Par
+00004080: 616d 6574 6572 733a 0d0a 2020 2020 2020  ameters:..      
+00004090: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d0d 0a20    -----------.. 
+000040a0: 2020 2020 2020 202a 7661 6c75 6573 203a         *values :
+000040b0: 2064 6174 610d 0a20 2020 2020 2020 2020   data..         
+000040c0: 2020 2054 6865 2064 6174 6120 7661 6c75     The data valu
+000040d0: 6573 2074 6f20 6265 206c 6f67 6765 642e  es to be logged.
+000040e0: 0d0a 2020 2020 2020 2020 6e20 3a20 696e  ..        n : in
+000040f0: 740d 0a20 2020 2020 2020 2020 2020 2054  t..            T
+00004100: 6865 2062 6174 6368 2073 697a 6520 696e  he batch size in
+00004110: 2067 656e 6572 616c 2e0d 0a20 2020 2020   general...     
+00004120: 2020 206d 6f64 6520 3a20 7374 722c 206f     mode : str, o
+00004130: 7074 696f 6e61 6c0d 0a20 2020 2020 2020  ptional..       
+00004140: 2020 2020 2054 6865 206d 6f64 6520 746f       The mode to
+00004150: 2063 6f6d 7075 7465 2074 6865 206d 6574   compute the met
+00004160: 7269 632e 2043 616e 2062 6520 2773 756d  ric. Can be 'sum
+00004170: 2720 6f72 2027 6d65 616e 2720 2864 6566  ' or 'mean' (def
+00004180: 6175 6c74 292e 0d0a 2020 2020 2020 2020  ault)...        
+00004190: 7072 6566 6978 203a 2073 7472 2c20 6f70  prefix : str, op
+000041a0: 7469 6f6e 616c 0d0a 2020 2020 2020 2020  tional..        
+000041b0: 2020 2020 5468 6520 7072 6566 6978 2073      The prefix s
+000041c0: 7472 696e 6720 696e 6469 6361 7469 6e67  tring indicating
+000041d0: 2077 6869 6368 206d 6f64 6520 7468 6520   which mode the 
+000041e0: 7661 6c75 6573 2062 656c 6f6e 6720 746f  values belong to
+000041f0: 2e20 4361 6e20 6265 2027 7472 6169 6e27  . Can be 'train'
+00004200: 2c20 2774 6573 7427 206f 7220 2776 616c  , 'test' or 'val
+00004210: 6964 272e 0d0a 2020 2020 2020 2020 706f  id'...        po
+00004220: 6f6c 203a 204c 6973 745b 7374 725d 2c20  ol : List[str], 
+00004230: 6f70 7469 6f6e 616c 0d0a 2020 2020 2020  optional..      
+00004240: 2020 2020 2020 4120 6c69 7374 206f 6620        A list of 
+00004250: 6d65 7472 6963 206e 616d 6573 2074 6f20  metric names to 
+00004260: 6c6f 672e 2049 6620 4e6f 6e65 2c20 616c  log. If None, al
+00004270: 6c20 6d65 7472 6963 7320 696e 2074 6865  l metrics in the
+00004280: 2070 6f6f 6c20 6f66 2060 7072 6566 6978   pool of `prefix
+00004290: 6020 7769 6c6c 2062 6520 6c6f 6767 6564  ` will be logged
+000042a0: 2e0d 0a20 2020 2020 2020 2022 2222 0d0a  ...        """..
+000042b0: 0d0a 2020 2020 2020 2020 6d65 7472 6963  ..        metric
+000042c0: 733a 2044 6963 745b 4c69 7374 5d20 3d20  s: Dict[List] = 
+000042d0: 7365 6c66 2e6d 6f6e 6974 6f72 735b 7072  self.monitors[pr
+000042e0: 6566 6978 5d0d 0a20 2020 2020 2020 2070  efix]..        p
+000042f0: 6f6f 6c20 3d20 6d65 7472 6963 7320 6966  ool = metrics if
+00004300: 2070 6f6f 6c20 6973 204e 6f6e 6520 656c   pool is None el
+00004310: 7365 2070 6f6f 6c0d 0a20 2020 2020 2020  se pool..       
+00004320: 2066 6f72 206c 6173 746e 616d 6520 696e   for lastname in
+00004330: 2070 6f6f 6c3a 0d0a 2020 2020 2020 2020   pool:..        
+00004340: 2020 2020 666f 7220 6d65 7465 7220 696e      for meter in
+00004350: 206d 6574 7269 6373 2e67 6574 286c 6173   metrics.get(las
+00004360: 746e 616d 652e 7570 7065 7228 292c 205b  tname.upper(), [
+00004370: 5d29 3a0d 0a20 2020 2020 2020 2020 2020  ]):..           
+00004380: 2020 2020 206d 6574 6572 282a 7661 6c75       meter(*valu
+00004390: 6573 2c20 6e3d 6e2c 206d 6f64 653d 6d6f  es, n=n, mode=mo
+000043a0: 6465 290d 0a0d 0a20 2020 2064 6566 2073  de)....    def s
+000043b0: 7465 7028 7365 6c66 2c20 6570 6f63 683a  tep(self, epoch:
+000043c0: 2069 6e74 293a 0d0a 2020 2020 2020 2020   int):..        
+000043d0: 7222 2222 0d0a 2020 2020 2020 2020 5072  r"""..        Pr
+000043e0: 696e 7473 2074 7261 696e 696e 6720 7374  ints training st
+000043f0: 6174 7573 2061 6e64 2065 7661 6c75 6174  atus and evaluat
+00004400: 696f 6e20 7265 7375 6c74 7320 666f 7220  ion results for 
+00004410: 6561 6368 2065 706f 6368 2c20 0d0a 2020  each epoch, ..  
+00004420: 2020 2020 2020 616e 6420 7265 7365 7473        and resets
+00004430: 2074 6865 2063 6f72 7265 7370 6f6e 6469   the correspondi
+00004440: 6e67 2060 4176 6572 6167 654d 6574 6572  ng `AverageMeter
+00004450: 6020 696e 7374 616e 6365 732e 0d0a 0d0a  ` instances.....
+00004460: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
+00004470: 7273 3a0d 0a20 2020 2020 2020 202d 2d2d  rs:..        ---
+00004480: 2d2d 2d2d 2d2d 2d2d 0d0a 2020 2020 2020  --------..      
+00004490: 2020 6570 6f63 6820 3a20 696e 740d 0a20    epoch : int.. 
+000044a0: 2020 2020 2020 2020 2020 2054 6865 2065             The e
+000044b0: 706f 6368 206e 756d 6265 722e 0d0a 0d0a  poch number.....
+000044c0: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
+000044d0: 0d0a 2020 2020 2020 2020 2d2d 2d2d 2d2d  ..        ------
+000044e0: 2d2d 0d0a 2020 2020 2020 2020 4e6f 6e65  --..        None
+000044f0: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
+00004500: 2020 2020 2020 206d 6574 7269 6373 3a20         metrics: 
+00004510: 4469 6374 5b73 7472 2c20 4c69 7374 5b41  Dict[str, List[A
+00004520: 7665 7261 6765 4d65 7465 725d 5d0d 0a20  verageMeter]].. 
+00004530: 2020 2020 2020 2066 6f72 2070 7265 6669         for prefi
+00004540: 782c 206d 6574 7269 6373 2069 6e20 7365  x, metrics in se
+00004550: 6c66 2e6d 6f6e 6974 6f72 732e 6974 656d  lf.monitors.item
+00004560: 7328 293a 0d0a 2020 2020 2020 2020 2020  s():..          
+00004570: 2020 696e 666f 7320 3d20 5b66 225b 436f    infos = [f"[Co
+00004580: 6163 685d 203e 3e3e 207b 7072 6566 6978  ach] >>> {prefix
+00004590: 2e75 7070 6572 2829 3a35 7d20 4045 706f  .upper():5} @Epo
+000045a0: 6368 3a20 7b65 706f 6368 3a3c 3464 7d20  ch: {epoch:<4d} 
+000045b0: 3e3e 3e20 225d 0d0a 2020 2020 2020 2020  >>> "]..        
+000045c0: 2020 2020 666f 7220 6d65 7465 7273 2069      for meters i
+000045d0: 6e20 6d65 7472 6963 732e 7661 6c75 6573  n metrics.values
+000045e0: 2829 3a0d 0a20 2020 2020 2020 2020 2020  ():..           
+000045f0: 2020 2020 2069 6e66 6f73 202b 3d20 5b6d       infos += [m
+00004600: 6574 6572 2e73 7465 7028 2920 666f 7220  eter.step() for 
+00004610: 6d65 7465 7220 696e 206d 6574 6572 7320  meter in meters 
+00004620: 6966 206d 6574 6572 2e61 6374 6976 655d  if meter.active]
+00004630: 0d0a 2020 2020 2020 2020 2020 2020 696e  ..            in
+00004640: 666f 4c6f 6767 6572 2827 207c 7c20 272e  foLogger(' || '.
+00004650: 6a6f 696e 2869 6e66 6f73 2929 0d0a 0d0a  join(infos))....
+00004660: 2020 2020 4074 696d 656d 6574 6572 2822      @timemeter("
+00004670: 436f 6163 682f 7375 6d6d 6172 7922 290d  Coach/summary").
+00004680: 0a20 2020 2064 6566 2073 756d 6d61 7279  .    def summary
+00004690: 2873 656c 6629 3a0d 0a20 2020 2020 2020  (self):..       
+000046a0: 2072 2222 220d 0a20 2020 2020 2020 2053   r"""..        S
+000046b0: 756d 6d61 7279 2074 6865 2077 686f 6c65  ummary the whole
+000046c0: 2074 7261 696e 696e 6720 7072 6f63 6573   training proces
+000046d0: 732e 0d0a 0d0a 2020 2020 2020 2020 4765  s.....        Ge
+000046e0: 6e65 7261 7465 2061 2073 756d 6d61 7279  nerate a summary
+000046f0: 206f 6620 7468 6520 656e 7469 7265 2074   of the entire t
+00004700: 7261 696e 696e 6720 7072 6f63 6573 732c  raining process,
+00004710: 2069 6e63 6c75 6469 6e67 2074 6865 2068   including the h
+00004720: 6973 746f 7269 6361 6c20 6576 616c 7561  istorical evalua
+00004730: 7469 6f6e 2072 6573 756c 7473 2c20 7468  tion results, th
+00004740: 6520 6265 7374 0d0a 2020 2020 2020 2020  e best..        
+00004750: 6869 7374 6f72 6963 616c 2072 6573 756c  historical resul
+00004760: 7473 2c20 616e 6420 7468 6520 6375 7276  ts, and the curv
+00004770: 6573 206f 6620 6869 7374 6f72 6963 616c  es of historical
+00004780: 2072 6573 756c 7473 2e20 5468 6520 7265   results. The re
+00004790: 7375 6c74 696e 6720 7375 6d6d 6172 7920  sulting summary 
+000047a0: 6973 2073 6176 6564 2074 6f20 6120 4d61  is saved to a Ma
+000047b0: 726b 646f 776e 2066 696c 6520 6e61 6d65  rkdown file name
+000047c0: 640d 0a20 2020 2020 2020 2022 5375 6d6d  d..        "Summ
+000047d0: 6172 792e 6d64 2220 696e 2074 6865 2060  ary.md" in the `
+000047e0: 7365 6c66 2e63 6667 2e4c 4f47 5f50 4154  self.cfg.LOG_PAT
+000047f0: 4860 2064 6972 6563 746f 7279 2e0d 0a0d  H` directory....
+00004800: 0a20 2020 2020 2020 2041 6464 6974 696f  .        Additio
+00004810: 6e61 6c6c 792c 2074 6865 2062 6573 7420  nally, the best 
+00004820: 6869 7374 6f72 6963 616c 2072 6573 756c  historical resul
+00004830: 7473 2061 7265 2073 6176 6564 2074 6f20  ts are saved to 
+00004840: 6120 6269 6e61 7279 2066 696c 6520 6e61  a binary file na
+00004850: 6d65 6420 6073 656c 662e 6366 672e 4d4f  med `self.cfg.MO
+00004860: 4e49 544f 525f 4245 5354 5f46 494c 454e  NITOR_BEST_FILEN
+00004870: 414d 4560 2e0d 0a20 2020 2020 2020 2022  AME`...        "
+00004880: 2222 0d0a 2020 2020 2020 2020 7320 3d20  ""..        s = 
+00004890: 227c 2020 7b70 7265 6669 787d 2020 7c20  "|  {prefix}  | 
+000048a0: 2020 7b6e 616d 657d 2020 207c 2020 207b    {name}   |   {
+000048b0: 7661 6c7d 2020 207c 2020 207b 6570 6f63  val}   |   {epoc
+000048c0: 687d 2020 207c 2020 207b 696d 677d 2020  h}   |   {img}  
+000048d0: 207c 5c6e 220d 0a20 2020 2020 2020 2069   |\n"..        i
+000048e0: 6e66 6f20 3d20 2222 0d0a 2020 2020 2020  nfo = ""..      
+000048f0: 2020 696e 666f 202b 3d20 227c 2020 5072    info += "|  Pr
+00004900: 6566 6978 2020 7c20 2020 4d65 7472 6963  efix  |   Metric
+00004910: 2020 207c 2020 2042 6573 7420 2020 7c20     |   Best   | 
+00004920: 2020 4045 706f 6368 2020 207c 2020 2049    @Epoch   |   I
+00004930: 6d67 2020 207c 5c6e 220d 0a20 2020 2020  mg   |\n"..     
+00004940: 2020 2069 6e66 6f20 2b3d 2022 7c20 3a2d     info += "| :-
+00004950: 2d2d 2d2d 2d2d 3a20 7c20 3a2d 2d2d 2d2d  ------: | :-----
+00004960: 2d2d 3a20 7c20 3a2d 2d2d 2d2d 2d2d 3a20  --: | :-------: 
+00004970: 7c20 3a2d 2d2d 2d2d 2d2d 3a20 7c20 3a2d  | :-------: | :-
+00004980: 2d2d 2d2d 2d2d 3a20 7c5c 6e22 0d0a 2020  ------: |\n"..  
+00004990: 2020 2020 2020 6461 7461 203d 205b 5d0d        data = [].
+000049a0: 0a20 2020 2020 2020 2062 6573 7420 3d20  .        best = 
+000049b0: 6465 6661 756c 7464 6963 7428 6469 6374  defaultdict(dict
+000049c0: 290d 0a0d 0a20 2020 2020 2020 2066 6f72  )....        for
+000049d0: 2070 7265 6669 782c 206d 6574 7269 6373   prefix, metrics
+000049e0: 2069 6e20 7365 6c66 2e6d 6f6e 6974 6f72   in self.monitor
+000049f0: 732e 6974 656d 7328 293a 0d0a 2020 2020  s.items():..    
+00004a00: 2020 2020 2020 2020 6d65 7472 6963 733a          metrics:
+00004a10: 2064 6566 6175 6c74 6469 6374 5b73 7472   defaultdict[str
+00004a20: 2c20 4c69 7374 5b41 7665 7261 6765 4d65  , List[AverageMe
+00004a30: 7465 725d 5d0d 0a20 2020 2020 2020 2020  ter]]..         
+00004a40: 2020 2066 7265 7120 3d20 3120 6966 2070     freq = 1 if p
+00004a50: 7265 6669 7820 3d3d 2027 7472 6169 6e27  refix == 'train'
+00004a60: 2065 6c73 6520 7365 6c66 2e63 6667 2e45   else self.cfg.E
+00004a70: 5641 4c5f 4652 4551 0d0a 2020 2020 2020  VAL_FREQ..      
+00004a80: 2020 2020 2020 666f 7220 6c61 7374 6e61        for lastna
+00004a90: 6d65 2c20 6d65 7465 7273 2069 6e20 6d65  me, meters in me
+00004aa0: 7472 6963 732e 6974 656d 7328 293a 0d0a  trics.items():..
+00004ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004ac0: 666f 7220 6d65 7465 7220 696e 206d 6574  for meter in met
+00004ad0: 6572 733a 0d0a 2020 2020 2020 2020 2020  ers:..          
+00004ae0: 2020 2020 2020 2020 2020 2320 536b 6970            # Skip
+00004af0: 2074 686f 7365 206d 6574 6572 7320 6e65   those meters ne
+00004b00: 7665 7220 6163 7469 7661 7465 642e 0d0a  ver activated...
+00004b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004b20: 2020 2020 6966 206c 656e 286d 6574 6572      if len(meter
+00004b30: 2e68 6973 746f 7279 2920 3d3d 2030 3a0d  .history) == 0:.
+00004b40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004b50: 2020 2020 2020 2020 2063 6f6e 7469 6e75           continu
+00004b60: 650d 0a20 2020 2020 2020 2020 2020 2020  e..             
+00004b70: 2020 2020 2020 206d 6574 6572 2e70 6c6f         meter.plo
+00004b80: 7428 6672 6571 3d66 7265 7129 0d0a 2020  t(freq=freq)..  
+00004b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004ba0: 2020 696d 676e 616d 6520 3d20 6d65 7465    imgname = mete
+00004bb0: 722e 7361 7665 2870 6174 683d 6f73 2e70  r.save(path=os.p
+00004bc0: 6174 682e 6a6f 696e 2873 656c 662e 6366  ath.join(self.cf
+00004bd0: 672e 4c4f 475f 5041 5448 2c20 7365 6c66  g.LOG_PATH, self
+00004be0: 2e63 6667 2e53 554d 4d41 5259 5f44 4952  .cfg.SUMMARY_DIR
+00004bf0: 292c 2070 7265 6669 783d 7072 6566 6978  ), prefix=prefix
+00004c00: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00004c10: 2020 2020 2020 2065 706f 6368 2c20 7661         epoch, va
+00004c20: 6c20 3d20 6d65 7465 722e 6172 6762 6573  l = meter.argbes
+00004c30: 7428 6672 6571 290d 0a20 2020 2020 2020  t(freq)..       
+00004c40: 2020 2020 2020 2020 2020 2020 2069 6e66               inf
+00004c50: 6f20 2b3d 2073 2e66 6f72 6d61 7428 0d0a  o += s.format(..
 00004c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004c70: 2076 616c 3d76 616c 2c20 6570 6f63 683d   val=val, epoch=
-00004c80: 6570 6f63 682c 2069 6d67 3d66 2221 5b5d  epoch, img=f"![]
-00004c90: 287b 696d 676e 616d 657d 2922 0d0a 2020  ({imgname})"..  
+00004c70: 2020 2020 2020 2020 7072 6566 6978 3d70          prefix=p
+00004c80: 7265 6669 782c 206e 616d 653d 6d65 7465  refix, name=mete
+00004c90: 722e 6e61 6d65 2c0d 0a20 2020 2020 2020  r.name,..       
 00004ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004cb0: 2020 290d 0a20 2020 2020 2020 2020 2020    )..           
-00004cc0: 2020 2020 2020 2020 2064 6174 612e 6170           data.ap
-00004cd0: 7065 6e64 285b 7072 6566 6978 2c20 6d65  pend([prefix, me
-00004ce0: 7465 722e 6e61 6d65 2c20 7661 6c2c 2065  ter.name, val, e
-00004cf0: 706f 6368 5d29 0d0a 2020 2020 2020 2020  poch])..        
-00004d00: 2020 2020 2020 2020 2020 2020 6966 2076              if v
-00004d10: 616c 2021 3d20 2d31 3a20 2320 4f6e 6c79  al != -1: # Only
-00004d20: 2073 6176 6520 6176 6169 6c61 626c 6520   save available 
-00004d30: 6461 7461 2e0d 0a20 2020 2020 2020 2020  data...         
-00004d40: 2020 2020 2020 2020 2020 2020 2020 2062                 b
-00004d50: 6573 745b 7072 6566 6978 5d5b 6d65 7465  est[prefix][mete
-00004d60: 722e 6e61 6d65 5d20 3d20 7661 6c0d 0a0d  r.name] = val...
-00004d70: 0a20 2020 2020 2020 2066 696c 655f 203d  .        file_ =
-00004d80: 206f 732e 7061 7468 2e6a 6f69 6e28 7365   os.path.join(se
-00004d90: 6c66 2e63 6667 2e4c 4f47 5f50 4154 482c  lf.cfg.LOG_PATH,
-00004da0: 2073 656c 662e 6366 672e 5355 4d4d 4152   self.cfg.SUMMAR
-00004db0: 595f 4449 522c 2073 656c 662e 6366 672e  Y_DIR, self.cfg.
-00004dc0: 5355 4d4d 4152 595f 4649 4c45 4e41 4d45  SUMMARY_FILENAME
-00004dd0: 290d 0a20 2020 2020 2020 2077 6974 6820  )..        with 
-00004de0: 6f70 656e 2866 696c 655f 2c20 2277 222c  open(file_, "w",
-00004df0: 2065 6e63 6f64 696e 673d 2275 7466 3822   encoding="utf8"
-00004e00: 2920 6173 2066 683a 0d0a 2020 2020 2020  ) as fh:..      
-00004e10: 2020 2020 2020 6668 2e77 7269 7465 2869        fh.write(i
-00004e20: 6e66 6f29 0d0a 0d0a 2020 2020 2020 2020  nfo)....        
-00004e30: 6466 203d 2070 642e 4461 7461 4672 616d  df = pd.DataFram
-00004e40: 6528 6461 7461 2c20 636f 6c75 6d6e 733d  e(data, columns=
-00004e50: 5b27 5072 6566 6978 272c 2027 4d65 7472  ['Prefix', 'Metr
-00004e60: 6963 272c 2027 4265 7374 272c 2027 4045  ic', 'Best', '@E
-00004e70: 706f 6368 275d 290d 0a20 2020 2020 2020  poch'])..       
-00004e80: 2069 6e66 6f4c 6f67 6765 7228 7374 7228   infoLogger(str(
-00004e90: 6466 2929 0d0a 2020 2020 2020 2020 696e  df))..        in
-00004ea0: 666f 4c6f 6767 6572 2866 225b 4c6f 475f  foLogger(f"[LoG_
-00004eb0: 5061 5448 5d20 3e3e 3e20 7b73 656c 662e  PaTH] >>> {self.
-00004ec0: 6366 672e 4c4f 475f 5041 5448 7d22 290d  cfg.LOG_PATH}").
-00004ed0: 0a0d 0a20 2020 2020 2020 2073 656c 662e  ...        self.
-00004ee0: 6d6f 6e69 746f 7273 2e77 7269 7465 286f  monitors.write(o
-00004ef0: 732e 7061 7468 2e6a 6f69 6e28 7365 6c66  s.path.join(self
-00004f00: 2e63 6667 2e4c 4f47 5f50 4154 482c 2073  .cfg.LOG_PATH, s
-00004f10: 656c 662e 6366 672e 5355 4d4d 4152 595f  elf.cfg.SUMMARY_
-00004f20: 4449 5229 2920 2320 7465 6e73 6f72 626f  DIR)) # tensorbo
-00004f30: 6172 640d 0a0d 0a20 2020 2020 2020 2073  ard....        s
-00004f40: 656c 662e 6d6f 6e69 746f 7273 2e73 6176  elf.monitors.sav
-00004f50: 6528 6f73 2e70 6174 682e 6a6f 696e 2873  e(os.path.join(s
-00004f60: 656c 662e 6366 672e 4c4f 475f 5041 5448  elf.cfg.LOG_PATH
-00004f70: 2c20 7365 6c66 2e63 6667 2e44 4154 415f  , self.cfg.DATA_
-00004f80: 4449 5229 2c20 7365 6c66 2e63 6667 2e4d  DIR), self.cfg.M
-00004f90: 4f4e 4954 4f52 5f46 494c 454e 414d 4529  ONITOR_FILENAME)
-00004fa0: 0d0a 2020 2020 2020 2020 6578 706f 7274  ..        export
-00004fb0: 5f70 6963 6b6c 6528 6265 7374 2c20 6f73  _pickle(best, os
-00004fc0: 2e70 6174 682e 6a6f 696e 2873 656c 662e  .path.join(self.
-00004fd0: 6366 672e 4c4f 475f 5041 5448 2c20 7365  cfg.LOG_PATH, se
-00004fe0: 6c66 2e63 6667 2e44 4154 415f 4449 522c  lf.cfg.DATA_DIR,
-00004ff0: 2073 656c 662e 6366 672e 4d4f 4e49 544f   self.cfg.MONITO
-00005000: 525f 4245 5354 5f46 494c 454e 414d 4529  R_BEST_FILENAME)
-00005010: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
-00005020: 200d 0a20 2020 2040 7469 6d65 6d65 7465   ..    @timemete
-00005030: 7228 2243 6f61 6368 2f66 6974 2229 0d0a  r("Coach/fit")..
-00005040: 2020 2020 6465 6620 6669 7428 7365 6c66      def fit(self
-00005050: 293a 0d0a 0d0a 2020 2020 2020 2020 6465  ):....        de
-00005060: 6620 7369 676e 616c 5f68 616e 646c 6572  f signal_handler
-00005070: 2873 6967 2c20 6672 616d 6529 3a0d 0a20  (sig, frame):.. 
-00005080: 2020 2020 2020 2020 2020 2069 6e66 6f4c             infoL
-00005090: 6f67 6765 7228 6622 5c30 3333 5b30 3b33  ogger(f"\033[0;3
-000050a0: 313b 3437 6d3d 3d3d 3d3d 3d3d 3d3d 3d3d  1;47m===========
-000050b0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000050c0: 3d3d 3d3d 5445 524d 494e 4154 4520 4355  ====TERMINATE CU
-000050d0: 5252 454e 5420 5052 4f43 4553 533d 3d3d  RRENT PROCESS===
-000050e0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000050f0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 5c30 3333  ============\033
-00005100: 5b30 6d22 290d 0a20 2020 2020 2020 2020  [0m")..         
-00005110: 2020 2073 7973 2e65 7869 7428 290d 0a20     sys.exit().. 
-00005120: 2020 2020 2020 2073 6967 6e61 6c2e 7369         signal.si
-00005130: 676e 616c 2873 6967 6e61 6c2e 5349 4749  gnal(signal.SIGI
-00005140: 4e54 2c20 7369 676e 616c 5f68 616e 646c  NT, signal_handl
-00005150: 6572 290d 0a0d 0a20 2020 2020 2020 2073  er)....        s
-00005160: 7461 7274 5f65 706f 6368 203d 2073 656c  tart_epoch = sel
-00005170: 662e 7265 7375 6d65 2829 0d0a 2020 2020  f.resume()..    
-00005180: 2020 2020 666f 7220 6570 6f63 6820 696e      for epoch in
-00005190: 2072 616e 6765 2873 7461 7274 5f65 706f   range(start_epo
-000051a0: 6368 2c20 7365 6c66 2e63 6667 2e65 706f  ch, self.cfg.epo
-000051b0: 6368 7329 3a0d 0a20 2020 2020 2020 2020  chs):..         
-000051c0: 2020 2069 6620 6570 6f63 6820 2520 7365     if epoch % se
-000051d0: 6c66 2e63 6667 2e43 4845 434b 504f 494e  lf.cfg.CHECKPOIN
-000051e0: 545f 4652 4551 203d 3d20 303a 0d0a 2020  T_FREQ == 0:..  
-000051f0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00005200: 6c66 2e73 6176 655f 6368 6563 6b70 6f69  lf.save_checkpoi
-00005210: 6e74 2865 706f 6368 290d 0a20 2020 2020  nt(epoch)..     
-00005220: 2020 2020 2020 2069 6620 6570 6f63 6820         if epoch 
-00005230: 2520 7365 6c66 2e63 6667 2e45 5641 4c5f  % self.cfg.EVAL_
-00005240: 4652 4551 203d 3d20 303a 0d0a 2020 2020  FREQ == 0:..    
-00005250: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-00005260: 656c 662e 6366 672e 4556 414c 5f56 414c  elf.cfg.EVAL_VAL
-00005270: 4944 3a0d 0a20 2020 2020 2020 2020 2020  ID:..           
-00005280: 2020 2020 2020 2020 2073 656c 662e 7661           self.va
-00005290: 6c69 6428 6570 6f63 6829 0d0a 2020 2020  lid(epoch)..    
-000052a0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-000052b0: 656c 662e 6366 672e 4556 414c 5f54 4553  elf.cfg.EVAL_TES
-000052c0: 543a 0d0a 2020 2020 2020 2020 2020 2020  T:..            
-000052d0: 2020 2020 2020 2020 7365 6c66 2e74 6573          self.tes
-000052e0: 7428 6570 6f63 6829 0d0a 2020 2020 2020  t(epoch)..      
-000052f0: 2020 2020 2020 7365 6c66 2e63 6865 636b        self.check
-00005300: 5f62 6573 7428 6570 6f63 6829 0d0a 2020  _best(epoch)..  
-00005310: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
-00005320: 7465 7028 6570 6f63 6829 0d0a 2020 2020  tep(epoch)..    
-00005330: 2020 2020 2020 2020 7365 6c66 2e74 7261          self.tra
-00005340: 696e 2865 706f 6368 290d 0a0d 0a20 2020  in(epoch)....   
-00005350: 2020 2020 2073 656c 662e 7361 7665 2829       self.save()
-00005360: 0d0a 0d0a 2020 2020 2020 2020 2320 6c61  ....        # la
-00005370: 7374 2065 706f 6368 0d0a 2020 2020 2020  st epoch..      
-00005380: 2020 7365 6c66 2e76 616c 6964 2873 656c    self.valid(sel
-00005390: 662e 6366 672e 6570 6f63 6873 290d 0a20  f.cfg.epochs).. 
-000053a0: 2020 2020 2020 2073 656c 662e 7465 7374         self.test
-000053b0: 2873 656c 662e 6366 672e 6570 6f63 6873  (self.cfg.epochs
-000053c0: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-000053d0: 6368 6563 6b5f 6265 7374 2873 656c 662e  check_best(self.
-000053e0: 6366 672e 6570 6f63 6873 290d 0a20 2020  cfg.epochs)..   
-000053f0: 2020 2020 2073 656c 662e 7374 6570 2873       self.step(s
-00005400: 656c 662e 6366 672e 6570 6f63 6873 290d  elf.cfg.epochs).
-00005410: 0a0d 0a20 2020 2020 2020 2073 656c 662e  ...        self.
-00005420: 7375 6d6d 6172 7928 290d 0a0d 0a20 2020  summary()....   
-00005430: 2020 2020 2073 656c 662e 6576 616c 5f61       self.eval_a
-00005440: 745f 6265 7374 2829 0d0a 0d0a 0d0a 636c  t_best()......cl
-00005450: 6173 7320 4164 6170 7465 723a 0d0a 2020  ass Adapter:..  
-00005460: 2020 7222 2222 0d0a 2020 2020 5061 7261    r"""..    Para
-00005470: 6d73 2074 756e 6572 2e0d 0a0d 0a20 2020  ms tuner.....   
-00005480: 2046 6c6f 7773 3a0d 0a20 2020 202d 2d2d   Flows:..    ---
-00005490: 2d2d 2d0d 0a20 2020 2031 2e20 636f 6d70  ---..    1. comp
-000054a0: 696c 653a 2063 6f6e 6669 6775 7265 2074  ile: configure t
-000054b0: 6865 2063 6f6d 6d61 6e64 2c20 656e 7669  he command, envi
-000054c0: 726f 6e6d 656e 7473 2c20 616e 6420 7061  ronments, and pa
-000054d0: 7261 6d65 7465 7273 2066 6f72 2074 7261  rameters for tra
-000054e0: 696e 696e 672e 0d0a 2020 2020 322e 2061  ining...    2. a
-000054f0: 6c6c 6f63 6174 6520 6465 7669 6365 7320  llocate devices 
-00005500: 666f 7220 7661 7269 6f75 7320 7061 7261  for various para
-00005510: 6d65 7465 7273 3a0d 0a20 2020 2020 2020  meters:..       
-00005520: 202d 2072 6567 6973 7465 7220 7468 6520   - register the 
-00005530: 4944 2c20 6c6f 6720 7061 7468 2c20 616e  ID, log path, an
-00005540: 6420 6465 7669 6365 2066 6972 7374 0d0a  d device first..
-00005550: 2020 2020 2020 2020 2d20 6578 6563 7574          - execut
-00005560: 6520 7468 6520 636f 6d6d 616e 640d 0a20  e the command.. 
-00005570: 2020 2020 2020 202d 2063 6f6c 6c65 6374         - collect
-00005580: 2069 6e66 6f72 6d61 7469 6f6e 2066 726f   information fro
-00005590: 6d20 7468 6520 6c6f 6720 7061 7468 2061  m the log path a
-000055a0: 6e64 206f 7574 7075 7420 746f 2054 656e  nd output to Ten
-000055b0: 736f 7242 6f61 7264 0d0a 2020 2020 2020  sorBoard..      
-000055c0: 2020 2d20 7361 7665 2074 6865 2063 6865    - save the che
-000055d0: 636b 706f 696e 740d 0a20 2020 2020 2020  ckpoint..       
-000055e0: 202d 2072 656c 6561 7365 2074 6865 2063   - release the c
-000055f0: 6f72 7265 7370 6f6e 6469 6e67 2064 6576  orresponding dev
-00005600: 6963 650d 0a0d 0a20 2020 2045 7861 6d70  ice....    Examp
-00005610: 6c65 733a 0d0a 2020 2020 2d2d 2d2d 2d2d  les:..    ------
-00005620: 2d2d 2d0d 0a20 2020 203e 3e3e 2063 6667  ---..    >>> cfg
-00005630: 203d 207b 2763 6f6d 6d61 6e64 273a 2027   = {'command': '
-00005640: 7079 7468 6f6e 2078 7878 2e70 7927 2c20  python xxx.py', 
-00005650: 2770 6172 616d 7327 3a20 7b27 6f70 7469  'params': {'opti
-00005660: 6d69 7a65 7227 3a20 5b27 7367 6427 2c20  mizer': ['sgd', 
-00005670: 2761 6461 6d27 5d7d 7d0d 0a20 2020 203e  'adam']}}..    >
-00005680: 3e3e 2074 756e 6572 203d 2041 6461 7074  >> tuner = Adapt
-00005690: 6572 2829 0d0a 2020 2020 3e3e 3e20 7475  er()..    >>> tu
-000056a0: 6e65 722e 636f 6d70 696c 6528 6366 6729  ner.compile(cfg)
-000056b0: 0d0a 2020 2020 3e3e 3e20 7475 6e65 722e  ..    >>> tuner.
-000056c0: 6669 7428 290d 0a20 2020 2022 2222 0d0a  fit()..    """..
-000056d0: 0d0a 2020 2020 6465 6620 5f5f 696e 6974  ..    def __init
-000056e0: 5f5f 2873 656c 6629 202d 3e20 4e6f 6e65  __(self) -> None
-000056f0: 3a0d 0a20 2020 2020 2020 2073 656c 662e  :..        self.
-00005700: 7061 7261 6d73 203d 205b 5d0d 0a20 2020  params = []..   
-00005710: 2020 2020 2073 656c 662e 7661 6c75 6573       self.values
-00005720: 203d 205b 5d0d 0a20 2020 2020 2020 2073   = []..        s
-00005730: 656c 662e 6465 7669 6365 7320 3d20 5b5d  elf.devices = []
-00005740: 0d0a 0d0a 2020 2020 2020 2020 6465 6620  ....        def 
-00005750: 636c 6561 6e28 293a 0d0a 2020 2020 2020  clean():..      
-00005760: 2020 2020 2020 7061 7265 6e74 203d 2070        parent = p
-00005770: 7375 7469 6c2e 5072 6f63 6573 7328 6f73  sutil.Process(os
-00005780: 2e67 6574 7069 6428 2929 0d0a 2020 2020  .getpid())..    
-00005790: 2020 2020 2020 2020 6368 696c 6472 656e          children
-000057a0: 203d 2070 6172 656e 742e 6368 696c 6472   = parent.childr
-000057b0: 656e 2872 6563 7572 7369 7665 3d54 7275  en(recursive=Tru
-000057c0: 6529 0d0a 2020 2020 2020 2020 2020 2020  e)..            
-000057d0: 666f 7220 7072 6f63 6573 7320 696e 2063  for process in c
-000057e0: 6869 6c64 7265 6e3a 0d0a 2020 2020 2020  hildren:..      
-000057f0: 2020 2020 2020 2020 2020 7072 6f63 6573            proces
-00005800: 732e 7365 6e64 5f73 6967 6e61 6c28 7369  s.send_signal(si
-00005810: 676e 616c 2e53 4947 5445 524d 290d 0a20  gnal.SIGTERM).. 
-00005820: 2020 2020 2020 2020 2020 2070 7375 7469             psuti
-00005830: 6c2e 7761 6974 5f70 726f 6373 2863 6869  l.wait_procs(chi
-00005840: 6c64 7265 6e2c 2074 696d 656f 7574 3d35  ldren, timeout=5
-00005850: 290d 0a0d 0a20 2020 2020 2020 2061 7465  )....        ate
-00005860: 7869 742e 7265 6769 7374 6572 2863 6c65  xit.register(cle
-00005870: 616e 290d 0a0d 0a20 2020 2040 7072 6f70  an)....    @prop
-00005880: 6572 7479 0d0a 2020 2020 6465 6620 434f  erty..    def CO
-00005890: 4d4d 414e 4428 7365 6c66 293a 0d0a 2020  MMAND(self):..  
-000058a0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-000058b0: 662e 6366 672e 434f 4d4d 414e 440d 0a0d  f.cfg.COMMAND...
-000058c0: 0a20 2020 2064 6566 2072 6567 6973 7465  .    def registe
-000058d0: 7228 7365 6c66 2c20 6465 7669 6365 3a20  r(self, device: 
-000058e0: 7374 7229 202d 3e20 5475 706c 655b 7374  str) -> Tuple[st
-000058f0: 722c 2073 7472 5d3a 0d0a 2020 2020 2020  r, str]:..      
-00005900: 2020 7365 6c66 2e63 6667 2e45 4e56 535b    self.cfg.ENVS[
-00005910: 2769 6427 5d20 3d20 7469 6d65 2e73 7472  'id'] = time.str
-00005920: 6674 696d 6528 5449 4d45 290d 0a20 2020  ftime(TIME)..   
-00005930: 2020 2020 2073 656c 662e 6366 672e 454e       self.cfg.EN
-00005940: 5653 5b27 6465 7669 6365 275d 203d 2064  VS['device'] = d
-00005950: 6576 6963 650d 0a20 2020 2020 2020 2063  evice..        c
-00005960: 6f6d 6d61 6e64 203d 2073 656c 662e 434f  ommand = self.CO
-00005970: 4d4d 414e 4420 2b20 7365 6c66 2e67 6574  MMAND + self.get
-00005980: 5f6f 7074 696f 6e28 2769 6427 2c20 7365  _option('id', se
-00005990: 6c66 2e63 6667 2e45 4e56 532e 6964 290d  lf.cfg.ENVS.id).
-000059a0: 0a20 2020 2020 2020 2063 6f6d 6d61 6e64  .        command
-000059b0: 202b 3d20 7365 6c66 2e67 6574 5f6f 7074   += self.get_opt
-000059c0: 696f 6e28 2764 6576 6963 6527 2c20 7365  ion('device', se
-000059d0: 6c66 2e63 6667 2e45 4e56 532e 6465 7669  lf.cfg.ENVS.devi
-000059e0: 6365 290d 0a20 2020 2020 2020 2072 6574  ce)..        ret
-000059f0: 7572 6e20 636f 6d6d 616e 642c 2073 656c  urn command, sel
-00005a00: 662e 6366 672e 454e 5653 2e69 642c 2073  f.cfg.ENVS.id, s
-00005a10: 656c 662e 6366 672e 4c4f 475f 5041 5448  elf.cfg.LOG_PATH
-00005a20: 2e66 6f72 6d61 7428 2a2a 7365 6c66 2e63  .format(**self.c
-00005a30: 6667 2e45 4e56 5329 0d0a 0d0a 2020 2020  fg.ENVS)....    
-00005a40: 4074 696d 656d 6574 6572 2822 4164 6170  @timemeter("Adap
-00005a50: 7465 722f 636f 6d70 696c 6522 290d 0a20  ter/compile").. 
-00005a60: 2020 2064 6566 2063 6f6d 7069 6c65 2873     def compile(s
-00005a70: 656c 662c 2063 6667 3a20 436f 6e66 6967  elf, cfg: Config
-00005a80: 2920 2d3e 204e 6f6e 653a 0d0a 2020 2020  ) -> None:..    
-00005a90: 2020 2020 7222 2222 0d0a 2020 2020 2020      r"""..      
-00005aa0: 2020 436f 6e66 6967 7572 6520 7468 6520    Configure the 
-00005ab0: 636f 6d6d 616e 642c 2065 6e76 6972 6f6e  command, environ
-00005ac0: 6d65 6e74 732c 2061 6e64 2070 6172 616d  ments, and param
-00005ad0: 6574 6572 7320 666f 7220 7472 6169 6e69  eters for traini
-00005ae0: 6e67 2e0d 0a0d 0a20 2020 2020 2020 2050  ng.....        P
-00005af0: 6172 616d 6574 6572 733a 0d0a 2020 2020  arameters:..    
-00005b00: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d0d      -----------.
-00005b10: 0a20 2020 2020 2020 2063 6667 203a 2043  .        cfg : C
-00005b20: 6f6e 6669 670d 0a20 2020 2020 2020 2020  onfig..         
-00005b30: 2020 2041 6e20 6f62 6a65 6374 2074 6861     An object tha
-00005b40: 7420 636f 6e74 6169 6e73 2074 6865 2063  t contains the c
-00005b50: 6f6d 6d61 6e64 2c20 656e 7669 726f 6e6d  ommand, environm
-00005b60: 656e 7473 2c20 7061 7261 6d65 7465 7273  ents, parameters
-00005b70: 2c20 616e 6420 6465 6661 756c 7473 2e0d  , and defaults..
-00005b80: 0a0d 0a20 2020 2020 2020 2046 6c6f 7773  ...        Flows
-00005b90: 3a0d 0a20 2020 2020 2020 202d 2d2d 2d2d  :..        -----
-00005ba0: 2d0d 0a20 2020 2020 2020 2031 2e20 4164  -..        1. Ad
-00005bb0: 6420 656e 7669 726f 6e6d 656e 7461 6c20  d environmental 
-00005bc0: 7061 7261 6d65 7465 7273 2074 6f20 7468  parameters to th
-00005bd0: 6520 6261 7369 6320 6063 6f6d 6d61 6e64  e basic `command
-00005be0: 602e 0d0a 2020 2020 2020 2020 322e 2052  `...        2. R
-00005bf0: 6567 6973 7465 7220 616c 6c20 6176 6169  egister all avai
-00005c00: 6c61 626c 6520 6465 7669 6365 732e 0d0a  lable devices...
-00005c10: 2020 2020 2020 2020 332e 2043 6f6e 7665          3. Conve
-00005c20: 7274 2061 6c6c 2070 6172 616d 6574 6572  rt all parameter
-00005c30: 7320 6672 6f6d 2060 6366 672e 5041 5241  s from `cfg.PARA
-00005c40: 4d53 602e 0d0a 2020 2020 2020 2020 342e  MS`...        4.
-00005c50: 2043 6f6e 7665 7274 2061 6c6c 2064 6566   Convert all def
-00005c60: 6175 6c74 7320 6672 6f6d 2060 6366 672e  aults from `cfg.
-00005c70: 4445 4641 554c 5453 602e 0d0a 0d0a 2020  DEFAULTS`.....  
-00005c80: 2020 2020 2020 5265 7475 726e 733a 0d0a        Returns:..
-00005c90: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
-00005ca0: 0d0a 2020 2020 2020 2020 4e6f 6e65 0d0a  ..        None..
-00005cb0: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
-00005cc0: 2020 2020 2073 656c 662e 6366 6720 3d20       self.cfg = 
-00005cd0: 6366 670d 0a20 2020 2020 2020 2070 6965  cfg..        pie
-00005ce0: 6365 203d 2022 5c74 7b6b 6579 7d3a 207b  ce = "\t{key}: {
-00005cf0: 7661 6c73 7d20 5c6e 220d 0a20 2020 2020  vals} \n"..     
-00005d00: 2020 2065 6e76 732c 2070 6172 616d 732c     envs, params,
-00005d10: 2064 6566 6175 6c74 7320 3d20 2222 2c20   defaults = "", 
-00005d20: 2222 2c20 2222 0d0a 2020 2020 2020 2020  "", ""..        
-00005d30: 666f 7220 6b65 792c 2076 616c 2069 6e20  for key, val in 
-00005d40: 7365 6c66 2e63 6667 2e45 4e56 532e 6974  self.cfg.ENVS.it
-00005d50: 656d 7328 293a 0d0a 2020 2020 2020 2020  ems():..        
-00005d60: 2020 2020 6966 206b 6579 203d 3d20 2764      if key == 'd
-00005d70: 6576 6963 6527 3a0d 0a20 2020 2020 2020  evice':..       
-00005d80: 2020 2020 2020 2020 2073 656c 662e 6465           self.de
-00005d90: 7669 6365 7320 3d20 7661 6c2e 7370 6c69  vices = val.spli
-00005da0: 7428 272c 2729 0d0a 2020 2020 2020 2020  t(',')..        
-00005db0: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
-00005dc0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00005dd0: 6366 672e 434f 4d4d 414e 4420 2b3d 2073  cfg.COMMAND += s
-00005de0: 656c 662e 6765 745f 6f70 7469 6f6e 286b  elf.get_option(k
-00005df0: 6579 2c20 7661 6c29 0d0a 2020 2020 2020  ey, val)..      
-00005e00: 2020 2020 2020 656e 7673 202b 3d20 7069        envs += pi
-00005e10: 6563 652e 666f 726d 6174 286b 6579 3d6b  ece.format(key=k
-00005e20: 6579 2c20 7661 6c73 3d76 616c 290d 0a20  ey, vals=val).. 
-00005e30: 2020 2020 2020 2066 6f72 206b 6579 2c20         for key, 
-00005e40: 7661 6c73 2069 6e20 7365 6c66 2e63 6667  vals in self.cfg
-00005e50: 2e50 4152 414d 532e 6974 656d 7328 293a  .PARAMS.items():
-00005e60: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-00005e70: 2069 7369 6e73 7461 6e63 6528 7661 6c73   isinstance(vals
-00005e80: 2c20 2873 7472 2c20 696e 742c 2066 6c6f  , (str, int, flo
-00005e90: 6174 2929 3a0d 0a20 2020 2020 2020 2020  at)):..         
-00005ea0: 2020 2020 2020 2076 616c 7320 3d20 5b76         vals = [v
-00005eb0: 616c 735d 0d0a 2020 2020 2020 2020 2020  als]..          
-00005ec0: 2020 7365 6c66 2e64 6570 6c6f 795f 7061    self.deploy_pa
-00005ed0: 7261 6d73 286b 6579 2c20 7661 6c73 290d  rams(key, vals).
-00005ee0: 0a20 2020 2020 2020 2020 2020 2070 6172  .            par
-00005ef0: 616d 7320 2b3d 2070 6965 6365 2e66 6f72  ams += piece.for
-00005f00: 6d61 7428 6b65 793d 6b65 792c 2076 616c  mat(key=key, val
-00005f10: 733d 7661 6c73 290d 0a20 2020 2020 2020  s=vals)..       
-00005f20: 2066 6f72 206b 6579 2c20 7661 6c20 696e   for key, val in
-00005f30: 2073 656c 662e 6366 672e 4445 4641 554c   self.cfg.DEFAUL
-00005f40: 5453 2e69 7465 6d73 2829 3a0d 0a20 2020  TS.items():..   
-00005f50: 2020 2020 2020 2020 2073 656c 662e 6366           self.cf
-00005f60: 672e 4445 4641 554c 5453 5b6b 6579 5d20  g.DEFAULTS[key] 
-00005f70: 3d20 7661 6c0d 0a20 2020 2020 2020 2020  = val..         
-00005f80: 2020 2064 6566 6175 6c74 7320 2b3d 2070     defaults += p
-00005f90: 6965 6365 2e66 6f72 6d61 7428 6b65 793d  iece.format(key=
-00005fa0: 6b65 792c 2076 616c 733d 7661 6c29 0d0a  key, vals=val)..
-00005fb0: 0d0a 2020 2020 2020 2020 6366 675f 696e  ..        cfg_in
-00005fc0: 666f 7320 3d20 6622 636f 6d6d 616e 643a  fos = f"command:
-00005fd0: 207b 7365 6c66 2e63 6667 2e43 4f4d 4d41   {self.cfg.COMMA
-00005fe0: 4e44 7d20 5c6e 656e 7673 3a20 5c6e 7b65  ND} \nenvs: \n{e
-00005ff0: 6e76 737d 7061 7261 6d73 3a20 5c6e 7b70  nvs}params: \n{p
-00006000: 6172 616d 737d 6465 6661 756c 7473 3a20  arams}defaults: 
-00006010: 5c6e 7b64 6566 6175 6c74 737d 220d 0a20  \n{defaults}".. 
-00006020: 2020 2020 2020 2069 6e66 6f4c 6f67 6765         infoLogge
-00006030: 7228 6622 5c30 3333 5b30 3b33 313b 3437  r(f"\033[0;31;47
-00006040: 6d7b 6366 675f 696e 666f 737d 5c30 3333  m{cfg_infos}\033
-00006050: 5b30 6d22 290d 0a20 2020 2020 2020 200d  [0m")..        .
-00006060: 0a0d 0a20 2020 2064 6566 2064 6570 6c6f  ...    def deplo
-00006070: 795f 7061 7261 6d73 2873 656c 662c 206b  y_params(self, k
-00006080: 6579 3a20 7374 722c 2076 616c 733a 2049  ey: str, vals: I
-00006090: 7465 7261 626c 6529 3a0d 0a20 2020 2020  terable):..     
-000060a0: 2020 2073 656c 662e 7061 7261 6d73 2e61     self.params.a
-000060b0: 7070 656e 6428 6b65 7929 0d0a 2020 2020  ppend(key)..    
-000060c0: 2020 2020 7365 6c66 2e76 616c 7565 732e      self.values.
-000060d0: 6170 7065 6e64 2876 616c 7329 0d0a 0d0a  append(vals)....
-000060e0: 2020 2020 4073 7461 7469 636d 6574 686f      @staticmetho
-000060f0: 640d 0a20 2020 2064 6566 2067 6574 5f6f  d..    def get_o
-00006100: 7074 696f 6e28 6b65 793a 2073 7472 2c20  ption(key: str, 
-00006110: 7661 6c3a 2041 6e79 293a 0d0a 2020 2020  val: Any):..    
-00006120: 2020 2020 7222 2222 0d0a 2020 2020 2020      r"""..      
-00006130: 2020 436f 6e76 6572 7420 286b 6579 2c20    Convert (key, 
-00006140: 7661 6c29 2074 6f20 272d 2d6b 6579 3d76  val) to '--key=v
-00006150: 616c 272e 0d0a 0d0a 2020 2020 2020 2020  al'.....        
-00006160: 5061 7261 6d65 7465 7273 3a0d 0a20 2020  Parameters:..   
-00006170: 2020 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d       -----------
-00006180: 0d0a 2020 2020 2020 2020 6b65 7920 3a20  ..        key : 
-00006190: 7374 720d 0a20 2020 2020 2020 2020 2020  str..           
-000061a0: 2054 6865 206b 6579 206f 6620 7468 6520   The key of the 
-000061b0: 7061 7261 6d65 7465 722e 0d0a 2020 2020  parameter...    
-000061c0: 2020 2020 7661 6c20 3a20 416e 790d 0a20      val : Any.. 
-000061d0: 2020 2020 2020 2020 2020 2054 6865 2076             The v
-000061e0: 616c 7565 206f 6620 7468 6520 7061 7261  alue of the para
-000061f0: 6d65 7465 722e 0d0a 0d0a 2020 2020 2020  meter.....      
-00006200: 2020 4e6f 7465 733a 0d0a 2020 2020 2020    Notes:..      
-00006210: 2020 2d2d 2d2d 2d2d 0d0a 2020 2020 2020    ------..      
-00006220: 2020 416c 6c20 275f 2720 696e 2060 6b65    All '_' in `ke
-00006230: 7960 2077 696c 6c20 6265 2072 6570 6c61  y` will be repla
-00006240: 6365 6420 6279 2027 2d27 2e0d 0a0d 0a20  ced by '-'..... 
-00006250: 2020 2020 2020 2052 6574 7572 6e73 3a0d         Returns:.
-00006260: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
-00006270: 2d0d 0a20 2020 2020 2020 2073 7472 0d0a  -..        str..
-00006280: 2020 2020 2020 2020 2020 2020 5468 6520              The 
-00006290: 7061 7261 6d65 7465 7220 7769 7468 2066  parameter with f
-000062a0: 6f72 6d61 7420 272d 2d6b 6579 3d76 616c  ormat '--key=val
-000062b0: 272e 0d0a 0d0a 2020 2020 2020 2020 4578  '.....        Ex
-000062c0: 616d 706c 6573 3a0d 0a20 2020 2020 2020  amples:..       
-000062d0: 202d 2d2d 2d2d 2d2d 2d2d 0d0a 2020 2020   ---------..    
-000062e0: 2020 2020 3e3e 3e20 4164 6170 7465 722e      >>> Adapter.
-000062f0: 6765 745f 6f70 7469 6f6e 2827 6c72 272c  get_option('lr',
-00006300: 2027 3165 2d33 2729 0d0a 2020 2020 2020   '1e-3')..      
-00006310: 2020 272d 2d6c 723d 3165 2d33 270d 0a20    '--lr=1e-3'.. 
-00006320: 2020 2020 2020 203e 3e3e 2041 6461 7074         >>> Adapt
-00006330: 6572 2e67 6574 5f6f 7074 696f 6e28 276c  er.get_option('l
-00006340: 6561 726e 696e 675f 7261 7465 272c 2027  earning_rate', '
-00006350: 3165 2d33 2729 0d0a 2020 2020 2020 2020  1e-3')..        
-00006360: 272d 2d6c 6561 726e 696e 672d 7261 7465  '--learning-rate
-00006370: 3d31 652d 3327 0d0a 2020 2020 2020 2020  =1e-3'..        
-00006380: 2222 220d 0a20 2020 2020 2020 2072 6574  """..        ret
-00006390: 7572 6e20 6622 202d 2d7b 6b65 792e 7265  urn f" --{key.re
-000063a0: 706c 6163 6528 275f 272c 2027 2d27 297d  place('_', '-')}
-000063b0: 3d7b 7661 6c7d 220d 0a0d 0a20 2020 2064  ={val}"....    d
-000063c0: 6566 206c 6f61 645f 6265 7374 2873 656c  ef load_best(sel
-000063d0: 662c 206c 6f67 5061 7468 3a20 7374 7229  f, logPath: str)
-000063e0: 3a0d 0a20 2020 2020 2020 2022 2222 4c6f  :..        """Lo
-000063f0: 6164 2062 6573 742e 7069 636b 6c65 2066  ad best.pickle f
-00006400: 726f 6d20 6c6f 6750 6174 6820 6f66 2063  rom logPath of c
-00006410: 6f72 7265 7370 6f6e 6469 6e67 2e22 2222  orresponding."""
-00006420: 0d0a 2020 2020 2020 2020 6669 6c65 5f20  ..        file_ 
-00006430: 3d20 6f73 2e70 6174 682e 6a6f 696e 286c  = os.path.join(l
-00006440: 6f67 5061 7468 2c20 7365 6c66 2e63 6667  ogPath, self.cfg
-00006450: 2e44 4154 415f 4449 522c 2073 656c 662e  .DATA_DIR, self.
-00006460: 6366 672e 4d4f 4e49 544f 525f 4245 5354  cfg.MONITOR_BEST
-00006470: 5f46 494c 454e 414d 4529 0d0a 2020 2020  _FILENAME)..    
-00006480: 2020 2020 7265 7475 726e 2069 6d70 6f72      return impor
-00006490: 745f 7069 636b 6c65 2866 696c 655f 290d  t_pickle(file_).
-000064a0: 0a0d 0a20 2020 2064 6566 2077 7269 7465  ...    def write
-000064b0: 2873 656c 662c 2069 645f 3a20 7374 722c  (self, id_: str,
-000064c0: 206c 6f67 5061 7468 3a20 7374 722c 2070   logPath: str, p
-000064d0: 6172 616d 733a 2044 6963 7429 3a0d 0a20  arams: Dict):.. 
-000064e0: 2020 2020 2020 2072 2222 220d 0a20 2020         r"""..   
-000064f0: 2020 2020 2057 7269 7465 2065 7870 6572       Write exper
-00006500: 696d 656e 7420 7265 7375 6c74 7320 746f  iment results to
-00006510: 2074 656e 736f 7262 6f61 7264 2e0d 0a0d   tensorboard....
-00006520: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
-00006530: 6572 733a 0d0a 2020 2020 2020 2020 2d2d  ers:..        --
-00006540: 2d2d 2d2d 2d2d 2d2d 2d0d 0a20 2020 2020  ---------..     
-00006550: 2020 2069 645f 3a20 7374 720d 0a20 2020     id_: str..   
-00006560: 2020 2020 2020 2020 2045 7870 6572 696d           Experim
-00006570: 656e 7420 4944 2e0d 0a20 2020 2020 2020  ent ID...       
-00006580: 206c 6f67 5061 7468 3a20 7374 720d 0a20   logPath: str.. 
-00006590: 2020 2020 2020 2020 2020 2050 6174 6820             Path 
-000065a0: 746f 2074 6865 2065 7870 6572 696d 656e  to the experimen
-000065b0: 7420 6c6f 6773 2e0d 0a20 2020 2020 2020  t logs...       
-000065c0: 2070 6172 616d 733a 2044 6963 740d 0a20   params: Dict.. 
-000065d0: 2020 2020 2020 2020 2020 2043 6f6e 6669             Confi
-000065e0: 6775 7261 7469 6f6e 2070 6172 616d 6574  guration paramet
-000065f0: 6572 7320 6f66 2074 6865 2065 7870 6572  ers of the exper
-00006600: 696d 656e 742e 0d0a 0d0a 2020 2020 2020  iment.....      
-00006610: 2020 466c 6f77 733a 0d0a 2020 2020 2020    Flows:..      
-00006620: 2020 2d2d 2d2d 2d2d 0d0a 2020 2020 2020    ------..      
-00006630: 2020 312e 204c 6f61 6420 7468 6520 6265    1. Load the be
-00006640: 7374 2064 6174 6120 6672 6f6d 2060 6c6f  st data from `lo
-00006650: 6750 6174 6860 2e0d 0a20 2020 2020 2020  gPath`...       
-00006660: 2032 2e20 5772 6974 6520 7468 6520 6265   2. Write the be
-00006670: 7374 2064 6174 6120 746f 2074 656e 736f  st data to tenso
-00006680: 7262 6f61 7264 2077 6974 6820 6070 6172  rboard with `par
-00006690: 616d 7360 2e0d 0a0d 0a20 2020 2020 2020  ams`.....       
-000066a0: 204e 6f74 6573 3a0d 0a20 2020 2020 2020   Notes:..       
-000066b0: 202d 2d2d 2d2d 2d0d 0a20 2020 2020 2020   ------..       
-000066c0: 2049 6620 796f 7520 6669 6e64 2060 2d31   If you find `-1
-000066d0: 6020 6170 7065 6172 696e 6720 696e 2074  ` appearing in t
-000066e0: 6865 2074 656e 736f 7262 6f61 7264 2c0d  he tensorboard,.
-000066f0: 0a20 2020 2020 2020 2069 7420 636f 756c  .        it coul
-00006700: 6420 6d65 616e 2074 6861 7420 7468 6520  d mean that the 
-00006710: 6461 7461 2069 7320 6f66 2060 7374 7260  data is of `str`
-00006720: 2074 7970 652c 0d0a 2020 2020 2020 2020   type,..        
-00006730: 7768 6963 6820 7769 6c6c 2063 6175 7365  which will cause
-00006740: 2061 6e20 6572 726f 7220 6966 2069 7420   an error if it 
-00006750: 6973 2073 656e 7420 746f 2074 656e 736f  is sent to tenso
-00006760: 7262 6f61 7264 2064 6972 6563 746c 7921  rboard directly!
-00006770: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
-00006780: 2020 2020 2020 2074 7279 3a0d 0a20 2020         try:..   
-00006790: 2020 2020 2020 2020 2064 6174 6120 3d20           data = 
-000067a0: 7365 6c66 2e6c 6f61 645f 6265 7374 286c  self.load_best(l
-000067b0: 6f67 5061 7468 290d 0a20 2020 2020 2020  ogPath)..       
-000067c0: 2020 2020 2070 6174 6820 3d20 6f73 2e70       path = os.p
-000067d0: 6174 682e 6a6f 696e 2873 656c 662e 6366  ath.join(self.cf
-000067e0: 672e 434f 5245 5f4c 4f47 5f50 4154 482c  g.CORE_LOG_PATH,
-000067f0: 2069 645f 290d 0a20 2020 2020 2020 2020   id_)..         
-00006800: 2020 2077 6974 6820 5375 6d6d 6172 7957     with SummaryW
-00006810: 7269 7465 7228 6c6f 675f 6469 723d 7061  riter(log_dir=pa
-00006820: 7468 2920 6173 2077 7269 7465 723a 0d0a  th) as writer:..
-00006830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006840: 6d65 7472 6963 7320 3d20 6469 6374 2829  metrics = dict()
-00006850: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00006860: 2020 666f 7220 7072 6566 6978 2c20 6265    for prefix, be
-00006870: 7374 2069 6e20 6461 7461 2e69 7465 6d73  st in data.items
-00006880: 2829 3a0d 0a20 2020 2020 2020 2020 2020  ():..           
-00006890: 2020 2020 2020 2020 2066 6f72 206d 6574           for met
-000068a0: 7269 632c 2076 616c 2069 6e20 6265 7374  ric, val in best
-000068b0: 2e69 7465 6d73 2829 3a0d 0a20 2020 2020  .items():..     
-000068c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000068d0: 2020 2076 616c 203d 2076 616c 2069 6620     val = val if 
-000068e0: 6973 696e 7374 616e 6365 2876 616c 2c20  isinstance(val, 
-000068f0: 2869 6e74 2c20 666c 6f61 7429 2920 656c  (int, float)) el
-00006900: 7365 202d 310d 0a20 2020 2020 2020 2020  se -1..         
-00006910: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-00006920: 6574 7269 6373 5b27 2f27 2e6a 6f69 6e28  etrics['/'.join(
-00006930: 5b70 7265 6669 782c 206d 6574 7269 635d  [prefix, metric]
-00006940: 295d 203d 2076 616c 0d0a 2020 2020 2020  )] = val..      
-00006950: 2020 2020 2020 2020 2020 7772 6974 6572            writer
-00006960: 2e61 6464 5f68 7061 7261 6d73 280d 0a20  .add_hparams(.. 
-00006970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006980: 2020 2070 6172 616d 732c 206d 6574 7269     params, metri
-00006990: 6373 2c0d 0a20 2020 2020 2020 2020 2020  cs,..           
-000069a0: 2020 2020 2029 0d0a 2020 2020 2020 2020       )..        
-000069b0: 6578 6365 7074 2045 7863 6570 7469 6f6e  except Exception
-000069c0: 3a0d 0a20 2020 2020 2020 2020 2020 2069  :..            i
-000069d0: 6e66 6f4c 6f67 6765 7228 0d0a 2020 2020  nfoLogger(..    
-000069e0: 2020 2020 2020 2020 2020 2020 6622 5c30              f"\0
-000069f0: 3333 5b30 3b33 313b 3437 6d5b 4164 6170  33[0;31;47m[Adap
-00006a00: 7465 725d 203e 3e3e 2055 6e6b 6e6f 776e  ter] >>> Unknown
-00006a10: 2065 7272 6f72 7320 6861 7070 656e 2e20   errors happen. 
-00006a20: 5468 6973 2069 7320 6d61 696e 6c79 2064  This is mainly d
-00006a30: 7565 2074 6f20 6162 6e6f 726d 616c 2065  ue to abnormal e
-00006a40: 7869 7473 206f 6620 6368 696c 6420 7072  xits of child pr
-00006a50: 6f63 6573 7365 732e 5c30 3333 5b30 6d22  ocesses.\033[0m"
-00006a60: 0d0a 2020 2020 2020 2020 2020 2020 290d  ..            ).
-00006a70: 0a0d 0a0d 0a20 2020 2064 6566 2065 6163  .....    def eac
-00006a80: 685f 6772 6964 2873 656c 6629 3a0d 0a20  h_grid(self):.. 
-00006a90: 2020 2020 2020 2022 2222 4772 6964 2073         """Grid s
-00006aa0: 6561 7263 6820 666f 7220 6561 6368 206b  earch for each k
-00006ab0: 696e 6420 6f66 2070 6172 616d 2e22 2222  ind of param."""
-00006ac0: 0d0a 2020 2020 2020 2020 666f 7220 6b65  ..        for ke
-00006ad0: 792c 2076 616c 7320 696e 207a 6970 2873  y, vals in zip(s
-00006ae0: 656c 662e 7061 7261 6d73 2c20 7365 6c66  elf.params, self
-00006af0: 2e76 616c 7565 7329 3a0d 0a20 2020 2020  .values):..     
-00006b00: 2020 2020 2020 2066 6f72 2076 616c 2069         for val i
-00006b10: 6e20 7661 6c73 3a0d 0a20 2020 2020 2020  n vals:..       
-00006b20: 2020 2020 2020 2020 2079 6965 6c64 2073           yield s
-00006b30: 656c 662e 6366 672e 4445 4641 554c 5453  elf.cfg.DEFAULTS
-00006b40: 207c 207b 6b65 793a 2076 616c 7d0d 0a0d   | {key: val}...
-00006b50: 0a20 2020 2064 6566 2070 726f 6475 6374  .    def product
-00006b60: 5f67 7269 6428 7365 6c66 293a 0d0a 2020  _grid(self):..  
-00006b70: 2020 2020 2020 2222 2247 7269 6420 7365        """Grid se
-00006b80: 6172 6368 2061 6372 6f73 7320 616c 6c20  arch across all 
-00006b90: 636f 6d62 696e 6174 696f 6e20 6f66 2070  combination of p
-00006ba0: 6172 616d 7322 2222 0d0a 2020 2020 2020  arams"""..      
-00006bb0: 2020 666f 7220 7661 6c73 2069 6e20 7072    for vals in pr
-00006bc0: 6f64 7563 7428 2a73 656c 662e 7661 6c75  oduct(*self.valu
-00006bd0: 6573 293a 0d0a 2020 2020 2020 2020 2020  es):..          
-00006be0: 2020 7969 656c 6420 7365 6c66 2e63 6667    yield self.cfg
-00006bf0: 2e44 4546 4155 4c54 5320 7c20 7b6f 7074  .DEFAULTS | {opt
-00006c00: 696f 6e3a 7661 6c20 666f 7220 6f70 7469  ion:val for opti
-00006c10: 6f6e 2c20 7661 6c20 696e 207a 6970 2873  on, val in zip(s
-00006c20: 656c 662e 7061 7261 6d73 2c20 7661 6c73  elf.params, vals
-00006c30: 297d 0d0a 0d0a 2020 2020 6465 6620 7361  )}....    def sa
-00006c40: 7665 5f63 6865 636b 706f 696e 7428 7365  ve_checkpoint(se
-00006c50: 6c66 2c20 736f 7572 6365 3a20 4c69 7374  lf, source: List
-00006c60: 2920 2d3e 204e 6f6e 653a 0d0a 2020 2020  ) -> None:..    
-00006c70: 2020 2020 2222 2253 6176 6520 7468 6520      """Save the 
-00006c80: 7265 7374 206f 6620 7061 7261 6d73 2e22  rest of params."
-00006c90: 2222 0d0a 2020 2020 2020 2020 7061 7468  ""..        path
-00006ca0: 203d 206f 732e 7061 7468 2e6a 6f69 6e28   = os.path.join(
-00006cb0: 7365 6c66 2e63 6667 2e43 4f52 455f 4348  self.cfg.CORE_CH
-00006cc0: 4543 4b50 4f49 4e54 5f50 4154 482c 2073  ECKPOINT_PATH, s
-00006cd0: 656c 662e 6366 672e 4348 4543 4b50 4f49  elf.cfg.CHECKPOI
-00006ce0: 4e54 5f46 494c 454e 414d 4529 0d0a 2020  NT_FILENAME)..  
-00006cf0: 2020 2020 2020 6368 6563 6b70 6f69 6e74        checkpoint
-00006d00: 203d 2064 6963 7428 290d 0a20 2020 2020   = dict()..     
-00006d10: 2020 2063 6865 636b 706f 696e 745b 2773     checkpoint['s
-00006d20: 6f75 7263 6527 5d20 3d20 736f 7572 6365  ource'] = source
-00006d30: 0d0a 2020 2020 2020 2020 746f 7263 682e  ..        torch.
-00006d40: 7361 7665 2863 6865 636b 706f 696e 742c  save(checkpoint,
-00006d50: 2070 6174 6829 0d0a 0d0a 2020 2020 6465   path)....    de
-00006d60: 6620 6c6f 6164 5f63 6865 636b 706f 696e  f load_checkpoin
-00006d70: 7428 7365 6c66 2920 2d3e 2069 6e74 3a0d  t(self) -> int:.
-00006d80: 0a20 2020 2020 2020 2022 2222 4c6f 6164  .        """Load
-00006d90: 2074 6865 2072 6573 7420 6f66 2070 6172   the rest of par
-00006da0: 616d 732e 2222 220d 0a20 2020 2020 2020  ams."""..       
-00006db0: 2070 6174 6820 3d20 6f73 2e70 6174 682e   path = os.path.
-00006dc0: 6a6f 696e 2873 656c 662e 6366 672e 434f  join(self.cfg.CO
-00006dd0: 5245 5f43 4845 434b 504f 494e 545f 5041  RE_CHECKPOINT_PA
-00006de0: 5448 2c20 7365 6c66 2e63 6667 2e43 4845  TH, self.cfg.CHE
-00006df0: 434b 504f 494e 545f 4649 4c45 4e41 4d45  CKPOINT_FILENAME
-00006e00: 290d 0a20 2020 2020 2020 2063 6865 636b  )..        check
-00006e10: 706f 696e 7420 3d20 746f 7263 682e 6c6f  point = torch.lo
-00006e20: 6164 2870 6174 6829 0d0a 2020 2020 2020  ad(path)..      
-00006e30: 2020 7265 7475 726e 2063 6865 636b 706f    return checkpo
-00006e40: 696e 745b 2773 6f75 7263 6527 5d0d 0a0d  int['source']...
-00006e50: 0a20 2020 2040 7469 6d65 6d65 7465 7228  .    @timemeter(
-00006e60: 2243 6f61 6368 2f72 6573 756d 6522 290d  "Coach/resume").
-00006e70: 0a20 2020 2064 6566 2072 6573 756d 6528  .    def resume(
-00006e80: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
-00006e90: 2222 2252 6573 756d 6520 6672 6f6d 2074  """Resume from t
-00006ea0: 6865 2072 6563 656e 7420 6368 6563 6b70  he recent checkp
-00006eb0: 6f69 6e74 2e22 2222 0d0a 2020 2020 2020  oint."""..      
-00006ec0: 2020 736f 7572 6365 203d 2073 656c 662e    source = self.
-00006ed0: 6561 6368 5f67 7269 6428 2920 6966 2073  each_grid() if s
-00006ee0: 656c 662e 6366 672e 4558 434c 5553 4956  elf.cfg.EXCLUSIV
-00006ef0: 4520 656c 7365 2073 656c 662e 7072 6f64  E else self.prod
-00006f00: 7563 745f 6772 6964 2829 0d0a 2020 2020  uct_grid()..    
-00006f10: 2020 2020 736f 7572 6365 203d 206c 6973      source = lis
-00006f20: 7428 736f 7572 6365 295b 3a3a 2d31 5d0d  t(source)[::-1].
-00006f30: 0a20 2020 2020 2020 2073 6f75 7263 6520  .        source 
-00006f40: 3d20 7365 6c66 2e6c 6f61 645f 6368 6563  = self.load_chec
-00006f50: 6b70 6f69 6e74 2829 2069 6620 7365 6c66  kpoint() if self
-00006f60: 2e63 6667 2e72 6573 756d 6520 656c 7365  .cfg.resume else
-00006f70: 2073 6f75 7263 650d 0a20 2020 2020 2020   source..       
-00006f80: 2069 6e66 6f4c 6f67 6765 7228 6622 5b43   infoLogger(f"[C
-00006f90: 6f61 6368 5d20 3e3e 3e20 4c6f 6164 2074  oach] >>> Load t
-00006fa0: 6865 2072 6563 656e 7420 6368 6563 6b70  he recent checkp
-00006fb0: 6f69 6e74 202e 2e2e 2229 0d0a 2020 2020  oint ...")..    
-00006fc0: 2020 2020 7265 7475 726e 2073 6f75 7263      return sourc
-00006fd0: 650d 0a0d 0a20 2020 2064 6566 2072 756e  e....    def run
-00006fe0: 2873 656c 662c 2063 6f6d 6d61 6e64 3a20  (self, command: 
-00006ff0: 7374 722c 2070 6172 616d 733a 2044 6963  str, params: Dic
-00007000: 7429 3a0d 0a20 2020 2020 2020 2022 2222  t):..        """
-00007010: 5374 6172 7420 6120 6e65 7720 7375 6270  Start a new subp
-00007020: 726f 6365 7373 2222 220d 0a20 2020 2020  rocess"""..     
-00007030: 2020 2066 6f72 206f 7074 696f 6e2c 2076     for option, v
-00007040: 616c 2069 6e20 7061 7261 6d73 2e69 7465  al in params.ite
-00007050: 6d73 2829 3a0d 0a20 2020 2020 2020 2020  ms():..         
-00007060: 2020 2063 6f6d 6d61 6e64 202b 3d20 7365     command += se
-00007070: 6c66 2e67 6574 5f6f 7074 696f 6e28 6f70  lf.get_option(op
-00007080: 7469 6f6e 2c20 7661 6c29 0d0a 2020 2020  tion, val)..    
-00007090: 2020 2020 696e 666f 4c6f 6767 6572 2866      infoLogger(f
-000070a0: 225c 3033 335b 303b 3331 3b34 376d 7b63  "\033[0;31;47m{c
-000070b0: 6f6d 6d61 6e64 7d5c 3033 335b 306d 2229  ommand}\033[0m")
-000070c0: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-000070d0: 2073 7562 7072 6f63 6573 732e 506f 7065   subprocess.Pope
-000070e0: 6e28 7368 6c65 782e 7370 6c69 7428 636f  n(shlex.split(co
-000070f0: 6d6d 616e 6429 290d 0a0d 0a20 2020 2064  mmand))....    d
-00007100: 6566 2077 6169 7428 7365 6c66 2c20 7461  ef wait(self, ta
-00007110: 736b 733a 2044 6963 7429 3a0d 0a20 2020  sks: Dict):..   
-00007120: 2020 2020 2022 2222 5761 6974 2075 7469       """Wait uti
-00007130: 6c20 616c 6c20 7072 6f63 6573 7365 7320  l all processes 
-00007140: 7465 726d 696e 6174 652e 2222 220d 0a20  terminate.""".. 
-00007150: 2020 2020 2020 2066 6f72 2070 726f 6365         for proce
-00007160: 7373 5f2c 2069 645f 2c20 6c6f 6750 6174  ss_, id_, logPat
-00007170: 682c 2070 6172 616d 7320 696e 2074 6173  h, params in tas
-00007180: 6b73 2e76 616c 7565 7328 293a 0d0a 2020  ks.values():..  
-00007190: 2020 2020 2020 2020 2020 7072 6f63 6573            proces
-000071a0: 735f 2e77 6169 7428 290d 0a20 2020 2020  s_.wait()..     
-000071b0: 2020 2020 2020 2073 656c 662e 7772 6974         self.writ
-000071c0: 6528 6964 5f2c 206c 6f67 5061 7468 2c20  e(id_, logPath, 
-000071d0: 7061 7261 6d73 290d 0a0d 0a20 2020 2064  params)....    d
-000071e0: 6566 2070 6f6c 6c28 7365 6c66 2c20 7461  ef poll(self, ta
-000071f0: 736b 733a 2044 6963 7429 3a0d 0a20 2020  sks: Dict):..   
-00007200: 2020 2020 2022 2222 5761 6974 2075 7469       """Wait uti
-00007210: 6c20 616e 7920 7072 6f63 6573 7320 7465  l any process te
-00007220: 726d 696e 6174 6573 2e22 2222 0d0a 2020  rminates."""..  
-00007230: 2020 2020 2020 6275 6666 6572 5f73 6f75        buffer_sou
-00007240: 7263 6520 3d20 5b5d 0d0a 2020 2020 2020  rce = []..      
-00007250: 2020 7469 6d65 2e73 6c65 6570 2831 2920    time.sleep(1) 
-00007260: 2320 666f 7220 756e 6971 7565 2069 640d  # for unique id.
-00007270: 0a20 2020 2020 2020 2077 6869 6c65 206c  .        while l
-00007280: 656e 2873 656c 662e 6465 7669 6365 7329  en(self.devices)
-00007290: 203d 3d20 303a 0d0a 2020 2020 2020 2020   == 0:..        
-000072a0: 2020 2020 7469 6d65 2e73 6c65 6570 2837      time.sleep(7
-000072b0: 290d 0a20 2020 2020 2020 2020 2020 2066  )..            f
-000072c0: 6f72 2064 6576 6963 652c 2028 7072 6f63  or device, (proc
-000072d0: 6573 735f 2c20 6964 5f2c 206c 6f67 5061  ess_, id_, logPa
-000072e0: 7468 2c20 7061 7261 6d73 2920 696e 2074  th, params) in t
-000072f0: 6173 6b73 2e69 7465 6d73 2829 3a0d 0a20  asks.items():.. 
-00007300: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00007310: 6620 7072 6f63 6573 735f 2e70 6f6c 6c28  f process_.poll(
-00007320: 2920 6973 206e 6f74 204e 6f6e 653a 0d0a  ) is not None:..
-00007330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007340: 2020 2020 7365 6c66 2e77 7269 7465 2869      self.write(i
-00007350: 645f 2c20 6c6f 6750 6174 682c 2070 6172  d_, logPath, par
-00007360: 616d 7329 0d0a 2020 2020 2020 2020 2020  ams)..          
-00007370: 2020 2020 2020 2020 2020 7365 6c66 2e64            self.d
-00007380: 6576 6963 6573 2e61 7070 656e 6428 6465  evices.append(de
-00007390: 7669 6365 290d 0a20 2020 2020 2020 2020  vice)..         
-000073a0: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
-000073b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000073c0: 2020 6275 6666 6572 5f73 6f75 7263 652e    buffer_source.
-000073d0: 6170 7065 6e64 2870 6172 616d 7329 0d0a  append(params)..
-000073e0: 2020 2020 2020 2020 7365 6c66 2e73 6176          self.sav
-000073f0: 655f 6368 6563 6b70 6f69 6e74 2873 656c  e_checkpoint(sel
-00007400: 662e 736f 7572 6365 202b 2062 7566 6665  f.source + buffe
-00007410: 725f 736f 7572 6365 290d 0a0d 0a20 2020  r_source)....   
-00007420: 2064 6566 2074 6572 6d69 6e61 7465 2873   def terminate(s
-00007430: 656c 662c 2074 6173 6b73 293a 0d0a 2020  elf, tasks):..  
-00007440: 2020 2020 2020 666f 7220 6465 7669 6365        for device
-00007450: 2069 6e20 7461 736b 733a 0d0a 2020 2020   in tasks:..    
-00007460: 2020 2020 2020 2020 7072 6f63 6573 735f          process_
-00007470: 2c20 5f2c 205f 2c20 5f20 3d20 7461 736b  , _, _, _ = task
-00007480: 735b 6465 7669 6365 5d0d 0a20 2020 2020  s[device]..     
-00007490: 2020 2020 2020 2069 6620 7072 6f63 6573         if proces
-000074a0: 735f 2e70 6f6c 6c28 2920 6973 204e 6f6e  s_.poll() is Non
-000074b0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-000074c0: 2020 2020 7072 6f63 6573 735f 2e74 6572      process_.ter
-000074d0: 6d69 6e61 7465 2829 0d0a 2020 2020 2020  minate()..      
-000074e0: 2020 7469 6d65 2e73 6c65 6570 2833 290d    time.sleep(3).
-000074f0: 0a20 2020 2020 2020 2066 6f72 2064 6576  .        for dev
-00007500: 6963 6520 696e 2074 6173 6b73 3a0d 0a20  ice in tasks:.. 
-00007510: 2020 2020 2020 2020 2020 2070 726f 6365             proce
-00007520: 7373 5f2c 205f 2c20 5f2c 205f 203d 2074  ss_, _, _, _ = t
-00007530: 6173 6b73 5b64 6576 6963 655d 0d0a 2020  asks[device]..  
-00007540: 2020 2020 2020 2020 2020 6966 2070 726f            if pro
-00007550: 6365 7373 5f2e 706f 6c6c 2829 2069 7320  cess_.poll() is 
-00007560: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2020  None:..         
-00007570: 2020 2020 2020 2070 726f 6365 7373 5f2e         process_.
-00007580: 6b69 6c6c 2829 0d0a 2020 2020 2020 2020  kill()..        
-00007590: 7379 732e 6578 6974 2829 0d0a 0d0a 2020  sys.exit()....  
-000075a0: 2020 4074 696d 656d 6574 6572 2822 4164    @timemeter("Ad
-000075b0: 6170 7465 722f 6669 7422 290d 0a20 2020  apter/fit")..   
-000075c0: 2064 6566 2066 6974 2873 656c 6629 3a0d   def fit(self):.
-000075d0: 0a20 2020 2020 2020 2022 2222 4772 6964  .        """Grid
-000075e0: 2073 6561 7263 682e 2222 220d 0a20 2020   search."""..   
-000075f0: 2020 2020 2073 656c 662e 736f 7572 6365       self.source
-00007600: 203d 2073 656c 662e 7265 7375 6d65 2829   = self.resume()
-00007610: 0d0a 2020 2020 2020 2020 7461 736b 7320  ..        tasks 
-00007620: 3d20 6469 6374 2829 0d0a 0d0a 2020 2020  = dict()....    
-00007630: 2020 2020 6465 6620 7369 676e 616c 5f68      def signal_h
-00007640: 616e 646c 6572 2873 6967 2c20 6672 616d  andler(sig, fram
-00007650: 6529 3a0d 0a20 2020 2020 2020 2020 2020  e):..           
-00007660: 2069 6e66 6f4c 6f67 6765 7228 6622 5c30   infoLogger(f"\0
-00007670: 3333 5b30 3b33 313b 3437 6d3d 3d3d 3d3d  33[0;31;47m=====
-00007680: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00007690: 3d3d 3d3d 3d3d 3d3d 3d3d 5445 524d 494e  ==========TERMIN
-000076a0: 4154 4520 414c 4c20 5355 4250 524f 4345  ATE ALL SUBPROCE
-000076b0: 5353 4553 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  SSES============
-000076c0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000076d0: 3d3d 3d5c 3033 335b 306d 2229 0d0a 2020  ===\033[0m")..  
-000076e0: 2020 2020 2020 2020 2020 7365 6c66 2e74            self.t
-000076f0: 6572 6d69 6e61 7465 2874 6173 6b73 290d  erminate(tasks).
-00007700: 0a20 2020 2020 2020 2073 6967 6e61 6c2e  .        signal.
-00007710: 7369 676e 616c 2873 6967 6e61 6c2e 5349  signal(signal.SI
-00007720: 4749 4e54 2c20 7369 676e 616c 5f68 616e  GINT, signal_han
-00007730: 646c 6572 290d 0a0d 0a20 2020 2020 2020  dler)....       
-00007740: 2074 7279 3a0d 0a20 2020 2020 2020 2020   try:..         
-00007750: 2020 2077 6869 6c65 2073 656c 662e 736f     while self.so
-00007760: 7572 6365 3a0d 0a20 2020 2020 2020 2020  urce:..         
-00007770: 2020 2020 2020 2073 656c 662e 706f 6c6c         self.poll
-00007780: 2874 6173 6b73 290d 0a20 2020 2020 2020  (tasks)..       
-00007790: 2020 2020 2020 2020 2070 6172 616d 7320           params 
-000077a0: 3d20 7365 6c66 2e73 6f75 7263 652e 706f  = self.source.po
-000077b0: 7028 290d 0a20 2020 2020 2020 2020 2020  p()..           
-000077c0: 2020 2020 2064 6576 6963 6520 3d20 7365       device = se
-000077d0: 6c66 2e64 6576 6963 6573 2e70 6f70 2829  lf.devices.pop()
-000077e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000077f0: 2020 636f 6d6d 616e 642c 2069 645f 2c20    command, id_, 
-00007800: 6c6f 6750 6174 6820 3d20 7365 6c66 2e72  logPath = self.r
-00007810: 6567 6973 7465 7228 6465 7669 6365 290d  egister(device).
-00007820: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007830: 2070 726f 6365 7373 5f20 3d20 7365 6c66   process_ = self
-00007840: 2e72 756e 2863 6f6d 6d61 6e64 2c20 7061  .run(command, pa
-00007850: 7261 6d73 290d 0a20 2020 2020 2020 2020  rams)..         
-00007860: 2020 2020 2020 2074 6173 6b73 5b64 6576         tasks[dev
-00007870: 6963 655d 203d 2028 7072 6f63 6573 735f  ice] = (process_
-00007880: 2c20 6964 5f2c 206c 6f67 5061 7468 2c20  , id_, logPath, 
-00007890: 7061 7261 6d73 290d 0a20 2020 2020 2020  params)..       
-000078a0: 2065 7863 6570 7420 4578 6365 7074 696f   except Exceptio
-000078b0: 6e20 6173 2065 3a0d 0a20 2020 2020 2020  n as e:..       
-000078c0: 2020 2020 2070 7269 6e74 2865 290d 0a20       print(e).. 
-000078d0: 2020 2020 2020 2066 696e 616c 6c79 3a0d         finally:.
-000078e0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-000078f0: 662e 7761 6974 2874 6173 6b73 290d 0a20  f.wait(tasks).. 
-00007900: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00007910: 7465 726d 696e 6174 6528 7461 736b 7329  terminate(tasks)
+00004cb0: 2076 616c 3d76 616c 2c20 6570 6f63 683d   val=val, epoch=
+00004cc0: 6570 6f63 682c 2069 6d67 3d66 2221 5b5d  epoch, img=f"![]
+00004cd0: 287b 696d 676e 616d 657d 2922 0d0a 2020  ({imgname})"..  
+00004ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004cf0: 2020 290d 0a20 2020 2020 2020 2020 2020    )..           
+00004d00: 2020 2020 2020 2020 2064 6174 612e 6170           data.ap
+00004d10: 7065 6e64 285b 7072 6566 6978 2c20 6d65  pend([prefix, me
+00004d20: 7465 722e 6e61 6d65 2c20 7661 6c2c 2065  ter.name, val, e
+00004d30: 706f 6368 5d29 0d0a 2020 2020 2020 2020  poch])..        
+00004d40: 2020 2020 2020 2020 2020 2020 6966 2076              if v
+00004d50: 616c 2021 3d20 2d31 3a20 2320 4f6e 6c79  al != -1: # Only
+00004d60: 2073 6176 6520 6176 6169 6c61 626c 6520   save available 
+00004d70: 6461 7461 2e0d 0a20 2020 2020 2020 2020  data...         
+00004d80: 2020 2020 2020 2020 2020 2020 2020 2062                 b
+00004d90: 6573 745b 7072 6566 6978 5d5b 6d65 7465  est[prefix][mete
+00004da0: 722e 6e61 6d65 5d20 3d20 7661 6c0d 0a0d  r.name] = val...
+00004db0: 0a20 2020 2020 2020 2066 696c 655f 203d  .        file_ =
+00004dc0: 206f 732e 7061 7468 2e6a 6f69 6e28 7365   os.path.join(se
+00004dd0: 6c66 2e63 6667 2e4c 4f47 5f50 4154 482c  lf.cfg.LOG_PATH,
+00004de0: 2073 656c 662e 6366 672e 5355 4d4d 4152   self.cfg.SUMMAR
+00004df0: 595f 4449 522c 2073 656c 662e 6366 672e  Y_DIR, self.cfg.
+00004e00: 5355 4d4d 4152 595f 4649 4c45 4e41 4d45  SUMMARY_FILENAME
+00004e10: 290d 0a20 2020 2020 2020 2077 6974 6820  )..        with 
+00004e20: 6f70 656e 2866 696c 655f 2c20 2277 222c  open(file_, "w",
+00004e30: 2065 6e63 6f64 696e 673d 2275 7466 3822   encoding="utf8"
+00004e40: 2920 6173 2066 683a 0d0a 2020 2020 2020  ) as fh:..      
+00004e50: 2020 2020 2020 6668 2e77 7269 7465 2869        fh.write(i
+00004e60: 6e66 6f29 0d0a 0d0a 2020 2020 2020 2020  nfo)....        
+00004e70: 6466 203d 2070 642e 4461 7461 4672 616d  df = pd.DataFram
+00004e80: 6528 6461 7461 2c20 636f 6c75 6d6e 733d  e(data, columns=
+00004e90: 5b27 5072 6566 6978 272c 2027 4d65 7472  ['Prefix', 'Metr
+00004ea0: 6963 272c 2027 4265 7374 272c 2027 4045  ic', 'Best', '@E
+00004eb0: 706f 6368 275d 290d 0a20 2020 2020 2020  poch'])..       
+00004ec0: 2069 6e66 6f4c 6f67 6765 7228 7374 7228   infoLogger(str(
+00004ed0: 6466 2929 0d0a 2020 2020 2020 2020 696e  df))..        in
+00004ee0: 666f 4c6f 6767 6572 2866 225b 4c6f 475f  foLogger(f"[LoG_
+00004ef0: 5061 5448 5d20 3e3e 3e20 7b73 656c 662e  PaTH] >>> {self.
+00004f00: 6366 672e 4c4f 475f 5041 5448 7d22 290d  cfg.LOG_PATH}").
+00004f10: 0a0d 0a20 2020 2020 2020 2073 656c 662e  ...        self.
+00004f20: 6d6f 6e69 746f 7273 2e77 7269 7465 286f  monitors.write(o
+00004f30: 732e 7061 7468 2e6a 6f69 6e28 7365 6c66  s.path.join(self
+00004f40: 2e63 6667 2e4c 4f47 5f50 4154 482c 2073  .cfg.LOG_PATH, s
+00004f50: 656c 662e 6366 672e 5355 4d4d 4152 595f  elf.cfg.SUMMARY_
+00004f60: 4449 5229 2920 2320 7465 6e73 6f72 626f  DIR)) # tensorbo
+00004f70: 6172 640d 0a0d 0a20 2020 2020 2020 2073  ard....        s
+00004f80: 656c 662e 6d6f 6e69 746f 7273 2e73 6176  elf.monitors.sav
+00004f90: 6528 6f73 2e70 6174 682e 6a6f 696e 2873  e(os.path.join(s
+00004fa0: 656c 662e 6366 672e 4c4f 475f 5041 5448  elf.cfg.LOG_PATH
+00004fb0: 2c20 7365 6c66 2e63 6667 2e44 4154 415f  , self.cfg.DATA_
+00004fc0: 4449 5229 2c20 7365 6c66 2e63 6667 2e4d  DIR), self.cfg.M
+00004fd0: 4f4e 4954 4f52 5f46 494c 454e 414d 4529  ONITOR_FILENAME)
+00004fe0: 0d0a 2020 2020 2020 2020 6578 706f 7274  ..        export
+00004ff0: 5f70 6963 6b6c 6528 6265 7374 2c20 6f73  _pickle(best, os
+00005000: 2e70 6174 682e 6a6f 696e 2873 656c 662e  .path.join(self.
+00005010: 6366 672e 4c4f 475f 5041 5448 2c20 7365  cfg.LOG_PATH, se
+00005020: 6c66 2e63 6667 2e44 4154 415f 4449 522c  lf.cfg.DATA_DIR,
+00005030: 2073 656c 662e 6366 672e 4d4f 4e49 544f   self.cfg.MONITO
+00005040: 525f 4245 5354 5f46 494c 454e 414d 4529  R_BEST_FILENAME)
+00005050: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
+00005060: 200d 0a20 2020 2040 7469 6d65 6d65 7465   ..    @timemete
+00005070: 7228 2243 6f61 6368 2f66 6974 2229 0d0a  r("Coach/fit")..
+00005080: 2020 2020 6465 6620 6669 7428 7365 6c66      def fit(self
+00005090: 293a 0d0a 0d0a 2020 2020 2020 2020 6465  ):....        de
+000050a0: 6620 7369 676e 616c 5f68 616e 646c 6572  f signal_handler
+000050b0: 2873 6967 2c20 6672 616d 6529 3a0d 0a20  (sig, frame):.. 
+000050c0: 2020 2020 2020 2020 2020 2069 6e66 6f4c             infoL
+000050d0: 6f67 6765 7228 6622 5c30 3333 5b30 3b33  ogger(f"\033[0;3
+000050e0: 313b 3437 6d3d 3d3d 3d3d 3d3d 3d3d 3d3d  1;47m===========
+000050f0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00005100: 3d3d 3d3d 5445 524d 494e 4154 4520 4355  ====TERMINATE CU
+00005110: 5252 454e 5420 5052 4f43 4553 533d 3d3d  RRENT PROCESS===
+00005120: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00005130: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 5c30 3333  ============\033
+00005140: 5b30 6d22 290d 0a20 2020 2020 2020 2020  [0m")..         
+00005150: 2020 2073 7973 2e65 7869 7428 290d 0a20     sys.exit().. 
+00005160: 2020 2020 2020 2073 6967 6e61 6c2e 7369         signal.si
+00005170: 676e 616c 2873 6967 6e61 6c2e 5349 4749  gnal(signal.SIGI
+00005180: 4e54 2c20 7369 676e 616c 5f68 616e 646c  NT, signal_handl
+00005190: 6572 290d 0a0d 0a20 2020 2020 2020 2073  er)....        s
+000051a0: 7461 7274 5f65 706f 6368 203d 2073 656c  tart_epoch = sel
+000051b0: 662e 7265 7375 6d65 2829 0d0a 2020 2020  f.resume()..    
+000051c0: 2020 2020 666f 7220 6570 6f63 6820 696e      for epoch in
+000051d0: 2072 616e 6765 2873 7461 7274 5f65 706f   range(start_epo
+000051e0: 6368 2c20 7365 6c66 2e63 6667 2e65 706f  ch, self.cfg.epo
+000051f0: 6368 7329 3a0d 0a20 2020 2020 2020 2020  chs):..         
+00005200: 2020 2069 6620 6570 6f63 6820 2520 7365     if epoch % se
+00005210: 6c66 2e63 6667 2e43 4845 434b 504f 494e  lf.cfg.CHECKPOIN
+00005220: 545f 4652 4551 203d 3d20 303a 0d0a 2020  T_FREQ == 0:..  
+00005230: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00005240: 6c66 2e73 6176 655f 6368 6563 6b70 6f69  lf.save_checkpoi
+00005250: 6e74 2865 706f 6368 290d 0a20 2020 2020  nt(epoch)..     
+00005260: 2020 2020 2020 2069 6620 6570 6f63 6820         if epoch 
+00005270: 2520 7365 6c66 2e63 6667 2e45 5641 4c5f  % self.cfg.EVAL_
+00005280: 4652 4551 203d 3d20 303a 0d0a 2020 2020  FREQ == 0:..    
+00005290: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+000052a0: 656c 662e 6366 672e 4556 414c 5f56 414c  elf.cfg.EVAL_VAL
+000052b0: 4944 3a0d 0a20 2020 2020 2020 2020 2020  ID:..           
+000052c0: 2020 2020 2020 2020 2073 656c 662e 7661           self.va
+000052d0: 6c69 6428 6570 6f63 6829 0d0a 2020 2020  lid(epoch)..    
+000052e0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+000052f0: 656c 662e 6366 672e 4556 414c 5f54 4553  elf.cfg.EVAL_TES
+00005300: 543a 0d0a 2020 2020 2020 2020 2020 2020  T:..            
+00005310: 2020 2020 2020 2020 7365 6c66 2e74 6573          self.tes
+00005320: 7428 6570 6f63 6829 0d0a 2020 2020 2020  t(epoch)..      
+00005330: 2020 2020 2020 7365 6c66 2e63 6865 636b        self.check
+00005340: 5f62 6573 7428 6570 6f63 6829 0d0a 2020  _best(epoch)..  
+00005350: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
+00005360: 7465 7028 6570 6f63 6829 0d0a 2020 2020  tep(epoch)..    
+00005370: 2020 2020 2020 2020 7365 6c66 2e74 7261          self.tra
+00005380: 696e 2865 706f 6368 290d 0a0d 0a20 2020  in(epoch)....   
+00005390: 2020 2020 2073 656c 662e 7361 7665 2829       self.save()
+000053a0: 0d0a 0d0a 2020 2020 2020 2020 2320 6c61  ....        # la
+000053b0: 7374 2065 706f 6368 0d0a 2020 2020 2020  st epoch..      
+000053c0: 2020 7365 6c66 2e76 616c 6964 2873 656c    self.valid(sel
+000053d0: 662e 6366 672e 6570 6f63 6873 290d 0a20  f.cfg.epochs).. 
+000053e0: 2020 2020 2020 2073 656c 662e 7465 7374         self.test
+000053f0: 2873 656c 662e 6366 672e 6570 6f63 6873  (self.cfg.epochs
+00005400: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00005410: 6368 6563 6b5f 6265 7374 2873 656c 662e  check_best(self.
+00005420: 6366 672e 6570 6f63 6873 290d 0a20 2020  cfg.epochs)..   
+00005430: 2020 2020 2073 656c 662e 7374 6570 2873       self.step(s
+00005440: 656c 662e 6366 672e 6570 6f63 6873 290d  elf.cfg.epochs).
+00005450: 0a0d 0a20 2020 2020 2020 2073 656c 662e  ...        self.
+00005460: 7375 6d6d 6172 7928 290d 0a0d 0a20 2020  summary()....   
+00005470: 2020 2020 2073 656c 662e 6576 616c 5f61       self.eval_a
+00005480: 745f 6265 7374 2829 0d0a 0d0a 0d0a 636c  t_best()......cl
+00005490: 6173 7320 4164 6170 7465 723a 0d0a 2020  ass Adapter:..  
+000054a0: 2020 7222 2222 0d0a 2020 2020 5061 7261    r"""..    Para
+000054b0: 6d73 2074 756e 6572 2e0d 0a0d 0a20 2020  ms tuner.....   
+000054c0: 2046 6c6f 7773 3a0d 0a20 2020 202d 2d2d   Flows:..    ---
+000054d0: 2d2d 2d0d 0a20 2020 2031 2e20 636f 6d70  ---..    1. comp
+000054e0: 696c 653a 2063 6f6e 6669 6775 7265 2074  ile: configure t
+000054f0: 6865 2063 6f6d 6d61 6e64 2c20 656e 7669  he command, envi
+00005500: 726f 6e6d 656e 7473 2c20 616e 6420 7061  ronments, and pa
+00005510: 7261 6d65 7465 7273 2066 6f72 2074 7261  rameters for tra
+00005520: 696e 696e 672e 0d0a 2020 2020 322e 2061  ining...    2. a
+00005530: 6c6c 6f63 6174 6520 6465 7669 6365 7320  llocate devices 
+00005540: 666f 7220 7661 7269 6f75 7320 7061 7261  for various para
+00005550: 6d65 7465 7273 3a0d 0a20 2020 2020 2020  meters:..       
+00005560: 202d 2072 6567 6973 7465 7220 7468 6520   - register the 
+00005570: 4944 2c20 6c6f 6720 7061 7468 2c20 616e  ID, log path, an
+00005580: 6420 6465 7669 6365 2066 6972 7374 0d0a  d device first..
+00005590: 2020 2020 2020 2020 2d20 6578 6563 7574          - execut
+000055a0: 6520 7468 6520 636f 6d6d 616e 640d 0a20  e the command.. 
+000055b0: 2020 2020 2020 202d 2063 6f6c 6c65 6374         - collect
+000055c0: 2069 6e66 6f72 6d61 7469 6f6e 2066 726f   information fro
+000055d0: 6d20 7468 6520 6c6f 6720 7061 7468 2061  m the log path a
+000055e0: 6e64 206f 7574 7075 7420 746f 2054 656e  nd output to Ten
+000055f0: 736f 7242 6f61 7264 0d0a 2020 2020 2020  sorBoard..      
+00005600: 2020 2d20 7361 7665 2074 6865 2063 6865    - save the che
+00005610: 636b 706f 696e 740d 0a20 2020 2020 2020  ckpoint..       
+00005620: 202d 2072 656c 6561 7365 2074 6865 2063   - release the c
+00005630: 6f72 7265 7370 6f6e 6469 6e67 2064 6576  orresponding dev
+00005640: 6963 650d 0a0d 0a20 2020 2045 7861 6d70  ice....    Examp
+00005650: 6c65 733a 0d0a 2020 2020 2d2d 2d2d 2d2d  les:..    ------
+00005660: 2d2d 2d0d 0a20 2020 203e 3e3e 2063 6667  ---..    >>> cfg
+00005670: 203d 207b 2763 6f6d 6d61 6e64 273a 2027   = {'command': '
+00005680: 7079 7468 6f6e 2078 7878 2e70 7927 2c20  python xxx.py', 
+00005690: 2770 6172 616d 7327 3a20 7b27 6f70 7469  'params': {'opti
+000056a0: 6d69 7a65 7227 3a20 5b27 7367 6427 2c20  mizer': ['sgd', 
+000056b0: 2761 6461 6d27 5d7d 7d0d 0a20 2020 203e  'adam']}}..    >
+000056c0: 3e3e 2074 756e 6572 203d 2041 6461 7074  >> tuner = Adapt
+000056d0: 6572 2829 0d0a 2020 2020 3e3e 3e20 7475  er()..    >>> tu
+000056e0: 6e65 722e 636f 6d70 696c 6528 6366 6729  ner.compile(cfg)
+000056f0: 0d0a 2020 2020 3e3e 3e20 7475 6e65 722e  ..    >>> tuner.
+00005700: 6669 7428 290d 0a20 2020 2022 2222 0d0a  fit()..    """..
+00005710: 0d0a 2020 2020 6465 6620 5f5f 696e 6974  ..    def __init
+00005720: 5f5f 2873 656c 6629 202d 3e20 4e6f 6e65  __(self) -> None
+00005730: 3a0d 0a20 2020 2020 2020 2073 656c 662e  :..        self.
+00005740: 7061 7261 6d73 203d 205b 5d0d 0a20 2020  params = []..   
+00005750: 2020 2020 2073 656c 662e 7661 6c75 6573       self.values
+00005760: 203d 205b 5d0d 0a20 2020 2020 2020 2073   = []..        s
+00005770: 656c 662e 6465 7669 6365 7320 3d20 7475  elf.devices = tu
+00005780: 706c 6528 290d 0a0d 0a20 2020 2020 2020  ple()....       
+00005790: 2064 6566 2063 6c65 616e 2829 3a0d 0a20   def clean():.. 
+000057a0: 2020 2020 2020 2020 2020 2070 6172 656e             paren
+000057b0: 7420 3d20 7073 7574 696c 2e50 726f 6365  t = psutil.Proce
+000057c0: 7373 286f 732e 6765 7470 6964 2829 290d  ss(os.getpid()).
+000057d0: 0a20 2020 2020 2020 2020 2020 2063 6869  .            chi
+000057e0: 6c64 7265 6e20 3d20 7061 7265 6e74 2e63  ldren = parent.c
+000057f0: 6869 6c64 7265 6e28 7265 6375 7273 6976  hildren(recursiv
+00005800: 653d 5472 7565 290d 0a20 2020 2020 2020  e=True)..       
+00005810: 2020 2020 2066 6f72 2070 726f 6365 7373       for process
+00005820: 2069 6e20 6368 696c 6472 656e 3a0d 0a20   in children:.. 
+00005830: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+00005840: 726f 6365 7373 2e73 656e 645f 7369 676e  rocess.send_sign
+00005850: 616c 2873 6967 6e61 6c2e 5349 4754 4552  al(signal.SIGTER
+00005860: 4d29 0d0a 2020 2020 2020 2020 2020 2020  M)..            
+00005870: 7073 7574 696c 2e77 6169 745f 7072 6f63  psutil.wait_proc
+00005880: 7328 6368 696c 6472 656e 2c20 7469 6d65  s(children, time
+00005890: 6f75 743d 3529 0d0a 0d0a 2020 2020 2020  out=5)....      
+000058a0: 2020 6174 6578 6974 2e72 6567 6973 7465    atexit.registe
+000058b0: 7228 636c 6561 6e29 0d0a 0d0a 2020 2020  r(clean)....    
+000058c0: 4070 726f 7065 7274 790d 0a20 2020 2064  @property..    d
+000058d0: 6566 2043 4f4d 4d41 4e44 2873 656c 6629  ef COMMAND(self)
+000058e0: 3a0d 0a20 2020 2020 2020 2072 6574 7572  :..        retur
+000058f0: 6e20 7365 6c66 2e63 6667 2e43 4f4d 4d41  n self.cfg.COMMA
+00005900: 4e44 0d0a 0d0a 2020 2020 6465 6620 7265  ND....    def re
+00005910: 6769 7374 6572 2873 656c 662c 2064 6576  gister(self, dev
+00005920: 6963 653a 2073 7472 2920 2d3e 2054 7570  ice: str) -> Tup
+00005930: 6c65 5b73 7472 2c20 7374 725d 3a0d 0a20  le[str, str]:.. 
+00005940: 2020 2020 2020 2073 656c 662e 6366 672e         self.cfg.
+00005950: 454e 5653 5b27 6964 275d 203d 2074 696d  ENVS['id'] = tim
+00005960: 652e 7374 7266 7469 6d65 2854 494d 4529  e.strftime(TIME)
+00005970: 0d0a 2020 2020 2020 2020 7365 6c66 2e63  ..        self.c
+00005980: 6667 2e45 4e56 535b 2764 6576 6963 6527  fg.ENVS['device'
+00005990: 5d20 3d20 6465 7669 6365 0d0a 2020 2020  ] = device..    
+000059a0: 2020 2020 636f 6d6d 616e 6420 3d20 7365      command = se
+000059b0: 6c66 2e43 4f4d 4d41 4e44 202b 2073 656c  lf.COMMAND + sel
+000059c0: 662e 6765 745f 6f70 7469 6f6e 2827 6964  f.get_option('id
+000059d0: 272c 2073 656c 662e 6366 672e 454e 5653  ', self.cfg.ENVS
+000059e0: 2e69 6429 0d0a 2020 2020 2020 2020 636f  .id)..        co
+000059f0: 6d6d 616e 6420 2b3d 2073 656c 662e 6765  mmand += self.ge
+00005a00: 745f 6f70 7469 6f6e 2827 6465 7669 6365  t_option('device
+00005a10: 272c 2073 656c 662e 6366 672e 454e 5653  ', self.cfg.ENVS
+00005a20: 2e64 6576 6963 6529 0d0a 2020 2020 2020  .device)..      
+00005a30: 2020 7265 7475 726e 2063 6f6d 6d61 6e64    return command
+00005a40: 2c20 7365 6c66 2e63 6667 2e45 4e56 532e  , self.cfg.ENVS.
+00005a50: 6964 2c20 7365 6c66 2e63 6667 2e4c 4f47  id, self.cfg.LOG
+00005a60: 5f50 4154 482e 666f 726d 6174 282a 2a73  _PATH.format(**s
+00005a70: 656c 662e 6366 672e 454e 5653 290d 0a0d  elf.cfg.ENVS)...
+00005a80: 0a20 2020 2040 7469 6d65 6d65 7465 7228  .    @timemeter(
+00005a90: 2241 6461 7074 6572 2f63 6f6d 7069 6c65  "Adapter/compile
+00005aa0: 2229 0d0a 2020 2020 6465 6620 636f 6d70  ")..    def comp
+00005ab0: 696c 6528 7365 6c66 2c20 6366 673a 2043  ile(self, cfg: C
+00005ac0: 6f6e 6669 6729 202d 3e20 4e6f 6e65 3a0d  onfig) -> None:.
+00005ad0: 0a20 2020 2020 2020 2072 2222 220d 0a20  .        r""".. 
+00005ae0: 2020 2020 2020 2043 6f6e 6669 6775 7265         Configure
+00005af0: 2074 6865 2063 6f6d 6d61 6e64 2c20 656e   the command, en
+00005b00: 7669 726f 6e6d 656e 7473 2c20 616e 6420  vironments, and 
+00005b10: 7061 7261 6d65 7465 7273 2066 6f72 2074  parameters for t
+00005b20: 7261 696e 696e 672e 0d0a 0d0a 2020 2020  raining.....    
+00005b30: 2020 2020 5061 7261 6d65 7465 7273 3a0d      Parameters:.
+00005b40: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
+00005b50: 2d2d 2d2d 0d0a 2020 2020 2020 2020 6366  ----..        cf
+00005b60: 6720 3a20 436f 6e66 6967 0d0a 2020 2020  g : Config..    
+00005b70: 2020 2020 2020 2020 416e 206f 626a 6563          An objec
+00005b80: 7420 7468 6174 2063 6f6e 7461 696e 7320  t that contains 
+00005b90: 7468 6520 636f 6d6d 616e 642c 2065 6e76  the command, env
+00005ba0: 6972 6f6e 6d65 6e74 732c 2070 6172 616d  ironments, param
+00005bb0: 6574 6572 732c 2061 6e64 2064 6566 6175  eters, and defau
+00005bc0: 6c74 732e 0d0a 0d0a 2020 2020 2020 2020  lts.....        
+00005bd0: 466c 6f77 733a 0d0a 2020 2020 2020 2020  Flows:..        
+00005be0: 2d2d 2d2d 2d2d 0d0a 2020 2020 2020 2020  ------..        
+00005bf0: 312e 2041 6464 2065 6e76 6972 6f6e 6d65  1. Add environme
+00005c00: 6e74 616c 2070 6172 616d 6574 6572 7320  ntal parameters 
+00005c10: 746f 2074 6865 2062 6173 6963 2060 636f  to the basic `co
+00005c20: 6d6d 616e 6460 2e0d 0a20 2020 2020 2020  mmand`...       
+00005c30: 2032 2e20 5265 6769 7374 6572 2061 6c6c   2. Register all
+00005c40: 2061 7661 696c 6162 6c65 2064 6576 6963   available devic
+00005c50: 6573 2e0d 0a20 2020 2020 2020 2033 2e20  es...        3. 
+00005c60: 436f 6e76 6572 7420 616c 6c20 7061 7261  Convert all para
+00005c70: 6d65 7465 7273 2066 726f 6d20 6063 6667  meters from `cfg
+00005c80: 2e50 4152 414d 5360 2e0d 0a20 2020 2020  .PARAMS`...     
+00005c90: 2020 2034 2e20 436f 6e76 6572 7420 616c     4. Convert al
+00005ca0: 6c20 6465 6661 756c 7473 2066 726f 6d20  l defaults from 
+00005cb0: 6063 6667 2e44 4546 4155 4c54 5360 2e0d  `cfg.DEFAULTS`..
+00005cc0: 0a0d 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
+00005cd0: 6e73 3a0d 0a20 2020 2020 2020 202d 2d2d  ns:..        ---
+00005ce0: 2d2d 2d2d 2d0d 0a20 2020 2020 2020 204e  -----..        N
+00005cf0: 6f6e 650d 0a20 2020 2020 2020 2022 2222  one..        """
+00005d00: 0d0a 2020 2020 2020 2020 7365 6c66 2e63  ..        self.c
+00005d10: 6667 203d 2063 6667 0d0a 2020 2020 2020  fg = cfg..      
+00005d20: 2020 7069 6563 6520 3d20 225c 747b 6b65    piece = "\t{ke
+00005d30: 797d 3a20 7b76 616c 737d 205c 6e22 0d0a  y}: {vals} \n"..
+00005d40: 2020 2020 2020 2020 656e 7673 2c20 7061          envs, pa
+00005d50: 7261 6d73 2c20 6465 6661 756c 7473 203d  rams, defaults =
+00005d60: 2022 222c 2022 222c 2022 220d 0a20 2020   "", "", ""..   
+00005d70: 2020 2020 2066 6f72 206b 6579 2c20 7661       for key, va
+00005d80: 6c20 696e 2073 656c 662e 6366 672e 454e  l in self.cfg.EN
+00005d90: 5653 2e69 7465 6d73 2829 3a0d 0a20 2020  VS.items():..   
+00005da0: 2020 2020 2020 2020 2069 6620 6b65 7920           if key 
+00005db0: 3d3d 2027 6465 7669 6365 273a 0d0a 2020  == 'device':..  
+00005dc0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00005dd0: 6c66 2e64 6576 6963 6573 203d 2074 7570  lf.devices = tup
+00005de0: 6c65 2876 616c 2e73 706c 6974 2827 2c27  le(val.split(','
+00005df0: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+00005e00: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
+00005e10: 2020 2020 2020 2073 656c 662e 6366 672e         self.cfg.
+00005e20: 434f 4d4d 414e 4420 2b3d 2073 656c 662e  COMMAND += self.
+00005e30: 6765 745f 6f70 7469 6f6e 286b 6579 2c20  get_option(key, 
+00005e40: 7661 6c29 0d0a 2020 2020 2020 2020 2020  val)..          
+00005e50: 2020 656e 7673 202b 3d20 7069 6563 652e    envs += piece.
+00005e60: 666f 726d 6174 286b 6579 3d6b 6579 2c20  format(key=key, 
+00005e70: 7661 6c73 3d76 616c 290d 0a20 2020 2020  vals=val)..     
+00005e80: 2020 2066 6f72 206b 6579 2c20 7661 6c73     for key, vals
+00005e90: 2069 6e20 7365 6c66 2e63 6667 2e50 4152   in self.cfg.PAR
+00005ea0: 414d 532e 6974 656d 7328 293a 0d0a 2020  AMS.items():..  
+00005eb0: 2020 2020 2020 2020 2020 6966 2069 7369            if isi
+00005ec0: 6e73 7461 6e63 6528 7661 6c73 2c20 2873  nstance(vals, (s
+00005ed0: 7472 2c20 696e 742c 2066 6c6f 6174 2929  tr, int, float))
+00005ee0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00005ef0: 2020 2076 616c 7320 3d20 5b76 616c 735d     vals = [vals]
+00005f00: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+00005f10: 6c66 2e64 6570 6c6f 795f 7061 7261 6d73  lf.deploy_params
+00005f20: 286b 6579 2c20 7661 6c73 290d 0a20 2020  (key, vals)..   
+00005f30: 2020 2020 2020 2020 2070 6172 616d 7320           params 
+00005f40: 2b3d 2070 6965 6365 2e66 6f72 6d61 7428  += piece.format(
+00005f50: 6b65 793d 6b65 792c 2076 616c 733d 7661  key=key, vals=va
+00005f60: 6c73 290d 0a20 2020 2020 2020 2066 6f72  ls)..        for
+00005f70: 206b 6579 2c20 7661 6c20 696e 2073 656c   key, val in sel
+00005f80: 662e 6366 672e 4445 4641 554c 5453 2e69  f.cfg.DEFAULTS.i
+00005f90: 7465 6d73 2829 3a0d 0a20 2020 2020 2020  tems():..       
+00005fa0: 2020 2020 2073 656c 662e 6366 672e 4445       self.cfg.DE
+00005fb0: 4641 554c 5453 5b6b 6579 5d20 3d20 7661  FAULTS[key] = va
+00005fc0: 6c0d 0a20 2020 2020 2020 2020 2020 2064  l..            d
+00005fd0: 6566 6175 6c74 7320 2b3d 2070 6965 6365  efaults += piece
+00005fe0: 2e66 6f72 6d61 7428 6b65 793d 6b65 792c  .format(key=key,
+00005ff0: 2076 616c 733d 7661 6c29 0d0a 0d0a 2020   vals=val)....  
+00006000: 2020 2020 2020 6366 675f 696e 666f 7320        cfg_infos 
+00006010: 3d20 6622 636f 6d6d 616e 643a 207b 7365  = f"command: {se
+00006020: 6c66 2e63 6667 2e43 4f4d 4d41 4e44 7d20  lf.cfg.COMMAND} 
+00006030: 5c6e 656e 7673 3a20 5c6e 7b65 6e76 737d  \nenvs: \n{envs}
+00006040: 7061 7261 6d73 3a20 5c6e 7b70 6172 616d  params: \n{param
+00006050: 737d 6465 6661 756c 7473 3a20 5c6e 7b64  s}defaults: \n{d
+00006060: 6566 6175 6c74 737d 220d 0a20 2020 2020  efaults}"..     
+00006070: 2020 2069 6e66 6f4c 6f67 6765 7228 6622     infoLogger(f"
+00006080: 5c30 3333 5b30 3b33 313b 3437 6d7b 6366  \033[0;31;47m{cf
+00006090: 675f 696e 666f 737d 5c30 3333 5b30 6d22  g_infos}\033[0m"
+000060a0: 290d 0a20 2020 2020 2020 200d 0a0d 0a20  )..        .... 
+000060b0: 2020 2064 6566 2064 6570 6c6f 795f 7061     def deploy_pa
+000060c0: 7261 6d73 2873 656c 662c 206b 6579 3a20  rams(self, key: 
+000060d0: 7374 722c 2076 616c 733a 2049 7465 7261  str, vals: Itera
+000060e0: 626c 6529 3a0d 0a20 2020 2020 2020 2073  ble):..        s
+000060f0: 656c 662e 7061 7261 6d73 2e61 7070 656e  elf.params.appen
+00006100: 6428 6b65 7929 0d0a 2020 2020 2020 2020  d(key)..        
+00006110: 7365 6c66 2e76 616c 7565 732e 6170 7065  self.values.appe
+00006120: 6e64 2876 616c 7329 0d0a 0d0a 2020 2020  nd(vals)....    
+00006130: 4073 7461 7469 636d 6574 686f 640d 0a20  @staticmethod.. 
+00006140: 2020 2064 6566 2067 6574 5f6f 7074 696f     def get_optio
+00006150: 6e28 6b65 793a 2073 7472 2c20 7661 6c3a  n(key: str, val:
+00006160: 2041 6e79 293a 0d0a 2020 2020 2020 2020   Any):..        
+00006170: 7222 2222 0d0a 2020 2020 2020 2020 436f  r"""..        Co
+00006180: 6e76 6572 7420 286b 6579 2c20 7661 6c29  nvert (key, val)
+00006190: 2074 6f20 272d 2d6b 6579 3d76 616c 272e   to '--key=val'.
+000061a0: 0d0a 0d0a 2020 2020 2020 2020 5061 7261  ....        Para
+000061b0: 6d65 7465 7273 3a0d 0a20 2020 2020 2020  meters:..       
+000061c0: 202d 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a 2020   -----------..  
+000061d0: 2020 2020 2020 6b65 7920 3a20 7374 720d        key : str.
+000061e0: 0a20 2020 2020 2020 2020 2020 2054 6865  .            The
+000061f0: 206b 6579 206f 6620 7468 6520 7061 7261   key of the para
+00006200: 6d65 7465 722e 0d0a 2020 2020 2020 2020  meter...        
+00006210: 7661 6c20 3a20 416e 790d 0a20 2020 2020  val : Any..     
+00006220: 2020 2020 2020 2054 6865 2076 616c 7565         The value
+00006230: 206f 6620 7468 6520 7061 7261 6d65 7465   of the paramete
+00006240: 722e 0d0a 0d0a 2020 2020 2020 2020 4e6f  r.....        No
+00006250: 7465 733a 0d0a 2020 2020 2020 2020 2d2d  tes:..        --
+00006260: 2d2d 2d2d 0d0a 2020 2020 2020 2020 416c  ----..        Al
+00006270: 6c20 275f 2720 696e 2060 6b65 7960 2077  l '_' in `key` w
+00006280: 696c 6c20 6265 2072 6570 6c61 6365 6420  ill be replaced 
+00006290: 6279 2027 2d27 2e0d 0a0d 0a20 2020 2020  by '-'.....     
+000062a0: 2020 2052 6574 7572 6e73 3a0d 0a20 2020     Returns:..   
+000062b0: 2020 2020 202d 2d2d 2d2d 2d2d 2d0d 0a20       --------.. 
+000062c0: 2020 2020 2020 2073 7472 0d0a 2020 2020         str..    
+000062d0: 2020 2020 2020 2020 5468 6520 7061 7261          The para
+000062e0: 6d65 7465 7220 7769 7468 2066 6f72 6d61  meter with forma
+000062f0: 7420 272d 2d6b 6579 3d76 616c 272e 0d0a  t '--key=val'...
+00006300: 0d0a 2020 2020 2020 2020 4578 616d 706c  ..        Exampl
+00006310: 6573 3a0d 0a20 2020 2020 2020 202d 2d2d  es:..        ---
+00006320: 2d2d 2d2d 2d2d 0d0a 2020 2020 2020 2020  ------..        
+00006330: 3e3e 3e20 4164 6170 7465 722e 6765 745f  >>> Adapter.get_
+00006340: 6f70 7469 6f6e 2827 6c72 272c 2027 3165  option('lr', '1e
+00006350: 2d33 2729 0d0a 2020 2020 2020 2020 272d  -3')..        '-
+00006360: 2d6c 723d 3165 2d33 270d 0a20 2020 2020  -lr=1e-3'..     
+00006370: 2020 203e 3e3e 2041 6461 7074 6572 2e67     >>> Adapter.g
+00006380: 6574 5f6f 7074 696f 6e28 276c 6561 726e  et_option('learn
+00006390: 696e 675f 7261 7465 272c 2027 3165 2d33  ing_rate', '1e-3
+000063a0: 2729 0d0a 2020 2020 2020 2020 272d 2d6c  ')..        '--l
+000063b0: 6561 726e 696e 672d 7261 7465 3d31 652d  earning-rate=1e-
+000063c0: 3327 0d0a 2020 2020 2020 2020 2222 220d  3'..        """.
+000063d0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+000063e0: 6622 202d 2d7b 6b65 792e 7265 706c 6163  f" --{key.replac
+000063f0: 6528 275f 272c 2027 2d27 297d 3d7b 7661  e('_', '-')}={va
+00006400: 6c7d 220d 0a0d 0a20 2020 2064 6566 206c  l}"....    def l
+00006410: 6f61 645f 6265 7374 2873 656c 662c 206c  oad_best(self, l
+00006420: 6f67 5061 7468 3a20 7374 7229 3a0d 0a20  ogPath: str):.. 
+00006430: 2020 2020 2020 2022 2222 4c6f 6164 2062         """Load b
+00006440: 6573 742e 7069 636b 6c65 2066 726f 6d20  est.pickle from 
+00006450: 6c6f 6750 6174 6820 6f66 2063 6f72 7265  logPath of corre
+00006460: 7370 6f6e 6469 6e67 2e22 2222 0d0a 2020  sponding."""..  
+00006470: 2020 2020 2020 6669 6c65 5f20 3d20 6f73        file_ = os
+00006480: 2e70 6174 682e 6a6f 696e 286c 6f67 5061  .path.join(logPa
+00006490: 7468 2c20 7365 6c66 2e63 6667 2e44 4154  th, self.cfg.DAT
+000064a0: 415f 4449 522c 2073 656c 662e 6366 672e  A_DIR, self.cfg.
+000064b0: 4d4f 4e49 544f 525f 4245 5354 5f46 494c  MONITOR_BEST_FIL
+000064c0: 454e 414d 4529 0d0a 2020 2020 2020 2020  ENAME)..        
+000064d0: 7265 7475 726e 2069 6d70 6f72 745f 7069  return import_pi
+000064e0: 636b 6c65 2866 696c 655f 290d 0a0d 0a20  ckle(file_).... 
+000064f0: 2020 2064 6566 2077 7269 7465 2873 656c     def write(sel
+00006500: 662c 2069 645f 3a20 7374 722c 206c 6f67  f, id_: str, log
+00006510: 5061 7468 3a20 7374 722c 2070 6172 616d  Path: str, param
+00006520: 733a 2044 6963 7429 3a0d 0a20 2020 2020  s: Dict):..     
+00006530: 2020 2072 2222 220d 0a20 2020 2020 2020     r"""..       
+00006540: 2057 7269 7465 2065 7870 6572 696d 656e   Write experimen
+00006550: 7420 7265 7375 6c74 7320 746f 2074 656e  t results to ten
+00006560: 736f 7262 6f61 7264 2e0d 0a0d 0a20 2020  sorboard.....   
+00006570: 2020 2020 2050 6172 616d 6574 6572 733a       Parameters:
+00006580: 0d0a 2020 2020 2020 2020 2d2d 2d2d 2d2d  ..        ------
+00006590: 2d2d 2d2d 2d0d 0a20 2020 2020 2020 2069  -----..        i
+000065a0: 645f 3a20 7374 720d 0a20 2020 2020 2020  d_: str..       
+000065b0: 2020 2020 2045 7870 6572 696d 656e 7420       Experiment 
+000065c0: 4944 2e0d 0a20 2020 2020 2020 206c 6f67  ID...        log
+000065d0: 5061 7468 3a20 7374 720d 0a20 2020 2020  Path: str..     
+000065e0: 2020 2020 2020 2050 6174 6820 746f 2074         Path to t
+000065f0: 6865 2065 7870 6572 696d 656e 7420 6c6f  he experiment lo
+00006600: 6773 2e0d 0a20 2020 2020 2020 2070 6172  gs...        par
+00006610: 616d 733a 2044 6963 740d 0a20 2020 2020  ams: Dict..     
+00006620: 2020 2020 2020 2043 6f6e 6669 6775 7261         Configura
+00006630: 7469 6f6e 2070 6172 616d 6574 6572 7320  tion parameters 
+00006640: 6f66 2074 6865 2065 7870 6572 696d 656e  of the experimen
+00006650: 742e 0d0a 0d0a 2020 2020 2020 2020 466c  t.....        Fl
+00006660: 6f77 733a 0d0a 2020 2020 2020 2020 2d2d  ows:..        --
+00006670: 2d2d 2d2d 0d0a 2020 2020 2020 2020 312e  ----..        1.
+00006680: 204c 6f61 6420 7468 6520 6265 7374 2064   Load the best d
+00006690: 6174 6120 6672 6f6d 2060 6c6f 6750 6174  ata from `logPat
+000066a0: 6860 2e0d 0a20 2020 2020 2020 2032 2e20  h`...        2. 
+000066b0: 5772 6974 6520 7468 6520 6265 7374 2064  Write the best d
+000066c0: 6174 6120 746f 2074 656e 736f 7262 6f61  ata to tensorboa
+000066d0: 7264 2077 6974 6820 6070 6172 616d 7360  rd with `params`
+000066e0: 2e0d 0a0d 0a20 2020 2020 2020 204e 6f74  .....        Not
+000066f0: 6573 3a0d 0a20 2020 2020 2020 202d 2d2d  es:..        ---
+00006700: 2d2d 2d0d 0a20 2020 2020 2020 2049 6620  ---..        If 
+00006710: 796f 7520 6669 6e64 2060 2d31 6020 6170  you find `-1` ap
+00006720: 7065 6172 696e 6720 696e 2074 6865 2074  pearing in the t
+00006730: 656e 736f 7262 6f61 7264 2c0d 0a20 2020  ensorboard,..   
+00006740: 2020 2020 2069 7420 636f 756c 6420 6d65       it could me
+00006750: 616e 2074 6861 7420 7468 6520 6461 7461  an that the data
+00006760: 2069 7320 6f66 2060 7374 7260 2074 7970   is of `str` typ
+00006770: 652c 0d0a 2020 2020 2020 2020 7768 6963  e,..        whic
+00006780: 6820 7769 6c6c 2063 6175 7365 2061 6e20  h will cause an 
+00006790: 6572 726f 7220 6966 2069 7420 6973 2073  error if it is s
+000067a0: 656e 7420 746f 2074 656e 736f 7262 6f61  ent to tensorboa
+000067b0: 7264 2064 6972 6563 746c 7921 0d0a 2020  rd directly!..  
+000067c0: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
+000067d0: 2020 2074 7279 3a0d 0a20 2020 2020 2020     try:..       
+000067e0: 2020 2020 2064 6174 6120 3d20 7365 6c66       data = self
+000067f0: 2e6c 6f61 645f 6265 7374 286c 6f67 5061  .load_best(logPa
+00006800: 7468 290d 0a20 2020 2020 2020 2020 2020  th)..           
+00006810: 2070 6174 6820 3d20 6f73 2e70 6174 682e   path = os.path.
+00006820: 6a6f 696e 2873 656c 662e 6366 672e 434f  join(self.cfg.CO
+00006830: 5245 5f4c 4f47 5f50 4154 482c 2069 645f  RE_LOG_PATH, id_
+00006840: 290d 0a20 2020 2020 2020 2020 2020 2077  )..            w
+00006850: 6974 6820 5375 6d6d 6172 7957 7269 7465  ith SummaryWrite
+00006860: 7228 6c6f 675f 6469 723d 7061 7468 2920  r(log_dir=path) 
+00006870: 6173 2077 7269 7465 723a 0d0a 2020 2020  as writer:..    
+00006880: 2020 2020 2020 2020 2020 2020 6d65 7472              metr
+00006890: 6963 7320 3d20 6469 6374 2829 0d0a 2020  ics = dict()..  
+000068a0: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+000068b0: 7220 7072 6566 6978 2c20 6265 7374 2069  r prefix, best i
+000068c0: 6e20 6461 7461 2e69 7465 6d73 2829 3a0d  n data.items():.
+000068d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000068e0: 2020 2020 2066 6f72 206d 6574 7269 632c       for metric,
+000068f0: 2076 616c 2069 6e20 6265 7374 2e69 7465   val in best.ite
+00006900: 6d73 2829 3a0d 0a20 2020 2020 2020 2020  ms():..         
+00006910: 2020 2020 2020 2020 2020 2020 2020 2076                 v
+00006920: 616c 203d 2076 616c 2069 6620 6973 696e  al = val if isin
+00006930: 7374 616e 6365 2876 616c 2c20 2869 6e74  stance(val, (int
+00006940: 2c20 666c 6f61 7429 2920 656c 7365 202d  , float)) else -
+00006950: 310d 0a20 2020 2020 2020 2020 2020 2020  1..             
+00006960: 2020 2020 2020 2020 2020 206d 6574 7269             metri
+00006970: 6373 5b27 2f27 2e6a 6f69 6e28 5b70 7265  cs['/'.join([pre
+00006980: 6669 782c 206d 6574 7269 635d 295d 203d  fix, metric])] =
+00006990: 2076 616c 0d0a 2020 2020 2020 2020 2020   val..          
+000069a0: 2020 2020 2020 7772 6974 6572 2e61 6464        writer.add
+000069b0: 5f68 7061 7261 6d73 280d 0a20 2020 2020  _hparams(..     
+000069c0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+000069d0: 6172 616d 732c 206d 6574 7269 6373 2c0d  arams, metrics,.
+000069e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000069f0: 2029 0d0a 2020 2020 2020 2020 6578 6365   )..        exce
+00006a00: 7074 2045 7863 6570 7469 6f6e 3a0d 0a20  pt Exception:.. 
+00006a10: 2020 2020 2020 2020 2020 2069 6e66 6f4c             infoL
+00006a20: 6f67 6765 7228 0d0a 2020 2020 2020 2020  ogger(..        
+00006a30: 2020 2020 2020 2020 6622 5c30 3333 5b30          f"\033[0
+00006a40: 3b33 313b 3437 6d5b 4164 6170 7465 725d  ;31;47m[Adapter]
+00006a50: 203e 3e3e 2055 6e6b 6e6f 776e 2065 7272   >>> Unknown err
+00006a60: 6f72 7320 6861 7070 656e 2e20 5468 6973  ors happen. This
+00006a70: 2069 7320 6d61 696e 6c79 2064 7565 2074   is mainly due t
+00006a80: 6f20 6162 6e6f 726d 616c 2065 7869 7473  o abnormal exits
+00006a90: 206f 6620 6368 696c 6420 7072 6f63 6573   of child proces
+00006aa0: 7365 732e 5c30 3333 5b30 6d22 0d0a 2020  ses.\033[0m"..  
+00006ab0: 2020 2020 2020 2020 2020 290d 0a0d 0a20            ).... 
+00006ac0: 2020 2064 6566 2065 6163 685f 6772 6964     def each_grid
+00006ad0: 2873 656c 6629 3a0d 0a20 2020 2020 2020  (self):..       
+00006ae0: 2022 2222 4772 6964 2073 6561 7263 6820   """Grid search 
+00006af0: 666f 7220 6561 6368 206b 696e 6420 6f66  for each kind of
+00006b00: 2070 6172 616d 2e22 2222 0d0a 2020 2020   param."""..    
+00006b10: 2020 2020 666f 7220 6b65 792c 2076 616c      for key, val
+00006b20: 7320 696e 207a 6970 2873 656c 662e 7061  s in zip(self.pa
+00006b30: 7261 6d73 2c20 7365 6c66 2e76 616c 7565  rams, self.value
+00006b40: 7329 3a0d 0a20 2020 2020 2020 2020 2020  s):..           
+00006b50: 2066 6f72 2076 616c 2069 6e20 7661 6c73   for val in vals
+00006b60: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00006b70: 2020 2079 6965 6c64 2073 656c 662e 6366     yield self.cf
+00006b80: 672e 4445 4641 554c 5453 207c 207b 6b65  g.DEFAULTS | {ke
+00006b90: 793a 2076 616c 7d0d 0a0d 0a20 2020 2064  y: val}....    d
+00006ba0: 6566 2070 726f 6475 6374 5f67 7269 6428  ef product_grid(
+00006bb0: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
+00006bc0: 2222 2247 7269 6420 7365 6172 6368 2061  """Grid search a
+00006bd0: 6372 6f73 7320 616c 6c20 636f 6d62 696e  cross all combin
+00006be0: 6174 696f 6e20 6f66 2070 6172 616d 7322  ation of params"
+00006bf0: 2222 0d0a 2020 2020 2020 2020 666f 7220  ""..        for 
+00006c00: 7661 6c73 2069 6e20 7072 6f64 7563 7428  vals in product(
+00006c10: 2a73 656c 662e 7661 6c75 6573 293a 0d0a  *self.values):..
+00006c20: 2020 2020 2020 2020 2020 2020 7969 656c              yiel
+00006c30: 6420 7365 6c66 2e63 6667 2e44 4546 4155  d self.cfg.DEFAU
+00006c40: 4c54 5320 7c20 7b6f 7074 696f 6e3a 7661  LTS | {option:va
+00006c50: 6c20 666f 7220 6f70 7469 6f6e 2c20 7661  l for option, va
+00006c60: 6c20 696e 207a 6970 2873 656c 662e 7061  l in zip(self.pa
+00006c70: 7261 6d73 2c20 7661 6c73 297d 0d0a 0d0a  rams, vals)}....
+00006c80: 2020 2020 6465 6620 7361 7665 5f63 6865      def save_che
+00006c90: 636b 706f 696e 7428 7365 6c66 2c20 736f  ckpoint(self, so
+00006ca0: 7572 6365 3a20 4c69 7374 2920 2d3e 204e  urce: List) -> N
+00006cb0: 6f6e 653a 0d0a 2020 2020 2020 2020 2222  one:..        ""
+00006cc0: 2253 6176 6520 7468 6520 7265 7374 206f  "Save the rest o
+00006cd0: 6620 7061 7261 6d73 2e22 2222 0d0a 2020  f params."""..  
+00006ce0: 2020 2020 2020 7061 7468 203d 206f 732e        path = os.
+00006cf0: 7061 7468 2e6a 6f69 6e28 7365 6c66 2e63  path.join(self.c
+00006d00: 6667 2e43 4f52 455f 4348 4543 4b50 4f49  fg.CORE_CHECKPOI
+00006d10: 4e54 5f50 4154 482c 2073 656c 662e 6366  NT_PATH, self.cf
+00006d20: 672e 4348 4543 4b50 4f49 4e54 5f46 494c  g.CHECKPOINT_FIL
+00006d30: 454e 414d 4529 0d0a 2020 2020 2020 2020  ENAME)..        
+00006d40: 6368 6563 6b70 6f69 6e74 203d 2064 6963  checkpoint = dic
+00006d50: 7428 290d 0a20 2020 2020 2020 2063 6865  t()..        che
+00006d60: 636b 706f 696e 745b 2773 6f75 7263 6527  ckpoint['source'
+00006d70: 5d20 3d20 736f 7572 6365 0d0a 2020 2020  ] = source..    
+00006d80: 2020 2020 746f 7263 682e 7361 7665 2863      torch.save(c
+00006d90: 6865 636b 706f 696e 742c 2070 6174 6829  heckpoint, path)
+00006da0: 0d0a 0d0a 2020 2020 6465 6620 6c6f 6164  ....    def load
+00006db0: 5f63 6865 636b 706f 696e 7428 7365 6c66  _checkpoint(self
+00006dc0: 2920 2d3e 2069 6e74 3a0d 0a20 2020 2020  ) -> int:..     
+00006dd0: 2020 2022 2222 4c6f 6164 2074 6865 2072     """Load the r
+00006de0: 6573 7420 6f66 2070 6172 616d 732e 2222  est of params.""
+00006df0: 220d 0a20 2020 2020 2020 2070 6174 6820  "..        path 
+00006e00: 3d20 6f73 2e70 6174 682e 6a6f 696e 2873  = os.path.join(s
+00006e10: 656c 662e 6366 672e 434f 5245 5f43 4845  elf.cfg.CORE_CHE
+00006e20: 434b 504f 494e 545f 5041 5448 2c20 7365  CKPOINT_PATH, se
+00006e30: 6c66 2e63 6667 2e43 4845 434b 504f 494e  lf.cfg.CHECKPOIN
+00006e40: 545f 4649 4c45 4e41 4d45 290d 0a20 2020  T_FILENAME)..   
+00006e50: 2020 2020 2063 6865 636b 706f 696e 7420       checkpoint 
+00006e60: 3d20 746f 7263 682e 6c6f 6164 2870 6174  = torch.load(pat
+00006e70: 6829 0d0a 2020 2020 2020 2020 7265 7475  h)..        retu
+00006e80: 726e 2063 6865 636b 706f 696e 745b 2773  rn checkpoint['s
+00006e90: 6f75 7263 6527 5d0d 0a0d 0a20 2020 2040  ource']....    @
+00006ea0: 7469 6d65 6d65 7465 7228 2243 6f61 6368  timemeter("Coach
+00006eb0: 2f72 6573 756d 6522 290d 0a20 2020 2064  /resume")..    d
+00006ec0: 6566 2072 6573 756d 6528 7365 6c66 293a  ef resume(self):
+00006ed0: 0d0a 2020 2020 2020 2020 2222 2252 6573  ..        """Res
+00006ee0: 756d 6520 6672 6f6d 2074 6865 2072 6563  ume from the rec
+00006ef0: 656e 7420 6368 6563 6b70 6f69 6e74 2e22  ent checkpoint."
+00006f00: 2222 0d0a 2020 2020 2020 2020 736f 7572  ""..        sour
+00006f10: 6365 203d 2073 656c 662e 6561 6368 5f67  ce = self.each_g
+00006f20: 7269 6428 2920 6966 2073 656c 662e 6366  rid() if self.cf
+00006f30: 672e 4558 434c 5553 4956 4520 656c 7365  g.EXCLUSIVE else
+00006f40: 2073 656c 662e 7072 6f64 7563 745f 6772   self.product_gr
+00006f50: 6964 2829 0d0a 2020 2020 2020 2020 736f  id()..        so
+00006f60: 7572 6365 203d 206c 6973 7428 736f 7572  urce = list(sour
+00006f70: 6365 295b 3a3a 2d31 5d0d 0a20 2020 2020  ce)[::-1]..     
+00006f80: 2020 2073 6f75 7263 6520 3d20 7365 6c66     source = self
+00006f90: 2e6c 6f61 645f 6368 6563 6b70 6f69 6e74  .load_checkpoint
+00006fa0: 2829 2069 6620 7365 6c66 2e63 6667 2e72  () if self.cfg.r
+00006fb0: 6573 756d 6520 656c 7365 2073 6f75 7263  esume else sourc
+00006fc0: 650d 0a20 2020 2020 2020 2069 6e66 6f4c  e..        infoL
+00006fd0: 6f67 6765 7228 6622 5b43 6f61 6368 5d20  ogger(f"[Coach] 
+00006fe0: 3e3e 3e20 4c6f 6164 2074 6865 2072 6563  >>> Load the rec
+00006ff0: 656e 7420 6368 6563 6b70 6f69 6e74 202e  ent checkpoint .
+00007000: 2e2e 2229 0d0a 2020 2020 2020 2020 7265  ..")..        re
+00007010: 7475 726e 2073 6f75 7263 650d 0a0d 0a20  turn source.... 
+00007020: 2020 2064 6566 2072 756e 2873 656c 662c     def run(self,
+00007030: 2063 6f6d 6d61 6e64 3a20 7374 722c 2070   command: str, p
+00007040: 6172 616d 733a 2044 6963 7429 3a0d 0a20  arams: Dict):.. 
+00007050: 2020 2020 2020 2022 2222 5374 6172 7420         """Start 
+00007060: 6120 6e65 7720 7375 6270 726f 6365 7373  a new subprocess
+00007070: 2222 220d 0a20 2020 2020 2020 2066 6f72  """..        for
+00007080: 206f 7074 696f 6e2c 2076 616c 2069 6e20   option, val in 
+00007090: 7061 7261 6d73 2e69 7465 6d73 2829 3a0d  params.items():.
+000070a0: 0a20 2020 2020 2020 2020 2020 2063 6f6d  .            com
+000070b0: 6d61 6e64 202b 3d20 7365 6c66 2e67 6574  mand += self.get
+000070c0: 5f6f 7074 696f 6e28 6f70 7469 6f6e 2c20  _option(option, 
+000070d0: 7661 6c29 0d0a 2020 2020 2020 2020 696e  val)..        in
+000070e0: 666f 4c6f 6767 6572 2866 225c 3033 335b  foLogger(f"\033[
+000070f0: 303b 3331 3b34 376d 7b63 6f6d 6d61 6e64  0;31;47m{command
+00007100: 7d5c 3033 335b 306d 2229 0d0a 2020 2020  }\033[0m")..    
+00007110: 2020 2020 7265 7475 726e 2073 7562 7072      return subpr
+00007120: 6f63 6573 732e 506f 7065 6e28 7368 6c65  ocess.Popen(shle
+00007130: 782e 7370 6c69 7428 636f 6d6d 616e 6429  x.split(command)
+00007140: 290d 0a0d 0a20 2020 2064 6566 2077 6169  )....    def wai
+00007150: 7428 7365 6c66 2c20 7461 736b 733a 204c  t(self, tasks: L
+00007160: 6973 7429 3a0d 0a20 2020 2020 2020 2022  ist):..        "
+00007170: 2222 5761 6974 2075 7469 6c20 616c 6c20  ""Wait util all 
+00007180: 7072 6f63 6573 7365 7320 7465 726d 696e  processes termin
+00007190: 6174 652e 2222 220d 0a20 2020 2020 2020  ate."""..       
+000071a0: 2074 6173 6b73 203d 205b 7461 736b 2066   tasks = [task f
+000071b0: 6f72 2074 6173 6b20 696e 2074 6173 6b73  or task in tasks
+000071c0: 2069 6620 7461 736b 2069 7320 6e6f 7420   if task is not 
+000071d0: 4e6f 6e65 5d0d 0a20 2020 2020 2020 2066  None]..        f
+000071e0: 6f72 2070 726f 6365 7373 5f2c 2069 645f  or process_, id_
+000071f0: 2c20 6c6f 6750 6174 682c 2070 6172 616d  , logPath, param
+00007200: 7320 696e 2074 6173 6b73 3a0d 0a20 2020  s in tasks:..   
+00007210: 2020 2020 2020 2020 2070 726f 6365 7373           process
+00007220: 5f2e 7761 6974 2829 0d0a 2020 2020 2020  _.wait()..      
+00007230: 2020 2020 2020 7365 6c66 2e77 7269 7465        self.write
+00007240: 2869 645f 2c20 6c6f 6750 6174 682c 2070  (id_, logPath, p
+00007250: 6172 616d 7329 0d0a 0d0a 2020 2020 6465  arams)....    de
+00007260: 6620 706f 6c6c 2873 656c 662c 2074 6173  f poll(self, tas
+00007270: 6b73 3a20 4c69 7374 293a 0d0a 2020 2020  ks: List):..    
+00007280: 2020 2020 2222 2257 6169 7420 7574 696c      """Wait util
+00007290: 2061 6e79 2070 726f 6365 7373 2074 6572   any process ter
+000072a0: 6d69 6e61 7465 732e 2222 220d 0a20 2020  minates."""..   
+000072b0: 2020 2020 2064 6566 2069 735f 6e75 6c6c       def is_null
+000072c0: 2874 6173 6b29 3a0d 0a20 2020 2020 2020  (task):..       
+000072d0: 2020 2020 2072 6574 7572 6e20 7461 736b       return task
+000072e0: 2069 7320 4e6f 6e65 0d0a 2020 2020 2020   is None..      
+000072f0: 2020 6275 6666 6572 5f73 6f75 7263 6520    buffer_source 
+00007300: 3d20 5b74 6173 6b5b 2d31 5d20 666f 7220  = [task[-1] for 
+00007310: 7461 736b 2069 6e20 7461 736b 7320 6966  task in tasks if
+00007320: 2074 6173 6b20 6973 206e 6f74 204e 6f6e   task is not Non
+00007330: 655d 0d0a 2020 2020 2020 2020 7469 6d65  e]..        time
+00007340: 2e73 6c65 6570 2831 2920 2320 666f 7220  .sleep(1) # for 
+00007350: 756e 6971 7565 2069 640d 0a20 2020 2020  unique id..     
+00007360: 2020 2077 6869 6c65 206e 6f74 2061 6e79     while not any
+00007370: 286d 6170 2869 735f 6e75 6c6c 2c20 7461  (map(is_null, ta
+00007380: 736b 7329 293a 0d0a 2020 2020 2020 2020  sks)):..        
+00007390: 2020 2020 7469 6d65 2e73 6c65 6570 2837      time.sleep(7
+000073a0: 290d 0a20 2020 2020 2020 2020 2020 2062  )..            b
+000073b0: 7566 6665 725f 736f 7572 6365 203d 205b  uffer_source = [
+000073c0: 5d0d 0a20 2020 2020 2020 2020 2020 2066  ]..            f
+000073d0: 6f72 2069 2c20 2870 726f 6365 7373 5f2c  or i, (process_,
+000073e0: 2069 645f 2c20 6c6f 6750 6174 682c 2070   id_, logPath, p
+000073f0: 6172 616d 7329 2069 6e20 656e 756d 6572  arams) in enumer
+00007400: 6174 6528 7461 736b 7329 3a0d 0a20 2020  ate(tasks):..   
+00007410: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00007420: 7072 6f63 6573 735f 2e70 6f6c 6c28 2920  process_.poll() 
+00007430: 6973 206e 6f74 204e 6f6e 653a 0d0a 2020  is not None:..  
+00007440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007450: 2020 7365 6c66 2e77 7269 7465 2869 645f    self.write(id_
+00007460: 2c20 6c6f 6750 6174 682c 2070 6172 616d  , logPath, param
+00007470: 7329 0d0a 2020 2020 2020 2020 2020 2020  s)..            
+00007480: 2020 2020 2020 2020 7461 736b 735b 695d          tasks[i]
+00007490: 203d 204e 6f6e 650d 0a20 2020 2020 2020   = None..       
+000074a0: 2020 2020 2020 2020 2065 6c73 653a 0d0a           else:..
+000074b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000074c0: 2020 2020 6275 6666 6572 5f73 6f75 7263      buffer_sourc
+000074d0: 652e 6170 7065 6e64 2870 6172 616d 7329  e.append(params)
+000074e0: 0d0a 2020 2020 2020 2020 7365 6c66 2e73  ..        self.s
+000074f0: 6176 655f 6368 6563 6b70 6f69 6e74 2873  ave_checkpoint(s
+00007500: 656c 662e 736f 7572 6365 202b 2062 7566  elf.source + buf
+00007510: 6665 725f 736f 7572 6365 290d 0a20 2020  fer_source)..   
+00007520: 2020 2020 2072 6574 7572 6e20 7461 736b       return task
+00007530: 732e 696e 6465 7828 4e6f 6e65 290d 0a0d  s.index(None)...
+00007540: 0a20 2020 2064 6566 2074 6572 6d69 6e61  .    def termina
+00007550: 7465 2873 656c 662c 2074 6173 6b73 3a20  te(self, tasks: 
+00007560: 4c69 7374 293a 0d0a 2020 2020 2020 2020  List):..        
+00007570: 7461 736b 7320 3d20 5b74 6173 6b20 666f  tasks = [task fo
+00007580: 7220 7461 736b 2069 6e20 7461 736b 7320  r task in tasks 
+00007590: 6966 2074 6173 6b20 6973 206e 6f74 204e  if task is not N
+000075a0: 6f6e 655d 0d0a 2020 2020 2020 2020 666f  one]..        fo
+000075b0: 7220 7072 6f63 6573 735f 2c20 5f2c 205f  r process_, _, _
+000075c0: 2c20 5f20 696e 2074 6173 6b73 3a0d 0a20  , _ in tasks:.. 
+000075d0: 2020 2020 2020 2020 2020 2069 6620 7072             if pr
+000075e0: 6f63 6573 735f 2e70 6f6c 6c28 2920 6973  ocess_.poll() is
+000075f0: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
+00007600: 2020 2020 2020 2020 7072 6f63 6573 735f          process_
+00007610: 2e74 6572 6d69 6e61 7465 2829 0d0a 2020  .terminate()..  
+00007620: 2020 2020 2020 7469 6d65 2e73 6c65 6570        time.sleep
+00007630: 2833 290d 0a20 2020 2020 2020 2066 6f72  (3)..        for
+00007640: 2070 726f 6365 7373 5f2c 205f 2c20 5f2c   process_, _, _,
+00007650: 205f 2069 6e20 7461 736b 733a 0d0a 2020   _ in tasks:..  
+00007660: 2020 2020 2020 2020 2020 6966 2070 726f            if pro
+00007670: 6365 7373 5f2e 706f 6c6c 2829 2069 7320  cess_.poll() is 
+00007680: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2020  None:..         
+00007690: 2020 2020 2020 2070 726f 6365 7373 5f2e         process_.
+000076a0: 6b69 6c6c 2829 0d0a 2020 2020 2020 2020  kill()..        
+000076b0: 7379 732e 6578 6974 2829 0d0a 0d0a 2020  sys.exit()....  
+000076c0: 2020 4074 696d 656d 6574 6572 2822 4164    @timemeter("Ad
+000076d0: 6170 7465 722f 6669 7422 290d 0a20 2020  apter/fit")..   
+000076e0: 2064 6566 2066 6974 2873 656c 6629 3a0d   def fit(self):.
+000076f0: 0a20 2020 2020 2020 2022 2222 4772 6964  .        """Grid
+00007700: 2073 6561 7263 682e 2222 220d 0a20 2020   search."""..   
+00007710: 2020 2020 2073 656c 662e 736f 7572 6365       self.source
+00007720: 203d 2073 656c 662e 7265 7375 6d65 2829   = self.resume()
+00007730: 0d0a 2020 2020 2020 2020 7461 736b 7320  ..        tasks 
+00007740: 3d20 5b4e 6f6e 6520 666f 7220 5f20 696e  = [None for _ in
+00007750: 2072 616e 6765 286c 656e 2873 656c 662e   range(len(self.
+00007760: 6465 7669 6365 7329 295d 0d0a 0d0a 2020  devices))]....  
+00007770: 2020 2020 2020 6465 6620 7369 676e 616c        def signal
+00007780: 5f68 616e 646c 6572 2873 6967 2c20 6672  _handler(sig, fr
+00007790: 616d 6529 3a0d 0a20 2020 2020 2020 2020  ame):..         
+000077a0: 2020 2069 6e66 6f4c 6f67 6765 7228 6622     infoLogger(f"
+000077b0: 5c30 3333 5b30 3b33 313b 3437 6d3d 3d3d  \033[0;31;47m===
+000077c0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000077d0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 5445 524d  ============TERM
+000077e0: 494e 4154 4520 414c 4c20 5355 4250 524f  INATE ALL SUBPRO
+000077f0: 4345 5353 4553 3d3d 3d3d 3d3d 3d3d 3d3d  CESSES==========
+00007800: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00007810: 3d3d 3d3d 3d5c 3033 335b 306d 2229 0d0a  =====\033[0m")..
+00007820: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00007830: 2e74 6572 6d69 6e61 7465 2874 6173 6b73  .terminate(tasks
+00007840: 290d 0a20 2020 2020 2020 2073 6967 6e61  )..        signa
+00007850: 6c2e 7369 676e 616c 2873 6967 6e61 6c2e  l.signal(signal.
+00007860: 5349 4749 4e54 2c20 7369 676e 616c 5f68  SIGINT, signal_h
+00007870: 616e 646c 6572 290d 0a0d 0a20 2020 2020  andler)....     
+00007880: 2020 2074 7279 3a0d 0a20 2020 2020 2020     try:..       
+00007890: 2020 2020 2077 6869 6c65 2073 656c 662e       while self.
+000078a0: 736f 7572 6365 3a0d 0a20 2020 2020 2020  source:..       
+000078b0: 2020 2020 2020 2020 2069 6e64 6578 203d           index =
+000078c0: 2073 656c 662e 706f 6c6c 2874 6173 6b73   self.poll(tasks
+000078d0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+000078e0: 2020 2064 6576 6963 6520 3d20 7365 6c66     device = self
+000078f0: 2e64 6576 6963 6573 5b69 6e64 6578 5d0d  .devices[index].
+00007900: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007910: 2070 6172 616d 7320 3d20 7365 6c66 2e73   params = self.s
+00007920: 6f75 7263 652e 706f 7028 290d 0a20 2020  ource.pop()..   
+00007930: 2020 2020 2020 2020 2020 2020 2063 6f6d               com
+00007940: 6d61 6e64 2c20 6964 5f2c 206c 6f67 5061  mand, id_, logPa
+00007950: 7468 203d 2073 656c 662e 7265 6769 7374  th = self.regist
+00007960: 6572 2864 6576 6963 6529 0d0a 2020 2020  er(device)..    
+00007970: 2020 2020 2020 2020 2020 2020 7072 6f63              proc
+00007980: 6573 735f 203d 2073 656c 662e 7275 6e28  ess_ = self.run(
+00007990: 636f 6d6d 616e 642c 2070 6172 616d 7329  command, params)
+000079a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000079b0: 2020 7461 736b 735b 696e 6465 785d 203d    tasks[index] =
+000079c0: 2028 7072 6f63 6573 735f 2c20 6964 5f2c   (process_, id_,
+000079d0: 206c 6f67 5061 7468 2c20 7061 7261 6d73   logPath, params
+000079e0: 290d 0a20 2020 2020 2020 2065 7863 6570  )..        excep
+000079f0: 7420 4578 6365 7074 696f 6e20 6173 2065  t Exception as e
+00007a00: 3a0d 0a20 2020 2020 2020 2020 2020 2070  :..            p
+00007a10: 7269 6e74 2865 290d 0a20 2020 2020 2020  rint(e)..       
+00007a20: 2066 696e 616c 6c79 3a0d 0a20 2020 2020   finally:..     
+00007a30: 2020 2020 2020 2073 656c 662e 7761 6974         self.wait
+00007a40: 2874 6173 6b73 290d 0a20 2020 2020 2020  (tasks)..       
+00007a50: 2020 2020 2073 656c 662e 7465 726d 696e       self.termin
+00007a60: 6174 6528 7461 736b 7329                 ate(tasks)
```

### Comparing `freerec-0.3.1/freerec/metrics.py` & `freerec-0.3.5/freerec/metrics.py`

 * *Files identical despite different names*

### Comparing `freerec-0.3.1/freerec/models/base.py` & `freerec-0.3.5/freerec/models/base.py`

 * *Files identical despite different names*

### Comparing `freerec-0.3.1/freerec/parser.py` & `freerec-0.3.5/freerec/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,16 +147,16 @@
         """Add README.md to the path."""
         time_ = time.strftime("%Y-%m-%d-%H:%M:%S")
         file_ = os.path.join(path, "README.md")
         s = "|  {key}  |   {val}    |\n"
         info = "\n## {0} \n\n\n".format(time_)
         info += "|  Attribute   |   Value   |\n"
         info += "| :-------------: | :-----------: |\n"
-        for key, val in self.items():
-            info += s.format(key=key, val=val)
+        for key in sorted(self.keys(), key=lambda x: x.upper()):
+            info += s.format(key=key, val=self[key])
         with open(file_, mode, encoding="utf8") as fh:
             fh.write(info)
 
     def reset(self):
         self.clear()
         for key, val in CONFIG.items():
             self[key] = val
```

### Comparing `freerec-0.3.1/freerec/utils.py` & `freerec-0.3.5/freerec/utils.py`

 * *Files identical despite different names*

### Comparing `freerec-0.3.1/freerec.egg-info/PKG-INFO` & `freerec-0.3.5/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freerec
-Version: 0.3.1
+Version: 0.3.5
 Summary: PyTorch library for recommender systems
 Home-page: https://github.com/MTandHJ/freerec
 Author: MTandHJ
 Author-email: congxueric@gmail.com
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -20,14 +20,42 @@
 
 
 ## Requirements: 
 
 Python == 3.9 | [PyTorch == 1.12.1](https://pytorch.org/) | [TorchData == 0.4.1](https://github.com/pytorch/data) | [PyG](https://pytorch-geometric.readthedocs.io/en/latest/notes/installation.html#)
 
 
+```
+conda create --name=PyT12 python=3.9
+conda activate PyT12
+```
+
+```
+pip install torch==1.12.1+cu113 --extra-index-url https://download.pytorch.org/whl/cu113
+pip install torchdata==0.4.1
+```
+
+- Linux
+
+```
+pip install torch_geometric==2.1.0.post1
+pip install https://data.pyg.org/whl/torch-1.12.0%2Bcu116/torch_scatter-2.0.9-cp39-cp39-linux_x86_64.whl
+pip install https://data.pyg.org/whl/torch-1.12.0%2Bcu116/torch_sparse-0.6.15%2Bpt112cu116-cp39-cp39-linux_x86_64.whl
+```
+
+- Windows
+
+```
+pip install torch_geometric==2.1.0.post1
+pip install https://data.pyg.org/whl/torch-1.12.0%2Bcu116/torch_scatter-2.0.9-cp39-cp39-win_amd64.whl
+pip install https://data.pyg.org/whl/torch-1.12.0%2Bcu116/torch_sparse-0.6.15%2Bpt112cu116-cp39-cp39-win_amd64.whl
+```
+
+
+
 ## Installation
 
     pip install freerec
 
 or (for latest)
 
     pip install git+https://github.com/MTandHJ/freerec.git
```

### Comparing `freerec-0.3.1/freerec.egg-info/SOURCES.txt` & `freerec-0.3.5/freerec.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `freerec-0.3.1/setup.py` & `freerec-0.3.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,17 +5,19 @@
   long_description = fh.read()
 
 requires = [
     "torchdata==0.4.1",
     "torchmetrics>=0.9.2",
     "tqdm>=4.64.0",
     'scipy>=1.9.1',
-    "freeplot>=0.3.0",
+    "freeplot>=0.3.1",
     "PyYAML>=6.0",
     "tensorboard>=2.10.0",
+    "psutil>=5.9.0",
+    "prettytable>=3.4.1"
 ]
 
 
 def get_property(prop, project):
     result = re.search(r'{}\s*=\s*[\'"]([^\'"]*)[\'"]'.format(prop), open(project + '/__init__.py').read())
     return result.group(1)
```

