# Comparing `tmp/mapdata-1.8.1.tar.gz` & `tmp/mapdata-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mapdata-1.8.1.tar", last modified: Tue May 16 16:26:31 2023, max compression
+gzip compressed data, was "mapdata-1.8.2.tar", last modified: Thu May 25 02:00:57 2023, max compression
```

## Comparing `mapdata-1.8.1.tar` & `mapdata-1.8.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2023-05-16 16:26:31.799225 mapdata-1.8.1/
--rw-------   0 dreas     (1000) dreas     (1000)      614 2023-05-10 02:52:31.000000 mapdata-1.8.1/LICENSE.txt
--rw-------   0 dreas     (1000) dreas     (1000)       88 2022-01-15 18:16:09.000000 mapdata-1.8.1/MANIFEST.in
--rw-rw-r--   0 dreas     (1000) dreas     (1000)     3009 2023-05-16 16:26:31.799225 mapdata-1.8.1/PKG-INFO
--rw-r--r--   0 dreas     (1000) dreas     (1000)     1866 2023-05-15 01:02:57.000000 mapdata-1.8.1/README.md
-drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2023-05-16 16:26:31.799225 mapdata-1.8.1/mapdata/
--rwxr-xr-x   0 dreas     (1000) dreas     (1000)    85218 2023-05-16 16:06:41.000000 mapdata-1.8.1/mapdata/mapdata.py
-drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2023-05-16 16:26:31.799225 mapdata-1.8.1/mapdata.egg-info/
--rw-rw-r--   0 dreas     (1000) dreas     (1000)     3009 2023-05-16 16:26:31.000000 mapdata-1.8.1/mapdata.egg-info/PKG-INFO
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      185 2023-05-16 16:26:31.000000 mapdata-1.8.1/mapdata.egg-info/SOURCES.txt
--rw-rw-r--   0 dreas     (1000) dreas     (1000)        1 2023-05-16 16:26:31.000000 mapdata-1.8.1/mapdata.egg-info/dependency_links.txt
--rw-rw-r--   0 dreas     (1000) dreas     (1000)        1 2023-05-16 16:26:31.000000 mapdata-1.8.1/mapdata.egg-info/top_level.txt
--rw-rw-r--   0 dreas     (1000) dreas     (1000)       38 2023-05-16 16:26:31.799225 mapdata-1.8.1/setup.cfg
--rw-rw-r--   0 dreas     (1000) dreas     (1000)     1279 2023-05-16 16:06:59.000000 mapdata-1.8.1/setup.py
+drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2023-05-25 02:00:57.572999 mapdata-1.8.2/
+-rw-------   0 dreas     (1000) dreas     (1000)      614 2023-05-10 02:52:31.000000 mapdata-1.8.2/LICENSE.txt
+-rw-------   0 dreas     (1000) dreas     (1000)       88 2022-01-15 18:16:09.000000 mapdata-1.8.2/MANIFEST.in
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)     3009 2023-05-25 02:00:57.572999 mapdata-1.8.2/PKG-INFO
+-rw-r--r--   0 dreas     (1000) dreas     (1000)     1866 2023-05-15 01:02:57.000000 mapdata-1.8.2/README.md
+drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2023-05-25 02:00:57.568999 mapdata-1.8.2/mapdata/
+-rwxr-xr-x   0 dreas     (1000) dreas     (1000)    86410 2023-05-25 01:40:23.000000 mapdata-1.8.2/mapdata/mapdata.py
+drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2023-05-25 02:00:57.572999 mapdata-1.8.2/mapdata.egg-info/
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)     3009 2023-05-25 02:00:57.000000 mapdata-1.8.2/mapdata.egg-info/PKG-INFO
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      185 2023-05-25 02:00:57.000000 mapdata-1.8.2/mapdata.egg-info/SOURCES.txt
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)        1 2023-05-25 02:00:57.000000 mapdata-1.8.2/mapdata.egg-info/dependency_links.txt
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)        1 2023-05-25 02:00:57.000000 mapdata-1.8.2/mapdata.egg-info/top_level.txt
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)       38 2023-05-25 02:00:57.572999 mapdata-1.8.2/setup.cfg
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)     1279 2023-05-25 02:00:53.000000 mapdata-1.8.2/setup.py
```

### Comparing `mapdata-1.8.1/LICENSE.txt` & `mapdata-1.8.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mapdata-1.8.1/PKG-INFO` & `mapdata-1.8.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapdata
-Version: 1.8.1
+Version: 1.8.2
 Summary: An interactive map and table explorer for geographic coordinates in a CSV file
 Home-page: https://osdn.net/project/mapdata/
 Author: Dreas Nielsen
 Author-email: dreas.nielsen@gmail.com
 License: GPL
 Keywords: Map,Locations,CRS,CSV,PNG,JPG,Postscript
 Platform: UNKNOWN
