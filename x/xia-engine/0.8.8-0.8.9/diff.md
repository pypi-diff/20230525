# Comparing `tmp/xia_engine-0.8.8-cp39-none-win_amd64.whl.zip` & `tmp/xia_engine-0.8.9-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 1262622 bytes, number of entries: 12
--rw-r--r--  2.0 unx     1417 b- defN 23-May-01 14:59 xia_engine/__init__.py
--rw-r--r--  2.0 unx   461312 b- defN 23-May-01 15:04 xia_engine/acl.cp39-win_amd64.pyd
--rw-r--r--  2.0 unx   594432 b- defN 23-May-01 15:03 xia_engine/base.cp39-win_amd64.pyd
--rw-r--r--  2.0 unx   798208 b- defN 23-May-01 15:09 xia_engine/document.cp39-win_amd64.pyd
--rw-r--r--  2.0 unx   750592 b- defN 23-May-01 15:07 xia_engine/engine.cp39-win_amd64.pyd
--rw-r--r--  2.0 unx   262144 b- defN 23-May-01 15:10 xia_engine/exception.cp39-win_amd64.pyd
--rw-r--r--  2.0 unx   462848 b- defN 23-May-01 15:05 xia_engine/fields.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      152 b- defN 23-May-01 15:10 xia_engine-0.8.8.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      745 b- defN 23-May-01 15:10 xia_engine-0.8.8.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-May-01 15:10 xia_engine-0.8.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-May-01 15:10 xia_engine-0.8.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1052 b- defN 23-May-01 15:10 xia_engine-0.8.8.dist-info/RECORD
-12 files, 3333012 bytes uncompressed, 1260856 bytes compressed:  62.2%
+Zip file size: 1262837 bytes, number of entries: 12
+-rw-r--r--  2.0 unx     1417 b- defN 23-May-02 16:31 xia_engine/__init__.py
+-rw-r--r--  2.0 unx   461312 b- defN 23-May-02 16:37 xia_engine/acl.cp39-win_amd64.pyd
+-rw-r--r--  2.0 unx   594432 b- defN 23-May-02 16:35 xia_engine/base.cp39-win_amd64.pyd
+-rw-r--r--  2.0 unx   798208 b- defN 23-May-02 16:41 xia_engine/document.cp39-win_amd64.pyd
+-rw-r--r--  2.0 unx   750592 b- defN 23-May-02 16:40 xia_engine/engine.cp39-win_amd64.pyd
+-rw-r--r--  2.0 unx   262144 b- defN 23-May-02 16:42 xia_engine/exception.cp39-win_amd64.pyd
+-rw-r--r--  2.0 unx   463872 b- defN 23-May-02 16:38 xia_engine/fields.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 unx      152 b- defN 23-May-02 16:42 xia_engine-0.8.9.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      745 b- defN 23-May-02 16:42 xia_engine-0.8.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-May-02 16:42 xia_engine-0.8.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-May-02 16:42 xia_engine-0.8.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1052 b- defN 23-May-02 16:42 xia_engine-0.8.9.dist-info/RECORD
+12 files, 3334036 bytes uncompressed, 1261071 bytes compressed:  62.2%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: xia_engine/exception.cp39-win_amd64.pyd
 Comment: 
 
 Filename: xia_engine/fields.cp39-win_amd64.pyd
 Comment: 
 
-Filename: xia_engine-0.8.8.dist-info/LICENSE.txt
+Filename: xia_engine-0.8.9.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_engine-0.8.8.dist-info/METADATA
+Filename: xia_engine-0.8.9.dist-info/METADATA
 Comment: 
 
-Filename: xia_engine-0.8.8.dist-info/WHEEL
+Filename: xia_engine-0.8.9.dist-info/WHEEL
 Comment: 
 
-Filename: xia_engine-0.8.8.dist-info/top_level.txt
+Filename: xia_engine-0.8.9.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_engine-0.8.8.dist-info/RECORD
+Filename: xia_engine-0.8.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_engine/__init__.py

```diff
@@ -20,8 +20,8 @@
     "MetaEngine", "MetaRamEngine", "MetaCache",
     "Acl", "AclItem",
     "XiaError", 'AuthorizationError', 'AuthenticationError', "OutOfScopeError",
     'NotFoundError', 'ConflictError', 'BadRequestError', "UnprocessableError",
     "ServerError"
 ]
 
-__version__ = "0.8.8"
+__version__ = "0.8.9"
```

