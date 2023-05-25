# Comparing `tmp/mona-openai-0.0.3.tar.gz` & `tmp/mona-openai-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mona-openai-0.0.3.tar", last modified: Thu May  4 06:53:27 2023, max compression
+gzip compressed data, was "mona-openai-0.0.4.tar", last modified: Thu May 25 06:03:54 2023, max compression
```

## Comparing `mona-openai-0.0.3.tar` & `mona-openai-0.0.4.tar`

### file list

```diff
@@ -1,31 +1,40 @@
-drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-05-04 06:53:27.363293 mona-openai-0.0.3/
--rw-r--r--   0 itaibarsinai   (501) staff       (20)    11356 2023-04-04 12:33:03.000000 mona-openai-0.0.3/LICENSE
--rw-r--r--   0 itaibarsinai   (501) staff       (20)     8665 2023-05-04 06:53:27.363069 mona-openai-0.0.3/PKG-INFO
--rw-r--r--   0 itaibarsinai   (501) staff       (20)     8071 2023-05-04 03:41:54.000000 mona-openai-0.0.3/README.md
-drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-05-04 06:53:27.360457 mona-openai-0.0.3/mona_openai/
--rw-r--r--   0 itaibarsinai   (501) staff       (20)       77 2023-05-04 03:41:54.000000 mona-openai-0.0.3/mona_openai/__init__.py
-drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-05-04 06:53:27.361741 mona-openai-0.0.3/mona_openai/analysis/
--rw-r--r--   0 itaibarsinai   (501) staff       (20)     1192 2023-04-04 12:33:03.000000 mona-openai-0.0.3/mona_openai/analysis/analysis.py
--rw-r--r--   0 itaibarsinai   (501) staff       (20)     2693 2023-04-04 12:33:03.000000 mona-openai-0.0.3/mona_openai/analysis/privacy.py
--rw-r--r--   0 itaibarsinai   (501) staff       (20)      381 2023-04-04 12:33:03.000000 mona-openai-0.0.3/mona_openai/analysis/profanity.py
--rw-r--r--   0 itaibarsinai   (501) staff       (20)     3748 2023-04-04 12:33:03.000000 mona-openai-0.0.3/mona_openai/analysis/textual.py
-drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-05-04 06:53:27.361943 mona-openai-0.0.3/mona_openai/endpoints/
--rw-r--r--   0 itaibarsinai   (501) staff       (20)     1786 2023-05-04 03:41:54.000000 mona-openai-0.0.3/mona_openai/endpoints/completion.py
--rw-r--r--   0 itaibarsinai   (501) staff       (20)      167 2023-04-04 12:33:03.000000 mona-openai-0.0.3/mona_openai/exceptions.py
--rw-r--r--   0 itaibarsinai   (501) staff       (20)     1379 2023-04-04 12:33:03.000000 mona-openai-0.0.3/mona_openai/mona_client.py
--rw-r--r--   0 itaibarsinai   (501) staff       (20)    13259 2023-05-04 03:41:54.000000 mona-openai-0.0.3/mona_openai/mona_openai.py
-drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-05-04 06:53:27.362598 mona-openai-0.0.3/mona_openai/util/
--rw-r--r--   0 itaibarsinai   (501) staff       (20)     1224 2023-04-04 12:33:03.000000 mona-openai-0.0.3/mona_openai/util/func_util.py
--rw-r--r--   0 itaibarsinai   (501) staff       (20)      494 2023-04-04 12:33:03.000000 mona-openai-0.0.3/mona_openai/util/math.py
--rw-r--r--   0 itaibarsinai   (501) staff       (20)      971 2023-04-04 12:33:03.000000 mona-openai-0.0.3/mona_openai/util/validation_util.py
-drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-05-04 06:53:27.361194 mona-openai-0.0.3/mona_openai.egg-info/
--rw-r--r--   0 itaibarsinai   (501) staff       (20)     8665 2023-05-04 06:53:27.000000 mona-openai-0.0.3/mona_openai.egg-info/PKG-INFO
--rw-r--r--   0 itaibarsinai   (501) staff       (20)      610 2023-05-04 06:53:27.000000 mona-openai-0.0.3/mona_openai.egg-info/SOURCES.txt
--rw-r--r--   0 itaibarsinai   (501) staff       (20)        1 2023-05-04 06:53:27.000000 mona-openai-0.0.3/mona_openai.egg-info/dependency_links.txt
--rw-r--r--   0 itaibarsinai   (501) staff       (20)       42 2023-05-04 06:53:27.000000 mona-openai-0.0.3/mona_openai.egg-info/requires.txt
--rw-r--r--   0 itaibarsinai   (501) staff       (20)       12 2023-05-04 06:53:27.000000 mona-openai-0.0.3/mona_openai.egg-info/top_level.txt
--rw-r--r--   0 itaibarsinai   (501) staff       (20)      818 2023-05-04 06:53:09.000000 mona-openai-0.0.3/pyproject.toml
--rw-r--r--   0 itaibarsinai   (501) staff       (20)       41 2023-05-04 06:52:57.000000 mona-openai-0.0.3/requirements.txt
--rw-r--r--   0 itaibarsinai   (501) staff       (20)       38 2023-05-04 06:53:27.363334 mona-openai-0.0.3/setup.cfg
-drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-05-04 06:53:27.362741 mona-openai-0.0.3/tests/
--rw-r--r--   0 itaibarsinai   (501) staff       (20)    11664 2023-05-04 03:41:54.000000 mona-openai-0.0.3/tests/test_completion.py
+drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-05-25 06:03:54.948670 mona-openai-0.0.4/
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)    11356 2023-04-04 12:33:03.000000 mona-openai-0.0.4/LICENSE
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)     9757 2023-05-25 06:03:54.948351 mona-openai-0.0.4/PKG-INFO
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)     9162 2023-05-25 05:50:33.000000 mona-openai-0.0.4/README.md
+drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-05-25 06:03:54.943688 mona-openai-0.0.4/mona_openai/
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)       77 2023-05-04 03:41:54.000000 mona-openai-0.0.4/mona_openai/__init__.py
+drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-05-25 06:03:54.945368 mona-openai-0.0.4/mona_openai/analysis/
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)     3613 2023-05-25 05:50:33.000000 mona-openai-0.0.4/mona_openai/analysis/privacy.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)      304 2023-05-25 05:50:33.000000 mona-openai-0.0.4/mona_openai/analysis/profanity.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)     3121 2023-05-25 05:50:33.000000 mona-openai-0.0.4/mona_openai/analysis/textual.py
+drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-05-25 06:03:54.946154 mona-openai-0.0.4/mona_openai/endpoints/
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)     7675 2023-05-25 05:50:33.000000 mona-openai-0.0.4/mona_openai/endpoints/chat_completion.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)     5091 2023-05-25 05:50:33.000000 mona-openai-0.0.4/mona_openai/endpoints/completion.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)     4792 2023-05-25 05:50:33.000000 mona-openai-0.0.4/mona_openai/endpoints/endpoint_wrapping.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)      792 2023-05-25 05:50:33.000000 mona-openai-0.0.4/mona_openai/endpoints/wrapping_getter.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)      167 2023-04-04 12:33:03.000000 mona-openai-0.0.4/mona_openai/exceptions.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)     1379 2023-04-04 12:33:03.000000 mona-openai-0.0.4/mona_openai/mona_client.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)    14956 2023-05-25 05:50:33.000000 mona-openai-0.0.4/mona_openai/mona_openai.py
+drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-05-25 06:03:54.947427 mona-openai-0.0.4/mona_openai/util/
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)      944 2023-05-11 08:33:47.000000 mona-openai-0.0.4/mona_openai/util/async_util.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)      675 2023-05-11 08:33:47.000000 mona-openai-0.0.4/mona_openai/util/func_util.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)     1177 2023-05-25 05:50:33.000000 mona-openai-0.0.4/mona_openai/util/oop_util.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)      364 2023-05-25 05:50:33.000000 mona-openai-0.0.4/mona_openai/util/openai_util.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)     3788 2023-05-25 05:50:33.000000 mona-openai-0.0.4/mona_openai/util/stream_util.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)      776 2023-05-25 05:50:33.000000 mona-openai-0.0.4/mona_openai/util/tokens_util.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)      971 2023-04-04 12:33:03.000000 mona-openai-0.0.4/mona_openai/util/validation_util.py
+drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-05-25 06:03:54.944664 mona-openai-0.0.4/mona_openai.egg-info/
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)     9757 2023-05-25 06:03:54.000000 mona-openai-0.0.4/mona_openai.egg-info/PKG-INFO
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)      925 2023-05-25 06:03:54.000000 mona-openai-0.0.4/mona_openai.egg-info/SOURCES.txt
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)        1 2023-05-25 06:03:54.000000 mona-openai-0.0.4/mona_openai.egg-info/dependency_links.txt
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)       51 2023-05-25 06:03:54.000000 mona-openai-0.0.4/mona_openai.egg-info/requires.txt
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)       12 2023-05-25 06:03:54.000000 mona-openai-0.0.4/mona_openai.egg-info/top_level.txt
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)      818 2023-05-25 05:54:16.000000 mona-openai-0.0.4/pyproject.toml
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)       50 2023-05-11 08:33:47.000000 mona-openai-0.0.4/requirements.txt
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)       38 2023-05-25 06:03:54.948715 mona-openai-0.0.4/setup.cfg
+drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-05-25 06:03:54.948138 mona-openai-0.0.4/tests/
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)    17351 2023-05-25 05:50:33.000000 mona-openai-0.0.4/tests/test_chat_completion.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)    19272 2023-05-25 05:50:33.000000 mona-openai-0.0.4/tests/test_completion.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)     1607 2023-05-25 05:50:33.000000 mona-openai-0.0.4/tests/test_privacy_analyzer.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)      852 2023-05-25 05:50:33.000000 mona-openai-0.0.4/tests/test_textual_analyzer.py
```

### Comparing `mona-openai-0.0.3/LICENSE` & `mona-openai-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mona-openai-0.0.3/PKG-INFO` & `mona-openai-0.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mona-openai
-Version: 0.0.3
+Version: 0.0.4
 Summary: Integration client for monitoring OpenAI usage with Mona
 Author-email: Itai Bar Sinai <itai@monalabs.io>
 Project-URL: Homepage, https://github.com/monalabs/mona-openai
 Project-URL: Bug Tracker, https://github.com/monalabs/mona-openai/issues
 Keywords: OpenAI,LLMs,GPT,Mona,Monitoring,AI
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Mona-OpenAI Integration Client
 <p align="center">
   <img src="https://github.com/monalabs/mona-sdk/blob/main/mona_logo.png?raw=true" alt="Mona's logo" width="180"/>
 </p>
