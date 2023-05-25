# Comparing `tmp/arkindex-base-worker-0.3.3rc3.tar.gz` & `tmp/arkindex-base-worker-0.3.3rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arkindex-base-worker-0.3.3rc3.tar", last modified: Fri Apr 28 11:09:42 2023, max compression
+gzip compressed data, was "arkindex-base-worker-0.3.3rc4.tar", last modified: Thu May 25 06:43:45 2023, max compression
```

## Comparing `arkindex-base-worker-0.3.3rc3.tar` & `arkindex-base-worker-0.3.3rc4.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 11:09:42.643734 arkindex-base-worker-0.3.3rc3/
--rw-r--r--   0 root         (0) root         (0)      248 2023-04-28 11:09:42.643734 arkindex-base-worker-0.3.3rc3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      233 2023-04-28 10:09:46.000000 arkindex-base-worker-0.3.3rc3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 11:09:42.639734 arkindex-base-worker-0.3.3rc3/arkindex_base_worker.egg-info/
--rw-r--r--   0 root         (0) root         (0)      248 2023-04-28 11:09:42.000000 arkindex-base-worker-0.3.3rc3/arkindex_base_worker.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1349 2023-04-28 11:09:42.000000 arkindex-base-worker-0.3.3rc3/arkindex_base_worker.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 11:09:42.000000 arkindex-base-worker-0.3.3rc3/arkindex_base_worker.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      318 2023-04-28 11:09:42.000000 arkindex-base-worker-0.3.3rc3/arkindex_base_worker.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-28 11:09:42.000000 arkindex-base-worker-0.3.3rc3/arkindex_base_worker.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 11:09:42.639734 arkindex-base-worker-0.3.3rc3/arkindex_worker/
--rw-rw-rw-   0 root         (0) root         (0)      186 2023-04-28 10:09:46.000000 arkindex-base-worker-0.3.3rc3/arkindex_worker/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9882 2023-04-28 10:27:51.000000 arkindex-base-worker-0.3.3rc3/arkindex_worker/cache.py
--rw-rw-rw-   0 root         (0) root         (0)    15338 2023-04-28 10:09:46.000000 arkindex-base-worker-0.3.3rc3/arkindex_worker/git.py
--rw-rw-rw-   0 root         (0) root         (0)    13466 2023-04-28 10:09:46.000000 arkindex-base-worker-0.3.3rc3/arkindex_worker/image.py
--rw-rw-rw-   0 root         (0) root         (0)     9619 2023-04-28 10:09:46.000000 arkindex-base-worker-0.3.3rc3/arkindex_worker/models.py
--rw-rw-rw-   0 root         (0) root         (0)     8012 2023-04-28 10:09:46.000000 arkindex-base-worker-0.3.3rc3/arkindex_worker/reporting.py
--rw-rw-rw-   0 root         (0) root         (0)     6926 2023-04-28 11:06:20.000000 arkindex-base-worker-0.3.3rc3/arkindex_worker/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 11:09:42.639734 arkindex-base-worker-0.3.3rc3/arkindex_worker/worker/
--rw-rw-rw-   0 root         (0) root         (0)    11662 2023-04-28 10:09:46.000000 arkindex-base-worker-0.3.3rc3/arkindex_worker/worker/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    16983 2023-04-28 10:27:51.000000 arkindex-base-worker-0.3.3rc3/arkindex_worker/worker/base.py
--rw-rw-rw-   0 root         (0) root         (0)    10935 2023-04-28 10:09:46.000000 arkindex-base-worker-0.3.3rc3/arkindex_worker/worker/classification.py
--rw-rw-rw-   0 root         (0) root         (0)    19034 2023-04-28 10:09:46.000000 arkindex-base-worker-0.3.3rc3/arkindex_worker/worker/element.py
--rw-rw-rw-   0 root         (0) root         (0)    14657 2023-04-28 10:09:46.000000 arkindex-base-worker-0.3.3rc3/arkindex_worker/worker/entity.py
--rw-rw-rw-   0 root         (0) root         (0)     6657 2023-04-28 10:09:46.000000 arkindex-base-worker-0.3.3rc3/arkindex_worker/worker/metadata.py
--rw-rw-rw-   0 root         (0) root         (0)    10211 2023-04-28 11:06:20.000000 arkindex-base-worker-0.3.3rc3/arkindex_worker/worker/training.py
--rw-rw-rw-   0 root         (0) root         (0)    19105 2023-04-28 10:09:46.000000 arkindex-base-worker-0.3.3rc3/arkindex_worker/worker/transcription.py
--rw-rw-rw-   0 root         (0) root         (0)     1460 2023-04-28 10:09:46.000000 arkindex-base-worker-0.3.3rc3/arkindex_worker/worker/version.py
--rw-rw-rw-   0 root         (0) root         (0)      110 2023-04-28 11:09:42.643734 arkindex-base-worker-0.3.3rc3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      768 2023-04-28 10:09:46.000000 arkindex-base-worker-0.3.3rc3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 11:09:42.639734 arkindex-base-worker-0.3.3rc3/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-28 10:09:46.000000 arkindex-base-worker-0.3.3rc3/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    17541 2023-04-28 10:09:46.000000 arkindex-base-worker-0.3.3rc3/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)    22358 2023-04-28 10:27:51.000000 arkindex-base-worker-0.3.3rc3/tests/test_base_worker.py
--rw-rw-rw-   0 root         (0) root         (0)     8705 2023-04-28 10:09:46.000000 arkindex-base-worker-0.3.3rc3/tests/test_cache.py
--rw-rw-rw-   0 root         (0) root         (0)    12961 2023-04-28 10:09:46.000000 arkindex-base-worker-0.3.3rc3/tests/test_element.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 11:09:42.643734 arkindex-base-worker-0.3.3rc3/tests/test_elements_worker/
--rw-rw-rw-   0 root         (0) root         (0)      203 2023-04-28 10:09:46.000000 arkindex-base-worker-0.3.3rc3/tests/test_elements_worker/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    32744 2023-04-28 10:09:46.000000 arkindex-base-worker-0.3.3rc3/tests/test_elements_worker/test_classifications.py
--rw-rw-rw-   0 root         (0) root         (0)     2751 2023-04-28 10:09:46.000000 arkindex-base-worker-0.3.3rc3/tests/test_elements_worker/test_cli.py
--rw-rw-rw-   0 root         (0) root         (0)    52786 2023-04-28 10:09:46.000000 arkindex-base-worker-0.3.3rc3/tests/test_elements_worker/test_elements.py
--rw-rw-rw-   0 root         (0) root         (0)    36695 2023-04-28 10:09:46.000000 arkindex-base-worker-0.3.3rc3/tests/test_elements_worker/test_entities.py
--rw-rw-rw-   0 root         (0) root         (0)    18023 2023-04-28 10:09:46.000000 arkindex-base-worker-0.3.3rc3/tests/test_elements_worker/test_metadata.py
--rw-rw-rw-   0 root         (0) root         (0)     8292 2023-04-28 10:09:46.000000 arkindex-base-worker-0.3.3rc3/tests/test_elements_worker/test_training.py
--rw-rw-rw-   0 root         (0) root         (0)    69404 2023-04-28 10:09:46.000000 arkindex-base-worker-0.3.3rc3/tests/test_elements_worker/test_transcriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    10239 2023-04-28 10:09:46.000000 arkindex-base-worker-0.3.3rc3/tests/test_elements_worker/test_worker.py
--rw-rw-rw-   0 root         (0) root         (0)    14944 2023-04-28 10:09:46.000000 arkindex-base-worker-0.3.3rc3/tests/test_git.py
--rw-rw-rw-   0 root         (0) root         (0)    14353 2023-04-28 10:09:46.000000 arkindex-base-worker-0.3.3rc3/tests/test_image.py
--rw-rw-rw-   0 root         (0) root         (0)     8402 2023-04-28 10:27:51.000000 arkindex-base-worker-0.3.3rc3/tests/test_merge.py
--rw-rw-rw-   0 root         (0) root         (0)     8802 2023-04-28 10:09:46.000000 arkindex-base-worker-0.3.3rc3/tests/test_reporting.py
--rw-rw-rw-   0 root         (0) root         (0)     1277 2023-04-28 10:09:46.000000 arkindex-base-worker-0.3.3rc3/tests/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 06:43:45.868299 arkindex-base-worker-0.3.3rc4/
+-rw-r--r--   0 root         (0) root         (0)      248 2023-05-25 06:43:45.868299 arkindex-base-worker-0.3.3rc4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      233 2023-05-25 06:40:01.000000 arkindex-base-worker-0.3.3rc4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 06:43:45.864299 arkindex-base-worker-0.3.3rc4/arkindex_base_worker.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      248 2023-05-25 06:43:45.000000 arkindex-base-worker-0.3.3rc4/arkindex_base_worker.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1349 2023-05-25 06:43:45.000000 arkindex-base-worker-0.3.3rc4/arkindex_base_worker.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 06:43:45.000000 arkindex-base-worker-0.3.3rc4/arkindex_base_worker.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      321 2023-05-25 06:43:45.000000 arkindex-base-worker-0.3.3rc4/arkindex_base_worker.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-25 06:43:45.000000 arkindex-base-worker-0.3.3rc4/arkindex_base_worker.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 06:43:45.864299 arkindex-base-worker-0.3.3rc4/arkindex_worker/
+-rw-rw-rw-   0 root         (0) root         (0)      186 2023-05-25 06:40:01.000000 arkindex-base-worker-0.3.3rc4/arkindex_worker/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9882 2023-05-25 06:40:01.000000 arkindex-base-worker-0.3.3rc4/arkindex_worker/cache.py
+-rw-rw-rw-   0 root         (0) root         (0)    15338 2023-05-25 06:40:01.000000 arkindex-base-worker-0.3.3rc4/arkindex_worker/git.py
+-rw-rw-rw-   0 root         (0) root         (0)    13466 2023-05-25 06:40:01.000000 arkindex-base-worker-0.3.3rc4/arkindex_worker/image.py
+-rw-rw-rw-   0 root         (0) root         (0)     9619 2023-05-25 06:40:01.000000 arkindex-base-worker-0.3.3rc4/arkindex_worker/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     8012 2023-05-25 06:40:01.000000 arkindex-base-worker-0.3.3rc4/arkindex_worker/reporting.py
+-rw-rw-rw-   0 root         (0) root         (0)     6926 2023-05-25 06:40:01.000000 arkindex-base-worker-0.3.3rc4/arkindex_worker/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 06:43:45.864299 arkindex-base-worker-0.3.3rc4/arkindex_worker/worker/
+-rw-rw-rw-   0 root         (0) root         (0)    11662 2023-05-25 06:40:01.000000 arkindex-base-worker-0.3.3rc4/arkindex_worker/worker/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    18850 2023-05-25 06:40:01.000000 arkindex-base-worker-0.3.3rc4/arkindex_worker/worker/base.py
+-rw-rw-rw-   0 root         (0) root         (0)    10935 2023-05-25 06:40:01.000000 arkindex-base-worker-0.3.3rc4/arkindex_worker/worker/classification.py
+-rw-rw-rw-   0 root         (0) root         (0)    19034 2023-05-25 06:40:01.000000 arkindex-base-worker-0.3.3rc4/arkindex_worker/worker/element.py
+-rw-rw-rw-   0 root         (0) root         (0)    14657 2023-05-25 06:40:01.000000 arkindex-base-worker-0.3.3rc4/arkindex_worker/worker/entity.py
+-rw-rw-rw-   0 root         (0) root         (0)     6657 2023-05-25 06:40:01.000000 arkindex-base-worker-0.3.3rc4/arkindex_worker/worker/metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)    10211 2023-05-25 06:40:01.000000 arkindex-base-worker-0.3.3rc4/arkindex_worker/worker/training.py
+-rw-rw-rw-   0 root         (0) root         (0)    19105 2023-05-25 06:40:01.000000 arkindex-base-worker-0.3.3rc4/arkindex_worker/worker/transcription.py
+-rw-rw-rw-   0 root         (0) root         (0)     1460 2023-05-25 06:40:01.000000 arkindex-base-worker-0.3.3rc4/arkindex_worker/worker/version.py
+-rw-rw-rw-   0 root         (0) root         (0)      110 2023-05-25 06:43:45.868299 arkindex-base-worker-0.3.3rc4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      768 2023-05-25 06:40:01.000000 arkindex-base-worker-0.3.3rc4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 06:43:45.868299 arkindex-base-worker-0.3.3rc4/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-25 06:40:01.000000 arkindex-base-worker-0.3.3rc4/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    17541 2023-05-25 06:40:01.000000 arkindex-base-worker-0.3.3rc4/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)    24869 2023-05-25 06:40:01.000000 arkindex-base-worker-0.3.3rc4/tests/test_base_worker.py
+-rw-rw-rw-   0 root         (0) root         (0)     8705 2023-05-25 06:40:01.000000 arkindex-base-worker-0.3.3rc4/tests/test_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)    12961 2023-05-25 06:40:01.000000 arkindex-base-worker-0.3.3rc4/tests/test_element.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 06:43:45.868299 arkindex-base-worker-0.3.3rc4/tests/test_elements_worker/
+-rw-rw-rw-   0 root         (0) root         (0)      203 2023-05-25 06:40:01.000000 arkindex-base-worker-0.3.3rc4/tests/test_elements_worker/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    32744 2023-05-25 06:40:01.000000 arkindex-base-worker-0.3.3rc4/tests/test_elements_worker/test_classifications.py
+-rw-rw-rw-   0 root         (0) root         (0)     2751 2023-05-25 06:40:01.000000 arkindex-base-worker-0.3.3rc4/tests/test_elements_worker/test_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)    52786 2023-05-25 06:40:01.000000 arkindex-base-worker-0.3.3rc4/tests/test_elements_worker/test_elements.py
+-rw-rw-rw-   0 root         (0) root         (0)    36695 2023-05-25 06:40:01.000000 arkindex-base-worker-0.3.3rc4/tests/test_elements_worker/test_entities.py
+-rw-rw-rw-   0 root         (0) root         (0)    18023 2023-05-25 06:40:01.000000 arkindex-base-worker-0.3.3rc4/tests/test_elements_worker/test_metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)     8292 2023-05-25 06:40:01.000000 arkindex-base-worker-0.3.3rc4/tests/test_elements_worker/test_training.py
+-rw-rw-rw-   0 root         (0) root         (0)    69404 2023-05-25 06:40:01.000000 arkindex-base-worker-0.3.3rc4/tests/test_elements_worker/test_transcriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    17450 2023-05-25 06:40:01.000000 arkindex-base-worker-0.3.3rc4/tests/test_elements_worker/test_worker.py
+-rw-rw-rw-   0 root         (0) root         (0)    14944 2023-05-25 06:40:01.000000 arkindex-base-worker-0.3.3rc4/tests/test_git.py
+-rw-rw-rw-   0 root         (0) root         (0)    14353 2023-05-25 06:40:01.000000 arkindex-base-worker-0.3.3rc4/tests/test_image.py
+-rw-rw-rw-   0 root         (0) root         (0)     8402 2023-05-25 06:40:01.000000 arkindex-base-worker-0.3.3rc4/tests/test_merge.py
+-rw-rw-rw-   0 root         (0) root         (0)     8802 2023-05-25 06:40:01.000000 arkindex-base-worker-0.3.3rc4/tests/test_reporting.py
+-rw-rw-rw-   0 root         (0) root         (0)     1260 2023-05-25 06:40:01.000000 arkindex-base-worker-0.3.3rc4/tests/test_utils.py
```

### Comparing `arkindex-base-worker-0.3.3rc3/arkindex_base_worker.egg-info/SOURCES.txt` & `arkindex-base-worker-0.3.3rc4/arkindex_base_worker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.3rc3/arkindex_worker/cache.py` & `arkindex-base-worker-0.3.3rc4/arkindex_worker/cache.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.3rc3/arkindex_worker/git.py` & `arkindex-base-worker-0.3.3rc4/arkindex_worker/git.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.3rc3/arkindex_worker/image.py` & `arkindex-base-worker-0.3.3rc4/arkindex_worker/image.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.3rc3/arkindex_worker/models.py` & `arkindex-base-worker-0.3.3rc4/arkindex_worker/models.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.3rc3/arkindex_worker/reporting.py` & `arkindex-base-worker-0.3.3rc4/arkindex_worker/reporting.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.3rc3/arkindex_worker/utils.py` & `arkindex-base-worker-0.3.3rc4/arkindex_worker/utils.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.3rc3/arkindex_worker/worker/__init__.py` & `arkindex-base-worker-0.3.3rc4/arkindex_worker/worker/__init__.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.3rc3/arkindex_worker/worker/base.py` & `arkindex-base-worker-0.3.3rc4/arkindex_worker/worker/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # -*- coding: utf-8 -*-
 """
 The base class for all Arkindex workers.
 """
