# Comparing `tmp/zh-langchain-0.1.0.tar.gz` & `tmp/zh-langchain-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zh-langchain-0.1.0.tar", last modified: Thu May 25 12:18:47 2023, max compression
+gzip compressed data, was "zh-langchain-0.1.1.tar", last modified: Thu May 25 12:35:18 2023, max compression
```

## Comparing `zh-langchain-0.1.0.tar` & `zh-langchain-0.1.1.tar`

### file list

```diff
@@ -1,27 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 12:18:47.008429 zh-langchain-0.1.0/
--rw-rw-rw-   0        0        0    11558 2023-05-21 14:47:03.000000 zh-langchain-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      493 2023-05-25 12:18:47.008429 zh-langchain-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0    12241 2023-05-21 14:47:03.000000 zh-langchain-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-25 12:18:46.965546 zh-langchain-0.1.0/agent/
--rw-rw-rw-   0        0        0       52 2023-05-21 14:47:03.000000 zh-langchain-0.1.0/agent/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 12:18:46.972504 zh-langchain-0.1.0/loader/
--rw-rw-rw-   0        0        0      110 2023-05-21 14:47:03.000000 zh-langchain-0.1.0/loader/__init__.py
--rw-rw-rw-   0        0        0     1577 2023-05-21 14:47:03.000000 zh-langchain-0.1.0/loader/image_loader.py
--rw-rw-rw-   0        0        0     2138 2023-05-21 14:47:03.000000 zh-langchain-0.1.0/loader/pdf_loader.py
-drwxrwxrwx   0        0        0        0 2023-05-25 12:18:46.981807 zh-langchain-0.1.0/models/
--rw-rw-rw-   0        0        0       28 2023-05-21 14:47:03.000000 zh-langchain-0.1.0/models/__init__.py
--rw-rw-rw-   0        0        0     7591 2023-05-21 14:47:03.000000 zh-langchain-0.1.0/models/chatglm_llm.py
--rw-rw-rw-   0        0        0     7775 2023-05-21 14:47:03.000000 zh-langchain-0.1.0/models/moss_llm.py
--rw-rw-rw-   0        0        0       42 2023-05-25 12:18:47.008429 zh-langchain-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      573 2023-05-25 12:17:56.000000 zh-langchain-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-25 12:18:46.991224 zh-langchain-0.1.0/textsplitter/
--rw-rw-rw-   0        0        0      102 2023-05-21 14:47:03.000000 zh-langchain-0.1.0/textsplitter/__init__.py
--rw-rw-rw-   0        0        0     1416 2023-05-21 14:47:03.000000 zh-langchain-0.1.0/textsplitter/ali_text_splitter.py
--rw-rw-rw-   0        0        0     3376 2023-05-21 14:47:03.000000 zh-langchain-0.1.0/textsplitter/chinese_text_splitter.py
-drwxrwxrwx   0        0        0        0 2023-05-25 12:18:46.993866 zh-langchain-0.1.0/utils/
--rw-rw-rw-   0        0        0      525 2023-05-21 14:47:03.000000 zh-langchain-0.1.0/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 12:18:47.006129 zh-langchain-0.1.0/zh_langchain.egg-info/
--rw-rw-rw-   0        0        0      493 2023-05-25 12:18:46.000000 zh-langchain-0.1.0/zh_langchain.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      426 2023-05-25 12:18:46.000000 zh-langchain-0.1.0/zh_langchain.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 12:18:46.000000 zh-langchain-0.1.0/zh_langchain.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-05-25 12:18:46.000000 zh-langchain-0.1.0/zh_langchain.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-25 12:35:18.593931 zh-langchain-0.1.1/
+-rw-rw-rw-   0        0        0    11558 2023-05-21 14:47:03.000000 zh-langchain-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      493 2023-05-25 12:35:18.592868 zh-langchain-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0    12241 2023-05-21 14:47:03.000000 zh-langchain-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-25 12:35:18.525198 zh-langchain-0.1.1/agent/
+-rw-rw-rw-   0        0        0       52 2023-05-21 14:47:03.000000 zh-langchain-0.1.1/agent/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 12:35:18.536705 zh-langchain-0.1.1/chains/
+-rw-rw-rw-   0        0        0       36 2023-05-25 12:33:30.000000 zh-langchain-0.1.1/chains/__init__.py
+-rw-rw-rw-   0        0        0    12754 2023-05-25 11:45:01.000000 zh-langchain-0.1.1/chains/local_doc_qa.py
+-rw-rw-rw-   0        0        0     1755 2023-05-21 14:47:03.000000 zh-langchain-0.1.1/chains/text_load.py
+drwxrwxrwx   0        0        0        0 2023-05-25 12:35:18.548673 zh-langchain-0.1.1/loader/
+-rw-rw-rw-   0        0        0      110 2023-05-21 14:47:03.000000 zh-langchain-0.1.1/loader/__init__.py
+-rw-rw-rw-   0        0        0     1577 2023-05-21 14:47:03.000000 zh-langchain-0.1.1/loader/image_loader.py
+-rw-rw-rw-   0        0        0     2138 2023-05-21 14:47:03.000000 zh-langchain-0.1.1/loader/pdf_loader.py
+drwxrwxrwx   0        0        0        0 2023-05-25 12:35:18.558218 zh-langchain-0.1.1/models/
+-rw-rw-rw-   0        0        0       28 2023-05-21 14:47:03.000000 zh-langchain-0.1.1/models/__init__.py
+-rw-rw-rw-   0        0        0     7591 2023-05-21 14:47:03.000000 zh-langchain-0.1.1/models/chatglm_llm.py
+-rw-rw-rw-   0        0        0     7775 2023-05-21 14:47:03.000000 zh-langchain-0.1.1/models/moss_llm.py
+-rw-rw-rw-   0        0        0       42 2023-05-25 12:35:18.595131 zh-langchain-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      573 2023-05-25 12:34:45.000000 zh-langchain-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-25 12:35:18.570697 zh-langchain-0.1.1/textsplitter/
+-rw-rw-rw-   0        0        0      102 2023-05-21 14:47:03.000000 zh-langchain-0.1.1/textsplitter/__init__.py
+-rw-rw-rw-   0        0        0     1416 2023-05-21 14:47:03.000000 zh-langchain-0.1.1/textsplitter/ali_text_splitter.py
+-rw-rw-rw-   0        0        0     3376 2023-05-21 14:47:03.000000 zh-langchain-0.1.1/textsplitter/chinese_text_splitter.py
+drwxrwxrwx   0        0        0        0 2023-05-25 12:35:18.573694 zh-langchain-0.1.1/utils/
+-rw-rw-rw-   0        0        0      525 2023-05-21 14:47:03.000000 zh-langchain-0.1.1/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 12:35:18.589351 zh-langchain-0.1.1/zh_langchain.egg-info/
+-rw-rw-rw-   0        0        0      493 2023-05-25 12:35:18.000000 zh-langchain-0.1.1/zh_langchain.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      488 2023-05-25 12:35:18.000000 zh-langchain-0.1.1/zh_langchain.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 12:35:18.000000 zh-langchain-0.1.1/zh_langchain.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-05-25 12:35:18.000000 zh-langchain-0.1.1/zh_langchain.egg-info/top_level.txt
```

### Comparing `zh-langchain-0.1.0/LICENSE` & `zh-langchain-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `zh-langchain-0.1.0/README.md` & `zh-langchain-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `zh-langchain-0.1.0/loader/image_loader.py` & `zh-langchain-0.1.1/loader/image_loader.py`

 * *Files identical despite different names*

### Comparing `zh-langchain-0.1.0/loader/pdf_loader.py` & `zh-langchain-0.1.1/loader/pdf_loader.py`

 * *Files identical despite different names*

### Comparing `zh-langchain-0.1.0/models/chatglm_llm.py` & `zh-langchain-0.1.1/models/chatglm_llm.py`

 * *Files identical despite different names*

### Comparing `zh-langchain-0.1.0/models/moss_llm.py` & `zh-langchain-0.1.1/models/moss_llm.py`

 * *Files identical despite different names*

### Comparing `zh-langchain-0.1.0/setup.py` & `zh-langchain-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='zh-langchain',
-    version='0.1.0',
+    version='0.1.1',
     description='Chinese language processing library',
     author='Your Name',
     author_email='your.email@example.com',
     url='https://github.com/imClumsyPanda/langchain-ChatGLM.git',
     packages=find_packages(),
     install_requires=[
     ],
```

### Comparing `zh-langchain-0.1.0/textsplitter/ali_text_splitter.py` & `zh-langchain-0.1.1/textsplitter/ali_text_splitter.py`

 * *Files identical despite different names*

### Comparing `zh-langchain-0.1.0/textsplitter/chinese_text_splitter.py` & `zh-langchain-0.1.1/textsplitter/chinese_text_splitter.py`

 * *Files identical despite different names*

### Comparing `zh-langchain-0.1.0/utils/__init__.py` & `zh-langchain-0.1.1/utils/__init__.py`

 * *Files identical despite different names*

