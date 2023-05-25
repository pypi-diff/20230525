# Comparing `tmp/tianrannlp-0.0.1-py2.py3-none-any.whl.zip` & `tmp/tianrannlp-0.0.2-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 2410 bytes, number of entries: 7
+Zip file size: 2376 bytes, number of entries: 7
 -rw-r--r--  2.0 unx      138 b- defN 23-May-25 07:48 tianrannlp/__init__.py
--rw-r--r--  2.0 unx      305 b- defN 23-May-25 07:47 tianrannlp/rules/__init__.py
+-rw-r--r--  2.0 unx      306 b- defN 23-May-25 07:52 tianrannlp/rules/__init__.py
 -rw-r--r--  2.0 unx     1642 b- defN 23-May-25 07:44 tianrannlp/rules/stringCheckUtils.py
--rw-r--r--  2.0 unx      239 b- defN 23-May-25 07:49 tianrannlp-0.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-May-25 07:49 tianrannlp-0.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-May-25 07:49 tianrannlp-0.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      565 b- defN 23-May-25 07:49 tianrannlp-0.0.1.dist-info/RECORD
-7 files, 3010 bytes uncompressed, 1404 bytes compressed:  53.4%
+-rw-r--r--  2.0 unx      168 b- defN 23-May-25 07:54 tianrannlp-0.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-May-25 07:54 tianrannlp-0.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-May-25 07:54 tianrannlp-0.0.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      565 b- defN 23-May-25 07:54 tianrannlp-0.0.2.dist-info/RECORD
+7 files, 2940 bytes uncompressed, 1370 bytes compressed:  53.4%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: tianrannlp/rules/__init__.py
 Comment: 
 
 Filename: tianrannlp/rules/stringCheckUtils.py
 Comment: 
 
-Filename: tianrannlp-0.0.1.dist-info/METADATA
+Filename: tianrannlp-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: tianrannlp-0.0.1.dist-info/WHEEL
+Filename: tianrannlp-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: tianrannlp-0.0.1.dist-info/top_level.txt
+Filename: tianrannlp-0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: tianrannlp-0.0.1.dist-info/RECORD
+Filename: tianrannlp-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tianrannlp/rules/__init__.py

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 # @Time    : 5/25/23 3:32 PM
 # @Author  : LIANYONGXING
 # @FileName: __init__.py.py
 
-from stringCheckUtils import StringCheckUtils
+from .stringCheckUtils import StringCheckUtils
 
 
 checker = StringCheckUtils()
 is_all_chinese = checker.is_all_chinese
 is_all_english = checker.is_all_english
 is_all_numbers = checker.is_all_numbers
```

## Comparing `tianrannlp-0.0.1.dist-info/RECORD` & `tianrannlp-0.0.2.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 tianrannlp/__init__.py,sha256=6S0iJidEveFC6C4qYZZ3C26Sxh2i8SrWuTN3C0cXWY4,138
-tianrannlp/rules/__init__.py,sha256=YZEihBw1mbUzSiC8MeqH3IhkFvN6v3dlF5sPLTxXm30,305
+tianrannlp/rules/__init__.py,sha256=0KVFwMij64daiJiVTSYSytN1KoZveZeowwflR8GPUyM,306
 tianrannlp/rules/stringCheckUtils.py,sha256=EBKy0f_rs-Aiel0l828Dd74MlrHqrZP15U_EjhpUm_8,1642
-tianrannlp-0.0.1.dist-info/METADATA,sha256=hqWgwGeH5YSQ0NJwTj6yAxsHtwiCa48gmMaYSPwDTUM,239
-tianrannlp-0.0.1.dist-info/WHEEL,sha256=z9j0xAa_JmUKMpmz72K0ZGALSM_n-wQVmGbleXx2VHg,110
-tianrannlp-0.0.1.dist-info/top_level.txt,sha256=MXUywYNZubOcvY4lTGj6-Kfk4kCIjvlb6CZVOd5grH4,11
-tianrannlp-0.0.1.dist-info/RECORD,,
+tianrannlp-0.0.2.dist-info/METADATA,sha256=ROmEgpjAqD9vV-8_C29u94j_as8hI-5eY89nr4zftiM,168
+tianrannlp-0.0.2.dist-info/WHEEL,sha256=z9j0xAa_JmUKMpmz72K0ZGALSM_n-wQVmGbleXx2VHg,110
+tianrannlp-0.0.2.dist-info/top_level.txt,sha256=MXUywYNZubOcvY4lTGj6-Kfk4kCIjvlb6CZVOd5grH4,11
+tianrannlp-0.0.2.dist-info/RECORD,,
```

