# Comparing `tmp/lanarky-0.6.5.tar.gz` & `tmp/lanarky-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lanarky-0.6.5.tar", max compression
+gzip compressed data, was "lanarky-0.6.6.tar", max compression
```

## Comparing `lanarky-0.6.5.tar` & `lanarky-0.6.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1073 2023-05-23 17:13:55.227473 lanarky-0.6.5/LICENSE
--rw-r--r--   0        0        0     3991 2023-05-23 17:13:55.227473 lanarky-0.6.5/README.md
--rw-r--r--   0        0        0        0 2023-05-23 17:13:55.443477 lanarky-0.6.5/lanarky/__init__.py
--rw-r--r--   0        0        0     2500 2023-05-23 17:13:55.443477 lanarky-0.6.5/lanarky/callbacks/__init__.py
--rw-r--r--   0        0        0     3023 2023-05-23 17:13:55.443477 lanarky-0.6.5/lanarky/callbacks/agents.py
--rw-r--r--   0        0        0     2216 2023-05-23 17:13:55.443477 lanarky-0.6.5/lanarky/callbacks/base.py
--rw-r--r--   0        0        0     1685 2023-05-23 17:13:55.443477 lanarky-0.6.5/lanarky/callbacks/llm.py
--rw-r--r--   0        0        0     3461 2023-05-23 17:13:55.443477 lanarky-0.6.5/lanarky/callbacks/retrieval_qa.py
--rw-r--r--   0        0        0     2004 2023-05-23 17:13:55.443477 lanarky-0.6.5/lanarky/register.py
--rw-r--r--   0        0        0       74 2023-05-23 17:13:55.443477 lanarky-0.6.5/lanarky/responses/__init__.py
--rw-r--r--   0        0        0     2926 2023-05-23 17:13:55.443477 lanarky-0.6.5/lanarky/responses/streaming.py
--rw-r--r--   0        0        0      715 2023-05-23 17:13:55.443477 lanarky-0.6.5/lanarky/schemas.py
--rw-r--r--   0        0        0       69 2023-05-23 17:13:55.443477 lanarky-0.6.5/lanarky/testing/__init__.py
--rw-r--r--   0        0        0     3212 2023-05-23 17:13:55.443477 lanarky-0.6.5/lanarky/testing/gradio.py
--rw-r--r--   0        0        0      391 2023-05-23 17:13:55.443477 lanarky-0.6.5/lanarky/testing/settings.py
--rw-r--r--   0        0        0       73 2023-05-23 17:13:55.443477 lanarky-0.6.5/lanarky/websockets/__init__.py
--rw-r--r--   0        0        0     3844 2023-05-23 17:13:55.443477 lanarky-0.6.5/lanarky/websockets/base.py
--rw-r--r--   0        0        0     1093 2023-05-23 17:13:55.443477 lanarky-0.6.5/pyproject.toml
--rw-r--r--   0        0        0     4812 1970-01-01 00:00:00.000000 lanarky-0.6.5/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-25 07:35:03.418717 lanarky-0.6.6/LICENSE
+-rw-r--r--   0        0        0     3991 2023-05-25 07:35:03.418717 lanarky-0.6.6/README.md
+-rw-r--r--   0        0        0        0 2023-05-25 07:35:03.602719 lanarky-0.6.6/lanarky/__init__.py
+-rw-r--r--   0        0        0     2874 2023-05-25 07:35:03.602719 lanarky-0.6.6/lanarky/callbacks/__init__.py
+-rw-r--r--   0        0        0     3023 2023-05-25 07:35:03.602719 lanarky-0.6.6/lanarky/callbacks/agents.py
+-rw-r--r--   0        0        0     2200 2023-05-25 07:35:03.602719 lanarky-0.6.6/lanarky/callbacks/base.py
+-rw-r--r--   0        0        0     1685 2023-05-25 07:35:03.602719 lanarky-0.6.6/lanarky/callbacks/llm.py
+-rw-r--r--   0        0        0     3461 2023-05-25 07:35:03.602719 lanarky-0.6.6/lanarky/callbacks/retrieval_qa.py
+-rw-r--r--   0        0        0     2004 2023-05-25 07:35:03.602719 lanarky-0.6.6/lanarky/register.py
+-rw-r--r--   0        0        0       74 2023-05-25 07:35:03.602719 lanarky-0.6.6/lanarky/responses/__init__.py
+-rw-r--r--   0        0        0     2926 2023-05-25 07:35:03.602719 lanarky-0.6.6/lanarky/responses/streaming.py
+-rw-r--r--   0        0        0      715 2023-05-25 07:35:03.602719 lanarky-0.6.6/lanarky/schemas.py
+-rw-r--r--   0        0        0       69 2023-05-25 07:35:03.602719 lanarky-0.6.6/lanarky/testing/__init__.py
+-rw-r--r--   0        0        0     3212 2023-05-25 07:35:03.602719 lanarky-0.6.6/lanarky/testing/gradio.py
+-rw-r--r--   0        0        0      391 2023-05-25 07:35:03.602719 lanarky-0.6.6/lanarky/testing/settings.py
+-rw-r--r--   0        0        0       73 2023-05-25 07:35:03.602719 lanarky-0.6.6/lanarky/websockets/__init__.py
+-rw-r--r--   0        0        0     3844 2023-05-25 07:35:03.602719 lanarky-0.6.6/lanarky/websockets/base.py
+-rw-r--r--   0        0        0     1110 2023-05-25 07:35:03.602719 lanarky-0.6.6/pyproject.toml
+-rw-r--r--   0        0        0     4812 1970-01-01 00:00:00.000000 lanarky-0.6.6/PKG-INFO
```

### Comparing `lanarky-0.6.5/LICENSE` & `lanarky-0.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `lanarky-0.6.5/README.md` & `lanarky-0.6.6/README.md`

 * *Files identical despite different names*

