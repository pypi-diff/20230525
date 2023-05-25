# Comparing `tmp/c7n_mailer-0.6.8-py3-none-any.whl.zip` & `tmp/c7n_mailer-0.6.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 54280 bytes, number of entries: 30
+Zip file size: 54299 bytes, number of entries: 30
 -rw-rw-r--  2.0 unx       79 b- defN 20-Nov-17 16:47 c7n_mailer/__init__.py
 -rw-rw-r--  2.0 unx    10356 b- defN 20-Dec-14 15:57 c7n_mailer/cli.py
 -rw-rw-r--  2.0 unx     3937 b- defN 20-Nov-17 16:47 c7n_mailer/datadog_delivery.py
 -rw-rw-r--  2.0 unx     2894 b- defN 20-Nov-17 16:47 c7n_mailer/deploy.py
 -rw-rw-r--  2.0 unx    11577 b- defN 20-Nov-17 16:47 c7n_mailer/email_delivery.py
 -rw-rw-r--  2.0 unx     1151 b- defN 20-Nov-17 16:47 c7n_mailer/handle.py
 -rw-rw-r--  2.0 unx     8540 b- defN 20-Nov-17 16:47 c7n_mailer/ldap_lookup.py
@@ -20,13 +20,13 @@
 -rw-rw-r--  2.0 unx      613 b- defN 20-Nov-17 16:47 c7n_mailer/azure_mailer/function.py
 -rw-rw-r--  2.0 unx      735 b- defN 20-Nov-17 16:47 c7n_mailer/azure_mailer/handle.py
 -rw-rw-r--  2.0 unx     5701 b- defN 20-Nov-17 16:47 c7n_mailer/azure_mailer/sendgrid_delivery.py
 -rw-rw-r--  2.0 unx      627 b- defN 20-Nov-17 16:47 c7n_mailer/azure_mailer/utils.py
 -rw-rw-r--  2.0 unx    10038 b- defN 20-Nov-17 16:47 c7n_mailer/msg-templates/default.html.j2
 -rw-rw-r--  2.0 unx      245 b- defN 20-Sep-08 15:42 c7n_mailer/msg-templates/default.j2
 -rw-rw-r--  2.0 unx     1103 b- defN 20-Sep-08 15:42 c7n_mailer/msg-templates/slack_default.j2
--rw-rw-r--  2.0 unx    42724 b- defN 20-Dec-14 16:37 c7n_mailer-0.6.8.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 20-Dec-14 16:37 c7n_mailer-0.6.8.dist-info/WHEEL
--rw-rw-r--  2.0 unx       95 b- defN 20-Dec-14 16:37 c7n_mailer-0.6.8.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx       11 b- defN 20-Dec-14 16:37 c7n_mailer-0.6.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     2575 b- defN 20-Dec-14 16:37 c7n_mailer-0.6.8.dist-info/RECORD
-30 files, 174474 bytes uncompressed, 50122 bytes compressed:  71.3%
+-rw-rw-r--  2.0 unx    42863 b- defN 21-Jan-11 16:55 c7n_mailer-0.6.9.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 21-Jan-11 16:55 c7n_mailer-0.6.9.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       95 b- defN 21-Jan-11 16:55 c7n_mailer-0.6.9.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx       11 b- defN 21-Jan-11 16:55 c7n_mailer-0.6.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     2575 b- defN 21-Jan-11 16:55 c7n_mailer-0.6.9.dist-info/RECORD
+30 files, 174613 bytes uncompressed, 50141 bytes compressed:  71.3%
```

## zipnote {}

```diff
@@ -69,23 +69,23 @@
 
 Filename: c7n_mailer/msg-templates/default.j2
 Comment: 
 
 Filename: c7n_mailer/msg-templates/slack_default.j2
 Comment: 
 
-Filename: c7n_mailer-0.6.8.dist-info/METADATA
+Filename: c7n_mailer-0.6.9.dist-info/METADATA
 Comment: 
 
