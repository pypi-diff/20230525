# Comparing `tmp/caafe-0.1.4.tar.gz` & `tmp/caafe-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caafe-0.1.4.tar", last modified: Thu May 25 18:27:20 2023, max compression
+gzip compressed data, was "caafe-0.1.5.tar", last modified: Thu May 25 18:31:13 2023, max compression
```

## Comparing `caafe-0.1.4.tar` & `caafe-0.1.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 18:27:20.181375 caafe-0.1.4/
--rw-r--r--   0 root         (0) root         (0)      381 2023-05-25 18:27:01.000000 caafe-0.1.4/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)     6826 2023-05-25 18:27:20.181375 caafe-0.1.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5953 2023-05-25 18:27:01.000000 caafe-0.1.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 18:27:20.180374 caafe-0.1.4/caafe/
--rw-r--r--   0 root         (0) root         (0)       45 2023-05-25 18:27:01.000000 caafe-0.1.4/caafe/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11664 2023-05-25 18:27:01.000000 caafe-0.1.4/caafe/caafe.py
--rw-r--r--   0 root         (0) root         (0)     4249 2023-05-25 18:27:01.000000 caafe-0.1.4/caafe/caafe_evaluate.py
--rw-r--r--   0 root         (0) root         (0)    11101 2023-05-25 18:27:01.000000 caafe-0.1.4/caafe/data.py
--rw-r--r--   0 root         (0) root         (0)     4399 2023-05-25 18:27:01.000000 caafe-0.1.4/caafe/evaluate.py
--rw-r--r--   0 root         (0) root         (0)     3605 2023-05-25 18:27:01.000000 caafe-0.1.4/caafe/feature_extension_baselines.py
--rw-r--r--   0 root         (0) root         (0)     1482 2023-05-25 18:27:01.000000 caafe-0.1.4/caafe/metrics.py
--rw-r--r--   0 root         (0) root         (0)     4439 2023-05-25 18:27:01.000000 caafe-0.1.4/caafe/plotting.py
--rw-r--r--   0 root         (0) root         (0)     4467 2023-05-25 18:27:01.000000 caafe-0.1.4/caafe/preprocessing.py
--rw-r--r--   0 root         (0) root         (0)     7895 2023-05-25 18:27:01.000000 caafe-0.1.4/caafe/run_llm_code.py
--rw-r--r--   0 root         (0) root         (0)     7065 2023-05-25 18:27:01.000000 caafe-0.1.4/caafe/sklearn_wrapper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 18:27:20.181375 caafe-0.1.4/caafe.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6826 2023-05-25 18:27:19.000000 caafe-0.1.4/caafe.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      435 2023-05-25 18:27:20.000000 caafe-0.1.4/caafe.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 18:27:19.000000 caafe-0.1.4/caafe.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       79 2023-05-25 18:27:19.000000 caafe-0.1.4/caafe.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-05-25 18:27:19.000000 caafe-0.1.4/caafe.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-25 18:27:20.182375 caafe-0.1.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1211 2023-05-25 18:27:01.000000 caafe-0.1.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 18:27:20.181375 caafe-0.1.4/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 18:27:01.000000 caafe-0.1.4/tests/test_sklearn_wrapper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 18:31:13.511086 caafe-0.1.5/
+-rw-r--r--   0 root         (0) root         (0)      381 2023-05-25 18:30:36.000000 caafe-0.1.5/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)     6846 2023-05-25 18:31:13.511086 caafe-0.1.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6002 2023-05-25 18:30:36.000000 caafe-0.1.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 18:31:13.510086 caafe-0.1.5/caafe/
+-rw-r--r--   0 root         (0) root         (0)       45 2023-05-25 18:30:36.000000 caafe-0.1.5/caafe/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11664 2023-05-25 18:30:36.000000 caafe-0.1.5/caafe/caafe.py
+-rw-r--r--   0 root         (0) root         (0)     4249 2023-05-25 18:30:36.000000 caafe-0.1.5/caafe/caafe_evaluate.py
+-rw-r--r--   0 root         (0) root         (0)    11101 2023-05-25 18:30:36.000000 caafe-0.1.5/caafe/data.py
+-rw-r--r--   0 root         (0) root         (0)     4399 2023-05-25 18:30:36.000000 caafe-0.1.5/caafe/evaluate.py
+-rw-r--r--   0 root         (0) root         (0)     3605 2023-05-25 18:30:36.000000 caafe-0.1.5/caafe/feature_extension_baselines.py
+-rw-r--r--   0 root         (0) root         (0)     1482 2023-05-25 18:30:36.000000 caafe-0.1.5/caafe/metrics.py
+-rw-r--r--   0 root         (0) root         (0)     4439 2023-05-25 18:30:36.000000 caafe-0.1.5/caafe/plotting.py
+-rw-r--r--   0 root         (0) root         (0)     4467 2023-05-25 18:30:36.000000 caafe-0.1.5/caafe/preprocessing.py
+-rw-r--r--   0 root         (0) root         (0)     7895 2023-05-25 18:30:36.000000 caafe-0.1.5/caafe/run_llm_code.py
+-rw-r--r--   0 root         (0) root         (0)     7065 2023-05-25 18:30:36.000000 caafe-0.1.5/caafe/sklearn_wrapper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 18:31:13.510086 caafe-0.1.5/caafe.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6846 2023-05-25 18:31:13.000000 caafe-0.1.5/caafe.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      435 2023-05-25 18:31:13.000000 caafe-0.1.5/caafe.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 18:31:13.000000 caafe-0.1.5/caafe.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       79 2023-05-25 18:31:13.000000 caafe-0.1.5/caafe.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-05-25 18:31:13.000000 caafe-0.1.5/caafe.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-25 18:31:13.511086 caafe-0.1.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1182 2023-05-25 18:31:10.000000 caafe-0.1.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 18:31:13.511086 caafe-0.1.5/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 18:30:36.000000 caafe-0.1.5/tests/test_sklearn_wrapper.py
```

### Comparing `caafe-0.1.4/PKG-INFO` & `caafe-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: caafe
-Version: 0.1.4
-Summary: Context-Aware Automated Feature Engineering (CAAFE) is an automated machine learning tool that uses large language models for feature engineering in tabular datasets. It generates Python code for new features along with explanations for their utility, enhancing interpretability. Find at more at priorlabs.ai
+Version: 0.1.5
+Summary: Context-Aware Automated Feature Engineering (CAAFE) is an automated machine learning tool that uses large language models for feature engineering in tabular datasets. It generates Python code for new features along with explanations for their utility, enhancing interpretability.
 Home-page: https://github.com/automl/CAAFE
 Author: Noah Hollmann, Samuel Müller, Frank Hutter
 Author-email: noah.homa@gmail.com
 License: LICENSE.txt
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: Free for non-commercial use
 Classifier: Programming Language :: Python :: 3.7
