# Comparing `tmp/odoo14_addon_aresta-14.0.1.0.0-py3-none-any.whl.zip` & `tmp/odoo14_addon_aresta-14.0.1.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,26 +1,26 @@
-Zip file size: 12032 bytes, number of entries: 24
+Zip file size: 12017 bytes, number of entries: 24
 -rw-r--r--  2.0 unx       64 b- defN 22-May-23 15:44 odoo/addons/aresta/__init__.py
--rw-r--r--  2.0 unx      799 b- defN 23-May-21 18:08 odoo/addons/aresta/__manifest__.py
+-rw-r--r--  2.0 unx      799 b- defN 23-May-25 13:35 odoo/addons/aresta/__manifest__.py
 -rw-r--r--  2.0 unx     2961 b- defN 22-Nov-18 09:16 odoo/addons/aresta/i18n/ca_ES.po
 -rw-r--r--  2.0 unx     2940 b- defN 22-Nov-18 09:16 odoo/addons/aresta/i18n/es.po
 -rw-r--r--  2.0 unx       25 b- defN 22-May-18 16:43 odoo/addons/aresta/models/__init__.py
--rw-r--r--  2.0 unx     1162 b- defN 22-Jul-18 15:02 odoo/addons/aresta/models/sale_order.py
+-rw-r--r--  2.0 unx     1142 b- defN 23-May-25 13:13 odoo/addons/aresta/models/sale_order.py
 -rw-r--r--  2.0 unx       26 b- defN 22-May-18 16:43 odoo/addons/aresta/report/__init__.py
 -rw-r--r--  2.0 unx      923 b- defN 22-Nov-18 09:16 odoo/addons/aresta/report/delivery_note_mail_template.xml
 -rw-r--r--  2.0 unx      430 b- defN 22-Sep-13 08:41 odoo/addons/aresta/report/sale_report.py
 -rw-r--r--  2.0 unx      651 b- defN 22-May-18 16:43 odoo/addons/aresta/report/stock_report_deliveryslip.xml
 -rw-r--r--  2.0 unx      531 b- defN 22-Nov-18 09:16 odoo/addons/aresta/report/stock_report_views.xml
 -rw-r--r--  2.0 unx     1042 b- defN 22-May-18 16:43 odoo/addons/aresta/views/sale_order.xml
 -rw-r--r--  2.0 unx      619 b- defN 22-May-18 16:43 odoo/addons/aresta/views/sale_report.xml
 -rw-r--r--  2.0 unx       66 b- defN 22-Nov-18 09:16 odoo/addons/aresta/wizards/__init__.py
 -rw-r--r--  2.0 unx       33 b- defN 22-May-23 15:44 odoo/addons/aresta/wizards/confirm_sale_order/__init__.py
--rw-r--r--  2.0 unx      570 b- defN 22-May-23 15:44 odoo/addons/aresta/wizards/confirm_sale_order/confirm_sale_order.py
--rw-r--r--  2.0 unx      987 b- defN 22-May-23 15:44 odoo/addons/aresta/wizards/confirm_sale_order/confirm_sale_order.xml
+-rw-r--r--  2.0 unx      552 b- defN 23-May-25 13:33 odoo/addons/aresta/wizards/confirm_sale_order/confirm_sale_order.py
+-rw-r--r--  2.0 unx      987 b- defN 23-May-25 13:22 odoo/addons/aresta/wizards/confirm_sale_order/confirm_sale_order.xml
 -rw-r--r--  2.0 unx       33 b- defN 22-Nov-18 09:16 odoo/addons/aresta/wizards/send_delivery_note/__init__.py
 -rw-r--r--  2.0 unx     1528 b- defN 22-Nov-18 09:16 odoo/addons/aresta/wizards/send_delivery_note/send_delivery_note.py
 -rw-r--r--  2.0 unx     1628 b- defN 22-Nov-18 09:16 odoo/addons/aresta/wizards/send_delivery_note/send_delivery_note.xml