-
 import argparse
 import json
 import logging
 import os
+import shutil
 from pathlib import Path
+from tempfile import mkdtemp
 from typing import List, Optional
 
 import gnupg
 import yaml
 from apistar.exceptions import ErrorResponse
 from tenacity import (
     before_sleep_log,
@@ -26,14 +27,15 @@
 from arkindex_worker.cache import (
     check_version,
     create_tables,
     create_version_table,
     init_cache_db,
     merge_parents_cache,
 )
+from arkindex_worker.utils import close_delete_file, extract_tar_zst_archive
 
 
 def _is_500_error(exc: Exception) -> bool:
     """
     Check if an Arkindex API error has a HTTP 5xx error code.
     Used to retry most API calls in [BaseWorker][arkindex_worker.worker.base.BaseWorker].
     :param exc: Exception to check
@@ -142,16 +144,16 @@
         self.user_configuration = {}
         self.model_configuration = {}
         self.support_cache = support_cache
         # use_cache will be updated in configure_cache() if the cache is supported and if
         # there is at least one available sqlite database either given or in the parent tasks
         self.use_cache = False
 
-        # task_parents will be updated in configure_cache() if the cache is supported and if
-        # there is at least one available sqlite database either given or in the parent tasks
+        # task_parents will be updated in configure_cache() if the cache is supported,
+        # if the task ID is set and if no database is passed as argument
         self.task_parents = []
 
         # Define API Client
         self.setup_api_client()
 
     @property
     def is_read_only(self) -> bool:
@@ -236,43 +238,43 @@
         self.worker_version_id = worker_version["id"]
 
         self.worker_details = worker_version["worker"]
         logger.info(
             f"Loaded worker {self.worker_details['name']} revision {worker_version['revision']['hash'][0:7]} from API"
         )
 
+        # Load model version configuration when available
+        model_version = worker_run.get("model_version")
+        if model_version and model_version.get("configuration"):
+            logger.info("Loaded model version configuration from WorkerRun")
+            self.model_configuration.update(model_version.get("configuration"))
+
+            # Set model_version ID as worker attribute
+            self.model_version_id = model_version.get("id")
+
         # Retrieve initial configuration from API
         self.config = worker_version["configuration"].get("configuration", {})
         if "user_configuration" in worker_version["configuration"]:
             # Add default values (if set) to user_configuration
             for key, value in worker_version["configuration"][
                 "user_configuration"
             ].items():
-                if "default" in value:
+                if "default" in value and key not in self.model_configuration:
                     self.user_configuration[key] = value["default"]
 
         # Load all required secrets
         required_secrets = worker_version["configuration"].get("secrets", [])
         self.secrets = {name: self.load_secret(Path(name)) for name in required_secrets}
 
         # Load worker run configuration when available
         worker_configuration = worker_run.get("configuration")
         if worker_configuration and worker_configuration.get("configuration"):
             logger.info("Loaded user configuration from WorkerRun")
             self.user_configuration.update(worker_configuration.get("configuration"))
 
-        # Load model version configuration when available
-        model_version = worker_run.get("model_version")
-        if model_version and model_version.get("configuration"):
-            logger.info("Loaded model version configuration from WorkerRun")
-            self.model_configuration.update(model_version.get("configuration"))
-
-            # Set model_version ID as worker attribute
-            self.model_version_id = model_version.get("id")
-
         # if debug mode is set to true activate debug mode in logger
         if self.user_configuration.get("debug"):
             logger.setLevel(logging.DEBUG)
             logger.debug("Debug output enabled")
 
     def configure_cache(self):
         """
@@ -361,24 +363,29 @@
 
         # By default give raw secret payload
         return secret
 
     def find_model_directory(self) -> Path:
         """
         Find the local path to the model. This supports two modes:
-        - the worker runs in ponos, the model is available at `/data/current`
+        - the worker runs in ponos, the model is available at `/data/extra_files` (first try) or `/data/current`.
         - the worker runs locally, the developer may specify it using either
            - the `model_dir` configuration parameter
            - the `--model-dir` CLI parameter
 
         :return: Path to the model on disk
         """
         if self.task_id:
             # When running in production with ponos, the agent
-            # downloads the model and set it in the current task work dir
+            # downloads the model and set it either in
+            # - `/data/extra_files`
+            # - the current task work dir
+            extra_dir = self.task_data_dir / "extra_files"
+            if extra_dir.exists():
+                return extra_dir
             return self.work_dir
         else:
             model_dir = self.config.get("model_dir", self.args.model_dir)
             if model_dir is None:
                 raise ModelNotFoundError(
                     "No path to the model was provided. "
                     "Please provide model_dir either through configuration "
@@ -390,16 +397,16 @@
                     f"The path {model_dir} does not link to any directory"
                 )
             return model_dir
 
     def find_parents_file_paths(self, filename: Path) -> List[Path]:
         """
         Find the paths of a specific file from the parent tasks.
-        Only works if the task_parents attributes is updated, so if the cache is supported and
-        if there is at least one available sqlite database either given or in the parent tasks
+        Only works if the task_parents attributes is updated, so if the cache is supported,
+        if the task ID is set and if no database is passed as argument
 
         :param filename: Name of the file to find
         :return: Paths to the parent files
         """
         # Handle possible chunk in parent task name
         # This is needed to support the init_elements databases
         filenames = [
@@ -418,14 +425,49 @@
                     self.task_data_dir / parent_id / name
                     for parent_id in self.task_parents
                     for name in filenames
                 ],
             )
         )
 
