# Comparing `tmp/HomoglyphsCJK-0.0.9.tar.gz` & `tmp/HomoglyphsCJK-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HomoglyphsCJK-0.0.9.tar", last modified: Mon May 22 15:03:32 2023, max compression
+gzip compressed data, was "HomoglyphsCJK-0.1.0.tar", last modified: Thu May 25 02:47:12 2023, max compression
```

## Comparing `HomoglyphsCJK-0.0.9.tar` & `HomoglyphsCJK-0.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 yangxinmei   (501) staff       (20)        0 2023-05-22 15:03:32.219113 HomoglyphsCJK-0.0.9/
-drwxr-xr-x   0 yangxinmei   (501) staff       (20)        0 2023-05-22 15:03:32.217255 HomoglyphsCJK-0.0.9/HomoglyphsCJK/
--rw-r--r--   0 yangxinmei   (501) staff       (20)       93 2023-05-22 03:32:58.000000 HomoglyphsCJK-0.0.9/HomoglyphsCJK/__init__.py
--rw-r--r--   0 yangxinmei   (501) staff       (20)     8873 2023-05-22 02:32:32.000000 HomoglyphsCJK-0.0.9/HomoglyphsCJK/hg_functions.py
--rw-r--r--   0 yangxinmei   (501) staff       (20)     2422 2023-05-13 13:49:58.000000 HomoglyphsCJK-0.0.9/HomoglyphsCJK/test_run.py
-drwxr-xr-x   0 yangxinmei   (501) staff       (20)        0 2023-05-22 15:03:32.218598 HomoglyphsCJK-0.0.9/HomoglyphsCJK.egg-info/
--rw-r--r--   0 yangxinmei   (501) staff       (20)     3357 2023-05-22 15:03:32.000000 HomoglyphsCJK-0.0.9/HomoglyphsCJK.egg-info/PKG-INFO
--rw-r--r--   0 yangxinmei   (501) staff       (20)      284 2023-05-22 15:03:32.000000 HomoglyphsCJK-0.0.9/HomoglyphsCJK.egg-info/SOURCES.txt
--rw-r--r--   0 yangxinmei   (501) staff       (20)        1 2023-05-22 15:03:32.000000 HomoglyphsCJK-0.0.9/HomoglyphsCJK.egg-info/dependency_links.txt
--rw-r--r--   0 yangxinmei   (501) staff       (20)       44 2023-05-22 15:03:32.000000 HomoglyphsCJK-0.0.9/HomoglyphsCJK.egg-info/requires.txt
--rw-r--r--   0 yangxinmei   (501) staff       (20)       14 2023-05-22 15:03:32.000000 HomoglyphsCJK-0.0.9/HomoglyphsCJK.egg-info/top_level.txt
--rw-r--r--   0 yangxinmei   (501) staff       (20)     3357 2023-05-22 15:03:32.218915 HomoglyphsCJK-0.0.9/PKG-INFO
--rw-r--r--   0 yangxinmei   (501) staff       (20)     2813 2023-05-22 15:03:01.000000 HomoglyphsCJK-0.0.9/README.md
--rw-r--r--   0 yangxinmei   (501) staff       (20)       38 2023-05-22 15:03:32.219177 HomoglyphsCJK-0.0.9/setup.cfg
--rw-r--r--   0 yangxinmei   (501) staff       (20)      950 2023-05-22 15:03:25.000000 HomoglyphsCJK-0.0.9/setup.py
+drwxr-xr-x   0 yangxinmei   (501) staff       (20)        0 2023-05-25 02:47:12.856681 HomoglyphsCJK-0.1.0/
+drwxr-xr-x   0 yangxinmei   (501) staff       (20)        0 2023-05-25 02:47:12.851896 HomoglyphsCJK-0.1.0/HomoglyphsCJK/
+-rw-r--r--   0 yangxinmei   (501) staff       (20)       93 2023-05-22 03:32:58.000000 HomoglyphsCJK-0.1.0/HomoglyphsCJK/__init__.py
+-rw-r--r--   0 yangxinmei   (501) staff       (20)     9586 2023-05-25 02:44:44.000000 HomoglyphsCJK-0.1.0/HomoglyphsCJK/hg_functions.py
+-rw-r--r--   0 yangxinmei   (501) staff       (20)     2422 2023-05-13 13:49:58.000000 HomoglyphsCJK-0.1.0/HomoglyphsCJK/test_run.py
+drwxr-xr-x   0 yangxinmei   (501) staff       (20)        0 2023-05-25 02:47:12.856082 HomoglyphsCJK-0.1.0/HomoglyphsCJK.egg-info/
+-rw-r--r--   0 yangxinmei   (501) staff       (20)     3752 2023-05-25 02:47:12.000000 HomoglyphsCJK-0.1.0/HomoglyphsCJK.egg-info/PKG-INFO
+-rw-r--r--   0 yangxinmei   (501) staff       (20)      284 2023-05-25 02:47:12.000000 HomoglyphsCJK-0.1.0/HomoglyphsCJK.egg-info/SOURCES.txt
+-rw-r--r--   0 yangxinmei   (501) staff       (20)        1 2023-05-25 02:47:12.000000 HomoglyphsCJK-0.1.0/HomoglyphsCJK.egg-info/dependency_links.txt
+-rw-r--r--   0 yangxinmei   (501) staff       (20)       44 2023-05-25 02:47:12.000000 HomoglyphsCJK-0.1.0/HomoglyphsCJK.egg-info/requires.txt
+-rw-r--r--   0 yangxinmei   (501) staff       (20)       14 2023-05-25 02:47:12.000000 HomoglyphsCJK-0.1.0/HomoglyphsCJK.egg-info/top_level.txt
+-rw-r--r--   0 yangxinmei   (501) staff       (20)     3752 2023-05-25 02:47:12.856453 HomoglyphsCJK-0.1.0/PKG-INFO
+-rw-r--r--   0 yangxinmei   (501) staff       (20)     3208 2023-05-25 02:46:46.000000 HomoglyphsCJK-0.1.0/README.md
+-rw-r--r--   0 yangxinmei   (501) staff       (20)       38 2023-05-25 02:47:12.856730 HomoglyphsCJK-0.1.0/setup.cfg
+-rw-r--r--   0 yangxinmei   (501) staff       (20)      950 2023-05-25 02:44:47.000000 HomoglyphsCJK-0.1.0/setup.py
```

### Comparing `HomoglyphsCJK-0.0.9/HomoglyphsCJK/hg_functions.py` & `HomoglyphsCJK-0.1.0/HomoglyphsCJK/hg_functions.py`

 * *Files 12% similar despite different names*

```diff
@@ -114,26 +114,33 @@
             return 1
     return 0
 
 def homoglyph_merge(lang, df_1,df_2,key_1,key_2,homo_lambda=1, insertion=1, deletion=1, parallel=False,num_workers=None):
     #cluster_dict = download_dict('ko')
     # Initialize the list 2
     list2 = df_2[key_2].tolist()
