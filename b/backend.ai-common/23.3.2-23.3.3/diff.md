# Comparing `tmp/backend.ai-common-23.3.2.tar.gz` & `tmp/backend.ai-common-23.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backend.ai-common-23.3.2.tar", last modified: Fri May  5 07:08:12 2023, max compression
+gzip compressed data, was "backend.ai-common-23.3.3.tar", last modified: Thu May 25 17:30:46 2023, max compression
```

## Comparing `backend.ai-common-23.3.2.tar` & `backend.ai-common-23.3.3.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:12.142857 backend.ai-common-23.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-05 07:08:11.000000 backend.ai-common-23.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-05-05 07:08:12.142857 backend.ai-common-23.3.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:12.134857 backend.ai-common-23.3.2/ai/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:12.134857 backend.ai-common-23.3.2/ai/backend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:12.138857 backend.ai-common-23.3.2/ai/backend/common/
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-05 07:08:11.000000 backend.ai-common-23.3.2/ai/backend/common/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-05 07:08:11.000000 backend.ai-common-23.3.2/ai/backend/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-05 07:08:11.000000 backend.ai-common-23.3.2/ai/backend/common/arch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-05-05 07:08:11.000000 backend.ai-common-23.3.2/ai/backend/common/argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-05-05 07:08:11.000000 backend.ai-common-23.3.2/ai/backend/common/asyncio.py
--rw-r--r--   0 runner    (1001) docker     (123)    11022 2023-05-05 07:08:11.000000 backend.ai-common-23.3.2/ai/backend/common/bgtask.py
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-05-05 07:08:11.000000 backend.ai-common-23.3.2/ai/backend/common/cgroup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-05-05 07:08:11.000000 backend.ai-common-23.3.2/ai/backend/common/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4622 2023-05-05 07:08:11.000000 backend.ai-common-23.3.2/ai/backend/common/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-05-05 07:08:11.000000 backend.ai-common-23.3.2/ai/backend/common/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)    18046 2023-05-05 07:08:11.000000 backend.ai-common-23.3.2/ai/backend/common/docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-05 07:08:11.000000 backend.ai-common-23.3.2/ai/backend/common/enum_extension.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-05 07:08:11.000000 backend.ai-common-23.3.2/ai/backend/common/enum_extension.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    19237 2023-05-05 07:08:11.000000 backend.ai-common-23.3.2/ai/backend/common/etcd.py
--rw-r--r--   0 runner    (1001) docker     (123)    26166 2023-05-05 07:08:11.000000 backend.ai-common-23.3.2/ai/backend/common/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-05-05 07:08:11.000000 backend.ai-common-23.3.2/ai/backend/common/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-05-05 07:08:11.000000 backend.ai-common-23.3.2/ai/backend/common/files.py
--rw-r--r--   0 runner    (1001) docker     (123)     9077 2023-05-05 07:08:11.000000 backend.ai-common-23.3.2/ai/backend/common/identity.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-05 07:08:11.000000 backend.ai-common-23.3.2/ai/backend/common/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     7882 2023-05-05 07:08:11.000000 backend.ai-common-23.3.2/ai/backend/common/lock.py
--rw-r--r--   0 runner    (1001) docker     (123)    21123 2023-05-05 07:08:11.000000 backend.ai-common-23.3.2/ai/backend/common/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-05 07:08:11.000000 backend.ai-common-23.3.2/ai/backend/common/logging_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-05-05 07:08:11.000000 backend.ai-common-23.3.2/ai/backend/common/msgpack.py
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-05 07:08:11.000000 backend.ai-common-23.3.2/ai/backend/common/netns.py
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-05-05 07:08:11.000000 backend.ai-common-23.3.2/ai/backend/common/networking.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:12.142857 backend.ai-common-23.3.2/ai/backend/common/plugin/
--rw-r--r--   0 runner    (1001) docker     (123)     7078 2023-05-05 07:08:11.000000 backend.ai-common-23.3.2/ai/backend/common/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-05-05 07:08:11.000000 backend.ai-common-23.3.2/ai/backend/common/plugin/hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-05-05 07:08:11.000000 backend.ai-common-23.3.2/ai/backend/common/plugin/monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-05 07:08:11.000000 backend.ai-common-23.3.2/ai/backend/common/plugin/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-05 07:08:11.000000 backend.ai-common-23.3.2/ai/backend/common/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    16476 2023-05-05 07:08:11.000000 backend.ai-common-23.3.2/ai/backend/common/redis_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-05-05 07:08:11.000000 backend.ai-common-23.3.2/ai/backend/common/sd_notify.py
--rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-05-05 07:08:11.000000 backend.ai-common-23.3.2/ai/backend/common/service_ports.py
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-05-05 07:08:11.000000 backend.ai-common-23.3.2/ai/backend/common/testutils.py
--rw-r--r--   0 runner    (1001) docker     (123)    30192 2023-05-05 07:08:11.000000 backend.ai-common-23.3.2/ai/backend/common/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     8911 2023-05-05 07:08:11.000000 backend.ai-common-23.3.2/ai/backend/common/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    22692 2023-05-05 07:08:11.000000 backend.ai-common-23.3.2/ai/backend/common/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:12.134857 backend.ai-common-23.3.2/ai/backend/common/web/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:12.142857 backend.ai-common-23.3.2/ai/backend/common/web/session/
--rw-r--r--   0 runner    (1001) docker     (123)    10798 2023-05-05 07:08:11.000000 backend.ai-common-23.3.2/ai/backend/common/web/session/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-05-05 07:08:11.000000 backend.ai-common-23.3.2/ai/backend/common/web/session/redis_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:12.142857 backend.ai-common-23.3.2/backend.ai_common.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-05-05 07:08:12.000000 backend.ai-common-23.3.2/backend.ai_common.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-05-05 07:08:12.000000 backend.ai-common-23.3.2/backend.ai_common.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 07:08:12.000000 backend.ai-common-23.3.2/backend.ai_common.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 07:08:12.000000 backend.ai-common-23.3.2/backend.ai_common.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 07:08:11.000000 backend.ai-common-23.3.2/backend.ai_common.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-05 07:08:12.000000 backend.ai-common-23.3.2/backend.ai_common.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-05 07:08:12.000000 backend.ai-common-23.3.2/backend.ai_common.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-05 07:08:11.000000 backend.ai-common-23.3.2/backend_shim.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 07:08:12.142857 backend.ai-common-23.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-05-05 07:08:11.000000 backend.ai-common-23.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:46.245153 backend.ai-common-23.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-25 17:30:45.000000 backend.ai-common-23.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-05-25 17:30:46.245153 backend.ai-common-23.3.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:46.237153 backend.ai-common-23.3.3/ai/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:46.237153 backend.ai-common-23.3.3/ai/backend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:46.245153 backend.ai-common-23.3.3/ai/backend/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-25 17:30:45.000000 backend.ai-common-23.3.3/ai/backend/common/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-25 17:30:45.000000 backend.ai-common-23.3.3/ai/backend/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-25 17:30:45.000000 backend.ai-common-23.3.3/ai/backend/common/arch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-05-25 17:30:45.000000 backend.ai-common-23.3.3/ai/backend/common/argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-05-25 17:30:45.000000 backend.ai-common-23.3.3/ai/backend/common/asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11022 2023-05-25 17:30:45.000000 backend.ai-common-23.3.3/ai/backend/common/bgtask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-05-25 17:30:45.000000 backend.ai-common-23.3.3/ai/backend/common/cgroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-05-25 17:30:45.000000 backend.ai-common-23.3.3/ai/backend/common/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4622 2023-05-25 17:30:45.000000 backend.ai-common-23.3.3/ai/backend/common/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-05-25 17:30:45.000000 backend.ai-common-23.3.3/ai/backend/common/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18046 2023-05-25 17:30:45.000000 backend.ai-common-23.3.3/ai/backend/common/docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-25 17:30:45.000000 backend.ai-common-23.3.3/ai/backend/common/enum_extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-25 17:30:45.000000 backend.ai-common-23.3.3/ai/backend/common/enum_extension.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    19237 2023-05-25 17:30:45.000000 backend.ai-common-23.3.3/ai/backend/common/etcd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26166 2023-05-25 17:30:45.000000 backend.ai-common-23.3.3/ai/backend/common/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-05-25 17:30:45.000000 backend.ai-common-23.3.3/ai/backend/common/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-05-25 17:30:45.000000 backend.ai-common-23.3.3/ai/backend/common/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9077 2023-05-25 17:30:45.000000 backend.ai-common-23.3.3/ai/backend/common/identity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-25 17:30:45.000000 backend.ai-common-23.3.3/ai/backend/common/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7882 2023-05-25 17:30:45.000000 backend.ai-common-23.3.3/ai/backend/common/lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21123 2023-05-25 17:30:45.000000 backend.ai-common-23.3.3/ai/backend/common/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-25 17:30:45.000000 backend.ai-common-23.3.3/ai/backend/common/logging_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-05-25 17:30:45.000000 backend.ai-common-23.3.3/ai/backend/common/msgpack.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-25 17:30:45.000000 backend.ai-common-23.3.3/ai/backend/common/netns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-05-25 17:30:45.000000 backend.ai-common-23.3.3/ai/backend/common/networking.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:46.245153 backend.ai-common-23.3.3/ai/backend/common/plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)     7078 2023-05-25 17:30:45.000000 backend.ai-common-23.3.3/ai/backend/common/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-05-25 17:30:45.000000 backend.ai-common-23.3.3/ai/backend/common/plugin/hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-05-25 17:30:45.000000 backend.ai-common-23.3.3/ai/backend/common/plugin/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-25 17:30:45.000000 backend.ai-common-23.3.3/ai/backend/common/plugin/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-25 17:30:45.000000 backend.ai-common-23.3.3/ai/backend/common/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    16566 2023-05-25 17:30:45.000000 backend.ai-common-23.3.3/ai/backend/common/redis_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-05-25 17:30:45.000000 backend.ai-common-23.3.3/ai/backend/common/sd_notify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-05-25 17:30:45.000000 backend.ai-common-23.3.3/ai/backend/common/service_ports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-05-25 17:30:45.000000 backend.ai-common-23.3.3/ai/backend/common/testutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30366 2023-05-25 17:30:45.000000 backend.ai-common-23.3.3/ai/backend/common/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8911 2023-05-25 17:30:45.000000 backend.ai-common-23.3.3/ai/backend/common/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22692 2023-05-25 17:30:45.000000 backend.ai-common-23.3.3/ai/backend/common/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:46.237153 backend.ai-common-23.3.3/ai/backend/common/web/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:46.245153 backend.ai-common-23.3.3/ai/backend/common/web/session/
+-rw-r--r--   0 runner    (1001) docker     (123)    10798 2023-05-25 17:30:45.000000 backend.ai-common-23.3.3/ai/backend/common/web/session/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-05-25 17:30:45.000000 backend.ai-common-23.3.3/ai/backend/common/web/session/redis_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:46.245153 backend.ai-common-23.3.3/backend.ai_common.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-05-25 17:30:46.000000 backend.ai-common-23.3.3/backend.ai_common.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-05-25 17:30:46.000000 backend.ai-common-23.3.3/backend.ai_common.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 17:30:46.000000 backend.ai-common-23.3.3/backend.ai_common.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 17:30:46.000000 backend.ai-common-23.3.3/backend.ai_common.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 17:30:46.000000 backend.ai-common-23.3.3/backend.ai_common.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-25 17:30:46.000000 backend.ai-common-23.3.3/backend.ai_common.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-25 17:30:46.000000 backend.ai-common-23.3.3/backend.ai_common.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-25 17:30:45.000000 backend.ai-common-23.3.3/backend_shim.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 17:30:46.245153 backend.ai-common-23.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-05-25 17:30:45.000000 backend.ai-common-23.3.3/setup.py
```

### Comparing `backend.ai-common-23.3.2/PKG-INFO` & `backend.ai-common-23.3.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-common
-Version: 23.3.2
+Version: 23.3.3
 Summary: Backend.AI commons library
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
 
 Backend.AI Commons
 ==================
