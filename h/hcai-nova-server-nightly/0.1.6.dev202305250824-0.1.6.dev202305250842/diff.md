# Comparing `tmp/hcai-nova-server-nightly-0.1.6.dev202305250824.tar.gz` & `tmp/hcai-nova-server-nightly-0.1.6.dev202305250842.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hcai-nova-server-nightly-0.1.6.dev202305250824.tar", last modified: Thu May 25 08:24:40 2023, max compression
+gzip compressed data, was "hcai-nova-server-nightly-0.1.6.dev202305250842.tar", last modified: Thu May 25 08:42:47 2023, max compression
```

## Comparing `hcai-nova-server-nightly-0.1.6.dev202305250824.tar` & `hcai-nova-server-nightly-0.1.6.dev202305250842.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 08:24:40.292440 hcai-nova-server-nightly-0.1.6.dev202305250824/
--rw-r--r--   0 runner    (1001) docker     (122)      117 2023-05-25 08:24:24.000000 hcai-nova-server-nightly-0.1.6.dev202305250824/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     1369 2023-05-25 08:24:40.292440 hcai-nova-server-nightly-0.1.6.dev202305250824/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      374 2023-05-25 08:24:24.000000 hcai-nova-server-nightly-0.1.6.dev202305250824/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 08:24:40.288440 hcai-nova-server-nightly-0.1.6.dev202305250824/hcai_nova_server_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1369 2023-05-25 08:24:40.000000 hcai-nova-server-nightly-0.1.6.dev202305250824/hcai_nova_server_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      963 2023-05-25 08:24:40.000000 hcai-nova-server-nightly-0.1.6.dev202305250824/hcai_nova_server_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-25 08:24:40.000000 hcai-nova-server-nightly-0.1.6.dev202305250824/hcai_nova_server_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       64 2023-05-25 08:24:40.000000 hcai-nova-server-nightly-0.1.6.dev202305250824/hcai_nova_server_nightly.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)       75 2023-05-25 08:24:40.000000 hcai-nova-server-nightly-0.1.6.dev202305250824/hcai_nova_server_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-05-25 08:24:40.000000 hcai-nova-server-nightly-0.1.6.dev202305250824/hcai_nova_server_nightly.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 08:24:40.288440 hcai-nova-server-nightly-0.1.6.dev202305250824/nova_server/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 08:24:24.000000 hcai-nova-server-nightly-0.1.6.dev202305250824/nova_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2597 2023-05-25 08:24:24.000000 hcai-nova-server-nightly-0.1.6.dev202305250824/nova_server/nova_server.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 08:24:40.288440 hcai-nova-server-nightly-0.1.6.dev202305250824/nova_server/route/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 08:24:24.000000 hcai-nova-server-nightly-0.1.6.dev202305250824/nova_server/route/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1051 2023-05-25 08:24:24.000000 hcai-nova-server-nightly-0.1.6.dev202305250824/nova_server/route/cancel.py
--rw-r--r--   0 runner    (1001) docker     (122)    13652 2023-05-25 08:24:24.000000 hcai-nova-server-nightly-0.1.6.dev202305250824/nova_server/route/explain.py
--rw-r--r--   0 runner    (1001) docker     (122)     9891 2023-05-25 08:24:24.000000 hcai-nova-server-nightly-0.1.6.dev202305250824/nova_server/route/extract.py
--rw-r--r--   0 runner    (1001) docker     (122)      809 2023-05-25 08:24:24.000000 hcai-nova-server-nightly-0.1.6.dev202305250824/nova_server/route/log.py
--rw-r--r--   0 runner    (1001) docker     (122)     7040 2023-05-25 08:24:24.000000 hcai-nova-server-nightly-0.1.6.dev202305250824/nova_server/route/predict.py
--rw-r--r--   0 runner    (1001) docker     (122)      756 2023-05-25 08:24:24.000000 hcai-nova-server-nightly-0.1.6.dev202305250824/nova_server/route/status.py
--rw-r--r--   0 runner    (1001) docker     (122)     6075 2023-05-25 08:24:24.000000 hcai-nova-server-nightly-0.1.6.dev202305250824/nova_server/route/train.py
--rw-r--r--   0 runner    (1001) docker     (122)      351 2023-05-25 08:24:24.000000 hcai-nova-server-nightly-0.1.6.dev202305250824/nova_server/route/ui.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 08:24:40.292440 hcai-nova-server-nightly-0.1.6.dev202305250824/nova_server/templates/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 08:24:24.000000 hcai-nova-server-nightly-0.1.6.dev202305250824/nova_server/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 08:24:40.292440 hcai-nova-server-nightly-0.1.6.dev202305250824/nova_server/utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 08:24:24.000000 hcai-nova-server-nightly-0.1.6.dev202305250824/nova_server/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2254 2023-05-25 08:24:24.000000 hcai-nova-server-nightly-0.1.6.dev202305250824/nova_server/utils/dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    12139 2023-05-25 08:24:24.000000 hcai-nova-server-nightly-0.1.6.dev202305250824/nova_server/utils/db_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1785 2023-05-25 08:24:24.000000 hcai-nova-server-nightly-0.1.6.dev202305250824/nova_server/utils/explain_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1233 2023-05-25 08:24:24.000000 hcai-nova-server-nightly-0.1.6.dev202305250824/nova_server/utils/import_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      983 2023-05-25 08:24:24.000000 hcai-nova-server-nightly-0.1.6.dev202305250824/nova_server/utils/key_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1375 2023-05-25 08:24:24.000000 hcai-nova-server-nightly-0.1.6.dev202305250824/nova_server/utils/log_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     2159 2023-05-25 08:24:24.000000 hcai-nova-server-nightly-0.1.6.dev202305250824/nova_server/utils/status_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1984 2023-05-25 08:24:24.000000 hcai-nova-server-nightly-0.1.6.dev202305250824/nova_server/utils/thread_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      103 2023-05-25 08:24:24.000000 hcai-nova-server-nightly-0.1.6.dev202305250824/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-25 08:24:40.292440 hcai-nova-server-nightly-0.1.6.dev202305250824/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2511 2023-05-25 08:24:24.000000 hcai-nova-server-nightly-0.1.6.dev202305250824/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 08:42:47.655534 hcai-nova-server-nightly-0.1.6.dev202305250842/
+-rw-r--r--   0 runner    (1001) docker     (122)      117 2023-05-25 08:42:32.000000 hcai-nova-server-nightly-0.1.6.dev202305250842/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1369 2023-05-25 08:42:47.655534 hcai-nova-server-nightly-0.1.6.dev202305250842/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      374 2023-05-25 08:42:32.000000 hcai-nova-server-nightly-0.1.6.dev202305250842/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 08:42:47.651534 hcai-nova-server-nightly-0.1.6.dev202305250842/hcai_nova_server_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1369 2023-05-25 08:42:47.000000 hcai-nova-server-nightly-0.1.6.dev202305250842/hcai_nova_server_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      955 2023-05-25 08:42:47.000000 hcai-nova-server-nightly-0.1.6.dev202305250842/hcai_nova_server_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-25 08:42:47.000000 hcai-nova-server-nightly-0.1.6.dev202305250842/hcai_nova_server_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       56 2023-05-25 08:42:47.000000 hcai-nova-server-nightly-0.1.6.dev202305250842/hcai_nova_server_nightly.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       75 2023-05-25 08:42:47.000000 hcai-nova-server-nightly-0.1.6.dev202305250842/hcai_nova_server_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-05-25 08:42:47.000000 hcai-nova-server-nightly-0.1.6.dev202305250842/hcai_nova_server_nightly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 08:42:47.651534 hcai-nova-server-nightly-0.1.6.dev202305250842/nova_server/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 08:42:33.000000 hcai-nova-server-nightly-0.1.6.dev202305250842/nova_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2597 2023-05-25 08:42:33.000000 hcai-nova-server-nightly-0.1.6.dev202305250842/nova_server/app.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 08:42:47.655534 hcai-nova-server-nightly-0.1.6.dev202305250842/nova_server/route/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 08:42:33.000000 hcai-nova-server-nightly-0.1.6.dev202305250842/nova_server/route/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1051 2023-05-25 08:42:33.000000 hcai-nova-server-nightly-0.1.6.dev202305250842/nova_server/route/cancel.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13652 2023-05-25 08:42:33.000000 hcai-nova-server-nightly-0.1.6.dev202305250842/nova_server/route/explain.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9891 2023-05-25 08:42:33.000000 hcai-nova-server-nightly-0.1.6.dev202305250842/nova_server/route/extract.py
+-rw-r--r--   0 runner    (1001) docker     (122)      809 2023-05-25 08:42:33.000000 hcai-nova-server-nightly-0.1.6.dev202305250842/nova_server/route/log.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7040 2023-05-25 08:42:33.000000 hcai-nova-server-nightly-0.1.6.dev202305250842/nova_server/route/predict.py
+-rw-r--r--   0 runner    (1001) docker     (122)      756 2023-05-25 08:42:33.000000 hcai-nova-server-nightly-0.1.6.dev202305250842/nova_server/route/status.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6075 2023-05-25 08:42:33.000000 hcai-nova-server-nightly-0.1.6.dev202305250842/nova_server/route/train.py
+-rw-r--r--   0 runner    (1001) docker     (122)      351 2023-05-25 08:42:33.000000 hcai-nova-server-nightly-0.1.6.dev202305250842/nova_server/route/ui.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 08:42:47.655534 hcai-nova-server-nightly-0.1.6.dev202305250842/nova_server/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 08:42:33.000000 hcai-nova-server-nightly-0.1.6.dev202305250842/nova_server/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 08:42:47.655534 hcai-nova-server-nightly-0.1.6.dev202305250842/nova_server/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 08:42:33.000000 hcai-nova-server-nightly-0.1.6.dev202305250842/nova_server/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2254 2023-05-25 08:42:33.000000 hcai-nova-server-nightly-0.1.6.dev202305250842/nova_server/utils/dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12139 2023-05-25 08:42:33.000000 hcai-nova-server-nightly-0.1.6.dev202305250842/nova_server/utils/db_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1785 2023-05-25 08:42:33.000000 hcai-nova-server-nightly-0.1.6.dev202305250842/nova_server/utils/explain_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1233 2023-05-25 08:42:33.000000 hcai-nova-server-nightly-0.1.6.dev202305250842/nova_server/utils/import_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      983 2023-05-25 08:42:33.000000 hcai-nova-server-nightly-0.1.6.dev202305250842/nova_server/utils/key_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1375 2023-05-25 08:42:33.000000 hcai-nova-server-nightly-0.1.6.dev202305250842/nova_server/utils/log_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2159 2023-05-25 08:42:33.000000 hcai-nova-server-nightly-0.1.6.dev202305250842/nova_server/utils/status_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1984 2023-05-25 08:42:33.000000 hcai-nova-server-nightly-0.1.6.dev202305250842/nova_server/utils/thread_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      103 2023-05-25 08:42:33.000000 hcai-nova-server-nightly-0.1.6.dev202305250842/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-25 08:42:47.655534 hcai-nova-server-nightly-0.1.6.dev202305250842/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2503 2023-05-25 08:42:33.000000 hcai-nova-server-nightly-0.1.6.dev202305250842/setup.py
```

### Comparing `hcai-nova-server-nightly-0.1.6.dev202305250824/PKG-INFO` & `hcai-nova-server-nightly-0.1.6.dev202305250842/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcai-nova-server-nightly
-Version: 0.1.6.dev202305250824
+Version: 0.1.6.dev202305250842
 Summary: !Alpha Version! - This repository contains code to setup a computational backend server for the nova annotation tool. You can use this backend to train models of your choosing or create explanations for existing models.
 Home-page: https://github.com/pypa/sampleproject
 Author: Dominik Schiller
 Author-email: dominik.schiller@uni-a.de
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `hcai-nova-server-nightly-0.1.6.dev202305250824/hcai_nova_server_nightly.egg-info/PKG-INFO` & `hcai-nova-server-nightly-0.1.6.dev202305250842/hcai_nova_server_nightly.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcai-nova-server-nightly
-Version: 0.1.6.dev202305250824
+Version: 0.1.6.dev202305250842
 Summary: !Alpha Version! - This repository contains code to setup a computational backend server for the nova annotation tool. You can use this backend to train models of your choosing or create explanations for existing models.
 Home-page: https://github.com/pypa/sampleproject
 Author: Dominik Schiller
 Author-email: dominik.schiller@uni-a.de
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `hcai-nova-server-nightly-0.1.6.dev202305250824/hcai_nova_server_nightly.egg-info/SOURCES.txt` & `hcai-nova-server-nightly-0.1.6.dev202305250842/hcai_nova_server_nightly.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 hcai_nova_server_nightly.egg-info/PKG-INFO
 hcai_nova_server_nightly.egg-info/SOURCES.txt
 hcai_nova_server_nightly.egg-info/dependency_links.txt
 hcai_nova_server_nightly.egg-info/entry_points.txt
 hcai_nova_server_nightly.egg-info/requires.txt
 hcai_nova_server_nightly.egg-info/top_level.txt
 nova_server/__init__.py
