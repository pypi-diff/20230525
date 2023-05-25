# Comparing `tmp/towhee-1.0.0-py3-none-any.whl.zip` & `tmp/towhee-1.0.0rc1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 207391 bytes, number of entries: 144
+Zip file size: 207434 bytes, number of entries: 144
 -rw-r--r--  2.0 unx     2855 b- defN 23-Mar-21 08:26 towhee/__init__.py
 -rw-r--r--  2.0 unx      665 b- defN 23-Mar-21 08:26 towhee/__main__.py
 -rw-r--r--  2.0 unx      619 b- defN 23-Mar-21 08:26 towhee/command/__init__.py
 -rw-r--r--  2.0 unx     1627 b- defN 23-Mar-21 08:26 towhee/command/cmdline.py
 -rw-r--r--  2.0 unx     4668 b- defN 23-Mar-21 08:26 towhee/command/develop.py
 -rw-r--r--  2.0 unx     4223 b- defN 23-Mar-21 08:26 towhee/command/execute.py
 -rw-r--r--  2.0 unx     4908 b- defN 23-Mar-21 08:26 towhee/command/repo.py
@@ -133,14 +133,14 @@
 -rw-r--r--  2.0 unx     1102 b- defN 23-Mar-21 08:26 towhee/utils/singleton.py
 -rw-r--r--  2.0 unx     1538 b- defN 23-Mar-21 08:26 towhee/utils/triton_httpclient.py
 -rw-r--r--  2.0 unx     2535 b- defN 23-Mar-21 08:26 towhee/utils/yaml_utils.py
 -rw-r--r--  2.0 unx      592 b- defN 23-Mar-21 08:26 towhee/utils/thirdparty/__init__.py
 -rw-r--r--  2.0 unx      845 b- defN 23-Mar-21 08:26 towhee/utils/thirdparty/dill_util.py
 -rw-r--r--  2.0 unx     1230 b- defN 23-Mar-21 08:26 towhee/utils/thirdparty/ipython_utils.py
 -rw-r--r--  2.0 unx     1130 b- defN 23-Mar-21 08:26 towhee/utils/thirdparty/pandas_utils.py
--rw-r--r--  2.0 unx    11357 b- defN 23-May-25 11:24 towhee-1.0.0.dist-info/LICENSE
--rw-r--r--  2.0 unx    17245 b- defN 23-May-25 11:24 towhee-1.0.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-25 11:24 towhee-1.0.0.dist-info/WHEEL
--rw-r--r--  2.0 unx      114 b- defN 23-May-25 11:24 towhee-1.0.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        7 b- defN 23-May-25 11:24 towhee-1.0.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx    12812 b- defN 23-May-25 11:24 towhee-1.0.0.dist-info/RECORD
-144 files, 604561 bytes uncompressed, 187047 bytes compressed:  69.1%
+-rw-r--r--  2.0 unx    11357 b- defN 23-May-04 08:04 towhee-1.0.0rc1.dist-info/LICENSE
+-rw-r--r--  2.0 unx    17248 b- defN 23-May-04 08:04 towhee-1.0.0rc1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-04 08:04 towhee-1.0.0rc1.dist-info/WHEEL
+-rw-r--r--  2.0 unx      114 b- defN 23-May-04 08:04 towhee-1.0.0rc1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        7 b- defN 23-May-04 08:04 towhee-1.0.0rc1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx    12830 b- defN 23-May-04 08:04 towhee-1.0.0rc1.dist-info/RECORD
+144 files, 604582 bytes uncompressed, 187054 bytes compressed:  69.1%
```

## zipnote {}

```diff
@@ -408,26 +408,26 @@
 
 Filename: towhee/utils/thirdparty/ipython_utils.py
 Comment: 
 
 Filename: towhee/utils/thirdparty/pandas_utils.py
 Comment: 
 
-Filename: towhee-1.0.0.dist-info/LICENSE
+Filename: towhee-1.0.0rc1.dist-info/LICENSE
 Comment: 
 
-Filename: towhee-1.0.0.dist-info/METADATA
+Filename: towhee-1.0.0rc1.dist-info/METADATA
 Comment: 
 
-Filename: towhee-1.0.0.dist-info/WHEEL
+Filename: towhee-1.0.0rc1.dist-info/WHEEL
 Comment: 
 
-Filename: towhee-1.0.0.dist-info/entry_points.txt
+Filename: towhee-1.0.0rc1.dist-info/entry_points.txt
 Comment: 
 
