# Comparing `tmp/twinlab-1.1.1.tar.gz` & `tmp/twinlab-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twinlab-1.1.1.tar", max compression
+gzip compressed data, was "twinlab-1.1.2.tar", max compression
```

## Comparing `twinlab-1.1.1.tar` & `twinlab-1.1.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1031 2023-05-18 13:40:02.600816 twinlab-1.1.1/LICENSE
--rw-r--r--   0        0        0     2115 2023-05-18 13:49:12.053818 twinlab-1.1.1/README.md
--rw-r--r--   0        0        0      932 2023-05-18 13:40:02.603772 twinlab-1.1.1/pyproject.toml
--rw-r--r--   0        0        0      529 2023-05-18 13:40:02.609012 twinlab-1.1.1/twinlab/__init__.py
--rw-r--r--   0        0        0     7858 2023-05-18 13:40:02.609191 twinlab-1.1.1/twinlab/client.py
--rw-r--r--   0        0        0      505 2023-05-11 09:23:10.154006 twinlab-1.1.1/twinlab/plotting.py
--rw-r--r--   0        0        0      664 2023-05-18 13:40:02.609342 twinlab-1.1.1/twinlab/settings.py
--rw-r--r--   0        0        0     5762 2023-05-18 15:23:53.182090 twinlab-1.1.1/twinlab/utils.py
--rw-r--r--   0        0        0     3066 1970-01-01 00:00:00.000000 twinlab-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1031 2023-05-18 13:40:02.600816 twinlab-1.1.2/LICENSE
+-rw-r--r--   0        0        0     2011 2023-05-25 12:10:23.882093 twinlab-1.1.2/README.md
+-rw-r--r--   0        0        0      932 2023-05-25 12:10:04.799611 twinlab-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0      529 2023-05-18 13:40:02.609012 twinlab-1.1.2/twinlab/__init__.py
+-rw-r--r--   0        0        0     8495 2023-05-25 12:10:04.800319 twinlab-1.1.2/twinlab/client.py
+-rw-r--r--   0        0        0      505 2023-05-11 09:23:10.154006 twinlab-1.1.2/twinlab/plotting.py
+-rw-r--r--   0        0        0      702 2023-05-25 12:10:04.800688 twinlab-1.1.2/twinlab/settings.py
+-rw-r--r--   0        0        0     6198 2023-05-25 12:10:04.802039 twinlab-1.1.2/twinlab/utils.py
+-rw-r--r--   0        0        0     2962 1970-01-01 00:00:00.000000 twinlab-1.1.2/PKG-INFO
```

### Comparing `twinlab-1.1.1/LICENSE` & `twinlab-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `twinlab-1.1.1/README.md` & `twinlab-1.1.2/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -12,54 +12,49 @@
 ## Installation
 
 Most users should use `pip`
 ```shell
 pip install twinlab
 ```
 
-If you want to modify the client-side code, or have a local installation for some reason
+If you want to modify the client-side code, or have a local installation, you will need to have `git`, `poetry`, and a `python` version of `3.9` or higher installed. Then you can do:
 ```shell
 git clone https://github.com/digiLab-ai/twinLab-client.git
 cd twinlab-client
 poetry install
 ```
 
 ## Environment setup
 
 You will need a `.env` file in your project directory that looks like the `.env.example` file in this repository
 ```shell
 cp .env.example .env
 ```
-and fill in your twinLab user details.
+and fill in your `twinLab` user details.
 
 ## Commands
 
 Testing:
 
 ```shell
-poetry run python scripts/test.py cloud 
+poetry run python scripts/test.py
 ```
 where `test.py` can be replaced with any of the scripts in the `script` directory.
 
-You need to have a local server for the (private) `twinlab-cloud` repository running for local testing. But local testing can then be run with
-```shell
-poetry run python scripts/test.py local
-```
-
 ## Example
 
 Here we create some mock data (which has a quadratic relationship between `X` and `y`) and use `twinLab` to create a surrogate model with quantified uncertainty.
 ```python
 # Import libraries
 import twinlab as tl
 import pandas as pd
 
-# Create a dataset and upload to twinLab cloud
+# Create a dataset and upload to the twinLab cloud
 df = pd.DataFrame({'X': [1, 2, 3, 4], 'y': [1, 4, 9, 16]})
-tl.upload_dataset('test.csv', df)
+tl.upload_dataset(df, 'test.csv')
 
 # Train a machine-learning model for the data
 params = {
     'filename': 'test.csv',
     'inputs': ['X'],
     'outputs': ['y'],
 }
