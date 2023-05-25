# Comparing `tmp/mb_pandas-1.0.202304041351-py3-none-any.whl.zip` & `tmp/mb_pandas-1.0.202305250337-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 9348 bytes, number of entries: 13
+Zip file size: 9302 bytes, number of entries: 13
 -rw-rw-r--  2.0 unx       43 b- defN 23-Mar-10 04:05 mb_pandas/src/__init__.py
--rw-rw-r--  2.0 unx     1627 b- defN 22-Nov-28 03:21 mb_pandas/src/aio.py
--rw-rw-r--  2.0 unx      501 b- defN 23-Mar-14 16:03 mb_pandas/src/convert_data.py
--rw-rw-r--  2.0 unx     3459 b- defN 23-Apr-04 01:24 mb_pandas/src/dfload.py
--rw-rw-r--  2.0 unx     2458 b- defN 22-Nov-27 20:00 mb_pandas/src/profiler.py
--rw-rw-r--  2.0 unx     6094 b- defN 23-Mar-14 16:05 mb_pandas/src/transform.py
--rw-rw-r--  2.0 unx      396 b- defN 23-Apr-04 13:51 mb_pandas/src/version.py
--rwxrwxr-x  2.0 unx     1671 b- defN 23-Apr-04 13:51 mb_pandas-1.0.202304041351.data/scripts/df_profile
--rwxrwxr-x  2.0 unx     3683 b- defN 23-Apr-04 13:51 mb_pandas-1.0.202304041351.data/scripts/df_view
--rw-rw-r--  2.0 unx      224 b- defN 23-Apr-04 13:51 mb_pandas-1.0.202304041351.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Apr-04 13:51 mb_pandas-1.0.202304041351.dist-info/WHEEL
--rw-rw-r--  2.0 unx       10 b- defN 23-Apr-04 13:51 mb_pandas-1.0.202304041351.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1127 b- defN 23-Apr-04 13:51 mb_pandas-1.0.202304041351.dist-info/RECORD
-13 files, 21385 bytes uncompressed, 7440 bytes compressed:  65.2%
+-rw-rw-r--  2.0 unx     1612 b- defN 23-May-25 03:36 mb_pandas/src/aio.py
+-rw-rw-r--  2.0 unx      482 b- defN 23-May-25 03:36 mb_pandas/src/convert_data.py
+-rw-rw-r--  2.0 unx     3451 b- defN 23-May-25 03:36 mb_pandas/src/dfload.py
+-rw-rw-r--  2.0 unx     2418 b- defN 23-May-25 03:36 mb_pandas/src/profiler.py
+-rw-rw-r--  2.0 unx     6091 b- defN 23-Apr-04 14:19 mb_pandas/src/transform.py
+-rw-rw-r--  2.0 unx      396 b- defN 23-May-25 03:37 mb_pandas/src/version.py
+-rwxrwxr-x  2.0 unx     1671 b- defN 23-May-25 03:37 mb_pandas-1.0.202305250337.data/scripts/df_profile
+-rwxrwxr-x  2.0 unx     3683 b- defN 23-May-25 03:37 mb_pandas-1.0.202305250337.data/scripts/df_view
+-rw-rw-r--  2.0 unx      224 b- defN 23-May-25 03:37 mb_pandas-1.0.202305250337.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-25 03:37 mb_pandas-1.0.202305250337.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       10 b- defN 23-May-25 03:37 mb_pandas-1.0.202305250337.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1127 b- defN 23-May-25 03:37 mb_pandas-1.0.202305250337.dist-info/RECORD
+13 files, 21300 bytes uncompressed, 7394 bytes compressed:  65.3%
```

## zipnote {}

```diff
@@ -15,26 +15,26 @@
 
 Filename: mb_pandas/src/transform.py
 Comment: 
 
 Filename: mb_pandas/src/version.py
 Comment: 
 
-Filename: mb_pandas-1.0.202304041351.data/scripts/df_profile
+Filename: mb_pandas-1.0.202305250337.data/scripts/df_profile
 Comment: 
 
-Filename: mb_pandas-1.0.202304041351.data/scripts/df_view
+Filename: mb_pandas-1.0.202305250337.data/scripts/df_view
 Comment: 
 
-Filename: mb_pandas-1.0.202304041351.dist-info/METADATA
+Filename: mb_pandas-1.0.202305250337.dist-info/METADATA
 Comment: 
 