+    def extract_parent_archives(self, archive_name: Path, dest: Path) -> None:
+        """
+        Find and extract the paths from a specific file from the parent tasks.
+        Only works if the task_parents attributes is updated, so if the cache is supported,
+        if the task ID is set and if no database is passed as argument
+
+        :param archive_name: Name of the file to find
+        :param dest: Folder to store the extracted files
+        """
+        base_extracted_path = Path(mkdtemp(suffix="-extracted-data"))
+        file_paths = self.find_parents_file_paths(archive_name)
+
+        # Uncompress and extract the archive
+        for file_path in file_paths:
+            archive_fd, archive_path = extract_tar_zst_archive(
+                file_path, base_extracted_path
+            )
+            # Remove the tar archive
+            close_delete_file(archive_fd, archive_path)
+
+            # Move all files in the dest folder
+            for tmp_extracted_path in base_extracted_path.rglob("*"):
+                if not tmp_extracted_path.is_file():
+                    continue
+
+                extracted_file = Path(
+                    str(tmp_extracted_path).replace(str(base_extracted_path), str(dest))
+                )
+                extracted_file.parent.mkdir(parents=True, exist_ok=True)
+                # Use shutil to avoid errors when the files are not on the same filesystem
+                shutil.move(tmp_extracted_path, extracted_file)
+
+            # Clean up
+            shutil.rmtree(base_extracted_path)
+
     @retry(
         retry=retry_if_exception(_is_500_error),
         wait=wait_exponential(multiplier=2, min=3),
         reraise=True,
         stop=stop_after_attempt(5),
         before_sleep=before_sleep_log(logger, logging.INFO),
     )
