# Comparing `tmp/kumo-ai-0.1.3.tar.gz` & `tmp/kumo-ai-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kumo-ai-0.1.3.tar", last modified: Tue May 23 18:31:12 2023, max compression
+gzip compressed data, was "kumo-ai-0.1.4.tar", last modified: Thu May 25 04:14:26 2023, max compression
```

## Comparing `kumo-ai-0.1.3.tar` & `kumo-ai-0.1.4.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 siyang     (501) staff       (20)        0 2023-05-23 18:31:12.285743 kumo-ai-0.1.3/
--rw-r--r--   0 siyang     (501) staff       (20)     1800 2023-02-27 18:06:46.000000 kumo-ai-0.1.3/.gitignore
--rw-r--r--   0 siyang     (501) staff       (20)      933 2023-03-17 21:55:08.000000 kumo-ai-0.1.3/.pre-commit-config.yaml
--rw-r--r--   0 siyang     (501) staff       (20)     1061 2023-02-23 21:09:43.000000 kumo-ai-0.1.3/LICENSE
--rw-r--r--   0 siyang     (501) staff       (20)      161 2023-03-17 21:55:08.000000 kumo-ai-0.1.3/Makefile
--rw-r--r--   0 siyang     (501) staff       (20)      482 2023-05-23 18:31:12.285605 kumo-ai-0.1.3/PKG-INFO
--rw-r--r--   0 siyang     (501) staff       (20)       39 2023-02-23 21:09:43.000000 kumo-ai-0.1.3/README.md
-drwxr-xr-x   0 siyang     (501) staff       (20)        0 2023-05-23 18:31:12.282997 kumo-ai-0.1.3/kumo_ai.egg-info/
--rw-r--r--   0 siyang     (501) staff       (20)      482 2023-05-23 18:31:12.000000 kumo-ai-0.1.3/kumo_ai.egg-info/PKG-INFO
--rw-r--r--   0 siyang     (501) staff       (20)      722 2023-05-23 18:31:12.000000 kumo-ai-0.1.3/kumo_ai.egg-info/SOURCES.txt
--rw-r--r--   0 siyang     (501) staff       (20)        1 2023-05-23 18:31:12.000000 kumo-ai-0.1.3/kumo_ai.egg-info/dependency_links.txt
--rw-r--r--   0 siyang     (501) staff       (20)       34 2023-05-23 18:31:12.000000 kumo-ai-0.1.3/kumo_ai.egg-info/requires.txt
--rw-r--r--   0 siyang     (501) staff       (20)        7 2023-05-23 18:31:12.000000 kumo-ai-0.1.3/kumo_ai.egg-info/top_level.txt
-drwxr-xr-x   0 siyang     (501) staff       (20)        0 2023-05-23 18:31:12.283342 kumo-ai-0.1.3/kumoai/
--rw-r--r--   0 siyang     (501) staff       (20)        0 2023-02-27 18:06:46.000000 kumo-ai-0.1.3/kumoai/__init__.py
--rw-r--r--   0 siyang     (501) staff       (20)    11086 2023-05-23 18:23:16.000000 kumo-ai-0.1.3/kumoai/client.py
-drwxr-xr-x   0 siyang     (501) staff       (20)        0 2023-05-23 18:31:12.283992 kumo-ai-0.1.3/kumoai/datamodel/
--rw-r--r--   0 siyang     (501) staff       (20)        0 2023-02-27 18:06:46.000000 kumo-ai-0.1.3/kumoai/datamodel/__init__.py
--rw-r--r--   0 siyang     (501) staff       (20)      974 2023-04-03 17:42:04.000000 kumo-ai-0.1.3/kumoai/datamodel/data_source.py
--rw-r--r--   0 siyang     (501) staff       (20)     6355 2023-05-23 18:15:25.000000 kumo-ai-0.1.3/kumoai/datamodel/jobs.py
--rw-r--r--   0 siyang     (501) staff       (20)      561 2023-04-05 16:11:01.000000 kumo-ai-0.1.3/kumoai/datamodel/json_serde.py
--rw-r--r--   0 siyang     (501) staff       (20)     6471 2023-05-23 18:02:40.000000 kumo-ai-0.1.3/kumoai/datamodel/pquery.py
-drwxr-xr-x   0 siyang     (501) staff       (20)        0 2023-05-23 18:31:12.285434 kumo-ai-0.1.3/kumoai/examples/
--rw-r--r--   0 siyang     (501) staff       (20)        0 2023-03-29 16:49:40.000000 kumo-ai-0.1.3/kumoai/examples/__init__.py
--rw-r--r--   0 siyang     (501) staff       (20)     4807 2023-05-18 17:13:05.000000 kumo-ai-0.1.3/kumoai/examples/financial.py
--rw-r--r--   0 siyang     (501) staff       (20)     8950 2023-05-12 16:27:03.000000 kumo-ai-0.1.3/kumoai/examples/financial_binary_classify_S3.json
--rw-r--r--   0 siyang     (501) staff       (20)     9339 2023-04-04 17:45:36.000000 kumo-ai-0.1.3/kumoai/examples/financial_binary_classify_SNOWFLAKE.json
--rw-r--r--   0 siyang     (501) staff       (20)     5373 2023-03-29 17:21:11.000000 kumo-ai-0.1.3/kumoai/examples/hm_churn.json
--rw-r--r--   0 siyang     (501) staff       (20)     3080 2023-05-18 17:13:05.000000 kumo-ai-0.1.3/kumoai/examples/orchestration.py
--rw-r--r--   0 siyang     (501) staff       (20)     3434 2023-05-18 17:13:05.000000 kumo-ai-0.1.3/kumoai/examples/save_load_modify_pquery.py
--rw-r--r--   0 siyang     (501) staff       (20)      967 2023-05-18 17:51:43.000000 kumo-ai-0.1.3/precommit-pyrightconfig.json
--rw-r--r--   0 siyang     (501) staff       (20)      924 2023-05-18 17:52:10.000000 kumo-ai-0.1.3/pyrightconfig.json
--rw-r--r--   0 siyang     (501) staff       (20)       38 2023-05-23 18:31:12.285783 kumo-ai-0.1.3/setup.cfg
--rw-r--r--   0 siyang     (501) staff       (20)      885 2023-05-23 18:30:31.000000 kumo-ai-0.1.3/setup.py
+drwxr-xr-x   0 siyang     (501) staff       (20)        0 2023-05-25 04:14:26.089274 kumo-ai-0.1.4/
+-rw-r--r--   0 siyang     (501) staff       (20)     1800 2023-02-27 18:06:46.000000 kumo-ai-0.1.4/.gitignore
+-rw-r--r--   0 siyang     (501) staff       (20)      933 2023-03-17 21:55:08.000000 kumo-ai-0.1.4/.pre-commit-config.yaml
+-rw-r--r--   0 siyang     (501) staff       (20)     1061 2023-02-23 21:09:43.000000 kumo-ai-0.1.4/LICENSE
+-rw-r--r--   0 siyang     (501) staff       (20)      161 2023-03-17 21:55:08.000000 kumo-ai-0.1.4/Makefile
+-rw-r--r--   0 siyang     (501) staff       (20)      482 2023-05-25 04:14:26.089144 kumo-ai-0.1.4/PKG-INFO
+-rw-r--r--   0 siyang     (501) staff       (20)       39 2023-02-23 21:09:43.000000 kumo-ai-0.1.4/README.md
+drwxr-xr-x   0 siyang     (501) staff       (20)        0 2023-05-25 04:14:26.087273 kumo-ai-0.1.4/kumo_ai.egg-info/
+-rw-r--r--   0 siyang     (501) staff       (20)      482 2023-05-25 04:14:26.000000 kumo-ai-0.1.4/kumo_ai.egg-info/PKG-INFO
+-rw-r--r--   0 siyang     (501) staff       (20)      722 2023-05-25 04:14:26.000000 kumo-ai-0.1.4/kumo_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 siyang     (501) staff       (20)        1 2023-05-25 04:14:26.000000 kumo-ai-0.1.4/kumo_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 siyang     (501) staff       (20)       34 2023-05-25 04:14:26.000000 kumo-ai-0.1.4/kumo_ai.egg-info/requires.txt
+-rw-r--r--   0 siyang     (501) staff       (20)        7 2023-05-25 04:14:26.000000 kumo-ai-0.1.4/kumo_ai.egg-info/top_level.txt
+drwxr-xr-x   0 siyang     (501) staff       (20)        0 2023-05-25 04:14:26.087482 kumo-ai-0.1.4/kumoai/
+-rw-r--r--   0 siyang     (501) staff       (20)        0 2023-02-27 18:06:46.000000 kumo-ai-0.1.4/kumoai/__init__.py
+-rw-r--r--   0 siyang     (501) staff       (20)    15096 2023-05-24 23:57:44.000000 kumo-ai-0.1.4/kumoai/client.py
+drwxr-xr-x   0 siyang     (501) staff       (20)        0 2023-05-25 04:14:26.088084 kumo-ai-0.1.4/kumoai/datamodel/
+-rw-r--r--   0 siyang     (501) staff       (20)        0 2023-02-27 18:06:46.000000 kumo-ai-0.1.4/kumoai/datamodel/__init__.py
+-rw-r--r--   0 siyang     (501) staff       (20)      974 2023-04-03 17:42:04.000000 kumo-ai-0.1.4/kumoai/datamodel/data_source.py
+-rw-r--r--   0 siyang     (501) staff       (20)     6467 2023-05-24 19:47:25.000000 kumo-ai-0.1.4/kumoai/datamodel/jobs.py
+-rw-r--r--   0 siyang     (501) staff       (20)      561 2023-04-05 16:11:01.000000 kumo-ai-0.1.4/kumoai/datamodel/json_serde.py
+-rw-r--r--   0 siyang     (501) staff       (20)     6471 2023-05-24 04:53:09.000000 kumo-ai-0.1.4/kumoai/datamodel/pquery.py
+drwxr-xr-x   0 siyang     (501) staff       (20)        0 2023-05-25 04:14:26.088954 kumo-ai-0.1.4/kumoai/examples/
+-rw-r--r--   0 siyang     (501) staff       (20)        0 2023-03-29 16:49:40.000000 kumo-ai-0.1.4/kumoai/examples/__init__.py
+-rw-r--r--   0 siyang     (501) staff       (20)     4807 2023-05-18 17:13:05.000000 kumo-ai-0.1.4/kumoai/examples/financial.py
+-rw-r--r--   0 siyang     (501) staff       (20)     8950 2023-05-12 16:27:03.000000 kumo-ai-0.1.4/kumoai/examples/financial_binary_classify_S3.json
+-rw-r--r--   0 siyang     (501) staff       (20)     9339 2023-04-04 17:45:36.000000 kumo-ai-0.1.4/kumoai/examples/financial_binary_classify_SNOWFLAKE.json
+-rw-r--r--   0 siyang     (501) staff       (20)     5373 2023-03-29 17:21:11.000000 kumo-ai-0.1.4/kumoai/examples/hm_churn.json
+-rw-r--r--   0 siyang     (501) staff       (20)     3080 2023-05-18 17:13:05.000000 kumo-ai-0.1.4/kumoai/examples/orchestration.py
+-rw-r--r--   0 siyang     (501) staff       (20)     3434 2023-05-18 17:13:05.000000 kumo-ai-0.1.4/kumoai/examples/save_load_modify_pquery.py
+-rw-r--r--   0 siyang     (501) staff       (20)      967 2023-05-18 17:51:43.000000 kumo-ai-0.1.4/precommit-pyrightconfig.json
+-rw-r--r--   0 siyang     (501) staff       (20)      924 2023-05-18 17:52:10.000000 kumo-ai-0.1.4/pyrightconfig.json
+-rw-r--r--   0 siyang     (501) staff       (20)       38 2023-05-25 04:14:26.089316 kumo-ai-0.1.4/setup.cfg
+-rw-r--r--   0 siyang     (501) staff       (20)      885 2023-05-25 04:14:10.000000 kumo-ai-0.1.4/setup.py
```

### Comparing `kumo-ai-0.1.3/.gitignore` & `kumo-ai-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `kumo-ai-0.1.3/.pre-commit-config.yaml` & `kumo-ai-0.1.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `kumo-ai-0.1.3/LICENSE` & `kumo-ai-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `kumo-ai-0.1.3/kumo_ai.egg-info/SOURCES.txt` & `kumo-ai-0.1.4/kumo_ai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kumo-ai-0.1.3/kumoai/datamodel/data_source.py` & `kumo-ai-0.1.4/kumoai/datamodel/data_source.py`

 * *Files identical despite different names*

