# Comparing `tmp/karrio.fedex-2023.4.4-py3-none-any.whl.zip` & `tmp/karrio.fedex-2023.4.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,26 +1,26 @@
-Zip file size: 31986 bytes, number of entries: 24
+Zip file size: 32042 bytes, number of entries: 24
 -rw-rw-r--  2.0 unx      535 b- defN 22-Nov-15 19:21 karrio/mappers/fedex/__init__.py
 -rw-rw-r--  2.0 unx     3996 b- defN 23-Apr-23 04:04 karrio/mappers/fedex/mapper.py
 -rw-rw-r--  2.0 unx     3556 b- defN 23-Apr-23 04:04 karrio/mappers/fedex/proxy.py
 -rw-rw-r--  2.0 unx      603 b- defN 23-Apr-23 04:04 karrio/mappers/fedex/settings.py
 -rw-rw-r--  2.0 unx      833 b- defN 22-Nov-15 19:21 karrio/providers/fedex/__init__.py
--rw-rw-r--  2.0 unx     4518 b- defN 23-May-17 00:17 karrio/providers/fedex/address.py
+-rw-rw-r--  2.0 unx     4518 b- defN 23-May-21 02:20 karrio/providers/fedex/address.py
 -rw-rw-r--  2.0 unx     4414 b- defN 23-Apr-23 04:04 karrio/providers/fedex/document.py
 -rw-rw-r--  2.0 unx     1074 b- defN 22-Nov-15 19:21 karrio/providers/fedex/error.py
--rw-rw-r--  2.0 unx    12452 b- defN 23-Apr-23 04:04 karrio/providers/fedex/rate.py
--rw-rw-r--  2.0 unx     6184 b- defN 23-May-18 05:41 karrio/providers/fedex/tracking.py
+-rw-rw-r--  2.0 unx    12585 b- defN 23-May-24 18:16 karrio/providers/fedex/rate.py
+-rw-rw-r--  2.0 unx     6184 b- defN 23-May-21 02:20 karrio/providers/fedex/tracking.py
 -rw-rw-r--  2.0 unx    19457 b- defN 23-Mar-27 07:55 karrio/providers/fedex/units.py
 -rw-rw-r--  2.0 unx     1753 b- defN 23-Apr-15 02:55 karrio/providers/fedex/utils.py
 -rw-rw-r--  2.0 unx      289 b- defN 22-Nov-15 19:21 karrio/providers/fedex/pickup/__init__.py
--rw-rw-r--  2.0 unx     2599 b- defN 23-May-17 00:17 karrio/providers/fedex/pickup/availability.py
+-rw-rw-r--  2.0 unx     2599 b- defN 23-May-21 02:20 karrio/providers/fedex/pickup/availability.py
 -rw-rw-r--  2.0 unx     2637 b- defN 23-Apr-23 04:04 karrio/providers/fedex/pickup/cancel.py
 -rw-rw-r--  2.0 unx     6150 b- defN 23-Apr-23 04:04 karrio/providers/fedex/pickup/create.py
 -rw-rw-r--  2.0 unx     2057 b- defN 23-Apr-23 04:04 karrio/providers/fedex/pickup/update.py
 -rw-rw-r--  2.0 unx      226 b- defN 22-Nov-15 19:21 karrio/providers/fedex/shipment/__init__.py
 -rw-rw-r--  2.0 unx     2357 b- defN 23-Apr-23 04:04 karrio/providers/fedex/shipment/cancel.py
 -rw-rw-r--  2.0 unx    31290 b- defN 23-Apr-23 04:04 karrio/providers/fedex/shipment/create.py
--rw-rw-r--  2.0 unx      969 b- defN 23-May-20 11:14 karrio.fedex-2023.4.4.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-20 11:14 karrio.fedex-2023.4.4.dist-info/WHEEL
--rw-rw-r--  2.0 unx        7 b- defN 23-May-20 11:14 karrio.fedex-2023.4.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     2175 b- defN 23-May-20 11:14 karrio.fedex-2023.4.4.dist-info/RECORD
-24 files, 110223 bytes uncompressed, 28402 bytes compressed:  74.2%
+-rw-rw-r--  2.0 unx      969 b- defN 23-May-25 14:30 karrio.fedex-2023.4.6.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-25 14:30 karrio.fedex-2023.4.6.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        7 b- defN 23-May-25 14:30 karrio.fedex-2023.4.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     2175 b- defN 23-May-25 14:30 karrio.fedex-2023.4.6.dist-info/RECORD
+24 files, 110356 bytes uncompressed, 28458 bytes compressed:  74.2%
```

## zipnote {}

```diff
@@ -54,20 +54,20 @@
 
 Filename: karrio/providers/fedex/shipment/cancel.py
 Comment: 
 
 Filename: karrio/providers/fedex/shipment/create.py
 Comment: 
 