--rw-r--r--  2.0 unx      517 b- defN 23-May-22 05:31 odoo14_addon_aresta-14.0.1.0.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-22 05:31 odoo14_addon_aresta-14.0.1.0.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 23-May-22 05:31 odoo14_addon_aresta-14.0.1.0.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     2423 b- defN 23-May-22 05:31 odoo14_addon_aresta-14.0.1.0.0.dist-info/RECORD
-24 files, 20055 bytes uncompressed, 7916 bytes compressed:  60.5%
+-rw-r--r--  2.0 unx      517 b- defN 23-May-25 13:36 odoo14_addon_aresta-14.0.1.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-25 13:36 odoo14_addon_aresta-14.0.1.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 23-May-25 13:36 odoo14_addon_aresta-14.0.1.0.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     2423 b- defN 23-May-25 13:36 odoo14_addon_aresta-14.0.1.0.2.dist-info/RECORD
+24 files, 20017 bytes uncompressed, 7901 bytes compressed:  60.5%
```

## zipnote {}

```diff
@@ -54,20 +54,20 @@
 
 Filename: odoo/addons/aresta/wizards/send_delivery_note/send_delivery_note.py
 Comment: 
 
 Filename: odoo/addons/aresta/wizards/send_delivery_note/send_delivery_note.xml
 Comment: 
 
-Filename: odoo14_addon_aresta-14.0.1.0.0.dist-info/METADATA
+Filename: odoo14_addon_aresta-14.0.1.0.2.dist-info/METADATA
 Comment: 
 
-Filename: odoo14_addon_aresta-14.0.1.0.0.dist-info/WHEEL
+Filename: odoo14_addon_aresta-14.0.1.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: odoo14_addon_aresta-14.0.1.0.0.dist-info/top_level.txt
+Filename: odoo14_addon_aresta-14.0.1.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo14_addon_aresta-14.0.1.0.0.dist-info/RECORD
+Filename: odoo14_addon_aresta-14.0.1.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## odoo/addons/aresta/__manifest__.py

```diff
@@ -1,10 +1,10 @@
 {
     "name": "Odoo customizations for Aresta",
-    "version": "14.0.1.0.0",
+    "version": "14.0.1.0.2",
     "depends": [
         "delivery",
         "pos_order_to_sale_order",
         "pos_sale",
         "sale",
         "website_sale",
     ],
```

## odoo/addons/aresta/models/sale_order.py

```diff
@@ -1,23 +1,22 @@
-from odoo import fields, models, api
+from odoo import fields, models
 
 
 class SaleOrder(models.Model):
     _inherit = 'sale.order'
 
     # Field used on sale reports pivot view
     pos_name = fields.Char()
 
     # Field shown on sales view in order to facilitate all sale points
     pos_id = fields.Many2one(
         'pos.config',
         string='POS name'
     )
 
-    @api.model
     def _prepare_from_pos(self, order_data):
         vals = super()._prepare_from_pos(order_data)
 
         res_partner = self.env['res.partner'].search([
             ('id', '=', vals["partner_id"])
         ])
         carrier_id = res_partner.property_delivery_carrier_id.id
```

## odoo/addons/aresta/wizards/confirm_sale_order/confirm_sale_order.py

```diff
@@ -1,15 +1,14 @@
-from odoo import fields, models, _, api
+from odoo import fields, models, api
 
 
 class ConfirmSaleOrderWizard(models.TransientModel):
     _name = 'confirm.sale.order.wizard'
     sale_order_ids = fields.Many2many('sale.order')
 
-    @api.multi
     def button_confirm(self):
         for order in self.sale_order_ids:
             order.action_confirm()
         return True
 
     @api.model
     def default_get(self, fields_list):
```

## Comparing `odoo14_addon_aresta-14.0.1.0.0.dist-info/METADATA` & `odoo14_addon_aresta-14.0.1.0.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo14-addon-aresta
-Version: 14.0.1.0.0
+Version: 14.0.1.0.2
 Summary: Odoo customizations for Aresta.
 Home-page: https://coopdevs.org
 Author: Coopdevs Treball SCCL
 License: AGPL-3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
