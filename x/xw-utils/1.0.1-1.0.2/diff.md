# Comparing `tmp/xw_utils-1.0.1-cp39-cp39-win_amd64.whl.zip` & `tmp/xw_utils-1.0.2-cp39-cp39-musllinux_1_1_aarch64.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,12 @@
-Zip file size: 52773 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat   105984 b- defN 23-May-22 04:47 xw_utils.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat     2182 b- defN 23-May-22 04:47 xw_utils-1.0.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      296 b- defN 23-May-22 04:47 xw_utils-1.0.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-May-22 04:47 xw_utils-1.0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 23-May-22 04:47 xw_utils-1.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      476 b- defN 23-May-22 04:47 xw_utils-1.0.1.dist-info/RECORD
-6 files, 109047 bytes uncompressed, 51913 bytes compressed:  52.4%
+Zip file size: 600229 bytes, number of entries: 10
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-25 04:16 xw_utils-1.0.2.dist-info/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-25 04:16 xw_utils.libs/
+-rwxr-xr-x  2.0 unx   268809 b- defN 23-May-25 04:16 xw_utils.cpython-39-aarch64-linux-gnu.so
+-rw-rw-r--  2.0 unx      694 b- defN 23-May-25 04:16 xw_utils-1.0.2.dist-info/RECORD
+-rw-r--r--  2.0 unx        9 b- defN 23-May-25 04:16 xw_utils-1.0.2.dist-info/top_level.txt
+-rw-r--r--  2.0 unx      283 b- defN 23-May-25 04:16 xw_utils-1.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx      112 b- defN 23-May-25 04:16 xw_utils-1.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx     2182 b- defN 23-May-25 04:16 xw_utils-1.0.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx   134393 b- defN 23-May-25 04:16 xw_utils.libs/libgcc_s-4e37474d.so.1
+-rwxr-xr-x  2.0 unx  2599041 b- defN 23-May-25 04:16 xw_utils.libs/libstdc++-fd9f4683.so.6.0.28
+10 files, 3005523 bytes uncompressed, 598805 bytes compressed:  80.1%
```

## zipnote {}

```diff
@@ -1,19 +1,31 @@
-Filename: xw_utils.cp39-win_amd64.pyd
+Filename: xw_utils-1.0.2.dist-info/
 Comment: 
 
-Filename: xw_utils-1.0.1.dist-info/LICENSE
+Filename: xw_utils.libs/
 Comment: 
 
-Filename: xw_utils-1.0.1.dist-info/METADATA
+Filename: xw_utils.cpython-39-aarch64-linux-gnu.so
 Comment: 
 
-Filename: xw_utils-1.0.1.dist-info/WHEEL
+Filename: xw_utils-1.0.2.dist-info/RECORD
 Comment: 
 
-Filename: xw_utils-1.0.1.dist-info/top_level.txt
+Filename: xw_utils-1.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: xw_utils-1.0.1.dist-info/RECORD
+Filename: xw_utils-1.0.2.dist-info/METADATA
+Comment: 
+
+Filename: xw_utils-1.0.2.dist-info/WHEEL
+Comment: 
+
+Filename: xw_utils-1.0.2.dist-info/LICENSE
+Comment: 
+
+Filename: xw_utils.libs/libgcc_s-4e37474d.so.1
+Comment: 
+
+Filename: xw_utils.libs/libstdc++-fd9f4683.so.6.0.28
 Comment: 
 
 Zip file comment:
```

## filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=deflate
+Zip archive data, at least v2.0 to extract, compression method=store
```

## Comparing `xw_utils-1.0.1.dist-info/LICENSE` & `xw_utils-1.0.2.dist-info/LICENSE`

 * *Files identical despite different names*