```

### Comparing `backend.ai-common-23.3.2/ai/backend/common/argparse.py` & `backend.ai-common-23.3.3/ai/backend/common/argparse.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.2/ai/backend/common/asyncio.py` & `backend.ai-common-23.3.3/ai/backend/common/asyncio.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.2/ai/backend/common/bgtask.py` & `backend.ai-common-23.3.3/ai/backend/common/bgtask.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.2/ai/backend/common/cgroup.py` & `backend.ai-common-23.3.3/ai/backend/common/cgroup.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.2/ai/backend/common/cli.py` & `backend.ai-common-23.3.3/ai/backend/common/cli.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.2/ai/backend/common/config.py` & `backend.ai-common-23.3.3/ai/backend/common/config.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.2/ai/backend/common/distributed.py` & `backend.ai-common-23.3.3/ai/backend/common/distributed.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.2/ai/backend/common/docker.py` & `backend.ai-common-23.3.3/ai/backend/common/docker.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.2/ai/backend/common/enum_extension.py` & `backend.ai-common-23.3.3/ai/backend/common/enum_extension.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.2/ai/backend/common/enum_extension.pyi` & `backend.ai-common-23.3.3/ai/backend/common/enum_extension.pyi`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.2/ai/backend/common/etcd.py` & `backend.ai-common-23.3.3/ai/backend/common/etcd.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.2/ai/backend/common/events.py` & `backend.ai-common-23.3.3/ai/backend/common/events.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.2/ai/backend/common/exception.py` & `backend.ai-common-23.3.3/ai/backend/common/exception.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.2/ai/backend/common/files.py` & `backend.ai-common-23.3.3/ai/backend/common/files.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.2/ai/backend/common/identity.py` & `backend.ai-common-23.3.3/ai/backend/common/identity.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.2/ai/backend/common/lock.py` & `backend.ai-common-23.3.3/ai/backend/common/lock.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,15 +79,15 @@
             log.debug("file lock implicitly released: {}", self._path)
 
     async def acquire(self) -> None:
         assert self._file is None
         assert not self._locked
         if not self._path.exists():
             self._path.touch()
-        self._file = open(self._path, "rb")
+        self._file = open(self._path, "wb")
         stop_func = stop_never if self._timeout <= 0 else stop_after_delay(self._timeout)
         try:
             async for attempt in AsyncRetrying(
                 retry=retry_if_exception_type(BlockingIOError),
                 wait=wait_exponential(multiplier=0.02, min=0.02, max=1.0) + wait_random(0, 0.05),
                 stop=stop_func,
             ):
```

