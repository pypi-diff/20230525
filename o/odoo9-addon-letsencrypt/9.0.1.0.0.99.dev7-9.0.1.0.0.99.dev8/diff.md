# Comparing `tmp/odoo9_addon_letsencrypt-9.0.1.0.0.99.dev7-py2-none-any.whl.zip` & `tmp/odoo9_addon_letsencrypt-9.0.1.0.0.99.dev8-py2-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,42 +1,77 @@
-Zip file size: 34952 bytes, number of entries: 40
--rw-r--r--  2.0 unx      320 b- defN 16-Oct-10 14:03 odoo9_addon_letsencrypt-9.0.1.0.0.99.dev7-py2.7-nspkg.pth
--rw-r--r--  2.0 unx      806 b- defN 16-Oct-10 14:03 odoo_addons/letsencrypt/__openerp__.py
+Zip file size: 64881 bytes, number of entries: 75
+-rw-r--r--  2.0 unx      320 b- defN 16-Nov-30 03:36 odoo9_addon_letsencrypt-9.0.1.0.0.99.dev8-py2.7-nspkg.pth
+-rw-r--r--  2.0 unx       12 b- defN 16-Nov-30 03:36 odoo9_addon_letsencrypt-9.0.1.0.0.99.dev8.dist-info/top_level.txt
+-rw-r--r--  2.0 unx       92 b- defN 16-Nov-30 03:36 odoo9_addon_letsencrypt-9.0.1.0.0.99.dev8.dist-info/WHEEL
+-rw-r--r--  2.0 unx     7231 b- defN 17-Apr-08 19:10 odoo9_addon_letsencrypt-9.0.1.0.0.99.dev8.dist-info/RECORD
+-rw-r--r--  2.0 unx      675 b- defN 17-Apr-08 19:10 odoo9_addon_letsencrypt-9.0.1.0.0.99.dev8.dist-info/metadata.json
+-rw-r--r--  2.0 unx     5641 b- defN 16-Nov-30 03:36 odoo9_addon_letsencrypt-9.0.1.0.0.99.dev8.dist-info/DESCRIPTION.rst
+-rw-r--r--  2.0 unx     6165 b- defN 17-Apr-08 19:10 odoo9_addon_letsencrypt-9.0.1.0.0.99.dev8.dist-info/METADATA
+-rw-r--r--  2.0 unx       12 b- defN 16-Nov-30 03:36 odoo9_addon_letsencrypt-9.0.1.0.0.99.dev8.dist-info/namespace_packages.txt
+-rw-r--r--  2.0 unx      806 b- defN 16-Nov-30 03:36 odoo_addons/letsencrypt/__openerp__.py
 -rw-r--r--  2.0 unx      294 b- defN 16-May-26 02:39 odoo_addons/letsencrypt/hooks.py
 -rw-r--r--  2.0 unx      211 b- defN 16-May-26 02:39 odoo_addons/letsencrypt/__init__.py
--rw-r--r--  2.0 unx     5639 b- defN 16-Oct-07 14:39 odoo_addons/letsencrypt/README.rst
+-rw-r--r--  2.0 unx     5639 b- defN 16-Nov-30 03:34 odoo_addons/letsencrypt/README.rst
 -rw-r--r--  2.0 unx     6190 b- defN 16-May-26 02:39 odoo_addons/letsencrypt/models/letsencrypt.py
 -rw-r--r--  2.0 unx      156 b- defN 16-May-26 02:39 odoo_addons/letsencrypt/models/__init__.py
