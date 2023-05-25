# Comparing `tmp/PythonToolsKit-1.2.5.tar.gz` & `tmp/PythonToolsKit-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PythonToolsKit-1.2.5.tar", last modified: Fri May  5 10:40:51 2023, max compression
+gzip compressed data, was "PythonToolsKit-1.2.6.tar", last modified: Thu May 25 19:38:07 2023, max compression
```

## Comparing `PythonToolsKit-1.2.5.tar` & `PythonToolsKit-1.2.6.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-05-05 10:40:51.434679 PythonToolsKit-1.2.5/
--rw-r--r--   0 kali      (1000) kali      (1000)    35149 2023-05-05 14:37:14.000000 PythonToolsKit-1.2.5/LICENSE.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       27 2023-05-05 14:37:14.000000 PythonToolsKit-1.2.5/MANIFEST.in
--rw-r--r--   0 kali      (1000) kali      (1000)    15504 2023-05-05 10:40:51.434679 PythonToolsKit-1.2.5/PKG-INFO
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-05-05 10:40:51.434679 PythonToolsKit-1.2.5/PythonToolsKit/
--rw-r--r--   0 kali      (1000) kali      (1000)    14031 2023-05-05 14:37:14.000000 PythonToolsKit-1.2.5/PythonToolsKit/Arguments.py
--rw-r--r--   0 kali      (1000) kali      (1000)     8577 2023-05-05 14:37:14.000000 PythonToolsKit-1.2.5/PythonToolsKit/Characters.py
--rw-r--r--   0 kali      (1000) kali      (1000)    27267 2023-05-05 14:37:14.000000 PythonToolsKit-1.2.5/PythonToolsKit/Colors.py
--rw-r--r--   0 kali      (1000) kali      (1000)    42959 2023-05-05 14:44:46.000000 PythonToolsKit-1.2.5/PythonToolsKit/DataAnalysis.py
--rw-r--r--   0 kali      (1000) kali      (1000)    19183 2023-05-05 14:37:14.000000 PythonToolsKit-1.2.5/PythonToolsKit/DebugEncoding.py
--rw-r--r--   0 kali      (1000) kali      (1000)     5837 2023-05-05 14:37:14.000000 PythonToolsKit-1.2.5/PythonToolsKit/Dict.py
--rw-r--r--   0 kali      (1000) kali      (1000)     4452 2023-05-05 14:37:14.000000 PythonToolsKit-1.2.5/PythonToolsKit/DictObject.py
--rw-r--r--   0 kali      (1000) kali      (1000)    11277 2023-05-05 14:37:14.000000 PythonToolsKit-1.2.5/PythonToolsKit/Encodings.py
--rw-r--r--   0 kali      (1000) kali      (1000)     2661 2023-05-05 14:37:14.000000 PythonToolsKit-1.2.5/PythonToolsKit/Function.py
--rw-r--r--   0 kali      (1000) kali      (1000)     3701 2023-05-05 14:37:14.000000 PythonToolsKit-1.2.5/PythonToolsKit/GetFile.py
--rw-r--r--   0 kali      (1000) kali      (1000)     3810 2023-05-05 14:37:14.000000 PythonToolsKit-1.2.5/PythonToolsKit/GetPass.py
--rw-r--r--   0 kali      (1000) kali      (1000)    19618 2023-05-05 14:37:14.000000 PythonToolsKit-1.2.5/PythonToolsKit/GetType.py
--rw-r--r--   0 kali      (1000) kali      (1000)     2400 2023-05-05 14:37:14.000000 PythonToolsKit-1.2.5/PythonToolsKit/Import.py
--rw-r--r--   0 kali      (1000) kali      (1000)     5260 2023-05-05 14:37:14.000000 PythonToolsKit-1.2.5/PythonToolsKit/Json.py
--rw-r--r--   0 kali      (1000) kali      (1000)     3225 2023-05-05 14:37:14.000000 PythonToolsKit-1.2.5/PythonToolsKit/List.py
--rw-r--r--   0 kali      (1000) kali      (1000)     8574 2023-05-05 14:37:14.000000 PythonToolsKit-1.2.5/PythonToolsKit/Logs.py
--rw-r--r--   0 kali      (1000) kali      (1000)    16523 2023-05-05 14:37:14.000000 PythonToolsKit-1.2.5/PythonToolsKit/OrdDict.py
--rw-r--r--   0 kali      (1000) kali      (1000)     5351 2023-05-05 14:37:14.000000 PythonToolsKit-1.2.5/PythonToolsKit/PrintF.py
--rw-r--r--   0 kali      (1000) kali      (1000)     3392 2023-05-05 14:37:14.000000 PythonToolsKit-1.2.5/PythonToolsKit/Process.py
--rw-r--r--   0 kali      (1000) kali      (1000)     6189 2023-05-05 14:37:14.000000 PythonToolsKit-1.2.5/PythonToolsKit/Random.py
--rw-r--r--   0 kali      (1000) kali      (1000)     2488 2023-05-05 14:37:14.000000 PythonToolsKit-1.2.5/PythonToolsKit/RecursionDebug.py
--rw-r--r--   0 kali      (1000) kali      (1000)    18306 2023-05-05 14:37:14.000000 PythonToolsKit-1.2.5/PythonToolsKit/Report.py
--rw-r--r--   0 kali      (1000) kali      (1000)     9654 2023-05-05 14:37:14.000000 PythonToolsKit-1.2.5/PythonToolsKit/ScapyTools.py
--rw-r--r--   0 kali      (1000) kali      (1000)     7131 2023-05-05 14:37:14.000000 PythonToolsKit-1.2.5/PythonToolsKit/StringF.py
--rw-r--r--   0 kali      (1000) kali      (1000)    15457 2023-05-05 14:37:14.000000 PythonToolsKit-1.2.5/PythonToolsKit/Terminal.py
--rw-r--r--   0 kali      (1000) kali      (1000)     1106 2023-05-05 14:37:14.000000 PythonToolsKit-1.2.5/PythonToolsKit/TestArguments.py
--rw-r--r--   0 kali      (1000) kali      (1000)     4710 2023-05-05 14:37:14.000000 PythonToolsKit-1.2.5/PythonToolsKit/TestTimeout.py
--rw-r--r--   0 kali      (1000) kali      (1000)     3092 2023-05-05 14:37:14.000000 PythonToolsKit-1.2.5/PythonToolsKit/Thread.py
--rw-r--r--   0 kali      (1000) kali      (1000)     7854 2023-05-05 14:37:14.000000 PythonToolsKit-1.2.5/PythonToolsKit/Timeout.py
--rw-r--r--   0 kali      (1000) kali      (1000)     3252 2023-05-05 14:37:14.000000 PythonToolsKit-1.2.5/PythonToolsKit/Tuple.py
--rw-r--r--   0 kali      (1000) kali      (1000)    10004 2023-05-05 14:37:14.000000 PythonToolsKit-1.2.5/PythonToolsKit/WindowsTerminal.py
--rw-r--r--   0 kali      (1000) kali      (1000)     1641 2023-05-05 14:44:58.000000 PythonToolsKit-1.2.5/PythonToolsKit/__init__.py
--rw-r--r--   0 kali      (1000) kali      (1000)     5935 2023-05-05 14:37:14.000000 PythonToolsKit-1.2.5/PythonToolsKit/urlopen.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-05-05 10:40:51.434679 PythonToolsKit-1.2.5/PythonToolsKit.egg-info/
--rw-r--r--   0 kali      (1000) kali      (1000)    15504 2023-05-05 10:40:51.000000 PythonToolsKit-1.2.5/PythonToolsKit.egg-info/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)     1135 2023-05-05 10:40:51.000000 PythonToolsKit-1.2.5/PythonToolsKit.egg-info/SOURCES.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-05-05 10:40:51.000000 PythonToolsKit-1.2.5/PythonToolsKit.egg-info/dependency_links.txt
--rw-r--r--   0 kali      (1000) kali      (1000)      112 2023-05-05 10:40:51.000000 PythonToolsKit-1.2.5/PythonToolsKit.egg-info/entry_points.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       15 2023-05-05 10:40:51.000000 PythonToolsKit-1.2.5/PythonToolsKit.egg-info/top_level.txt
--rw-r--r--   0 kali      (1000) kali      (1000)    10968 2023-05-05 14:37:14.000000 PythonToolsKit-1.2.5/README.md
--rw-r--r--   0 kali      (1000) kali      (1000)       38 2023-05-05 10:40:51.434679 PythonToolsKit-1.2.5/setup.cfg
--rw-r--r--   0 kali      (1000) kali      (1000)     6693 2023-05-05 14:37:14.000000 PythonToolsKit-1.2.5/setup.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-05-25 19:38:07.119105 PythonToolsKit-1.2.6/
+-rw-r--r--   0 kali      (1000) kali      (1000)    35149 2023-05-26 01:32:02.000000 PythonToolsKit-1.2.6/LICENSE.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       27 2023-05-26 01:32:02.000000 PythonToolsKit-1.2.6/MANIFEST.in
+-rw-r--r--   0 kali      (1000) kali      (1000)    15504 2023-05-25 19:38:07.119105 PythonToolsKit-1.2.6/PKG-INFO
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-05-25 19:38:07.115103 PythonToolsKit-1.2.6/PythonToolsKit/
+-rw-r--r--   0 kali      (1000) kali      (1000)    14031 2023-05-26 01:32:02.000000 PythonToolsKit-1.2.6/PythonToolsKit/Arguments.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     8577 2023-05-26 01:32:02.000000 PythonToolsKit-1.2.6/PythonToolsKit/Characters.py
+-rw-r--r--   0 kali      (1000) kali      (1000)    27267 2023-05-26 01:32:02.000000 PythonToolsKit-1.2.6/PythonToolsKit/Colors.py
+-rw-r--r--   0 kali      (1000) kali      (1000)    42959 2023-05-26 01:32:02.000000 PythonToolsKit-1.2.6/PythonToolsKit/DataAnalysis.py
+-rw-r--r--   0 kali      (1000) kali      (1000)    19183 2023-05-26 01:32:02.000000 PythonToolsKit-1.2.6/PythonToolsKit/DebugEncoding.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     5837 2023-05-26 01:32:02.000000 PythonToolsKit-1.2.6/PythonToolsKit/Dict.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     4452 2023-05-26 01:32:02.000000 PythonToolsKit-1.2.6/PythonToolsKit/DictObject.py
+-rw-r--r--   0 kali      (1000) kali      (1000)    11277 2023-05-26 01:32:02.000000 PythonToolsKit-1.2.6/PythonToolsKit/Encodings.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     2661 2023-05-26 01:32:02.000000 PythonToolsKit-1.2.6/PythonToolsKit/Function.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     3701 2023-05-26 01:32:02.000000 PythonToolsKit-1.2.6/PythonToolsKit/GetFile.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     3810 2023-05-26 01:32:02.000000 PythonToolsKit-1.2.6/PythonToolsKit/GetPass.py
+-rw-r--r--   0 kali      (1000) kali      (1000)    19618 2023-05-26 01:32:02.000000 PythonToolsKit-1.2.6/PythonToolsKit/GetType.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     2400 2023-05-26 01:32:02.000000 PythonToolsKit-1.2.6/PythonToolsKit/Import.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     5260 2023-05-26 01:32:02.000000 PythonToolsKit-1.2.6/PythonToolsKit/Json.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     3225 2023-05-26 01:32:02.000000 PythonToolsKit-1.2.6/PythonToolsKit/List.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     8574 2023-05-26 01:32:02.000000 PythonToolsKit-1.2.6/PythonToolsKit/Logs.py
+-rw-r--r--   0 kali      (1000) kali      (1000)    16523 2023-05-26 01:32:02.000000 PythonToolsKit-1.2.6/PythonToolsKit/OrdDict.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     5377 2023-05-26 01:34:52.000000 PythonToolsKit-1.2.6/PythonToolsKit/PrintF.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     3392 2023-05-26 01:32:02.000000 PythonToolsKit-1.2.6/PythonToolsKit/Process.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     6189 2023-05-26 01:32:02.000000 PythonToolsKit-1.2.6/PythonToolsKit/Random.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     2488 2023-05-26 01:32:02.000000 PythonToolsKit-1.2.6/PythonToolsKit/RecursionDebug.py
+-rw-r--r--   0 kali      (1000) kali      (1000)    18306 2023-05-26 01:32:02.000000 PythonToolsKit-1.2.6/PythonToolsKit/Report.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     9654 2023-05-26 01:32:02.000000 PythonToolsKit-1.2.6/PythonToolsKit/ScapyTools.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     7131 2023-05-26 01:32:02.000000 PythonToolsKit-1.2.6/PythonToolsKit/StringF.py
+-rw-r--r--   0 kali      (1000) kali      (1000)    15457 2023-05-26 01:32:02.000000 PythonToolsKit-1.2.6/PythonToolsKit/Terminal.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     1106 2023-05-26 01:32:02.000000 PythonToolsKit-1.2.6/PythonToolsKit/TestArguments.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     4710 2023-05-26 01:32:02.000000 PythonToolsKit-1.2.6/PythonToolsKit/TestTimeout.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     3092 2023-05-26 01:32:02.000000 PythonToolsKit-1.2.6/PythonToolsKit/Thread.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     7854 2023-05-26 01:32:02.000000 PythonToolsKit-1.2.6/PythonToolsKit/Timeout.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     3252 2023-05-26 01:32:02.000000 PythonToolsKit-1.2.6/PythonToolsKit/Tuple.py
+-rw-r--r--   0 kali      (1000) kali      (1000)    10004 2023-05-26 01:32:02.000000 PythonToolsKit-1.2.6/PythonToolsKit/WindowsTerminal.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     1641 2023-05-26 01:35:14.000000 PythonToolsKit-1.2.6/PythonToolsKit/__init__.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     5935 2023-05-26 01:32:02.000000 PythonToolsKit-1.2.6/PythonToolsKit/urlopen.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-05-25 19:38:07.119105 PythonToolsKit-1.2.6/PythonToolsKit.egg-info/
+-rw-r--r--   0 kali      (1000) kali      (1000)    15504 2023-05-25 19:38:07.000000 PythonToolsKit-1.2.6/PythonToolsKit.egg-info/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)     1135 2023-05-25 19:38:07.000000 PythonToolsKit-1.2.6/PythonToolsKit.egg-info/SOURCES.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-05-25 19:38:07.000000 PythonToolsKit-1.2.6/PythonToolsKit.egg-info/dependency_links.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)      112 2023-05-25 19:38:07.000000 PythonToolsKit-1.2.6/PythonToolsKit.egg-info/entry_points.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       15 2023-05-25 19:38:07.000000 PythonToolsKit-1.2.6/PythonToolsKit.egg-info/top_level.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)    10968 2023-05-26 01:32:02.000000 PythonToolsKit-1.2.6/README.md
+-rw-r--r--   0 kali      (1000) kali      (1000)       38 2023-05-25 19:38:07.119105 PythonToolsKit-1.2.6/setup.cfg
+-rw-r--r--   0 kali      (1000) kali      (1000)     6693 2023-05-26 01:32:02.000000 PythonToolsKit-1.2.6/setup.py
```

### Comparing `PythonToolsKit-1.2.5/LICENSE.txt` & `PythonToolsKit-1.2.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PythonToolsKit-1.2.5/PKG-INFO` & `PythonToolsKit-1.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PythonToolsKit
-Version: 1.2.5
+Version: 1.2.6
 Summary: This package implements tools to build python package and tools.
 Home-page: https://github.com/mauricelambert/PythonToolsKit
 Author: Maurice Lambert
 Author-email: mauricelambert434@gmail.com
 Maintainer: Maurice Lambert
 Maintainer-email: mauricelambert434@gmail.com
 License: GPL-3.0 License