```

### Comparing `mapdata-1.8.1/README.md` & `mapdata-1.8.2/README.md`

 * *Files identical despite different names*

### Comparing `mapdata-1.8.1/mapdata/mapdata.py` & `mapdata-1.8.2/mapdata/mapdata.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,32 +59,34 @@
 #				to export the map and quit.  RDN.
 #	2023-05-12	Added export of configuration settings.  Cleaned up help
 #				dialogs.  RDN.
 #	2023-05-14	Put the map and table in a PanedWindow.  RDN.
 #	2023-05-16	Fixed label wrapping in Windows on the CSV open dialog.  Corrected
 #				binding of Return and Escape keys to dialog button actions.  Adujsted
 #				button position in MsgDialog.  RDN.
+#	2023-05-24	Modified dialogs, added 'Help' buttons.  RDN.
 # ==================================================================
 
-version = "1.8.1"
-vdate = "2023-05-16"
+version = "1.8.2"
+vdate = "2023-05-24"
 
 copyright = "2023"
 
 
 import sys
 import os.path
 import io
 import codecs
 import argparse
 from configparser import ConfigParser
 import csv
 import re
 import datetime
 import time
+import webbrowser
 import tkinter as tk
 import tkinter.ttk as ttk
 import tkinter.font as tkfont
 import tkinter.filedialog as tkfiledialog
 import tkintermapview as tkmv
 from PIL import ImageGrab
 
@@ -1164,15 +1166,14 @@
 				f.write("select_color=%s\n" % select_color)
 				f.write("label_color=%s\n" % label_color)
 				f.write("label_font=%s\n" % label_font)
 				f.write("label_size=%s\n" % label_size)
 				f.write("label_bold=%s\n" % ('No' if not label_bold else 'Yes'))
 				f.write("label_position=%s\n" % label_position)
 		def online_help():
-			import webbrowser
 			webbrowser.open("https://mapdata.osdn.io", new=2, autoraise=True)
 		def show_config_files():
 			if len(config_files) == 0 and len(config_files_user) == 0:
 				msg = "No configuration files have been read."
 			else:
 				if len(config_files) > 0:
 					msg = "Configuration files read on startup:\n   %s" % "\n   ".join(config_files)
@@ -1211,19 +1212,20 @@
 		help_menu.add_command(label="About", command = show_about)
 
 
 
 class MarkerDialog(object):
 	def __init__(self, parent):
 		self.dlg = tk.Toplevel()
-		self.dlg.title("New marker")
+		self.dlg.title("Change Marker")
 		prompt_frame = tk.Frame(self.dlg)
 		prompt_frame.grid(row=0, column=0, sticky=tk.NSEW, pady=(3,3))
 		btn_frame = tk.Frame(self.dlg, borderwidth=3, relief=tk.RIDGE)
 		btn_frame.grid(row=1, column=0, sticky=tk.EW, pady=(3,3))
+		btn_frame.columnconfigure(0, weight=1)
 		symbol_lbl = ttk.Label(prompt_frame, text="Symbol:")
 		symbol_lbl.grid(row=0, column=0, sticky=tk.E, padx=(3,3))
 		self.symbol_var = tk.StringVar(self.dlg, "wedge")
 		symbol_vals = list(icon_xbm.keys())
 		self.symbol_opts = tk.OptionMenu(prompt_frame, self.symbol_var, *symbol_vals)
 		self.symbol_opts.configure(width=15)
 		self.symbol_opts.grid(row=0, column=1, sticky=tk.W, padx=(3,3))