--rw-r--r--  2.0 unx     1583 b- defN 16-Oct-10 14:03 odoo_addons/letsencrypt/i18n/zh_CN.po
--rw-r--r--  2.0 unx     1453 b- defN 16-Oct-07 14:39 odoo_addons/letsencrypt/i18n/pt.po
--rw-r--r--  2.0 unx     1488 b- defN 16-Oct-07 14:39 odoo_addons/letsencrypt/i18n/it.po
--rw-r--r--  2.0 unx     1494 b- defN 16-Oct-07 14:39 odoo_addons/letsencrypt/i18n/es.po
--rw-r--r--  2.0 unx     1449 b- defN 16-Oct-07 14:39 odoo_addons/letsencrypt/i18n/tr.po
--rw-r--r--  2.0 unx     1747 b- defN 16-Oct-10 14:03 odoo_addons/letsencrypt/i18n/hr.po
--rw-r--r--  2.0 unx     1490 b- defN 16-Oct-10 14:03 odoo_addons/letsencrypt/i18n/bg.po
--rw-r--r--  2.0 unx     1451 b- defN 16-Oct-07 14:39 odoo_addons/letsencrypt/i18n/gl.po
--rw-r--r--  2.0 unx     1450 b- defN 16-Oct-07 14:39 odoo_addons/letsencrypt/i18n/ca.po
--rw-r--r--  2.0 unx     1539 b- defN 16-Oct-07 14:39 odoo_addons/letsencrypt/i18n/sl.po
--rw-r--r--  2.0 unx     1479 b- defN 16-Oct-07 14:39 odoo_addons/letsencrypt/i18n/nl.po
--rw-r--r--  2.0 unx     1449 b- defN 16-Oct-07 14:39 odoo_addons/letsencrypt/i18n/am.po
--rw-r--r--  2.0 unx     1480 b- defN 16-Oct-07 14:39 odoo_addons/letsencrypt/i18n/de.po
--rw-r--r--  2.0 unx     1488 b- defN 16-Oct-07 14:39 odoo_addons/letsencrypt/i18n/fr.po
--rw-r--r--  2.0 unx     1521 b- defN 16-Oct-07 14:39 odoo_addons/letsencrypt/i18n/pt_BR.po
--rw-r--r--  2.0 unx     1475 b- defN 16-Oct-07 14:39 odoo_addons/letsencrypt/i18n/el_GR.po
--rw-r--r--  2.0 unx     1471 b- defN 16-Oct-07 14:39 odoo_addons/letsencrypt/i18n/fi.po
--rw-r--r--  2.0 unx     1563 b- defN 16-Oct-07 14:39 odoo_addons/letsencrypt/i18n/hr_HR.po
+-rw-r--r--  2.0 unx     1468 b- defN 16-Nov-30 03:36 odoo_addons/letsencrypt/i18n/ja.po
+-rw-r--r--  2.0 unx     1485 b- defN 16-Nov-30 03:36 odoo_addons/letsencrypt/i18n/lv.po
+-rw-r--r--  2.0 unx     1583 b- defN 16-Nov-30 03:36 odoo_addons/letsencrypt/i18n/zh_CN.po
+-rw-r--r--  2.0 unx     1605 b- defN 16-Nov-30 03:36 odoo_addons/letsencrypt/i18n/uk.po
+-rw-r--r--  2.0 unx     1506 b- defN 16-Nov-30 03:36 odoo_addons/letsencrypt/i18n/es_AR.po
+-rw-r--r--  2.0 unx     1468 b- defN 16-Nov-30 03:36 odoo_addons/letsencrypt/i18n/ko.po
+-rw-r--r--  2.0 unx     1465 b- defN 16-Nov-30 03:36 odoo_addons/letsencrypt/i18n/gl_ES.po
+-rw-r--r--  2.0 unx     1485 b- defN 16-Nov-30 03:36 odoo_addons/letsencrypt/i18n/pt.po
+-rw-r--r--  2.0 unx     1468 b- defN 16-Nov-30 03:36 odoo_addons/letsencrypt/i18n/fr_CH.po
+-rw-r--r--  2.0 unx     1488 b- defN 16-Nov-30 03:34 odoo_addons/letsencrypt/i18n/it.po
+-rw-r--r--  2.0 unx     1494 b- defN 16-Nov-30 03:34 odoo_addons/letsencrypt/i18n/es.po
+-rw-r--r--  2.0 unx     1493 b- defN 16-Nov-30 03:36 odoo_addons/letsencrypt/i18n/nl_BE.po
+-rw-r--r--  2.0 unx     1581 b- defN 16-Nov-30 03:36 odoo_addons/letsencrypt/i18n/ar.po
+-rw-r--r--  2.0 unx     1564 b- defN 16-Nov-30 03:36 odoo_addons/letsencrypt/i18n/lt.po
+-rw-r--r--  2.0 unx     1449 b- defN 16-Nov-30 03:34 odoo_addons/letsencrypt/i18n/tr.po
+-rw-r--r--  2.0 unx     1467 b- defN 16-Nov-30 03:36 odoo_addons/letsencrypt/i18n/es_PY.po
+-rw-r--r--  2.0 unx     1540 b- defN 16-Nov-30 03:36 odoo_addons/letsencrypt/i18n/mk.po
+-rw-r--r--  2.0 unx     1747 b- defN 16-Nov-30 03:36 odoo_addons/letsencrypt/i18n/hr.po
+-rw-r--r--  2.0 unx     1520 b- defN 16-Nov-30 03:36 odoo_addons/letsencrypt/i18n/bg.po
+-rw-r--r--  2.0 unx     1523 b- defN 16-Nov-30 03:36 odoo_addons/letsencrypt/i18n/es_EC.po
+-rw-r--r--  2.0 unx     1487 b- defN 16-Nov-30 03:36 odoo_addons/letsencrypt/i18n/zh_TW.po
+-rw-r--r--  2.0 unx     1472 b- defN 16-Nov-30 03:36 odoo_addons/letsencrypt/i18n/gl.po
+-rw-r--r--  2.0 unx     1450 b- defN 16-Nov-30 03:34 odoo_addons/letsencrypt/i18n/ca.po
+-rw-r--r--  2.0 unx     1469 b- defN 16-Nov-30 03:36 odoo_addons/letsencrypt/i18n/es_CR.po
+-rw-r--r--  2.0 unx     1504 b- defN 16-Nov-30 03:36 odoo_addons/letsencrypt/i18n/he.po
+-rw-r--r--  2.0 unx     1506 b- defN 16-Nov-30 03:36 odoo_addons/letsencrypt/i18n/es_CO.po
+-rw-r--r--  2.0 unx     1539 b- defN 16-Nov-30 03:34 odoo_addons/letsencrypt/i18n/sl.po
+-rw-r--r--  2.0 unx     1571 b- defN 16-Nov-30 03:36 odoo_addons/letsencrypt/i18n/sr@latin.po
+-rw-r--r--  2.0 unx     1558 b- defN 16-Nov-30 03:36 odoo_addons/letsencrypt/i18n/th.po
+-rw-r--r--  2.0 unx     1502 b- defN 16-Nov-30 03:36 odoo_addons/letsencrypt/i18n/es_PE.po
+-rw-r--r--  2.0 unx     1511 b- defN 16-Nov-30 03:36 odoo_addons/letsencrypt/i18n/cs.po
+-rw-r--r--  2.0 unx     1511 b- defN 16-Nov-30 03:36 odoo_addons/letsencrypt/i18n/pt_PT.po
+-rw-r--r--  2.0 unx     1463 b- defN 16-Nov-30 03:36 odoo_addons/letsencrypt/i18n/eu.po
+-rw-r--r--  2.0 unx     1488 b- defN 16-Nov-30 03:36 odoo_addons/letsencrypt/i18n/nb.po
+-rw-r--r--  2.0 unx     1475 b- defN 16-Nov-30 03:36 odoo_addons/letsencrypt/i18n/da.po
+-rw-r--r--  2.0 unx     1481 b- defN 16-Nov-30 03:36 odoo_addons/letsencrypt/i18n/et.po
+-rw-r--r--  2.0 unx     1528 b- defN 16-Nov-30 03:36 odoo_addons/letsencrypt/i18n/mn.po
+-rw-r--r--  2.0 unx     1481 b- defN 16-Nov-30 03:36 odoo_addons/letsencrypt/i18n/nl.po
+-rw-r--r--  2.0 unx     1449 b- defN 16-Nov-30 03:34 odoo_addons/letsencrypt/i18n/am.po
+-rw-r--r--  2.0 unx     1480 b- defN 16-Nov-30 03:34 odoo_addons/letsencrypt/i18n/de.po
+-rw-r--r--  2.0 unx     1486 b- defN 16-Nov-30 03:36 odoo_addons/letsencrypt/i18n/vi.po
+-rw-r--r--  2.0 unx     1488 b- defN 16-Nov-30 03:34 odoo_addons/letsencrypt/i18n/fr.po
+-rw-r--r--  2.0 unx     1515 b- defN 16-Nov-30 03:36 odoo_addons/letsencrypt/i18n/fa.po
+-rw-r--r--  2.0 unx     1554 b- defN 16-Nov-30 03:36 odoo_addons/letsencrypt/i18n/bs.po
+-rw-r--r--  2.0 unx     1521 b- defN 16-Nov-30 03:34 odoo_addons/letsencrypt/i18n/pt_BR.po
+-rw-r--r--  2.0 unx     1501 b- defN 16-Nov-30 03:36 odoo_addons/letsencrypt/i18n/en_GB.po
+-rw-r--r--  2.0 unx     1475 b- defN 16-Nov-30 03:34 odoo_addons/letsencrypt/i18n/el_GR.po
+-rw-r--r--  2.0 unx     1508 b- defN 16-Nov-30 03:36 odoo_addons/letsencrypt/i18n/es_VE.po
+-rw-r--r--  2.0 unx     1511 b- defN 16-Nov-30 03:36 odoo_addons/letsencrypt/i18n/es_MX.po
+-rw-r--r--  2.0 unx     1475 b- defN 16-Nov-30 03:36 odoo_addons/letsencrypt/i18n/sv.po
+-rw-r--r--  2.0 unx     1512 b- defN 16-Nov-30 03:36 odoo_addons/letsencrypt/i18n/sk.po
+-rw-r--r--  2.0 unx     1471 b- defN 16-Nov-30 03:34 odoo_addons/letsencrypt/i18n/fi.po
+-rw-r--r--  2.0 unx     1563 b- defN 16-Nov-30 03:34 odoo_addons/letsencrypt/i18n/hr_HR.po
 -rw-r--r--  2.0 unx      656 b- defN 16-May-26 02:39 odoo_addons/letsencrypt/controllers/main.py
 -rw-r--r--  2.0 unx      149 b- defN 16-May-26 02:39 odoo_addons/letsencrypt/controllers/__init__.py
 -rw-r--r--  2.0 unx      435 b- defN 16-May-26 02:39 odoo_addons/letsencrypt/data/ir_config_parameter.xml
 -rw-r--r--  2.0 unx      540 b- defN 16-May-26 02:39 odoo_addons/letsencrypt/data/ir_cron.xml
 -rw-r--r--  2.0 unx      516 b- defN 16-May-26 02:39 odoo_addons/letsencrypt/tests/test_letsencrypt.py
 -rw-r--r--  2.0 unx      161 b- defN 16-May-26 02:39 odoo_addons/letsencrypt/tests/__init__.py
