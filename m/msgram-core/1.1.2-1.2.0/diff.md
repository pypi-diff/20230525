# Comparing `tmp/msgram_core-1.1.2.tar.gz` & `tmp/msgram_core-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msgram_core-1.1.2.tar", last modified: Mon Feb 13 03:32:19 2023, max compression
+gzip compressed data, was "msgram_core-1.2.0.tar", last modified: Thu May 25 21:51:15 2023, max compression
```

## Comparing `msgram_core-1.1.2.tar` & `msgram_core-1.2.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 03:32:19.984989 msgram_core-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)    34464 2023-02-13 03:32:05.000000 msgram_core-1.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    44641 2023-02-13 03:32:19.984989 msgram_core-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-02-13 03:32:05.000000 msgram_core-1.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-02-13 03:32:05.000000 msgram_core-1.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-13 03:32:19.984989 msgram_core-1.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 03:32:19.980989 msgram_core-1.1.2/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-13 03:32:05.000000 msgram_core-1.1.2/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 03:32:19.984989 msgram_core-1.1.2/src/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-13 03:32:05.000000 msgram_core-1.1.2/src/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-02-13 03:32:05.000000 msgram_core-1.1.2/src/core/agregation.py
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-02-13 03:32:05.000000 msgram_core-1.1.2/src/core/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-02-13 03:32:05.000000 msgram_core-1.1.2/src/core/interpretation_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8839 2023-02-13 03:32:05.000000 msgram_core-1.1.2/src/core/measures_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-02-13 03:32:05.000000 msgram_core-1.1.2/src/core/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-02-13 03:32:05.000000 msgram_core-1.1.2/src/core/weighting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 03:32:19.984989 msgram_core-1.1.2/src/msgram_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    44641 2023-02-13 03:32:19.000000 msgram_core-1.1.2/src/msgram_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-02-13 03:32:19.000000 msgram_core-1.1.2/src/msgram_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-13 03:32:19.000000 msgram_core-1.1.2/src/msgram_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-02-13 03:32:19.000000 msgram_core-1.1.2/src/msgram_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-02-13 03:32:19.000000 msgram_core-1.1.2/src/msgram_core.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 03:32:19.984989 msgram_core-1.1.2/src/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-02-13 03:32:05.000000 msgram_core-1.1.2/src/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-02-13 03:32:05.000000 msgram_core-1.1.2/src/parsers/sonarqube.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 03:32:19.984989 msgram_core-1.1.2/src/resources/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-02-13 03:32:05.000000 msgram_core-1.1.2/src/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-02-13 03:32:05.000000 msgram_core-1.1.2/src/resources/analysis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 03:32:19.984989 msgram_core-1.1.2/src/staticfiles/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-02-13 03:32:05.000000 msgram_core-1.1.2/src/staticfiles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-02-13 03:32:05.000000 msgram_core-1.1.2/src/staticfiles/default_pre_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    34875 2023-02-13 03:32:05.000000 msgram_core-1.1.2/src/staticfiles/sonarqube_available_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-02-13 03:32:05.000000 msgram_core-1.1.2/src/staticfiles/sonarqube_supported_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 03:32:19.984989 msgram_core-1.1.2/src/util/
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-02-13 03:32:05.000000 msgram_core-1.1.2/src/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-02-13 03:32:05.000000 msgram_core-1.1.2/src/util/check_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-02-13 03:32:05.000000 msgram_core-1.1.2/src/util/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-02-13 03:32:05.000000 msgram_core-1.1.2/src/util/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-02-13 03:32:05.000000 msgram_core-1.1.2/src/util/get_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 03:32:19.984989 msgram_core-1.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-02-13 03:32:05.000000 msgram_core-1.1.2/tests/test_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:51:15.771896 msgram_core-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    34464 2023-05-25 21:50:59.000000 msgram_core-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    44641 2023-05-25 21:51:15.771896 msgram_core-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-05-25 21:50:59.000000 msgram_core-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-05-25 21:50:59.000000 msgram_core-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 21:51:15.771896 msgram_core-1.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:51:15.767895 msgram_core-1.2.0/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 21:50:59.000000 msgram_core-1.2.0/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:51:15.767895 msgram_core-1.2.0/src/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 21:50:59.000000 msgram_core-1.2.0/src/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-25 21:50:59.000000 msgram_core-1.2.0/src/core/agregation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-25 21:50:59.000000 msgram_core-1.2.0/src/core/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4447 2023-05-25 21:50:59.000000 msgram_core-1.2.0/src/core/interpretation_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11714 2023-05-25 21:50:59.000000 msgram_core-1.2.0/src/core/measures_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4796 2023-05-25 21:50:59.000000 msgram_core-1.2.0/src/core/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-25 21:50:59.000000 msgram_core-1.2.0/src/core/weighting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:51:15.767895 msgram_core-1.2.0/src/msgram_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    44641 2023-05-25 21:51:15.000000 msgram_core-1.2.0/src/msgram_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-25 21:51:15.000000 msgram_core-1.2.0/src/msgram_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 21:51:15.000000 msgram_core-1.2.0/src/msgram_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-25 21:51:15.000000 msgram_core-1.2.0/src/msgram_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-25 21:51:15.000000 msgram_core-1.2.0/src/msgram_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:51:15.771896 msgram_core-1.2.0/src/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-25 21:50:59.000000 msgram_core-1.2.0/src/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-05-25 21:50:59.000000 msgram_core-1.2.0/src/parsers/sonarqube.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:51:15.771896 msgram_core-1.2.0/src/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-25 21:50:59.000000 msgram_core-1.2.0/src/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-05-25 21:50:59.000000 msgram_core-1.2.0/src/resources/analysis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:51:15.771896 msgram_core-1.2.0/src/staticfiles/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-25 21:50:59.000000 msgram_core-1.2.0/src/staticfiles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-05-25 21:50:59.000000 msgram_core-1.2.0/src/staticfiles/default_pre_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34977 2023-05-25 21:50:59.000000 msgram_core-1.2.0/src/staticfiles/sonarqube_available_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-05-25 21:50:59.000000 msgram_core-1.2.0/src/staticfiles/sonarqube_supported_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:51:15.771896 msgram_core-1.2.0/src/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-25 21:50:59.000000 msgram_core-1.2.0/src/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-05-25 21:50:59.000000 msgram_core-1.2.0/src/util/check_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-05-25 21:50:59.000000 msgram_core-1.2.0/src/util/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-25 21:50:59.000000 msgram_core-1.2.0/src/util/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-25 21:50:59.000000 msgram_core-1.2.0/src/util/get_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:51:15.771896 msgram_core-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-05-25 21:50:59.000000 msgram_core-1.2.0/tests/test_helpers.py
```

### Comparing `msgram_core-1.1.2/LICENSE` & `msgram_core-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `msgram_core-1.1.2/PKG-INFO` & `msgram_core-1.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msgram_core
-Version: 1.1.2
+Version: 1.2.0
 Summary: The MeasureSoftGram-Core is a Software system for continuous quality of product observation and multidimensional use in continuous design engineering software and is where you have the innovative mathematical models for software analysis.
 Author-email: MeasureSoftGram <measuresoftgram@gmail.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -672,29 +672,29 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# 2022-2-MeasureSoftGram-Core
+# 2023-1-MeasureSoftGram-Core
 
 ## Badges
 
-[![Code Smells](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2022-2-MeasureSoftGram-Core&metric=code_smells)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2022-2-MeasureSoftGram-Core)
-[![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2022-2-MeasureSoftGram-Core&metric=sqale_rating)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2022-2-MeasureSoftGram-Core)
-[![Security Rating](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2022-2-MeasureSoftGram-Core&metric=security_rating)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2022-2-MeasureSoftGram-Core)
-[![Bugs](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2022-2-MeasureSoftGram-Core&metric=bugs)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2022-2-MeasureSoftGram-Core)
-[![Vulnerabilities](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2022-2-MeasureSoftGram-Core&metric=vulnerabilities)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2022-2-MeasureSoftGram-Core)
-[![Duplicated Lines (%)](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2022-2-MeasureSoftGram-Core&metric=duplicated_lines_density)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2022-2-MeasureSoftGram-Core)
-[![Reliability Rating](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2022-2-MeasureSoftGram-Core&metric=reliability_rating)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2022-2-MeasureSoftGram-Core)
-[![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2022-2-MeasureSoftGram-Core&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2022-2-MeasureSoftGram-Core)
-[![Technical Debt](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2022-2-MeasureSoftGram-Core&metric=sqale_index)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2022-2-MeasureSoftGram-Core)
-[![Coverage](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2022-2-MeasureSoftGram-Core&metric=coverage)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2022-2-MeasureSoftGram-Core)
-[![Lines of Code](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2022-2-MeasureSoftGram-Core&metric=ncloc)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2022-2-MeasureSoftGram-Core)
+[![Code Smells](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2023-1-MeasureSoftGram-Core&metric=code_smells)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2023-1-MeasureSoftGram-Core)
+[![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2023-1-MeasureSoftGram-Core&metric=sqale_rating)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2023-1-MeasureSoftGram-Core)
+[![Security Rating](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2023-1-MeasureSoftGram-Core&metric=security_rating)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2023-1-MeasureSoftGram-Core)
+[![Bugs](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2023-1-MeasureSoftGram-Core&metric=bugs)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2023-1-MeasureSoftGram-Core)
+[![Vulnerabilities](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2023-1-MeasureSoftGram-Core&metric=vulnerabilities)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2023-1-MeasureSoftGram-Core)
+[![Duplicated Lines (%)](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2023-1-MeasureSoftGram-Core&metric=duplicated_lines_density)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2023-1-MeasureSoftGram-Core)
+[![Reliability Rating](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2023-1-MeasureSoftGram-Core&metric=reliability_rating)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2023-1-MeasureSoftGram-Core)
+[![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2023-1-MeasureSoftGram-Core&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2023-1-MeasureSoftGram-Core)
+[![Technical Debt](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2023-1-MeasureSoftGram-Core&metric=sqale_index)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2023-1-MeasureSoftGram-Core)
+[![Coverage](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2023-1-MeasureSoftGram-Core&metric=coverage)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2023-1-MeasureSoftGram-Core)
+[![Lines of Code](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2023-1-MeasureSoftGram-Core&metric=ncloc)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2023-1-MeasureSoftGram-Core)
 
 ## What is it?
 
 The MeasureSoftGram-Core is a Software system for continuous quality of product observation and multidimensional use in continuous design engineering software and is where you have the innovative mathematical models for software analysis.
 
 ## How to use MeasureSoftGram Core
 -[How to use](https://fga-eps-mds.github.io/2021-2-MeasureSoftGram-Doc/docs/artifact/how_to_use)
@@ -754,9 +754,9 @@
 Our services are available on [Docker Hub](https://hub.docker.com/):
 - [Core](https://hub.docker.com/r/measuresoftgram/core)
 - [Service](https://hub.docker.com/r/measuresoftgram/service)
 
 ### Wiki
 
 For more informations, you can see our wiki:
-- [Wiki](https://fga-eps-mds.github.io/2022-2-MeasureSoftGram-Doc/)
+- [Wiki](https://fga-eps-mds.github.io/2023-1-MeasureSoftGram-Doc/)
```

