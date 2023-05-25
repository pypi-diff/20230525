# Comparing `tmp/dagster-azure-0.9.9rc1.tar.gz` & `tmp/dagster-azure-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dagster-azure-0.9.9rc1.tar", last modified: Thu Sep 17 21:08:31 2020, max compression
+gzip compressed data, was "dagster-azure-1.0.5.tar", last modified: Fri Aug 26 13:44:05 2022, max compression
```

## Comparing `dagster-azure-0.9.9rc1.tar` & `dagster-azure-1.0.5.tar`

### file list

```diff
@@ -1,43 +1,31 @@
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:31.000000 dagster-azure-0.9.9rc1/
--rw-r--r--   0 bobchen    (501) staff       (20)    11357 2020-09-17 21:04:59.000000 dagster-azure-0.9.9rc1/LICENSE
--rw-r--r--   0 bobchen    (501) staff       (20)      173 2020-09-17 21:04:59.000000 dagster-azure-0.9.9rc1/MANIFEST.in
--rw-r--r--   0 bobchen    (501) staff       (20)      614 2020-09-17 21:08:31.000000 dagster-azure-0.9.9rc1/PKG-INFO
--rw-r--r--   0 bobchen    (501) staff       (20)      125 2020-09-17 21:04:59.000000 dagster-azure-0.9.9rc1/README.md
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:31.000000 dagster-azure-0.9.9rc1/dagster_azure/
--rw-r--r--   0 bobchen    (501) staff       (20)      156 2020-09-17 21:04:59.000000 dagster-azure-0.9.9rc1/dagster_azure/__init__.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:31.000000 dagster-azure-0.9.9rc1/dagster_azure/adls2/
--rw-r--r--   0 bobchen    (501) staff       (20)      629 2020-09-17 21:04:59.000000 dagster-azure-0.9.9rc1/dagster_azure/adls2/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)     4669 2020-09-17 21:04:59.000000 dagster-azure-0.9.9rc1/dagster_azure/adls2/fake_adls2_resource.py
--rw-r--r--   0 bobchen    (501) staff       (20)     2881 2020-09-17 21:04:59.000000 dagster-azure-0.9.9rc1/dagster_azure/adls2/file_cache.py
--rw-r--r--   0 bobchen    (501) staff       (20)     3744 2020-09-17 21:04:59.000000 dagster-azure-0.9.9rc1/dagster_azure/adls2/file_manager.py
--rw-r--r--   0 bobchen    (501) staff       (20)     1525 2020-09-17 21:04:59.000000 dagster-azure-0.9.9rc1/dagster_azure/adls2/intermediate_storage.py
--rw-r--r--   0 bobchen    (501) staff       (20)     5880 2020-09-17 21:04:59.000000 dagster-azure-0.9.9rc1/dagster_azure/adls2/object_store.py
--rw-r--r--   0 bobchen    (501) staff       (20)     4200 2020-09-17 21:04:59.000000 dagster-azure-0.9.9rc1/dagster_azure/adls2/resources.py
--rw-r--r--   0 bobchen    (501) staff       (20)     5236 2020-09-17 21:04:59.000000 dagster-azure-0.9.9rc1/dagster_azure/adls2/system_storage.py
--rw-r--r--   0 bobchen    (501) staff       (20)     1154 2020-09-17 21:04:59.000000 dagster-azure-0.9.9rc1/dagster_azure/adls2/utils.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:31.000000 dagster-azure-0.9.9rc1/dagster_azure/blob/
--rw-r--r--   0 bobchen    (501) staff       (20)      150 2020-09-17 21:04:59.000000 dagster-azure-0.9.9rc1/dagster_azure/blob/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)     7816 2020-09-17 21:04:59.000000 dagster-azure-0.9.9rc1/dagster_azure/blob/compute_log_manager.py
--rw-r--r--   0 bobchen    (501) staff       (20)     4805 2020-09-17 21:04:59.000000 dagster-azure-0.9.9rc1/dagster_azure/blob/fake_blob_client.py
--rw-r--r--   0 bobchen    (501) staff       (20)     1258 2020-09-17 21:04:59.000000 dagster-azure-0.9.9rc1/dagster_azure/blob/utils.py
--rw-r--r--   0 bobchen    (501) staff       (20)       27 2020-09-17 21:04:59.000000 dagster-azure-0.9.9rc1/dagster_azure/version.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:31.000000 dagster-azure-0.9.9rc1/dagster_azure.egg-info/
--rw-r--r--   0 bobchen    (501) staff       (20)      614 2020-09-17 21:08:31.000000 dagster-azure-0.9.9rc1/dagster_azure.egg-info/PKG-INFO
--rw-r--r--   0 bobchen    (501) staff       (20)     1210 2020-09-17 21:08:31.000000 dagster-azure-0.9.9rc1/dagster_azure.egg-info/SOURCES.txt
--rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:08:31.000000 dagster-azure-0.9.9rc1/dagster_azure.egg-info/dependency_links.txt
--rw-r--r--   0 bobchen    (501) staff       (20)       62 2020-09-17 21:08:31.000000 dagster-azure-0.9.9rc1/dagster_azure.egg-info/entry_points.txt
--rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:08:31.000000 dagster-azure-0.9.9rc1/dagster_azure.egg-info/not-zip-safe
--rw-r--r--   0 bobchen    (501) staff       (20)       71 2020-09-17 21:08:31.000000 dagster-azure-0.9.9rc1/dagster_azure.egg-info/requires.txt
--rw-r--r--   0 bobchen    (501) staff       (20)       34 2020-09-17 21:08:31.000000 dagster-azure-0.9.9rc1/dagster_azure.egg-info/top_level.txt
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:31.000000 dagster-azure-0.9.9rc1/dagster_azure_tests/
--rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:04:59.000000 dagster-azure-0.9.9rc1/dagster_azure_tests/__init__.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:31.000000 dagster-azure-0.9.9rc1/dagster_azure_tests/adls2_tests/
--rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:04:59.000000 dagster-azure-0.9.9rc1/dagster_azure_tests/adls2_tests/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)      307 2020-09-17 21:04:59.000000 dagster-azure-0.9.9rc1/dagster_azure_tests/adls2_tests/conftest.py
--rw-r--r--   0 bobchen    (501) staff       (20)     1881 2020-09-17 21:04:59.000000 dagster-azure-0.9.9rc1/dagster_azure_tests/adls2_tests/test_adls2_file_cache.py
--rw-r--r--   0 bobchen    (501) staff       (20)     7518 2020-09-17 21:04:59.000000 dagster-azure-0.9.9rc1/dagster_azure_tests/adls2_tests/test_adls2_file_manager.py
--rw-r--r--   0 bobchen    (501) staff       (20)    18490 2020-09-17 21:04:59.000000 dagster-azure-0.9.9rc1/dagster_azure_tests/adls2_tests/test_intermediate_storage.py
--rw-r--r--   0 bobchen    (501) staff       (20)     1636 2020-09-17 21:04:59.000000 dagster-azure-0.9.9rc1/dagster_azure_tests/adls2_tests/test_object_store.py
--rw-r--r--   0 bobchen    (501) staff       (20)       91 2020-09-17 21:04:59.000000 dagster-azure-0.9.9rc1/dagster_azure_tests/test_version.py
--rw-r--r--   0 bobchen    (501) staff       (20)       74 2020-09-17 21:08:31.000000 dagster-azure-0.9.9rc1/setup.cfg
--rw-r--r--   0 bobchen    (501) staff       (20)     1295 2020-09-17 21:04:59.000000 dagster-azure-0.9.9rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:44:05.256004 dagster-azure-1.0.5/
+-rw-r--r--   0 root         (0) root         (0)    11357 2022-08-26 13:33:01.000000 dagster-azure-1.0.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      204 2022-08-26 13:33:01.000000 dagster-azure-1.0.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      670 2022-08-26 13:44:05.256004 dagster-azure-1.0.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      125 2022-08-26 13:33:01.000000 dagster-azure-1.0.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:44:05.248005 dagster-azure-1.0.5/dagster_azure/
+-rw-r--r--   0 root         (0) root         (0)      157 2022-08-26 13:33:01.000000 dagster-azure-1.0.5/dagster_azure/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:44:05.252004 dagster-azure-1.0.5/dagster_azure/adls2/
+-rw-r--r--   0 root         (0) root         (0)      330 2022-08-26 13:33:01.000000 dagster-azure-1.0.5/dagster_azure/adls2/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6001 2022-08-26 13:33:01.000000 dagster-azure-1.0.5/dagster_azure/adls2/fake_adls2_resource.py
+-rw-r--r--   0 root         (0) root         (0)     4091 2022-08-26 13:33:01.000000 dagster-azure-1.0.5/dagster_azure/adls2/file_manager.py
+-rw-r--r--   0 root         (0) root         (0)     6609 2022-08-26 13:33:01.000000 dagster-azure-1.0.5/dagster_azure/adls2/io_manager.py
+-rw-r--r--   0 root         (0) root         (0)     4176 2022-08-26 13:33:01.000000 dagster-azure-1.0.5/dagster_azure/adls2/resources.py
+-rw-r--r--   0 root         (0) root         (0)     1154 2022-08-26 13:33:01.000000 dagster-azure-1.0.5/dagster_azure/adls2/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:44:05.256004 dagster-azure-1.0.5/dagster_azure/blob/
+-rw-r--r--   0 root         (0) root         (0)      150 2022-08-26 13:33:01.000000 dagster-azure-1.0.5/dagster_azure/blob/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8105 2022-08-26 13:33:01.000000 dagster-azure-1.0.5/dagster_azure/blob/compute_log_manager.py
+-rw-r--r--   0 root         (0) root         (0)     4765 2022-08-26 13:33:01.000000 dagster-azure-1.0.5/dagster_azure/blob/fake_blob_client.py
+-rw-r--r--   0 root         (0) root         (0)     1233 2022-08-26 13:33:01.000000 dagster-azure-1.0.5/dagster_azure/blob/utils.py
+-rw-r--r--   0 root         (0) root         (0)        8 2022-08-26 13:33:01.000000 dagster-azure-1.0.5/dagster_azure/py.typed
+-rw-r--r--   0 root         (0) root         (0)       22 2022-08-26 13:33:01.000000 dagster-azure-1.0.5/dagster_azure/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:44:05.248005 dagster-azure-1.0.5/dagster_azure.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      670 2022-08-26 13:44:05.000000 dagster-azure-1.0.5/dagster_azure.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      729 2022-08-26 13:44:05.000000 dagster-azure-1.0.5/dagster_azure.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-08-26 13:44:05.000000 dagster-azure-1.0.5/dagster_azure.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       62 2022-08-26 13:44:05.000000 dagster-azure-1.0.5/dagster_azure.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-08-26 13:44:05.000000 dagster-azure-1.0.5/dagster_azure.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      117 2022-08-26 13:44:05.000000 dagster-azure-1.0.5/dagster_azure.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2022-08-26 13:44:05.000000 dagster-azure-1.0.5/dagster_azure.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      160 2022-08-26 13:44:05.256004 dagster-azure-1.0.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1610 2022-08-26 13:33:01.000000 dagster-azure-1.0.5/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `dagster-azure-0.9.9rc1/LICENSE` & `dagster-azure-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-azure-0.9.9rc1/PKG-INFO` & `dagster-azure-1.0.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,19 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: dagster-azure
-Version: 0.9.9rc1
-Summary: Package for Azure-specific Dagster framework solid and resource components.
+Version: 1.0.5
+Summary: Package for Azure-specific Dagster framework op and resource components.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-azure
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
-Description: UNKNOWN
 Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
+License-File: LICENSE
+
+UNKNOWN
+
```