@@ -87,15 +87,15 @@
     temperature=temperature,
     MONA_additional_data={"customer_id": "A531251"},
 ))
 
 print(response.choices[0].text)
 ```
 ## Supported OpenAI APIs
-Currently this client supports only `openai.Completion`. Mona can support processes based on other APIs and also non-OpenAI-based apps.
+Currently this client supports `openai.Completion` and `openai.ChatCompletion`. Mona can support processes based on other APIs and also non-OpenAI-based apps.
 If you have a differrent use-case, we'd love to hear about it! Please email us at support@monalabs.io.
 
 ## Usage
 ### Initialization
 
 The main and only function exposed in this package is `monitor`.
 ```py
@@ -133,15 +133,15 @@
 The specs arg allows you to configure what should be monitored. It expects a python dict with the follwoing possible keys:
 * sampling_ratio (1): A number between 0 and 1 for how often should the call be logged.
 * avoid_monitoring_exceptions (False): Whether or not to log out to Mona when there is an OpenAI exception. Default is to track exceptions - and Mona will alert you on things like a jump in number of exceptions
 * export_prompt (False): Whether Mona should export the actual prompt text. Be default set to False to avoid privacy concerns.
 * export_response_texts (False): Whether Mona should export the actual response texts. Be default set to False to avoid privacy concerns.
 * analysis: A dictionary mapping each analysis type to a boolean value telling the client whether or not to run said analysis and log it to Mona. Possible options currently are "privacy", "profanity", and "textual". By default, all analyses take place and are logged out to Mona.
 