+    # key_2 to other variables
+    df_2_columns = df_2.columns.values.tolist()
+    df_2.set_index(key_2,inplace=True)
+    for df_2_col in df_2_columns:
+        if df_2_col!=key_2:
+            globals()['col%s' % df_2_col] = df_2.to_dict()[df_2_col]
+
     # Initialize the list 1
     result_list = df_1[key_1].tolist() # The result_list is list 1
-    assert len(list2) == len(result_list)
+    # assert len(list2) == len(result_list)
     list1 = [] # initialize the list1
     for res, truth in zip(result_list,list2):
         res_dict = {}
         res_dict[key_1] = res
         res_dict[key_2] = truth
         list1.append(res_dict)
     # Save output and initialize the accuracy results storage
     ## add the df_matched
-    df_matched = pd.DataFrame(list(zip(list2,result_list)), columns=[key_2,key_1])
+    # df_matched = pd.DataFrame(list(zip(list2,result_list)), columns=[key_2,key_1])
 
     global cluster_dict
     download_dict(lang)
 
     if parallel==False:
         word_dist_min_list = map(partial(list_fd,list2=list2,homo_lambda=homo_lambda, insertion=insertion, deletion=deletion),result_list)#added the functions
     else:
@@ -148,19 +155,29 @@
     distance_list = []
     for id, (list1_ele, word_dist_min) in enumerate(zip(list1,word_dist_min_list)):
         list1[id]["matched_word"] = word_dist_min[1]
         matched_list.append(word_dist_min[1])
         list1[id]["matched_word_dist"] = round(word_dist_min[0],2)
         distance_list.append(round(word_dist_min[0],2))
 