-nova_server/nova_server.py
+nova_server/app.py
 nova_server/route/__init__.py
 nova_server/route/cancel.py
 nova_server/route/explain.py
 nova_server/route/extract.py
 nova_server/route/log.py
 nova_server/route/predict.py
 nova_server/route/status.py
```

### Comparing `hcai-nova-server-nightly-0.1.6.dev202305250824/nova_server/nova_server.py` & `hcai-nova-server-nightly-0.1.6.dev202305250842/nova_server/app.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.6.dev202305250824/nova_server/route/cancel.py` & `hcai-nova-server-nightly-0.1.6.dev202305250842/nova_server/route/cancel.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.6.dev202305250824/nova_server/route/explain.py` & `hcai-nova-server-nightly-0.1.6.dev202305250842/nova_server/route/explain.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.6.dev202305250824/nova_server/route/extract.py` & `hcai-nova-server-nightly-0.1.6.dev202305250842/nova_server/route/extract.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.6.dev202305250824/nova_server/route/log.py` & `hcai-nova-server-nightly-0.1.6.dev202305250842/nova_server/route/log.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.6.dev202305250824/nova_server/route/predict.py` & `hcai-nova-server-nightly-0.1.6.dev202305250842/nova_server/route/predict.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.6.dev202305250824/nova_server/route/status.py` & `hcai-nova-server-nightly-0.1.6.dev202305250842/nova_server/route/status.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.6.dev202305250824/nova_server/route/train.py` & `hcai-nova-server-nightly-0.1.6.dev202305250842/nova_server/route/train.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.6.dev202305250824/nova_server/utils/dataset_utils.py` & `hcai-nova-server-nightly-0.1.6.dev202305250842/nova_server/utils/dataset_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.6.dev202305250824/nova_server/utils/db_utils.py` & `hcai-nova-server-nightly-0.1.6.dev202305250842/nova_server/utils/db_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.6.dev202305250824/nova_server/utils/explain_utils.py` & `hcai-nova-server-nightly-0.1.6.dev202305250842/nova_server/utils/explain_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.6.dev202305250824/nova_server/utils/import_utils.py` & `hcai-nova-server-nightly-0.1.6.dev202305250842/nova_server/utils/import_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.6.dev202305250824/nova_server/utils/key_utils.py` & `hcai-nova-server-nightly-0.1.6.dev202305250842/nova_server/utils/key_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.6.dev202305250824/nova_server/utils/log_utils.py` & `hcai-nova-server-nightly-0.1.6.dev202305250842/nova_server/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.6.dev202305250824/nova_server/utils/status_utils.py` & `hcai-nova-server-nightly-0.1.6.dev202305250842/nova_server/utils/status_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.6.dev202305250824/nova_server/utils/thread_utils.py` & `hcai-nova-server-nightly-0.1.6.dev202305250842/nova_server/utils/thread_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.6.dev202305250824/setup.py` & `hcai-nova-server-nightly-0.1.6.dev202305250842/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,11 +69,11 @@
     packages=find_packages(exclude=["*tests*"]),
     python_requires=">=3.6, <4",
     install_requires = install_requires,
     include_package_data=True,
     package_data={"": ["*.csv"]},
     entry_points = {
         'console_scripts': [
-            'nova-server = nova_server.nova_server:run_app',
+            'nova-server = nova_server.app:run_app',
         ]
     }
 )
```