-### on-going
+### Capabilities during API calls
 
 After wrapping your endpoint with `monitor`, you really don't need to do anything else. When using `create` or `acreate` data will be tracked and monitoring will take place.
 
 There are, however, several capabilities that are added to these functions. Specifically, you can add the following arguments to any create call:
 * MONA_context_id: The unique id of the context in which the call is made. By using this ID you can export more data to Mona to the same context from other places. If not supplied, the "id" field of the OpenAI Endpoint's response will be used as the Mona context ID automatically.
 * MONA_export_timestamp: Can be used to simulate as if the current call was made in a different time, as far as Mona is concerned.
 * MONA_additional_data: A JSON-serializable dict with any other data you want to add to the monitoring context. This comes in handy if you want to add more information to the monitoring contex that isn't part of the basic OpenAI API call information. For example, if you are using a specific template ID or if this call is being made for a specific customer ID, these are fields you can add there to help get full context when monitoring with Mona.
@@ -220,11 +220,23 @@
     print(response.json()["choices"][0]["text"])
 
 except Exception as err:
     # Log exception to Mona
     exception_logger()
 ```
 
+### Stream support
+
+OpenAI allows receiving responses as a stream of tokens using the "stream" parameter. When this is done, Mona will collect all the tokens in memory and will create the analysis and log out the data the moment the stream is over. You don't need to do anything to make this happen.
+
+Since for streaming responses OpenAI doesn't supply the full usage tokens summary, Mona uses the tiktoken package to calculate the tokens of the prompt and completion and log them for monitoring.
+
+NOTE: Stream is currently only supported with SDK usage, and not with using REST directly.
+
+
 ## Mona SDK
 
 This package uses the mona_sdk package to export the relevant data to Mona. There are several environment variables you can use to configure the SDK's behavior. For example, you can set it up to raise exceptions when exporting data to Mona fails (it doesn't do that by default).
 
+## Monitoring for profanity
+
+Mona uses the alt-profanity-check pacakge (https://pypi.org/project/alt-profanity-check/) to create both boolean predictions and probabilty scores for the existence of profanity both in the prompt and in the responses. We use the built in package methods for that. If you want, for example, to use a different probability threshold for the boolean prediction, you can do that by changing your Mona config on the Mona dashboard.
```