### Comparing `backend.ai-common-23.3.2/ai/backend/common/logging.py` & `backend.ai-common-23.3.3/ai/backend/common/logging.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.2/ai/backend/common/logging_utils.py` & `backend.ai-common-23.3.3/ai/backend/common/logging_utils.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.2/ai/backend/common/msgpack.py` & `backend.ai-common-23.3.3/ai/backend/common/msgpack.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.2/ai/backend/common/netns.py` & `backend.ai-common-23.3.3/ai/backend/common/netns.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.2/ai/backend/common/networking.py` & `backend.ai-common-23.3.3/ai/backend/common/networking.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.2/ai/backend/common/plugin/__init__.py` & `backend.ai-common-23.3.3/ai/backend/common/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.2/ai/backend/common/plugin/hook.py` & `backend.ai-common-23.3.3/ai/backend/common/plugin/hook.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.2/ai/backend/common/plugin/monitor.py` & `backend.ai-common-23.3.3/ai/backend/common/plugin/monitor.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.2/ai/backend/common/redis_helper.py` & `backend.ai-common-23.3.3/ai/backend/common/redis_helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -245,25 +245,27 @@
                 if callable(func):
                     aw_or_pipe = func(r)
                 else:
                     raise TypeError(
                         "The func must be a function or a coroutinefunction with no arguments."
                     )
                 if isinstance(aw_or_pipe, Pipeline):