```

### Comparing `arkindex-base-worker-0.3.3rc3/arkindex_worker/worker/classification.py` & `arkindex-base-worker-0.3.3rc4/arkindex_worker/worker/classification.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.3rc3/arkindex_worker/worker/element.py` & `arkindex-base-worker-0.3.3rc4/arkindex_worker/worker/element.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.3rc3/arkindex_worker/worker/entity.py` & `arkindex-base-worker-0.3.3rc4/arkindex_worker/worker/entity.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.3rc3/arkindex_worker/worker/metadata.py` & `arkindex-base-worker-0.3.3rc4/arkindex_worker/worker/metadata.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.3rc3/arkindex_worker/worker/training.py` & `arkindex-base-worker-0.3.3rc4/arkindex_worker/worker/training.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.3rc3/arkindex_worker/worker/transcription.py` & `arkindex-base-worker-0.3.3rc4/arkindex_worker/worker/transcription.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.3rc3/arkindex_worker/worker/version.py` & `arkindex-base-worker-0.3.3rc4/arkindex_worker/worker/version.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.3rc3/setup.py` & `arkindex-base-worker-0.3.3rc4/setup.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.3rc3/tests/conftest.py` & `arkindex-base-worker-0.3.3rc4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.3rc3/tests/test_base_worker.py` & `arkindex-base-worker-0.3.3rc4/tests/test_base_worker.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 # -*- coding: utf-8 -*-
 import json
 import logging
 import sys
