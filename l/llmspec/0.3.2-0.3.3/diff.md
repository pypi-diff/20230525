# Comparing `tmp/llmspec-0.3.2.tar.gz` & `tmp/llmspec-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmspec-0.3.2.tar", last modified: Tue May 23 09:40:29 2023, max compression
+gzip compressed data, was "llmspec-0.3.3.tar", last modified: Thu May 25 03:43:34 2023, max compression
```

## Comparing `llmspec-0.3.2.tar` & `llmspec-0.3.3.tar`

### file list

```diff
@@ -1,7 +1,9 @@
--rw-r--r--   0        0        0    11098 2023-05-23 09:40:17.925076 llmspec-0.3.2/LICENSE
--rw-r--r--   0        0        0       33 2023-05-23 09:40:17.925076 llmspec-0.3.2/README.md
--rw-r--r--   0        0        0      609 2023-05-23 09:40:17.929076 llmspec-0.3.2/llmspec/__init__.py
--rw-r--r--   0        0        0     9587 2023-05-23 09:40:17.929076 llmspec-0.3.2/llmspec/llmspec.py
--rw-r--r--   0        0        0     1056 2023-05-23 09:40:29.229894 llmspec-0.3.2/pyproject.toml
--rw-r--r--   0        0        0       34 2023-05-23 09:40:17.929076 llmspec-0.3.2/tests/dummy_test.py
--rw-r--r--   0        0        0      457 1970-01-01 00:00:00.000000 llmspec-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0    11098 2023-05-25 03:43:24.623457 llmspec-0.3.3/LICENSE
+-rw-r--r--   0        0        0       33 2023-05-25 03:43:24.623457 llmspec-0.3.3/README.md
+-rw-r--r--   0        0        0      649 2023-05-25 03:43:24.623457 llmspec-0.3.3/llmspec/__init__.py
+-rw-r--r--   0        0        0     9773 2023-05-25 03:43:24.623457 llmspec-0.3.3/llmspec/llmspec.py
+-rw-r--r--   0        0        0      215 2023-05-25 03:43:24.623457 llmspec-0.3.3/llmspec/mixins.py
+-rw-r--r--   0        0        0       54 2023-05-25 03:43:24.623457 llmspec-0.3.3/llmspec/types.py
+-rw-r--r--   0        0        0     1097 2023-05-25 03:43:34.899867 llmspec-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0       34 2023-05-25 03:43:24.623457 llmspec-0.3.3/tests/dummy_test.py
+-rw-r--r--   0        0        0      457 1970-01-01 00:00:00.000000 llmspec-0.3.3/PKG-INFO
```

### Comparing `llmspec-0.3.2/LICENSE` & `llmspec-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `llmspec-0.3.2/llmspec/llmspec.py` & `llmspec-0.3.3/llmspec/llmspec.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 from __future__ import annotations
+
 import json
-from typing import Union, Optional, Dict, List
 from datetime import datetime
 from enum import Enum
+from typing import Dict, List, Optional, Union
 
 import msgspec
 
+from llmspec.mixins import JSONSerializableMixin
+
 
 class Role(Enum):
     """Chat roles."""
 
     SYSTEM = "system"
     USER = "user"
     ASSISTANT = "assistant"
@@ -76,33 +79,29 @@
     append_assistant_token=True,
 )
 BloomZ = LanguageModelInfo()
 LLaMA = LanguageModelInfo()
 Unknown = LanguageModelInfo()
 
 
-class CompletionRequest(msgspec.Struct, kw_only=True):
+class CompletionRequest(msgspec.Struct, JSONSerializableMixin, kw_only=True):
     suffix: Optional[str] = None
     max_tokens: int = 16
     temperature: float = 1.0
     top_p: float = 1.0
     n: int = 1
     stream: bool = False
     stop: Optional[Union[str, List[str]]] = None
     presence_penalty: float = 0.0
     frequency_penalty: float = 0.0
     repetition_penalty: float = 0.0
     logit_bias: Optional[Dict] = None
     user: str = ""
     do_sample: bool = False
 
-    @classmethod
-    def from_bytes(cls, buf: bytes):
-        return msgspec.json.decode(buf, type=cls)
-
 
 class PromptCompletionRequest(CompletionRequest):
     model: str
     prompt: Union[str, List[str]] = "<|endoftext|>"
     echo: bool = False
     logprobs: Optional[int] = None
     best_of: int = 1
@@ -198,60 +197,62 @@
 class CompletionChoice(msgspec.Struct):
     text: str
     index: int = 0
     logprobs: Optional[int] = None
     finish_reason: str = "length"
 
 
-class LMResponse(msgspec.Struct):
+class LMResponse(msgspec.Struct, JSONSerializableMixin):
     id: str
     object: str
     created: datetime
     model: str
     usage: TokenUsage
 
-    def to_json(self):
-        return msgspec.json.encode(self)
-
 
 class CompletionResponse(LMResponse):
     choices: List[CompletionChoice]
 
 
 class ChatResponse(LMResponse):
     choices: List[ChatChoice]
 
 
-class EmbeddingRequest(msgspec.Struct):
+class EmbeddingRequest(msgspec.Struct, JSONSerializableMixin):
     model: str
     input: Union[str, List[str]]
     user: str = ""
 
 
 class EmbeddingData(msgspec.Struct):
-    embedding: List[float]
+    # not using EmbeddingValue
+    # TypeError: Type unions may not contain more than
+    # one array-like (list, set, tuple) type - type
+    # `typing.Union[typing.List[float], typing.List[typing.List[float]]]`
+    # is not supported
+    embedding: List[Union[float, List[float]]]
     index: int
     object: str = "embedding"
 
 
-class EmbeddingResponse(msgspec.Struct):
+class EmbeddingResponse(msgspec.Struct, JSONSerializableMixin):
     data: EmbeddingData
     model: str
     usage: TokenUsage
     object: str = "list"
 
 
 class ErrorMessage(msgspec.Struct):
     code: int
     type: str
     message: str
     param: str
 
 
-class ErrorResponse(msgspec.Struct):
+class ErrorResponse(msgspec.Struct, JSONSerializableMixin):
     error: ErrorMessage
 
     @classmethod
     def from_validation_err(
         cls, err: msgspec.ValidationError, param: str = ""
     ) -> ErrorResponse:
         return ErrorResponse(
@@ -259,17 +260,14 @@
                 code=400,
                 type="validation_error",
                 message=str(err),
                 param=param,
             )
         )
 
-    def to_json(self):
-        return msgspec.json.encode(self)
-
 
 class LLMSpec:
     """
     Represents an LLMSpec object.
 
     Args:
         text (str): The text content of the LLMSpec.
```

### Comparing `llmspec-0.3.2/pyproject.toml` & `llmspec-0.3.3/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
 ]
 dependencies = [
     "msgspec>=0.15.0",
 ]
 requires-python = ">=3.8"
 readme = "README.md"
-version = "0.3.2"
+version = "0.3.3"
 
 [project.license]
 text = "Apache-2.0"
 
 [build-system]
 requires = [
     "pdm-backend",
@@ -56,11 +56,15 @@
 
 [tool.ruff]
 line-length = 88
 select = [
     "E",
     "F",
     "B",
+    "I",
+    "SIM",
+    "TID",
+    "PL",
 ]
 
 [tool.black]
 line-length = 88
```