### Comparing `lanarky-0.6.5/lanarky/callbacks/agents.py` & `lanarky-0.6.6/lanarky/callbacks/agents.py`

 * *Files identical despite different names*

### Comparing `lanarky-0.6.5/lanarky/callbacks/base.py` & `lanarky-0.6.6/lanarky/callbacks/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     """Async Callback handler for WebsocketConnection."""
 
     websocket: WebSocket = Field(...)
     response: WebsocketResponse = Field(...)
 
     def _construct_message(self, content: str) -> dict:
         """Construct a WebsocketResponse from a string."""
-        return {**self.response.dict(), **{"message": content.encode("utf-8")}}
+        return {**self.response.dict(), **{"message": content}}
 
 
 class AsyncStreamingJSONResponseCallback(AsyncStreamingResponseCallback):
     """Async Callback handler for StreamingJSONResponse."""
 
     send: Send = Field(...)
```

### Comparing `lanarky-0.6.5/lanarky/callbacks/llm.py` & `lanarky-0.6.6/lanarky/callbacks/llm.py`

 * *Files identical despite different names*

### Comparing `lanarky-0.6.5/lanarky/callbacks/retrieval_qa.py` & `lanarky-0.6.6/lanarky/callbacks/retrieval_qa.py`

 * *Files identical despite different names*

### Comparing `lanarky-0.6.5/lanarky/register.py` & `lanarky-0.6.6/lanarky/register.py`

 * *Files identical despite different names*

### Comparing `lanarky-0.6.5/lanarky/responses/streaming.py` & `lanarky-0.6.6/lanarky/responses/streaming.py`

 * *Files identical despite different names*

### Comparing `lanarky-0.6.5/lanarky/schemas.py` & `lanarky-0.6.6/lanarky/schemas.py`

 * *Files identical despite different names*

### Comparing `lanarky-0.6.5/lanarky/testing/gradio.py` & `lanarky-0.6.6/lanarky/testing/gradio.py`

 * *Files identical despite different names*

### Comparing `lanarky-0.6.5/lanarky/websockets/base.py` & `lanarky-0.6.6/lanarky/websockets/base.py`

 * *Files identical despite different names*

### Comparing `lanarky-0.6.5/pyproject.toml` & `lanarky-0.6.6/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lanarky"
-version = "0.6.5"
+version = "0.6.6"
 description = "Ship production-ready LLM projects with FastAPI"
 authors = ["Ajinkya Indulkar <26824103+ajndkr@users.noreply.github.com>"]
 readme = "README.md"
 homepage = "https://github.com/ajndkr/lanarky"
 repository = "https://github.com/ajndkr/lanarky"
 license = "MIT"
 packages = [{include = "lanarky"}]
@@ -23,14 +23,15 @@
 
 [tool.poetry.group.docs.dependencies]
 furo = "^2023.3.27"
 sphinx-autobuild = "^2021.3.14"
 myst-parser = "^1.0.0"
 sphinx-copybutton = "^0.5.2"
 autodoc-pydantic = "^1.8.0"
+toml = "^0.10.2"
 
 
 [tool.poetry.group.tests.dependencies]
 pytest = "^7.3.1"
 pytest-cov = "^4.0.0"
 pytest-asyncio = "^0.21.0"
 coveralls = "^3.3.1"
```

### Comparing `lanarky-0.6.5/PKG-INFO` & `lanarky-0.6.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lanarky
-Version: 0.6.5
+Version: 0.6.6
 Summary: Ship production-ready LLM projects with FastAPI
 Home-page: https://github.com/ajndkr/lanarky
 License: MIT
 Author: Ajinkya Indulkar
 Author-email: 26824103+ajndkr@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

