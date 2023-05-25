# Comparing `tmp/openai_parallel_toolkit-0.4-py3-none-any.whl.zip` & `tmp/openai_parallel_toolkit-0.4.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,21 @@
-Zip file size: 18474 bytes, number of entries: 19
+Zip file size: 18844 bytes, number of entries: 19
 -rw-r--r--  2.0 unx      213 b- defN 23-May-17 02:40 openai_parallel_toolkit/__init__.py
 -rw-r--r--  2.0 unx       20 b- defN 23-May-17 01:58 openai_parallel_toolkit/config.py
 -rw-r--r--  2.0 unx      113 b- defN 23-May-17 12:36 openai_parallel_toolkit/api/__init__.py
 -rw-r--r--  2.0 unx     1769 b- defN 23-May-17 12:36 openai_parallel_toolkit/api/api.py
--rw-r--r--  2.0 unx     5810 b- defN 23-May-23 11:48 openai_parallel_toolkit/api/keys.py
--rw-r--r--  2.0 unx     2906 b- defN 23-May-18 11:47 openai_parallel_toolkit/api/request.py
+-rw-r--r--  2.0 unx     5809 b- defN 23-May-23 12:55 openai_parallel_toolkit/api/keys.py
+-rw-r--r--  2.0 unx     3034 b- defN 23-May-25 08:28 openai_parallel_toolkit/api/request.py
 -rw-r--r--  2.0 unx       95 b- defN 23-May-17 01:02 openai_parallel_toolkit/core/__init__.py
--rw-r--r--  2.0 unx     4575 b- defN 23-May-17 08:17 openai_parallel_toolkit/core/main.py
+-rw-r--r--  2.0 unx     4532 b- defN 23-May-25 08:13 openai_parallel_toolkit/core/main.py
 -rw-r--r--  2.0 unx     4852 b- defN 23-May-18 11:47 openai_parallel_toolkit/core/multithread.py
 -rw-r--r--  2.0 unx      214 b- defN 23-May-17 12:36 openai_parallel_toolkit/utils/__init__.py
 -rw-r--r--  2.0 unx     1042 b- defN 23-May-18 11:32 openai_parallel_toolkit/utils/logger.py
--rw-r--r--  2.0 unx     4114 b- defN 23-May-23 04:55 openai_parallel_toolkit/utils/reader.py
+-rw-r--r--  2.0 unx     4077 b- defN 23-May-25 08:22 openai_parallel_toolkit/utils/reader.py
 -rw-r--r--  2.0 unx      913 b- defN 23-May-17 11:15 openai_parallel_toolkit/utils/token.py
 -rw-r--r--  2.0 unx      753 b- defN 23-May-18 11:47 openai_parallel_toolkit/utils/tqdm.py
--rw-r--r--  2.0 unx     1063 b- defN 23-May-23 12:01 openai_parallel_toolkit-0.4.dist-info/LICENSE
--rw-r--r--  2.0 unx    13578 b- defN 23-May-23 12:01 openai_parallel_toolkit-0.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-23 12:01 openai_parallel_toolkit-0.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       24 b- defN 23-May-23 12:01 openai_parallel_toolkit-0.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1773 b- defN 23-May-23 12:01 openai_parallel_toolkit-0.4.dist-info/RECORD
-19 files, 43919 bytes uncompressed, 15496 bytes compressed:  64.7%
+-rw-r--r--  2.0 unx     1063 b- defN 23-May-25 08:48 openai_parallel_toolkit-0.4.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx    14604 b- defN 23-May-25 08:48 openai_parallel_toolkit-0.4.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-25 08:48 openai_parallel_toolkit-0.4.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       24 b- defN 23-May-25 08:48 openai_parallel_toolkit-0.4.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1783 b- defN 23-May-25 08:48 openai_parallel_toolkit-0.4.1.dist-info/RECORD
+19 files, 45002 bytes uncompressed, 15846 bytes compressed:  64.8%
```

## zipnote {}

```diff
@@ -36,23 +36,23 @@
 
 Filename: openai_parallel_toolkit/utils/token.py
 Comment: 
 
 Filename: openai_parallel_toolkit/utils/tqdm.py
 Comment: 
 