### Comparing `dagster-azure-0.9.9rc1/dagster_azure/adls2/fake_adls2_resource.py` & `dagster-azure-1.0.5/dagster_azure/adls2/fake_adls2_resource.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,34 +1,64 @@
 import io
 import random
-from collections import defaultdict
-from contextlib import contextmanager
+from typing import Dict
+from unittest import mock
 
 from dagster_azure.blob import FakeBlobServiceClient
 
-from dagster.seven import mock
+from dagster import resource
 
 from .resources import ADLS2Resource
 from .utils import ResourceNotFoundError
 
 
+@resource({"account_name": str})
+def fake_adls2_resource(context):
+    return FakeADLS2Resource(account_name=context.resource_config["account_name"])
+
+
 class FakeADLS2Resource(ADLS2Resource):
     """Stateful mock of an ADLS2Resource for testing.
 
     Wraps a ``mock.MagicMock``. Containers are implemented using an in-memory dict.
     """
 
     def __init__(
         self, account_name, credential="fake-creds"
     ):  # pylint: disable=unused-argument,super-init-not-called
         self._adls2_client = FakeADLS2ServiceClient(account_name)
         self._blob_client = FakeBlobServiceClient(account_name)
+        self._lease_client_constructor = FakeLeaseClient
+
+
+class FakeLeaseClient:
+    def __init__(self, client):
+        self.client = client
+        self.id = None
+
+        # client needs a ref to self to check if a given lease is valid
+        self.client._lease = self
+
+    def acquire(self, lease_duration=-1):  # pylint: disable=unused-argument
+        if self.id is None:
+            self.id = random.randint(0, 2**9)
+        else:
+            raise Exception("Lease already held")
+
+    def release(self):
+        self.id = None
 
