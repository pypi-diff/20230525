# Comparing `tmp/mmWave-0.1.96.tar.gz` & `tmp/mmWave-0.1.97.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mmWave-0.1.96.tar", last modified: Fri Apr  7 03:23:20 2023, max compression
+gzip compressed data, was "dist/mmWave-0.1.97.tar", last modified: Thu May 25 06:32:03 2023, max compression
```

## Comparing `mmWave-0.1.96.tar` & `mmWave-0.1.97.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-04-07 03:23:20.872240 mmWave-0.1.96/
--rw-r--r--   0 zach       (501) staff       (20)     6147 2023-04-07 03:23:20.872405 mmWave-0.1.96/PKG-INFO
--rw-r--r--   0 zach       (501) staff       (20)     5646 2023-04-07 03:20:06.000000 mmWave-0.1.96/README.md
-drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-04-07 03:23:20.870686 mmWave-0.1.96/mmWave/
--rw-r--r--   0 zach       (501) staff       (20)        2 2019-01-18 15:34:28.000000 mmWave-0.1.96/mmWave/__init__.py
--rwxrwxrwx   0 zach       (501) staff       (20)    15857 2020-05-13 09:15:42.000000 mmWave-0.1.96/mmWave/droneRN.py
--rwxrwxrwx   0 zach       (501) staff       (20)     8286 2019-07-03 01:50:56.000000 mmWave-0.1.96/mmWave/highAccuracy.py
--rw-r--r--   0 zach       (501) staff       (20)    18084 2021-05-26 05:59:29.000000 mmWave-0.1.96/mmWave/lpdFDS.py
--rwxrwxrwx   0 zach       (501) staff       (20)    12507 2023-02-04 06:54:20.000000 mmWave-0.1.96/mmWave/lpdISK.py
--rwxrwxrwx   0 zach       (501) staff       (20)     4465 2019-12-05 19:36:36.000000 mmWave-0.1.96/mmWave/lpdISK_kv.py
--rwxrwxrwx   0 zach       (501) staff       (20)    11171 2022-11-03 03:52:22.000000 mmWave-0.1.96/mmWave/lpdISK_v2.py
--rwxrwxrwx   0 zach       (501) staff       (20)    17158 2023-03-24 07:25:35.000000 mmWave-0.1.96/mmWave/mrRadar.py
--rwxrwxrwx   0 zach       (501) staff       (20)    18021 2021-12-30 16:06:25.000000 mmWave-0.1.96/mmWave/pc3.py
--rw-rw-r--   0 zach       (501) staff       (20)    19716 2022-10-06 04:29:24.000000 mmWave-0.1.96/mmWave/pc3OVH.py
--rw-r--r--   0 zach       (501) staff       (20)    19045 2022-09-02 15:04:31.000000 mmWave-0.1.96/mmWave/pc3_360.py
--rwxrwxrwx   0 zach       (501) staff       (20)    22189 2022-03-02 12:54:15.000000 mmWave-0.1.96/mmWave/pc3_oob.py
--rw-r--r--   0 zach       (501) staff       (20)    16407 2023-04-07 03:18:25.000000 mmWave-0.1.96/mmWave/pc3_v1884R.py
--rwxrwxrwx   0 zach       (501) staff       (20)    19380 2022-06-13 08:50:32.000000 mmWave-0.1.96/mmWave/pc3_v2.py
--rwxrwxrwx   0 zach       (501) staff       (20)    22899 2022-09-02 02:15:42.000000 mmWave-0.1.96/mmWave/pc3_vsd.py
--rwxrwxrwx   0 zach       (501) staff       (20)    11294 2022-09-15 06:03:06.000000 mmWave-0.1.96/mmWave/pc3_vsd_v2.py
--rwxrwxrwx   0 zach       (501) staff       (20)    10563 2019-12-01 23:33:06.000000 mmWave-0.1.96/mmWave/pc3d.py
--rwxrwxrwx   0 zach       (501) staff       (20)     4209 2019-12-01 23:33:32.000000 mmWave-0.1.96/mmWave/pc3d_kv.py
--rw-r--r--   0 zach       (501) staff       (20)    18872 2023-02-09 15:38:21.000000 mmWave-0.1.96/mmWave/pct.py
--rwxrwxrwx   0 zach       (501) staff       (20)     4052 2019-11-26 11:17:46.000000 mmWave-0.1.96/mmWave/people3D.py
--rwxrwxrwx   0 zach       (501) staff       (20)     8311 2020-04-21 03:50:24.000000 mmWave-0.1.96/mmWave/peopleMB.py
--rw-r--r--   0 zach       (501) staff       (20)     5914 2022-10-13 04:02:11.000000 mmWave-0.1.96/mmWave/roadwayTMD_kv.py
--rwxrwxrwx   0 zach       (501) staff       (20)     9165 2021-12-30 05:31:56.000000 mmWave-0.1.96/mmWave/srradar.py
--rwxrwxrwx   0 zach       (501) staff       (20)    15643 2020-04-17 03:47:43.000000 mmWave-0.1.96/mmWave/surfaceVD.py
--rwxrwxrwx   0 zach       (501) staff       (20)    18348 2023-03-24 07:23:52.000000 mmWave-0.1.96/mmWave/trafficMD.py
--rw-r--r--   0 zach       (501) staff       (20)    19893 2023-03-24 07:30:55.000000 mmWave-0.1.96/mmWave/trafficMD_I480.py
--rw-r--r--   0 zach       (501) staff       (20)     4612 2020-04-30 09:13:56.000000 mmWave-0.1.96/mmWave/trafficMD_kv.py
--rwxrwxrwx   0 zach       (501) staff       (20)    10456 2020-04-21 03:35:54.000000 mmWave-0.1.96/mmWave/vehicleOD.py
--rw-r--r--   0 zach       (501) staff       (20)    10075 2020-07-21 15:14:04.000000 mmWave-0.1.96/mmWave/vehicleODHeatMap.py
--rwxrwxrwx   0 zach       (501) staff       (20)    14108 2021-01-07 04:09:32.000000 mmWave-0.1.96/mmWave/vehicleODR.py
--rw-r--r--   0 zach       (501) staff       (20)     7125 2020-02-04 15:39:27.000000 mmWave-0.1.96/mmWave/vitalsign.py
--rw-r--r--   0 zach       (501) staff       (20)     2498 2020-10-21 06:27:00.000000 mmWave-0.1.96/mmWave/vitalsign_kv.py
-drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-04-07 03:23:20.871950 mmWave-0.1.96/mmWave.egg-info/
--rw-r--r--   0 zach       (501) staff       (20)     6147 2023-04-07 03:23:19.000000 mmWave-0.1.96/mmWave.egg-info/PKG-INFO
--rw-r--r--   0 zach       (501) staff       (20)      770 2023-04-07 03:23:20.000000 mmWave-0.1.96/mmWave.egg-info/SOURCES.txt
--rw-r--r--   0 zach       (501) staff       (20)        1 2023-04-07 03:23:19.000000 mmWave-0.1.96/mmWave.egg-info/dependency_links.txt
--rw-r--r--   0 zach       (501) staff       (20)        7 2023-04-07 03:23:20.000000 mmWave-0.1.96/mmWave.egg-info/top_level.txt
--rw-r--r--   0 zach       (501) staff       (20)       38 2023-04-07 03:23:20.872781 mmWave-0.1.96/setup.cfg
--rw-r--r--   0 zach       (501) staff       (20)     6343 2023-04-07 03:21:21.000000 mmWave-0.1.96/setup.py
+drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-05-25 06:32:03.727208 mmWave-0.1.97/
+-rw-r--r--   0 zach       (501) staff       (20)     6283 2023-05-25 06:32:03.727473 mmWave-0.1.97/PKG-INFO
+-rw-r--r--   0 zach       (501) staff       (20)     5782 2023-05-25 06:27:57.000000 mmWave-0.1.97/README.md
+drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-05-25 06:32:03.724551 mmWave-0.1.97/mmWave/
+-rw-r--r--   0 zach       (501) staff       (20)        2 2019-01-18 15:34:28.000000 mmWave-0.1.97/mmWave/__init__.py
+-rwxrwxrwx   0 zach       (501) staff       (20)    15857 2020-05-13 09:15:42.000000 mmWave-0.1.97/mmWave/droneRN.py
+-rwxrwxrwx   0 zach       (501) staff       (20)     8286 2019-07-03 01:50:56.000000 mmWave-0.1.97/mmWave/highAccuracy.py
+-rw-r--r--   0 zach       (501) staff       (20)    18084 2021-05-26 05:59:29.000000 mmWave-0.1.97/mmWave/lpdFDS.py
+-rwxrwxrwx   0 zach       (501) staff       (20)    12507 2023-02-04 06:54:20.000000 mmWave-0.1.97/mmWave/lpdISK.py
+-rwxrwxrwx   0 zach       (501) staff       (20)     4465 2019-12-05 19:36:36.000000 mmWave-0.1.97/mmWave/lpdISK_kv.py
+-rwxrwxrwx   0 zach       (501) staff       (20)    11171 2022-11-03 03:52:22.000000 mmWave-0.1.97/mmWave/lpdISK_v2.py
+-rwxrwxrwx   0 zach       (501) staff       (20)    17158 2023-03-24 07:25:35.000000 mmWave-0.1.97/mmWave/mrRadar.py
+-rwxrwxrwx   0 zach       (501) staff       (20)    18021 2021-12-30 16:06:25.000000 mmWave-0.1.97/mmWave/pc3.py
+-rw-rw-r--   0 zach       (501) staff       (20)    19716 2022-10-06 04:29:24.000000 mmWave-0.1.97/mmWave/pc3OVH.py
+-rw-r--r--   0 zach       (501) staff       (20)    19045 2022-09-02 15:04:31.000000 mmWave-0.1.97/mmWave/pc3_360.py
+-rwxrwxrwx   0 zach       (501) staff       (20)    21393 2023-05-25 06:30:51.000000 mmWave-0.1.97/mmWave/pc3_oob.py
+-rw-r--r--   0 zach       (501) staff       (20)    16407 2023-04-07 03:18:25.000000 mmWave-0.1.97/mmWave/pc3_v1884R.py
+-rwxrwxrwx   0 zach       (501) staff       (20)    19380 2022-06-13 08:50:32.000000 mmWave-0.1.97/mmWave/pc3_v2.py
+-rwxrwxrwx   0 zach       (501) staff       (20)    22899 2022-09-02 02:15:42.000000 mmWave-0.1.97/mmWave/pc3_vsd.py
+-rwxrwxrwx   0 zach       (501) staff       (20)    11294 2022-09-15 06:03:06.000000 mmWave-0.1.97/mmWave/pc3_vsd_v2.py
+-rwxrwxrwx   0 zach       (501) staff       (20)    10563 2019-12-01 23:33:06.000000 mmWave-0.1.97/mmWave/pc3d.py
+-rwxrwxrwx   0 zach       (501) staff       (20)     4209 2019-12-01 23:33:32.000000 mmWave-0.1.97/mmWave/pc3d_kv.py
+-rw-r--r--   0 zach       (501) staff       (20)    18872 2023-02-09 15:38:21.000000 mmWave-0.1.97/mmWave/pct.py
+-rwxrwxrwx   0 zach       (501) staff       (20)     4052 2019-11-26 11:17:46.000000 mmWave-0.1.97/mmWave/people3D.py
+-rwxrwxrwx   0 zach       (501) staff       (20)     8311 2020-04-21 03:50:24.000000 mmWave-0.1.97/mmWave/peopleMB.py
+-rw-r--r--   0 zach       (501) staff       (20)     5914 2022-10-13 04:02:11.000000 mmWave-0.1.97/mmWave/roadwayTMD_kv.py
+-rwxrwxrwx   0 zach       (501) staff       (20)     9165 2021-12-30 05:31:56.000000 mmWave-0.1.97/mmWave/srradar.py
+-rwxrwxrwx   0 zach       (501) staff       (20)    15643 2020-04-17 03:47:43.000000 mmWave-0.1.97/mmWave/surfaceVD.py
+-rwxrwxrwx   0 zach       (501) staff       (20)    18348 2023-03-24 07:23:52.000000 mmWave-0.1.97/mmWave/trafficMD.py
+-rw-r--r--   0 zach       (501) staff       (20)    19893 2023-03-24 07:30:55.000000 mmWave-0.1.97/mmWave/trafficMD_I480.py
+-rw-r--r--   0 zach       (501) staff       (20)     4612 2020-04-30 09:13:56.000000 mmWave-0.1.97/mmWave/trafficMD_kv.py
+-rwxrwxrwx   0 zach       (501) staff       (20)    10456 2020-04-21 03:35:54.000000 mmWave-0.1.97/mmWave/vehicleOD.py
+-rw-r--r--   0 zach       (501) staff       (20)    10075 2020-07-21 15:14:04.000000 mmWave-0.1.97/mmWave/vehicleODHeatMap.py
+-rwxrwxrwx   0 zach       (501) staff       (20)    14108 2021-01-07 04:09:32.000000 mmWave-0.1.97/mmWave/vehicleODR.py
+-rw-r--r--   0 zach       (501) staff       (20)     7125 2020-02-04 15:39:27.000000 mmWave-0.1.97/mmWave/vitalsign.py
+-rw-r--r--   0 zach       (501) staff       (20)     2498 2020-10-21 06:27:00.000000 mmWave-0.1.97/mmWave/vitalsign_kv.py
+drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-05-25 06:32:03.726680 mmWave-0.1.97/mmWave.egg-info/
+-rw-r--r--   0 zach       (501) staff       (20)     6283 2023-05-25 06:32:02.000000 mmWave-0.1.97/mmWave.egg-info/PKG-INFO
+-rw-r--r--   0 zach       (501) staff       (20)      770 2023-05-25 06:32:03.000000 mmWave-0.1.97/mmWave.egg-info/SOURCES.txt
+-rw-r--r--   0 zach       (501) staff       (20)        1 2023-05-25 06:32:02.000000 mmWave-0.1.97/mmWave.egg-info/dependency_links.txt
+-rw-r--r--   0 zach       (501) staff       (20)        7 2023-05-25 06:32:03.000000 mmWave-0.1.97/mmWave.egg-info/top_level.txt
+-rw-r--r--   0 zach       (501) staff       (20)       38 2023-05-25 06:32:03.728151 mmWave-0.1.97/setup.cfg
+-rw-r--r--   0 zach       (501) staff       (20)     6467 2023-05-25 06:28:25.000000 mmWave-0.1.97/setup.py
```

### Comparing `mmWave-0.1.96/PKG-INFO` & `mmWave-0.1.97/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmWave
-Version: 0.1.96
+Version: 0.1.97
 Summary: Joybien mmWave (Batman-101/201/301/501/601) library
 Home-page: http://www.joybien.com
 Download-URL: https://pypi.org/project/mmWave
 Author: Bighead Chen
 Author-email: zach_chen@joybien.com
 Project-URL: API Source Code, https://github.com/bigheadG/mmWave
 Classifier: Programming Language :: Python :: 3