```

### Comparing `PythonToolsKit-1.2.5/PythonToolsKit/Arguments.py` & `PythonToolsKit-1.2.6/PythonToolsKit/Arguments.py`

 * *Files identical despite different names*

### Comparing `PythonToolsKit-1.2.5/PythonToolsKit/Characters.py` & `PythonToolsKit-1.2.6/PythonToolsKit/Characters.py`

 * *Files identical despite different names*

### Comparing `PythonToolsKit-1.2.5/PythonToolsKit/Colors.py` & `PythonToolsKit-1.2.6/PythonToolsKit/Colors.py`

 * *Files identical despite different names*

### Comparing `PythonToolsKit-1.2.5/PythonToolsKit/DataAnalysis.py` & `PythonToolsKit-1.2.6/PythonToolsKit/DataAnalysis.py`

 * *Files identical despite different names*

### Comparing `PythonToolsKit-1.2.5/PythonToolsKit/DebugEncoding.py` & `PythonToolsKit-1.2.6/PythonToolsKit/DebugEncoding.py`

 * *Files identical despite different names*

### Comparing `PythonToolsKit-1.2.5/PythonToolsKit/Dict.py` & `PythonToolsKit-1.2.6/PythonToolsKit/Dict.py`

 * *Files identical despite different names*

### Comparing `PythonToolsKit-1.2.5/PythonToolsKit/DictObject.py` & `PythonToolsKit-1.2.6/PythonToolsKit/DictObject.py`

 * *Files identical despite different names*

### Comparing `PythonToolsKit-1.2.5/PythonToolsKit/Encodings.py` & `PythonToolsKit-1.2.6/PythonToolsKit/Encodings.py`

 * *Files identical despite different names*

### Comparing `PythonToolsKit-1.2.5/PythonToolsKit/Function.py` & `PythonToolsKit-1.2.6/PythonToolsKit/Function.py`

 * *Files identical despite different names*

### Comparing `PythonToolsKit-1.2.5/PythonToolsKit/GetFile.py` & `PythonToolsKit-1.2.6/PythonToolsKit/GetFile.py`

 * *Files identical despite different names*

### Comparing `PythonToolsKit-1.2.5/PythonToolsKit/GetPass.py` & `PythonToolsKit-1.2.6/PythonToolsKit/GetPass.py`

 * *Files identical despite different names*

### Comparing `PythonToolsKit-1.2.5/PythonToolsKit/GetType.py` & `PythonToolsKit-1.2.6/PythonToolsKit/GetType.py`

 * *Files identical despite different names*

### Comparing `PythonToolsKit-1.2.5/PythonToolsKit/Import.py` & `PythonToolsKit-1.2.6/PythonToolsKit/Import.py`

 * *Files identical despite different names*

### Comparing `PythonToolsKit-1.2.5/PythonToolsKit/Json.py` & `PythonToolsKit-1.2.6/PythonToolsKit/Json.py`

 * *Files identical despite different names*

### Comparing `PythonToolsKit-1.2.5/PythonToolsKit/List.py` & `PythonToolsKit-1.2.6/PythonToolsKit/List.py`

 * *Files identical despite different names*

### Comparing `PythonToolsKit-1.2.5/PythonToolsKit/Logs.py` & `PythonToolsKit-1.2.6/PythonToolsKit/Logs.py`

 * *Files identical despite different names*

### Comparing `PythonToolsKit-1.2.5/PythonToolsKit/OrdDict.py` & `PythonToolsKit-1.2.6/PythonToolsKit/OrdDict.py`

 * *Files identical despite different names*

### Comparing `PythonToolsKit-1.2.5/PythonToolsKit/PrintF.py` & `PythonToolsKit-1.2.6/PythonToolsKit/PrintF.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 ###################
 #    This package implements tools to build python package and tools.