--rw-r--r--  2.0 unx      196 b- defN 16-Oct-07 14:39 odoo_addons/letsencrypt/demo/ir_cron.xml
+-rw-r--r--  2.0 unx      196 b- defN 16-Nov-30 03:34 odoo_addons/letsencrypt/demo/ir_cron.xml
 -rw-r--r--  2.0 unx     2157 b- defN 16-May-26 02:39 odoo_addons/letsencrypt/static/description/icon.png
--rw-r--r--  2.0 unx       12 b- defN 16-Oct-10 14:03 odoo9_addon_letsencrypt-9.0.1.0.0.99.dev7.dist-info/top_level.txt
--rw-r--r--  2.0 unx       92 b- defN 16-Oct-10 14:03 odoo9_addon_letsencrypt-9.0.1.0.0.99.dev7.dist-info/WHEEL
--rw-r--r--  2.0 unx     3963 b- defN 17-Apr-08 19:14 odoo9_addon_letsencrypt-9.0.1.0.0.99.dev7.dist-info/RECORD
--rw-r--r--  2.0 unx      539 b- defN 17-Apr-08 19:14 odoo9_addon_letsencrypt-9.0.1.0.0.99.dev7.dist-info/metadata.json
--rw-r--r--  2.0 unx     5641 b- defN 16-Oct-10 14:03 odoo9_addon_letsencrypt-9.0.1.0.0.99.dev7.dist-info/DESCRIPTION.rst
--rw-r--r--  2.0 unx     6102 b- defN 17-Apr-08 19:14 odoo9_addon_letsencrypt-9.0.1.0.0.99.dev7.dist-info/METADATA
--rw-r--r--  2.0 unx       12 b- defN 16-Oct-10 14:03 odoo9_addon_letsencrypt-9.0.1.0.0.99.dev7.dist-info/namespace_packages.txt
-40 files, 61857 bytes uncompressed, 28458 bytes compressed:  54.0%
+75 files, 118158 bytes uncompressed, 53251 bytes compressed:  54.9%
```

## zipnote {}

```diff
@@ -1,8 +1,29 @@
-Filename: odoo9_addon_letsencrypt-9.0.1.0.0.99.dev7-py2.7-nspkg.pth
+Filename: odoo9_addon_letsencrypt-9.0.1.0.0.99.dev8-py2.7-nspkg.pth
+Comment: 
+
+Filename: odoo9_addon_letsencrypt-9.0.1.0.0.99.dev8.dist-info/top_level.txt
+Comment: 
+
+Filename: odoo9_addon_letsencrypt-9.0.1.0.0.99.dev8.dist-info/WHEEL
+Comment: 
+
+Filename: odoo9_addon_letsencrypt-9.0.1.0.0.99.dev8.dist-info/RECORD
+Comment: 
+
+Filename: odoo9_addon_letsencrypt-9.0.1.0.0.99.dev8.dist-info/metadata.json
+Comment: 
+
+Filename: odoo9_addon_letsencrypt-9.0.1.0.0.99.dev8.dist-info/DESCRIPTION.rst
+Comment: 
+
+Filename: odoo9_addon_letsencrypt-9.0.1.0.0.99.dev8.dist-info/METADATA
+Comment: 
+
+Filename: odoo9_addon_letsencrypt-9.0.1.0.0.99.dev8.dist-info/namespace_packages.txt
 Comment: 
 
 Filename: odoo_addons/letsencrypt/__openerp__.py
 Comment: 
 
 Filename: odoo_addons/letsencrypt/hooks.py
 Comment: 
