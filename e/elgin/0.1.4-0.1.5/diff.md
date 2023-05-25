# Comparing `tmp/elgin-0.1.4-py3-none-any.whl.zip` & `tmp/elgin-0.1.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,10 @@
-Zip file size: 5391 bytes, number of entries: 6
+Zip file size: 7832 bytes, number of entries: 8
 -rw-r--r--  2.0 unx        0 b- defN 23-May-24 18:41 elgin/__init__.py
 -rw-r--r--  2.0 unx    12044 b- defN 23-May-25 15:44 elgin/monitoramento.py
--rw-r--r--  2.0 unx     2430 b- defN 23-May-25 15:44 elgin-0.1.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-25 15:44 elgin-0.1.4.dist-info/WHEEL
--rw-r--r--  2.0 unx        6 b- defN 23-May-25 15:44 elgin-0.1.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      440 b- defN 23-May-25 15:44 elgin-0.1.4.dist-info/RECORD
-6 files, 15012 bytes uncompressed, 4595 bytes compressed:  69.4%
+-rw-r--r--  2.0 unx     3978 b- defN 23-May-24 18:09 elgin/templates/template_email_log.html
+-rw-r--r--  2.0 unx     4019 b- defN 23-May-24 20:41 elgin/templates/template_teams.json
+-rw-r--r--  2.0 unx     2430 b- defN 23-May-25 15:55 elgin-0.1.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-25 15:55 elgin-0.1.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx        6 b- defN 23-May-25 15:55 elgin-0.1.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      628 b- defN 23-May-25 15:55 elgin-0.1.5.dist-info/RECORD
+8 files, 23197 bytes uncompressed, 6736 bytes compressed:  71.0%
```

## zipnote {}

```diff
@@ -1,19 +1,25 @@
 Filename: elgin/__init__.py
 Comment: 
 
 Filename: elgin/monitoramento.py
 Comment: 
 
-Filename: elgin-0.1.4.dist-info/METADATA
+Filename: elgin/templates/template_email_log.html
 Comment: 
 
-Filename: elgin-0.1.4.dist-info/WHEEL
+Filename: elgin/templates/template_teams.json
 Comment: 
 
-Filename: elgin-0.1.4.dist-info/top_level.txt
+Filename: elgin-0.1.5.dist-info/METADATA
 Comment: 
 
-Filename: elgin-0.1.4.dist-info/RECORD
+Filename: elgin-0.1.5.dist-info/WHEEL
+Comment: 
+
+Filename: elgin-0.1.5.dist-info/top_level.txt
+Comment: 
+
+Filename: elgin-0.1.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `elgin-0.1.4.dist-info/METADATA` & `elgin-0.1.5.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elgin
-Version: 0.1.4
+Version: 0.1.5
 Summary: Biblioteca responsavel por gerar o monitoramento dos processos da empresa elgin.
 Home-page: UNKNOWN
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

