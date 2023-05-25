# Comparing `tmp/csv-embeddings-creator-1.0.6.tar.gz` & `tmp/csv-embeddings-creator-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csv-embeddings-creator-1.0.6.tar", last modified: Wed May 24 06:48:07 2023, max compression
+gzip compressed data, was "csv-embeddings-creator-1.0.7.tar", last modified: Thu May 25 14:30:34 2023, max compression
```

## Comparing `csv-embeddings-creator-1.0.6.tar` & `csv-embeddings-creator-1.0.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-05-24 06:48:07.161478 csv-embeddings-creator-1.0.6/
--rw-r--r--   0 chiubowen   (501) staff       (20)     3136 2023-05-24 06:48:07.161357 csv-embeddings-creator-1.0.6/PKG-INFO
--rw-r--r--   0 chiubowen   (501) staff       (20)     2956 2023-05-24 06:48:07.000000 csv-embeddings-creator-1.0.6/README.md
-drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-05-24 06:48:07.161180 csv-embeddings-creator-1.0.6/csv_embeddings_creator.egg-info/
--rw-r--r--   0 chiubowen   (501) staff       (20)     3136 2023-05-24 06:48:07.000000 csv-embeddings-creator-1.0.6/csv_embeddings_creator.egg-info/PKG-INFO
--rw-r--r--   0 chiubowen   (501) staff       (20)      322 2023-05-24 06:48:07.000000 csv-embeddings-creator-1.0.6/csv_embeddings_creator.egg-info/SOURCES.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)        1 2023-05-24 06:48:07.000000 csv-embeddings-creator-1.0.6/csv_embeddings_creator.egg-info/dependency_links.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)       72 2023-05-24 06:48:07.000000 csv-embeddings-creator-1.0.6/csv_embeddings_creator.egg-info/entry_points.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)       37 2023-05-24 06:48:07.000000 csv-embeddings-creator-1.0.6/csv_embeddings_creator.egg-info/requires.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)       23 2023-05-24 06:48:07.000000 csv-embeddings-creator-1.0.6/csv_embeddings_creator.egg-info/top_level.txt
--rwxr-xr-x   0 chiubowen   (501) staff       (20)     3058 2023-05-24 06:48:07.000000 csv-embeddings-creator-1.0.6/csv_embeddings_creator.py
--rw-r--r--   0 chiubowen   (501) staff       (20)       38 2023-05-24 06:48:07.161518 csv-embeddings-creator-1.0.6/setup.cfg
--rw-r--r--   0 chiubowen   (501) staff       (20)      552 2023-05-24 06:48:07.000000 csv-embeddings-creator-1.0.6/setup.py
+drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-05-25 14:30:34.639886 csv-embeddings-creator-1.0.7/
+-rw-r--r--   0 chiubowen   (501) staff       (20)     3136 2023-05-25 14:30:34.639776 csv-embeddings-creator-1.0.7/PKG-INFO
+-rw-r--r--   0 chiubowen   (501) staff       (20)     2956 2023-05-25 14:30:34.000000 csv-embeddings-creator-1.0.7/README.md
+drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-05-25 14:30:34.639603 csv-embeddings-creator-1.0.7/csv_embeddings_creator.egg-info/
+-rw-r--r--   0 chiubowen   (501) staff       (20)     3136 2023-05-25 14:30:34.000000 csv-embeddings-creator-1.0.7/csv_embeddings_creator.egg-info/PKG-INFO
+-rw-r--r--   0 chiubowen   (501) staff       (20)      322 2023-05-25 14:30:34.000000 csv-embeddings-creator-1.0.7/csv_embeddings_creator.egg-info/SOURCES.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)        1 2023-05-25 14:30:34.000000 csv-embeddings-creator-1.0.7/csv_embeddings_creator.egg-info/dependency_links.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)       72 2023-05-25 14:30:34.000000 csv-embeddings-creator-1.0.7/csv_embeddings_creator.egg-info/entry_points.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)       37 2023-05-25 14:30:34.000000 csv-embeddings-creator-1.0.7/csv_embeddings_creator.egg-info/requires.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)       23 2023-05-25 14:30:34.000000 csv-embeddings-creator-1.0.7/csv_embeddings_creator.egg-info/top_level.txt
+-rwxr-xr-x   0 chiubowen   (501) staff       (20)     3220 2023-05-25 14:30:34.000000 csv-embeddings-creator-1.0.7/csv_embeddings_creator.py
+-rw-r--r--   0 chiubowen   (501) staff       (20)       38 2023-05-25 14:30:34.639920 csv-embeddings-creator-1.0.7/setup.cfg
+-rw-r--r--   0 chiubowen   (501) staff       (20)      552 2023-05-25 14:30:34.000000 csv-embeddings-creator-1.0.7/setup.py
```

### Comparing `csv-embeddings-creator-1.0.6/PKG-INFO` & `csv-embeddings-creator-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csv-embeddings-creator
-Version: 1.0.6
+Version: 1.0.7
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # csv_embeddings_creator v1.0.4 by Bowen Chiu
```

### Comparing `csv-embeddings-creator-1.0.6/README.md` & `csv-embeddings-creator-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `csv-embeddings-creator-1.0.6/csv_embeddings_creator.egg-info/PKG-INFO` & `csv-embeddings-creator-1.0.7/csv_embeddings_creator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csv-embeddings-creator
-Version: 1.0.6
+Version: 1.0.7
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # csv_embeddings_creator v1.0.4 by Bowen Chiu
```