### Comparing `mona-openai-0.0.3/README.md` & `mona-openai-0.0.4/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -72,15 +72,15 @@
     temperature=temperature,
     MONA_additional_data={"customer_id": "A531251"},
 ))
 
 print(response.choices[0].text)
 ```
 ## Supported OpenAI APIs
-Currently this client supports only `openai.Completion`. Mona can support processes based on other APIs and also non-OpenAI-based apps.
+Currently this client supports `openai.Completion` and `openai.ChatCompletion`. Mona can support processes based on other APIs and also non-OpenAI-based apps.
 If you have a differrent use-case, we'd love to hear about it! Please email us at support@monalabs.io.
 
 ## Usage
 ### Initialization
 
 The main and only function exposed in this package is `monitor`.
 ```py
@@ -118,15 +118,15 @@
 The specs arg allows you to configure what should be monitored. It expects a python dict with the follwoing possible keys:
 * sampling_ratio (1): A number between 0 and 1 for how often should the call be logged.
 * avoid_monitoring_exceptions (False): Whether or not to log out to Mona when there is an OpenAI exception. Default is to track exceptions - and Mona will alert you on things like a jump in number of exceptions
 * export_prompt (False): Whether Mona should export the actual prompt text. Be default set to False to avoid privacy concerns.
 * export_response_texts (False): Whether Mona should export the actual response texts. Be default set to False to avoid privacy concerns.
 * analysis: A dictionary mapping each analysis type to a boolean value telling the client whether or not to run said analysis and log it to Mona. Possible options currently are "privacy", "profanity", and "textual". By default, all analyses take place and are logged out to Mona.
 
-### on-going
+### Capabilities during API calls
 
 After wrapping your endpoint with `monitor`, you really don't need to do anything else. When using `create` or `acreate` data will be tracked and monitoring will take place.
 
 There are, however, several capabilities that are added to these functions. Specifically, you can add the following arguments to any create call:
 * MONA_context_id: The unique id of the context in which the call is made. By using this ID you can export more data to Mona to the same context from other places. If not supplied, the "id" field of the OpenAI Endpoint's response will be used as the Mona context ID automatically.
 * MONA_export_timestamp: Can be used to simulate as if the current call was made in a different time, as far as Mona is concerned.
 * MONA_additional_data: A JSON-serializable dict with any other data you want to add to the monitoring context. This comes in handy if you want to add more information to the monitoring contex that isn't part of the basic OpenAI API call information. For example, if you are using a specific template ID or if this call is being made for a specific customer ID, these are fields you can add there to help get full context when monitoring with Mona.
