# Comparing `tmp/mb_utils-1.0.202303150603-py3-none-any.whl.zip` & `tmp/mb_utils-1.0.202305250048-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 8243 bytes, number of entries: 15
--rw-rw-r--  2.0 unx      110 b- defN 22-Nov-18 19:19 mb_utils/src/__init__.py
+Zip file size: 8326 bytes, number of entries: 15
+-rw-rw-r--  2.0 unx      343 b- defN 23-May-25 00:34 mb_utils/src/__init__.py
 -rw-rw-r--  2.0 unx     3346 b- defN 22-Nov-19 01:53 mb_utils/src/deprecated.py
 -rw-rw-r--  2.0 unx      625 b- defN 23-Feb-14 19:50 mb_utils/src/edge_points_cron.py
 -rw-rw-r--  2.0 unx     1318 b- defN 22-Nov-20 04:18 mb_utils/src/extra.py
 -rw-rw-r--  2.0 unx     1813 b- defN 22-Nov-20 05:35 mb_utils/src/logging.py
 -rw-rw-r--  2.0 unx      664 b- defN 23-Mar-10 05:03 mb_utils/src/path_checker.py
 -rw-rw-r--  2.0 unx     1306 b- defN 22-Nov-19 01:51 mb_utils/src/retry_decorator.py
 -rw-rw-r--  2.0 unx     3073 b- defN 22-Nov-19 00:49 mb_utils/src/s3.py
 -rw-rw-r--  2.0 unx      777 b- defN 22-Nov-20 04:17 mb_utils/src/terminal.py
 -rw-rw-r--  2.0 unx     1821 b- defN 22-Nov-19 01:53 mb_utils/src/verify_image.py
--rw-rw-r--  2.0 unx      396 b- defN 23-Mar-15 06:03 mb_utils/src/version.py
--rw-rw-r--  2.0 unx      251 b- defN 23-Mar-15 06:03 mb_utils-1.0.202303150603.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Mar-15 06:03 mb_utils-1.0.202303150603.dist-info/WHEEL
--rw-rw-r--  2.0 unx        9 b- defN 23-Mar-15 06:03 mb_utils-1.0.202303150603.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1244 b- defN 23-Mar-15 06:03 mb_utils-1.0.202303150603.dist-info/RECORD
-15 files, 16845 bytes uncompressed, 6173 bytes compressed:  63.4%
+-rw-rw-r--  2.0 unx      396 b- defN 23-May-25 00:48 mb_utils/src/version.py
+-rw-rw-r--  2.0 unx      251 b- defN 23-May-25 00:49 mb_utils-1.0.202305250048.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-25 00:49 mb_utils-1.0.202305250048.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        9 b- defN 23-May-25 00:49 mb_utils-1.0.202305250048.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1244 b- defN 23-May-25 00:49 mb_utils-1.0.202305250048.dist-info/RECORD
+15 files, 17078 bytes uncompressed, 6256 bytes compressed:  63.4%
```

## zipnote {}

```diff
@@ -27,20 +27,20 @@
 
 Filename: mb_utils/src/verify_image.py
 Comment: 
 
 Filename: mb_utils/src/version.py
 Comment: 
 
-Filename: mb_utils-1.0.202303150603.dist-info/METADATA
+Filename: mb_utils-1.0.202305250048.dist-info/METADATA
 Comment: 
 
-Filename: mb_utils-1.0.202303150603.dist-info/WHEEL
+Filename: mb_utils-1.0.202305250048.dist-info/WHEEL
 Comment: 
 
-Filename: mb_utils-1.0.202303150603.dist-info/top_level.txt
+Filename: mb_utils-1.0.202305250048.dist-info/top_level.txt
 Comment: 
 
-Filename: mb_utils-1.0.202303150603.dist-info/RECORD
+Filename: mb_utils-1.0.202305250048.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mb_utils/src/__init__.py

```diff
@@ -1,3 +1,14 @@
 from .version import version
+from .deprecated import *
+from .edge_points_cron import *
+from .extra import *
+from .s3 import *
+from .terminal import *
+from .verify_image import *
+from .logging import *
+from .path_checker import *
+from .retry_decorator import *
+
+
 # import logging
 # logging.getLogger(__name__).addHandler(logging.NullHandler())
```