-                    result = await aw_or_pipe.execute()
+                    async with aw_or_pipe:
+                        result = await aw_or_pipe.execute()
                 elif inspect.isawaitable(aw_or_pipe):
                     result = await aw_or_pipe
                 else:
                     raise TypeError(
                         "The return value must be an awaitable"
                         "or redis.asyncio.client.Pipeline object"
                     )
                 if isinstance(result, Pipeline):
                     # This happens when func is an async function that returns a pipeline.
-                    result = await result.execute()
+                    async with result:
+                        result = await result.execute()
                 if encoding:
                     if isinstance(result, bytes):
                         return result.decode(encoding)
                     elif isinstance(result, dict):
                         newdict = {}
                         for k, v in result.items():
                             newdict[k.decode(encoding)] = v.decode(encoding)
```

### Comparing `backend.ai-common-23.3.2/ai/backend/common/sd_notify.py` & `backend.ai-common-23.3.3/ai/backend/common/sd_notify.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.2/ai/backend/common/service_ports.py` & `backend.ai-common-23.3.3/ai/backend/common/service_ports.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.2/ai/backend/common/testutils.py` & `backend.ai-common-23.3.3/ai/backend/common/testutils.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.2/ai/backend/common/types.py` & `backend.ai-common-23.3.3/ai/backend/common/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -288,14 +288,24 @@
 
 
 class CommitStatus(str, enum.Enum):
     READY = "ready"
     ONGOING = "ongoing"
 
 
