# Comparing `tmp/aars-0.7.1.tar.gz` & `tmp/aars-0.7.2.tar.gz`

## Comparing `aars-0.7.1.tar` & `aars-0.7.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 aars-0.7.1/docs-requirements.txt
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 aars-0.7.1/mkdocs.yml
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 aars-0.7.1/requirements.txt
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 aars-0.7.1/.github/workflows/mkdocs-gh-pages.yml
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 aars-0.7.1/.github/workflows/publish.yml
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 aars-0.7.1/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     4932 2020-02-02 00:00:00.000000 aars-0.7.1/docs/FastAPI_Cookbook.md
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 aars-0.7.1/docs/index.md -> ../README.md
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 aars-0.7.1/docs/Code_Reference/Exceptions.md
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 aars-0.7.1/docs/Code_Reference/utils.md
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 aars-0.7.1/docs/Code_Reference/core/AARS.md
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 aars-0.7.1/docs/Code_Reference/core/Index.md
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 aars-0.7.1/docs/Code_Reference/core/Record.md
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 aars-0.7.1/src/aars/__init__.py
--rw-r--r--   0        0        0    39839 2020-02-02 00:00:00.000000 aars-0.7.1/src/aars/core.py
--rw-r--r--   0        0        0     3400 2020-02-02 00:00:00.000000 aars-0.7.1/src/aars/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aars-0.7.1/src/aars/py.typed
--rw-r--r--   0        0        0    12396 2020-02-02 00:00:00.000000 aars-0.7.1/src/aars/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aars-0.7.1/tests/__init__.py
--rw-r--r--   0        0        0     6411 2020-02-02 00:00:00.000000 aars-0.7.1/tests/aars.py
--rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 aars-0.7.1/.gitignore
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 aars-0.7.1/LICENSE
--rw-r--r--   0        0        0     3322 2020-02-02 00:00:00.000000 aars-0.7.1/README.md
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 aars-0.7.1/pyproject.toml
--rw-r--r--   0        0        0     3802 2020-02-02 00:00:00.000000 aars-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 aars-0.7.2/docs-requirements.txt
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 aars-0.7.2/mkdocs.yml
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 aars-0.7.2/requirements.txt
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 aars-0.7.2/.github/workflows/mkdocs-gh-pages.yml
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 aars-0.7.2/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 aars-0.7.2/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     4932 2020-02-02 00:00:00.000000 aars-0.7.2/docs/FastAPI_Cookbook.md
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 aars-0.7.2/docs/index.md -> ../README.md
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 aars-0.7.2/docs/Code_Reference/Exceptions.md
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 aars-0.7.2/docs/Code_Reference/utils.md
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 aars-0.7.2/docs/Code_Reference/core/AARS.md
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 aars-0.7.2/docs/Code_Reference/core/Index.md
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 aars-0.7.2/docs/Code_Reference/core/Record.md
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 aars-0.7.2/src/aars/__init__.py
+-rw-r--r--   0        0        0    40541 2020-02-02 00:00:00.000000 aars-0.7.2/src/aars/core.py
+-rw-r--r--   0        0        0     3916 2020-02-02 00:00:00.000000 aars-0.7.2/src/aars/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aars-0.7.2/src/aars/py.typed
+-rw-r--r--   0        0        0    12396 2020-02-02 00:00:00.000000 aars-0.7.2/src/aars/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aars-0.7.2/tests/__init__.py
+-rw-r--r--   0        0        0     6411 2020-02-02 00:00:00.000000 aars-0.7.2/tests/aars.py
+-rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 aars-0.7.2/.gitignore
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 aars-0.7.2/LICENSE
+-rw-r--r--   0        0        0     3322 2020-02-02 00:00:00.000000 aars-0.7.2/README.md
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 aars-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0     3802 2020-02-02 00:00:00.000000 aars-0.7.2/PKG-INFO
```

### Comparing `aars-0.7.1/mkdocs.yml` & `aars-0.7.2/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `aars-0.7.1/.github/workflows/mkdocs-gh-pages.yml` & `aars-0.7.2/.github/workflows/mkdocs-gh-pages.yml`

 * *Files identical despite different names*

### Comparing `aars-0.7.1/.github/workflows/publish.yml` & `aars-0.7.2/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `aars-0.7.1/.github/workflows/python-publish.yml` & `aars-0.7.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `aars-0.7.1/docs/FastAPI_Cookbook.md` & `aars-0.7.2/docs/FastAPI_Cookbook.md`

 * *Files identical despite different names*