## mb_utils/src/version.py

```diff
@@ -1,11 +1,11 @@
 VERSION_YEAR = 2023
-VERSION_MONTH = int('03')
-VERSION_DAY = int('15')
-VERSION_HOUR = int('06')
-VERSION_MINUTE = int('03')
+VERSION_MONTH = int('05')
+VERSION_DAY = int('25')
+VERSION_HOUR = int('00')
+VERSION_MINUTE = int('48')
 MAJOR_VERSION = 1
 MINOR_VERSION = 0
-PATCH_VERSION = 202303150603
-version_date = '2023/03/15 06:03'
+PATCH_VERSION = 202305250048
+version_date = '2023/05/25 00:48'
 version = '{}.{}.{}'.format(MAJOR_VERSION, MINOR_VERSION, PATCH_VERSION)
 __all__  = ['MAJOR_VERSION', 'MINOR_VERSION', 'PATCH_VERSION', 'version_date', 'version']
```

## Comparing `mb_utils-1.0.202303150603.dist-info/RECORD` & `mb_utils-1.0.202305250048.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-mb_utils/src/__init__.py,sha256=UsjmVG5bbc3syW6rLQhQy9OAK_BCLUK44ldaB8leHDE,110
+mb_utils/src/__init__.py,sha256=z3wWkGLIjR8RrXsgRxLnKcq4QOaMY7-b0iqoE4Y9-VI,343
 mb_utils/src/deprecated.py,sha256=VOYR9hBLPDKFcc5Lyv-Zemy9E0_uGfaL_igGdWknci0,3346
 mb_utils/src/edge_points_cron.py,sha256=PfBj3_rYGU1oi2pRupg5xo8L8S8_A_zHGU0ZW7SWV8I,625
 mb_utils/src/extra.py,sha256=NP5JlU0oktw7j2cn_-W3rAMzjMYDKwzBeiSjpg-Evh4,1318
 mb_utils/src/logging.py,sha256=bwkKDej4pI1WzNKrQs9rTRx73z-EyZkB7UCPsYHnbs0,1813
 mb_utils/src/path_checker.py,sha256=MrE3P2hkDjOIWyZJ-Lh1X3wODKRnJk_nfVgKW0nQEMU,664
 mb_utils/src/retry_decorator.py,sha256=1lotNMXwALWFgb0ikrK9B-flOOMj9tTlOQgYCb-ejwY,1306
 mb_utils/src/s3.py,sha256=s-8K29xeRPomDy-RzT7Zu3s4-XHtIoCxatSg_vTzeuU,3073
 mb_utils/src/terminal.py,sha256=_1l8K9CwAFYx4UgfkwOWfgeZ2bZu4s-71gnyxWJc2xA,777
 mb_utils/src/verify_image.py,sha256=L_XAlYBsdAhTkMSVcMpgwS0Ea8I9r-ZjoChjL0GHT38,1821
-mb_utils/src/version.py,sha256=KmWIjjErGEcQiA7jBfaeF7RGABSHPiIN0Rpis9uUGIs,396
-mb_utils-1.0.202303150603.dist-info/METADATA,sha256=h70lEG-MR0nH3rw9Kjsl6C6PCAx1G6d6FHoCvvNGDOM,251
-mb_utils-1.0.202303150603.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-mb_utils-1.0.202303150603.dist-info/top_level.txt,sha256=xeK1qEZ7uoXfZyNlYlurb_F_T8trKUaTU_Fm_UpKhyg,9
-mb_utils-1.0.202303150603.dist-info/RECORD,,
+mb_utils/src/version.py,sha256=_JaVHK4ucEYDB55IslMDZzl3XvOBFpGG9CjFVPMqRFs,396
+mb_utils-1.0.202305250048.dist-info/METADATA,sha256=EeiQgV19AtQemzck6c_3Zbd1EVR3adKJsSMBybpkFq8,251
+mb_utils-1.0.202305250048.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+mb_utils-1.0.202305250048.dist-info/top_level.txt,sha256=xeK1qEZ7uoXfZyNlYlurb_F_T8trKUaTU_Fm_UpKhyg,9
+mb_utils-1.0.202305250048.dist-info/RECORD,,
```