@@ -205,11 +205,23 @@
     print(response.json()["choices"][0]["text"])
 
 except Exception as err:
     # Log exception to Mona
     exception_logger()
 ```
 
+### Stream support
+
+OpenAI allows receiving responses as a stream of tokens using the "stream" parameter. When this is done, Mona will collect all the tokens in memory and will create the analysis and log out the data the moment the stream is over. You don't need to do anything to make this happen.
+
+Since for streaming responses OpenAI doesn't supply the full usage tokens summary, Mona uses the tiktoken package to calculate the tokens of the prompt and completion and log them for monitoring.
+
+NOTE: Stream is currently only supported with SDK usage, and not with using REST directly.
+
+
 ## Mona SDK
 
 This package uses the mona_sdk package to export the relevant data to Mona. There are several environment variables you can use to configure the SDK's behavior. For example, you can set it up to raise exceptions when exporting data to Mona fails (it doesn't do that by default).
 
+## Monitoring for profanity
+
+Mona uses the alt-profanity-check pacakge (https://pypi.org/project/alt-profanity-check/) to create both boolean predictions and probabilty scores for the existence of profanity both in the prompt and in the responses. We use the built in package methods for that. If you want, for example, to use a different probability threshold for the boolean prediction, you can do that by changing your Mona config on the Mona dashboard.
```

### Comparing `mona-openai-0.0.3/mona_openai/mona_client.py` & `mona-openai-0.0.4/mona_openai/mona_client.py`

 * *Files identical despite different names*

### Comparing `mona-openai-0.0.3/mona_openai/mona_openai.py` & `mona-openai-0.0.4/mona_openai/mona_openai.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,91 +1,72 @@
 import time
-import asyncio
 from copy import deepcopy
 from types import MappingProxyType
 
 from mona_sdk import MonaSingleMessage
 
-from .exceptions import WrongOpenAIClassException
+from .endpoints.wrapping_getter import get_endpoint_wrapping
 from .mona_client import get_mona_clients