+    def is_valid(self, lease):
+        if self.id is None:
+            # no lease is held so any operation is valid
+            return True
+        return lease == self.id
 
-class FakeADLS2ServiceClient(object):
+
+class FakeADLS2ServiceClient:
     """Stateful mock of an ADLS2 service client for testing.
 
     Wraps a ``mock.MagicMock``. Containers are implemented using an in-memory dict.
     """
 
     def __init__(self, account_name, credential="fake-creds"):
 
@@ -54,19 +84,19 @@
             file_system, FakeADLS2FilesystemClient(self.account_name, file_system)
         )
 
     def get_file_client(self, file_system, file_path):
         return self.get_file_system_client(file_system).get_file_client(file_path)
 
 
-class FakeADLS2FilesystemClient(object):
+class FakeADLS2FilesystemClient:
     """Stateful mock of an ADLS2 filesystem client for testing."""
 
     def __init__(self, account_name, file_system_name):
-        self._file_system = defaultdict(FakeADLS2FileClient)
+        self._file_system: Dict[str, FakeADLS2FileClient] = {}
         self._account_name = account_name
         self._file_system_name = file_system_name
 
     @property
     def account_name(self):
         return self._account_name
 
@@ -80,71 +110,78 @@
     def get_file_system_properties(self):
         return {"account_name": self.account_name, "file_system_name": self.file_system_name}
 
     def has_file(self, path):
         return bool(self._file_system.get(path))
 
     def get_file_client(self, file_path):