@@ -56,14 +56,16 @@
             v0.0.2 2022/02/07 format revised
             v0.1.0 2022/06/02 fit v3 data
             v1.0.0 2022/06/08 change data get method
             v1.0.1 :2022/06/09 added headerShowAll()
 24. pc3_oob v0.0.1 2022/03/01 first released
             v0.0.2 2022/03/01 bug fix
             v0.0.3 2022/03/03
+            v0.0.4 :2023/05/25 @v1.0.97 add v7, playback
+            
 25. pc3_vsd v0.0.1 2022/03/10 Bata version (deprecated)
 26. pc3_v2  v2     2022/04/19 first released
             v2.0.1 2022/06/10 pc3_v2 v6 add sx,sy,sz   
             v2.0.2 2022/06/13 pc3_v2 add azimuth offset 
             
 27. pc3_360 v0.0.1 2022/08/16 for integrate 3 sets of module. 
 
@@ -149,7 +151,9 @@
 29. mmWave-1.0.95
     2023/03/24 mrRadar   v1.0.2  header enable/disable in inital
     2023/03/24 trafficMD v0.1.1  header enable/disable in inital
     2023/03/24  trafficMD_I480   ver:2.0.6 header enable/disable in inital
 30. mmWave-1.0.96
     2023/04/07 pc3_V1884R v0.0.2  add try..except in unpack
 