@@ -78,14 +78,16 @@
 CAAFE uses OpenAIs GPT-4 or GPT-3.5 as an endpoint. OpenAI charges The cost of running CAAFE depends on the number of iterations, the number of features in the dataset, the length of the dataset description and of the generated code. For example, for a dataset with 1000 rows and 10 columns, 10 iterations cost about 0.50$ for GPT-4 and 0.05$ for GPT-3.5.
 
 ### Paper
 Hollmann, N., Müller, S., & Hutter, F. (2023). LLMs for Semi-Automated Data Science: Introducing CAAFE for Context-Aware Automated Feature Engineering
 https://arxiv.org/abs/2305.03403
 
 ### License
+Copyright by [Prior Labs](http://priorlabs.ai).
+
 [![CC BY-NC-SA 4.0][cc-by-nc-sa-shield]][cc-by-nc-sa]
 
 This work is licensed under a
 [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License][cc-by-nc-sa].
 
 [![CC BY-NC-SA 4.0][cc-by-nc-sa-image]][cc-by-nc-sa]
```

### Comparing `caafe-0.1.4/README.md` & `caafe-0.1.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -60,14 +60,16 @@
 CAAFE uses OpenAIs GPT-4 or GPT-3.5 as an endpoint. OpenAI charges The cost of running CAAFE depends on the number of iterations, the number of features in the dataset, the length of the dataset description and of the generated code. For example, for a dataset with 1000 rows and 10 columns, 10 iterations cost about 0.50$ for GPT-4 and 0.05$ for GPT-3.5.
 
 ### Paper
 Hollmann, N., Müller, S., & Hutter, F. (2023). LLMs for Semi-Automated Data Science: Introducing CAAFE for Context-Aware Automated Feature Engineering
 https://arxiv.org/abs/2305.03403
 
 ### License
+Copyright by [Prior Labs](http://priorlabs.ai).
+
 [![CC BY-NC-SA 4.0][cc-by-nc-sa-shield]][cc-by-nc-sa]
 
 This work is licensed under a
 [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License][cc-by-nc-sa].
 
 [![CC BY-NC-SA 4.0][cc-by-nc-sa-image]][cc-by-nc-sa]
```

### Comparing `caafe-0.1.4/caafe/caafe.py` & `caafe-0.1.5/caafe/caafe.py`

 * *Files identical despite different names*

### Comparing `caafe-0.1.4/caafe/caafe_evaluate.py` & `caafe-0.1.5/caafe/caafe_evaluate.py`

 * *Files identical despite different names*

### Comparing `caafe-0.1.4/caafe/data.py` & `caafe-0.1.5/caafe/data.py`

 * *Files identical despite different names*

### Comparing `caafe-0.1.4/caafe/evaluate.py` & `caafe-0.1.5/caafe/evaluate.py`

 * *Files identical despite different names*

### Comparing `caafe-0.1.4/caafe/feature_extension_baselines.py` & `caafe-0.1.5/caafe/feature_extension_baselines.py`

 * *Files identical despite different names*

### Comparing `caafe-0.1.4/caafe/metrics.py` & `caafe-0.1.5/caafe/metrics.py`

 * *Files identical despite different names*

### Comparing `caafe-0.1.4/caafe/plotting.py` & `caafe-0.1.5/caafe/plotting.py`

 * *Files identical despite different names*

### Comparing `caafe-0.1.4/caafe/preprocessing.py` & `caafe-0.1.5/caafe/preprocessing.py`

 * *Files identical despite different names*

### Comparing `caafe-0.1.4/caafe/run_llm_code.py` & `caafe-0.1.5/caafe/run_llm_code.py`

 * *Files identical despite different names*

### Comparing `caafe-0.1.4/caafe/sklearn_wrapper.py` & `caafe-0.1.5/caafe/sklearn_wrapper.py`

 * *Files identical despite different names*

### Comparing `caafe-0.1.4/caafe.egg-info/PKG-INFO` & `caafe-0.1.5/caafe.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: caafe
-Version: 0.1.4
-Summary: Context-Aware Automated Feature Engineering (CAAFE) is an automated machine learning tool that uses large language models for feature engineering in tabular datasets. It generates Python code for new features along with explanations for their utility, enhancing interpretability. Find at more at priorlabs.ai
+Version: 0.1.5
+Summary: Context-Aware Automated Feature Engineering (CAAFE) is an automated machine learning tool that uses large language models for feature engineering in tabular datasets. It generates Python code for new features along with explanations for their utility, enhancing interpretability.
 Home-page: https://github.com/automl/CAAFE
 Author: Noah Hollmann, Samuel Müller, Frank Hutter
 Author-email: noah.homa@gmail.com
 License: LICENSE.txt
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: Free for non-commercial use
 Classifier: Programming Language :: Python :: 3.7
@@ -78,14 +78,16 @@
 CAAFE uses OpenAIs GPT-4 or GPT-3.5 as an endpoint. OpenAI charges The cost of running CAAFE depends on the number of iterations, the number of features in the dataset, the length of the dataset description and of the generated code. For example, for a dataset with 1000 rows and 10 columns, 10 iterations cost about 0.50$ for GPT-4 and 0.05$ for GPT-3.5.
 
 ### Paper
 Hollmann, N., Müller, S., & Hutter, F. (2023). LLMs for Semi-Automated Data Science: Introducing CAAFE for Context-Aware Automated Feature Engineering
 https://arxiv.org/abs/2305.03403
 
 ### License
+Copyright by [Prior Labs](http://priorlabs.ai).
+
 [![CC BY-NC-SA 4.0][cc-by-nc-sa-shield]][cc-by-nc-sa]
 
 This work is licensed under a
 [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License][cc-by-nc-sa].
 
 [![CC BY-NC-SA 4.0][cc-by-nc-sa-image]][cc-by-nc-sa]
```

### Comparing `caafe-0.1.4/setup.py` & `caafe-0.1.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 setup(
     name="caafe",
-    version="0.1.4",
+    version="0.1.5",
     packages=find_packages(),
-    description="Context-Aware Automated Feature Engineering (CAAFE) is an automated machine learning tool that uses large language models for feature engineering in tabular datasets. It generates Python code for new features along with explanations for their utility, enhancing interpretability. Find at more at priorlabs.ai",
+    description="Context-Aware Automated Feature Engineering (CAAFE) is an automated machine learning tool that uses large language models for feature engineering in tabular datasets. It generates Python code for new features along with explanations for their utility, enhancing interpretability.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Noah Hollmann, Samuel Müller, Frank Hutter",
     author_email="noah.homa@gmail.com",
     url="https://github.com/automl/CAAFE",
     license="LICENSE.txt",
     classifiers=[
```

