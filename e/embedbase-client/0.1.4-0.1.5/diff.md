# Comparing `tmp/embedbase_client-0.1.4.tar.gz` & `tmp/embedbase_client-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embedbase_client-0.1.4.tar", max compression
+gzip compressed data, was "embedbase_client-0.1.5.tar", max compression
```

## Comparing `embedbase_client-0.1.4.tar` & `embedbase_client-0.1.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1077 2023-05-23 15:58:36.848724 embedbase_client-0.1.4/LICENSE
--rw-r--r--   0        0        0     1005 2023-05-23 15:58:36.848724 embedbase_client-0.1.4/README.md
--rw-r--r--   0        0        0      389 2023-05-23 15:58:36.848724 embedbase_client-0.1.4/embedbase_client/__init__.py
--rw-r--r--   0        0        0    15456 2023-05-23 15:58:36.848724 embedbase_client-0.1.4/embedbase_client/async_client.py
--rw-r--r--   0        0        0      913 2023-05-23 15:58:36.848724 embedbase_client-0.1.4/embedbase_client/base.py
--rw-r--r--   0        0        0     1194 2023-05-23 15:58:36.848724 embedbase_client-0.1.4/embedbase_client/errors.py
--rw-r--r--   0        0        0     1694 2023-05-23 15:58:36.848724 embedbase_client-0.1.4/embedbase_client/model.py
--rw-r--r--   0        0        0     3388 2023-05-23 15:58:36.848724 embedbase_client-0.1.4/embedbase_client/split.py
--rw-r--r--   0        0        0    15373 2023-05-23 15:58:36.848724 embedbase_client-0.1.4/embedbase_client/sync_client.py
--rw-r--r--   0        0        0     2051 2023-05-23 15:58:36.848724 embedbase_client-0.1.4/embedbase_client/utils.py
--rw-r--r--   0        0        0     3535 2023-05-23 15:58:36.848724 embedbase_client-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     2102 1970-01-01 00:00:00.000000 embedbase_client-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-05-25 18:21:51.616626 embedbase_client-0.1.5/LICENSE
+-rw-r--r--   0        0        0     1005 2023-05-25 18:21:51.616626 embedbase_client-0.1.5/README.md
+-rw-r--r--   0        0        0      389 2023-05-25 18:21:51.616626 embedbase_client-0.1.5/embedbase_client/__init__.py
+-rw-r--r--   0        0        0    16730 2023-05-25 18:21:51.616626 embedbase_client-0.1.5/embedbase_client/async_client.py
+-rw-r--r--   0        0        0      913 2023-05-25 18:21:51.616626 embedbase_client-0.1.5/embedbase_client/base.py
+-rw-r--r--   0        0        0     1150 2023-05-25 18:21:51.616626 embedbase_client-0.1.5/embedbase_client/errors.py
+-rw-r--r--   0        0        0     1694 2023-05-25 18:21:51.616626 embedbase_client-0.1.5/embedbase_client/model.py
+-rw-r--r--   0        0        0     3388 2023-05-25 18:21:51.616626 embedbase_client-0.1.5/embedbase_client/split.py
+-rw-r--r--   0        0        0    16681 2023-05-25 18:21:51.616626 embedbase_client-0.1.5/embedbase_client/sync_client.py
+-rw-r--r--   0        0        0     2051 2023-05-25 18:21:51.616626 embedbase_client-0.1.5/embedbase_client/utils.py
+-rw-r--r--   0        0        0     3535 2023-05-25 18:21:51.616626 embedbase_client-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     2102 1970-01-01 00:00:00.000000 embedbase_client-0.1.5/PKG-INFO
```

### Comparing `embedbase_client-0.1.4/LICENSE` & `embedbase_client-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `embedbase_client-0.1.4/README.md` & `embedbase_client-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `embedbase_client-0.1.4/embedbase_client/async_client.py` & `embedbase_client-0.1.5/embedbase_client/async_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,17 +51,23 @@
         async with httpx.AsyncClient() as client:
             res = await client.post(
                 search_url,
                 headers=headers,
                 json=request_body,
                 timeout=self.client.timeout,
             )
