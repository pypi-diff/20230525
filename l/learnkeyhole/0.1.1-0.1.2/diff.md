# Comparing `tmp/learnkeyhole-0.1.1.tar.gz` & `tmp/learnkeyhole-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "learnkeyhole-0.1.1.tar", last modified: Thu May 25 11:56:16 2023, max compression
+gzip compressed data, was "learnkeyhole-0.1.2.tar", last modified: Thu May 25 13:02:06 2023, max compression
```

## Comparing `learnkeyhole-0.1.1.tar` & `learnkeyhole-0.1.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 11:56:16.143833 learnkeyhole-0.1.1/
--rw-rw-rw-   0        0        0     1066 2023-05-24 15:34:14.000000 learnkeyhole-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     5926 2023-05-25 11:56:16.144838 learnkeyhole-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     5044 2023-05-24 15:50:07.000000 learnkeyhole-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-25 11:56:16.085020 learnkeyhole-0.1.1/learnkeyhole/
--rw-rw-rw-   0        0        0        0 2023-05-24 16:16:46.000000 learnkeyhole-0.1.1/learnkeyhole/__init__.py
--rw-rw-rw-   0        0        0    14996 2023-05-25 11:23:51.000000 learnkeyhole-0.1.1/learnkeyhole/__main__.py
--rw-rw-rw-   0        0        0     3313 2023-05-25 03:03:47.000000 learnkeyhole-0.1.1/learnkeyhole/miou.py
-drwxrwxrwx   0        0        0        0 2023-05-25 11:56:16.125630 learnkeyhole-0.1.1/learnkeyhole/nets/
--rw-rw-rw-   0        0        0        1 2023-03-19 13:58:02.000000 learnkeyhole-0.1.1/learnkeyhole/nets/__init__.py
--rw-rw-rw-   0        0        0     6197 2023-05-25 03:01:42.000000 learnkeyhole-0.1.1/learnkeyhole/nets/resnet.py
--rw-rw-rw-   0        0        0     3403 2023-05-25 03:01:44.000000 learnkeyhole-0.1.1/learnkeyhole/nets/unet.py
--rw-rw-rw-   0        0        0     5031 2023-05-25 03:01:43.000000 learnkeyhole-0.1.1/learnkeyhole/nets/unet_training.py
--rw-rw-rw-   0        0        0     2797 2023-05-25 03:01:45.000000 learnkeyhole-0.1.1/learnkeyhole/nets/vgg.py
--rw-rw-rw-   0        0        0    10131 2023-05-25 02:45:23.000000 learnkeyhole-0.1.1/learnkeyhole/predict.py
--rw-rw-rw-   0        0        0     1361 2023-05-25 02:46:08.000000 learnkeyhole-0.1.1/learnkeyhole/summary.py
--rw-rw-rw-   0        0        0    30659 2023-05-25 03:03:47.000000 learnkeyhole-0.1.1/learnkeyhole/train.py
--rw-rw-rw-   0        0        0    18156 2023-05-25 03:01:39.000000 learnkeyhole-0.1.1/learnkeyhole/unet.py
-drwxrwxrwx   0        0        0        0 2023-05-25 11:56:16.141871 learnkeyhole-0.1.1/learnkeyhole/utils/
--rw-rw-rw-   0        0        0        1 2023-05-25 03:01:46.000000 learnkeyhole-0.1.1/learnkeyhole/utils/__init__.py
--rw-rw-rw-   0        0        0     8792 2023-05-25 03:01:47.000000 learnkeyhole-0.1.1/learnkeyhole/utils/callbacks.py
--rw-rw-rw-   0        0        0     6245 2023-05-25 03:01:49.000000 learnkeyhole-0.1.1/learnkeyhole/utils/dataloader.py
--rw-rw-rw-   0        0        0     6220 2023-05-25 03:01:48.000000 learnkeyhole-0.1.1/learnkeyhole/utils/dataloader_medical.py
--rw-rw-rw-   0        0        0     2022 2023-05-25 03:01:51.000000 learnkeyhole-0.1.1/learnkeyhole/utils/utils.py
--rw-rw-rw-   0        0        0    11137 2023-05-25 03:01:49.000000 learnkeyhole-0.1.1/learnkeyhole/utils/utils_fit.py
--rw-rw-rw-   0        0        0    11371 2023-05-25 03:01:50.000000 learnkeyhole-0.1.1/learnkeyhole/utils/utils_metrics.py
--rw-rw-rw-   0        0        0    20744 2023-05-22 08:20:14.000000 learnkeyhole-0.1.1/learnkeyhole/window.ui
-drwxrwxrwx   0        0        0        0 2023-05-25 11:56:16.116374 learnkeyhole-0.1.1/learnkeyhole.egg-info/
--rw-rw-rw-   0        0        0     5926 2023-05-25 11:56:15.000000 learnkeyhole-0.1.1/learnkeyhole.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      847 2023-05-25 11:56:15.000000 learnkeyhole-0.1.1/learnkeyhole.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 11:56:15.000000 learnkeyhole-0.1.1/learnkeyhole.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2023-05-25 11:56:15.000000 learnkeyhole-0.1.1/learnkeyhole.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      195 2023-05-25 11:56:15.000000 learnkeyhole-0.1.1/learnkeyhole.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-25 11:56:15.000000 learnkeyhole-0.1.1/learnkeyhole.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-05-25 11:39:45.000000 learnkeyhole-0.1.1/learnkeyhole.egg-info/zip-safe
--rw-rw-rw-   0        0        0     1088 2023-05-25 11:56:16.148866 learnkeyhole-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      826 2023-05-25 11:37:28.000000 learnkeyhole-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-25 13:02:06.761985 learnkeyhole-0.1.2/
+-rw-rw-rw-   0        0        0     1066 2023-05-24 15:34:14.000000 learnkeyhole-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     5926 2023-05-25 13:02:06.762978 learnkeyhole-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     5044 2023-05-24 15:50:07.000000 learnkeyhole-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-25 13:02:06.689890 learnkeyhole-0.1.2/learnkeyhole/
+-rw-rw-rw-   0        0        0        0 2023-05-24 16:16:46.000000 learnkeyhole-0.1.2/learnkeyhole/__init__.py
+-rw-rw-rw-   0        0        0    14996 2023-05-25 11:23:51.000000 learnkeyhole-0.1.2/learnkeyhole/__main__.py
+-rw-rw-rw-   0        0        0     3313 2023-05-25 03:03:47.000000 learnkeyhole-0.1.2/learnkeyhole/miou.py
+drwxrwxrwx   0        0        0        0 2023-05-25 13:02:06.735976 learnkeyhole-0.1.2/learnkeyhole/nets/
+-rw-rw-rw-   0        0        0        1 2023-03-19 13:58:02.000000 learnkeyhole-0.1.2/learnkeyhole/nets/__init__.py
+-rw-rw-rw-   0        0        0     6197 2023-05-25 03:01:42.000000 learnkeyhole-0.1.2/learnkeyhole/nets/resnet.py
+-rw-rw-rw-   0        0        0     3403 2023-05-25 03:01:44.000000 learnkeyhole-0.1.2/learnkeyhole/nets/unet.py
+-rw-rw-rw-   0        0        0     5031 2023-05-25 03:01:43.000000 learnkeyhole-0.1.2/learnkeyhole/nets/unet_training.py
+-rw-rw-rw-   0        0        0     2797 2023-05-25 03:01:45.000000 learnkeyhole-0.1.2/learnkeyhole/nets/vgg.py
+-rw-rw-rw-   0        0        0    10131 2023-05-25 02:45:23.000000 learnkeyhole-0.1.2/learnkeyhole/predict.py
+-rw-rw-rw-   0        0        0     1361 2023-05-25 02:46:08.000000 learnkeyhole-0.1.2/learnkeyhole/summary.py
+-rw-rw-rw-   0        0        0    30659 2023-05-25 03:03:47.000000 learnkeyhole-0.1.2/learnkeyhole/train.py
+-rw-rw-rw-   0        0        0    18156 2023-05-25 03:01:39.000000 learnkeyhole-0.1.2/learnkeyhole/unet.py
+drwxrwxrwx   0        0        0        0 2023-05-25 13:02:06.759977 learnkeyhole-0.1.2/learnkeyhole/utils/
+-rw-rw-rw-   0        0        0        1 2023-05-25 03:01:46.000000 learnkeyhole-0.1.2/learnkeyhole/utils/__init__.py
+-rw-rw-rw-   0        0        0     8792 2023-05-25 03:01:47.000000 learnkeyhole-0.1.2/learnkeyhole/utils/callbacks.py
+-rw-rw-rw-   0        0        0     6245 2023-05-25 03:01:49.000000 learnkeyhole-0.1.2/learnkeyhole/utils/dataloader.py
+-rw-rw-rw-   0        0        0     6220 2023-05-25 03:01:48.000000 learnkeyhole-0.1.2/learnkeyhole/utils/dataloader_medical.py
+-rw-rw-rw-   0        0        0     2022 2023-05-25 03:01:51.000000 learnkeyhole-0.1.2/learnkeyhole/utils/utils.py
+-rw-rw-rw-   0        0        0    11137 2023-05-25 03:01:49.000000 learnkeyhole-0.1.2/learnkeyhole/utils/utils_fit.py
+-rw-rw-rw-   0        0        0    11371 2023-05-25 03:01:50.000000 learnkeyhole-0.1.2/learnkeyhole/utils/utils_metrics.py
+-rw-rw-rw-   0        0        0    20744 2023-05-22 08:20:14.000000 learnkeyhole-0.1.2/learnkeyhole/window.ui
+drwxrwxrwx   0        0        0        0 2023-05-25 13:02:06.719897 learnkeyhole-0.1.2/learnkeyhole.egg-info/
+-rw-rw-rw-   0        0        0     5926 2023-05-25 13:02:06.000000 learnkeyhole-0.1.2/learnkeyhole.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      847 2023-05-25 13:02:06.000000 learnkeyhole-0.1.2/learnkeyhole.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 13:02:06.000000 learnkeyhole-0.1.2/learnkeyhole.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2023-05-25 13:02:06.000000 learnkeyhole-0.1.2/learnkeyhole.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      183 2023-05-25 13:02:06.000000 learnkeyhole-0.1.2/learnkeyhole.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-25 13:02:06.000000 learnkeyhole-0.1.2/learnkeyhole.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-05-25 13:02:02.000000 learnkeyhole-0.1.2/learnkeyhole.egg-info/zip-safe
+-rw-rw-rw-   0        0        0     1076 2023-05-25 13:02:06.767974 learnkeyhole-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      826 2023-05-25 12:56:35.000000 learnkeyhole-0.1.2/setup.py
```

### Comparing `learnkeyhole-0.1.1/LICENSE` & `learnkeyhole-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `learnkeyhole-0.1.1/PKG-INFO` & `learnkeyhole-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: learnkeyhole
-Version: 0.1.1
+Version: 0.1.2
 Summary: Use this package to train your keyhole and predict it rapidly and right
 Home-page: https://github.com/wu-xz21/learnkeyhole  #github地址或其他地址
 Author: WUXianzhi,ZhengQingzhi,WeiLang
 Author-email: wu-xz@outlook.com
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `learnkeyhole-0.1.1/README.md` & `learnkeyhole-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `learnkeyhole-0.1.1/learnkeyhole/__main__.py` & `learnkeyhole-0.1.2/learnkeyhole/__main__.py`

 * *Files identical despite different names*

