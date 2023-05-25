# Comparing `tmp/zep_python-0.25.tar.gz` & `tmp/zep_python-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zep_python-0.25.tar", max compression
+gzip compressed data, was "zep_python-0.3.0.tar", max compression
```

## Comparing `zep_python-0.25.tar` & `zep_python-0.3.0.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0    11357 2023-05-17 05:23:06.606851 zep_python-0.25/LICENSE
--rw-r--r--   0        0        0     2434 2023-05-17 05:23:06.606851 zep_python-0.25/README.md
--rw-r--r--   0        0        0      775 2023-05-17 05:23:06.610851 zep_python-0.25/pyproject.toml
--rw-r--r--   0        0        0      340 2023-05-17 05:23:06.610851 zep_python-0.25/zep_python/__init__.py
--rw-r--r--   0        0        0     1236 2023-05-17 05:23:06.610851 zep_python-0.25/zep_python/exceptions.py
--rw-r--r--   0        0        0     4861 2023-05-17 05:23:06.610851 zep_python-0.25/zep_python/models.py
--rw-r--r--   0        0        0        0 2023-05-17 05:23:06.610851 zep_python-0.25/zep_python/py.typed
--rw-r--r--   0        0        0      670 2023-05-17 05:23:06.610851 zep_python-0.25/zep_python/utils.py
--rw-r--r--   0        0        0    12621 2023-05-17 05:23:06.610851 zep_python-0.25/zep_python/zep_client.py
--rw-r--r--   0        0        0     3113 1970-01-01 00:00:00.000000 zep_python-0.25/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-25 18:21:47.636865 zep_python-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2393 2023-05-25 18:21:47.636865 zep_python-0.3.0/README.md
+-rw-r--r--   0        0        0      873 2023-05-25 18:21:47.640865 zep_python-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      340 2023-05-25 18:21:47.640865 zep_python-0.3.0/zep_python/__init__.py
+-rw-r--r--   0        0        0     1236 2023-05-25 18:21:47.640865 zep_python-0.3.0/zep_python/exceptions.py
+-rw-r--r--   0        0        0     4956 2023-05-25 18:21:47.640865 zep_python-0.3.0/zep_python/models.py
+-rw-r--r--   0        0        0        0 2023-05-25 18:21:47.640865 zep_python-0.3.0/zep_python/py.typed
+-rw-r--r--   0        0        0    13465 2023-05-25 18:21:47.640865 zep_python-0.3.0/zep_python/zep_client.py
+-rw-r--r--   0        0        0     3073 1970-01-01 00:00:00.000000 zep_python-0.3.0/PKG-INFO
```

### Comparing `zep_python-0.25/LICENSE` & `zep_python-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zep_python-0.25/README.md` & `zep_python-0.3.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -38,23 +38,22 @@
     memory = Memory()
     memory.messages = [message]
     # Add a memory
     result = await client.aadd_memory(session_id, memory)
 
     # Long chat histories will automatically be summarized.
     # A summary and chat history are returned with a `get_memory`
-    memories = await client.aget_memory(session_id)
-    for memory in memories:
-        for message in memory.messages:
-            print(message.to_dict())
+    memory = await client.aget_memory(session_id)
+    for message in memory.messages:
+         print(message.to_dict())
 
     # Search memory
     # Messages uploaded to Zep are automatically embedded and made available
     # for vector-based similarity search.
-    search_payload = SearchPayload({}, "Who is Yuri Gagarin?")
+    search_payload = SearchPayload("Who is Yuri Gagarin?")
     search_results = await client.asearch_memory(session_id, search_payload)
     for search_result in search_results:
         # Access the 'content' field within the 'message' object.
         message_content = search_result.message
         print(message_content)
 ```
```