```

## Comparing `odoo14_addon_aresta-14.0.1.0.0.dist-info/RECORD` & `odoo14_addon_aresta-14.0.1.0.2.dist-info/RECORD`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 odoo/addons/aresta/__init__.py,sha256=_VLgEjYAhyqNIDKrTT30DsZQunCJnNimROSWiqXsfgA,64
-odoo/addons/aresta/__manifest__.py,sha256=yKohH7hxgyhqY8Rjjvoq2HNaKuKtnQdokRGFlTlA39g,799
+odoo/addons/aresta/__manifest__.py,sha256=k1RR-IrLnVVeroKY9mlKc_5RCpOJ-vm-ekXdxMUtwvY,799
 odoo/addons/aresta/i18n/ca_ES.po,sha256=Ps-QK15EweUcSZq0_Tan-czgvN9xyKmvsOaBQeqsLkc,2961
 odoo/addons/aresta/i18n/es.po,sha256=8fRylQ-j0v-mg15PaJKdMlhBznFeAezBe_5kAkDsG88,2940
 odoo/addons/aresta/models/__init__.py,sha256=LsPoCIAYodIFzh85VEjY5GiuzDQDQpiF38txDw10qT0,25
-odoo/addons/aresta/models/sale_order.py,sha256=MPW2DYUXRs6dN0eSMzBakNAo5f3oUs2TTBpfVb7e0OM,1162
+odoo/addons/aresta/models/sale_order.py,sha256=8fuCpYQZ2gpla3xMyMp2iI0cx6rQ1jCJaOx_NGrhwHk,1142
 odoo/addons/aresta/report/__init__.py,sha256=ByYRbiCY7uWnvbKwYusgp99HtcOyGnzWogDif_GEsec,26
 odoo/addons/aresta/report/delivery_note_mail_template.xml,sha256=gLC3-5JRUL4JoFEznN3vAOOeN4e9Dt7pOUZBgGH4kWk,923
 odoo/addons/aresta/report/sale_report.py,sha256=zQVZCKJKjKY7NDXIHcWfBNZQ0D2JBjAmfrBYhv7-Wpw,430
 odoo/addons/aresta/report/stock_report_deliveryslip.xml,sha256=DyFRwUY7NmyRscBqGQOJjvuhO09NNeGgZkA7-TSdVVM,651
 odoo/addons/aresta/report/stock_report_views.xml,sha256=Ax7V7KdNg4KPGDx4b09nAHViUpSS3L0Q4guGKMxFRAY,531
 odoo/addons/aresta/views/sale_order.xml,sha256=DTszDMUS0EjBFWKiurkINbUqiFmsY-hp60PG4eBm5d4,1042
 odoo/addons/aresta/views/sale_report.xml,sha256=5Ua_HuCtegqfGqyOazXq3bYMW0rcq11PkUue8moGrMU,619
 odoo/addons/aresta/wizards/__init__.py,sha256=ty9RulJBonHhEOBb1F-zhneH9Ypo_XpD47N0dRCXg7o,66
 odoo/addons/aresta/wizards/confirm_sale_order/__init__.py,sha256=eJHLMK9ZPgK7VA4_UMkfw9QFWJj3vRFUqFBWghnl2PE,33
-odoo/addons/aresta/wizards/confirm_sale_order/confirm_sale_order.py,sha256=Dwe_WvSkug5FFtP0MTJBkuyNU2LT6-EfO__6x3zowio,570
+odoo/addons/aresta/wizards/confirm_sale_order/confirm_sale_order.py,sha256=Vbs496-dsazl9tMLEoxl1UoWj0cyZktmjNubkv19fl0,552
 odoo/addons/aresta/wizards/confirm_sale_order/confirm_sale_order.xml,sha256=N4esiUT8w8jld83XWChaFcqvIC8dJ1nZDkqnmH12SIg,987
 odoo/addons/aresta/wizards/send_delivery_note/__init__.py,sha256=u-kmnLsZfAlSKS5c8kdBTqh2vRBstgY7PU_xpUYQx7w,33
 odoo/addons/aresta/wizards/send_delivery_note/send_delivery_note.py,sha256=kH1iELSKkqCLBF8XDZAiSgPIW6Vy_mRCPog_y8OH4cI,1528
 odoo/addons/aresta/wizards/send_delivery_note/send_delivery_note.xml,sha256=LofHOhJIYuf-KEjTUcFDIWOUX6tcaT3AJQPjBzCc7MI,1628
-odoo14_addon_aresta-14.0.1.0.0.dist-info/METADATA,sha256=LxmRKTmJj4pGpPwypdZtc8c189TKMARNefwjK7dLbH8,517
-odoo14_addon_aresta-14.0.1.0.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-odoo14_addon_aresta-14.0.1.0.0.dist-info/top_level.txt,sha256=qBj40grFkGOfDZ2WDSw3y1RnDlgG0u8rP8pvGNdbz4w,5
-odoo14_addon_aresta-14.0.1.0.0.dist-info/RECORD,,
+odoo14_addon_aresta-14.0.1.0.2.dist-info/METADATA,sha256=WOJNT7Ws1v7Rktng5d8zoLcbET99S2RbY8K69ehn9W0,517
+odoo14_addon_aresta-14.0.1.0.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+odoo14_addon_aresta-14.0.1.0.2.dist-info/top_level.txt,sha256=qBj40grFkGOfDZ2WDSw3y1RnDlgG0u8rP8pvGNdbz4w,5
+odoo14_addon_aresta-14.0.1.0.2.dist-info/RECORD,,
```