+        # pass fileclient a ref to self and its name so the file can delete itself
+        self._file_system.setdefault(file_path, FakeADLS2FileClient(self, file_path))
         return self._file_system[file_path]
 
     def create_file(self, file):
+        # pass fileclient a ref to self and the file's name so the file can delete itself by
+        # accessing the self._file_system dict
+        self._file_system.setdefault(file, FakeADLS2FileClient(fs_client=self, name=file))
         return self._file_system[file]
 
     def delete_file(self, file):
         for k in list(self._file_system.keys()):
             if k.startswith(file):
                 del self._file_system[k]
 
 
-class FakeADLS2FileClient(object):
+class FakeADLS2FileClient:
     """Stateful mock of an ADLS2 file client for testing."""
 
-    def __init__(self):
+    def __init__(self, name, fs_client):
+        self.name = name
         self.contents = None
-        self.lease = None
+        self._lease = None
+        self.fs_client = fs_client
+
+    @property
+    def lease(self):
+        return self._lease if self._lease is None else self._lease.id
 
     def get_file_properties(self):
         if self.contents is None:
             raise ResourceNotFoundError("File does not exist!")
-        return {"lease": self.lease}
+        lease_id = None if self._lease is None else self._lease.id
+        return {"lease": lease_id}
 
     def upload_data(self, contents, overwrite=False, lease=None):
-        if self.lease is not None:
-            if lease != self.lease:
+        if self._lease is not None:
+            if not self._lease.is_valid(lease):
                 raise Exception("Invalid lease!")
         if self.contents is not None or overwrite is True:
             if isinstance(contents, str):
                 self.contents = contents.encode("utf8")
             elif isinstance(contents, io.BytesIO):
                 self.contents = contents.read()
             elif isinstance(contents, io.StringIO):
                 self.contents = contents.read().encode("utf8")
             elif isinstance(contents, bytes):
                 self.contents = contents
             else:
                 self.contents = contents
 
-    @contextmanager
-    def acquire_lease(self, lease_duration=-1):  # pylint: disable=unused-argument
-        if self.lease is None:
-            self.lease = random.randint(0, 2 ** 9)
-            try:
-                yield self.lease
-            finally:
-                self.lease = None
-        else:
-            raise Exception("Lease already held")
-
     def download_file(self):
         if self.contents is None:
             raise ResourceNotFoundError("File does not exist!")
         return FakeADLS2FileDownloader(contents=self.contents)
 
+    def delete_file(self, lease=None):
+        if self._lease is not None:
+            if not self._lease.is_valid(lease):
+                raise Exception("Invalid lease!")
+        self.fs_client.delete_file(self.name)
+
 
-class FakeADLS2FileDownloader(object):
+class FakeADLS2FileDownloader:
     """Mock of an ADLS2 file downloader for testing."""
 
     def __init__(self, contents):
         self.contents = contents
 
     def readall(self):
         return self.contents