@@ -1232,20 +1234,24 @@
 		self.color_var = tk.StringVar(self.dlg, "red")
 		color_vals = list(select_colors)
 		color_opts = tk.OptionMenu(prompt_frame, self.color_var, *color_vals)
 		color_opts.configure(width=15)
 		color_opts.grid(row=1, column=1, sticky=tk.W, padx=(3,3))
 		# Buttons
 		self.canceled = False
+		help_btn = ttk.Button(btn_frame, text="Help", command=self.do_help)
+		help_btn.grid(row=0, column=0, sticky=tk.W, padx=(6,3))
+		ok_btn = ttk.Button(btn_frame, text="OK", command=self.do_select)
+		ok_btn.grid(row=0, column=1, sticky=tk.E, padx=(3,3))
 		cancel_btn = ttk.Button(btn_frame, text="Cancel", command=self.do_cancel)
-		cancel_btn.grid(row=0, column=1, sticky=tk.E, padx=(3,5))
-		ok_btn = ttk.Button(btn_frame, text="Ok", command=self.do_select)
-		ok_btn.grid(row=0, column=0, sticky=tk.E, padx=(60,2))
+		cancel_btn.grid(row=0, column=2, sticky=tk.E, padx=(3,6))
 		self.dlg.bind("<Return>", self.do_select)
 		self.dlg.bind("<Escape>", self.do_cancel)
+	def do_help(self, *args):
+		webbrowser.open("https://mapdata.osdn.io/dialogs.html#change-marker", new=2, autoraise=True)
 	def do_cancel(self, *args):
 		self.canceled = True
 		self.dlg.destroy()
 	def do_select(self, *args):
 		self.canceled = False
 		self.dlg.destroy()
 	def get_marker(self):
@@ -1273,15 +1279,16 @@
 		self.dlg.title("Import X11 Bitmap Symbol")
 		prompt_frame = tk.Frame(self.dlg)
 		prompt_frame.grid(row=0, column=0, sticky=tk.NSEW, pady=(3,3))
 		button_frame = tk.Frame(self.dlg, borderwidth=3, relief=tk.RIDGE)
 		button_frame.grid(row=1, column=0, columnspan=3, sticky=tk.EW, pady=(3,3))
 		button_frame.columnconfigure(0, weight=1)
 		btn_frame = tk.Frame(button_frame)
-		btn_frame.grid(row=0, column=0, sticky=tk.E)
+		btn_frame.grid(row=0, column=0, sticky=tk.EW)
+		btn_frame.columnconfigure(0, weight=1)
 		# Prompts
 		symbol_lbl = ttk.Label(prompt_frame, text="Symbol name:")
 		symbol_lbl.grid(row=0, column=0, sticky=tk.E, padx=(3,3))
 		self.symbol_var = tk.StringVar(self.dlg, "")
 		self.symbol_var.trace('w', check_enable)
 		self.symbol_entry = ttk.Entry(prompt_frame, textvariable=self.symbol_var, width=12)
 		self.symbol_entry.grid(row=0, column=1, sticky=tk.W, padx=(3,3))
@@ -1293,21 +1300,25 @@
 		fn_entry = ttk.Entry(prompt_frame, textvariable=self.fn_var)
 		fn_entry.configure(width=64)
 		fn_entry.grid(row=1, column=1, sticky=tk.EW, padx=(3,3))
 		fn_btn = ttk.Button(prompt_frame, text="Browse", command=get_fn)
 		fn_btn.grid(row=1, column=2, sticky=tk.W)
 		# Buttons
 		self.canceled = False
-		cancel_btn = ttk.Button(btn_frame, text="Cancel", command=self.do_cancel)
-		cancel_btn.grid(row=0, column=1, sticky=tk.E, padx=(3,5))
-		ok_btn = ttk.Button(btn_frame, text="Ok", command=self.do_select)
+		help_btn = ttk.Button(btn_frame, text="Help", command=self.do_help)
+		help_btn.grid(row=0, column=0, sticky=tk.W, padx=(6,3))
+		ok_btn = ttk.Button(btn_frame, text="OK", command=self.do_select)
 		ok_btn["state"] = tk.DISABLED