```

### Comparing `twinlab-1.1.1/pyproject.toml` & `twinlab-1.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "twinlab"
-version = "1.1.1"
+version = "1.1.2"
 description = "Client interface for twinLab machine-learning in the cloud."
 license = "MIT"
 homepage = "https://www.digilab.co.uk/"
 repository = "https://github.com/digiLab-ai/twinLab-client"
 documentation = "https://digilab-ai.github.io/twinLab-client"
 authors = ["DigiLab Solutions Ltd. <info@digilab.co.uk>"]
 maintainers = [
```

### Comparing `twinlab-1.1.1/twinlab/__init__.py` & `twinlab-1.1.2/twinlab/__init__.py`

 * *Files identical despite different names*

### Comparing `twinlab-1.1.1/twinlab/client.py` & `twinlab-1.1.2/twinlab/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,51 +1,67 @@
 # Standard imports
 import io
 import json
 from pprint import pprint
+from typing import Union
 
 # Third-party imports
 import requests
 import pandas as pd
 
 # Project imports
 from . import utils
 
 ### Dataset functions ###
 
 
-def upload_dataset(dataset_filepath: str, df=None, server="cloud", verbose=False, debug=False) -> None:
+def upload_dataset(filepath_or_df: Union[str, pd.DataFrame], dataset_name=None, server="cloud", verbose=False, debug=False) -> None:
     """
     Upload a dataset to the cloud so that it can be queried and used for training
     params:
-        dataset_filepath: str; location of csv dataset on local machine
-        dt: None or pd.DataFrame; if None, then dataset_filepath is used to load the dataframe
+        filepath_or_df: str; location of csv dataset on local machine or pandas dataframe
+        dataset_name: str; name of dataset on S3 (same as the uploaded file name if file)
         server: str; either "cloud" or "local"
         verbose: bool
         debug: bool
     """
+
+    # Sort out dataset_name
+    if dataset_name is None:
+        if type(filepath_or_df) == str:
+            dataset_name = filepath_or_df
+        else:
+            raise ValueError("Name must be specified if uploading dataframe")
+    else:
+        if "/" in dataset_name:
+            raise ValueError("Dataset name cannot contain '/'")
+
+    # Get the upload URL
     headers = utils.construct_standard_headers(debug=debug)
-    headers["X-Dataset"] = dataset_filepath
+    headers["X-Dataset"] = dataset_name
     lambda_url = utils.get_server_url(server) + "/generate_upload_url"
     r = requests.get(lambda_url, headers=headers)
     utils.check_response(r)
+
+    # Upload the file
     if verbose:
         utils.print_response_message(r)
     upload_url = r.json()["url"]
-    if df is None:
+    if type(filepath_or_df) is str:
+        filepath = filepath_or_df
         utils.upload_file_to_presigned_url(
-            dataset_filepath, upload_url, verbose=verbose)
+            filepath, upload_url, verbose=verbose)
     else:
-        dataset_name = dataset_filepath
-        if "/" in dataset_name:
-            raise ValueError("Dataset name cannot contain '/'")
+        df = filepath_or_df
         utils.upload_dataframe_to_presigned_url(dataset_name,
                                                 df, upload_url, verbose=verbose)
     if verbose:
-        print(f"Uploading {dataset_filepath}")
+        print(f"Uploading {dataset_name}")
+
+    # Process the uploaded dataset remotely
     process_url = utils.get_server_url(server) + "/process_uploaded_dataset"
     r = requests.post(process_url, headers=headers)
     if verbose:
         utils.print_response_message(r)
 
 
 def query_dataset(dataset_name: str, server="cloud", verbose=False, debug=False) -> pd.DataFrame:
@@ -65,30 +81,33 @@
     df = utils.extract_csv_from_response(r, "summary")
     if verbose:
         utils.print_response_message(r)
         print("Summary:\n", df, "\n")
     return df
 
 
-def list_datasets(server="cloud", verbose=False, debug=False) -> list:
+def list_datasets(server="cloud", verbose=False, debug=False) -> Union[list, None]:
     """
     List datasets that have been uploaded to the cloud
     params:
         server: str; either "cloud" or "local"
         verbose: bool
         debug: bool
     """
     url = utils.get_server_url(server) + "/list_datasets"
     headers = utils.construct_standard_headers(debug=debug)
     r = requests.get(url, headers=headers)
     utils.check_response(r)
     if verbose:
         utils.print_response_message(r)
