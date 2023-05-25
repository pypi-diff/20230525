# Comparing `tmp/EasyTCR-0.0.1.tar.gz` & `tmp/easyTCR-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "H:\tcr_pdata\package_tu\dist\.tmp-21i_gmlm\EasyTCR-0.0.1.tar", last modified: Thu May 25 04:21:09 2023, max compression
+gzip compressed data, was "H:\tcr_pdata\package_tu\dist\.tmp-e67g5mm6\easyTCR-0.0.2.tar", last modified: Thu May 25 05:18:10 2023, max compression
```

## Comparing `EasyTCR-0.0.1.tar` & `easyTCR-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 04:21:09.149749 EasyTCR-0.0.1/
--rw-rw-rw-   0        0        0     1091 2023-05-25 02:42:46.000000 EasyTCR-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      381 2023-05-25 04:21:09.149242 EasyTCR-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       11 2023-05-25 02:43:28.000000 EasyTCR-0.0.1/README.md
--rw-rw-rw-   0        0        0      539 2023-05-25 04:20:33.000000 EasyTCR-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-25 04:21:09.150277 EasyTCR-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-25 04:21:09.136506 EasyTCR-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-25 04:21:09.146198 EasyTCR-0.0.1/src/EasyTCR.egg-info/
--rw-rw-rw-   0        0        0      381 2023-05-25 04:21:09.000000 EasyTCR-0.0.1/src/EasyTCR.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      253 2023-05-25 04:21:09.000000 EasyTCR-0.0.1/src/EasyTCR.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 04:21:09.000000 EasyTCR-0.0.1/src/EasyTCR.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       91 2023-05-25 04:21:09.000000 EasyTCR-0.0.1/src/EasyTCR.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-25 04:21:09.000000 EasyTCR-0.0.1/src/EasyTCR.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-25 04:21:09.148733 EasyTCR-0.0.1/src/EazyTCR/
--rw-rw-rw-   0        0        0        2 2023-04-24 08:23:46.000000 EasyTCR-0.0.1/src/EazyTCR/__init__.py
--rw-rw-rw-   0        0        0    31500 2023-05-25 03:04:13.000000 EasyTCR-0.0.1/src/EazyTCR/easytcr.py
+drwxrwxrwx   0        0        0        0 2023-05-25 05:18:10.671660 easyTCR-0.0.2/
+-rw-rw-rw-   0        0        0     1091 2023-05-25 02:42:46.000000 easyTCR-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      381 2023-05-25 05:18:10.671151 easyTCR-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       11 2023-05-25 04:42:31.000000 easyTCR-0.0.2/README.md
+-rw-rw-rw-   0        0        0      539 2023-05-25 04:42:31.000000 easyTCR-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-25 05:18:10.672165 easyTCR-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-25 05:18:10.656157 easyTCR-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-05-25 05:18:10.665044 easyTCR-0.0.2/src/easyTCR/
+-rw-rw-rw-   0        0        0        2 2023-04-24 08:23:46.000000 easyTCR-0.0.2/src/easyTCR/__init__.py
+-rw-rw-rw-   0        0        0    31445 2023-05-25 05:17:20.000000 easyTCR-0.0.2/src/easyTCR/easytcr.py
+drwxrwxrwx   0        0        0        0 2023-05-25 05:18:10.670135 easyTCR-0.0.2/src/easyTCR.egg-info/
+-rw-rw-rw-   0        0        0      381 2023-05-25 05:18:10.000000 easyTCR-0.0.2/src/easyTCR.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      253 2023-05-25 05:18:10.000000 easyTCR-0.0.2/src/easyTCR.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 05:18:10.000000 easyTCR-0.0.2/src/easyTCR.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       91 2023-05-25 05:18:10.000000 easyTCR-0.0.2/src/easyTCR.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-25 05:18:10.000000 easyTCR-0.0.2/src/easyTCR.egg-info/top_level.txt
```

### Comparing `EasyTCR-0.0.1/LICENSE` & `easyTCR-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `EasyTCR-0.0.1/pyproject.toml` & `easyTCR-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
-name = "EasyTCR"
-version = "0.0.1"
+name = "easyTCR"
+version = "0.0.2"
 authors = [
   { name="gary", email="gary_dou327@163.com" },
 ]
 description = "Explore TCR repertoire"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `EasyTCR-0.0.1/src/EazyTCR/easytcr.py` & `easyTCR-0.0.2/src/easyTCR/easytcr.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,16 +5,14 @@
 import seaborn as sns
 import matplotlib.pyplot as plt
 from copy import deepcopy
 from typing import Callable, Union, Tuple
 from scipy.spatial.distance import squareform
 
 
-def load_test():
-    return np.load('test_data.npy')
 
 # 导入数据
 def tcr_load(filepath, process=True):
     """
     Example:
                     count          frac    vgene    jgene            cdr3aa
               0     120167  2.580886e-02   TRBV30  TRBJ2-7     CAWSRPPVHEQYF
```