-Filename: karrio.fedex-2023.4.4.dist-info/METADATA
+Filename: karrio.fedex-2023.4.6.dist-info/METADATA
 Comment: 
 
-Filename: karrio.fedex-2023.4.4.dist-info/WHEEL
+Filename: karrio.fedex-2023.4.6.dist-info/WHEEL
 Comment: 
 
-Filename: karrio.fedex-2023.4.4.dist-info/top_level.txt
+Filename: karrio.fedex-2023.4.6.dist-info/top_level.txt
 Comment: 
 
-Filename: karrio.fedex-2023.4.4.dist-info/RECORD
+Filename: karrio.fedex-2023.4.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## karrio/providers/fedex/rate.py

```diff
@@ -1,8 +1,7 @@
-from datetime import datetime
 from fedex_lib.rate_service_v28 import (
     RateRequest as FedexRateRequest,
     RateReplyDetail,
     TransactionDetail,
     VersionId,
     RequestedShipment,
     TaxpayerIdentification,
@@ -15,14 +14,15 @@
     RequestedPackageLineItem,
     Dimensions,
     CustomerReference,
     CustomerReferenceType,
 )
 
 import typing
+import datetime
 import karrio.lib as lib
 import karrio.core.units as units
 import karrio.core.models as models
 import karrio.providers.fedex.error as provider_error
 import karrio.providers.fedex.units as provider_units
 import karrio.providers.fedex.utils as provider_utils
 
@@ -66,26 +66,28 @@
         ("Base charge", shipment_rate.TotalBaseCharge.Amount),
         ("Discount", getattr(shipment_discount, "Amount", None)),
         *(
             (s.Description, s.Amount.Amount)
             for s in shipment_rate.Surcharges + shipment_rate.Taxes
         ),
     ]
-    estimated_delivery = lib.to_date(rate.DeliveryTimestamp)
-    shipping_date = lib.to_date(ctx.get("shipment_date") or datetime.now())
-    transit = (
-        ((estimated_delivery.date() - shipping_date.date()).days or None)
-        if estimated_delivery is not None
-        else None
-    )
     applied_options = (
         dict(applied_options=applied_options)
         if (applied_options is not None and len(applied_options) > 0)
         else {}
     )
+    transit = None
+    estimated_delivery = lib.to_date(rate.DeliveryTimestamp)
+    shipping_date = lib.to_date(ctx.get("shipment_date") or datetime.datetime.now())
+    if estimated_delivery is not None:
+        days = (
+            shipping_date + datetime.timedelta(x + 1)
+            for x in range((estimated_delivery.date() - shipping_date.date()).days)
+        )
+        transit = sum(1 for day in days if day.weekday() < 5)
 
     return models.RateDetails(
         carrier_name=settings.carrier_name,
         carrier_id=settings.carrier_id,
         service=service.name_or_key,
         currency=currency,
         total_charge=lib.to_decimal(
@@ -120,15 +122,15 @@
     options = lib.to_shipping_options(
         payload.options,
         package_options=packages.options,
         option_type=provider_units.RatingOption,
         initializer=provider_units.shipping_options_initializer,
     )
     request_types = ["LIST"] + ([] if "currency" not in options else ["PREFERRED"])
-    shipment_date = lib.to_date(options.shipment_date.state or datetime.now())
+    shipment_date = lib.to_date(options.shipment_date.state or datetime.datetime.now())
 
     request = FedexRateRequest(
         WebAuthenticationDetail=settings.webAuthenticationDetail,
         ClientDetail=settings.clientDetail,
         TransactionDetail=TransactionDetail(CustomerTransactionId="FTC"),
         Version=VersionId(ServiceId="crs", Major=28, Intermediate=0, Minor=0),
         ReturnTransitAndCommit=True,
```

## Comparing `karrio.fedex-2023.4.4.dist-info/METADATA` & `karrio.fedex-2023.4.6.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: karrio.fedex
-Version: 2023.4.4
+Version: 2023.4.6
 Summary: Karrio - Fedex Shipping extension
 Home-page: https://github.com/karrioapi/karrio
 Author: karrio
 Author-email: hello@karrio.io
 License: Apache-2.0
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

