# Comparing `tmp/miscSupports-0.9.0-py3-none-any.whl.zip` & `tmp/miscSupports-0.9.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 15001 bytes, number of entries: 15
+Zip file size: 15061 bytes, number of entries: 15
 -rw-rw-rw-  2.0 fat     1176 b- defN 21-Aug-02 14:06 miscSupports/Errors.py
 -rw-rw-rw-  2.0 fat     1107 b- defN 21-Jun-18 12:38 miscSupports/ShellMaker.py
 -rw-rw-rw-  2.0 fat      319 b- defN 21-Aug-02 14:08 miscSupports/__init__.py
 -rw-rw-rw-  2.0 fat    11237 b- defN 21-Aug-02 14:03 miscSupports/alter_array.py
 -rw-rw-rw-  2.0 fat     1682 b- defN 21-Aug-02 14:06 miscSupports/alter_string.py
 -rw-rw-rw-  2.0 fat     2748 b- defN 21-May-10 19:04 miscSupports/byte_supports.py
 -rw-rw-rw-  2.0 fat     3972 b- defN 21-Aug-02 13:59 miscSupports/dates_and_time.py
--rw-rw-rw-  2.0 fat     6424 b- defN 21-Jun-02 09:32 miscSupports/file_support.py
+-rw-rw-rw-  2.0 fat     6656 b- defN 21-Aug-04 16:10 miscSupports/file_support.py
 -rw-rw-rw-  2.0 fat     1826 b- defN 21-Aug-02 14:03 miscSupports/misc.py
 -rw-rw-rw-  2.0 fat     1210 b- defN 21-Jan-12 10:08 miscSupports/shapely_support.py
--rw-rw-rw-  2.0 fat     1090 b- defN 21-Aug-02 14:10 miscSupports-0.9.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      795 b- defN 21-Aug-02 14:10 miscSupports-0.9.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       97 b- defN 21-Aug-02 14:10 miscSupports-0.9.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       13 b- defN 21-Aug-02 14:10 miscSupports-0.9.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1245 b- defN 21-Aug-02 14:10 miscSupports-0.9.0.dist-info/RECORD
-15 files, 34941 bytes uncompressed, 12941 bytes compressed:  63.0%
+-rw-rw-rw-  2.0 fat     1090 b- defN 21-Aug-04 16:10 miscSupports-0.9.1.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      795 b- defN 21-Aug-04 16:10 miscSupports-0.9.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       97 b- defN 21-Aug-04 16:10 miscSupports-0.9.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       13 b- defN 21-Aug-04 16:10 miscSupports-0.9.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1245 b- defN 21-Aug-04 16:10 miscSupports-0.9.1.dist-info/RECORD
+15 files, 35173 bytes uncompressed, 13001 bytes compressed:  63.0%
```

## zipnote {}

```diff
@@ -24,23 +24,23 @@
 
 Filename: miscSupports/misc.py
 Comment: 
 
 Filename: miscSupports/shapely_support.py
 Comment: 
 
-Filename: miscSupports-0.9.0.dist-info/LICENSE
+Filename: miscSupports-0.9.1.dist-info/LICENSE
 Comment: 
 
-Filename: miscSupports-0.9.0.dist-info/METADATA
+Filename: miscSupports-0.9.1.dist-info/METADATA
 Comment: 
 
-Filename: miscSupports-0.9.0.dist-info/WHEEL
+Filename: miscSupports-0.9.1.dist-info/WHEEL
 Comment: 
 
-Filename: miscSupports-0.9.0.dist-info/top_level.txt
+Filename: miscSupports-0.9.1.dist-info/top_level.txt
 Comment: 
 
-Filename: miscSupports-0.9.0.dist-info/RECORD
+Filename: miscSupports-0.9.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## miscSupports/file_support.py

```diff
@@ -84,14 +84,21 @@
 
 def write_pickle(directory, file_name, data):
     """Write Pickle Data"""
     with open(Path(directory, file_name), 'wb') as handle:
         pickle.dump(data, handle, protocol=pickle.HIGHEST_PROTOCOL)
 
 
+def write_markdown(directory, file_name, lines_to_write):
+    """Write MarkDown File"""
+    with open(Path(directory, f"{file_name}.md"), "w") as outfile:
+        for line in lines_to_write:
+            outfile.write(line)
+
+
 def extract_headers(path):
     """
     Extract the first row from the file and return it as a list
     """
     with open(path) as header_extract:
         csv_data = csv.reader(header_extract)
         for row in csv_data:
```