-    response = r.json()
-    return response["datasets"]
+    datasets = r.json()["datasets"]
+    if verbose and datasets:
+        print("Datasets:")
+        pprint(datasets)
+    return datasets
 
 
 def delete_dataset(dataset_name: str, server="cloud", verbose=False, debug=False) -> None:
     """
     Delete a dataset from the cloud
     params:
         dataset_name: str; name of dataset on S3 (same as the uploaded file name)
@@ -105,15 +124,15 @@
         utils.print_response_message(r)
 
 ###  ###
 
 ### Campaign functions ###
 
 
-def train_campaign(filepath_or_params, campaign: str, server="cloud", verbose=False, debug=False) -> None:
+def train_campaign(filepath_or_params: Union[str, dict], campaign: str, server="cloud", verbose=False, debug=False) -> None:
     """
     Train a campaign remotely using twinLab
     params:
         filepath_or_params: str or dict; filepath to json or parameters dict for training
         campaign: str; name of this campaign and final trained model (user choice)
         server: str; either "cloud" or "local"
         verbose: bool
@@ -153,30 +172,33 @@
     if verbose:
         utils.print_response_message(r)
         print("Metadata:")
         pprint(metadata, compact=True, sort_dicts=False)
     return metadata
 
 
-def list_campaigns(server="cloud", verbose=False, debug=False) -> list:
+def list_campaigns(server="cloud", verbose=False, debug=False) -> Union[list, None]:
     """
     List all trained campaigns stored in cloud
     params:
         server: str; either "cloud" or "local"
         verbose: bool
         debug: bool
     """
     url = utils.get_server_url(server) + "/list_campaigns"
     headers = utils.construct_standard_headers(debug=debug)
     r = requests.get(url, headers=headers)
     utils.check_response(r)
     if verbose:
         utils.print_response_message(r)
-    response = r.json()
-    return response["campaigns"]
+    campaigns = r.json()["campaigns"]
+    if verbose and campaigns:
+        print("Campaigns:")
+        pprint(campaigns)
+    return campaigns
 
 
 def predict_campaign(
     filepath_or_df, campaign: str, server="cloud", verbose=False, debug=False
 ) -> tuple:
     """
     Predict from a pre-trained campaign that exists on the cloud
```

### Comparing `twinlab-1.1.1/twinlab/settings.py` & `twinlab-1.1.2/twinlab/settings.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 # Third-party imports
 from pydantic import BaseSettings
 
 
 class Environment(BaseSettings):
     TWINLAB_LOCAL_SERVER: Optional[str]
+    TWINLAB_DEV_SERVER: Optional[str]
     TWINLAB_STAGE_SERVER: Optional[str]
     TWINLAB_SERVER: str
     TWINLAB_GROUPNAME: str
     TWINLAB_USERNAME: str
     TWINLAB_TOKEN: str
 
     class Config:
```

### Comparing `twinlab-1.1.1/twinlab/utils.py` & `twinlab-1.1.2/twinlab/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 # Standard imports
 import io
+import os
 import argparse
 import json
 from pprint import pprint
 
 # Third-party imports
 import requests
 import pandas as pd
 
 # Project imports
 from .settings import ENV
 
 
 PARAMS_COERCION = {  # Convert these names in the params file
     "test_train_split": "train_test_split",  # Common mistake
-    # "num_train_examples": "train_test_split", # TODO: Think of something better
+    "num_training_examples": "train_test_split",  #  TODO: Think of something better
+    "dataset": "filename",
 }
-TRAIN_CAMPAIGN_CLOUD_URL = "https://cma567qwquixu7bbjcnhbjsxjm0yumvu.lambda-url.eu-west-2.on.aws/"
+TRAIN_CAMPAIGN_DEV_URL = "https://pdersvjxmgrkqojwyeyocqm7le0iwtkx.lambda-url.eu-west-2.on.aws/"
 TRAIN_CAMPAIGN_STAGE_URL = "https://b7vgjlsn73e7n7kci5rwoxjc7e0pkcqn.lambda-url.eu-west-2.on.aws/"
+TRAIN_CAMPAIGN_CLOUD_URL = "https://cma567qwquixu7bbjcnhbjsxjm0yumvu.lambda-url.eu-west-2.on.aws/"
+
 
 ### Utility functions ###
 
 
 # def unwrap_payload(event: dict) -> dict:
 #     """
 #     Return payload and decode if it is base64 encoded