### Comparing `learnkeyhole-0.1.1/learnkeyhole/miou.py` & `learnkeyhole-0.1.2/learnkeyhole/miou.py`

 * *Files identical despite different names*

### Comparing `learnkeyhole-0.1.1/learnkeyhole/nets/resnet.py` & `learnkeyhole-0.1.2/learnkeyhole/nets/resnet.py`

 * *Files identical despite different names*

### Comparing `learnkeyhole-0.1.1/learnkeyhole/nets/unet.py` & `learnkeyhole-0.1.2/learnkeyhole/nets/unet.py`

 * *Files identical despite different names*

### Comparing `learnkeyhole-0.1.1/learnkeyhole/nets/unet_training.py` & `learnkeyhole-0.1.2/learnkeyhole/nets/unet_training.py`

 * *Files identical despite different names*

### Comparing `learnkeyhole-0.1.1/learnkeyhole/nets/vgg.py` & `learnkeyhole-0.1.2/learnkeyhole/nets/vgg.py`

 * *Files identical despite different names*

### Comparing `learnkeyhole-0.1.1/learnkeyhole/predict.py` & `learnkeyhole-0.1.2/learnkeyhole/predict.py`

 * *Files identical despite different names*

### Comparing `learnkeyhole-0.1.1/learnkeyhole/summary.py` & `learnkeyhole-0.1.2/learnkeyhole/summary.py`

 * *Files identical despite different names*

