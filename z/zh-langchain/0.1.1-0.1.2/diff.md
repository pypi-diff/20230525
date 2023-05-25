# Comparing `tmp/zh-langchain-0.1.1.tar.gz` & `tmp/zh-langchain-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zh-langchain-0.1.1.tar", last modified: Thu May 25 12:35:18 2023, max compression
+gzip compressed data, was "zh-langchain-0.1.2.tar", last modified: Thu May 25 12:43:08 2023, max compression
```

## Comparing `zh-langchain-0.1.1.tar` & `zh-langchain-0.1.2.tar`

### file list

```diff
@@ -1,31 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 12:35:18.593931 zh-langchain-0.1.1/
--rw-rw-rw-   0        0        0    11558 2023-05-21 14:47:03.000000 zh-langchain-0.1.1/LICENSE
--rw-rw-rw-   0        0        0      493 2023-05-25 12:35:18.592868 zh-langchain-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0    12241 2023-05-21 14:47:03.000000 zh-langchain-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-25 12:35:18.525198 zh-langchain-0.1.1/agent/
--rw-rw-rw-   0        0        0       52 2023-05-21 14:47:03.000000 zh-langchain-0.1.1/agent/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 12:35:18.536705 zh-langchain-0.1.1/chains/
--rw-rw-rw-   0        0        0       36 2023-05-25 12:33:30.000000 zh-langchain-0.1.1/chains/__init__.py
--rw-rw-rw-   0        0        0    12754 2023-05-25 11:45:01.000000 zh-langchain-0.1.1/chains/local_doc_qa.py
--rw-rw-rw-   0        0        0     1755 2023-05-21 14:47:03.000000 zh-langchain-0.1.1/chains/text_load.py
-drwxrwxrwx   0        0        0        0 2023-05-25 12:35:18.548673 zh-langchain-0.1.1/loader/
--rw-rw-rw-   0        0        0      110 2023-05-21 14:47:03.000000 zh-langchain-0.1.1/loader/__init__.py
--rw-rw-rw-   0        0        0     1577 2023-05-21 14:47:03.000000 zh-langchain-0.1.1/loader/image_loader.py
--rw-rw-rw-   0        0        0     2138 2023-05-21 14:47:03.000000 zh-langchain-0.1.1/loader/pdf_loader.py
-drwxrwxrwx   0        0        0        0 2023-05-25 12:35:18.558218 zh-langchain-0.1.1/models/
--rw-rw-rw-   0        0        0       28 2023-05-21 14:47:03.000000 zh-langchain-0.1.1/models/__init__.py
--rw-rw-rw-   0        0        0     7591 2023-05-21 14:47:03.000000 zh-langchain-0.1.1/models/chatglm_llm.py
--rw-rw-rw-   0        0        0     7775 2023-05-21 14:47:03.000000 zh-langchain-0.1.1/models/moss_llm.py
--rw-rw-rw-   0        0        0       42 2023-05-25 12:35:18.595131 zh-langchain-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      573 2023-05-25 12:34:45.000000 zh-langchain-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-25 12:35:18.570697 zh-langchain-0.1.1/textsplitter/
--rw-rw-rw-   0        0        0      102 2023-05-21 14:47:03.000000 zh-langchain-0.1.1/textsplitter/__init__.py
--rw-rw-rw-   0        0        0     1416 2023-05-21 14:47:03.000000 zh-langchain-0.1.1/textsplitter/ali_text_splitter.py
--rw-rw-rw-   0        0        0     3376 2023-05-21 14:47:03.000000 zh-langchain-0.1.1/textsplitter/chinese_text_splitter.py
-drwxrwxrwx   0        0        0        0 2023-05-25 12:35:18.573694 zh-langchain-0.1.1/utils/
--rw-rw-rw-   0        0        0      525 2023-05-21 14:47:03.000000 zh-langchain-0.1.1/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 12:35:18.589351 zh-langchain-0.1.1/zh_langchain.egg-info/
--rw-rw-rw-   0        0        0      493 2023-05-25 12:35:18.000000 zh-langchain-0.1.1/zh_langchain.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      488 2023-05-25 12:35:18.000000 zh-langchain-0.1.1/zh_langchain.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 12:35:18.000000 zh-langchain-0.1.1/zh_langchain.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-05-25 12:35:18.000000 zh-langchain-0.1.1/zh_langchain.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-25 12:43:08.704181 zh-langchain-0.1.2/
+-rw-rw-rw-   0        0        0      470 2023-05-25 12:43:08.695207 zh-langchain-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0    12241 2023-05-21 14:47:03.000000 zh-langchain-0.1.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-25 12:43:08.704181 zh-langchain-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      615 2023-05-25 12:42:53.000000 zh-langchain-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-25 12:43:08.592728 zh-langchain-0.1.2/zh_langchain/
+-rw-rw-rw-   0        0        0       60 2023-05-25 12:34:21.000000 zh-langchain-0.1.2/zh_langchain/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 12:43:08.614862 zh-langchain-0.1.2/zh_langchain/agent/
+-rw-rw-rw-   0        0        0       52 2023-05-21 14:47:03.000000 zh-langchain-0.1.2/zh_langchain/agent/__init__.py
+-rw-rw-rw-   0        0        0    14843 2023-05-21 14:47:03.000000 zh-langchain-0.1.2/zh_langchain/api.py
+drwxrwxrwx   0        0        0        0 2023-05-25 12:43:08.626829 zh-langchain-0.1.2/zh_langchain/chains/
+-rw-rw-rw-   0        0        0       36 2023-05-25 12:33:30.000000 zh-langchain-0.1.2/zh_langchain/chains/__init__.py
+-rw-rw-rw-   0        0        0    12754 2023-05-25 11:45:01.000000 zh-langchain-0.1.2/zh_langchain/chains/local_doc_qa.py
+-rw-rw-rw-   0        0        0     1755 2023-05-21 14:47:03.000000 zh-langchain-0.1.2/zh_langchain/chains/text_load.py
+-rw-rw-rw-   0        0        0     1240 2023-05-21 14:47:03.000000 zh-langchain-0.1.2/zh_langchain/cli.py
+-rw-rw-rw-   0        0        0     2090 2023-05-21 14:47:03.000000 zh-langchain-0.1.2/zh_langchain/cli_demo.py
+-rw-rw-rw-   0        0        0        0 2023-05-25 11:45:18.000000 zh-langchain-0.1.2/zh_langchain/cradle.py
+drwxrwxrwx   0        0        0        0 2023-05-25 12:43:08.646788 zh-langchain-0.1.2/zh_langchain/loader/
+-rw-rw-rw-   0        0        0      110 2023-05-21 14:47:03.000000 zh-langchain-0.1.2/zh_langchain/loader/__init__.py
+-rw-rw-rw-   0        0        0     1577 2023-05-21 14:47:03.000000 zh-langchain-0.1.2/zh_langchain/loader/image_loader.py
+-rw-rw-rw-   0        0        0     2138 2023-05-21 14:47:03.000000 zh-langchain-0.1.2/zh_langchain/loader/pdf_loader.py
+drwxrwxrwx   0        0        0        0 2023-05-25 12:43:08.657305 zh-langchain-0.1.2/zh_langchain/models/
+-rw-rw-rw-   0        0        0       28 2023-05-21 14:47:03.000000 zh-langchain-0.1.2/zh_langchain/models/__init__.py
+-rw-rw-rw-   0        0        0     7591 2023-05-21 14:47:03.000000 zh-langchain-0.1.2/zh_langchain/models/chatglm_llm.py
+-rw-rw-rw-   0        0        0     7775 2023-05-21 14:47:03.000000 zh-langchain-0.1.2/zh_langchain/models/moss_llm.py
+-rw-rw-rw-   0        0        0     1600 2023-05-21 14:47:03.000000 zh-langchain-0.1.2/zh_langchain/release.py
+drwxrwxrwx   0        0        0        0 2023-05-25 12:43:08.668278 zh-langchain-0.1.2/zh_langchain/textsplitter/
+-rw-rw-rw-   0        0        0      102 2023-05-21 14:47:03.000000 zh-langchain-0.1.2/zh_langchain/textsplitter/__init__.py
+-rw-rw-rw-   0        0        0     1416 2023-05-21 14:47:03.000000 zh-langchain-0.1.2/zh_langchain/textsplitter/ali_text_splitter.py
+-rw-rw-rw-   0        0        0     3376 2023-05-21 14:47:03.000000 zh-langchain-0.1.2/zh_langchain/textsplitter/chinese_text_splitter.py
+drwxrwxrwx   0        0        0        0 2023-05-25 12:43:08.672267 zh-langchain-0.1.2/zh_langchain/utils/
+-rw-rw-rw-   0        0        0      525 2023-05-21 14:47:03.000000 zh-langchain-0.1.2/zh_langchain/utils/__init__.py
+-rw-rw-rw-   0        0        0    25632 2023-05-25 11:26:09.000000 zh-langchain-0.1.2/zh_langchain/webui.py
+-rw-rw-rw-   0        0        0     2948 2023-05-25 12:34:27.000000 zh-langchain-0.1.2/zh_langchain/zh_langchain.py
+drwxrwxrwx   0        0        0        0 2023-05-25 12:43:08.611869 zh-langchain-0.1.2/zh_langchain.egg-info/
+-rw-rw-rw-   0        0        0      470 2023-05-25 12:43:08.000000 zh-langchain-0.1.2/zh_langchain.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      850 2023-05-25 12:43:08.000000 zh-langchain-0.1.2/zh_langchain.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 12:43:08.000000 zh-langchain-0.1.2/zh_langchain.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-25 12:43:08.000000 zh-langchain-0.1.2/zh_langchain.egg-info/top_level.txt
```

### Comparing `zh-langchain-0.1.1/README.md` & `zh-langchain-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `zh-langchain-0.1.1/chains/local_doc_qa.py` & `zh-langchain-0.1.2/zh_langchain/chains/local_doc_qa.py`

 * *Files identical despite different names*