+31. mmWave-1.0.97
+    2023/05/25 pc3_oob v0.0.4 add v7, playback
```

### Comparing `mmWave-0.1.96/README.md` & `mmWave-0.1.97/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,16 @@
             v0.0.2 2022/02/07 format revised
             v0.1.0 2022/06/02 fit v3 data
             v1.0.0 2022/06/08 change data get method
             v1.0.1 :2022/06/09 added headerShowAll()
 24. pc3_oob v0.0.1 2022/03/01 first released
             v0.0.2 2022/03/01 bug fix
             v0.0.3 2022/03/03
+            v0.0.4 :2023/05/25 @v1.0.97 add v7, playback
+            
 25. pc3_vsd v0.0.1 2022/03/10 Bata version (deprecated)
 26. pc3_v2  v2     2022/04/19 first released
             v2.0.1 2022/06/10 pc3_v2 v6 add sx,sy,sz   
             v2.0.2 2022/06/13 pc3_v2 add azimuth offset 
             
 27. pc3_360 v0.0.1 2022/08/16 for integrate 3 sets of module. 
 
@@ -135,7 +137,9 @@
 29. mmWave-1.0.95
     2023/03/24 mrRadar   v1.0.2  header enable/disable in inital
     2023/03/24 trafficMD v0.1.1  header enable/disable in inital
     2023/03/24  trafficMD_I480   ver:2.0.6 header enable/disable in inital
 30. mmWave-1.0.96
     2023/04/07 pc3_V1884R v0.0.2  add try..except in unpack
 
