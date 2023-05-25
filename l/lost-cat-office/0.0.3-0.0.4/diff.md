# Comparing `tmp/lost_cat_office-0.0.3.tar.gz` & `tmp/lost_cat_office-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lost_cat_office-0.0.3.tar", last modified: Fri Jan 27 00:09:06 2023, max compression
+gzip compressed data, was "lost_cat_office-0.0.4.tar", last modified: Thu May 25 15:31:13 2023, max compression
```

## Comparing `lost_cat_office-0.0.3.tar` & `lost_cat_office-0.0.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-01-27 00:09:06.918468 lost_cat_office-0.0.3/
--rw-rw-rw-   0        0        0     1093 2022-10-31 17:45:04.000000 lost_cat_office-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     2546 2023-01-27 00:09:06.914958 lost_cat_office-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      602 2023-01-17 20:30:49.000000 lost_cat_office-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-01-27 00:09:06.862832 lost_cat_office-0.0.3/lost_cat_office/
--rw-rw-rw-   0        0        0        0 2023-01-14 15:56:39.000000 lost_cat_office-0.0.3/lost_cat_office/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-27 00:09:06.878862 lost_cat_office-0.0.3/lost_cat_office/examples/
--rw-rw-rw-   0        0        0     4652 2023-01-20 00:17:28.000000 lost_cat_office-0.0.3/lost_cat_office/examples/run_azurescan.py
-drwxrwxrwx   0        0        0        0 2023-01-27 00:09:06.890397 lost_cat_office-0.0.3/lost_cat_office/parsers/
--rw-rw-rw-   0        0        0        0 2023-01-14 15:56:39.000000 lost_cat_office-0.0.3/lost_cat_office/parsers/__init__.py
--rw-rw-rw-   0        0        0     4725 2023-01-16 18:29:44.000000 lost_cat_office-0.0.3/lost_cat_office/parsers/pdf_parser.py
--rw-rw-rw-   0        0        0     3207 2023-01-16 16:35:51.000000 lost_cat_office-0.0.3/lost_cat_office/parsers/word_parser.py
-drwxrwxrwx   0        0        0        0 2023-01-27 00:09:06.900431 lost_cat_office-0.0.3/lost_cat_office/processors/
--rw-rw-rw-   0        0        0        0 2023-01-14 15:56:39.000000 lost_cat_office-0.0.3/lost_cat_office/processors/__init__.py
--rw-rw-rw-   0        0        0     7547 2023-01-16 16:35:51.000000 lost_cat_office-0.0.3/lost_cat_office/processors/azureblob_processor.py
--rw-rw-rw-   0        0        0     6842 2023-01-27 00:07:28.000000 lost_cat_office-0.0.3/lost_cat_office/processors/word_processor.py
-drwxrwxrwx   0        0        0        0 2023-01-27 00:09:06.905439 lost_cat_office-0.0.3/lost_cat_office/utils/
--rw-rw-rw-   0        0        0        0 2023-01-14 15:56:39.000000 lost_cat_office-0.0.3/lost_cat_office/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-27 00:09:06.876357 lost_cat_office-0.0.3/lost_cat_office.egg-info/
--rw-rw-rw-   0        0        0     2546 2023-01-27 00:09:06.000000 lost_cat_office-0.0.3/lost_cat_office.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      594 2023-01-27 00:09:06.000000 lost_cat_office-0.0.3/lost_cat_office.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-27 00:09:06.000000 lost_cat_office-0.0.3/lost_cat_office.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       71 2023-01-27 00:09:06.000000 lost_cat_office-0.0.3/lost_cat_office.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-01-27 00:09:06.000000 lost_cat_office-0.0.3/lost_cat_office.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1040 2023-01-27 00:07:48.000000 lost_cat_office-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-01-27 00:09:06.918468 lost_cat_office-0.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-01-27 00:09:06.907439 lost_cat_office-0.0.3/test/
--rw-rw-rw-   0        0        0     4489 2023-01-16 18:28:56.000000 lost_cat_office-0.0.3/test/test_pdf.py
+drwxrwxrwx   0        0        0        0 2023-05-25 15:31:13.161002 lost_cat_office-0.0.4/
+-rw-rw-rw-   0        0        0     1093 2022-10-31 17:45:04.000000 lost_cat_office-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     2546 2023-05-25 15:31:13.159002 lost_cat_office-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      602 2023-01-17 20:30:49.000000 lost_cat_office-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-25 15:31:13.106406 lost_cat_office-0.0.4/lost_cat_office/
+-rw-rw-rw-   0        0        0        0 2023-01-14 15:56:39.000000 lost_cat_office-0.0.4/lost_cat_office/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 15:31:13.122942 lost_cat_office-0.0.4/lost_cat_office/examples/
+-rw-rw-rw-   0        0        0     4652 2023-01-20 00:17:28.000000 lost_cat_office-0.0.4/lost_cat_office/examples/run_azurescan.py
+drwxrwxrwx   0        0        0        0 2023-05-25 15:31:13.132950 lost_cat_office-0.0.4/lost_cat_office/parsers/
+-rw-rw-rw-   0        0        0        0 2023-01-14 15:56:39.000000 lost_cat_office-0.0.4/lost_cat_office/parsers/__init__.py
+-rw-rw-rw-   0        0        0     8201 2023-05-23 18:09:11.000000 lost_cat_office-0.0.4/lost_cat_office/parsers/pdf_parser.py
+-rw-rw-rw-   0        0        0     3207 2023-01-16 16:35:51.000000 lost_cat_office-0.0.4/lost_cat_office/parsers/word_parser.py
+drwxrwxrwx   0        0        0        0 2023-05-25 15:31:13.143471 lost_cat_office-0.0.4/lost_cat_office/processors/
+-rw-rw-rw-   0        0        0        0 2023-01-14 15:56:39.000000 lost_cat_office-0.0.4/lost_cat_office/processors/__init__.py
+-rw-rw-rw-   0        0        0     7547 2023-01-16 16:35:51.000000 lost_cat_office-0.0.4/lost_cat_office/processors/azureblob_processor.py
+-rw-rw-rw-   0        0        0     7010 2023-03-30 18:55:16.000000 lost_cat_office-0.0.4/lost_cat_office/processors/word_processor.py
+drwxrwxrwx   0        0        0        0 2023-05-25 15:31:13.147993 lost_cat_office-0.0.4/lost_cat_office/utils/
+-rw-rw-rw-   0        0        0        0 2023-01-14 15:56:39.000000 lost_cat_office-0.0.4/lost_cat_office/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 15:31:13.120943 lost_cat_office-0.0.4/lost_cat_office.egg-info/
+-rw-rw-rw-   0        0        0     2546 2023-05-25 15:31:13.000000 lost_cat_office-0.0.4/lost_cat_office.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      594 2023-05-25 15:31:13.000000 lost_cat_office-0.0.4/lost_cat_office.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 15:31:13.000000 lost_cat_office-0.0.4/lost_cat_office.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       71 2023-05-25 15:31:13.000000 lost_cat_office-0.0.4/lost_cat_office.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-25 15:31:13.000000 lost_cat_office-0.0.4/lost_cat_office.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1040 2023-05-15 18:19:25.000000 lost_cat_office-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-25 15:31:13.161002 lost_cat_office-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-25 15:31:13.149997 lost_cat_office-0.0.4/test/
+-rw-rw-rw-   0        0        0     4489 2023-01-16 18:28:56.000000 lost_cat_office-0.0.4/test/test_pdf.py
```

### Comparing `lost_cat_office-0.0.3/LICENSE` & `lost_cat_office-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `lost_cat_office-0.0.3/PKG-INFO` & `lost_cat_office-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lost_cat_office
-Version: 0.0.3
+Version: 0.0.4
 Summary: Lost cat Office is a package containing office document parsers
 Author-email: Dreffed aka David Gloyn-Cox <dreffed@gmail.com>, Thoughtswin Systems Inc <david.gloyn-cox@thoughtswinsystems.com>
 License: MIT License
         
         Copyright (c) 2022 David Gloyn-Cox
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `lost_cat_office-0.0.3/README.md` & `lost_cat_office-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `lost_cat_office-0.0.3/lost_cat_office/examples/run_azurescan.py` & `lost_cat_office-0.0.4/lost_cat_office/examples/run_azurescan.py`

 * *Files identical despite different names*

