# Comparing `tmp/backend.ai-storage-proxy-23.3.2.tar.gz` & `tmp/backend.ai-storage-proxy-23.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backend.ai-storage-proxy-23.3.2.tar", last modified: Fri May  5 07:08:21 2023, max compression
+gzip compressed data, was "backend.ai-storage-proxy-23.3.3.tar", last modified: Thu May 25 17:30:44 2023, max compression
```

## Comparing `backend.ai-storage-proxy-23.3.2.tar` & `backend.ai-storage-proxy-23.3.3.tar`

### file list

```diff
@@ -1,53 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:21.426488 backend.ai-storage-proxy-23.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-05 07:08:20.000000 backend.ai-storage-proxy-23.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6684 2023-05-05 07:08:21.426488 backend.ai-storage-proxy-23.3.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:21.418488 backend.ai-storage-proxy-23.3.2/ai/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:21.418488 backend.ai-storage-proxy-23.3.2/ai/backend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:21.418488 backend.ai-storage-proxy-23.3.2/ai/backend/storage/
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-05 07:08:20.000000 backend.ai-storage-proxy-23.3.2/ai/backend/storage/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-05 07:08:20.000000 backend.ai-storage-proxy-23.3.2/ai/backend/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6431 2023-05-05 07:08:20.000000 backend.ai-storage-proxy-23.3.2/ai/backend/storage/abc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:21.422488 backend.ai-storage-proxy-23.3.2/ai/backend/storage/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:20.000000 backend.ai-storage-proxy-23.3.2/ai/backend/storage/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13343 2023-05-05 07:08:20.000000 backend.ai-storage-proxy-23.3.2/ai/backend/storage/api/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    23528 2023-05-05 07:08:20.000000 backend.ai-storage-proxy-23.3.2/ai/backend/storage/api/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:21.422488 backend.ai-storage-proxy-23.3.2/ai/backend/storage/cephfs/
--rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-05-05 07:08:20.000000 backend.ai-storage-proxy-23.3.2/ai/backend/storage/cephfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4629 2023-05-05 07:08:20.000000 backend.ai-storage-proxy-23.3.2/ai/backend/storage/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-05-05 07:08:20.000000 backend.ai-storage-proxy-23.3.2/ai/backend/storage/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-05-05 07:08:20.000000 backend.ai-storage-proxy-23.3.2/ai/backend/storage/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:21.422488 backend.ai-storage-proxy-23.3.2/ai/backend/storage/gpfs/
--rw-r--r--   0 runner    (1001) docker     (123)     6490 2023-05-05 07:08:20.000000 backend.ai-storage-proxy-23.3.2/ai/backend/storage/gpfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-05 07:08:20.000000 backend.ai-storage-proxy-23.3.2/ai/backend/storage/gpfs/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12362 2023-05-05 07:08:20.000000 backend.ai-storage-proxy-23.3.2/ai/backend/storage/gpfs/gpfs_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-05-05 07:08:20.000000 backend.ai-storage-proxy-23.3.2/ai/backend/storage/gpfs/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:21.422488 backend.ai-storage-proxy-23.3.2/ai/backend/storage/netapp/
--rw-r--r--   0 runner    (1001) docker     (123)    14060 2023-05-05 07:08:20.000000 backend.ai-storage-proxy-23.3.2/ai/backend/storage/netapp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8329 2023-05-05 07:08:20.000000 backend.ai-storage-proxy-23.3.2/ai/backend/storage/netapp/netappclient.py
--rw-r--r--   0 runner    (1001) docker     (123)     5332 2023-05-05 07:08:20.000000 backend.ai-storage-proxy-23.3.2/ai/backend/storage/netapp/quotamanager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:21.422488 backend.ai-storage-proxy-23.3.2/ai/backend/storage/purestorage/
--rw-r--r--   0 runner    (1001) docker     (123)     9318 2023-05-05 07:08:20.000000 backend.ai-storage-proxy-23.3.2/ai/backend/storage/purestorage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-05-05 07:08:20.000000 backend.ai-storage-proxy-23.3.2/ai/backend/storage/purestorage/purity.py
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-05 07:08:20.000000 backend.ai-storage-proxy-23.3.2/ai/backend/storage/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     8726 2023-05-05 07:08:20.000000 backend.ai-storage-proxy-23.3.2/ai/backend/storage/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-05-05 07:08:20.000000 backend.ai-storage-proxy-23.3.2/ai/backend/storage/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-05-05 07:08:20.000000 backend.ai-storage-proxy-23.3.2/ai/backend/storage/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:21.422488 backend.ai-storage-proxy-23.3.2/ai/backend/storage/vfs/
--rw-r--r--   0 runner    (1001) docker     (123)    16485 2023-05-05 07:08:20.000000 backend.ai-storage-proxy-23.3.2/ai/backend/storage/vfs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:21.422488 backend.ai-storage-proxy-23.3.2/ai/backend/storage/weka/
--rw-r--r--   0 runner    (1001) docker     (123)     6243 2023-05-05 07:08:20.000000 backend.ai-storage-proxy-23.3.2/ai/backend/storage/weka/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-05 07:08:20.000000 backend.ai-storage-proxy-23.3.2/ai/backend/storage/weka/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12747 2023-05-05 07:08:20.000000 backend.ai-storage-proxy-23.3.2/ai/backend/storage/weka/weka_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:21.422488 backend.ai-storage-proxy-23.3.2/ai/backend/storage/xfs/
--rw-r--r--   0 runner    (1001) docker     (123)    10645 2023-05-05 07:08:20.000000 backend.ai-storage-proxy-23.3.2/ai/backend/storage/xfs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:21.422488 backend.ai-storage-proxy-23.3.2/backend.ai_storage_proxy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6684 2023-05-05 07:08:21.000000 backend.ai-storage-proxy-23.3.2/backend.ai_storage_proxy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-05-05 07:08:21.000000 backend.ai-storage-proxy-23.3.2/backend.ai_storage_proxy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 07:08:21.000000 backend.ai-storage-proxy-23.3.2/backend.ai_storage_proxy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 07:08:21.000000 backend.ai-storage-proxy-23.3.2/backend.ai_storage_proxy.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 07:08:21.000000 backend.ai-storage-proxy-23.3.2/backend.ai_storage_proxy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-05 07:08:21.000000 backend.ai-storage-proxy-23.3.2/backend.ai_storage_proxy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-05 07:08:21.000000 backend.ai-storage-proxy-23.3.2/backend.ai_storage_proxy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-05 07:08:20.000000 backend.ai-storage-proxy-23.3.2/backend_shim.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 07:08:21.426488 backend.ai-storage-proxy-23.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     8006 2023-05-05 07:08:20.000000 backend.ai-storage-proxy-23.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:44.589146 backend.ai-storage-proxy-23.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-25 17:30:44.000000 backend.ai-storage-proxy-23.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6735 2023-05-25 17:30:44.589146 backend.ai-storage-proxy-23.3.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:44.581146 backend.ai-storage-proxy-23.3.3/ai/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:44.581146 backend.ai-storage-proxy-23.3.3/ai/backend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:44.581146 backend.ai-storage-proxy-23.3.3/ai/backend/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-25 17:30:44.000000 backend.ai-storage-proxy-23.3.3/ai/backend/storage/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-25 17:30:44.000000 backend.ai-storage-proxy-23.3.3/ai/backend/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6431 2023-05-25 17:30:44.000000 backend.ai-storage-proxy-23.3.3/ai/backend/storage/abc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:44.581146 backend.ai-storage-proxy-23.3.3/ai/backend/storage/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:44.000000 backend.ai-storage-proxy-23.3.3/ai/backend/storage/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13372 2023-05-25 17:30:44.000000 backend.ai-storage-proxy-23.3.3/ai/backend/storage/api/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24079 2023-05-25 17:30:44.000000 backend.ai-storage-proxy-23.3.3/ai/backend/storage/api/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:44.585146 backend.ai-storage-proxy-23.3.3/ai/backend/storage/cephfs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-05-25 17:30:44.000000 backend.ai-storage-proxy-23.3.3/ai/backend/storage/cephfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4629 2023-05-25 17:30:44.000000 backend.ai-storage-proxy-23.3.3/ai/backend/storage/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-05-25 17:30:44.000000 backend.ai-storage-proxy-23.3.3/ai/backend/storage/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:44.585146 backend.ai-storage-proxy-23.3.3/ai/backend/storage/dellemc/
+-rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-05-25 17:30:44.000000 backend.ai-storage-proxy-23.3.3/ai/backend/storage/dellemc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6757 2023-05-25 17:30:44.000000 backend.ai-storage-proxy-23.3.3/ai/backend/storage/dellemc/dellemc_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-05-25 17:30:44.000000 backend.ai-storage-proxy-23.3.3/ai/backend/storage/dellemc/dellemc_quota_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-25 17:30:44.000000 backend.ai-storage-proxy-23.3.3/ai/backend/storage/dellemc/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-05-25 17:30:44.000000 backend.ai-storage-proxy-23.3.3/ai/backend/storage/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:44.585146 backend.ai-storage-proxy-23.3.3/ai/backend/storage/gpfs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6490 2023-05-25 17:30:44.000000 backend.ai-storage-proxy-23.3.3/ai/backend/storage/gpfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-25 17:30:44.000000 backend.ai-storage-proxy-23.3.3/ai/backend/storage/gpfs/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12362 2023-05-25 17:30:44.000000 backend.ai-storage-proxy-23.3.3/ai/backend/storage/gpfs/gpfs_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-05-25 17:30:44.000000 backend.ai-storage-proxy-23.3.3/ai/backend/storage/gpfs/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:44.585146 backend.ai-storage-proxy-23.3.3/ai/backend/storage/netapp/
+-rw-r--r--   0 runner    (1001) docker     (123)    14060 2023-05-25 17:30:44.000000 backend.ai-storage-proxy-23.3.3/ai/backend/storage/netapp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8329 2023-05-25 17:30:44.000000 backend.ai-storage-proxy-23.3.3/ai/backend/storage/netapp/netappclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5332 2023-05-25 17:30:44.000000 backend.ai-storage-proxy-23.3.3/ai/backend/storage/netapp/quotamanager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:44.585146 backend.ai-storage-proxy-23.3.3/ai/backend/storage/purestorage/
+-rw-r--r--   0 runner    (1001) docker     (123)     9318 2023-05-25 17:30:44.000000 backend.ai-storage-proxy-23.3.3/ai/backend/storage/purestorage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-05-25 17:30:44.000000 backend.ai-storage-proxy-23.3.3/ai/backend/storage/purestorage/purity.py
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-25 17:30:44.000000 backend.ai-storage-proxy-23.3.3/ai/backend/storage/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     8726 2023-05-25 17:30:44.000000 backend.ai-storage-proxy-23.3.3/ai/backend/storage/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-05-25 17:30:44.000000 backend.ai-storage-proxy-23.3.3/ai/backend/storage/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-05-25 17:30:44.000000 backend.ai-storage-proxy-23.3.3/ai/backend/storage/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:44.585146 backend.ai-storage-proxy-23.3.3/ai/backend/storage/vfs/
+-rw-r--r--   0 runner    (1001) docker     (123)    16485 2023-05-25 17:30:44.000000 backend.ai-storage-proxy-23.3.3/ai/backend/storage/vfs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:44.585146 backend.ai-storage-proxy-23.3.3/ai/backend/storage/weka/
+-rw-r--r--   0 runner    (1001) docker     (123)     6243 2023-05-25 17:30:44.000000 backend.ai-storage-proxy-23.3.3/ai/backend/storage/weka/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-25 17:30:44.000000 backend.ai-storage-proxy-23.3.3/ai/backend/storage/weka/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12747 2023-05-25 17:30:44.000000 backend.ai-storage-proxy-23.3.3/ai/backend/storage/weka/weka_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:44.585146 backend.ai-storage-proxy-23.3.3/ai/backend/storage/xfs/
+-rw-r--r--   0 runner    (1001) docker     (123)    10645 2023-05-25 17:30:44.000000 backend.ai-storage-proxy-23.3.3/ai/backend/storage/xfs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:44.589146 backend.ai-storage-proxy-23.3.3/backend.ai_storage_proxy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6735 2023-05-25 17:30:44.000000 backend.ai-storage-proxy-23.3.3/backend.ai_storage_proxy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-05-25 17:30:44.000000 backend.ai-storage-proxy-23.3.3/backend.ai_storage_proxy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 17:30:44.000000 backend.ai-storage-proxy-23.3.3/backend.ai_storage_proxy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 17:30:44.000000 backend.ai-storage-proxy-23.3.3/backend.ai_storage_proxy.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 17:30:44.000000 backend.ai-storage-proxy-23.3.3/backend.ai_storage_proxy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-25 17:30:44.000000 backend.ai-storage-proxy-23.3.3/backend.ai_storage_proxy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-25 17:30:44.000000 backend.ai-storage-proxy-23.3.3/backend.ai_storage_proxy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-25 17:30:44.000000 backend.ai-storage-proxy-23.3.3/backend_shim.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 17:30:44.589146 backend.ai-storage-proxy-23.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     8094 2023-05-25 17:30:44.000000 backend.ai-storage-proxy-23.3.3/setup.py
```

### Comparing `backend.ai-storage-proxy-23.3.2/PKG-INFO` & `backend.ai-storage-proxy-23.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-storage-proxy
-Version: 23.3.2
+Version: 23.3.3
 Summary: Backend.AI Storage Proxy
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: LGPLv3
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
@@ -12,14 +12,15 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Environment :: No Input/Output (Daemon)
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Classifier: Development Status :: 5 - Production/Stable
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Requires-Python: >=3.11,<3.12
 Description-Content-Type: text/markdown
 
 # Backend.AI Storage Proxy
 
 Backend.AI Storage Proxy is an RPC daemon to manage vfolders used in Backend.AI agent, with quota and
