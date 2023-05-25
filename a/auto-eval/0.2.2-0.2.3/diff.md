# Comparing `tmp/auto-eval-0.2.2.tar.gz` & `tmp/auto-eval-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto-eval-0.2.2.tar", last modified: Mon May 22 09:20:07 2023, max compression
+gzip compressed data, was "auto-eval-0.2.3.tar", last modified: Thu May 25 03:19:16 2023, max compression
```

## Comparing `auto-eval-0.2.2.tar` & `auto-eval-0.2.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-22 09:20:07.287827 auto-eval-0.2.2/
--rw-r--r--   0 zhangchong   (501) staff       (20)     1071 2023-04-28 07:53:45.000000 auto-eval-0.2.2/LICENSE
--rw-r--r--   0 zhangchong   (501) staff       (20)    14210 2023-05-22 09:20:07.287564 auto-eval-0.2.2/PKG-INFO
--rw-r--r--   0 zhangchong   (501) staff       (20)    13784 2023-05-22 08:54:26.000000 auto-eval-0.2.2/README.md
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-22 09:20:07.284974 auto-eval-0.2.2/auto_eval.egg-info/
--rw-r--r--   0 zhangchong   (501) staff       (20)    14210 2023-05-22 09:20:07.000000 auto-eval-0.2.2/auto_eval.egg-info/PKG-INFO
--rw-r--r--   0 zhangchong   (501) staff       (20)      465 2023-05-22 09:20:07.000000 auto-eval-0.2.2/auto_eval.egg-info/SOURCES.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)        1 2023-05-22 09:20:07.000000 auto-eval-0.2.2/auto_eval.egg-info/dependency_links.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)       59 2023-05-22 09:20:07.000000 auto-eval-0.2.2/auto_eval.egg-info/entry_points.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)       49 2023-05-22 09:20:07.000000 auto-eval-0.2.2/auto_eval.egg-info/requires.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)        5 2023-05-22 09:20:07.000000 auto-eval-0.2.2/auto_eval.egg-info/top_level.txt
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-22 09:20:07.285426 auto-eval-0.2.2/eval/
--rw-r--r--   0 zhangchong   (501) staff       (20)      136 2023-05-08 07:54:51.000000 auto-eval-0.2.2/eval/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     8295 2023-05-22 09:15:23.000000 auto-eval-0.2.2/eval/auto_llms_eval.py
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-22 09:20:07.285852 auto-eval-0.2.2/eval/commands/
--rw-r--r--   0 zhangchong   (501) staff       (20)        0 2023-04-28 08:32:15.000000 auto-eval-0.2.2/eval/commands/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     5552 2023-05-19 08:57:24.000000 auto-eval-0.2.2/eval/commands/auto_eval.py
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-22 09:20:07.286709 auto-eval-0.2.2/eval/prompt_template/
--rw-r--r--   0 zhangchong   (501) staff       (20)      198 2023-05-19 08:23:31.000000 auto-eval-0.2.2/eval/prompt_template/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     3090 2023-05-19 09:15:03.000000 auto-eval-0.2.2/eval/prompt_template/prompter.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     2134 2023-05-22 07:59:55.000000 auto-eval-0.2.2/eval/prompt_template/prompts.py
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-22 09:20:07.287160 auto-eval-0.2.2/eval/utils/
--rw-r--r--   0 zhangchong   (501) staff       (20)       26 2023-04-28 09:40:19.000000 auto-eval-0.2.2/eval/utils/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     3422 2023-05-18 04:08:41.000000 auto-eval-0.2.2/eval/utils/data_utils.py
--rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-05-22 09:20:07.287877 auto-eval-0.2.2/setup.cfg
--rw-r--r--   0 zhangchong   (501) staff       (20)      956 2023-05-22 09:17:45.000000 auto-eval-0.2.2/setup.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-25 03:19:16.599714 auto-eval-0.2.3/
+-rw-r--r--   0 zhangchong   (501) staff       (20)     1071 2023-04-28 07:53:45.000000 auto-eval-0.2.3/LICENSE
+-rw-r--r--   0 zhangchong   (501) staff       (20)    14212 2023-05-25 03:19:16.599534 auto-eval-0.2.3/PKG-INFO
+-rw-r--r--   0 zhangchong   (501) staff       (20)    13786 2023-05-25 03:15:57.000000 auto-eval-0.2.3/README.md
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-25 03:19:16.596681 auto-eval-0.2.3/auto_eval.egg-info/
+-rw-r--r--   0 zhangchong   (501) staff       (20)    14212 2023-05-25 03:19:16.000000 auto-eval-0.2.3/auto_eval.egg-info/PKG-INFO
+-rw-r--r--   0 zhangchong   (501) staff       (20)      465 2023-05-25 03:19:16.000000 auto-eval-0.2.3/auto_eval.egg-info/SOURCES.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)        1 2023-05-25 03:19:16.000000 auto-eval-0.2.3/auto_eval.egg-info/dependency_links.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)       59 2023-05-25 03:19:16.000000 auto-eval-0.2.3/auto_eval.egg-info/entry_points.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)       49 2023-05-25 03:19:16.000000 auto-eval-0.2.3/auto_eval.egg-info/requires.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)        5 2023-05-25 03:19:16.000000 auto-eval-0.2.3/auto_eval.egg-info/top_level.txt
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-25 03:19:16.597230 auto-eval-0.2.3/eval/
+-rw-r--r--   0 zhangchong   (501) staff       (20)      136 2023-05-08 07:54:51.000000 auto-eval-0.2.3/eval/__init__.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     8295 2023-05-22 09:15:23.000000 auto-eval-0.2.3/eval/auto_llms_eval.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-25 03:19:16.597704 auto-eval-0.2.3/eval/commands/
+-rw-r--r--   0 zhangchong   (501) staff       (20)        0 2023-04-28 08:32:15.000000 auto-eval-0.2.3/eval/commands/__init__.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     5552 2023-05-19 08:57:24.000000 auto-eval-0.2.3/eval/commands/auto_eval.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-25 03:19:16.598615 auto-eval-0.2.3/eval/prompt_template/
+-rw-r--r--   0 zhangchong   (501) staff       (20)      198 2023-05-19 08:23:31.000000 auto-eval-0.2.3/eval/prompt_template/__init__.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     3090 2023-05-19 09:15:03.000000 auto-eval-0.2.3/eval/prompt_template/prompter.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     2134 2023-05-22 07:59:55.000000 auto-eval-0.2.3/eval/prompt_template/prompts.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-25 03:19:16.599192 auto-eval-0.2.3/eval/utils/
+-rw-r--r--   0 zhangchong   (501) staff       (20)       26 2023-04-28 09:40:19.000000 auto-eval-0.2.3/eval/utils/__init__.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     3522 2023-05-25 03:17:37.000000 auto-eval-0.2.3/eval/utils/data_utils.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-05-25 03:19:16.599762 auto-eval-0.2.3/setup.cfg
+-rw-r--r--   0 zhangchong   (501) staff       (20)      956 2023-05-25 03:18:21.000000 auto-eval-0.2.3/setup.py
```

### Comparing `auto-eval-0.2.2/LICENSE` & `auto-eval-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `auto-eval-0.2.2/PKG-INFO` & `auto-eval-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-eval
-Version: 0.2.2
+Version: 0.2.3
 Summary: Using only one line of commmands to evaluate multiple models
 Home-page: https://github.com/muximus3/Auto-Eval
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -245,14 +245,14 @@
 
 `--sample_num`: number ${\color{grey}\text{Optional}}$ Defaults to 0<br>Sample number of prompt-answer pairs to evaluate.
 
 `--interval`: number ${\color{grey}\text{Optional}}$ Defaults to 1 <br> Sleep interval in seconds between each request to avoid exceeding the request rate limit. A larger value like 10 is recommended for GPT-4.
 
 `--retry`:  ${\color{grey}\text{Optional}}$ Defaults to True <br> Whether to retry once for all failed requests. Failed requests may be due to reasons such as exceeding API request frequency, incorrect answer format parsing, or network failure.
 
-`score_by`: array ${\color{grey}\text{Optional}}$ Defaults to null <br> Used to determine the groups for the groupby `pandas.groupby(by=args.score_by)` to get the summary scores of certain groups.
+`--score_by`: array ${\color{grey}\text{Optional}}$ Defaults to null <br> Used to determine the groups for the groupby `pandas.groupby(by=args.score_by)` to get the summary scores of certain groups.
 
 
 ## ToDo
 - [ ] Conbining multiple GPT-like models for prediction: routing or simply averaging.
 - [ ] Supporting prompts evaluation by output the accuracy of different prompts. 
 - [ ] Configuring a default test set for prompt evaluation.
```

