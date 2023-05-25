# Comparing `tmp/apigw_manager-1.2.0-py3-none-any.whl.zip` & `tmp/apigw_manager-2.0.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 40898 bytes, number of entries: 38
+Zip file size: 41967 bytes, number of entries: 39
 -rw-r--r--  2.0 unx      760 b- defN 80-Jan-01 00:00 apigw_manager/__init__.py
 -rw-r--r--  2.0 unx      760 b- defN 80-Jan-01 00:00 apigw_manager/apigw/__init__.py
 -rw-r--r--  2.0 unx     1058 b- defN 80-Jan-01 00:00 apigw_manager/apigw/admin.py
 -rw-r--r--  2.0 unx      878 b- defN 80-Jan-01 00:00 apigw_manager/apigw/apps.py
 -rw-r--r--  2.0 unx     5938 b- defN 80-Jan-01 00:00 apigw_manager/apigw/authentication.py
 -rw-r--r--  2.0 unx     3311 b- defN 80-Jan-01 00:00 apigw_manager/apigw/command.py
 -rw-r--r--  2.0 unx     1566 b- defN 80-Jan-01 00:00 apigw_manager/apigw/decorators.py
@@ -14,14 +14,15 @@
 -rw-r--r--  2.0 unx     6185 b- defN 80-Jan-01 00:00 apigw_manager/apigw/management/commands/create_version_and_release_apigw.py
 -rw-r--r--  2.0 unx     1965 b- defN 80-Jan-01 00:00 apigw_manager/apigw/management/commands/fetch_apigw_public_key.py
 -rw-r--r--  2.0 unx     1116 b- defN 80-Jan-01 00:00 apigw_manager/apigw/management/commands/fetch_esb_public_key.py
 -rw-r--r--  2.0 unx     1664 b- defN 80-Jan-01 00:00 apigw_manager/apigw/management/commands/grant_apigw_permissions.py
 -rw-r--r--  2.0 unx     1598 b- defN 80-Jan-01 00:00 apigw_manager/apigw/management/commands/sync_apigw_config.py
 -rw-r--r--  2.0 unx     2401 b- defN 80-Jan-01 00:00 apigw_manager/apigw/management/commands/sync_apigw_resources.py
 -rw-r--r--  2.0 unx     1153 b- defN 80-Jan-01 00:00 apigw_manager/apigw/management/commands/sync_apigw_stage.py
+-rw-r--r--  2.0 unx     1465 b- defN 80-Jan-01 00:00 apigw_manager/apigw/management/commands/sync_apigw_strategies.py
 -rw-r--r--  2.0 unx     2393 b- defN 80-Jan-01 00:00 apigw_manager/apigw/management/commands/sync_resource_docs_by_archive.py
 -rw-r--r--  2.0 unx     1915 b- defN 80-Jan-01 00:00 apigw_manager/apigw/migrations/0001_initial.py
 -rw-r--r--  2.0 unx      760 b- defN 80-Jan-01 00:00 apigw_manager/apigw/migrations/__init__.py
 -rw-r--r--  2.0 unx     1270 b- defN 80-Jan-01 00:00 apigw_manager/apigw/models.py
 -rw-r--r--  2.0 unx     6602 b- defN 80-Jan-01 00:00 apigw_manager/apigw/providers.py
 -rw-r--r--  2.0 unx     3907 b- defN 80-Jan-01 00:00 apigw_manager/apigw/utils.py
 -rw-r--r--  2.0 unx      760 b- defN 80-Jan-01 00:00 apigw_manager/apigw/views.py
@@ -30,11 +31,11 @@
 -rw-r--r--  2.0 unx     1441 b- defN 80-Jan-01 00:00 apigw_manager/core/exceptions.py
 -rw-r--r--  2.0 unx     1643 b- defN 80-Jan-01 00:00 apigw_manager/core/fetch.py
 -rw-r--r--  2.0 unx     4321 b- defN 80-Jan-01 00:00 apigw_manager/core/handler.py
 -rw-r--r--  2.0 unx     1415 b- defN 80-Jan-01 00:00 apigw_manager/core/permission.py
 -rw-r--r--  2.0 unx     1576 b- defN 80-Jan-01 00:00 apigw_manager/core/release.py
 -rw-r--r--  2.0 unx     1793 b- defN 80-Jan-01 00:00 apigw_manager/core/sync.py
 -rw-r--r--  2.0 unx     1096 b- defN 80-Jan-01 00:00 apigw_manager/core/utils.py
