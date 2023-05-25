# Comparing `tmp/licensekeygentest-1.1.3.tar.gz` & `tmp/licensekeygentest-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "licensekeygentest-1.1.3.tar", last modified: Thu May 25 10:14:53 2023, max compression
+gzip compressed data, was "licensekeygentest-1.1.4.tar", last modified: Thu May 25 10:51:17 2023, max compression
```

## Comparing `licensekeygentest-1.1.3.tar` & `licensekeygentest-1.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 goofynugtz  (1000) goofynugtz  (1000)        0 2023-05-25 10:14:53.541572 licensekeygentest-1.1.3/
--rw-rw-r--   0 goofynugtz  (1000) goofynugtz  (1000)     1063 2023-05-23 11:20:36.000000 licensekeygentest-1.1.3/LICENSE
--rw-rw-r--   0 goofynugtz  (1000) goofynugtz  (1000)      699 2023-05-25 10:14:53.541572 licensekeygentest-1.1.3/PKG-INFO
--rw-rw-r--   0 goofynugtz  (1000) goofynugtz  (1000)      152 2023-05-23 11:20:36.000000 licensekeygentest-1.1.3/README.md
-drwxrwxr-x   0 goofynugtz  (1000) goofynugtz  (1000)        0 2023-05-25 10:14:53.541572 licensekeygentest-1.1.3/licensekeygentest/
--rw-rw-r--   0 goofynugtz  (1000) goofynugtz  (1000)       43 2023-05-23 11:20:36.000000 licensekeygentest-1.1.3/licensekeygentest/__init__.py
--rw-rw-r--   0 goofynugtz  (1000) goofynugtz  (1000)     4297 2023-05-25 10:07:43.000000 licensekeygentest-1.1.3/licensekeygentest/main.py
-drwxrwxr-x   0 goofynugtz  (1000) goofynugtz  (1000)        0 2023-05-25 10:14:53.541572 licensekeygentest-1.1.3/licensekeygentest.egg-info/
--rw-rw-r--   0 goofynugtz  (1000) goofynugtz  (1000)      699 2023-05-25 10:14:53.000000 licensekeygentest-1.1.3/licensekeygentest.egg-info/PKG-INFO
--rw-rw-r--   0 goofynugtz  (1000) goofynugtz  (1000)      286 2023-05-25 10:14:53.000000 licensekeygentest-1.1.3/licensekeygentest.egg-info/SOURCES.txt
--rw-rw-r--   0 goofynugtz  (1000) goofynugtz  (1000)        1 2023-05-25 10:14:53.000000 licensekeygentest-1.1.3/licensekeygentest.egg-info/dependency_links.txt
--rw-rw-r--   0 goofynugtz  (1000) goofynugtz  (1000)        9 2023-05-25 10:14:53.000000 licensekeygentest-1.1.3/licensekeygentest.egg-info/requires.txt
--rw-rw-r--   0 goofynugtz  (1000) goofynugtz  (1000)       18 2023-05-25 10:14:53.000000 licensekeygentest-1.1.3/licensekeygentest.egg-info/top_level.txt
--rw-rw-r--   0 goofynugtz  (1000) goofynugtz  (1000)       38 2023-05-25 10:14:53.541572 licensekeygentest-1.1.3/setup.cfg
--rw-rw-r--   0 goofynugtz  (1000) goofynugtz  (1000)     1063 2023-05-25 10:14:39.000000 licensekeygentest-1.1.3/setup.py
+drwxrwxr-x   0 goofynugtz  (1000) goofynugtz  (1000)        0 2023-05-25 10:51:17.410318 licensekeygentest-1.1.4/
+-rw-rw-r--   0 goofynugtz  (1000) goofynugtz  (1000)     1063 2023-05-23 11:20:36.000000 licensekeygentest-1.1.4/LICENSE
+-rw-rw-r--   0 goofynugtz  (1000) goofynugtz  (1000)      699 2023-05-25 10:51:17.410318 licensekeygentest-1.1.4/PKG-INFO
+-rw-rw-r--   0 goofynugtz  (1000) goofynugtz  (1000)      152 2023-05-23 11:20:36.000000 licensekeygentest-1.1.4/README.md
+drwxrwxr-x   0 goofynugtz  (1000) goofynugtz  (1000)        0 2023-05-25 10:51:17.406318 licensekeygentest-1.1.4/licensekeygentest/
+-rw-rw-r--   0 goofynugtz  (1000) goofynugtz  (1000)       43 2023-05-23 11:20:36.000000 licensekeygentest-1.1.4/licensekeygentest/__init__.py
+-rw-rw-r--   0 goofynugtz  (1000) goofynugtz  (1000)     4513 2023-05-25 10:49:12.000000 licensekeygentest-1.1.4/licensekeygentest/main.py
+drwxrwxr-x   0 goofynugtz  (1000) goofynugtz  (1000)        0 2023-05-25 10:51:17.410318 licensekeygentest-1.1.4/licensekeygentest.egg-info/
+-rw-rw-r--   0 goofynugtz  (1000) goofynugtz  (1000)      699 2023-05-25 10:51:17.000000 licensekeygentest-1.1.4/licensekeygentest.egg-info/PKG-INFO
+-rw-rw-r--   0 goofynugtz  (1000) goofynugtz  (1000)      286 2023-05-25 10:51:17.000000 licensekeygentest-1.1.4/licensekeygentest.egg-info/SOURCES.txt
+-rw-rw-r--   0 goofynugtz  (1000) goofynugtz  (1000)        1 2023-05-25 10:51:17.000000 licensekeygentest-1.1.4/licensekeygentest.egg-info/dependency_links.txt
+-rw-rw-r--   0 goofynugtz  (1000) goofynugtz  (1000)        9 2023-05-25 10:51:17.000000 licensekeygentest-1.1.4/licensekeygentest.egg-info/requires.txt
+-rw-rw-r--   0 goofynugtz  (1000) goofynugtz  (1000)       18 2023-05-25 10:51:17.000000 licensekeygentest-1.1.4/licensekeygentest.egg-info/top_level.txt
+-rw-rw-r--   0 goofynugtz  (1000) goofynugtz  (1000)       38 2023-05-25 10:51:17.410318 licensekeygentest-1.1.4/setup.cfg
+-rw-rw-r--   0 goofynugtz  (1000) goofynugtz  (1000)     1063 2023-05-25 10:51:01.000000 licensekeygentest-1.1.4/setup.py
```

### Comparing `licensekeygentest-1.1.3/LICENSE` & `licensekeygentest-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `licensekeygentest-1.1.3/PKG-INFO` & `licensekeygentest-1.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: licensekeygentest
-Version: 1.1.3
+Version: 1.1.4
 Summary: POC for license validation checks
 Author: Rahul R
 Author-email: <rahulranjan25.RR@gmail.com>
 Keywords: python,authentication,licensing
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `licensekeygentest-1.1.3/licensekeygentest/main.py` & `licensekeygentest-1.1.4/licensekeygentest/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,25 +30,25 @@
         if ________________________________________________________________________________________________________________________:
           print(f"[{____________________________________________________________________________________________________________________________________________________________________________________.status_code}] Response >> Status:", __)
 
         if (____________________________________________________________________________________________________________________________________________________________________________________.status_code != '200'):
           if (____________________________________________________________________________________________________________________________________________________________________________________.status_code/400 == 1):
             ___________()
 