-            if res.status_code != 200:
+            try:
+                data = res.json()
+            except json.JSONDecodeError:
+                # pylint: disable=raise-missing-from
                 raise EmbedbaseAPIException(res.text)
-            data = res.json()
+
+            if res.status_code != 200:
+                raise EmbedbaseAPIException(data.get("error", res.text))
+
             return [
                 SearchSimilarity(
                     id=similarity["id"],
                     similarity=similarity["score"],
                     data=similarity["data"],
                     embedding=similarity["embedding"],
                     hash=similarity["hash"],
@@ -111,17 +117,23 @@
             list_url += f"&limit={self.options['limit']}"
 
         headers = self.client.headers
         async with httpx.AsyncClient() as client:
             res = await client.get(
                 list_url, headers=headers, timeout=self.client.timeout
             )
-            if res.status_code != 200:
+            try:
+                data = res.json()
+            except json.JSONDecodeError:
+                # pylint: disable=raise-missing-from
                 raise EmbedbaseAPIException(res.text)
-            data = res.json()
+
+            if res.status_code != 200:
+                raise EmbedbaseAPIException(data.get("error", res.text))
+
             return [Document(**document) for document in data["documents"]]
 
     def offset(self, offset: int) -> "AsyncListBuilder":
         self.options["offset"] = offset
         return self
 
     def limit(self, limit: int) -> "AsyncListBuilder":
@@ -253,17 +265,23 @@
         ) as client:
             res = await client.post(
                 search_url,
                 headers=self.headers,
                 json={"query": query, "top_k": top_k},
                 timeout=self.timeout,
             )
-        if res.status_code != 200:
+        try:
+            data = res.json()
+        except json.JSONDecodeError:
+            # pylint: disable=raise-missing-from
             raise EmbedbaseAPIException(res.text)
-        data = res.json()
+
+        if res.status_code != 200:
+            raise EmbedbaseAPIException(data.get("error", res.text))
+
         return [similarity["data"] for similarity in data["similarities"]]
 
     def search(
         self, dataset: str, query: str, limit: Optional[int] = None
     ) -> AsyncSearchBuilder:
         """
         Search for documents similar to the given query in the specified dataset asynchronously.
@@ -302,17 +320,22 @@
         ) as client:
             res = await client.post(
                 add_url,
                 headers=self.headers,
                 json={"documents": [{"data": document, "metadata": metadata}]},
                 timeout=self.timeout,
             )
-        if res.status_code != 200:
+        try:
+            data = res.json()
+        except json.JSONDecodeError:
+            # pylint: disable=raise-missing-from
             raise EmbedbaseAPIException(res.text)
-        data = res.json()
+
+        if res.status_code != 200:
+            raise EmbedbaseAPIException(data.get("error", res.text))
         return Document(**data["results"][0])
 
     async def batch_add(
         self, dataset: str, documents: List[Dict[str, Any]]
     ) -> List[Document]:
         """
         Add multiple documents to the specified dataset in a single batch asynchronously.
@@ -337,17 +360,23 @@
         ) as client:
             res = await client.post(
                 add_url,
                 headers=self.headers,
                 json={"documents": documents},
                 timeout=self.timeout,
             )
-        if res.status_code != 200:
+
+        try:
+            data = res.json()
+        except json.JSONDecodeError:
+            # pylint: disable=raise-missing-from
             raise EmbedbaseAPIException(res.text)