-Filename: openai_parallel_toolkit-0.4.dist-info/LICENSE
+Filename: openai_parallel_toolkit-0.4.1.dist-info/LICENSE
 Comment: 
 
-Filename: openai_parallel_toolkit-0.4.dist-info/METADATA
+Filename: openai_parallel_toolkit-0.4.1.dist-info/METADATA
 Comment: 
 
-Filename: openai_parallel_toolkit-0.4.dist-info/WHEEL
+Filename: openai_parallel_toolkit-0.4.1.dist-info/WHEEL
 Comment: 
 
-Filename: openai_parallel_toolkit-0.4.dist-info/top_level.txt
+Filename: openai_parallel_toolkit-0.4.1.dist-info/top_level.txt
 Comment: 
 
-Filename: openai_parallel_toolkit-0.4.dist-info/RECORD
+Filename: openai_parallel_toolkit-0.4.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## openai_parallel_toolkit/api/keys.py

```diff
@@ -26,15 +26,15 @@
         If the instance doesn't exist, create it. If it does, return the existing instance.
         """
         if not cls._instance:
             if not api_keys:
                 if config_path:
                     api_keys = read_keys(config_path)
                 else:
-                    raise ValueError("No OpenAi keys available")
+                    raise Exception("No OpenAi keys available")
             if set_api_base:
                 api_base = read_api_base(config_path)
                 if api_base:
                     openai.api_base = api_base
             cls._instance = super().__new__(cls)
             cls._instance.__init_once(api_keys)
         cls.check_key_available(cls._instance)
```

## openai_parallel_toolkit/api/request.py

```diff
@@ -1,8 +1,10 @@
 import logging
+import random
+import time
 
 import openai
 
 # Import related local modules
 from .api import OpenAIModel
 from .keys import APIKeyManager
 from ..config import LOG_LABEL
@@ -28,14 +30,15 @@
     attempts = 0  # Initialize attempts
 
     while attempts < max_retries:
         key = openai.api_key  # Get the current API key
 
         try:
             # Attempt to generate a completion
+            time.sleep(random.uniform(0, 0.2))  # Sleep for 0-0.2s seconds to avoid infinite requests
             completion = openai_model.generate()
             break
         except Exception as e:
             # Handle different types of errors
             if "exceeded your current quota" in str(e) or "<empty message>" in str(e):
                 # If the quota has been exceeded, remove the key and try again
                 key_manager.remove_key(key)
```

## openai_parallel_toolkit/core/main.py

```diff
@@ -1,12 +1,10 @@
 import multiprocessing  # For accessing the number of CPUs
 from abc import ABC, abstractmethod  # For defining abstract base classes
 
-from py._io.capture import TextIO
-
 from .multithread import multi_thread_run  # Importing the local function for multithreaded execution
 
 
 class ParallelToolkit(ABC):
     """
     Abstract base class for parallel processing tools.
     This class provides a template for tools that process files in parallel.
@@ -51,15 +49,15 @@
         self.max_workers = num_threads
         self.name = name
         self.file_count = file_count
         self.config_path = config_path
 
     @staticmethod
     @abstractmethod
-    def process_input(file: TextIO):
+    def process_input(file):
         """
         Abstract method to process an input file.
         This method should read the file and return the file content.
         Must be implemented in a subclass.
 
         Args:
             file (TextIO): Read byte stream object
```

## openai_parallel_toolkit/utils/reader.py