@@ -15,107 +36,191 @@
 
 Filename: odoo_addons/letsencrypt/models/letsencrypt.py
 Comment: 
 
 Filename: odoo_addons/letsencrypt/models/__init__.py
 Comment: 
 
+Filename: odoo_addons/letsencrypt/i18n/ja.po
+Comment: 
+
+Filename: odoo_addons/letsencrypt/i18n/lv.po
+Comment: 
+
 Filename: odoo_addons/letsencrypt/i18n/zh_CN.po
 Comment: 
 
+Filename: odoo_addons/letsencrypt/i18n/uk.po
+Comment: 
+
+Filename: odoo_addons/letsencrypt/i18n/es_AR.po
+Comment: 
+
+Filename: odoo_addons/letsencrypt/i18n/ko.po
+Comment: 
+
+Filename: odoo_addons/letsencrypt/i18n/gl_ES.po
+Comment: 
+
 Filename: odoo_addons/letsencrypt/i18n/pt.po
 Comment: 
 
+Filename: odoo_addons/letsencrypt/i18n/fr_CH.po
+Comment: 
+
 Filename: odoo_addons/letsencrypt/i18n/it.po
 Comment: 
 
 Filename: odoo_addons/letsencrypt/i18n/es.po
 Comment: 
 
+Filename: odoo_addons/letsencrypt/i18n/nl_BE.po
+Comment: 
+
+Filename: odoo_addons/letsencrypt/i18n/ar.po
+Comment: 
+
+Filename: odoo_addons/letsencrypt/i18n/lt.po
+Comment: 
+
 Filename: odoo_addons/letsencrypt/i18n/tr.po
 Comment: 
 