### Comparing `learnkeyhole-0.1.1/learnkeyhole/train.py` & `learnkeyhole-0.1.2/learnkeyhole/train.py`

 * *Files identical despite different names*

### Comparing `learnkeyhole-0.1.1/learnkeyhole/unet.py` & `learnkeyhole-0.1.2/learnkeyhole/unet.py`

 * *Files identical despite different names*

### Comparing `learnkeyhole-0.1.1/learnkeyhole/utils/callbacks.py` & `learnkeyhole-0.1.2/learnkeyhole/utils/callbacks.py`

 * *Files identical despite different names*

### Comparing `learnkeyhole-0.1.1/learnkeyhole/utils/dataloader.py` & `learnkeyhole-0.1.2/learnkeyhole/utils/dataloader.py`

 * *Files identical despite different names*

### Comparing `learnkeyhole-0.1.1/learnkeyhole/utils/dataloader_medical.py` & `learnkeyhole-0.1.2/learnkeyhole/utils/dataloader_medical.py`

 * *Files identical despite different names*

### Comparing `learnkeyhole-0.1.1/learnkeyhole/utils/utils.py` & `learnkeyhole-0.1.2/learnkeyhole/utils/utils.py`

 * *Files identical despite different names*

### Comparing `learnkeyhole-0.1.1/learnkeyhole/utils/utils_fit.py` & `learnkeyhole-0.1.2/learnkeyhole/utils/utils_fit.py`

 * *Files identical despite different names*

