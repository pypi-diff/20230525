# Comparing `tmp/dagster-airflow-1.3.5.tar.gz` & `tmp/dagster-airflow-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-airflow-1.3.5.tar", last modified: Thu May 18 20:48:21 2023, max compression
+gzip compressed data, was "dagster-airflow-1.3.6.tar", last modified: Thu May 25 17:24:33 2023, max compression
```

## Comparing `dagster-airflow-1.3.5.tar` & `dagster-airflow-1.3.6.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:48:21.109655 dagster-airflow-1.3.5/
--rw-r--r--   0 root         (0) root         (0)    11344 2023-05-18 20:38:07.000000 dagster-airflow-1.3.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)      105 2023-05-18 20:38:07.000000 dagster-airflow-1.3.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      649 2023-05-18 20:48:21.109655 dagster-airflow-1.3.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      131 2023-05-18 20:38:07.000000 dagster-airflow-1.3.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:48:21.101656 dagster-airflow-1.3.5/dagster_airflow/
--rw-r--r--   0 root         (0) root         (0)     2474 2023-05-18 20:38:07.000000 dagster-airflow-1.3.5/dagster_airflow/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3759 2023-05-18 20:38:07.000000 dagster-airflow-1.3.5/dagster_airflow/airflow_dag_converter.py
--rw-r--r--   0 root         (0) root         (0)     7716 2023-05-18 20:38:07.000000 dagster-airflow-1.3.5/dagster_airflow/dagster_asset_factory.py
--rw-r--r--   0 root         (0) root         (0)     8158 2023-05-18 20:38:07.000000 dagster-airflow-1.3.5/dagster_airflow/dagster_factory.py
--rw-r--r--   0 root         (0) root         (0)     3896 2023-05-18 20:38:07.000000 dagster-airflow-1.3.5/dagster_airflow/dagster_job_factory.py
--rw-r--r--   0 root         (0) root         (0)     1763 2023-05-18 20:38:07.000000 dagster-airflow-1.3.5/dagster_airflow/dagster_schedule_factory.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:48:21.101656 dagster-airflow-1.3.5/dagster_airflow/hooks/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 20:38:07.000000 dagster-airflow-1.3.5/dagster_airflow/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9138 2023-05-18 20:38:07.000000 dagster-airflow-1.3.5/dagster_airflow/hooks/dagster_hook.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:48:21.101656 dagster-airflow-1.3.5/dagster_airflow/links/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 20:38:07.000000 dagster-airflow-1.3.5/dagster_airflow/links/__init__.py
--rw-r--r--   0 root         (0) root         (0)      851 2023-05-18 20:38:07.000000 dagster-airflow-1.3.5/dagster_airflow/links/dagster_link.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:48:21.105656 dagster-airflow-1.3.5/dagster_airflow/operators/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 20:38:07.000000 dagster-airflow-1.3.5/dagster_airflow/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5170 2023-05-18 20:38:07.000000 dagster-airflow-1.3.5/dagster_airflow/operators/dagster_operator.py
--rw-r--r--   0 root         (0) root         (0)      651 2023-05-18 20:38:07.000000 dagster-airflow-1.3.5/dagster_airflow/patch_airflow_example_dag.py
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-18 20:38:07.000000 dagster-airflow-1.3.5/dagster_airflow/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:48:21.105656 dagster-airflow-1.3.5/dagster_airflow/resources/
--rw-r--r--   0 root         (0) root         (0)      324 2023-05-18 20:38:07.000000 dagster-airflow-1.3.5/dagster_airflow/resources/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3966 2023-05-18 20:38:07.000000 dagster-airflow-1.3.5/dagster_airflow/resources/airflow_db.py
--rw-r--r--   0 root         (0) root         (0)     3659 2023-05-18 20:38:07.000000 dagster-airflow-1.3.5/dagster_airflow/resources/airflow_ephemeral_db.py
--rw-r--r--   0 root         (0) root         (0)     4037 2023-05-18 20:38:07.000000 dagster-airflow-1.3.5/dagster_airflow/resources/airflow_persistent_db.py
--rw-r--r--   0 root         (0) root         (0)     4496 2023-05-18 20:38:07.000000 dagster-airflow-1.3.5/dagster_airflow/utils.py
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 20:38:07.000000 dagster-airflow-1.3.5/dagster_airflow/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:48:21.101656 dagster-airflow-1.3.5/dagster_airflow.egg-info/
--rw-r--r--   0 root         (0) root         (0)      649 2023-05-18 20:48:21.000000 dagster-airflow-1.3.5/dagster_airflow.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1041 2023-05-18 20:48:21.000000 dagster-airflow-1.3.5/dagster_airflow.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 20:48:21.000000 dagster-airflow-1.3.5/dagster_airflow.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      168 2023-05-18 20:48:21.000000 dagster-airflow-1.3.5/dagster_airflow.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      469 2023-05-18 20:48:21.000000 dagster-airflow-1.3.5/dagster_airflow.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-05-18 20:48:21.000000 dagster-airflow-1.3.5/dagster_airflow.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      192 2023-05-18 20:48:21.109655 dagster-airflow-1.3.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2637 2023-05-18 20:38:07.000000 dagster-airflow-1.3.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:24:33.217456 dagster-airflow-1.3.6/
+-rw-r--r--   0 root         (0) root         (0)    11344 2023-05-25 17:16:50.000000 dagster-airflow-1.3.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      105 2023-05-25 17:16:50.000000 dagster-airflow-1.3.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      649 2023-05-25 17:24:33.217456 dagster-airflow-1.3.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      131 2023-05-25 17:16:50.000000 dagster-airflow-1.3.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:24:33.209456 dagster-airflow-1.3.6/dagster_airflow/
+-rw-r--r--   0 root         (0) root         (0)     2474 2023-05-25 17:16:50.000000 dagster-airflow-1.3.6/dagster_airflow/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3759 2023-05-25 17:16:50.000000 dagster-airflow-1.3.6/dagster_airflow/airflow_dag_converter.py
+-rw-r--r--   0 root         (0) root         (0)     7716 2023-05-25 17:16:50.000000 dagster-airflow-1.3.6/dagster_airflow/dagster_asset_factory.py
+-rw-r--r--   0 root         (0) root         (0)     8158 2023-05-25 17:16:50.000000 dagster-airflow-1.3.6/dagster_airflow/dagster_factory.py
+-rw-r--r--   0 root         (0) root         (0)     3896 2023-05-25 17:16:50.000000 dagster-airflow-1.3.6/dagster_airflow/dagster_job_factory.py
+-rw-r--r--   0 root         (0) root         (0)     1763 2023-05-25 17:16:50.000000 dagster-airflow-1.3.6/dagster_airflow/dagster_schedule_factory.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:24:33.209456 dagster-airflow-1.3.6/dagster_airflow/hooks/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 17:16:50.000000 dagster-airflow-1.3.6/dagster_airflow/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9138 2023-05-25 17:16:50.000000 dagster-airflow-1.3.6/dagster_airflow/hooks/dagster_hook.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:24:33.213456 dagster-airflow-1.3.6/dagster_airflow/links/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 17:16:50.000000 dagster-airflow-1.3.6/dagster_airflow/links/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      851 2023-05-25 17:16:50.000000 dagster-airflow-1.3.6/dagster_airflow/links/dagster_link.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:24:33.213456 dagster-airflow-1.3.6/dagster_airflow/operators/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 17:16:50.000000 dagster-airflow-1.3.6/dagster_airflow/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5170 2023-05-25 17:16:50.000000 dagster-airflow-1.3.6/dagster_airflow/operators/dagster_operator.py
+-rw-r--r--   0 root         (0) root         (0)      651 2023-05-25 17:16:50.000000 dagster-airflow-1.3.6/dagster_airflow/patch_airflow_example_dag.py
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-25 17:16:50.000000 dagster-airflow-1.3.6/dagster_airflow/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:24:33.217456 dagster-airflow-1.3.6/dagster_airflow/resources/
+-rw-r--r--   0 root         (0) root         (0)      324 2023-05-25 17:16:50.000000 dagster-airflow-1.3.6/dagster_airflow/resources/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3966 2023-05-25 17:16:50.000000 dagster-airflow-1.3.6/dagster_airflow/resources/airflow_db.py
+-rw-r--r--   0 root         (0) root         (0)     3659 2023-05-25 17:16:50.000000 dagster-airflow-1.3.6/dagster_airflow/resources/airflow_ephemeral_db.py
+-rw-r--r--   0 root         (0) root         (0)     4037 2023-05-25 17:16:50.000000 dagster-airflow-1.3.6/dagster_airflow/resources/airflow_persistent_db.py
+-rw-r--r--   0 root         (0) root         (0)     4496 2023-05-25 17:16:50.000000 dagster-airflow-1.3.6/dagster_airflow/utils.py
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-25 17:16:50.000000 dagster-airflow-1.3.6/dagster_airflow/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:24:33.209456 dagster-airflow-1.3.6/dagster_airflow.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      649 2023-05-25 17:24:33.000000 dagster-airflow-1.3.6/dagster_airflow.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1041 2023-05-25 17:24:33.000000 dagster-airflow-1.3.6/dagster_airflow.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 17:24:33.000000 dagster-airflow-1.3.6/dagster_airflow.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      168 2023-05-25 17:24:33.000000 dagster-airflow-1.3.6/dagster_airflow.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      469 2023-05-25 17:24:33.000000 dagster-airflow-1.3.6/dagster_airflow.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-05-25 17:24:33.000000 dagster-airflow-1.3.6/dagster_airflow.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      192 2023-05-25 17:24:33.217456 dagster-airflow-1.3.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2637 2023-05-25 17:16:50.000000 dagster-airflow-1.3.6/setup.py
```

### Comparing `dagster-airflow-1.3.5/LICENSE` & `dagster-airflow-1.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-airflow-1.3.5/PKG-INFO` & `dagster-airflow-1.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-airflow
-Version: 1.3.5
+Version: 1.3.6
 Summary: Airflow plugin for Dagster
 Home-page: https://github.com/dagster-io/dagster
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Project-URL: project-url/documentation, https://docs.dagster.io
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `dagster-airflow-1.3.5/dagster_airflow/__init__.py` & `dagster-airflow-1.3.6/dagster_airflow/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-airflow-1.3.5/dagster_airflow/airflow_dag_converter.py` & `dagster-airflow-1.3.6/dagster_airflow/airflow_dag_converter.py`

 * *Files identical despite different names*

