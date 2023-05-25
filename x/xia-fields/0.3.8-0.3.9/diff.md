# Comparing `tmp/xia_fields-0.3.8-cp39-none-win_amd64.whl.zip` & `tmp/xia_fields-0.3.9-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 460729 bytes, number of entries: 9
--rw-r--r--  2.0 unx     1177 b- defN 23-May-04 19:12 xia_fields/__init__.py
--rw-r--r--  2.0 unx   366080 b- defN 23-May-04 19:16 xia_fields/base.cp39-win_amd64.pyd
--rw-r--r--  2.0 unx   415744 b- defN 23-May-04 19:17 xia_fields/fields.cp39-win_amd64.pyd
--rw-r--r--  2.0 unx   388096 b- defN 23-May-04 19:19 xia_fields/fields_ext.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      152 b- defN 23-May-04 19:19 xia_fields-0.3.8.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     3308 b- defN 23-May-04 19:19 xia_fields-0.3.8.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-May-04 19:19 xia_fields-0.3.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-May-04 19:19 xia_fields-0.3.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      770 b- defN 23-May-04 19:19 xia_fields-0.3.8.dist-info/RECORD
-9 files, 1175437 bytes uncompressed, 459403 bytes compressed:  60.9%
+Zip file size: 460792 bytes, number of entries: 9
+-rw-r--r--  2.0 unx     1177 b- defN 23-May-25 06:09 xia_fields/__init__.py
+-rw-r--r--  2.0 unx   366080 b- defN 23-May-25 06:13 xia_fields/base.cp39-win_amd64.pyd
+-rw-r--r--  2.0 unx   415744 b- defN 23-May-25 06:14 xia_fields/fields.cp39-win_amd64.pyd
+-rw-r--r--  2.0 unx   388096 b- defN 23-May-25 06:15 xia_fields/fields_ext.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 unx      150 b- defN 23-May-25 06:15 xia_fields-0.3.9.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     3308 b- defN 23-May-25 06:15 xia_fields-0.3.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-May-25 06:15 xia_fields-0.3.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-May-25 06:15 xia_fields-0.3.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      770 b- defN 23-May-25 06:15 xia_fields-0.3.9.dist-info/RECORD
+9 files, 1175435 bytes uncompressed, 459466 bytes compressed:  60.9%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: xia_fields/fields.cp39-win_amd64.pyd
 Comment: 
 
 Filename: xia_fields/fields_ext.cp39-win_amd64.pyd
 Comment: 
 
-Filename: xia_fields-0.3.8.dist-info/LICENSE.txt
+Filename: xia_fields-0.3.9.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_fields-0.3.8.dist-info/METADATA
+Filename: xia_fields-0.3.9.dist-info/METADATA
 Comment: 
 
-Filename: xia_fields-0.3.8.dist-info/WHEEL
+Filename: xia_fields-0.3.9.dist-info/WHEEL
 Comment: 
 
-Filename: xia_fields-0.3.8.dist-info/top_level.txt
+Filename: xia_fields-0.3.9.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_fields-0.3.8.dist-info/RECORD
+Filename: xia_fields-0.3.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_fields/__init__.py

```diff
@@ -14,8 +14,8 @@
     "JsonField", "DictField", "CompressedStringField",
     "Int64Field", "Int32Field", "SFixed64Field", "SFixed32Field",
     "UInt64Field", "UInt32Field", "Fixed64Field", "Fixed32Field",
     "DoubleField", "DateField", "TimestampField", "TimeField", "DateTimeField",
     "OsEnvironField"
 ]
 
-__version__ = "0.3.8"
+__version__ = "0.3.9"
```

## Comparing `xia_fields-0.3.8.dist-info/METADATA` & `xia_fields-0.3.9.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xia-fields
-Version: 0.3.8
+Version: 0.3.9
 Summary: X-I-A Field Protocol
-Home-page: https://develop.x-i-a.com/docs/xia-fields/0.3.8/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-fields/0.3.9/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