### Comparing `auto-eval-0.2.2/README.md` & `auto-eval-0.2.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -233,14 +233,14 @@
 
 `--sample_num`: number ${\color{grey}\text{Optional}}$ Defaults to 0<br>Sample number of prompt-answer pairs to evaluate.
 
 `--interval`: number ${\color{grey}\text{Optional}}$ Defaults to 1 <br> Sleep interval in seconds between each request to avoid exceeding the request rate limit. A larger value like 10 is recommended for GPT-4.
 
 `--retry`:  ${\color{grey}\text{Optional}}$ Defaults to True <br> Whether to retry once for all failed requests. Failed requests may be due to reasons such as exceeding API request frequency, incorrect answer format parsing, or network failure.
 
-`score_by`: array ${\color{grey}\text{Optional}}$ Defaults to null <br> Used to determine the groups for the groupby `pandas.groupby(by=args.score_by)` to get the summary scores of certain groups.
+`--score_by`: array ${\color{grey}\text{Optional}}$ Defaults to null <br> Used to determine the groups for the groupby `pandas.groupby(by=args.score_by)` to get the summary scores of certain groups.
 
 
 ## ToDo
 - [ ] Conbining multiple GPT-like models for prediction: routing or simply averaging.
 - [ ] Supporting prompts evaluation by output the accuracy of different prompts. 
 - [ ] Configuring a default test set for prompt evaluation.