-Filename: mb_pandas-1.0.202304041351.dist-info/WHEEL
+Filename: mb_pandas-1.0.202305250337.dist-info/WHEEL
 Comment: 
 
-Filename: mb_pandas-1.0.202304041351.dist-info/top_level.txt
+Filename: mb_pandas-1.0.202305250337.dist-info/top_level.txt
 Comment: 
 
-Filename: mb_pandas-1.0.202304041351.dist-info/RECORD
+Filename: mb_pandas-1.0.202305250337.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mb_pandas/src/aio.py

```diff
@@ -1,8 +1,7 @@
-import asyncio
 import aiofiles 
 
 __all__ = ['srun','read_text']
 
 def srun(async_func, *args,extra_context_var: dict={} ,show_progress=False, **kwargs):
     """
     Run asyncio function in synchronous way
```

## mb_pandas/src/convert_data.py

```diff
@@ -1,22 +1,22 @@
 import ast
-from mb_utils.src.logging import logger
 import pandas as pd
 
 
 __all__ = ['convert_string_to_list']
 
-def convert_string_to_list(df,column,logger =None):
+def convert_string_to_list(df,logger =None):
     """
-    Input
-    df (pd.DataFrame): pandas dataframe
-    column (str): column name
-    logger (logger): logger
+    Convert string to list data of a column
     
-    OutPut:
+    Input:
+        df (pd.DataFrame): pandas dataframe
+        logger (logger): logger
+    
+    Output:
         df (pd.DataFrame): pandas dataframe
     """
 
     df_l = list(df['columns'])
     df_l2 = [ast.literal_eval(i) for i in range(len(df_l))]
     df2 = df.copy()
     df2['columns'] = df_l2
```

## mb_pandas/src/dfload.py

```diff
@@ -78,17 +78,17 @@
         show_progress (bool): show progress bar
         literal_ast_columns (list): columns to be converted to literal ast
         logger (logger): logger object
     Output:
         df (pd.DataFrame): pandas dataframe
     """
     try:
-        if file_path.str.endswith('.csv'):
+        if file_path.endswith('.csv'):
             df = asyncio.run(load_df_new(file_path,show_progress=show_progress))
-        elif file_path.str.endswith('.parquet'):
+        elif file_path.endswith('.parquet'):
             df = asyncio.run(load_df_new_parquet(file_path,show_progress=show_progress))
         if logger:
             logger.info("Loaded dataframe from {} using asyncio".format(file_path))
     except:
         raise ValueError("File type not supported")
     
     #df = df.reset_index(drop=True)
```

## mb_pandas/src/profiler.py

```diff
@@ -1,10 +1,9 @@
 ##pandas file profilier functions
 import pandas as pd
-from mb_utils.src.logging import logger
 
 __all__ = ['create_profile','profile_compare']
 
 def create_profile(df,profile_name='./pandas_profiling_report.html',minimal=False,target=[],logger=None):
     """
     Create pandas profiling report
     Input:
```

## mb_pandas/src/transform.py

```diff
@@ -124,15 +124,15 @@
         the type of the series. If it is a normal series, the string representing the dtype
         attribute of the series is returned
     '''
     if len(s) == 0:
         return 'object'
 
     dftype = None
-    for x in s.tolist():
+    for x in list(s):
         if isinstance(x, str):
             if dftype is None:
                 dftype = 'str'
             elif dftype != 'str':
                 break
             continue
         if isinstance(x, (list, dict)):
```

## mb_pandas/src/version.py

```diff
@@ -1,11 +1,11 @@
 VERSION_YEAR = 2023
-VERSION_MONTH = int('04')
-VERSION_DAY = int('04')
-VERSION_HOUR = int('13')
-VERSION_MINUTE = int('51')
+VERSION_MONTH = int('05')
+VERSION_DAY = int('25')
+VERSION_HOUR = int('03')
+VERSION_MINUTE = int('37')
 MAJOR_VERSION = 1
 MINOR_VERSION = 0
-PATCH_VERSION = 202304041351
-version_date = '2023/04/04 13:51'
+PATCH_VERSION = 202305250337
+version_date = '2023/05/25 03:37'
 version = '{}.{}.{}'.format(MAJOR_VERSION, MINOR_VERSION, PATCH_VERSION)
 __all__  = ['MAJOR_VERSION', 'MINOR_VERSION', 'PATCH_VERSION', 'version_date', 'version']
```

