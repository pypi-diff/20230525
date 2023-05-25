# Comparing `tmp/c7n_logexporter-0.4.8-py3-none-any.whl.zip` & `tmp/c7n_logexporter-0.4.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 13887 bytes, number of entries: 9
+Zip file size: 13902 bytes, number of entries: 9
 -rw-rw-r--  2.0 unx       79 b- defN 20-Nov-17 16:47 c7n_logexporter/__init__.py
 -rw-rw-r--  2.0 unx    31723 b- defN 20-Nov-17 16:47 c7n_logexporter/exporter.py
 -rw-rw-r--  2.0 unx     5303 b- defN 20-Nov-17 16:47 c7n_logexporter/flowdeliver.py
 -rw-rw-r--  2.0 unx     3146 b- defN 20-Nov-17 16:47 c7n_logexporter/stream.py
--rw-rw-r--  2.0 unx     2951 b- defN 20-Dec-14 16:37 c7n_logexporter-0.4.8.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 20-Dec-14 16:37 c7n_logexporter-0.4.8.dist-info/WHEEL
--rw-rw-r--  2.0 unx       67 b- defN 20-Dec-14 16:37 c7n_logexporter-0.4.8.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx       16 b- defN 20-Dec-14 16:37 c7n_logexporter-0.4.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      769 b- defN 20-Dec-14 16:37 c7n_logexporter-0.4.8.dist-info/RECORD
-9 files, 44146 bytes uncompressed, 12547 bytes compressed:  71.6%
+-rw-rw-r--  2.0 unx     2997 b- defN 21-Jan-11 16:55 c7n_logexporter-0.4.9.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 21-Jan-11 16:55 c7n_logexporter-0.4.9.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       67 b- defN 21-Jan-11 16:55 c7n_logexporter-0.4.9.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx       16 b- defN 21-Jan-11 16:55 c7n_logexporter-0.4.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      769 b- defN 21-Jan-11 16:55 c7n_logexporter-0.4.9.dist-info/RECORD
+9 files, 44192 bytes uncompressed, 12562 bytes compressed:  71.6%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: c7n_logexporter/flowdeliver.py
 Comment: 
 
 Filename: c7n_logexporter/stream.py
 Comment: 
 
-Filename: c7n_logexporter-0.4.8.dist-info/METADATA
+Filename: c7n_logexporter-0.4.9.dist-info/METADATA
 Comment: 
 
-Filename: c7n_logexporter-0.4.8.dist-info/WHEEL
+Filename: c7n_logexporter-0.4.9.dist-info/WHEEL
 Comment: 
 
-Filename: c7n_logexporter-0.4.8.dist-info/entry_points.txt
+Filename: c7n_logexporter-0.4.9.dist-info/entry_points.txt
 Comment: 
 
-Filename: c7n_logexporter-0.4.8.dist-info/top_level.txt
+Filename: c7n_logexporter-0.4.9.dist-info/top_level.txt
 Comment: 
 
-Filename: c7n_logexporter-0.4.8.dist-info/RECORD
+Filename: c7n_logexporter-0.4.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `c7n_logexporter-0.4.8.dist-info/METADATA` & `c7n_logexporter-0.4.9.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 Metadata-Version: 2.1
 Name: c7n-logexporter
-Version: 0.4.8
+Version: 0.4.9
 Summary: Cloud Custodian - Cloud Watch Log S3 exporter
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
-Requires-Dist: importlib-metadata (==1.7.0)
+Requires-Dist: boto3 (==1.16.42)
+Requires-Dist: botocore (==1.19.42)
+Requires-Dist: c7n (==0.9.10)
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
 
 # c7n-log-exporter: Cloud watch log exporter automation
 
 A small serverless app to archive cloud logs across accounts to an archive bucket. It utilizes
```

## Comparing `c7n_logexporter-0.4.8.dist-info/RECORD` & `c7n_logexporter-0.4.9.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 c7n_logexporter/__init__.py,sha256=R2mFrmBMYQznzGuzGQD6mqkcos4U9cix1uSQkh0m2lA,79
 c7n_logexporter/exporter.py,sha256=W1eBr8ubVjouhuzX2G99NbubHC98PXSMV1LHmDQOQO4,31723
 c7n_logexporter/flowdeliver.py,sha256=ZYOsyA0SBdcc3m-lpRhUistCltHA2fRwnH6iiSiWPpQ,5303
 c7n_logexporter/stream.py,sha256=vx8qjWc5GV7xLrDfZ5EdIaZPlO5QH3JODFjKvqg4X7s,3146
-c7n_logexporter-0.4.8.dist-info/METADATA,sha256=mi6evkUR9JwcXKqHMh_t_TqaDRxfgzGRBxhQ1QKED58,2951
-c7n_logexporter-0.4.8.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
-c7n_logexporter-0.4.8.dist-info/entry_points.txt,sha256=Rvk5ZhthueQBKIqiVWip_aBrtjbfCrjoplEp5nfeX2w,67
-c7n_logexporter-0.4.8.dist-info/top_level.txt,sha256=BHNU0s2E_UhsV50Gn7iz-4YNVSfg9ZZqzQ39QmPPxB8,16
-c7n_logexporter-0.4.8.dist-info/RECORD,,
+c7n_logexporter-0.4.9.dist-info/METADATA,sha256=PtIW7YyXMLce5YzoIk-jA_X_uaT3OUm_Dcx_e-nkfgs,2997
+c7n_logexporter-0.4.9.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
+c7n_logexporter-0.4.9.dist-info/entry_points.txt,sha256=Rvk5ZhthueQBKIqiVWip_aBrtjbfCrjoplEp5nfeX2w,67
+c7n_logexporter-0.4.9.dist-info/top_level.txt,sha256=BHNU0s2E_UhsV50Gn7iz-4YNVSfg9ZZqzQ39QmPPxB8,16
+c7n_logexporter-0.4.9.dist-info/RECORD,,
```

