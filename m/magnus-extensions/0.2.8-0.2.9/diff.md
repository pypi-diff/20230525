# Comparing `tmp/magnus_extensions-0.2.8.tar.gz` & `tmp/magnus_extensions-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magnus_extensions-0.2.8.tar", max compression
+gzip compressed data, was "magnus_extensions-0.2.9.tar", max compression
```

## Comparing `magnus_extensions-0.2.8.tar` & `magnus_extensions-0.2.9.tar`

### file list

```diff
@@ -1,30 +1,32 @@
--rw-r--r--   0        0        0    11357 2023-04-20 13:10:43.146381 magnus_extensions-0.2.8/LICENSE
--rw-r--r--   0        0        0     2304 2023-04-20 13:10:43.146381 magnus_extensions-0.2.8/README.md
--rw-r--r--   0        0        0     5339 2023-04-20 13:10:43.154381 magnus_extensions-0.2.8/magnus_extensions/aws.py
--rw-r--r--   0        0        0      718 2023-04-20 13:10:43.154381 magnus_extensions-0.2.8/magnus_extensions/catalog/k8s_pvc/implementation.py
--rw-r--r--   0        0        0     1952 2023-04-20 13:10:43.154381 magnus_extensions-0.2.8/magnus_extensions/catalog/k8s_pvc/integration.py
--rw-r--r--   0        0        0     7820 2023-04-20 13:10:43.154381 magnus_extensions-0.2.8/magnus_extensions/catalog/s3/implementation.py
--rw-r--r--   0        0        0      632 2023-04-20 13:10:43.154381 magnus_extensions-0.2.8/magnus_extensions/catalog/s3/integration.py
--rw-r--r--   0        0        0      598 2023-04-20 13:10:43.154381 magnus_extensions-0.2.8/magnus_extensions/datastore/chunked_k8s_pvc/implementation.py
--rw-r--r--   0        0        0     2020 2023-04-20 13:10:43.154381 magnus_extensions-0.2.8/magnus_extensions/datastore/chunked_k8s_pvc/integration.py
--rw-r--r--   0        0        0     7953 2023-04-20 13:10:43.154381 magnus_extensions-0.2.8/magnus_extensions/datastore/chunked_s3/implementation.py
--rw-r--r--   0        0        0      777 2023-04-20 13:10:43.154381 magnus_extensions-0.2.8/magnus_extensions/datastore/chunked_s3/integration.py
--rw-r--r--   0        0        0    18942 2023-04-20 13:10:43.154381 magnus_extensions-0.2.8/magnus_extensions/datastore/db/implementation.py
--rw-r--r--   0        0        0      818 2023-04-20 13:10:43.154381 magnus_extensions-0.2.8/magnus_extensions/datastore/db/integration.py
--rw-r--r--   0        0        0      562 2023-04-20 13:10:43.154381 magnus_extensions-0.2.8/magnus_extensions/datastore/k8s_pvc/implementation.py
--rw-r--r--   0        0        0     2013 2023-04-20 13:10:43.154381 magnus_extensions-0.2.8/magnus_extensions/datastore/k8s_pvc/integration.py
--rw-r--r--   0        0        0     5037 2023-04-20 13:10:43.154381 magnus_extensions-0.2.8/magnus_extensions/datastore/s3/implementation.py
--rw-r--r--   0        0        0     1868 2023-04-20 13:10:43.154381 magnus_extensions-0.2.8/magnus_extensions/datastore/s3/integration.py
--rw-r--r--   0        0        0    16160 2023-04-20 13:10:43.154381 magnus_extensions-0.2.8/magnus_extensions/executor/argo/implementation.py
--rw-r--r--   0        0        0     1589 2023-04-20 13:10:43.154381 magnus_extensions-0.2.8/magnus_extensions/executor/argo/integration.py
--rw-r--r--   0        0        0     9776 2023-04-20 13:10:43.154381 magnus_extensions-0.2.8/magnus_extensions/executor/k8s_job/implementation.py
--rw-r--r--   0        0        0     2169 2023-04-20 13:10:43.154381 magnus_extensions-0.2.8/magnus_extensions/executor/k8s_job/integration.py
--rw-r--r--   0        0        0    13340 2023-04-20 13:10:43.154381 magnus_extensions-0.2.8/magnus_extensions/executor/kubeflow/implementation.py
--rw-r--r--   0        0        0     1577 2023-04-20 13:10:43.154381 magnus_extensions-0.2.8/magnus_extensions/executor/kubeflow/integration.py
--rw-r--r--   0        0        0     3364 2023-04-20 13:10:43.154381 magnus_extensions-0.2.8/magnus_extensions/experiment_tracker/mlflow/implementation.py
--rw-r--r--   0        0        0       87 2023-04-20 13:10:43.154381 magnus_extensions-0.2.8/magnus_extensions/magnus_extension_template/implementation.py
--rw-r--r--   0        0        0       47 2023-04-20 13:10:43.154381 magnus_extensions-0.2.8/magnus_extensions/magnus_extension_template/integration.py
--rw-r--r--   0        0        0     2623 2023-04-20 13:10:43.154381 magnus_extensions-0.2.8/magnus_extensions/secrets/aws/implementation.py
--rw-r--r--   0        0        0      641 2023-04-20 13:10:43.154381 magnus_extensions-0.2.8/magnus_extensions/secrets/aws/integration.py
--rw-r--r--   0        0        0     4996 2023-04-20 13:11:00.795077 magnus_extensions-0.2.8/pyproject.toml
--rw-r--r--   0        0        0     3246 1970-01-01 00:00:00.000000 magnus_extensions-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-27 13:24:21.646887 magnus_extensions-0.2.9/LICENSE
+-rw-r--r--   0        0        0     2304 2023-04-27 13:24:21.646887 magnus_extensions-0.2.9/README.md
+-rw-r--r--   0        0        0     5339 2023-04-27 13:24:21.654887 magnus_extensions-0.2.9/magnus_extensions/aws.py
+-rw-r--r--   0        0        0      718 2023-04-27 13:24:21.654887 magnus_extensions-0.2.9/magnus_extensions/catalog/k8s_pvc/implementation.py
+-rw-r--r--   0        0        0     1952 2023-04-27 13:24:21.654887 magnus_extensions-0.2.9/magnus_extensions/catalog/k8s_pvc/integration.py
+-rw-r--r--   0        0        0     7820 2023-04-27 13:24:21.654887 magnus_extensions-0.2.9/magnus_extensions/catalog/s3/implementation.py
+-rw-r--r--   0        0        0      632 2023-04-27 13:24:21.654887 magnus_extensions-0.2.9/magnus_extensions/catalog/s3/integration.py
+-rw-r--r--   0        0        0      598 2023-04-27 13:24:21.654887 magnus_extensions-0.2.9/magnus_extensions/datastore/chunked_k8s_pvc/implementation.py
+-rw-r--r--   0        0        0     2020 2023-04-27 13:24:21.654887 magnus_extensions-0.2.9/magnus_extensions/datastore/chunked_k8s_pvc/integration.py
+-rw-r--r--   0        0        0     7953 2023-04-27 13:24:21.654887 magnus_extensions-0.2.9/magnus_extensions/datastore/chunked_s3/implementation.py
+-rw-r--r--   0        0        0      777 2023-04-27 13:24:21.654887 magnus_extensions-0.2.9/magnus_extensions/datastore/chunked_s3/integration.py
+-rw-r--r--   0        0        0    18942 2023-04-27 13:24:21.654887 magnus_extensions-0.2.9/magnus_extensions/datastore/db/implementation.py
+-rw-r--r--   0        0        0      818 2023-04-27 13:24:21.654887 magnus_extensions-0.2.9/magnus_extensions/datastore/db/integration.py
+-rw-r--r--   0        0        0      562 2023-04-27 13:24:21.654887 magnus_extensions-0.2.9/magnus_extensions/datastore/k8s_pvc/implementation.py
+-rw-r--r--   0        0        0     2013 2023-04-27 13:24:21.654887 magnus_extensions-0.2.9/magnus_extensions/datastore/k8s_pvc/integration.py
+-rw-r--r--   0        0        0     5037 2023-04-27 13:24:21.654887 magnus_extensions-0.2.9/magnus_extensions/datastore/s3/implementation.py
+-rw-r--r--   0        0        0     1868 2023-04-27 13:24:21.654887 magnus_extensions-0.2.9/magnus_extensions/datastore/s3/integration.py
+-rw-r--r--   0        0        0    16160 2023-04-27 13:24:21.654887 magnus_extensions-0.2.9/magnus_extensions/executor/argo/implementation.py
+-rw-r--r--   0        0        0     1589 2023-04-27 13:24:21.654887 magnus_extensions-0.2.9/magnus_extensions/executor/argo/integration.py
+-rw-r--r--   0        0        0     9776 2023-04-27 13:24:21.654887 magnus_extensions-0.2.9/magnus_extensions/executor/k8s_job/implementation.py
+-rw-r--r--   0        0        0     2169 2023-04-27 13:24:21.654887 magnus_extensions-0.2.9/magnus_extensions/executor/k8s_job/integration.py
+-rw-r--r--   0        0        0    13340 2023-04-27 13:24:21.654887 magnus_extensions-0.2.9/magnus_extensions/executor/kubeflow/implementation.py
+-rw-r--r--   0        0        0     1577 2023-04-27 13:24:21.654887 magnus_extensions-0.2.9/magnus_extensions/executor/kubeflow/integration.py
+-rw-r--r--   0        0        0     5284 2023-04-27 13:24:21.654887 magnus_extensions-0.2.9/magnus_extensions/executor/slurm_job/implementation.py
+-rw-r--r--   0        0        0      564 2023-04-27 13:24:21.654887 magnus_extensions-0.2.9/magnus_extensions/executor/slurm_job/integration.py
+-rw-r--r--   0        0        0     3364 2023-04-27 13:24:21.658887 magnus_extensions-0.2.9/magnus_extensions/experiment_tracker/mlflow/implementation.py
+-rw-r--r--   0        0        0       87 2023-04-27 13:24:21.658887 magnus_extensions-0.2.9/magnus_extensions/magnus_extension_template/implementation.py
+-rw-r--r--   0        0        0       47 2023-04-27 13:24:21.658887 magnus_extensions-0.2.9/magnus_extensions/magnus_extension_template/integration.py
+-rw-r--r--   0        0        0     2623 2023-04-27 13:24:21.658887 magnus_extensions-0.2.9/magnus_extensions/secrets/aws/implementation.py
+-rw-r--r--   0        0        0      641 2023-04-27 13:24:21.658887 magnus_extensions-0.2.9/magnus_extensions/secrets/aws/integration.py
+-rw-r--r--   0        0        0     5176 2023-04-27 13:24:42.738978 magnus_extensions-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0     3246 1970-01-01 00:00:00.000000 magnus_extensions-0.2.9/PKG-INFO
```

### Comparing `magnus_extensions-0.2.8/LICENSE` & `magnus_extensions-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `magnus_extensions-0.2.8/README.md` & `magnus_extensions-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `magnus_extensions-0.2.8/magnus_extensions/aws.py` & `magnus_extensions-0.2.9/magnus_extensions/aws.py`

 * *Files identical despite different names*

### Comparing `magnus_extensions-0.2.8/magnus_extensions/catalog/k8s_pvc/implementation.py` & `magnus_extensions-0.2.9/magnus_extensions/catalog/k8s_pvc/implementation.py`

 * *Files identical despite different names*

### Comparing `magnus_extensions-0.2.8/magnus_extensions/catalog/k8s_pvc/integration.py` & `magnus_extensions-0.2.9/magnus_extensions/catalog/k8s_pvc/integration.py`

 * *Files identical despite different names*

### Comparing `magnus_extensions-0.2.8/magnus_extensions/catalog/s3/implementation.py` & `magnus_extensions-0.2.9/magnus_extensions/catalog/s3/implementation.py`

 * *Files identical despite different names*

### Comparing `magnus_extensions-0.2.8/magnus_extensions/catalog/s3/integration.py` & `magnus_extensions-0.2.9/magnus_extensions/catalog/s3/integration.py`

 * *Files identical despite different names*

### Comparing `magnus_extensions-0.2.8/magnus_extensions/datastore/chunked_k8s_pvc/implementation.py` & `magnus_extensions-0.2.9/magnus_extensions/datastore/chunked_k8s_pvc/implementation.py`

 * *Files identical despite different names*

### Comparing `magnus_extensions-0.2.8/magnus_extensions/datastore/chunked_k8s_pvc/integration.py` & `magnus_extensions-0.2.9/magnus_extensions/datastore/chunked_k8s_pvc/integration.py`

 * *Files identical despite different names*

### Comparing `magnus_extensions-0.2.8/magnus_extensions/datastore/chunked_s3/implementation.py` & `magnus_extensions-0.2.9/magnus_extensions/datastore/chunked_s3/implementation.py`

 * *Files identical despite different names*

### Comparing `magnus_extensions-0.2.8/magnus_extensions/datastore/chunked_s3/integration.py` & `magnus_extensions-0.2.9/magnus_extensions/datastore/chunked_s3/integration.py`

 * *Files identical despite different names*

### Comparing `magnus_extensions-0.2.8/magnus_extensions/datastore/db/implementation.py` & `magnus_extensions-0.2.9/magnus_extensions/datastore/db/implementation.py`

 * *Files identical despite different names*

### Comparing `magnus_extensions-0.2.8/magnus_extensions/datastore/db/integration.py` & `magnus_extensions-0.2.9/magnus_extensions/datastore/db/integration.py`

 * *Files identical despite different names*

### Comparing `magnus_extensions-0.2.8/magnus_extensions/datastore/k8s_pvc/implementation.py` & `magnus_extensions-0.2.9/magnus_extensions/datastore/k8s_pvc/implementation.py`

 * *Files identical despite different names*

### Comparing `magnus_extensions-0.2.8/magnus_extensions/datastore/k8s_pvc/integration.py` & `magnus_extensions-0.2.9/magnus_extensions/datastore/k8s_pvc/integration.py`

 * *Files identical despite different names*

### Comparing `magnus_extensions-0.2.8/magnus_extensions/datastore/s3/implementation.py` & `magnus_extensions-0.2.9/magnus_extensions/datastore/s3/implementation.py`

 * *Files identical despite different names*

### Comparing `magnus_extensions-0.2.8/magnus_extensions/datastore/s3/integration.py` & `magnus_extensions-0.2.9/magnus_extensions/datastore/s3/integration.py`

 * *Files identical despite different names*

### Comparing `magnus_extensions-0.2.8/magnus_extensions/executor/argo/implementation.py` & `magnus_extensions-0.2.9/magnus_extensions/executor/argo/implementation.py`

 * *Files identical despite different names*

### Comparing `magnus_extensions-0.2.8/magnus_extensions/executor/argo/integration.py` & `magnus_extensions-0.2.9/magnus_extensions/executor/argo/integration.py`

 * *Files identical despite different names*

### Comparing `magnus_extensions-0.2.8/magnus_extensions/executor/k8s_job/implementation.py` & `magnus_extensions-0.2.9/magnus_extensions/executor/k8s_job/implementation.py`

 * *Files identical despite different names*

### Comparing `magnus_extensions-0.2.8/magnus_extensions/executor/k8s_job/integration.py` & `magnus_extensions-0.2.9/magnus_extensions/executor/k8s_job/integration.py`

 * *Files identical despite different names*

### Comparing `magnus_extensions-0.2.8/magnus_extensions/executor/kubeflow/implementation.py` & `magnus_extensions-0.2.9/magnus_extensions/executor/kubeflow/implementation.py`

 * *Files identical despite different names*

### Comparing `magnus_extensions-0.2.8/magnus_extensions/executor/kubeflow/integration.py` & `magnus_extensions-0.2.9/magnus_extensions/executor/kubeflow/integration.py`

 * *Files identical despite different names*

### Comparing `magnus_extensions-0.2.8/magnus_extensions/experiment_tracker/mlflow/implementation.py` & `magnus_extensions-0.2.9/magnus_extensions/experiment_tracker/mlflow/implementation.py`

 * *Files identical despite different names*

### Comparing `magnus_extensions-0.2.8/magnus_extensions/secrets/aws/implementation.py` & `magnus_extensions-0.2.9/magnus_extensions/secrets/aws/implementation.py`

 * *Files identical despite different names*

### Comparing `magnus_extensions-0.2.8/magnus_extensions/secrets/aws/integration.py` & `magnus_extensions-0.2.9/magnus_extensions/secrets/aws/integration.py`

 * *Files identical despite different names*

### Comparing `magnus_extensions-0.2.8/pyproject.toml` & `magnus_extensions-0.2.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "magnus_extensions"
-version = "0.2.8"
+version = "0.2.9"
 description = "Extensions to Magnus core"
 authors = ["Vijay Vammi <mesanthu@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{include = "magnus_extensions"}]
 
 [tool.poetry.dependencies]
@@ -51,14 +51,15 @@
 [tool.poetry.plugins."secrets"]
 "aws-secrets-manager" = "magnus_extensions.secrets.aws.implementation:AWSSecretsManager"
 
 [tool.poetry.plugins."executor"]
 "kfp" = "magnus_extensions.executor.kubeflow.implementation:KubeFlowExecutor"
 "argo" = "magnus_extensions.executor.argo.implementation:ArgoExecutor"
 "k8s-job" = "magnus_extensions.executor.k8s_job.implementation:K8sJobExecutor"
+"slurm-job" = "magnus_extensions.executor.slurm_job.implementation:SlurmJobExecutor"
 
 [tool.poetry.plugins."experiment_tracker"]
 "mlflow" = "magnus_extensions.experiment_tracker.mlflow.implementation:MLFlowExperimentTracker"
 
 # Use this provide namespace of the integration
 # naming convention: keep it simple.
 [tool.poetry.plugins."integration"]
@@ -95,14 +96,16 @@
 "pvccatalogkfp" = "magnus_extensions.catalog.k8s_pvc.integration:KfpCompute"
 "pvccatalogargo" = "magnus_extensions.catalog.k8s_pvc.integration:ArgoCompute"
 # k8s-job
 "k8sjobbuffered" = "magnus_extensions.k8s_job.integration:BufferedRunLogStore"
 "k8sjobfsrunlog" = "magnus_extensions.k8s_job.integration:FileSystemRunLogStore"
 "k8sjobfschunkedfsrunlog" = "magnus_extensions.k8s_job.integration:ChunkedFSRunLogStore"
 "k8sjobffscatalog" = "magnus_extensions.k8s_job.integration:FileSystemCatalog"
+# slurm-job
+"slurmjobbuffered" = "magnus_extensions.slurm_job.integration:BufferedRunLogStore"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.semantic_release]
```

### Comparing `magnus_extensions-0.2.8/PKG-INFO` & `magnus_extensions-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magnus-extensions
-Version: 0.2.8
+Version: 0.2.9
 Summary: Extensions to Magnus core
 License: Apache-2.0
 Author: Vijay Vammi
 Author-email: mesanthu@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