+31. mmWave-1.0.97
+    2023/05/25 pc3_oob v0.0.4 add v7, playback
```

### Comparing `mmWave-0.1.96/mmWave/droneRN.py` & `mmWave-0.1.97/mmWave/droneRN.py`

 * *Files identical despite different names*

### Comparing `mmWave-0.1.96/mmWave/highAccuracy.py` & `mmWave-0.1.97/mmWave/highAccuracy.py`

 * *Files identical despite different names*

### Comparing `mmWave-0.1.96/mmWave/lpdFDS.py` & `mmWave-0.1.97/mmWave/lpdFDS.py`

 * *Files identical despite different names*

### Comparing `mmWave-0.1.96/mmWave/lpdISK.py` & `mmWave-0.1.97/mmWave/lpdISK.py`

 * *Files identical despite different names*

### Comparing `mmWave-0.1.96/mmWave/lpdISK_kv.py` & `mmWave-0.1.97/mmWave/lpdISK_kv.py`

 * *Files identical despite different names*

### Comparing `mmWave-0.1.96/mmWave/lpdISK_v2.py` & `mmWave-0.1.97/mmWave/lpdISK_v2.py`

 * *Files identical despite different names*

### Comparing `mmWave-0.1.96/mmWave/mrRadar.py` & `mmWave-0.1.97/mmWave/mrRadar.py`

 * *Files identical despite different names*

### Comparing `mmWave-0.1.96/mmWave/pc3.py` & `mmWave-0.1.97/mmWave/pc3.py`

 * *Files identical despite different names*

### Comparing `mmWave-0.1.96/mmWave/pc3OVH.py` & `mmWave-0.1.97/mmWave/pc3OVH.py`

 * *Files identical despite different names*

### Comparing `mmWave-0.1.96/mmWave/pc3_360.py` & `mmWave-0.1.97/mmWave/pc3_360.py`

 * *Files identical despite different names*

### Comparing `mmWave-0.1.96/mmWave/pc3_oob.py` & `mmWave-0.1.97/mmWave/pc3_oob.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # People Counting 3D OOB
 # 2022/03/01: alpha
-# 
+# 2023/05/25: v0.0.4
+#
 # parsing People Counting 3D + OOB  
 # hardware: BM-601 
 #     
 # company: Joybien Technologies: www.joybien.com
 # author: Zach Chen
-# v0.0.3
+# v0.0.4
 #===========================================
 # output: V1,V2,V3,V4,V5,V6,V7 and V9 
 # 
 
 import serial
 import time
 import struct
@@ -56,18 +57,18 @@
 	dopplerUnit :float = 0.0
 	rangeUnit :float = 0.0
 	snrUnit :float = 0.0
 
 class Pc3_OOB:
 	
 	Q9 = 1.0 / 2**9 
-	#magicWord =  [b'\x01',b'\x02',b'\x03',b'\x04',b'\x05',b'\x06',b'\x07',b'\x08',b'\0x99']
-	magicWord =  [b'\x02',b'\x01',b'\x04',b'\x03',b'\x06',b'\x05',b'\x08',b'\x07',b'\0x99']
+	#magicWord =  [b'\x02',b'\x01',b'\x04',b'\x03',b'\x06',b'\x05',b'\x08',b'\x07',b'\0x99']  #ori
+	magicWord =  [b'\x01',b'\x02',b'\x03',b'\x04',b'\x05',b'\x06',b'\x07',b'\x08',b'\0x99']
 	typeList = [1,2,3,4,5,6,7,9] 
-	
+	X_CALI_DEGREE = 4.85
 	v2 = []
 	v2df = []
 	
 	port = ""
 	hdr = header
 	u = unitS
 	ss = statistics
@@ -233,15 +234,16 @@
 	def list2df(self,dck,l1,l6,l9):
 		ll1 = pd.DataFrame(l1,columns=self.v1_col_names_rt)
 		ll6 = pd.DataFrame(l6,columns=self.v6_col_names_rt) 
 		ll9 = pd.DataFrame(l9,columns=self.v9_col_names_rt) 
 		 
 		return (dck,ll1,ll6,ll9)
 
-	
+	def x_calibrate(self,x,y):
+		return  x + np.array(y) * np.tan(np.deg2rad(self.X_CALI_DEGREE))
 #
 # TLV: Type-Length-Value
 # read TLV data
 # Usuage:
 # (dck,v1,v6,v9)  = radar.tlvRead(True,df = 'DataFrame')
 # input:
 #     disp: True:print message
@@ -286,21 +288,22 @@
 		self.v2df = ([])
 		v3df = ([])
 		v4df = ([])
 		v5df = ([])
 		v6df = ([])
 		v7df = ([])
 		v9df = ([])
-		 
+		v17simo = []
+		v2simo  = [] 
 		
 		while True:
 			try:
 				ch = self.port.read()
 			except:
-				return self.list2df(False,v1df,v6df,v9df) if (df == 'DataFrame') else (False,v1,v6,v9)
+				return self.list2df(False,v1df,v6df,v9df,v7) if (df == 'DataFrame') else (False,v1,v6,v9,v7)
 				
 			#print(str(ch))
 			if lstate == 'idle':
 				#print(self.magicWord)
 				if ch == self.magicWord[idx]:
 					#print("*** magicWord:"+ "{:02x}".format(ord(ch)) + ":" + str(idx))
 					idx += 1
@@ -310,15 +313,15 @@
 						rangeProfile = b""
 						sbuf = b""
 						self.escapeCount = 0
 				else:
 					#print("not: magicWord state:")
 					idx = 0
 					rangeProfile = b""
-					return self.list2df(False,v1df,v6df,v9df) if (df == 'DataFrame') else (False,v1,v6,v9)
+					return self.list2df(False,v1df,v6df,v9df,v7) if (df == 'DataFrame') else (False,v1,v6,v9,v7)
 		
 			elif lstate == 'header':
 				sbuf += ch
 				idx += 1
 				escapeCount += 1
 				if idx == 32: 
 					#print("------header-----")
