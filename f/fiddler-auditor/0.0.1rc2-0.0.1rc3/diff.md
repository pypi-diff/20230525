# Comparing `tmp/fiddler-auditor-0.0.1rc2.tar.gz` & `tmp/fiddler-auditor-0.0.1rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fiddler-auditor-0.0.1rc2.tar", last modified: Tue May 23 07:05:26 2023, max compression
+gzip compressed data, was "fiddler-auditor-0.0.1rc3.tar", last modified: Thu May 25 01:17:47 2023, max compression
```

## Comparing `fiddler-auditor-0.0.1rc2.tar` & `fiddler-auditor-0.0.1rc3.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:05:26.873343 fiddler-auditor-0.0.1rc2/
--rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-05-23 07:00:44.000000 fiddler-auditor-0.0.1rc2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-05-23 07:05:26.873343 fiddler-auditor-0.0.1rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-05-23 07:00:44.000000 fiddler-auditor-0.0.1rc2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:05:26.853343 fiddler-auditor-0.0.1rc2/auditor/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-23 07:00:44.000000 fiddler-auditor-0.0.1rc2/auditor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:05:26.849343 fiddler-auditor-0.0.1rc2/auditor/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:05:26.857343 fiddler-auditor-0.0.1rc2/auditor/assets/data/
--rw-r--r--   0 runner    (1001) docker     (123)    43309 2023-05-23 07:00:44.000000 fiddler-auditor-0.0.1rc2/auditor/assets/data/snips_dataset_dev.csv
--rw-r--r--   0 runner    (1001) docker     (123)    43115 2023-05-23 07:00:44.000000 fiddler-auditor-0.0.1rc2/auditor/assets/data/snips_dataset_test.csv
--rw-r--r--   0 runner    (1001) docker     (123)   798933 2023-05-23 07:00:44.000000 fiddler-auditor-0.0.1rc2/auditor/assets/data/snips_dataset_train.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:05:26.861343 fiddler-auditor-0.0.1rc2/auditor/evaluation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 07:00:44.000000 fiddler-auditor-0.0.1rc2/auditor/evaluation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8024 2023-05-23 07:00:44.000000 fiddler-auditor-0.0.1rc2/auditor/evaluation/discriminative.py
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-23 07:00:44.000000 fiddler-auditor-0.0.1rc2/auditor/evaluation/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-05-23 07:00:44.000000 fiddler-auditor-0.0.1rc2/auditor/evaluation/expected_behavior.py
--rw-r--r--   0 runner    (1001) docker     (123)    10204 2023-05-23 07:00:44.000000 fiddler-auditor-0.0.1rc2/auditor/evaluation/generative.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:05:26.861343 fiddler-auditor-0.0.1rc2/auditor/generations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 07:00:44.000000 fiddler-auditor-0.0.1rc2/auditor/generations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-23 07:00:44.000000 fiddler-auditor-0.0.1rc2/auditor/generations/paraphrase.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:05:26.865343 fiddler-auditor-0.0.1rc2/auditor/perturbations/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-23 07:00:44.000000 fiddler-auditor-0.0.1rc2/auditor/perturbations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-23 07:00:44.000000 fiddler-auditor-0.0.1rc2/auditor/perturbations/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    10348 2023-05-23 07:00:44.000000 fiddler-auditor-0.0.1rc2/auditor/perturbations/text.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:05:26.865343 fiddler-auditor-0.0.1rc2/auditor/reporting/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-23 07:00:44.000000 fiddler-auditor-0.0.1rc2/auditor/reporting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-05-23 07:00:44.000000 fiddler-auditor-0.0.1rc2/auditor/reporting/generate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:05:26.865343 fiddler-auditor-0.0.1rc2/auditor/reporting/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     6384 2023-05-23 07:00:44.000000 fiddler-auditor-0.0.1rc2/auditor/reporting/templates/report_template.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:05:26.869343 fiddler-auditor-0.0.1rc2/auditor/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 07:00:44.000000 fiddler-auditor-0.0.1rc2/auditor/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10571 2023-05-23 07:00:44.000000 fiddler-auditor-0.0.1rc2/auditor/utils/data.py
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-23 07:00:44.000000 fiddler-auditor-0.0.1rc2/auditor/utils/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-23 07:00:44.000000 fiddler-auditor-0.0.1rc2/auditor/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-23 07:00:44.000000 fiddler-auditor-0.0.1rc2/auditor/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-23 07:00:44.000000 fiddler-auditor-0.0.1rc2/auditor/utils/similarity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:05:26.869343 fiddler-auditor-0.0.1rc2/fiddler_auditor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-05-23 07:05:26.000000 fiddler-auditor-0.0.1rc2/fiddler_auditor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-23 07:05:26.000000 fiddler-auditor-0.0.1rc2/fiddler_auditor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 07:05:26.000000 fiddler-auditor-0.0.1rc2/fiddler_auditor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-23 07:05:26.000000 fiddler-auditor-0.0.1rc2/fiddler_auditor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-23 07:05:26.000000 fiddler-auditor-0.0.1rc2/fiddler_auditor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-23 07:00:44.000000 fiddler-auditor-0.0.1rc2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 07:05:26.873343 fiddler-auditor-0.0.1rc2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:05:26.873343 fiddler-auditor-0.0.1rc2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-05-23 07:00:44.000000 fiddler-auditor-0.0.1rc2/tests/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-05-23 07:00:44.000000 fiddler-auditor-0.0.1rc2/tests/test_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4694 2023-05-23 07:00:44.000000 fiddler-auditor-0.0.1rc2/tests/test_llm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-23 07:00:44.000000 fiddler-auditor-0.0.1rc2/tests/test_perturbations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 01:17:47.778644 fiddler-auditor-0.0.1rc3/
+-rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-05-25 01:14:17.000000 fiddler-auditor-0.0.1rc3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-05-25 01:17:47.778644 fiddler-auditor-0.0.1rc3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-05-25 01:14:17.000000 fiddler-auditor-0.0.1rc3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 01:17:47.766644 fiddler-auditor-0.0.1rc3/auditor/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-25 01:14:17.000000 fiddler-auditor-0.0.1rc3/auditor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 01:17:47.766644 fiddler-auditor-0.0.1rc3/auditor/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 01:17:47.766644 fiddler-auditor-0.0.1rc3/auditor/assets/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    43309 2023-05-25 01:14:17.000000 fiddler-auditor-0.0.1rc3/auditor/assets/data/snips_dataset_dev.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    43115 2023-05-25 01:14:17.000000 fiddler-auditor-0.0.1rc3/auditor/assets/data/snips_dataset_test.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   798933 2023-05-25 01:14:17.000000 fiddler-auditor-0.0.1rc3/auditor/assets/data/snips_dataset_train.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 01:17:47.770644 fiddler-auditor-0.0.1rc3/auditor/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 01:14:17.000000 fiddler-auditor-0.0.1rc3/auditor/evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8024 2023-05-25 01:14:17.000000 fiddler-auditor-0.0.1rc3/auditor/evaluation/discriminative.py
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-25 01:14:17.000000 fiddler-auditor-0.0.1rc3/auditor/evaluation/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-05-25 01:14:17.000000 fiddler-auditor-0.0.1rc3/auditor/evaluation/expected_behavior.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10204 2023-05-25 01:14:17.000000 fiddler-auditor-0.0.1rc3/auditor/evaluation/generative.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 01:17:47.770644 fiddler-auditor-0.0.1rc3/auditor/generations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 01:14:17.000000 fiddler-auditor-0.0.1rc3/auditor/generations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-25 01:14:17.000000 fiddler-auditor-0.0.1rc3/auditor/generations/paraphrase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 01:17:47.770644 fiddler-auditor-0.0.1rc3/auditor/perturbations/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-25 01:14:17.000000 fiddler-auditor-0.0.1rc3/auditor/perturbations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-25 01:14:17.000000 fiddler-auditor-0.0.1rc3/auditor/perturbations/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10348 2023-05-25 01:14:17.000000 fiddler-auditor-0.0.1rc3/auditor/perturbations/text.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 01:17:47.770644 fiddler-auditor-0.0.1rc3/auditor/reporting/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-25 01:14:17.000000 fiddler-auditor-0.0.1rc3/auditor/reporting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-05-25 01:14:17.000000 fiddler-auditor-0.0.1rc3/auditor/reporting/generate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 01:17:47.770644 fiddler-auditor-0.0.1rc3/auditor/reporting/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     6384 2023-05-25 01:14:17.000000 fiddler-auditor-0.0.1rc3/auditor/reporting/templates/report_template.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 01:17:47.770644 fiddler-auditor-0.0.1rc3/auditor/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 01:14:17.000000 fiddler-auditor-0.0.1rc3/auditor/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10571 2023-05-25 01:14:17.000000 fiddler-auditor-0.0.1rc3/auditor/utils/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-25 01:14:17.000000 fiddler-auditor-0.0.1rc3/auditor/utils/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-25 01:14:17.000000 fiddler-auditor-0.0.1rc3/auditor/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-25 01:14:17.000000 fiddler-auditor-0.0.1rc3/auditor/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-25 01:14:17.000000 fiddler-auditor-0.0.1rc3/auditor/utils/similarity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 01:17:47.770644 fiddler-auditor-0.0.1rc3/fiddler_auditor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-05-25 01:17:47.000000 fiddler-auditor-0.0.1rc3/fiddler_auditor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-25 01:17:47.000000 fiddler-auditor-0.0.1rc3/fiddler_auditor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 01:17:47.000000 fiddler-auditor-0.0.1rc3/fiddler_auditor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-25 01:17:47.000000 fiddler-auditor-0.0.1rc3/fiddler_auditor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-25 01:17:47.000000 fiddler-auditor-0.0.1rc3/fiddler_auditor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-25 01:14:17.000000 fiddler-auditor-0.0.1rc3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 01:17:47.778644 fiddler-auditor-0.0.1rc3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 01:17:47.774644 fiddler-auditor-0.0.1rc3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-05-25 01:14:17.000000 fiddler-auditor-0.0.1rc3/tests/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-05-25 01:14:17.000000 fiddler-auditor-0.0.1rc3/tests/test_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4694 2023-05-25 01:14:17.000000 fiddler-auditor-0.0.1rc3/tests/test_llm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-25 01:14:17.000000 fiddler-auditor-0.0.1rc3/tests/test_perturbations.py
```

### Comparing `fiddler-auditor-0.0.1rc2/LICENSE` & `fiddler-auditor-0.0.1rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `fiddler-auditor-0.0.1rc2/PKG-INFO` & `fiddler-auditor-0.0.1rc3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: fiddler-auditor
-Version: 0.0.1rc2
+Version: 0.0.1rc3
 Summary: Auditing large language models made easy.
 Author-email: Fiddler Labs <support@fiddler.ai>
 License: Elastic License 2.0 (ELv2)
 Project-URL: repository, https://github.com/fiddler-labs/fiddler-auditor
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
-Requires-Python: <4.0,>=3.10.1
+Requires-Python: <4.0,>=3.8.1
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 # <img src="https://github.com/fiddler-labs/fiddler-auditor/blob/main/docs/source/images/fiddler-auditor-logo.png" width="60%" alt="Fiddler Auditor">
 
 Auditing Large Language Models made easy!
```