### Comparing `lost_cat_office-0.0.3/lost_cat_office/parsers/word_parser.py` & `lost_cat_office-0.0.4/lost_cat_office/parsers/word_parser.py`

 * *Files identical despite different names*

### Comparing `lost_cat_office-0.0.3/lost_cat_office/processors/azureblob_processor.py` & `lost_cat_office-0.0.4/lost_cat_office/processors/azureblob_processor.py`

 * *Files identical despite different names*

### Comparing `lost_cat_office-0.0.3/lost_cat_office/processors/word_processor.py` & `lost_cat_office-0.0.4/lost_cat_office/processors/word_processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,28 +124,33 @@
             scan_q.join()
 
     def parser_file(self):
         """A parser scanner function, quick and dirty"""
         t_settings = self.settings.get("threads",{})
         self.input.put(self.semiphore)
 
+        _exts = []
+        for _src in self.settings.get("source",{}):
+            if _src.get("field","") == "key" and _src.get("select","") == "ext":
+                _exts.extend(_src.get("filter",[]))
+
         while self.input:
             try:
                 q_item = self.input.get(timeout=t_settings.get("timeout")) if self.input else None
                 if q_item == self.semiphore:
                     break
 
                 # if the user wants to kill the queue if there are not entries...
                 # requires timeout set, otherwise the queue get blocks...
                 if not q_item and self.settings.get("threads",{}).get("stop"):
                     break
 
                 _uri=q_item.get("uri")
                 _, _ext = os.path.splitext(_uri)