-          _ =  __ == __________(b'Q&m$?MNULTL;') or __ == __________(b'NlsQlOi4r')   or __ == __________(b'MOaWtQbj}')   or __ == __________(b'RZ~S$UsFR*P(@!&NmEThR6|G')
+          _ =  __ == ________________(__________(b'Q&m$?MNULTL;')) or __ == ________________(__________(b'NlsQlOi4r'))   or __ == ________________(__________(b'MOaWtQbj}'))   or __ == ________________(__________(b'RZ~S$UsFR*P(@!&NmEThR6|G'))
           if _:
             ___________()
-            if __ == __________(b'Q&m$?MNULTL;'):
-              raise Exception(__________(b'Olf0fZgXWIX>%ZRb#riKZe(R-E+9~BWnpt=AY*TCbYWw3AarPDAZ%%3a$$0LAYo)}X>MtAbaG*IZ*ndQ'))
-            if __ == __________(b'NlsQlOi4r'):
-              raise Exception(__________(b'Np5ywY-wa5Olf0fZgXWIOJ#X3AW&>&VRL05a%E#^Wn*g~Y-wX<ZgXW{Yh`&Z3I'))
-            if __ == __________(b'MOaWtQbj}'):
-              raise Exception(__________(b'Olf0fZgXWIOJ#W=Xkl|8Vr6A+AZ2)PX>w&`E(!'))
-            if __ == __________(b'RZ~S$UsFR*P(@!&NmEThR6|G'):
-              raise Exception(__________(b'Np53ra&l#3bRcDIVQFk2X=E-SR%LQ&W_ciGZDDC_AZcVS3I'))
+            if __ == ________________(__________(b'Q&m$?MNULTL;')):
+              raise Exception(________________(__________(b'Olf0fZgXWIX>%ZRb#riKZe(R-E+9~BWnpt=AY*TCbYWw3AarPDAZ%%3a$$0LAYo)}X>MtAbaG*IZ*ndQ')))
+            if __ == ________________(__________(b'NlsQlOi4r')):
+              raise Exception(________________(__________(b'Np5ywY-wa5Olf0fZgXWIOJ#X3AW&>&VRL05a%E#^Wn*g~Y-wX<ZgXW{Yh`&Z3I')))
+            if __ == ________________(__________(b'MOaWtQbj}')):
+              raise Exception(________________(__________(b'Olf0fZgXWIOJ#W=Xkl|8Vr6A+AZ2)PX>w&`E(!')))
+            if __ == ________________(__________(b'RZ~S$UsFR*P(@!&NmEThR6|G')):
+              raise Exception(________________(__________(b'Np53ra&l#3bRcDIVQFk2X=E-SR%LQ&W_ciGZDDC_AZcVS3I')))
         # _________(60*60*24)
         _________(10)
 
       except _____:
         ___________()
         raise Exception(__________(b'Olf0fZgXWIc42I3WMOn^Z*CxRWpQ<7b95kMZ*^>BAZ~ATAYx@8ZDC|(E+9~BWnpt=AZ=l5Wgv5Pa%CWSZ*?GHa%CW6Z*Fd7V{~O?AarjabZBKDX>N37a&BdGE(!'))
```

### Comparing `licensekeygentest-1.1.3/licensekeygentest.egg-info/PKG-INFO` & `licensekeygentest-1.1.4/licensekeygentest.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: licensekeygentest
-Version: 1.1.3
+Version: 1.1.4
 Summary: POC for license validation checks
 Author: Rahul R
 Author-email: <rahulranjan25.RR@gmail.com>
 Keywords: python,authentication,licensing
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `licensekeygentest-1.1.3/setup.py` & `licensekeygentest-1.1.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.1.3'
+VERSION = '1.1.4'
 DESCRIPTION = 'POC for license validation checks'
 LONG_DESCRIPTION = 'A POC package that allows lisencing of python libraries.'
 
 # Setting up
 setup(
     name="licensekeygentest",
     version=VERSION,
```