+class AbuseReportValue(str, enum.Enum):
+    DETECTED = "detected"
+    CLEANING = "cleaning"
+
+
+class AbuseReport(TypedDict):
+    kernel: str
+    abuse_report: Optional[str]
+
+
 class MovingStatValue(TypedDict):
     min: str
     max: str
     sum: str
     avg: str
     diff: str
     rate: str
```

### Comparing `backend.ai-common-23.3.2/ai/backend/common/utils.py` & `backend.ai-common-23.3.3/ai/backend/common/utils.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.2/ai/backend/common/validators.py` & `backend.ai-common-23.3.3/ai/backend/common/validators.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.2/ai/backend/common/web/session/__init__.py` & `backend.ai-common-23.3.3/ai/backend/common/web/session/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.2/ai/backend/common/web/session/redis_storage.py` & `backend.ai-common-23.3.3/ai/backend/common/web/session/redis_storage.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.2/backend.ai_common.egg-info/PKG-INFO` & `backend.ai-common-23.3.3/backend.ai_common.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-common
-Version: 23.3.2
+Version: 23.3.3
 Summary: Backend.AI commons library
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
 
 Backend.AI Commons
 ==================
```

### Comparing `backend.ai-common-23.3.2/backend.ai_common.egg-info/SOURCES.txt` & `backend.ai-common-23.3.3/backend.ai_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.2/backend_shim.py` & `backend.ai-common-23.3.3/backend_shim.py`

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

### Comparing `backend.ai-common-23.3.2/setup.py` & `backend.ai-common-23.3.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,42 +12,43 @@
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
     'description': 'Backend.AI commons library',
     'install_requires': (
         'PyJWT~=2.0',
         'aiodns>=3.0',
         'aiohttp_sse>=2.0',
         'aiohttp~=3.8.1',
         'aiomonitor-ng~=0.7.2',
         'aiotools~=1.6.1',
         'async_timeout~=4.0',
         'asynctest>=0.13.0',
         'asyncudp>=0.4',
         'attrs>=20.3',
-        """backend.ai-plugin==23.03.2
+        """backend.ai-plugin==23.03.3
 """,
         'click>=7.1.2',
         'coloredlogs~=15.0',
         'etcetra==0.1.15',
         'ifaddr~=0.2',
         'janus~=1.0.0',
         'msgpack>=1.0.5rc1',
         'multidict>=6.0',
         'packaging>=21.3',
         'python-dateutil>=2.8',
         'python-json-logger>=2.0.1',
         'pyzmq~=24.0.1',
-        'redis[hiredis]~=4.3.4',
+        'redis[hiredis]~=4.5.5',
         'tblib~=1.7',
         'temporenc~=0.1.0',
         'tenacity>=8.0',
         'tomli~=2.0.1',
         'trafaret~=2.1',
         'typeguard~=2.10',
         'typing_extensions~=4.3',
@@ -115,11 +116,11 @@
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

