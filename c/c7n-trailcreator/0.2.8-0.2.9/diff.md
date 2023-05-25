# Comparing `tmp/c7n_trailcreator-0.2.8-py3-none-any.whl.zip` & `tmp/c7n_trailcreator-0.2.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 11739 bytes, number of entries: 7
+Zip file size: 11755 bytes, number of entries: 7
 -rw-rw-r--  2.0 unx      129 b- defN 20-Sep-08 15:42 c7n_trailcreator/__init__.py
 -rw-rw-r--  2.0 unx    29244 b- defN 20-Nov-17 16:47 c7n_trailcreator/trailcreator.py
--rw-rw-r--  2.0 unx     5526 b- defN 20-Dec-14 16:37 c7n_trailcreator-0.2.8.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 20-Dec-14 16:37 c7n_trailcreator-0.2.8.dist-info/WHEEL
--rw-rw-r--  2.0 unx       72 b- defN 20-Dec-14 16:37 c7n_trailcreator-0.2.8.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx       17 b- defN 20-Dec-14 16:37 c7n_trailcreator-0.2.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      612 b- defN 20-Dec-14 16:37 c7n_trailcreator-0.2.8.dist-info/RECORD
-7 files, 35692 bytes uncompressed, 10639 bytes compressed:  70.2%
+-rw-rw-r--  2.0 unx     5572 b- defN 21-Jan-11 16:55 c7n_trailcreator-0.2.9.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 21-Jan-11 16:55 c7n_trailcreator-0.2.9.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       72 b- defN 21-Jan-11 16:55 c7n_trailcreator-0.2.9.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx       17 b- defN 21-Jan-11 16:55 c7n_trailcreator-0.2.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      612 b- defN 21-Jan-11 16:55 c7n_trailcreator-0.2.9.dist-info/RECORD
+7 files, 35738 bytes uncompressed, 10655 bytes compressed:  70.2%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: c7n_trailcreator/__init__.py
 Comment: 
 
 Filename: c7n_trailcreator/trailcreator.py
 Comment: 
 
-Filename: c7n_trailcreator-0.2.8.dist-info/METADATA
+Filename: c7n_trailcreator-0.2.9.dist-info/METADATA
 Comment: 
 
-Filename: c7n_trailcreator-0.2.8.dist-info/WHEEL
+Filename: c7n_trailcreator-0.2.9.dist-info/WHEEL
 Comment: 
 
-Filename: c7n_trailcreator-0.2.8.dist-info/entry_points.txt
+Filename: c7n_trailcreator-0.2.9.dist-info/entry_points.txt
 Comment: 
 
-Filename: c7n_trailcreator-0.2.8.dist-info/top_level.txt
+Filename: c7n_trailcreator-0.2.9.dist-info/top_level.txt
 Comment: 
 
-Filename: c7n_trailcreator-0.2.8.dist-info/RECORD
+Filename: c7n_trailcreator-0.2.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `c7n_trailcreator-0.2.8.dist-info/METADATA` & `c7n_trailcreator-0.2.9.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 Metadata-Version: 2.1
 Name: c7n-trailcreator
-Version: 0.2.8
+Version: 0.2.9
 Summary: Cloud Custodian - Retroactive Tag Resource Creators from CloudTrail
 Home-page: https://cloudcustodian.io
 Author: Cloud Custodian Project
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.6,<4.0
 Description-Content-Type: text/markdown
 Requires-Dist: argcomplete (==1.12.2)
 Requires-Dist: attrs (==20.3.0)
-Requires-Dist: boto3 (==1.16.32)
-Requires-Dist: botocore (==1.19.32)
-Requires-Dist: c7n (==0.9.8)
-Requires-Dist: c7n-org (==0.6.7)
+Requires-Dist: boto3 (==1.16.42)
+Requires-Dist: botocore (==1.19.42)
+Requires-Dist: c7n (==0.9.10)
+Requires-Dist: c7n-org (==0.6.9)
 Requires-Dist: click (==7.1.2)
-Requires-Dist: importlib-metadata (==1.7.0)
+Requires-Dist: importlib-metadata (==3.3.0)
 Requires-Dist: jmespath (==0.10.0)
 Requires-Dist: jsonpickle (==1.3)
 Requires-Dist: jsonschema (==3.2.0)
 Requires-Dist: pyrsistent (==0.17.3)
 Requires-Dist: python-dateutil (==2.8.1)
 Requires-Dist: pyyaml (==5.3.1)
 Requires-Dist: s3transfer (==0.3.3)
 Requires-Dist: six (==1.15.0)
 Requires-Dist: tabulate (==0.8.7)
+Requires-Dist: typing-extensions (==3.7.4.3)
 Requires-Dist: urllib3 (==1.26.2)
 Requires-Dist: zipp (==3.4.0)
 Requires-Dist: click (==7.1.2) ; python_version >= "2.7" and python_full_version < "3.0.0" or python_full_version >= "3.5.0"
 
 # c7n-trailcreator:  Retroactive Resource Creator Tagging
 
 This script will process cloudtrail records to create a sqlite db of
```