-    df_matched = pd.DataFrame(list(zip(result_list, \
-        matched_list, distance_list, \
-            )),columns=[key_1, \
-                f'homo_matched_{key_2}','homo_dist', \
-                                        ])
+    for df_2_col in df_2_columns:
+        if df_2_col!=key_2:
+            globals()['col%s_list' % df_2_col] = []
+            for matched in matched_list:
+                globals()['col%s_list' % df_2_col].append(globals()['col%s' % df_2_col][matched])
+
+    aux_df = pd.DataFrame(list(matched_list),columns=[f'homo_matched_{key_2}'])# The matched_list is already on
+    for df_2_col in df_2_columns:
+        if df_2_col!=key_2:
+            aux_df = pd.concat([aux_df, pd.DataFrame(globals()['col%s_list' % df_2_col],columns=[df_2_col])],axis=1)
+    
+
+    df_matched = pd.concat([df_1, pd.DataFrame(list(distance_list),columns=['homo_dist']),
+            aux_df],axis=1
+            )
     return df_matched
     
 # @njit
 # def wagner_fischer_with_cluster_dict_fast(str1, str2, cluster_dict_keys, cluster_dict_values):
 #     m = len(str1)
 #     n = len(str2)
 #     ###If the strings are the same, return zero
```

### Comparing `HomoglyphsCJK-0.0.9/HomoglyphsCJK/test_run.py` & `HomoglyphsCJK-0.1.0/HomoglyphsCJK/test_run.py`

 * *Files identical despite different names*

### Comparing `HomoglyphsCJK-0.0.9/HomoglyphsCJK.egg-info/PKG-INFO` & `HomoglyphsCJK-0.1.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,76 +1,65 @@
-Metadata-Version: 2.1
-Name: HomoglyphsCJK
-Version: 0.0.9
-Summary: An easy Python package for fuzzy matching Chinese(simplified and traditional), Japanese and Korean, using character similarity trained from ViT transformer
-Home-page: https://github.com/dell-research-harvard/HomoglyphsCJK.git
-Author: HomoglyphsCJK Team
-Author-email: homoglyphscjk@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-
 HomoglyphsCJK
 =====
 
 An efficient and useful tool to fuzzy match Japanese, Korean, Simplified Chinese or Traditional Chinese words.
 
 ## Installation
 ```
 pip install HomoglyphsCJK
 ```
 
 ## Usage
 There are two functionalities of this package: calculate homoglyph distance between two strings, or merge two dataframes based on keys using homoglyph distance.
-
-When you firstly use this on one language, the homoglyph dict will be downloaded automatically in the current directory you run your script. So please make sure you run the script from a folder that has permission to write.
-
-+ Merge two dataframes. When you merge two dataframes, you can specify the parallel argument to run multiprocessing. Mac users probably want to use Python version == 3.7 for multiprocessing.
++ If you use homoglyph_merge on specific language, the dict will be downloaded automatically. If you want to calculate pair wise homoglyphic edit distance, before using homoglyph_distance(str1, str2), you need to download_dict(lang) to either download or load the homoglyphs dict.
++ When you firstly use this on one language, the homoglyph dict will be downloaded automatically in the current directory you run your script. So please make sure you run the script from a folder that has permission to write. The available languages are [zhs, zht, ko, ja] for simplified Chinese, traditional Chinese, Korean and Japanese respectively.
++ Merge two dataframes. When you merge two dataframes, you can specify the parallel argument to run multiprocessing. If you don't specify the num_workers when using parallel, it will automatically use the number of all detected CPU cores
 
 ```python
-    from HomoglyphsCJK import homoglyph_distance,homoglyph_merge,download_dict
-    import pandas as pd
-    df_1 = pd.DataFrame(list(['苏萃乡','办雄','虐格给','雪拉普岗']),columns=['ocred_text'])
-    df_2 = pd.DataFrame(list(['雪拉普岗日','小苏莽乡','协雄','唐格给']),columns=['truth_text'])
-
-    # merge two dataframes, note that the homoglyph dict of specified language will be downloaded automatically when first run.
-    ## run in parallel with pool of 4, if num_workers is not specified, all available CPU cores are used.
-    dataframe_merged = homoglyph_merge('zhs',df_1,df_2,'ocred_text','truth_text',homo_lambda=1, insertion=1, deletion=1,parallel=True,num_workers=4)
-    
-    ## not run in parallel
-    dataframe_merged = homoglyph_merge('zhs',df_1,df_2,'ocred_text','truth_text',homo_lambda=1, insertion=1, deletion=1) 
-    '''
-    lang: choose from zhs, zht, ja, ko
-    dataframe 1: the first dataframe
-    dataframe 2: the second dataframe
-    key from dataframe 1
-    key from dataframe 2
-    weight on substitution homoglyph distance, default is 1
-    weight on insertion cost, default is 1
-    weight on deletion cost, default is 1
-    '''
+from HomoglyphsCJK import homoglyph_distance,homoglyph_merge,download_dict
+import pandas as pd
+df_1 = pd.DataFrame(list(['苏萃乡','办雄','虐格给','雪拉普岗']),columns=['query'])
+df_2 = pd.DataFrame(list(['雪拉普岗日','小苏莽乡','协雄','唐格给','太阳村','月亮湾']),columns=['key'])
+
+# merge two dataframes, note that the homoglyph dict of specified language will be downloaded automatically when first run.
+## run in parallel with pool of 4, if num_workers is not specified, all available CPU cores are used.
+dataframe_merged = homoglyph_merge('zhs',df_1,df_2,'query','key',homo_lambda=1, insertion=1, deletion=1,parallel=True,num_workers=4)
+
+## not run in parallel
+dataframe_merged = homoglyph_merge('zhs',df_1,df_2,'query','key',homo_lambda=1, insertion=1, deletion=1) 
+'''
+lang: choose from zhs, zht, ja, ko
+dataframe 1: the first dataframe
+dataframe 2: the second dataframe
+key from dataframe 1
+key from dataframe 2
+weight on substitution homoglyph distance, default is 1
+weight on insertion cost, default is 1
+weight on deletion cost, default is 1
+'''
 ```
 
 | ocred_text | homo_matched_truth_text | homo_dist |
 | ---------- | ----------------------- | --------- |
 | 苏萃乡      | 小苏莽乡                 | 1.88      | 
 | 办雄        | 协雄                    | 0.15      |
 | 虐格给      | 唐格给                   | 0.87      |
 | 雪拉普岗    | 雪拉普岗日                | 1.0       | 
 
 + Homoglyph distance between two strings. The default weight on substitution, insertion, deletion is 1.
