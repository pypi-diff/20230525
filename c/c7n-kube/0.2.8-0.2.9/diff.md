# Comparing `tmp/c7n_kube-0.2.8-py3-none-any.whl.zip` & `tmp/c7n_kube-0.2.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 16501 bytes, number of entries: 32
+Zip file size: 16525 bytes, number of entries: 32
 -rw-rw-r--  2.0 unx       79 b- defN 20-Nov-17 16:47 c7n_kube/__init__.py
 -rw-rw-r--  2.0 unx     1460 b- defN 20-Nov-17 16:47 c7n_kube/client.py
 -rw-rw-r--  2.0 unx      765 b- defN 20-Nov-17 16:47 c7n_kube/entry.py
 -rw-rw-r--  2.0 unx      110 b- defN 20-Nov-17 16:47 c7n_kube/filters.py
 -rw-rw-r--  2.0 unx      829 b- defN 20-Nov-17 16:47 c7n_kube/provider.py
 -rw-rw-r--  2.0 unx     4662 b- defN 20-Nov-17 16:47 c7n_kube/query.py
 -rw-rw-r--  2.0 unx       79 b- defN 20-Nov-17 16:47 c7n_kube/actions/__init__.py
@@ -23,12 +23,12 @@
 -rw-rw-r--  2.0 unx      461 b- defN 20-Nov-17 16:47 c7n_kube/resources/core/node.py
 -rw-rw-r--  2.0 unx      470 b- defN 20-Nov-17 16:47 c7n_kube/resources/core/pod.py
 -rw-rw-r--  2.0 unx      564 b- defN 20-Nov-17 16:47 c7n_kube/resources/core/replicationcontroller.py
 -rw-rw-r--  2.0 unx      485 b- defN 20-Nov-17 16:47 c7n_kube/resources/core/secret.py
 -rw-rw-r--  2.0 unx      489 b- defN 20-Nov-17 16:47 c7n_kube/resources/core/service.py
 -rw-rw-r--  2.0 unx      528 b- defN 20-Nov-17 16:47 c7n_kube/resources/core/serviceaccount.py
 -rw-rw-r--  2.0 unx      890 b- defN 20-Nov-17 16:47 c7n_kube/resources/core/volume.py
--rw-rw-r--  2.0 unx     2607 b- defN 20-Dec-14 16:37 c7n_kube-0.2.8.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 20-Dec-14 16:37 c7n_kube-0.2.8.dist-info/WHEEL
--rw-rw-r--  2.0 unx        9 b- defN 20-Dec-14 16:37 c7n_kube-0.2.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     2714 b- defN 20-Dec-14 16:37 c7n_kube-0.2.8.dist-info/RECORD
-32 files, 30043 bytes uncompressed, 12095 bytes compressed:  59.7%
+-rw-rw-r--  2.0 unx     2747 b- defN 21-Jan-11 16:55 c7n_kube-0.2.9.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 21-Jan-11 16:55 c7n_kube-0.2.9.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        9 b- defN 21-Jan-11 16:55 c7n_kube-0.2.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     2714 b- defN 21-Jan-11 16:55 c7n_kube-0.2.9.dist-info/RECORD
+32 files, 30183 bytes uncompressed, 12119 bytes compressed:  59.8%
```

## zipnote {}

```diff
@@ -78,20 +78,20 @@
 
 Filename: c7n_kube/resources/core/serviceaccount.py
 Comment: 
 
 Filename: c7n_kube/resources/core/volume.py
 Comment: 
 
-Filename: c7n_kube-0.2.8.dist-info/METADATA
+Filename: c7n_kube-0.2.9.dist-info/METADATA
 Comment: 
 
-Filename: c7n_kube-0.2.8.dist-info/WHEEL
+Filename: c7n_kube-0.2.9.dist-info/WHEEL
 Comment: 
 
-Filename: c7n_kube-0.2.8.dist-info/top_level.txt
+Filename: c7n_kube-0.2.9.dist-info/top_level.txt
 Comment: 
 