```diff
@@ -36,29 +36,29 @@
         dict: A dictionary mapping filenames (without extension) to processed data. Returns None if there's no data to process.
     """
     skipped_files_count = 0
     if output_path is not None:
         output_files = read_files(output_path)
         output_files_basename = [os.path.splitext(f)[0] for f in output_files]
         files = [f for f in read_files(input_path) if os.path.splitext(f)[0] not in output_files_basename][:file_count]
-        skipped_files_count = len(output_files)  # 计算已经跳过的文件数
+        skipped_files_count = len(output_files)
         logging.info(f"{LOG_LABEL}Output path: {output_path} Skipped files count: {skipped_files_count}")
     else:
         files = [
                     f for f in os.listdir(input_path) if
                     os.path.isfile(os.path.join(input_path, f)) and f[0] != "." and not os.path.splitext(f)[
                         0].startswith(
                         ".")
                 ][:file_count]
 
     data = {}
     for file in files:
         file_path = os.path.join(input_path, file)
         with open(file_path, 'r') as f:
-            file_name = os.path.splitext(file)[0]  # 获取文件名，不包含后缀
+            file_name = os.path.splitext(file)[0]
             data[file_name] = process_input(f)
     if len(data) == 0:
         if skipped_files_count != 0:
             logging.info(f"{LOG_LABEL}All files have been processed: {input_path},file count: {skipped_files_count}")
             return None
         logging.error(f"{LOG_LABEL}input_path error, No data to process:{input_path}")
         return None
@@ -95,15 +95,15 @@
     Returns:
         str: The 'api_keys' field from the configuration file.
     """
     with open(config_path, 'r') as f:
         config = json.load(f)
         if 'api_keys' in config:
             return config['api_keys']
-        return []
+        raise Exception("No OpenAi keys available")
 
 
 def read_api_base(config_path):
     """
     Read and return the 'api_base' field from a JSON configuration file.
 
     Args:
```

### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

## Comparing `openai_parallel_toolkit-0.4.dist-info/LICENSE` & `openai_parallel_toolkit-0.4.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `openai_parallel_toolkit-0.4.dist-info/METADATA` & `openai_parallel_toolkit-0.4.1.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,42 +1,44 @@
 Metadata-Version: 2.1
 Name: openai-parallel-toolkit
-Version: 0.4
+Version: 0.4.1
 Summary: OpenAI-Parallel-Toolkit is a Python library for handling multiple OpenAI API keys and parallel tasks. It provides API key rotation, multithreading for faster task execution, and utility functions to boost your OpenAI integration. Ideal for efficient large-scale OpenAI usage.
 Home-page: https://github.com/CZT0/OpenAI-Parallel-Toolkit
 Author: Jellow
 Author-email: dvdx@foxmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: openai
 Requires-Dist: colorlog
 Requires-Dist: tqdm
 Requires-Dist: tiktoken
-Requires-Dist: py
+Requires-Dist: regex
 
 # OpenAI Parallel Toolkit
 
 The OpenAI Parallel Toolkit is a specialized Python library crafted to proficiently manage multiple OpenAI API keys and
 effectively supervise parallel tasks. It comes packed with features that cater to API key rotation, accelerating task
 execution through multithreading, and provides an assortment of utility functions to optimize your OpenAI integration.
 This toolkit serves as an efficient solution for extensive, high-performance OpenAI usage.
 
-### function
+### Function
 
-- [x] Support rotating multiple OpenAI API keys to maximize usage rate
-- [x] Support parallel processing with multiple threads
-- [x] Support resuming file output (skipping duplicate files)
-- [x] Provides the function of splitting long text by token count
+1. &#x2705; Enables automated OpenAI API key rotation when usage limit is reached, with built-in error handling and
+   auto-retry mechanisms.
+2. &#x2705; Provides a method for proxy access to OpenAI services in China.
+3. &#x2705; Supports parallel processing for both API and file operations, optimizing throughput and efficiency.
+4. &#x2705; Features a file processing resumption function, effectively skipping previously processed files.
+5. &#x2705; Includes a utility to split long text into specified length segments, following the token count method used
+   in GPT-3.5 model.
 
 ## Context
 
 In the field of natural language processing (NLP), Generative Pretrained Transformer (GPT) models have revolutionized
 the methodology of processing and comprehending textual data. They've equipped us with the ability to accomplish a vast
 array of tasks such as data annotation, processing, and generating text with a human-like semblance. However, employing
 GPT models for large-scale or time-critical tasks can often present unique hurdles.