### Comparing `fiddler-auditor-0.0.1rc2/README.md` & `fiddler-auditor-0.0.1rc3/README.md`

 * *Files identical despite different names*

### Comparing `fiddler-auditor-0.0.1rc2/auditor/assets/data/snips_dataset_dev.csv` & `fiddler-auditor-0.0.1rc3/auditor/assets/data/snips_dataset_dev.csv`

 * *Files identical despite different names*

### Comparing `fiddler-auditor-0.0.1rc2/auditor/assets/data/snips_dataset_test.csv` & `fiddler-auditor-0.0.1rc3/auditor/assets/data/snips_dataset_test.csv`

 * *Files identical despite different names*

### Comparing `fiddler-auditor-0.0.1rc2/auditor/assets/data/snips_dataset_train.csv` & `fiddler-auditor-0.0.1rc3/auditor/assets/data/snips_dataset_train.csv`

 * *Files identical despite different names*

### Comparing `fiddler-auditor-0.0.1rc2/auditor/evaluation/discriminative.py` & `fiddler-auditor-0.0.1rc3/auditor/evaluation/discriminative.py`

 * *Files identical despite different names*

### Comparing `fiddler-auditor-0.0.1rc2/auditor/evaluation/expected_behavior.py` & `fiddler-auditor-0.0.1rc3/auditor/evaluation/expected_behavior.py`

 * *Files identical despite different names*

