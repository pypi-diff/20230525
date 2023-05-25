# Comparing `tmp/decomp2dbg-3.3.1.tar.gz` & `tmp/decomp2dbg-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decomp2dbg-3.3.1.tar", last modified: Mon Feb 27 05:26:43 2023, max compression
+gzip compressed data, was "decomp2dbg-3.4.0.tar", last modified: Thu May 25 05:08:28 2023, max compression
```

## Comparing `decomp2dbg-3.3.1.tar` & `decomp2dbg-3.4.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 05:26:43.559395 decomp2dbg-3.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-02-27 05:26:35.000000 decomp2dbg-3.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-02-27 05:26:35.000000 decomp2dbg-3.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7294 2023-02-27 05:26:43.559395 decomp2dbg-3.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6870 2023-02-27 05:26:35.000000 decomp2dbg-3.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-02-27 05:26:35.000000 decomp2dbg-3.3.1/d2d.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 05:26:43.555395 decomp2dbg-3.3.1/decomp2dbg/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-02-27 05:26:35.000000 decomp2dbg-3.3.1/decomp2dbg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-02-27 05:26:35.000000 decomp2dbg-3.3.1/decomp2dbg/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 05:26:43.555395 decomp2dbg-3.3.1/decomp2dbg/clients/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-02-27 05:26:35.000000 decomp2dbg-3.3.1/decomp2dbg/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-02-27 05:26:35.000000 decomp2dbg-3.3.1/decomp2dbg/clients/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 05:26:43.555395 decomp2dbg-3.3.1/decomp2dbg/clients/gdb/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-02-27 05:26:35.000000 decomp2dbg-3.3.1/decomp2dbg/clients/gdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4875 2023-02-27 05:26:35.000000 decomp2dbg-3.3.1/decomp2dbg/clients/gdb/decompiler_pane.py
--rw-r--r--   0 runner    (1001) docker     (123)    11039 2023-02-27 05:26:35.000000 decomp2dbg-3.3.1/decomp2dbg/clients/gdb/gdb_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-02-27 05:26:35.000000 decomp2dbg-3.3.1/decomp2dbg/clients/gdb/gef_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-02-27 05:26:35.000000 decomp2dbg-3.3.1/decomp2dbg/clients/gdb/pwndbg_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9023 2023-02-27 05:26:35.000000 decomp2dbg-3.3.1/decomp2dbg/clients/gdb/symbol_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     8666 2023-02-27 05:26:35.000000 decomp2dbg-3.3.1/decomp2dbg/clients/gdb/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-02-27 05:26:35.000000 decomp2dbg-3.3.1/decomp2dbg/installer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5077 2023-02-27 05:26:35.000000 decomp2dbg-3.3.1/decomp2dbg/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 05:26:43.555395 decomp2dbg-3.3.1/decomp2dbg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7294 2023-02-27 05:26:43.000000 decomp2dbg-3.3.1/decomp2dbg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-02-27 05:26:43.000000 decomp2dbg-3.3.1/decomp2dbg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-27 05:26:43.000000 decomp2dbg-3.3.1/decomp2dbg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-02-27 05:26:43.000000 decomp2dbg-3.3.1/decomp2dbg.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-02-27 05:26:43.000000 decomp2dbg-3.3.1/decomp2dbg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-02-27 05:26:43.000000 decomp2dbg-3.3.1/decomp2dbg.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 05:26:43.555395 decomp2dbg-3.3.1/decompilers/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 05:26:43.555395 decomp2dbg-3.3.1/decompilers/d2d_angr/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-02-27 05:26:35.000000 decomp2dbg-3.3.1/decompilers/d2d_angr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-02-27 05:26:35.000000 decomp2dbg-3.3.1/decompilers/d2d_angr/d2d_angr.py
--rw-r--r--   0 runner    (1001) docker     (123)     5602 2023-02-27 05:26:35.000000 decomp2dbg-3.3.1/decompilers/d2d_angr/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 05:26:43.559395 decomp2dbg-3.3.1/decompilers/d2d_binja/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-27 05:26:35.000000 decomp2dbg-3.3.1/decompilers/d2d_binja/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5478 2023-02-27 05:26:35.000000 decomp2dbg-3.3.1/decompilers/d2d_binja/d2d_binja.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-02-27 05:26:35.000000 decomp2dbg-3.3.1/decompilers/d2d_binja/plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-02-27 05:26:35.000000 decomp2dbg-3.3.1/decompilers/d2d_binja/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 05:26:43.559395 decomp2dbg-3.3.1/decompilers/d2d_ida/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 05:26:43.559395 decomp2dbg-3.3.1/decompilers/d2d_ida/d2d_ida/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-27 05:26:35.000000 decomp2dbg-3.3.1/decompilers/d2d_ida/d2d_ida/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6352 2023-02-27 05:26:35.000000 decomp2dbg-3.3.1/decompilers/d2d_ida/d2d_ida/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    10568 2023-02-27 05:26:35.000000 decomp2dbg-3.3.1/decompilers/d2d_ida/d2d_ida/server.py
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-02-27 05:26:35.000000 decomp2dbg-3.3.1/decompilers/d2d_ida/d2d_ida.py
--rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-02-27 05:26:35.000000 decomp2dbg-3.3.1/decompilers/server_template.py
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-02-27 05:26:43.559395 decomp2dbg-3.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-02-27 05:26:35.000000 decomp2dbg-3.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 05:08:28.674800 decomp2dbg-3.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-05-25 05:08:18.000000 decomp2dbg-3.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-25 05:08:18.000000 decomp2dbg-3.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7294 2023-05-25 05:08:28.674800 decomp2dbg-3.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6870 2023-05-25 05:08:18.000000 decomp2dbg-3.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-05-25 05:08:18.000000 decomp2dbg-3.4.0/d2d.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 05:08:28.670799 decomp2dbg-3.4.0/decomp2dbg/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-25 05:08:18.000000 decomp2dbg-3.4.0/decomp2dbg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-25 05:08:18.000000 decomp2dbg-3.4.0/decomp2dbg/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 05:08:28.674800 decomp2dbg-3.4.0/decomp2dbg/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-25 05:08:18.000000 decomp2dbg-3.4.0/decomp2dbg/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-05-25 05:08:18.000000 decomp2dbg-3.4.0/decomp2dbg/clients/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 05:08:28.674800 decomp2dbg-3.4.0/decomp2dbg/clients/gdb/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-25 05:08:18.000000 decomp2dbg-3.4.0/decomp2dbg/clients/gdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4875 2023-05-25 05:08:18.000000 decomp2dbg-3.4.0/decomp2dbg/clients/gdb/decompiler_pane.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11039 2023-05-25 05:08:18.000000 decomp2dbg-3.4.0/decomp2dbg/clients/gdb/gdb_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-05-25 05:08:18.000000 decomp2dbg-3.4.0/decomp2dbg/clients/gdb/gef_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-05-25 05:08:18.000000 decomp2dbg-3.4.0/decomp2dbg/clients/gdb/pwndbg_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9210 2023-05-25 05:08:18.000000 decomp2dbg-3.4.0/decomp2dbg/clients/gdb/symbol_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8666 2023-05-25 05:08:18.000000 decomp2dbg-3.4.0/decomp2dbg/clients/gdb/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-05-25 05:08:18.000000 decomp2dbg-3.4.0/decomp2dbg/installer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5077 2023-05-25 05:08:18.000000 decomp2dbg-3.4.0/decomp2dbg/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 05:08:28.674800 decomp2dbg-3.4.0/decomp2dbg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7294 2023-05-25 05:08:28.000000 decomp2dbg-3.4.0/decomp2dbg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-25 05:08:28.000000 decomp2dbg-3.4.0/decomp2dbg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 05:08:28.000000 decomp2dbg-3.4.0/decomp2dbg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-25 05:08:28.000000 decomp2dbg-3.4.0/decomp2dbg.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-25 05:08:28.000000 decomp2dbg-3.4.0/decomp2dbg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-25 05:08:28.000000 decomp2dbg-3.4.0/decomp2dbg.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 05:08:28.674800 decomp2dbg-3.4.0/decompilers/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 05:08:28.674800 decomp2dbg-3.4.0/decompilers/d2d_angr/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-25 05:08:18.000000 decomp2dbg-3.4.0/decompilers/d2d_angr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-05-25 05:08:18.000000 decomp2dbg-3.4.0/decompilers/d2d_angr/d2d_angr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5602 2023-05-25 05:08:18.000000 decomp2dbg-3.4.0/decompilers/d2d_angr/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 05:08:28.674800 decomp2dbg-3.4.0/decompilers/d2d_binja/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-25 05:08:18.000000 decomp2dbg-3.4.0/decompilers/d2d_binja/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5478 2023-05-25 05:08:18.000000 decomp2dbg-3.4.0/decompilers/d2d_binja/d2d_binja.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-05-25 05:08:18.000000 decomp2dbg-3.4.0/decompilers/d2d_binja/plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-05-25 05:08:18.000000 decomp2dbg-3.4.0/decompilers/d2d_binja/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 05:08:28.674800 decomp2dbg-3.4.0/decompilers/d2d_ida/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 05:08:28.674800 decomp2dbg-3.4.0/decompilers/d2d_ida/d2d_ida/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 05:08:18.000000 decomp2dbg-3.4.0/decompilers/d2d_ida/d2d_ida/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6352 2023-05-25 05:08:18.000000 decomp2dbg-3.4.0/decompilers/d2d_ida/d2d_ida/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10568 2023-05-25 05:08:18.000000 decomp2dbg-3.4.0/decompilers/d2d_ida/d2d_ida/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-25 05:08:18.000000 decomp2dbg-3.4.0/decompilers/d2d_ida/d2d_ida.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-05-25 05:08:18.000000 decomp2dbg-3.4.0/decompilers/server_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-05-25 05:08:28.674800 decomp2dbg-3.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-05-25 05:08:18.000000 decomp2dbg-3.4.0/setup.py
```

### Comparing `decomp2dbg-3.3.1/LICENSE` & `decomp2dbg-3.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `decomp2dbg-3.3.1/PKG-INFO` & `decomp2dbg-3.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decomp2dbg
-Version: 3.3.1
+Version: 3.4.0
 Summary: Symbol syncing framework for decompilers and debuggers
 Home-page: https://github.com/mahaloz/decomp2dbg
 License: BSD 2 Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Requires-Python: >=3.5
```