-Filename: towhee-1.0.0.dist-info/top_level.txt
+Filename: towhee-1.0.0rc1.dist-info/top_level.txt
 Comment: 
 
-Filename: towhee-1.0.0.dist-info/RECORD
+Filename: towhee-1.0.0rc1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `towhee-1.0.0.dist-info/LICENSE` & `towhee-1.0.0rc1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `towhee-1.0.0.dist-info/METADATA` & `towhee-1.0.0rc1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: towhee
-Version: 1.0.0
+Version: 1.0.0rc1
 Summary: Towhee is a framework that helps you encode your unstructured data into embeddings.
 Home-page: https://github.com/towhee-io/towhee
 Author: Towhee Team
 Author-email: towhee-team@zilliz.com
 License: http://www.apache.org/licenses/LICENSE-2.0
 Platform: unix
 Platform: linux
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: towhee Version: 1.0.0 Summary: Towhee is a
+Metadata-Version: 2.1 Name: towhee Version: 1.0.0rc1 Summary: Towhee is a
 framework that helps you encode your unstructured data into embeddings. Home-
 page: https://github.com/towhee-io/towhee Author: Towhee Team Author-email:
 towhee-team@zilliz.com License: http://www.apache.org/licenses/LICENSE-2.0
 Platform: unix Platform: linux Platform: osx Platform: win32 Description-
 Content-Type: text/markdown License-File: LICENSE Requires-Dist: requests
 (>=2.12.5) Requires-Dist: tqdm (>=4.59.0) Requires-Dist: tabulate Requires-
 Dist: numpy Requires-Dist: twine Requires-Dist: contextvars ; python_version <=
```

## Comparing `towhee-1.0.0.dist-info/RECORD` & `towhee-1.0.0rc1.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -132,13 +132,13 @@
 towhee/utils/singleton.py,sha256=H3n3l8gicm-6udX0-2vNV-QysrNAhTBNut7OzTGJjAc,1102
 towhee/utils/triton_httpclient.py,sha256=qoafN9GXE--tZkqKGsqYoQho6-q7hicFwt9EDYCLCPg,1538
 towhee/utils/yaml_utils.py,sha256=qZ0Mvcbh_qD2ymgRMQyal8Cp6w3d3I4q6ttCoaA7WQ0,2535
 towhee/utils/thirdparty/__init__.py,sha256=CeCaoChD6XAbWtan8cl1tZ0mD2QokRuoG_IPrSqyvxk,592
 towhee/utils/thirdparty/dill_util.py,sha256=YwnUvKa9sm566UHE5mw_8Jmu8YYvaBgVhVr27ckFr-c,845
 towhee/utils/thirdparty/ipython_utils.py,sha256=r0coEqQidnouFbSzVx3Q_dSgu45PPnUgDZwiTcm-FuE,1230
 towhee/utils/thirdparty/pandas_utils.py,sha256=W_1RdRIuyZ95L2x2pv9xbvZRW6hvGMKJ2Y_PLO2hWvE,1130
-towhee-1.0.0.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-towhee-1.0.0.dist-info/METADATA,sha256=fwPLBE1tVb9Rga7R91muvr-_N63eMHhKprkfwWSrq50,17245
-towhee-1.0.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-towhee-1.0.0.dist-info/entry_points.txt,sha256=Li9rdXM7RZW5O7NR9d9OOQV9D99bK1Fv4BilWvB1btk,114
-towhee-1.0.0.dist-info/top_level.txt,sha256=s8O0-CAA8lmENHKY-FR5ojkSAmqEOEkrpg6ITjplm4A,7
-towhee-1.0.0.dist-info/RECORD,,
+towhee-1.0.0rc1.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+towhee-1.0.0rc1.dist-info/METADATA,sha256=5mNf8ngXj8nQZ8_D4L7a5nqwWbh6whxeox4uz9pjMN8,17248
+towhee-1.0.0rc1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+towhee-1.0.0rc1.dist-info/entry_points.txt,sha256=Li9rdXM7RZW5O7NR9d9OOQV9D99bK1Fv4BilWvB1btk,114
+towhee-1.0.0rc1.dist-info/top_level.txt,sha256=s8O0-CAA8lmENHKY-FR5ojkSAmqEOEkrpg6ITjplm4A,7
+towhee-1.0.0rc1.dist-info/RECORD,,
```

