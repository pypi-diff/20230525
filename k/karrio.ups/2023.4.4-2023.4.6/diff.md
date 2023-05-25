# Comparing `tmp/karrio.ups-2023.4.4-py3-none-any.whl.zip` & `tmp/karrio.ups-2023.4.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -3,24 +3,24 @@
 -rw-rw-r--  2.0 unx     3992 b- defN 23-Apr-23 04:04 karrio/mappers/ups/mapper.py
 -rw-rw-r--  2.0 unx     4701 b- defN 23-Apr-23 04:04 karrio/mappers/ups/proxy.py
 -rw-rw-r--  2.0 unx      512 b- defN 23-Apr-23 04:04 karrio/mappers/ups/settings.py
 -rw-rw-r--  2.0 unx      819 b- defN 22-Nov-15 19:21 karrio/providers/ups/__init__.py
 -rw-rw-r--  2.0 unx     1843 b- defN 23-Apr-23 04:04 karrio/providers/ups/address.py
 -rw-rw-r--  2.0 unx     3380 b- defN 23-Apr-23 04:04 karrio/providers/ups/document.py
 -rw-rw-r--  2.0 unx     2554 b- defN 23-Mar-27 07:55 karrio/providers/ups/error.py
--rw-rw-r--  2.0 unx    15747 b- defN 23-May-17 00:17 karrio/providers/ups/rate.py
+-rw-rw-r--  2.0 unx    15747 b- defN 23-May-21 02:20 karrio/providers/ups/rate.py
 -rw-rw-r--  2.0 unx     4309 b- defN 23-Apr-23 04:04 karrio/providers/ups/tracking.py
 -rw-rw-r--  2.0 unx    16310 b- defN 23-Apr-23 04:04 karrio/providers/ups/units.py
 -rw-rw-r--  2.0 unx     2709 b- defN 23-Apr-23 04:04 karrio/providers/ups/utils.py
 -rw-rw-r--  2.0 unx      309 b- defN 22-Nov-15 19:21 karrio/providers/ups/pickup/__init__.py
 -rw-rw-r--  2.0 unx     1716 b- defN 23-Apr-23 04:04 karrio/providers/ups/pickup/cancel.py
--rw-rw-r--  2.0 unx     5653 b- defN 23-May-17 00:17 karrio/providers/ups/pickup/create.py
+-rw-rw-r--  2.0 unx     5653 b- defN 23-May-21 02:20 karrio/providers/ups/pickup/create.py
 -rw-rw-r--  2.0 unx     2285 b- defN 23-Apr-23 04:04 karrio/providers/ups/pickup/rate.py
 -rw-rw-r--  2.0 unx     1918 b- defN 23-Apr-23 04:04 karrio/providers/ups/pickup/update.py
 -rw-rw-r--  2.0 unx      222 b- defN 22-Nov-15 19:21 karrio/providers/ups/shipment/__init__.py
 -rw-rw-r--  2.0 unx     2659 b- defN 23-Apr-23 04:04 karrio/providers/ups/shipment/cancel.py
 -rw-rw-r--  2.0 unx    30434 b- defN 23-Apr-23 04:04 karrio/providers/ups/shipment/create.py
--rw-rw-r--  2.0 unx      951 b- defN 23-May-20 11:14 karrio.ups-2023.4.4.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-20 11:14 karrio.ups-2023.4.4.dist-info/WHEEL
--rw-rw-r--  2.0 unx        7 b- defN 23-May-20 11:14 karrio.ups-2023.4.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     2119 b- defN 23-May-20 11:14 karrio.ups-2023.4.4.dist-info/RECORD
+-rw-rw-r--  2.0 unx      951 b- defN 23-May-25 14:30 karrio.ups-2023.4.6.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-25 14:30 karrio.ups-2023.4.6.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        7 b- defN 23-May-25 14:30 karrio.ups-2023.4.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     2119 b- defN 23-May-25 14:30 karrio.ups-2023.4.6.dist-info/RECORD
 24 files, 105815 bytes uncompressed, 25792 bytes compressed:  75.6%
```

## zipnote {}

```diff
@@ -54,20 +54,20 @@
 
 Filename: karrio/providers/ups/shipment/cancel.py
 Comment: 
 
 Filename: karrio/providers/ups/shipment/create.py
 Comment: 
 
-Filename: karrio.ups-2023.4.4.dist-info/METADATA
+Filename: karrio.ups-2023.4.6.dist-info/METADATA
 Comment: 
 
-Filename: karrio.ups-2023.4.4.dist-info/WHEEL
+Filename: karrio.ups-2023.4.6.dist-info/WHEEL
 Comment: 
 
-Filename: karrio.ups-2023.4.4.dist-info/top_level.txt
+Filename: karrio.ups-2023.4.6.dist-info/top_level.txt
 Comment: 
 
-Filename: karrio.ups-2023.4.4.dist-info/RECORD
+Filename: karrio.ups-2023.4.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `karrio.ups-2023.4.4.dist-info/METADATA` & `karrio.ups-2023.4.6.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: karrio.ups
-Version: 2023.4.4
+Version: 2023.4.6
 Summary: Karrio - UPS Shipping extension
 Home-page: https://github.com/karrioapi/karrio
 Author: karrio
 Author-email: hello@karrio.io
 License: Apache-2.0
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

## Comparing `karrio.ups-2023.4.4.dist-info/RECORD` & `karrio.ups-2023.4.6.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -14,11 +14,11 @@
 karrio/providers/ups/pickup/cancel.py,sha256=OuECyxmV3JBPcJt6yfvFkSMWUHTIPD8oeUUpB2XwUFM,1716
 karrio/providers/ups/pickup/create.py,sha256=iG1bOYbtVH8SQz6JG_t5xJStkLshxqpl3uhkXOXnn_0,5653
 karrio/providers/ups/pickup/rate.py,sha256=YF-bm3EzzJMyfTq3i2dyAb9PuuXK-yyjdW8brqGT0Ow,2285
 karrio/providers/ups/pickup/update.py,sha256=kSYEOw5k42cqGKqC_oQPTAOJzoGJ6AajYFuz6UiVR84,1918
 karrio/providers/ups/shipment/__init__.py,sha256=JqRkKBAx-8wJ3_RSvWD76ink2bX2N3LRi132oNB76xk,222
 karrio/providers/ups/shipment/cancel.py,sha256=3hmkDCHRRXvSSo13jVHKnh6fx2LBNBzsyjcUbo5qJcY,2659
 karrio/providers/ups/shipment/create.py,sha256=FCC7EuVB8FELKNQXBly-YPZWmXyd3FGERniXfNybfFs,30434
-karrio.ups-2023.4.4.dist-info/METADATA,sha256=E-8FPdbdR4uVf4A9j8cWv6XsMcLlKlaIWDnCUMMLFaw,951
-karrio.ups-2023.4.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-karrio.ups-2023.4.4.dist-info/top_level.txt,sha256=mfkVZXzNuVRmA7NRlck_Ub-C8Zgtqxbx3gX1Rq_W-i0,7
-karrio.ups-2023.4.4.dist-info/RECORD,,
+karrio.ups-2023.4.6.dist-info/METADATA,sha256=z2mI03iN8k60xLKWIaUhW3o8mH1QWqIjrDGLL_4AbV8,951
+karrio.ups-2023.4.6.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+karrio.ups-2023.4.6.dist-info/top_level.txt,sha256=mfkVZXzNuVRmA7NRlck_Ub-C8Zgtqxbx3gX1Rq_W-i0,7
+karrio.ups-2023.4.6.dist-info/RECORD,,
```