### Comparing `fiddler-auditor-0.0.1rc2/auditor/evaluation/generative.py` & `fiddler-auditor-0.0.1rc3/auditor/evaluation/generative.py`

 * *Files identical despite different names*

### Comparing `fiddler-auditor-0.0.1rc2/auditor/generations/paraphrase.py` & `fiddler-auditor-0.0.1rc3/auditor/generations/paraphrase.py`

 * *Files identical despite different names*

### Comparing `fiddler-auditor-0.0.1rc2/auditor/perturbations/text.py` & `fiddler-auditor-0.0.1rc3/auditor/perturbations/text.py`

 * *Files identical despite different names*

### Comparing `fiddler-auditor-0.0.1rc2/auditor/reporting/generate.py` & `fiddler-auditor-0.0.1rc3/auditor/reporting/generate.py`

 * *Files identical despite different names*

### Comparing `fiddler-auditor-0.0.1rc2/auditor/reporting/templates/report_template.html` & `fiddler-auditor-0.0.1rc3/auditor/reporting/templates/report_template.html`

 * *Files identical despite different names*

### Comparing `fiddler-auditor-0.0.1rc2/auditor/utils/data.py` & `fiddler-auditor-0.0.1rc3/auditor/utils/data.py`

 * *Files identical despite different names*