### Comparing `zh-langchain-0.1.1/chains/text_load.py` & `zh-langchain-0.1.2/zh_langchain/chains/text_load.py`

 * *Files identical despite different names*

### Comparing `zh-langchain-0.1.1/loader/image_loader.py` & `zh-langchain-0.1.2/zh_langchain/loader/image_loader.py`

 * *Files identical despite different names*

### Comparing `zh-langchain-0.1.1/loader/pdf_loader.py` & `zh-langchain-0.1.2/zh_langchain/loader/pdf_loader.py`

 * *Files identical despite different names*

### Comparing `zh-langchain-0.1.1/models/chatglm_llm.py` & `zh-langchain-0.1.2/zh_langchain/models/chatglm_llm.py`

 * *Files identical despite different names*

### Comparing `zh-langchain-0.1.1/models/moss_llm.py` & `zh-langchain-0.1.2/zh_langchain/models/moss_llm.py`

 * *Files identical despite different names*

### Comparing `zh-langchain-0.1.1/setup.py` & `zh-langchain-0.1.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup, find_packages
 
 setup(
     name='zh-langchain',
-    version='0.1.1',
+    version='0.1.2',
     description='Chinese language processing library',
     author='Your Name',
     author_email='your.email@example.com',
     url='https://github.com/imClumsyPanda/langchain-ChatGLM.git',
-    packages=find_packages(),
+    packages=find_packages(include=['zh_langchain', 'zh_langchain.*']),
     install_requires=[
     ],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
```

### Comparing `zh-langchain-0.1.1/textsplitter/ali_text_splitter.py` & `zh-langchain-0.1.2/zh_langchain/textsplitter/ali_text_splitter.py`

 * *Files identical despite different names*

### Comparing `zh-langchain-0.1.1/textsplitter/chinese_text_splitter.py` & `zh-langchain-0.1.2/zh_langchain/textsplitter/chinese_text_splitter.py`

 * *Files identical despite different names*

### Comparing `zh-langchain-0.1.1/utils/__init__.py` & `zh-langchain-0.1.2/zh_langchain/utils/__init__.py`

 * *Files identical despite different names*