-        data = res.json()
+
+        if res.status_code != 200:
+            raise EmbedbaseAPIException(data.get("error", res.text))
 
         return [Document(**result) for result in data["results"]]
 
     async def clear(self, dataset: str) -> None:
         """
         Clear all documents from the specified dataset asynchronously.
         Args:
@@ -356,17 +385,23 @@
             await embedbase.clear("my_dataset")
         """
         url = f"/{dataset}/clear"
         async with httpx.AsyncClient(
             app=self.fastapi_app, base_url=self.embedbase_url
         ) as client:
             res = await client.get(url, headers=self.headers, timeout=self.timeout)
-        if res.status_code != 200:
+        try:
+            data = res.json()
+        except json.JSONDecodeError:
+            # pylint: disable=raise-missing-from
             raise EmbedbaseAPIException(res.text)
 
+        if res.status_code != 200:
+            raise EmbedbaseAPIException(data.get("error", res.text))
+
     async def datasets(self) -> List[ClientDatasets]:
         """
         Retrieve a list of all datasets asynchronously.
         Returns:
             A list of dataset names.
         Example usage
             results = await embedbase.datasets()
@@ -374,17 +409,23 @@
         datasets_url = "/datasets"
         async with httpx.AsyncClient(
             app=self.fastapi_app, base_url=self.embedbase_url
         ) as client:
             res = await client.get(
                 datasets_url, headers=self.headers, timeout=self.timeout
             )
-        if res.status_code != 200:
+        try:
+            data = res.json()
+        except json.JSONDecodeError:
+            # pylint: disable=raise-missing-from
             raise EmbedbaseAPIException(res.text)
-        data = res.json()
+
+        if res.status_code != 200:
+            raise EmbedbaseAPIException(data.get("error", res.text))
+
         return [ClientDatasets(**dataset) for dataset in data["datasets"]]
 
     def list(self, dataset: str) -> AsyncListBuilder:
         """
         Retrieve a list of all documents in the specified dataset asynchronously.
 
         Args:
```

### Comparing `embedbase_client-0.1.4/embedbase_client/base.py` & `embedbase_client-0.1.5/embedbase_client/base.py`

 * *Files identical despite different names*

### Comparing `embedbase_client-0.1.4/embedbase_client/errors.py` & `embedbase_client-0.1.5/embedbase_client/errors.py`

 * *Files 13% similar despite different names*

```diff
@@ -30,13 +30,12 @@
     # in python2 via `error.message`. Unlike `str(error)`, it omits "Request
     # req_..." from the beginning of the string.
     @property
     def user_message(self):
         return self._message
 
     def __repr__(self):