@@ -331,36 +334,36 @@
 						self.hdr.platform,self.hdr.frameNumber,
 						self.hdr.timeInCPUcycle,self.hdr.numDetectedObj,
 						self.hdr.numTLVs,self.hdr.subframeNumber) = struct.unpack('8I', sbuf)
 						self.frameNumber = self.hdr.frameNumber
 					except:
 						if self.dbg == True:
 							print("(Header)Improper TLV structure found: ")
-						return self.list2df(False,v1df,v6df,v9df) if (df == 'DataFrame') else (False,v1,v6,v9)
+						return self.list2df(False,v1df,v6df,v9df,v7) if (df == 'DataFrame') else (False,v1,v6,v9,v7)
 					
 					if disp == True:  
 						self.headerShow()
 					
 					tlvCount = self.hdr.numTLVs
 					#print("tlvCount:{:}".format(tlvCount))
 					if self.hdr.numTLVs == 0:
-						return self.list2df(True,v1df,v6df,v9df) if (df == 'DataFrame') else (True,v1,v6,v9)
+						return self.list2df(True,v1df,v6df,v9df,v7) if (df == 'DataFrame') else (True,v1,v6,v9,v7)
 						
 					if self.sm == True:
 						print("(Header)")
 						
 					sbuf = b""
 					idx = 0
 					lstate = 'TL'
 					  
 				elif idx > 64: #44
 					idx = 0
 					sbuf = b''
 					lstate = 'idle'
-					return self.list2df(False,v1df,v6df,v9df) if (df == 'DataFrame') else (False,v1,v6,v9)
+					return self.list2df(False,v1df,v6df,v9df,v7) if (df == 'DataFrame') else (False,v1,v6,v9,v7)
 					
 			elif lstate == 'TL': #TLV Header type/length
 				sbuf += ch
 				idx += 1
 				self.escapeCount += 1
 				
 				if idx == 8:
@@ -372,21 +375,21 @@
 						if ttype not in self.typeList or self.tlvLength > 20000:
 							if self.dbg == True:
 								print("(TL)Improper TL Length(hex):(T){:d} (L){:x} numTLVs:{:d}".format(ttype,self.tlvLength,self.hdr.numTLVs))
 							sbuf = b""
 							idx = 0
 							lstate = 'idle'
 							self.port.flushInput()
-							return self.list2df(False,v1df,v6df,v9df) if (df == 'DataFrame') else (False,v1,v6,v9)
+							return self.list2df(False,v1df,v6df,v9df,v7) if (df == 'DataFrame') else (False,v1,v6,v9,v7)
 							
 					except:
 						if self.dbg == True:
 							print("TL unpack Improper Data Found:")
 						self.port.flushInput()
-						return self.list2df(False,v1df,v6df,v9df) if (df == 'DataFrame') else (False,v1,v6,v9)
+						return self.list2df(False,v1df,v6df,v9df,v7) if (df == 'DataFrame') else (False,v1,v6,v9,v7)
 						
 					
 						
 					unitByteCount,lstate ,plen ,dataBytes,lenCount, numOfPoints = self.tlvTypeInfo(ttype,self.tlvLength,disp)
 					if self.dbg == True:
 						print("unitByteCount={}  lstate ={} , bytes(type+len)={} dataBytes= {} lenCount ={} numOfPoint={}".format(unitByteCount,lstate ,plen ,dataBytes,lenCount, numOfPoints))
 					#if ttype == 10:
@@ -415,15 +418,17 @@
 			elif lstate == 'V1':
 				sbuf += ch
 				idx += 1
 				self.escapeCount += 1
 				if (idx%dataBytes == 0):
 					try:
 						#print(":".join("{:02x}".format(c) for c in sbuf))
-						(x,y,z,d) = struct.unpack('4f', sbuf)
+						(x0,y,z,d) = struct.unpack('4f', sbuf)
+						x = self.x_calibrate(x0,y)
+						
 						if self.dbg == True:
 							print("({:2d}:{:4d})(idx:({:4d}) x:{:.4f} y:{:.4f} z:{:.4f} d:{:.4f}".format(numOfPoints,lenCount,idx,x,y,z,d))
 						
 						if (df == 'DataFrame'):
 							v1df.append((self.hdr.frameNumber,'v1',x,y,z,d)) 
 						else:
 							v1.append((x,y,z,d))
@@ -431,52 +436,52 @@
 						#print("point_cloud_2d.append:[{:d}]".format(len(point_cloud_2d)))
 						sbuf = b""
 						
 					except:
 						if self.dbg == True:
 							print("(6.1)Improper Type 1 Value structure found: ")
 						
-						return self.list2df(False,v1df,v6df,v9df) if (df == 'DataFrame') else (False,v1,v6,v9)
+						return self.list2df(False,v1df,v6df,v9df,v7) if (df == 'DataFrame') else (False,v1,v6,v9,v7)
 				
 				if idx == lenCount:
 					if disp == True:
 						print("v1[{:d}]".format(len(v1)))
 					idx = 0
 					sbuf = b""
 					if tlvCount <= 0: # Back to idle
 						lstate = 'idle'
 						if self.sm == True:
 							print("(V1:{:d})=>(idle) :true".format(tlvCount))
 						
-						return self.list2df(True,v1df,v6df,v9df) if (df == 'DataFrame') else (True,v1,v6,v9)
+						return self.list2df(True,v1df,v6df,v9df,v7) if (df == 'DataFrame') else (True,v1,v6,v9,v7)
 						
 					else: # Go to TL to get others type value
 						lstate = 'TL'
 						if self.sm == True:
 							print("(V1:{:d})=>(TL)".format(tlvCount))
 					
 				elif idx > lenCount or self.escapeCount > self.hdr.totalPackLen:
 					idx = 0
 					sbuf = b""
 					lstate = 'idle'
