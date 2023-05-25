# Comparing `tmp/hcai-nova-server-nightly-0.1.6.dev202305250853.tar.gz` & `tmp/hcai-nova-server-nightly-0.1.6.dev202305250922.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hcai-nova-server-nightly-0.1.6.dev202305250853.tar", last modified: Thu May 25 08:53:54 2023, max compression
+gzip compressed data, was "hcai-nova-server-nightly-0.1.6.dev202305250922.tar", last modified: Thu May 25 09:22:34 2023, max compression
```

## Comparing `hcai-nova-server-nightly-0.1.6.dev202305250853.tar` & `hcai-nova-server-nightly-0.1.6.dev202305250922.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 08:53:54.394434 hcai-nova-server-nightly-0.1.6.dev202305250853/
--rw-r--r--   0 runner    (1001) docker     (122)      117 2023-05-25 08:53:43.000000 hcai-nova-server-nightly-0.1.6.dev202305250853/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     1369 2023-05-25 08:53:54.394434 hcai-nova-server-nightly-0.1.6.dev202305250853/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      374 2023-05-25 08:53:43.000000 hcai-nova-server-nightly-0.1.6.dev202305250853/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 08:53:54.394434 hcai-nova-server-nightly-0.1.6.dev202305250853/hcai_nova_server_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1369 2023-05-25 08:53:54.000000 hcai-nova-server-nightly-0.1.6.dev202305250853/hcai_nova_server_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      955 2023-05-25 08:53:54.000000 hcai-nova-server-nightly-0.1.6.dev202305250853/hcai_nova_server_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-25 08:53:54.000000 hcai-nova-server-nightly-0.1.6.dev202305250853/hcai_nova_server_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       56 2023-05-25 08:53:54.000000 hcai-nova-server-nightly-0.1.6.dev202305250853/hcai_nova_server_nightly.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)       75 2023-05-25 08:53:54.000000 hcai-nova-server-nightly-0.1.6.dev202305250853/hcai_nova_server_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-05-25 08:53:54.000000 hcai-nova-server-nightly-0.1.6.dev202305250853/hcai_nova_server_nightly.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 08:53:54.394434 hcai-nova-server-nightly-0.1.6.dev202305250853/nova_server/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 08:53:43.000000 hcai-nova-server-nightly-0.1.6.dev202305250853/nova_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2597 2023-05-25 08:53:43.000000 hcai-nova-server-nightly-0.1.6.dev202305250853/nova_server/app.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 08:53:54.394434 hcai-nova-server-nightly-0.1.6.dev202305250853/nova_server/route/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 08:53:43.000000 hcai-nova-server-nightly-0.1.6.dev202305250853/nova_server/route/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1051 2023-05-25 08:53:43.000000 hcai-nova-server-nightly-0.1.6.dev202305250853/nova_server/route/cancel.py
--rw-r--r--   0 runner    (1001) docker     (122)    13652 2023-05-25 08:53:43.000000 hcai-nova-server-nightly-0.1.6.dev202305250853/nova_server/route/explain.py
--rw-r--r--   0 runner    (1001) docker     (122)     9891 2023-05-25 08:53:43.000000 hcai-nova-server-nightly-0.1.6.dev202305250853/nova_server/route/extract.py
--rw-r--r--   0 runner    (1001) docker     (122)      809 2023-05-25 08:53:43.000000 hcai-nova-server-nightly-0.1.6.dev202305250853/nova_server/route/log.py
--rw-r--r--   0 runner    (1001) docker     (122)     7040 2023-05-25 08:53:43.000000 hcai-nova-server-nightly-0.1.6.dev202305250853/nova_server/route/predict.py
--rw-r--r--   0 runner    (1001) docker     (122)      756 2023-05-25 08:53:43.000000 hcai-nova-server-nightly-0.1.6.dev202305250853/nova_server/route/status.py
--rw-r--r--   0 runner    (1001) docker     (122)     6075 2023-05-25 08:53:43.000000 hcai-nova-server-nightly-0.1.6.dev202305250853/nova_server/route/train.py
--rw-r--r--   0 runner    (1001) docker     (122)      351 2023-05-25 08:53:43.000000 hcai-nova-server-nightly-0.1.6.dev202305250853/nova_server/route/ui.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 08:53:54.394434 hcai-nova-server-nightly-0.1.6.dev202305250853/nova_server/templates/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 08:53:43.000000 hcai-nova-server-nightly-0.1.6.dev202305250853/nova_server/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 08:53:54.394434 hcai-nova-server-nightly-0.1.6.dev202305250853/nova_server/utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 08:53:43.000000 hcai-nova-server-nightly-0.1.6.dev202305250853/nova_server/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2254 2023-05-25 08:53:43.000000 hcai-nova-server-nightly-0.1.6.dev202305250853/nova_server/utils/dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    12139 2023-05-25 08:53:43.000000 hcai-nova-server-nightly-0.1.6.dev202305250853/nova_server/utils/db_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1785 2023-05-25 08:53:43.000000 hcai-nova-server-nightly-0.1.6.dev202305250853/nova_server/utils/explain_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1233 2023-05-25 08:53:43.000000 hcai-nova-server-nightly-0.1.6.dev202305250853/nova_server/utils/import_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      983 2023-05-25 08:53:43.000000 hcai-nova-server-nightly-0.1.6.dev202305250853/nova_server/utils/key_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1375 2023-05-25 08:53:43.000000 hcai-nova-server-nightly-0.1.6.dev202305250853/nova_server/utils/log_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     2159 2023-05-25 08:53:43.000000 hcai-nova-server-nightly-0.1.6.dev202305250853/nova_server/utils/status_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1984 2023-05-25 08:53:43.000000 hcai-nova-server-nightly-0.1.6.dev202305250853/nova_server/utils/thread_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      103 2023-05-25 08:53:43.000000 hcai-nova-server-nightly-0.1.6.dev202305250853/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-25 08:53:54.394434 hcai-nova-server-nightly-0.1.6.dev202305250853/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2526 2023-05-25 08:53:43.000000 hcai-nova-server-nightly-0.1.6.dev202305250853/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 09:22:34.771998 hcai-nova-server-nightly-0.1.6.dev202305250922/
+-rw-r--r--   0 runner    (1001) docker     (122)      117 2023-05-25 09:22:23.000000 hcai-nova-server-nightly-0.1.6.dev202305250922/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1369 2023-05-25 09:22:34.771998 hcai-nova-server-nightly-0.1.6.dev202305250922/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      374 2023-05-25 09:22:23.000000 hcai-nova-server-nightly-0.1.6.dev202305250922/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 09:22:34.771998 hcai-nova-server-nightly-0.1.6.dev202305250922/hcai_nova_server_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1369 2023-05-25 09:22:34.000000 hcai-nova-server-nightly-0.1.6.dev202305250922/hcai_nova_server_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      955 2023-05-25 09:22:34.000000 hcai-nova-server-nightly-0.1.6.dev202305250922/hcai_nova_server_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-25 09:22:34.000000 hcai-nova-server-nightly-0.1.6.dev202305250922/hcai_nova_server_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       56 2023-05-25 09:22:34.000000 hcai-nova-server-nightly-0.1.6.dev202305250922/hcai_nova_server_nightly.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       91 2023-05-25 09:22:34.000000 hcai-nova-server-nightly-0.1.6.dev202305250922/hcai_nova_server_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-05-25 09:22:34.000000 hcai-nova-server-nightly-0.1.6.dev202305250922/hcai_nova_server_nightly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 09:22:34.771998 hcai-nova-server-nightly-0.1.6.dev202305250922/nova_server/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 09:22:23.000000 hcai-nova-server-nightly-0.1.6.dev202305250922/nova_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2597 2023-05-25 09:22:23.000000 hcai-nova-server-nightly-0.1.6.dev202305250922/nova_server/app.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 09:22:34.771998 hcai-nova-server-nightly-0.1.6.dev202305250922/nova_server/route/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 09:22:23.000000 hcai-nova-server-nightly-0.1.6.dev202305250922/nova_server/route/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1051 2023-05-25 09:22:23.000000 hcai-nova-server-nightly-0.1.6.dev202305250922/nova_server/route/cancel.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13652 2023-05-25 09:22:23.000000 hcai-nova-server-nightly-0.1.6.dev202305250922/nova_server/route/explain.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9891 2023-05-25 09:22:23.000000 hcai-nova-server-nightly-0.1.6.dev202305250922/nova_server/route/extract.py
+-rw-r--r--   0 runner    (1001) docker     (122)      809 2023-05-25 09:22:23.000000 hcai-nova-server-nightly-0.1.6.dev202305250922/nova_server/route/log.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7040 2023-05-25 09:22:23.000000 hcai-nova-server-nightly-0.1.6.dev202305250922/nova_server/route/predict.py
+-rw-r--r--   0 runner    (1001) docker     (122)      756 2023-05-25 09:22:23.000000 hcai-nova-server-nightly-0.1.6.dev202305250922/nova_server/route/status.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6075 2023-05-25 09:22:23.000000 hcai-nova-server-nightly-0.1.6.dev202305250922/nova_server/route/train.py
+-rw-r--r--   0 runner    (1001) docker     (122)      351 2023-05-25 09:22:23.000000 hcai-nova-server-nightly-0.1.6.dev202305250922/nova_server/route/ui.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 09:22:34.771998 hcai-nova-server-nightly-0.1.6.dev202305250922/nova_server/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 09:22:23.000000 hcai-nova-server-nightly-0.1.6.dev202305250922/nova_server/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 09:22:34.771998 hcai-nova-server-nightly-0.1.6.dev202305250922/nova_server/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 09:22:23.000000 hcai-nova-server-nightly-0.1.6.dev202305250922/nova_server/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2254 2023-05-25 09:22:23.000000 hcai-nova-server-nightly-0.1.6.dev202305250922/nova_server/utils/dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12139 2023-05-25 09:22:23.000000 hcai-nova-server-nightly-0.1.6.dev202305250922/nova_server/utils/db_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1785 2023-05-25 09:22:23.000000 hcai-nova-server-nightly-0.1.6.dev202305250922/nova_server/utils/explain_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1233 2023-05-25 09:22:23.000000 hcai-nova-server-nightly-0.1.6.dev202305250922/nova_server/utils/import_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      983 2023-05-25 09:22:23.000000 hcai-nova-server-nightly-0.1.6.dev202305250922/nova_server/utils/key_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1375 2023-05-25 09:22:23.000000 hcai-nova-server-nightly-0.1.6.dev202305250922/nova_server/utils/log_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2159 2023-05-25 09:22:23.000000 hcai-nova-server-nightly-0.1.6.dev202305250922/nova_server/utils/status_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1984 2023-05-25 09:22:23.000000 hcai-nova-server-nightly-0.1.6.dev202305250922/nova_server/utils/thread_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      103 2023-05-25 09:22:23.000000 hcai-nova-server-nightly-0.1.6.dev202305250922/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-25 09:22:34.771998 hcai-nova-server-nightly-0.1.6.dev202305250922/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2553 2023-05-25 09:22:23.000000 hcai-nova-server-nightly-0.1.6.dev202305250922/setup.py
```

### Comparing `hcai-nova-server-nightly-0.1.6.dev202305250853/PKG-INFO` & `hcai-nova-server-nightly-0.1.6.dev202305250922/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcai-nova-server-nightly
-Version: 0.1.6.dev202305250853
+Version: 0.1.6.dev202305250922
 Summary: !Alpha Version! - This repository contains code to setup a computational backend server for the nova annotation tool. You can use this backend to train models of your choosing or create explanations for existing models.
 Home-page: https://github.com/pypa/sampleproject
 Author: Dominik Schiller
 Author-email: dominik.schiller@uni-a.de
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `hcai-nova-server-nightly-0.1.6.dev202305250853/hcai_nova_server_nightly.egg-info/PKG-INFO` & `hcai-nova-server-nightly-0.1.6.dev202305250922/hcai_nova_server_nightly.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcai-nova-server-nightly
-Version: 0.1.6.dev202305250853
+Version: 0.1.6.dev202305250922
 Summary: !Alpha Version! - This repository contains code to setup a computational backend server for the nova annotation tool. You can use this backend to train models of your choosing or create explanations for existing models.
 Home-page: https://github.com/pypa/sampleproject
 Author: Dominik Schiller
 Author-email: dominik.schiller@uni-a.de
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `hcai-nova-server-nightly-0.1.6.dev202305250853/hcai_nova_server_nightly.egg-info/SOURCES.txt` & `hcai-nova-server-nightly-0.1.6.dev202305250922/hcai_nova_server_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.6.dev202305250853/nova_server/app.py` & `hcai-nova-server-nightly-0.1.6.dev202305250922/nova_server/app.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.6.dev202305250853/nova_server/route/cancel.py` & `hcai-nova-server-nightly-0.1.6.dev202305250922/nova_server/route/cancel.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.6.dev202305250853/nova_server/route/explain.py` & `hcai-nova-server-nightly-0.1.6.dev202305250922/nova_server/route/explain.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.6.dev202305250853/nova_server/route/extract.py` & `hcai-nova-server-nightly-0.1.6.dev202305250922/nova_server/route/extract.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.6.dev202305250853/nova_server/route/log.py` & `hcai-nova-server-nightly-0.1.6.dev202305250922/nova_server/route/log.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.6.dev202305250853/nova_server/route/predict.py` & `hcai-nova-server-nightly-0.1.6.dev202305250922/nova_server/route/predict.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.6.dev202305250853/nova_server/route/status.py` & `hcai-nova-server-nightly-0.1.6.dev202305250922/nova_server/route/status.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.6.dev202305250853/nova_server/route/train.py` & `hcai-nova-server-nightly-0.1.6.dev202305250922/nova_server/route/train.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.6.dev202305250853/nova_server/utils/dataset_utils.py` & `hcai-nova-server-nightly-0.1.6.dev202305250922/nova_server/utils/dataset_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.6.dev202305250853/nova_server/utils/db_utils.py` & `hcai-nova-server-nightly-0.1.6.dev202305250922/nova_server/utils/db_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.6.dev202305250853/nova_server/utils/explain_utils.py` & `hcai-nova-server-nightly-0.1.6.dev202305250922/nova_server/utils/explain_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.6.dev202305250853/nova_server/utils/import_utils.py` & `hcai-nova-server-nightly-0.1.6.dev202305250922/nova_server/utils/import_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.6.dev202305250853/nova_server/utils/key_utils.py` & `hcai-nova-server-nightly-0.1.6.dev202305250922/nova_server/utils/key_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.6.dev202305250853/nova_server/utils/log_utils.py` & `hcai-nova-server-nightly-0.1.6.dev202305250922/nova_server/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.6.dev202305250853/nova_server/utils/status_utils.py` & `hcai-nova-server-nightly-0.1.6.dev202305250922/nova_server/utils/status_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.6.dev202305250853/nova_server/utils/thread_utils.py` & `hcai-nova-server-nightly-0.1.6.dev202305250922/nova_server/utils/thread_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.6.dev202305250853/setup.py` & `hcai-nova-server-nightly-0.1.6.dev202305250922/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 if nightly:
     project_name += "-nightly"
     datestring = datetime.datetime.now().strftime("%Y%m%d%H%M")
     curr_version = pkg_resources.parse_version(__version__)
     __version__ = f"{curr_version.base_version}.dev{datestring}"
     install_requires=[
         "hcai-datasets-nightly",
+        "hcai-nova-utils",
         "Flask == 2.0.2",
         "imbalanced-learn==0.8.1",
         "waitress==2.0.0",
     ]
 
 # Setup
 setup(
```