-		ok_btn.grid(row=0, column=0, sticky=tk.E, padx=(60,2))
+		ok_btn.grid(row=0, column=1, sticky=tk.E, padx=(3,3))
+		cancel_btn = ttk.Button(btn_frame, text="Cancel", command=self.do_cancel)
+		cancel_btn.grid(row=0, column=2, sticky=tk.E, padx=(3,6))
 		self.dlg.bind("<Return>", self.do_select)
 		self.dlg.bind("<Escape>", self.do_cancel)
+	def do_help(self, *args):
+		webbrowser.open("https://mapdata.osdn.io/dialogs.html#import-symbol", new=2, autoraise=True)
 	def do_cancel(self, *args):
 		self.canceled = True
 		self.dlg.destroy()
 	def do_select(self, *args):
 		self.canceled = False
 		self.dlg.destroy()
 	def run(self):
@@ -1339,15 +1350,15 @@
 				ok_btn["state"] = tk.NORMAL
 			else:
 				ok_btn["state"] = tk.DISABLED
 		def new_fn(*args):
 			check_enable()
 		self.header_list = []
 		self.dlg = tk.Toplevel()
-		self.dlg.title("New data file for map display")
+		self.dlg.title("Open CSV Data File for Map Display")
 		# Main frames
 		prompt_frame = tk.Frame(self.dlg)
 		prompt_frame.grid(row=0, column=0, sticky=tk.NSEW, padx=(3,3), pady=(3,3))
 		dir_frame = tk.Frame(prompt_frame)
 		dir_frame.grid(row=0, column=0, sticky=tk.EW, padx=(3,3), pady=(3,3))
 		dir_frame.rowconfigure(0, weight=1)
 		dir_frame.columnconfigure(0, weight=1)
@@ -1430,22 +1441,26 @@
 		title_label = ttk.Label(opt_col_frame, text="Description:")
 		title_label.grid(row=2, column=0, sticky=tk.E, padx=(6,3), pady=(3,3))
 		self.title_var = tk.StringVar(opt_col_frame, '')
 		title_entry = ttk.Entry(opt_col_frame, width=60, textvariable=self.title_var)
 		title_entry.grid(row=2, column=1, columnspan=3, sticky=tk.EW, padx=(3,6), pady=(3,3))
 		# Buttons
 		self.canceled = False
-		cancel_btn = ttk.Button(btn_frame, text="Cancel", command=self.do_cancel)
-		cancel_btn.grid(row=0, column=2, sticky=tk.E, padx=3)
-		ok_btn = ttk.Button(btn_frame, text="Ok", command=self.do_select)
+		help_btn = ttk.Button(btn_frame, text="Help", command=self.do_help)
+		help_btn.grid(row=0, column=0, sticky=tk.W, padx=(6,3))
+		ok_btn = ttk.Button(btn_frame, text="OK", command=self.do_select)
 		ok_btn.grid(row=0, column=1, sticky=tk.E, padx=3)
+		cancel_btn = ttk.Button(btn_frame, text="Cancel", command=self.do_cancel)
+		cancel_btn.grid(row=0, column=2, sticky=tk.E, padx=(3,6))
 		ok_btn["state"] = tk.DISABLED
 		self.dlg.bind("<Return>", self.do_select)
 		self.dlg.bind("<Escape>", self.do_cancel)
 		self.dlg.resizable(False, False)
+	def do_help(self, *args):
+		webbrowser.open("https://mapdata.osdn.io/dialogs.html#open-csv-data-file", new=2, autoraise=True)
 	def do_cancel(self, *args):
 		self.canceled = True
 		self.dlg.destroy()
 	def do_select(self, *args):
 		if self.fn_var.get() != '' and self.lat_var.get() != '' and self.lon_var.get() != '':
 			self.canceled = False
 			self.dlg.destroy()
