# Comparing `tmp/ScriptCollection-3.3.93-py3-none-any.whl.zip` & `tmp/ScriptCollection-3.3.94-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 57992 bytes, number of entries: 14
+Zip file size: 57989 bytes, number of entries: 14
 -rw-rw-rw-  2.0 fat    18064 b- defN 23-Mar-05 15:39 ScriptCollection/Executables.py
--rw-rw-rw-  2.0 fat    34139 b- defN 23-May-20 16:21 ScriptCollection/GeneralUtilities.py
+-rw-rw-rw-  2.0 fat    34149 b- defN 23-May-25 10:33 ScriptCollection/GeneralUtilities.py
 -rw-rw-rw-  2.0 fat     1937 b- defN 22-Aug-30 21:59 ScriptCollection/ProgramRunnerBase.py
 -rw-rw-rw-  2.0 fat     6273 b- defN 22-Oct-16 19:55 ScriptCollection/ProgramRunnerEpew.py
 -rw-rw-rw-  2.0 fat     3023 b- defN 22-Aug-30 21:59 ScriptCollection/ProgramRunnerPopen.py
--rw-rw-rw-  2.0 fat    86233 b- defN 23-May-23 21:53 ScriptCollection/ScriptCollectionCore.py
+-rw-rw-rw-  2.0 fat    86233 b- defN 23-May-25 10:33 ScriptCollection/ScriptCollectionCore.py
 -rw-rw-rw-  2.0 fat   130752 b- defN 23-May-23 21:53 ScriptCollection/TasksForCommonProjectStructure.py
 -rw-rw-rw-  2.0 fat     7918 b- defN 22-Aug-30 21:59 ScriptCollection/UpdateCertificates.py
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Aug-29 05:45 ScriptCollection/__init__.py
--rw-rw-rw-  2.0 fat     7864 b- defN 23-May-23 21:54 ScriptCollection-3.3.93.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-23 21:54 ScriptCollection-3.3.93.dist-info/WHEEL
--rw-rw-rw-  2.0 fat     1968 b- defN 23-May-23 21:54 ScriptCollection-3.3.93.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat       17 b- defN 23-May-23 21:54 ScriptCollection-3.3.93.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1295 b- defN 23-May-23 21:54 ScriptCollection-3.3.93.dist-info/RECORD
-14 files, 299575 bytes uncompressed, 55800 bytes compressed:  81.4%
+-rw-rw-rw-  2.0 fat     7864 b- defN 23-May-25 10:34 ScriptCollection-3.3.94.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-25 10:34 ScriptCollection-3.3.94.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat     1968 b- defN 23-May-25 10:34 ScriptCollection-3.3.94.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat       17 b- defN 23-May-25 10:34 ScriptCollection-3.3.94.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1295 b- defN 23-May-25 10:34 ScriptCollection-3.3.94.dist-info/RECORD
+14 files, 299585 bytes uncompressed, 55797 bytes compressed:  81.4%
```

## zipnote {}

```diff
@@ -21,23 +21,23 @@
 
 Filename: ScriptCollection/UpdateCertificates.py
 Comment: 
 
 Filename: ScriptCollection/__init__.py
 Comment: 
 
-Filename: ScriptCollection-3.3.93.dist-info/METADATA
+Filename: ScriptCollection-3.3.94.dist-info/METADATA
 Comment: 
 
-Filename: ScriptCollection-3.3.93.dist-info/WHEEL
+Filename: ScriptCollection-3.3.94.dist-info/WHEEL
 Comment: 
 
-Filename: ScriptCollection-3.3.93.dist-info/entry_points.txt
+Filename: ScriptCollection-3.3.94.dist-info/entry_points.txt
 Comment: 
 
-Filename: ScriptCollection-3.3.93.dist-info/top_level.txt
+Filename: ScriptCollection-3.3.94.dist-info/top_level.txt
 Comment: 
 
-Filename: ScriptCollection-3.3.93.dist-info/RECORD
+Filename: ScriptCollection-3.3.94.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ScriptCollection/GeneralUtilities.py

```diff
@@ -226,15 +226,15 @@
 
     @staticmethod
     @check_arguments
     def write_exception_to_stderr_with_traceback(exception: Exception, current_traceback=None, extra_message: str = None):
         GeneralUtilities.write_message_to_stderr("Exception(")
         GeneralUtilities.write_message_to_stderr("Type: " + str(type(exception)))
         GeneralUtilities.write_message_to_stderr("Message: " + str(exception))
-        if str is not None:
+        if extra_message is not None:
             GeneralUtilities.write_message_to_stderr("Extra-message: " + str(extra_message))
         if isinstance(exception, OSError):
             GeneralUtilities.write_message_to_stderr(GeneralUtilities.get_advanced_errormessage_for_os_error(exception))
         if current_traceback is not None:
             GeneralUtilities.write_message_to_stderr("Traceback: " + current_traceback.format_exc())
         GeneralUtilities.write_message_to_stderr(")")
```

