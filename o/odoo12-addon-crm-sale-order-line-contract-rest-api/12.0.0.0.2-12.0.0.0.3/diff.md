# Comparing `tmp/odoo12_addon_crm_sale_order_line_contract_rest_api-12.0.0.0.2-py3-none-any.whl.zip` & `tmp/odoo12_addon_crm_sale_order_line_contract_rest_api-12.0.0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 4135 bytes, number of entries: 10
--rwxr-xr-x  2.0 unx      205 b- defN 23-Apr-21 07:41 odoo/addons/crm_sale_order_line_contract_rest_api/README.rst
--rwxr-xr-x  2.0 unx       23 b- defN 23-Apr-21 07:41 odoo/addons/crm_sale_order_line_contract_rest_api/__init__.py
--rwxr-xr-x  2.0 unx      522 b- defN 23-Apr-21 13:15 odoo/addons/crm_sale_order_line_contract_rest_api/__manifest__.py
--rwxr-xr-x  2.0 unx       32 b- defN 23-Apr-21 07:41 odoo/addons/crm_sale_order_line_contract_rest_api/services/__init__.py
--rwxr-xr-x  2.0 unx      358 b- defN 23-Apr-21 07:41 odoo/addons/crm_sale_order_line_contract_rest_api/services/crm_lead_services.py
--rwxr-xr-x  2.0 unx     1181 b- defN 23-Apr-21 13:01 odoo/addons/crm_sale_order_line_contract_rest_api/services/schemas.py
--rw-r--r--  2.0 unx      652 b- defN 23-Apr-21 13:22 odoo12_addon_crm_sale_order_line_contract_rest_api-12.0.0.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-21 13:22 odoo12_addon_crm_sale_order_line_contract_rest_api-12.0.0.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 23-Apr-21 13:22 odoo12_addon_crm_sale_order_line_contract_rest_api-12.0.0.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1227 b- defN 23-Apr-21 13:22 odoo12_addon_crm_sale_order_line_contract_rest_api-12.0.0.0.2.dist-info/RECORD
-10 files, 4297 bytes uncompressed, 1905 bytes compressed:  55.7%
+Zip file size: 4136 bytes, number of entries: 10
+-rwxr-xr-x  2.0 unx      205 b- defN 23-May-11 14:11 odoo/addons/crm_sale_order_line_contract_rest_api/README.rst
+-rwxr-xr-x  2.0 unx       23 b- defN 23-May-11 14:11 odoo/addons/crm_sale_order_line_contract_rest_api/__init__.py
+-rwxr-xr-x  2.0 unx      522 b- defN 23-May-25 07:37 odoo/addons/crm_sale_order_line_contract_rest_api/__manifest__.py
+-rwxr-xr-x  2.0 unx       32 b- defN 23-May-11 14:11 odoo/addons/crm_sale_order_line_contract_rest_api/services/__init__.py
+-rwxr-xr-x  2.0 unx      358 b- defN 23-May-11 14:11 odoo/addons/crm_sale_order_line_contract_rest_api/services/crm_lead_services.py
+-rwxr-xr-x  2.0 unx     1179 b- defN 23-May-24 15:21 odoo/addons/crm_sale_order_line_contract_rest_api/services/schemas.py
+-rw-r--r--  2.0 unx      652 b- defN 23-May-25 07:41 odoo12_addon_crm_sale_order_line_contract_rest_api-12.0.0.0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-25 07:41 odoo12_addon_crm_sale_order_line_contract_rest_api-12.0.0.0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 23-May-25 07:41 odoo12_addon_crm_sale_order_line_contract_rest_api-12.0.0.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1227 b- defN 23-May-25 07:41 odoo12_addon_crm_sale_order_line_contract_rest_api-12.0.0.0.3.dist-info/RECORD
+10 files, 4295 bytes uncompressed, 1906 bytes compressed:  55.6%
```

## zipnote {}

```diff
@@ -12,20 +12,20 @@
 
 Filename: odoo/addons/crm_sale_order_line_contract_rest_api/services/crm_lead_services.py
 Comment: 
 
 Filename: odoo/addons/crm_sale_order_line_contract_rest_api/services/schemas.py
 Comment: 
 
-Filename: odoo12_addon_crm_sale_order_line_contract_rest_api-12.0.0.0.2.dist-info/METADATA
+Filename: odoo12_addon_crm_sale_order_line_contract_rest_api-12.0.0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: odoo12_addon_crm_sale_order_line_contract_rest_api-12.0.0.0.2.dist-info/WHEEL
+Filename: odoo12_addon_crm_sale_order_line_contract_rest_api-12.0.0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: odoo12_addon_crm_sale_order_line_contract_rest_api-12.0.0.0.2.dist-info/top_level.txt
+Filename: odoo12_addon_crm_sale_order_line_contract_rest_api-12.0.0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo12_addon_crm_sale_order_line_contract_rest_api-12.0.0.0.2.dist-info/RECORD
+Filename: odoo12_addon_crm_sale_order_line_contract_rest_api-12.0.0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## odoo/addons/crm_sale_order_line_contract_rest_api/__manifest__.py