-Filename: c7n_kube-0.2.8.dist-info/RECORD
+Filename: c7n_kube-0.2.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `c7n_kube-0.2.8.dist-info/METADATA` & `c7n_kube-0.2.9.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,51 +1,52 @@
 Metadata-Version: 2.1
 Name: c7n-kube
-Version: 0.2.8
+Version: 0.2.9
 Summary: Cloud Custodian - Kubernetes Provider
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
+Requires-Dist: boto3 (==1.16.42)
+Requires-Dist: botocore (==1.19.42)
+Requires-Dist: c7n (==0.9.10)
 Requires-Dist: certifi (==2020.12.5)
-Requires-Dist: chardet (==3.0.4)
-Requires-Dist: importlib-metadata (==1.7.0)
+Requires-Dist: importlib-metadata (==3.3.0)
 Requires-Dist: jmespath (==0.10.0)
 Requires-Dist: jsonpickle (==1.3)
 Requires-Dist: jsonschema (==3.2.0)
 Requires-Dist: kubernetes (==10.0.1)
 Requires-Dist: pyasn1-modules (==0.2.8)
 Requires-Dist: pyasn1 (==0.4.8)
 Requires-Dist: pyrsistent (==0.17.3)
 Requires-Dist: python-dateutil (==2.8.1)
 Requires-Dist: pyyaml (==5.3.1)
 Requires-Dist: s3transfer (==0.3.3)
 Requires-Dist: six (==1.15.0)
 Requires-Dist: tabulate (==0.8.7)
+Requires-Dist: typing-extensions (==3.7.4.3)
 Requires-Dist: urllib3 (==1.26.2)
 Requires-Dist: zipp (==3.4.0)
 Requires-Dist: websocket-client (==0.57.0) ; python_version >= "2.6" and python_full_version < "3.0.0" or python_full_version >= "3.4.0"
 Requires-Dist: python-dateutil (==2.8.1) ; python_version >= "2.7" and python_full_version < "3.0.0" or python_full_version >= "3.3.0"
 Requires-Dist: six (==1.15.0) ; python_version >= "2.7" and python_full_version < "3.0.0" or python_full_version >= "3.3.0"
-Requires-Dist: google-auth (==1.23.0) ; python_version >= "2.7" and python_full_version < "3.0.0" or python_full_version >= "3.4.0"
 Requires-Dist: idna (==2.10) ; python_version >= "2.7" and python_full_version < "3.0.0" or python_full_version >= "3.4.0"
 Requires-Dist: oauthlib (==3.1.0) ; python_version >= "2.7" and python_full_version < "3.0.0" or python_full_version >= "3.4.0"
 Requires-Dist: requests-oauthlib (==1.3.0) ; python_version >= "2.7" and python_full_version < "3.0.0" or python_full_version >= "3.4.0"
+Requires-Dist: chardet (==4.0.0) ; python_version >= "2.7" and python_full_version < "3.0.0" or python_full_version >= "3.5.0"
 Requires-Dist: pyyaml (==5.3.1) ; python_version >= "2.7" and python_full_version < "3.0.0" or python_full_version >= "3.5.0"
-Requires-Dist: requests (==2.25.0) ; python_version >= "2.7" and python_full_version < "3.0.0" or python_full_version >= "3.5.0"
+Requires-Dist: requests (==2.25.1) ; python_version >= "2.7" and python_full_version < "3.0.0" or python_full_version >= "3.5.0"
 Requires-Dist: urllib3 (==1.26.2) ; python_version >= "2.7" and python_full_version < "3.0.0" or python_full_version >= "3.5.0" and python_version < "4"
+Requires-Dist: google-auth (==1.24.0) ; python_version >= "2.7" and python_full_version < "3.0.0" or python_full_version >= "3.6.0"
 Requires-Dist: rsa (==4.6) ; python_version >= "3.5" and python_version < "4"
-Requires-Dist: cachetools (==4.1.1) ; python_version >= "3.5" and python_version < "4.0"
+Requires-Dist: cachetools (==4.2.0) ; python_version >= "3.5" and python_version < "4.0"
 
 # Custodian Kubernetes Support
 
 
 Work in Progress - Not Ready For Use.
```

## Comparing `c7n_kube-0.2.8.dist-info/RECORD` & `c7n_kube-0.2.9.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -22,11 +22,11 @@
 c7n_kube/resources/core/node.py,sha256=HKSK7NWbRSsN_wvNA6tcMH2URgjuQsp-GmEFO3rrFaw,461
 c7n_kube/resources/core/pod.py,sha256=ha5KxLhlJ_yNO60Kgfg2SmRe_ufeRRqD5irnU9qTtvA,470
 c7n_kube/resources/core/replicationcontroller.py,sha256=74xwi7IpP3uSqXEfoJNVv4a402VyJ2PhfNQZ25wUcSg,564
 c7n_kube/resources/core/secret.py,sha256=VqTKEzixJi0qzAYbQx049ywwK6Cg7fSJOj8qqbmib30,485
 c7n_kube/resources/core/service.py,sha256=St9dF4czBuh_K8BjO9kBphbKpbzmmTGTuBwHHHgDS4M,489
 c7n_kube/resources/core/serviceaccount.py,sha256=bPn9dtAm_mpbAmQiZi3c7c90yFhzwCBoQFkDarrkP1c,528
 c7n_kube/resources/core/volume.py,sha256=qjO-7JWKTwC3_gBNDh_GsQwDE_h82adtRMvTbanGLHw,890
-c7n_kube-0.2.8.dist-info/METADATA,sha256=19awLv-xrcxhs1Xdju1L4C6nieWo5mh-yE068s0POF8,2607
-c7n_kube-0.2.8.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
-c7n_kube-0.2.8.dist-info/top_level.txt,sha256=X2YyvcJ6AgIBExnusNXfUywTM3Uo-KsNUciYDIH_iFY,9
-c7n_kube-0.2.8.dist-info/RECORD,,
+c7n_kube-0.2.9.dist-info/METADATA,sha256=qMtsxCm680JT2OHIjMdSSuDYWgE-gL8wRh3nPl6Wjgc,2747
+c7n_kube-0.2.9.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
+c7n_kube-0.2.9.dist-info/top_level.txt,sha256=X2YyvcJ6AgIBExnusNXfUywTM3Uo-KsNUciYDIH_iFY,9
+c7n_kube-0.2.9.dist-info/RECORD,,
```