```

### Comparing `dagster-azure-0.9.9rc1/dagster_azure/adls2/file_manager.py` & `dagster-azure-1.0.5/dagster_azure/adls2/file_manager.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,47 +1,55 @@
 import io
 import uuid
 from contextlib import contextmanager
 
-from dagster import check, usable_as_dagster_type
-from dagster.core.storage.file_manager import (
+import dagster._check as check
+from dagster._core.storage.file_manager import (
     FileHandle,
     FileManager,
     TempfileManager,
     check_file_like_obj,
 )
 
 
-@usable_as_dagster_type
 class ADLS2FileHandle(FileHandle):
-    def __init__(self, account, file_system, key):
+    """A reference to a file on ADLS2."""
+
+    def __init__(self, account: str, file_system: str, key: str):
         self._account = check.str_param(account, "account")
         self._file_system = check.str_param(file_system, "file_system")
         self._key = check.str_param(key, "key")
 
     @property
     def account(self):
+        """str: The name of the ADLS2 account."""
         return self._account
 
     @property
     def file_system(self):
+        """str: The name of the ADLS2 file system."""
         return self._file_system
 
     @property
     def key(self):
+        """str: The ADLS2 key."""
         return self._key
 
     @property
     def path_desc(self):
+        """str: The file's ADLS2 URL."""
         return self.adls2_path
 
     @property
     def adls2_path(self):
+        """str: The file's ADLS2 URL."""
         return "adfss://{file_system}@{account}.dfs.core.windows.net/{key}".format(
-            file_system=self.file_system, account=self.account, key=self.key,
+            file_system=self.file_system,
+            account=self.account,
+            key=self.key,
         )
 
 
 class ADLS2FileManager(FileManager):
     def __init__(self, adls2_client, file_system, prefix):
         self._client = adls2_client
         self._file_system = check.str_param(file_system, "file_system")
@@ -55,15 +63,16 @@
 
     def _download_if_not_cached(self, file_handle):
         if not self._file_handle_cached(file_handle):
             # instigate download
             temp_file_obj = self._temp_file_manager.tempfile()
             temp_name = temp_file_obj.name
             file = self._client.get_file_client(
-                file_system=file_handle.file_system, file_path=file_handle.key,
+                file_system=file_handle.file_system,
+                file_path=file_handle.key,
             )
             download = file.download_file()
             with open(temp_name, "wb") as file_obj:
                 download.readinto(file_obj)
             self._local_handle_cache[file_handle.adls2_path] = temp_name
 
         return file_handle
@@ -72,15 +81,16 @@
     def read(self, file_handle, mode="rb"):
         check.inst_param(file_handle, "file_handle", ADLS2FileHandle)
         check.str_param(mode, "mode")
         check.param_invariant(mode in {"r", "rb"}, "mode")
 
         self._download_if_not_cached(file_handle)
 
-        with open(self._get_local_path(file_handle), mode) as file_obj:
+        encoding = None if "b" in mode else "utf-8"
+        with open(self._get_local_path(file_handle), mode, encoding=encoding) as file_obj:
             yield file_obj
 
     def _file_handle_cached(self, file_handle):
         return file_handle.adls2_path in self._local_handle_cache
 
     def _get_local_path(self, file_handle):
         return self._local_handle_cache[file_handle.adls2_path]
```

### Comparing `dagster-azure-0.9.9rc1/dagster_azure/adls2/resources.py` & `dagster-azure-1.0.5/dagster_azure/adls2/resources.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,12 @@
+from azure.storage.filedatalake import DataLakeLeaseClient
 from dagster_azure.blob.utils import create_blob_client
 
 from dagster import Field, Selector, StringSource, resource
-from dagster.utils.merger import merge_dicts
+from dagster._utils.merger import merge_dicts
 
 from .file_manager import ADLS2FileManager
 from .utils import create_adls2_client
 
 ADLS2_CLIENT_CONFIG = {
     "storage_account": Field(StringSource, description="The storage account name."),
     "credential": Field(
@@ -18,47 +19,37 @@
         description="The credentials with which to authenticate.",
     ),
 }
 
 
 @resource(ADLS2_CLIENT_CONFIG)
 def adls2_resource(context):
-    """Resource that gives solids access to Azure Data Lake Storage Gen2.
+    """Resource that gives ops access to Azure Data Lake Storage Gen2.
 
     The underlying client is a :py:class:`~azure.storage.filedatalake.DataLakeServiceClient`.
 
-    Attach this resource definition to a :py:class:`~dagster.ModeDefinition` in order to make it
-    available to your solids.
+    Attach this resource definition to a :py:class:`~dagster.JobDefinition` in order to make it
+    available to your ops.
 
     Example:
 
         .. code-block:: python
 
-            from dagster import ModeDefinition, execute_solid, solid
+            from dagster import job, op
             from dagster_azure.adls2 import adls2_resource
 
-            @solid(required_resource_keys={'adls2'})
-            def example_adls2_solid(context):
-                return list(context.resources.adls2.list_file_systems())
-
-            result = execute_solid(
-                example_adls2_solid,
-                run_config={
-                    'resources': {
-                        'adls2': {
-                            'config': {
-                                'storage_account': 'my_storage_account'
-                            }
-                        }
-                    }
-                },
-                mode_def=ModeDefinition(resource_defs={'adls2': adls2_resource}),
-            )
+            @op(required_resource_keys={'adls2'})
+            def example_adls2_op(context):
+                return list(context.resources.adls2.adls2_client.list_file_systems())
+
+            @job(resource_defs={"adls2": adls2_resource})
+            def my_job():
+                example_adls2_op()
 
-    Note that your solids must also declare that they require this resource with
+    Note that your ops must also declare that they require this resource with
     `required_resource_keys`, or it will not be initialized for the execution of their compute
     functions.
 
     You may pass credentials to this resource using either a SAS token or a key, using
     environment variables if desired:
 
     .. code-block:: YAML
@@ -84,42 +75,51 @@
         {
             "adls2_file_system": Field(StringSource, description="ADLS Gen2 file system name"),
             "adls2_prefix": Field(StringSource, is_required=False, default_value="dagster"),
         },
     )
 )
 def adls2_file_manager(context):