### Comparing `kumo-ai-0.1.3/kumoai/datamodel/jobs.py` & `kumo-ai-0.1.4/kumoai/datamodel/jobs.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,14 +7,19 @@
 from pydantic import Field, validator
 from pydantic.dataclasses import dataclass
 from typing_extensions import Annotated
 
 logger = logging.getLogger(__name__)
 
 
+class JobType(str, Enum):
+    TRAINING_JOB = "TRAINING_JOB"
+    BATCH_PREDICTION_JOB = "BATCH_PREDICTION_JOB"
+
+
 # Execution status of a Training or Batch Prediction job.
 class JobStatus(Enum):
     # Job has been submitted and is currently running.
     RUNNING = 'RUNNING'
 
     # Terminal status:
     DONE = 'DONE'  # Job has completed successfully
```

### Comparing `kumo-ai-0.1.3/kumoai/datamodel/json_serde.py` & `kumo-ai-0.1.4/kumoai/datamodel/json_serde.py`

 * *Files identical despite different names*

### Comparing `kumo-ai-0.1.3/kumoai/datamodel/pquery.py` & `kumo-ai-0.1.4/kumoai/datamodel/pquery.py`

 * *Files identical despite different names*

### Comparing `kumo-ai-0.1.3/kumoai/examples/financial.py` & `kumo-ai-0.1.4/kumoai/examples/financial.py`

 * *Files identical despite different names*

### Comparing `kumo-ai-0.1.3/kumoai/examples/financial_binary_classify_S3.json` & `kumo-ai-0.1.4/kumoai/examples/financial_binary_classify_S3.json`

 * *Files identical despite different names*

### Comparing `kumo-ai-0.1.3/kumoai/examples/financial_binary_classify_SNOWFLAKE.json` & `kumo-ai-0.1.4/kumoai/examples/financial_binary_classify_SNOWFLAKE.json`

 * *Files identical despite different names*

### Comparing `kumo-ai-0.1.3/kumoai/examples/hm_churn.json` & `kumo-ai-0.1.4/kumoai/examples/hm_churn.json`

 * *Files identical despite different names*

### Comparing `kumo-ai-0.1.3/kumoai/examples/orchestration.py` & `kumo-ai-0.1.4/kumoai/examples/orchestration.py`

 * *Files identical despite different names*

### Comparing `kumo-ai-0.1.3/kumoai/examples/save_load_modify_pquery.py` & `kumo-ai-0.1.4/kumoai/examples/save_load_modify_pquery.py`

 * *Files identical despite different names*

### Comparing `kumo-ai-0.1.3/precommit-pyrightconfig.json` & `kumo-ai-0.1.4/precommit-pyrightconfig.json`

 * *Files identical despite different names*

### Comparing `kumo-ai-0.1.3/pyrightconfig.json` & `kumo-ai-0.1.4/pyrightconfig.json`

 * *Files identical despite different names*

### Comparing `kumo-ai-0.1.3/setup.py` & `kumo-ai-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import find_packages, setup
 
-VERSION = '0.1.3'
+VERSION = '0.1.4'
 DESCRIPTION = 'Kumo.ai Client SDK'
 LONG_DESCRIPTION = """
 SDK/API for Kumo.ai clients to allow programmatic access to Kumo.ai
 """
 
 install_requires = [
     "pydantic==1.10.4",
```

