# Comparing `tmp/fedml_databricks-1.0.3.tar.gz` & `tmp/fedml_databricks-1.0.3.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fedml_databricks-1.0.3.tar", last modified: Thu May 25 02:21:03 2023, max compression
+gzip compressed data, was "fedml_databricks-1.0.3.dev0.tar", last modified: Wed May 17 23:12:18 2023, max compression
```

## Comparing `fedml_databricks-1.0.3.tar` & `fedml_databricks-1.0.3.dev0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 I550585    (501) staff       (20)        0 2023-05-25 02:21:03.880990 fedml_databricks-1.0.3/
--rw-r--r--   0 I550585    (501) staff       (20)    11307 2023-04-27 21:31:25.000000 fedml_databricks-1.0.3/LICENSE.txt
--rw-r--r--   0 I550585    (501) staff       (20)     1343 2023-05-25 02:21:03.880423 fedml_databricks-1.0.3/PKG-INFO
--rw-r--r--   0 I550585    (501) staff       (20)      950 2023-04-27 21:31:25.000000 fedml_databricks-1.0.3/README.md
--rw-r--r--   0 I550585    (501) staff       (20)      103 2023-02-01 00:25:03.000000 fedml_databricks-1.0.3/pyproject.toml
--rw-r--r--   0 I550585    (501) staff       (20)       38 2023-05-25 02:21:03.881141 fedml_databricks-1.0.3/setup.cfg
--rw-r--r--   0 I550585    (501) staff       (20)     1097 2023-05-25 02:19:36.000000 fedml_databricks-1.0.3/setup.py
-drwxr-xr-x   0 I550585    (501) staff       (20)        0 2023-05-25 02:21:03.775461 fedml_databricks-1.0.3/src/
-drwxr-xr-x   0 I550585    (501) staff       (20)        0 2023-05-25 02:21:03.828368 fedml_databricks-1.0.3/src/fedml_databricks/
--rw-r--r--   0 I550585    (501) staff       (20)      107 2023-04-27 21:31:25.000000 fedml_databricks-1.0.3/src/fedml_databricks/__init__.py
-drwxr-xr-x   0 I550585    (501) staff       (20)        0 2023-05-25 02:21:03.859816 fedml_databricks-1.0.3/src/fedml_databricks/acr/
--rw-r--r--   0 I550585    (501) staff       (20)        0 2023-04-27 21:31:25.000000 fedml_databricks-1.0.3/src/fedml_databricks/acr/__init__.py
--rw-r--r--   0 I550585    (501) staff       (20)     1694 2023-04-27 21:31:25.000000 fedml_databricks-1.0.3/src/fedml_databricks/acr/acr_kyma_deploy.py
--rw-r--r--   0 I550585    (501) staff       (20)     6823 2023-04-27 21:31:25.000000 fedml_databricks-1.0.3/src/fedml_databricks/acr/acr_kyma_deploy.sh
--rw-r--r--   0 I550585    (501) staff       (20)      332 2023-04-27 21:31:25.000000 fedml_databricks-1.0.3/src/fedml_databricks/databricks_cli_configure.sh
--rw-r--r--   0 I550585    (501) staff       (20)    15793 2023-05-17 23:11:58.000000 fedml_databricks-1.0.3/src/fedml_databricks/dbconnection.py
--rw-r--r--   0 I550585    (501) staff       (20)      682 2023-04-27 21:31:25.000000 fedml_databricks-1.0.3/src/fedml_databricks/deployment_helper.py
-drwxr-xr-x   0 I550585    (501) staff       (20)        0 2023-05-25 02:21:03.879421 fedml_databricks-1.0.3/src/fedml_databricks/ecr/
--rw-r--r--   0 I550585    (501) staff       (20)        0 2023-04-27 21:31:25.000000 fedml_databricks-1.0.3/src/fedml_databricks/ecr/__init__.py
--rw-r--r--   0 I550585    (501) staff       (20)     1597 2023-04-27 21:31:25.000000 fedml_databricks-1.0.3/src/fedml_databricks/ecr/ecr_kyma_deploy.py
--rw-r--r--   0 I550585    (501) staff       (20)     5006 2023-04-27 21:31:25.000000 fedml_databricks-1.0.3/src/fedml_databricks/ecr/ecr_kyma_deploy.sh
--rw-r--r--   0 I550585    (501) staff       (20)     1771 2023-04-27 21:31:25.000000 fedml_databricks-1.0.3/src/fedml_databricks/kubectl_install_validate.sh
--rw-r--r--   0 I550585    (501) staff       (20)     3909 2023-04-27 21:31:25.000000 fedml_databricks-1.0.3/src/fedml_databricks/kyma_deploy.py
--rw-r--r--   0 I550585    (501) staff       (20)      656 2023-02-01 00:25:03.000000 fedml_databricks-1.0.3/src/fedml_databricks/logger.py
--rw-r--r--   0 I550585    (501) staff       (20)      701 2023-04-27 21:31:25.000000 fedml_databricks-1.0.3/src/fedml_databricks/predict.py
-drwxr-xr-x   0 I550585    (501) staff       (20)        0 2023-05-25 02:21:03.836148 fedml_databricks-1.0.3/src/fedml_databricks.egg-info/
--rw-r--r--   0 I550585    (501) staff       (20)     1343 2023-05-25 02:21:03.000000 fedml_databricks-1.0.3/src/fedml_databricks.egg-info/PKG-INFO
--rw-r--r--   0 I550585    (501) staff       (20)      823 2023-05-25 02:21:03.000000 fedml_databricks-1.0.3/src/fedml_databricks.egg-info/SOURCES.txt
--rw-r--r--   0 I550585    (501) staff       (20)        1 2023-05-25 02:21:03.000000 fedml_databricks-1.0.3/src/fedml_databricks.egg-info/dependency_links.txt
--rw-r--r--   0 I550585    (501) staff       (20)       65 2023-05-25 02:21:03.000000 fedml_databricks-1.0.3/src/fedml_databricks.egg-info/requires.txt
--rw-r--r--   0 I550585    (501) staff       (20)       17 2023-05-25 02:21:03.000000 fedml_databricks-1.0.3/src/fedml_databricks.egg-info/top_level.txt
+drwxr-xr-x   0 I550585    (501) staff       (20)        0 2023-05-17 23:12:18.249156 fedml_databricks-1.0.3.dev0/
+-rw-r--r--   0 I550585    (501) staff       (20)    11307 2023-04-27 21:31:25.000000 fedml_databricks-1.0.3.dev0/LICENSE.txt
+-rw-r--r--   0 I550585    (501) staff       (20)     1348 2023-05-17 23:12:18.247909 fedml_databricks-1.0.3.dev0/PKG-INFO
+-rw-r--r--   0 I550585    (501) staff       (20)      950 2023-04-27 21:31:25.000000 fedml_databricks-1.0.3.dev0/README.md
+-rw-r--r--   0 I550585    (501) staff       (20)      103 2023-02-01 00:25:03.000000 fedml_databricks-1.0.3.dev0/pyproject.toml
+-rw-r--r--   0 I550585    (501) staff       (20)       38 2023-05-17 23:12:18.249377 fedml_databricks-1.0.3.dev0/setup.cfg
+-rw-r--r--   0 I550585    (501) staff       (20)     1102 2023-05-17 20:51:35.000000 fedml_databricks-1.0.3.dev0/setup.py
+drwxr-xr-x   0 I550585    (501) staff       (20)        0 2023-05-17 23:12:18.203152 fedml_databricks-1.0.3.dev0/src/
+drwxr-xr-x   0 I550585    (501) staff       (20)        0 2023-05-17 23:12:18.234724 fedml_databricks-1.0.3.dev0/src/fedml_databricks/
+-rw-r--r--   0 I550585    (501) staff       (20)      107 2023-04-27 21:31:25.000000 fedml_databricks-1.0.3.dev0/src/fedml_databricks/__init__.py
+drwxr-xr-x   0 I550585    (501) staff       (20)        0 2023-05-17 23:12:18.243544 fedml_databricks-1.0.3.dev0/src/fedml_databricks/acr/
+-rw-r--r--   0 I550585    (501) staff       (20)        0 2023-04-27 21:31:25.000000 fedml_databricks-1.0.3.dev0/src/fedml_databricks/acr/__init__.py
+-rw-r--r--   0 I550585    (501) staff       (20)     1694 2023-04-27 21:31:25.000000 fedml_databricks-1.0.3.dev0/src/fedml_databricks/acr/acr_kyma_deploy.py
+-rw-r--r--   0 I550585    (501) staff       (20)     6823 2023-04-27 21:31:25.000000 fedml_databricks-1.0.3.dev0/src/fedml_databricks/acr/acr_kyma_deploy.sh
+-rw-r--r--   0 I550585    (501) staff       (20)      332 2023-04-27 21:31:25.000000 fedml_databricks-1.0.3.dev0/src/fedml_databricks/databricks_cli_configure.sh
+-rw-r--r--   0 I550585    (501) staff       (20)    15793 2023-05-17 23:11:58.000000 fedml_databricks-1.0.3.dev0/src/fedml_databricks/dbconnection.py
+-rw-r--r--   0 I550585    (501) staff       (20)      682 2023-04-27 21:31:25.000000 fedml_databricks-1.0.3.dev0/src/fedml_databricks/deployment_helper.py
+drwxr-xr-x   0 I550585    (501) staff       (20)        0 2023-05-17 23:12:18.246838 fedml_databricks-1.0.3.dev0/src/fedml_databricks/ecr/
+-rw-r--r--   0 I550585    (501) staff       (20)        0 2023-04-27 21:31:25.000000 fedml_databricks-1.0.3.dev0/src/fedml_databricks/ecr/__init__.py
+-rw-r--r--   0 I550585    (501) staff       (20)     1597 2023-04-27 21:31:25.000000 fedml_databricks-1.0.3.dev0/src/fedml_databricks/ecr/ecr_kyma_deploy.py
+-rw-r--r--   0 I550585    (501) staff       (20)     5006 2023-04-27 21:31:25.000000 fedml_databricks-1.0.3.dev0/src/fedml_databricks/ecr/ecr_kyma_deploy.sh
+-rw-r--r--   0 I550585    (501) staff       (20)     1771 2023-04-27 21:31:25.000000 fedml_databricks-1.0.3.dev0/src/fedml_databricks/kubectl_install_validate.sh
+-rw-r--r--   0 I550585    (501) staff       (20)     3909 2023-04-27 21:31:25.000000 fedml_databricks-1.0.3.dev0/src/fedml_databricks/kyma_deploy.py
+-rw-r--r--   0 I550585    (501) staff       (20)      656 2023-02-01 00:25:03.000000 fedml_databricks-1.0.3.dev0/src/fedml_databricks/logger.py
+-rw-r--r--   0 I550585    (501) staff       (20)      701 2023-04-27 21:31:25.000000 fedml_databricks-1.0.3.dev0/src/fedml_databricks/predict.py
+drwxr-xr-x   0 I550585    (501) staff       (20)        0 2023-05-17 23:12:18.240671 fedml_databricks-1.0.3.dev0/src/fedml_databricks.egg-info/
+-rw-r--r--   0 I550585    (501) staff       (20)     1348 2023-05-17 23:12:18.000000 fedml_databricks-1.0.3.dev0/src/fedml_databricks.egg-info/PKG-INFO
+-rw-r--r--   0 I550585    (501) staff       (20)      823 2023-05-17 23:12:18.000000 fedml_databricks-1.0.3.dev0/src/fedml_databricks.egg-info/SOURCES.txt
+-rw-r--r--   0 I550585    (501) staff       (20)        1 2023-05-17 23:12:18.000000 fedml_databricks-1.0.3.dev0/src/fedml_databricks.egg-info/dependency_links.txt
+-rw-r--r--   0 I550585    (501) staff       (20)       65 2023-05-17 23:12:18.000000 fedml_databricks-1.0.3.dev0/src/fedml_databricks.egg-info/requires.txt
+-rw-r--r--   0 I550585    (501) staff       (20)       17 2023-05-17 23:12:18.000000 fedml_databricks-1.0.3.dev0/src/fedml_databricks.egg-info/top_level.txt
```

### Comparing `fedml_databricks-1.0.3/LICENSE.txt` & `fedml_databricks-1.0.3.dev0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fedml_databricks-1.0.3/PKG-INFO` & `fedml_databricks-1.0.3.dev0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fedml_databricks
-Version: 1.0.3
+Version: 1.0.3.dev0
 Summary: A python library for building machine learning models on Databricks using a federated data source
 Author: SAP SE
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