+import uuid
 from pathlib import Path
 
 import gnupg
 import pytest
 
 from arkindex.mock import MockApiClient
 from arkindex_worker import logger
 from arkindex_worker.worker import BaseWorker
 from arkindex_worker.worker.base import ModelNotFoundError
+from tests.conftest import FIXTURES_DIR
 
 
 def test_init_default_local_share(monkeypatch):
     worker = BaseWorker()
 
     assert worker.work_dir == Path("~/.local/share/arkindex").expanduser()
 
@@ -596,21 +598,31 @@
     assert worker.load_secret(Path("testLocal")) == "this is a local secret value"
 
     # The remote api is checked first
     assert len(worker.api_client.history) == 1
     assert worker.api_client.history[0].operation == "RetrieveSecret"
 
 
-def test_find_model_directory_ponos(monkeypatch):
+def test_find_model_directory_ponos_no_extra_files(monkeypatch):
     monkeypatch.setenv("PONOS_TASK", "my_task")
     monkeypatch.setenv("PONOS_DATA", "/data")
     worker = BaseWorker()
     assert worker.find_model_directory() == Path("/data/current")
 
 
+def test_find_model_directory_ponos_with_extra_files(monkeypatch):
+    monkeypatch.setenv("PONOS_TASK", "my_task")
+    monkeypatch.setenv("PONOS_DATA", "/data")
+    # Make the `extra_files` folder exist
+    monkeypatch.setattr("pathlib.Path.exists", lambda x: True)
+
+    worker = BaseWorker()
+    assert worker.find_model_directory() == Path("/data/extra_files")
+
+
 def test_find_model_directory_from_cli(monkeypatch):
     monkeypatch.setattr(sys, "argv", ["worker", "--model-dir", "models"])
     monkeypatch.setattr("pathlib.Path.exists", lambda x: True)
     worker = BaseWorker()
     worker.args = worker.parser.parse_args()
     worker.config = {}
     assert worker.find_model_directory() == Path("models")
