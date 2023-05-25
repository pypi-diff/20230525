# Comparing `tmp/irene_pro-0.0.44.tar.gz` & `tmp/irene_pro-0.0.45.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irene_pro-0.0.44.tar", last modified: Thu May 25 07:52:31 2023, max compression
+gzip compressed data, was "irene_pro-0.0.45.tar", last modified: Thu May 25 14:06:00 2023, max compression
```

## Comparing `irene_pro-0.0.44.tar` & `irene_pro-0.0.45.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 07:52:30.983152 irene_pro-0.0.44/
--rw-rw-rw-   0        0        0      227 2023-05-04 09:47:29.000000 irene_pro-0.0.44/LICENSE
--rw-rw-rw-   0        0        0       14 2023-05-08 07:12:29.000000 irene_pro-0.0.44/MANIFEST.in
--rw-rw-rw-   0        0        0     1740 2023-05-25 07:52:30.979135 irene_pro-0.0.44/PKG-INFO
--rw-rw-rw-   0        0        0     1165 2023-05-25 07:51:23.000000 irene_pro-0.0.44/README.md
-drwxrwxrwx   0        0        0        0 2023-05-25 07:52:30.912251 irene_pro-0.0.44/irene_pro/
--rw-rw-rw-   0        0        0        0 2023-05-04 13:31:01.000000 irene_pro-0.0.44/irene_pro/__init__.py
--rw-rw-rw-   0        0        0     4001 2023-05-24 10:17:54.000000 irene_pro-0.0.44/irene_pro/logic.py
--rw-rw-rw-   0        0        0    31614 2023-05-25 07:49:29.000000 irene_pro-0.0.44/irene_pro/widgets.py
-drwxrwxrwx   0        0        0        0 2023-05-25 07:52:30.970160 irene_pro-0.0.44/irene_pro.egg-info/
--rw-rw-rw-   0        0        0     1740 2023-05-25 07:52:30.000000 irene_pro-0.0.44/irene_pro.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      264 2023-05-25 07:52:30.000000 irene_pro-0.0.44/irene_pro.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 07:52:30.000000 irene_pro-0.0.44/irene_pro.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-05-25 07:52:30.000000 irene_pro-0.0.44/irene_pro.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-25 07:52:30.000000 irene_pro-0.0.44/irene_pro.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-25 07:52:30.984123 irene_pro-0.0.44/setup.cfg
--rw-rw-rw-   0        0        0     1164 2023-05-25 07:50:19.000000 irene_pro-0.0.44/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-25 14:06:00.492912 irene_pro-0.0.45/
+-rw-rw-rw-   0        0        0      227 2023-05-04 09:47:29.000000 irene_pro-0.0.45/LICENSE
+-rw-rw-rw-   0        0        0       14 2023-05-08 07:12:29.000000 irene_pro-0.0.45/MANIFEST.in
+-rw-rw-rw-   0        0        0     1740 2023-05-25 14:06:00.489920 irene_pro-0.0.45/PKG-INFO
+-rw-rw-rw-   0        0        0     1165 2023-05-25 07:51:23.000000 irene_pro-0.0.45/README.md
+drwxrwxrwx   0        0        0        0 2023-05-25 14:06:00.445039 irene_pro-0.0.45/irene_pro/
+-rw-rw-rw-   0        0        0        0 2023-05-04 13:31:01.000000 irene_pro-0.0.45/irene_pro/__init__.py
+-rw-rw-rw-   0        0        0     4001 2023-05-24 10:17:54.000000 irene_pro-0.0.45/irene_pro/logic.py
+-rw-rw-rw-   0        0        0    31920 2023-05-25 14:04:48.000000 irene_pro-0.0.45/irene_pro/widgets.py
+drwxrwxrwx   0        0        0        0 2023-05-25 14:06:00.483936 irene_pro-0.0.45/irene_pro.egg-info/
+-rw-rw-rw-   0        0        0     1740 2023-05-25 14:06:00.000000 irene_pro-0.0.45/irene_pro.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      264 2023-05-25 14:06:00.000000 irene_pro-0.0.45/irene_pro.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 14:06:00.000000 irene_pro-0.0.45/irene_pro.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-05-25 14:06:00.000000 irene_pro-0.0.45/irene_pro.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-25 14:06:00.000000 irene_pro-0.0.45/irene_pro.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-25 14:06:00.493909 irene_pro-0.0.45/setup.cfg
+-rw-rw-rw-   0        0        0     1164 2023-05-25 14:05:09.000000 irene_pro-0.0.45/setup.py
```

### Comparing `irene_pro-0.0.44/PKG-INFO` & `irene_pro-0.0.45/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irene_pro
-Version: 0.0.44
+Version: 0.0.45
 Summary: Use customized GUI
 Author: Irene coldsober
 Author-email: <irene.study.2023@gmail.com>
 Keywords: tkinter,widget,gui
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `irene_pro-0.0.44/README.md` & `irene_pro-0.0.45/README.md`

 * *Files identical despite different names*