+Filename: odoo_addons/letsencrypt/i18n/es_PY.po
+Comment: 
+
+Filename: odoo_addons/letsencrypt/i18n/mk.po
+Comment: 
+
 Filename: odoo_addons/letsencrypt/i18n/hr.po
 Comment: 
 
 Filename: odoo_addons/letsencrypt/i18n/bg.po
 Comment: 
 
+Filename: odoo_addons/letsencrypt/i18n/es_EC.po
+Comment: 
+
+Filename: odoo_addons/letsencrypt/i18n/zh_TW.po
+Comment: 
+
 Filename: odoo_addons/letsencrypt/i18n/gl.po
 Comment: 
 
 Filename: odoo_addons/letsencrypt/i18n/ca.po
 Comment: 
 
+Filename: odoo_addons/letsencrypt/i18n/es_CR.po
+Comment: 
+
+Filename: odoo_addons/letsencrypt/i18n/he.po
+Comment: 
+
+Filename: odoo_addons/letsencrypt/i18n/es_CO.po
+Comment: 
+
 Filename: odoo_addons/letsencrypt/i18n/sl.po
 Comment: 
 
+Filename: odoo_addons/letsencrypt/i18n/sr@latin.po
+Comment: 
+
+Filename: odoo_addons/letsencrypt/i18n/th.po
+Comment: 
+
+Filename: odoo_addons/letsencrypt/i18n/es_PE.po
+Comment: 
+
+Filename: odoo_addons/letsencrypt/i18n/cs.po
+Comment: 
+
+Filename: odoo_addons/letsencrypt/i18n/pt_PT.po
+Comment: 
+
+Filename: odoo_addons/letsencrypt/i18n/eu.po
+Comment: 
+
+Filename: odoo_addons/letsencrypt/i18n/nb.po
+Comment: 
+
+Filename: odoo_addons/letsencrypt/i18n/da.po
+Comment: 
+
+Filename: odoo_addons/letsencrypt/i18n/et.po
+Comment: 
+
+Filename: odoo_addons/letsencrypt/i18n/mn.po
+Comment: 
+
 Filename: odoo_addons/letsencrypt/i18n/nl.po
 Comment: 
 
 Filename: odoo_addons/letsencrypt/i18n/am.po
 Comment: 
 
 Filename: odoo_addons/letsencrypt/i18n/de.po
 Comment: 
 