### Comparing `learnkeyhole-0.1.1/learnkeyhole/utils/utils_metrics.py` & `learnkeyhole-0.1.2/learnkeyhole/utils/utils_metrics.py`

 * *Files identical despite different names*

### Comparing `learnkeyhole-0.1.1/learnkeyhole/window.ui` & `learnkeyhole-0.1.2/learnkeyhole/window.ui`

 * *Files identical despite different names*

### Comparing `learnkeyhole-0.1.1/learnkeyhole.egg-info/PKG-INFO` & `learnkeyhole-0.1.2/learnkeyhole.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: learnkeyhole
-Version: 0.1.1
+Version: 0.1.2
 Summary: Use this package to train your keyhole and predict it rapidly and right
 Home-page: https://github.com/wu-xz21/learnkeyhole  #github地址或其他地址
 Author: WUXianzhi,ZhengQingzhi,WeiLang
 Author-email: wu-xz@outlook.com
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `learnkeyhole-0.1.1/learnkeyhole.egg-info/SOURCES.txt` & `learnkeyhole-0.1.2/learnkeyhole.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `learnkeyhole-0.1.1/setup.cfg` & `learnkeyhole-0.1.2/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206c 6561 726e 6b65 7968 6f6c 650d   = learnkeyhole.
-00000020: 0a76 6572 7369 6f6e 203d 2030 2e31 2e31  .version = 0.1.1
+00000020: 0a76 6572 7369 6f6e 203d 2030 2e31 2e32  .version = 0.1.2
 00000030: 0d0a 6175 7468 6f72 203d 2057 5558 6961  ..author = WUXia
 00000040: 6e7a 6869 2c5a 6865 6e67 5169 6e67 7a68  nzhi,ZhengQingzh
 00000050: 692c 5765 694c 616e 670d 0a61 7574 686f  i,WeiLang..autho
 00000060: 725f 656d 6169 6c20 3d20 7775 2d78 7a40  r_email = wu-xz@
 00000070: 6f75 746c 6f6f 6b2e 636f 6d0d 0a64 6573  outlook.com..des
 00000080: 6372 6970 7469 6f6e 203d 2055 7365 2074  cription = Use t
 00000090: 6869 7320 7061 636b 6167 6520 746f 2074  his package to t