### Comparing `dagster-airflow-1.3.5/dagster_airflow/dagster_asset_factory.py` & `dagster-airflow-1.3.6/dagster_airflow/dagster_asset_factory.py`

 * *Files identical despite different names*

### Comparing `dagster-airflow-1.3.5/dagster_airflow/dagster_factory.py` & `dagster-airflow-1.3.6/dagster_airflow/dagster_factory.py`

 * *Files identical despite different names*

### Comparing `dagster-airflow-1.3.5/dagster_airflow/dagster_job_factory.py` & `dagster-airflow-1.3.6/dagster_airflow/dagster_job_factory.py`

 * *Files identical despite different names*

### Comparing `dagster-airflow-1.3.5/dagster_airflow/dagster_schedule_factory.py` & `dagster-airflow-1.3.6/dagster_airflow/dagster_schedule_factory.py`

 * *Files identical despite different names*

### Comparing `dagster-airflow-1.3.5/dagster_airflow/hooks/dagster_hook.py` & `dagster-airflow-1.3.6/dagster_airflow/hooks/dagster_hook.py`

 * *Files identical despite different names*

### Comparing `dagster-airflow-1.3.5/dagster_airflow/links/dagster_link.py` & `dagster-airflow-1.3.6/dagster_airflow/links/dagster_link.py`

 * *Files identical despite different names*