```diff
@@ -5,15 +5,15 @@
     'summary': """
         Enhance CRM order lines Rest API to add contract specific configs""",
 
     'author': "Coopdevs Treball SCCL",
     'website': "",
 
     'category': 'api',
-    'version': '12.0.0.0.2',
+    'version': '12.0.0.0.3',
 
     # any module necessary for this one to work correctly
     'depends': [
         'base',
         'crm_sale_order_line_rest_api'
     ],
```

## odoo/addons/crm_sale_order_line_contract_rest_api/services/schemas.py

```diff
@@ -7,15 +7,15 @@
     "order_lines": {
         "type": "list",
         "empty": True,
         "schema": {
             "type": "dict",
             "schema": {
                 "product_id": {"type": "integer", "required": True},
-                "price_unit": {"type": "integer", "required": False},
+                "price_unit": {"type": "float", "required": False},
                 "attach_to_existing_contract": {
                     "type": "boolean",
                     "required": False
                 },
                 "contract_id": {
                     "type": "integer",
                     "required": False
```

## Comparing `odoo12_addon_crm_sale_order_line_contract_rest_api-12.0.0.0.2.dist-info/METADATA` & `odoo12_addon_crm_sale_order_line_contract_rest_api-12.0.0.0.3.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo12-addon-crm-sale-order-line-contract-rest-api
-Version: 12.0.0.0.2
+Version: 12.0.0.0.3
 Summary: Enhance CRM order lines Rest API to add contract specific configs
 Home-page: 
 Author: Coopdevs Treball SCCL
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 12.0
 Requires-Python: >=3.5
```

## Comparing `odoo12_addon_crm_sale_order_line_contract_rest_api-12.0.0.0.2.dist-info/RECORD` & `odoo12_addon_crm_sale_order_line_contract_rest_api-12.0.0.0.3.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 odoo/addons/crm_sale_order_line_contract_rest_api/README.rst,sha256=fZIaxyCLibnyk-uEeHmrT7mTISskLKTpK0RHge8hMe8,205
 odoo/addons/crm_sale_order_line_contract_rest_api/__init__.py,sha256=qksdRxAxHhEXpY0NZlTEolhxFILjRI5o7J0O4UrAE04,23
-odoo/addons/crm_sale_order_line_contract_rest_api/__manifest__.py,sha256=ERxyzfxnBxjxnm_zh_yK_z4HTbwHOTGVPlSLTl6RzhM,522
+odoo/addons/crm_sale_order_line_contract_rest_api/__manifest__.py,sha256=ZJgr5wdV2hp5U6v-mkKItfbiAYjg_Z7dbWpNk5Ntct0,522
 odoo/addons/crm_sale_order_line_contract_rest_api/services/__init__.py,sha256=gyXaE_NlVgF1KawzsiRb0DeYYTT13kmL4Ya1LgcRg5c,32
 odoo/addons/crm_sale_order_line_contract_rest_api/services/crm_lead_services.py,sha256=tGc69_TjJnQefIMrdI1LCsggLSINAhWR-8nl3DhYi3g,358
-odoo/addons/crm_sale_order_line_contract_rest_api/services/schemas.py,sha256=RXYcIqNJ6QSUw0Iujsw98cYhJwyB5PYJAR8j5oiqFqU,1181
-odoo12_addon_crm_sale_order_line_contract_rest_api-12.0.0.0.2.dist-info/METADATA,sha256=r2CXkGVQKEzXOjBnMvDGYokMVWlVZSI23OvoAJIgVlc,652
-odoo12_addon_crm_sale_order_line_contract_rest_api-12.0.0.0.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-odoo12_addon_crm_sale_order_line_contract_rest_api-12.0.0.0.2.dist-info/top_level.txt,sha256=qBj40grFkGOfDZ2WDSw3y1RnDlgG0u8rP8pvGNdbz4w,5
-odoo12_addon_crm_sale_order_line_contract_rest_api-12.0.0.0.2.dist-info/RECORD,,
+odoo/addons/crm_sale_order_line_contract_rest_api/services/schemas.py,sha256=Z-iFrHHj0o2mvS9AT3p3x-i75oSSlmYEC761zDk5mOM,1179
+odoo12_addon_crm_sale_order_line_contract_rest_api-12.0.0.0.3.dist-info/METADATA,sha256=A97vwkfAYcMrtJGj7OcomU9SNSpeHMgWpgYh0R6Vg_0,652
+odoo12_addon_crm_sale_order_line_contract_rest_api-12.0.0.0.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+odoo12_addon_crm_sale_order_line_contract_rest_api-12.0.0.0.3.dist-info/top_level.txt,sha256=qBj40grFkGOfDZ2WDSw3y1RnDlgG0u8rP8pvGNdbz4w,5
+odoo12_addon_crm_sale_order_line_contract_rest_api-12.0.0.0.3.dist-info/RECORD,,
```

