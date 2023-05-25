# Comparing `tmp/twinlab-1.1.2.tar.gz` & `tmp/twinlab-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twinlab-1.1.2.tar", max compression
+gzip compressed data, was "twinlab-1.1.3.tar", max compression
```

## Comparing `twinlab-1.1.2.tar` & `twinlab-1.1.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1031 2023-05-18 13:40:02.600816 twinlab-1.1.2/LICENSE
--rw-r--r--   0        0        0     2011 2023-05-25 12:10:23.882093 twinlab-1.1.2/README.md
--rw-r--r--   0        0        0      932 2023-05-25 12:10:04.799611 twinlab-1.1.2/pyproject.toml
--rw-r--r--   0        0        0      529 2023-05-18 13:40:02.609012 twinlab-1.1.2/twinlab/__init__.py
--rw-r--r--   0        0        0     8495 2023-05-25 12:10:04.800319 twinlab-1.1.2/twinlab/client.py
--rw-r--r--   0        0        0      505 2023-05-11 09:23:10.154006 twinlab-1.1.2/twinlab/plotting.py
--rw-r--r--   0        0        0      702 2023-05-25 12:10:04.800688 twinlab-1.1.2/twinlab/settings.py
--rw-r--r--   0        0        0     6198 2023-05-25 12:10:04.802039 twinlab-1.1.2/twinlab/utils.py
--rw-r--r--   0        0        0     2962 1970-01-01 00:00:00.000000 twinlab-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1031 2023-05-18 13:40:02.600816 twinlab-1.1.3/LICENSE
+-rw-r--r--   0        0        0     2011 2023-05-25 13:37:52.705700 twinlab-1.1.3/README.md
+-rw-r--r--   0        0        0      932 2023-05-25 13:37:55.886193 twinlab-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0      529 2023-05-18 13:40:02.609012 twinlab-1.1.3/twinlab/__init__.py
+-rw-r--r--   0        0        0     8531 2023-05-25 13:37:55.886468 twinlab-1.1.3/twinlab/client.py
+-rw-r--r--   0        0        0      505 2023-05-11 09:23:10.154006 twinlab-1.1.3/twinlab/plotting.py
+-rw-r--r--   0        0        0      702 2023-05-25 12:10:04.800688 twinlab-1.1.3/twinlab/settings.py
+-rw-r--r--   0        0        0     6174 2023-05-25 13:37:55.886723 twinlab-1.1.3/twinlab/utils.py
+-rw-r--r--   0        0        0     2962 1970-01-01 00:00:00.000000 twinlab-1.1.3/PKG-INFO
```

### Comparing `twinlab-1.1.2/LICENSE` & `twinlab-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `twinlab-1.1.2/README.md` & `twinlab-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `twinlab-1.1.2/pyproject.toml` & `twinlab-1.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "twinlab"
-version = "1.1.2"
+version = "1.1.3"
 description = "Client interface for twinLab machine-learning in the cloud."
 license = "MIT"
 homepage = "https://www.digilab.co.uk/"
 repository = "https://github.com/digiLab-ai/twinLab-client"
 documentation = "https://digilab-ai.github.io/twinLab-client"
 authors = ["DigiLab Solutions Ltd. <info@digilab.co.uk>"]
 maintainers = [
```

### Comparing `twinlab-1.1.2/twinlab/__init__.py` & `twinlab-1.1.3/twinlab/__init__.py`

 * *Files identical despite different names*

### Comparing `twinlab-1.1.2/twinlab/client.py` & `twinlab-1.1.3/twinlab/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,16 +28,16 @@
     # Sort out dataset_name
     if dataset_name is None:
         if type(filepath_or_df) == str:
             dataset_name = filepath_or_df
         else:
             raise ValueError("Name must be specified if uploading dataframe")
     else:
-        if "/" in dataset_name:
-            raise ValueError("Dataset name cannot contain '/'")
+        if ("/" in dataset_name) or ("\\" in dataset_name):
+            raise ValueError("Dataset name cannot contain '/' or '\\'")
 
     # Get the upload URL
     headers = utils.construct_standard_headers(debug=debug)
     headers["X-Dataset"] = dataset_name
     lambda_url = utils.get_server_url(server) + "/generate_upload_url"
     r = requests.get(lambda_url, headers=headers)
     utils.check_response(r)
```

### Comparing `twinlab-1.1.2/twinlab/settings.py` & `twinlab-1.1.3/twinlab/settings.py`

 * *Files identical despite different names*

### Comparing `twinlab-1.1.2/twinlab/utils.py` & `twinlab-1.1.3/twinlab/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 # Standard imports
 import io
-import os
 import argparse
 import json
 from pprint import pprint
 
 # Third-party imports
 import requests
 import pandas as pd
@@ -98,15 +97,15 @@
     if server == "dev":
         url = TRAIN_CAMPAIGN_DEV_URL
     elif server == "stage":
         url = TRAIN_CAMPAIGN_STAGE_URL
     elif server == "cloud":
         url = TRAIN_CAMPAIGN_CLOUD_URL
     else:
-        url = os.path.join(get_server_url(server), "train_campaign")
+        url = get_server_url(server)+"/train_campaign"
     return url
 
 
 def coerce_params_dict(params: dict) -> dict:
     """
     Relabel parameters to be consistent with twinLab library
     """
```

### Comparing `twinlab-1.1.2/PKG-INFO` & `twinlab-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twinlab
-Version: 1.1.2
+Version: 1.1.3
 Summary: Client interface for twinLab machine-learning in the cloud.
 Home-page: https://www.digilab.co.uk/
 License: MIT
 Keywords: machine-learning,AI,cloud,twinLab,digiLab
 Author: DigiLab Solutions Ltd.
 Author-email: info@digilab.co.uk
 Maintainer: Alexander Mead
```