-					return self.list2df(False,v1df,v6df,v9df) if (df == 'DataFrame') else (False,v1,v6,v9)
+					return self.list2df(False,v1df,v6df,v9df,v7) if (df == 'DataFrame') else (False,v1,v6,v9,v7)
 				
 				
 			
 			elif lstate == 'V2' or lstate == 'V3' or lstate == 'V4' or lstate == 'V5' or lstate == 'V6' or lstate == 'V9':
 				sbuf += ch
 				idx += 1
 				self.escapeCount += 1
 				#if (idx%dataBytes == 0):
 				
 				if lenCount == 0:
 					idx = 0
 					sbuf = b""
 					lstate = 'idle'
-					return self.list2df(False,v1df,v6df,v9df) if (df == 'DataFrame') else (False,v1,v6,v9)
+					return self.list2df(False,v1df,v6df,v9df,v7) if (df == 'DataFrame') else (False,v1,v6,v9,v7)
 				
 				if (idx%lenCount == 0):
 					try:
 						#print(":".join("{:02x}".format(c) for c in sbuf))
 						if lstate == 'V2':
 							rp = struct.unpack('256H', sbuf)
 							rpf = [float(i) * self.Q9 for i in rp] 
@@ -564,145 +569,117 @@
 						#print("point_cloud_2d.append:[{:d}]".format(len(point_cloud_2d)))
 						sbuf = b""
 						#lstate = 'TL'
 						
 					except:
 						if self.dbg == True:
 							print("Improper Type {} Value structure found: ".format(lstate))
-						return self.list2df(False,v1df,v6df,v9df) if (df == 'DataFrame') else (False,v1,v6,v9)
+						return self.list2df(False,v1df,v6df,v9df,v7) if (df == 'DataFrame') else (False,v1,v6,v9,v7)
 				
 				if idx == lenCount:
-					'''
-					if disp == True:
-						if lstate == 'V2':
-							print("v2[{:d}]".format(len(v2)))
-						else:
-							print("v3[{:d}]".format(len(v3)))
-					'''
 					idx = 0
 					sbuf = b""
 					if tlvCount <= 0: # Back to idle
 						if self.sm == True:
 							print("({}:tlvCount({:d})) lenCount:{}=>(idle)".format(lstate,tlvCount,lenCount))
 						lstate = 'idle'
 						
-						return self.list2df(True,v1df,v6df,v9df) if (df == 'DataFrame') else (True,v1,v6,v9)
+						return self.list2df(True,v1df,v6df,v9df,v7) if (df == 'DataFrame') else (True,v1,v6,v9,v7)
 						
 					else: # Go to TL to get others type value
 						if self.sm == True:
 							print("({}:tlvCount({:d})) lenCount:{}=>(TL)".format(lstate,tlvCount,lenCount))
 						lstate = 'TL'
 											
 				elif idx > lenCount or self.escapeCount > self.hdr.totalPackLen:
 					print("(ESC)========type={:} lenth = 0 =============self.escapeCount > self.hdr.totoalPackLen==============================".format(lstate))
 					idx = 0
 					sbuf = b""
 					lstate = 'idle'
-					return self.list2df(False,v1df,v6df,v9df) if (df == 'DataFrame') else (False,v1,v6,v9)
+					return self.list2df(False,v1df,v6df,v9df,v7) if (df == 'DataFrame') else (False,v1,v6,v9,v7)
 				
 					
 			elif lstate == 'V7': 
 				sbuf += ch
 				idx += 1
 				self.escapeCount += 1
 				if (idx%dataBytes == 0):
 					try:
 						#print(":".join("{:02x}".format(c) for c in sbuf))
 						(snr,noise) = struct.unpack('2H', sbuf)
 						v7.append((snr,noise))
 						sbuf = b""
-						
+					
 					except:
 						if self.dbg == True:
 							print("(6.1)Improper Type 6 Value structure found: ")
 						
-						return self.list2df(False,v1df,v6df,v9df) if (df == 'DataFrame') else (False,v1,v6,v9)
+						return self.list2df(False,v1df,v6df,v9df,v7) if (df == 'DataFrame') else (False,v1,v6,v9,v7)
+					
+					if tlvCount <= 0: # Back to idle
+						if self.sm == True:
+							print("({}:tlvCount({:d})) lenCount:{}=>(idle)".format(lstate,tlvCount,lenCount))
+						lstate = 'idle'
+						return self.list2df(True,v1df,v6df,v9df,v7) if (df == 'DataFrame') else (True,v1,v6,v9,v7)
+					
+					
 					
 				if idx == lenCount:
 					if disp == True:
 						print("v7[len:{:d}]".format(len(v7)))
 					idx = 0
 					sbuf = b""
 					if tlvCount <= 0: # Back to idle
 						lstate = 'idle'
 						if self.sm == True:
 							print("(V7:{:d})=>(idle) :true".format(tlvCount))
 						
-						return self.list2df(True,v1df,v6df,v9df) if (df == 'DataFrame') else (True,v1,v6,v9)
+						return self.list2df(True,v1df,v6df,v9df,v7) if (df == 'DataFrame') else (True,v1,v6,v9,v7)
 						
 					else: # Go to TL to get others type value
 						lstate = 'TL'
 						if self.sm == True:
 							print("(V7:{:d})=>(TL)".format(tlvCount))
 							
 					
 				elif idx > lenCount or self.escapeCount > self.hdr.totalPackLen:
 					print("(ESC)========type={:} lenth = 0 =============self.escapeCount > self.hdr.totoalPackLen==============================".format(lstate))
 					idx = 0
 					sbuf = b""
 					lstate = 'idle'