### Comparing `decomp2dbg-3.3.1/README.md` & `decomp2dbg-3.4.0/README.md`

 * *Files identical despite different names*

### Comparing `decomp2dbg-3.3.1/d2d.py` & `decomp2dbg-3.4.0/d2d.py`

 * *Files identical despite different names*

### Comparing `decomp2dbg-3.3.1/decomp2dbg/__main__.py` & `decomp2dbg-3.4.0/decomp2dbg/__main__.py`

 * *Files identical despite different names*

### Comparing `decomp2dbg-3.3.1/decomp2dbg/clients/client.py` & `decomp2dbg-3.4.0/decomp2dbg/clients/client.py`

 * *Files identical despite different names*

### Comparing `decomp2dbg-3.3.1/decomp2dbg/clients/gdb/decompiler_pane.py` & `decomp2dbg-3.4.0/decomp2dbg/clients/gdb/decompiler_pane.py`

 * *Files identical despite different names*

### Comparing `decomp2dbg-3.3.1/decomp2dbg/clients/gdb/gdb_client.py` & `decomp2dbg-3.4.0/decomp2dbg/clients/gdb/gdb_client.py`

 * *Files identical despite different names*

### Comparing `decomp2dbg-3.3.1/decomp2dbg/clients/gdb/gef_client.py` & `decomp2dbg-3.4.0/decomp2dbg/clients/gdb/gef_client.py`

 * *Files identical despite different names*