-from .util.func_util import (
-    add_conditional_sampling,
+from .util.func_util import add_conditional_sampling
+from .util.async_util import (
+    run_in_an_event_loop,
     call_non_blocking_sync_or_async,
 )
-from .endpoints.completion import (
-    COMPLETION_CLASS_NAME,
-    get_completion_class,
-    get_analysis_params as completion_analysis_getter,
-    get_clean_message as completion_message_cleaner,
-)
+from .util.openai_util import get_model_param
+from .util.tokens_util import get_usage
+from .util.stream_util import ResponseGatheringIterator
 from .util.validation_util import validate_and_get_sampling_ratio
 
 EMPTY_DICT = MappingProxyType({})
 
 MONA_ARGS_PREFIX = "MONA_"
 CONTEXT_ID_ARG_NAME = MONA_ARGS_PREFIX + "context_id"
 EXPORT_TIMESTAMP_ARG_NAME = MONA_ARGS_PREFIX + "export_timestamp"
 ADDITIONAL_DATA_ARG_NAME = MONA_ARGS_PREFIX + "additional_data"
 
-# TODO(Itai): This is essetially a nice-looking "switch" statement. We should
-#   try to use the name to find the exact monitoring-enrichment function and
-#   filename instead of listing all options here.
-ENDPOINT_NAME_TO_WRAPPER = {COMPLETION_CLASS_NAME: get_completion_class}
-
-
-def _get_monitored_base_class(openai_class):
-    """
-    Returns a class that wrapps the given api class with that
-    api-specific functionality.
-    """
-    class_name = openai_class.__name__
-
-    if class_name not in ENDPOINT_NAME_TO_WRAPPER:
-        raise WrongOpenAIClassException("Class not supported: " + class_name)
-    return ENDPOINT_NAME_TO_WRAPPER[class_name](openai_class)
-
 
 def _get_mona_single_message(
     api_name,
     request_input,
     start_time,
     is_exception,
     is_async,
+    stream_start_time,
     response,
-    analysis_params_getter,
-    specs,
+    analysis_getter,
     context_class,
     message_cleaner,
     additional_data,
     context_id,
     export_timestamp,
 ):
     """
     Returns a MonaSingleMessage object to be used for data
     exporting to Mona's servers by a Mona client.
     """
 
     message = {
         "input": request_input,
         "latency": time.time() - start_time,
+        "stream_start_latency": stream_start_time - start_time
+        if stream_start_time is not None
+        else None,
         "is_exception": is_exception,
         "api_name": api_name,
         "is_async": is_async,
     }
 
     if additional_data:
         message["additional_data"] = additional_data
 
     if response:
         message["response"] = response
-        message["analysis"] = analysis_params_getter(
-            request_input, response, specs
-        )
+        message["analysis"] = analysis_getter(request_input, response)
 
-    message = message_cleaner(message, specs)
+    message = message_cleaner(message)
 
     return MonaSingleMessage(
         message=message,
         contextClass=context_class,
         contextId=context_id,
         exportTimestamp=export_timestamp,
     )
@@ -154,27 +135,35 @@
             sampling ratio.
         mona_clients_getter: Used only for testing purposes
     """
     client, async_client = mona_clients_getter(mona_creds)
 
     sampling_ratio = validate_and_get_sampling_ratio(specs)
 
-    base_class = _get_monitored_base_class(openai_class)
+    base_class = get_endpoint_wrapping(
+        openai_class.__name__, specs
+    ).wrap_class(openai_class)
 
     # TODO(itai): Add call to Mona servers to init the context class if it
     #   isn't inited yet once we have the relevant endpoint for this.
 
     class MonitoredOpenAI(base_class):
         """
         A mona-monitored version of an openai API class.
         """
 
         @classmethod
         def _get_mona_single_message(
-            cls, kwargs_param, start_time, is_exception, is_async, response
+            cls,
+            kwargs_param,
+            start_time,
+            is_exception,
+            is_async,
+            stream_start_time,
+            response,
         ):
             """
             Returns a MonaSingleMessage object to be used for data
             exporting to Mona's servers by a Mona client.
             """
             # Recreate the input dict to avoid manipulating the caller's data,
             # and remove Mona-related data.
@@ -188,17 +177,17 @@
 
             return _get_mona_single_message(
                 api_name=openai_class.__name__,
                 request_input=request_input,
                 start_time=start_time,
                 is_exception=is_exception,
                 is_async=is_async,
+                stream_start_time=stream_start_time,
                 response=response,
-                analysis_params_getter=super()._get_analysis_params,
-                specs=specs,
+                analysis_getter=super()._get_full_analysis,
                 context_class=context_class,
                 message_cleaner=super()._get_clean_message,
                 additional_data=kwargs_param.get(ADDITIONAL_DATA_ARG_NAME),
                 context_id=kwargs_param.get(
                     CONTEXT_ID_ARG_NAME, response["id"] if response else None
                 ),
                 export_timestamp=kwargs_param.get(
@@ -213,64 +202,116 @@
             """
             The main logic for wrapping create functions with mona data
             exporting.
             This internal function porovides a template for both sync
             and async activations (helps with wrapping both "create"
             and "acreate").
             """
-            start_time = time.time()
+
+            is_stream = kwargs.get("stream", False)
+            is_async = super_function.__name__ == "acreate"
 
             response = None
 
+            # will be used only when stream is enabled
+            stream_start_time = None
+
             async def _inner_mona_export(is_exception):
                 return await call_non_blocking_sync_or_async(
                     export_function,
                     (
                         cls._get_mona_single_message(
                             kwargs,
                             start_time,
                             is_exception,
-                            super_function.__name__ == "acreate",
+                            is_async,
+                            stream_start_time,
                             response,
                         ),
                     ),
                 )
 
             mona_export = add_conditional_sampling(
                 _inner_mona_export, sampling_ratio
             )
 
-            try:
+            start_time = time.time()
+
+            async def inner_super_function():
                 # Call the actual openai create function without the Mona
                 # specific arguments.
-                response = await call_non_blocking_sync_or_async(
+                return await call_non_blocking_sync_or_async(
                     super_function,
                     args,
                     {
                         x: kwargs[x]
                         for x in kwargs
                         if not x.startswith(MONA_ARGS_PREFIX)
                     },
                 )
-            except Exception:
+
+            async def inner_handle_exception():
                 if not specs.get("avoid_monitoring_exceptions", False):
                     await mona_export(True)
-                raise
 
-            await mona_export(False)
+            if not is_stream:
+                try:
+                    response = await inner_super_function()
+                except Exception:
+                    await inner_handle_exception()
+                    raise
+
+                await mona_export(False)
+
+                return response
+
+            # From here it's stream handling.
+
+            async def _stream_done_callback(
+                final_response, actual_stream_start_time
+            ):
+                nonlocal response
+                nonlocal stream_start_time
+                # There is no usage data in returned stream responses, so
+                # we add it here.
+                response = final_response | {
+                    "usage": get_usage(
+                        model=get_model_param(kwargs),
+                        prompt_texts=base_class._get_all_prompt_texts(kwargs),
+                        response_texts=base_class._get_all_response_texts(
+                            final_response
+                        ),
+                    )
+                }
+                stream_start_time = actual_stream_start_time
+                await mona_export(False)
 
-            return response
+            try:
+                # Call the actual openai create function without the Mona
+                # specific arguments.
+                return ResponseGatheringIterator(
+                    original_iterator=await inner_super_function(),
+                    delta_choice_text_getter=(
+                        base_class._get_stream_delta_text_from_choice
+                    ),
+                    final_choice_getter=base_class._get_final_choice,
+                    callback=_stream_done_callback,
+                )
+
+            except Exception:
+                await inner_handle_exception()
+                raise
 
         @classmethod
         def create(cls, *args, **kwargs):
             """
             A mona-monitored version of the openai base class' "create"
             function.
             """
-            return asyncio.run(
+            return run_in_an_event_loop(
                 cls._inner_create(client.export, super().create, args, kwargs)
             )
 
         @classmethod
         async def acreate(cls, *args, **kwargs):
             """
             An async mona-monitored version of the openai base class'
@@ -308,14 +349,16 @@
     """
 
     # TODO(itai): Consider creating an async version as well.
     client, _ = mona_clients_getter(mona_creds)
 
     sampling_ratio = validate_and_get_sampling_ratio(specs)
 
+    wrapping_logic = get_endpoint_wrapping(openai_endpoint_name, specs)
+
     class RestClient:
         """
         This will be the returned Mona logging class. We follow
         OpenAI's way of doing things by using a static classe with
         relevant class methods.
         """
 
@@ -343,19 +386,20 @@
                 return client.export(
                     _get_mona_single_message(
                         api_name=openai_endpoint_name,
                         request_input=request_dict,
                         start_time=start_time,
                         is_exception=is_exception,
                         is_async=False,
+                        # TODO(itai): Support stream in REST as well.
+                        stream_start_time=None,
                         response=inner_response,
-                        analysis_params_getter=completion_analysis_getter,
-                        specs=specs,
+                        analysis_getter=wrapping_logic.get_full_analysis,
                         context_class=context_class,
-                        message_cleaner=completion_message_cleaner,
+                        message_cleaner=wrapping_logic.get_clean_message,
                         additional_data=additional_data,
                         context_id=context_id,
                         export_timestamp=export_timestamp,
                     )
                 )
 
             mona_export = add_conditional_sampling(
```

### Comparing `mona-openai-0.0.3/mona_openai/util/validation_util.py` & `mona-openai-0.0.4/mona_openai/util/validation_util.py`

 * *Files identical despite different names*

### Comparing `mona-openai-0.0.3/mona_openai.egg-info/PKG-INFO` & `mona-openai-0.0.4/mona_openai.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mona-openai
-Version: 0.0.3
+Version: 0.0.4
 Summary: Integration client for monitoring OpenAI usage with Mona
 Author-email: Itai Bar Sinai <itai@monalabs.io>
 Project-URL: Homepage, https://github.com/monalabs/mona-openai
 Project-URL: Bug Tracker, https://github.com/monalabs/mona-openai/issues
 Keywords: OpenAI,LLMs,GPT,Mona,Monitoring,AI
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Mona-OpenAI Integration Client
 <p align="center">
   <img src="https://github.com/monalabs/mona-sdk/blob/main/mona_logo.png?raw=true" alt="Mona's logo" width="180"/>
 </p>
@@ -87,15 +87,15 @@
     temperature=temperature,
     MONA_additional_data={"customer_id": "A531251"},
 ))
 
 print(response.choices[0].text)
 ```
 ## Supported OpenAI APIs
-Currently this client supports only `openai.Completion`. Mona can support processes based on other APIs and also non-OpenAI-based apps.
+Currently this client supports `openai.Completion` and `openai.ChatCompletion`. Mona can support processes based on other APIs and also non-OpenAI-based apps.
 If you have a differrent use-case, we'd love to hear about it! Please email us at support@monalabs.io.
 
 ## Usage
 ### Initialization
 
 The main and only function exposed in this package is `monitor`.
 ```py
@@ -133,15 +133,15 @@
 The specs arg allows you to configure what should be monitored. It expects a python dict with the follwoing possible keys:
 * sampling_ratio (1): A number between 0 and 1 for how often should the call be logged.
 * avoid_monitoring_exceptions (False): Whether or not to log out to Mona when there is an OpenAI exception. Default is to track exceptions - and Mona will alert you on things like a jump in number of exceptions
 * export_prompt (False): Whether Mona should export the actual prompt text. Be default set to False to avoid privacy concerns.
 * export_response_texts (False): Whether Mona should export the actual response texts. Be default set to False to avoid privacy concerns.
 * analysis: A dictionary mapping each analysis type to a boolean value telling the client whether or not to run said analysis and log it to Mona. Possible options currently are "privacy", "profanity", and "textual". By default, all analyses take place and are logged out to Mona.
 
-### on-going
+### Capabilities during API calls
 
 After wrapping your endpoint with `monitor`, you really don't need to do anything else. When using `create` or `acreate` data will be tracked and monitoring will take place.
 
 There are, however, several capabilities that are added to these functions. Specifically, you can add the following arguments to any create call:
 * MONA_context_id: The unique id of the context in which the call is made. By using this ID you can export more data to Mona to the same context from other places. If not supplied, the "id" field of the OpenAI Endpoint's response will be used as the Mona context ID automatically.
 * MONA_export_timestamp: Can be used to simulate as if the current call was made in a different time, as far as Mona is concerned.
 * MONA_additional_data: A JSON-serializable dict with any other data you want to add to the monitoring context. This comes in handy if you want to add more information to the monitoring contex that isn't part of the basic OpenAI API call information. For example, if you are using a specific template ID or if this call is being made for a specific customer ID, these are fields you can add there to help get full context when monitoring with Mona.
@@ -220,11 +220,23 @@
     print(response.json()["choices"][0]["text"])
 
 except Exception as err:
     # Log exception to Mona
     exception_logger()
 ```
 
+### Stream support
+
+OpenAI allows receiving responses as a stream of tokens using the "stream" parameter. When this is done, Mona will collect all the tokens in memory and will create the analysis and log out the data the moment the stream is over. You don't need to do anything to make this happen.
+
+Since for streaming responses OpenAI doesn't supply the full usage tokens summary, Mona uses the tiktoken package to calculate the tokens of the prompt and completion and log them for monitoring.
+
+NOTE: Stream is currently only supported with SDK usage, and not with using REST directly.
+
+
 ## Mona SDK
 
 This package uses the mona_sdk package to export the relevant data to Mona. There are several environment variables you can use to configure the SDK's behavior. For example, you can set it up to raise exceptions when exporting data to Mona fails (it doesn't do that by default).
 
+## Monitoring for profanity
+
+Mona uses the alt-profanity-check pacakge (https://pypi.org/project/alt-profanity-check/) to create both boolean predictions and probabilty scores for the existence of profanity both in the prompt and in the responses. We use the built in package methods for that. If you want, for example, to use a different probability threshold for the boolean prediction, you can do that by changing your Mona config on the Mona dashboard.
```

### Comparing `mona-openai-0.0.3/pyproject.toml` & `mona-openai-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mona-openai"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Itai Bar Sinai", email="itai@monalabs.io" },
 ]
 description = "Integration client for monitoring OpenAI usage with Mona"
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
 ]
 keywords = ["OpenAI", "LLMs", "GPT", "Mona", "Monitoring", "AI"]
 dynamic = ["dependencies"]
```