+Filename: odoo_addons/letsencrypt/i18n/vi.po
+Comment: 
+
 Filename: odoo_addons/letsencrypt/i18n/fr.po
 Comment: 
 
-Filename: odoo_addons/letsencrypt/i18n/pt_BR.po
+Filename: odoo_addons/letsencrypt/i18n/fa.po
 Comment: 
 
-Filename: odoo_addons/letsencrypt/i18n/el_GR.po
+Filename: odoo_addons/letsencrypt/i18n/bs.po
 Comment: 
 
-Filename: odoo_addons/letsencrypt/i18n/fi.po
+Filename: odoo_addons/letsencrypt/i18n/pt_BR.po
 Comment: 
 
-Filename: odoo_addons/letsencrypt/i18n/hr_HR.po
+Filename: odoo_addons/letsencrypt/i18n/en_GB.po
 Comment: 
 
-Filename: odoo_addons/letsencrypt/controllers/main.py
+Filename: odoo_addons/letsencrypt/i18n/el_GR.po
 Comment: 
 
-Filename: odoo_addons/letsencrypt/controllers/__init__.py
+Filename: odoo_addons/letsencrypt/i18n/es_VE.po
 Comment: 
 
-Filename: odoo_addons/letsencrypt/data/ir_config_parameter.xml
+Filename: odoo_addons/letsencrypt/i18n/es_MX.po
 Comment: 
 
-Filename: odoo_addons/letsencrypt/data/ir_cron.xml
+Filename: odoo_addons/letsencrypt/i18n/sv.po
 Comment: 
 
-Filename: odoo_addons/letsencrypt/tests/test_letsencrypt.py
+Filename: odoo_addons/letsencrypt/i18n/sk.po
 Comment: 
 
-Filename: odoo_addons/letsencrypt/tests/__init__.py
+Filename: odoo_addons/letsencrypt/i18n/fi.po
 Comment: 
 
-Filename: odoo_addons/letsencrypt/demo/ir_cron.xml
+Filename: odoo_addons/letsencrypt/i18n/hr_HR.po
 Comment: 
 
-Filename: odoo_addons/letsencrypt/static/description/icon.png
+Filename: odoo_addons/letsencrypt/controllers/main.py
 Comment: 
 
