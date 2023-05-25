# Comparing `tmp/paper-qa-1.8.0.tar.gz` & `tmp/paper-qa-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paper-qa-1.8.0.tar", last modified: Mon May 22 16:09:54 2023, max compression
+gzip compressed data, was "paper-qa-1.9.0.tar", last modified: Thu May 25 13:45:02 2023, max compression
```

## Comparing `paper-qa-1.8.0.tar` & `paper-qa-1.9.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:09:54.293750 paper-qa-1.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-22 16:09:10.000000 paper-qa-1.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12585 2023-05-22 16:09:54.293750 paper-qa-1.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12150 2023-05-22 16:09:10.000000 paper-qa-1.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:09:54.293750 paper-qa-1.8.0/paper_qa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12585 2023-05-22 16:09:54.000000 paper-qa-1.8.0/paper_qa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-22 16:09:54.000000 paper-qa-1.8.0/paper_qa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 16:09:54.000000 paper-qa-1.8.0/paper_qa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-22 16:09:54.000000 paper-qa-1.8.0/paper_qa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-22 16:09:54.000000 paper-qa-1.8.0/paper_qa.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:09:54.293750 paper-qa-1.8.0/paperqa/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-22 16:09:10.000000 paper-qa-1.8.0/paperqa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5855 2023-05-22 16:09:10.000000 paper-qa-1.8.0/paperqa/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:09:54.293750 paper-qa-1.8.0/paperqa/contrib/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-22 16:09:10.000000 paper-qa-1.8.0/paperqa/contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11743 2023-05-22 16:09:10.000000 paper-qa-1.8.0/paperqa/contrib/zotero.py
--rw-r--r--   0 runner    (1001) docker     (123)    20314 2023-05-22 16:09:10.000000 paper-qa-1.8.0/paperqa/docs.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-22 16:09:10.000000 paper-qa-1.8.0/paperqa/paths.py
--rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-05-22 16:09:10.000000 paper-qa-1.8.0/paperqa/qaprompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     6773 2023-05-22 16:09:10.000000 paper-qa-1.8.0/paperqa/readers.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-22 16:09:10.000000 paper-qa-1.8.0/paperqa/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-05-22 16:09:10.000000 paper-qa-1.8.0/paperqa/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-22 16:09:10.000000 paper-qa-1.8.0/paperqa/version.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 16:09:54.293750 paper-qa-1.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-05-22 16:09:10.000000 paper-qa-1.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:09:54.293750 paper-qa-1.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    12936 2023-05-22 16:09:10.000000 paper-qa-1.8.0/tests/test_paperqa.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:45:02.333935 paper-qa-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-25 13:44:23.000000 paper-qa-1.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12585 2023-05-25 13:45:02.333935 paper-qa-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12150 2023-05-25 13:44:23.000000 paper-qa-1.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:45:02.329935 paper-qa-1.9.0/paper_qa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12585 2023-05-25 13:45:02.000000 paper-qa-1.9.0/paper_qa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-25 13:45:02.000000 paper-qa-1.9.0/paper_qa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 13:45:02.000000 paper-qa-1.9.0/paper_qa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-25 13:45:02.000000 paper-qa-1.9.0/paper_qa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-25 13:45:02.000000 paper-qa-1.9.0/paper_qa.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:45:02.333935 paper-qa-1.9.0/paperqa/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-25 13:44:23.000000 paper-qa-1.9.0/paperqa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5855 2023-05-25 13:44:23.000000 paper-qa-1.9.0/paperqa/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:45:02.333935 paper-qa-1.9.0/paperqa/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-25 13:44:23.000000 paper-qa-1.9.0/paperqa/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11743 2023-05-25 13:44:23.000000 paper-qa-1.9.0/paperqa/contrib/zotero.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21407 2023-05-25 13:44:23.000000 paper-qa-1.9.0/paperqa/docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-25 13:44:23.000000 paper-qa-1.9.0/paperqa/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-05-25 13:44:23.000000 paper-qa-1.9.0/paperqa/qaprompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6773 2023-05-25 13:44:23.000000 paper-qa-1.9.0/paperqa/readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-25 13:44:23.000000 paper-qa-1.9.0/paperqa/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-05-25 13:44:23.000000 paper-qa-1.9.0/paperqa/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-25 13:44:23.000000 paper-qa-1.9.0/paperqa/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 13:45:02.333935 paper-qa-1.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-05-25 13:44:23.000000 paper-qa-1.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:45:02.333935 paper-qa-1.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    14167 2023-05-25 13:44:23.000000 paper-qa-1.9.0/tests/test_paperqa.py
```

### Comparing `paper-qa-1.8.0/LICENSE` & `paper-qa-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `paper-qa-1.8.0/PKG-INFO` & `paper-qa-1.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paper-qa
-Version: 1.8.0
+Version: 1.9.0
 Summary: LLM Chain for answering questions from docs 
 Home-page: https://github.com/whitead/paper-qa
 Author: Andrew White
 Author-email: white.d.andrew@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `paper-qa-1.8.0/README.md` & `paper-qa-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `paper-qa-1.8.0/paper_qa.egg-info/PKG-INFO` & `paper-qa-1.9.0/paper_qa.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paper-qa
-Version: 1.8.0
+Version: 1.9.0
 Summary: LLM Chain for answering questions from docs 
 Home-page: https://github.com/whitead/paper-qa
 Author: Andrew White
 Author-email: white.d.andrew@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `paper-qa-1.8.0/paperqa/agent.py` & `paper-qa-1.9.0/paperqa/agent.py`

 * *Files identical despite different names*

### Comparing `paper-qa-1.8.0/paperqa/contrib/zotero.py` & `paper-qa-1.9.0/paperqa/contrib/zotero.py`

 * *Files identical despite different names*

### Comparing `paper-qa-1.8.0/paperqa/docs.py` & `paper-qa-1.9.0/paperqa/docs.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,16 +16,22 @@
 from langchain.docstore.document import Document
 from langchain.embeddings.base import Embeddings
 from langchain.embeddings.openai import OpenAIEmbeddings
 from langchain.llms.base import LLM
 from langchain.vectorstores import FAISS
 
 from .paths import CACHE_PATH