### Comparing `decomp2dbg-3.3.1/decomp2dbg/clients/gdb/pwndbg_client.py` & `decomp2dbg-3.4.0/decomp2dbg/clients/gdb/pwndbg_client.py`

 * *Files identical despite different names*

### Comparing `decomp2dbg-3.3.1/decomp2dbg/clients/gdb/symbol_mapper.py` & `decomp2dbg-3.4.0/decomp2dbg/clients/gdb/symbol_mapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from ...utils import *
 from .utils import *
 import tempfile
 from elftools.elf.elffile import ELFFile
+import shlex
+
 import gdb
 
 
 class SymbolMapper:
     """
     A binary search dict implementation for ranges. Symbols will map for a range and we need to
     be able to lookup addresses in the middle of the range fast
@@ -82,17 +84,20 @@
             #    addr_str = "{:#x}".format(addr)
             # relative addressing
             #else:
 
             # you always want relative adressing
             addr_str = ".text:{:#x}".format(addr)
 
+            # clean name
+            name = self._clean_string(name)
+
             # create a symbol command for the symbol
             objcopy_cmds.append(
-                "--add-symbol '{name}'={addr_str},global,{type_flag}".format(
+                '--add-symbol {name}={addr_str},global,{type_flag}'.format(
                     name=name, addr_str=addr_str, type_flag=typ
                 )
             )
 
             # batch commit
             if i > 1 and i % max_commit_size == 0:
                 # add the queued symbols
@@ -116,14 +121,18 @@
             self._objcopy = which("objcopy")
         except FileNotFoundError as e:
             err(f"Binutils binaries not found: {e}")
             return False
 
         return True
 
+    @staticmethod
+    def _clean_string(string: str):
+        return re.sub(r'[^\w_. -:]', '_', string)
+
     def _delete_old_sym_files(self):
         for sym_file in self._last_sym_files:
             try:
                 gdb.execute(f"remove-symbol-file {sym_file}")
             except Exception as e:
                 pass
```

### Comparing `decomp2dbg-3.3.1/decomp2dbg/clients/gdb/utils.py` & `decomp2dbg-3.4.0/decomp2dbg/clients/gdb/utils.py`

 * *Files identical despite different names*

### Comparing `decomp2dbg-3.3.1/decomp2dbg/installer.py` & `decomp2dbg-3.4.0/decomp2dbg/installer.py`

 * *Files identical despite different names*

### Comparing `decomp2dbg-3.3.1/decomp2dbg/utils.py` & `decomp2dbg-3.4.0/decomp2dbg/utils.py`

 * *Files identical despite different names*

### Comparing `decomp2dbg-3.3.1/decomp2dbg.egg-info/PKG-INFO` & `decomp2dbg-3.4.0/decomp2dbg.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decomp2dbg
-Version: 3.3.1
+Version: 3.4.0
 Summary: Symbol syncing framework for decompilers and debuggers
 Home-page: https://github.com/mahaloz/decomp2dbg
 License: BSD 2 Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Requires-Python: >=3.5
```

### Comparing `decomp2dbg-3.3.1/decomp2dbg.egg-info/SOURCES.txt` & `decomp2dbg-3.4.0/decomp2dbg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `decomp2dbg-3.3.1/decompilers/d2d_angr/d2d_angr.py` & `decomp2dbg-3.4.0/decompilers/d2d_angr/d2d_angr.py`

 * *Files identical despite different names*

### Comparing `decomp2dbg-3.3.1/decompilers/d2d_angr/server.py` & `decomp2dbg-3.4.0/decompilers/d2d_angr/server.py`

 * *Files identical despite different names*

### Comparing `decomp2dbg-3.3.1/decompilers/d2d_binja/d2d_binja.py` & `decomp2dbg-3.4.0/decompilers/d2d_binja/d2d_binja.py`

 * *Files identical despite different names*

### Comparing `decomp2dbg-3.3.1/decompilers/d2d_binja/plugin.json` & `decomp2dbg-3.4.0/decompilers/d2d_binja/plugin.json`

 * *Files identical despite different names*

### Comparing `decomp2dbg-3.3.1/decompilers/d2d_binja/server.py` & `decomp2dbg-3.4.0/decompilers/d2d_binja/server.py`

 * *Files identical despite different names*

### Comparing `decomp2dbg-3.3.1/decompilers/d2d_ida/d2d_ida/plugin.py` & `decomp2dbg-3.4.0/decompilers/d2d_ida/d2d_ida/plugin.py`

 * *Files identical despite different names*

### Comparing `decomp2dbg-3.3.1/decompilers/d2d_ida/d2d_ida/server.py` & `decomp2dbg-3.4.0/decompilers/d2d_ida/d2d_ida/server.py`

 * *Files identical despite different names*

### Comparing `decomp2dbg-3.3.1/decompilers/server_template.py` & `decomp2dbg-3.4.0/decompilers/server_template.py`

 * *Files identical despite different names*

### Comparing `decomp2dbg-3.3.1/setup.cfg` & `decomp2dbg-3.4.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `decomp2dbg-3.3.1/setup.py` & `decomp2dbg-3.4.0/setup.py`

 * *Files identical despite different names*