@@ -146,43 +148,64 @@
     "your api key 2",
     "your api key 3"
   ],
   "api_base": "https://api.openai.com/v1"
 }
 ```
 
-For users in China or other regions where accessing OpenAI is challenging, it is recommended to deploy your own proxy
-and pass in `api_base`. For more details, refer to this
-project: [OpenAI Proxy](https://github.com/justjavac/openai-proxy). I provide a method using Cloudflare's proxy, which
-allows up to 100,000 free calls per day.
+### Troubleshooting: Progress Bar Not Moving
+
+If you're running the program and the progress bar isn't showing any progress, it's possible that you're experiencing
+connectivity issues, particularly if you're in China or another region where accessing OpenAI is challenging.
+
+To resolve this issue, we recommend deploying your own proxy and passing in `api_base`. You can refer to
+the [OpenAI Proxy](https://github.com/justjavac/openai-proxy) project for more details.
+
+This project provides a method that uses Cloudflare's proxy, which allows up to 100,000 free calls per day. This can
+effectively help bypass the connectivity issue and ensure the smooth running of your program.
+
+Remember to replace the project link with the actual URL for your specific situation.
 
 If you don't need the api base field, you can leave it unwritten to the config.json file.
 
 ## Parallel processing of one file
 
 If you have a single file that is too long, you can split it into smaller segments, process them in parallel, and then
 merge the results in order. You can use the `multi_process_one` function for this purpose. Here's an example of how to
 use it in the `process_data` function:
 
+Here's how you can add this information into your markdown documentation:
+
+---
+
+## Usage: Processing Data
+
+In the Python function `multi_process_one`, `data` is a list of tuples. Here's an example:
+
 ```python
 from openai_parallel_toolkit import multi_process_one, Gpt35Turbo
 
 
 @staticmethod
 def process_data(data):
-    # data = [('hello1', 'world'), ('hello2', 'world'), ('hello3', 'world'), ('hello4', 'world'), ('hello5', 'world')]
+    # data example: 
+    # [('hello1', 'world'), ('hello2', 'world'), ('hello3', 'world'), 
+    #  ('hello4', 'world'), ('hello5', 'world')]
     results = multi_process_one(data=data, openai_model_class=Gpt35Turbo, temperature=0.7)
     return results
-
 ```
 
-It is important to note that in the `data` list, you need to pass the prompt as the first element and the content as the
-second element to ensure the correctness of the results. The remaining parameters should be passed in the order of the
-Gpt35Turbo (or your custom model) with the prompt and content parameters. If you are unsure, you can refer to the source
-code of the `multi_process_one` function.
+It's important to note that in the `data` list, you need to pass the prompt as the first element and the content as the
+second element of each tuple. This is necessary to ensure the correctness of the results.
+
+Any remaining parameters should be passed in the order defined by the `Gpt35Turbo` (or your custom model) after the
+prompt and content parameters.
+
+If you're unsure about the parameters, you can refer to the source code of the `multi_process_one` function for
+additional clarity.
 
 ## Customizing OpenAI API Interface
 
 Currently, the OpenAI API interfaces supported are:
 
 - GPT-3.5
```

## Comparing `openai_parallel_toolkit-0.4.dist-info/RECORD` & `openai_parallel_toolkit-0.4.1.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 openai_parallel_toolkit/__init__.py,sha256=GOaSwAXBRlbKqwi42SH2g6G3OOJBs_cyCTPYwv7JY6A,213
 openai_parallel_toolkit/config.py,sha256=UvWwqK1cxCx4XId6pswW4jkSF1XDozEg58RftfY8yxU,20
 openai_parallel_toolkit/api/__init__.py,sha256=eabIIe9ATUy6StxNz50Ul9Dr7iPPuc3I7ebAyGWvNLQ,113
 openai_parallel_toolkit/api/api.py,sha256=kePe00bV_6M9OL0-TvvYA_Uu65Riv4YmSr4pXVFA_E4,1769
