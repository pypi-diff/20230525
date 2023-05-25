# Comparing `tmp/irene_pro-0.0.43.tar.gz` & `tmp/irene_pro-0.0.44.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irene_pro-0.0.43.tar", last modified: Wed May 24 10:19:16 2023, max compression
+gzip compressed data, was "irene_pro-0.0.44.tar", last modified: Thu May 25 07:52:31 2023, max compression
```

## Comparing `irene_pro-0.0.43.tar` & `irene_pro-0.0.44.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 10:19:16.976613 irene_pro-0.0.43/
--rw-rw-rw-   0        0        0      227 2023-05-04 09:47:29.000000 irene_pro-0.0.43/LICENSE
--rw-rw-rw-   0        0        0       14 2023-05-08 07:12:29.000000 irene_pro-0.0.43/MANIFEST.in
--rw-rw-rw-   0        0        0     1632 2023-05-24 10:19:16.975617 irene_pro-0.0.43/PKG-INFO
--rw-rw-rw-   0        0        0     1058 2023-05-24 10:17:13.000000 irene_pro-0.0.43/README.md
-drwxrwxrwx   0        0        0        0 2023-05-24 10:19:16.955670 irene_pro-0.0.43/irene_pro/
--rw-rw-rw-   0        0        0        0 2023-05-04 13:31:01.000000 irene_pro-0.0.43/irene_pro/__init__.py
--rw-rw-rw-   0        0        0     4001 2023-05-24 10:17:54.000000 irene_pro-0.0.43/irene_pro/logic.py
--rw-rw-rw-   0        0        0    30349 2023-05-24 10:18:07.000000 irene_pro-0.0.43/irene_pro/widgets.py
-drwxrwxrwx   0        0        0        0 2023-05-24 10:19:16.972625 irene_pro-0.0.43/irene_pro.egg-info/
--rw-rw-rw-   0        0        0     1632 2023-05-24 10:19:16.000000 irene_pro-0.0.43/irene_pro.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      264 2023-05-24 10:19:16.000000 irene_pro-0.0.43/irene_pro.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 10:19:16.000000 irene_pro-0.0.43/irene_pro.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-05-24 10:19:16.000000 irene_pro-0.0.43/irene_pro.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-24 10:19:16.000000 irene_pro-0.0.43/irene_pro.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-24 10:19:16.977610 irene_pro-0.0.43/setup.cfg
--rw-rw-rw-   0        0        0     1164 2023-05-24 10:16:41.000000 irene_pro-0.0.43/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-25 07:52:30.983152 irene_pro-0.0.44/
+-rw-rw-rw-   0        0        0      227 2023-05-04 09:47:29.000000 irene_pro-0.0.44/LICENSE
+-rw-rw-rw-   0        0        0       14 2023-05-08 07:12:29.000000 irene_pro-0.0.44/MANIFEST.in
+-rw-rw-rw-   0        0        0     1740 2023-05-25 07:52:30.979135 irene_pro-0.0.44/PKG-INFO
+-rw-rw-rw-   0        0        0     1165 2023-05-25 07:51:23.000000 irene_pro-0.0.44/README.md
+drwxrwxrwx   0        0        0        0 2023-05-25 07:52:30.912251 irene_pro-0.0.44/irene_pro/
+-rw-rw-rw-   0        0        0        0 2023-05-04 13:31:01.000000 irene_pro-0.0.44/irene_pro/__init__.py
+-rw-rw-rw-   0        0        0     4001 2023-05-24 10:17:54.000000 irene_pro-0.0.44/irene_pro/logic.py
+-rw-rw-rw-   0        0        0    31614 2023-05-25 07:49:29.000000 irene_pro-0.0.44/irene_pro/widgets.py
+drwxrwxrwx   0        0        0        0 2023-05-25 07:52:30.970160 irene_pro-0.0.44/irene_pro.egg-info/
+-rw-rw-rw-   0        0        0     1740 2023-05-25 07:52:30.000000 irene_pro-0.0.44/irene_pro.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      264 2023-05-25 07:52:30.000000 irene_pro-0.0.44/irene_pro.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 07:52:30.000000 irene_pro-0.0.44/irene_pro.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-05-25 07:52:30.000000 irene_pro-0.0.44/irene_pro.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-25 07:52:30.000000 irene_pro-0.0.44/irene_pro.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-25 07:52:30.984123 irene_pro-0.0.44/setup.cfg
+-rw-rw-rw-   0        0        0     1164 2023-05-25 07:50:19.000000 irene_pro-0.0.44/setup.py
```

### Comparing `irene_pro-0.0.43/PKG-INFO` & `irene_pro-0.0.44/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irene_pro
-Version: 0.0.43
+Version: 0.0.44
 Summary: Use customized GUI
 Author: Irene coldsober
 Author-email: <irene.study.2023@gmail.com>
 Keywords: tkinter,widget,gui
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -38,8 +38,9 @@
 sign = widgets.LoginSignup(master)
 # get the sign_in_btn
 login_btn = sign.Login_btn()
 # call a function if the validation is successfully
 login_btn.config(command = sign.validate_login(callback = func_to_call, saved_username, saved_password))
 
 # SQLITE3 DATABASE ADDED IN LOGIC LIBRALY
