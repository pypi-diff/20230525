# Comparing `tmp/torch_ort-1.9.0-py3-none-any.whl.zip` & `tmp/torch_ort-1.9.0.dev20210923-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 6004 bytes, number of entries: 11
--rw-rw-r--  2.0 unx      582 b- defN 21-Sep-23 01:06 torch_ort/__init__.py
--rw-rw-r--  2.0 unx       21 b- defN 21-Sep-23 01:11 torch_ort/_version.py
--rw-rw-r--  2.0 unx      447 b- defN 21-Sep-23 01:06 torch_ort/configure/__main__.py
--rw-rw-r--  2.0 unx      369 b- defN 21-Sep-23 01:06 torch_ort/experimental/__init__.py
--rw-rw-r--  2.0 unx     4517 b- defN 21-Sep-23 01:06 torch_ort/experimental/graph_config.py
--rw-rw-r--  2.0 unx      331 b- defN 21-Sep-23 01:06 torch_ort/experimental/json_config/__init__.py
--rw-rw-r--  2.0 unx     1072 b- defN 21-Sep-23 01:11 torch_ort-1.9.0.dist-info/LICENSE
--rw-rw-r--  2.0 unx     1715 b- defN 21-Sep-23 01:11 torch_ort-1.9.0.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 21-Sep-23 01:11 torch_ort-1.9.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx       10 b- defN 21-Sep-23 01:11 torch_ort-1.9.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      923 b- defN 21-Sep-23 01:11 torch_ort-1.9.0.dist-info/RECORD
-11 files, 10079 bytes uncompressed, 4426 bytes compressed:  56.1%
+Zip file size: 6158 bytes, number of entries: 11
+-rw-rw-r--  2.0 unx      582 b- defN 21-Sep-22 23:57 torch_ort/__init__.py
+-rw-rw-r--  2.0 unx       33 b- defN 21-Sep-23 00:03 torch_ort/_version.py
+-rw-rw-r--  2.0 unx      447 b- defN 21-Sep-22 23:57 torch_ort/configure/__main__.py
+-rw-rw-r--  2.0 unx      369 b- defN 21-Sep-22 23:57 torch_ort/experimental/__init__.py
+-rw-rw-r--  2.0 unx     4517 b- defN 21-Sep-22 23:57 torch_ort/experimental/graph_config.py
+-rw-rw-r--  2.0 unx      331 b- defN 21-Sep-22 23:57 torch_ort/experimental/json_config/__init__.py
+-rw-rw-r--  2.0 unx     1072 b- defN 21-Sep-23 00:03 torch_ort-1.9.0.dev20210923.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     1727 b- defN 21-Sep-23 00:03 torch_ort-1.9.0.dev20210923.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 21-Sep-23 00:03 torch_ort-1.9.0.dev20210923.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       10 b- defN 21-Sep-23 00:03 torch_ort-1.9.0.dev20210923.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      983 b- defN 21-Sep-23 00:03 torch_ort-1.9.0.dev20210923.dist-info/RECORD
+11 files, 10163 bytes uncompressed, 4460 bytes compressed:  56.1%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: torch_ort/experimental/graph_config.py
 Comment: 
 
 Filename: torch_ort/experimental/json_config/__init__.py
 Comment: 
 
-Filename: torch_ort-1.9.0.dist-info/LICENSE
+Filename: torch_ort-1.9.0.dev20210923.dist-info/LICENSE
 Comment: 
 
-Filename: torch_ort-1.9.0.dist-info/METADATA
+Filename: torch_ort-1.9.0.dev20210923.dist-info/METADATA
 Comment: 
 
-Filename: torch_ort-1.9.0.dist-info/WHEEL
+Filename: torch_ort-1.9.0.dev20210923.dist-info/WHEEL
 Comment: 
 
-Filename: torch_ort-1.9.0.dist-info/top_level.txt
+Filename: torch_ort-1.9.0.dev20210923.dist-info/top_level.txt
 Comment: 
 
-Filename: torch_ort-1.9.0.dist-info/RECORD
+Filename: torch_ort-1.9.0.dev20210923.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## torch_ort/_version.py

```diff
@@ -1 +1 @@
-__version__ = '1.9.0'
+__version__ = '1.9.0.dev20210923'
```

## Comparing `torch_ort-1.9.0.dist-info/LICENSE` & `torch_ort-1.9.0.dev20210923.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `torch_ort-1.9.0.dist-info/METADATA` & `torch_ort-1.9.0.dev20210923.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-ort
-Version: 1.9.0
+Version: 1.9.0.dev20210923
 Summary: Accelerate PyTorch models with ONNX Runtime
 Home-page: https://github.com/pytorch/ort
 Author: torch-ort contributors
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/pytorch/ort/issues
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