### Comparing `irene_pro-0.0.44/irene_pro/logic.py` & `irene_pro-0.0.45/irene_pro/logic.py`

 * *Files identical despite different names*

### Comparing `irene_pro-0.0.44/irene_pro/widgets.py` & `irene_pro-0.0.45/irene_pro/widgets.py`

 * *Files 2% similar despite different names*

```diff
@@ -731,29 +731,33 @@
     def widget_triger(self, widget, btns = 4, btn_labels = {'1':'delete', '2':'edit', '3':'status', '4':'details'}):
         """event: like `<Button-1>`"""
         fr = frame(self.parent)
         fr.place(x = widget.winfo_rootx(), y = widget.winfo_rooty(), width = w(250), height = h(30*btns))
 
         # delete member from the database
         delete_btn = btn(fr, text = btn_labels['1'], activebackground = fr.cget('bg'))
+        # delete_btn.bind("<Button-1>", lambda e: fr.destroy(), add = "+")
         delete_btn.pack(side = TOP, padx = w(1), pady = h(0), fill=X, expand = True, anchor = NW)
 
         # change name, qualification, department, knowledgeability and so on
         edit_btn = btn(fr, text = btn_labels['2'], activebackground = fr.cget('bg'))
+        # edit_btn.bind("<Button-1>", lambda e: fr.destroy(), add = "+")
         edit_btn.pack(side = TOP, padx = w(1), pady = h(0), fill=X, expand = True, anchor = NW)
 
         # in work, in leave, idle or other status
         status = btn(fr, text = btn_labels['3'], activebackground = fr.cget('bg'), bg = "#112200", fg = "#fff")
+        # status.bind("<Button-1>", lambda e: fr.destroy(), add = "+")
         status.pack(side = TOP, padx = w(1), pady = h(0), fill=X, expand = True, anchor = NW)
 
         # to get the data analysis of single clicked employee or else member
         details = btn(fr, text = btn_labels['4'], activebackground = fr.cget('bg'), bg = "#ffaa00")
+        # details.bind("<Button-1>", lambda e: fr.destroy(), add = "+")
         details.pack(side = TOP, padx = w(1), pady = h(0), fill=X, expand = True, anchor = NW)
 
-        self.parent.bind("<Button-1>", lambda e: fr.destroy())
+        self.parent.bind("<Button-1>", lambda e: fr.destroy(), add = "+")
 
         return delete_btn, edit_btn, status, details
 
 # CONSTANTS
 comb_syle = 'comb.TCombobox'
 check_style = "TCheckbutton"
 radio_style = "Custom.TRadiobutton"
```

### Comparing `irene_pro-0.0.44/irene_pro.egg-info/PKG-INFO` & `irene_pro-0.0.45/irene_pro.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irene-pro
-Version: 0.0.44
+Version: 0.0.45
 Summary: Use customized GUI
 Author: Irene coldsober
 Author-email: <irene.study.2023@gmail.com>
 Keywords: tkinter,widget,gui
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `irene_pro-0.0.44/setup.py` & `irene_pro-0.0.45/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 00000090: 286f 732e 7061 7468 2e6a 6f69 6e28 6865  (os.path.join(he
 000000a0: 7265 2c20 2252 4541 444d 452e 6d64 2229  re, "README.md")
 000000b0: 2c20 656e 636f 6469 6e67 3d22 7574 662d  , encoding="utf-
 000000c0: 3822 2920 6173 2066 683a 0d0a 2020 2020  8") as fh:..    
 000000d0: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
 000000e0: 203d 2022 5c6e 2220 2b20 6668 2e72 6561   = "\n" + fh.rea
 000000f0: 6428 290d 0a0d 0a56 4552 5349 4f4e 203d  d()....VERSION =
-00000100: 2027 302e 302e 3434 270d 0a44 4553 4352   '0.0.44'..DESCR
+00000100: 2027 302e 302e 3435 270d 0a44 4553 4352   '0.0.45'..DESCR
 00000110: 4950 5449 4f4e 203d 2027 5573 6520 6375  IPTION = 'Use cu
 00000120: 7374 6f6d 697a 6564 2047 5549 270d 0a4c  stomized GUI'..L
 00000130: 4f4e 475f 4445 5343 5249 5054 494f 4e20  ONG_DESCRIPTION 
 00000140: 3d20 2741 2070 6163 6b61 6765 2074 6861  = 'A package tha
 00000150: 7420 616c 6c6f 7773 2079 6f75 2074 6f20  t allows you to 
 00000160: 7573 6520 7374 796c 6573 2061 6e64 2077  use styles and w
 00000170: 6964 6765 7420 6f66 2073 7570 6572 206c  idget of super l
```