+    """FileManager that provides abstract access to ADLS2.
+
+    Implements the :py:class:`~dagster._core.storage.file_manager.FileManager` API.
+    """
     adls2_client = _adls2_resource_from_config(context.resource_config).adls2_client
 
     return ADLS2FileManager(
         adls2_client=adls2_client,
         file_system=context.resource_config["adls2_file_system"],
         prefix=context.resource_config["adls2_prefix"],
     )
 
 
-class ADLS2Resource(object):
+class ADLS2Resource:
     """Resource containing clients to access Azure Data Lake Storage Gen2.
 
     Contains a client for both the Data Lake and Blob APIs, to work around the limitations
     of each.
     """
 
     def __init__(self, storage_account, credential):
         self._adls2_client = create_adls2_client(storage_account, credential)
         self._blob_client = create_blob_client(storage_account, credential)
+        self._lease_client_constructor = DataLakeLeaseClient
 
     @property
     def adls2_client(self):
         return self._adls2_client
 
     @property
     def blob_client(self):
         return self._blob_client
 
+    @property
+    def lease_client_constructor(self):
+        return self._lease_client_constructor
+
 
 def _adls2_resource_from_config(config):
     """
     Args:
         config: A configuration containing the fields in ADLS2_CLIENT_CONFIG.
 
     Returns: An adls2 client.
```

### Comparing `dagster-azure-0.9.9rc1/dagster_azure/adls2/utils.py` & `dagster-azure-1.0.5/dagster_azure/adls2/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-azure-0.9.9rc1/dagster_azure/blob/compute_log_manager.py` & `dagster-azure-1.0.5/dagster_azure/blob/compute_log_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 import itertools
 import os
 from contextlib import contextmanager
 
-from dagster import Field, check, seven
-from dagster.core.storage.compute_log_manager import (
+import dagster._seven as seven
+from dagster import Field, StringSource
+from dagster import _check as check
+from dagster._core.storage.compute_log_manager import (
     MAX_BYTES_FILE_READ,
     ComputeIOType,
     ComputeLogFileData,
     ComputeLogManager,
 )
-from dagster.core.storage.local_compute_log_manager import IO_TYPE_EXTENSION, LocalComputeLogManager
-from dagster.serdes import ConfigurableClass, ConfigurableClassData
-from dagster.utils import ensure_dir, ensure_file
+from dagster._core.storage.local_compute_log_manager import (
+    IO_TYPE_EXTENSION,
+    LocalComputeLogManager,
+)
+from dagster._serdes import ConfigurableClass, ConfigurableClassData
+from dagster._utils import ensure_dir, ensure_file
 
 from .utils import create_blob_client, generate_blob_sas
 
 
 class AzureBlobComputeLogManager(ComputeLogManager, ConfigurableClass):
-    """Logs solid compute function stdout and stderr to Azure Blob Storage.
+    """Logs op compute function stdout and stderr to Azure Blob Storage.
 
     This is also compatible with Azure Data Lake Storage.
 
     Users should not instantiate this class directly. Instead, use a YAML block in ``dagster.yaml``
     such as the following:
 
     .. code-block:: YAML
@@ -38,15 +43,15 @@
 
     Args:
         storage_account (str): The storage account name to which to log.
         container (str): The container (or ADLS2 filesystem) to which to log.
         secret_key (str): Secret key for the storage account. SAS tokens are not
             supported because we need a secret key to generate a SAS token for a download URL.
         local_dir (Optional[str]): Path to the local directory in which to stage logs. Default:
-            ``dagster.seven.get_system_temp_directory()``.
+            ``dagster._seven.get_system_temp_directory()``.
         prefix (Optional[str]): Prefix for the log file keys.
         inst_data (Optional[ConfigurableClassData]): Serializable representation of the compute
             log manager when newed up from config.
     """
 
     def __init__(
         self,
@@ -84,19 +89,19 @@
     @property
     def inst_data(self):
         return self._inst_data
 
     @classmethod
     def config_type(cls):
         return {
-            "storage_account": str,
-            "container": str,
-            "secret_key": str,
-            "local_dir": Field(str, is_required=False),
-            "prefix": Field(str, is_required=False, default_value="dagster"),
+            "storage_account": StringSource,
+            "container": StringSource,
+            "secret_key": StringSource,
+            "local_dir": Field(StringSource, is_required=False),
+            "prefix": Field(StringSource, is_required=False, default_value="dagster"),
         }
 
     @staticmethod
     def from_config_value(inst_data, config_value):
         return AzureBlobComputeLogManager(inst_data=inst_data, **config_value)
 
     def get_local_path(self, run_id, key, io_type):
@@ -136,14 +141,17 @@
             self._download_to_local(run_id, key, io_type)
         data = self.local_manager.read_logs_file(run_id, key, io_type, cursor, max_bytes)
         return self._from_local_file_data(run_id, key, io_type, data)
 
     def on_subscribe(self, subscription):
         self.local_manager.on_subscribe(subscription)
 
+    def on_unsubscribe(self, subscription):
+        self.local_manager.on_unsubscribe(subscription)
+
     def _should_download(self, run_id, key, io_type):
         local_path = self.get_local_path(run_id, key, io_type)
         if os.path.exists(local_path):
             return False
         blob_objects = self._container_client.list_blobs(self._blob_key(run_id, key, io_type))
         # Limit the generator to avoid paging since we only need one element
         # to return True
@@ -193,7 +201,10 @@
             self._blob_prefix,
             "storage",
             run_id,
             "compute_logs",
             "{}.{}".format(key, extension),
         ]
         return "/".join(paths)  # blob path delimiter