## Comparing `miscSupports-0.9.0.dist-info/LICENSE` & `miscSupports-0.9.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `miscSupports-0.9.0.dist-info/METADATA` & `miscSupports-0.9.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miscSupports
-Version: 0.9.0
+Version: 0.9.1
 Summary: Supporting common methods for multiple packages and repositories I have written
 Home-page: UNKNOWN
 Author: Samuel Baker
 Author-email: samuelbaker.researcher@gmail.com
 Maintainer: Samuel Baker
 Maintainer-email: samuelbaker.researcher@gmail.com
 License: MIT
```

## Comparing `miscSupports-0.9.0.dist-info/RECORD` & `miscSupports-0.9.1.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 miscSupports/Errors.py,sha256=BYPKaQCVqhQ738PiLNFNZFCmSDtfVmiytgRGqTH0xEs,1176
 miscSupports/ShellMaker.py,sha256=V6qUsM-iteENxFxuYS-AtAaboW6xJQM7FwPoOAh_6sY,1107
 miscSupports/__init__.py,sha256=iMSRrmtPDb0-CT1yrfcXLnwjVEIaBmo0k5dmu90VjJY,319
 miscSupports/alter_array.py,sha256=F7vZco_AjeWbJX7zYbamCN3MTPgE87mVnAKXRpxKRsU,11237
 miscSupports/alter_string.py,sha256=b7IFIxu8LN6f3SQ0CkbaLKGB9bHOe0ZEAOi3vOL04qo,1682
 miscSupports/byte_supports.py,sha256=jUD0nvWka0qFuIJtPi6LfsSG_7giFUYPfvfDwJe9JgU,2748
 miscSupports/dates_and_time.py,sha256=eODTVYhSEG1Dnv07xKxeykHDt3wgPRVdveoyPV3D0nc,3972
-miscSupports/file_support.py,sha256=oSOCUwtASdosVN7kMFmQVvKc3Kd905OnXnzzpQhcri0,6424
+miscSupports/file_support.py,sha256=XDO_F0sv49wzrgp6Bg95zNXPgVAvdva1Yytcgknv2zg,6656
 miscSupports/misc.py,sha256=iYqWG7CZooFDYfsKfJQu4TD0WhNsIRDUUtp_JpYnobU,1826
 miscSupports/shapely_support.py,sha256=mpYJF9USdfDhmFMAcZZfOckpVd0a2ads9buJTkySp-0,1210
-miscSupports-0.9.0.dist-info/LICENSE,sha256=m6Hmim3NNA-_y97X6yarvaf6IUerwLQFF3hlCXsc0KI,1090
-miscSupports-0.9.0.dist-info/METADATA,sha256=8StHtxQP-eVIbauLlZrAodUK6R0fVCUfjSdQKueTk90,795
-miscSupports-0.9.0.dist-info/WHEEL,sha256=D1Wh14kWDxPnrM-5t_6UCB-UuQNrEODtRa3vF4OsvQY,97
-miscSupports-0.9.0.dist-info/top_level.txt,sha256=SkyJWNczNshZ7W_O7QO7jvaUJbnBhaN-P0HeWOkl7ts,13
-miscSupports-0.9.0.dist-info/RECORD,,
+miscSupports-0.9.1.dist-info/LICENSE,sha256=m6Hmim3NNA-_y97X6yarvaf6IUerwLQFF3hlCXsc0KI,1090
+miscSupports-0.9.1.dist-info/METADATA,sha256=rFuVhlLyQWIPuhdd2BTE_hGixfapDXhac0SINnxzrzI,795
+miscSupports-0.9.1.dist-info/WHEEL,sha256=D1Wh14kWDxPnrM-5t_6UCB-UuQNrEODtRa3vF4OsvQY,97
+miscSupports-0.9.1.dist-info/top_level.txt,sha256=SkyJWNczNshZ7W_O7QO7jvaUJbnBhaN-P0HeWOkl7ts,13
+miscSupports-0.9.1.dist-info/RECORD,,
```