-from .qaprompts import (citation_prompt, make_chain, qa_prompt, search_prompt,
-                        select_paper_prompt, summary_prompt)
+from .qaprompts import (
+    citation_prompt,
+    make_chain,
+    qa_prompt,
+    search_prompt,
+    select_paper_prompt,
+    summary_prompt,
+)
 from .readers import read_doc
 from .types import Answer, Context
 from .utils import maybe_is_text, md5sum
 
 os.makedirs(os.path.dirname(CACHE_PATH), exist_ok=True)
 langchain.llm_cache = SQLiteCache(CACHE_PATH)
 
@@ -61,22 +67,23 @@
         if index_path is None:
             index_path = Path.home() / ".paperqa" / name
         self.index_path = index_path
         self.name = name
         if embeddings is None:
             embeddings = OpenAIEmbeddings()
         self.embeddings = embeddings
+        self._deleted_keys = set()
 
     def update_llm(
         self,
         llm: Optional[Union[LLM, str]] = None,
         summary_llm: Optional[Union[LLM, str]] = None,
     ) -> None:
         """Update the LLM for answering questions."""
-        if llm is None:
+        if llm is None and os.environ.get("OPENAI_API_KEY") is not None:
             llm = "gpt-3.5-turbo"
         if type(llm) is str:
             llm = ChatOpenAI(temperature=0.1, model_name=llm)
         if type(summary_llm) is str:
             summary_llm = ChatOpenAI(temperature=0.1, model_name=summary_llm)
         self.llm = llm
         if summary_llm is None:
@@ -108,19 +115,21 @@
         # first check to see if we already have this document
         # this way we don't make api call to create citation on file we already have
         hash = md5sum(path)
         if hash in [d["hash"] for d in self.docs]:
             raise ValueError(f"Document {path} already in collection.")
 
         if citation is None:
-            cite_chain = make_chain(prompt=citation_prompt, llm=self.summary_llm)
+            cite_chain = make_chain(
+                prompt=citation_prompt, llm=self.summary_llm)
             # peak first chunk
             texts, _ = read_doc(path, "", "", chunk_chars=chunk_chars)
             if len(texts) == 0:
-                raise ValueError(f"Could not read document {path}. Is it empty?")
+                raise ValueError(
+                    f"Could not read document {path}. Is it empty?")
             citation = cite_chain.run(texts[0])
             if len(citation) < 3 or "Unknown" in citation or "insufficient" in citation:
                 citation = f"Unknown, {os.path.basename(path)}, {datetime.now().year}"
 
         if key is None:
             # get first name and year from citation
             try:
@@ -132,15 +141,16 @@
                 )
             try:
                 year = re.search(r"(\d{4})", citation).group(1)
             except AttributeError:
                 year = ""
             key = f"{author}{year}"
         key = self.get_unique_key(key)