+
+    def dispose(self):
+        self.local_manager.dispose()
```

### Comparing `dagster-azure-0.9.9rc1/dagster_azure/blob/fake_blob_client.py` & `dagster-azure-1.0.5/dagster_azure/blob/fake_blob_client.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import io
 import random
 from collections import defaultdict
 from contextlib import contextmanager
-
-from dagster.seven import mock
+from unittest import mock
 
 from .utils import ResourceNotFoundError
 
 
-class FakeBlobServiceClient(object):
+class FakeBlobServiceClient:
     """Stateful mock of an Blob service client for testing.
 
     Wraps a ``mock.MagicMock``. Containers are implemented using an in-memory dict.
     """
 
     def __init__(self, account_name, credential="fake-creds"):
 
@@ -38,15 +37,15 @@
             container, FakeBlobContainerClient(self.account_name, container)
         )
 
     def get_blob_client(self, container, blob):
         return self.get_container_client(container).get_blob_client(blob)
 
 
-class FakeBlobContainerClient(object):
+class FakeBlobContainerClient:
     """Stateful mock of an Blob container client for testing."""
 
     def __init__(self, account_name, container_name):
         self._container = defaultdict(FakeBlobClient)
         self._account_name = account_name
         self._container_name = container_name
 
@@ -86,15 +85,15 @@
     def delete_blob(self, blob):
         # Use list to avoid mutating dict as we iterate
         for k in list(self._container.keys()):
             if k.startswith(blob):
                 del self._container[k]
 
 
-class FakeBlobClient(object):
+class FakeBlobClient:
     """Stateful mock of an Blob blob client for testing."""
 
     def __init__(self):
         self.contents = None
         self.lease = None
 
     def start_copy_from_url(self, url):