@@ -1472,20 +1487,24 @@
 		crs_lbl = ttk.Label(prompt_frame, text="New CRS:")
 		crs_lbl.grid(row=0, column=0, sticky=tk.E, padx=(3,3))
 		self.crs_var = tk.IntVar(self.dlg, current_crs)
 		self.crs_entry = ttk.Entry(prompt_frame, width=12, textvariable=self.crs_var)
 		self.crs_entry.grid(row=0, column=1, sticky=tk.W, padx=(3,3))
 		# Buttons
 		self.canceled = False
+		help_btn = ttk.Button(btn_frame, text="Help", command=self.do_help)
+		help_btn.grid(row=0, column=0, sticky=tk.W, padx=(6,3))
+		ok_btn = ttk.Button(btn_frame, text="OK", command=self.do_select)
+		ok_btn.grid(row=0, column=1, sticky=tk.E, padx=(3,3))
 		cancel_btn = ttk.Button(btn_frame, text="Cancel", command=self.do_cancel)
-		cancel_btn.grid(row=0, column=1, sticky=tk.E, padx=(3,5))
-		ok_btn = ttk.Button(btn_frame, text="Ok", command=self.do_select)
-		ok_btn.grid(row=0, column=0, sticky=tk.E, padx=(3,3))
+		cancel_btn.grid(row=0, column=2, sticky=tk.E, padx=(3,6))
 		self.dlg.bind("<Return>", self.do_select)
 		self.dlg.bind("<Escape>", self.do_cancel)
+	def do_help(self, *args):
+		webbrowser.open("https://mapdata.osdn.io/dialogs.html#change-crs", new=2, autoraise=True)
 	def do_cancel(self, *args):
 		self.canceled = True
 		self.dlg.destroy()
 	def do_select(self, *args):
 		self.canceled = False
 		self.dlg.destroy()
 	def get_crs(self):
@@ -1511,14 +1530,15 @@
 		prompt_frame = tk.Frame(self.dlg)
 		prompt_frame.grid(row=0, column=0, sticky=tk.NSEW, pady=(3,3))
 		msg_lbl = ttk.Label(prompt_frame, text=message)
 		msg_lbl.grid(row=0, column=0, padx=(6,6), pady=(3,3))
 		btn_frame = tk.Frame(self.dlg, borderwidth=3, relief=tk.RIDGE)
 		btn_frame.columnconfigure(0, weight=1)
 		btn_frame.grid(row=1, column=0, sticky=tk.EW, pady=(3,3))
+		btn_frame.columnconfigure(0, weight=1)
 		# Buttons
 		self.canceled = False
 		ok_btn = ttk.Button(btn_frame, text="Close", command=self.do_select)
 		ok_btn.grid(row=0, column=0, sticky=tk.E, padx=(6,6))
 		self.dlg.bind("<Return>", self.do_select)
 		self.dlg.bind("<Escape>", self.do_select)
 	def do_select(self, *args):
```

### Comparing `mapdata-1.8.1/mapdata.egg-info/PKG-INFO` & `mapdata-1.8.2/mapdata.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapdata
-Version: 1.8.1
+Version: 1.8.2
 Summary: An interactive map and table explorer for geographic coordinates in a CSV file
 Home-page: https://osdn.net/project/mapdata/
 Author: Dreas Nielsen
 Author-email: dreas.nielsen@gmail.com
 License: GPL
 Keywords: Map,Locations,CRS,CSV,PNG,JPG,Postscript
 Platform: UNKNOWN
```

### Comparing `mapdata-1.8.1/setup.py` & `mapdata-1.8.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 import io
 
 with io.open('README.md', encoding='utf-8') as f:
 	long_description = f.read()
 
 setuptools.setup(name='mapdata',
-	version='1.8.1',
+	version='1.8.2',
 	description="An interactive map and table explorer for geographic coordinates in a CSV file",
 	author='Dreas Nielsen',
 	author_email='dreas.nielsen@gmail.com',
     url='https://osdn.net/project/mapdata/',
 	scripts=['mapdata/mapdata.py'],
     license='GPL',
 	requires=['tkintermapview', 'pyproj', 'odfpy'],
```