-Filename: c7n_mailer-0.6.8.dist-info/WHEEL
+Filename: c7n_mailer-0.6.9.dist-info/WHEEL
 Comment: 
 
-Filename: c7n_mailer-0.6.8.dist-info/entry_points.txt
+Filename: c7n_mailer-0.6.9.dist-info/entry_points.txt
 Comment: 
 
-Filename: c7n_mailer-0.6.8.dist-info/top_level.txt
+Filename: c7n_mailer-0.6.9.dist-info/top_level.txt
 Comment: 
 
-Filename: c7n_mailer-0.6.8.dist-info/RECORD
+Filename: c7n_mailer-0.6.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `c7n_mailer-0.6.8.dist-info/METADATA` & `c7n_mailer-0.6.9.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,45 +1,46 @@
 Metadata-Version: 2.1
 Name: c7n-mailer
-Version: 0.6.8
+Version: 0.6.9
 Summary: Cloud Custodian - Reference Mailer
 Home-page: https://cloudcustodian.io
 Author: Cloud Custodian Project
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.6,<4.0
 Description-Content-Type: text/markdown
-Requires-Dist: boto3 (==1.16.32)
-Requires-Dist: botocore (==1.19.32)
+Requires-Dist: boto3 (==1.16.42)
+Requires-Dist: botocore (==1.19.42)
 Requires-Dist: certifi (==2020.12.5)
-Requires-Dist: chardet (==3.0.4)
 Requires-Dist: datadog (==0.34.1)
 Requires-Dist: jsonschema (==3.2.0)
 Requires-Dist: ldap3 (==2.8.1)
 Requires-Dist: pyasn1 (==0.4.8)
 Requires-Dist: s3transfer (==0.3.3)
 Requires-Dist: starkbank-ecdsa (==1.1.0)
+Requires-Dist: typing-extensions (==3.7.4.3)
 Requires-Dist: decorator (==4.4.2) ; python_version >= "2.6" and python_full_version < "3.0.0" or python_full_version >= "3.2.0"
 Requires-Dist: jmespath (==0.10.0) ; python_version >= "2.6" and python_full_version < "3.0.0" or python_full_version >= "3.3.0"
 Requires-Dist: python-dateutil (==2.8.1) ; python_version >= "2.7" and python_full_version < "3.0.0" or python_full_version >= "3.3.0"
 Requires-Dist: six (==1.15.0) ; python_version >= "2.7" and python_full_version < "3.0.0" or python_full_version >= "3.3.0"
 Requires-Dist: attrs (==20.3.0) ; python_version >= "2.7" and python_full_version < "3.0.0" or python_full_version >= "3.4.0"
 Requires-Dist: idna (==2.10) ; python_version >= "2.7" and python_full_version < "3.0.0" or python_full_version >= "3.4.0"
 Requires-Dist: jsonpointer (==2.0) ; python_version >= "2.7" and python_full_version < "3.0.0" or python_full_version >= "3.4.0"
 Requires-Dist: markupsafe (==1.1.1) ; python_version >= "2.7" and python_full_version < "3.0.0" or python_full_version >= "3.4.0"
 Requires-Dist: python-http-client (==3.3.1) ; python_version >= "2.7" and python_full_version < "3.0.0" or python_full_version >= "3.4.0"
+Requires-Dist: chardet (==4.0.0) ; python_version >= "2.7" and python_full_version < "3.0.0" or python_full_version >= "3.5.0"
 Requires-Dist: jinja2 (==2.11.2) ; python_version >= "2.7" and python_full_version < "3.0.0" or python_full_version >= "3.5.0"
 Requires-Dist: jsonpatch (==1.28) ; python_version >= "2.7" and python_full_version < "3.0.0" or python_full_version >= "3.5.0"
 Requires-Dist: pyyaml (==5.3.1) ; python_version >= "2.7" and python_full_version < "3.0.0" or python_full_version >= "3.5.0"
 Requires-Dist: redis (==3.5.3) ; python_version >= "2.7" and python_full_version < "3.0.0" or python_full_version >= "3.5.0"
-Requires-Dist: requests (==2.25.0) ; python_version >= "2.7" and python_full_version < "3.0.0" or python_full_version >= "3.5.0"
+Requires-Dist: requests (==2.25.1) ; python_version >= "2.7" and python_full_version < "3.0.0" or python_full_version >= "3.5.0"
 Requires-Dist: sendgrid (==6.4.8) ; python_version >= "2.7" and python_full_version < "3.0.0" or python_full_version >= "3.5.0"
 Requires-Dist: urllib3 (==1.26.2) ; python_version >= "2.7" and python_full_version < "3.0.0" or python_full_version >= "3.5.0" and python_version < "4"
 Requires-Dist: pyrsistent (==0.17.3) ; python_version >= "3.5"
-Requires-Dist: importlib-metadata (==3.1.1) ; python_version >= "3.6"
+Requires-Dist: importlib-metadata (==3.3.0) ; python_version >= "3.6"
 Requires-Dist: zipp (==3.4.0) ; python_version >= "3.6"
 
 # c7n-mailer: Custodian Mailer
 
 [//]: # (         !!! IMPORTANT !!!                    )
 [//]: # (This file is moved during document generation.)
 [//]: # (Only edit the original document at ./tools/c7n_mailer/README.md)
```