## ScriptCollection/ScriptCollectionCore.py

```diff
@@ -21,15 +21,15 @@
 from PyPDF2 import PdfFileMerger
 from .GeneralUtilities import GeneralUtilities
 from .ProgramRunnerBase import ProgramRunnerBase
 from .ProgramRunnerPopen import ProgramRunnerPopen
 from .ProgramRunnerEpew import ProgramRunnerEpew, CustomEpewArgument
 
 
-version = "3.3.93"
+version = "3.3.94"
 __version__ = version
 
 
 class ScriptCollectionCore:
 
     # The purpose of this property is to use it when testing your code which uses scriptcollection for external program-calls.
     # Do not change this value for productive environments.
```

## Comparing `ScriptCollection-3.3.93.dist-info/METADATA` & `ScriptCollection-3.3.94.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ScriptCollection
-Version: 3.3.93
+Version: 3.3.94
 Summary: The ScriptCollection is the place for reusable scripts.
 Home-page: https://github.com/anionDev/ScriptCollection
 Author: Marius Göcke
 Author-email: marius.goecke@gmail.com
 Project-URL: Documentation, https://aniondev.github.io/ScriptCollectionReference/index.html
 Project-URL: Changelog, https://github.com/anionDev/ScriptCollection/tree/main/Other/Resources/Changelog
 Keywords: package release build management
```

## Comparing `ScriptCollection-3.3.93.dist-info/entry_points.txt` & `ScriptCollection-3.3.94.dist-info/entry_points.txt`

 * *Files identical despite different names*

## Comparing `ScriptCollection-3.3.93.dist-info/RECORD` & `ScriptCollection-3.3.94.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ScriptCollection/Executables.py,sha256=kXTIX92KLeFuxnYOlsyFs5lkznsxkuoBMVrV3OU7FZU,18064
-ScriptCollection/GeneralUtilities.py,sha256=7-KuXjS_S-oiMcMM9bEDGx8n4RlnGxGpqHdhXhN47I8,34139
+ScriptCollection/GeneralUtilities.py,sha256=RDK5DGX0GEu9dO9JKSRMZCrA_5rKuf12mvT8CE6vRQA,34149
 ScriptCollection/ProgramRunnerBase.py,sha256=2kyOuoM3oFjBfLc9Q5t5RTz7Ya2CjUxFtB1rBBDmnjU,1937
 ScriptCollection/ProgramRunnerEpew.py,sha256=ZiBZVMcsphmo49z2BwUwQYXo2uTKXPu33QW3IxCT46E,6273
 ScriptCollection/ProgramRunnerPopen.py,sha256=HOs1QVnXiQtwXy1_xvH79bWBdd0i-2tUyyLloQBvMto,3023
-ScriptCollection/ScriptCollectionCore.py,sha256=IoZc3kmwLjrP9QAeTU_clHWwHc3Np816lACKKhNC1F8,86233
+ScriptCollection/ScriptCollectionCore.py,sha256=JOu7QAP4B-iSYZcmS1_0NAcZBiSfvlXcF8NaJwjm26s,86233
 ScriptCollection/TasksForCommonProjectStructure.py,sha256=_R5kBf88cySZE_5q6Cch9eRddwbJrRzsBFTISVXFhr0,130752
 ScriptCollection/UpdateCertificates.py,sha256=Go-JJK-YTi7aBB1phlLxypa8GHkmFHBEPB0_TT9G-bw,7918
 ScriptCollection/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-ScriptCollection-3.3.93.dist-info/METADATA,sha256=vKTeuSCESq0cj4EsHBNWMF2f3QgdLXZSpQ4-Dyp6ZwA,7864
-ScriptCollection-3.3.93.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-ScriptCollection-3.3.93.dist-info/entry_points.txt,sha256=VIuxVCOpX38lSJUwRRENBNgcGKTIBxQyrCfbJVRHP8g,1968
-ScriptCollection-3.3.93.dist-info/top_level.txt,sha256=hY2hOVH0V0Ce51WB76zKkIWTUNwMUdHo4XDkR2vYVwg,17
-ScriptCollection-3.3.93.dist-info/RECORD,,
+ScriptCollection-3.3.94.dist-info/METADATA,sha256=MCJ65Y1i58EIE6aP7QJWH7mEq6Z6jS6_j0Atjdw6798,7864
+ScriptCollection-3.3.94.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+ScriptCollection-3.3.94.dist-info/entry_points.txt,sha256=VIuxVCOpX38lSJUwRRENBNgcGKTIBxQyrCfbJVRHP8g,1968
+ScriptCollection-3.3.94.dist-info/top_level.txt,sha256=hY2hOVH0V0Ce51WB76zKkIWTUNwMUdHo4XDkR2vYVwg,17
+ScriptCollection-3.3.94.dist-info/RECORD,,
```