@@ -127,29 +126,29 @@
     @property
     def url(self):
         return ":memory:"
 
     @contextmanager
     def acquire_lease(self, lease_duration=-1):  # pylint: disable=unused-argument
         if self.lease is None:
-            self.lease = random.randint(0, 2 ** 9)
+            self.lease = random.randint(0, 2**9)
             try:
                 yield self.lease
             finally:
                 self.lease = None
         else:
             raise Exception("Lease already held")
 
     def download_blob(self):
         if self.contents is None:
             raise ResourceNotFoundError("File does not exist!")
         return FakeBlobDownloader(contents=self.contents)
 
 
-class FakeBlobDownloader(object):
+class FakeBlobDownloader:
     """Mock of a Blob file downloader for testing."""
 
     def __init__(self, contents):
         self.contents = contents
 
     def readall(self):
         return self.contents
```

### Comparing `dagster-azure-0.9.9rc1/dagster_azure/blob/utils.py` & `dagster-azure-1.0.5/dagster_azure/blob/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 import warnings
 
 try:
     # Centralise Azure imports here so we only need to warn in one place
     from azure.core.exceptions import ResourceNotFoundError
-    from azure.storage.blob import (
-        generate_blob_sas,
-        BlobServiceClient,
-    )
+    from azure.storage.blob import BlobServiceClient, generate_blob_sas
 except ImportError:
     msg = (
         "Could not import required Azure objects. This probably means you have an old version "
         "of azure-storage-blob installed. dagster-azure requires azure-storage-blob~=12.0.0; "
         "this conflicts with dagster-snowflake which requires azure-storage-blob<12.0.0 and is "
         "incompatible. Please uninstall dagster-snowflake and reinstall dagster-azure to fix "
         "this error."
```

### Comparing `dagster-azure-0.9.9rc1/dagster_azure.egg-info/PKG-INFO` & `dagster-azure-1.0.5/dagster_azure.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,19 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: dagster-azure
-Version: 0.9.9rc1
-Summary: Package for Azure-specific Dagster framework solid and resource components.
+Version: 1.0.5
+Summary: Package for Azure-specific Dagster framework op and resource components.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-azure
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
-Description: UNKNOWN
 Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
+License-File: LICENSE
+
+UNKNOWN
+
```

### Comparing `dagster-azure-0.9.9rc1/setup.py` & `dagster-azure-1.0.5/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,37 +1,44 @@
+from typing import Dict
+
 from setuptools import find_packages, setup
 
 
-def get_version():
-    version = {}
-    with open("dagster_azure/version.py") as fp:
+def get_version() -> str:
+    version: Dict[str, str] = {}
+    with open("dagster_azure/version.py", encoding="utf8") as fp:
         exec(fp.read(), version)  # pylint: disable=W0122
 
     return version["__version__"]
 
 
 if __name__ == "__main__":
+    ver = get_version()
+    # dont pin dev installs to avoid pip dep resolver issues
+    pin = "" if ver == "0+dev" else f"=={ver}"
     setup(
         name="dagster-azure",
-        version=get_version(),
+        version=ver,
         author="Elementl",
         author_email="hello@elementl.com",
         license="Apache-2.0",
-        description="Package for Azure-specific Dagster framework solid and resource components.",
+        description="Package for Azure-specific Dagster framework op and resource components.",
         url="https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-azure",
         classifiers=[
-            "Programming Language :: Python :: 2.7",
-            "Programming Language :: Python :: 3.6",
             "Programming Language :: Python :: 3.7",
+            "Programming Language :: Python :: 3.8",
+            "Programming Language :: Python :: 3.9",
+            "Programming Language :: Python :: 3.10",
             "License :: OSI Approved :: Apache Software License",
             "Operating System :: OS Independent",
         ],
-        packages=find_packages(exclude=["test"]),
+        packages=find_packages(exclude=["dagster_azure_tests*"]),
         include_package_data=True,
         install_requires=[
-            "azure-storage-blob~=12.3.0",
-            "azure-storage-file-datalake~=12.0.1",
-            "dagster",
+            "azure-core<2.0.0,>=1.7.0",
+            "azure-storage-blob<13.0.0,>=12.5.0",
+            "azure-storage-file-datalake<13.0.0,>=12.5",
+            "dagster==1.0.5",
         ],
         entry_points={"console_scripts": ["dagster-azure = dagster_azure.cli.cli:main"]},
         zip_safe=False,
     )
```