-+ download_dict and homoglyph_merge will trigger downloading homoglyph dicts to your current directory if it does not already exist, otherwise it just load the existing dict from your local computer.
++ download_dict will trigger downloading homoglyph dicts to your current directory if it does not already exist, otherwise it just load the existing dict from your local computer.
 
 ```python
     
-    download_dict('zhs')
-    homoglyph_distance('苏萃乡','小苏莽乡',homo_lambda=1, insertion=1, deletion=1)
-    # 1.88
+download_dict('zhs')
+homoglyph_distance('苏萃乡','小苏莽乡',homo_lambda=1, insertion=1, deletion=1)
+# 1.88
 ```
+## Contributing
+We encourage you to contribute to HomoglyphsCJK!
 
 ## Citation
 
 Coming Soon
 ```bibtex
 
 ```
```

### Comparing `HomoglyphsCJK-0.0.9/PKG-INFO` & `HomoglyphsCJK-0.1.0/HomoglyphsCJK.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HomoglyphsCJK
-Version: 0.0.9
+Version: 0.1.0
 Summary: An easy Python package for fuzzy matching Chinese(simplified and traditional), Japanese and Korean, using character similarity trained from ViT transformer
 Home-page: https://github.com/dell-research-harvard/HomoglyphsCJK.git
 Author: HomoglyphsCJK Team
 Author-email: homoglyphscjk@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -18,59 +18,60 @@
 ## Installation
 ```
 pip install HomoglyphsCJK
 ```
 
 ## Usage
 There are two functionalities of this package: calculate homoglyph distance between two strings, or merge two dataframes based on keys using homoglyph distance.