### Comparing `msgram_core-1.1.2/README.md` & `msgram_core-1.2.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-# 2022-2-MeasureSoftGram-Core
+# 2023-1-MeasureSoftGram-Core
 
 ## Badges
 
-[![Code Smells](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2022-2-MeasureSoftGram-Core&metric=code_smells)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2022-2-MeasureSoftGram-Core)
-[![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2022-2-MeasureSoftGram-Core&metric=sqale_rating)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2022-2-MeasureSoftGram-Core)
-[![Security Rating](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2022-2-MeasureSoftGram-Core&metric=security_rating)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2022-2-MeasureSoftGram-Core)
-[![Bugs](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2022-2-MeasureSoftGram-Core&metric=bugs)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2022-2-MeasureSoftGram-Core)
-[![Vulnerabilities](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2022-2-MeasureSoftGram-Core&metric=vulnerabilities)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2022-2-MeasureSoftGram-Core)
-[![Duplicated Lines (%)](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2022-2-MeasureSoftGram-Core&metric=duplicated_lines_density)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2022-2-MeasureSoftGram-Core)
-[![Reliability Rating](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2022-2-MeasureSoftGram-Core&metric=reliability_rating)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2022-2-MeasureSoftGram-Core)
-[![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2022-2-MeasureSoftGram-Core&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2022-2-MeasureSoftGram-Core)
-[![Technical Debt](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2022-2-MeasureSoftGram-Core&metric=sqale_index)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2022-2-MeasureSoftGram-Core)
-[![Coverage](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2022-2-MeasureSoftGram-Core&metric=coverage)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2022-2-MeasureSoftGram-Core)
-[![Lines of Code](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2022-2-MeasureSoftGram-Core&metric=ncloc)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2022-2-MeasureSoftGram-Core)
+[![Code Smells](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2023-1-MeasureSoftGram-Core&metric=code_smells)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2023-1-MeasureSoftGram-Core)
+[![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2023-1-MeasureSoftGram-Core&metric=sqale_rating)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2023-1-MeasureSoftGram-Core)
+[![Security Rating](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2023-1-MeasureSoftGram-Core&metric=security_rating)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2023-1-MeasureSoftGram-Core)
+[![Bugs](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2023-1-MeasureSoftGram-Core&metric=bugs)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2023-1-MeasureSoftGram-Core)
+[![Vulnerabilities](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2023-1-MeasureSoftGram-Core&metric=vulnerabilities)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2023-1-MeasureSoftGram-Core)
+[![Duplicated Lines (%)](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2023-1-MeasureSoftGram-Core&metric=duplicated_lines_density)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2023-1-MeasureSoftGram-Core)
+[![Reliability Rating](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2023-1-MeasureSoftGram-Core&metric=reliability_rating)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2023-1-MeasureSoftGram-Core)
+[![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2023-1-MeasureSoftGram-Core&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2023-1-MeasureSoftGram-Core)
+[![Technical Debt](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2023-1-MeasureSoftGram-Core&metric=sqale_index)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2023-1-MeasureSoftGram-Core)
+[![Coverage](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2023-1-MeasureSoftGram-Core&metric=coverage)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2023-1-MeasureSoftGram-Core)
+[![Lines of Code](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2023-1-MeasureSoftGram-Core&metric=ncloc)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2023-1-MeasureSoftGram-Core)
 
 ## What is it?
 
 The MeasureSoftGram-Core is a Software system for continuous quality of product observation and multidimensional use in continuous design engineering software and is where you have the innovative mathematical models for software analysis.
 
 ## How to use MeasureSoftGram Core
 -[How to use](https://fga-eps-mds.github.io/2021-2-MeasureSoftGram-Doc/docs/artifact/how_to_use)
@@ -76,9 +76,9 @@
 Our services are available on [Docker Hub](https://hub.docker.com/):
 - [Core](https://hub.docker.com/r/measuresoftgram/core)
 - [Service](https://hub.docker.com/r/measuresoftgram/service)
 
 ### Wiki
 
 For more informations, you can see our wiki:
-- [Wiki](https://fga-eps-mds.github.io/2022-2-MeasureSoftGram-Doc/)
+- [Wiki](https://fga-eps-mds.github.io/2023-1-MeasureSoftGram-Doc/)
```

### Comparing `msgram_core-1.1.2/pyproject.toml` & `msgram_core-1.2.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "msgram_core"
-version = "1.1.2"
+version = "1.2.0"
 description = "The MeasureSoftGram-Core is a Software system for continuous quality of product observation and multidimensional use in continuous design engineering software and is where you have the innovative mathematical models for software analysis."
 readme = "README.md"
 authors = [
     { name = "MeasureSoftGram", email = "measuresoftgram@gmail.com" }
 ]
 license = { file = "LICENSE" }
 classifiers = [
@@ -17,11 +17,11 @@
     "Natural Language :: Portuguese (Brazilian)",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3.8",
     "Topic :: Utilities",
 ]
 keywords = ["core", "measures", "quality", "algebraic model"]
 requires-python = ">=3.8"
-dependencies = ["Flask==2.1.*", "Flask-RESTful==0.3.*", "pandas==1.4.*", "tensorly==0.7.*", "requests==2.28.*" ,"gunicorn==20.1.*", "flask-marshmallow==0.14.*"]
+dependencies = ["pandas==1.4.*", "tensorly==0.7.*", "requests==2.28.*", "flask-marshmallow==0.14.*"]
 
 [tool.mypy]
 strict = true
```

### Comparing `msgram_core-1.1.2/src/core/dataframe.py` & `msgram_core-1.2.0/src/core/dataframe.py`

 * *Files identical despite different names*

### Comparing `msgram_core-1.1.2/src/core/measures_functions.py` & `msgram_core-1.2.0/src/core/measures_functions.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 from typing import Dict
 
 import numpy as np
 import pandas as pd
 
-from util.exceptions import ImplicitMetricValueError, InvalidMetricValue
+from util.exceptions import (
+    ImplicitMetricValueError,
+    InvalidMetricValue,
+    InvalidThresholdValue,
+)
 from util.get_functions import create_coordinate_pair
 
 
 def interpolate_series(series, x, y):
     """
     Interpolates a series using the given x and y values.
 
@@ -23,21 +27,39 @@
 
     This functions converts the metric parameter to a pandas Series if it is a list (CalculateMeasures endpoint)
     otherwise it just returns the metric - already a pandas Series (Analysis endpoint).
     """
     return pd.Series(metric, dtype=np.float64) if isinstance(metric, list) else metric
 
 
-def calculate_em1(data: Dict):
+def calculate_em1(
+    data: Dict,
+    min_complex_files_density: float = 0,
+    max_complex_files_density: float = 10,
+):
     """
     Calculates non-complex files density (em1).
 
     This function calculates non-complex files density measure (em1)
     used to assess the changeability quality sub characteristic.
     """
+    if min_complex_files_density != 0:
+        raise InvalidThresholdValue(("min_complex_files_density is not equal to 0"))
+
+    if min_complex_files_density >= max_complex_files_density:
+        raise InvalidThresholdValue(
+            (
+                "min_complex_files_density is greater or equal to"
+                " max_complex_files_density"
+            )
+        )
+
+    # if max_complex_files_density > 100:
+    #     raise InvalidThresholdValue(("max_complex_files_density is greater than 100"))
+
     files_complexity = resolve_metric_list_parameter(data["complexity"])
     files_functions = resolve_metric_list_parameter(data["functions"])
 
     if "number_of_files" in data:
         number_of_files = data["number_of_files"]
 
     elif len(files_complexity) != len(files_functions):
@@ -53,208 +75,296 @@
 
     has_none = files_complexity is None or files_functions is None
     has_zero = len(files_complexity) == 0 or len(files_functions) == 0
 
     if has_none or has_zero:
         return 0
 
-    COMPLEX_FILES_DENSITY_THRESHOLD = 10
-
     if files_complexity.sum() <= 0:
-        raise InvalidMetricValue("The cyclomatic complexity of all files is lesser or equal than 0")
+        raise InvalidMetricValue(
+            "The cyclomatic complexity of all files is lesser or equal than 0"
+        )
 
     if files_functions.sum() <= 0:
-        raise InvalidMetricValue("The number of functions of all files is lesser or equal than 0")
+        raise InvalidMetricValue(
+            "The number of functions of all files is lesser or equal than 0"
+        )
 
-    x, y = create_coordinate_pair(0, COMPLEX_FILES_DENSITY_THRESHOLD)
+    x, y = create_coordinate_pair(
+        min_complex_files_density,
+        max_complex_files_density,
+    )
 
-    files_in_thresholds_df = (files_complexity / files_functions) <= COMPLEX_FILES_DENSITY_THRESHOLD
-    IF1 = np.interp(list(files_in_thresholds_df[(files_functions > 0)]), x, y)
+    files_in_thresholds_df = files_complexity / files_functions
+    files_in_thresholds_bool_index = files_in_thresholds_df <= max_complex_files_density
+    files_functions_gt_zero_bool_index = files_functions > 0
+    IF1 = np.interp(
+        list(
+            files_in_thresholds_df[
+                files_in_thresholds_bool_index * files_functions_gt_zero_bool_index
+            ]
+        ),
+        x,
+        y,
+    )
     em1 = np.divide(sum(IF1), number_of_files)
 
     if np.isnan(em1) or np.isinf(em1):
         return 0
     return em1
 
 
-def calculate_em2(data: Dict):
+def calculate_em2(
+    data: Dict,
+    min_comment_density: float = 10,
+    max_comment_density: float = 30,
+):
     """
     Calculates commented files density (em2).
 
     This function calculates commented files density measure (em2)
     used to assess the changeability quality sub characteristic.
     """
-    files_comment_lines_density = resolve_metric_list_parameter(data["comment_lines_density"])
+    if min_comment_density < 0:
+        raise InvalidThresholdValue(("min_comment_density is lesser than 0"))
+
+    if min_comment_density >= max_comment_density:
+        raise InvalidThresholdValue(
+            ("min_comment_density is greater or equal to" " max_comment_density")
+        )
+    if max_comment_density > 100:
+        raise InvalidThresholdValue(("max_comment_density is greater than 100"))
+
+    files_comment_lines_density = resolve_metric_list_parameter(
+        data["comment_lines_density"]
+    )
 
     if "number_of_files" in data:
         number_of_files = data["number_of_files"]
     else:
         number_of_files = len(files_comment_lines_density)
 
     has_none = files_comment_lines_density is None
     has_zero = len(files_comment_lines_density) == 0
 
     if has_none or has_zero:
         return 0
 
-    MINIMUM_COMMENT_DENSITY_THRESHOLD = 10
-    MAXIMUM_COMMENT_DENSITY_THRESHOLD = 30
-
     if files_comment_lines_density.sum() < 0:
-        raise InvalidMetricValue("The number of files comment lines density is lesser than 0")
+        raise InvalidMetricValue(
+            "The number of files comment lines density is lesser than 0"
+        )
 
     x, y = create_coordinate_pair(
-        MINIMUM_COMMENT_DENSITY_THRESHOLD / 100, MAXIMUM_COMMENT_DENSITY_THRESHOLD / 100
+        min_comment_density / 100,
+        max_comment_density / 100,
     )
 
     files_between_thresholds = files_comment_lines_density[
         files_comment_lines_density.between(
-            MINIMUM_COMMENT_DENSITY_THRESHOLD,
-            MAXIMUM_COMMENT_DENSITY_THRESHOLD,
+            min_comment_density,
+            max_comment_density,
             inclusive="both",
         )
     ]
 
     em2i = interpolate_series(files_between_thresholds, x, y)
     em2 = np.divide(np.sum(em2i), number_of_files)
 
     if np.isnan(em2) or np.isinf(em2):
         return 0
     return em2
 
 
-def calculate_em3(data: Dict):
+def calculate_em3(
+    data: Dict,
+    min_duplicated_lines: float = 0,
+    max_duplicated_lines: float = 5.0,
+):
     """
     Calculates duplicated files absence (em3).
 
     This function calculates the duplicated files absence measure (em3)
     used to assess the changeability quality sub characteristic.
     """
-    files_duplicated_lines_density = resolve_metric_list_parameter(data["duplicated_lines_density"])
+    if min_duplicated_lines != 0:
+        raise InvalidThresholdValue(("min_duplicated_lines is not equal to 0"))
+
+    if min_duplicated_lines >= max_duplicated_lines:
+        raise InvalidThresholdValue(
+            ("min_duplicated_lines is greater or equal to" " max_duplicated_lines")
+        )
+
+    if max_duplicated_lines > 100:
+        raise InvalidThresholdValue(("max_duplicated_lines is greater than 100"))
+
+    files_duplicated_lines_density = resolve_metric_list_parameter(
+        data["duplicated_lines_density"]
+    )
 
     if "number_of_files" in data:
         number_of_files = data["number_of_files"]
     else:
         number_of_files = len(files_duplicated_lines_density)
 
     has_none = files_duplicated_lines_density is None
     has_zero = len(files_duplicated_lines_density) == 0
 
     if has_none or has_zero:
         return 0
 
-    DUPLICATED_LINES_THRESHOLD = 5.0
-
     if files_duplicated_lines_density.sum() < 0:
-        raise InvalidMetricValue("The number of files duplicated lines density is lesser than 0")
+        raise InvalidMetricValue(
+            "The number of files duplicated lines density is lesser than 0"
+        )
 
-    x, y = create_coordinate_pair(0, DUPLICATED_LINES_THRESHOLD / 100)
+    x, y = create_coordinate_pair(
+        min_duplicated_lines / 100,
+        max_duplicated_lines / 100,
+    )
 
     files_below_threshold = files_duplicated_lines_density[
-        files_duplicated_lines_density <= DUPLICATED_LINES_THRESHOLD
+        files_duplicated_lines_density <= max_duplicated_lines
     ]
 
     em3i = interpolate_series(files_below_threshold, x, y)
     em3 = np.divide(np.sum(em3i), number_of_files)
 
     if np.isnan(em3) or np.isinf(em3):
         return 0
     return em3
 
 
-def calculate_em4(data: Dict[str, float]):
+def calculate_em4(
+    data: Dict[str, float],
+    min_passed_tests: float = 0,
+    max_passed_tests: float = 1,
+):
     """
     Calculates passed tests (em4)
 
     This function calculates the passed tests measure (em4)
     used to assess the testing status sub characteristic.
     """
+    if min_passed_tests != 0:
+        raise InvalidThresholdValue(("min_passed_tests is not equal to 0"))
+
+    if max_passed_tests != 1:
+        raise InvalidThresholdValue(("max_passed_tests is not equal to 1"))
     try:
         # number_of_tests está retornando valores incorretos
         number_of_tests = resolve_metric_list_parameter(data["tests"]).sum()
         number_of_test_errors = data["test_errors"]
         number_of_test_failures = data["test_failures"]
 
-        x, y = create_coordinate_pair(0, 1, reverse_y=True)
+        x, y = create_coordinate_pair(
+            min_passed_tests,
+            max_passed_tests,
+            reverse_y=True,
+        )
 
         number_of_fail_tests = number_of_test_errors + number_of_test_failures
         if4i = np.divide((number_of_tests - number_of_fail_tests), number_of_tests)
 
     except ZeroDivisionError:
         return 0
 
     else:
         if np.isnan(if4i) or np.isinf(if4i):
             return 0
         return np.interp(if4i, x, y)
 
 
-def calculate_em5(data: Dict[str, list]):
+def calculate_em5(
+    data: Dict[str, list],
+    min_fast_test_time: float = 0,
+    max_fast_test_time: float = 300000,
+):
     """
     Calculates fast test builds (em5)
 
     This function calculates the fast test builds measure (em5)
     used to assess the testing status sub characteristic.
     """
+    if min_fast_test_time != 0:
+        raise InvalidThresholdValue(("min_fast_test_time is not equal to 0"))
+
+    if min_fast_test_time >= max_fast_test_time:
+        raise InvalidThresholdValue(
+            ("min_fast_test_time is greater or equal to" " max_fast_test_time")
+        )
+
     execution_time = resolve_metric_list_parameter(data["test_execution_time"])
     number_of_tests = resolve_metric_list_parameter(data["tests"])
     number_of_files = len(execution_time)
 
     has_none = execution_time is None or number_of_tests is None
     has_zero = len(execution_time) == 0 or len(number_of_tests) == 0
 
     if has_none or has_zero:
         return 0
 
-    MAXIMUM_COVERAGE_THRESHOLD = 300000
-
-    x, y = create_coordinate_pair(0, MAXIMUM_COVERAGE_THRESHOLD)
+    x, y = create_coordinate_pair(min_fast_test_time, max_fast_test_time)
 
-    execution_between_thresholds = execution_time[execution_time <= MAXIMUM_COVERAGE_THRESHOLD]
-    fast_tests_between_thresholds = np.divide(execution_between_thresholds, number_of_tests)
+    execution_between_thresholds = execution_time[execution_time <= max_fast_test_time]
+    fast_tests_between_thresholds = np.divide(
+        execution_between_thresholds, number_of_tests
+    )
 
     em5i = interpolate_series(fast_tests_between_thresholds, x, y)
     em5 = np.divide(np.sum(em5i), number_of_files)
 
     if np.isnan(em5) or np.isinf(em5):
         return 0
 
     return em5
 
 
-def calculate_em6(data: Dict):
+def calculate_em6(
+    data: Dict,
+    min_coverage: float = 60,
+    max_coverage: float = 90,
+):
     """
     Calculates test coverage (em6).
 
     This function calculates the test coverage measure (em6)
     used to assess the testing status sub characteristic.
     """
+    if min_coverage < 0:
+        raise InvalidThresholdValue(("min_coverage is lesser than 0"))
+
+    if min_coverage >= max_coverage:
+        raise InvalidThresholdValue(
+            ("min_coverage is greater or equal to" " max_coverage")
+        )
+
+    if max_coverage > 100:
+        raise InvalidThresholdValue(("max_coverage is greater than 100"))
+
     coverage = resolve_metric_list_parameter(data["coverage"])
 
     if "number_of_files" in data:
         number_of_files = data["number_of_files"]
     else:
         number_of_files = len(coverage)
 
     has_none = coverage is None
     has_zero = len(coverage) == 0
 
     if has_none or has_zero:
         return 0
 
-    MINIMUM_COVERAGE_THRESHOLD = 60
-    MAXIMUM_COVERAGE_THRESHOLD = 90
-
     x, y = create_coordinate_pair(
-        MINIMUM_COVERAGE_THRESHOLD / 100,
-        MAXIMUM_COVERAGE_THRESHOLD / 100,
+        min_coverage / 100,
+        max_coverage / 100,
         reverse_y=True,
     )
 
-    files_between_thresholds = coverage[coverage >= MINIMUM_COVERAGE_THRESHOLD]
+    files_between_thresholds = coverage[coverage >= min_coverage]
     em6i = interpolate_series(files_between_thresholds, x, y)
     em6 = np.divide(np.sum(em6i), number_of_files)
 
     if np.isnan(em6) or np.isinf(em6):
         return 0
     return em6
 
@@ -266,15 +376,17 @@
     This function calculates the team throughput measure (em7)
     used to assess the functional completeness subcharacteristic.
     """
     resolved_issues_with_us_label = data[
         "number_of_resolved_issues_with_US_label_in_the_last_x_days"
     ]
 
-    total_issues_with_us_label = data["total_number_of_issues_with_US_label_in_the_last_x_days"]
+    total_issues_with_us_label = data[
+        "total_number_of_issues_with_US_label_in_the_last_x_days"
+    ]
 
     x, y = create_coordinate_pair(0, 1, reverse_y=True)
 
     if7 = np.divide(resolved_issues_with_us_label, total_issues_with_us_label)
 
     if np.isnan(if7) or np.isinf(if7):
         return 0
```

### Comparing `msgram_core-1.1.2/src/core/schemas.py` & `msgram_core-1.2.0/src/core/schemas.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
         "parameters": {
             "tests": 10,
             "test_errors": 3,
             "test_failures": 1
         }
     }
     """
+
     key = fields.Str(required=True)
     parameters = fields.Dict(required=True)
 
 
 class CalculateMeasureSchema(Schema):
     """
     {
@@ -35,14 +36,15 @@
                     "param2": 19,
                     "parma3": 4
                 }
             }
         ]
     }
     """
+
     measures = fields.List(fields.Nested(MeasureSchema), required=True)
 
 
 class CalculatedSubEntitySchema(Schema):
     key = fields.Str(required=True)
     value = fields.Float(validate=validate.Range(min=0, max=1), required=True)
     weight = fields.Float(validate=validate.Range(min=0, max=100), required=True)
@@ -68,20 +70,25 @@
                     ...
                 ]
             },
             ...
         ]
     }
     """
-    subcharacteristics = fields.List(fields.Nested(SubCharacteristicSchema), required=True)
+
+    subcharacteristics = fields.List(
+        fields.Nested(SubCharacteristicSchema), required=True
+    )
 
 
 class CharacteristicSchema(Schema):
     key = fields.Str(required=True)
-    subcharacteristics = fields.List(fields.Nested(CalculatedSubEntitySchema), required=True)
+    subcharacteristics = fields.List(
+        fields.Nested(CalculatedSubEntitySchema), required=True
+    )
 
 
 class CalculateCharacteristicSchema(Schema):
     """
     {
         "characteristics": [
             {
@@ -95,20 +102,23 @@
                     ...
                 ]
             },
             ...
         ]
     }
     """
+
     characteristics = fields.List(fields.Nested(CharacteristicSchema), required=True)
 
 
 class SQCSchema(Schema):
     key = fields.Str(required=True)
-    characteristics = fields.List(fields.Nested(CalculatedSubEntitySchema), required=True)
+    characteristics = fields.List(
+        fields.Nested(CalculatedSubEntitySchema), required=True
+    )
 
 
 class CalculateSQCSchema(Schema):
     """
     {
         "sqc": {
             "key": "sqc",
@@ -119,69 +129,81 @@
                     "weight": 50,
                 },
                 ...
             ]
         }
     }
     """
+
     sqc = fields.Nested(SQCSchema, required=True)
 
 
 class NonComplexFileDensitySchema(Schema):
     """
     "key": "non_complex_file_density",
     "function": calculate_em1
     """
+
     complexity = fields.List(fields.Float(required=True))
     functions = fields.List(fields.Float(required=True))
 
 
 class CommentedFileDensitySchema(Schema):
     """
     "key": "commented_file_density",
     "function": calculate_em2
     """
+
     comment_lines_density = fields.List(fields.Float(required=True))
 
 
 class DuplicationAbsenceSchema(Schema):
     """
     "key": "duplication_absense",
     "function": calculate_em3
     """
+
     duplicated_lines_density = fields.List(fields.Float(required=True))
 
 
 class PassedTestsSchema(Schema):
     """
     "key": "passed_tests",
     "function": calculate_em4
     """
+
     tests = fields.List(fields.Float(required=True))
     test_errors = fields.Float(required=True)
     test_failures = fields.Float(required=True)
 
 
 class TestBuildsSchema(Schema):
     """
     "key": "test_builds",
     "function": calculate_em5
     """
+
     test_execution_time = fields.List(fields.Float(required=True))
     tests = fields.List(fields.Float(required=True))
 
 
 class TestCoverageSchema(Schema):
     """
     "key": "test_coverage",
     "function": calculate_em6
     """
+
     coverage = fields.List(fields.Float(required=True))
 
 
 class TeamThroughputSchema(Schema):
     """
     "key": "team_throughput",
     "function": calculate_em7
     """
-    number_of_resolved_issues_with_US_label_in_the_last_x_days = fields.Integer(required=True)
-    total_number_of_issues_with_US_label_in_the_last_x_days = fields.Integer(required=True)
+
+    number_of_resolved_issues_with_US_label_in_the_last_x_days = fields.Integer(
+        required=True
+    )
+    total_number_of_issues_with_US_label_in_the_last_x_days = fields.Integer(
+        required=True
+    )
```

### Comparing `msgram_core-1.1.2/src/msgram_core.egg-info/PKG-INFO` & `msgram_core-1.2.0/src/msgram_core.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msgram-core
-Version: 1.1.2
+Version: 1.2.0
 Summary: The MeasureSoftGram-Core is a Software system for continuous quality of product observation and multidimensional use in continuous design engineering software and is where you have the innovative mathematical models for software analysis.
 Author-email: MeasureSoftGram <measuresoftgram@gmail.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -672,29 +672,29 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# 2022-2-MeasureSoftGram-Core
+# 2023-1-MeasureSoftGram-Core
 
 ## Badges
 
-[![Code Smells](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2022-2-MeasureSoftGram-Core&metric=code_smells)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2022-2-MeasureSoftGram-Core)
-[![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2022-2-MeasureSoftGram-Core&metric=sqale_rating)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2022-2-MeasureSoftGram-Core)
-[![Security Rating](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2022-2-MeasureSoftGram-Core&metric=security_rating)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2022-2-MeasureSoftGram-Core)
-[![Bugs](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2022-2-MeasureSoftGram-Core&metric=bugs)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2022-2-MeasureSoftGram-Core)
-[![Vulnerabilities](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2022-2-MeasureSoftGram-Core&metric=vulnerabilities)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2022-2-MeasureSoftGram-Core)
-[![Duplicated Lines (%)](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2022-2-MeasureSoftGram-Core&metric=duplicated_lines_density)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2022-2-MeasureSoftGram-Core)
-[![Reliability Rating](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2022-2-MeasureSoftGram-Core&metric=reliability_rating)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2022-2-MeasureSoftGram-Core)
-[![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2022-2-MeasureSoftGram-Core&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2022-2-MeasureSoftGram-Core)
-[![Technical Debt](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2022-2-MeasureSoftGram-Core&metric=sqale_index)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2022-2-MeasureSoftGram-Core)
-[![Coverage](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2022-2-MeasureSoftGram-Core&metric=coverage)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2022-2-MeasureSoftGram-Core)
-[![Lines of Code](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2022-2-MeasureSoftGram-Core&metric=ncloc)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2022-2-MeasureSoftGram-Core)
+[![Code Smells](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2023-1-MeasureSoftGram-Core&metric=code_smells)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2023-1-MeasureSoftGram-Core)
+[![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2023-1-MeasureSoftGram-Core&metric=sqale_rating)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2023-1-MeasureSoftGram-Core)
+[![Security Rating](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2023-1-MeasureSoftGram-Core&metric=security_rating)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2023-1-MeasureSoftGram-Core)
+[![Bugs](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2023-1-MeasureSoftGram-Core&metric=bugs)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2023-1-MeasureSoftGram-Core)
+[![Vulnerabilities](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2023-1-MeasureSoftGram-Core&metric=vulnerabilities)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2023-1-MeasureSoftGram-Core)
+[![Duplicated Lines (%)](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2023-1-MeasureSoftGram-Core&metric=duplicated_lines_density)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2023-1-MeasureSoftGram-Core)
+[![Reliability Rating](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2023-1-MeasureSoftGram-Core&metric=reliability_rating)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2023-1-MeasureSoftGram-Core)
+[![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2023-1-MeasureSoftGram-Core&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2023-1-MeasureSoftGram-Core)
+[![Technical Debt](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2023-1-MeasureSoftGram-Core&metric=sqale_index)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2023-1-MeasureSoftGram-Core)
+[![Coverage](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2023-1-MeasureSoftGram-Core&metric=coverage)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2023-1-MeasureSoftGram-Core)
+[![Lines of Code](https://sonarcloud.io/api/project_badges/measure?project=fga-eps-mds_2023-1-MeasureSoftGram-Core&metric=ncloc)](https://sonarcloud.io/summary/new_code?id=fga-eps-mds_2023-1-MeasureSoftGram-Core)
 
 ## What is it?
 
 The MeasureSoftGram-Core is a Software system for continuous quality of product observation and multidimensional use in continuous design engineering software and is where you have the innovative mathematical models for software analysis.
 
 ## How to use MeasureSoftGram Core
 -[How to use](https://fga-eps-mds.github.io/2021-2-MeasureSoftGram-Doc/docs/artifact/how_to_use)
@@ -754,9 +754,9 @@
 Our services are available on [Docker Hub](https://hub.docker.com/):
 - [Core](https://hub.docker.com/r/measuresoftgram/core)
 - [Service](https://hub.docker.com/r/measuresoftgram/service)
 
 ### Wiki
 
 For more informations, you can see our wiki:
-- [Wiki](https://fga-eps-mds.github.io/2022-2-MeasureSoftGram-Doc/)
+- [Wiki](https://fga-eps-mds.github.io/2023-1-MeasureSoftGram-Doc/)
```

### Comparing `msgram_core-1.1.2/src/msgram_core.egg-info/SOURCES.txt` & `msgram_core-1.2.0/src/msgram_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `msgram_core-1.1.2/src/parsers/sonarqube.py` & `msgram_core-1.2.0/src/parsers/sonarqube.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 
 import requests
 
 from staticfiles import SONARQUBE_AVAILABLE_METRICS, SONARQUBE_SUPPORTED_MEASURES
 
 
 class Sonarqube:
-
     def __init__(self):
-        self.endpoint = os.getenv("SONAR_URL", "https://sonarcloud.io/api/metrics/search")
+        self.endpoint = os.getenv(
+            "SONAR_URL", "https://sonarcloud.io/api/metrics/search"
+        )
 
     def extract_supported_metrics(self, metrics, first_request=False):
         data = SONARQUBE_AVAILABLE_METRICS
 
         if not first_request:
             return self.__extract_sonarqube_supported_metrics(metrics, data)
 
@@ -29,30 +30,26 @@
     def __extract_sonarqube_supported_metrics(self, metrics, sonar_metrics):
         collected_metrics = {}
         supported_metrics = []
 
         # NOTE: list comprehension que preenche o supported_metrics apenas
         #       com os valores das "metrics" do dicionário de SUPPORTEDs
         [
-            supported_metrics.extend(list(x.values())[0]['metrics'])
+            supported_metrics.extend(list(x.values())[0]["metrics"])
             for x in SONARQUBE_SUPPORTED_MEASURES
         ]
 
         for component in metrics:
-            qualifier = component['qualifier']
-            path = component['path' if qualifier != 'TRK' else 'name']
-            collected_metrics[path] = {
-                'qualifier': qualifier,
-                'measures': []
-            }
+            qualifier = component["qualifier"]
+            path = component["path" if qualifier != "TRK" else "name"]
+            collected_metrics[path] = {"qualifier": qualifier, "measures": []}
 
-            for obj in component['measures']:
-                metric_key = obj['metric']
+            for obj in component["measures"]:
+                metric_key = obj["metric"]
                 if metric_key not in supported_metrics:
                     continue
 
-                collected_metrics[path]['measures'].append({
-                    'metric': metric_key,
-                    'value': float(obj['value'])
-                })
+                collected_metrics[path]["measures"].append(
+                    {"metric": metric_key, "value": float(obj["value"])}
+                )
 
         return collected_metrics
```

### Comparing `msgram_core-1.1.2/src/resources/analysis.py` & `msgram_core-1.2.0/src/resources/analysis.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,155 +1,170 @@
 import requests
 from marshmallow.exceptions import ValidationError
 
 from core.schemas import (
     CalculateMeasureSchema,
     CalculateSubCharacteristicSchema,
     CalculateCharacteristicSchema,
-    CalculateSQCSchema
+    CalculateSQCSchema,
 )
 from core.agregation import aggregation_operation
 from core.weighting import weighting_operation
 from util.constants import MEASURES_INTERPRETATION_MAPPING
 
 
 def calculate_aggregated_value(values_list, weights_list):
     weighted_items = weighting_operation(values_list, weights_list)
     return aggregation_operation(weighted_items, weights_list)
 
 
-def calculate_measures(extracted_measures):
+def calculate_measures(extracted_measures, config: dict = {"thresholds": {}}):
     # Validate if outter keys is valid
     try:
         data = CalculateMeasureSchema().load(extracted_measures)
     except ValidationError as error:
         return {
             "error": "Failed to validate request",
             "schema_errors": error.messages,
-            "code": requests.codes.unprocessable_entity
+            "code": requests.codes.unprocessable_entity,
         }
 
     # Objeto retornado em caso de sucesso
     response_data = {"measures": []}
 
     valid_measures = MEASURES_INTERPRETATION_MAPPING.keys()
 
     for measure in data["measures"]:
-        measure_key: str = measure['key']
+        measure_key: str = measure["key"]
 
         if measure_key not in valid_measures:
             return {
                 "error": f"Measure {measure_key} is not supported",
-                "code": requests.codes.unprocessable_entity
+                "code": requests.codes.unprocessable_entity,
             }
 
         measure_params = measure["parameters"]
         schema = MEASURES_INTERPRETATION_MAPPING[measure_key]["schema"]
 
         try:
             validated_params = schema().load(measure_params)
         except ValidationError as exc:
             return {
                 "error": f"Metric parameters {measure_key} are not valid",
                 "schema_errors": exc.messages,
-                "code": requests.codes.unprocessable_entity
+                "code": requests.codes.unprocessable_entity,
             }
 
-        interpretation_function = MEASURES_INTERPRETATION_MAPPING[measure_key]["interpretation_function"]
-        result = interpretation_function(validated_params)
+        interpretation_function = MEASURES_INTERPRETATION_MAPPING[measure_key][
+            "interpretation_function"
+        ]
+        threshold_config = {
+            threshold: config["thresholds"][threshold]
+            for threshold in config["thresholds"].keys()
+            if threshold in MEASURES_INTERPRETATION_MAPPING[measure_key]["thresholds"]
+        }
+        result = interpretation_function(validated_params, **threshold_config)
 
-        response_data["measures"].append({
-            "key": measure_key,
-            "value": result,
-        })
+        response_data["measures"].append(
+            {
+                "key": measure_key,
+                "value": result,
+            }
+        )
 
     return response_data
 
 
 def calculate_subcharacteristics(extracted_subcharacteristics):
     try:
         data = CalculateSubCharacteristicSchema().load(extracted_subcharacteristics)
     except ValidationError as error:
         return {
             "error": "Failed to validate request",
             "schema_errors": error.messages,
-            "code": requests.codes.unprocessable_entity
+            "code": requests.codes.unprocessable_entity,
         }
 
     response_data = {"subcharacteristics": []}
 
     for subcharacteristic in data["subcharacteristics"]:
         subcharacteristic_key: str = subcharacteristic["key"]
 
         values_list, weights_list = [], []
         for measure in subcharacteristic["measures"]:
             values_list.append(measure["value"])
             weights_list.append(measure["weight"])
 
         aggregated_value = calculate_aggregated_value(values_list, weights_list)
 
-        response_data["subcharacteristics"].append({
-            "key": subcharacteristic_key,
-            "value": aggregated_value,
-        })
+        response_data["subcharacteristics"].append(
+            {
+                "key": subcharacteristic_key,
+                "value": aggregated_value,
+            }
+        )
 
     return response_data
 
 
 def calculate_characteristics(extracted_characteristics):
     try:
         data = CalculateCharacteristicSchema().load(extracted_characteristics)
     except ValidationError as error:
         return {
             "error": "Failed to validate request",
             "schema_errors": error.messages,
-            "code": requests.codes.unprocessable_entity
+            "code": requests.codes.unprocessable_entity,
         }
 
     response_data = {"characteristics": []}
 
     for characteristic in data["characteristics"]:
         characteristic_key: str = characteristic["key"]
 
         values_list, weights_list = [], []
         for measure in characteristic["subcharacteristics"]:
             values_list.append(measure["value"])
             weights_list.append(measure["weight"])
 
         aggregated_value = calculate_aggregated_value(values_list, weights_list)
 
-        response_data["characteristics"].append({
-            "key": characteristic_key,
-            "value": aggregated_value,
-        })
+        response_data["characteristics"].append(
+            {
+                "key": characteristic_key,
+                "value": aggregated_value,
+            }
+        )
 
     return response_data
 
 
 def calculate_sqc(extracted_sqc):
     try:
         data = CalculateSQCSchema().load(extracted_sqc)
     except ValidationError as error:
         return {
             "error": "Failed to validate request",
             "schema_errors": error.messages,
-            "code": requests.codes.unprocessable_entity
+            "code": requests.codes.unprocessable_entity,
         }
 
     response_data = {"sqc": []}
 
     sqc = data["sqc"]
     sqc_key: str = sqc["key"]
 
     values_list, weights_list = [], []
     for characteristic in sqc["characteristics"]:
         values_list.append(characteristic["value"])
         weights_list.append(characteristic["weight"])
 
     aggregated_value = calculate_aggregated_value(values_list, weights_list)
 
-    response_data["sqc"].append({
-        "key": sqc_key,
-        "value": aggregated_value,
-    })
+    response_data["sqc"].append(
+        {
+            "key": sqc_key,
+            "value": aggregated_value,
+        }
+    )
 
     return response_data
```

### Comparing `msgram_core-1.1.2/src/staticfiles/sonarqube_available_metrics.py` & `msgram_core-1.2.0/src/staticfiles/sonarqube_available_metrics.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,1116 +7,1116 @@
             "key": "new_technical_debt",
             "type": "WORK_DUR",
             "name": "Added Technical Debt",
             "description": "Added technical debt",
             "domain": "Maintainability",
             "direction": -1,
             "qualitative": True,
-            "hidden": False
+            "hidden": False,
         },
         {
             "id": "386",
             "key": "analysis_from_sonarqube_9_4",
             "type": "BOOL",
             "name": "Analysis From SonarQube 9.4",
             "description": "Indicates whether the analysis has been run after the upgrade to SonarQube 9.4. It affects how the issues will be detected for branches that use reference branch as the strategy for detecting new code.",
             "domain": "Issues",
             "direction": 0,
             "qualitative": False,
-            "hidden": True
+            "hidden": True,
         },
         {
             "id": "78",
             "key": "blocker_violations",
             "type": "INT",
             "name": "Blocker Issues",
             "description": "Blocker issues",
             "domain": "Issues",
             "direction": -1,
             "qualitative": True,
-            "hidden": False
+            "hidden": False,
         },
         {
             "id": "308",
             "key": "bugs",
             "type": "INT",
             "name": "Bugs",
             "description": "Bugs",
             "domain": "Reliability",
             "direction": -1,
             "qualitative": False,
-            "hidden": False
+            "hidden": False,
         },
         {
             "id": "4",
             "key": "classes",
             "type": "INT",
             "name": "Classes",
             "description": "Classes",
             "domain": "Size",
             "direction": -1,
             "qualitative": False,
-            "hidden": False
+            "hidden": False,
         },
         {
             "id": "306",
             "key": "code_smells",
             "type": "INT",
             "name": "Code Smells",
             "description": "Code Smells",
             "domain": "Maintainability",
             "direction": -1,
             "qualitative": False,
-            "hidden": False
+            "hidden": False,
         },
         {
             "id": "347",
             "key": "cognitive_complexity",
             "type": "INT",
             "name": "Cognitive Complexity",
             "description": "Cognitive complexity",
             "domain": "Complexity",
             "direction": -1,
             "qualitative": False,
-            "hidden": False
+            "hidden": False,
         },
         {
             "id": "32",
             "key": "comment_lines",
             "type": "INT",
             "name": "Comment Lines",
             "description": "Number of comment lines",
             "domain": "Size",
             "direction": 1,
             "qualitative": False,
-            "hidden": False
+            "hidden": False,
         },
         {
             "id": "239",
             "key": "comment_lines_data",
             "type": "DATA",
             "name": "comment_lines_data",
             "domain": "Size",
             "direction": 0,
             "qualitative": False,
-            "hidden": True
+            "hidden": True,
         },
         {
             "id": "33",
             "key": "comment_lines_density",
             "type": "PERCENT",
             "name": "Comments (%)",
             "description": "Comments balanced by ncloc + comment lines",
             "domain": "Size",
             "direction": 1,
             "qualitative": True,
             "hidden": False,
-            "decimalScale": 1
+            "decimalScale": 1,
         },
         {
             "id": "27",
             "key": "class_complexity",
             "type": "FLOAT",
             "name": "Complexity / Class",
             "description": "Complexity average by class",
             "domain": "Complexity",
             "direction": -1,
             "qualitative": True,
             "hidden": True,
-            "decimalScale": 1
+            "decimalScale": 1,
         },
         {
             "id": "38",
             "key": "file_complexity",
             "type": "FLOAT",
             "name": "Complexity / File",
             "description": "Complexity average by file",
             "domain": "Complexity",
             "direction": -1,
             "qualitative": True,
             "hidden": True,
-            "decimalScale": 1
+            "decimalScale": 1,
         },
         {
             "id": "28",
             "key": "function_complexity",
             "type": "FLOAT",
             "name": "Complexity / Function",
             "description": "Complexity average by function",
             "domain": "Complexity",
             "direction": -1,
             "qualitative": True,
             "hidden": True,
-            "decimalScale": 1
+            "decimalScale": 1,
         },
         {
             "id": "272",
             "key": "complexity_in_classes",
             "type": "INT",
             "name": "Complexity in Classes",
             "description": "Cyclomatic complexity in classes",
             "domain": "Complexity",
             "direction": -1,
             "qualitative": False,
-            "hidden": True
+            "hidden": True,
         },
         {
             "id": "273",
             "key": "complexity_in_functions",
             "type": "INT",
             "name": "Complexity in Functions",
             "description": "Cyclomatic complexity in functions",
             "domain": "Complexity",
             "direction": -1,
             "qualitative": False,
-            "hidden": True
+            "hidden": True,
         },
         {
             "id": "97",
             "key": "branch_coverage",
             "type": "PERCENT",
             "name": "Condition Coverage",
             "description": "Condition coverage",
             "domain": "Coverage",
             "direction": 1,
             "qualitative": True,
             "hidden": False,
-            "decimalScale": 1
+            "decimalScale": 1,
         },
         {
             "id": "178",
             "key": "new_branch_coverage",
             "type": "PERCENT",
             "name": "Condition Coverage on New Code",
             "description": "Condition coverage of new/changed code",
             "domain": "Coverage",
             "direction": 1,
             "qualitative": True,
             "hidden": False,
-            "decimalScale": 1
+            "decimalScale": 1,
         },
         {
             "id": "95",
             "key": "conditions_to_cover",
             "type": "INT",
             "name": "Conditions to Cover",
             "description": "Conditions to cover",
             "domain": "Coverage",
             "direction": -1,
             "qualitative": False,
-            "hidden": False
+            "hidden": False,
         },
         {
             "id": "176",
             "key": "new_conditions_to_cover",
             "type": "INT",
             "name": "Conditions to Cover on New Code",
             "description": "Conditions to cover on new code",
             "domain": "Coverage",
             "direction": -1,
             "qualitative": False,
-            "hidden": False
+            "hidden": False,
         },
         {
             "id": "277",
             "key": "confirmed_issues",
             "type": "INT",
             "name": "Confirmed Issues",
             "description": "Confirmed issues",
             "domain": "Issues",
             "direction": -1,
             "qualitative": True,
-            "hidden": False
+            "hidden": False,
         },
         {
             "id": "20",
             "key": "coverage",
             "type": "PERCENT",
             "name": "Coverage",
             "description": "Coverage by tests",
             "domain": "Coverage",
             "direction": 1,
             "qualitative": True,
             "hidden": False,
-            "decimalScale": 1
+            "decimalScale": 1,
         },
         {
             "id": "172",
             "key": "new_coverage",
             "type": "PERCENT",
             "name": "Coverage on New Code",
             "description": "Coverage of new/changed code",
             "domain": "Coverage",
             "direction": 1,
             "qualitative": True,
             "hidden": False,
-            "decimalScale": 1
+            "decimalScale": 1,
         },
         {
             "id": "79",
             "key": "critical_violations",
             "type": "INT",
             "name": "Critical Issues",
             "description": "Critical issues",
             "domain": "Issues",
             "direction": -1,
             "qualitative": True,
-            "hidden": False
+            "hidden": False,
         },
         {
             "id": "26",
             "key": "complexity",
             "type": "INT",
             "name": "Cyclomatic Complexity",
             "description": "Cyclomatic complexity",
             "domain": "Complexity",
             "direction": -1,
             "qualitative": False,
-            "hidden": False
+            "hidden": False,
         },
         {
             "id": "181",
             "key": "last_commit_date",
             "type": "MILLISEC",
             "name": "Date of Last Commit",
             "domain": "SCM",
             "direction": 0,
             "qualitative": False,
-            "hidden": True
+            "hidden": True,
         },
         {
             "id": "280",
             "key": "development_cost",
             "type": "STRING",
             "name": "Development Cost",
             "description": "Development cost",
             "domain": "Maintainability",
             "direction": -1,
             "qualitative": True,
-            "hidden": True
+            "hidden": True,
         },
         {
             "id": "348",
             "key": "new_development_cost",
             "type": "FLOAT",
             "name": "Development Cost on New Code",
             "description": "Development cost on new code",
             "domain": "Maintainability",
             "direction": -1,
             "qualitative": True,
             "hidden": True,
-            "decimalScale": 1
+            "decimalScale": 1,
         },
         {
             "id": "37",
             "key": "directories",
             "type": "INT",
             "name": "Directories",
             "description": "Directories",
             "domain": "Size",
             "direction": -1,
             "qualitative": False,
-            "hidden": False
+            "hidden": False,
         },
         {
             "id": "51",
             "key": "duplicated_blocks",
             "type": "INT",
             "name": "Duplicated Blocks",
             "description": "Duplicated blocks",
             "domain": "Duplications",
             "direction": -1,
             "qualitative": True,
-            "hidden": False
+            "hidden": False,
         },
         {
             "id": "339",
             "key": "new_duplicated_blocks",
             "type": "INT",
             "name": "Duplicated Blocks on New Code",
             "description": "Duplicated blocks on new code",
             "domain": "Duplications",
             "direction": -1,
             "qualitative": True,
-            "hidden": False
+            "hidden": False,
         },
         {
             "id": "52",
             "key": "duplicated_files",
             "type": "INT",
             "name": "Duplicated Files",
             "description": "Duplicated files",
             "domain": "Duplications",
             "direction": -1,
             "qualitative": True,
-            "hidden": False
+            "hidden": False,
         },
         {
             "id": "8",
             "key": "duplicated_lines",
             "type": "INT",
             "name": "Duplicated Lines",
             "description": "Duplicated lines",
             "domain": "Duplications",
             "direction": -1,
             "qualitative": True,
-            "hidden": False
+            "hidden": False,
         },
         {
             "id": "34",
             "key": "duplicated_lines_density",
             "type": "PERCENT",
             "name": "Duplicated Lines (%)",
             "description": "Duplicated lines balanced by statements",
             "domain": "Duplications",
             "direction": -1,
             "qualitative": True,
             "hidden": False,
-            "decimalScale": 1
+            "decimalScale": 1,
         },
         {
             "id": "340",
             "key": "new_duplicated_lines_density",
             "type": "PERCENT",
             "name": "Duplicated Lines (%) on New Code",
             "description": "Duplicated lines (%) on new code balanced by statements",
             "domain": "Duplications",
             "direction": -1,
             "qualitative": True,
             "hidden": False,
-            "decimalScale": 1
+            "decimalScale": 1,
         },
         {
             "id": "338",
             "key": "new_duplicated_lines",
             "type": "INT",
             "name": "Duplicated Lines on New Code",
             "description": "Duplicated Lines on New Code",
             "domain": "Duplications",
             "direction": -1,
             "qualitative": True,
-            "hidden": False
+            "hidden": False,
         },
         {
             "id": "53",
             "key": "duplications_data",
             "type": "DATA",
             "name": "Duplication Details",
             "description": "Duplications details",
             "domain": "Duplications",
             "direction": 0,
             "qualitative": False,
-            "hidden": False
+            "hidden": False,
         },
         {
             "id": "312",
             "key": "effort_to_reach_maintainability_rating_a",
             "type": "WORK_DUR",
             "name": "Effort to Reach Maintainability Rating A",
             "description": "Effort to reach maintainability rating A",
             "domain": "Maintainability",
             "direction": -1,
             "qualitative": True,
-            "hidden": False
+            "hidden": False,
         },
         {
             "id": "321",
             "key": "executable_lines_data",
             "type": "DATA",
             "name": "executable_lines_data",
             "domain": "Coverage",
             "direction": 0,
             "qualitative": False,
-            "hidden": True
+            "hidden": True,
         },
         {
             "id": "274",
             "key": "False_positive_issues",
             "type": "INT",
             "name": "False Positive Issues",
             "description": "False positive issues",
             "domain": "Issues",
             "direction": -1,
             "qualitative": False,
-            "hidden": False
+            "hidden": False,
         },
         {
             "id": "154",
             "key": "file_complexity_distribution",
             "type": "DISTRIB",
             "name": "File Distribution / Complexity",
             "description": "Files distribution /complexity",
             "domain": "Complexity",
             "direction": 0,
             "qualitative": True,
-            "hidden": True
+            "hidden": True,
         },
         {
             "id": "36",
             "key": "files",
             "type": "INT",
             "name": "Files",
             "description": "Number of files",
             "domain": "Size",
             "direction": -1,
             "qualitative": False,
-            "hidden": False
+            "hidden": False,
         },
         {
             "id": "59",
             "key": "function_complexity_distribution",
             "type": "DISTRIB",
             "name": "Function Distribution / Complexity",
             "description": "Functions distribution /complexity",
             "domain": "Complexity",
             "direction": 0,
             "qualitative": True,
-            "hidden": True
+            "hidden": True,
         },
         {
             "id": "6",
             "key": "functions",
             "type": "INT",
             "name": "Functions",
             "description": "Functions",
             "domain": "Size",
             "direction": -1,
             "qualitative": False,
-            "hidden": False
+            "hidden": False,
         },
         {
             "id": "150",
             "key": "generated_lines",
             "type": "INT",
             "name": "Generated Lines",
             "description": "Number of generated lines",
             "domain": "Size",
             "direction": -1,
             "qualitative": False,
-            "hidden": False
+            "hidden": False,
         },
         {
             "id": "151",
             "key": "generated_ncloc",
             "type": "INT",
             "name": "Generated Lines of Code",
             "description": "Generated non Commenting Lines of Code",
             "domain": "Size",
             "direction": -1,
             "qualitative": False,
-            "hidden": False
+            "hidden": False,
         },
         {
             "id": "82",
             "key": "info_violations",
             "type": "INT",
             "name": "Info Issues",
             "description": "Info issues",
             "domain": "Issues",
             "direction": -1,
             "qualitative": True,
-            "hidden": False
+            "hidden": False,
         },
         {
             "id": "42",
             "key": "violations",
             "type": "INT",
             "name": "Issues",
             "description": "Issues",
             "domain": "Issues",
             "direction": -1,
             "qualitative": True,
-            "hidden": False
+            "hidden": False,
         },
         {
             "id": "94",
             "key": "line_coverage",
             "type": "PERCENT",
             "name": "Line Coverage",
             "description": "Line coverage",
             "domain": "Coverage",
             "direction": 1,
             "qualitative": True,
             "hidden": False,
-            "decimalScale": 1
+            "decimalScale": 1,
         },
         {
             "id": "175",
             "key": "new_line_coverage",
             "type": "PERCENT",
             "name": "Line Coverage on New Code",
             "description": "Line coverage of added/changed code",
             "domain": "Coverage",
             "direction": 1,
             "qualitative": True,
             "hidden": False,
-            "decimalScale": 1
+            "decimalScale": 1,
         },
         {
             "id": "55",
             "key": "lines",
             "type": "INT",
             "name": "Lines",
             "description": "Lines",
             "domain": "Size",
             "direction": -1,
             "qualitative": False,
-            "hidden": False
+            "hidden": False,
         },
         {
             "id": "5",
             "key": "ncloc",
             "type": "INT",
             "name": "Lines of Code",
             "description": "Non commenting lines of code",
             "domain": "Size",
             "direction": -1,
             "qualitative": False,
-            "hidden": False
+            "hidden": False,
         },
         {
             "id": "293",
             "key": "ncloc_language_distribution",
             "type": "DATA",
             "name": "Lines of Code Per Language",
             "description": "Non Commenting Lines of Code Distributed By Language",
             "domain": "Size",
             "direction": -1,
             "qualitative": False,
-            "hidden": False
+            "hidden": False,
         },
         {
             "id": "92",
             "key": "lines_to_cover",
             "type": "INT",
             "name": "Lines to Cover",
             "description": "Lines to cover",
             "domain": "Coverage",
             "direction": -1,
             "qualitative": False,
-            "hidden": False
+            "hidden": False,
         },
         {
             "id": "173",
             "key": "new_lines_to_cover",
             "type": "INT",
             "name": "Lines to Cover on New Code",
             "description": "Lines to cover on new code",
             "domain": "Coverage",
             "direction": -1,
             "qualitative": False,
-            "hidden": False
+            "hidden": False,
         },
         {
             "id": "163",
             "key": "sqale_rating",
             "type": "RATING",
             "name": "Maintainability Rating",
             "description": "A-to-E rating based on the technical debt ratio",
             "domain": "Maintainability",
             "direction": -1,
             "qualitative": True,
-            "hidden": False
+            "hidden": False,
         },
         {
             "id": "341",
             "key": "new_maintainability_rating",
             "type": "RATING",
             "name": "Maintainability Rating on New Code",
             "description": "Maintainability rating on new code",
             "domain": "Maintainability",
             "direction": -1,
             "qualitative": True,
-            "hidden": False
+            "hidden": False,
         },
         {
             "id": "80",
             "key": "major_violations",
             "type": "INT",
             "name": "Major Issues",
             "description": "Major issues",
             "domain": "Issues",
             "direction": -1,
             "qualitative": True,
-            "hidden": False
+            "hidden": False,
         },
         {
             "id": "81",
             "key": "minor_violations",
             "type": "INT",
             "name": "Minor Issues",
             "description": "Minor issues",
             "domain": "Issues",
             "direction": -1,
             "qualitative": True,
-            "hidden": False
+            "hidden": False,
         },
         {
             "id": "238",
             "key": "ncloc_data",
             "type": "DATA",
             "name": "ncloc_data",
             "domain": "Size",
             "direction": 0,
             "qualitative": False,
-            "hidden": True
+            "hidden": True,
         },
         {
             "id": "165",
             "key": "new_blocker_violations",
             "type": "INT",
             "name": "New Blocker Issues",
             "description": "New Blocker issues",
             "domain": "Issues",
             "direction": -1,
             "qualitative": True,
-            "hidden": False
+            "hidden": False,
         },
         {
             "id": "309",
             "key": "new_bugs",
             "type": "INT",
             "name": "New Bugs",
             "description": "New Bugs",
             "domain": "Reliability",
             "direction": -1,
             "qualitative": True,
-            "hidden": False
+            "hidden": False,
         },
         {
             "id": "307",
             "key": "new_code_smells",
             "type": "INT",
             "name": "New Code Smells",
             "description": "New Code Smells",
             "domain": "Maintainability",
             "direction": -1,
             "qualitative": True,
-            "hidden": False
+            "hidden": False,
         },
         {
             "id": "166",
             "key": "new_critical_violations",
             "type": "INT",
             "name": "New Critical Issues",
             "description": "New Critical issues",
             "domain": "Issues",
             "direction": -1,
             "qualitative": True,
-            "hidden": False
+            "hidden": False,
         },
         {
             "id": "169",
             "key": "new_info_violations",
             "type": "INT",
             "name": "New Info Issues",
             "description": "New Info issues",
             "domain": "Issues",
             "direction": -1,
             "qualitative": True,
-            "hidden": False
+            "hidden": False,
         },
         {
             "id": "164",
             "key": "new_violations",
             "type": "INT",
             "name": "New Issues",
             "description": "New issues",
             "domain": "Issues",
             "direction": -1,
             "qualitative": True,
-            "hidden": False
+            "hidden": False,
         },
         {
             "id": "337",
             "key": "new_lines",
             "type": "INT",
             "name": "New Lines",
             "description": "New lines",
             "domain": "Size",
             "direction": -1,
             "qualitative": False,
-            "hidden": False
+            "hidden": False,
         },
         {
             "id": "167",
             "key": "new_major_violations",
             "type": "INT",
             "name": "New Major Issues",
             "description": "New Major issues",
             "domain": "Issues",
             "direction": -1,
             "qualitative": True,
-            "hidden": False
+            "hidden": False,
         },
         {
             "id": "168",
             "key": "new_minor_violations",
             "type": "INT",
             "name": "New Minor Issues",
             "description": "New Minor issues",
             "domain": "Issues",
             "direction": -1,
             "qualitative": True,
-            "hidden": False
+            "hidden": False,
         },
         {
             "id": "351",
             "key": "new_security_hotspots",
             "type": "INT",
             "name": "New Security Hotspots",
             "description": "New Security Hotspots",
             "domain": "SecurityReview",
             "direction": -1,
             "qualitative": True,
-            "hidden": False
+            "hidden": False,
         },
         {
             "id": "311",
             "key": "new_vulnerabilities",
             "type": "INT",
             "name": "New Vulnerabilities",
             "description": "New Vulnerabilities",
             "domain": "Security",
             "direction": -1,
             "qualitative": True,
-            "hidden": False
+            "hidden": False,
         },
         {
             "id": "275",
             "key": "open_issues",
             "type": "INT",
             "name": "Open Issues",
             "description": "Open issues",
             "domain": "Issues",
             "direction": -1,
             "qualitative": False,
-            "hidden": False
+            "hidden": False,
         },
         {
             "id": "47",
             "key": "quality_profiles",
             "type": "DATA",
             "name": "Profiles",
             "description": "Details of quality profiles used during analysis",
             "domain": "General",
             "direction": 0,
             "qualitative": False,
-            "hidden": True
+            "hidden": True,
         },
         {
             "id": "240",
             "key": "projects",
             "type": "INT",
             "name": "Project branches",
             "description": "Number of project branches",
             "domain": "Size",
             "direction": -1,
             "qualitative": False,
-            "hidden": False
+            "hidden": False,
         },
         {
             "id": "58",
             "key": "public_api",
             "type": "INT",
             "name": "Public API",
             "description": "Public API",
             "domain": "Documentation",
             "direction": -1,
             "qualitative": False,
-            "hidden": True
+            "hidden": True,
         },
         {
             "id": "61",
             "key": "public_documented_api_density",
             "type": "PERCENT",
             "name": "Public Documented API (%)",
             "description": "Public documented classes and functions balanced by ncloc",
             "domain": "Documentation",
             "direction": 1,
             "qualitative": True,
             "hidden": True,
-            "decimalScale": 1
+            "decimalScale": 1,
         },
         {
             "id": "62",
             "key": "public_undocumented_api",
             "type": "INT",
             "name": "Public Undocumented API",
             "description": "Public undocumented classes, functions and variables",
             "domain": "Documentation",
             "direction": -1,
             "qualitative": True,
-            "hidden": True
+            "hidden": True,
         },
         {
             "id": "294",
             "key": "quality_gate_details",
             "type": "DATA",
             "name": "Quality Gate Details",
             "description": "The project detailed status with regard to its quality gate",
             "domain": "General",
             "direction": 0,
             "qualitative": False,
-            "hidden": False
+            "hidden": False,
         },
         {
             "id": "48",
             "key": "alert_status",
             "type": "LEVEL",
             "name": "Quality Gate Status",
             "description": "The project status with regard to its quality gate.",
             "domain": "Releasability",
             "direction": 1,
             "qualitative": True,
-            "hidden": False
+            "hidden": False,
         },
         {
             "id": "315",
             "key": "reliability_rating",
             "type": "RATING",
             "name": "Reliability Rating",
             "description": "Reliability rating",
             "domain": "Reliability",
             "direction": -1,
             "qualitative": True,
-            "hidden": False
+            "hidden": False,
         },
         {
             "id": "342",
             "key": "new_reliability_rating",
             "type": "RATING",
             "name": "Reliability Rating on New Code",
             "description": "Reliability rating on new code",
             "domain": "Reliability",
             "direction": -1,
             "qualitative": True,
-            "hidden": False
+            "hidden": False,
         },
         {
             "id": "313",
             "key": "reliability_remediation_effort",
             "type": "WORK_DUR",
             "name": "Reliability Remediation Effort",
             "description": "Reliability Remediation Effort",
             "domain": "Reliability",
             "direction": -1,
             "qualitative": True,
-            "hidden": False
+            "hidden": False,
         },
         {
             "id": "314",
             "key": "new_reliability_remediation_effort",
             "type": "WORK_DUR",
             "name": "Reliability Remediation Effort on New Code",
             "description": "Reliability remediation effort on new code",
             "domain": "Reliability",
             "direction": -1,
             "qualitative": True,
-            "hidden": False
+            "hidden": False,
         },
         {
             "id": "276",
             "key": "reopened_issues",
             "type": "INT",
             "name": "Reopened Issues",
             "description": "Reopened issues",
             "domain": "Issues",
             "direction": -1,
             "qualitative": True,
-            "hidden": False
+            "hidden": False,
         },
         {
             "id": "350",
             "key": "security_hotspots",
             "type": "INT",
             "name": "Security Hotspots",
             "description": "Security Hotspots",
             "domain": "SecurityReview",
             "direction": -1,
             "qualitative": False,
-            "hidden": False
+            "hidden": False,
         },
         {
             "id": "354",
             "key": "security_hotspots_reviewed",
             "type": "PERCENT",
             "name": "Security Hotspots Reviewed",
             "description": "Percentage of Security Hotspots Reviewed",
             "domain": "SecurityReview",
             "direction": 1,
             "qualitative": True,
             "hidden": False,
-            "decimalScale": 1
+            "decimalScale": 1,
         },
         {
             "id": "355",
             "key": "new_security_hotspots_reviewed",
             "type": "PERCENT",
             "name": "Security Hotspots Reviewed on New Code",
             "description": "Percentage of Security Hotspots Reviewed on New Code",
             "domain": "SecurityReview",
             "direction": 1,
             "qualitative": True,
             "hidden": False,
-            "decimalScale": 1
+            "decimalScale": 1,
         },
         {
             "id": "319",
             "key": "security_rating",
             "type": "RATING",
             "name": "Security Rating",
             "description": "Security rating",
             "domain": "Security",
             "direction": -1,
             "qualitative": True,
-            "hidden": False
+            "hidden": False,
         },
         {
             "id": "343",
             "key": "new_security_rating",
             "type": "RATING",
             "name": "Security Rating on New Code",
             "description": "Security rating on new code",
             "domain": "Security",
             "direction": -1,
             "qualitative": True,
-            "hidden": False
+            "hidden": False,
         },
         {
             "id": "317",
             "key": "security_remediation_effort",
             "type": "WORK_DUR",
             "name": "Security Remediation Effort",
             "description": "Security remediation effort",
             "domain": "Security",
             "direction": -1,
             "qualitative": True,
-            "hidden": False
+            "hidden": False,
         },
         {
             "id": "318",
             "key": "new_security_remediation_effort",
             "type": "WORK_DUR",
             "name": "Security Remediation Effort on New Code",
             "description": "Security remediation effort on new code",
             "domain": "Security",
             "direction": -1,
             "qualitative": True,
-            "hidden": False
+            "hidden": False,
         },
         {
             "id": "352",
             "key": "security_review_rating",
             "type": "RATING",
             "name": "Security Review Rating",
             "description": "Security Review Rating",
             "domain": "SecurityReview",
             "direction": -1,
             "qualitative": True,
-            "hidden": False
+            "hidden": False,
         },
         {
             "id": "353",
             "key": "new_security_review_rating",
             "type": "RATING",
             "name": "Security Review Rating on New Code",
             "description": "Security Review Rating on New Code",
             "domain": "SecurityReview",
             "direction": -1,
             "qualitative": True,
-            "hidden": False
+            "hidden": False,
         },
         {
             "id": "356",
             "key": "security_hotspots_reviewed_status",
             "type": "INT",
             "name": "Security Review Reviewed Status",
             "description": "Security Review Reviewed Status",
             "domain": "SecurityReview",
             "direction": -1,
             "qualitative": False,
-            "hidden": True
+            "hidden": True,
         },
         {
             "id": "358",
             "key": "new_security_hotspots_reviewed_status",
             "type": "INT",
             "name": "Security Review Reviewed Status on New Code",
             "description": "Security Review Reviewed Status on New Code",
             "domain": "SecurityReview",
             "direction": -1,
             "qualitative": False,
-            "hidden": True
+            "hidden": True,
         },
         {
             "id": "357",
             "key": "security_hotspots_to_review_status",
             "type": "INT",
             "name": "Security Review To Review Status",
             "description": "Security Review To Review Status",
             "domain": "SecurityReview",
             "direction": -1,
             "qualitative": False,
-            "hidden": True
+            "hidden": True,
         },
         {
             "id": "359",
             "key": "new_security_hotspots_to_review_status",
             "type": "INT",
             "name": "Security Review To Review Status on New Code",
             "description": "Security Review To Review Status on New Code",
             "domain": "SecurityReview",
             "direction": -1,
             "qualitative": False,
-            "hidden": True
+            "hidden": True,
         },
         {
             "id": "11",
             "key": "skipped_tests",
             "type": "INT",
             "name": "Skipped Unit Tests",
             "description": "Number of skipped unit tests",
             "domain": "Coverage",
             "direction": -1,
             "qualitative": True,
-            "hidden": False
+            "hidden": False,
         },
         {
             "id": "60",
             "key": "statements",
             "type": "INT",
             "name": "Statements",
             "description": "Number of statements",
             "domain": "Size",
             "direction": -1,
             "qualitative": False,
-            "hidden": False
+            "hidden": False,
         },
         {
             "id": "162",
             "key": "sqale_index",
             "type": "WORK_DUR",
             "name": "Technical Debt",
             "description": "Total effort (in hours) to fix all the issues on the component and therefore to comply to all the requirements.",
             "domain": "Maintainability",
             "direction": -1,
             "qualitative": True,
-            "hidden": False
+            "hidden": False,
         },
         {
             "id": "297",
             "key": "sqale_debt_ratio",
             "type": "PERCENT",
             "name": "Technical Debt Ratio",
             "description": "Ratio of the actual technical debt compared to the estimated cost to develop the whole source code from scratch",
             "domain": "Maintainability",
             "direction": -1,
             "qualitative": True,
             "hidden": False,
-            "decimalScale": 1
-        }
+            "decimalScale": 1,
+        },
     ],
     "total": 112,
     "p": 1,
-    "ps": 100
+    "ps": 100,
 }
```

### Comparing `msgram_core-1.1.2/src/staticfiles/sonarqube_supported_metrics.py` & `msgram_core-1.2.0/src/staticfiles/sonarqube_supported_metrics.py`

 * *Files identical despite different names*

### Comparing `msgram_core-1.1.2/src/util/check_functions.py` & `msgram_core-1.2.0/src/util/check_functions.py`

 * *Files identical despite different names*

### Comparing `msgram_core-1.1.2/src/util/constants.py` & `msgram_core-1.2.0/src/util/constants.py`

 * *Files 8% similar despite different names*

```diff
@@ -88,51 +88,58 @@
         },
         "team_throughput": {
             "name": "Team Throughput",
             "subcharacteristics": ["functional_completeness"],
             "characteristics": ["functional_suitability"],
             "metrics": [
                 "number_of_resolved_issues_with_US_label_in_the_last_x_days",
-                "total_number_of_issues_with_US_label_in_the_last_x_days"
+                "total_number_of_issues_with_US_label_in_the_last_x_days",
             ],
         },
     },
 }
 
 
 MEASURES_INTERPRETATION_MAPPING = {
     "non_complex_file_density": {
         "interpretation_function": non_complex_files_density,
         "calculation_function": ems_functions.calculate_em1,
         "schema": schemas.NonComplexFileDensitySchema,
+        "thresholds": ["min_complex_files_density", "max_complex_files_density"],
     },
     "commented_file_density": {
         "interpretation_function": commented_files_density,
         "calculation_function": ems_functions.calculate_em2,
         "schema": schemas.CommentedFileDensitySchema,
+        "thresholds": ["min_comment_density", "max_comment_density"],
     },
     "duplication_absense": {
         "interpretation_function": absence_of_duplications,
         "calculation_function": ems_functions.calculate_em3,
         "schema": schemas.DuplicationAbsenceSchema,
+        "thresholds": ["min_duplicated_lines", "max_duplicated_lines"],
     },
     "passed_tests": {
         "interpretation_function": passed_tests,
         "calculation_function": ems_functions.calculate_em4,
         "schema": schemas.PassedTestsSchema,
+        "thresholds": ["min_passed_tests", "max_passed_tests"],
     },
     "test_builds": {
         "interpretation_function": fast_test_builds,
         "calculation_function": ems_functions.calculate_em5,
         "schema": schemas.TestBuildsSchema,
+        "thresholds": ["min_fast_test_time", "max_fast_test_time"],
     },
     "test_coverage": {
         "interpretation_function": test_coverage,
         "calculation_function": ems_functions.calculate_em6,
         "schema": schemas.TestCoverageSchema,
+        "thresholds": ["min_coverage", "max_coverage"],
     },
     "team_throughput": {
         "interpretation_function": ...,
         "calculation_function": ems_functions.calculate_em7,
         "schema": schemas.TeamThroughputSchema,
+        "thresholds": [],
     },
 }
```

### Comparing `msgram_core-1.1.2/src/util/exceptions.py` & `msgram_core-1.2.0/src/util/exceptions.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,26 +1,37 @@
 class MeasureSoftGramCoreException(Exception):
     """Base MeasureSoftGram Core exception"""
+
     pass
 
 
 class InvalidMetricValue(MeasureSoftGramCoreException):
     """Raised when a invalid metric value is provided to the interpretation function"""
+
     pass
 
 
 class InvalidInterpretationFunctionArguments(MeasureSoftGramCoreException):
     """Raised when invalid arguments are provided to an interpretation function"""
+
     pass
 
 
 class ValuesAndWeightsOfDifferentSizes(MeasureSoftGramCoreException):
     """Raised when the length of the weight and values are not equal"""
+
     pass
 
 
 class ImplicitMetricValueError(MeasureSoftGramCoreException):
     """
     Exception levantanda quando uma métrica não é passada e não é possível
     obter seu valor de maneira implícita.
     """
+
+    pass
+
+
+class InvalidThresholdValue(MeasureSoftGramCoreException):
+    """Raised when a invalid threshold value is provided to the interpretation function"""
+
     pass
```

### Comparing `msgram_core-1.1.2/src/util/get_functions.py` & `msgram_core-1.2.0/src/util/get_functions.py`

 * *Files identical despite different names*

### Comparing `msgram_core-1.1.2/tests/test_helpers.py` & `msgram_core-1.2.0/tests/test_helpers.py`

 * *Files identical despite different names*