## Comparing `xia_engine-0.8.8.dist-info/METADATA` & `xia_engine-0.8.9.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xia-engine
-Version: 0.8.8
+Version: 0.8.9
 Summary: X-I-A Engine
-Home-page: https://develop.x-i-a.com/docs/xia-engine/0.8.8/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-engine/0.8.9/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

## Comparing `xia_engine-0.8.8.dist-info/RECORD` & `xia_engine-0.8.9.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-xia_engine/__init__.py,sha256=tYJku76i67v2J0fzKG7ZB2_-6j0axcK65W9XqcsWFv4,1417
-xia_engine/acl.cp39-win_amd64.pyd,sha256=oj0mAiojCnycPhrn9NX52X8bVN57aaYdZEmekSEWjaU,461312
-xia_engine/base.cp39-win_amd64.pyd,sha256=h-iVq996k4x7EMkrV1rCc95RjTmZLMjxC_4022GszvI,594432
-xia_engine/document.cp39-win_amd64.pyd,sha256=qKIGb7itAyJ83wT_iDWSDYp4Jgr3hxXY2HsxSGUzjug,798208
-xia_engine/engine.cp39-win_amd64.pyd,sha256=dW7TpecM3MnH01Etv5fvNeW-rGO-haDIu418XlFSzIo,750592
-xia_engine/exception.cp39-win_amd64.pyd,sha256=Va0N0K5qDPayvdEdmwTxvaGJtG-0qanB1QxguIzwc74,262144
-xia_engine/fields.cp39-win_amd64.pyd,sha256=Xv5QiTSNP7sedh2hXWrbu96pR7xY930NFkzwEiW7-ic,462848
-xia_engine-0.8.8.dist-info/LICENSE.txt,sha256=30wWxpufZqbxK7WdwZRoX8iA_veQA4gbl5oih3j5vFs,152
-xia_engine-0.8.8.dist-info/METADATA,sha256=R9gbMtIEa5C6i72Fp7XBbj04VUzewGBORvg9t34Aqdc,745
-xia_engine-0.8.8.dist-info/WHEEL,sha256=T8VPDjot1YI5-NaRzS6kIMlJNVl0SSGa_dm-8Fprszg,99
-xia_engine-0.8.8.dist-info/top_level.txt,sha256=Q896WUzHNHm14oiEaw7BbLcGbvHkKPKEQOBa8Z06dbk,11
-xia_engine-0.8.8.dist-info/RECORD,,
+xia_engine/__init__.py,sha256=OU49Po1FSu9PjmrRF60dOOyTGCAw9XMoExoZZm0EVZA,1417
+xia_engine/acl.cp39-win_amd64.pyd,sha256=3jFfrnGfCQzwjBC10gIoOZrXaSEFZAdCkg1j5ryCkbI,461312
+xia_engine/base.cp39-win_amd64.pyd,sha256=E8jGNQ5lHclOYiNghOIuwfYBYOEIKScxu3NVopBWMro,594432
+xia_engine/document.cp39-win_amd64.pyd,sha256=Ay9XP0ly0fCVEpg-Fq1TqYU0HNy22tYuF9dZNsnsa-8,798208
+xia_engine/engine.cp39-win_amd64.pyd,sha256=5_NR7iMXKdgQproAiqD8Qjf1MXXQYPE5NbGnz1K04ss,750592
+xia_engine/exception.cp39-win_amd64.pyd,sha256=1_t_msCW8dy5CdQb2gRvX7vVqhiD5U5scpapLQxZ6ks,262144
+xia_engine/fields.cp39-win_amd64.pyd,sha256=e00HIlaZvv89rIUm3Xy0eMwnkA9t3ZyB7XKg_ZgAQMc,463872
+xia_engine-0.8.9.dist-info/LICENSE.txt,sha256=30wWxpufZqbxK7WdwZRoX8iA_veQA4gbl5oih3j5vFs,152
+xia_engine-0.8.9.dist-info/METADATA,sha256=0LAV5djPVByU2A7_fLz9X9i7IzcOzghptku71GLDTuY,745
+xia_engine-0.8.9.dist-info/WHEEL,sha256=T8VPDjot1YI5-NaRzS6kIMlJNVl0SSGa_dm-8Fprszg,99
+xia_engine-0.8.9.dist-info/top_level.txt,sha256=Q896WUzHNHm14oiEaw7BbLcGbvHkKPKEQOBa8Z06dbk,11
+xia_engine-0.8.9.dist-info/RECORD,,
```