-?rw-r--r--  2.0 unx       83 b- defN 16-Jan-01 00:00 apigw_manager-1.2.0.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1107 b- defN 16-Jan-01 00:00 apigw_manager-1.2.0.dist-info/METADATA
-?rw-r--r--  2.0 unx     3638 b- defN 16-Jan-01 00:00 apigw_manager-1.2.0.dist-info/RECORD
-38 files, 79873 bytes uncompressed, 34916 bytes compressed:  56.3%
+-rw-r--r--  2.0 unx     1164 b- defN 80-Jan-01 00:00 apigw_manager-2.0.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 apigw_manager-2.0.0.dist-info/WHEEL
+?rw-r--r--  2.0 unx     3759 b- defN 16-Jan-01 00:00 apigw_manager-2.0.0.dist-info/RECORD
+39 files, 81521 bytes uncompressed, 35781 bytes compressed:  56.1%
```

## zipnote {}

```diff
@@ -51,14 +51,17 @@
 
 Filename: apigw_manager/apigw/management/commands/sync_apigw_resources.py
 Comment: 
 
 Filename: apigw_manager/apigw/management/commands/sync_apigw_stage.py
 Comment: 
 
+Filename: apigw_manager/apigw/management/commands/sync_apigw_strategies.py
+Comment: 
+
 Filename: apigw_manager/apigw/management/commands/sync_resource_docs_by_archive.py
 Comment: 
 
 Filename: apigw_manager/apigw/migrations/0001_initial.py
 Comment: 
 
 Filename: apigw_manager/apigw/migrations/__init__.py
@@ -99,17 +102,17 @@
 
 Filename: apigw_manager/core/sync.py
 Comment: 
 
 Filename: apigw_manager/core/utils.py
 Comment: 
 
-Filename: apigw_manager-1.2.0.dist-info/WHEEL
+Filename: apigw_manager-2.0.0.dist-info/METADATA
 Comment: 
 
-Filename: apigw_manager-1.2.0.dist-info/METADATA
+Filename: apigw_manager-2.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: apigw_manager-1.2.0.dist-info/RECORD
+Filename: apigw_manager-2.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `apigw_manager-1.2.0.dist-info/METADATA` & `apigw_manager-2.0.0.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: apigw-manager
-Version: 1.2.0
+Version: 2.0.0
 Summary: 
 Requires-Python: >=3.6.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: cryptography
 Provides-Extra: demo
 Provides-Extra: django
 Provides-Extra: kubernetes
-Requires-Dist: Django (>=1.11.1); extra == "django" or extra == "demo"
-Requires-Dist: PyMySQL (>=1.0.2,<2.0.0); extra == "demo"
+Requires-Dist: Django (>=1.11.1) ; extra == "django" or extra == "demo"
+Requires-Dist: PyMySQL (>=1.0.2,<2.0.0) ; extra == "demo"
 Requires-Dist: bkapi-bk-apigateway (>=1.0.11,<2.0.0)
 Requires-Dist: bkapi-client-core (>=1.1.3)
-Requires-Dist: cryptography (>=3.1.1); extra == "cryptography"
-Requires-Dist: django-environ (>=0.8.1); extra == "demo"
+Requires-Dist: cryptography (>=3.1.1) ; extra == "cryptography"
+Requires-Dist: django-environ (>=0.8.1) ; extra == "demo"
 Requires-Dist: future (==0.18.2)
-Requires-Dist: kubernetes; extra == "kubernetes"
+Requires-Dist: kubernetes ; extra == "kubernetes"
 Requires-Dist: packaging (>=21.0)
-Requires-Dist: pyjwt (>=1.6.4); extra == "cryptography" or extra == "django" or extra == "demo"
+Requires-Dist: pyjwt (>=1.6.4) ; extra == "cryptography" or extra == "django" or extra == "demo"
 Requires-Dist: pyyaml (>=5.4.1)
 Requires-Dist: setuptools (>=21.0.0)
 Requires-Dist: urllib3 (>=1.25.3)
```