@@ -50,19 +50,19 @@
 00000310: 6972 6573 203d 203e 3d33 2e36 2c3c 3d33  ires = >=3.6,<=3
 00000320: 2e39 0d0a 696e 7374 616c 6c5f 7265 7175  .9..install_requ
 00000330: 6972 6573 203d 200d 0a09 7061 6e64 6173  ires = ...pandas
 00000340: 3e3d 312e 352e 330d 0a09 6e75 6d70 793e  >=1.5.3...numpy>
 00000350: 3d31 2e32 342e 320d 0a09 7363 6970 793e  =1.24.2...scipy>
 00000360: 3d31 2e31 302e 300d 0a09 6e75 6d70 793e  =1.10.0...numpy>
 00000370: 3d31 2e32 342e 320d 0a09 6d61 7470 6c6f  =1.24.2...matplo
-00000380: 746c 6962 3d3d 332e 372e 310d 0a09 6f70  tlib==3.7.1...op
-00000390: 656e 6376 5f70 7974 686f 6e3d 3d34 2e31  encv_python==4.1
-000003a0: 2e32 2e33 300d 0a09 746f 7263 683d 3d31  .2.30...torch==1
-000003b0: 2e37 2e31 2b63 7531 3130 0d0a 0974 6f72  .7.1+cu110...tor
-000003c0: 6368 7669 7369 6f6e 3d3d 302e 382e 322b  chvision==0.8.2+
-000003d0: 6375 3131 300d 0a09 7471 646d 3d3d 342e  cu110...tqdm==4.
-000003e0: 3634 2e31 0d0a 0970 696c 6c6f 773d 3d39  64.1...pillow==9
-000003f0: 2e34 2e30 0d0a 0968 3570 793d 3d33 2e38  .4.0...h5py==3.8
-00000400: 2e30 0d0a 0950 7951 7435 3d3d 352e 3135  .0...PyQt5==5.15
-00000410: 2e37 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d  .7....[egg_info]
-00000420: 0d0a 7461 675f 6275 696c 6420 3d20 0d0a  ..tag_build = ..
-00000430: 7461 675f 6461 7465 203d 2030 0d0a 0d0a  tag_date = 0....
+00000380: 746c 6962 3e3d 332e 372e 300d 0a09 6f70  tlib>=3.7.0...op
+00000390: 656e 6376 5f70 7974 686f 6e3e 3d34 2e34  encv_python>=4.4
+000003a0: 2e30 2e34 300d 0a09 746f 7263 683e 3d31  .0.40...torch>=1
+000003b0: 2e37 2e31 0d0a 0974 6f72 6368 7669 7369  .7.1...torchvisi
+000003c0: 6f6e 3e3d 302e 382e 320d 0a09 7471 646d  on>=0.8.2...tqdm
+000003d0: 3e3d 342e 3634 2e30 0d0a 0970 696c 6c6f  >=4.64.0...pillo
+000003e0: 773e 3d39 2e34 2e30 0d0a 0968 3570 793e  w>=9.4.0...h5py>
+000003f0: 3d33 2e36 2e30 0d0a 0950 7951 7435 3e3d  =3.6.0...PyQt5>=
+00000400: 352e 3134 2e30 0d0a 0d0a 5b65 6767 5f69  5.14.0....[egg_i
+00000410: 6e66 6f5d 0d0a 7461 675f 6275 696c 6420  nfo]..tag_build 
+00000420: 3d20 0d0a 7461 675f 6461 7465 203d 2030  = ..tag_date = 0
+00000430: 0d0a 0d0a                                ....
```

### Comparing `learnkeyhole-0.1.1/setup.py` & `learnkeyhole-0.1.2/setup.py`

 * *Files identical despite different names*