-#    Copyright (C) 2021  Maurice Lambert
+#    Copyright (C) 2021, 2022, 2023  Maurice Lambert
 
 #    This program is free software: you can redistribute it and/or modify
 #    it under the terms of the GNU General Public License as published by
 #    the Free Software Foundation, either version 3 of the License, or
 #    (at your option) any later version.
 
 #    This program is distributed in the hope that it will be useful,
@@ -63,27 +63,27 @@
 >>> custom_progress = ProgressBar("[", "]", "#", "-", 30)
 >>> printf("Step 1 OK", progressbar=custom_progress, pourcent=20); print()
 [+] Step 1 OK
 [+] 20% [######------------------------]
 >>>
 """
 
-__version__ = "1.0.0"
+__version__ = "1.0.1"
 __author__ = "Maurice Lambert"
 __author_email__ = "mauricelambert434@gmail.com"
 __maintainer__ = "Maurice Lambert"
 __maintainer_email__ = "mauricelambert434@gmail.com"
 __description__ = """
 This package implements tools to build python package and tools.
 """
 license = "GPL-3.0 License"
 __url__ = "https://github.com/mauricelambert/PythonToolsKit"
 
 copyright = """
-PythonToolsKit  Copyright (C) 2022  Maurice Lambert
+PythonToolsKit  Copyright (C) 2021, 2022, 2023  Maurice Lambert
 This program comes with ABSOLUTELY NO WARRANTY.
 This is free software, and you are welcome to redistribute it
 under certain conditions.
 """
 __license__ = license
 __copyright__ = copyright
 
@@ -146,20 +146,20 @@
             progressbar.start
             + (progressbar.character * pourcent_size)
             + (progressbar.empty * (max_size - pourcent_size))
             + progressbar.end
         )
 
     if has_pourcent:
-        progress_bar = f"{pourcent}% {progress_bar}\x1b[0m{end}\x1b[F"
+        progress_bar = f"{pourcent}% {progress_bar}\x1b[39m{end}\x1b[F"
         if not oneline_progress:
             progress_bar = f"{color}{show} {progress_bar}"
 
     if oneline_progress:
         to_print = f"\x1b[K{start}{color}{show} {string} {progress_bar}"
     else:
         to_print = (
-            f"\x1b[K{start}{color}{show} {string}\x1b[0m{end}"
+            f"\x1b[K{start}{color}{show} {string}\x1b[39m{end}"
             f"{progress_bar}"
         )
 
     print(to_print, flush=True, end="", **kwargs)
```

### Comparing `PythonToolsKit-1.2.5/PythonToolsKit/Process.py` & `PythonToolsKit-1.2.6/PythonToolsKit/Process.py`

 * *Files identical despite different names*

### Comparing `PythonToolsKit-1.2.5/PythonToolsKit/Random.py` & `PythonToolsKit-1.2.6/PythonToolsKit/Random.py`

 * *Files identical despite different names*

### Comparing `PythonToolsKit-1.2.5/PythonToolsKit/RecursionDebug.py` & `PythonToolsKit-1.2.6/PythonToolsKit/RecursionDebug.py`

 * *Files identical despite different names*

### Comparing `PythonToolsKit-1.2.5/PythonToolsKit/Report.py` & `PythonToolsKit-1.2.6/PythonToolsKit/Report.py`

 * *Files identical despite different names*

### Comparing `PythonToolsKit-1.2.5/PythonToolsKit/ScapyTools.py` & `PythonToolsKit-1.2.6/PythonToolsKit/ScapyTools.py`

 * *Files identical despite different names*

### Comparing `PythonToolsKit-1.2.5/PythonToolsKit/StringF.py` & `PythonToolsKit-1.2.6/PythonToolsKit/StringF.py`

 * *Files identical despite different names*

### Comparing `PythonToolsKit-1.2.5/PythonToolsKit/Terminal.py` & `PythonToolsKit-1.2.6/PythonToolsKit/Terminal.py`

 * *Files identical despite different names*

### Comparing `PythonToolsKit-1.2.5/PythonToolsKit/TestArguments.py` & `PythonToolsKit-1.2.6/PythonToolsKit/TestArguments.py`

 * *Files identical despite different names*

### Comparing `PythonToolsKit-1.2.5/PythonToolsKit/TestTimeout.py` & `PythonToolsKit-1.2.6/PythonToolsKit/TestTimeout.py`

 * *Files identical despite different names*

### Comparing `PythonToolsKit-1.2.5/PythonToolsKit/Thread.py` & `PythonToolsKit-1.2.6/PythonToolsKit/Thread.py`

 * *Files identical despite different names*

### Comparing `PythonToolsKit-1.2.5/PythonToolsKit/Timeout.py` & `PythonToolsKit-1.2.6/PythonToolsKit/Timeout.py`

 * *Files identical despite different names*

### Comparing `PythonToolsKit-1.2.5/PythonToolsKit/Tuple.py` & `PythonToolsKit-1.2.6/PythonToolsKit/Tuple.py`

 * *Files identical despite different names*

### Comparing `PythonToolsKit-1.2.5/PythonToolsKit/WindowsTerminal.py` & `PythonToolsKit-1.2.6/PythonToolsKit/WindowsTerminal.py`

 * *Files identical despite different names*

### Comparing `PythonToolsKit-1.2.5/PythonToolsKit/__init__.py` & `PythonToolsKit-1.2.6/PythonToolsKit/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 #    along with this program.  If not, see <https://www.gnu.org/licenses/>.
 ###################
 
 """
 This package implements tools to build python package and tools.
 """
 
-__version__ = "1.2.5"
+__version__ = "1.2.6"
 __author__ = "Maurice Lambert"
 __author_email__ = "mauricelambert434@gmail.com"
 __maintainer__ = "Maurice Lambert"
 __maintainer_email__ = "mauricelambert434@gmail.com"
 __description__ = """
 This package implements tools to build python package and tools.
 """
```

### Comparing `PythonToolsKit-1.2.5/PythonToolsKit/urlopen.py` & `PythonToolsKit-1.2.6/PythonToolsKit/urlopen.py`

 * *Files identical despite different names*

### Comparing `PythonToolsKit-1.2.5/PythonToolsKit.egg-info/PKG-INFO` & `PythonToolsKit-1.2.6/PythonToolsKit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PythonToolsKit
-Version: 1.2.5
+Version: 1.2.6
 Summary: This package implements tools to build python package and tools.
 Home-page: https://github.com/mauricelambert/PythonToolsKit
 Author: Maurice Lambert
 Author-email: mauricelambert434@gmail.com
 Maintainer: Maurice Lambert
 Maintainer-email: mauricelambert434@gmail.com
 License: GPL-3.0 License
```

### Comparing `PythonToolsKit-1.2.5/PythonToolsKit.egg-info/SOURCES.txt` & `PythonToolsKit-1.2.6/PythonToolsKit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PythonToolsKit-1.2.5/README.md` & `PythonToolsKit-1.2.6/README.md`

 * *Files identical despite different names*

### Comparing `PythonToolsKit-1.2.5/setup.py` & `PythonToolsKit-1.2.6/setup.py`

 * *Files identical despite different names*

