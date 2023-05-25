# Comparing `tmp/odoo12_addon_crm_sale_order_line_rest_api-12.0.0.0.3-py3-none-any.whl.zip` & `tmp/odoo12_addon_crm_sale_order_line_rest_api-12.0.0.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 3904 bytes, number of entries: 10
--rwxr-xr-x  2.0 unx      149 b- defN 23-Apr-21 07:41 odoo/addons/crm_sale_order_line_rest_api/README.rst
--rwxr-xr-x  2.0 unx       23 b- defN 23-Apr-21 07:41 odoo/addons/crm_sale_order_line_rest_api/__init__.py
--rwxr-xr-x  2.0 unx      501 b- defN 23-Apr-26 11:08 odoo/addons/crm_sale_order_line_rest_api/__manifest__.py
--rwxr-xr-x  2.0 unx       32 b- defN 23-Apr-21 07:41 odoo/addons/crm_sale_order_line_rest_api/services/__init__.py
--rwxr-xr-x  2.0 unx      906 b- defN 23-Apr-26 11:04 odoo/addons/crm_sale_order_line_rest_api/services/crm_lead_services.py
--rwxr-xr-x  2.0 unx      332 b- defN 23-Apr-21 12:57 odoo/addons/crm_sale_order_line_rest_api/services/schemas.py
--rw-r--r--  2.0 unx      592 b- defN 23-Apr-26 11:10 odoo12_addon_crm_sale_order_line_rest_api-12.0.0.0.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-26 11:10 odoo12_addon_crm_sale_order_line_rest_api-12.0.0.0.3.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 23-Apr-26 11:10 odoo12_addon_crm_sale_order_line_rest_api-12.0.0.0.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1136 b- defN 23-Apr-26 11:10 odoo12_addon_crm_sale_order_line_rest_api-12.0.0.0.3.dist-info/RECORD
-10 files, 3768 bytes uncompressed, 1854 bytes compressed:  50.8%
+Zip file size: 3911 bytes, number of entries: 10
+-rwxr-xr-x  2.0 unx      149 b- defN 23-May-11 14:11 odoo/addons/crm_sale_order_line_rest_api/README.rst
+-rwxr-xr-x  2.0 unx       23 b- defN 23-May-11 14:11 odoo/addons/crm_sale_order_line_rest_api/__init__.py
+-rwxr-xr-x  2.0 unx      501 b- defN 23-May-25 07:39 odoo/addons/crm_sale_order_line_rest_api/__manifest__.py
+-rwxr-xr-x  2.0 unx       32 b- defN 23-May-11 14:11 odoo/addons/crm_sale_order_line_rest_api/services/__init__.py
+-rwxr-xr-x  2.0 unx      906 b- defN 23-May-11 14:12 odoo/addons/crm_sale_order_line_rest_api/services/crm_lead_services.py
+-rwxr-xr-x  2.0 unx      330 b- defN 23-May-24 14:08 odoo/addons/crm_sale_order_line_rest_api/services/schemas.py
+-rw-r--r--  2.0 unx      592 b- defN 23-May-25 07:42 odoo12_addon_crm_sale_order_line_rest_api-12.0.0.0.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-25 07:42 odoo12_addon_crm_sale_order_line_rest_api-12.0.0.0.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 23-May-25 07:42 odoo12_addon_crm_sale_order_line_rest_api-12.0.0.0.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1136 b- defN 23-May-25 07:42 odoo12_addon_crm_sale_order_line_rest_api-12.0.0.0.4.dist-info/RECORD
+10 files, 3766 bytes uncompressed, 1861 bytes compressed:  50.6%
```

## zipnote {}

```diff
@@ -12,20 +12,20 @@
 
 Filename: odoo/addons/crm_sale_order_line_rest_api/services/crm_lead_services.py
 Comment: 
 
 Filename: odoo/addons/crm_sale_order_line_rest_api/services/schemas.py
 Comment: 
 
-Filename: odoo12_addon_crm_sale_order_line_rest_api-12.0.0.0.3.dist-info/METADATA
+Filename: odoo12_addon_crm_sale_order_line_rest_api-12.0.0.0.4.dist-info/METADATA
 Comment: 
 
-Filename: odoo12_addon_crm_sale_order_line_rest_api-12.0.0.0.3.dist-info/WHEEL
+Filename: odoo12_addon_crm_sale_order_line_rest_api-12.0.0.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: odoo12_addon_crm_sale_order_line_rest_api-12.0.0.0.3.dist-info/top_level.txt
+Filename: odoo12_addon_crm_sale_order_line_rest_api-12.0.0.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo12_addon_crm_sale_order_line_rest_api-12.0.0.0.3.dist-info/RECORD
+Filename: odoo12_addon_crm_sale_order_line_rest_api-12.0.0.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## odoo/addons/crm_sale_order_line_rest_api/__manifest__.py

