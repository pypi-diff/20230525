# Comparing `tmp/amazon-textract-response-parser-0.1.8.tar.gz` & `tmp/amazon-textract-response-parser-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/amazon-textract-response-parser-0.1.8.tar", last modified: Fri Apr 30 18:14:22 2021, max compression
+gzip compressed data, was "dist/amazon-textract-response-parser-0.1.9.tar", last modified: Fri Apr 30 20:38:01 2021, max compression
```

## Comparing `amazon-textract-response-parser-0.1.8.tar` & `amazon-textract-response-parser-0.1.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 schadem  (1964830885) staff       (20)        0 2021-04-30 18:14:22.536130 amazon-textract-response-parser-0.1.8/
--rw-r--r--   0 schadem  (1964830885) staff       (20)     8474 2021-04-30 18:14:22.536432 amazon-textract-response-parser-0.1.8/PKG-INFO
--rw-r--r--   0 schadem  (1964830885) staff       (20)     6148 2021-04-30 16:54:10.000000 amazon-textract-response-parser-0.1.8/README.md
-drwxr-xr-x   0 schadem  (1964830885) staff       (20)        0 2021-04-30 18:14:22.527640 amazon-textract-response-parser-0.1.8/a2i/
--rw-r--r--   0 schadem  (1964830885) staff       (20)      108 2021-04-30 18:13:58.000000 amazon-textract-response-parser-0.1.8/a2i/__init__.py
--rw-r--r--   0 schadem  (1964830885) staff       (20)     7188 2020-12-17 00:30:39.000000 amazon-textract-response-parser-0.1.8/a2i/a2irp.py
--rw-r--r--   0 schadem  (1964830885) staff       (20)     1355 2020-12-17 00:30:39.000000 amazon-textract-response-parser-0.1.8/a2i/a2irptest.py
-drwxr-xr-x   0 schadem  (1964830885) staff       (20)        0 2021-04-30 18:14:22.531186 amazon-textract-response-parser-0.1.8/amazon_textract_response_parser.egg-info/
--rw-r--r--   0 schadem  (1964830885) staff       (20)     8474 2021-04-30 18:14:22.000000 amazon-textract-response-parser-0.1.8/amazon_textract_response_parser.egg-info/PKG-INFO
--rw-r--r--   0 schadem  (1964830885) staff       (20)      423 2021-04-30 18:14:22.000000 amazon-textract-response-parser-0.1.8/amazon_textract_response_parser.egg-info/SOURCES.txt
--rw-r--r--   0 schadem  (1964830885) staff       (20)        1 2021-04-30 18:14:22.000000 amazon-textract-response-parser-0.1.8/amazon_textract_response_parser.egg-info/dependency_links.txt
--rw-r--r--   0 schadem  (1964830885) staff       (20)       26 2021-04-30 18:14:22.000000 amazon-textract-response-parser-0.1.8/amazon_textract_response_parser.egg-info/requires.txt
--rw-r--r--   0 schadem  (1964830885) staff       (20)        8 2021-04-30 18:14:22.000000 amazon-textract-response-parser-0.1.8/amazon_textract_response_parser.egg-info/top_level.txt
-drwxr-xr-x   0 schadem  (1964830885) staff       (20)        0 2021-04-30 18:14:22.531919 amazon-textract-response-parser-0.1.8/bin/
--rw-r--r--   0 schadem  (1964830885) staff       (20)      920 2021-04-30 18:05:03.000000 amazon-textract-response-parser-0.1.8/bin/amazon-textract-pipeline
--rw-r--r--   0 schadem  (1964830885) staff       (20)      505 2021-04-30 18:14:22.537547 amazon-textract-response-parser-0.1.8/setup.cfg
--rw-r--r--   0 schadem  (1964830885) staff       (20)     1874 2021-04-30 18:13:58.000000 amazon-textract-response-parser-0.1.8/setup.py
-drwxr-xr-x   0 schadem  (1964830885) staff       (20)        0 2021-04-30 18:14:22.535527 amazon-textract-response-parser-0.1.8/trp/
--rw-r--r--   0 schadem  (1964830885) staff       (20)    15507 2021-04-30 18:13:58.000000 amazon-textract-response-parser-0.1.8/trp/__init__.py
--rw-r--r--   0 schadem  (1964830885) staff       (20)     1574 2021-04-29 15:28:03.000000 amazon-textract-response-parser-0.1.8/trp/t_pipeline.py
--rw-r--r--   0 schadem  (1964830885) staff       (20)    19506 2021-04-30 16:27:39.000000 amazon-textract-response-parser-0.1.8/trp/trp2.py
+drwxr-xr-x   0 schadem  (1964830885) staff       (20)        0 2021-04-30 20:38:01.172180 amazon-textract-response-parser-0.1.9/
+-rw-r--r--   0 schadem  (1964830885) staff       (20)     8474 2021-04-30 20:38:01.172477 amazon-textract-response-parser-0.1.9/PKG-INFO
+-rw-r--r--   0 schadem  (1964830885) staff       (20)     6148 2021-04-30 16:54:10.000000 amazon-textract-response-parser-0.1.9/README.md
+drwxr-xr-x   0 schadem  (1964830885) staff       (20)        0 2021-04-30 20:38:01.165054 amazon-textract-response-parser-0.1.9/a2i/
+-rw-r--r--   0 schadem  (1964830885) staff       (20)      108 2021-04-30 20:34:27.000000 amazon-textract-response-parser-0.1.9/a2i/__init__.py
+-rw-r--r--   0 schadem  (1964830885) staff       (20)     7188 2020-12-17 00:30:39.000000 amazon-textract-response-parser-0.1.9/a2i/a2irp.py
+-rw-r--r--   0 schadem  (1964830885) staff       (20)     1355 2020-12-17 00:30:39.000000 amazon-textract-response-parser-0.1.9/a2i/a2irptest.py
+drwxr-xr-x   0 schadem  (1964830885) staff       (20)        0 2021-04-30 20:38:01.168402 amazon-textract-response-parser-0.1.9/amazon_textract_response_parser.egg-info/
+-rw-r--r--   0 schadem  (1964830885) staff       (20)     8474 2021-04-30 20:38:00.000000 amazon-textract-response-parser-0.1.9/amazon_textract_response_parser.egg-info/PKG-INFO
+-rw-r--r--   0 schadem  (1964830885) staff       (20)      423 2021-04-30 20:38:00.000000 amazon-textract-response-parser-0.1.9/amazon_textract_response_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 schadem  (1964830885) staff       (20)        1 2021-04-30 20:38:00.000000 amazon-textract-response-parser-0.1.9/amazon_textract_response_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 schadem  (1964830885) staff       (20)       26 2021-04-30 20:38:00.000000 amazon-textract-response-parser-0.1.9/amazon_textract_response_parser.egg-info/requires.txt
+-rw-r--r--   0 schadem  (1964830885) staff       (20)        8 2021-04-30 20:38:00.000000 amazon-textract-response-parser-0.1.9/amazon_textract_response_parser.egg-info/top_level.txt
+drwxr-xr-x   0 schadem  (1964830885) staff       (20)        0 2021-04-30 20:38:01.169117 amazon-textract-response-parser-0.1.9/bin/
+-rwxr-xr-x   0 schadem  (1964830885) staff       (20)     1175 2021-04-30 20:32:03.000000 amazon-textract-response-parser-0.1.9/bin/amazon-textract-pipeline
+-rw-r--r--   0 schadem  (1964830885) staff       (20)      505 2021-04-30 20:38:01.173522 amazon-textract-response-parser-0.1.9/setup.cfg
+-rw-r--r--   0 schadem  (1964830885) staff       (20)     1874 2021-04-30 20:34:27.000000 amazon-textract-response-parser-0.1.9/setup.py
+drwxr-xr-x   0 schadem  (1964830885) staff       (20)        0 2021-04-30 20:38:01.171014 amazon-textract-response-parser-0.1.9/trp/
+-rw-r--r--   0 schadem  (1964830885) staff       (20)    15507 2021-04-30 20:34:27.000000 amazon-textract-response-parser-0.1.9/trp/__init__.py
+-rw-r--r--   0 schadem  (1964830885) staff       (20)     1574 2021-04-29 15:28:03.000000 amazon-textract-response-parser-0.1.9/trp/t_pipeline.py
+-rw-r--r--   0 schadem  (1964830885) staff       (20)    19506 2021-04-30 16:27:39.000000 amazon-textract-response-parser-0.1.9/trp/trp2.py
```

### Comparing `amazon-textract-response-parser-0.1.8/PKG-INFO` & `amazon-textract-response-parser-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amazon-textract-response-parser
-Version: 0.1.8
+Version: 0.1.9
 Summary: Easily parse JSON returned by Amazon Textract.
 Home-page: https://github.com/aws-samples/amazon-textract-response-parser
 Author: Amazon Rekognition Textract Demoes
 Author-email: rekognition-textract-demos@amazon.com
 License: Apache License Version 2.0
 Description: # Textract Response Parser