-        return "%s(message=%r, http_status=%r, request_id=%r)" % (
+        return "%s(message=%r, http_status=%r)" % (
             self.__class__.__name__,
             self._message,
             self.http_status,
-            self.request_id,
         )
```

### Comparing `embedbase_client-0.1.4/embedbase_client/model.py` & `embedbase_client-0.1.5/embedbase_client/model.py`

 * *Files identical despite different names*

### Comparing `embedbase_client-0.1.4/embedbase_client/split.py` & `embedbase_client-0.1.5/embedbase_client/split.py`

 * *Files identical despite different names*

### Comparing `embedbase_client-0.1.4/embedbase_client/sync_client.py` & `embedbase_client-0.1.5/embedbase_client/sync_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,21 @@
 
 import json
 from dataclasses import dataclass
 
 import requests
 from embedbase_client.base import BaseClient
 from embedbase_client.errors import EmbedbaseAPIException
-from embedbase_client.model import ClientDatasets, Document, GenerateOptions, Metadata, SearchSimilarity
+from embedbase_client.model import (
+    ClientDatasets,
+    Document,
+    GenerateOptions,
+    Metadata,
+    SearchSimilarity,
+)
 from embedbase_client.utils import sync_stream
 
 
 class SyncSearchBuilder:
     def __init__(
         self,
         client: BaseClient,
@@ -51,17 +57,23 @@
         if "where" in self.options:
             request_body["where"] = self.options["where"]
 
         headers = self.client.headers
         res = requests.post(
             search_url, headers=headers, json=request_body, timeout=self.client.timeout
         )
-        if res.status_code != 200:
+        try:
+            data = res.json()
+        except json.JSONDecodeError:
+            # pylint: disable=raise-missing-from
             raise EmbedbaseAPIException(res.text)
-        data = res.json()
+
+        if res.status_code != 200:
+            raise EmbedbaseAPIException(data.get("error", res.text))
+
         return [
             SearchSimilarity(
                 id=similarity["id"],
                 similarity=similarity["score"],
                 data=similarity["data"],
                 embedding=similarity["embedding"],
                 hash=similarity["hash"],
@@ -99,17 +111,23 @@
         if "offset" in self.options:
             list_url += f"?offset={self.options['offset']}"
         if "limit" in self.options:
             list_url += f"&limit={self.options['limit']}"
 
         headers = self.client.headers
         res = requests.get(list_url, headers=headers, timeout=self.client.timeout)
-        if res.status_code != 200:
+        try:
+            data = res.json()
+        except json.JSONDecodeError:
+            # pylint: disable=raise-missing-from
             raise EmbedbaseAPIException(res.text)
-        data = res.json()
+
+        if res.status_code != 200:
+            raise EmbedbaseAPIException(data.get("error", res.text))
+
         return [Document(**document) for document in data["documents"]]
 
     def offset(self, offset: int) -> "SyncListBuilder":
         self.options["offset"] = offset
         return self
 
     def limit(self, limit: int) -> "SyncListBuilder":
@@ -258,17 +276,23 @@
         search_url = f"{self.embedbase_url}/{dataset}/search"
         res = requests.post(
             search_url,
             headers=self.headers,
             json={"query": query, "top_k": top_k},
             timeout=self.timeout,
         )
-        if res.status_code != 200:
+        try:
+            data = res.json()
+        except json.JSONDecodeError:
+            # pylint: disable=raise-missing-from
             raise EmbedbaseAPIException(res.text)
-        data = res.json()
+
+        if res.status_code != 200:
+            raise EmbedbaseAPIException(data.get("error", res.text))
+
         return [similarity["data"] for similarity in data["similarities"]]
 
     def search(
         self, dataset: str, query: str, limit: Optional[int] = None
     ) -> SyncSearchBuilder:
         """
         Search for documents similar to the given query in the specified dataset.
@@ -314,16 +338,23 @@
         add_url = f"{self.embedbase_url}/{dataset}"
         res = requests.post(
             add_url,
             headers=self.headers,
             json={"documents": [{"data": document, "metadata": metadata}]},
             timeout=self.timeout,
         )
-        if res.status_code != 200:
+        try:
+            data = res.json()
+        except json.JSONDecodeError:
+            # pylint: disable=raise-missing-from
             raise EmbedbaseAPIException(res.text)
+
+        if res.status_code != 200:
+            raise EmbedbaseAPIException(data.get("error", res.text))
+
         data = res.json()
 
         return Document(
             **data["results"][0],
         )
 
     def batch_add(
@@ -349,17 +380,23 @@
         add_url = f"{self.embedbase_url}/{dataset}"
         res = requests.post(
             add_url,
             headers=self.headers,
             json={"documents": documents},
             timeout=self.timeout,
         )
-        if res.status_code != 200:
+        try:
+            data = res.json()
+        except json.JSONDecodeError:
+            # pylint: disable=raise-missing-from
             raise EmbedbaseAPIException(res.text)
-        data = res.json()
+
+        if res.status_code != 200:
+            raise EmbedbaseAPIException(data.get("error", res.text))
+
         return [
             Document(
                 **result,
             )
             for result in data["results"]
         ]
 
@@ -371,17 +408,23 @@
             dataset: The name of the dataset to clear.
 
         Example usage:
             embedbase.clear("my_dataset")
         """
         url = f"{self.embedbase_url}/{dataset}/clear"
         res = requests.get(url, headers=self.headers, timeout=self.timeout)
-        if res.status_code != 200:
+        try:
+            data = res.json()
+        except json.JSONDecodeError:
+            # pylint: disable=raise-missing-from
             raise EmbedbaseAPIException(res.text)
 
+        if res.status_code != 200:
+            raise EmbedbaseAPIException(data.get("error", res.text))
+
     def dataset(self, dataset: str) -> Dataset:
         return Dataset(client=self, dataset=dataset)
 
     def datasets(self) -> List[ClientDatasets]:
         """
         Retrieve a list of all datasets.
 
@@ -389,17 +432,23 @@
             A list of dataset names and metadata.
 
         Example usage:
             datasets = embedbase.datasets()
         """
         datasets_url = f"{self.embedbase_url}/datasets"
         res = requests.get(datasets_url, headers=self.headers, timeout=self.timeout)
-        if res.status_code != 200:
+        try:
+            data = res.json()
+        except json.JSONDecodeError:
+            # pylint: disable=raise-missing-from
             raise EmbedbaseAPIException(res.text)
-        data = res.json()
+
+        if res.status_code != 200:
+            raise EmbedbaseAPIException(data.get("error", res.text))
+
         return [ClientDatasets(**dataset) for dataset in data["datasets"]]
 
     def list(self, dataset: str) -> SyncListBuilder:
         """
         Retrieve a list of all documents in the specified dataset.
 
         Args:
@@ -409,15 +458,17 @@
             A list of document IDs and metadata.
 
         Example usage:
             documents = embedbase.list("my_dataset")
         """
         return SyncListBuilder(self, dataset, {})
 
-    def generate(self, prompt: str, options: GenerateOptions = None) -> Generator[str, None, None]:
+    def generate(
+        self, prompt: str, options: GenerateOptions = None
+    ) -> Generator[str, None, None]:
         """
         Generate text from an LLM using a synchronous generator that fetches generated text data in chunks.
 
         Args:
             prompt (str): The text prompt to send to the API for generating responses.
             options (dict, optional): Options for the generation process, including history.
                                     Defaults to None.
```

### Comparing `embedbase_client-0.1.4/embedbase_client/utils.py` & `embedbase_client-0.1.5/embedbase_client/utils.py`

 * *Files identical despite different names*

### Comparing `embedbase_client-0.1.4/pyproject.toml` & `embedbase_client-0.1.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Poetry pyproject.toml: https://python-poetry.org/docs/pyproject/
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "embedbase-client"
-version = "0.1.4"
+version = "0.1.5"
 description = "Python client for Embedbase"
 readme = "README.md"
 authors = ["Different AI <louis@embedbase.xyz>"]
 license = "MIT"
 repository = "https://github.com/different-ai/embedbase/tree/main/sdk/embedbase-py"
 homepage = "https://github.com/different-ai/embedbase/tree/main/sdk/embedbase-py"
```

### Comparing `embedbase_client-0.1.4/PKG-INFO` & `embedbase_client-0.1.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: embedbase-client
-Version: 0.1.4
+Version: 0.1.5
 Summary: Python client for Embedbase
 Home-page: https://github.com/different-ai/embedbase/tree/main/sdk/embedbase-py
 License: MIT
 Keywords: embeddings,machine learning,artificial intelligence,llm
 Author: Different AI
 Author-email: louis@embedbase.xyz
 Requires-Python: >=3.8,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: embedbase-client Version: 0.1.4 Summary: Python
+Metadata-Version: 2.1 Name: embedbase-client Version: 0.1.5 Summary: Python
 client for Embedbase Home-page: https://github.com/different-ai/embedbase/tree/
 main/sdk/embedbase-py License: MIT Keywords: embeddings,machine
 learning,artificial intelligence,llm Author: Different AI Author-email:
 louis@embedbase.xyz Requires-Python: >=3.8,<4.0 Classifier: Development Status
 :: 4 - Beta Classifier: Intended Audience :: Developers Classifier: License ::
 OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
```