### Comparing `aars-0.7.1/src/aars/core.py` & `aars-0.7.2/src/aars/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     Tuple,
     Optional,
     Generic,
     AsyncIterator,
 )
 
 from aiohttp import ServerDisconnectedError
+from aleph_message.status import MessageStatus
 from pydantic import BaseModel, Field
 
 from aleph.sdk.client import AuthenticatedAlephClient
 from aleph.sdk.types import Account
 from aleph.sdk.chains.ethereum import get_fallback_account
 from aleph.sdk.conf import settings
 from aleph.sdk.vm.cache import VmCache
@@ -44,15 +45,20 @@
     subslices,
     async_iterator_to_list,
     IndexQuery,
     PageableResponse,
     PageableRequest,
     EmptyAsyncIterator,
 )
-from .exceptions import AlreadyForgottenError, AlephPermissionError, NotStoredError
+from .exceptions import (
+    AlreadyForgottenError,
+    AlephPermissionError,
+    NotStoredError,
+    AlephPostError,
+)
 
 logger = logging.getLogger(__name__)
 R = TypeVar("R", bound="Record")
 
 
 class Record(BaseModel, ABC):
     """
@@ -758,14 +764,27 @@
             )
         message, status = await cls.session.create_post(
             post_content=obj.content,
             post_type=post_type,
             channel=channel,
             ref=obj.item_hash,
         )
+        if status not in (MessageStatus.PROCESSED, MessageStatus.PENDING):
+            # retry
+            for i in range(cls.retry_count):
+                message, status = await cls.session.create_post(
+                    post_content=obj.content,
+                    post_type=post_type,
+                    channel=channel,
+                    ref=obj.item_hash,
+                )
+                if status in (MessageStatus.PROCESSED, MessageStatus.PENDING):
+                    break
+                if i == cls.retry_count - 1:
+                    raise AlephPostError(obj, status, message)
         if obj.item_hash is None:
             obj.item_hash = message.item_hash
         obj.revision_hashes.append(message.item_hash)
         obj.current_revision = len(obj.revision_hashes) - 1
         obj.timestamp = message.time
         obj.signer = message.sender
         if cls.cache:
```

### Comparing `aars-0.7.1/src/aars/exceptions.py` & `aars-0.7.2/src/aars/exceptions.py`

 * *Files 9% similar despite different names*

```diff
@@ -98,7 +98,24 @@
         record,
         message="Record '{0}'\nis not stored on Aleph. It is required to store the "
         "record with .save() before calling this method.",
     ):
         self.type = record.content
         self.message = f"{message.format(self.type)}"
         super().__init__(self.message)
+
+
+class AlephPostError(AlephError):
+    """Exception raised when a network request to Aleph fails."""
+
+    def __init__(
+        self,
+        obj,
+        response_code,
+        response,
+        message="Failed to post object '{0}' to Aleph with status {1}: {2}",
+    ):
+        self.obj = obj
+        self.response_code = response_code
+        self.response = response
+        self.message = f"{message.format(self.obj, self.response_code, self.response)}"
+        super().__init__(self.message)
```

### Comparing `aars-0.7.1/src/aars/utils.py` & `aars-0.7.2/src/aars/utils.py`

 * *Files identical despite different names*

### Comparing `aars-0.7.1/tests/aars.py` & `aars-0.7.2/tests/aars.py`

 * *Files identical despite different names*

### Comparing `aars-0.7.1/.gitignore` & `aars-0.7.2/.gitignore`

 * *Files identical despite different names*

### Comparing `aars-0.7.1/LICENSE` & `aars-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aars-0.7.1/README.md` & `aars-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `aars-0.7.1/pyproject.toml` & `aars-0.7.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "aars"
-version = "0.7.1"
+version = "0.7.2"
 authors = [
   { name="Mike Hukiewitz", email="mike.hukiewitz@robotter.ai" },
 ]
 description = "Experimental Object-Document-Mapper using pydantic to store objects on Aleph.im"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `aars-0.7.1/PKG-INFO` & `aars-0.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aars
-Version: 0.7.1
+Version: 0.7.2
 Summary: Experimental Object-Document-Mapper using pydantic to store objects on Aleph.im
 Project-URL: Homepage, https://github.com/aleph-im/active-record-sdk
 Project-URL: Bug Tracker, https://github.com/aleph-im/active-record-sdk/issues
 Author-email: Mike Hukiewitz <mike.hukiewitz@robotter.ai>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

