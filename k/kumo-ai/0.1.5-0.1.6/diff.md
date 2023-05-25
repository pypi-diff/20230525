# Comparing `tmp/kumo-ai-0.1.5.tar.gz` & `tmp/kumo-ai-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kumo-ai-0.1.5.tar", last modified: Thu May 25 17:49:37 2023, max compression
+gzip compressed data, was "kumo-ai-0.1.6.tar", last modified: Thu May 25 20:14:14 2023, max compression
```

## Comparing `kumo-ai-0.1.5.tar` & `kumo-ai-0.1.6.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 siyang     (501) staff       (20)        0 2023-05-25 17:49:37.197975 kumo-ai-0.1.5/
--rw-r--r--   0 siyang     (501) staff       (20)     1800 2023-02-27 18:06:46.000000 kumo-ai-0.1.5/.gitignore
--rw-r--r--   0 siyang     (501) staff       (20)      933 2023-03-17 21:55:08.000000 kumo-ai-0.1.5/.pre-commit-config.yaml
--rw-r--r--   0 siyang     (501) staff       (20)     1061 2023-02-23 21:09:43.000000 kumo-ai-0.1.5/LICENSE
--rw-r--r--   0 siyang     (501) staff       (20)      161 2023-03-17 21:55:08.000000 kumo-ai-0.1.5/Makefile
--rw-r--r--   0 siyang     (501) staff       (20)      482 2023-05-25 17:49:37.197843 kumo-ai-0.1.5/PKG-INFO
--rw-r--r--   0 siyang     (501) staff       (20)       39 2023-02-23 21:09:43.000000 kumo-ai-0.1.5/README.md
-drwxr-xr-x   0 siyang     (501) staff       (20)        0 2023-05-25 17:49:37.195586 kumo-ai-0.1.5/kumo_ai.egg-info/
--rw-r--r--   0 siyang     (501) staff       (20)      482 2023-05-25 17:49:37.000000 kumo-ai-0.1.5/kumo_ai.egg-info/PKG-INFO
--rw-r--r--   0 siyang     (501) staff       (20)      722 2023-05-25 17:49:37.000000 kumo-ai-0.1.5/kumo_ai.egg-info/SOURCES.txt
--rw-r--r--   0 siyang     (501) staff       (20)        1 2023-05-25 17:49:37.000000 kumo-ai-0.1.5/kumo_ai.egg-info/dependency_links.txt
--rw-r--r--   0 siyang     (501) staff       (20)       34 2023-05-25 17:49:37.000000 kumo-ai-0.1.5/kumo_ai.egg-info/requires.txt
--rw-r--r--   0 siyang     (501) staff       (20)        7 2023-05-25 17:49:37.000000 kumo-ai-0.1.5/kumo_ai.egg-info/top_level.txt
-drwxr-xr-x   0 siyang     (501) staff       (20)        0 2023-05-25 17:49:37.195794 kumo-ai-0.1.5/kumoai/
--rw-r--r--   0 siyang     (501) staff       (20)        0 2023-02-27 18:06:46.000000 kumo-ai-0.1.5/kumoai/__init__.py
--rw-r--r--   0 siyang     (501) staff       (20)    15118 2023-05-25 17:33:50.000000 kumo-ai-0.1.5/kumoai/client.py
-drwxr-xr-x   0 siyang     (501) staff       (20)        0 2023-05-25 17:49:37.196445 kumo-ai-0.1.5/kumoai/datamodel/
--rw-r--r--   0 siyang     (501) staff       (20)        0 2023-02-27 18:06:46.000000 kumo-ai-0.1.5/kumoai/datamodel/__init__.py
--rw-r--r--   0 siyang     (501) staff       (20)      974 2023-04-03 17:42:04.000000 kumo-ai-0.1.5/kumoai/datamodel/data_source.py
--rw-r--r--   0 siyang     (501) staff       (20)     6467 2023-05-24 19:47:25.000000 kumo-ai-0.1.5/kumoai/datamodel/jobs.py
--rw-r--r--   0 siyang     (501) staff       (20)      561 2023-04-05 16:11:01.000000 kumo-ai-0.1.5/kumoai/datamodel/json_serde.py
--rw-r--r--   0 siyang     (501) staff       (20)     6471 2023-05-24 04:53:09.000000 kumo-ai-0.1.5/kumoai/datamodel/pquery.py
-drwxr-xr-x   0 siyang     (501) staff       (20)        0 2023-05-25 17:49:37.197667 kumo-ai-0.1.5/kumoai/examples/
--rw-r--r--   0 siyang     (501) staff       (20)        0 2023-03-29 16:49:40.000000 kumo-ai-0.1.5/kumoai/examples/__init__.py
--rw-r--r--   0 siyang     (501) staff       (20)     4807 2023-05-18 17:13:05.000000 kumo-ai-0.1.5/kumoai/examples/financial.py
--rw-r--r--   0 siyang     (501) staff       (20)     8950 2023-05-12 16:27:03.000000 kumo-ai-0.1.5/kumoai/examples/financial_binary_classify_S3.json
--rw-r--r--   0 siyang     (501) staff       (20)     9339 2023-04-04 17:45:36.000000 kumo-ai-0.1.5/kumoai/examples/financial_binary_classify_SNOWFLAKE.json
--rw-r--r--   0 siyang     (501) staff       (20)     5373 2023-03-29 17:21:11.000000 kumo-ai-0.1.5/kumoai/examples/hm_churn.json
--rw-r--r--   0 siyang     (501) staff       (20)     3080 2023-05-18 17:13:05.000000 kumo-ai-0.1.5/kumoai/examples/orchestration.py
--rw-r--r--   0 siyang     (501) staff       (20)     3434 2023-05-18 17:13:05.000000 kumo-ai-0.1.5/kumoai/examples/save_load_modify_pquery.py
--rw-r--r--   0 siyang     (501) staff       (20)      967 2023-05-18 17:51:43.000000 kumo-ai-0.1.5/precommit-pyrightconfig.json
--rw-r--r--   0 siyang     (501) staff       (20)      924 2023-05-18 17:52:10.000000 kumo-ai-0.1.5/pyrightconfig.json
--rw-r--r--   0 siyang     (501) staff       (20)       38 2023-05-25 17:49:37.198022 kumo-ai-0.1.5/setup.cfg
--rw-r--r--   0 siyang     (501) staff       (20)      885 2023-05-25 17:49:20.000000 kumo-ai-0.1.5/setup.py
+drwxr-xr-x   0 siyang     (501) staff       (20)        0 2023-05-25 20:14:14.382582 kumo-ai-0.1.6/
+-rw-r--r--   0 siyang     (501) staff       (20)     1800 2023-02-27 18:06:46.000000 kumo-ai-0.1.6/.gitignore
+-rw-r--r--   0 siyang     (501) staff       (20)      933 2023-03-17 21:55:08.000000 kumo-ai-0.1.6/.pre-commit-config.yaml
+-rw-r--r--   0 siyang     (501) staff       (20)     1061 2023-02-23 21:09:43.000000 kumo-ai-0.1.6/LICENSE
+-rw-r--r--   0 siyang     (501) staff       (20)      175 2023-05-25 20:13:16.000000 kumo-ai-0.1.6/Makefile
+-rw-r--r--   0 siyang     (501) staff       (20)      482 2023-05-25 20:14:14.382440 kumo-ai-0.1.6/PKG-INFO
+-rw-r--r--   0 siyang     (501) staff       (20)       39 2023-02-23 21:09:43.000000 kumo-ai-0.1.6/README.md
+drwxr-xr-x   0 siyang     (501) staff       (20)        0 2023-05-25 20:14:14.380254 kumo-ai-0.1.6/kumo_ai.egg-info/
+-rw-r--r--   0 siyang     (501) staff       (20)      482 2023-05-25 20:14:14.000000 kumo-ai-0.1.6/kumo_ai.egg-info/PKG-INFO
+-rw-r--r--   0 siyang     (501) staff       (20)      722 2023-05-25 20:14:14.000000 kumo-ai-0.1.6/kumo_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 siyang     (501) staff       (20)        1 2023-05-25 20:14:14.000000 kumo-ai-0.1.6/kumo_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 siyang     (501) staff       (20)       34 2023-05-25 20:14:14.000000 kumo-ai-0.1.6/kumo_ai.egg-info/requires.txt
+-rw-r--r--   0 siyang     (501) staff       (20)        7 2023-05-25 20:14:14.000000 kumo-ai-0.1.6/kumo_ai.egg-info/top_level.txt
+drwxr-xr-x   0 siyang     (501) staff       (20)        0 2023-05-25 20:14:14.380727 kumo-ai-0.1.6/kumoai/
+-rw-r--r--   0 siyang     (501) staff       (20)        0 2023-02-27 18:06:46.000000 kumo-ai-0.1.6/kumoai/__init__.py
+-rw-r--r--   0 siyang     (501) staff       (20)    15118 2023-05-25 17:33:50.000000 kumo-ai-0.1.6/kumoai/client.py
+drwxr-xr-x   0 siyang     (501) staff       (20)        0 2023-05-25 20:14:14.381428 kumo-ai-0.1.6/kumoai/datamodel/
+-rw-r--r--   0 siyang     (501) staff       (20)        0 2023-02-27 18:06:46.000000 kumo-ai-0.1.6/kumoai/datamodel/__init__.py
+-rw-r--r--   0 siyang     (501) staff       (20)      974 2023-04-03 17:42:04.000000 kumo-ai-0.1.6/kumoai/datamodel/data_source.py
+-rw-r--r--   0 siyang     (501) staff       (20)     6467 2023-05-24 19:47:25.000000 kumo-ai-0.1.6/kumoai/datamodel/jobs.py
+-rw-r--r--   0 siyang     (501) staff       (20)      561 2023-04-05 16:11:01.000000 kumo-ai-0.1.6/kumoai/datamodel/json_serde.py
+-rw-r--r--   0 siyang     (501) staff       (20)     6471 2023-05-24 04:53:09.000000 kumo-ai-0.1.6/kumoai/datamodel/pquery.py
+drwxr-xr-x   0 siyang     (501) staff       (20)        0 2023-05-25 20:14:14.382249 kumo-ai-0.1.6/kumoai/examples/
+-rw-r--r--   0 siyang     (501) staff       (20)        0 2023-03-29 16:49:40.000000 kumo-ai-0.1.6/kumoai/examples/__init__.py
+-rw-r--r--   0 siyang     (501) staff       (20)     4807 2023-05-18 17:13:05.000000 kumo-ai-0.1.6/kumoai/examples/financial.py
+-rw-r--r--   0 siyang     (501) staff       (20)     8950 2023-05-12 16:27:03.000000 kumo-ai-0.1.6/kumoai/examples/financial_binary_classify_S3.json
+-rw-r--r--   0 siyang     (501) staff       (20)     9339 2023-04-04 17:45:36.000000 kumo-ai-0.1.6/kumoai/examples/financial_binary_classify_SNOWFLAKE.json
+-rw-r--r--   0 siyang     (501) staff       (20)     5373 2023-03-29 17:21:11.000000 kumo-ai-0.1.6/kumoai/examples/hm_churn.json
+-rw-r--r--   0 siyang     (501) staff       (20)     3080 2023-05-18 17:13:05.000000 kumo-ai-0.1.6/kumoai/examples/orchestration.py
+-rw-r--r--   0 siyang     (501) staff       (20)     3434 2023-05-18 17:13:05.000000 kumo-ai-0.1.6/kumoai/examples/save_load_modify_pquery.py
+-rw-r--r--   0 siyang     (501) staff       (20)      967 2023-05-18 17:51:43.000000 kumo-ai-0.1.6/precommit-pyrightconfig.json
+-rw-r--r--   0 siyang     (501) staff       (20)      924 2023-05-18 17:52:10.000000 kumo-ai-0.1.6/pyrightconfig.json
+-rw-r--r--   0 siyang     (501) staff       (20)       38 2023-05-25 20:14:14.382623 kumo-ai-0.1.6/setup.cfg
+-rw-r--r--   0 siyang     (501) staff       (20)      885 2023-05-25 20:12:49.000000 kumo-ai-0.1.6/setup.py
```

### Comparing `kumo-ai-0.1.5/.gitignore` & `kumo-ai-0.1.6/.gitignore`

 * *Files identical despite different names*

### Comparing `kumo-ai-0.1.5/.pre-commit-config.yaml` & `kumo-ai-0.1.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `kumo-ai-0.1.5/LICENSE` & `kumo-ai-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `kumo-ai-0.1.5/kumo_ai.egg-info/SOURCES.txt` & `kumo-ai-0.1.6/kumo_ai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kumo-ai-0.1.5/kumoai/client.py` & `kumo-ai-0.1.6/kumoai/client.py`

 * *Files identical despite different names*

### Comparing `kumo-ai-0.1.5/kumoai/datamodel/data_source.py` & `kumo-ai-0.1.6/kumoai/datamodel/data_source.py`

 * *Files identical despite different names*

### Comparing `kumo-ai-0.1.5/kumoai/datamodel/jobs.py` & `kumo-ai-0.1.6/kumoai/datamodel/jobs.py`

 * *Files identical despite different names*

### Comparing `kumo-ai-0.1.5/kumoai/datamodel/json_serde.py` & `kumo-ai-0.1.6/kumoai/datamodel/json_serde.py`

 * *Files identical despite different names*

### Comparing `kumo-ai-0.1.5/kumoai/datamodel/pquery.py` & `kumo-ai-0.1.6/kumoai/datamodel/pquery.py`

 * *Files identical despite different names*

### Comparing `kumo-ai-0.1.5/kumoai/examples/financial.py` & `kumo-ai-0.1.6/kumoai/examples/financial.py`

 * *Files identical despite different names*

### Comparing `kumo-ai-0.1.5/kumoai/examples/financial_binary_classify_S3.json` & `kumo-ai-0.1.6/kumoai/examples/financial_binary_classify_S3.json`

 * *Files identical despite different names*

### Comparing `kumo-ai-0.1.5/kumoai/examples/financial_binary_classify_SNOWFLAKE.json` & `kumo-ai-0.1.6/kumoai/examples/financial_binary_classify_SNOWFLAKE.json`

 * *Files identical despite different names*

### Comparing `kumo-ai-0.1.5/kumoai/examples/hm_churn.json` & `kumo-ai-0.1.6/kumoai/examples/hm_churn.json`

 * *Files identical despite different names*

### Comparing `kumo-ai-0.1.5/kumoai/examples/orchestration.py` & `kumo-ai-0.1.6/kumoai/examples/orchestration.py`

 * *Files identical despite different names*

### Comparing `kumo-ai-0.1.5/kumoai/examples/save_load_modify_pquery.py` & `kumo-ai-0.1.6/kumoai/examples/save_load_modify_pquery.py`

 * *Files identical despite different names*

### Comparing `kumo-ai-0.1.5/precommit-pyrightconfig.json` & `kumo-ai-0.1.6/precommit-pyrightconfig.json`

 * *Files identical despite different names*

### Comparing `kumo-ai-0.1.5/pyrightconfig.json` & `kumo-ai-0.1.6/pyrightconfig.json`

 * *Files identical despite different names*

### Comparing `kumo-ai-0.1.5/setup.py` & `kumo-ai-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import find_packages, setup
 
-VERSION = '0.1.5'
+VERSION = '0.1.6'
 DESCRIPTION = 'Kumo.ai Client SDK'
 LONG_DESCRIPTION = """
 SDK/API for Kumo.ai clients to allow programmatic access to Kumo.ai
 """
 
 install_requires = [
     "pydantic==1.10.4",
```

