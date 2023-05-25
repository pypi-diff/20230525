# Comparing `tmp/mlflow-deploifai-0.0.2.tar.gz` & `tmp/mlflow-deploifai-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/mlflow-deploifai-plugin/mlflow-deploifai-plugin/dist/tmpu1fip21s/mlflow-deploifai-0.0.2.tar", last modified: Wed Jun  1 08:38:33 2022, max compression
+gzip compressed data, was "mlflow-deploifai-0.0.3.tar", last modified: Thu May 25 07:39:25 2023, max compression
```

## Comparing `mlflow-deploifai-0.0.2.tar` & `mlflow-deploifai-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 08:38:33.000000 mlflow-deploifai-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (121)     1517 2022-06-01 08:37:49.000000 mlflow-deploifai-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-06-01 08:37:49.000000 mlflow-deploifai-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1155 2022-06-01 08:38:33.000000 mlflow-deploifai-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      882 2022-06-01 08:37:49.000000 mlflow-deploifai-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 08:38:33.000000 mlflow-deploifai-0.0.2/mlflow_deploifai/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-01 08:37:49.000000 mlflow-deploifai-0.0.2/mlflow_deploifai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1100 2022-06-01 08:37:49.000000 mlflow-deploifai-0.0.2/mlflow_deploifai/request_header_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 08:38:33.000000 mlflow-deploifai-0.0.2/mlflow_deploifai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1155 2022-06-01 08:38:32.000000 mlflow-deploifai-0.0.2/mlflow_deploifai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      368 2022-06-01 08:38:33.000000 mlflow-deploifai-0.0.2/mlflow_deploifai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-01 08:38:32.000000 mlflow-deploifai-0.0.2/mlflow_deploifai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      114 2022-06-01 08:38:32.000000 mlflow-deploifai-0.0.2/mlflow_deploifai.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-06-01 08:38:32.000000 mlflow-deploifai-0.0.2/mlflow_deploifai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-06-01 08:38:32.000000 mlflow-deploifai-0.0.2/mlflow_deploifai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      104 2022-06-01 08:37:49.000000 mlflow-deploifai-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-01 08:38:33.000000 mlflow-deploifai-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      824 2022-06-01 08:37:49.000000 mlflow-deploifai-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:39:25.136376 mlflow-deploifai-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-05-25 07:38:35.000000 mlflow-deploifai-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-25 07:38:35.000000 mlflow-deploifai-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-05-25 07:39:25.136376 mlflow-deploifai-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-25 07:38:35.000000 mlflow-deploifai-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:39:25.136376 mlflow-deploifai-0.0.3/mlflow_deploifai/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:38:35.000000 mlflow-deploifai-0.0.3/mlflow_deploifai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-25 07:38:35.000000 mlflow-deploifai-0.0.3/mlflow_deploifai/request_header_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:39:25.136376 mlflow-deploifai-0.0.3/mlflow_deploifai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-05-25 07:39:25.000000 mlflow-deploifai-0.0.3/mlflow_deploifai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-25 07:39:25.000000 mlflow-deploifai-0.0.3/mlflow_deploifai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 07:39:25.000000 mlflow-deploifai-0.0.3/mlflow_deploifai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-25 07:39:25.000000 mlflow-deploifai-0.0.3/mlflow_deploifai.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-25 07:39:25.000000 mlflow-deploifai-0.0.3/mlflow_deploifai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-25 07:39:25.000000 mlflow-deploifai-0.0.3/mlflow_deploifai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-25 07:38:35.000000 mlflow-deploifai-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 07:39:25.136376 mlflow-deploifai-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-25 07:38:35.000000 mlflow-deploifai-0.0.3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `mlflow-deploifai-0.0.2/LICENSE` & `mlflow-deploifai-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mlflow-deploifai-0.0.2/PKG-INFO` & `mlflow-deploifai-0.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlflow-deploifai
-Version: 0.0.2
+Version: 0.0.3
 Summary: Deploifai plugin for MLflow
 Home-page: https://github.com/deploifai/mlflow-deploifai-plugin
 Author: Deploifai Limited
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `mlflow-deploifai-0.0.2/README.md` & `mlflow-deploifai-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `mlflow-deploifai-0.0.2/mlflow_deploifai/request_header_provider.py` & `mlflow-deploifai-0.0.3/mlflow_deploifai/request_header_provider.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,17 +3,20 @@
 from mlflow.tracking.request_header.abstract_request_header_provider import (
     RequestHeaderProvider,
 )
 from mlflow.tracking.fluent import active_run, _get_experiment_id, get_experiment
 
 
 class DeploifaiRequestHeaderProvider(RequestHeaderProvider):
-    # set class variable to identify deploifai experiment run so that all mlflow runs get associated with the same deploifai experiment run
-    # if USER_EXPERIMENT_RUN_ID environment variable is not set, generate a new deploifai experiment run using a new uuid
-    _deploifai_run_id = os.environ.get("USER_EXPERIMENT_RUN_ID", default=str(uuid.uuid4()))
+    # set class variable to identify deploifai experiment run so that all mlflow runs get associated with the same
+    # deploifai experiment run if USER_EXPERIMENT_RUN_ID environment variable is not set, generate a new deploifai
+    # experiment run using a new uuid
+    _deploifai_run_id = os.environ.get(
+        "USER_EXPERIMENT_RUN_ID", default=str(uuid.uuid4())
+    )
 
     def in_context(self):
         return True
 
     def request_headers(self):
         added_headers = {}
```

### Comparing `mlflow-deploifai-0.0.2/mlflow_deploifai.egg-info/PKG-INFO` & `mlflow-deploifai-0.0.3/mlflow_deploifai.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlflow-deploifai
-Version: 0.0.2
+Version: 0.0.3
 Summary: Deploifai plugin for MLflow
 Home-page: https://github.com/deploifai/mlflow-deploifai-plugin
 Author: Deploifai Limited
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `mlflow-deploifai-0.0.2/setup.py` & `mlflow-deploifai-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="mlflow-deploifai",
-    version="0.0.2",
+    version="0.0.3",
     author="Deploifai Limited",
     description="Deploifai plugin for MLflow",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/deploifai/mlflow-deploifai-plugin",
     python_requires=">=3.7",
     packages=find_packages(),
-    # Require MLflow as a dependency of the plugin, so that plugin users can simply install
-    # the plugin & then immediately use it with MLflow
+    # Require MLFlow as a dependency of the plugin, so that plugin users can simply install
+    # the plugin & then immediately use it with MLFlow
     install_requires=["mlflow"],
     entry_points={
         "mlflow.request_header_provider":
             "unused=mlflow_deploifai.request_header_provider:DeploifaiRequestHeaderProvider"
     },
 )
```