```

### Comparing `amazon-textract-response-parser-0.1.8/README.md` & `amazon-textract-response-parser-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `amazon-textract-response-parser-0.1.8/a2i/a2irp.py` & `amazon-textract-response-parser-0.1.9/a2i/a2irp.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-response-parser-0.1.8/a2i/a2irptest.py` & `amazon-textract-response-parser-0.1.9/a2i/a2irptest.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-response-parser-0.1.8/amazon_textract_response_parser.egg-info/PKG-INFO` & `amazon-textract-response-parser-0.1.9/amazon_textract_response_parser.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amazon-textract-response-parser
-Version: 0.1.8
+Version: 0.1.9
 Summary: Easily parse JSON returned by Amazon Textract.
 Home-page: https://github.com/aws-samples/amazon-textract-response-parser
 Author: Amazon Rekognition Textract Demoes
 Author-email: rekognition-textract-demos@amazon.com
 License: Apache License Version 2.0
 Description: # Textract Response Parser
```

### Comparing `amazon-textract-response-parser-0.1.8/bin/amazon-textract-pipeline` & `amazon-textract-response-parser-0.1.9/bin/amazon-textract-pipeline`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,31 @@
+#!/usr/bin/env python
+
 import json
 import sys
 from trp.trp2 import TDocumentSchema
 from trp.t_pipeline import order_blocks_by_geo, add_page_orientation
 import argparse
