# Comparing `tmp/bambu_qsar-0.0.8-py3-none-any.whl.zip` & `tmp/bambu_qsar-0.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,19 @@
-Zip file size: 10536 bytes, number of entries: 16
+Zip file size: 13169 bytes, number of entries: 17
 -rw-r--r--  2.0 unx       89 b- defN 22-Jan-13 19:57 bambu/__init__.py
 -rw-r--r--  2.0 unx      187 b- defN 22-Jan-12 18:25 bambu/logo.py
 -rw-r--r--  2.0 unx     3904 b- defN 22-Jan-14 18:51 bambu/download/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 22-Jan-14 16:01 bambu/models/__init__.py
+-rw-r--r--  2.0 unx     4433 b- defN 22-Jan-15 04:50 bambu/models/decision_tree.py
 -rw-r--r--  2.0 unx     2437 b- defN 22-Jan-14 17:22 bambu/predict/__init__.py
 -rw-r--r--  2.0 unx      837 b- defN 22-Jan-12 03:38 bambu/predict/run.py
--rw-r--r--  2.0 unx     4765 b- defN 22-Jan-14 16:59 bambu/preprocess/__init__.py
+-rw-r--r--  2.0 unx     5164 b- defN 22-Jan-19 17:15 bambu/preprocess/__init__.py
 -rw-r--r--  2.0 unx       46 b- defN 22-Jan-12 05:07 bambu/preprocess/preprocessors/__init__.py
 -rw-r--r--  2.0 unx      389 b- defN 22-Jan-12 17:52 bambu/preprocess/preprocessors/descriptors.py
 -rw-r--r--  2.0 unx      538 b- defN 22-Jan-12 03:38 bambu/preprocess/preprocessors/morgan.py
 -rw-r--r--  2.0 unx     3876 b- defN 22-Jan-14 16:14 bambu/train/__init__.py
--rw-r--r--  2.0 unx     3594 b- defN 22-Jan-14 19:21 bambu_qsar-0.0.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Jan-14 19:21 bambu_qsar-0.0.8.dist-info/WHEEL
--rw-r--r--  2.0 unx      163 b- defN 22-Jan-14 19:21 bambu_qsar-0.0.8.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        6 b- defN 22-Jan-14 19:21 bambu_qsar-0.0.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1327 b- defN 22-Jan-14 19:21 bambu_qsar-0.0.8.dist-info/RECORD
-16 files, 22250 bytes uncompressed, 8326 bytes compressed:  62.6%
+-rw-r--r--  2.0 unx     8042 b- defN 22-Jan-19 17:28 bambu_qsar-0.0.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 22-Jan-19 17:28 bambu_qsar-0.0.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx      163 b- defN 22-Jan-19 17:28 bambu_qsar-0.0.9.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        6 b- defN 22-Jan-19 17:28 bambu_qsar-0.0.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1413 b- defN 22-Jan-19 17:28 bambu_qsar-0.0.9.dist-info/RECORD
+17 files, 31616 bytes uncompressed, 10825 bytes compressed:  65.8%
```

## zipnote {}

```diff
@@ -6,14 +6,17 @@
 
 Filename: bambu/download/__init__.py
 Comment: 
 
 Filename: bambu/models/__init__.py
 Comment: 
 
+Filename: bambu/models/decision_tree.py
+Comment: 
+
 Filename: bambu/predict/__init__.py
 Comment: 
 
 Filename: bambu/predict/run.py
 Comment: 
 
 Filename: bambu/preprocess/__init__.py
@@ -27,23 +30,23 @@
 
 Filename: bambu/preprocess/preprocessors/morgan.py
 Comment: 
 
 Filename: bambu/train/__init__.py
 Comment: 
 
-Filename: bambu_qsar-0.0.8.dist-info/METADATA
+Filename: bambu_qsar-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: bambu_qsar-0.0.8.dist-info/WHEEL
+Filename: bambu_qsar-0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: bambu_qsar-0.0.8.dist-info/entry_points.txt
+Filename: bambu_qsar-0.0.9.dist-info/entry_points.txt
 Comment: 
 
-Filename: bambu_qsar-0.0.8.dist-info/top_level.txt
+Filename: bambu_qsar-0.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: bambu_qsar-0.0.8.dist-info/RECORD
+Filename: bambu_qsar-0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## bambu/preprocess/__init__.py