-                if _ext not in self.settings.get("source",{}).get("filter",[]):
+                if _ext not in _exts:
                     self.input(q_item)
                     break
 
                 if not os.path.exists(_uri):
                     # most likely a zipfile...
                     zf = zipfile.ZipFile(q_item.get("zipfile"))
                     file_data = zf.read(q_item.get("uri"))
```

### Comparing `lost_cat_office-0.0.3/lost_cat_office.egg-info/PKG-INFO` & `lost_cat_office-0.0.4/lost_cat_office.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lost-cat-office
-Version: 0.0.3
+Version: 0.0.4
 Summary: Lost cat Office is a package containing office document parsers
 Author-email: Dreffed aka David Gloyn-Cox <dreffed@gmail.com>, Thoughtswin Systems Inc <david.gloyn-cox@thoughtswinsystems.com>
 License: MIT License
         
         Copyright (c) 2022 David Gloyn-Cox
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `lost_cat_office-0.0.3/lost_cat_office.egg-info/SOURCES.txt` & `lost_cat_office-0.0.4/lost_cat_office.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lost_cat_office-0.0.3/pyproject.toml` & `lost_cat_office-0.0.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=61.0",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lost_cat_office"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Dreffed aka David Gloyn-Cox", email="dreffed@gmail.com" },
   { name="Thoughtswin Systems Inc", email="david.gloyn-cox@thoughtswinsystems.com" },
 ]
 description = "Lost cat Office is a package containing office document parsers"
 readme = "README.md"
 license = { file="LICENSE" }
```

### Comparing `lost_cat_office-0.0.3/test/test_pdf.py` & `lost_cat_office-0.0.4/test/test_pdf.py`

 * *Files identical despite different names*