+# Sub menu to extend the functionalities like edit, delete and getting some details on the selected label
```

### Comparing `irene_pro-0.0.43/README.md` & `irene_pro-0.0.44/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -21,8 +21,9 @@
 sign = widgets.LoginSignup(master)
 # get the sign_in_btn
 login_btn = sign.Login_btn()
 # call a function if the validation is successfully
 login_btn.config(command = sign.validate_login(callback = func_to_call, saved_username, saved_password))
 
 # SQLITE3 DATABASE ADDED IN LOGIC LIBRALY
+# Sub menu to extend the functionalities like edit, delete and getting some details on the selected label
```

### Comparing `irene_pro-0.0.43/irene_pro/logic.py` & `irene_pro-0.0.44/irene_pro/logic.py`

 * *Files identical despite different names*

### Comparing `irene_pro-0.0.43/irene_pro/widgets.py` & `irene_pro-0.0.44/irene_pro/widgets.py`

 * *Files 2% similar despite different names*

```diff
@@ -540,15 +540,15 @@
 
         if login:
             self.login()
         else:
             self.signup()
 
     def login(self):
-        global lusername, lpassword, validate_btn
+        global lusername, lpassword, login_btn
         for fr in self.login_frame:
             fr.destroy()
 
         login_fr = frame(self.base_frame)
         login_fr.pack(fill = BOTH, expand = True)
         self.login_frame.append(login_fr)
         self.signup_frame.append(login_fr)
@@ -568,39 +568,36 @@
         lpassword = entry(login_fr, default="Enter password")
         lpassword.pack(side = TOP, pady = h(2), padx = w(1), fill = X, expand = True)
 
         btns = frame(login_fr)
         btns.config(bg = login_fr['bg'])
         btns.pack(fill = X, side = BOTTOM, expand = True, padx = w(1), pady = h(1), anchor=S)
 
-        login_btn = btn(btns, text = "login")
+        login_btn = btn(btns, text = "sign in")
         login_btn.config(bg = "#b04", fg = "#fff")
         login_btn.pack(side = LEFT, padx = w(3), expand = True, fill = X)
 
         signup_btn = btn(btns, text = "Sign up", command = self.signup)
         signup_btn.config(bg = "#023", fg = "#fff")
         signup_btn.pack(side = LEFT, padx = w(3), expand = True, fill = X)
 
-        validate_btn = btn(btns, text = "Next")
-        validate_btn.config(bg = "#023", fg = "#fff")
-        validate_btn.pack(side = LEFT, padx = w(3), expand = True, fill = X)
 
         cancel_btn = btn(btns, text = "cancel", command = lambda: self.base_frame.destroy())
         cancel_btn.config(bg = "#600", fg = "#fff")
         cancel_btn.pack(side = RIGHT, padx = w(3), expand = True, fill = X)
     
     @property
     def Login_btn(self):
-        return validate_btn
+        return login_btn
 
     def login_user_data(self):
         return lusername.get(), lpassword.get()
 
     def signup(self):
-        global confirm_btn, username, password, re_password
+        global signup_btn, username, password, re_password
         for fr in self.signup_frame:
             fr.destroy()
             
         signup_fr = frame(self.base_frame)
         signup_fr.pack(fill = BOTH, expand = True)
         signup_fr.pack_propagate(False)
         self.signup_frame.append(signup_fr)
@@ -631,26 +628,22 @@
         login_btn.config(bg = "#b04", fg = "#fff")
         login_btn.pack(side = LEFT, padx = w(1), expand = True, fill = X)
 
         signup_btn = btn(btns, text = "Sign up")
         signup_btn.config(bg = "#023", fg = "#fff")
         signup_btn.pack(side = LEFT, padx = w(1), expand = True, fill = X)
 