### Comparing `dagster-airflow-1.3.5/dagster_airflow/operators/dagster_operator.py` & `dagster-airflow-1.3.6/dagster_airflow/operators/dagster_operator.py`

 * *Files identical despite different names*

### Comparing `dagster-airflow-1.3.5/dagster_airflow/patch_airflow_example_dag.py` & `dagster-airflow-1.3.6/dagster_airflow/patch_airflow_example_dag.py`

 * *Files identical despite different names*

### Comparing `dagster-airflow-1.3.5/dagster_airflow/resources/airflow_db.py` & `dagster-airflow-1.3.6/dagster_airflow/resources/airflow_db.py`

 * *Files identical despite different names*

### Comparing `dagster-airflow-1.3.5/dagster_airflow/resources/airflow_ephemeral_db.py` & `dagster-airflow-1.3.6/dagster_airflow/resources/airflow_ephemeral_db.py`

 * *Files identical despite different names*

### Comparing `dagster-airflow-1.3.5/dagster_airflow/resources/airflow_persistent_db.py` & `dagster-airflow-1.3.6/dagster_airflow/resources/airflow_persistent_db.py`

 * *Files identical despite different names*

### Comparing `dagster-airflow-1.3.5/dagster_airflow/utils.py` & `dagster-airflow-1.3.6/dagster_airflow/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-airflow-1.3.5/dagster_airflow.egg-info/PKG-INFO` & `dagster-airflow-1.3.6/dagster_airflow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-airflow
-Version: 1.3.5
+Version: 1.3.6
 Summary: Airflow plugin for Dagster
 Home-page: https://github.com/dagster-io/dagster
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Project-URL: project-url/documentation, https://docs.dagster.io
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `dagster-airflow-1.3.5/dagster_airflow.egg-info/SOURCES.txt` & `dagster-airflow-1.3.6/dagster_airflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagster-airflow-1.3.5/setup.py` & `dagster-airflow-1.3.6/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_airflow_tests*"]),
     install_requires=[
-        "dagster==1.3.5",
+        "dagster==1.3.6",
         "docker>=5.0.3,<6.0.0",
         "lazy_object_proxy",
         "pendulum",
     ],
     project_urls={
         # airflow will embed a link this in the providers page UI
         "project-url/documentation": "https://docs.dagster.io",
```