### Comparing `csv-embeddings-creator-1.0.6/csv_embeddings_creator.py` & `csv-embeddings-creator-1.0.7/csv_embeddings_creator.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,62 +1,66 @@
 #!/usr/bin/env python
 # csv_embeddings_creator.py
 import argparse
 import csv
 import glob
 import os
 import re
+from time import time
+
 import torch
 from sentence_transformers import SentenceTransformer
 
 
 def create_embeddings(input_folder, output_txt_folder, output_embeddings_folder, force=False):
     model = SentenceTransformer('paraphrase-multilingual-MiniLM-L12-v2')
 
     os.makedirs(output_txt_folder, exist_ok=True)
     os.makedirs(output_embeddings_folder, exist_ok=True)
 
     csv_files = glob.glob(os.path.join(input_folder, '**/*.csv'), recursive=True)
     embedding_files = glob.glob(os.path.join(output_embeddings_folder, '**/*.pt'), recursive=True)
 
-    # 跳過已經做完的
     dic_doc_id = {}
     for path in embedding_files:
-        doc_id = re.findall('doc-id_(.*?)_sha', path)[0]
-        dic_doc_id[doc_id] = True
+        matches = re.findall('doc-id_(.*?)_sha', path)
+        if matches:
+            doc_id = matches[0]
+            dic_doc_id[doc_id] = True
 
     i = 0
     for csv_file in csv_files:
-        doc_id = re.findall('doc-id_(.*?)_sha', csv_file)[0]
-        if doc_id in dic_doc_id:
-            continue
+        matches = re.findall('doc-id_(.*?)_sha', path)
+        if matches:
+            doc_id = matches[0]
+            if doc_id in dic_doc_id:
+                continue
 
         file_base_name = os.path.splitext(os.path.basename(csv_file))[0]
         existing_txt_files = glob.glob(os.path.join(output_txt_folder, f"{file_base_name}_*.txt"))
 
         if not force and existing_txt_files:
             continue
 
         with open(csv_file, 'r', encoding='utf-8') as f:
             reader = csv.reader(f)
-            next(reader)  # Skip header
-
             for idx, row in enumerate(reader):
+                t = time()
                 i += 1
                 folder_txt = os.path.join(output_txt_folder, f"{file_base_name}")
                 os.makedirs(folder_txt, exist_ok=True)
                 txt_file = os.path.join(folder_txt, f"{file_base_name}_{idx + 1}.txt")
                 with open(txt_file, 'w', encoding='utf-8') as txt_f:
                     txt_f.write('"' + '","'.join(row) + '"')
-
                 embeddings = model.encode('"' + '","'.join(row) + '"')
                 folder_embeddings = os.path.join(output_embeddings_folder, f"{file_base_name}")
                 os.makedirs(folder_embeddings, exist_ok=True)
                 embeddings_file = os.path.join(folder_embeddings, f"{file_base_name}_{idx + 1}.pt")
                 torch.save(embeddings, embeddings_file)
+                print('csv_embeddings_creator.py,i,time:', i, time() - t)
 
 
 def parse_arguments():
     parser = argparse.ArgumentParser(description='Create embeddings for text files using Hugging Face Transformers.')
     parser.add_argument('--input-folder', type=str, required=True,
                         help='Input folder containing CSV files')
     parser.add_argument('--output-txt-folder', type=str, required=True,
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `csv-embeddings-creator-1.0.6/setup.py` & `csv-embeddings-creator-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt') as f:
     requirements = [line.strip() for line in f.readlines()]
 
 setup(
     name="csv-embeddings-creator",
-    version="1.0.6",
+    version="1.0.7",
     packages=find_packages(),
     py_modules=['csv_embeddings_creator'],
     install_requires=requirements,
     entry_points={
         'console_scripts': [
             'csv_embeddings_creator = csv_embeddings_creator:main',
         ],
```