```

### Comparing `backend.ai-storage-proxy-23.3.2/ai/backend/storage/abc.py` & `backend.ai-storage-proxy-23.3.3/ai/backend/storage/abc.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.2/ai/backend/storage/api/client.py` & `backend.ai-storage-proxy-23.3.3/ai/backend/storage/api/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -255,15 +255,15 @@
         ),
         read_from=CheckParamSource.QUERY,
     ) as params:
         token_data = params["token"]
         async with ctx.get_volume(token_data["volume"]) as volume:
             headers = await prepare_tus_session_headers(request, token_data, volume)
             vfpath = volume.mangle_vfpath(token_data["vfid"])
-            upload_temp_path = vfpath / ".upload" / token_data["session"]
+            upload_temp_path: Path = vfpath / ".upload" / token_data["session"]
 
             async with AsyncFileWriter(
                 target_filename=upload_temp_path,
                 access_mode="ab",
                 max_chunks=DEFAULT_INFLIGHT_CHUNKS,
             ) as writer:
                 while not request.content.at_eof():
@@ -271,17 +271,17 @@
                     await writer.write(chunk)
 
             current_size = Path(upload_temp_path).stat().st_size
             if current_size >= int(token_data["size"]):
                 parent_dir = vfpath
                 if (dst_dir := params["dst_dir"]) is not None:
                     parent_dir = vfpath / dst_dir