### Comparing `fedml_databricks-1.0.3/README.md` & `fedml_databricks-1.0.3.dev0/README.md`

 * *Files identical despite different names*

### Comparing `fedml_databricks-1.0.3/setup.py` & `fedml_databricks-1.0.3.dev0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 setuptools.setup(
     name="fedml_databricks",
-    version="1.0.3",
+    version="1.0.3.dev0",
     author="SAP SE",
     description="A python library for building machine learning models on Databricks using a federated data source",
     license='Apache License 2.0',
     license_files = ['LICENSE.txt'],
     long_description=long_description,
     long_description_content_type='text/markdown',
     classifiers=[
```

### Comparing `fedml_databricks-1.0.3/src/fedml_databricks/acr/acr_kyma_deploy.py` & `fedml_databricks-1.0.3.dev0/src/fedml_databricks/acr/acr_kyma_deploy.py`

 * *Files identical despite different names*

### Comparing `fedml_databricks-1.0.3/src/fedml_databricks/acr/acr_kyma_deploy.sh` & `fedml_databricks-1.0.3.dev0/src/fedml_databricks/acr/acr_kyma_deploy.sh`

 * *Files identical despite different names*

### Comparing `fedml_databricks-1.0.3/src/fedml_databricks/dbconnection.py` & `fedml_databricks-1.0.3.dev0/src/fedml_databricks/dbconnection.py`

 * *Files identical despite different names*

### Comparing `fedml_databricks-1.0.3/src/fedml_databricks/deployment_helper.py` & `fedml_databricks-1.0.3.dev0/src/fedml_databricks/deployment_helper.py`

 * *Files identical despite different names*

### Comparing `fedml_databricks-1.0.3/src/fedml_databricks/ecr/ecr_kyma_deploy.py` & `fedml_databricks-1.0.3.dev0/src/fedml_databricks/ecr/ecr_kyma_deploy.py`

 * *Files identical despite different names*

### Comparing `fedml_databricks-1.0.3/src/fedml_databricks/ecr/ecr_kyma_deploy.sh` & `fedml_databricks-1.0.3.dev0/src/fedml_databricks/ecr/ecr_kyma_deploy.sh`

 * *Files identical despite different names*

### Comparing `fedml_databricks-1.0.3/src/fedml_databricks/kubectl_install_validate.sh` & `fedml_databricks-1.0.3.dev0/src/fedml_databricks/kubectl_install_validate.sh`

 * *Files identical despite different names*

### Comparing `fedml_databricks-1.0.3/src/fedml_databricks/kyma_deploy.py` & `fedml_databricks-1.0.3.dev0/src/fedml_databricks/kyma_deploy.py`

 * *Files identical despite different names*

### Comparing `fedml_databricks-1.0.3/src/fedml_databricks/logger.py` & `fedml_databricks-1.0.3.dev0/src/fedml_databricks/logger.py`

 * *Files identical despite different names*

### Comparing `fedml_databricks-1.0.3/src/fedml_databricks/predict.py` & `fedml_databricks-1.0.3.dev0/src/fedml_databricks/predict.py`

 * *Files identical despite different names*

### Comparing `fedml_databricks-1.0.3/src/fedml_databricks.egg-info/PKG-INFO` & `fedml_databricks-1.0.3.dev0/src/fedml_databricks.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fedml-databricks
-Version: 1.0.3
+Version: 1.0.3.dev0
 Summary: A python library for building machine learning models on Databricks using a federated data source
 Author: SAP SE
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

### Comparing `fedml_databricks-1.0.3/src/fedml_databricks.egg-info/SOURCES.txt` & `fedml_databricks-1.0.3.dev0/src/fedml_databricks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