```

### Comparing `auto-eval-0.2.2/auto_eval.egg-info/PKG-INFO` & `auto-eval-0.2.3/auto_eval.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-eval
-Version: 0.2.2
+Version: 0.2.3
 Summary: Using only one line of commmands to evaluate multiple models
 Home-page: https://github.com/muximus3/Auto-Eval
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -245,14 +245,14 @@
 
 `--sample_num`: number ${\color{grey}\text{Optional}}$ Defaults to 0<br>Sample number of prompt-answer pairs to evaluate.
 
 `--interval`: number ${\color{grey}\text{Optional}}$ Defaults to 1 <br> Sleep interval in seconds between each request to avoid exceeding the request rate limit. A larger value like 10 is recommended for GPT-4.
 
 `--retry`:  ${\color{grey}\text{Optional}}$ Defaults to True <br> Whether to retry once for all failed requests. Failed requests may be due to reasons such as exceeding API request frequency, incorrect answer format parsing, or network failure.
 
-`score_by`: array ${\color{grey}\text{Optional}}$ Defaults to null <br> Used to determine the groups for the groupby `pandas.groupby(by=args.score_by)` to get the summary scores of certain groups.
+`--score_by`: array ${\color{grey}\text{Optional}}$ Defaults to null <br> Used to determine the groups for the groupby `pandas.groupby(by=args.score_by)` to get the summary scores of certain groups.
 
 
 ## ToDo
 - [ ] Conbining multiple GPT-like models for prediction: routing or simply averaging.
 - [ ] Supporting prompts evaluation by output the accuracy of different prompts. 
 - [ ] Configuring a default test set for prompt evaluation.
```

### Comparing `auto-eval-0.2.2/eval/auto_llms_eval.py` & `auto-eval-0.2.3/eval/auto_llms_eval.py`

 * *Files identical despite different names*

### Comparing `auto-eval-0.2.2/eval/commands/auto_eval.py` & `auto-eval-0.2.3/eval/commands/auto_eval.py`

 * *Files identical despite different names*

### Comparing `auto-eval-0.2.2/eval/prompt_template/prompter.py` & `auto-eval-0.2.3/eval/prompt_template/prompter.py`

 * *Files identical despite different names*

### Comparing `auto-eval-0.2.2/eval/prompt_template/prompts.py` & `auto-eval-0.2.3/eval/prompt_template/prompts.py`

 * *Files identical despite different names*

### Comparing `auto-eval-0.2.2/eval/utils/data_utils.py` & `auto-eval-0.2.3/eval/utils/data_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,23 +13,25 @@
         df_data = pd.read_json(data_path, lines=True)
     elif data_path.endswith('xlsx'):
         df_data = pd.read_excel(data_path, header=header, usecols=usecols, sheet_name=sheet_name)
     elif data_path.endswith('.pkl'):
         df_data = pd.read_pickle(data_path)
     elif data_path.endswith('csv'):
         df_data = pd.read_csv(data_path, header=header, usecols=usecols, sep=sep)
+    elif data_path.endswith('.parquet'):
+        df_data = pd.read_parquet(data_path)
     else:
         raise AssertionError(f'not supported file type:{data_path}, suport types: json, jsonl, xlsx, csv')
     return df_data
 
 def df_saver(df: pd.DataFrame, data_path):
     if data_path.endswith('json'):
-        df.to_json(df, orient='records', force_ascii=False)
+        df.to_json(data_path, orient='records', force_ascii=False)
     if data_path.endswith('jsonl'):
-        df.to_json(df, orient='records', force_ascii=False, lines=True)
+        df.to_json(data_path, orient='records', force_ascii=False, lines=True)
     elif data_path.endswith('xlsx'):
         df2xlsx(df, data_path, index=False)
     elif data_path.endswith('csv'):
         df.to_csv(data_path)
     else:
         raise AssertionError(f'not supported file type:{data_path}, suport types: json, jsonl, xlsx, csv')
```

### Comparing `auto-eval-0.2.2/setup.py` & `auto-eval-0.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="auto-eval",
-    version="0.2.2",
+    version="0.2.3",
     packages=find_packages(),
     # package_data={
     #   "eval":["prompt_template/eval_prompt_template.json"]  
     # },
     install_requires=[
         # Add your library's dependencies here
         "one-api-tool",
```