-					return self.list2df(False,v1df,v6df,v9df) if (df == 'DataFrame') else (False,v1,v6,v9)
+					return self.list2df(False,v1df,v6df,v9df,v7) if (df == 'DataFrame') else (False,v1,v6,v9,v7)
 					
 		
-				
-	def v67Simlog(frameNum):
-		global sim_startFN,sim_stopFN
-		s_fn = frameNum + sim_startFN
-		#print("frame number:{:}".format(s_fn))
-		v6d = v6sim[v6sim['fN'] == s_fn]
-		#v6d =  v6dd[v6dd['doppler'] < 0.0]
-		#print(v6d)
-		v7d = v7sim[v7sim['fN'] == s_fn]
-		chk = 0
-		if v6d.count != 0:
-			chk = 1
-		return (chk,v6d,v7d)
-		
 	def getRecordData(self,frameNum):
 		s_fn = frameNum + self.sim_startFN
 		#print("frame number:{:}".format(s_fn))
-		v6d = self.v6simo[self.v6simo['fN'] == s_fn]
-		#v6d =  v6dd[v6dd['doppler'] < 0.0]
-		#print(v6d)
-		v7d = self.v7simo[self.v7simo['fN'] == s_fn]
-		v8d = self.v8simo[self.v8simo['fN'] == s_fn]
-		chk = 0
-		if v6d.count != 0:
-			chk = 1
-		return (chk,v6d,v7d,v8d)
+		v17d = self.v17simo[(self.v17simo.fN == str(s_fn))]
+		v17o = v17d.loc[:,['x','y','z' ,'doppler','snr','noise']].apply(pd.to_numeric)
+		v2d = self.v2simo[self.v2simo['fN'] == str(s_fn)]
+		v2x = v2d.loc[:,['x']] 
+		
+		v2f = []
+		v2o = np.array(v2x)
+		v2f = np.array(eval(v2o[0][0])) 
+		return (v17o,v2f)
 		
+
 	def readFile(self,fileName):
 		#fileName = "pc32021-03-19-10-02-17.csv"  
 		#df = pd.read_csv(fileName, error_bad_lines=False, warn_bad_lines=False) 
 		self.fileName = fileName 
-		#          ['time','fN','type','elv','azimuth','range' ,'doppler','snr','sx', 'sy', 'sz']
-		df = pd.read_csv(self.fileName, names = self.v6_col_names, skiprows = [0,11,12]) 
+		#          ['fN','type','x','y','z' ,'doppler','snr','noise']
+		v17_col_names = ['fN','type','x','y','z' ,'doppler','snr','noise']
+		df = pd.read_csv(self.fileName, names = v17_col_names)
 		df.dropna()
 		#print("------------------- df --------------------shape:{:}".format(df.shape))
 		print(df.info())
-		print(df.info(memory_usage="deep")) 
+		#print(df.info(memory_usage="deep")) 
+		self.v17simo = df[(df.type == 'v17')] 
 		
-		v6simOri = df[(df.type == 'v6')]
-		#print("-------------------v6sim------------:{:}".format(v6simOri.shape))
-		#self.v6simo = v6simOri.loc[:,['fN','elv','azimuth','range','doppler','snr']]
-		self.v6simo = v6simOri.loc[:,['fN','type','elv','azimuth','range' ,'doppler','snr','sx', 'sy', 'sz']]
-		self.v6simo['elv'] = self.v6simo['elv'].astype(float, errors = 'raise') 
-		
-		df7 = pd.read_csv(self.fileName, names = self.v7_col_names, skiprows = [0])  
-		
-		v7simc = df7[df7['type'] == 'v7']
-		self.v7simo  = v7simc.loc[:,['fN','posX','posY','posZ','velX','velY','velZ','accX','accY','accZ','ec0','ec1','ec2','ec3','ec4','ec5','ec6','ec7','ec8','ec9','ec10','ec11','ec12','ec13','ec14','ec15','g','confi','tid']]
-		self.sim_startFN = df['fN'].values[0]
-		self.sim_stopFN  = df['fN'].values[-1]
-		'''
-		print("---------start frame number---------:{:}".format(self.sim_startFN))
-		print("---------stop  frame number---------:{:}".format(self.sim_stopFN))
-		print(self.v7simo)
-		print("-----v8sim data lib-----")
-		'''
-		v8simc = df[df['type'] == 'v8']
-		self.v8simo  = v8simc.loc[:,['fN','type','elv']]
-		self.v8simo.columns = ['fN','type','targetID']
-		#print(self.v8simo)
-		return (self.v6simo,self.v7simo,self.v8simo)
-
-
+		self.sim_startFN = int(df['fN'].values[1])
+		self.sim_stopFN  = int(df['fN'].values[-1])
+		
+		
+		v2simc = df[(df.type == 'v2')]
+		self.v2simo = v2simc.loc[:,['fN','type','x']]
+		return (self.v17simo,self.v2simo)
```

### Comparing `mmWave-0.1.96/mmWave/pc3_v1884R.py` & `mmWave-0.1.97/mmWave/pc3_v1884R.py`

 * *Files identical despite different names*

### Comparing `mmWave-0.1.96/mmWave/pc3_v2.py` & `mmWave-0.1.97/mmWave/pc3_v2.py`

 * *Files identical despite different names*

### Comparing `mmWave-0.1.96/mmWave/pc3_vsd.py` & `mmWave-0.1.97/mmWave/pc3_vsd.py`

 * *Files identical despite different names*

### Comparing `mmWave-0.1.96/mmWave/pc3_vsd_v2.py` & `mmWave-0.1.97/mmWave/pc3_vsd_v2.py`

 * *Files identical despite different names*

### Comparing `mmWave-0.1.96/mmWave/pc3d.py` & `mmWave-0.1.97/mmWave/pc3d.py`

 * *Files identical despite different names*

### Comparing `mmWave-0.1.96/mmWave/pc3d_kv.py` & `mmWave-0.1.97/mmWave/pc3d_kv.py`

 * *Files identical despite different names*

### Comparing `mmWave-0.1.96/mmWave/pct.py` & `mmWave-0.1.97/mmWave/pct.py`

 * *Files identical despite different names*

### Comparing `mmWave-0.1.96/mmWave/people3D.py` & `mmWave-0.1.97/mmWave/people3D.py`

 * *Files identical despite different names*

### Comparing `mmWave-0.1.96/mmWave/peopleMB.py` & `mmWave-0.1.97/mmWave/peopleMB.py`

 * *Files identical despite different names*

### Comparing `mmWave-0.1.96/mmWave/roadwayTMD_kv.py` & `mmWave-0.1.97/mmWave/roadwayTMD_kv.py`

 * *Files identical despite different names*

### Comparing `mmWave-0.1.96/mmWave/srradar.py` & `mmWave-0.1.97/mmWave/srradar.py`

 * *Files identical despite different names*

### Comparing `mmWave-0.1.96/mmWave/surfaceVD.py` & `mmWave-0.1.97/mmWave/surfaceVD.py`

 * *Files identical despite different names*

### Comparing `mmWave-0.1.96/mmWave/trafficMD.py` & `mmWave-0.1.97/mmWave/trafficMD.py`

 * *Files identical despite different names*

### Comparing `mmWave-0.1.96/mmWave/trafficMD_I480.py` & `mmWave-0.1.97/mmWave/trafficMD_I480.py`

 * *Files identical despite different names*

### Comparing `mmWave-0.1.96/mmWave/trafficMD_kv.py` & `mmWave-0.1.97/mmWave/trafficMD_kv.py`

 * *Files identical despite different names*

### Comparing `mmWave-0.1.96/mmWave/vehicleOD.py` & `mmWave-0.1.97/mmWave/vehicleOD.py`

 * *Files identical despite different names*

### Comparing `mmWave-0.1.96/mmWave/vehicleODHeatMap.py` & `mmWave-0.1.97/mmWave/vehicleODHeatMap.py`

 * *Files identical despite different names*

### Comparing `mmWave-0.1.96/mmWave/vehicleODR.py` & `mmWave-0.1.97/mmWave/vehicleODR.py`

 * *Files identical despite different names*

### Comparing `mmWave-0.1.96/mmWave/vitalsign.py` & `mmWave-0.1.97/mmWave/vitalsign.py`

 * *Files identical despite different names*

### Comparing `mmWave-0.1.96/mmWave/vitalsign_kv.py` & `mmWave-0.1.97/mmWave/vitalsign_kv.py`

 * *Files identical despite different names*

### Comparing `mmWave-0.1.96/mmWave.egg-info/PKG-INFO` & `mmWave-0.1.97/mmWave.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmWave
-Version: 0.1.96
+Version: 0.1.97
 Summary: Joybien mmWave (Batman-101/201/301/501/601) library
 Home-page: http://www.joybien.com
 Download-URL: https://pypi.org/project/mmWave
 Author: Bighead Chen
 Author-email: zach_chen@joybien.com
 Project-URL: API Source Code, https://github.com/bigheadG/mmWave
 Classifier: Programming Language :: Python :: 3