-                if not parent_dir.exists():
-                    parent_dir.mkdir(parents=True, exist_ok=True)
-                target_path = parent_dir / token_data["relpath"]
+                target_path: Path = parent_dir / token_data["relpath"]
+                if not target_path.parent.exists():
+                    target_path.parent.mkdir(parents=True, exist_ok=True)
                 upload_temp_path.rename(target_path)
                 try:
                     loop = asyncio.get_running_loop()
                     await loop.run_in_executor(
                         None,
                         lambda: upload_temp_path.parent.rmdir(),
                     )
@@ -361,8 +361,9 @@
     cors = aiohttp_cors.setup(app, defaults=cors_options)
     r = cors.add(app.router.add_resource("/download"))
     r.add_route("GET", download)
     r = app.router.add_resource("/upload")  # tus handlers handle CORS by themselves
     r.add_route("OPTIONS", tus_options)
     r.add_route("HEAD", tus_check_session)
     r.add_route("PATCH", tus_upload_part)
+
     return app
```

### Comparing `backend.ai-storage-proxy-23.3.2/ai/backend/storage/api/manager.py` & `backend.ai-storage-proxy-23.3.3/ai/backend/storage/api/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,23 +29,32 @@
 
 
 @web.middleware
 async def token_auth_middleware(
     request: web.Request,
     handler: Callable[[web.Request], Awaitable[web.StreamResponse]],
 ) -> web.StreamResponse:
