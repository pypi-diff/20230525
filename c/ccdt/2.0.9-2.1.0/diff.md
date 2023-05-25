# Comparing `tmp/ccdt-2.0.9.tar.gz` & `tmp/ccdt-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ccdt-2.0.9.tar", last modified: Tue May  9 08:14:29 2023, max compression
+gzip compressed data, was "ccdt-2.1.0.tar", last modified: Thu May 25 08:01:16 2023, max compression
```

## Comparing `ccdt-2.0.9.tar` & `ccdt-2.1.0.tar`

### file list

```diff
@@ -1,38 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-09 08:14:29.982794 ccdt-2.0.9/
--rw-rw-rw-   0        0        0    35823 2022-02-07 08:35:22.000000 ccdt-2.0.9/LICENSE
--rw-rw-rw-   0        0        0     4319 2023-05-09 08:14:29.980797 ccdt-2.0.9/PKG-INFO
--rw-rw-rw-   0        0        0     3795 2022-02-07 08:35:22.000000 ccdt-2.0.9/README.md
-drwxrwxrwx   0        0        0        0 2023-05-09 08:14:29.909988 ccdt-2.0.9/ccdt/
--rw-rw-rw-   0        0        0      119 2023-03-30 08:20:38.000000 ccdt-2.0.9/ccdt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-09 08:14:29.932927 ccdt-2.0.9/ccdt/dataset/
--rw-rw-rw-   0        0        0      195 2023-04-07 09:48:43.000000 ccdt-2.0.9/ccdt/dataset/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-09 08:14:29.939908 ccdt-2.0.9/ccdt/dataset/base_coco/
--rw-rw-rw-   0        0        0      136 2023-04-20 09:55:44.000000 ccdt-2.0.9/ccdt/dataset/base_coco/__init__.py
--rw-rw-rw-   0        0        0    22389 2023-04-25 09:55:26.000000 ccdt-2.0.9/ccdt/dataset/base_coco/coco.py
-drwxrwxrwx   0        0        0        0 2023-05-09 08:14:29.951875 ccdt-2.0.9/ccdt/dataset/base_labelme/
--rw-rw-rw-   0        0        0      315 2023-04-21 03:03:13.000000 ccdt-2.0.9/ccdt/dataset/base_labelme/__init__.py
--rw-rw-rw-   0        0        0     7885 2023-04-25 10:13:02.000000 ccdt-2.0.9/ccdt/dataset/base_labelme/async_io_task.py
--rw-rw-rw-   0        0        0    63485 2023-05-09 08:13:56.000000 ccdt-2.0.9/ccdt/dataset/base_labelme/base_labelme.py
--rw-rw-rw-   0        0        0      471 2023-05-08 06:44:57.000000 ccdt-2.0.9/ccdt/dataset/base_labelme/test_async_io.py
-drwxrwxrwx   0        0        0        0 2023-05-09 08:14:29.954867 ccdt-2.0.9/ccdt/dataset/logs/
--rw-rw-rw-   0        0        0       91 2023-04-17 07:05:17.000000 ccdt-2.0.9/ccdt/dataset/logs/__init__.py
--rw-rw-rw-   0        0        0    12305 2023-05-09 07:48:32.000000 ccdt-2.0.9/ccdt/dataset/main.py
-drwxrwxrwx   0        0        0        0 2023-05-09 08:14:29.968829 ccdt-2.0.9/ccdt/dataset/utils/
--rw-rw-rw-   0        0        0      251 2023-05-09 03:47:20.000000 ccdt-2.0.9/ccdt/dataset/utils/__init__.py
--rw-rw-rw-   0        0        0      894 2023-05-09 03:47:20.000000 ccdt-2.0.9/ccdt/dataset/utils/async_dirIterator.py
--rw-rw-rw-   0        0        0      525 2022-03-25 05:57:57.000000 ccdt-2.0.9/ccdt/dataset/utils/encoder.py
--rw-rw-rw-   0        0        0    17244 2023-05-09 03:37:25.000000 ccdt-2.0.9/ccdt/dataset/utils/labelme_load.py
--rw-rw-rw-   0        0        0       91 2023-04-17 07:05:59.000000 ccdt-2.0.9/ccdt/dataset/utils/logs.py
-drwxrwxrwx   0        0        0        0 2023-05-09 08:14:29.977805 ccdt-2.0.9/ccdt/video_tool/
--rw-rw-rw-   0        0        0      124 2022-03-31 07:58:09.000000 ccdt-2.0.9/ccdt/video_tool/__init__.py
--rw-rw-rw-   0        0        0     1394 2023-02-11 04:06:30.000000 ccdt-2.0.9/ccdt/video_tool/split.py
--rw-rw-rw-   0        0        0     4779 2023-04-25 05:47:57.000000 ccdt-2.0.9/ccdt/video_tool/video_main.py
-drwxrwxrwx   0        0        0        0 2023-05-09 08:14:29.927938 ccdt-2.0.9/ccdt.egg-info/
--rw-rw-rw-   0        0        0     4319 2023-05-09 08:14:29.000000 ccdt-2.0.9/ccdt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      767 2023-05-09 08:14:29.000000 ccdt-2.0.9/ccdt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 08:14:29.000000 ccdt-2.0.9/ccdt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       88 2023-05-09 08:14:29.000000 ccdt-2.0.9/ccdt.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       57 2023-05-09 08:14:29.000000 ccdt-2.0.9/ccdt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-05-09 08:14:29.000000 ccdt-2.0.9/ccdt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-09 08:14:29.983789 ccdt-2.0.9/setup.cfg
--rw-rw-rw-   0        0        0     2278 2023-05-09 08:13:56.000000 ccdt-2.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-25 08:01:16.545445 ccdt-2.1.0/
+-rw-rw-rw-   0        0        0    35823 2023-05-23 02:06:29.000000 ccdt-2.1.0/LICENSE
+-rw-rw-rw-   0        0        0     4309 2023-05-25 08:01:16.543493 ccdt-2.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3785 2023-05-23 02:44:28.000000 ccdt-2.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-25 08:01:16.539488 ccdt-2.1.0/ccdt.egg-info/
+-rw-rw-rw-   0        0        0     4309 2023-05-25 08:01:16.000000 ccdt-2.1.0/ccdt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      196 2023-05-25 08:01:16.000000 ccdt-2.1.0/ccdt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 08:01:16.000000 ccdt-2.1.0/ccdt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       88 2023-05-25 08:01:16.000000 ccdt-2.1.0/ccdt.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       89 2023-05-25 08:01:16.000000 ccdt-2.1.0/ccdt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 08:01:16.000000 ccdt-2.1.0/ccdt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-25 08:01:16.546470 ccdt-2.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     2357 2023-05-25 06:41:56.000000 ccdt-2.1.0/setup.py
```

### Comparing `ccdt-2.0.9/LICENSE` & `ccdt-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ccdt-2.0.9/PKG-INFO` & `ccdt-2.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccdt
-Version: 2.0.9
+Version: 2.1.0
 Summary: AI数据转换工具箱
 Home-page: https://github.com/chipeak/chipeak_cv_data_tool
 Author: zhanyong
 Author-email: zhan.yong@chipeak.com
 Project-URL: Bug Tracker, https://github.com/chipeak/chipeak_cv_data_tool/issues
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
@@ -103,18 +103,18 @@
 
 无
 
 ## 引用
 
 ```
 @misc{ccdt2021,
-  author =       {詹勇，朱文海},
+  author =       {詹勇},
   title =        {{ccdt: Annotation conversion and file video processing tools}},
-  howpublished = {url{https://github.com/540717421/chipeak_cv_data_tool}},
-  year =         {2021}
+  howpublished = {url{https://github.com/chipeak/chipeak_cv_data_tool.git}},
+  year =         {2023}
 }
 ```
 ## ChiPeak的其它项目
 
 - [ccdt](https://github.com/540717421/chipeak_data_tool): chipeak_cv_data_tool AI数据处理工具箱
```

### Comparing `ccdt-2.0.9/README.md` & `ccdt-2.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -89,18 +89,18 @@
 
 无
 
 ## 引用
 
 ```
 @misc{ccdt2021,
-  author =       {詹勇，朱文海},
+  author =       {詹勇},
   title =        {{ccdt: Annotation conversion and file video processing tools}},
-  howpublished = {url{https://github.com/540717421/chipeak_cv_data_tool}},
-  year =         {2021}
+  howpublished = {url{https://github.com/chipeak/chipeak_cv_data_tool.git}},
+  year =         {2023}
 }
 ```
 ## ChiPeak的其它项目
 
 - [ccdt](https://github.com/540717421/chipeak_data_tool): chipeak_cv_data_tool AI数据处理工具箱
```

### Comparing `ccdt-2.0.9/ccdt.egg-info/PKG-INFO` & `ccdt-2.1.0/ccdt.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccdt
-Version: 2.0.9
+Version: 2.1.0
 Summary: AI数据转换工具箱
 Home-page: https://github.com/chipeak/chipeak_cv_data_tool
 Author: zhanyong
 Author-email: zhan.yong@chipeak.com
 Project-URL: Bug Tracker, https://github.com/chipeak/chipeak_cv_data_tool/issues
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
@@ -103,18 +103,18 @@
 
 无
 
 ## 引用
 
 ```
 @misc{ccdt2021,
-  author =       {詹勇，朱文海},
+  author =       {詹勇},
   title =        {{ccdt: Annotation conversion and file video processing tools}},
-  howpublished = {url{https://github.com/540717421/chipeak_cv_data_tool}},
-  year =         {2021}
+  howpublished = {url{https://github.com/chipeak/chipeak_cv_data_tool.git}},
+  year =         {2023}
 }
 ```
 ## ChiPeak的其它项目
 
 - [ccdt](https://github.com/540717421/chipeak_data_tool): chipeak_cv_data_tool AI数据处理工具箱
```

### Comparing `ccdt-2.0.9/setup.py` & `ccdt-2.1.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,22 +13,26 @@
     install_requires = [
         'tqdm',
         'opencv_python',  # for PyInstaller
         'numpy',
         'pycocotools',
         'prettytable',
         'shapely',
+        'psutil',
+        'pypinyin',
+        'aiofiles',
+        'Pillow'
     ]
     return install_requires
 
 
 setup(
     # 取名不能够用_会自动变-   ccdt
     name='ccdt',
-    version='2.0.9',
+    version='2.1.0',
     packages=find_packages(exclude=['data']),
     install_requires=get_install_requires(),
     author='zhanyong',
     author_email='zhan.yong@chipeak.com',
     description='AI数据转换工具箱',
     long_description=long_description,
     long_description_content_type='text/markdown',
```

