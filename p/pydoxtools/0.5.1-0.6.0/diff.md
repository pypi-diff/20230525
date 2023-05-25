# Comparing `tmp/pydoxtools-0.5.1.tar.gz` & `tmp/pydoxtools-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydoxtools-0.5.1.tar", max compression
+gzip compressed data, was "pydoxtools-0.6.0.tar", max compression
```

## Comparing `pydoxtools-0.5.1.tar` & `pydoxtools-0.6.0.tar`

### file list

```diff
@@ -1,38 +1,42 @@
--rw-r--r--   0        0        0     1072 2022-11-13 06:52:05.633039 pydoxtools-0.5.1/LICENSE
--rw-r--r--   0        0        0     7184 2023-04-30 16:24:58.954881 pydoxtools-0.5.1/README.md
--rw-r--r--   0        0        0      179 2023-05-01 00:24:50.651336 pydoxtools-0.5.1/pydoxtools/__init__.py
--rw-r--r--   0        0        0     2508 2022-06-29 18:27:36.743357 pydoxtools-0.5.1/pydoxtools/class_utils.py
--rwxr-xr-x   0        0        0    30578 2023-04-28 07:35:46.790006 pydoxtools-0.5.1/pydoxtools/classifier.py
--rw-r--r--   0        0        0    29431 2022-11-13 06:52:05.609037 pydoxtools-0.5.1/pydoxtools/cluster_utils.py
--rw-r--r--   0        0        0    28848 2023-05-01 00:12:52.179681 pydoxtools-0.5.1/pydoxtools/document.py
--rw-r--r--   0        0        0    26940 2023-05-01 00:09:33.425312 pydoxtools-0.5.1/pydoxtools/document_base.py
--rw-r--r--   0        0        0     1664 2023-04-28 23:18:54.122413 pydoxtools-0.5.1/pydoxtools/extract_classes.py
--rw-r--r--   0        0        0     2586 2023-05-01 00:12:52.179681 pydoxtools-0.5.1/pydoxtools/extract_filesystem.py
--rw-r--r--   0        0        0    13332 2023-04-28 23:18:54.122413 pydoxtools-0.5.1/pydoxtools/extract_html.py
--rw-r--r--   0        0        0     7305 2023-04-30 00:35:06.851296 pydoxtools-0.5.1/pydoxtools/extract_index.py
--rw-r--r--   0        0        0     2261 2023-04-30 20:11:24.899459 pydoxtools-0.5.1/pydoxtools/extract_nlpchat.py
--rw-r--r--   0        0        0     2081 2023-04-28 23:18:54.122413 pydoxtools-0.5.1/pydoxtools/extract_objects.py
--rw-r--r--   0        0        0     1494 2023-04-28 23:18:54.122413 pydoxtools-0.5.1/pydoxtools/extract_ocr.py
--rw-r--r--   0        0        0     4773 2023-04-30 16:24:58.954881 pydoxtools-0.5.1/pydoxtools/extract_pandoc.py
--rw-r--r--   0        0        0     5539 2023-04-28 23:18:54.126413 pydoxtools-0.5.1/pydoxtools/extract_spacy.py
--rw-r--r--   0        0        0    43212 2023-05-01 00:09:33.425312 pydoxtools-0.5.1/pydoxtools/extract_tables.py
--rw-r--r--   0        0        0     7473 2023-04-28 23:18:54.126413 pydoxtools-0.5.1/pydoxtools/extract_textstructure.py
--rw-r--r--   0        0        0     1232 2023-04-27 18:19:20.092916 pydoxtools-0.5.1/pydoxtools/file_utils.py
--rwxr-xr-x   0        0        0     6143 2022-11-13 06:52:05.613038 pydoxtools-0.5.1/pydoxtools/html_utils.py
--rw-r--r--   0        0        0      150 2022-06-29 18:27:36.743357 pydoxtools-0.5.1/pydoxtools/initialize_library.py
--rw-r--r--   0        0        0     7077 2022-11-13 06:52:05.613038 pydoxtools-0.5.1/pydoxtools/labeling.py
--rw-r--r--   0        0        0     6972 2023-04-29 23:54:56.248127 pydoxtools-0.5.1/pydoxtools/list_utils.py
--rw-r--r--   0        0        0      371 2022-11-13 06:52:05.613038 pydoxtools-0.5.1/pydoxtools/math_utils.py
--rw-r--r--   0        0        0     2431 2022-11-13 06:52:05.613038 pydoxtools-0.5.1/pydoxtools/models.py
--rwxr-xr-x   0        0        0    21372 2023-04-30 16:24:58.954881 pydoxtools-0.5.1/pydoxtools/nlp_utils.py
--rw-r--r--   0        0        0     2502 2022-06-29 18:27:36.747357 pydoxtools-0.5.1/pydoxtools/ocr_language_mappings.py
--rw-r--r--   0        0        0     8886 2023-04-30 16:24:58.954881 pydoxtools-0.5.1/pydoxtools/operator_huggingface.py
--rw-r--r--   0        0        0     8098 2023-05-01 00:09:33.425312 pydoxtools-0.5.1/pydoxtools/operators.py
--rwxr-xr-x   0        0        0    12103 2023-04-28 23:18:54.126413 pydoxtools-0.5.1/pydoxtools/pdf_utils.py
--rw-r--r--   0        0        0    34126 2023-03-26 07:49:32.670915 pydoxtools-0.5.1/pydoxtools/random_data_generators.py
--rwxr-xr-x   0        0        0     1679 2023-04-28 23:18:54.126413 pydoxtools-0.5.1/pydoxtools/settings.py
--rw-r--r--   0        0        0    17730 2023-04-22 06:12:25.093623 pydoxtools-0.5.1/pydoxtools/training.py
--rw-r--r--   0        0        0     3898 2022-06-29 18:27:36.747357 pydoxtools-0.5.1/pydoxtools/visual_document_analysis.py
--rw-r--r--   0        0        0     3209 2023-01-02 07:05:17.767492 pydoxtools-0.5.1/pydoxtools/webdav_utils.py
--rw-r--r--   0        0        0     5744 2023-05-01 00:26:12.181393 pydoxtools-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     9798 1970-01-01 00:00:00.000000 pydoxtools-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-01-19 05:32:50.265107 pydoxtools-0.6.0/LICENSE
+-rw-r--r--   0        0        0     8260 2023-05-25 01:08:00.818589 pydoxtools-0.6.0/README.md
+-rw-r--r--   0        0        0      258 2023-05-25 06:20:55.635381 pydoxtools-0.6.0/pydoxtools/__init__.py
+-rw-r--r--   0        0        0    11153 2023-05-25 00:15:16.561311 pydoxtools-0.6.0/pydoxtools/agent.py
+-rw-r--r--   0        0        0     2508 2022-02-09 15:52:43.898218 pydoxtools-0.6.0/pydoxtools/class_utils.py
+-rwxr-xr-x   0        0        0    30541 2023-05-09 05:49:37.140825 pydoxtools-0.6.0/pydoxtools/classifier.py
+-rw-r--r--   0        0        0    29431 2022-11-12 20:39:33.790453 pydoxtools-0.6.0/pydoxtools/cluster_utils.py
+-rw-r--r--   0        0        0     6047 2023-05-25 01:00:13.344389 pydoxtools-0.6.0/pydoxtools/dask_operators.py
+-rw-r--r--   0        0        0    53220 2023-05-24 17:14:40.070633 pydoxtools-0.6.0/pydoxtools/document.py
+-rw-r--r--   0        0        0    35071 2023-05-24 00:02:05.489329 pydoxtools-0.6.0/pydoxtools/document_base.py
+-rw-r--r--   0        0        0     1673 2023-05-09 23:54:11.246379 pydoxtools-0.6.0/pydoxtools/extract_classes.py
+-rw-r--r--   0        0        0        3 2023-05-02 20:33:41.756428 pydoxtools-0.6.0/pydoxtools/extract_db.py
+-rw-r--r--   0        0        0     3978 2023-05-23 19:28:54.538602 pydoxtools-0.6.0/pydoxtools/extract_filesystem.py
+-rw-r--r--   0        0        0    13329 2023-05-09 23:54:11.178377 pydoxtools-0.6.0/pydoxtools/extract_html.py
+-rw-r--r--   0        0        0    12396 2023-05-25 06:02:49.144053 pydoxtools-0.6.0/pydoxtools/extract_index.py
+-rw-r--r--   0        0        0     3177 2023-05-20 06:10:12.179526 pydoxtools-0.6.0/pydoxtools/extract_nlpchat.py
+-rw-r--r--   0        0        0     2469 2023-05-09 23:54:11.186378 pydoxtools-0.6.0/pydoxtools/extract_objects.py
+-rw-r--r--   0        0        0     1656 2023-05-10 07:01:17.768739 pydoxtools-0.6.0/pydoxtools/extract_ocr.py
+-rw-r--r--   0        0        0     6469 2023-05-23 19:52:11.543694 pydoxtools-0.6.0/pydoxtools/extract_pandoc.py
+-rw-r--r--   0        0        0     5544 2023-05-09 23:54:11.270379 pydoxtools-0.6.0/pydoxtools/extract_spacy.py
+-rw-r--r--   0        0        0    43269 2023-05-20 05:43:43.697769 pydoxtools-0.6.0/pydoxtools/extract_tables.py
+-rw-r--r--   0        0        0     8139 2023-05-09 23:54:11.150377 pydoxtools-0.6.0/pydoxtools/extract_textstructure.py
+-rw-r--r--   0        0        0     1232 2023-04-26 22:02:00.116297 pydoxtools-0.6.0/pydoxtools/file_utils.py
+-rwxr-xr-x   0        0        0     6143 2022-11-12 20:39:33.794453 pydoxtools-0.6.0/pydoxtools/html_utils.py
+-rw-r--r--   0        0        0      150 2022-02-09 15:52:43.898218 pydoxtools-0.6.0/pydoxtools/initialize_library.py
+-rw-r--r--   0        0        0     7077 2022-11-12 20:39:33.794453 pydoxtools-0.6.0/pydoxtools/labeling.py
+-rw-r--r--   0        0        0     7364 2023-05-18 23:05:10.290935 pydoxtools-0.6.0/pydoxtools/list_utils.py
+-rw-r--r--   0        0        0      371 2022-11-12 20:39:33.794453 pydoxtools-0.6.0/pydoxtools/math_utils.py
+-rw-r--r--   0        0        0     2431 2022-11-12 20:39:33.794453 pydoxtools-0.6.0/pydoxtools/models.py
+-rwxr-xr-x   0        0        0    18776 2023-05-06 19:40:13.998671 pydoxtools-0.6.0/pydoxtools/nlp_utils.py
+-rw-r--r--   0        0        0     2502 2022-03-30 10:01:09.241031 pydoxtools-0.6.0/pydoxtools/ocr_language_mappings.py
+-rw-r--r--   0        0        0     8897 2023-05-09 23:54:11.158377 pydoxtools-0.6.0/pydoxtools/operator_huggingface.py
+-rw-r--r--   0        0        0     1137 2023-05-14 18:22:46.918667 pydoxtools-0.6.0/pydoxtools/operators.py
+-rw-r--r--   0        0        0     7856 2023-05-22 06:53:09.989310 pydoxtools-0.6.0/pydoxtools/operators_base.py
+-rwxr-xr-x   0        0        0    12146 2023-05-09 23:54:11.106376 pydoxtools-0.6.0/pydoxtools/pdf_utils.py
+-rw-r--r--   0        0        0    34126 2023-03-28 06:51:36.920970 pydoxtools-0.6.0/pydoxtools/random_data_generators.py
+-rwxr-xr-x   0        0        0     1332 2023-05-11 04:47:15.118352 pydoxtools-0.6.0/pydoxtools/settings.py
+-rw-r--r--   0        0        0    17693 2023-05-09 05:49:37.108824 pydoxtools-0.6.0/pydoxtools/training.py
+-rw-r--r--   0        0        0     3898 2022-02-09 15:52:43.898218 pydoxtools-0.6.0/pydoxtools/visual_document_analysis.py
+-rw-r--r--   0        0        0     3209 2023-01-19 05:32:50.269106 pydoxtools-0.6.0/pydoxtools/webdav_utils.py
+-rw-r--r--   0        0        0     5950 2023-05-25 06:30:37.837691 pydoxtools-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0    11122 1970-01-01 00:00:00.000000 pydoxtools-0.6.0/PKG-INFO
```

### Comparing `pydoxtools-0.5.1/LICENSE` & `pydoxtools-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydoxtools-0.5.1/README.md` & `pydoxtools-0.6.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-🚀 pydoxtools (Python Library) 🚀
+🎩✨📄 pydoxtools (Python Library) 🎩✨📄
 ================================================================================
 
 ![Python](https://img.shields.io/pypi/pyversions/pydoxtools.svg)
 [![PyPI version](https://img.shields.io/pypi/v/pydoxtools.svg)](https://pypi.python.org/pypi/pydoxtools)
 [![Mkdocs](https://img.shields.io/badge/doc-mkdocs-845ed7.svg)](https://pydoxtools.xyntopia.com)
 [![GitHub discussions](https://img.shields.io/badge/discuss-online-845ef7)](https://github.com/xyntopia/pydoxtools/discussions)
 [![GitHub stars](https://img.shields.io/github/stars/xyntopia/pydoxtools)](https://github.com/xyntopia/pydoxtools/stargazers)
@@ -11,148 +11,171 @@
 
 (*WIP*) [Documentation](https://pydoxtools.xyntopia.com)
 
 Pydoxtools is a library that provides a sophisticated interface for reading and
 writing documents, designed to work with AI models such as GPT, Alpaca, and
 Huggingface. It offers functionalities such as:
 
-- Table extraction
-- Vector Index Creation
+- Pipeline management
+- Integration with AI (LLMs and more) models
+- low-resource (PDF) table extraction without configuration and expensive
+  layout detection algorithms!
 - Document analysis and question-answering
+- Support for most of todays document formats
+- Vector index Creation
 - Entity, address identification and more
 - List and keyword extraction
 - Data normalization, translation, and cleaning
 
 The library allows for the creation of complex extraction pipelines
 for batch-processing of documents by defining them as a lazily-executed graph.
 
 ## Installation
 
-While pydoxtools can already be installed through pip. Due to the
-many updates coming in right now, it is right now recommended to use
-the latest version from github as follows:
+### Installing from GitHub
+
+While pydoxtools can already be installed through pip, due to the
+many updates coming in right now, it is currently recommended to use
+the latest version from GitHub as follows:
 
     pip install -U "pydoxtools[etl,inference] @ git+https://github.com/xyntopia/pydoxtools.git"
 
-Pydoxtools can be also be installed through pip which will become the recommended
+### Installing from PyPI
+
+Pydoxtools can also be installed through pip, which will become the recommended
 method once it becomes more stable:
 
     pip install -U pydoxtools[etl,inference]
 
-For loading additional file formats (docx, odt, epub) and images, checkout
+For loading additional file formats (docx, odt, epub) and images, check out
 the additional > [Installation Options](#installation-options) <.
 
-## Teaser
+## 🚀 Teaser 🚀
+
+Experience a new level of convenience and efficiency in handling
+documents with Pydoxtools, and reimagine your data extraction pipelines!
 
-Experience a new level of convenience and efficiency in handling documents with Pydoxtools, and reimagine your data
-extraction pipelines! 🎩✨📄.
+In this teaser, we'll demonstrate how to create a document, extract
+tables, and ask questions using AI models:
 
-    import pydoxtools as pdx
+```python
+import pydoxtools as pdx
 
-    # create a document from a file, string, bytestring, file-like object
-    # or even an url:
-    doc = pdx.Document(
-        "https://www.raspberrypi.org/app/uploads/2012/12/quick-start-guide-v1.1.pdf", 
-        document_type=".pdf"
-    )
+# Create a document from various sources: file, string, bytestring, file-like object, or URL
+doc = pdx.Document("https://www.raspberrypi.org/app/uploads/2012/12/quick-start-guide-v1.1.pdf")
 
-You can easily extract a large number of pre-defined information
-about your document. To get a list of possible operators use `print(doc.x_funcs)`.
+# List available extraction functions
+print(doc.x_funcs)
 
-    # extract tables from the pdf as a pandas dataframe:
-    print(doc.tables_df)
+# get all tables from a single document:
+print(doc.tables)
 
-Some extraction operations need input when called. The model that should be
-used for the question answering can be specified through doc.config() and can be any
-model from huggingface.
+# Extract the first 20 tables that we can find in a directory (this might take a while,
+# make sure, to only choose a small directory for testing purposes)
+docs = pdx.DocumentBag("./my_directory_with_documents", forgiving_extracts=True)
+print(docs.bag_apply(["tables_df", "filename"]).take(20))
 
-    # ask a question about the document, using Q&A Models (questionas answered locally!):
-    print(doc.answers(["how much ram does it have?"]))
+# Ask a question about the documents using a local Q&A model
+print(doc.answers(["how much ram does it have?"]))
+# Or only ask about the documents tables (or any other extracted information):
+print(doc.answers(["how much ram does it have?"], "tables"))
 
-others need an API key installed, if it refers to an online service.
+# To use ChatGPT for question-answering, set the API key as an environment variable:
+# OPENAI_API_KEY="sk ...."
+# Then, ask questions about the document using ChatGPT
+print(doc.chat_answers(["What is the target group of this document?"])[0].content)
+print(doc.chat_answers(["Answer if a 5-year old would be able to follow these instructions?"])[0].content)
+```
 
-    # ask a question about the document, using ChatGPT (we need the API key for ChatGPT!):
-    # load the API key into an environment variable like this: 
-    #   
-    # OPENAI_API_KEY="sk ...."
-    # 
-    # Do **NOT** use the key in your code. This could potentially cost you a lot of money...
-    print(doc.chat_answers(["What is the target group of this document?"])[0].content)
-    print(doc.chat_answers(["Answer if a 5-year old would be able to follow these instructions?"])[0].content)
+With Pydoxtools, you can easily access and process your documents, perform various extractions,
+and utilize AI models for more advanced analysis.
 
-## Features
+## Some Features in More Detail
 
-### Large pipelines
+### Large Pipelines
 
-Pydoxtools main feature is the ability to mix LLMs and other
-AI models in large, composable and customizable pipelines.
-As a teaser, check out this pipeline for *.png images from the repository including
-OCR, keyword extraction, vectorization and more. In this pipeline:
+Pydoxtools' main feature is the ability to mix LLMs and other
+AI models in large, composable, and customizable pipelines.
+Using pipelines comes with the slight disadvantage that it
+can be more challenging to add type hints to the code.
+However, using pipelines decouples all parts of your code,
+allowing all operators to work independently. This
+makes it easy to run the pipeline in a distributed setting for big data
+and enables easy, lazy evaluation. Additionally,
+mixing different LLM logics together becomes much easier.
+
+Check out how Pydoxtools' `Document` class mixes pipelines for each individual file type:
 
 - Every node in an ellipse can be called as an attribute of the document-analysis pipeline.
-- Every execution-path is lazily executed throughout the entire graph.
-- Every node is cached by default (can be turned off).
+- Every execution path is lazily executed throughout the entire graph.
+- Every node is cached by default (but can be turned off).
 - Every piece of this pipeline can be replaced by a customized version.
 
-<img src="http://pydoxtools.xyntopia.com/images/document_logic_png.svg" width="500">
+As an example, consider this pipeline for *.png images from the repository,
+which includes OCR, keyword extraction, vectorization, and more:
+
+![png pipeline](http://pydoxtools.xyntopia.com/images/document_logic_.png.svg)
 
-Pipelines can be mixed, partially overwritten and extended which gives you a lot of possibilities
-to extend and adapt the functionality for your specific use-case.
+Pipelines can be mixed, partially overwritten, and extended, giving you a lot of possibilities
+to extend and adapt the functionality for your specific use case.
 
-Find out more about it in the [documentation](http://pydoxtools.xyntopia.com/reference/#pydoxtools.document.Document)
+To learn more about Pydoxtools' large pipelines feature, please refer to
+the [documentation](http://pydoxtools.xyntopia.com/reference/#pydoxtools.document.Document).
 
-#### Pipeline configuration
+#### Pipeline Configuration
 
 Pipelines can be configured. For example the local model used for
 question answering can be selected like this:
 
     doc = Document(fobj="./data/PFR-PR23_BAT-110__V1.00_.pdf"))
             .config(qam_model_id='bert-large-uncased-whole-word-masking-finetuned-squad')
 
 where "qam_model_id" can be any model from huggingface for question answering.
 
     TODO: document how to configure a pipeline
 
-### PDF table extraction algorithms
+### PDF Table Extraction Algorithms
 
 The library features its own sophisticated Table extraction algorithm which is benchmarked
-against a large pdf table dataset. In contrast to most other table extraction frameworks
-out there it does not require:
+against a large pdf table dataset. In contrast to how most "classical" table extraction
+algorithms work, it doesn't require:
 
 - extensive configuration
-- no expensive deep neural networks which need a GPU
+- no expensive deep neural networks for table area recognition which need a GPU and
+  a lot of memory/CPU requirements
 
 This makes it possible to run analysis on PDF files with pydoxtools on CPU with
 very limited resources!
 
 ### TODO: Describe more of the features here...
 
 ## Use Cases
 
-- analyze documents using any model from huggingface...
+- create new documents from unstructured information
+- analyze documents using any model from huggingface
 - analyze documents using a custom model
 - download a pdf from URL
 - generate document keywords
 - extract tables
 - download document from URL "manually" and then feed to document
 - extract addresses
 - extract addresses and use this information for the qam
 - ingest documents into a vector db
 
 ## Installation Options
 
-### Supporting *.docx, *.odt, *.epub
+### Supporting \*.docx, \*.odt, \*.epub
 
 In order to be able to load docx, odt and rtf files, you have to install pandoc.
 Right now, the python pandoc library does not work with pandoc version > 3.0.0. It
 is therefore recommended to install a version from here for your OS:
 
 https://github.com/jgm/pandoc/releases/tag/2.19.2
 
-### Image OCR support
+### Image OCR Support
 
 Pydoxtools can automatically analyze images as well, makin use of
 [OCR](https://en.wikipedia.org/wiki/Optical_character_recognition).
 In order to be able to use this, install tesseract on your system:
 
 Under linux this looks like the following:
 
@@ -175,10 +198,12 @@
 
 You can check the compatibility using the following tool in a venv environment in a production
 setting:
 
     pip install pip-licenses
     pip-licenses | grep -Ev 'MIT License|BSD License|Apache Software License|Python Software Foundation License|Apache 2.0|MIT|Apache License 2.0|hnswlib|Pillow|new BSD|BSD'
 
-## list of libraries, that this project is based on:
+### Dependencies
+
+Here is a list of Libraries, that this project is based on:
 
 [list](poetry.lock)
```

### Comparing `pydoxtools-0.5.1/pydoxtools/class_utils.py` & `pydoxtools-0.6.0/pydoxtools/class_utils.py`

 * *Files identical despite different names*

### Comparing `pydoxtools-0.5.1/pydoxtools/classifier.py` & `pydoxtools-0.6.0/pydoxtools/classifier.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 from torch.nn import functional as F
 from transformers import AutoTokenizer, AutoModel
 
 from pydoxtools import html_utils
 from pydoxtools.settings import settings
 
 logger = logging.getLogger(__name__)
-memory = settings.get_memory_cache()
 tqdm.tqdm.pandas()
 
 
 def init_embeddings(model_name: str = None, dimension=None):
     """
     This function can be used to pre-initialize the embeddings using
     for example BERT embeddings.
```

### Comparing `pydoxtools-0.5.1/pydoxtools/cluster_utils.py` & `pydoxtools-0.6.0/pydoxtools/cluster_utils.py`

 * *Files identical despite different names*

### Comparing `pydoxtools-0.5.1/pydoxtools/document_base.py` & `pydoxtools-0.6.0/pydoxtools/document_base.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,62 +1,69 @@
 import functools
 import json
 import logging
 import pathlib
+import pickle
 import uuid
 from dataclasses import dataclass
 from enum import Enum
 from functools import cached_property
 from time import time
 from typing import List, Any, get_type_hints
 
 import networkx as nx
 import numpy as np
+import pandas as pd
 import spacy.tokens
 import yaml
+from diskcache import Cache
 
-from . import operators
 from .list_utils import deep_str_convert
+from .operators_base import Operator, Configuration, OperatorException, OperatorOutputException
+from .settings import settings
 
 logger = logging.getLogger(__name__)
 
 
 @dataclass(eq=True, frozen=True, slots=True)
 class Font:
     name: str
     size: float
     color: str
 
 
 class ElementType(Enum):
     Graphic = 1
-    Line = 2
+    Text = 2
     Image = 3
 
 
 @dataclass(slots=True)
 class DocumentElement:
     type: ElementType
-    p_num: int
-    x0: float
-    y0: float
-    x1: float
-    y1: float
-    rawtext: str | None
-    font_infos: set[Font] | None
-    linenum: int | None
-    linewidth: float | None
-    boxnum: int | None
-    lineobj: Any | None
-    gobj: Any | None
-    non_stroking_color: str | None
-    stroking_color: str | None
-    stroke: bool | None
-    fill: bool | None
-    evenodd: int | None
+    p_num: int | None = None
+    x0: float | None = None
+    y0: float | None = None
+    x1: float | None = None
+    y1: float | None = None
+    rawtext: str | None = None
+    text: str | None = None
+    sections: list[str] | None = None
+    font_infos: set[Font] | None = None
+    linenum: int | None = None
+    linewidth: float | None = None
+    boxnum: int | None = None
+    lineobj: Any | None = None
+    gobj: Any | None = None
+    non_stroking_color: str | None = None
+    stroking_color: str | None = None
+    stroke: bool | None = None
+    fill: bool | None = None
+    evenodd: int | None = None
+    level: int = 0
 
 
 class TokenCollection:
     def __init__(self, tokens: List[spacy.tokens.Token]):
         self._tokens = tokens
 
     @cached_property
@@ -76,17 +83,14 @@
     def __str__(self):
         return " ".join(t.text for t in self._tokens)
 
     def __repr__(self):
         return "|".join(t.text for t in self._tokens)
 
 
-# TODO: rename into "Operator"
-
-
 class ConfigurationError(Exception):
     pass
 
 
 class MetaPipelineClassConfiguration(type):
     """
     configures derived document class logic on construction.
@@ -131,26 +135,24 @@
                 #
                 # We also combine _extractor definitions from parent class and child class
                 # here. We need to do this here and not use the _pipelines from parent class as
                 # we need to make sure that new functions that were added to e.g. "*" also get added
                 # to "*.pdf" and other document logic if we use the already calculated _pipelines this
                 # would not be guaranteed.
 
-                uncombined_operators: dict[str, dict[str, operators.Operator]] = {}
+                uncombined_operators: dict[str, dict[str, Operator]] = {}
                 extractor_combinations: dict[str, list[str]] = {}  # record the extraction hierarchy
-                uncombined_x_configs: dict[str, dict[str, list[str]]] = {}
-                ex: operators.Operator | str
+                ex: Operator | str
                 # loop through class hierarchy in order to get the logic of parent classes as well,
                 # including the newly defined class
                 for cl in reversed(class_hierarchy):
                     # loop through doc types
                     for doc_type, ex_list in cl._operators.items():
                         doc_type_pipeline = {}  # save function mappings for single doc_type
                         extractor_combinations[doc_type] = []  # save combination list for single doctype
-                        doc_type_x_config = {}  # save configuration mappings for single doc_type
                         for ex in ex_list:
                             # strings indicate that we would like to
                             # add all the functions from that document type as well but with
                             # lower priority
                             if isinstance(ex, str):
                                 extractor_combinations[doc_type].append(ex)
                             else:
@@ -159,30 +161,21 @@
                                 # TODO: we could explicitly add the variables as property functions
                                 #       which refer to the "x"-function in document?
                                 for ex_key, doc_key in ex._out_mapping.items():
                                     # input<->output mapping is already done i the extractor itself
                                     # check out Operator.pipe and Operator.map member functions
                                     doc_type_pipeline[doc_key] = ex
 
-                                    # build a map of configuration values for each
-                                    # parameter. This means when a parameter gets called we know automatically
-                                    # how to configure the corresponding Operator
-                                    if ex._dynamic_config:
-                                        doc_type_x_config[doc_key] = list(ex._dynamic_config.keys())
-
                         uncombined_operators[doc_type] = uncombined_operators.get(doc_type, {})
                         uncombined_operators[doc_type].update(doc_type_pipeline)
-                        uncombined_x_configs[doc_type] = uncombined_x_configs.get(doc_type, {})
-                        uncombined_x_configs[doc_type].update(doc_type_x_config)
 
                 logger.debug("combining... extraction logic")
                 # we need to re-initialize the class logic so that they are not linked
                 # to the logic of the parent classes.
                 new_class._pipelines = {}
-                new_class._x_config = {}
                 doc_type: str
                 # add all extractors by combining the logic for the different document types
                 for doc_type in uncombined_operators:
                     # first take our other document type and then add the current document type
                     # itself on top of it because of its higher priority overwriting
                     # extractors of the lower priority extractors
                     # TODO: how do we make sure that we adhere to the tree structure?
@@ -190,15 +183,14 @@
                     #       document types first, and then subsequently until we are at the bottom
                     #       of the tree.
 
                     # TODO: add classes recursively (we can not combine logic blocks using multiple
                     #       levels right now). We probably need to run this function multiple times
                     #       in order for this to work.
                     new_class._pipelines[doc_type] = {}
-                    new_class._x_config[doc_type] = {}
 
                     # build class combination in correct order:
                     # the first one is the least important, because it gets
                     # overwritten by subsequent classes
                     # TODO: get rid of the "standard" fallback...  for the pipeline
                     doc_type_order = ["*"]  # always use "*" as a fallback
                     if doc_type != "*":
@@ -209,137 +201,149 @@
                     # (which might already exist from the parent class) in the correct order.
                     # already existing functions from the parent class get overwritten by the
                     # ones defined in the child class in "uncombined_operators"
                     for ordered_doc_type in doc_type_order:
                         # add newly defined extractors overriding extractors defined
                         # in lower hierarchy logic
                         new_class._pipelines[doc_type].update(uncombined_operators[ordered_doc_type])
-                        new_class._x_config[doc_type].update(uncombined_x_configs[ordered_doc_type])
-
-                        # TODO: how do we add x-functions to
 
                 # TODO: remove "dangling" extractors which lack input mapping
 
         else:
             raise ConfigurationError(f"no extractors defined in class {new_class}")
 
         elapsed = round((time() - start_time) * 1000, 4)
         logger.info(f"setting up Document class {new_class} took: {elapsed}ms")
 
         return new_class
 
 
 class Pipeline(metaclass=MetaPipelineClassConfiguration):
     """
-    This class is the base for all document classes in pydoxtools and
-    defines a common pipeline interface for all.
-
-    This class also defines a basic extraction schema which derived
-    classes can override
-
-    in order to create a new pipeline, the
-    _extractor variable shoud be overwritten with a pipeline definition
+    Base class for all document classes in pydoxtools, defining a common pipeline
+    interface and establishing a basic pipeline schema that derived classes can override.
 
-    this pipeline will get compiled in a function mappint defined in
-    _pipelines
+    The MetaPipelineClassConfiguration acts as a compiler to resolve the pipeline hierarchy,
+    allowing pipelines to inherit, mix, extend, or partially overwrite each other.
+    Each key in the _pipelines dictionary represents a different pipeline version.
+
+    The [pydoxtools.Document][] class leverages this functionality to build separate pipelines for
+    different file types, as the information processing requirements differ significantly
+    between file types.
+
+    Attributes:
+        _operators (dict[str, list[pydoxtools.operators_base.Operator]]): Stores the definition of the
+            pipeline graph, a collection of connected operators/functions that process
+            data from a document.
+        _pipelines (dict[str, dict[str, pydoxtools.operators_base.Operator]]): Provides access to all
+            operator functions by their "out-key" which was defined in _operators.
+
+    Todo:
+        * Use pandera (https://github.com/unionai-oss/pandera) to validate dataframes
+          exchanged between extractors & loaders
+          (https://pandera.readthedocs.io/en/stable/pydantic_integration.html)
     """
 
-    # TODO: use pandera (https://github.com/unionai-oss/pandera)
-    #       in order to validate dataframes exchanged between extractors & loaders
-    #       https://pandera.readthedocs.io/en/stable/pydantic_integration.html
-
-    # TODO: how do we change extraction configuration "on-the-fly" if we have
-    #       for example a structured document vs unstructered (PDF: unstructure,
-    #       Markdown: structured)
-    #       in this case table extraction algorithms for example would have to
-    #       behave differently. We would like to use
-    #       a different extractor configuration in that case...
-    #       in other words: each extractor needs to be "conditional"
-
-    # stores the definition of the pipeline graph, a collection of connected
-    # operators/functions
-    # which extract data from a document
-    _operators: dict[str, list[operators.Operator]] = {}
-
-    # a dict which provides access for all extractor functions by their "out-key"
-    # which was defined in _operators
-    # TODO: rename into operators
-    _pipelines: dict[str, dict[str, operators.Operator]] = {}
-
-    def __init__(self):
-        self._cache_hits = 0
-        self._x_func_cache: dict[operators.Operator, dict[str, Any]] = {}
+    _operators: dict[str, list[Operator]] = {}
+    _pipelines: dict[str, dict[str, Operator]] = {}
 
-    def config(self, **settings: dict[str, Any]) -> "Pipeline":
+    def __init__(self, **configuration):
         """
-        Set configuration parameters for a pipeline.
+        Initializes the Pipeline instance with cache-related attributes.
 
-        This method loops through all "operators.Configure" instances in the pipeline
-        and assigns the provided configuration settings to them.
-
-        Args:
-            **settings: A dictionary of key-value pairs representing the configuration
+        **configuration: A dictionary of key-value pairs representing the configuration
                 settings for the pipeline. Each key is a string representing the name
                 of the configuration setting, and the value is the corresponding value
                 to be set.
+        """
+        self._configuration = {}
+        self._configuration.update(configuration)
+        self._stats = dict(
+            cache_hits=0,
+            disk_cache_hits=0,
+            # this is a set, because the same error can appear many time
+            cache_errors=set()  # log operators that are not cachable for debugging purposes
+        )
+        self._source = "base_pipeline"
+        self._disk_cache_enable = settings.PDX_ENABLE_DISK_CACHE
+        self._disk_cache_ttl = None
+
+    def _key(self):
+        return None
+
+    def set_disk_cache_settings(
+            self,
+            enable: bool,
+            ttl: int = 3600 * 24 * 7  # default cache expires after 1 week
+    ):
+        """Sets disk cache settings
+        """
+        self._disk_cache_ttl = ttl
+        self._disk_cache_enable = enable
+        return self
 
-        Returns:
-            self: A reference to the current pipeline instance, allowing for method chaining.
+    @cached_property
+    def _disk_cache_enabled(self):
+        return self._disk_cache_enable
 
-        Example:
-            pipeline = Pipeline()
-            pipeline.config(param1=value1, param2=value2)
-        """
-        # Get all configuration objects in the pipeline
-        configuration: dict[str, operators.Configuration] = \
-            {k: v for k, v in self.x_funcs.items() if isinstance(v, operators.Configuration)}
-
-        # Assign the settings to the corresponding configuration objects
-        for k, v in settings.items():
-            configuration[k]._configuration_map[k] = v
+    @cached_property
+    def _cache(self):
+        return {}
 
-        # Return the current pipeline instance for method chaining
-        return self
+    @cached_property
+    def _disk_cache(self) -> dict[Operator, dict[str, Any]] | Cache:
+        cache = Cache(settings.PDX_CACHE_DIR_BASE / "pipelines")
+        return cache
 
     @property
-    def configuration(self) -> dict[str, Any]:
+    def configuration(self):
+        """Returns a dictionary of all configuration objects for the current pipeline.
+
+        Returns:
+            dict: A dictionary containing the names and values of all configuration objects
+                  for the current pipeline.
         """
-        Gets all configuration objects of the pipeline and merges them into a single dictionary.
+        return {k: self.x(k) for k in self.get_configuration_names(self.pipeline_chooser)}
+
+    @classmethod
+    @functools.lru_cache
+    def get_configuration_names(cls, pipeline: str) -> list[str]:
+        """Returns a list of names of all configuration objects for a given pipeline.
+
+        Args:
+            pipeline (str): The name of the pipeline to retrieve configuration objects from.
 
         Returns:
-            dict: A dictionary containing the merged configuration objects of the pipeline, with keys as
-                  the configuration names and values as the configuration objects.
+            list: A list of strings containing the names of all configuration objects for the
+                  given pipeline.
         """
-        configuration: dict[str, operators.Configuration] = \
-            {k: v for k, v in self.x_funcs.items() if isinstance(v, operators.Configuration)}
-        configuration_map = {}
-        for c in configuration:
-            configuration_map.update(**(configuration[c]._configuration_map))
-        return configuration_map
+        configuration: dict[str, Configuration] = \
+            {k: v for k, v in cls._pipelines[pipeline].items() if isinstance(v, Configuration)}
+        return list(configuration.keys())
 
-    @cached_property
+    @property
     def pipeline_chooser(self) -> str:
         """
         Must be implemented by derived classes
         to decide which pipeline they should use.
         """
         # TODO: maybe rename this into "head-pipeline" or something like that?
         # TODO: not sure how to do this the "correct" way with @abstractmethod
         #       as we can not derive from ABC due to our metaclass...
         raise NotImplementedError("derived pipelines need to override this function!")
 
     @cached_property
-    def x_funcs(self) -> dict[str, operators.Operator]:
+    def x_funcs(self) -> dict[str, Operator]:
         """
         get all operators/pipeline nodes and their property names
         for this specific file type/pipeline
         """
         return self._pipelines[self.pipeline_chooser]
 
-    def property_dict(self, *args, **kwargs):
+    def to_dict(self, *args, **kwargs):
         """
         Returns a dictionary that accumulates the properties given in *args or with a mapping in **kwargs.
 
         Args:
             *args (str): A variable number of strings, each representing a property name.
             **kwargs (dict): A dictionary mapping property names (values) to custom keys (keys) for the
                              returned dictionary.
@@ -355,15 +359,21 @@
         """
 
         properties = {a: getattr(self, a) for a in args}
         properties.update({v: getattr(self, k) for k, v in kwargs.items()})
 
         return deep_str_convert(properties)
 
-    def yaml(self, *args, **kwargs):
+    @functools.cache
+    def to_dataframe(self, *args, **kwargs):
+        dictlist = self.to_dict(*args, **kwargs)
+        df = pd.DataFrame(dictlist)
+        return df
+
+    def to_yaml(self, *args, **kwargs):
         """
         Returns a dictionary that accumulates the properties given in *args or with a mapping in **kwargs, and dumps the output as YAML.
 
         Args:
             *args (str): A variable number of strings, each representing a property name.
             **kwargs (dict): A dictionary mapping property names (values) to custom keys (keys) for the
                              returned dictionary.
@@ -373,19 +383,19 @@
             "full_text". Properties like "answers" that return a function requiring arguments cannot be
             used with this function.
 
         Returns:
             str: A YAML-formatted string representing the accumulated properties and their values, using
                  either the property names or custom keys as specified in the input arguments.
         """
-        out = self.property_dict(*args, **kwargs)
+        out = self.to_dict(*args, **kwargs)
         out = yaml.safe_dump(out)
         return out
 
-    def json(self, *args, **kwargs):
+    def to_json(self, *args, **kwargs):
         """
         Returns a dictionary that accumulates the properties given in *args or with a
         mapping in **kwargs, and dumps the output as JSON.
 
         Args:
             *args (str): A variable number of strings, each representing a property name.
             **kwargs (dict): A dictionary mapping property names (values) to custom keys (keys) for the
@@ -396,108 +406,263 @@
             "full_text". Properties like "answers" that return a function requiring arguments cannot be
             used with this function.
 
         Returns:
             str: A JSON-formatted string representing the accumulated properties and their values, using
                  either the property names or custom keys as specified in the input arguments.
         """
-        out = self.property_dict(*args, **kwargs)
+        out = self.to_dict(*args, **kwargs)
         out = json.dumps(out)
         return out
 
-    def non_interactive_pipeline(self) -> dict[str, operators.Operator]:
+    def non_interactive_pipeline(self) -> dict[str, Operator]:
         """return all non-interactive extractors/pipeline nodes"""
         NotImplementedError("TODO: search for functions that are type hinted as callable")
 
     @classmethod
-    def pipeline_docs(cls):
+    def pipeline_docs(cls, pipeline_type=None):
         """
-        Returns a formatted string containing the documentation for each pipeline operation in the class.
+        Aggregates the pipeline operations and their corresponding types and metadata.
 
-        This class method iterates through the pipeline operations, collects information about their
-        output types and supported pipelines, and formats the documentation accordingly.
+        This method iterates through all the pipelines registered in the class, and gathers
+        information about each operation, such as the pipeline types it appears in,
+        the return type of the operation, and the operation's docstring.
 
         Returns:
-            str: A formatted string containing the documentation for each pipeline operation, including
-                 operation name, usage, return type, and supported pipelines.
+            output_infos (Dict[str, Dict[str, Union[Set, str]]]): The aggregated information
+                about pipeline operations, with operation keys as the top-level keys, and
+                metadata such as pipeline types, output types, and descriptions as nested
+                dictionaries.
         """
         output_infos = {}
         # aggregate information
         for pipeline_id, ops in cls._pipelines.items():
             for op_k, op in ops.items():
                 oi: dict[str, set] = output_infos.get(op_k, None) or dict(pipe_types=set(), output_types=set())
                 oi["pipe_types"].add(pipeline_id)
                 if return_type := get_type_hints(op.__class__.__call__).get("return", None):
                     oi["output_types"].add(return_type)
+                oi["description"] = op.__node_doc__
                 output_infos[op_k] = oi
 
+        if pipeline_type:
+            return output_infos[pipeline_type]
+        else:
+            return output_infos
+
+    @classmethod
+    def markdown_docs(cls):
+        """
+        Returns a formatted string containing the documentation for each pipeline operation in the class.
+
+        This class method iterates through the pipeline operations, collects information about their
+        output types and supported pipelines, and formats the documentation accordingly.
+
+        Returns:
+            str: A formatted string containing the documentation for each pipeline operation, including
+                 operation name, usage, return type, and supported pipelines.
+        """
+        output_infos = cls.pipeline_docs()
+
         node_docs = []
         for k, v in output_infos.items():
+            return_types = " | ".join(sorted(str(i) for i in v['output_types']))
+            return_types = return_types.replace(">", "\>")
+            pipeline_flows = ", ".join(sorted(v['pipe_types']))
+            pipeline_flows = pipeline_flows.replace(">", "\>")
+
             single_node_doc = f"""### {k}
+            
+{v['description']}
 
 Can be called using:
 
-    doc.x('{k}')
+    <{cls.__name__}>.x('{k}')
     # or
-    doc.{k}
+    <{cls.__name__}>.{k}
 
 return type
-: {"".join(sorted(str(i) for i in v['output_types']))}
+: {return_types}
 
-supports pipelines
-: {",".join(sorted(v['pipe_types']))}"""
+supports pipeline flows:
+: {pipeline_flows}"""
             node_docs.append(single_node_doc)
 
         docs = '\n\n'.join(node_docs)
         return docs
 
-    def x(self, extract_name: str, *args, **kwargs) -> Any:
+    def gather_arguments(self, **kwargs):
+        """
+        Gathers arguments from the pipeline and class, and maps them to the provided keys of kwargs.
+
+        This method retrieves all required input parameters from _in_mapping, which was declared with "pipe".
+        It first checks if the parameter is available as an extractor. If so, it calls the function to get the value.
+        Otherwise, it gets the "native" member-variables or other functions if an extractor with that name is not found.
+
+        Args:
+            **kwargs (dict): A dictionary containing the keys to be mapped to the corresponding values.
+
+        Returns:
+            dict: A dictionary containing the mapped keys and their corresponding values.
+        """
+        mapped_kwargs = {}
+        # get all required input parameters from _in_mapping which was declared with "pipe"
+        for k, v in kwargs.items():
+            # first check if parameter is available as an extractor
+            if v in self.x_funcs:
+                # then call the function to get the value
+                mapped_kwargs[k] = self.x(v)
+            else:
+                # get "native" member-variables or other functions
+                # if not found an extractor with that name
+                mapped_kwargs[k] = getattr(self, v)
+        return mapped_kwargs
+
+    def x(self, operator_name: str) -> Any:
         """
         Calls an extractor from the defined pipeline and returns the result.
 
         Args:
-            extract_name (str): The name of the extractor to be called.
-            *args: Variable-length argument list to be passed to the extractor.
-            **kwargs: Arbitrary keyword arguments to be passed to the extractor.
+            operator_name (str): The name of the extractor to be called.
 
         Returns:
             Any: The result of the extractor after processing the document.
 
         Raises:
             operators.OperatorException: If an error occurs while executing the extractor.
 
         Notes:
             The extractor's parameters can be overridden using *args and **kwargs.
         """
-        if not (extractor_func := self.x_funcs.get(extract_name, None)):
-            return self.__dict__[extract_name]  # choose the class' own properties as a fallback
+        # override the operator if this instance has its own configuration
+        if operator_name in self._configuration:
+            return self._configuration[operator_name]
+        elif not (operator_function := self.x_funcs.get(operator_name, None)):
+            return self.__dict__[operator_name]  # choose the class' own properties as a fallback
 
         try:
-            # check if we executed this function at some point...
-            if extractor_func._cache:
-                key = functools._make_key((extractor_func,) + args, kwargs, typed=False)
+            # whether function should be cached or not...
+            finished_calculation = False
+            # taking the operator_function instead of the output as a key makes everything here more
+            # efficient, because we don't have to store the output for individual
+            # keys in case a function has multiple keys as an output...
+            dict_cache_key = operator_function
+            disk_cache_key = None
+            if operator_function._cache:
+                # first check if we already have the result in memory-cache,
+                # as this is much faster than getting the result from disk
+                # we can be less specific about this key as our cache here is
+                # saved in the document instance.
+                # As the arguments are always going to be the same,
+                # only the operator name is sufficient here
                 # we need to check for "is not None" as we also have pandas dataframes in this
                 # which cannot be checked for by simply using "if"
-                if (res := self._x_func_cache.get(key, None)) is not None:
-                    self._cache_hits += 1
+                if (res := self._cache.get(dict_cache_key, None)) is not None:
+                    self._stats["cache_hits"] += 1
+                    finished_calculation = True
+
+                # TODO: hash pandas.util.hash_pandas_object for mapped kwargs key
+                if (not finished_calculation) and self._disk_cache_enabled \
+                        and operator_function._allow_disk_cache:
+                    # We are creating a key using a hash value
+                    # for this specific instance of a pipeline object.
+                    # this key should be provided by the pipeline itself.
+                    # we can not use the function arguments as keys, as they are iteratively
+                    # calculated through the pipeline. this means
+                    # that we would have to calculate the entire tree in the pipeline to get the
+                    # parameters for this function.
+                    if disk_cache_key := self._key():  # key might not exist!
+                        disk_cache_key = operator_name + str(disk_cache_key)
+
+                    if (not finished_calculation) and disk_cache_key:
+                        try:
+                            # we need to check for "is not None" as we also have pandas dataframes in this
+                            # which cannot be checked for by simply using "if"
+                            if (res := self._disk_cache.get(disk_cache_key, None)) is not None:
+                                self._stats["disk_cache_hits"] += 1
+                                finished_calculation = True
+                        except (pickle.PicklingError) as error:
+                            # simply don't do anything with the cache, if we can not cache it, but log
+                            # the function;)
+                            self._stats["cache_errors"].add((operator_name, error))
+                    else:
+                        self._stats["cache_errors"].add((operator_name, "no key for disk caching"))
+
+            # if we haven't gotten the result from cache yet...
+            if finished_calculation == False:
+                mapped_kwargs = self.gather_arguments(**operator_function._in_mapping)
+                if operator_function._default:
+                    try:
+                        res = operator_function(**mapped_kwargs)
+                    except:
+                        res = operator_function._default
                 else:
-                    res = extractor_func._mapped_call(self, *args, **kwargs)
-                    self._x_func_cache[key] = res
+                    res = operator_function(**mapped_kwargs)
+                # and save the result in both caches
+                if operator_function._cache:
+                    self._cache[dict_cache_key] = res
+                    if self._disk_cache_enabled and disk_cache_key:
+                        try:
+                            # self._disk_cache.set(disk_cache_key, res, expire=self._disk_cache_ttl)
+                            self._disk_cache.set(disk_cache_key, res)
+                        except (pickle.PicklingError, AttributeError, TypeError) as error:
+                            self._stats["cache_errors"].add((operator_name, error))
+
+            # TODO: this can probably made more elegant
+            if isinstance(res, dict):
+                res = {operator_function._out_mapping[k]: v for k, v in res.items()
+                       if k in operator_function._out_mapping}
             else:
-                res = extractor_func._mapped_call(self, *args, **kwargs)
+                # use first key of out_mapping for output if
+                # we only have a single return value
+                res = {next(iter(operator_function._out_mapping)): res}
+
 
-        except operators.OperatorException as e:
-            logger.error(f"Extraction error in '{extract_name}': {e}")
+        except OperatorException as e:
+            logger.error(f"Extraction error in {self}, '{operator_name}': {e}")
             raise e
         except Exception as e:
-            logger.error(f"Extraction error in '{extract_name}': {e}")
-            raise operators.OperatorException(f"could not get {extract_name} for {self}")
+            logger.error(f"Extraction error in {self}, '{operator_name}': {e}")
+            raise OperatorException(f"could not get {operator_name} for {self}")
             # raise e
 
-        return res[extract_name]
+        # TODO automatically wrap the result with functools.cache if
+        #      it is a callable. (or use our own cache decorator)
+
+        try:
+            return res[operator_name]
+        except KeyError:
+            raise OperatorOutputException(
+                f"Key '{operator_name}' does not exist in output dict of Operator {operator_function}")
+
+    def get(self, property: str, default_return: Any = None) -> Any:
+        try:
+            return self.x(property)
+        except KeyError:
+            return default_return
+
+    def __getitem__(self, extract_name) -> Any:
+        """
+        Retrieves an extractor result by directly accessing it as an attribute.
+
+        This method is automatically called for attribute names that
+        aren't defined on class level, allowing for a convenient
+        way to access pipeline operator outputs without needing to call the 'x' method.
+
+        Example:
+            >>> document["addresses"]
+            instead of document.x('addresses')
+
+        Args:
+            extract_name (str): The name of the extractor result to be accessed.
+
+        Returns:
+            Any: The result of the extractor after processing the document.
+        """
+        return self.x(extract_name)
 
     def __getattr__(self, extract_name) -> Any:
         """
         Retrieves an extractor result by directly accessing it as an attribute.
 
         This method is automatically called for attribute names that
         aren't defined on class level, allowing for a convenient
@@ -511,37 +676,68 @@
             extract_name (str): The name of the extractor result to be accessed.
 
         Returns:
             Any: The result of the extractor after processing the document.
         """
         return self.x(extract_name)
 
+    def __getstate__(self):
+        """
+        return necessary variables for pickling, ensuring that
+        we leave out everything that can potentiall have some sort
+        of a lambda function in it...
+        """
+        state = self.__dict__.copy()
+        drop_vars = [
+            "x_funcs", "_pipelines", "_cache",
+            "_disk_cache", "_operators",
+        ]
+        for v in drop_vars:
+            state.pop(v, None)
+        return state
+
+    def __setstate__(self, state: dict):
+        """
+        we need to restore _x_func_cache for pickling to work...
+        """
+        # for k,v in state:
+        self.__dict__.update(state)
+        # TODO: restore more cached values to increase speed in a distributed setting.
+        #       for this we need to rely on our cache to work with strings as keys
+        #       and not functions...
+
     def x_all(self):
         """
         Retrieves the results of all extractors defined in the pipeline.
 
         Returns:
             dict: A dictionary containing the results of all extractors, with keys as the extractor
                   names and values as the corresponding results.
         """
         return {property: self.x(property) for property in self.x_funcs}
 
-    def run_pipeline(self):
+    def run_pipeline(self, exclude: list[str] = None):
         """
         Runs all extractors defined in the pipeline for testing or pre-caching purposes.
 
         !!IMPORTANT!!!  This function should normally not be used as the pipeline is lazily executed
         anyway.
 
         This method iterates through the defined extractors and calls each one, ensuring that the
         extractor logic is functioning correctly and caching the results if required.
         """
         # print(pdfdoc.elements)
+        exclude = exclude or []
         for x in self.x_funcs:
-            self.x(x)
+            if x not in exclude:
+                self.x(x)
+
+    def run_pipeline_fast(self):
+        """run pipeline, but exclude long-running calculations"""
+        self.run_pipeline(exclude=["slow_summary"])
 
     def pre_cache(self):
         """
         Pre-caches the results of all extractors that have caching enabled.
 
         This method iterates through the defined extractors and calls each one with caching enabled,
         storing the results for faster access in future calls.
@@ -558,26 +754,18 @@
 
     # TODO: save document structure as a graph...
     # nx.write_graphml_lxml(G,'test.graphml')
     # nx.write_graphml(G,'test.graphml')
 
     def __repr__(self):
         """
-        Returns a string representation of the instance.
-
-        This method provides a string representation of the instance, including the module and class
-        names, as well as the file object or string and the source.
-
         Returns:
             str: A string representation of the instance.
         """
-        if isinstance(self._fobj, str | bytes):
-            return f"{self.__module__}.{self.__class__.__name__}({self._fobj[-10:]},{self.source})>"
-        else:
-            return f"{self.__module__}.{self.__class__.__name__}({self._fobj},{self.source})>"
+        return f"{self.__module__}.{self.__class__.__name__}"
 
     # TODO: more configuration options:
     #       - which nlp models (spacy/transformers) to use
     #       - should "full text" include tables?
     #       - should ner include tables/figures?
 
     # TODO: calculate md5-hash for the document and
@@ -595,15 +783,16 @@
         accesses.
 
         Returns:
             uuid.UUID: A unique identifier for the instance.
         """
         return uuid.uuid4()
 
-    def pipeline_graph(self, image_path: str | pathlib.Path = None, document_logic_id="current"):
+    @classmethod
+    def pipeline_graph(cls, image_path: str | pathlib.Path = None, document_logic_id="*"):
         """
         Generates a visualization of the defined pipelines and optionally saves it as an image.
 
         Args:
             image_path (str | pathlib.Path, optional): File path for the generated image. If provided, the
                                                        generated graph will be saved as an image.
             document_logic_id (str, optional): The document logic ID for which the pipeline graph should
@@ -614,25 +803,23 @@
                     visualized or manipulated using PyGraphviz functions.
 
         Notes:
             This method requires the NetworkX and PyGraphviz libraries to be installed.
         """
         # TODO: change into a static method
         graph = nx.DiGraph()
-        if document_logic_id == "current":
-            logic = self.x_funcs
-        else:
-            logic = self._pipelines[document_logic_id]
+        logic = cls._pipelines[document_logic_id]
 
         for name, f in logic.items():
-            f_class = f.__class__.__name__ + "\n".join(f._out_mapping.keys())
+            f_class = "\n".join([f.__class__.__name__] + list(f._out_mapping.keys()))
+            name = f.__class__.__name__
             shape = "none"
-            if isinstance(f, operators.Configuration):
+            if isinstance(f, Configuration):
                 shape = "invhouse"
-            graph.add_node(f_class, shape=shape)
+            graph.add_node(f_class, shape=shape, label=name)
             # out-edges
             for k, v in f._out_mapping.items():
                 graph.add_node(v)  # , shape="none")
                 graph.add_edge(f_class, v)
             for k, v in f._in_mapping.items():
                 graph.add_edge(v, f_class)
             # f._dynamic_config
```

### Comparing `pydoxtools-0.5.1/pydoxtools/extract_classes.py` & `pydoxtools-0.6.0/pydoxtools/extract_classes.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 
 import langdetect
 import pandas as pd
 from transformers import AutoModelForSequenceClassification, pipeline, AutoTokenizer
 
-from pydoxtools.operators import Operator
+from pydoxtools.operators_base import Operator
 from pydoxtools.settings import settings
 
 logger = logging.getLogger(__name__)
 
 
 class LanguageExtractor(Operator):
     def __call__(self, text) -> str:
@@ -23,15 +23,15 @@
 class TextBlockClassifier(Operator):
     def __init__(self):
         super().__init__()
 
     def __call__(self, text_box_elements: pd.DataFrame):
         tokenizer = AutoTokenizer.from_pretrained("bert-base-uncased")
         model_name = "txtblockclassifier"
-        model_dir = settings.MODEL_DIR / model_name
+        model_dir = settings.PDX_MODEL_DIR / model_name
         if not model_dir.exists():
             # TODO: download "any" model that we want from transformers
             logger.info(f"model {model_name} not found in pydoxtools models, download directly from transformers!")
             model_dir = "xyntopia/tb_classifier"
         # tokenizer_kwargs = {'padding': True, 'truncation': True, 'max_length': 512, 'return_tensors': 'pt'}
         # TODO: optionally enable CUDA...
         # TODO: only extract "unique" addresses
```

### Comparing `pydoxtools-0.5.1/pydoxtools/extract_html.py` & `pydoxtools-0.6.0/pydoxtools/extract_html.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,16 +12,15 @@
 import lxml
 import numpy as np
 import pandas as pd
 import readability
 from bs4 import BeautifulSoup, NavigableString
 from goose3 import Goose
 
-import pydoxtools.operators
-from pydoxtools import document_base
+import pydoxtools.operators_base
 from pydoxtools import html_utils
 from pydoxtools.html_utils import logger, clean_html
 
 try:
     # import a couple libraries that are only
     # needed for analysis purposes
     import selenium
@@ -187,20 +186,22 @@
 def extract_schema(raw_html, url):
     baseurl = urlsplit(url).netloc
     # all meta tags
     data = extruct.extract(raw_html, baseurl, uniform=True)
     return data
 
 
-class HtmlExtractor(pydoxtools.operators.Operator):
+class HtmlExtractor(pydoxtools.operators_base.Operator):
     def __init__(self, engine="combined"):
         super().__init__()
         self._engine = engine
 
     def __call__(self, raw_html: str, url: str = ""):
+        url = str(url)
+
         if self._engine == "combined":
             try:  # try to unescape html its ok if it doesn't work
                 raw_html = html.unescape(raw_html)
             except TypeError:
                 pass
             main_content_html2, title, short_title = extract_title_and_content(raw_html)
```

### Comparing `pydoxtools-0.5.1/pydoxtools/extract_objects.py` & `pydoxtools-0.6.0/pydoxtools/extract_objects.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,20 @@
 from typing import Any
 
 import pandas as pd
+from urlextract import URLExtract
 
-from pydoxtools import nlp_utils
-from pydoxtools.operators import Operator
+from pydoxtools.operators_base import Operator
+from pydoxtools.settings import settings
+
+dns_cache_dir = settings.PDX_CACHE_DIR_BASE / "urlextract"
+dns_cache_dir.mkdir(parents=True, exist_ok=True)
+urlextractor = URLExtract(extract_email=True, cache_dns=True, extract_localhost=True,
+                          cache_dir=dns_cache_dir)
+urlextractor.update_when_older(7)  # updates when list is older that 7 days
 
 
 class EntityExtractor(Operator):
     def __call__(self, spacy_doc) -> dict[str, list[str]]:
         """TODO: add more entity extraction algorithms (e.g. hugginface)"""
         # TODO: add transformers as ner recognition as well:
         #       from transformers import pipeline
@@ -36,15 +43,15 @@
 def grouped_ner(self) -> dict[str, Any]:
     """Group labels from named entity recognition."""
     groups = group_by([n[::-1] for n in self.ner])
     return groups
 
 
 def urls(self) -> list[str]:
-    urls = nlp_utils.get_urls_from_text(self.full_text)
+    urls = urlextractor.find_urls(text, only_unique=False, check_dns=True)
     return urls
 
 
 @property
 def images(self) -> list:
     return []
```

### Comparing `pydoxtools-0.5.1/pydoxtools/extract_ocr.py` & `pydoxtools-0.6.0/pydoxtools/extract_ocr.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import langdetect
 import pytesseract
 from PIL import Image
 from pdfminer.high_level import extract_text
 
 from pydoxtools import ocr_language_mappings
-from pydoxtools.operators import Operator
+from pydoxtools.operators_base import Operator
 
 logger = logging.getLogger(__name__)
 
 
 class OCRException(Exception):
     pass
 
@@ -30,16 +30,19 @@
             raise OCRException("OCR is not enabled!!")
         file = Image.open(io.BytesIO(file))
         if ocr_lang == "auto":
             pdf = pytesseract.image_to_pdf_or_hocr(file, extension='pdf', lang=None)
             text = extract_text(io.BytesIO(pdf))
             try:
                 lang = langdetect.detect(text)
-            except langdetect.lang_detect_exception.LangDetectException:
-                raise OCRException("could not detect language !!!")
+            except langdetect.lang_detect_exception.LangDetectException as err:
+                if err.args[0] == 'No features in text.':
+                    lang = "en" #simply use english as a language
+                else:
+                    raise OCRException("could not detect language !!!")
             # get the corresponding language for tesseract
             lang = ocr_language_mappings.langdetect2tesseract.get(lang, None)
             file.seek(0)  # we are scanning th same file now with the correct language
         else:
             lang = ocr_lang
 
         pdf = pytesseract.image_to_pdf_or_hocr(file, extension='pdf', lang=lang)
```

### Comparing `pydoxtools-0.5.1/pydoxtools/extract_spacy.py` & `pydoxtools-0.6.0/pydoxtools/extract_spacy.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 import numpy as np
 import spacy
 from spacy import Language
 from spacy.tokens import Doc, Token, Span
 
 from .document_base import TokenCollection
-from .operators import Operator
+from .operators_base import Operator
 
 logger = logging.getLogger(__name__)
 
 
 def download_model(model_id: str):
     # python -m spacy download en_core_web_sm
     return subprocess.call(['python', '-m', 'spacy', 'download', model_id])
```

### Comparing `pydoxtools-0.5.1/pydoxtools/extract_tables.py` & `pydoxtools-0.6.0/pydoxtools/extract_tables.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,18 +8,19 @@
 import numpy as np
 import pandas as pd
 import pydantic
 from pdfminer.layout import LTChar
 from sklearn.neighbors import KernelDensity
 
 import pydoxtools
-import pydoxtools.operators
+import pydoxtools.document_base
+import pydoxtools.operators_base
 from pydoxtools import cluster_utils as gu
 from pydoxtools.cluster_utils import pairwise_txtbox_dist, box_cols, y1, x0, x1, boundarybox_intersection_query
-from pydoxtools.operators import Operator
+from pydoxtools.operators_base import Operator
 from pydoxtools.extract_html import extract_lists, extract_tables
 from pydoxtools.extract_textstructure import _line2txt
 
 logger = logging.getLogger(__name__)
 
 idx = pd.IndexSlice
 
@@ -688,16 +689,16 @@
                 y1=y1,
                 w=w,
                 h=h,
                 area=area,
                 row_count=table.shape[0],
                 col_count=table.shape[1],
                 empty_cells_sum=empty_cells.values.sum(),
-                empty_cols_count=empty_cells.any(1).sum(),
-                empty_rows_count=empty_cells.any(0).sum(),
+                empty_cols_count=empty_cells.any(axis=1).sum(),
+                empty_rows_count=empty_cells.any(axis=0).sum(),
 
                 # conditional metrics
                 cell_detected_size_sum=0,
                 cells_span_num=0,  # cells that span more than one cell in the grid
             ))
 
             if "coords" in cells:
@@ -993,15 +994,15 @@
             boxes = boxes.loc[boxes.aspect_ratio < max_aspect_ratio]
     else:
         boxes = pd.DataFrame()
 
     return boxes
 
 
-class Iterator2Dataframe(pydoxtools.operators.Operator):
+class Iterator2Dataframe(pydoxtools.operators_base.Operator):
     """convert arbitrary iterators with arguments into pandas dataframes"""
 
     def __call__(self, iterator):
         def create_data_frame(*args, **kwargs):
             df = pd.DataFrame(iterator(*args, **kwargs))
             return df
```

### Comparing `pydoxtools-0.5.1/pydoxtools/extract_textstructure.py` & `pydoxtools-0.6.0/pydoxtools/extract_textstructure.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from dataclasses import asdict
 
 import pandas as pd
 import pdfminer
 from pdfminer.layout import LTChar, LTTextLineVertical
 from sklearn.ensemble import IsolationForest
 
-import pydoxtools.operators
+import pydoxtools.operators_base
 from pydoxtools import document_base
 
 
 def _line2txt(LTOBJ: typing.Iterable, size_hints=False):
     """
     extract text from pdfiner.six lineobj including size hints
 
@@ -59,27 +59,53 @@
     """
     type such as "pdf", "html" etc...  can also be the mimetype!
     TODO: maybe we can do something generic here?
     """
     return "unknown"
 
 
-class DocumentElementFilter(pydoxtools.operators.Operator):
+class DocumentElementFilter(pydoxtools.operators_base.Operator):
     """Filter document elements for various criteria"""
 
     def __init__(self, element_type: document_base.ElementType):
         super().__init__()
         self.element_type = element_type
 
     def __call__(self, elements: pd.DataFrame):
         df = elements.loc[elements["type"] == self.element_type].copy()
         return df
 
 
-class TextBoxElementExtractor(pydoxtools.operators.Operator):
+def group_elements(elements: pd.DataFrame, by: list[str], agg: str):
+    group = elements.groupby(by)
+    if agg == "boxes_from_lines_w_bb":
+        # aggregate object from the same box and calculate new
+        # bounding boxes, also join the formatted text
+        bg = group.agg(
+            x0=("x0", "min"), y0=("y0", "min"),
+            x1=("x1", "max"), y1=("y1", "max"),
+            text=("lineobj",
+                  lambda x: "".join(_line2txt(obj, size_hints=False) for obj in x.values))
+        )
+        # remove empty box_groups
+        bg = bg[bg.text.str.strip().str.len() > 1].copy()
+        # do some calculations
+        bg['y_mean'] = bg[['y0', 'y1']].mean(axis=1)
+        bg['x_mean'] = bg[['x0', 'x1']].mean(axis=1)
+        bg['w'] = bg.x1 - bg.x0
+        bg['h'] = bg.y1 - bg.y0
+        return bg
+    elif "sections":
+        group = elements.explode('sections').groupby(*by)
+        df = group.agg(text=("rawtext", "sum"), order=("boxnum", "min")).sort_values("order")
+
+        return df["text"].to_dict()
+
+
+class TextBoxElementExtractor(pydoxtools.operators_base.Operator):
     """
     create textboxes and create bounding boxes and aggregated text from
     a pandas dataframe with textlines.
     returns a list of textboxes together wth some coordinate data and
     the contained text.
 
     TODO: generalize this function into an "aggregator" function
@@ -92,36 +118,31 @@
           we save them in the elements array)
 
     TODO: do some schema validation on the pandas dataframes...
     """
 
     def __call__(self, line_elements: pd.DataFrame):
         if "boxnum" in line_elements:
-            group = line_elements.groupby(['p_num', 'boxnum'])
-            # aggregate object from the same box and calculate new
-            # bounding boxes, also join the formatted text
-            bg = group.agg(
-                x0=("x0", "min"), y0=("y0", "min"),
-                x1=("x1", "max"), y1=("y1", "max"),
-                text=("lineobj",
-                      lambda x: "".join(_line2txt(obj, size_hints=False) for obj in x.values))
-            )
-            # remove empty box_groups
-            bg = bg[bg.text.str.strip().str.len() > 1].copy()
-            # do some calculations
-            bg['y_mean'] = bg[['y0', 'y1']].mean(axis=1)
-            bg['x_mean'] = bg[['x0', 'x1']].mean(axis=1)
-            bg['w'] = bg.x1 - bg.x0
-            bg['h'] = bg.y1 - bg.y0
+            bg = group_elements(line_elements, ['p_num', 'boxnum'], agg="boxes_from_lines_w_bb")
             return dict(text_box_elements=bg)
         else:
             return dict(text_box_elements=None)
 
 
-class TitleExtractor(pydoxtools.operators.Operator):
+class SectionsExtractor(pydoxtools.operators_base.Operator):
+    """
+    extract sections from a textbox dataframe
+    """
+
+    def __call__(self, df: pd.DataFrame):
+        bg = group_elements(df, ['sections'], agg="sections")
+        return {"sections": bg}
+
+
+class TitleExtractor(pydoxtools.operators_base.Operator):
     """
     This Operator extracts titels and other interesting text parts
     from a visual document. It does this by characterising parts
     of the text being "different" than the rest using an
     Isolation Forest algorithm (anomyla detection).
     Features are for example: font size,
     position, length etc...
@@ -162,15 +183,16 @@
         dfl['wordcount'] = dfl.text.str.split().apply(len)
         dfl['vertical'] = dfl.lineobj.apply(lambda x: isinstance(x, LTTextLineVertical))
 
         dfl = dfl.join(pd.get_dummies(dfl.font, prefix="font"))
         dfl = dfl.join(pd.get_dummies(dfl.font, prefix="color"))
 
         features = set(dfl.columns) - {'gobj', 'linewidth', 'non_stroking_color', 'stroking_color', 'stroke',
-                                       'fill', 'evenodd', 'type', 'text', 'font_infos', 'font', 'rawtext', 'lineobj',
+                                       'fill', 'evenodd', 'type', 'text', 'font_infos', 'font', 'rawtext',
+                                       'lineobj',
                                        'color'}
 
         # detect outliers to isolate titles and other content from "normal"
         # content
         # TODO: this could be subject to some hyperparameter optimization...
         df = dfl[list(features)]
         clf = IsolationForest()  # contamination=0.05)
```

### Comparing `pydoxtools-0.5.1/pydoxtools/file_utils.py` & `pydoxtools-0.6.0/pydoxtools/file_utils.py`

 * *Files identical despite different names*

### Comparing `pydoxtools-0.5.1/pydoxtools/html_utils.py` & `pydoxtools-0.6.0/pydoxtools/html_utils.py`

 * *Files identical despite different names*

### Comparing `pydoxtools-0.5.1/pydoxtools/labeling.py` & `pydoxtools-0.6.0/pydoxtools/labeling.py`

 * *Files identical despite different names*

### Comparing `pydoxtools-0.5.1/pydoxtools/list_utils.py` & `pydoxtools-0.6.0/pydoxtools/list_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -190,7 +190,21 @@
     specfies the group key.
     """
     groups = {}
     for k, group in groupby(sorted(data, key=itemgetter(0)), lambda x: x[0]):
         groups[k] = [g[1:] for g in group]
 
     return groups
+
+
+def remove_list_from_lonely_object(obj):
+    """remove list if obj is a list and only has a single member"""
+    try:
+        if len(obj) == 1:
+            if isinstance(obj, list):
+                obj = obj[0]
+            elif isinstance(obj, dict):
+                obj = next(iter(obj.values()))
+    except TypeError:  # if obj doesn't have a "len" attribute
+        pass
+
+    return obj
```

### Comparing `pydoxtools-0.5.1/pydoxtools/models.py` & `pydoxtools-0.6.0/pydoxtools/models.py`

 * *Files identical despite different names*

### Comparing `pydoxtools-0.5.1/pydoxtools/nlp_utils.py` & `pydoxtools-0.6.0/pydoxtools/nlp_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -28,17 +28,15 @@
 import sklearn as sk
 import sklearn.linear_model
 import torch
 from pydantic import BaseModel
 from scipy.spatial.distance import pdist, squareform
 from tqdm import tqdm
 from transformers import AutoTokenizer, AutoModel, AutoModelForQuestionAnswering
-from urlextract import URLExtract
 
-from pydoxtools import html_utils
 from pydoxtools.settings import settings
 
 logger = logging.getLogger(__name__)
 
 # from transformers import pipeline #for sentiment analysis
 compare = sklearn.metrics.pairwise.cosine_similarity
 
@@ -51,20 +49,30 @@
     """
     return SequenceMatcher(None, a, b).ratio()
 
 
 device = torch.device("cuda:0" if torch.cuda.is_available() else "cpu")
 logger.info(f"using {device}-device for nlp_operations!")
 
-memory = settings.get_memory_cache()
-dns_cache_dir = settings.CACHE_DIR_BASE / "urlextract"
-dns_cache_dir.mkdir(parents=True, exist_ok=True)
-urlextractor = URLExtract(extract_email=True, cache_dns=True, extract_localhost=True,
-                          cache_dir=dns_cache_dir)
-urlextractor.update_when_older(7)  # updates when list is older that 7 days
+
+@functools.lru_cache(maxsize=32)
+def load_tokenizer(model_id):
+    logger.info("load_tokenizer")
+    tokenizer = AutoTokenizer.from_pretrained(model_id)
+    return tokenizer
+
+
+@functools.lru_cache()
+def load_model(model_id: str) -> Any:
+    logger.info(f"load model {model_id} on device: {device}")
+    # model = AutoModelForQuestionAnswering.from_pretrained(model_id, output_hidden_states=True)
+    model = AutoModel.from_pretrained(model_id, output_hidden_states=True)
+    model.to(device)
+    model.eval()
+    return model
 
 
 # TODO: enhance this with "textrank" algorithms
 def self_similarity_matrix(strlist):
     """
     calculates self-similarity of strings using
     pythons difflib in a matrix
@@ -75,66 +83,59 @@
     def sim(u, v):
         return str_similarity(u[0].lower(), v[0].lower())
 
     s = squareform(pdist(strlist.values.reshape(-1, 1), sim))
     return pd.DataFrame(s)  # , columns=strlist, index=strlist)
 
 
-def get_urls_from_text(text):
-    # TODO:  add this to
-    urls = urlextractor.find_urls(text, only_unique=False, check_dns=True)
-    return urls
-
-
-def get_embeddings(txt, tokenizer):
+def get_tokenizer_only_embeddings(txt: str, model_id: str):
     """
     generate word-piece embeddings (pseudo-syllables)
     using only transformers tokenizer without
     model.
     """
+    tokenizer = load_tokenizer(model_id=model_id)
     txttok = tokenizer.tokenize(txt)
     tok_ids = tokenizer.convert_tokens_to_ids(txttok)
     tok_vecs = get_vocabulary(tokenizer.name_or_path)[tok_ids]
     return tok_vecs, txttok
 
 
-def tokenize_windows(txt, tokenizer, win_len=500, overlap=50,
-                     max_len=510, add_special_tokens=True):
+def tokenize_windows(txt, model_id: str, win_len: int = 500, overlap_ratio: float = 0.1,
+                     max_len: int = 510, add_special_tokens: bool = True):
     """
-    Tokenize a given text into a series of overlapping windows with special tokens.
+    Tokenize text into overlapping windows with special tokens.
 
-    This function tokenizes a given text into a series of overlapping windows,
+    Given an input text, this function tokenizes it into a series of overlapping windows,
     adds special tokens ([CLS], [SEP]) if required, and converts the tokens into
-    token IDs. The function accepts parameters for the window length, overlap between
-    consecutive windows, maximum tokenization length, and a flag to add special tokens.
-    It returns the tokenized windows with token IDs and the tokenized text without
+    token IDs. It returns the tokenized windows with token IDs and the tokenized text without
     token IDs.
 
     Args:
         txt (str): The input text to be tokenized.
-        tokenizer (Tokenizer): The tokenizer instance to be used for tokenization.
+        model_id (str): The model ID for the tokenizer to be used for tokenization.
         win_len (int, optional): The length of each token window. Default is 500.
-        overlap (int, optional): The number of overlapping tokens between consecutive windows. Default is 50.
+        overlap_ratio (float, optional): The ratio of overlapping tokens between consecutive windows. Default is 0.1.
         max_len (int, optional): The maximum length for tokenization. Default is 510.
-        add_special_tokens (bool, optional): Whether to add special tokens ([CLS], [SEP]) to the tokenized text. Default is True.
+        add_special_tokens (bool, optional): Whether to add special tokens ([CLS], [SEP]) to the tokenized text.
+            Default is True.
 
     Returns:
-        list: A list of lists containing the tokenized windows with token IDs.
-        list: The tokenized text without token IDs.
+        Tuple[List[List[int]], List[str]]: A tuple containing a list of lists with the tokenized windows' token IDs
+            and the tokenized text without token IDs.
 
     Example:
 
-        tokenizer = BertTokenizer.from_pretrained("bert-base-uncased")
         txt = "This is a sample text."
-        tok_wins_ids, toktxt = tokenize_windows(txt, tokenizer)
+        tok_wins_ids, toktxt = tokenize_windows(txt, "bert-base-uncased")
 
     """
-    # token_ids = tokenizer.encode(txt,add_special_tokens=False)
+    overlap = int(max_len * overlap_ratio)
+    tokenizer = load_tokenizer(model_id)
     toktxt = tokenizer.tokenize(txt)
-    # tokenizer.convert_tokens_to_ids(toktxt)
 
     tk_num = len(toktxt)
     if tk_num < max_len:
         toktxt = tokenizer.encode(txt)
         if add_special_tokens:
             return [toktxt], toktxt
         else:
@@ -150,26 +151,31 @@
         sep_tok = tokenizer.special_tokens_map['sep_token']
         if add_special_tokens:
             tok_wins = [[cls_tok] + win + [sep_tok] for win in tok_wins]
         tok_wins_ids = [tokenizer.convert_tokens_to_ids(win) for win in tok_wins]
         return tok_wins_ids, toktxt
 
 
-def transform_to_contextual_embeddings(input_ids_t, model, tokenizer=None, lang=False):
+def transform_to_contextual_embeddings(input_ids_t, model_id: str, tokenizer=None, lang=False):
+    """
+    Create contextual embeddings using a huggingface model
+    """
     # for one sentence all ids are "1" for two, the first sentence gets "0"
     input_ids_t = torch.tensor([input_ids_t]).to(device)
     segments_ids_t = torch.tensor([[1] * input_ids_t.shape[1]]).to(device)
 
     # create language IDs
     if lang:
         language_id = tokenizer.lang2id[lang]  # 0
         langs_t = torch.tensor([language_id] * input_ids_t.shape[1])  # torch.tensor([0, 0, 0, ..., 0])
         # We reshape it to be of size (batch_size, sequence_length)
         langs_t = langs_t.view(1, -1)  # is
 
+    model = load_model(model_id=model_id)
+
     # Predict hidden states features for each layer
     with torch.no_grad():
         if lang:  # if XLM cross lingual models
             encoded_layers = model(input_ids_t, langs=langs_t)
             wvecs_out = encoded_layers[0].detach().cpu().numpy()
         else:  # if using BERT-likes/multilingual
             encoded_layers = model(input_ids_t, segments_ids_t)
@@ -179,58 +185,71 @@
             # wvecs_out = encoded_layers[1][-1][0].numpy()[1:-1]
             # this one is for "normal" BERT:
             # wvecs_out = encoded_layers[2][-1][0].numpy()[1:-1]
             # wvecs_out = encoded_layers[2][-1][0].numpy()[1:-1]
     return wvecs_out
 
 
-def longtxt_fullword_embeddings_only_lookup_table(txt, tokenizer):
+def longtxt_fullword_embeddings_only_lookup_table(txt: str, model_id: str):
     """
     generate whole-word embeddings (without pseudo-syllables)
     using only transformers tokenizer without
     model.
     """
-    vs, toktxt = get_embeddings(txt, tokenizer)
+    vs, toktxt = get_tokenizer_only_embeddings(txt, model_id=model_id)
     return fullword_embeddings(toktxt, vs)
 
 
-def longtxt_embeddings_fullword(txt, model, tokenizer):
+def longtxt_embeddings_fullword(txt, model_id: str):
     """
     generate whole-word embeddings (without pseudo-syllables)
     using transformers models.
     """
-    vs, toktxt = longtxt_embeddings(txt, model, tokenizer)
+    vs, toktxt = longtxt_embeddings(txt, model_id)
     return fullword_embeddings(toktxt, vs)
 
 
 def longtxt_embeddings(
-        txt, model, tokenizer,
-        pooling=None,
-        overlap=50,
-        longtextcap=True,
-        status_bar=False
-):
-    """
-    generate wordpiece embeddings (pseudo-syllables) using transformer model
-    and text windowing. The individual windows are stitched
-    back together at the and by averaging their values
+        txt: str, model_id: str,
+        overlap_ratio: float = 0.1, longtextcap: bool = True,
+        status_bar: bool = False
+) -> tuple[np.ndarray, list[str]]:
+    """
+    Generate wordpiece embeddings using a transformer model and text windowing.
+
+    This function generates wordpiece embeddings (pseudo-syllables) using a transformer model
+    and text windowing. The individual windows are stitched back together by averaging their
+    values in the overlapped areas.
+
+    Args:
+        txt (str): Input text for generating embeddings.
+        model_id (str): Model ID for the transformer model to be used.
+        overlap_ratio (float, optional): Ratio of overlapping tokens between consecutive windows. Default is 0.1.
+        longtextcap (bool, optional): Limit the number of tokenized windows to 100. Default is True.
+        status_bar (bool, optional): Display a progress bar for long-lasting transformations. Default is False.
+
+    Returns:
+        Tuple[np.ndarray, List[str]]: A tuple containing the generated embeddings and tokenized text.
+
+    Todo:
+        Add an option to cancel embeddings generation after a certain number of windows to ensure
+        it finishes within a guaranteed time.
 
-    TODO: add option to cancel embeddings generation afte a certain
-          number of windows to make sure it finishes in a guaranteed time
     """
-    tok_wins, toktxt = tokenize_windows(txt, tokenizer=tokenizer,
-                                        overlap=overlap)
+    max_len = get_model_max_len(load_model(model_id=model_id))
+    overlap = int(max_len * overlap_ratio)
+    tok_wins, toktxt = tokenize_windows(txt, model_id=model_id, max_len=max_len, overlap_ratio=overlap_ratio)
     if longtextcap:
         tok_wins = tok_wins[:100]
 
     if status_bar:  # only use tqdm for "long lasting" transformations
-        vec_wins = [transform_to_contextual_embeddings(win, model=model)
+        vec_wins = [transform_to_contextual_embeddings(win, model_id=model_id)
                     for win in tqdm(tok_wins)]
     else:
-        vec_wins = [transform_to_contextual_embeddings(win, model=model)
+        vec_wins = [transform_to_contextual_embeddings(win, model_id=model_id)
                     for win in tok_wins]
     # pd.DataFrame(vec_wins).shapeFalse
 
     if len(vec_wins) == 1:
         vecs = vec_wins[0]
     else:
         win_len = vec_wins[0].shape[0]
@@ -239,36 +258,36 @@
         for i in range(len(vec_wins) - 1):
             # average overlapping vectors of current and next window
             nxtvecs = (vec_wins[i][step:] + vec_wins[i + 1][:overlap]) / 2
             vecs = np.vstack((vecs, nxtvecs))
             vecs = np.vstack((vecs, vec_wins[i + 1][overlap:step]))
         # vecs = np.vstack((vecs,vec_wins[-1][step:]))
 
-    if pooling == None:
-        return vecs, toktxt
-    else:
-        return pooling(vecs, axis=0), toktxt
+    return vecs, toktxt
 
 
 # old name: create_cross_lingual_embeddings
-def create_cross_lingual_contextual_embeddings(txt, model, tokenizer, lang=False):
+def create_cross_lingual_contextual_embeddings(txt: str, model_id: str, lang: bool = False):
     # Map the token strings to their vocabulary indeces.
     # indexed_tokens = tokenizer.convert_tokens_to_ids(toktxt)
+    tokenizer = load_tokenizer(model_id=model_id)
     input_ids_t = torch.tensor([tokenizer.encode(txt)])
 
     # for one sentence all ids are "1" for two, the first sentence gets "0"
     segments_ids_t = torch.tensor([[1] * input_ids_t.shape[1]])
 
     # create language IDs
     if lang:
         language_id = tokenizer.lang2id[lang]  # 0
         langs_t = torch.tensor([language_id] * input_ids_t.shape[1])  # torch.tensor([0, 0, 0, ..., 0])
         # We reshape it to be of size (batch_size, sequence_length)
         langs_t = langs_t.view(1, -1)  # is
 
+    model = load_model(model_id=model_id)
+
     # Predict hidden states features for each layer
     with torch.no_grad():
         if lang:  # if XLM cross lingual models
             encoded_layers = model(input_ids_t, langs=langs_t)
             wvecs_out = encoded_layers[0].detach().numpy()
         else:  # if using BERT-likes
             encoded_layers = model(input_ids_t, segments_ids_t)
@@ -289,58 +308,44 @@
     ab = (a * b).sum(1)
     d = ab / (IaI * IbI)
     return d
 
 
 def reset_models():
     """clear models from memory"""
-    load_models.cache_clear()
+    load_model.cache_clear()
     load_tokenizer.cache_clear()
 
 
-def veclengths(x):
-    return np.sqrt((x * x).sum(axis=1))
-
-
-def maxlens(x):
-    return np.max(x, axis=1)
-
-
 def vecseq_similarity(vs, search_vec):
     return cos_compare(vs, [search_vec])
 
 
 @functools.lru_cache()
 def get_vocabulary(model_id: str):
     """make sure the vocabulary only gets loaded once
     TODO: implement more vocabularies"""
     logger.info(f"loading vocabulary from {model_id}")
-    model, _ = load_models(model_id)
+    model = load_model(model_id)
     # return and transform embeddings into numpy array
     return model.embeddings.word_embeddings.weight.detach().numpy()
 
 
-def fullword_embeddings(toktxt, vs):
+def fullword_embeddings(toktxt: list[str], vs: np.ndarray) -> tuple[np.ndarray, np.ndarray]:
     """
-    get embeddings for entire words by sowing wordpieces back together.
-
-    Parameters
-    ----------
-    toktxt : tokenized text
-        DESCRIPTION.
-    vs : word piece vectors
-        DESCRIPTION.
+    Get embeddings for entire words by sewing word pieces back together.
 
-    Returns
-    -------
-    numpy.ndarray, numpy.ndarray
-        return full word-tokens and vectors
+    Args:
+        toktxt (List[str]): Tokenized text as a list of word pieces.
+        vs (np.ndarray): Word piece vectors as a 2D numpy array.
 
+    Returns:
+        Tuple[np.ndarray, np.ndarray]: Returns two 1D numpy arrays for full word-tokens and vectors respectively.
     """
-    # average embedding vectors for entire words:
+    # Average embedding vectors for entire words:
     emb_map = list(zip(toktxt, vs))
 
     syl_sep = ""  # could also be "-" for example
 
     newtoks = []
     newvs = []
     cur_word = ""
@@ -348,15 +353,15 @@
     for tok, v in emb_map:
         if len(tok) >= 3:
             if tok[:2] == '##':
                 cur_word += tok
                 cur_vec += [v]
                 continue
         newtoks += [cur_word.replace("##", syl_sep)]
-        # TODO:  replace np.mean with np.sum here and below?
+        # TODO: replace np.mean with np.sum here and below?
         newvs += [np.mean(cur_vec, axis=0)]
         cur_vec = [v]
         cur_word = tok
 
     newtoks += [cur_word.replace("##", syl_sep)]
     newvs += [np.mean(cur_vec, axis=0)]
 
@@ -373,121 +378,44 @@
     """
     toktxt = np.array(toktxt)
     idxs = np.argpartition(match.flatten(), -num)[-num:][::-1]
     idxs = idxs[np.argsort(match[idxs][:, 0])][::-1]
     return toktxt[idxs], idxs, match[idxs]
 
 
-def get_max_word_similarity(vs, searchstring, model, tokenizer):
-    sv, _ = get_embeddings(searchstring, tokenizer)
+def get_max_word_similarity(vs, searchstring, model_id: str):
+    sv, _ = get_tokenizer_only_embeddings(searchstring, model_id=model_id)
     match = vecseq_similarity(vs, sv.mean(axis=0))
     return match.max()
 
 
-def search(toktxt, vs, searchstring, model, tokenizer, num=1):
+def search(toktxt, vs, searchstring: str, model_id: str, num=1):
     """
     returns:
         top tokens, token ids, correponding scores, all token scores
     """
     # sv, _ = longtxt_embeddings(search_word,model,tokenizer)
-    sv, _ = get_embeddings(searchstring, tokenizer)
+    sv, _ = get_tokenizer_only_embeddings(searchstring, model_id=model_id)
 
     match = vecseq_similarity(vs, sv.mean(axis=0))
     return top_search_results(toktxt, match, num=num) + (match,)
 
 
-def get_keywords():
-    raise NotImplementedError
-    # justsome ideas in the following
-    # TODO: generate "vs" using transform_to_contextual_embeddings
-    # TODO: maybe to a ANN search with the vocabulary from BERT?
-    similarity = nlpu.vecseq_similarity(vs, sentvec)
-    wordranks = pd.DataFrame(zip(similarity, tokwords),
-                             columns=['similarity', 'words'])
-    wordranks['importance'] = importance * wordranks['similarity']
-    # colhtml = html_utils.color_text(tokwords, similarity)
-    # oib = html_utils.oib
-    # oib(colhtml)
-
-
-# def topic_similarity(model):
-
-# these urls were selected, because they have particularly long webpages
-# to slow down the classifiers etc...
-example_urls = [
-    "https://www.newark.com/c/passive-components/resistors-fixed-value",
-    "https://www.newark.com/c/test-measurement/test-equipment-accessories",
-    "https://www.newark.com/c/enclosures-racks-cabinets/enclosures-boxes-cases",
-    "https://www.newark.com/c/circuit-protection/tvs-transient-voltage-suppressors",
-    "https://chicagodist.com/collections/pololu",
-    "https://www.newark.com/c/semiconductors-discretes/transistors",
-    "https://chicagodist.com/collections/all-in-stock-items",
-    "https://buyzero.de/products/raspberry-pi-4-model-b?variant=28034033287270",
-    "https://buyzero.de/products/raspberry-pi-4-model-b?variant=28034033090662",
-    "https://buyzero.de/products/raspberry-pi-4-model-b?variant=28034034008166",
-]
-
-
-def calculate_string_embeddings(text: str, model_id: str, only_tokenizer: bool):
+def calculate_string_embeddings(text: str, model_id: str, only_tokenizer: bool, overlap_ratio: float = 0.1):
     """
     this method converts a text of arbitrary length into
     a vector.
     """
-    tokenizer = load_tokenizer(model_id)
     if only_tokenizer:
-        vs, toktxt = get_embeddings(text, tokenizer)
-        vs = vs.mean(axis=0)
-        return vs
+        vs, toktxt = get_tokenizer_only_embeddings(text, model_id)
+        return vs, toktxt
     else:
-        model = load_models()
-        vs, toktxt = longtxt_embeddings(text, model, tokenizer, np.mean)
-        return vs
-
-
-def page2vec(page_str, url=None, method="slow"):
-    """
-    TODO: use the document class for this....
-
-    calculate a fingerprint from any arbitrary webpage
-    
-    TODO: include potential incoming links in fingerprint.
-        Those would have to be search independently
-    
-    TODO: include more information into vectorization such as
-    - tag-density
-    - link-density
-    - nomalized pagelength
-    
-    - which tags
-    - structure of html
-    - screenshot of page
-    """
-    # +length = len(html)
-    # length = len(" ".join(html.split()))
-    if method == "no_embeddings":
-        vs = [
-            len(url),
-            len(page_str),
-        ]
-    elif method in ["slow", "fast"]:
-        try:
-            # TODO: can we somehow move html_utils out of this file?
-            text_short = html_utils.get_pure_html_text(page_str)
-            vs = calculate_string_embeddings(text_short, method)
-        except:
-            logger.exception(f"can not convert: {url}")
-            return None
-
-    vectorization = vs
-    return vectorization
-
-
-# TODO implement this function for reinforcement link following
-def link2vec(source_html, source_url, link_context, link_url):
-    raise NotImplementedError()
+        # vs, toktxt = longtxt_embeddings(text, model, tokenizer, np.mean)
+        vs, toktxt = longtxt_embeddings(text, model_id, overlap_ratio=overlap_ratio)
+        return vs, toktxt
 
 
 def topic_similarity(html, topic, method="slow"):
     """
     compare similarity of a given html page
     with a certain topic.
     
@@ -498,16 +426,17 @@
     
     TODO: make a more "finegrained analysis" 
     """
     vs = page2vec(html, method)
 
     model_id = settings.PDXT_STANDARD_TOKENIZER
     tokenizers = load_tokenizer(model_id)
-    model = load_models(model_id)
-    sv, _ = longtxt_embeddings(topic, model, tokenizer, np.mean)
+    model = load_model(model_id)
+    sv, _ = longtxt_embeddings(topic, model)
+    sv.mean()
     # sv, _ = get_embeddings(searchstring,tokenizer)
 
     similarity = cos_compare([vs], [sv])
     # match = vecseq_similarity(vs,sv.mean(axis=0))
 
     return similarity
 
@@ -515,87 +444,66 @@
 # TODO: we need to move this into the nlp_context class
 #      and provide the use of the models with a timeout
 #      or a "with" context or something similar...
 
 # @functools.lru_cache()
 
 
-def convert_ids_to_string(tokenizer, ids):
+def convert_ids_to_string(model_id: str, ids):
+    tokenizer = load_tokenizer(model_id=model_id)
     a = tokenizer.convert_ids_to_tokens(ids)
     return tokenizer.convert_tokens_to_string(a)
 
 
-# TODO: get rid of this...
-# we are creating a factory here as our tranformers vector calculation is stateful
-# and we need a specific class for this..
-# @Language.factory("my_component", default_config={"some_setting": True})
-# def my_component(nlp, name, some_setting: bool):
-#    return MyComponent(some_setting=some_setting)
-class NLPContext(BaseModel):
-    # doesn't work with trasformers yet because AutoTokenizer/Model
-    # are converted into the respective model classes which don't inherit from Autotokenizer...
-    # TODO: find a potential base class?
-    # TODO: generalize this class with nlp_utils loading models...
-    tokenizer: Any  # transformers.AutoTokenizer
-    model: Any  # transformers.AutoModel
-    capabilities: set[str] = []  # model capabilities e.g. "qam"  or "ner"
-
-    class Config:
-        # we need this as pydantic doesn't have validators for transformers models
-        arbitrary_types_allowed = True
-
-
-@functools.lru_cache(maxsize=32)
-def load_tokenizer(model_name):
-    logger.info("load_tokenizer")
-    tokenizer = AutoTokenizer.from_pretrained(model_name)
-    return tokenizer
-
-
-# TODO: merge this function with
-@functools.lru_cache()
-def load_models(model_id: str):
-    logger.info(f"load model on device: {device}")
-    tokenizer = load_tokenizer(model_id)
-    # model = AutoModelForQuestionAnswering.from_pretrained(model_id, output_hidden_states=True)
-    model = AutoModel.from_pretrained(model_id, output_hidden_states=True)
-    model.to(device)
-    model.eval()
-    return model, tokenizer
-
-
 @functools.lru_cache()
 def load_pipeline(pipeline_type: str, model_id: str):
     from transformers import pipeline
     pipeline_instance = pipeline(pipeline_type, model=model_id)
     return pipeline_instance
 
 
 @functools.lru_cache()
-def QandAmodels(model_id: str):
+def load_qa_models(model_id: str):
     # TODO: only load model "id" and use that id
     #        with transformers AutoModel etc...
     logger.info(f"loading Q & A model and tokenizer {model_id}")
     # model, tokenizer = load_models(model_id)
     # TODO: use load_tokenizer function for this
     tokenizer = load_tokenizer(model_id)
     model = AutoModelForQuestionAnswering.from_pretrained(model_id)
     logger.info(f"finished loading Q & A models... {model_id}")
-    return NLPContext(tokenizer=tokenizer, model=model)
+    return model, tokenizer
+
+
+def get_model_max_len(model):
+    try:
+        max_input_tokens = model.config.max_position_embeddings
+    except AttributeError:
+        # TOOD: we should probably find a better method for this....
+        max_input_tokens = 512  # e.g. this is a good choice for t5 (doesn't have a hard limit,
+        # but huge memory consumption)
+
+    return max_input_tokens
 
 
 def summarize_long_text(
         long_text: str,
         model_id: str,
         token_overlap=50,
         max_len=200,
 ):
+    """
+    This function is rather slow due to the recursive nature of it.
+    It is usually a good idea to do some pre-processing of the
+    text before using this summarizer. For example reducing the text size
+    using a textrank algorithm which filters out unimportant sentences .
+    """
     pipeline = load_pipeline("summarization", model_id=model_id)
     model, tokenizer = pipeline.model, pipeline.tokenizer
-    max_input_tokens = pipeline.model.config.max_position_embeddings
+    max_input_tokens = get_model_max_len(model)
 
     def summarize_chunks(text) -> (str, int):
         inputs = tokenizer(text, return_tensors="pt").input_ids
 
         # Split the input into smaller chunks if it's longer than the maximum number of tokens
         input_chunks = []
         for i in range(0, inputs.shape[1], max_input_tokens - token_overlap):
@@ -615,8 +523,8 @@
         # Combine the summarized chunks
         return " ".join(summarized_chunks), len(input_chunks)
 
     summary, chunk_num = summarize_chunks(long_text)
     while chunk_num > 1:
         summary, chunk_num = summarize_chunks(summary)
 
-    return summary
+    return summary.strip()
```

### Comparing `pydoxtools-0.5.1/pydoxtools/ocr_language_mappings.py` & `pydoxtools-0.6.0/pydoxtools/ocr_language_mappings.py`

 * *Files identical despite different names*

### Comparing `pydoxtools-0.5.1/pydoxtools/operator_huggingface.py` & `pydoxtools-0.6.0/pydoxtools/operator_huggingface.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,26 +9,26 @@
 import functools
 import logging
 from typing import Dict, List, Tuple, Callable
 
 import torch
 
 from pydoxtools import nlp_utils
+from pydoxtools.operators_base import Operator
 from pydoxtools.list_utils import iterablefyer
-from pydoxtools.nlp_utils import tokenize_windows, QandAmodels
-from pydoxtools.operators import Operator
+from pydoxtools.nlp_utils import tokenize_windows
 
 logger = logging.getLogger(__name__)
 
 
-def answer_questions_on_long_text(questions, text, nlp_context) -> Dict[str, List[Tuple[str, float]]]:
+def answer_questions_on_long_text(questions, text, model_id) -> Dict[str, List[Tuple[str, float]]]:
     all_answers = {}
     for q in questions:
         answers = long_text_question(
-            q, text, nlp_context.tokenizer, nlp_context.model)
+            q, text, model_id=model_id)
         all_answers[q] = sorted(answers, key=lambda x: -x[1])
 
     return all_answers
 
 
 # we have functools.lru_cache outside of NLPContext because we would like to
 # cache this function and there is memory leak when using lru_cache on a member function
@@ -71,21 +71,22 @@
         if len(answer.split()) > max_ans_words:
             continue
         answer_score = (answers_start_scores[i] + answers_end_scores[i]).detach().numpy()
         answers.append((answer, answer_score.item()))
     return answers
 
 
-def long_text_question(question, text, tokenizer, model):
+def long_text_question(question, text, model_id: str):
     max_len = 512  # maximum possble input for BERT and other transformers
+    model, tokenizer = nlp_utils.load_qa_models(model_id=model_id)
     q_inputs = tokenizer(question, add_special_tokens=False, return_tensors="pt")
     q_len = q_inputs.input_ids.shape[1]
     max_txt_len = max_len - q_len - 3  # -1, because the [CLS] token from q_len will get truncated
     win_tokens, win_toktxt = tokenize_windows(
-        text, tokenizer, win_len=max_txt_len, overlap=50, max_len=512,
+        text, model_id, win_len=max_txt_len, overlap_ratio=0.1, max_len=512,
         add_special_tokens=False)
 
     q_tokens = q_inputs.input_ids[0].tolist()
     q_len = len(q_tokens)
     answers = []
     # check if model needs type_ids:
     needs_type_ids = 'token_type_ids' in tokenizer("test1", "test2")
@@ -154,16 +155,14 @@
     Question Answering Machine Operator
 
     The Operator generates a function takes questions and gives back
     answers on the given text.
 """
 
     def __call__(self, property_dict: Callable, trf_model_id: str = None):
-        nlpc = QandAmodels(trf_model_id)
-
         @functools.lru_cache
         def qa_machine(
                 questions: list[str] | str,
                 props: list[str] | str = "full_text"
         ) -> list[list[tuple[str, float]]]:
             # choose the property that we want to ask a question about...
             if isinstance(props, str):
@@ -171,15 +170,15 @@
                 data = property_dict(props)[props]
             else:
                 data = property_dict(*props)
 
             # TODO: sort answers regarding threshold
             text = str(data)
             questions = iterablefyer(questions)
-            allanswers = answer_questions_on_long_text(questions, text, nlpc)
+            allanswers = answer_questions_on_long_text(questions, text, model_id=trf_model_id)
             answers = list(allanswers.values())
             return answers
 
         return qa_machine
 
 
 if __name__ == "__main__":
```

### Comparing `pydoxtools-0.5.1/pydoxtools/operators.py` & `pydoxtools-0.6.0/pydoxtools/operators_base.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """
 The pydoxtools.operators module defines
 a set of generic pipeline operators that can
 be used inside of a pipeline class definition
 to create your own pipelines.
 """
-
 import abc
 import typing
 from abc import ABC
+
 from typing import Callable, Iterable, Any
 
 
 class Operator(ABC):
     """Base class to build extraction logic for information extraction from
     unstructured documents and loading files
 
@@ -22,86 +22,52 @@
     - Extractors can be "hooked" into the document pipeline by using:
         pipe, out and cache calls.
     - all parameters given in "out" can be accessed through the "x" property
       (e.g. doc.x("extraction_parameter"))
 
     dynamic configuration of an extractor parameters can be configured through
     "config" function which will indicate to the parent document class
-    to set some input parameters to this function manually.
-    If the same parameters are also set in doc.pipe the parameters are
-    optional and will only be taken if explicitly set through doc.config(...).
+    to set some input parameters to this function automatically.
+
+    configuration parameters can be set during pipeline initialization like this:
 
     ```
-    doc.dynamic()
+    Pipeline(source=...).config(
+        first_config_parameter=...,
+        seconf_config_parameter=...
+    )
     ```
 
-    This function can be accessed through:
+    In order to know what parameters of a pipeline are configurable and what
+    their default values are, call the configuration parameter like this:
 
-    ```python
-    doc.config(my_dynamic_parameter="some_new_value")
-    ```
+    Pipeline(source=...).configuration
+
+    If the same parameters are also set in doc.pipe the parameters are
+    optional and will only be taken if explicitly set through doc.config(...).
+
+    TODO: explain configuration parameters
     """
 
     # TODO:  how can we anhance the type checking for outputs?
     #        maybe turn this into a dataclass?
 
     def __init__(self):
         # try to keep __init__ with no arguments for Operator..
         self._in_mapping: dict[str, str] = {}
         self._out_mapping: dict[str, str] = {}
         self._cache = False  # TODO: switch to "True" by default
-        self._dynamic_config: dict[str, str] = {}
+        self._allow_disk_cache = True
+        self._default = None
+        self.__node_doc__ = ""
 
     @abc.abstractmethod
     def __call__(self, *args, **kwargs) -> dict[str, typing.Any] | Any:
         pass
 
-    def _mapped_call(
-            self, parent_document: "document_base.Pipeline",
-            *args,
-            **kwargs
-    ) -> dict[
-        str, typing.Any]:
-        """
-        map objects from document properties to
-        processing function.
-
-        essentially, This maps the outputs from one element of _operators
-        to the inputs of another and also makes sure
-        to override certain parameters that were specified in
-        a config when calling the document class.
-
-        argument precedence is as follows:
-
-        python-class-member < extractor-graph-function < config
-
-        # TODO: maybe we should change precedence and make config the lowest?
-        """
-        mapped_kwargs = {}
-        # get all required input parameters from _in_mapping which was declared with "pipe"
-        for k, v in self._in_mapping.items():
-            # first check if parameter is available as an extractor
-            if v in parent_document.x_funcs:
-                # then call the function to get the value
-                mapped_kwargs[k] = parent_document.x(v)
-            else:
-                # get "native" member-variables or other functions
-                # if not found an extractor with that name
-                mapped_kwargs[k] = getattr(parent_document, v)
-
-        # override graph args directly with function call params...
-        mapped_kwargs.update(kwargs)
-        output = self(*args, **mapped_kwargs)
-        if isinstance(output, dict):
-            return {self._out_mapping[k]: v for k, v in output.items() if k in self._out_mapping}
-        else:
-            # use first key of out_mapping for output if
-            # we only have a single return value
-            return {next(iter(self._out_mapping)): output}
-
     def pipe(self, *args, **kwargs):
         """
         configure input parameter mappings to this function
 
         keys: are the actual function parameters of the extractor function
         values: are the outside function names
 
@@ -118,23 +84,38 @@
         """
         # TODO: rename to "name" because this actually represents the
         #       variable names of the extractor?
         self._out_mapping = kwargs
         self._out_mapping.update({k: k for k in args})
         return self
 
-    def cache(self):
+    def default(self, default: Any):
+        """
+        indicate a default value that we would like to have in case
+        our function has an exception...
+
+        (for example if we can not detect a language, because document is to short)
+        """
+        self._default = default
+        return self
+
+    def cache(self, allow_disk_cache=True):
         """indicate to document that we want this extractor function to be cached"""
         self._cache = True
+        self._allow_disk_cache = allow_disk_cache
         return self
 
     def no_cache(self):
         self._cache = False
         return self
 
+    def docs(self, doc_str: str = ""):
+        self.__node_doc__ = doc_str
+        return self
+
 
 class Alias(Operator):
     """Connect extractor variables with Aliases"""
 
     def __init__(self, **kwargs):
         super().__init__()
         self.pipe(**{v: v for k, v in kwargs.items()})
@@ -153,23 +134,78 @@
         self.out(**{k: k for k in kwargs})
         self.no_cache()
 
     def __call__(self):
         return self.const_result
 
 
-class LambdaOperator(Operator):
+class FunctionOperator(Operator):
     """Wrap an arbitrary function as an Operator"""
 
-    def __init__(self, func):
+    def __init__(self, func, default_return_value: Any = None):
         super().__init__()
         self._func = func
+        self._default_return_value = default_return_value
 
     def __call__(self, *args, **kwargs):
-        return self._func(*args, **kwargs)
+        try:
+            return self._func(*args, **kwargs)
+        except Exception as err:
+            if self._default_return_value:
+                return self._default_return_value
+            else:
+                raise err
+
+
+class ElementWiseOperator(Operator):
+    """
+    Take a function and apply it elementwise to
+    an iterable. Return a list or iterator.
+
+    the "elements" argument will be evaluated
+    element-wise. You can specify additional arguments for the
+    function using *args and **kwargs.
+    """
+
+    # TODO: automatically add documentation from self._func
+    def __init__(self, func: Callable, return_iterator: bool):
+        super().__init__()
+        self._func = func
+        self._return_iterator = return_iterator
+
+    def __call__(self, elements: Iterable, *args, **kwargs):
+        res = (self._func(element, *args, **kwargs) for element in elements)
+        if self._return_iterator:
+            return res
+        else:
+            return list(res)
+
+
+class DictSelector(Operator):
+    def __call__(self, selectable: dict) -> Callable[[...], dict]:
+        def selector(*args, **kwargs) -> dict:
+            selection = {a: selectable.get(a, None) for a in args}
+            selection.update({v: selectable.get(k, None) for k, v in kwargs.items()})
+            return selection
+
+        return selector
+
+
+class DataMerger(Operator):
+    """
+    Merges data from several sources into a single dictionary,
+    it will try to convert everything into strings!
+    """
+
+    def __init__(self):
+        super().__init__()
+
+    def __call__(self, **kwargs):
+        out = kwargs
+        return {"joint_data": out}
 
 
 class Configuration(Operator):
     """
     This is a special operator which can be used to configure a pipeline.
 
     Declare some configuration values which can then be used as inputs for
@@ -208,47 +244,13 @@
         # use the configuration map directly as output mapping
         self.out(*list(configuration_map.keys()))
 
     def __call__(self):
         return self._configuration_map
 
 
-class ElementWiseOperator(Operator):
-    """
-    Take a function and apply it elementwise to
-    an iterable. Return a list or iterator.
-
-    the "elements" argument will be evaluated
-    element-wise. You can specify additional arguments for the
-    function using *args and **kwargs.
-    """
-
-    # TODO: automatically add documentation from self._func
-    def __init__(self, func: Callable, return_iterator: bool):
-        super().__init__()
-        self._func = func
-        self._return_iterator = return_iterator
-
-    def __call__(self, elements: Iterable, *args, **kwargs):
-        res = (self._func(element, *args, **kwargs) for element in elements)
-        if self._return_iterator:
-            return res
-        else:
-            return list(res)
-
-
 class OperatorException(Exception):
     pass
 
 
-class DataMerger(Operator):
-    """
-    Merges data from several sources into a single dictionary,
-    it will try to convert everything into strings!
-    """
-
-    def __init__(self):
-        super().__init__()
-
-    def __call__(self, **kwargs):
-        out = kwargs
-        return {"joint_data": out}
+class OperatorOutputException(OperatorException):
+    pass
```

### Comparing `pydoxtools-0.5.1/pydoxtools/pdf_utils.py` & `pydoxtools-0.6.0/pydoxtools/pdf_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,16 @@
 from pdfminer.high_level import extract_pages
 from pdfminer.layout import LAParams
 from pdfminer.layout import LTChar, LTCurve, LTFigure, LTTextLine
 from pdfminer.layout import LTTextContainer
 from pdfminer.pdfinterp import resolve1
 from pdfminer.pdfparser import PDFParser
 
-import pydoxtools.operators
+import pydoxtools.document_base
+import pydoxtools.operators_base
 from pydoxtools import document_base, list_utils
 
 logger = logging.getLogger(__name__)
 
 try:
     from functools import cached_property
 except ImportError:
@@ -148,15 +149,15 @@
     res = list_utils.deep_str_convert({
         **(doc.info[0]),
         "pagenum": pagenum
     })
     return res
 
 
-class PDFFileLoader(pydoxtools.operators.Operator):
+class PDFFileLoader(pydoxtools.operators_base.Operator):
     """
     Loads a pdf file and can extract all kinds of information from it.
 
     - we extract all textlines with some metadata such as color, textsize
     - use that information to extract "outliers" which are assumed to hold
       important information and represent for example titles of textboxes
     - extract assumed titles by text-size and word count
@@ -259,15 +260,15 @@
                                     str(character.graphicstate.ncolor))
                                 fontset.add(charfont)
                         linetext = text_line.get_text()
                         # extract metadata
                         # TODO: move most of these function to a "feature-generation-function"
                         # which extracts the information directly from the LTTextLine object
                         docelements.append(dict(
-                            type=document_base.ElementType.Line,
+                            type=document_base.ElementType.Text,
                             lineobj=text_line,
                             rawtext=linetext,
                             font_infos=fontset,
                             p_num=page_layout.pageid,
                             linenum=linenum,
                             boxnum=boxnum,
                             x0=text_line.x0,
```

### Comparing `pydoxtools-0.5.1/pydoxtools/random_data_generators.py` & `pydoxtools-0.6.0/pydoxtools/random_data_generators.py`

 * *Files identical despite different names*

### Comparing `pydoxtools-0.5.1/pydoxtools/settings.py` & `pydoxtools-0.6.0/pydoxtools/settings.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,21 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
 Created on Tue Apr 28 21:55:35 2020
 
-general settings for comcharax project.
-scrapy crawler specific settings can be found in
-the the crawler directory and scrapy.cfg.
-
-TODO:
-- adapt this to kubernetes with environment variables or 
-  docker parameters/environmen variables or whatever
-
 @author: tom
 """
 
 import logging
 import os
 from pathlib import Path
 
 import appdirs
 # TODO: remove joblib as a dependency from here ...
-import joblib
 from pydantic import BaseSettings
 
 logger = logging.getLogger(__name__)
 
 # from base64 import b64encode
 
 _FILE_DIR = Path(os.path.dirname(os.path.realpath(__file__)))
@@ -32,30 +23,27 @@
 _HOME = Path.home()
 
 appname = "pydoxtools"
 appauthor = "pydoxtools"
 
 
 class _Settings(BaseSettings):
-    CACHE_DIR_BASE: Path = Path(appdirs.user_cache_dir(appname, appauthor))
+    PDX_CACHE_DIR_BASE: Path = Path(appdirs.user_cache_dir(appname, appauthor))
+    PDX_ENABLE_DISK_CACHE: bool = False
     TRAINING_DATA_DIR: Path = _PYDOXTOOLS_DIR / 'training_data'
-    MODEL_DIR = CACHE_DIR_BASE / "models"
+    PDX_MODEL_DIR = PDX_CACHE_DIR_BASE / "models"
 
     # in order to be able to access OPENAI api
     OPENAI_API_KEY: str = "sk ...."
 
     # PDXT_STANDARD_QAM_MODEL = 'distilbert-base-cased-distilled-squad'
     PDXT_STANDARD_QAM_MODEL = 'deepset/minilm-uncased-squad2'
     # be careful with this one here!!  we would have to retrain ALL of our
     # own, custom models!!!!
     PDXT_STANDARD_TOKENIZER = 'distilbert-base-multilingual-cased'
 
     # TODO: download classifiers in cache memory...
     def MODEL_STORE(self, name) -> Path:
-        return self.MODEL_DIR / f"{name}classifier.ckpt"
-
-    # TODO: replace this with diskcache
-    def get_memory_cache(self):
-        return joblib.Memory(str(self.CACHE_DIR_BASE), verbose=0)
+        return self.PDX_MODEL_DIR / f"{name}classifier.ckpt"
 
 
 settings = _Settings()
```

### Comparing `pydoxtools-0.5.1/pydoxtools/training.py` & `pydoxtools-0.6.0/pydoxtools/training.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 from pydoxtools import file_utils
 from pydoxtools.classifier import pdfClassifier, gen_meta_info_cached, \
     pageClassifier, txt_block_classifier
 from pydoxtools.random_data_generators import TextBlockGenerator
 from pydoxtools.settings import settings
 
 logger = logging.getLogger(__name__)
-memory = settings.get_memory_cache()
 
 
 @functools.lru_cache()
 def load_labeled_webpages():
     trainingfiles = file_utils.get_nested_paths(settings.TRAINING_DATA_DIR, "trainingitem*.parquet")
 
     df = pd.read_parquet(trainingfiles[0])
```

### Comparing `pydoxtools-0.5.1/pydoxtools/visual_document_analysis.py` & `pydoxtools-0.6.0/pydoxtools/visual_document_analysis.py`

 * *Files identical despite different names*

### Comparing `pydoxtools-0.5.1/pydoxtools/webdav_utils.py` & `pydoxtools-0.6.0/pydoxtools/webdav_utils.py`

 * *Files identical despite different names*

### Comparing `pydoxtools-0.5.1/pyproject.toml` & `pydoxtools-0.6.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "pydoxtools"
-version = "0.5.1"
-description = "This library contains a set of tools in order to extract structured information from documents"
+version = "0.6.0"
+description = "This library contains a set of tools in order to extract and synthesize structured information from documents"
 authors = ["thomas meschede <yeusblender@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://pydoxtools.xyntopia.com"
 repository = "https://github.com/xyntopia/pydoxtools"
 documentation = "https://pydoxtools.xyntopia.com"
 keywords = ["AI", "document-analysis", "LLM", "NLP", "ML"]
@@ -25,51 +25,56 @@
 extruct = { optional = true, version = ">=0.9.0" }
 quantulum3 = { optional = true, version = ">=0.7.4" }
 quantities = { optional = true, version = ">=0.12.4" }
 tqdm = { optional = true, version = ">=4.47.0" }
 urlextract = { optional = true, version = ">=1.1.0" }
 pydantic = { version = ">=1.7.2" }
 beautifulsoup4 = { optional = true, version = ">=4.8.0" }
-joblib = ">=1.0.1"
 lxml = { optional = true, version = ">=4.6.2" }
 # stemming is needed for quantulum3
 stemming = { optional = true, version = ">=1.0.1" }
 # TODO: try to replace quantulum with Pint
 Pint = ">=0.16.1"
 # used to "repair" pdfs
 pikepdf = ">=2.10.0"
 # TODO: try to get rid of this and move it only to "development"
 pytorch-lightning = { optional = true, version = ">=1.5.6" }
 pdf2image = { version = "^1.16.0", optional = true }
 Shapely = { version = "^1.8.0", optional = true }
 scikit-learn = { version = "^1.0.2", optional = true }
 spacy = { version = "^3.2.3", optional = true }
-pandas = "^1.4.1"
-hnswlib = { version = "^0.6.2", optional = true }
+pandas = "^2.0.1"
+hnswlib = { version = ">=0.6.2", optional = true }
 networkx = { version = "^2.8.6", optional = true }
-python-magic = { version = "^0.4.27", optional = true } # for fil type identification
+python-magic = { version = "^0.4.27" } # for fil type identification
 openai = { version = "^0.27.4", optional = true }
 python-pptx = { version = "^0.6.21", optional = true }
 # TODO: odp  / open document presentation
 pandoc = { version = "^2.3", optional = true }
 packaging = "^23.0"
 torch = { version = ">=1.12.1", optional = true }
 pytesseract = {version = "^0.3.10", optional = true}
 pyyaml = "^6.0"
+dask = {extras = ["complete"], version = "^2023.4.1", optional = true}
+diskcache = "^5.6.1"
+chardet = "^5.1.0"
+chromadb = {version = "^0.3.23", optional = true}
 
 [tool.poetry.extras]
 # extraction-transformation-load facilities
 etl = ["goose3", "langdetect", "tldextract", "spacy", "pdfminer.six",
     "extruct", "urlextract", "quantulum3", "stemming",
     "quantities", "readability-lxml", "pandas", "beautifulsoup4", "hnswlib",
-    "networkx", "openai", "textract", "pandoc", "python-pptx"
+    "networkx", "openai", "textract", "pandoc", "python-pptx", "dask", "pytesseract"
 ]
 # TODO: rename & regroups extras (e.g. light, medium average or something like that...)
 inference = ["transformers", "scikit-learn", "tqdm", "torch", "pytorch-lightning", "spacy",
-    "beautifulsoup4", "pandas", "urlextract", "hnswlib"]
+    "beautifulsoup4", "pandas", "urlextract", "hnswlib", "chromadb"]
+
+all = ["chromadb"]
 
 [tool.poetry.group.colab]
 optional = true
 
 [tool.poetry.group.colab.dependencies]
 pytest = ">=6.0.1"
 yattag = ">=1.13.2" #for html text coloring
@@ -131,16 +136,16 @@
 evaluate = "^0.4.0"
 pygraphviz = "^1.10"
 mkdocs = "^1.4.2"
 mkdocstrings = {extras = ["crystal", "python"], version = "^0.21.2"}
 mkdocs-material = "^9.1.8"
 
 [build-system]
-requires = ["poetry>=1.1.8"]
-build-backend = "poetry.masonry.api"
+requires = ["poetry-core>=1.0.0"]
+build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 log_cli = true
 log_cli_level = "INFO"
 log_cli_format = "%(asctime)s [%(levelname)8s] %(message)s (%(filename)s:%(lineno)s)"
 log_cli_date_format = "%Y-%m-%d %H:%M:%S"
 testpaths = "tests"
```

### Comparing `pydoxtools-0.5.1/PKG-INFO` & `pydoxtools-0.6.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,43 +1,47 @@
 Metadata-Version: 2.1
 Name: pydoxtools
-Version: 0.5.1
-Summary: This library contains a set of tools in order to extract structured information from documents
+Version: 0.6.0
+Summary: This library contains a set of tools in order to extract and synthesize structured information from documents
 Home-page: https://pydoxtools.xyntopia.com
 License: MIT
 Keywords: AI,document-analysis,LLM,NLP,ML
 Author: thomas meschede
 Author-email: yeusblender@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: all
 Provides-Extra: etl
 Provides-Extra: inference
 Requires-Dist: Pint (>=0.16.1)
 Requires-Dist: Shapely (>=1.8.0,<2.0.0)
 Requires-Dist: appdirs (>=1.4.4)
 Requires-Dist: beautifulsoup4 (>=4.8.0) ; extra == "etl" or extra == "inference"
+Requires-Dist: chardet (>=5.1.0,<6.0.0)
+Requires-Dist: chromadb (>=0.3.23,<0.4.0) ; extra == "inference" or extra == "all"
+Requires-Dist: dask[complete] (>=2023.4.1,<2024.0.0) ; extra == "etl"
+Requires-Dist: diskcache (>=5.6.1,<6.0.0)
 Requires-Dist: extruct (>=0.9.0) ; extra == "etl"
 Requires-Dist: goose3 (>=3.1.6) ; extra == "etl"
-Requires-Dist: hnswlib (>=0.6.2,<0.7.0) ; extra == "etl" or extra == "inference"
-Requires-Dist: joblib (>=1.0.1)
+Requires-Dist: hnswlib (>=0.6.2) ; extra == "etl" or extra == "inference"
 Requires-Dist: langdetect (>=1.0.8) ; extra == "etl"
 Requires-Dist: lxml (>=4.6.2)
 Requires-Dist: networkx (>=2.8.6,<3.0.0) ; extra == "etl"
 Requires-Dist: openai (>=0.27.4,<0.28.0) ; extra == "etl"
 Requires-Dist: packaging (>=23.0,<24.0)
-Requires-Dist: pandas (>=1.4.1,<2.0.0) ; extra == "etl" or extra == "inference"
+Requires-Dist: pandas (>=2.0.1,<3.0.0) ; extra == "etl" or extra == "inference"
 Requires-Dist: pandoc (>=2.3,<3.0) ; extra == "etl"
 Requires-Dist: pdf2image (>=1.16.0,<2.0.0)
 Requires-Dist: pdfminer.six (>=20200726) ; extra == "etl"
 Requires-Dist: pikepdf (>=2.10.0)
 Requires-Dist: pydantic (>=1.7.2)
-Requires-Dist: pytesseract (>=0.3.10,<0.4.0)
+Requires-Dist: pytesseract (>=0.3.10,<0.4.0) ; extra == "etl"
 Requires-Dist: python-magic (>=0.4.27,<0.5.0)
 Requires-Dist: python-pptx (>=0.6.21,<0.7.0) ; extra == "etl"
 Requires-Dist: pytorch-lightning (>=1.5.6) ; extra == "inference"
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: quantities (>=0.12.4) ; extra == "etl"
 Requires-Dist: quantulum3 (>=0.7.4) ; extra == "etl"
 Requires-Dist: readability-lxml (>=0.8.1) ; extra == "etl"
@@ -49,15 +53,15 @@
 Requires-Dist: tqdm (>=4.47.0) ; extra == "inference"
 Requires-Dist: transformers (>=4.17.0) ; extra == "inference"
 Requires-Dist: urlextract (>=1.1.0) ; extra == "etl" or extra == "inference"
 Project-URL: Documentation, https://pydoxtools.xyntopia.com
 Project-URL: Repository, https://github.com/xyntopia/pydoxtools
 Description-Content-Type: text/markdown
 
-🚀 pydoxtools (Python Library) 🚀
+🎩✨📄 pydoxtools (Python Library) 🎩✨📄
 ================================================================================
 
 ![Python](https://img.shields.io/pypi/pyversions/pydoxtools.svg)
 [![PyPI version](https://img.shields.io/pypi/v/pydoxtools.svg)](https://pypi.python.org/pypi/pydoxtools)
 [![Mkdocs](https://img.shields.io/badge/doc-mkdocs-845ed7.svg)](https://pydoxtools.xyntopia.com)
 [![GitHub discussions](https://img.shields.io/badge/discuss-online-845ef7)](https://github.com/xyntopia/pydoxtools/discussions)
 [![GitHub stars](https://img.shields.io/github/stars/xyntopia/pydoxtools)](https://github.com/xyntopia/pydoxtools/stargazers)
@@ -66,148 +70,171 @@
 
 (*WIP*) [Documentation](https://pydoxtools.xyntopia.com)
 
 Pydoxtools is a library that provides a sophisticated interface for reading and
 writing documents, designed to work with AI models such as GPT, Alpaca, and
 Huggingface. It offers functionalities such as:
 
-- Table extraction
-- Vector Index Creation
+- Pipeline management
+- Integration with AI (LLMs and more) models
+- low-resource (PDF) table extraction without configuration and expensive
+  layout detection algorithms!
 - Document analysis and question-answering
+- Support for most of todays document formats
+- Vector index Creation
 - Entity, address identification and more
 - List and keyword extraction
 - Data normalization, translation, and cleaning
 
 The library allows for the creation of complex extraction pipelines
 for batch-processing of documents by defining them as a lazily-executed graph.
 
 ## Installation
 
-While pydoxtools can already be installed through pip. Due to the
-many updates coming in right now, it is right now recommended to use
-the latest version from github as follows:
+### Installing from GitHub
+
+While pydoxtools can already be installed through pip, due to the
+many updates coming in right now, it is currently recommended to use
+the latest version from GitHub as follows:
 
     pip install -U "pydoxtools[etl,inference] @ git+https://github.com/xyntopia/pydoxtools.git"
 
-Pydoxtools can be also be installed through pip which will become the recommended
+### Installing from PyPI
+
+Pydoxtools can also be installed through pip, which will become the recommended
 method once it becomes more stable:
 
     pip install -U pydoxtools[etl,inference]
 
-For loading additional file formats (docx, odt, epub) and images, checkout
+For loading additional file formats (docx, odt, epub) and images, check out
 the additional > [Installation Options](#installation-options) <.
 
-## Teaser
+## 🚀 Teaser 🚀
+
+Experience a new level of convenience and efficiency in handling
+documents with Pydoxtools, and reimagine your data extraction pipelines!
 
-Experience a new level of convenience and efficiency in handling documents with Pydoxtools, and reimagine your data
-extraction pipelines! 🎩✨📄.
+In this teaser, we'll demonstrate how to create a document, extract
+tables, and ask questions using AI models:
 
-    import pydoxtools as pdx
+```python
+import pydoxtools as pdx
 
-    # create a document from a file, string, bytestring, file-like object
-    # or even an url:
-    doc = pdx.Document(
-        "https://www.raspberrypi.org/app/uploads/2012/12/quick-start-guide-v1.1.pdf", 
-        document_type=".pdf"
-    )
+# Create a document from various sources: file, string, bytestring, file-like object, or URL
+doc = pdx.Document("https://www.raspberrypi.org/app/uploads/2012/12/quick-start-guide-v1.1.pdf")
 
-You can easily extract a large number of pre-defined information
-about your document. To get a list of possible operators use `print(doc.x_funcs)`.
+# List available extraction functions
+print(doc.x_funcs)
 
-    # extract tables from the pdf as a pandas dataframe:
-    print(doc.tables_df)
+# get all tables from a single document:
+print(doc.tables)
 
-Some extraction operations need input when called. The model that should be
-used for the question answering can be specified through doc.config() and can be any
-model from huggingface.
+# Extract the first 20 tables that we can find in a directory (this might take a while,
+# make sure, to only choose a small directory for testing purposes)
+docs = pdx.DocumentBag("./my_directory_with_documents", forgiving_extracts=True)
+print(docs.bag_apply(["tables_df", "filename"]).take(20))
 
-    # ask a question about the document, using Q&A Models (questionas answered locally!):
-    print(doc.answers(["how much ram does it have?"]))
+# Ask a question about the documents using a local Q&A model
+print(doc.answers(["how much ram does it have?"]))
+# Or only ask about the documents tables (or any other extracted information):
+print(doc.answers(["how much ram does it have?"], "tables"))
 
-others need an API key installed, if it refers to an online service.
+# To use ChatGPT for question-answering, set the API key as an environment variable:
+# OPENAI_API_KEY="sk ...."
+# Then, ask questions about the document using ChatGPT
+print(doc.chat_answers(["What is the target group of this document?"])[0].content)
+print(doc.chat_answers(["Answer if a 5-year old would be able to follow these instructions?"])[0].content)
+```
 
-    # ask a question about the document, using ChatGPT (we need the API key for ChatGPT!):
-    # load the API key into an environment variable like this: 
-    #   
-    # OPENAI_API_KEY="sk ...."
-    # 
-    # Do **NOT** use the key in your code. This could potentially cost you a lot of money...
-    print(doc.chat_answers(["What is the target group of this document?"])[0].content)
-    print(doc.chat_answers(["Answer if a 5-year old would be able to follow these instructions?"])[0].content)
+With Pydoxtools, you can easily access and process your documents, perform various extractions,
+and utilize AI models for more advanced analysis.
 
-## Features
+## Some Features in More Detail
 
-### Large pipelines
+### Large Pipelines
 
-Pydoxtools main feature is the ability to mix LLMs and other
-AI models in large, composable and customizable pipelines.
-As a teaser, check out this pipeline for *.png images from the repository including
-OCR, keyword extraction, vectorization and more. In this pipeline:
+Pydoxtools' main feature is the ability to mix LLMs and other
+AI models in large, composable, and customizable pipelines.
+Using pipelines comes with the slight disadvantage that it
+can be more challenging to add type hints to the code.
+However, using pipelines decouples all parts of your code,
+allowing all operators to work independently. This
+makes it easy to run the pipeline in a distributed setting for big data
+and enables easy, lazy evaluation. Additionally,
+mixing different LLM logics together becomes much easier.
+
+Check out how Pydoxtools' `Document` class mixes pipelines for each individual file type:
 
 - Every node in an ellipse can be called as an attribute of the document-analysis pipeline.
-- Every execution-path is lazily executed throughout the entire graph.
-- Every node is cached by default (can be turned off).
+- Every execution path is lazily executed throughout the entire graph.
+- Every node is cached by default (but can be turned off).
 - Every piece of this pipeline can be replaced by a customized version.
 
-<img src="http://pydoxtools.xyntopia.com/images/document_logic_png.svg" width="500">
+As an example, consider this pipeline for *.png images from the repository,
+which includes OCR, keyword extraction, vectorization, and more:
+
+![png pipeline](http://pydoxtools.xyntopia.com/images/document_logic_.png.svg)
 
-Pipelines can be mixed, partially overwritten and extended which gives you a lot of possibilities
-to extend and adapt the functionality for your specific use-case.
+Pipelines can be mixed, partially overwritten, and extended, giving you a lot of possibilities
+to extend and adapt the functionality for your specific use case.
 
-Find out more about it in the [documentation](http://pydoxtools.xyntopia.com/reference/#pydoxtools.document.Document)
+To learn more about Pydoxtools' large pipelines feature, please refer to
+the [documentation](http://pydoxtools.xyntopia.com/reference/#pydoxtools.document.Document).
 
-#### Pipeline configuration
+#### Pipeline Configuration
 
 Pipelines can be configured. For example the local model used for
 question answering can be selected like this:
 
     doc = Document(fobj="./data/PFR-PR23_BAT-110__V1.00_.pdf"))
             .config(qam_model_id='bert-large-uncased-whole-word-masking-finetuned-squad')
 
 where "qam_model_id" can be any model from huggingface for question answering.
 
     TODO: document how to configure a pipeline
 
-### PDF table extraction algorithms
+### PDF Table Extraction Algorithms
 
 The library features its own sophisticated Table extraction algorithm which is benchmarked
-against a large pdf table dataset. In contrast to most other table extraction frameworks
-out there it does not require:
+against a large pdf table dataset. In contrast to how most "classical" table extraction
+algorithms work, it doesn't require:
 
 - extensive configuration
-- no expensive deep neural networks which need a GPU
+- no expensive deep neural networks for table area recognition which need a GPU and
+  a lot of memory/CPU requirements
 
 This makes it possible to run analysis on PDF files with pydoxtools on CPU with
 very limited resources!
 
 ### TODO: Describe more of the features here...
 
 ## Use Cases
 
-- analyze documents using any model from huggingface...
+- create new documents from unstructured information
+- analyze documents using any model from huggingface
 - analyze documents using a custom model
 - download a pdf from URL
 - generate document keywords
 - extract tables
 - download document from URL "manually" and then feed to document
 - extract addresses
 - extract addresses and use this information for the qam
 - ingest documents into a vector db
 
 ## Installation Options
 
-### Supporting *.docx, *.odt, *.epub
+### Supporting \*.docx, \*.odt, \*.epub
 
 In order to be able to load docx, odt and rtf files, you have to install pandoc.
 Right now, the python pandoc library does not work with pandoc version > 3.0.0. It
 is therefore recommended to install a version from here for your OS:
 
 https://github.com/jgm/pandoc/releases/tag/2.19.2
 
-### Image OCR support
+### Image OCR Support
 
 Pydoxtools can automatically analyze images as well, makin use of
 [OCR](https://en.wikipedia.org/wiki/Optical_character_recognition).
 In order to be able to use this, install tesseract on your system:
 
 Under linux this looks like the following:
 
@@ -230,11 +257,13 @@
 
 You can check the compatibility using the following tool in a venv environment in a production
 setting:
 
     pip install pip-licenses
     pip-licenses | grep -Ev 'MIT License|BSD License|Apache Software License|Python Software Foundation License|Apache 2.0|MIT|Apache License 2.0|hnswlib|Pillow|new BSD|BSD'
 
-## list of libraries, that this project is based on:
+### Dependencies
+
+Here is a list of Libraries, that this project is based on:
 
 [list](poetry.lock)
```