-        texts, metadata = read_doc(path, citation, key, chunk_chars=chunk_chars)
+        texts, metadata = read_doc(
+            path, citation, key, chunk_chars=chunk_chars)
         # loose check to see if document was loaded
         #
         if len("".join(texts)) < 10 or (
             not disable_check and not maybe_is_text("".join(texts))
         ):
             raise ValueError(
                 f"This does not look like a text document: {path}. Path disable_check to ignore this error."
@@ -184,14 +194,22 @@
                 key=key,
                 hash=hash,
                 text_embeddings=text_embeddings,
             )
         )
         self.keys.add(key)
 
+    def delete(self, key: str) -> None:
+        """Delete a document from the collection."""
+        if key not in self.keys:
+            return
+        self.keys.remove(key)
+        self.docs = [doc for doc in self.docs if doc["key"] != key]
+        self._deleted_keys.add(key)
+
     def clear(self) -> None:
         """Clear the collection of documents."""
         self.docs = []
         self.keys = set()
         self._faiss_index = None
         self._doc_index = None
         # delete index file
@@ -217,19 +235,24 @@
         self, query: str, k: int = 25, callbacks: List[AsyncCallbackHandler] = []
     ) -> List[str]:
         """Return a list of documents that match the query."""
         if len(self.docs) == 0:
             return ""
         if self._doc_index is None:
             texts = [doc["metadata"][0]["citation"] for doc in self.docs]
-            metadatas = [{"key": doc["metadata"][0]["dockey"]} for doc in self.docs]
+            metadatas = [{"key": doc["metadata"][0]["dockey"]}
+                         for doc in self.docs]
             self._doc_index = FAISS.from_texts(
                 texts, metadatas=metadatas, embedding=self.embeddings
             )
-        docs = self._doc_index.max_marginal_relevance_search(query, k=k)
+        docs = self._doc_index.max_marginal_relevance_search(
+            query, k=k + len(self._deleted_keys)
+        )
+        docs = [doc for doc in docs if doc.metadata["key"]
+                not in self._deleted_keys]
         chain = make_chain(select_paper_prompt, self.summary_llm)
         papers = [f"{d.metadata['key']}: {d.page_content}" for d in docs]
         result = await chain.arun(
             instructions=query, papers="\n".join(papers), callbacks=callbacks
         )
         return result
 
@@ -237,19 +260,24 @@
         self, query: str, k: int = 25, callbacks: List[AsyncCallbackHandler] = []
     ) -> List[str]:
         """Return a list of documents that match the query."""
         if len(self.docs) == 0:
             return ""
         if self._doc_index is None:
             texts = [doc["metadata"][0]["citation"] for doc in self.docs]
-            metadatas = [{"key": doc["metadata"][0]["dockey"]} for doc in self.docs]
+            metadatas = [{"key": doc["metadata"][0]["dockey"]}
+                         for doc in self.docs]
             self._doc_index = FAISS.from_texts(
                 texts, metadatas=metadatas, embedding=self.embeddings
             )
-        docs = self._doc_index.max_marginal_relevance_search(query, k=k)
+        docs = self._doc_index.max_marginal_relevance_search(
+            query, k=k + len(self._deleted_keys)
+        )
+        docs = [doc for doc in docs if doc.metadata["key"]
+                not in self._deleted_keys]
         chain = make_chain(select_paper_prompt, self.summary_llm)
         papers = [f"{d.metadata['key']}: {d.page_content}" for d in docs]
         result = chain.run(
             instructions=query, papers="\n".join(papers), callbacks=callbacks
         )
         return result
 
@@ -260,27 +288,33 @@
         del state["_faiss_index"]
         del state["_doc_index"]
         return state
 
     def __setstate__(self, state):
         self.__dict__.update(state)
         try:
-            self._faiss_index = FAISS.load_local(self.index_path, self.embeddings)
+            self._faiss_index = FAISS.load_local(
+                self.index_path, self.embeddings)
         except:
             # they use some special exception type, but I don't want to import it
             self._faiss_index = None
         if not hasattr(self, "_doc_index"):
             self._doc_index = None
+        # must be a better way to have backwards compatibility
+        if not hasattr(self, "_deleted_keys"):
+            self._deleted_keys = set()
         self.update_llm(None, None)
 
     def _build_faiss_index(self):
         if self._faiss_index is None:
-            texts = reduce(lambda x, y: x + y, [doc["texts"] for doc in self.docs], [])
+            texts = reduce(lambda x, y: x + y,
+                           [doc["texts"] for doc in self.docs], [])
             text_embeddings = reduce(
-                lambda x, y: x + y, [doc["text_embeddings"] for doc in self.docs], []
+                lambda x, y: x + y, [doc["text_embeddings"]
+                                     for doc in self.docs], []
             )
             metadatas = reduce(
                 lambda x, y: x + y, [doc["metadata"] for doc in self.docs], []
             )
             self._faiss_index = FAISS.from_embeddings(
                 # wow adding list to the zip was tricky
                 text_embeddings=list(zip(texts, text_embeddings)),
@@ -341,14 +375,16 @@
             )
         else:
             docs = self._faiss_index.similarity_search(
                 answer.question, k=_k, fetch_k=5 * _k
             )
 
         async def process(doc):