+from trp import __version__
 from enum import Enum, auto
 
 class TPipelineComponents(Enum):
     order_blocks_by_geo = auto()
     add_page_orientation = auto()
 
 
 
 
 parser = argparse.ArgumentParser()
 parser.add_argument("--components", nargs='+', choices=[TPipelineComponents.add_page_orientation.name, TPipelineComponents.order_blocks_by_geo.name], help="define which components to call", required=True)
+parser.add_argument("--version",
+                    action='version',
+                    version='%(prog)s {version}'.format(version=__version__),
+                    help="print version information")
+
 
 args = parser.parse_args()
 components = [TPipelineComponents[x] for x in args.components]
 
 
 doc_json = json.load(sys.stdin)
 t_doc = TDocumentSchema().load(doc_json)
```

### Comparing `amazon-textract-response-parser-0.1.8/setup.py` & `amazon-textract-response-parser-0.1.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     os.system('twine check dist/*')
     os.system('twine upload --repository pypi dist/*')
     sys.exit()
 
 setup(
     name='amazon-textract-response-parser',
     packages=['trp', 'a2i'],
-    version='0.1.8',
+    version='0.1.9',
     description='Easily parse JSON returned by Amazon Textract.',
     install_requires=requirements,
     scripts=['bin/amazon-textract-pipeline'],
     long_description_content_type='text/markdown',
     long_description=read('README.md'),
     author='Amazon Rekognition Textract Demoes',
     author_email='rekognition-textract-demos@amazon.com',
```

### Comparing `amazon-textract-response-parser-0.1.8/trp/__init__.py` & `amazon-textract-response-parser-0.1.9/trp/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import logging
 from logging import NullHandler
 
 logging.getLogger(__name__).addHandler(NullHandler())
 
 logger = logging.getLogger(__name__)
 
-__version__ = '0.1.8'
+__version__ = '0.1.9'
 
 class BaseBlock():
     def __init__(self, block, blockMap):
         self._block = block
         self._confidence = block['Confidence']
         self._geometry = Geometry(block['Geometry'])
         self._id = block['Id']
```

### Comparing `amazon-textract-response-parser-0.1.8/trp/t_pipeline.py` & `amazon-textract-response-parser-0.1.9/trp/t_pipeline.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-response-parser-0.1.8/trp/trp2.py` & `amazon-textract-response-parser-0.1.9/trp/trp2.py`

 * *Files identical despite different names*