## Comparing `apigw_manager-1.2.0.dist-info/RECORD` & `apigw_manager-2.0.0.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 apigw_manager/apigw/management/commands/create_version_and_release_apigw.py,sha256=JHoAvF3VifpeOWmjVsv5lVZnWsyIgdAEODFj1jcDDHA,6185
 apigw_manager/apigw/management/commands/fetch_apigw_public_key.py,sha256=1_-2A7PB3ZoONmB9_QaZEcAtaC61d82IotNNNSD0XQU,1965
 apigw_manager/apigw/management/commands/fetch_esb_public_key.py,sha256=qKt_k8SDrTuIr6OgT6yuG8e2KoOOqywP1WUMV8gtqxI,1116
 apigw_manager/apigw/management/commands/grant_apigw_permissions.py,sha256=HpMhVUjewtnCiaoN2DqMHQBrAOuvoPb8vRajh5TAkCo,1664
 apigw_manager/apigw/management/commands/sync_apigw_config.py,sha256=lU0fTJl_tvRwp_uovYcriTTJxoZGKgo5s4zG3_XxRss,1598
 apigw_manager/apigw/management/commands/sync_apigw_resources.py,sha256=49LI43U7HoxmrscuitBQJMrWKssPgeFFC299GQ9rYE8,2401
 apigw_manager/apigw/management/commands/sync_apigw_stage.py,sha256=ql9O_u3PcMvWVgSILSVRIULVgq1vVeuXGedAmXaUBas,1153
+apigw_manager/apigw/management/commands/sync_apigw_strategies.py,sha256=AwvQ5j9y8lxAV0pTq4gSgu97sbbWy64jYZmGeVpECbM,1465
 apigw_manager/apigw/management/commands/sync_resource_docs_by_archive.py,sha256=V1ZG43A4LqjH42LlT59ySiY-ROjz-ojLkKTlFqSabU8,2393
 apigw_manager/apigw/migrations/0001_initial.py,sha256=6EJOCcS4jYBgROzmkDKQKIQyo4ZBay11RZuK3bBC7U8,1915
 apigw_manager/apigw/migrations/__init__.py,sha256=IrhSBTIdq4nO5gGCVXRwR4rWptnjS6X0iGe53LVHp8g,760
 apigw_manager/apigw/models.py,sha256=Eu8udmsrxXV1obEoy9gTtFeNV2RZdOnG48Wcri3BX7s,1270
 apigw_manager/apigw/providers.py,sha256=EbpNpXcqTS7fRXa2VxA7fmOMy3wDWbxeeTl6xS6YbP0,6602
 apigw_manager/apigw/utils.py,sha256=vP8gPnV_s71MeBy3QGTtdBNrOoVpYA_PDyZ-YN1agKM,3907
 apigw_manager/apigw/views.py,sha256=IrhSBTIdq4nO5gGCVXRwR4rWptnjS6X0iGe53LVHp8g,760
@@ -29,10 +30,10 @@
 apigw_manager/core/exceptions.py,sha256=mKGaLRrdqHGuf3iAOizSqOvTr-pnybq9RHaUAe2weBk,1441
 apigw_manager/core/fetch.py,sha256=3SabZhCMh7F5DlC_SJkDHrJVAR6mhHLekO8z-gMV3zc,1643
 apigw_manager/core/handler.py,sha256=lYxhfBaJ_fQOKRrREOyWqcqRDTP5Hyc1G0DRh_OtTyU,4321
 apigw_manager/core/permission.py,sha256=RGvGbL60WZ9I0mzXnTHoEmUwP3AKlwysOV-nipdN0rk,1415
 apigw_manager/core/release.py,sha256=zu17zfYegBFx3MEpt2GjsSWEKvHd0B63IYplqtycGOc,1576
 apigw_manager/core/sync.py,sha256=iTmPDmBS_s-wIB5t94Lk-cpapqC-yayWQgK9xY1cpno,1793
 apigw_manager/core/utils.py,sha256=Em36ItO907rdziRYJizl540P-09aAXeprOSow60mCxc,1096
-apigw_manager-1.2.0.dist-info/WHEEL,sha256=DA86_h4QwwzGeRoz62o1svYt5kGEXpoUTuTtwzoTb30,83
-apigw_manager-1.2.0.dist-info/METADATA,sha256=QQluyhcwi_ltwSGpNhYkykELOQ5rez3ivK8wlZJVCbM,1107
-apigw_manager-1.2.0.dist-info/RECORD,,
+apigw_manager-2.0.0.dist-info/METADATA,sha256=Wn7BECrp3kCXIJ8CLNDV4G6trykbsdu-BbwUwLPj9jU,1164
+apigw_manager-2.0.0.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
+apigw_manager-2.0.0.dist-info/RECORD,,
```