-openai_parallel_toolkit/api/keys.py,sha256=baQWRfNl3e0p1m1oem1H5GfBRhCLBSnNBaPpSZuaccY,5810
-openai_parallel_toolkit/api/request.py,sha256=zyFWK7syojup7QUK6ZCJpnMDiEoVJaCZtDCtFhwlC9w,2906
+openai_parallel_toolkit/api/keys.py,sha256=RB9BmU7Qth3QIUWP30KXcfgmyblWVFYUnH0uB538ISs,5809
+openai_parallel_toolkit/api/request.py,sha256=75V3R79jE055WovuwQp7Pp29Ib_NUCDbFFqYVyaBA0w,3034
 openai_parallel_toolkit/core/__init__.py,sha256=bgIhoLSNMQAno1ICwhMfEhEZQMHqVCwEcnKvxZuXd70,95
-openai_parallel_toolkit/core/main.py,sha256=Q-8ixhJLjsg0EFDMSFJvnoaEA7O2RaoEVaGNaEFknv0,4575
+openai_parallel_toolkit/core/main.py,sha256=omai73kazjZ_8iHOaayG0jlfyPxwGUc8tYQ3M8bhQ2g,4532
 openai_parallel_toolkit/core/multithread.py,sha256=v8GPaJ7Wukxfv43i1szqreOvtCgzbK6yjh_PkiZ3qnY,4852
 openai_parallel_toolkit/utils/__init__.py,sha256=zgDb7rU1behG7hcrbLgxGOen_ojX_hUuBn5t9jnr3nk,214
 openai_parallel_toolkit/utils/logger.py,sha256=6PnPaAsBTr0PnA8tslgR0L7WSQcMZF08e8iqv-_Tvjo,1042
-openai_parallel_toolkit/utils/reader.py,sha256=UzPqVFjH5udZpyGwoeI8sk4JdJoVmn-L830xB3U4h0o,4114
+openai_parallel_toolkit/utils/reader.py,sha256=3V0ZSTwLiJbpUVERTqDFySSN41Bcd94Mm4RaqIcp62Q,4077
 openai_parallel_toolkit/utils/token.py,sha256=lN3oasNGcHesWjoBiIfn5hMwjPYb3wTcRFUCIFtNY4k,913
 openai_parallel_toolkit/utils/tqdm.py,sha256=Xc4ymtGfZzCdbmWdqNR6bAoGDWQWOtjQqvNpvrxv-KY,753
-openai_parallel_toolkit-0.4.dist-info/LICENSE,sha256=GcBhJWMnrpUPC70Dvfs6cFG8fLIitA0WwucEgQjGWcw,1063
-openai_parallel_toolkit-0.4.dist-info/METADATA,sha256=4IZl3miOFtCgeJr7b2cAsa3b6qj1Xcr_opjA-IIbVrI,13578
-openai_parallel_toolkit-0.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-openai_parallel_toolkit-0.4.dist-info/top_level.txt,sha256=EaHQWFuNRtse4G2kzDTEMstiiaGFy0zIAHBJ0Mm9a_E,24
-openai_parallel_toolkit-0.4.dist-info/RECORD,,
+openai_parallel_toolkit-0.4.1.dist-info/LICENSE,sha256=GcBhJWMnrpUPC70Dvfs6cFG8fLIitA0WwucEgQjGWcw,1063
+openai_parallel_toolkit-0.4.1.dist-info/METADATA,sha256=s8F2KMxh_kQRJoU-gwE2m6JKsppUf8kfgrKAB_eJ7ak,14604
+openai_parallel_toolkit-0.4.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+openai_parallel_toolkit-0.4.1.dist-info/top_level.txt,sha256=EaHQWFuNRtse4G2kzDTEMstiiaGFy0zIAHBJ0Mm9a_E,24
+openai_parallel_toolkit-0.4.1.dist-info/RECORD,,
```

