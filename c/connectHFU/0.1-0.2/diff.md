# Comparing `tmp/connectHFU-0.1-py3-none-any.whl.zip` & `tmp/connectHFU-0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,13 @@
-Zip file size: 1868 bytes, number of entries: 5
--rw-rw-rw-  2.0 fat     1095 b- defN 23-May-25 10:28 connectHFU-0.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      181 b- defN 23-May-25 10:28 connectHFU-0.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-25 10:28 connectHFU-0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        1 b- defN 23-May-25 10:28 connectHFU-0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      389 b- defN 23-May-25 10:28 connectHFU-0.1.dist-info/RECORD
-5 files, 1758 bytes uncompressed, 1138 bytes compressed:  35.3%
+Zip file size: 3830 bytes, number of entries: 11
+-rw-rw-rw-  2.0 fat        0 b- defN 23-May-24 10:44 connectHFU/__init__.py
+-rw-rw-rw-  2.0 fat       79 b- defN 23-May-24 10:50 connectHFU/client.py
+-rw-rw-rw-  2.0 fat     1048 b- defN 23-May-24 14:32 connectHFU/server.py
+-rw-rw-rw-  2.0 fat        0 b- defN 23-May-24 10:44 connectpy/__init__.py
+-rw-rw-rw-  2.0 fat       79 b- defN 23-May-24 10:50 connectpy/client.py
+-rw-rw-rw-  2.0 fat     1048 b- defN 23-May-24 14:32 connectpy/server.py
+-rw-rw-rw-  2.0 fat     1095 b- defN 23-May-25 11:28 connectHFU-0.2.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      181 b- defN 23-May-25 11:28 connectHFU-0.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-25 11:28 connectHFU-0.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       11 b- defN 23-May-25 11:28 connectHFU-0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      843 b- defN 23-May-25 11:28 connectHFU-0.2.dist-info/RECORD
+11 files, 4476 bytes uncompressed, 2402 bytes compressed:  46.3%
```

## zipnote {}

```diff
@@ -1,16 +1,34 @@
-Filename: connectHFU-0.1.dist-info/LICENSE
+Filename: connectHFU/__init__.py
 Comment: 
 
-Filename: connectHFU-0.1.dist-info/METADATA
+Filename: connectHFU/client.py
 Comment: 
 
-Filename: connectHFU-0.1.dist-info/WHEEL
+Filename: connectHFU/server.py
 Comment: 
 
-Filename: connectHFU-0.1.dist-info/top_level.txt
+Filename: connectpy/__init__.py
 Comment: 
 
-Filename: connectHFU-0.1.dist-info/RECORD
+Filename: connectpy/client.py
+Comment: 
+
+Filename: connectpy/server.py
+Comment: 
+
+Filename: connectHFU-0.2.dist-info/LICENSE
+Comment: 
+
+Filename: connectHFU-0.2.dist-info/METADATA
+Comment: 
+
+Filename: connectHFU-0.2.dist-info/WHEEL
+Comment: 
+
+Filename: connectHFU-0.2.dist-info/top_level.txt
+Comment: 
+
+Filename: connectHFU-0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `connectHFU-0.1.dist-info/LICENSE` & `connectHFU-0.2.dist-info/LICENSE`

 * *Files identical despite different names*