### Comparing `zep_python-0.25/pyproject.toml` & `zep_python-0.3.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zep-python"
-version = "0.25"
+version = "0.3.0"
 description = "Zep stores, manages, enriches, indexes, and searches long-term memory for conversational AI applications. This is the Python client for the Zep service."
 authors = ["Daniel Chalef <daniel.chalef@private.org>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 httpx = "^0.24.0"
@@ -19,12 +19,15 @@
 pytest-mock = "^3.10.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 ruff = "^0.0.265"
 mypy = "^1.2.0"
 pre-commit = "^3.3.1"
-sphinxawesome-theme = "^4.0.3"
+mkdocs = "^1.4.3"
+mkdocstrings = {version = "0.21.2", extras = ["python"]}
+python-dotenv = "^1.0.0"
+mkdocs-material = "^9.1.13"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `zep_python-0.25/zep_python/exceptions.py` & `zep_python-0.3.0/zep_python/exceptions.py`

 * *Files identical despite different names*

### Comparing `zep_python-0.25/zep_python/models.py` & `zep_python-0.3.0/zep_python/models.py`

 * *Files 16% similar despite different names*

```diff
@@ -70,14 +70,15 @@
     """
 
     role: str = Field("A role is required")
     content: str = Field("Content is required")
     uuid: Optional[str] = Field(optional=True, default=None)
     created_at: Optional[str] = Field(optional=True, default=None)
     token_count: Optional[int] = Field(optional=True, default=None)
+    metadata: Optional[Dict[str, Any]] = Field(optional=True, default=None)
 
     def to_dict(self) -> Dict[str, Any]:
         """
         Returns a dictionary representation of the message.
 
         Returns
         -------
@@ -87,27 +88,33 @@
         return self.dict()
 
 
 class Memory(BaseModel):
     """
     Represents a memory object with messages, metadata, and other attributes.
 
-    :param messages: A list of message objects, where each message contains a role and
-                     content.
-    :type messages: Optional[List[Dict[str, Any]]]
-    :param metadata: A dictionary containing metadata associated with the memory.
-    :type metadata: Optional[Dict[str, Any]]
-    :param summary: A Summary object.
-    :type summary: Optional[Summary]
-    :param uuid: A unique identifier for the memory.
-    :type uuid: Optional[str]
-    :param created_at: The timestamp when the memory was created.
-    :type created_at: Optional[str]
-    :param token_count: The token count of the memory.
-    :type token_count: Optional[int]
+    Attributes
+    ----------
+    messages : Optional[List[Dict[str, Any]]]
+        A list of message objects, where each message contains a role and content.
+    metadata : Optional[Dict[str, Any]]
+        A dictionary containing metadata associated with the memory.
+    summary : Optional[Summary]
+        A Summary object.
+    uuid : Optional[str]
+        A unique identifier for the memory.
+    created_at : Optional[str]
+        The timestamp when the memory was created.
+    token_count : Optional[int]
+        The token count of the memory.
+
+    Methods
+    -------
+    to_dict() -> Dict[str, Any]:
+        Returns a dictionary representation of the message.
     """
 
     messages: List[Message] = Field(
         default=[], description="A List of Messages or empty List is required"
     )
     metadata: Optional[Dict[str, Any]] = Field(optional=True, default=None)
     summary: Optional[Summary] = Field(optional=True, default=None)
```

### Comparing `zep_python-0.25/zep_python/zep_client.py` & `zep_python-0.3.0/zep_python/zep_client.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 from __future__ import annotations
 
-import asyncio
 from types import TracebackType
-from typing import List, Optional, Type
+from typing import Any, Dict, List, Optional, Type
 
 import httpx
 
 from zep_python.exceptions import APIError, NotFoundError
 from zep_python.models import Memory, Message, SearchPayload, SearchResult, Summary
-from zep_python.utils import sync
 
-API_BASEURL = "/api/v1"
+API_BASE_PATH = "/api/v1"
 
 
 class ZepClient:
     """
     ZepClient class implementation.
 
     Attributes
@@ -44,73 +42,114 @@
         Initialize the ZepClient with the specified base URL.
 
         Parameters
         ----------
         base_url : str
             The base URL of the API.
         """
-        self.base_url = base_url
-        self.client = httpx.AsyncClient()
+        self.base_url = f"{base_url}{API_BASE_PATH}"
+        self.aclient = httpx.AsyncClient(base_url=self.base_url)
+        self.client = httpx.Client(base_url=self.base_url)
 
-    # Asynchronous context manager entry point
     async def __aenter__(self) -> "ZepClient":
+        """Asynchronous context manager entry point"""
         return self
 
-    # Sync context manager exit point
     async def __aexit__(
         self,
         exc_type: Type[Exception],
         exc_val: Exception,
         exc_tb: TracebackType,
     ) -> None:
+        """Asynchronous context manager exit point"""
         await self.aclose()
 
-    # Asynchronous context manager entry point
     def __enter__(self) -> "ZepClient":
+        """Sync context manager entry point"""
         return self
 
-    # Sync context manager exit point
     def __exit__(
         self,
         exc_type: Type[Exception],
         exc_val: Exception,
         exc_tb: TracebackType,
     ) -> None:
+        """Sync context manager exit point"""
         self.close()
 
-    @sync
+    def _parse_get_memory_response(self, response_data: Any) -> Memory:
+        """Parse the response from the get_memory API call."""
+        messages: List[Message]
+        try:
+            messages = [
+                Message.parse_obj(m) for m in response_data.get("messages", None)
+            ]
+            if len(messages) == 0:
+                raise ValueError("Messages can't be empty")
+        except (TypeError, ValueError) as e:
+            raise APIError("Unexpected response format from the API") from e
+
+        summary: Optional[Summary] = None
+        if response_data.get("summary", None) is not None:
+            summary = Summary.parse_obj(response_data["summary"])
+
+        memory = Memory(
+            messages=messages,
+            # Add the 'summary' field if it is present in the response.
+            summary=summary,
+            # Add any other fields from the response that are relevant to the
+            # Memory class.
+        )
+        return memory
+
+    def _gen_get_params(self, lastn: Optional[int] = None) -> Dict[str, Any]:
+        params = {}
+        if lastn is not None:
+            params["lastn"] = lastn
+        return params
+
     def get_memory(self, session_id: str, lastn: Optional[int] = None) -> Memory:
         """
-        Retrieve memory for the specified session. This method is a synchronous wrapper
-        for the asynchronous method `aget_memory`.
+        Retrieve memory for the specified session.
 
         Parameters
         ----------
         session_id : str
             The ID of the session for which to retrieve memory.
         lastn : Optional[int], optional
             The number of most recent memory entries to retrieve. Defaults to None (all
             entries).
 
         Returns
         -------
-        List[Memory]
-            A list of Memory objects representing the retrieved memory entries.
+        Memory
+            A memory object containing a Summary, metadata, and list of Messages.
 
         Raises
         ------
         APIError
             If the API response format is unexpected.
         """
-        # we've wrapped the function in a decorator that will run it synchronously.
-        # ignore the type error.
+
         if session_id is None or session_id == "":
             raise ValueError("session_id must be provided")
 
-        return self.aget_memory(session_id, lastn)  # type: ignore
+        url = f"/sessions/{session_id}/memory"
+        params = self._gen_get_params(lastn)
+        response = self.client.get(url, params=params)
+
+        if response.status_code == 404:
+            raise NotFoundError(f"No memory found for session {session_id}")
+
+        if response.status_code != 200:
+            raise APIError(f"Unexpected status code: {response.status_code}")
+
+        response_data = response.json()
+
+        return self._parse_get_memory_response(response_data)
 
     async def aget_memory(self, session_id: str, lastn: Optional[int] = None) -> Memory:
         """
         Asynchronously retrieve memory for the specified session.
 
         Parameters
         ----------
@@ -119,65 +158,41 @@
         lastn : Optional[int], optional
             The number of most recent memory entries to retrieve. Defaults to None (all
             entries).
 
         Returns
         -------
         Memory
-            A Memory object representing the retrieved memory entries.
+            A memory object containing a Summary, metadata, and list of Messages.
 
         Raises
         ------
         APIError
             If the API response format is unexpected.
         """
         if session_id is None or session_id == "":
             raise ValueError("session_id must be provided")
 
-        url = f"{self.base_url}{API_BASEURL}/sessions/{session_id}/memory"
-        params = (
-            {"lastn": lastn} if lastn is not None else {}
-        )  # Include 'lastn' as a query parameter if provided
-        response = await self.client.get(url, params=params)
+        url = f"/sessions/{session_id}/memory"
+        params = self._gen_get_params(lastn)
+        response = await self.aclient.get(url, params=params)
 
         if response.status_code == 404:
             raise NotFoundError(f"No memory found for session {session_id}")
 
         if response.status_code != 200:
             raise APIError(f"Unexpected status code: {response.status_code}")
 
         response_data = response.json()
-        messages: List[Message]
-        try:
-            messages = [
-                Message.parse_obj(m) for m in response_data.get("messages", None)
-            ]
-            if len(messages) == 0:
-                raise ValueError("Messages can't be empty")
-        except (TypeError, ValueError) as e:
-            raise APIError("Unexpected response format from the API") from e
 
-        summary: Optional[Summary] = None
-        if response_data.get("summary", None) is not None:
-            summary = Summary.parse_obj(response_data["summary"])
+        return self._parse_get_memory_response(response_data)
 
-        memory = Memory(
-            messages=messages,
-            # Add the 'summary' field if it is present in the response.
-            summary=summary,
-            # Add any other fields from the response that are relevant to the
-            # Memory class.
-        )
-        return memory
-
-    @sync
     def add_memory(self, session_id: str, memory_messages: Memory) -> str:
         """
-        Add memory to the specified session. This method is a synchronous wrapper for
-        the asynchronous method `aadd_memory`.
+        Add memory to the specified session.
 
         Parameters
         ----------
         session_id : str
             The ID of the session to which memory should be added.
         memory_messages : Memory
             A Memory object representing the memory messages to be added.
@@ -188,20 +203,25 @@
             The response text from the API.
 
         Raises
         ------
         APIError
             If the API response format is unexpected.
         """
-        # we've wrapped the function in a decorator that will run it synchronously.
-        # ignore the type error.
         if session_id is None or session_id == "":
             raise ValueError("session_id must be provided")
 
-        return self.aadd_memory(session_id, memory_messages)  # type: ignore
+        response = self.client.post(
+            f"/sessions/{session_id}/memory",
+            json=memory_messages.dict(exclude_none=True),
+        )
+        if response.status_code != 200:
+            raise APIError(f"Unexpected status code: {response.status_code}")
+
+        return response.text
 
     async def aadd_memory(self, session_id: str, memory_messages: Memory) -> str:
         """
         Asynchronously add memory to the specified session.
 
         Parameters
         ----------
@@ -219,28 +239,26 @@
         ------
         APIError
             If the API response format is unexpected.
         """
         if session_id is None or session_id == "":
             raise ValueError("session_id must be provided")
 
-        response = await self.client.post(
-            f"{self.base_url}{API_BASEURL}/sessions/{session_id}/memory",
+        response = await self.aclient.post(
+            f"/sessions/{session_id}/memory",
             json=memory_messages.dict(exclude_none=True),
         )
         if response.status_code != 200:
             raise APIError(f"Unexpected status code: {response.status_code}")
 
         return response.text
 
-    @sync
     def delete_memory(self, session_id: str) -> str:
         """
-        Delete memory for the specified session. This method is a synchronous wrapper
-        for the asynchronous method `adelete_memory`.
+        Delete memory for the specified session.
 
         Parameters
         ----------
         session_id : str
             The ID of the session for which memory should be deleted.
 
         Returns
@@ -249,20 +267,24 @@
             The response text from the API.
 
         Raises
         ------
         APIError
             If the API response format is unexpected.
         """
-        # we've wrapped the function in a decorator that will run it synchronously.
-        # ignore the type error.
         if session_id is None or session_id == "":
             raise ValueError("session_id must be provided")
 
-        return self.adelete_memory(session_id)  # type: ignore
+        response = self.client.delete(f"/sessions/{session_id}/memory")
+        if response.status_code == 404:
+            raise NotFoundError(f"No session found for session {session_id}")
+
+        if response.status_code != 200:
+            raise APIError(f"Unexpected status code: {response.status_code}")
+        return response.text
 
     async def adelete_memory(self, session_id: str) -> str:
         """
         Asynchronously delete memory for the specified session.
 
         Parameters
         ----------
@@ -278,34 +300,30 @@
         ------
         APIError
             If the API response format is unexpected.
         """
         if session_id is None or session_id == "":
             raise ValueError("session_id must be provided")
 
-        response = await self.client.delete(
-            f"{self.base_url}{API_BASEURL}/sessions/{session_id}/memory"
-        )
+        response = await self.aclient.delete(f"/sessions/{session_id}/memory")
         if response.status_code == 404:
             raise NotFoundError(f"No session found for session {session_id}")
 
         if response.status_code != 200:
             raise APIError(f"Unexpected status code: {response.status_code}")
         return response.text
 
-    @sync
     def search_memory(
         self,
         session_id: str,
         search_payload: SearchPayload,
         limit: Optional[int] = None,
     ) -> List[SearchResult]:
         """
-        Search memory for the specified session. This method is a synchronous wrapper
-        for the asynchronous method `asearch_memory`.
+        Search memory for the specified session.
 
         Parameters
         ----------
         session_id : str
             The ID of the session for which memory should be searched.
         search_payload : SearchPayload
             A SearchPayload object representing the search query.
@@ -318,20 +336,31 @@
             A list of SearchResult objects representing the search results.
 
         Raises
         ------
         APIError
             If the API response format is unexpected.
         """
-        # we've wrapped the function in a decorator that will run it synchronously.
-        # ignore the type error.
         if session_id is None or session_id == "":
             raise ValueError("session_id must be provided")
 
-        return self.asearch_memory(session_id, search_payload, limit)  # type: ignore
+        if search_payload is None:
+            raise ValueError("search_payload must be provided")
+
+        params = {"limit": limit} if limit is not None else {}
+        response = self.client.post(
+            f"/sessions/{session_id}/search",
+            json=search_payload.dict(),
+            params=params,
+        )
+        if response.status_code == 404:
+            raise NotFoundError("No query results found")
+        if response.status_code != 200:
+            raise APIError(f"Unexpected status code: {response.status_code}")
+        return [SearchResult(**search_result) for search_result in response.json()]
 
     async def asearch_memory(
         self,
         session_id: str,
         search_payload: SearchPayload,
         limit: Optional[int] = None,
     ) -> List[SearchResult]:
@@ -360,16 +389,16 @@
         if session_id is None or session_id == "":
             raise ValueError("session_id must be provided")
 
         if search_payload is None:
             raise ValueError("search_payload must be provided")
 
         params = {"limit": limit} if limit is not None else {}
-        response = await self.client.post(
-            f"{self.base_url}{API_BASEURL}/sessions/{session_id}/search",
+        response = await self.aclient.post(
+            f"/sessions/{session_id}/search",
             json=search_payload.dict(),
             params=params,
         )
         if response.status_code == 404:
             raise NotFoundError("No query results found")
         if response.status_code != 200:
             raise APIError(f"Unexpected status code: {response.status_code}")
@@ -378,17 +407,17 @@
     async def aclose(self) -> None:
         """
         Asynchronously close the HTTP client.
 
         [Optional] This method may be called when the ZepClient is no longer needed to
         release resources.
         """
-        await self.client.aclose()
+        await self.aclient.aclose()
 
     def close(self) -> None:
         """
         Close the HTTP client.
 
         [Optional] This method may be called when the ZepClient is no longer needed to
         release resources.
         """
-        asyncio.run(self.client.aclose())
+        self.client.close()
```

### Comparing `zep_python-0.25/PKG-INFO` & `zep_python-0.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zep-python
-Version: 0.25
+Version: 0.3.0
 Summary: Zep stores, manages, enriches, indexes, and searches long-term memory for conversational AI applications. This is the Python client for the Zep service.
 Author: Daniel Chalef
 Author-email: daniel.chalef@private.org
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -54,23 +54,22 @@
     memory = Memory()
     memory.messages = [message]
     # Add a memory
     result = await client.aadd_memory(session_id, memory)
 
     # Long chat histories will automatically be summarized.
     # A summary and chat history are returned with a `get_memory`
-    memories = await client.aget_memory(session_id)
-    for memory in memories:
-        for message in memory.messages:
-            print(message.to_dict())
+    memory = await client.aget_memory(session_id)
+    for message in memory.messages:
+         print(message.to_dict())
 
     # Search memory
     # Messages uploaded to Zep are automatically embedded and made available
     # for vector-based similarity search.
-    search_payload = SearchPayload({}, "Who is Yuri Gagarin?")
+    search_payload = SearchPayload("Who is Yuri Gagarin?")
     search_results = await client.asearch_memory(session_id, search_payload)
     for search_result in search_results:
         # Access the 'content' field within the 'message' object.
         message_content = search_result.message
         print(message_content)
 ```
```