-    token = request.headers.get("X-BackendAI-Storage-Auth-Token", None)
-    if not token:
-        raise web.HTTPForbidden()
-    ctx: Context = request.app["ctx"]
-    if token != ctx.local_config["api"]["manager"]["secret"]:
-        raise web.HTTPForbidden()
+    skip_token_check = getattr(handler, "skip_token_check", False)
+    if not skip_token_check:
+        token = request.headers.get("X-BackendAI-Storage-Auth-Token", None)
+        if not token:
+            raise web.HTTPForbidden()
+        ctx: Context = request.app["ctx"]
+        if token != ctx.local_config["api"]["manager"]["secret"]:
+            raise web.HTTPForbidden()
     return await handler(request)
 
 
+def skip_token_check(
+    handler: Callable[[web.Request], Awaitable[web.StreamResponse]]
+) -> Callable[[web.Request], Awaitable[web.StreamResponse]]:
+    setattr(handler, "skip_token_check", True)
+    return handler
+
+
 async def get_status(request: web.Request) -> web.Response:
     async with check_params(request, None) as params:
         await log_manager_api_entry(log, "get_status", params)
         return web.json_response(
             {
                 "status": "ok",
             },
@@ -370,14 +379,23 @@
         except ExecutionError:
             return web.Response(
                 status=500,
                 reason="Storage server is busy. Please try again",
             )
 
 
+@skip_token_check
+async def status(request: web.Request) -> web.Response:
+    return web.json_response(
+        {
+            "status": "ok",
+        },
+    )
+
+
 async def get_vfolder_used_bytes(request: web.Request) -> web.Response:
     async with check_params(
         request,
         t.Dict(
             {
                 t.Key("volume"): t.String(),
                 t.Key("vfid"): tx.UUID(),
@@ -675,8 +693,9 @@
     app.router.add_route("POST", "/folder/file/list", list_files)
     app.router.add_route("POST", "/folder/file/rename", rename_file)
     app.router.add_route("POST", "/folder/file/move", move_file)
     app.router.add_route("POST", "/folder/file/fetch", fetch_file)
     app.router.add_route("POST", "/folder/file/download", create_download_session)
     app.router.add_route("POST", "/folder/file/upload", create_upload_session)
     app.router.add_route("POST", "/folder/file/delete", delete_files)
+    app.router.add_route("GET", "/status", status)
     return app
```

### Comparing `backend.ai-storage-proxy-23.3.2/ai/backend/storage/cephfs/__init__.py` & `backend.ai-storage-proxy-23.3.3/ai/backend/storage/cephfs/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.2/ai/backend/storage/config.py` & `backend.ai-storage-proxy-23.3.3/ai/backend/storage/config.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.2/ai/backend/storage/context.py` & `backend.ai-storage-proxy-23.3.3/ai/backend/storage/context.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,27 +5,29 @@
 from typing import Any, AsyncIterator, Mapping, Type
 
 from ai.backend.common.etcd import AsyncEtcd
 from ai.backend.storage.weka import WekaVolume
 
 from .abc import AbstractVolume
 from .cephfs import CephFSVolume
+from .dellemc import DellEMCVolume
 from .exception import InvalidVolumeError
 from .gpfs import GPFSVolume
 from .netapp import NetAppVolume
 from .purestorage import FlashBladeVolume
 from .types import VolumeInfo
 from .vfs import BaseVolume
 from .xfs import XfsVolume
 
 BACKENDS: Mapping[str, Type[AbstractVolume]] = {
     "purestorage": FlashBladeVolume,
     "vfs": BaseVolume,
     "xfs": XfsVolume,
     "netapp": NetAppVolume,
+    "dell": DellEMCVolume,
     "weka": WekaVolume,
     "spectrumscale": GPFSVolume,
     "cephfs": CephFSVolume,
 }
 
 
 class Context:
```

### Comparing `backend.ai-storage-proxy-23.3.2/ai/backend/storage/exception.py` & `backend.ai-storage-proxy-23.3.3/ai/backend/storage/exception.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.2/ai/backend/storage/gpfs/__init__.py` & `backend.ai-storage-proxy-23.3.3/ai/backend/storage/gpfs/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.2/ai/backend/storage/gpfs/exceptions.py` & `backend.ai-storage-proxy-23.3.3/ai/backend/storage/gpfs/exceptions.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.2/ai/backend/storage/gpfs/gpfs_client.py` & `backend.ai-storage-proxy-23.3.3/ai/backend/storage/gpfs/gpfs_client.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.2/ai/backend/storage/gpfs/types.py` & `backend.ai-storage-proxy-23.3.3/ai/backend/storage/gpfs/types.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.2/ai/backend/storage/netapp/__init__.py` & `backend.ai-storage-proxy-23.3.3/ai/backend/storage/netapp/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.2/ai/backend/storage/netapp/netappclient.py` & `backend.ai-storage-proxy-23.3.3/ai/backend/storage/netapp/netappclient.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.2/ai/backend/storage/netapp/quotamanager.py` & `backend.ai-storage-proxy-23.3.3/ai/backend/storage/netapp/quotamanager.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.2/ai/backend/storage/purestorage/__init__.py` & `backend.ai-storage-proxy-23.3.3/ai/backend/storage/purestorage/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.2/ai/backend/storage/purestorage/purity.py` & `backend.ai-storage-proxy-23.3.3/ai/backend/storage/purestorage/purity.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.2/ai/backend/storage/server.py` & `backend.ai-storage-proxy-23.3.3/ai/backend/storage/server.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.2/ai/backend/storage/types.py` & `backend.ai-storage-proxy-23.3.3/ai/backend/storage/types.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.2/ai/backend/storage/utils.py` & `backend.ai-storage-proxy-23.3.3/ai/backend/storage/utils.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.2/ai/backend/storage/vfs/__init__.py` & `backend.ai-storage-proxy-23.3.3/ai/backend/storage/vfs/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.2/ai/backend/storage/weka/__init__.py` & `backend.ai-storage-proxy-23.3.3/ai/backend/storage/weka/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.2/ai/backend/storage/weka/exceptions.py` & `backend.ai-storage-proxy-23.3.3/ai/backend/storage/weka/exceptions.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.2/ai/backend/storage/weka/weka_client.py` & `backend.ai-storage-proxy-23.3.3/ai/backend/storage/weka/weka_client.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.2/ai/backend/storage/xfs/__init__.py` & `backend.ai-storage-proxy-23.3.3/ai/backend/storage/xfs/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.2/backend.ai_storage_proxy.egg-info/PKG-INFO` & `backend.ai-storage-proxy-23.3.3/backend.ai_storage_proxy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-storage-proxy
-Version: 23.3.2
+Version: 23.3.3
 Summary: Backend.AI Storage Proxy
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: LGPLv3
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
@@ -12,14 +12,15 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Environment :: No Input/Output (Daemon)
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Classifier: Development Status :: 5 - Production/Stable
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Requires-Python: >=3.11,<3.12
 Description-Content-Type: text/markdown
 
 # Backend.AI Storage Proxy
 
 Backend.AI Storage Proxy is an RPC daemon to manage vfolders used in Backend.AI agent, with quota and
```

### Comparing `backend.ai-storage-proxy-23.3.2/backend.ai_storage_proxy.egg-info/SOURCES.txt` & `backend.ai-storage-proxy-23.3.3/backend.ai_storage_proxy.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -11,14 +11,18 @@
 ai/backend/storage/server.py
 ai/backend/storage/types.py
 ai/backend/storage/utils.py
 ai/backend/storage/api/__init__.py
 ai/backend/storage/api/client.py
 ai/backend/storage/api/manager.py
 ai/backend/storage/cephfs/__init__.py
+ai/backend/storage/dellemc/__init__.py
+ai/backend/storage/dellemc/dellemc_client.py
+ai/backend/storage/dellemc/dellemc_quota_manager.py
+ai/backend/storage/dellemc/exceptions.py
 ai/backend/storage/gpfs/__init__.py
 ai/backend/storage/gpfs/exceptions.py
 ai/backend/storage/gpfs/gpfs_client.py
 ai/backend/storage/gpfs/types.py
 ai/backend/storage/netapp/__init__.py
 ai/backend/storage/netapp/netappclient.py
 ai/backend/storage/netapp/quotamanager.py
```

### Comparing `backend.ai-storage-proxy-23.3.2/backend_shim.py` & `backend.ai-storage-proxy-23.3.3/backend_shim.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,15 +10,21 @@
 build_wheel = True
 build_sdist = True
 wheel_config_settings = {
 }
 sdist_config_settings = {
 }
 
-os.makedirs(dist_dir, exist_ok=True)
+# Python 2.7 doesn't have the exist_ok arg on os.makedirs().
+try:
+    os.makedirs(dist_dir)
+except OSError as e:
+    if e.errno != errno.EEXIST:
+        raise
+
 wheel_path = backend.build_wheel(dist_dir, wheel_config_settings) if build_wheel else None
 sdist_path = backend.build_sdist(dist_dir, sdist_config_settings) if build_sdist else None
 
 if wheel_path:
     print("wheel: {wheel_path}".format(wheel_path=wheel_path))
 if sdist_path:
     print("sdist: {sdist_path}".format(sdist_path=sdist_path))
```

### Comparing `backend.ai-storage-proxy-23.3.2/setup.py` & `backend.ai-storage-proxy-23.3.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,26 +12,27 @@
         'Operating System :: POSIX :: Linux',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Environment :: No Input/Output (Daemon)',
         'Topic :: Scientific/Engineering',
         'Topic :: Software Development',
         'Development Status :: 5 - Production/Stable',
+        'Programming Language :: Python :: 3.11',
         'License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)',
     ],
     'description': 'Backend.AI Storage Proxy',
     'install_requires': (
         'PyJWT~=2.0',
         'aiofiles~=0.8.0',
         'aiohttp_cors~=0.7',
         'aiohttp~=3.8.1',
         'aiomonitor-ng~=0.7.2',
         'aiotools~=1.6.1',
         'attrs>=20.3',
-        """backend.ai-common==23.03.2
+        """backend.ai-common==23.03.3
 """,
         'click>=7.1.2',
         'dataclasses-json~=0.5.7',
         'janus~=1.0.0',
         'setproctitle~=1.2.2',
         'tenacity>=8.0',
         'trafaret~=2.1',
@@ -230,24 +231,25 @@
             'py.typed',
         ),
     },
     'packages': (
         'ai.backend.storage',
         'ai.backend.storage.api',
         'ai.backend.storage.cephfs',
+        'ai.backend.storage.dellemc',
         'ai.backend.storage.gpfs',
         'ai.backend.storage.netapp',
         'ai.backend.storage.purestorage',
         'ai.backend.storage.vfs',
         'ai.backend.storage.weka',
         'ai.backend.storage.xfs',
     ),
     'project_urls': {
         'Documentation': 'https://docs.backend.ai/',
         'Source': 'https://github.com/lablup/backend.ai',
     },
     'python_requires': '>=3.11,<3.12',
     'url': 'https://github.com/lablup/backend.ai',
-    'version': """23.03.2
+    'version': """23.03.3
 """,
     'zip_safe': False,
 })
```