```diff
@@ -5,15 +5,15 @@
     'summary': """
         Expose CRM order lines on the Rest API""",
 
     'author': "Coopdevs Treball SCCL",
     'website': "",
 
     'category': 'api',
-    'version': '12.0.0.0.3',
+    'version': '12.0.0.0.4',
 
     # any module necessary for this one to work correctly
     'depends': [
         'base',
         'crm_rest_api',
         'crm_sale_order_line'
     ],
```

## odoo/addons/crm_sale_order_line_rest_api/services/schemas.py

```diff
@@ -2,12 +2,12 @@
     "order_lines": {
         "type": "list",
         "empty": True,
         "schema": {
             "type": "dict",
             "schema": {
                 "product_id": {"type": "integer", "required": True},
-                "price_unit": {"type": "integer", "required": False}
+                "price_unit": {"type": "float", "required": False}
             }
         }
     }
 }
```

## Comparing `odoo12_addon_crm_sale_order_line_rest_api-12.0.0.0.3.dist-info/METADATA` & `odoo12_addon_crm_sale_order_line_rest_api-12.0.0.0.4.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo12-addon-crm-sale-order-line-rest-api
-Version: 12.0.0.0.3
+Version: 12.0.0.0.4
 Summary: Expose CRM order lines on the Rest API
 Home-page: 
 Author: Coopdevs Treball SCCL
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 12.0
 Requires-Python: >=3.5
```

## Comparing `odoo12_addon_crm_sale_order_line_rest_api-12.0.0.0.3.dist-info/RECORD` & `odoo12_addon_crm_sale_order_line_rest_api-12.0.0.0.4.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 odoo/addons/crm_sale_order_line_rest_api/README.rst,sha256=TbC3DjY4NLfKhsHanGsOWW_jEi0eFHD4Hbq0nKihPxY,149
 odoo/addons/crm_sale_order_line_rest_api/__init__.py,sha256=qksdRxAxHhEXpY0NZlTEolhxFILjRI5o7J0O4UrAE04,23
-odoo/addons/crm_sale_order_line_rest_api/__manifest__.py,sha256=lYNqTgDrk9rvF8fgkG1cZNDa2PFcoB152MGrjKFVGwA,501
+odoo/addons/crm_sale_order_line_rest_api/__manifest__.py,sha256=eqFg38W7bx6KjAIccJeIOUnvv6qgU5VrCik7Tcn5yaI,501
 odoo/addons/crm_sale_order_line_rest_api/services/__init__.py,sha256=gyXaE_NlVgF1KawzsiRb0DeYYTT13kmL4Ya1LgcRg5c,32
 odoo/addons/crm_sale_order_line_rest_api/services/crm_lead_services.py,sha256=xMr4PV_YLnn_2OB51WCNEzhQ3Xn7yASMzVievYjHKbQ,906
-odoo/addons/crm_sale_order_line_rest_api/services/schemas.py,sha256=tTudvFX7WOVnZ_58fjiEzl4m8LnXuvw2j_gGgqcmIEE,332
-odoo12_addon_crm_sale_order_line_rest_api-12.0.0.0.3.dist-info/METADATA,sha256=WRkQGka89YJLYDD6bua03mhbiV4sRANAjKACmz5rJEE,592
-odoo12_addon_crm_sale_order_line_rest_api-12.0.0.0.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-odoo12_addon_crm_sale_order_line_rest_api-12.0.0.0.3.dist-info/top_level.txt,sha256=qBj40grFkGOfDZ2WDSw3y1RnDlgG0u8rP8pvGNdbz4w,5
-odoo12_addon_crm_sale_order_line_rest_api-12.0.0.0.3.dist-info/RECORD,,
+odoo/addons/crm_sale_order_line_rest_api/services/schemas.py,sha256=niU20xgQRWGLzqTVlw-E1uONW3zIy7oDJThcK6-RSss,330
+odoo12_addon_crm_sale_order_line_rest_api-12.0.0.0.4.dist-info/METADATA,sha256=H6jmYeBJdwLr9iqLbsLApIBw9P0aFd1zFn5xH_Tec6M,592
+odoo12_addon_crm_sale_order_line_rest_api-12.0.0.0.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+odoo12_addon_crm_sale_order_line_rest_api-12.0.0.0.4.dist-info/top_level.txt,sha256=qBj40grFkGOfDZ2WDSw3y1RnDlgG0u8rP8pvGNdbz4w,5
+odoo12_addon_crm_sale_order_line_rest_api-12.0.0.0.4.dist-info/RECORD,,
```