## Comparing `c7n_mailer-0.6.8.dist-info/RECORD` & `c7n_mailer-0.6.9.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -19,12 +19,12 @@
 c7n_mailer/azure_mailer/function.py,sha256=VzalrCKQ0pKviZuSu4VzDtseZHgYNrhoXjTiiYneoWk,613
 c7n_mailer/azure_mailer/handle.py,sha256=lDx0EDCE-DZZ_JyL02v5sVCA0JWz_vO0qMf3bJgG9So,735
 c7n_mailer/azure_mailer/sendgrid_delivery.py,sha256=tBSdCyJ6V_eyctSd4oSrX3LiJU6VrW_n5cCRfIwlzDE,5701
 c7n_mailer/azure_mailer/utils.py,sha256=20WJs48MGms-PQP3UaEr55zGor-vJZhLtAArm-oXruI,627
 c7n_mailer/msg-templates/default.html.j2,sha256=s85ngJl69bZ7a3XUdYwuUqzMgnSeQfgTGt5ZrJrp2_0,10038
 c7n_mailer/msg-templates/default.j2,sha256=RJ1v5qm_zL9vUGGG1IuoABVZNXdFihcxi6O2cPthxXw,245
 c7n_mailer/msg-templates/slack_default.j2,sha256=uXUnE65XNmGEzZbeE9L3Tp5sjUwjo1ZPQUasiXXI-aY,1103
-c7n_mailer-0.6.8.dist-info/METADATA,sha256=taJTzE6hFaSqM_8xIDpMR3DLcvlEhAOTYbbJHonrhGw,42724
-c7n_mailer-0.6.8.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
-c7n_mailer-0.6.8.dist-info/entry_points.txt,sha256=WjuO0T_pdS5BNYosQFXdEuUgRVZVtG9V8bf_hIZ_Iow,95
-c7n_mailer-0.6.8.dist-info/top_level.txt,sha256=L59wkuoIsn_VeK7uFkEsqsdn7_Qj3XCbA84GpNocka4,11
-c7n_mailer-0.6.8.dist-info/RECORD,,
+c7n_mailer-0.6.9.dist-info/METADATA,sha256=y0z9CEJn2fklVuacq2u2b1VqXmEx0kbZFvGhOYFxVY8,42863
+c7n_mailer-0.6.9.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
+c7n_mailer-0.6.9.dist-info/entry_points.txt,sha256=WjuO0T_pdS5BNYosQFXdEuUgRVZVtG9V8bf_hIZ_Iow,95
+c7n_mailer-0.6.9.dist-info/top_level.txt,sha256=L59wkuoIsn_VeK7uFkEsqsdn7_Qj3XCbA84GpNocka4,11
+c7n_mailer-0.6.9.dist-info/RECORD,,
```