-Filename: odoo9_addon_letsencrypt-9.0.1.0.0.99.dev7.dist-info/top_level.txt
+Filename: odoo_addons/letsencrypt/controllers/__init__.py
 Comment: 
 
-Filename: odoo9_addon_letsencrypt-9.0.1.0.0.99.dev7.dist-info/WHEEL
+Filename: odoo_addons/letsencrypt/data/ir_config_parameter.xml
 Comment: 
 
-Filename: odoo9_addon_letsencrypt-9.0.1.0.0.99.dev7.dist-info/RECORD
+Filename: odoo_addons/letsencrypt/data/ir_cron.xml
 Comment: 
 
-Filename: odoo9_addon_letsencrypt-9.0.1.0.0.99.dev7.dist-info/metadata.json
+Filename: odoo_addons/letsencrypt/tests/test_letsencrypt.py
 Comment: 
 
-Filename: odoo9_addon_letsencrypt-9.0.1.0.0.99.dev7.dist-info/DESCRIPTION.rst
+Filename: odoo_addons/letsencrypt/tests/__init__.py
 Comment: 
 
-Filename: odoo9_addon_letsencrypt-9.0.1.0.0.99.dev7.dist-info/METADATA
+Filename: odoo_addons/letsencrypt/demo/ir_cron.xml
 Comment: 
 
-Filename: odoo9_addon_letsencrypt-9.0.1.0.0.99.dev7.dist-info/namespace_packages.txt
+Filename: odoo_addons/letsencrypt/static/description/icon.png
 Comment: 
 
 Zip file comment:
```

## odoo_addons/letsencrypt/i18n/pt.po

```diff
@@ -3,15 +3,15 @@
 # * letsencrypt
 # 
 # Translators:
 msgid ""
 msgstr ""
 "Project-Id-Version: server-tools (9.0)\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2016-09-10 02:53+0000\n"
+"POT-Creation-Date: 2016-11-26 01:46+0000\n"
 "PO-Revision-Date: 2016-05-25 16:43+0000\n"
 "Last-Translator: <>\n"
 "Language-Team: Portuguese (http://www.transifex.com/oca/OCA-server-tools-9-0/language/pt/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: \n"
 "Language: pt\n"
@@ -21,15 +21,15 @@
 #: model:ir.model,name:letsencrypt.model_letsencrypt
 msgid "Abstract model providing functions for letsencrypt"
 msgstr ""
 
 #. module: letsencrypt
 #: model:ir.model.fields,field_description:letsencrypt.field_letsencrypt_display_name
 msgid "Display Name"
-msgstr ""
+msgstr "Nome"
 
 #. module: letsencrypt
 #: code:addons/letsencrypt/models/letsencrypt.py:44
 #, python-format
 msgid "Error calling %s: %d"
 msgstr ""
 
@@ -37,14 +37,14 @@
 #: model:ir.model.fields,field_description:letsencrypt.field_letsencrypt_id
 msgid "ID"
 msgstr "ID"
 
 #. module: letsencrypt
 #: model:ir.model.fields,field_description:letsencrypt.field_letsencrypt___last_update
 msgid "Last Modified on"
-msgstr ""
+msgstr "Modificado a última vez por"
 
 #. module: letsencrypt
 #: code:addons/letsencrypt/models/letsencrypt.py:93
 #, python-format
 msgid "Let's encrypt doesn't work with private addresses or local domains!"
 msgstr ""
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

## odoo_addons/letsencrypt/i18n/bg.po

```diff
@@ -3,15 +3,15 @@
 # * letsencrypt
 # 
 # Translators:
 msgid ""
 msgstr ""
 "Project-Id-Version: server-tools (9.0)\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2016-10-04 09:42+0000\n"
+"POT-Creation-Date: 2016-11-26 01:46+0000\n"
 "PO-Revision-Date: 2016-05-25 16:43+0000\n"
 "Last-Translator: <>\n"
 "Language-Team: Bulgarian (http://www.transifex.com/oca/OCA-server-tools-9-0/language/bg/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: \n"
 "Language: bg\n"
@@ -21,15 +21,15 @@
 #: model:ir.model,name:letsencrypt.model_letsencrypt
 msgid "Abstract model providing functions for letsencrypt"
 msgstr ""
 
 #. module: letsencrypt
 #: model:ir.model.fields,field_description:letsencrypt.field_letsencrypt_display_name
 msgid "Display Name"
-msgstr ""
+msgstr "Име за Показване"
 
 #. module: letsencrypt
 #: code:addons/letsencrypt/models/letsencrypt.py:44
 #, python-format
 msgid "Error calling %s: %d"
 msgstr ""
```