+            if doc.metadata["dockey"] in self._deleted_keys:
+                return None, None
             if key_filter is not None and doc.metadata["dockey"] not in key_filter:
                 return None, None
             # check if it is already in answer (possible in agent setting)
             if doc.metadata["key"] in [c.key for c in answer.contexts]:
                 return None, None
             callbacks = [OpenAICallbackHandler()] + get_callbacks(
                 "evidence:" + doc.metadata["key"]
```

### Comparing `paper-qa-1.8.0/paperqa/qaprompts.py` & `paper-qa-1.9.0/paperqa/qaprompts.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,15 @@
 from datetime import datetime
 from typing import Any, Dict, List, Optional
 
 import langchain.prompts as prompts
 from langchain.callbacks.manager import AsyncCallbackManagerForChainRun
 from langchain.chains import LLMChain
 from langchain.chat_models import ChatOpenAI
-from langchain.prompts.chat import (ChatPromptTemplate,
-                                    HumanMessagePromptTemplate)
+from langchain.prompts.chat import ChatPromptTemplate, HumanMessagePromptTemplate
 from langchain.schema import LLMResult, SystemMessage
 
 summary_prompt = prompts.PromptTemplate(
     input_variables=["question", "context_str", "citation"],
     template="Summarize and provide direct quotes from the text below to help answer a question. "
     "Do not directly answer the question, instead summarize and "
     "quote to give evidence to help answer the question. "
```

### Comparing `paper-qa-1.8.0/paperqa/readers.py` & `paper-qa-1.9.0/paperqa/readers.py`

 * *Files identical despite different names*

### Comparing `paper-qa-1.8.0/paperqa/types.py` & `paper-qa-1.9.0/paperqa/types.py`

 * *Files identical despite different names*

### Comparing `paper-qa-1.8.0/paperqa/utils.py` & `paper-qa-1.9.0/paperqa/utils.py`

 * *Files identical despite different names*

### Comparing `paper-qa-1.8.0/setup.py` & `paper-qa-1.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `paper-qa-1.8.0/tests/test_paperqa.py` & `paper-qa-1.9.0/tests/test_paperqa.py`

 * *Files 5% similar despite different names*

```diff
@@ -308,14 +308,44 @@
         f.write(r.text)
         f.write("\n")  # so we don't have same hash
     docs.add("example.txt", "WikiMedia Foundation, 2023, Accessed now", key="test")
     answer = paperqa.Answer("What country is Bates from?")
     docs.get_evidence(answer, key_filter=["test"])
 
 
+def test_dockey_delete():
+    """Test that we can filter evidence with dockeys"""
+    doc_path = "example2.txt"
+    with open(doc_path, "w", encoding="utf-8") as f:
+        # get wiki page about politician
+        r = requests.get("https://en.wikipedia.org/wiki/Frederick_Bates_(politician)")
+        f.write(r.text)
+    docs = paperqa.Docs()
+    docs.add(doc_path, "WikiMedia Foundation, 2023, Accessed now")
+    # add with new dockey
+    with open("example.txt", "w", encoding="utf-8") as f:
+        f.write(r.text)
+        f.write("\n\nBates could be from Angola")  # so we don't have same hash
+    docs.add("example.txt", "WikiMedia Foundation, 2023, Accessed now", key="test")
+    answer = paperqa.Answer("What country is Bates from?")
+    answer = docs.get_evidence(answer, marginal_relevance=False)
+    keys = set([c.key for c in answer.contexts])
+    assert len(keys) == 2
+    assert len(docs.docs) == 2
+    assert len(docs.keys) == 2
+
+    docs.delete("test")
+    assert len(docs.docs) == 1
+    assert len(docs.keys) == 1
+    answer = paperqa.Answer("What country is Bates from?")
+    answer = docs.get_evidence(answer, marginal_relevance=False)
+    keys = set([c.key for c in answer.contexts])
+    assert len(keys) == 1
+
+
 def test_query_filter():
     """Test that we can filter evidence with in query"""
     doc_path = "example2.txt"
     with open(doc_path, "w", encoding="utf-8") as f:
         # get wiki page about politician
         r = requests.get("https://en.wikipedia.org/wiki/Frederick_Bates_(politician)")
         f.write(r.text)
```