@@ -56,14 +56,16 @@
             v0.0.2 2022/02/07 format revised
             v0.1.0 2022/06/02 fit v3 data
             v1.0.0 2022/06/08 change data get method
             v1.0.1 :2022/06/09 added headerShowAll()
 24. pc3_oob v0.0.1 2022/03/01 first released
             v0.0.2 2022/03/01 bug fix
             v0.0.3 2022/03/03
+            v0.0.4 :2023/05/25 @v1.0.97 add v7, playback
+            
 25. pc3_vsd v0.0.1 2022/03/10 Bata version (deprecated)
 26. pc3_v2  v2     2022/04/19 first released
             v2.0.1 2022/06/10 pc3_v2 v6 add sx,sy,sz   
             v2.0.2 2022/06/13 pc3_v2 add azimuth offset 
             
 27. pc3_360 v0.0.1 2022/08/16 for integrate 3 sets of module. 
 
@@ -149,7 +151,9 @@
 29. mmWave-1.0.95
     2023/03/24 mrRadar   v1.0.2  header enable/disable in inital
     2023/03/24 trafficMD v0.1.1  header enable/disable in inital
     2023/03/24  trafficMD_I480   ver:2.0.6 header enable/disable in inital
 30. mmWave-1.0.96
     2023/04/07 pc3_V1884R v0.0.2  add try..except in unpack
 
+31. mmWave-1.0.97
+    2023/05/25 pc3_oob v0.0.4 add v7, playback
```

### Comparing `mmWave-0.1.96/mmWave.egg-info/SOURCES.txt` & `mmWave-0.1.97/mmWave.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mmWave-0.1.96/setup.py` & `mmWave-0.1.97/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,14 +94,16 @@
 #               :v0.0.2 :2022/02/07 format revised @v0.1.63
 #               :v0.1.0 :2022/06/02 tune to fit v3 data
 #               :v1.0.0 :2022/06/08 change get Uart Data Method
 #               :v1.0.1 :2022/06/09 added headerShowAll()
 # pc3_oob.py    :v0.0.1 :2022/03/01 @v0.1.64
 #	            :v0.0.2 :2022/03/01 @v0.1.65 bug fix
 #               :v0.0.3 :2022/03/03 @v1.0.66
+#               :v0.0.4 :2023/05/25 @v1.0.97 add v7, playback
+#
 # @v1.0.67 modified description
 #
 # @v1.0.68
 # pc3_vsd.py    :v0.0.1 :2022/03/10 bata version
 #
 # @v1.0.70
 # pc3_v2.py     :v2.0 :2022/04/19
@@ -171,23 +173,25 @@
 #    2023/03/24 mrRadar   v1.0.2  header enable/disable in inital
 #    2023/03/24 trafficMD v0.1.1  header enable/disable in inital
 #    2023/03/24	trafficMD_I480   ver:2.0.6 header enable/disable in inital
 #
 # @1.0.96
 #    2023/04/07 pc3_V1884R v0.0.2  add try..except in unpack
 #
+# @1.0.97
+#   2023/05/25 pc3_oob v0.0.4 add v7 and playback
 
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="mmWave",
-    version="0.1.96",
+    version="0.1.97",
     author="Bighead Chen",
     author_email="zach_chen@joybien.com",
     description="Joybien mmWave (Batman-101/201/301/501/601) library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="http://www.joybien.com",
     download_url="https://pypi.org/project/mmWave",
```