## Comparing `mb_pandas-1.0.202304041351.data/scripts/df_profile` & `mb_pandas-1.0.202305250337.data/scripts/df_profile`

 * *Files identical despite different names*

## Comparing `mb_pandas-1.0.202304041351.data/scripts/df_view` & `mb_pandas-1.0.202305250337.data/scripts/df_view`

 * *Files identical despite different names*

## Comparing `mb_pandas-1.0.202304041351.dist-info/RECORD` & `mb_pandas-1.0.202305250337.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 mb_pandas/src/__init__.py,sha256=16ZetnIdcpfU3bmRa_MNC07b0I9bZWeJLSvN4UvCEHk,43
-mb_pandas/src/aio.py,sha256=cXeSQ0wMw_yNPe33dJu-RyVA1q3DkwGzUxG-uh3cPI0,1627
-mb_pandas/src/convert_data.py,sha256=mnRBGl-njTMMyMLQo2DgSHUHJVmQsULrGzQvwyjMNTo,501
-mb_pandas/src/dfload.py,sha256=nbXqX5TfmZyG_wXyESj1DFEd-0dEw7c2ast5YkJ48sQ,3459
-mb_pandas/src/profiler.py,sha256=m7-S0es-GhoUqKUMw1Avcox3DG0evfLTXv-5A1K4tXc,2458
-mb_pandas/src/transform.py,sha256=4gzASZnzyDcuLvyAvASkVqVmzbnDs3kNYoGQItociOQ,6094
-mb_pandas/src/version.py,sha256=qLDbNeL063uXHMTt_9Bc8Qxf3TnmJPS_cyeMtijVwEo,396
-mb_pandas-1.0.202304041351.data/scripts/df_profile,sha256=zi4GRNQ6P5_JEB_0wMYB1KzLRG59eHXxRZG_I84lTYQ,1671
-mb_pandas-1.0.202304041351.data/scripts/df_view,sha256=BbS_rNgrPl7Raz_zVmTBqw_dvyAhc3-KqS4W2LV0_yo,3683
-mb_pandas-1.0.202304041351.dist-info/METADATA,sha256=LpyRV1lhgUh5gmbNHNcRR04rA_5Gq-3Y1Zk_2uby-30,224
-mb_pandas-1.0.202304041351.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-mb_pandas-1.0.202304041351.dist-info/top_level.txt,sha256=5JkDz2-6yNAp6GiwpeR4FpxqXVysaksS5MD1iAvfMgo,10
-mb_pandas-1.0.202304041351.dist-info/RECORD,,
+mb_pandas/src/aio.py,sha256=UK3o2TMFDeNQvhiFAulAyd1fKJPjrShEbK-Y-85tlsM,1612
+mb_pandas/src/convert_data.py,sha256=Wp1yDT9Ie-lBZGE7WmsMXB7nN3mv0MwbiloInr1aoc0,482
+mb_pandas/src/dfload.py,sha256=35lcohyvdhIx_a17FxHlCQ5gmSkyGczTG9mqzLFjFzw,3451
+mb_pandas/src/profiler.py,sha256=iX_nAksh-HzjyhQLnbutvEtNVGfVwja2CsQ1zaYZbeA,2418
+mb_pandas/src/transform.py,sha256=Pq-xTzpfktzAlpu4dg42Kd6uoSI5mcq8vHhetFhgDUM,6091
+mb_pandas/src/version.py,sha256=6SP1jioYCThALgM7Sw0MGMT5jVLfZ-8c56N63LQXOPw,396
+mb_pandas-1.0.202305250337.data/scripts/df_profile,sha256=zi4GRNQ6P5_JEB_0wMYB1KzLRG59eHXxRZG_I84lTYQ,1671
+mb_pandas-1.0.202305250337.data/scripts/df_view,sha256=BbS_rNgrPl7Raz_zVmTBqw_dvyAhc3-KqS4W2LV0_yo,3683
+mb_pandas-1.0.202305250337.dist-info/METADATA,sha256=b5PcXKuy6v2DVj37jdHN0NrTBngVTIxc6UrOEoh993A,224
+mb_pandas-1.0.202305250337.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+mb_pandas-1.0.202305250337.dist-info/top_level.txt,sha256=5JkDz2-6yNAp6GiwpeR4FpxqXVysaksS5MD1iAvfMgo,10
+mb_pandas-1.0.202305250337.dist-info/RECORD,,
```