-
-When you firstly use this on one language, the homoglyph dict will be downloaded automatically in the current directory you run your script. So please make sure you run the script from a folder that has permission to write.
-
-+ Merge two dataframes. When you merge two dataframes, you can specify the parallel argument to run multiprocessing. Mac users probably want to use Python version == 3.7 for multiprocessing.
++ If you use homoglyph_merge on specific language, the dict will be downloaded automatically. If you want to calculate pair wise homoglyphic edit distance, before using homoglyph_distance(str1, str2), you need to download_dict(lang) to either download or load the homoglyphs dict.
++ When you firstly use this on one language, the homoglyph dict will be downloaded automatically in the current directory you run your script. So please make sure you run the script from a folder that has permission to write. The available languages are [zhs, zht, ko, ja] for simplified Chinese, traditional Chinese, Korean and Japanese respectively.
++ Merge two dataframes. When you merge two dataframes, you can specify the parallel argument to run multiprocessing. If you don't specify the num_workers when using parallel, it will automatically use the number of all detected CPU cores
 
 ```python
-    from HomoglyphsCJK import homoglyph_distance,homoglyph_merge,download_dict
-    import pandas as pd
-    df_1 = pd.DataFrame(list(['苏萃乡','办雄','虐格给','雪拉普岗']),columns=['ocred_text'])
-    df_2 = pd.DataFrame(list(['雪拉普岗日','小苏莽乡','协雄','唐格给']),columns=['truth_text'])
-
-    # merge two dataframes, note that the homoglyph dict of specified language will be downloaded automatically when first run.
-    ## run in parallel with pool of 4, if num_workers is not specified, all available CPU cores are used.
-    dataframe_merged = homoglyph_merge('zhs',df_1,df_2,'ocred_text','truth_text',homo_lambda=1, insertion=1, deletion=1,parallel=True,num_workers=4)
-    
-    ## not run in parallel
-    dataframe_merged = homoglyph_merge('zhs',df_1,df_2,'ocred_text','truth_text',homo_lambda=1, insertion=1, deletion=1) 
-    '''
-    lang: choose from zhs, zht, ja, ko
-    dataframe 1: the first dataframe
-    dataframe 2: the second dataframe
-    key from dataframe 1
-    key from dataframe 2
-    weight on substitution homoglyph distance, default is 1
-    weight on insertion cost, default is 1
-    weight on deletion cost, default is 1
-    '''
+from HomoglyphsCJK import homoglyph_distance,homoglyph_merge,download_dict
+import pandas as pd
+df_1 = pd.DataFrame(list(['苏萃乡','办雄','虐格给','雪拉普岗']),columns=['query'])
+df_2 = pd.DataFrame(list(['雪拉普岗日','小苏莽乡','协雄','唐格给','太阳村','月亮湾']),columns=['key'])
+
+# merge two dataframes, note that the homoglyph dict of specified language will be downloaded automatically when first run.
+## run in parallel with pool of 4, if num_workers is not specified, all available CPU cores are used.
+dataframe_merged = homoglyph_merge('zhs',df_1,df_2,'query','key',homo_lambda=1, insertion=1, deletion=1,parallel=True,num_workers=4)
+
+## not run in parallel
+dataframe_merged = homoglyph_merge('zhs',df_1,df_2,'query','key',homo_lambda=1, insertion=1, deletion=1) 
+'''
+lang: choose from zhs, zht, ja, ko
+dataframe 1: the first dataframe
+dataframe 2: the second dataframe
+key from dataframe 1
+key from dataframe 2
+weight on substitution homoglyph distance, default is 1
+weight on insertion cost, default is 1
+weight on deletion cost, default is 1
+'''
 ```
 
 | ocred_text | homo_matched_truth_text | homo_dist |
 | ---------- | ----------------------- | --------- |
 | 苏萃乡      | 小苏莽乡                 | 1.88      | 
 | 办雄        | 协雄                    | 0.15      |
 | 虐格给      | 唐格给                   | 0.87      |
 | 雪拉普岗    | 雪拉普岗日                | 1.0       | 
 
 + Homoglyph distance between two strings. The default weight on substitution, insertion, deletion is 1.
-+ download_dict and homoglyph_merge will trigger downloading homoglyph dicts to your current directory if it does not already exist, otherwise it just load the existing dict from your local computer.
++ download_dict will trigger downloading homoglyph dicts to your current directory if it does not already exist, otherwise it just load the existing dict from your local computer.
 
 ```python
     
-    download_dict('zhs')
-    homoglyph_distance('苏萃乡','小苏莽乡',homo_lambda=1, insertion=1, deletion=1)
-    # 1.88
+download_dict('zhs')
+homoglyph_distance('苏萃乡','小苏莽乡',homo_lambda=1, insertion=1, deletion=1)
+# 1.88
 ```
+## Contributing
+We encourage you to contribute to HomoglyphsCJK!
 
 ## Citation
 
 Coming Soon
 ```bibtex
 
 ```
```

### Comparing `HomoglyphsCJK-0.0.9/setup.py` & `HomoglyphsCJK-0.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open("README.md","r") as fh:
     long_des = fh.read()
 
 setup(
     name="HomoglyphsCJK",
     packages=["HomoglyphsCJK"],
-    version="0.0.9",
+    version="0.1.0",
     author="HomoglyphsCJK Team",
     author_email="homoglyphscjk@gmail.com",
     description="An easy Python package for fuzzy matching Chinese(simplified and traditional), Japanese and Korean, using character similarity trained from ViT transformer",
     long_description=long_des,
     long_description_content_type="text/markdown",
     url="https://github.com/dell-research-harvard/HomoglyphsCJK.git",
     classifiers=[
```