@@ -43,16 +47,17 @@
 def get_command_line_args() -> argparse.Namespace:
     """
     Parse command-line arguments
     """
     parser = argparse.ArgumentParser()
     parser.add_argument(
         "server",
-        default=False,
-        help="specify whether to use local or cloud lambda function",
+        default="cloud",
+        nargs='?',
+        help="Specify whether to use local or cloud lambda function",
     )
     args = parser.parse_args()
     return args
 
 
 def construct_standard_headers(debug=False) -> dict:
     headers = {
@@ -66,35 +71,42 @@
 
 def get_server_url(server: str) -> str:
     """
     The URL is the dockerised lambda function that's been set up in cloud by alexander
     """
     if server == "local":
         baseURL = ENV.TWINLAB_LOCAL_SERVER
-    elif server == "cloud":
-        baseURL = ENV.TWINLAB_SERVER
+    elif server == "dev":
+        baseURL = ENV.TWINLAB_DEV_SERVER
     elif server == "stage":
         baseURL = ENV.TWINLAB_STAGE_SERVER
+    elif server == "cloud":
+        baseURL = ENV.TWINLAB_SERVER
     else:
         print("Server:", server)
-        raise ValueError("Server must be either 'local', 'cloud', or 'stage'")
+        raise ValueError(
+            "Server must be either 'local', 'dev', 'stage', or 'cloud'")
+    if baseURL is None:  # Catch if the server URL has not been set
+        raise ValueError("Server URL not set")
     return baseURL
 
 
 def get_train_campaign_url(server: str) -> str:
     """
     Get the URL for the train_campaign lambda function
     These are different to avoid the AWS Lambda 29s gateway timeout
     """
-    if server == "cloud":
-        url = TRAIN_CAMPAIGN_CLOUD_URL
+    if server == "dev":
+        url = TRAIN_CAMPAIGN_DEV_URL
     elif server == "stage":
         url = TRAIN_CAMPAIGN_STAGE_URL
+    elif server == "cloud":
+        url = TRAIN_CAMPAIGN_CLOUD_URL
     else:
-        url = get_server_url(server) + "/train_campaign"
+        url = os.path.join(get_server_url(server), "train_campaign")
     return url
 
 
 def coerce_params_dict(params: dict) -> dict:
     """
     Relabel parameters to be consistent with twinLab library
     """
```

### Comparing `twinlab-1.1.1/PKG-INFO` & `twinlab-1.1.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twinlab
-Version: 1.1.1
+Version: 1.1.2
 Summary: Client interface for twinLab machine-learning in the cloud.
 Home-page: https://www.digilab.co.uk/
 License: MIT
 Keywords: machine-learning,AI,cloud,twinLab,digiLab
 Author: DigiLab Solutions Ltd.
 Author-email: info@digilab.co.uk
 Maintainer: Alexander Mead
@@ -36,54 +36,49 @@
 ## Installation
 
 Most users should use `pip`
 ```shell
 pip install twinlab
 ```
 
-If you want to modify the client-side code, or have a local installation for some reason
+If you want to modify the client-side code, or have a local installation, you will need to have `git`, `poetry`, and a `python` version of `3.9` or higher installed. Then you can do:
 ```shell
 git clone https://github.com/digiLab-ai/twinLab-client.git
 cd twinlab-client
 poetry install
 ```
 
 ## Environment setup
 
 You will need a `.env` file in your project directory that looks like the `.env.example` file in this repository
 ```shell
 cp .env.example .env
 ```
-and fill in your twinLab user details.
+and fill in your `twinLab` user details.
 
 ## Commands
 
 Testing:
 
 ```shell
-poetry run python scripts/test.py cloud 
+poetry run python scripts/test.py
 ```
 where `test.py` can be replaced with any of the scripts in the `script` directory.
 
-You need to have a local server for the (private) `twinlab-cloud` repository running for local testing. But local testing can then be run with
-```shell
-poetry run python scripts/test.py local
-```
-
 ## Example
 
 Here we create some mock data (which has a quadratic relationship between `X` and `y`) and use `twinLab` to create a surrogate model with quantified uncertainty.
 ```python
 # Import libraries
 import twinlab as tl
 import pandas as pd
 
-# Create a dataset and upload to twinLab cloud
+# Create a dataset and upload to the twinLab cloud
 df = pd.DataFrame({'X': [1, 2, 3, 4], 'y': [1, 4, 9, 16]})
-tl.upload_dataset('test.csv', df)
+tl.upload_dataset(df, 'test.csv')
 
 # Train a machine-learning model for the data
 params = {
     'filename': 'test.csv',
     'inputs': ['X'],
     'outputs': ['y'],
 }
```