@@ -674,7 +686,56 @@
     mock_base_worker_with_cache.configure()
     mock_base_worker_with_cache.configure_cache()
 
     assert mock_base_worker_with_cache.find_parents_file_paths(filename) == [
         tmp_path / "first" / filename,
         tmp_path / "third" / filename,
     ]
+
+
+def test_extract_parent_archives(tmp_path):
+    worker = BaseWorker()
+
+    # Mock task attributes
+    worker.task_parents = [
+        "invalid_id",
+        "first_parent",
+        str(uuid.uuid4()),
+        "second_parent",
+    ]
+    worker.task_data_dir = FIXTURES_DIR / "extract_parent_archives"
+
+    worker.extract_parent_archives("arkindex_data.zstd", tmp_path)
+
+    extracted_files = [
+        # Test
+        tmp_path / "test/images/f2649ce7-333e-44d2-ae73-387f18aad1f6.png",
+        tmp_path / "test/labels/f2649ce7-333e-44d2-ae73-387f18aad1f6.png",
+        tmp_path / "test/labels_json/f2649ce7-333e-44d2-ae73-387f18aad1f6.json",
+        # Train
+        tmp_path / "train/images/98115546-df07-448c-a2f0-34aa24789b77.png",
+        tmp_path / "train/images/ebeaa451-9287-4df7-9c40-07eb25cadb78.png",
+        tmp_path / "train/labels/98115546-df07-448c-a2f0-34aa24789b77.png",
+        tmp_path / "train/labels/ebeaa451-9287-4df7-9c40-07eb25cadb78.png",
+        tmp_path / "train/labels_json/98115546-df07-448c-a2f0-34aa24789b77.json",
+        tmp_path / "train/labels_json/ebeaa451-9287-4df7-9c40-07eb25cadb78.json",
+        # Val
+        tmp_path / "val/images/2987176d-4338-40f2-90d9-6d2cb4fd4a00.png",
+        tmp_path / "val/images/e3f91312-9201-45b7-9c32-e04a97ff1334.png",
+        tmp_path / "val/labels/2987176d-4338-40f2-90d9-6d2cb4fd4a00.png",
+        tmp_path / "val/labels/e3f91312-9201-45b7-9c32-e04a97ff1334.png",
+        tmp_path / "val/labels_json/2987176d-4338-40f2-90d9-6d2cb4fd4a00.json",
+        tmp_path / "val/labels_json/e3f91312-9201-45b7-9c32-e04a97ff1334.json",
+    ]
+    assert (
+        sorted([path for path in tmp_path.rglob("*") if path.is_file()])
+        == extracted_files
+    )
+
+    for extracted_file in extracted_files:
+        expected_file = (
+            FIXTURES_DIR
+            / "extract_parent_archives"
+            / str(extracted_file).replace(str(tmp_path), "expected")
+        )
+        mode = "rb" if extracted_file.suffix == ".png" else "r"
+        assert extracted_file.open(mode).read() == expected_file.open(mode).read()
```

### Comparing `arkindex-base-worker-0.3.3rc3/tests/test_cache.py` & `arkindex-base-worker-0.3.3rc4/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.3rc3/tests/test_element.py` & `arkindex-base-worker-0.3.3rc4/tests/test_element.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.3rc3/tests/test_elements_worker/test_classifications.py` & `arkindex-base-worker-0.3.3rc4/tests/test_elements_worker/test_classifications.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.3rc3/tests/test_elements_worker/test_cli.py` & `arkindex-base-worker-0.3.3rc4/tests/test_elements_worker/test_cli.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.3rc3/tests/test_elements_worker/test_elements.py` & `arkindex-base-worker-0.3.3rc4/tests/test_elements_worker/test_elements.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.3rc3/tests/test_elements_worker/test_entities.py` & `arkindex-base-worker-0.3.3rc4/tests/test_elements_worker/test_entities.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.3rc3/tests/test_elements_worker/test_metadata.py` & `arkindex-base-worker-0.3.3rc4/tests/test_elements_worker/test_metadata.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.3rc3/tests/test_elements_worker/test_training.py` & `arkindex-base-worker-0.3.3rc4/tests/test_elements_worker/test_training.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.3rc3/tests/test_elements_worker/test_transcriptions.py` & `arkindex-base-worker-0.3.3rc4/tests/test_elements_worker/test_transcriptions.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.3rc3/tests/test_git.py` & `arkindex-base-worker-0.3.3rc4/tests/test_git.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.3rc3/tests/test_image.py` & `arkindex-base-worker-0.3.3rc4/tests/test_image.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.3rc3/tests/test_merge.py` & `arkindex-base-worker-0.3.3rc4/tests/test_merge.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.3rc3/tests/test_reporting.py` & `arkindex-base-worker-0.3.3rc4/tests/test_reporting.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.3rc3/tests/test_utils.py` & `arkindex-base-worker-0.3.3rc4/tests/test_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from arkindex_worker.utils import close_delete_file, extract_tar_zst_archive
 
 FIXTURES = Path(__file__).absolute().parent / "data"
 ARCHIVE = FIXTURES / "archive.tar.zst"
 
 
-def test_extract_tar_zst_archive(mocker, tmp_path):
+def test_extract_tar_zst_archive(tmp_path):
     destination = tmp_path / "destination"
     _, archive_path = extract_tar_zst_archive(ARCHIVE, destination)
 
     assert archive_path.is_file()
     assert archive_path.suffix == ".tar"
     assert sorted(list(destination.rglob("*"))) == [
         destination / "archive.tar.zst",
@@ -24,13 +24,13 @@
         destination / "rotated_mirrored_image.jpg",
         destination / "test_image.jpg",
         destination / "tiled_image.jpg",
         destination / "ufcn_line_historical_worker_version.json",
     ]
 
 
-def test_delete_tar_archive(mocker, tmp_path):
+def test_close_delete_file(tmp_path):
     destination = tmp_path / "destination"
     archive_fd, archive_path = extract_tar_zst_archive(ARCHIVE, destination)
     close_delete_file(archive_fd, archive_path)
 
     assert not archive_path.exists()
```

