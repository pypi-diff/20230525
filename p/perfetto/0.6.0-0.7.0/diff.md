# Comparing `tmp/perfetto-0.6.0.tar.gz` & `tmp/perfetto-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "perfetto-0.6.0.tar", last modified: Thu Oct 27 15:38:57 2022, max compression
+gzip compressed data, was "perfetto-0.7.0.tar", last modified: Thu May 25 13:45:23 2023, max compression
```

## Comparing `perfetto-0.6.0.tar` & `perfetto-0.7.0.tar`

### file list

```diff
@@ -1,24 +1,33 @@
-drwxr-x---   0 lalitm   (325227) primarygroup (89939)        0 2022-10-27 15:38:57.245893 perfetto-0.6.0/
--rw-r-----   0 lalitm   (325227) primarygroup (89939)      779 2022-10-27 15:38:57.245893 perfetto-0.6.0/PKG-INFO
-drwxr-x---   0 lalitm   (325227) primarygroup (89939)        0 2022-10-27 15:38:57.241893 perfetto-0.6.0/perfetto/
--rw-r-----   0 lalitm   (325227) primarygroup (89939)      773 2022-06-13 16:18:02.269595 perfetto-0.6.0/perfetto/__init__.py
-drwxr-x---   0 lalitm   (325227) primarygroup (89939)        0 2022-10-27 15:38:57.241893 perfetto-0.6.0/perfetto/batch_trace_processor/
--rw-r-----   0 lalitm   (325227) primarygroup (89939)      807 2022-06-13 16:18:02.273595 perfetto-0.6.0/perfetto/batch_trace_processor/__init__.py
--rw-r-----   0 lalitm   (325227) primarygroup (89939)    13893 2022-08-30 15:29:22.795885 perfetto-0.6.0/perfetto/batch_trace_processor/api.py
--rw-r-----   0 lalitm   (325227) primarygroup (89939)     1014 2022-06-13 16:18:02.273595 perfetto-0.6.0/perfetto/batch_trace_processor/platform.py
-drwxr-x---   0 lalitm   (325227) primarygroup (89939)        0 2022-10-27 15:38:57.245893 perfetto-0.6.0/perfetto/trace_processor/
--rw-r-----   0 lalitm   (325227) primarygroup (89939)      924 2022-06-13 16:18:02.273595 perfetto-0.6.0/perfetto/trace_processor/__init__.py
--rw-r-----   0 lalitm   (325227) primarygroup (89939)    14246 2022-10-26 17:18:19.236814 perfetto-0.6.0/perfetto/trace_processor/api.py
--rw-r-----   0 lalitm   (325227) primarygroup (89939)     2568 2022-07-04 14:48:53.686016 perfetto-0.6.0/perfetto/trace_processor/http.py
--rw-r--r--   0 lalitm   (325227) primarygroup (89939)    37295 2022-10-27 13:47:28.731805 perfetto-0.6.0/perfetto/trace_processor/metrics.descriptor
--rw-r-----   0 lalitm   (325227) primarygroup (89939)     3009 2022-07-14 12:47:37.414657 perfetto-0.6.0/perfetto/trace_processor/platform.py
--rw-r-----   0 lalitm   (325227) primarygroup (89939)     2815 2022-07-04 14:48:53.686016 perfetto-0.6.0/perfetto/trace_processor/protos.py
--rw-r--r--   0 lalitm   (325227) primarygroup (89939)     2195 2022-10-25 15:27:03.050399 perfetto-0.6.0/perfetto/trace_processor/shell.py
--rw-r--r--   0 lalitm   (325227) primarygroup (89939)     5729 2022-10-27 14:02:33.585756 perfetto-0.6.0/perfetto/trace_processor/trace_processor.descriptor
-drwxr-x---   0 lalitm   (325227) primarygroup (89939)        0 2022-10-27 15:38:57.245893 perfetto-0.6.0/perfetto/trace_uri_resolver/
--rw-r-----   0 lalitm   (325227) primarygroup (89939)        0 2022-07-04 14:48:53.690016 perfetto-0.6.0/perfetto/trace_uri_resolver/__init__.py
--rw-r-----   0 lalitm   (325227) primarygroup (89939)     1186 2022-06-13 16:18:02.273595 perfetto-0.6.0/perfetto/trace_uri_resolver/path.py
--rw-r-----   0 lalitm   (325227) primarygroup (89939)     2916 2022-06-13 16:18:02.273595 perfetto-0.6.0/perfetto/trace_uri_resolver/registry.py
--rw-r-----   0 lalitm   (325227) primarygroup (89939)     7613 2022-08-30 15:29:22.795885 perfetto-0.6.0/perfetto/trace_uri_resolver/resolver.py
--rw-r-----   0 lalitm   (325227) primarygroup (89939)     3952 2022-07-04 14:48:53.690016 perfetto-0.6.0/perfetto/trace_uri_resolver/util.py
--rw-r-----   0 lalitm   (325227) primarygroup (89939)     1127 2022-10-27 14:27:26.677130 perfetto-0.6.0/setup.py
+drwxr-xr-x   0 lalitm   (325227) primarygroup (89939)        0 2023-05-25 13:45:23.411645 perfetto-0.7.0/
+-rw-r-----   0 lalitm   (325227) primarygroup (89939)    10689 2023-01-27 10:13:53.000000 perfetto-0.7.0/LICENSE
+-rw-r--r--   0 lalitm   (325227) primarygroup (89939)      762 2023-05-25 13:45:23.411645 perfetto-0.7.0/PKG-INFO
+-rw-r-----   0 lalitm   (325227) primarygroup (89939)      456 2023-01-27 10:13:53.000000 perfetto-0.7.0/README.md
+drwxr-xr-x   0 lalitm   (325227) primarygroup (89939)        0 2023-05-25 13:45:23.407645 perfetto-0.7.0/perfetto/
+-rw-r-----   0 lalitm   (325227) primarygroup (89939)      773 2023-01-27 10:13:53.000000 perfetto-0.7.0/perfetto/__init__.py
+drwxr-xr-x   0 lalitm   (325227) primarygroup (89939)        0 2023-05-25 13:45:23.407645 perfetto-0.7.0/perfetto/batch_trace_processor/
+-rw-r-----   0 lalitm   (325227) primarygroup (89939)      807 2023-01-27 10:13:53.000000 perfetto-0.7.0/perfetto/batch_trace_processor/__init__.py
+-rw-r--r--   0 lalitm   (325227) primarygroup (89939)    13893 2023-03-27 16:08:03.000000 perfetto-0.7.0/perfetto/batch_trace_processor/api.py
+-rw-r-----   0 lalitm   (325227) primarygroup (89939)     1014 2023-01-27 10:13:53.000000 perfetto-0.7.0/perfetto/batch_trace_processor/platform.py
+drwxr-xr-x   0 lalitm   (325227) primarygroup (89939)        0 2023-05-25 13:45:23.411645 perfetto-0.7.0/perfetto/trace_processor/
+-rw-r-----   0 lalitm   (325227) primarygroup (89939)      924 2023-01-27 10:13:53.000000 perfetto-0.7.0/perfetto/trace_processor/__init__.py
+-rw-r-----   0 lalitm   (325227) primarygroup (89939)    14285 2023-05-24 20:08:51.000000 perfetto-0.7.0/perfetto/trace_processor/api.py
+-rw-r--r--   0 lalitm   (325227) primarygroup (89939)     2568 2023-03-27 16:08:03.000000 perfetto-0.7.0/perfetto/trace_processor/http.py
+-rw-r-----   0 lalitm   (325227) primarygroup (89939)    43184 2023-05-23 19:10:47.000000 perfetto-0.7.0/perfetto/trace_processor/metrics.descriptor
+-rw-r--r--   0 lalitm   (325227) primarygroup (89939)     3009 2023-03-27 16:08:03.000000 perfetto-0.7.0/perfetto/trace_processor/platform.py
+-rw-r--r--   0 lalitm   (325227) primarygroup (89939)     2930 2023-03-27 16:08:03.000000 perfetto-0.7.0/perfetto/trace_processor/protos.py
+-rw-r--r--   0 lalitm   (325227) primarygroup (89939)     2227 2023-03-27 16:08:03.000000 perfetto-0.7.0/perfetto/trace_processor/shell.py
+-rw-r-----   0 lalitm   (325227) primarygroup (89939)     6315 2023-05-23 19:10:47.000000 perfetto-0.7.0/perfetto/trace_processor/trace_processor.descriptor
+drwxr-xr-x   0 lalitm   (325227) primarygroup (89939)        0 2023-05-25 13:45:23.411645 perfetto-0.7.0/perfetto/trace_uri_resolver/
+-rw-r-----   0 lalitm   (325227) primarygroup (89939)        0 2023-01-27 10:13:53.000000 perfetto-0.7.0/perfetto/trace_uri_resolver/__init__.py
+-rw-r-----   0 lalitm   (325227) primarygroup (89939)     1186 2023-01-27 10:13:53.000000 perfetto-0.7.0/perfetto/trace_uri_resolver/path.py
+-rw-r-----   0 lalitm   (325227) primarygroup (89939)     2916 2023-01-27 10:13:53.000000 perfetto-0.7.0/perfetto/trace_uri_resolver/registry.py
+-rw-r--r--   0 lalitm   (325227) primarygroup (89939)     7613 2023-03-27 16:08:03.000000 perfetto-0.7.0/perfetto/trace_uri_resolver/resolver.py
+-rw-r--r--   0 lalitm   (325227) primarygroup (89939)     3952 2023-03-27 16:08:03.000000 perfetto-0.7.0/perfetto/trace_uri_resolver/util.py
+drwxr-xr-x   0 lalitm   (325227) primarygroup (89939)        0 2023-05-25 13:45:23.407645 perfetto-0.7.0/perfetto.egg-info/
+-rw-r--r--   0 lalitm   (325227) primarygroup (89939)      762 2023-05-25 13:45:23.000000 perfetto-0.7.0/perfetto.egg-info/PKG-INFO
+-rw-r--r--   0 lalitm   (325227) primarygroup (89939)      826 2023-05-25 13:45:23.000000 perfetto-0.7.0/perfetto.egg-info/SOURCES.txt
+-rw-r--r--   0 lalitm   (325227) primarygroup (89939)        1 2023-05-25 13:45:23.000000 perfetto-0.7.0/perfetto.egg-info/dependency_links.txt
+-rw-r--r--   0 lalitm   (325227) primarygroup (89939)        9 2023-05-25 13:45:23.000000 perfetto-0.7.0/perfetto.egg-info/requires.txt
+-rw-r--r--   0 lalitm   (325227) primarygroup (89939)        9 2023-05-25 13:45:23.000000 perfetto-0.7.0/perfetto.egg-info/top_level.txt
+-rw-r--r--   0 lalitm   (325227) primarygroup (89939)       38 2023-05-25 13:45:23.411645 perfetto-0.7.0/setup.cfg
+-rw-r--r--   0 lalitm   (325227) primarygroup (89939)     1127 2023-05-25 13:40:38.000000 perfetto-0.7.0/setup.py
```

### Comparing `perfetto-0.6.0/PKG-INFO` & `perfetto-0.7.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,19 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: perfetto
-Version: 0.6.0
+Version: 0.7.0
 Summary: Python API for Perfetto's Trace Processor
 Home-page: https://perfetto.dev/
+Download-URL: https://github.com/google/perfetto/archive/refs/tags/v30.0.tar.gz
 Author: Perfetto
 Author-email: perfetto-pypi@google.com
 License: apache-2.0
-Download-URL: https://github.com/google/perfetto/archive/refs/tags/v30.0.tar.gz
-Description: UNKNOWN
 Keywords: trace processor,tracing,perfetto
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+License-File: LICENSE
```

### Comparing `perfetto-0.6.0/perfetto/__init__.py` & `perfetto-0.7.0/perfetto/__init__.py`

 * *Files identical despite different names*

### Comparing `perfetto-0.6.0/perfetto/batch_trace_processor/__init__.py` & `perfetto-0.7.0/perfetto/batch_trace_processor/__init__.py`

 * *Files identical despite different names*

### Comparing `perfetto-0.6.0/perfetto/batch_trace_processor/api.py` & `perfetto-0.7.0/perfetto/batch_trace_processor/api.py`

 * *Files identical despite different names*

### Comparing `perfetto-0.6.0/perfetto/batch_trace_processor/platform.py` & `perfetto-0.7.0/perfetto/batch_trace_processor/platform.py`

 * *Files identical despite different names*

### Comparing `perfetto-0.6.0/perfetto/trace_processor/__init__.py` & `perfetto-0.7.0/perfetto/trace_processor/__init__.py`

 * *Files identical despite different names*

### Comparing `perfetto-0.6.0/perfetto/trace_processor/api.py` & `perfetto-0.7.0/perfetto/trace_processor/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,15 @@
 
     def __repr__(self):
       return self.__dict__
 
   class QueryResultIterator:
 
     def __init__(self, column_names, batches):
-      self.__column_names = column_names
+      self.__column_names = list(column_names)
       self.__column_count = 0
       self.__count = 0
       self.__cells = []
       self.__data_lists = [[], [], [], [], [], []]
       self.__data_lists_index = [0, 0, 0, 0, 0, 0]
       self.__current_index = 0
 
@@ -363,11 +363,13 @@
     self.close()
     return False
 
   def close(self):
     if hasattr(self, 'subprocess'):
       self.subprocess.kill()
       self.subprocess.wait()
-    self.http.conn.close()
+
+    if hasattr(self, 'http'):
+      self.http.conn.close()
 
   def __del__(self):
     self.close()
```

### Comparing `perfetto-0.6.0/perfetto/trace_processor/http.py` & `perfetto-0.7.0/perfetto/trace_processor/http.py`

 * *Files identical despite different names*

### Comparing `perfetto-0.6.0/perfetto/trace_processor/metrics.descriptor` & `perfetto-0.7.0/perfetto/trace_processor/metrics.descriptor`

 * *Files 10% similar despite different names*

```diff
@@ -1,2331 +1,2699 @@
-00000000: 0ac0 030a 3670 726f 746f 732f 7065 7266  ....6protos/perf
+00000000: 0ad2 030a 3670 726f 746f 732f 7065 7266  ....6protos/perf
 00000010: 6574 746f 2f6d 6574 7269 6373 2f61 6e64  etto/metrics/and
 00000020: 726f 6964 2f70 726f 6365 7373 5f6d 6574  roid/process_met
 00000030: 6164 6174 612e 7072 6f74 6f12 0f70 6572  adata.proto..per
-00000040: 6665 7474 6f2e 7072 6f74 6f73 22f4 020a  fetto.protos"...
+00000040: 6665 7474 6f2e 7072 6f74 6f73 2286 030a  fetto.protos"...
 00000050: 1641 6e64 726f 6964 5072 6f63 6573 734d  .AndroidProcessM
 00000060: 6574 6164 6174 6112 120a 046e 616d 6518  etadata....name.
 00000070: 0120 0128 0952 046e 616d 6512 100a 0375  . .(.R.name....u
 00000080: 6964 1802 2001 2803 5203 7569 6412 490a  id.. .(.R.uid.I.
 00000090: 0770 6163 6b61 6765 1807 2001 280b 322f  .package.. .(.2/
 000000a0: 2e70 6572 6665 7474 6f2e 7072 6f74 6f73  .perfetto.protos
 000000b0: 2e41 6e64 726f 6964 5072 6f63 6573 734d  .AndroidProcessM
 000000c0: 6574 6164 6174 612e 5061 636b 6167 6552  etadata.PackageR
 000000d0: 0770 6163 6b61 6765 1259 0a10 7061 636b  .package.Y..pack
 000000e0: 6167 6573 5f66 6f72 5f75 6964 1808 2003  ages_for_uid.. .
 000000f0: 280b 322f 2e70 6572 6665 7474 6f2e 7072  (.2/.perfetto.pr
 00000100: 6f74 6f73 2e41 6e64 726f 6964 5072 6f63  otos.AndroidProc
 00000110: 6573 734d 6574 6164 6174 612e 5061 636b  essMetadata.Pack
 00000120: 6167 6552 0e70 6163 6b61 6765 7346 6f72  ageR.packagesFor
-00000130: 5569 641a 760a 0750 6163 6b61 6765 1221  Uid.v..Package.!
-00000140: 0a0c 7061 636b 6167 655f 6e61 6d65 1801  ..package_name..
-00000150: 2001 2809 520b 7061 636b 6167 654e 616d   .(.R.packageNam
-00000160: 6512 280a 1061 706b 5f76 6572 7369 6f6e  e.(..apk_version
-00000170: 5f63 6f64 6518 0220 0128 0352 0e61 706b  _code.. .(.R.apk
-00000180: 5665 7273 696f 6e43 6f64 6512 1e0a 0a64  VersionCode....d
-00000190: 6562 7567 6761 626c 6518 0320 0128 0852  ebuggable.. .(.R
-000001a0: 0a64 6562 7567 6761 626c 654a 0408 0310  .debuggableJ....
-000001b0: 044a 0408 0410 054a 0408 0510 064a 0408  .J.....J.....J..
-000001c0: 0610 070a b406 0a43 7072 6f74 6f73 2f70  .......Cprotos/p
-000001d0: 6572 6665 7474 6f2f 6d65 7472 6963 732f  erfetto/metrics/
-000001e0: 616e 6472 6f69 642f 616e 6472 6f69 645f  android/android_
-000001f0: 6672 616d 655f 7469 6d65 6c69 6e65 5f6d  frame_timeline_m
-00000200: 6574 7269 632e 7072 6f74 6f12 0f70 6572  etric.proto..per
-00000210: 6665 7474 6f2e 7072 6f74 6f73 1a36 7072  fetto.protos.6pr
-00000220: 6f74 6f73 2f70 6572 6665 7474 6f2f 6d65  otos/perfetto/me
-00000230: 7472 6963 732f 616e 6472 6f69 642f 7072  trics/android/pr
-00000240: 6f63 6573 735f 6d65 7461 6461 7461 2e70  ocess_metadata.p
-00000250: 726f 746f 22a3 050a 1a41 6e64 726f 6964  roto"....Android
-00000260: 4672 616d 6554 696d 656c 696e 654d 6574  FrameTimelineMet
-00000270: 7269 6312 210a 0c74 6f74 616c 5f66 7261  ric.!..total_fra
-00000280: 6d65 7318 0420 0128 0352 0b74 6f74 616c  mes.. .(.R.total
-00000290: 4672 616d 6573 122a 0a11 6d69 7373 6564  Frames.*..missed
-000002a0: 5f61 7070 5f66 7261 6d65 7318 0520 0128  _app_frames.. .(
-000002b0: 0352 0f6d 6973 7365 6441 7070 4672 616d  .R.missedAppFram
-000002c0: 6573 1256 0a07 7072 6f63 6573 7318 0220  es.V..process.. 
-000002d0: 0328 0b32 3c2e 7065 7266 6574 746f 2e70  .(.2<.perfetto.p
-000002e0: 726f 746f 732e 416e 6472 6f69 6446 7261  rotos.AndroidFra
-000002f0: 6d65 5469 6d65 6c69 6e65 4d65 7472 6963  meTimelineMetric
-00000300: 2e50 726f 6365 7373 4272 6561 6b64 6f77  .ProcessBreakdow
-00000310: 6e52 0770 726f 6365 7373 1ad7 030a 1050  nR.process.....P
-00000320: 726f 6365 7373 4272 6561 6b64 6f77 6e12  rocessBreakdown.
-00000330: 410a 0770 726f 6365 7373 1803 2001 280b  A..process.. .(.
-00000340: 3227 2e70 6572 6665 7474 6f2e 7072 6f74  2'.perfetto.prot
-00000350: 6f73 2e41 6e64 726f 6964 5072 6f63 6573  os.AndroidProces
-00000360: 734d 6574 6164 6174 6152 0770 726f 6365  sMetadataR.proce
-00000370: 7373 1221 0a0c 746f 7461 6c5f 6672 616d  ss.!..total_fram
-00000380: 6573 1804 2001 2803 520b 746f 7461 6c46  es.. .(.R.totalF
-00000390: 7261 6d65 7312 230a 0d6d 6973 7365 645f  rames.#..missed_
-000003a0: 6672 616d 6573 1805 2001 2803 520c 6d69  frames.. .(.R.mi
-000003b0: 7373 6564 4672 616d 6573 122a 0a11 6d69  ssedFrames.*..mi
-000003c0: 7373 6564 5f61 7070 5f66 7261 6d65 7318  ssed_app_frames.
-000003d0: 0620 0128 0352 0f6d 6973 7365 6441 7070  . .(.R.missedApp
-000003e0: 4672 616d 6573 1228 0a10 6d69 7373 6564  Frames.(..missed
-000003f0: 5f73 665f 6672 616d 6573 1807 2001 2803  _sf_frames.. .(.
-00000400: 520e 6d69 7373 6564 5366 4672 616d 6573  R.missedSfFrames
-00000410: 1222 0a0d 6672 616d 655f 6475 725f 6d61  ."..frame_dur_ma
-00000420: 7818 0820 0128 0352 0b66 7261 6d65 4475  x.. .(.R.frameDu
-00000430: 724d 6178 1222 0a0d 6672 616d 655f 6475  rMax."..frame_du
-00000440: 725f 6176 6718 0920 0128 0352 0b66 7261  r_avg.. .(.R.fra
-00000450: 6d65 4475 7241 7667 1222 0a0d 6672 616d  meDurAvg."..fram
-00000460: 655f 6475 725f 7035 3018 0a20 0128 0352  e_dur_p50.. .(.R
-00000470: 0b66 7261 6d65 4475 7250 3530 1222 0a0d  .frameDurP50."..
-00000480: 6672 616d 655f 6475 725f 7039 3018 0b20  frame_dur_p90.. 
-00000490: 0128 0352 0b66 7261 6d65 4475 7250 3930  .(.R.frameDurP90
-000004a0: 1222 0a0d 6672 616d 655f 6475 725f 7039  ."..frame_dur_p9
-000004b0: 3518 0c20 0128 0352 0b66 7261 6d65 4475  5.. .(.R.frameDu
-000004c0: 7250 3935 1222 0a0d 6672 616d 655f 6475  rP95."..frame_du
-000004d0: 725f 7039 3918 0d20 0128 0352 0b66 7261  r_p99.. .(.R.fra
-000004e0: 6d65 4475 7250 3939 4a04 0801 1002 4a04  meDurP99J.....J.
-000004f0: 0802 1003 4a04 0801 1002 0aa4 080a 3170  ....J.........1p
-00000500: 726f 746f 732f 7065 7266 6574 746f 2f6d  rotos/perfetto/m
-00000510: 6574 7269 6373 2f61 6e64 726f 6964 2f62  etrics/android/b
-00000520: 6174 745f 6d65 7472 6963 2e70 726f 746f  att_metric.proto
-00000530: 120f 7065 7266 6574 746f 2e70 726f 746f  ..perfetto.proto
-00000540: 7322 dd07 0a14 416e 6472 6f69 6442 6174  s"....AndroidBat
-00000550: 7465 7279 4d65 7472 6963 1260 0a10 6261  teryMetric.`..ba
-00000560: 7474 6572 795f 636f 756e 7465 7273 1801  ttery_counters..
-00000570: 2003 280b 3235 2e70 6572 6665 7474 6f2e   .(.25.perfetto.
-00000580: 7072 6f74 6f73 2e41 6e64 726f 6964 4261  protos.AndroidBa
-00000590: 7474 6572 794d 6574 7269 632e 4261 7474  tteryMetric.Batt
-000005a0: 6572 7943 6f75 6e74 6572 7352 0f62 6174  eryCountersR.bat
-000005b0: 7465 7279 436f 756e 7465 7273 1266 0a12  teryCounters.f..
-000005c0: 6261 7474 6572 795f 6167 6772 6567 6174  battery_aggregat
-000005d0: 6573 1802 2001 280b 3237 2e70 6572 6665  es.. .(.27.perfe
-000005e0: 7474 6f2e 7072 6f74 6f73 2e41 6e64 726f  tto.protos.Andro
-000005f0: 6964 4261 7474 6572 794d 6574 7269 632e  idBatteryMetric.
-00000600: 4261 7474 6572 7941 6767 7265 6761 7465  BatteryAggregate
-00000610: 7352 1162 6174 7465 7279 4167 6772 6567  sR.batteryAggreg
-00000620: 6174 6573 125a 0a0e 7375 7370 656e 645f  ates.Z..suspend_
-00000630: 7065 7269 6f64 1803 2003 280b 3233 2e70  period.. .(.23.p
-00000640: 6572 6665 7474 6f2e 7072 6f74 6f73 2e41  erfetto.protos.A
-00000650: 6e64 726f 6964 4261 7474 6572 794d 6574  ndroidBatteryMet
-00000660: 7269 632e 5375 7370 656e 6450 6572 696f  ric.SuspendPerio
-00000670: 6452 0d73 7573 7065 6e64 5065 7269 6f64  dR.suspendPeriod
-00000680: 1ad2 010a 0f42 6174 7465 7279 436f 756e  .....BatteryCoun
-00000690: 7465 7273 1221 0a0c 7469 6d65 7374 616d  ters.!..timestam
-000006a0: 705f 6e73 1801 2001 2803 520b 7469 6d65  p_ns.. .(.R.time
-000006b0: 7374 616d 704e 7312 2c0a 1263 6861 7267  stampNs.,..charg
-000006c0: 655f 636f 756e 7465 725f 7561 6818 0220  e_counter_uah.. 
-000006d0: 0128 0152 1063 6861 7267 6543 6f75 6e74  .(.R.chargeCount
-000006e0: 6572 5561 6812 290a 1063 6170 6163 6974  erUah.)..capacit
-000006f0: 795f 7065 7263 656e 7418 0320 0128 0252  y_percent.. .(.R
-00000700: 0f63 6170 6163 6974 7950 6572 6365 6e74  .capacityPercent
-00000710: 121d 0a0a 6375 7272 656e 745f 7561 1804  ....current_ua..
-00000720: 2001 2801 5209 6375 7272 656e 7455 6112   .(.R.currentUa.
-00000730: 240a 0e63 7572 7265 6e74 5f61 7667 5f75  $..current_avg_u
-00000740: 6118 0520 0128 0152 0c63 7572 7265 6e74  a.. .(.R.current
-00000750: 4176 6755 611a f402 0a11 4261 7474 6572  AvgUa.....Batter
-00000760: 7941 6767 7265 6761 7465 7312 2d0a 1374  yAggregates.-..t
-00000770: 6f74 616c 5f73 6372 6565 6e5f 6f66 665f  otal_screen_off_
-00000780: 6e73 1801 2001 2803 5210 746f 7461 6c53  ns.. .(.R.totalS
-00000790: 6372 6565 6e4f 6666 4e73 122b 0a12 746f  creenOffNs.+..to
-000007a0: 7461 6c5f 7363 7265 656e 5f6f 6e5f 6e73  tal_screen_on_ns
-000007b0: 1802 2001 2803 520f 746f 7461 6c53 6372  .. .(.R.totalScr
-000007c0: 6565 6e4f 6e4e 7312 2f0a 1474 6f74 616c  eenOnNs./..total
-000007d0: 5f73 6372 6565 6e5f 646f 7a65 5f6e 7318  _screen_doze_ns.
-000007e0: 0320 0128 0352 1174 6f74 616c 5363 7265  . .(.R.totalScre
-000007f0: 656e 446f 7a65 4e73 122a 0a11 746f 7461  enDozeNs.*..tota
-00000800: 6c5f 7761 6b65 6c6f 636b 5f6e 7318 0420  l_wakelock_ns.. 
-00000810: 0128 0352 0f74 6f74 616c 5761 6b65 6c6f  .(.R.totalWakelo
-00000820: 636b 4e73 1219 0a08 736c 6565 705f 6e73  ckNs....sleep_ns
-00000830: 1805 2001 2803 5207 736c 6565 704e 7312  .. .(.R.sleepNs.
-00000840: 2d0a 1373 6c65 6570 5f73 6372 6565 6e5f  -..sleep_screen_
-00000850: 6f66 665f 6e73 1806 2001 2803 5210 736c  off_ns.. .(.R.sl
-00000860: 6565 7053 6372 6565 6e4f 6666 4e73 122b  eepScreenOffNs.+
-00000870: 0a12 736c 6565 705f 7363 7265 656e 5f6f  ..sleep_screen_o
-00000880: 6e5f 6e73 1807 2001 2803 520f 736c 6565  n_ns.. .(.R.slee
-00000890: 7053 6372 6565 6e4f 6e4e 7312 2f0a 1473  pScreenOnNs./..s
-000008a0: 6c65 6570 5f73 6372 6565 6e5f 646f 7a65  leep_screen_doze
-000008b0: 5f6e 7318 0820 0128 0352 1173 6c65 6570  _ns.. .(.R.sleep
-000008c0: 5363 7265 656e 446f 7a65 4e73 1a53 0a0d  ScreenDozeNs.S..
-000008d0: 5375 7370 656e 6450 6572 696f 6412 210a  SuspendPeriod.!.
-000008e0: 0c74 696d 6573 7461 6d70 5f6e 7318 0120  .timestamp_ns.. 
-000008f0: 0128 0352 0b74 696d 6573 7461 6d70 4e73  .(.R.timestampNs
-00000900: 121f 0a0b 6475 7261 7469 6f6e 5f6e 7318  ....duration_ns.
-00000910: 0220 0128 0352 0a64 7572 6174 696f 6e4e  . .(.R.durationN
-00000920: 730a d408 0a30 7072 6f74 6f73 2f70 6572  s....0protos/per
-00000930: 6665 7474 6f2f 6d65 7472 6963 732f 616e  fetto/metrics/an
-00000940: 6472 6f69 642f 6370 755f 6d65 7472 6963  droid/cpu_metric
-00000950: 2e70 726f 746f 120f 7065 7266 6574 746f  .proto..perfetto
-00000960: 2e70 726f 746f 7322 8e08 0a10 416e 6472  .protos"....Andr
-00000970: 6f69 6443 7075 4d65 7472 6963 124c 0a0c  oidCpuMetric.L..
-00000980: 7072 6f63 6573 735f 696e 666f 1801 2003  process_info.. .
-00000990: 280b 3229 2e70 6572 6665 7474 6f2e 7072  (.2).perfetto.pr
-000009a0: 6f74 6f73 2e41 6e64 726f 6964 4370 754d  otos.AndroidCpuM
-000009b0: 6574 7269 632e 5072 6f63 6573 7352 0b70  etric.ProcessR.p
-000009c0: 726f 6365 7373 496e 666f 1aa8 010a 074d  rocessInfo.....M
-000009d0: 6574 7269 6373 1218 0a07 6d63 7963 6c65  etrics....mcycle
-000009e0: 7318 0120 0128 0352 076d 6379 636c 6573  s.. .(.R.mcycles
-000009f0: 121d 0a0a 7275 6e74 696d 655f 6e73 1802  ....runtime_ns..
-00000a00: 2001 2803 5209 7275 6e74 696d 654e 7312   .(.R.runtimeNs.
-00000a10: 200a 0c6d 696e 5f66 7265 715f 6b68 7a18   ..min_freq_khz.
-00000a20: 0320 0128 0352 0a6d 696e 4672 6571 4b68  . .(.R.minFreqKh
-00000a30: 7a12 200a 0c6d 6178 5f66 7265 715f 6b68  z. ..max_freq_kh
-00000a40: 7a18 0420 0128 0352 0a6d 6178 4672 6571  z.. .(.R.maxFreq
-00000a50: 4b68 7a12 200a 0c61 7667 5f66 7265 715f  Khz. ..avg_freq_
-00000a60: 6b68 7a18 0520 0128 0352 0a61 7667 4672  khz.. .(.R.avgFr
-00000a70: 6571 4b68 7a1a 650a 0843 6f72 6544 6174  eqKhz.e..CoreDat
-00000a80: 6112 0e0a 0269 6418 0120 0128 0d52 0269  a....id.. .(.R.i
-00000a90: 6412 430a 076d 6574 7269 6373 1806 2001  d.C..metrics.. .
-00000aa0: 280b 3229 2e70 6572 6665 7474 6f2e 7072  (.2).perfetto.pr
-00000ab0: 6f74 6f73 2e41 6e64 726f 6964 4370 754d  otos.AndroidCpuM
-00000ac0: 6574 7269 632e 4d65 7472 6963 7352 076d  etric.MetricsR.m
-00000ad0: 6574 7269 6373 4a04 0802 1006 1a67 0a0c  etricsJ......g..
-00000ae0: 436f 7265 5479 7065 4461 7461 1212 0a04  CoreTypeData....
-00000af0: 7479 7065 1801 2001 2809 5204 7479 7065  type.. .(.R.type
-00000b00: 1243 0a07 6d65 7472 6963 7318 0220 0128  .C..metrics.. .(
-00000b10: 0b32 292e 7065 7266 6574 746f 2e70 726f  .2).perfetto.pro
-00000b20: 746f 732e 416e 6472 6f69 6443 7075 4d65  tos.AndroidCpuMe
-00000b30: 7472 6963 2e4d 6574 7269 6373 5207 6d65  tric.MetricsR.me
-00000b40: 7472 6963 731a f401 0a06 5468 7265 6164  trics.....Thread
-00000b50: 1212 0a04 6e61 6d65 1801 2001 2809 5204  ....name.. .(.R.
-00000b60: 6e61 6d65 1243 0a07 6d65 7472 6963 7318  name.C..metrics.
-00000b70: 0420 0128 0b32 292e 7065 7266 6574 746f  . .(.2).perfetto
-00000b80: 2e70 726f 746f 732e 416e 6472 6f69 6443  .protos.AndroidC
-00000b90: 7075 4d65 7472 6963 2e4d 6574 7269 6373  puMetric.Metrics
-00000ba0: 5207 6d65 7472 6963 7312 3e0a 0463 6f72  R.metrics.>..cor
-00000bb0: 6518 0220 0328 0b32 2a2e 7065 7266 6574  e.. .(.2*.perfet
-00000bc0: 746f 2e70 726f 746f 732e 416e 6472 6f69  to.protos.Androi
-00000bd0: 6443 7075 4d65 7472 6963 2e43 6f72 6544  dCpuMetric.CoreD
-00000be0: 6174 6152 0463 6f72 6512 4b0a 0963 6f72  ataR.core.K..cor
-00000bf0: 655f 7479 7065 1805 2003 280b 322e 2e70  e_type.. .(.2..p
-00000c00: 6572 6665 7474 6f2e 7072 6f74 6f73 2e41  erfetto.protos.A
-00000c10: 6e64 726f 6964 4370 754d 6574 7269 632e  ndroidCpuMetric.
-00000c20: 436f 7265 5479 7065 4461 7461 5208 636f  CoreTypeDataR.co
-00000c30: 7265 5479 7065 4a04 0803 1004 1ab9 020a  reTypeJ.........
-00000c40: 0750 726f 6365 7373 1212 0a04 6e61 6d65  .Process....name
-00000c50: 1801 2001 2809 5204 6e61 6d65 1243 0a07  .. .(.R.name.C..
-00000c60: 6d65 7472 6963 7318 0420 0128 0b32 292e  metrics.. .(.2).
-00000c70: 7065 7266 6574 746f 2e70 726f 746f 732e  perfetto.protos.
-00000c80: 416e 6472 6f69 6443 7075 4d65 7472 6963  AndroidCpuMetric
-00000c90: 2e4d 6574 7269 6373 5207 6d65 7472 6963  .MetricsR.metric
-00000ca0: 7312 420a 0774 6872 6561 6473 1806 2003  s.B..threads.. .
-00000cb0: 280b 3228 2e70 6572 6665 7474 6f2e 7072  (.2(.perfetto.pr
-00000cc0: 6f74 6f73 2e41 6e64 726f 6964 4370 754d  otos.AndroidCpuM
-00000cd0: 6574 7269 632e 5468 7265 6164 5207 7468  etric.ThreadR.th
-00000ce0: 7265 6164 7312 3e0a 0463 6f72 6518 0720  reads.>..core.. 
-00000cf0: 0328 0b32 2a2e 7065 7266 6574 746f 2e70  .(.2*.perfetto.p
-00000d00: 726f 746f 732e 416e 6472 6f69 6443 7075  rotos.AndroidCpu
-00000d10: 4d65 7472 6963 2e43 6f72 6544 6174 6152  Metric.CoreDataR
-00000d20: 0463 6f72 6512 4b0a 0963 6f72 655f 7479  .core.K..core_ty
-00000d30: 7065 1805 2003 280b 322e 2e70 6572 6665  pe.. .(.2..perfe
-00000d40: 7474 6f2e 7072 6f74 6f73 2e41 6e64 726f  tto.protos.Andro
-00000d50: 6964 4370 754d 6574 7269 632e 436f 7265  idCpuMetric.Core
-00000d60: 5479 7065 4461 7461 5208 636f 7265 5479  TypeDataR.coreTy
-00000d70: 7065 4a04 0803 1004 0af2 010a 3370 726f  peJ.........3pro
-00000d80: 746f 732f 7065 7266 6574 746f 2f6d 6574  tos/perfetto/met
-00000d90: 7269 6373 2f61 6e64 726f 6964 2f63 616d  rics/android/cam
-00000da0: 6572 615f 6d65 7472 6963 2e70 726f 746f  era_metric.proto
-00000db0: 120f 7065 7266 6574 746f 2e70 726f 746f  ..perfetto.proto
-00000dc0: 7322 a901 0a13 416e 6472 6f69 6443 616d  s"....AndroidCam
-00000dd0: 6572 614d 6574 7269 6312 510a 0e67 635f  eraMetric.Q..gc_
-00000de0: 7273 735f 616e 645f 646d 6118 0120 0128  rss_and_dma.. .(
-00000df0: 0b32 2c2e 7065 7266 6574 746f 2e70 726f  .2,.perfetto.pro
-00000e00: 746f 732e 416e 6472 6f69 6443 616d 6572  tos.AndroidCamer
-00000e10: 614d 6574 7269 632e 436f 756e 7465 7252  aMetric.CounterR
-00000e20: 0b67 6352 7373 416e 6444 6d61 1a3f 0a07  .gcRssAndDma.?..
-00000e30: 436f 756e 7465 7212 100a 036d 696e 1801  Counter....min..
-00000e40: 2001 2801 5203 6d69 6e12 100a 036d 6178   .(.R.min....max
-00000e50: 1802 2001 2801 5203 6d61 7812 100a 0361  .. .(.R.max....a
-00000e60: 7667 1803 2001 2801 5203 6176 670a fc01  vg.. .(.R.avg...
-00000e70: 0a39 7072 6f74 6f73 2f70 6572 6665 7474  .9protos/perfett
-00000e80: 6f2f 6d65 7472 6963 732f 616e 6472 6f69  o/metrics/androi
-00000e90: 642f 6361 6d65 7261 5f75 6e61 6767 5f6d  d/camera_unagg_m
-00000ea0: 6574 7269 632e 7072 6f74 6f12 0f70 6572  etric.proto..per
-00000eb0: 6665 7474 6f2e 7072 6f74 6f73 22ad 010a  fetto.protos"...
-00000ec0: 1f41 6e64 726f 6964 4361 6d65 7261 556e  .AndroidCameraUn
-00000ed0: 6167 6772 6567 6174 6564 4d65 7472 6963  aggregatedMetric
-00000ee0: 125b 0a0e 6763 5f72 7373 5f61 6e64 5f64  .[..gc_rss_and_d
-00000ef0: 6d61 1801 2003 280b 3236 2e70 6572 6665  ma.. .(.26.perfe
-00000f00: 7474 6f2e 7072 6f74 6f73 2e41 6e64 726f  tto.protos.Andro
-00000f10: 6964 4361 6d65 7261 556e 6167 6772 6567  idCameraUnaggreg
-00000f20: 6174 6564 4d65 7472 6963 2e56 616c 7565  atedMetric.Value
-00000f30: 520b 6763 5273 7341 6e64 446d 611a 2d0a  R.gcRssAndDma.-.
-00000f40: 0556 616c 7565 120e 0a02 7473 1801 2001  .Value....ts.. .
-00000f50: 2803 5202 7473 1214 0a05 7661 6c75 6518  (.R.ts....value.
-00000f60: 0220 0128 0152 0576 616c 7565 0ad8 050a  . .(.R.value....
-00000f70: 3570 726f 746f 732f 7065 7266 6574 746f  5protos/perfetto
-00000f80: 2f6d 6574 7269 6373 2f61 6e64 726f 6964  /metrics/android
-00000f90: 2f64 6973 706c 6179 5f6d 6574 7269 6373  /display_metrics
-00000fa0: 2e70 726f 746f 120f 7065 7266 6574 746f  .proto..perfetto
-00000fb0: 2e70 726f 746f 7322 8d05 0a15 416e 6472  .protos"....Andr
-00000fc0: 6f69 6444 6973 706c 6179 4d65 7472 6963  oidDisplayMetric
-00000fd0: 7312 340a 1674 6f74 616c 5f64 7570 6c69  s.4..total_dupli
-00000fe0: 6361 7465 5f66 7261 6d65 7318 0120 0128  cate_frames.. .(
-00000ff0: 0d52 1474 6f74 616c 4475 706c 6963 6174  .R.totalDuplicat
-00001000: 6546 7261 6d65 7312 360a 1764 7570 6c69  eFrames.6..dupli
-00001010: 6361 7465 5f66 7261 6d65 735f 6c6f 6767  cate_frames_logg
-00001020: 6564 1802 2001 280d 5215 6475 706c 6963  ed.. .(.R.duplic
-00001030: 6174 6546 7261 6d65 734c 6f67 6765 6412  ateFramesLogged.
-00001040: 370a 1874 6f74 616c 5f64 7075 5f75 6e64  7..total_dpu_und
-00001050: 6572 7275 6e5f 636f 756e 7418 0320 0128  errun_count.. .(
-00001060: 0d52 1574 6f74 616c 4470 7555 6e64 6572  .R.totalDpuUnder
-00001070: 7275 6e43 6f75 6e74 1232 0a15 7265 6672  runCount.2..refr
-00001080: 6573 685f 7261 7465 5f73 7769 7463 6865  esh_rate_switche
-00001090: 7318 0420 0128 0d52 1372 6566 7265 7368  s.. .(.R.refresh
-000010a0: 5261 7465 5377 6974 6368 6573 1264 0a12  RateSwitches.d..
-000010b0: 7265 6672 6573 685f 7261 7465 5f73 7461  refresh_rate_sta
-000010c0: 7473 1805 2003 280b 3236 2e70 6572 6665  ts.. .(.26.perfe
-000010d0: 7474 6f2e 7072 6f74 6f73 2e41 6e64 726f  tto.protos.Andro
-000010e0: 6964 4469 7370 6c61 794d 6574 7269 6373  idDisplayMetrics
-000010f0: 2e52 6566 7265 7368 5261 7465 5374 6174  .RefreshRateStat
-00001100: 5210 7265 6672 6573 6852 6174 6553 7461  R.refreshRateSta
-00001110: 7473 1265 0a12 7570 6461 7465 5f70 6f77  ts.e..update_pow
-00001120: 6572 5f73 7461 7465 1806 2001 280b 3237  er_state.. .(.27
-00001130: 2e70 6572 6665 7474 6f2e 7072 6f74 6f73  .perfetto.protos
-00001140: 2e41 6e64 726f 6964 4469 7370 6c61 794d  .AndroidDisplayM
-00001150: 6574 7269 6373 2e55 7064 6174 6550 6f77  etrics.UpdatePow
-00001160: 6572 5374 6174 6552 1075 7064 6174 6550  erStateR.updateP
-00001170: 6f77 6572 5374 6174 651a 9101 0a0f 5265  owerState.....Re
-00001180: 6672 6573 6852 6174 6553 7461 7412 280a  freshRateStat.(.
-00001190: 1072 6566 7265 7368 5f72 6174 655f 6670  .refresh_rate_fp
-000011a0: 7318 0120 0128 0d52 0e72 6566 7265 7368  s.. .(.R.refresh
-000011b0: 5261 7465 4670 7312 140a 0563 6f75 6e74  RateFps....count
-000011c0: 1802 2001 280d 5205 636f 756e 7412 200a  .. .(.R.count. .
-000011d0: 0c74 6f74 616c 5f64 7572 5f6d 7318 0320  .total_dur_ms.. 
-000011e0: 0128 0152 0a74 6f74 616c 4475 724d 7312  .(.R.totalDurMs.
-000011f0: 1c0a 0a61 7667 5f64 7572 5f6d 7318 0420  ...avg_dur_ms.. 
-00001200: 0128 0152 0861 7667 4475 724d 731a 380a  .(.R.avgDurMs.8.
-00001210: 1055 7064 6174 6550 6f77 6572 5374 6174  .UpdatePowerStat
-00001220: 6512 240a 0e61 7667 5f72 756e 7469 6d65  e.$..avg_runtime
-00001230: 5f6d 7318 0120 0128 0d52 0c61 7667 5275  _ms.. .(.R.avgRu
-00001240: 6e74 696d 654d 730a 8802 0a35 7072 6f74  ntimeMs....5prot
-00001250: 6f73 2f70 6572 6665 7474 6f2f 6d65 7472  os/perfetto/metr
-00001260: 6963 732f 616e 6472 6f69 642f 646d 615f  ics/android/dma_
-00001270: 6865 6170 5f6d 6574 7269 632e 7072 6f74  heap_metric.prot
-00001280: 6f12 0f70 6572 6665 7474 6f2e 7072 6f74  o..perfetto.prot
-00001290: 6f73 22bd 010a 1441 6e64 726f 6964 446d  os"....AndroidDm
-000012a0: 6148 6561 704d 6574 7269 6312 240a 0e61  aHeapMetric.$..a
-000012b0: 7667 5f73 697a 655f 6279 7465 7318 0120  vg_size_bytes.. 
-000012c0: 0128 0152 0c61 7667 5369 7a65 4279 7465  .(.R.avgSizeByte
-000012d0: 7312 240a 0e6d 696e 5f73 697a 655f 6279  s.$..min_size_by
-000012e0: 7465 7318 0220 0128 0152 0c6d 696e 5369  tes.. .(.R.minSi
-000012f0: 7a65 4279 7465 7312 240a 0e6d 6178 5f73  zeBytes.$..max_s
-00001300: 697a 655f 6279 7465 7318 0320 0128 0152  ize_bytes.. .(.R
-00001310: 0c6d 6178 5369 7a65 4279 7465 7312 330a  .maxSizeBytes.3.
-00001320: 1674 6f74 616c 5f61 6c6c 6f63 5f73 697a  .total_alloc_siz
-00001330: 655f 6279 7465 7318 0420 0128 0152 1374  e_bytes.. .(.R.t
-00001340: 6f74 616c 416c 6c6f 6353 697a 6542 7974  otalAllocSizeByt
-00001350: 6573 0aa5 030a 3170 726f 746f 732f 7065  es....1protos/pe
-00001360: 7266 6574 746f 2f6d 6574 7269 6373 2f61  rfetto/metrics/a
-00001370: 6e64 726f 6964 2f64 7666 735f 6d65 7472  ndroid/dvfs_metr
-00001380: 6963 2e70 726f 746f 120f 7065 7266 6574  ic.proto..perfet
-00001390: 746f 2e70 726f 746f 7322 de02 0a11 416e  to.protos"....An
-000013a0: 6472 6f69 6444 7666 734d 6574 7269 6312  droidDvfsMetric.
-000013b0: 600a 1066 7265 715f 7265 7369 6465 6e63  `..freq_residenc
-000013c0: 6965 7318 0120 0328 0b32 352e 7065 7266  ies.. .(.25.perf
-000013d0: 6574 746f 2e70 726f 746f 732e 416e 6472  etto.protos.Andr
-000013e0: 6f69 6444 7666 734d 6574 7269 632e 4672  oidDvfsMetric.Fr
-000013f0: 6571 7565 6e63 7952 6573 6964 656e 6379  equencyResidency
-00001400: 520f 6672 6571 5265 7369 6465 6e63 6965  R.freqResidencie
-00001410: 731a 6a0a 0842 616e 6453 7461 7412 1d0a  s.j..BandStat...
-00001420: 0a66 7265 715f 7661 6c75 6518 0120 0128  .freq_value.. .(
-00001430: 0552 0966 7265 7156 616c 7565 121e 0a0a  .R.freqValue....
-00001440: 7065 7263 656e 7461 6765 1802 2001 2801  percentage.. .(.
-00001450: 520a 7065 7263 656e 7461 6765 121f 0a0b  R.percentage....
-00001460: 6475 7261 7469 6f6e 5f6e 7318 0320 0128  duration_ns.. .(
-00001470: 0352 0a64 7572 6174 696f 6e4e 731a 7b0a  .R.durationNs.{.
-00001480: 1246 7265 7175 656e 6379 5265 7369 6465  .FrequencyReside
-00001490: 6e63 7912 1b0a 0966 7265 715f 6e61 6d65  ncy....freq_name
-000014a0: 1801 2001 2809 5208 6672 6571 4e61 6d65  .. .(.R.freqName
-000014b0: 1248 0a09 6261 6e64 5f73 7461 7418 0220  .H..band_stat.. 
-000014c0: 0328 0b32 2b2e 7065 7266 6574 746f 2e70  .(.2+.perfetto.p
-000014d0: 726f 746f 732e 416e 6472 6f69 6444 7666  rotos.AndroidDvf
-000014e0: 734d 6574 7269 632e 4261 6e64 5374 6174  sMetric.BandStat
-000014f0: 5208 6261 6e64 5374 6174 0af8 020a 3470  R.bandStat....4p
-00001500: 726f 746f 732f 7065 7266 6574 746f 2f6d  rotos/perfetto/m
-00001510: 6574 7269 6373 2f61 6e64 726f 6964 2f66  etrics/android/f
-00001520: 6173 7472 7063 5f6d 6574 7269 632e 7072  astrpc_metric.pr
-00001530: 6f74 6f12 0f70 6572 6665 7474 6f2e 7072  oto..perfetto.pr
-00001540: 6f74 6f73 22ae 020a 1441 6e64 726f 6964  otos"....Android
-00001550: 4661 7374 7270 634d 6574 7269 6312 4d0a  FastrpcMetric.M.
-00001560: 0973 7562 7379 7374 656d 1801 2003 280b  .subsystem.. .(.
-00001570: 322f 2e70 6572 6665 7474 6f2e 7072 6f74  2/.perfetto.prot
-00001580: 6f73 2e41 6e64 726f 6964 4661 7374 7270  os.AndroidFastrp
-00001590: 634d 6574 7269 632e 5375 6273 7973 7465  cMetric.Subsyste
-000015a0: 6d52 0973 7562 7379 7374 656d 1ac6 010a  mR.subsystem....
-000015b0: 0953 7562 7379 7374 656d 1212 0a04 6e61  .Subsystem....na
-000015c0: 6d65 1801 2001 2809 5204 6e61 6d65 1224  me.. .(.R.name.$
-000015d0: 0a0e 6176 675f 7369 7a65 5f62 7974 6573  ..avg_size_bytes
-000015e0: 1802 2001 2801 520c 6176 6753 697a 6542  .. .(.R.avgSizeB
-000015f0: 7974 6573 1224 0a0e 6d69 6e5f 7369 7a65  ytes.$..min_size
-00001600: 5f62 7974 6573 1803 2001 2801 520c 6d69  _bytes.. .(.R.mi
-00001610: 6e53 697a 6542 7974 6573 1224 0a0e 6d61  nSizeBytes.$..ma
-00001620: 785f 7369 7a65 5f62 7974 6573 1804 2001  x_size_bytes.. .
-00001630: 2801 520c 6d61 7853 697a 6542 7974 6573  (.R.maxSizeBytes
-00001640: 1233 0a16 746f 7461 6c5f 616c 6c6f 635f  .3..total_alloc_
-00001650: 7369 7a65 5f62 7974 6573 1805 2001 2801  size_bytes.. .(.
-00001660: 5213 746f 7461 6c41 6c6c 6f63 5369 7a65  R.totalAllocSize
-00001670: 4279 7465 730a 8b05 0a30 7072 6f74 6f73  Bytes....0protos
-00001680: 2f70 6572 6665 7474 6f2f 6d65 7472 6963  /perfetto/metric
-00001690: 732f 616e 6472 6f69 642f 6732 645f 6d65  s/android/g2d_me
-000016a0: 7472 6963 2e70 726f 746f 120f 7065 7266  tric.proto..perf
-000016b0: 6574 746f 2e70 726f 746f 7322 c504 0a0a  etto.protos"....
-000016c0: 4732 644d 6574 7269 6373 123c 0a06 6732  G2dMetrics.<..g2
-000016d0: 645f 6877 1801 2001 280b 3225 2e70 6572  d_hw.. .(.2%.per
-000016e0: 6665 7474 6f2e 7072 6f74 6f73 2e47 3264  fetto.protos.G2d
-000016f0: 4d65 7472 6963 732e 4732 644d 6574 7269  Metrics.G2dMetri
-00001700: 6352 0567 3264 4877 123c 0a06 6732 645f  cR.g2dHw.<..g2d_
-00001710: 7377 1802 2001 280b 3225 2e70 6572 6665  sw.. .(.2%.perfe
-00001720: 7474 6f2e 7072 6f74 6f73 2e47 3264 4d65  tto.protos.G2dMe
-00001730: 7472 6963 732e 4732 644d 6574 7269 6352  trics.G2dMetricR
-00001740: 0567 3264 5377 1ac3 010a 0b47 3264 496e  .g2dSw.....G2dIn
-00001750: 7374 616e 6365 1212 0a04 6e61 6d65 1801  stance....name..
-00001760: 2001 2809 5204 6e61 6d65 121f 0a0b 6672   .(.R.name....fr
-00001770: 616d 655f 636f 756e 7418 0520 0128 0d52  ame_count.. .(.R
-00001780: 0a66 7261 6d65 436f 756e 7412 1f0a 0b65  .frameCount....e
-00001790: 7272 6f72 5f63 6f75 6e74 1806 2001 280d  rror_count.. .(.
-000017a0: 520a 6572 726f 7243 6f75 6e74 121c 0a0a  R.errorCount....
-000017b0: 6d61 785f 6475 725f 6d73 1807 2001 2801  max_dur_ms.. .(.
-000017c0: 5208 6d61 7844 7572 4d73 121c 0a0a 6d69  R.maxDurMs....mi
-000017d0: 6e5f 6475 725f 6d73 1808 2001 2801 5208  n_dur_ms.. .(.R.
-000017e0: 6d69 6e44 7572 4d73 121c 0a0a 6176 675f  minDurMs....avg_
-000017f0: 6475 725f 6d73 1809 2001 2801 5208 6176  dur_ms.. .(.R.av
-00001800: 6744 7572 4d73 4a04 0802 1005 1af4 010a  gDurMsJ.........
-00001810: 0947 3264 4d65 7472 6963 1245 0a09 696e  .G2dMetric.E..in
-00001820: 7374 616e 6365 7318 0120 0328 0b32 272e  stances.. .(.2'.
-00001830: 7065 7266 6574 746f 2e70 726f 746f 732e  perfetto.protos.
-00001840: 4732 644d 6574 7269 6373 2e47 3264 496e  G2dMetrics.G2dIn
-00001850: 7374 616e 6365 5209 696e 7374 616e 6365  stanceR.instance
-00001860: 7312 1f0a 0b66 7261 6d65 5f63 6f75 6e74  s....frame_count
-00001870: 1805 2001 280d 520a 6672 616d 6543 6f75  .. .(.R.frameCou
-00001880: 6e74 121f 0a0b 6572 726f 725f 636f 756e  nt....error_coun
-00001890: 7418 0620 0128 0d52 0a65 7272 6f72 436f  t.. .(.R.errorCo
-000018a0: 756e 7412 1c0a 0a6d 6178 5f64 7572 5f6d  unt....max_dur_m
-000018b0: 7318 0720 0128 0152 086d 6178 4475 724d  s.. .(.R.maxDurM
-000018c0: 7312 1c0a 0a6d 696e 5f64 7572 5f6d 7318  s....min_dur_ms.
-000018d0: 0820 0128 0152 086d 696e 4475 724d 7312  . .(.R.minDurMs.
-000018e0: 1c0a 0a61 7667 5f64 7572 5f6d 7318 0920  ...avg_dur_ms.. 
-000018f0: 0128 0152 0861 7667 4475 724d 734a 0408  .(.R.avgDurMsJ..
-00001900: 0210 050a f005 0a30 7072 6f74 6f73 2f70  .......0protos/p
-00001910: 6572 6665 7474 6f2f 6d65 7472 6963 732f  erfetto/metrics/
-00001920: 616e 6472 6f69 642f 6770 755f 6d65 7472  android/gpu_metr
-00001930: 6963 2e70 726f 746f 120f 7065 7266 6574  ic.proto..perfet
-00001940: 746f 2e70 726f 746f 7322 aa05 0a10 416e  to.protos"....An
-00001950: 6472 6f69 6447 7075 4d65 7472 6963 1247  droidGpuMetric.G
-00001960: 0a09 7072 6f63 6573 7365 7318 0120 0328  ..processes.. .(
-00001970: 0b32 292e 7065 7266 6574 746f 2e70 726f  .2).perfetto.pro
-00001980: 746f 732e 416e 6472 6f69 6447 7075 4d65  tos.AndroidGpuMe
-00001990: 7472 6963 2e50 726f 6365 7373 5209 7072  tric.ProcessR.pr
-000019a0: 6f63 6573 7365 7312 170a 076d 656d 5f6d  ocesses....mem_m
-000019b0: 6178 1802 2001 2803 5206 6d65 6d4d 6178  ax.. .(.R.memMax
-000019c0: 1217 0a07 6d65 6d5f 6d69 6e18 0320 0128  ....mem_min.. .(
-000019d0: 0352 066d 656d 4d69 6e12 170a 076d 656d  .R.memMin....mem
-000019e0: 5f61 7667 1804 2001 2803 5206 6d65 6d41  _avg.. .(.R.memA
-000019f0: 7667 1254 0a0c 6672 6571 5f6d 6574 7269  vg.T..freq_metri
-00001a00: 6373 1805 2003 280b 3231 2e70 6572 6665  cs.. .(.21.perfe
-00001a10: 7474 6f2e 7072 6f74 6f73 2e41 6e64 726f  tto.protos.Andro
-00001a20: 6964 4770 754d 6574 7269 632e 4672 6571  idGpuMetric.Freq
-00001a30: 7565 6e63 794d 6574 7269 6352 0b66 7265  uencyMetricR.fre
-00001a40: 714d 6574 7269 6373 1a68 0a07 5072 6f63  qMetrics.h..Proc
-00001a50: 6573 7312 120a 046e 616d 6518 0120 0128  ess....name.. .(
-00001a60: 0952 046e 616d 6512 170a 076d 656d 5f6d  .R.name....mem_m
-00001a70: 6178 1802 2001 2803 5206 6d65 6d4d 6178  ax.. .(.R.memMax
-00001a80: 1217 0a07 6d65 6d5f 6d69 6e18 0320 0128  ....mem_min.. .(
-00001a90: 0352 066d 656d 4d69 6e12 170a 076d 656d  .R.memMin....mem
-00001aa0: 5f61 7667 1804 2001 2803 5206 6d65 6d41  _avg.. .(.R.memA
-00001ab0: 7667 1ac1 020a 0f46 7265 7175 656e 6379  vg.....Frequency
-00001ac0: 4d65 7472 6963 1215 0a06 6770 755f 6964  Metric....gpu_id
-00001ad0: 1801 2001 280d 5205 6770 7549 6412 190a  .. .(.R.gpuId...
-00001ae0: 0866 7265 715f 6d61 7818 0220 0128 0352  .freq_max.. .(.R
-00001af0: 0766 7265 714d 6178 1219 0a08 6672 6571  .freqMax....freq
-00001b00: 5f6d 696e 1803 2001 2803 5207 6672 6571  _min.. .(.R.freq
-00001b10: 4d69 6e12 190a 0866 7265 715f 6176 6718  Min....freq_avg.
-00001b20: 0420 0128 0152 0766 7265 7141 7667 1264  . .(.R.freqAvg.d
-00001b30: 0a0a 7573 6564 5f66 7265 7173 1805 2003  ..used_freqs.. .
-00001b40: 280b 3245 2e70 6572 6665 7474 6f2e 7072  (.2E.perfetto.pr
-00001b50: 6f74 6f73 2e41 6e64 726f 6964 4770 754d  otos.AndroidGpuM
-00001b60: 6574 7269 632e 4672 6571 7565 6e63 794d  etric.FrequencyM
-00001b70: 6574 7269 632e 4d65 7472 6963 7350 6572  etric.MetricsPer
-00001b80: 4672 6571 7565 6e63 7952 0975 7365 6446  FrequencyR.usedF
-00001b90: 7265 7173 1a60 0a13 4d65 7472 6963 7350  reqs.`..MetricsP
-00001ba0: 6572 4672 6571 7565 6e63 7912 120a 0466  erFrequency....f
-00001bb0: 7265 7118 0120 0128 0352 0466 7265 7112  req.. .(.R.freq.
-00001bc0: 150a 0664 7572 5f6d 7318 0220 0128 0152  ...dur_ms.. .(.R
-00001bd0: 0564 7572 4d73 121e 0a0a 7065 7263 656e  .durMs....percen
-00001be0: 7461 6765 1803 2001 2801 520a 7065 7263  tage.. .(.R.perc
-00001bf0: 656e 7461 6765 0ac2 090a 3070 726f 746f  entage....0proto
-00001c00: 732f 7065 7266 6574 746f 2f6d 6574 7269  s/perfetto/metri
-00001c10: 6373 2f61 6e64 726f 6964 2f68 7763 6f6d  cs/android/hwcom
-00001c20: 706f 7365 722e 7072 6f74 6f12 0f70 6572  poser.proto..per
-00001c30: 6665 7474 6f2e 7072 6f74 6f73 22fc 080a  fetto.protos"...
-00001c40: 1841 6e64 726f 6964 4877 636f 6d70 6f73  .AndroidHwcompos
-00001c50: 6572 4d65 7472 6963 7312 380a 1863 6f6d  erMetrics.8..com
-00001c60: 706f 7369 7469 6f6e 5f74 6f74 616c 5f6c  position_total_l
-00001c70: 6179 6572 7318 0120 0128 0152 1663 6f6d  ayers.. .(.R.com
-00001c80: 706f 7369 7469 6f6e 546f 7461 6c4c 6179  positionTotalLay
-00001c90: 6572 7312 340a 1663 6f6d 706f 7369 7469  ers.4..compositi
-00001ca0: 6f6e 5f64 7075 5f6c 6179 6572 7318 0220  on_dpu_layers.. 
-00001cb0: 0128 0152 1463 6f6d 706f 7369 7469 6f6e  .(.R.composition
-00001cc0: 4470 754c 6179 6572 7312 340a 1663 6f6d  DpuLayers.4..com
-00001cd0: 706f 7369 7469 6f6e 5f67 7075 5f6c 6179  position_gpu_lay
-00001ce0: 6572 7318 0320 0128 0152 1463 6f6d 706f  ers.. .(.R.compo
-00001cf0: 7369 7469 6f6e 4770 754c 6179 6572 7312  sitionGpuLayers.
-00001d00: 410a 1d63 6f6d 706f 7369 7469 6f6e 5f64  A..composition_d
-00001d10: 7075 5f63 6163 6865 645f 6c61 7965 7273  pu_cached_layers
-00001d20: 1804 2001 2801 521a 636f 6d70 6f73 6974  .. .(.R.composit
-00001d30: 696f 6e44 7075 4361 6368 6564 4c61 7965  ionDpuCachedLaye
-00001d40: 7273 123f 0a1c 636f 6d70 6f73 6974 696f  rs.?..compositio
-00001d50: 6e5f 7366 5f63 6163 6865 645f 6c61 7965  n_sf_cached_laye
-00001d60: 7273 1805 2001 2801 5219 636f 6d70 6f73  rs.. .(.R.compos
-00001d70: 6974 696f 6e53 6643 6163 6865 644c 6179  itionSfCachedLay
-00001d80: 6572 7312 380a 1873 6b69 7070 6564 5f76  ers.8..skipped_v
-00001d90: 616c 6964 6174 696f 6e5f 636f 756e 7418  alidation_count.
-00001da0: 0620 0128 0552 1673 6b69 7070 6564 5661  . .(.R.skippedVa
-00001db0: 6c69 6461 7469 6f6e 436f 756e 7412 3c0a  lidationCount.<.
-00001dc0: 1a75 6e73 6b69 7070 6564 5f76 616c 6964  .unskipped_valid
-00001dd0: 6174 696f 6e5f 636f 756e 7418 0720 0128  ation_count.. .(
-00001de0: 0552 1875 6e73 6b69 7070 6564 5661 6c69  .R.unskippedVali
-00001df0: 6461 7469 6f6e 436f 756e 7412 3c0a 1a73  dationCount.<..s
-00001e00: 6570 6172 6174 6564 5f76 616c 6964 6174  eparated_validat
-00001e10: 696f 6e5f 636f 756e 7418 0820 0128 0552  ion_count.. .(.R
-00001e20: 1873 6570 6172 6174 6564 5661 6c69 6461  .separatedValida
-00001e30: 7469 6f6e 436f 756e 7412 380a 1875 6e6b  tionCount.8..unk
-00001e40: 6e6f 776e 5f76 616c 6964 6174 696f 6e5f  nown_validation_
-00001e50: 636f 756e 7418 0920 0128 0552 1675 6e6b  count.. .(.R.unk
-00001e60: 6e6f 776e 5661 6c69 6461 7469 6f6e 436f  nownValidationCo
-00001e70: 756e 7412 380a 1961 7667 5f61 6c6c 5f65  unt.8..avg_all_e
-00001e80: 7865 6375 7469 6f6e 5f74 696d 655f 6d73  xecution_time_ms
-00001e90: 180a 2001 2801 5215 6176 6741 6c6c 4578  .. .(.R.avgAllEx
-00001ea0: 6563 7574 696f 6e54 696d 654d 7312 400a  ecutionTimeMs.@.
-00001eb0: 1d61 7667 5f73 6b69 7070 6564 5f65 7865  .avg_skipped_exe
-00001ec0: 6375 7469 6f6e 5f74 696d 655f 6d73 180b  cution_time_ms..
-00001ed0: 2001 2801 5219 6176 6753 6b69 7070 6564   .(.R.avgSkipped
-00001ee0: 4578 6563 7574 696f 6e54 696d 654d 7312  ExecutionTimeMs.
-00001ef0: 440a 1f61 7667 5f75 6e73 6b69 7070 6564  D..avg_unskipped
-00001f00: 5f65 7865 6375 7469 6f6e 5f74 696d 655f  _execution_time_
-00001f10: 6d73 180c 2001 2801 521b 6176 6755 6e73  ms.. .(.R.avgUns
-00001f20: 6b69 7070 6564 4578 6563 7574 696f 6e54  kippedExecutionT
-00001f30: 696d 654d 7312 440a 1f61 7667 5f73 6570  imeMs.D..avg_sep
-00001f40: 6172 6174 6564 5f65 7865 6375 7469 6f6e  arated_execution
-00001f50: 5f74 696d 655f 6d73 180d 2001 2801 521b  _time_ms.. .(.R.
-00001f60: 6176 6753 6570 6172 6174 6564 4578 6563  avgSeparatedExec
-00001f70: 7574 696f 6e54 696d 654d 7312 620a 1064  utionTimeMs.b..d
-00001f80: 7075 5f76 6f74 655f 6d65 7472 6963 7318  pu_vote_metrics.
-00001f90: 0e20 0328 0b32 382e 7065 7266 6574 746f  . .(.28.perfetto
-00001fa0: 2e70 726f 746f 732e 416e 6472 6f69 6448  .protos.AndroidH
-00001fb0: 7763 6f6d 706f 7365 724d 6574 7269 6373  wcomposerMetrics
-00001fc0: 2e44 7075 566f 7465 4d65 7472 6963 7352  .DpuVoteMetricsR
-00001fd0: 0e64 7075 566f 7465 4d65 7472 6963 731a  .dpuVoteMetrics.
-00001fe0: d901 0a0e 4470 7556 6f74 654d 6574 7269  ....DpuVoteMetri
-00001ff0: 6373 1210 0a03 7469 6418 0120 0128 0d52  cs....tid.. .(.R
-00002000: 0374 6964 122b 0a12 6176 675f 6470 755f  .tid.+..avg_dpu_
-00002010: 766f 7465 5f63 6c6f 636b 1802 2001 2801  vote_clock.. .(.
-00002020: 520f 6176 6744 7075 566f 7465 436c 6f63  R.avgDpuVoteCloc
-00002030: 6b12 2c0a 1361 7667 5f64 7075 5f76 6f74  k.,..avg_dpu_vot
-00002040: 655f 6176 675f 6277 1803 2001 2801 520f  e_avg_bw.. .(.R.
-00002050: 6176 6744 7075 566f 7465 4176 6742 7712  avgDpuVoteAvgBw.
-00002060: 2e0a 1461 7667 5f64 7075 5f76 6f74 655f  ...avg_dpu_vote_
-00002070: 7065 616b 5f62 7718 0420 0128 0152 1061  peak_bw.. .(.R.a
-00002080: 7667 4470 7556 6f74 6550 6561 6b42 7712  vgDpuVotePeakBw.
-00002090: 2a0a 1261 7667 5f64 7075 5f76 6f74 655f  *..avg_dpu_vote_
-000020a0: 7274 5f62 7718 0520 0128 0152 0e61 7667  rt_bw.. .(.R.avg
-000020b0: 4470 7556 6f74 6552 7442 770a 860f 0a31  DpuVoteRtBw....1
-000020c0: 7072 6f74 6f73 2f70 6572 6665 7474 6f2f  protos/perfetto/
-000020d0: 6d65 7472 6963 732f 616e 6472 6f69 642f  metrics/android/
-000020e0: 6877 7569 5f6d 6574 7269 632e 7072 6f74  hwui_metric.prot
-000020f0: 6f12 0f70 6572 6665 7474 6f2e 7072 6f74  o..perfetto.prot
-00002100: 6f73 22e3 0d0a 1150 726f 6365 7373 5265  os"....ProcessRe
-00002110: 6e64 6572 496e 666f 1221 0a0c 7072 6f63  nderInfo.!..proc
-00002120: 6573 735f 6e61 6d65 1801 2001 2809 520b  ess_name.. .(.R.
-00002130: 7072 6f63 6573 734e 616d 6512 230a 0e72  processName.#..r
-00002140: 745f 6370 755f 7469 6d65 5f6d 7318 0220  t_cpu_time_ms.. 
-00002150: 0128 0352 0b72 7443 7075 5469 6d65 4d73  .(.R.rtCpuTimeMs
-00002160: 1228 0a10 6472 6177 5f66 7261 6d65 5f63  .(..draw_frame_c
-00002170: 6f75 6e74 1803 2001 280d 520e 6472 6177  ount.. .(.R.draw
-00002180: 4672 616d 6543 6f75 6e74 1224 0a0e 6472  FrameCount.$..dr
-00002190: 6177 5f66 7261 6d65 5f6d 6178 1804 2001  aw_frame_max.. .
-000021a0: 2803 520c 6472 6177 4672 616d 654d 6178  (.R.drawFrameMax
-000021b0: 1224 0a0e 6472 6177 5f66 7261 6d65 5f6d  .$..draw_frame_m
-000021c0: 696e 1805 2001 2803 520c 6472 6177 4672  in.. .(.R.drawFr
-000021d0: 616d 654d 696e 1224 0a0e 6472 6177 5f66  ameMin.$..draw_f
-000021e0: 7261 6d65 5f61 7667 1806 2001 2801 520c  rame_avg.. .(.R.
-000021f0: 6472 6177 4672 616d 6541 7667 121f 0a0b  drawFrameAvg....
-00002200: 666c 7573 685f 636f 756e 7418 0720 0128  flush_count.. .(
-00002210: 0d52 0a66 6c75 7368 436f 756e 7412 1b0a  .R.flushCount...
-00002220: 0966 6c75 7368 5f6d 6178 1808 2001 2803  .flush_max.. .(.
-00002230: 5208 666c 7573 684d 6178 121b 0a09 666c  R.flushMax....fl
-00002240: 7573 685f 6d69 6e18 0920 0128 0352 0866  ush_min.. .(.R.f
-00002250: 6c75 7368 4d69 6e12 1b0a 0966 6c75 7368  lushMin....flush
-00002260: 5f61 7667 180a 2001 2801 5208 666c 7573  _avg.. .(.R.flus
-00002270: 6841 7667 122c 0a12 7072 6570 6172 655f  hAvg.,..prepare_
-00002280: 7472 6565 5f63 6f75 6e74 180b 2001 280d  tree_count.. .(.
-00002290: 5210 7072 6570 6172 6554 7265 6543 6f75  R.prepareTreeCou
-000022a0: 6e74 1228 0a10 7072 6570 6172 655f 7472  nt.(..prepare_tr
-000022b0: 6565 5f6d 6178 180c 2001 2803 520e 7072  ee_max.. .(.R.pr
-000022c0: 6570 6172 6554 7265 654d 6178 1228 0a10  epareTreeMax.(..
-000022d0: 7072 6570 6172 655f 7472 6565 5f6d 696e  prepare_tree_min
-000022e0: 180d 2001 2803 520e 7072 6570 6172 6554  .. .(.R.prepareT
-000022f0: 7265 654d 696e 1228 0a10 7072 6570 6172  reeMin.(..prepar
-00002300: 655f 7472 6565 5f61 7667 180e 2001 2801  e_tree_avg.. .(.
-00002310: 520e 7072 6570 6172 6554 7265 6541 7667  R.prepareTreeAvg
-00002320: 1230 0a14 6770 755f 636f 6d70 6c65 7469  .0..gpu_completi
-00002330: 6f6e 5f63 6f75 6e74 180f 2001 280d 5212  on_count.. .(.R.
-00002340: 6770 7543 6f6d 706c 6574 696f 6e43 6f75  gpuCompletionCou
-00002350: 6e74 122c 0a12 6770 755f 636f 6d70 6c65  nt.,..gpu_comple
-00002360: 7469 6f6e 5f6d 6178 1810 2001 2803 5210  tion_max.. .(.R.
-00002370: 6770 7543 6f6d 706c 6574 696f 6e4d 6178  gpuCompletionMax
-00002380: 122c 0a12 6770 755f 636f 6d70 6c65 7469  .,..gpu_completi
-00002390: 6f6e 5f6d 696e 1811 2001 2803 5210 6770  on_min.. .(.R.gp
-000023a0: 7543 6f6d 706c 6574 696f 6e4d 696e 122c  uCompletionMin.,
-000023b0: 0a12 6770 755f 636f 6d70 6c65 7469 6f6e  ..gpu_completion
-000023c0: 5f61 7667 1812 2001 2801 5210 6770 7543  _avg.. .(.R.gpuC
-000023d0: 6f6d 706c 6574 696f 6e41 7667 1226 0a0f  ompletionAvg.&..
-000023e0: 7569 5f72 6563 6f72 645f 636f 756e 7418  ui_record_count.
-000023f0: 1320 0128 0d52 0d75 6952 6563 6f72 6443  . .(.R.uiRecordC
-00002400: 6f75 6e74 1222 0a0d 7569 5f72 6563 6f72  ount."..ui_recor
-00002410: 645f 6d61 7818 1420 0128 0352 0b75 6952  d_max.. .(.R.uiR
-00002420: 6563 6f72 644d 6178 1222 0a0d 7569 5f72  ecordMax."..ui_r
-00002430: 6563 6f72 645f 6d69 6e18 1520 0128 0352  ecord_min.. .(.R
-00002440: 0b75 6952 6563 6f72 644d 696e 1222 0a0d  .uiRecordMin."..
-00002450: 7569 5f72 6563 6f72 645f 6176 6718 1620  ui_record_avg.. 
-00002460: 0128 0152 0b75 6952 6563 6f72 6441 7667  .(.R.uiRecordAvg
-00002470: 1230 0a14 7368 6164 6572 5f63 6f6d 7069  .0..shader_compi
-00002480: 6c65 5f63 6f75 6e74 1817 2001 280d 5212  le_count.. .(.R.
-00002490: 7368 6164 6572 436f 6d70 696c 6543 6f75  shaderCompileCou
-000024a0: 6e74 122e 0a13 7368 6164 6572 5f63 6f6d  nt....shader_com
-000024b0: 7069 6c65 5f74 696d 6518 1820 0128 0352  pile_time.. .(.R
-000024c0: 1173 6861 6465 7243 6f6d 7069 6c65 5469  .shaderCompileTi
-000024d0: 6d65 122c 0a12 7368 6164 6572 5f63 6f6d  me.,..shader_com
-000024e0: 7069 6c65 5f61 7667 1819 2001 2801 5210  pile_avg.. .(.R.
-000024f0: 7368 6164 6572 436f 6d70 696c 6541 7667  shaderCompileAvg
-00002500: 1226 0a0f 6361 6368 655f 6869 745f 636f  .&..cache_hit_co
-00002510: 756e 7418 1a20 0128 0d52 0d63 6163 6865  unt.. .(.R.cache
-00002520: 4869 7443 6f75 6e74 1224 0a0e 6361 6368  HitCount.$..cach
-00002530: 655f 6869 745f 7469 6d65 181b 2001 2803  e_hit_time.. .(.
-00002540: 520c 6361 6368 6548 6974 5469 6d65 1222  R.cacheHitTime."
-00002550: 0a0d 6361 6368 655f 6869 745f 6176 6718  ..cache_hit_avg.
-00002560: 1c20 0128 0152 0b63 6163 6865 4869 7441  . .(.R.cacheHitA
-00002570: 7667 1228 0a10 6361 6368 655f 6d69 7373  vg.(..cache_miss
-00002580: 5f63 6f75 6e74 181d 2001 280d 520e 6361  _count.. .(.R.ca
-00002590: 6368 654d 6973 7343 6f75 6e74 1226 0a0f  cheMissCount.&..
-000025a0: 6361 6368 655f 6d69 7373 5f74 696d 6518  cache_miss_time.
-000025b0: 1e20 0128 0352 0d63 6163 6865 4d69 7373  . .(.R.cacheMiss
-000025c0: 5469 6d65 1224 0a0e 6361 6368 655f 6d69  Time.$..cache_mi
-000025d0: 7373 5f61 7667 181f 2001 2801 520c 6361  ss_avg.. .(.R.ca
-000025e0: 6368 654d 6973 7341 7667 122f 0a14 6772  cheMissAvg./..gr
-000025f0: 6170 6869 6373 5f63 7075 5f6d 656d 5f6d  aphics_cpu_mem_m
-00002600: 6178 1820 2001 2803 5211 6772 6170 6869  ax.  .(.R.graphi
-00002610: 6373 4370 754d 656d 4d61 7812 2f0a 1467  csCpuMemMax./..g
-00002620: 7261 7068 6963 735f 6370 755f 6d65 6d5f  raphics_cpu_mem_
-00002630: 6d69 6e18 2120 0128 0352 1167 7261 7068  min.! .(.R.graph
-00002640: 6963 7343 7075 4d65 6d4d 696e 122f 0a14  icsCpuMemMin./..
-00002650: 6772 6170 6869 6373 5f63 7075 5f6d 656d  graphics_cpu_mem
-00002660: 5f61 7667 1822 2001 2801 5211 6772 6170  _avg." .(.R.grap
-00002670: 6869 6373 4370 754d 656d 4176 6712 2f0a  hicsCpuMemAvg./.
-00002680: 1467 7261 7068 6963 735f 6770 755f 6d65  .graphics_gpu_me
-00002690: 6d5f 6d61 7818 2320 0128 0352 1167 7261  m_max.# .(.R.gra
-000026a0: 7068 6963 7347 7075 4d65 6d4d 6178 122f  phicsGpuMemMax./
-000026b0: 0a14 6772 6170 6869 6373 5f67 7075 5f6d  ..graphics_gpu_m
-000026c0: 656d 5f6d 696e 1824 2001 2803 5211 6772  em_min.$ .(.R.gr
-000026d0: 6170 6869 6373 4770 754d 656d 4d69 6e12  aphicsGpuMemMin.
-000026e0: 2f0a 1467 7261 7068 6963 735f 6770 755f  /..graphics_gpu_
-000026f0: 6d65 6d5f 6176 6718 2520 0128 0152 1167  mem_avg.% .(.R.g
-00002700: 7261 7068 6963 7347 7075 4d65 6d41 7667  raphicsGpuMemAvg
-00002710: 1226 0a0f 7465 7874 7572 655f 6d65 6d5f  .&..texture_mem_
-00002720: 6d61 7818 2620 0128 0352 0d74 6578 7475  max.& .(.R.textu
-00002730: 7265 4d65 6d4d 6178 1226 0a0f 7465 7874  reMemMax.&..text
-00002740: 7572 655f 6d65 6d5f 6d69 6e18 2720 0128  ure_mem_min.' .(
-00002750: 0352 0d74 6578 7475 7265 4d65 6d4d 696e  .R.textureMemMin
-00002760: 1226 0a0f 7465 7874 7572 655f 6d65 6d5f  .&..texture_mem_
-00002770: 6176 6718 2820 0128 0152 0d74 6578 7475  avg.( .(.R.textu
-00002780: 7265 4d65 6d41 7667 121e 0a0b 616c 6c5f  reMemAvg....all_
-00002790: 6d65 6d5f 6d61 7818 2920 0128 0352 0961  mem_max.) .(.R.a
-000027a0: 6c6c 4d65 6d4d 6178 121e 0a0b 616c 6c5f  llMemMax....all_
-000027b0: 6d65 6d5f 6d69 6e18 2a20 0128 0352 0961  mem_min.* .(.R.a
-000027c0: 6c6c 4d65 6d4d 696e 121e 0a0b 616c 6c5f  llMemMin....all_
-000027d0: 6d65 6d5f 6176 6718 2b20 0128 0152 0961  mem_avg.+ .(.R.a
-000027e0: 6c6c 4d65 6d41 7667 225a 0a11 416e 6472  llMemAvg"Z..Andr
-000027f0: 6f69 6448 7775 694d 6574 7269 6312 450a  oidHwuiMetric.E.
-00002800: 0c70 726f 6365 7373 5f69 6e66 6f18 0120  .process_info.. 
-00002810: 0328 0b32 222e 7065 7266 6574 746f 2e70  .(.2".perfetto.p
-00002820: 726f 746f 732e 5072 6f63 6573 7352 656e  rotos.ProcessRen
-00002830: 6465 7249 6e66 6f52 0b70 726f 6365 7373  derInfoR.process
-00002840: 496e 666f 0ae0 020a 3070 726f 746f 732f  Info....0protos/
-00002850: 7065 7266 6574 746f 2f6d 6574 7269 6373  perfetto/metrics
-00002860: 2f61 6e64 726f 6964 2f69 6f6e 5f6d 6574  /android/ion_met
-00002870: 7269 632e 7072 6f74 6f12 0f70 6572 6665  ric.proto..perfe
-00002880: 7474 6f2e 7072 6f74 6f73 229a 020a 1041  tto.protos"....A
-00002890: 6e64 726f 6964 496f 6e4d 6574 7269 6312  ndroidIonMetric.
-000028a0: 400a 0662 7566 6665 7218 0120 0328 0b32  @..buffer.. .(.2
-000028b0: 282e 7065 7266 6574 746f 2e70 726f 746f  (.perfetto.proto
-000028c0: 732e 416e 6472 6f69 6449 6f6e 4d65 7472  s.AndroidIonMetr
-000028d0: 6963 2e42 7566 6665 7252 0662 7566 6665  ic.BufferR.buffe
-000028e0: 721a c301 0a06 4275 6666 6572 1212 0a04  r.....Buffer....
-000028f0: 6e61 6d65 1801 2001 2809 5204 6e61 6d65  name.. .(.R.name
-00002900: 1224 0a0e 6176 675f 7369 7a65 5f62 7974  .$..avg_size_byt
-00002910: 6573 1802 2001 2801 520c 6176 6753 697a  es.. .(.R.avgSiz
-00002920: 6542 7974 6573 1224 0a0e 6d69 6e5f 7369  eBytes.$..min_si
-00002930: 7a65 5f62 7974 6573 1803 2001 2801 520c  ze_bytes.. .(.R.
-00002940: 6d69 6e53 697a 6542 7974 6573 1224 0a0e  minSizeBytes.$..
-00002950: 6d61 785f 7369 7a65 5f62 7974 6573 1804  max_size_bytes..
-00002960: 2001 2801 520c 6d61 7853 697a 6542 7974   .(.R.maxSizeByt
-00002970: 6573 1233 0a16 746f 7461 6c5f 616c 6c6f  es.3..total_allo
-00002980: 635f 7369 7a65 5f62 7974 6573 1805 2001  c_size_bytes.. .
-00002990: 2801 5213 746f 7461 6c41 6c6c 6f63 5369  (.R.totalAllocSi
-000029a0: 7a65 4279 7465 730a fa05 0a38 7072 6f74  zeBytes....8prot
-000029b0: 6f73 2f70 6572 6665 7474 6f2f 6d65 7472  os/perfetto/metr
-000029c0: 6963 732f 616e 6472 6f69 642f 6972 715f  ics/android/irq_
-000029d0: 7275 6e74 696d 655f 6d65 7472 6963 2e70  runtime_metric.p
-000029e0: 726f 746f 120f 7065 7266 6574 746f 2e70  roto..perfetto.p
-000029f0: 726f 746f 7322 ac05 0a17 416e 6472 6f69  rotos"....Androi
-00002a00: 6449 7271 5275 6e74 696d 654d 6574 7269  dIrqRuntimeMetri
-00002a10: 6312 500a 0668 775f 6972 7118 0120 0128  c.P..hw_irq.. .(
-00002a20: 0b32 392e 7065 7266 6574 746f 2e70 726f  .29.perfetto.pro
-00002a30: 746f 732e 416e 6472 6f69 6449 7271 5275  tos.AndroidIrqRu
-00002a40: 6e74 696d 654d 6574 7269 632e 4972 7152  ntimeMetric.IrqR
-00002a50: 756e 7469 6d65 4d65 7472 6963 5205 6877  untimeMetricR.hw
-00002a60: 4972 7112 500a 0673 775f 6972 7118 0220  Irq.P..sw_irq.. 
-00002a70: 0128 0b32 392e 7065 7266 6574 746f 2e70  .(.29.perfetto.p
-00002a80: 726f 746f 732e 416e 6472 6f69 6449 7271  rotos.AndroidIrq
-00002a90: 5275 6e74 696d 654d 6574 7269 632e 4972  RuntimeMetric.Ir
-00002aa0: 7152 756e 7469 6d65 4d65 7472 6963 5205  qRuntimeMetricR.
-00002ab0: 7377 4972 711a 470a 0849 7271 536c 6963  swIrq.G..IrqSlic
-00002ac0: 6512 190a 0869 7271 5f6e 616d 6518 0120  e....irq_name.. 
-00002ad0: 0128 0952 0769 7271 4e61 6d65 120e 0a02  .(.R.irqName....
-00002ae0: 7473 1802 2001 2803 5202 7473 1210 0a03  ts.. .(.R.ts....
-00002af0: 6475 7218 0320 0128 0352 0364 7572 1a86  dur.. .(.R.dur..
-00002b00: 010a 0f54 6872 6573 686f 6c64 4d65 7472  ...ThresholdMetr
-00002b10: 6963 121c 0a09 7468 7265 7368 6f6c 6418  ic....threshold.
-00002b20: 0120 0128 0952 0974 6872 6573 686f 6c64  . .(.R.threshold
-00002b30: 1230 0a14 6f76 6572 5f74 6872 6573 686f  .0..over_thresho
-00002b40: 6c64 5f63 6f75 6e74 1802 2001 2803 5212  ld_count.. .(.R.
-00002b50: 6f76 6572 5468 7265 7368 6f6c 6443 6f75  overThresholdCou
-00002b60: 6e74 1223 0a0d 616e 6f6d 616c 795f 7261  nt.#..anomaly_ra
-00002b70: 7469 6f18 0320 0128 0152 0c61 6e6f 6d61  tio.. .(.R.anoma
-00002b80: 6c79 5261 7469 6f1a 9a02 0a10 4972 7152  lyRatio.....IrqR
-00002b90: 756e 7469 6d65 4d65 7472 6963 121f 0a0b  untimeMetric....
-00002ba0: 6d61 785f 7275 6e74 696d 6518 0120 0128  max_runtime.. .(
-00002bb0: 0352 0a6d 6178 5275 6e74 696d 6512 1f0a  .R.maxRuntime...
-00002bc0: 0b74 6f74 616c 5f63 6f75 6e74 1802 2001  .total_count.. .
-00002bd0: 2803 520a 746f 7461 6c43 6f75 6e74 1263  (.R.totalCount.c
-00002be0: 0a10 7468 7265 7368 6f6c 645f 6d65 7472  ..threshold_metr
-00002bf0: 6963 1803 2001 280b 3238 2e70 6572 6665  ic.. .(.28.perfe
-00002c00: 7474 6f2e 7072 6f74 6f73 2e41 6e64 726f  tto.protos.Andro
-00002c10: 6964 4972 7152 756e 7469 6d65 4d65 7472  idIrqRuntimeMetr
-00002c20: 6963 2e54 6872 6573 686f 6c64 4d65 7472  ic.ThresholdMetr
-00002c30: 6963 520f 7468 7265 7368 6f6c 644d 6574  icR.thresholdMet
-00002c40: 7269 6312 5f0a 126c 6f6e 6765 7374 5f69  ric._..longest_i
-00002c50: 7271 5f73 6c69 6365 7318 0420 0328 0b32  rq_slices.. .(.2
-00002c60: 312e 7065 7266 6574 746f 2e70 726f 746f  1.perfetto.proto
-00002c70: 732e 416e 6472 6f69 6449 7271 5275 6e74  s.AndroidIrqRunt
-00002c80: 696d 654d 6574 7269 632e 4972 7153 6c69  imeMetric.IrqSli
-00002c90: 6365 5210 6c6f 6e67 6573 7449 7271 536c  ceR.longestIrqSl
-00002ca0: 6963 6573 0aff 0a0a 3570 726f 746f 732f  ices....5protos/
-00002cb0: 7065 7266 6574 746f 2f6d 6574 7269 6373  perfetto/metrics
-00002cc0: 2f61 6e64 726f 6964 2f6a 616e 6b5f 6375  /android/jank_cu
-00002cd0: 6a5f 6d65 7472 6963 2e70 726f 746f 120f  j_metric.proto..
-00002ce0: 7065 7266 6574 746f 2e70 726f 746f 731a  perfetto.protos.
-00002cf0: 3670 726f 746f 732f 7065 7266 6574 746f  6protos/perfetto
-00002d00: 2f6d 6574 7269 6373 2f61 6e64 726f 6964  /metrics/android
-00002d10: 2f70 726f 6365 7373 5f6d 6574 6164 6174  /process_metadat
-00002d20: 612e 7072 6f74 6f22 fc09 0a14 416e 6472  a.proto"....Andr
-00002d30: 6f69 644a 616e 6b43 756a 4d65 7472 6963  oidJankCujMetric
-00002d40: 123b 0a03 6375 6a18 0120 0328 0b32 292e  .;..cuj.. .(.2).
-00002d50: 7065 7266 6574 746f 2e70 726f 746f 732e  perfetto.protos.
-00002d60: 416e 6472 6f69 644a 616e 6b43 756a 4d65  AndroidJankCujMe
-00002d70: 7472 6963 2e43 756a 5203 6375 6a1a 9f04  tric.CujR.cuj...
-00002d80: 0a03 4375 6a12 0e0a 0269 6418 0120 0128  ..Cuj....id.. .(
-00002d90: 0552 0269 6412 120a 046e 616d 6518 0220  .R.id....name.. 
-00002da0: 0128 0952 046e 616d 6512 410a 0770 726f  .(.R.name.A..pro
-00002db0: 6365 7373 1803 2001 280b 3227 2e70 6572  cess.. .(.2'.per
-00002dc0: 6665 7474 6f2e 7072 6f74 6f73 2e41 6e64  fetto.protos.And
-00002dd0: 726f 6964 5072 6f63 6573 734d 6574 6164  roidProcessMetad
-00002de0: 6174 6152 0770 726f 6365 7373 120e 0a02  ataR.process....
-00002df0: 7473 1804 2001 2803 5202 7473 1210 0a03  ts.. .(.R.ts....
-00002e00: 6475 7218 0520 0128 0352 0364 7572 1241  dur.. .(.R.dur.A
-00002e10: 0a05 6672 616d 6518 0620 0328 0b32 2b2e  ..frame.. .(.2+.
-00002e20: 7065 7266 6574 746f 2e70 726f 746f 732e  perfetto.protos.
-00002e30: 416e 6472 6f69 644a 616e 6b43 756a 4d65  AndroidJankCujMe
-00002e40: 7472 6963 2e46 7261 6d65 5205 6672 616d  tric.FrameR.fram
-00002e50: 6512 460a 0873 665f 6672 616d 6518 0a20  e.F..sf_frame.. 
-00002e60: 0328 0b32 2b2e 7065 7266 6574 746f 2e70  .(.2+.perfetto.p
-00002e70: 726f 746f 732e 416e 6472 6f69 644a 616e  rotos.AndroidJan
-00002e80: 6b43 756a 4d65 7472 6963 2e46 7261 6d65  kCujMetric.Frame
-00002e90: 5207 7366 4672 616d 6512 560a 0f63 6f75  R.sfFrame.V..cou
-00002ea0: 6e74 6572 5f6d 6574 7269 6373 1807 2001  nter_metrics.. .
-00002eb0: 280b 322d 2e70 6572 6665 7474 6f2e 7072  (.2-.perfetto.pr
-00002ec0: 6f74 6f73 2e41 6e64 726f 6964 4a61 6e6b  otos.AndroidJank
-00002ed0: 4375 6a4d 6574 7269 632e 4d65 7472 6963  CujMetric.Metric
-00002ee0: 7352 0e63 6f75 6e74 6572 4d65 7472 6963  sR.counterMetric
-00002ef0: 7312 580a 1074 696d 656c 696e 655f 6d65  s.X..timeline_me
-00002f00: 7472 6963 7318 0820 0128 0b32 2d2e 7065  trics.. .(.2-.pe
-00002f10: 7266 6574 746f 2e70 726f 746f 732e 416e  rfetto.protos.An
-00002f20: 6472 6f69 644a 616e 6b43 756a 4d65 7472  droidJankCujMetr
-00002f30: 6963 2e4d 6574 7269 6373 520f 7469 6d65  ic.MetricsR.time
-00002f40: 6c69 6e65 4d65 7472 6963 7312 520a 0d74  lineMetrics.R..t
-00002f50: 7261 6365 5f6d 6574 7269 6373 1809 2001  race_metrics.. .
-00002f60: 280b 322d 2e70 6572 6665 7474 6f2e 7072  (.2-.perfetto.pr
-00002f70: 6f74 6f73 2e41 6e64 726f 6964 4a61 6e6b  otos.AndroidJank
-00002f80: 4375 6a4d 6574 7269 632e 4d65 7472 6963  CujMetric.Metric
-00002f90: 7352 0c74 7261 6365 4d65 7472 6963 731a  sR.traceMetrics.
-00002fa0: c101 0a05 4672 616d 6512 210a 0c66 7261  ....Frame.!..fra
-00002fb0: 6d65 5f6e 756d 6265 7218 0120 0128 0352  me_number.. .(.R
-00002fc0: 0b66 7261 6d65 4e75 6d62 6572 1214 0a05  .frameNumber....
-00002fd0: 7673 796e 6318 0220 0128 0352 0576 7379  vsync.. .(.R.vsy
-00002fe0: 6e63 120e 0a02 7473 1803 2001 2803 5202  nc....ts.. .(.R.
-00002ff0: 7473 1210 0a03 6475 7218 0420 0128 0352  ts....dur.. .(.R
-00003000: 0364 7572 1221 0a0c 6475 725f 6578 7065  .dur.!..dur_expe
-00003010: 6374 6564 1807 2001 2803 520b 6475 7245  cted.. .(.R.durE
-00003020: 7870 6563 7465 6412 1d0a 0a61 7070 5f6d  xpected....app_m
-00003030: 6973 7365 6418 0520 0128 0852 0961 7070  issed.. .(.R.app
-00003040: 4d69 7373 6564 121b 0a09 7366 5f6d 6973  Missed....sf_mis
-00003050: 7365 6418 0620 0128 0852 0873 664d 6973  sed.. .(.R.sfMis
-00003060: 7365 641a c003 0a07 4d65 7472 6963 7312  sed.....Metrics.
-00003070: 210a 0c74 6f74 616c 5f66 7261 6d65 7318  !..total_frames.
-00003080: 0120 0128 0352 0b74 6f74 616c 4672 616d  . .(.R.totalFram
-00003090: 6573 1223 0a0d 6d69 7373 6564 5f66 7261  es.#..missed_fra
-000030a0: 6d65 7318 0220 0128 0352 0c6d 6973 7365  mes.. .(.R.misse
-000030b0: 6446 7261 6d65 7312 2a0a 116d 6973 7365  dFrames.*..misse
-000030c0: 645f 6170 705f 6672 616d 6573 1803 2001  d_app_frames.. .
-000030d0: 2803 520f 6d69 7373 6564 4170 7046 7261  (.R.missedAppFra
-000030e0: 6d65 7312 280a 106d 6973 7365 645f 7366  mes.(..missed_sf
-000030f0: 5f66 7261 6d65 7318 0420 0128 0352 0e6d  _frames.. .(.R.m
-00003100: 6973 7365 6453 6646 7261 6d65 7312 3f0a  issedSfFrames.?.
-00003110: 1c6d 6973 7365 645f 6672 616d 6573 5f6d  .missed_frames_m
-00003120: 6178 5f73 7563 6365 7373 6976 6518 0520  ax_successive.. 
-00003130: 0128 0352 196d 6973 7365 6446 7261 6d65  .(.R.missedFrame
-00003140: 734d 6178 5375 6363 6573 7369 7665 1222  sMaxSuccessive."
-00003150: 0a0d 6672 616d 655f 6475 725f 6d61 7818  ..frame_dur_max.
-00003160: 0620 0128 0352 0b66 7261 6d65 4475 724d  . .(.R.frameDurM
-00003170: 6178 1222 0a0d 6672 616d 655f 6475 725f  ax."..frame_dur_
-00003180: 6176 6718 0720 0128 0352 0b66 7261 6d65  avg.. .(.R.frame
-00003190: 4475 7241 7667 1222 0a0d 6672 616d 655f  DurAvg."..frame_
-000031a0: 6475 725f 7035 3018 0820 0128 0352 0b66  dur_p50.. .(.R.f
-000031b0: 7261 6d65 4475 7250 3530 1222 0a0d 6672  rameDurP50."..fr
-000031c0: 616d 655f 6475 725f 7039 3018 0920 0128  ame_dur_p90.. .(
-000031d0: 0352 0b66 7261 6d65 4475 7250 3930 1222  .R.frameDurP90."
-000031e0: 0a0d 6672 616d 655f 6475 725f 7039 3518  ..frame_dur_p95.
-000031f0: 0a20 0128 0352 0b66 7261 6d65 4475 7250  . .(.R.frameDurP
-00003200: 3935 1222 0a0d 6672 616d 655f 6475 725f  95."..frame_dur_
-00003210: 7039 3918 0b20 0128 0352 0b66 7261 6d65  p99.. .(.R.frame
-00003220: 4475 7250 3939 0ac0 060a 3970 726f 746f  DurP99....9proto
-00003230: 732f 7065 7266 6574 746f 2f6d 6574 7269  s/perfetto/metri
-00003240: 6373 2f61 6e64 726f 6964 2f6a 6176 615f  cs/android/java_
-00003250: 6865 6170 5f68 6973 746f 6772 616d 2e70  heap_histogram.p
-00003260: 726f 746f 120f 7065 7266 6574 746f 2e70  roto..perfetto.p
-00003270: 726f 746f 731a 3670 726f 746f 732f 7065  rotos.6protos/pe
-00003280: 7266 6574 746f 2f6d 6574 7269 6373 2f61  rfetto/metrics/a
-00003290: 6e64 726f 6964 2f70 726f 6365 7373 5f6d  ndroid/process_m
-000032a0: 6574 6164 6174 612e 7072 6f74 6f22 b905  etadata.proto"..
-000032b0: 0a11 4a61 7661 4865 6170 4869 7374 6f67  ..JavaHeapHistog
-000032c0: 7261 6d12 570a 0e69 6e73 7461 6e63 655f  ram.W..instance_
-000032d0: 7374 6174 7318 0120 0328 0b32 302e 7065  stats.. .(.20.pe
-000032e0: 7266 6574 746f 2e70 726f 746f 732e 4a61  rfetto.protos.Ja
-000032f0: 7661 4865 6170 4869 7374 6f67 7261 6d2e  vaHeapHistogram.
-00003300: 496e 7374 616e 6365 5374 6174 7352 0d69  InstanceStatsR.i
-00003310: 6e73 7461 6e63 6553 7461 7473 1ab5 020a  nstanceStats....
-00003320: 0954 7970 6543 6f75 6e74 121b 0a09 7479  .TypeCount....ty
-00003330: 7065 5f6e 616d 6518 0120 0128 0952 0874  pe_name.. .(.R.t
-00003340: 7970 654e 616d 6512 1a0a 0863 6174 6567  ypeName....categ
-00003350: 6f72 7918 0420 0128 0952 0863 6174 6567  ory.. .(.R.categ
-00003360: 6f72 7912 1b0a 096f 626a 5f63 6f75 6e74  ory....obj_count
-00003370: 1802 2001 280d 5208 6f62 6a43 6f75 6e74  .. .(.R.objCount
-00003380: 122e 0a13 7265 6163 6861 626c 655f 6f62  ....reachable_ob
-00003390: 6a5f 636f 756e 7418 0320 0128 0d52 1172  j_count.. .(.R.r
-000033a0: 6561 6368 6162 6c65 4f62 6a43 6f75 6e74  eachableObjCount
-000033b0: 1217 0a07 7369 7a65 5f6b 6218 0520 0128  ....size_kb.. .(
-000033c0: 0d52 0673 697a 654b 6212 2a0a 1172 6561  .R.sizeKb.*..rea
-000033d0: 6368 6162 6c65 5f73 697a 655f 6b62 1806  chable_size_kb..
-000033e0: 2001 280d 520f 7265 6163 6861 626c 6553   .(.R.reachableS
-000033f0: 697a 654b 6212 240a 0e6e 6174 6976 655f  izeKb.$..native_
-00003400: 7369 7a65 5f6b 6218 0720 0128 0d52 0c6e  size_kb.. .(.R.n
-00003410: 6174 6976 6553 697a 654b 6212 370a 1872  ativeSizeKb.7..r
-00003420: 6561 6368 6162 6c65 5f6e 6174 6976 655f  eachable_native_
-00003430: 7369 7a65 5f6b 6218 0820 0128 0d52 1572  size_kb.. .(.R.r
-00003440: 6561 6368 6162 6c65 4e61 7469 7665 5369  eachableNativeSi
-00003450: 7a65 4b62 1a65 0a06 5361 6d70 6c65 120e  zeKb.e..Sample..
-00003460: 0a02 7473 1801 2001 2803 5202 7473 124b  ..ts.. .(.R.ts.K
-00003470: 0a0a 7479 7065 5f63 6f75 6e74 1802 2003  ..type_count.. .
-00003480: 280b 322c 2e70 6572 6665 7474 6f2e 7072  (.2,.perfetto.pr
-00003490: 6f74 6f73 2e4a 6176 6148 6561 7048 6973  otos.JavaHeapHis
-000034a0: 746f 6772 616d 2e54 7970 6543 6f75 6e74  togram.TypeCount
-000034b0: 5209 7479 7065 436f 756e 741a ab01 0a0d  R.typeCount.....
-000034c0: 496e 7374 616e 6365 5374 6174 7312 120a  InstanceStats...
-000034d0: 0475 7069 6418 0120 0128 0d52 0475 7069  .upid.. .(.R.upi
-000034e0: 6412 410a 0770 726f 6365 7373 1802 2001  d.A..process.. .
-000034f0: 280b 3227 2e70 6572 6665 7474 6f2e 7072  (.2'.perfetto.pr
-00003500: 6f74 6f73 2e41 6e64 726f 6964 5072 6f63  otos.AndroidProc
-00003510: 6573 734d 6574 6164 6174 6152 0770 726f  essMetadataR.pro
-00003520: 6365 7373 1243 0a07 7361 6d70 6c65 7318  cess.C..samples.
-00003530: 0320 0328 0b32 292e 7065 7266 6574 746f  . .(.2).perfetto
-00003540: 2e70 726f 746f 732e 4a61 7661 4865 6170  .protos.JavaHeap
-00003550: 4869 7374 6f67 7261 6d2e 5361 6d70 6c65  Histogram.Sample
-00003560: 5207 7361 6d70 6c65 730a 8507 0a35 7072  R.samples....5pr
-00003570: 6f74 6f73 2f70 6572 6665 7474 6f2f 6d65  otos/perfetto/me
-00003580: 7472 6963 732f 616e 6472 6f69 642f 6a61  trics/android/ja
-00003590: 7661 5f68 6561 705f 7374 6174 732e 7072  va_heap_stats.pr
-000035a0: 6f74 6f12 0f70 6572 6665 7474 6f2e 7072  oto..perfetto.pr
-000035b0: 6f74 6f73 1a36 7072 6f74 6f73 2f70 6572  otos.6protos/per
-000035c0: 6665 7474 6f2f 6d65 7472 6963 732f 616e  fetto/metrics/an
-000035d0: 6472 6f69 642f 7072 6f63 6573 735f 6d65  droid/process_me
-000035e0: 7461 6461 7461 2e70 726f 746f 2282 060a  tadata.proto"...
-000035f0: 0d4a 6176 6148 6561 7053 7461 7473 1253  .JavaHeapStats.S
-00003600: 0a0e 696e 7374 616e 6365 5f73 7461 7473  ..instance_stats
-00003610: 1801 2003 280b 322c 2e70 6572 6665 7474  .. .(.2,.perfett
-00003620: 6f2e 7072 6f74 6f73 2e4a 6176 6148 6561  o.protos.JavaHea
-00003630: 7053 7461 7473 2e49 6e73 7461 6e63 6553  pStats.InstanceS
-00003640: 7461 7473 520d 696e 7374 616e 6365 5374  tatsR.instanceSt
-00003650: 6174 731a 620a 0948 6561 7052 6f6f 7473  ats.b..HeapRoots
-00003660: 121b 0a09 726f 6f74 5f74 7970 6518 0120  ....root_type.. 
-00003670: 0128 0952 0872 6f6f 7454 7970 6512 1b0a  .(.R.rootType...
-00003680: 0974 7970 655f 6e61 6d65 1802 2001 2809  .type_name.. .(.
-00003690: 5208 7479 7065 4e61 6d65 121b 0a09 6f62  R.typeName....ob
-000036a0: 6a5f 636f 756e 7418 0320 0128 0352 086f  j_count.. .(.R.o
-000036b0: 626a 436f 756e 741a 8d03 0a06 5361 6d70  bjCount.....Samp
-000036c0: 6c65 120e 0a02 7473 1801 2001 2803 5202  le....ts.. .(.R.
-000036d0: 7473 121b 0a09 6865 6170 5f73 697a 6518  ts....heap_size.
-000036e0: 0220 0128 0352 0868 6561 7053 697a 6512  . .(.R.heapSize.
-000036f0: 280a 1068 6561 705f 6e61 7469 7665 5f73  (..heap_native_s
-00003700: 697a 6518 0820 0128 0352 0e68 6561 704e  ize.. .(.R.heapN
-00003710: 6174 6976 6553 697a 6512 1b0a 096f 626a  ativeSize....obj
-00003720: 5f63 6f75 6e74 1804 2001 2803 5208 6f62  _count.. .(.R.ob
-00003730: 6a43 6f75 6e74 122e 0a13 7265 6163 6861  jCount....reacha
-00003740: 626c 655f 6865 6170 5f73 697a 6518 0320  ble_heap_size.. 
-00003750: 0128 0352 1172 6561 6368 6162 6c65 4865  .(.R.reachableHe
-00003760: 6170 5369 7a65 123b 0a1a 7265 6163 6861  apSize.;..reacha
-00003770: 626c 655f 6865 6170 5f6e 6174 6976 655f  ble_heap_native_
-00003780: 7369 7a65 1809 2001 2803 5217 7265 6163  size.. .(.R.reac
-00003790: 6861 626c 6548 6561 704e 6174 6976 6553  hableHeapNativeS
-000037a0: 697a 6512 2e0a 1372 6561 6368 6162 6c65  ize....reachable
-000037b0: 5f6f 626a 5f63 6f75 6e74 1805 2001 2803  _obj_count.. .(.
-000037c0: 5211 7265 6163 6861 626c 654f 626a 436f  R.reachableObjCo
-000037d0: 756e 7412 320a 1661 6e6f 6e5f 7273 735f  unt.2..anon_rss_
-000037e0: 616e 645f 7377 6170 5f73 697a 6518 0620  and_swap_size.. 
-000037f0: 0128 0352 1261 6e6f 6e52 7373 416e 6453  .(.R.anonRssAndS
-00003800: 7761 7053 697a 6512 3e0a 0572 6f6f 7473  wapSize.>..roots
-00003810: 1807 2003 280b 3228 2e70 6572 6665 7474  .. .(.2(.perfett
-00003820: 6f2e 7072 6f74 6f73 2e4a 6176 6148 6561  o.protos.JavaHea
-00003830: 7053 7461 7473 2e48 6561 7052 6f6f 7473  pStats.HeapRoots
-00003840: 5205 726f 6f74 731a a701 0a0d 496e 7374  R.roots.....Inst
-00003850: 616e 6365 5374 6174 7312 120a 0475 7069  anceStats....upi
-00003860: 6418 0120 0128 0d52 0475 7069 6412 410a  d.. .(.R.upid.A.
-00003870: 0770 726f 6365 7373 1802 2001 280b 3227  .process.. .(.2'
-00003880: 2e70 6572 6665 7474 6f2e 7072 6f74 6f73  .perfetto.protos
-00003890: 2e41 6e64 726f 6964 5072 6f63 6573 734d  .AndroidProcessM
-000038a0: 6574 6164 6174 6152 0770 726f 6365 7373  etadataR.process
-000038b0: 123f 0a07 7361 6d70 6c65 7318 0320 0328  .?..samples.. .(
-000038c0: 0b32 252e 7065 7266 6574 746f 2e70 726f  .2%.perfetto.pro
-000038d0: 746f 732e 4a61 7661 4865 6170 5374 6174  tos.JavaHeapStat
-000038e0: 732e 5361 6d70 6c65 5207 7361 6d70 6c65  s.SampleR.sample
-000038f0: 730a bb02 0a30 7072 6f74 6f73 2f70 6572  s....0protos/per
-00003900: 6665 7474 6f2f 6d65 7472 6963 732f 616e  fetto/metrics/an
-00003910: 6472 6f69 642f 6c6d 6b5f 6d65 7472 6963  droid/lmk_metric
-00003920: 2e70 726f 746f 120f 7065 7266 6574 746f  .proto..perfetto
-00003930: 2e70 726f 746f 7322 f501 0a10 416e 6472  .protos"....Andr
-00003940: 6f69 644c 6d6b 4d65 7472 6963 121f 0a0b  oidLmkMetric....
-00003950: 746f 7461 6c5f 636f 756e 7418 0120 0128  total_count.. .(
-00003960: 0552 0a74 6f74 616c 436f 756e 7412 4e0a  .R.totalCount.N.
-00003970: 0c62 795f 6f6f 6d5f 7363 6f72 6518 0220  .by_oom_score.. 
-00003980: 0328 0b32 2c2e 7065 7266 6574 746f 2e70  .(.2,.perfetto.p
-00003990: 726f 746f 732e 416e 6472 6f69 644c 6d6b  rotos.AndroidLmk
-000039a0: 4d65 7472 6963 2e42 794f 6f6d 5363 6f72  Metric.ByOomScor
-000039b0: 6552 0a62 794f 6f6d 5363 6f72 6512 280a  eR.byOomScore.(.
-000039c0: 106f 6f6d 5f76 6963 7469 6d5f 636f 756e  .oom_victim_coun
-000039d0: 7418 0320 0128 0552 0e6f 6f6d 5669 6374  t.. .(.R.oomVict
-000039e0: 696d 436f 756e 741a 460a 0a42 794f 6f6d  imCount.F..ByOom
-000039f0: 5363 6f72 6512 220a 0d6f 6f6d 5f73 636f  Score."..oom_sco
-00003a00: 7265 5f61 646a 1801 2001 2805 520b 6f6f  re_adj.. .(.R.oo
-00003a10: 6d53 636f 7265 4164 6a12 140a 0563 6f75  mScoreAdj....cou
-00003a20: 6e74 1802 2001 2805 5205 636f 756e 740a  nt.. .(.R.count.
-00003a30: cc05 0a37 7072 6f74 6f73 2f70 6572 6665  ...7protos/perfe
-00003a40: 7474 6f2f 6d65 7472 6963 732f 616e 6472  tto/metrics/andr
-00003a50: 6f69 642f 6c6d 6b5f 7265 6173 6f6e 5f6d  oid/lmk_reason_m
-00003a60: 6574 7269 632e 7072 6f74 6f12 0f70 6572  etric.proto..per
-00003a70: 6665 7474 6f2e 7072 6f74 6f73 1a36 7072  fetto.protos.6pr
-00003a80: 6f74 6f73 2f70 6572 6665 7474 6f2f 6d65  otos/perfetto/me
-00003a90: 7472 6963 732f 616e 6472 6f69 642f 7072  trics/android/pr
-00003aa0: 6f63 6573 735f 6d65 7461 6461 7461 2e70  ocess_metadata.p
-00003ab0: 726f 746f 22c7 040a 1641 6e64 726f 6964  roto"....Android
-00003ac0: 4c6d 6b52 6561 736f 6e4d 6574 7269 6312  LmkReasonMetric.
-00003ad0: 3f0a 046c 6d6b 7318 0120 0328 0b32 2b2e  ?..lmks.. .(.2+.
-00003ae0: 7065 7266 6574 746f 2e70 726f 746f 732e  perfetto.protos.
-00003af0: 416e 6472 6f69 644c 6d6b 5265 6173 6f6e  AndroidLmkReason
-00003b00: 4d65 7472 6963 2e4c 6d6b 5204 6c6d 6b73  Metric.LmkR.lmks
-00003b10: 1a97 020a 0750 726f 6365 7373 1241 0a07  .....Process.A..
-00003b20: 7072 6f63 6573 7318 0120 0128 0b32 272e  process.. .(.2'.
-00003b30: 7065 7266 6574 746f 2e70 726f 746f 732e  perfetto.protos.
-00003b40: 416e 6472 6f69 6450 726f 6365 7373 4d65  AndroidProcessMe
-00003b50: 7461 6461 7461 5207 7072 6f63 6573 7312  tadataR.process.
-00003b60: 220a 0d6f 6f6d 5f73 636f 7265 5f61 646a  "..oom_score_adj
-00003b70: 1802 2001 2805 520b 6f6f 6d53 636f 7265  .. .(.R.oomScore
-00003b80: 4164 6a12 120a 0473 697a 6518 0320 0128  Adj....size.. .(
-00003b90: 0352 0473 697a 6512 240a 0e66 696c 655f  .R.size.$..file_
-00003ba0: 7273 735f 6279 7465 7318 0420 0128 0352  rss_bytes.. .(.R
-00003bb0: 0c66 696c 6552 7373 4279 7465 7312 240a  .fileRssBytes.$.
-00003bc0: 0e61 6e6f 6e5f 7273 735f 6279 7465 7318  .anon_rss_bytes.
-00003bd0: 0520 0128 0352 0c61 6e6f 6e52 7373 4279  . .(.R.anonRssBy
-00003be0: 7465 7312 260a 0f73 686d 656d 5f72 7373  tes.&..shmem_rss
-00003bf0: 5f62 7974 6573 1806 2001 2803 520d 7368  _bytes.. .(.R.sh
-00003c00: 6d65 6d52 7373 4279 7465 7312 1d0a 0a73  memRssBytes....s
-00003c10: 7761 705f 6279 7465 7318 0720 0128 0352  wap_bytes.. .(.R
-00003c20: 0973 7761 7042 7974 6573 1ad1 010a 034c  .swapBytes.....L
-00003c30: 6d6b 1222 0a0d 6f6f 6d5f 7363 6f72 655f  mk."..oom_score_
-00003c40: 6164 6a18 0120 0128 0552 0b6f 6f6d 5363  adj.. .(.R.oomSc
-00003c50: 6f72 6541 646a 1226 0a0f 696f 6e5f 6865  oreAdj.&..ion_he
-00003c60: 6170 735f 6279 7465 7318 0420 0128 0352  aps_bytes.. .(.R
-00003c70: 0d69 6f6e 4865 6170 7342 7974 6573 122f  .ionHeapsBytes./
-00003c80: 0a14 7379 7374 656d 5f69 6f6e 5f68 6561  ..system_ion_hea
-00003c90: 705f 7369 7a65 1802 2001 2803 5211 7379  p_size.. .(.R.sy
-00003ca0: 7374 656d 496f 6e48 6561 7053 697a 6512  stemIonHeapSize.
-00003cb0: 4d0a 0970 726f 6365 7373 6573 1803 2003  M..processes.. .
-00003cc0: 280b 322f 2e70 6572 6665 7474 6f2e 7072  (.2/.perfetto.pr
-00003cd0: 6f74 6f73 2e41 6e64 726f 6964 4c6d 6b52  otos.AndroidLmkR
-00003ce0: 6561 736f 6e4d 6574 7269 632e 5072 6f63  easonMetric.Proc
-00003cf0: 6573 7352 0970 726f 6365 7373 6573 0aa5  essR.processes..
-00003d00: 080a 3070 726f 746f 732f 7065 7266 6574  ..0protos/perfet
-00003d10: 746f 2f6d 6574 7269 6373 2f61 6e64 726f  to/metrics/andro
-00003d20: 6964 2f6d 656d 5f6d 6574 7269 632e 7072  id/mem_metric.pr
-00003d30: 6f74 6f12 0f70 6572 6665 7474 6f2e 7072  oto..perfetto.pr
-00003d40: 6f74 6f73 22df 070a 1341 6e64 726f 6964  otos"....Android
-00003d50: 4d65 6d6f 7279 4d65 7472 6963 125c 0a0f  MemoryMetric.\..
-00003d60: 7072 6f63 6573 735f 6d65 7472 6963 7318  process_metrics.
-00003d70: 0120 0328 0b32 332e 7065 7266 6574 746f  . .(.23.perfetto
-00003d80: 2e70 726f 746f 732e 416e 6472 6f69 644d  .protos.AndroidM
-00003d90: 656d 6f72 794d 6574 7269 632e 5072 6f63  emoryMetric.Proc
-00003da0: 6573 734d 6574 7269 6373 520e 7072 6f63  essMetricsR.proc
-00003db0: 6573 734d 6574 7269 6373 1afd 010a 0e50  essMetrics.....P
-00003dc0: 726f 6365 7373 4d65 7472 6963 7312 210a  rocessMetrics.!.
-00003dd0: 0c70 726f 6365 7373 5f6e 616d 6518 0120  .process_name.. 
-00003de0: 0128 0952 0b70 726f 6365 7373 4e61 6d65  .(.R.processName
-00003df0: 1261 0a0e 746f 7461 6c5f 636f 756e 7465  .a..total_counte
-00003e00: 7273 1802 2001 280b 323a 2e70 6572 6665  rs.. .(.2:.perfe
-00003e10: 7474 6f2e 7072 6f74 6f73 2e41 6e64 726f  tto.protos.Andro
-00003e20: 6964 4d65 6d6f 7279 4d65 7472 6963 2e50  idMemoryMetric.P
-00003e30: 726f 6365 7373 4d65 6d6f 7279 436f 756e  rocessMemoryCoun
-00003e40: 7465 7273 520d 746f 7461 6c43 6f75 6e74  tersR.totalCount
-00003e50: 6572 7312 650a 1270 7269 6f72 6974 795f  ers.e..priority_
-00003e60: 6272 6561 6b64 6f77 6e18 0320 0328 0b32  breakdown.. .(.2
-00003e70: 362e 7065 7266 6574 746f 2e70 726f 746f  6.perfetto.proto
-00003e80: 732e 416e 6472 6f69 644d 656d 6f72 794d  s.AndroidMemoryM
-00003e90: 6574 7269 632e 5072 696f 7269 7479 4272  etric.PriorityBr
-00003ea0: 6561 6b64 6f77 6e52 1170 7269 6f72 6974  eakdownR.priorit
-00003eb0: 7942 7265 616b 646f 776e 1a87 010a 1150  yBreakdown.....P
-00003ec0: 7269 6f72 6974 7942 7265 616b 646f 776e  riorityBreakdown
-00003ed0: 121a 0a08 7072 696f 7269 7479 1801 2001  ....priority.. .
-00003ee0: 2809 5208 7072 696f 7269 7479 1256 0a08  (.R.priority.V..
-00003ef0: 636f 756e 7465 7273 1802 2001 280b 323a  counters.. .(.2:
-00003f00: 2e70 6572 6665 7474 6f2e 7072 6f74 6f73  .perfetto.protos
-00003f10: 2e41 6e64 726f 6964 4d65 6d6f 7279 4d65  .AndroidMemoryMe
-00003f20: 7472 6963 2e50 726f 6365 7373 4d65 6d6f  tric.ProcessMemo
-00003f30: 7279 436f 756e 7465 7273 5208 636f 756e  ryCountersR.coun
-00003f40: 7465 7273 1a88 030a 1550 726f 6365 7373  ters.....Process
-00003f50: 4d65 6d6f 7279 436f 756e 7465 7273 1247  MemoryCounters.G
-00003f60: 0a08 616e 6f6e 5f72 7373 1801 2001 280b  ..anon_rss.. .(.
-00003f70: 322c 2e70 6572 6665 7474 6f2e 7072 6f74  2,.perfetto.prot
-00003f80: 6f73 2e41 6e64 726f 6964 4d65 6d6f 7279  os.AndroidMemory
-00003f90: 4d65 7472 6963 2e43 6f75 6e74 6572 5207  Metric.CounterR.
-00003fa0: 616e 6f6e 5273 7312 470a 0866 696c 655f  anonRss.G..file_
-00003fb0: 7273 7318 0220 0128 0b32 2c2e 7065 7266  rss.. .(.2,.perf
-00003fc0: 6574 746f 2e70 726f 746f 732e 416e 6472  etto.protos.Andr
-00003fd0: 6f69 644d 656d 6f72 794d 6574 7269 632e  oidMemoryMetric.
-00003fe0: 436f 756e 7465 7252 0766 696c 6552 7373  CounterR.fileRss
-00003ff0: 1240 0a04 7377 6170 1803 2001 280b 322c  .@..swap.. .(.2,
-00004000: 2e70 6572 6665 7474 6f2e 7072 6f74 6f73  .perfetto.protos
-00004010: 2e41 6e64 726f 6964 4d65 6d6f 7279 4d65  .AndroidMemoryMe
-00004020: 7472 6963 2e43 6f75 6e74 6572 5204 7377  tric.CounterR.sw
-00004030: 6170 1250 0a0d 616e 6f6e 5f61 6e64 5f73  ap.P..anon_and_s
-00004040: 7761 7018 0420 0128 0b32 2c2e 7065 7266  wap.. .(.2,.perf
-00004050: 6574 746f 2e70 726f 746f 732e 416e 6472  etto.protos.Andr
-00004060: 6f69 644d 656d 6f72 794d 6574 7269 632e  oidMemoryMetric.
-00004070: 436f 756e 7465 7252 0b61 6e6f 6e41 6e64  CounterR.anonAnd
-00004080: 5377 6170 1249 0a09 6a61 7661 5f68 6561  Swap.I..java_hea
-00004090: 7018 0520 0128 0b32 2c2e 7065 7266 6574  p.. .(.2,.perfet
-000040a0: 746f 2e70 726f 746f 732e 416e 6472 6f69  to.protos.Androi
-000040b0: 644d 656d 6f72 794d 6574 7269 632e 436f  dMemoryMetric.Co
-000040c0: 756e 7465 7252 086a 6176 6148 6561 701a  unterR.javaHeap.
-000040d0: 550a 0743 6f75 6e74 6572 1210 0a03 6d69  U..Counter....mi
-000040e0: 6e18 0120 0128 0152 036d 696e 1210 0a03  n.. .(.R.min....
-000040f0: 6d61 7818 0220 0128 0152 036d 6178 1210  max.. .(.R.max..
-00004100: 0a03 6176 6718 0320 0128 0152 0361 7667  ..avg.. .(.R.avg
-00004110: 1214 0a05 6465 6c74 6118 0420 0128 0152  ....delta.. .(.R
-00004120: 0564 656c 7461 0aa0 060a 3670 726f 746f  .delta....6proto
-00004130: 732f 7065 7266 6574 746f 2f6d 6574 7269  s/perfetto/metri
-00004140: 6373 2f61 6e64 726f 6964 2f6d 656d 5f75  cs/android/mem_u
-00004150: 6e61 6767 5f6d 6574 7269 632e 7072 6f74  nagg_metric.prot
-00004160: 6f12 0f70 6572 6665 7474 6f2e 7072 6f74  o..perfetto.prot
-00004170: 6f73 22d4 050a 1f41 6e64 726f 6964 4d65  os"....AndroidMe
-00004180: 6d6f 7279 556e 6167 6772 6567 6174 6564  moryUnaggregated
-00004190: 4d65 7472 6963 1265 0a0e 7072 6f63 6573  Metric.e..proces
-000041a0: 735f 7661 6c75 6573 1801 2003 280b 323e  s_values.. .(.2>
-000041b0: 2e70 6572 6665 7474 6f2e 7072 6f74 6f73  .perfetto.protos
-000041c0: 2e41 6e64 726f 6964 4d65 6d6f 7279 556e  .AndroidMemoryUn
-000041d0: 6167 6772 6567 6174 6564 4d65 7472 6963  aggregatedMetric
-000041e0: 2e50 726f 6365 7373 5661 6c75 6573 520d  .ProcessValuesR.
-000041f0: 7072 6f63 6573 7356 616c 7565 731a 9701  processValues...
-00004200: 0a0d 5072 6f63 6573 7356 616c 7565 7312  ..ProcessValues.
-00004210: 210a 0c70 726f 6365 7373 5f6e 616d 6518  !..process_name.
-00004220: 0120 0128 0952 0b70 726f 6365 7373 4e61  . .(.R.processNa
-00004230: 6d65 1263 0a0a 6d65 6d5f 7661 6c75 6573  me.c..mem_values
-00004240: 1802 2001 280b 3244 2e70 6572 6665 7474  .. .(.2D.perfett
-00004250: 6f2e 7072 6f74 6f73 2e41 6e64 726f 6964  o.protos.Android
-00004260: 4d65 6d6f 7279 556e 6167 6772 6567 6174  MemoryUnaggregat
-00004270: 6564 4d65 7472 6963 2e50 726f 6365 7373  edMetric.Process
-00004280: 4d65 6d6f 7279 5661 6c75 6573 5209 6d65  MemoryValuesR.me
-00004290: 6d56 616c 7565 731a e302 0a13 5072 6f63  mValues.....Proc
-000042a0: 6573 734d 656d 6f72 7956 616c 7565 7312  essMemoryValues.
-000042b0: 510a 0861 6e6f 6e5f 7273 7318 0120 0328  Q..anon_rss.. .(
-000042c0: 0b32 362e 7065 7266 6574 746f 2e70 726f  .26.perfetto.pro
-000042d0: 746f 732e 416e 6472 6f69 644d 656d 6f72  tos.AndroidMemor
-000042e0: 7955 6e61 6767 7265 6761 7465 644d 6574  yUnaggregatedMet
-000042f0: 7269 632e 5661 6c75 6552 0761 6e6f 6e52  ric.ValueR.anonR
-00004300: 7373 1251 0a08 6669 6c65 5f72 7373 1802  ss.Q..file_rss..
-00004310: 2003 280b 3236 2e70 6572 6665 7474 6f2e   .(.26.perfetto.
-00004320: 7072 6f74 6f73 2e41 6e64 726f 6964 4d65  protos.AndroidMe
-00004330: 6d6f 7279 556e 6167 6772 6567 6174 6564  moryUnaggregated
-00004340: 4d65 7472 6963 2e56 616c 7565 5207 6669  Metric.ValueR.fi
-00004350: 6c65 5273 7312 4a0a 0473 7761 7018 0320  leRss.J..swap.. 
-00004360: 0328 0b32 362e 7065 7266 6574 746f 2e70  .(.26.perfetto.p
-00004370: 726f 746f 732e 416e 6472 6f69 644d 656d  rotos.AndroidMem
-00004380: 6f72 7955 6e61 6767 7265 6761 7465 644d  oryUnaggregatedM
-00004390: 6574 7269 632e 5661 6c75 6552 0473 7761  etric.ValueR.swa
-000043a0: 7012 5a0a 0d61 6e6f 6e5f 616e 645f 7377  p.Z..anon_and_sw
-000043b0: 6170 1804 2003 280b 3236 2e70 6572 6665  ap.. .(.26.perfe
-000043c0: 7474 6f2e 7072 6f74 6f73 2e41 6e64 726f  tto.protos.Andro
-000043d0: 6964 4d65 6d6f 7279 556e 6167 6772 6567  idMemoryUnaggreg
-000043e0: 6174 6564 4d65 7472 6963 2e56 616c 7565  atedMetric.Value
-000043f0: 520b 616e 6f6e 416e 6453 7761 701a 4a0a  R.anonAndSwap.J.
-00004400: 0556 616c 7565 120e 0a02 7473 1801 2001  .Value....ts.. .
-00004410: 2803 5202 7473 121b 0a09 6f6f 6d5f 7363  (.R.ts....oom_sc
-00004420: 6f72 6518 0220 0128 0552 086f 6f6d 5363  ore.. .(.R.oomSc
-00004430: 6f72 6512 140a 0576 616c 7565 1803 2001  ore....value.. .
-00004440: 2801 5205 7661 6c75 650a f103 0a36 7072  (.R.value....6pr
-00004450: 6f74 6f73 2f70 6572 6665 7474 6f2f 6d65  otos/perfetto/me
-00004460: 7472 6963 732f 616e 6472 6f69 642f 6d75  trics/android/mu
-00004470: 6c74 6975 7365 725f 6d65 7472 6963 2e70  ltiuser_metric.p
-00004480: 726f 746f 120f 7065 7266 6574 746f 2e70  roto..perfetto.p
-00004490: 726f 746f 7322 a503 0a16 416e 6472 6f69  rotos"....Androi
-000044a0: 644d 756c 7469 7573 6572 4d65 7472 6963  dMultiuserMetric
-000044b0: 1252 0a0b 7573 6572 5f73 7769 7463 6818  .R..user_switch.
-000044c0: 0120 0128 0b32 312e 7065 7266 6574 746f  . .(.21.perfetto
-000044d0: 2e70 726f 746f 732e 416e 6472 6f69 644d  .protos.AndroidM
-000044e0: 756c 7469 7573 6572 4d65 7472 6963 2e45  ultiuserMetric.E
-000044f0: 7665 6e74 4461 7461 520a 7573 6572 5377  ventDataR.userSw
-00004500: 6974 6368 1ab6 020a 0945 7665 6e74 4461  itch.....EventDa
-00004510: 7461 121f 0a0b 6475 7261 7469 6f6e 5f6d  ta....duration_m
-00004520: 7318 0120 0128 0552 0a64 7572 6174 696f  s.. .(.R.duratio
-00004530: 6e4d 7312 570a 0963 7075 5f75 7361 6765  nMs.W..cpu_usage
-00004540: 1802 2003 280b 323a 2e70 6572 6665 7474  .. .(.2:.perfett
-00004550: 6f2e 7072 6f74 6f73 2e41 6e64 726f 6964  o.protos.Android
-00004560: 4d75 6c74 6975 7365 724d 6574 7269 632e  MultiuserMetric.
-00004570: 4576 656e 7444 6174 612e 4370 7555 7361  EventData.CpuUsa
-00004580: 6765 5208 6370 7555 7361 6765 1aae 010a  geR.cpuUsage....
-00004590: 0843 7075 5573 6167 6512 170a 0775 7365  .CpuUsage....use
-000045a0: 725f 6964 1801 2001 2805 5206 7573 6572  r_id.. .(.R.user
-000045b0: 4964 1221 0a0c 7072 6f63 6573 735f 6e61  Id.!..process_na
-000045c0: 6d65 1802 2001 2809 520b 7072 6f63 6573  me.. .(.R.proces
-000045d0: 734e 616d 6512 1f0a 0b63 7075 5f6d 6379  sName....cpu_mcy
-000045e0: 636c 6573 1803 2001 2805 520a 6370 754d  cles.. .(.R.cpuM
-000045f0: 6379 636c 6573 1225 0a0e 6370 755f 7065  cycles.%..cpu_pe
-00004600: 7263 656e 7461 6765 1804 2001 2802 520d  rcentage.. .(.R.
-00004610: 6370 7550 6572 6365 6e74 6167 6512 1e0a  cpuPercentage...
-00004620: 0a69 6465 6e74 6966 6965 7218 0520 0128  .identifier.. .(
-00004630: 0952 0a69 6465 6e74 6966 6965 720a b515  .R.identifier...
-00004640: 0a34 7072 6f74 6f73 2f70 6572 6665 7474  .4protos/perfett
-00004650: 6f2f 6d65 7472 6963 732f 616e 6472 6f69  o/metrics/androi
-00004660: 642f 6e65 7477 6f72 6b5f 6d65 7472 6963  d/network_metric
-00004670: 2e70 726f 746f 120f 7065 7266 6574 746f  .proto..perfetto
-00004680: 2e70 726f 746f 7322 eb14 0a14 416e 6472  .protos"....Andr
-00004690: 6f69 644e 6574 776f 726b 4d65 7472 6963  oidNetworkMetric
-000046a0: 1250 0a0b 6e65 745f 6465 7669 6365 7318  .P..net_devices.
-000046b0: 0120 0328 0b32 2f2e 7065 7266 6574 746f  . .(.2/.perfetto
-000046c0: 2e70 726f 746f 732e 416e 6472 6f69 644e  .protos.AndroidN
-000046d0: 6574 776f 726b 4d65 7472 6963 2e4e 6574  etworkMetric.Net
-000046e0: 4465 7669 6365 520a 6e65 7444 6576 6963  DeviceR.netDevic
-000046f0: 6573 1255 0a0d 6e65 745f 7278 5f61 6374  es.U..net_rx_act
-00004700: 696f 6e18 0220 0128 0b32 312e 7065 7266  ion.. .(.21.perf
-00004710: 6574 746f 2e70 726f 746f 732e 416e 6472  etto.protos.Andr
-00004720: 6f69 644e 6574 776f 726b 4d65 7472 6963  oidNetworkMetric
-00004730: 2e4e 6574 5278 4163 7469 6f6e 520b 6e65  .NetRxActionR.ne
-00004740: 7452 7841 6374 696f 6e12 2f0a 1372 6574  tRxAction./..ret
-00004750: 7261 6e73 6d69 7373 696f 6e5f 7261 7465  ransmission_rate
-00004760: 1803 2001 2801 5212 7265 7472 616e 736d  .. .(.R.retransm
-00004770: 6973 7369 6f6e 5261 7465 1224 0a0e 6b66  issionRate.$..kf
-00004780: 7265 655f 736b 625f 7261 7465 1804 2001  ree_skb_rate.. .
-00004790: 2801 520c 6b66 7265 6553 6b62 5261 7465  (.R.kfreeSkbRate
-000047a0: 1255 0a0d 6e65 745f 7478 5f61 6374 696f  .U..net_tx_actio
-000047b0: 6e18 0520 0128 0b32 312e 7065 7266 6574  n.. .(.21.perfet
-000047c0: 746f 2e70 726f 746f 732e 416e 6472 6f69  to.protos.Androi
-000047d0: 644e 6574 776f 726b 4d65 7472 6963 2e4e  dNetworkMetric.N
-000047e0: 6574 5478 4163 7469 6f6e 520b 6e65 7454  etTxActionR.netT
-000047f0: 7841 6374 696f 6e12 4e0a 0a69 7069 5f61  xAction.N..ipi_a
-00004800: 6374 696f 6e18 0620 0128 0b32 2f2e 7065  ction.. .(.2/.pe
-00004810: 7266 6574 746f 2e70 726f 746f 732e 416e  rfetto.protos.An
-00004820: 6472 6f69 644e 6574 776f 726b 4d65 7472  droidNetworkMetr
-00004830: 6963 2e49 7069 4163 7469 6f6e 5209 6970  ic.IpiActionR.ip
-00004840: 6941 6374 696f 6e1a fc01 0a0f 5061 636b  iAction.....Pack
-00004850: 6574 5374 6174 6973 7469 6312 180a 0770  etStatistic....p
-00004860: 6163 6b65 7473 1801 2001 2803 5207 7061  ackets.. .(.R.pa
-00004870: 636b 6574 7312 140a 0562 7974 6573 1802  ckets....bytes..
-00004880: 2001 2803 5205 6279 7465 7312 390a 1966   .(.R.bytes.9..f
-00004890: 6972 7374 5f70 6163 6b65 745f 7469 6d65  irst_packet_time
-000048a0: 7374 616d 705f 6e73 1803 2001 2803 5216  stamp_ns.. .(.R.
-000048b0: 6669 7273 7450 6163 6b65 7454 696d 6573  firstPacketTimes
-000048c0: 7461 6d70 4e73 1237 0a18 6c61 7374 5f70  tampNs.7..last_p
-000048d0: 6163 6b65 745f 7469 6d65 7374 616d 705f  acket_timestamp_
-000048e0: 6e73 1804 2001 2803 5215 6c61 7374 5061  ns.. .(.R.lastPa
-000048f0: 636b 6574 5469 6d65 7374 616d 704e 7312  cketTimestampNs.
-00004900: 1f0a 0b69 6e74 6572 7661 6c5f 6e73 1805  ...interval_ns..
-00004910: 2001 2803 520a 696e 7465 7276 616c 4e73   .(.R.intervalNs
-00004920: 1224 0a0e 6461 7461 5f72 6174 655f 6b62  .$..data_rate_kb
-00004930: 7073 1806 2001 2801 520c 6461 7461 5261  ps.. .(.R.dataRa
-00004940: 7465 4b62 7073 1a87 010a 1343 6f72 6550  teKbps.....CoreP
-00004950: 6163 6b65 7453 7461 7469 7374 6963 120e  acketStatistic..
-00004960: 0a02 6964 1801 2001 280d 5202 6964 1260  ..id.. .(.R.id.`
-00004970: 0a10 7061 636b 6574 5f73 7461 7469 7374  ..packet_statist
-00004980: 6963 1802 2001 280b 3235 2e70 6572 6665  ic.. .(.25.perfe
-00004990: 7474 6f2e 7072 6f74 6f73 2e41 6e64 726f  tto.protos.Andro
-000049a0: 6964 4e65 7477 6f72 6b4d 6574 7269 632e  idNetworkMetric.
-000049b0: 5061 636b 6574 5374 6174 6973 7469 6352  PacketStatisticR
-000049c0: 0f70 6163 6b65 7453 7461 7469 7374 6963  .packetStatistic
-000049d0: 1ad4 010a 0252 7812 4b0a 0574 6f74 616c  .....Rx.K..total
-000049e0: 1801 2001 280b 3235 2e70 6572 6665 7474  .. .(.25.perfett
-000049f0: 6f2e 7072 6f74 6f73 2e41 6e64 726f 6964  o.protos.Android
-00004a00: 4e65 7477 6f72 6b4d 6574 7269 632e 5061  NetworkMetric.Pa
-00004a10: 636b 6574 5374 6174 6973 7469 6352 0574  cketStatisticR.t
-00004a20: 6f74 616c 124d 0a04 636f 7265 1802 2003  otal.M..core.. .
-00004a30: 280b 3239 2e70 6572 6665 7474 6f2e 7072  (.29.perfetto.pr
-00004a40: 6f74 6f73 2e41 6e64 726f 6964 4e65 7477  otos.AndroidNetw
-00004a50: 6f72 6b4d 6574 7269 632e 436f 7265 5061  orkMetric.CorePa
-00004a60: 636b 6574 5374 6174 6973 7469 6352 0463  cketStatisticR.c
-00004a70: 6f72 6512 320a 1567 726f 5f61 6767 7265  ore.2..gro_aggre
-00004a80: 6761 7469 6f6e 5f72 6174 696f 1803 2001  gation_ratio.. .
-00004a90: 2809 5213 6772 6f41 6767 7265 6761 7469  (.R.groAggregati
-00004aa0: 6f6e 5261 7469 6f1a a001 0a02 5478 124b  onRatio.....Tx.K
-00004ab0: 0a05 746f 7461 6c18 0120 0128 0b32 352e  ..total.. .(.25.
-00004ac0: 7065 7266 6574 746f 2e70 726f 746f 732e  perfetto.protos.
-00004ad0: 416e 6472 6f69 644e 6574 776f 726b 4d65  AndroidNetworkMe
-00004ae0: 7472 6963 2e50 6163 6b65 7453 7461 7469  tric.PacketStati
-00004af0: 7374 6963 5205 746f 7461 6c12 4d0a 0463  sticR.total.M..c
-00004b00: 6f72 6518 0220 0328 0b32 392e 7065 7266  ore.. .(.29.perf
-00004b10: 6574 746f 2e70 726f 746f 732e 416e 6472  etto.protos.Andr
-00004b20: 6f69 644e 6574 776f 726b 4d65 7472 6963  oidNetworkMetric
-00004b30: 2e43 6f72 6550 6163 6b65 7453 7461 7469  .CorePacketStati
-00004b40: 7374 6963 5204 636f 7265 1a93 010a 094e  sticR.core.....N
-00004b50: 6574 4465 7669 6365 1212 0a04 6e61 6d65  etDevice....name
-00004b60: 1801 2001 2809 5204 6e61 6d65 1238 0a02  .. .(.R.name.8..
-00004b70: 7278 1802 2001 280b 3228 2e70 6572 6665  rx.. .(.2(.perfe
-00004b80: 7474 6f2e 7072 6f74 6f73 2e41 6e64 726f  tto.protos.Andro
-00004b90: 6964 4e65 7477 6f72 6b4d 6574 7269 632e  idNetworkMetric.
-00004ba0: 5278 5202 7278 1238 0a02 7478 1803 2001  RxR.rx.8..tx.. .
-00004bb0: 280b 3228 2e70 6572 6665 7474 6f2e 7072  (.2(.perfetto.pr
-00004bc0: 6f74 6f73 2e41 6e64 726f 6964 4e65 7477  otos.AndroidNetw
-00004bd0: 6f72 6b4d 6574 7269 632e 5478 5202 7478  orkMetric.TxR.tx
-00004be0: 1aad 010a 144e 6574 5278 4163 7469 6f6e  .....NetRxAction
-00004bf0: 5374 6174 6973 7469 6312 140a 0563 6f75  Statistic....cou
-00004c00: 6e74 1801 2001 2803 5205 636f 756e 7412  nt.. .(.R.count.
-00004c10: 1d0a 0a72 756e 7469 6d65 5f6d 7318 0220  ...runtime_ms.. 
-00004c20: 0128 0152 0972 756e 7469 6d65 4d73 1224  .(.R.runtimeMs.$
-00004c30: 0a0e 6176 675f 7275 6e74 696d 655f 6d73  ..avg_runtime_ms
-00004c40: 1803 2001 2801 520c 6176 6752 756e 7469  .. .(.R.avgRunti
-00004c50: 6d65 4d73 1218 0a07 6d63 7963 6c65 7318  meMs....mcycles.
-00004c60: 0420 0128 0352 076d 6379 636c 6573 1220  . .(.R.mcycles. 
-00004c70: 0a0c 6176 675f 6672 6571 5f6b 687a 1805  ..avg_freq_khz..
-00004c80: 2001 2803 520a 6176 6746 7265 714b 687a   .(.R.avgFreqKhz
-00004c90: 1aad 010a 144e 6574 5478 4163 7469 6f6e  .....NetTxAction
-00004ca0: 5374 6174 6973 7469 6312 140a 0563 6f75  Statistic....cou
-00004cb0: 6e74 1801 2001 2803 5205 636f 756e 7412  nt.. .(.R.count.
-00004cc0: 1d0a 0a72 756e 7469 6d65 5f6d 7318 0220  ...runtime_ms.. 
-00004cd0: 0128 0152 0972 756e 7469 6d65 4d73 1224  .(.R.runtimeMs.$
-00004ce0: 0a0e 6176 675f 7275 6e74 696d 655f 6d73  ..avg_runtime_ms
-00004cf0: 1803 2001 2801 520c 6176 6752 756e 7469  .. .(.R.avgRunti
-00004d00: 6d65 4d73 1218 0a07 6d63 7963 6c65 7318  meMs....mcycles.
-00004d10: 0420 0128 0352 076d 6379 636c 6573 1220  . .(.R.mcycles. 
-00004d20: 0a0c 6176 675f 6672 6571 5f6b 687a 1805  ..avg_freq_khz..
-00004d30: 2001 2803 520a 6176 6746 7265 714b 687a   .(.R.avgFreqKhz
-00004d40: 1a6f 0a12 4970 6941 6374 696f 6e53 7461  .o..IpiActionSta
-00004d50: 7469 7374 6963 1214 0a05 636f 756e 7418  tistic....count.
-00004d60: 0120 0128 0352 0563 6f75 6e74 121d 0a0a  . .(.R.count....
-00004d70: 7275 6e74 696d 655f 6d73 1802 2001 2801  runtime_ms.. .(.
-00004d80: 5209 7275 6e74 696d 654d 7312 240a 0e61  R.runtimeMs.$..a
-00004d90: 7667 5f72 756e 7469 6d65 5f6d 7318 0320  vg_runtime_ms.. 
-00004da0: 0128 0152 0c61 7667 5275 6e74 696d 654d  .(.R.avgRuntimeM
-00004db0: 731a 9d01 0a18 436f 7265 4e65 7452 7841  s.....CoreNetRxA
-00004dc0: 6374 696f 6e53 7461 7469 7374 6963 120e  ctionStatistic..
-00004dd0: 0a02 6964 1801 2001 280d 5202 6964 1271  ..id.. .(.R.id.q
-00004de0: 0a17 6e65 745f 7278 5f61 6374 696f 6e5f  ..net_rx_action_
-00004df0: 7374 6174 6973 7469 6318 0220 0128 0b32  statistic.. .(.2
-00004e00: 3a2e 7065 7266 6574 746f 2e70 726f 746f  :.perfetto.proto
-00004e10: 732e 416e 6472 6f69 644e 6574 776f 726b  s.AndroidNetwork
-00004e20: 4d65 7472 6963 2e4e 6574 5278 4163 7469  Metric.NetRxActi
-00004e30: 6f6e 5374 6174 6973 7469 6352 146e 6574  onStatisticR.net
-00004e40: 5278 4163 7469 6f6e 5374 6174 6973 7469  RxActionStatisti
-00004e50: 631a 9d01 0a18 436f 7265 4e65 7454 7841  c.....CoreNetTxA
-00004e60: 6374 696f 6e53 7461 7469 7374 6963 120e  ctionStatistic..
-00004e70: 0a02 6964 1801 2001 280d 5202 6964 1271  ..id.. .(.R.id.q
-00004e80: 0a17 6e65 745f 7478 5f61 6374 696f 6e5f  ..net_tx_action_
-00004e90: 7374 6174 6973 7469 6318 0220 0128 0b32  statistic.. .(.2
-00004ea0: 3a2e 7065 7266 6574 746f 2e70 726f 746f  :.perfetto.proto
-00004eb0: 732e 416e 6472 6f69 644e 6574 776f 726b  s.AndroidNetwork
-00004ec0: 4d65 7472 6963 2e4e 6574 5478 4163 7469  Metric.NetTxActi
-00004ed0: 6f6e 5374 6174 6973 7469 6352 146e 6574  onStatisticR.net
-00004ee0: 5478 4163 7469 6f6e 5374 6174 6973 7469  TxActionStatisti
-00004ef0: 631a ee01 0a0b 4e65 7452 7841 6374 696f  c.....NetRxActio
-00004f00: 6e12 500a 0574 6f74 616c 1801 2001 280b  n.P..total.. .(.
-00004f10: 323a 2e70 6572 6665 7474 6f2e 7072 6f74  2:.perfetto.prot
-00004f20: 6f73 2e41 6e64 726f 6964 4e65 7477 6f72  os.AndroidNetwor
-00004f30: 6b4d 6574 7269 632e 4e65 7452 7841 6374  kMetric.NetRxAct
-00004f40: 696f 6e53 7461 7469 7374 6963 5205 746f  ionStatisticR.to
-00004f50: 7461 6c12 520a 0463 6f72 6518 0220 0328  tal.R..core.. .(
-00004f60: 0b32 3e2e 7065 7266 6574 746f 2e70 726f  .2>.perfetto.pro
-00004f70: 746f 732e 416e 6472 6f69 644e 6574 776f  tos.AndroidNetwo
-00004f80: 726b 4d65 7472 6963 2e43 6f72 654e 6574  rkMetric.CoreNet
-00004f90: 5278 4163 7469 6f6e 5374 6174 6973 7469  RxActionStatisti
-00004fa0: 6352 0463 6f72 6512 390a 1961 7667 5f69  cR.core.9..avg_i
-00004fb0: 6e74 6572 7374 6163 6b5f 6c61 7465 6e63  nterstack_latenc
-00004fc0: 795f 6d73 1803 2001 2801 5216 6176 6749  y_ms.. .(.R.avgI
-00004fd0: 6e74 6572 7374 6163 6b4c 6174 656e 6379  nterstackLatency
-00004fe0: 4d73 1ab3 010a 0b4e 6574 5478 4163 7469  Ms.....NetTxActi
-00004ff0: 6f6e 1250 0a05 746f 7461 6c18 0120 0128  on.P..total.. .(
-00005000: 0b32 3a2e 7065 7266 6574 746f 2e70 726f  .2:.perfetto.pro
-00005010: 746f 732e 416e 6472 6f69 644e 6574 776f  tos.AndroidNetwo
-00005020: 726b 4d65 7472 6963 2e4e 6574 5478 4163  rkMetric.NetTxAc
-00005030: 7469 6f6e 5374 6174 6973 7469 6352 0574  tionStatisticR.t
-00005040: 6f74 616c 1252 0a04 636f 7265 1802 2003  otal.R..core.. .
-00005050: 280b 323e 2e70 6572 6665 7474 6f2e 7072  (.2>.perfetto.pr
-00005060: 6f74 6f73 2e41 6e64 726f 6964 4e65 7477  otos.AndroidNetw
-00005070: 6f72 6b4d 6574 7269 632e 436f 7265 4e65  orkMetric.CoreNe
-00005080: 7454 7841 6374 696f 6e53 7461 7469 7374  tTxActionStatist
-00005090: 6963 5204 636f 7265 1a5b 0a09 4970 6941  icR.core.[..IpiA
-000050a0: 6374 696f 6e12 4e0a 0574 6f74 616c 1801  ction.N..total..
-000050b0: 2001 280b 3238 2e70 6572 6665 7474 6f2e   .(.28.perfetto.
-000050c0: 7072 6f74 6f73 2e41 6e64 726f 6964 4e65  protos.AndroidNe
-000050d0: 7477 6f72 6b4d 6574 7269 632e 4970 6941  tworkMetric.IpiA
-000050e0: 6374 696f 6e53 7461 7469 7374 6963 5205  ctionStatisticR.
-000050f0: 746f 7461 6c0a 9501 0a32 7072 6f74 6f73  total....2protos
-00005100: 2f70 6572 6665 7474 6f2f 6d65 7472 6963  /perfetto/metric
-00005110: 732f 616e 6472 6f69 642f 6f74 6865 725f  s/android/other_
-00005120: 7472 6163 6573 2e70 726f 746f 120f 7065  traces.proto..pe
-00005130: 7266 6574 746f 2e70 726f 746f 7322 4e0a  rfetto.protos"N.
-00005140: 1841 6e64 726f 6964 4f74 6865 7254 7261  .AndroidOtherTra
-00005150: 6365 734d 6574 7269 6312 320a 1566 696e  cesMetric.2..fin
-00005160: 616c 697a 6564 5f74 7261 6365 735f 7575  alized_traces_uu
-00005170: 6964 1801 2003 2809 5213 6669 6e61 6c69  id.. .(.R.finali
-00005180: 7a65 6454 7261 6365 7355 7569 640a 8802  zedTracesUuid...
-00005190: 0a32 7072 6f74 6f73 2f70 6572 6665 7474  .2protos/perfett
-000051a0: 6f2f 6d65 7472 6963 732f 616e 6472 6f69  o/metrics/androi
-000051b0: 642f 7061 636b 6167 655f 6c69 7374 2e70  d/package_list.p
-000051c0: 726f 746f 120f 7065 7266 6574 746f 2e70  roto..perfetto.p
-000051d0: 726f 746f 7322 c001 0a12 416e 6472 6f69  rotos"....Androi
-000051e0: 6450 6163 6b61 6765 4c69 7374 1247 0a08  dPackageList.G..
-000051f0: 7061 636b 6167 6573 1801 2003 280b 322b  packages.. .(.2+
-00005200: 2e70 6572 6665 7474 6f2e 7072 6f74 6f73  .perfetto.protos
-00005210: 2e41 6e64 726f 6964 5061 636b 6167 654c  .AndroidPackageL
-00005220: 6973 742e 5061 636b 6167 6552 0870 6163  ist.PackageR.pac
-00005230: 6b61 6765 731a 610a 0750 6163 6b61 6765  kages.a..Package
-00005240: 1221 0a0c 7061 636b 6167 655f 6e61 6d65  .!..package_name
-00005250: 1801 2001 2809 520b 7061 636b 6167 654e  .. .(.R.packageN
-00005260: 616d 6512 100a 0375 6964 1802 2001 2803  ame....uid.. .(.
-00005270: 5203 7569 6412 210a 0c76 6572 7369 6f6e  R.uid.!..version
-00005280: 5f63 6f64 6518 0320 0128 0352 0b76 6572  _code.. .(.R.ver
-00005290: 7369 6f6e 436f 6465 0ad2 030a 3570 726f  sionCode....5pro
-000052a0: 746f 732f 7065 7266 6574 746f 2f6d 6574  tos/perfetto/met
-000052b0: 7269 6373 2f61 6e64 726f 6964 2f70 6f77  rics/android/pow
-000052c0: 7261 696c 735f 6d65 7472 6963 2e70 726f  rails_metric.pro
-000052d0: 746f 120f 7065 7266 6574 746f 2e70 726f  to..perfetto.pro
-000052e0: 746f 7322 8703 0a11 416e 6472 6f69 6450  tos"....AndroidP
-000052f0: 6f77 6572 5261 696c 7312 4e0a 0b70 6f77  owerRails.N..pow
-00005300: 6572 5f72 6169 6c73 1801 2003 280b 322d  er_rails.. .(.2-
-00005310: 2e70 6572 6665 7474 6f2e 7072 6f74 6f73  .perfetto.protos
-00005320: 2e41 6e64 726f 6964 506f 7765 7252 6169  .AndroidPowerRai
-00005330: 6c73 2e50 6f77 6572 5261 696c 7352 0a70  ls.PowerRailsR.p
-00005340: 6f77 6572 5261 696c 7312 340a 1761 7667  owerRails.4..avg
-00005350: 5f74 6f74 616c 5f75 7365 645f 706f 7765  _total_used_powe
-00005360: 725f 6d77 1802 2001 2801 5213 6176 6754  r_mw.. .(.R.avgT
-00005370: 6f74 616c 5573 6564 506f 7765 724d 771a  otalUsedPowerMw.
-00005380: 4e0a 0a45 6e65 7267 7944 6174 6112 210a  N..EnergyData.!.
-00005390: 0c74 696d 6573 7461 6d70 5f6d 7318 0120  .timestamp_ms.. 
-000053a0: 0128 0352 0b74 696d 6573 7461 6d70 4d73  .(.R.timestampMs
-000053b0: 121d 0a0a 656e 6572 6779 5f75 7773 1802  ....energy_uws..
-000053c0: 2001 2801 5209 656e 6572 6779 5577 731a   .(.R.energyUws.
-000053d0: 9b01 0a0a 506f 7765 7252 6169 6c73 1212  ....PowerRails..
-000053e0: 0a04 6e61 6d65 1801 2001 2809 5204 6e61  ..name.. .(.R.na
-000053f0: 6d65 124e 0a0b 656e 6572 6779 5f64 6174  me.N..energy_dat
-00005400: 6118 0220 0328 0b32 2d2e 7065 7266 6574  a.. .(.2-.perfet
-00005410: 746f 2e70 726f 746f 732e 416e 6472 6f69  to.protos.Androi
-00005420: 6450 6f77 6572 5261 696c 732e 456e 6572  dPowerRails.Ener
-00005430: 6779 4461 7461 520a 656e 6572 6779 4461  gyDataR.energyDa
-00005440: 7461 1229 0a11 6176 675f 7573 6564 5f70  ta.)..avg_used_p
-00005450: 6f77 6572 5f6d 7718 0320 0128 0152 0e61  ower_mw.. .(.R.a
-00005460: 7667 5573 6564 506f 7765 724d 770a e503  vgUsedPowerMw...
-00005470: 0a34 7072 6f74 6f73 2f70 6572 6665 7474  .4protos/perfett
-00005480: 6f2f 6d65 7472 6963 732f 616e 6472 6f69  o/metrics/androi
-00005490: 642f 7072 6f66 696c 6572 5f73 6d61 7073  d/profiler_smaps
-000054a0: 2e70 726f 746f 120f 7065 7266 6574 746f  .proto..perfetto
-000054b0: 2e70 726f 746f 731a 3670 726f 746f 732f  .protos.6protos/
-000054c0: 7065 7266 6574 746f 2f6d 6574 7269 6373  perfetto/metrics
-000054d0: 2f61 6e64 726f 6964 2f70 726f 6365 7373  /android/process
-000054e0: 5f6d 6574 6164 6174 612e 7072 6f74 6f22  _metadata.proto"
-000054f0: e302 0a0d 5072 6f66 696c 6572 536d 6170  ....ProfilerSmap
-00005500: 7312 430a 0869 6e73 7461 6e63 6518 0120  s.C..instance.. 
-00005510: 0328 0b32 272e 7065 7266 6574 746f 2e70  .(.2'.perfetto.p
-00005520: 726f 746f 732e 5072 6f66 696c 6572 536d  rotos.ProfilerSm
-00005530: 6170 732e 496e 7374 616e 6365 5208 696e  aps.InstanceR.in
-00005540: 7374 616e 6365 1a79 0a07 4d61 7070 696e  stance.y..Mappin
-00005550: 6712 120a 0470 6174 6818 0120 0128 0952  g....path.. .(.R
-00005560: 0470 6174 6812 170a 0773 697a 655f 6b62  .path....size_kb
-00005570: 1802 2001 2805 5206 7369 7a65 4b62 1228  .. .(.R.sizeKb.(
-00005580: 0a10 7072 6976 6174 655f 6469 7274 795f  ..private_dirty_
-00005590: 6b62 1803 2001 2805 520e 7072 6976 6174  kb.. .(.R.privat
-000055a0: 6544 6972 7479 4b62 1217 0a07 7377 6170  eDirtyKb....swap
-000055b0: 5f6b 6218 0420 0128 0552 0673 7761 704b  _kb.. .(.R.swapK
-000055c0: 621a 9101 0a08 496e 7374 616e 6365 1241  b.....Instance.A
-000055d0: 0a07 7072 6f63 6573 7318 0120 0128 0b32  ..process.. .(.2
-000055e0: 272e 7065 7266 6574 746f 2e70 726f 746f  '.perfetto.proto
-000055f0: 732e 416e 6472 6f69 6450 726f 6365 7373  s.AndroidProcess
-00005600: 4d65 7461 6461 7461 5207 7072 6f63 6573  MetadataR.proces
-00005610: 7312 420a 086d 6170 7069 6e67 7318 0220  s.B..mappings.. 
-00005620: 0328 0b32 262e 7065 7266 6574 746f 2e70  .(.2&.perfetto.p
-00005630: 726f 746f 732e 5072 6f66 696c 6572 536d  rotos.ProfilerSm
-00005640: 6170 732e 4d61 7070 696e 6752 086d 6170  aps.MappingR.map
-00005650: 7069 6e67 730a cc02 0a37 7072 6f74 6f73  pings....7protos
-00005660: 2f70 6572 6665 7474 6f2f 6d65 7472 6963  /perfetto/metric
-00005670: 732f 616e 6472 6f69 642f 7274 5f72 756e  s/android/rt_run
-00005680: 7469 6d65 5f6d 6574 7269 632e 7072 6f74  time_metric.prot
-00005690: 6f12 0f70 6572 6665 7474 6f2e 7072 6f74  o..perfetto.prot
-000056a0: 6f73 22ff 010a 1641 6e64 726f 6964 5274  os"....AndroidRt
-000056b0: 5275 6e74 696d 654d 6574 7269 6312 1f0a  RuntimeMetric...
-000056c0: 0b6d 6178 5f72 756e 7469 6d65 1801 2001  .max_runtime.. .
-000056d0: 2803 520a 6d61 7852 756e 7469 6d65 1224  (.R.maxRuntime.$
-000056e0: 0a0e 6f76 6572 5f35 6d73 5f63 6f75 6e74  ..over_5ms_count
-000056f0: 1802 2001 2803 520c 6f76 6572 356d 7343  .. .(.R.over5msC
-00005700: 6f75 6e74 125b 0a11 6c6f 6e67 6573 745f  ount.[..longest_
-00005710: 7274 5f73 6c69 6365 7318 0320 0328 0b32  rt_slices.. .(.2
-00005720: 2f2e 7065 7266 6574 746f 2e70 726f 746f  /.perfetto.proto
-00005730: 732e 416e 6472 6f69 6452 7452 756e 7469  s.AndroidRtRunti
-00005740: 6d65 4d65 7472 6963 2e52 7453 6c69 6365  meMetric.RtSlice
-00005750: 520f 6c6f 6e67 6573 7452 7453 6c69 6365  R.longestRtSlice
-00005760: 731a 410a 0752 7453 6c69 6365 1214 0a05  s.A..RtSlice....
-00005770: 746e 616d 6518 0120 0128 0952 0574 6e61  tname.. .(.R.tna
-00005780: 6d65 120e 0a02 7473 1802 2001 2803 5202  me....ts.. .(.R.
-00005790: 7473 1210 0a03 6475 7218 0320 0128 0352  ts....dur.. .(.R
-000057a0: 0364 7572 0aed 040a 3070 726f 746f 732f  .dur....0protos/
-000057b0: 7065 7266 6574 746f 2f6d 6574 7269 6373  perfetto/metrics
-000057c0: 2f61 6e64 726f 6964 2f73 696d 706c 6570  /android/simplep
-000057d0: 6572 662e 7072 6f74 6f12 0f70 6572 6665  erf.proto..perfe
-000057e0: 7474 6f2e 7072 6f74 6f73 22a7 040a 1741  tto.protos"....A
-000057f0: 6e64 726f 6964 5369 6d70 6c65 7065 7266  ndroidSimpleperf
-00005800: 4d65 7472 6963 1221 0a0c 7572 6765 6e74  Metric.!..urgent
-00005810: 5f72 6174 696f 1801 2001 2801 520b 7572  _ratio.. .(.R.ur
-00005820: 6765 6e74 5261 7469 6f12 500a 0665 7665  gentRatio.P..eve
-00005830: 6e74 7318 0220 0328 0b32 382e 7065 7266  nts.. .(.28.perf
-00005840: 6574 746f 2e70 726f 746f 732e 416e 6472  etto.protos.Andr
-00005850: 6f69 6453 696d 706c 6570 6572 664d 6574  oidSimpleperfMet
-00005860: 7269 632e 5065 7266 4576 656e 744d 6574  ric.PerfEventMet
-00005870: 7269 6352 0665 7665 6e74 731a 9603 0a0f  ricR.events.....
-00005880: 5065 7266 4576 656e 744d 6574 7269 6312  PerfEventMetric.
-00005890: 120a 046e 616d 6518 0120 0128 0952 046e  ...name.. .(.R.n
-000058a0: 616d 6512 5e0a 0970 726f 6365 7373 6573  ame.^..processes
-000058b0: 1802 2003 280b 3240 2e70 6572 6665 7474  .. .(.2@.perfett
-000058c0: 6f2e 7072 6f74 6f73 2e41 6e64 726f 6964  o.protos.Android
-000058d0: 5369 6d70 6c65 7065 7266 4d65 7472 6963  SimpleperfMetric
-000058e0: 2e50 6572 6645 7665 6e74 4d65 7472 6963  .PerfEventMetric
-000058f0: 2e50 726f 6365 7373 5209 7072 6f63 6573  .ProcessR.proces
-00005900: 7365 7312 140a 0574 6f74 616c 1803 2001  ses....total.. .
-00005910: 2801 5205 746f 7461 6c1a 560a 0654 6872  (.R.total.V..Thr
-00005920: 6561 6412 100a 0374 6964 1801 2001 2805  ead....tid.. .(.
-00005930: 5203 7469 6412 120a 046e 616d 6518 0220  R.tid....name.. 
-00005940: 0128 0952 046e 616d 6512 100a 0363 7075  .(.R.name....cpu
-00005950: 1803 2001 2805 5203 6370 7512 140a 0574  .. .(.R.cpu....t
-00005960: 6f74 616c 1804 2001 2801 5205 746f 7461  otal.. .(.R.tota
-00005970: 6c1a a001 0a07 5072 6f63 6573 7312 100a  l.....Process...
-00005980: 0370 6964 1801 2001 2805 5203 7069 6412  .pid.. .(.R.pid.
-00005990: 120a 046e 616d 6518 0220 0128 0952 046e  ...name.. .(.R.n
-000059a0: 616d 6512 590a 0774 6872 6561 6473 1803  ame.Y..threads..
-000059b0: 2003 280b 323f 2e70 6572 6665 7474 6f2e   .(.2?.perfetto.
-000059c0: 7072 6f74 6f73 2e41 6e64 726f 6964 5369  protos.AndroidSi
-000059d0: 6d70 6c65 7065 7266 4d65 7472 6963 2e50  mpleperfMetric.P
-000059e0: 6572 6645 7665 6e74 4d65 7472 6963 2e54  erfEventMetric.T
-000059f0: 6872 6561 6452 0774 6872 6561 6473 1214  hreadR.threads..
-00005a00: 0a05 746f 7461 6c18 0420 0128 0152 0574  ..total.. .(.R.t
-00005a10: 6f74 616c 0a97 2b0a 3470 726f 746f 732f  otal..+.4protos/
-00005a20: 7065 7266 6574 746f 2f6d 6574 7269 6373  perfetto/metrics
-00005a30: 2f61 6e64 726f 6964 2f73 7461 7274 7570  /android/startup
-00005a40: 5f6d 6574 7269 632e 7072 6f74 6f12 0f70  _metric.proto..p
-00005a50: 6572 6665 7474 6f2e 7072 6f74 6f73 1a36  erfetto.protos.6
-00005a60: 7072 6f74 6f73 2f70 6572 6665 7474 6f2f  protos/perfetto/
-00005a70: 6d65 7472 6963 732f 616e 6472 6f69 642f  metrics/android/
-00005a80: 7072 6f63 6573 735f 6d65 7461 6461 7461  process_metadata
-00005a90: 2e70 726f 746f 2295 2a0a 1441 6e64 726f  .proto".*..Andro
-00005aa0: 6964 5374 6172 7475 704d 6574 7269 6312  idStartupMetric.
-00005ab0: 470a 0773 7461 7274 7570 1801 2003 280b  G..startup.. .(.
-00005ac0: 322d 2e70 6572 6665 7474 6f2e 7072 6f74  2-.perfetto.prot
-00005ad0: 6f73 2e41 6e64 726f 6964 5374 6172 7475  os.AndroidStartu
-00005ae0: 704d 6574 7269 632e 5374 6172 7475 7052  pMetric.StartupR
-00005af0: 0773 7461 7274 7570 1af3 020a 1254 6173  .startup.....Tas
-00005b00: 6b53 7461 7465 4272 6561 6b64 6f77 6e12  kStateBreakdown.
-00005b10: 240a 0e72 756e 6e69 6e67 5f64 7572 5f6e  $..running_dur_n
-00005b20: 7318 0120 0128 0352 0c72 756e 6e69 6e67  s.. .(.R.running
-00005b30: 4475 724e 7312 260a 0f72 756e 6e61 626c  DurNs.&..runnabl
-00005b40: 655f 6475 725f 6e73 1802 2001 2803 520d  e_dur_ns.. .(.R.
-00005b50: 7275 6e6e 6162 6c65 4475 724e 7312 3f0a  runnableDurNs.?.
-00005b60: 1c75 6e69 6e74 6572 7275 7074 6962 6c65  .uninterruptible
-00005b70: 5f73 6c65 6570 5f64 7572 5f6e 7318 0320  _sleep_dur_ns.. 
-00005b80: 0128 0352 1975 6e69 6e74 6572 7275 7074  .(.R.uninterrupt
-00005b90: 6962 6c65 536c 6565 7044 7572 4e73 123b  ibleSleepDurNs.;
-00005ba0: 0a1a 696e 7465 7272 7570 7469 626c 655f  ..interruptible_
-00005bb0: 736c 6565 705f 6475 725f 6e73 1804 2001  sleep_dur_ns.. .
-00005bc0: 2803 5217 696e 7465 7272 7570 7469 626c  (.R.interruptibl
-00005bd0: 6553 6c65 6570 4475 724e 7312 440a 1f75  eSleepDurNs.D..u
-00005be0: 6e69 6e74 6572 7275 7074 6962 6c65 5f69  ninterruptible_i
-00005bf0: 6f5f 736c 6565 705f 6475 725f 6e73 1805  o_sleep_dur_ns..
-00005c00: 2001 2803 521b 756e 696e 7465 7272 7570   .(.R.uninterrup
-00005c10: 7469 626c 6549 6f53 6c65 6570 4475 724e  tibleIoSleepDurN
-00005c20: 7312 4b0a 2375 6e69 6e74 6572 7275 7074  s.K.#uninterrupt
-00005c30: 6962 6c65 5f6e 6f6e 5f69 6f5f 736c 6565  ible_non_io_slee
-00005c40: 705f 6475 725f 6e73 1806 2001 2803 521e  p_dur_ns.. .(.R.
-00005c50: 756e 696e 7465 7272 7570 7469 626c 654e  uninterruptibleN
-00005c60: 6f6e 496f 536c 6565 7044 7572 4e73 1a6f  onIoSleepDurNs.o
-00005c70: 0a11 4d63 7963 6c65 7342 7943 6f72 6554  ..McyclesByCoreT
-00005c80: 7970 6512 160a 066c 6974 746c 6518 0120  ype....little.. 
-00005c90: 0128 0352 066c 6974 746c 6512 100a 0362  .(.R.little....b
-00005ca0: 6967 1802 2001 2803 5203 6269 6712 160a  ig.. .(.R.big...
-00005cb0: 0662 6967 6765 7218 0320 0128 0352 0662  .bigger.. .(.R.b
-00005cc0: 6967 6765 7212 180a 0775 6e6b 6e6f 776e  igger....unknown
-00005cd0: 1804 2001 2803 5207 756e 6b6e 6f77 6e1a  .. .(.R.unknown.
-00005ce0: 350a 0553 6c69 6365 1215 0a06 6475 725f  5..Slice....dur_
-00005cf0: 6e73 1801 2001 2803 5205 6475 724e 7312  ns.. .(.R.durNs.
-00005d00: 150a 0664 7572 5f6d 7318 0220 0128 0152  ...dur_ms.. .(.R
-00005d10: 0564 7572 4d73 1acf 130a 0c54 6f46 6972  .durMs.....ToFir
-00005d20: 7374 4672 616d 6512 150a 0664 7572 5f6e  stFrame....dur_n
-00005d30: 7318 0120 0128 0352 0564 7572 4e73 1215  s.. .(.R.durNs..
-00005d40: 0a06 6475 725f 6d73 1811 2001 2801 5205  ..dur_ms.. .(.R.
-00005d50: 6475 724d 7312 720a 196d 6169 6e5f 7468  durMs.r..main_th
-00005d60: 7265 6164 5f62 795f 7461 736b 5f73 7461  read_by_task_sta
-00005d70: 7465 1802 2001 280b 3238 2e70 6572 6665  te.. .(.28.perfe
-00005d80: 7474 6f2e 7072 6f74 6f73 2e41 6e64 726f  tto.protos.Andro
-00005d90: 6964 5374 6172 7475 704d 6574 7269 632e  idStartupMetric.
-00005da0: 5461 736b 5374 6174 6542 7265 616b 646f  TaskStateBreakdo
-00005db0: 776e 5215 6d61 696e 5468 7265 6164 4279  wnR.mainThreadBy
-00005dc0: 5461 736b 5374 6174 6512 680a 146d 6379  TaskState.h..mcy
-00005dd0: 636c 6573 5f62 795f 636f 7265 5f74 7970  cles_by_core_typ
-00005de0: 6518 1a20 0128 0b32 372e 7065 7266 6574  e.. .(.27.perfet
-00005df0: 746f 2e70 726f 746f 732e 416e 6472 6f69  to.protos.Androi
-00005e00: 6453 7461 7274 7570 4d65 7472 6963 2e4d  dStartupMetric.M
-00005e10: 6379 636c 6573 4279 436f 7265 5479 7065  cyclesByCoreType
-00005e20: 5211 6d63 7963 6c65 7342 7943 6f72 6554  R.mcyclesByCoreT
-00005e30: 7970 6512 410a 1d6f 7468 6572 5f70 726f  ype.A..other_pro
-00005e40: 6365 7373 6573 5f73 7061 776e 6564 5f63  cesses_spawned_c
-00005e50: 6f75 6e74 1803 2001 280d 521a 6f74 6865  ount.. .(.R.othe
-00005e60: 7250 726f 6365 7373 6573 5370 6177 6e65  rProcessesSpawne
-00005e70: 6443 6f75 6e74 125f 0a15 7469 6d65 5f61  dCount._..time_a
-00005e80: 6374 6976 6974 795f 6d61 6e61 6765 7218  ctivity_manager.
-00005e90: 0420 0128 0b32 2b2e 7065 7266 6574 746f  . .(.2+.perfetto
-00005ea0: 2e70 726f 746f 732e 416e 6472 6f69 6453  .protos.AndroidS
-00005eb0: 7461 7274 7570 4d65 7472 6963 2e53 6c69  tartupMetric.Sli
-00005ec0: 6365 5213 7469 6d65 4163 7469 7669 7479  ceR.timeActivity
-00005ed0: 4d61 6e61 6765 7212 660a 1974 696d 655f  Manager.f..time_
-00005ee0: 6163 7469 7669 7479 5f74 6872 6561 645f  activity_thread_
-00005ef0: 6d61 696e 1805 2001 280b 322b 2e70 6572  main.. .(.2+.per
-00005f00: 6665 7474 6f2e 7072 6f74 6f73 2e41 6e64  fetto.protos.And
-00005f10: 726f 6964 5374 6172 7475 704d 6574 7269  roidStartupMetri
-00005f20: 632e 536c 6963 6552 1674 696d 6541 6374  c.SliceR.timeAct
-00005f30: 6976 6974 7954 6872 6561 644d 6169 6e12  ivityThreadMain.
-00005f40: 5f0a 1574 696d 655f 6269 6e64 5f61 7070  _..time_bind_app
-00005f50: 6c69 6361 7469 6f6e 1806 2001 280b 322b  lication.. .(.2+
-00005f60: 2e70 6572 6665 7474 6f2e 7072 6f74 6f73  .perfetto.protos
-00005f70: 2e41 6e64 726f 6964 5374 6172 7475 704d  .AndroidStartupM
-00005f80: 6574 7269 632e 536c 6963 6552 1374 696d  etric.SliceR.tim
-00005f90: 6542 696e 6441 7070 6c69 6361 7469 6f6e  eBindApplication
-00005fa0: 125b 0a13 7469 6d65 5f61 6374 6976 6974  .[..time_activit
-00005fb0: 795f 7374 6172 7418 0720 0128 0b32 2b2e  y_start.. .(.2+.
-00005fc0: 7065 7266 6574 746f 2e70 726f 746f 732e  perfetto.protos.
-00005fd0: 416e 6472 6f69 6453 7461 7274 7570 4d65  AndroidStartupMe
-00005fe0: 7472 6963 2e53 6c69 6365 5211 7469 6d65  tric.SliceR.time
-00005ff0: 4163 7469 7669 7479 5374 6172 7412 5d0a  ActivityStart.].
-00006000: 1474 696d 655f 6163 7469 7669 7479 5f72  .time_activity_r
-00006010: 6573 756d 6518 0820 0128 0b32 2b2e 7065  esume.. .(.2+.pe
-00006020: 7266 6574 746f 2e70 726f 746f 732e 416e  rfetto.protos.An
-00006030: 6472 6f69 6453 7461 7274 7570 4d65 7472  droidStartupMetr
-00006040: 6963 2e53 6c69 6365 5212 7469 6d65 4163  ic.SliceR.timeAc
-00006050: 7469 7669 7479 5265 7375 6d65 125f 0a15  tivityResume._..
-00006060: 7469 6d65 5f61 6374 6976 6974 795f 7265  time_activity_re
-00006070: 7374 6172 7418 1520 0128 0b32 2b2e 7065  start.. .(.2+.pe
-00006080: 7266 6574 746f 2e70 726f 746f 732e 416e  rfetto.protos.An
-00006090: 6472 6f69 6453 7461 7274 7570 4d65 7472  droidStartupMetr
-000060a0: 6963 2e53 6c69 6365 5213 7469 6d65 4163  ic.SliceR.timeAc
-000060b0: 7469 7669 7479 5265 7374 6172 7412 5a0a  tivityRestart.Z.
-000060c0: 1274 696d 655f 6368 6f72 656f 6772 6170  .time_choreograp
-000060d0: 6865 7218 0920 0128 0b32 2b2e 7065 7266  her.. .(.2+.perf
-000060e0: 6574 746f 2e70 726f 746f 732e 416e 6472  etto.protos.Andr
-000060f0: 6f69 6453 7461 7274 7570 4d65 7472 6963  oidStartupMetric
-00006100: 2e53 6c69 6365 5211 7469 6d65 4368 6f72  .SliceR.timeChor
-00006110: 656f 6772 6170 6865 7212 4e0a 0c74 696d  eographer.N..tim
-00006120: 655f 696e 666c 6174 6518 1620 0128 0b32  e_inflate.. .(.2
-00006130: 2b2e 7065 7266 6574 746f 2e70 726f 746f  +.perfetto.proto
-00006140: 732e 416e 6472 6f69 6453 7461 7274 7570  s.AndroidStartup
-00006150: 4d65 7472 6963 2e53 6c69 6365 520b 7469  Metric.SliceR.ti
-00006160: 6d65 496e 666c 6174 6512 590a 1274 696d  meInflate.Y..tim
-00006170: 655f 6765 745f 7265 736f 7572 6365 7318  e_get_resources.
-00006180: 1720 0128 0b32 2b2e 7065 7266 6574 746f  . .(.2+.perfetto
-00006190: 2e70 726f 746f 732e 416e 6472 6f69 6453  .protos.AndroidS
-000061a0: 7461 7274 7570 4d65 7472 6963 2e53 6c69  tartupMetric.Sli
-000061b0: 6365 5210 7469 6d65 4765 7452 6573 6f75  ceR.timeGetResou
-000061c0: 7263 6573 1266 0a19 7469 6d65 5f62 6566  rces.f..time_bef
-000061d0: 6f72 655f 7374 6172 745f 7072 6f63 6573  ore_start_proces
-000061e0: 7318 0a20 0128 0b32 2b2e 7065 7266 6574  s.. .(.2+.perfet
-000061f0: 746f 2e70 726f 746f 732e 416e 6472 6f69  to.protos.Androi
-00006200: 6453 7461 7274 7570 4d65 7472 6963 2e53  dStartupMetric.S
-00006210: 6c69 6365 5216 7469 6d65 4265 666f 7265  liceR.timeBefore
-00006220: 5374 6172 7450 726f 6365 7373 1266 0a19  StartProcess.f..
-00006230: 7469 6d65 5f64 7572 696e 675f 7374 6172  time_during_star
-00006240: 745f 7072 6f63 6573 7318 0b20 0128 0b32  t_process.. .(.2
-00006250: 2b2e 7065 7266 6574 746f 2e70 726f 746f  +.perfetto.proto
-00006260: 732e 416e 6472 6f69 6453 7461 7274 7570  s.AndroidStartup
-00006270: 4d65 7472 6963 2e53 6c69 6365 5216 7469  Metric.SliceR.ti
-00006280: 6d65 4475 7269 6e67 5374 6172 7450 726f  meDuringStartPro
-00006290: 6365 7373 124d 0a0c 746f 5f70 6f73 745f  cess.M..to_post_
-000062a0: 666f 726b 1812 2001 280b 322b 2e70 6572  fork.. .(.2+.per
-000062b0: 6665 7474 6f2e 7072 6f74 6f73 2e41 6e64  fetto.protos.And
-000062c0: 726f 6964 5374 6172 7475 704d 6574 7269  roidStartupMetri
-000062d0: 632e 536c 6963 6552 0a74 6f50 6f73 7446  c.SliceR.toPostF
-000062e0: 6f72 6b12 620a 1774 6f5f 6163 7469 7669  ork.b..to_activi
-000062f0: 7479 5f74 6872 6561 645f 6d61 696e 1813  ty_thread_main..
-00006300: 2001 280b 322b 2e70 6572 6665 7474 6f2e   .(.2+.perfetto.
-00006310: 7072 6f74 6f73 2e41 6e64 726f 6964 5374  protos.AndroidSt
-00006320: 6172 7475 704d 6574 7269 632e 536c 6963  artupMetric.Slic
-00006330: 6552 1474 6f41 6374 6976 6974 7954 6872  eR.toActivityThr
-00006340: 6561 644d 6169 6e12 5b0a 1374 6f5f 6269  eadMain.[..to_bi
-00006350: 6e64 5f61 7070 6c69 6361 7469 6f6e 1814  nd_application..
-00006360: 2001 280b 322b 2e70 6572 6665 7474 6f2e   .(.2+.perfetto.
-00006370: 7072 6f74 6f73 2e41 6e64 726f 6964 5374  protos.AndroidSt
-00006380: 6172 7475 704d 6574 7269 632e 536c 6963  artupMetric.Slic
-00006390: 6552 1174 6f42 696e 6441 7070 6c69 6361  eR.toBindApplica
-000063a0: 7469 6f6e 1251 0a0e 7469 6d65 5f70 6f73  tion.Q..time_pos
-000063b0: 745f 666f 726b 1810 2001 280b 322b 2e70  t_fork.. .(.2+.p
-000063c0: 6572 6665 7474 6f2e 7072 6f74 6f73 2e41  erfetto.protos.A
-000063d0: 6e64 726f 6964 5374 6172 7475 704d 6574  ndroidStartupMet
-000063e0: 7269 632e 536c 6963 6552 0c74 696d 6550  ric.SliceR.timeP
-000063f0: 6f73 7446 6f72 6b12 4f0a 0d74 696d 655f  ostFork.O..time_
-00006400: 6465 785f 6f70 656e 1818 2001 280b 322b  dex_open.. .(.2+
-00006410: 2e70 6572 6665 7474 6f2e 7072 6f74 6f73  .perfetto.protos
-00006420: 2e41 6e64 726f 6964 5374 6172 7475 704d  .AndroidStartupM
-00006430: 6574 7269 632e 536c 6963 6552 0b74 696d  etric.SliceR.tim
-00006440: 6544 6578 4f70 656e 1257 0a11 7469 6d65  eDexOpen.W..time
-00006450: 5f76 6572 6966 795f 636c 6173 7318 1920  _verify_class.. 
-00006460: 0128 0b32 2b2e 7065 7266 6574 746f 2e70  .(.2+.perfetto.p
-00006470: 726f 746f 732e 416e 6472 6f69 6453 7461  rotos.AndroidSta
-00006480: 7274 7570 4d65 7472 6963 2e53 6c69 6365  rtupMetric.Slice
-00006490: 520f 7469 6d65 5665 7269 6679 436c 6173  R.timeVerifyClas
-000064a0: 7312 300a 146a 6974 5f63 6f6d 7069 6c65  s.0..jit_compile
-000064b0: 645f 6d65 7468 6f64 7318 1b20 0128 0d52  d_methods.. .(.R
-000064c0: 126a 6974 436f 6d70 696c 6564 4d65 7468  .jitCompiledMeth
-000064d0: 6f64 7312 680a 1b74 696d 655f 6a69 745f  ods.h..time_jit_
-000064e0: 7468 7265 6164 5f70 6f6f 6c5f 6f6e 5f63  thread_pool_on_c
-000064f0: 7075 181c 2001 280b 322b 2e70 6572 6665  pu.. .(.2+.perfe
-00006500: 7474 6f2e 7072 6f74 6f73 2e41 6e64 726f  tto.protos.Andro
-00006510: 6964 5374 6172 7475 704d 6574 7269 632e  idStartupMetric.
-00006520: 536c 6963 6552 1674 696d 654a 6974 5468  SliceR.timeJitTh
-00006530: 7265 6164 506f 6f6c 4f6e 4370 7512 4f0a  readPoolOnCpu.O.
-00006540: 0d74 696d 655f 6763 5f74 6f74 616c 181d  .time_gc_total..
-00006550: 2001 280b 322b 2e70 6572 6665 7474 6f2e   .(.2+.perfetto.
-00006560: 7072 6f74 6f73 2e41 6e64 726f 6964 5374  protos.AndroidSt
-00006570: 6172 7475 704d 6574 7269 632e 536c 6963  artupMetric.Slic
-00006580: 6552 0b74 696d 6547 6354 6f74 616c 1250  eR.timeGcTotal.P
-00006590: 0a0e 7469 6d65 5f67 635f 6f6e 5f63 7075  ..time_gc_on_cpu
-000065a0: 181e 2001 280b 322b 2e70 6572 6665 7474  .. .(.2+.perfett
-000065b0: 6f2e 7072 6f74 6f73 2e41 6e64 726f 6964  o.protos.Android
-000065c0: 5374 6172 7475 704d 6574 7269 632e 536c  StartupMetric.Sl
-000065d0: 6963 6552 0b74 696d 6547 634f 6e43 7075  iceR.timeGcOnCpu
-000065e0: 1273 0a20 7469 6d65 5f6c 6f63 6b5f 636f  .s. time_lock_co
-000065f0: 6e74 656e 7469 6f6e 5f74 6872 6561 645f  ntention_thread_
-00006600: 6d61 696e 181f 2001 280b 322b 2e70 6572  main.. .(.2+.per
-00006610: 6665 7474 6f2e 7072 6f74 6f73 2e41 6e64  fetto.protos.And
-00006620: 726f 6964 5374 6172 7475 704d 6574 7269  roidStartupMetri
-00006630: 632e 536c 6963 6552 1c74 696d 654c 6f63  c.SliceR.timeLoc
-00006640: 6b43 6f6e 7465 6e74 696f 6e54 6872 6561  kContentionThrea
-00006650: 644d 6169 6e12 790a 2374 696d 655f 6d6f  dMain.y.#time_mo
-00006660: 6e69 746f 725f 636f 6e74 656e 7469 6f6e  nitor_contention
-00006670: 5f74 6872 6561 645f 6d61 696e 1820 2001  _thread_main.  .
-00006680: 280b 322b 2e70 6572 6665 7474 6f2e 7072  (.2+.perfetto.pr
-00006690: 6f74 6f73 2e41 6e64 726f 6964 5374 6172  otos.AndroidStar
-000066a0: 7475 704d 6574 7269 632e 536c 6963 6552  tupMetric.SliceR
-000066b0: 1f74 696d 654d 6f6e 6974 6f72 436f 6e74  .timeMonitorCont
-000066c0: 656e 7469 6f6e 5468 7265 6164 4d61 696e  entionThreadMain
-000066d0: 4a04 080c 100d 4a04 080d 100e 4a04 080e  J.....J.....J...
-000066e0: 100f 4a04 080f 1010 1a5c 0a0a 4873 634d  ..J......\..HscM
-000066f0: 6574 7269 6373 124e 0a0c 6675 6c6c 5f73  etrics.N..full_s
-00006700: 7461 7274 7570 1801 2001 280b 322b 2e70  tartup.. .(.2+.p
-00006710: 6572 6665 7474 6f2e 7072 6f74 6f73 2e41  erfetto.protos.A
-00006720: 6e64 726f 6964 5374 6172 7475 704d 6574  ndroidStartupMet
-00006730: 7269 632e 536c 6963 6552 0b66 756c 6c53  ric.SliceR.fullS
-00006740: 7461 7274 7570 1a64 0a08 4163 7469 7669  tartup.d..Activi
-00006750: 7479 1212 0a04 6e61 6d65 1801 2001 2809  ty....name.. .(.
-00006760: 5204 6e61 6d65 1216 0a06 6d65 7468 6f64  R.name....method
-00006770: 1802 2001 2809 5206 6d65 7468 6f64 1226  .. .(.R.method.&
-00006780: 0a0f 7473 5f6d 6574 686f 645f 7374 6172  ..ts_method_star
-00006790: 7418 0420 0128 0352 0d74 734d 6574 686f  t.. .(.R.tsMetho
-000067a0: 6453 7461 7274 4a04 0803 1004 1a9b 020a  dStartJ.........
-000067b0: 1142 696e 6465 7254 7261 6e73 6163 7469  .BinderTransacti
-000067c0: 6f6e 1247 0a08 6475 7261 7469 6f6e 1801  on.G..duration..
-000067d0: 2001 280b 322b 2e70 6572 6665 7474 6f2e   .(.2+.perfetto.
-000067e0: 7072 6f74 6f73 2e41 6e64 726f 6964 5374  protos.AndroidSt
-000067f0: 6172 7475 704d 6574 7269 632e 536c 6963  artupMetric.Slic
-00006800: 6552 0864 7572 6174 696f 6e12 160a 0674  eR.duration....t
-00006810: 6872 6561 6418 0220 0128 0952 0674 6872  hread.. .(.R.thr
-00006820: 6561 6412 2d0a 1264 6573 7469 6e61 7469  ead.-..destinati
-00006830: 6f6e 5f74 6872 6561 6418 0320 0128 0952  on_thread.. .(.R
-00006840: 1164 6573 7469 6e61 7469 6f6e 5468 7265  .destinationThre
-00006850: 6164 122f 0a13 6465 7374 696e 6174 696f  ad./..destinatio
-00006860: 6e5f 7072 6f63 6573 7318 0420 0128 0952  n_process.. .(.R
-00006870: 1264 6573 7469 6e61 7469 6f6e 5072 6f63  .destinationProc
-00006880: 6573 7312 140a 0566 6c61 6773 1805 2001  ess....flags.. .
-00006890: 2809 5205 666c 6167 7312 120a 0463 6f64  (.R.flags....cod
-000068a0: 6518 0620 0128 0952 0463 6f64 6512 1b0a  e.. .(.R.code...
-000068b0: 0964 6174 615f 7369 7a65 1807 2001 2803  .data_size.. .(.
-000068c0: 5208 6461 7461 5369 7a65 1aaf 010a 124f  R.dataSize.....O
-000068d0: 7074 696d 697a 6174 696f 6e53 7461 7475  ptimizationStatu
-000068e0: 7312 1f0a 0b6f 6465 785f 7374 6174 7573  s....odex_status
-000068f0: 1801 2001 2809 520a 6f64 6578 5374 6174  .. .(.R.odexStat
-00006900: 7573 122d 0a12 636f 6d70 696c 6174 696f  us.-..compilatio
-00006910: 6e5f 6669 6c74 6572 1802 2001 2809 5211  n_filter.. .(.R.
-00006920: 636f 6d70 696c 6174 696f 6e46 696c 7465  compilationFilte
-00006930: 7212 2d0a 1263 6f6d 7069 6c61 7469 6f6e  r.-..compilation
-00006940: 5f72 6561 736f 6e18 0320 0128 0952 1163  _reason.. .(.R.c
-00006950: 6f6d 7069 6c61 7469 6f6e 5265 6173 6f6e  ompilationReason
-00006960: 121a 0a08 6c6f 6361 7469 6f6e 1804 2001  ....location.. .
-00006970: 2809 5208 6c6f 6361 7469 6f6e 1a5b 0a0f  (.R.location.[..
-00006980: 4576 656e 7454 696d 6573 7461 6d70 7312  EventTimestamps.
-00006990: 270a 0f69 6e74 656e 745f 7265 6365 6976  '..intent_receiv
-000069a0: 6564 1801 2001 2803 520e 696e 7465 6e74  ed.. .(.R.intent
-000069b0: 5265 6365 6976 6564 121f 0a0b 6669 7273  Received....firs
-000069c0: 745f 6672 616d 6518 0220 0128 0352 0a66  t_frame.. .(.R.f
-000069d0: 6972 7374 4672 616d 651a f702 0a0b 5379  irstFrame.....Sy
-000069e0: 7374 656d 5374 6174 6512 2b0a 0f64 6578  stemState.+..dex
-000069f0: 326f 6174 5f72 756e 6e69 6e67 1801 2001  2oat_running.. .
-00006a00: 2808 4202 1801 520e 6465 7832 6f61 7452  (.B...R.dex2oatR
-00006a10: 756e 6e69 6e67 122d 0a10 696e 7374 616c  unning.-..instal
-00006a20: 6c64 5f72 756e 6e69 6e67 1802 2001 2808  ld_running.. .(.
-00006a30: 4202 1801 520f 696e 7374 616c 6c64 5275  B...R.installdRu
-00006a40: 6e6e 696e 6712 3c0a 1a62 726f 6164 6361  nning.<..broadca
-00006a50: 7374 5f64 6973 7061 7463 6865 645f 636f  st_dispatched_co
-00006a60: 756e 7418 0320 0128 0352 1862 726f 6164  unt.. .(.R.broad
-00006a70: 6361 7374 4469 7370 6174 6368 6564 436f  castDispatchedCo
-00006a80: 756e 7412 380a 1862 726f 6164 6361 7374  unt.8..broadcast
-00006a90: 5f72 6563 6569 7665 645f 636f 756e 7418  _received_count.
-00006aa0: 0420 0128 0352 1662 726f 6164 6361 7374  . .(.R.broadcast
-00006ab0: 5265 6365 6976 6564 436f 756e 7412 460a  ReceivedCount.F.
-00006ac0: 206d 6f73 745f 6163 7469 7665 5f6e 6f6e   most_active_non
-00006ad0: 5f6c 6175 6e63 685f 7072 6f63 6573 7365  _launch_processe
-00006ae0: 7318 0520 0328 0952 1c6d 6f73 7441 6374  s.. .(.R.mostAct
-00006af0: 6976 654e 6f6e 4c61 756e 6368 5072 6f63  iveNonLaunchProc
-00006b00: 6573 7365 7312 260a 0f69 6e73 7461 6c6c  esses.&..install
-00006b10: 645f 6475 725f 6e73 1806 2001 2803 520d  d_dur_ns.. .(.R.
-00006b20: 696e 7374 616c 6c64 4475 724e 7312 240a  installdDurNs.$.
-00006b30: 0e64 6578 326f 6174 5f64 7572 5f6e 7318  .dex2oat_dur_ns.
-00006b40: 0720 0128 0352 0c64 6578 326f 6174 4475  . .(.R.dex2oatDu
-00006b50: 724e 731a d808 0a07 5374 6172 7475 7012  rNs.....Startup.
-00006b60: 1d0a 0a73 7461 7274 7570 5f69 6418 0120  ...startup_id.. 
-00006b70: 0128 0d52 0973 7461 7274 7570 4964 1221  .(.R.startupId.!
-00006b80: 0a0c 7374 6172 7475 705f 7479 7065 1810  ..startup_type..
-00006b90: 2001 2809 520b 7374 6172 7475 7054 7970   .(.R.startupTyp
-00006ba0: 6512 210a 0c70 6163 6b61 6765 5f6e 616d  e.!..package_nam
-00006bb0: 6518 0220 0128 0952 0b70 6163 6b61 6765  e.. .(.R.package
-00006bc0: 4e61 6d65 1221 0a0c 7072 6f63 6573 735f  Name.!..process_
-00006bd0: 6e61 6d65 1803 2001 2809 520b 7072 6f63  name.. .(.R.proc
-00006be0: 6573 734e 616d 6512 4e0a 0a61 6374 6976  essName.N..activ
-00006bf0: 6974 6965 7318 0b20 0328 0b32 2e2e 7065  ities.. .(.2..pe
-00006c00: 7266 6574 746f 2e70 726f 746f 732e 416e  rfetto.protos.An
-00006c10: 6472 6f69 6453 7461 7274 7570 4d65 7472  droidStartupMetr
-00006c20: 6963 2e41 6374 6976 6974 7952 0a61 6374  ic.ActivityR.act
-00006c30: 6976 6974 6965 7312 710a 186c 6f6e 675f  ivities.q..long_
-00006c40: 6269 6e64 6572 5f74 7261 6e73 6163 7469  binder_transacti
-00006c50: 6f6e 7318 0e20 0328 0b32 372e 7065 7266  ons.. .(.27.perf
-00006c60: 6574 746f 2e70 726f 746f 732e 416e 6472  etto.protos.Andr
-00006c70: 6f69 6453 7461 7274 7570 4d65 7472 6963  oidStartupMetric
-00006c80: 2e42 696e 6465 7254 7261 6e73 6163 7469  .BinderTransacti
-00006c90: 6f6e 5216 6c6f 6e67 4269 6e64 6572 5472  onR.longBinderTr
-00006ca0: 616e 7361 6374 696f 6e73 122c 0a12 7a79  ansactions.,..zy
-00006cb0: 676f 7465 5f6e 6577 5f70 726f 6365 7373  gote_new_process
-00006cc0: 1804 2001 2808 5210 7a79 676f 7465 4e65  .. .(.R.zygoteNe
-00006cd0: 7750 726f 6365 7373 1243 0a1e 6163 7469  wProcess.C..acti
-00006ce0: 7669 7479 5f68 6f73 7469 6e67 5f70 726f  vity_hosting_pro
-00006cf0: 6365 7373 5f63 6f75 6e74 1806 2001 280d  cess_count.. .(.
-00006d00: 521b 6163 7469 7669 7479 486f 7374 696e  R.activityHostin
-00006d10: 6750 726f 6365 7373 436f 756e 7412 600a  gProcessCount.`.
-00006d20: 1065 7665 6e74 5f74 696d 6573 7461 6d70  .event_timestamp
-00006d30: 7318 0d20 0128 0b32 352e 7065 7266 6574  s.. .(.25.perfet
-00006d40: 746f 2e70 726f 746f 732e 416e 6472 6f69  to.protos.Androi
-00006d50: 6453 7461 7274 7570 4d65 7472 6963 2e45  dStartupMetric.E
-00006d60: 7665 6e74 5469 6d65 7374 616d 7073 520f  ventTimestampsR.
-00006d70: 6576 656e 7454 696d 6573 7461 6d70 7312  eventTimestamps.
-00006d80: 580a 0e74 6f5f 6669 7273 745f 6672 616d  X..to_first_fram
-00006d90: 6518 0520 0128 0b32 322e 7065 7266 6574  e.. .(.22.perfet
-00006da0: 746f 2e70 726f 746f 732e 416e 6472 6f69  to.protos.Androi
-00006db0: 6453 7461 7274 7570 4d65 7472 6963 2e54  dStartupMetric.T
-00006dc0: 6f46 6972 7374 4672 616d 6552 0c74 6f46  oFirstFrameR.toF
-00006dd0: 6972 7374 4672 616d 6512 410a 0770 726f  irstFrame.A..pro
-00006de0: 6365 7373 1807 2001 280b 3227 2e70 6572  cess.. .(.2'.per
-00006df0: 6665 7474 6f2e 7072 6f74 6f73 2e41 6e64  fetto.protos.And
-00006e00: 726f 6964 5072 6f63 6573 734d 6574 6164  roidProcessMetad
-00006e10: 6174 6152 0770 726f 6365 7373 1242 0a03  ataR.process.B..
-00006e20: 6873 6318 0820 0128 0b32 302e 7065 7266  hsc.. .(.20.perf
-00006e30: 6574 746f 2e70 726f 746f 732e 416e 6472  etto.protos.Andr
-00006e40: 6f69 6453 7461 7274 7570 4d65 7472 6963  oidStartupMetric
-00006e50: 2e48 7363 4d65 7472 6963 7352 0368 7363  .HscMetricsR.hsc
-00006e60: 1259 0a12 7265 706f 7274 5f66 756c 6c79  .Y..report_fully
-00006e70: 5f64 7261 776e 1809 2001 280b 322b 2e70  _drawn.. .(.2+.p
-00006e80: 6572 6665 7474 6f2e 7072 6f74 6f73 2e41  erfetto.protos.A
-00006e90: 6e64 726f 6964 5374 6172 7475 704d 6574  ndroidStartupMet
-00006ea0: 7269 632e 536c 6963 6552 1072 6570 6f72  ric.SliceR.repor
-00006eb0: 7446 756c 6c79 4472 6177 6e12 690a 136f  tFullyDrawn.i..o
-00006ec0: 7074 696d 697a 6174 696f 6e5f 7374 6174  ptimization_stat
-00006ed0: 7573 180c 2003 280b 3238 2e70 6572 6665  us.. .(.28.perfe
-00006ee0: 7474 6f2e 7072 6f74 6f73 2e41 6e64 726f  tto.protos.Andro
-00006ef0: 6964 5374 6172 7475 704d 6574 7269 632e  idStartupMetric.
-00006f00: 4f70 7469 6d69 7a61 7469 6f6e 5374 6174  OptimizationStat
-00006f10: 7573 5212 6f70 7469 6d69 7a61 7469 6f6e  usR.optimization
-00006f20: 5374 6174 7573 1254 0a0c 7379 7374 656d  Status.T..system
-00006f30: 5f73 7461 7465 180f 2001 280b 3231 2e70  _state.. .(.21.p
-00006f40: 6572 6665 7474 6f2e 7072 6f74 6f73 2e41  erfetto.protos.A
-00006f50: 6e64 726f 6964 5374 6172 7475 704d 6574  ndroidStartupMet
-00006f60: 7269 632e 5379 7374 656d 5374 6174 6552  ric.SystemStateR
-00006f70: 0b73 7973 7465 6d53 7461 7465 122a 0a11  .systemState.*..
-00006f80: 736c 6f77 5f73 7461 7274 5f72 6561 736f  slow_start_reaso
-00006f90: 6e18 1120 0328 0952 0f73 6c6f 7753 7461  n.. .(.R.slowSta
-00006fa0: 7274 5265 6173 6f6e 4a04 080a 100b 0a9d  rtReasonJ.......
-00006fb0: 040a 3470 726f 746f 732f 7065 7266 6574  ..4protos/perfet
-00006fc0: 746f 2f6d 6574 7269 6373 2f61 6e64 726f  to/metrics/andro
-00006fd0: 6964 2f73 7572 6661 6365 666c 696e 6765  id/surfaceflinge
-00006fe0: 722e 7072 6f74 6f12 0f70 6572 6665 7474  r.proto..perfett
-00006ff0: 6f2e 7072 6f74 6f73 22d3 030a 1b41 6e64  o.protos"....And
-00007000: 726f 6964 5375 7266 6163 6566 6c69 6e67  roidSurfacefling
-00007010: 6572 4d65 7472 6963 1223 0a0d 6d69 7373  erMetric.#..miss
-00007020: 6564 5f66 7261 6d65 7318 0120 0128 0d52  ed_frames.. .(.R
-00007030: 0c6d 6973 7365 6446 7261 6d65 7312 2a0a  .missedFrames.*.
-00007040: 116d 6973 7365 645f 6877 635f 6672 616d  .missed_hwc_fram
-00007050: 6573 1802 2001 280d 520f 6d69 7373 6564  es.. .(.R.missed
-00007060: 4877 6346 7261 6d65 7312 2a0a 116d 6973  HwcFrames.*..mis
-00007070: 7365 645f 6770 755f 6672 616d 6573 1803  sed_gpu_frames..
-00007080: 2001 280d 520f 6d69 7373 6564 4770 7546   .(.R.missedGpuF
-00007090: 7261 6d65 7312 2a0a 116d 6973 7365 645f  rames.*..missed_
-000070a0: 6672 616d 655f 7261 7465 1804 2001 2801  frame_rate.. .(.
-000070b0: 520f 6d69 7373 6564 4672 616d 6552 6174  R.missedFrameRat
-000070c0: 6512 310a 156d 6973 7365 645f 6877 635f  e.1..missed_hwc_
-000070d0: 6672 616d 655f 7261 7465 1805 2001 2801  frame_rate.. .(.
-000070e0: 5212 6d69 7373 6564 4877 6346 7261 6d65  R.missedHwcFrame
-000070f0: 5261 7465 1231 0a15 6d69 7373 6564 5f67  Rate.1..missed_g
-00007100: 7075 5f66 7261 6d65 5f72 6174 6518 0620  pu_frame_rate.. 
-00007110: 0128 0152 126d 6973 7365 6447 7075 4672  .(.R.missedGpuFr
-00007120: 616d 6552 6174 6512 270a 0f67 7075 5f69  ameRate.'..gpu_i
-00007130: 6e76 6f63 6174 696f 6e73 1807 2001 280d  nvocations.. .(.
-00007140: 520e 6770 7549 6e76 6f63 6174 696f 6e73  R.gpuInvocations
-00007150: 1232 0a16 6176 675f 6770 755f 7761 6974  .2..avg_gpu_wait
-00007160: 696e 675f 6475 725f 6d73 1808 2001 2801  ing_dur_ms.. .(.
-00007170: 5212 6176 6747 7075 5761 6974 696e 6744  R.avgGpuWaitingD
-00007180: 7572 4d73 1248 0a22 746f 7461 6c5f 6e6f  urMs.H."total_no
-00007190: 6e5f 656d 7074 795f 6770 755f 7761 6974  n_empty_gpu_wait
-000071a0: 696e 675f 6475 725f 6d73 1809 2001 2801  ing_dur_ms.. .(.
-000071b0: 521c 746f 7461 6c4e 6f6e 456d 7074 7947  R.totalNonEmptyG
-000071c0: 7075 5761 6974 696e 6744 7572 4d73 0af0  puWaitingDurMs..
-000071d0: 030a 3770 726f 746f 732f 7065 7266 6574  ..7protos/perfet
-000071e0: 746f 2f6d 6574 7269 6373 2f61 6e64 726f  to/metrics/andro
-000071f0: 6964 2f73 7973 7569 5f63 756a 5f6d 6574  id/sysui_cuj_met
-00007200: 7269 6373 2e70 726f 746f 120f 7065 7266  rics.proto..perf
-00007210: 6574 746f 2e70 726f 746f 731a 3670 726f  etto.protos.6pro
-00007220: 746f 732f 7065 7266 6574 746f 2f6d 6574  tos/perfetto/met
-00007230: 7269 6373 2f61 6e64 726f 6964 2f70 726f  rics/android/pro
-00007240: 6365 7373 5f6d 6574 6164 6174 612e 7072  cess_metadata.pr
-00007250: 6f74 6f22 eb02 0a16 416e 6472 6f69 6453  oto"....AndroidS
-00007260: 7973 5569 4375 6a4d 6574 7269 6373 1245  ysUiCujMetrics.E
-00007270: 0a06 6672 616d 6573 1801 2003 280b 322d  ..frames.. .(.2-
-00007280: 2e70 6572 6665 7474 6f2e 7072 6f74 6f73  .perfetto.protos
-00007290: 2e41 6e64 726f 6964 5379 7355 6943 756a  .AndroidSysUiCuj
-000072a0: 4d65 7472 6963 732e 4672 616d 6552 0666  Metrics.FrameR.f
-000072b0: 7261 6d65 7312 190a 0863 756a 5f6e 616d  rames....cuj_nam
-000072c0: 6518 0220 0128 0952 0763 756a 4e61 6d65  e.. .(.R.cujName
-000072d0: 121b 0a09 6375 6a5f 7374 6172 7418 0320  ....cuj_start.. 
-000072e0: 0128 0352 0863 756a 5374 6172 7412 170a  .(.R.cujStart...
-000072f0: 0763 756a 5f64 7572 1804 2001 2803 5206  .cuj_dur.. .(.R.
-00007300: 6375 6a44 7572 1241 0a07 7072 6f63 6573  cujDur.A..proces
-00007310: 7318 0520 0128 0b32 272e 7065 7266 6574  s.. .(.2'.perfet
-00007320: 746f 2e70 726f 746f 732e 416e 6472 6f69  to.protos.Androi
-00007330: 6450 726f 6365 7373 4d65 7461 6461 7461  dProcessMetadata
-00007340: 5207 7072 6f63 6573 731a 760a 0546 7261  R.process.v..Fra
-00007350: 6d65 1216 0a06 6e75 6d62 6572 1801 2001  me....number.. .
-00007360: 2803 5206 6e75 6d62 6572 1214 0a05 7673  (.R.number....vs
-00007370: 796e 6318 0520 0128 0352 0576 7379 6e63  ync.. .(.R.vsync
-00007380: 120e 0a02 7473 1802 2001 2803 5202 7473  ....ts.. .(.R.ts
-00007390: 1210 0a03 6475 7218 0320 0128 0352 0364  ....dur.. .(.R.d
-000073a0: 7572 121d 0a0a 6a61 6e6b 5f63 6175 7365  ur....jank_cause
-000073b0: 1804 2003 2809 5209 6a61 6e6b 4361 7573  .. .(.R.jankCaus
-000073c0: 650a bb02 0a30 7072 6f74 6f73 2f70 6572  e....0protos/per
-000073d0: 6665 7474 6f2f 6d65 7472 6963 732f 616e  fetto/metrics/an
-000073e0: 6472 6f69 642f 7461 736b 5f6e 616d 6573  droid/task_names
-000073f0: 2e70 726f 746f 120f 7065 7266 6574 746f  .proto..perfetto
-00007400: 2e70 726f 746f 7322 f501 0a10 416e 6472  .protos"....Andr
-00007410: 6f69 6454 6173 6b4e 616d 6573 1243 0a07  oidTaskNames.C..
-00007420: 7072 6f63 6573 7318 0120 0328 0b32 292e  process.. .(.2).
-00007430: 7065 7266 6574 746f 2e70 726f 746f 732e  perfetto.protos.
-00007440: 416e 6472 6f69 6454 6173 6b4e 616d 6573  AndroidTaskNames
-00007450: 2e50 726f 6365 7373 5207 7072 6f63 6573  .ProcessR.proces
-00007460: 731a 9b01 0a07 5072 6f63 6573 7312 100a  s.....Process...
-00007470: 0370 6964 1801 2001 2803 5203 7069 6412  .pid.. .(.R.pid.
-00007480: 210a 0c70 726f 6365 7373 5f6e 616d 6518  !..process_name.
-00007490: 0220 0128 0952 0b70 726f 6365 7373 4e61  . .(.R.processNa
-000074a0: 6d65 121f 0a0b 7468 7265 6164 5f6e 616d  me....thread_nam
-000074b0: 6518 0320 0328 0952 0a74 6872 6561 644e  e.. .(.R.threadN
-000074c0: 616d 6512 100a 0375 6964 1804 2001 2803  ame....uid.. .(.
-000074d0: 5203 7569 6412 280a 1075 6964 5f70 6163  R.uid.(..uid_pac
-000074e0: 6b61 6765 5f6e 616d 6518 0520 0328 0952  kage_name.. .(.R
-000074f0: 0e75 6964 5061 636b 6167 654e 616d 650a  .uidPackageName.
-00007500: d301 0a33 7072 6f74 6f73 2f70 6572 6665  ...3protos/perfe
-00007510: 7474 6f2f 6d65 7472 6963 732f 616e 6472  tto/metrics/andr
-00007520: 6f69 642f 7472 6163 655f 7175 616c 6974  oid/trace_qualit
-00007530: 792e 7072 6f74 6f12 0f70 6572 6665 7474  y.proto..perfett
-00007540: 6f2e 7072 6f74 6f73 228a 010a 1941 6e64  o.protos"....And
-00007550: 726f 6964 5472 6163 6551 7561 6c69 7479  roidTraceQuality
-00007560: 4d65 7472 6963 124e 0a08 6661 696c 7572  Metric.N..failur
-00007570: 6573 1801 2003 280b 3232 2e70 6572 6665  es.. .(.22.perfe
-00007580: 7474 6f2e 7072 6f74 6f73 2e41 6e64 726f  tto.protos.Andro
-00007590: 6964 5472 6163 6551 7561 6c69 7479 4d65  idTraceQualityMe
-000075a0: 7472 6963 2e46 6169 6c75 7265 5208 6661  tric.FailureR.fa
-000075b0: 696c 7572 6573 1a1d 0a07 4661 696c 7572  ilures....Failur
-000075c0: 6512 120a 046e 616d 6518 0120 0128 0952  e....name.. .(.R
-000075d0: 046e 616d 650a 6d0a 3f70 726f 746f 732f  .name.m.?protos/
-000075e0: 7065 7266 6574 746f 2f6d 6574 7269 6373  perfetto/metrics
-000075f0: 2f61 6e64 726f 6964 2f61 6e64 726f 6964  /android/android
-00007600: 5f74 7275 7374 795f 776f 726b 7175 6575  _trusty_workqueu
-00007610: 6573 2e70 726f 746f 120f 7065 7266 6574  es.proto..perfet
-00007620: 746f 2e70 726f 746f 7322 190a 1741 6e64  to.protos"...And
-00007630: 726f 6964 5472 7573 7479 576f 726b 7175  roidTrustyWorkqu
-00007640: 6575 6573 0aa6 020a 3970 726f 746f 732f  eues....9protos/
-00007650: 7065 7266 6574 746f 2f6d 6574 7269 6373  perfetto/metrics
-00007660: 2f61 6e64 726f 6964 2f75 6e73 796d 626f  /android/unsymbo
-00007670: 6c69 7a65 645f 6672 616d 6573 2e70 726f  lized_frames.pro
-00007680: 746f 120f 7065 7266 6574 746f 2e70 726f  to..perfetto.pro
-00007690: 746f 7322 d701 0a12 556e 7379 6d62 6f6c  tos"....Unsymbol
-000076a0: 697a 6564 4672 616d 6573 1241 0a06 6672  izedFrames.A..fr
-000076b0: 616d 6573 1801 2003 280b 3229 2e70 6572  ames.. .(.2).per
-000076c0: 6665 7474 6f2e 7072 6f74 6f73 2e55 6e73  fetto.protos.Uns
-000076d0: 796d 626f 6c69 7a65 6446 7261 6d65 732e  ymbolizedFrames.
-000076e0: 4672 616d 6552 0666 7261 6d65 731a 7e0a  FrameR.frames.~.
-000076f0: 0546 7261 6d65 1216 0a06 6d6f 6475 6c65  .Frame....module
-00007700: 1801 2001 2809 5206 6d6f 6475 6c65 1219  .. .(.R.module..
-00007710: 0a08 6275 696c 645f 6964 1802 2001 2809  ..build_id.. .(.
-00007720: 5207 6275 696c 6449 6412 180a 0761 6464  R.buildId....add
-00007730: 7265 7373 1803 2001 2803 5207 6164 6472  ress.. .(.R.addr
-00007740: 6573 7312 280a 1067 6f6f 676c 655f 6c6f  ess.(..google_lo
-00007750: 6f6b 7570 5f69 6418 0420 0128 0952 0e67  okup_id.. .(.R.g
-00007760: 6f6f 676c 654c 6f6f 6b75 7049 640a c602  oogleLookupId...
-00007770: 0a33 7072 6f74 6f73 2f70 6572 6665 7474  .3protos/perfett
-00007780: 6f2f 6d65 7472 6963 732f 616e 6472 6f69  o/metrics/androi
-00007790: 642f 6269 6e64 6572 5f6d 6574 7269 632e  d/binder_metric.
-000077a0: 7072 6f74 6f12 0f70 6572 6665 7474 6f2e  proto..perfetto.
-000077b0: 7072 6f74 6f73 22fd 010a 1341 6e64 726f  protos"....Andro
-000077c0: 6964 4269 6e64 6572 4d65 7472 6963 1265  idBinderMetric.e
-000077d0: 0a11 7072 6f63 6573 735f 6272 6561 6b64  ..process_breakd
-000077e0: 6f77 6e18 0120 0328 0b32 382e 7065 7266  own.. .(.28.perf
-000077f0: 6574 746f 2e70 726f 746f 732e 416e 6472  etto.protos.Andr
-00007800: 6f69 6442 696e 6465 724d 6574 7269 632e  oidBinderMetric.
-00007810: 5065 7250 726f 6365 7373 4272 6561 6b64  PerProcessBreakd
-00007820: 6f77 6e52 1070 726f 6365 7373 4272 6561  ownR.processBrea
-00007830: 6b64 6f77 6e1a 7f0a 1350 6572 5072 6f63  kdown....PerProc
-00007840: 6573 7342 7265 616b 646f 776e 1221 0a0c  essBreakdown.!..
-00007850: 7072 6f63 6573 735f 6e61 6d65 1801 2001  process_name.. .
-00007860: 2809 520b 7072 6f63 6573 734e 616d 6512  (.R.processName.
-00007870: 100a 0370 6964 1802 2001 280d 5203 7069  ...pid.. .(.R.pi
-00007880: 6412 1d0a 0a73 6c69 6365 5f6e 616d 6518  d....slice_name.
-00007890: 0320 0128 0952 0973 6c69 6365 4e61 6d65  . .(.R.sliceName
-000078a0: 1214 0a05 636f 756e 7418 0420 0128 0d52  ....count.. .(.R
-000078b0: 0563 6f75 6e74 0af6 310a 2570 726f 746f  .count..1.%proto
-000078c0: 732f 7065 7266 6574 746f 2f6d 6574 7269  s/perfetto/metri
-000078d0: 6373 2f6d 6574 7269 6373 2e70 726f 746f  cs/metrics.proto
-000078e0: 120f 7065 7266 6574 746f 2e70 726f 746f  ..perfetto.proto
-000078f0: 731a 4370 726f 746f 732f 7065 7266 6574  s.Cprotos/perfet
-00007900: 746f 2f6d 6574 7269 6373 2f61 6e64 726f  to/metrics/andro
-00007910: 6964 2f61 6e64 726f 6964 5f66 7261 6d65  id/android_frame
-00007920: 5f74 696d 656c 696e 655f 6d65 7472 6963  _timeline_metric
-00007930: 2e70 726f 746f 1a31 7072 6f74 6f73 2f70  .proto.1protos/p
-00007940: 6572 6665 7474 6f2f 6d65 7472 6963 732f  erfetto/metrics/
-00007950: 616e 6472 6f69 642f 6261 7474 5f6d 6574  android/batt_met
-00007960: 7269 632e 7072 6f74 6f1a 3070 726f 746f  ric.proto.0proto
-00007970: 732f 7065 7266 6574 746f 2f6d 6574 7269  s/perfetto/metri
-00007980: 6373 2f61 6e64 726f 6964 2f63 7075 5f6d  cs/android/cpu_m
-00007990: 6574 7269 632e 7072 6f74 6f1a 3370 726f  etric.proto.3pro
-000079a0: 746f 732f 7065 7266 6574 746f 2f6d 6574  tos/perfetto/met
-000079b0: 7269 6373 2f61 6e64 726f 6964 2f63 616d  rics/android/cam
-000079c0: 6572 615f 6d65 7472 6963 2e70 726f 746f  era_metric.proto
-000079d0: 1a39 7072 6f74 6f73 2f70 6572 6665 7474  .9protos/perfett
-000079e0: 6f2f 6d65 7472 6963 732f 616e 6472 6f69  o/metrics/androi
-000079f0: 642f 6361 6d65 7261 5f75 6e61 6767 5f6d  d/camera_unagg_m
-00007a00: 6574 7269 632e 7072 6f74 6f1a 3570 726f  etric.proto.5pro
-00007a10: 746f 732f 7065 7266 6574 746f 2f6d 6574  tos/perfetto/met
-00007a20: 7269 6373 2f61 6e64 726f 6964 2f64 6973  rics/android/dis
-00007a30: 706c 6179 5f6d 6574 7269 6373 2e70 726f  play_metrics.pro
-00007a40: 746f 1a35 7072 6f74 6f73 2f70 6572 6665  to.5protos/perfe
-00007a50: 7474 6f2f 6d65 7472 6963 732f 616e 6472  tto/metrics/andr
-00007a60: 6f69 642f 646d 615f 6865 6170 5f6d 6574  oid/dma_heap_met
-00007a70: 7269 632e 7072 6f74 6f1a 3170 726f 746f  ric.proto.1proto
-00007a80: 732f 7065 7266 6574 746f 2f6d 6574 7269  s/perfetto/metri
-00007a90: 6373 2f61 6e64 726f 6964 2f64 7666 735f  cs/android/dvfs_
-00007aa0: 6d65 7472 6963 2e70 726f 746f 1a34 7072  metric.proto.4pr
-00007ab0: 6f74 6f73 2f70 6572 6665 7474 6f2f 6d65  otos/perfetto/me
-00007ac0: 7472 6963 732f 616e 6472 6f69 642f 6661  trics/android/fa
-00007ad0: 7374 7270 635f 6d65 7472 6963 2e70 726f  strpc_metric.pro
-00007ae0: 746f 1a30 7072 6f74 6f73 2f70 6572 6665  to.0protos/perfe
-00007af0: 7474 6f2f 6d65 7472 6963 732f 616e 6472  tto/metrics/andr
-00007b00: 6f69 642f 6732 645f 6d65 7472 6963 2e70  oid/g2d_metric.p
-00007b10: 726f 746f 1a30 7072 6f74 6f73 2f70 6572  roto.0protos/per
-00007b20: 6665 7474 6f2f 6d65 7472 6963 732f 616e  fetto/metrics/an
-00007b30: 6472 6f69 642f 6770 755f 6d65 7472 6963  droid/gpu_metric
-00007b40: 2e70 726f 746f 1a30 7072 6f74 6f73 2f70  .proto.0protos/p
-00007b50: 6572 6665 7474 6f2f 6d65 7472 6963 732f  erfetto/metrics/
-00007b60: 616e 6472 6f69 642f 6877 636f 6d70 6f73  android/hwcompos
-00007b70: 6572 2e70 726f 746f 1a31 7072 6f74 6f73  er.proto.1protos
-00007b80: 2f70 6572 6665 7474 6f2f 6d65 7472 6963  /perfetto/metric
-00007b90: 732f 616e 6472 6f69 642f 6877 7569 5f6d  s/android/hwui_m
-00007ba0: 6574 7269 632e 7072 6f74 6f1a 3070 726f  etric.proto.0pro
-00007bb0: 746f 732f 7065 7266 6574 746f 2f6d 6574  tos/perfetto/met
-00007bc0: 7269 6373 2f61 6e64 726f 6964 2f69 6f6e  rics/android/ion
-00007bd0: 5f6d 6574 7269 632e 7072 6f74 6f1a 3870  _metric.proto.8p
-00007be0: 726f 746f 732f 7065 7266 6574 746f 2f6d  rotos/perfetto/m
-00007bf0: 6574 7269 6373 2f61 6e64 726f 6964 2f69  etrics/android/i
-00007c00: 7271 5f72 756e 7469 6d65 5f6d 6574 7269  rq_runtime_metri
-00007c10: 632e 7072 6f74 6f1a 3570 726f 746f 732f  c.proto.5protos/
-00007c20: 7065 7266 6574 746f 2f6d 6574 7269 6373  perfetto/metrics
-00007c30: 2f61 6e64 726f 6964 2f6a 616e 6b5f 6375  /android/jank_cu
-00007c40: 6a5f 6d65 7472 6963 2e70 726f 746f 1a39  j_metric.proto.9
-00007c50: 7072 6f74 6f73 2f70 6572 6665 7474 6f2f  protos/perfetto/
-00007c60: 6d65 7472 6963 732f 616e 6472 6f69 642f  metrics/android/
-00007c70: 6a61 7661 5f68 6561 705f 6869 7374 6f67  java_heap_histog
-00007c80: 7261 6d2e 7072 6f74 6f1a 3570 726f 746f  ram.proto.5proto
-00007c90: 732f 7065 7266 6574 746f 2f6d 6574 7269  s/perfetto/metri
-00007ca0: 6373 2f61 6e64 726f 6964 2f6a 6176 615f  cs/android/java_
-00007cb0: 6865 6170 5f73 7461 7473 2e70 726f 746f  heap_stats.proto
-00007cc0: 1a30 7072 6f74 6f73 2f70 6572 6665 7474  .0protos/perfett
-00007cd0: 6f2f 6d65 7472 6963 732f 616e 6472 6f69  o/metrics/androi
-00007ce0: 642f 6c6d 6b5f 6d65 7472 6963 2e70 726f  d/lmk_metric.pro
-00007cf0: 746f 1a37 7072 6f74 6f73 2f70 6572 6665  to.7protos/perfe
-00007d00: 7474 6f2f 6d65 7472 6963 732f 616e 6472  tto/metrics/andr
-00007d10: 6f69 642f 6c6d 6b5f 7265 6173 6f6e 5f6d  oid/lmk_reason_m
-00007d20: 6574 7269 632e 7072 6f74 6f1a 3070 726f  etric.proto.0pro
-00007d30: 746f 732f 7065 7266 6574 746f 2f6d 6574  tos/perfetto/met
-00007d40: 7269 6373 2f61 6e64 726f 6964 2f6d 656d  rics/android/mem
-00007d50: 5f6d 6574 7269 632e 7072 6f74 6f1a 3670  _metric.proto.6p
-00007d60: 726f 746f 732f 7065 7266 6574 746f 2f6d  rotos/perfetto/m
-00007d70: 6574 7269 6373 2f61 6e64 726f 6964 2f6d  etrics/android/m
-00007d80: 656d 5f75 6e61 6767 5f6d 6574 7269 632e  em_unagg_metric.
-00007d90: 7072 6f74 6f1a 3670 726f 746f 732f 7065  proto.6protos/pe
-00007da0: 7266 6574 746f 2f6d 6574 7269 6373 2f61  rfetto/metrics/a
-00007db0: 6e64 726f 6964 2f6d 756c 7469 7573 6572  ndroid/multiuser
-00007dc0: 5f6d 6574 7269 632e 7072 6f74 6f1a 3470  _metric.proto.4p
-00007dd0: 726f 746f 732f 7065 7266 6574 746f 2f6d  rotos/perfetto/m
-00007de0: 6574 7269 6373 2f61 6e64 726f 6964 2f6e  etrics/android/n
-00007df0: 6574 776f 726b 5f6d 6574 7269 632e 7072  etwork_metric.pr
-00007e00: 6f74 6f1a 3270 726f 746f 732f 7065 7266  oto.2protos/perf
-00007e10: 6574 746f 2f6d 6574 7269 6373 2f61 6e64  etto/metrics/and
-00007e20: 726f 6964 2f6f 7468 6572 5f74 7261 6365  roid/other_trace
-00007e30: 732e 7072 6f74 6f1a 3270 726f 746f 732f  s.proto.2protos/
-00007e40: 7065 7266 6574 746f 2f6d 6574 7269 6373  perfetto/metrics
-00007e50: 2f61 6e64 726f 6964 2f70 6163 6b61 6765  /android/package
-00007e60: 5f6c 6973 742e 7072 6f74 6f1a 3570 726f  _list.proto.5pro
-00007e70: 746f 732f 7065 7266 6574 746f 2f6d 6574  tos/perfetto/met
-00007e80: 7269 6373 2f61 6e64 726f 6964 2f70 6f77  rics/android/pow
-00007e90: 7261 696c 735f 6d65 7472 6963 2e70 726f  rails_metric.pro
-00007ea0: 746f 1a34 7072 6f74 6f73 2f70 6572 6665  to.4protos/perfe
-00007eb0: 7474 6f2f 6d65 7472 6963 732f 616e 6472  tto/metrics/andr
-00007ec0: 6f69 642f 7072 6f66 696c 6572 5f73 6d61  oid/profiler_sma
-00007ed0: 7073 2e70 726f 746f 1a37 7072 6f74 6f73  ps.proto.7protos
-00007ee0: 2f70 6572 6665 7474 6f2f 6d65 7472 6963  /perfetto/metric
-00007ef0: 732f 616e 6472 6f69 642f 7274 5f72 756e  s/android/rt_run
-00007f00: 7469 6d65 5f6d 6574 7269 632e 7072 6f74  time_metric.prot
-00007f10: 6f1a 3070 726f 746f 732f 7065 7266 6574  o.0protos/perfet
-00007f20: 746f 2f6d 6574 7269 6373 2f61 6e64 726f  to/metrics/andro
-00007f30: 6964 2f73 696d 706c 6570 6572 662e 7072  id/simpleperf.pr
-00007f40: 6f74 6f1a 3470 726f 746f 732f 7065 7266  oto.4protos/perf
-00007f50: 6574 746f 2f6d 6574 7269 6373 2f61 6e64  etto/metrics/and
-00007f60: 726f 6964 2f73 7461 7274 7570 5f6d 6574  roid/startup_met
-00007f70: 7269 632e 7072 6f74 6f1a 3470 726f 746f  ric.proto.4proto
-00007f80: 732f 7065 7266 6574 746f 2f6d 6574 7269  s/perfetto/metri
-00007f90: 6373 2f61 6e64 726f 6964 2f73 7572 6661  cs/android/surfa
-00007fa0: 6365 666c 696e 6765 722e 7072 6f74 6f1a  ceflinger.proto.
-00007fb0: 3770 726f 746f 732f 7065 7266 6574 746f  7protos/perfetto
-00007fc0: 2f6d 6574 7269 6373 2f61 6e64 726f 6964  /metrics/android
-00007fd0: 2f73 7973 7569 5f63 756a 5f6d 6574 7269  /sysui_cuj_metri
-00007fe0: 6373 2e70 726f 746f 1a30 7072 6f74 6f73  cs.proto.0protos
-00007ff0: 2f70 6572 6665 7474 6f2f 6d65 7472 6963  /perfetto/metric
-00008000: 732f 616e 6472 6f69 642f 7461 736b 5f6e  s/android/task_n
-00008010: 616d 6573 2e70 726f 746f 1a33 7072 6f74  ames.proto.3prot
-00008020: 6f73 2f70 6572 6665 7474 6f2f 6d65 7472  os/perfetto/metr
-00008030: 6963 732f 616e 6472 6f69 642f 7472 6163  ics/android/trac
-00008040: 655f 7175 616c 6974 792e 7072 6f74 6f1a  e_quality.proto.
-00008050: 3f70 726f 746f 732f 7065 7266 6574 746f  ?protos/perfetto
-00008060: 2f6d 6574 7269 6373 2f61 6e64 726f 6964  /metrics/android
-00008070: 2f61 6e64 726f 6964 5f74 7275 7374 795f  /android_trusty_
-00008080: 776f 726b 7175 6575 6573 2e70 726f 746f  workqueues.proto
-00008090: 1a39 7072 6f74 6f73 2f70 6572 6665 7474  .9protos/perfett
-000080a0: 6f2f 6d65 7472 6963 732f 616e 6472 6f69  o/metrics/androi
-000080b0: 642f 756e 7379 6d62 6f6c 697a 6564 5f66  d/unsymbolized_f
-000080c0: 7261 6d65 732e 7072 6f74 6f1a 3370 726f  rames.proto.3pro
-000080d0: 746f 732f 7065 7266 6574 746f 2f6d 6574  tos/perfetto/met
-000080e0: 7269 6373 2f61 6e64 726f 6964 2f62 696e  rics/android/bin
-000080f0: 6465 725f 6d65 7472 6963 2e70 726f 746f  der_metric.proto
-00008100: 22c0 030a 0d54 7261 6365 4d65 7461 6461  "....TraceMetada
-00008110: 7461 122a 0a11 7472 6163 655f 6475 7261  ta.*..trace_dura
-00008120: 7469 6f6e 5f6e 7318 0220 0128 0352 0f74  tion_ns.. .(.R.t
-00008130: 7261 6365 4475 7261 7469 6f6e 4e73 121d  raceDurationNs..
-00008140: 0a0a 7472 6163 655f 7575 6964 1803 2001  ..trace_uuid.. .
-00008150: 2809 5209 7472 6163 6555 7569 6412 3a0a  (.R.traceUuid.:.
-00008160: 1961 6e64 726f 6964 5f62 7569 6c64 5f66  .android_build_f
-00008170: 696e 6765 7270 7269 6e74 1804 2001 2809  ingerprint.. .(.
-00008180: 5217 616e 6472 6f69 6442 7569 6c64 4669  R.androidBuildFi
-00008190: 6e67 6572 7072 696e 7412 490a 2173 7461  ngerprint.I.!sta
-000081a0: 7473 645f 7472 6967 6765 7269 6e67 5f73  tsd_triggering_s
-000081b0: 7562 7363 7269 7074 696f 6e5f 6964 1805  ubscription_id..
-000081c0: 2001 2803 521e 7374 6174 7364 5472 6967   .(.R.statsdTrig
-000081d0: 6765 7269 6e67 5375 6273 6372 6970 7469  geringSubscripti
-000081e0: 6f6e 4964 1228 0a10 7472 6163 655f 7369  onId.(..trace_si
-000081f0: 7a65 5f62 7974 6573 1806 2001 2803 520e  ze_bytes.. .(.R.
-00008200: 7472 6163 6553 697a 6542 7974 6573 1223  traceSizeBytes.#
-00008210: 0a0d 7472 6163 655f 7472 6967 6765 7218  ..trace_trigger.
-00008220: 0720 0328 0952 0c74 7261 6365 5472 6967  . .(.R.traceTrig
-00008230: 6765 7212 2e0a 1375 6e69 7175 655f 7365  ger....unique_se
-00008240: 7373 696f 6e5f 6e61 6d65 1808 2001 2809  ssion_name.. .(.
-00008250: 5211 756e 6971 7565 5365 7373 696f 6e4e  R.uniqueSessionN
-00008260: 616d 6512 2c0a 1274 7261 6365 5f63 6f6e  ame.,..trace_con
-00008270: 6669 675f 7062 7478 7418 0920 0128 0952  fig_pbtxt.. .(.R
-00008280: 1074 7261 6365 436f 6e66 6967 5062 7478  .traceConfigPbtx
-00008290: 7412 2a0a 1173 6368 6564 5f64 7572 6174  t.*..sched_durat
-000082a0: 696f 6e5f 6e73 180a 2001 2803 520f 7363  ion_ns.. .(.R.sc
-000082b0: 6865 6444 7572 6174 696f 6e4e 734a 0408  hedDurationNsJ..
-000082c0: 0110 0222 cb03 0a12 5472 6163 6541 6e61  ..."....TraceAna
-000082d0: 6c79 7369 7353 7461 7473 123c 0a04 7374  lysisStats.<..st
-000082e0: 6174 1801 2003 280b 3228 2e70 6572 6665  at.. .(.2(.perfe
-000082f0: 7474 6f2e 7072 6f74 6f73 2e54 7261 6365  tto.protos.Trace
-00008300: 416e 616c 7973 6973 5374 6174 732e 5374  AnalysisStats.St
-00008310: 6174 5204 7374 6174 1ad0 010a 0453 7461  atR.stat.....Sta
-00008320: 7412 120a 046e 616d 6518 0120 0128 0952  t....name.. .(.R
-00008330: 046e 616d 6512 100a 0369 6478 1802 2001  .name....idx.. .
-00008340: 280d 5203 6964 7812 480a 0873 6576 6572  (.R.idx.H..sever
-00008350: 6974 7918 0320 0128 0e32 2c2e 7065 7266  ity.. .(.2,.perf
-00008360: 6574 746f 2e70 726f 746f 732e 5472 6163  etto.protos.Trac
-00008370: 6541 6e61 6c79 7369 7353 7461 7473 2e53  eAnalysisStats.S
-00008380: 6576 6572 6974 7952 0873 6576 6572 6974  everityR.severit
-00008390: 7912 420a 0673 6f75 7263 6518 0420 0128  y.B..source.. .(
-000083a0: 0e32 2a2e 7065 7266 6574 746f 2e70 726f  .2*.perfetto.pro
-000083b0: 746f 732e 5472 6163 6541 6e61 6c79 7369  tos.TraceAnalysi
-000083c0: 7353 7461 7473 2e53 6f75 7263 6552 0673  sStats.SourceR.s
-000083d0: 6f75 7263 6512 140a 0563 6f75 6e74 1805  ource....count..
-000083e0: 2001 2803 5205 636f 756e 7422 5f0a 0853   .(.R.count"_..S
-000083f0: 6576 6572 6974 7912 140a 1053 4556 4552  everity....SEVER
-00008400: 4954 595f 554e 4b4e 4f57 4e10 0012 110a  ITY_UNKNOWN.....
-00008410: 0d53 4556 4552 4954 595f 494e 464f 1001  .SEVERITY_INFO..
-00008420: 1216 0a12 5345 5645 5249 5459 5f44 4154  ....SEVERITY_DAT
-00008430: 415f 4c4f 5353 1002 1212 0a0e 5345 5645  A_LOSS......SEVE
-00008440: 5249 5459 5f45 5252 4f52 1003 2243 0a06  RITY_ERROR.."C..
-00008450: 536f 7572 6365 1212 0a0e 534f 5552 4345  Source....SOURCE
-00008460: 5f55 4e4b 4e4f 574e 1000 1210 0a0c 534f  _UNKNOWN......SO
-00008470: 5552 4345 5f54 5241 4345 1001 1213 0a0f  URCE_TRACE......
-00008480: 534f 5552 4345 5f41 4e41 4c59 5349 5310  SOURCE_ANALYSIS.
-00008490: 0222 9b1a 0a0c 5472 6163 654d 6574 7269  ."....TraceMetri
-000084a0: 6373 1248 0a0c 616e 6472 6f69 645f 6261  cs.H..android_ba
-000084b0: 7474 1805 2001 280b 3225 2e70 6572 6665  tt.. .(.2%.perfe
-000084c0: 7474 6f2e 7072 6f74 6f73 2e41 6e64 726f  tto.protos.Andro
-000084d0: 6964 4261 7474 6572 794d 6574 7269 6352  idBatteryMetricR
-000084e0: 0b61 6e64 726f 6964 4261 7474 1242 0a0b  .androidBatt.B..
-000084f0: 616e 6472 6f69 645f 6370 7518 0620 0128  android_cpu.. .(
-00008500: 0b32 212e 7065 7266 6574 746f 2e70 726f  .2!.perfetto.pro
-00008510: 746f 732e 416e 6472 6f69 6443 7075 4d65  tos.AndroidCpuMe
-00008520: 7472 6963 520a 616e 6472 6f69 6443 7075  tricR.androidCpu
-00008530: 1245 0a0b 616e 6472 6f69 645f 6d65 6d18  .E..android_mem.
-00008540: 0120 0128 0b32 242e 7065 7266 6574 746f  . .(.2$.perfetto
-00008550: 2e70 726f 746f 732e 416e 6472 6f69 644d  .protos.AndroidM
-00008560: 656d 6f72 794d 6574 7269 6352 0a61 6e64  emoryMetricR.and
-00008570: 726f 6964 4d65 6d12 5c0a 1161 6e64 726f  roidMem.\..andro
-00008580: 6964 5f6d 656d 5f75 6e61 6767 180b 2001  id_mem_unagg.. .
-00008590: 280b 3230 2e70 6572 6665 7474 6f2e 7072  (.20.perfetto.pr
-000085a0: 6f74 6f73 2e41 6e64 726f 6964 4d65 6d6f  otos.AndroidMemo
-000085b0: 7279 556e 6167 6772 6567 6174 6564 4d65  ryUnaggregatedMe
-000085c0: 7472 6963 520f 616e 6472 6f69 644d 656d  tricR.androidMem
-000085d0: 556e 6167 6712 550a 1461 6e64 726f 6964  Unagg.U..android
-000085e0: 5f70 6163 6b61 6765 5f6c 6973 7418 0c20  _package_list.. 
-000085f0: 0128 0b32 232e 7065 7266 6574 746f 2e70  .(.2#.perfetto.p
-00008600: 726f 746f 732e 416e 6472 6f69 6450 6163  rotos.AndroidPac
-00008610: 6b61 6765 4c69 7374 5212 616e 6472 6f69  kageListR.androi
-00008620: 6450 6163 6b61 6765 4c69 7374 1242 0a0b  dPackageList.B..
-00008630: 616e 6472 6f69 645f 696f 6e18 0920 0128  android_ion.. .(
-00008640: 0b32 212e 7065 7266 6574 746f 2e70 726f  .2!.perfetto.pro
-00008650: 746f 732e 416e 6472 6f69 6449 6f6e 4d65  tos.AndroidIonMe
-00008660: 7472 6963 520a 616e 6472 6f69 6449 6f6e  tricR.androidIon
-00008670: 124e 0a0f 616e 6472 6f69 645f 6661 7374  .N..android_fast
-00008680: 7270 6318 1f20 0128 0b32 252e 7065 7266  rpc.. .(.2%.perf
-00008690: 6574 746f 2e70 726f 746f 732e 416e 6472  etto.protos.Andr
-000086a0: 6f69 6446 6173 7472 7063 4d65 7472 6963  oidFastrpcMetric
-000086b0: 520e 616e 6472 6f69 6446 6173 7472 7063  R.androidFastrpc
-000086c0: 1242 0a0b 616e 6472 6f69 645f 6c6d 6b18  .B..android_lmk.
-000086d0: 0820 0128 0b32 212e 7065 7266 6574 746f  . .(.2!.perfetto
-000086e0: 2e70 726f 746f 732e 416e 6472 6f69 644c  .protos.AndroidL
-000086f0: 6d6b 4d65 7472 6963 520a 616e 6472 6f69  mkMetricR.androi
-00008700: 644c 6d6b 124d 0a10 616e 6472 6f69 645f  dLmk.M..android_
-00008710: 706f 7772 6169 6c73 1807 2001 280b 3222  powrails.. .(.2"
-00008720: 2e70 6572 6665 7474 6f2e 7072 6f74 6f73  .perfetto.protos
-00008730: 2e41 6e64 726f 6964 506f 7765 7252 6169  .AndroidPowerRai
-00008740: 6c73 520f 616e 6472 6f69 6450 6f77 7261  lsR.androidPowra
-00008750: 696c 7312 4e0a 0f61 6e64 726f 6964 5f73  ils.N..android_s
-00008760: 7461 7274 7570 1802 2001 280b 3225 2e70  tartup.. .(.2%.p
-00008770: 6572 6665 7474 6f2e 7072 6f74 6f73 2e41  erfetto.protos.A
-00008780: 6e64 726f 6964 5374 6172 7475 704d 6574  ndroidStartupMet
-00008790: 7269 6352 0e61 6e64 726f 6964 5374 6172  ricR.androidStar
-000087a0: 7475 7012 450a 0e74 7261 6365 5f6d 6574  tup.E..trace_met
-000087b0: 6164 6174 6118 0320 0128 0b32 1e2e 7065  adata.. .(.2..pe
-000087c0: 7266 6574 746f 2e70 726f 746f 732e 5472  rfetto.protos.Tr
-000087d0: 6163 654d 6574 6164 6174 6152 0d74 7261  aceMetadataR.tra
-000087e0: 6365 4d65 7461 6461 7461 1244 0a0b 7472  ceMetadata.D..tr
-000087f0: 6163 655f 7374 6174 7318 2120 0128 0b32  ace_stats.! .(.2
-00008800: 232e 7065 7266 6574 746f 2e70 726f 746f  #.perfetto.proto
-00008810: 732e 5472 6163 6541 6e61 6c79 7369 7353  s.TraceAnalysisS
-00008820: 7461 7473 520a 7472 6163 6553 7461 7473  tatsR.traceStats
-00008830: 1254 0a13 756e 7379 6d62 6f6c 697a 6564  .T..unsymbolized
-00008840: 5f66 7261 6d65 7318 0f20 0128 0b32 232e  _frames.. .(.2#.
-00008850: 7065 7266 6574 746f 2e70 726f 746f 732e  perfetto.protos.
-00008860: 556e 7379 6d62 6f6c 697a 6564 4672 616d  UnsymbolizedFram
-00008870: 6573 5212 756e 7379 6d62 6f6c 697a 6564  esR.unsymbolized
-00008880: 4672 616d 6573 1246 0a0f 6a61 7661 5f68  Frames.F..java_h
-00008890: 6561 705f 7374 6174 7318 1120 0128 0b32  eap_stats.. .(.2
-000088a0: 1e2e 7065 7266 6574 746f 2e70 726f 746f  ..perfetto.proto
-000088b0: 732e 4a61 7661 4865 6170 5374 6174 7352  s.JavaHeapStatsR
-000088c0: 0d6a 6176 6148 6561 7053 7461 7473 1252  .javaHeapStats.R
-000088d0: 0a13 6a61 7661 5f68 6561 705f 6869 7374  ..java_heap_hist
-000088e0: 6f67 7261 6d18 1520 0128 0b32 222e 7065  ogram.. .(.2".pe
-000088f0: 7266 6574 746f 2e70 726f 746f 732e 4a61  rfetto.protos.Ja
-00008900: 7661 4865 6170 4869 7374 6f67 7261 6d52  vaHeapHistogramR
-00008910: 116a 6176 6148 6561 7048 6973 746f 6772  .javaHeapHistogr
-00008920: 616d 1255 0a12 616e 6472 6f69 645f 6c6d  am.U..android_lm
-00008930: 6b5f 7265 6173 6f6e 1812 2001 280b 3227  k_reason.. .(.2'
-00008940: 2e70 6572 6665 7474 6f2e 7072 6f74 6f73  .perfetto.protos
-00008950: 2e41 6e64 726f 6964 4c6d 6b52 6561 736f  .AndroidLmkReaso
-00008960: 6e4d 6574 7269 6352 1061 6e64 726f 6964  nMetricR.android
-00008970: 4c6d 6b52 6561 736f 6e12 520a 1361 6e64  LmkReason.R..and
-00008980: 726f 6964 5f68 7775 695f 6d65 7472 6963  roid_hwui_metric
-00008990: 1814 2001 280b 3222 2e70 6572 6665 7474  .. .(.2".perfett
-000089a0: 6f2e 7072 6f74 6f73 2e41 6e64 726f 6964  o.protos.Android
-000089b0: 4877 7569 4d65 7472 6963 5211 616e 6472  HwuiMetricR.andr
-000089c0: 6f69 6448 7775 694d 6574 7269 6312 4f0a  oidHwuiMetric.O.
-000089d0: 0f64 6973 706c 6179 5f6d 6574 7269 6373  .display_metrics
-000089e0: 1816 2001 280b 3226 2e70 6572 6665 7474  .. .(.2&.perfett
-000089f0: 6f2e 7072 6f74 6f73 2e41 6e64 726f 6964  o.protos.Android
-00008a00: 4469 7370 6c61 794d 6574 7269 6373 520e  DisplayMetricsR.
-00008a10: 6469 7370 6c61 794d 6574 7269 6373 124f  displayMetrics.O
-00008a20: 0a12 616e 6472 6f69 645f 7461 736b 5f6e  ..android_task_n
-00008a30: 616d 6573 1817 2001 280b 3221 2e70 6572  ames.. .(.2!.per
-00008a40: 6665 7474 6f2e 7072 6f74 6f73 2e41 6e64  fetto.protos.And
-00008a50: 726f 6964 5461 736b 4e61 6d65 7352 1061  roidTaskNamesR.a
-00008a60: 6e64 726f 6964 5461 736b 4e61 6d65 7312  ndroidTaskNames.
-00008a70: 630a 1661 6e64 726f 6964 5f73 7572 6661  c..android_surfa
-00008a80: 6365 666c 696e 6765 7218 1920 0128 0b32  ceflinger.. .(.2
-00008a90: 2c2e 7065 7266 6574 746f 2e70 726f 746f  ,.perfetto.proto
-00008aa0: 732e 416e 6472 6f69 6453 7572 6661 6365  s.AndroidSurface
-00008ab0: 666c 696e 6765 724d 6574 7269 6352 1561  flingerMetricR.a
-00008ac0: 6e64 726f 6964 5375 7266 6163 6566 6c69  ndroidSurfacefli
-00008ad0: 6e67 6572 1242 0a0b 616e 6472 6f69 645f  nger.B..android_
-00008ae0: 6770 7518 1a20 0128 0b32 212e 7065 7266  gpu.. .(.2!.perf
-00008af0: 6574 746f 2e70 726f 746f 732e 416e 6472  etto.protos.Andr
-00008b00: 6f69 6447 7075 4d65 7472 6963 520a 616e  oidGpuMetricR.an
-00008b10: 6472 6f69 6447 7075 1253 0a11 616e 6472  droidGpu.S..andr
-00008b20: 6f69 645f 7379 7375 695f 6375 6a18 1b20  oid_sysui_cuj.. 
-00008b30: 0128 0b32 272e 7065 7266 6574 746f 2e70  .(.2'.perfetto.p
-00008b40: 726f 746f 732e 416e 6472 6f69 6453 7973  rotos.AndroidSys
-00008b50: 5569 4375 6a4d 6574 7269 6373 520f 616e  UiCujMetricsR.an
-00008b60: 6472 6f69 6453 7973 7569 4375 6a12 4f0a  droidSysuiCuj.O.
-00008b70: 1061 6e64 726f 6964 5f6a 616e 6b5f 6375  .android_jank_cu
-00008b80: 6a18 3020 0128 0b32 252e 7065 7266 6574  j.0 .(.2%.perfet
-00008b90: 746f 2e70 726f 746f 732e 416e 6472 6f69  to.protos.Androi
-00008ba0: 644a 616e 6b43 756a 4d65 7472 6963 520e  dJankCujMetricR.
-00008bb0: 616e 6472 6f69 644a 616e 6b43 756a 1258  androidJankCuj.X
-00008bc0: 0a12 616e 6472 6f69 645f 6877 636f 6d70  ..android_hwcomp
-00008bd0: 6f73 6572 181c 2001 280b 3229 2e70 6572  oser.. .(.2).per
-00008be0: 6665 7474 6f2e 7072 6f74 6f73 2e41 6e64  fetto.protos.And
-00008bf0: 726f 6964 4877 636f 6d70 6f73 6572 4d65  roidHwcomposerMe
-00008c00: 7472 6963 7352 1161 6e64 726f 6964 4877  tricsR.androidHw
-00008c10: 636f 6d70 6f73 6572 122d 0a03 6732 6418  composer.-..g2d.
-00008c20: 1e20 0128 0b32 1b2e 7065 7266 6574 746f  . .(.2..perfetto
-00008c30: 2e70 726f 746f 732e 4732 644d 6574 7269  .protos.G2dMetri
-00008c40: 6373 5203 6732 6412 4f0a 1061 6e64 726f  csR.g2d.O..andro
-00008c50: 6964 5f64 6d61 5f68 6561 7018 2020 0128  id_dma_heap.  .(
-00008c60: 0b32 252e 7065 7266 6574 746f 2e70 726f  .2%.perfetto.pro
-00008c70: 746f 732e 416e 6472 6f69 6444 6d61 4865  tos.AndroidDmaHe
-00008c80: 6170 4d65 7472 6963 520e 616e 6472 6f69  apMetricR.androi
-00008c90: 6444 6d61 4865 6170 125e 0a15 616e 6472  dDmaHeap.^..andr
-00008ca0: 6f69 645f 7472 6163 655f 7175 616c 6974  oid_trace_qualit
-00008cb0: 7918 2220 0128 0b32 2a2e 7065 7266 6574  y." .(.2*.perfet
-00008cc0: 746f 2e70 726f 746f 732e 416e 6472 6f69  to.protos.Androi
-00008cd0: 6454 7261 6365 5175 616c 6974 794d 6574  dTraceQualityMet
-00008ce0: 7269 6352 1361 6e64 726f 6964 5472 6163  ricR.androidTrac
-00008cf0: 6551 7561 6c69 7479 1245 0a0e 7072 6f66  eQuality.E..prof
-00008d00: 696c 6572 5f73 6d61 7073 1823 2001 280b  iler_smaps.# .(.
-00008d10: 321e 2e70 6572 6665 7474 6f2e 7072 6f74  2..perfetto.prot
-00008d20: 6f73 2e50 726f 6669 6c65 7253 6d61 7073  os.ProfilerSmaps
-00008d30: 520d 7072 6f66 696c 6572 536d 6170 7312  R.profilerSmaps.
-00008d40: 540a 1161 6e64 726f 6964 5f6d 756c 7469  T..android_multi
-00008d50: 7573 6572 1824 2001 280b 3227 2e70 6572  user.$ .(.2'.per
-00008d60: 6665 7474 6f2e 7072 6f74 6f73 2e41 6e64  fetto.protos.And
-00008d70: 726f 6964 4d75 6c74 6975 7365 724d 6574  roidMultiuserMet
-00008d80: 7269 6352 1061 6e64 726f 6964 4d75 6c74  ricR.androidMult
-00008d90: 6975 7365 7212 570a 1261 6e64 726f 6964  iuser.W..android
-00008da0: 5f73 696d 706c 6570 6572 6618 2520 0128  _simpleperf.% .(
-00008db0: 0b32 282e 7065 7266 6574 746f 2e70 726f  .2(.perfetto.pro
-00008dc0: 746f 732e 416e 6472 6f69 6453 696d 706c  tos.AndroidSimpl
-00008dd0: 6570 6572 664d 6574 7269 6352 1161 6e64  eperfMetricR.and
-00008de0: 726f 6964 5369 6d70 6c65 7065 7266 124b  roidSimpleperf.K
-00008df0: 0a0e 616e 6472 6f69 645f 6361 6d65 7261  ..android_camera
-00008e00: 1826 2001 280b 3224 2e70 6572 6665 7474  .& .(.2$.perfett
-00008e10: 6f2e 7072 6f74 6f73 2e41 6e64 726f 6964  o.protos.Android
-00008e20: 4361 6d65 7261 4d65 7472 6963 520d 616e  CameraMetricR.an
-00008e30: 6472 6f69 6443 616d 6572 6112 450a 0c61  droidCamera.E..a
-00008e40: 6e64 726f 6964 5f64 7666 7318 2720 0128  ndroid_dvfs.' .(
-00008e50: 0b32 222e 7065 7266 6574 746f 2e70 726f  .2".perfetto.pro
-00008e60: 746f 732e 416e 6472 6f69 6444 7666 734d  tos.AndroidDvfsM
-00008e70: 6574 7269 6352 0b61 6e64 726f 6964 4476  etricR.androidDv
-00008e80: 6673 124e 0a0f 616e 6472 6f69 645f 6e65  fs.N..android_ne
-00008e90: 7470 6572 6618 2820 0128 0b32 252e 7065  tperf.( .(.2%.pe
-00008ea0: 7266 6574 746f 2e70 726f 746f 732e 416e  rfetto.protos.An
-00008eb0: 6472 6f69 644e 6574 776f 726b 4d65 7472  droidNetworkMetr
-00008ec0: 6963 520e 616e 6472 6f69 644e 6574 7065  icR.androidNetpe
-00008ed0: 7266 1262 0a14 616e 6472 6f69 645f 6361  rf.b..android_ca
-00008ee0: 6d65 7261 5f75 6e61 6767 1829 2001 280b  mera_unagg.) .(.
-00008ef0: 3230 2e70 6572 6665 7474 6f2e 7072 6f74  20.perfetto.prot
-00008f00: 6f73 2e41 6e64 726f 6964 4361 6d65 7261  os.AndroidCamera
-00008f10: 556e 6167 6772 6567 6174 6564 4d65 7472  UnaggregatedMetr
-00008f20: 6963 5212 616e 6472 6f69 6443 616d 6572  icR.androidCamer
-00008f30: 6155 6e61 6767 1255 0a12 616e 6472 6f69  aUnagg.U..androi
-00008f40: 645f 7274 5f72 756e 7469 6d65 182a 2001  d_rt_runtime.* .
-00008f50: 280b 3227 2e70 6572 6665 7474 6f2e 7072  (.2'.perfetto.pr
-00008f60: 6f74 6f73 2e41 6e64 726f 6964 5274 5275  otos.AndroidRtRu
-00008f70: 6e74 696d 654d 6574 7269 6352 1061 6e64  ntimeMetricR.and
-00008f80: 726f 6964 5274 5275 6e74 696d 6512 580a  roidRtRuntime.X.
-00008f90: 1361 6e64 726f 6964 5f69 7271 5f72 756e  .android_irq_run
-00008fa0: 7469 6d65 182b 2001 280b 3228 2e70 6572  time.+ .(.2(.per
-00008fb0: 6665 7474 6f2e 7072 6f74 6f73 2e41 6e64  fetto.protos.And
-00008fc0: 726f 6964 4972 7152 756e 7469 6d65 4d65  roidIrqRuntimeMe
-00008fd0: 7472 6963 5211 616e 6472 6f69 6449 7271  tricR.androidIrq
-00008fe0: 5275 6e74 696d 6512 640a 1961 6e64 726f  Runtime.d..andro
-00008ff0: 6964 5f74 7275 7374 795f 776f 726b 7175  id_trusty_workqu
-00009000: 6575 6573 182c 2001 280b 3228 2e70 6572  eues., .(.2(.per
-00009010: 6665 7474 6f2e 7072 6f74 6f73 2e41 6e64  fetto.protos.And
-00009020: 726f 6964 5472 7573 7479 576f 726b 7175  roidTrustyWorkqu
-00009030: 6575 6573 5217 616e 6472 6f69 6454 7275  euesR.androidTru
-00009040: 7374 7957 6f72 6b71 7565 7565 7312 5b0a  styWorkqueues.[.
-00009050: 1461 6e64 726f 6964 5f6f 7468 6572 5f74  .android_other_t
-00009060: 7261 6365 7318 2d20 0128 0b32 292e 7065  races.- .(.2).pe
-00009070: 7266 6574 746f 2e70 726f 746f 732e 416e  rfetto.protos.An
-00009080: 6472 6f69 644f 7468 6572 5472 6163 6573  droidOtherTraces
-00009090: 4d65 7472 6963 5212 616e 6472 6f69 644f  MetricR.androidO
-000090a0: 7468 6572 5472 6163 6573 124b 0a0e 616e  therTraces.K..an
-000090b0: 6472 6f69 645f 6269 6e64 6572 182e 2001  droid_binder.. .
-000090c0: 280b 3224 2e70 6572 6665 7474 6f2e 7072  (.2$.perfetto.pr
-000090d0: 6f74 6f73 2e41 6e64 726f 6964 4269 6e64  otos.AndroidBind
-000090e0: 6572 4d65 7472 6963 520d 616e 6472 6f69  erMetricR.androi
-000090f0: 6442 696e 6465 7212 6e0a 1d61 6e64 726f  dBinder.n..andro
-00009100: 6964 5f66 7261 6d65 5f74 696d 656c 696e  id_frame_timelin
-00009110: 655f 6d65 7472 6963 182f 2001 280b 322b  e_metric./ .(.2+
-00009120: 2e70 6572 6665 7474 6f2e 7072 6f74 6f73  .perfetto.protos
-00009130: 2e41 6e64 726f 6964 4672 616d 6554 696d  .AndroidFrameTim
-00009140: 656c 696e 654d 6574 7269 6352 1a61 6e64  elineMetricR.and
-00009150: 726f 6964 4672 616d 6554 696d 656c 696e  roidFrameTimelin
-00009160: 654d 6574 7269 632a 0608 c203 10f4 032a  eMetric*.......*
-00009170: 0608 f403 10e9 072a 0608 e907 10d1 0f4a  .......*.......J
-00009180: 0408 0410 054a 0408 0a10 0b4a 0408 0d10  .....J.....J....
-00009190: 0e4a 0408 0e10 0f4a 0408 1010 114a 0408  .J.....J.....J..
-000091a0: 1310 144a 0408 1810 194a 0408 1d10 1e    ...J.....J.....
+00000130: 5569 6412 100a 0370 6964 1809 2001 2803  Uid....pid.. .(.
+00000140: 5203 7069 641a 760a 0750 6163 6b61 6765  R.pid.v..Package
+00000150: 1221 0a0c 7061 636b 6167 655f 6e61 6d65  .!..package_name
+00000160: 1801 2001 2809 520b 7061 636b 6167 654e  .. .(.R.packageN
+00000170: 616d 6512 280a 1061 706b 5f76 6572 7369  ame.(..apk_versi
+00000180: 6f6e 5f63 6f64 6518 0220 0128 0352 0e61  on_code.. .(.R.a
+00000190: 706b 5665 7273 696f 6e43 6f64 6512 1e0a  pkVersionCode...
+000001a0: 0a64 6562 7567 6761 626c 6518 0320 0128  .debuggable.. .(
+000001b0: 0852 0a64 6562 7567 6761 626c 654a 0408  .R.debuggableJ..
+000001c0: 0310 044a 0408 0410 054a 0408 0510 064a  ...J.....J.....J
+000001d0: 0408 0610 070a a608 0a43 7072 6f74 6f73  .........Cprotos
+000001e0: 2f70 6572 6665 7474 6f2f 6d65 7472 6963  /perfetto/metric
+000001f0: 732f 616e 6472 6f69 642f 616e 6472 6f69  s/android/androi
+00000200: 645f 6672 616d 655f 7469 6d65 6c69 6e65  d_frame_timeline
+00000210: 5f6d 6574 7269 632e 7072 6f74 6f12 0f70  _metric.proto..p
+00000220: 6572 6665 7474 6f2e 7072 6f74 6f73 1a36  erfetto.protos.6
+00000230: 7072 6f74 6f73 2f70 6572 6665 7474 6f2f  protos/perfetto/
+00000240: 6d65 7472 6963 732f 616e 6472 6f69 642f  metrics/android/
+00000250: 7072 6f63 6573 735f 6d65 7461 6461 7461  process_metadata
+00000260: 2e70 726f 746f 2295 070a 1a41 6e64 726f  .proto"....Andro
+00000270: 6964 4672 616d 6554 696d 656c 696e 654d  idFrameTimelineM
+00000280: 6574 7269 6312 210a 0c74 6f74 616c 5f66  etric.!..total_f
+00000290: 7261 6d65 7318 0420 0128 0352 0b74 6f74  rames.. .(.R.tot
+000002a0: 616c 4672 616d 6573 122a 0a11 6d69 7373  alFrames.*..miss
+000002b0: 6564 5f61 7070 5f66 7261 6d65 7318 0520  ed_app_frames.. 
+000002c0: 0128 0352 0f6d 6973 7365 6441 7070 4672  .(.R.missedAppFr
+000002d0: 616d 6573 1225 0a0e 6472 6f70 7065 645f  ames.%..dropped_
+000002e0: 6672 616d 6573 1806 2001 2803 520d 6472  frames.. .(.R.dr
+000002f0: 6f70 7065 6446 7261 6d65 7312 560a 0770  oppedFrames.V..p
+00000300: 726f 6365 7373 1802 2003 280b 323c 2e70  rocess.. .(.2<.p
+00000310: 6572 6665 7474 6f2e 7072 6f74 6f73 2e41  erfetto.protos.A
+00000320: 6e64 726f 6964 4672 616d 6554 696d 656c  ndroidFrameTimel
+00000330: 696e 654d 6574 7269 632e 5072 6f63 6573  ineMetric.Proces
+00000340: 7342 7265 616b 646f 776e 5207 7072 6f63  sBreakdownR.proc
+00000350: 6573 731a a205 0a10 5072 6f63 6573 7342  ess.....ProcessB
+00000360: 7265 616b 646f 776e 1241 0a07 7072 6f63  reakdown.A..proc
+00000370: 6573 7318 0320 0128 0b32 272e 7065 7266  ess.. .(.2'.perf
+00000380: 6574 746f 2e70 726f 746f 732e 416e 6472  etto.protos.Andr
+00000390: 6f69 6450 726f 6365 7373 4d65 7461 6461  oidProcessMetada
+000003a0: 7461 5207 7072 6f63 6573 7312 210a 0c74  taR.process.!..t
+000003b0: 6f74 616c 5f66 7261 6d65 7318 0420 0128  otal_frames.. .(
+000003c0: 0352 0b74 6f74 616c 4672 616d 6573 1223  .R.totalFrames.#
+000003d0: 0a0d 6d69 7373 6564 5f66 7261 6d65 7318  ..missed_frames.
+000003e0: 0520 0128 0352 0c6d 6973 7365 6446 7261  . .(.R.missedFra
+000003f0: 6d65 7312 2a0a 116d 6973 7365 645f 6170  mes.*..missed_ap
+00000400: 705f 6672 616d 6573 1806 2001 2803 520f  p_frames.. .(.R.
+00000410: 6d69 7373 6564 4170 7046 7261 6d65 7312  missedAppFrames.
+00000420: 280a 106d 6973 7365 645f 7366 5f66 7261  (..missed_sf_fra
+00000430: 6d65 7318 0720 0128 0352 0e6d 6973 7365  mes.. .(.R.misse
+00000440: 6453 6646 7261 6d65 7312 220a 0d66 7261  dSfFrames."..fra
+00000450: 6d65 5f64 7572 5f6d 6178 1808 2001 2803  me_dur_max.. .(.
+00000460: 520b 6672 616d 6544 7572 4d61 7812 220a  R.frameDurMax.".
+00000470: 0d66 7261 6d65 5f64 7572 5f61 7667 1809  .frame_dur_avg..
+00000480: 2001 2803 520b 6672 616d 6544 7572 4176   .(.R.frameDurAv
+00000490: 6712 220a 0d66 7261 6d65 5f64 7572 5f70  g."..frame_dur_p
+000004a0: 3530 180a 2001 2803 520b 6672 616d 6544  50.. .(.R.frameD
+000004b0: 7572 5035 3012 220a 0d66 7261 6d65 5f64  urP50."..frame_d
+000004c0: 7572 5f70 3930 180b 2001 2803 520b 6672  ur_p90.. .(.R.fr
+000004d0: 616d 6544 7572 5039 3012 220a 0d66 7261  ameDurP90."..fra
+000004e0: 6d65 5f64 7572 5f70 3935 180c 2001 2803  me_dur_p95.. .(.
+000004f0: 520b 6672 616d 6544 7572 5039 3512 220a  R.frameDurP95.".
+00000500: 0d66 7261 6d65 5f64 7572 5f70 3939 180d  .frame_dur_p99..
+00000510: 2001 2803 520b 6672 616d 6544 7572 5039   .(.R.frameDurP9
+00000520: 3912 270a 1066 7261 6d65 5f64 7572 5f6d  9.'..frame_dur_m
+00000530: 735f 7035 3018 0e20 0128 0152 0d66 7261  s_p50.. .(.R.fra
+00000540: 6d65 4475 724d 7350 3530 1227 0a10 6672  meDurMsP50.'..fr
+00000550: 616d 655f 6475 725f 6d73 5f70 3930 180f  ame_dur_ms_p90..
+00000560: 2001 2801 520d 6672 616d 6544 7572 4d73   .(.R.frameDurMs
+00000570: 5039 3012 270a 1066 7261 6d65 5f64 7572  P90.'..frame_dur
+00000580: 5f6d 735f 7039 3518 1020 0128 0152 0d66  _ms_p95.. .(.R.f
+00000590: 7261 6d65 4475 724d 7350 3935 1227 0a10  rameDurMsP95.'..
+000005a0: 6672 616d 655f 6475 725f 6d73 5f70 3939  frame_dur_ms_p99
+000005b0: 1811 2001 2801 520d 6672 616d 6544 7572  .. .(.R.frameDur
+000005c0: 4d73 5039 3912 250a 0e64 726f 7070 6564  MsP99.%..dropped
+000005d0: 5f66 7261 6d65 7318 1220 0128 0352 0d64  _frames.. .(.R.d
+000005e0: 726f 7070 6564 4672 616d 6573 4a04 0801  roppedFramesJ...
+000005f0: 1002 4a04 0802 1003 4a04 0801 1002 0aa4  ..J.....J.......
+00000600: 080a 3170 726f 746f 732f 7065 7266 6574  ..1protos/perfet
+00000610: 746f 2f6d 6574 7269 6373 2f61 6e64 726f  to/metrics/andro
+00000620: 6964 2f62 6174 745f 6d65 7472 6963 2e70  id/batt_metric.p
+00000630: 726f 746f 120f 7065 7266 6574 746f 2e70  roto..perfetto.p
+00000640: 726f 746f 7322 dd07 0a14 416e 6472 6f69  rotos"....Androi
+00000650: 6442 6174 7465 7279 4d65 7472 6963 1260  dBatteryMetric.`
+00000660: 0a10 6261 7474 6572 795f 636f 756e 7465  ..battery_counte
+00000670: 7273 1801 2003 280b 3235 2e70 6572 6665  rs.. .(.25.perfe
+00000680: 7474 6f2e 7072 6f74 6f73 2e41 6e64 726f  tto.protos.Andro
+00000690: 6964 4261 7474 6572 794d 6574 7269 632e  idBatteryMetric.
+000006a0: 4261 7474 6572 7943 6f75 6e74 6572 7352  BatteryCountersR
+000006b0: 0f62 6174 7465 7279 436f 756e 7465 7273  .batteryCounters
+000006c0: 1266 0a12 6261 7474 6572 795f 6167 6772  .f..battery_aggr
+000006d0: 6567 6174 6573 1802 2001 280b 3237 2e70  egates.. .(.27.p
+000006e0: 6572 6665 7474 6f2e 7072 6f74 6f73 2e41  erfetto.protos.A
+000006f0: 6e64 726f 6964 4261 7474 6572 794d 6574  ndroidBatteryMet
+00000700: 7269 632e 4261 7474 6572 7941 6767 7265  ric.BatteryAggre
+00000710: 6761 7465 7352 1162 6174 7465 7279 4167  gatesR.batteryAg
+00000720: 6772 6567 6174 6573 125a 0a0e 7375 7370  gregates.Z..susp
+00000730: 656e 645f 7065 7269 6f64 1803 2003 280b  end_period.. .(.
+00000740: 3233 2e70 6572 6665 7474 6f2e 7072 6f74  23.perfetto.prot
+00000750: 6f73 2e41 6e64 726f 6964 4261 7474 6572  os.AndroidBatter
+00000760: 794d 6574 7269 632e 5375 7370 656e 6450  yMetric.SuspendP
+00000770: 6572 696f 6452 0d73 7573 7065 6e64 5065  eriodR.suspendPe
+00000780: 7269 6f64 1ad2 010a 0f42 6174 7465 7279  riod.....Battery
+00000790: 436f 756e 7465 7273 1221 0a0c 7469 6d65  Counters.!..time
+000007a0: 7374 616d 705f 6e73 1801 2001 2803 520b  stamp_ns.. .(.R.
+000007b0: 7469 6d65 7374 616d 704e 7312 2c0a 1263  timestampNs.,..c
+000007c0: 6861 7267 655f 636f 756e 7465 725f 7561  harge_counter_ua
+000007d0: 6818 0220 0128 0152 1063 6861 7267 6543  h.. .(.R.chargeC
+000007e0: 6f75 6e74 6572 5561 6812 290a 1063 6170  ounterUah.)..cap
+000007f0: 6163 6974 795f 7065 7263 656e 7418 0320  acity_percent.. 
+00000800: 0128 0252 0f63 6170 6163 6974 7950 6572  .(.R.capacityPer
+00000810: 6365 6e74 121d 0a0a 6375 7272 656e 745f  cent....current_
+00000820: 7561 1804 2001 2801 5209 6375 7272 656e  ua.. .(.R.curren
+00000830: 7455 6112 240a 0e63 7572 7265 6e74 5f61  tUa.$..current_a
+00000840: 7667 5f75 6118 0520 0128 0152 0c63 7572  vg_ua.. .(.R.cur
+00000850: 7265 6e74 4176 6755 611a f402 0a11 4261  rentAvgUa.....Ba
+00000860: 7474 6572 7941 6767 7265 6761 7465 7312  tteryAggregates.
+00000870: 2d0a 1374 6f74 616c 5f73 6372 6565 6e5f  -..total_screen_
+00000880: 6f66 665f 6e73 1801 2001 2803 5210 746f  off_ns.. .(.R.to
+00000890: 7461 6c53 6372 6565 6e4f 6666 4e73 122b  talScreenOffNs.+
+000008a0: 0a12 746f 7461 6c5f 7363 7265 656e 5f6f  ..total_screen_o
+000008b0: 6e5f 6e73 1802 2001 2803 520f 746f 7461  n_ns.. .(.R.tota
+000008c0: 6c53 6372 6565 6e4f 6e4e 7312 2f0a 1474  lScreenOnNs./..t
+000008d0: 6f74 616c 5f73 6372 6565 6e5f 646f 7a65  otal_screen_doze
+000008e0: 5f6e 7318 0320 0128 0352 1174 6f74 616c  _ns.. .(.R.total
+000008f0: 5363 7265 656e 446f 7a65 4e73 122a 0a11  ScreenDozeNs.*..
+00000900: 746f 7461 6c5f 7761 6b65 6c6f 636b 5f6e  total_wakelock_n
+00000910: 7318 0420 0128 0352 0f74 6f74 616c 5761  s.. .(.R.totalWa
+00000920: 6b65 6c6f 636b 4e73 1219 0a08 736c 6565  kelockNs....slee
+00000930: 705f 6e73 1805 2001 2803 5207 736c 6565  p_ns.. .(.R.slee
+00000940: 704e 7312 2d0a 1373 6c65 6570 5f73 6372  pNs.-..sleep_scr
+00000950: 6565 6e5f 6f66 665f 6e73 1806 2001 2803  een_off_ns.. .(.
+00000960: 5210 736c 6565 7053 6372 6565 6e4f 6666  R.sleepScreenOff
+00000970: 4e73 122b 0a12 736c 6565 705f 7363 7265  Ns.+..sleep_scre
+00000980: 656e 5f6f 6e5f 6e73 1807 2001 2803 520f  en_on_ns.. .(.R.
+00000990: 736c 6565 7053 6372 6565 6e4f 6e4e 7312  sleepScreenOnNs.
+000009a0: 2f0a 1473 6c65 6570 5f73 6372 6565 6e5f  /..sleep_screen_
+000009b0: 646f 7a65 5f6e 7318 0820 0128 0352 1173  doze_ns.. .(.R.s
+000009c0: 6c65 6570 5363 7265 656e 446f 7a65 4e73  leepScreenDozeNs
+000009d0: 1a53 0a0d 5375 7370 656e 6450 6572 696f  .S..SuspendPerio
+000009e0: 6412 210a 0c74 696d 6573 7461 6d70 5f6e  d.!..timestamp_n
+000009f0: 7318 0120 0128 0352 0b74 696d 6573 7461  s.. .(.R.timesta
+00000a00: 6d70 4e73 121f 0a0b 6475 7261 7469 6f6e  mpNs....duration
+00000a10: 5f6e 7318 0220 0128 0352 0a64 7572 6174  _ns.. .(.R.durat
+00000a20: 696f 6e4e 730a 8405 0a47 7072 6f74 6f73  ionNs....Gprotos
+00000a30: 2f70 6572 6665 7474 6f2f 6d65 7472 6963  /perfetto/metric
+00000a40: 732f 616e 6472 6f69 642f 616e 6472 6f69  s/android/androi
+00000a50: 645f 626c 6f63 6b69 6e67 5f63 616c 6c73  d_blocking_calls
+00000a60: 5f63 756a 5f6d 6574 7269 632e 7072 6f74  _cuj_metric.prot
+00000a70: 6f12 0f70 6572 6665 7474 6f2e 7072 6f74  o..perfetto.prot
+00000a80: 6f73 1a36 7072 6f74 6f73 2f70 6572 6665  os.6protos/perfe
+00000a90: 7474 6f2f 6d65 7472 6963 732f 616e 6472  tto/metrics/andr
+00000aa0: 6f69 642f 7072 6f63 6573 735f 6d65 7461  oid/process_meta
+00000ab0: 6461 7461 2e70 726f 746f 22ef 030a 1d41  data.proto"....A
+00000ac0: 6e64 726f 6964 426c 6f63 6b69 6e67 4361  ndroidBlockingCa
+00000ad0: 6c6c 7343 756a 4d65 7472 6963 1244 0a03  llsCujMetric.D..
+00000ae0: 6375 6a18 0120 0328 0b32 322e 7065 7266  cuj.. .(.22.perf
+00000af0: 6574 746f 2e70 726f 746f 732e 416e 6472  etto.protos.Andr
+00000b00: 6f69 6442 6c6f 636b 696e 6743 616c 6c73  oidBlockingCalls
+00000b10: 4375 6a4d 6574 7269 632e 4375 6a52 0363  CujMetric.CujR.c
+00000b20: 756a 1af2 010a 0343 756a 120e 0a02 6964  uj.....Cuj....id
+00000b30: 1801 2001 2805 5202 6964 1212 0a04 6e61  .. .(.R.id....na
+00000b40: 6d65 1802 2001 2809 5204 6e61 6d65 1241  me.. .(.R.name.A
+00000b50: 0a07 7072 6f63 6573 7318 0320 0128 0b32  ..process.. .(.2
+00000b60: 272e 7065 7266 6574 746f 2e70 726f 746f  '.perfetto.proto
+00000b70: 732e 416e 6472 6f69 6450 726f 6365 7373  s.AndroidProcess
+00000b80: 4d65 7461 6461 7461 5207 7072 6f63 6573  MetadataR.proces
+00000b90: 7312 0e0a 0274 7318 0420 0128 0352 0274  s....ts.. .(.R.t
+00000ba0: 7312 100a 0364 7572 1805 2001 2803 5203  s....dur.. .(.R.
+00000bb0: 6475 7212 620a 0e62 6c6f 636b 696e 675f  dur.b..blocking_
+00000bc0: 6361 6c6c 7318 0620 0328 0b32 3b2e 7065  calls.. .(.2;.pe
+00000bd0: 7266 6574 746f 2e70 726f 746f 732e 416e  rfetto.protos.An
+00000be0: 6472 6f69 6442 6c6f 636b 696e 6743 616c  droidBlockingCal
+00000bf0: 6c73 4375 6a4d 6574 7269 632e 426c 6f63  lsCujMetric.Bloc
+00000c00: 6b69 6e67 4361 6c6c 520d 626c 6f63 6b69  kingCallR.blocki
+00000c10: 6e67 4361 6c6c 731a 9201 0a0c 426c 6f63  ngCalls.....Bloc
+00000c20: 6b69 6e67 4361 6c6c 1212 0a04 6e61 6d65  kingCall....name
+00000c30: 1801 2001 2809 5204 6e61 6d65 1210 0a03  .. .(.R.name....
+00000c40: 636e 7418 0220 0128 0352 0363 6e74 1220  cnt.. .(.R.cnt. 
+00000c50: 0a0c 746f 7461 6c5f 6475 725f 6d73 1803  ..total_dur_ms..
+00000c60: 2001 2803 520a 746f 7461 6c44 7572 4d73   .(.R.totalDurMs
+00000c70: 121c 0a0a 6d61 785f 6475 725f 6d73 1804  ....max_dur_ms..
+00000c80: 2001 2803 5208 6d61 7844 7572 4d73 121c   .(.R.maxDurMs..
+00000c90: 0a0a 6d69 6e5f 6475 725f 6d73 1805 2001  ..min_dur_ms.. .
+00000ca0: 2803 5208 6d69 6e44 7572 4d73 0ad4 080a  (.R.minDurMs....
+00000cb0: 3070 726f 746f 732f 7065 7266 6574 746f  0protos/perfetto
+00000cc0: 2f6d 6574 7269 6373 2f61 6e64 726f 6964  /metrics/android
+00000cd0: 2f63 7075 5f6d 6574 7269 632e 7072 6f74  /cpu_metric.prot
+00000ce0: 6f12 0f70 6572 6665 7474 6f2e 7072 6f74  o..perfetto.prot
+00000cf0: 6f73 228e 080a 1041 6e64 726f 6964 4370  os"....AndroidCp
+00000d00: 754d 6574 7269 6312 4c0a 0c70 726f 6365  uMetric.L..proce
+00000d10: 7373 5f69 6e66 6f18 0120 0328 0b32 292e  ss_info.. .(.2).
+00000d20: 7065 7266 6574 746f 2e70 726f 746f 732e  perfetto.protos.
+00000d30: 416e 6472 6f69 6443 7075 4d65 7472 6963  AndroidCpuMetric
+00000d40: 2e50 726f 6365 7373 520b 7072 6f63 6573  .ProcessR.proces
+00000d50: 7349 6e66 6f1a a801 0a07 4d65 7472 6963  sInfo.....Metric
+00000d60: 7312 180a 076d 6379 636c 6573 1801 2001  s....mcycles.. .
+00000d70: 2803 5207 6d63 7963 6c65 7312 1d0a 0a72  (.R.mcycles....r
+00000d80: 756e 7469 6d65 5f6e 7318 0220 0128 0352  untime_ns.. .(.R
+00000d90: 0972 756e 7469 6d65 4e73 1220 0a0c 6d69  .runtimeNs. ..mi
+00000da0: 6e5f 6672 6571 5f6b 687a 1803 2001 2803  n_freq_khz.. .(.
+00000db0: 520a 6d69 6e46 7265 714b 687a 1220 0a0c  R.minFreqKhz. ..
+00000dc0: 6d61 785f 6672 6571 5f6b 687a 1804 2001  max_freq_khz.. .
+00000dd0: 2803 520a 6d61 7846 7265 714b 687a 1220  (.R.maxFreqKhz. 
+00000de0: 0a0c 6176 675f 6672 6571 5f6b 687a 1805  ..avg_freq_khz..
+00000df0: 2001 2803 520a 6176 6746 7265 714b 687a   .(.R.avgFreqKhz
+00000e00: 1a65 0a08 436f 7265 4461 7461 120e 0a02  .e..CoreData....
+00000e10: 6964 1801 2001 280d 5202 6964 1243 0a07  id.. .(.R.id.C..
+00000e20: 6d65 7472 6963 7318 0620 0128 0b32 292e  metrics.. .(.2).
+00000e30: 7065 7266 6574 746f 2e70 726f 746f 732e  perfetto.protos.
+00000e40: 416e 6472 6f69 6443 7075 4d65 7472 6963  AndroidCpuMetric
+00000e50: 2e4d 6574 7269 6373 5207 6d65 7472 6963  .MetricsR.metric
+00000e60: 734a 0408 0210 061a 670a 0c43 6f72 6554  sJ......g..CoreT
+00000e70: 7970 6544 6174 6112 120a 0474 7970 6518  ypeData....type.
+00000e80: 0120 0128 0952 0474 7970 6512 430a 076d  . .(.R.type.C..m
+00000e90: 6574 7269 6373 1802 2001 280b 3229 2e70  etrics.. .(.2).p
+00000ea0: 6572 6665 7474 6f2e 7072 6f74 6f73 2e41  erfetto.protos.A
+00000eb0: 6e64 726f 6964 4370 754d 6574 7269 632e  ndroidCpuMetric.
+00000ec0: 4d65 7472 6963 7352 076d 6574 7269 6373  MetricsR.metrics
+00000ed0: 1af4 010a 0654 6872 6561 6412 120a 046e  .....Thread....n
+00000ee0: 616d 6518 0120 0128 0952 046e 616d 6512  ame.. .(.R.name.
+00000ef0: 430a 076d 6574 7269 6373 1804 2001 280b  C..metrics.. .(.
+00000f00: 3229 2e70 6572 6665 7474 6f2e 7072 6f74  2).perfetto.prot
+00000f10: 6f73 2e41 6e64 726f 6964 4370 754d 6574  os.AndroidCpuMet
+00000f20: 7269 632e 4d65 7472 6963 7352 076d 6574  ric.MetricsR.met
+00000f30: 7269 6373 123e 0a04 636f 7265 1802 2003  rics.>..core.. .
+00000f40: 280b 322a 2e70 6572 6665 7474 6f2e 7072  (.2*.perfetto.pr
+00000f50: 6f74 6f73 2e41 6e64 726f 6964 4370 754d  otos.AndroidCpuM
+00000f60: 6574 7269 632e 436f 7265 4461 7461 5204  etric.CoreDataR.
+00000f70: 636f 7265 124b 0a09 636f 7265 5f74 7970  core.K..core_typ
+00000f80: 6518 0520 0328 0b32 2e2e 7065 7266 6574  e.. .(.2..perfet
+00000f90: 746f 2e70 726f 746f 732e 416e 6472 6f69  to.protos.Androi
+00000fa0: 6443 7075 4d65 7472 6963 2e43 6f72 6554  dCpuMetric.CoreT
+00000fb0: 7970 6544 6174 6152 0863 6f72 6554 7970  ypeDataR.coreTyp
+00000fc0: 654a 0408 0310 041a b902 0a07 5072 6f63  eJ..........Proc
+00000fd0: 6573 7312 120a 046e 616d 6518 0120 0128  ess....name.. .(
+00000fe0: 0952 046e 616d 6512 430a 076d 6574 7269  .R.name.C..metri
+00000ff0: 6373 1804 2001 280b 3229 2e70 6572 6665  cs.. .(.2).perfe
+00001000: 7474 6f2e 7072 6f74 6f73 2e41 6e64 726f  tto.protos.Andro
+00001010: 6964 4370 754d 6574 7269 632e 4d65 7472  idCpuMetric.Metr
+00001020: 6963 7352 076d 6574 7269 6373 1242 0a07  icsR.metrics.B..
+00001030: 7468 7265 6164 7318 0620 0328 0b32 282e  threads.. .(.2(.
+00001040: 7065 7266 6574 746f 2e70 726f 746f 732e  perfetto.protos.
+00001050: 416e 6472 6f69 6443 7075 4d65 7472 6963  AndroidCpuMetric
+00001060: 2e54 6872 6561 6452 0774 6872 6561 6473  .ThreadR.threads
+00001070: 123e 0a04 636f 7265 1807 2003 280b 322a  .>..core.. .(.2*
+00001080: 2e70 6572 6665 7474 6f2e 7072 6f74 6f73  .perfetto.protos
+00001090: 2e41 6e64 726f 6964 4370 754d 6574 7269  .AndroidCpuMetri
+000010a0: 632e 436f 7265 4461 7461 5204 636f 7265  c.CoreDataR.core
+000010b0: 124b 0a09 636f 7265 5f74 7970 6518 0520  .K..core_type.. 
+000010c0: 0328 0b32 2e2e 7065 7266 6574 746f 2e70  .(.2..perfetto.p
+000010d0: 726f 746f 732e 416e 6472 6f69 6443 7075  rotos.AndroidCpu
+000010e0: 4d65 7472 6963 2e43 6f72 6554 7970 6544  Metric.CoreTypeD
+000010f0: 6174 6152 0863 6f72 6554 7970 654a 0408  ataR.coreTypeJ..
+00001100: 0310 040a f201 0a33 7072 6f74 6f73 2f70  .......3protos/p
+00001110: 6572 6665 7474 6f2f 6d65 7472 6963 732f  erfetto/metrics/
+00001120: 616e 6472 6f69 642f 6361 6d65 7261 5f6d  android/camera_m
+00001130: 6574 7269 632e 7072 6f74 6f12 0f70 6572  etric.proto..per
+00001140: 6665 7474 6f2e 7072 6f74 6f73 22a9 010a  fetto.protos"...
+00001150: 1341 6e64 726f 6964 4361 6d65 7261 4d65  .AndroidCameraMe
+00001160: 7472 6963 1251 0a0e 6763 5f72 7373 5f61  tric.Q..gc_rss_a
+00001170: 6e64 5f64 6d61 1801 2001 280b 322c 2e70  nd_dma.. .(.2,.p
+00001180: 6572 6665 7474 6f2e 7072 6f74 6f73 2e41  erfetto.protos.A
+00001190: 6e64 726f 6964 4361 6d65 7261 4d65 7472  ndroidCameraMetr
+000011a0: 6963 2e43 6f75 6e74 6572 520b 6763 5273  ic.CounterR.gcRs
+000011b0: 7341 6e64 446d 611a 3f0a 0743 6f75 6e74  sAndDma.?..Count
+000011c0: 6572 1210 0a03 6d69 6e18 0120 0128 0152  er....min.. .(.R
+000011d0: 036d 696e 1210 0a03 6d61 7818 0220 0128  .min....max.. .(
+000011e0: 0152 036d 6178 1210 0a03 6176 6718 0320  .R.max....avg.. 
+000011f0: 0128 0152 0361 7667 0afc 010a 3970 726f  .(.R.avg....9pro
+00001200: 746f 732f 7065 7266 6574 746f 2f6d 6574  tos/perfetto/met
+00001210: 7269 6373 2f61 6e64 726f 6964 2f63 616d  rics/android/cam
+00001220: 6572 615f 756e 6167 675f 6d65 7472 6963  era_unagg_metric
+00001230: 2e70 726f 746f 120f 7065 7266 6574 746f  .proto..perfetto
+00001240: 2e70 726f 746f 7322 ad01 0a1f 416e 6472  .protos"....Andr
+00001250: 6f69 6443 616d 6572 6155 6e61 6767 7265  oidCameraUnaggre
+00001260: 6761 7465 644d 6574 7269 6312 5b0a 0e67  gatedMetric.[..g
+00001270: 635f 7273 735f 616e 645f 646d 6118 0120  c_rss_and_dma.. 
+00001280: 0328 0b32 362e 7065 7266 6574 746f 2e70  .(.26.perfetto.p
+00001290: 726f 746f 732e 416e 6472 6f69 6443 616d  rotos.AndroidCam
+000012a0: 6572 6155 6e61 6767 7265 6761 7465 644d  eraUnaggregatedM
+000012b0: 6574 7269 632e 5661 6c75 6552 0b67 6352  etric.ValueR.gcR
+000012c0: 7373 416e 6444 6d61 1a2d 0a05 5661 6c75  ssAndDma.-..Valu
+000012d0: 6512 0e0a 0274 7318 0120 0128 0352 0274  e....ts.. .(.R.t
+000012e0: 7312 140a 0576 616c 7565 1802 2001 2801  s....value.. .(.
+000012f0: 5205 7661 6c75 650a ed05 0a35 7072 6f74  R.value....5prot
+00001300: 6f73 2f70 6572 6665 7474 6f2f 6d65 7472  os/perfetto/metr
+00001310: 6963 732f 616e 6472 6f69 642f 6469 7370  ics/android/disp
+00001320: 6c61 795f 6d65 7472 6963 732e 7072 6f74  lay_metrics.prot
+00001330: 6f12 0f70 6572 6665 7474 6f2e 7072 6f74  o..perfetto.prot
+00001340: 6f73 22a2 050a 1541 6e64 726f 6964 4469  os"....AndroidDi
+00001350: 7370 6c61 794d 6574 7269 6373 1234 0a16  splayMetrics.4..
+00001360: 746f 7461 6c5f 6475 706c 6963 6174 655f  total_duplicate_
+00001370: 6672 616d 6573 1801 2001 280d 5214 746f  frames.. .(.R.to
+00001380: 7461 6c44 7570 6c69 6361 7465 4672 616d  talDuplicateFram
+00001390: 6573 1236 0a17 6475 706c 6963 6174 655f  es.6..duplicate_
+000013a0: 6672 616d 6573 5f6c 6f67 6765 6418 0220  frames_logged.. 
+000013b0: 0128 0d52 1564 7570 6c69 6361 7465 4672  .(.R.duplicateFr
+000013c0: 616d 6573 4c6f 6767 6564 1237 0a18 746f  amesLogged.7..to
+000013d0: 7461 6c5f 6470 755f 756e 6465 7272 756e  tal_dpu_underrun
+000013e0: 5f63 6f75 6e74 1803 2001 280d 5215 746f  _count.. .(.R.to
+000013f0: 7461 6c44 7075 556e 6465 7272 756e 436f  talDpuUnderrunCo
+00001400: 756e 7412 320a 1572 6566 7265 7368 5f72  unt.2..refresh_r
+00001410: 6174 655f 7377 6974 6368 6573 1804 2001  ate_switches.. .
+00001420: 280d 5213 7265 6672 6573 6852 6174 6553  (.R.refreshRateS
+00001430: 7769 7463 6865 7312 640a 1272 6566 7265  witches.d..refre
+00001440: 7368 5f72 6174 655f 7374 6174 7318 0520  sh_rate_stats.. 
+00001450: 0328 0b32 362e 7065 7266 6574 746f 2e70  .(.26.perfetto.p
+00001460: 726f 746f 732e 416e 6472 6f69 6444 6973  rotos.AndroidDis
+00001470: 706c 6179 4d65 7472 6963 732e 5265 6672  playMetrics.Refr
+00001480: 6573 6852 6174 6553 7461 7452 1072 6566  eshRateStatR.ref
+00001490: 7265 7368 5261 7465 5374 6174 7312 650a  reshRateStats.e.
+000014a0: 1275 7064 6174 655f 706f 7765 725f 7374  .update_power_st
+000014b0: 6174 6518 0620 0128 0b32 372e 7065 7266  ate.. .(.27.perf
+000014c0: 6574 746f 2e70 726f 746f 732e 416e 6472  etto.protos.Andr
+000014d0: 6f69 6444 6973 706c 6179 4d65 7472 6963  oidDisplayMetric
+000014e0: 732e 5570 6461 7465 506f 7765 7253 7461  s.UpdatePowerSta
+000014f0: 7465 5210 7570 6461 7465 506f 7765 7253  teR.updatePowerS
+00001500: 7461 7465 1a91 010a 0f52 6566 7265 7368  tate.....Refresh
+00001510: 5261 7465 5374 6174 1228 0a10 7265 6672  RateStat.(..refr
+00001520: 6573 685f 7261 7465 5f66 7073 1801 2001  esh_rate_fps.. .
+00001530: 280d 520e 7265 6672 6573 6852 6174 6546  (.R.refreshRateF
+00001540: 7073 1214 0a05 636f 756e 7418 0220 0128  ps....count.. .(
+00001550: 0d52 0563 6f75 6e74 1220 0a0c 746f 7461  .R.count. ..tota
+00001560: 6c5f 6475 725f 6d73 1803 2001 2801 520a  l_dur_ms.. .(.R.
+00001570: 746f 7461 6c44 7572 4d73 121c 0a0a 6176  totalDurMs....av
+00001580: 675f 6475 725f 6d73 1804 2001 2801 5208  g_dur_ms.. .(.R.
+00001590: 6176 6744 7572 4d73 1a4d 0a10 5570 6461  avgDurMs.M..Upda
+000015a0: 7465 506f 7765 7253 7461 7465 1233 0a16  tePowerState.3..
+000015b0: 6176 675f 7275 6e74 696d 655f 6d69 6372  avg_runtime_micr
+000015c0: 6f5f 7365 6373 1802 2001 280d 5213 6176  o_secs.. .(.R.av
+000015d0: 6752 756e 7469 6d65 4d69 6372 6f53 6563  gRuntimeMicroSec
+000015e0: 734a 0408 0110 020a 8802 0a35 7072 6f74  sJ.........5prot
+000015f0: 6f73 2f70 6572 6665 7474 6f2f 6d65 7472  os/perfetto/metr
+00001600: 6963 732f 616e 6472 6f69 642f 646d 615f  ics/android/dma_
+00001610: 6865 6170 5f6d 6574 7269 632e 7072 6f74  heap_metric.prot
+00001620: 6f12 0f70 6572 6665 7474 6f2e 7072 6f74  o..perfetto.prot
+00001630: 6f73 22bd 010a 1441 6e64 726f 6964 446d  os"....AndroidDm
+00001640: 6148 6561 704d 6574 7269 6312 240a 0e61  aHeapMetric.$..a
+00001650: 7667 5f73 697a 655f 6279 7465 7318 0120  vg_size_bytes.. 
+00001660: 0128 0152 0c61 7667 5369 7a65 4279 7465  .(.R.avgSizeByte
+00001670: 7312 240a 0e6d 696e 5f73 697a 655f 6279  s.$..min_size_by
+00001680: 7465 7318 0220 0128 0152 0c6d 696e 5369  tes.. .(.R.minSi
+00001690: 7a65 4279 7465 7312 240a 0e6d 6178 5f73  zeBytes.$..max_s
+000016a0: 697a 655f 6279 7465 7318 0320 0128 0152  ize_bytes.. .(.R
+000016b0: 0c6d 6178 5369 7a65 4279 7465 7312 330a  .maxSizeBytes.3.
+000016c0: 1674 6f74 616c 5f61 6c6c 6f63 5f73 697a  .total_alloc_siz
+000016d0: 655f 6279 7465 7318 0420 0128 0152 1374  e_bytes.. .(.R.t
+000016e0: 6f74 616c 416c 6c6f 6353 697a 6542 7974  otalAllocSizeByt
+000016f0: 6573 0aa5 030a 3170 726f 746f 732f 7065  es....1protos/pe
+00001700: 7266 6574 746f 2f6d 6574 7269 6373 2f61  rfetto/metrics/a
+00001710: 6e64 726f 6964 2f64 7666 735f 6d65 7472  ndroid/dvfs_metr
+00001720: 6963 2e70 726f 746f 120f 7065 7266 6574  ic.proto..perfet
+00001730: 746f 2e70 726f 746f 7322 de02 0a11 416e  to.protos"....An
+00001740: 6472 6f69 6444 7666 734d 6574 7269 6312  droidDvfsMetric.
+00001750: 600a 1066 7265 715f 7265 7369 6465 6e63  `..freq_residenc
+00001760: 6965 7318 0120 0328 0b32 352e 7065 7266  ies.. .(.25.perf
+00001770: 6574 746f 2e70 726f 746f 732e 416e 6472  etto.protos.Andr
+00001780: 6f69 6444 7666 734d 6574 7269 632e 4672  oidDvfsMetric.Fr
+00001790: 6571 7565 6e63 7952 6573 6964 656e 6379  equencyResidency
+000017a0: 520f 6672 6571 5265 7369 6465 6e63 6965  R.freqResidencie
+000017b0: 731a 6a0a 0842 616e 6453 7461 7412 1d0a  s.j..BandStat...
+000017c0: 0a66 7265 715f 7661 6c75 6518 0120 0128  .freq_value.. .(
+000017d0: 0552 0966 7265 7156 616c 7565 121e 0a0a  .R.freqValue....
+000017e0: 7065 7263 656e 7461 6765 1802 2001 2801  percentage.. .(.
+000017f0: 520a 7065 7263 656e 7461 6765 121f 0a0b  R.percentage....
+00001800: 6475 7261 7469 6f6e 5f6e 7318 0320 0128  duration_ns.. .(
+00001810: 0352 0a64 7572 6174 696f 6e4e 731a 7b0a  .R.durationNs.{.
+00001820: 1246 7265 7175 656e 6379 5265 7369 6465  .FrequencyReside
+00001830: 6e63 7912 1b0a 0966 7265 715f 6e61 6d65  ncy....freq_name
+00001840: 1801 2001 2809 5208 6672 6571 4e61 6d65  .. .(.R.freqName
+00001850: 1248 0a09 6261 6e64 5f73 7461 7418 0220  .H..band_stat.. 
+00001860: 0328 0b32 2b2e 7065 7266 6574 746f 2e70  .(.2+.perfetto.p
+00001870: 726f 746f 732e 416e 6472 6f69 6444 7666  rotos.AndroidDvf
+00001880: 734d 6574 7269 632e 4261 6e64 5374 6174  sMetric.BandStat
+00001890: 5208 6261 6e64 5374 6174 0af8 020a 3470  R.bandStat....4p
+000018a0: 726f 746f 732f 7065 7266 6574 746f 2f6d  rotos/perfetto/m
+000018b0: 6574 7269 6373 2f61 6e64 726f 6964 2f66  etrics/android/f
+000018c0: 6173 7472 7063 5f6d 6574 7269 632e 7072  astrpc_metric.pr
+000018d0: 6f74 6f12 0f70 6572 6665 7474 6f2e 7072  oto..perfetto.pr
+000018e0: 6f74 6f73 22ae 020a 1441 6e64 726f 6964  otos"....Android
+000018f0: 4661 7374 7270 634d 6574 7269 6312 4d0a  FastrpcMetric.M.
+00001900: 0973 7562 7379 7374 656d 1801 2003 280b  .subsystem.. .(.
+00001910: 322f 2e70 6572 6665 7474 6f2e 7072 6f74  2/.perfetto.prot
+00001920: 6f73 2e41 6e64 726f 6964 4661 7374 7270  os.AndroidFastrp
+00001930: 634d 6574 7269 632e 5375 6273 7973 7465  cMetric.Subsyste
+00001940: 6d52 0973 7562 7379 7374 656d 1ac6 010a  mR.subsystem....
+00001950: 0953 7562 7379 7374 656d 1212 0a04 6e61  .Subsystem....na
+00001960: 6d65 1801 2001 2809 5204 6e61 6d65 1224  me.. .(.R.name.$
+00001970: 0a0e 6176 675f 7369 7a65 5f62 7974 6573  ..avg_size_bytes
+00001980: 1802 2001 2801 520c 6176 6753 697a 6542  .. .(.R.avgSizeB
+00001990: 7974 6573 1224 0a0e 6d69 6e5f 7369 7a65  ytes.$..min_size
+000019a0: 5f62 7974 6573 1803 2001 2801 520c 6d69  _bytes.. .(.R.mi
+000019b0: 6e53 697a 6542 7974 6573 1224 0a0e 6d61  nSizeBytes.$..ma
+000019c0: 785f 7369 7a65 5f62 7974 6573 1804 2001  x_size_bytes.. .
+000019d0: 2801 520c 6d61 7853 697a 6542 7974 6573  (.R.maxSizeBytes
+000019e0: 1233 0a16 746f 7461 6c5f 616c 6c6f 635f  .3..total_alloc_
+000019f0: 7369 7a65 5f62 7974 6573 1805 2001 2801  size_bytes.. .(.
+00001a00: 5213 746f 7461 6c41 6c6c 6f63 5369 7a65  R.totalAllocSize
+00001a10: 4279 7465 730a 8b05 0a30 7072 6f74 6f73  Bytes....0protos
+00001a20: 2f70 6572 6665 7474 6f2f 6d65 7472 6963  /perfetto/metric
+00001a30: 732f 616e 6472 6f69 642f 6732 645f 6d65  s/android/g2d_me
+00001a40: 7472 6963 2e70 726f 746f 120f 7065 7266  tric.proto..perf
+00001a50: 6574 746f 2e70 726f 746f 7322 c504 0a0a  etto.protos"....
+00001a60: 4732 644d 6574 7269 6373 123c 0a06 6732  G2dMetrics.<..g2
+00001a70: 645f 6877 1801 2001 280b 3225 2e70 6572  d_hw.. .(.2%.per
+00001a80: 6665 7474 6f2e 7072 6f74 6f73 2e47 3264  fetto.protos.G2d
+00001a90: 4d65 7472 6963 732e 4732 644d 6574 7269  Metrics.G2dMetri
+00001aa0: 6352 0567 3264 4877 123c 0a06 6732 645f  cR.g2dHw.<..g2d_
+00001ab0: 7377 1802 2001 280b 3225 2e70 6572 6665  sw.. .(.2%.perfe
+00001ac0: 7474 6f2e 7072 6f74 6f73 2e47 3264 4d65  tto.protos.G2dMe
+00001ad0: 7472 6963 732e 4732 644d 6574 7269 6352  trics.G2dMetricR
+00001ae0: 0567 3264 5377 1ac3 010a 0b47 3264 496e  .g2dSw.....G2dIn
+00001af0: 7374 616e 6365 1212 0a04 6e61 6d65 1801  stance....name..
+00001b00: 2001 2809 5204 6e61 6d65 121f 0a0b 6672   .(.R.name....fr
+00001b10: 616d 655f 636f 756e 7418 0520 0128 0d52  ame_count.. .(.R
+00001b20: 0a66 7261 6d65 436f 756e 7412 1f0a 0b65  .frameCount....e
+00001b30: 7272 6f72 5f63 6f75 6e74 1806 2001 280d  rror_count.. .(.
+00001b40: 520a 6572 726f 7243 6f75 6e74 121c 0a0a  R.errorCount....
+00001b50: 6d61 785f 6475 725f 6d73 1807 2001 2801  max_dur_ms.. .(.
+00001b60: 5208 6d61 7844 7572 4d73 121c 0a0a 6d69  R.maxDurMs....mi
+00001b70: 6e5f 6475 725f 6d73 1808 2001 2801 5208  n_dur_ms.. .(.R.
+00001b80: 6d69 6e44 7572 4d73 121c 0a0a 6176 675f  minDurMs....avg_
+00001b90: 6475 725f 6d73 1809 2001 2801 5208 6176  dur_ms.. .(.R.av
+00001ba0: 6744 7572 4d73 4a04 0802 1005 1af4 010a  gDurMsJ.........
+00001bb0: 0947 3264 4d65 7472 6963 1245 0a09 696e  .G2dMetric.E..in
+00001bc0: 7374 616e 6365 7318 0120 0328 0b32 272e  stances.. .(.2'.
+00001bd0: 7065 7266 6574 746f 2e70 726f 746f 732e  perfetto.protos.
+00001be0: 4732 644d 6574 7269 6373 2e47 3264 496e  G2dMetrics.G2dIn
+00001bf0: 7374 616e 6365 5209 696e 7374 616e 6365  stanceR.instance
+00001c00: 7312 1f0a 0b66 7261 6d65 5f63 6f75 6e74  s....frame_count
+00001c10: 1805 2001 280d 520a 6672 616d 6543 6f75  .. .(.R.frameCou
+00001c20: 6e74 121f 0a0b 6572 726f 725f 636f 756e  nt....error_coun
+00001c30: 7418 0620 0128 0d52 0a65 7272 6f72 436f  t.. .(.R.errorCo
+00001c40: 756e 7412 1c0a 0a6d 6178 5f64 7572 5f6d  unt....max_dur_m
+00001c50: 7318 0720 0128 0152 086d 6178 4475 724d  s.. .(.R.maxDurM
+00001c60: 7312 1c0a 0a6d 696e 5f64 7572 5f6d 7318  s....min_dur_ms.
+00001c70: 0820 0128 0152 086d 696e 4475 724d 7312  . .(.R.minDurMs.
+00001c80: 1c0a 0a61 7667 5f64 7572 5f6d 7318 0920  ...avg_dur_ms.. 
+00001c90: 0128 0152 0861 7667 4475 724d 734a 0408  .(.R.avgDurMsJ..
+00001ca0: 0210 050a f005 0a30 7072 6f74 6f73 2f70  .......0protos/p
+00001cb0: 6572 6665 7474 6f2f 6d65 7472 6963 732f  erfetto/metrics/
+00001cc0: 616e 6472 6f69 642f 6770 755f 6d65 7472  android/gpu_metr
+00001cd0: 6963 2e70 726f 746f 120f 7065 7266 6574  ic.proto..perfet
+00001ce0: 746f 2e70 726f 746f 7322 aa05 0a10 416e  to.protos"....An
+00001cf0: 6472 6f69 6447 7075 4d65 7472 6963 1247  droidGpuMetric.G
+00001d00: 0a09 7072 6f63 6573 7365 7318 0120 0328  ..processes.. .(
+00001d10: 0b32 292e 7065 7266 6574 746f 2e70 726f  .2).perfetto.pro
+00001d20: 746f 732e 416e 6472 6f69 6447 7075 4d65  tos.AndroidGpuMe
+00001d30: 7472 6963 2e50 726f 6365 7373 5209 7072  tric.ProcessR.pr
+00001d40: 6f63 6573 7365 7312 170a 076d 656d 5f6d  ocesses....mem_m
+00001d50: 6178 1802 2001 2803 5206 6d65 6d4d 6178  ax.. .(.R.memMax
+00001d60: 1217 0a07 6d65 6d5f 6d69 6e18 0320 0128  ....mem_min.. .(
+00001d70: 0352 066d 656d 4d69 6e12 170a 076d 656d  .R.memMin....mem
+00001d80: 5f61 7667 1804 2001 2803 5206 6d65 6d41  _avg.. .(.R.memA
+00001d90: 7667 1254 0a0c 6672 6571 5f6d 6574 7269  vg.T..freq_metri
+00001da0: 6373 1805 2003 280b 3231 2e70 6572 6665  cs.. .(.21.perfe
+00001db0: 7474 6f2e 7072 6f74 6f73 2e41 6e64 726f  tto.protos.Andro
+00001dc0: 6964 4770 754d 6574 7269 632e 4672 6571  idGpuMetric.Freq
+00001dd0: 7565 6e63 794d 6574 7269 6352 0b66 7265  uencyMetricR.fre
+00001de0: 714d 6574 7269 6373 1a68 0a07 5072 6f63  qMetrics.h..Proc
+00001df0: 6573 7312 120a 046e 616d 6518 0120 0128  ess....name.. .(
+00001e00: 0952 046e 616d 6512 170a 076d 656d 5f6d  .R.name....mem_m
+00001e10: 6178 1802 2001 2803 5206 6d65 6d4d 6178  ax.. .(.R.memMax
+00001e20: 1217 0a07 6d65 6d5f 6d69 6e18 0320 0128  ....mem_min.. .(
+00001e30: 0352 066d 656d 4d69 6e12 170a 076d 656d  .R.memMin....mem
+00001e40: 5f61 7667 1804 2001 2803 5206 6d65 6d41  _avg.. .(.R.memA
+00001e50: 7667 1ac1 020a 0f46 7265 7175 656e 6379  vg.....Frequency
+00001e60: 4d65 7472 6963 1215 0a06 6770 755f 6964  Metric....gpu_id
+00001e70: 1801 2001 280d 5205 6770 7549 6412 190a  .. .(.R.gpuId...
+00001e80: 0866 7265 715f 6d61 7818 0220 0128 0352  .freq_max.. .(.R
+00001e90: 0766 7265 714d 6178 1219 0a08 6672 6571  .freqMax....freq
+00001ea0: 5f6d 696e 1803 2001 2803 5207 6672 6571  _min.. .(.R.freq
+00001eb0: 4d69 6e12 190a 0866 7265 715f 6176 6718  Min....freq_avg.
+00001ec0: 0420 0128 0152 0766 7265 7141 7667 1264  . .(.R.freqAvg.d
+00001ed0: 0a0a 7573 6564 5f66 7265 7173 1805 2003  ..used_freqs.. .
+00001ee0: 280b 3245 2e70 6572 6665 7474 6f2e 7072  (.2E.perfetto.pr
+00001ef0: 6f74 6f73 2e41 6e64 726f 6964 4770 754d  otos.AndroidGpuM
+00001f00: 6574 7269 632e 4672 6571 7565 6e63 794d  etric.FrequencyM
+00001f10: 6574 7269 632e 4d65 7472 6963 7350 6572  etric.MetricsPer
+00001f20: 4672 6571 7565 6e63 7952 0975 7365 6446  FrequencyR.usedF
+00001f30: 7265 7173 1a60 0a13 4d65 7472 6963 7350  reqs.`..MetricsP
+00001f40: 6572 4672 6571 7565 6e63 7912 120a 0466  erFrequency....f
+00001f50: 7265 7118 0120 0128 0352 0466 7265 7112  req.. .(.R.freq.
+00001f60: 150a 0664 7572 5f6d 7318 0220 0128 0152  ...dur_ms.. .(.R
+00001f70: 0564 7572 4d73 121e 0a0a 7065 7263 656e  .durMs....percen
+00001f80: 7461 6765 1803 2001 2801 520a 7065 7263  tage.. .(.R.perc
+00001f90: 656e 7461 6765 0af2 110a 3070 726f 746f  entage....0proto
+00001fa0: 732f 7065 7266 6574 746f 2f6d 6574 7269  s/perfetto/metri
+00001fb0: 6373 2f61 6e64 726f 6964 2f68 7763 6f6d  cs/android/hwcom
+00001fc0: 706f 7365 722e 7072 6f74 6f12 0f70 6572  poser.proto..per
+00001fd0: 6665 7474 6f2e 7072 6f74 6f73 22ac 110a  fetto.protos"...
+00001fe0: 1841 6e64 726f 6964 4877 636f 6d70 6f73  .AndroidHwcompos
+00001ff0: 6572 4d65 7472 6963 7312 380a 1863 6f6d  erMetrics.8..com
+00002000: 706f 7369 7469 6f6e 5f74 6f74 616c 5f6c  position_total_l
+00002010: 6179 6572 7318 0120 0128 0152 1663 6f6d  ayers.. .(.R.com
+00002020: 706f 7369 7469 6f6e 546f 7461 6c4c 6179  positionTotalLay
+00002030: 6572 7312 340a 1663 6f6d 706f 7369 7469  ers.4..compositi
+00002040: 6f6e 5f64 7075 5f6c 6179 6572 7318 0220  on_dpu_layers.. 
+00002050: 0128 0152 1463 6f6d 706f 7369 7469 6f6e  .(.R.composition
+00002060: 4470 754c 6179 6572 7312 340a 1663 6f6d  DpuLayers.4..com
+00002070: 706f 7369 7469 6f6e 5f67 7075 5f6c 6179  position_gpu_lay
+00002080: 6572 7318 0320 0128 0152 1463 6f6d 706f  ers.. .(.R.compo
+00002090: 7369 7469 6f6e 4770 754c 6179 6572 7312  sitionGpuLayers.
+000020a0: 410a 1d63 6f6d 706f 7369 7469 6f6e 5f64  A..composition_d
+000020b0: 7075 5f63 6163 6865 645f 6c61 7965 7273  pu_cached_layers
+000020c0: 1804 2001 2801 521a 636f 6d70 6f73 6974  .. .(.R.composit
+000020d0: 696f 6e44 7075 4361 6368 6564 4c61 7965  ionDpuCachedLaye
+000020e0: 7273 123f 0a1c 636f 6d70 6f73 6974 696f  rs.?..compositio
+000020f0: 6e5f 7366 5f63 6163 6865 645f 6c61 7965  n_sf_cached_laye
+00002100: 7273 1805 2001 2801 5219 636f 6d70 6f73  rs.. .(.R.compos
+00002110: 6974 696f 6e53 6643 6163 6865 644c 6179  itionSfCachedLay
+00002120: 6572 7312 340a 1663 6f6d 706f 7369 7469  ers.4..compositi
+00002130: 6f6e 5f72 6364 5f6c 6179 6572 7318 0f20  on_rcd_layers.. 
+00002140: 0128 0152 1463 6f6d 706f 7369 7469 6f6e  .(.R.composition
+00002150: 5263 644c 6179 6572 7312 380a 1873 6b69  RcdLayers.8..ski
+00002160: 7070 6564 5f76 616c 6964 6174 696f 6e5f  pped_validation_
+00002170: 636f 756e 7418 0620 0128 0552 1673 6b69  count.. .(.R.ski
+00002180: 7070 6564 5661 6c69 6461 7469 6f6e 436f  ppedValidationCo
+00002190: 756e 7412 3c0a 1a75 6e73 6b69 7070 6564  unt.<..unskipped
+000021a0: 5f76 616c 6964 6174 696f 6e5f 636f 756e  _validation_coun
+000021b0: 7418 0720 0128 0552 1875 6e73 6b69 7070  t.. .(.R.unskipp
+000021c0: 6564 5661 6c69 6461 7469 6f6e 436f 756e  edValidationCoun
+000021d0: 7412 3c0a 1a73 6570 6172 6174 6564 5f76  t.<..separated_v
+000021e0: 616c 6964 6174 696f 6e5f 636f 756e 7418  alidation_count.
+000021f0: 0820 0128 0552 1873 6570 6172 6174 6564  . .(.R.separated
+00002200: 5661 6c69 6461 7469 6f6e 436f 756e 7412  ValidationCount.
+00002210: 380a 1875 6e6b 6e6f 776e 5f76 616c 6964  8..unknown_valid
+00002220: 6174 696f 6e5f 636f 756e 7418 0920 0128  ation_count.. .(
+00002230: 0552 1675 6e6b 6e6f 776e 5661 6c69 6461  .R.unknownValida
+00002240: 7469 6f6e 436f 756e 7412 380a 1961 7667  tionCount.8..avg
+00002250: 5f61 6c6c 5f65 7865 6375 7469 6f6e 5f74  _all_execution_t
+00002260: 696d 655f 6d73 180a 2001 2801 5215 6176  ime_ms.. .(.R.av
+00002270: 6741 6c6c 4578 6563 7574 696f 6e54 696d  gAllExecutionTim
+00002280: 654d 7312 400a 1d61 7667 5f73 6b69 7070  eMs.@..avg_skipp
+00002290: 6564 5f65 7865 6375 7469 6f6e 5f74 696d  ed_execution_tim
+000022a0: 655f 6d73 180b 2001 2801 5219 6176 6753  e_ms.. .(.R.avgS
+000022b0: 6b69 7070 6564 4578 6563 7574 696f 6e54  kippedExecutionT
+000022c0: 696d 654d 7312 440a 1f61 7667 5f75 6e73  imeMs.D..avg_uns
+000022d0: 6b69 7070 6564 5f65 7865 6375 7469 6f6e  kipped_execution
+000022e0: 5f74 696d 655f 6d73 180c 2001 2801 521b  _time_ms.. .(.R.
+000022f0: 6176 6755 6e73 6b69 7070 6564 4578 6563  avgUnskippedExec
+00002300: 7574 696f 6e54 696d 654d 7312 440a 1f61  utionTimeMs.D..a
+00002310: 7667 5f73 6570 6172 6174 6564 5f65 7865  vg_separated_exe
+00002320: 6375 7469 6f6e 5f74 696d 655f 6d73 180d  cution_time_ms..
+00002330: 2001 2801 521b 6176 6753 6570 6172 6174   .(.R.avgSeparat
+00002340: 6564 4578 6563 7574 696f 6e54 696d 654d  edExecutionTimeM
+00002350: 7312 620a 1064 7075 5f76 6f74 655f 6d65  s.b..dpu_vote_me
+00002360: 7472 6963 7318 0e20 0328 0b32 382e 7065  trics.. .(.28.pe
+00002370: 7266 6574 746f 2e70 726f 746f 732e 416e  rfetto.protos.An
+00002380: 6472 6f69 6448 7763 6f6d 706f 7365 724d  droidHwcomposerM
+00002390: 6574 7269 6373 2e44 7075 566f 7465 4d65  etrics.DpuVoteMe
+000023a0: 7472 6963 7352 0e64 7075 566f 7465 4d65  tricsR.dpuVoteMe
+000023b0: 7472 6963 7312 6b0a 136d 6574 7269 6373  trics.k..metrics
+000023c0: 5f70 6572 5f64 6973 706c 6179 1810 2003  _per_display.. .
+000023d0: 280b 323b 2e70 6572 6665 7474 6f2e 7072  (.2;.perfetto.pr
+000023e0: 6f74 6f73 2e41 6e64 726f 6964 4877 636f  otos.AndroidHwco
+000023f0: 6d70 6f73 6572 4d65 7472 6963 732e 4d65  mposerMetrics.Me
+00002400: 7472 6963 7350 6572 4469 7370 6c61 7952  tricsPerDisplayR
+00002410: 116d 6574 7269 6373 5065 7244 6973 706c  .metricsPerDispl
+00002420: 6179 1ad9 010a 0e44 7075 566f 7465 4d65  ay.....DpuVoteMe
+00002430: 7472 6963 7312 100a 0374 6964 1801 2001  trics....tid.. .
+00002440: 280d 5203 7469 6412 2b0a 1261 7667 5f64  (.R.tid.+..avg_d
+00002450: 7075 5f76 6f74 655f 636c 6f63 6b18 0220  pu_vote_clock.. 
+00002460: 0128 0152 0f61 7667 4470 7556 6f74 6543  .(.R.avgDpuVoteC
+00002470: 6c6f 636b 122c 0a13 6176 675f 6470 755f  lock.,..avg_dpu_
+00002480: 766f 7465 5f61 7667 5f62 7718 0320 0128  vote_avg_bw.. .(
+00002490: 0152 0f61 7667 4470 7556 6f74 6541 7667  .R.avgDpuVoteAvg
+000024a0: 4277 122e 0a14 6176 675f 6470 755f 766f  Bw....avg_dpu_vo
+000024b0: 7465 5f70 6561 6b5f 6277 1804 2001 2801  te_peak_bw.. .(.
+000024c0: 5210 6176 6744 7075 566f 7465 5065 616b  R.avgDpuVotePeak
+000024d0: 4277 122a 0a12 6176 675f 6470 755f 766f  Bw.*..avg_dpu_vo
+000024e0: 7465 5f72 745f 6277 1805 2001 2801 520e  te_rt_bw.. .(.R.
+000024f0: 6176 6744 7075 566f 7465 5274 4277 1a8a  avgDpuVoteRtBw..
+00002500: 070a 114d 6574 7269 6373 5065 7244 6973  ...MetricsPerDis
+00002510: 706c 6179 121d 0a0a 6469 7370 6c61 795f  play....display_
+00002520: 6964 1801 2001 2809 5209 6469 7370 6c61  id.. .(.R.displa
+00002530: 7949 6412 380a 1863 6f6d 706f 7369 7469  yId.8..compositi
+00002540: 6f6e 5f74 6f74 616c 5f6c 6179 6572 7318  on_total_layers.
+00002550: 0220 0128 0152 1663 6f6d 706f 7369 7469  . .(.R.compositi
+00002560: 6f6e 546f 7461 6c4c 6179 6572 7312 340a  onTotalLayers.4.
+00002570: 1663 6f6d 706f 7369 7469 6f6e 5f64 7075  .composition_dpu
+00002580: 5f6c 6179 6572 7318 0320 0128 0152 1463  _layers.. .(.R.c
+00002590: 6f6d 706f 7369 7469 6f6e 4470 754c 6179  ompositionDpuLay
+000025a0: 6572 7312 340a 1663 6f6d 706f 7369 7469  ers.4..compositi
+000025b0: 6f6e 5f67 7075 5f6c 6179 6572 7318 0420  on_gpu_layers.. 
+000025c0: 0128 0152 1463 6f6d 706f 7369 7469 6f6e  .(.R.composition
+000025d0: 4770 754c 6179 6572 7312 410a 1d63 6f6d  GpuLayers.A..com
+000025e0: 706f 7369 7469 6f6e 5f64 7075 5f63 6163  position_dpu_cac
+000025f0: 6865 645f 6c61 7965 7273 1805 2001 2801  hed_layers.. .(.
+00002600: 521a 636f 6d70 6f73 6974 696f 6e44 7075  R.compositionDpu
+00002610: 4361 6368 6564 4c61 7965 7273 123f 0a1c  CachedLayers.?..
+00002620: 636f 6d70 6f73 6974 696f 6e5f 7366 5f63  composition_sf_c
+00002630: 6163 6865 645f 6c61 7965 7273 1806 2001  ached_layers.. .
+00002640: 2801 5219 636f 6d70 6f73 6974 696f 6e53  (.R.compositionS
+00002650: 6643 6163 6865 644c 6179 6572 7312 340a  fCachedLayers.4.
+00002660: 1663 6f6d 706f 7369 7469 6f6e 5f72 6364  .composition_rcd
+00002670: 5f6c 6179 6572 7318 0720 0128 0152 1463  _layers.. .(.R.c
+00002680: 6f6d 706f 7369 7469 6f6e 5263 644c 6179  ompositionRcdLay
+00002690: 6572 7312 380a 1873 6b69 7070 6564 5f76  ers.8..skipped_v
+000026a0: 616c 6964 6174 696f 6e5f 636f 756e 7418  alidation_count.
+000026b0: 0820 0128 0552 1673 6b69 7070 6564 5661  . .(.R.skippedVa
+000026c0: 6c69 6461 7469 6f6e 436f 756e 7412 3c0a  lidationCount.<.
+000026d0: 1a75 6e73 6b69 7070 6564 5f76 616c 6964  .unskipped_valid
+000026e0: 6174 696f 6e5f 636f 756e 7418 0920 0128  ation_count.. .(
+000026f0: 0552 1875 6e73 6b69 7070 6564 5661 6c69  .R.unskippedVali
+00002700: 6461 7469 6f6e 436f 756e 7412 3c0a 1a73  dationCount.<..s
+00002710: 6570 6172 6174 6564 5f76 616c 6964 6174  eparated_validat
+00002720: 696f 6e5f 636f 756e 7418 0a20 0128 0552  ion_count.. .(.R
+00002730: 1873 6570 6172 6174 6564 5661 6c69 6461  .separatedValida
+00002740: 7469 6f6e 436f 756e 7412 380a 1875 6e6b  tionCount.8..unk
+00002750: 6e6f 776e 5f76 616c 6964 6174 696f 6e5f  nown_validation_
+00002760: 636f 756e 7418 0b20 0128 0552 1675 6e6b  count.. .(.R.unk
+00002770: 6e6f 776e 5661 6c69 6461 7469 6f6e 436f  nownValidationCo
+00002780: 756e 7412 380a 1961 7667 5f61 6c6c 5f65  unt.8..avg_all_e
+00002790: 7865 6375 7469 6f6e 5f74 696d 655f 6d73  xecution_time_ms
+000027a0: 180c 2001 2801 5215 6176 6741 6c6c 4578  .. .(.R.avgAllEx
+000027b0: 6563 7574 696f 6e54 696d 654d 7312 400a  ecutionTimeMs.@.
+000027c0: 1d61 7667 5f73 6b69 7070 6564 5f65 7865  .avg_skipped_exe
+000027d0: 6375 7469 6f6e 5f74 696d 655f 6d73 180d  cution_time_ms..
+000027e0: 2001 2801 5219 6176 6753 6b69 7070 6564   .(.R.avgSkipped
+000027f0: 4578 6563 7574 696f 6e54 696d 654d 7312  ExecutionTimeMs.
+00002800: 440a 1f61 7667 5f75 6e73 6b69 7070 6564  D..avg_unskipped
+00002810: 5f65 7865 6375 7469 6f6e 5f74 696d 655f  _execution_time_
+00002820: 6d73 180e 2001 2801 521b 6176 6755 6e73  ms.. .(.R.avgUns
+00002830: 6b69 7070 6564 4578 6563 7574 696f 6e54  kippedExecutionT
+00002840: 696d 654d 7312 440a 1f61 7667 5f73 6570  imeMs.D..avg_sep
+00002850: 6172 6174 6564 5f65 7865 6375 7469 6f6e  arated_execution
+00002860: 5f74 696d 655f 6d73 180f 2001 2801 521b  _time_ms.. .(.R.
+00002870: 6176 6753 6570 6172 6174 6564 4578 6563  avgSeparatedExec
+00002880: 7574 696f 6e54 696d 654d 730a 860f 0a31  utionTimeMs....1
+00002890: 7072 6f74 6f73 2f70 6572 6665 7474 6f2f  protos/perfetto/
+000028a0: 6d65 7472 6963 732f 616e 6472 6f69 642f  metrics/android/
+000028b0: 6877 7569 5f6d 6574 7269 632e 7072 6f74  hwui_metric.prot
+000028c0: 6f12 0f70 6572 6665 7474 6f2e 7072 6f74  o..perfetto.prot
+000028d0: 6f73 22e3 0d0a 1150 726f 6365 7373 5265  os"....ProcessRe
+000028e0: 6e64 6572 496e 666f 1221 0a0c 7072 6f63  nderInfo.!..proc
+000028f0: 6573 735f 6e61 6d65 1801 2001 2809 520b  ess_name.. .(.R.
+00002900: 7072 6f63 6573 734e 616d 6512 230a 0e72  processName.#..r
+00002910: 745f 6370 755f 7469 6d65 5f6d 7318 0220  t_cpu_time_ms.. 
+00002920: 0128 0352 0b72 7443 7075 5469 6d65 4d73  .(.R.rtCpuTimeMs
+00002930: 1228 0a10 6472 6177 5f66 7261 6d65 5f63  .(..draw_frame_c
+00002940: 6f75 6e74 1803 2001 280d 520e 6472 6177  ount.. .(.R.draw
+00002950: 4672 616d 6543 6f75 6e74 1224 0a0e 6472  FrameCount.$..dr
+00002960: 6177 5f66 7261 6d65 5f6d 6178 1804 2001  aw_frame_max.. .
+00002970: 2803 520c 6472 6177 4672 616d 654d 6178  (.R.drawFrameMax
+00002980: 1224 0a0e 6472 6177 5f66 7261 6d65 5f6d  .$..draw_frame_m
+00002990: 696e 1805 2001 2803 520c 6472 6177 4672  in.. .(.R.drawFr
+000029a0: 616d 654d 696e 1224 0a0e 6472 6177 5f66  ameMin.$..draw_f
+000029b0: 7261 6d65 5f61 7667 1806 2001 2801 520c  rame_avg.. .(.R.
+000029c0: 6472 6177 4672 616d 6541 7667 121f 0a0b  drawFrameAvg....
+000029d0: 666c 7573 685f 636f 756e 7418 0720 0128  flush_count.. .(
+000029e0: 0d52 0a66 6c75 7368 436f 756e 7412 1b0a  .R.flushCount...
+000029f0: 0966 6c75 7368 5f6d 6178 1808 2001 2803  .flush_max.. .(.
+00002a00: 5208 666c 7573 684d 6178 121b 0a09 666c  R.flushMax....fl
+00002a10: 7573 685f 6d69 6e18 0920 0128 0352 0866  ush_min.. .(.R.f
+00002a20: 6c75 7368 4d69 6e12 1b0a 0966 6c75 7368  lushMin....flush
+00002a30: 5f61 7667 180a 2001 2801 5208 666c 7573  _avg.. .(.R.flus
+00002a40: 6841 7667 122c 0a12 7072 6570 6172 655f  hAvg.,..prepare_
+00002a50: 7472 6565 5f63 6f75 6e74 180b 2001 280d  tree_count.. .(.
+00002a60: 5210 7072 6570 6172 6554 7265 6543 6f75  R.prepareTreeCou
+00002a70: 6e74 1228 0a10 7072 6570 6172 655f 7472  nt.(..prepare_tr
+00002a80: 6565 5f6d 6178 180c 2001 2803 520e 7072  ee_max.. .(.R.pr
+00002a90: 6570 6172 6554 7265 654d 6178 1228 0a10  epareTreeMax.(..
+00002aa0: 7072 6570 6172 655f 7472 6565 5f6d 696e  prepare_tree_min
+00002ab0: 180d 2001 2803 520e 7072 6570 6172 6554  .. .(.R.prepareT
+00002ac0: 7265 654d 696e 1228 0a10 7072 6570 6172  reeMin.(..prepar
+00002ad0: 655f 7472 6565 5f61 7667 180e 2001 2801  e_tree_avg.. .(.
+00002ae0: 520e 7072 6570 6172 6554 7265 6541 7667  R.prepareTreeAvg
+00002af0: 1230 0a14 6770 755f 636f 6d70 6c65 7469  .0..gpu_completi
+00002b00: 6f6e 5f63 6f75 6e74 180f 2001 280d 5212  on_count.. .(.R.
+00002b10: 6770 7543 6f6d 706c 6574 696f 6e43 6f75  gpuCompletionCou
+00002b20: 6e74 122c 0a12 6770 755f 636f 6d70 6c65  nt.,..gpu_comple
+00002b30: 7469 6f6e 5f6d 6178 1810 2001 2803 5210  tion_max.. .(.R.
+00002b40: 6770 7543 6f6d 706c 6574 696f 6e4d 6178  gpuCompletionMax
+00002b50: 122c 0a12 6770 755f 636f 6d70 6c65 7469  .,..gpu_completi
+00002b60: 6f6e 5f6d 696e 1811 2001 2803 5210 6770  on_min.. .(.R.gp
+00002b70: 7543 6f6d 706c 6574 696f 6e4d 696e 122c  uCompletionMin.,
+00002b80: 0a12 6770 755f 636f 6d70 6c65 7469 6f6e  ..gpu_completion
+00002b90: 5f61 7667 1812 2001 2801 5210 6770 7543  _avg.. .(.R.gpuC
+00002ba0: 6f6d 706c 6574 696f 6e41 7667 1226 0a0f  ompletionAvg.&..
+00002bb0: 7569 5f72 6563 6f72 645f 636f 756e 7418  ui_record_count.
+00002bc0: 1320 0128 0d52 0d75 6952 6563 6f72 6443  . .(.R.uiRecordC
+00002bd0: 6f75 6e74 1222 0a0d 7569 5f72 6563 6f72  ount."..ui_recor
+00002be0: 645f 6d61 7818 1420 0128 0352 0b75 6952  d_max.. .(.R.uiR
+00002bf0: 6563 6f72 644d 6178 1222 0a0d 7569 5f72  ecordMax."..ui_r
+00002c00: 6563 6f72 645f 6d69 6e18 1520 0128 0352  ecord_min.. .(.R
+00002c10: 0b75 6952 6563 6f72 644d 696e 1222 0a0d  .uiRecordMin."..
+00002c20: 7569 5f72 6563 6f72 645f 6176 6718 1620  ui_record_avg.. 
+00002c30: 0128 0152 0b75 6952 6563 6f72 6441 7667  .(.R.uiRecordAvg
+00002c40: 1230 0a14 7368 6164 6572 5f63 6f6d 7069  .0..shader_compi
+00002c50: 6c65 5f63 6f75 6e74 1817 2001 280d 5212  le_count.. .(.R.
+00002c60: 7368 6164 6572 436f 6d70 696c 6543 6f75  shaderCompileCou
+00002c70: 6e74 122e 0a13 7368 6164 6572 5f63 6f6d  nt....shader_com
+00002c80: 7069 6c65 5f74 696d 6518 1820 0128 0352  pile_time.. .(.R
+00002c90: 1173 6861 6465 7243 6f6d 7069 6c65 5469  .shaderCompileTi
+00002ca0: 6d65 122c 0a12 7368 6164 6572 5f63 6f6d  me.,..shader_com
+00002cb0: 7069 6c65 5f61 7667 1819 2001 2801 5210  pile_avg.. .(.R.
+00002cc0: 7368 6164 6572 436f 6d70 696c 6541 7667  shaderCompileAvg
+00002cd0: 1226 0a0f 6361 6368 655f 6869 745f 636f  .&..cache_hit_co
+00002ce0: 756e 7418 1a20 0128 0d52 0d63 6163 6865  unt.. .(.R.cache
+00002cf0: 4869 7443 6f75 6e74 1224 0a0e 6361 6368  HitCount.$..cach
+00002d00: 655f 6869 745f 7469 6d65 181b 2001 2803  e_hit_time.. .(.
+00002d10: 520c 6361 6368 6548 6974 5469 6d65 1222  R.cacheHitTime."
+00002d20: 0a0d 6361 6368 655f 6869 745f 6176 6718  ..cache_hit_avg.
+00002d30: 1c20 0128 0152 0b63 6163 6865 4869 7441  . .(.R.cacheHitA
+00002d40: 7667 1228 0a10 6361 6368 655f 6d69 7373  vg.(..cache_miss
+00002d50: 5f63 6f75 6e74 181d 2001 280d 520e 6361  _count.. .(.R.ca
+00002d60: 6368 654d 6973 7343 6f75 6e74 1226 0a0f  cheMissCount.&..
+00002d70: 6361 6368 655f 6d69 7373 5f74 696d 6518  cache_miss_time.
+00002d80: 1e20 0128 0352 0d63 6163 6865 4d69 7373  . .(.R.cacheMiss
+00002d90: 5469 6d65 1224 0a0e 6361 6368 655f 6d69  Time.$..cache_mi
+00002da0: 7373 5f61 7667 181f 2001 2801 520c 6361  ss_avg.. .(.R.ca
+00002db0: 6368 654d 6973 7341 7667 122f 0a14 6772  cheMissAvg./..gr
+00002dc0: 6170 6869 6373 5f63 7075 5f6d 656d 5f6d  aphics_cpu_mem_m
+00002dd0: 6178 1820 2001 2803 5211 6772 6170 6869  ax.  .(.R.graphi
+00002de0: 6373 4370 754d 656d 4d61 7812 2f0a 1467  csCpuMemMax./..g
+00002df0: 7261 7068 6963 735f 6370 755f 6d65 6d5f  raphics_cpu_mem_
+00002e00: 6d69 6e18 2120 0128 0352 1167 7261 7068  min.! .(.R.graph
+00002e10: 6963 7343 7075 4d65 6d4d 696e 122f 0a14  icsCpuMemMin./..
+00002e20: 6772 6170 6869 6373 5f63 7075 5f6d 656d  graphics_cpu_mem
+00002e30: 5f61 7667 1822 2001 2801 5211 6772 6170  _avg." .(.R.grap
+00002e40: 6869 6373 4370 754d 656d 4176 6712 2f0a  hicsCpuMemAvg./.
+00002e50: 1467 7261 7068 6963 735f 6770 755f 6d65  .graphics_gpu_me
+00002e60: 6d5f 6d61 7818 2320 0128 0352 1167 7261  m_max.# .(.R.gra
+00002e70: 7068 6963 7347 7075 4d65 6d4d 6178 122f  phicsGpuMemMax./
+00002e80: 0a14 6772 6170 6869 6373 5f67 7075 5f6d  ..graphics_gpu_m
+00002e90: 656d 5f6d 696e 1824 2001 2803 5211 6772  em_min.$ .(.R.gr
+00002ea0: 6170 6869 6373 4770 754d 656d 4d69 6e12  aphicsGpuMemMin.
+00002eb0: 2f0a 1467 7261 7068 6963 735f 6770 755f  /..graphics_gpu_
+00002ec0: 6d65 6d5f 6176 6718 2520 0128 0152 1167  mem_avg.% .(.R.g
+00002ed0: 7261 7068 6963 7347 7075 4d65 6d41 7667  raphicsGpuMemAvg
+00002ee0: 1226 0a0f 7465 7874 7572 655f 6d65 6d5f  .&..texture_mem_
+00002ef0: 6d61 7818 2620 0128 0352 0d74 6578 7475  max.& .(.R.textu
+00002f00: 7265 4d65 6d4d 6178 1226 0a0f 7465 7874  reMemMax.&..text
+00002f10: 7572 655f 6d65 6d5f 6d69 6e18 2720 0128  ure_mem_min.' .(
+00002f20: 0352 0d74 6578 7475 7265 4d65 6d4d 696e  .R.textureMemMin
+00002f30: 1226 0a0f 7465 7874 7572 655f 6d65 6d5f  .&..texture_mem_
+00002f40: 6176 6718 2820 0128 0152 0d74 6578 7475  avg.( .(.R.textu
+00002f50: 7265 4d65 6d41 7667 121e 0a0b 616c 6c5f  reMemAvg....all_
+00002f60: 6d65 6d5f 6d61 7818 2920 0128 0352 0961  mem_max.) .(.R.a
+00002f70: 6c6c 4d65 6d4d 6178 121e 0a0b 616c 6c5f  llMemMax....all_
+00002f80: 6d65 6d5f 6d69 6e18 2a20 0128 0352 0961  mem_min.* .(.R.a
+00002f90: 6c6c 4d65 6d4d 696e 121e 0a0b 616c 6c5f  llMemMin....all_
+00002fa0: 6d65 6d5f 6176 6718 2b20 0128 0152 0961  mem_avg.+ .(.R.a
+00002fb0: 6c6c 4d65 6d41 7667 225a 0a11 416e 6472  llMemAvg"Z..Andr
+00002fc0: 6f69 6448 7775 694d 6574 7269 6312 450a  oidHwuiMetric.E.
+00002fd0: 0c70 726f 6365 7373 5f69 6e66 6f18 0120  .process_info.. 
+00002fe0: 0328 0b32 222e 7065 7266 6574 746f 2e70  .(.2".perfetto.p
+00002ff0: 726f 746f 732e 5072 6f63 6573 7352 656e  rotos.ProcessRen
+00003000: 6465 7249 6e66 6f52 0b70 726f 6365 7373  derInfoR.process
+00003010: 496e 666f 0ae0 020a 3070 726f 746f 732f  Info....0protos/
+00003020: 7065 7266 6574 746f 2f6d 6574 7269 6373  perfetto/metrics
+00003030: 2f61 6e64 726f 6964 2f69 6f6e 5f6d 6574  /android/ion_met
+00003040: 7269 632e 7072 6f74 6f12 0f70 6572 6665  ric.proto..perfe
+00003050: 7474 6f2e 7072 6f74 6f73 229a 020a 1041  tto.protos"....A
+00003060: 6e64 726f 6964 496f 6e4d 6574 7269 6312  ndroidIonMetric.
+00003070: 400a 0662 7566 6665 7218 0120 0328 0b32  @..buffer.. .(.2
+00003080: 282e 7065 7266 6574 746f 2e70 726f 746f  (.perfetto.proto
+00003090: 732e 416e 6472 6f69 6449 6f6e 4d65 7472  s.AndroidIonMetr
+000030a0: 6963 2e42 7566 6665 7252 0662 7566 6665  ic.BufferR.buffe
+000030b0: 721a c301 0a06 4275 6666 6572 1212 0a04  r.....Buffer....
+000030c0: 6e61 6d65 1801 2001 2809 5204 6e61 6d65  name.. .(.R.name
+000030d0: 1224 0a0e 6176 675f 7369 7a65 5f62 7974  .$..avg_size_byt
+000030e0: 6573 1802 2001 2801 520c 6176 6753 697a  es.. .(.R.avgSiz
+000030f0: 6542 7974 6573 1224 0a0e 6d69 6e5f 7369  eBytes.$..min_si
+00003100: 7a65 5f62 7974 6573 1803 2001 2801 520c  ze_bytes.. .(.R.
+00003110: 6d69 6e53 697a 6542 7974 6573 1224 0a0e  minSizeBytes.$..
+00003120: 6d61 785f 7369 7a65 5f62 7974 6573 1804  max_size_bytes..
+00003130: 2001 2801 520c 6d61 7853 697a 6542 7974   .(.R.maxSizeByt
+00003140: 6573 1233 0a16 746f 7461 6c5f 616c 6c6f  es.3..total_allo
+00003150: 635f 7369 7a65 5f62 7974 6573 1805 2001  c_size_bytes.. .
+00003160: 2801 5213 746f 7461 6c41 6c6c 6f63 5369  (.R.totalAllocSi
+00003170: 7a65 4279 7465 730a fa05 0a38 7072 6f74  zeBytes....8prot
+00003180: 6f73 2f70 6572 6665 7474 6f2f 6d65 7472  os/perfetto/metr
+00003190: 6963 732f 616e 6472 6f69 642f 6972 715f  ics/android/irq_
+000031a0: 7275 6e74 696d 655f 6d65 7472 6963 2e70  runtime_metric.p
+000031b0: 726f 746f 120f 7065 7266 6574 746f 2e70  roto..perfetto.p
+000031c0: 726f 746f 7322 ac05 0a17 416e 6472 6f69  rotos"....Androi
+000031d0: 6449 7271 5275 6e74 696d 654d 6574 7269  dIrqRuntimeMetri
+000031e0: 6312 500a 0668 775f 6972 7118 0120 0128  c.P..hw_irq.. .(
+000031f0: 0b32 392e 7065 7266 6574 746f 2e70 726f  .29.perfetto.pro
+00003200: 746f 732e 416e 6472 6f69 6449 7271 5275  tos.AndroidIrqRu
+00003210: 6e74 696d 654d 6574 7269 632e 4972 7152  ntimeMetric.IrqR
+00003220: 756e 7469 6d65 4d65 7472 6963 5205 6877  untimeMetricR.hw
+00003230: 4972 7112 500a 0673 775f 6972 7118 0220  Irq.P..sw_irq.. 
+00003240: 0128 0b32 392e 7065 7266 6574 746f 2e70  .(.29.perfetto.p
+00003250: 726f 746f 732e 416e 6472 6f69 6449 7271  rotos.AndroidIrq
+00003260: 5275 6e74 696d 654d 6574 7269 632e 4972  RuntimeMetric.Ir
+00003270: 7152 756e 7469 6d65 4d65 7472 6963 5205  qRuntimeMetricR.
+00003280: 7377 4972 711a 470a 0849 7271 536c 6963  swIrq.G..IrqSlic
+00003290: 6512 190a 0869 7271 5f6e 616d 6518 0120  e....irq_name.. 
+000032a0: 0128 0952 0769 7271 4e61 6d65 120e 0a02  .(.R.irqName....
+000032b0: 7473 1802 2001 2803 5202 7473 1210 0a03  ts.. .(.R.ts....
+000032c0: 6475 7218 0320 0128 0352 0364 7572 1a86  dur.. .(.R.dur..
+000032d0: 010a 0f54 6872 6573 686f 6c64 4d65 7472  ...ThresholdMetr
+000032e0: 6963 121c 0a09 7468 7265 7368 6f6c 6418  ic....threshold.
+000032f0: 0120 0128 0952 0974 6872 6573 686f 6c64  . .(.R.threshold
+00003300: 1230 0a14 6f76 6572 5f74 6872 6573 686f  .0..over_thresho
+00003310: 6c64 5f63 6f75 6e74 1802 2001 2803 5212  ld_count.. .(.R.
+00003320: 6f76 6572 5468 7265 7368 6f6c 6443 6f75  overThresholdCou
+00003330: 6e74 1223 0a0d 616e 6f6d 616c 795f 7261  nt.#..anomaly_ra
+00003340: 7469 6f18 0320 0128 0152 0c61 6e6f 6d61  tio.. .(.R.anoma
+00003350: 6c79 5261 7469 6f1a 9a02 0a10 4972 7152  lyRatio.....IrqR
+00003360: 756e 7469 6d65 4d65 7472 6963 121f 0a0b  untimeMetric....
+00003370: 6d61 785f 7275 6e74 696d 6518 0120 0128  max_runtime.. .(
+00003380: 0352 0a6d 6178 5275 6e74 696d 6512 1f0a  .R.maxRuntime...
+00003390: 0b74 6f74 616c 5f63 6f75 6e74 1802 2001  .total_count.. .
+000033a0: 2803 520a 746f 7461 6c43 6f75 6e74 1263  (.R.totalCount.c
+000033b0: 0a10 7468 7265 7368 6f6c 645f 6d65 7472  ..threshold_metr
+000033c0: 6963 1803 2001 280b 3238 2e70 6572 6665  ic.. .(.28.perfe
+000033d0: 7474 6f2e 7072 6f74 6f73 2e41 6e64 726f  tto.protos.Andro
+000033e0: 6964 4972 7152 756e 7469 6d65 4d65 7472  idIrqRuntimeMetr
+000033f0: 6963 2e54 6872 6573 686f 6c64 4d65 7472  ic.ThresholdMetr
+00003400: 6963 520f 7468 7265 7368 6f6c 644d 6574  icR.thresholdMet
+00003410: 7269 6312 5f0a 126c 6f6e 6765 7374 5f69  ric._..longest_i
+00003420: 7271 5f73 6c69 6365 7318 0420 0328 0b32  rq_slices.. .(.2
+00003430: 312e 7065 7266 6574 746f 2e70 726f 746f  1.perfetto.proto
+00003440: 732e 416e 6472 6f69 6449 7271 5275 6e74  s.AndroidIrqRunt
+00003450: 696d 654d 6574 7269 632e 4972 7153 6c69  imeMetric.IrqSli
+00003460: 6365 5210 6c6f 6e67 6573 7449 7271 536c  ceR.longestIrqSl
+00003470: 6963 6573 0a9c 0e0a 3570 726f 746f 732f  ices....5protos/
+00003480: 7065 7266 6574 746f 2f6d 6574 7269 6373  perfetto/metrics
+00003490: 2f61 6e64 726f 6964 2f6a 616e 6b5f 6375  /android/jank_cu
+000034a0: 6a5f 6d65 7472 6963 2e70 726f 746f 120f  j_metric.proto..
+000034b0: 7065 7266 6574 746f 2e70 726f 746f 731a  perfetto.protos.
+000034c0: 3670 726f 746f 732f 7065 7266 6574 746f  6protos/perfetto
+000034d0: 2f6d 6574 7269 6373 2f61 6e64 726f 6964  /metrics/android
+000034e0: 2f70 726f 6365 7373 5f6d 6574 6164 6174  /process_metadat
+000034f0: 612e 7072 6f74 6f22 990d 0a14 416e 6472  a.proto"....Andr
+00003500: 6f69 644a 616e 6b43 756a 4d65 7472 6963  oidJankCujMetric
+00003510: 123b 0a03 6375 6a18 0120 0328 0b32 292e  .;..cuj.. .(.2).
+00003520: 7065 7266 6574 746f 2e70 726f 746f 732e  perfetto.protos.
+00003530: 416e 6472 6f69 644a 616e 6b43 756a 4d65  AndroidJankCujMe
+00003540: 7472 6963 2e43 756a 5203 6375 6a1a be04  tric.CujR.cuj...
+00003550: 0a03 4375 6a12 0e0a 0269 6418 0120 0128  ..Cuj....id.. .(
+00003560: 0552 0269 6412 120a 046e 616d 6518 0220  .R.id....name.. 
+00003570: 0128 0952 046e 616d 6512 410a 0770 726f  .(.R.name.A..pro
+00003580: 6365 7373 1803 2001 280b 3227 2e70 6572  cess.. .(.2'.per
+00003590: 6665 7474 6f2e 7072 6f74 6f73 2e41 6e64  fetto.protos.And
+000035a0: 726f 6964 5072 6f63 6573 734d 6574 6164  roidProcessMetad
+000035b0: 6174 6152 0770 726f 6365 7373 120e 0a02  ataR.process....
+000035c0: 7473 1804 2001 2803 5202 7473 1210 0a03  ts.. .(.R.ts....
+000035d0: 6475 7218 0520 0128 0352 0364 7572 1241  dur.. .(.R.dur.A
+000035e0: 0a05 6672 616d 6518 0620 0328 0b32 2b2e  ..frame.. .(.2+.
+000035f0: 7065 7266 6574 746f 2e70 726f 746f 732e  perfetto.protos.
+00003600: 416e 6472 6f69 644a 616e 6b43 756a 4d65  AndroidJankCujMe
+00003610: 7472 6963 2e46 7261 6d65 5205 6672 616d  tric.FrameR.fram
+00003620: 6512 460a 0873 665f 6672 616d 6518 0a20  e.F..sf_frame.. 
+00003630: 0328 0b32 2b2e 7065 7266 6574 746f 2e70  .(.2+.perfetto.p
+00003640: 726f 746f 732e 416e 6472 6f69 644a 616e  rotos.AndroidJan
+00003650: 6b43 756a 4d65 7472 6963 2e46 7261 6d65  kCujMetric.Frame
+00003660: 5207 7366 4672 616d 6512 560a 0f63 6f75  R.sfFrame.V..cou
+00003670: 6e74 6572 5f6d 6574 7269 6373 1807 2001  nter_metrics.. .
+00003680: 280b 322d 2e70 6572 6665 7474 6f2e 7072  (.2-.perfetto.pr
+00003690: 6f74 6f73 2e41 6e64 726f 6964 4a61 6e6b  otos.AndroidJank
+000036a0: 4375 6a4d 6574 7269 632e 4d65 7472 6963  CujMetric.Metric
+000036b0: 7352 0e63 6f75 6e74 6572 4d65 7472 6963  sR.counterMetric
+000036c0: 7312 580a 1074 696d 656c 696e 655f 6d65  s.X..timeline_me
+000036d0: 7472 6963 7318 0820 0128 0b32 2d2e 7065  trics.. .(.2-.pe
+000036e0: 7266 6574 746f 2e70 726f 746f 732e 416e  rfetto.protos.An
+000036f0: 6472 6f69 644a 616e 6b43 756a 4d65 7472  droidJankCujMetr
+00003700: 6963 2e4d 6574 7269 6373 520f 7469 6d65  ic.MetricsR.time
+00003710: 6c69 6e65 4d65 7472 6963 7312 520a 0d74  lineMetrics.R..t
+00003720: 7261 6365 5f6d 6574 7269 6373 1809 2001  race_metrics.. .
+00003730: 280b 322d 2e70 6572 6665 7474 6f2e 7072  (.2-.perfetto.pr
+00003740: 6f74 6f73 2e41 6e64 726f 6964 4a61 6e6b  otos.AndroidJank
+00003750: 4375 6a4d 6574 7269 632e 4d65 7472 6963  CujMetric.Metric
+00003760: 7352 0c74 7261 6365 4d65 7472 6963 7312  sR.traceMetrics.
+00003770: 1d0a 0a6c 6179 6572 5f6e 616d 6518 0b20  ...layer_name.. 
+00003780: 0128 0952 096c 6179 6572 4e61 6d65 1aa1  .(.R.layerName..
+00003790: 020a 0546 7261 6d65 1221 0a0c 6672 616d  ...Frame.!..fram
+000037a0: 655f 6e75 6d62 6572 1801 2001 2803 520b  e_number.. .(.R.
+000037b0: 6672 616d 654e 756d 6265 7212 140a 0576  frameNumber....v
+000037c0: 7379 6e63 1802 2001 2803 5205 7673 796e  sync.. .(.R.vsyn
+000037d0: 6312 0e0a 0274 7318 0320 0128 0352 0274  c....ts.. .(.R.t
+000037e0: 7312 100a 0364 7572 1804 2001 2803 5203  s....dur.. .(.R.
+000037f0: 6475 7212 210a 0c64 7572 5f65 7870 6563  dur.!..dur_expec
+00003800: 7465 6418 0720 0128 0352 0b64 7572 4578  ted.. .(.R.durEx
+00003810: 7065 6374 6564 121d 0a0a 6170 705f 6d69  pected....app_mi
+00003820: 7373 6564 1805 2001 2808 5209 6170 704d  ssed.. .(.R.appM
+00003830: 6973 7365 6412 1b0a 0973 665f 6d69 7373  issed....sf_miss
+00003840: 6564 1806 2001 2808 5208 7366 4d69 7373  ed.. .(.R.sfMiss
+00003850: 6564 122c 0a12 7366 5f63 616c 6c62 6163  ed.,..sf_callbac
+00003860: 6b5f 6d69 7373 6564 1808 2001 2808 5210  k_missed.. .(.R.
+00003870: 7366 4361 6c6c 6261 636b 4d69 7373 6564  sfCallbackMissed
+00003880: 1230 0a14 6877 7569 5f63 616c 6c62 6163  .0..hwui_callbac
+00003890: 6b5f 6d69 7373 6564 1809 2001 2808 5212  k_missed.. .(.R.
+000038a0: 6877 7569 4361 6c6c 6261 636b 4d69 7373  hwuiCallbackMiss
+000038b0: 6564 1ade 050a 074d 6574 7269 6373 1221  ed.....Metrics.!
+000038c0: 0a0c 746f 7461 6c5f 6672 616d 6573 1801  ..total_frames..
+000038d0: 2001 2803 520b 746f 7461 6c46 7261 6d65   .(.R.totalFrame
+000038e0: 7312 230a 0d6d 6973 7365 645f 6672 616d  s.#..missed_fram
+000038f0: 6573 1802 2001 2803 520c 6d69 7373 6564  es.. .(.R.missed
+00003900: 4672 616d 6573 122a 0a11 6d69 7373 6564  Frames.*..missed
+00003910: 5f61 7070 5f66 7261 6d65 7318 0320 0128  _app_frames.. .(
+00003920: 0352 0f6d 6973 7365 6441 7070 4672 616d  .R.missedAppFram
+00003930: 6573 1228 0a10 6d69 7373 6564 5f73 665f  es.(..missed_sf_
+00003940: 6672 616d 6573 1804 2001 2803 520e 6d69  frames.. .(.R.mi
+00003950: 7373 6564 5366 4672 616d 6573 123f 0a1c  ssedSfFrames.?..
+00003960: 6d69 7373 6564 5f66 7261 6d65 735f 6d61  missed_frames_ma
+00003970: 785f 7375 6363 6573 7369 7665 1805 2001  x_successive.. .
+00003980: 2803 5219 6d69 7373 6564 4672 616d 6573  (.R.missedFrames
+00003990: 4d61 7853 7563 6365 7373 6976 6512 220a  MaxSuccessive.".
+000039a0: 0d66 7261 6d65 5f64 7572 5f6d 6178 1806  .frame_dur_max..
+000039b0: 2001 2803 520b 6672 616d 6544 7572 4d61   .(.R.frameDurMa
+000039c0: 7812 220a 0d66 7261 6d65 5f64 7572 5f61  x."..frame_dur_a
+000039d0: 7667 1807 2001 2803 520b 6672 616d 6544  vg.. .(.R.frameD
+000039e0: 7572 4176 6712 220a 0d66 7261 6d65 5f64  urAvg."..frame_d
+000039f0: 7572 5f70 3530 1808 2001 2803 520b 6672  ur_p50.. .(.R.fr
+00003a00: 616d 6544 7572 5035 3012 220a 0d66 7261  ameDurP50."..fra
+00003a10: 6d65 5f64 7572 5f70 3930 1809 2001 2803  me_dur_p90.. .(.
+00003a20: 520b 6672 616d 6544 7572 5039 3012 220a  R.frameDurP90.".
+00003a30: 0d66 7261 6d65 5f64 7572 5f70 3935 180a  .frame_dur_p95..
+00003a40: 2001 2803 520b 6672 616d 6544 7572 5039   .(.R.frameDurP9
+00003a50: 3512 220a 0d66 7261 6d65 5f64 7572 5f70  5."..frame_dur_p
+00003a60: 3939 180b 2001 2803 520b 6672 616d 6544  99.. .(.R.frameD
+00003a70: 7572 5039 3912 270a 1066 7261 6d65 5f64  urP99.'..frame_d
+00003a80: 7572 5f6d 735f 7035 3018 0c20 0128 0152  ur_ms_p50.. .(.R
+00003a90: 0d66 7261 6d65 4475 724d 7350 3530 1227  .frameDurMsP50.'
+00003aa0: 0a10 6672 616d 655f 6475 725f 6d73 5f70  ..frame_dur_ms_p
+00003ab0: 3930 180d 2001 2801 520d 6672 616d 6544  90.. .(.R.frameD
+00003ac0: 7572 4d73 5039 3012 270a 1066 7261 6d65  urMsP90.'..frame
+00003ad0: 5f64 7572 5f6d 735f 7039 3518 0e20 0128  _dur_ms_p95.. .(
+00003ae0: 0152 0d66 7261 6d65 4475 724d 7350 3935  .R.frameDurMsP95
+00003af0: 1227 0a10 6672 616d 655f 6475 725f 6d73  .'..frame_dur_ms
+00003b00: 5f70 3939 180f 2001 2801 520d 6672 616d  _p99.. .(.R.fram
+00003b10: 6544 7572 4d73 5039 3912 390a 1973 665f  eDurMsP99.9..sf_
+00003b20: 6361 6c6c 6261 636b 5f6d 6973 7365 645f  callback_missed_
+00003b30: 6672 616d 6573 1810 2001 2803 5216 7366  frames.. .(.R.sf
+00003b40: 4361 6c6c 6261 636b 4d69 7373 6564 4672  CallbackMissedFr
+00003b50: 616d 6573 123d 0a1b 6877 7569 5f63 616c  ames.=..hwui_cal
+00003b60: 6c62 6163 6b5f 6d69 7373 6564 5f66 7261  lback_missed_fra
+00003b70: 6d65 7318 1120 0128 0352 1868 7775 6943  mes.. .(.R.hwuiC
+00003b80: 616c 6c62 6163 6b4d 6973 7365 6446 7261  allbackMissedFra
+00003b90: 6d65 730a c006 0a39 7072 6f74 6f73 2f70  mes....9protos/p
+00003ba0: 6572 6665 7474 6f2f 6d65 7472 6963 732f  erfetto/metrics/
+00003bb0: 616e 6472 6f69 642f 6a61 7661 5f68 6561  android/java_hea
+00003bc0: 705f 6869 7374 6f67 7261 6d2e 7072 6f74  p_histogram.prot
+00003bd0: 6f12 0f70 6572 6665 7474 6f2e 7072 6f74  o..perfetto.prot
+00003be0: 6f73 1a36 7072 6f74 6f73 2f70 6572 6665  os.6protos/perfe
+00003bf0: 7474 6f2f 6d65 7472 6963 732f 616e 6472  tto/metrics/andr
+00003c00: 6f69 642f 7072 6f63 6573 735f 6d65 7461  oid/process_meta
+00003c10: 6461 7461 2e70 726f 746f 22b9 050a 114a  data.proto"....J
+00003c20: 6176 6148 6561 7048 6973 746f 6772 616d  avaHeapHistogram
+00003c30: 1257 0a0e 696e 7374 616e 6365 5f73 7461  .W..instance_sta
+00003c40: 7473 1801 2003 280b 3230 2e70 6572 6665  ts.. .(.20.perfe
+00003c50: 7474 6f2e 7072 6f74 6f73 2e4a 6176 6148  tto.protos.JavaH
+00003c60: 6561 7048 6973 746f 6772 616d 2e49 6e73  eapHistogram.Ins
+00003c70: 7461 6e63 6553 7461 7473 520d 696e 7374  tanceStatsR.inst
+00003c80: 616e 6365 5374 6174 731a b502 0a09 5479  anceStats.....Ty
+00003c90: 7065 436f 756e 7412 1b0a 0974 7970 655f  peCount....type_
+00003ca0: 6e61 6d65 1801 2001 2809 5208 7479 7065  name.. .(.R.type
+00003cb0: 4e61 6d65 121a 0a08 6361 7465 676f 7279  Name....category
+00003cc0: 1804 2001 2809 5208 6361 7465 676f 7279  .. .(.R.category
+00003cd0: 121b 0a09 6f62 6a5f 636f 756e 7418 0220  ....obj_count.. 
+00003ce0: 0128 0d52 086f 626a 436f 756e 7412 2e0a  .(.R.objCount...
+00003cf0: 1372 6561 6368 6162 6c65 5f6f 626a 5f63  .reachable_obj_c
+00003d00: 6f75 6e74 1803 2001 280d 5211 7265 6163  ount.. .(.R.reac
+00003d10: 6861 626c 654f 626a 436f 756e 7412 170a  hableObjCount...
+00003d20: 0773 697a 655f 6b62 1805 2001 280d 5206  .size_kb.. .(.R.
+00003d30: 7369 7a65 4b62 122a 0a11 7265 6163 6861  sizeKb.*..reacha
+00003d40: 626c 655f 7369 7a65 5f6b 6218 0620 0128  ble_size_kb.. .(
+00003d50: 0d52 0f72 6561 6368 6162 6c65 5369 7a65  .R.reachableSize
+00003d60: 4b62 1224 0a0e 6e61 7469 7665 5f73 697a  Kb.$..native_siz
+00003d70: 655f 6b62 1807 2001 280d 520c 6e61 7469  e_kb.. .(.R.nati
+00003d80: 7665 5369 7a65 4b62 1237 0a18 7265 6163  veSizeKb.7..reac
+00003d90: 6861 626c 655f 6e61 7469 7665 5f73 697a  hable_native_siz
+00003da0: 655f 6b62 1808 2001 280d 5215 7265 6163  e_kb.. .(.R.reac
+00003db0: 6861 626c 654e 6174 6976 6553 697a 654b  hableNativeSizeK
+00003dc0: 621a 650a 0653 616d 706c 6512 0e0a 0274  b.e..Sample....t
+00003dd0: 7318 0120 0128 0352 0274 7312 4b0a 0a74  s.. .(.R.ts.K..t
+00003de0: 7970 655f 636f 756e 7418 0220 0328 0b32  ype_count.. .(.2
+00003df0: 2c2e 7065 7266 6574 746f 2e70 726f 746f  ,.perfetto.proto
+00003e00: 732e 4a61 7661 4865 6170 4869 7374 6f67  s.JavaHeapHistog
+00003e10: 7261 6d2e 5479 7065 436f 756e 7452 0974  ram.TypeCountR.t
+00003e20: 7970 6543 6f75 6e74 1aab 010a 0d49 6e73  ypeCount.....Ins
+00003e30: 7461 6e63 6553 7461 7473 1212 0a04 7570  tanceStats....up
+00003e40: 6964 1801 2001 280d 5204 7570 6964 1241  id.. .(.R.upid.A
+00003e50: 0a07 7072 6f63 6573 7318 0220 0128 0b32  ..process.. .(.2
+00003e60: 272e 7065 7266 6574 746f 2e70 726f 746f  '.perfetto.proto
+00003e70: 732e 416e 6472 6f69 6450 726f 6365 7373  s.AndroidProcess
+00003e80: 4d65 7461 6461 7461 5207 7072 6f63 6573  MetadataR.proces
+00003e90: 7312 430a 0773 616d 706c 6573 1803 2003  s.C..samples.. .
+00003ea0: 280b 3229 2e70 6572 6665 7474 6f2e 7072  (.2).perfetto.pr
+00003eb0: 6f74 6f73 2e4a 6176 6148 6561 7048 6973  otos.JavaHeapHis
+00003ec0: 746f 6772 616d 2e53 616d 706c 6552 0773  togram.SampleR.s
+00003ed0: 616d 706c 6573 0aa9 070a 3570 726f 746f  amples....5proto
+00003ee0: 732f 7065 7266 6574 746f 2f6d 6574 7269  s/perfetto/metri
+00003ef0: 6373 2f61 6e64 726f 6964 2f6a 6176 615f  cs/android/java_
+00003f00: 6865 6170 5f73 7461 7473 2e70 726f 746f  heap_stats.proto
+00003f10: 120f 7065 7266 6574 746f 2e70 726f 746f  ..perfetto.proto
+00003f20: 731a 3670 726f 746f 732f 7065 7266 6574  s.6protos/perfet
+00003f30: 746f 2f6d 6574 7269 6373 2f61 6e64 726f  to/metrics/andro
+00003f40: 6964 2f70 726f 6365 7373 5f6d 6574 6164  id/process_metad
+00003f50: 6174 612e 7072 6f74 6f22 a606 0a0d 4a61  ata.proto"....Ja
+00003f60: 7661 4865 6170 5374 6174 7312 530a 0e69  vaHeapStats.S..i
+00003f70: 6e73 7461 6e63 655f 7374 6174 7318 0120  nstance_stats.. 
+00003f80: 0328 0b32 2c2e 7065 7266 6574 746f 2e70  .(.2,.perfetto.p
+00003f90: 726f 746f 732e 4a61 7661 4865 6170 5374  rotos.JavaHeapSt
+00003fa0: 6174 732e 496e 7374 616e 6365 5374 6174  ats.InstanceStat
+00003fb0: 7352 0d69 6e73 7461 6e63 6553 7461 7473  sR.instanceStats
+00003fc0: 1a62 0a09 4865 6170 526f 6f74 7312 1b0a  .b..HeapRoots...
+00003fd0: 0972 6f6f 745f 7479 7065 1801 2001 2809  .root_type.. .(.
+00003fe0: 5208 726f 6f74 5479 7065 121b 0a09 7479  R.rootType....ty
+00003ff0: 7065 5f6e 616d 6518 0220 0128 0952 0874  pe_name.. .(.R.t
+00004000: 7970 654e 616d 6512 1b0a 096f 626a 5f63  ypeName....obj_c
+00004010: 6f75 6e74 1803 2001 2803 5208 6f62 6a43  ount.. .(.R.objC
+00004020: 6f75 6e74 1ab1 030a 0653 616d 706c 6512  ount.....Sample.
+00004030: 0e0a 0274 7318 0120 0128 0352 0274 7312  ...ts.. .(.R.ts.
+00004040: 1b0a 0968 6561 705f 7369 7a65 1802 2001  ...heap_size.. .
+00004050: 2803 5208 6865 6170 5369 7a65 1228 0a10  (.R.heapSize.(..
+00004060: 6865 6170 5f6e 6174 6976 655f 7369 7a65  heap_native_size
+00004070: 1808 2001 2803 520e 6865 6170 4e61 7469  .. .(.R.heapNati
+00004080: 7665 5369 7a65 121b 0a09 6f62 6a5f 636f  veSize....obj_co
+00004090: 756e 7418 0420 0128 0352 086f 626a 436f  unt.. .(.R.objCo
+000040a0: 756e 7412 2e0a 1372 6561 6368 6162 6c65  unt....reachable
+000040b0: 5f68 6561 705f 7369 7a65 1803 2001 2803  _heap_size.. .(.
+000040c0: 5211 7265 6163 6861 626c 6548 6561 7053  R.reachableHeapS
+000040d0: 697a 6512 3b0a 1a72 6561 6368 6162 6c65  ize.;..reachable
+000040e0: 5f68 6561 705f 6e61 7469 7665 5f73 697a  _heap_native_siz
+000040f0: 6518 0920 0128 0352 1772 6561 6368 6162  e.. .(.R.reachab
+00004100: 6c65 4865 6170 4e61 7469 7665 5369 7a65  leHeapNativeSize
+00004110: 122e 0a13 7265 6163 6861 626c 655f 6f62  ....reachable_ob
+00004120: 6a5f 636f 756e 7418 0520 0128 0352 1172  j_count.. .(.R.r
+00004130: 6561 6368 6162 6c65 4f62 6a43 6f75 6e74  eachableObjCount
+00004140: 1232 0a16 616e 6f6e 5f72 7373 5f61 6e64  .2..anon_rss_and
+00004150: 5f73 7761 705f 7369 7a65 1806 2001 2803  _swap_size.. .(.
+00004160: 5212 616e 6f6e 5273 7341 6e64 5377 6170  R.anonRssAndSwap
+00004170: 5369 7a65 123e 0a05 726f 6f74 7318 0720  Size.>..roots.. 
+00004180: 0328 0b32 282e 7065 7266 6574 746f 2e70  .(.2(.perfetto.p
+00004190: 726f 746f 732e 4a61 7661 4865 6170 5374  rotos.JavaHeapSt
+000041a0: 6174 732e 4865 6170 526f 6f74 7352 0572  ats.HeapRootsR.r
+000041b0: 6f6f 7473 1222 0a0d 6f6f 6d5f 7363 6f72  oots."..oom_scor
+000041c0: 655f 6164 6a18 0a20 0128 0352 0b6f 6f6d  e_adj.. .(.R.oom
+000041d0: 5363 6f72 6541 646a 1aa7 010a 0d49 6e73  ScoreAdj.....Ins
+000041e0: 7461 6e63 6553 7461 7473 1212 0a04 7570  tanceStats....up
+000041f0: 6964 1801 2001 280d 5204 7570 6964 1241  id.. .(.R.upid.A
+00004200: 0a07 7072 6f63 6573 7318 0220 0128 0b32  ..process.. .(.2
+00004210: 272e 7065 7266 6574 746f 2e70 726f 746f  '.perfetto.proto
+00004220: 732e 416e 6472 6f69 6450 726f 6365 7373  s.AndroidProcess
+00004230: 4d65 7461 6461 7461 5207 7072 6f63 6573  MetadataR.proces
+00004240: 7312 3f0a 0773 616d 706c 6573 1803 2003  s.?..samples.. .
+00004250: 280b 3225 2e70 6572 6665 7474 6f2e 7072  (.2%.perfetto.pr
+00004260: 6f74 6f73 2e4a 6176 6148 6561 7053 7461  otos.JavaHeapSta
+00004270: 7473 2e53 616d 706c 6552 0773 616d 706c  ts.SampleR.sampl
+00004280: 6573 0abb 020a 3070 726f 746f 732f 7065  es....0protos/pe
+00004290: 7266 6574 746f 2f6d 6574 7269 6373 2f61  rfetto/metrics/a
+000042a0: 6e64 726f 6964 2f6c 6d6b 5f6d 6574 7269  ndroid/lmk_metri
+000042b0: 632e 7072 6f74 6f12 0f70 6572 6665 7474  c.proto..perfett
+000042c0: 6f2e 7072 6f74 6f73 22f5 010a 1041 6e64  o.protos"....And
+000042d0: 726f 6964 4c6d 6b4d 6574 7269 6312 1f0a  roidLmkMetric...
+000042e0: 0b74 6f74 616c 5f63 6f75 6e74 1801 2001  .total_count.. .
+000042f0: 2805 520a 746f 7461 6c43 6f75 6e74 124e  (.R.totalCount.N
+00004300: 0a0c 6279 5f6f 6f6d 5f73 636f 7265 1802  ..by_oom_score..
+00004310: 2003 280b 322c 2e70 6572 6665 7474 6f2e   .(.2,.perfetto.
+00004320: 7072 6f74 6f73 2e41 6e64 726f 6964 4c6d  protos.AndroidLm
+00004330: 6b4d 6574 7269 632e 4279 4f6f 6d53 636f  kMetric.ByOomSco
+00004340: 7265 520a 6279 4f6f 6d53 636f 7265 1228  reR.byOomScore.(
+00004350: 0a10 6f6f 6d5f 7669 6374 696d 5f63 6f75  ..oom_victim_cou
+00004360: 6e74 1803 2001 2805 520e 6f6f 6d56 6963  nt.. .(.R.oomVic
+00004370: 7469 6d43 6f75 6e74 1a46 0a0a 4279 4f6f  timCount.F..ByOo
+00004380: 6d53 636f 7265 1222 0a0d 6f6f 6d5f 7363  mScore."..oom_sc
+00004390: 6f72 655f 6164 6a18 0120 0128 0552 0b6f  ore_adj.. .(.R.o
+000043a0: 6f6d 5363 6f72 6541 646a 1214 0a05 636f  omScoreAdj....co
+000043b0: 756e 7418 0220 0128 0552 0563 6f75 6e74  unt.. .(.R.count
+000043c0: 0acc 050a 3770 726f 746f 732f 7065 7266  ....7protos/perf
+000043d0: 6574 746f 2f6d 6574 7269 6373 2f61 6e64  etto/metrics/and
+000043e0: 726f 6964 2f6c 6d6b 5f72 6561 736f 6e5f  roid/lmk_reason_
+000043f0: 6d65 7472 6963 2e70 726f 746f 120f 7065  metric.proto..pe
+00004400: 7266 6574 746f 2e70 726f 746f 731a 3670  rfetto.protos.6p
+00004410: 726f 746f 732f 7065 7266 6574 746f 2f6d  rotos/perfetto/m
+00004420: 6574 7269 6373 2f61 6e64 726f 6964 2f70  etrics/android/p
+00004430: 726f 6365 7373 5f6d 6574 6164 6174 612e  rocess_metadata.
+00004440: 7072 6f74 6f22 c704 0a16 416e 6472 6f69  proto"....Androi
+00004450: 644c 6d6b 5265 6173 6f6e 4d65 7472 6963  dLmkReasonMetric
+00004460: 123f 0a04 6c6d 6b73 1801 2003 280b 322b  .?..lmks.. .(.2+
+00004470: 2e70 6572 6665 7474 6f2e 7072 6f74 6f73  .perfetto.protos
+00004480: 2e41 6e64 726f 6964 4c6d 6b52 6561 736f  .AndroidLmkReaso
+00004490: 6e4d 6574 7269 632e 4c6d 6b52 046c 6d6b  nMetric.LmkR.lmk
+000044a0: 731a 9702 0a07 5072 6f63 6573 7312 410a  s.....Process.A.
+000044b0: 0770 726f 6365 7373 1801 2001 280b 3227  .process.. .(.2'
+000044c0: 2e70 6572 6665 7474 6f2e 7072 6f74 6f73  .perfetto.protos
+000044d0: 2e41 6e64 726f 6964 5072 6f63 6573 734d  .AndroidProcessM
+000044e0: 6574 6164 6174 6152 0770 726f 6365 7373  etadataR.process
+000044f0: 1222 0a0d 6f6f 6d5f 7363 6f72 655f 6164  ."..oom_score_ad
+00004500: 6a18 0220 0128 0552 0b6f 6f6d 5363 6f72  j.. .(.R.oomScor
+00004510: 6541 646a 1212 0a04 7369 7a65 1803 2001  eAdj....size.. .
+00004520: 2803 5204 7369 7a65 1224 0a0e 6669 6c65  (.R.size.$..file
+00004530: 5f72 7373 5f62 7974 6573 1804 2001 2803  _rss_bytes.. .(.
+00004540: 520c 6669 6c65 5273 7342 7974 6573 1224  R.fileRssBytes.$
+00004550: 0a0e 616e 6f6e 5f72 7373 5f62 7974 6573  ..anon_rss_bytes
+00004560: 1805 2001 2803 520c 616e 6f6e 5273 7342  .. .(.R.anonRssB
+00004570: 7974 6573 1226 0a0f 7368 6d65 6d5f 7273  ytes.&..shmem_rs
+00004580: 735f 6279 7465 7318 0620 0128 0352 0d73  s_bytes.. .(.R.s
+00004590: 686d 656d 5273 7342 7974 6573 121d 0a0a  hmemRssBytes....
+000045a0: 7377 6170 5f62 7974 6573 1807 2001 2803  swap_bytes.. .(.
+000045b0: 5209 7377 6170 4279 7465 731a d101 0a03  R.swapBytes.....
+000045c0: 4c6d 6b12 220a 0d6f 6f6d 5f73 636f 7265  Lmk."..oom_score
+000045d0: 5f61 646a 1801 2001 2805 520b 6f6f 6d53  _adj.. .(.R.oomS
+000045e0: 636f 7265 4164 6a12 260a 0f69 6f6e 5f68  coreAdj.&..ion_h
+000045f0: 6561 7073 5f62 7974 6573 1804 2001 2803  eaps_bytes.. .(.
+00004600: 520d 696f 6e48 6561 7073 4279 7465 7312  R.ionHeapsBytes.
+00004610: 2f0a 1473 7973 7465 6d5f 696f 6e5f 6865  /..system_ion_he
+00004620: 6170 5f73 697a 6518 0220 0128 0352 1173  ap_size.. .(.R.s
+00004630: 7973 7465 6d49 6f6e 4865 6170 5369 7a65  ystemIonHeapSize
+00004640: 124d 0a09 7072 6f63 6573 7365 7318 0320  .M..processes.. 
+00004650: 0328 0b32 2f2e 7065 7266 6574 746f 2e70  .(.2/.perfetto.p
+00004660: 726f 746f 732e 416e 6472 6f69 644c 6d6b  rotos.AndroidLmk
+00004670: 5265 6173 6f6e 4d65 7472 6963 2e50 726f  ReasonMetric.Pro
+00004680: 6365 7373 5209 7072 6f63 6573 7365 730a  cessR.processes.
+00004690: a508 0a30 7072 6f74 6f73 2f70 6572 6665  ...0protos/perfe
+000046a0: 7474 6f2f 6d65 7472 6963 732f 616e 6472  tto/metrics/andr
+000046b0: 6f69 642f 6d65 6d5f 6d65 7472 6963 2e70  oid/mem_metric.p
+000046c0: 726f 746f 120f 7065 7266 6574 746f 2e70  roto..perfetto.p
+000046d0: 726f 746f 7322 df07 0a13 416e 6472 6f69  rotos"....Androi
+000046e0: 644d 656d 6f72 794d 6574 7269 6312 5c0a  dMemoryMetric.\.
+000046f0: 0f70 726f 6365 7373 5f6d 6574 7269 6373  .process_metrics
+00004700: 1801 2003 280b 3233 2e70 6572 6665 7474  .. .(.23.perfett
+00004710: 6f2e 7072 6f74 6f73 2e41 6e64 726f 6964  o.protos.Android
+00004720: 4d65 6d6f 7279 4d65 7472 6963 2e50 726f  MemoryMetric.Pro
+00004730: 6365 7373 4d65 7472 6963 7352 0e70 726f  cessMetricsR.pro
+00004740: 6365 7373 4d65 7472 6963 731a fd01 0a0e  cessMetrics.....
+00004750: 5072 6f63 6573 734d 6574 7269 6373 1221  ProcessMetrics.!
+00004760: 0a0c 7072 6f63 6573 735f 6e61 6d65 1801  ..process_name..
+00004770: 2001 2809 520b 7072 6f63 6573 734e 616d   .(.R.processNam
+00004780: 6512 610a 0e74 6f74 616c 5f63 6f75 6e74  e.a..total_count
+00004790: 6572 7318 0220 0128 0b32 3a2e 7065 7266  ers.. .(.2:.perf
+000047a0: 6574 746f 2e70 726f 746f 732e 416e 6472  etto.protos.Andr
+000047b0: 6f69 644d 656d 6f72 794d 6574 7269 632e  oidMemoryMetric.
+000047c0: 5072 6f63 6573 734d 656d 6f72 7943 6f75  ProcessMemoryCou
+000047d0: 6e74 6572 7352 0d74 6f74 616c 436f 756e  ntersR.totalCoun
+000047e0: 7465 7273 1265 0a12 7072 696f 7269 7479  ters.e..priority
+000047f0: 5f62 7265 616b 646f 776e 1803 2003 280b  _breakdown.. .(.
+00004800: 3236 2e70 6572 6665 7474 6f2e 7072 6f74  26.perfetto.prot
+00004810: 6f73 2e41 6e64 726f 6964 4d65 6d6f 7279  os.AndroidMemory
+00004820: 4d65 7472 6963 2e50 7269 6f72 6974 7942  Metric.PriorityB
+00004830: 7265 616b 646f 776e 5211 7072 696f 7269  reakdownR.priori
+00004840: 7479 4272 6561 6b64 6f77 6e1a 8701 0a11  tyBreakdown.....
+00004850: 5072 696f 7269 7479 4272 6561 6b64 6f77  PriorityBreakdow
+00004860: 6e12 1a0a 0870 7269 6f72 6974 7918 0120  n....priority.. 
+00004870: 0128 0952 0870 7269 6f72 6974 7912 560a  .(.R.priority.V.
+00004880: 0863 6f75 6e74 6572 7318 0220 0128 0b32  .counters.. .(.2
+00004890: 3a2e 7065 7266 6574 746f 2e70 726f 746f  :.perfetto.proto
+000048a0: 732e 416e 6472 6f69 644d 656d 6f72 794d  s.AndroidMemoryM
+000048b0: 6574 7269 632e 5072 6f63 6573 734d 656d  etric.ProcessMem
+000048c0: 6f72 7943 6f75 6e74 6572 7352 0863 6f75  oryCountersR.cou
+000048d0: 6e74 6572 731a 8803 0a15 5072 6f63 6573  nters.....Proces
+000048e0: 734d 656d 6f72 7943 6f75 6e74 6572 7312  sMemoryCounters.
+000048f0: 470a 0861 6e6f 6e5f 7273 7318 0120 0128  G..anon_rss.. .(
+00004900: 0b32 2c2e 7065 7266 6574 746f 2e70 726f  .2,.perfetto.pro
+00004910: 746f 732e 416e 6472 6f69 644d 656d 6f72  tos.AndroidMemor
+00004920: 794d 6574 7269 632e 436f 756e 7465 7252  yMetric.CounterR
+00004930: 0761 6e6f 6e52 7373 1247 0a08 6669 6c65  .anonRss.G..file
+00004940: 5f72 7373 1802 2001 280b 322c 2e70 6572  _rss.. .(.2,.per
+00004950: 6665 7474 6f2e 7072 6f74 6f73 2e41 6e64  fetto.protos.And
+00004960: 726f 6964 4d65 6d6f 7279 4d65 7472 6963  roidMemoryMetric
+00004970: 2e43 6f75 6e74 6572 5207 6669 6c65 5273  .CounterR.fileRs
+00004980: 7312 400a 0473 7761 7018 0320 0128 0b32  s.@..swap.. .(.2
+00004990: 2c2e 7065 7266 6574 746f 2e70 726f 746f  ,.perfetto.proto
+000049a0: 732e 416e 6472 6f69 644d 656d 6f72 794d  s.AndroidMemoryM
+000049b0: 6574 7269 632e 436f 756e 7465 7252 0473  etric.CounterR.s
+000049c0: 7761 7012 500a 0d61 6e6f 6e5f 616e 645f  wap.P..anon_and_
+000049d0: 7377 6170 1804 2001 280b 322c 2e70 6572  swap.. .(.2,.per
+000049e0: 6665 7474 6f2e 7072 6f74 6f73 2e41 6e64  fetto.protos.And
+000049f0: 726f 6964 4d65 6d6f 7279 4d65 7472 6963  roidMemoryMetric
+00004a00: 2e43 6f75 6e74 6572 520b 616e 6f6e 416e  .CounterR.anonAn
+00004a10: 6453 7761 7012 490a 096a 6176 615f 6865  dSwap.I..java_he
+00004a20: 6170 1805 2001 280b 322c 2e70 6572 6665  ap.. .(.2,.perfe
+00004a30: 7474 6f2e 7072 6f74 6f73 2e41 6e64 726f  tto.protos.Andro
+00004a40: 6964 4d65 6d6f 7279 4d65 7472 6963 2e43  idMemoryMetric.C
+00004a50: 6f75 6e74 6572 5208 6a61 7661 4865 6170  ounterR.javaHeap
+00004a60: 1a55 0a07 436f 756e 7465 7212 100a 036d  .U..Counter....m
+00004a70: 696e 1801 2001 2801 5203 6d69 6e12 100a  in.. .(.R.min...
+00004a80: 036d 6178 1802 2001 2801 5203 6d61 7812  .max.. .(.R.max.
+00004a90: 100a 0361 7667 1803 2001 2801 5203 6176  ...avg.. .(.R.av
+00004aa0: 6712 140a 0564 656c 7461 1804 2001 2801  g....delta.. .(.
+00004ab0: 5205 6465 6c74 610a a006 0a36 7072 6f74  R.delta....6prot
+00004ac0: 6f73 2f70 6572 6665 7474 6f2f 6d65 7472  os/perfetto/metr
+00004ad0: 6963 732f 616e 6472 6f69 642f 6d65 6d5f  ics/android/mem_
+00004ae0: 756e 6167 675f 6d65 7472 6963 2e70 726f  unagg_metric.pro
+00004af0: 746f 120f 7065 7266 6574 746f 2e70 726f  to..perfetto.pro
+00004b00: 746f 7322 d405 0a1f 416e 6472 6f69 644d  tos"....AndroidM
+00004b10: 656d 6f72 7955 6e61 6767 7265 6761 7465  emoryUnaggregate
+00004b20: 644d 6574 7269 6312 650a 0e70 726f 6365  dMetric.e..proce
+00004b30: 7373 5f76 616c 7565 7318 0120 0328 0b32  ss_values.. .(.2
+00004b40: 3e2e 7065 7266 6574 746f 2e70 726f 746f  >.perfetto.proto
+00004b50: 732e 416e 6472 6f69 644d 656d 6f72 7955  s.AndroidMemoryU
+00004b60: 6e61 6767 7265 6761 7465 644d 6574 7269  naggregatedMetri
+00004b70: 632e 5072 6f63 6573 7356 616c 7565 7352  c.ProcessValuesR
+00004b80: 0d70 726f 6365 7373 5661 6c75 6573 1a97  .processValues..
+00004b90: 010a 0d50 726f 6365 7373 5661 6c75 6573  ...ProcessValues
+00004ba0: 1221 0a0c 7072 6f63 6573 735f 6e61 6d65  .!..process_name
+00004bb0: 1801 2001 2809 520b 7072 6f63 6573 734e  .. .(.R.processN
+00004bc0: 616d 6512 630a 0a6d 656d 5f76 616c 7565  ame.c..mem_value
+00004bd0: 7318 0220 0128 0b32 442e 7065 7266 6574  s.. .(.2D.perfet
+00004be0: 746f 2e70 726f 746f 732e 416e 6472 6f69  to.protos.Androi
+00004bf0: 644d 656d 6f72 7955 6e61 6767 7265 6761  dMemoryUnaggrega
+00004c00: 7465 644d 6574 7269 632e 5072 6f63 6573  tedMetric.Proces
+00004c10: 734d 656d 6f72 7956 616c 7565 7352 096d  sMemoryValuesR.m
+00004c20: 656d 5661 6c75 6573 1ae3 020a 1350 726f  emValues.....Pro
+00004c30: 6365 7373 4d65 6d6f 7279 5661 6c75 6573  cessMemoryValues
+00004c40: 1251 0a08 616e 6f6e 5f72 7373 1801 2003  .Q..anon_rss.. .
+00004c50: 280b 3236 2e70 6572 6665 7474 6f2e 7072  (.26.perfetto.pr
+00004c60: 6f74 6f73 2e41 6e64 726f 6964 4d65 6d6f  otos.AndroidMemo
+00004c70: 7279 556e 6167 6772 6567 6174 6564 4d65  ryUnaggregatedMe
+00004c80: 7472 6963 2e56 616c 7565 5207 616e 6f6e  tric.ValueR.anon
+00004c90: 5273 7312 510a 0866 696c 655f 7273 7318  Rss.Q..file_rss.
+00004ca0: 0220 0328 0b32 362e 7065 7266 6574 746f  . .(.26.perfetto
+00004cb0: 2e70 726f 746f 732e 416e 6472 6f69 644d  .protos.AndroidM
+00004cc0: 656d 6f72 7955 6e61 6767 7265 6761 7465  emoryUnaggregate
+00004cd0: 644d 6574 7269 632e 5661 6c75 6552 0766  dMetric.ValueR.f
+00004ce0: 696c 6552 7373 124a 0a04 7377 6170 1803  ileRss.J..swap..
+00004cf0: 2003 280b 3236 2e70 6572 6665 7474 6f2e   .(.26.perfetto.
+00004d00: 7072 6f74 6f73 2e41 6e64 726f 6964 4d65  protos.AndroidMe
+00004d10: 6d6f 7279 556e 6167 6772 6567 6174 6564  moryUnaggregated
+00004d20: 4d65 7472 6963 2e56 616c 7565 5204 7377  Metric.ValueR.sw
+00004d30: 6170 125a 0a0d 616e 6f6e 5f61 6e64 5f73  ap.Z..anon_and_s
+00004d40: 7761 7018 0420 0328 0b32 362e 7065 7266  wap.. .(.26.perf
+00004d50: 6574 746f 2e70 726f 746f 732e 416e 6472  etto.protos.Andr
+00004d60: 6f69 644d 656d 6f72 7955 6e61 6767 7265  oidMemoryUnaggre
+00004d70: 6761 7465 644d 6574 7269 632e 5661 6c75  gatedMetric.Valu
+00004d80: 6552 0b61 6e6f 6e41 6e64 5377 6170 1a4a  eR.anonAndSwap.J
+00004d90: 0a05 5661 6c75 6512 0e0a 0274 7318 0120  ..Value....ts.. 
+00004da0: 0128 0352 0274 7312 1b0a 096f 6f6d 5f73  .(.R.ts....oom_s
+00004db0: 636f 7265 1802 2001 2805 5208 6f6f 6d53  core.. .(.R.oomS
+00004dc0: 636f 7265 1214 0a05 7661 6c75 6518 0320  core....value.. 
+00004dd0: 0128 0152 0576 616c 7565 0af1 030a 3670  .(.R.value....6p
+00004de0: 726f 746f 732f 7065 7266 6574 746f 2f6d  rotos/perfetto/m
+00004df0: 6574 7269 6373 2f61 6e64 726f 6964 2f6d  etrics/android/m
+00004e00: 756c 7469 7573 6572 5f6d 6574 7269 632e  ultiuser_metric.
+00004e10: 7072 6f74 6f12 0f70 6572 6665 7474 6f2e  proto..perfetto.
+00004e20: 7072 6f74 6f73 22a5 030a 1641 6e64 726f  protos"....Andro
+00004e30: 6964 4d75 6c74 6975 7365 724d 6574 7269  idMultiuserMetri
+00004e40: 6312 520a 0b75 7365 725f 7377 6974 6368  c.R..user_switch
+00004e50: 1801 2001 280b 3231 2e70 6572 6665 7474  .. .(.21.perfett
+00004e60: 6f2e 7072 6f74 6f73 2e41 6e64 726f 6964  o.protos.Android
+00004e70: 4d75 6c74 6975 7365 724d 6574 7269 632e  MultiuserMetric.
+00004e80: 4576 656e 7444 6174 6152 0a75 7365 7253  EventDataR.userS
+00004e90: 7769 7463 681a b602 0a09 4576 656e 7444  witch.....EventD
+00004ea0: 6174 6112 1f0a 0b64 7572 6174 696f 6e5f  ata....duration_
+00004eb0: 6d73 1801 2001 2805 520a 6475 7261 7469  ms.. .(.R.durati
+00004ec0: 6f6e 4d73 1257 0a09 6370 755f 7573 6167  onMs.W..cpu_usag
+00004ed0: 6518 0220 0328 0b32 3a2e 7065 7266 6574  e.. .(.2:.perfet
+00004ee0: 746f 2e70 726f 746f 732e 416e 6472 6f69  to.protos.Androi
+00004ef0: 644d 756c 7469 7573 6572 4d65 7472 6963  dMultiuserMetric
+00004f00: 2e45 7665 6e74 4461 7461 2e43 7075 5573  .EventData.CpuUs
+00004f10: 6167 6552 0863 7075 5573 6167 651a ae01  ageR.cpuUsage...
+00004f20: 0a08 4370 7555 7361 6765 1217 0a07 7573  ..CpuUsage....us
+00004f30: 6572 5f69 6418 0120 0128 0552 0675 7365  er_id.. .(.R.use
+00004f40: 7249 6412 210a 0c70 726f 6365 7373 5f6e  rId.!..process_n
+00004f50: 616d 6518 0220 0128 0952 0b70 726f 6365  ame.. .(.R.proce
+00004f60: 7373 4e61 6d65 121f 0a0b 6370 755f 6d63  ssName....cpu_mc
+00004f70: 7963 6c65 7318 0320 0128 0552 0a63 7075  ycles.. .(.R.cpu
+00004f80: 4d63 7963 6c65 7312 250a 0e63 7075 5f70  Mcycles.%..cpu_p
+00004f90: 6572 6365 6e74 6167 6518 0420 0128 0252  ercentage.. .(.R
+00004fa0: 0d63 7075 5065 7263 656e 7461 6765 121e  .cpuPercentage..
+00004fb0: 0a0a 6964 656e 7469 6669 6572 1805 2001  ..identifier.. .
+00004fc0: 2809 520a 6964 656e 7469 6669 6572 0ab5  (.R.identifier..
+00004fd0: 150a 3470 726f 746f 732f 7065 7266 6574  ..4protos/perfet
+00004fe0: 746f 2f6d 6574 7269 6373 2f61 6e64 726f  to/metrics/andro
+00004ff0: 6964 2f6e 6574 776f 726b 5f6d 6574 7269  id/network_metri
+00005000: 632e 7072 6f74 6f12 0f70 6572 6665 7474  c.proto..perfett
+00005010: 6f2e 7072 6f74 6f73 22eb 140a 1441 6e64  o.protos"....And
+00005020: 726f 6964 4e65 7477 6f72 6b4d 6574 7269  roidNetworkMetri
+00005030: 6312 500a 0b6e 6574 5f64 6576 6963 6573  c.P..net_devices
+00005040: 1801 2003 280b 322f 2e70 6572 6665 7474  .. .(.2/.perfett
+00005050: 6f2e 7072 6f74 6f73 2e41 6e64 726f 6964  o.protos.Android
+00005060: 4e65 7477 6f72 6b4d 6574 7269 632e 4e65  NetworkMetric.Ne
+00005070: 7444 6576 6963 6552 0a6e 6574 4465 7669  tDeviceR.netDevi
+00005080: 6365 7312 550a 0d6e 6574 5f72 785f 6163  ces.U..net_rx_ac
+00005090: 7469 6f6e 1802 2001 280b 3231 2e70 6572  tion.. .(.21.per
+000050a0: 6665 7474 6f2e 7072 6f74 6f73 2e41 6e64  fetto.protos.And
+000050b0: 726f 6964 4e65 7477 6f72 6b4d 6574 7269  roidNetworkMetri
+000050c0: 632e 4e65 7452 7841 6374 696f 6e52 0b6e  c.NetRxActionR.n
+000050d0: 6574 5278 4163 7469 6f6e 122f 0a13 7265  etRxAction./..re
+000050e0: 7472 616e 736d 6973 7369 6f6e 5f72 6174  transmission_rat
+000050f0: 6518 0320 0128 0152 1272 6574 7261 6e73  e.. .(.R.retrans
+00005100: 6d69 7373 696f 6e52 6174 6512 240a 0e6b  missionRate.$..k
+00005110: 6672 6565 5f73 6b62 5f72 6174 6518 0420  free_skb_rate.. 
+00005120: 0128 0152 0c6b 6672 6565 536b 6252 6174  .(.R.kfreeSkbRat
+00005130: 6512 550a 0d6e 6574 5f74 785f 6163 7469  e.U..net_tx_acti
+00005140: 6f6e 1805 2001 280b 3231 2e70 6572 6665  on.. .(.21.perfe
+00005150: 7474 6f2e 7072 6f74 6f73 2e41 6e64 726f  tto.protos.Andro
+00005160: 6964 4e65 7477 6f72 6b4d 6574 7269 632e  idNetworkMetric.
+00005170: 4e65 7454 7841 6374 696f 6e52 0b6e 6574  NetTxActionR.net
+00005180: 5478 4163 7469 6f6e 124e 0a0a 6970 695f  TxAction.N..ipi_
+00005190: 6163 7469 6f6e 1806 2001 280b 322f 2e70  action.. .(.2/.p
+000051a0: 6572 6665 7474 6f2e 7072 6f74 6f73 2e41  erfetto.protos.A
+000051b0: 6e64 726f 6964 4e65 7477 6f72 6b4d 6574  ndroidNetworkMet
+000051c0: 7269 632e 4970 6941 6374 696f 6e52 0969  ric.IpiActionR.i
+000051d0: 7069 4163 7469 6f6e 1afc 010a 0f50 6163  piAction.....Pac
+000051e0: 6b65 7453 7461 7469 7374 6963 1218 0a07  ketStatistic....
+000051f0: 7061 636b 6574 7318 0120 0128 0352 0770  packets.. .(.R.p
+00005200: 6163 6b65 7473 1214 0a05 6279 7465 7318  ackets....bytes.
+00005210: 0220 0128 0352 0562 7974 6573 1239 0a19  . .(.R.bytes.9..
+00005220: 6669 7273 745f 7061 636b 6574 5f74 696d  first_packet_tim
+00005230: 6573 7461 6d70 5f6e 7318 0320 0128 0352  estamp_ns.. .(.R
+00005240: 1666 6972 7374 5061 636b 6574 5469 6d65  .firstPacketTime
+00005250: 7374 616d 704e 7312 370a 186c 6173 745f  stampNs.7..last_
+00005260: 7061 636b 6574 5f74 696d 6573 7461 6d70  packet_timestamp
+00005270: 5f6e 7318 0420 0128 0352 156c 6173 7450  _ns.. .(.R.lastP
+00005280: 6163 6b65 7454 696d 6573 7461 6d70 4e73  acketTimestampNs
+00005290: 121f 0a0b 696e 7465 7276 616c 5f6e 7318  ....interval_ns.
+000052a0: 0520 0128 0352 0a69 6e74 6572 7661 6c4e  . .(.R.intervalN
+000052b0: 7312 240a 0e64 6174 615f 7261 7465 5f6b  s.$..data_rate_k
+000052c0: 6270 7318 0620 0128 0152 0c64 6174 6152  bps.. .(.R.dataR
+000052d0: 6174 654b 6270 731a 8701 0a13 436f 7265  ateKbps.....Core
+000052e0: 5061 636b 6574 5374 6174 6973 7469 6312  PacketStatistic.
+000052f0: 0e0a 0269 6418 0120 0128 0d52 0269 6412  ...id.. .(.R.id.
+00005300: 600a 1070 6163 6b65 745f 7374 6174 6973  `..packet_statis
+00005310: 7469 6318 0220 0128 0b32 352e 7065 7266  tic.. .(.25.perf
+00005320: 6574 746f 2e70 726f 746f 732e 416e 6472  etto.protos.Andr
+00005330: 6f69 644e 6574 776f 726b 4d65 7472 6963  oidNetworkMetric
+00005340: 2e50 6163 6b65 7453 7461 7469 7374 6963  .PacketStatistic
+00005350: 520f 7061 636b 6574 5374 6174 6973 7469  R.packetStatisti
+00005360: 631a d401 0a02 5278 124b 0a05 746f 7461  c.....Rx.K..tota
+00005370: 6c18 0120 0128 0b32 352e 7065 7266 6574  l.. .(.25.perfet
+00005380: 746f 2e70 726f 746f 732e 416e 6472 6f69  to.protos.Androi
+00005390: 644e 6574 776f 726b 4d65 7472 6963 2e50  dNetworkMetric.P
+000053a0: 6163 6b65 7453 7461 7469 7374 6963 5205  acketStatisticR.
+000053b0: 746f 7461 6c12 4d0a 0463 6f72 6518 0220  total.M..core.. 
+000053c0: 0328 0b32 392e 7065 7266 6574 746f 2e70  .(.29.perfetto.p
+000053d0: 726f 746f 732e 416e 6472 6f69 644e 6574  rotos.AndroidNet
+000053e0: 776f 726b 4d65 7472 6963 2e43 6f72 6550  workMetric.CoreP
+000053f0: 6163 6b65 7453 7461 7469 7374 6963 5204  acketStatisticR.
+00005400: 636f 7265 1232 0a15 6772 6f5f 6167 6772  core.2..gro_aggr
+00005410: 6567 6174 696f 6e5f 7261 7469 6f18 0320  egation_ratio.. 
+00005420: 0128 0952 1367 726f 4167 6772 6567 6174  .(.R.groAggregat
+00005430: 696f 6e52 6174 696f 1aa0 010a 0254 7812  ionRatio.....Tx.
+00005440: 4b0a 0574 6f74 616c 1801 2001 280b 3235  K..total.. .(.25
+00005450: 2e70 6572 6665 7474 6f2e 7072 6f74 6f73  .perfetto.protos
+00005460: 2e41 6e64 726f 6964 4e65 7477 6f72 6b4d  .AndroidNetworkM
+00005470: 6574 7269 632e 5061 636b 6574 5374 6174  etric.PacketStat
+00005480: 6973 7469 6352 0574 6f74 616c 124d 0a04  isticR.total.M..
+00005490: 636f 7265 1802 2003 280b 3239 2e70 6572  core.. .(.29.per
+000054a0: 6665 7474 6f2e 7072 6f74 6f73 2e41 6e64  fetto.protos.And
+000054b0: 726f 6964 4e65 7477 6f72 6b4d 6574 7269  roidNetworkMetri
+000054c0: 632e 436f 7265 5061 636b 6574 5374 6174  c.CorePacketStat
+000054d0: 6973 7469 6352 0463 6f72 651a 9301 0a09  isticR.core.....
+000054e0: 4e65 7444 6576 6963 6512 120a 046e 616d  NetDevice....nam
+000054f0: 6518 0120 0128 0952 046e 616d 6512 380a  e.. .(.R.name.8.
+00005500: 0272 7818 0220 0128 0b32 282e 7065 7266  .rx.. .(.2(.perf
+00005510: 6574 746f 2e70 726f 746f 732e 416e 6472  etto.protos.Andr
+00005520: 6f69 644e 6574 776f 726b 4d65 7472 6963  oidNetworkMetric
+00005530: 2e52 7852 0272 7812 380a 0274 7818 0320  .RxR.rx.8..tx.. 
+00005540: 0128 0b32 282e 7065 7266 6574 746f 2e70  .(.2(.perfetto.p
+00005550: 726f 746f 732e 416e 6472 6f69 644e 6574  rotos.AndroidNet
+00005560: 776f 726b 4d65 7472 6963 2e54 7852 0274  workMetric.TxR.t
+00005570: 781a ad01 0a14 4e65 7452 7841 6374 696f  x.....NetRxActio
+00005580: 6e53 7461 7469 7374 6963 1214 0a05 636f  nStatistic....co
+00005590: 756e 7418 0120 0128 0352 0563 6f75 6e74  unt.. .(.R.count
+000055a0: 121d 0a0a 7275 6e74 696d 655f 6d73 1802  ....runtime_ms..
+000055b0: 2001 2801 5209 7275 6e74 696d 654d 7312   .(.R.runtimeMs.
+000055c0: 240a 0e61 7667 5f72 756e 7469 6d65 5f6d  $..avg_runtime_m
+000055d0: 7318 0320 0128 0152 0c61 7667 5275 6e74  s.. .(.R.avgRunt
+000055e0: 696d 654d 7312 180a 076d 6379 636c 6573  imeMs....mcycles
+000055f0: 1804 2001 2803 5207 6d63 7963 6c65 7312  .. .(.R.mcycles.
+00005600: 200a 0c61 7667 5f66 7265 715f 6b68 7a18   ..avg_freq_khz.
+00005610: 0520 0128 0352 0a61 7667 4672 6571 4b68  . .(.R.avgFreqKh
+00005620: 7a1a ad01 0a14 4e65 7454 7841 6374 696f  z.....NetTxActio
+00005630: 6e53 7461 7469 7374 6963 1214 0a05 636f  nStatistic....co
+00005640: 756e 7418 0120 0128 0352 0563 6f75 6e74  unt.. .(.R.count
+00005650: 121d 0a0a 7275 6e74 696d 655f 6d73 1802  ....runtime_ms..
+00005660: 2001 2801 5209 7275 6e74 696d 654d 7312   .(.R.runtimeMs.
+00005670: 240a 0e61 7667 5f72 756e 7469 6d65 5f6d  $..avg_runtime_m
+00005680: 7318 0320 0128 0152 0c61 7667 5275 6e74  s.. .(.R.avgRunt
+00005690: 696d 654d 7312 180a 076d 6379 636c 6573  imeMs....mcycles
+000056a0: 1804 2001 2803 5207 6d63 7963 6c65 7312  .. .(.R.mcycles.
+000056b0: 200a 0c61 7667 5f66 7265 715f 6b68 7a18   ..avg_freq_khz.
+000056c0: 0520 0128 0352 0a61 7667 4672 6571 4b68  . .(.R.avgFreqKh
+000056d0: 7a1a 6f0a 1249 7069 4163 7469 6f6e 5374  z.o..IpiActionSt
+000056e0: 6174 6973 7469 6312 140a 0563 6f75 6e74  atistic....count
+000056f0: 1801 2001 2803 5205 636f 756e 7412 1d0a  .. .(.R.count...
+00005700: 0a72 756e 7469 6d65 5f6d 7318 0220 0128  .runtime_ms.. .(
+00005710: 0152 0972 756e 7469 6d65 4d73 1224 0a0e  .R.runtimeMs.$..
+00005720: 6176 675f 7275 6e74 696d 655f 6d73 1803  avg_runtime_ms..
+00005730: 2001 2801 520c 6176 6752 756e 7469 6d65   .(.R.avgRuntime
+00005740: 4d73 1a9d 010a 1843 6f72 654e 6574 5278  Ms.....CoreNetRx
+00005750: 4163 7469 6f6e 5374 6174 6973 7469 6312  ActionStatistic.
+00005760: 0e0a 0269 6418 0120 0128 0d52 0269 6412  ...id.. .(.R.id.
+00005770: 710a 176e 6574 5f72 785f 6163 7469 6f6e  q..net_rx_action
+00005780: 5f73 7461 7469 7374 6963 1802 2001 280b  _statistic.. .(.
+00005790: 323a 2e70 6572 6665 7474 6f2e 7072 6f74  2:.perfetto.prot
+000057a0: 6f73 2e41 6e64 726f 6964 4e65 7477 6f72  os.AndroidNetwor
+000057b0: 6b4d 6574 7269 632e 4e65 7452 7841 6374  kMetric.NetRxAct
+000057c0: 696f 6e53 7461 7469 7374 6963 5214 6e65  ionStatisticR.ne
+000057d0: 7452 7841 6374 696f 6e53 7461 7469 7374  tRxActionStatist
+000057e0: 6963 1a9d 010a 1843 6f72 654e 6574 5478  ic.....CoreNetTx
+000057f0: 4163 7469 6f6e 5374 6174 6973 7469 6312  ActionStatistic.
+00005800: 0e0a 0269 6418 0120 0128 0d52 0269 6412  ...id.. .(.R.id.
+00005810: 710a 176e 6574 5f74 785f 6163 7469 6f6e  q..net_tx_action
+00005820: 5f73 7461 7469 7374 6963 1802 2001 280b  _statistic.. .(.
+00005830: 323a 2e70 6572 6665 7474 6f2e 7072 6f74  2:.perfetto.prot
+00005840: 6f73 2e41 6e64 726f 6964 4e65 7477 6f72  os.AndroidNetwor
+00005850: 6b4d 6574 7269 632e 4e65 7454 7841 6374  kMetric.NetTxAct
+00005860: 696f 6e53 7461 7469 7374 6963 5214 6e65  ionStatisticR.ne
+00005870: 7454 7841 6374 696f 6e53 7461 7469 7374  tTxActionStatist
+00005880: 6963 1aee 010a 0b4e 6574 5278 4163 7469  ic.....NetRxActi
+00005890: 6f6e 1250 0a05 746f 7461 6c18 0120 0128  on.P..total.. .(
+000058a0: 0b32 3a2e 7065 7266 6574 746f 2e70 726f  .2:.perfetto.pro
+000058b0: 746f 732e 416e 6472 6f69 644e 6574 776f  tos.AndroidNetwo
+000058c0: 726b 4d65 7472 6963 2e4e 6574 5278 4163  rkMetric.NetRxAc
+000058d0: 7469 6f6e 5374 6174 6973 7469 6352 0574  tionStatisticR.t
+000058e0: 6f74 616c 1252 0a04 636f 7265 1802 2003  otal.R..core.. .
+000058f0: 280b 323e 2e70 6572 6665 7474 6f2e 7072  (.2>.perfetto.pr
+00005900: 6f74 6f73 2e41 6e64 726f 6964 4e65 7477  otos.AndroidNetw
+00005910: 6f72 6b4d 6574 7269 632e 436f 7265 4e65  orkMetric.CoreNe
+00005920: 7452 7841 6374 696f 6e53 7461 7469 7374  tRxActionStatist
+00005930: 6963 5204 636f 7265 1239 0a19 6176 675f  icR.core.9..avg_
+00005940: 696e 7465 7273 7461 636b 5f6c 6174 656e  interstack_laten
+00005950: 6379 5f6d 7318 0320 0128 0152 1661 7667  cy_ms.. .(.R.avg
+00005960: 496e 7465 7273 7461 636b 4c61 7465 6e63  InterstackLatenc
+00005970: 794d 731a b301 0a0b 4e65 7454 7841 6374  yMs.....NetTxAct
+00005980: 696f 6e12 500a 0574 6f74 616c 1801 2001  ion.P..total.. .
+00005990: 280b 323a 2e70 6572 6665 7474 6f2e 7072  (.2:.perfetto.pr
+000059a0: 6f74 6f73 2e41 6e64 726f 6964 4e65 7477  otos.AndroidNetw
+000059b0: 6f72 6b4d 6574 7269 632e 4e65 7454 7841  orkMetric.NetTxA
+000059c0: 6374 696f 6e53 7461 7469 7374 6963 5205  ctionStatisticR.
+000059d0: 746f 7461 6c12 520a 0463 6f72 6518 0220  total.R..core.. 
+000059e0: 0328 0b32 3e2e 7065 7266 6574 746f 2e70  .(.2>.perfetto.p
+000059f0: 726f 746f 732e 416e 6472 6f69 644e 6574  rotos.AndroidNet
+00005a00: 776f 726b 4d65 7472 6963 2e43 6f72 654e  workMetric.CoreN
+00005a10: 6574 5478 4163 7469 6f6e 5374 6174 6973  etTxActionStatis
+00005a20: 7469 6352 0463 6f72 651a 5b0a 0949 7069  ticR.core.[..Ipi
+00005a30: 4163 7469 6f6e 124e 0a05 746f 7461 6c18  Action.N..total.
+00005a40: 0120 0128 0b32 382e 7065 7266 6574 746f  . .(.28.perfetto
+00005a50: 2e70 726f 746f 732e 416e 6472 6f69 644e  .protos.AndroidN
+00005a60: 6574 776f 726b 4d65 7472 6963 2e49 7069  etworkMetric.Ipi
+00005a70: 4163 7469 6f6e 5374 6174 6973 7469 6352  ActionStatisticR
+00005a80: 0574 6f74 616c 0a95 010a 3270 726f 746f  .total....2proto
+00005a90: 732f 7065 7266 6574 746f 2f6d 6574 7269  s/perfetto/metri
+00005aa0: 6373 2f61 6e64 726f 6964 2f6f 7468 6572  cs/android/other
+00005ab0: 5f74 7261 6365 732e 7072 6f74 6f12 0f70  _traces.proto..p
+00005ac0: 6572 6665 7474 6f2e 7072 6f74 6f73 224e  erfetto.protos"N
+00005ad0: 0a18 416e 6472 6f69 644f 7468 6572 5472  ..AndroidOtherTr
+00005ae0: 6163 6573 4d65 7472 6963 1232 0a15 6669  acesMetric.2..fi
+00005af0: 6e61 6c69 7a65 645f 7472 6163 6573 5f75  nalized_traces_u
+00005b00: 7569 6418 0120 0328 0952 1366 696e 616c  uid.. .(.R.final
+00005b10: 697a 6564 5472 6163 6573 5575 6964 0a88  izedTracesUuid..
+00005b20: 020a 3270 726f 746f 732f 7065 7266 6574  ..2protos/perfet
+00005b30: 746f 2f6d 6574 7269 6373 2f61 6e64 726f  to/metrics/andro
+00005b40: 6964 2f70 6163 6b61 6765 5f6c 6973 742e  id/package_list.
+00005b50: 7072 6f74 6f12 0f70 6572 6665 7474 6f2e  proto..perfetto.
+00005b60: 7072 6f74 6f73 22c0 010a 1241 6e64 726f  protos"....Andro
+00005b70: 6964 5061 636b 6167 654c 6973 7412 470a  idPackageList.G.
+00005b80: 0870 6163 6b61 6765 7318 0120 0328 0b32  .packages.. .(.2
+00005b90: 2b2e 7065 7266 6574 746f 2e70 726f 746f  +.perfetto.proto
+00005ba0: 732e 416e 6472 6f69 6450 6163 6b61 6765  s.AndroidPackage
+00005bb0: 4c69 7374 2e50 6163 6b61 6765 5208 7061  List.PackageR.pa
+00005bc0: 636b 6167 6573 1a61 0a07 5061 636b 6167  ckages.a..Packag
+00005bd0: 6512 210a 0c70 6163 6b61 6765 5f6e 616d  e.!..package_nam
+00005be0: 6518 0120 0128 0952 0b70 6163 6b61 6765  e.. .(.R.package
+00005bf0: 4e61 6d65 1210 0a03 7569 6418 0220 0128  Name....uid.. .(
+00005c00: 0352 0375 6964 1221 0a0c 7665 7273 696f  .R.uid.!..versio
+00005c10: 6e5f 636f 6465 1803 2001 2803 520b 7665  n_code.. .(.R.ve
+00005c20: 7273 696f 6e43 6f64 650a d203 0a35 7072  rsionCode....5pr
+00005c30: 6f74 6f73 2f70 6572 6665 7474 6f2f 6d65  otos/perfetto/me
+00005c40: 7472 6963 732f 616e 6472 6f69 642f 706f  trics/android/po
+00005c50: 7772 6169 6c73 5f6d 6574 7269 632e 7072  wrails_metric.pr
+00005c60: 6f74 6f12 0f70 6572 6665 7474 6f2e 7072  oto..perfetto.pr
+00005c70: 6f74 6f73 2287 030a 1141 6e64 726f 6964  otos"....Android
+00005c80: 506f 7765 7252 6169 6c73 124e 0a0b 706f  PowerRails.N..po
+00005c90: 7765 725f 7261 696c 7318 0120 0328 0b32  wer_rails.. .(.2
+00005ca0: 2d2e 7065 7266 6574 746f 2e70 726f 746f  -.perfetto.proto
+00005cb0: 732e 416e 6472 6f69 6450 6f77 6572 5261  s.AndroidPowerRa
+00005cc0: 696c 732e 506f 7765 7252 6169 6c73 520a  ils.PowerRailsR.
+00005cd0: 706f 7765 7252 6169 6c73 1234 0a17 6176  powerRails.4..av
+00005ce0: 675f 746f 7461 6c5f 7573 6564 5f70 6f77  g_total_used_pow
+00005cf0: 6572 5f6d 7718 0220 0128 0152 1361 7667  er_mw.. .(.R.avg
+00005d00: 546f 7461 6c55 7365 6450 6f77 6572 4d77  TotalUsedPowerMw
+00005d10: 1a4e 0a0a 456e 6572 6779 4461 7461 1221  .N..EnergyData.!
+00005d20: 0a0c 7469 6d65 7374 616d 705f 6d73 1801  ..timestamp_ms..
+00005d30: 2001 2803 520b 7469 6d65 7374 616d 704d   .(.R.timestampM
+00005d40: 7312 1d0a 0a65 6e65 7267 795f 7577 7318  s....energy_uws.
+00005d50: 0220 0128 0152 0965 6e65 7267 7955 7773  . .(.R.energyUws
+00005d60: 1a9b 010a 0a50 6f77 6572 5261 696c 7312  .....PowerRails.
+00005d70: 120a 046e 616d 6518 0120 0128 0952 046e  ...name.. .(.R.n
+00005d80: 616d 6512 4e0a 0b65 6e65 7267 795f 6461  ame.N..energy_da
+00005d90: 7461 1802 2003 280b 322d 2e70 6572 6665  ta.. .(.2-.perfe
+00005da0: 7474 6f2e 7072 6f74 6f73 2e41 6e64 726f  tto.protos.Andro
+00005db0: 6964 506f 7765 7252 6169 6c73 2e45 6e65  idPowerRails.Ene
+00005dc0: 7267 7944 6174 6152 0a65 6e65 7267 7944  rgyDataR.energyD
+00005dd0: 6174 6112 290a 1161 7667 5f75 7365 645f  ata.)..avg_used_
+00005de0: 706f 7765 725f 6d77 1803 2001 2801 520e  power_mw.. .(.R.
+00005df0: 6176 6755 7365 6450 6f77 6572 4d77 0ae5  avgUsedPowerMw..
+00005e00: 030a 3470 726f 746f 732f 7065 7266 6574  ..4protos/perfet
+00005e10: 746f 2f6d 6574 7269 6373 2f61 6e64 726f  to/metrics/andro
+00005e20: 6964 2f70 726f 6669 6c65 725f 736d 6170  id/profiler_smap
+00005e30: 732e 7072 6f74 6f12 0f70 6572 6665 7474  s.proto..perfett
+00005e40: 6f2e 7072 6f74 6f73 1a36 7072 6f74 6f73  o.protos.6protos
+00005e50: 2f70 6572 6665 7474 6f2f 6d65 7472 6963  /perfetto/metric
+00005e60: 732f 616e 6472 6f69 642f 7072 6f63 6573  s/android/proces
+00005e70: 735f 6d65 7461 6461 7461 2e70 726f 746f  s_metadata.proto
+00005e80: 22e3 020a 0d50 726f 6669 6c65 7253 6d61  "....ProfilerSma
+00005e90: 7073 1243 0a08 696e 7374 616e 6365 1801  ps.C..instance..
+00005ea0: 2003 280b 3227 2e70 6572 6665 7474 6f2e   .(.2'.perfetto.
+00005eb0: 7072 6f74 6f73 2e50 726f 6669 6c65 7253  protos.ProfilerS
+00005ec0: 6d61 7073 2e49 6e73 7461 6e63 6552 0869  maps.InstanceR.i
+00005ed0: 6e73 7461 6e63 651a 790a 074d 6170 7069  nstance.y..Mappi
+00005ee0: 6e67 1212 0a04 7061 7468 1801 2001 2809  ng....path.. .(.
+00005ef0: 5204 7061 7468 1217 0a07 7369 7a65 5f6b  R.path....size_k
+00005f00: 6218 0220 0128 0552 0673 697a 654b 6212  b.. .(.R.sizeKb.
+00005f10: 280a 1070 7269 7661 7465 5f64 6972 7479  (..private_dirty
+00005f20: 5f6b 6218 0320 0128 0552 0e70 7269 7661  _kb.. .(.R.priva
+00005f30: 7465 4469 7274 794b 6212 170a 0773 7761  teDirtyKb....swa
+00005f40: 705f 6b62 1804 2001 2805 5206 7377 6170  p_kb.. .(.R.swap
+00005f50: 4b62 1a91 010a 0849 6e73 7461 6e63 6512  Kb.....Instance.
+00005f60: 410a 0770 726f 6365 7373 1801 2001 280b  A..process.. .(.
+00005f70: 3227 2e70 6572 6665 7474 6f2e 7072 6f74  2'.perfetto.prot
+00005f80: 6f73 2e41 6e64 726f 6964 5072 6f63 6573  os.AndroidProces
+00005f90: 734d 6574 6164 6174 6152 0770 726f 6365  sMetadataR.proce
+00005fa0: 7373 1242 0a08 6d61 7070 696e 6773 1802  ss.B..mappings..
+00005fb0: 2003 280b 3226 2e70 6572 6665 7474 6f2e   .(.2&.perfetto.
+00005fc0: 7072 6f74 6f73 2e50 726f 6669 6c65 7253  protos.ProfilerS
+00005fd0: 6d61 7073 2e4d 6170 7069 6e67 5208 6d61  maps.MappingR.ma
+00005fe0: 7070 696e 6773 0acc 020a 3770 726f 746f  ppings....7proto
+00005ff0: 732f 7065 7266 6574 746f 2f6d 6574 7269  s/perfetto/metri
+00006000: 6373 2f61 6e64 726f 6964 2f72 745f 7275  cs/android/rt_ru
+00006010: 6e74 696d 655f 6d65 7472 6963 2e70 726f  ntime_metric.pro
+00006020: 746f 120f 7065 7266 6574 746f 2e70 726f  to..perfetto.pro
+00006030: 746f 7322 ff01 0a16 416e 6472 6f69 6452  tos"....AndroidR
+00006040: 7452 756e 7469 6d65 4d65 7472 6963 121f  tRuntimeMetric..
+00006050: 0a0b 6d61 785f 7275 6e74 696d 6518 0120  ..max_runtime.. 
+00006060: 0128 0352 0a6d 6178 5275 6e74 696d 6512  .(.R.maxRuntime.
+00006070: 240a 0e6f 7665 725f 356d 735f 636f 756e  $..over_5ms_coun
+00006080: 7418 0220 0128 0352 0c6f 7665 7235 6d73  t.. .(.R.over5ms
+00006090: 436f 756e 7412 5b0a 116c 6f6e 6765 7374  Count.[..longest
+000060a0: 5f72 745f 736c 6963 6573 1803 2003 280b  _rt_slices.. .(.
+000060b0: 322f 2e70 6572 6665 7474 6f2e 7072 6f74  2/.perfetto.prot
+000060c0: 6f73 2e41 6e64 726f 6964 5274 5275 6e74  os.AndroidRtRunt
+000060d0: 696d 654d 6574 7269 632e 5274 536c 6963  imeMetric.RtSlic
+000060e0: 6552 0f6c 6f6e 6765 7374 5274 536c 6963  eR.longestRtSlic
+000060f0: 6573 1a41 0a07 5274 536c 6963 6512 140a  es.A..RtSlice...
+00006100: 0574 6e61 6d65 1801 2001 2809 5205 746e  .tname.. .(.R.tn
+00006110: 616d 6512 0e0a 0274 7318 0220 0128 0352  ame....ts.. .(.R
+00006120: 0274 7312 100a 0364 7572 1803 2001 2803  .ts....dur.. .(.
+00006130: 5203 6475 720a ed04 0a30 7072 6f74 6f73  R.dur....0protos
+00006140: 2f70 6572 6665 7474 6f2f 6d65 7472 6963  /perfetto/metric
+00006150: 732f 616e 6472 6f69 642f 7369 6d70 6c65  s/android/simple
+00006160: 7065 7266 2e70 726f 746f 120f 7065 7266  perf.proto..perf
+00006170: 6574 746f 2e70 726f 746f 7322 a704 0a17  etto.protos"....
+00006180: 416e 6472 6f69 6453 696d 706c 6570 6572  AndroidSimpleper
+00006190: 664d 6574 7269 6312 210a 0c75 7267 656e  fMetric.!..urgen
+000061a0: 745f 7261 7469 6f18 0120 0128 0152 0b75  t_ratio.. .(.R.u
+000061b0: 7267 656e 7452 6174 696f 1250 0a06 6576  rgentRatio.P..ev
+000061c0: 656e 7473 1802 2003 280b 3238 2e70 6572  ents.. .(.28.per
+000061d0: 6665 7474 6f2e 7072 6f74 6f73 2e41 6e64  fetto.protos.And
+000061e0: 726f 6964 5369 6d70 6c65 7065 7266 4d65  roidSimpleperfMe
+000061f0: 7472 6963 2e50 6572 6645 7665 6e74 4d65  tric.PerfEventMe
+00006200: 7472 6963 5206 6576 656e 7473 1a96 030a  tricR.events....
+00006210: 0f50 6572 6645 7665 6e74 4d65 7472 6963  .PerfEventMetric
+00006220: 1212 0a04 6e61 6d65 1801 2001 2809 5204  ....name.. .(.R.
+00006230: 6e61 6d65 125e 0a09 7072 6f63 6573 7365  name.^..processe
+00006240: 7318 0220 0328 0b32 402e 7065 7266 6574  s.. .(.2@.perfet
+00006250: 746f 2e70 726f 746f 732e 416e 6472 6f69  to.protos.Androi
+00006260: 6453 696d 706c 6570 6572 664d 6574 7269  dSimpleperfMetri
+00006270: 632e 5065 7266 4576 656e 744d 6574 7269  c.PerfEventMetri
+00006280: 632e 5072 6f63 6573 7352 0970 726f 6365  c.ProcessR.proce
+00006290: 7373 6573 1214 0a05 746f 7461 6c18 0320  sses....total.. 
+000062a0: 0128 0152 0574 6f74 616c 1a56 0a06 5468  .(.R.total.V..Th
+000062b0: 7265 6164 1210 0a03 7469 6418 0120 0128  read....tid.. .(
+000062c0: 0552 0374 6964 1212 0a04 6e61 6d65 1802  .R.tid....name..
+000062d0: 2001 2809 5204 6e61 6d65 1210 0a03 6370   .(.R.name....cp
+000062e0: 7518 0320 0128 0552 0363 7075 1214 0a05  u.. .(.R.cpu....
+000062f0: 746f 7461 6c18 0420 0128 0152 0574 6f74  total.. .(.R.tot
+00006300: 616c 1aa0 010a 0750 726f 6365 7373 1210  al.....Process..
+00006310: 0a03 7069 6418 0120 0128 0552 0370 6964  ..pid.. .(.R.pid
+00006320: 1212 0a04 6e61 6d65 1802 2001 2809 5204  ....name.. .(.R.
+00006330: 6e61 6d65 1259 0a07 7468 7265 6164 7318  name.Y..threads.
+00006340: 0320 0328 0b32 3f2e 7065 7266 6574 746f  . .(.2?.perfetto
+00006350: 2e70 726f 746f 732e 416e 6472 6f69 6453  .protos.AndroidS
+00006360: 696d 706c 6570 6572 664d 6574 7269 632e  impleperfMetric.
+00006370: 5065 7266 4576 656e 744d 6574 7269 632e  PerfEventMetric.
+00006380: 5468 7265 6164 5207 7468 7265 6164 7312  ThreadR.threads.
+00006390: 140a 0574 6f74 616c 1804 2001 2801 5205  ...total.. .(.R.
+000063a0: 746f 7461 6c0a d42e 0a34 7072 6f74 6f73  total....4protos
+000063b0: 2f70 6572 6665 7474 6f2f 6d65 7472 6963  /perfetto/metric
+000063c0: 732f 616e 6472 6f69 642f 7374 6172 7475  s/android/startu
+000063d0: 705f 6d65 7472 6963 2e70 726f 746f 120f  p_metric.proto..
+000063e0: 7065 7266 6574 746f 2e70 726f 746f 731a  perfetto.protos.
+000063f0: 3670 726f 746f 732f 7065 7266 6574 746f  6protos/perfetto
+00006400: 2f6d 6574 7269 6373 2f61 6e64 726f 6964  /metrics/android
+00006410: 2f70 726f 6365 7373 5f6d 6574 6164 6174  /process_metadat
+00006420: 612e 7072 6f74 6f22 d22d 0a14 416e 6472  a.proto".-..Andr
+00006430: 6f69 6453 7461 7274 7570 4d65 7472 6963  oidStartupMetric
+00006440: 1247 0a07 7374 6172 7475 7018 0120 0328  .G..startup.. .(
+00006450: 0b32 2d2e 7065 7266 6574 746f 2e70 726f  .2-.perfetto.pro
+00006460: 746f 732e 416e 6472 6f69 6453 7461 7274  tos.AndroidStart
+00006470: 7570 4d65 7472 6963 2e53 7461 7274 7570  upMetric.Startup
+00006480: 5207 7374 6172 7475 701a f302 0a12 5461  R.startup.....Ta
+00006490: 736b 5374 6174 6542 7265 616b 646f 776e  skStateBreakdown
+000064a0: 1224 0a0e 7275 6e6e 696e 675f 6475 725f  .$..running_dur_
+000064b0: 6e73 1801 2001 2803 520c 7275 6e6e 696e  ns.. .(.R.runnin
+000064c0: 6744 7572 4e73 1226 0a0f 7275 6e6e 6162  gDurNs.&..runnab
+000064d0: 6c65 5f64 7572 5f6e 7318 0220 0128 0352  le_dur_ns.. .(.R
+000064e0: 0d72 756e 6e61 626c 6544 7572 4e73 123f  .runnableDurNs.?
+000064f0: 0a1c 756e 696e 7465 7272 7570 7469 626c  ..uninterruptibl
+00006500: 655f 736c 6565 705f 6475 725f 6e73 1803  e_sleep_dur_ns..
+00006510: 2001 2803 5219 756e 696e 7465 7272 7570   .(.R.uninterrup
+00006520: 7469 626c 6553 6c65 6570 4475 724e 7312  tibleSleepDurNs.
+00006530: 3b0a 1a69 6e74 6572 7275 7074 6962 6c65  ;..interruptible
+00006540: 5f73 6c65 6570 5f64 7572 5f6e 7318 0420  _sleep_dur_ns.. 
+00006550: 0128 0352 1769 6e74 6572 7275 7074 6962  .(.R.interruptib
+00006560: 6c65 536c 6565 7044 7572 4e73 1244 0a1f  leSleepDurNs.D..
+00006570: 756e 696e 7465 7272 7570 7469 626c 655f  uninterruptible_
+00006580: 696f 5f73 6c65 6570 5f64 7572 5f6e 7318  io_sleep_dur_ns.
+00006590: 0520 0128 0352 1b75 6e69 6e74 6572 7275  . .(.R.uninterru
+000065a0: 7074 6962 6c65 496f 536c 6565 7044 7572  ptibleIoSleepDur
+000065b0: 4e73 124b 0a23 756e 696e 7465 7272 7570  Ns.K.#uninterrup
+000065c0: 7469 626c 655f 6e6f 6e5f 696f 5f73 6c65  tible_non_io_sle
+000065d0: 6570 5f64 7572 5f6e 7318 0620 0128 0352  ep_dur_ns.. .(.R
+000065e0: 1e75 6e69 6e74 6572 7275 7074 6962 6c65  .uninterruptible
+000065f0: 4e6f 6e49 6f53 6c65 6570 4475 724e 731a  NonIoSleepDurNs.
+00006600: 6f0a 114d 6379 636c 6573 4279 436f 7265  o..McyclesByCore
+00006610: 5479 7065 1216 0a06 6c69 7474 6c65 1801  Type....little..
+00006620: 2001 2803 5206 6c69 7474 6c65 1210 0a03   .(.R.little....
+00006630: 6269 6718 0220 0128 0352 0362 6967 1216  big.. .(.R.big..
+00006640: 0a06 6269 6767 6572 1803 2001 2803 5206  ..bigger.. .(.R.
+00006650: 6269 6767 6572 1218 0a07 756e 6b6e 6f77  bigger....unknow
+00006660: 6e18 0420 0128 0352 0775 6e6b 6e6f 776e  n.. .(.R.unknown
+00006670: 1a35 0a05 536c 6963 6512 150a 0664 7572  .5..Slice....dur
+00006680: 5f6e 7318 0120 0128 0352 0564 7572 4e73  _ns.. .(.R.durNs
+00006690: 1215 0a06 6475 725f 6d73 1802 2001 2801  ....dur_ms.. .(.
+000066a0: 5205 6475 724d 731a 9a15 0a0c 546f 4669  R.durMs.....ToFi
+000066b0: 7273 7446 7261 6d65 1215 0a06 6475 725f  rstFrame....dur_
+000066c0: 6e73 1801 2001 2803 5205 6475 724e 7312  ns.. .(.R.durNs.
+000066d0: 150a 0664 7572 5f6d 7318 1120 0128 0152  ...dur_ms.. .(.R
+000066e0: 0564 7572 4d73 1272 0a19 6d61 696e 5f74  .durMs.r..main_t
+000066f0: 6872 6561 645f 6279 5f74 6173 6b5f 7374  hread_by_task_st
+00006700: 6174 6518 0220 0128 0b32 382e 7065 7266  ate.. .(.28.perf
+00006710: 6574 746f 2e70 726f 746f 732e 416e 6472  etto.protos.Andr
+00006720: 6f69 6453 7461 7274 7570 4d65 7472 6963  oidStartupMetric
+00006730: 2e54 6173 6b53 7461 7465 4272 6561 6b64  .TaskStateBreakd
+00006740: 6f77 6e52 156d 6169 6e54 6872 6561 6442  ownR.mainThreadB
+00006750: 7954 6173 6b53 7461 7465 1268 0a14 6d63  yTaskState.h..mc
+00006760: 7963 6c65 735f 6279 5f63 6f72 655f 7479  ycles_by_core_ty
+00006770: 7065 181a 2001 280b 3237 2e70 6572 6665  pe.. .(.27.perfe
+00006780: 7474 6f2e 7072 6f74 6f73 2e41 6e64 726f  tto.protos.Andro
+00006790: 6964 5374 6172 7475 704d 6574 7269 632e  idStartupMetric.
+000067a0: 4d63 7963 6c65 7342 7943 6f72 6554 7970  McyclesByCoreTyp
+000067b0: 6552 116d 6379 636c 6573 4279 436f 7265  eR.mcyclesByCore
+000067c0: 5479 7065 1241 0a1d 6f74 6865 725f 7072  Type.A..other_pr
+000067d0: 6f63 6573 7365 735f 7370 6177 6e65 645f  ocesses_spawned_
+000067e0: 636f 756e 7418 0320 0128 0d52 1a6f 7468  count.. .(.R.oth
+000067f0: 6572 5072 6f63 6573 7365 7353 7061 776e  erProcessesSpawn
+00006800: 6564 436f 756e 7412 5f0a 1574 696d 655f  edCount._..time_
+00006810: 6163 7469 7669 7479 5f6d 616e 6167 6572  activity_manager
+00006820: 1804 2001 280b 322b 2e70 6572 6665 7474  .. .(.2+.perfett
+00006830: 6f2e 7072 6f74 6f73 2e41 6e64 726f 6964  o.protos.Android
+00006840: 5374 6172 7475 704d 6574 7269 632e 536c  StartupMetric.Sl
+00006850: 6963 6552 1374 696d 6541 6374 6976 6974  iceR.timeActivit
+00006860: 794d 616e 6167 6572 1266 0a19 7469 6d65  yManager.f..time
+00006870: 5f61 6374 6976 6974 795f 7468 7265 6164  _activity_thread
+00006880: 5f6d 6169 6e18 0520 0128 0b32 2b2e 7065  _main.. .(.2+.pe
+00006890: 7266 6574 746f 2e70 726f 746f 732e 416e  rfetto.protos.An
+000068a0: 6472 6f69 6453 7461 7274 7570 4d65 7472  droidStartupMetr
+000068b0: 6963 2e53 6c69 6365 5216 7469 6d65 4163  ic.SliceR.timeAc
+000068c0: 7469 7669 7479 5468 7265 6164 4d61 696e  tivityThreadMain
+000068d0: 125f 0a15 7469 6d65 5f62 696e 645f 6170  ._..time_bind_ap
+000068e0: 706c 6963 6174 696f 6e18 0620 0128 0b32  plication.. .(.2
+000068f0: 2b2e 7065 7266 6574 746f 2e70 726f 746f  +.perfetto.proto
+00006900: 732e 416e 6472 6f69 6453 7461 7274 7570  s.AndroidStartup
+00006910: 4d65 7472 6963 2e53 6c69 6365 5213 7469  Metric.SliceR.ti
+00006920: 6d65 4269 6e64 4170 706c 6963 6174 696f  meBindApplicatio
+00006930: 6e12 5b0a 1374 696d 655f 6163 7469 7669  n.[..time_activi
+00006940: 7479 5f73 7461 7274 1807 2001 280b 322b  ty_start.. .(.2+
+00006950: 2e70 6572 6665 7474 6f2e 7072 6f74 6f73  .perfetto.protos
+00006960: 2e41 6e64 726f 6964 5374 6172 7475 704d  .AndroidStartupM
+00006970: 6574 7269 632e 536c 6963 6552 1174 696d  etric.SliceR.tim
+00006980: 6541 6374 6976 6974 7953 7461 7274 125d  eActivityStart.]
+00006990: 0a14 7469 6d65 5f61 6374 6976 6974 795f  ..time_activity_
+000069a0: 7265 7375 6d65 1808 2001 280b 322b 2e70  resume.. .(.2+.p
+000069b0: 6572 6665 7474 6f2e 7072 6f74 6f73 2e41  erfetto.protos.A
+000069c0: 6e64 726f 6964 5374 6172 7475 704d 6574  ndroidStartupMet
+000069d0: 7269 632e 536c 6963 6552 1274 696d 6541  ric.SliceR.timeA
+000069e0: 6374 6976 6974 7952 6573 756d 6512 5f0a  ctivityResume._.
+000069f0: 1574 696d 655f 6163 7469 7669 7479 5f72  .time_activity_r
+00006a00: 6573 7461 7274 1815 2001 280b 322b 2e70  estart.. .(.2+.p
+00006a10: 6572 6665 7474 6f2e 7072 6f74 6f73 2e41  erfetto.protos.A
+00006a20: 6e64 726f 6964 5374 6172 7475 704d 6574  ndroidStartupMet
+00006a30: 7269 632e 536c 6963 6552 1374 696d 6541  ric.SliceR.timeA
+00006a40: 6374 6976 6974 7952 6573 7461 7274 125a  ctivityRestart.Z
+00006a50: 0a12 7469 6d65 5f63 686f 7265 6f67 7261  ..time_choreogra
+00006a60: 7068 6572 1809 2001 280b 322b 2e70 6572  pher.. .(.2+.per
+00006a70: 6665 7474 6f2e 7072 6f74 6f73 2e41 6e64  fetto.protos.And
+00006a80: 726f 6964 5374 6172 7475 704d 6574 7269  roidStartupMetri
+00006a90: 632e 536c 6963 6552 1174 696d 6543 686f  c.SliceR.timeCho
+00006aa0: 7265 6f67 7261 7068 6572 124e 0a0c 7469  reographer.N..ti
+00006ab0: 6d65 5f69 6e66 6c61 7465 1816 2001 280b  me_inflate.. .(.
+00006ac0: 322b 2e70 6572 6665 7474 6f2e 7072 6f74  2+.perfetto.prot
+00006ad0: 6f73 2e41 6e64 726f 6964 5374 6172 7475  os.AndroidStartu
+00006ae0: 704d 6574 7269 632e 536c 6963 6552 0b74  pMetric.SliceR.t
+00006af0: 696d 6549 6e66 6c61 7465 1259 0a12 7469  imeInflate.Y..ti
+00006b00: 6d65 5f67 6574 5f72 6573 6f75 7263 6573  me_get_resources
+00006b10: 1817 2001 280b 322b 2e70 6572 6665 7474  .. .(.2+.perfett
+00006b20: 6f2e 7072 6f74 6f73 2e41 6e64 726f 6964  o.protos.Android
+00006b30: 5374 6172 7475 704d 6574 7269 632e 536c  StartupMetric.Sl
+00006b40: 6963 6552 1074 696d 6547 6574 5265 736f  iceR.timeGetReso
+00006b50: 7572 6365 7312 660a 1974 696d 655f 6265  urces.f..time_be
+00006b60: 666f 7265 5f73 7461 7274 5f70 726f 6365  fore_start_proce
+00006b70: 7373 180a 2001 280b 322b 2e70 6572 6665  ss.. .(.2+.perfe
+00006b80: 7474 6f2e 7072 6f74 6f73 2e41 6e64 726f  tto.protos.Andro
+00006b90: 6964 5374 6172 7475 704d 6574 7269 632e  idStartupMetric.
+00006ba0: 536c 6963 6552 1674 696d 6542 6566 6f72  SliceR.timeBefor
+00006bb0: 6553 7461 7274 5072 6f63 6573 7312 660a  eStartProcess.f.
+00006bc0: 1974 696d 655f 6475 7269 6e67 5f73 7461  .time_during_sta
+00006bd0: 7274 5f70 726f 6365 7373 180b 2001 280b  rt_process.. .(.
+00006be0: 322b 2e70 6572 6665 7474 6f2e 7072 6f74  2+.perfetto.prot
+00006bf0: 6f73 2e41 6e64 726f 6964 5374 6172 7475  os.AndroidStartu
+00006c00: 704d 6574 7269 632e 536c 6963 6552 1674  pMetric.SliceR.t
+00006c10: 696d 6544 7572 696e 6753 7461 7274 5072  imeDuringStartPr
+00006c20: 6f63 6573 7312 4d0a 0c74 6f5f 706f 7374  ocess.M..to_post
+00006c30: 5f66 6f72 6b18 1220 0128 0b32 2b2e 7065  _fork.. .(.2+.pe
+00006c40: 7266 6574 746f 2e70 726f 746f 732e 416e  rfetto.protos.An
+00006c50: 6472 6f69 6453 7461 7274 7570 4d65 7472  droidStartupMetr
+00006c60: 6963 2e53 6c69 6365 520a 746f 506f 7374  ic.SliceR.toPost
+00006c70: 466f 726b 1262 0a17 746f 5f61 6374 6976  Fork.b..to_activ
+00006c80: 6974 795f 7468 7265 6164 5f6d 6169 6e18  ity_thread_main.
+00006c90: 1320 0128 0b32 2b2e 7065 7266 6574 746f  . .(.2+.perfetto
+00006ca0: 2e70 726f 746f 732e 416e 6472 6f69 6453  .protos.AndroidS
+00006cb0: 7461 7274 7570 4d65 7472 6963 2e53 6c69  tartupMetric.Sli
+00006cc0: 6365 5214 746f 4163 7469 7669 7479 5468  ceR.toActivityTh
+00006cd0: 7265 6164 4d61 696e 125b 0a13 746f 5f62  readMain.[..to_b
+00006ce0: 696e 645f 6170 706c 6963 6174 696f 6e18  ind_application.
+00006cf0: 1420 0128 0b32 2b2e 7065 7266 6574 746f  . .(.2+.perfetto
+00006d00: 2e70 726f 746f 732e 416e 6472 6f69 6453  .protos.AndroidS
+00006d10: 7461 7274 7570 4d65 7472 6963 2e53 6c69  tartupMetric.Sli
+00006d20: 6365 5211 746f 4269 6e64 4170 706c 6963  ceR.toBindApplic
+00006d30: 6174 696f 6e12 510a 0e74 696d 655f 706f  ation.Q..time_po
+00006d40: 7374 5f66 6f72 6b18 1020 0128 0b32 2b2e  st_fork.. .(.2+.
+00006d50: 7065 7266 6574 746f 2e70 726f 746f 732e  perfetto.protos.
+00006d60: 416e 6472 6f69 6453 7461 7274 7570 4d65  AndroidStartupMe
+00006d70: 7472 6963 2e53 6c69 6365 520c 7469 6d65  tric.SliceR.time
+00006d80: 506f 7374 466f 726b 124f 0a0d 7469 6d65  PostFork.O..time
+00006d90: 5f64 6578 5f6f 7065 6e18 1820 0128 0b32  _dex_open.. .(.2
+00006da0: 2b2e 7065 7266 6574 746f 2e70 726f 746f  +.perfetto.proto
+00006db0: 732e 416e 6472 6f69 6453 7461 7274 7570  s.AndroidStartup
+00006dc0: 4d65 7472 6963 2e53 6c69 6365 520b 7469  Metric.SliceR.ti
+00006dd0: 6d65 4465 784f 7065 6e12 570a 1174 696d  meDexOpen.W..tim
+00006de0: 655f 7665 7269 6679 5f63 6c61 7373 1819  e_verify_class..
+00006df0: 2001 280b 322b 2e70 6572 6665 7474 6f2e   .(.2+.perfetto.
+00006e00: 7072 6f74 6f73 2e41 6e64 726f 6964 5374  protos.AndroidSt
+00006e10: 6172 7475 704d 6574 7269 632e 536c 6963  artupMetric.Slic
+00006e20: 6552 0f74 696d 6556 6572 6966 7943 6c61  eR.timeVerifyCla
+00006e30: 7373 1230 0a14 6a69 745f 636f 6d70 696c  ss.0..jit_compil
+00006e40: 6564 5f6d 6574 686f 6473 181b 2001 280d  ed_methods.. .(.
+00006e50: 5212 6a69 7443 6f6d 7069 6c65 644d 6574  R.jitCompiledMet
+00006e60: 686f 6473 1268 0a1b 7469 6d65 5f6a 6974  hods.h..time_jit
+00006e70: 5f74 6872 6561 645f 706f 6f6c 5f6f 6e5f  _thread_pool_on_
+00006e80: 6370 7518 1c20 0128 0b32 2b2e 7065 7266  cpu.. .(.2+.perf
+00006e90: 6574 746f 2e70 726f 746f 732e 416e 6472  etto.protos.Andr
+00006ea0: 6f69 6453 7461 7274 7570 4d65 7472 6963  oidStartupMetric
+00006eb0: 2e53 6c69 6365 5216 7469 6d65 4a69 7454  .SliceR.timeJitT
+00006ec0: 6872 6561 6450 6f6f 6c4f 6e43 7075 124f  hreadPoolOnCpu.O
+00006ed0: 0a0d 7469 6d65 5f67 635f 746f 7461 6c18  ..time_gc_total.
+00006ee0: 1d20 0128 0b32 2b2e 7065 7266 6574 746f  . .(.2+.perfetto
+00006ef0: 2e70 726f 746f 732e 416e 6472 6f69 6453  .protos.AndroidS
+00006f00: 7461 7274 7570 4d65 7472 6963 2e53 6c69  tartupMetric.Sli
+00006f10: 6365 520b 7469 6d65 4763 546f 7461 6c12  ceR.timeGcTotal.
+00006f20: 500a 0e74 696d 655f 6763 5f6f 6e5f 6370  P..time_gc_on_cp
+00006f30: 7518 1e20 0128 0b32 2b2e 7065 7266 6574  u.. .(.2+.perfet
+00006f40: 746f 2e70 726f 746f 732e 416e 6472 6f69  to.protos.Androi
+00006f50: 6453 7461 7274 7570 4d65 7472 6963 2e53  dStartupMetric.S
+00006f60: 6c69 6365 520b 7469 6d65 4763 4f6e 4370  liceR.timeGcOnCp
+00006f70: 7512 730a 2074 696d 655f 6c6f 636b 5f63  u.s. time_lock_c
+00006f80: 6f6e 7465 6e74 696f 6e5f 7468 7265 6164  ontention_thread
+00006f90: 5f6d 6169 6e18 1f20 0128 0b32 2b2e 7065  _main.. .(.2+.pe
+00006fa0: 7266 6574 746f 2e70 726f 746f 732e 416e  rfetto.protos.An
+00006fb0: 6472 6f69 6453 7461 7274 7570 4d65 7472  droidStartupMetr
+00006fc0: 6963 2e53 6c69 6365 521c 7469 6d65 4c6f  ic.SliceR.timeLo
+00006fd0: 636b 436f 6e74 656e 7469 6f6e 5468 7265  ckContentionThre
+00006fe0: 6164 4d61 696e 1279 0a23 7469 6d65 5f6d  adMain.y.#time_m
+00006ff0: 6f6e 6974 6f72 5f63 6f6e 7465 6e74 696f  onitor_contentio
+00007000: 6e5f 7468 7265 6164 5f6d 6169 6e18 2020  n_thread_main.  
+00007010: 0128 0b32 2b2e 7065 7266 6574 746f 2e70  .(.2+.perfetto.p
+00007020: 726f 746f 732e 416e 6472 6f69 6453 7461  rotos.AndroidSta
+00007030: 7274 7570 4d65 7472 6963 2e53 6c69 6365  rtupMetric.Slice
+00007040: 521f 7469 6d65 4d6f 6e69 746f 7243 6f6e  R.timeMonitorCon
+00007050: 7465 6e74 696f 6e54 6872 6561 644d 6169  tentionThreadMai
+00007060: 6e12 650a 1974 696d 655f 6465 785f 6f70  n.e..time_dex_op
+00007070: 656e 5f74 6872 6561 645f 6d61 696e 1821  en_thread_main.!
+00007080: 2001 280b 322b 2e70 6572 6665 7474 6f2e   .(.2+.perfetto.
+00007090: 7072 6f74 6f73 2e41 6e64 726f 6964 5374  protos.AndroidSt
+000070a0: 6172 7475 704d 6574 7269 632e 536c 6963  artupMetric.Slic
+000070b0: 6552 1574 696d 6544 6578 4f70 656e 5468  eR.timeDexOpenTh
+000070c0: 7265 6164 4d61 696e 1262 0a17 7469 6d65  readMain.b..time
+000070d0: 5f64 6c6f 7065 6e5f 7468 7265 6164 5f6d  _dlopen_thread_m
+000070e0: 6169 6e18 2220 0128 0b32 2b2e 7065 7266  ain." .(.2+.perf
+000070f0: 6574 746f 2e70 726f 746f 732e 416e 6472  etto.protos.Andr
+00007100: 6f69 6453 7461 7274 7570 4d65 7472 6963  oidStartupMetric
+00007110: 2e53 6c69 6365 5214 7469 6d65 446c 6f70  .SliceR.timeDlop
+00007120: 656e 5468 7265 6164 4d61 696e 4a04 080c  enThreadMainJ...
+00007130: 100d 4a04 080d 100e 4a04 080e 100f 4a04  ..J.....J.....J.
+00007140: 080f 1010 1a5c 0a0a 4873 634d 6574 7269  .....\..HscMetri
+00007150: 6373 124e 0a0c 6675 6c6c 5f73 7461 7274  cs.N..full_start
+00007160: 7570 1801 2001 280b 322b 2e70 6572 6665  up.. .(.2+.perfe
+00007170: 7474 6f2e 7072 6f74 6f73 2e41 6e64 726f  tto.protos.Andro
+00007180: 6964 5374 6172 7475 704d 6574 7269 632e  idStartupMetric.
+00007190: 536c 6963 6552 0b66 756c 6c53 7461 7274  SliceR.fullStart
+000071a0: 7570 1a64 0a08 4163 7469 7669 7479 1212  up.d..Activity..
+000071b0: 0a04 6e61 6d65 1801 2001 2809 5204 6e61  ..name.. .(.R.na
+000071c0: 6d65 1216 0a06 6d65 7468 6f64 1802 2001  me....method.. .
+000071d0: 2809 5206 6d65 7468 6f64 1226 0a0f 7473  (.R.method.&..ts
+000071e0: 5f6d 6574 686f 645f 7374 6172 7418 0420  _method_start.. 
+000071f0: 0128 0352 0d74 734d 6574 686f 6453 7461  .(.R.tsMethodSta
+00007200: 7274 4a04 0803 1004 1a9b 020a 1142 696e  rtJ..........Bin
+00007210: 6465 7254 7261 6e73 6163 7469 6f6e 1247  derTransaction.G
+00007220: 0a08 6475 7261 7469 6f6e 1801 2001 280b  ..duration.. .(.
+00007230: 322b 2e70 6572 6665 7474 6f2e 7072 6f74  2+.perfetto.prot
+00007240: 6f73 2e41 6e64 726f 6964 5374 6172 7475  os.AndroidStartu
+00007250: 704d 6574 7269 632e 536c 6963 6552 0864  pMetric.SliceR.d
+00007260: 7572 6174 696f 6e12 160a 0674 6872 6561  uration....threa
+00007270: 6418 0220 0128 0952 0674 6872 6561 6412  d.. .(.R.thread.
+00007280: 2d0a 1264 6573 7469 6e61 7469 6f6e 5f74  -..destination_t
+00007290: 6872 6561 6418 0320 0128 0952 1164 6573  hread.. .(.R.des
+000072a0: 7469 6e61 7469 6f6e 5468 7265 6164 122f  tinationThread./
+000072b0: 0a13 6465 7374 696e 6174 696f 6e5f 7072  ..destination_pr
+000072c0: 6f63 6573 7318 0420 0128 0952 1264 6573  ocess.. .(.R.des
+000072d0: 7469 6e61 7469 6f6e 5072 6f63 6573 7312  tinationProcess.
+000072e0: 140a 0566 6c61 6773 1805 2001 2809 5205  ...flags.. .(.R.
+000072f0: 666c 6167 7312 120a 0463 6f64 6518 0620  flags....code.. 
+00007300: 0128 0952 0463 6f64 6512 1b0a 0964 6174  .(.R.code....dat
+00007310: 615f 7369 7a65 1807 2001 2803 5208 6461  a_size.. .(.R.da
+00007320: 7461 5369 7a65 1aaf 010a 124f 7074 696d  taSize.....Optim
+00007330: 697a 6174 696f 6e53 7461 7475 7312 1f0a  izationStatus...
+00007340: 0b6f 6465 785f 7374 6174 7573 1801 2001  .odex_status.. .
+00007350: 2809 520a 6f64 6578 5374 6174 7573 122d  (.R.odexStatus.-
+00007360: 0a12 636f 6d70 696c 6174 696f 6e5f 6669  ..compilation_fi
+00007370: 6c74 6572 1802 2001 2809 5211 636f 6d70  lter.. .(.R.comp
+00007380: 696c 6174 696f 6e46 696c 7465 7212 2d0a  ilationFilter.-.
+00007390: 1263 6f6d 7069 6c61 7469 6f6e 5f72 6561  .compilation_rea
+000073a0: 736f 6e18 0320 0128 0952 1163 6f6d 7069  son.. .(.R.compi
+000073b0: 6c61 7469 6f6e 5265 6173 6f6e 121a 0a08  lationReason....
+000073c0: 6c6f 6361 7469 6f6e 1804 2001 2809 5208  location.. .(.R.
+000073d0: 6c6f 6361 7469 6f6e 1a38 0a0b 5665 7269  location.8..Veri
+000073e0: 6679 436c 6173 7312 120a 046e 616d 6518  fyClass....name.
+000073f0: 0120 0128 0952 046e 616d 6512 150a 0664  . .(.R.name....d
+00007400: 7572 5f6e 7318 0220 0128 0352 0564 7572  ur_ns.. .(.R.dur
+00007410: 4e73 1a5b 0a0f 4576 656e 7454 696d 6573  Ns.[..EventTimes
+00007420: 7461 6d70 7312 270a 0f69 6e74 656e 745f  tamps.'..intent_
+00007430: 7265 6365 6976 6564 1801 2001 2803 520e  received.. .(.R.
+00007440: 696e 7465 6e74 5265 6365 6976 6564 121f  intentReceived..
+00007450: 0a0b 6669 7273 745f 6672 616d 6518 0220  ..first_frame.. 
+00007460: 0128 0352 0a66 6972 7374 4672 616d 651a  .(.R.firstFrame.
+00007470: f702 0a0b 5379 7374 656d 5374 6174 6512  ....SystemState.
+00007480: 2b0a 0f64 6578 326f 6174 5f72 756e 6e69  +..dex2oat_runni
+00007490: 6e67 1801 2001 2808 4202 1801 520e 6465  ng.. .(.B...R.de
+000074a0: 7832 6f61 7452 756e 6e69 6e67 122d 0a10  x2oatRunning.-..
+000074b0: 696e 7374 616c 6c64 5f72 756e 6e69 6e67  installd_running
+000074c0: 1802 2001 2808 4202 1801 520f 696e 7374  .. .(.B...R.inst
+000074d0: 616c 6c64 5275 6e6e 696e 6712 3c0a 1a62  alldRunning.<..b
+000074e0: 726f 6164 6361 7374 5f64 6973 7061 7463  roadcast_dispatc
+000074f0: 6865 645f 636f 756e 7418 0320 0128 0352  hed_count.. .(.R
+00007500: 1862 726f 6164 6361 7374 4469 7370 6174  .broadcastDispat
+00007510: 6368 6564 436f 756e 7412 380a 1862 726f  chedCount.8..bro
+00007520: 6164 6361 7374 5f72 6563 6569 7665 645f  adcast_received_
+00007530: 636f 756e 7418 0420 0128 0352 1662 726f  count.. .(.R.bro
+00007540: 6164 6361 7374 5265 6365 6976 6564 436f  adcastReceivedCo
+00007550: 756e 7412 460a 206d 6f73 745f 6163 7469  unt.F. most_acti
+00007560: 7665 5f6e 6f6e 5f6c 6175 6e63 685f 7072  ve_non_launch_pr
+00007570: 6f63 6573 7365 7318 0520 0328 0952 1c6d  ocesses.. .(.R.m
+00007580: 6f73 7441 6374 6976 654e 6f6e 4c61 756e  ostActiveNonLaun
+00007590: 6368 5072 6f63 6573 7365 7312 260a 0f69  chProcesses.&..i
+000075a0: 6e73 7461 6c6c 645f 6475 725f 6e73 1806  nstalld_dur_ns..
+000075b0: 2001 2803 520d 696e 7374 616c 6c64 4475   .(.R.installdDu
+000075c0: 724e 7312 240a 0e64 6578 326f 6174 5f64  rNs.$..dex2oat_d
+000075d0: 7572 5f6e 7318 0720 0128 0352 0c64 6578  ur_ns.. .(.R.dex
+000075e0: 326f 6174 4475 724e 731a 900a 0a07 5374  2oatDurNs.....St
+000075f0: 6172 7475 7012 1d0a 0a73 7461 7274 7570  artup....startup
+00007600: 5f69 6418 0120 0128 0d52 0973 7461 7274  _id.. .(.R.start
+00007610: 7570 4964 1221 0a0c 7374 6172 7475 705f  upId.!..startup_
+00007620: 7479 7065 1810 2001 2809 520b 7374 6172  type.. .(.R.star
+00007630: 7475 7054 7970 6512 210a 0c70 6163 6b61  tupType.!..packa
+00007640: 6765 5f6e 616d 6518 0220 0128 0952 0b70  ge_name.. .(.R.p
+00007650: 6163 6b61 6765 4e61 6d65 1221 0a0c 7072  ackageName.!..pr
+00007660: 6f63 6573 735f 6e61 6d65 1803 2001 2809  ocess_name.. .(.
+00007670: 520b 7072 6f63 6573 734e 616d 6512 4e0a  R.processName.N.
+00007680: 0a61 6374 6976 6974 6965 7318 0b20 0328  .activities.. .(
+00007690: 0b32 2e2e 7065 7266 6574 746f 2e70 726f  .2..perfetto.pro
+000076a0: 746f 732e 416e 6472 6f69 6453 7461 7274  tos.AndroidStart
+000076b0: 7570 4d65 7472 6963 2e41 6374 6976 6974  upMetric.Activit
+000076c0: 7952 0a61 6374 6976 6974 6965 7312 710a  yR.activities.q.
+000076d0: 186c 6f6e 675f 6269 6e64 6572 5f74 7261  .long_binder_tra
+000076e0: 6e73 6163 7469 6f6e 7318 0e20 0328 0b32  nsactions.. .(.2
+000076f0: 372e 7065 7266 6574 746f 2e70 726f 746f  7.perfetto.proto
+00007700: 732e 416e 6472 6f69 6453 7461 7274 7570  s.AndroidStartup
+00007710: 4d65 7472 6963 2e42 696e 6465 7254 7261  Metric.BinderTra
+00007720: 6e73 6163 7469 6f6e 5216 6c6f 6e67 4269  nsactionR.longBi
+00007730: 6e64 6572 5472 616e 7361 6374 696f 6e73  nderTransactions
+00007740: 122c 0a12 7a79 676f 7465 5f6e 6577 5f70  .,..zygote_new_p
+00007750: 726f 6365 7373 1804 2001 2808 5210 7a79  rocess.. .(.R.zy
+00007760: 676f 7465 4e65 7750 726f 6365 7373 1243  goteNewProcess.C
+00007770: 0a1e 6163 7469 7669 7479 5f68 6f73 7469  ..activity_hosti
+00007780: 6e67 5f70 726f 6365 7373 5f63 6f75 6e74  ng_process_count
+00007790: 1806 2001 280d 521b 6163 7469 7669 7479  .. .(.R.activity
+000077a0: 486f 7374 696e 6750 726f 6365 7373 436f  HostingProcessCo
+000077b0: 756e 7412 600a 1065 7665 6e74 5f74 696d  unt.`..event_tim
+000077c0: 6573 7461 6d70 7318 0d20 0128 0b32 352e  estamps.. .(.25.
+000077d0: 7065 7266 6574 746f 2e70 726f 746f 732e  perfetto.protos.
+000077e0: 416e 6472 6f69 6453 7461 7274 7570 4d65  AndroidStartupMe
+000077f0: 7472 6963 2e45 7665 6e74 5469 6d65 7374  tric.EventTimest
+00007800: 616d 7073 520f 6576 656e 7454 696d 6573  ampsR.eventTimes
+00007810: 7461 6d70 7312 580a 0e74 6f5f 6669 7273  tamps.X..to_firs
+00007820: 745f 6672 616d 6518 0520 0128 0b32 322e  t_frame.. .(.22.
+00007830: 7065 7266 6574 746f 2e70 726f 746f 732e  perfetto.protos.
+00007840: 416e 6472 6f69 6453 7461 7274 7570 4d65  AndroidStartupMe
+00007850: 7472 6963 2e54 6f46 6972 7374 4672 616d  tric.ToFirstFram
+00007860: 6552 0c74 6f46 6972 7374 4672 616d 6512  eR.toFirstFrame.
+00007870: 410a 0770 726f 6365 7373 1807 2001 280b  A..process.. .(.
+00007880: 3227 2e70 6572 6665 7474 6f2e 7072 6f74  2'.perfetto.prot
+00007890: 6f73 2e41 6e64 726f 6964 5072 6f63 6573  os.AndroidProces
+000078a0: 734d 6574 6164 6174 6152 0770 726f 6365  sMetadataR.proce
+000078b0: 7373 1242 0a03 6873 6318 0820 0128 0b32  ss.B..hsc.. .(.2
+000078c0: 302e 7065 7266 6574 746f 2e70 726f 746f  0.perfetto.proto
+000078d0: 732e 416e 6472 6f69 6453 7461 7274 7570  s.AndroidStartup
+000078e0: 4d65 7472 6963 2e48 7363 4d65 7472 6963  Metric.HscMetric
+000078f0: 7352 0368 7363 1259 0a12 7265 706f 7274  sR.hsc.Y..report
+00007900: 5f66 756c 6c79 5f64 7261 776e 1809 2001  _fully_drawn.. .
+00007910: 280b 322b 2e70 6572 6665 7474 6f2e 7072  (.2+.perfetto.pr
+00007920: 6f74 6f73 2e41 6e64 726f 6964 5374 6172  otos.AndroidStar
+00007930: 7475 704d 6574 7269 632e 536c 6963 6552  tupMetric.SliceR
+00007940: 1072 6570 6f72 7446 756c 6c79 4472 6177  .reportFullyDraw
+00007950: 6e12 690a 136f 7074 696d 697a 6174 696f  n.i..optimizatio
+00007960: 6e5f 7374 6174 7573 180c 2003 280b 3238  n_status.. .(.28
+00007970: 2e70 6572 6665 7474 6f2e 7072 6f74 6f73  .perfetto.protos
+00007980: 2e41 6e64 726f 6964 5374 6172 7475 704d  .AndroidStartupM
+00007990: 6574 7269 632e 4f70 7469 6d69 7a61 7469  etric.Optimizati
+000079a0: 6f6e 5374 6174 7573 5212 6f70 7469 6d69  onStatusR.optimi
+000079b0: 7a61 7469 6f6e 5374 6174 7573 1254 0a0c  zationStatus.T..
+000079c0: 7665 7269 6679 5f63 6c61 7373 1813 2003  verify_class.. .
+000079d0: 280b 3231 2e70 6572 6665 7474 6f2e 7072  (.21.perfetto.pr
+000079e0: 6f74 6f73 2e41 6e64 726f 6964 5374 6172  otos.AndroidStar
+000079f0: 7475 704d 6574 7269 632e 5665 7269 6679  tupMetric.Verify
+00007a00: 436c 6173 7352 0b76 6572 6966 7943 6c61  ClassR.verifyCla
+00007a10: 7373 121f 0a0b 646c 6f70 656e 5f66 696c  ss....dlopen_fil
+00007a20: 6518 1420 0328 0952 0a64 6c6f 7065 6e46  e.. .(.R.dlopenF
+00007a30: 696c 6512 3f0a 1c73 7461 7274 7570 5f63  ile.?..startup_c
+00007a40: 6f6e 6375 7272 656e 745f 746f 5f6c 6175  oncurrent_to_lau
+00007a50: 6e63 6818 1220 0328 0952 1973 7461 7274  nch.. .(.R.start
+00007a60: 7570 436f 6e63 7572 7265 6e74 546f 4c61  upConcurrentToLa
+00007a70: 756e 6368 1254 0a0c 7379 7374 656d 5f73  unch.T..system_s
+00007a80: 7461 7465 180f 2001 280b 3231 2e70 6572  tate.. .(.21.per
+00007a90: 6665 7474 6f2e 7072 6f74 6f73 2e41 6e64  fetto.protos.And
+00007aa0: 726f 6964 5374 6172 7475 704d 6574 7269  roidStartupMetri
+00007ab0: 632e 5379 7374 656d 5374 6174 6552 0b73  c.SystemStateR.s
+00007ac0: 7973 7465 6d53 7461 7465 122a 0a11 736c  ystemState.*..sl
+00007ad0: 6f77 5f73 7461 7274 5f72 6561 736f 6e18  ow_start_reason.
+00007ae0: 1120 0328 0952 0f73 6c6f 7753 7461 7274  . .(.R.slowStart
+00007af0: 5265 6173 6f6e 4a04 080a 100b 0ad1 070a  ReasonJ.........
+00007b00: 3470 726f 746f 732f 7065 7266 6574 746f  4protos/perfetto
+00007b10: 2f6d 6574 7269 6373 2f61 6e64 726f 6964  /metrics/android
+00007b20: 2f73 7572 6661 6365 666c 696e 6765 722e  /surfaceflinger.
+00007b30: 7072 6f74 6f12 0f70 6572 6665 7474 6f2e  proto..perfetto.
+00007b40: 7072 6f74 6f73 2287 070a 1b41 6e64 726f  protos"....Andro
+00007b50: 6964 5375 7266 6163 6566 6c69 6e67 6572  idSurfaceflinger
+00007b60: 4d65 7472 6963 1223 0a0d 6d69 7373 6564  Metric.#..missed
+00007b70: 5f66 7261 6d65 7318 0120 0128 0d52 0c6d  _frames.. .(.R.m
+00007b80: 6973 7365 6446 7261 6d65 7312 2a0a 116d  issedFrames.*..m
+00007b90: 6973 7365 645f 6877 635f 6672 616d 6573  issed_hwc_frames
+00007ba0: 1802 2001 280d 520f 6d69 7373 6564 4877  .. .(.R.missedHw
+00007bb0: 6346 7261 6d65 7312 2a0a 116d 6973 7365  cFrames.*..misse
+00007bc0: 645f 6770 755f 6672 616d 6573 1803 2001  d_gpu_frames.. .
+00007bd0: 280d 520f 6d69 7373 6564 4770 7546 7261  (.R.missedGpuFra
+00007be0: 6d65 7312 2a0a 116d 6973 7365 645f 6672  mes.*..missed_fr
+00007bf0: 616d 655f 7261 7465 1804 2001 2801 520f  ame_rate.. .(.R.
+00007c00: 6d69 7373 6564 4672 616d 6552 6174 6512  missedFrameRate.
+00007c10: 310a 156d 6973 7365 645f 6877 635f 6672  1..missed_hwc_fr
+00007c20: 616d 655f 7261 7465 1805 2001 2801 5212  ame_rate.. .(.R.
+00007c30: 6d69 7373 6564 4877 6346 7261 6d65 5261  missedHwcFrameRa
+00007c40: 7465 1231 0a15 6d69 7373 6564 5f67 7075  te.1..missed_gpu
+00007c50: 5f66 7261 6d65 5f72 6174 6518 0620 0128  _frame_rate.. .(
+00007c60: 0152 126d 6973 7365 6447 7075 4672 616d  .R.missedGpuFram
+00007c70: 6552 6174 6512 270a 0f67 7075 5f69 6e76  eRate.'..gpu_inv
+00007c80: 6f63 6174 696f 6e73 1807 2001 280d 520e  ocations.. .(.R.
+00007c90: 6770 7549 6e76 6f63 6174 696f 6e73 1232  gpuInvocations.2
+00007ca0: 0a16 6176 675f 6770 755f 7761 6974 696e  ..avg_gpu_waitin
+00007cb0: 675f 6475 725f 6d73 1808 2001 2801 5212  g_dur_ms.. .(.R.
+00007cc0: 6176 6747 7075 5761 6974 696e 6744 7572  avgGpuWaitingDur
+00007cd0: 4d73 1248 0a22 746f 7461 6c5f 6e6f 6e5f  Ms.H."total_non_
+00007ce0: 656d 7074 795f 6770 755f 7761 6974 696e  empty_gpu_waitin
+00007cf0: 675f 6475 725f 6d73 1809 2001 2801 521c  g_dur_ms.. .(.R.
+00007d00: 746f 7461 6c4e 6f6e 456d 7074 7947 7075  totalNonEmptyGpu
+00007d10: 5761 6974 696e 6744 7572 4d73 126e 0a13  WaitingDurMs.n..
+00007d20: 6d65 7472 6963 735f 7065 725f 6469 7370  metrics_per_disp
+00007d30: 6c61 7918 0a20 0328 0b32 3e2e 7065 7266  lay.. .(.2>.perf
+00007d40: 6574 746f 2e70 726f 746f 732e 416e 6472  etto.protos.Andr
+00007d50: 6f69 6453 7572 6661 6365 666c 696e 6765  oidSurfaceflinge
+00007d60: 724d 6574 7269 632e 4d65 7472 6963 7350  rMetric.MetricsP
+00007d70: 6572 4469 7370 6c61 7952 116d 6574 7269  erDisplayR.metri
+00007d80: 6373 5065 7244 6973 706c 6179 1ac1 020a  csPerDisplay....
+00007d90: 114d 6574 7269 6373 5065 7244 6973 706c  .MetricsPerDispl
+00007da0: 6179 121d 0a0a 6469 7370 6c61 795f 6964  ay....display_id
+00007db0: 1801 2001 2809 5209 6469 7370 6c61 7949  .. .(.R.displayI
+00007dc0: 6412 230a 0d6d 6973 7365 645f 6672 616d  d.#..missed_fram
+00007dd0: 6573 1802 2001 280d 520c 6d69 7373 6564  es.. .(.R.missed
+00007de0: 4672 616d 6573 122a 0a11 6d69 7373 6564  Frames.*..missed
+00007df0: 5f68 7763 5f66 7261 6d65 7318 0320 0128  _hwc_frames.. .(
+00007e00: 0d52 0f6d 6973 7365 6448 7763 4672 616d  .R.missedHwcFram
+00007e10: 6573 122a 0a11 6d69 7373 6564 5f67 7075  es.*..missed_gpu
+00007e20: 5f66 7261 6d65 7318 0420 0128 0d52 0f6d  _frames.. .(.R.m
+00007e30: 6973 7365 6447 7075 4672 616d 6573 122a  issedGpuFrames.*
+00007e40: 0a11 6d69 7373 6564 5f66 7261 6d65 5f72  ..missed_frame_r
+00007e50: 6174 6518 0520 0128 0152 0f6d 6973 7365  ate.. .(.R.misse
+00007e60: 6446 7261 6d65 5261 7465 1231 0a15 6d69  dFrameRate.1..mi
+00007e70: 7373 6564 5f68 7763 5f66 7261 6d65 5f72  ssed_hwc_frame_r
+00007e80: 6174 6518 0620 0128 0152 126d 6973 7365  ate.. .(.R.misse
+00007e90: 6448 7763 4672 616d 6552 6174 6512 310a  dHwcFrameRate.1.
+00007ea0: 156d 6973 7365 645f 6770 755f 6672 616d  .missed_gpu_fram
+00007eb0: 655f 7261 7465 1807 2001 2801 5212 6d69  e_rate.. .(.R.mi
+00007ec0: 7373 6564 4770 7546 7261 6d65 5261 7465  ssedGpuFrameRate
+00007ed0: 0abb 020a 3070 726f 746f 732f 7065 7266  ....0protos/perf
+00007ee0: 6574 746f 2f6d 6574 7269 6373 2f61 6e64  etto/metrics/and
+00007ef0: 726f 6964 2f74 6173 6b5f 6e61 6d65 732e  roid/task_names.
+00007f00: 7072 6f74 6f12 0f70 6572 6665 7474 6f2e  proto..perfetto.
+00007f10: 7072 6f74 6f73 22f5 010a 1041 6e64 726f  protos"....Andro
+00007f20: 6964 5461 736b 4e61 6d65 7312 430a 0770  idTaskNames.C..p
+00007f30: 726f 6365 7373 1801 2003 280b 3229 2e70  rocess.. .(.2).p
+00007f40: 6572 6665 7474 6f2e 7072 6f74 6f73 2e41  erfetto.protos.A
+00007f50: 6e64 726f 6964 5461 736b 4e61 6d65 732e  ndroidTaskNames.
+00007f60: 5072 6f63 6573 7352 0770 726f 6365 7373  ProcessR.process
+00007f70: 1a9b 010a 0750 726f 6365 7373 1210 0a03  .....Process....
+00007f80: 7069 6418 0120 0128 0352 0370 6964 1221  pid.. .(.R.pid.!
+00007f90: 0a0c 7072 6f63 6573 735f 6e61 6d65 1802  ..process_name..
+00007fa0: 2001 2809 520b 7072 6f63 6573 734e 616d   .(.R.processNam
+00007fb0: 6512 1f0a 0b74 6872 6561 645f 6e61 6d65  e....thread_name
+00007fc0: 1803 2003 2809 520a 7468 7265 6164 4e61  .. .(.R.threadNa
+00007fd0: 6d65 1210 0a03 7569 6418 0420 0128 0352  me....uid.. .(.R
+00007fe0: 0375 6964 1228 0a10 7569 645f 7061 636b  .uid.(..uid_pack
+00007ff0: 6167 655f 6e61 6d65 1805 2003 2809 520e  age_name.. .(.R.
+00008000: 7569 6450 6163 6b61 6765 4e61 6d65 0ad3  uidPackageName..
+00008010: 010a 3370 726f 746f 732f 7065 7266 6574  ..3protos/perfet
+00008020: 746f 2f6d 6574 7269 6373 2f61 6e64 726f  to/metrics/andro
+00008030: 6964 2f74 7261 6365 5f71 7561 6c69 7479  id/trace_quality
+00008040: 2e70 726f 746f 120f 7065 7266 6574 746f  .proto..perfetto
+00008050: 2e70 726f 746f 7322 8a01 0a19 416e 6472  .protos"....Andr
+00008060: 6f69 6454 7261 6365 5175 616c 6974 794d  oidTraceQualityM
+00008070: 6574 7269 6312 4e0a 0866 6169 6c75 7265  etric.N..failure
+00008080: 7318 0120 0328 0b32 322e 7065 7266 6574  s.. .(.22.perfet
+00008090: 746f 2e70 726f 746f 732e 416e 6472 6f69  to.protos.Androi
+000080a0: 6454 7261 6365 5175 616c 6974 794d 6574  dTraceQualityMet
+000080b0: 7269 632e 4661 696c 7572 6552 0866 6169  ric.FailureR.fai
+000080c0: 6c75 7265 731a 1d0a 0746 6169 6c75 7265  lures....Failure
+000080d0: 1212 0a04 6e61 6d65 1801 2001 2809 5204  ....name.. .(.R.
+000080e0: 6e61 6d65 0a6d 0a3f 7072 6f74 6f73 2f70  name.m.?protos/p
+000080f0: 6572 6665 7474 6f2f 6d65 7472 6963 732f  erfetto/metrics/
+00008100: 616e 6472 6f69 642f 616e 6472 6f69 645f  android/android_
+00008110: 7472 7573 7479 5f77 6f72 6b71 7565 7565  trusty_workqueue
+00008120: 732e 7072 6f74 6f12 0f70 6572 6665 7474  s.proto..perfett
+00008130: 6f2e 7072 6f74 6f73 2219 0a17 416e 6472  o.protos"...Andr
+00008140: 6f69 6454 7275 7374 7957 6f72 6b71 7565  oidTrustyWorkque
+00008150: 7565 730a a602 0a39 7072 6f74 6f73 2f70  ues....9protos/p
+00008160: 6572 6665 7474 6f2f 6d65 7472 6963 732f  erfetto/metrics/
+00008170: 616e 6472 6f69 642f 756e 7379 6d62 6f6c  android/unsymbol
+00008180: 697a 6564 5f66 7261 6d65 732e 7072 6f74  ized_frames.prot
+00008190: 6f12 0f70 6572 6665 7474 6f2e 7072 6f74  o..perfetto.prot
+000081a0: 6f73 22d7 010a 1255 6e73 796d 626f 6c69  os"....Unsymboli
+000081b0: 7a65 6446 7261 6d65 7312 410a 0666 7261  zedFrames.A..fra
+000081c0: 6d65 7318 0120 0328 0b32 292e 7065 7266  mes.. .(.2).perf
+000081d0: 6574 746f 2e70 726f 746f 732e 556e 7379  etto.protos.Unsy
+000081e0: 6d62 6f6c 697a 6564 4672 616d 6573 2e46  mbolizedFrames.F
+000081f0: 7261 6d65 5206 6672 616d 6573 1a7e 0a05  rameR.frames.~..
+00008200: 4672 616d 6512 160a 066d 6f64 756c 6518  Frame....module.
+00008210: 0120 0128 0952 066d 6f64 756c 6512 190a  . .(.R.module...
+00008220: 0862 7569 6c64 5f69 6418 0220 0128 0952  .build_id.. .(.R
+00008230: 0762 7569 6c64 4964 1218 0a07 6164 6472  .buildId....addr
+00008240: 6573 7318 0320 0128 0352 0761 6464 7265  ess.. .(.R.addre
+00008250: 7373 1228 0a10 676f 6f67 6c65 5f6c 6f6f  ss.(..google_loo
+00008260: 6b75 705f 6964 1804 2001 2809 520e 676f  kup_id.. .(.R.go
+00008270: 6f67 6c65 4c6f 6f6b 7570 4964 0aa3 0c0a  ogleLookupId....
+00008280: 3370 726f 746f 732f 7065 7266 6574 746f  3protos/perfetto
+00008290: 2f6d 6574 7269 6373 2f61 6e64 726f 6964  /metrics/android
+000082a0: 2f62 696e 6465 725f 6d65 7472 6963 2e70  /binder_metric.p
+000082b0: 726f 746f 120f 7065 7266 6574 746f 2e70  roto..perfetto.p
+000082c0: 726f 746f 7322 da0b 0a13 416e 6472 6f69  rotos"....Androi
+000082d0: 6442 696e 6465 724d 6574 7269 6312 650a  dBinderMetric.e.
+000082e0: 1170 726f 6365 7373 5f62 7265 616b 646f  .process_breakdo
+000082f0: 776e 1801 2003 280b 3238 2e70 6572 6665  wn.. .(.28.perfe
+00008300: 7474 6f2e 7072 6f74 6f73 2e41 6e64 726f  tto.protos.Andro
+00008310: 6964 4269 6e64 6572 4d65 7472 6963 2e50  idBinderMetric.P
+00008320: 6572 5072 6f63 6573 7342 7265 616b 646f  erProcessBreakdo
+00008330: 776e 5210 7072 6f63 6573 7342 7265 616b  wnR.processBreak
+00008340: 646f 776e 127b 0a1a 756e 6167 6772 6567  down.{..unaggreg
+00008350: 6174 6564 5f74 786e 5f62 7265 616b 646f  ated_txn_breakdo
+00008360: 776e 1802 2003 280b 323d 2e70 6572 6665  wn.. .(.2=.perfe
+00008370: 7474 6f2e 7072 6f74 6f73 2e41 6e64 726f  tto.protos.Andro
+00008380: 6964 4269 6e64 6572 4d65 7472 6963 2e55  idBinderMetric.U
+00008390: 6e61 6767 7265 6761 7465 6454 786e 4272  naggregatedTxnBr
+000083a0: 6561 6b64 6f77 6e52 1875 6e61 6767 7265  eakdownR.unaggre
+000083b0: 6761 7465 6454 786e 4272 6561 6b64 6f77  gatedTxnBreakdow
+000083c0: 6e1a 7f0a 1350 6572 5072 6f63 6573 7342  n....PerProcessB
+000083d0: 7265 616b 646f 776e 1221 0a0c 7072 6f63  reakdown.!..proc
+000083e0: 6573 735f 6e61 6d65 1801 2001 2809 520b  ess_name.. .(.R.
+000083f0: 7072 6f63 6573 734e 616d 6512 100a 0370  processName....p
+00008400: 6964 1802 2001 280d 5203 7069 6412 1d0a  id.. .(.R.pid...
+00008410: 0a73 6c69 6365 5f6e 616d 6518 0320 0128  .slice_name.. .(
+00008420: 0952 0973 6c69 6365 4e61 6d65 1214 0a05  .R.sliceName....
+00008430: 636f 756e 7418 0420 0128 0d52 0563 6f75  count.. .(.R.cou
+00008440: 6e74 1ac1 050a 1855 6e61 6767 7265 6761  nt.....Unaggrega
+00008450: 7465 6454 786e 4272 6561 6b64 6f77 6e12  tedTxnBreakdown.
+00008460: 1b0a 0961 6964 6c5f 6e61 6d65 1801 2001  ...aidl_name.. .
+00008470: 2809 5208 6169 646c 4e61 6d65 1225 0a0e  (.R.aidlName.%..
+00008480: 636c 6965 6e74 5f70 726f 6365 7373 1803  client_process..
+00008490: 2001 2809 520d 636c 6965 6e74 5072 6f63   .(.R.clientProc
+000084a0: 6573 7312 230a 0d63 6c69 656e 745f 7468  ess.#..client_th
+000084b0: 7265 6164 1804 2001 2809 520c 636c 6965  read.. .(.R.clie
+000084c0: 6e74 5468 7265 6164 1224 0a0e 6973 5f6d  ntThread.$..is_m
+000084d0: 6169 6e5f 7468 7265 6164 1805 2001 2808  ain_thread.. .(.
+000084e0: 520c 6973 4d61 696e 5468 7265 6164 121b  R.isMainThread..
+000084f0: 0a09 636c 6965 6e74 5f74 7318 0620 0128  ..client_ts.. .(
+00008500: 0352 0863 6c69 656e 7454 7312 1d0a 0a63  .R.clientTs....c
+00008510: 6c69 656e 745f 6475 7218 0720 0128 0352  lient_dur.. .(.R
+00008520: 0963 6c69 656e 7444 7572 1225 0a0e 7365  .clientDur.%..se
+00008530: 7276 6572 5f70 726f 6365 7373 1809 2001  rver_process.. .
+00008540: 2809 520d 7365 7276 6572 5072 6f63 6573  (.R.serverProces
+00008550: 7312 230a 0d73 6572 7665 725f 7468 7265  s.#..server_thre
+00008560: 6164 180a 2001 2809 520c 7365 7276 6572  ad.. .(.R.server
+00008570: 5468 7265 6164 121b 0a09 7365 7276 6572  Thread....server
+00008580: 5f74 7318 0b20 0128 0352 0873 6572 7665  _ts.. .(.R.serve
+00008590: 7254 7312 1d0a 0a73 6572 7665 725f 6475  rTs....server_du
+000085a0: 7218 0c20 0128 0352 0973 6572 7665 7244  r.. .(.R.serverD
+000085b0: 7572 125e 0a0d 7468 7265 6164 5f73 7461  ur.^..thread_sta
+000085c0: 7465 7318 0d20 0328 0b32 392e 7065 7266  tes.. .(.29.perf
+000085d0: 6574 746f 2e70 726f 746f 732e 416e 6472  etto.protos.Andr
+000085e0: 6f69 6442 696e 6465 724d 6574 7269 632e  oidBinderMetric.
+000085f0: 5468 7265 6164 5374 6174 6542 7265 616b  ThreadStateBreak
+00008600: 646f 776e 520c 7468 7265 6164 5374 6174  downR.threadStat
+00008610: 6573 126a 0a11 626c 6f63 6b65 645f 6675  es.j..blocked_fu
+00008620: 6e63 7469 6f6e 7318 0e20 0328 0b32 3d2e  nctions.. .(.2=.
+00008630: 7065 7266 6574 746f 2e70 726f 746f 732e  perfetto.protos.
+00008640: 416e 6472 6f69 6442 696e 6465 724d 6574  AndroidBinderMet
+00008650: 7269 632e 426c 6f63 6b65 6446 756e 6374  ric.BlockedFunct
+00008660: 696f 6e42 7265 616b 646f 776e 5210 626c  ionBreakdownR.bl
+00008670: 6f63 6b65 6446 756e 6374 696f 6e73 121d  ockedFunctions..
+00008680: 0a0a 636c 6965 6e74 5f74 6964 180f 2001  ..client_tid.. .
+00008690: 280d 5209 636c 6965 6e74 5469 6412 1d0a  (.R.clientTid...
+000086a0: 0a73 6572 7665 725f 7469 6418 1020 0128  .server_tid.. .(
+000086b0: 0d52 0973 6572 7665 7254 6964 121d 0a0a  .R.serverTid....
+000086c0: 636c 6965 6e74 5f70 6964 1811 2001 280d  client_pid.. .(.
+000086d0: 5209 636c 6965 6e74 5069 6412 1d0a 0a73  R.clientPid....s
+000086e0: 6572 7665 725f 7069 6418 1220 0128 0d52  erver_pid.. .(.R
+000086f0: 0973 6572 7665 7250 6964 4a04 0802 1003  .serverPidJ.....
+00008700: 4a04 0808 1009 1abd 010a 1454 6872 6561  J..........Threa
+00008710: 6453 7461 7465 4272 6561 6b64 6f77 6e12  dStateBreakdown.
+00008720: 2a0a 1174 6872 6561 645f 7374 6174 655f  *..thread_state_
+00008730: 7479 7065 1801 2001 2809 520f 7468 7265  type.. .(.R.thre
+00008740: 6164 5374 6174 6554 7970 6512 210a 0c74  adStateType.!..t
+00008750: 6872 6561 645f 7374 6174 6518 0220 0128  hread_state.. .(
+00008760: 0952 0b74 6872 6561 6453 7461 7465 1228  .R.threadState.(
+00008770: 0a10 7468 7265 6164 5f73 7461 7465 5f64  ..thread_state_d
+00008780: 7572 1803 2001 2803 520e 7468 7265 6164  ur.. .(.R.thread
+00008790: 5374 6174 6544 7572 122c 0a12 7468 7265  StateDur.,..thre
+000087a0: 6164 5f73 7461 7465 5f63 6f75 6e74 1804  ad_state_count..
+000087b0: 2001 2803 5210 7468 7265 6164 5374 6174   .(.R.threadStat
+000087c0: 6543 6f75 6e74 1ad9 010a 1842 6c6f 636b  eCount.....Block
+000087d0: 6564 4675 6e63 7469 6f6e 4272 6561 6b64  edFunctionBreakd
+000087e0: 6f77 6e12 2a0a 1174 6872 6561 645f 7374  own.*..thread_st
+000087f0: 6174 655f 7479 7065 1801 2001 2809 520f  ate_type.. .(.R.
+00008800: 7468 7265 6164 5374 6174 6554 7970 6512  threadStateType.
+00008810: 290a 1062 6c6f 636b 6564 5f66 756e 6374  )..blocked_funct
+00008820: 696f 6e18 0220 0128 0952 0f62 6c6f 636b  ion.. .(.R.block
+00008830: 6564 4675 6e63 7469 6f6e 1230 0a14 626c  edFunction.0..bl
+00008840: 6f63 6b65 645f 6675 6e63 7469 6f6e 5f64  ocked_function_d
+00008850: 7572 1803 2001 2803 5212 626c 6f63 6b65  ur.. .(.R.blocke
+00008860: 6446 756e 6374 696f 6e44 7572 1234 0a16  dFunctionDur.4..
+00008870: 626c 6f63 6b65 645f 6675 6e63 7469 6f6e  blocked_function
+00008880: 5f63 6f75 6e74 1804 2001 2803 5214 626c  _count.. .(.R.bl
+00008890: 6f63 6b65 6446 756e 6374 696f 6e43 6f75  ockedFunctionCou
+000088a0: 6e74 0a9f 0c0a 3f70 726f 746f 732f 7065  nt....?protos/pe
+000088b0: 7266 6574 746f 2f6d 6574 7269 6373 2f61  rfetto/metrics/a
+000088c0: 6e64 726f 6964 2f6d 6f6e 6974 6f72 5f63  ndroid/monitor_c
+000088d0: 6f6e 7465 6e74 696f 6e5f 6d65 7472 6963  ontention_metric
+000088e0: 2e70 726f 746f 120f 7065 7266 6574 746f  .proto..perfetto
+000088f0: 2e70 726f 746f 7322 ca0b 0a1e 416e 6472  .protos"....Andr
+00008900: 6f69 644d 6f6e 6974 6f72 436f 6e74 656e  oidMonitorConten
+00008910: 7469 6f6e 4d65 7472 6963 1248 0a04 6e6f  tionMetric.H..no
+00008920: 6465 1801 2003 280b 3234 2e70 6572 6665  de.. .(.24.perfe
+00008930: 7474 6f2e 7072 6f74 6f73 2e41 6e64 726f  tto.protos.Andro
+00008940: 6964 4d6f 6e69 746f 7243 6f6e 7465 6e74  idMonitorContent
+00008950: 696f 6e4d 6574 7269 632e 4e6f 6465 5204  ionMetric.NodeR.
+00008960: 6e6f 6465 1a99 080a 044e 6f64 6512 240a  node.....Node.$.
+00008970: 0e6e 6f64 655f 7061 7265 6e74 5f69 6418  .node_parent_id.
+00008980: 0120 0128 0352 0c6e 6f64 6550 6172 656e  . .(.R.nodeParen
+00008990: 7449 6412 170a 076e 6f64 655f 6964 1802  tId....node_id..
+000089a0: 2001 2803 5206 6e6f 6465 4964 120e 0a02   .(.R.nodeId....
+000089b0: 7473 1803 2001 2803 5202 7473 1210 0a03  ts.. .(.R.ts....
+000089c0: 6475 7218 0420 0128 0352 0364 7572 1221  dur.. .(.R.dur.!
+000089d0: 0a0c 7072 6f63 6573 735f 6e61 6d65 180e  ..process_name..
+000089e0: 2001 2809 520b 7072 6f63 6573 734e 616d   .(.R.processNam
+000089f0: 6512 100a 0370 6964 1817 2001 280d 5203  e....pid.. .(.R.
+00008a00: 7069 6412 210a 0c77 6169 7465 725f 636f  pid.!..waiter_co
+00008a10: 756e 7418 0b20 0128 0d52 0b77 6169 7465  unt.. .(.R.waite
+00008a20: 7243 6f75 6e74 1269 0a0d 7468 7265 6164  rCount.i..thread
+00008a30: 5f73 7461 7465 7318 1320 0328 0b32 442e  _states.. .(.2D.
+00008a40: 7065 7266 6574 746f 2e70 726f 746f 732e  perfetto.protos.
+00008a50: 416e 6472 6f69 644d 6f6e 6974 6f72 436f  AndroidMonitorCo
+00008a60: 6e74 656e 7469 6f6e 4d65 7472 6963 2e54  ntentionMetric.T
+00008a70: 6872 6561 6453 7461 7465 4272 6561 6b64  hreadStateBreakd
+00008a80: 6f77 6e52 0c74 6872 6561 6453 7461 7465  ownR.threadState
+00008a90: 7312 750a 1162 6c6f 636b 6564 5f66 756e  s.u..blocked_fun
+00008aa0: 6374 696f 6e73 1814 2003 280b 3248 2e70  ctions.. .(.2H.p
+00008ab0: 6572 6665 7474 6f2e 7072 6f74 6f73 2e41  erfetto.protos.A
+00008ac0: 6e64 726f 6964 4d6f 6e69 746f 7243 6f6e  ndroidMonitorCon
+00008ad0: 7465 6e74 696f 6e4d 6574 7269 632e 426c  tentionMetric.Bl
+00008ae0: 6f63 6b65 6446 756e 6374 696f 6e42 7265  ockedFunctionBre
+00008af0: 616b 646f 776e 5210 626c 6f63 6b65 6446  akdownR.blockedF
+00008b00: 756e 6374 696f 6e73 1227 0a0f 626c 6f63  unctions.'..bloc
+00008b10: 6b69 6e67 5f6d 6574 686f 6418 0520 0128  king_method.. .(
+00008b20: 0952 0e62 6c6f 636b 696e 674d 6574 686f  .R.blockingMetho
+00008b30: 6412 320a 1573 686f 7274 5f62 6c6f 636b  d.2..short_block
+00008b40: 696e 675f 6d65 7468 6f64 1807 2001 2809  ing_method.. .(.
+00008b50: 5213 7368 6f72 7442 6c6f 636b 696e 674d  R.shortBlockingM
+00008b60: 6574 686f 6412 210a 0c62 6c6f 636b 696e  ethod.!..blockin
+00008b70: 675f 7372 6318 0920 0128 0952 0b62 6c6f  g_src.. .(.R.blo
+00008b80: 636b 696e 6753 7263 1230 0a14 626c 6f63  ckingSrc.0..bloc
+00008b90: 6b69 6e67 5f74 6872 6561 645f 6e61 6d65  king_thread_name
+00008ba0: 180d 2001 2809 5212 626c 6f63 6b69 6e67  .. .(.R.blocking
+00008bb0: 5468 7265 6164 4e61 6d65 1235 0a17 6973  ThreadName.5..is
+00008bc0: 5f62 6c6f 636b 696e 675f 7468 7265 6164  _blocking_thread
+00008bd0: 5f6d 6169 6e18 1020 0128 0852 1469 7342  _main.. .(.R.isB
+00008be0: 6c6f 636b 696e 6754 6872 6561 644d 6169  lockingThreadMai
+00008bf0: 6e12 2e0a 1362 6c6f 636b 696e 675f 7468  n....blocking_th
+00008c00: 7265 6164 5f74 6964 1816 2001 280d 5211  read_tid.. .(.R.
+00008c10: 626c 6f63 6b69 6e67 5468 7265 6164 5469  blockingThreadTi
+00008c20: 6412 250a 0e62 6c6f 636b 6564 5f6d 6574  d.%..blocked_met
+00008c30: 686f 6418 0620 0128 0952 0d62 6c6f 636b  hod.. .(.R.block
+00008c40: 6564 4d65 7468 6f64 1230 0a14 7368 6f72  edMethod.0..shor
+00008c50: 745f 626c 6f63 6b65 645f 6d65 7468 6f64  t_blocked_method
+00008c60: 1808 2001 2809 5212 7368 6f72 7442 6c6f  .. .(.R.shortBlo
+00008c70: 636b 6564 4d65 7468 6f64 121f 0a0b 626c  ckedMethod....bl
+00008c80: 6f63 6b65 645f 7372 6318 0a20 0128 0952  ocked_src.. .(.R
+00008c90: 0a62 6c6f 636b 6564 5372 6312 2e0a 1362  .blockedSrc....b
+00008ca0: 6c6f 636b 6564 5f74 6872 6561 645f 6e61  locked_thread_na
+00008cb0: 6d65 180c 2001 2809 5211 626c 6f63 6b65  me.. .(.R.blocke
+00008cc0: 6454 6872 6561 644e 616d 6512 330a 1669  dThreadName.3..i
+00008cd0: 735f 626c 6f63 6b65 645f 7468 7265 6164  s_blocked_thread
+00008ce0: 5f6d 6169 6e18 0f20 0128 0852 1369 7342  _main.. .(.R.isB
+00008cf0: 6c6f 636b 6564 5468 7265 6164 4d61 696e  lockedThreadMain
+00008d00: 122c 0a12 626c 6f63 6b65 645f 7468 7265  .,..blocked_thre
+00008d10: 6164 5f74 6964 1815 2001 280d 5210 626c  ad_tid.. .(.R.bl
+00008d20: 6f63 6b65 6454 6872 6561 6454 6964 1226  ockedThreadTid.&
+00008d30: 0a0f 6269 6e64 6572 5f72 6570 6c79 5f74  ..binder_reply_t
+00008d40: 7318 1120 0128 0352 0d62 696e 6465 7252  s.. .(.R.binderR
+00008d50: 6570 6c79 5473 1228 0a10 6269 6e64 6572  eplyTs.(..binder
+00008d60: 5f72 6570 6c79 5f74 6964 1812 2001 280d  _reply_tid.. .(.
+00008d70: 520e 6269 6e64 6572 5265 706c 7954 6964  R.binderReplyTid
+00008d80: 1a91 010a 1454 6872 6561 6453 7461 7465  .....ThreadState
+00008d90: 4272 6561 6b64 6f77 6e12 210a 0c74 6872  Breakdown.!..thr
+00008da0: 6561 645f 7374 6174 6518 0120 0128 0952  ead_state.. .(.R
+00008db0: 0b74 6872 6561 6453 7461 7465 1228 0a10  .threadState.(..
+00008dc0: 7468 7265 6164 5f73 7461 7465 5f64 7572  thread_state_dur
+00008dd0: 1802 2001 2803 520e 7468 7265 6164 5374  .. .(.R.threadSt
+00008de0: 6174 6544 7572 122c 0a12 7468 7265 6164  ateDur.,..thread
+00008df0: 5f73 7461 7465 5f63 6f75 6e74 1803 2001  _state_count.. .
+00008e00: 2803 5210 7468 7265 6164 5374 6174 6543  (.R.threadStateC
+00008e10: 6f75 6e74 1aad 010a 1842 6c6f 636b 6564  ount.....Blocked
+00008e20: 4675 6e63 7469 6f6e 4272 6561 6b64 6f77  FunctionBreakdow
+00008e30: 6e12 290a 1062 6c6f 636b 6564 5f66 756e  n.)..blocked_fun
+00008e40: 6374 696f 6e18 0120 0128 0952 0f62 6c6f  ction.. .(.R.blo
+00008e50: 636b 6564 4675 6e63 7469 6f6e 1230 0a14  ckedFunction.0..
+00008e60: 626c 6f63 6b65 645f 6675 6e63 7469 6f6e  blocked_function
+00008e70: 5f64 7572 1802 2001 2803 5212 626c 6f63  _dur.. .(.R.bloc
+00008e80: 6b65 6446 756e 6374 696f 6e44 7572 1234  kedFunctionDur.4
+00008e90: 0a16 626c 6f63 6b65 645f 6675 6e63 7469  ..blocked_functi
+00008ea0: 6f6e 5f63 6f75 6e74 1803 2001 2803 5214  on_count.. .(.R.
+00008eb0: 626c 6f63 6b65 6446 756e 6374 696f 6e43  blockedFunctionC
+00008ec0: 6f75 6e74 0ae9 330a 2570 726f 746f 732f  ount..3.%protos/
+00008ed0: 7065 7266 6574 746f 2f6d 6574 7269 6373  perfetto/metrics
+00008ee0: 2f6d 6574 7269 6373 2e70 726f 746f 120f  /metrics.proto..
+00008ef0: 7065 7266 6574 746f 2e70 726f 746f 731a  perfetto.protos.
+00008f00: 4370 726f 746f 732f 7065 7266 6574 746f  Cprotos/perfetto
+00008f10: 2f6d 6574 7269 6373 2f61 6e64 726f 6964  /metrics/android
+00008f20: 2f61 6e64 726f 6964 5f66 7261 6d65 5f74  /android_frame_t
+00008f30: 696d 656c 696e 655f 6d65 7472 6963 2e70  imeline_metric.p
+00008f40: 726f 746f 1a31 7072 6f74 6f73 2f70 6572  roto.1protos/per
+00008f50: 6665 7474 6f2f 6d65 7472 6963 732f 616e  fetto/metrics/an
+00008f60: 6472 6f69 642f 6261 7474 5f6d 6574 7269  droid/batt_metri
+00008f70: 632e 7072 6f74 6f1a 4770 726f 746f 732f  c.proto.Gprotos/
+00008f80: 7065 7266 6574 746f 2f6d 6574 7269 6373  perfetto/metrics
+00008f90: 2f61 6e64 726f 6964 2f61 6e64 726f 6964  /android/android
+00008fa0: 5f62 6c6f 636b 696e 675f 6361 6c6c 735f  _blocking_calls_
+00008fb0: 6375 6a5f 6d65 7472 6963 2e70 726f 746f  cuj_metric.proto
+00008fc0: 1a30 7072 6f74 6f73 2f70 6572 6665 7474  .0protos/perfett
+00008fd0: 6f2f 6d65 7472 6963 732f 616e 6472 6f69  o/metrics/androi
+00008fe0: 642f 6370 755f 6d65 7472 6963 2e70 726f  d/cpu_metric.pro
+00008ff0: 746f 1a33 7072 6f74 6f73 2f70 6572 6665  to.3protos/perfe
+00009000: 7474 6f2f 6d65 7472 6963 732f 616e 6472  tto/metrics/andr
+00009010: 6f69 642f 6361 6d65 7261 5f6d 6574 7269  oid/camera_metri
+00009020: 632e 7072 6f74 6f1a 3970 726f 746f 732f  c.proto.9protos/
+00009030: 7065 7266 6574 746f 2f6d 6574 7269 6373  perfetto/metrics
+00009040: 2f61 6e64 726f 6964 2f63 616d 6572 615f  /android/camera_
+00009050: 756e 6167 675f 6d65 7472 6963 2e70 726f  unagg_metric.pro
+00009060: 746f 1a35 7072 6f74 6f73 2f70 6572 6665  to.5protos/perfe
+00009070: 7474 6f2f 6d65 7472 6963 732f 616e 6472  tto/metrics/andr
+00009080: 6f69 642f 6469 7370 6c61 795f 6d65 7472  oid/display_metr
+00009090: 6963 732e 7072 6f74 6f1a 3570 726f 746f  ics.proto.5proto
+000090a0: 732f 7065 7266 6574 746f 2f6d 6574 7269  s/perfetto/metri
+000090b0: 6373 2f61 6e64 726f 6964 2f64 6d61 5f68  cs/android/dma_h
+000090c0: 6561 705f 6d65 7472 6963 2e70 726f 746f  eap_metric.proto
+000090d0: 1a31 7072 6f74 6f73 2f70 6572 6665 7474  .1protos/perfett
+000090e0: 6f2f 6d65 7472 6963 732f 616e 6472 6f69  o/metrics/androi
+000090f0: 642f 6476 6673 5f6d 6574 7269 632e 7072  d/dvfs_metric.pr
+00009100: 6f74 6f1a 3470 726f 746f 732f 7065 7266  oto.4protos/perf
+00009110: 6574 746f 2f6d 6574 7269 6373 2f61 6e64  etto/metrics/and
+00009120: 726f 6964 2f66 6173 7472 7063 5f6d 6574  roid/fastrpc_met
+00009130: 7269 632e 7072 6f74 6f1a 3070 726f 746f  ric.proto.0proto
+00009140: 732f 7065 7266 6574 746f 2f6d 6574 7269  s/perfetto/metri
+00009150: 6373 2f61 6e64 726f 6964 2f67 3264 5f6d  cs/android/g2d_m
+00009160: 6574 7269 632e 7072 6f74 6f1a 3070 726f  etric.proto.0pro
+00009170: 746f 732f 7065 7266 6574 746f 2f6d 6574  tos/perfetto/met
+00009180: 7269 6373 2f61 6e64 726f 6964 2f67 7075  rics/android/gpu
+00009190: 5f6d 6574 7269 632e 7072 6f74 6f1a 3070  _metric.proto.0p
+000091a0: 726f 746f 732f 7065 7266 6574 746f 2f6d  rotos/perfetto/m
+000091b0: 6574 7269 6373 2f61 6e64 726f 6964 2f68  etrics/android/h
+000091c0: 7763 6f6d 706f 7365 722e 7072 6f74 6f1a  wcomposer.proto.
+000091d0: 3170 726f 746f 732f 7065 7266 6574 746f  1protos/perfetto
+000091e0: 2f6d 6574 7269 6373 2f61 6e64 726f 6964  /metrics/android
+000091f0: 2f68 7775 695f 6d65 7472 6963 2e70 726f  /hwui_metric.pro
+00009200: 746f 1a30 7072 6f74 6f73 2f70 6572 6665  to.0protos/perfe
+00009210: 7474 6f2f 6d65 7472 6963 732f 616e 6472  tto/metrics/andr
+00009220: 6f69 642f 696f 6e5f 6d65 7472 6963 2e70  oid/ion_metric.p
+00009230: 726f 746f 1a38 7072 6f74 6f73 2f70 6572  roto.8protos/per
+00009240: 6665 7474 6f2f 6d65 7472 6963 732f 616e  fetto/metrics/an
+00009250: 6472 6f69 642f 6972 715f 7275 6e74 696d  droid/irq_runtim
+00009260: 655f 6d65 7472 6963 2e70 726f 746f 1a35  e_metric.proto.5
+00009270: 7072 6f74 6f73 2f70 6572 6665 7474 6f2f  protos/perfetto/
+00009280: 6d65 7472 6963 732f 616e 6472 6f69 642f  metrics/android/
+00009290: 6a61 6e6b 5f63 756a 5f6d 6574 7269 632e  jank_cuj_metric.
+000092a0: 7072 6f74 6f1a 3970 726f 746f 732f 7065  proto.9protos/pe
+000092b0: 7266 6574 746f 2f6d 6574 7269 6373 2f61  rfetto/metrics/a
+000092c0: 6e64 726f 6964 2f6a 6176 615f 6865 6170  ndroid/java_heap
+000092d0: 5f68 6973 746f 6772 616d 2e70 726f 746f  _histogram.proto
+000092e0: 1a35 7072 6f74 6f73 2f70 6572 6665 7474  .5protos/perfett
+000092f0: 6f2f 6d65 7472 6963 732f 616e 6472 6f69  o/metrics/androi
+00009300: 642f 6a61 7661 5f68 6561 705f 7374 6174  d/java_heap_stat
+00009310: 732e 7072 6f74 6f1a 3070 726f 746f 732f  s.proto.0protos/
+00009320: 7065 7266 6574 746f 2f6d 6574 7269 6373  perfetto/metrics
+00009330: 2f61 6e64 726f 6964 2f6c 6d6b 5f6d 6574  /android/lmk_met
+00009340: 7269 632e 7072 6f74 6f1a 3770 726f 746f  ric.proto.7proto
+00009350: 732f 7065 7266 6574 746f 2f6d 6574 7269  s/perfetto/metri
+00009360: 6373 2f61 6e64 726f 6964 2f6c 6d6b 5f72  cs/android/lmk_r
+00009370: 6561 736f 6e5f 6d65 7472 6963 2e70 726f  eason_metric.pro
+00009380: 746f 1a30 7072 6f74 6f73 2f70 6572 6665  to.0protos/perfe
+00009390: 7474 6f2f 6d65 7472 6963 732f 616e 6472  tto/metrics/andr
+000093a0: 6f69 642f 6d65 6d5f 6d65 7472 6963 2e70  oid/mem_metric.p
+000093b0: 726f 746f 1a36 7072 6f74 6f73 2f70 6572  roto.6protos/per
+000093c0: 6665 7474 6f2f 6d65 7472 6963 732f 616e  fetto/metrics/an
+000093d0: 6472 6f69 642f 6d65 6d5f 756e 6167 675f  droid/mem_unagg_
+000093e0: 6d65 7472 6963 2e70 726f 746f 1a36 7072  metric.proto.6pr
+000093f0: 6f74 6f73 2f70 6572 6665 7474 6f2f 6d65  otos/perfetto/me
+00009400: 7472 6963 732f 616e 6472 6f69 642f 6d75  trics/android/mu
+00009410: 6c74 6975 7365 725f 6d65 7472 6963 2e70  ltiuser_metric.p
+00009420: 726f 746f 1a34 7072 6f74 6f73 2f70 6572  roto.4protos/per
+00009430: 6665 7474 6f2f 6d65 7472 6963 732f 616e  fetto/metrics/an
+00009440: 6472 6f69 642f 6e65 7477 6f72 6b5f 6d65  droid/network_me
+00009450: 7472 6963 2e70 726f 746f 1a32 7072 6f74  tric.proto.2prot
+00009460: 6f73 2f70 6572 6665 7474 6f2f 6d65 7472  os/perfetto/metr
+00009470: 6963 732f 616e 6472 6f69 642f 6f74 6865  ics/android/othe
+00009480: 725f 7472 6163 6573 2e70 726f 746f 1a32  r_traces.proto.2
+00009490: 7072 6f74 6f73 2f70 6572 6665 7474 6f2f  protos/perfetto/
+000094a0: 6d65 7472 6963 732f 616e 6472 6f69 642f  metrics/android/
+000094b0: 7061 636b 6167 655f 6c69 7374 2e70 726f  package_list.pro
+000094c0: 746f 1a35 7072 6f74 6f73 2f70 6572 6665  to.5protos/perfe
+000094d0: 7474 6f2f 6d65 7472 6963 732f 616e 6472  tto/metrics/andr
+000094e0: 6f69 642f 706f 7772 6169 6c73 5f6d 6574  oid/powrails_met
+000094f0: 7269 632e 7072 6f74 6f1a 3470 726f 746f  ric.proto.4proto
+00009500: 732f 7065 7266 6574 746f 2f6d 6574 7269  s/perfetto/metri
+00009510: 6373 2f61 6e64 726f 6964 2f70 726f 6669  cs/android/profi
+00009520: 6c65 725f 736d 6170 732e 7072 6f74 6f1a  ler_smaps.proto.
+00009530: 3770 726f 746f 732f 7065 7266 6574 746f  7protos/perfetto
+00009540: 2f6d 6574 7269 6373 2f61 6e64 726f 6964  /metrics/android
+00009550: 2f72 745f 7275 6e74 696d 655f 6d65 7472  /rt_runtime_metr
+00009560: 6963 2e70 726f 746f 1a30 7072 6f74 6f73  ic.proto.0protos
+00009570: 2f70 6572 6665 7474 6f2f 6d65 7472 6963  /perfetto/metric
+00009580: 732f 616e 6472 6f69 642f 7369 6d70 6c65  s/android/simple
+00009590: 7065 7266 2e70 726f 746f 1a34 7072 6f74  perf.proto.4prot
+000095a0: 6f73 2f70 6572 6665 7474 6f2f 6d65 7472  os/perfetto/metr
+000095b0: 6963 732f 616e 6472 6f69 642f 7374 6172  ics/android/star
+000095c0: 7475 705f 6d65 7472 6963 2e70 726f 746f  tup_metric.proto
+000095d0: 1a34 7072 6f74 6f73 2f70 6572 6665 7474  .4protos/perfett
+000095e0: 6f2f 6d65 7472 6963 732f 616e 6472 6f69  o/metrics/androi
+000095f0: 642f 7375 7266 6163 6566 6c69 6e67 6572  d/surfaceflinger
+00009600: 2e70 726f 746f 1a30 7072 6f74 6f73 2f70  .proto.0protos/p
+00009610: 6572 6665 7474 6f2f 6d65 7472 6963 732f  erfetto/metrics/
+00009620: 616e 6472 6f69 642f 7461 736b 5f6e 616d  android/task_nam
+00009630: 6573 2e70 726f 746f 1a33 7072 6f74 6f73  es.proto.3protos
+00009640: 2f70 6572 6665 7474 6f2f 6d65 7472 6963  /perfetto/metric
+00009650: 732f 616e 6472 6f69 642f 7472 6163 655f  s/android/trace_
+00009660: 7175 616c 6974 792e 7072 6f74 6f1a 3f70  quality.proto.?p
+00009670: 726f 746f 732f 7065 7266 6574 746f 2f6d  rotos/perfetto/m
+00009680: 6574 7269 6373 2f61 6e64 726f 6964 2f61  etrics/android/a
+00009690: 6e64 726f 6964 5f74 7275 7374 795f 776f  ndroid_trusty_wo
+000096a0: 726b 7175 6575 6573 2e70 726f 746f 1a39  rkqueues.proto.9
+000096b0: 7072 6f74 6f73 2f70 6572 6665 7474 6f2f  protos/perfetto/
+000096c0: 6d65 7472 6963 732f 616e 6472 6f69 642f  metrics/android/
+000096d0: 756e 7379 6d62 6f6c 697a 6564 5f66 7261  unsymbolized_fra
+000096e0: 6d65 732e 7072 6f74 6f1a 3370 726f 746f  mes.proto.3proto
+000096f0: 732f 7065 7266 6574 746f 2f6d 6574 7269  s/perfetto/metri
+00009700: 6373 2f61 6e64 726f 6964 2f62 696e 6465  cs/android/binde
+00009710: 725f 6d65 7472 6963 2e70 726f 746f 1a3f  r_metric.proto.?
+00009720: 7072 6f74 6f73 2f70 6572 6665 7474 6f2f  protos/perfetto/
+00009730: 6d65 7472 6963 732f 616e 6472 6f69 642f  metrics/android/
+00009740: 6d6f 6e69 746f 725f 636f 6e74 656e 7469  monitor_contenti
+00009750: 6f6e 5f6d 6574 7269 632e 7072 6f74 6f22  on_metric.proto"
+00009760: c003 0a0d 5472 6163 654d 6574 6164 6174  ....TraceMetadat
+00009770: 6112 2a0a 1174 7261 6365 5f64 7572 6174  a.*..trace_durat
+00009780: 696f 6e5f 6e73 1802 2001 2803 520f 7472  ion_ns.. .(.R.tr
+00009790: 6163 6544 7572 6174 696f 6e4e 7312 1d0a  aceDurationNs...
+000097a0: 0a74 7261 6365 5f75 7569 6418 0320 0128  .trace_uuid.. .(
+000097b0: 0952 0974 7261 6365 5575 6964 123a 0a19  .R.traceUuid.:..
+000097c0: 616e 6472 6f69 645f 6275 696c 645f 6669  android_build_fi
+000097d0: 6e67 6572 7072 696e 7418 0420 0128 0952  ngerprint.. .(.R
+000097e0: 1761 6e64 726f 6964 4275 696c 6446 696e  .androidBuildFin
+000097f0: 6765 7270 7269 6e74 1249 0a21 7374 6174  gerprint.I.!stat
+00009800: 7364 5f74 7269 6767 6572 696e 675f 7375  sd_triggering_su
+00009810: 6273 6372 6970 7469 6f6e 5f69 6418 0520  bscription_id.. 
+00009820: 0128 0352 1e73 7461 7473 6454 7269 6767  .(.R.statsdTrigg
+00009830: 6572 696e 6753 7562 7363 7269 7074 696f  eringSubscriptio
+00009840: 6e49 6412 280a 1074 7261 6365 5f73 697a  nId.(..trace_siz
+00009850: 655f 6279 7465 7318 0620 0128 0352 0e74  e_bytes.. .(.R.t
+00009860: 7261 6365 5369 7a65 4279 7465 7312 230a  raceSizeBytes.#.
+00009870: 0d74 7261 6365 5f74 7269 6767 6572 1807  .trace_trigger..
+00009880: 2003 2809 520c 7472 6163 6554 7269 6767   .(.R.traceTrigg
+00009890: 6572 122e 0a13 756e 6971 7565 5f73 6573  er....unique_ses
+000098a0: 7369 6f6e 5f6e 616d 6518 0820 0128 0952  sion_name.. .(.R
+000098b0: 1175 6e69 7175 6553 6573 7369 6f6e 4e61  .uniqueSessionNa
+000098c0: 6d65 122c 0a12 7472 6163 655f 636f 6e66  me.,..trace_conf
+000098d0: 6967 5f70 6274 7874 1809 2001 2809 5210  ig_pbtxt.. .(.R.
+000098e0: 7472 6163 6543 6f6e 6669 6750 6274 7874  traceConfigPbtxt
+000098f0: 122a 0a11 7363 6865 645f 6475 7261 7469  .*..sched_durati
+00009900: 6f6e 5f6e 7318 0a20 0128 0352 0f73 6368  on_ns.. .(.R.sch
+00009910: 6564 4475 7261 7469 6f6e 4e73 4a04 0801  edDurationNsJ...
+00009920: 1002 22cb 030a 1254 7261 6365 416e 616c  .."....TraceAnal
+00009930: 7973 6973 5374 6174 7312 3c0a 0473 7461  ysisStats.<..sta
+00009940: 7418 0120 0328 0b32 282e 7065 7266 6574  t.. .(.2(.perfet
+00009950: 746f 2e70 726f 746f 732e 5472 6163 6541  to.protos.TraceA
+00009960: 6e61 6c79 7369 7353 7461 7473 2e53 7461  nalysisStats.Sta
+00009970: 7452 0473 7461 741a d001 0a04 5374 6174  tR.stat.....Stat
+00009980: 1212 0a04 6e61 6d65 1801 2001 2809 5204  ....name.. .(.R.
+00009990: 6e61 6d65 1210 0a03 6964 7818 0220 0128  name....idx.. .(
+000099a0: 0d52 0369 6478 1248 0a08 7365 7665 7269  .R.idx.H..severi
+000099b0: 7479 1803 2001 280e 322c 2e70 6572 6665  ty.. .(.2,.perfe
+000099c0: 7474 6f2e 7072 6f74 6f73 2e54 7261 6365  tto.protos.Trace
+000099d0: 416e 616c 7973 6973 5374 6174 732e 5365  AnalysisStats.Se
+000099e0: 7665 7269 7479 5208 7365 7665 7269 7479  verityR.severity
+000099f0: 1242 0a06 736f 7572 6365 1804 2001 280e  .B..source.. .(.
+00009a00: 322a 2e70 6572 6665 7474 6f2e 7072 6f74  2*.perfetto.prot
+00009a10: 6f73 2e54 7261 6365 416e 616c 7973 6973  os.TraceAnalysis
+00009a20: 5374 6174 732e 536f 7572 6365 5206 736f  Stats.SourceR.so
+00009a30: 7572 6365 1214 0a05 636f 756e 7418 0520  urce....count.. 
+00009a40: 0128 0352 0563 6f75 6e74 225f 0a08 5365  .(.R.count"_..Se
+00009a50: 7665 7269 7479 1214 0a10 5345 5645 5249  verity....SEVERI
+00009a60: 5459 5f55 4e4b 4e4f 574e 1000 1211 0a0d  TY_UNKNOWN......
+00009a70: 5345 5645 5249 5459 5f49 4e46 4f10 0112  SEVERITY_INFO...
+00009a80: 160a 1253 4556 4552 4954 595f 4441 5441  ...SEVERITY_DATA
+00009a90: 5f4c 4f53 5310 0212 120a 0e53 4556 4552  _LOSS......SEVER
+00009aa0: 4954 595f 4552 524f 5210 0322 430a 0653  ITY_ERROR.."C..S
+00009ab0: 6f75 7263 6512 120a 0e53 4f55 5243 455f  ource....SOURCE_
+00009ac0: 554e 4b4e 4f57 4e10 0012 100a 0c53 4f55  UNKNOWN......SOU
+00009ad0: 5243 455f 5452 4143 4510 0112 130a 0f53  RCE_TRACE......S
+00009ae0: 4f55 5243 455f 414e 414c 5953 4953 1002  OURCE_ANALYSIS..
+00009af0: 22bd 1b0a 0c54 7261 6365 4d65 7472 6963  "....TraceMetric
+00009b00: 7312 480a 0c61 6e64 726f 6964 5f62 6174  s.H..android_bat
+00009b10: 7418 0520 0128 0b32 252e 7065 7266 6574  t.. .(.2%.perfet
+00009b20: 746f 2e70 726f 746f 732e 416e 6472 6f69  to.protos.Androi
+00009b30: 6442 6174 7465 7279 4d65 7472 6963 520b  dBatteryMetricR.
+00009b40: 616e 6472 6f69 6442 6174 7412 420a 0b61  androidBatt.B..a
+00009b50: 6e64 726f 6964 5f63 7075 1806 2001 280b  ndroid_cpu.. .(.
+00009b60: 3221 2e70 6572 6665 7474 6f2e 7072 6f74  2!.perfetto.prot
+00009b70: 6f73 2e41 6e64 726f 6964 4370 754d 6574  os.AndroidCpuMet
+00009b80: 7269 6352 0a61 6e64 726f 6964 4370 7512  ricR.androidCpu.
+00009b90: 450a 0b61 6e64 726f 6964 5f6d 656d 1801  E..android_mem..
+00009ba0: 2001 280b 3224 2e70 6572 6665 7474 6f2e   .(.2$.perfetto.
+00009bb0: 7072 6f74 6f73 2e41 6e64 726f 6964 4d65  protos.AndroidMe
+00009bc0: 6d6f 7279 4d65 7472 6963 520a 616e 6472  moryMetricR.andr
+00009bd0: 6f69 644d 656d 125c 0a11 616e 6472 6f69  oidMem.\..androi
+00009be0: 645f 6d65 6d5f 756e 6167 6718 0b20 0128  d_mem_unagg.. .(
+00009bf0: 0b32 302e 7065 7266 6574 746f 2e70 726f  .20.perfetto.pro
+00009c00: 746f 732e 416e 6472 6f69 644d 656d 6f72  tos.AndroidMemor
+00009c10: 7955 6e61 6767 7265 6761 7465 644d 6574  yUnaggregatedMet
+00009c20: 7269 6352 0f61 6e64 726f 6964 4d65 6d55  ricR.androidMemU
+00009c30: 6e61 6767 1255 0a14 616e 6472 6f69 645f  nagg.U..android_
+00009c40: 7061 636b 6167 655f 6c69 7374 180c 2001  package_list.. .
+00009c50: 280b 3223 2e70 6572 6665 7474 6f2e 7072  (.2#.perfetto.pr
+00009c60: 6f74 6f73 2e41 6e64 726f 6964 5061 636b  otos.AndroidPack
+00009c70: 6167 654c 6973 7452 1261 6e64 726f 6964  ageListR.android
+00009c80: 5061 636b 6167 654c 6973 7412 420a 0b61  PackageList.B..a
+00009c90: 6e64 726f 6964 5f69 6f6e 1809 2001 280b  ndroid_ion.. .(.
+00009ca0: 3221 2e70 6572 6665 7474 6f2e 7072 6f74  2!.perfetto.prot
+00009cb0: 6f73 2e41 6e64 726f 6964 496f 6e4d 6574  os.AndroidIonMet
+00009cc0: 7269 6352 0a61 6e64 726f 6964 496f 6e12  ricR.androidIon.
+00009cd0: 4e0a 0f61 6e64 726f 6964 5f66 6173 7472  N..android_fastr
+00009ce0: 7063 181f 2001 280b 3225 2e70 6572 6665  pc.. .(.2%.perfe
+00009cf0: 7474 6f2e 7072 6f74 6f73 2e41 6e64 726f  tto.protos.Andro
+00009d00: 6964 4661 7374 7270 634d 6574 7269 6352  idFastrpcMetricR
+00009d10: 0e61 6e64 726f 6964 4661 7374 7270 6312  .androidFastrpc.
+00009d20: 420a 0b61 6e64 726f 6964 5f6c 6d6b 1808  B..android_lmk..
+00009d30: 2001 280b 3221 2e70 6572 6665 7474 6f2e   .(.2!.perfetto.
+00009d40: 7072 6f74 6f73 2e41 6e64 726f 6964 4c6d  protos.AndroidLm
+00009d50: 6b4d 6574 7269 6352 0a61 6e64 726f 6964  kMetricR.android
+00009d60: 4c6d 6b12 4d0a 1061 6e64 726f 6964 5f70  Lmk.M..android_p
+00009d70: 6f77 7261 696c 7318 0720 0128 0b32 222e  owrails.. .(.2".
+00009d80: 7065 7266 6574 746f 2e70 726f 746f 732e  perfetto.protos.
+00009d90: 416e 6472 6f69 6450 6f77 6572 5261 696c  AndroidPowerRail
+00009da0: 7352 0f61 6e64 726f 6964 506f 7772 6169  sR.androidPowrai
+00009db0: 6c73 124e 0a0f 616e 6472 6f69 645f 7374  ls.N..android_st
+00009dc0: 6172 7475 7018 0220 0128 0b32 252e 7065  artup.. .(.2%.pe
+00009dd0: 7266 6574 746f 2e70 726f 746f 732e 416e  rfetto.protos.An
+00009de0: 6472 6f69 6453 7461 7274 7570 4d65 7472  droidStartupMetr
+00009df0: 6963 520e 616e 6472 6f69 6453 7461 7274  icR.androidStart
+00009e00: 7570 1245 0a0e 7472 6163 655f 6d65 7461  up.E..trace_meta
+00009e10: 6461 7461 1803 2001 280b 321e 2e70 6572  data.. .(.2..per
+00009e20: 6665 7474 6f2e 7072 6f74 6f73 2e54 7261  fetto.protos.Tra
+00009e30: 6365 4d65 7461 6461 7461 520d 7472 6163  ceMetadataR.trac
+00009e40: 654d 6574 6164 6174 6112 440a 0b74 7261  eMetadata.D..tra
+00009e50: 6365 5f73 7461 7473 1821 2001 280b 3223  ce_stats.! .(.2#
+00009e60: 2e70 6572 6665 7474 6f2e 7072 6f74 6f73  .perfetto.protos
+00009e70: 2e54 7261 6365 416e 616c 7973 6973 5374  .TraceAnalysisSt
+00009e80: 6174 7352 0a74 7261 6365 5374 6174 7312  atsR.traceStats.
+00009e90: 540a 1375 6e73 796d 626f 6c69 7a65 645f  T..unsymbolized_
+00009ea0: 6672 616d 6573 180f 2001 280b 3223 2e70  frames.. .(.2#.p
+00009eb0: 6572 6665 7474 6f2e 7072 6f74 6f73 2e55  erfetto.protos.U
+00009ec0: 6e73 796d 626f 6c69 7a65 6446 7261 6d65  nsymbolizedFrame
+00009ed0: 7352 1275 6e73 796d 626f 6c69 7a65 6446  sR.unsymbolizedF
+00009ee0: 7261 6d65 7312 460a 0f6a 6176 615f 6865  rames.F..java_he
+00009ef0: 6170 5f73 7461 7473 1811 2001 280b 321e  ap_stats.. .(.2.
+00009f00: 2e70 6572 6665 7474 6f2e 7072 6f74 6f73  .perfetto.protos
+00009f10: 2e4a 6176 6148 6561 7053 7461 7473 520d  .JavaHeapStatsR.
+00009f20: 6a61 7661 4865 6170 5374 6174 7312 520a  javaHeapStats.R.
+00009f30: 136a 6176 615f 6865 6170 5f68 6973 746f  .java_heap_histo
+00009f40: 6772 616d 1815 2001 280b 3222 2e70 6572  gram.. .(.2".per
+00009f50: 6665 7474 6f2e 7072 6f74 6f73 2e4a 6176  fetto.protos.Jav
+00009f60: 6148 6561 7048 6973 746f 6772 616d 5211  aHeapHistogramR.
+00009f70: 6a61 7661 4865 6170 4869 7374 6f67 7261  javaHeapHistogra
+00009f80: 6d12 550a 1261 6e64 726f 6964 5f6c 6d6b  m.U..android_lmk
+00009f90: 5f72 6561 736f 6e18 1220 0128 0b32 272e  _reason.. .(.2'.
+00009fa0: 7065 7266 6574 746f 2e70 726f 746f 732e  perfetto.protos.
+00009fb0: 416e 6472 6f69 644c 6d6b 5265 6173 6f6e  AndroidLmkReason
+00009fc0: 4d65 7472 6963 5210 616e 6472 6f69 644c  MetricR.androidL
+00009fd0: 6d6b 5265 6173 6f6e 1252 0a13 616e 6472  mkReason.R..andr
+00009fe0: 6f69 645f 6877 7569 5f6d 6574 7269 6318  oid_hwui_metric.
+00009ff0: 1420 0128 0b32 222e 7065 7266 6574 746f  . .(.2".perfetto
+0000a000: 2e70 726f 746f 732e 416e 6472 6f69 6448  .protos.AndroidH
+0000a010: 7775 694d 6574 7269 6352 1161 6e64 726f  wuiMetricR.andro
+0000a020: 6964 4877 7569 4d65 7472 6963 124f 0a0f  idHwuiMetric.O..
+0000a030: 6469 7370 6c61 795f 6d65 7472 6963 7318  display_metrics.
+0000a040: 1620 0128 0b32 262e 7065 7266 6574 746f  . .(.2&.perfetto
+0000a050: 2e70 726f 746f 732e 416e 6472 6f69 6444  .protos.AndroidD
+0000a060: 6973 706c 6179 4d65 7472 6963 7352 0e64  isplayMetricsR.d
+0000a070: 6973 706c 6179 4d65 7472 6963 7312 4f0a  isplayMetrics.O.
+0000a080: 1261 6e64 726f 6964 5f74 6173 6b5f 6e61  .android_task_na
+0000a090: 6d65 7318 1720 0128 0b32 212e 7065 7266  mes.. .(.2!.perf
+0000a0a0: 6574 746f 2e70 726f 746f 732e 416e 6472  etto.protos.Andr
+0000a0b0: 6f69 6454 6173 6b4e 616d 6573 5210 616e  oidTaskNamesR.an
+0000a0c0: 6472 6f69 6454 6173 6b4e 616d 6573 1263  droidTaskNames.c
+0000a0d0: 0a16 616e 6472 6f69 645f 7375 7266 6163  ..android_surfac
+0000a0e0: 6566 6c69 6e67 6572 1819 2001 280b 322c  eflinger.. .(.2,
+0000a0f0: 2e70 6572 6665 7474 6f2e 7072 6f74 6f73  .perfetto.protos
+0000a100: 2e41 6e64 726f 6964 5375 7266 6163 6566  .AndroidSurfacef
+0000a110: 6c69 6e67 6572 4d65 7472 6963 5215 616e  lingerMetricR.an
+0000a120: 6472 6f69 6453 7572 6661 6365 666c 696e  droidSurfaceflin
+0000a130: 6765 7212 420a 0b61 6e64 726f 6964 5f67  ger.B..android_g
+0000a140: 7075 181a 2001 280b 3221 2e70 6572 6665  pu.. .(.2!.perfe
+0000a150: 7474 6f2e 7072 6f74 6f73 2e41 6e64 726f  tto.protos.Andro
+0000a160: 6964 4770 754d 6574 7269 6352 0a61 6e64  idGpuMetricR.and
+0000a170: 726f 6964 4770 7512 4f0a 1061 6e64 726f  roidGpu.O..andro
+0000a180: 6964 5f6a 616e 6b5f 6375 6a18 3020 0128  id_jank_cuj.0 .(
+0000a190: 0b32 252e 7065 7266 6574 746f 2e70 726f  .2%.perfetto.pro
+0000a1a0: 746f 732e 416e 6472 6f69 644a 616e 6b43  tos.AndroidJankC
+0000a1b0: 756a 4d65 7472 6963 520e 616e 6472 6f69  ujMetricR.androi
+0000a1c0: 644a 616e 6b43 756a 1258 0a12 616e 6472  dJankCuj.X..andr
+0000a1d0: 6f69 645f 6877 636f 6d70 6f73 6572 181c  oid_hwcomposer..
+0000a1e0: 2001 280b 3229 2e70 6572 6665 7474 6f2e   .(.2).perfetto.
+0000a1f0: 7072 6f74 6f73 2e41 6e64 726f 6964 4877  protos.AndroidHw
+0000a200: 636f 6d70 6f73 6572 4d65 7472 6963 7352  composerMetricsR
+0000a210: 1161 6e64 726f 6964 4877 636f 6d70 6f73  .androidHwcompos
+0000a220: 6572 122d 0a03 6732 6418 1e20 0128 0b32  er.-..g2d.. .(.2
+0000a230: 1b2e 7065 7266 6574 746f 2e70 726f 746f  ..perfetto.proto
+0000a240: 732e 4732 644d 6574 7269 6373 5203 6732  s.G2dMetricsR.g2
+0000a250: 6412 4f0a 1061 6e64 726f 6964 5f64 6d61  d.O..android_dma
+0000a260: 5f68 6561 7018 2020 0128 0b32 252e 7065  _heap.  .(.2%.pe
+0000a270: 7266 6574 746f 2e70 726f 746f 732e 416e  rfetto.protos.An
+0000a280: 6472 6f69 6444 6d61 4865 6170 4d65 7472  droidDmaHeapMetr
+0000a290: 6963 520e 616e 6472 6f69 6444 6d61 4865  icR.androidDmaHe
+0000a2a0: 6170 125e 0a15 616e 6472 6f69 645f 7472  ap.^..android_tr
+0000a2b0: 6163 655f 7175 616c 6974 7918 2220 0128  ace_quality." .(
+0000a2c0: 0b32 2a2e 7065 7266 6574 746f 2e70 726f  .2*.perfetto.pro
+0000a2d0: 746f 732e 416e 6472 6f69 6454 7261 6365  tos.AndroidTrace
+0000a2e0: 5175 616c 6974 794d 6574 7269 6352 1361  QualityMetricR.a
+0000a2f0: 6e64 726f 6964 5472 6163 6551 7561 6c69  ndroidTraceQuali
+0000a300: 7479 1245 0a0e 7072 6f66 696c 6572 5f73  ty.E..profiler_s
+0000a310: 6d61 7073 1823 2001 280b 321e 2e70 6572  maps.# .(.2..per
+0000a320: 6665 7474 6f2e 7072 6f74 6f73 2e50 726f  fetto.protos.Pro
+0000a330: 6669 6c65 7253 6d61 7073 520d 7072 6f66  filerSmapsR.prof
+0000a340: 696c 6572 536d 6170 7312 540a 1161 6e64  ilerSmaps.T..and
+0000a350: 726f 6964 5f6d 756c 7469 7573 6572 1824  roid_multiuser.$
+0000a360: 2001 280b 3227 2e70 6572 6665 7474 6f2e   .(.2'.perfetto.
+0000a370: 7072 6f74 6f73 2e41 6e64 726f 6964 4d75  protos.AndroidMu
+0000a380: 6c74 6975 7365 724d 6574 7269 6352 1061  ltiuserMetricR.a
+0000a390: 6e64 726f 6964 4d75 6c74 6975 7365 7212  ndroidMultiuser.
+0000a3a0: 570a 1261 6e64 726f 6964 5f73 696d 706c  W..android_simpl
+0000a3b0: 6570 6572 6618 2520 0128 0b32 282e 7065  eperf.% .(.2(.pe
+0000a3c0: 7266 6574 746f 2e70 726f 746f 732e 416e  rfetto.protos.An
+0000a3d0: 6472 6f69 6453 696d 706c 6570 6572 664d  droidSimpleperfM
+0000a3e0: 6574 7269 6352 1161 6e64 726f 6964 5369  etricR.androidSi
+0000a3f0: 6d70 6c65 7065 7266 124b 0a0e 616e 6472  mpleperf.K..andr
+0000a400: 6f69 645f 6361 6d65 7261 1826 2001 280b  oid_camera.& .(.
+0000a410: 3224 2e70 6572 6665 7474 6f2e 7072 6f74  2$.perfetto.prot
+0000a420: 6f73 2e41 6e64 726f 6964 4361 6d65 7261  os.AndroidCamera
+0000a430: 4d65 7472 6963 520d 616e 6472 6f69 6443  MetricR.androidC
+0000a440: 616d 6572 6112 450a 0c61 6e64 726f 6964  amera.E..android
+0000a450: 5f64 7666 7318 2720 0128 0b32 222e 7065  _dvfs.' .(.2".pe
+0000a460: 7266 6574 746f 2e70 726f 746f 732e 416e  rfetto.protos.An
+0000a470: 6472 6f69 6444 7666 734d 6574 7269 6352  droidDvfsMetricR
+0000a480: 0b61 6e64 726f 6964 4476 6673 124e 0a0f  .androidDvfs.N..
+0000a490: 616e 6472 6f69 645f 6e65 7470 6572 6618  android_netperf.
+0000a4a0: 2820 0128 0b32 252e 7065 7266 6574 746f  ( .(.2%.perfetto
+0000a4b0: 2e70 726f 746f 732e 416e 6472 6f69 644e  .protos.AndroidN
+0000a4c0: 6574 776f 726b 4d65 7472 6963 520e 616e  etworkMetricR.an
+0000a4d0: 6472 6f69 644e 6574 7065 7266 1262 0a14  droidNetperf.b..
+0000a4e0: 616e 6472 6f69 645f 6361 6d65 7261 5f75  android_camera_u
+0000a4f0: 6e61 6767 1829 2001 280b 3230 2e70 6572  nagg.) .(.20.per
+0000a500: 6665 7474 6f2e 7072 6f74 6f73 2e41 6e64  fetto.protos.And
+0000a510: 726f 6964 4361 6d65 7261 556e 6167 6772  roidCameraUnaggr
+0000a520: 6567 6174 6564 4d65 7472 6963 5212 616e  egatedMetricR.an
+0000a530: 6472 6f69 6443 616d 6572 6155 6e61 6767  droidCameraUnagg
+0000a540: 1255 0a12 616e 6472 6f69 645f 7274 5f72  .U..android_rt_r
+0000a550: 756e 7469 6d65 182a 2001 280b 3227 2e70  untime.* .(.2'.p
+0000a560: 6572 6665 7474 6f2e 7072 6f74 6f73 2e41  erfetto.protos.A
+0000a570: 6e64 726f 6964 5274 5275 6e74 696d 654d  ndroidRtRuntimeM
+0000a580: 6574 7269 6352 1061 6e64 726f 6964 5274  etricR.androidRt
+0000a590: 5275 6e74 696d 6512 580a 1361 6e64 726f  Runtime.X..andro
+0000a5a0: 6964 5f69 7271 5f72 756e 7469 6d65 182b  id_irq_runtime.+
+0000a5b0: 2001 280b 3228 2e70 6572 6665 7474 6f2e   .(.2(.perfetto.
+0000a5c0: 7072 6f74 6f73 2e41 6e64 726f 6964 4972  protos.AndroidIr
+0000a5d0: 7152 756e 7469 6d65 4d65 7472 6963 5211  qRuntimeMetricR.
+0000a5e0: 616e 6472 6f69 6449 7271 5275 6e74 696d  androidIrqRuntim
+0000a5f0: 6512 640a 1961 6e64 726f 6964 5f74 7275  e.d..android_tru
+0000a600: 7374 795f 776f 726b 7175 6575 6573 182c  sty_workqueues.,
+0000a610: 2001 280b 3228 2e70 6572 6665 7474 6f2e   .(.2(.perfetto.
+0000a620: 7072 6f74 6f73 2e41 6e64 726f 6964 5472  protos.AndroidTr
+0000a630: 7573 7479 576f 726b 7175 6575 6573 5217  ustyWorkqueuesR.
+0000a640: 616e 6472 6f69 6454 7275 7374 7957 6f72  androidTrustyWor
+0000a650: 6b71 7565 7565 7312 5b0a 1461 6e64 726f  kqueues.[..andro
+0000a660: 6964 5f6f 7468 6572 5f74 7261 6365 7318  id_other_traces.
+0000a670: 2d20 0128 0b32 292e 7065 7266 6574 746f  - .(.2).perfetto
+0000a680: 2e70 726f 746f 732e 416e 6472 6f69 644f  .protos.AndroidO
+0000a690: 7468 6572 5472 6163 6573 4d65 7472 6963  therTracesMetric
+0000a6a0: 5212 616e 6472 6f69 644f 7468 6572 5472  R.androidOtherTr
+0000a6b0: 6163 6573 124b 0a0e 616e 6472 6f69 645f  aces.K..android_
+0000a6c0: 6269 6e64 6572 182e 2001 280b 3224 2e70  binder.. .(.2$.p
+0000a6d0: 6572 6665 7474 6f2e 7072 6f74 6f73 2e41  erfetto.protos.A
+0000a6e0: 6e64 726f 6964 4269 6e64 6572 4d65 7472  ndroidBinderMetr
+0000a6f0: 6963 520d 616e 6472 6f69 6442 696e 6465  icR.androidBinde
+0000a700: 7212 6e0a 1d61 6e64 726f 6964 5f66 7261  r.n..android_fra
+0000a710: 6d65 5f74 696d 656c 696e 655f 6d65 7472  me_timeline_metr
+0000a720: 6963 182f 2001 280b 322b 2e70 6572 6665  ic./ .(.2+.perfe
+0000a730: 7474 6f2e 7072 6f74 6f73 2e41 6e64 726f  tto.protos.Andro
+0000a740: 6964 4672 616d 6554 696d 656c 696e 654d  idFrameTimelineM
+0000a750: 6574 7269 6352 1a61 6e64 726f 6964 4672  etricR.androidFr
+0000a760: 616d 6554 696d 656c 696e 654d 6574 7269  ameTimelineMetri
+0000a770: 6312 780a 2161 6e64 726f 6964 5f62 6c6f  c.x.!android_blo
+0000a780: 636b 696e 675f 6361 6c6c 735f 6375 6a5f  cking_calls_cuj_
+0000a790: 6d65 7472 6963 1831 2001 280b 322e 2e70  metric.1 .(.2..p
+0000a7a0: 6572 6665 7474 6f2e 7072 6f74 6f73 2e41  erfetto.protos.A
+0000a7b0: 6e64 726f 6964 426c 6f63 6b69 6e67 4361  ndroidBlockingCa
+0000a7c0: 6c6c 7343 756a 4d65 7472 6963 521d 616e  llsCujMetricR.an
+0000a7d0: 6472 6f69 6442 6c6f 636b 696e 6743 616c  droidBlockingCal
+0000a7e0: 6c73 4375 6a4d 6574 7269 6312 6d0a 1a61  lsCujMetric.m..a
+0000a7f0: 6e64 726f 6964 5f6d 6f6e 6974 6f72 5f63  ndroid_monitor_c
+0000a800: 6f6e 7465 6e74 696f 6e18 3220 0128 0b32  ontention.2 .(.2
+0000a810: 2f2e 7065 7266 6574 746f 2e70 726f 746f  /.perfetto.proto
+0000a820: 732e 416e 6472 6f69 644d 6f6e 6974 6f72  s.AndroidMonitor
+0000a830: 436f 6e74 656e 7469 6f6e 4d65 7472 6963  ContentionMetric
+0000a840: 5218 616e 6472 6f69 644d 6f6e 6974 6f72  R.androidMonitor
+0000a850: 436f 6e74 656e 7469 6f6e 2a06 08c2 0310  Contention*.....
+0000a860: f403 2a06 08f4 0310 e907 2a06 08e9 0710  ..*.......*.....
+0000a870: d10f 2a06 08d1 0f10 c513 4a04 0804 1005  ..*.......J.....
+0000a880: 4a04 080a 100b 4a04 080d 100e 4a04 080e  J.....J.....J...
+0000a890: 100f 4a04 0810 1011 4a04 0813 1014 4a04  ..J.....J.....J.
+0000a8a0: 0818 1019 4a04 081b 101c 4a04 081d 101e  ....J.....J.....
```

### Comparing `perfetto-0.6.0/perfetto/trace_processor/platform.py` & `perfetto-0.7.0/perfetto/trace_processor/platform.py`

 * *Files identical despite different names*

### Comparing `perfetto-0.6.0/perfetto/trace_processor/protos.py` & `perfetto-0.7.0/perfetto/trace_processor/protos.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,16 @@
     metrics_file_desc_set_pb2.MergeFromString(metrics_desc)
 
     for f_desc_pb2 in metrics_file_desc_set_pb2.file:
       self.descriptor_pool.Add(f_desc_pb2)
 
     def create_message_factory(message_type):
       message_desc = self.descriptor_pool.FindMessageTypeByName(message_type)
+      if hasattr(message_factory, 'GetMessageClass'):
+        return message_factory.GetMessageClass(message_desc)
       return message_factory.MessageFactory().GetPrototype(message_desc)
 
     # Create proto messages to correctly communicate with the RPC API by sending
     # and receiving data as protos
     self.AppendTraceDataResult = create_message_factory(
         'perfetto.protos.AppendTraceDataResult')
     self.StatusResult = create_message_factory('perfetto.protos.StatusResult')
```

### Comparing `perfetto-0.6.0/perfetto/trace_processor/shell.py` & `perfetto-0.7.0/perfetto/trace_processor/shell.py`

 * *Files 13% similar despite different names*

```diff
@@ -43,19 +43,20 @@
     args.append('--no-ftrace-raw')
 
   if enable_dev_features:
     args.append('--dev')
 
   p = subprocess.Popen(
       tp_exec + args,
+      stdin=subprocess.DEVNULL,
       stdout=subprocess.DEVNULL,
       stderr=None if verbose else subprocess.DEVNULL)
 
   success = False
-  for i in range(3):
+  for _ in range(3):
     try:
       if p.poll() is None:
         _ = request.urlretrieve(f'http://{url}/status')
         success = True
       break
     except error.URLError:
       time.sleep(1)
```

### Comparing `perfetto-0.6.0/perfetto/trace_processor/trace_processor.descriptor` & `perfetto-0.7.0/perfetto/trace_processor/trace_processor.descriptor`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 0aa6 110a 2770 726f 746f 732f 7065 7266  ....'protos/perf
+00000000: 0a81 120a 2770 726f 746f 732f 7065 7266  ....'protos/perf
 00000010: 6574 746f 2f63 6f6d 6d6f 6e2f 6465 7363  etto/common/desc
 00000020: 7269 7074 6f72 2e70 726f 746f 120f 7065  riptor.proto..pe
 00000030: 7266 6574 746f 2e70 726f 746f 7322 4d0a  rfetto.protos"M.
 00000040: 1146 696c 6544 6573 6372 6970 746f 7253  .FileDescriptorS
 00000050: 6574 1238 0a04 6669 6c65 1801 2003 280b  et.8..file.. .(.
 00000060: 3224 2e70 6572 6665 7474 6f2e 7072 6f74  2$.perfetto.prot
 00000070: 6f73 2e46 696c 6544 6573 6372 6970 746f  os.FileDescripto
@@ -64,296 +64,332 @@
 000003f0: 6572 7665 6452 616e 6765 1223 0a0d 7265  ervedRange.#..re
 00000400: 7365 7276 6564 5f6e 616d 6518 0a20 0328  served_name.. .(
 00000410: 0952 0c72 6573 6572 7665 644e 616d 651a  .R.reservedName.
 00000420: 370a 0d52 6573 6572 7665 6452 616e 6765  7..ReservedRange
 00000430: 1214 0a05 7374 6172 7418 0120 0128 0552  ....start.. .(.R
 00000440: 0573 7461 7274 1210 0a03 656e 6418 0220  .start....end.. 
 00000450: 0128 0552 0365 6e64 4a04 0805 1006 4a04  .(.R.endJ.....J.
-00000460: 0807 1008 22ce 050a 1446 6965 6c64 4465  ...."....FieldDe
-00000470: 7363 7269 7074 6f72 5072 6f74 6f12 120a  scriptorProto...
-00000480: 046e 616d 6518 0120 0128 0952 046e 616d  .name.. .(.R.nam
-00000490: 6512 160a 066e 756d 6265 7218 0320 0128  e....number.. .(
-000004a0: 0552 066e 756d 6265 7212 410a 056c 6162  .R.number.A..lab
-000004b0: 656c 1804 2001 280e 322b 2e70 6572 6665  el.. .(.2+.perfe
-000004c0: 7474 6f2e 7072 6f74 6f73 2e46 6965 6c64  tto.protos.Field
-000004d0: 4465 7363 7269 7074 6f72 5072 6f74 6f2e  DescriptorProto.
-000004e0: 4c61 6265 6c52 056c 6162 656c 123e 0a04  LabelR.label.>..
-000004f0: 7479 7065 1805 2001 280e 322a 2e70 6572  type.. .(.2*.per
-00000500: 6665 7474 6f2e 7072 6f74 6f73 2e46 6965  fetto.protos.Fie
-00000510: 6c64 4465 7363 7269 7074 6f72 5072 6f74  ldDescriptorProt
-00000520: 6f2e 5479 7065 5204 7479 7065 121b 0a09  o.TypeR.type....
-00000530: 7479 7065 5f6e 616d 6518 0620 0128 0952  type_name.. .(.R
-00000540: 0874 7970 654e 616d 6512 1a0a 0865 7874  .typeName....ext
-00000550: 656e 6465 6518 0220 0128 0952 0865 7874  endee.. .(.R.ext
-00000560: 656e 6465 6512 230a 0d64 6566 6175 6c74  endee.#..default
-00000570: 5f76 616c 7565 1807 2001 2809 520c 6465  _value.. .(.R.de
-00000580: 6661 756c 7456 616c 7565 121f 0a0b 6f6e  faultValue....on
-00000590: 656f 665f 696e 6465 7818 0920 0128 0552  eof_index.. .(.R
-000005a0: 0a6f 6e65 6f66 496e 6465 7822 b602 0a04  .oneofIndex"....
-000005b0: 5479 7065 120f 0a0b 5459 5045 5f44 4f55  Type....TYPE_DOU
-000005c0: 424c 4510 0112 0e0a 0a54 5950 455f 464c  BLE......TYPE_FL
-000005d0: 4f41 5410 0212 0e0a 0a54 5950 455f 494e  OAT......TYPE_IN
-000005e0: 5436 3410 0312 0f0a 0b54 5950 455f 5549  T64......TYPE_UI
-000005f0: 4e54 3634 1004 120e 0a0a 5459 5045 5f49  NT64......TYPE_I
-00000600: 4e54 3332 1005 1210 0a0c 5459 5045 5f46  NT32......TYPE_F
-00000610: 4958 4544 3634 1006 1210 0a0c 5459 5045  IXED64......TYPE
-00000620: 5f46 4958 4544 3332 1007 120d 0a09 5459  _FIXED32......TY
-00000630: 5045 5f42 4f4f 4c10 0812 0f0a 0b54 5950  PE_BOOL......TYP
-00000640: 455f 5354 5249 4e47 1009 120e 0a0a 5459  E_STRING......TY
-00000650: 5045 5f47 524f 5550 100a 1210 0a0c 5459  PE_GROUP......TY
-00000660: 5045 5f4d 4553 5341 4745 100b 120e 0a0a  PE_MESSAGE......
-00000670: 5459 5045 5f42 5954 4553 100c 120f 0a0b  TYPE_BYTES......
-00000680: 5459 5045 5f55 494e 5433 3210 0d12 0d0a  TYPE_UINT32.....
-00000690: 0954 5950 455f 454e 554d 100e 1211 0a0d  .TYPE_ENUM......
-000006a0: 5459 5045 5f53 4649 5845 4433 3210 0f12  TYPE_SFIXED32...
-000006b0: 110a 0d54 5950 455f 5346 4958 4544 3634  ...TYPE_SFIXED64
-000006c0: 1010 120f 0a0b 5459 5045 5f53 494e 5433  ......TYPE_SINT3
-000006d0: 3210 1112 0f0a 0b54 5950 455f 5349 4e54  2......TYPE_SINT
-000006e0: 3634 1012 2243 0a05 4c61 6265 6c12 120a  64.."C..Label...
-000006f0: 0e4c 4142 454c 5f4f 5054 494f 4e41 4c10  .LABEL_OPTIONAL.
-00000700: 0112 120a 0e4c 4142 454c 5f52 4551 5549  .....LABEL_REQUI
-00000710: 5245 4410 0212 120a 0e4c 4142 454c 5f52  RED......LABEL_R
-00000720: 4550 4541 5445 4410 034a 0408 0a10 0b4a  EPEATED..J.....J
-00000730: 0408 0810 0922 630a 144f 6e65 6f66 4465  ....."c..OneofDe
-00000740: 7363 7269 7074 6f72 5072 6f74 6f12 120a  scriptorProto...
-00000750: 046e 616d 6518 0120 0128 0952 046e 616d  .name.. .(.R.nam
-00000760: 6512 370a 076f 7074 696f 6e73 1802 2001  e.7..options.. .
-00000770: 280b 321d 2e70 6572 6665 7474 6f2e 7072  (.2..perfetto.pr
-00000780: 6f74 6f73 2e4f 6e65 6f66 4f70 7469 6f6e  otos.OneofOption
-00000790: 7352 076f 7074 696f 6e73 229b 010a 1345  sR.options"....E
-000007a0: 6e75 6d44 6573 6372 6970 746f 7250 726f  numDescriptorPro
-000007b0: 746f 1212 0a04 6e61 6d65 1801 2001 2809  to....name.. .(.
-000007c0: 5204 6e61 6d65 123f 0a05 7661 6c75 6518  R.name.?..value.
-000007d0: 0220 0328 0b32 292e 7065 7266 6574 746f  . .(.2).perfetto
-000007e0: 2e70 726f 746f 732e 456e 756d 5661 6c75  .protos.EnumValu
-000007f0: 6544 6573 6372 6970 746f 7250 726f 746f  eDescriptorProto
-00000800: 5205 7661 6c75 6512 230a 0d72 6573 6572  R.value.#..reser
-00000810: 7665 645f 6e61 6d65 1805 2003 2809 520c  ved_name.. .(.R.
-00000820: 7265 7365 7276 6564 4e61 6d65 4a04 0803  reservedNameJ...
-00000830: 1004 4a04 0804 1005 224c 0a18 456e 756d  ..J....."L..Enum
-00000840: 5661 6c75 6544 6573 6372 6970 746f 7250  ValueDescriptorP
-00000850: 726f 746f 1212 0a04 6e61 6d65 1801 2001  roto....name.. .
-00000860: 2809 5204 6e61 6d65 1216 0a06 6e75 6d62  (.R.name....numb
-00000870: 6572 1802 2001 2805 5206 6e75 6d62 6572  er.. .(.R.number
-00000880: 4a04 0803 1004 2221 0a0c 4f6e 656f 664f  J....."!..OneofO
-00000890: 7074 696f 6e73 2a09 08e8 0710 8080 8080  ptions*.........
-000008a0: 024a 0608 e707 10e8 070a 9e01 0a3a 7072  .J...........:pr
-000008b0: 6f74 6f73 2f70 6572 6665 7474 6f2f 7472  otos/perfetto/tr
-000008c0: 6163 655f 7072 6f63 6573 736f 722f 6d65  ace_processor/me
-000008d0: 7461 7472 6163 655f 6361 7465 676f 7269  tatrace_categori
-000008e0: 6573 2e70 726f 746f 120f 7065 7266 6574  es.proto..perfet
-000008f0: 746f 2e70 726f 746f 732a 4f0a 134d 6574  to.protos*O..Met
-00000900: 6174 7261 6365 4361 7465 676f 7269 6573  atraceCategories
-00000910: 120c 0a08 544f 504c 4556 454c 1001 1209  ....TOPLEVEL....
-00000920: 0a05 5155 4552 5910 0212 0c0a 0846 554e  ..QUERY......FUN
-00000930: 4354 494f 4e10 0412 080a 044e 4f4e 4510  CTION......NONE.
-00000940: 0012 070a 0341 4c4c 1007 0a94 1a0a 3570  .....ALL......5p
-00000950: 726f 746f 732f 7065 7266 6574 746f 2f74  rotos/perfetto/t
-00000960: 7261 6365 5f70 726f 6365 7373 6f72 2f74  race_processor/t
-00000970: 7261 6365 5f70 726f 6365 7373 6f72 2e70  race_processor.p
-00000980: 726f 746f 120f 7065 7266 6574 746f 2e70  roto..perfetto.p
-00000990: 726f 746f 731a 2770 726f 746f 732f 7065  rotos.'protos/pe
-000009a0: 7266 6574 746f 2f63 6f6d 6d6f 6e2f 6465  rfetto/common/de
-000009b0: 7363 7269 7074 6f72 2e70 726f 746f 1a3a  scriptor.proto.:
-000009c0: 7072 6f74 6f73 2f70 6572 6665 7474 6f2f  protos/perfetto/
-000009d0: 7472 6163 655f 7072 6f63 6573 736f 722f  trace_processor/
-000009e0: 6d65 7461 7472 6163 655f 6361 7465 676f  metatrace_catego
-000009f0: 7269 6573 2e70 726f 746f 224f 0a17 5472  ries.proto"O..Tr
-00000a00: 6163 6550 726f 6365 7373 6f72 5270 6353  aceProcessorRpcS
-00000a10: 7472 6561 6d12 340a 036d 7367 1801 2003  tream.4..msg.. .
-00000a20: 280b 3222 2e70 6572 6665 7474 6f2e 7072  (.2".perfetto.pr
-00000a30: 6f74 6f73 2e54 7261 6365 5072 6f63 6573  otos.TraceProces
-00000a40: 736f 7252 7063 5203 6d73 6722 990b 0a11  sorRpcR.msg"....
-00000a50: 5472 6163 6550 726f 6365 7373 6f72 5270  TraceProcessorRp
-00000a60: 6312 100a 0373 6571 1801 2001 2803 5203  c....seq.. .(.R.
-00000a70: 7365 7112 1f0a 0b66 6174 616c 5f65 7272  seq....fatal_err
-00000a80: 6f72 1805 2001 2809 520a 6661 7461 6c45  or.. .(.R.fatalE
-00000a90: 7272 6f72 1253 0a07 7265 7175 6573 7418  rror.S..request.
-00000aa0: 0220 0128 0e32 372e 7065 7266 6574 746f  . .(.27.perfetto
-00000ab0: 2e70 726f 746f 732e 5472 6163 6550 726f  .protos.TracePro
-00000ac0: 6365 7373 6f72 5270 632e 5472 6163 6550  cessorRpc.TraceP
-00000ad0: 726f 6365 7373 6f72 4d65 7468 6f64 4800  rocessorMethodH.
-00000ae0: 5207 7265 7175 6573 7412 550a 0872 6573  R.request.U..res
-00000af0: 706f 6e73 6518 0320 0128 0e32 372e 7065  ponse.. .(.27.pe
-00000b00: 7266 6574 746f 2e70 726f 746f 732e 5472  rfetto.protos.Tr
-00000b10: 6163 6550 726f 6365 7373 6f72 5270 632e  aceProcessorRpc.
-00000b20: 5472 6163 6550 726f 6365 7373 6f72 4d65  TraceProcessorMe
-00000b30: 7468 6f64 4800 5208 7265 7370 6f6e 7365  thodH.R.response
-00000b40: 1262 0a0f 696e 7661 6c69 645f 7265 7175  .b..invalid_requ
-00000b50: 6573 7418 0420 0128 0e32 372e 7065 7266  est.. .(.27.perf
-00000b60: 6574 746f 2e70 726f 746f 732e 5472 6163  etto.protos.Trac
-00000b70: 6550 726f 6365 7373 6f72 5270 632e 5472  eProcessorRpc.Tr
-00000b80: 6163 6550 726f 6365 7373 6f72 4d65 7468  aceProcessorMeth
-00000b90: 6f64 4800 520e 696e 7661 6c69 6452 6571  odH.R.invalidReq
-00000ba0: 7565 7374 122c 0a11 6170 7065 6e64 5f74  uest.,..append_t
-00000bb0: 7261 6365 5f64 6174 6118 6520 0128 0c48  race_data.e .(.H
-00000bc0: 0152 0f61 7070 656e 6454 7261 6365 4461  .R.appendTraceDa
-00000bd0: 7461 123b 0a0a 7175 6572 795f 6172 6773  ta.;..query_args
-00000be0: 1867 2001 280b 321a 2e70 6572 6665 7474  .g .(.2..perfett
-00000bf0: 6f2e 7072 6f74 6f73 2e51 7565 7279 4172  o.protos.QueryAr
-00000c00: 6773 4801 5209 7175 6572 7941 7267 7312  gsH.R.queryArgs.
-00000c10: 540a 1363 6f6d 7075 7465 5f6d 6574 7269  T..compute_metri
-00000c20: 635f 6172 6773 1869 2001 280b 3222 2e70  c_args.i .(.2".p
-00000c30: 6572 6665 7474 6f2e 7072 6f74 6f73 2e43  erfetto.protos.C
-00000c40: 6f6d 7075 7465 4d65 7472 6963 4172 6773  omputeMetricArgs
-00000c50: 4801 5211 636f 6d70 7574 654d 6574 7269  H.R.computeMetri
-00000c60: 6341 7267 7312 5a0a 1565 6e61 626c 655f  cArgs.Z..enable_
-00000c70: 6d65 7461 7472 6163 655f 6172 6773 186a  metatrace_args.j
-00000c80: 2001 280b 3224 2e70 6572 6665 7474 6f2e   .(.2$.perfetto.
-00000c90: 7072 6f74 6f73 2e45 6e61 626c 654d 6574  protos.EnableMet
-00000ca0: 6174 7261 6365 4172 6773 4801 5213 656e  atraceArgsH.R.en
-00000cb0: 6162 6c65 4d65 7461 7472 6163 6541 7267  ableMetatraceArg
-00000cc0: 7312 4e0a 0d61 7070 656e 645f 7265 7375  s.N..append_resu
-00000cd0: 6c74 18c9 0120 0128 0b32 262e 7065 7266  lt... .(.2&.perf
-00000ce0: 6574 746f 2e70 726f 746f 732e 4170 7065  etto.protos.Appe
-00000cf0: 6e64 5472 6163 6544 6174 6152 6573 756c  ndTraceDataResul
-00000d00: 7448 0152 0c61 7070 656e 6452 6573 756c  tH.R.appendResul
-00000d10: 7412 420a 0c71 7565 7279 5f72 6573 756c  t.B..query_resul
-00000d20: 7418 cb01 2001 280b 321c 2e70 6572 6665  t... .(.2..perfe
-00000d30: 7474 6f2e 7072 6f74 6f73 2e51 7565 7279  tto.protos.Query
-00000d40: 5265 7375 6c74 4801 520b 7175 6572 7952  ResultH.R.queryR
-00000d50: 6573 756c 7412 4c0a 0d6d 6574 7269 635f  esult.L..metric_
-00000d60: 7265 7375 6c74 18cd 0120 0128 0b32 242e  result... .(.2$.
-00000d70: 7065 7266 6574 746f 2e70 726f 746f 732e  perfetto.protos.
-00000d80: 436f 6d70 7574 654d 6574 7269 6352 6573  ComputeMetricRes
-00000d90: 756c 7448 0152 0c6d 6574 7269 6352 6573  ultH.R.metricRes
-00000da0: 756c 7412 500a 126d 6574 7269 635f 6465  ult.P..metric_de
-00000db0: 7363 7269 7074 6f72 7318 ce01 2001 280b  scriptors... .(.
-00000dc0: 321e 2e70 6572 6665 7474 6f2e 7072 6f74  2..perfetto.prot
-00000dd0: 6f73 2e44 6573 6372 6970 746f 7253 6574  os.DescriptorSet
-00000de0: 4801 5211 6d65 7472 6963 4465 7363 7269  H.R.metricDescri
-00000df0: 7074 6f72 7312 4f0a 096d 6574 6174 7261  ptors.O..metatra
-00000e00: 6365 18d1 0120 0128 0b32 2e2e 7065 7266  ce... .(.2..perf
-00000e10: 6574 746f 2e70 726f 746f 732e 4469 7361  etto.protos.Disa
-00000e20: 626c 6541 6e64 5265 6164 4d65 7461 7472  bleAndReadMetatr
-00000e30: 6163 6552 6573 756c 7448 0152 096d 6574  aceResultH.R.met
-00000e40: 6174 7261 6365 1238 0a06 7374 6174 7573  atrace.8..status
-00000e50: 18d2 0120 0128 0b32 1d2e 7065 7266 6574  ... .(.2..perfet
-00000e60: 746f 2e70 726f 746f 732e 5374 6174 7573  to.protos.Status
-00000e70: 5265 7375 6c74 4801 5206 7374 6174 7573  ResultH.R.status
-00000e80: 22c6 020a 1454 7261 6365 5072 6f63 6573  "....TraceProces
-00000e90: 736f 724d 6574 686f 6412 130a 0f54 504d  sorMethod....TPM
-00000ea0: 5f55 4e53 5045 4349 4649 4544 1000 1219  _UNSPECIFIED....
-00000eb0: 0a15 5450 4d5f 4150 5045 4e44 5f54 5241  ..TPM_APPEND_TRA
-00000ec0: 4345 5f44 4154 4110 0112 1b0a 1754 504d  CE_DATA......TPM
-00000ed0: 5f46 494e 414c 495a 455f 5452 4143 455f  _FINALIZE_TRACE_
-00000ee0: 4441 5441 1002 1217 0a13 5450 4d5f 5155  DATA......TPM_QU
-00000ef0: 4552 595f 5354 5245 414d 494e 4710 0312  ERY_STREAMING...
-00000f00: 160a 1254 504d 5f43 4f4d 5055 5445 5f4d  ...TPM_COMPUTE_M
-00000f10: 4554 5249 4310 0512 1e0a 1a54 504d 5f47  ETRIC......TPM_G
-00000f20: 4554 5f4d 4554 5249 435f 4445 5343 5249  ET_METRIC_DESCRI
-00000f30: 5054 4f52 5310 0612 1e0a 1a54 504d 5f52  PTORS......TPM_R
-00000f40: 4553 544f 5245 5f49 4e49 5449 414c 5f54  ESTORE_INITIAL_T
-00000f50: 4142 4c45 5310 0712 180a 1454 504d 5f45  ABLES......TPM_E
-00000f60: 4e41 424c 455f 4d45 5441 5452 4143 4510  NABLE_METATRACE.
-00000f70: 0812 220a 1e54 504d 5f44 4953 4142 4c45  .."..TPM_DISABLE
-00000f80: 5f41 4e44 5f52 4541 445f 4d45 5441 5452  _AND_READ_METATR
-00000f90: 4143 4510 0912 120a 0e54 504d 5f47 4554  ACE......TPM_GET
-00000fa0: 5f53 5441 5455 5310 0a22 0408 0410 042a  _STATUS..".....*
-00000fb0: 1854 504d 5f51 5545 5259 5f52 4157 5f44  .TPM_QUERY_RAW_D
-00000fc0: 4550 5245 4341 5445 4442 060a 0474 7970  EPRECATEDB...typ
-00000fd0: 6542 060a 0461 7267 734a 0408 6810 694a  eB...argsJ..h.iJ
-00000fe0: 0608 cc01 10cd 0122 5b0a 1541 7070 656e  ......."[..Appen
-00000ff0: 6454 7261 6365 4461 7461 5265 7375 6c74  dTraceDataResult
-00001000: 122c 0a12 746f 7461 6c5f 6279 7465 735f  .,..total_bytes_
-00001010: 7061 7273 6564 1801 2001 2803 5210 746f  parsed.. .(.R.to
-00001020: 7461 6c42 7974 6573 5061 7273 6564 1214  talBytesParsed..
-00001030: 0a05 6572 726f 7218 0220 0128 0952 0565  ..error.. .(.R.e
-00001040: 7272 6f72 2240 0a09 5175 6572 7941 7267  rror"@..QueryArg
-00001050: 7312 1b0a 0973 716c 5f71 7565 7279 1801  s....sql_query..
-00001060: 2001 2809 5208 7371 6c51 7565 7279 1210   .(.R.sqlQuery..
-00001070: 0a03 7461 6718 0320 0128 0952 0374 6167  ..tag.. .(.R.tag
-00001080: 4a04 0802 1003 22f4 040a 0b51 7565 7279  J....."....Query
-00001090: 5265 7375 6c74 1221 0a0c 636f 6c75 6d6e  Result.!..column
-000010a0: 5f6e 616d 6573 1801 2003 2809 520b 636f  _names.. .(.R.co
-000010b0: 6c75 6d6e 4e61 6d65 7312 140a 0565 7272  lumnNames....err
-000010c0: 6f72 1802 2001 2809 5205 6572 726f 7212  or.. .(.R.error.
-000010d0: 3d0a 0562 6174 6368 1803 2003 280b 3227  =..batch.. .(.2'
-000010e0: 2e70 6572 6665 7474 6f2e 7072 6f74 6f73  .perfetto.protos
-000010f0: 2e51 7565 7279 5265 7375 6c74 2e43 656c  .QueryResult.Cel
-00001100: 6c73 4261 7463 6852 0562 6174 6368 1227  lsBatchR.batch.'
-00001110: 0a0f 7374 6174 656d 656e 745f 636f 756e  ..statement_coun
-00001120: 7418 0420 0128 0d52 0e73 7461 7465 6d65  t.. .(.R.stateme
-00001130: 6e74 436f 756e 7412 3d0a 1b73 7461 7465  ntCount.=..state
-00001140: 6d65 6e74 5f77 6974 685f 6f75 7470 7574  ment_with_output
-00001150: 5f63 6f75 6e74 1805 2001 280d 5218 7374  _count.. .(.R.st
-00001160: 6174 656d 656e 7457 6974 684f 7574 7075  atementWithOutpu
-00001170: 7443 6f75 6e74 1a84 030a 0a43 656c 6c73  tCount.....Cells
-00001180: 4261 7463 6812 4a0a 0563 656c 6c73 1801  Batch.J..cells..
-00001190: 2003 280e 3230 2e70 6572 6665 7474 6f2e   .(.20.perfetto.
-000011a0: 7072 6f74 6f73 2e51 7565 7279 5265 7375  protos.QueryResu
-000011b0: 6c74 2e43 656c 6c73 4261 7463 682e 4365  lt.CellsBatch.Ce
-000011c0: 6c6c 5479 7065 4202 1001 5205 6365 6c6c  llTypeB...R.cell
-000011d0: 7312 250a 0c76 6172 696e 745f 6365 6c6c  s.%..varint_cell
-000011e0: 7318 0220 0328 0342 0210 0152 0b76 6172  s.. .(.B...R.var
-000011f0: 696e 7443 656c 6c73 1227 0a0d 666c 6f61  intCells.'..floa
-00001200: 7436 345f 6365 6c6c 7318 0320 0328 0142  t64_cells.. .(.B
-00001210: 0210 0152 0c66 6c6f 6174 3634 4365 6c6c  ...R.float64Cell
-00001220: 7312 1d0a 0a62 6c6f 625f 6365 6c6c 7318  s....blob_cells.
-00001230: 0420 0328 0c52 0962 6c6f 6243 656c 6c73  . .(.R.blobCells
-00001240: 1221 0a0c 7374 7269 6e67 5f63 656c 6c73  .!..string_cells
-00001250: 1805 2001 2809 520b 7374 7269 6e67 4365  .. .(.R.stringCe
-00001260: 6c6c 7312 220a 0d69 735f 6c61 7374 5f62  lls."..is_last_b
-00001270: 6174 6368 1806 2001 2808 520b 6973 4c61  atch.. .(.R.isLa
-00001280: 7374 4261 7463 6822 6e0a 0843 656c 6c54  stBatch"n..CellT
-00001290: 7970 6512 100a 0c43 454c 4c5f 494e 5641  ype....CELL_INVA
-000012a0: 4c49 4410 0012 0d0a 0943 454c 4c5f 4e55  LID......CELL_NU
-000012b0: 4c4c 1001 120f 0a0b 4345 4c4c 5f56 4152  LL......CELL_VAR
-000012c0: 494e 5410 0212 100a 0c43 454c 4c5f 464c  INT......CELL_FL
-000012d0: 4f41 5436 3410 0312 0f0a 0b43 454c 4c5f  OAT64......CELL_
-000012e0: 5354 5249 4e47 1004 120d 0a09 4345 4c4c  STRING......CELL
-000012f0: 5f42 4c4f 4210 054a 0408 0710 0822 0c0a  _BLOB..J....."..
-00001300: 0a53 7461 7475 7341 7267 7322 9101 0a0c  .StatusArgs"....
-00001310: 5374 6174 7573 5265 7375 6c74 122a 0a11  StatusResult.*..
-00001320: 6c6f 6164 6564 5f74 7261 6365 5f6e 616d  loaded_trace_nam
-00001330: 6518 0120 0128 0952 0f6c 6f61 6465 6454  e.. .(.R.loadedT
-00001340: 7261 6365 4e61 6d65 1234 0a16 6875 6d61  raceName.4..huma
-00001350: 6e5f 7265 6164 6162 6c65 5f76 6572 7369  n_readable_versi
-00001360: 6f6e 1802 2001 2809 5214 6875 6d61 6e52  on.. .(.R.humanR
-00001370: 6561 6461 626c 6556 6572 7369 6f6e 121f  eadableVersion..
-00001380: 0a0b 6170 695f 7665 7273 696f 6e18 0320  ..api_version.. 
-00001390: 0128 0552 0a61 7069 5665 7273 696f 6e22  .(.R.apiVersion"
-000013a0: b301 0a11 436f 6d70 7574 654d 6574 7269  ....ComputeMetri
-000013b0: 6341 7267 7312 210a 0c6d 6574 7269 635f  cArgs.!..metric_
-000013c0: 6e61 6d65 7318 0120 0328 0952 0b6d 6574  names.. .(.R.met
-000013d0: 7269 634e 616d 6573 1247 0a06 666f 726d  ricNames.G..form
-000013e0: 6174 1802 2001 280e 322f 2e70 6572 6665  at.. .(.2/.perfe
-000013f0: 7474 6f2e 7072 6f74 6f73 2e43 6f6d 7075  tto.protos.Compu
-00001400: 7465 4d65 7472 6963 4172 6773 2e52 6573  teMetricArgs.Res
-00001410: 756c 7446 6f72 6d61 7452 0666 6f72 6d61  ultFormatR.forma
-00001420: 7422 320a 0c52 6573 756c 7446 6f72 6d61  t"2..ResultForma
-00001430: 7412 130a 0f42 494e 4152 595f 5052 4f54  t....BINARY_PROT
-00001440: 4f42 5546 1000 120d 0a09 5445 5854 5052  OBUF......TEXTPR
-00001450: 4f54 4f10 0122 8501 0a13 436f 6d70 7574  OTO.."....Comput
-00001460: 654d 6574 7269 6352 6573 756c 7412 1a0a  eMetricResult...
-00001470: 076d 6574 7269 6373 1801 2001 280c 4800  .metrics.. .(.H.
-00001480: 5207 6d65 7472 6963 7312 320a 146d 6574  R.metrics.2..met
-00001490: 7269 6373 5f61 735f 7072 6f74 6f74 6578  rics_as_prototex
-000014a0: 7418 0320 0128 0948 0052 126d 6574 7269  t.. .(.H.R.metri
-000014b0: 6373 4173 5072 6f74 6f74 6578 7412 140a  csAsPrototext...
-000014c0: 0565 7272 6f72 1802 2001 2809 5205 6572  .error.. .(.R.er
-000014d0: 726f 7242 080a 0672 6573 756c 7422 5b0a  rorB...result"[.
-000014e0: 1345 6e61 626c 654d 6574 6174 7261 6365  .EnableMetatrace
-000014f0: 4172 6773 1244 0a0a 6361 7465 676f 7269  Args.D..categori
-00001500: 6573 1801 2001 280e 3224 2e70 6572 6665  es.. .(.2$.perfe
-00001510: 7474 6f2e 7072 6f74 6f73 2e4d 6574 6174  tto.protos.Metat
-00001520: 7261 6365 4361 7465 676f 7269 6573 520a  raceCategoriesR.
-00001530: 6361 7465 676f 7269 6573 2217 0a15 456e  categories"...En
-00001540: 6162 6c65 4d65 7461 7472 6163 6552 6573  ableMetatraceRes
-00001550: 756c 7422 1d0a 1b44 6973 6162 6c65 416e  ult"...DisableAn
-00001560: 6452 6561 644d 6574 6174 7261 6365 4172  dReadMetatraceAr
-00001570: 6773 2253 0a1d 4469 7361 626c 6541 6e64  gs"S..DisableAnd
-00001580: 5265 6164 4d65 7461 7472 6163 6552 6573  ReadMetatraceRes
-00001590: 756c 7412 1c0a 096d 6574 6174 7261 6365  ult....metatrace
-000015a0: 1801 2001 280c 5209 6d65 7461 7472 6163  .. .(.R.metatrac
-000015b0: 6512 140a 0565 7272 6f72 1802 2001 2809  e....error.. .(.
-000015c0: 5205 6572 726f 7222 530a 0d44 6573 6372  R.error"S..Descr
-000015d0: 6970 746f 7253 6574 1242 0a0b 6465 7363  iptorSet.B..desc
-000015e0: 7269 7074 6f72 7318 0120 0328 0b32 202e  riptors.. .(.2 .
-000015f0: 7065 7266 6574 746f 2e70 726f 746f 732e  perfetto.protos.
-00001600: 4465 7363 7269 7074 6f72 5072 6f74 6f52  DescriptorProtoR
-00001610: 0b64 6573 6372 6970 746f 7273 2a43 0a18  .descriptors*C..
-00001620: 5472 6163 6550 726f 6365 7373 6f72 4170  TraceProcessorAp
-00001630: 6956 6572 7369 6f6e 1227 0a23 5452 4143  iVersion.'.#TRAC
-00001640: 455f 5052 4f43 4553 534f 525f 4355 5252  E_PROCESSOR_CURR
-00001650: 454e 545f 4150 495f 5645 5253 494f 4e10  ENT_API_VERSION.
-00001660: 06                                       .
+00000460: 0807 1008 2226 0a0c 4669 656c 644f 7074  ...."&..FieldOpt
+00000470: 696f 6e73 1216 0a06 7061 636b 6564 1802  ions....packed..
+00000480: 2001 2808 5206 7061 636b 6564 2281 060a   .(.R.packed"...
+00000490: 1446 6965 6c64 4465 7363 7269 7074 6f72  .FieldDescriptor
+000004a0: 5072 6f74 6f12 120a 046e 616d 6518 0120  Proto....name.. 
+000004b0: 0128 0952 046e 616d 6512 160a 066e 756d  .(.R.name....num
+000004c0: 6265 7218 0320 0128 0552 066e 756d 6265  ber.. .(.R.numbe
+000004d0: 7212 410a 056c 6162 656c 1804 2001 280e  r.A..label.. .(.
+000004e0: 322b 2e70 6572 6665 7474 6f2e 7072 6f74  2+.perfetto.prot
+000004f0: 6f73 2e46 6965 6c64 4465 7363 7269 7074  os.FieldDescript
+00000500: 6f72 5072 6f74 6f2e 4c61 6265 6c52 056c  orProto.LabelR.l
+00000510: 6162 656c 123e 0a04 7479 7065 1805 2001  abel.>..type.. .
+00000520: 280e 322a 2e70 6572 6665 7474 6f2e 7072  (.2*.perfetto.pr
+00000530: 6f74 6f73 2e46 6965 6c64 4465 7363 7269  otos.FieldDescri
+00000540: 7074 6f72 5072 6f74 6f2e 5479 7065 5204  ptorProto.TypeR.
+00000550: 7479 7065 121b 0a09 7479 7065 5f6e 616d  type....type_nam
+00000560: 6518 0620 0128 0952 0874 7970 654e 616d  e.. .(.R.typeNam
+00000570: 6512 1a0a 0865 7874 656e 6465 6518 0220  e....extendee.. 
+00000580: 0128 0952 0865 7874 656e 6465 6512 230a  .(.R.extendee.#.
+00000590: 0d64 6566 6175 6c74 5f76 616c 7565 1807  .default_value..
+000005a0: 2001 2809 520c 6465 6661 756c 7456 616c   .(.R.defaultVal
+000005b0: 7565 1237 0a07 6f70 7469 6f6e 7318 0820  ue.7..options.. 
+000005c0: 0128 0b32 1d2e 7065 7266 6574 746f 2e70  .(.2..perfetto.p
+000005d0: 726f 746f 732e 4669 656c 644f 7074 696f  rotos.FieldOptio
+000005e0: 6e73 5207 6f70 7469 6f6e 7312 1f0a 0b6f  nsR.options....o
+000005f0: 6e65 6f66 5f69 6e64 6578 1809 2001 2805  neof_index.. .(.
+00000600: 520a 6f6e 656f 6649 6e64 6578 22b6 020a  R.oneofIndex"...
+00000610: 0454 7970 6512 0f0a 0b54 5950 455f 444f  .Type....TYPE_DO
+00000620: 5542 4c45 1001 120e 0a0a 5459 5045 5f46  UBLE......TYPE_F
+00000630: 4c4f 4154 1002 120e 0a0a 5459 5045 5f49  LOAT......TYPE_I
+00000640: 4e54 3634 1003 120f 0a0b 5459 5045 5f55  NT64......TYPE_U
+00000650: 494e 5436 3410 0412 0e0a 0a54 5950 455f  INT64......TYPE_
+00000660: 494e 5433 3210 0512 100a 0c54 5950 455f  INT32......TYPE_
+00000670: 4649 5845 4436 3410 0612 100a 0c54 5950  FIXED64......TYP
+00000680: 455f 4649 5845 4433 3210 0712 0d0a 0954  E_FIXED32......T
+00000690: 5950 455f 424f 4f4c 1008 120f 0a0b 5459  YPE_BOOL......TY
+000006a0: 5045 5f53 5452 494e 4710 0912 0e0a 0a54  PE_STRING......T
+000006b0: 5950 455f 4752 4f55 5010 0a12 100a 0c54  YPE_GROUP......T
+000006c0: 5950 455f 4d45 5353 4147 4510 0b12 0e0a  YPE_MESSAGE.....
+000006d0: 0a54 5950 455f 4259 5445 5310 0c12 0f0a  .TYPE_BYTES.....
+000006e0: 0b54 5950 455f 5549 4e54 3332 100d 120d  .TYPE_UINT32....
+000006f0: 0a09 5459 5045 5f45 4e55 4d10 0e12 110a  ..TYPE_ENUM.....
+00000700: 0d54 5950 455f 5346 4958 4544 3332 100f  .TYPE_SFIXED32..
+00000710: 1211 0a0d 5459 5045 5f53 4649 5845 4436  ....TYPE_SFIXED6
+00000720: 3410 1012 0f0a 0b54 5950 455f 5349 4e54  4......TYPE_SINT
+00000730: 3332 1011 120f 0a0b 5459 5045 5f53 494e  32......TYPE_SIN
+00000740: 5436 3410 1222 430a 054c 6162 656c 1212  T64.."C..Label..
+00000750: 0a0e 4c41 4245 4c5f 4f50 5449 4f4e 414c  ..LABEL_OPTIONAL
+00000760: 1001 1212 0a0e 4c41 4245 4c5f 5245 5155  ......LABEL_REQU
+00000770: 4952 4544 1002 1212 0a0e 4c41 4245 4c5f  IRED......LABEL_
+00000780: 5245 5045 4154 4544 1003 4a04 080a 100b  REPEATED..J.....
+00000790: 2263 0a14 4f6e 656f 6644 6573 6372 6970  "c..OneofDescrip
+000007a0: 746f 7250 726f 746f 1212 0a04 6e61 6d65  torProto....name
+000007b0: 1801 2001 2809 5204 6e61 6d65 1237 0a07  .. .(.R.name.7..
+000007c0: 6f70 7469 6f6e 7318 0220 0128 0b32 1d2e  options.. .(.2..
+000007d0: 7065 7266 6574 746f 2e70 726f 746f 732e  perfetto.protos.
+000007e0: 4f6e 656f 664f 7074 696f 6e73 5207 6f70  OneofOptionsR.op
+000007f0: 7469 6f6e 7322 9b01 0a13 456e 756d 4465  tions"....EnumDe
+00000800: 7363 7269 7074 6f72 5072 6f74 6f12 120a  scriptorProto...
+00000810: 046e 616d 6518 0120 0128 0952 046e 616d  .name.. .(.R.nam
+00000820: 6512 3f0a 0576 616c 7565 1802 2003 280b  e.?..value.. .(.
+00000830: 3229 2e70 6572 6665 7474 6f2e 7072 6f74  2).perfetto.prot
+00000840: 6f73 2e45 6e75 6d56 616c 7565 4465 7363  os.EnumValueDesc
+00000850: 7269 7074 6f72 5072 6f74 6f52 0576 616c  riptorProtoR.val
+00000860: 7565 1223 0a0d 7265 7365 7276 6564 5f6e  ue.#..reserved_n
+00000870: 616d 6518 0520 0328 0952 0c72 6573 6572  ame.. .(.R.reser
+00000880: 7665 644e 616d 654a 0408 0310 044a 0408  vedNameJ.....J..
+00000890: 0410 0522 4c0a 1845 6e75 6d56 616c 7565  ..."L..EnumValue
+000008a0: 4465 7363 7269 7074 6f72 5072 6f74 6f12  DescriptorProto.
+000008b0: 120a 046e 616d 6518 0120 0128 0952 046e  ...name.. .(.R.n
+000008c0: 616d 6512 160a 066e 756d 6265 7218 0220  ame....number.. 
+000008d0: 0128 0552 066e 756d 6265 724a 0408 0310  .(.R.numberJ....
+000008e0: 0422 210a 0c4f 6e65 6f66 4f70 7469 6f6e  ."!..OneofOption
+000008f0: 732a 0908 e807 1080 8080 8002 4a06 08e7  s*..........J...
+00000900: 0710 e807 0a9e 010a 3a70 726f 746f 732f  ........:protos/
+00000910: 7065 7266 6574 746f 2f74 7261 6365 5f70  perfetto/trace_p
+00000920: 726f 6365 7373 6f72 2f6d 6574 6174 7261  rocessor/metatra
+00000930: 6365 5f63 6174 6567 6f72 6965 732e 7072  ce_categories.pr
+00000940: 6f74 6f12 0f70 6572 6665 7474 6f2e 7072  oto..perfetto.pr
+00000950: 6f74 6f73 2a4f 0a13 4d65 7461 7472 6163  otos*O..Metatrac
+00000960: 6543 6174 6567 6f72 6965 7312 0c0a 0854  eCategories....T
+00000970: 4f50 4c45 5645 4c10 0112 090a 0551 5545  OPLEVEL......QUE
+00000980: 5259 1002 120c 0a08 4655 4e43 5449 4f4e  RY......FUNCTION
+00000990: 1004 1208 0a04 4e4f 4e45 1000 1207 0a03  ......NONE......
+000009a0: 414c 4c10 070a 831e 0a35 7072 6f74 6f73  ALL......5protos
+000009b0: 2f70 6572 6665 7474 6f2f 7472 6163 655f  /perfetto/trace_
+000009c0: 7072 6f63 6573 736f 722f 7472 6163 655f  processor/trace_
+000009d0: 7072 6f63 6573 736f 722e 7072 6f74 6f12  processor.proto.
+000009e0: 0f70 6572 6665 7474 6f2e 7072 6f74 6f73  .perfetto.protos
+000009f0: 1a27 7072 6f74 6f73 2f70 6572 6665 7474  .'protos/perfett
+00000a00: 6f2f 636f 6d6d 6f6e 2f64 6573 6372 6970  o/common/descrip
+00000a10: 746f 722e 7072 6f74 6f1a 3a70 726f 746f  tor.proto.:proto
+00000a20: 732f 7065 7266 6574 746f 2f74 7261 6365  s/perfetto/trace
+00000a30: 5f70 726f 6365 7373 6f72 2f6d 6574 6174  _processor/metat
+00000a40: 7261 6365 5f63 6174 6567 6f72 6965 732e  race_categories.
+00000a50: 7072 6f74 6f22 4f0a 1754 7261 6365 5072  proto"O..TracePr
+00000a60: 6f63 6573 736f 7252 7063 5374 7265 616d  ocessorRpcStream
+00000a70: 1234 0a03 6d73 6718 0120 0328 0b32 222e  .4..msg.. .(.2".
+00000a80: 7065 7266 6574 746f 2e70 726f 746f 732e  perfetto.protos.
+00000a90: 5472 6163 6550 726f 6365 7373 6f72 5270  TraceProcessorRp
+00000aa0: 6352 036d 7367 22a1 0c0a 1154 7261 6365  cR.msg"....Trace
+00000ab0: 5072 6f63 6573 736f 7252 7063 1210 0a03  ProcessorRpc....
+00000ac0: 7365 7118 0120 0128 0352 0373 6571 121f  seq.. .(.R.seq..
+00000ad0: 0a0b 6661 7461 6c5f 6572 726f 7218 0520  ..fatal_error.. 
+00000ae0: 0128 0952 0a66 6174 616c 4572 726f 7212  .(.R.fatalError.
+00000af0: 530a 0772 6571 7565 7374 1802 2001 280e  S..request.. .(.
+00000b00: 3237 2e70 6572 6665 7474 6f2e 7072 6f74  27.perfetto.prot
+00000b10: 6f73 2e54 7261 6365 5072 6f63 6573 736f  os.TraceProcesso
+00000b20: 7252 7063 2e54 7261 6365 5072 6f63 6573  rRpc.TraceProces
+00000b30: 736f 724d 6574 686f 6448 0052 0772 6571  sorMethodH.R.req
+00000b40: 7565 7374 1255 0a08 7265 7370 6f6e 7365  uest.U..response
+00000b50: 1803 2001 280e 3237 2e70 6572 6665 7474  .. .(.27.perfett
+00000b60: 6f2e 7072 6f74 6f73 2e54 7261 6365 5072  o.protos.TracePr
+00000b70: 6f63 6573 736f 7252 7063 2e54 7261 6365  ocessorRpc.Trace
+00000b80: 5072 6f63 6573 736f 724d 6574 686f 6448  ProcessorMethodH
+00000b90: 0052 0872 6573 706f 6e73 6512 620a 0f69  .R.response.b..i
+00000ba0: 6e76 616c 6964 5f72 6571 7565 7374 1804  nvalid_request..
+00000bb0: 2001 280e 3237 2e70 6572 6665 7474 6f2e   .(.27.perfetto.
+00000bc0: 7072 6f74 6f73 2e54 7261 6365 5072 6f63  protos.TraceProc
+00000bd0: 6573 736f 7252 7063 2e54 7261 6365 5072  essorRpc.TracePr
+00000be0: 6f63 6573 736f 724d 6574 686f 6448 0052  ocessorMethodH.R
+00000bf0: 0e69 6e76 616c 6964 5265 7175 6573 7412  .invalidRequest.
+00000c00: 2c0a 1161 7070 656e 645f 7472 6163 655f  ,..append_trace_
+00000c10: 6461 7461 1865 2001 280c 4801 520f 6170  data.e .(.H.R.ap
+00000c20: 7065 6e64 5472 6163 6544 6174 6112 3b0a  pendTraceData.;.
+00000c30: 0a71 7565 7279 5f61 7267 7318 6720 0128  .query_args.g .(
+00000c40: 0b32 1a2e 7065 7266 6574 746f 2e70 726f  .2..perfetto.pro
+00000c50: 746f 732e 5175 6572 7941 7267 7348 0152  tos.QueryArgsH.R
+00000c60: 0971 7565 7279 4172 6773 1254 0a13 636f  .queryArgs.T..co
+00000c70: 6d70 7574 655f 6d65 7472 6963 5f61 7267  mpute_metric_arg
+00000c80: 7318 6920 0128 0b32 222e 7065 7266 6574  s.i .(.2".perfet
+00000c90: 746f 2e70 726f 746f 732e 436f 6d70 7574  to.protos.Comput
+00000ca0: 654d 6574 7269 6341 7267 7348 0152 1163  eMetricArgsH.R.c
+00000cb0: 6f6d 7075 7465 4d65 7472 6963 4172 6773  omputeMetricArgs
+00000cc0: 125a 0a15 656e 6162 6c65 5f6d 6574 6174  .Z..enable_metat
+00000cd0: 7261 6365 5f61 7267 7318 6a20 0128 0b32  race_args.j .(.2
+00000ce0: 242e 7065 7266 6574 746f 2e70 726f 746f  $.perfetto.proto
+00000cf0: 732e 456e 6162 6c65 4d65 7461 7472 6163  s.EnableMetatrac
+00000d00: 6541 7267 7348 0152 1365 6e61 626c 654d  eArgsH.R.enableM
+00000d10: 6574 6174 7261 6365 4172 6773 1267 0a1a  etatraceArgs.g..
+00000d20: 7265 7365 745f 7472 6163 655f 7072 6f63  reset_trace_proc
+00000d30: 6573 736f 725f 6172 6773 186b 2001 280b  essor_args.k .(.
+00000d40: 3228 2e70 6572 6665 7474 6f2e 7072 6f74  2(.perfetto.prot
+00000d50: 6f73 2e52 6573 6574 5472 6163 6550 726f  os.ResetTracePro
+00000d60: 6365 7373 6f72 4172 6773 4801 5217 7265  cessorArgsH.R.re
+00000d70: 7365 7454 7261 6365 5072 6f63 6573 736f  setTraceProcesso
+00000d80: 7241 7267 7312 4e0a 0d61 7070 656e 645f  rArgs.N..append_
+00000d90: 7265 7375 6c74 18c9 0120 0128 0b32 262e  result... .(.2&.
+00000da0: 7065 7266 6574 746f 2e70 726f 746f 732e  perfetto.protos.
+00000db0: 4170 7065 6e64 5472 6163 6544 6174 6152  AppendTraceDataR
+00000dc0: 6573 756c 7448 0152 0c61 7070 656e 6452  esultH.R.appendR
+00000dd0: 6573 756c 7412 420a 0c71 7565 7279 5f72  esult.B..query_r
+00000de0: 6573 756c 7418 cb01 2001 280b 321c 2e70  esult... .(.2..p
+00000df0: 6572 6665 7474 6f2e 7072 6f74 6f73 2e51  erfetto.protos.Q
+00000e00: 7565 7279 5265 7375 6c74 4801 520b 7175  ueryResultH.R.qu
+00000e10: 6572 7952 6573 756c 7412 4c0a 0d6d 6574  eryResult.L..met
+00000e20: 7269 635f 7265 7375 6c74 18cd 0120 0128  ric_result... .(
+00000e30: 0b32 242e 7065 7266 6574 746f 2e70 726f  .2$.perfetto.pro
+00000e40: 746f 732e 436f 6d70 7574 654d 6574 7269  tos.ComputeMetri
+00000e50: 6352 6573 756c 7448 0152 0c6d 6574 7269  cResultH.R.metri
+00000e60: 6352 6573 756c 7412 500a 126d 6574 7269  cResult.P..metri
+00000e70: 635f 6465 7363 7269 7074 6f72 7318 ce01  c_descriptors...
+00000e80: 2001 280b 321e 2e70 6572 6665 7474 6f2e   .(.2..perfetto.
+00000e90: 7072 6f74 6f73 2e44 6573 6372 6970 746f  protos.Descripto
+00000ea0: 7253 6574 4801 5211 6d65 7472 6963 4465  rSetH.R.metricDe
+00000eb0: 7363 7269 7074 6f72 7312 4f0a 096d 6574  scriptors.O..met
+00000ec0: 6174 7261 6365 18d1 0120 0128 0b32 2e2e  atrace... .(.2..
+00000ed0: 7065 7266 6574 746f 2e70 726f 746f 732e  perfetto.protos.
+00000ee0: 4469 7361 626c 6541 6e64 5265 6164 4d65  DisableAndReadMe
+00000ef0: 7461 7472 6163 6552 6573 756c 7448 0152  tatraceResultH.R
+00000f00: 096d 6574 6174 7261 6365 1238 0a06 7374  .metatrace.8..st
+00000f10: 6174 7573 18d2 0120 0128 0b32 1d2e 7065  atus... .(.2..pe
+00000f20: 7266 6574 746f 2e70 726f 746f 732e 5374  rfetto.protos.St
+00000f30: 6174 7573 5265 7375 6c74 4801 5206 7374  atusResultH.R.st
+00000f40: 6174 7573 22e5 020a 1454 7261 6365 5072  atus"....TracePr
+00000f50: 6f63 6573 736f 724d 6574 686f 6412 130a  ocessorMethod...
+00000f60: 0f54 504d 5f55 4e53 5045 4349 4649 4544  .TPM_UNSPECIFIED
+00000f70: 1000 1219 0a15 5450 4d5f 4150 5045 4e44  ......TPM_APPEND
+00000f80: 5f54 5241 4345 5f44 4154 4110 0112 1b0a  _TRACE_DATA.....
+00000f90: 1754 504d 5f46 494e 414c 495a 455f 5452  .TPM_FINALIZE_TR
+00000fa0: 4143 455f 4441 5441 1002 1217 0a13 5450  ACE_DATA......TP
+00000fb0: 4d5f 5155 4552 595f 5354 5245 414d 494e  M_QUERY_STREAMIN
+00000fc0: 4710 0312 160a 1254 504d 5f43 4f4d 5055  G......TPM_COMPU
+00000fd0: 5445 5f4d 4554 5249 4310 0512 1e0a 1a54  TE_METRIC......T
+00000fe0: 504d 5f47 4554 5f4d 4554 5249 435f 4445  PM_GET_METRIC_DE
+00000ff0: 5343 5249 5054 4f52 5310 0612 1e0a 1a54  SCRIPTORS......T
+00001000: 504d 5f52 4553 544f 5245 5f49 4e49 5449  PM_RESTORE_INITI
+00001010: 414c 5f54 4142 4c45 5310 0712 180a 1454  AL_TABLES......T
+00001020: 504d 5f45 4e41 424c 455f 4d45 5441 5452  PM_ENABLE_METATR
+00001030: 4143 4510 0812 220a 1e54 504d 5f44 4953  ACE..."..TPM_DIS
+00001040: 4142 4c45 5f41 4e44 5f52 4541 445f 4d45  ABLE_AND_READ_ME
+00001050: 5441 5452 4143 4510 0912 120a 0e54 504d  TATRACE......TPM
+00001060: 5f47 4554 5f53 5441 5455 5310 0a12 1d0a  _GET_STATUS.....
+00001070: 1954 504d 5f52 4553 4554 5f54 5241 4345  .TPM_RESET_TRACE
+00001080: 5f50 524f 4345 5353 4f52 100b 2204 0804  _PROCESSOR.."...
+00001090: 1004 2a18 5450 4d5f 5155 4552 595f 5241  ..*.TPM_QUERY_RA
+000010a0: 575f 4445 5052 4543 4154 4544 4206 0a04  W_DEPRECATEDB...
+000010b0: 7479 7065 4206 0a04 6172 6773 4a04 0868  typeB...argsJ..h
+000010c0: 1069 4a06 08cc 0110 cd01 225b 0a15 4170  .iJ......."[..Ap
+000010d0: 7065 6e64 5472 6163 6544 6174 6152 6573  pendTraceDataRes
+000010e0: 756c 7412 2c0a 1274 6f74 616c 5f62 7974  ult.,..total_byt
+000010f0: 6573 5f70 6172 7365 6418 0120 0128 0352  es_parsed.. .(.R
+00001100: 1074 6f74 616c 4279 7465 7350 6172 7365  .totalBytesParse
+00001110: 6412 140a 0565 7272 6f72 1802 2001 2809  d....error.. .(.
+00001120: 5205 6572 726f 7222 400a 0951 7565 7279  R.error"@..Query
+00001130: 4172 6773 121b 0a09 7371 6c5f 7175 6572  Args....sql_quer
+00001140: 7918 0120 0128 0952 0873 716c 5175 6572  y.. .(.R.sqlQuer
+00001150: 7912 100a 0374 6167 1803 2001 2809 5203  y....tag.. .(.R.
+00001160: 7461 674a 0408 0210 0322 f404 0a0b 5175  tagJ....."....Qu
+00001170: 6572 7952 6573 756c 7412 210a 0c63 6f6c  eryResult.!..col
+00001180: 756d 6e5f 6e61 6d65 7318 0120 0328 0952  umn_names.. .(.R
+00001190: 0b63 6f6c 756d 6e4e 616d 6573 1214 0a05  .columnNames....
+000011a0: 6572 726f 7218 0220 0128 0952 0565 7272  error.. .(.R.err
+000011b0: 6f72 123d 0a05 6261 7463 6818 0320 0328  or.=..batch.. .(
+000011c0: 0b32 272e 7065 7266 6574 746f 2e70 726f  .2'.perfetto.pro
+000011d0: 746f 732e 5175 6572 7952 6573 756c 742e  tos.QueryResult.
+000011e0: 4365 6c6c 7342 6174 6368 5205 6261 7463  CellsBatchR.batc
+000011f0: 6812 270a 0f73 7461 7465 6d65 6e74 5f63  h.'..statement_c
+00001200: 6f75 6e74 1804 2001 280d 520e 7374 6174  ount.. .(.R.stat
+00001210: 656d 656e 7443 6f75 6e74 123d 0a1b 7374  ementCount.=..st
+00001220: 6174 656d 656e 745f 7769 7468 5f6f 7574  atement_with_out
+00001230: 7075 745f 636f 756e 7418 0520 0128 0d52  put_count.. .(.R
+00001240: 1873 7461 7465 6d65 6e74 5769 7468 4f75  .statementWithOu
+00001250: 7470 7574 436f 756e 741a 8403 0a0a 4365  tputCount.....Ce
+00001260: 6c6c 7342 6174 6368 124a 0a05 6365 6c6c  llsBatch.J..cell
+00001270: 7318 0120 0328 0e32 302e 7065 7266 6574  s.. .(.20.perfet
+00001280: 746f 2e70 726f 746f 732e 5175 6572 7952  to.protos.QueryR
+00001290: 6573 756c 742e 4365 6c6c 7342 6174 6368  esult.CellsBatch
+000012a0: 2e43 656c 6c54 7970 6542 0210 0152 0563  .CellTypeB...R.c
+000012b0: 656c 6c73 1225 0a0c 7661 7269 6e74 5f63  ells.%..varint_c
+000012c0: 656c 6c73 1802 2003 2803 4202 1001 520b  ells.. .(.B...R.
+000012d0: 7661 7269 6e74 4365 6c6c 7312 270a 0d66  varintCells.'..f
+000012e0: 6c6f 6174 3634 5f63 656c 6c73 1803 2003  loat64_cells.. .
+000012f0: 2801 4202 1001 520c 666c 6f61 7436 3443  (.B...R.float64C
+00001300: 656c 6c73 121d 0a0a 626c 6f62 5f63 656c  ells....blob_cel
+00001310: 6c73 1804 2003 280c 5209 626c 6f62 4365  ls.. .(.R.blobCe
+00001320: 6c6c 7312 210a 0c73 7472 696e 675f 6365  lls.!..string_ce
+00001330: 6c6c 7318 0520 0128 0952 0b73 7472 696e  lls.. .(.R.strin
+00001340: 6743 656c 6c73 1222 0a0d 6973 5f6c 6173  gCells."..is_las
+00001350: 745f 6261 7463 6818 0620 0128 0852 0b69  t_batch.. .(.R.i
+00001360: 734c 6173 7442 6174 6368 226e 0a08 4365  sLastBatch"n..Ce
+00001370: 6c6c 5479 7065 1210 0a0c 4345 4c4c 5f49  llType....CELL_I
+00001380: 4e56 414c 4944 1000 120d 0a09 4345 4c4c  NVALID......CELL
+00001390: 5f4e 554c 4c10 0112 0f0a 0b43 454c 4c5f  _NULL......CELL_
+000013a0: 5641 5249 4e54 1002 1210 0a0c 4345 4c4c  VARINT......CELL
+000013b0: 5f46 4c4f 4154 3634 1003 120f 0a0b 4345  _FLOAT64......CE
+000013c0: 4c4c 5f53 5452 494e 4710 0412 0d0a 0943  LL_STRING......C
+000013d0: 454c 4c5f 424c 4f42 1005 4a04 0807 1008  ELL_BLOB..J.....
+000013e0: 220c 0a0a 5374 6174 7573 4172 6773 2291  "...StatusArgs".
+000013f0: 010a 0c53 7461 7475 7352 6573 756c 7412  ...StatusResult.
+00001400: 2a0a 116c 6f61 6465 645f 7472 6163 655f  *..loaded_trace_
+00001410: 6e61 6d65 1801 2001 2809 520f 6c6f 6164  name.. .(.R.load
+00001420: 6564 5472 6163 654e 616d 6512 340a 1668  edTraceName.4..h
+00001430: 756d 616e 5f72 6561 6461 626c 655f 7665  uman_readable_ve
+00001440: 7273 696f 6e18 0220 0128 0952 1468 756d  rsion.. .(.R.hum
+00001450: 616e 5265 6164 6162 6c65 5665 7273 696f  anReadableVersio
+00001460: 6e12 1f0a 0b61 7069 5f76 6572 7369 6f6e  n....api_version
+00001470: 1803 2001 2805 520a 6170 6956 6572 7369  .. .(.R.apiVersi
+00001480: 6f6e 22b3 010a 1143 6f6d 7075 7465 4d65  on"....ComputeMe
+00001490: 7472 6963 4172 6773 1221 0a0c 6d65 7472  tricArgs.!..metr
+000014a0: 6963 5f6e 616d 6573 1801 2003 2809 520b  ic_names.. .(.R.
+000014b0: 6d65 7472 6963 4e61 6d65 7312 470a 0666  metricNames.G..f
+000014c0: 6f72 6d61 7418 0220 0128 0e32 2f2e 7065  ormat.. .(.2/.pe
+000014d0: 7266 6574 746f 2e70 726f 746f 732e 436f  rfetto.protos.Co
+000014e0: 6d70 7574 654d 6574 7269 6341 7267 732e  mputeMetricArgs.
+000014f0: 5265 7375 6c74 466f 726d 6174 5206 666f  ResultFormatR.fo
+00001500: 726d 6174 2232 0a0c 5265 7375 6c74 466f  rmat"2..ResultFo
+00001510: 726d 6174 1213 0a0f 4249 4e41 5259 5f50  rmat....BINARY_P
+00001520: 524f 544f 4255 4610 0012 0d0a 0954 4558  ROTOBUF......TEX
+00001530: 5450 524f 544f 1001 2285 010a 1343 6f6d  TPROTO.."....Com
+00001540: 7075 7465 4d65 7472 6963 5265 7375 6c74  puteMetricResult
+00001550: 121a 0a07 6d65 7472 6963 7318 0120 0128  ....metrics.. .(
+00001560: 0c48 0052 076d 6574 7269 6373 1232 0a14  .H.R.metrics.2..
+00001570: 6d65 7472 6963 735f 6173 5f70 726f 746f  metrics_as_proto
+00001580: 7465 7874 1803 2001 2809 4800 5212 6d65  text.. .(.H.R.me
+00001590: 7472 6963 7341 7350 726f 746f 7465 7874  tricsAsPrototext
+000015a0: 1214 0a05 6572 726f 7218 0220 0128 0952  ....error.. .(.R
+000015b0: 0565 7272 6f72 4208 0a06 7265 7375 6c74  .errorB...result
+000015c0: 225b 0a13 456e 6162 6c65 4d65 7461 7472  "[..EnableMetatr
+000015d0: 6163 6541 7267 7312 440a 0a63 6174 6567  aceArgs.D..categ
+000015e0: 6f72 6965 7318 0120 0128 0e32 242e 7065  ories.. .(.2$.pe
+000015f0: 7266 6574 746f 2e70 726f 746f 732e 4d65  rfetto.protos.Me
+00001600: 7461 7472 6163 6543 6174 6567 6f72 6965  tatraceCategorie
+00001610: 7352 0a63 6174 6567 6f72 6965 7322 170a  sR.categories"..
+00001620: 1545 6e61 626c 654d 6574 6174 7261 6365  .EnableMetatrace
+00001630: 5265 7375 6c74 221d 0a1b 4469 7361 626c  Result"...Disabl
+00001640: 6541 6e64 5265 6164 4d65 7461 7472 6163  eAndReadMetatrac
+00001650: 6541 7267 7322 530a 1d44 6973 6162 6c65  eArgs"S..Disable
+00001660: 416e 6452 6561 644d 6574 6174 7261 6365  AndReadMetatrace
+00001670: 5265 7375 6c74 121c 0a09 6d65 7461 7472  Result....metatr
+00001680: 6163 6518 0120 0128 0c52 096d 6574 6174  ace.. .(.R.metat
+00001690: 7261 6365 1214 0a05 6572 726f 7218 0220  race....error.. 
+000016a0: 0128 0952 0565 7272 6f72 2253 0a0d 4465  .(.R.error"S..De
+000016b0: 7363 7269 7074 6f72 5365 7412 420a 0b64  scriptorSet.B..d
+000016c0: 6573 6372 6970 746f 7273 1801 2003 280b  escriptors.. .(.
+000016d0: 3220 2e70 6572 6665 7474 6f2e 7072 6f74  2 .perfetto.prot
+000016e0: 6f73 2e44 6573 6372 6970 746f 7250 726f  os.DescriptorPro
+000016f0: 746f 520b 6465 7363 7269 7074 6f72 7322  toR.descriptors"
+00001700: e402 0a17 5265 7365 7454 7261 6365 5072  ....ResetTracePr
+00001710: 6f63 6573 736f 7241 7267 7312 8101 0a1c  ocessorArgs.....
+00001720: 6472 6f70 5f74 7261 636b 5f65 7665 6e74  drop_track_event
+00001730: 5f64 6174 615f 6265 666f 7265 1801 2001  _data_before.. .
+00001740: 280e 3241 2e70 6572 6665 7474 6f2e 7072  (.2A.perfetto.pr
+00001750: 6f74 6f73 2e52 6573 6574 5472 6163 6550  otos.ResetTraceP
+00001760: 726f 6365 7373 6f72 4172 6773 2e44 726f  rocessorArgs.Dro
+00001770: 7054 7261 636b 4576 656e 7444 6174 6142  pTrackEventDataB
+00001780: 6566 6f72 6552 1864 726f 7054 7261 636b  eforeR.dropTrack
+00001790: 4576 656e 7444 6174 6142 6566 6f72 6512  EventDataBefore.
+000017a0: 3a0a 1a69 6e67 6573 745f 6674 7261 6365  :..ingest_ftrace
+000017b0: 5f69 6e5f 7261 775f 7461 626c 6518 0220  _in_raw_table.. 
+000017c0: 0128 0852 1669 6e67 6573 7446 7472 6163  .(.R.ingestFtrac
+000017d0: 6549 6e52 6177 5461 626c 6512 3d0a 1b61  eInRawTable.=..a
+000017e0: 6e61 6c79 7a65 5f74 7261 6365 5f70 726f  nalyze_trace_pro
+000017f0: 746f 5f63 6f6e 7465 6e74 1803 2001 2808  to_content.. .(.
+00001800: 5218 616e 616c 797a 6554 7261 6365 5072  R.analyzeTracePr
+00001810: 6f74 6f43 6f6e 7465 6e74 224a 0a18 4472  otoContent"J..Dr
+00001820: 6f70 5472 6163 6b45 7665 6e74 4461 7461  opTrackEventData
+00001830: 4265 666f 7265 120b 0a07 4e4f 5f44 524f  Before....NO_DRO
+00001840: 5010 0012 210a 1d54 5241 434b 5f45 5645  P...!..TRACK_EVE
+00001850: 4e54 5f52 414e 4745 5f4f 465f 494e 5445  NT_RANGE_OF_INTE
+00001860: 5245 5354 1001 2a43 0a18 5472 6163 6550  REST..*C..TraceP
+00001870: 726f 6365 7373 6f72 4170 6956 6572 7369  rocessorApiVersi
+00001880: 6f6e 1227 0a23 5452 4143 455f 5052 4f43  on.'.#TRACE_PROC
+00001890: 4553 534f 525f 4355 5252 454e 545f 4150  ESSOR_CURRENT_AP
+000018a0: 495f 5645 5253 494f 4e10 07              I_VERSION..
```

### Comparing `perfetto-0.6.0/perfetto/trace_uri_resolver/path.py` & `perfetto-0.7.0/perfetto/trace_uri_resolver/path.py`

 * *Files identical despite different names*

### Comparing `perfetto-0.6.0/perfetto/trace_uri_resolver/registry.py` & `perfetto-0.7.0/perfetto/trace_uri_resolver/registry.py`

 * *Files identical despite different names*

### Comparing `perfetto-0.6.0/perfetto/trace_uri_resolver/resolver.py` & `perfetto-0.7.0/perfetto/trace_uri_resolver/resolver.py`

 * *Files identical despite different names*

### Comparing `perfetto-0.6.0/perfetto/trace_uri_resolver/util.py` & `perfetto-0.7.0/perfetto/trace_uri_resolver/util.py`

 * *Files identical despite different names*

### Comparing `perfetto-0.6.0/setup.py` & `perfetto-0.7.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     name='perfetto',
     packages=[
         'perfetto', 'perfetto.batch_trace_processor',
         'perfetto.trace_processor', 'perfetto.trace_uri_resolver'
     ],
     package_data={'perfetto.trace_processor': ['*.descriptor']},
     include_package_data=True,
-    version='0.6.0',
+    version='0.7.0',
     license='apache-2.0',
     description='Python API for Perfetto\'s Trace Processor',
     author='Perfetto',
     author_email='perfetto-pypi@google.com',
     url='https://perfetto.dev/',
     download_url='https://github.com/google/perfetto/archive/refs/tags/v30.0.tar.gz',
     keywords=['trace processor', 'tracing', 'perfetto'],
```

