# Comparing `tmp/irene_pro-0.0.42.tar.gz` & `tmp/irene_pro-0.0.43.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irene_pro-0.0.42.tar", last modified: Mon May 22 09:51:11 2023, max compression
+gzip compressed data, was "irene_pro-0.0.43.tar", last modified: Wed May 24 10:19:16 2023, max compression
```

## Comparing `irene_pro-0.0.42.tar` & `irene_pro-0.0.43.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 09:51:11.000580 irene_pro-0.0.42/
--rw-rw-rw-   0        0        0      227 2023-05-04 09:47:29.000000 irene_pro-0.0.42/LICENSE
--rw-rw-rw-   0        0        0       14 2023-05-08 07:12:29.000000 irene_pro-0.0.42/MANIFEST.in
--rw-rw-rw-   0        0        0     1622 2023-05-22 09:51:10.998584 irene_pro-0.0.42/PKG-INFO
--rw-rw-rw-   0        0        0     1048 2023-05-22 09:50:08.000000 irene_pro-0.0.42/README.md
-drwxrwxrwx   0        0        0        0 2023-05-22 09:51:10.976642 irene_pro-0.0.42/irene_pro/
--rw-rw-rw-   0        0        0        0 2023-05-04 13:31:01.000000 irene_pro-0.0.42/irene_pro/__init__.py
--rw-rw-rw-   0        0        0     1445 2023-05-11 09:46:57.000000 irene_pro-0.0.42/irene_pro/logic.py
--rw-rw-rw-   0        0        0    30351 2023-05-22 09:48:23.000000 irene_pro-0.0.42/irene_pro/widgets.py
-drwxrwxrwx   0        0        0        0 2023-05-22 09:51:10.994595 irene_pro-0.0.42/irene_pro.egg-info/
--rw-rw-rw-   0        0        0     1622 2023-05-22 09:51:10.000000 irene_pro-0.0.42/irene_pro.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      264 2023-05-22 09:51:10.000000 irene_pro-0.0.42/irene_pro.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 09:51:10.000000 irene_pro-0.0.42/irene_pro.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-05-22 09:51:10.000000 irene_pro-0.0.42/irene_pro.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-22 09:51:10.000000 irene_pro-0.0.42/irene_pro.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-22 09:51:11.001577 irene_pro-0.0.42/setup.cfg
--rw-rw-rw-   0        0        0     1164 2023-05-22 09:49:38.000000 irene_pro-0.0.42/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-24 10:19:16.976613 irene_pro-0.0.43/
+-rw-rw-rw-   0        0        0      227 2023-05-04 09:47:29.000000 irene_pro-0.0.43/LICENSE
+-rw-rw-rw-   0        0        0       14 2023-05-08 07:12:29.000000 irene_pro-0.0.43/MANIFEST.in
+-rw-rw-rw-   0        0        0     1632 2023-05-24 10:19:16.975617 irene_pro-0.0.43/PKG-INFO
+-rw-rw-rw-   0        0        0     1058 2023-05-24 10:17:13.000000 irene_pro-0.0.43/README.md
+drwxrwxrwx   0        0        0        0 2023-05-24 10:19:16.955670 irene_pro-0.0.43/irene_pro/
+-rw-rw-rw-   0        0        0        0 2023-05-04 13:31:01.000000 irene_pro-0.0.43/irene_pro/__init__.py
+-rw-rw-rw-   0        0        0     4001 2023-05-24 10:17:54.000000 irene_pro-0.0.43/irene_pro/logic.py
+-rw-rw-rw-   0        0        0    30349 2023-05-24 10:18:07.000000 irene_pro-0.0.43/irene_pro/widgets.py
+drwxrwxrwx   0        0        0        0 2023-05-24 10:19:16.972625 irene_pro-0.0.43/irene_pro.egg-info/
+-rw-rw-rw-   0        0        0     1632 2023-05-24 10:19:16.000000 irene_pro-0.0.43/irene_pro.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      264 2023-05-24 10:19:16.000000 irene_pro-0.0.43/irene_pro.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 10:19:16.000000 irene_pro-0.0.43/irene_pro.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-05-24 10:19:16.000000 irene_pro-0.0.43/irene_pro.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-24 10:19:16.000000 irene_pro-0.0.43/irene_pro.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-24 10:19:16.977610 irene_pro-0.0.43/setup.cfg
+-rw-rw-rw-   0        0        0     1164 2023-05-24 10:16:41.000000 irene_pro-0.0.43/setup.py
```

### Comparing `irene_pro-0.0.42/PKG-INFO` & `irene_pro-0.0.43/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irene_pro
-Version: 0.0.42
+Version: 0.0.43
 Summary: Use customized GUI
 Author: Irene coldsober
 Author-email: <irene.study.2023@gmail.com>
 Keywords: tkinter,widget,gui
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -37,9 +37,9 @@
 # login and signup template has been added too
 sign = widgets.LoginSignup(master)
 # get the sign_in_btn
 login_btn = sign.Login_btn()
 # call a function if the validation is successfully
 login_btn.config(command = sign.validate_login(callback = func_to_call, saved_username, saved_password))
 