```diff
@@ -97,18 +97,28 @@
         test_filepath  = f'{filepath}_test{fileext}'
 
         X = df_output.drop(['activity'], axis=1)
         y = df_output['activity']
 
         X_train, X_test, y_train, y_test = train_test_split(X, y, train_size=train_test_split_percent)
 
+        X_train = X_train.astype(np.float32)
+        X_test  = X_test.astype(np.float32)
+
         df_output_train = pd.DataFrame(X_train)
         df_output_train['activity'] = y_train
+        df_output_train = clean_dataset(df_output_train)
         df_output_train.to_csv(train_filepath, index=False)
 
         df_output_test = pd.DataFrame(X_test)
         df_output_test['activity'] = y_test
+        df_output_test = clean_dataset(df_output_test)
         df_output_test.to_csv(test_filepath, index=False)
 
+def clean_dataset(df):
+    df = df.astype(np.float32)
+    df.dropna(inplace=True)
+    indices_to_keep = ~df.isin([np.nan, np.inf, -np.inf]).any(1)
+    return df[indices_to_keep].astype(np.float32)
 
 if __name__ == "__main__":
     main()
```

## Comparing `bambu_qsar-0.0.8.dist-info/RECORD` & `bambu_qsar-0.0.9.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 bambu/__init__.py,sha256=0Z7dqanmYBbhvCdjzR28g0mOlbxSv9ePnkKAYCAyZCQ,89
 bambu/logo.py,sha256=1-FlybwcDmV8z-VuI7ZhV6_xJKAlTsKWVdo063EXVSg,187
 bambu/download/__init__.py,sha256=bmKm8t9R_yOAsl1tyaAZkvc0-1NXzaZi_Y4u3mzpKks,3904
 bambu/models/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+bambu/models/decision_tree.py,sha256=yO9HfDFGRaz-inTQxC25tIhkmUnB4e4n-6NbnfNzvqs,4433
 bambu/predict/__init__.py,sha256=deSm8UDIhuUCAtckfiZxhQ79N4RbIE9zvnAqeM4uEHA,2437
 bambu/predict/run.py,sha256=FK9G3-BL2m5KIaxlhBo9k2LFZdvDmSIDMirLkR2mAIc,837
-bambu/preprocess/__init__.py,sha256=yzVWSQfR-JaPVZVlNZ3--jd_yIEwcmHWMTeXrHXrJ-Q,4765
+bambu/preprocess/__init__.py,sha256=edRvdvAbMUgE6oaAIggXaggGeOWkZkzLOWlkSV81cZY,5164
 bambu/preprocess/preprocessors/__init__.py,sha256=ECfP5scTbcVSVCW3xj8NqAqFGvN3tG1RW2xwkOkYKRk,46
 bambu/preprocess/preprocessors/descriptors.py,sha256=V_DlXPJd0e4-820T29_6JKTbvsP9M-8ZF9EtkUFUTgk,389
 bambu/preprocess/preprocessors/morgan.py,sha256=FB3SZ2fm4BZ5NcH_nTii_thVVf24ANsUheP0yfBr4Ws,538
 bambu/train/__init__.py,sha256=MWMsf3TjyPaFhtcadyPNl7RlLijOe2fTwkdM7Ob8kyI,3876
-bambu_qsar-0.0.8.dist-info/METADATA,sha256=n5LU7FPsFfNVxyPsHiVpI26mGwkgqFdkFzgkNJ6tLD8,3594
-bambu_qsar-0.0.8.dist-info/WHEEL,sha256=EVRjI69F5qVjm_YgqcTXPnTAv3BfSUr0WVAHuSP3Xoo,92
-bambu_qsar-0.0.8.dist-info/entry_points.txt,sha256=MzFgvmjcuiSP6XQBHZWGf-RGjrO4_G1CAWrnxDL8qm4,163
-bambu_qsar-0.0.8.dist-info/top_level.txt,sha256=_5HMWp_Og5eXEnHSTOdZSXOV5wGC70y_D2vD-A1mQdk,6
-bambu_qsar-0.0.8.dist-info/RECORD,,
+bambu_qsar-0.0.9.dist-info/METADATA,sha256=TL8D7EMBZVWYHPvID8pqm39CAFnSIq6TZZeP_LXt6Jo,8042
+bambu_qsar-0.0.9.dist-info/WHEEL,sha256=EVRjI69F5qVjm_YgqcTXPnTAv3BfSUr0WVAHuSP3Xoo,92
+bambu_qsar-0.0.9.dist-info/entry_points.txt,sha256=MzFgvmjcuiSP6XQBHZWGf-RGjrO4_G1CAWrnxDL8qm4,163
+bambu_qsar-0.0.9.dist-info/top_level.txt,sha256=_5HMWp_Og5eXEnHSTOdZSXOV5wGC70y_D2vD-A1mQdk,6
+bambu_qsar-0.0.9.dist-info/RECORD,,
```