## odoo_addons/letsencrypt/i18n/gl.po

```diff
@@ -3,15 +3,15 @@
 # * letsencrypt
 # 
 # Translators:
 msgid ""
 msgstr ""
 "Project-Id-Version: server-tools (9.0)\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2016-09-10 02:53+0000\n"
+"POT-Creation-Date: 2016-11-26 01:46+0000\n"
 "PO-Revision-Date: 2016-05-25 16:43+0000\n"
 "Last-Translator: <>\n"
 "Language-Team: Galician (http://www.transifex.com/oca/OCA-server-tools-9-0/language/gl/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: \n"
 "Language: gl\n"
@@ -37,14 +37,14 @@
 #: model:ir.model.fields,field_description:letsencrypt.field_letsencrypt_id
 msgid "ID"
 msgstr "ID"
 
 #. module: letsencrypt
 #: model:ir.model.fields,field_description:letsencrypt.field_letsencrypt___last_update
 msgid "Last Modified on"
-msgstr ""
+msgstr "Última modificación"
 
 #. module: letsencrypt
 #: code:addons/letsencrypt/models/letsencrypt.py:93
 #, python-format
 msgid "Let's encrypt doesn't work with private addresses or local domains!"
 msgstr ""
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

## odoo_addons/letsencrypt/i18n/nl.po

```diff
@@ -3,15 +3,15 @@
 # * letsencrypt
 # 
 # Translators:
 msgid ""
 msgstr ""
 "Project-Id-Version: server-tools (9.0)\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2016-09-10 02:53+0000\n"
+"POT-Creation-Date: 2016-11-26 01:46+0000\n"
 "PO-Revision-Date: 2016-05-25 16:43+0000\n"
 "Last-Translator: <>\n"
 "Language-Team: Dutch (http://www.transifex.com/oca/OCA-server-tools-9-0/language/nl/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: \n"
 "Language: nl\n"
@@ -32,15 +32,15 @@
 #, python-format
 msgid "Error calling %s: %d"
 msgstr ""
 
 #. module: letsencrypt
 #: model:ir.model.fields,field_description:letsencrypt.field_letsencrypt_id
 msgid "ID"
-msgstr ""
+msgstr "ID"
 
 #. module: letsencrypt
 #: model:ir.model.fields,field_description:letsencrypt.field_letsencrypt___last_update
 msgid "Last Modified on"
 msgstr "Laatst bijgewerkt op"
 
 #. module: letsencrypt
```

## Comparing `odoo9_addon_letsencrypt-9.0.1.0.0.99.dev7.dist-info/DESCRIPTION.rst` & `odoo9_addon_letsencrypt-9.0.1.0.0.99.dev8.dist-info/DESCRIPTION.rst`

 * *Files identical despite different names*

## Comparing `odoo9_addon_letsencrypt-9.0.1.0.0.99.dev7.dist-info/METADATA` & `odoo9_addon_letsencrypt-9.0.1.0.0.99.dev8.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.0
 Name: odoo9-addon-letsencrypt
-Version: 9.0.1.0.0.99.dev7
+Version: 9.0.1.0.0.99.dev8
 Summary: Request SSL certificates from letsencrypt.org
 Home-page: UNKNOWN
-Author: UNKNOWN
-Author-email: UNKNOWN
+Author: Therp BV,Tecnativa,Odoo Community Association (OCA)
+Author-email: support@odoo-community.org
 License: AGPL-3
 Platform: UNKNOWN
 Requires-Dist: IPy
 Requires-Dist: acme-tiny
 Requires-Dist: odoo (<9.1a,>=9.0a)
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Framework :: Odoo
```