-# working on authentication gui
+# SQLITE3 DATABASE ADDED IN LOGIC LIBRALY
```

### Comparing `irene_pro-0.0.42/README.md` & `irene_pro-0.0.43/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -20,9 +20,9 @@
 # login and signup template has been added too
 sign = widgets.LoginSignup(master)
 # get the sign_in_btn
 login_btn = sign.Login_btn()
 # call a function if the validation is successfully
 login_btn.config(command = sign.validate_login(callback = func_to_call, saved_username, saved_password))
 
-# working on authentication gui
+# SQLITE3 DATABASE ADDED IN LOGIC LIBRALY
```

### Comparing `irene_pro-0.0.42/irene_pro/widgets.py` & `irene_pro-0.0.43/irene_pro/widgets.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 
 from tkinter import *
 from tkinter import ttk, filedialog, messagebox
 import re, random
 from win32api import GetSystemMetrics as ruler
 from math import ceil
 import cv2
-
 from tkcalendar import Calendar
 import ttkthemes
 import numpy as np
 
 s_width = ruler(0)
 s_height = ruler(1)
```

### Comparing `irene_pro-0.0.42/irene_pro.egg-info/PKG-INFO` & `irene_pro-0.0.43/irene_pro.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irene-pro
-Version: 0.0.42
+Version: 0.0.43
 Summary: Use customized GUI
 Author: Irene coldsober
 Author-email: <irene.study.2023@gmail.com>
 Keywords: tkinter,widget,gui
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -37,9 +37,9 @@
 # login and signup template has been added too
 sign = widgets.LoginSignup(master)
 # get the sign_in_btn
 login_btn = sign.Login_btn()
 # call a function if the validation is successfully
 login_btn.config(command = sign.validate_login(callback = func_to_call, saved_username, saved_password))
 
-# working on authentication gui
+# SQLITE3 DATABASE ADDED IN LOGIC LIBRALY
```

### Comparing `irene_pro-0.0.42/setup.py` & `irene_pro-0.0.43/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 00000090: 286f 732e 7061 7468 2e6a 6f69 6e28 6865  (os.path.join(he
 000000a0: 7265 2c20 2252 4541 444d 452e 6d64 2229  re, "README.md")
 000000b0: 2c20 656e 636f 6469 6e67 3d22 7574 662d  , encoding="utf-
 000000c0: 3822 2920 6173 2066 683a 0d0a 2020 2020  8") as fh:..    
 000000d0: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
 000000e0: 203d 2022 5c6e 2220 2b20 6668 2e72 6561   = "\n" + fh.rea
 000000f0: 6428 290d 0a0d 0a56 4552 5349 4f4e 203d  d()....VERSION =
-00000100: 2027 302e 302e 3432 270d 0a44 4553 4352   '0.0.42'..DESCR
+00000100: 2027 302e 302e 3433 270d 0a44 4553 4352   '0.0.43'..DESCR
 00000110: 4950 5449 4f4e 203d 2027 5573 6520 6375  IPTION = 'Use cu
 00000120: 7374 6f6d 697a 6564 2047 5549 270d 0a4c  stomized GUI'..L
 00000130: 4f4e 475f 4445 5343 5249 5054 494f 4e20  ONG_DESCRIPTION 
 00000140: 3d20 2741 2070 6163 6b61 6765 2074 6861  = 'A package tha
 00000150: 7420 616c 6c6f 7773 2079 6f75 2074 6f20  t allows you to 
 00000160: 7573 6520 7374 796c 6573 2061 6e64 2077  use styles and w
 00000170: 6964 6765 7420 6f66 2073 7570 6572 206c  idget of super l
```

