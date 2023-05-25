# Comparing `tmp/knowledgebase-gsheet-gpt-1.2.8.tar.gz` & `tmp/knowledgebase-gsheet-gpt-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "knowledgebase-gsheet-gpt-1.2.8.tar", last modified: Wed May 24 06:53:05 2023, max compression
+gzip compressed data, was "knowledgebase-gsheet-gpt-1.2.9.tar", last modified: Thu May 25 14:31:53 2023, max compression
```

## Comparing `knowledgebase-gsheet-gpt-1.2.8.tar` & `knowledgebase-gsheet-gpt-1.2.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-05-24 06:53:05.943923 knowledgebase-gsheet-gpt-1.2.8/
--rw-r--r--   0 chiubowen   (501) staff       (20)     1658 2023-05-24 06:53:05.943803 knowledgebase-gsheet-gpt-1.2.8/PKG-INFO
--rw-r--r--   0 chiubowen   (501) staff       (20)     1476 2023-05-24 06:53:05.000000 knowledgebase-gsheet-gpt-1.2.8/README.md
-drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-05-24 06:53:05.943622 knowledgebase-gsheet-gpt-1.2.8/knowledgebase_gsheet_gpt.egg-info/
--rw-r--r--   0 chiubowen   (501) staff       (20)     1658 2023-05-24 06:53:05.000000 knowledgebase-gsheet-gpt-1.2.8/knowledgebase_gsheet_gpt.egg-info/PKG-INFO
--rw-r--r--   0 chiubowen   (501) staff       (20)      336 2023-05-24 06:53:05.000000 knowledgebase-gsheet-gpt-1.2.8/knowledgebase_gsheet_gpt.egg-info/SOURCES.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)        1 2023-05-24 06:53:05.000000 knowledgebase-gsheet-gpt-1.2.8/knowledgebase_gsheet_gpt.egg-info/dependency_links.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)       76 2023-05-24 06:53:05.000000 knowledgebase-gsheet-gpt-1.2.8/knowledgebase_gsheet_gpt.egg-info/entry_points.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)      112 2023-05-24 06:53:05.000000 knowledgebase-gsheet-gpt-1.2.8/knowledgebase_gsheet_gpt.egg-info/requires.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)       25 2023-05-24 06:53:05.000000 knowledgebase-gsheet-gpt-1.2.8/knowledgebase_gsheet_gpt.egg-info/top_level.txt
--rwxr-xr-x   0 chiubowen   (501) staff       (20)     6193 2023-05-24 06:53:05.000000 knowledgebase-gsheet-gpt-1.2.8/knowledgebase_gsheet_gpt.py
--rw-r--r--   0 chiubowen   (501) staff       (20)       38 2023-05-24 06:53:05.943962 knowledgebase-gsheet-gpt-1.2.8/setup.cfg
--rw-r--r--   0 chiubowen   (501) staff       (20)      560 2023-05-24 06:53:05.000000 knowledgebase-gsheet-gpt-1.2.8/setup.py
+drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-05-25 14:31:53.146066 knowledgebase-gsheet-gpt-1.2.9/
+-rw-r--r--   0 chiubowen   (501) staff       (20)     1658 2023-05-25 14:31:53.145954 knowledgebase-gsheet-gpt-1.2.9/PKG-INFO
+-rw-r--r--   0 chiubowen   (501) staff       (20)     1476 2023-05-25 14:31:52.000000 knowledgebase-gsheet-gpt-1.2.9/README.md
+drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-05-25 14:31:53.145769 knowledgebase-gsheet-gpt-1.2.9/knowledgebase_gsheet_gpt.egg-info/
+-rw-r--r--   0 chiubowen   (501) staff       (20)     1658 2023-05-25 14:31:53.000000 knowledgebase-gsheet-gpt-1.2.9/knowledgebase_gsheet_gpt.egg-info/PKG-INFO
+-rw-r--r--   0 chiubowen   (501) staff       (20)      336 2023-05-25 14:31:53.000000 knowledgebase-gsheet-gpt-1.2.9/knowledgebase_gsheet_gpt.egg-info/SOURCES.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)        1 2023-05-25 14:31:53.000000 knowledgebase-gsheet-gpt-1.2.9/knowledgebase_gsheet_gpt.egg-info/dependency_links.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)       76 2023-05-25 14:31:53.000000 knowledgebase-gsheet-gpt-1.2.9/knowledgebase_gsheet_gpt.egg-info/entry_points.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)      112 2023-05-25 14:31:53.000000 knowledgebase-gsheet-gpt-1.2.9/knowledgebase_gsheet_gpt.egg-info/requires.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)       25 2023-05-25 14:31:53.000000 knowledgebase-gsheet-gpt-1.2.9/knowledgebase_gsheet_gpt.egg-info/top_level.txt
+-rwxr-xr-x   0 chiubowen   (501) staff       (20)     6170 2023-05-25 14:31:52.000000 knowledgebase-gsheet-gpt-1.2.9/knowledgebase_gsheet_gpt.py
+-rw-r--r--   0 chiubowen   (501) staff       (20)       38 2023-05-25 14:31:53.146103 knowledgebase-gsheet-gpt-1.2.9/setup.cfg
+-rw-r--r--   0 chiubowen   (501) staff       (20)      560 2023-05-25 14:31:52.000000 knowledgebase-gsheet-gpt-1.2.9/setup.py
```

### Comparing `knowledgebase-gsheet-gpt-1.2.8/PKG-INFO` & `knowledgebase-gsheet-gpt-1.2.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: knowledgebase-gsheet-gpt
-Version: 1.2.8
+Version: 1.2.9
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # Knowledgebase GSheet GPT
```

### Comparing `knowledgebase-gsheet-gpt-1.2.8/README.md` & `knowledgebase-gsheet-gpt-1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `knowledgebase-gsheet-gpt-1.2.8/knowledgebase_gsheet_gpt.egg-info/PKG-INFO` & `knowledgebase-gsheet-gpt-1.2.9/knowledgebase_gsheet_gpt.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: knowledgebase-gsheet-gpt
-Version: 1.2.8
+Version: 1.2.9
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # Knowledgebase GSheet GPT
```

### Comparing `knowledgebase-gsheet-gpt-1.2.8/knowledgebase_gsheet_gpt.py` & `knowledgebase-gsheet-gpt-1.2.9/knowledgebase_gsheet_gpt.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 #!/usr/bin/env python
 # knowledgebase_gsheet_gpt.py
 import argparse
 import os
 
-from time import time
-
 import csv_embeddings_creator
 import google_sheet_downloader
 import openai_chat_thread
 import similarity_ranker
 
 DEFAULT_BEFORE_QUESTION_PROMPT = '\n-- the user question\n'
 DEFAULT_BEFORE_KNOWLEDGE_PROMPT = '\n-- reference following knowledge base content to answer the user question (answer as long as possible)\n'
```

### Comparing `knowledgebase-gsheet-gpt-1.2.8/setup.py` & `knowledgebase-gsheet-gpt-1.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt') as f:
     requirements = [line.strip() for line in f.readlines()]
 
 setup(
     name="knowledgebase-gsheet-gpt",
-    version="1.2.8",
+    version="1.2.9",
     packages=find_packages(),
     py_modules=['knowledgebase_gsheet_gpt'],
     install_requires=requirements,
     entry_points={
         'console_scripts': [
             'knowledgebase_gsheet_gpt = knowledgebase_gsheet_gpt:main',
         ],
```