## Comparing `karrio.fedex-2023.4.4.dist-info/RECORD` & `karrio.fedex-2023.4.6.dist-info/RECORD`

 * *Files 5% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 karrio/mappers/fedex/mapper.py,sha256=LIOzi69-boBNKYcqURKrv1lLeCoG_cuq0Jx6mdaA-_I,3996
 karrio/mappers/fedex/proxy.py,sha256=08bxmfJH-Wg3_76LKfZDCF-qxtfba2PJDiOCeGtdAjA,3556
 karrio/mappers/fedex/settings.py,sha256=GDhqnw6z-DkT1s3-ytYT3IYAyt-mDYAr0SuOpnMq0S0,603
 karrio/providers/fedex/__init__.py,sha256=jdHaTk7oqsmI6C8_19mv5vwDGgvisBXaP87o-SnEMB0,833
 karrio/providers/fedex/address.py,sha256=K4W3dgZvzzwZ0sX6TwdvAeV02Dqog1o4LM1mgnLhwf8,4518
 karrio/providers/fedex/document.py,sha256=sdwV3DfMXdIj8kLzHX65jwetrha-C2JVNi1UDRNQXgo,4414
 karrio/providers/fedex/error.py,sha256=ilLswzwO1GktrRylZZl7sfxzlXinjOmHrrx35tfrU8I,1074
-karrio/providers/fedex/rate.py,sha256=Pkl_YVQDQKQH9KdYMUzEKFWUb6h0AmF66jGYG3UcbnI,12452
+karrio/providers/fedex/rate.py,sha256=J-IZ_implWhtk86A_VokGyTDFOXYMWM4DYihdPcCn9s,12585
 karrio/providers/fedex/tracking.py,sha256=xpSgetbDObtYpo6KBh8YVXsjNwhMVF7SvA5a44cC0iY,6184
 karrio/providers/fedex/units.py,sha256=zb9WOvF-DJhKnj_yqTDz-mUpVmzKOkDzvfAmRN_dSRo,19457
 karrio/providers/fedex/utils.py,sha256=lzhiOwr0Wlwd2bv_aJ9joyYRVp3JiK5izloAbgL_XSU,1753
 karrio/providers/fedex/pickup/__init__.py,sha256=zYavrB_GHWEjNyebHSBjqI4gRMOhd2BYr67ivmxxK4o,289
 karrio/providers/fedex/pickup/availability.py,sha256=G6GW6n4PYSwtmE6GsNMFU4aPo2D9qMOvfEtRSKLmewM,2599
 karrio/providers/fedex/pickup/cancel.py,sha256=QV9913sqGSGHjNUVzwDNp_LhhtHZjxWhEObgoqwNN14,2637
 karrio/providers/fedex/pickup/create.py,sha256=KYif9AooxuOd9VmPfSJHNdSiRWVNve-YSx3fMmteHPc,6150
 karrio/providers/fedex/pickup/update.py,sha256=bJFvCYLFKNCBFZVgrfiOj_Zeines-VrdTxt2UtSbIHA,2057
 karrio/providers/fedex/shipment/__init__.py,sha256=dBO2yZUpISVe-H4Cvf8WZmOuPgxZlGsW4u145ly5gpA,226
 karrio/providers/fedex/shipment/cancel.py,sha256=pjO0oiljqS9_icV4S9GXfarKRfS6VyWXaThdJhw2_bc,2357
 karrio/providers/fedex/shipment/create.py,sha256=r-DwMwwjmpt3j9dXYtIQP06TEmsG2JvHIgdo68rpZUE,31290
-karrio.fedex-2023.4.4.dist-info/METADATA,sha256=J58kom-4NUgu0SKahCFFwD7pIEfer91aa-5acY1zs_s,969
-karrio.fedex-2023.4.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-karrio.fedex-2023.4.4.dist-info/top_level.txt,sha256=mfkVZXzNuVRmA7NRlck_Ub-C8Zgtqxbx3gX1Rq_W-i0,7
-karrio.fedex-2023.4.4.dist-info/RECORD,,
+karrio.fedex-2023.4.6.dist-info/METADATA,sha256=tMejBX3thhlAOktAXuhxh_7wNyNtG5CjnNt5M7KK1Ys,969
+karrio.fedex-2023.4.6.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+karrio.fedex-2023.4.6.dist-info/top_level.txt,sha256=mfkVZXzNuVRmA7NRlck_Ub-C8Zgtqxbx3gX1Rq_W-i0,7
+karrio.fedex-2023.4.6.dist-info/RECORD,,
```