### Comparing `fiddler-auditor-0.0.1rc2/auditor/utils/dataset.py` & `fiddler-auditor-0.0.1rc3/auditor/utils/dataset.py`

 * *Files identical despite different names*

### Comparing `fiddler-auditor-0.0.1rc2/auditor/utils/logging.py` & `fiddler-auditor-0.0.1rc3/auditor/utils/logging.py`

 * *Files identical despite different names*

### Comparing `fiddler-auditor-0.0.1rc2/auditor/utils/similarity.py` & `fiddler-auditor-0.0.1rc3/auditor/utils/similarity.py`

 * *Files identical despite different names*

### Comparing `fiddler-auditor-0.0.1rc2/fiddler_auditor.egg-info/PKG-INFO` & `fiddler-auditor-0.0.1rc3/fiddler_auditor.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: fiddler-auditor
-Version: 0.0.1rc2
+Version: 0.0.1rc3
 Summary: Auditing large language models made easy.
 Author-email: Fiddler Labs <support@fiddler.ai>
 License: Elastic License 2.0 (ELv2)
 Project-URL: repository, https://github.com/fiddler-labs/fiddler-auditor
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
-Requires-Python: <4.0,>=3.10.1
+Requires-Python: <4.0,>=3.8.1
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 # <img src="https://github.com/fiddler-labs/fiddler-auditor/blob/main/docs/source/images/fiddler-auditor-logo.png" width="60%" alt="Fiddler Auditor">
 
 Auditing Large Language Models made easy!
```

### Comparing `fiddler-auditor-0.0.1rc2/fiddler_auditor.egg-info/SOURCES.txt` & `fiddler-auditor-0.0.1rc3/fiddler_auditor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fiddler-auditor-0.0.1rc2/pyproject.toml` & `fiddler-auditor-0.0.1rc3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fiddler-auditor"
-version = "0.0.1.rc2"
+version = "0.0.1.rc3"
 authors = [
   { name="Fiddler Labs", email="support@fiddler.ai" },
 ]
 description = "Auditing large language models made easy."
 readme = "README.md"
-requires-python = ">=3.10.1,<4.0"
+requires-python = ">=3.8.1,<4.0"
 
 
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
 ]
 dependencies = [
```

### Comparing `fiddler-auditor-0.0.1rc2/tests/test_dataset.py` & `fiddler-auditor-0.0.1rc3/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `fiddler-auditor-0.0.1rc2/tests/test_evaluation.py` & `fiddler-auditor-0.0.1rc3/tests/test_evaluation.py`

 * *Files identical despite different names*

### Comparing `fiddler-auditor-0.0.1rc2/tests/test_llm.py` & `fiddler-auditor-0.0.1rc3/tests/test_llm.py`

 * *Files identical despite different names*

### Comparing `fiddler-auditor-0.0.1rc2/tests/test_perturbations.py` & `fiddler-auditor-0.0.1rc3/tests/test_perturbations.py`

 * *Files identical despite different names*