-        confirm_btn = btn(btns, text = "confirm")
-        confirm_btn.config(bg = "#023", fg = "#fff")
-        confirm_btn.pack(side = LEFT, padx = w(1), expand = True, fill = X)
-
         cancel_btn = btn(btns, text = "cancel", command = lambda: self.base_frame.destroy())
         cancel_btn.config(bg = "#600", fg = "#fff")
         cancel_btn.pack(side = LEFT, padx = w(1), expand = True, fill = X)
 
     @property
     def Signup_btn(self):
-        return confirm_btn
-
+        return signup_btn
+    
     def signup_user_data(self):
         return username.get(), password.get(), re_password.get()
 
 class Table_gui:
     def __init__(self, parent):
         self.rows = 1
         self.cols = 1
@@ -725,11 +718,42 @@
     
     def final_data(self):
         # BY NOW, THE DATAFRAME WILL BE BEING DISLPLAY IN THE TERMINAL
         nd = np.array(self.data)
         transposed_data = nd.T
         return transposed_data.tolist()
 
+
+class Modify:
+    def __init__(self, parent):
+        """bind a widget to button-3: right mouse click and then extend the functionalities"""
+        self.parent = parent
+
+    def widget_triger(self, widget, btns = 4, btn_labels = {'1':'delete', '2':'edit', '3':'status', '4':'details'}):
+        """event: like `<Button-1>`"""
+        fr = frame(self.parent)
+        fr.place(x = widget.winfo_rootx(), y = widget.winfo_rooty(), width = w(250), height = h(30*btns))
+
+        # delete member from the database
+        delete_btn = btn(fr, text = btn_labels['1'], activebackground = fr.cget('bg'))
+        delete_btn.pack(side = TOP, padx = w(1), pady = h(0), fill=X, expand = True, anchor = NW)
+
+        # change name, qualification, department, knowledgeability and so on
+        edit_btn = btn(fr, text = btn_labels['2'], activebackground = fr.cget('bg'))
+        edit_btn.pack(side = TOP, padx = w(1), pady = h(0), fill=X, expand = True, anchor = NW)
+
+        # in work, in leave, idle or other status
+        status = btn(fr, text = btn_labels['3'], activebackground = fr.cget('bg'), bg = "#112200", fg = "#fff")
+        status.pack(side = TOP, padx = w(1), pady = h(0), fill=X, expand = True, anchor = NW)
+
+        # to get the data analysis of single clicked employee or else member
+        details = btn(fr, text = btn_labels['4'], activebackground = fr.cget('bg'), bg = "#ffaa00")
+        details.pack(side = TOP, padx = w(1), pady = h(0), fill=X, expand = True, anchor = NW)
+
+        self.parent.bind("<Button-1>", lambda e: fr.destroy())
+
+        return delete_btn, edit_btn, status, details
+
 # CONSTANTS
 comb_syle = 'comb.TCombobox'
 check_style = "TCheckbutton"
 radio_style = "Custom.TRadiobutton"
```

### Comparing `irene_pro-0.0.43/irene_pro.egg-info/PKG-INFO` & `irene_pro-0.0.44/irene_pro.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irene-pro
-Version: 0.0.43
+Version: 0.0.44
 Summary: Use customized GUI
 Author: Irene coldsober
 Author-email: <irene.study.2023@gmail.com>
 Keywords: tkinter,widget,gui
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -38,8 +38,9 @@
 sign = widgets.LoginSignup(master)
 # get the sign_in_btn
 login_btn = sign.Login_btn()
 # call a function if the validation is successfully
 login_btn.config(command = sign.validate_login(callback = func_to_call, saved_username, saved_password))
 
 # SQLITE3 DATABASE ADDED IN LOGIC LIBRALY
+# Sub menu to extend the functionalities like edit, delete and getting some details on the selected label
```

### Comparing `irene_pro-0.0.43/setup.py` & `irene_pro-0.0.44/setup.py`

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
-00000100: 2027 302e 302e 3433 270d 0a44 4553 4352   '0.0.43'..DESCR
+00000100: 2027 302e 302e 3434 270d 0a44 4553 4352   '0.0.44'..DESCR
 00000110: 4950 5449 4f4e 203d 2027 5573 6520 6375  IPTION = 'Use cu
 00000120: 7374 6f6d 697a 6564 2047 5549 270d 0a4c  stomized GUI'..L
 00000130: 4f4e 475f 4445 5343 5249 5054 494f 4e20  ONG_DESCRIPTION 
 00000140: 3d20 2741 2070 6163 6b61 6765 2074 6861  = 'A package tha
 00000150: 7420 616c 6c6f 7773 2079 6f75 2074 6f20  t allows you to 
 00000160: 7573 6520 7374 796c 6573 2061 6e64 2077  use styles and w
 00000170: 6964 6765 7420 6f66 2073 7570 6572 206c  idget of super l
```

