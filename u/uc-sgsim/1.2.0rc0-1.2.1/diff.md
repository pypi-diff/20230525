# Comparing `tmp/uc_sgsim-1.2.0rc0.tar.gz` & `tmp/uc_sgsim-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uc_sgsim-1.2.0rc0.tar", last modified: Sat May 13 07:21:17 2023, max compression
+gzip compressed data, was "uc_sgsim-1.2.1.tar", last modified: Thu May 25 16:52:04 2023, max compression
```

## Comparing `uc_sgsim-1.2.0rc0.tar` & `uc_sgsim-1.2.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 07:21:17.248176 uc_sgsim-1.2.0rc0/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-13 07:21:06.000000 uc_sgsim-1.2.0rc0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     8980 2023-05-13 07:21:17.248176 uc_sgsim-1.2.0rc0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8486 2023-05-13 07:21:06.000000 uc_sgsim-1.2.0rc0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-13 07:21:17.248176 uc_sgsim-1.2.0rc0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-13 07:21:06.000000 uc_sgsim-1.2.0rc0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 07:21:17.248176 uc_sgsim-1.2.0rc0/uc_sgsim/
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-13 07:21:06.000000 uc_sgsim-1.2.0rc0/uc_sgsim/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 07:21:17.248176 uc_sgsim-1.2.0rc0/uc_sgsim/c_core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 07:21:06.000000 uc_sgsim-1.2.0rc0/uc_sgsim/c_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    85331 2023-05-13 07:21:06.000000 uc_sgsim-1.2.0rc0/uc_sgsim/c_core/uc_sgsim.dll
--rwxr-xr-x   0 runner    (1001) docker     (123)    41272 2023-05-13 07:21:06.000000 uc_sgsim-1.2.0rc0/uc_sgsim/c_core/uc_sgsim.so
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 07:21:17.248176 uc_sgsim-1.2.0rc0/uc_sgsim/cov_model/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-13 07:21:06.000000 uc_sgsim-1.2.0rc0/uc_sgsim/cov_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-05-13 07:21:06.000000 uc_sgsim-1.2.0rc0/uc_sgsim/cov_model/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-13 07:21:06.000000 uc_sgsim-1.2.0rc0/uc_sgsim/cov_model/model.py
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-13 07:21:06.000000 uc_sgsim-1.2.0rc0/uc_sgsim/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 07:21:17.248176 uc_sgsim-1.2.0rc0/uc_sgsim/krige/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-13 07:21:06.000000 uc_sgsim-1.2.0rc0/uc_sgsim/krige/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-13 07:21:06.000000 uc_sgsim-1.2.0rc0/uc_sgsim/krige/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-05-13 07:21:06.000000 uc_sgsim-1.2.0rc0/uc_sgsim/krige/kriging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 07:21:17.248176 uc_sgsim-1.2.0rc0/uc_sgsim/plot/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-13 07:21:06.000000 uc_sgsim-1.2.0rc0/uc_sgsim/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-05-13 07:21:06.000000 uc_sgsim-1.2.0rc0/uc_sgsim/plot/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5062 2023-05-13 07:21:06.000000 uc_sgsim-1.2.0rc0/uc_sgsim/plot/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-05-13 07:21:06.000000 uc_sgsim-1.2.0rc0/uc_sgsim/random_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     9428 2023-05-13 07:21:06.000000 uc_sgsim-1.2.0rc0/uc_sgsim/sgsim.py
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-05-13 07:21:06.000000 uc_sgsim-1.2.0rc0/uc_sgsim/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 07:21:17.248176 uc_sgsim-1.2.0rc0/uc_sgsim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8980 2023-05-13 07:21:17.000000 uc_sgsim-1.2.0rc0/uc_sgsim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-13 07:21:17.000000 uc_sgsim-1.2.0rc0/uc_sgsim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 07:21:17.000000 uc_sgsim-1.2.0rc0/uc_sgsim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 07:21:17.000000 uc_sgsim-1.2.0rc0/uc_sgsim.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-13 07:21:17.000000 uc_sgsim-1.2.0rc0/uc_sgsim.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-13 07:21:17.000000 uc_sgsim-1.2.0rc0/uc_sgsim.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:52:04.915214 uc_sgsim-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-25 16:51:51.000000 uc_sgsim-1.2.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     9002 2023-05-25 16:52:04.915214 uc_sgsim-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8432 2023-05-25 16:51:51.000000 uc_sgsim-1.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-25 16:52:04.915214 uc_sgsim-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-25 16:51:51.000000 uc_sgsim-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:52:04.911213 uc_sgsim-1.2.1/uc_sgsim/
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-25 16:51:51.000000 uc_sgsim-1.2.1/uc_sgsim/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:52:04.915214 uc_sgsim-1.2.1/uc_sgsim/c_core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 16:51:51.000000 uc_sgsim-1.2.1/uc_sgsim/c_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85843 2023-05-25 16:51:51.000000 uc_sgsim-1.2.1/uc_sgsim/c_core/uc_sgsim.dll
+-rwxr-xr-x   0 runner    (1001) docker     (123)    37024 2023-05-25 16:51:51.000000 uc_sgsim-1.2.1/uc_sgsim/c_core/uc_sgsim.so
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:52:04.915214 uc_sgsim-1.2.1/uc_sgsim/cov_model/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-25 16:51:51.000000 uc_sgsim-1.2.1/uc_sgsim/cov_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-05-25 16:51:51.000000 uc_sgsim-1.2.1/uc_sgsim/cov_model/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-05-25 16:51:51.000000 uc_sgsim-1.2.1/uc_sgsim/cov_model/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-25 16:51:51.000000 uc_sgsim-1.2.1/uc_sgsim/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:52:04.915214 uc_sgsim-1.2.1/uc_sgsim/krige/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-25 16:51:51.000000 uc_sgsim-1.2.1/uc_sgsim/krige/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-25 16:51:51.000000 uc_sgsim-1.2.1/uc_sgsim/krige/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-05-25 16:51:51.000000 uc_sgsim-1.2.1/uc_sgsim/krige/kriging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:52:04.915214 uc_sgsim-1.2.1/uc_sgsim/plot/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-25 16:51:51.000000 uc_sgsim-1.2.1/uc_sgsim/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-05-25 16:51:51.000000 uc_sgsim-1.2.1/uc_sgsim/plot/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5031 2023-05-25 16:51:51.000000 uc_sgsim-1.2.1/uc_sgsim/plot/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-05-25 16:51:51.000000 uc_sgsim-1.2.1/uc_sgsim/random_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9568 2023-05-25 16:51:51.000000 uc_sgsim-1.2.1/uc_sgsim/sgsim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-05-25 16:51:51.000000 uc_sgsim-1.2.1/uc_sgsim/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:52:04.911213 uc_sgsim-1.2.1/uc_sgsim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9002 2023-05-25 16:52:04.000000 uc_sgsim-1.2.1/uc_sgsim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-25 16:52:04.000000 uc_sgsim-1.2.1/uc_sgsim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 16:52:04.000000 uc_sgsim-1.2.1/uc_sgsim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 16:52:04.000000 uc_sgsim-1.2.1/uc_sgsim.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-25 16:52:04.000000 uc_sgsim-1.2.1/uc_sgsim.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-25 16:52:04.000000 uc_sgsim-1.2.1/uc_sgsim.egg-info/top_level.txt
```

### Comparing `uc_sgsim-1.2.0rc0/LICENSE.md` & `uc_sgsim-1.2.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `uc_sgsim-1.2.0rc0/PKG-INFO` & `uc_sgsim-1.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,15 @@
-Metadata-Version: 2.1
-Name: uc_sgsim
-Version: 1.2.0rc0
-Summary: Random Field Generation
-Home-page: https://github.com/Zncl2222/Stochastic_UC_SGSIM
-Author: Zncl2222
-Author-email: 3002shinning@gmail.com
-License: MIT
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Scientific/Engineering :: Mathematics
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
 ![licence](https://img.shields.io/github/license/Zncl2222/Stochastic_UC_SGSIM)
 ![python](https://img.shields.io/pypi/pyversions/uc-sgsim)
 ![language](https://img.shields.io/badge/Solutions-black.svg?style=flat&logo=c%2B%2B)
 ![language](https://img.shields.io/badge/Solutions-black.svg?style=flat&logo=python)
 [![ci](https://github.com/Zncl2222/Stochastic_UC_SGSIM/actions/workflows/github-pre-commit.yml/badge.svg)](https://github.com/Zncl2222/Stochastic_UC_SGSIM/actions/workflows/github-pre-commit.yml)
 [![build](https://github.com/Zncl2222/Stochastic_UC_SGSIM/actions/workflows/cmake.yml/badge.svg)](https://github.com/Zncl2222/Stochastic_UC_SGSIM/actions/workflows/cmake.yml)
 [![build](https://github.com/Zncl2222/Stochastic_UC_SGSIM/actions/workflows/codeql.yml/badge.svg)](https://github.com/Zncl2222/Stochastic_UC_SGSIM/actions/workflows/codeql.yml)
-[![codecov](https://codecov.io/github/Zncl2222/Stochastic_UC_SGSIM/branch/main/graph/badge.svg?token=3qZt0OqDNI)](https://app.codecov.io/github/Zncl2222/Stochastic_UC_SGSIM)
+[![codecov](https://codecov.io/gh/Zncl2222/uc_sgsim/branch/main/graph/badge.svg?token=3qZt0OqDNI)](https://codecov.io/gh/Zncl2222/uc_sgsim)
 
 #### Python Sonar Cloud state
 [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=zncl2222_Stochastic_UC_SGSIM_py&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=zncl2222_Stochastic_UC_SGSIM_py)
 [![Reliability Rating](https://sonarcloud.io/api/project_badges/measure?project=zncl2222_Stochastic_UC_SGSIM_py&metric=reliability_rating)](https://sonarcloud.io/summary/new_code?id=zncl2222_Stochastic_UC_SGSIM_py)
 [![Security Rating](https://sonarcloud.io/api/project_badges/measure?project=zncl2222_Stochastic_UC_SGSIM_py&metric=security_rating)](https://sonarcloud.io/summary/new_code?id=zncl2222_Stochastic_UC_SGSIM_py)
 [![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=zncl2222_Stochastic_UC_SGSIM_py&metric=sqale_rating)](https://sonarcloud.io/summary/new_code?id=zncl2222_Stochastic_UC_SGSIM_py)
 
@@ -161,27 +146,27 @@
    <img src="https://github.com/Zncl2222/Stochastic_SGSIM/blob/main/figure/Variogram.png"  width="50%"/>
    <img src="https://github.com/Zncl2222/Stochastic_SGSIM/blob/main/figure/HIST.png"  width="40%"/>
    <img src="https://github.com/Zncl2222/Stochastic_SGSIM/blob/main/figure/CDF.png"  width="50%"/>
 </p>
 
 ## Future plans
 * 2D unconditional randomfield generation
-* GUI mode in pyhton package
+* GUI mode in pyhton
 * More covariance models
 * More kriging methods (etc. Oridinary Kriging)
 * Performance enhancement
 * More completely documents and easy to use designs.
 
 ## Performance
 <p align="center">
 <img src="https://github.com/Zncl2222/Stochastic_SGSIM/blob/main/figure/C_Cpp_py_comparision.png"  width="70%"/>
 </p>
 
 ```
-Parameters for testing:
+Parameters:
 
 model len = 150
 
 number of realizations = 1000
 
 Range scale = 17.32
```

### Comparing `uc_sgsim-1.2.0rc0/README.md` & `uc_sgsim-1.2.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,32 @@
+Metadata-Version: 2.1
+Name: uc_sgsim
+Version: 1.2.1
+Summary: Random Field Generation
+Home-page: https://github.com/Zncl2222/Stochastic_UC_SGSIM
+Author: Zncl2222
+Author-email: 3002shinning@gmail.com
+License: MIT
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Topic :: Scientific/Engineering :: Mathematics
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
 ![licence](https://img.shields.io/github/license/Zncl2222/Stochastic_UC_SGSIM)
 ![python](https://img.shields.io/pypi/pyversions/uc-sgsim)
 ![language](https://img.shields.io/badge/Solutions-black.svg?style=flat&logo=c%2B%2B)
 ![language](https://img.shields.io/badge/Solutions-black.svg?style=flat&logo=python)
 [![ci](https://github.com/Zncl2222/Stochastic_UC_SGSIM/actions/workflows/github-pre-commit.yml/badge.svg)](https://github.com/Zncl2222/Stochastic_UC_SGSIM/actions/workflows/github-pre-commit.yml)
 [![build](https://github.com/Zncl2222/Stochastic_UC_SGSIM/actions/workflows/cmake.yml/badge.svg)](https://github.com/Zncl2222/Stochastic_UC_SGSIM/actions/workflows/cmake.yml)
 [![build](https://github.com/Zncl2222/Stochastic_UC_SGSIM/actions/workflows/codeql.yml/badge.svg)](https://github.com/Zncl2222/Stochastic_UC_SGSIM/actions/workflows/codeql.yml)
-[![codecov](https://codecov.io/github/Zncl2222/Stochastic_UC_SGSIM/branch/main/graph/badge.svg?token=3qZt0OqDNI)](https://app.codecov.io/github/Zncl2222/Stochastic_UC_SGSIM)
+[![codecov](https://codecov.io/gh/Zncl2222/uc_sgsim/branch/main/graph/badge.svg?token=3qZt0OqDNI)](https://codecov.io/gh/Zncl2222/uc_sgsim)
 
 #### Python Sonar Cloud state
 [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=zncl2222_Stochastic_UC_SGSIM_py&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=zncl2222_Stochastic_UC_SGSIM_py)
 [![Reliability Rating](https://sonarcloud.io/api/project_badges/measure?project=zncl2222_Stochastic_UC_SGSIM_py&metric=reliability_rating)](https://sonarcloud.io/summary/new_code?id=zncl2222_Stochastic_UC_SGSIM_py)
 [![Security Rating](https://sonarcloud.io/api/project_badges/measure?project=zncl2222_Stochastic_UC_SGSIM_py&metric=security_rating)](https://sonarcloud.io/summary/new_code?id=zncl2222_Stochastic_UC_SGSIM_py)
 [![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=zncl2222_Stochastic_UC_SGSIM_py&metric=sqale_rating)](https://sonarcloud.io/summary/new_code?id=zncl2222_Stochastic_UC_SGSIM_py)
 
@@ -146,27 +163,27 @@
    <img src="https://github.com/Zncl2222/Stochastic_SGSIM/blob/main/figure/Variogram.png"  width="50%"/>
    <img src="https://github.com/Zncl2222/Stochastic_SGSIM/blob/main/figure/HIST.png"  width="40%"/>
    <img src="https://github.com/Zncl2222/Stochastic_SGSIM/blob/main/figure/CDF.png"  width="50%"/>
 </p>
 
 ## Future plans
 * 2D unconditional randomfield generation
-* GUI mode in pyhton package
+* GUI mode in pyhton
 * More covariance models
 * More kriging methods (etc. Oridinary Kriging)
 * Performance enhancement
 * More completely documents and easy to use designs.
 
 ## Performance
 <p align="center">
 <img src="https://github.com/Zncl2222/Stochastic_SGSIM/blob/main/figure/C_Cpp_py_comparision.png"  width="70%"/>
 </p>
 
 ```
-Parameters for testing:
+Parameters:
 
 model len = 150
 
 number of realizations = 1000
 
 Range scale = 17.32
```

### Comparing `uc_sgsim-1.2.0rc0/setup.cfg` & `uc_sgsim-1.2.1/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 [metadata]
 name = uc_sgsim
-version = 1.2.0rc0
+version = 1.2.1
 description = Random Field Generation
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Zncl2222/Stochastic_UC_SGSIM
 author = Zncl2222
 author_email = 3002shinning@gmail.com
 license = MIT
 license_file = LICENSE.md
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	License :: OSI Approved :: MIT License
 	Programming Language :: Python :: 3
+	Programming Language :: Python :: 3 :: Only
 	Topic :: Scientific/Engineering :: Mathematics
-python_requires = >=3.9
 
 [options]
 packages = 
 	uc_sgsim
 	uc_sgsim/cov_model
 	uc_sgsim/krige
 	uc_sgsim/plot
 	uc_sgsim/c_core
 install_requires = 
 	matplotlib
 	numpy
 	scipy
+python_requires = >=3.9
 include_package_data = true
 zip_safe = false
 
 [options.package_data]
 * = *.dll, *.so
 
 [egg_info]
```

### Comparing `uc_sgsim-1.2.0rc0/uc_sgsim/c_core/uc_sgsim.dll` & `uc_sgsim-1.2.1/uc_sgsim/c_core/uc_sgsim.dll`

 * *Files 3% similar despite different names*

#### objdump

```diff
@@ -5,20 +5,20 @@
 
 Characteristics 0x2026
 	executable
 	line numbers stripped
 	large address aware
 	DLL
 
-Time/Date		Thu Mar 23 14:59:41 2023
+Time/Date		Wed May 24 15:05:26 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	2
 MinorLinkerVersion	30
-SizeOfCode		0000000000006e00
-SizeOfInitializedData	0000000000009c00
+SizeOfCode		0000000000007000
+SizeOfInitializedData	0000000000009e00
 SizeOfUninitializedData	0000000000000c00
 AddressOfEntryPoint	0000000000001330
 BaseOfCode		0000000000001000
 ImageBase		00000000646c0000
 SectionAlignment	00001000
 FileAlignment		00000200
 MajorOSystemVersion	4
@@ -26,15 +26,15 @@
 MajorImageVersion	0
 MinorImageVersion	0
 MajorSubsystemVersion	5
 MinorSubsystemVersion	2
 Win32Version		00000000
 SizeOfImage		00019000
 SizeOfHeaders		00000600
-CheckSum		0001ae4a
+CheckSum		00019925
 Subsystem		00000003	(Windows CUI)
 DllCharacteristics	00000000
 SizeOfStackReserve	0000000000200000
 SizeOfStackCommit	0000000000001000
 SizeOfHeapReserve	0000000000100000
 SizeOfHeapCommit	0000000000001000
 LoaderFlags		00000000
@@ -124,29 +124,29 @@
  0000e028	00000000 00000000 00000000 00000000 00000000
 
 There is an export table in .edata at 0x646cd000
 
 The Export Tables (interpreted .edata section contents)
 
 Export Flags 			0
-Time/Date stamp 		641c695d
+Time/Date stamp 		646e27b6
 Major/Minor 			0/0
 Name 				000000000000d28a uc_sgsim.dll
 Ordinal Base 			1
 Number in:
 	Export Address Table 		0000003d
 	[Name Pointer/Ordinal] Table	0000003d
 Table Addresses
 	Export Address Table 		000000000000d028
 	Name Pointer Table 		000000000000d11c
 	Ordinal Table 			000000000000d210
 
 Export Address Table -- Ordinal Base 1
-	[   0] +base[   1] 4e20 Export RVA
-	[   1] +base[   2] 4289 Export RVA
+	[   0] +base[   1] 4eb0 Export RVA
+	[   1] +base[   2] 4329 Export RVA
 	[   2] +base[   3] 18e2 Export RVA
 	[   3] +base[   4] 1704 Export RVA
 	[   4] +base[   5] 13b0 Export RVA
 	[   5] +base[   6] 1543 Export RVA
 	[   6] +base[   7] 278e Export RVA
 	[   7] +base[   8] 2752 Export RVA
 	[   8] +base[   9] 26db Export RVA
@@ -167,45 +167,45 @@
 	[  23] +base[  24] 2371 Export RVA
 	[  24] +base[  25] 2253 Export RVA
 	[  25] +base[  26] 22e1 Export RVA
 	[  26] +base[  27] 29c8 Export RVA
 	[  27] +base[  28] 296e Export RVA
 	[  28] +base[  29] 292e Export RVA
 	[  29] +base[  30] 294c Export RVA
-	[  30] +base[  31] 2f06 Export RVA
-	[  31] +base[  32] 2fcf Export RVA
+	[  30] +base[  31] 2f24 Export RVA
+	[  31] +base[  32] 302e Export RVA
 	[  32] +base[  33] 2ec0 Export RVA
-	[  33] +base[  34] 42e1 Export RVA
-	[  34] +base[  35] 383d Export RVA
-	[  35] +base[  36] 39da Export RVA
-	[  36] +base[  37] 31bd Export RVA
-	[  37] +base[  38] 3ef8 Export RVA
-	[  38] +base[  39] 3b7a Export RVA
-	[  39] +base[  40] 43f0 Export RVA
+	[  33] +base[  34] 4381 Export RVA
+	[  34] +base[  35] 38c7 Export RVA
+	[  35] +base[  36] 3a7b Export RVA
+	[  36] +base[  37] 325d Export RVA
+	[  37] +base[  38] 3f98 Export RVA
+	[  38] +base[  39] 3c1a Export RVA
+	[  39] +base[  40] 4490 Export RVA
 	[  40] +base[  41] 2aae Export RVA
 	[  41] +base[  42] 2d5e Export RVA
 	[  42] +base[  43] 2db2 Export RVA
 	[  43] +base[  44] 2caa Export RVA
 	[  44] +base[  45] 2cf4 Export RVA
 	[  45] +base[  46] 2c6d Export RVA
 	[  46] +base[  47] 2a30 Export RVA
 	[  47] +base[  48] 2e27 Export RVA
-	[  48] +base[  49] 433d Export RVA
-	[  49] +base[  50] 5021 Export RVA
-	[  50] +base[  51] 4630 Export RVA
-	[  51] +base[  52] 30e0 Export RVA
-	[  52] +base[  53] 3191 Export RVA
-	[  53] +base[  54] 447d Export RVA
-	[  54] +base[  55] 46e0 Export RVA
-	[  55] +base[  56] 4745 Export RVA
-	[  56] +base[  57] 4c08 Export RVA
-	[  57] +base[  58] 3413 Export RVA
-	[  58] +base[  59] 4c90 Export RVA
-	[  59] +base[  60] 530c Export RVA
-	[  60] +base[  61] 5090 Export RVA
+	[  48] +base[  49] 43dd Export RVA
+	[  49] +base[  50] 50b1 Export RVA
+	[  50] +base[  51] 46d0 Export RVA
+	[  51] +base[  52] 3180 Export RVA
+	[  52] +base[  53] 3231 Export RVA
+	[  53] +base[  54] 451d Export RVA
+	[  54] +base[  55] 4780 Export RVA
+	[  55] +base[  56] 47e5 Export RVA
+	[  56] +base[  57] 4c9b Export RVA
+	[  57] +base[  58] 34b9 Export RVA
+	[  58] +base[  59] 4d20 Export RVA
+	[  59] +base[  60] 539c Export RVA
+	[  60] +base[  61] 5120 Export RVA
 
 [Ordinal/Name Pointer] Table
 	[   0] Partition2d
 	[   1] arange
 	[   2] c_array_max_double
 	[   3] c_array_max_float
 	[   4] c_array_max_int
@@ -307,93 +307,93 @@
  00000000646ca1b0:	00000000646c2aae 00000000646c2c6d 00000000646cb190
  00000000646ca1bc:	00000000646c2c6d 00000000646c2caa 00000000646cb19c
  00000000646ca1c8:	00000000646c2caa 00000000646c2cf4 00000000646cb1a8
  00000000646ca1d4:	00000000646c2cf4 00000000646c2d5e 00000000646cb1b4
  00000000646ca1e0:	00000000646c2d5e 00000000646c2db2 00000000646cb1c0
  00000000646ca1ec:	00000000646c2db2 00000000646c2e27 00000000646cb1cc
  00000000646ca1f8:	00000000646c2e27 00000000646c2eba 00000000646cb1d8
- 00000000646ca204:	00000000646c2ec0 00000000646c2f06 00000000646cb1e8
- 00000000646ca210:	00000000646c2f06 00000000646c2fcf 00000000646cb1f0
- 00000000646ca21c:	00000000646c2fcf 00000000646c30db 00000000646cb1fc
- 00000000646ca228:	00000000646c30e0 00000000646c3191 00000000646cb208
- 00000000646ca234:	00000000646c3191 00000000646c31bd 00000000646cb214
- 00000000646ca240:	00000000646c31bd 00000000646c3413 00000000646cb21c
- 00000000646ca24c:	00000000646c3413 00000000646c383d 00000000646cb228
- 00000000646ca258:	00000000646c383d 00000000646c39da 00000000646cb238
- 00000000646ca264:	00000000646c39da 00000000646c3b24 00000000646cb244
- 00000000646ca270:	00000000646c3b30 00000000646c3b7a 00000000646cb250
- 00000000646ca27c:	00000000646c3b7a 00000000646c3ef8 00000000646cb25c
- 00000000646ca288:	00000000646c3ef8 00000000646c4289 00000000646cb26c
- 00000000646ca294:	00000000646c4289 00000000646c42e1 00000000646cb278
- 00000000646ca2a0:	00000000646c42e1 00000000646c433d 00000000646cb284
- 00000000646ca2ac:	00000000646c433d 00000000646c43f0 00000000646cb290
- 00000000646ca2b8:	00000000646c43f0 00000000646c447d 00000000646cb29c
- 00000000646ca2c4:	00000000646c447d 00000000646c462b 00000000646cb2a8
- 00000000646ca2d0:	00000000646c4630 00000000646c46df 00000000646cb2b4
- 00000000646ca2dc:	00000000646c46e0 00000000646c4745 00000000646cb2c0
- 00000000646ca2e8:	00000000646c4745 00000000646c4c08 00000000646cb2cc
- 00000000646ca2f4:	00000000646c4c08 00000000646c4c2b 00000000646cb2d8
- 00000000646ca300:	00000000646c4c2b 00000000646c4c85 00000000646cb2e4
- 00000000646ca30c:	00000000646c4c90 00000000646c4e20 00000000646cb2f0
- 00000000646ca318:	00000000646c4e20 00000000646c5021 00000000646cb2fc
- 00000000646ca324:	00000000646c5021 00000000646c5088 00000000646cb308
- 00000000646ca330:	00000000646c5090 00000000646c530c 00000000646cb314
- 00000000646ca33c:	00000000646c530c 00000000646c53f4 00000000646cb324
- 00000000646ca348:	00000000646c5410 00000000646c5445 00000000646cb330
- 00000000646ca354:	00000000646c5450 00000000646c54b6 00000000646cb338
- 00000000646ca360:	00000000646c54c0 00000000646c54df 00000000646cb344
- 00000000646ca36c:	00000000646c54e0 00000000646c55b6 00000000646cb348
- 00000000646ca378:	00000000646c55c0 00000000646c56b8 00000000646cb358
- 00000000646ca384:	00000000646c56c0 00000000646c56ef 00000000646cb368
- 00000000646ca390:	00000000646c56f0 00000000646c5763 00000000646cb370
- 00000000646ca39c:	00000000646c5770 00000000646c5773 00000000646cb37c
- 00000000646ca3a8:	00000000646c5780 00000000646c5784 00000000646cb380
- 00000000646ca3b4:	00000000646c5790 00000000646c5794 00000000646cb384
- 00000000646ca3c0:	00000000646c57a0 00000000646c596d 00000000646cb394
- 00000000646ca3cc:	00000000646c5970 00000000646c5c2b 00000000646cb3a4
- 00000000646ca3d8:	00000000646c5c30 00000000646c5dd0 00000000646cb3bc
- 00000000646ca3e4:	00000000646c5dd0 00000000646c5ebc 00000000646cb3c4
- 00000000646ca3f0:	00000000646c5ec0 00000000646c60a7 00000000646cb3d4
- 00000000646ca3fc:	00000000646c60b0 00000000646c611a 00000000646cb3dc
- 00000000646ca408:	00000000646c6120 00000000646c619f 00000000646cb3ec
- 00000000646ca414:	00000000646c61a0 00000000646c6240 00000000646cb3fc
- 00000000646ca420:	00000000646c6240 00000000646c631a 00000000646cb404
- 00000000646ca42c:	00000000646c6320 00000000646c633e 00000000646cb40c
- 00000000646ca438:	00000000646c6340 00000000646c6352 00000000646cb410
- 00000000646ca444:	00000000646c6360 00000000646c63a4 00000000646cb414
- 00000000646ca450:	00000000646c63b0 00000000646c643d 00000000646cb418
- 00000000646ca45c:	00000000646c6440 00000000646c64b4 00000000646cb424
- 00000000646ca468:	00000000646c64c0 00000000646c64fe 00000000646cb42c
- 00000000646ca474:	00000000646c6500 00000000646c656f 00000000646cb434
- 00000000646ca480:	00000000646c6570 00000000646c65a7 00000000646cb43c
- 00000000646ca48c:	00000000646c65b0 00000000646c6641 00000000646cb444
- 00000000646ca498:	00000000646c6650 00000000646c66f6 00000000646cb44c
- 00000000646ca4a4:	00000000646c6700 00000000646c6703 00000000646cb454
- 00000000646ca4b0:	00000000646c6750 00000000646c6756 00000000646cb458
- 00000000646ca4bc:	00000000646c6760 00000000646c6766 00000000646cb45c
- 00000000646ca4c8:	00000000646c6770 00000000646c67c4 00000000646cb460
- 00000000646ca4d4:	00000000646c67d0 00000000646c68f6 00000000646cb464
- 00000000646ca4e0:	00000000646c6900 00000000646c6905 00000000646cb470
- 00000000646ca4ec:	00000000646c6910 00000000646c69e7 00000000646cb474
- 00000000646ca4f8:	00000000646c69f0 00000000646c6ae4 00000000646cb478
- 00000000646ca504:	00000000646c6b20 00000000646c6d04 00000000646cb484
- 00000000646ca510:	00000000646c6d10 00000000646c6e30 00000000646cb490
- 00000000646ca51c:	00000000646c6e30 00000000646c6ec6 00000000646cb49c
- 00000000646ca528:	00000000646c6ed0 00000000646c7427 00000000646cb4a4
- 00000000646ca534:	00000000646c7430 00000000646c76ae 00000000646cb4c0
- 00000000646ca540:	00000000646c7780 00000000646c783e 00000000646cb4cc
- 00000000646ca54c:	00000000646c7960 00000000646c7985 00000000646cb4d4
- 00000000646ca558:	00000000646c7990 00000000646c7a58 00000000646cb4d8
- 00000000646ca564:	00000000646c7a60 00000000646c7acf 00000000646cb4e8
- 00000000646ca570:	00000000646c7ad0 00000000646c7aef 00000000646cb4f4
- 00000000646ca57c:	00000000646c7bc0 00000000646c7c01 00000000646cb4fc
- 00000000646ca588:	00000000646c7c10 00000000646c7c1c 00000000646cb504
- 00000000646ca594:	00000000646c7c20 00000000646c7d1c 00000000646cb508
- 00000000646ca5a0:	00000000646c7d30 00000000646c7d99 00000000646cb388
- 00000000646ca5ac:	00000000646c7da0 00000000646c7da5 00000000646cb520
+ 00000000646ca204:	00000000646c2ec0 00000000646c2f24 00000000646cb1e8
+ 00000000646ca210:	00000000646c2f24 00000000646c302e 00000000646cb1f0
+ 00000000646ca21c:	00000000646c302e 00000000646c317b 00000000646cb1fc
+ 00000000646ca228:	00000000646c3180 00000000646c3231 00000000646cb208
+ 00000000646ca234:	00000000646c3231 00000000646c325d 00000000646cb214
+ 00000000646ca240:	00000000646c325d 00000000646c34b9 00000000646cb21c
+ 00000000646ca24c:	00000000646c34b9 00000000646c38c7 00000000646cb228
+ 00000000646ca258:	00000000646c38c7 00000000646c3a7b 00000000646cb238
+ 00000000646ca264:	00000000646c3a7b 00000000646c3bc5 00000000646cb244
+ 00000000646ca270:	00000000646c3bd0 00000000646c3c1a 00000000646cb250
+ 00000000646ca27c:	00000000646c3c1a 00000000646c3f98 00000000646cb25c
+ 00000000646ca288:	00000000646c3f98 00000000646c4329 00000000646cb26c
+ 00000000646ca294:	00000000646c4329 00000000646c4381 00000000646cb278
+ 00000000646ca2a0:	00000000646c4381 00000000646c43dd 00000000646cb284
+ 00000000646ca2ac:	00000000646c43dd 00000000646c4490 00000000646cb290
+ 00000000646ca2b8:	00000000646c4490 00000000646c451d 00000000646cb29c
+ 00000000646ca2c4:	00000000646c451d 00000000646c46cb 00000000646cb2a8
+ 00000000646ca2d0:	00000000646c46d0 00000000646c477f 00000000646cb2b4
+ 00000000646ca2dc:	00000000646c4780 00000000646c47e5 00000000646cb2c0
+ 00000000646ca2e8:	00000000646c47e5 00000000646c4c9b 00000000646cb2cc
+ 00000000646ca2f4:	00000000646c4c9b 00000000646c4cbe 00000000646cb2d8
+ 00000000646ca300:	00000000646c4cbe 00000000646c4d18 00000000646cb2e4
+ 00000000646ca30c:	00000000646c4d20 00000000646c4eb0 00000000646cb2f0
+ 00000000646ca318:	00000000646c4eb0 00000000646c50b1 00000000646cb2fc
+ 00000000646ca324:	00000000646c50b1 00000000646c5118 00000000646cb308
+ 00000000646ca330:	00000000646c5120 00000000646c539c 00000000646cb314
+ 00000000646ca33c:	00000000646c539c 00000000646c5484 00000000646cb324
+ 00000000646ca348:	00000000646c54a0 00000000646c54d5 00000000646cb330
+ 00000000646ca354:	00000000646c54e0 00000000646c5546 00000000646cb338
+ 00000000646ca360:	00000000646c5550 00000000646c556f 00000000646cb344
+ 00000000646ca36c:	00000000646c5570 00000000646c5646 00000000646cb348
+ 00000000646ca378:	00000000646c5650 00000000646c5748 00000000646cb358
+ 00000000646ca384:	00000000646c5750 00000000646c577f 00000000646cb368
+ 00000000646ca390:	00000000646c5780 00000000646c57f3 00000000646cb370
+ 00000000646ca39c:	00000000646c5800 00000000646c5803 00000000646cb37c
+ 00000000646ca3a8:	00000000646c5810 00000000646c5814 00000000646cb380
+ 00000000646ca3b4:	00000000646c5820 00000000646c5824 00000000646cb384
+ 00000000646ca3c0:	00000000646c5830 00000000646c59fd 00000000646cb394
+ 00000000646ca3cc:	00000000646c5a00 00000000646c5cbb 00000000646cb3a4
+ 00000000646ca3d8:	00000000646c5cc0 00000000646c5e60 00000000646cb3bc
+ 00000000646ca3e4:	00000000646c5e60 00000000646c5f4c 00000000646cb3c4
+ 00000000646ca3f0:	00000000646c5f50 00000000646c6137 00000000646cb3d4
+ 00000000646ca3fc:	00000000646c6140 00000000646c61aa 00000000646cb3dc
+ 00000000646ca408:	00000000646c61b0 00000000646c622f 00000000646cb3ec
+ 00000000646ca414:	00000000646c6230 00000000646c62d0 00000000646cb3fc
+ 00000000646ca420:	00000000646c62d0 00000000646c63aa 00000000646cb404
+ 00000000646ca42c:	00000000646c63b0 00000000646c63ce 00000000646cb40c
+ 00000000646ca438:	00000000646c63d0 00000000646c63e2 00000000646cb410
+ 00000000646ca444:	00000000646c63f0 00000000646c6434 00000000646cb414
+ 00000000646ca450:	00000000646c6440 00000000646c64cd 00000000646cb418
+ 00000000646ca45c:	00000000646c64d0 00000000646c6544 00000000646cb424
+ 00000000646ca468:	00000000646c6550 00000000646c658e 00000000646cb42c
+ 00000000646ca474:	00000000646c6590 00000000646c65ff 00000000646cb434
+ 00000000646ca480:	00000000646c6600 00000000646c6637 00000000646cb43c
+ 00000000646ca48c:	00000000646c6640 00000000646c66d1 00000000646cb444
+ 00000000646ca498:	00000000646c66e0 00000000646c6786 00000000646cb44c
+ 00000000646ca4a4:	00000000646c6790 00000000646c6793 00000000646cb454
+ 00000000646ca4b0:	00000000646c67e0 00000000646c67e6 00000000646cb458
+ 00000000646ca4bc:	00000000646c67f0 00000000646c67f6 00000000646cb45c
+ 00000000646ca4c8:	00000000646c6800 00000000646c6854 00000000646cb460
+ 00000000646ca4d4:	00000000646c6860 00000000646c6986 00000000646cb464
+ 00000000646ca4e0:	00000000646c6990 00000000646c6995 00000000646cb470
+ 00000000646ca4ec:	00000000646c69a0 00000000646c6a77 00000000646cb474
+ 00000000646ca4f8:	00000000646c6a80 00000000646c6b74 00000000646cb478
+ 00000000646ca504:	00000000646c6bb0 00000000646c6d94 00000000646cb484
+ 00000000646ca510:	00000000646c6da0 00000000646c6ec0 00000000646cb490
+ 00000000646ca51c:	00000000646c6ec0 00000000646c6f56 00000000646cb49c
+ 00000000646ca528:	00000000646c6f60 00000000646c74b7 00000000646cb4a4
+ 00000000646ca534:	00000000646c74c0 00000000646c773e 00000000646cb4c0
+ 00000000646ca540:	00000000646c7810 00000000646c78ce 00000000646cb4cc
+ 00000000646ca54c:	00000000646c79f0 00000000646c7a15 00000000646cb4d4
+ 00000000646ca558:	00000000646c7a20 00000000646c7ae8 00000000646cb4d8
+ 00000000646ca564:	00000000646c7af0 00000000646c7b5f 00000000646cb4e8
+ 00000000646ca570:	00000000646c7b60 00000000646c7b7f 00000000646cb4f4
+ 00000000646ca57c:	00000000646c7c50 00000000646c7c91 00000000646cb4fc
+ 00000000646ca588:	00000000646c7ca0 00000000646c7cac 00000000646cb504
+ 00000000646ca594:	00000000646c7cb0 00000000646c7dac 00000000646cb508
+ 00000000646ca5a0:	00000000646c7dc0 00000000646c7e29 00000000646cb388
+ 00000000646ca5ac:	00000000646c7e30 00000000646c7e35 00000000646cb520
 
 Dump of .xdata
  00000000646cb000 (rva: 0000b000): 00000000646c1000 - 00000000646c100c
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
  00000000646cb004 (rva: 0000b004): 00000000646c1010 - 00000000646c11ff
 	Version: 1, Flags: none
@@ -638,455 +638,454 @@
  00000000646cb1d8 (rva: 0000b1d8): 00000000646c2e27 - 00000000646c2eba
 	Version: 1, Flags: none
 	Nbr codes: 5, Prologue size: 0x0c, Frame offset: 0x0, Frame reg: rbp
 	  pc+0x0c: save xmm6 at rsp + 0x40
 	  pc+0x08: alloc small area: rsp = rsp - 0x50
 	  pc+0x04: FPReg: rbp = rsp + 0x0 (info = 0x0)
 	  pc+0x01: push rbp
- 00000000646cb1e8 (rva: 0000b1e8): 00000000646c2ec0 - 00000000646c2f06
+ 00000000646cb1e8 (rva: 0000b1e8): 00000000646c2ec0 - 00000000646c2f24
 	Version: 1, Flags: none
 	Nbr codes: 2, Prologue size: 0x04, Frame offset: 0x0, Frame reg: rbp
 	  pc+0x04: FPReg: rbp = rsp + 0x0 (info = 0x0)
 	  pc+0x01: push rbp
- 00000000646cb1f0 (rva: 0000b1f0): 00000000646c2f06 - 00000000646c2fcf
+ 00000000646cb1f0 (rva: 0000b1f0): 00000000646c2f24 - 00000000646c302e
 	Version: 1, Flags: none
 	Nbr codes: 3, Prologue size: 0x08, Frame offset: 0x0, Frame reg: rbp
-	  pc+0x08: alloc small area: rsp = rsp - 0x30
+	  pc+0x08: alloc small area: rsp = rsp - 0x40
 	  pc+0x04: FPReg: rbp = rsp + 0x0 (info = 0x0)
 	  pc+0x01: push rbp
- 00000000646cb1fc (rva: 0000b1fc): 00000000646c2fcf - 00000000646c30db
+ 00000000646cb1fc (rva: 0000b1fc): 00000000646c302e - 00000000646c317b
 	Version: 1, Flags: none
 	Nbr codes: 3, Prologue size: 0x08, Frame offset: 0x0, Frame reg: rbp
-	  pc+0x08: alloc small area: rsp = rsp - 0x30
+	  pc+0x08: alloc small area: rsp = rsp - 0x40
 	  pc+0x04: FPReg: rbp = rsp + 0x0 (info = 0x0)
 	  pc+0x01: push rbp
- 00000000646cb208 (rva: 0000b208): 00000000646c30e0 - 00000000646c3191
+ 00000000646cb208 (rva: 0000b208): 00000000646c3180 - 00000000646c3231
 	Version: 1, Flags: none
 	Nbr codes: 3, Prologue size: 0x08, Frame offset: 0x0, Frame reg: rbp
 	  pc+0x08: alloc small area: rsp = rsp - 0x20
 	  pc+0x04: FPReg: rbp = rsp + 0x0 (info = 0x0)
 	  pc+0x01: push rbp
- 00000000646cb214 (rva: 0000b214): 00000000646c3191 - 00000000646c31bd
+ 00000000646cb214 (rva: 0000b214): 00000000646c3231 - 00000000646c325d
 	Version: 1, Flags: none
 	Nbr codes: 2, Prologue size: 0x04, Frame offset: 0x0, Frame reg: rbp
 	  pc+0x04: FPReg: rbp = rsp + 0x0 (info = 0x0)
 	  pc+0x01: push rbp
- 00000000646cb21c (rva: 0000b21c): 00000000646c31bd - 00000000646c3413
+ 00000000646cb21c (rva: 0000b21c): 00000000646c325d - 00000000646c34b9
 	Version: 1, Flags: none
 	Nbr codes: 4, Prologue size: 0x0e, Frame offset: 0x8, Frame reg: rbp
 	  pc+0x0e: FPReg: rbp = rsp + 0x80 (info = 0x0)
 	  pc+0x06: alloc small area: rsp = rsp - 0x38
 	  pc+0x02: push rbx
 	  pc+0x01: push rbp
- 00000000646cb228 (rva: 0000b228): 00000000646c3413 - 00000000646c383d
+ 00000000646cb228 (rva: 0000b228): 00000000646c34b9 - 00000000646c38c7
 	Version: 1, Flags: none
 	Nbr codes: 5, Prologue size: 0x0c, Frame offset: 0x0, Frame reg: rbp
-	  pc+0x0c: save xmm6 at rsp + 0x40
-	  pc+0x08: alloc small area: rsp = rsp - 0x50
+	  pc+0x0c: save xmm6 at rsp + 0x30
+	  pc+0x08: alloc small area: rsp = rsp - 0x40
 	  pc+0x04: FPReg: rbp = rsp + 0x0 (info = 0x0)
 	  pc+0x01: push rbp
- 00000000646cb238 (rva: 0000b238): 00000000646c383d - 00000000646c39da
+ 00000000646cb238 (rva: 0000b238): 00000000646c38c7 - 00000000646c3a7b
 	Version: 1, Flags: none
-	Nbr codes: 4, Prologue size: 0x0e, Frame offset: 0x8, Frame reg: rbp
-	  pc+0x0e: FPReg: rbp = rsp + 0x80 (info = 0x0)
-	  pc+0x06: alloc small area: rsp = rsp - 0x38
-	  pc+0x02: push rbx
+	Nbr codes: 3, Prologue size: 0x08, Frame offset: 0x0, Frame reg: rbp
+	  pc+0x08: alloc small area: rsp = rsp - 0x30
+	  pc+0x04: FPReg: rbp = rsp + 0x0 (info = 0x0)
 	  pc+0x01: push rbp
- 00000000646cb244 (rva: 0000b244): 00000000646c39da - 00000000646c3b24
+ 00000000646cb244 (rva: 0000b244): 00000000646c3a7b - 00000000646c3bc5
 	Version: 1, Flags: none
 	Nbr codes: 3, Prologue size: 0x08, Frame offset: 0x0, Frame reg: rbp
 	  pc+0x08: alloc small area: rsp = rsp - 0x30
 	  pc+0x04: FPReg: rbp = rsp + 0x0 (info = 0x0)
 	  pc+0x01: push rbp
- 00000000646cb250 (rva: 0000b250): 00000000646c3b30 - 00000000646c3b7a
+ 00000000646cb250 (rva: 0000b250): 00000000646c3bd0 - 00000000646c3c1a
 	Version: 1, Flags: none
 	Nbr codes: 3, Prologue size: 0x08, Frame offset: 0x0, Frame reg: rbp
 	  pc+0x08: alloc small area: rsp = rsp - 0x30
 	  pc+0x04: FPReg: rbp = rsp + 0x0 (info = 0x0)
 	  pc+0x01: push rbp
- 00000000646cb25c (rva: 0000b25c): 00000000646c3b7a - 00000000646c3ef8
+ 00000000646cb25c (rva: 0000b25c): 00000000646c3c1a - 00000000646c3f98
 	Version: 1, Flags: none
 	Nbr codes: 5, Prologue size: 0x11, Frame offset: 0x8, Frame reg: rbp
 	  pc+0x11: FPReg: rbp = rsp + 0x80 (info = 0x0)
 	  pc+0x09: alloc large area: rsp = rsp - 0xd8
 	  pc+0x02: push rbx
 	  pc+0x01: push rbp
- 00000000646cb26c (rva: 0000b26c): 00000000646c3ef8 - 00000000646c4289
+ 00000000646cb26c (rva: 0000b26c): 00000000646c3f98 - 00000000646c4329
 	Version: 1, Flags: none
 	Nbr codes: 3, Prologue size: 0x08, Frame offset: 0x0, Frame reg: rbp
 	  pc+0x08: alloc small area: rsp = rsp - 0x20
 	  pc+0x04: FPReg: rbp = rsp + 0x0 (info = 0x0)
 	  pc+0x01: push rbp
- 00000000646cb278 (rva: 0000b278): 00000000646c4289 - 00000000646c42e1
+ 00000000646cb278 (rva: 0000b278): 00000000646c4329 - 00000000646c4381
 	Version: 1, Flags: none
 	Nbr codes: 3, Prologue size: 0x08, Frame offset: 0x0, Frame reg: rbp
 	  pc+0x08: alloc small area: rsp = rsp - 0x30
 	  pc+0x04: FPReg: rbp = rsp + 0x0 (info = 0x0)
 	  pc+0x01: push rbp
- 00000000646cb284 (rva: 0000b284): 00000000646c42e1 - 00000000646c433d
+ 00000000646cb284 (rva: 0000b284): 00000000646c4381 - 00000000646c43dd
 	Version: 1, Flags: none
 	Nbr codes: 3, Prologue size: 0x08, Frame offset: 0x0, Frame reg: rbp
 	  pc+0x08: alloc small area: rsp = rsp - 0x30
 	  pc+0x04: FPReg: rbp = rsp + 0x0 (info = 0x0)
 	  pc+0x01: push rbp
- 00000000646cb290 (rva: 0000b290): 00000000646c433d - 00000000646c43f0
+ 00000000646cb290 (rva: 0000b290): 00000000646c43dd - 00000000646c4490
 	Version: 1, Flags: none
 	Nbr codes: 3, Prologue size: 0x08, Frame offset: 0x0, Frame reg: rbp
 	  pc+0x08: alloc small area: rsp = rsp - 0x10
 	  pc+0x04: FPReg: rbp = rsp + 0x0 (info = 0x0)
 	  pc+0x01: push rbp
- 00000000646cb29c (rva: 0000b29c): 00000000646c43f0 - 00000000646c447d
+ 00000000646cb29c (rva: 0000b29c): 00000000646c4490 - 00000000646c451d
 	Version: 1, Flags: none
 	Nbr codes: 3, Prologue size: 0x08, Frame offset: 0x0, Frame reg: rbp
 	  pc+0x08: alloc small area: rsp = rsp - 0x10
 	  pc+0x04: FPReg: rbp = rsp + 0x0 (info = 0x0)
 	  pc+0x01: push rbp
- 00000000646cb2a8 (rva: 0000b2a8): 00000000646c447d - 00000000646c462b
+ 00000000646cb2a8 (rva: 0000b2a8): 00000000646c451d - 00000000646c46cb
 	Version: 1, Flags: none
 	Nbr codes: 4, Prologue size: 0x10, Frame offset: 0x8, Frame reg: rbp
 	  pc+0x10: FPReg: rbp = rsp + 0x80 (info = 0x0)
 	  pc+0x08: alloc large area: rsp = rsp - 0x1e0
 	  pc+0x01: push rbp
- 00000000646cb2b4 (rva: 0000b2b4): 00000000646c4630 - 00000000646c46df
+ 00000000646cb2b4 (rva: 0000b2b4): 00000000646c46d0 - 00000000646c477f
 	Version: 1, Flags: none
 	Nbr codes: 3, Prologue size: 0x08, Frame offset: 0x0, Frame reg: rbp
 	  pc+0x08: alloc small area: rsp = rsp - 0x30
 	  pc+0x04: FPReg: rbp = rsp + 0x0 (info = 0x0)
 	  pc+0x01: push rbp
- 00000000646cb2c0 (rva: 0000b2c0): 00000000646c46e0 - 00000000646c4745
+ 00000000646cb2c0 (rva: 0000b2c0): 00000000646c4780 - 00000000646c47e5
 	Version: 1, Flags: none
 	Nbr codes: 3, Prologue size: 0x08, Frame offset: 0x0, Frame reg: rbp
 	  pc+0x08: alloc small area: rsp = rsp - 0x30
 	  pc+0x04: FPReg: rbp = rsp + 0x0 (info = 0x0)
 	  pc+0x01: push rbp
- 00000000646cb2cc (rva: 0000b2cc): 00000000646c4745 - 00000000646c4c08
+ 00000000646cb2cc (rva: 0000b2cc): 00000000646c47e5 - 00000000646c4c9b
 	Version: 1, Flags: none
 	Nbr codes: 4, Prologue size: 0x10, Frame offset: 0x8, Frame reg: rbp
 	  pc+0x10: FPReg: rbp = rsp + 0x80 (info = 0x0)
 	  pc+0x08: alloc large area: rsp = rsp - 0xa00
 	  pc+0x01: push rbp
- 00000000646cb2d8 (rva: 0000b2d8): 00000000646c4c08 - 00000000646c4c2b
+ 00000000646cb2d8 (rva: 0000b2d8): 00000000646c4c9b - 00000000646c4cbe
 	Version: 1, Flags: none
 	Nbr codes: 3, Prologue size: 0x08, Frame offset: 0x0, Frame reg: rbp
 	  pc+0x08: alloc small area: rsp = rsp - 0x20
 	  pc+0x04: FPReg: rbp = rsp + 0x0 (info = 0x0)
 	  pc+0x01: push rbp
- 00000000646cb2e4 (rva: 0000b2e4): 00000000646c4c2b - 00000000646c4c85
+ 00000000646cb2e4 (rva: 0000b2e4): 00000000646c4cbe - 00000000646c4d18
 	Version: 1, Flags: none
 	Nbr codes: 3, Prologue size: 0x08, Frame offset: 0x0, Frame reg: rbp
 	  pc+0x08: alloc small area: rsp = rsp - 0x20
 	  pc+0x04: FPReg: rbp = rsp + 0x0 (info = 0x0)
 	  pc+0x01: push rbp
- 00000000646cb2f0 (rva: 0000b2f0): 00000000646c4c90 - 00000000646c4e20
+ 00000000646cb2f0 (rva: 0000b2f0): 00000000646c4d20 - 00000000646c4eb0
 	Version: 1, Flags: none
 	Nbr codes: 3, Prologue size: 0x08, Frame offset: 0x0, Frame reg: rbp
 	  pc+0x08: alloc small area: rsp = rsp - 0x20
 	  pc+0x04: FPReg: rbp = rsp + 0x0 (info = 0x0)
 	  pc+0x01: push rbp
- 00000000646cb2fc (rva: 0000b2fc): 00000000646c4e20 - 00000000646c5021
+ 00000000646cb2fc (rva: 0000b2fc): 00000000646c4eb0 - 00000000646c50b1
 	Version: 1, Flags: none
 	Nbr codes: 3, Prologue size: 0x08, Frame offset: 0x0, Frame reg: rbp
 	  pc+0x08: alloc small area: rsp = rsp - 0x30
 	  pc+0x04: FPReg: rbp = rsp + 0x0 (info = 0x0)
 	  pc+0x01: push rbp
- 00000000646cb308 (rva: 0000b308): 00000000646c5021 - 00000000646c5088
+ 00000000646cb308 (rva: 0000b308): 00000000646c50b1 - 00000000646c5118
 	Version: 1, Flags: none
 	Nbr codes: 3, Prologue size: 0x08, Frame offset: 0x0, Frame reg: rbp
 	  pc+0x08: alloc small area: rsp = rsp - 0x30
 	  pc+0x04: FPReg: rbp = rsp + 0x0 (info = 0x0)
 	  pc+0x01: push rbp
- 00000000646cb314 (rva: 0000b314): 00000000646c5090 - 00000000646c530c
+ 00000000646cb314 (rva: 0000b314): 00000000646c5120 - 00000000646c539c
 	Version: 1, Flags: none
 	Nbr codes: 5, Prologue size: 0x11, Frame offset: 0x8, Frame reg: rbp
 	  pc+0x11: FPReg: rbp = rsp + 0x80 (info = 0x0)
 	  pc+0x09: alloc large area: rsp = rsp - 0x88
 	  pc+0x02: push rbx
 	  pc+0x01: push rbp
- 00000000646cb324 (rva: 0000b324): 00000000646c530c - 00000000646c53f4
+ 00000000646cb324 (rva: 0000b324): 00000000646c539c - 00000000646c5484
 	Version: 1, Flags: none
 	Nbr codes: 3, Prologue size: 0x08, Frame offset: 0x0, Frame reg: rbp
 	  pc+0x08: alloc small area: rsp = rsp - 0x40
 	  pc+0x04: FPReg: rbp = rsp + 0x0 (info = 0x0)
 	  pc+0x01: push rbp
- 00000000646cb330 (rva: 0000b330): 00000000646c5410 - 00000000646c5445
+ 00000000646cb330 (rva: 0000b330): 00000000646c54a0 - 00000000646c54d5
 	Version: 1, Flags: none
 	Nbr codes: 1, Prologue size: 0x04, Frame offset: 0x0, Frame reg: none
 	  pc+0x04: alloc small area: rsp = rsp - 0x28
- 00000000646cb338 (rva: 0000b338): 00000000646c5450 - 00000000646c54b6
+ 00000000646cb338 (rva: 0000b338): 00000000646c54e0 - 00000000646c5546
 	Version: 1, Flags: none
 	Nbr codes: 3, Prologue size: 0x06, Frame offset: 0x0, Frame reg: none
 	  pc+0x06: alloc small area: rsp = rsp - 0x28
 	  pc+0x02: push rbx
 	  pc+0x01: push rsi
- 00000000646cb344 (rva: 0000b344): 00000000646c54c0 - 00000000646c54df
+ 00000000646cb344 (rva: 0000b344): 00000000646c5550 - 00000000646c556f
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 00000000646cb348 (rva: 0000b348): 00000000646c54e0 - 00000000646c55b6
+ 00000000646cb348 (rva: 0000b348): 00000000646c5570 - 00000000646c5646
 	Version: 1, Flags: none
 	Nbr codes: 6, Prologue size: 0x0a, Frame offset: 0x0, Frame reg: none
 	  pc+0x0a: alloc small area: rsp = rsp - 0x30
 	  pc+0x06: push rbx
 	  pc+0x05: push rsi
 	  pc+0x04: push rdi
 	  pc+0x03: push rbp
 	  pc+0x02: push r12
- 00000000646cb358 (rva: 0000b358): 00000000646c55c0 - 00000000646c56b8
+ 00000000646cb358 (rva: 0000b358): 00000000646c5650 - 00000000646c5748
 	Version: 1, Flags: none
 	Nbr codes: 5, Prologue size: 0x0a, Frame offset: 0x0, Frame reg: rbp
 	  pc+0x0a: alloc small area: rsp = rsp - 0x70
 	  pc+0x06: FPReg: rbp = rsp + 0x0 (info = 0x0)
 	  pc+0x03: push rbx
 	  pc+0x02: push rsi
 	  pc+0x01: push rbp
- 00000000646cb368 (rva: 0000b368): 00000000646c56c0 - 00000000646c56ef
+ 00000000646cb368 (rva: 0000b368): 00000000646c5750 - 00000000646c577f
 	Version: 1, Flags: none
 	Nbr codes: 1, Prologue size: 0x04, Frame offset: 0x0, Frame reg: none
 	  pc+0x04: alloc small area: rsp = rsp - 0x28
- 00000000646cb370 (rva: 0000b370): 00000000646c56f0 - 00000000646c5763
+ 00000000646cb370 (rva: 0000b370): 00000000646c5780 - 00000000646c57f3
 	Version: 1, Flags: none
 	Nbr codes: 3, Prologue size: 0x06, Frame offset: 0x0, Frame reg: none
 	  pc+0x06: alloc small area: rsp = rsp - 0x28
 	  pc+0x02: push rbx
 	  pc+0x01: push rsi
- 00000000646cb37c (rva: 0000b37c): 00000000646c5770 - 00000000646c5773
+ 00000000646cb37c (rva: 0000b37c): 00000000646c5800 - 00000000646c5803
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 00000000646cb380 (rva: 0000b380): 00000000646c5780 - 00000000646c5784
+ 00000000646cb380 (rva: 0000b380): 00000000646c5810 - 00000000646c5814
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 00000000646cb384 (rva: 0000b384): 00000000646c5790 - 00000000646c5794
+ 00000000646cb384 (rva: 0000b384): 00000000646c5820 - 00000000646c5824
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 00000000646cb394 (rva: 0000b394): 00000000646c57a0 - 00000000646c596d
+ 00000000646cb394 (rva: 0000b394): 00000000646c5830 - 00000000646c59fd
 	Version: 1, Flags: none
 	Nbr codes: 6, Prologue size: 0x0a, Frame offset: 0x0, Frame reg: none
 	  pc+0x0a: alloc small area: rsp = rsp - 0x50
 	  pc+0x06: push rbx
 	  pc+0x05: push rsi
 	  pc+0x04: push rdi
 	  pc+0x03: push rbp
 	  pc+0x02: push r12
- 00000000646cb3a4 (rva: 0000b3a4): 00000000646c5970 - 00000000646c5c2b
+ 00000000646cb3a4 (rva: 0000b3a4): 00000000646c5a00 - 00000000646c5cbb
 	Version: 1, Flags: none
 	Nbr codes: 10, Prologue size: 0x18, Frame offset: 0x8, Frame reg: rbp
 	  pc+0x18: FPReg: rbp = rsp + 0x80 (info = 0x0)
 	  pc+0x10: alloc small area: rsp = rsp - 0x38
 	  pc+0x0c: push rbx
 	  pc+0x0b: push rsi
 	  pc+0x0a: push rdi
 	  pc+0x09: push r12
 	  pc+0x07: push r13
 	  pc+0x05: push r14
 	  pc+0x03: push r15
 	  pc+0x01: push rbp
- 00000000646cb3bc (rva: 0000b3bc): 00000000646c5c30 - 00000000646c5dd0
+ 00000000646cb3bc (rva: 0000b3bc): 00000000646c5cc0 - 00000000646c5e60
 	Version: 1, Flags: none
 	Nbr codes: 1, Prologue size: 0x04, Frame offset: 0x0, Frame reg: none
 	  pc+0x04: alloc small area: rsp = rsp - 0x28
- 00000000646cb3c4 (rva: 0000b3c4): 00000000646c5dd0 - 00000000646c5ebc
+ 00000000646cb3c4 (rva: 0000b3c4): 00000000646c5e60 - 00000000646c5f4c
 	Version: 1, Flags: none
 	Nbr codes: 6, Prologue size: 0x0a, Frame offset: 0x0, Frame reg: none
 	  pc+0x0a: alloc small area: rsp = rsp - 0x20
 	  pc+0x06: push rbx
 	  pc+0x05: push rsi
 	  pc+0x04: push rdi
 	  pc+0x03: push rbp
 	  pc+0x02: push r12
- 00000000646cb3d4 (rva: 0000b3d4): 00000000646c5ec0 - 00000000646c60a7
+ 00000000646cb3d4 (rva: 0000b3d4): 00000000646c5f50 - 00000000646c6137
 	Version: 1, Flags: none
 	Nbr codes: 2, Prologue size: 0x05, Frame offset: 0x0, Frame reg: none
 	  pc+0x05: alloc small area: rsp = rsp - 0x20
 	  pc+0x01: push rbx
- 00000000646cb3dc (rva: 0000b3dc): 00000000646c60b0 - 00000000646c611a
+ 00000000646cb3dc (rva: 0000b3dc): 00000000646c6140 - 00000000646c61aa
 	Version: 1, Flags: none
 	Nbr codes: 5, Prologue size: 0x08, Frame offset: 0x0, Frame reg: none
 	  pc+0x08: alloc small area: rsp = rsp - 0x28
 	  pc+0x04: push rbx
 	  pc+0x03: push rsi
 	  pc+0x02: push rdi
 	  pc+0x01: push rbp
- 00000000646cb3ec (rva: 0000b3ec): 00000000646c6120 - 00000000646c619f
+ 00000000646cb3ec (rva: 0000b3ec): 00000000646c61b0 - 00000000646c622f
 	Version: 1, Flags: none
 	Nbr codes: 5, Prologue size: 0x08, Frame offset: 0x0, Frame reg: none
 	  pc+0x08: alloc small area: rsp = rsp - 0x28
 	  pc+0x04: push rbx
 	  pc+0x03: push rsi
 	  pc+0x02: push rdi
 	  pc+0x01: push rbp
- 00000000646cb3fc (rva: 0000b3fc): 00000000646c61a0 - 00000000646c6240
+ 00000000646cb3fc (rva: 0000b3fc): 00000000646c6230 - 00000000646c62d0
 	Version: 1, Flags: none
 	Nbr codes: 2, Prologue size: 0x05, Frame offset: 0x0, Frame reg: none
 	  pc+0x05: alloc small area: rsp = rsp - 0x20
 	  pc+0x01: push rbx
- 00000000646cb404 (rva: 0000b404): 00000000646c6240 - 00000000646c631a
+ 00000000646cb404 (rva: 0000b404): 00000000646c62d0 - 00000000646c63aa
 	Version: 1, Flags: none
 	Nbr codes: 2, Prologue size: 0x05, Frame offset: 0x0, Frame reg: none
 	  pc+0x05: alloc small area: rsp = rsp - 0x20
 	  pc+0x01: push rbx
- 00000000646cb40c (rva: 0000b40c): 00000000646c6320 - 00000000646c633e
+ 00000000646cb40c (rva: 0000b40c): 00000000646c63b0 - 00000000646c63ce
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 00000000646cb410 (rva: 0000b410): 00000000646c6340 - 00000000646c6352
+ 00000000646cb410 (rva: 0000b410): 00000000646c63d0 - 00000000646c63e2
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 00000000646cb414 (rva: 0000b414): 00000000646c6360 - 00000000646c63a4
+ 00000000646cb414 (rva: 0000b414): 00000000646c63f0 - 00000000646c6434
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 00000000646cb418 (rva: 0000b418): 00000000646c63b0 - 00000000646c643d
+ 00000000646cb418 (rva: 0000b418): 00000000646c6440 - 00000000646c64cd
 	Version: 1, Flags: none
 	Nbr codes: 4, Prologue size: 0x07, Frame offset: 0x0, Frame reg: none
 	  pc+0x07: alloc small area: rsp = rsp - 0x20
 	  pc+0x03: push rbx
 	  pc+0x02: push rsi
 	  pc+0x01: push rdi
- 00000000646cb424 (rva: 0000b424): 00000000646c6440 - 00000000646c64b4
+ 00000000646cb424 (rva: 0000b424): 00000000646c64d0 - 00000000646c6544
 	Version: 1, Flags: none
 	Nbr codes: 1, Prologue size: 0x04, Frame offset: 0x0, Frame reg: none
 	  pc+0x04: alloc small area: rsp = rsp - 0x28
- 00000000646cb42c (rva: 0000b42c): 00000000646c64c0 - 00000000646c64fe
+ 00000000646cb42c (rva: 0000b42c): 00000000646c6550 - 00000000646c658e
 	Version: 1, Flags: none
 	Nbr codes: 1, Prologue size: 0x04, Frame offset: 0x0, Frame reg: none
 	  pc+0x04: alloc small area: rsp = rsp - 0x28
- 00000000646cb434 (rva: 0000b434): 00000000646c6500 - 00000000646c656f
+ 00000000646cb434 (rva: 0000b434): 00000000646c6590 - 00000000646c65ff
 	Version: 1, Flags: none
 	Nbr codes: 1, Prologue size: 0x04, Frame offset: 0x0, Frame reg: none
 	  pc+0x04: alloc small area: rsp = rsp - 0x28
- 00000000646cb43c (rva: 0000b43c): 00000000646c6570 - 00000000646c65a7
+ 00000000646cb43c (rva: 0000b43c): 00000000646c6600 - 00000000646c6637
 	Version: 1, Flags: none
 	Nbr codes: 1, Prologue size: 0x04, Frame offset: 0x0, Frame reg: none
 	  pc+0x04: alloc small area: rsp = rsp - 0x28
- 00000000646cb444 (rva: 0000b444): 00000000646c65b0 - 00000000646c6641
+ 00000000646cb444 (rva: 0000b444): 00000000646c6640 - 00000000646c66d1
 	Version: 1, Flags: none
 	Nbr codes: 1, Prologue size: 0x04, Frame offset: 0x0, Frame reg: none
 	  pc+0x04: alloc small area: rsp = rsp - 0x28
- 00000000646cb44c (rva: 0000b44c): 00000000646c6650 - 00000000646c66f6
+ 00000000646cb44c (rva: 0000b44c): 00000000646c66e0 - 00000000646c6786
 	Version: 1, Flags: none
 	Nbr codes: 1, Prologue size: 0x04, Frame offset: 0x0, Frame reg: none
 	  pc+0x04: alloc small area: rsp = rsp - 0x28
- 00000000646cb454 (rva: 0000b454): 00000000646c6700 - 00000000646c6703
+ 00000000646cb454 (rva: 0000b454): 00000000646c6790 - 00000000646c6793
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 00000000646cb458 (rva: 0000b458): 00000000646c6750 - 00000000646c6756
+ 00000000646cb458 (rva: 0000b458): 00000000646c67e0 - 00000000646c67e6
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 00000000646cb45c (rva: 0000b45c): 00000000646c6760 - 00000000646c6766
+ 00000000646cb45c (rva: 0000b45c): 00000000646c67f0 - 00000000646c67f6
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 00000000646cb460 (rva: 0000b460): 00000000646c6770 - 00000000646c67c4
+ 00000000646cb460 (rva: 0000b460): 00000000646c6800 - 00000000646c6854
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 00000000646cb464 (rva: 0000b464): 00000000646c67d0 - 00000000646c68f6
+ 00000000646cb464 (rva: 0000b464): 00000000646c6860 - 00000000646c6986
 	Version: 1, Flags: none
 	Nbr codes: 4, Prologue size: 0x0a, Frame offset: 0x0, Frame reg: none
 	  pc+0x0a: save xmm6 at rsp + 0x40
 	  pc+0x05: alloc small area: rsp = rsp - 0x50
 	  pc+0x01: push rbx
- 00000000646cb470 (rva: 0000b470): 00000000646c6900 - 00000000646c6905
+ 00000000646cb470 (rva: 0000b470): 00000000646c6990 - 00000000646c6995
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 00000000646cb474 (rva: 0000b474): 00000000646c6910 - 00000000646c69e7
+ 00000000646cb474 (rva: 0000b474): 00000000646c69a0 - 00000000646c6a77
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 00000000646cb478 (rva: 0000b478): 00000000646c69f0 - 00000000646c6ae4
+ 00000000646cb478 (rva: 0000b478): 00000000646c6a80 - 00000000646c6b74
 	Version: 1, Flags: none
 	Nbr codes: 4, Prologue size: 0x0a, Frame offset: 0x0, Frame reg: none
 	  pc+0x0a: save xmm6 at rsp + 0x60
 	  pc+0x05: alloc small area: rsp = rsp - 0x70
 	  pc+0x01: push rbx
- 00000000646cb484 (rva: 0000b484): 00000000646c6b20 - 00000000646c6d04
+ 00000000646cb484 (rva: 0000b484): 00000000646c6bb0 - 00000000646c6d94
 	Version: 1, Flags: none
 	Nbr codes: 4, Prologue size: 0x0a, Frame offset: 0x0, Frame reg: none
 	  pc+0x0a: save xmm6 at rsp + 0x40
 	  pc+0x05: alloc small area: rsp = rsp - 0x50
 	  pc+0x01: push rbx
- 00000000646cb490 (rva: 0000b490): 00000000646c6d10 - 00000000646c6e30
+ 00000000646cb490 (rva: 0000b490): 00000000646c6da0 - 00000000646c6ec0
 	Version: 1, Flags: none
 	Nbr codes: 4, Prologue size: 0x0a, Frame offset: 0x0, Frame reg: none
 	  pc+0x0a: save xmm6 at rsp + 0x60
 	  pc+0x05: alloc small area: rsp = rsp - 0x70
 	  pc+0x01: push rbx
- 00000000646cb49c (rva: 0000b49c): 00000000646c6e30 - 00000000646c6ec6
+ 00000000646cb49c (rva: 0000b49c): 00000000646c6ec0 - 00000000646c6f56
 	Version: 1, Flags: none
 	Nbr codes: 1, Prologue size: 0x04, Frame offset: 0x0, Frame reg: none
 	  pc+0x04: alloc small area: rsp = rsp - 0x18
- 00000000646cb4a4 (rva: 0000b4a4): 00000000646c6ed0 - 00000000646c7427
+ 00000000646cb4a4 (rva: 0000b4a4): 00000000646c6f60 - 00000000646c74b7
 	Version: 1, Flags: none
 	Nbr codes: 11, Prologue size: 0x1a, Frame offset: 0x0, Frame reg: none
 	  pc+0x1a: save xmm7 at rsp + 0x80
 	  pc+0x12: save xmm6 at rsp + 0x70
 	  pc+0x0d: alloc large area: rsp = rsp - 0x90
 	  pc+0x06: push rbx
 	  pc+0x05: push rsi
 	  pc+0x04: push rdi
 	  pc+0x03: push rbp
 	  pc+0x02: push r12
- 00000000646cb4c0 (rva: 0000b4c0): 00000000646c7430 - 00000000646c76ae
+ 00000000646cb4c0 (rva: 0000b4c0): 00000000646c74c0 - 00000000646c773e
 	Version: 1, Flags: none
 	Nbr codes: 3, Prologue size: 0x09, Frame offset: 0x0, Frame reg: none
 	  pc+0x09: save xmm6 at rsp + 0x40
 	  pc+0x04: alloc small area: rsp = rsp - 0x58
- 00000000646cb4cc (rva: 0000b4cc): 00000000646c7780 - 00000000646c783e
+ 00000000646cb4cc (rva: 0000b4cc): 00000000646c7810 - 00000000646c78ce
 	Version: 1, Flags: none
 	Nbr codes: 2, Prologue size: 0x05, Frame offset: 0x0, Frame reg: none
 	  pc+0x05: alloc small area: rsp = rsp - 0x30
 	  pc+0x01: push rbx
- 00000000646cb4d4 (rva: 0000b4d4): 00000000646c7960 - 00000000646c7985
+ 00000000646cb4d4 (rva: 0000b4d4): 00000000646c79f0 - 00000000646c7a15
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 00000000646cb4d8 (rva: 0000b4d8): 00000000646c7990 - 00000000646c7a58
+ 00000000646cb4d8 (rva: 0000b4d8): 00000000646c7a20 - 00000000646c7ae8
 	Version: 1, Flags: none
 	Nbr codes: 5, Prologue size: 0x08, Frame offset: 0x0, Frame reg: none
 	  pc+0x08: alloc small area: rsp = rsp - 0x28
 	  pc+0x04: push rbx
 	  pc+0x03: push rsi
 	  pc+0x02: push rdi
 	  pc+0x01: push rbp
- 00000000646cb4e8 (rva: 0000b4e8): 00000000646c7a60 - 00000000646c7acf
+ 00000000646cb4e8 (rva: 0000b4e8): 00000000646c7af0 - 00000000646c7b5f
 	Version: 1, Flags: none
 	Nbr codes: 4, Prologue size: 0x07, Frame offset: 0x0, Frame reg: none
 	  pc+0x07: alloc small area: rsp = rsp - 0x20
 	  pc+0x03: push rbx
 	  pc+0x02: push rsi
 	  pc+0x01: push rdi
- 00000000646cb4f4 (rva: 0000b4f4): 00000000646c7ad0 - 00000000646c7aef
+ 00000000646cb4f4 (rva: 0000b4f4): 00000000646c7b60 - 00000000646c7b7f
 	Version: 1, Flags: none
 	Nbr codes: 2, Prologue size: 0x05, Frame offset: 0x0, Frame reg: none
 	  pc+0x05: alloc small area: rsp = rsp - 0x20
 	  pc+0x01: push rbx
- 00000000646cb4fc (rva: 0000b4fc): 00000000646c7bc0 - 00000000646c7c01
+ 00000000646cb4fc (rva: 0000b4fc): 00000000646c7c50 - 00000000646c7c91
 	Version: 1, Flags: none
 	Nbr codes: 1, Prologue size: 0x04, Frame offset: 0x0, Frame reg: none
 	  pc+0x04: alloc small area: rsp = rsp - 0x58
- 00000000646cb504 (rva: 0000b504): 00000000646c7c10 - 00000000646c7c1c
+ 00000000646cb504 (rva: 0000b504): 00000000646c7ca0 - 00000000646c7cac
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 00000000646cb508 (rva: 0000b508): 00000000646c7c20 - 00000000646c7d1c
+ 00000000646cb508 (rva: 0000b508): 00000000646c7cb0 - 00000000646c7dac
 	Version: 1, Flags: none
 	Nbr codes: 9, Prologue size: 0x16, Frame offset: 0x0, Frame reg: none
 	  pc+0x16: save xmm8 at rsp + 0x60
 	  pc+0x10: save xmm7 at rsp + 0x50
 	  pc+0x0b: save xmm6 at rsp + 0x40
 	  pc+0x06: alloc small area: rsp = rsp - 0x78
 	  pc+0x02: push rbx
 	  pc+0x01: push rsi
- 00000000646cb388 (rva: 0000b388): 00000000646c7d30 - 00000000646c7d99
+ 00000000646cb388 (rva: 0000b388): 00000000646c7dc0 - 00000000646c7e29
 	Version: 1, Flags: none
 	Nbr codes: 3, Prologue size: 0x06, Frame offset: 0x0, Frame reg: none
 	  pc+0x06: alloc small area: rsp = rsp - 0x38
 	  pc+0x02: push rbx
 	  pc+0x01: push rsi
- 00000000646cb520 (rva: 0000b520): 00000000646c7da0 - 00000000646c7da5
+ 00000000646cb520 (rva: 0000b520): 00000000646c7e30 - 00000000646c7e35
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
 
 
 PE File Base Relocations (interpreted .reloc section contents)
 
 Virtual Address: 00007000 Chunk size 12 (0xc) Number of fixups 2
-	reloc    0 offset  db8 [7db8] DIR64
+	reloc    0 offset  e48 [7e48] DIR64
 	reloc    1 offset    0 [7000] ABSOLUTE
 
 Virtual Address: 00008000 Chunk size 20 (0x14) Number of fixups 6
 	reloc    0 offset    0 [8000] DIR64
 	reloc    1 offset   50 [8050] DIR64
 	reloc    2 offset   58 [8058] DIR64
 	reloc    3 offset   60 [8060] DIR64
@@ -1121,47 +1120,47 @@
 	reloc    0 offset   18 [f018] DIR64
 	reloc    1 offset   30 [f030] DIR64
 	reloc    2 offset   38 [f038] DIR64
 	reloc    3 offset    0 [f000] ABSOLUTE
 
 Sections:
 Idx Name          Size      VMA               LMA               File off  Algn
-  0 .text         00006dd8  00000000646c1000  00000000646c1000  00000600  2**4
+  0 .text         00006e68  00000000646c1000  00000000646c1000  00000600  2**4
                   CONTENTS, ALLOC, LOAD, READONLY, CODE, DATA
-  1 .data         000000a0  00000000646c8000  00000000646c8000  00007400  2**4
+  1 .data         000000a0  00000000646c8000  00000000646c8000  00007600  2**4
                   CONTENTS, ALLOC, LOAD, DATA
-  2 .rdata        00000900  00000000646c9000  00000000646c9000  00007600  2**5
+  2 .rdata        00000900  00000000646c9000  00000000646c9000  00007800  2**5
                   CONTENTS, ALLOC, LOAD, READONLY, DATA
-  3 .pdata        000005b8  00000000646ca000  00000000646ca000  00008000  2**2
+  3 .pdata        000005b8  00000000646ca000  00000000646ca000  00008200  2**2
                   CONTENTS, ALLOC, LOAD, READONLY, DATA
-  4 .xdata        00000524  00000000646cb000  00000000646cb000  00008600  2**2
+  4 .xdata        00000524  00000000646cb000  00000000646cb000  00008800  2**2
                   CONTENTS, ALLOC, LOAD, READONLY, DATA
   5 .bss          00000b90  00000000646cc000  00000000646cc000  00000000  2**5
                   ALLOC
-  6 .edata        00000670  00000000646cd000  00000000646cd000  00008c00  2**2
+  6 .edata        00000670  00000000646cd000  00000000646cd000  00008e00  2**2
                   CONTENTS, ALLOC, LOAD, READONLY, DATA
-  7 .idata        00000720  00000000646ce000  00000000646ce000  00009400  2**2
+  7 .idata        00000720  00000000646ce000  00000000646ce000  00009600  2**2
                   CONTENTS, ALLOC, LOAD, DATA
-  8 .CRT          00000058  00000000646cf000  00000000646cf000  00009c00  2**3
+  8 .CRT          00000058  00000000646cf000  00000000646cf000  00009e00  2**3
                   CONTENTS, ALLOC, LOAD, DATA
-  9 .tls          00000010  00000000646d0000  00000000646d0000  00009e00  2**3
+  9 .tls          00000010  00000000646d0000  00000000646d0000  0000a000  2**3
                   CONTENTS, ALLOC, LOAD, DATA
- 10 .reloc        00000064  00000000646d1000  00000000646d1000  0000a000  2**2
+ 10 .reloc        00000064  00000000646d1000  00000000646d1000  0000a200  2**2
                   CONTENTS, ALLOC, LOAD, READONLY, DATA
- 11 .debug_aranges 00000050  00000000646d2000  00000000646d2000  0000a200  2**4
+ 11 .debug_aranges 00000050  00000000646d2000  00000000646d2000  0000a400  2**4
                   CONTENTS, READONLY, DEBUGGING
- 12 .debug_info   00001f08  00000000646d3000  00000000646d3000  0000a400  2**0
+ 12 .debug_info   00001f08  00000000646d3000  00000000646d3000  0000a600  2**0
                   CONTENTS, READONLY, DEBUGGING
- 13 .debug_abbrev 00000149  00000000646d5000  00000000646d5000  0000c400  2**0
+ 13 .debug_abbrev 00000149  00000000646d5000  00000000646d5000  0000c600  2**0
                   CONTENTS, READONLY, DEBUGGING
- 14 .debug_line   00000222  00000000646d6000  00000000646d6000  0000c600  2**0
+ 14 .debug_line   00000222  00000000646d6000  00000000646d6000  0000c800  2**0
                   CONTENTS, READONLY, DEBUGGING
- 15 .debug_frame  00000048  00000000646d7000  00000000646d7000  0000ca00  2**3
+ 15 .debug_frame  00000048  00000000646d7000  00000000646d7000  0000cc00  2**3
                   CONTENTS, READONLY, DEBUGGING
- 16 .debug_str    0000009b  00000000646d8000  00000000646d8000  0000cc00  2**0
+ 16 .debug_str    0000009b  00000000646d8000  00000000646d8000  0000ce00  2**0
                   CONTENTS, READONLY, DEBUGGING
 SYMBOL TABLE:
 [  0](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000028 crtdll.c
 File 
 [  2](sec  1)(fl 0x00)(ty   20)(scl   3) (nx 1) 0x0000000000000000 pre_c_init
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
 [  4](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000000 atexit_table
@@ -1285,79 +1284,79 @@
 AUX scnlen 0x20 nreloc 0 nlnno 0
 [123](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000700 .rdata$zzz
 AUX scnlen 0x3f nreloc 0 nlnno 0
 [125](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000091 cov_model.c
 File 
 [127](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000001ec0 cov_model_init
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[129](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001f06 cov_model
-[130](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001fcf cov_model2d
+[129](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001f24 cov_model
+[130](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x000000000000202e cov_model2d
 [131](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000001ec0 .text
-AUX scnlen 0x21b nreloc 6 nlnno 0
+AUX scnlen 0x2bb nreloc 6 nlnno 0
 [133](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000000 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [135](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000020 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [137](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000001e8 .xdata
 AUX scnlen 0x20 nreloc 0 nlnno 0
 [139](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000204 .pdata
 AUX scnlen 0x24 nreloc 9 nlnno 0
 [141](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000050 .rdata
 AUX scnlen 0x10 nreloc 0 nlnno 0
 [143](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000740 .rdata$zzz
 AUX scnlen 0x3f nreloc 0 nlnno 0
 [145](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000000b6 krige.c
 File 
-[147](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000020 range
-[148](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000028 sill
+[147](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000020 model
+[148](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000028 k_range
 [149](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000030 estimation
 [150](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000038 krige_var
 [151](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000040 fix
 [152](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 location
 [153](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000070 loc_cov
 [154](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000090 data_temp
 [155](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000b0 loc_cov2
 [156](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000d0 flatten_temp
 [157](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000f0 weights
 [158](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000110 array2d_temp
 [159](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000130 pdist_temp
 [160](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000150 datacov
-[161](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x00000000000020e0 sampling_state_init
+[161](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000002180 sampling_state_init
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[163](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000002191 sampling_state_update
-[164](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000021bd krige_param_setting
-[165](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000002413 simple_kriging
-[166](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x000000000000283d find_neighbor
-[167](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000029da krige_memory_free
-[168](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000020e0 .text
-AUX scnlen 0xa44 nreloc 130 nlnno 0
+[163](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000002231 sampling_state_update
+[164](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x000000000000225d krige_param_setting
+[165](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000024b9 simple_kriging
+[166](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000028c7 find_neighbor
+[167](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000002a7b krige_memory_free
+[168](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000002180 .text
+AUX scnlen 0xa45 nreloc 130 nlnno 0
 [170](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000000 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [172](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000020 .bss
 AUX scnlen 0x148 nreloc 0 nlnno 0
 [174](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000208 .xdata
 AUX scnlen 0x48 nreloc 0 nlnno 0
 [176](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000228 .pdata
 AUX scnlen 0x48 nreloc 18 nlnno 0
 [178](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000060 .rdata
 AUX scnlen 0x28 nreloc 0 nlnno 0
 [180](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000780 .rdata$zzz
 AUX scnlen 0x3f nreloc 0 nlnno 0
 [182](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000000cf matrix_tools.c
 File 
-[184](sec  1)(fl 0x00)(ty   20)(scl   3) (nx 1) 0x0000000000002b30 snprintf
+[184](sec  1)(fl 0x00)(ty   20)(scl   3) (nx 1) 0x0000000000002bd0 snprintf
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[186](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000002b7a lu_inverse_solver
-[187](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000002ef8 lu_decomposition
-[188](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000003289 arange
-[189](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000032e1 d_arange
-[190](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x000000000000333d pdist
-[191](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000033f0 matrixform
-[192](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x000000000000347d save_1darray
-[193](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000002b30 .text
+[186](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000002c1a lu_inverse_solver
+[187](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000002f98 lu_decomposition
+[188](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000003329 arange
+[189](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000003381 d_arange
+[190](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000033dd pdist
+[191](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000003490 matrixform
+[192](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x000000000000351d save_1darray
+[193](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000002bd0 .text
 AUX scnlen 0xafb nreloc 28 nlnno 0
 [195](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000000 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [197](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000170 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [199](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000250 .xdata
 AUX scnlen 0x64 nreloc 0 nlnno 0
@@ -1365,17 +1364,17 @@
 AUX scnlen 0x60 nreloc 24 nlnno 0
 [203](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000090 .rdata
 AUX scnlen 0x70 nreloc 0 nlnno 0
 [205](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000007c0 .rdata$zzz
 AUX scnlen 0x3f nreloc 0 nlnno 0
 [207](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000000df random_tools.c
 File 
-[209](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000003630 randompath
+[209](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x00000000000036d0 randompath
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[211](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000003630 .text
+[211](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000036d0 .text
 AUX scnlen 0xaf nreloc 1 nlnno 0
 [213](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000000 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [215](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000170 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [217](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000002b4 .xdata
 AUX scnlen 0xc nreloc 0 nlnno 0
@@ -1389,168 +1388,168 @@
 [226](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001a0 u_array
 [227](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001c0 sampled
 [228](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001e0 variogram_array
 [229](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000200 sgsim_array
 [230](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000220 _sampling
 [231](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000268 flag
 [232](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000026c count
-[233](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x00000000000036e0 sgsim_init
+[233](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000003780 sgsim_init
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[235](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000003745 sgsim_run
-[236](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000003c08 sgsim_t_free
-[237](sec  1)(fl 0x00)(ty   20)(scl   3) (nx 0) 0x0000000000003c2b sgsim_memory_free
-[238](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000036e0 .text
-AUX scnlen 0x5a5 nreloc 82 nlnno 0
+[235](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000037e5 sgsim_run
+[236](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000003c9b sgsim_t_free
+[237](sec  1)(fl 0x00)(ty   20)(scl   3) (nx 0) 0x0000000000003cbe sgsim_memory_free
+[238](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000003780 .text
+AUX scnlen 0x598 nreloc 82 nlnno 0
 [240](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000000 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [242](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000180 .bss
 AUX scnlen 0xf0 nreloc 0 nlnno 0
 [244](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000002c0 .xdata
 AUX scnlen 0x30 nreloc 0 nlnno 0
 [246](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000002dc .pdata
 AUX scnlen 0x30 nreloc 12 nlnno 0
 [248](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000100 .rdata
 AUX scnlen 0x58 nreloc 0 nlnno 0
 [250](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000840 .rdata$zzz
 AUX scnlen 0x3f nreloc 0 nlnno 0
 [252](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x000000000000010e sort_tools.c
 File 
-[254](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000003c90 swap
+[254](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000003d20 swap
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[256](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000003e20 Partition2d
-[257](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000004021 quicksort2d
-[258](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000003c90 .text
+[256](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000003eb0 Partition2d
+[257](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000040b1 quicksort2d
+[258](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000003d20 .text
 AUX scnlen 0x3f8 nreloc 0 nlnno 0
 [260](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000000 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [262](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000280 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [264](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000002f0 .xdata
 AUX scnlen 0x24 nreloc 0 nlnno 0
 [266](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000030c .pdata
 AUX scnlen 0x24 nreloc 9 nlnno 0
 [268](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000880 .rdata$zzz
 AUX scnlen 0x3f nreloc 0 nlnno 0
 [270](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000128 variogram.c
 File 
-[272](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000004090 variogram
+[272](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000004120 variogram
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[274](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x000000000000430c variance
-[275](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000004090 .text
+[274](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x000000000000439c variance
+[275](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000004120 .text
 AUX scnlen 0x364 nreloc 13 nlnno 0
 [277](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000000 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [279](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000280 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [281](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000314 .xdata
 AUX scnlen 0x1c nreloc 0 nlnno 0
 [283](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000330 .pdata
 AUX scnlen 0x18 nreloc 6 nlnno 0
 [285](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000160 .rdata
 AUX scnlen 0x18 nreloc 0 nlnno 0
 [287](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000008c0 .rdata$zzz
 AUX scnlen 0x3f nreloc 0 nlnno 0
-[289](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000004400 .text
+[289](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000004490 .text
 [290](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000000 .data
 [291](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000280 .bss
 [292](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000684 .idata$7
 [293](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000024c .idata$5
 [294](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000bc .idata$4
 [295](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000004ca .idata$6
 [296](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000136 fake
 File 
 [298](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000003c hname
 [299](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001cc fthunk
-[300](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000004410 .text
+[300](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000044a0 .text
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [302](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000000 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [304](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000280 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [306](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000000 .idata$2
 AUX scnlen 0x14 nreloc 3 nlnno 0
 [308](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000003c .idata$4
 [309](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001cc .idata$5
 [310](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000144 fake
 File 
-[312](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000004410 .text
+[312](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000044a0 .text
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [314](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000000 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [316](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000280 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [318](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000000ec .idata$4
 AUX scnlen 0x8 nreloc 0 nlnno 0
 [320](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000027c .idata$5
 AUX scnlen 0x8 nreloc 0 nlnno 0
 [322](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000069c .idata$7
 AUX scnlen 0xd nreloc 0 nlnno 0
 [324](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000158 gccmain.c
 File 
-[326](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000004410 __do_global_dtors
+[326](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x00000000000044a0 __do_global_dtors
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
 [328](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000000 p.93846
-[329](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000004450 __do_global_ctors
+[329](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000044e0 __do_global_ctors
 [330](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000005f0 .rdata$.refptr.__CTOR_LIST__
 AUX scnlen 0x8 nreloc 1 nlnno 0 checksum 0x0 assoc 0 comdat 2
-[332](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000044c0 __main
+[332](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000004550 __main
 [333](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000280 initialized
-[334](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000004410 .text
+[334](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000044a0 .text
 AUX scnlen 0xcf nreloc 7 nlnno 0
 [336](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000000 .data
 AUX scnlen 0x8 nreloc 1 nlnno 0
 [338](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000280 .bss
 AUX scnlen 0x4 nreloc 0 nlnno 0
 [340](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000330 .xdata
 AUX scnlen 0x18 nreloc 0 nlnno 0
 [342](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000348 .pdata
 AUX scnlen 0x24 nreloc 9 nlnno 0
 [344](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000160 natstart.c
 File 
-[346](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000044e0 .text
+[346](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000004570 .text
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [348](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000010 .data
 AUX scnlen 0x8 nreloc 0 nlnno 0
 [350](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000290 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [352](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000178 gs_support.c
 File 
-[354](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x00000000000044e0 __security_init_cookie
+[354](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000004570 __security_init_cookie
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
 [356](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000080 .data$__security_cookie
 AUX scnlen 0x8 nreloc 0 nlnno 0 checksum 0x0 assoc 0 comdat 3
 [358](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000090 .data$__security_cookie_complement
 AUX scnlen 0x8 nreloc 0 nlnno 0 checksum 0x0 assoc 0 comdat 3
-[360](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000045c0 __report_gsfailure
+[360](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000004650 __report_gsfailure
 [361](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002a0 GS_ContextRecord
 [362](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000780 GS_ExceptionRecord
 [363](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000180 GS_ExceptionPointers
-[364](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000044e0 .text
+[364](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000004570 .text
 AUX scnlen 0x1d8 nreloc 29 nlnno 0
 [366](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000020 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [368](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000002a0 .bss
 AUX scnlen 0x578 nreloc 0 nlnno 0
 [370](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000348 .xdata
 AUX scnlen 0x20 nreloc 0 nlnno 0
 [372](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000036c .pdata
 AUX scnlen 0x18 nreloc 6 nlnno 0
 [374](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000180 .rdata
 AUX scnlen 0x10 nreloc 2 nlnno 0
 [376](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x000000000000019e tlssup.c
 File 
-[378](sec  1)(fl 0x00)(ty   20)(scl   3) (nx 1) 0x00000000000046c0 __dyn_tls_dtor
+[378](sec  1)(fl 0x00)(ty   20)(scl   3) (nx 1) 0x0000000000004750 __dyn_tls_dtor
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[380](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000046f0 __dyn_tls_init
+[380](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000004780 __dyn_tls_init
 [381](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000005e0 .rdata$.refptr._CRT_MT
 AUX scnlen 0x8 nreloc 1 nlnno 0 checksum 0x0 assoc 0 comdat 2
 [383](sec  9)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000048 __xd_a
 [384](sec  9)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 __xd_z
-[385](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000004770 __tlregdtor
-[386](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000046c0 .text
+[385](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000004800 __tlregdtor
+[386](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000004750 .text
 AUX scnlen 0xb3 nreloc 5 nlnno 0
 [388](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000020 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [390](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000820 .bss
 AUX scnlen 0x10 nreloc 0 nlnno 0
 [392](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000368 .xdata
 AUX scnlen 0x18 nreloc 0 nlnno 0
@@ -1572,15 +1571,15 @@
 AUX scnlen 0x8 nreloc 0 nlnno 0
 [410](sec 10)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000008 .tls$ZZZ
 AUX scnlen 0x8 nreloc 0 nlnno 0
 [412](sec 10)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000000 .tls
 AUX scnlen 0x8 nreloc 0 nlnno 0
 [414](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000001ae cinitexe.c
 File 
-[416](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000004780 .text
+[416](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000004810 .text
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [418](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000020 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [420](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000830 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [422](sec  9)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000008 .CRT$XCZ
 AUX scnlen 0x8 nreloc 0 nlnno 0
@@ -1588,146 +1587,146 @@
 AUX scnlen 0x8 nreloc 0 nlnno 0
 [426](sec  9)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000020 .CRT$XIZ
 AUX scnlen 0x8 nreloc 0 nlnno 0
 [428](sec  9)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000010 .CRT$XIA
 AUX scnlen 0x8 nreloc 0 nlnno 0
 [430](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000001bd mingw_helpers.c
 File 
-[432](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000004780 _decode_pointer
+[432](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000004810 _decode_pointer
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[434](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000004790 _encode_pointer
-[435](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000004780 .text
+[434](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000004820 _encode_pointer
+[435](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000004810 .text
 AUX scnlen 0x14 nreloc 0 nlnno 0
 [437](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000020 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [439](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000830 .bss
 AUX scnlen 0x4 nreloc 0 nlnno 0
 [441](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000380 .xdata
 AUX scnlen 0x8 nreloc 0 nlnno 0
 [443](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000003a8 .pdata
 AUX scnlen 0x18 nreloc 6 nlnno 0
 [445](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000001de pseudo-reloc.c
 File 
-[447](sec  1)(fl 0x00)(ty   20)(scl   3) (nx 1) 0x0000000000006d30 __report_error
+[447](sec  1)(fl 0x00)(ty   20)(scl   3) (nx 1) 0x0000000000006dc0 __report_error
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[449](sec  1)(fl 0x00)(ty   20)(scl   3) (nx 0) 0x00000000000047a0 __write_memory.part.0
+[449](sec  1)(fl 0x00)(ty   20)(scl   3) (nx 0) 0x0000000000004830 __write_memory.part.0
 [450](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000844 maxSections
 [451](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000848 the_secs
-[452](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000004970 _pei386_runtime_relocator
+[452](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000004a00 _pei386_runtime_relocator
 [453](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000840 was_init.95174
 [454](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000600 .rdata$.refptr.__RUNTIME_PSEUDO_RELOC_LIST_END__
 AUX scnlen 0x8 nreloc 1 nlnno 0 checksum 0x0 assoc 0 comdat 2
 [456](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000610 .rdata$.refptr.__RUNTIME_PSEUDO_RELOC_LIST__
 AUX scnlen 0x8 nreloc 1 nlnno 0 checksum 0x0 assoc 0 comdat 2
 [458](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000630 .rdata$.refptr.__image_base__
 AUX scnlen 0x8 nreloc 1 nlnno 0 checksum 0x0 assoc 0 comdat 2
-[460](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000047a0 .text
+[460](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000004830 .text
 AUX scnlen 0x48b nreloc 36 nlnno 0
 [462](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000020 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [464](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000840 .bss
 AUX scnlen 0x10 nreloc 0 nlnno 0
 [466](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000200 .rdata
 AUX scnlen 0x102 nreloc 0 nlnno 0
-[468](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000006d30 .text.unlikely
+[468](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000006dc0 .text.unlikely
 AUX scnlen 0x69 nreloc 6 nlnno 0
 [470](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000388 .xdata.unlikely
 AUX scnlen 0xc nreloc 0 nlnno 0
 [472](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000003c0 .pdata.unlikely
 AUX scnlen 0xc nreloc 3 nlnno 0
 [474](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000394 .xdata
 AUX scnlen 0x28 nreloc 0 nlnno 0
 [476](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000003cc .pdata
 AUX scnlen 0x18 nreloc 6 nlnno 0
 [478](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000001f3 crt_handler.c
 File 
-[480](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000004c30 __mingw_SEH_error_handler
+[480](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000004cc0 __mingw_SEH_error_handler
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[482](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000004dd0 __mingw_init_ehandler
+[482](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000004e60 __mingw_init_ehandler
 [483](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000868 was_here.95013
 [484](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000980 emu_pdata
 [485](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000880 emu_xdata
-[486](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000004ec0 _gnu_exception_handler
-[487](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000004c30 .text
+[486](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000004f50 _gnu_exception_handler
+[487](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000004cc0 .text
 AUX scnlen 0x477 nreloc 29 nlnno 0
 [489](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000020 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [491](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000860 .bss
 AUX scnlen 0x2a0 nreloc 0 nlnno 0
 [493](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000003bc .xdata
 AUX scnlen 0x20 nreloc 0 nlnno 0
 [495](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000003e4 .pdata
 AUX scnlen 0x24 nreloc 9 nlnno 0
 [497](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000310 .rdata
 AUX scnlen 0x7 nreloc 0 nlnno 0
 [499](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000207 tlsthrd.c
 File 
-[501](sec  1)(fl 0x00)(ty   20)(scl   3) (nx 1) 0x00000000000050b0 __mingwthr_run_key_dtors.part.0
+[501](sec  1)(fl 0x00)(ty   20)(scl   3) (nx 1) 0x0000000000005140 __mingwthr_run_key_dtors.part.0
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
 [503](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b20 __mingwthr_cs
 [504](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b00 key_dtor_list
-[505](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000005120 ___w64_mingwthr_add_key_dtor
+[505](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000051b0 ___w64_mingwthr_add_key_dtor
 [506](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b08 __mingwthr_cs_init
-[507](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000051a0 ___w64_mingwthr_remove_key_dtor
-[508](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000005240 __mingw_TLScallback
-[509](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000050b0 .text
+[507](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000005230 ___w64_mingwthr_remove_key_dtor
+[508](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000052d0 __mingw_TLScallback
+[509](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000005140 .text
 AUX scnlen 0x26a nreloc 39 nlnno 0
 [511](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000020 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [513](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b00 .bss
 AUX scnlen 0x48 nreloc 0 nlnno 0
 [515](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000003dc .xdata
 AUX scnlen 0x30 nreloc 0 nlnno 0
 [517](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000408 .pdata
 AUX scnlen 0x30 nreloc 12 nlnno 0
 [519](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x000000000000020f tlsmcrt.c
 File 
-[521](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000005320 .text
+[521](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000053b0 .text
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [523](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000020 .data
 AUX scnlen 0x4 nreloc 0 nlnno 0
 [525](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b60 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [527](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000217 pseudo-reloc-list.c
 File 
-[529](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000005320 .text
+[529](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000053b0 .text
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [531](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000030 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [533](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b60 .bss
 AUX scnlen 0x2 nreloc 0 nlnno 0
 [535](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x000000000000022e pesect.c
 File 
-[537](sec  1)(fl 0x00)(ty   20)(scl   3) (nx 1) 0x0000000000005320 _ValidateImageBase.part.0
+[537](sec  1)(fl 0x00)(ty   20)(scl   3) (nx 1) 0x00000000000053b0 _ValidateImageBase.part.0
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[539](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000005340 _ValidateImageBase
-[540](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000005360 _FindPESection
-[541](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000053b0 _FindPESectionByName
-[542](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000005440 __mingw_GetSectionForAddress
-[543](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000054c0 __mingw_GetSectionCount
-[544](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000005500 _FindPESectionExec
-[545](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000005570 _GetPEImageBase
-[546](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000055b0 _IsNonwritableInCurrentImage
-[547](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000005650 __mingw_enum_import_library_names
-[548](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000005320 .text
+[539](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000053d0 _ValidateImageBase
+[540](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000053f0 _FindPESection
+[541](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000005440 _FindPESectionByName
+[542](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000054d0 __mingw_GetSectionForAddress
+[543](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000005550 __mingw_GetSectionCount
+[544](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000005590 _FindPESectionExec
+[545](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000005600 _GetPEImageBase
+[546](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000005640 _IsNonwritableInCurrentImage
+[547](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000056e0 __mingw_enum_import_library_names
+[548](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000053b0 .text
 AUX scnlen 0x3d6 nreloc 9 nlnno 0
 [550](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000030 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [552](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b70 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [554](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000040c .xdata
 AUX scnlen 0x48 nreloc 0 nlnno 0
 [556](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000438 .pdata
 AUX scnlen 0x78 nreloc 30 nlnno 0
 [558](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x000000000000023d CRT_fp10.c
 File 
-[560](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000005700 _fpreset
+[560](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000005790 _fpreset
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[562](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000005700 fpreset
-[563](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000005700 .text
+[562](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000005790 fpreset
+[563](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000005790 .text
 AUX scnlen 0x3 nreloc 0 nlnno 0
 [565](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000030 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [567](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b70 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [569](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000454 .xdata
 AUX scnlen 0x4 nreloc 0 nlnno 0
@@ -1737,29 +1736,29 @@
 File 
 [575](sec 13)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000000 .debug_info
 AUX scnlen 0x2e nreloc 7 nlnno 0
 [577](sec 14)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000000 .debug_abbrev
 AUX scnlen 0x14 nreloc 0 nlnno 0
 [579](sec 15)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000000 .debug_line
 AUX scnlen 0x7b nreloc 1 nlnno 0
-[581](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000005710 .text
+[581](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000057a0 .text
 AUX scnlen 0x32 nreloc 0 nlnno 0
 [583](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000030 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [585](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b70 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [587](sec 12)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000000 .debug_aranges
 AUX scnlen 0x30 nreloc 2 nlnno 0
 [589](sec 17)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000000 .debug_str
 AUX scnlen 0x9b nreloc 0 nlnno 0
 [591](sec 16)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000000 .debug_frame
 AUX scnlen 0x48 nreloc 2 nlnno 0
 [593](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000261 libgcc2.c
 File 
-[595](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000005750 .text
+[595](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000057e0 .text
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [597](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000030 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [599](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b70 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [601](sec 13)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000002e .debug_info
 AUX scnlen 0x1eda nreloc 4 nlnno 0
@@ -1767,874 +1766,874 @@
 AUX scnlen 0x135 nreloc 0 nlnno 0
 [605](sec 12)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000030 .debug_aranges
 AUX scnlen 0x20 nreloc 1 nlnno 0
 [607](sec 15)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000007b .debug_line
 AUX scnlen 0x1a7 nreloc 0 nlnno 0
 [609](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x000000000000026f dllentry.c
 File 
-[611](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000005750 DllEntryPoint
+[611](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x00000000000057e0 DllEntryPoint
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[613](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000005750 .text
+[613](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000057e0 .text
 AUX scnlen 0x6 nreloc 0 nlnno 0
 [615](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000030 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [617](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b70 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [619](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000458 .xdata
 AUX scnlen 0x4 nreloc 0 nlnno 0
 [621](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000004bc .pdata
 AUX scnlen 0xc nreloc 3 nlnno 0
 [623](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x000000000000027d dllmain.c
 File 
-[625](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000005760 DllMain
+[625](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x00000000000057f0 DllMain
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[627](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000005760 .text
+[627](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000057f0 .text
 AUX scnlen 0x6 nreloc 0 nlnno 0
 [629](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000030 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [631](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b70 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [633](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000045c .xdata
 AUX scnlen 0x4 nreloc 0 nlnno 0
 [635](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000004c8 .pdata
 AUX scnlen 0xc nreloc 3 nlnno 0
 [637](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x000000000000028b fpclassify.c
 File 
-[639](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000005770 __fpclassify
+[639](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000005800 __fpclassify
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[641](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000005770 .text
+[641](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000005800 .text
 AUX scnlen 0x54 nreloc 0 nlnno 0
 [643](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000030 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [645](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b70 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [647](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000460 .xdata
 AUX scnlen 0x4 nreloc 0 nlnno 0
 [649](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000004d4 .pdata
 AUX scnlen 0xc nreloc 3 nlnno 0
 [651](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x000000000000029b sqrt.c
 File 
-[653](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x00000000000057d0 sqrt
+[653](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000005860 sqrt
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[655](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000057d0 .text
+[655](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000005860 .text
 AUX scnlen 0x126 nreloc 10 nlnno 0
 [657](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000030 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [659](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b70 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [661](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000320 .rdata
 AUX scnlen 0x28 nreloc 0 nlnno 0
 [663](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000464 .xdata
 AUX scnlen 0xc nreloc 0 nlnno 0
 [665](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000004e0 .pdata
 AUX scnlen 0xc nreloc 3 nlnno 0
 [667](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000002a9 vsnprintf.c
 File 
-[669](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000005900 __ms_vsnprintf
+[669](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000005990 __ms_vsnprintf
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[671](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000005900 .text
+[671](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000005990 .text
 AUX scnlen 0x5 nreloc 1 nlnno 0
 [673](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000030 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [675](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b70 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [677](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000470 .xdata
 AUX scnlen 0x4 nreloc 0 nlnno 0
 [679](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000004ec .pdata
 AUX scnlen 0xc nreloc 3 nlnno 0
 [681](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000002c2 ceil.S
 File 
-[683](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000005910 ceil
+[683](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x00000000000059a0 ceil
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[685](sec  1)(fl 0x00)(ty    0)(scl   6) (nx 0) 0x00000000000059d0 .is_intnaninf
-[686](sec  1)(fl 0x00)(ty    0)(scl   6) (nx 0) 0x00000000000059e0 .ret_org
-[687](sec  1)(fl 0x00)(ty    0)(scl   6) (nx 0) 0x0000000000005990 .signed_val
+[685](sec  1)(fl 0x00)(ty    0)(scl   6) (nx 0) 0x0000000000005a60 .is_intnaninf
+[686](sec  1)(fl 0x00)(ty    0)(scl   6) (nx 0) 0x0000000000005a70 .ret_org
+[687](sec  1)(fl 0x00)(ty    0)(scl   6) (nx 0) 0x0000000000005a20 .signed_val
 [688](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000350 .huge
 [689](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000358 .zero
-[690](sec  1)(fl 0x00)(ty    0)(scl   6) (nx 0) 0x0000000000005981 .doret
-[691](sec  1)(fl 0x00)(ty    0)(scl   6) (nx 0) 0x000000000000597b .l1
-[692](sec  1)(fl 0x00)(ty    0)(scl   6) (nx 0) 0x00000000000059c0 .doret2
-[693](sec  1)(fl 0x00)(ty    0)(scl   6) (nx 0) 0x00000000000059e2 .ret_naninf
-[694](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000005910 .text
+[690](sec  1)(fl 0x00)(ty    0)(scl   6) (nx 0) 0x0000000000005a11 .doret
+[691](sec  1)(fl 0x00)(ty    0)(scl   6) (nx 0) 0x0000000000005a0b .l1
+[692](sec  1)(fl 0x00)(ty    0)(scl   6) (nx 0) 0x0000000000005a50 .doret2
+[693](sec  1)(fl 0x00)(ty    0)(scl   6) (nx 0) 0x0000000000005a72 .ret_naninf
+[694](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000059a0 .text
 AUX scnlen 0xd7 nreloc 4 nlnno 0
 [696](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000030 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [698](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b70 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [700](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000474 .xdata
 AUX scnlen 0x4 nreloc 0 nlnno 0
 [702](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000004f8 .pdata
 AUX scnlen 0xc nreloc 3 nlnno 0
 [704](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000350 .rdata
 AUX scnlen 0x10 nreloc 0 nlnno 0
 [706](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000002d2 cos.c
 File 
-[708](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x00000000000059f0 cos
+[708](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000005a80 cos
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[710](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000059f0 .text
+[710](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000005a80 .text
 AUX scnlen 0xf4 nreloc 8 nlnno 0
 [712](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000030 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [714](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b70 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [716](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000360 .rdata
 AUX scnlen 0x10 nreloc 0 nlnno 0
 [718](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000478 .xdata
 AUX scnlen 0xc nreloc 0 nlnno 0
 [720](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000504 .pdata
 AUX scnlen 0xc nreloc 3 nlnno 0
 [722](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000002dc cosl_internal.S
 File 
-[724](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000005af0 __cosl_internal
+[724](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000005b80 __cosl_internal
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[726](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000005af0 .text
+[726](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000005b80 .text
 AUX scnlen 0x30 nreloc 0 nlnno 0
 [728](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000030 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [730](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b70 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [732](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000002ee exp.c
 File 
-[734](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000005b20 exp
+[734](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000005bb0 exp
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
 [736](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000040 c0
 [737](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000030 c1
-[738](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000005b20 .text
+[738](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000005bb0 .text
 AUX scnlen 0x1e4 nreloc 17 nlnno 0
 [740](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000030 .data
 AUX scnlen 0x20 nreloc 0 nlnno 0
 [742](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b70 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [744](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000370 .rdata
 AUX scnlen 0x28 nreloc 0 nlnno 0
 [746](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000484 .xdata
 AUX scnlen 0xc nreloc 0 nlnno 0
 [748](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000510 .pdata
 AUX scnlen 0xc nreloc 3 nlnno 0
 [750](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000002fe log.c
 File 
-[752](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000005d10 log
+[752](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000005da0 log
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[754](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000005d10 .text
+[754](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000005da0 .text
 AUX scnlen 0x120 nreloc 11 nlnno 0
 [756](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000050 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [758](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b70 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [760](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000003a0 .rdata
 AUX scnlen 0x20 nreloc 0 nlnno 0
 [762](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000490 .xdata
 AUX scnlen 0xc nreloc 0 nlnno 0
 [764](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000051c .pdata
 AUX scnlen 0xc nreloc 3 nlnno 0
 [766](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x000000000000030f pow.c
 File 
-[768](sec  1)(fl 0x00)(ty   20)(scl   3) (nx 1) 0x0000000000005e30 internal_modf
+[768](sec  1)(fl 0x00)(ty   20)(scl   3) (nx 1) 0x0000000000005ec0 internal_modf
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[770](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000005ed0 pow
-[771](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000005e30 .text
+[770](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000005f60 pow
+[771](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000005ec0 .text
 AUX scnlen 0x5f7 nreloc 31 nlnno 0
 [773](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000050 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [775](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b70 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [777](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000049c .xdata
 AUX scnlen 0x24 nreloc 0 nlnno 0
 [779](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000528 .pdata
 AUX scnlen 0x18 nreloc 6 nlnno 0
 [781](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000003c0 .rdata
 AUX scnlen 0x80 nreloc 0 nlnno 0
 [783](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x000000000000031f powi.c
 File 
-[785](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000006430 __powi
+[785](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x00000000000064c0 __powi
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[787](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000006430 .text
+[787](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000064c0 .text
 AUX scnlen 0x27e nreloc 15 nlnno 0
 [789](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000050 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [791](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b70 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [793](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000440 .rdata
 AUX scnlen 0x60 nreloc 0 nlnno 0
 [795](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000004c0 .xdata
 AUX scnlen 0xc nreloc 0 nlnno 0
 [797](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000540 .pdata
 AUX scnlen 0xc nreloc 3 nlnno 0
 [799](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000329 exp2l.S
 File 
-[801](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x00000000000066b0 exp2l
+[801](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000006740 exp2l
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[803](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000066b0 .text
+[803](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000006740 .text
 AUX scnlen 0x68 nreloc 0 nlnno 0
 [805](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000050 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [807](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b70 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [809](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000335 internal_logl.S
 File 
-[811](sec  1)(fl 0x00)(ty    0)(scl   6) (nx 0) 0x0000000000006720 one
-[812](sec  1)(fl 0x00)(ty    0)(scl   6) (nx 0) 0x0000000000006728 limit
-[813](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000006730 __logl_internal
+[811](sec  1)(fl 0x00)(ty    0)(scl   6) (nx 0) 0x00000000000067b0 one
+[812](sec  1)(fl 0x00)(ty    0)(scl   6) (nx 0) 0x00000000000067b8 limit
+[813](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x00000000000067c0 __logl_internal
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[815](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000006720 .text
+[815](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000067b0 .text
 AUX scnlen 0x51 nreloc 0 nlnno 0
 [817](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000050 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [819](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b70 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [821](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000343 ldexp.c
 File 
-[823](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000006780 ldexp
+[823](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000006810 ldexp
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[825](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000006780 .text
+[825](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000006810 .text
 AUX scnlen 0xbe nreloc 1 nlnno 0
 [827](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000050 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [829](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b70 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [831](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000004cc .xdata
 AUX scnlen 0x8 nreloc 0 nlnno 0
 [833](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000054c .pdata
 AUX scnlen 0xc nreloc 3 nlnno 0
 [835](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000003e2 log2l.S
 File 
-[837](sec  1)(fl 0x00)(ty    0)(scl   6) (nx 0) 0x0000000000006840 one
-[838](sec  1)(fl 0x00)(ty    0)(scl   6) (nx 0) 0x0000000000006848 limit
-[839](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000006850 log2l
+[837](sec  1)(fl 0x00)(ty    0)(scl   6) (nx 0) 0x00000000000068d0 one
+[838](sec  1)(fl 0x00)(ty    0)(scl   6) (nx 0) 0x00000000000068d8 limit
+[839](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x00000000000068e0 log2l
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[841](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000006840 .text
+[841](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000068d0 .text
 AUX scnlen 0x6c nreloc 0 nlnno 0
 [843](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000050 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [845](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b70 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[847](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000068b0 .text
+[847](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006940 .text
 [848](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
 [849](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
 [850](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000710 .idata$7
 [851](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000034c .idata$5
 [852](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001bc .idata$4
 [853](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000638 .idata$6
-[854](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000068b8 .text
+[854](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006948 .text
 [855](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
 [856](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
 [857](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000070c .idata$7
 [858](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000344 .idata$5
 [859](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001b4 .idata$4
 [860](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000062e .idata$6
-[861](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000068c0 .text
+[861](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006950 .text
 [862](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
 [863](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
 [864](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000708 .idata$7
 [865](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000033c .idata$5
 [866](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001ac .idata$4
 [867](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000624 .idata$6
-[868](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000068c8 .text
+[868](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006958 .text
 [869](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
 [870](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
 [871](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000704 .idata$7
 [872](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000334 .idata$5
 [873](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001a4 .idata$4
 [874](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000061a .idata$6
-[875](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000068d0 .text
+[875](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006960 .text
 [876](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
 [877](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
 [878](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006fc .idata$7
 [879](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000324 .idata$5
 [880](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000194 .idata$4
 [881](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000606 .idata$6
-[882](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000068d8 .text
+[882](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006968 .text
 [883](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
 [884](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
 [885](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006f8 .idata$7
 [886](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000031c .idata$5
 [887](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000018c .idata$4
 [888](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000005fc .idata$6
-[889](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000068e0 .text
+[889](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006970 .text
 [890](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
 [891](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
 [892](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006f4 .idata$7
 [893](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000314 .idata$5
 [894](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000184 .idata$4
 [895](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000005f2 .idata$6
-[896](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000068e8 .text
+[896](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006978 .text
 [897](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
 [898](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
 [899](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006f0 .idata$7
 [900](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000030c .idata$5
 [901](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000017c .idata$4
 [902](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000005ea .idata$6
-[903](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000068f0 .text
+[903](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006980 .text
 [904](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
 [905](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
 [906](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006ec .idata$7
 [907](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000304 .idata$5
 [908](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000174 .idata$4
 [909](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000005e0 .idata$6
-[910](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000068f8 .text
+[910](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006988 .text
 [911](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
 [912](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
 [913](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006e8 .idata$7
 [914](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002fc .idata$5
 [915](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000016c .idata$4
 [916](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000005d8 .idata$6
-[917](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006900 .text
+[917](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006990 .text
 [918](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
 [919](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
 [920](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006e4 .idata$7
 [921](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002f4 .idata$5
 [922](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000164 .idata$4
 [923](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000005ce .idata$6
-[924](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006908 .text
+[924](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006998 .text
 [925](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
 [926](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
 [927](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006e0 .idata$7
 [928](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002ec .idata$5
 [929](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000015c .idata$4
 [930](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000005c6 .idata$6
-[931](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006910 .text
+[931](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000069a0 .text
 [932](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
 [933](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
 [934](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006dc .idata$7
 [935](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002e4 .idata$5
 [936](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000154 .idata$4
 [937](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000005bc .idata$6
-[938](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006918 .text
+[938](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000069a8 .text
 [939](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
 [940](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
 [941](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006d8 .idata$7
 [942](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002dc .idata$5
 [943](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000014c .idata$4
 [944](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000005b4 .idata$6
-[945](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006920 .text
+[945](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000069b0 .text
 [946](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
 [947](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
 [948](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006d4 .idata$7
 [949](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002d4 .idata$5
 [950](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000144 .idata$4
 [951](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000005aa .idata$6
-[952](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006928 .text
+[952](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000069b8 .text
 [953](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
 [954](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
 [955](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006d0 .idata$7
 [956](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002cc .idata$5
 [957](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000013c .idata$4
 [958](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000005a2 .idata$6
-[959](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006930 .text
+[959](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000069c0 .text
 [960](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
 [961](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
 [962](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006cc .idata$7
 [963](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002c4 .idata$5
 [964](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000134 .idata$4
 [965](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000594 .idata$6
-[966](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006938 .text
+[966](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000069c8 .text
 [967](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
 [968](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
 [969](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006c4 .idata$7
 [970](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002b4 .idata$5
 [971](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000124 .idata$4
 [972](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000580 .idata$6
-[973](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006940 .text
+[973](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000069d0 .text
 [974](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
 [975](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
 [976](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006bc .idata$7
 [977](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002a4 .idata$5
 [978](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000114 .idata$4
 [979](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000056c .idata$6
-[980](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006948 .text
+[980](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000069d8 .text
 [981](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
 [982](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
 [983](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006b8 .idata$7
 [984](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000029c .idata$5
 [985](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000010c .idata$4
 [986](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000562 .idata$6
-[987](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006950 .text
+[987](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000069e0 .text
 [988](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
 [989](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
 [990](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006b4 .idata$7
 [991](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000294 .idata$5
 [992](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000104 .idata$4
 [993](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000554 .idata$6
 [994](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000003f2 onexit_table.c
 File 
-[996](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000006960 _initialize_onexit_table
+[996](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x00000000000069f0 _initialize_onexit_table
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[998](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006990 _register_onexit_function
-[999](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006a60 _execute_onexit_table
-[1000](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000006960 .text
+[998](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006a20 _register_onexit_function
+[999](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006af0 _execute_onexit_table
+[1000](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000069f0 .text
 AUX scnlen 0x16f nreloc 8 nlnno 0
 [1002](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000050 .data
 AUX scnlen 0x18 nreloc 3 nlnno 0
 [1004](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b70 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [1006](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000004d4 .xdata
 AUX scnlen 0x20 nreloc 0 nlnno 0
 [1008](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000558 .pdata
 AUX scnlen 0x24 nreloc 9 nlnno 0
 [1010](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000400 acrt_iob_func.c
 File 
-[1012](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000006ad0 __acrt_iob_func
+[1012](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000006b60 __acrt_iob_func
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[1014](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000006ad0 .text
+[1014](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000006b60 .text
 AUX scnlen 0x1f nreloc 1 nlnno 0
 [1016](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000070 .data
 AUX scnlen 0x8 nreloc 1 nlnno 0
 [1018](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b70 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [1020](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000004f4 .xdata
 AUX scnlen 0x8 nreloc 0 nlnno 0
 [1022](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000057c .pdata
 AUX scnlen 0xc nreloc 3 nlnno 0
 [1024](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x000000000000042a fake
 File 
 [1026](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000f4 hname
 [1027](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000284 fthunk
-[1028](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000006af0 .text
+[1028](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000006b80 .text
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [1030](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000080 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [1032](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b70 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [1034](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000014 .idata$2
 AUX scnlen 0x14 nreloc 3 nlnno 0
 [1036](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000f4 .idata$4
 [1037](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000284 .idata$5
-[1038](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006af0 .text
+[1038](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006b80 .text
 [1039](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
 [1040](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
 [1041](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000700 .idata$7
 [1042](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000032c .idata$5
 [1043](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000019c .idata$4
 [1044](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000610 .idata$6
-[1045](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006af8 .text
+[1045](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006b88 .text
 [1046](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
 [1047](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
 [1048](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006c8 .idata$7
 [1049](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002bc .idata$5
 [1050](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000012c .idata$4
 [1051](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000058a .idata$6
-[1052](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006b00 .text
+[1052](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006b90 .text
 [1053](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
 [1054](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
 [1055](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006c0 .idata$7
 [1056](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002ac .idata$5
 [1057](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000011c .idata$4
 [1058](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000578 .idata$6
-[1059](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006b08 .text
+[1059](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006b98 .text
 [1060](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
 [1061](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
 [1062](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006ac .idata$7
 [1063](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000284 .idata$5
 [1064](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000f4 .idata$4
 [1065](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000532 .idata$6
 [1066](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000004cb fake
 File 
-[1068](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000006b10 .text
+[1068](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000006ba0 .text
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [1070](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000080 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [1072](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b70 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [1074](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000001c4 .idata$4
 AUX scnlen 0x8 nreloc 0 nlnno 0
 [1076](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000354 .idata$5
 AUX scnlen 0x8 nreloc 0 nlnno 0
 [1078](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000714 .idata$7
 AUX scnlen 0xb nreloc 0 nlnno 0
-[1080](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006b10 .text
+[1080](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006ba0 .text
 [1081](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
 [1082](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
 [1083](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000698 .idata$7
 [1084](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000274 .idata$5
 [1085](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000e4 .idata$4
 [1086](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000522 .idata$6
-[1087](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006b18 .text
+[1087](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006ba8 .text
 [1088](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
 [1089](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
 [1090](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000694 .idata$7
 [1091](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000026c .idata$5
 [1092](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000dc .idata$4
 [1093](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000510 .idata$6
-[1094](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006b20 .text
+[1094](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006bb0 .text
 [1095](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
 [1096](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
 [1097](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000690 .idata$7
 [1098](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000264 .idata$5
 [1099](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000d4 .idata$4
 [1100](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000004f4 .idata$6
-[1101](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006b28 .text
+[1101](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006bb8 .text
 [1102](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
 [1103](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
 [1104](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000068c .idata$7
 [1105](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000025c .idata$5
 [1106](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000cc .idata$4
 [1107](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000004e6 .idata$6
-[1108](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006b30 .text
+[1108](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006bc0 .text
 [1109](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
 [1110](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
 [1111](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000688 .idata$7
 [1112](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000254 .idata$5
 [1113](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000c4 .idata$4
 [1114](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000004d2 .idata$6
-[1115](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006b38 .text
+[1115](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006bc8 .text
 [1116](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
 [1117](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
 [1118](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000680 .idata$7
 [1119](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000244 .idata$5
 [1120](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000b4 .idata$4
 [1121](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000004ac .idata$6
-[1122](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006b40 .text
+[1122](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006bd0 .text
 [1123](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
 [1124](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
 [1125](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000067c .idata$7
 [1126](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000023c .idata$5
 [1127](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000ac .idata$4
 [1128](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000498 .idata$6
-[1129](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006b48 .text
+[1129](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006bd8 .text
 [1130](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
 [1131](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
 [1132](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000678 .idata$7
 [1133](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000234 .idata$5
 [1134](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000a4 .idata$4
 [1135](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000047e .idata$6
-[1136](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006b50 .text
+[1136](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006be0 .text
 [1137](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
 [1138](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
 [1139](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000674 .idata$7
 [1140](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000022c .idata$5
 [1141](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000009c .idata$4
 [1142](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000046a .idata$6
-[1143](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006b58 .text
+[1143](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006be8 .text
 [1144](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
 [1145](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
 [1146](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000670 .idata$7
 [1147](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000224 .idata$5
 [1148](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000094 .idata$4
 [1149](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000454 .idata$6
-[1150](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006b60 .text
+[1150](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006bf0 .text
 [1151](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
 [1152](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
 [1153](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000066c .idata$7
 [1154](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000021c .idata$5
 [1155](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000008c .idata$4
 [1156](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000043a .idata$6
-[1157](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006b68 .text
+[1157](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006bf8 .text
 [1158](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
 [1159](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
 [1160](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000668 .idata$7
 [1161](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000214 .idata$5
 [1162](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000084 .idata$4
 [1163](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000422 .idata$6
-[1164](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006b70 .text
+[1164](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006c00 .text
 [1165](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
 [1166](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
 [1167](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000664 .idata$7
 [1168](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000020c .idata$5
 [1169](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000007c .idata$4
 [1170](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000406 .idata$6
-[1171](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006b78 .text
+[1171](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006c08 .text
 [1172](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
 [1173](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
 [1174](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000660 .idata$7
 [1175](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000204 .idata$5
 [1176](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000074 .idata$4
 [1177](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000003f6 .idata$6
-[1178](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006b80 .text
+[1178](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006c10 .text
 [1179](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
 [1180](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
 [1181](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000065c .idata$7
 [1182](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001fc .idata$5
 [1183](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000006c .idata$4
 [1184](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000003dc .idata$6
-[1185](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006b88 .text
+[1185](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006c18 .text
 [1186](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
 [1187](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
 [1188](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000658 .idata$7
 [1189](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001f4 .idata$5
 [1190](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000064 .idata$4
 [1191](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000003cc .idata$6
-[1192](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006b90 .text
+[1192](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006c20 .text
 [1193](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
 [1194](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
 [1195](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000654 .idata$7
 [1196](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001ec .idata$5
 [1197](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000005c .idata$4
 [1198](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000003b6 .idata$6
-[1199](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006b98 .text
+[1199](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006c28 .text
 [1200](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
 [1201](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
 [1202](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000650 .idata$7
 [1203](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001e4 .idata$5
 [1204](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000054 .idata$4
 [1205](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000003a0 .idata$6
-[1206](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006ba0 .text
+[1206](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006c30 .text
 [1207](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
 [1208](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
 [1209](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000064c .idata$7
 [1210](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001dc .idata$5
 [1211](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000004c .idata$4
 [1212](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000038c .idata$6
-[1213](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006ba8 .text
+[1213](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006c38 .text
 [1214](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
 [1215](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
 [1216](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000648 .idata$7
 [1217](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001d4 .idata$5
 [1218](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000044 .idata$4
 [1219](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000374 .idata$6
-[1220](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006bb0 .text
+[1220](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006c40 .text
 [1221](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
 [1222](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
 [1223](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000644 .idata$7
 [1224](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001cc .idata$5
 [1225](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000003c .idata$4
 [1226](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000035c .idata$6
 [1227](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000004e5 merr.c
 File 
-[1229](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000006bc0 __mingw_raise_matherr
+[1229](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000006c50 __mingw_raise_matherr
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
 [1231](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 stUserMathErr
-[1232](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006c10 __mingw_setusermatherr
-[1233](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006c20 _matherr
-[1234](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000006bc0 .text
+[1232](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006ca0 __mingw_setusermatherr
+[1233](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006cb0 _matherr
+[1234](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000006c50 .text
 AUX scnlen 0x15c nreloc 14 nlnno 0
 [1236](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000080 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [1238](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b70 .bss
 AUX scnlen 0x8 nreloc 0 nlnno 0
 [1240](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000004fc .xdata
 AUX scnlen 0x24 nreloc 0 nlnno 0
 [1242](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000588 .pdata
 AUX scnlen 0x24 nreloc 9 nlnno 0
 [1244](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000004a0 .rdata
 AUX scnlen 0x140 nreloc 7 nlnno 0
-[1246](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006d20 .text
+[1246](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006db0 .text
 [1247](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
 [1248](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b80 .bss
 [1249](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006b0 .idata$7
 [1250](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000028c .idata$5
 [1251](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000fc .idata$4
 [1252](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000540 .idata$6
 [1253](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000004f7 cygming-crtend.c
 File 
-[1255](sec  1)(fl 0x00)(ty   20)(scl   3) (nx 1) 0x0000000000006da0 register_frame_ctor
+[1255](sec  1)(fl 0x00)(ty   20)(scl   3) (nx 1) 0x0000000000006e30 register_frame_ctor
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[1257](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000006d30 .text
+[1257](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000006dc0 .text
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [1259](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000080 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [1261](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b80 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[1263](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000006da0 .text.startup
+[1263](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000006e30 .text.startup
 AUX scnlen 0x5 nreloc 1 nlnno 0
 [1265](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000520 .xdata.startup
 AUX scnlen 0x4 nreloc 0 nlnno 0
 [1267](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000005ac .pdata.startup
 AUX scnlen 0xc nreloc 3 nlnno 0
-[1269](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000006db8 .ctors.65535
+[1269](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000006e48 .ctors.65535
 AUX scnlen 0x8 nreloc 1 nlnno 0
 [1271](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000008 __xc_z
 [1272](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000900 ___RUNTIME_PSEUDO_RELOC_LIST__
 [1273](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002c4 __imp__vsnprintf
 [1274](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002cc __imp_abort
 [1275](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000069c __lib64_libkernel32_a_iname
 [1276](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __data_start__
-[1277](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006dc8 ___DTOR_LIST__
+[1277](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006e58 ___DTOR_LIST__
 [1278](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002ac __imp__lock
-[1279](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000068d0 printf
+[1279](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006960 printf
 [1280](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002b4 __imp__mkdir
 [1281](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000023c __imp_RtlVirtualUnwind
-[1282](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006b38 SetUnhandledExceptionFilter
-[1283](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006930 _vsnprintf
+[1282](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006bc8 SetUnhandledExceptionFilter
+[1283](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000069c0 _vsnprintf
 [1284](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002d4 __imp_calloc
-[1285](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006b00 _lock
-[1286](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006938 _mkdir
+[1285](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006b90 _lock
+[1286](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000069c8 _mkdir
 [1287](sec 10)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 ___tls_start__
 [1288](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000660 .refptr.__native_startup_state
 [1289](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000646c0000 __ImageBase
 [1290](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000028 __xl_a
-[1291](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006b88 GetLastError
-[1292](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006b80 GetSystemTimeAsFileTime
+[1291](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006c18 GetLastError
+[1292](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006c10 GetSystemTimeAsFileTime
 [1293](sec  6)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000820 mingw_initltssuo_force
 [1294](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000900 __rt_psrelocs_start
 [1295](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __dll_characteristics__
 [1296](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000001000 __size_of_stack_commit__
-[1297](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006b08 __iob_func
+[1297](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006b98 __iob_func
 [1298](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000200000 __size_of_stack_reserve__
 [1299](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000005 __major_subsystem_version__
 [1300](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000028 ___crt_xl_start__
 [1301](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000001cc __imp_DeleteCriticalSection
 [1302](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000038 __xl_d
 [1303](sec 10)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000008 _tls_end
 [1304](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000005f0 .refptr.__CTOR_LIST__
-[1305](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006b10 VirtualQuery
+[1305](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006ba0 VirtualQuery
 [1306](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000010 ___crt_xi_start__
 [1307](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000294 __imp__amsg_exit
 [1308](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000028 ___crt_xi_end__
 [1309](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000029c __imp__errno
 [1310](sec 10)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 _tls_start
-[1311](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000068d8 perror
+[1311](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006968 perror
 [1312](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000610 .refptr.__RUNTIME_PSEUDO_RELOC_LIST__
 [1313](sec  6)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000860 __mingw_oldexcpt_handler
 [1314](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000001ec __imp_GetCurrentThreadId
-[1315](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000068e0 malloc
-[1316](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006b98 GetCurrentProcessId
+[1315](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006970 malloc
+[1316](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006c28 GetCurrentProcessId
 [1317](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000020 _CRT_MT
-[1318](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006b28 TlsGetValue
-[1319](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006b30 TerminateProcess
+[1318](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006bb8 TlsGetValue
+[1319](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006bc0 TerminateProcess
 [1320](sec  6)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __bss_start__
 [1321](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000900 ___RUNTIME_PSEUDO_RELOC_LIST_END__
-[1322](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006b48 RtlLookupFunctionEntry
+[1322](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006bd8 RtlLookupFunctionEntry
 [1323](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000001000 __size_of_heap_commit__
 [1324](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000001f4 __imp_GetLastError
 [1325](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002fc __imp_free
 [1326](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000234 __imp_RtlLookupFunctionEntry
-[1327](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006b18 VirtualProtect
+[1327](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006ba8 VirtualProtect
 [1328](sec  6)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000830 mingw_app_type
 [1329](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000048 ___crt_xp_start__
 [1330](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000214 __imp_LeaveCriticalSection
 [1331](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000204 __imp_GetTickCount
-[1332](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006928 abort
+[1332](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000069b8 abort
 [1333](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000600 .refptr.__RUNTIME_PSEUDO_RELOC_LIST_END__
 [1334](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000048 ___crt_xp_end__
 [1335](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __dll__
 [1336](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __minor_os_version__
 [1337](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000001fc __imp_GetSystemTimeAsFileTime
-[1338](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006ba8 EnterCriticalSection
+[1338](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006c38 EnterCriticalSection
 [1339](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000690 .refptr.__xi_a
 [1340](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000646c0000 __image_base__
 [1341](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000005e0 .refptr._CRT_MT
-[1342](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006b50 RtlCaptureContext
+[1342](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006be0 RtlCaptureContext
 [1343](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000001000 __section_alignment__
 [1344](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000014 __native_dllmain_reason
-[1345](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006920 calloc
+[1345](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000069b0 calloc
 [1346](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000001c0 _tls_used
-[1347](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006b20 UnhandledExceptionFilter
+[1347](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006bb0 UnhandledExceptionFilter
 [1348](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000035c __IAT_end__
 [1349](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000900 __RUNTIME_PSEUDO_RELOC_LIST__
-[1350](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006900 fprintf
+[1350](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006990 fprintf
 [1351](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000224 __imp_RtlAddFunctionTable
-[1352](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000004400 Sleep
+[1352](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000004490 Sleep
 [1353](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000000a0 __data_end__
 [1354](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000304 __imp_fwrite
-[1355](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006db0 __CTOR_LIST__
+[1355](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006e40 __CTOR_LIST__
 [1356](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 _head_lib64_libkernel32_a
 [1357](sec  6)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000b90 __bss_end__
 [1358](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000020 __xi_z
-[1359](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006b78 GetTickCount
+[1359](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006c08 GetTickCount
 [1360](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000018 pcinit
 [1361](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000010 __native_vcclrit_reason
 [1362](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000010 ___crt_xc_end__
-[1363](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006b58 RtlAddFunctionTable
+[1363](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006be8 RtlAddFunctionTable
 [1364](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000650 .refptr.__native_startup_lock
 [1365](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000001d4 __imp_EnterCriticalSection
 [1366](sec  6)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000082c _tls_index
-[1367](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000068c8 signal
+[1367](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006958 signal
 [1368](sec  6)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000b80 __native_startup_state
 [1369](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 ___crt_xc_start__
 [1370](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000001e4 __imp_GetCurrentProcessId
-[1371](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000068b8 strncmp
+[1371](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006948 strncmp
 [1372](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000254 __imp_TerminateProcess
 [1373](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000714 __lib64_libmsvcrt_os_a_iname
-[1374](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006db0 ___CTOR_LIST__
+[1374](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006e40 ___CTOR_LIST__
 [1375](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000620 .refptr.__dyn_tls_init_callback
 [1376](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000334 __imp_signal
-[1377](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000068e8 log10
+[1377](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006978 log10
 [1378](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000058 __imp__register_onexit_function
-[1379](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006af0 realloc
+[1379](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006b80 realloc
 [1380](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __rt_psrelocs_size
 [1381](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000021c __imp_QueryPerformanceCounter
 [1382](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000033c __imp_strlen
 [1383](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000314 __imp_malloc
 [1384](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000200 __file_alignment__
 [1385](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000020c __imp_InitializeCriticalSection
 [1386](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000032c __imp_realloc
-[1387](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006b70 InitializeCriticalSection
+[1387](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006c00 InitializeCriticalSection
 [1388](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002dc __imp_exit
-[1389](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006908 fopen
+[1389](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006998 fopen
 [1390](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000034c __imp_vfprintf
 [1391](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000004 __major_os_version__
-[1392](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006910 fclose
+[1392](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000069a0 fclose
 [1393](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000001cc __IAT_start__
 [1394](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000264 __imp_UnhandledExceptionFilter
 [1395](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000040 __xl_z
 [1396](sec  0)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __end__
 [1397](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000244 __imp_SetUnhandledExceptionFilter
 [1398](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000006b0 .refptr.mingw_app_type
 [1399](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000031c __imp_perror
-[1400](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006dc8 __DTOR_LIST__
-[1401](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006b40 RtlVirtualUnwind
+[1400](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006e58 __DTOR_LIST__
+[1401](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006bd0 RtlVirtualUnwind
 [1402](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000060 __imp__initialize_onexit_table
 [1403](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000010 __xi_a
 [1404](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000024c __imp_Sleep
-[1405](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006b68 LeaveCriticalSection
+[1405](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006bf8 LeaveCriticalSection
 [1406](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __xc_a
 [1407](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000028c __imp___setusermatherr
 [1408](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000100000 __size_of_heap_reserve__
 [1409](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000048 ___crt_xt_start__
 [1410](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000003 __subsystem__
-[1411](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006950 _amsg_exit
+[1411](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000069e0 _amsg_exit
 [1412](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000090 __security_cookie_complement
 [1413](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000025c __imp_TlsGetValue
-[1414](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006ba0 GetCurrentProcess
+[1414](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006c30 GetCurrentProcess
 [1415](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000050 __imp__execute_onexit_table
-[1416](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006d20 __setusermatherr
+[1416](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006db0 __setusermatherr
 [1417](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002f4 __imp_fprintf
 [1418](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000026c __imp_VirtualProtect
 [1419](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000030 __xl_c
 [1420](sec 10)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000010 ___tls_end__
-[1421](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006b60 QueryPerformanceCounter
+[1421](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006bf0 QueryPerformanceCounter
 [1422](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000274 __imp_VirtualQuery
 [1423](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002a4 __imp__initterm
 [1424](sec  6)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000824 mingw_initltsdyn_force
 [1425](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002e4 __imp_fclose
 [1426](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000284 __imp___iob_func
 [1427](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000001a0 __dyn_tls_init_callback
 [1428](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000630 .refptr.__image_base__
-[1429](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006940 _initterm
-[1430](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000068f0 fwrite
+[1429](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000069d0 _initterm
+[1430](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006980 fwrite
 [1431](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000344 __imp_strncmp
 [1432](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000014 _head_lib64_libmsvcrt_os_a
 [1433](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000070 __imp___acrt_iob_func
 [1434](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __major_image_version__
 [1435](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __loader_flags__
-[1436](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000005710 ___chkstk_ms
+[1436](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000057a0 ___chkstk_ms
 [1437](sec  6)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000b88 __native_startup_lock
 [1438](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000640 .refptr.__native_dllmain_reason
 [1439](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000030c __imp_log10
-[1440](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006b90 GetCurrentThreadId
+[1440](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006c20 GetCurrentThreadId
 [1441](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000900 __rt_psrelocs_end
-[1442](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006918 exit
+[1442](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000069a8 exit
 [1443](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000002 __minor_subsystem_version__
 [1444](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __minor_image_version__
 [1445](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002bc __imp__unlock
-[1446](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006948 _errno
+[1446](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000069d8 _errno
 [1447](sec  6)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000828 mingw_initltsdrot_force
 [1448](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000324 __imp_printf
 [1449](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000670 .refptr.__xc_a
-[1450](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000068c0 strlen
+[1450](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006950 strlen
 [1451](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000006a0 .refptr.__xi_z
-[1452](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006bb0 DeleteCriticalSection
+[1452](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006c40 DeleteCriticalSection
 [1453](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000022c __imp_RtlCaptureContext
 [1454](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000900 __RUNTIME_PSEUDO_RELOC_LIST_END__
 [1455](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002ec __imp_fopen
-[1456](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006af8 _unlock
+[1456](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006b88 _unlock
 [1457](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000001dc __imp_GetCurrentProcess
 [1458](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000680 .refptr.__xc_z
 [1459](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000048 ___crt_xt_end__
-[1460](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000068b0 vfprintf
-[1461](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000068f8 free
+[1460](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006940 vfprintf
+[1461](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006988 free
 [1462](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000080 __security_cookie
 
 
 
 Disassembly of section .text:
 
 00000000646c1000 <pre_c_init>:
     646c1000:	lea    0xaff9(%rip),%rcx        # 646cc000 <__bss_start__>
-    646c1007:	jmp    646c7960 <_initialize_onexit_table>
+    646c1007:	jmp    646c79f0 <_initialize_onexit_table>
     646c100c:	nopl   0x0(%rax)
 
 00000000646c1010 <_CRT_INIT>:
     646c1010:	push   %r13
     646c1012:	push   %r12
     646c1014:	push   %rbp
     646c1015:	push   %rdi
@@ -2664,15 +2663,15 @@
     646c1065:	mov    %rax,%rsi
     646c1068:	jne    646c1052 <_CRT_INIT+0x42>
     646c106a:	mov    0x85ef(%rip),%rdi        # 646c9660 <.refptr.__native_startup_state>
     646c1071:	mov    (%rdi),%eax
     646c1073:	cmp    $0x2,%eax
     646c1076:	je     646c1165 <_CRT_INIT+0x155>
     646c107c:	mov    $0x1f,%ecx
-    646c1081:	call   646c7950 <_amsg_exit>
+    646c1081:	call   646c79e0 <_amsg_exit>
     646c1086:	mov    $0x1,%eax
     646c108b:	add    $0x28,%rsp
     646c108f:	pop    %rbx
     646c1090:	pop    %rsi
     646c1091:	pop    %rdi
     646c1092:	pop    %rbp
     646c1093:	pop    %r12
@@ -2733,15 +2732,15 @@
     646c115d:	pop    %rsi
     646c115e:	pop    %rdi
     646c115f:	pop    %rbp
     646c1160:	pop    %r12
     646c1162:	pop    %r13
     646c1164:	ret
     646c1165:	lea    0xae94(%rip),%rcx        # 646cc000 <__bss_start__>
-    646c116c:	call   646c7a60 <_execute_onexit_table>
+    646c116c:	call   646c7af0 <_execute_onexit_table>
     646c1171:	movl   $0x0,(%rdi)
     646c1177:	xchg   %rsi,(%rbx)
     646c117a:	mov    $0x1,%eax
     646c117f:	add    $0x28,%rsp
     646c1183:	pop    %rbx
     646c1184:	pop    %rsi
     646c1185:	pop    %rdi
@@ -2756,25 +2755,25 @@
     646c11a0:	xor    %eax,%eax
     646c11a2:	xchg   %rax,(%rbx)
     646c11a5:	jmp    646c111e <_CRT_INIT+0x10e>
     646c11aa:	nopw   0x0(%rax,%rax,1)
     646c11b0:	mov    0x84e9(%rip),%rdx        # 646c96a0 <.refptr.__xi_z>
     646c11b7:	movl   $0x1,(%rsi)
     646c11bd:	mov    0x84cc(%rip),%rcx        # 646c9690 <.refptr.__xi_a>
-    646c11c4:	call   646c7940 <_initterm>
+    646c11c4:	call   646c79d0 <_initterm>
     646c11c9:	jmp    646c110b <_CRT_INIT+0xfb>
     646c11ce:	xchg   %ax,%ax
     646c11d0:	mov    0x84a9(%rip),%rdx        # 646c9680 <.refptr.__xc_z>
     646c11d7:	mov    0x8492(%rip),%rcx        # 646c9670 <.refptr.__xc_a>
-    646c11de:	call   646c7940 <_initterm>
+    646c11de:	call   646c79d0 <_initterm>
     646c11e3:	movl   $0x2,(%rsi)
     646c11e9:	jmp    646c1116 <_CRT_INIT+0x106>
     646c11ee:	xchg   %ax,%ax
     646c11f0:	mov    $0x1f,%ecx
-    646c11f5:	call   646c7950 <_amsg_exit>
+    646c11f5:	call   646c79e0 <_amsg_exit>
     646c11fa:	jmp    646c110b <_CRT_INIT+0xfb>
     646c11ff:	nop
 
 00000000646c1200 <__DllMainCRTStartup>:
     646c1200:	push   %r12
     646c1202:	push   %rbp
     646c1203:	push   %rdi
@@ -2787,23 +2786,23 @@
     646c1216:	mov    %edx,%ebx
     646c1218:	mov    %edx,(%rsi)
     646c121a:	mov    %r8,%rbp
     646c121d:	jne    646c1273 <__DllMainCRTStartup+0x73>
     646c121f:	mov    0xadf3(%rip),%eax        # 646cc018 <__proc_attached>
     646c1225:	test   %eax,%eax
     646c1227:	je     646c125c <__DllMainCRTStartup+0x5c>
-    646c1229:	call   646c5970 <_pei386_runtime_relocator>
+    646c1229:	call   646c5a00 <_pei386_runtime_relocator>
     646c122e:	mov    %rbp,%r8
     646c1231:	xor    %edx,%edx
     646c1233:	mov    %rdi,%rcx
-    646c1236:	call   646c6760 <DllMain>
+    646c1236:	call   646c67f0 <DllMain>
     646c123b:	mov    %rbp,%r8
     646c123e:	mov    %ebx,%edx
     646c1240:	mov    %rdi,%rcx
-    646c1243:	call   646c6750 <DllEntryPoint>
+    646c1243:	call   646c67e0 <DllEntryPoint>
     646c1248:	mov    %rbp,%r8
     646c124b:	mov    %ebx,%edx
     646c124d:	mov    %rdi,%rcx
     646c1250:	mov    %eax,%r12d
     646c1253:	call   646c1010 <_CRT_INIT>
     646c1258:	test   %eax,%eax
     646c125a:	jne    646c125f <__DllMainCRTStartup+0x5f>
@@ -2813,58 +2812,58 @@
     646c1268:	add    $0x20,%rsp
     646c126c:	pop    %rbx
     646c126d:	pop    %rsi
     646c126e:	pop    %rdi
     646c126f:	pop    %rbp
     646c1270:	pop    %r12
     646c1272:	ret
-    646c1273:	call   646c5970 <_pei386_runtime_relocator>
+    646c1273:	call   646c5a00 <_pei386_runtime_relocator>
     646c1278:	lea    -0x1(%rbx),%eax
     646c127b:	cmp    $0x1,%eax
     646c127e:	jbe    646c12a0 <__DllMainCRTStartup+0xa0>
     646c1280:	mov    %rbp,%r8
     646c1283:	mov    %ebx,%edx
     646c1285:	mov    %rdi,%rcx
-    646c1288:	call   646c6760 <DllMain>
+    646c1288:	call   646c67f0 <DllMain>
     646c128d:	cmp    $0x3,%ebx
     646c1290:	mov    %eax,%r12d
     646c1293:	jne    646c125f <__DllMainCRTStartup+0x5f>
     646c1295:	jmp    646c123b <__DllMainCRTStartup+0x3b>
     646c1297:	nopw   0x0(%rax,%rax,1)
     646c12a0:	mov    %rbp,%r8
     646c12a3:	mov    %ebx,%edx
     646c12a5:	mov    %rdi,%rcx
     646c12a8:	call   646c1010 <_CRT_INIT>
     646c12ad:	test   %eax,%eax
     646c12af:	je     646c125c <__DllMainCRTStartup+0x5c>
     646c12b1:	mov    %rbp,%r8
     646c12b4:	mov    %ebx,%edx
     646c12b6:	mov    %rdi,%rcx
-    646c12b9:	call   646c6750 <DllEntryPoint>
+    646c12b9:	call   646c67e0 <DllEntryPoint>
     646c12be:	test   %eax,%eax
     646c12c0:	mov    %eax,%r12d
     646c12c3:	je     646c1320 <__DllMainCRTStartup+0x120>
     646c12c5:	cmp    $0x1,%ebx
     646c12c8:	jne    646c1280 <__DllMainCRTStartup+0x80>
-    646c12ca:	call   646c54c0 <__main>
+    646c12ca:	call   646c5550 <__main>
     646c12cf:	mov    %rbp,%r8
     646c12d2:	mov    $0x1,%edx
     646c12d7:	mov    %rdi,%rcx
-    646c12da:	call   646c6760 <DllMain>
+    646c12da:	call   646c67f0 <DllMain>
     646c12df:	test   %eax,%eax
     646c12e1:	mov    %eax,%r12d
     646c12e4:	jne    646c125f <__DllMainCRTStartup+0x5f>
     646c12ea:	mov    %rbp,%r8
     646c12ed:	xor    %edx,%edx
     646c12ef:	mov    %rdi,%rcx
-    646c12f2:	call   646c6760 <DllMain>
+    646c12f2:	call   646c67f0 <DllMain>
     646c12f7:	mov    %rbp,%r8
     646c12fa:	xor    %edx,%edx
     646c12fc:	mov    %rdi,%rcx
-    646c12ff:	call   646c6750 <DllEntryPoint>
+    646c12ff:	call   646c67e0 <DllEntryPoint>
     646c1304:	mov    %rbp,%r8
     646c1307:	xor    %edx,%edx
     646c1309:	mov    %rdi,%rcx
     646c130c:	call   646c1010 <_CRT_INIT>
     646c1311:	jmp    646c125f <__DllMainCRTStartup+0x5f>
     646c1316:	cs nopw 0x0(%rax,%rax,1)
     646c1320:	cmp    $0x1,%ebx
@@ -2880,27 +2879,27 @@
     646c1344:	je     646c1350 <DllMainCRTStartup+0x20>
     646c1346:	add    $0x48,%rsp
     646c134a:	jmp    646c1200 <__DllMainCRTStartup>
     646c134f:	nop
     646c1350:	mov    %r8,0x38(%rsp)
     646c1355:	mov    %edx,0x34(%rsp)
     646c1359:	mov    %rcx,0x28(%rsp)
-    646c135e:	call   646c54e0 <__security_init_cookie>
-    646c1363:	call   646c5dd0 <__mingw_init_ehandler>
+    646c135e:	call   646c5570 <__security_init_cookie>
+    646c1363:	call   646c5e60 <__mingw_init_ehandler>
     646c1368:	mov    0x38(%rsp),%r8
     646c136d:	mov    0x34(%rsp),%edx
     646c1371:	mov    0x28(%rsp),%rcx
     646c1376:	add    $0x48,%rsp
     646c137a:	jmp    646c1200 <__DllMainCRTStartup>
     646c137f:	nop
 
 00000000646c1380 <atexit>:
     646c1380:	mov    %rcx,%rdx
     646c1383:	lea    0xac76(%rip),%rcx        # 646cc000 <__bss_start__>
-    646c138a:	jmp    646c7990 <_register_onexit_function>
+    646c138a:	jmp    646c7a20 <_register_onexit_function>
     646c138f:	nop
 
 00000000646c1390 <__gcc_register_frame>:
     646c1390:	lea    0x9(%rip),%rcx        # 646c13a0 <__gcc_deregister_frame>
     646c1397:	jmp    646c1380 <atexit>
     646c139c:	nopl   0x0(%rax)
 
@@ -3934,15 +3933,15 @@
     646c227e:	lea    0x0(,%rax,4),%rdx
     646c2286:	mov    0x10(%rbp),%rax
     646c228a:	add    %rdx,%rax
     646c228d:	mov    (%rax),%eax
     646c228f:	cvtsi2sd %eax,%xmm0
     646c2293:	subsd  0x20(%rbp),%xmm0
     646c2298:	movsd  0x6d80(%rip),%xmm1        # 646c9020 <.rdata+0x20>
-    646c22a0:	call   646c6ed0 <pow>
+    646c22a0:	call   646c6f60 <pow>
     646c22a5:	movapd %xmm0,%xmm1
     646c22a9:	movsd  -0x8(%rbp),%xmm0
     646c22ae:	addsd  %xmm1,%xmm0
     646c22b2:	movsd  %xmm0,-0x8(%rbp)
     646c22b7:	addl   $0x1,-0xc(%rbp)
     646c22bb:	mov    -0xc(%rbp),%eax
     646c22be:	cmp    0x18(%rbp),%eax
@@ -3972,15 +3971,15 @@
     646c230c:	lea    0x0(,%rax,8),%rdx
     646c2314:	mov    0x10(%rbp),%rax
     646c2318:	add    %rdx,%rax
     646c231b:	mov    (%rax),%rax
     646c231e:	cvtsi2sd %rax,%xmm0
     646c2323:	subsd  0x20(%rbp),%xmm0
     646c2328:	movsd  0x6cf0(%rip),%xmm1        # 646c9020 <.rdata+0x20>
-    646c2330:	call   646c6ed0 <pow>
+    646c2330:	call   646c6f60 <pow>
     646c2335:	movapd %xmm0,%xmm1
     646c2339:	movsd  -0x8(%rbp),%xmm0
     646c233e:	addsd  %xmm1,%xmm0
     646c2342:	movsd  %xmm0,-0x8(%rbp)
     646c2347:	addl   $0x1,-0xc(%rbp)
     646c234b:	mov    -0xc(%rbp),%eax
     646c234e:	cmp    0x18(%rbp),%eax
@@ -4010,15 +4009,15 @@
     646c239c:	lea    0x0(,%rax,4),%rdx
     646c23a4:	mov    0x10(%rbp),%rax
     646c23a8:	add    %rdx,%rax
     646c23ab:	movss  (%rax),%xmm0
     646c23af:	cvtss2sd %xmm0,%xmm0
     646c23b3:	subsd  0x20(%rbp),%xmm0
     646c23b8:	movsd  0x6c60(%rip),%xmm1        # 646c9020 <.rdata+0x20>
-    646c23c0:	call   646c6ed0 <pow>
+    646c23c0:	call   646c6f60 <pow>
     646c23c5:	movapd %xmm0,%xmm1
     646c23c9:	movsd  -0x8(%rbp),%xmm0
     646c23ce:	addsd  %xmm1,%xmm0
     646c23d2:	movsd  %xmm0,-0x8(%rbp)
     646c23d7:	addl   $0x1,-0xc(%rbp)
     646c23db:	mov    -0xc(%rbp),%eax
     646c23de:	cmp    0x18(%rbp),%eax
@@ -4047,15 +4046,15 @@
     646c242a:	cltq
     646c242c:	lea    0x0(,%rax,8),%rdx
     646c2434:	mov    0x10(%rbp),%rax
     646c2438:	add    %rdx,%rax
     646c243b:	movsd  (%rax),%xmm0
     646c243f:	subsd  0x20(%rbp),%xmm0
     646c2444:	movsd  0x6bd4(%rip),%xmm1        # 646c9020 <.rdata+0x20>
-    646c244c:	call   646c6ed0 <pow>
+    646c244c:	call   646c6f60 <pow>
     646c2451:	movapd %xmm0,%xmm1
     646c2455:	movsd  -0x8(%rbp),%xmm0
     646c245a:	addsd  %xmm1,%xmm0
     646c245e:	movsd  %xmm0,-0x8(%rbp)
     646c2463:	addl   $0x1,-0xc(%rbp)
     646c2467:	mov    -0xc(%rbp),%eax
     646c246a:	cmp    0x18(%rbp),%eax
@@ -4085,27 +4084,27 @@
     646c24b8:	lea    0x0(,%rax,4),%rdx
     646c24c0:	mov    0x10(%rbp),%rax
     646c24c4:	add    %rdx,%rax
     646c24c7:	mov    (%rax),%eax
     646c24c9:	cvtsi2sd %eax,%xmm0
     646c24cd:	subsd  0x20(%rbp),%xmm0
     646c24d2:	movsd  0x6b46(%rip),%xmm1        # 646c9020 <.rdata+0x20>
-    646c24da:	call   646c6ed0 <pow>
+    646c24da:	call   646c6f60 <pow>
     646c24df:	movapd %xmm0,%xmm1
     646c24e3:	movsd  -0x8(%rbp),%xmm0
     646c24e8:	addsd  %xmm1,%xmm0
     646c24ec:	movsd  %xmm0,-0x8(%rbp)
     646c24f1:	addl   $0x1,-0xc(%rbp)
     646c24f5:	mov    -0xc(%rbp),%eax
     646c24f8:	cmp    0x18(%rbp),%eax
     646c24fb:	jl     646c24b3 <c_array_std_int+0x26>
     646c24fd:	cvtsi2sdl 0x18(%rbp),%xmm1
     646c2502:	movsd  -0x8(%rbp),%xmm0
     646c2507:	divsd  %xmm1,%xmm0
-    646c250b:	call   646c67d0 <sqrt>
+    646c250b:	call   646c6860 <sqrt>
     646c2510:	movq   %xmm0,%rax
     646c2515:	movq   %rax,%xmm0
     646c251a:	add    $0x30,%rsp
     646c251e:	pop    %rbp
     646c251f:	ret
 
 00000000646c2520 <c_array_std_long_long>:
@@ -4124,27 +4123,27 @@
     646c254b:	lea    0x0(,%rax,8),%rdx
     646c2553:	mov    0x10(%rbp),%rax
     646c2557:	add    %rdx,%rax
     646c255a:	mov    (%rax),%rax
     646c255d:	cvtsi2sd %rax,%xmm0
     646c2562:	subsd  0x20(%rbp),%xmm0
     646c2567:	movsd  0x6ab1(%rip),%xmm1        # 646c9020 <.rdata+0x20>
-    646c256f:	call   646c6ed0 <pow>
+    646c256f:	call   646c6f60 <pow>
     646c2574:	movapd %xmm0,%xmm1
     646c2578:	movsd  -0x8(%rbp),%xmm0
     646c257d:	addsd  %xmm1,%xmm0
     646c2581:	movsd  %xmm0,-0x8(%rbp)
     646c2586:	addl   $0x1,-0xc(%rbp)
     646c258a:	mov    -0xc(%rbp),%eax
     646c258d:	cmp    0x18(%rbp),%eax
     646c2590:	jl     646c2546 <c_array_std_long_long+0x26>
     646c2592:	cvtsi2sdl 0x18(%rbp),%xmm1
     646c2597:	movsd  -0x8(%rbp),%xmm0
     646c259c:	divsd  %xmm1,%xmm0
-    646c25a0:	call   646c67d0 <sqrt>
+    646c25a0:	call   646c6860 <sqrt>
     646c25a5:	movq   %xmm0,%rax
     646c25aa:	movq   %rax,%xmm0
     646c25af:	add    $0x30,%rsp
     646c25b3:	pop    %rbp
     646c25b4:	ret
 
 00000000646c25b5 <c_array_std_float>:
@@ -4163,27 +4162,27 @@
     646c25e0:	lea    0x0(,%rax,4),%rdx
     646c25e8:	mov    0x10(%rbp),%rax
     646c25ec:	add    %rdx,%rax
     646c25ef:	movss  (%rax),%xmm0
     646c25f3:	cvtss2sd %xmm0,%xmm0
     646c25f7:	subsd  0x20(%rbp),%xmm0
     646c25fc:	movsd  0x6a1c(%rip),%xmm1        # 646c9020 <.rdata+0x20>
-    646c2604:	call   646c6ed0 <pow>
+    646c2604:	call   646c6f60 <pow>
     646c2609:	movapd %xmm0,%xmm1
     646c260d:	movsd  -0x8(%rbp),%xmm0
     646c2612:	addsd  %xmm1,%xmm0
     646c2616:	movsd  %xmm0,-0x8(%rbp)
     646c261b:	addl   $0x1,-0xc(%rbp)
     646c261f:	mov    -0xc(%rbp),%eax
     646c2622:	cmp    0x18(%rbp),%eax
     646c2625:	jl     646c25db <c_array_std_float+0x26>
     646c2627:	cvtsi2sdl 0x18(%rbp),%xmm1
     646c262c:	movsd  -0x8(%rbp),%xmm0
     646c2631:	divsd  %xmm1,%xmm0
-    646c2635:	call   646c67d0 <sqrt>
+    646c2635:	call   646c6860 <sqrt>
     646c263a:	movq   %xmm0,%rax
     646c263f:	movq   %rax,%xmm0
     646c2644:	add    $0x30,%rsp
     646c2648:	pop    %rbp
     646c2649:	ret
 
 00000000646c264a <c_array_std_double>:
@@ -4201,27 +4200,27 @@
     646c2673:	cltq
     646c2675:	lea    0x0(,%rax,8),%rdx
     646c267d:	mov    0x10(%rbp),%rax
     646c2681:	add    %rdx,%rax
     646c2684:	movsd  (%rax),%xmm0
     646c2688:	subsd  0x20(%rbp),%xmm0
     646c268d:	movsd  0x698b(%rip),%xmm1        # 646c9020 <.rdata+0x20>
-    646c2695:	call   646c6ed0 <pow>
+    646c2695:	call   646c6f60 <pow>
     646c269a:	movapd %xmm0,%xmm1
     646c269e:	movsd  -0x8(%rbp),%xmm0
     646c26a3:	addsd  %xmm1,%xmm0
     646c26a7:	movsd  %xmm0,-0x8(%rbp)
     646c26ac:	addl   $0x1,-0xc(%rbp)
     646c26b0:	mov    -0xc(%rbp),%eax
     646c26b3:	cmp    0x18(%rbp),%eax
     646c26b6:	jl     646c2670 <c_array_std_double+0x26>
     646c26b8:	cvtsi2sdl 0x18(%rbp),%xmm1
     646c26bd:	movsd  -0x8(%rbp),%xmm0
     646c26c2:	divsd  %xmm1,%xmm0
-    646c26c6:	call   646c67d0 <sqrt>
+    646c26c6:	call   646c6860 <sqrt>
     646c26cb:	movq   %xmm0,%rax
     646c26d0:	movq   %rax,%xmm0
     646c26d5:	add    $0x30,%rsp
     646c26d9:	pop    %rbp
     646c26da:	ret
 
 00000000646c26db <c_array_mean_int>:
@@ -4821,24 +4820,24 @@
     646c2e45:	mov    %rax,-0x18(%rbp)
     646c2e49:	mov    0x10(%rbp),%rcx
     646c2e4d:	call   646c2d5e <mt19937_get_double>
     646c2e52:	movq   %xmm0,%rax
     646c2e57:	mov    %rax,-0x20(%rbp)
     646c2e5b:	mov    -0x18(%rbp),%rax
     646c2e5f:	movq   %rax,%xmm0
-    646c2e64:	call   646c6d10 <log>
+    646c2e64:	call   646c6da0 <log>
     646c2e69:	movapd %xmm0,%xmm1
     646c2e6d:	movsd  0x61cb(%rip),%xmm0        # 646c9040 <.rdata+0x10>
     646c2e75:	mulsd  %xmm1,%xmm0
-    646c2e79:	call   646c67d0 <sqrt>
+    646c2e79:	call   646c6860 <sqrt>
     646c2e7e:	movapd %xmm0,%xmm6
     646c2e82:	movsd  -0x20(%rbp),%xmm1
     646c2e87:	movsd  0x61b9(%rip),%xmm0        # 646c9048 <.rdata+0x18>
     646c2e8f:	mulsd  %xmm1,%xmm0
-    646c2e93:	call   646c69f0 <cos>
+    646c2e93:	call   646c6a80 <cos>
     646c2e98:	mulsd  %xmm6,%xmm0
     646c2e9c:	movsd  %xmm0,-0x28(%rbp)
     646c2ea1:	movsd  -0x28(%rbp),%xmm0
     646c2ea6:	movq   %xmm0,%rax
     646c2eab:	movq   %rax,%xmm0
     646c2eb0:	movaps -0x10(%rbp),%xmm6
     646c2eb4:	add    $0x50,%rsp
@@ -4860,5773 +4859,5813 @@
     646c2ecf:	movsd  %xmm3,0x28(%rbp)
     646c2ed4:	mov    0x10(%rbp),%rax
     646c2ed8:	mov    0x18(%rbp),%edx
     646c2edb:	mov    %edx,(%rax)
     646c2edd:	mov    0x10(%rbp),%rax
     646c2ee1:	mov    0x20(%rbp),%edx
     646c2ee4:	mov    %edx,0x4(%rax)
-    646c2ee7:	mov    0x10(%rbp),%rax
-    646c2eeb:	movsd  0x28(%rbp),%xmm0
-    646c2ef0:	movsd  %xmm0,0x8(%rax)
-    646c2ef5:	mov    0x10(%rbp),%rax
-    646c2ef9:	movsd  0x30(%rbp),%xmm0
-    646c2efe:	movsd  %xmm0,0x10(%rax)
-    646c2f03:	nop
-    646c2f04:	pop    %rbp
-    646c2f05:	ret
-
-00000000646c2f06 <cov_model>:
-    646c2f06:	push   %rbp
-    646c2f07:	mov    %rsp,%rbp
-    646c2f0a:	sub    $0x30,%rsp
-    646c2f0e:	mov    %rcx,0x10(%rbp)
-    646c2f12:	mov    %rdx,0x18(%rbp)
-    646c2f16:	mov    %r8d,0x20(%rbp)
-    646c2f1a:	movsd  %xmm3,0x28(%rbp)
-    646c2f1f:	movl   $0x0,-0x4(%rbp)
-    646c2f26:	jmp    646c2fbc <cov_model+0xb6>
-    646c2f2b:	mov    -0x4(%rbp),%eax
-    646c2f2e:	cltq
-    646c2f30:	lea    0x0(,%rax,8),%rdx
-    646c2f38:	mov    0x10(%rbp),%rax
-    646c2f3c:	add    %rdx,%rax
-    646c2f3f:	movsd  (%rax),%xmm1
-    646c2f43:	mov    -0x4(%rbp),%eax
-    646c2f46:	cltq
-    646c2f48:	lea    0x0(,%rax,8),%rdx
-    646c2f50:	mov    0x10(%rbp),%rax
-    646c2f54:	add    %rdx,%rax
-    646c2f57:	movsd  (%rax),%xmm0
-    646c2f5b:	mulsd  %xmm0,%xmm1
-    646c2f5f:	movsd  0x60e9(%rip),%xmm0        # 646c9050 <.rdata>
-    646c2f67:	mulsd  %xmm1,%xmm0
-    646c2f6b:	movsd  0x28(%rbp),%xmm1
-    646c2f70:	mulsd  0x28(%rbp),%xmm1
-    646c2f75:	divsd  %xmm1,%xmm0
-    646c2f79:	call   646c6b20 <exp>
-    646c2f7e:	movapd %xmm0,%xmm1
-    646c2f82:	movsd  0x60ce(%rip),%xmm0        # 646c9058 <.rdata+0x8>
-    646c2f8a:	subsd  %xmm1,%xmm0
-    646c2f8e:	movapd %xmm0,%xmm1
-    646c2f92:	mulsd  0x30(%rbp),%xmm1
-    646c2f97:	mov    -0x4(%rbp),%eax
-    646c2f9a:	cltq
-    646c2f9c:	lea    0x0(,%rax,8),%rdx
-    646c2fa4:	mov    0x18(%rbp),%rax
-    646c2fa8:	add    %rdx,%rax
-    646c2fab:	movsd  0x30(%rbp),%xmm0
-    646c2fb0:	subsd  %xmm1,%xmm0
-    646c2fb4:	movsd  %xmm0,(%rax)
-    646c2fb8:	addl   $0x1,-0x4(%rbp)
-    646c2fbc:	mov    -0x4(%rbp),%eax
-    646c2fbf:	cmp    0x20(%rbp),%eax
-    646c2fc2:	jl     646c2f2b <cov_model+0x25>
-    646c2fc8:	nop
-    646c2fc9:	add    $0x30,%rsp
-    646c2fcd:	pop    %rbp
-    646c2fce:	ret
-
-00000000646c2fcf <cov_model2d>:
-    646c2fcf:	push   %rbp
-    646c2fd0:	mov    %rsp,%rbp
-    646c2fd3:	sub    $0x30,%rsp
-    646c2fd7:	mov    %rcx,0x10(%rbp)
-    646c2fdb:	mov    %rdx,0x18(%rbp)
-    646c2fdf:	mov    %r8d,0x20(%rbp)
-    646c2fe3:	movsd  %xmm3,0x28(%rbp)
-    646c2fe8:	movl   $0x0,-0x4(%rbp)
-    646c2fef:	jmp    646c30c8 <cov_model2d+0xf9>
-    646c2ff4:	movl   $0x0,-0x8(%rbp)
-    646c2ffb:	jmp    646c30b8 <cov_model2d+0xe9>
-    646c3000:	mov    -0x4(%rbp),%eax
-    646c3003:	cltq
-    646c3005:	lea    0x0(,%rax,8),%rdx
-    646c300d:	mov    0x10(%rbp),%rax
-    646c3011:	add    %rdx,%rax
-    646c3014:	mov    (%rax),%rdx
-    646c3017:	mov    -0x8(%rbp),%eax
-    646c301a:	cltq
-    646c301c:	shl    $0x3,%rax
-    646c3020:	add    %rdx,%rax
-    646c3023:	movsd  (%rax),%xmm1
-    646c3027:	mov    -0x4(%rbp),%eax
-    646c302a:	cltq
-    646c302c:	lea    0x0(,%rax,8),%rdx
-    646c3034:	mov    0x10(%rbp),%rax
-    646c3038:	add    %rdx,%rax
-    646c303b:	mov    (%rax),%rdx
-    646c303e:	mov    -0x8(%rbp),%eax
-    646c3041:	cltq
-    646c3043:	shl    $0x3,%rax
-    646c3047:	add    %rdx,%rax
-    646c304a:	movsd  (%rax),%xmm0
-    646c304e:	mulsd  %xmm0,%xmm1
-    646c3052:	movsd  0x5ff6(%rip),%xmm0        # 646c9050 <.rdata>
-    646c305a:	mulsd  %xmm1,%xmm0
-    646c305e:	movsd  0x28(%rbp),%xmm1
-    646c3063:	mulsd  0x28(%rbp),%xmm1
-    646c3068:	divsd  %xmm1,%xmm0
-    646c306c:	call   646c6b20 <exp>
-    646c3071:	movapd %xmm0,%xmm1
-    646c3075:	movsd  0x5fdb(%rip),%xmm0        # 646c9058 <.rdata+0x8>
-    646c307d:	subsd  %xmm1,%xmm0
-    646c3081:	movapd %xmm0,%xmm1
-    646c3085:	mulsd  0x30(%rbp),%xmm1
-    646c308a:	mov    0x20(%rbp),%eax
-    646c308d:	imul   -0x4(%rbp),%eax
-    646c3091:	mov    -0x8(%rbp),%edx
-    646c3094:	add    %edx,%eax
-    646c3096:	cltq
-    646c3098:	lea    0x0(,%rax,8),%rdx
-    646c30a0:	mov    0x18(%rbp),%rax
-    646c30a4:	add    %rdx,%rax
-    646c30a7:	movsd  0x30(%rbp),%xmm0
-    646c30ac:	subsd  %xmm1,%xmm0
-    646c30b0:	movsd  %xmm0,(%rax)
-    646c30b4:	addl   $0x1,-0x8(%rbp)
-    646c30b8:	mov    -0x8(%rbp),%eax
-    646c30bb:	cmp    0x20(%rbp),%eax
-    646c30be:	jl     646c3000 <cov_model2d+0x31>
-    646c30c4:	addl   $0x1,-0x4(%rbp)
-    646c30c8:	mov    -0x4(%rbp),%eax
-    646c30cb:	cmp    0x20(%rbp),%eax
-    646c30ce:	jl     646c2ff4 <cov_model2d+0x25>
-    646c30d4:	nop
-    646c30d5:	add    $0x30,%rsp
-    646c30d9:	pop    %rbp
-    646c30da:	ret
-    646c30db:	nop
-    646c30dc:	nop
-    646c30dd:	nop
-    646c30de:	nop
-    646c30df:	nop
-
-00000000646c30e0 <sampling_state_init>:
-    646c30e0:	push   %rbp
-    646c30e1:	mov    %rsp,%rbp
-    646c30e4:	sub    $0x20,%rsp
-    646c30e8:	mov    %rcx,0x10(%rbp)
-    646c30ec:	mov    %edx,0x18(%rbp)
-    646c30ef:	mov    0x10(%rbp),%rax
-    646c30f3:	movl   $0x0,(%rax)
-    646c30f9:	mov    0x10(%rbp),%rax
-    646c30fd:	movl   $0x0,0x4(%rax)
-    646c3104:	mov    0x10(%rbp),%rax
-    646c3108:	movl   $0x0,0x8(%rax)
-    646c310f:	mov    0x10(%rbp),%rax
-    646c3113:	pxor   %xmm0,%xmm0
-    646c3117:	movsd  %xmm0,0x10(%rax)
-    646c311c:	mov    0x18(%rbp),%eax
-    646c311f:	cltq
-    646c3121:	mov    0x10(%rbp),%rdx
-    646c3125:	mov    %rax,0x20(%rdx)
-    646c3129:	mov    0x18(%rbp),%eax
-    646c312c:	cltq
-    646c312e:	mov    0x10(%rbp),%rdx
-    646c3132:	mov    %rax,0x28(%rdx)
-    646c3136:	mov    0x18(%rbp),%eax
-    646c3139:	cltq
-    646c313b:	mov    $0x8,%edx
-    646c3140:	mov    %rax,%rcx
-    646c3143:	call   646c7920 <calloc>
-    646c3148:	mov    %rax,%rdx
-    646c314b:	mov    0x10(%rbp),%rax
-    646c314f:	mov    %rdx,0x18(%rax)
-    646c3153:	mov    0x18(%rbp),%eax
-    646c3156:	cltq
-    646c3158:	mov    0x10(%rbp),%rdx
-    646c315c:	mov    %rax,0x38(%rdx)
-    646c3160:	mov    0x18(%rbp),%eax
-    646c3163:	cltq
-    646c3165:	mov    0x10(%rbp),%rdx
-    646c3169:	mov    %rax,0x40(%rdx)
-    646c316d:	mov    0x18(%rbp),%eax
-    646c3170:	cltq
-    646c3172:	mov    $0x8,%edx
-    646c3177:	mov    %rax,%rcx
-    646c317a:	call   646c7920 <calloc>
-    646c317f:	mov    %rax,%rdx
-    646c3182:	mov    0x10(%rbp),%rax
-    646c3186:	mov    %rdx,0x30(%rax)
-    646c318a:	nop
-    646c318b:	add    $0x20,%rsp
-    646c318f:	pop    %rbp
-    646c3190:	ret
-
-00000000646c3191 <sampling_state_update>:
-    646c3191:	push   %rbp
-    646c3192:	mov    %rsp,%rbp
-    646c3195:	mov    %rcx,0x10(%rbp)
-    646c3199:	movsd  %xmm1,0x18(%rbp)
-    646c319e:	mov    %r8d,0x20(%rbp)
-    646c31a2:	mov    0x10(%rbp),%rax
-    646c31a6:	movsd  0x18(%rbp),%xmm0
-    646c31ab:	movsd  %xmm0,0x10(%rax)
-    646c31b0:	mov    0x10(%rbp),%rax
-    646c31b4:	mov    0x20(%rbp),%edx
-    646c31b7:	mov    %edx,0x8(%rax)
-    646c31ba:	nop
-    646c31bb:	pop    %rbp
-    646c31bc:	ret
-
-00000000646c31bd <krige_param_setting>:
-    646c31bd:	push   %rbp
-    646c31be:	push   %rbx
-    646c31bf:	sub    $0x38,%rsp
-    646c31c3:	lea    0x80(%rsp),%rbp
-    646c31cb:	movsd  %xmm0,-0x30(%rbp)
-    646c31d0:	movsd  %xmm1,-0x28(%rbp)
-    646c31d5:	movsd  -0x30(%rbp),%xmm0
-    646c31da:	movsd  %xmm0,0x8e3e(%rip)        # 646cc020 <range>
-    646c31e2:	movsd  -0x28(%rbp),%xmm0
-    646c31e7:	movsd  %xmm0,0x8e39(%rip)        # 646cc028 <sill>
-    646c31ef:	movq   $0xa,0x8e5e(%rip)        # 646cc058 <location+0x8>
-    646c31fa:	movq   $0xa,0x8e5b(%rip)        # 646cc060 <location+0x10>
-    646c3205:	mov    $0x8,%edx
-    646c320a:	mov    $0xa,%ecx
-    646c320f:	call   646c7920 <calloc>
-    646c3214:	mov    %rax,0x8e35(%rip)        # 646cc050 <location>
-    646c321b:	movq   $0xa,0x8e52(%rip)        # 646cc078 <loc_cov+0x8>
-    646c3226:	movq   $0xa,0x8e4f(%rip)        # 646cc080 <loc_cov+0x10>
-    646c3231:	mov    $0x8,%edx
-    646c3236:	mov    $0xa,%ecx
-    646c323b:	call   646c7920 <calloc>
-    646c3240:	mov    %rax,0x8e29(%rip)        # 646cc070 <loc_cov>
-    646c3247:	movq   $0xa,0x8e66(%rip)        # 646cc0b8 <loc_cov2+0x8>
-    646c3252:	movq   $0xa,0x8e63(%rip)        # 646cc0c0 <loc_cov2+0x10>
-    646c325d:	mov    $0x8,%edx
-    646c3262:	mov    $0xa,%ecx
-    646c3267:	call   646c7920 <calloc>
-    646c326c:	mov    %rax,0x8e3d(%rip)        # 646cc0b0 <loc_cov2>
-    646c3273:	movq   $0xa,0x8e7a(%rip)        # 646cc0f8 <weights+0x8>
-    646c327e:	movq   $0xa,0x8e77(%rip)        # 646cc100 <weights+0x10>
-    646c3289:	mov    $0x8,%edx
-    646c328e:	mov    $0xa,%ecx
-    646c3293:	call   646c7920 <calloc>
-    646c3298:	mov    %rax,0x8e51(%rip)        # 646cc0f0 <weights>
-    646c329f:	movq   $0x64,0x8e2e(%rip)        # 646cc0d8 <flatten_temp+0x8>
-    646c32aa:	movq   $0x64,0x8e2b(%rip)        # 646cc0e0 <flatten_temp+0x10>
-    646c32b5:	mov    $0x8,%edx
-    646c32ba:	mov    $0x64,%ecx
-    646c32bf:	call   646c7920 <calloc>
-    646c32c4:	mov    %rax,0x8e05(%rip)        # 646cc0d0 <flatten_temp>
-    646c32cb:	movq   $0xa,0x8dc2(%rip)        # 646cc098 <data_temp+0x8>
-    646c32d6:	movq   $0xa,0x8dbf(%rip)        # 646cc0a0 <data_temp+0x10>
-    646c32e1:	mov    $0x8,%edx
-    646c32e6:	mov    $0xa,%ecx
-    646c32eb:	call   646c7920 <calloc>
-    646c32f0:	mov    %rax,0x8d99(%rip)        # 646cc090 <data_temp>
-    646c32f7:	movq   $0xa,0x8e36(%rip)        # 646cc138 <pdist_temp+0x8>
-    646c3302:	movq   $0xa,0x8e33(%rip)        # 646cc140 <pdist_temp+0x10>
-    646c330d:	mov    $0x50,%ecx
-    646c3312:	call   646c78e0 <malloc>
-    646c3317:	mov    %rax,0x8e12(%rip)        # 646cc130 <pdist_temp>
-    646c331e:	movl   $0x0,-0x54(%rbp)
-    646c3325:	jmp    646c334c <krige_param_setting+0x18f>
-    646c3327:	mov    0x8e02(%rip),%rdx        # 646cc130 <pdist_temp>
-    646c332e:	mov    -0x54(%rbp),%eax
-    646c3331:	cltq
-    646c3333:	shl    $0x3,%rax
-    646c3337:	lea    (%rdx,%rax,1),%rbx
-    646c333b:	mov    $0x50,%ecx
-    646c3340:	call   646c78e0 <malloc>
-    646c3345:	mov    %rax,(%rbx)
-    646c3348:	addl   $0x1,-0x54(%rbp)
-    646c334c:	cmpl   $0x9,-0x54(%rbp)
-    646c3350:	jle    646c3327 <krige_param_setting+0x16a>
-    646c3352:	movq   $0xa,0x8dfb(%rip)        # 646cc158 <datacov+0x8>
-    646c335d:	movq   $0xa,0x8df8(%rip)        # 646cc160 <datacov+0x10>
-    646c3368:	mov    $0x50,%ecx
-    646c336d:	call   646c78e0 <malloc>
-    646c3372:	mov    %rax,0x8dd7(%rip)        # 646cc150 <datacov>
-    646c3379:	movl   $0x0,-0x58(%rbp)
-    646c3380:	jmp    646c33a7 <krige_param_setting+0x1ea>
-    646c3382:	mov    0x8dc7(%rip),%rdx        # 646cc150 <datacov>
-    646c3389:	mov    -0x58(%rbp),%eax
-    646c338c:	cltq
-    646c338e:	shl    $0x3,%rax
-    646c3392:	lea    (%rdx,%rax,1),%rbx
-    646c3396:	mov    $0x50,%ecx
-    646c339b:	call   646c78e0 <malloc>
-    646c33a0:	mov    %rax,(%rbx)
-    646c33a3:	addl   $0x1,-0x58(%rbp)
-    646c33a7:	cmpl   $0x9,-0x58(%rbp)
-    646c33ab:	jle    646c3382 <krige_param_setting+0x1c5>
-    646c33ad:	movq   $0x96,0x8d60(%rip)        # 646cc118 <array2d_temp+0x8>
-    646c33b8:	movq   $0x3,0x8d5d(%rip)        # 646cc120 <array2d_temp+0x10>
-    646c33c3:	mov    $0x4b0,%ecx
-    646c33c8:	call   646c78e0 <malloc>
-    646c33cd:	mov    %rax,0x8d3c(%rip)        # 646cc110 <array2d_temp>
-    646c33d4:	movl   $0x0,-0x5c(%rbp)
-    646c33db:	jmp    646c3402 <krige_param_setting+0x245>
-    646c33dd:	mov    0x8d2c(%rip),%rdx        # 646cc110 <array2d_temp>
-    646c33e4:	mov    -0x5c(%rbp),%eax
-    646c33e7:	cltq
-    646c33e9:	shl    $0x3,%rax
-    646c33ed:	lea    (%rdx,%rax,1),%rbx
-    646c33f1:	mov    $0x18,%ecx
-    646c33f6:	call   646c78e0 <malloc>
-    646c33fb:	mov    %rax,(%rbx)
-    646c33fe:	addl   $0x1,-0x5c(%rbp)
-    646c3402:	cmpl   $0x95,-0x5c(%rbp)
-    646c3409:	jle    646c33dd <krige_param_setting+0x220>
-    646c340b:	nop
-    646c340c:	add    $0x38,%rsp
-    646c3410:	pop    %rbx
-    646c3411:	pop    %rbp
-    646c3412:	ret
-
-00000000646c3413 <simple_kriging>:
-    646c3413:	push   %rbp
-    646c3414:	mov    %rsp,%rbp
-    646c3417:	sub    $0x50,%rsp
-    646c341b:	movaps %xmm6,-0x10(%rbp)
-    646c341f:	mov    %rcx,0x10(%rbp)
-    646c3423:	mov    %rdx,0x18(%rbp)
-    646c3427:	mov    %r8,0x20(%rbp)
-    646c342b:	mov    0x20(%rbp),%rdx
-    646c342f:	mov    0x18(%rbp),%rax
-    646c3433:	mov    %rdx,%r8
-    646c3436:	mov    %rax,%rdx
-    646c3439:	mov    0x10(%rbp),%rcx
-    646c343d:	call   646c383d <find_neighbor>
-    646c3442:	mov    %eax,-0x20(%rbp)
-    646c3445:	cmpl   $0x0,-0x20(%rbp)
-    646c3449:	je     646c3832 <simple_kriging+0x41f>
-    646c344f:	movl   $0x0,-0x14(%rbp)
-    646c3456:	jmp    646c3516 <simple_kriging+0x103>
-    646c345b:	mov    0x18(%rbp),%rax
-    646c345f:	mov    0x18(%rax),%rdx
-    646c3463:	mov    -0x14(%rbp),%eax
+    646c2ee7:	mov    0x18(%rbp),%eax
+    646c2eea:	cltd
+    646c2eeb:	idivl  0x20(%rbp)
+    646c2eee:	mov    %eax,%edx
+    646c2ef0:	mov    0x10(%rbp),%rax
+    646c2ef4:	mov    %edx,0x8(%rax)
+    646c2ef7:	mov    0x10(%rbp),%rax
+    646c2efb:	movsd  0x28(%rbp),%xmm0
+    646c2f00:	movsd  %xmm0,0x10(%rax)
+    646c2f05:	mov    0x10(%rbp),%rax
+    646c2f09:	movsd  0x30(%rbp),%xmm0
+    646c2f0e:	movsd  %xmm0,0x18(%rax)
+    646c2f13:	mov    0x10(%rbp),%rax
+    646c2f17:	movsd  0x38(%rbp),%xmm0
+    646c2f1c:	movsd  %xmm0,0x20(%rax)
+    646c2f21:	nop
+    646c2f22:	pop    %rbp
+    646c2f23:	ret
+
+00000000646c2f24 <cov_model>:
+    646c2f24:	push   %rbp
+    646c2f25:	mov    %rsp,%rbp
+    646c2f28:	sub    $0x40,%rsp
+    646c2f2c:	mov    %rcx,0x10(%rbp)
+    646c2f30:	mov    %rdx,0x18(%rbp)
+    646c2f34:	mov    %r8d,0x20(%rbp)
+    646c2f38:	mov    %r9,0x28(%rbp)
+    646c2f3c:	mov    0x28(%rbp),%rax
+    646c2f40:	movsd  0x18(%rax),%xmm0
+    646c2f45:	mov    0x28(%rbp),%rax
+    646c2f49:	movsd  0x20(%rax),%xmm1
+    646c2f4e:	subsd  %xmm1,%xmm0
+    646c2f52:	movsd  %xmm0,-0x10(%rbp)
+    646c2f57:	movl   $0x0,-0x4(%rbp)
+    646c2f5e:	jmp    646c301b <cov_model+0xf7>
+    646c2f63:	mov    -0x4(%rbp),%eax
+    646c2f66:	cltq
+    646c2f68:	lea    0x0(,%rax,8),%rdx
+    646c2f70:	mov    0x10(%rbp),%rax
+    646c2f74:	add    %rdx,%rax
+    646c2f77:	movsd  (%rax),%xmm1
+    646c2f7b:	mov    -0x4(%rbp),%eax
+    646c2f7e:	cltq
+    646c2f80:	lea    0x0(,%rax,8),%rdx
+    646c2f88:	mov    0x10(%rbp),%rax
+    646c2f8c:	add    %rdx,%rax
+    646c2f8f:	movsd  (%rax),%xmm0
+    646c2f93:	mulsd  %xmm0,%xmm1
+    646c2f97:	movsd  0x60b1(%rip),%xmm0        # 646c9050 <.rdata>
+    646c2f9f:	mulsd  %xmm1,%xmm0
+    646c2fa3:	mov    0x28(%rbp),%rax
+    646c2fa7:	movsd  0x10(%rax),%xmm2
+    646c2fac:	mov    0x28(%rbp),%rax
+    646c2fb0:	movsd  0x10(%rax),%xmm1
+    646c2fb5:	mulsd  %xmm2,%xmm1
+    646c2fb9:	divsd  %xmm1,%xmm0
+    646c2fbd:	call   646c6bb0 <exp>
+    646c2fc2:	movapd %xmm0,%xmm1
+    646c2fc6:	movsd  0x608a(%rip),%xmm0        # 646c9058 <.rdata+0x8>
+    646c2fce:	subsd  %xmm1,%xmm0
+    646c2fd2:	movsd  %xmm0,-0x18(%rbp)
+    646c2fd7:	mov    0x28(%rbp),%rax
+    646c2fdb:	movsd  0x18(%rax),%xmm0
+    646c2fe0:	movsd  -0x10(%rbp),%xmm1
+    646c2fe5:	mulsd  -0x18(%rbp),%xmm1
+    646c2fea:	subsd  %xmm1,%xmm0
+    646c2fee:	movapd %xmm0,%xmm1
+    646c2ff2:	mov    0x28(%rbp),%rax
+    646c2ff6:	movsd  0x20(%rax),%xmm0
+    646c2ffb:	mov    -0x4(%rbp),%eax
+    646c2ffe:	cltq
+    646c3000:	lea    0x0(,%rax,8),%rdx
+    646c3008:	mov    0x18(%rbp),%rax
+    646c300c:	add    %rdx,%rax
+    646c300f:	addsd  %xmm1,%xmm0
+    646c3013:	movsd  %xmm0,(%rax)
+    646c3017:	addl   $0x1,-0x4(%rbp)
+    646c301b:	mov    -0x4(%rbp),%eax
+    646c301e:	cmp    0x20(%rbp),%eax
+    646c3021:	jl     646c2f63 <cov_model+0x3f>
+    646c3027:	nop
+    646c3028:	add    $0x40,%rsp
+    646c302c:	pop    %rbp
+    646c302d:	ret
+
+00000000646c302e <cov_model2d>:
+    646c302e:	push   %rbp
+    646c302f:	mov    %rsp,%rbp
+    646c3032:	sub    $0x40,%rsp
+    646c3036:	mov    %rcx,0x10(%rbp)
+    646c303a:	mov    %rdx,0x18(%rbp)
+    646c303e:	mov    %r8d,0x20(%rbp)
+    646c3042:	mov    %r9,0x28(%rbp)
+    646c3046:	mov    0x28(%rbp),%rax
+    646c304a:	movsd  0x18(%rax),%xmm0
+    646c304f:	mov    0x28(%rbp),%rax
+    646c3053:	movsd  0x20(%rax),%xmm1
+    646c3058:	subsd  %xmm1,%xmm0
+    646c305c:	movsd  %xmm0,-0x10(%rbp)
+    646c3061:	movl   $0x0,-0x4(%rbp)
+    646c3068:	jmp    646c3168 <cov_model2d+0x13a>
+    646c306d:	movl   $0x0,-0x8(%rbp)
+    646c3074:	jmp    646c3158 <cov_model2d+0x12a>
+    646c3079:	mov    -0x4(%rbp),%eax
+    646c307c:	cltq
+    646c307e:	lea    0x0(,%rax,8),%rdx
+    646c3086:	mov    0x10(%rbp),%rax
+    646c308a:	add    %rdx,%rax
+    646c308d:	mov    (%rax),%rdx
+    646c3090:	mov    -0x8(%rbp),%eax
+    646c3093:	cltq
+    646c3095:	shl    $0x3,%rax
+    646c3099:	add    %rdx,%rax
+    646c309c:	movsd  (%rax),%xmm1
+    646c30a0:	mov    -0x4(%rbp),%eax
+    646c30a3:	cltq
+    646c30a5:	lea    0x0(,%rax,8),%rdx
+    646c30ad:	mov    0x10(%rbp),%rax
+    646c30b1:	add    %rdx,%rax
+    646c30b4:	mov    (%rax),%rdx
+    646c30b7:	mov    -0x8(%rbp),%eax
+    646c30ba:	cltq
+    646c30bc:	shl    $0x3,%rax
+    646c30c0:	add    %rdx,%rax
+    646c30c3:	movsd  (%rax),%xmm0
+    646c30c7:	mulsd  %xmm0,%xmm1
+    646c30cb:	movsd  0x5f7d(%rip),%xmm0        # 646c9050 <.rdata>
+    646c30d3:	mulsd  %xmm1,%xmm0
+    646c30d7:	mov    0x28(%rbp),%rax
+    646c30db:	movsd  0x10(%rax),%xmm2
+    646c30e0:	mov    0x28(%rbp),%rax
+    646c30e4:	movsd  0x10(%rax),%xmm1
+    646c30e9:	mulsd  %xmm2,%xmm1
+    646c30ed:	divsd  %xmm1,%xmm0
+    646c30f1:	call   646c6bb0 <exp>
+    646c30f6:	movapd %xmm0,%xmm1
+    646c30fa:	movsd  0x5f56(%rip),%xmm0        # 646c9058 <.rdata+0x8>
+    646c3102:	subsd  %xmm1,%xmm0
+    646c3106:	movsd  %xmm0,-0x18(%rbp)
+    646c310b:	mov    0x28(%rbp),%rax
+    646c310f:	movsd  0x18(%rax),%xmm0
+    646c3114:	movsd  -0x10(%rbp),%xmm1
+    646c3119:	mulsd  -0x18(%rbp),%xmm1
+    646c311e:	subsd  %xmm1,%xmm0
+    646c3122:	movapd %xmm0,%xmm1
+    646c3126:	mov    0x28(%rbp),%rax
+    646c312a:	movsd  0x20(%rax),%xmm0
+    646c312f:	mov    0x20(%rbp),%eax
+    646c3132:	imul   -0x4(%rbp),%eax
+    646c3136:	mov    -0x8(%rbp),%edx
+    646c3139:	add    %edx,%eax
+    646c313b:	cltq
+    646c313d:	lea    0x0(,%rax,8),%rdx
+    646c3145:	mov    0x18(%rbp),%rax
+    646c3149:	add    %rdx,%rax
+    646c314c:	addsd  %xmm1,%xmm0
+    646c3150:	movsd  %xmm0,(%rax)
+    646c3154:	addl   $0x1,-0x8(%rbp)
+    646c3158:	mov    -0x8(%rbp),%eax
+    646c315b:	cmp    0x20(%rbp),%eax
+    646c315e:	jl     646c3079 <cov_model2d+0x4b>
+    646c3164:	addl   $0x1,-0x4(%rbp)
+    646c3168:	mov    -0x4(%rbp),%eax
+    646c316b:	cmp    0x20(%rbp),%eax
+    646c316e:	jl     646c306d <cov_model2d+0x3f>
+    646c3174:	nop
+    646c3175:	add    $0x40,%rsp
+    646c3179:	pop    %rbp
+    646c317a:	ret
+    646c317b:	nop
+    646c317c:	nop
+    646c317d:	nop
+    646c317e:	nop
+    646c317f:	nop
+
+00000000646c3180 <sampling_state_init>:
+    646c3180:	push   %rbp
+    646c3181:	mov    %rsp,%rbp
+    646c3184:	sub    $0x20,%rsp
+    646c3188:	mov    %rcx,0x10(%rbp)
+    646c318c:	mov    %edx,0x18(%rbp)
+    646c318f:	mov    0x10(%rbp),%rax
+    646c3193:	movl   $0x0,(%rax)
+    646c3199:	mov    0x10(%rbp),%rax
+    646c319d:	movl   $0x0,0x4(%rax)
+    646c31a4:	mov    0x10(%rbp),%rax
+    646c31a8:	movl   $0x0,0x8(%rax)
+    646c31af:	mov    0x10(%rbp),%rax
+    646c31b3:	pxor   %xmm0,%xmm0
+    646c31b7:	movsd  %xmm0,0x10(%rax)
+    646c31bc:	mov    0x18(%rbp),%eax
+    646c31bf:	cltq
+    646c31c1:	mov    0x10(%rbp),%rdx
+    646c31c5:	mov    %rax,0x20(%rdx)
+    646c31c9:	mov    0x18(%rbp),%eax
+    646c31cc:	cltq
+    646c31ce:	mov    0x10(%rbp),%rdx
+    646c31d2:	mov    %rax,0x28(%rdx)
+    646c31d6:	mov    0x18(%rbp),%eax
+    646c31d9:	cltq
+    646c31db:	mov    $0x8,%edx
+    646c31e0:	mov    %rax,%rcx
+    646c31e3:	call   646c79b0 <calloc>
+    646c31e8:	mov    %rax,%rdx
+    646c31eb:	mov    0x10(%rbp),%rax
+    646c31ef:	mov    %rdx,0x18(%rax)
+    646c31f3:	mov    0x18(%rbp),%eax
+    646c31f6:	cltq
+    646c31f8:	mov    0x10(%rbp),%rdx
+    646c31fc:	mov    %rax,0x38(%rdx)
+    646c3200:	mov    0x18(%rbp),%eax
+    646c3203:	cltq
+    646c3205:	mov    0x10(%rbp),%rdx
+    646c3209:	mov    %rax,0x40(%rdx)
+    646c320d:	mov    0x18(%rbp),%eax
+    646c3210:	cltq
+    646c3212:	mov    $0x8,%edx
+    646c3217:	mov    %rax,%rcx
+    646c321a:	call   646c79b0 <calloc>
+    646c321f:	mov    %rax,%rdx
+    646c3222:	mov    0x10(%rbp),%rax
+    646c3226:	mov    %rdx,0x30(%rax)
+    646c322a:	nop
+    646c322b:	add    $0x20,%rsp
+    646c322f:	pop    %rbp
+    646c3230:	ret
+
+00000000646c3231 <sampling_state_update>:
+    646c3231:	push   %rbp
+    646c3232:	mov    %rsp,%rbp
+    646c3235:	mov    %rcx,0x10(%rbp)
+    646c3239:	movsd  %xmm1,0x18(%rbp)
+    646c323e:	mov    %r8d,0x20(%rbp)
+    646c3242:	mov    0x10(%rbp),%rax
+    646c3246:	movsd  0x18(%rbp),%xmm0
+    646c324b:	movsd  %xmm0,0x10(%rax)
+    646c3250:	mov    0x10(%rbp),%rax
+    646c3254:	mov    0x20(%rbp),%edx
+    646c3257:	mov    %edx,0x8(%rax)
+    646c325a:	nop
+    646c325b:	pop    %rbp
+    646c325c:	ret
+
+00000000646c325d <krige_param_setting>:
+    646c325d:	push   %rbp
+    646c325e:	push   %rbx
+    646c325f:	sub    $0x38,%rsp
+    646c3263:	lea    0x80(%rsp),%rbp
+    646c326b:	mov    %ecx,-0x30(%rbp)
+    646c326e:	mov    %rdx,-0x28(%rbp)
+    646c3272:	mov    -0x28(%rbp),%rax
+    646c3276:	mov    %rax,0x8da3(%rip)        # 646cc020 <model>
+    646c327d:	mov    -0x28(%rbp),%rax
+    646c3281:	movsd  0x10(%rax),%xmm0
+    646c3286:	movsd  %xmm0,0x8d9a(%rip)        # 646cc028 <k_range>
+    646c328e:	movq   $0xa,0x8dbf(%rip)        # 646cc058 <location+0x8>
+    646c3299:	movq   $0xa,0x8dbc(%rip)        # 646cc060 <location+0x10>
+    646c32a4:	mov    $0x8,%edx
+    646c32a9:	mov    $0xa,%ecx
+    646c32ae:	call   646c79b0 <calloc>
+    646c32b3:	mov    %rax,0x8d96(%rip)        # 646cc050 <location>
+    646c32ba:	movq   $0xa,0x8db3(%rip)        # 646cc078 <loc_cov+0x8>
+    646c32c5:	movq   $0xa,0x8db0(%rip)        # 646cc080 <loc_cov+0x10>
+    646c32d0:	mov    $0x8,%edx
+    646c32d5:	mov    $0xa,%ecx
+    646c32da:	call   646c79b0 <calloc>
+    646c32df:	mov    %rax,0x8d8a(%rip)        # 646cc070 <loc_cov>
+    646c32e6:	movq   $0xa,0x8dc7(%rip)        # 646cc0b8 <loc_cov2+0x8>
+    646c32f1:	movq   $0xa,0x8dc4(%rip)        # 646cc0c0 <loc_cov2+0x10>
+    646c32fc:	mov    $0x8,%edx
+    646c3301:	mov    $0xa,%ecx
+    646c3306:	call   646c79b0 <calloc>
+    646c330b:	mov    %rax,0x8d9e(%rip)        # 646cc0b0 <loc_cov2>
+    646c3312:	movq   $0xa,0x8ddb(%rip)        # 646cc0f8 <weights+0x8>
+    646c331d:	movq   $0xa,0x8dd8(%rip)        # 646cc100 <weights+0x10>
+    646c3328:	mov    $0x8,%edx
+    646c332d:	mov    $0xa,%ecx
+    646c3332:	call   646c79b0 <calloc>
+    646c3337:	mov    %rax,0x8db2(%rip)        # 646cc0f0 <weights>
+    646c333e:	movq   $0x64,0x8d8f(%rip)        # 646cc0d8 <flatten_temp+0x8>
+    646c3349:	movq   $0x64,0x8d8c(%rip)        # 646cc0e0 <flatten_temp+0x10>
+    646c3354:	mov    $0x8,%edx
+    646c3359:	mov    $0x64,%ecx
+    646c335e:	call   646c79b0 <calloc>
+    646c3363:	mov    %rax,0x8d66(%rip)        # 646cc0d0 <flatten_temp>
+    646c336a:	movq   $0xa,0x8d23(%rip)        # 646cc098 <data_temp+0x8>
+    646c3375:	movq   $0xa,0x8d20(%rip)        # 646cc0a0 <data_temp+0x10>
+    646c3380:	mov    $0x8,%edx
+    646c3385:	mov    $0xa,%ecx
+    646c338a:	call   646c79b0 <calloc>
+    646c338f:	mov    %rax,0x8cfa(%rip)        # 646cc090 <data_temp>
+    646c3396:	movq   $0xa,0x8d97(%rip)        # 646cc138 <pdist_temp+0x8>
+    646c33a1:	movq   $0xa,0x8d94(%rip)        # 646cc140 <pdist_temp+0x10>
+    646c33ac:	mov    $0x50,%ecx
+    646c33b1:	call   646c7970 <malloc>
+    646c33b6:	mov    %rax,0x8d73(%rip)        # 646cc130 <pdist_temp>
+    646c33bd:	movl   $0x0,-0x54(%rbp)
+    646c33c4:	jmp    646c33eb <krige_param_setting+0x18e>
+    646c33c6:	mov    0x8d63(%rip),%rdx        # 646cc130 <pdist_temp>
+    646c33cd:	mov    -0x54(%rbp),%eax
+    646c33d0:	cltq
+    646c33d2:	shl    $0x3,%rax
+    646c33d6:	lea    (%rdx,%rax,1),%rbx
+    646c33da:	mov    $0x50,%ecx
+    646c33df:	call   646c7970 <malloc>
+    646c33e4:	mov    %rax,(%rbx)
+    646c33e7:	addl   $0x1,-0x54(%rbp)
+    646c33eb:	cmpl   $0x9,-0x54(%rbp)
+    646c33ef:	jle    646c33c6 <krige_param_setting+0x169>
+    646c33f1:	movq   $0xa,0x8d5c(%rip)        # 646cc158 <datacov+0x8>
+    646c33fc:	movq   $0xa,0x8d59(%rip)        # 646cc160 <datacov+0x10>
+    646c3407:	mov    $0x50,%ecx
+    646c340c:	call   646c7970 <malloc>
+    646c3411:	mov    %rax,0x8d38(%rip)        # 646cc150 <datacov>
+    646c3418:	movl   $0x0,-0x58(%rbp)
+    646c341f:	jmp    646c3446 <krige_param_setting+0x1e9>
+    646c3421:	mov    0x8d28(%rip),%rdx        # 646cc150 <datacov>
+    646c3428:	mov    -0x58(%rbp),%eax
+    646c342b:	cltq
+    646c342d:	shl    $0x3,%rax
+    646c3431:	lea    (%rdx,%rax,1),%rbx
+    646c3435:	mov    $0x50,%ecx
+    646c343a:	call   646c7970 <malloc>
+    646c343f:	mov    %rax,(%rbx)
+    646c3442:	addl   $0x1,-0x58(%rbp)
+    646c3446:	cmpl   $0x9,-0x58(%rbp)
+    646c344a:	jle    646c3421 <krige_param_setting+0x1c4>
+    646c344c:	mov    -0x30(%rbp),%eax
+    646c344f:	cltq
+    646c3451:	mov    %rax,0x8cc0(%rip)        # 646cc118 <array2d_temp+0x8>
+    646c3458:	movq   $0x3,0x8cbd(%rip)        # 646cc120 <array2d_temp+0x10>
+    646c3463:	mov    -0x30(%rbp),%eax
     646c3466:	cltq
     646c3468:	shl    $0x3,%rax
-    646c346c:	add    %rax,%rdx
-    646c346f:	mov    0x8c9a(%rip),%rcx        # 646cc110 <array2d_temp>
-    646c3476:	mov    -0x14(%rbp),%eax
-    646c3479:	cltq
-    646c347b:	shl    $0x3,%rax
-    646c347f:	add    %rcx,%rax
-    646c3482:	mov    (%rax),%rax
-    646c3485:	movsd  (%rdx),%xmm0
-    646c3489:	movsd  %xmm0,(%rax)
-    646c348d:	mov    0x18(%rbp),%rax
-    646c3491:	mov    0x18(%rax),%rdx
-    646c3495:	mov    -0x14(%rbp),%eax
-    646c3498:	cltq
-    646c349a:	shl    $0x3,%rax
-    646c349e:	add    %rdx,%rax
-    646c34a1:	movsd  (%rax),%xmm0
-    646c34a5:	cvttsd2si %xmm0,%eax
-    646c34a9:	cltq
-    646c34ab:	lea    0x0(,%rax,8),%rdx
-    646c34b3:	mov    0x10(%rbp),%rax
-    646c34b7:	add    %rax,%rdx
-    646c34ba:	mov    0x8c4f(%rip),%rcx        # 646cc110 <array2d_temp>
-    646c34c1:	mov    -0x14(%rbp),%eax
-    646c34c4:	cltq
-    646c34c6:	shl    $0x3,%rax
-    646c34ca:	add    %rcx,%rax
-    646c34cd:	mov    (%rax),%rax
-    646c34d0:	add    $0x8,%rax
-    646c34d4:	movsd  (%rdx),%xmm0
-    646c34d8:	movsd  %xmm0,(%rax)
-    646c34dc:	mov    0x18(%rbp),%rax
-    646c34e0:	mov    0x30(%rax),%rdx
-    646c34e4:	mov    -0x14(%rbp),%eax
-    646c34e7:	cltq
-    646c34e9:	shl    $0x3,%rax
-    646c34ed:	add    %rax,%rdx
-    646c34f0:	mov    0x8c19(%rip),%rcx        # 646cc110 <array2d_temp>
-    646c34f7:	mov    -0x14(%rbp),%eax
-    646c34fa:	cltq
-    646c34fc:	shl    $0x3,%rax
-    646c3500:	add    %rcx,%rax
-    646c3503:	mov    (%rax),%rax
-    646c3506:	add    $0x10,%rax
-    646c350a:	movsd  (%rdx),%xmm0
-    646c350e:	movsd  %xmm0,(%rax)
-    646c3512:	addl   $0x1,-0x14(%rbp)
-    646c3516:	mov    0x18(%rbp),%rax
-    646c351a:	mov    0x4(%rax),%eax
-    646c351d:	cmp    %eax,-0x14(%rbp)
-    646c3520:	jl     646c345b <simple_kriging+0x48>
-    646c3526:	mov    0x18(%rbp),%rax
-    646c352a:	mov    (%rax),%eax
-    646c352c:	cmp    $0x1,%eax
-    646c352f:	jle    646c3552 <simple_kriging+0x13f>
-    646c3531:	mov    0x18(%rbp),%rax
-    646c3535:	mov    0x4(%rax),%eax
-    646c3538:	lea    -0x1(%rax),%edx
-    646c353b:	mov    0x8bce(%rip),%rax        # 646cc110 <array2d_temp>
-    646c3542:	mov    %edx,%r8d
-    646c3545:	mov    $0x0,%edx
-    646c354a:	mov    %rax,%rcx
-    646c354d:	call   646c5021 <quicksort2d>
-    646c3552:	movl   $0x0,-0x18(%rbp)
-    646c3559:	jmp    646c35c2 <simple_kriging+0x1af>
-    646c355b:	mov    0x8bae(%rip),%rdx        # 646cc110 <array2d_temp>
-    646c3562:	mov    -0x18(%rbp),%eax
-    646c3565:	cltq
-    646c3567:	shl    $0x3,%rax
-    646c356b:	add    %rdx,%rax
-    646c356e:	mov    (%rax),%rdx
-    646c3571:	mov    0x8ad8(%rip),%rcx        # 646cc050 <location>
-    646c3578:	mov    -0x18(%rbp),%eax
-    646c357b:	cltq
-    646c357d:	shl    $0x3,%rax
-    646c3581:	add    %rcx,%rax
-    646c3584:	movsd  (%rdx),%xmm0
-    646c3588:	movsd  %xmm0,(%rax)
-    646c358c:	mov    0x8b7d(%rip),%rdx        # 646cc110 <array2d_temp>
-    646c3593:	mov    -0x18(%rbp),%eax
-    646c3596:	cltq
-    646c3598:	shl    $0x3,%rax
-    646c359c:	add    %rdx,%rax
-    646c359f:	mov    (%rax),%rdx
-    646c35a2:	mov    0x8b07(%rip),%rcx        # 646cc0b0 <loc_cov2>
-    646c35a9:	mov    -0x18(%rbp),%eax
-    646c35ac:	cltq
-    646c35ae:	shl    $0x3,%rax
-    646c35b2:	add    %rcx,%rax
-    646c35b5:	movsd  0x10(%rdx),%xmm0
-    646c35ba:	movsd  %xmm0,(%rax)
-    646c35be:	addl   $0x1,-0x18(%rbp)
-    646c35c2:	mov    0x18(%rbp),%rax
-    646c35c6:	mov    (%rax),%eax
-    646c35c8:	cmp    %eax,-0x18(%rbp)
-    646c35cb:	jl     646c355b <simple_kriging+0x148>
-    646c35cd:	mov    0x18(%rbp),%rax
-    646c35d1:	mov    (%rax),%ecx
-    646c35d3:	mov    0x8b56(%rip),%rdx        # 646cc130 <pdist_temp>
-    646c35da:	mov    0x8a6f(%rip),%rax        # 646cc050 <location>
-    646c35e1:	mov    %ecx,%r8d
-    646c35e4:	mov    %rax,%rcx
-    646c35e7:	call   646c433d <pdist>
-    646c35ec:	movsd  0x8a34(%rip),%xmm0        # 646cc028 <sill>
-    646c35f4:	movsd  0x8a24(%rip),%xmm1        # 646cc020 <range>
-    646c35fc:	mov    0x18(%rbp),%rax
-    646c3600:	mov    (%rax),%ecx
-    646c3602:	mov    0x8ac7(%rip),%rdx        # 646cc0d0 <flatten_temp>
-    646c3609:	mov    0x8b20(%rip),%rax        # 646cc130 <pdist_temp>
-    646c3610:	movsd  %xmm0,0x20(%rsp)
-    646c3616:	movapd %xmm1,%xmm3
-    646c361a:	mov    %ecx,%r8d
-    646c361d:	mov    %rax,%rcx
-    646c3620:	call   646c2fcf <cov_model2d>
-    646c3625:	mov    0x18(%rbp),%rax
-    646c3629:	mov    (%rax),%ecx
-    646c362b:	mov    0x8b1e(%rip),%rdx        # 646cc150 <datacov>
-    646c3632:	mov    0x8a97(%rip),%rax        # 646cc0d0 <flatten_temp>
-    646c3639:	mov    %ecx,%r8d
-    646c363c:	mov    %rax,%rcx
-    646c363f:	call   646c43f0 <matrixform>
-    646c3644:	movsd  0x89dc(%rip),%xmm0        # 646cc028 <sill>
-    646c364c:	movsd  0x89cc(%rip),%xmm1        # 646cc020 <range>
-    646c3654:	mov    0x18(%rbp),%rax
-    646c3658:	mov    (%rax),%ecx
-    646c365a:	mov    0x8a0f(%rip),%rdx        # 646cc070 <loc_cov>
-    646c3661:	mov    0x8a48(%rip),%rax        # 646cc0b0 <loc_cov2>
-    646c3668:	movsd  %xmm0,0x20(%rsp)
-    646c366e:	movapd %xmm1,%xmm3
-    646c3672:	mov    %ecx,%r8d
-    646c3675:	mov    %rax,%rcx
-    646c3678:	call   646c2f06 <cov_model>
-    646c367d:	mov    0x18(%rbp),%rax
-    646c3681:	mov    (%rax),%eax
-    646c3683:	test   %eax,%eax
-    646c3685:	jle    646c36b1 <simple_kriging+0x29e>
-    646c3687:	mov    0x18(%rbp),%rax
-    646c368b:	mov    (%rax),%r8d
-    646c368e:	mov    0x8a5b(%rip),%rcx        # 646cc0f0 <weights>
-    646c3695:	mov    0x89d4(%rip),%rdx        # 646cc070 <loc_cov>
-    646c369c:	mov    0x8aad(%rip),%rax        # 646cc150 <datacov>
-    646c36a3:	mov    %r8d,%r9d
-    646c36a6:	mov    %rcx,%r8
-    646c36a9:	mov    %rax,%rcx
-    646c36ac:	call   646c3b7a <lu_inverse_solver>
-    646c36b1:	pxor   %xmm0,%xmm0
-    646c36b5:	movsd  %xmm0,0x8973(%rip)        # 646cc030 <estimation>
-    646c36bd:	pxor   %xmm0,%xmm0
-    646c36c1:	movsd  %xmm0,0x896f(%rip)        # 646cc038 <krige_var>
-    646c36c9:	pxor   %xmm0,%xmm0
-    646c36cd:	movsd  %xmm0,0x896b(%rip)        # 646cc040 <fix>
-    646c36d5:	movl   $0x0,-0x1c(%rbp)
-    646c36dc:	jmp    646c3778 <simple_kriging+0x365>
-    646c36e1:	mov    0x8a28(%rip),%rdx        # 646cc110 <array2d_temp>
-    646c36e8:	mov    -0x1c(%rbp),%eax
-    646c36eb:	cltq
-    646c36ed:	shl    $0x3,%rax
-    646c36f1:	add    %rdx,%rax
-    646c36f4:	mov    (%rax),%rax
-    646c36f7:	add    $0x8,%rax
-    646c36fb:	movsd  (%rax),%xmm1
-    646c36ff:	mov    0x89ea(%rip),%rdx        # 646cc0f0 <weights>
-    646c3706:	mov    -0x1c(%rbp),%eax
-    646c3709:	cltq
-    646c370b:	shl    $0x3,%rax
-    646c370f:	add    %rdx,%rax
-    646c3712:	movsd  (%rax),%xmm0
-    646c3716:	mulsd  %xmm0,%xmm1
-    646c371a:	movsd  0x890e(%rip),%xmm0        # 646cc030 <estimation>
-    646c3722:	addsd  %xmm1,%xmm0
-    646c3726:	movsd  %xmm0,0x8902(%rip)        # 646cc030 <estimation>
-    646c372e:	mov    0x893b(%rip),%rdx        # 646cc070 <loc_cov>
-    646c3735:	mov    -0x1c(%rbp),%eax
-    646c3738:	cltq
-    646c373a:	shl    $0x3,%rax
-    646c373e:	add    %rdx,%rax
-    646c3741:	movsd  (%rax),%xmm1
-    646c3745:	mov    0x89a4(%rip),%rdx        # 646cc0f0 <weights>
-    646c374c:	mov    -0x1c(%rbp),%eax
-    646c374f:	cltq
-    646c3751:	shl    $0x3,%rax
-    646c3755:	add    %rdx,%rax
-    646c3758:	movsd  (%rax),%xmm0
-    646c375c:	mulsd  %xmm0,%xmm1
-    646c3760:	movsd  0x88d0(%rip),%xmm0        # 646cc038 <krige_var>
-    646c3768:	addsd  %xmm1,%xmm0
-    646c376c:	movsd  %xmm0,0x88c4(%rip)        # 646cc038 <krige_var>
-    646c3774:	addl   $0x1,-0x1c(%rbp)
-    646c3778:	mov    0x18(%rbp),%rax
-    646c377c:	mov    (%rax),%eax
-    646c377e:	cmp    %eax,-0x1c(%rbp)
-    646c3781:	jl     646c36e1 <simple_kriging+0x2ce>
-    646c3787:	movsd  0x88a9(%rip),%xmm1        # 646cc038 <krige_var>
-    646c378f:	movsd  0x58c9(%rip),%xmm0        # 646c9060 <.rdata>
-    646c3797:	subsd  %xmm1,%xmm0
-    646c379b:	movsd  %xmm0,0x8895(%rip)        # 646cc038 <krige_var>
-    646c37a3:	movsd  0x888d(%rip),%xmm1        # 646cc038 <krige_var>
-    646c37ab:	pxor   %xmm0,%xmm0
-    646c37af:	comisd %xmm1,%xmm0
-    646c37b3:	jbe    646c37c1 <simple_kriging+0x3ae>
-    646c37b5:	pxor   %xmm0,%xmm0
-    646c37b9:	movsd  %xmm0,0x8877(%rip)        # 646cc038 <krige_var>
-    646c37c1:	mov    0x20(%rbp),%rax
-    646c37c5:	mov    %rax,%rcx
-    646c37c8:	call   646c2e27 <mt19937_random_normal>
-    646c37cd:	movapd %xmm0,%xmm6
-    646c37d1:	mov    0x8860(%rip),%rax        # 646cc038 <krige_var>
-    646c37d8:	movsd  0x5888(%rip),%xmm0        # 646c9068 <.rdata+0x8>
-    646c37e0:	movapd %xmm0,%xmm1
-    646c37e4:	movq   %rax,%xmm0
-    646c37e9:	call   646c6ed0 <pow>
-    646c37ee:	mulsd  %xmm6,%xmm0
-    646c37f2:	movsd  %xmm0,0x8846(%rip)        # 646cc040 <fix>
-    646c37fa:	movsd  0x882e(%rip),%xmm1        # 646cc030 <estimation>
-    646c3802:	movsd  0x8836(%rip),%xmm0        # 646cc040 <fix>
-    646c380a:	mov    0x18(%rbp),%rax
-    646c380e:	movsd  0x10(%rax),%xmm2
-    646c3813:	cvttsd2si %xmm2,%eax
-    646c3817:	cltq
-    646c3819:	lea    0x0(,%rax,8),%rdx
-    646c3821:	mov    0x10(%rbp),%rax
-    646c3825:	add    %rdx,%rax
-    646c3828:	addsd  %xmm1,%xmm0
-    646c382c:	movsd  %xmm0,(%rax)
-    646c3830:	jmp    646c3833 <simple_kriging+0x420>
-    646c3832:	nop
-    646c3833:	movaps -0x10(%rbp),%xmm6
-    646c3837:	add    $0x50,%rsp
-    646c383b:	pop    %rbp
-    646c383c:	ret
-
-00000000646c383d <find_neighbor>:
-    646c383d:	push   %rbp
-    646c383e:	push   %rbx
-    646c383f:	sub    $0x38,%rsp
-    646c3843:	lea    0x80(%rsp),%rbp
-    646c384b:	mov    %rcx,-0x30(%rbp)
-    646c384f:	mov    %rdx,-0x28(%rbp)
-    646c3853:	mov    %r8,-0x20(%rbp)
-    646c3857:	mov    -0x28(%rbp),%rax
-    646c385b:	mov    (%rax),%eax
-    646c385d:	test   %eax,%eax
-    646c385f:	jne    646c38c3 <find_neighbor+0x86>
-    646c3861:	mov    -0x28(%rbp),%rax
-    646c3865:	movsd  0x10(%rax),%xmm0
-    646c386a:	cvttsd2si %xmm0,%eax
-    646c386e:	cltq
-    646c3870:	lea    0x0(,%rax,8),%rdx
-    646c3878:	mov    -0x30(%rbp),%rax
-    646c387c:	lea    (%rdx,%rax,1),%rbx
-    646c3880:	mov    -0x20(%rbp),%rax
-    646c3884:	mov    %rax,%rcx
-    646c3887:	call   646c2e27 <mt19937_random_normal>
-    646c388c:	movq   %xmm0,%rax
-    646c3891:	mov    %rax,(%rbx)
-    646c3894:	mov    -0x28(%rbp),%rax
-    646c3898:	mov    0x18(%rax),%rdx
-    646c389c:	mov    -0x28(%rbp),%rax
-    646c38a0:	mov    0x8(%rax),%eax
-    646c38a3:	cltq
-    646c38a5:	shl    $0x3,%rax
-    646c38a9:	add    %rdx,%rax
-    646c38ac:	mov    -0x28(%rbp),%rdx
-    646c38b0:	movsd  0x10(%rdx),%xmm0
-    646c38b5:	movsd  %xmm0,(%rax)
-    646c38b9:	mov    $0x0,%eax
-    646c38be:	jmp    646c39d3 <find_neighbor+0x196>
-    646c38c3:	movl   $0x0,-0x54(%rbp)
-    646c38ca:	movl   $0x0,-0x58(%rbp)
-    646c38d1:	jmp    646c3959 <find_neighbor+0x11c>
-    646c38d6:	mov    -0x28(%rbp),%rax
-    646c38da:	mov    0x18(%rax),%rdx
-    646c38de:	mov    -0x58(%rbp),%eax
-    646c38e1:	cltq
-    646c38e3:	shl    $0x3,%rax
-    646c38e7:	add    %rdx,%rax
-    646c38ea:	movsd  (%rax),%xmm0
-    646c38ee:	mov    -0x28(%rbp),%rax
-    646c38f2:	movsd  0x10(%rax),%xmm1
-    646c38f7:	subsd  %xmm1,%xmm0
-    646c38fb:	mov    -0x28(%rbp),%rax
-    646c38ff:	mov    0x30(%rax),%rdx
-    646c3903:	mov    -0x58(%rbp),%eax
-    646c3906:	cltq
-    646c3908:	shl    $0x3,%rax
-    646c390c:	add    %rdx,%rax
-    646c390f:	movq   0x5759(%rip),%xmm1        # 646c9070 <.rdata+0x10>
-    646c3917:	andpd  %xmm1,%xmm0
-    646c391b:	movsd  %xmm0,(%rax)
-    646c391f:	mov    -0x28(%rbp),%rax
-    646c3923:	mov    0x30(%rax),%rdx
-    646c3927:	mov    -0x58(%rbp),%eax
-    646c392a:	cltq
-    646c392c:	shl    $0x3,%rax
-    646c3930:	add    %rdx,%rax
-    646c3933:	movsd  (%rax),%xmm1
-    646c3937:	movsd  0x86e1(%rip),%xmm2        # 646cc020 <range>
-    646c393f:	movsd  0x5739(%rip),%xmm0        # 646c9080 <.rdata+0x20>
-    646c3947:	mulsd  %xmm2,%xmm0
-    646c394b:	comisd %xmm1,%xmm0
-    646c394f:	jbe    646c3955 <find_neighbor+0x118>
-    646c3951:	addl   $0x1,-0x54(%rbp)
-    646c3955:	addl   $0x1,-0x58(%rbp)
-    646c3959:	mov    -0x28(%rbp),%rax
-    646c395d:	mov    0x4(%rax),%eax
-    646c3960:	cmp    %eax,-0x58(%rbp)
-    646c3963:	jl     646c38d6 <find_neighbor+0x99>
-    646c3969:	cmpl   $0x0,-0x54(%rbp)
-    646c396d:	jne    646c39ce <find_neighbor+0x191>
-    646c396f:	mov    -0x28(%rbp),%rax
-    646c3973:	movsd  0x10(%rax),%xmm0
-    646c3978:	cvttsd2si %xmm0,%eax
-    646c397c:	cltq
-    646c397e:	lea    0x0(,%rax,8),%rdx
-    646c3986:	mov    -0x30(%rbp),%rax
-    646c398a:	lea    (%rdx,%rax,1),%rbx
-    646c398e:	mov    -0x20(%rbp),%rax
-    646c3992:	mov    %rax,%rcx
-    646c3995:	call   646c2e27 <mt19937_random_normal>
-    646c399a:	movq   %xmm0,%rax
-    646c399f:	mov    %rax,(%rbx)
-    646c39a2:	mov    -0x28(%rbp),%rax
-    646c39a6:	mov    0x18(%rax),%rdx
-    646c39aa:	mov    -0x28(%rbp),%rax
-    646c39ae:	mov    0x8(%rax),%eax
-    646c39b1:	cltq
-    646c39b3:	shl    $0x3,%rax
-    646c39b7:	add    %rdx,%rax
-    646c39ba:	mov    -0x28(%rbp),%rdx
-    646c39be:	movsd  0x10(%rdx),%xmm0
-    646c39c3:	movsd  %xmm0,(%rax)
-    646c39c7:	mov    $0x0,%eax
-    646c39cc:	jmp    646c39d3 <find_neighbor+0x196>
-    646c39ce:	mov    $0x1,%eax
-    646c39d3:	add    $0x38,%rsp
-    646c39d7:	pop    %rbx
-    646c39d8:	pop    %rbp
-    646c39d9:	ret
-
-00000000646c39da <krige_memory_free>:
-    646c39da:	push   %rbp
-    646c39db:	mov    %rsp,%rbp
-    646c39de:	sub    $0x30,%rsp
-    646c39e2:	mov    0x8667(%rip),%rax        # 646cc050 <location>
-    646c39e9:	mov    %rax,%rcx
-    646c39ec:	call   646c78f8 <free>
-    646c39f1:	mov    0x8678(%rip),%rax        # 646cc070 <loc_cov>
-    646c39f8:	mov    %rax,%rcx
-    646c39fb:	call   646c78f8 <free>
-    646c3a00:	mov    0x8689(%rip),%rax        # 646cc090 <data_temp>
-    646c3a07:	mov    %rax,%rcx
-    646c3a0a:	call   646c78f8 <free>
-    646c3a0f:	mov    0x869a(%rip),%rax        # 646cc0b0 <loc_cov2>
-    646c3a16:	mov    %rax,%rcx
-    646c3a19:	call   646c78f8 <free>
-    646c3a1e:	mov    0x86ab(%rip),%rax        # 646cc0d0 <flatten_temp>
-    646c3a25:	mov    %rax,%rcx
-    646c3a28:	call   646c78f8 <free>
-    646c3a2d:	mov    0x86bc(%rip),%rax        # 646cc0f0 <weights>
-    646c3a34:	mov    %rax,%rcx
-    646c3a37:	call   646c78f8 <free>
-    646c3a3c:	movl   $0x0,-0x4(%rbp)
-    646c3a43:	jmp    646c3a67 <krige_memory_free+0x8d>
-    646c3a45:	mov    0x86c4(%rip),%rdx        # 646cc110 <array2d_temp>
-    646c3a4c:	mov    -0x4(%rbp),%eax
-    646c3a4f:	cltq
-    646c3a51:	shl    $0x3,%rax
-    646c3a55:	add    %rdx,%rax
-    646c3a58:	mov    (%rax),%rax
-    646c3a5b:	mov    %rax,%rcx
-    646c3a5e:	call   646c78f8 <free>
-    646c3a63:	addl   $0x1,-0x4(%rbp)
-    646c3a67:	mov    -0x4(%rbp),%eax
-    646c3a6a:	cltq
-    646c3a6c:	mov    0x86a5(%rip),%rdx        # 646cc118 <array2d_temp+0x8>
-    646c3a73:	cmp    %rdx,%rax
-    646c3a76:	jb     646c3a45 <krige_memory_free+0x6b>
-    646c3a78:	mov    0x8691(%rip),%rax        # 646cc110 <array2d_temp>
-    646c3a7f:	mov    %rax,%rcx
-    646c3a82:	call   646c78f8 <free>
-    646c3a87:	movl   $0x0,-0x8(%rbp)
-    646c3a8e:	jmp    646c3ab2 <krige_memory_free+0xd8>
-    646c3a90:	mov    0x8699(%rip),%rdx        # 646cc130 <pdist_temp>
-    646c3a97:	mov    -0x8(%rbp),%eax
-    646c3a9a:	cltq
-    646c3a9c:	shl    $0x3,%rax
-    646c3aa0:	add    %rdx,%rax
-    646c3aa3:	mov    (%rax),%rax
-    646c3aa6:	mov    %rax,%rcx
-    646c3aa9:	call   646c78f8 <free>
-    646c3aae:	addl   $0x1,-0x8(%rbp)
-    646c3ab2:	mov    -0x8(%rbp),%eax
-    646c3ab5:	cltq
-    646c3ab7:	mov    0x867a(%rip),%rdx        # 646cc138 <pdist_temp+0x8>
-    646c3abe:	cmp    %rdx,%rax
-    646c3ac1:	jb     646c3a90 <krige_memory_free+0xb6>
-    646c3ac3:	mov    0x8666(%rip),%rax        # 646cc130 <pdist_temp>
-    646c3aca:	mov    %rax,%rcx
-    646c3acd:	call   646c78f8 <free>
-    646c3ad2:	movl   $0x0,-0xc(%rbp)
-    646c3ad9:	jmp    646c3afd <krige_memory_free+0x123>
-    646c3adb:	mov    0x866e(%rip),%rdx        # 646cc150 <datacov>
-    646c3ae2:	mov    -0xc(%rbp),%eax
-    646c3ae5:	cltq
-    646c3ae7:	shl    $0x3,%rax
-    646c3aeb:	add    %rdx,%rax
-    646c3aee:	mov    (%rax),%rax
-    646c3af1:	mov    %rax,%rcx
-    646c3af4:	call   646c78f8 <free>
-    646c3af9:	addl   $0x1,-0xc(%rbp)
-    646c3afd:	mov    -0xc(%rbp),%eax
-    646c3b00:	cltq
-    646c3b02:	mov    0x864f(%rip),%rdx        # 646cc158 <datacov+0x8>
-    646c3b09:	cmp    %rdx,%rax
-    646c3b0c:	jb     646c3adb <krige_memory_free+0x101>
-    646c3b0e:	mov    0x863b(%rip),%rax        # 646cc150 <datacov>
-    646c3b15:	mov    %rax,%rcx
-    646c3b18:	call   646c78f8 <free>
-    646c3b1d:	nop
-    646c3b1e:	add    $0x30,%rsp
-    646c3b22:	pop    %rbp
-    646c3b23:	ret
-    646c3b24:	nop
-    646c3b25:	nop
-    646c3b26:	nop
-    646c3b27:	nop
-    646c3b28:	nop
-    646c3b29:	nop
-    646c3b2a:	nop
-    646c3b2b:	nop
-    646c3b2c:	nop
-    646c3b2d:	nop
-    646c3b2e:	nop
-    646c3b2f:	nop
-
-00000000646c3b30 <snprintf>:
-    646c3b30:	push   %rbp
-    646c3b31:	mov    %rsp,%rbp
-    646c3b34:	sub    $0x30,%rsp
-    646c3b38:	mov    %rcx,0x10(%rbp)
-    646c3b3c:	mov    %rdx,0x18(%rbp)
-    646c3b40:	mov    %r8,0x20(%rbp)
-    646c3b44:	mov    %r9,0x28(%rbp)
-    646c3b48:	lea    0x28(%rbp),%rax
-    646c3b4c:	mov    %rax,-0x10(%rbp)
-    646c3b50:	mov    -0x10(%rbp),%rcx
-    646c3b54:	mov    0x20(%rbp),%rdx
-    646c3b58:	mov    0x18(%rbp),%rax
-    646c3b5c:	mov    %rcx,%r9
-    646c3b5f:	mov    %rdx,%r8
-    646c3b62:	mov    %rax,%rdx
-    646c3b65:	mov    0x10(%rbp),%rcx
-    646c3b69:	call   646c6900 <__ms_vsnprintf>
-    646c3b6e:	mov    %eax,-0x4(%rbp)
-    646c3b71:	mov    -0x4(%rbp),%eax
-    646c3b74:	add    $0x30,%rsp
-    646c3b78:	pop    %rbp
-    646c3b79:	ret
-
-00000000646c3b7a <lu_inverse_solver>:
-    646c3b7a:	push   %rbp
-    646c3b7b:	push   %rbx
-    646c3b7c:	sub    $0xd8,%rsp
-    646c3b83:	lea    0x80(%rsp),%rbp
-    646c3b8b:	mov    %rcx,0x70(%rbp)
-    646c3b8f:	mov    %rdx,0x78(%rbp)
-    646c3b93:	mov    %r8,0x80(%rbp)
-    646c3b9a:	mov    %r9d,0x88(%rbp)
-    646c3ba1:	movq   $0xa,0x18(%rbp)
-    646c3ba9:	movq   $0xa,0x20(%rbp)
-    646c3bb1:	mov    $0x50,%ecx
-    646c3bb6:	call   646c78e0 <malloc>
-    646c3bbb:	mov    %rax,0x10(%rbp)
-    646c3bbf:	movl   $0x0,0x4c(%rbp)
-    646c3bc6:	jmp    646c3bea <lu_inverse_solver+0x70>
-    646c3bc8:	mov    0x10(%rbp),%rdx
-    646c3bcc:	mov    0x4c(%rbp),%eax
-    646c3bcf:	cltq
-    646c3bd1:	shl    $0x3,%rax
-    646c3bd5:	lea    (%rdx,%rax,1),%rbx
-    646c3bd9:	mov    $0x50,%ecx
-    646c3bde:	call   646c78e0 <malloc>
-    646c3be3:	mov    %rax,(%rbx)
-    646c3be6:	addl   $0x1,0x4c(%rbp)
-    646c3bea:	cmpl   $0x9,0x4c(%rbp)
-    646c3bee:	jle    646c3bc8 <lu_inverse_solver+0x4e>
-    646c3bf0:	movq   $0xa,-0x8(%rbp)
-    646c3bf8:	movq   $0xa,0x0(%rbp)
-    646c3c00:	mov    $0x50,%ecx
-    646c3c05:	call   646c78e0 <malloc>
-    646c3c0a:	mov    %rax,-0x10(%rbp)
-    646c3c0e:	movl   $0x0,0x48(%rbp)
-    646c3c15:	jmp    646c3c39 <lu_inverse_solver+0xbf>
-    646c3c17:	mov    -0x10(%rbp),%rdx
-    646c3c1b:	mov    0x48(%rbp),%eax
-    646c3c1e:	cltq
-    646c3c20:	shl    $0x3,%rax
-    646c3c24:	lea    (%rdx,%rax,1),%rbx
-    646c3c28:	mov    $0x50,%ecx
-    646c3c2d:	call   646c78e0 <malloc>
-    646c3c32:	mov    %rax,(%rbx)
-    646c3c35:	addl   $0x1,0x48(%rbp)
-    646c3c39:	cmpl   $0x9,0x48(%rbp)
-    646c3c3d:	jle    646c3c17 <lu_inverse_solver+0x9d>
-    646c3c3f:	mov    -0x10(%rbp),%rdx
-    646c3c43:	mov    0x10(%rbp),%rax
-    646c3c47:	mov    0x88(%rbp),%ecx
-    646c3c4d:	mov    %ecx,%r9d
-    646c3c50:	mov    %rdx,%r8
-    646c3c53:	mov    %rax,%rdx
-    646c3c56:	mov    0x70(%rbp),%rcx
-    646c3c5a:	call   646c3ef8 <lu_decomposition>
-    646c3c5f:	mov    0x78(%rbp),%rax
-    646c3c63:	movsd  (%rax),%xmm0
-    646c3c67:	mov    0x10(%rbp),%rax
-    646c3c6b:	mov    (%rax),%rax
-    646c3c6e:	movsd  (%rax),%xmm1
-    646c3c72:	divsd  %xmm1,%xmm0
-    646c3c76:	movsd  %xmm0,-0x60(%rbp)
-    646c3c7b:	movl   $0x1,0x44(%rbp)
-    646c3c82:	jmp    646c3d4c <lu_inverse_solver+0x1d2>
-    646c3c87:	mov    0x44(%rbp),%eax
-    646c3c8a:	cltq
-    646c3c8c:	lea    0x0(,%rax,8),%rdx
-    646c3c94:	mov    0x78(%rbp),%rax
-    646c3c98:	add    %rdx,%rax
-    646c3c9b:	movsd  (%rax),%xmm0
-    646c3c9f:	mov    0x44(%rbp),%eax
-    646c3ca2:	cltq
-    646c3ca4:	movsd  %xmm0,-0x60(%rbp,%rax,8)
-    646c3caa:	movl   $0x0,0x40(%rbp)
-    646c3cb1:	jmp    646c3d03 <lu_inverse_solver+0x189>
-    646c3cb3:	mov    0x44(%rbp),%eax
-    646c3cb6:	cltq
-    646c3cb8:	movsd  -0x60(%rbp,%rax,8),%xmm0
-    646c3cbe:	mov    0x10(%rbp),%rdx
-    646c3cc2:	mov    0x44(%rbp),%eax
-    646c3cc5:	cltq
-    646c3cc7:	shl    $0x3,%rax
-    646c3ccb:	add    %rdx,%rax
-    646c3cce:	mov    (%rax),%rdx
-    646c3cd1:	mov    0x40(%rbp),%eax
-    646c3cd4:	cltq
-    646c3cd6:	shl    $0x3,%rax
-    646c3cda:	add    %rdx,%rax
-    646c3cdd:	movsd  (%rax),%xmm2
-    646c3ce1:	mov    0x40(%rbp),%eax
-    646c3ce4:	cltq
-    646c3ce6:	movsd  -0x60(%rbp,%rax,8),%xmm1
-    646c3cec:	mulsd  %xmm2,%xmm1
-    646c3cf0:	subsd  %xmm1,%xmm0
-    646c3cf4:	mov    0x44(%rbp),%eax
-    646c3cf7:	cltq
-    646c3cf9:	movsd  %xmm0,-0x60(%rbp,%rax,8)
-    646c3cff:	addl   $0x1,0x40(%rbp)
-    646c3d03:	mov    0x40(%rbp),%eax
-    646c3d06:	cmp    0x44(%rbp),%eax
-    646c3d09:	jl     646c3cb3 <lu_inverse_solver+0x139>
-    646c3d0b:	mov    0x44(%rbp),%eax
-    646c3d0e:	cltq
-    646c3d10:	movsd  -0x60(%rbp,%rax,8),%xmm0
-    646c3d16:	mov    0x10(%rbp),%rdx
-    646c3d1a:	mov    0x44(%rbp),%eax
-    646c3d1d:	cltq
-    646c3d1f:	shl    $0x3,%rax
-    646c3d23:	add    %rdx,%rax
-    646c3d26:	mov    (%rax),%rdx
-    646c3d29:	mov    0x44(%rbp),%eax
-    646c3d2c:	cltq
-    646c3d2e:	shl    $0x3,%rax
-    646c3d32:	add    %rdx,%rax
-    646c3d35:	movsd  (%rax),%xmm1
-    646c3d39:	divsd  %xmm1,%xmm0
-    646c3d3d:	mov    0x44(%rbp),%eax
-    646c3d40:	cltq
-    646c3d42:	movsd  %xmm0,-0x60(%rbp,%rax,8)
-    646c3d48:	addl   $0x1,0x44(%rbp)
-    646c3d4c:	mov    0x44(%rbp),%eax
-    646c3d4f:	cmp    0x88(%rbp),%eax
-    646c3d55:	jl     646c3c87 <lu_inverse_solver+0x10d>
-    646c3d5b:	mov    0x88(%rbp),%eax
-    646c3d61:	cltq
-    646c3d63:	lea    0x0(,%rax,8),%rdx
-    646c3d6b:	mov    0x80(%rbp),%rax
-    646c3d72:	add    %rax,%rdx
-    646c3d75:	mov    0x88(%rbp),%eax
-    646c3d7b:	cltq
-    646c3d7d:	movsd  -0x60(%rbp,%rax,8),%xmm0
-    646c3d83:	movsd  %xmm0,(%rdx)
-    646c3d87:	mov    0x88(%rbp),%eax
-    646c3d8d:	sub    $0x1,%eax
-    646c3d90:	mov    %eax,0x3c(%rbp)
-    646c3d93:	jmp    646c3e5f <lu_inverse_solver+0x2e5>
-    646c3d98:	mov    0x3c(%rbp),%eax
-    646c3d9b:	cltq
-    646c3d9d:	lea    0x0(,%rax,8),%rdx
-    646c3da5:	mov    0x80(%rbp),%rax
-    646c3dac:	add    %rax,%rdx
-    646c3daf:	mov    0x3c(%rbp),%eax
-    646c3db2:	cltq
-    646c3db4:	movsd  -0x60(%rbp,%rax,8),%xmm0
-    646c3dba:	movsd  %xmm0,(%rdx)
-    646c3dbe:	mov    0x3c(%rbp),%eax
-    646c3dc1:	add    $0x1,%eax
-    646c3dc4:	mov    %eax,0x38(%rbp)
-    646c3dc7:	jmp    646c3e4c <lu_inverse_solver+0x2d2>
-    646c3dcc:	mov    0x3c(%rbp),%eax
-    646c3dcf:	cltq
-    646c3dd1:	lea    0x0(,%rax,8),%rdx
-    646c3dd9:	mov    0x80(%rbp),%rax
-    646c3de0:	add    %rdx,%rax
-    646c3de3:	movsd  (%rax),%xmm0
-    646c3de7:	mov    -0x10(%rbp),%rdx
-    646c3deb:	mov    0x3c(%rbp),%eax
-    646c3dee:	cltq
-    646c3df0:	shl    $0x3,%rax
-    646c3df4:	add    %rdx,%rax
-    646c3df7:	mov    (%rax),%rdx
-    646c3dfa:	mov    0x38(%rbp),%eax
-    646c3dfd:	cltq
-    646c3dff:	shl    $0x3,%rax
-    646c3e03:	add    %rdx,%rax
-    646c3e06:	movsd  (%rax),%xmm2
-    646c3e0a:	mov    0x38(%rbp),%eax
-    646c3e0d:	cltq
-    646c3e0f:	lea    0x0(,%rax,8),%rdx
-    646c3e17:	mov    0x80(%rbp),%rax
-    646c3e1e:	add    %rdx,%rax
-    646c3e21:	movsd  (%rax),%xmm1
-    646c3e25:	mulsd  %xmm2,%xmm1
-    646c3e29:	mov    0x3c(%rbp),%eax
-    646c3e2c:	cltq
-    646c3e2e:	lea    0x0(,%rax,8),%rdx
-    646c3e36:	mov    0x80(%rbp),%rax
-    646c3e3d:	add    %rdx,%rax
-    646c3e40:	subsd  %xmm1,%xmm0
-    646c3e44:	movsd  %xmm0,(%rax)
-    646c3e48:	addl   $0x1,0x38(%rbp)
-    646c3e4c:	mov    0x38(%rbp),%eax
-    646c3e4f:	cmp    0x88(%rbp),%eax
-    646c3e55:	jl     646c3dcc <lu_inverse_solver+0x252>
-    646c3e5b:	subl   $0x1,0x3c(%rbp)
-    646c3e5f:	cmpl   $0x0,0x3c(%rbp)
-    646c3e63:	jns    646c3d98 <lu_inverse_solver+0x21e>
-    646c3e69:	movl   $0x0,0x34(%rbp)
-    646c3e70:	jmp    646c3e91 <lu_inverse_solver+0x317>
-    646c3e72:	mov    0x10(%rbp),%rdx
-    646c3e76:	mov    0x34(%rbp),%eax
-    646c3e79:	cltq
-    646c3e7b:	shl    $0x3,%rax
-    646c3e7f:	add    %rdx,%rax
-    646c3e82:	mov    (%rax),%rax
-    646c3e85:	mov    %rax,%rcx
-    646c3e88:	call   646c78f8 <free>
-    646c3e8d:	addl   $0x1,0x34(%rbp)
-    646c3e91:	mov    0x34(%rbp),%eax
-    646c3e94:	cltq
-    646c3e96:	mov    0x18(%rbp),%rdx
-    646c3e9a:	cmp    %rdx,%rax
-    646c3e9d:	jb     646c3e72 <lu_inverse_solver+0x2f8>
-    646c3e9f:	mov    0x10(%rbp),%rax
-    646c3ea3:	mov    %rax,%rcx
-    646c3ea6:	call   646c78f8 <free>
-    646c3eab:	movl   $0x0,0x30(%rbp)
-    646c3eb2:	jmp    646c3ed3 <lu_inverse_solver+0x359>
-    646c3eb4:	mov    -0x10(%rbp),%rdx
-    646c3eb8:	mov    0x30(%rbp),%eax
-    646c3ebb:	cltq
-    646c3ebd:	shl    $0x3,%rax
-    646c3ec1:	add    %rdx,%rax
-    646c3ec4:	mov    (%rax),%rax
-    646c3ec7:	mov    %rax,%rcx
-    646c3eca:	call   646c78f8 <free>
-    646c3ecf:	addl   $0x1,0x30(%rbp)
-    646c3ed3:	mov    0x30(%rbp),%eax
-    646c3ed6:	cltq
-    646c3ed8:	mov    -0x8(%rbp),%rdx
-    646c3edc:	cmp    %rdx,%rax
-    646c3edf:	jb     646c3eb4 <lu_inverse_solver+0x33a>
-    646c3ee1:	mov    -0x10(%rbp),%rax
-    646c3ee5:	mov    %rax,%rcx
-    646c3ee8:	call   646c78f8 <free>
-    646c3eed:	nop
-    646c3eee:	add    $0xd8,%rsp
-    646c3ef5:	pop    %rbx
-    646c3ef6:	pop    %rbp
-    646c3ef7:	ret
-
-00000000646c3ef8 <lu_decomposition>:
-    646c3ef8:	push   %rbp
-    646c3ef9:	mov    %rsp,%rbp
-    646c3efc:	sub    $0x20,%rsp
-    646c3f00:	mov    %rcx,0x10(%rbp)
-    646c3f04:	mov    %rdx,0x18(%rbp)
-    646c3f08:	mov    %r8,0x20(%rbp)
-    646c3f0c:	mov    %r9d,0x28(%rbp)
-    646c3f10:	movl   $0x0,-0x4(%rbp)
-    646c3f17:	jmp    646c4276 <lu_decomposition+0x37e>
-    646c3f1c:	movl   $0x0,-0x8(%rbp)
-    646c3f23:	jmp    646c4072 <lu_decomposition+0x17a>
-    646c3f28:	mov    -0x8(%rbp),%eax
-    646c3f2b:	cmp    -0x4(%rbp),%eax
-    646c3f2e:	jge    646c3f60 <lu_decomposition+0x68>
-    646c3f30:	mov    -0x8(%rbp),%eax
-    646c3f33:	cltq
-    646c3f35:	lea    0x0(,%rax,8),%rdx
-    646c3f3d:	mov    0x18(%rbp),%rax
-    646c3f41:	add    %rdx,%rax
-    646c3f44:	mov    (%rax),%rdx
-    646c3f47:	mov    -0x4(%rbp),%eax
-    646c3f4a:	cltq
-    646c3f4c:	shl    $0x3,%rax
-    646c3f50:	add    %rdx,%rax
-    646c3f53:	pxor   %xmm0,%xmm0
-    646c3f57:	movsd  %xmm0,(%rax)
-    646c3f5b:	jmp    646c406e <lu_decomposition+0x176>
-    646c3f60:	mov    -0x8(%rbp),%eax
-    646c3f63:	cltq
-    646c3f65:	lea    0x0(,%rax,8),%rdx
-    646c3f6d:	mov    0x10(%rbp),%rax
-    646c3f71:	add    %rdx,%rax
-    646c3f74:	mov    (%rax),%rdx
-    646c3f77:	mov    -0x4(%rbp),%eax
-    646c3f7a:	cltq
-    646c3f7c:	shl    $0x3,%rax
-    646c3f80:	add    %rax,%rdx
-    646c3f83:	mov    -0x8(%rbp),%eax
-    646c3f86:	cltq
-    646c3f88:	lea    0x0(,%rax,8),%rcx
-    646c3f90:	mov    0x18(%rbp),%rax
-    646c3f94:	add    %rcx,%rax
-    646c3f97:	mov    (%rax),%rcx
-    646c3f9a:	mov    -0x4(%rbp),%eax
-    646c3f9d:	cltq
-    646c3f9f:	shl    $0x3,%rax
-    646c3fa3:	add    %rcx,%rax
-    646c3fa6:	movsd  (%rdx),%xmm0
-    646c3faa:	movsd  %xmm0,(%rax)
-    646c3fae:	movl   $0x0,-0xc(%rbp)
-    646c3fb5:	jmp    646c4062 <lu_decomposition+0x16a>
-    646c3fba:	mov    -0x8(%rbp),%eax
-    646c3fbd:	cltq
-    646c3fbf:	lea    0x0(,%rax,8),%rdx
-    646c3fc7:	mov    0x18(%rbp),%rax
-    646c3fcb:	add    %rdx,%rax
-    646c3fce:	mov    (%rax),%rdx
-    646c3fd1:	mov    -0x4(%rbp),%eax
-    646c3fd4:	cltq
-    646c3fd6:	shl    $0x3,%rax
-    646c3fda:	add    %rdx,%rax
-    646c3fdd:	movsd  (%rax),%xmm0
-    646c3fe1:	mov    -0x8(%rbp),%eax
-    646c3fe4:	cltq
-    646c3fe6:	lea    0x0(,%rax,8),%rdx
-    646c3fee:	mov    0x18(%rbp),%rax
-    646c3ff2:	add    %rdx,%rax
-    646c3ff5:	mov    (%rax),%rdx
-    646c3ff8:	mov    -0xc(%rbp),%eax
-    646c3ffb:	cltq
-    646c3ffd:	shl    $0x3,%rax
-    646c4001:	add    %rdx,%rax
-    646c4004:	movsd  (%rax),%xmm2
-    646c4008:	mov    -0xc(%rbp),%eax
-    646c400b:	cltq
-    646c400d:	lea    0x0(,%rax,8),%rdx
-    646c4015:	mov    0x20(%rbp),%rax
-    646c4019:	add    %rdx,%rax
-    646c401c:	mov    (%rax),%rdx
-    646c401f:	mov    -0x4(%rbp),%eax
-    646c4022:	cltq
-    646c4024:	shl    $0x3,%rax
-    646c4028:	add    %rdx,%rax
-    646c402b:	movsd  (%rax),%xmm1
-    646c402f:	mulsd  %xmm2,%xmm1
-    646c4033:	mov    -0x8(%rbp),%eax
-    646c4036:	cltq
-    646c4038:	lea    0x0(,%rax,8),%rdx
-    646c4040:	mov    0x18(%rbp),%rax
-    646c4044:	add    %rdx,%rax
-    646c4047:	mov    (%rax),%rdx
-    646c404a:	mov    -0x4(%rbp),%eax
-    646c404d:	cltq
-    646c404f:	shl    $0x3,%rax
-    646c4053:	add    %rdx,%rax
-    646c4056:	subsd  %xmm1,%xmm0
-    646c405a:	movsd  %xmm0,(%rax)
-    646c405e:	addl   $0x1,-0xc(%rbp)
-    646c4062:	mov    -0xc(%rbp),%eax
-    646c4065:	cmp    -0x4(%rbp),%eax
-    646c4068:	jl     646c3fba <lu_decomposition+0xc2>
-    646c406e:	addl   $0x1,-0x8(%rbp)
-    646c4072:	mov    -0x8(%rbp),%eax
-    646c4075:	cmp    0x28(%rbp),%eax
-    646c4078:	jl     646c3f28 <lu_decomposition+0x30>
-    646c407e:	movl   $0x0,-0x10(%rbp)
-    646c4085:	jmp    646c4266 <lu_decomposition+0x36e>
-    646c408a:	mov    -0x10(%rbp),%eax
-    646c408d:	cmp    -0x4(%rbp),%eax
-    646c4090:	jge    646c40c2 <lu_decomposition+0x1ca>
-    646c4092:	mov    -0x4(%rbp),%eax
-    646c4095:	cltq
-    646c4097:	lea    0x0(,%rax,8),%rdx
-    646c409f:	mov    0x20(%rbp),%rax
-    646c40a3:	add    %rdx,%rax
-    646c40a6:	mov    (%rax),%rdx
-    646c40a9:	mov    -0x10(%rbp),%eax
-    646c40ac:	cltq
-    646c40ae:	shl    $0x3,%rax
-    646c40b2:	add    %rdx,%rax
-    646c40b5:	pxor   %xmm0,%xmm0
-    646c40b9:	movsd  %xmm0,(%rax)
-    646c40bd:	jmp    646c4262 <lu_decomposition+0x36a>
-    646c40c2:	mov    -0x10(%rbp),%eax
-    646c40c5:	cmp    -0x4(%rbp),%eax
-    646c40c8:	jne    646c40fe <lu_decomposition+0x206>
-    646c40ca:	mov    -0x4(%rbp),%eax
-    646c40cd:	cltq
-    646c40cf:	lea    0x0(,%rax,8),%rdx
-    646c40d7:	mov    0x20(%rbp),%rax
-    646c40db:	add    %rdx,%rax
-    646c40de:	mov    (%rax),%rdx
-    646c40e1:	mov    -0x10(%rbp),%eax
-    646c40e4:	cltq
-    646c40e6:	shl    $0x3,%rax
-    646c40ea:	add    %rdx,%rax
-    646c40ed:	movsd  0x4feb(%rip),%xmm0        # 646c90e0 <.rdata+0x50>
-    646c40f5:	movsd  %xmm0,(%rax)
-    646c40f9:	jmp    646c4262 <lu_decomposition+0x36a>
-    646c40fe:	mov    -0x4(%rbp),%eax
-    646c4101:	cltq
-    646c4103:	lea    0x0(,%rax,8),%rdx
-    646c410b:	mov    0x10(%rbp),%rax
-    646c410f:	add    %rdx,%rax
-    646c4112:	mov    (%rax),%rdx
-    646c4115:	mov    -0x10(%rbp),%eax
-    646c4118:	cltq
-    646c411a:	shl    $0x3,%rax
-    646c411e:	add    %rdx,%rax
-    646c4121:	movsd  (%rax),%xmm0
-    646c4125:	mov    -0x4(%rbp),%eax
-    646c4128:	cltq
-    646c412a:	lea    0x0(,%rax,8),%rdx
-    646c4132:	mov    0x18(%rbp),%rax
-    646c4136:	add    %rdx,%rax
-    646c4139:	mov    (%rax),%rdx
-    646c413c:	mov    -0x4(%rbp),%eax
-    646c413f:	cltq
-    646c4141:	shl    $0x3,%rax
-    646c4145:	add    %rdx,%rax
-    646c4148:	movsd  (%rax),%xmm1
-    646c414c:	mov    -0x4(%rbp),%eax
-    646c414f:	cltq
-    646c4151:	lea    0x0(,%rax,8),%rdx
-    646c4159:	mov    0x20(%rbp),%rax
-    646c415d:	add    %rdx,%rax
-    646c4160:	mov    (%rax),%rdx
-    646c4163:	mov    -0x10(%rbp),%eax
-    646c4166:	cltq
-    646c4168:	shl    $0x3,%rax
-    646c416c:	add    %rdx,%rax
-    646c416f:	divsd  %xmm1,%xmm0
-    646c4173:	movsd  %xmm0,(%rax)
-    646c4177:	movl   $0x0,-0x14(%rbp)
-    646c417e:	jmp    646c4256 <lu_decomposition+0x35e>
-    646c4183:	mov    -0x4(%rbp),%eax
-    646c4186:	cltq
-    646c4188:	lea    0x0(,%rax,8),%rdx
-    646c4190:	mov    0x20(%rbp),%rax
-    646c4194:	add    %rdx,%rax
-    646c4197:	mov    (%rax),%rdx
-    646c419a:	mov    -0x10(%rbp),%eax
-    646c419d:	cltq
-    646c419f:	shl    $0x3,%rax
-    646c41a3:	add    %rdx,%rax
-    646c41a6:	movsd  (%rax),%xmm0
-    646c41aa:	mov    -0x4(%rbp),%eax
-    646c41ad:	cltq
-    646c41af:	lea    0x0(,%rax,8),%rdx
-    646c41b7:	mov    0x18(%rbp),%rax
-    646c41bb:	add    %rdx,%rax
-    646c41be:	mov    (%rax),%rdx
-    646c41c1:	mov    -0x14(%rbp),%eax
-    646c41c4:	cltq
-    646c41c6:	shl    $0x3,%rax
-    646c41ca:	add    %rdx,%rax
-    646c41cd:	movsd  (%rax),%xmm2
-    646c41d1:	mov    -0x14(%rbp),%eax
-    646c41d4:	cltq
-    646c41d6:	lea    0x0(,%rax,8),%rdx
-    646c41de:	mov    0x20(%rbp),%rax
-    646c41e2:	add    %rdx,%rax
-    646c41e5:	mov    (%rax),%rdx
-    646c41e8:	mov    -0x10(%rbp),%eax
-    646c41eb:	cltq
-    646c41ed:	shl    $0x3,%rax
-    646c41f1:	add    %rdx,%rax
-    646c41f4:	movsd  (%rax),%xmm1
-    646c41f8:	mulsd  %xmm2,%xmm1
-    646c41fc:	mov    -0x4(%rbp),%eax
-    646c41ff:	cltq
-    646c4201:	lea    0x0(,%rax,8),%rdx
-    646c4209:	mov    0x18(%rbp),%rax
-    646c420d:	add    %rdx,%rax
-    646c4210:	mov    (%rax),%rdx
-    646c4213:	mov    -0x4(%rbp),%eax
-    646c4216:	cltq
-    646c4218:	shl    $0x3,%rax
-    646c421c:	add    %rdx,%rax
-    646c421f:	movsd  (%rax),%xmm2
-    646c4223:	divsd  %xmm2,%xmm1
-    646c4227:	mov    -0x4(%rbp),%eax
-    646c422a:	cltq
-    646c422c:	lea    0x0(,%rax,8),%rdx
-    646c4234:	mov    0x20(%rbp),%rax
-    646c4238:	add    %rdx,%rax
-    646c423b:	mov    (%rax),%rdx
-    646c423e:	mov    -0x10(%rbp),%eax
-    646c4241:	cltq
-    646c4243:	shl    $0x3,%rax
-    646c4247:	add    %rdx,%rax
-    646c424a:	subsd  %xmm1,%xmm0
-    646c424e:	movsd  %xmm0,(%rax)
-    646c4252:	addl   $0x1,-0x14(%rbp)
-    646c4256:	mov    -0x14(%rbp),%eax
-    646c4259:	cmp    -0x4(%rbp),%eax
-    646c425c:	jl     646c4183 <lu_decomposition+0x28b>
-    646c4262:	addl   $0x1,-0x10(%rbp)
-    646c4266:	mov    -0x10(%rbp),%eax
-    646c4269:	cmp    0x28(%rbp),%eax
-    646c426c:	jl     646c408a <lu_decomposition+0x192>
-    646c4272:	addl   $0x1,-0x4(%rbp)
-    646c4276:	mov    -0x4(%rbp),%eax
-    646c4279:	cmp    0x28(%rbp),%eax
-    646c427c:	jl     646c3f1c <lu_decomposition+0x24>
-    646c4282:	nop
-    646c4283:	add    $0x20,%rsp
-    646c4287:	pop    %rbp
-    646c4288:	ret
-
-00000000646c4289 <arange>:
-    646c4289:	push   %rbp
-    646c428a:	mov    %rsp,%rbp
-    646c428d:	sub    $0x30,%rsp
-    646c4291:	mov    %ecx,0x10(%rbp)
-    646c4294:	mov    0x10(%rbp),%eax
-    646c4297:	cltq
-    646c4299:	shl    $0x2,%rax
-    646c429d:	mov    %rax,%rcx
-    646c42a0:	call   646c78e0 <malloc>
-    646c42a5:	mov    %rax,-0x10(%rbp)
-    646c42a9:	movl   $0x0,-0x4(%rbp)
-    646c42b0:	jmp    646c42cf <arange+0x46>
-    646c42b2:	mov    -0x4(%rbp),%eax
-    646c42b5:	cltq
-    646c42b7:	lea    0x0(,%rax,4),%rdx
-    646c42bf:	mov    -0x10(%rbp),%rax
-    646c42c3:	add    %rdx,%rax
-    646c42c6:	mov    -0x4(%rbp),%edx
-    646c42c9:	mov    %edx,(%rax)
-    646c42cb:	addl   $0x1,-0x4(%rbp)
-    646c42cf:	mov    -0x4(%rbp),%eax
-    646c42d2:	cmp    0x10(%rbp),%eax
-    646c42d5:	jl     646c42b2 <arange+0x29>
-    646c42d7:	mov    -0x10(%rbp),%rax
-    646c42db:	add    $0x30,%rsp
-    646c42df:	pop    %rbp
-    646c42e0:	ret
-
-00000000646c42e1 <d_arange>:
-    646c42e1:	push   %rbp
-    646c42e2:	mov    %rsp,%rbp
-    646c42e5:	sub    $0x30,%rsp
-    646c42e9:	mov    %ecx,0x10(%rbp)
-    646c42ec:	mov    0x10(%rbp),%eax
-    646c42ef:	cltq
-    646c42f1:	shl    $0x3,%rax
-    646c42f5:	mov    %rax,%rcx
-    646c42f8:	call   646c78e0 <malloc>
-    646c42fd:	mov    %rax,-0x10(%rbp)
-    646c4301:	movl   $0x0,-0x4(%rbp)
-    646c4308:	jmp    646c432b <d_arange+0x4a>
-    646c430a:	mov    -0x4(%rbp),%eax
-    646c430d:	cltq
-    646c430f:	lea    0x0(,%rax,8),%rdx
-    646c4317:	mov    -0x10(%rbp),%rax
-    646c431b:	add    %rdx,%rax
-    646c431e:	cvtsi2sdl -0x4(%rbp),%xmm0
-    646c4323:	movsd  %xmm0,(%rax)
-    646c4327:	addl   $0x1,-0x4(%rbp)
-    646c432b:	mov    -0x4(%rbp),%eax
-    646c432e:	cmp    0x10(%rbp),%eax
-    646c4331:	jl     646c430a <d_arange+0x29>
-    646c4333:	mov    -0x10(%rbp),%rax
-    646c4337:	add    $0x30,%rsp
-    646c433b:	pop    %rbp
-    646c433c:	ret
-
-00000000646c433d <pdist>:
-    646c433d:	push   %rbp
-    646c433e:	mov    %rsp,%rbp
-    646c4341:	sub    $0x10,%rsp
-    646c4345:	mov    %rcx,0x10(%rbp)
-    646c4349:	mov    %rdx,0x18(%rbp)
-    646c434d:	mov    %r8d,0x20(%rbp)
-    646c4351:	movl   $0x0,-0x4(%rbp)
-    646c4358:	jmp    646c43dd <pdist+0xa0>
-    646c435d:	movl   $0x0,-0x8(%rbp)
-    646c4364:	jmp    646c43d1 <pdist+0x94>
-    646c4366:	mov    -0x8(%rbp),%eax
-    646c4369:	cltq
-    646c436b:	lea    0x0(,%rax,8),%rdx
-    646c4373:	mov    0x10(%rbp),%rax
-    646c4377:	add    %rdx,%rax
-    646c437a:	movsd  (%rax),%xmm0
-    646c437e:	mov    -0x4(%rbp),%eax
-    646c4381:	cltq
-    646c4383:	lea    0x0(,%rax,8),%rdx
-    646c438b:	mov    0x10(%rbp),%rax
-    646c438f:	add    %rdx,%rax
-    646c4392:	movsd  (%rax),%xmm1
-    646c4396:	subsd  %xmm1,%xmm0
-    646c439a:	mov    -0x4(%rbp),%eax
-    646c439d:	cltq
-    646c439f:	lea    0x0(,%rax,8),%rdx
-    646c43a7:	mov    0x18(%rbp),%rax
-    646c43ab:	add    %rdx,%rax
-    646c43ae:	mov    (%rax),%rdx
-    646c43b1:	mov    -0x8(%rbp),%eax
-    646c43b4:	cltq
-    646c43b6:	shl    $0x3,%rax
-    646c43ba:	add    %rdx,%rax
-    646c43bd:	movq   0x4d2b(%rip),%xmm1        # 646c90f0 <.rdata+0x60>
-    646c43c5:	andpd  %xmm1,%xmm0
-    646c43c9:	movsd  %xmm0,(%rax)
-    646c43cd:	addl   $0x1,-0x8(%rbp)
-    646c43d1:	mov    -0x8(%rbp),%eax
-    646c43d4:	cmp    0x20(%rbp),%eax
-    646c43d7:	jl     646c4366 <pdist+0x29>
-    646c43d9:	addl   $0x1,-0x4(%rbp)
-    646c43dd:	mov    -0x4(%rbp),%eax
-    646c43e0:	cmp    0x20(%rbp),%eax
-    646c43e3:	jl     646c435d <pdist+0x20>
-    646c43e9:	nop
-    646c43ea:	add    $0x10,%rsp
-    646c43ee:	pop    %rbp
-    646c43ef:	ret
-
-00000000646c43f0 <matrixform>:
-    646c43f0:	push   %rbp
-    646c43f1:	mov    %rsp,%rbp
-    646c43f4:	sub    $0x10,%rsp
-    646c43f8:	mov    %rcx,0x10(%rbp)
-    646c43fc:	mov    %rdx,0x18(%rbp)
-    646c4400:	mov    %r8d,0x20(%rbp)
-    646c4404:	movl   $0x0,-0x4(%rbp)
-    646c440b:	jmp    646c446e <matrixform+0x7e>
-    646c440d:	movl   $0x0,-0x8(%rbp)
-    646c4414:	jmp    646c4462 <matrixform+0x72>
-    646c4416:	mov    0x20(%rbp),%eax
-    646c4419:	imul   -0x4(%rbp),%eax
-    646c441d:	mov    -0x8(%rbp),%edx
-    646c4420:	add    %edx,%eax
-    646c4422:	cltq
-    646c4424:	lea    0x0(,%rax,8),%rdx
-    646c442c:	mov    0x10(%rbp),%rax
-    646c4430:	add    %rax,%rdx
-    646c4433:	mov    -0x4(%rbp),%eax
-    646c4436:	cltq
-    646c4438:	lea    0x0(,%rax,8),%rcx
-    646c4440:	mov    0x18(%rbp),%rax
-    646c4444:	add    %rcx,%rax
-    646c4447:	mov    (%rax),%rcx
-    646c444a:	mov    -0x8(%rbp),%eax
-    646c444d:	cltq
-    646c444f:	shl    $0x3,%rax
-    646c4453:	add    %rcx,%rax
-    646c4456:	movsd  (%rdx),%xmm0
-    646c445a:	movsd  %xmm0,(%rax)
-    646c445e:	addl   $0x1,-0x8(%rbp)
-    646c4462:	mov    -0x8(%rbp),%eax
-    646c4465:	cmp    0x20(%rbp),%eax
-    646c4468:	jl     646c4416 <matrixform+0x26>
-    646c446a:	addl   $0x1,-0x4(%rbp)
-    646c446e:	mov    -0x4(%rbp),%eax
-    646c4471:	cmp    0x20(%rbp),%eax
-    646c4474:	jl     646c440d <matrixform+0x1d>
-    646c4476:	nop
-    646c4477:	add    $0x10,%rsp
-    646c447b:	pop    %rbp
-    646c447c:	ret
-
-00000000646c447d <save_1darray>:
-    646c447d:	push   %rbp
-    646c447e:	sub    $0x1e0,%rsp
-    646c4485:	lea    0x80(%rsp),%rbp
-    646c448d:	mov    %rcx,0x170(%rbp)
-    646c4494:	mov    %edx,0x178(%rbp)
-    646c449a:	mov    %r8,0x180(%rbp)
-    646c44a1:	mov    %r9,0x188(%rbp)
-    646c44a8:	cvtsi2sdl 0x190(%rbp),%xmm0
-    646c44b0:	call   646c78e8 <log10>
-    646c44b5:	movq   %xmm0,%rax
-    646c44ba:	movq   %rax,%xmm0
-    646c44bf:	call   646c6910 <ceil>
-    646c44c4:	cvttsd2si %xmm0,%eax
-    646c44c8:	add    $0x1,%eax
-    646c44cb:	mov    %eax,0x158(%rbp)
-    646c44d1:	mov    0x188(%rbp),%rcx
-    646c44d8:	lea    0x80(%rbp),%rax
-    646c44df:	mov    0x158(%rbp),%edx
-    646c44e5:	mov    %edx,0x28(%rsp)
-    646c44e9:	mov    0x180(%rbp),%rdx
-    646c44f0:	mov    %rdx,0x20(%rsp)
-    646c44f5:	mov    %rcx,%r9
-    646c44f8:	lea    0x4b91(%rip),%r8        # 646c9090 <.rdata>
-    646c44ff:	mov    $0xc8,%edx
-    646c4504:	mov    %rax,%rcx
-    646c4507:	call   646c3b30 <snprintf>
-    646c450c:	mov    0x188(%rbp),%rax
-    646c4513:	mov    %rax,%rcx
-    646c4516:	call   646c7938 <_mkdir>
-    646c451b:	cmp    $0xffffffff,%eax
-    646c451e:	jne    646c453c <save_1darray+0xbf>
-    646c4520:	mov    0x9d75(%rip),%rax        # 646ce29c <__imp__errno>
-    646c4527:	call   *%rax
-    646c4529:	mov    (%rax),%eax
-    646c452b:	cmp    $0x11,%eax
-    646c452e:	je     646c453c <save_1darray+0xbf>
-    646c4530:	lea    0x4b68(%rip),%rcx        # 646c909f <.rdata+0xf>
-    646c4537:	call   646c78d0 <printf>
-    646c453c:	mov    0x198(%rbp),%ecx
-    646c4542:	lea    0x80(%rbp),%rdx
-    646c4549:	lea    -0x50(%rbp),%rax
-    646c454d:	mov    %ecx,%r9d
-    646c4550:	mov    %rdx,%r8
-    646c4553:	mov    $0xc8,%edx
-    646c4558:	mov    %rax,%rcx
-    646c455b:	call   646c3b30 <snprintf>
-    646c4560:	lea    -0x50(%rbp),%rax
-    646c4564:	lea    0x4b4a(%rip),%rdx        # 646c90b5 <.rdata+0x25>
-    646c456b:	mov    %rax,%rcx
-    646c456e:	call   646c7908 <fopen>
-    646c4573:	mov    %rax,0x150(%rbp)
-    646c457a:	cmpq   $0x0,0x150(%rbp)
-    646c4582:	jne    646c459a <save_1darray+0x11d>
-    646c4584:	lea    0x4b2c(%rip),%rcx        # 646c90b7 <.rdata+0x27>
-    646c458b:	call   646c78d8 <perror>
-    646c4590:	mov    $0x1,%ecx
-    646c4595:	call   646c7918 <exit>
-    646c459a:	movl   $0x0,0x15c(%rbp)
-    646c45a4:	jmp    646c4604 <save_1darray+0x187>
-    646c45a6:	mov    0x15c(%rbp),%eax
-    646c45ac:	cltq
-    646c45ae:	lea    0x0(,%rax,8),%rdx
-    646c45b6:	mov    0x170(%rbp),%rax
-    646c45bd:	add    %rdx,%rax
-    646c45c0:	movsd  (%rax),%xmm0
-    646c45c4:	movq   %xmm0,%rax
-    646c45c9:	mov    %rax,%rdx
-    646c45cc:	mov    %rdx,%rcx
-    646c45cf:	movq   %rax,%xmm0
-    646c45d4:	mov    0x15c(%rbp),%edx
-    646c45da:	mov    0x150(%rbp),%rax
-    646c45e1:	movq   %rcx,%xmm3
-    646c45e6:	movq   %xmm0,%r9
-    646c45eb:	mov    %edx,%r8d
-    646c45ee:	lea    0x4ada(%rip),%rdx        # 646c90cf <.rdata+0x3f>
-    646c45f5:	mov    %rax,%rcx
-    646c45f8:	call   646c7900 <fprintf>
-    646c45fd:	addl   $0x1,0x15c(%rbp)
-    646c4604:	mov    0x15c(%rbp),%eax
-    646c460a:	cmp    0x178(%rbp),%eax
-    646c4610:	jl     646c45a6 <save_1darray+0x129>
-    646c4612:	mov    0x150(%rbp),%rax
-    646c4619:	mov    %rax,%rcx
-    646c461c:	call   646c7910 <fclose>
-    646c4621:	nop
-    646c4622:	add    $0x1e0,%rsp
-    646c4629:	pop    %rbp
-    646c462a:	ret
-    646c462b:	nop
-    646c462c:	nop
-    646c462d:	nop
-    646c462e:	nop
-    646c462f:	nop
-
-00000000646c4630 <randompath>:
-    646c4630:	push   %rbp
-    646c4631:	mov    %rsp,%rbp
-    646c4634:	sub    $0x30,%rsp
-    646c4638:	mov    %rcx,0x10(%rbp)
-    646c463c:	mov    %edx,0x18(%rbp)
-    646c463f:	mov    %r8,0x20(%rbp)
-    646c4643:	mov    0x18(%rbp),%eax
-    646c4646:	sub    $0x1,%eax
-    646c4649:	mov    %eax,-0x4(%rbp)
-    646c464c:	jmp    646c46cb <randompath+0x9b>
-    646c464e:	mov    0x20(%rbp),%rax
-    646c4652:	mov    %rax,%rcx
-    646c4655:	call   646c2aae <mt19937_generate>
-    646c465a:	mov    -0x4(%rbp),%ecx
-    646c465d:	mov    $0x0,%edx
-    646c4662:	div    %ecx
-    646c4664:	mov    %edx,%eax
-    646c4666:	mov    %eax,-0x8(%rbp)
-    646c4669:	mov    -0x8(%rbp),%eax
-    646c466c:	cltq
-    646c466e:	lea    0x0(,%rax,4),%rdx
-    646c4676:	mov    0x10(%rbp),%rax
-    646c467a:	add    %rdx,%rax
-    646c467d:	mov    (%rax),%eax
-    646c467f:	mov    %eax,-0xc(%rbp)
-    646c4682:	mov    -0x4(%rbp),%eax
-    646c4685:	cltq
-    646c4687:	lea    0x0(,%rax,4),%rdx
-    646c468f:	mov    0x10(%rbp),%rax
-    646c4693:	add    %rax,%rdx
-    646c4696:	mov    -0x8(%rbp),%eax
-    646c4699:	cltq
-    646c469b:	lea    0x0(,%rax,4),%rcx
-    646c46a3:	mov    0x10(%rbp),%rax
-    646c46a7:	add    %rcx,%rax
-    646c46aa:	mov    (%rdx),%edx
-    646c46ac:	mov    %edx,(%rax)
-    646c46ae:	mov    -0x4(%rbp),%eax
-    646c46b1:	cltq
-    646c46b3:	lea    0x0(,%rax,4),%rdx
-    646c46bb:	mov    0x10(%rbp),%rax
-    646c46bf:	add    %rdx,%rax
-    646c46c2:	mov    -0xc(%rbp),%edx
-    646c46c5:	mov    %edx,(%rax)
-    646c46c7:	subl   $0x1,-0x4(%rbp)
-    646c46cb:	cmpl   $0x0,-0x4(%rbp)
-    646c46cf:	jne    646c464e <randompath+0x1e>
-    646c46d5:	mov    0x10(%rbp),%rax
-    646c46d9:	add    $0x30,%rsp
-    646c46dd:	pop    %rbp
-    646c46de:	ret
-    646c46df:	nop
-
-00000000646c46e0 <sgsim_init>:
-    646c46e0:	push   %rbp
-    646c46e1:	mov    %rsp,%rbp
-    646c46e4:	sub    $0x30,%rsp
-    646c46e8:	mov    %rcx,0x10(%rbp)
-    646c46ec:	mov    %edx,0x18(%rbp)
-    646c46ef:	mov    %r8d,0x20(%rbp)
-    646c46f3:	mov    %r9d,0x28(%rbp)
-    646c46f7:	mov    0x10(%rbp),%rax
-    646c46fb:	mov    0x18(%rbp),%edx
-    646c46fe:	mov    %edx,(%rax)
-    646c4700:	mov    0x10(%rbp),%rax
-    646c4704:	mov    0x20(%rbp),%edx
-    646c4707:	mov    %edx,0x4(%rax)
-    646c470a:	mov    0x10(%rbp),%rax
-    646c470e:	mov    0x28(%rbp),%edx
-    646c4711:	mov    %edx,0x8(%rax)
-    646c4714:	cmpl   $0x1,0x30(%rbp)
-    646c4718:	jne    646c473e <sgsim_init+0x5e>
-    646c471a:	mov    0x18(%rbp),%eax
-    646c471d:	imul   0x20(%rbp),%eax
-    646c4721:	mov    %eax,-0x4(%rbp)
-    646c4724:	mov    -0x4(%rbp),%eax
-    646c4727:	shl    $0x3,%rax
-    646c472b:	mov    %rax,%rcx
-    646c472e:	call   646c78e0 <malloc>
-    646c4733:	mov    %rax,%rdx
-    646c4736:	mov    0x10(%rbp),%rax
-    646c473a:	mov    %rdx,0x10(%rax)
-    646c473e:	nop
-    646c473f:	add    $0x30,%rsp
-    646c4743:	pop    %rbp
-    646c4744:	ret
-
-00000000646c4745 <sgsim_run>:
-    646c4745:	push   %rbp
-    646c4746:	sub    $0xa00,%rsp
-    646c474d:	lea    0x80(%rsp),%rbp
-    646c4755:	mov    %rcx,0x990(%rbp)
-    646c475c:	mov    %rdx,0x998(%rbp)
-    646c4763:	mov    %r8d,0x9a0(%rbp)
-    646c476a:	mov    0x990(%rbp),%rax
-    646c4771:	mov    0x8(%rax),%eax
-    646c4774:	mov    %eax,%edx
-    646c4776:	lea    -0x50(%rbp),%rax
-    646c477a:	mov    %rax,%rcx
-    646c477d:	call   646c2a30 <mt19937_init>
-    646c4782:	mov    0x990(%rbp),%rax
-    646c4789:	mov    (%rax),%eax
-    646c478b:	mov    %eax,%edx
-    646c478d:	lea    0x7a8c(%rip),%rcx        # 646cc220 <_sampling>
-    646c4794:	call   646c30e0 <sampling_state_init>
-    646c4799:	mov    0x998(%rbp),%rax
-    646c47a0:	mov    0x4(%rax),%eax
-    646c47a3:	cltq
-    646c47a5:	mov    %rax,0x7a3c(%rip)        # 646cc1e8 <variogram_array+0x8>
-    646c47ac:	mov    0x998(%rbp),%rax
-    646c47b3:	mov    0x4(%rax),%eax
-    646c47b6:	cltq
-    646c47b8:	mov    %rax,0x7a31(%rip)        # 646cc1f0 <variogram_array+0x10>
-    646c47bf:	mov    0x998(%rbp),%rax
-    646c47c6:	mov    0x4(%rax),%eax
-    646c47c9:	cltq
-    646c47cb:	mov    $0x8,%edx
-    646c47d0:	mov    %rax,%rcx
-    646c47d3:	call   646c7920 <calloc>
-    646c47d8:	mov    %rax,0x7a01(%rip)        # 646cc1e0 <variogram_array>
-    646c47df:	mov    0x990(%rbp),%rax
-    646c47e6:	mov    (%rax),%eax
-    646c47e8:	cltq
-    646c47ea:	mov    %rax,0x7a17(%rip)        # 646cc208 <sgsim_array+0x8>
-    646c47f1:	mov    0x990(%rbp),%rax
-    646c47f8:	mov    (%rax),%eax
-    646c47fa:	cltq
-    646c47fc:	mov    %rax,0x7a0d(%rip)        # 646cc210 <sgsim_array+0x10>
-    646c4803:	mov    0x990(%rbp),%rax
-    646c480a:	mov    (%rax),%eax
-    646c480c:	cltq
-    646c480e:	mov    $0x8,%edx
-    646c4813:	mov    %rax,%rcx
-    646c4816:	call   646c7920 <calloc>
-    646c481b:	mov    %rax,0x79de(%rip)        # 646cc200 <sgsim_array>
-    646c4822:	mov    0x998(%rbp),%rax
-    646c4829:	movsd  0x10(%rax),%xmm0
-    646c482e:	mov    0x998(%rbp),%rax
-    646c4835:	mov    0x8(%rax),%rax
-    646c4839:	movapd %xmm0,%xmm1
-    646c483d:	movq   %rax,%xmm0
-    646c4842:	call   646c31bd <krige_param_setting>
-    646c4847:	mov    0x990(%rbp),%rax
-    646c484e:	mov    (%rax),%eax
-    646c4850:	mov    %eax,%ecx
-    646c4852:	call   646c4289 <arange>
-    646c4857:	mov    %rax,0x7922(%rip)        # 646cc180 <x_grid>
-    646c485e:	movl   $0x0,0x7a04(%rip)        # 646cc26c <count>
-    646c4868:	jmp    646c4bdc <sgsim_run+0x497>
-    646c486d:	mov    0x79f9(%rip),%eax        # 646cc26c <count>
-    646c4873:	mov    %eax,%edx
-    646c4875:	lea    0x4884(%rip),%rcx        # 646c9100 <.rdata>
-    646c487c:	call   646c78d0 <printf>
-    646c4881:	movl   $0x0,0x7999(%rip)        # 646cc224 <_sampling+0x4>
-    646c488b:	movl   $0x0,0x798b(%rip)        # 646cc220 <_sampling>
-    646c4895:	movl   $0x0,0x79c9(%rip)        # 646cc268 <flag>
-    646c489f:	mov    0x990(%rbp),%rax
-    646c48a6:	mov    (%rax),%edx
-    646c48a8:	mov    0x78d1(%rip),%rax        # 646cc180 <x_grid>
-    646c48af:	lea    -0x50(%rbp),%rcx
-    646c48b3:	mov    %rcx,%r8
-    646c48b6:	mov    %rax,%rcx
-    646c48b9:	call   646c4630 <randompath>
-    646c48be:	mov    %rax,0x78bb(%rip)        # 646cc180 <x_grid>
-    646c48c5:	movl   $0x0,0x97c(%rbp)
-    646c48cf:	jmp    646c4936 <sgsim_run+0x1f1>
-    646c48d1:	mov    0x7928(%rip),%rdx        # 646cc200 <sgsim_array>
-    646c48d8:	mov    0x97c(%rbp),%eax
-    646c48de:	cltq
-    646c48e0:	shl    $0x3,%rax
-    646c48e4:	add    %rdx,%rax
-    646c48e7:	pxor   %xmm0,%xmm0
-    646c48eb:	movsd  %xmm0,(%rax)
-    646c48ef:	mov    0x7942(%rip),%rdx        # 646cc238 <_sampling+0x18>
-    646c48f6:	mov    0x97c(%rbp),%eax
-    646c48fc:	cltq
-    646c48fe:	shl    $0x3,%rax
-    646c4902:	add    %rdx,%rax
-    646c4905:	pxor   %xmm0,%xmm0
-    646c4909:	movsd  %xmm0,(%rax)
-    646c490d:	mov    0x793c(%rip),%rdx        # 646cc250 <_sampling+0x30>
-    646c4914:	mov    0x97c(%rbp),%eax
-    646c491a:	cltq
-    646c491c:	shl    $0x3,%rax
-    646c4920:	add    %rdx,%rax
-    646c4923:	movsd  0x4825(%rip),%xmm0        # 646c9150 <.rdata+0x50>
-    646c492b:	movsd  %xmm0,(%rax)
-    646c492f:	addl   $0x1,0x97c(%rbp)
-    646c4936:	mov    0x990(%rbp),%rax
-    646c493d:	mov    (%rax),%eax
-    646c493f:	cmp    %eax,0x97c(%rbp)
-    646c4945:	jl     646c48d1 <sgsim_run+0x18c>
-    646c4947:	movl   $0x0,0x978(%rbp)
-    646c4951:	jmp    646c4acf <sgsim_run+0x38a>
-    646c4956:	mov    0x7823(%rip),%rdx        # 646cc180 <x_grid>
-    646c495d:	mov    0x978(%rbp),%eax
-    646c4963:	cltq
-    646c4965:	shl    $0x2,%rax
-    646c4969:	add    %rdx,%rax
-    646c496c:	mov    (%rax),%eax
-    646c496e:	cvtsi2sd %eax,%xmm0
-    646c4972:	mov    0x978(%rbp),%eax
-    646c4978:	mov    %eax,%r8d
-    646c497b:	movapd %xmm0,%xmm1
-    646c497f:	lea    0x789a(%rip),%rcx        # 646cc220 <_sampling>
-    646c4986:	call   646c3191 <sampling_state_update>
-    646c498b:	mov    0x786e(%rip),%rax        # 646cc200 <sgsim_array>
-    646c4992:	lea    -0x50(%rbp),%rdx
-    646c4996:	mov    %rdx,%r8
-    646c4999:	lea    0x7880(%rip),%rdx        # 646cc220 <_sampling>
-    646c49a0:	mov    %rax,%rcx
-    646c49a3:	call   646c3413 <simple_kriging>
-    646c49a8:	mov    0x7851(%rip),%rdx        # 646cc200 <sgsim_array>
-    646c49af:	mov    0x77ca(%rip),%rcx        # 646cc180 <x_grid>
-    646c49b6:	mov    0x978(%rbp),%eax
-    646c49bc:	cltq
-    646c49be:	shl    $0x2,%rax
-    646c49c2:	add    %rcx,%rax
-    646c49c5:	mov    (%rax),%eax
-    646c49c7:	cltq
-    646c49c9:	shl    $0x3,%rax
-    646c49cd:	add    %rax,%rdx
-    646c49d0:	mov    0x990(%rbp),%rax
-    646c49d7:	mov    0x10(%rax),%rcx
-    646c49db:	mov    0x779e(%rip),%r8        # 646cc180 <x_grid>
-    646c49e2:	mov    0x978(%rbp),%eax
-    646c49e8:	cltq
-    646c49ea:	shl    $0x2,%rax
-    646c49ee:	add    %r8,%rax
-    646c49f1:	mov    (%rax),%r8d
-    646c49f4:	mov    0x990(%rbp),%rax
-    646c49fb:	mov    (%rax),%r9d
-    646c49fe:	mov    0x7868(%rip),%eax        # 646cc26c <count>
-    646c4a04:	imul   %r9d,%eax
-    646c4a08:	add    %r8d,%eax
-    646c4a0b:	cltq
-    646c4a0d:	shl    $0x3,%rax
-    646c4a11:	add    %rcx,%rax
-    646c4a14:	movsd  (%rdx),%xmm0
-    646c4a18:	movsd  %xmm0,(%rax)
-    646c4a1c:	mov    0x77fe(%rip),%eax        # 646cc220 <_sampling>
-    646c4a22:	cmp    $0x7,%eax
-    646c4a25:	jg     646c4a36 <sgsim_run+0x2f1>
-    646c4a27:	mov    0x77f3(%rip),%eax        # 646cc220 <_sampling>
-    646c4a2d:	add    $0x1,%eax
-    646c4a30:	mov    %eax,0x77ea(%rip)        # 646cc220 <_sampling>
-    646c4a36:	mov    0x7743(%rip),%rdx        # 646cc180 <x_grid>
-    646c4a3d:	mov    0x978(%rbp),%eax
-    646c4a43:	cltq
-    646c4a45:	shl    $0x2,%rax
-    646c4a49:	add    %rdx,%rax
-    646c4a4c:	mov    (%rax),%ecx
-    646c4a4e:	mov    0x77e3(%rip),%rdx        # 646cc238 <_sampling+0x18>
-    646c4a55:	mov    0x978(%rbp),%eax
-    646c4a5b:	cltq
-    646c4a5d:	shl    $0x3,%rax
-    646c4a61:	add    %rdx,%rax
-    646c4a64:	cvtsi2sd %ecx,%xmm0
-    646c4a68:	movsd  %xmm0,(%rax)
-    646c4a6c:	mov    0x77b2(%rip),%eax        # 646cc224 <_sampling+0x4>
-    646c4a72:	add    $0x1,%eax
-    646c4a75:	mov    %eax,0x77a9(%rip)        # 646cc224 <_sampling+0x4>
-    646c4a7b:	mov    0x777e(%rip),%rdx        # 646cc200 <sgsim_array>
-    646c4a82:	mov    0x76f7(%rip),%rcx        # 646cc180 <x_grid>
-    646c4a89:	mov    0x978(%rbp),%eax
-    646c4a8f:	cltq
-    646c4a91:	shl    $0x2,%rax
-    646c4a95:	add    %rcx,%rax
-    646c4a98:	mov    (%rax),%eax
-    646c4a9a:	cltq
-    646c4a9c:	shl    $0x3,%rax
-    646c4aa0:	add    %rdx,%rax
-    646c4aa3:	mov    (%rax),%rax
-    646c4aa6:	movq   %rax,%xmm0
-    646c4aab:	call   646c6770 <__fpclassify>
-    646c4ab0:	and    $0x100,%eax
-    646c4ab5:	test   %eax,%eax
-    646c4ab7:	je     646c4ac8 <sgsim_run+0x383>
-    646c4ab9:	mov    0x77a9(%rip),%eax        # 646cc268 <flag>
+    646c346c:	mov    %rax,%rcx
+    646c346f:	call   646c7970 <malloc>
+    646c3474:	mov    %rax,0x8c95(%rip)        # 646cc110 <array2d_temp>
+    646c347b:	movl   $0x0,-0x5c(%rbp)
+    646c3482:	jmp    646c34a9 <krige_param_setting+0x24c>
+    646c3484:	mov    0x8c85(%rip),%rdx        # 646cc110 <array2d_temp>
+    646c348b:	mov    -0x5c(%rbp),%eax
+    646c348e:	cltq
+    646c3490:	shl    $0x3,%rax
+    646c3494:	lea    (%rdx,%rax,1),%rbx
+    646c3498:	mov    $0x18,%ecx
+    646c349d:	call   646c7970 <malloc>
+    646c34a2:	mov    %rax,(%rbx)
+    646c34a5:	addl   $0x1,-0x5c(%rbp)
+    646c34a9:	mov    -0x5c(%rbp),%eax
+    646c34ac:	cmp    -0x30(%rbp),%eax
+    646c34af:	jl     646c3484 <krige_param_setting+0x227>
+    646c34b1:	nop
+    646c34b2:	add    $0x38,%rsp
+    646c34b6:	pop    %rbx
+    646c34b7:	pop    %rbp
+    646c34b8:	ret
+
+00000000646c34b9 <simple_kriging>:
+    646c34b9:	push   %rbp
+    646c34ba:	mov    %rsp,%rbp
+    646c34bd:	sub    $0x40,%rsp
+    646c34c1:	movaps %xmm6,-0x10(%rbp)
+    646c34c5:	mov    %rcx,0x10(%rbp)
+    646c34c9:	mov    %rdx,0x18(%rbp)
+    646c34cd:	mov    %r8,0x20(%rbp)
+    646c34d1:	mov    0x20(%rbp),%rdx
+    646c34d5:	mov    0x18(%rbp),%rax
+    646c34d9:	mov    %rdx,%r8
+    646c34dc:	mov    %rax,%rdx
+    646c34df:	mov    0x10(%rbp),%rcx
+    646c34e3:	call   646c38c7 <find_neighbor>
+    646c34e8:	mov    %eax,-0x20(%rbp)
+    646c34eb:	cmpl   $0x0,-0x20(%rbp)
+    646c34ef:	je     646c38bc <simple_kriging+0x403>
+    646c34f5:	movl   $0x0,-0x14(%rbp)
+    646c34fc:	jmp    646c35bc <simple_kriging+0x103>
+    646c3501:	mov    0x18(%rbp),%rax
+    646c3505:	mov    0x18(%rax),%rdx
+    646c3509:	mov    -0x14(%rbp),%eax
+    646c350c:	cltq
+    646c350e:	shl    $0x3,%rax
+    646c3512:	add    %rax,%rdx
+    646c3515:	mov    0x8bf4(%rip),%rcx        # 646cc110 <array2d_temp>
+    646c351c:	mov    -0x14(%rbp),%eax
+    646c351f:	cltq
+    646c3521:	shl    $0x3,%rax
+    646c3525:	add    %rcx,%rax
+    646c3528:	mov    (%rax),%rax
+    646c352b:	movsd  (%rdx),%xmm0
+    646c352f:	movsd  %xmm0,(%rax)
+    646c3533:	mov    0x18(%rbp),%rax
+    646c3537:	mov    0x18(%rax),%rdx
+    646c353b:	mov    -0x14(%rbp),%eax
+    646c353e:	cltq
+    646c3540:	shl    $0x3,%rax
+    646c3544:	add    %rdx,%rax
+    646c3547:	movsd  (%rax),%xmm0
+    646c354b:	cvttsd2si %xmm0,%eax
+    646c354f:	cltq
+    646c3551:	lea    0x0(,%rax,8),%rdx
+    646c3559:	mov    0x10(%rbp),%rax
+    646c355d:	add    %rax,%rdx
+    646c3560:	mov    0x8ba9(%rip),%rcx        # 646cc110 <array2d_temp>
+    646c3567:	mov    -0x14(%rbp),%eax
+    646c356a:	cltq
+    646c356c:	shl    $0x3,%rax
+    646c3570:	add    %rcx,%rax
+    646c3573:	mov    (%rax),%rax
+    646c3576:	add    $0x8,%rax
+    646c357a:	movsd  (%rdx),%xmm0
+    646c357e:	movsd  %xmm0,(%rax)
+    646c3582:	mov    0x18(%rbp),%rax
+    646c3586:	mov    0x30(%rax),%rdx
+    646c358a:	mov    -0x14(%rbp),%eax
+    646c358d:	cltq
+    646c358f:	shl    $0x3,%rax
+    646c3593:	add    %rax,%rdx
+    646c3596:	mov    0x8b73(%rip),%rcx        # 646cc110 <array2d_temp>
+    646c359d:	mov    -0x14(%rbp),%eax
+    646c35a0:	cltq
+    646c35a2:	shl    $0x3,%rax
+    646c35a6:	add    %rcx,%rax
+    646c35a9:	mov    (%rax),%rax
+    646c35ac:	add    $0x10,%rax
+    646c35b0:	movsd  (%rdx),%xmm0
+    646c35b4:	movsd  %xmm0,(%rax)
+    646c35b8:	addl   $0x1,-0x14(%rbp)
+    646c35bc:	mov    0x18(%rbp),%rax
+    646c35c0:	mov    0x4(%rax),%eax
+    646c35c3:	cmp    %eax,-0x14(%rbp)
+    646c35c6:	jl     646c3501 <simple_kriging+0x48>
+    646c35cc:	mov    0x18(%rbp),%rax
+    646c35d0:	mov    (%rax),%eax
+    646c35d2:	cmp    $0x1,%eax
+    646c35d5:	jle    646c35f8 <simple_kriging+0x13f>
+    646c35d7:	mov    0x18(%rbp),%rax
+    646c35db:	mov    0x4(%rax),%eax
+    646c35de:	lea    -0x1(%rax),%edx
+    646c35e1:	mov    0x8b28(%rip),%rax        # 646cc110 <array2d_temp>
+    646c35e8:	mov    %edx,%r8d
+    646c35eb:	mov    $0x0,%edx
+    646c35f0:	mov    %rax,%rcx
+    646c35f3:	call   646c50b1 <quicksort2d>
+    646c35f8:	movl   $0x0,-0x18(%rbp)
+    646c35ff:	jmp    646c3668 <simple_kriging+0x1af>
+    646c3601:	mov    0x8b08(%rip),%rdx        # 646cc110 <array2d_temp>
+    646c3608:	mov    -0x18(%rbp),%eax
+    646c360b:	cltq
+    646c360d:	shl    $0x3,%rax
+    646c3611:	add    %rdx,%rax
+    646c3614:	mov    (%rax),%rdx
+    646c3617:	mov    0x8a32(%rip),%rcx        # 646cc050 <location>
+    646c361e:	mov    -0x18(%rbp),%eax
+    646c3621:	cltq
+    646c3623:	shl    $0x3,%rax
+    646c3627:	add    %rcx,%rax
+    646c362a:	movsd  (%rdx),%xmm0
+    646c362e:	movsd  %xmm0,(%rax)
+    646c3632:	mov    0x8ad7(%rip),%rdx        # 646cc110 <array2d_temp>
+    646c3639:	mov    -0x18(%rbp),%eax
+    646c363c:	cltq
+    646c363e:	shl    $0x3,%rax
+    646c3642:	add    %rdx,%rax
+    646c3645:	mov    (%rax),%rdx
+    646c3648:	mov    0x8a61(%rip),%rcx        # 646cc0b0 <loc_cov2>
+    646c364f:	mov    -0x18(%rbp),%eax
+    646c3652:	cltq
+    646c3654:	shl    $0x3,%rax
+    646c3658:	add    %rcx,%rax
+    646c365b:	movsd  0x10(%rdx),%xmm0
+    646c3660:	movsd  %xmm0,(%rax)
+    646c3664:	addl   $0x1,-0x18(%rbp)
+    646c3668:	mov    0x18(%rbp),%rax
+    646c366c:	mov    (%rax),%eax
+    646c366e:	cmp    %eax,-0x18(%rbp)
+    646c3671:	jl     646c3601 <simple_kriging+0x148>
+    646c3673:	mov    0x18(%rbp),%rax
+    646c3677:	mov    (%rax),%ecx
+    646c3679:	mov    0x8ab0(%rip),%rdx        # 646cc130 <pdist_temp>
+    646c3680:	mov    0x89c9(%rip),%rax        # 646cc050 <location>
+    646c3687:	mov    %ecx,%r8d
+    646c368a:	mov    %rax,%rcx
+    646c368d:	call   646c43dd <pdist>
+    646c3692:	mov    0x8987(%rip),%r8        # 646cc020 <model>
+    646c3699:	mov    0x18(%rbp),%rax
+    646c369d:	mov    (%rax),%ecx
+    646c369f:	mov    0x8a2a(%rip),%rdx        # 646cc0d0 <flatten_temp>
+    646c36a6:	mov    0x8a83(%rip),%rax        # 646cc130 <pdist_temp>
+    646c36ad:	mov    %r8,%r9
+    646c36b0:	mov    %ecx,%r8d
+    646c36b3:	mov    %rax,%rcx
+    646c36b6:	call   646c302e <cov_model2d>
+    646c36bb:	mov    0x18(%rbp),%rax
+    646c36bf:	mov    (%rax),%ecx
+    646c36c1:	mov    0x8a88(%rip),%rdx        # 646cc150 <datacov>
+    646c36c8:	mov    0x8a01(%rip),%rax        # 646cc0d0 <flatten_temp>
+    646c36cf:	mov    %ecx,%r8d
+    646c36d2:	mov    %rax,%rcx
+    646c36d5:	call   646c4490 <matrixform>
+    646c36da:	mov    0x893f(%rip),%r8        # 646cc020 <model>
+    646c36e1:	mov    0x18(%rbp),%rax
+    646c36e5:	mov    (%rax),%ecx
+    646c36e7:	mov    0x8982(%rip),%rdx        # 646cc070 <loc_cov>
+    646c36ee:	mov    0x89bb(%rip),%rax        # 646cc0b0 <loc_cov2>
+    646c36f5:	mov    %r8,%r9
+    646c36f8:	mov    %ecx,%r8d
+    646c36fb:	mov    %rax,%rcx
+    646c36fe:	call   646c2f24 <cov_model>
+    646c3703:	mov    0x18(%rbp),%rax
+    646c3707:	mov    (%rax),%eax
+    646c3709:	test   %eax,%eax
+    646c370b:	jle    646c3737 <simple_kriging+0x27e>
+    646c370d:	mov    0x18(%rbp),%rax
+    646c3711:	mov    (%rax),%r8d
+    646c3714:	mov    0x89d5(%rip),%rcx        # 646cc0f0 <weights>
+    646c371b:	mov    0x894e(%rip),%rdx        # 646cc070 <loc_cov>
+    646c3722:	mov    0x8a27(%rip),%rax        # 646cc150 <datacov>
+    646c3729:	mov    %r8d,%r9d
+    646c372c:	mov    %rcx,%r8
+    646c372f:	mov    %rax,%rcx
+    646c3732:	call   646c3c1a <lu_inverse_solver>
+    646c3737:	pxor   %xmm0,%xmm0
+    646c373b:	movsd  %xmm0,0x88ed(%rip)        # 646cc030 <estimation>
+    646c3743:	pxor   %xmm0,%xmm0
+    646c3747:	movsd  %xmm0,0x88e9(%rip)        # 646cc038 <krige_var>
+    646c374f:	pxor   %xmm0,%xmm0
+    646c3753:	movsd  %xmm0,0x88e5(%rip)        # 646cc040 <fix>
+    646c375b:	movl   $0x0,-0x1c(%rbp)
+    646c3762:	jmp    646c37fe <simple_kriging+0x345>
+    646c3767:	mov    0x89a2(%rip),%rdx        # 646cc110 <array2d_temp>
+    646c376e:	mov    -0x1c(%rbp),%eax
+    646c3771:	cltq
+    646c3773:	shl    $0x3,%rax
+    646c3777:	add    %rdx,%rax
+    646c377a:	mov    (%rax),%rax
+    646c377d:	add    $0x8,%rax
+    646c3781:	movsd  (%rax),%xmm1
+    646c3785:	mov    0x8964(%rip),%rdx        # 646cc0f0 <weights>
+    646c378c:	mov    -0x1c(%rbp),%eax
+    646c378f:	cltq
+    646c3791:	shl    $0x3,%rax
+    646c3795:	add    %rdx,%rax
+    646c3798:	movsd  (%rax),%xmm0
+    646c379c:	mulsd  %xmm0,%xmm1
+    646c37a0:	movsd  0x8888(%rip),%xmm0        # 646cc030 <estimation>
+    646c37a8:	addsd  %xmm1,%xmm0
+    646c37ac:	movsd  %xmm0,0x887c(%rip)        # 646cc030 <estimation>
+    646c37b4:	mov    0x88b5(%rip),%rdx        # 646cc070 <loc_cov>
+    646c37bb:	mov    -0x1c(%rbp),%eax
+    646c37be:	cltq
+    646c37c0:	shl    $0x3,%rax
+    646c37c4:	add    %rdx,%rax
+    646c37c7:	movsd  (%rax),%xmm1
+    646c37cb:	mov    0x891e(%rip),%rdx        # 646cc0f0 <weights>
+    646c37d2:	mov    -0x1c(%rbp),%eax
+    646c37d5:	cltq
+    646c37d7:	shl    $0x3,%rax
+    646c37db:	add    %rdx,%rax
+    646c37de:	movsd  (%rax),%xmm0
+    646c37e2:	mulsd  %xmm0,%xmm1
+    646c37e6:	movsd  0x884a(%rip),%xmm0        # 646cc038 <krige_var>
+    646c37ee:	addsd  %xmm1,%xmm0
+    646c37f2:	movsd  %xmm0,0x883e(%rip)        # 646cc038 <krige_var>
+    646c37fa:	addl   $0x1,-0x1c(%rbp)
+    646c37fe:	mov    0x18(%rbp),%rax
+    646c3802:	mov    (%rax),%eax
+    646c3804:	cmp    %eax,-0x1c(%rbp)
+    646c3807:	jl     646c3767 <simple_kriging+0x2ae>
+    646c380d:	mov    0x880c(%rip),%rax        # 646cc020 <model>
+    646c3814:	movsd  0x18(%rax),%xmm0
+    646c3819:	movsd  0x8817(%rip),%xmm1        # 646cc038 <krige_var>
+    646c3821:	subsd  %xmm1,%xmm0
+    646c3825:	movsd  %xmm0,0x880b(%rip)        # 646cc038 <krige_var>
+    646c382d:	movsd  0x8803(%rip),%xmm1        # 646cc038 <krige_var>
+    646c3835:	pxor   %xmm0,%xmm0
+    646c3839:	comisd %xmm1,%xmm0
+    646c383d:	jbe    646c384b <simple_kriging+0x392>
+    646c383f:	pxor   %xmm0,%xmm0
+    646c3843:	movsd  %xmm0,0x87ed(%rip)        # 646cc038 <krige_var>
+    646c384b:	mov    0x20(%rbp),%rax
+    646c384f:	mov    %rax,%rcx
+    646c3852:	call   646c2e27 <mt19937_random_normal>
+    646c3857:	movapd %xmm0,%xmm6
+    646c385b:	mov    0x87d6(%rip),%rax        # 646cc038 <krige_var>
+    646c3862:	movsd  0x57f6(%rip),%xmm0        # 646c9060 <.rdata>
+    646c386a:	movapd %xmm0,%xmm1
+    646c386e:	movq   %rax,%xmm0
+    646c3873:	call   646c6f60 <pow>
+    646c3878:	mulsd  %xmm6,%xmm0
+    646c387c:	movsd  %xmm0,0x87bc(%rip)        # 646cc040 <fix>
+    646c3884:	movsd  0x87a4(%rip),%xmm1        # 646cc030 <estimation>
+    646c388c:	movsd  0x87ac(%rip),%xmm0        # 646cc040 <fix>
+    646c3894:	mov    0x18(%rbp),%rax
+    646c3898:	movsd  0x10(%rax),%xmm2
+    646c389d:	cvttsd2si %xmm2,%eax
+    646c38a1:	cltq
+    646c38a3:	lea    0x0(,%rax,8),%rdx
+    646c38ab:	mov    0x10(%rbp),%rax
+    646c38af:	add    %rdx,%rax
+    646c38b2:	addsd  %xmm1,%xmm0
+    646c38b6:	movsd  %xmm0,(%rax)
+    646c38ba:	jmp    646c38bd <simple_kriging+0x404>
+    646c38bc:	nop
+    646c38bd:	movaps -0x10(%rbp),%xmm6
+    646c38c1:	add    $0x40,%rsp
+    646c38c5:	pop    %rbp
+    646c38c6:	ret
+
+00000000646c38c7 <find_neighbor>:
+    646c38c7:	push   %rbp
+    646c38c8:	mov    %rsp,%rbp
+    646c38cb:	sub    $0x30,%rsp
+    646c38cf:	mov    %rcx,0x10(%rbp)
+    646c38d3:	mov    %rdx,0x18(%rbp)
+    646c38d7:	mov    %r8,0x20(%rbp)
+    646c38db:	mov    0x18(%rbp),%rax
+    646c38df:	mov    (%rax),%eax
+    646c38e1:	test   %eax,%eax
+    646c38e3:	jne    646c3956 <find_neighbor+0x8f>
+    646c38e5:	mov    0x20(%rbp),%rax
+    646c38e9:	mov    %rax,%rcx
+    646c38ec:	call   646c2e27 <mt19937_random_normal>
+    646c38f1:	movapd %xmm0,%xmm1
+    646c38f5:	mov    0x8724(%rip),%rax        # 646cc020 <model>
+    646c38fc:	movsd  0x18(%rax),%xmm0
+    646c3901:	mov    0x18(%rbp),%rax
+    646c3905:	movsd  0x10(%rax),%xmm2
+    646c390a:	cvttsd2si %xmm2,%eax
+    646c390e:	cltq
+    646c3910:	lea    0x0(,%rax,8),%rdx
+    646c3918:	mov    0x10(%rbp),%rax
+    646c391c:	add    %rdx,%rax
+    646c391f:	mulsd  %xmm1,%xmm0
+    646c3923:	movsd  %xmm0,(%rax)
+    646c3927:	mov    0x18(%rbp),%rax
+    646c392b:	mov    0x18(%rax),%rdx
+    646c392f:	mov    0x18(%rbp),%rax
+    646c3933:	mov    0x8(%rax),%eax
+    646c3936:	cltq
+    646c3938:	shl    $0x3,%rax
+    646c393c:	add    %rdx,%rax
+    646c393f:	mov    0x18(%rbp),%rdx
+    646c3943:	movsd  0x10(%rdx),%xmm0
+    646c3948:	movsd  %xmm0,(%rax)
+    646c394c:	mov    $0x0,%eax
+    646c3951:	jmp    646c3a75 <find_neighbor+0x1ae>
+    646c3956:	movl   $0x0,-0x4(%rbp)
+    646c395d:	movl   $0x0,-0x8(%rbp)
+    646c3964:	jmp    646c39ec <find_neighbor+0x125>
+    646c3969:	mov    0x18(%rbp),%rax
+    646c396d:	mov    0x18(%rax),%rdx
+    646c3971:	mov    -0x8(%rbp),%eax
+    646c3974:	cltq
+    646c3976:	shl    $0x3,%rax
+    646c397a:	add    %rdx,%rax
+    646c397d:	movsd  (%rax),%xmm0
+    646c3981:	mov    0x18(%rbp),%rax
+    646c3985:	movsd  0x10(%rax),%xmm1
+    646c398a:	subsd  %xmm1,%xmm0
+    646c398e:	mov    0x18(%rbp),%rax
+    646c3992:	mov    0x30(%rax),%rdx
+    646c3996:	mov    -0x8(%rbp),%eax
+    646c3999:	cltq
+    646c399b:	shl    $0x3,%rax
+    646c399f:	add    %rdx,%rax
+    646c39a2:	movq   0x56c6(%rip),%xmm1        # 646c9070 <.rdata+0x10>
+    646c39aa:	andpd  %xmm1,%xmm0
+    646c39ae:	movsd  %xmm0,(%rax)
+    646c39b2:	mov    0x18(%rbp),%rax
+    646c39b6:	mov    0x30(%rax),%rdx
+    646c39ba:	mov    -0x8(%rbp),%eax
+    646c39bd:	cltq
+    646c39bf:	shl    $0x3,%rax
+    646c39c3:	add    %rdx,%rax
+    646c39c6:	movsd  (%rax),%xmm1
+    646c39ca:	movsd  0x8656(%rip),%xmm2        # 646cc028 <k_range>
+    646c39d2:	movsd  0x56a6(%rip),%xmm0        # 646c9080 <.rdata+0x20>
+    646c39da:	mulsd  %xmm2,%xmm0
+    646c39de:	comisd %xmm1,%xmm0
+    646c39e2:	jbe    646c39e8 <find_neighbor+0x121>
+    646c39e4:	addl   $0x1,-0x4(%rbp)
+    646c39e8:	addl   $0x1,-0x8(%rbp)
+    646c39ec:	mov    0x18(%rbp),%rax
+    646c39f0:	mov    0x4(%rax),%eax
+    646c39f3:	cmp    %eax,-0x8(%rbp)
+    646c39f6:	jl     646c3969 <find_neighbor+0xa2>
+    646c39fc:	cmpl   $0x0,-0x4(%rbp)
+    646c3a00:	jne    646c3a70 <find_neighbor+0x1a9>
+    646c3a02:	mov    0x20(%rbp),%rax
+    646c3a06:	mov    %rax,%rcx
+    646c3a09:	call   646c2e27 <mt19937_random_normal>
+    646c3a0e:	movapd %xmm0,%xmm1
+    646c3a12:	mov    0x8607(%rip),%rax        # 646cc020 <model>
+    646c3a19:	movsd  0x18(%rax),%xmm0
+    646c3a1e:	mov    0x18(%rbp),%rax
+    646c3a22:	movsd  0x10(%rax),%xmm2
+    646c3a27:	cvttsd2si %xmm2,%eax
+    646c3a2b:	cltq
+    646c3a2d:	lea    0x0(,%rax,8),%rdx
+    646c3a35:	mov    0x10(%rbp),%rax
+    646c3a39:	add    %rdx,%rax
+    646c3a3c:	mulsd  %xmm1,%xmm0
+    646c3a40:	movsd  %xmm0,(%rax)
+    646c3a44:	mov    0x18(%rbp),%rax
+    646c3a48:	mov    0x18(%rax),%rdx
+    646c3a4c:	mov    0x18(%rbp),%rax
+    646c3a50:	mov    0x8(%rax),%eax
+    646c3a53:	cltq
+    646c3a55:	shl    $0x3,%rax
+    646c3a59:	add    %rdx,%rax
+    646c3a5c:	mov    0x18(%rbp),%rdx
+    646c3a60:	movsd  0x10(%rdx),%xmm0
+    646c3a65:	movsd  %xmm0,(%rax)
+    646c3a69:	mov    $0x0,%eax
+    646c3a6e:	jmp    646c3a75 <find_neighbor+0x1ae>
+    646c3a70:	mov    $0x1,%eax
+    646c3a75:	add    $0x30,%rsp
+    646c3a79:	pop    %rbp
+    646c3a7a:	ret
+
+00000000646c3a7b <krige_memory_free>:
+    646c3a7b:	push   %rbp
+    646c3a7c:	mov    %rsp,%rbp
+    646c3a7f:	sub    $0x30,%rsp
+    646c3a83:	mov    0x85c6(%rip),%rax        # 646cc050 <location>
+    646c3a8a:	mov    %rax,%rcx
+    646c3a8d:	call   646c7988 <free>
+    646c3a92:	mov    0x85d7(%rip),%rax        # 646cc070 <loc_cov>
+    646c3a99:	mov    %rax,%rcx
+    646c3a9c:	call   646c7988 <free>
+    646c3aa1:	mov    0x85e8(%rip),%rax        # 646cc090 <data_temp>
+    646c3aa8:	mov    %rax,%rcx
+    646c3aab:	call   646c7988 <free>
+    646c3ab0:	mov    0x85f9(%rip),%rax        # 646cc0b0 <loc_cov2>
+    646c3ab7:	mov    %rax,%rcx
+    646c3aba:	call   646c7988 <free>
+    646c3abf:	mov    0x860a(%rip),%rax        # 646cc0d0 <flatten_temp>
+    646c3ac6:	mov    %rax,%rcx
+    646c3ac9:	call   646c7988 <free>
+    646c3ace:	mov    0x861b(%rip),%rax        # 646cc0f0 <weights>
+    646c3ad5:	mov    %rax,%rcx
+    646c3ad8:	call   646c7988 <free>
+    646c3add:	movl   $0x0,-0x4(%rbp)
+    646c3ae4:	jmp    646c3b08 <krige_memory_free+0x8d>
+    646c3ae6:	mov    0x8623(%rip),%rdx        # 646cc110 <array2d_temp>
+    646c3aed:	mov    -0x4(%rbp),%eax
+    646c3af0:	cltq
+    646c3af2:	shl    $0x3,%rax
+    646c3af6:	add    %rdx,%rax
+    646c3af9:	mov    (%rax),%rax
+    646c3afc:	mov    %rax,%rcx
+    646c3aff:	call   646c7988 <free>
+    646c3b04:	addl   $0x1,-0x4(%rbp)
+    646c3b08:	mov    -0x4(%rbp),%eax
+    646c3b0b:	cltq
+    646c3b0d:	mov    0x8604(%rip),%rdx        # 646cc118 <array2d_temp+0x8>
+    646c3b14:	cmp    %rdx,%rax
+    646c3b17:	jb     646c3ae6 <krige_memory_free+0x6b>
+    646c3b19:	mov    0x85f0(%rip),%rax        # 646cc110 <array2d_temp>
+    646c3b20:	mov    %rax,%rcx
+    646c3b23:	call   646c7988 <free>
+    646c3b28:	movl   $0x0,-0x8(%rbp)
+    646c3b2f:	jmp    646c3b53 <krige_memory_free+0xd8>
+    646c3b31:	mov    0x85f8(%rip),%rdx        # 646cc130 <pdist_temp>
+    646c3b38:	mov    -0x8(%rbp),%eax
+    646c3b3b:	cltq
+    646c3b3d:	shl    $0x3,%rax
+    646c3b41:	add    %rdx,%rax
+    646c3b44:	mov    (%rax),%rax
+    646c3b47:	mov    %rax,%rcx
+    646c3b4a:	call   646c7988 <free>
+    646c3b4f:	addl   $0x1,-0x8(%rbp)
+    646c3b53:	mov    -0x8(%rbp),%eax
+    646c3b56:	cltq
+    646c3b58:	mov    0x85d9(%rip),%rdx        # 646cc138 <pdist_temp+0x8>
+    646c3b5f:	cmp    %rdx,%rax
+    646c3b62:	jb     646c3b31 <krige_memory_free+0xb6>
+    646c3b64:	mov    0x85c5(%rip),%rax        # 646cc130 <pdist_temp>
+    646c3b6b:	mov    %rax,%rcx
+    646c3b6e:	call   646c7988 <free>
+    646c3b73:	movl   $0x0,-0xc(%rbp)
+    646c3b7a:	jmp    646c3b9e <krige_memory_free+0x123>
+    646c3b7c:	mov    0x85cd(%rip),%rdx        # 646cc150 <datacov>
+    646c3b83:	mov    -0xc(%rbp),%eax
+    646c3b86:	cltq
+    646c3b88:	shl    $0x3,%rax
+    646c3b8c:	add    %rdx,%rax
+    646c3b8f:	mov    (%rax),%rax
+    646c3b92:	mov    %rax,%rcx
+    646c3b95:	call   646c7988 <free>
+    646c3b9a:	addl   $0x1,-0xc(%rbp)
+    646c3b9e:	mov    -0xc(%rbp),%eax
+    646c3ba1:	cltq
+    646c3ba3:	mov    0x85ae(%rip),%rdx        # 646cc158 <datacov+0x8>
+    646c3baa:	cmp    %rdx,%rax
+    646c3bad:	jb     646c3b7c <krige_memory_free+0x101>
+    646c3baf:	mov    0x859a(%rip),%rax        # 646cc150 <datacov>
+    646c3bb6:	mov    %rax,%rcx
+    646c3bb9:	call   646c7988 <free>
+    646c3bbe:	nop
+    646c3bbf:	add    $0x30,%rsp
+    646c3bc3:	pop    %rbp
+    646c3bc4:	ret
+    646c3bc5:	nop
+    646c3bc6:	nop
+    646c3bc7:	nop
+    646c3bc8:	nop
+    646c3bc9:	nop
+    646c3bca:	nop
+    646c3bcb:	nop
+    646c3bcc:	nop
+    646c3bcd:	nop
+    646c3bce:	nop
+    646c3bcf:	nop
+
+00000000646c3bd0 <snprintf>:
+    646c3bd0:	push   %rbp
+    646c3bd1:	mov    %rsp,%rbp
+    646c3bd4:	sub    $0x30,%rsp
+    646c3bd8:	mov    %rcx,0x10(%rbp)
+    646c3bdc:	mov    %rdx,0x18(%rbp)
+    646c3be0:	mov    %r8,0x20(%rbp)
+    646c3be4:	mov    %r9,0x28(%rbp)
+    646c3be8:	lea    0x28(%rbp),%rax
+    646c3bec:	mov    %rax,-0x10(%rbp)
+    646c3bf0:	mov    -0x10(%rbp),%rcx
+    646c3bf4:	mov    0x20(%rbp),%rdx
+    646c3bf8:	mov    0x18(%rbp),%rax
+    646c3bfc:	mov    %rcx,%r9
+    646c3bff:	mov    %rdx,%r8
+    646c3c02:	mov    %rax,%rdx
+    646c3c05:	mov    0x10(%rbp),%rcx
+    646c3c09:	call   646c6990 <__ms_vsnprintf>
+    646c3c0e:	mov    %eax,-0x4(%rbp)
+    646c3c11:	mov    -0x4(%rbp),%eax
+    646c3c14:	add    $0x30,%rsp
+    646c3c18:	pop    %rbp
+    646c3c19:	ret
+
+00000000646c3c1a <lu_inverse_solver>:
+    646c3c1a:	push   %rbp
+    646c3c1b:	push   %rbx
+    646c3c1c:	sub    $0xd8,%rsp
+    646c3c23:	lea    0x80(%rsp),%rbp
+    646c3c2b:	mov    %rcx,0x70(%rbp)
+    646c3c2f:	mov    %rdx,0x78(%rbp)
+    646c3c33:	mov    %r8,0x80(%rbp)
+    646c3c3a:	mov    %r9d,0x88(%rbp)
+    646c3c41:	movq   $0xa,0x18(%rbp)
+    646c3c49:	movq   $0xa,0x20(%rbp)
+    646c3c51:	mov    $0x50,%ecx
+    646c3c56:	call   646c7970 <malloc>
+    646c3c5b:	mov    %rax,0x10(%rbp)
+    646c3c5f:	movl   $0x0,0x4c(%rbp)
+    646c3c66:	jmp    646c3c8a <lu_inverse_solver+0x70>
+    646c3c68:	mov    0x10(%rbp),%rdx
+    646c3c6c:	mov    0x4c(%rbp),%eax
+    646c3c6f:	cltq
+    646c3c71:	shl    $0x3,%rax
+    646c3c75:	lea    (%rdx,%rax,1),%rbx
+    646c3c79:	mov    $0x50,%ecx
+    646c3c7e:	call   646c7970 <malloc>
+    646c3c83:	mov    %rax,(%rbx)
+    646c3c86:	addl   $0x1,0x4c(%rbp)
+    646c3c8a:	cmpl   $0x9,0x4c(%rbp)
+    646c3c8e:	jle    646c3c68 <lu_inverse_solver+0x4e>
+    646c3c90:	movq   $0xa,-0x8(%rbp)
+    646c3c98:	movq   $0xa,0x0(%rbp)
+    646c3ca0:	mov    $0x50,%ecx
+    646c3ca5:	call   646c7970 <malloc>
+    646c3caa:	mov    %rax,-0x10(%rbp)
+    646c3cae:	movl   $0x0,0x48(%rbp)
+    646c3cb5:	jmp    646c3cd9 <lu_inverse_solver+0xbf>
+    646c3cb7:	mov    -0x10(%rbp),%rdx
+    646c3cbb:	mov    0x48(%rbp),%eax
+    646c3cbe:	cltq
+    646c3cc0:	shl    $0x3,%rax
+    646c3cc4:	lea    (%rdx,%rax,1),%rbx
+    646c3cc8:	mov    $0x50,%ecx
+    646c3ccd:	call   646c7970 <malloc>
+    646c3cd2:	mov    %rax,(%rbx)
+    646c3cd5:	addl   $0x1,0x48(%rbp)
+    646c3cd9:	cmpl   $0x9,0x48(%rbp)
+    646c3cdd:	jle    646c3cb7 <lu_inverse_solver+0x9d>
+    646c3cdf:	mov    -0x10(%rbp),%rdx
+    646c3ce3:	mov    0x10(%rbp),%rax
+    646c3ce7:	mov    0x88(%rbp),%ecx
+    646c3ced:	mov    %ecx,%r9d
+    646c3cf0:	mov    %rdx,%r8
+    646c3cf3:	mov    %rax,%rdx
+    646c3cf6:	mov    0x70(%rbp),%rcx
+    646c3cfa:	call   646c3f98 <lu_decomposition>
+    646c3cff:	mov    0x78(%rbp),%rax
+    646c3d03:	movsd  (%rax),%xmm0
+    646c3d07:	mov    0x10(%rbp),%rax
+    646c3d0b:	mov    (%rax),%rax
+    646c3d0e:	movsd  (%rax),%xmm1
+    646c3d12:	divsd  %xmm1,%xmm0
+    646c3d16:	movsd  %xmm0,-0x60(%rbp)
+    646c3d1b:	movl   $0x1,0x44(%rbp)
+    646c3d22:	jmp    646c3dec <lu_inverse_solver+0x1d2>
+    646c3d27:	mov    0x44(%rbp),%eax
+    646c3d2a:	cltq
+    646c3d2c:	lea    0x0(,%rax,8),%rdx
+    646c3d34:	mov    0x78(%rbp),%rax
+    646c3d38:	add    %rdx,%rax
+    646c3d3b:	movsd  (%rax),%xmm0
+    646c3d3f:	mov    0x44(%rbp),%eax
+    646c3d42:	cltq
+    646c3d44:	movsd  %xmm0,-0x60(%rbp,%rax,8)
+    646c3d4a:	movl   $0x0,0x40(%rbp)
+    646c3d51:	jmp    646c3da3 <lu_inverse_solver+0x189>
+    646c3d53:	mov    0x44(%rbp),%eax
+    646c3d56:	cltq
+    646c3d58:	movsd  -0x60(%rbp,%rax,8),%xmm0
+    646c3d5e:	mov    0x10(%rbp),%rdx
+    646c3d62:	mov    0x44(%rbp),%eax
+    646c3d65:	cltq
+    646c3d67:	shl    $0x3,%rax
+    646c3d6b:	add    %rdx,%rax
+    646c3d6e:	mov    (%rax),%rdx
+    646c3d71:	mov    0x40(%rbp),%eax
+    646c3d74:	cltq
+    646c3d76:	shl    $0x3,%rax
+    646c3d7a:	add    %rdx,%rax
+    646c3d7d:	movsd  (%rax),%xmm2
+    646c3d81:	mov    0x40(%rbp),%eax
+    646c3d84:	cltq
+    646c3d86:	movsd  -0x60(%rbp,%rax,8),%xmm1
+    646c3d8c:	mulsd  %xmm2,%xmm1
+    646c3d90:	subsd  %xmm1,%xmm0
+    646c3d94:	mov    0x44(%rbp),%eax
+    646c3d97:	cltq
+    646c3d99:	movsd  %xmm0,-0x60(%rbp,%rax,8)
+    646c3d9f:	addl   $0x1,0x40(%rbp)
+    646c3da3:	mov    0x40(%rbp),%eax
+    646c3da6:	cmp    0x44(%rbp),%eax
+    646c3da9:	jl     646c3d53 <lu_inverse_solver+0x139>
+    646c3dab:	mov    0x44(%rbp),%eax
+    646c3dae:	cltq
+    646c3db0:	movsd  -0x60(%rbp,%rax,8),%xmm0
+    646c3db6:	mov    0x10(%rbp),%rdx
+    646c3dba:	mov    0x44(%rbp),%eax
+    646c3dbd:	cltq
+    646c3dbf:	shl    $0x3,%rax
+    646c3dc3:	add    %rdx,%rax
+    646c3dc6:	mov    (%rax),%rdx
+    646c3dc9:	mov    0x44(%rbp),%eax
+    646c3dcc:	cltq
+    646c3dce:	shl    $0x3,%rax
+    646c3dd2:	add    %rdx,%rax
+    646c3dd5:	movsd  (%rax),%xmm1
+    646c3dd9:	divsd  %xmm1,%xmm0
+    646c3ddd:	mov    0x44(%rbp),%eax
+    646c3de0:	cltq
+    646c3de2:	movsd  %xmm0,-0x60(%rbp,%rax,8)
+    646c3de8:	addl   $0x1,0x44(%rbp)
+    646c3dec:	mov    0x44(%rbp),%eax
+    646c3def:	cmp    0x88(%rbp),%eax
+    646c3df5:	jl     646c3d27 <lu_inverse_solver+0x10d>
+    646c3dfb:	mov    0x88(%rbp),%eax
+    646c3e01:	cltq
+    646c3e03:	lea    0x0(,%rax,8),%rdx
+    646c3e0b:	mov    0x80(%rbp),%rax
+    646c3e12:	add    %rax,%rdx
+    646c3e15:	mov    0x88(%rbp),%eax
+    646c3e1b:	cltq
+    646c3e1d:	movsd  -0x60(%rbp,%rax,8),%xmm0
+    646c3e23:	movsd  %xmm0,(%rdx)
+    646c3e27:	mov    0x88(%rbp),%eax
+    646c3e2d:	sub    $0x1,%eax
+    646c3e30:	mov    %eax,0x3c(%rbp)
+    646c3e33:	jmp    646c3eff <lu_inverse_solver+0x2e5>
+    646c3e38:	mov    0x3c(%rbp),%eax
+    646c3e3b:	cltq
+    646c3e3d:	lea    0x0(,%rax,8),%rdx
+    646c3e45:	mov    0x80(%rbp),%rax
+    646c3e4c:	add    %rax,%rdx
+    646c3e4f:	mov    0x3c(%rbp),%eax
+    646c3e52:	cltq
+    646c3e54:	movsd  -0x60(%rbp,%rax,8),%xmm0
+    646c3e5a:	movsd  %xmm0,(%rdx)
+    646c3e5e:	mov    0x3c(%rbp),%eax
+    646c3e61:	add    $0x1,%eax
+    646c3e64:	mov    %eax,0x38(%rbp)
+    646c3e67:	jmp    646c3eec <lu_inverse_solver+0x2d2>
+    646c3e6c:	mov    0x3c(%rbp),%eax
+    646c3e6f:	cltq
+    646c3e71:	lea    0x0(,%rax,8),%rdx
+    646c3e79:	mov    0x80(%rbp),%rax
+    646c3e80:	add    %rdx,%rax
+    646c3e83:	movsd  (%rax),%xmm0
+    646c3e87:	mov    -0x10(%rbp),%rdx
+    646c3e8b:	mov    0x3c(%rbp),%eax
+    646c3e8e:	cltq
+    646c3e90:	shl    $0x3,%rax
+    646c3e94:	add    %rdx,%rax
+    646c3e97:	mov    (%rax),%rdx
+    646c3e9a:	mov    0x38(%rbp),%eax
+    646c3e9d:	cltq
+    646c3e9f:	shl    $0x3,%rax
+    646c3ea3:	add    %rdx,%rax
+    646c3ea6:	movsd  (%rax),%xmm2
+    646c3eaa:	mov    0x38(%rbp),%eax
+    646c3ead:	cltq
+    646c3eaf:	lea    0x0(,%rax,8),%rdx
+    646c3eb7:	mov    0x80(%rbp),%rax
+    646c3ebe:	add    %rdx,%rax
+    646c3ec1:	movsd  (%rax),%xmm1
+    646c3ec5:	mulsd  %xmm2,%xmm1
+    646c3ec9:	mov    0x3c(%rbp),%eax
+    646c3ecc:	cltq
+    646c3ece:	lea    0x0(,%rax,8),%rdx
+    646c3ed6:	mov    0x80(%rbp),%rax
+    646c3edd:	add    %rdx,%rax
+    646c3ee0:	subsd  %xmm1,%xmm0
+    646c3ee4:	movsd  %xmm0,(%rax)
+    646c3ee8:	addl   $0x1,0x38(%rbp)
+    646c3eec:	mov    0x38(%rbp),%eax
+    646c3eef:	cmp    0x88(%rbp),%eax
+    646c3ef5:	jl     646c3e6c <lu_inverse_solver+0x252>
+    646c3efb:	subl   $0x1,0x3c(%rbp)
+    646c3eff:	cmpl   $0x0,0x3c(%rbp)
+    646c3f03:	jns    646c3e38 <lu_inverse_solver+0x21e>
+    646c3f09:	movl   $0x0,0x34(%rbp)
+    646c3f10:	jmp    646c3f31 <lu_inverse_solver+0x317>
+    646c3f12:	mov    0x10(%rbp),%rdx
+    646c3f16:	mov    0x34(%rbp),%eax
+    646c3f19:	cltq
+    646c3f1b:	shl    $0x3,%rax
+    646c3f1f:	add    %rdx,%rax
+    646c3f22:	mov    (%rax),%rax
+    646c3f25:	mov    %rax,%rcx
+    646c3f28:	call   646c7988 <free>
+    646c3f2d:	addl   $0x1,0x34(%rbp)
+    646c3f31:	mov    0x34(%rbp),%eax
+    646c3f34:	cltq
+    646c3f36:	mov    0x18(%rbp),%rdx
+    646c3f3a:	cmp    %rdx,%rax
+    646c3f3d:	jb     646c3f12 <lu_inverse_solver+0x2f8>
+    646c3f3f:	mov    0x10(%rbp),%rax
+    646c3f43:	mov    %rax,%rcx
+    646c3f46:	call   646c7988 <free>
+    646c3f4b:	movl   $0x0,0x30(%rbp)
+    646c3f52:	jmp    646c3f73 <lu_inverse_solver+0x359>
+    646c3f54:	mov    -0x10(%rbp),%rdx
+    646c3f58:	mov    0x30(%rbp),%eax
+    646c3f5b:	cltq
+    646c3f5d:	shl    $0x3,%rax
+    646c3f61:	add    %rdx,%rax
+    646c3f64:	mov    (%rax),%rax
+    646c3f67:	mov    %rax,%rcx
+    646c3f6a:	call   646c7988 <free>
+    646c3f6f:	addl   $0x1,0x30(%rbp)
+    646c3f73:	mov    0x30(%rbp),%eax
+    646c3f76:	cltq
+    646c3f78:	mov    -0x8(%rbp),%rdx
+    646c3f7c:	cmp    %rdx,%rax
+    646c3f7f:	jb     646c3f54 <lu_inverse_solver+0x33a>
+    646c3f81:	mov    -0x10(%rbp),%rax
+    646c3f85:	mov    %rax,%rcx
+    646c3f88:	call   646c7988 <free>
+    646c3f8d:	nop
+    646c3f8e:	add    $0xd8,%rsp
+    646c3f95:	pop    %rbx
+    646c3f96:	pop    %rbp
+    646c3f97:	ret
+
+00000000646c3f98 <lu_decomposition>:
+    646c3f98:	push   %rbp
+    646c3f99:	mov    %rsp,%rbp
+    646c3f9c:	sub    $0x20,%rsp
+    646c3fa0:	mov    %rcx,0x10(%rbp)
+    646c3fa4:	mov    %rdx,0x18(%rbp)
+    646c3fa8:	mov    %r8,0x20(%rbp)
+    646c3fac:	mov    %r9d,0x28(%rbp)
+    646c3fb0:	movl   $0x0,-0x4(%rbp)
+    646c3fb7:	jmp    646c4316 <lu_decomposition+0x37e>
+    646c3fbc:	movl   $0x0,-0x8(%rbp)
+    646c3fc3:	jmp    646c4112 <lu_decomposition+0x17a>
+    646c3fc8:	mov    -0x8(%rbp),%eax
+    646c3fcb:	cmp    -0x4(%rbp),%eax
+    646c3fce:	jge    646c4000 <lu_decomposition+0x68>
+    646c3fd0:	mov    -0x8(%rbp),%eax
+    646c3fd3:	cltq
+    646c3fd5:	lea    0x0(,%rax,8),%rdx
+    646c3fdd:	mov    0x18(%rbp),%rax
+    646c3fe1:	add    %rdx,%rax
+    646c3fe4:	mov    (%rax),%rdx
+    646c3fe7:	mov    -0x4(%rbp),%eax
+    646c3fea:	cltq
+    646c3fec:	shl    $0x3,%rax
+    646c3ff0:	add    %rdx,%rax
+    646c3ff3:	pxor   %xmm0,%xmm0
+    646c3ff7:	movsd  %xmm0,(%rax)
+    646c3ffb:	jmp    646c410e <lu_decomposition+0x176>
+    646c4000:	mov    -0x8(%rbp),%eax
+    646c4003:	cltq
+    646c4005:	lea    0x0(,%rax,8),%rdx
+    646c400d:	mov    0x10(%rbp),%rax
+    646c4011:	add    %rdx,%rax
+    646c4014:	mov    (%rax),%rdx
+    646c4017:	mov    -0x4(%rbp),%eax
+    646c401a:	cltq
+    646c401c:	shl    $0x3,%rax
+    646c4020:	add    %rax,%rdx
+    646c4023:	mov    -0x8(%rbp),%eax
+    646c4026:	cltq
+    646c4028:	lea    0x0(,%rax,8),%rcx
+    646c4030:	mov    0x18(%rbp),%rax
+    646c4034:	add    %rcx,%rax
+    646c4037:	mov    (%rax),%rcx
+    646c403a:	mov    -0x4(%rbp),%eax
+    646c403d:	cltq
+    646c403f:	shl    $0x3,%rax
+    646c4043:	add    %rcx,%rax
+    646c4046:	movsd  (%rdx),%xmm0
+    646c404a:	movsd  %xmm0,(%rax)
+    646c404e:	movl   $0x0,-0xc(%rbp)
+    646c4055:	jmp    646c4102 <lu_decomposition+0x16a>
+    646c405a:	mov    -0x8(%rbp),%eax
+    646c405d:	cltq
+    646c405f:	lea    0x0(,%rax,8),%rdx
+    646c4067:	mov    0x18(%rbp),%rax
+    646c406b:	add    %rdx,%rax
+    646c406e:	mov    (%rax),%rdx
+    646c4071:	mov    -0x4(%rbp),%eax
+    646c4074:	cltq
+    646c4076:	shl    $0x3,%rax
+    646c407a:	add    %rdx,%rax
+    646c407d:	movsd  (%rax),%xmm0
+    646c4081:	mov    -0x8(%rbp),%eax
+    646c4084:	cltq
+    646c4086:	lea    0x0(,%rax,8),%rdx
+    646c408e:	mov    0x18(%rbp),%rax
+    646c4092:	add    %rdx,%rax
+    646c4095:	mov    (%rax),%rdx
+    646c4098:	mov    -0xc(%rbp),%eax
+    646c409b:	cltq
+    646c409d:	shl    $0x3,%rax
+    646c40a1:	add    %rdx,%rax
+    646c40a4:	movsd  (%rax),%xmm2
+    646c40a8:	mov    -0xc(%rbp),%eax
+    646c40ab:	cltq
+    646c40ad:	lea    0x0(,%rax,8),%rdx
+    646c40b5:	mov    0x20(%rbp),%rax
+    646c40b9:	add    %rdx,%rax
+    646c40bc:	mov    (%rax),%rdx
+    646c40bf:	mov    -0x4(%rbp),%eax
+    646c40c2:	cltq
+    646c40c4:	shl    $0x3,%rax
+    646c40c8:	add    %rdx,%rax
+    646c40cb:	movsd  (%rax),%xmm1
+    646c40cf:	mulsd  %xmm2,%xmm1
+    646c40d3:	mov    -0x8(%rbp),%eax
+    646c40d6:	cltq
+    646c40d8:	lea    0x0(,%rax,8),%rdx
+    646c40e0:	mov    0x18(%rbp),%rax
+    646c40e4:	add    %rdx,%rax
+    646c40e7:	mov    (%rax),%rdx
+    646c40ea:	mov    -0x4(%rbp),%eax
+    646c40ed:	cltq
+    646c40ef:	shl    $0x3,%rax
+    646c40f3:	add    %rdx,%rax
+    646c40f6:	subsd  %xmm1,%xmm0
+    646c40fa:	movsd  %xmm0,(%rax)
+    646c40fe:	addl   $0x1,-0xc(%rbp)
+    646c4102:	mov    -0xc(%rbp),%eax
+    646c4105:	cmp    -0x4(%rbp),%eax
+    646c4108:	jl     646c405a <lu_decomposition+0xc2>
+    646c410e:	addl   $0x1,-0x8(%rbp)
+    646c4112:	mov    -0x8(%rbp),%eax
+    646c4115:	cmp    0x28(%rbp),%eax
+    646c4118:	jl     646c3fc8 <lu_decomposition+0x30>
+    646c411e:	movl   $0x0,-0x10(%rbp)
+    646c4125:	jmp    646c4306 <lu_decomposition+0x36e>
+    646c412a:	mov    -0x10(%rbp),%eax
+    646c412d:	cmp    -0x4(%rbp),%eax
+    646c4130:	jge    646c4162 <lu_decomposition+0x1ca>
+    646c4132:	mov    -0x4(%rbp),%eax
+    646c4135:	cltq
+    646c4137:	lea    0x0(,%rax,8),%rdx
+    646c413f:	mov    0x20(%rbp),%rax
+    646c4143:	add    %rdx,%rax
+    646c4146:	mov    (%rax),%rdx
+    646c4149:	mov    -0x10(%rbp),%eax
+    646c414c:	cltq
+    646c414e:	shl    $0x3,%rax
+    646c4152:	add    %rdx,%rax
+    646c4155:	pxor   %xmm0,%xmm0
+    646c4159:	movsd  %xmm0,(%rax)
+    646c415d:	jmp    646c4302 <lu_decomposition+0x36a>
+    646c4162:	mov    -0x10(%rbp),%eax
+    646c4165:	cmp    -0x4(%rbp),%eax
+    646c4168:	jne    646c419e <lu_decomposition+0x206>
+    646c416a:	mov    -0x4(%rbp),%eax
+    646c416d:	cltq
+    646c416f:	lea    0x0(,%rax,8),%rdx
+    646c4177:	mov    0x20(%rbp),%rax
+    646c417b:	add    %rdx,%rax
+    646c417e:	mov    (%rax),%rdx
+    646c4181:	mov    -0x10(%rbp),%eax
+    646c4184:	cltq
+    646c4186:	shl    $0x3,%rax
+    646c418a:	add    %rdx,%rax
+    646c418d:	movsd  0x4f4b(%rip),%xmm0        # 646c90e0 <.rdata+0x50>
+    646c4195:	movsd  %xmm0,(%rax)
+    646c4199:	jmp    646c4302 <lu_decomposition+0x36a>
+    646c419e:	mov    -0x4(%rbp),%eax
+    646c41a1:	cltq
+    646c41a3:	lea    0x0(,%rax,8),%rdx
+    646c41ab:	mov    0x10(%rbp),%rax
+    646c41af:	add    %rdx,%rax
+    646c41b2:	mov    (%rax),%rdx
+    646c41b5:	mov    -0x10(%rbp),%eax
+    646c41b8:	cltq
+    646c41ba:	shl    $0x3,%rax
+    646c41be:	add    %rdx,%rax
+    646c41c1:	movsd  (%rax),%xmm0
+    646c41c5:	mov    -0x4(%rbp),%eax
+    646c41c8:	cltq
+    646c41ca:	lea    0x0(,%rax,8),%rdx
+    646c41d2:	mov    0x18(%rbp),%rax
+    646c41d6:	add    %rdx,%rax
+    646c41d9:	mov    (%rax),%rdx
+    646c41dc:	mov    -0x4(%rbp),%eax
+    646c41df:	cltq
+    646c41e1:	shl    $0x3,%rax
+    646c41e5:	add    %rdx,%rax
+    646c41e8:	movsd  (%rax),%xmm1
+    646c41ec:	mov    -0x4(%rbp),%eax
+    646c41ef:	cltq
+    646c41f1:	lea    0x0(,%rax,8),%rdx
+    646c41f9:	mov    0x20(%rbp),%rax
+    646c41fd:	add    %rdx,%rax
+    646c4200:	mov    (%rax),%rdx
+    646c4203:	mov    -0x10(%rbp),%eax
+    646c4206:	cltq
+    646c4208:	shl    $0x3,%rax
+    646c420c:	add    %rdx,%rax
+    646c420f:	divsd  %xmm1,%xmm0
+    646c4213:	movsd  %xmm0,(%rax)
+    646c4217:	movl   $0x0,-0x14(%rbp)
+    646c421e:	jmp    646c42f6 <lu_decomposition+0x35e>
+    646c4223:	mov    -0x4(%rbp),%eax
+    646c4226:	cltq
+    646c4228:	lea    0x0(,%rax,8),%rdx
+    646c4230:	mov    0x20(%rbp),%rax
+    646c4234:	add    %rdx,%rax
+    646c4237:	mov    (%rax),%rdx
+    646c423a:	mov    -0x10(%rbp),%eax
+    646c423d:	cltq
+    646c423f:	shl    $0x3,%rax
+    646c4243:	add    %rdx,%rax
+    646c4246:	movsd  (%rax),%xmm0
+    646c424a:	mov    -0x4(%rbp),%eax
+    646c424d:	cltq
+    646c424f:	lea    0x0(,%rax,8),%rdx
+    646c4257:	mov    0x18(%rbp),%rax
+    646c425b:	add    %rdx,%rax
+    646c425e:	mov    (%rax),%rdx
+    646c4261:	mov    -0x14(%rbp),%eax
+    646c4264:	cltq
+    646c4266:	shl    $0x3,%rax
+    646c426a:	add    %rdx,%rax
+    646c426d:	movsd  (%rax),%xmm2
+    646c4271:	mov    -0x14(%rbp),%eax
+    646c4274:	cltq
+    646c4276:	lea    0x0(,%rax,8),%rdx
+    646c427e:	mov    0x20(%rbp),%rax
+    646c4282:	add    %rdx,%rax
+    646c4285:	mov    (%rax),%rdx
+    646c4288:	mov    -0x10(%rbp),%eax
+    646c428b:	cltq
+    646c428d:	shl    $0x3,%rax
+    646c4291:	add    %rdx,%rax
+    646c4294:	movsd  (%rax),%xmm1
+    646c4298:	mulsd  %xmm2,%xmm1
+    646c429c:	mov    -0x4(%rbp),%eax
+    646c429f:	cltq
+    646c42a1:	lea    0x0(,%rax,8),%rdx
+    646c42a9:	mov    0x18(%rbp),%rax
+    646c42ad:	add    %rdx,%rax
+    646c42b0:	mov    (%rax),%rdx
+    646c42b3:	mov    -0x4(%rbp),%eax
+    646c42b6:	cltq
+    646c42b8:	shl    $0x3,%rax
+    646c42bc:	add    %rdx,%rax
+    646c42bf:	movsd  (%rax),%xmm2
+    646c42c3:	divsd  %xmm2,%xmm1
+    646c42c7:	mov    -0x4(%rbp),%eax
+    646c42ca:	cltq
+    646c42cc:	lea    0x0(,%rax,8),%rdx
+    646c42d4:	mov    0x20(%rbp),%rax
+    646c42d8:	add    %rdx,%rax
+    646c42db:	mov    (%rax),%rdx
+    646c42de:	mov    -0x10(%rbp),%eax
+    646c42e1:	cltq
+    646c42e3:	shl    $0x3,%rax
+    646c42e7:	add    %rdx,%rax
+    646c42ea:	subsd  %xmm1,%xmm0
+    646c42ee:	movsd  %xmm0,(%rax)
+    646c42f2:	addl   $0x1,-0x14(%rbp)
+    646c42f6:	mov    -0x14(%rbp),%eax
+    646c42f9:	cmp    -0x4(%rbp),%eax
+    646c42fc:	jl     646c4223 <lu_decomposition+0x28b>
+    646c4302:	addl   $0x1,-0x10(%rbp)
+    646c4306:	mov    -0x10(%rbp),%eax
+    646c4309:	cmp    0x28(%rbp),%eax
+    646c430c:	jl     646c412a <lu_decomposition+0x192>
+    646c4312:	addl   $0x1,-0x4(%rbp)
+    646c4316:	mov    -0x4(%rbp),%eax
+    646c4319:	cmp    0x28(%rbp),%eax
+    646c431c:	jl     646c3fbc <lu_decomposition+0x24>
+    646c4322:	nop
+    646c4323:	add    $0x20,%rsp
+    646c4327:	pop    %rbp
+    646c4328:	ret
+
+00000000646c4329 <arange>:
+    646c4329:	push   %rbp
+    646c432a:	mov    %rsp,%rbp
+    646c432d:	sub    $0x30,%rsp
+    646c4331:	mov    %ecx,0x10(%rbp)
+    646c4334:	mov    0x10(%rbp),%eax
+    646c4337:	cltq
+    646c4339:	shl    $0x2,%rax
+    646c433d:	mov    %rax,%rcx
+    646c4340:	call   646c7970 <malloc>
+    646c4345:	mov    %rax,-0x10(%rbp)
+    646c4349:	movl   $0x0,-0x4(%rbp)
+    646c4350:	jmp    646c436f <arange+0x46>
+    646c4352:	mov    -0x4(%rbp),%eax
+    646c4355:	cltq
+    646c4357:	lea    0x0(,%rax,4),%rdx
+    646c435f:	mov    -0x10(%rbp),%rax
+    646c4363:	add    %rdx,%rax
+    646c4366:	mov    -0x4(%rbp),%edx
+    646c4369:	mov    %edx,(%rax)
+    646c436b:	addl   $0x1,-0x4(%rbp)
+    646c436f:	mov    -0x4(%rbp),%eax
+    646c4372:	cmp    0x10(%rbp),%eax
+    646c4375:	jl     646c4352 <arange+0x29>
+    646c4377:	mov    -0x10(%rbp),%rax
+    646c437b:	add    $0x30,%rsp
+    646c437f:	pop    %rbp
+    646c4380:	ret
+
+00000000646c4381 <d_arange>:
+    646c4381:	push   %rbp
+    646c4382:	mov    %rsp,%rbp
+    646c4385:	sub    $0x30,%rsp
+    646c4389:	mov    %ecx,0x10(%rbp)
+    646c438c:	mov    0x10(%rbp),%eax
+    646c438f:	cltq
+    646c4391:	shl    $0x3,%rax
+    646c4395:	mov    %rax,%rcx
+    646c4398:	call   646c7970 <malloc>
+    646c439d:	mov    %rax,-0x10(%rbp)
+    646c43a1:	movl   $0x0,-0x4(%rbp)
+    646c43a8:	jmp    646c43cb <d_arange+0x4a>
+    646c43aa:	mov    -0x4(%rbp),%eax
+    646c43ad:	cltq
+    646c43af:	lea    0x0(,%rax,8),%rdx
+    646c43b7:	mov    -0x10(%rbp),%rax
+    646c43bb:	add    %rdx,%rax
+    646c43be:	cvtsi2sdl -0x4(%rbp),%xmm0
+    646c43c3:	movsd  %xmm0,(%rax)
+    646c43c7:	addl   $0x1,-0x4(%rbp)
+    646c43cb:	mov    -0x4(%rbp),%eax
+    646c43ce:	cmp    0x10(%rbp),%eax
+    646c43d1:	jl     646c43aa <d_arange+0x29>
+    646c43d3:	mov    -0x10(%rbp),%rax
+    646c43d7:	add    $0x30,%rsp
+    646c43db:	pop    %rbp
+    646c43dc:	ret
+
+00000000646c43dd <pdist>:
+    646c43dd:	push   %rbp
+    646c43de:	mov    %rsp,%rbp
+    646c43e1:	sub    $0x10,%rsp
+    646c43e5:	mov    %rcx,0x10(%rbp)
+    646c43e9:	mov    %rdx,0x18(%rbp)
+    646c43ed:	mov    %r8d,0x20(%rbp)
+    646c43f1:	movl   $0x0,-0x4(%rbp)
+    646c43f8:	jmp    646c447d <pdist+0xa0>
+    646c43fd:	movl   $0x0,-0x8(%rbp)
+    646c4404:	jmp    646c4471 <pdist+0x94>
+    646c4406:	mov    -0x8(%rbp),%eax
+    646c4409:	cltq
+    646c440b:	lea    0x0(,%rax,8),%rdx
+    646c4413:	mov    0x10(%rbp),%rax
+    646c4417:	add    %rdx,%rax
+    646c441a:	movsd  (%rax),%xmm0
+    646c441e:	mov    -0x4(%rbp),%eax
+    646c4421:	cltq
+    646c4423:	lea    0x0(,%rax,8),%rdx
+    646c442b:	mov    0x10(%rbp),%rax
+    646c442f:	add    %rdx,%rax
+    646c4432:	movsd  (%rax),%xmm1
+    646c4436:	subsd  %xmm1,%xmm0
+    646c443a:	mov    -0x4(%rbp),%eax
+    646c443d:	cltq
+    646c443f:	lea    0x0(,%rax,8),%rdx
+    646c4447:	mov    0x18(%rbp),%rax
+    646c444b:	add    %rdx,%rax
+    646c444e:	mov    (%rax),%rdx
+    646c4451:	mov    -0x8(%rbp),%eax
+    646c4454:	cltq
+    646c4456:	shl    $0x3,%rax
+    646c445a:	add    %rdx,%rax
+    646c445d:	movq   0x4c8b(%rip),%xmm1        # 646c90f0 <.rdata+0x60>
+    646c4465:	andpd  %xmm1,%xmm0
+    646c4469:	movsd  %xmm0,(%rax)
+    646c446d:	addl   $0x1,-0x8(%rbp)
+    646c4471:	mov    -0x8(%rbp),%eax
+    646c4474:	cmp    0x20(%rbp),%eax
+    646c4477:	jl     646c4406 <pdist+0x29>
+    646c4479:	addl   $0x1,-0x4(%rbp)
+    646c447d:	mov    -0x4(%rbp),%eax
+    646c4480:	cmp    0x20(%rbp),%eax
+    646c4483:	jl     646c43fd <pdist+0x20>
+    646c4489:	nop
+    646c448a:	add    $0x10,%rsp
+    646c448e:	pop    %rbp
+    646c448f:	ret
+
+00000000646c4490 <matrixform>:
+    646c4490:	push   %rbp
+    646c4491:	mov    %rsp,%rbp
+    646c4494:	sub    $0x10,%rsp
+    646c4498:	mov    %rcx,0x10(%rbp)
+    646c449c:	mov    %rdx,0x18(%rbp)
+    646c44a0:	mov    %r8d,0x20(%rbp)
+    646c44a4:	movl   $0x0,-0x4(%rbp)
+    646c44ab:	jmp    646c450e <matrixform+0x7e>
+    646c44ad:	movl   $0x0,-0x8(%rbp)
+    646c44b4:	jmp    646c4502 <matrixform+0x72>
+    646c44b6:	mov    0x20(%rbp),%eax
+    646c44b9:	imul   -0x4(%rbp),%eax
+    646c44bd:	mov    -0x8(%rbp),%edx
+    646c44c0:	add    %edx,%eax
+    646c44c2:	cltq
+    646c44c4:	lea    0x0(,%rax,8),%rdx
+    646c44cc:	mov    0x10(%rbp),%rax
+    646c44d0:	add    %rax,%rdx
+    646c44d3:	mov    -0x4(%rbp),%eax
+    646c44d6:	cltq
+    646c44d8:	lea    0x0(,%rax,8),%rcx
+    646c44e0:	mov    0x18(%rbp),%rax
+    646c44e4:	add    %rcx,%rax
+    646c44e7:	mov    (%rax),%rcx
+    646c44ea:	mov    -0x8(%rbp),%eax
+    646c44ed:	cltq
+    646c44ef:	shl    $0x3,%rax
+    646c44f3:	add    %rcx,%rax
+    646c44f6:	movsd  (%rdx),%xmm0
+    646c44fa:	movsd  %xmm0,(%rax)
+    646c44fe:	addl   $0x1,-0x8(%rbp)
+    646c4502:	mov    -0x8(%rbp),%eax
+    646c4505:	cmp    0x20(%rbp),%eax
+    646c4508:	jl     646c44b6 <matrixform+0x26>
+    646c450a:	addl   $0x1,-0x4(%rbp)
+    646c450e:	mov    -0x4(%rbp),%eax
+    646c4511:	cmp    0x20(%rbp),%eax
+    646c4514:	jl     646c44ad <matrixform+0x1d>
+    646c4516:	nop
+    646c4517:	add    $0x10,%rsp
+    646c451b:	pop    %rbp
+    646c451c:	ret
+
+00000000646c451d <save_1darray>:
+    646c451d:	push   %rbp
+    646c451e:	sub    $0x1e0,%rsp
+    646c4525:	lea    0x80(%rsp),%rbp
+    646c452d:	mov    %rcx,0x170(%rbp)
+    646c4534:	mov    %edx,0x178(%rbp)
+    646c453a:	mov    %r8,0x180(%rbp)
+    646c4541:	mov    %r9,0x188(%rbp)
+    646c4548:	cvtsi2sdl 0x190(%rbp),%xmm0
+    646c4550:	call   646c7978 <log10>
+    646c4555:	movq   %xmm0,%rax
+    646c455a:	movq   %rax,%xmm0
+    646c455f:	call   646c69a0 <ceil>
+    646c4564:	cvttsd2si %xmm0,%eax
+    646c4568:	add    $0x1,%eax
+    646c456b:	mov    %eax,0x158(%rbp)
+    646c4571:	mov    0x188(%rbp),%rcx
+    646c4578:	lea    0x80(%rbp),%rax
+    646c457f:	mov    0x158(%rbp),%edx
+    646c4585:	mov    %edx,0x28(%rsp)
+    646c4589:	mov    0x180(%rbp),%rdx
+    646c4590:	mov    %rdx,0x20(%rsp)
+    646c4595:	mov    %rcx,%r9
+    646c4598:	lea    0x4af1(%rip),%r8        # 646c9090 <.rdata>
+    646c459f:	mov    $0xc8,%edx
+    646c45a4:	mov    %rax,%rcx
+    646c45a7:	call   646c3bd0 <snprintf>
+    646c45ac:	mov    0x188(%rbp),%rax
+    646c45b3:	mov    %rax,%rcx
+    646c45b6:	call   646c79c8 <_mkdir>
+    646c45bb:	cmp    $0xffffffff,%eax
+    646c45be:	jne    646c45dc <save_1darray+0xbf>
+    646c45c0:	mov    0x9cd5(%rip),%rax        # 646ce29c <__imp__errno>
+    646c45c7:	call   *%rax
+    646c45c9:	mov    (%rax),%eax
+    646c45cb:	cmp    $0x11,%eax
+    646c45ce:	je     646c45dc <save_1darray+0xbf>
+    646c45d0:	lea    0x4ac8(%rip),%rcx        # 646c909f <.rdata+0xf>
+    646c45d7:	call   646c7960 <printf>
+    646c45dc:	mov    0x198(%rbp),%ecx
+    646c45e2:	lea    0x80(%rbp),%rdx
+    646c45e9:	lea    -0x50(%rbp),%rax
+    646c45ed:	mov    %ecx,%r9d
+    646c45f0:	mov    %rdx,%r8
+    646c45f3:	mov    $0xc8,%edx
+    646c45f8:	mov    %rax,%rcx
+    646c45fb:	call   646c3bd0 <snprintf>
+    646c4600:	lea    -0x50(%rbp),%rax
+    646c4604:	lea    0x4aaa(%rip),%rdx        # 646c90b5 <.rdata+0x25>
+    646c460b:	mov    %rax,%rcx
+    646c460e:	call   646c7998 <fopen>
+    646c4613:	mov    %rax,0x150(%rbp)
+    646c461a:	cmpq   $0x0,0x150(%rbp)
+    646c4622:	jne    646c463a <save_1darray+0x11d>
+    646c4624:	lea    0x4a8c(%rip),%rcx        # 646c90b7 <.rdata+0x27>
+    646c462b:	call   646c7968 <perror>
+    646c4630:	mov    $0x1,%ecx
+    646c4635:	call   646c79a8 <exit>
+    646c463a:	movl   $0x0,0x15c(%rbp)
+    646c4644:	jmp    646c46a4 <save_1darray+0x187>
+    646c4646:	mov    0x15c(%rbp),%eax
+    646c464c:	cltq
+    646c464e:	lea    0x0(,%rax,8),%rdx
+    646c4656:	mov    0x170(%rbp),%rax
+    646c465d:	add    %rdx,%rax
+    646c4660:	movsd  (%rax),%xmm0
+    646c4664:	movq   %xmm0,%rax
+    646c4669:	mov    %rax,%rdx
+    646c466c:	mov    %rdx,%rcx
+    646c466f:	movq   %rax,%xmm0
+    646c4674:	mov    0x15c(%rbp),%edx
+    646c467a:	mov    0x150(%rbp),%rax
+    646c4681:	movq   %rcx,%xmm3
+    646c4686:	movq   %xmm0,%r9
+    646c468b:	mov    %edx,%r8d
+    646c468e:	lea    0x4a3a(%rip),%rdx        # 646c90cf <.rdata+0x3f>
+    646c4695:	mov    %rax,%rcx
+    646c4698:	call   646c7990 <fprintf>
+    646c469d:	addl   $0x1,0x15c(%rbp)
+    646c46a4:	mov    0x15c(%rbp),%eax
+    646c46aa:	cmp    0x178(%rbp),%eax
+    646c46b0:	jl     646c4646 <save_1darray+0x129>
+    646c46b2:	mov    0x150(%rbp),%rax
+    646c46b9:	mov    %rax,%rcx
+    646c46bc:	call   646c79a0 <fclose>
+    646c46c1:	nop
+    646c46c2:	add    $0x1e0,%rsp
+    646c46c9:	pop    %rbp
+    646c46ca:	ret
+    646c46cb:	nop
+    646c46cc:	nop
+    646c46cd:	nop
+    646c46ce:	nop
+    646c46cf:	nop
+
+00000000646c46d0 <randompath>:
+    646c46d0:	push   %rbp
+    646c46d1:	mov    %rsp,%rbp
+    646c46d4:	sub    $0x30,%rsp
+    646c46d8:	mov    %rcx,0x10(%rbp)
+    646c46dc:	mov    %edx,0x18(%rbp)
+    646c46df:	mov    %r8,0x20(%rbp)
+    646c46e3:	mov    0x18(%rbp),%eax
+    646c46e6:	sub    $0x1,%eax
+    646c46e9:	mov    %eax,-0x4(%rbp)
+    646c46ec:	jmp    646c476b <randompath+0x9b>
+    646c46ee:	mov    0x20(%rbp),%rax
+    646c46f2:	mov    %rax,%rcx
+    646c46f5:	call   646c2aae <mt19937_generate>
+    646c46fa:	mov    -0x4(%rbp),%ecx
+    646c46fd:	mov    $0x0,%edx
+    646c4702:	div    %ecx
+    646c4704:	mov    %edx,%eax
+    646c4706:	mov    %eax,-0x8(%rbp)
+    646c4709:	mov    -0x8(%rbp),%eax
+    646c470c:	cltq
+    646c470e:	lea    0x0(,%rax,4),%rdx
+    646c4716:	mov    0x10(%rbp),%rax
+    646c471a:	add    %rdx,%rax
+    646c471d:	mov    (%rax),%eax
+    646c471f:	mov    %eax,-0xc(%rbp)
+    646c4722:	mov    -0x4(%rbp),%eax
+    646c4725:	cltq
+    646c4727:	lea    0x0(,%rax,4),%rdx
+    646c472f:	mov    0x10(%rbp),%rax
+    646c4733:	add    %rax,%rdx
+    646c4736:	mov    -0x8(%rbp),%eax
+    646c4739:	cltq
+    646c473b:	lea    0x0(,%rax,4),%rcx
+    646c4743:	mov    0x10(%rbp),%rax
+    646c4747:	add    %rcx,%rax
+    646c474a:	mov    (%rdx),%edx
+    646c474c:	mov    %edx,(%rax)
+    646c474e:	mov    -0x4(%rbp),%eax
+    646c4751:	cltq
+    646c4753:	lea    0x0(,%rax,4),%rdx
+    646c475b:	mov    0x10(%rbp),%rax
+    646c475f:	add    %rdx,%rax
+    646c4762:	mov    -0xc(%rbp),%edx
+    646c4765:	mov    %edx,(%rax)
+    646c4767:	subl   $0x1,-0x4(%rbp)
+    646c476b:	cmpl   $0x0,-0x4(%rbp)
+    646c476f:	jne    646c46ee <randompath+0x1e>
+    646c4775:	mov    0x10(%rbp),%rax
+    646c4779:	add    $0x30,%rsp
+    646c477d:	pop    %rbp
+    646c477e:	ret
+    646c477f:	nop
+
+00000000646c4780 <sgsim_init>:
+    646c4780:	push   %rbp
+    646c4781:	mov    %rsp,%rbp
+    646c4784:	sub    $0x30,%rsp
+    646c4788:	mov    %rcx,0x10(%rbp)
+    646c478c:	mov    %edx,0x18(%rbp)
+    646c478f:	mov    %r8d,0x20(%rbp)
+    646c4793:	mov    %r9d,0x28(%rbp)
+    646c4797:	mov    0x10(%rbp),%rax
+    646c479b:	mov    0x18(%rbp),%edx
+    646c479e:	mov    %edx,(%rax)
+    646c47a0:	mov    0x10(%rbp),%rax
+    646c47a4:	mov    0x20(%rbp),%edx
+    646c47a7:	mov    %edx,0x4(%rax)
+    646c47aa:	mov    0x10(%rbp),%rax
+    646c47ae:	mov    0x28(%rbp),%edx
+    646c47b1:	mov    %edx,0x8(%rax)
+    646c47b4:	cmpl   $0x1,0x30(%rbp)
+    646c47b8:	jne    646c47de <sgsim_init+0x5e>
+    646c47ba:	mov    0x18(%rbp),%eax
+    646c47bd:	imul   0x20(%rbp),%eax
+    646c47c1:	mov    %eax,-0x4(%rbp)
+    646c47c4:	mov    -0x4(%rbp),%eax
+    646c47c7:	shl    $0x3,%rax
+    646c47cb:	mov    %rax,%rcx
+    646c47ce:	call   646c7970 <malloc>
+    646c47d3:	mov    %rax,%rdx
+    646c47d6:	mov    0x10(%rbp),%rax
+    646c47da:	mov    %rdx,0x10(%rax)
+    646c47de:	nop
+    646c47df:	add    $0x30,%rsp
+    646c47e3:	pop    %rbp
+    646c47e4:	ret
+
+00000000646c47e5 <sgsim_run>:
+    646c47e5:	push   %rbp
+    646c47e6:	sub    $0xa00,%rsp
+    646c47ed:	lea    0x80(%rsp),%rbp
+    646c47f5:	mov    %rcx,0x990(%rbp)
+    646c47fc:	mov    %rdx,0x998(%rbp)
+    646c4803:	mov    %r8d,0x9a0(%rbp)
+    646c480a:	mov    0x990(%rbp),%rax
+    646c4811:	mov    0x8(%rax),%eax
+    646c4814:	mov    %eax,%edx
+    646c4816:	lea    -0x50(%rbp),%rax
+    646c481a:	mov    %rax,%rcx
+    646c481d:	call   646c2a30 <mt19937_init>
+    646c4822:	mov    0x990(%rbp),%rax
+    646c4829:	mov    (%rax),%eax
+    646c482b:	mov    %eax,%edx
+    646c482d:	lea    0x79ec(%rip),%rcx        # 646cc220 <_sampling>
+    646c4834:	call   646c3180 <sampling_state_init>
+    646c4839:	mov    0x998(%rbp),%rax
+    646c4840:	mov    0x8(%rax),%eax
+    646c4843:	cltq
+    646c4845:	mov    %rax,0x799c(%rip)        # 646cc1e8 <variogram_array+0x8>
+    646c484c:	mov    0x998(%rbp),%rax
+    646c4853:	mov    0x8(%rax),%eax
+    646c4856:	cltq
+    646c4858:	mov    %rax,0x7991(%rip)        # 646cc1f0 <variogram_array+0x10>
+    646c485f:	mov    0x998(%rbp),%rax
+    646c4866:	mov    0x8(%rax),%eax
+    646c4869:	cltq
+    646c486b:	mov    $0x8,%edx
+    646c4870:	mov    %rax,%rcx
+    646c4873:	call   646c79b0 <calloc>
+    646c4878:	mov    %rax,0x7961(%rip)        # 646cc1e0 <variogram_array>
+    646c487f:	mov    0x990(%rbp),%rax
+    646c4886:	mov    (%rax),%eax
+    646c4888:	cltq
+    646c488a:	mov    %rax,0x7977(%rip)        # 646cc208 <sgsim_array+0x8>
+    646c4891:	mov    0x990(%rbp),%rax
+    646c4898:	mov    (%rax),%eax
+    646c489a:	cltq
+    646c489c:	mov    %rax,0x796d(%rip)        # 646cc210 <sgsim_array+0x10>
+    646c48a3:	mov    0x990(%rbp),%rax
+    646c48aa:	mov    (%rax),%eax
+    646c48ac:	cltq
+    646c48ae:	mov    $0x8,%edx
+    646c48b3:	mov    %rax,%rcx
+    646c48b6:	call   646c79b0 <calloc>
+    646c48bb:	mov    %rax,0x793e(%rip)        # 646cc200 <sgsim_array>
+    646c48c2:	mov    0x990(%rbp),%rax
+    646c48c9:	mov    (%rax),%eax
+    646c48cb:	mov    0x998(%rbp),%rdx
+    646c48d2:	mov    %eax,%ecx
+    646c48d4:	call   646c325d <krige_param_setting>
+    646c48d9:	mov    0x990(%rbp),%rax
+    646c48e0:	mov    (%rax),%eax
+    646c48e2:	mov    %eax,%ecx
+    646c48e4:	call   646c4329 <arange>
+    646c48e9:	mov    %rax,0x7890(%rip)        # 646cc180 <x_grid>
+    646c48f0:	movl   $0x0,0x7972(%rip)        # 646cc26c <count>
+    646c48fa:	jmp    646c4c6f <sgsim_run+0x48a>
+    646c48ff:	mov    0x7967(%rip),%eax        # 646cc26c <count>
+    646c4905:	mov    %eax,%edx
+    646c4907:	lea    0x47f2(%rip),%rcx        # 646c9100 <.rdata>
+    646c490e:	call   646c7960 <printf>
+    646c4913:	movl   $0x0,0x7907(%rip)        # 646cc224 <_sampling+0x4>
+    646c491d:	movl   $0x0,0x78f9(%rip)        # 646cc220 <_sampling>
+    646c4927:	movl   $0x0,0x7937(%rip)        # 646cc268 <flag>
+    646c4931:	mov    0x990(%rbp),%rax
+    646c4938:	mov    (%rax),%edx
+    646c493a:	mov    0x783f(%rip),%rax        # 646cc180 <x_grid>
+    646c4941:	lea    -0x50(%rbp),%rcx
+    646c4945:	mov    %rcx,%r8
+    646c4948:	mov    %rax,%rcx
+    646c494b:	call   646c46d0 <randompath>
+    646c4950:	mov    %rax,0x7829(%rip)        # 646cc180 <x_grid>
+    646c4957:	movl   $0x0,0x97c(%rbp)
+    646c4961:	jmp    646c49c8 <sgsim_run+0x1e3>
+    646c4963:	mov    0x7896(%rip),%rdx        # 646cc200 <sgsim_array>
+    646c496a:	mov    0x97c(%rbp),%eax
+    646c4970:	cltq
+    646c4972:	shl    $0x3,%rax
+    646c4976:	add    %rdx,%rax
+    646c4979:	pxor   %xmm0,%xmm0
+    646c497d:	movsd  %xmm0,(%rax)
+    646c4981:	mov    0x78b0(%rip),%rdx        # 646cc238 <_sampling+0x18>
+    646c4988:	mov    0x97c(%rbp),%eax
+    646c498e:	cltq
+    646c4990:	shl    $0x3,%rax
+    646c4994:	add    %rdx,%rax
+    646c4997:	pxor   %xmm0,%xmm0
+    646c499b:	movsd  %xmm0,(%rax)
+    646c499f:	mov    0x78aa(%rip),%rdx        # 646cc250 <_sampling+0x30>
+    646c49a6:	mov    0x97c(%rbp),%eax
+    646c49ac:	cltq
+    646c49ae:	shl    $0x3,%rax
+    646c49b2:	add    %rdx,%rax
+    646c49b5:	movsd  0x4793(%rip),%xmm0        # 646c9150 <.rdata+0x50>
+    646c49bd:	movsd  %xmm0,(%rax)
+    646c49c1:	addl   $0x1,0x97c(%rbp)
+    646c49c8:	mov    0x990(%rbp),%rax
+    646c49cf:	mov    (%rax),%eax
+    646c49d1:	cmp    %eax,0x97c(%rbp)
+    646c49d7:	jl     646c4963 <sgsim_run+0x17e>
+    646c49d9:	movl   $0x0,0x978(%rbp)
+    646c49e3:	jmp    646c4b61 <sgsim_run+0x37c>
+    646c49e8:	mov    0x7791(%rip),%rdx        # 646cc180 <x_grid>
+    646c49ef:	mov    0x978(%rbp),%eax
+    646c49f5:	cltq
+    646c49f7:	shl    $0x2,%rax
+    646c49fb:	add    %rdx,%rax
+    646c49fe:	mov    (%rax),%eax
+    646c4a00:	cvtsi2sd %eax,%xmm0
+    646c4a04:	mov    0x978(%rbp),%eax
+    646c4a0a:	mov    %eax,%r8d
+    646c4a0d:	movapd %xmm0,%xmm1
+    646c4a11:	lea    0x7808(%rip),%rcx        # 646cc220 <_sampling>
+    646c4a18:	call   646c3231 <sampling_state_update>
+    646c4a1d:	mov    0x77dc(%rip),%rax        # 646cc200 <sgsim_array>
+    646c4a24:	lea    -0x50(%rbp),%rdx
+    646c4a28:	mov    %rdx,%r8
+    646c4a2b:	lea    0x77ee(%rip),%rdx        # 646cc220 <_sampling>
+    646c4a32:	mov    %rax,%rcx
+    646c4a35:	call   646c34b9 <simple_kriging>
+    646c4a3a:	mov    0x77bf(%rip),%rdx        # 646cc200 <sgsim_array>
+    646c4a41:	mov    0x7738(%rip),%rcx        # 646cc180 <x_grid>
+    646c4a48:	mov    0x978(%rbp),%eax
+    646c4a4e:	cltq
+    646c4a50:	shl    $0x2,%rax
+    646c4a54:	add    %rcx,%rax
+    646c4a57:	mov    (%rax),%eax
+    646c4a59:	cltq
+    646c4a5b:	shl    $0x3,%rax
+    646c4a5f:	add    %rax,%rdx
+    646c4a62:	mov    0x990(%rbp),%rax
+    646c4a69:	mov    0x10(%rax),%rcx
+    646c4a6d:	mov    0x770c(%rip),%r8        # 646cc180 <x_grid>
+    646c4a74:	mov    0x978(%rbp),%eax
+    646c4a7a:	cltq
+    646c4a7c:	shl    $0x2,%rax
+    646c4a80:	add    %r8,%rax
+    646c4a83:	mov    (%rax),%r8d
+    646c4a86:	mov    0x990(%rbp),%rax
+    646c4a8d:	mov    (%rax),%r9d
+    646c4a90:	mov    0x77d6(%rip),%eax        # 646cc26c <count>
+    646c4a96:	imul   %r9d,%eax
+    646c4a9a:	add    %r8d,%eax
+    646c4a9d:	cltq
+    646c4a9f:	shl    $0x3,%rax
+    646c4aa3:	add    %rcx,%rax
+    646c4aa6:	movsd  (%rdx),%xmm0
+    646c4aaa:	movsd  %xmm0,(%rax)
+    646c4aae:	mov    0x776c(%rip),%eax        # 646cc220 <_sampling>
+    646c4ab4:	cmp    $0x7,%eax
+    646c4ab7:	jg     646c4ac8 <sgsim_run+0x2e3>
+    646c4ab9:	mov    0x7761(%rip),%eax        # 646cc220 <_sampling>
     646c4abf:	add    $0x1,%eax
-    646c4ac2:	mov    %eax,0x77a0(%rip)        # 646cc268 <flag>
-    646c4ac8:	addl   $0x1,0x978(%rbp)
-    646c4acf:	mov    0x990(%rbp),%rax
-    646c4ad6:	mov    (%rax),%eax
-    646c4ad8:	cmp    %eax,0x978(%rbp)
-    646c4ade:	jl     646c4956 <sgsim_run+0x211>
-    646c4ae4:	mov    0x7782(%rip),%eax        # 646cc26c <count>
-    646c4aea:	add    $0x1,%eax
-    646c4aed:	mov    %eax,0x7779(%rip)        # 646cc26c <count>
-    646c4af3:	cmpl   $0x1,0x9a0(%rbp)
-    646c4afa:	jne    646c4b34 <sgsim_run+0x3ef>
-    646c4afc:	mov    0x998(%rbp),%rax
-    646c4b03:	mov    (%rax),%ecx
-    646c4b05:	mov    0x998(%rbp),%rax
-    646c4b0c:	mov    0x4(%rax),%r9d
-    646c4b10:	mov    0x990(%rbp),%rax
-    646c4b17:	mov    (%rax),%r8d
-    646c4b1a:	mov    0x76bf(%rip),%rdx        # 646cc1e0 <variogram_array>
-    646c4b21:	mov    0x76d8(%rip),%rax        # 646cc200 <sgsim_array>
-    646c4b28:	mov    %ecx,0x20(%rsp)
-    646c4b2c:	mov    %rax,%rcx
-    646c4b2f:	call   646c5090 <variogram>
-    646c4b34:	mov    0x772e(%rip),%eax        # 646cc268 <flag>
-    646c4b3a:	test   %eax,%eax
-    646c4b3c:	jle    646c4b52 <sgsim_run+0x40d>
-    646c4b3e:	mov    0x7728(%rip),%eax        # 646cc26c <count>
-    646c4b44:	sub    $0x1,%eax
-    646c4b47:	mov    %eax,0x771f(%rip)        # 646cc26c <count>
-    646c4b4d:	jmp    646c4bdc <sgsim_run+0x497>
-    646c4b52:	mov    0x7713(%rip),%r8d        # 646cc26c <count>
-    646c4b59:	mov    0x990(%rbp),%rax
-    646c4b60:	mov    0x4(%rax),%ecx
-    646c4b63:	mov    0x990(%rbp),%rax
-    646c4b6a:	mov    (%rax),%edx
-    646c4b6c:	mov    0x768d(%rip),%rax        # 646cc200 <sgsim_array>
-    646c4b73:	mov    %r8d,0x28(%rsp)
-    646c4b78:	mov    %ecx,0x20(%rsp)
-    646c4b7c:	lea    0x458a(%rip),%r9        # 646c910d <.rdata+0xd>
-    646c4b83:	lea    0x4593(%rip),%r8        # 646c911d <.rdata+0x1d>
-    646c4b8a:	mov    %rax,%rcx
-    646c4b8d:	call   646c447d <save_1darray>
-    646c4b92:	cmpl   $0x1,0x9a0(%rbp)
-    646c4b99:	jne    646c4bdc <sgsim_run+0x497>
-    646c4b9b:	mov    0x76ca(%rip),%r8d        # 646cc26c <count>
-    646c4ba2:	mov    0x990(%rbp),%rax
-    646c4ba9:	mov    0x4(%rax),%ecx
-    646c4bac:	mov    0x998(%rbp),%rax
-    646c4bb3:	mov    0x4(%rax),%edx
-    646c4bb6:	mov    0x7623(%rip),%rax        # 646cc1e0 <variogram_array>
-    646c4bbd:	mov    %r8d,0x28(%rsp)
-    646c4bc2:	mov    %ecx,0x20(%rsp)
-    646c4bc6:	lea    0x455d(%rip),%r9        # 646c912a <.rdata+0x2a>
-    646c4bcd:	lea    0x4570(%rip),%r8        # 646c9144 <.rdata+0x44>
-    646c4bd4:	mov    %rax,%rcx
-    646c4bd7:	call   646c447d <save_1darray>
-    646c4bdc:	mov    0x990(%rbp),%rax
-    646c4be3:	mov    0x4(%rax),%edx
-    646c4be6:	mov    0x7680(%rip),%eax        # 646cc26c <count>
-    646c4bec:	cmp    %eax,%edx
-    646c4bee:	jg     646c486d <sgsim_run+0x128>
-    646c4bf4:	call   646c39da <krige_memory_free>
-    646c4bf9:	call   646c4c2b <sgsim_memory_free>
-    646c4bfe:	nop
-    646c4bff:	add    $0xa00,%rsp
-    646c4c06:	pop    %rbp
-    646c4c07:	ret
-
-00000000646c4c08 <sgsim_t_free>:
-    646c4c08:	push   %rbp
-    646c4c09:	mov    %rsp,%rbp
-    646c4c0c:	sub    $0x20,%rsp
-    646c4c10:	mov    %rcx,0x10(%rbp)
-    646c4c14:	mov    0x10(%rbp),%rax
-    646c4c18:	mov    0x10(%rax),%rax
-    646c4c1c:	mov    %rax,%rcx
-    646c4c1f:	call   646c78f8 <free>
-    646c4c24:	nop
-    646c4c25:	add    $0x20,%rsp
-    646c4c29:	pop    %rbp
-    646c4c2a:	ret
-
-00000000646c4c2b <sgsim_memory_free>:
-    646c4c2b:	push   %rbp
-    646c4c2c:	mov    %rsp,%rbp
-    646c4c2f:	sub    $0x20,%rsp
-    646c4c33:	mov    0x75fe(%rip),%rax        # 646cc238 <_sampling+0x18>
-    646c4c3a:	mov    %rax,%rcx
-    646c4c3d:	call   646c78f8 <free>
-    646c4c42:	mov    0x7607(%rip),%rax        # 646cc250 <_sampling+0x30>
-    646c4c49:	mov    %rax,%rcx
-    646c4c4c:	call   646c78f8 <free>
-    646c4c51:	mov    0x75a8(%rip),%rax        # 646cc200 <sgsim_array>
-    646c4c58:	mov    %rax,%rcx
-    646c4c5b:	call   646c78f8 <free>
-    646c4c60:	mov    0x7519(%rip),%rax        # 646cc180 <x_grid>
+    646c4ac2:	mov    %eax,0x7758(%rip)        # 646cc220 <_sampling>
+    646c4ac8:	mov    0x76b1(%rip),%rdx        # 646cc180 <x_grid>
+    646c4acf:	mov    0x978(%rbp),%eax
+    646c4ad5:	cltq
+    646c4ad7:	shl    $0x2,%rax
+    646c4adb:	add    %rdx,%rax
+    646c4ade:	mov    (%rax),%ecx
+    646c4ae0:	mov    0x7751(%rip),%rdx        # 646cc238 <_sampling+0x18>
+    646c4ae7:	mov    0x978(%rbp),%eax
+    646c4aed:	cltq
+    646c4aef:	shl    $0x3,%rax
+    646c4af3:	add    %rdx,%rax
+    646c4af6:	cvtsi2sd %ecx,%xmm0
+    646c4afa:	movsd  %xmm0,(%rax)
+    646c4afe:	mov    0x7720(%rip),%eax        # 646cc224 <_sampling+0x4>
+    646c4b04:	add    $0x1,%eax
+    646c4b07:	mov    %eax,0x7717(%rip)        # 646cc224 <_sampling+0x4>
+    646c4b0d:	mov    0x76ec(%rip),%rdx        # 646cc200 <sgsim_array>
+    646c4b14:	mov    0x7665(%rip),%rcx        # 646cc180 <x_grid>
+    646c4b1b:	mov    0x978(%rbp),%eax
+    646c4b21:	cltq
+    646c4b23:	shl    $0x2,%rax
+    646c4b27:	add    %rcx,%rax
+    646c4b2a:	mov    (%rax),%eax
+    646c4b2c:	cltq
+    646c4b2e:	shl    $0x3,%rax
+    646c4b32:	add    %rdx,%rax
+    646c4b35:	mov    (%rax),%rax
+    646c4b38:	movq   %rax,%xmm0
+    646c4b3d:	call   646c6800 <__fpclassify>
+    646c4b42:	and    $0x100,%eax
+    646c4b47:	test   %eax,%eax
+    646c4b49:	je     646c4b5a <sgsim_run+0x375>
+    646c4b4b:	mov    0x7717(%rip),%eax        # 646cc268 <flag>
+    646c4b51:	add    $0x1,%eax
+    646c4b54:	mov    %eax,0x770e(%rip)        # 646cc268 <flag>
+    646c4b5a:	addl   $0x1,0x978(%rbp)
+    646c4b61:	mov    0x990(%rbp),%rax
+    646c4b68:	mov    (%rax),%eax
+    646c4b6a:	cmp    %eax,0x978(%rbp)
+    646c4b70:	jl     646c49e8 <sgsim_run+0x203>
+    646c4b76:	mov    0x76f0(%rip),%eax        # 646cc26c <count>
+    646c4b7c:	add    $0x1,%eax
+    646c4b7f:	mov    %eax,0x76e7(%rip)        # 646cc26c <count>
+    646c4b85:	cmpl   $0x1,0x9a0(%rbp)
+    646c4b8c:	jne    646c4bc7 <sgsim_run+0x3e2>
+    646c4b8e:	mov    0x998(%rbp),%rax
+    646c4b95:	mov    0x4(%rax),%ecx
+    646c4b98:	mov    0x998(%rbp),%rax
+    646c4b9f:	mov    0x8(%rax),%r9d
+    646c4ba3:	mov    0x990(%rbp),%rax
+    646c4baa:	mov    (%rax),%r8d
+    646c4bad:	mov    0x762c(%rip),%rdx        # 646cc1e0 <variogram_array>
+    646c4bb4:	mov    0x7645(%rip),%rax        # 646cc200 <sgsim_array>
+    646c4bbb:	mov    %ecx,0x20(%rsp)
+    646c4bbf:	mov    %rax,%rcx
+    646c4bc2:	call   646c5120 <variogram>
+    646c4bc7:	mov    0x769b(%rip),%eax        # 646cc268 <flag>
+    646c4bcd:	test   %eax,%eax
+    646c4bcf:	jle    646c4be5 <sgsim_run+0x400>
+    646c4bd1:	mov    0x7695(%rip),%eax        # 646cc26c <count>
+    646c4bd7:	sub    $0x1,%eax
+    646c4bda:	mov    %eax,0x768c(%rip)        # 646cc26c <count>
+    646c4be0:	jmp    646c4c6f <sgsim_run+0x48a>
+    646c4be5:	mov    0x7680(%rip),%r8d        # 646cc26c <count>
+    646c4bec:	mov    0x990(%rbp),%rax
+    646c4bf3:	mov    0x4(%rax),%ecx
+    646c4bf6:	mov    0x990(%rbp),%rax
+    646c4bfd:	mov    (%rax),%edx
+    646c4bff:	mov    0x75fa(%rip),%rax        # 646cc200 <sgsim_array>
+    646c4c06:	mov    %r8d,0x28(%rsp)
+    646c4c0b:	mov    %ecx,0x20(%rsp)
+    646c4c0f:	lea    0x44f7(%rip),%r9        # 646c910d <.rdata+0xd>
+    646c4c16:	lea    0x4500(%rip),%r8        # 646c911d <.rdata+0x1d>
+    646c4c1d:	mov    %rax,%rcx
+    646c4c20:	call   646c451d <save_1darray>
+    646c4c25:	cmpl   $0x1,0x9a0(%rbp)
+    646c4c2c:	jne    646c4c6f <sgsim_run+0x48a>
+    646c4c2e:	mov    0x7637(%rip),%r8d        # 646cc26c <count>
+    646c4c35:	mov    0x990(%rbp),%rax
+    646c4c3c:	mov    0x4(%rax),%ecx
+    646c4c3f:	mov    0x998(%rbp),%rax
+    646c4c46:	mov    0x8(%rax),%edx
+    646c4c49:	mov    0x7590(%rip),%rax        # 646cc1e0 <variogram_array>
+    646c4c50:	mov    %r8d,0x28(%rsp)
+    646c4c55:	mov    %ecx,0x20(%rsp)
+    646c4c59:	lea    0x44ca(%rip),%r9        # 646c912a <.rdata+0x2a>
+    646c4c60:	lea    0x44dd(%rip),%r8        # 646c9144 <.rdata+0x44>
     646c4c67:	mov    %rax,%rcx
-    646c4c6a:	call   646c78f8 <free>
-    646c4c6f:	mov    0x756a(%rip),%rax        # 646cc1e0 <variogram_array>
-    646c4c76:	mov    %rax,%rcx
-    646c4c79:	call   646c78f8 <free>
-    646c4c7e:	nop
-    646c4c7f:	add    $0x20,%rsp
-    646c4c83:	pop    %rbp
-    646c4c84:	ret
-    646c4c85:	nop
-    646c4c86:	nop
-    646c4c87:	nop
-    646c4c88:	nop
-    646c4c89:	nop
-    646c4c8a:	nop
-    646c4c8b:	nop
-    646c4c8c:	nop
-    646c4c8d:	nop
-    646c4c8e:	nop
-    646c4c8f:	nop
-
-00000000646c4c90 <swap>:
-    646c4c90:	push   %rbp
-    646c4c91:	mov    %rsp,%rbp
-    646c4c94:	sub    $0x20,%rsp
-    646c4c98:	mov    %rcx,0x10(%rbp)
-    646c4c9c:	mov    %edx,0x18(%rbp)
-    646c4c9f:	mov    %r8d,0x20(%rbp)
-    646c4ca3:	mov    0x20(%rbp),%eax
-    646c4ca6:	cltq
-    646c4ca8:	lea    0x0(,%rax,8),%rdx
-    646c4cb0:	mov    0x10(%rbp),%rax
-    646c4cb4:	add    %rdx,%rax
-    646c4cb7:	mov    (%rax),%rax
-    646c4cba:	movsd  (%rax),%xmm0
-    646c4cbe:	movsd  %xmm0,-0x8(%rbp)
-    646c4cc3:	mov    0x20(%rbp),%eax
-    646c4cc6:	cltq
-    646c4cc8:	lea    0x0(,%rax,8),%rdx
-    646c4cd0:	mov    0x10(%rbp),%rax
-    646c4cd4:	add    %rdx,%rax
-    646c4cd7:	mov    (%rax),%rax
-    646c4cda:	movsd  0x8(%rax),%xmm0
-    646c4cdf:	movsd  %xmm0,-0x10(%rbp)
-    646c4ce4:	mov    0x20(%rbp),%eax
-    646c4ce7:	cltq
-    646c4ce9:	lea    0x0(,%rax,8),%rdx
-    646c4cf1:	mov    0x10(%rbp),%rax
-    646c4cf5:	add    %rdx,%rax
-    646c4cf8:	mov    (%rax),%rax
-    646c4cfb:	movsd  0x10(%rax),%xmm0
-    646c4d00:	movsd  %xmm0,-0x18(%rbp)
-    646c4d05:	mov    0x18(%rbp),%eax
-    646c4d08:	cltq
-    646c4d0a:	lea    0x0(,%rax,8),%rdx
-    646c4d12:	mov    0x10(%rbp),%rax
-    646c4d16:	add    %rdx,%rax
-    646c4d19:	mov    (%rax),%rdx
-    646c4d1c:	mov    0x20(%rbp),%eax
-    646c4d1f:	cltq
-    646c4d21:	lea    0x0(,%rax,8),%rcx
-    646c4d29:	mov    0x10(%rbp),%rax
-    646c4d2d:	add    %rcx,%rax
-    646c4d30:	mov    (%rax),%rax
-    646c4d33:	movsd  (%rdx),%xmm0
-    646c4d37:	movsd  %xmm0,(%rax)
-    646c4d3b:	mov    0x18(%rbp),%eax
-    646c4d3e:	cltq
-    646c4d40:	lea    0x0(,%rax,8),%rdx
-    646c4d48:	mov    0x10(%rbp),%rax
-    646c4d4c:	add    %rdx,%rax
-    646c4d4f:	mov    (%rax),%rdx
-    646c4d52:	mov    0x20(%rbp),%eax
-    646c4d55:	cltq
-    646c4d57:	lea    0x0(,%rax,8),%rcx
-    646c4d5f:	mov    0x10(%rbp),%rax
-    646c4d63:	add    %rcx,%rax
-    646c4d66:	mov    (%rax),%rax
-    646c4d69:	add    $0x8,%rax
-    646c4d6d:	movsd  0x8(%rdx),%xmm0
-    646c4d72:	movsd  %xmm0,(%rax)
-    646c4d76:	mov    0x18(%rbp),%eax
-    646c4d79:	cltq
-    646c4d7b:	lea    0x0(,%rax,8),%rdx
-    646c4d83:	mov    0x10(%rbp),%rax
-    646c4d87:	add    %rdx,%rax
-    646c4d8a:	mov    (%rax),%rdx
-    646c4d8d:	mov    0x20(%rbp),%eax
-    646c4d90:	cltq
-    646c4d92:	lea    0x0(,%rax,8),%rcx
-    646c4d9a:	mov    0x10(%rbp),%rax
-    646c4d9e:	add    %rcx,%rax
-    646c4da1:	mov    (%rax),%rax
-    646c4da4:	add    $0x10,%rax
-    646c4da8:	movsd  0x10(%rdx),%xmm0
-    646c4dad:	movsd  %xmm0,(%rax)
-    646c4db1:	mov    0x18(%rbp),%eax
-    646c4db4:	cltq
-    646c4db6:	lea    0x0(,%rax,8),%rdx
-    646c4dbe:	mov    0x10(%rbp),%rax
-    646c4dc2:	add    %rdx,%rax
-    646c4dc5:	mov    (%rax),%rax
-    646c4dc8:	movsd  -0x8(%rbp),%xmm0
-    646c4dcd:	movsd  %xmm0,(%rax)
-    646c4dd1:	mov    0x18(%rbp),%eax
-    646c4dd4:	cltq
-    646c4dd6:	lea    0x0(,%rax,8),%rdx
-    646c4dde:	mov    0x10(%rbp),%rax
-    646c4de2:	add    %rdx,%rax
-    646c4de5:	mov    (%rax),%rax
-    646c4de8:	add    $0x8,%rax
-    646c4dec:	movsd  -0x10(%rbp),%xmm0
-    646c4df1:	movsd  %xmm0,(%rax)
-    646c4df5:	mov    0x18(%rbp),%eax
-    646c4df8:	cltq
-    646c4dfa:	lea    0x0(,%rax,8),%rdx
-    646c4e02:	mov    0x10(%rbp),%rax
-    646c4e06:	add    %rdx,%rax
-    646c4e09:	mov    (%rax),%rax
-    646c4e0c:	add    $0x10,%rax
-    646c4e10:	movsd  -0x18(%rbp),%xmm0
-    646c4e15:	movsd  %xmm0,(%rax)
-    646c4e19:	nop
-    646c4e1a:	add    $0x20,%rsp
-    646c4e1e:	pop    %rbp
-    646c4e1f:	ret
-
-00000000646c4e20 <Partition2d>:
-    646c4e20:	push   %rbp
-    646c4e21:	mov    %rsp,%rbp
-    646c4e24:	sub    $0x30,%rsp
-    646c4e28:	mov    %rcx,0x10(%rbp)
-    646c4e2c:	mov    %edx,0x18(%rbp)
-    646c4e2f:	mov    %r8d,0x20(%rbp)
-    646c4e33:	mov    0x20(%rbp),%eax
-    646c4e36:	sub    0x18(%rbp),%eax
-    646c4e39:	mov    %eax,%edx
-    646c4e3b:	shr    $0x1f,%edx
-    646c4e3e:	add    %edx,%eax
-    646c4e40:	sar    %eax
-    646c4e42:	mov    %eax,%edx
-    646c4e44:	mov    0x18(%rbp),%eax
-    646c4e47:	add    %edx,%eax
-    646c4e49:	mov    %eax,-0x4(%rbp)
-    646c4e4c:	mov    0x18(%rbp),%eax
-    646c4e4f:	cltq
-    646c4e51:	lea    0x0(,%rax,8),%rdx
-    646c4e59:	mov    0x10(%rbp),%rax
-    646c4e5d:	add    %rdx,%rax
-    646c4e60:	mov    (%rax),%rax
-    646c4e63:	add    $0x10,%rax
-    646c4e67:	movsd  (%rax),%xmm0
-    646c4e6b:	mov    0x20(%rbp),%eax
-    646c4e6e:	cltq
-    646c4e70:	lea    0x0(,%rax,8),%rdx
-    646c4e78:	mov    0x10(%rbp),%rax
-    646c4e7c:	add    %rdx,%rax
-    646c4e7f:	mov    (%rax),%rax
-    646c4e82:	add    $0x10,%rax
-    646c4e86:	movsd  (%rax),%xmm1
-    646c4e8a:	comisd %xmm1,%xmm0
-    646c4e8e:	jbe    646c4ea4 <Partition2d+0x84>
-    646c4e90:	mov    0x20(%rbp),%edx
-    646c4e93:	mov    0x18(%rbp),%eax
-    646c4e96:	mov    %edx,%r8d
-    646c4e99:	mov    %eax,%edx
-    646c4e9b:	mov    0x10(%rbp),%rcx
-    646c4e9f:	call   646c4c90 <swap>
-    646c4ea4:	mov    -0x4(%rbp),%eax
-    646c4ea7:	cltq
-    646c4ea9:	lea    0x0(,%rax,8),%rdx
-    646c4eb1:	mov    0x10(%rbp),%rax
-    646c4eb5:	add    %rdx,%rax
-    646c4eb8:	mov    (%rax),%rax
-    646c4ebb:	add    $0x10,%rax
-    646c4ebf:	movsd  (%rax),%xmm0
+    646c4c6a:	call   646c451d <save_1darray>
+    646c4c6f:	mov    0x990(%rbp),%rax
+    646c4c76:	mov    0x4(%rax),%edx
+    646c4c79:	mov    0x75ed(%rip),%eax        # 646cc26c <count>
+    646c4c7f:	cmp    %eax,%edx
+    646c4c81:	jg     646c48ff <sgsim_run+0x11a>
+    646c4c87:	call   646c3a7b <krige_memory_free>
+    646c4c8c:	call   646c4cbe <sgsim_memory_free>
+    646c4c91:	nop
+    646c4c92:	add    $0xa00,%rsp
+    646c4c99:	pop    %rbp
+    646c4c9a:	ret
+
+00000000646c4c9b <sgsim_t_free>:
+    646c4c9b:	push   %rbp
+    646c4c9c:	mov    %rsp,%rbp
+    646c4c9f:	sub    $0x20,%rsp
+    646c4ca3:	mov    %rcx,0x10(%rbp)
+    646c4ca7:	mov    0x10(%rbp),%rax
+    646c4cab:	mov    0x10(%rax),%rax
+    646c4caf:	mov    %rax,%rcx
+    646c4cb2:	call   646c7988 <free>
+    646c4cb7:	nop
+    646c4cb8:	add    $0x20,%rsp
+    646c4cbc:	pop    %rbp
+    646c4cbd:	ret
+
+00000000646c4cbe <sgsim_memory_free>:
+    646c4cbe:	push   %rbp
+    646c4cbf:	mov    %rsp,%rbp
+    646c4cc2:	sub    $0x20,%rsp
+    646c4cc6:	mov    0x756b(%rip),%rax        # 646cc238 <_sampling+0x18>
+    646c4ccd:	mov    %rax,%rcx
+    646c4cd0:	call   646c7988 <free>
+    646c4cd5:	mov    0x7574(%rip),%rax        # 646cc250 <_sampling+0x30>
+    646c4cdc:	mov    %rax,%rcx
+    646c4cdf:	call   646c7988 <free>
+    646c4ce4:	mov    0x7515(%rip),%rax        # 646cc200 <sgsim_array>
+    646c4ceb:	mov    %rax,%rcx
+    646c4cee:	call   646c7988 <free>
+    646c4cf3:	mov    0x7486(%rip),%rax        # 646cc180 <x_grid>
+    646c4cfa:	mov    %rax,%rcx
+    646c4cfd:	call   646c7988 <free>
+    646c4d02:	mov    0x74d7(%rip),%rax        # 646cc1e0 <variogram_array>
+    646c4d09:	mov    %rax,%rcx
+    646c4d0c:	call   646c7988 <free>
+    646c4d11:	nop
+    646c4d12:	add    $0x20,%rsp
+    646c4d16:	pop    %rbp
+    646c4d17:	ret
+    646c4d18:	nop
+    646c4d19:	nop
+    646c4d1a:	nop
+    646c4d1b:	nop
+    646c4d1c:	nop
+    646c4d1d:	nop
+    646c4d1e:	nop
+    646c4d1f:	nop
+
+00000000646c4d20 <swap>:
+    646c4d20:	push   %rbp
+    646c4d21:	mov    %rsp,%rbp
+    646c4d24:	sub    $0x20,%rsp
+    646c4d28:	mov    %rcx,0x10(%rbp)
+    646c4d2c:	mov    %edx,0x18(%rbp)
+    646c4d2f:	mov    %r8d,0x20(%rbp)
+    646c4d33:	mov    0x20(%rbp),%eax
+    646c4d36:	cltq
+    646c4d38:	lea    0x0(,%rax,8),%rdx
+    646c4d40:	mov    0x10(%rbp),%rax
+    646c4d44:	add    %rdx,%rax
+    646c4d47:	mov    (%rax),%rax
+    646c4d4a:	movsd  (%rax),%xmm0
+    646c4d4e:	movsd  %xmm0,-0x8(%rbp)
+    646c4d53:	mov    0x20(%rbp),%eax
+    646c4d56:	cltq
+    646c4d58:	lea    0x0(,%rax,8),%rdx
+    646c4d60:	mov    0x10(%rbp),%rax
+    646c4d64:	add    %rdx,%rax
+    646c4d67:	mov    (%rax),%rax
+    646c4d6a:	movsd  0x8(%rax),%xmm0
+    646c4d6f:	movsd  %xmm0,-0x10(%rbp)
+    646c4d74:	mov    0x20(%rbp),%eax
+    646c4d77:	cltq
+    646c4d79:	lea    0x0(,%rax,8),%rdx
+    646c4d81:	mov    0x10(%rbp),%rax
+    646c4d85:	add    %rdx,%rax
+    646c4d88:	mov    (%rax),%rax
+    646c4d8b:	movsd  0x10(%rax),%xmm0
+    646c4d90:	movsd  %xmm0,-0x18(%rbp)
+    646c4d95:	mov    0x18(%rbp),%eax
+    646c4d98:	cltq
+    646c4d9a:	lea    0x0(,%rax,8),%rdx
+    646c4da2:	mov    0x10(%rbp),%rax
+    646c4da6:	add    %rdx,%rax
+    646c4da9:	mov    (%rax),%rdx
+    646c4dac:	mov    0x20(%rbp),%eax
+    646c4daf:	cltq
+    646c4db1:	lea    0x0(,%rax,8),%rcx
+    646c4db9:	mov    0x10(%rbp),%rax
+    646c4dbd:	add    %rcx,%rax
+    646c4dc0:	mov    (%rax),%rax
+    646c4dc3:	movsd  (%rdx),%xmm0
+    646c4dc7:	movsd  %xmm0,(%rax)
+    646c4dcb:	mov    0x18(%rbp),%eax
+    646c4dce:	cltq
+    646c4dd0:	lea    0x0(,%rax,8),%rdx
+    646c4dd8:	mov    0x10(%rbp),%rax
+    646c4ddc:	add    %rdx,%rax
+    646c4ddf:	mov    (%rax),%rdx
+    646c4de2:	mov    0x20(%rbp),%eax
+    646c4de5:	cltq
+    646c4de7:	lea    0x0(,%rax,8),%rcx
+    646c4def:	mov    0x10(%rbp),%rax
+    646c4df3:	add    %rcx,%rax
+    646c4df6:	mov    (%rax),%rax
+    646c4df9:	add    $0x8,%rax
+    646c4dfd:	movsd  0x8(%rdx),%xmm0
+    646c4e02:	movsd  %xmm0,(%rax)
+    646c4e06:	mov    0x18(%rbp),%eax
+    646c4e09:	cltq
+    646c4e0b:	lea    0x0(,%rax,8),%rdx
+    646c4e13:	mov    0x10(%rbp),%rax
+    646c4e17:	add    %rdx,%rax
+    646c4e1a:	mov    (%rax),%rdx
+    646c4e1d:	mov    0x20(%rbp),%eax
+    646c4e20:	cltq
+    646c4e22:	lea    0x0(,%rax,8),%rcx
+    646c4e2a:	mov    0x10(%rbp),%rax
+    646c4e2e:	add    %rcx,%rax
+    646c4e31:	mov    (%rax),%rax
+    646c4e34:	add    $0x10,%rax
+    646c4e38:	movsd  0x10(%rdx),%xmm0
+    646c4e3d:	movsd  %xmm0,(%rax)
+    646c4e41:	mov    0x18(%rbp),%eax
+    646c4e44:	cltq
+    646c4e46:	lea    0x0(,%rax,8),%rdx
+    646c4e4e:	mov    0x10(%rbp),%rax
+    646c4e52:	add    %rdx,%rax
+    646c4e55:	mov    (%rax),%rax
+    646c4e58:	movsd  -0x8(%rbp),%xmm0
+    646c4e5d:	movsd  %xmm0,(%rax)
+    646c4e61:	mov    0x18(%rbp),%eax
+    646c4e64:	cltq
+    646c4e66:	lea    0x0(,%rax,8),%rdx
+    646c4e6e:	mov    0x10(%rbp),%rax
+    646c4e72:	add    %rdx,%rax
+    646c4e75:	mov    (%rax),%rax
+    646c4e78:	add    $0x8,%rax
+    646c4e7c:	movsd  -0x10(%rbp),%xmm0
+    646c4e81:	movsd  %xmm0,(%rax)
+    646c4e85:	mov    0x18(%rbp),%eax
+    646c4e88:	cltq
+    646c4e8a:	lea    0x0(,%rax,8),%rdx
+    646c4e92:	mov    0x10(%rbp),%rax
+    646c4e96:	add    %rdx,%rax
+    646c4e99:	mov    (%rax),%rax
+    646c4e9c:	add    $0x10,%rax
+    646c4ea0:	movsd  -0x18(%rbp),%xmm0
+    646c4ea5:	movsd  %xmm0,(%rax)
+    646c4ea9:	nop
+    646c4eaa:	add    $0x20,%rsp
+    646c4eae:	pop    %rbp
+    646c4eaf:	ret
+
+00000000646c4eb0 <Partition2d>:
+    646c4eb0:	push   %rbp
+    646c4eb1:	mov    %rsp,%rbp
+    646c4eb4:	sub    $0x30,%rsp
+    646c4eb8:	mov    %rcx,0x10(%rbp)
+    646c4ebc:	mov    %edx,0x18(%rbp)
+    646c4ebf:	mov    %r8d,0x20(%rbp)
     646c4ec3:	mov    0x20(%rbp),%eax
-    646c4ec6:	cltq
-    646c4ec8:	lea    0x0(,%rax,8),%rdx
-    646c4ed0:	mov    0x10(%rbp),%rax
-    646c4ed4:	add    %rdx,%rax
-    646c4ed7:	mov    (%rax),%rax
-    646c4eda:	add    $0x10,%rax
-    646c4ede:	movsd  (%rax),%xmm1
-    646c4ee2:	comisd %xmm1,%xmm0
-    646c4ee6:	jbe    646c4efc <Partition2d+0xdc>
-    646c4ee8:	mov    0x20(%rbp),%edx
-    646c4eeb:	mov    -0x4(%rbp),%eax
-    646c4eee:	mov    %edx,%r8d
-    646c4ef1:	mov    %eax,%edx
-    646c4ef3:	mov    0x10(%rbp),%rcx
-    646c4ef7:	call   646c4c90 <swap>
-    646c4efc:	mov    -0x4(%rbp),%eax
-    646c4eff:	cltq
-    646c4f01:	lea    0x0(,%rax,8),%rdx
-    646c4f09:	mov    0x10(%rbp),%rax
-    646c4f0d:	add    %rdx,%rax
-    646c4f10:	mov    (%rax),%rax
-    646c4f13:	add    $0x10,%rax
-    646c4f17:	movsd  (%rax),%xmm0
-    646c4f1b:	mov    0x18(%rbp),%eax
-    646c4f1e:	cltq
-    646c4f20:	lea    0x0(,%rax,8),%rdx
-    646c4f28:	mov    0x10(%rbp),%rax
-    646c4f2c:	add    %rdx,%rax
-    646c4f2f:	mov    (%rax),%rax
-    646c4f32:	add    $0x10,%rax
-    646c4f36:	movsd  (%rax),%xmm1
-    646c4f3a:	comisd %xmm1,%xmm0
-    646c4f3e:	jbe    646c4f54 <Partition2d+0x134>
-    646c4f40:	mov    0x18(%rbp),%edx
-    646c4f43:	mov    -0x4(%rbp),%eax
-    646c4f46:	mov    %edx,%r8d
-    646c4f49:	mov    %eax,%edx
-    646c4f4b:	mov    0x10(%rbp),%rcx
-    646c4f4f:	call   646c4c90 <swap>
-    646c4f54:	mov    0x18(%rbp),%eax
-    646c4f57:	cltq
-    646c4f59:	lea    0x0(,%rax,8),%rdx
-    646c4f61:	mov    0x10(%rbp),%rax
-    646c4f65:	add    %rdx,%rax
-    646c4f68:	mov    (%rax),%rax
-    646c4f6b:	movsd  0x10(%rax),%xmm0
-    646c4f70:	movsd  %xmm0,-0x10(%rbp)
-    646c4f75:	jmp    646c500c <Partition2d+0x1ec>
-    646c4f7a:	subl   $0x1,0x20(%rbp)
-    646c4f7e:	mov    0x18(%rbp),%eax
-    646c4f81:	cmp    0x20(%rbp),%eax
-    646c4f84:	jge    646c4fac <Partition2d+0x18c>
-    646c4f86:	mov    0x20(%rbp),%eax
-    646c4f89:	cltq
-    646c4f8b:	lea    0x0(,%rax,8),%rdx
-    646c4f93:	mov    0x10(%rbp),%rax
-    646c4f97:	add    %rdx,%rax
-    646c4f9a:	mov    (%rax),%rax
-    646c4f9d:	add    $0x10,%rax
-    646c4fa1:	movsd  (%rax),%xmm0
-    646c4fa5:	comisd -0x10(%rbp),%xmm0
-    646c4faa:	jae    646c4f7a <Partition2d+0x15a>
-    646c4fac:	mov    0x20(%rbp),%edx
-    646c4faf:	mov    0x18(%rbp),%eax
-    646c4fb2:	mov    %edx,%r8d
-    646c4fb5:	mov    %eax,%edx
-    646c4fb7:	mov    0x10(%rbp),%rcx
-    646c4fbb:	call   646c4c90 <swap>
-    646c4fc0:	jmp    646c4fc6 <Partition2d+0x1a6>
-    646c4fc2:	addl   $0x1,0x18(%rbp)
-    646c4fc6:	mov    0x18(%rbp),%eax
-    646c4fc9:	cmp    0x20(%rbp),%eax
-    646c4fcc:	jge    646c4ff8 <Partition2d+0x1d8>
-    646c4fce:	mov    0x18(%rbp),%eax
-    646c4fd1:	cltq
-    646c4fd3:	lea    0x0(,%rax,8),%rdx
-    646c4fdb:	mov    0x10(%rbp),%rax
-    646c4fdf:	add    %rdx,%rax
-    646c4fe2:	mov    (%rax),%rax
-    646c4fe5:	add    $0x10,%rax
-    646c4fe9:	movsd  (%rax),%xmm1
-    646c4fed:	movsd  -0x10(%rbp),%xmm0
-    646c4ff2:	comisd %xmm1,%xmm0
-    646c4ff6:	jae    646c4fc2 <Partition2d+0x1a2>
-    646c4ff8:	mov    0x20(%rbp),%edx
-    646c4ffb:	mov    0x18(%rbp),%eax
-    646c4ffe:	mov    %edx,%r8d
-    646c5001:	mov    %eax,%edx
-    646c5003:	mov    0x10(%rbp),%rcx
-    646c5007:	call   646c4c90 <swap>
-    646c500c:	mov    0x18(%rbp),%eax
-    646c500f:	cmp    0x20(%rbp),%eax
-    646c5012:	jl     646c4f7e <Partition2d+0x15e>
-    646c5018:	mov    0x18(%rbp),%eax
-    646c501b:	add    $0x30,%rsp
-    646c501f:	pop    %rbp
-    646c5020:	ret
-
-00000000646c5021 <quicksort2d>:
-    646c5021:	push   %rbp
-    646c5022:	mov    %rsp,%rbp
-    646c5025:	sub    $0x30,%rsp
-    646c5029:	mov    %rcx,0x10(%rbp)
-    646c502d:	mov    %edx,0x18(%rbp)
-    646c5030:	mov    %r8d,0x20(%rbp)
-    646c5034:	mov    0x18(%rbp),%eax
-    646c5037:	cmp    0x20(%rbp),%eax
-    646c503a:	jge    646c5081 <quicksort2d+0x60>
+    646c4ec6:	sub    0x18(%rbp),%eax
+    646c4ec9:	mov    %eax,%edx
+    646c4ecb:	shr    $0x1f,%edx
+    646c4ece:	add    %edx,%eax
+    646c4ed0:	sar    %eax
+    646c4ed2:	mov    %eax,%edx
+    646c4ed4:	mov    0x18(%rbp),%eax
+    646c4ed7:	add    %edx,%eax
+    646c4ed9:	mov    %eax,-0x4(%rbp)
+    646c4edc:	mov    0x18(%rbp),%eax
+    646c4edf:	cltq
+    646c4ee1:	lea    0x0(,%rax,8),%rdx
+    646c4ee9:	mov    0x10(%rbp),%rax
+    646c4eed:	add    %rdx,%rax
+    646c4ef0:	mov    (%rax),%rax
+    646c4ef3:	add    $0x10,%rax
+    646c4ef7:	movsd  (%rax),%xmm0
+    646c4efb:	mov    0x20(%rbp),%eax
+    646c4efe:	cltq
+    646c4f00:	lea    0x0(,%rax,8),%rdx
+    646c4f08:	mov    0x10(%rbp),%rax
+    646c4f0c:	add    %rdx,%rax
+    646c4f0f:	mov    (%rax),%rax
+    646c4f12:	add    $0x10,%rax
+    646c4f16:	movsd  (%rax),%xmm1
+    646c4f1a:	comisd %xmm1,%xmm0
+    646c4f1e:	jbe    646c4f34 <Partition2d+0x84>
+    646c4f20:	mov    0x20(%rbp),%edx
+    646c4f23:	mov    0x18(%rbp),%eax
+    646c4f26:	mov    %edx,%r8d
+    646c4f29:	mov    %eax,%edx
+    646c4f2b:	mov    0x10(%rbp),%rcx
+    646c4f2f:	call   646c4d20 <swap>
+    646c4f34:	mov    -0x4(%rbp),%eax
+    646c4f37:	cltq
+    646c4f39:	lea    0x0(,%rax,8),%rdx
+    646c4f41:	mov    0x10(%rbp),%rax
+    646c4f45:	add    %rdx,%rax
+    646c4f48:	mov    (%rax),%rax
+    646c4f4b:	add    $0x10,%rax
+    646c4f4f:	movsd  (%rax),%xmm0
+    646c4f53:	mov    0x20(%rbp),%eax
+    646c4f56:	cltq
+    646c4f58:	lea    0x0(,%rax,8),%rdx
+    646c4f60:	mov    0x10(%rbp),%rax
+    646c4f64:	add    %rdx,%rax
+    646c4f67:	mov    (%rax),%rax
+    646c4f6a:	add    $0x10,%rax
+    646c4f6e:	movsd  (%rax),%xmm1
+    646c4f72:	comisd %xmm1,%xmm0
+    646c4f76:	jbe    646c4f8c <Partition2d+0xdc>
+    646c4f78:	mov    0x20(%rbp),%edx
+    646c4f7b:	mov    -0x4(%rbp),%eax
+    646c4f7e:	mov    %edx,%r8d
+    646c4f81:	mov    %eax,%edx
+    646c4f83:	mov    0x10(%rbp),%rcx
+    646c4f87:	call   646c4d20 <swap>
+    646c4f8c:	mov    -0x4(%rbp),%eax
+    646c4f8f:	cltq
+    646c4f91:	lea    0x0(,%rax,8),%rdx
+    646c4f99:	mov    0x10(%rbp),%rax
+    646c4f9d:	add    %rdx,%rax
+    646c4fa0:	mov    (%rax),%rax
+    646c4fa3:	add    $0x10,%rax
+    646c4fa7:	movsd  (%rax),%xmm0
+    646c4fab:	mov    0x18(%rbp),%eax
+    646c4fae:	cltq
+    646c4fb0:	lea    0x0(,%rax,8),%rdx
+    646c4fb8:	mov    0x10(%rbp),%rax
+    646c4fbc:	add    %rdx,%rax
+    646c4fbf:	mov    (%rax),%rax
+    646c4fc2:	add    $0x10,%rax
+    646c4fc6:	movsd  (%rax),%xmm1
+    646c4fca:	comisd %xmm1,%xmm0
+    646c4fce:	jbe    646c4fe4 <Partition2d+0x134>
+    646c4fd0:	mov    0x18(%rbp),%edx
+    646c4fd3:	mov    -0x4(%rbp),%eax
+    646c4fd6:	mov    %edx,%r8d
+    646c4fd9:	mov    %eax,%edx
+    646c4fdb:	mov    0x10(%rbp),%rcx
+    646c4fdf:	call   646c4d20 <swap>
+    646c4fe4:	mov    0x18(%rbp),%eax
+    646c4fe7:	cltq
+    646c4fe9:	lea    0x0(,%rax,8),%rdx
+    646c4ff1:	mov    0x10(%rbp),%rax
+    646c4ff5:	add    %rdx,%rax
+    646c4ff8:	mov    (%rax),%rax
+    646c4ffb:	movsd  0x10(%rax),%xmm0
+    646c5000:	movsd  %xmm0,-0x10(%rbp)
+    646c5005:	jmp    646c509c <Partition2d+0x1ec>
+    646c500a:	subl   $0x1,0x20(%rbp)
+    646c500e:	mov    0x18(%rbp),%eax
+    646c5011:	cmp    0x20(%rbp),%eax
+    646c5014:	jge    646c503c <Partition2d+0x18c>
+    646c5016:	mov    0x20(%rbp),%eax
+    646c5019:	cltq
+    646c501b:	lea    0x0(,%rax,8),%rdx
+    646c5023:	mov    0x10(%rbp),%rax
+    646c5027:	add    %rdx,%rax
+    646c502a:	mov    (%rax),%rax
+    646c502d:	add    $0x10,%rax
+    646c5031:	movsd  (%rax),%xmm0
+    646c5035:	comisd -0x10(%rbp),%xmm0
+    646c503a:	jae    646c500a <Partition2d+0x15a>
     646c503c:	mov    0x20(%rbp),%edx
     646c503f:	mov    0x18(%rbp),%eax
     646c5042:	mov    %edx,%r8d
     646c5045:	mov    %eax,%edx
     646c5047:	mov    0x10(%rbp),%rcx
-    646c504b:	call   646c4e20 <Partition2d>
-    646c5050:	mov    %eax,-0x4(%rbp)
-    646c5053:	mov    -0x4(%rbp),%eax
-    646c5056:	lea    -0x1(%rax),%edx
-    646c5059:	mov    0x18(%rbp),%eax
-    646c505c:	mov    %edx,%r8d
-    646c505f:	mov    %eax,%edx
-    646c5061:	mov    0x10(%rbp),%rcx
-    646c5065:	call   646c5021 <quicksort2d>
-    646c506a:	mov    -0x4(%rbp),%eax
-    646c506d:	add    $0x1,%eax
-    646c5070:	mov    0x20(%rbp),%edx
-    646c5073:	mov    %edx,%r8d
-    646c5076:	mov    %eax,%edx
-    646c5078:	mov    0x10(%rbp),%rcx
-    646c507c:	call   646c5021 <quicksort2d>
-    646c5081:	nop
-    646c5082:	add    $0x30,%rsp
-    646c5086:	pop    %rbp
-    646c5087:	ret
-    646c5088:	nop
-    646c5089:	nop
-    646c508a:	nop
-    646c508b:	nop
-    646c508c:	nop
-    646c508d:	nop
-    646c508e:	nop
-    646c508f:	nop
-
-00000000646c5090 <variogram>:
-    646c5090:	push   %rbp
-    646c5091:	push   %rbx
-    646c5092:	sub    $0x88,%rsp
-    646c5099:	lea    0x80(%rsp),%rbp
-    646c50a1:	mov    %rcx,0x20(%rbp)
-    646c50a5:	mov    %rdx,0x28(%rbp)
-    646c50a9:	mov    %r8d,0x30(%rbp)
-    646c50ad:	mov    %r9d,0x38(%rbp)
-    646c50b1:	mov    0x30(%rbp),%eax
-    646c50b4:	cltq
-    646c50b6:	mov    %rax,-0x58(%rbp)
-    646c50ba:	mov    0x30(%rbp),%eax
-    646c50bd:	cltq
-    646c50bf:	mov    %rax,-0x50(%rbp)
-    646c50c3:	mov    0x30(%rbp),%eax
-    646c50c6:	cltq
-    646c50c8:	shl    $0x3,%rax
-    646c50cc:	mov    %rax,%rcx
-    646c50cf:	call   646c78e0 <malloc>
-    646c50d4:	mov    %rax,-0x60(%rbp)
-    646c50d8:	movl   $0x0,-0x14(%rbp)
-    646c50df:	jmp    646c510b <variogram+0x7b>
-    646c50e1:	mov    0x30(%rbp),%eax
-    646c50e4:	cltq
-    646c50e6:	shl    $0x3,%rax
-    646c50ea:	mov    -0x60(%rbp),%rcx
-    646c50ee:	mov    -0x14(%rbp),%edx
-    646c50f1:	movslq %edx,%rdx
-    646c50f4:	shl    $0x3,%rdx
-    646c50f8:	lea    (%rcx,%rdx,1),%rbx
-    646c50fc:	mov    %rax,%rcx
-    646c50ff:	call   646c78e0 <malloc>
-    646c5104:	mov    %rax,(%rbx)
-    646c5107:	addl   $0x1,-0x14(%rbp)
-    646c510b:	mov    -0x14(%rbp),%eax
-    646c510e:	cmp    0x30(%rbp),%eax
-    646c5111:	jl     646c50e1 <variogram+0x51>
-    646c5113:	mov    0x30(%rbp),%eax
-    646c5116:	mov    %eax,%ecx
-    646c5118:	call   646c42e1 <d_arange>
-    646c511d:	mov    %rax,-0x40(%rbp)
-    646c5121:	mov    -0x60(%rbp),%rdx
-    646c5125:	mov    -0x40(%rbp),%rax
-    646c5129:	mov    0x30(%rbp),%ecx
-    646c512c:	mov    %ecx,%r8d
-    646c512f:	mov    %rax,%rcx
-    646c5132:	call   646c433d <pdist>
-    646c5137:	movl   $0x0,-0x18(%rbp)
-    646c513e:	jmp    646c52a7 <variogram+0x217>
-    646c5143:	pxor   %xmm0,%xmm0
-    646c5147:	movsd  %xmm0,-0x8(%rbp)
-    646c514c:	pxor   %xmm0,%xmm0
-    646c5150:	movsd  %xmm0,-0x10(%rbp)
-    646c5155:	movl   $0x0,-0x1c(%rbp)
-    646c515c:	jmp    646c5258 <variogram+0x1c8>
-    646c5161:	mov    -0x1c(%rbp),%eax
-    646c5164:	add    $0x1,%eax
-    646c5167:	mov    %eax,-0x20(%rbp)
-    646c516a:	jmp    646c5248 <variogram+0x1b8>
-    646c516f:	mov    -0x60(%rbp),%rdx
-    646c5173:	mov    -0x1c(%rbp),%eax
-    646c5176:	cltq
-    646c5178:	shl    $0x3,%rax
-    646c517c:	add    %rdx,%rax
-    646c517f:	mov    (%rax),%rdx
-    646c5182:	mov    -0x20(%rbp),%eax
-    646c5185:	cltq
-    646c5187:	shl    $0x3,%rax
-    646c518b:	add    %rdx,%rax
-    646c518e:	movsd  (%rax),%xmm0
-    646c5192:	mov    -0x18(%rbp),%eax
-    646c5195:	sub    0x40(%rbp),%eax
-    646c5198:	cvtsi2sd %eax,%xmm1
-    646c519c:	comisd %xmm1,%xmm0
-    646c51a0:	jb     646c5244 <variogram+0x1b4>
-    646c51a6:	mov    -0x60(%rbp),%rdx
-    646c51aa:	mov    -0x1c(%rbp),%eax
-    646c51ad:	cltq
-    646c51af:	shl    $0x3,%rax
-    646c51b3:	add    %rdx,%rax
-    646c51b6:	mov    (%rax),%rdx
-    646c51b9:	mov    -0x20(%rbp),%eax
-    646c51bc:	cltq
-    646c51be:	shl    $0x3,%rax
-    646c51c2:	add    %rdx,%rax
-    646c51c5:	movsd  (%rax),%xmm1
-    646c51c9:	mov    -0x18(%rbp),%edx
-    646c51cc:	mov    0x40(%rbp),%eax
-    646c51cf:	add    %edx,%eax
-    646c51d1:	cvtsi2sd %eax,%xmm0
-    646c51d5:	comisd %xmm1,%xmm0
-    646c51d9:	jb     646c5244 <variogram+0x1b4>
-    646c51db:	mov    -0x1c(%rbp),%eax
-    646c51de:	cltq
-    646c51e0:	lea    0x0(,%rax,8),%rdx
-    646c51e8:	mov    0x20(%rbp),%rax
-    646c51ec:	add    %rdx,%rax
-    646c51ef:	movsd  (%rax),%xmm0
-    646c51f3:	mov    -0x20(%rbp),%eax
-    646c51f6:	cltq
-    646c51f8:	lea    0x0(,%rax,8),%rdx
-    646c5200:	mov    0x20(%rbp),%rax
-    646c5204:	add    %rdx,%rax
-    646c5207:	movsd  (%rax),%xmm1
-    646c520b:	subsd  %xmm1,%xmm0
-    646c520f:	movsd  0x3f49(%rip),%xmm1        # 646c9160 <.rdata>
-    646c5217:	call   646c6ed0 <pow>
-    646c521c:	movapd %xmm0,%xmm1
-    646c5220:	movsd  -0x8(%rbp),%xmm0
-    646c5225:	addsd  %xmm1,%xmm0
-    646c5229:	movsd  %xmm0,-0x8(%rbp)
-    646c522e:	movsd  -0x10(%rbp),%xmm1
-    646c5233:	movsd  0x3f2d(%rip),%xmm0        # 646c9168 <.rdata+0x8>
-    646c523b:	addsd  %xmm1,%xmm0
-    646c523f:	movsd  %xmm0,-0x10(%rbp)
-    646c5244:	addl   $0x1,-0x20(%rbp)
-    646c5248:	mov    -0x20(%rbp),%eax
-    646c524b:	cmp    0x30(%rbp),%eax
-    646c524e:	jl     646c516f <variogram+0xdf>
-    646c5254:	addl   $0x1,-0x1c(%rbp)
-    646c5258:	mov    -0x1c(%rbp),%eax
-    646c525b:	cmp    0x30(%rbp),%eax
-    646c525e:	jl     646c5161 <variogram+0xd1>
-    646c5264:	movsd  -0x8(%rbp),%xmm0
-    646c5269:	comisd 0x3eff(%rip),%xmm0        # 646c9170 <.rdata+0x10>
-    646c5271:	jb     646c52a1 <variogram+0x211>
-    646c5273:	movsd  -0x10(%rbp),%xmm0
-    646c5278:	movapd %xmm0,%xmm1
-    646c527c:	addsd  %xmm0,%xmm1
-    646c5280:	mov    -0x18(%rbp),%eax
-    646c5283:	cltq
-    646c5285:	lea    0x0(,%rax,8),%rdx
-    646c528d:	mov    0x28(%rbp),%rax
-    646c5291:	add    %rdx,%rax
-    646c5294:	movsd  -0x8(%rbp),%xmm0
-    646c5299:	divsd  %xmm1,%xmm0
-    646c529d:	movsd  %xmm0,(%rax)
-    646c52a1:	mov    0x40(%rbp),%eax
-    646c52a4:	add    %eax,-0x18(%rbp)
-    646c52a7:	mov    -0x18(%rbp),%eax
-    646c52aa:	cmp    0x38(%rbp),%eax
-    646c52ad:	jl     646c5143 <variogram+0xb3>
-    646c52b3:	mov    -0x40(%rbp),%rax
-    646c52b7:	mov    %rax,%rcx
-    646c52ba:	call   646c78f8 <free>
-    646c52bf:	movl   $0x0,-0x24(%rbp)
-    646c52c6:	jmp    646c52e7 <variogram+0x257>
-    646c52c8:	mov    -0x60(%rbp),%rdx
-    646c52cc:	mov    -0x24(%rbp),%eax
-    646c52cf:	cltq
-    646c52d1:	shl    $0x3,%rax
-    646c52d5:	add    %rdx,%rax
-    646c52d8:	mov    (%rax),%rax
-    646c52db:	mov    %rax,%rcx
-    646c52de:	call   646c78f8 <free>
-    646c52e3:	addl   $0x1,-0x24(%rbp)
-    646c52e7:	mov    -0x24(%rbp),%eax
-    646c52ea:	cltq
-    646c52ec:	mov    -0x58(%rbp),%rdx
-    646c52f0:	cmp    %rdx,%rax
-    646c52f3:	jb     646c52c8 <variogram+0x238>
-    646c52f5:	mov    -0x60(%rbp),%rax
-    646c52f9:	mov    %rax,%rcx
-    646c52fc:	call   646c78f8 <free>
-    646c5301:	nop
-    646c5302:	add    $0x88,%rsp
-    646c5309:	pop    %rbx
-    646c530a:	pop    %rbp
-    646c530b:	ret
-
-00000000646c530c <variance>:
-    646c530c:	push   %rbp
-    646c530d:	mov    %rsp,%rbp
-    646c5310:	sub    $0x40,%rsp
-    646c5314:	mov    %rcx,0x10(%rbp)
-    646c5318:	mov    %edx,0x18(%rbp)
-    646c531b:	pxor   %xmm0,%xmm0
-    646c531f:	movsd  %xmm0,-0x8(%rbp)
-    646c5324:	pxor   %xmm0,%xmm0
-    646c5328:	movsd  %xmm0,-0x10(%rbp)
-    646c532d:	movl   $0x0,-0x14(%rbp)
-    646c5334:	jmp    646c5360 <variance+0x54>
-    646c5336:	mov    -0x14(%rbp),%eax
-    646c5339:	cltq
-    646c533b:	lea    0x0(,%rax,8),%rdx
-    646c5343:	mov    0x10(%rbp),%rax
-    646c5347:	add    %rdx,%rax
-    646c534a:	movsd  (%rax),%xmm0
-    646c534e:	movsd  -0x8(%rbp),%xmm1
-    646c5353:	addsd  %xmm1,%xmm0
-    646c5357:	movsd  %xmm0,-0x8(%rbp)
-    646c535c:	addl   $0x1,-0x14(%rbp)
-    646c5360:	mov    -0x14(%rbp),%eax
-    646c5363:	cmp    0x18(%rbp),%eax
-    646c5366:	jl     646c5336 <variance+0x2a>
-    646c5368:	cvtsi2sdl 0x18(%rbp),%xmm1
-    646c536d:	movsd  -0x8(%rbp),%xmm0
-    646c5372:	divsd  %xmm1,%xmm0
-    646c5376:	movsd  %xmm0,-0x8(%rbp)
-    646c537b:	movl   $0x0,-0x18(%rbp)
-    646c5382:	jmp    646c53c4 <variance+0xb8>
-    646c5384:	mov    -0x18(%rbp),%eax
-    646c5387:	cltq
-    646c5389:	lea    0x0(,%rax,8),%rdx
-    646c5391:	mov    0x10(%rbp),%rax
-    646c5395:	add    %rdx,%rax
-    646c5398:	movsd  (%rax),%xmm0
-    646c539c:	subsd  -0x8(%rbp),%xmm0
-    646c53a1:	movsd  0x3db7(%rip),%xmm1        # 646c9160 <.rdata>
-    646c53a9:	call   646c6ed0 <pow>
-    646c53ae:	movapd %xmm0,%xmm1
-    646c53b2:	movsd  -0x10(%rbp),%xmm0
-    646c53b7:	addsd  %xmm1,%xmm0
-    646c53bb:	movsd  %xmm0,-0x10(%rbp)
-    646c53c0:	addl   $0x1,-0x18(%rbp)
-    646c53c4:	mov    -0x18(%rbp),%eax
-    646c53c7:	cmp    0x18(%rbp),%eax
-    646c53ca:	jl     646c5384 <variance+0x78>
-    646c53cc:	cvtsi2sdl 0x18(%rbp),%xmm1
-    646c53d1:	movsd  -0x10(%rbp),%xmm0
-    646c53d6:	divsd  %xmm1,%xmm0
-    646c53da:	movsd  %xmm0,-0x10(%rbp)
-    646c53df:	movsd  -0x10(%rbp),%xmm0
-    646c53e4:	movq   %xmm0,%rax
-    646c53e9:	movq   %rax,%xmm0
-    646c53ee:	add    $0x40,%rsp
-    646c53f2:	pop    %rbp
-    646c53f3:	ret
-    646c53f4:	nop
-    646c53f5:	nop
-    646c53f6:	nop
-    646c53f7:	nop
-    646c53f8:	nop
-    646c53f9:	nop
-    646c53fa:	nop
-    646c53fb:	nop
-    646c53fc:	nop
-    646c53fd:	nop
-    646c53fe:	nop
-    646c53ff:	nop
-
-00000000646c5400 <Sleep>:
-    646c5400:	jmp    *0x8e46(%rip)        # 646ce24c <__imp_Sleep>
-    646c5406:	nop
-    646c5407:	nop
-    646c5408:	nopl   0x0(%rax,%rax,1)
-
-00000000646c5410 <__do_global_dtors>:
-    646c5410:	sub    $0x28,%rsp
-    646c5414:	mov    0x2be5(%rip),%rax        # 646c8000 <__data_start__>
-    646c541b:	mov    (%rax),%rax
-    646c541e:	test   %rax,%rax
-    646c5421:	je     646c5440 <__do_global_dtors+0x30>
-    646c5423:	call   *%rax
-    646c5425:	mov    0x2bd4(%rip),%rax        # 646c8000 <__data_start__>
-    646c542c:	lea    0x8(%rax),%rdx
-    646c5430:	mov    0x8(%rax),%rax
-    646c5434:	mov    %rdx,0x2bc5(%rip)        # 646c8000 <__data_start__>
-    646c543b:	test   %rax,%rax
-    646c543e:	jne    646c5423 <__do_global_dtors+0x13>
-    646c5440:	add    $0x28,%rsp
-    646c5444:	ret
-    646c5445:	nop
-    646c5446:	cs nopw 0x0(%rax,%rax,1)
-
-00000000646c5450 <__do_global_ctors>:
-    646c5450:	push   %rsi
-    646c5451:	push   %rbx
-    646c5452:	sub    $0x28,%rsp
-    646c5456:	mov    0x4193(%rip),%rcx        # 646c95f0 <.refptr.__CTOR_LIST__>
-    646c545d:	mov    (%rcx),%rdx
-    646c5460:	cmp    $0xffffffff,%edx
-    646c5463:	mov    %edx,%eax
-    646c5465:	je     646c54a0 <__do_global_ctors+0x50>
-    646c5467:	test   %eax,%eax
-    646c5469:	je     646c548b <__do_global_ctors+0x3b>
-    646c546b:	mov    %eax,%edx
-    646c546d:	sub    $0x1,%eax
-    646c5470:	lea    (%rcx,%rdx,8),%rbx
-    646c5474:	sub    %rax,%rdx
-    646c5477:	lea    -0x8(%rcx,%rdx,8),%rsi
-    646c547c:	nopl   0x0(%rax)
-    646c5480:	call   *(%rbx)
-    646c5482:	sub    $0x8,%rbx
-    646c5486:	cmp    %rsi,%rbx
-    646c5489:	jne    646c5480 <__do_global_ctors+0x30>
-    646c548b:	lea    -0x82(%rip),%rcx        # 646c5410 <__do_global_dtors>
-    646c5492:	add    $0x28,%rsp
-    646c5496:	pop    %rbx
-    646c5497:	pop    %rsi
-    646c5498:	jmp    646c1380 <atexit>
-    646c549d:	nopl   (%rax)
-    646c54a0:	xor    %eax,%eax
-    646c54a2:	jmp    646c54a6 <__do_global_ctors+0x56>
-    646c54a4:	mov    %edx,%eax
-    646c54a6:	lea    0x1(%rax),%r8d
-    646c54aa:	cmpq   $0x0,(%rcx,%r8,8)
-    646c54af:	mov    %r8,%rdx
-    646c54b2:	jne    646c54a4 <__do_global_ctors+0x54>
-    646c54b4:	jmp    646c5467 <__do_global_ctors+0x17>
-    646c54b6:	cs nopw 0x0(%rax,%rax,1)
-
-00000000646c54c0 <__main>:
-    646c54c0:	mov    0x6dba(%rip),%eax        # 646cc280 <initialized>
-    646c54c6:	test   %eax,%eax
-    646c54c8:	je     646c54d0 <__main+0x10>
-    646c54ca:	ret
-    646c54cb:	nopl   0x0(%rax,%rax,1)
-    646c54d0:	movl   $0x1,0x6da6(%rip)        # 646cc280 <initialized>
-    646c54da:	jmp    646c5450 <__do_global_ctors>
-    646c54df:	nop
-
-00000000646c54e0 <__security_init_cookie>:
-    646c54e0:	push   %r12
-    646c54e2:	push   %rbp
-    646c54e3:	push   %rdi
-    646c54e4:	push   %rsi
-    646c54e5:	push   %rbx
-    646c54e6:	sub    $0x30,%rsp
-    646c54ea:	mov    0x2b8f(%rip),%rbx        # 646c8080 <__security_cookie>
-    646c54f1:	movabs $0x2b992ddfa232,%rax
-    646c54fb:	cmp    %rax,%rbx
-    646c54fe:	movq   $0x0,0x20(%rsp)
-    646c5507:	je     646c5520 <__security_init_cookie+0x40>
-    646c5509:	not    %rbx
-    646c550c:	mov    %rbx,0x2b7d(%rip)        # 646c8090 <__security_cookie_complement>
-    646c5513:	add    $0x30,%rsp
-    646c5517:	pop    %rbx
-    646c5518:	pop    %rsi
-    646c5519:	pop    %rdi
-    646c551a:	pop    %rbp
-    646c551b:	pop    %r12
-    646c551d:	ret
-    646c551e:	xchg   %ax,%ax
-    646c5520:	lea    0x20(%rsp),%rcx
-    646c5525:	call   *0x8cd1(%rip)        # 646ce1fc <__imp_GetSystemTimeAsFileTime>
-    646c552b:	mov    0x20(%rsp),%rsi
-    646c5530:	call   *0x8cae(%rip)        # 646ce1e4 <__imp_GetCurrentProcessId>
-    646c5536:	mov    %eax,%r12d
-    646c5539:	call   *0x8cad(%rip)        # 646ce1ec <__imp_GetCurrentThreadId>
-    646c553f:	mov    %eax,%ebp
-    646c5541:	call   *0x8cbd(%rip)        # 646ce204 <__imp_GetTickCount>
-    646c5547:	lea    0x28(%rsp),%rcx
-    646c554c:	mov    %eax,%edi
-    646c554e:	call   *0x8cc8(%rip)        # 646ce21c <__imp_QueryPerformanceCounter>
-    646c5554:	xor    0x28(%rsp),%rsi
-    646c5559:	mov    %r12d,%eax
-    646c555c:	movabs $0xffffffffffff,%rdx
-    646c5566:	xor    %rsi,%rax
-    646c5569:	mov    %ebp,%esi
-    646c556b:	xor    %rax,%rsi
-    646c556e:	mov    %edi,%eax
-    646c5570:	xor    %rsi,%rax
-    646c5573:	and    %rdx,%rax
-    646c5576:	cmp    %rbx,%rax
-    646c5579:	je     646c55a0 <__security_init_cookie+0xc0>
-    646c557b:	mov    %rax,%rdx
-    646c557e:	not    %rdx
-    646c5581:	mov    %rax,0x2af8(%rip)        # 646c8080 <__security_cookie>
-    646c5588:	mov    %rdx,0x2b01(%rip)        # 646c8090 <__security_cookie_complement>
-    646c558f:	add    $0x30,%rsp
-    646c5593:	pop    %rbx
-    646c5594:	pop    %rsi
-    646c5595:	pop    %rdi
-    646c5596:	pop    %rbp
-    646c5597:	pop    %r12
-    646c5599:	ret
-    646c559a:	nopw   0x0(%rax,%rax,1)
-    646c55a0:	movabs $0xffffd466d2205dcc,%rdx
-    646c55aa:	movabs $0x2b992ddfa233,%rax
-    646c55b4:	jmp    646c5581 <__security_init_cookie+0xa1>
-    646c55b6:	cs nopw 0x0(%rax,%rax,1)
-
-00000000646c55c0 <__report_gsfailure>:
-    646c55c0:	push   %rbp
-    646c55c1:	push   %rsi
-    646c55c2:	push   %rbx
-    646c55c3:	mov    %rsp,%rbp
-    646c55c6:	sub    $0x70,%rsp
-    646c55ca:	mov    %rcx,%rsi
-    646c55cd:	lea    0x6ccc(%rip),%rcx        # 646cc2a0 <GS_ContextRecord>
-    646c55d4:	call   *0x8c52(%rip)        # 646ce22c <__imp_RtlCaptureContext>
-    646c55da:	mov    0x6db7(%rip),%rbx        # 646cc398 <GS_ContextRecord+0xf8>
-    646c55e1:	lea    -0x28(%rbp),%rdx
-    646c55e5:	xor    %r8d,%r8d
-    646c55e8:	mov    %rbx,%rcx
-    646c55eb:	call   *0x8c43(%rip)        # 646ce234 <__imp_RtlLookupFunctionEntry>
-    646c55f1:	test   %rax,%rax
-    646c55f4:	je     646c569d <__report_gsfailure+0xdd>
-    646c55fa:	lea    -0x20(%rbp),%rdx
-    646c55fe:	mov    %rax,%r9
-    646c5601:	mov    %rbx,%r8
-    646c5604:	movq   $0x0,0x38(%rsp)
-    646c560d:	lea    0x6c8c(%rip),%rcx        # 646cc2a0 <GS_ContextRecord>
-    646c5614:	mov    %rdx,0x30(%rsp)
-    646c5619:	lea    -0x18(%rbp),%rdx
-    646c561d:	mov    %rcx,0x20(%rsp)
-    646c5622:	xor    %ecx,%ecx
-    646c5624:	mov    %rdx,0x28(%rsp)
-    646c5629:	mov    -0x28(%rbp),%rdx
-    646c562d:	call   *0x8c09(%rip)        # 646ce23c <__imp_RtlVirtualUnwind>
-    646c5633:	mov    0x6d5e(%rip),%rax        # 646cc398 <GS_ContextRecord+0xf8>
-    646c563a:	xor    %ecx,%ecx
-    646c563c:	mov    %rsi,0x6cdd(%rip)        # 646cc320 <GS_ContextRecord+0x80>
-    646c5643:	mov    %rax,0x7146(%rip)        # 646cc790 <GS_ExceptionRecord+0x10>
-    646c564a:	movabs $0x1c0000409,%rax
-    646c5654:	mov    %rax,0x7125(%rip)        # 646cc780 <GS_ExceptionRecord>
-    646c565b:	mov    0x2a1e(%rip),%rax        # 646c8080 <__security_cookie>
-    646c5662:	mov    %rax,-0x10(%rbp)
-    646c5666:	mov    0x2a23(%rip),%rax        # 646c8090 <__security_cookie_complement>
-    646c566d:	mov    %rax,-0x8(%rbp)
-    646c5671:	call   *0x8bcd(%rip)        # 646ce244 <__imp_SetUnhandledExceptionFilter>
-    646c5677:	lea    0x3b02(%rip),%rcx        # 646c9180 <GS_ExceptionPointers>
-    646c567e:	call   *0x8be0(%rip)        # 646ce264 <__imp_UnhandledExceptionFilter>
-    646c5684:	call   *0x8b52(%rip)        # 646ce1dc <__imp_GetCurrentProcess>
-    646c568a:	mov    $0xc0000409,%edx
-    646c568f:	mov    %rax,%rcx
-    646c5692:	call   *0x8bbc(%rip)        # 646ce254 <__imp_TerminateProcess>
-    646c5698:	call   646c7928 <abort>
-    646c569d:	mov    0x18(%rbp),%rax
-    646c56a1:	mov    %rax,0x6cf0(%rip)        # 646cc398 <GS_ContextRecord+0xf8>
-    646c56a8:	lea    0x8(%rbp),%rax
-    646c56ac:	mov    %rax,0x6c85(%rip)        # 646cc338 <GS_ContextRecord+0x98>
-    646c56b3:	jmp    646c5633 <__report_gsfailure+0x73>
-    646c56b8:	nop
-    646c56b9:	nop
-    646c56ba:	nop
-    646c56bb:	nop
-    646c56bc:	nop
-    646c56bd:	nop
-    646c56be:	nop
-    646c56bf:	nop
-
-00000000646c56c0 <__dyn_tls_dtor>:
-    646c56c0:	sub    $0x28,%rsp
-    646c56c4:	cmp    $0x3,%edx
-    646c56c7:	je     646c56e0 <__dyn_tls_dtor+0x20>
-    646c56c9:	test   %edx,%edx
-    646c56cb:	je     646c56e0 <__dyn_tls_dtor+0x20>
-    646c56cd:	mov    $0x1,%eax
-    646c56d2:	add    $0x28,%rsp
-    646c56d6:	ret
-    646c56d7:	nopw   0x0(%rax,%rax,1)
-    646c56e0:	call   646c6240 <__mingw_TLScallback>
-    646c56e5:	mov    $0x1,%eax
-    646c56ea:	add    $0x28,%rsp
-    646c56ee:	ret
-    646c56ef:	nop
-
-00000000646c56f0 <__dyn_tls_init>:
-    646c56f0:	push   %rsi
-    646c56f1:	push   %rbx
-    646c56f2:	sub    $0x28,%rsp
-    646c56f6:	mov    0x3ee3(%rip),%rax        # 646c95e0 <.refptr._CRT_MT>
-    646c56fd:	cmpl   $0x2,(%rax)
-    646c5700:	je     646c5708 <__dyn_tls_init+0x18>
-    646c5702:	movl   $0x2,(%rax)
-    646c5708:	cmp    $0x2,%edx
-    646c570b:	je     646c5720 <__dyn_tls_init+0x30>
-    646c570d:	cmp    $0x1,%edx
-    646c5710:	je     646c5752 <__dyn_tls_init+0x62>
-    646c5712:	mov    $0x1,%eax
-    646c5717:	add    $0x28,%rsp
-    646c571b:	pop    %rbx
-    646c571c:	pop    %rsi
-    646c571d:	ret
-    646c571e:	xchg   %ax,%ax
-    646c5720:	lea    0x9929(%rip),%rbx        # 646cf050 <__xd_z>
-    646c5727:	lea    0x9922(%rip),%rsi        # 646cf050 <__xd_z>
-    646c572e:	cmp    %rbx,%rsi
-    646c5731:	je     646c5712 <__dyn_tls_init+0x22>
-    646c5733:	mov    (%rbx),%rax
-    646c5736:	test   %rax,%rax
-    646c5739:	je     646c573d <__dyn_tls_init+0x4d>
-    646c573b:	call   *%rax
-    646c573d:	add    $0x8,%rbx
-    646c5741:	cmp    %rbx,%rsi
-    646c5744:	jne    646c5733 <__dyn_tls_init+0x43>
-    646c5746:	mov    $0x1,%eax
-    646c574b:	add    $0x28,%rsp
-    646c574f:	pop    %rbx
-    646c5750:	pop    %rsi
-    646c5751:	ret
-    646c5752:	call   646c6240 <__mingw_TLScallback>
-    646c5757:	mov    $0x1,%eax
-    646c575c:	add    $0x28,%rsp
-    646c5760:	pop    %rbx
-    646c5761:	pop    %rsi
-    646c5762:	ret
-    646c5763:	nopl   (%rax)
-    646c5766:	cs nopw 0x0(%rax,%rax,1)
-
-00000000646c5770 <__tlregdtor>:
-    646c5770:	xor    %eax,%eax
-    646c5772:	ret
-    646c5773:	nop
-    646c5774:	nop
-    646c5775:	nop
-    646c5776:	nop
-    646c5777:	nop
-    646c5778:	nop
-    646c5779:	nop
-    646c577a:	nop
-    646c577b:	nop
-    646c577c:	nop
-    646c577d:	nop
-    646c577e:	nop
+    646c504b:	call   646c4d20 <swap>
+    646c5050:	jmp    646c5056 <Partition2d+0x1a6>
+    646c5052:	addl   $0x1,0x18(%rbp)
+    646c5056:	mov    0x18(%rbp),%eax
+    646c5059:	cmp    0x20(%rbp),%eax
+    646c505c:	jge    646c5088 <Partition2d+0x1d8>
+    646c505e:	mov    0x18(%rbp),%eax
+    646c5061:	cltq
+    646c5063:	lea    0x0(,%rax,8),%rdx
+    646c506b:	mov    0x10(%rbp),%rax
+    646c506f:	add    %rdx,%rax
+    646c5072:	mov    (%rax),%rax
+    646c5075:	add    $0x10,%rax
+    646c5079:	movsd  (%rax),%xmm1
+    646c507d:	movsd  -0x10(%rbp),%xmm0
+    646c5082:	comisd %xmm1,%xmm0
+    646c5086:	jae    646c5052 <Partition2d+0x1a2>
+    646c5088:	mov    0x20(%rbp),%edx
+    646c508b:	mov    0x18(%rbp),%eax
+    646c508e:	mov    %edx,%r8d
+    646c5091:	mov    %eax,%edx
+    646c5093:	mov    0x10(%rbp),%rcx
+    646c5097:	call   646c4d20 <swap>
+    646c509c:	mov    0x18(%rbp),%eax
+    646c509f:	cmp    0x20(%rbp),%eax
+    646c50a2:	jl     646c500e <Partition2d+0x15e>
+    646c50a8:	mov    0x18(%rbp),%eax
+    646c50ab:	add    $0x30,%rsp
+    646c50af:	pop    %rbp
+    646c50b0:	ret
+
+00000000646c50b1 <quicksort2d>:
+    646c50b1:	push   %rbp
+    646c50b2:	mov    %rsp,%rbp
+    646c50b5:	sub    $0x30,%rsp
+    646c50b9:	mov    %rcx,0x10(%rbp)
+    646c50bd:	mov    %edx,0x18(%rbp)
+    646c50c0:	mov    %r8d,0x20(%rbp)
+    646c50c4:	mov    0x18(%rbp),%eax
+    646c50c7:	cmp    0x20(%rbp),%eax
+    646c50ca:	jge    646c5111 <quicksort2d+0x60>
+    646c50cc:	mov    0x20(%rbp),%edx
+    646c50cf:	mov    0x18(%rbp),%eax
+    646c50d2:	mov    %edx,%r8d
+    646c50d5:	mov    %eax,%edx
+    646c50d7:	mov    0x10(%rbp),%rcx
+    646c50db:	call   646c4eb0 <Partition2d>
+    646c50e0:	mov    %eax,-0x4(%rbp)
+    646c50e3:	mov    -0x4(%rbp),%eax
+    646c50e6:	lea    -0x1(%rax),%edx
+    646c50e9:	mov    0x18(%rbp),%eax
+    646c50ec:	mov    %edx,%r8d
+    646c50ef:	mov    %eax,%edx
+    646c50f1:	mov    0x10(%rbp),%rcx
+    646c50f5:	call   646c50b1 <quicksort2d>
+    646c50fa:	mov    -0x4(%rbp),%eax
+    646c50fd:	add    $0x1,%eax
+    646c5100:	mov    0x20(%rbp),%edx
+    646c5103:	mov    %edx,%r8d
+    646c5106:	mov    %eax,%edx
+    646c5108:	mov    0x10(%rbp),%rcx
+    646c510c:	call   646c50b1 <quicksort2d>
+    646c5111:	nop
+    646c5112:	add    $0x30,%rsp
+    646c5116:	pop    %rbp
+    646c5117:	ret
+    646c5118:	nop
+    646c5119:	nop
+    646c511a:	nop
+    646c511b:	nop
+    646c511c:	nop
+    646c511d:	nop
+    646c511e:	nop
+    646c511f:	nop
+
+00000000646c5120 <variogram>:
+    646c5120:	push   %rbp
+    646c5121:	push   %rbx
+    646c5122:	sub    $0x88,%rsp
+    646c5129:	lea    0x80(%rsp),%rbp
+    646c5131:	mov    %rcx,0x20(%rbp)
+    646c5135:	mov    %rdx,0x28(%rbp)
+    646c5139:	mov    %r8d,0x30(%rbp)
+    646c513d:	mov    %r9d,0x38(%rbp)
+    646c5141:	mov    0x30(%rbp),%eax
+    646c5144:	cltq
+    646c5146:	mov    %rax,-0x58(%rbp)
+    646c514a:	mov    0x30(%rbp),%eax
+    646c514d:	cltq
+    646c514f:	mov    %rax,-0x50(%rbp)
+    646c5153:	mov    0x30(%rbp),%eax
+    646c5156:	cltq
+    646c5158:	shl    $0x3,%rax
+    646c515c:	mov    %rax,%rcx
+    646c515f:	call   646c7970 <malloc>
+    646c5164:	mov    %rax,-0x60(%rbp)
+    646c5168:	movl   $0x0,-0x14(%rbp)
+    646c516f:	jmp    646c519b <variogram+0x7b>
+    646c5171:	mov    0x30(%rbp),%eax
+    646c5174:	cltq
+    646c5176:	shl    $0x3,%rax
+    646c517a:	mov    -0x60(%rbp),%rcx
+    646c517e:	mov    -0x14(%rbp),%edx
+    646c5181:	movslq %edx,%rdx
+    646c5184:	shl    $0x3,%rdx
+    646c5188:	lea    (%rcx,%rdx,1),%rbx
+    646c518c:	mov    %rax,%rcx
+    646c518f:	call   646c7970 <malloc>
+    646c5194:	mov    %rax,(%rbx)
+    646c5197:	addl   $0x1,-0x14(%rbp)
+    646c519b:	mov    -0x14(%rbp),%eax
+    646c519e:	cmp    0x30(%rbp),%eax
+    646c51a1:	jl     646c5171 <variogram+0x51>
+    646c51a3:	mov    0x30(%rbp),%eax
+    646c51a6:	mov    %eax,%ecx
+    646c51a8:	call   646c4381 <d_arange>
+    646c51ad:	mov    %rax,-0x40(%rbp)
+    646c51b1:	mov    -0x60(%rbp),%rdx
+    646c51b5:	mov    -0x40(%rbp),%rax
+    646c51b9:	mov    0x30(%rbp),%ecx
+    646c51bc:	mov    %ecx,%r8d
+    646c51bf:	mov    %rax,%rcx
+    646c51c2:	call   646c43dd <pdist>
+    646c51c7:	movl   $0x0,-0x18(%rbp)
+    646c51ce:	jmp    646c5337 <variogram+0x217>
+    646c51d3:	pxor   %xmm0,%xmm0
+    646c51d7:	movsd  %xmm0,-0x8(%rbp)
+    646c51dc:	pxor   %xmm0,%xmm0
+    646c51e0:	movsd  %xmm0,-0x10(%rbp)
+    646c51e5:	movl   $0x0,-0x1c(%rbp)
+    646c51ec:	jmp    646c52e8 <variogram+0x1c8>
+    646c51f1:	mov    -0x1c(%rbp),%eax
+    646c51f4:	add    $0x1,%eax
+    646c51f7:	mov    %eax,-0x20(%rbp)
+    646c51fa:	jmp    646c52d8 <variogram+0x1b8>
+    646c51ff:	mov    -0x60(%rbp),%rdx
+    646c5203:	mov    -0x1c(%rbp),%eax
+    646c5206:	cltq
+    646c5208:	shl    $0x3,%rax
+    646c520c:	add    %rdx,%rax
+    646c520f:	mov    (%rax),%rdx
+    646c5212:	mov    -0x20(%rbp),%eax
+    646c5215:	cltq
+    646c5217:	shl    $0x3,%rax
+    646c521b:	add    %rdx,%rax
+    646c521e:	movsd  (%rax),%xmm0
+    646c5222:	mov    -0x18(%rbp),%eax
+    646c5225:	sub    0x40(%rbp),%eax
+    646c5228:	cvtsi2sd %eax,%xmm1
+    646c522c:	comisd %xmm1,%xmm0
+    646c5230:	jb     646c52d4 <variogram+0x1b4>
+    646c5236:	mov    -0x60(%rbp),%rdx
+    646c523a:	mov    -0x1c(%rbp),%eax
+    646c523d:	cltq
+    646c523f:	shl    $0x3,%rax
+    646c5243:	add    %rdx,%rax
+    646c5246:	mov    (%rax),%rdx
+    646c5249:	mov    -0x20(%rbp),%eax
+    646c524c:	cltq
+    646c524e:	shl    $0x3,%rax
+    646c5252:	add    %rdx,%rax
+    646c5255:	movsd  (%rax),%xmm1
+    646c5259:	mov    -0x18(%rbp),%edx
+    646c525c:	mov    0x40(%rbp),%eax
+    646c525f:	add    %edx,%eax
+    646c5261:	cvtsi2sd %eax,%xmm0
+    646c5265:	comisd %xmm1,%xmm0
+    646c5269:	jb     646c52d4 <variogram+0x1b4>
+    646c526b:	mov    -0x1c(%rbp),%eax
+    646c526e:	cltq
+    646c5270:	lea    0x0(,%rax,8),%rdx
+    646c5278:	mov    0x20(%rbp),%rax
+    646c527c:	add    %rdx,%rax
+    646c527f:	movsd  (%rax),%xmm0
+    646c5283:	mov    -0x20(%rbp),%eax
+    646c5286:	cltq
+    646c5288:	lea    0x0(,%rax,8),%rdx
+    646c5290:	mov    0x20(%rbp),%rax
+    646c5294:	add    %rdx,%rax
+    646c5297:	movsd  (%rax),%xmm1
+    646c529b:	subsd  %xmm1,%xmm0
+    646c529f:	movsd  0x3eb9(%rip),%xmm1        # 646c9160 <.rdata>
+    646c52a7:	call   646c6f60 <pow>
+    646c52ac:	movapd %xmm0,%xmm1
+    646c52b0:	movsd  -0x8(%rbp),%xmm0
+    646c52b5:	addsd  %xmm1,%xmm0
+    646c52b9:	movsd  %xmm0,-0x8(%rbp)
+    646c52be:	movsd  -0x10(%rbp),%xmm1
+    646c52c3:	movsd  0x3e9d(%rip),%xmm0        # 646c9168 <.rdata+0x8>
+    646c52cb:	addsd  %xmm1,%xmm0
+    646c52cf:	movsd  %xmm0,-0x10(%rbp)
+    646c52d4:	addl   $0x1,-0x20(%rbp)
+    646c52d8:	mov    -0x20(%rbp),%eax
+    646c52db:	cmp    0x30(%rbp),%eax
+    646c52de:	jl     646c51ff <variogram+0xdf>
+    646c52e4:	addl   $0x1,-0x1c(%rbp)
+    646c52e8:	mov    -0x1c(%rbp),%eax
+    646c52eb:	cmp    0x30(%rbp),%eax
+    646c52ee:	jl     646c51f1 <variogram+0xd1>
+    646c52f4:	movsd  -0x8(%rbp),%xmm0
+    646c52f9:	comisd 0x3e6f(%rip),%xmm0        # 646c9170 <.rdata+0x10>
+    646c5301:	jb     646c5331 <variogram+0x211>
+    646c5303:	movsd  -0x10(%rbp),%xmm0
+    646c5308:	movapd %xmm0,%xmm1
+    646c530c:	addsd  %xmm0,%xmm1
+    646c5310:	mov    -0x18(%rbp),%eax
+    646c5313:	cltq
+    646c5315:	lea    0x0(,%rax,8),%rdx
+    646c531d:	mov    0x28(%rbp),%rax
+    646c5321:	add    %rdx,%rax
+    646c5324:	movsd  -0x8(%rbp),%xmm0
+    646c5329:	divsd  %xmm1,%xmm0
+    646c532d:	movsd  %xmm0,(%rax)
+    646c5331:	mov    0x40(%rbp),%eax
+    646c5334:	add    %eax,-0x18(%rbp)
+    646c5337:	mov    -0x18(%rbp),%eax
+    646c533a:	cmp    0x38(%rbp),%eax
+    646c533d:	jl     646c51d3 <variogram+0xb3>
+    646c5343:	mov    -0x40(%rbp),%rax
+    646c5347:	mov    %rax,%rcx
+    646c534a:	call   646c7988 <free>
+    646c534f:	movl   $0x0,-0x24(%rbp)
+    646c5356:	jmp    646c5377 <variogram+0x257>
+    646c5358:	mov    -0x60(%rbp),%rdx
+    646c535c:	mov    -0x24(%rbp),%eax
+    646c535f:	cltq
+    646c5361:	shl    $0x3,%rax
+    646c5365:	add    %rdx,%rax
+    646c5368:	mov    (%rax),%rax
+    646c536b:	mov    %rax,%rcx
+    646c536e:	call   646c7988 <free>
+    646c5373:	addl   $0x1,-0x24(%rbp)
+    646c5377:	mov    -0x24(%rbp),%eax
+    646c537a:	cltq
+    646c537c:	mov    -0x58(%rbp),%rdx
+    646c5380:	cmp    %rdx,%rax
+    646c5383:	jb     646c5358 <variogram+0x238>
+    646c5385:	mov    -0x60(%rbp),%rax
+    646c5389:	mov    %rax,%rcx
+    646c538c:	call   646c7988 <free>
+    646c5391:	nop
+    646c5392:	add    $0x88,%rsp
+    646c5399:	pop    %rbx
+    646c539a:	pop    %rbp
+    646c539b:	ret
+
+00000000646c539c <variance>:
+    646c539c:	push   %rbp
+    646c539d:	mov    %rsp,%rbp
+    646c53a0:	sub    $0x40,%rsp
+    646c53a4:	mov    %rcx,0x10(%rbp)
+    646c53a8:	mov    %edx,0x18(%rbp)
+    646c53ab:	pxor   %xmm0,%xmm0
+    646c53af:	movsd  %xmm0,-0x8(%rbp)
+    646c53b4:	pxor   %xmm0,%xmm0
+    646c53b8:	movsd  %xmm0,-0x10(%rbp)
+    646c53bd:	movl   $0x0,-0x14(%rbp)
+    646c53c4:	jmp    646c53f0 <variance+0x54>
+    646c53c6:	mov    -0x14(%rbp),%eax
+    646c53c9:	cltq
+    646c53cb:	lea    0x0(,%rax,8),%rdx
+    646c53d3:	mov    0x10(%rbp),%rax
+    646c53d7:	add    %rdx,%rax
+    646c53da:	movsd  (%rax),%xmm0
+    646c53de:	movsd  -0x8(%rbp),%xmm1
+    646c53e3:	addsd  %xmm1,%xmm0
+    646c53e7:	movsd  %xmm0,-0x8(%rbp)
+    646c53ec:	addl   $0x1,-0x14(%rbp)
+    646c53f0:	mov    -0x14(%rbp),%eax
+    646c53f3:	cmp    0x18(%rbp),%eax
+    646c53f6:	jl     646c53c6 <variance+0x2a>
+    646c53f8:	cvtsi2sdl 0x18(%rbp),%xmm1
+    646c53fd:	movsd  -0x8(%rbp),%xmm0
+    646c5402:	divsd  %xmm1,%xmm0
+    646c5406:	movsd  %xmm0,-0x8(%rbp)
+    646c540b:	movl   $0x0,-0x18(%rbp)
+    646c5412:	jmp    646c5454 <variance+0xb8>
+    646c5414:	mov    -0x18(%rbp),%eax
+    646c5417:	cltq
+    646c5419:	lea    0x0(,%rax,8),%rdx
+    646c5421:	mov    0x10(%rbp),%rax
+    646c5425:	add    %rdx,%rax
+    646c5428:	movsd  (%rax),%xmm0
+    646c542c:	subsd  -0x8(%rbp),%xmm0
+    646c5431:	movsd  0x3d27(%rip),%xmm1        # 646c9160 <.rdata>
+    646c5439:	call   646c6f60 <pow>
+    646c543e:	movapd %xmm0,%xmm1
+    646c5442:	movsd  -0x10(%rbp),%xmm0
+    646c5447:	addsd  %xmm1,%xmm0
+    646c544b:	movsd  %xmm0,-0x10(%rbp)
+    646c5450:	addl   $0x1,-0x18(%rbp)
+    646c5454:	mov    -0x18(%rbp),%eax
+    646c5457:	cmp    0x18(%rbp),%eax
+    646c545a:	jl     646c5414 <variance+0x78>
+    646c545c:	cvtsi2sdl 0x18(%rbp),%xmm1
+    646c5461:	movsd  -0x10(%rbp),%xmm0
+    646c5466:	divsd  %xmm1,%xmm0
+    646c546a:	movsd  %xmm0,-0x10(%rbp)
+    646c546f:	movsd  -0x10(%rbp),%xmm0
+    646c5474:	movq   %xmm0,%rax
+    646c5479:	movq   %rax,%xmm0
+    646c547e:	add    $0x40,%rsp
+    646c5482:	pop    %rbp
+    646c5483:	ret
+    646c5484:	nop
+    646c5485:	nop
+    646c5486:	nop
+    646c5487:	nop
+    646c5488:	nop
+    646c5489:	nop
+    646c548a:	nop
+    646c548b:	nop
+    646c548c:	nop
+    646c548d:	nop
+    646c548e:	nop
+    646c548f:	nop
+
+00000000646c5490 <Sleep>:
+    646c5490:	jmp    *0x8db6(%rip)        # 646ce24c <__imp_Sleep>
+    646c5496:	nop
+    646c5497:	nop
+    646c5498:	nopl   0x0(%rax,%rax,1)
+
+00000000646c54a0 <__do_global_dtors>:
+    646c54a0:	sub    $0x28,%rsp
+    646c54a4:	mov    0x2b55(%rip),%rax        # 646c8000 <__data_start__>
+    646c54ab:	mov    (%rax),%rax
+    646c54ae:	test   %rax,%rax
+    646c54b1:	je     646c54d0 <__do_global_dtors+0x30>
+    646c54b3:	call   *%rax
+    646c54b5:	mov    0x2b44(%rip),%rax        # 646c8000 <__data_start__>
+    646c54bc:	lea    0x8(%rax),%rdx
+    646c54c0:	mov    0x8(%rax),%rax
+    646c54c4:	mov    %rdx,0x2b35(%rip)        # 646c8000 <__data_start__>
+    646c54cb:	test   %rax,%rax
+    646c54ce:	jne    646c54b3 <__do_global_dtors+0x13>
+    646c54d0:	add    $0x28,%rsp
+    646c54d4:	ret
+    646c54d5:	nop
+    646c54d6:	cs nopw 0x0(%rax,%rax,1)
+
+00000000646c54e0 <__do_global_ctors>:
+    646c54e0:	push   %rsi
+    646c54e1:	push   %rbx
+    646c54e2:	sub    $0x28,%rsp
+    646c54e6:	mov    0x4103(%rip),%rcx        # 646c95f0 <.refptr.__CTOR_LIST__>
+    646c54ed:	mov    (%rcx),%rdx
+    646c54f0:	cmp    $0xffffffff,%edx
+    646c54f3:	mov    %edx,%eax
+    646c54f5:	je     646c5530 <__do_global_ctors+0x50>
+    646c54f7:	test   %eax,%eax
+    646c54f9:	je     646c551b <__do_global_ctors+0x3b>
+    646c54fb:	mov    %eax,%edx
+    646c54fd:	sub    $0x1,%eax
+    646c5500:	lea    (%rcx,%rdx,8),%rbx
+    646c5504:	sub    %rax,%rdx
+    646c5507:	lea    -0x8(%rcx,%rdx,8),%rsi
+    646c550c:	nopl   0x0(%rax)
+    646c5510:	call   *(%rbx)
+    646c5512:	sub    $0x8,%rbx
+    646c5516:	cmp    %rsi,%rbx
+    646c5519:	jne    646c5510 <__do_global_ctors+0x30>
+    646c551b:	lea    -0x82(%rip),%rcx        # 646c54a0 <__do_global_dtors>
+    646c5522:	add    $0x28,%rsp
+    646c5526:	pop    %rbx
+    646c5527:	pop    %rsi
+    646c5528:	jmp    646c1380 <atexit>
+    646c552d:	nopl   (%rax)
+    646c5530:	xor    %eax,%eax
+    646c5532:	jmp    646c5536 <__do_global_ctors+0x56>
+    646c5534:	mov    %edx,%eax
+    646c5536:	lea    0x1(%rax),%r8d
+    646c553a:	cmpq   $0x0,(%rcx,%r8,8)
+    646c553f:	mov    %r8,%rdx
+    646c5542:	jne    646c5534 <__do_global_ctors+0x54>
+    646c5544:	jmp    646c54f7 <__do_global_ctors+0x17>
+    646c5546:	cs nopw 0x0(%rax,%rax,1)
+
+00000000646c5550 <__main>:
+    646c5550:	mov    0x6d2a(%rip),%eax        # 646cc280 <initialized>
+    646c5556:	test   %eax,%eax
+    646c5558:	je     646c5560 <__main+0x10>
+    646c555a:	ret
+    646c555b:	nopl   0x0(%rax,%rax,1)
+    646c5560:	movl   $0x1,0x6d16(%rip)        # 646cc280 <initialized>
+    646c556a:	jmp    646c54e0 <__do_global_ctors>
+    646c556f:	nop
+
+00000000646c5570 <__security_init_cookie>:
+    646c5570:	push   %r12
+    646c5572:	push   %rbp
+    646c5573:	push   %rdi
+    646c5574:	push   %rsi
+    646c5575:	push   %rbx
+    646c5576:	sub    $0x30,%rsp
+    646c557a:	mov    0x2aff(%rip),%rbx        # 646c8080 <__security_cookie>
+    646c5581:	movabs $0x2b992ddfa232,%rax
+    646c558b:	cmp    %rax,%rbx
+    646c558e:	movq   $0x0,0x20(%rsp)
+    646c5597:	je     646c55b0 <__security_init_cookie+0x40>
+    646c5599:	not    %rbx
+    646c559c:	mov    %rbx,0x2aed(%rip)        # 646c8090 <__security_cookie_complement>
+    646c55a3:	add    $0x30,%rsp
+    646c55a7:	pop    %rbx
+    646c55a8:	pop    %rsi
+    646c55a9:	pop    %rdi
+    646c55aa:	pop    %rbp
+    646c55ab:	pop    %r12
+    646c55ad:	ret
+    646c55ae:	xchg   %ax,%ax
+    646c55b0:	lea    0x20(%rsp),%rcx
+    646c55b5:	call   *0x8c41(%rip)        # 646ce1fc <__imp_GetSystemTimeAsFileTime>
+    646c55bb:	mov    0x20(%rsp),%rsi
+    646c55c0:	call   *0x8c1e(%rip)        # 646ce1e4 <__imp_GetCurrentProcessId>
+    646c55c6:	mov    %eax,%r12d
+    646c55c9:	call   *0x8c1d(%rip)        # 646ce1ec <__imp_GetCurrentThreadId>
+    646c55cf:	mov    %eax,%ebp
+    646c55d1:	call   *0x8c2d(%rip)        # 646ce204 <__imp_GetTickCount>
+    646c55d7:	lea    0x28(%rsp),%rcx
+    646c55dc:	mov    %eax,%edi
+    646c55de:	call   *0x8c38(%rip)        # 646ce21c <__imp_QueryPerformanceCounter>
+    646c55e4:	xor    0x28(%rsp),%rsi
+    646c55e9:	mov    %r12d,%eax
+    646c55ec:	movabs $0xffffffffffff,%rdx
+    646c55f6:	xor    %rsi,%rax
+    646c55f9:	mov    %ebp,%esi
+    646c55fb:	xor    %rax,%rsi
+    646c55fe:	mov    %edi,%eax
+    646c5600:	xor    %rsi,%rax
+    646c5603:	and    %rdx,%rax
+    646c5606:	cmp    %rbx,%rax
+    646c5609:	je     646c5630 <__security_init_cookie+0xc0>
+    646c560b:	mov    %rax,%rdx
+    646c560e:	not    %rdx
+    646c5611:	mov    %rax,0x2a68(%rip)        # 646c8080 <__security_cookie>
+    646c5618:	mov    %rdx,0x2a71(%rip)        # 646c8090 <__security_cookie_complement>
+    646c561f:	add    $0x30,%rsp
+    646c5623:	pop    %rbx
+    646c5624:	pop    %rsi
+    646c5625:	pop    %rdi
+    646c5626:	pop    %rbp
+    646c5627:	pop    %r12
+    646c5629:	ret
+    646c562a:	nopw   0x0(%rax,%rax,1)
+    646c5630:	movabs $0xffffd466d2205dcc,%rdx
+    646c563a:	movabs $0x2b992ddfa233,%rax
+    646c5644:	jmp    646c5611 <__security_init_cookie+0xa1>
+    646c5646:	cs nopw 0x0(%rax,%rax,1)
+
+00000000646c5650 <__report_gsfailure>:
+    646c5650:	push   %rbp
+    646c5651:	push   %rsi
+    646c5652:	push   %rbx
+    646c5653:	mov    %rsp,%rbp
+    646c5656:	sub    $0x70,%rsp
+    646c565a:	mov    %rcx,%rsi
+    646c565d:	lea    0x6c3c(%rip),%rcx        # 646cc2a0 <GS_ContextRecord>
+    646c5664:	call   *0x8bc2(%rip)        # 646ce22c <__imp_RtlCaptureContext>
+    646c566a:	mov    0x6d27(%rip),%rbx        # 646cc398 <GS_ContextRecord+0xf8>
+    646c5671:	lea    -0x28(%rbp),%rdx
+    646c5675:	xor    %r8d,%r8d
+    646c5678:	mov    %rbx,%rcx
+    646c567b:	call   *0x8bb3(%rip)        # 646ce234 <__imp_RtlLookupFunctionEntry>
+    646c5681:	test   %rax,%rax
+    646c5684:	je     646c572d <__report_gsfailure+0xdd>
+    646c568a:	lea    -0x20(%rbp),%rdx
+    646c568e:	mov    %rax,%r9
+    646c5691:	mov    %rbx,%r8
+    646c5694:	movq   $0x0,0x38(%rsp)
+    646c569d:	lea    0x6bfc(%rip),%rcx        # 646cc2a0 <GS_ContextRecord>
+    646c56a4:	mov    %rdx,0x30(%rsp)
+    646c56a9:	lea    -0x18(%rbp),%rdx
+    646c56ad:	mov    %rcx,0x20(%rsp)
+    646c56b2:	xor    %ecx,%ecx
+    646c56b4:	mov    %rdx,0x28(%rsp)
+    646c56b9:	mov    -0x28(%rbp),%rdx
+    646c56bd:	call   *0x8b79(%rip)        # 646ce23c <__imp_RtlVirtualUnwind>
+    646c56c3:	mov    0x6cce(%rip),%rax        # 646cc398 <GS_ContextRecord+0xf8>
+    646c56ca:	xor    %ecx,%ecx
+    646c56cc:	mov    %rsi,0x6c4d(%rip)        # 646cc320 <GS_ContextRecord+0x80>
+    646c56d3:	mov    %rax,0x70b6(%rip)        # 646cc790 <GS_ExceptionRecord+0x10>
+    646c56da:	movabs $0x1c0000409,%rax
+    646c56e4:	mov    %rax,0x7095(%rip)        # 646cc780 <GS_ExceptionRecord>
+    646c56eb:	mov    0x298e(%rip),%rax        # 646c8080 <__security_cookie>
+    646c56f2:	mov    %rax,-0x10(%rbp)
+    646c56f6:	mov    0x2993(%rip),%rax        # 646c8090 <__security_cookie_complement>
+    646c56fd:	mov    %rax,-0x8(%rbp)
+    646c5701:	call   *0x8b3d(%rip)        # 646ce244 <__imp_SetUnhandledExceptionFilter>
+    646c5707:	lea    0x3a72(%rip),%rcx        # 646c9180 <GS_ExceptionPointers>
+    646c570e:	call   *0x8b50(%rip)        # 646ce264 <__imp_UnhandledExceptionFilter>
+    646c5714:	call   *0x8ac2(%rip)        # 646ce1dc <__imp_GetCurrentProcess>
+    646c571a:	mov    $0xc0000409,%edx
+    646c571f:	mov    %rax,%rcx
+    646c5722:	call   *0x8b2c(%rip)        # 646ce254 <__imp_TerminateProcess>
+    646c5728:	call   646c79b8 <abort>
+    646c572d:	mov    0x18(%rbp),%rax
+    646c5731:	mov    %rax,0x6c60(%rip)        # 646cc398 <GS_ContextRecord+0xf8>
+    646c5738:	lea    0x8(%rbp),%rax
+    646c573c:	mov    %rax,0x6bf5(%rip)        # 646cc338 <GS_ContextRecord+0x98>
+    646c5743:	jmp    646c56c3 <__report_gsfailure+0x73>
+    646c5748:	nop
+    646c5749:	nop
+    646c574a:	nop
+    646c574b:	nop
+    646c574c:	nop
+    646c574d:	nop
+    646c574e:	nop
+    646c574f:	nop
+
+00000000646c5750 <__dyn_tls_dtor>:
+    646c5750:	sub    $0x28,%rsp
+    646c5754:	cmp    $0x3,%edx
+    646c5757:	je     646c5770 <__dyn_tls_dtor+0x20>
+    646c5759:	test   %edx,%edx
+    646c575b:	je     646c5770 <__dyn_tls_dtor+0x20>
+    646c575d:	mov    $0x1,%eax
+    646c5762:	add    $0x28,%rsp
+    646c5766:	ret
+    646c5767:	nopw   0x0(%rax,%rax,1)
+    646c5770:	call   646c62d0 <__mingw_TLScallback>
+    646c5775:	mov    $0x1,%eax
+    646c577a:	add    $0x28,%rsp
+    646c577e:	ret
     646c577f:	nop
 
-00000000646c5780 <_decode_pointer>:
-    646c5780:	mov    %rcx,%rax
-    646c5783:	ret
-    646c5784:	xchg   %ax,%ax
-    646c5786:	cs nopw 0x0(%rax,%rax,1)
-
-00000000646c5790 <_encode_pointer>:
-    646c5790:	mov    %rcx,%rax
-    646c5793:	ret
-    646c5794:	nop
-    646c5795:	nop
-    646c5796:	nop
-    646c5797:	nop
-    646c5798:	nop
-    646c5799:	nop
-    646c579a:	nop
-    646c579b:	nop
-    646c579c:	nop
-    646c579d:	nop
-    646c579e:	nop
-    646c579f:	nop
-
-00000000646c57a0 <__write_memory.part.0>:
-    646c57a0:	push   %r12
-    646c57a2:	push   %rbp
-    646c57a3:	push   %rdi
-    646c57a4:	push   %rsi
-    646c57a5:	push   %rbx
-    646c57a6:	sub    $0x50,%rsp
-    646c57aa:	movslq 0x7093(%rip),%rsi        # 646cc844 <maxSections>
-    646c57b1:	test   %esi,%esi
-    646c57b3:	mov    %rcx,%rbx
-    646c57b6:	mov    %rdx,%rbp
-    646c57b9:	mov    %r8,%rdi
-    646c57bc:	jle    646c5928 <__write_memory.part.0+0x188>
-    646c57c2:	mov    0x707f(%rip),%rax        # 646cc848 <the_secs>
-    646c57c9:	xor    %ecx,%ecx
-    646c57cb:	add    $0x18,%rax
-    646c57cf:	nop
-    646c57d0:	mov    (%rax),%rdx
-    646c57d3:	cmp    %rdx,%rbx
-    646c57d6:	jb     646c57ec <__write_memory.part.0+0x4c>
-    646c57d8:	mov    0x8(%rax),%r8
-    646c57dc:	mov    0x8(%r8),%r8d
-    646c57e0:	add    %r8,%rdx
-    646c57e3:	cmp    %rdx,%rbx
-    646c57e6:	jb     646c5875 <__write_memory.part.0+0xd5>
-    646c57ec:	add    $0x1,%ecx
-    646c57ef:	add    $0x28,%rax
-    646c57f3:	cmp    %esi,%ecx
-    646c57f5:	jne    646c57d0 <__write_memory.part.0+0x30>
-    646c57f7:	mov    %rbx,%rcx
-    646c57fa:	call   646c6440 <__mingw_GetSectionForAddress>
-    646c57ff:	test   %rax,%rax
-    646c5802:	mov    %rax,%r12
-    646c5805:	je     646c595d <__write_memory.part.0+0x1bd>
-    646c580b:	mov    0x7036(%rip),%rax        # 646cc848 <the_secs>
-    646c5812:	lea    (%rsi,%rsi,4),%rsi
-    646c5816:	shl    $0x3,%rsi
-    646c581a:	add    %rsi,%rax
-    646c581d:	mov    %r12,0x20(%rax)
-    646c5821:	movl   $0x0,(%rax)
-    646c5827:	call   646c6570 <_GetPEImageBase>
-    646c582c:	mov    0xc(%r12),%ecx
-    646c5831:	lea    0x20(%rsp),%rdx
-    646c5836:	mov    $0x30,%r8d
-    646c583c:	add    %rax,%rcx
-    646c583f:	mov    0x7002(%rip),%rax        # 646cc848 <the_secs>
-    646c5846:	mov    %rcx,0x18(%rax,%rsi,1)
-    646c584b:	call   *0x8a23(%rip)        # 646ce274 <__imp_VirtualQuery>
-    646c5851:	test   %rax,%rax
-    646c5854:	je     646c5940 <__write_memory.part.0+0x1a0>
-    646c585a:	mov    0x44(%rsp),%eax
-    646c585e:	lea    -0x4(%rax),%edx
-    646c5861:	and    $0xfffffffb,%edx
-    646c5864:	je     646c586e <__write_memory.part.0+0xce>
-    646c5866:	sub    $0x40,%eax
-    646c5869:	and    $0xffffffbf,%eax
-    646c586c:	jne    646c58d0 <__write_memory.part.0+0x130>
-    646c586e:	addl   $0x1,0x6fcf(%rip)        # 646cc844 <maxSections>
-    646c5875:	cmp    $0x8,%edi
-    646c5878:	jae    646c58a3 <__write_memory.part.0+0x103>
-    646c587a:	test   $0x4,%dil
-    646c587e:	jne    646c5914 <__write_memory.part.0+0x174>
-    646c5884:	test   %edi,%edi
-    646c5886:	je     646c5898 <__write_memory.part.0+0xf8>
-    646c5888:	movzbl 0x0(%rbp),%eax
-    646c588c:	test   $0x2,%dil
-    646c5890:	mov    %al,(%rbx)
-    646c5892:	jne    646c592f <__write_memory.part.0+0x18f>
-    646c5898:	add    $0x50,%rsp
-    646c589c:	pop    %rbx
-    646c589d:	pop    %rsi
-    646c589e:	pop    %rdi
-    646c589f:	pop    %rbp
-    646c58a0:	pop    %r12
-    646c58a2:	ret
-    646c58a3:	mov    %edi,%eax
-    646c58a5:	sub    $0x1,%edi
-    646c58a8:	mov    -0x8(%rbp,%rax,1),%rdx
-    646c58ad:	cmp    $0x8,%edi
-    646c58b0:	mov    %rdx,-0x8(%rbx,%rax,1)
-    646c58b5:	jb     646c5898 <__write_memory.part.0+0xf8>
-    646c58b7:	and    $0xfffffff8,%edi
-    646c58ba:	xor    %eax,%eax
-    646c58bc:	mov    %eax,%edx
-    646c58be:	add    $0x8,%eax
-    646c58c1:	mov    0x0(%rbp,%rdx,1),%rcx
-    646c58c6:	cmp    %edi,%eax
-    646c58c8:	mov    %rcx,(%rbx,%rdx,1)
-    646c58cc:	jb     646c58bc <__write_memory.part.0+0x11c>
-    646c58ce:	jmp    646c5898 <__write_memory.part.0+0xf8>
-    646c58d0:	add    0x6f71(%rip),%rsi        # 646cc848 <the_secs>
-    646c58d7:	mov    $0x40,%r8d
-    646c58dd:	mov    0x20(%rsp),%rcx
-    646c58e2:	mov    0x38(%rsp),%rdx
-    646c58e7:	mov    %rsi,%r9
-    646c58ea:	mov    %rcx,0x8(%rsi)
-    646c58ee:	mov    %rdx,0x10(%rsi)
-    646c58f2:	call   *0x8974(%rip)        # 646ce26c <__imp_VirtualProtect>
-    646c58f8:	test   %eax,%eax
-    646c58fa:	jne    646c586e <__write_memory.part.0+0xce>
-    646c5900:	call   *0x88ee(%rip)        # 646ce1f4 <__imp_GetLastError>
-    646c5906:	lea    0x396b(%rip),%rcx        # 646c9278 <.rdata+0x78>
-    646c590d:	mov    %eax,%edx
-    646c590f:	call   646c7d30 <__report_error>
-    646c5914:	mov    0x0(%rbp),%eax
-    646c5917:	mov    %edi,%edi
-    646c5919:	mov    %eax,(%rbx)
-    646c591b:	mov    -0x4(%rbp,%rdi,1),%eax
-    646c591f:	mov    %eax,-0x4(%rbx,%rdi,1)
-    646c5923:	jmp    646c5898 <__write_memory.part.0+0xf8>
-    646c5928:	xor    %esi,%esi
-    646c592a:	jmp    646c57f7 <__write_memory.part.0+0x57>
-    646c592f:	mov    %edi,%edi
-    646c5931:	movzwl -0x2(%rbp,%rdi,1),%eax
-    646c5936:	mov    %ax,-0x2(%rbx,%rdi,1)
-    646c593b:	jmp    646c5898 <__write_memory.part.0+0xf8>
-    646c5940:	mov    0x6f01(%rip),%rax        # 646cc848 <the_secs>
-    646c5947:	lea    0x38f2(%rip),%rcx        # 646c9240 <.rdata+0x40>
-    646c594e:	mov    0x8(%r12),%edx
-    646c5953:	mov    0x18(%rax,%rsi,1),%r8
-    646c5958:	call   646c7d30 <__report_error>
-    646c595d:	lea    0x38bc(%rip),%rcx        # 646c9220 <.rdata+0x20>
-    646c5964:	mov    %rbx,%rdx
-    646c5967:	call   646c7d30 <__report_error>
-    646c596c:	nop
-    646c596d:	nopl   (%rax)
-
-00000000646c5970 <_pei386_runtime_relocator>:
-    646c5970:	push   %rbp
-    646c5971:	push   %r15
-    646c5973:	push   %r14
-    646c5975:	push   %r13
-    646c5977:	push   %r12
-    646c5979:	push   %rdi
-    646c597a:	push   %rsi
-    646c597b:	push   %rbx
-    646c597c:	sub    $0x38,%rsp
-    646c5980:	lea    0x80(%rsp),%rbp
-    646c5988:	mov    0x6eb2(%rip),%ebx        # 646cc840 <was_init.95174>
-    646c598e:	test   %ebx,%ebx
-    646c5990:	je     646c59a3 <_pei386_runtime_relocator+0x33>
-    646c5992:	lea    -0x48(%rbp),%rsp
-    646c5996:	pop    %rbx
-    646c5997:	pop    %rsi
-    646c5998:	pop    %rdi
-    646c5999:	pop    %r12
-    646c599b:	pop    %r13
-    646c599d:	pop    %r14
-    646c599f:	pop    %r15
-    646c59a1:	pop    %rbp
-    646c59a2:	ret
-    646c59a3:	movl   $0x1,0x6e93(%rip)        # 646cc840 <was_init.95174>
-    646c59ad:	call   646c64c0 <__mingw_GetSectionCount>
-    646c59b2:	cltq
-    646c59b4:	lea    (%rax,%rax,4),%rax
-    646c59b8:	lea    0x1e(,%rax,8),%rax
-    646c59c0:	and    $0xfffffffffffffff0,%rax
-    646c59c4:	call   646c6710 <___chkstk_ms>
-    646c59c9:	mov    0x3c30(%rip),%r12        # 646c9600 <.refptr.__RUNTIME_PSEUDO_RELOC_LIST_END__>
-    646c59d0:	movl   $0x0,0x6e6a(%rip)        # 646cc844 <maxSections>
-    646c59da:	mov    0x3c2f(%rip),%rsi        # 646c9610 <.refptr.__RUNTIME_PSEUDO_RELOC_LIST__>
-    646c59e1:	sub    %rax,%rsp
-    646c59e4:	lea    0x20(%rsp),%rax
-    646c59e9:	mov    %rax,0x6e58(%rip)        # 646cc848 <the_secs>
-    646c59f0:	mov    %r12,%rax
-    646c59f3:	sub    %rsi,%rax
-    646c59f6:	cmp    $0x7,%rax
-    646c59fa:	jle    646c5992 <_pei386_runtime_relocator+0x22>
-    646c59fc:	cmp    $0xb,%rax
-    646c5a00:	mov    (%rsi),%edx
-    646c5a02:	jle    646c5ad0 <_pei386_runtime_relocator+0x160>
-    646c5a08:	test   %edx,%edx
-    646c5a0a:	je     646c5ab4 <_pei386_runtime_relocator+0x144>
-    646c5a10:	cmp    %r12,%rsi
-    646c5a13:	jae    646c5992 <_pei386_runtime_relocator+0x22>
-    646c5a19:	lea    0x8(%rsi),%r14
-    646c5a1d:	add    $0x7,%r12
-    646c5a21:	mov    0x3c08(%rip),%r13        # 646c9630 <.refptr.__image_base__>
-    646c5a28:	lea    -0x58(%rbp),%rdi
-    646c5a2c:	sub    %r14,%r12
-    646c5a2f:	shr    $0x3,%r12
-    646c5a33:	lea    0x8(%rsi,%r12,8),%r12
-    646c5a38:	jmp    646c5a44 <_pei386_runtime_relocator+0xd4>
-    646c5a3a:	nopw   0x0(%rax,%rax,1)
-    646c5a40:	add    $0x8,%r14
-    646c5a44:	mov    0x4(%rsi),%ecx
-    646c5a47:	mov    $0x4,%r8d
-    646c5a4d:	mov    %rdi,%rdx
-    646c5a50:	mov    (%rsi),%eax
-    646c5a52:	mov    %r14,%rsi
-    646c5a55:	add    %r13,%rcx
-    646c5a58:	add    (%rcx),%eax
-    646c5a5a:	mov    %eax,-0x58(%rbp)
-    646c5a5d:	call   646c57a0 <__write_memory.part.0>
-    646c5a62:	cmp    %r12,%r14
-    646c5a65:	jne    646c5a40 <_pei386_runtime_relocator+0xd0>
-    646c5a67:	mov    0x6dd7(%rip),%eax        # 646cc844 <maxSections>
-    646c5a6d:	xor    %esi,%esi
-    646c5a6f:	mov    0x87f6(%rip),%r12        # 646ce26c <__imp_VirtualProtect>
-    646c5a76:	test   %eax,%eax
-    646c5a78:	jle    646c5992 <_pei386_runtime_relocator+0x22>
-    646c5a7e:	xchg   %ax,%ax
-    646c5a80:	mov    0x6dc1(%rip),%rax        # 646cc848 <the_secs>
-    646c5a87:	add    %rsi,%rax
-    646c5a8a:	mov    (%rax),%r8d
-    646c5a8d:	test   %r8d,%r8d
-    646c5a90:	je     646c5aa0 <_pei386_runtime_relocator+0x130>
-    646c5a92:	mov    0x10(%rax),%rdx
-    646c5a96:	mov    %rdi,%r9
-    646c5a99:	mov    0x8(%rax),%rcx
-    646c5a9d:	call   *%r12
-    646c5aa0:	add    $0x1,%ebx
-    646c5aa3:	add    $0x28,%rsi
-    646c5aa7:	cmp    0x6d97(%rip),%ebx        # 646cc844 <maxSections>
-    646c5aad:	jl     646c5a80 <_pei386_runtime_relocator+0x110>
-    646c5aaf:	jmp    646c5992 <_pei386_runtime_relocator+0x22>
-    646c5ab4:	mov    0x4(%rsi),%ecx
-    646c5ab7:	test   %ecx,%ecx
-    646c5ab9:	jne    646c5a10 <_pei386_runtime_relocator+0xa0>
-    646c5abf:	mov    0x8(%rsi),%edx
-    646c5ac2:	test   %edx,%edx
-    646c5ac4:	jne    646c5ae3 <_pei386_runtime_relocator+0x173>
-    646c5ac6:	mov    0xc(%rsi),%edx
-    646c5ac9:	add    $0xc,%rsi
-    646c5acd:	nopl   (%rax)
-    646c5ad0:	test   %edx,%edx
-    646c5ad2:	jne    646c5a10 <_pei386_runtime_relocator+0xa0>
-    646c5ad8:	mov    0x4(%rsi),%eax
-    646c5adb:	test   %eax,%eax
-    646c5add:	jne    646c5a10 <_pei386_runtime_relocator+0xa0>
-    646c5ae3:	mov    0x8(%rsi),%edx
-    646c5ae6:	cmp    $0x1,%edx
-    646c5ae9:	jne    646c5c1e <_pei386_runtime_relocator+0x2ae>
-    646c5aef:	mov    0x3b3a(%rip),%r13        # 646c9630 <.refptr.__image_base__>
-    646c5af6:	add    $0xc,%rsi
-    646c5afa:	movabs $0xffffffff00000000,%r15
-    646c5b04:	lea    -0x58(%rbp),%r14
-    646c5b08:	cmp    %r12,%rsi
-    646c5b0b:	jb     646c5b55 <_pei386_runtime_relocator+0x1e5>
-    646c5b0d:	jmp    646c5992 <_pei386_runtime_relocator+0x22>
-    646c5b12:	jbe    646c5bd0 <_pei386_runtime_relocator+0x260>
-    646c5b18:	cmp    $0x20,%edx
-    646c5b1b:	je     646c5ba0 <_pei386_runtime_relocator+0x230>
-    646c5b21:	cmp    $0x40,%edx
-    646c5b24:	jne    646c5c0a <_pei386_runtime_relocator+0x29a>
-    646c5b2a:	mov    (%rcx),%rdx
-    646c5b2d:	mov    $0x8,%r8d
-    646c5b33:	mov    %r14,%rdi
-    646c5b36:	sub    %rax,%rdx
-    646c5b39:	add    %r9,%rdx
-    646c5b3c:	mov    %rdx,-0x58(%rbp)
-    646c5b40:	mov    %r14,%rdx
-    646c5b43:	call   646c57a0 <__write_memory.part.0>
-    646c5b48:	add    $0xc,%rsi
-    646c5b4c:	cmp    %r12,%rsi
-    646c5b4f:	jae    646c5a67 <_pei386_runtime_relocator+0xf7>
-    646c5b55:	mov    0x4(%rsi),%ecx
-    646c5b58:	mov    (%rsi),%eax
-    646c5b5a:	movzbl 0x8(%rsi),%edx
-    646c5b5e:	add    %r13,%rcx
-    646c5b61:	add    %r13,%rax
-    646c5b64:	cmp    $0x10,%edx
-    646c5b67:	mov    (%rax),%r9
-    646c5b6a:	jne    646c5b12 <_pei386_runtime_relocator+0x1a2>
-    646c5b6c:	movzwl (%rcx),%r8d
-    646c5b70:	mov    %r14,%rdx
-    646c5b73:	mov    %r14,%rdi
-    646c5b76:	mov    %r8,%r10
-    646c5b79:	or     $0xffffffffffff0000,%r10
-    646c5b80:	test   %r8w,%r8w
-    646c5b84:	cmovs  %r10,%r8
-    646c5b88:	sub    %rax,%r8
-    646c5b8b:	add    %r9,%r8
-    646c5b8e:	mov    %r8,-0x58(%rbp)
-    646c5b92:	mov    $0x2,%r8d
-    646c5b98:	call   646c57a0 <__write_memory.part.0>
-    646c5b9d:	jmp    646c5b48 <_pei386_runtime_relocator+0x1d8>
-    646c5b9f:	nop
-    646c5ba0:	mov    (%rcx),%edx
-    646c5ba2:	mov    %r14,%rdi
-    646c5ba5:	mov    %rdx,%r8
-    646c5ba8:	or     %r15,%rdx
-    646c5bab:	test   %r8d,%r8d
-    646c5bae:	cmovns %r8,%rdx
-    646c5bb2:	mov    $0x4,%r8d
-    646c5bb8:	sub    %rax,%rdx
-    646c5bbb:	add    %r9,%rdx
-    646c5bbe:	mov    %rdx,-0x58(%rbp)
-    646c5bc2:	mov    %r14,%rdx
-    646c5bc5:	call   646c57a0 <__write_memory.part.0>
-    646c5bca:	jmp    646c5b48 <_pei386_runtime_relocator+0x1d8>
-    646c5bcf:	nop
-    646c5bd0:	cmp    $0x8,%edx
-    646c5bd3:	jne    646c5c0a <_pei386_runtime_relocator+0x29a>
-    646c5bd5:	movzbl (%rcx),%r8d
-    646c5bd9:	mov    %r14,%rdx
-    646c5bdc:	mov    %r14,%rdi
-    646c5bdf:	mov    %r8,%r10
-    646c5be2:	or     $0xffffffffffffff00,%r10
-    646c5be9:	test   %r8b,%r8b
-    646c5bec:	cmovs  %r10,%r8
-    646c5bf0:	sub    %rax,%r8
-    646c5bf3:	add    %r9,%r8
-    646c5bf6:	mov    %r8,-0x58(%rbp)
-    646c5bfa:	mov    $0x1,%r8d
-    646c5c00:	call   646c57a0 <__write_memory.part.0>
-    646c5c05:	jmp    646c5b48 <_pei386_runtime_relocator+0x1d8>
-    646c5c0a:	lea    0x36c7(%rip),%rcx        # 646c92d8 <.rdata+0xd8>
-    646c5c11:	movq   $0x0,-0x58(%rbp)
-    646c5c19:	call   646c7d30 <__report_error>
-    646c5c1e:	lea    0x367b(%rip),%rcx        # 646c92a0 <.rdata+0xa0>
-    646c5c25:	call   646c7d30 <__report_error>
-    646c5c2a:	nop
-    646c5c2b:	nop
-    646c5c2c:	nop
-    646c5c2d:	nop
-    646c5c2e:	nop
+00000000646c5780 <__dyn_tls_init>:
+    646c5780:	push   %rsi
+    646c5781:	push   %rbx
+    646c5782:	sub    $0x28,%rsp
+    646c5786:	mov    0x3e53(%rip),%rax        # 646c95e0 <.refptr._CRT_MT>
+    646c578d:	cmpl   $0x2,(%rax)
+    646c5790:	je     646c5798 <__dyn_tls_init+0x18>
+    646c5792:	movl   $0x2,(%rax)
+    646c5798:	cmp    $0x2,%edx
+    646c579b:	je     646c57b0 <__dyn_tls_init+0x30>
+    646c579d:	cmp    $0x1,%edx
+    646c57a0:	je     646c57e2 <__dyn_tls_init+0x62>
+    646c57a2:	mov    $0x1,%eax
+    646c57a7:	add    $0x28,%rsp
+    646c57ab:	pop    %rbx
+    646c57ac:	pop    %rsi
+    646c57ad:	ret
+    646c57ae:	xchg   %ax,%ax
+    646c57b0:	lea    0x9899(%rip),%rbx        # 646cf050 <__xd_z>
+    646c57b7:	lea    0x9892(%rip),%rsi        # 646cf050 <__xd_z>
+    646c57be:	cmp    %rbx,%rsi
+    646c57c1:	je     646c57a2 <__dyn_tls_init+0x22>
+    646c57c3:	mov    (%rbx),%rax
+    646c57c6:	test   %rax,%rax
+    646c57c9:	je     646c57cd <__dyn_tls_init+0x4d>
+    646c57cb:	call   *%rax
+    646c57cd:	add    $0x8,%rbx
+    646c57d1:	cmp    %rbx,%rsi
+    646c57d4:	jne    646c57c3 <__dyn_tls_init+0x43>
+    646c57d6:	mov    $0x1,%eax
+    646c57db:	add    $0x28,%rsp
+    646c57df:	pop    %rbx
+    646c57e0:	pop    %rsi
+    646c57e1:	ret
+    646c57e2:	call   646c62d0 <__mingw_TLScallback>
+    646c57e7:	mov    $0x1,%eax
+    646c57ec:	add    $0x28,%rsp
+    646c57f0:	pop    %rbx
+    646c57f1:	pop    %rsi
+    646c57f2:	ret
+    646c57f3:	nopl   (%rax)
+    646c57f6:	cs nopw 0x0(%rax,%rax,1)
+
+00000000646c5800 <__tlregdtor>:
+    646c5800:	xor    %eax,%eax
+    646c5802:	ret
+    646c5803:	nop
+    646c5804:	nop
+    646c5805:	nop
+    646c5806:	nop
+    646c5807:	nop
+    646c5808:	nop
+    646c5809:	nop
+    646c580a:	nop
+    646c580b:	nop
+    646c580c:	nop
+    646c580d:	nop
+    646c580e:	nop
+    646c580f:	nop
+
+00000000646c5810 <_decode_pointer>:
+    646c5810:	mov    %rcx,%rax
+    646c5813:	ret
+    646c5814:	xchg   %ax,%ax
+    646c5816:	cs nopw 0x0(%rax,%rax,1)
+
+00000000646c5820 <_encode_pointer>:
+    646c5820:	mov    %rcx,%rax
+    646c5823:	ret
+    646c5824:	nop
+    646c5825:	nop
+    646c5826:	nop
+    646c5827:	nop
+    646c5828:	nop
+    646c5829:	nop
+    646c582a:	nop
+    646c582b:	nop
+    646c582c:	nop
+    646c582d:	nop
+    646c582e:	nop
+    646c582f:	nop
+
+00000000646c5830 <__write_memory.part.0>:
+    646c5830:	push   %r12
+    646c5832:	push   %rbp
+    646c5833:	push   %rdi
+    646c5834:	push   %rsi
+    646c5835:	push   %rbx
+    646c5836:	sub    $0x50,%rsp
+    646c583a:	movslq 0x7003(%rip),%rsi        # 646cc844 <maxSections>
+    646c5841:	test   %esi,%esi
+    646c5843:	mov    %rcx,%rbx
+    646c5846:	mov    %rdx,%rbp
+    646c5849:	mov    %r8,%rdi
+    646c584c:	jle    646c59b8 <__write_memory.part.0+0x188>
+    646c5852:	mov    0x6fef(%rip),%rax        # 646cc848 <the_secs>
+    646c5859:	xor    %ecx,%ecx
+    646c585b:	add    $0x18,%rax
+    646c585f:	nop
+    646c5860:	mov    (%rax),%rdx
+    646c5863:	cmp    %rdx,%rbx
+    646c5866:	jb     646c587c <__write_memory.part.0+0x4c>
+    646c5868:	mov    0x8(%rax),%r8
+    646c586c:	mov    0x8(%r8),%r8d
+    646c5870:	add    %r8,%rdx
+    646c5873:	cmp    %rdx,%rbx
+    646c5876:	jb     646c5905 <__write_memory.part.0+0xd5>
+    646c587c:	add    $0x1,%ecx
+    646c587f:	add    $0x28,%rax
+    646c5883:	cmp    %esi,%ecx
+    646c5885:	jne    646c5860 <__write_memory.part.0+0x30>
+    646c5887:	mov    %rbx,%rcx
+    646c588a:	call   646c64d0 <__mingw_GetSectionForAddress>
+    646c588f:	test   %rax,%rax
+    646c5892:	mov    %rax,%r12
+    646c5895:	je     646c59ed <__write_memory.part.0+0x1bd>
+    646c589b:	mov    0x6fa6(%rip),%rax        # 646cc848 <the_secs>
+    646c58a2:	lea    (%rsi,%rsi,4),%rsi
+    646c58a6:	shl    $0x3,%rsi
+    646c58aa:	add    %rsi,%rax
+    646c58ad:	mov    %r12,0x20(%rax)
+    646c58b1:	movl   $0x0,(%rax)
+    646c58b7:	call   646c6600 <_GetPEImageBase>
+    646c58bc:	mov    0xc(%r12),%ecx
+    646c58c1:	lea    0x20(%rsp),%rdx
+    646c58c6:	mov    $0x30,%r8d
+    646c58cc:	add    %rax,%rcx
+    646c58cf:	mov    0x6f72(%rip),%rax        # 646cc848 <the_secs>
+    646c58d6:	mov    %rcx,0x18(%rax,%rsi,1)
+    646c58db:	call   *0x8993(%rip)        # 646ce274 <__imp_VirtualQuery>
+    646c58e1:	test   %rax,%rax
+    646c58e4:	je     646c59d0 <__write_memory.part.0+0x1a0>
+    646c58ea:	mov    0x44(%rsp),%eax
+    646c58ee:	lea    -0x4(%rax),%edx
+    646c58f1:	and    $0xfffffffb,%edx
+    646c58f4:	je     646c58fe <__write_memory.part.0+0xce>
+    646c58f6:	sub    $0x40,%eax
+    646c58f9:	and    $0xffffffbf,%eax
+    646c58fc:	jne    646c5960 <__write_memory.part.0+0x130>
+    646c58fe:	addl   $0x1,0x6f3f(%rip)        # 646cc844 <maxSections>
+    646c5905:	cmp    $0x8,%edi
+    646c5908:	jae    646c5933 <__write_memory.part.0+0x103>
+    646c590a:	test   $0x4,%dil
+    646c590e:	jne    646c59a4 <__write_memory.part.0+0x174>
+    646c5914:	test   %edi,%edi
+    646c5916:	je     646c5928 <__write_memory.part.0+0xf8>
+    646c5918:	movzbl 0x0(%rbp),%eax
+    646c591c:	test   $0x2,%dil
+    646c5920:	mov    %al,(%rbx)
+    646c5922:	jne    646c59bf <__write_memory.part.0+0x18f>
+    646c5928:	add    $0x50,%rsp
+    646c592c:	pop    %rbx
+    646c592d:	pop    %rsi
+    646c592e:	pop    %rdi
+    646c592f:	pop    %rbp
+    646c5930:	pop    %r12
+    646c5932:	ret
+    646c5933:	mov    %edi,%eax
+    646c5935:	sub    $0x1,%edi
+    646c5938:	mov    -0x8(%rbp,%rax,1),%rdx
+    646c593d:	cmp    $0x8,%edi
+    646c5940:	mov    %rdx,-0x8(%rbx,%rax,1)
+    646c5945:	jb     646c5928 <__write_memory.part.0+0xf8>
+    646c5947:	and    $0xfffffff8,%edi
+    646c594a:	xor    %eax,%eax
+    646c594c:	mov    %eax,%edx
+    646c594e:	add    $0x8,%eax
+    646c5951:	mov    0x0(%rbp,%rdx,1),%rcx
+    646c5956:	cmp    %edi,%eax
+    646c5958:	mov    %rcx,(%rbx,%rdx,1)
+    646c595c:	jb     646c594c <__write_memory.part.0+0x11c>
+    646c595e:	jmp    646c5928 <__write_memory.part.0+0xf8>
+    646c5960:	add    0x6ee1(%rip),%rsi        # 646cc848 <the_secs>
+    646c5967:	mov    $0x40,%r8d
+    646c596d:	mov    0x20(%rsp),%rcx
+    646c5972:	mov    0x38(%rsp),%rdx
+    646c5977:	mov    %rsi,%r9
+    646c597a:	mov    %rcx,0x8(%rsi)
+    646c597e:	mov    %rdx,0x10(%rsi)
+    646c5982:	call   *0x88e4(%rip)        # 646ce26c <__imp_VirtualProtect>
+    646c5988:	test   %eax,%eax
+    646c598a:	jne    646c58fe <__write_memory.part.0+0xce>
+    646c5990:	call   *0x885e(%rip)        # 646ce1f4 <__imp_GetLastError>
+    646c5996:	lea    0x38db(%rip),%rcx        # 646c9278 <.rdata+0x78>
+    646c599d:	mov    %eax,%edx
+    646c599f:	call   646c7dc0 <__report_error>
+    646c59a4:	mov    0x0(%rbp),%eax
+    646c59a7:	mov    %edi,%edi
+    646c59a9:	mov    %eax,(%rbx)
+    646c59ab:	mov    -0x4(%rbp,%rdi,1),%eax
+    646c59af:	mov    %eax,-0x4(%rbx,%rdi,1)
+    646c59b3:	jmp    646c5928 <__write_memory.part.0+0xf8>
+    646c59b8:	xor    %esi,%esi
+    646c59ba:	jmp    646c5887 <__write_memory.part.0+0x57>
+    646c59bf:	mov    %edi,%edi
+    646c59c1:	movzwl -0x2(%rbp,%rdi,1),%eax
+    646c59c6:	mov    %ax,-0x2(%rbx,%rdi,1)
+    646c59cb:	jmp    646c5928 <__write_memory.part.0+0xf8>
+    646c59d0:	mov    0x6e71(%rip),%rax        # 646cc848 <the_secs>
+    646c59d7:	lea    0x3862(%rip),%rcx        # 646c9240 <.rdata+0x40>
+    646c59de:	mov    0x8(%r12),%edx
+    646c59e3:	mov    0x18(%rax,%rsi,1),%r8
+    646c59e8:	call   646c7dc0 <__report_error>
+    646c59ed:	lea    0x382c(%rip),%rcx        # 646c9220 <.rdata+0x20>
+    646c59f4:	mov    %rbx,%rdx
+    646c59f7:	call   646c7dc0 <__report_error>
+    646c59fc:	nop
+    646c59fd:	nopl   (%rax)
+
+00000000646c5a00 <_pei386_runtime_relocator>:
+    646c5a00:	push   %rbp
+    646c5a01:	push   %r15
+    646c5a03:	push   %r14
+    646c5a05:	push   %r13
+    646c5a07:	push   %r12
+    646c5a09:	push   %rdi
+    646c5a0a:	push   %rsi
+    646c5a0b:	push   %rbx
+    646c5a0c:	sub    $0x38,%rsp
+    646c5a10:	lea    0x80(%rsp),%rbp
+    646c5a18:	mov    0x6e22(%rip),%ebx        # 646cc840 <was_init.95174>
+    646c5a1e:	test   %ebx,%ebx
+    646c5a20:	je     646c5a33 <_pei386_runtime_relocator+0x33>
+    646c5a22:	lea    -0x48(%rbp),%rsp
+    646c5a26:	pop    %rbx
+    646c5a27:	pop    %rsi
+    646c5a28:	pop    %rdi
+    646c5a29:	pop    %r12
+    646c5a2b:	pop    %r13
+    646c5a2d:	pop    %r14
+    646c5a2f:	pop    %r15
+    646c5a31:	pop    %rbp
+    646c5a32:	ret
+    646c5a33:	movl   $0x1,0x6e03(%rip)        # 646cc840 <was_init.95174>
+    646c5a3d:	call   646c6550 <__mingw_GetSectionCount>
+    646c5a42:	cltq
+    646c5a44:	lea    (%rax,%rax,4),%rax
+    646c5a48:	lea    0x1e(,%rax,8),%rax
+    646c5a50:	and    $0xfffffffffffffff0,%rax
+    646c5a54:	call   646c67a0 <___chkstk_ms>
+    646c5a59:	mov    0x3ba0(%rip),%r12        # 646c9600 <.refptr.__RUNTIME_PSEUDO_RELOC_LIST_END__>
+    646c5a60:	movl   $0x0,0x6dda(%rip)        # 646cc844 <maxSections>
+    646c5a6a:	mov    0x3b9f(%rip),%rsi        # 646c9610 <.refptr.__RUNTIME_PSEUDO_RELOC_LIST__>
+    646c5a71:	sub    %rax,%rsp
+    646c5a74:	lea    0x20(%rsp),%rax
+    646c5a79:	mov    %rax,0x6dc8(%rip)        # 646cc848 <the_secs>
+    646c5a80:	mov    %r12,%rax
+    646c5a83:	sub    %rsi,%rax
+    646c5a86:	cmp    $0x7,%rax
+    646c5a8a:	jle    646c5a22 <_pei386_runtime_relocator+0x22>
+    646c5a8c:	cmp    $0xb,%rax
+    646c5a90:	mov    (%rsi),%edx
+    646c5a92:	jle    646c5b60 <_pei386_runtime_relocator+0x160>
+    646c5a98:	test   %edx,%edx
+    646c5a9a:	je     646c5b44 <_pei386_runtime_relocator+0x144>
+    646c5aa0:	cmp    %r12,%rsi
+    646c5aa3:	jae    646c5a22 <_pei386_runtime_relocator+0x22>
+    646c5aa9:	lea    0x8(%rsi),%r14
+    646c5aad:	add    $0x7,%r12
+    646c5ab1:	mov    0x3b78(%rip),%r13        # 646c9630 <.refptr.__image_base__>
+    646c5ab8:	lea    -0x58(%rbp),%rdi
+    646c5abc:	sub    %r14,%r12
+    646c5abf:	shr    $0x3,%r12
+    646c5ac3:	lea    0x8(%rsi,%r12,8),%r12
+    646c5ac8:	jmp    646c5ad4 <_pei386_runtime_relocator+0xd4>
+    646c5aca:	nopw   0x0(%rax,%rax,1)
+    646c5ad0:	add    $0x8,%r14
+    646c5ad4:	mov    0x4(%rsi),%ecx
+    646c5ad7:	mov    $0x4,%r8d
+    646c5add:	mov    %rdi,%rdx
+    646c5ae0:	mov    (%rsi),%eax
+    646c5ae2:	mov    %r14,%rsi
+    646c5ae5:	add    %r13,%rcx
+    646c5ae8:	add    (%rcx),%eax
+    646c5aea:	mov    %eax,-0x58(%rbp)
+    646c5aed:	call   646c5830 <__write_memory.part.0>
+    646c5af2:	cmp    %r12,%r14
+    646c5af5:	jne    646c5ad0 <_pei386_runtime_relocator+0xd0>
+    646c5af7:	mov    0x6d47(%rip),%eax        # 646cc844 <maxSections>
+    646c5afd:	xor    %esi,%esi
+    646c5aff:	mov    0x8766(%rip),%r12        # 646ce26c <__imp_VirtualProtect>
+    646c5b06:	test   %eax,%eax
+    646c5b08:	jle    646c5a22 <_pei386_runtime_relocator+0x22>
+    646c5b0e:	xchg   %ax,%ax
+    646c5b10:	mov    0x6d31(%rip),%rax        # 646cc848 <the_secs>
+    646c5b17:	add    %rsi,%rax
+    646c5b1a:	mov    (%rax),%r8d
+    646c5b1d:	test   %r8d,%r8d
+    646c5b20:	je     646c5b30 <_pei386_runtime_relocator+0x130>
+    646c5b22:	mov    0x10(%rax),%rdx
+    646c5b26:	mov    %rdi,%r9
+    646c5b29:	mov    0x8(%rax),%rcx
+    646c5b2d:	call   *%r12
+    646c5b30:	add    $0x1,%ebx
+    646c5b33:	add    $0x28,%rsi
+    646c5b37:	cmp    0x6d07(%rip),%ebx        # 646cc844 <maxSections>
+    646c5b3d:	jl     646c5b10 <_pei386_runtime_relocator+0x110>
+    646c5b3f:	jmp    646c5a22 <_pei386_runtime_relocator+0x22>
+    646c5b44:	mov    0x4(%rsi),%ecx
+    646c5b47:	test   %ecx,%ecx
+    646c5b49:	jne    646c5aa0 <_pei386_runtime_relocator+0xa0>
+    646c5b4f:	mov    0x8(%rsi),%edx
+    646c5b52:	test   %edx,%edx
+    646c5b54:	jne    646c5b73 <_pei386_runtime_relocator+0x173>
+    646c5b56:	mov    0xc(%rsi),%edx
+    646c5b59:	add    $0xc,%rsi
+    646c5b5d:	nopl   (%rax)
+    646c5b60:	test   %edx,%edx
+    646c5b62:	jne    646c5aa0 <_pei386_runtime_relocator+0xa0>
+    646c5b68:	mov    0x4(%rsi),%eax
+    646c5b6b:	test   %eax,%eax
+    646c5b6d:	jne    646c5aa0 <_pei386_runtime_relocator+0xa0>
+    646c5b73:	mov    0x8(%rsi),%edx
+    646c5b76:	cmp    $0x1,%edx
+    646c5b79:	jne    646c5cae <_pei386_runtime_relocator+0x2ae>
+    646c5b7f:	mov    0x3aaa(%rip),%r13        # 646c9630 <.refptr.__image_base__>
+    646c5b86:	add    $0xc,%rsi
+    646c5b8a:	movabs $0xffffffff00000000,%r15
+    646c5b94:	lea    -0x58(%rbp),%r14
+    646c5b98:	cmp    %r12,%rsi
+    646c5b9b:	jb     646c5be5 <_pei386_runtime_relocator+0x1e5>
+    646c5b9d:	jmp    646c5a22 <_pei386_runtime_relocator+0x22>
+    646c5ba2:	jbe    646c5c60 <_pei386_runtime_relocator+0x260>
+    646c5ba8:	cmp    $0x20,%edx
+    646c5bab:	je     646c5c30 <_pei386_runtime_relocator+0x230>
+    646c5bb1:	cmp    $0x40,%edx
+    646c5bb4:	jne    646c5c9a <_pei386_runtime_relocator+0x29a>
+    646c5bba:	mov    (%rcx),%rdx
+    646c5bbd:	mov    $0x8,%r8d
+    646c5bc3:	mov    %r14,%rdi
+    646c5bc6:	sub    %rax,%rdx
+    646c5bc9:	add    %r9,%rdx
+    646c5bcc:	mov    %rdx,-0x58(%rbp)
+    646c5bd0:	mov    %r14,%rdx
+    646c5bd3:	call   646c5830 <__write_memory.part.0>
+    646c5bd8:	add    $0xc,%rsi
+    646c5bdc:	cmp    %r12,%rsi
+    646c5bdf:	jae    646c5af7 <_pei386_runtime_relocator+0xf7>
+    646c5be5:	mov    0x4(%rsi),%ecx
+    646c5be8:	mov    (%rsi),%eax
+    646c5bea:	movzbl 0x8(%rsi),%edx
+    646c5bee:	add    %r13,%rcx
+    646c5bf1:	add    %r13,%rax
+    646c5bf4:	cmp    $0x10,%edx
+    646c5bf7:	mov    (%rax),%r9
+    646c5bfa:	jne    646c5ba2 <_pei386_runtime_relocator+0x1a2>
+    646c5bfc:	movzwl (%rcx),%r8d
+    646c5c00:	mov    %r14,%rdx
+    646c5c03:	mov    %r14,%rdi
+    646c5c06:	mov    %r8,%r10
+    646c5c09:	or     $0xffffffffffff0000,%r10
+    646c5c10:	test   %r8w,%r8w
+    646c5c14:	cmovs  %r10,%r8
+    646c5c18:	sub    %rax,%r8
+    646c5c1b:	add    %r9,%r8
+    646c5c1e:	mov    %r8,-0x58(%rbp)
+    646c5c22:	mov    $0x2,%r8d
+    646c5c28:	call   646c5830 <__write_memory.part.0>
+    646c5c2d:	jmp    646c5bd8 <_pei386_runtime_relocator+0x1d8>
     646c5c2f:	nop
-
-00000000646c5c30 <__mingw_SEH_error_handler>:
-    646c5c30:	sub    $0x28,%rsp
-    646c5c34:	mov    (%rcx),%eax
-    646c5c36:	cmp    $0xc0000091,%eax
-    646c5c3b:	ja     646c5ca0 <__mingw_SEH_error_handler+0x70>
-    646c5c3d:	cmp    $0xc000008d,%eax
-    646c5c42:	jae    646c5cbf <__mingw_SEH_error_handler+0x8f>
-    646c5c44:	cmp    $0xc0000008,%eax
-    646c5c49:	je     646c5d54 <__mingw_SEH_error_handler+0x124>
-    646c5c4f:	ja     646c5d20 <__mingw_SEH_error_handler+0xf0>
-    646c5c55:	cmp    $0x80000002,%eax
-    646c5c5a:	je     646c5d54 <__mingw_SEH_error_handler+0x124>
-    646c5c60:	cmp    $0xc0000005,%eax
-    646c5c65:	jne    646c5d2e <__mingw_SEH_error_handler+0xfe>
-    646c5c6b:	xor    %edx,%edx
-    646c5c6d:	mov    $0xb,%ecx
-    646c5c72:	call   646c78c8 <signal>
-    646c5c77:	cmp    $0x1,%rax
-    646c5c7b:	je     646c5db0 <__mingw_SEH_error_handler+0x180>
-    646c5c81:	test   %rax,%rax
-    646c5c84:	je     646c5dc6 <__mingw_SEH_error_handler+0x196>
-    646c5c8a:	mov    $0xb,%ecx
-    646c5c8f:	call   *%rax
-    646c5c91:	xor    %eax,%eax
-    646c5c93:	add    $0x28,%rsp
-    646c5c97:	ret
-    646c5c98:	nopl   0x0(%rax,%rax,1)
-    646c5ca0:	cmp    $0xc0000094,%eax
-    646c5ca5:	je     646c5d60 <__mingw_SEH_error_handler+0x130>
-    646c5cab:	ja     646c5ce4 <__mingw_SEH_error_handler+0xb4>
-    646c5cad:	cmp    $0xc0000092,%eax
-    646c5cb2:	je     646c5d54 <__mingw_SEH_error_handler+0x124>
-    646c5cb8:	cmp    $0xc0000093,%eax
-    646c5cbd:	jne    646c5d2e <__mingw_SEH_error_handler+0xfe>
-    646c5cbf:	xor    %edx,%edx
-    646c5cc1:	mov    $0x8,%ecx
-    646c5cc6:	call   646c78c8 <signal>
-    646c5ccb:	cmp    $0x1,%rax
-    646c5ccf:	je     646c5d40 <__mingw_SEH_error_handler+0x110>
-    646c5cd1:	test   %rax,%rax
-    646c5cd4:	je     646c5d2e <__mingw_SEH_error_handler+0xfe>
-    646c5cd6:	mov    $0x8,%ecx
-    646c5cdb:	call   *%rax
-    646c5cdd:	xor    %eax,%eax
-    646c5cdf:	add    $0x28,%rsp
-    646c5ce3:	ret
-    646c5ce4:	cmp    $0xc0000095,%eax
-    646c5ce9:	je     646c5d54 <__mingw_SEH_error_handler+0x124>
-    646c5ceb:	cmp    $0xc0000096,%eax
-    646c5cf0:	jne    646c5d2e <__mingw_SEH_error_handler+0xfe>
-    646c5cf2:	xor    %edx,%edx
-    646c5cf4:	mov    $0x4,%ecx
-    646c5cf9:	call   646c78c8 <signal>
-    646c5cfe:	cmp    $0x1,%rax
-    646c5d02:	je     646c5d90 <__mingw_SEH_error_handler+0x160>
-    646c5d08:	test   %rax,%rax
-    646c5d0b:	je     646c5dc6 <__mingw_SEH_error_handler+0x196>
-    646c5d11:	mov    $0x4,%ecx
-    646c5d16:	call   *%rax
-    646c5d18:	xor    %eax,%eax
-    646c5d1a:	add    $0x28,%rsp
-    646c5d1e:	ret
-    646c5d1f:	nop
-    646c5d20:	cmp    $0xc000001d,%eax
-    646c5d25:	je     646c5cf2 <__mingw_SEH_error_handler+0xc2>
-    646c5d27:	cmp    $0xc000008c,%eax
-    646c5d2c:	je     646c5d54 <__mingw_SEH_error_handler+0x124>
-    646c5d2e:	mov    $0x1,%eax
-    646c5d33:	add    $0x28,%rsp
-    646c5d37:	ret
-    646c5d38:	nopl   0x0(%rax,%rax,1)
-    646c5d40:	mov    $0x1,%edx
-    646c5d45:	mov    $0x8,%ecx
-    646c5d4a:	call   646c78c8 <signal>
-    646c5d4f:	call   646c6700 <_fpreset>
-    646c5d54:	xor    %eax,%eax
-    646c5d56:	add    $0x28,%rsp
-    646c5d5a:	ret
-    646c5d5b:	nopl   0x0(%rax,%rax,1)
-    646c5d60:	xor    %edx,%edx
-    646c5d62:	mov    $0x8,%ecx
-    646c5d67:	call   646c78c8 <signal>
-    646c5d6c:	cmp    $0x1,%rax
-    646c5d70:	jne    646c5cd1 <__mingw_SEH_error_handler+0xa1>
-    646c5d76:	mov    $0x1,%edx
-    646c5d7b:	mov    $0x8,%ecx
-    646c5d80:	call   646c78c8 <signal>
-    646c5d85:	xor    %eax,%eax
-    646c5d87:	jmp    646c5c93 <__mingw_SEH_error_handler+0x63>
-    646c5d8c:	nopl   0x0(%rax)
-    646c5d90:	mov    $0x1,%edx
-    646c5d95:	mov    $0x4,%ecx
-    646c5d9a:	call   646c78c8 <signal>
-    646c5d9f:	xor    %eax,%eax
-    646c5da1:	jmp    646c5c93 <__mingw_SEH_error_handler+0x63>
-    646c5da6:	cs nopw 0x0(%rax,%rax,1)
-    646c5db0:	mov    $0x1,%edx
-    646c5db5:	mov    $0xb,%ecx
-    646c5dba:	call   646c78c8 <signal>
-    646c5dbf:	xor    %eax,%eax
-    646c5dc1:	jmp    646c5c93 <__mingw_SEH_error_handler+0x63>
-    646c5dc6:	mov    $0x4,%eax
-    646c5dcb:	jmp    646c5c93 <__mingw_SEH_error_handler+0x63>
-
-00000000646c5dd0 <__mingw_init_ehandler>:
-    646c5dd0:	push   %r12
-    646c5dd2:	push   %rbp
-    646c5dd3:	push   %rdi
-    646c5dd4:	push   %rsi
-    646c5dd5:	push   %rbx
-    646c5dd6:	sub    $0x20,%rsp
-    646c5dda:	call   646c6570 <_GetPEImageBase>
-    646c5ddf:	mov    %rax,%rbp
-    646c5de2:	mov    0x6a80(%rip),%eax        # 646cc868 <was_here.95013>
-    646c5de8:	test   %eax,%eax
-    646c5dea:	jne    646c5e11 <__mingw_init_ehandler+0x41>
-    646c5dec:	test   %rbp,%rbp
-    646c5def:	je     646c5e11 <__mingw_init_ehandler+0x41>
-    646c5df1:	lea    0x3518(%rip),%rcx        # 646c9310 <.rdata>
-    646c5df8:	movl   $0x1,0x6a66(%rip)        # 646cc868 <was_here.95013>
-    646c5e02:	call   646c63b0 <_FindPESectionByName>
-    646c5e07:	test   %rax,%rax
-    646c5e0a:	je     646c5e20 <__mingw_init_ehandler+0x50>
-    646c5e0c:	mov    $0x1,%eax
-    646c5e11:	add    $0x20,%rsp
-    646c5e15:	pop    %rbx
-    646c5e16:	pop    %rsi
-    646c5e17:	pop    %rdi
-    646c5e18:	pop    %rbp
-    646c5e19:	pop    %r12
-    646c5e1b:	ret
+    646c5c30:	mov    (%rcx),%edx
+    646c5c32:	mov    %r14,%rdi
+    646c5c35:	mov    %rdx,%r8
+    646c5c38:	or     %r15,%rdx
+    646c5c3b:	test   %r8d,%r8d
+    646c5c3e:	cmovns %r8,%rdx
+    646c5c42:	mov    $0x4,%r8d
+    646c5c48:	sub    %rax,%rdx
+    646c5c4b:	add    %r9,%rdx
+    646c5c4e:	mov    %rdx,-0x58(%rbp)
+    646c5c52:	mov    %r14,%rdx
+    646c5c55:	call   646c5830 <__write_memory.part.0>
+    646c5c5a:	jmp    646c5bd8 <_pei386_runtime_relocator+0x1d8>
+    646c5c5f:	nop
+    646c5c60:	cmp    $0x8,%edx
+    646c5c63:	jne    646c5c9a <_pei386_runtime_relocator+0x29a>
+    646c5c65:	movzbl (%rcx),%r8d
+    646c5c69:	mov    %r14,%rdx
+    646c5c6c:	mov    %r14,%rdi
+    646c5c6f:	mov    %r8,%r10
+    646c5c72:	or     $0xffffffffffffff00,%r10
+    646c5c79:	test   %r8b,%r8b
+    646c5c7c:	cmovs  %r10,%r8
+    646c5c80:	sub    %rax,%r8
+    646c5c83:	add    %r9,%r8
+    646c5c86:	mov    %r8,-0x58(%rbp)
+    646c5c8a:	mov    $0x1,%r8d
+    646c5c90:	call   646c5830 <__write_memory.part.0>
+    646c5c95:	jmp    646c5bd8 <_pei386_runtime_relocator+0x1d8>
+    646c5c9a:	lea    0x3637(%rip),%rcx        # 646c92d8 <.rdata+0xd8>
+    646c5ca1:	movq   $0x0,-0x58(%rbp)
+    646c5ca9:	call   646c7dc0 <__report_error>
+    646c5cae:	lea    0x35eb(%rip),%rcx        # 646c92a0 <.rdata+0xa0>
+    646c5cb5:	call   646c7dc0 <__report_error>
+    646c5cba:	nop
+    646c5cbb:	nop
+    646c5cbc:	nop
+    646c5cbd:	nop
+    646c5cbe:	nop
+    646c5cbf:	nop
+
+00000000646c5cc0 <__mingw_SEH_error_handler>:
+    646c5cc0:	sub    $0x28,%rsp
+    646c5cc4:	mov    (%rcx),%eax
+    646c5cc6:	cmp    $0xc0000091,%eax
+    646c5ccb:	ja     646c5d30 <__mingw_SEH_error_handler+0x70>
+    646c5ccd:	cmp    $0xc000008d,%eax
+    646c5cd2:	jae    646c5d4f <__mingw_SEH_error_handler+0x8f>
+    646c5cd4:	cmp    $0xc0000008,%eax
+    646c5cd9:	je     646c5de4 <__mingw_SEH_error_handler+0x124>
+    646c5cdf:	ja     646c5db0 <__mingw_SEH_error_handler+0xf0>
+    646c5ce5:	cmp    $0x80000002,%eax
+    646c5cea:	je     646c5de4 <__mingw_SEH_error_handler+0x124>
+    646c5cf0:	cmp    $0xc0000005,%eax
+    646c5cf5:	jne    646c5dbe <__mingw_SEH_error_handler+0xfe>
+    646c5cfb:	xor    %edx,%edx
+    646c5cfd:	mov    $0xb,%ecx
+    646c5d02:	call   646c7958 <signal>
+    646c5d07:	cmp    $0x1,%rax
+    646c5d0b:	je     646c5e40 <__mingw_SEH_error_handler+0x180>
+    646c5d11:	test   %rax,%rax
+    646c5d14:	je     646c5e56 <__mingw_SEH_error_handler+0x196>
+    646c5d1a:	mov    $0xb,%ecx
+    646c5d1f:	call   *%rax
+    646c5d21:	xor    %eax,%eax
+    646c5d23:	add    $0x28,%rsp
+    646c5d27:	ret
+    646c5d28:	nopl   0x0(%rax,%rax,1)
+    646c5d30:	cmp    $0xc0000094,%eax
+    646c5d35:	je     646c5df0 <__mingw_SEH_error_handler+0x130>
+    646c5d3b:	ja     646c5d74 <__mingw_SEH_error_handler+0xb4>
+    646c5d3d:	cmp    $0xc0000092,%eax
+    646c5d42:	je     646c5de4 <__mingw_SEH_error_handler+0x124>
+    646c5d48:	cmp    $0xc0000093,%eax
+    646c5d4d:	jne    646c5dbe <__mingw_SEH_error_handler+0xfe>
+    646c5d4f:	xor    %edx,%edx
+    646c5d51:	mov    $0x8,%ecx
+    646c5d56:	call   646c7958 <signal>
+    646c5d5b:	cmp    $0x1,%rax
+    646c5d5f:	je     646c5dd0 <__mingw_SEH_error_handler+0x110>
+    646c5d61:	test   %rax,%rax
+    646c5d64:	je     646c5dbe <__mingw_SEH_error_handler+0xfe>
+    646c5d66:	mov    $0x8,%ecx
+    646c5d6b:	call   *%rax
+    646c5d6d:	xor    %eax,%eax
+    646c5d6f:	add    $0x28,%rsp
+    646c5d73:	ret
+    646c5d74:	cmp    $0xc0000095,%eax
+    646c5d79:	je     646c5de4 <__mingw_SEH_error_handler+0x124>
+    646c5d7b:	cmp    $0xc0000096,%eax
+    646c5d80:	jne    646c5dbe <__mingw_SEH_error_handler+0xfe>
+    646c5d82:	xor    %edx,%edx
+    646c5d84:	mov    $0x4,%ecx
+    646c5d89:	call   646c7958 <signal>
+    646c5d8e:	cmp    $0x1,%rax
+    646c5d92:	je     646c5e20 <__mingw_SEH_error_handler+0x160>
+    646c5d98:	test   %rax,%rax
+    646c5d9b:	je     646c5e56 <__mingw_SEH_error_handler+0x196>
+    646c5da1:	mov    $0x4,%ecx
+    646c5da6:	call   *%rax
+    646c5da8:	xor    %eax,%eax
+    646c5daa:	add    $0x28,%rsp
+    646c5dae:	ret
+    646c5daf:	nop
+    646c5db0:	cmp    $0xc000001d,%eax
+    646c5db5:	je     646c5d82 <__mingw_SEH_error_handler+0xc2>
+    646c5db7:	cmp    $0xc000008c,%eax
+    646c5dbc:	je     646c5de4 <__mingw_SEH_error_handler+0x124>
+    646c5dbe:	mov    $0x1,%eax
+    646c5dc3:	add    $0x28,%rsp
+    646c5dc7:	ret
+    646c5dc8:	nopl   0x0(%rax,%rax,1)
+    646c5dd0:	mov    $0x1,%edx
+    646c5dd5:	mov    $0x8,%ecx
+    646c5dda:	call   646c7958 <signal>
+    646c5ddf:	call   646c6790 <_fpreset>
+    646c5de4:	xor    %eax,%eax
+    646c5de6:	add    $0x28,%rsp
+    646c5dea:	ret
+    646c5deb:	nopl   0x0(%rax,%rax,1)
+    646c5df0:	xor    %edx,%edx
+    646c5df2:	mov    $0x8,%ecx
+    646c5df7:	call   646c7958 <signal>
+    646c5dfc:	cmp    $0x1,%rax
+    646c5e00:	jne    646c5d61 <__mingw_SEH_error_handler+0xa1>
+    646c5e06:	mov    $0x1,%edx
+    646c5e0b:	mov    $0x8,%ecx
+    646c5e10:	call   646c7958 <signal>
+    646c5e15:	xor    %eax,%eax
+    646c5e17:	jmp    646c5d23 <__mingw_SEH_error_handler+0x63>
     646c5e1c:	nopl   0x0(%rax)
-    646c5e20:	lea    0x6b59(%rip),%rbx        # 646cc980 <emu_pdata>
-    646c5e27:	mov    $0x30,%ecx
-    646c5e2c:	xor    %esi,%esi
-    646c5e2e:	lea    0x6a4b(%rip),%rdx        # 646cc880 <emu_xdata>
-    646c5e35:	mov    %rbx,%rdi
-    646c5e38:	rep stos %rax,%es:(%rdi)
-    646c5e3b:	lea    -0x212(%rip),%r12        # 646c5c30 <__mingw_SEH_error_handler>
-    646c5e42:	mov    $0x20,%ecx
-    646c5e47:	mov    %rdx,%rdi
-    646c5e4a:	rep stos %rax,%es:(%rdi)
-    646c5e4d:	sub    %rbp,%r12
-    646c5e50:	mov    %rdx,%rdi
-    646c5e53:	jmp    646c5e83 <__mingw_init_ehandler+0xb3>
-    646c5e55:	movb   $0x9,(%rdi)
-    646c5e58:	add    $0x1,%rsi
-    646c5e5c:	add    $0xc,%rbx
-    646c5e60:	mov    %r12d,0x4(%rdi)
-    646c5e64:	mov    0xc(%rax),%ecx
-    646c5e67:	mov    %ecx,-0xc(%rbx)
-    646c5e6a:	add    0x8(%rax),%ecx
-    646c5e6d:	mov    %rdi,%rax
-    646c5e70:	add    $0x8,%rdi
-    646c5e74:	sub    %rbp,%rax
-    646c5e77:	mov    %eax,-0x4(%rbx)
-    646c5e7a:	mov    %ecx,-0x8(%rbx)
-    646c5e7d:	cmp    $0x20,%rsi
-    646c5e81:	je     646c5eb5 <__mingw_init_ehandler+0xe5>
-    646c5e83:	mov    %rsi,%rcx
-    646c5e86:	call   646c6500 <_FindPESectionExec>
-    646c5e8b:	test   %rax,%rax
-    646c5e8e:	jne    646c5e55 <__mingw_init_ehandler+0x85>
-    646c5e90:	test   %rsi,%rsi
-    646c5e93:	mov    %esi,%edx
-    646c5e95:	je     646c5e0c <__mingw_init_ehandler+0x3c>
-    646c5e9b:	nopl   0x0(%rax,%rax,1)
-    646c5ea0:	lea    0x6ad9(%rip),%rcx        # 646cc980 <emu_pdata>
-    646c5ea7:	mov    %rbp,%r8
-    646c5eaa:	call   *0x8374(%rip)        # 646ce224 <__imp_RtlAddFunctionTable>
-    646c5eb0:	jmp    646c5e0c <__mingw_init_ehandler+0x3c>
-    646c5eb5:	mov    $0x20,%edx
-    646c5eba:	jmp    646c5ea0 <__mingw_init_ehandler+0xd0>
-    646c5ebc:	nopl   0x0(%rax)
-
-00000000646c5ec0 <_gnu_exception_handler>:
-    646c5ec0:	push   %rbx
-    646c5ec1:	sub    $0x20,%rsp
-    646c5ec5:	mov    (%rcx),%rdx
-    646c5ec8:	mov    (%rdx),%eax
-    646c5eca:	mov    %rcx,%rbx
-    646c5ecd:	mov    %eax,%ecx
-    646c5ecf:	and    $0x20ffffff,%ecx
-    646c5ed5:	cmp    $0x20474343,%ecx
-    646c5edb:	je     646c5fa0 <_gnu_exception_handler+0xe0>
-    646c5ee1:	cmp    $0xc0000091,%eax
-    646c5ee6:	ja     646c5f50 <_gnu_exception_handler+0x90>
-    646c5ee8:	cmp    $0xc000008d,%eax
-    646c5eed:	jae    646c5f6b <_gnu_exception_handler+0xab>
-    646c5eef:	cmp    $0xc0000008,%eax
-    646c5ef4:	je     646c5faa <_gnu_exception_handler+0xea>
-    646c5efa:	ja     646c5ff4 <_gnu_exception_handler+0x134>
-    646c5f00:	cmp    $0x80000002,%eax
-    646c5f05:	je     646c5faa <_gnu_exception_handler+0xea>
-    646c5f0b:	cmp    $0xc0000005,%eax
-    646c5f10:	jne    646c5f31 <_gnu_exception_handler+0x71>
-    646c5f12:	xor    %edx,%edx
-    646c5f14:	mov    $0xb,%ecx
-    646c5f19:	call   646c78c8 <signal>
-    646c5f1e:	cmp    $0x1,%rax
-    646c5f22:	je     646c6079 <_gnu_exception_handler+0x1b9>
-    646c5f28:	test   %rax,%rax
-    646c5f2b:	jne    646c6040 <_gnu_exception_handler+0x180>
-    646c5f31:	mov    0x6928(%rip),%rax        # 646cc860 <__mingw_oldexcpt_handler>
-    646c5f38:	test   %rax,%rax
-    646c5f3b:	je     646c6051 <_gnu_exception_handler+0x191>
-    646c5f41:	mov    %rbx,%rcx
-    646c5f44:	add    $0x20,%rsp
-    646c5f48:	pop    %rbx
-    646c5f49:	rex.W jmp *%rax
+    646c5e20:	mov    $0x1,%edx
+    646c5e25:	mov    $0x4,%ecx
+    646c5e2a:	call   646c7958 <signal>
+    646c5e2f:	xor    %eax,%eax
+    646c5e31:	jmp    646c5d23 <__mingw_SEH_error_handler+0x63>
+    646c5e36:	cs nopw 0x0(%rax,%rax,1)
+    646c5e40:	mov    $0x1,%edx
+    646c5e45:	mov    $0xb,%ecx
+    646c5e4a:	call   646c7958 <signal>
+    646c5e4f:	xor    %eax,%eax
+    646c5e51:	jmp    646c5d23 <__mingw_SEH_error_handler+0x63>
+    646c5e56:	mov    $0x4,%eax
+    646c5e5b:	jmp    646c5d23 <__mingw_SEH_error_handler+0x63>
+
+00000000646c5e60 <__mingw_init_ehandler>:
+    646c5e60:	push   %r12
+    646c5e62:	push   %rbp
+    646c5e63:	push   %rdi
+    646c5e64:	push   %rsi
+    646c5e65:	push   %rbx
+    646c5e66:	sub    $0x20,%rsp
+    646c5e6a:	call   646c6600 <_GetPEImageBase>
+    646c5e6f:	mov    %rax,%rbp
+    646c5e72:	mov    0x69f0(%rip),%eax        # 646cc868 <was_here.95013>
+    646c5e78:	test   %eax,%eax
+    646c5e7a:	jne    646c5ea1 <__mingw_init_ehandler+0x41>
+    646c5e7c:	test   %rbp,%rbp
+    646c5e7f:	je     646c5ea1 <__mingw_init_ehandler+0x41>
+    646c5e81:	lea    0x3488(%rip),%rcx        # 646c9310 <.rdata>
+    646c5e88:	movl   $0x1,0x69d6(%rip)        # 646cc868 <was_here.95013>
+    646c5e92:	call   646c6440 <_FindPESectionByName>
+    646c5e97:	test   %rax,%rax
+    646c5e9a:	je     646c5eb0 <__mingw_init_ehandler+0x50>
+    646c5e9c:	mov    $0x1,%eax
+    646c5ea1:	add    $0x20,%rsp
+    646c5ea5:	pop    %rbx
+    646c5ea6:	pop    %rsi
+    646c5ea7:	pop    %rdi
+    646c5ea8:	pop    %rbp
+    646c5ea9:	pop    %r12
+    646c5eab:	ret
+    646c5eac:	nopl   0x0(%rax)
+    646c5eb0:	lea    0x6ac9(%rip),%rbx        # 646cc980 <emu_pdata>
+    646c5eb7:	mov    $0x30,%ecx
+    646c5ebc:	xor    %esi,%esi
+    646c5ebe:	lea    0x69bb(%rip),%rdx        # 646cc880 <emu_xdata>
+    646c5ec5:	mov    %rbx,%rdi
+    646c5ec8:	rep stos %rax,%es:(%rdi)
+    646c5ecb:	lea    -0x212(%rip),%r12        # 646c5cc0 <__mingw_SEH_error_handler>
+    646c5ed2:	mov    $0x20,%ecx
+    646c5ed7:	mov    %rdx,%rdi
+    646c5eda:	rep stos %rax,%es:(%rdi)
+    646c5edd:	sub    %rbp,%r12
+    646c5ee0:	mov    %rdx,%rdi
+    646c5ee3:	jmp    646c5f13 <__mingw_init_ehandler+0xb3>
+    646c5ee5:	movb   $0x9,(%rdi)
+    646c5ee8:	add    $0x1,%rsi
+    646c5eec:	add    $0xc,%rbx
+    646c5ef0:	mov    %r12d,0x4(%rdi)
+    646c5ef4:	mov    0xc(%rax),%ecx
+    646c5ef7:	mov    %ecx,-0xc(%rbx)
+    646c5efa:	add    0x8(%rax),%ecx
+    646c5efd:	mov    %rdi,%rax
+    646c5f00:	add    $0x8,%rdi
+    646c5f04:	sub    %rbp,%rax
+    646c5f07:	mov    %eax,-0x4(%rbx)
+    646c5f0a:	mov    %ecx,-0x8(%rbx)
+    646c5f0d:	cmp    $0x20,%rsi
+    646c5f11:	je     646c5f45 <__mingw_init_ehandler+0xe5>
+    646c5f13:	mov    %rsi,%rcx
+    646c5f16:	call   646c6590 <_FindPESectionExec>
+    646c5f1b:	test   %rax,%rax
+    646c5f1e:	jne    646c5ee5 <__mingw_init_ehandler+0x85>
+    646c5f20:	test   %rsi,%rsi
+    646c5f23:	mov    %esi,%edx
+    646c5f25:	je     646c5e9c <__mingw_init_ehandler+0x3c>
+    646c5f2b:	nopl   0x0(%rax,%rax,1)
+    646c5f30:	lea    0x6a49(%rip),%rcx        # 646cc980 <emu_pdata>
+    646c5f37:	mov    %rbp,%r8
+    646c5f3a:	call   *0x82e4(%rip)        # 646ce224 <__imp_RtlAddFunctionTable>
+    646c5f40:	jmp    646c5e9c <__mingw_init_ehandler+0x3c>
+    646c5f45:	mov    $0x20,%edx
+    646c5f4a:	jmp    646c5f30 <__mingw_init_ehandler+0xd0>
     646c5f4c:	nopl   0x0(%rax)
-    646c5f50:	cmp    $0xc0000094,%eax
-    646c5f55:	je     646c6010 <_gnu_exception_handler+0x150>
-    646c5f5b:	ja     646c5fb5 <_gnu_exception_handler+0xf5>
-    646c5f5d:	cmp    $0xc0000092,%eax
-    646c5f62:	je     646c5faa <_gnu_exception_handler+0xea>
-    646c5f64:	cmp    $0xc0000093,%eax
-    646c5f69:	jne    646c5f31 <_gnu_exception_handler+0x71>
-    646c5f6b:	xor    %edx,%edx
-    646c5f6d:	mov    $0x8,%ecx
-    646c5f72:	call   646c78c8 <signal>
-    646c5f77:	cmp    $0x1,%rax
-    646c5f7b:	je     646c6060 <_gnu_exception_handler+0x1a0>
-    646c5f81:	test   %rax,%rax
-    646c5f84:	je     646c5f31 <_gnu_exception_handler+0x71>
-    646c5f86:	mov    $0x8,%ecx
-    646c5f8b:	call   *%rax
-    646c5f8d:	mov    $0xffffffff,%eax
-    646c5f92:	add    $0x20,%rsp
-    646c5f96:	pop    %rbx
-    646c5f97:	ret
-    646c5f98:	nopl   0x0(%rax,%rax,1)
-    646c5fa0:	testb  $0x1,0x4(%rdx)
-    646c5fa4:	jne    646c5ee1 <_gnu_exception_handler+0x21>
-    646c5faa:	mov    $0xffffffff,%eax
-    646c5faf:	add    $0x20,%rsp
-    646c5fb3:	pop    %rbx
-    646c5fb4:	ret
-    646c5fb5:	cmp    $0xc0000095,%eax
-    646c5fba:	je     646c5faa <_gnu_exception_handler+0xea>
-    646c5fbc:	cmp    $0xc0000096,%eax
-    646c5fc1:	jne    646c5f31 <_gnu_exception_handler+0x71>
-    646c5fc7:	xor    %edx,%edx
-    646c5fc9:	mov    $0x4,%ecx
-    646c5fce:	call   646c78c8 <signal>
-    646c5fd3:	cmp    $0x1,%rax
-    646c5fd7:	je     646c6090 <_gnu_exception_handler+0x1d0>
-    646c5fdd:	test   %rax,%rax
-    646c5fe0:	je     646c5f31 <_gnu_exception_handler+0x71>
-    646c5fe6:	mov    $0x4,%ecx
-    646c5feb:	call   *%rax
-    646c5fed:	mov    $0xffffffff,%eax
-    646c5ff2:	jmp    646c5f92 <_gnu_exception_handler+0xd2>
-    646c5ff4:	cmp    $0xc000001d,%eax
-    646c5ff9:	je     646c5fc7 <_gnu_exception_handler+0x107>
-    646c5ffb:	cmp    $0xc000008c,%eax
-    646c6000:	jne    646c5f31 <_gnu_exception_handler+0x71>
-    646c6006:	jmp    646c5faa <_gnu_exception_handler+0xea>
-    646c6008:	nopl   0x0(%rax,%rax,1)
-    646c6010:	xor    %edx,%edx
-    646c6012:	mov    $0x8,%ecx
-    646c6017:	call   646c78c8 <signal>
-    646c601c:	cmp    $0x1,%rax
-    646c6020:	jne    646c5f81 <_gnu_exception_handler+0xc1>
-    646c6026:	mov    $0x1,%edx
-    646c602b:	mov    $0x8,%ecx
-    646c6030:	call   646c78c8 <signal>
-    646c6035:	mov    $0xffffffff,%eax
-    646c603a:	jmp    646c5f92 <_gnu_exception_handler+0xd2>
-    646c603f:	nop
-    646c6040:	mov    $0xb,%ecx
-    646c6045:	call   *%rax
-    646c6047:	mov    $0xffffffff,%eax
-    646c604c:	jmp    646c5f92 <_gnu_exception_handler+0xd2>
-    646c6051:	xor    %eax,%eax
-    646c6053:	jmp    646c5f92 <_gnu_exception_handler+0xd2>
-    646c6058:	nopl   0x0(%rax,%rax,1)
-    646c6060:	mov    $0x1,%edx
-    646c6065:	mov    $0x8,%ecx
-    646c606a:	call   646c78c8 <signal>
-    646c606f:	call   646c6700 <_fpreset>
-    646c6074:	jmp    646c5faa <_gnu_exception_handler+0xea>
-    646c6079:	mov    $0x1,%edx
-    646c607e:	mov    $0xb,%ecx
-    646c6083:	call   646c78c8 <signal>
-    646c6088:	or     $0xffffffff,%eax
-    646c608b:	jmp    646c5f92 <_gnu_exception_handler+0xd2>
-    646c6090:	mov    $0x1,%edx
-    646c6095:	mov    $0x4,%ecx
-    646c609a:	call   646c78c8 <signal>
-    646c609f:	or     $0xffffffff,%eax
-    646c60a2:	jmp    646c5f92 <_gnu_exception_handler+0xd2>
-    646c60a7:	nop
-    646c60a8:	nop
-    646c60a9:	nop
-    646c60aa:	nop
-    646c60ab:	nop
-    646c60ac:	nop
-    646c60ad:	nop
-    646c60ae:	nop
-    646c60af:	nop
-
-00000000646c60b0 <__mingwthr_run_key_dtors.part.0>:
-    646c60b0:	push   %rbp
-    646c60b1:	push   %rdi
-    646c60b2:	push   %rsi
-    646c60b3:	push   %rbx
-    646c60b4:	sub    $0x28,%rsp
-    646c60b8:	lea    0x6a61(%rip),%rcx        # 646ccb20 <__mingwthr_cs>
-    646c60bf:	call   *0x810f(%rip)        # 646ce1d4 <__imp_EnterCriticalSection>
-    646c60c5:	mov    0x6a34(%rip),%rbx        # 646ccb00 <key_dtor_list>
-    646c60cc:	test   %rbx,%rbx
-    646c60cf:	je     646c6104 <__mingwthr_run_key_dtors.part.0+0x54>
-    646c60d1:	mov    0x8184(%rip),%rbp        # 646ce25c <__imp_TlsGetValue>
-    646c60d8:	mov    0x8115(%rip),%rdi        # 646ce1f4 <__imp_GetLastError>
-    646c60df:	nop
-    646c60e0:	mov    (%rbx),%ecx
-    646c60e2:	call   *%rbp
-    646c60e4:	mov    %rax,%rsi
-    646c60e7:	call   *%rdi
-    646c60e9:	test   %eax,%eax
-    646c60eb:	jne    646c60fb <__mingwthr_run_key_dtors.part.0+0x4b>
-    646c60ed:	test   %rsi,%rsi
-    646c60f0:	je     646c60fb <__mingwthr_run_key_dtors.part.0+0x4b>
-    646c60f2:	mov    0x8(%rbx),%rax
-    646c60f6:	mov    %rsi,%rcx
-    646c60f9:	call   *%rax
-    646c60fb:	mov    0x10(%rbx),%rbx
-    646c60ff:	test   %rbx,%rbx
-    646c6102:	jne    646c60e0 <__mingwthr_run_key_dtors.part.0+0x30>
-    646c6104:	lea    0x6a15(%rip),%rcx        # 646ccb20 <__mingwthr_cs>
-    646c610b:	add    $0x28,%rsp
-    646c610f:	pop    %rbx
-    646c6110:	pop    %rsi
-    646c6111:	pop    %rdi
-    646c6112:	pop    %rbp
-    646c6113:	rex.W jmp *0x80fa(%rip)        # 646ce214 <__imp_LeaveCriticalSection>
-    646c611a:	nopw   0x0(%rax,%rax,1)
-
-00000000646c6120 <___w64_mingwthr_add_key_dtor>:
-    646c6120:	push   %rbp
-    646c6121:	push   %rdi
-    646c6122:	push   %rsi
-    646c6123:	push   %rbx
-    646c6124:	sub    $0x28,%rsp
-    646c6128:	mov    0x69da(%rip),%eax        # 646ccb08 <__mingwthr_cs_init>
-    646c612e:	xor    %esi,%esi
-    646c6130:	test   %eax,%eax
-    646c6132:	mov    %ecx,%ebp
-    646c6134:	mov    %rdx,%rdi
-    646c6137:	jne    646c6144 <___w64_mingwthr_add_key_dtor+0x24>
-    646c6139:	mov    %esi,%eax
-    646c613b:	add    $0x28,%rsp
-    646c613f:	pop    %rbx
-    646c6140:	pop    %rsi
-    646c6141:	pop    %rdi
-    646c6142:	pop    %rbp
-    646c6143:	ret
-    646c6144:	mov    $0x18,%edx
-    646c6149:	mov    $0x1,%ecx
-    646c614e:	call   646c7920 <calloc>
-    646c6153:	test   %rax,%rax
-    646c6156:	mov    %rax,%rbx
-    646c6159:	je     646c6198 <___w64_mingwthr_add_key_dtor+0x78>
-    646c615b:	mov    %ebp,(%rax)
-    646c615d:	lea    0x69bc(%rip),%rcx        # 646ccb20 <__mingwthr_cs>
-    646c6164:	mov    %rdi,0x8(%rax)
-    646c6168:	call   *0x8066(%rip)        # 646ce1d4 <__imp_EnterCriticalSection>
-    646c616e:	mov    0x698b(%rip),%rax        # 646ccb00 <key_dtor_list>
-    646c6175:	lea    0x69a4(%rip),%rcx        # 646ccb20 <__mingwthr_cs>
-    646c617c:	mov    %rbx,0x697d(%rip)        # 646ccb00 <key_dtor_list>
-    646c6183:	mov    %rax,0x10(%rbx)
-    646c6187:	call   *0x8087(%rip)        # 646ce214 <__imp_LeaveCriticalSection>
-    646c618d:	mov    %esi,%eax
-    646c618f:	add    $0x28,%rsp
-    646c6193:	pop    %rbx
-    646c6194:	pop    %rsi
-    646c6195:	pop    %rdi
-    646c6196:	pop    %rbp
-    646c6197:	ret
-    646c6198:	mov    $0xffffffff,%esi
-    646c619d:	jmp    646c6139 <___w64_mingwthr_add_key_dtor+0x19>
-    646c619f:	nop
-
-00000000646c61a0 <___w64_mingwthr_remove_key_dtor>:
-    646c61a0:	push   %rbx
-    646c61a1:	sub    $0x20,%rsp
-    646c61a5:	mov    0x695d(%rip),%eax        # 646ccb08 <__mingwthr_cs_init>
-    646c61ab:	test   %eax,%eax
-    646c61ad:	mov    %ecx,%ebx
-    646c61af:	jne    646c61c0 <___w64_mingwthr_remove_key_dtor+0x20>
-    646c61b1:	xor    %eax,%eax
-    646c61b3:	add    $0x20,%rsp
-    646c61b7:	pop    %rbx
-    646c61b8:	ret
-    646c61b9:	nopl   0x0(%rax)
-    646c61c0:	lea    0x6959(%rip),%rcx        # 646ccb20 <__mingwthr_cs>
-    646c61c7:	call   *0x8007(%rip)        # 646ce1d4 <__imp_EnterCriticalSection>
-    646c61cd:	mov    0x692c(%rip),%rax        # 646ccb00 <key_dtor_list>
-    646c61d4:	test   %rax,%rax
-    646c61d7:	je     646c61f3 <___w64_mingwthr_remove_key_dtor+0x53>
-    646c61d9:	mov    (%rax),%edx
-    646c61db:	cmp    %edx,%ebx
-    646c61dd:	jne    646c61ea <___w64_mingwthr_remove_key_dtor+0x4a>
-    646c61df:	jmp    646c6230 <___w64_mingwthr_remove_key_dtor+0x90>
-    646c61e1:	mov    (%rcx),%edx
-    646c61e3:	cmp    %ebx,%edx
-    646c61e5:	je     646c6210 <___w64_mingwthr_remove_key_dtor+0x70>
-    646c61e7:	mov    %rcx,%rax
-    646c61ea:	mov    0x10(%rax),%rcx
-    646c61ee:	test   %rcx,%rcx
-    646c61f1:	jne    646c61e1 <___w64_mingwthr_remove_key_dtor+0x41>
-    646c61f3:	lea    0x6926(%rip),%rcx        # 646ccb20 <__mingwthr_cs>
-    646c61fa:	call   *0x8014(%rip)        # 646ce214 <__imp_LeaveCriticalSection>
-    646c6200:	xor    %eax,%eax
-    646c6202:	add    $0x20,%rsp
-    646c6206:	pop    %rbx
-    646c6207:	ret
-    646c6208:	nopl   0x0(%rax,%rax,1)
-    646c6210:	mov    0x10(%rcx),%rdx
-    646c6214:	mov    %rdx,0x10(%rax)
-    646c6218:	call   646c78f8 <free>
-    646c621d:	lea    0x68fc(%rip),%rcx        # 646ccb20 <__mingwthr_cs>
-    646c6224:	call   *0x7fea(%rip)        # 646ce214 <__imp_LeaveCriticalSection>
-    646c622a:	jmp    646c6200 <___w64_mingwthr_remove_key_dtor+0x60>
-    646c622c:	nopl   0x0(%rax)
-    646c6230:	mov    0x10(%rax),%rdx
-    646c6234:	mov    %rax,%rcx
-    646c6237:	mov    %rdx,0x68c2(%rip)        # 646ccb00 <key_dtor_list>
-    646c623e:	jmp    646c6218 <___w64_mingwthr_remove_key_dtor+0x78>
-
-00000000646c6240 <__mingw_TLScallback>:
-    646c6240:	push   %rbx
-    646c6241:	sub    $0x20,%rsp
-    646c6245:	cmp    $0x1,%edx
-    646c6248:	je     646c62e0 <__mingw_TLScallback+0xa0>
-    646c624e:	jb     646c6280 <__mingw_TLScallback+0x40>
-    646c6250:	cmp    $0x2,%edx
-    646c6253:	je     646c6270 <__mingw_TLScallback+0x30>
-    646c6255:	cmp    $0x3,%edx
-    646c6258:	jne    646c6275 <__mingw_TLScallback+0x35>
-    646c625a:	mov    0x68a8(%rip),%eax        # 646ccb08 <__mingwthr_cs_init>
-    646c6260:	test   %eax,%eax
-    646c6262:	je     646c6275 <__mingw_TLScallback+0x35>
-    646c6264:	call   646c60b0 <__mingwthr_run_key_dtors.part.0>
-    646c6269:	jmp    646c6275 <__mingw_TLScallback+0x35>
-    646c626b:	nopl   0x0(%rax,%rax,1)
-    646c6270:	call   646c6700 <_fpreset>
-    646c6275:	mov    $0x1,%eax
-    646c627a:	add    $0x20,%rsp
-    646c627e:	pop    %rbx
-    646c627f:	ret
-    646c6280:	mov    0x6882(%rip),%eax        # 646ccb08 <__mingwthr_cs_init>
-    646c6286:	test   %eax,%eax
-    646c6288:	jne    646c6310 <__mingw_TLScallback+0xd0>
-    646c628e:	mov    0x6874(%rip),%eax        # 646ccb08 <__mingwthr_cs_init>
-    646c6294:	cmp    $0x1,%eax
-    646c6297:	jne    646c6275 <__mingw_TLScallback+0x35>
-    646c6299:	mov    0x6860(%rip),%rcx        # 646ccb00 <key_dtor_list>
-    646c62a0:	test   %rcx,%rcx
-    646c62a3:	je     646c62b6 <__mingw_TLScallback+0x76>
-    646c62a5:	mov    0x10(%rcx),%rbx
-    646c62a9:	call   646c78f8 <free>
-    646c62ae:	test   %rbx,%rbx
-    646c62b1:	mov    %rbx,%rcx
-    646c62b4:	jne    646c62a5 <__mingw_TLScallback+0x65>
-    646c62b6:	lea    0x6863(%rip),%rcx        # 646ccb20 <__mingwthr_cs>
-    646c62bd:	movq   $0x0,0x6838(%rip)        # 646ccb00 <key_dtor_list>
-    646c62c8:	movl   $0x0,0x6836(%rip)        # 646ccb08 <__mingwthr_cs_init>
-    646c62d2:	call   *0x7ef4(%rip)        # 646ce1cc <__IAT_start__>
-    646c62d8:	jmp    646c6275 <__mingw_TLScallback+0x35>
-    646c62da:	nopw   0x0(%rax,%rax,1)
-    646c62e0:	mov    0x6822(%rip),%eax        # 646ccb08 <__mingwthr_cs_init>
-    646c62e6:	test   %eax,%eax
-    646c62e8:	je     646c6300 <__mingw_TLScallback+0xc0>
-    646c62ea:	movl   $0x1,0x6814(%rip)        # 646ccb08 <__mingwthr_cs_init>
-    646c62f4:	mov    $0x1,%eax
-    646c62f9:	add    $0x20,%rsp
-    646c62fd:	pop    %rbx
-    646c62fe:	ret
-    646c62ff:	nop
-    646c6300:	lea    0x6819(%rip),%rcx        # 646ccb20 <__mingwthr_cs>
-    646c6307:	call   *0x7eff(%rip)        # 646ce20c <__imp_InitializeCriticalSection>
-    646c630d:	jmp    646c62ea <__mingw_TLScallback+0xaa>
-    646c630f:	nop
-    646c6310:	call   646c60b0 <__mingwthr_run_key_dtors.part.0>
-    646c6315:	jmp    646c628e <__mingw_TLScallback+0x4e>
-    646c631a:	nop
-    646c631b:	nop
-    646c631c:	nop
-    646c631d:	nop
-    646c631e:	nop
-    646c631f:	nop
-
-00000000646c6320 <_ValidateImageBase.part.0>:
-    646c6320:	movslq 0x3c(%rcx),%rax
-    646c6324:	add    %rax,%rcx
-    646c6327:	xor    %eax,%eax
-    646c6329:	cmpl   $0x4550,(%rcx)
-    646c632f:	je     646c6332 <_ValidateImageBase.part.0+0x12>
-    646c6331:	ret
-    646c6332:	xor    %eax,%eax
-    646c6334:	cmpw   $0x20b,0x18(%rcx)
-    646c633a:	sete   %al
-    646c633d:	ret
-    646c633e:	xchg   %ax,%ax
-
-00000000646c6340 <_ValidateImageBase>:
-    646c6340:	cmpw   $0x5a4d,(%rcx)
-    646c6345:	je     646c6350 <_ValidateImageBase+0x10>
-    646c6347:	xor    %eax,%eax
-    646c6349:	ret
-    646c634a:	nopw   0x0(%rax,%rax,1)
-    646c6350:	jmp    646c6320 <_ValidateImageBase.part.0>
-    646c6352:	nopl   0x0(%rax)
-    646c6356:	cs nopw 0x0(%rax,%rax,1)
-
-00000000646c6360 <_FindPESection>:
-    646c6360:	movslq 0x3c(%rcx),%rax
-    646c6364:	add    %rax,%rcx
-    646c6367:	movzwl 0x14(%rcx),%eax
-    646c636b:	lea    0x18(%rcx,%rax,1),%rax
-    646c6370:	movzwl 0x6(%rcx),%ecx
-    646c6374:	test   %ecx,%ecx
-    646c6376:	je     646c63a1 <_FindPESection+0x41>
-    646c6378:	sub    $0x1,%ecx
-    646c637b:	lea    (%rcx,%rcx,4),%rcx
-    646c637f:	lea    0x28(%rax,%rcx,8),%r9
-    646c6384:	mov    0xc(%rax),%r8d
-    646c6388:	cmp    %rdx,%r8
-    646c638b:	mov    %r8,%rcx
-    646c638e:	ja     646c6398 <_FindPESection+0x38>
-    646c6390:	add    0x8(%rax),%ecx
-    646c6393:	cmp    %rdx,%rcx
-    646c6396:	ja     646c63a3 <_FindPESection+0x43>
-    646c6398:	add    $0x28,%rax
-    646c639c:	cmp    %r9,%rax
-    646c639f:	jne    646c6384 <_FindPESection+0x24>
-    646c63a1:	xor    %eax,%eax
-    646c63a3:	ret
-    646c63a4:	xchg   %ax,%ax
-    646c63a6:	cs nopw 0x0(%rax,%rax,1)
-
-00000000646c63b0 <_FindPESectionByName>:
-    646c63b0:	push   %rdi
-    646c63b1:	push   %rsi
-    646c63b2:	push   %rbx
-    646c63b3:	sub    $0x20,%rsp
-    646c63b7:	mov    %rcx,%rsi
-    646c63ba:	call   646c78c0 <strlen>
-    646c63bf:	cmp    $0x8,%rax
-    646c63c3:	ja     646c6430 <_FindPESectionByName+0x80>
-    646c63c5:	mov    0x3264(%rip),%rdx        # 646c9630 <.refptr.__image_base__>
-    646c63cc:	cmpw   $0x5a4d,(%rdx)
-    646c63d1:	jne    646c6430 <_FindPESectionByName+0x80>
-    646c63d3:	mov    %rdx,%rcx
-    646c63d6:	call   646c6320 <_ValidateImageBase.part.0>
-    646c63db:	test   %eax,%eax
-    646c63dd:	je     646c6430 <_FindPESectionByName+0x80>
-    646c63df:	movslq 0x3c(%rdx),%rcx
-    646c63e3:	add    %rdx,%rcx
-    646c63e6:	movzwl 0x14(%rcx),%eax
-    646c63ea:	lea    0x18(%rcx,%rax,1),%rbx
-    646c63ef:	movzwl 0x6(%rcx),%eax
-    646c63f3:	test   %eax,%eax
-    646c63f5:	je     646c6430 <_FindPESectionByName+0x80>
-    646c63f7:	sub    $0x1,%eax
-    646c63fa:	lea    (%rax,%rax,4),%rax
-    646c63fe:	lea    0x28(%rbx,%rax,8),%rdi
-    646c6403:	jmp    646c640e <_FindPESectionByName+0x5e>
-    646c6405:	add    $0x28,%rbx
-    646c6409:	cmp    %rdi,%rbx
-    646c640c:	je     646c6430 <_FindPESectionByName+0x80>
-    646c640e:	mov    $0x8,%r8d
-    646c6414:	mov    %rsi,%rdx
-    646c6417:	mov    %rbx,%rcx
-    646c641a:	call   646c78b8 <strncmp>
-    646c641f:	test   %eax,%eax
-    646c6421:	jne    646c6405 <_FindPESectionByName+0x55>
-    646c6423:	mov    %rbx,%rax
-    646c6426:	add    $0x20,%rsp
-    646c642a:	pop    %rbx
-    646c642b:	pop    %rsi
-    646c642c:	pop    %rdi
-    646c642d:	ret
-    646c642e:	xchg   %ax,%ax
-    646c6430:	xor    %ebx,%ebx
-    646c6432:	mov    %rbx,%rax
-    646c6435:	add    $0x20,%rsp
-    646c6439:	pop    %rbx
-    646c643a:	pop    %rsi
-    646c643b:	pop    %rdi
-    646c643c:	ret
-    646c643d:	nopl   (%rax)
-
-00000000646c6440 <__mingw_GetSectionForAddress>:
-    646c6440:	sub    $0x28,%rsp
-    646c6444:	mov    0x31e5(%rip),%r8        # 646c9630 <.refptr.__image_base__>
-    646c644b:	cmpw   $0x5a4d,(%r8)
-    646c6451:	mov    %rcx,%rdx
-    646c6454:	jne    646c64ad <__mingw_GetSectionForAddress+0x6d>
-    646c6456:	mov    %r8,%rcx
-    646c6459:	call   646c6320 <_ValidateImageBase.part.0>
-    646c645e:	test   %eax,%eax
-    646c6460:	je     646c64ad <__mingw_GetSectionForAddress+0x6d>
-    646c6462:	movslq 0x3c(%r8),%rax
-    646c6466:	mov    %rdx,%rcx
-    646c6469:	sub    %r8,%rcx
-    646c646c:	add    %rax,%r8
-    646c646f:	movzwl 0x6(%r8),%edx
-    646c6474:	movzwl 0x14(%r8),%eax
-    646c6479:	test   %edx,%edx
-    646c647b:	lea    0x18(%r8,%rax,1),%rax
-    646c6480:	je     646c64ad <__mingw_GetSectionForAddress+0x6d>
-    646c6482:	sub    $0x1,%edx
-    646c6485:	lea    (%rdx,%rdx,4),%rdx
-    646c6489:	lea    0x28(%rax,%rdx,8),%r9
-    646c648e:	xchg   %ax,%ax
-    646c6490:	mov    0xc(%rax),%r8d
-    646c6494:	cmp    %r8,%rcx
-    646c6497:	mov    %r8,%rdx
-    646c649a:	jb     646c64a4 <__mingw_GetSectionForAddress+0x64>
-    646c649c:	add    0x8(%rax),%edx
-    646c649f:	cmp    %rdx,%rcx
-    646c64a2:	jb     646c64af <__mingw_GetSectionForAddress+0x6f>
-    646c64a4:	add    $0x28,%rax
-    646c64a8:	cmp    %r9,%rax
-    646c64ab:	jne    646c6490 <__mingw_GetSectionForAddress+0x50>
-    646c64ad:	xor    %eax,%eax
-    646c64af:	add    $0x28,%rsp
-    646c64b3:	ret
-    646c64b4:	xchg   %ax,%ax
-    646c64b6:	cs nopw 0x0(%rax,%rax,1)
-
-00000000646c64c0 <__mingw_GetSectionCount>:
-    646c64c0:	sub    $0x28,%rsp
-    646c64c4:	mov    0x3165(%rip),%rdx        # 646c9630 <.refptr.__image_base__>
-    646c64cb:	xor    %r8d,%r8d
-    646c64ce:	cmpw   $0x5a4d,(%rdx)
-    646c64d3:	je     646c64e0 <__mingw_GetSectionCount+0x20>
-    646c64d5:	mov    %r8d,%eax
-    646c64d8:	add    $0x28,%rsp
-    646c64dc:	ret
-    646c64dd:	nopl   (%rax)
-    646c64e0:	mov    %rdx,%rcx
-    646c64e3:	call   646c6320 <_ValidateImageBase.part.0>
-    646c64e8:	test   %eax,%eax
-    646c64ea:	je     646c64d5 <__mingw_GetSectionCount+0x15>
-    646c64ec:	movslq 0x3c(%rdx),%rax
-    646c64f0:	movzwl 0x6(%rax,%rdx,1),%r8d
-    646c64f6:	mov    %r8d,%eax
-    646c64f9:	add    $0x28,%rsp
-    646c64fd:	ret
-    646c64fe:	xchg   %ax,%ax
-
-00000000646c6500 <_FindPESectionExec>:
-    646c6500:	sub    $0x28,%rsp
-    646c6504:	mov    0x3125(%rip),%r8        # 646c9630 <.refptr.__image_base__>
-    646c650b:	cmpw   $0x5a4d,(%r8)
-    646c6511:	mov    %rcx,%rdx
-    646c6514:	jne    646c6568 <_FindPESectionExec+0x68>
-    646c6516:	mov    %r8,%rcx
-    646c6519:	call   646c6320 <_ValidateImageBase.part.0>
-    646c651e:	test   %eax,%eax
-    646c6520:	je     646c6568 <_FindPESectionExec+0x68>
-    646c6522:	movslq 0x3c(%r8),%rcx
-    646c6526:	add    %r8,%rcx
-    646c6529:	movzwl 0x14(%rcx),%eax
-    646c652d:	lea    0x18(%rcx,%rax,1),%rax
-    646c6532:	movzwl 0x6(%rcx),%ecx
-    646c6536:	test   %ecx,%ecx
-    646c6538:	je     646c6568 <_FindPESectionExec+0x68>
-    646c653a:	sub    $0x1,%ecx
-    646c653d:	lea    (%rcx,%rcx,4),%rcx
-    646c6541:	lea    0x28(%rax,%rcx,8),%rcx
+
+00000000646c5f50 <_gnu_exception_handler>:
+    646c5f50:	push   %rbx
+    646c5f51:	sub    $0x20,%rsp
+    646c5f55:	mov    (%rcx),%rdx
+    646c5f58:	mov    (%rdx),%eax
+    646c5f5a:	mov    %rcx,%rbx
+    646c5f5d:	mov    %eax,%ecx
+    646c5f5f:	and    $0x20ffffff,%ecx
+    646c5f65:	cmp    $0x20474343,%ecx
+    646c5f6b:	je     646c6030 <_gnu_exception_handler+0xe0>
+    646c5f71:	cmp    $0xc0000091,%eax
+    646c5f76:	ja     646c5fe0 <_gnu_exception_handler+0x90>
+    646c5f78:	cmp    $0xc000008d,%eax
+    646c5f7d:	jae    646c5ffb <_gnu_exception_handler+0xab>
+    646c5f7f:	cmp    $0xc0000008,%eax
+    646c5f84:	je     646c603a <_gnu_exception_handler+0xea>
+    646c5f8a:	ja     646c6084 <_gnu_exception_handler+0x134>
+    646c5f90:	cmp    $0x80000002,%eax
+    646c5f95:	je     646c603a <_gnu_exception_handler+0xea>
+    646c5f9b:	cmp    $0xc0000005,%eax
+    646c5fa0:	jne    646c5fc1 <_gnu_exception_handler+0x71>
+    646c5fa2:	xor    %edx,%edx
+    646c5fa4:	mov    $0xb,%ecx
+    646c5fa9:	call   646c7958 <signal>
+    646c5fae:	cmp    $0x1,%rax
+    646c5fb2:	je     646c6109 <_gnu_exception_handler+0x1b9>
+    646c5fb8:	test   %rax,%rax
+    646c5fbb:	jne    646c60d0 <_gnu_exception_handler+0x180>
+    646c5fc1:	mov    0x6898(%rip),%rax        # 646cc860 <__mingw_oldexcpt_handler>
+    646c5fc8:	test   %rax,%rax
+    646c5fcb:	je     646c60e1 <_gnu_exception_handler+0x191>
+    646c5fd1:	mov    %rbx,%rcx
+    646c5fd4:	add    $0x20,%rsp
+    646c5fd8:	pop    %rbx
+    646c5fd9:	rex.W jmp *%rax
+    646c5fdc:	nopl   0x0(%rax)
+    646c5fe0:	cmp    $0xc0000094,%eax
+    646c5fe5:	je     646c60a0 <_gnu_exception_handler+0x150>
+    646c5feb:	ja     646c6045 <_gnu_exception_handler+0xf5>
+    646c5fed:	cmp    $0xc0000092,%eax
+    646c5ff2:	je     646c603a <_gnu_exception_handler+0xea>
+    646c5ff4:	cmp    $0xc0000093,%eax
+    646c5ff9:	jne    646c5fc1 <_gnu_exception_handler+0x71>
+    646c5ffb:	xor    %edx,%edx
+    646c5ffd:	mov    $0x8,%ecx
+    646c6002:	call   646c7958 <signal>
+    646c6007:	cmp    $0x1,%rax
+    646c600b:	je     646c60f0 <_gnu_exception_handler+0x1a0>
+    646c6011:	test   %rax,%rax
+    646c6014:	je     646c5fc1 <_gnu_exception_handler+0x71>
+    646c6016:	mov    $0x8,%ecx
+    646c601b:	call   *%rax
+    646c601d:	mov    $0xffffffff,%eax
+    646c6022:	add    $0x20,%rsp
+    646c6026:	pop    %rbx
+    646c6027:	ret
+    646c6028:	nopl   0x0(%rax,%rax,1)
+    646c6030:	testb  $0x1,0x4(%rdx)
+    646c6034:	jne    646c5f71 <_gnu_exception_handler+0x21>
+    646c603a:	mov    $0xffffffff,%eax
+    646c603f:	add    $0x20,%rsp
+    646c6043:	pop    %rbx
+    646c6044:	ret
+    646c6045:	cmp    $0xc0000095,%eax
+    646c604a:	je     646c603a <_gnu_exception_handler+0xea>
+    646c604c:	cmp    $0xc0000096,%eax
+    646c6051:	jne    646c5fc1 <_gnu_exception_handler+0x71>
+    646c6057:	xor    %edx,%edx
+    646c6059:	mov    $0x4,%ecx
+    646c605e:	call   646c7958 <signal>
+    646c6063:	cmp    $0x1,%rax
+    646c6067:	je     646c6120 <_gnu_exception_handler+0x1d0>
+    646c606d:	test   %rax,%rax
+    646c6070:	je     646c5fc1 <_gnu_exception_handler+0x71>
+    646c6076:	mov    $0x4,%ecx
+    646c607b:	call   *%rax
+    646c607d:	mov    $0xffffffff,%eax
+    646c6082:	jmp    646c6022 <_gnu_exception_handler+0xd2>
+    646c6084:	cmp    $0xc000001d,%eax
+    646c6089:	je     646c6057 <_gnu_exception_handler+0x107>
+    646c608b:	cmp    $0xc000008c,%eax
+    646c6090:	jne    646c5fc1 <_gnu_exception_handler+0x71>
+    646c6096:	jmp    646c603a <_gnu_exception_handler+0xea>
+    646c6098:	nopl   0x0(%rax,%rax,1)
+    646c60a0:	xor    %edx,%edx
+    646c60a2:	mov    $0x8,%ecx
+    646c60a7:	call   646c7958 <signal>
+    646c60ac:	cmp    $0x1,%rax
+    646c60b0:	jne    646c6011 <_gnu_exception_handler+0xc1>
+    646c60b6:	mov    $0x1,%edx
+    646c60bb:	mov    $0x8,%ecx
+    646c60c0:	call   646c7958 <signal>
+    646c60c5:	mov    $0xffffffff,%eax
+    646c60ca:	jmp    646c6022 <_gnu_exception_handler+0xd2>
+    646c60cf:	nop
+    646c60d0:	mov    $0xb,%ecx
+    646c60d5:	call   *%rax
+    646c60d7:	mov    $0xffffffff,%eax
+    646c60dc:	jmp    646c6022 <_gnu_exception_handler+0xd2>
+    646c60e1:	xor    %eax,%eax
+    646c60e3:	jmp    646c6022 <_gnu_exception_handler+0xd2>
+    646c60e8:	nopl   0x0(%rax,%rax,1)
+    646c60f0:	mov    $0x1,%edx
+    646c60f5:	mov    $0x8,%ecx
+    646c60fa:	call   646c7958 <signal>
+    646c60ff:	call   646c6790 <_fpreset>
+    646c6104:	jmp    646c603a <_gnu_exception_handler+0xea>
+    646c6109:	mov    $0x1,%edx
+    646c610e:	mov    $0xb,%ecx
+    646c6113:	call   646c7958 <signal>
+    646c6118:	or     $0xffffffff,%eax
+    646c611b:	jmp    646c6022 <_gnu_exception_handler+0xd2>
+    646c6120:	mov    $0x1,%edx
+    646c6125:	mov    $0x4,%ecx
+    646c612a:	call   646c7958 <signal>
+    646c612f:	or     $0xffffffff,%eax
+    646c6132:	jmp    646c6022 <_gnu_exception_handler+0xd2>
+    646c6137:	nop
+    646c6138:	nop
+    646c6139:	nop
+    646c613a:	nop
+    646c613b:	nop
+    646c613c:	nop
+    646c613d:	nop
+    646c613e:	nop
+    646c613f:	nop
+
+00000000646c6140 <__mingwthr_run_key_dtors.part.0>:
+    646c6140:	push   %rbp
+    646c6141:	push   %rdi
+    646c6142:	push   %rsi
+    646c6143:	push   %rbx
+    646c6144:	sub    $0x28,%rsp
+    646c6148:	lea    0x69d1(%rip),%rcx        # 646ccb20 <__mingwthr_cs>
+    646c614f:	call   *0x807f(%rip)        # 646ce1d4 <__imp_EnterCriticalSection>
+    646c6155:	mov    0x69a4(%rip),%rbx        # 646ccb00 <key_dtor_list>
+    646c615c:	test   %rbx,%rbx
+    646c615f:	je     646c6194 <__mingwthr_run_key_dtors.part.0+0x54>
+    646c6161:	mov    0x80f4(%rip),%rbp        # 646ce25c <__imp_TlsGetValue>
+    646c6168:	mov    0x8085(%rip),%rdi        # 646ce1f4 <__imp_GetLastError>
+    646c616f:	nop
+    646c6170:	mov    (%rbx),%ecx
+    646c6172:	call   *%rbp
+    646c6174:	mov    %rax,%rsi
+    646c6177:	call   *%rdi
+    646c6179:	test   %eax,%eax
+    646c617b:	jne    646c618b <__mingwthr_run_key_dtors.part.0+0x4b>
+    646c617d:	test   %rsi,%rsi
+    646c6180:	je     646c618b <__mingwthr_run_key_dtors.part.0+0x4b>
+    646c6182:	mov    0x8(%rbx),%rax
+    646c6186:	mov    %rsi,%rcx
+    646c6189:	call   *%rax
+    646c618b:	mov    0x10(%rbx),%rbx
+    646c618f:	test   %rbx,%rbx
+    646c6192:	jne    646c6170 <__mingwthr_run_key_dtors.part.0+0x30>
+    646c6194:	lea    0x6985(%rip),%rcx        # 646ccb20 <__mingwthr_cs>
+    646c619b:	add    $0x28,%rsp
+    646c619f:	pop    %rbx
+    646c61a0:	pop    %rsi
+    646c61a1:	pop    %rdi
+    646c61a2:	pop    %rbp
+    646c61a3:	rex.W jmp *0x806a(%rip)        # 646ce214 <__imp_LeaveCriticalSection>
+    646c61aa:	nopw   0x0(%rax,%rax,1)
+
+00000000646c61b0 <___w64_mingwthr_add_key_dtor>:
+    646c61b0:	push   %rbp
+    646c61b1:	push   %rdi
+    646c61b2:	push   %rsi
+    646c61b3:	push   %rbx
+    646c61b4:	sub    $0x28,%rsp
+    646c61b8:	mov    0x694a(%rip),%eax        # 646ccb08 <__mingwthr_cs_init>
+    646c61be:	xor    %esi,%esi
+    646c61c0:	test   %eax,%eax
+    646c61c2:	mov    %ecx,%ebp
+    646c61c4:	mov    %rdx,%rdi
+    646c61c7:	jne    646c61d4 <___w64_mingwthr_add_key_dtor+0x24>
+    646c61c9:	mov    %esi,%eax
+    646c61cb:	add    $0x28,%rsp
+    646c61cf:	pop    %rbx
+    646c61d0:	pop    %rsi
+    646c61d1:	pop    %rdi
+    646c61d2:	pop    %rbp
+    646c61d3:	ret
+    646c61d4:	mov    $0x18,%edx
+    646c61d9:	mov    $0x1,%ecx
+    646c61de:	call   646c79b0 <calloc>
+    646c61e3:	test   %rax,%rax
+    646c61e6:	mov    %rax,%rbx
+    646c61e9:	je     646c6228 <___w64_mingwthr_add_key_dtor+0x78>
+    646c61eb:	mov    %ebp,(%rax)
+    646c61ed:	lea    0x692c(%rip),%rcx        # 646ccb20 <__mingwthr_cs>
+    646c61f4:	mov    %rdi,0x8(%rax)
+    646c61f8:	call   *0x7fd6(%rip)        # 646ce1d4 <__imp_EnterCriticalSection>
+    646c61fe:	mov    0x68fb(%rip),%rax        # 646ccb00 <key_dtor_list>
+    646c6205:	lea    0x6914(%rip),%rcx        # 646ccb20 <__mingwthr_cs>
+    646c620c:	mov    %rbx,0x68ed(%rip)        # 646ccb00 <key_dtor_list>
+    646c6213:	mov    %rax,0x10(%rbx)
+    646c6217:	call   *0x7ff7(%rip)        # 646ce214 <__imp_LeaveCriticalSection>
+    646c621d:	mov    %esi,%eax
+    646c621f:	add    $0x28,%rsp
+    646c6223:	pop    %rbx
+    646c6224:	pop    %rsi
+    646c6225:	pop    %rdi
+    646c6226:	pop    %rbp
+    646c6227:	ret
+    646c6228:	mov    $0xffffffff,%esi
+    646c622d:	jmp    646c61c9 <___w64_mingwthr_add_key_dtor+0x19>
+    646c622f:	nop
+
+00000000646c6230 <___w64_mingwthr_remove_key_dtor>:
+    646c6230:	push   %rbx
+    646c6231:	sub    $0x20,%rsp
+    646c6235:	mov    0x68cd(%rip),%eax        # 646ccb08 <__mingwthr_cs_init>
+    646c623b:	test   %eax,%eax
+    646c623d:	mov    %ecx,%ebx
+    646c623f:	jne    646c6250 <___w64_mingwthr_remove_key_dtor+0x20>
+    646c6241:	xor    %eax,%eax
+    646c6243:	add    $0x20,%rsp
+    646c6247:	pop    %rbx
+    646c6248:	ret
+    646c6249:	nopl   0x0(%rax)
+    646c6250:	lea    0x68c9(%rip),%rcx        # 646ccb20 <__mingwthr_cs>
+    646c6257:	call   *0x7f77(%rip)        # 646ce1d4 <__imp_EnterCriticalSection>
+    646c625d:	mov    0x689c(%rip),%rax        # 646ccb00 <key_dtor_list>
+    646c6264:	test   %rax,%rax
+    646c6267:	je     646c6283 <___w64_mingwthr_remove_key_dtor+0x53>
+    646c6269:	mov    (%rax),%edx
+    646c626b:	cmp    %edx,%ebx
+    646c626d:	jne    646c627a <___w64_mingwthr_remove_key_dtor+0x4a>
+    646c626f:	jmp    646c62c0 <___w64_mingwthr_remove_key_dtor+0x90>
+    646c6271:	mov    (%rcx),%edx
+    646c6273:	cmp    %ebx,%edx
+    646c6275:	je     646c62a0 <___w64_mingwthr_remove_key_dtor+0x70>
+    646c6277:	mov    %rcx,%rax
+    646c627a:	mov    0x10(%rax),%rcx
+    646c627e:	test   %rcx,%rcx
+    646c6281:	jne    646c6271 <___w64_mingwthr_remove_key_dtor+0x41>
+    646c6283:	lea    0x6896(%rip),%rcx        # 646ccb20 <__mingwthr_cs>
+    646c628a:	call   *0x7f84(%rip)        # 646ce214 <__imp_LeaveCriticalSection>
+    646c6290:	xor    %eax,%eax
+    646c6292:	add    $0x20,%rsp
+    646c6296:	pop    %rbx
+    646c6297:	ret
+    646c6298:	nopl   0x0(%rax,%rax,1)
+    646c62a0:	mov    0x10(%rcx),%rdx
+    646c62a4:	mov    %rdx,0x10(%rax)
+    646c62a8:	call   646c7988 <free>
+    646c62ad:	lea    0x686c(%rip),%rcx        # 646ccb20 <__mingwthr_cs>
+    646c62b4:	call   *0x7f5a(%rip)        # 646ce214 <__imp_LeaveCriticalSection>
+    646c62ba:	jmp    646c6290 <___w64_mingwthr_remove_key_dtor+0x60>
+    646c62bc:	nopl   0x0(%rax)
+    646c62c0:	mov    0x10(%rax),%rdx
+    646c62c4:	mov    %rax,%rcx
+    646c62c7:	mov    %rdx,0x6832(%rip)        # 646ccb00 <key_dtor_list>
+    646c62ce:	jmp    646c62a8 <___w64_mingwthr_remove_key_dtor+0x78>
+
+00000000646c62d0 <__mingw_TLScallback>:
+    646c62d0:	push   %rbx
+    646c62d1:	sub    $0x20,%rsp
+    646c62d5:	cmp    $0x1,%edx
+    646c62d8:	je     646c6370 <__mingw_TLScallback+0xa0>
+    646c62de:	jb     646c6310 <__mingw_TLScallback+0x40>
+    646c62e0:	cmp    $0x2,%edx
+    646c62e3:	je     646c6300 <__mingw_TLScallback+0x30>
+    646c62e5:	cmp    $0x3,%edx
+    646c62e8:	jne    646c6305 <__mingw_TLScallback+0x35>
+    646c62ea:	mov    0x6818(%rip),%eax        # 646ccb08 <__mingwthr_cs_init>
+    646c62f0:	test   %eax,%eax
+    646c62f2:	je     646c6305 <__mingw_TLScallback+0x35>
+    646c62f4:	call   646c6140 <__mingwthr_run_key_dtors.part.0>
+    646c62f9:	jmp    646c6305 <__mingw_TLScallback+0x35>
+    646c62fb:	nopl   0x0(%rax,%rax,1)
+    646c6300:	call   646c6790 <_fpreset>
+    646c6305:	mov    $0x1,%eax
+    646c630a:	add    $0x20,%rsp
+    646c630e:	pop    %rbx
+    646c630f:	ret
+    646c6310:	mov    0x67f2(%rip),%eax        # 646ccb08 <__mingwthr_cs_init>
+    646c6316:	test   %eax,%eax
+    646c6318:	jne    646c63a0 <__mingw_TLScallback+0xd0>
+    646c631e:	mov    0x67e4(%rip),%eax        # 646ccb08 <__mingwthr_cs_init>
+    646c6324:	cmp    $0x1,%eax
+    646c6327:	jne    646c6305 <__mingw_TLScallback+0x35>
+    646c6329:	mov    0x67d0(%rip),%rcx        # 646ccb00 <key_dtor_list>
+    646c6330:	test   %rcx,%rcx
+    646c6333:	je     646c6346 <__mingw_TLScallback+0x76>
+    646c6335:	mov    0x10(%rcx),%rbx
+    646c6339:	call   646c7988 <free>
+    646c633e:	test   %rbx,%rbx
+    646c6341:	mov    %rbx,%rcx
+    646c6344:	jne    646c6335 <__mingw_TLScallback+0x65>
+    646c6346:	lea    0x67d3(%rip),%rcx        # 646ccb20 <__mingwthr_cs>
+    646c634d:	movq   $0x0,0x67a8(%rip)        # 646ccb00 <key_dtor_list>
+    646c6358:	movl   $0x0,0x67a6(%rip)        # 646ccb08 <__mingwthr_cs_init>
+    646c6362:	call   *0x7e64(%rip)        # 646ce1cc <__IAT_start__>
+    646c6368:	jmp    646c6305 <__mingw_TLScallback+0x35>
+    646c636a:	nopw   0x0(%rax,%rax,1)
+    646c6370:	mov    0x6792(%rip),%eax        # 646ccb08 <__mingwthr_cs_init>
+    646c6376:	test   %eax,%eax
+    646c6378:	je     646c6390 <__mingw_TLScallback+0xc0>
+    646c637a:	movl   $0x1,0x6784(%rip)        # 646ccb08 <__mingwthr_cs_init>
+    646c6384:	mov    $0x1,%eax
+    646c6389:	add    $0x20,%rsp
+    646c638d:	pop    %rbx
+    646c638e:	ret
+    646c638f:	nop
+    646c6390:	lea    0x6789(%rip),%rcx        # 646ccb20 <__mingwthr_cs>
+    646c6397:	call   *0x7e6f(%rip)        # 646ce20c <__imp_InitializeCriticalSection>
+    646c639d:	jmp    646c637a <__mingw_TLScallback+0xaa>
+    646c639f:	nop
+    646c63a0:	call   646c6140 <__mingwthr_run_key_dtors.part.0>
+    646c63a5:	jmp    646c631e <__mingw_TLScallback+0x4e>
+    646c63aa:	nop
+    646c63ab:	nop
+    646c63ac:	nop
+    646c63ad:	nop
+    646c63ae:	nop
+    646c63af:	nop
+
+00000000646c63b0 <_ValidateImageBase.part.0>:
+    646c63b0:	movslq 0x3c(%rcx),%rax
+    646c63b4:	add    %rax,%rcx
+    646c63b7:	xor    %eax,%eax
+    646c63b9:	cmpl   $0x4550,(%rcx)
+    646c63bf:	je     646c63c2 <_ValidateImageBase.part.0+0x12>
+    646c63c1:	ret
+    646c63c2:	xor    %eax,%eax
+    646c63c4:	cmpw   $0x20b,0x18(%rcx)
+    646c63ca:	sete   %al
+    646c63cd:	ret
+    646c63ce:	xchg   %ax,%ax
+
+00000000646c63d0 <_ValidateImageBase>:
+    646c63d0:	cmpw   $0x5a4d,(%rcx)
+    646c63d5:	je     646c63e0 <_ValidateImageBase+0x10>
+    646c63d7:	xor    %eax,%eax
+    646c63d9:	ret
+    646c63da:	nopw   0x0(%rax,%rax,1)
+    646c63e0:	jmp    646c63b0 <_ValidateImageBase.part.0>
+    646c63e2:	nopl   0x0(%rax)
+    646c63e6:	cs nopw 0x0(%rax,%rax,1)
+
+00000000646c63f0 <_FindPESection>:
+    646c63f0:	movslq 0x3c(%rcx),%rax
+    646c63f4:	add    %rax,%rcx
+    646c63f7:	movzwl 0x14(%rcx),%eax
+    646c63fb:	lea    0x18(%rcx,%rax,1),%rax
+    646c6400:	movzwl 0x6(%rcx),%ecx
+    646c6404:	test   %ecx,%ecx
+    646c6406:	je     646c6431 <_FindPESection+0x41>
+    646c6408:	sub    $0x1,%ecx
+    646c640b:	lea    (%rcx,%rcx,4),%rcx
+    646c640f:	lea    0x28(%rax,%rcx,8),%r9
+    646c6414:	mov    0xc(%rax),%r8d
+    646c6418:	cmp    %rdx,%r8
+    646c641b:	mov    %r8,%rcx
+    646c641e:	ja     646c6428 <_FindPESection+0x38>
+    646c6420:	add    0x8(%rax),%ecx
+    646c6423:	cmp    %rdx,%rcx
+    646c6426:	ja     646c6433 <_FindPESection+0x43>
+    646c6428:	add    $0x28,%rax
+    646c642c:	cmp    %r9,%rax
+    646c642f:	jne    646c6414 <_FindPESection+0x24>
+    646c6431:	xor    %eax,%eax
+    646c6433:	ret
+    646c6434:	xchg   %ax,%ax
+    646c6436:	cs nopw 0x0(%rax,%rax,1)
+
+00000000646c6440 <_FindPESectionByName>:
+    646c6440:	push   %rdi
+    646c6441:	push   %rsi
+    646c6442:	push   %rbx
+    646c6443:	sub    $0x20,%rsp
+    646c6447:	mov    %rcx,%rsi
+    646c644a:	call   646c7950 <strlen>
+    646c644f:	cmp    $0x8,%rax
+    646c6453:	ja     646c64c0 <_FindPESectionByName+0x80>
+    646c6455:	mov    0x31d4(%rip),%rdx        # 646c9630 <.refptr.__image_base__>
+    646c645c:	cmpw   $0x5a4d,(%rdx)
+    646c6461:	jne    646c64c0 <_FindPESectionByName+0x80>
+    646c6463:	mov    %rdx,%rcx
+    646c6466:	call   646c63b0 <_ValidateImageBase.part.0>
+    646c646b:	test   %eax,%eax
+    646c646d:	je     646c64c0 <_FindPESectionByName+0x80>
+    646c646f:	movslq 0x3c(%rdx),%rcx
+    646c6473:	add    %rdx,%rcx
+    646c6476:	movzwl 0x14(%rcx),%eax
+    646c647a:	lea    0x18(%rcx,%rax,1),%rbx
+    646c647f:	movzwl 0x6(%rcx),%eax
+    646c6483:	test   %eax,%eax
+    646c6485:	je     646c64c0 <_FindPESectionByName+0x80>
+    646c6487:	sub    $0x1,%eax
+    646c648a:	lea    (%rax,%rax,4),%rax
+    646c648e:	lea    0x28(%rbx,%rax,8),%rdi
+    646c6493:	jmp    646c649e <_FindPESectionByName+0x5e>
+    646c6495:	add    $0x28,%rbx
+    646c6499:	cmp    %rdi,%rbx
+    646c649c:	je     646c64c0 <_FindPESectionByName+0x80>
+    646c649e:	mov    $0x8,%r8d
+    646c64a4:	mov    %rsi,%rdx
+    646c64a7:	mov    %rbx,%rcx
+    646c64aa:	call   646c7948 <strncmp>
+    646c64af:	test   %eax,%eax
+    646c64b1:	jne    646c6495 <_FindPESectionByName+0x55>
+    646c64b3:	mov    %rbx,%rax
+    646c64b6:	add    $0x20,%rsp
+    646c64ba:	pop    %rbx
+    646c64bb:	pop    %rsi
+    646c64bc:	pop    %rdi
+    646c64bd:	ret
+    646c64be:	xchg   %ax,%ax
+    646c64c0:	xor    %ebx,%ebx
+    646c64c2:	mov    %rbx,%rax
+    646c64c5:	add    $0x20,%rsp
+    646c64c9:	pop    %rbx
+    646c64ca:	pop    %rsi
+    646c64cb:	pop    %rdi
+    646c64cc:	ret
+    646c64cd:	nopl   (%rax)
+
+00000000646c64d0 <__mingw_GetSectionForAddress>:
+    646c64d0:	sub    $0x28,%rsp
+    646c64d4:	mov    0x3155(%rip),%r8        # 646c9630 <.refptr.__image_base__>
+    646c64db:	cmpw   $0x5a4d,(%r8)
+    646c64e1:	mov    %rcx,%rdx
+    646c64e4:	jne    646c653d <__mingw_GetSectionForAddress+0x6d>
+    646c64e6:	mov    %r8,%rcx
+    646c64e9:	call   646c63b0 <_ValidateImageBase.part.0>
+    646c64ee:	test   %eax,%eax
+    646c64f0:	je     646c653d <__mingw_GetSectionForAddress+0x6d>
+    646c64f2:	movslq 0x3c(%r8),%rax
+    646c64f6:	mov    %rdx,%rcx
+    646c64f9:	sub    %r8,%rcx
+    646c64fc:	add    %rax,%r8
+    646c64ff:	movzwl 0x6(%r8),%edx
+    646c6504:	movzwl 0x14(%r8),%eax
+    646c6509:	test   %edx,%edx
+    646c650b:	lea    0x18(%r8,%rax,1),%rax
+    646c6510:	je     646c653d <__mingw_GetSectionForAddress+0x6d>
+    646c6512:	sub    $0x1,%edx
+    646c6515:	lea    (%rdx,%rdx,4),%rdx
+    646c6519:	lea    0x28(%rax,%rdx,8),%r9
+    646c651e:	xchg   %ax,%ax
+    646c6520:	mov    0xc(%rax),%r8d
+    646c6524:	cmp    %r8,%rcx
+    646c6527:	mov    %r8,%rdx
+    646c652a:	jb     646c6534 <__mingw_GetSectionForAddress+0x64>
+    646c652c:	add    0x8(%rax),%edx
+    646c652f:	cmp    %rdx,%rcx
+    646c6532:	jb     646c653f <__mingw_GetSectionForAddress+0x6f>
+    646c6534:	add    $0x28,%rax
+    646c6538:	cmp    %r9,%rax
+    646c653b:	jne    646c6520 <__mingw_GetSectionForAddress+0x50>
+    646c653d:	xor    %eax,%eax
+    646c653f:	add    $0x28,%rsp
+    646c6543:	ret
+    646c6544:	xchg   %ax,%ax
     646c6546:	cs nopw 0x0(%rax,%rax,1)
-    646c6550:	testb  $0x20,0x27(%rax)
-    646c6554:	je     646c655f <_FindPESectionExec+0x5f>
-    646c6556:	test   %rdx,%rdx
-    646c6559:	je     646c656a <_FindPESectionExec+0x6a>
-    646c655b:	sub    $0x1,%rdx
-    646c655f:	add    $0x28,%rax
-    646c6563:	cmp    %rcx,%rax
-    646c6566:	jne    646c6550 <_FindPESectionExec+0x50>
-    646c6568:	xor    %eax,%eax
-    646c656a:	add    $0x28,%rsp
-    646c656e:	ret
-    646c656f:	nop
-
-00000000646c6570 <_GetPEImageBase>:
-    646c6570:	sub    $0x28,%rsp
-    646c6574:	mov    0x30b5(%rip),%rdx        # 646c9630 <.refptr.__image_base__>
-    646c657b:	cmpw   $0x5a4d,(%rdx)
-    646c6580:	jne    646c65a0 <_GetPEImageBase+0x30>
-    646c6582:	mov    %rdx,%rcx
-    646c6585:	call   646c6320 <_ValidateImageBase.part.0>
-    646c658a:	test   %eax,%eax
-    646c658c:	mov    $0x0,%eax
-    646c6591:	cmovne %rdx,%rax
-    646c6595:	add    $0x28,%rsp
-    646c6599:	ret
-    646c659a:	nopw   0x0(%rax,%rax,1)
-    646c65a0:	xor    %eax,%eax
-    646c65a2:	add    $0x28,%rsp
-    646c65a6:	ret
-    646c65a7:	nopw   0x0(%rax,%rax,1)
-
-00000000646c65b0 <_IsNonwritableInCurrentImage>:
-    646c65b0:	sub    $0x28,%rsp
-    646c65b4:	mov    0x3075(%rip),%r8        # 646c9630 <.refptr.__image_base__>
-    646c65bb:	xor    %eax,%eax
-    646c65bd:	cmpw   $0x5a4d,(%r8)
-    646c65c3:	mov    %rcx,%rdx
-    646c65c6:	je     646c65d0 <_IsNonwritableInCurrentImage+0x20>
-    646c65c8:	add    $0x28,%rsp
-    646c65cc:	ret
-    646c65cd:	nopl   (%rax)
-    646c65d0:	mov    %r8,%rcx
-    646c65d3:	call   646c6320 <_ValidateImageBase.part.0>
-    646c65d8:	test   %eax,%eax
-    646c65da:	je     646c65c8 <_IsNonwritableInCurrentImage+0x18>
-    646c65dc:	movslq 0x3c(%r8),%rax
-    646c65e0:	mov    %rdx,%rcx
-    646c65e3:	sub    %r8,%rcx
-    646c65e6:	add    %rax,%r8
-    646c65e9:	movzwl 0x6(%r8),%edx
-    646c65ee:	movzwl 0x14(%r8),%eax
-    646c65f3:	test   %edx,%edx
-    646c65f5:	lea    0x18(%r8,%rax,1),%rax
-    646c65fa:	je     646c662d <_IsNonwritableInCurrentImage+0x7d>
-    646c65fc:	sub    $0x1,%edx
-    646c65ff:	lea    (%rdx,%rdx,4),%rdx
-    646c6603:	lea    0x28(%rax,%rdx,8),%r9
-    646c6608:	nopl   0x0(%rax,%rax,1)
-    646c6610:	mov    0xc(%rax),%r8d
-    646c6614:	cmp    %r8,%rcx
-    646c6617:	mov    %r8,%rdx
-    646c661a:	jb     646c6624 <_IsNonwritableInCurrentImage+0x74>
-    646c661c:	add    0x8(%rax),%edx
-    646c661f:	cmp    %rdx,%rcx
-    646c6622:	jb     646c6634 <_IsNonwritableInCurrentImage+0x84>
-    646c6624:	add    $0x28,%rax
-    646c6628:	cmp    %r9,%rax
-    646c662b:	jne    646c6610 <_IsNonwritableInCurrentImage+0x60>
-    646c662d:	xor    %eax,%eax
-    646c662f:	add    $0x28,%rsp
-    646c6633:	ret
-    646c6634:	mov    0x24(%rax),%eax
-    646c6637:	not    %eax
-    646c6639:	shr    $0x1f,%eax
-    646c663c:	add    $0x28,%rsp
-    646c6640:	ret
-    646c6641:	nopl   0x0(%rax,%rax,1)
-    646c6646:	cs nopw 0x0(%rax,%rax,1)
-
-00000000646c6650 <__mingw_enum_import_library_names>:
-    646c6650:	sub    $0x28,%rsp
-    646c6654:	mov    0x2fd5(%rip),%r11        # 646c9630 <.refptr.__image_base__>
-    646c665b:	cmpw   $0x5a4d,(%r11)
-    646c6661:	mov    %ecx,%r9d
-    646c6664:	jne    646c66be <__mingw_enum_import_library_names+0x6e>
-    646c6666:	mov    %r11,%rcx
-    646c6669:	call   646c6320 <_ValidateImageBase.part.0>
-    646c666e:	test   %eax,%eax
-    646c6670:	je     646c66be <__mingw_enum_import_library_names+0x6e>
-    646c6672:	movslq 0x3c(%r11),%rax
-    646c6676:	add    %r11,%rax
-    646c6679:	mov    0x90(%rax),%edx
-    646c667f:	test   %edx,%edx
-    646c6681:	je     646c66be <__mingw_enum_import_library_names+0x6e>
-    646c6683:	movzwl 0x14(%rax),%ecx
-    646c6687:	lea    0x18(%rax,%rcx,1),%rcx
-    646c668c:	movzwl 0x6(%rax),%eax
-    646c6690:	test   %eax,%eax
-    646c6692:	je     646c66be <__mingw_enum_import_library_names+0x6e>
-    646c6694:	sub    $0x1,%eax
-    646c6697:	lea    (%rax,%rax,4),%rax
-    646c669b:	lea    0x28(%rcx,%rax,8),%rax
-    646c66a0:	mov    0xc(%rcx),%r10d
-    646c66a4:	cmp    %r10,%rdx
-    646c66a7:	mov    %r10,%r8
-    646c66aa:	jb     646c66b5 <__mingw_enum_import_library_names+0x65>
-    646c66ac:	add    0x8(%rcx),%r8d
-    646c66b0:	cmp    %r8,%rdx
-    646c66b3:	jb     646c66c5 <__mingw_enum_import_library_names+0x75>
-    646c66b5:	add    $0x28,%rcx
-    646c66b9:	cmp    %rax,%rcx
-    646c66bc:	jne    646c66a0 <__mingw_enum_import_library_names+0x50>
-    646c66be:	xor    %eax,%eax
-    646c66c0:	add    $0x28,%rsp
-    646c66c4:	ret
-    646c66c5:	add    %r11,%rdx
-    646c66c8:	jne    646c66d8 <__mingw_enum_import_library_names+0x88>
-    646c66ca:	jmp    646c66be <__mingw_enum_import_library_names+0x6e>
-    646c66cc:	nopl   0x0(%rax)
-    646c66d0:	sub    $0x1,%r9d
-    646c66d4:	add    $0x14,%rdx
-    646c66d8:	mov    0x4(%rdx),%ecx
-    646c66db:	test   %ecx,%ecx
-    646c66dd:	jne    646c66e6 <__mingw_enum_import_library_names+0x96>
-    646c66df:	mov    0xc(%rdx),%eax
-    646c66e2:	test   %eax,%eax
-    646c66e4:	je     646c66be <__mingw_enum_import_library_names+0x6e>
-    646c66e6:	test   %r9d,%r9d
-    646c66e9:	jg     646c66d0 <__mingw_enum_import_library_names+0x80>
-    646c66eb:	mov    0xc(%rdx),%eax
-    646c66ee:	add    %r11,%rax
-    646c66f1:	add    $0x28,%rsp
-    646c66f5:	ret
-    646c66f6:	nop
-    646c66f7:	nop
-    646c66f8:	nop
-    646c66f9:	nop
-    646c66fa:	nop
-    646c66fb:	nop
-    646c66fc:	nop
-    646c66fd:	nop
-    646c66fe:	nop
-    646c66ff:	nop
-
-00000000646c6700 <_fpreset>:
-    646c6700:	fninit
-    646c6702:	ret
-    646c6703:	nop
-    646c6704:	nop
-    646c6705:	nop
-    646c6706:	nop
-    646c6707:	nop
-    646c6708:	nop
-    646c6709:	nop
-    646c670a:	nop
-    646c670b:	nop
-    646c670c:	nop
-    646c670d:	nop
-    646c670e:	nop
-    646c670f:	nop
 
-00000000646c6710 <___chkstk_ms>:
+00000000646c6550 <__mingw_GetSectionCount>:
+    646c6550:	sub    $0x28,%rsp
+    646c6554:	mov    0x30d5(%rip),%rdx        # 646c9630 <.refptr.__image_base__>
+    646c655b:	xor    %r8d,%r8d
+    646c655e:	cmpw   $0x5a4d,(%rdx)
+    646c6563:	je     646c6570 <__mingw_GetSectionCount+0x20>
+    646c6565:	mov    %r8d,%eax
+    646c6568:	add    $0x28,%rsp
+    646c656c:	ret
+    646c656d:	nopl   (%rax)
+    646c6570:	mov    %rdx,%rcx
+    646c6573:	call   646c63b0 <_ValidateImageBase.part.0>
+    646c6578:	test   %eax,%eax
+    646c657a:	je     646c6565 <__mingw_GetSectionCount+0x15>
+    646c657c:	movslq 0x3c(%rdx),%rax
+    646c6580:	movzwl 0x6(%rax,%rdx,1),%r8d
+    646c6586:	mov    %r8d,%eax
+    646c6589:	add    $0x28,%rsp
+    646c658d:	ret
+    646c658e:	xchg   %ax,%ax
+
+00000000646c6590 <_FindPESectionExec>:
+    646c6590:	sub    $0x28,%rsp
+    646c6594:	mov    0x3095(%rip),%r8        # 646c9630 <.refptr.__image_base__>
+    646c659b:	cmpw   $0x5a4d,(%r8)
+    646c65a1:	mov    %rcx,%rdx
+    646c65a4:	jne    646c65f8 <_FindPESectionExec+0x68>
+    646c65a6:	mov    %r8,%rcx
+    646c65a9:	call   646c63b0 <_ValidateImageBase.part.0>
+    646c65ae:	test   %eax,%eax
+    646c65b0:	je     646c65f8 <_FindPESectionExec+0x68>
+    646c65b2:	movslq 0x3c(%r8),%rcx
+    646c65b6:	add    %r8,%rcx
+    646c65b9:	movzwl 0x14(%rcx),%eax
+    646c65bd:	lea    0x18(%rcx,%rax,1),%rax
+    646c65c2:	movzwl 0x6(%rcx),%ecx
+    646c65c6:	test   %ecx,%ecx
+    646c65c8:	je     646c65f8 <_FindPESectionExec+0x68>
+    646c65ca:	sub    $0x1,%ecx
+    646c65cd:	lea    (%rcx,%rcx,4),%rcx
+    646c65d1:	lea    0x28(%rax,%rcx,8),%rcx
+    646c65d6:	cs nopw 0x0(%rax,%rax,1)
+    646c65e0:	testb  $0x20,0x27(%rax)
+    646c65e4:	je     646c65ef <_FindPESectionExec+0x5f>
+    646c65e6:	test   %rdx,%rdx
+    646c65e9:	je     646c65fa <_FindPESectionExec+0x6a>
+    646c65eb:	sub    $0x1,%rdx
+    646c65ef:	add    $0x28,%rax
+    646c65f3:	cmp    %rcx,%rax
+    646c65f6:	jne    646c65e0 <_FindPESectionExec+0x50>
+    646c65f8:	xor    %eax,%eax
+    646c65fa:	add    $0x28,%rsp
+    646c65fe:	ret
+    646c65ff:	nop
+
+00000000646c6600 <_GetPEImageBase>:
+    646c6600:	sub    $0x28,%rsp
+    646c6604:	mov    0x3025(%rip),%rdx        # 646c9630 <.refptr.__image_base__>
+    646c660b:	cmpw   $0x5a4d,(%rdx)
+    646c6610:	jne    646c6630 <_GetPEImageBase+0x30>
+    646c6612:	mov    %rdx,%rcx
+    646c6615:	call   646c63b0 <_ValidateImageBase.part.0>
+    646c661a:	test   %eax,%eax
+    646c661c:	mov    $0x0,%eax
+    646c6621:	cmovne %rdx,%rax
+    646c6625:	add    $0x28,%rsp
+    646c6629:	ret
+    646c662a:	nopw   0x0(%rax,%rax,1)
+    646c6630:	xor    %eax,%eax
+    646c6632:	add    $0x28,%rsp
+    646c6636:	ret
+    646c6637:	nopw   0x0(%rax,%rax,1)
+
+00000000646c6640 <_IsNonwritableInCurrentImage>:
+    646c6640:	sub    $0x28,%rsp
+    646c6644:	mov    0x2fe5(%rip),%r8        # 646c9630 <.refptr.__image_base__>
+    646c664b:	xor    %eax,%eax
+    646c664d:	cmpw   $0x5a4d,(%r8)
+    646c6653:	mov    %rcx,%rdx
+    646c6656:	je     646c6660 <_IsNonwritableInCurrentImage+0x20>
+    646c6658:	add    $0x28,%rsp
+    646c665c:	ret
+    646c665d:	nopl   (%rax)
+    646c6660:	mov    %r8,%rcx
+    646c6663:	call   646c63b0 <_ValidateImageBase.part.0>
+    646c6668:	test   %eax,%eax
+    646c666a:	je     646c6658 <_IsNonwritableInCurrentImage+0x18>
+    646c666c:	movslq 0x3c(%r8),%rax
+    646c6670:	mov    %rdx,%rcx
+    646c6673:	sub    %r8,%rcx
+    646c6676:	add    %rax,%r8
+    646c6679:	movzwl 0x6(%r8),%edx
+    646c667e:	movzwl 0x14(%r8),%eax
+    646c6683:	test   %edx,%edx
+    646c6685:	lea    0x18(%r8,%rax,1),%rax
+    646c668a:	je     646c66bd <_IsNonwritableInCurrentImage+0x7d>
+    646c668c:	sub    $0x1,%edx
+    646c668f:	lea    (%rdx,%rdx,4),%rdx
+    646c6693:	lea    0x28(%rax,%rdx,8),%r9
+    646c6698:	nopl   0x0(%rax,%rax,1)
+    646c66a0:	mov    0xc(%rax),%r8d
+    646c66a4:	cmp    %r8,%rcx
+    646c66a7:	mov    %r8,%rdx
+    646c66aa:	jb     646c66b4 <_IsNonwritableInCurrentImage+0x74>
+    646c66ac:	add    0x8(%rax),%edx
+    646c66af:	cmp    %rdx,%rcx
+    646c66b2:	jb     646c66c4 <_IsNonwritableInCurrentImage+0x84>
+    646c66b4:	add    $0x28,%rax
+    646c66b8:	cmp    %r9,%rax
+    646c66bb:	jne    646c66a0 <_IsNonwritableInCurrentImage+0x60>
+    646c66bd:	xor    %eax,%eax
+    646c66bf:	add    $0x28,%rsp
+    646c66c3:	ret
+    646c66c4:	mov    0x24(%rax),%eax
+    646c66c7:	not    %eax
+    646c66c9:	shr    $0x1f,%eax
+    646c66cc:	add    $0x28,%rsp
+    646c66d0:	ret
+    646c66d1:	nopl   0x0(%rax,%rax,1)
+    646c66d6:	cs nopw 0x0(%rax,%rax,1)
+
+00000000646c66e0 <__mingw_enum_import_library_names>:
+    646c66e0:	sub    $0x28,%rsp
+    646c66e4:	mov    0x2f45(%rip),%r11        # 646c9630 <.refptr.__image_base__>
+    646c66eb:	cmpw   $0x5a4d,(%r11)
+    646c66f1:	mov    %ecx,%r9d
+    646c66f4:	jne    646c674e <__mingw_enum_import_library_names+0x6e>
+    646c66f6:	mov    %r11,%rcx
+    646c66f9:	call   646c63b0 <_ValidateImageBase.part.0>
+    646c66fe:	test   %eax,%eax
+    646c6700:	je     646c674e <__mingw_enum_import_library_names+0x6e>
+    646c6702:	movslq 0x3c(%r11),%rax
+    646c6706:	add    %r11,%rax
+    646c6709:	mov    0x90(%rax),%edx
+    646c670f:	test   %edx,%edx
+    646c6711:	je     646c674e <__mingw_enum_import_library_names+0x6e>
+    646c6713:	movzwl 0x14(%rax),%ecx
+    646c6717:	lea    0x18(%rax,%rcx,1),%rcx
+    646c671c:	movzwl 0x6(%rax),%eax
+    646c6720:	test   %eax,%eax
+    646c6722:	je     646c674e <__mingw_enum_import_library_names+0x6e>
+    646c6724:	sub    $0x1,%eax
+    646c6727:	lea    (%rax,%rax,4),%rax
+    646c672b:	lea    0x28(%rcx,%rax,8),%rax
+    646c6730:	mov    0xc(%rcx),%r10d
+    646c6734:	cmp    %r10,%rdx
+    646c6737:	mov    %r10,%r8
+    646c673a:	jb     646c6745 <__mingw_enum_import_library_names+0x65>
+    646c673c:	add    0x8(%rcx),%r8d
+    646c6740:	cmp    %r8,%rdx
+    646c6743:	jb     646c6755 <__mingw_enum_import_library_names+0x75>
+    646c6745:	add    $0x28,%rcx
+    646c6749:	cmp    %rax,%rcx
+    646c674c:	jne    646c6730 <__mingw_enum_import_library_names+0x50>
+    646c674e:	xor    %eax,%eax
+    646c6750:	add    $0x28,%rsp
+    646c6754:	ret
+    646c6755:	add    %r11,%rdx
+    646c6758:	jne    646c6768 <__mingw_enum_import_library_names+0x88>
+    646c675a:	jmp    646c674e <__mingw_enum_import_library_names+0x6e>
+    646c675c:	nopl   0x0(%rax)
+    646c6760:	sub    $0x1,%r9d
+    646c6764:	add    $0x14,%rdx
+    646c6768:	mov    0x4(%rdx),%ecx
+    646c676b:	test   %ecx,%ecx
+    646c676d:	jne    646c6776 <__mingw_enum_import_library_names+0x96>
+    646c676f:	mov    0xc(%rdx),%eax
+    646c6772:	test   %eax,%eax
+    646c6774:	je     646c674e <__mingw_enum_import_library_names+0x6e>
+    646c6776:	test   %r9d,%r9d
+    646c6779:	jg     646c6760 <__mingw_enum_import_library_names+0x80>
+    646c677b:	mov    0xc(%rdx),%eax
+    646c677e:	add    %r11,%rax
+    646c6781:	add    $0x28,%rsp
+    646c6785:	ret
+    646c6786:	nop
+    646c6787:	nop
+    646c6788:	nop
+    646c6789:	nop
+    646c678a:	nop
+    646c678b:	nop
+    646c678c:	nop
+    646c678d:	nop
+    646c678e:	nop
+    646c678f:	nop
+
+00000000646c6790 <_fpreset>:
+    646c6790:	fninit
+    646c6792:	ret
+    646c6793:	nop
+    646c6794:	nop
+    646c6795:	nop
+    646c6796:	nop
+    646c6797:	nop
+    646c6798:	nop
+    646c6799:	nop
+    646c679a:	nop
+    646c679b:	nop
+    646c679c:	nop
+    646c679d:	nop
+    646c679e:	nop
+    646c679f:	nop
+
+00000000646c67a0 <___chkstk_ms>:
 C:\mingw810\x86_64-810-win32-seh-rt_v6-rev0\build\gcc-8.1.0\x86_64-w64-mingw32\libgcc/../../../../../src/gcc-8.1.0/libgcc/config/i386/cygwin.S:117
-    646c6710:	push   %rcx
+    646c67a0:	push   %rcx
 C:\mingw810\x86_64-810-win32-seh-rt_v6-rev0\build\gcc-8.1.0\x86_64-w64-mingw32\libgcc/../../../../../src/gcc-8.1.0/libgcc/config/i386/cygwin.S:119
-    646c6711:	push   %rax
+    646c67a1:	push   %rax
 C:\mingw810\x86_64-810-win32-seh-rt_v6-rev0\build\gcc-8.1.0\x86_64-w64-mingw32\libgcc/../../../../../src/gcc-8.1.0/libgcc/config/i386/cygwin.S:121
-    646c6712:	cmp    $0x1000,%rax
+    646c67a2:	cmp    $0x1000,%rax
 C:\mingw810\x86_64-810-win32-seh-rt_v6-rev0\build\gcc-8.1.0\x86_64-w64-mingw32\libgcc/../../../../../src/gcc-8.1.0/libgcc/config/i386/cygwin.S:122
-    646c6718:	lea    0x18(%rsp),%rcx
+    646c67a8:	lea    0x18(%rsp),%rcx
 C:\mingw810\x86_64-810-win32-seh-rt_v6-rev0\build\gcc-8.1.0\x86_64-w64-mingw32\libgcc/../../../../../src/gcc-8.1.0/libgcc/config/i386/cygwin.S:123
-    646c671d:	jb     646c6738 <___chkstk_ms+0x28>
+    646c67ad:	jb     646c67c8 <___chkstk_ms+0x28>
 C:\mingw810\x86_64-810-win32-seh-rt_v6-rev0\build\gcc-8.1.0\x86_64-w64-mingw32\libgcc/../../../../../src/gcc-8.1.0/libgcc/config/i386/cygwin.S:125
-    646c671f:	sub    $0x1000,%rcx
+    646c67af:	sub    $0x1000,%rcx
 C:\mingw810\x86_64-810-win32-seh-rt_v6-rev0\build\gcc-8.1.0\x86_64-w64-mingw32\libgcc/../../../../../src/gcc-8.1.0/libgcc/config/i386/cygwin.S:126
-    646c6726:	orq    $0x0,(%rcx)
+    646c67b6:	orq    $0x0,(%rcx)
 C:\mingw810\x86_64-810-win32-seh-rt_v6-rev0\build\gcc-8.1.0\x86_64-w64-mingw32\libgcc/../../../../../src/gcc-8.1.0/libgcc/config/i386/cygwin.S:127
-    646c672a:	sub    $0x1000,%rax
+    646c67ba:	sub    $0x1000,%rax
 C:\mingw810\x86_64-810-win32-seh-rt_v6-rev0\build\gcc-8.1.0\x86_64-w64-mingw32\libgcc/../../../../../src/gcc-8.1.0/libgcc/config/i386/cygwin.S:128
-    646c6730:	cmp    $0x1000,%rax
+    646c67c0:	cmp    $0x1000,%rax
 C:\mingw810\x86_64-810-win32-seh-rt_v6-rev0\build\gcc-8.1.0\x86_64-w64-mingw32\libgcc/../../../../../src/gcc-8.1.0/libgcc/config/i386/cygwin.S:129
-    646c6736:	ja     646c671f <___chkstk_ms+0xf>
+    646c67c6:	ja     646c67af <___chkstk_ms+0xf>
 C:\mingw810\x86_64-810-win32-seh-rt_v6-rev0\build\gcc-8.1.0\x86_64-w64-mingw32\libgcc/../../../../../src/gcc-8.1.0/libgcc/config/i386/cygwin.S:131
-    646c6738:	sub    %rax,%rcx
+    646c67c8:	sub    %rax,%rcx
 C:\mingw810\x86_64-810-win32-seh-rt_v6-rev0\build\gcc-8.1.0\x86_64-w64-mingw32\libgcc/../../../../../src/gcc-8.1.0/libgcc/config/i386/cygwin.S:132
-    646c673b:	orq    $0x0,(%rcx)
+    646c67cb:	orq    $0x0,(%rcx)
 C:\mingw810\x86_64-810-win32-seh-rt_v6-rev0\build\gcc-8.1.0\x86_64-w64-mingw32\libgcc/../../../../../src/gcc-8.1.0/libgcc/config/i386/cygwin.S:134
-    646c673f:	pop    %rax
+    646c67cf:	pop    %rax
 C:\mingw810\x86_64-810-win32-seh-rt_v6-rev0\build\gcc-8.1.0\x86_64-w64-mingw32\libgcc/../../../../../src/gcc-8.1.0/libgcc/config/i386/cygwin.S:136
-    646c6740:	pop    %rcx
+    646c67d0:	pop    %rcx
 C:\mingw810\x86_64-810-win32-seh-rt_v6-rev0\build\gcc-8.1.0\x86_64-w64-mingw32\libgcc/../../../../../src/gcc-8.1.0/libgcc/config/i386/cygwin.S:138
-    646c6741:	ret
-    646c6742:	nop
-    646c6743:	nop
-    646c6744:	nop
-    646c6745:	nop
-    646c6746:	nop
-    646c6747:	nop
-    646c6748:	nop
-    646c6749:	nop
-    646c674a:	nop
-    646c674b:	nop
-    646c674c:	nop
-    646c674d:	nop
-    646c674e:	nop
-    646c674f:	nop
-
-00000000646c6750 <DllEntryPoint>:
-    646c6750:	mov    $0x1,%eax
-    646c6755:	ret
-    646c6756:	nop
-    646c6757:	nop
-    646c6758:	nop
-    646c6759:	nop
-    646c675a:	nop
-    646c675b:	nop
-    646c675c:	nop
-    646c675d:	nop
-    646c675e:	nop
-    646c675f:	nop
-
-00000000646c6760 <DllMain>:
-    646c6760:	mov    $0x1,%eax
-    646c6765:	ret
-    646c6766:	nop
-    646c6767:	nop
-    646c6768:	nop
-    646c6769:	nop
-    646c676a:	nop
-    646c676b:	nop
-    646c676c:	nop
-    646c676d:	nop
-    646c676e:	nop
-    646c676f:	nop
-
-00000000646c6770 <__fpclassify>:
-    646c6770:	movq   %xmm0,%rax
-    646c6775:	movq   %xmm0,%rdx
-    646c677a:	shr    $0x20,%rax
-    646c677e:	mov    %eax,%ecx
-    646c6780:	and    $0xfffff,%ecx
-    646c6786:	or     %edx,%ecx
-    646c6788:	mov    %eax,%edx
-    646c678a:	mov    $0x4000,%eax
-    646c678f:	and    $0x7ff00000,%edx
-    646c6795:	mov    %ecx,%r8d
-    646c6798:	or     %edx,%r8d
-    646c679b:	je     646c67b3 <__fpclassify+0x43>
-    646c679d:	test   %edx,%edx
-    646c679f:	mov    $0x4400,%eax
-    646c67a4:	je     646c67b3 <__fpclassify+0x43>
-    646c67a6:	cmp    $0x7ff00000,%edx
-    646c67ac:	mov    $0x400,%eax
-    646c67b1:	je     646c67b4 <__fpclassify+0x44>
-    646c67b3:	ret
-    646c67b4:	cmp    $0x1,%ecx
-    646c67b7:	sbb    %eax,%eax
-    646c67b9:	and    $0x400,%eax
-    646c67be:	add    $0x100,%eax
-    646c67c3:	ret
-    646c67c4:	nop
-    646c67c5:	nop
-    646c67c6:	nop
-    646c67c7:	nop
-    646c67c8:	nop
-    646c67c9:	nop
-    646c67ca:	nop
-    646c67cb:	nop
-    646c67cc:	nop
-    646c67cd:	nop
-    646c67ce:	nop
-    646c67cf:	nop
-
-00000000646c67d0 <sqrt>:
-    646c67d0:	push   %rbx
-    646c67d1:	sub    $0x50,%rsp
-    646c67d5:	movaps %xmm6,0x40(%rsp)
-    646c67da:	movq   %xmm0,%rdx
-    646c67df:	movq   %xmm0,%rbx
-    646c67e4:	shr    $0x20,%rdx
-    646c67e8:	mov    %edx,%eax
-    646c67ea:	mov    %edx,%ecx
-    646c67ec:	and    $0xfffff,%eax
-    646c67f1:	and    $0x7ff00000,%ecx
-    646c67f7:	or     %ebx,%eax
-    646c67f9:	mov    %eax,%r8d
-    646c67fc:	or     %ecx,%r8d
-    646c67ff:	je     646c6840 <sqrt+0x70>
-    646c6801:	test   %ecx,%ecx
-    646c6803:	jne    646c6860 <sqrt+0x90>
-    646c6805:	test   %edx,%edx
-    646c6807:	js     646c6880 <sqrt+0xb0>
-    646c6809:	movsd  0x2b2f(%rip),%xmm0        # 646c9340 <.rdata+0x20>
-    646c6811:	movq   %rbx,%xmm1
-    646c6816:	ucomisd %xmm0,%xmm1
-    646c681a:	jp     646c681e <sqrt+0x4e>
-    646c681c:	je     646c6833 <sqrt+0x63>
-    646c681e:	mov    %rbx,0x38(%rsp)
-    646c6823:	fldl   0x38(%rsp)
-    646c6827:	fsqrt
-    646c6829:	fstpl  0x38(%rsp)
-    646c682d:	movsd  0x38(%rsp),%xmm0
-    646c6833:	movaps 0x40(%rsp),%xmm6
-    646c6838:	add    $0x50,%rsp
-    646c683c:	pop    %rbx
-    646c683d:	ret
-    646c683e:	xchg   %ax,%ax
-    646c6840:	test   %edx,%edx
-    646c6842:	pxor   %xmm0,%xmm0
-    646c6846:	jns    646c6833 <sqrt+0x63>
-    646c6848:	movsd  0x2ad8(%rip),%xmm0        # 646c9328 <.rdata+0x8>
-    646c6850:	movaps 0x40(%rsp),%xmm6
-    646c6855:	add    $0x50,%rsp
-    646c6859:	pop    %rbx
-    646c685a:	ret
-    646c685b:	nopl   0x0(%rax,%rax,1)
-    646c6860:	cmp    $0x7ff00000,%ecx
-    646c6866:	jne    646c6805 <sqrt+0x35>
-    646c6868:	test   %eax,%eax
-    646c686a:	jne    646c68c2 <sqrt+0xf2>
-    646c686c:	test   %edx,%edx
-    646c686e:	js     646c6880 <sqrt+0xb0>
-    646c6870:	movsd  0x2ac0(%rip),%xmm0        # 646c9338 <.rdata+0x18>
-    646c6878:	jmp    646c6833 <sqrt+0x63>
-    646c687a:	nopw   0x0(%rax,%rax,1)
-    646c6880:	call   646c7948 <_errno>
-    646c6885:	movq   %rbx,%xmm2
-    646c688a:	mov    $0x1,%ecx
-    646c688f:	movsd  0x2a99(%rip),%xmm6        # 646c9330 <.rdata+0x10>
-    646c6897:	movl   $0x21,(%rax)
-    646c689d:	lea    0x2a7c(%rip),%rdx        # 646c9320 <.rdata>
-    646c68a4:	pxor   %xmm3,%xmm3
-    646c68a8:	movsd  %xmm6,0x20(%rsp)
-    646c68ae:	call   646c7bc0 <__mingw_raise_matherr>
-    646c68b3:	movapd %xmm6,%xmm0
-    646c68b7:	movaps 0x40(%rsp),%xmm6
-    646c68bc:	add    $0x50,%rsp
-    646c68c0:	pop    %rbx
-    646c68c1:	ret
-    646c68c2:	call   646c7948 <_errno>
-    646c68c7:	movq   %rbx,%xmm2
-    646c68cc:	mov    $0x1,%ecx
-    646c68d1:	pxor   %xmm3,%xmm3
-    646c68d5:	movl   $0x21,(%rax)
-    646c68db:	lea    0x2a3e(%rip),%rdx        # 646c9320 <.rdata>
-    646c68e2:	mov    %rbx,0x20(%rsp)
-    646c68e7:	call   646c7bc0 <__mingw_raise_matherr>
-    646c68ec:	movq   %rbx,%xmm0
-    646c68f1:	jmp    646c6833 <sqrt+0x63>
-    646c68f6:	nop
-    646c68f7:	nop
-    646c68f8:	nop
-    646c68f9:	nop
-    646c68fa:	nop
-    646c68fb:	nop
-    646c68fc:	nop
-    646c68fd:	nop
-    646c68fe:	nop
-    646c68ff:	nop
-
-00000000646c6900 <__ms_vsnprintf>:
-    646c6900:	jmp    646c7930 <_vsnprintf>
-    646c6905:	nop
-    646c6906:	nop
-    646c6907:	nop
-    646c6908:	nop
-    646c6909:	nop
-    646c690a:	nop
-    646c690b:	nop
-    646c690c:	nop
-    646c690d:	nop
-    646c690e:	nop
-    646c690f:	nop
-
-00000000646c6910 <ceil>:
-    646c6910:	movq   %xmm0,%rax
-    646c6915:	mov    %rax,%rcx
-    646c6918:	sar    $0x34,%rcx
-    646c691c:	and    $0x7ff,%ecx
-    646c6922:	sub    $0x3ff,%ecx
-    646c6928:	cmp    $0x33,%ecx
-    646c692b:	jg     646c69d0 <.is_intnaninf>
-    646c6931:	test   %rax,%rax
-    646c6934:	je     646c69e0 <.ret_org>
-    646c693a:	test   %ecx,%ecx
-    646c693c:	js     646c6990 <.signed_val>
-    646c693e:	movabs $0xfffffffffffff,%rdx
-    646c6948:	sar    %cl,%rdx
-    646c694b:	test   %rax,%rdx
-    646c694e:	je     646c69e0 <.ret_org>
-    646c6954:	addsd  0x29f4(%rip),%xmm0        # 646c9350 <.huge>
-    646c695c:	ucomisd 0x29f4(%rip),%xmm0        # 646c9358 <.zero>
-    646c6964:	jbe    646c6981 <.doret>
-    646c6966:	test   %rax,%rax
-    646c6969:	jle    646c697b <.l1>
-    646c696b:	movabs $0x10000000000000,%r8
-    646c6975:	shr    %cl,%r8
-    646c6978:	add    %r8,%rax
-
-00000000646c697b <.l1>:
-    646c697b:	not    %rdx
-    646c697e:	and    %rdx,%rax
-
-00000000646c6981 <.doret>:
-    646c6981:	movq   %rax,%xmm0
-    646c6986:	ret
-    646c6987:	nopw   0x0(%rax,%rax,1)
-
-00000000646c6990 <.signed_val>:
-    646c6990:	addsd  0x29b8(%rip),%xmm0        # 646c9350 <.huge>
-    646c6998:	ucomisd 0x29b8(%rip),%xmm0        # 646c9358 <.zero>
-    646c69a0:	jbe    646c69c0 <.doret2>
-    646c69a2:	test   %rax,%rax
-    646c69a5:	movabs $0x3ff0000000000000,%rdx
-    646c69af:	movabs $0x8000000000000000,%rax
-    646c69b9:	cmovns %rdx,%rax
-    646c69bd:	nopl   (%rax)
-
-00000000646c69c0 <.doret2>:
-    646c69c0:	movq   %rax,%xmm0
-    646c69c5:	ret
-    646c69c6:	cs nopw 0x0(%rax,%rax,1)
-
-00000000646c69d0 <.is_intnaninf>:
-    646c69d0:	cmp    $0x400,%ecx
-    646c69d6:	je     646c69e2 <.ret_naninf>
-    646c69d8:	nopl   0x0(%rax,%rax,1)
-
-00000000646c69e0 <.ret_org>:
-    646c69e0:	repz ret
-
-00000000646c69e2 <.ret_naninf>:
-    646c69e2:	addsd  %xmm0,%xmm0
-    646c69e6:	ret
-    646c69e7:	nop
-    646c69e8:	nop
-    646c69e9:	nop
-    646c69ea:	nop
-    646c69eb:	nop
-    646c69ec:	nop
-    646c69ed:	nop
-    646c69ee:	nop
-    646c69ef:	nop
-
-00000000646c69f0 <cos>:
-    646c69f0:	push   %rbx
-    646c69f1:	sub    $0x70,%rsp
-    646c69f5:	movaps %xmm6,0x60(%rsp)
-    646c69fa:	movq   %xmm0,%rax
-    646c69ff:	movq   %xmm0,%rbx
-    646c6a04:	shr    $0x20,%rax
-    646c6a08:	mov    %eax,%edx
-    646c6a0a:	and    $0x7ff00000,%eax
-    646c6a0f:	and    $0xfffff,%edx
-    646c6a15:	or     %ebx,%edx
-    646c6a17:	mov    %edx,%ecx
-    646c6a19:	or     %eax,%ecx
-    646c6a1b:	sete   %r8b
-    646c6a1f:	test   %eax,%eax
-    646c6a21:	sete   %cl
-    646c6a24:	or     %cl,%r8b
-    646c6a27:	jne    646c6a30 <cos+0x40>
-    646c6a29:	cmp    $0x7ff00000,%eax
-    646c6a2e:	je     646c6a65 <cos+0x75>
-    646c6a30:	mov    %rbx,0x30(%rsp)
-    646c6a35:	lea    0x50(%rsp),%rcx
-    646c6a3a:	fldl   0x30(%rsp)
-    646c6a3e:	fstpt  0x40(%rsp)
-    646c6a42:	lea    0x40(%rsp),%rdx
-    646c6a47:	call   646c6af0 <__cosl_internal>
-    646c6a4c:	fldt   0x50(%rsp)
-    646c6a50:	fstpl  0x38(%rsp)
-    646c6a54:	movsd  0x38(%rsp),%xmm0
-    646c6a5a:	movaps 0x60(%rsp),%xmm6
-    646c6a5f:	add    $0x70,%rsp
-    646c6a63:	pop    %rbx
-    646c6a64:	ret
-    646c6a65:	test   %edx,%edx
-    646c6a67:	jne    646c6ab0 <cos+0xc0>
-    646c6a69:	call   646c7948 <_errno>
-    646c6a6e:	movq   %rbx,%xmm2
-    646c6a73:	mov    $0x1,%ecx
-    646c6a78:	movsd  0x28e8(%rip),%xmm6        # 646c9368 <.rdata+0x8>
-    646c6a80:	movl   $0x21,(%rax)
-    646c6a86:	lea    0x28d3(%rip),%rdx        # 646c9360 <.rdata>
-    646c6a8d:	pxor   %xmm3,%xmm3
-    646c6a91:	movsd  %xmm6,0x20(%rsp)
-    646c6a97:	call   646c7bc0 <__mingw_raise_matherr>
-    646c6a9c:	movapd %xmm6,%xmm0
-    646c6aa0:	movaps 0x60(%rsp),%xmm6
-    646c6aa5:	add    $0x70,%rsp
-    646c6aa9:	pop    %rbx
-    646c6aaa:	ret
-    646c6aab:	nopl   0x0(%rax,%rax,1)
-    646c6ab0:	call   646c7948 <_errno>
-    646c6ab5:	movq   %rbx,%xmm2
-    646c6aba:	mov    $0x1,%ecx
-    646c6abf:	pxor   %xmm3,%xmm3
-    646c6ac3:	movl   $0x21,(%rax)
-    646c6ac9:	lea    0x2890(%rip),%rdx        # 646c9360 <.rdata>
-    646c6ad0:	mov    %rbx,0x20(%rsp)
-    646c6ad5:	call   646c7bc0 <__mingw_raise_matherr>
-    646c6ada:	movq   %rbx,%xmm0
-    646c6adf:	jmp    646c6a5a <cos+0x6a>
-    646c6ae4:	nop
-    646c6ae5:	nop
-    646c6ae6:	nop
-    646c6ae7:	nop
-    646c6ae8:	nop
-    646c6ae9:	nop
-    646c6aea:	nop
-    646c6aeb:	nop
-    646c6aec:	nop
-    646c6aed:	nop
-    646c6aee:	nop
-    646c6aef:	nop
-
-00000000646c6af0 <__cosl_internal>:
-    646c6af0:	fldt   (%rdx)
-    646c6af2:	fcos
-    646c6af4:	fnstsw %ax
-    646c6af6:	test   $0x400,%eax
-    646c6afb:	je     646c6b12 <__cosl_internal+0x22>
-    646c6afd:	fldpi
-    646c6aff:	fadd   %st(0),%st
-    646c6b01:	fxch   %st(1)
-    646c6b03:	fprem1
-    646c6b05:	fnstsw %ax
-    646c6b07:	test   $0x400,%eax
-    646c6b0c:	jne    646c6b03 <__cosl_internal+0x13>
-    646c6b0e:	fstp   %st(1)
-    646c6b10:	fcos
-    646c6b12:	mov    %rcx,%rax
-    646c6b15:	movq   $0x0,0x8(%rcx)
-    646c6b1d:	fstpt  (%rcx)
-    646c6b1f:	ret
-
-00000000646c6b20 <exp>:
-    646c6b20:	push   %rbx
-    646c6b21:	sub    $0x50,%rsp
-    646c6b25:	movaps %xmm6,0x40(%rsp)
-    646c6b2a:	movsd  0x284e(%rip),%xmm6        # 646c9380 <.rdata+0x10>
-    646c6b32:	movq   %xmm0,%rdx
-    646c6b37:	movq   %xmm0,%rbx
-    646c6b3c:	shr    $0x20,%rdx
-    646c6b40:	mov    %edx,%eax
-    646c6b42:	mov    %edx,%ecx
-    646c6b44:	and    $0xfffff,%eax
-    646c6b49:	and    $0x7ff00000,%ecx
-    646c6b4f:	or     %ebx,%eax
-    646c6b51:	mov    %eax,%r8d
-    646c6b54:	or     %ecx,%r8d
-    646c6b57:	je     646c6b89 <exp+0x69>
-    646c6b59:	cmp    $0x7ff00000,%ecx
-    646c6b5f:	je     646c6c20 <exp+0x100>
-    646c6b65:	ucomisd 0x281b(%rip),%xmm0        # 646c9388 <.rdata+0x18>
-    646c6b6d:	movapd %xmm0,%xmm1
-    646c6b71:	ja     646c6c72 <exp+0x152>
-    646c6b77:	movsd  0x2811(%rip),%xmm0        # 646c9390 <.rdata+0x20>
-    646c6b7f:	pxor   %xmm6,%xmm6
-    646c6b83:	ucomisd %xmm1,%xmm0
-    646c6b87:	jbe    646c6ba0 <exp+0x80>
-    646c6b89:	movapd %xmm6,%xmm0
-    646c6b8d:	movaps 0x40(%rsp),%xmm6
-    646c6b92:	add    $0x50,%rsp
-    646c6b96:	pop    %rbx
-    646c6b97:	ret
-    646c6b98:	nopl   0x0(%rax,%rax,1)
-    646c6ba0:	mov    %rbx,0x30(%rsp)
-    646c6ba5:	fldl   0x30(%rsp)
-    646c6ba9:	fldl2e
-    646c6bab:	fmul   %st(1),%st
-    646c6bad:	sub    $0x8,%rsp
-    646c6bb1:	fnstcw 0x4(%rsp)
-    646c6bb5:	movzwl 0x4(%rsp),%eax
-    646c6bba:	or     $0xc,%ah
-    646c6bbd:	mov    %ax,(%rsp)
-    646c6bc1:	fldcw  (%rsp)
-    646c6bc4:	frndint
-    646c6bc6:	fld    %st(1)
-    646c6bc8:	frndint
-    646c6bca:	fldcw  0x4(%rsp)
-    646c6bce:	add    $0x8,%rsp
-    646c6bd2:	fld    %st(1)
-    646c6bd4:	fldt   0x1466(%rip)        # 646c8040 <c0>
-    646c6bda:	fld    %st(2)
-    646c6bdc:	fmul   %st(1),%st
-    646c6bde:	fsubp  %st,%st(2)
-    646c6be0:	fld    %st(4)
-    646c6be2:	fsub   %st(3),%st
-    646c6be4:	fmulp  %st,%st(1)
-    646c6be6:	faddp  %st,%st(1)
-    646c6be8:	fldt   0x1442(%rip)        # 646c8030 <c1>
-    646c6bee:	fmul   %st(4),%st
-    646c6bf0:	faddp  %st,%st(1)
-    646c6bf2:	f2xm1
-    646c6bf4:	fld1
-    646c6bf6:	faddp  %st,%st(1)
-    646c6bf8:	fstp   %st(1)
-    646c6bfa:	fscale
-    646c6bfc:	fstp   %st(1)
-    646c6bfe:	fstp   %st(1)
-    646c6c00:	fstpl  0x38(%rsp)
-    646c6c04:	movsd  0x38(%rsp),%xmm6
-    646c6c0a:	movapd %xmm6,%xmm0
-    646c6c0e:	movaps 0x40(%rsp),%xmm6
-    646c6c13:	add    $0x50,%rsp
-    646c6c17:	pop    %rbx
-    646c6c18:	ret
-    646c6c19:	nopl   0x0(%rax)
-    646c6c20:	test   %eax,%eax
-    646c6c22:	jne    646c6cd0 <exp+0x1b0>
-    646c6c28:	test   %edx,%edx
-    646c6c2a:	js     646c6cb4 <exp+0x194>
-    646c6c30:	call   646c7948 <_errno>
-    646c6c35:	movsd  0x273b(%rip),%xmm6        # 646c9378 <.rdata+0x8>
-    646c6c3d:	mov    $0x4,%ecx
-    646c6c42:	movl   $0x22,(%rax)
-    646c6c48:	movsd  %xmm6,0x20(%rsp)
-    646c6c4e:	movq   %rbx,%xmm2
-    646c6c53:	pxor   %xmm3,%xmm3
-    646c6c57:	lea    0x2712(%rip),%rdx        # 646c9370 <.rdata>
-    646c6c5e:	call   646c7bc0 <__mingw_raise_matherr>
-    646c6c63:	movapd %xmm6,%xmm0
-    646c6c67:	movaps 0x40(%rsp),%xmm6
-    646c6c6c:	add    $0x50,%rsp
-    646c6c70:	pop    %rbx
-    646c6c71:	ret
-    646c6c72:	call   646c7948 <_errno>
-    646c6c77:	movq   %rbx,%xmm2
-    646c6c7c:	mov    $0x3,%ecx
-    646c6c81:	movsd  0x26ef(%rip),%xmm6        # 646c9378 <.rdata+0x8>
-    646c6c89:	movl   $0x22,(%rax)
-    646c6c8f:	lea    0x26da(%rip),%rdx        # 646c9370 <.rdata>
-    646c6c96:	pxor   %xmm3,%xmm3
-    646c6c9a:	movsd  %xmm6,0x20(%rsp)
-    646c6ca0:	call   646c7bc0 <__mingw_raise_matherr>
-    646c6ca5:	movapd %xmm6,%xmm0
-    646c6ca9:	movaps 0x40(%rsp),%xmm6
-    646c6cae:	add    $0x50,%rsp
-    646c6cb2:	pop    %rbx
-    646c6cb3:	ret
-    646c6cb4:	call   646c7948 <_errno>
-    646c6cb9:	pxor   %xmm6,%xmm6
-    646c6cbd:	mov    $0x3,%ecx
-    646c6cc2:	movl   $0x22,(%rax)
-    646c6cc8:	jmp    646c6c48 <exp+0x128>
-    646c6ccd:	nopl   (%rax)
-    646c6cd0:	call   646c7948 <_errno>
-    646c6cd5:	movq   %rbx,%xmm2
-    646c6cda:	mov    $0x1,%ecx
-    646c6cdf:	pxor   %xmm3,%xmm3
-    646c6ce3:	movl   $0x21,(%rax)
-    646c6ce9:	lea    0x2680(%rip),%rdx        # 646c9370 <.rdata>
-    646c6cf0:	movq   %rbx,%xmm6
-    646c6cf5:	mov    %rbx,0x20(%rsp)
-    646c6cfa:	call   646c7bc0 <__mingw_raise_matherr>
-    646c6cff:	jmp    646c6b89 <exp+0x69>
-    646c6d04:	nop
-    646c6d05:	nop
-    646c6d06:	nop
-    646c6d07:	nop
-    646c6d08:	nop
-    646c6d09:	nop
-    646c6d0a:	nop
-    646c6d0b:	nop
-    646c6d0c:	nop
-    646c6d0d:	nop
-    646c6d0e:	nop
-    646c6d0f:	nop
-
-00000000646c6d10 <log>:
-    646c6d10:	push   %rbx
-    646c6d11:	sub    $0x70,%rsp
-    646c6d15:	movaps %xmm6,0x60(%rsp)
-    646c6d1a:	movq   %xmm0,%rdx
-    646c6d1f:	movq   %xmm0,%rbx
-    646c6d24:	shr    $0x20,%rdx
-    646c6d28:	mov    %edx,%eax
-    646c6d2a:	mov    %edx,%ecx
-    646c6d2c:	and    $0xfffff,%eax
-    646c6d31:	and    $0x7ff00000,%ecx
-    646c6d37:	or     %ebx,%eax
-    646c6d39:	mov    %eax,%r8d
-    646c6d3c:	or     %ecx,%r8d
-    646c6d3f:	je     646c6da0 <log+0x90>
-    646c6d41:	test   %ecx,%ecx
-    646c6d43:	jne    646c6d82 <log+0x72>
-    646c6d45:	test   %edx,%edx
-    646c6d47:	js     646c6dee <log+0xde>
-    646c6d4d:	mov    %rbx,0x30(%rsp)
-    646c6d52:	lea    0x50(%rsp),%rcx
-    646c6d57:	fldl   0x30(%rsp)
-    646c6d5b:	fstpt  0x40(%rsp)
-    646c6d5f:	lea    0x40(%rsp),%rdx
-    646c6d64:	call   646c7730 <__logl_internal>
-    646c6d69:	fldt   0x50(%rsp)
-    646c6d6d:	fstpl  0x38(%rsp)
-    646c6d71:	movsd  0x38(%rsp),%xmm0
-    646c6d77:	movaps 0x60(%rsp),%xmm6
-    646c6d7c:	add    $0x70,%rsp
-    646c6d80:	pop    %rbx
-    646c6d81:	ret
-    646c6d82:	cmp    $0x7ff00000,%ecx
-    646c6d88:	jne    646c6d45 <log+0x35>
-    646c6d8a:	test   %eax,%eax
-    646c6d8c:	je     646c6de2 <log+0xd2>
-    646c6d8e:	test   %edx,%edx
-    646c6d90:	js     646c6dee <log+0xde>
-    646c6d92:	movsd  0x2616(%rip),%xmm0        # 646c93b0 <.rdata+0x10>
-    646c6d9a:	jmp    646c6d77 <log+0x67>
-    646c6d9c:	nopl   0x0(%rax)
-    646c6da0:	call   646c7948 <_errno>
-    646c6da5:	movq   %rbx,%xmm2
-    646c6daa:	mov    $0x3,%ecx
-    646c6daf:	movsd  0x25f1(%rip),%xmm6        # 646c93a8 <.rdata+0x8>
-    646c6db7:	movl   $0x22,(%rax)
-    646c6dbd:	lea    0x25dc(%rip),%rdx        # 646c93a0 <.rdata>
-    646c6dc4:	pxor   %xmm3,%xmm3
-    646c6dc8:	movsd  %xmm6,0x20(%rsp)
-    646c6dce:	call   646c7bc0 <__mingw_raise_matherr>
-    646c6dd3:	movapd %xmm6,%xmm0
-    646c6dd7:	movaps 0x60(%rsp),%xmm6
-    646c6ddc:	add    $0x70,%rsp
-    646c6de0:	pop    %rbx
-    646c6de1:	ret
-    646c6de2:	test   %edx,%edx
-    646c6de4:	movsd  0x25cc(%rip),%xmm0        # 646c93b8 <.rdata+0x18>
-    646c6dec:	jns    646c6d77 <log+0x67>
-    646c6dee:	call   646c7948 <_errno>
-    646c6df3:	movq   %rbx,%xmm2
-    646c6df8:	mov    $0x1,%ecx
-    646c6dfd:	movsd  0x25ab(%rip),%xmm6        # 646c93b0 <.rdata+0x10>
-    646c6e05:	movl   $0x21,(%rax)
-    646c6e0b:	lea    0x258e(%rip),%rdx        # 646c93a0 <.rdata>
-    646c6e12:	pxor   %xmm3,%xmm3
-    646c6e16:	movsd  %xmm6,0x20(%rsp)
-    646c6e1c:	call   646c7bc0 <__mingw_raise_matherr>
-    646c6e21:	movapd %xmm6,%xmm0
-    646c6e25:	movaps 0x60(%rsp),%xmm6
-    646c6e2a:	add    $0x70,%rsp
-    646c6e2e:	pop    %rbx
-    646c6e2f:	ret
-
-00000000646c6e30 <internal_modf>:
-    646c6e30:	sub    $0x18,%rsp
-    646c6e34:	movsd  %xmm0,0x8(%rsp)
-    646c6e3a:	fldl   0x8(%rsp)
-    646c6e3e:	push   %rax
-    646c6e3f:	sub    $0x8,%rsp
-    646c6e43:	fnstcw 0x4(%rsp)
-    646c6e47:	movzwl 0x4(%rsp),%eax
-    646c6e4c:	or     $0xc,%ah
-    646c6e4f:	mov    %ax,(%rsp)
-    646c6e53:	fldcw  (%rsp)
-    646c6e56:	frndint
-    646c6e58:	fldcw  0x4(%rsp)
-    646c6e5c:	add    $0x8,%rsp
-    646c6e60:	pop    %rax
-    646c6e61:	movq   %xmm0,%rax
-    646c6e66:	fstpl  0x8(%rsp)
-    646c6e6a:	movsd  0x8(%rsp),%xmm1
-    646c6e70:	shr    $0x20,%rax
-    646c6e74:	mov    %eax,%ecx
-    646c6e76:	movsd  %xmm1,(%rdx)
-    646c6e7a:	movq   %xmm0,%rdx
-    646c6e7f:	and    $0x7ff00000,%eax
-    646c6e84:	and    $0xfffff,%ecx
-    646c6e8a:	or     %edx,%ecx
-    646c6e8c:	mov    %ecx,%edx
-    646c6e8e:	or     %eax,%edx
-    646c6e90:	sete   %dl
-    646c6e93:	test   %eax,%eax
-    646c6e95:	sete   %r8b
-    646c6e99:	or     %r8d,%edx
-    646c6e9c:	xor    $0x1,%edx
-    646c6e9f:	cmp    $0x7ff00000,%eax
-    646c6ea4:	sete   %al
-    646c6ea7:	test   %al,%dl
-    646c6ea9:	je     646c6eaf <internal_modf+0x7f>
-    646c6eab:	test   %ecx,%ecx
-    646c6ead:	je     646c6ec0 <internal_modf+0x90>
-    646c6eaf:	subsd  0x8(%rsp),%xmm0
-    646c6eb5:	add    $0x18,%rsp
-    646c6eb9:	ret
-    646c6eba:	nopw   0x0(%rax,%rax,1)
-    646c6ec0:	pxor   %xmm0,%xmm0
-    646c6ec4:	jmp    646c6eb5 <internal_modf+0x85>
-    646c6ec6:	cs nopw 0x0(%rax,%rax,1)
-
-00000000646c6ed0 <pow>:
-    646c6ed0:	push   %r12
-    646c6ed2:	push   %rbp
-    646c6ed3:	push   %rdi
-    646c6ed4:	push   %rsi
-    646c6ed5:	push   %rbx
-    646c6ed6:	sub    $0x90,%rsp
-    646c6edd:	movaps %xmm6,0x70(%rsp)
-    646c6ee2:	movaps %xmm7,0x80(%rsp)
-    646c6eea:	mov    $0x4000,%edx
-    646c6eef:	movq   %xmm0,%rbx
-    646c6ef4:	movq   %xmm0,%rdi
-    646c6ef9:	movq   %xmm1,%rbp
-    646c6efe:	shr    $0x20,%rbx
-    646c6f02:	mov    %ebx,%eax
-    646c6f04:	mov    %ebx,%ecx
-    646c6f06:	and    $0xfffff,%eax
-    646c6f0b:	and    $0x7ff00000,%ecx
-    646c6f11:	or     %edi,%eax
-    646c6f13:	mov    %ecx,%esi
-    646c6f15:	or     %eax,%esi
-    646c6f17:	je     646c6f26 <pow+0x56>
-    646c6f19:	test   %ecx,%ecx
-    646c6f1b:	mov    $0x4400,%edx
-    646c6f20:	jne    646c7071 <pow+0x1a1>
-    646c6f26:	mov    %rbp,%rsi
-    646c6f29:	movsd  0x24bf(%rip),%xmm6        # 646c93f0 <.rdata+0x30>
-    646c6f31:	shr    $0x20,%rsi
-    646c6f35:	mov    %esi,%eax
-    646c6f37:	mov    %esi,%ecx
-    646c6f39:	and    $0xfffff,%eax
-    646c6f3e:	and    $0x7ff00000,%ecx
-    646c6f44:	or     %ebp,%eax
-    646c6f46:	mov    %ecx,%r9d
-    646c6f49:	or     %eax,%r9d
-    646c6f4c:	je     646c6fdb <pow+0x10b>
-    646c6f52:	test   %ecx,%ecx
-    646c6f54:	jne    646c7000 <pow+0x130>
-    646c6f5a:	mov    $0x4400,%r8d
-    646c6f60:	movsd  0x2488(%rip),%xmm2        # 646c93f0 <.rdata+0x30>
-    646c6f68:	movq   %rdi,%xmm4
-    646c6f6d:	ucomisd %xmm2,%xmm4
-    646c6f71:	jp     646c6f79 <pow+0xa9>
-    646c6f73:	je     646c73c8 <pow+0x4f8>
-    646c6f79:	cmp    $0x100,%edx
-    646c6f7f:	je     646c7030 <pow+0x160>
-    646c6f85:	cmp    $0x4000,%edx
-    646c6f8b:	je     646c70a0 <pow+0x1d0>
-    646c6f91:	cmp    $0x500,%r8d
-    646c6f98:	je     646c70f0 <pow+0x220>
-    646c6f9e:	cmp    $0x500,%edx
-    646c6fa4:	jne    646c7115 <pow+0x245>
-    646c6faa:	test   %ebx,%ebx
-    646c6fac:	js     646c72b1 <pow+0x3e1>
-    646c6fb2:	mov    $0xffffffff,%edx
-    646c6fb7:	movq   %rbp,%xmm0
-    646c6fbc:	call   646c7780 <ldexp>
-    646c6fc1:	lea    0x68(%rsp),%rdx
-    646c6fc6:	call   646c6e30 <internal_modf>
-    646c6fcb:	test   %esi,%esi
-    646c6fcd:	js     646c70d2 <pow+0x202>
-    646c6fd3:	movsd  0x240d(%rip),%xmm6        # 646c93e8 <.rdata+0x28>
-    646c6fdb:	movapd %xmm6,%xmm0
-    646c6fdf:	movaps 0x80(%rsp),%xmm7
-    646c6fe7:	movaps 0x70(%rsp),%xmm6
-    646c6fec:	add    $0x90,%rsp
-    646c6ff3:	pop    %rbx
-    646c6ff4:	pop    %rsi
-    646c6ff5:	pop    %rdi
-    646c6ff6:	pop    %rbp
-    646c6ff7:	pop    %r12
-    646c6ff9:	ret
-    646c6ffa:	nopw   0x0(%rax,%rax,1)
-    646c7000:	cmp    $0x7ff00000,%ecx
-    646c7006:	mov    $0x400,%r8d
-    646c700c:	jne    646c6f60 <pow+0x90>
-    646c7012:	test   %eax,%eax
-    646c7014:	mov    $0x500,%r8d
-    646c701a:	je     646c6f60 <pow+0x90>
-    646c7020:	movq   %rdi,%xmm5
-    646c7025:	ucomisd %xmm6,%xmm5
-    646c7029:	jp     646c7030 <pow+0x160>
-    646c702b:	je     646c6fdb <pow+0x10b>
-    646c702d:	nopl   (%rax)
-    646c7030:	test   %ebx,%ebx
-    646c7032:	movsd  0x2396(%rip),%xmm6        # 646c93d0 <.rdata+0x10>
-    646c703a:	js     646c70e0 <pow+0x210>
-    646c7040:	call   646c7948 <_errno>
-    646c7045:	movl   $0x21,(%rax)
-    646c704b:	movsd  %xmm6,0x20(%rsp)
-    646c7051:	movq   %rbp,%xmm3
-    646c7056:	movq   %rdi,%xmm2
-    646c705b:	mov    $0x1,%ecx
-    646c7060:	lea    0x2359(%rip),%rdx        # 646c93c0 <.rdata>
-    646c7067:	call   646c7bc0 <__mingw_raise_matherr>
-    646c706c:	jmp    646c6fdb <pow+0x10b>
-    646c7071:	cmp    $0x7ff00000,%ecx
-    646c7077:	mov    $0x400,%edx
-    646c707c:	jne    646c6f26 <pow+0x56>
-    646c7082:	cmp    $0x1,%eax
-    646c7085:	sbb    %edx,%edx
-    646c7087:	and    $0x400,%edx
-    646c708d:	add    $0x100,%edx
-    646c7093:	jmp    646c6f26 <pow+0x56>
-    646c7098:	nopl   0x0(%rax,%rax,1)
-    646c70a0:	cmp    $0x500,%r8d
-    646c70a7:	je     646c70ca <pow+0x1fa>
-    646c70a9:	test   %ebx,%ebx
-    646c70ab:	js     646c7270 <pow+0x3a0>
-    646c70b1:	mov    $0xffffffff,%edx
-    646c70b6:	movq   %rbp,%xmm0
-    646c70bb:	call   646c7780 <ldexp>
-    646c70c0:	lea    0x68(%rsp),%rdx
-    646c70c5:	call   646c6e30 <internal_modf>
-    646c70ca:	test   %esi,%esi
-    646c70cc:	js     646c6fd3 <pow+0x103>
-    646c70d2:	pxor   %xmm6,%xmm6
-    646c70d6:	jmp    646c6fdb <pow+0x10b>
-    646c70db:	nopl   0x0(%rax,%rax,1)
-    646c70e0:	movsd  0x22e0(%rip),%xmm6        # 646c93c8 <.rdata+0x8>
-    646c70e8:	jmp    646c7040 <pow+0x170>
-    646c70ed:	nopl   (%rax)
-    646c70f0:	cmp    $0x500,%edx
-    646c70f6:	je     646c6fcb <pow+0xfb>
-    646c70fc:	test   %ebx,%ebx
-    646c70fe:	js     646c73a5 <pow+0x4d5>
-    646c7104:	movq   %rdi,%xmm5
-    646c7109:	ucomisd %xmm2,%xmm5
-    646c710d:	ja     646c6fcb <pow+0xfb>
-    646c7113:	jmp    646c70ca <pow+0x1fa>
-    646c7115:	lea    0x68(%rsp),%rsi
-    646c711a:	movq   %rbp,%xmm0
-    646c711f:	pxor   %xmm7,%xmm7
-    646c7123:	mov    %rsi,%rdx
-    646c7126:	call   646c6e30 <internal_modf>
-    646c712b:	ucomisd %xmm7,%xmm0
-    646c712f:	jp     646c71f1 <pow+0x321>
-    646c7135:	jne    646c71f1 <pow+0x321>
-    646c713b:	movsd  0x68(%rsp),%xmm0
-    646c7141:	movsd  0x22d7(%rip),%xmm1        # 646c9420 <.rdata+0x60>
-    646c7149:	ucomisd %xmm0,%xmm1
-    646c714d:	jb     646c715d <pow+0x28d>
-    646c714f:	ucomisd 0x22d1(%rip),%xmm0        # 646c9428 <.rdata+0x68>
-    646c7157:	jae    646c7403 <pow+0x533>
-    646c715d:	lea    0x50(%rsp),%r12
-    646c7162:	movq   %rdi,%xmm5
-    646c7167:	andpd  0x22c1(%rip),%xmm5        # 646c9430 <.rdata+0x70>
-    646c716f:	movsd  %xmm5,0x30(%rsp)
-    646c7175:	lea    0x40(%rsp),%rdi
-    646c717a:	fldl   0x30(%rsp)
-    646c717e:	mov    %r12,%rcx
-    646c7181:	fstpt  0x40(%rsp)
-    646c7185:	mov    %rdi,%rdx
-    646c7188:	call   646c7850 <log2l>
-    646c718d:	mov    %rdi,%rdx
-    646c7190:	mov    %r12,%rcx
-    646c7193:	fldt   0x50(%rsp)
-    646c7197:	mov    %rbp,0x30(%rsp)
-    646c719c:	fldl   0x30(%rsp)
-    646c71a0:	fmulp  %st,%st(1)
-    646c71a2:	fstpt  0x40(%rsp)
-    646c71a6:	call   646c76b0 <exp2l>
-    646c71ab:	test   %ebx,%ebx
-    646c71ad:	fldt   0x50(%rsp)
-    646c71b1:	fstpl  0x38(%rsp)
-    646c71b5:	movsd  0x38(%rsp),%xmm6
-    646c71bb:	jns    646c6fdb <pow+0x10b>
-    646c71c1:	mov    $0xffffffff,%edx
-    646c71c6:	movq   %rbp,%xmm0
-    646c71cb:	call   646c7780 <ldexp>
-    646c71d0:	mov    %rsi,%rdx
-    646c71d3:	call   646c6e30 <internal_modf>
-    646c71d8:	ucomisd %xmm7,%xmm0
-    646c71dc:	jp     646c71e4 <pow+0x314>
-    646c71de:	je     646c6fdb <pow+0x10b>
-    646c71e4:	xorpd  0x2214(%rip),%xmm6        # 646c9400 <.rdata+0x40>
-    646c71ec:	jmp    646c6fdb <pow+0x10b>
-    646c71f1:	test   %ebx,%ebx
-    646c71f3:	js     646c73eb <pow+0x51b>
-    646c71f9:	movq   %rbp,%xmm5
-    646c71fe:	ucomisd 0x2212(%rip),%xmm5        # 646c9418 <.rdata+0x58>
-    646c7206:	jp     646c720e <pow+0x33e>
-    646c7208:	je     646c73d1 <pow+0x501>
-    646c720e:	lea    0x50(%rsp),%rbx
-    646c7213:	movq   %rdi,%xmm3
-    646c7218:	andpd  0x2210(%rip),%xmm3        # 646c9430 <.rdata+0x70>
-    646c7220:	movsd  %xmm3,0x30(%rsp)
-    646c7226:	lea    0x40(%rsp),%rsi
-    646c722b:	fldl   0x30(%rsp)
-    646c722f:	mov    %rbx,%rcx
+    646c67d1:	ret
+    646c67d2:	nop
+    646c67d3:	nop
+    646c67d4:	nop
+    646c67d5:	nop
+    646c67d6:	nop
+    646c67d7:	nop
+    646c67d8:	nop
+    646c67d9:	nop
+    646c67da:	nop
+    646c67db:	nop
+    646c67dc:	nop
+    646c67dd:	nop
+    646c67de:	nop
+    646c67df:	nop
+
+00000000646c67e0 <DllEntryPoint>:
+    646c67e0:	mov    $0x1,%eax
+    646c67e5:	ret
+    646c67e6:	nop
+    646c67e7:	nop
+    646c67e8:	nop
+    646c67e9:	nop
+    646c67ea:	nop
+    646c67eb:	nop
+    646c67ec:	nop
+    646c67ed:	nop
+    646c67ee:	nop
+    646c67ef:	nop
+
+00000000646c67f0 <DllMain>:
+    646c67f0:	mov    $0x1,%eax
+    646c67f5:	ret
+    646c67f6:	nop
+    646c67f7:	nop
+    646c67f8:	nop
+    646c67f9:	nop
+    646c67fa:	nop
+    646c67fb:	nop
+    646c67fc:	nop
+    646c67fd:	nop
+    646c67fe:	nop
+    646c67ff:	nop
+
+00000000646c6800 <__fpclassify>:
+    646c6800:	movq   %xmm0,%rax
+    646c6805:	movq   %xmm0,%rdx
+    646c680a:	shr    $0x20,%rax
+    646c680e:	mov    %eax,%ecx
+    646c6810:	and    $0xfffff,%ecx
+    646c6816:	or     %edx,%ecx
+    646c6818:	mov    %eax,%edx
+    646c681a:	mov    $0x4000,%eax
+    646c681f:	and    $0x7ff00000,%edx
+    646c6825:	mov    %ecx,%r8d
+    646c6828:	or     %edx,%r8d
+    646c682b:	je     646c6843 <__fpclassify+0x43>
+    646c682d:	test   %edx,%edx
+    646c682f:	mov    $0x4400,%eax
+    646c6834:	je     646c6843 <__fpclassify+0x43>
+    646c6836:	cmp    $0x7ff00000,%edx
+    646c683c:	mov    $0x400,%eax
+    646c6841:	je     646c6844 <__fpclassify+0x44>
+    646c6843:	ret
+    646c6844:	cmp    $0x1,%ecx
+    646c6847:	sbb    %eax,%eax
+    646c6849:	and    $0x400,%eax
+    646c684e:	add    $0x100,%eax
+    646c6853:	ret
+    646c6854:	nop
+    646c6855:	nop
+    646c6856:	nop
+    646c6857:	nop
+    646c6858:	nop
+    646c6859:	nop
+    646c685a:	nop
+    646c685b:	nop
+    646c685c:	nop
+    646c685d:	nop
+    646c685e:	nop
+    646c685f:	nop
+
+00000000646c6860 <sqrt>:
+    646c6860:	push   %rbx
+    646c6861:	sub    $0x50,%rsp
+    646c6865:	movaps %xmm6,0x40(%rsp)
+    646c686a:	movq   %xmm0,%rdx
+    646c686f:	movq   %xmm0,%rbx
+    646c6874:	shr    $0x20,%rdx
+    646c6878:	mov    %edx,%eax
+    646c687a:	mov    %edx,%ecx
+    646c687c:	and    $0xfffff,%eax
+    646c6881:	and    $0x7ff00000,%ecx
+    646c6887:	or     %ebx,%eax
+    646c6889:	mov    %eax,%r8d
+    646c688c:	or     %ecx,%r8d
+    646c688f:	je     646c68d0 <sqrt+0x70>
+    646c6891:	test   %ecx,%ecx
+    646c6893:	jne    646c68f0 <sqrt+0x90>
+    646c6895:	test   %edx,%edx
+    646c6897:	js     646c6910 <sqrt+0xb0>
+    646c6899:	movsd  0x2a9f(%rip),%xmm0        # 646c9340 <.rdata+0x20>
+    646c68a1:	movq   %rbx,%xmm1
+    646c68a6:	ucomisd %xmm0,%xmm1
+    646c68aa:	jp     646c68ae <sqrt+0x4e>
+    646c68ac:	je     646c68c3 <sqrt+0x63>
+    646c68ae:	mov    %rbx,0x38(%rsp)
+    646c68b3:	fldl   0x38(%rsp)
+    646c68b7:	fsqrt
+    646c68b9:	fstpl  0x38(%rsp)
+    646c68bd:	movsd  0x38(%rsp),%xmm0
+    646c68c3:	movaps 0x40(%rsp),%xmm6
+    646c68c8:	add    $0x50,%rsp
+    646c68cc:	pop    %rbx
+    646c68cd:	ret
+    646c68ce:	xchg   %ax,%ax
+    646c68d0:	test   %edx,%edx
+    646c68d2:	pxor   %xmm0,%xmm0
+    646c68d6:	jns    646c68c3 <sqrt+0x63>
+    646c68d8:	movsd  0x2a48(%rip),%xmm0        # 646c9328 <.rdata+0x8>
+    646c68e0:	movaps 0x40(%rsp),%xmm6
+    646c68e5:	add    $0x50,%rsp
+    646c68e9:	pop    %rbx
+    646c68ea:	ret
+    646c68eb:	nopl   0x0(%rax,%rax,1)
+    646c68f0:	cmp    $0x7ff00000,%ecx
+    646c68f6:	jne    646c6895 <sqrt+0x35>
+    646c68f8:	test   %eax,%eax
+    646c68fa:	jne    646c6952 <sqrt+0xf2>
+    646c68fc:	test   %edx,%edx
+    646c68fe:	js     646c6910 <sqrt+0xb0>
+    646c6900:	movsd  0x2a30(%rip),%xmm0        # 646c9338 <.rdata+0x18>
+    646c6908:	jmp    646c68c3 <sqrt+0x63>
+    646c690a:	nopw   0x0(%rax,%rax,1)
+    646c6910:	call   646c79d8 <_errno>
+    646c6915:	movq   %rbx,%xmm2
+    646c691a:	mov    $0x1,%ecx
+    646c691f:	movsd  0x2a09(%rip),%xmm6        # 646c9330 <.rdata+0x10>
+    646c6927:	movl   $0x21,(%rax)
+    646c692d:	lea    0x29ec(%rip),%rdx        # 646c9320 <.rdata>
+    646c6934:	pxor   %xmm3,%xmm3
+    646c6938:	movsd  %xmm6,0x20(%rsp)
+    646c693e:	call   646c7c50 <__mingw_raise_matherr>
+    646c6943:	movapd %xmm6,%xmm0
+    646c6947:	movaps 0x40(%rsp),%xmm6
+    646c694c:	add    $0x50,%rsp
+    646c6950:	pop    %rbx
+    646c6951:	ret
+    646c6952:	call   646c79d8 <_errno>
+    646c6957:	movq   %rbx,%xmm2
+    646c695c:	mov    $0x1,%ecx
+    646c6961:	pxor   %xmm3,%xmm3
+    646c6965:	movl   $0x21,(%rax)
+    646c696b:	lea    0x29ae(%rip),%rdx        # 646c9320 <.rdata>
+    646c6972:	mov    %rbx,0x20(%rsp)
+    646c6977:	call   646c7c50 <__mingw_raise_matherr>
+    646c697c:	movq   %rbx,%xmm0
+    646c6981:	jmp    646c68c3 <sqrt+0x63>
+    646c6986:	nop
+    646c6987:	nop
+    646c6988:	nop
+    646c6989:	nop
+    646c698a:	nop
+    646c698b:	nop
+    646c698c:	nop
+    646c698d:	nop
+    646c698e:	nop
+    646c698f:	nop
+
+00000000646c6990 <__ms_vsnprintf>:
+    646c6990:	jmp    646c79c0 <_vsnprintf>
+    646c6995:	nop
+    646c6996:	nop
+    646c6997:	nop
+    646c6998:	nop
+    646c6999:	nop
+    646c699a:	nop
+    646c699b:	nop
+    646c699c:	nop
+    646c699d:	nop
+    646c699e:	nop
+    646c699f:	nop
+
+00000000646c69a0 <ceil>:
+    646c69a0:	movq   %xmm0,%rax
+    646c69a5:	mov    %rax,%rcx
+    646c69a8:	sar    $0x34,%rcx
+    646c69ac:	and    $0x7ff,%ecx
+    646c69b2:	sub    $0x3ff,%ecx
+    646c69b8:	cmp    $0x33,%ecx
+    646c69bb:	jg     646c6a60 <.is_intnaninf>
+    646c69c1:	test   %rax,%rax
+    646c69c4:	je     646c6a70 <.ret_org>
+    646c69ca:	test   %ecx,%ecx
+    646c69cc:	js     646c6a20 <.signed_val>
+    646c69ce:	movabs $0xfffffffffffff,%rdx
+    646c69d8:	sar    %cl,%rdx
+    646c69db:	test   %rax,%rdx
+    646c69de:	je     646c6a70 <.ret_org>
+    646c69e4:	addsd  0x2964(%rip),%xmm0        # 646c9350 <.huge>
+    646c69ec:	ucomisd 0x2964(%rip),%xmm0        # 646c9358 <.zero>
+    646c69f4:	jbe    646c6a11 <.doret>
+    646c69f6:	test   %rax,%rax
+    646c69f9:	jle    646c6a0b <.l1>
+    646c69fb:	movabs $0x10000000000000,%r8
+    646c6a05:	shr    %cl,%r8
+    646c6a08:	add    %r8,%rax
+
+00000000646c6a0b <.l1>:
+    646c6a0b:	not    %rdx
+    646c6a0e:	and    %rdx,%rax
+
+00000000646c6a11 <.doret>:
+    646c6a11:	movq   %rax,%xmm0
+    646c6a16:	ret
+    646c6a17:	nopw   0x0(%rax,%rax,1)
+
+00000000646c6a20 <.signed_val>:
+    646c6a20:	addsd  0x2928(%rip),%xmm0        # 646c9350 <.huge>
+    646c6a28:	ucomisd 0x2928(%rip),%xmm0        # 646c9358 <.zero>
+    646c6a30:	jbe    646c6a50 <.doret2>
+    646c6a32:	test   %rax,%rax
+    646c6a35:	movabs $0x3ff0000000000000,%rdx
+    646c6a3f:	movabs $0x8000000000000000,%rax
+    646c6a49:	cmovns %rdx,%rax
+    646c6a4d:	nopl   (%rax)
+
+00000000646c6a50 <.doret2>:
+    646c6a50:	movq   %rax,%xmm0
+    646c6a55:	ret
+    646c6a56:	cs nopw 0x0(%rax,%rax,1)
+
+00000000646c6a60 <.is_intnaninf>:
+    646c6a60:	cmp    $0x400,%ecx
+    646c6a66:	je     646c6a72 <.ret_naninf>
+    646c6a68:	nopl   0x0(%rax,%rax,1)
+
+00000000646c6a70 <.ret_org>:
+    646c6a70:	repz ret
+
+00000000646c6a72 <.ret_naninf>:
+    646c6a72:	addsd  %xmm0,%xmm0
+    646c6a76:	ret
+    646c6a77:	nop
+    646c6a78:	nop
+    646c6a79:	nop
+    646c6a7a:	nop
+    646c6a7b:	nop
+    646c6a7c:	nop
+    646c6a7d:	nop
+    646c6a7e:	nop
+    646c6a7f:	nop
+
+00000000646c6a80 <cos>:
+    646c6a80:	push   %rbx
+    646c6a81:	sub    $0x70,%rsp
+    646c6a85:	movaps %xmm6,0x60(%rsp)
+    646c6a8a:	movq   %xmm0,%rax
+    646c6a8f:	movq   %xmm0,%rbx
+    646c6a94:	shr    $0x20,%rax
+    646c6a98:	mov    %eax,%edx
+    646c6a9a:	and    $0x7ff00000,%eax
+    646c6a9f:	and    $0xfffff,%edx
+    646c6aa5:	or     %ebx,%edx
+    646c6aa7:	mov    %edx,%ecx
+    646c6aa9:	or     %eax,%ecx
+    646c6aab:	sete   %r8b
+    646c6aaf:	test   %eax,%eax
+    646c6ab1:	sete   %cl
+    646c6ab4:	or     %cl,%r8b
+    646c6ab7:	jne    646c6ac0 <cos+0x40>
+    646c6ab9:	cmp    $0x7ff00000,%eax
+    646c6abe:	je     646c6af5 <cos+0x75>
+    646c6ac0:	mov    %rbx,0x30(%rsp)
+    646c6ac5:	lea    0x50(%rsp),%rcx
+    646c6aca:	fldl   0x30(%rsp)
+    646c6ace:	fstpt  0x40(%rsp)
+    646c6ad2:	lea    0x40(%rsp),%rdx
+    646c6ad7:	call   646c6b80 <__cosl_internal>
+    646c6adc:	fldt   0x50(%rsp)
+    646c6ae0:	fstpl  0x38(%rsp)
+    646c6ae4:	movsd  0x38(%rsp),%xmm0
+    646c6aea:	movaps 0x60(%rsp),%xmm6
+    646c6aef:	add    $0x70,%rsp
+    646c6af3:	pop    %rbx
+    646c6af4:	ret
+    646c6af5:	test   %edx,%edx
+    646c6af7:	jne    646c6b40 <cos+0xc0>
+    646c6af9:	call   646c79d8 <_errno>
+    646c6afe:	movq   %rbx,%xmm2
+    646c6b03:	mov    $0x1,%ecx
+    646c6b08:	movsd  0x2858(%rip),%xmm6        # 646c9368 <.rdata+0x8>
+    646c6b10:	movl   $0x21,(%rax)
+    646c6b16:	lea    0x2843(%rip),%rdx        # 646c9360 <.rdata>
+    646c6b1d:	pxor   %xmm3,%xmm3
+    646c6b21:	movsd  %xmm6,0x20(%rsp)
+    646c6b27:	call   646c7c50 <__mingw_raise_matherr>
+    646c6b2c:	movapd %xmm6,%xmm0
+    646c6b30:	movaps 0x60(%rsp),%xmm6
+    646c6b35:	add    $0x70,%rsp
+    646c6b39:	pop    %rbx
+    646c6b3a:	ret
+    646c6b3b:	nopl   0x0(%rax,%rax,1)
+    646c6b40:	call   646c79d8 <_errno>
+    646c6b45:	movq   %rbx,%xmm2
+    646c6b4a:	mov    $0x1,%ecx
+    646c6b4f:	pxor   %xmm3,%xmm3
+    646c6b53:	movl   $0x21,(%rax)
+    646c6b59:	lea    0x2800(%rip),%rdx        # 646c9360 <.rdata>
+    646c6b60:	mov    %rbx,0x20(%rsp)
+    646c6b65:	call   646c7c50 <__mingw_raise_matherr>
+    646c6b6a:	movq   %rbx,%xmm0
+    646c6b6f:	jmp    646c6aea <cos+0x6a>
+    646c6b74:	nop
+    646c6b75:	nop
+    646c6b76:	nop
+    646c6b77:	nop
+    646c6b78:	nop
+    646c6b79:	nop
+    646c6b7a:	nop
+    646c6b7b:	nop
+    646c6b7c:	nop
+    646c6b7d:	nop
+    646c6b7e:	nop
+    646c6b7f:	nop
+
+00000000646c6b80 <__cosl_internal>:
+    646c6b80:	fldt   (%rdx)
+    646c6b82:	fcos
+    646c6b84:	fnstsw %ax
+    646c6b86:	test   $0x400,%eax
+    646c6b8b:	je     646c6ba2 <__cosl_internal+0x22>
+    646c6b8d:	fldpi
+    646c6b8f:	fadd   %st(0),%st
+    646c6b91:	fxch   %st(1)
+    646c6b93:	fprem1
+    646c6b95:	fnstsw %ax
+    646c6b97:	test   $0x400,%eax
+    646c6b9c:	jne    646c6b93 <__cosl_internal+0x13>
+    646c6b9e:	fstp   %st(1)
+    646c6ba0:	fcos
+    646c6ba2:	mov    %rcx,%rax
+    646c6ba5:	movq   $0x0,0x8(%rcx)
+    646c6bad:	fstpt  (%rcx)
+    646c6baf:	ret
+
+00000000646c6bb0 <exp>:
+    646c6bb0:	push   %rbx
+    646c6bb1:	sub    $0x50,%rsp
+    646c6bb5:	movaps %xmm6,0x40(%rsp)
+    646c6bba:	movsd  0x27be(%rip),%xmm6        # 646c9380 <.rdata+0x10>
+    646c6bc2:	movq   %xmm0,%rdx
+    646c6bc7:	movq   %xmm0,%rbx
+    646c6bcc:	shr    $0x20,%rdx
+    646c6bd0:	mov    %edx,%eax
+    646c6bd2:	mov    %edx,%ecx
+    646c6bd4:	and    $0xfffff,%eax
+    646c6bd9:	and    $0x7ff00000,%ecx
+    646c6bdf:	or     %ebx,%eax
+    646c6be1:	mov    %eax,%r8d
+    646c6be4:	or     %ecx,%r8d
+    646c6be7:	je     646c6c19 <exp+0x69>
+    646c6be9:	cmp    $0x7ff00000,%ecx
+    646c6bef:	je     646c6cb0 <exp+0x100>
+    646c6bf5:	ucomisd 0x278b(%rip),%xmm0        # 646c9388 <.rdata+0x18>
+    646c6bfd:	movapd %xmm0,%xmm1
+    646c6c01:	ja     646c6d02 <exp+0x152>
+    646c6c07:	movsd  0x2781(%rip),%xmm0        # 646c9390 <.rdata+0x20>
+    646c6c0f:	pxor   %xmm6,%xmm6
+    646c6c13:	ucomisd %xmm1,%xmm0
+    646c6c17:	jbe    646c6c30 <exp+0x80>
+    646c6c19:	movapd %xmm6,%xmm0
+    646c6c1d:	movaps 0x40(%rsp),%xmm6
+    646c6c22:	add    $0x50,%rsp
+    646c6c26:	pop    %rbx
+    646c6c27:	ret
+    646c6c28:	nopl   0x0(%rax,%rax,1)
+    646c6c30:	mov    %rbx,0x30(%rsp)
+    646c6c35:	fldl   0x30(%rsp)
+    646c6c39:	fldl2e
+    646c6c3b:	fmul   %st(1),%st
+    646c6c3d:	sub    $0x8,%rsp
+    646c6c41:	fnstcw 0x4(%rsp)
+    646c6c45:	movzwl 0x4(%rsp),%eax
+    646c6c4a:	or     $0xc,%ah
+    646c6c4d:	mov    %ax,(%rsp)
+    646c6c51:	fldcw  (%rsp)
+    646c6c54:	frndint
+    646c6c56:	fld    %st(1)
+    646c6c58:	frndint
+    646c6c5a:	fldcw  0x4(%rsp)
+    646c6c5e:	add    $0x8,%rsp
+    646c6c62:	fld    %st(1)
+    646c6c64:	fldt   0x13d6(%rip)        # 646c8040 <c0>
+    646c6c6a:	fld    %st(2)
+    646c6c6c:	fmul   %st(1),%st
+    646c6c6e:	fsubp  %st,%st(2)
+    646c6c70:	fld    %st(4)
+    646c6c72:	fsub   %st(3),%st
+    646c6c74:	fmulp  %st,%st(1)
+    646c6c76:	faddp  %st,%st(1)
+    646c6c78:	fldt   0x13b2(%rip)        # 646c8030 <c1>
+    646c6c7e:	fmul   %st(4),%st
+    646c6c80:	faddp  %st,%st(1)
+    646c6c82:	f2xm1
+    646c6c84:	fld1
+    646c6c86:	faddp  %st,%st(1)
+    646c6c88:	fstp   %st(1)
+    646c6c8a:	fscale
+    646c6c8c:	fstp   %st(1)
+    646c6c8e:	fstp   %st(1)
+    646c6c90:	fstpl  0x38(%rsp)
+    646c6c94:	movsd  0x38(%rsp),%xmm6
+    646c6c9a:	movapd %xmm6,%xmm0
+    646c6c9e:	movaps 0x40(%rsp),%xmm6
+    646c6ca3:	add    $0x50,%rsp
+    646c6ca7:	pop    %rbx
+    646c6ca8:	ret
+    646c6ca9:	nopl   0x0(%rax)
+    646c6cb0:	test   %eax,%eax
+    646c6cb2:	jne    646c6d60 <exp+0x1b0>
+    646c6cb8:	test   %edx,%edx
+    646c6cba:	js     646c6d44 <exp+0x194>
+    646c6cc0:	call   646c79d8 <_errno>
+    646c6cc5:	movsd  0x26ab(%rip),%xmm6        # 646c9378 <.rdata+0x8>
+    646c6ccd:	mov    $0x4,%ecx
+    646c6cd2:	movl   $0x22,(%rax)
+    646c6cd8:	movsd  %xmm6,0x20(%rsp)
+    646c6cde:	movq   %rbx,%xmm2
+    646c6ce3:	pxor   %xmm3,%xmm3
+    646c6ce7:	lea    0x2682(%rip),%rdx        # 646c9370 <.rdata>
+    646c6cee:	call   646c7c50 <__mingw_raise_matherr>
+    646c6cf3:	movapd %xmm6,%xmm0
+    646c6cf7:	movaps 0x40(%rsp),%xmm6
+    646c6cfc:	add    $0x50,%rsp
+    646c6d00:	pop    %rbx
+    646c6d01:	ret
+    646c6d02:	call   646c79d8 <_errno>
+    646c6d07:	movq   %rbx,%xmm2
+    646c6d0c:	mov    $0x3,%ecx
+    646c6d11:	movsd  0x265f(%rip),%xmm6        # 646c9378 <.rdata+0x8>
+    646c6d19:	movl   $0x22,(%rax)
+    646c6d1f:	lea    0x264a(%rip),%rdx        # 646c9370 <.rdata>
+    646c6d26:	pxor   %xmm3,%xmm3
+    646c6d2a:	movsd  %xmm6,0x20(%rsp)
+    646c6d30:	call   646c7c50 <__mingw_raise_matherr>
+    646c6d35:	movapd %xmm6,%xmm0
+    646c6d39:	movaps 0x40(%rsp),%xmm6
+    646c6d3e:	add    $0x50,%rsp
+    646c6d42:	pop    %rbx
+    646c6d43:	ret
+    646c6d44:	call   646c79d8 <_errno>
+    646c6d49:	pxor   %xmm6,%xmm6
+    646c6d4d:	mov    $0x3,%ecx
+    646c6d52:	movl   $0x22,(%rax)
+    646c6d58:	jmp    646c6cd8 <exp+0x128>
+    646c6d5d:	nopl   (%rax)
+    646c6d60:	call   646c79d8 <_errno>
+    646c6d65:	movq   %rbx,%xmm2
+    646c6d6a:	mov    $0x1,%ecx
+    646c6d6f:	pxor   %xmm3,%xmm3
+    646c6d73:	movl   $0x21,(%rax)
+    646c6d79:	lea    0x25f0(%rip),%rdx        # 646c9370 <.rdata>
+    646c6d80:	movq   %rbx,%xmm6
+    646c6d85:	mov    %rbx,0x20(%rsp)
+    646c6d8a:	call   646c7c50 <__mingw_raise_matherr>
+    646c6d8f:	jmp    646c6c19 <exp+0x69>
+    646c6d94:	nop
+    646c6d95:	nop
+    646c6d96:	nop
+    646c6d97:	nop
+    646c6d98:	nop
+    646c6d99:	nop
+    646c6d9a:	nop
+    646c6d9b:	nop
+    646c6d9c:	nop
+    646c6d9d:	nop
+    646c6d9e:	nop
+    646c6d9f:	nop
+
+00000000646c6da0 <log>:
+    646c6da0:	push   %rbx
+    646c6da1:	sub    $0x70,%rsp
+    646c6da5:	movaps %xmm6,0x60(%rsp)
+    646c6daa:	movq   %xmm0,%rdx
+    646c6daf:	movq   %xmm0,%rbx
+    646c6db4:	shr    $0x20,%rdx
+    646c6db8:	mov    %edx,%eax
+    646c6dba:	mov    %edx,%ecx
+    646c6dbc:	and    $0xfffff,%eax
+    646c6dc1:	and    $0x7ff00000,%ecx
+    646c6dc7:	or     %ebx,%eax
+    646c6dc9:	mov    %eax,%r8d
+    646c6dcc:	or     %ecx,%r8d
+    646c6dcf:	je     646c6e30 <log+0x90>
+    646c6dd1:	test   %ecx,%ecx
+    646c6dd3:	jne    646c6e12 <log+0x72>
+    646c6dd5:	test   %edx,%edx
+    646c6dd7:	js     646c6e7e <log+0xde>
+    646c6ddd:	mov    %rbx,0x30(%rsp)
+    646c6de2:	lea    0x50(%rsp),%rcx
+    646c6de7:	fldl   0x30(%rsp)
+    646c6deb:	fstpt  0x40(%rsp)
+    646c6def:	lea    0x40(%rsp),%rdx
+    646c6df4:	call   646c77c0 <__logl_internal>
+    646c6df9:	fldt   0x50(%rsp)
+    646c6dfd:	fstpl  0x38(%rsp)
+    646c6e01:	movsd  0x38(%rsp),%xmm0
+    646c6e07:	movaps 0x60(%rsp),%xmm6
+    646c6e0c:	add    $0x70,%rsp
+    646c6e10:	pop    %rbx
+    646c6e11:	ret
+    646c6e12:	cmp    $0x7ff00000,%ecx
+    646c6e18:	jne    646c6dd5 <log+0x35>
+    646c6e1a:	test   %eax,%eax
+    646c6e1c:	je     646c6e72 <log+0xd2>
+    646c6e1e:	test   %edx,%edx
+    646c6e20:	js     646c6e7e <log+0xde>
+    646c6e22:	movsd  0x2586(%rip),%xmm0        # 646c93b0 <.rdata+0x10>
+    646c6e2a:	jmp    646c6e07 <log+0x67>
+    646c6e2c:	nopl   0x0(%rax)
+    646c6e30:	call   646c79d8 <_errno>
+    646c6e35:	movq   %rbx,%xmm2
+    646c6e3a:	mov    $0x3,%ecx
+    646c6e3f:	movsd  0x2561(%rip),%xmm6        # 646c93a8 <.rdata+0x8>
+    646c6e47:	movl   $0x22,(%rax)
+    646c6e4d:	lea    0x254c(%rip),%rdx        # 646c93a0 <.rdata>
+    646c6e54:	pxor   %xmm3,%xmm3
+    646c6e58:	movsd  %xmm6,0x20(%rsp)
+    646c6e5e:	call   646c7c50 <__mingw_raise_matherr>
+    646c6e63:	movapd %xmm6,%xmm0
+    646c6e67:	movaps 0x60(%rsp),%xmm6
+    646c6e6c:	add    $0x70,%rsp
+    646c6e70:	pop    %rbx
+    646c6e71:	ret
+    646c6e72:	test   %edx,%edx
+    646c6e74:	movsd  0x253c(%rip),%xmm0        # 646c93b8 <.rdata+0x18>
+    646c6e7c:	jns    646c6e07 <log+0x67>
+    646c6e7e:	call   646c79d8 <_errno>
+    646c6e83:	movq   %rbx,%xmm2
+    646c6e88:	mov    $0x1,%ecx
+    646c6e8d:	movsd  0x251b(%rip),%xmm6        # 646c93b0 <.rdata+0x10>
+    646c6e95:	movl   $0x21,(%rax)
+    646c6e9b:	lea    0x24fe(%rip),%rdx        # 646c93a0 <.rdata>
+    646c6ea2:	pxor   %xmm3,%xmm3
+    646c6ea6:	movsd  %xmm6,0x20(%rsp)
+    646c6eac:	call   646c7c50 <__mingw_raise_matherr>
+    646c6eb1:	movapd %xmm6,%xmm0
+    646c6eb5:	movaps 0x60(%rsp),%xmm6
+    646c6eba:	add    $0x70,%rsp
+    646c6ebe:	pop    %rbx
+    646c6ebf:	ret
+
+00000000646c6ec0 <internal_modf>:
+    646c6ec0:	sub    $0x18,%rsp
+    646c6ec4:	movsd  %xmm0,0x8(%rsp)
+    646c6eca:	fldl   0x8(%rsp)
+    646c6ece:	push   %rax
+    646c6ecf:	sub    $0x8,%rsp
+    646c6ed3:	fnstcw 0x4(%rsp)
+    646c6ed7:	movzwl 0x4(%rsp),%eax
+    646c6edc:	or     $0xc,%ah
+    646c6edf:	mov    %ax,(%rsp)
+    646c6ee3:	fldcw  (%rsp)
+    646c6ee6:	frndint
+    646c6ee8:	fldcw  0x4(%rsp)
+    646c6eec:	add    $0x8,%rsp
+    646c6ef0:	pop    %rax
+    646c6ef1:	movq   %xmm0,%rax
+    646c6ef6:	fstpl  0x8(%rsp)
+    646c6efa:	movsd  0x8(%rsp),%xmm1
+    646c6f00:	shr    $0x20,%rax
+    646c6f04:	mov    %eax,%ecx
+    646c6f06:	movsd  %xmm1,(%rdx)
+    646c6f0a:	movq   %xmm0,%rdx
+    646c6f0f:	and    $0x7ff00000,%eax
+    646c6f14:	and    $0xfffff,%ecx
+    646c6f1a:	or     %edx,%ecx
+    646c6f1c:	mov    %ecx,%edx
+    646c6f1e:	or     %eax,%edx
+    646c6f20:	sete   %dl
+    646c6f23:	test   %eax,%eax
+    646c6f25:	sete   %r8b
+    646c6f29:	or     %r8d,%edx
+    646c6f2c:	xor    $0x1,%edx
+    646c6f2f:	cmp    $0x7ff00000,%eax
+    646c6f34:	sete   %al
+    646c6f37:	test   %al,%dl
+    646c6f39:	je     646c6f3f <internal_modf+0x7f>
+    646c6f3b:	test   %ecx,%ecx
+    646c6f3d:	je     646c6f50 <internal_modf+0x90>
+    646c6f3f:	subsd  0x8(%rsp),%xmm0
+    646c6f45:	add    $0x18,%rsp
+    646c6f49:	ret
+    646c6f4a:	nopw   0x0(%rax,%rax,1)
+    646c6f50:	pxor   %xmm0,%xmm0
+    646c6f54:	jmp    646c6f45 <internal_modf+0x85>
+    646c6f56:	cs nopw 0x0(%rax,%rax,1)
+
+00000000646c6f60 <pow>:
+    646c6f60:	push   %r12
+    646c6f62:	push   %rbp
+    646c6f63:	push   %rdi
+    646c6f64:	push   %rsi
+    646c6f65:	push   %rbx
+    646c6f66:	sub    $0x90,%rsp
+    646c6f6d:	movaps %xmm6,0x70(%rsp)
+    646c6f72:	movaps %xmm7,0x80(%rsp)
+    646c6f7a:	mov    $0x4000,%edx
+    646c6f7f:	movq   %xmm0,%rbx
+    646c6f84:	movq   %xmm0,%rdi
+    646c6f89:	movq   %xmm1,%rbp
+    646c6f8e:	shr    $0x20,%rbx
+    646c6f92:	mov    %ebx,%eax
+    646c6f94:	mov    %ebx,%ecx
+    646c6f96:	and    $0xfffff,%eax
+    646c6f9b:	and    $0x7ff00000,%ecx
+    646c6fa1:	or     %edi,%eax
+    646c6fa3:	mov    %ecx,%esi
+    646c6fa5:	or     %eax,%esi
+    646c6fa7:	je     646c6fb6 <pow+0x56>
+    646c6fa9:	test   %ecx,%ecx
+    646c6fab:	mov    $0x4400,%edx
+    646c6fb0:	jne    646c7101 <pow+0x1a1>
+    646c6fb6:	mov    %rbp,%rsi
+    646c6fb9:	movsd  0x242f(%rip),%xmm6        # 646c93f0 <.rdata+0x30>
+    646c6fc1:	shr    $0x20,%rsi
+    646c6fc5:	mov    %esi,%eax
+    646c6fc7:	mov    %esi,%ecx
+    646c6fc9:	and    $0xfffff,%eax
+    646c6fce:	and    $0x7ff00000,%ecx
+    646c6fd4:	or     %ebp,%eax
+    646c6fd6:	mov    %ecx,%r9d
+    646c6fd9:	or     %eax,%r9d
+    646c6fdc:	je     646c706b <pow+0x10b>
+    646c6fe2:	test   %ecx,%ecx
+    646c6fe4:	jne    646c7090 <pow+0x130>
+    646c6fea:	mov    $0x4400,%r8d
+    646c6ff0:	movsd  0x23f8(%rip),%xmm2        # 646c93f0 <.rdata+0x30>
+    646c6ff8:	movq   %rdi,%xmm4
+    646c6ffd:	ucomisd %xmm2,%xmm4
+    646c7001:	jp     646c7009 <pow+0xa9>
+    646c7003:	je     646c7458 <pow+0x4f8>
+    646c7009:	cmp    $0x100,%edx
+    646c700f:	je     646c70c0 <pow+0x160>
+    646c7015:	cmp    $0x4000,%edx
+    646c701b:	je     646c7130 <pow+0x1d0>
+    646c7021:	cmp    $0x500,%r8d
+    646c7028:	je     646c7180 <pow+0x220>
+    646c702e:	cmp    $0x500,%edx
+    646c7034:	jne    646c71a5 <pow+0x245>
+    646c703a:	test   %ebx,%ebx
+    646c703c:	js     646c7341 <pow+0x3e1>
+    646c7042:	mov    $0xffffffff,%edx
+    646c7047:	movq   %rbp,%xmm0
+    646c704c:	call   646c7810 <ldexp>
+    646c7051:	lea    0x68(%rsp),%rdx
+    646c7056:	call   646c6ec0 <internal_modf>
+    646c705b:	test   %esi,%esi
+    646c705d:	js     646c7162 <pow+0x202>
+    646c7063:	movsd  0x237d(%rip),%xmm6        # 646c93e8 <.rdata+0x28>
+    646c706b:	movapd %xmm6,%xmm0
+    646c706f:	movaps 0x80(%rsp),%xmm7
+    646c7077:	movaps 0x70(%rsp),%xmm6
+    646c707c:	add    $0x90,%rsp
+    646c7083:	pop    %rbx
+    646c7084:	pop    %rsi
+    646c7085:	pop    %rdi
+    646c7086:	pop    %rbp
+    646c7087:	pop    %r12
+    646c7089:	ret
+    646c708a:	nopw   0x0(%rax,%rax,1)
+    646c7090:	cmp    $0x7ff00000,%ecx
+    646c7096:	mov    $0x400,%r8d
+    646c709c:	jne    646c6ff0 <pow+0x90>
+    646c70a2:	test   %eax,%eax
+    646c70a4:	mov    $0x500,%r8d
+    646c70aa:	je     646c6ff0 <pow+0x90>
+    646c70b0:	movq   %rdi,%xmm5
+    646c70b5:	ucomisd %xmm6,%xmm5
+    646c70b9:	jp     646c70c0 <pow+0x160>
+    646c70bb:	je     646c706b <pow+0x10b>
+    646c70bd:	nopl   (%rax)
+    646c70c0:	test   %ebx,%ebx
+    646c70c2:	movsd  0x2306(%rip),%xmm6        # 646c93d0 <.rdata+0x10>
+    646c70ca:	js     646c7170 <pow+0x210>
+    646c70d0:	call   646c79d8 <_errno>
+    646c70d5:	movl   $0x21,(%rax)
+    646c70db:	movsd  %xmm6,0x20(%rsp)
+    646c70e1:	movq   %rbp,%xmm3
+    646c70e6:	movq   %rdi,%xmm2
+    646c70eb:	mov    $0x1,%ecx
+    646c70f0:	lea    0x22c9(%rip),%rdx        # 646c93c0 <.rdata>
+    646c70f7:	call   646c7c50 <__mingw_raise_matherr>
+    646c70fc:	jmp    646c706b <pow+0x10b>
+    646c7101:	cmp    $0x7ff00000,%ecx
+    646c7107:	mov    $0x400,%edx
+    646c710c:	jne    646c6fb6 <pow+0x56>
+    646c7112:	cmp    $0x1,%eax
+    646c7115:	sbb    %edx,%edx
+    646c7117:	and    $0x400,%edx
+    646c711d:	add    $0x100,%edx
+    646c7123:	jmp    646c6fb6 <pow+0x56>
+    646c7128:	nopl   0x0(%rax,%rax,1)
+    646c7130:	cmp    $0x500,%r8d
+    646c7137:	je     646c715a <pow+0x1fa>
+    646c7139:	test   %ebx,%ebx
+    646c713b:	js     646c7300 <pow+0x3a0>
+    646c7141:	mov    $0xffffffff,%edx
+    646c7146:	movq   %rbp,%xmm0
+    646c714b:	call   646c7810 <ldexp>
+    646c7150:	lea    0x68(%rsp),%rdx
+    646c7155:	call   646c6ec0 <internal_modf>
+    646c715a:	test   %esi,%esi
+    646c715c:	js     646c7063 <pow+0x103>
+    646c7162:	pxor   %xmm6,%xmm6
+    646c7166:	jmp    646c706b <pow+0x10b>
+    646c716b:	nopl   0x0(%rax,%rax,1)
+    646c7170:	movsd  0x2250(%rip),%xmm6        # 646c93c8 <.rdata+0x8>
+    646c7178:	jmp    646c70d0 <pow+0x170>
+    646c717d:	nopl   (%rax)
+    646c7180:	cmp    $0x500,%edx
+    646c7186:	je     646c705b <pow+0xfb>
+    646c718c:	test   %ebx,%ebx
+    646c718e:	js     646c7435 <pow+0x4d5>
+    646c7194:	movq   %rdi,%xmm5
+    646c7199:	ucomisd %xmm2,%xmm5
+    646c719d:	ja     646c705b <pow+0xfb>
+    646c71a3:	jmp    646c715a <pow+0x1fa>
+    646c71a5:	lea    0x68(%rsp),%rsi
+    646c71aa:	movq   %rbp,%xmm0
+    646c71af:	pxor   %xmm7,%xmm7
+    646c71b3:	mov    %rsi,%rdx
+    646c71b6:	call   646c6ec0 <internal_modf>
+    646c71bb:	ucomisd %xmm7,%xmm0
+    646c71bf:	jp     646c7281 <pow+0x321>
+    646c71c5:	jne    646c7281 <pow+0x321>
+    646c71cb:	movsd  0x68(%rsp),%xmm0
+    646c71d1:	movsd  0x2247(%rip),%xmm1        # 646c9420 <.rdata+0x60>
+    646c71d9:	ucomisd %xmm0,%xmm1
+    646c71dd:	jb     646c71ed <pow+0x28d>
+    646c71df:	ucomisd 0x2241(%rip),%xmm0        # 646c9428 <.rdata+0x68>
+    646c71e7:	jae    646c7493 <pow+0x533>
+    646c71ed:	lea    0x50(%rsp),%r12
+    646c71f2:	movq   %rdi,%xmm5
+    646c71f7:	andpd  0x2231(%rip),%xmm5        # 646c9430 <.rdata+0x70>
+    646c71ff:	movsd  %xmm5,0x30(%rsp)
+    646c7205:	lea    0x40(%rsp),%rdi
+    646c720a:	fldl   0x30(%rsp)
+    646c720e:	mov    %r12,%rcx
+    646c7211:	fstpt  0x40(%rsp)
+    646c7215:	mov    %rdi,%rdx
+    646c7218:	call   646c78e0 <log2l>
+    646c721d:	mov    %rdi,%rdx
+    646c7220:	mov    %r12,%rcx
+    646c7223:	fldt   0x50(%rsp)
+    646c7227:	mov    %rbp,0x30(%rsp)
+    646c722c:	fldl   0x30(%rsp)
+    646c7230:	fmulp  %st,%st(1)
     646c7232:	fstpt  0x40(%rsp)
-    646c7236:	mov    %rsi,%rdx
-    646c7239:	call   646c7850 <log2l>
-    646c723e:	mov    %rsi,%rdx
-    646c7241:	mov    %rbx,%rcx
-    646c7244:	fldt   0x50(%rsp)
-    646c7248:	mov    %rbp,0x30(%rsp)
-    646c724d:	fldl   0x30(%rsp)
-    646c7251:	fmulp  %st,%st(1)
-    646c7253:	fstpt  0x40(%rsp)
-    646c7257:	call   646c76b0 <exp2l>
-    646c725c:	fldt   0x50(%rsp)
-    646c7260:	fstpl  0x38(%rsp)
-    646c7264:	movsd  0x38(%rsp),%xmm6
-    646c726a:	jmp    646c6fdb <pow+0x10b>
-    646c726f:	nop
-    646c7270:	lea    0x68(%rsp),%rbx
-    646c7275:	movq   %rbp,%xmm0
-    646c727a:	pxor   %xmm7,%xmm7
-    646c727e:	mov    %rbx,%rdx
-    646c7281:	call   646c6e30 <internal_modf>
-    646c7286:	ucomisd %xmm7,%xmm0
-    646c728a:	jp     646c7292 <pow+0x3c2>
-    646c728c:	je     646c7371 <pow+0x4a1>
-    646c7292:	test   %esi,%esi
-    646c7294:	jns    646c70d2 <pow+0x202>
-    646c729a:	btc    $0x3f,%rdi
-    646c729f:	movq   %rdi,%xmm5
-    646c72a4:	divsd  %xmm5,%xmm2
-    646c72a8:	movapd %xmm2,%xmm6
-    646c72ac:	jmp    646c6fdb <pow+0x10b>
-    646c72b1:	lea    0x68(%rsp),%rbx
-    646c72b6:	movq   %rbp,%xmm0
-    646c72bb:	pxor   %xmm7,%xmm7
-    646c72bf:	mov    %rbx,%rdx
-    646c72c2:	call   646c6e30 <internal_modf>
-    646c72c7:	ucomisd %xmm7,%xmm0
-    646c72cb:	jp     646c72cf <pow+0x3ff>
-    646c72cd:	je     646c72f1 <pow+0x421>
-    646c72cf:	test   %esi,%esi
-    646c72d1:	movq   %rdi,%xmm6
-    646c72d6:	xorpd  0x2122(%rip),%xmm6        # 646c9400 <.rdata+0x40>
-    646c72de:	jns    646c6fdb <pow+0x10b>
-    646c72e4:	divsd  %xmm6,%xmm2
-    646c72e8:	movapd %xmm2,%xmm6
-    646c72ec:	jmp    646c6fdb <pow+0x10b>
-    646c72f1:	mov    $0xffffffff,%edx
-    646c72f6:	movq   %rbp,%xmm0
-    646c72fb:	call   646c7780 <ldexp>
-    646c7300:	mov    %rbx,%rdx
-    646c7303:	call   646c6e30 <internal_modf>
-    646c7308:	mov    $0x0,%edx
-    646c730d:	ucomisd %xmm7,%xmm0
-    646c7311:	setnp  %al
-    646c7314:	cmovne %edx,%eax
-    646c7317:	mov    %esi,%edx
-    646c7319:	shr    $0x1f,%edx
-    646c731c:	test   %dl,%dl
-    646c731e:	je     646c7328 <pow+0x458>
-    646c7320:	test   %al,%al
-    646c7322:	jne    646c70d2 <pow+0x202>
-    646c7328:	mov    %esi,%edx
-    646c732a:	mov    $0x1,%r8d
-    646c7330:	not    %edx
-    646c7332:	shr    $0x1f,%edx
-    646c7335:	ucomisd %xmm7,%xmm0
-    646c7339:	setp   %cl
-    646c733c:	cmovne %r8d,%ecx
-    646c7340:	test   %cl,%cl
-    646c7342:	je     646c7348 <pow+0x478>
-    646c7344:	test   %dl,%dl
-    646c7346:	jne    646c7364 <pow+0x494>
-    646c7348:	test   %al,%al
-    646c734a:	je     646c7354 <pow+0x484>
-    646c734c:	test   %dl,%dl
-    646c734e:	jne    646c6fd3 <pow+0x103>
-    646c7354:	test   %esi,%esi
-    646c7356:	js     646c738c <pow+0x4bc>
-    646c7358:	ucomisd %xmm7,%xmm0
-    646c735c:	jp     646c7364 <pow+0x494>
-    646c735e:	je     646c6fd3 <pow+0x103>
-    646c7364:	movsd  0x2074(%rip),%xmm6        # 646c93e0 <.rdata+0x20>
-    646c736c:	jmp    646c6fdb <pow+0x10b>
-    646c7371:	mov    $0xffffffff,%edx
-    646c7376:	movq   %rbp,%xmm0
-    646c737b:	call   646c7780 <ldexp>
-    646c7380:	mov    %rbx,%rdx
-    646c7383:	call   646c6e30 <internal_modf>
-    646c7388:	test   %esi,%esi
-    646c738a:	js     646c7358 <pow+0x488>
-    646c738c:	ucomisd %xmm7,%xmm0
-    646c7390:	jp     646c7398 <pow+0x4c8>
-    646c7392:	je     646c70d2 <pow+0x202>
-    646c7398:	movsd  0x2038(%rip),%xmm6        # 646c93d8 <.rdata+0x18>
-    646c73a0:	jmp    646c6fdb <pow+0x10b>
-    646c73a5:	movq   %rdi,%xmm5
-    646c73aa:	xorpd  0x204e(%rip),%xmm5        # 646c9400 <.rdata+0x40>
-    646c73b2:	movq   %xmm5,%rax
-    646c73b7:	movq   %rdi,%xmm5
-    646c73bc:	ucomisd 0x204c(%rip),%xmm5        # 646c9410 <.rdata+0x50>
-    646c73c4:	jp     646c741f <pow+0x54f>
-    646c73c6:	jne    646c741f <pow+0x54f>
-    646c73c8:	movapd %xmm2,%xmm6
-    646c73cc:	jmp    646c6fdb <pow+0x10b>
-    646c73d1:	mov    %rdi,0x30(%rsp)
-    646c73d6:	fldl   0x30(%rsp)
-    646c73da:	fsqrt
-    646c73dc:	fstpl  0x30(%rsp)
-    646c73e0:	movsd  0x30(%rsp),%xmm6
-    646c73e6:	jmp    646c6fdb <pow+0x10b>
-    646c73eb:	call   646c7948 <_errno>
-    646c73f0:	movsd  0x1fd0(%rip),%xmm6        # 646c93c8 <.rdata+0x8>
-    646c73f8:	movl   $0x21,(%rax)
-    646c73fe:	jmp    646c704b <pow+0x17b>
-    646c7403:	movq   %rbp,%xmm3
-    646c7408:	movq   %rdi,%xmm0
-    646c740d:	cvttsd2si %xmm3,%edx
-    646c7411:	call   646c7430 <__powi>
-    646c7416:	movapd %xmm0,%xmm6
-    646c741a:	jmp    646c6fdb <pow+0x10b>
-    646c741f:	mov    %rax,%rdi
-    646c7422:	jmp    646c7104 <pow+0x234>
-    646c7427:	nop
-    646c7428:	nop
-    646c7429:	nop
-    646c742a:	nop
-    646c742b:	nop
-    646c742c:	nop
-    646c742d:	nop
-    646c742e:	nop
-    646c742f:	nop
-
-00000000646c7430 <__powi>:
-    646c7430:	sub    $0x58,%rsp
-    646c7434:	movaps %xmm6,0x40(%rsp)
-    646c7439:	movsd  0x2017(%rip),%xmm1        # 646c9458 <.rdata+0x18>
-    646c7441:	mov    $0x0,%r10d
-    646c7447:	movq   %xmm0,%r8
-    646c744c:	movq   %xmm0,%rax
-    646c7451:	shr    $0x20,%r8
-    646c7455:	mov    %r8d,%ecx
-    646c7458:	mov    %r8d,%r9d
-    646c745b:	and    $0xfffff,%ecx
-    646c7461:	and    $0x7ff00000,%r9d
-    646c7468:	or     %eax,%ecx
-    646c746a:	ucomisd %xmm1,%xmm0
-    646c746e:	mov    %r9d,%r11d
-    646c7471:	setnp  %al
-    646c7474:	cmovne %r10d,%eax
-    646c7478:	test   %edx,%edx
-    646c747a:	sete   %r10b
-    646c747e:	or     %r10d,%eax
-    646c7481:	or     %ecx,%r11d
-    646c7484:	jne    646c74c0 <__powi+0x90>
-    646c7486:	test   %al,%al
-    646c7488:	movapd %xmm1,%xmm6
-    646c748c:	jne    646c74b0 <__powi+0x80>
-    646c748e:	mov    %edx,%eax
-    646c7490:	and    $0x1,%eax
-    646c7493:	test   %edx,%edx
-    646c7495:	js     646c7585 <__powi+0x155>
-    646c749b:	test   %eax,%eax
-    646c749d:	pxor   %xmm6,%xmm6
-    646c74a1:	je     646c74b0 <__powi+0x80>
-    646c74a3:	test   %r8d,%r8d
-    646c74a6:	jns    646c74b0 <__powi+0x80>
-    646c74a8:	movsd  0x1fb0(%rip),%xmm6        # 646c9460 <.rdata+0x20>
-    646c74b0:	movapd %xmm6,%xmm0
-    646c74b4:	movaps 0x40(%rsp),%xmm6
-    646c74b9:	add    $0x58,%rsp
-    646c74bd:	ret
-    646c74be:	xchg   %ax,%ax
-    646c74c0:	test   %r9d,%r9d
-    646c74c3:	jne    646c7530 <__powi+0x100>
-    646c74c5:	test   %al,%al
-    646c74c7:	movapd %xmm1,%xmm6
-    646c74cb:	jne    646c74b0 <__powi+0x80>
-    646c74cd:	mov    %edx,%eax
-    646c74cf:	movapd %xmm0,%xmm6
-    646c74d3:	andpd  0x1fa5(%rip),%xmm6        # 646c9480 <.rdata+0x40>
-    646c74db:	and    $0x1,%eax
-    646c74de:	test   %edx,%edx
-    646c74e0:	js     646c7572 <__powi+0x142>
-    646c74e6:	cmp    $0x1,%edx
-    646c74e9:	je     646c7511 <__powi+0xe1>
-    646c74eb:	test   $0x1,%dl
-    646c74ee:	jne    646c7620 <__powi+0x1f0>
-    646c74f4:	movapd %xmm6,%xmm0
-    646c74f8:	shr    %edx
-    646c74fa:	movapd %xmm1,%xmm6
-    646c74fe:	xchg   %ax,%ax
-    646c7500:	mulsd  %xmm0,%xmm0
-    646c7504:	test   $0x1,%dl
-    646c7507:	je     646c750d <__powi+0xdd>
-    646c7509:	mulsd  %xmm0,%xmm6
-    646c750d:	shr    %edx
-    646c750f:	jne    646c7500 <__powi+0xd0>
-    646c7511:	shr    $0x1f,%r8d
-    646c7515:	test   %r8b,%r8b
-    646c7518:	je     646c74b0 <__powi+0x80>
-    646c751a:	test   %eax,%eax
-    646c751c:	je     646c74b0 <__powi+0x80>
-    646c751e:	xorpd  0x1f6a(%rip),%xmm6        # 646c9490 <.rdata+0x50>
-    646c7526:	jmp    646c74b0 <__powi+0x80>
-    646c7528:	nopl   0x0(%rax,%rax,1)
-    646c7530:	cmp    $0x7ff00000,%r9d
-    646c7537:	jne    646c74c5 <__powi+0x95>
-    646c7539:	test   %ecx,%ecx
-    646c753b:	jne    646c75b0 <__powi+0x180>
-    646c753d:	mov    %edx,%r9d
-    646c7540:	movapd %xmm1,%xmm6
-    646c7544:	and    $0x1,%r9d
-    646c7548:	test   %al,%al
-    646c754a:	jne    646c74b0 <__powi+0x80>
-    646c7550:	test   %r8d,%r8d
-    646c7553:	js     646c7640 <__powi+0x210>
-    646c7559:	test   %edx,%edx
-    646c755b:	movsd  0x1f05(%rip),%xmm6        # 646c9468 <.rdata+0x28>
-    646c7563:	jns    646c74b0 <__powi+0x80>
-    646c7569:	pxor   %xmm6,%xmm6
-    646c756d:	jmp    646c74b0 <__powi+0x80>
-    646c7572:	movapd %xmm1,%xmm4
-    646c7576:	neg    %edx
-    646c7578:	divsd  %xmm6,%xmm4
-    646c757c:	movapd %xmm4,%xmm6
-    646c7580:	jmp    646c74e6 <__powi+0xb6>
-    646c7585:	test   %eax,%eax
-    646c7587:	movsd  0x1ed9(%rip),%xmm6        # 646c9468 <.rdata+0x28>
-    646c758f:	je     646c74b0 <__powi+0x80>
-    646c7595:	test   %r8d,%r8d
-    646c7598:	jns    646c74b0 <__powi+0x80>
-    646c759e:	movsd  0x1eca(%rip),%xmm6        # 646c9470 <.rdata+0x30>
-    646c75a6:	jmp    646c74b0 <__powi+0x80>
-    646c75ab:	nopl   0x0(%rax,%rax,1)
-    646c75b0:	test   %al,%al
-    646c75b2:	movapd %xmm1,%xmm6
-    646c75b6:	jne    646c74b0 <__powi+0x80>
-    646c75bc:	test   %r8d,%r8d
-    646c75bf:	movsd  0x1e89(%rip),%xmm6        # 646c9450 <.rdata+0x10>
-    646c75c7:	js     646c7630 <__powi+0x200>
-    646c75c9:	mov    %edx,0x3c(%rsp)
-    646c75cd:	movsd  %xmm0,0x30(%rsp)
-    646c75d3:	call   646c7948 <_errno>
-    646c75d8:	mov    0x3c(%rsp),%edx
-    646c75dc:	pxor   %xmm3,%xmm3
-    646c75e0:	mov    $0x1,%ecx
-    646c75e5:	movsd  0x30(%rsp),%xmm0
-    646c75eb:	movl   $0x21,(%rax)
-    646c75f1:	movsd  %xmm6,0x20(%rsp)
-    646c75f7:	movapd %xmm0,%xmm2
-    646c75fb:	cvtsi2sd %edx,%xmm3
-    646c75ff:	lea    0x1e3a(%rip),%rdx        # 646c9440 <.rdata>
-    646c7606:	call   646c7bc0 <__mingw_raise_matherr>
-    646c760b:	movapd %xmm6,%xmm0
-    646c760f:	movaps 0x40(%rsp),%xmm6
-    646c7614:	add    $0x58,%rsp
-    646c7618:	ret
-    646c7619:	nopl   0x0(%rax)
-    646c7620:	movapd %xmm6,%xmm1
-    646c7624:	jmp    646c74f4 <__powi+0xc4>
-    646c7629:	nopl   0x0(%rax)
-    646c7630:	movsd  0x1e10(%rip),%xmm6        # 646c9448 <.rdata+0x8>
-    646c7638:	jmp    646c75c9 <__powi+0x199>
-    646c763a:	nopw   0x0(%rax,%rax,1)
-    646c7640:	mov    %edx,%eax
-    646c7642:	not    %eax
-    646c7644:	mov    %eax,%ecx
-    646c7646:	and    $0x1,%ecx
-    646c7649:	test   %edx,%edx
-    646c764b:	jns    646c7659 <__powi+0x229>
-    646c764d:	test   %cl,%cl
-    646c764f:	pxor   %xmm6,%xmm6
-    646c7653:	jne    646c74b0 <__powi+0x80>
-    646c7659:	shr    $0x1f,%eax
-    646c765c:	test   $0x1,%dl
-    646c765f:	je     646c7671 <__powi+0x241>
-    646c7661:	test   %al,%al
-    646c7663:	movsd  0x1e05(%rip),%xmm6        # 646c9470 <.rdata+0x30>
-    646c766b:	jne    646c74b0 <__powi+0x80>
-    646c7671:	test   %cl,%cl
-    646c7673:	je     646c7685 <__powi+0x255>
-    646c7675:	test   %al,%al
-    646c7677:	movsd  0x1de9(%rip),%xmm6        # 646c9468 <.rdata+0x28>
-    646c767f:	jne    646c74b0 <__powi+0x80>
-    646c7685:	test   %edx,%edx
-    646c7687:	js     646c76a0 <__powi+0x270>
-    646c7689:	and    $0x1,%dl
-    646c768c:	jne    646c759e <__powi+0x16e>
-    646c7692:	movsd  0x1dce(%rip),%xmm6        # 646c9468 <.rdata+0x28>
-    646c769a:	jmp    646c74b0 <__powi+0x80>
-    646c769f:	nop
-    646c76a0:	test   %r9d,%r9d
-    646c76a3:	jne    646c74a8 <__powi+0x78>
-    646c76a9:	jmp    646c7569 <__powi+0x139>
-    646c76ae:	nop
-    646c76af:	nop
-
-00000000646c76b0 <exp2l>:
-    646c76b0:	fldt   (%rdx)
-    646c76b2:	fxam
-    646c76b4:	fstsw  %ax
-    646c76b7:	mov    $0x45,%dh
-    646c76b9:	and    %ah,%dh
-    646c76bb:	cmp    $0x5,%dh
-    646c76be:	je     646c76ff <exp2l+0x4f>
-    646c76c0:	fld    %st(0)
-    646c76c2:	sub    $0x8,%rsp
-    646c76c6:	fnstcw 0x4(%rsp)
-    646c76ca:	movzwl 0x4(%rsp),%eax
-    646c76cf:	or     $0xc,%ah
-    646c76d2:	mov    %ax,(%rsp)
-    646c76d6:	fldcw  (%rsp)
-    646c76d9:	frndint
-    646c76db:	fldcw  0x4(%rsp)
-    646c76df:	add    $0x8,%rsp
-    646c76e3:	fsubr  %st,%st(1)
-    646c76e5:	fxch   %st(1)
-    646c76e7:	f2xm1
-    646c76e9:	fld1
-    646c76eb:	faddp  %st,%st(1)
-    646c76ed:	fscale
-    646c76ef:	fstp   %st(1)
-    646c76f1:	mov    %rcx,%rax
-    646c76f4:	movq   $0x0,0x8(%rcx)
-    646c76fc:	fstpt  (%rcx)
-    646c76fe:	ret
-    646c76ff:	test   $0x200,%eax
-    646c7704:	je     646c770a <exp2l+0x5a>
-    646c7706:	fstp   %st(0)
-    646c7708:	fldz
-    646c770a:	mov    %rcx,%rax
-    646c770d:	movq   $0x0,0x8(%rcx)
-    646c7715:	fstpt  (%rcx)
-    646c7717:	ret
-    646c7718:	nop
-    646c7719:	nop
-    646c771a:	nop
-    646c771b:	nop
-    646c771c:	nop
-    646c771d:	nop
-    646c771e:	nop
-    646c771f:	nop
-
-00000000646c7720 <one>:
-    646c7720:	add    %al,(%rax)
-    646c7722:	add    %al,(%rax)
-    646c7724:	add    %al,(%rax)
-    646c7726:	lock (bad)
-
-00000000646c7728 <limit>:
-    646c7728:	pop    %rdx
-    646c772a:	cmc
-    646c772b:	sub    %bl,-0x2e(%rdi,%rcx,4)
-    646c772f:	(bad)
-
-00000000646c7730 <__logl_internal>:
-    646c7730:	fldln2
-    646c7732:	fldt   (%rdx)
-    646c7734:	fld    %st(0)
-    646c7736:	fsubl  -0x1c(%rip)        # 646c7720 <one>
-    646c773c:	fld    %st(0)
-    646c773e:	fabs
-    646c7740:	fcompl -0x1e(%rip)        # 646c7728 <limit>
-    646c7746:	fnstsw %ax
-    646c7748:	and    $0x45,%ah
-    646c774b:	je     646c775f <__logl_internal+0x2f>
-    646c774d:	fstp   %st(1)
-    646c774f:	fyl2xp1
-    646c7751:	mov    %rcx,%rax
-    646c7754:	movq   $0x0,0x8(%rcx)
-    646c775c:	fstpt  (%rcx)
-    646c775e:	ret
-    646c775f:	fstp   %st(0)
-    646c7761:	fyl2x
-    646c7763:	mov    %rcx,%rax
-    646c7766:	movq   $0x0,0x8(%rcx)
-    646c776e:	fstpt  (%rcx)
-    646c7770:	ret
-    646c7771:	nop
-    646c7772:	nop
-    646c7773:	nop
-    646c7774:	nop
-    646c7775:	nop
-    646c7776:	nop
-    646c7777:	nop
-    646c7778:	nop
-    646c7779:	nop
-    646c777a:	nop
-    646c777b:	nop
-    646c777c:	nop
-    646c777d:	nop
-    646c777e:	nop
-    646c777f:	nop
-
-00000000646c7780 <ldexp>:
-    646c7780:	push   %rbx
-    646c7781:	sub    $0x30,%rsp
-    646c7785:	movq   %xmm0,%rax
-    646c778a:	movq   %xmm0,%rbx
-    646c778f:	shr    $0x20,%rax
-    646c7793:	mov    %eax,%r8d
-    646c7796:	and    $0x7fffffff,%r8d
-    646c779d:	or     %ebx,%r8d
-    646c77a0:	sete   %r8b
-    646c77a4:	and    $0x7ff00000,%eax
-    646c77a9:	sete   %cl
-    646c77ac:	or     %cl,%r8b
-    646c77af:	jne    646c77b8 <ldexp+0x38>
-    646c77b1:	cmp    $0x7ff00000,%eax
-    646c77b6:	je     646c7833 <ldexp+0xb3>
-    646c77b8:	movq   %rbx,%xmm1
-    646c77bd:	pxor   %xmm0,%xmm0
-    646c77c1:	ucomisd %xmm0,%xmm1
-    646c77c5:	jp     646c77c9 <ldexp+0x49>
-    646c77c7:	je     646c7833 <ldexp+0xb3>
-    646c77c9:	pxor   %xmm2,%xmm2
-    646c77cd:	cvtsi2sd %edx,%xmm2
-    646c77d1:	mov    %rbx,0x20(%rsp)
-    646c77d6:	fldl   0x20(%rsp)
-    646c77da:	movsd  %xmm2,0x28(%rsp)
-    646c77e0:	fldl   0x28(%rsp)
-    646c77e4:	fxch   %st(1)
-    646c77e6:	fscale
-    646c77e8:	fstp   %st(1)
-    646c77ea:	fstpl  0x20(%rsp)
-    646c77ee:	mov    0x20(%rsp),%rbx
-    646c77f3:	mov    %rbx,%rax
-    646c77f6:	shr    $0x20,%rax
-    646c77fa:	mov    %eax,%ecx
-    646c77fc:	and    $0x7fffffff,%ecx
-    646c7802:	or     %ebx,%ecx
-    646c7804:	sete   %cl
-    646c7807:	and    $0x7ff00000,%eax
-    646c780c:	sete   %dl
-    646c780f:	or     %dl,%cl
-    646c7811:	jne    646c781a <ldexp+0x9a>
-    646c7813:	cmp    $0x7ff00000,%eax
-    646c7818:	je     646c7828 <ldexp+0xa8>
-    646c781a:	movsd  0x20(%rsp),%xmm3
-    646c7820:	ucomisd %xmm0,%xmm3
-    646c7824:	jp     646c7833 <ldexp+0xb3>
-    646c7826:	jne    646c7833 <ldexp+0xb3>
-    646c7828:	call   646c7948 <_errno>
-    646c782d:	movl   $0x22,(%rax)
-    646c7833:	movq   %rbx,%xmm0
-    646c7838:	add    $0x30,%rsp
-    646c783c:	pop    %rbx
-    646c783d:	ret
-    646c783e:	nop
-    646c783f:	nop
-
-00000000646c7840 <one>:
-    646c7840:	add    %al,(%rax)
-    646c7842:	add    %al,(%rax)
-    646c7844:	add    %al,(%rax)
-    646c7846:	lock (bad)
-
-00000000646c7848 <limit>:
-    646c7848:	pop    %rdx
-    646c784a:	cmc
-    646c784b:	sub    %bl,-0x2e(%rdi,%rcx,4)
-    646c784f:	(bad)
-
-00000000646c7850 <log2l>:
-    646c7850:	fldl   -0x16(%rip)        # 646c7840 <one>
-    646c7856:	fldt   (%rdx)
-    646c7858:	fxam
-    646c785a:	fnstsw %ax
-    646c785c:	fld    %st(0)
-    646c785e:	sahf
-    646c785f:	jb     646c7898 <log2l+0x48>
-    646c7861:	fsub   %st(2),%st
-    646c7863:	fld    %st(0)
-    646c7865:	fabs
-    646c7867:	fcompl -0x25(%rip)        # 646c7848 <limit>
-    646c786d:	fnstsw %ax
-    646c786f:	and    $0x45,%ah
-    646c7872:	je     646c7886 <log2l+0x36>
-    646c7874:	fstp   %st(1)
-    646c7876:	fyl2xp1
-    646c7878:	mov    %rcx,%rax
-    646c787b:	movq   $0x0,0x8(%rcx)
-    646c7883:	fstpt  (%rcx)
-    646c7885:	ret
-    646c7886:	fstp   %st(0)
-    646c7888:	fyl2x
-    646c788a:	mov    %rcx,%rax
-    646c788d:	movq   $0x0,0x8(%rcx)
-    646c7895:	fstpt  (%rcx)
-    646c7897:	ret
-    646c7898:	jp     646c7861 <log2l+0x11>
-    646c789a:	fstp   %st(1)
-    646c789c:	fstp   %st(1)
-    646c789e:	mov    %rcx,%rax
-    646c78a1:	movq   $0x0,0x8(%rcx)
-    646c78a9:	fstpt  (%rcx)
-    646c78ab:	ret
-    646c78ac:	nop
-    646c78ad:	nop
-    646c78ae:	nop
-    646c78af:	nop
-
-00000000646c78b0 <vfprintf>:
-    646c78b0:	jmp    *0x6a96(%rip)        # 646ce34c <__imp_vfprintf>
-    646c78b6:	nop
-    646c78b7:	nop
-
-00000000646c78b8 <strncmp>:
-    646c78b8:	jmp    *0x6a86(%rip)        # 646ce344 <__imp_strncmp>
-    646c78be:	nop
-    646c78bf:	nop
-
-00000000646c78c0 <strlen>:
-    646c78c0:	jmp    *0x6a76(%rip)        # 646ce33c <__imp_strlen>
-    646c78c6:	nop
-    646c78c7:	nop
-
-00000000646c78c8 <signal>:
-    646c78c8:	jmp    *0x6a66(%rip)        # 646ce334 <__imp_signal>
+    646c7236:	call   646c7740 <exp2l>
+    646c723b:	test   %ebx,%ebx
+    646c723d:	fldt   0x50(%rsp)
+    646c7241:	fstpl  0x38(%rsp)
+    646c7245:	movsd  0x38(%rsp),%xmm6
+    646c724b:	jns    646c706b <pow+0x10b>
+    646c7251:	mov    $0xffffffff,%edx
+    646c7256:	movq   %rbp,%xmm0
+    646c725b:	call   646c7810 <ldexp>
+    646c7260:	mov    %rsi,%rdx
+    646c7263:	call   646c6ec0 <internal_modf>
+    646c7268:	ucomisd %xmm7,%xmm0
+    646c726c:	jp     646c7274 <pow+0x314>
+    646c726e:	je     646c706b <pow+0x10b>
+    646c7274:	xorpd  0x2184(%rip),%xmm6        # 646c9400 <.rdata+0x40>
+    646c727c:	jmp    646c706b <pow+0x10b>
+    646c7281:	test   %ebx,%ebx
+    646c7283:	js     646c747b <pow+0x51b>
+    646c7289:	movq   %rbp,%xmm5
+    646c728e:	ucomisd 0x2182(%rip),%xmm5        # 646c9418 <.rdata+0x58>
+    646c7296:	jp     646c729e <pow+0x33e>
+    646c7298:	je     646c7461 <pow+0x501>
+    646c729e:	lea    0x50(%rsp),%rbx
+    646c72a3:	movq   %rdi,%xmm3
+    646c72a8:	andpd  0x2180(%rip),%xmm3        # 646c9430 <.rdata+0x70>
+    646c72b0:	movsd  %xmm3,0x30(%rsp)
+    646c72b6:	lea    0x40(%rsp),%rsi
+    646c72bb:	fldl   0x30(%rsp)
+    646c72bf:	mov    %rbx,%rcx
+    646c72c2:	fstpt  0x40(%rsp)
+    646c72c6:	mov    %rsi,%rdx
+    646c72c9:	call   646c78e0 <log2l>
+    646c72ce:	mov    %rsi,%rdx
+    646c72d1:	mov    %rbx,%rcx
+    646c72d4:	fldt   0x50(%rsp)
+    646c72d8:	mov    %rbp,0x30(%rsp)
+    646c72dd:	fldl   0x30(%rsp)
+    646c72e1:	fmulp  %st,%st(1)
+    646c72e3:	fstpt  0x40(%rsp)
+    646c72e7:	call   646c7740 <exp2l>
+    646c72ec:	fldt   0x50(%rsp)
+    646c72f0:	fstpl  0x38(%rsp)
+    646c72f4:	movsd  0x38(%rsp),%xmm6
+    646c72fa:	jmp    646c706b <pow+0x10b>
+    646c72ff:	nop
+    646c7300:	lea    0x68(%rsp),%rbx
+    646c7305:	movq   %rbp,%xmm0
+    646c730a:	pxor   %xmm7,%xmm7
+    646c730e:	mov    %rbx,%rdx
+    646c7311:	call   646c6ec0 <internal_modf>
+    646c7316:	ucomisd %xmm7,%xmm0
+    646c731a:	jp     646c7322 <pow+0x3c2>
+    646c731c:	je     646c7401 <pow+0x4a1>
+    646c7322:	test   %esi,%esi
+    646c7324:	jns    646c7162 <pow+0x202>
+    646c732a:	btc    $0x3f,%rdi
+    646c732f:	movq   %rdi,%xmm5
+    646c7334:	divsd  %xmm5,%xmm2
+    646c7338:	movapd %xmm2,%xmm6
+    646c733c:	jmp    646c706b <pow+0x10b>
+    646c7341:	lea    0x68(%rsp),%rbx
+    646c7346:	movq   %rbp,%xmm0
+    646c734b:	pxor   %xmm7,%xmm7
+    646c734f:	mov    %rbx,%rdx
+    646c7352:	call   646c6ec0 <internal_modf>
+    646c7357:	ucomisd %xmm7,%xmm0
+    646c735b:	jp     646c735f <pow+0x3ff>
+    646c735d:	je     646c7381 <pow+0x421>
+    646c735f:	test   %esi,%esi
+    646c7361:	movq   %rdi,%xmm6
+    646c7366:	xorpd  0x2092(%rip),%xmm6        # 646c9400 <.rdata+0x40>
+    646c736e:	jns    646c706b <pow+0x10b>
+    646c7374:	divsd  %xmm6,%xmm2
+    646c7378:	movapd %xmm2,%xmm6
+    646c737c:	jmp    646c706b <pow+0x10b>
+    646c7381:	mov    $0xffffffff,%edx
+    646c7386:	movq   %rbp,%xmm0
+    646c738b:	call   646c7810 <ldexp>
+    646c7390:	mov    %rbx,%rdx
+    646c7393:	call   646c6ec0 <internal_modf>
+    646c7398:	mov    $0x0,%edx
+    646c739d:	ucomisd %xmm7,%xmm0
+    646c73a1:	setnp  %al
+    646c73a4:	cmovne %edx,%eax
+    646c73a7:	mov    %esi,%edx
+    646c73a9:	shr    $0x1f,%edx
+    646c73ac:	test   %dl,%dl
+    646c73ae:	je     646c73b8 <pow+0x458>
+    646c73b0:	test   %al,%al
+    646c73b2:	jne    646c7162 <pow+0x202>
+    646c73b8:	mov    %esi,%edx
+    646c73ba:	mov    $0x1,%r8d
+    646c73c0:	not    %edx
+    646c73c2:	shr    $0x1f,%edx
+    646c73c5:	ucomisd %xmm7,%xmm0
+    646c73c9:	setp   %cl
+    646c73cc:	cmovne %r8d,%ecx
+    646c73d0:	test   %cl,%cl
+    646c73d2:	je     646c73d8 <pow+0x478>
+    646c73d4:	test   %dl,%dl
+    646c73d6:	jne    646c73f4 <pow+0x494>
+    646c73d8:	test   %al,%al
+    646c73da:	je     646c73e4 <pow+0x484>
+    646c73dc:	test   %dl,%dl
+    646c73de:	jne    646c7063 <pow+0x103>
+    646c73e4:	test   %esi,%esi
+    646c73e6:	js     646c741c <pow+0x4bc>
+    646c73e8:	ucomisd %xmm7,%xmm0
+    646c73ec:	jp     646c73f4 <pow+0x494>
+    646c73ee:	je     646c7063 <pow+0x103>
+    646c73f4:	movsd  0x1fe4(%rip),%xmm6        # 646c93e0 <.rdata+0x20>
+    646c73fc:	jmp    646c706b <pow+0x10b>
+    646c7401:	mov    $0xffffffff,%edx
+    646c7406:	movq   %rbp,%xmm0
+    646c740b:	call   646c7810 <ldexp>
+    646c7410:	mov    %rbx,%rdx
+    646c7413:	call   646c6ec0 <internal_modf>
+    646c7418:	test   %esi,%esi
+    646c741a:	js     646c73e8 <pow+0x488>
+    646c741c:	ucomisd %xmm7,%xmm0
+    646c7420:	jp     646c7428 <pow+0x4c8>
+    646c7422:	je     646c7162 <pow+0x202>
+    646c7428:	movsd  0x1fa8(%rip),%xmm6        # 646c93d8 <.rdata+0x18>
+    646c7430:	jmp    646c706b <pow+0x10b>
+    646c7435:	movq   %rdi,%xmm5
+    646c743a:	xorpd  0x1fbe(%rip),%xmm5        # 646c9400 <.rdata+0x40>
+    646c7442:	movq   %xmm5,%rax
+    646c7447:	movq   %rdi,%xmm5
+    646c744c:	ucomisd 0x1fbc(%rip),%xmm5        # 646c9410 <.rdata+0x50>
+    646c7454:	jp     646c74af <pow+0x54f>
+    646c7456:	jne    646c74af <pow+0x54f>
+    646c7458:	movapd %xmm2,%xmm6
+    646c745c:	jmp    646c706b <pow+0x10b>
+    646c7461:	mov    %rdi,0x30(%rsp)
+    646c7466:	fldl   0x30(%rsp)
+    646c746a:	fsqrt
+    646c746c:	fstpl  0x30(%rsp)
+    646c7470:	movsd  0x30(%rsp),%xmm6
+    646c7476:	jmp    646c706b <pow+0x10b>
+    646c747b:	call   646c79d8 <_errno>
+    646c7480:	movsd  0x1f40(%rip),%xmm6        # 646c93c8 <.rdata+0x8>
+    646c7488:	movl   $0x21,(%rax)
+    646c748e:	jmp    646c70db <pow+0x17b>
+    646c7493:	movq   %rbp,%xmm3
+    646c7498:	movq   %rdi,%xmm0
+    646c749d:	cvttsd2si %xmm3,%edx
+    646c74a1:	call   646c74c0 <__powi>
+    646c74a6:	movapd %xmm0,%xmm6
+    646c74aa:	jmp    646c706b <pow+0x10b>
+    646c74af:	mov    %rax,%rdi
+    646c74b2:	jmp    646c7194 <pow+0x234>
+    646c74b7:	nop
+    646c74b8:	nop
+    646c74b9:	nop
+    646c74ba:	nop
+    646c74bb:	nop
+    646c74bc:	nop
+    646c74bd:	nop
+    646c74be:	nop
+    646c74bf:	nop
+
+00000000646c74c0 <__powi>:
+    646c74c0:	sub    $0x58,%rsp
+    646c74c4:	movaps %xmm6,0x40(%rsp)
+    646c74c9:	movsd  0x1f87(%rip),%xmm1        # 646c9458 <.rdata+0x18>
+    646c74d1:	mov    $0x0,%r10d
+    646c74d7:	movq   %xmm0,%r8
+    646c74dc:	movq   %xmm0,%rax
+    646c74e1:	shr    $0x20,%r8
+    646c74e5:	mov    %r8d,%ecx
+    646c74e8:	mov    %r8d,%r9d
+    646c74eb:	and    $0xfffff,%ecx
+    646c74f1:	and    $0x7ff00000,%r9d
+    646c74f8:	or     %eax,%ecx
+    646c74fa:	ucomisd %xmm1,%xmm0
+    646c74fe:	mov    %r9d,%r11d
+    646c7501:	setnp  %al
+    646c7504:	cmovne %r10d,%eax
+    646c7508:	test   %edx,%edx
+    646c750a:	sete   %r10b
+    646c750e:	or     %r10d,%eax
+    646c7511:	or     %ecx,%r11d
+    646c7514:	jne    646c7550 <__powi+0x90>
+    646c7516:	test   %al,%al
+    646c7518:	movapd %xmm1,%xmm6
+    646c751c:	jne    646c7540 <__powi+0x80>
+    646c751e:	mov    %edx,%eax
+    646c7520:	and    $0x1,%eax
+    646c7523:	test   %edx,%edx
+    646c7525:	js     646c7615 <__powi+0x155>
+    646c752b:	test   %eax,%eax
+    646c752d:	pxor   %xmm6,%xmm6
+    646c7531:	je     646c7540 <__powi+0x80>
+    646c7533:	test   %r8d,%r8d
+    646c7536:	jns    646c7540 <__powi+0x80>
+    646c7538:	movsd  0x1f20(%rip),%xmm6        # 646c9460 <.rdata+0x20>
+    646c7540:	movapd %xmm6,%xmm0
+    646c7544:	movaps 0x40(%rsp),%xmm6
+    646c7549:	add    $0x58,%rsp
+    646c754d:	ret
+    646c754e:	xchg   %ax,%ax
+    646c7550:	test   %r9d,%r9d
+    646c7553:	jne    646c75c0 <__powi+0x100>
+    646c7555:	test   %al,%al
+    646c7557:	movapd %xmm1,%xmm6
+    646c755b:	jne    646c7540 <__powi+0x80>
+    646c755d:	mov    %edx,%eax
+    646c755f:	movapd %xmm0,%xmm6
+    646c7563:	andpd  0x1f15(%rip),%xmm6        # 646c9480 <.rdata+0x40>
+    646c756b:	and    $0x1,%eax
+    646c756e:	test   %edx,%edx
+    646c7570:	js     646c7602 <__powi+0x142>
+    646c7576:	cmp    $0x1,%edx
+    646c7579:	je     646c75a1 <__powi+0xe1>
+    646c757b:	test   $0x1,%dl
+    646c757e:	jne    646c76b0 <__powi+0x1f0>
+    646c7584:	movapd %xmm6,%xmm0
+    646c7588:	shr    %edx
+    646c758a:	movapd %xmm1,%xmm6
+    646c758e:	xchg   %ax,%ax
+    646c7590:	mulsd  %xmm0,%xmm0
+    646c7594:	test   $0x1,%dl
+    646c7597:	je     646c759d <__powi+0xdd>
+    646c7599:	mulsd  %xmm0,%xmm6
+    646c759d:	shr    %edx
+    646c759f:	jne    646c7590 <__powi+0xd0>
+    646c75a1:	shr    $0x1f,%r8d
+    646c75a5:	test   %r8b,%r8b
+    646c75a8:	je     646c7540 <__powi+0x80>
+    646c75aa:	test   %eax,%eax
+    646c75ac:	je     646c7540 <__powi+0x80>
+    646c75ae:	xorpd  0x1eda(%rip),%xmm6        # 646c9490 <.rdata+0x50>
+    646c75b6:	jmp    646c7540 <__powi+0x80>
+    646c75b8:	nopl   0x0(%rax,%rax,1)
+    646c75c0:	cmp    $0x7ff00000,%r9d
+    646c75c7:	jne    646c7555 <__powi+0x95>
+    646c75c9:	test   %ecx,%ecx
+    646c75cb:	jne    646c7640 <__powi+0x180>
+    646c75cd:	mov    %edx,%r9d
+    646c75d0:	movapd %xmm1,%xmm6
+    646c75d4:	and    $0x1,%r9d
+    646c75d8:	test   %al,%al
+    646c75da:	jne    646c7540 <__powi+0x80>
+    646c75e0:	test   %r8d,%r8d
+    646c75e3:	js     646c76d0 <__powi+0x210>
+    646c75e9:	test   %edx,%edx
+    646c75eb:	movsd  0x1e75(%rip),%xmm6        # 646c9468 <.rdata+0x28>
+    646c75f3:	jns    646c7540 <__powi+0x80>
+    646c75f9:	pxor   %xmm6,%xmm6
+    646c75fd:	jmp    646c7540 <__powi+0x80>
+    646c7602:	movapd %xmm1,%xmm4
+    646c7606:	neg    %edx
+    646c7608:	divsd  %xmm6,%xmm4
+    646c760c:	movapd %xmm4,%xmm6
+    646c7610:	jmp    646c7576 <__powi+0xb6>
+    646c7615:	test   %eax,%eax
+    646c7617:	movsd  0x1e49(%rip),%xmm6        # 646c9468 <.rdata+0x28>
+    646c761f:	je     646c7540 <__powi+0x80>
+    646c7625:	test   %r8d,%r8d
+    646c7628:	jns    646c7540 <__powi+0x80>
+    646c762e:	movsd  0x1e3a(%rip),%xmm6        # 646c9470 <.rdata+0x30>
+    646c7636:	jmp    646c7540 <__powi+0x80>
+    646c763b:	nopl   0x0(%rax,%rax,1)
+    646c7640:	test   %al,%al
+    646c7642:	movapd %xmm1,%xmm6
+    646c7646:	jne    646c7540 <__powi+0x80>
+    646c764c:	test   %r8d,%r8d
+    646c764f:	movsd  0x1df9(%rip),%xmm6        # 646c9450 <.rdata+0x10>
+    646c7657:	js     646c76c0 <__powi+0x200>
+    646c7659:	mov    %edx,0x3c(%rsp)
+    646c765d:	movsd  %xmm0,0x30(%rsp)
+    646c7663:	call   646c79d8 <_errno>
+    646c7668:	mov    0x3c(%rsp),%edx
+    646c766c:	pxor   %xmm3,%xmm3
+    646c7670:	mov    $0x1,%ecx
+    646c7675:	movsd  0x30(%rsp),%xmm0
+    646c767b:	movl   $0x21,(%rax)
+    646c7681:	movsd  %xmm6,0x20(%rsp)
+    646c7687:	movapd %xmm0,%xmm2
+    646c768b:	cvtsi2sd %edx,%xmm3
+    646c768f:	lea    0x1daa(%rip),%rdx        # 646c9440 <.rdata>
+    646c7696:	call   646c7c50 <__mingw_raise_matherr>
+    646c769b:	movapd %xmm6,%xmm0
+    646c769f:	movaps 0x40(%rsp),%xmm6
+    646c76a4:	add    $0x58,%rsp
+    646c76a8:	ret
+    646c76a9:	nopl   0x0(%rax)
+    646c76b0:	movapd %xmm6,%xmm1
+    646c76b4:	jmp    646c7584 <__powi+0xc4>
+    646c76b9:	nopl   0x0(%rax)
+    646c76c0:	movsd  0x1d80(%rip),%xmm6        # 646c9448 <.rdata+0x8>
+    646c76c8:	jmp    646c7659 <__powi+0x199>
+    646c76ca:	nopw   0x0(%rax,%rax,1)
+    646c76d0:	mov    %edx,%eax
+    646c76d2:	not    %eax
+    646c76d4:	mov    %eax,%ecx
+    646c76d6:	and    $0x1,%ecx
+    646c76d9:	test   %edx,%edx
+    646c76db:	jns    646c76e9 <__powi+0x229>
+    646c76dd:	test   %cl,%cl
+    646c76df:	pxor   %xmm6,%xmm6
+    646c76e3:	jne    646c7540 <__powi+0x80>
+    646c76e9:	shr    $0x1f,%eax
+    646c76ec:	test   $0x1,%dl
+    646c76ef:	je     646c7701 <__powi+0x241>
+    646c76f1:	test   %al,%al
+    646c76f3:	movsd  0x1d75(%rip),%xmm6        # 646c9470 <.rdata+0x30>
+    646c76fb:	jne    646c7540 <__powi+0x80>
+    646c7701:	test   %cl,%cl
+    646c7703:	je     646c7715 <__powi+0x255>
+    646c7705:	test   %al,%al
+    646c7707:	movsd  0x1d59(%rip),%xmm6        # 646c9468 <.rdata+0x28>
+    646c770f:	jne    646c7540 <__powi+0x80>
+    646c7715:	test   %edx,%edx
+    646c7717:	js     646c7730 <__powi+0x270>
+    646c7719:	and    $0x1,%dl
+    646c771c:	jne    646c762e <__powi+0x16e>
+    646c7722:	movsd  0x1d3e(%rip),%xmm6        # 646c9468 <.rdata+0x28>
+    646c772a:	jmp    646c7540 <__powi+0x80>
+    646c772f:	nop
+    646c7730:	test   %r9d,%r9d
+    646c7733:	jne    646c7538 <__powi+0x78>
+    646c7739:	jmp    646c75f9 <__powi+0x139>
+    646c773e:	nop
+    646c773f:	nop
+
+00000000646c7740 <exp2l>:
+    646c7740:	fldt   (%rdx)
+    646c7742:	fxam
+    646c7744:	fstsw  %ax
+    646c7747:	mov    $0x45,%dh
+    646c7749:	and    %ah,%dh
+    646c774b:	cmp    $0x5,%dh
+    646c774e:	je     646c778f <exp2l+0x4f>
+    646c7750:	fld    %st(0)
+    646c7752:	sub    $0x8,%rsp
+    646c7756:	fnstcw 0x4(%rsp)
+    646c775a:	movzwl 0x4(%rsp),%eax
+    646c775f:	or     $0xc,%ah
+    646c7762:	mov    %ax,(%rsp)
+    646c7766:	fldcw  (%rsp)
+    646c7769:	frndint
+    646c776b:	fldcw  0x4(%rsp)
+    646c776f:	add    $0x8,%rsp
+    646c7773:	fsubr  %st,%st(1)
+    646c7775:	fxch   %st(1)
+    646c7777:	f2xm1
+    646c7779:	fld1
+    646c777b:	faddp  %st,%st(1)
+    646c777d:	fscale
+    646c777f:	fstp   %st(1)
+    646c7781:	mov    %rcx,%rax
+    646c7784:	movq   $0x0,0x8(%rcx)
+    646c778c:	fstpt  (%rcx)
+    646c778e:	ret
+    646c778f:	test   $0x200,%eax
+    646c7794:	je     646c779a <exp2l+0x5a>
+    646c7796:	fstp   %st(0)
+    646c7798:	fldz
+    646c779a:	mov    %rcx,%rax
+    646c779d:	movq   $0x0,0x8(%rcx)
+    646c77a5:	fstpt  (%rcx)
+    646c77a7:	ret
+    646c77a8:	nop
+    646c77a9:	nop
+    646c77aa:	nop
+    646c77ab:	nop
+    646c77ac:	nop
+    646c77ad:	nop
+    646c77ae:	nop
+    646c77af:	nop
+
+00000000646c77b0 <one>:
+    646c77b0:	add    %al,(%rax)
+    646c77b2:	add    %al,(%rax)
+    646c77b4:	add    %al,(%rax)
+    646c77b6:	lock (bad)
+
+00000000646c77b8 <limit>:
+    646c77b8:	pop    %rdx
+    646c77ba:	cmc
+    646c77bb:	sub    %bl,-0x2e(%rdi,%rcx,4)
+    646c77bf:	(bad)
+
+00000000646c77c0 <__logl_internal>:
+    646c77c0:	fldln2
+    646c77c2:	fldt   (%rdx)
+    646c77c4:	fld    %st(0)
+    646c77c6:	fsubl  -0x1c(%rip)        # 646c77b0 <one>
+    646c77cc:	fld    %st(0)
+    646c77ce:	fabs
+    646c77d0:	fcompl -0x1e(%rip)        # 646c77b8 <limit>
+    646c77d6:	fnstsw %ax
+    646c77d8:	and    $0x45,%ah
+    646c77db:	je     646c77ef <__logl_internal+0x2f>
+    646c77dd:	fstp   %st(1)
+    646c77df:	fyl2xp1
+    646c77e1:	mov    %rcx,%rax
+    646c77e4:	movq   $0x0,0x8(%rcx)
+    646c77ec:	fstpt  (%rcx)
+    646c77ee:	ret
+    646c77ef:	fstp   %st(0)
+    646c77f1:	fyl2x
+    646c77f3:	mov    %rcx,%rax
+    646c77f6:	movq   $0x0,0x8(%rcx)
+    646c77fe:	fstpt  (%rcx)
+    646c7800:	ret
+    646c7801:	nop
+    646c7802:	nop
+    646c7803:	nop
+    646c7804:	nop
+    646c7805:	nop
+    646c7806:	nop
+    646c7807:	nop
+    646c7808:	nop
+    646c7809:	nop
+    646c780a:	nop
+    646c780b:	nop
+    646c780c:	nop
+    646c780d:	nop
+    646c780e:	nop
+    646c780f:	nop
+
+00000000646c7810 <ldexp>:
+    646c7810:	push   %rbx
+    646c7811:	sub    $0x30,%rsp
+    646c7815:	movq   %xmm0,%rax
+    646c781a:	movq   %xmm0,%rbx
+    646c781f:	shr    $0x20,%rax
+    646c7823:	mov    %eax,%r8d
+    646c7826:	and    $0x7fffffff,%r8d
+    646c782d:	or     %ebx,%r8d
+    646c7830:	sete   %r8b
+    646c7834:	and    $0x7ff00000,%eax
+    646c7839:	sete   %cl
+    646c783c:	or     %cl,%r8b
+    646c783f:	jne    646c7848 <ldexp+0x38>
+    646c7841:	cmp    $0x7ff00000,%eax
+    646c7846:	je     646c78c3 <ldexp+0xb3>
+    646c7848:	movq   %rbx,%xmm1
+    646c784d:	pxor   %xmm0,%xmm0
+    646c7851:	ucomisd %xmm0,%xmm1
+    646c7855:	jp     646c7859 <ldexp+0x49>
+    646c7857:	je     646c78c3 <ldexp+0xb3>
+    646c7859:	pxor   %xmm2,%xmm2
+    646c785d:	cvtsi2sd %edx,%xmm2
+    646c7861:	mov    %rbx,0x20(%rsp)
+    646c7866:	fldl   0x20(%rsp)
+    646c786a:	movsd  %xmm2,0x28(%rsp)
+    646c7870:	fldl   0x28(%rsp)
+    646c7874:	fxch   %st(1)
+    646c7876:	fscale
+    646c7878:	fstp   %st(1)
+    646c787a:	fstpl  0x20(%rsp)
+    646c787e:	mov    0x20(%rsp),%rbx
+    646c7883:	mov    %rbx,%rax
+    646c7886:	shr    $0x20,%rax
+    646c788a:	mov    %eax,%ecx
+    646c788c:	and    $0x7fffffff,%ecx
+    646c7892:	or     %ebx,%ecx
+    646c7894:	sete   %cl
+    646c7897:	and    $0x7ff00000,%eax
+    646c789c:	sete   %dl
+    646c789f:	or     %dl,%cl
+    646c78a1:	jne    646c78aa <ldexp+0x9a>
+    646c78a3:	cmp    $0x7ff00000,%eax
+    646c78a8:	je     646c78b8 <ldexp+0xa8>
+    646c78aa:	movsd  0x20(%rsp),%xmm3
+    646c78b0:	ucomisd %xmm0,%xmm3
+    646c78b4:	jp     646c78c3 <ldexp+0xb3>
+    646c78b6:	jne    646c78c3 <ldexp+0xb3>
+    646c78b8:	call   646c79d8 <_errno>
+    646c78bd:	movl   $0x22,(%rax)
+    646c78c3:	movq   %rbx,%xmm0
+    646c78c8:	add    $0x30,%rsp
+    646c78cc:	pop    %rbx
+    646c78cd:	ret
     646c78ce:	nop
     646c78cf:	nop
 
-00000000646c78d0 <printf>:
-    646c78d0:	jmp    *0x6a4e(%rip)        # 646ce324 <__imp_printf>
-    646c78d6:	nop
-    646c78d7:	nop
-
-00000000646c78d8 <perror>:
-    646c78d8:	jmp    *0x6a3e(%rip)        # 646ce31c <__imp_perror>
-    646c78de:	nop
-    646c78df:	nop
-
-00000000646c78e0 <malloc>:
-    646c78e0:	jmp    *0x6a2e(%rip)        # 646ce314 <__imp_malloc>
-    646c78e6:	nop
-    646c78e7:	nop
-
-00000000646c78e8 <log10>:
-    646c78e8:	jmp    *0x6a1e(%rip)        # 646ce30c <__imp_log10>
-    646c78ee:	nop
-    646c78ef:	nop
-
-00000000646c78f0 <fwrite>:
-    646c78f0:	jmp    *0x6a0e(%rip)        # 646ce304 <__imp_fwrite>
-    646c78f6:	nop
-    646c78f7:	nop
-
-00000000646c78f8 <free>:
-    646c78f8:	jmp    *0x69fe(%rip)        # 646ce2fc <__imp_free>
-    646c78fe:	nop
-    646c78ff:	nop
-
-00000000646c7900 <fprintf>:
-    646c7900:	jmp    *0x69ee(%rip)        # 646ce2f4 <__imp_fprintf>
-    646c7906:	nop
-    646c7907:	nop
-
-00000000646c7908 <fopen>:
-    646c7908:	jmp    *0x69de(%rip)        # 646ce2ec <__imp_fopen>
-    646c790e:	nop
-    646c790f:	nop
-
-00000000646c7910 <fclose>:
-    646c7910:	jmp    *0x69ce(%rip)        # 646ce2e4 <__imp_fclose>
-    646c7916:	nop
-    646c7917:	nop
-
-00000000646c7918 <exit>:
-    646c7918:	jmp    *0x69be(%rip)        # 646ce2dc <__imp_exit>
-    646c791e:	nop
-    646c791f:	nop
-
-00000000646c7920 <calloc>:
-    646c7920:	jmp    *0x69ae(%rip)        # 646ce2d4 <__imp_calloc>
-    646c7926:	nop
-    646c7927:	nop
-
-00000000646c7928 <abort>:
-    646c7928:	jmp    *0x699e(%rip)        # 646ce2cc <__imp_abort>
-    646c792e:	nop
-    646c792f:	nop
-
-00000000646c7930 <_vsnprintf>:
-    646c7930:	jmp    *0x698e(%rip)        # 646ce2c4 <__imp__vsnprintf>
-    646c7936:	nop
-    646c7937:	nop
-
-00000000646c7938 <_mkdir>:
-    646c7938:	jmp    *0x6976(%rip)        # 646ce2b4 <__imp__mkdir>
+00000000646c78d0 <one>:
+    646c78d0:	add    %al,(%rax)
+    646c78d2:	add    %al,(%rax)
+    646c78d4:	add    %al,(%rax)
+    646c78d6:	lock (bad)
+
+00000000646c78d8 <limit>:
+    646c78d8:	pop    %rdx
+    646c78da:	cmc
+    646c78db:	sub    %bl,-0x2e(%rdi,%rcx,4)
+    646c78df:	(bad)
+
+00000000646c78e0 <log2l>:
+    646c78e0:	fldl   -0x16(%rip)        # 646c78d0 <one>
+    646c78e6:	fldt   (%rdx)
+    646c78e8:	fxam
+    646c78ea:	fnstsw %ax
+    646c78ec:	fld    %st(0)
+    646c78ee:	sahf
+    646c78ef:	jb     646c7928 <log2l+0x48>
+    646c78f1:	fsub   %st(2),%st
+    646c78f3:	fld    %st(0)
+    646c78f5:	fabs
+    646c78f7:	fcompl -0x25(%rip)        # 646c78d8 <limit>
+    646c78fd:	fnstsw %ax
+    646c78ff:	and    $0x45,%ah
+    646c7902:	je     646c7916 <log2l+0x36>
+    646c7904:	fstp   %st(1)
+    646c7906:	fyl2xp1
+    646c7908:	mov    %rcx,%rax
+    646c790b:	movq   $0x0,0x8(%rcx)
+    646c7913:	fstpt  (%rcx)
+    646c7915:	ret
+    646c7916:	fstp   %st(0)
+    646c7918:	fyl2x
+    646c791a:	mov    %rcx,%rax
+    646c791d:	movq   $0x0,0x8(%rcx)
+    646c7925:	fstpt  (%rcx)
+    646c7927:	ret
+    646c7928:	jp     646c78f1 <log2l+0x11>
+    646c792a:	fstp   %st(1)
+    646c792c:	fstp   %st(1)
+    646c792e:	mov    %rcx,%rax
+    646c7931:	movq   $0x0,0x8(%rcx)
+    646c7939:	fstpt  (%rcx)
+    646c793b:	ret
+    646c793c:	nop
+    646c793d:	nop
     646c793e:	nop
     646c793f:	nop
 
-00000000646c7940 <_initterm>:
-    646c7940:	jmp    *0x695e(%rip)        # 646ce2a4 <__imp__initterm>
+00000000646c7940 <vfprintf>:
+    646c7940:	jmp    *0x6a06(%rip)        # 646ce34c <__imp_vfprintf>
     646c7946:	nop
     646c7947:	nop
 
-00000000646c7948 <_errno>:
-    646c7948:	jmp    *0x694e(%rip)        # 646ce29c <__imp__errno>
+00000000646c7948 <strncmp>:
+    646c7948:	jmp    *0x69f6(%rip)        # 646ce344 <__imp_strncmp>
     646c794e:	nop
     646c794f:	nop
 
-00000000646c7950 <_amsg_exit>:
-    646c7950:	jmp    *0x693e(%rip)        # 646ce294 <__imp__amsg_exit>
+00000000646c7950 <strlen>:
+    646c7950:	jmp    *0x69e6(%rip)        # 646ce33c <__imp_strlen>
     646c7956:	nop
     646c7957:	nop
-    646c7958:	nopl   0x0(%rax,%rax,1)
 
-00000000646c7960 <_initialize_onexit_table>:
-    646c7960:	test   %rcx,%rcx
-    646c7963:	je     646c797f <_initialize_onexit_table+0x1f>
-    646c7965:	xor    %eax,%eax
-    646c7967:	movq   $0x0,0x10(%rcx)
-    646c796f:	movq   $0x0,0x8(%rcx)
-    646c7977:	movq   $0x0,(%rcx)
-    646c797e:	ret
-    646c797f:	mov    $0xffffffff,%eax
-    646c7984:	ret
-    646c7985:	nop
-    646c7986:	cs nopw 0x0(%rax,%rax,1)
-
-00000000646c7990 <_register_onexit_function>:
-    646c7990:	push   %rbp
-    646c7991:	push   %rdi
-    646c7992:	push   %rsi
-    646c7993:	push   %rbx
-    646c7994:	sub    $0x28,%rsp
-    646c7998:	test   %rcx,%rcx
-    646c799b:	mov    %rcx,%rbx
-    646c799e:	mov    %rdx,%rdi
-    646c79a1:	je     646c7a40 <_register_onexit_function+0xb0>
-    646c79a7:	mov    $0x8,%ecx
-    646c79ac:	call   646c7b00 <_lock>
-    646c79b1:	cmpq   $0x0,(%rbx)
-    646c79b5:	je     646c7a14 <_register_onexit_function+0x84>
-    646c79b7:	mov    0x8(%rbx),%rsi
-    646c79bb:	mov    0x10(%rbx),%rax
-    646c79bf:	cmp    %rsi,%rax
-    646c79c2:	je     646c79e4 <_register_onexit_function+0x54>
-    646c79c4:	lea    0x8(%rsi),%rax
-    646c79c8:	mov    $0x8,%ecx
-    646c79cd:	mov    %rax,0x8(%rbx)
-    646c79d1:	mov    %rdi,(%rsi)
-    646c79d4:	call   646c7af8 <_unlock>
-    646c79d9:	xor    %eax,%eax
-    646c79db:	add    $0x28,%rsp
-    646c79df:	pop    %rbx
-    646c79e0:	pop    %rsi
-    646c79e1:	pop    %rdi
-    646c79e2:	pop    %rbp
-    646c79e3:	ret
-    646c79e4:	mov    (%rbx),%rcx
-    646c79e7:	sub    %rcx,%rsi
-    646c79ea:	mov    %rsi,%rax
-    646c79ed:	sar    $0x3,%rax
-    646c79f1:	shl    $0x4,%rax
-    646c79f5:	mov    %rax,%rdx
-    646c79f8:	mov    %rax,%rbp
-    646c79fb:	call   646c7af0 <realloc>
-    646c7a00:	test   %rax,%rax
-    646c7a03:	je     646c7a47 <_register_onexit_function+0xb7>
-    646c7a05:	mov    %rax,(%rbx)
-    646c7a08:	add    %rax,%rsi
-    646c7a0b:	add    %rbp,%rax
-    646c7a0e:	mov    %rax,0x10(%rbx)
-    646c7a12:	jmp    646c79c4 <_register_onexit_function+0x34>
-    646c7a14:	mov    $0x8,%edx
-    646c7a19:	mov    $0x20,%ecx
-    646c7a1e:	call   646c7920 <calloc>
-    646c7a23:	test   %rax,%rax
-    646c7a26:	mov    %rax,%rsi
-    646c7a29:	mov    %rax,(%rbx)
-    646c7a2c:	je     646c7a47 <_register_onexit_function+0xb7>
-    646c7a2e:	mov    %rax,0x8(%rbx)
-    646c7a32:	lea    0x100(%rax),%rax
-    646c7a39:	mov    %rax,0x10(%rbx)
-    646c7a3d:	jmp    646c79bf <_register_onexit_function+0x2f>
-    646c7a3f:	nop
-    646c7a40:	mov    $0xffffffff,%eax
-    646c7a45:	jmp    646c79db <_register_onexit_function+0x4b>
-    646c7a47:	mov    $0x8,%ecx
-    646c7a4c:	call   646c7af8 <_unlock>
-    646c7a51:	mov    $0xffffffff,%eax
-    646c7a56:	jmp    646c79db <_register_onexit_function+0x4b>
-    646c7a58:	nopl   0x0(%rax,%rax,1)
-
-00000000646c7a60 <_execute_onexit_table>:
-    646c7a60:	push   %rdi
-    646c7a61:	push   %rsi
-    646c7a62:	push   %rbx
-    646c7a63:	sub    $0x20,%rsp
-    646c7a67:	mov    %rcx,%rdi
-    646c7a6a:	mov    $0x8,%ecx
-    646c7a6f:	call   646c7b00 <_lock>
-    646c7a74:	mov    (%rdi),%rsi
-    646c7a77:	mov    $0x8,%ecx
-    646c7a7c:	movq   $0x0,0x10(%rdi)
-    646c7a84:	mov    0x8(%rdi),%rbx
-    646c7a88:	movq   $0x0,(%rdi)
-    646c7a8f:	movq   $0x0,0x8(%rdi)
-    646c7a97:	call   646c7af8 <_unlock>
-    646c7a9c:	test   %rsi,%rsi
-    646c7a9f:	je     646c7ac5 <_execute_onexit_table+0x65>
-    646c7aa1:	sub    $0x8,%rbx
-    646c7aa5:	cmp    %rbx,%rsi
-    646c7aa8:	ja     646c7abd <_execute_onexit_table+0x5d>
-    646c7aaa:	mov    (%rbx),%rax
-    646c7aad:	test   %rax,%rax
-    646c7ab0:	je     646c7aa1 <_execute_onexit_table+0x41>
-    646c7ab2:	call   *%rax
-    646c7ab4:	sub    $0x8,%rbx
-    646c7ab8:	cmp    %rbx,%rsi
-    646c7abb:	jbe    646c7aaa <_execute_onexit_table+0x4a>
-    646c7abd:	mov    %rsi,%rcx
-    646c7ac0:	call   646c78f8 <free>
-    646c7ac5:	xor    %eax,%eax
-    646c7ac7:	add    $0x20,%rsp
-    646c7acb:	pop    %rbx
-    646c7acc:	pop    %rsi
-    646c7acd:	pop    %rdi
-    646c7ace:	ret
+00000000646c7958 <signal>:
+    646c7958:	jmp    *0x69d6(%rip)        # 646ce334 <__imp_signal>
+    646c795e:	nop
+    646c795f:	nop
+
+00000000646c7960 <printf>:
+    646c7960:	jmp    *0x69be(%rip)        # 646ce324 <__imp_printf>
+    646c7966:	nop
+    646c7967:	nop
+
+00000000646c7968 <perror>:
+    646c7968:	jmp    *0x69ae(%rip)        # 646ce31c <__imp_perror>
+    646c796e:	nop
+    646c796f:	nop
+
+00000000646c7970 <malloc>:
+    646c7970:	jmp    *0x699e(%rip)        # 646ce314 <__imp_malloc>
+    646c7976:	nop
+    646c7977:	nop
+
+00000000646c7978 <log10>:
+    646c7978:	jmp    *0x698e(%rip)        # 646ce30c <__imp_log10>
+    646c797e:	nop
+    646c797f:	nop
+
+00000000646c7980 <fwrite>:
+    646c7980:	jmp    *0x697e(%rip)        # 646ce304 <__imp_fwrite>
+    646c7986:	nop
+    646c7987:	nop
+
+00000000646c7988 <free>:
+    646c7988:	jmp    *0x696e(%rip)        # 646ce2fc <__imp_free>
+    646c798e:	nop
+    646c798f:	nop
+
+00000000646c7990 <fprintf>:
+    646c7990:	jmp    *0x695e(%rip)        # 646ce2f4 <__imp_fprintf>
+    646c7996:	nop
+    646c7997:	nop
+
+00000000646c7998 <fopen>:
+    646c7998:	jmp    *0x694e(%rip)        # 646ce2ec <__imp_fopen>
+    646c799e:	nop
+    646c799f:	nop
+
+00000000646c79a0 <fclose>:
+    646c79a0:	jmp    *0x693e(%rip)        # 646ce2e4 <__imp_fclose>
+    646c79a6:	nop
+    646c79a7:	nop
+
+00000000646c79a8 <exit>:
+    646c79a8:	jmp    *0x692e(%rip)        # 646ce2dc <__imp_exit>
+    646c79ae:	nop
+    646c79af:	nop
+
+00000000646c79b0 <calloc>:
+    646c79b0:	jmp    *0x691e(%rip)        # 646ce2d4 <__imp_calloc>
+    646c79b6:	nop
+    646c79b7:	nop
+
+00000000646c79b8 <abort>:
+    646c79b8:	jmp    *0x690e(%rip)        # 646ce2cc <__imp_abort>
+    646c79be:	nop
+    646c79bf:	nop
+
+00000000646c79c0 <_vsnprintf>:
+    646c79c0:	jmp    *0x68fe(%rip)        # 646ce2c4 <__imp__vsnprintf>
+    646c79c6:	nop
+    646c79c7:	nop
+
+00000000646c79c8 <_mkdir>:
+    646c79c8:	jmp    *0x68e6(%rip)        # 646ce2b4 <__imp__mkdir>
+    646c79ce:	nop
+    646c79cf:	nop
+
+00000000646c79d0 <_initterm>:
+    646c79d0:	jmp    *0x68ce(%rip)        # 646ce2a4 <__imp__initterm>
+    646c79d6:	nop
+    646c79d7:	nop
+
+00000000646c79d8 <_errno>:
+    646c79d8:	jmp    *0x68be(%rip)        # 646ce29c <__imp__errno>
+    646c79de:	nop
+    646c79df:	nop
+
+00000000646c79e0 <_amsg_exit>:
+    646c79e0:	jmp    *0x68ae(%rip)        # 646ce294 <__imp__amsg_exit>
+    646c79e6:	nop
+    646c79e7:	nop
+    646c79e8:	nopl   0x0(%rax,%rax,1)
+
+00000000646c79f0 <_initialize_onexit_table>:
+    646c79f0:	test   %rcx,%rcx
+    646c79f3:	je     646c7a0f <_initialize_onexit_table+0x1f>
+    646c79f5:	xor    %eax,%eax
+    646c79f7:	movq   $0x0,0x10(%rcx)
+    646c79ff:	movq   $0x0,0x8(%rcx)
+    646c7a07:	movq   $0x0,(%rcx)
+    646c7a0e:	ret
+    646c7a0f:	mov    $0xffffffff,%eax
+    646c7a14:	ret
+    646c7a15:	nop
+    646c7a16:	cs nopw 0x0(%rax,%rax,1)
+
+00000000646c7a20 <_register_onexit_function>:
+    646c7a20:	push   %rbp
+    646c7a21:	push   %rdi
+    646c7a22:	push   %rsi
+    646c7a23:	push   %rbx
+    646c7a24:	sub    $0x28,%rsp
+    646c7a28:	test   %rcx,%rcx
+    646c7a2b:	mov    %rcx,%rbx
+    646c7a2e:	mov    %rdx,%rdi
+    646c7a31:	je     646c7ad0 <_register_onexit_function+0xb0>
+    646c7a37:	mov    $0x8,%ecx
+    646c7a3c:	call   646c7b90 <_lock>
+    646c7a41:	cmpq   $0x0,(%rbx)
+    646c7a45:	je     646c7aa4 <_register_onexit_function+0x84>
+    646c7a47:	mov    0x8(%rbx),%rsi
+    646c7a4b:	mov    0x10(%rbx),%rax
+    646c7a4f:	cmp    %rsi,%rax
+    646c7a52:	je     646c7a74 <_register_onexit_function+0x54>
+    646c7a54:	lea    0x8(%rsi),%rax
+    646c7a58:	mov    $0x8,%ecx
+    646c7a5d:	mov    %rax,0x8(%rbx)
+    646c7a61:	mov    %rdi,(%rsi)
+    646c7a64:	call   646c7b88 <_unlock>
+    646c7a69:	xor    %eax,%eax
+    646c7a6b:	add    $0x28,%rsp
+    646c7a6f:	pop    %rbx
+    646c7a70:	pop    %rsi
+    646c7a71:	pop    %rdi
+    646c7a72:	pop    %rbp
+    646c7a73:	ret
+    646c7a74:	mov    (%rbx),%rcx
+    646c7a77:	sub    %rcx,%rsi
+    646c7a7a:	mov    %rsi,%rax
+    646c7a7d:	sar    $0x3,%rax
+    646c7a81:	shl    $0x4,%rax
+    646c7a85:	mov    %rax,%rdx
+    646c7a88:	mov    %rax,%rbp
+    646c7a8b:	call   646c7b80 <realloc>
+    646c7a90:	test   %rax,%rax
+    646c7a93:	je     646c7ad7 <_register_onexit_function+0xb7>
+    646c7a95:	mov    %rax,(%rbx)
+    646c7a98:	add    %rax,%rsi
+    646c7a9b:	add    %rbp,%rax
+    646c7a9e:	mov    %rax,0x10(%rbx)
+    646c7aa2:	jmp    646c7a54 <_register_onexit_function+0x34>
+    646c7aa4:	mov    $0x8,%edx
+    646c7aa9:	mov    $0x20,%ecx
+    646c7aae:	call   646c79b0 <calloc>
+    646c7ab3:	test   %rax,%rax
+    646c7ab6:	mov    %rax,%rsi
+    646c7ab9:	mov    %rax,(%rbx)
+    646c7abc:	je     646c7ad7 <_register_onexit_function+0xb7>
+    646c7abe:	mov    %rax,0x8(%rbx)
+    646c7ac2:	lea    0x100(%rax),%rax
+    646c7ac9:	mov    %rax,0x10(%rbx)
+    646c7acd:	jmp    646c7a4f <_register_onexit_function+0x2f>
     646c7acf:	nop
-
-00000000646c7ad0 <__acrt_iob_func>:
-    646c7ad0:	push   %rbx
-    646c7ad1:	sub    $0x20,%rsp
-    646c7ad5:	mov    %ecx,%ebx
-    646c7ad7:	call   646c7b08 <__iob_func>
-    646c7adc:	mov    %ebx,%ecx
-    646c7ade:	lea    (%rcx,%rcx,2),%rdx
-    646c7ae2:	shl    $0x4,%rdx
-    646c7ae6:	add    %rdx,%rax
-    646c7ae9:	add    $0x20,%rsp
-    646c7aed:	pop    %rbx
-    646c7aee:	ret
-    646c7aef:	nop
-
-00000000646c7af0 <realloc>:
-    646c7af0:	jmp    *0x6836(%rip)        # 646ce32c <__imp_realloc>
-    646c7af6:	nop
-    646c7af7:	nop
-
-00000000646c7af8 <_unlock>:
-    646c7af8:	jmp    *0x67be(%rip)        # 646ce2bc <__imp__unlock>
-    646c7afe:	nop
-    646c7aff:	nop
-
-00000000646c7b00 <_lock>:
-    646c7b00:	jmp    *0x67a6(%rip)        # 646ce2ac <__imp__lock>
-    646c7b06:	nop
-    646c7b07:	nop
-
-00000000646c7b08 <__iob_func>:
-    646c7b08:	jmp    *0x6776(%rip)        # 646ce284 <__imp___iob_func>
-    646c7b0e:	nop
-    646c7b0f:	nop
-
-00000000646c7b10 <VirtualQuery>:
-    646c7b10:	jmp    *0x675e(%rip)        # 646ce274 <__imp_VirtualQuery>
-    646c7b16:	nop
-    646c7b17:	nop
-
-00000000646c7b18 <VirtualProtect>:
-    646c7b18:	jmp    *0x674e(%rip)        # 646ce26c <__imp_VirtualProtect>
-    646c7b1e:	nop
-    646c7b1f:	nop
-
-00000000646c7b20 <UnhandledExceptionFilter>:
-    646c7b20:	jmp    *0x673e(%rip)        # 646ce264 <__imp_UnhandledExceptionFilter>
-    646c7b26:	nop
-    646c7b27:	nop
-
-00000000646c7b28 <TlsGetValue>:
-    646c7b28:	jmp    *0x672e(%rip)        # 646ce25c <__imp_TlsGetValue>
-    646c7b2e:	nop
-    646c7b2f:	nop
-
-00000000646c7b30 <TerminateProcess>:
-    646c7b30:	jmp    *0x671e(%rip)        # 646ce254 <__imp_TerminateProcess>
-    646c7b36:	nop
-    646c7b37:	nop
-
-00000000646c7b38 <SetUnhandledExceptionFilter>:
-    646c7b38:	jmp    *0x6706(%rip)        # 646ce244 <__imp_SetUnhandledExceptionFilter>
-    646c7b3e:	nop
-    646c7b3f:	nop
-
-00000000646c7b40 <RtlVirtualUnwind>:
-    646c7b40:	jmp    *0x66f6(%rip)        # 646ce23c <__imp_RtlVirtualUnwind>
-    646c7b46:	nop
-    646c7b47:	nop
-
-00000000646c7b48 <RtlLookupFunctionEntry>:
-    646c7b48:	jmp    *0x66e6(%rip)        # 646ce234 <__imp_RtlLookupFunctionEntry>
-    646c7b4e:	nop
-    646c7b4f:	nop
-
-00000000646c7b50 <RtlCaptureContext>:
-    646c7b50:	jmp    *0x66d6(%rip)        # 646ce22c <__imp_RtlCaptureContext>
-    646c7b56:	nop
-    646c7b57:	nop
-
-00000000646c7b58 <RtlAddFunctionTable>:
-    646c7b58:	jmp    *0x66c6(%rip)        # 646ce224 <__imp_RtlAddFunctionTable>
-    646c7b5e:	nop
+    646c7ad0:	mov    $0xffffffff,%eax
+    646c7ad5:	jmp    646c7a6b <_register_onexit_function+0x4b>
+    646c7ad7:	mov    $0x8,%ecx
+    646c7adc:	call   646c7b88 <_unlock>
+    646c7ae1:	mov    $0xffffffff,%eax
+    646c7ae6:	jmp    646c7a6b <_register_onexit_function+0x4b>
+    646c7ae8:	nopl   0x0(%rax,%rax,1)
+
+00000000646c7af0 <_execute_onexit_table>:
+    646c7af0:	push   %rdi
+    646c7af1:	push   %rsi
+    646c7af2:	push   %rbx
+    646c7af3:	sub    $0x20,%rsp
+    646c7af7:	mov    %rcx,%rdi
+    646c7afa:	mov    $0x8,%ecx
+    646c7aff:	call   646c7b90 <_lock>
+    646c7b04:	mov    (%rdi),%rsi
+    646c7b07:	mov    $0x8,%ecx
+    646c7b0c:	movq   $0x0,0x10(%rdi)
+    646c7b14:	mov    0x8(%rdi),%rbx
+    646c7b18:	movq   $0x0,(%rdi)
+    646c7b1f:	movq   $0x0,0x8(%rdi)
+    646c7b27:	call   646c7b88 <_unlock>
+    646c7b2c:	test   %rsi,%rsi
+    646c7b2f:	je     646c7b55 <_execute_onexit_table+0x65>
+    646c7b31:	sub    $0x8,%rbx
+    646c7b35:	cmp    %rbx,%rsi
+    646c7b38:	ja     646c7b4d <_execute_onexit_table+0x5d>
+    646c7b3a:	mov    (%rbx),%rax
+    646c7b3d:	test   %rax,%rax
+    646c7b40:	je     646c7b31 <_execute_onexit_table+0x41>
+    646c7b42:	call   *%rax
+    646c7b44:	sub    $0x8,%rbx
+    646c7b48:	cmp    %rbx,%rsi
+    646c7b4b:	jbe    646c7b3a <_execute_onexit_table+0x4a>
+    646c7b4d:	mov    %rsi,%rcx
+    646c7b50:	call   646c7988 <free>
+    646c7b55:	xor    %eax,%eax
+    646c7b57:	add    $0x20,%rsp
+    646c7b5b:	pop    %rbx
+    646c7b5c:	pop    %rsi
+    646c7b5d:	pop    %rdi
+    646c7b5e:	ret
     646c7b5f:	nop
 
-00000000646c7b60 <QueryPerformanceCounter>:
-    646c7b60:	jmp    *0x66b6(%rip)        # 646ce21c <__imp_QueryPerformanceCounter>
-    646c7b66:	nop
-    646c7b67:	nop
-
-00000000646c7b68 <LeaveCriticalSection>:
-    646c7b68:	jmp    *0x66a6(%rip)        # 646ce214 <__imp_LeaveCriticalSection>
-    646c7b6e:	nop
-    646c7b6f:	nop
-
-00000000646c7b70 <InitializeCriticalSection>:
-    646c7b70:	jmp    *0x6696(%rip)        # 646ce20c <__imp_InitializeCriticalSection>
-    646c7b76:	nop
-    646c7b77:	nop
-
-00000000646c7b78 <GetTickCount>:
-    646c7b78:	jmp    *0x6686(%rip)        # 646ce204 <__imp_GetTickCount>
-    646c7b7e:	nop
+00000000646c7b60 <__acrt_iob_func>:
+    646c7b60:	push   %rbx
+    646c7b61:	sub    $0x20,%rsp
+    646c7b65:	mov    %ecx,%ebx
+    646c7b67:	call   646c7b98 <__iob_func>
+    646c7b6c:	mov    %ebx,%ecx
+    646c7b6e:	lea    (%rcx,%rcx,2),%rdx
+    646c7b72:	shl    $0x4,%rdx
+    646c7b76:	add    %rdx,%rax
+    646c7b79:	add    $0x20,%rsp
+    646c7b7d:	pop    %rbx
+    646c7b7e:	ret
     646c7b7f:	nop
 
-00000000646c7b80 <GetSystemTimeAsFileTime>:
-    646c7b80:	jmp    *0x6676(%rip)        # 646ce1fc <__imp_GetSystemTimeAsFileTime>
+00000000646c7b80 <realloc>:
+    646c7b80:	jmp    *0x67a6(%rip)        # 646ce32c <__imp_realloc>
     646c7b86:	nop
     646c7b87:	nop
 
-00000000646c7b88 <GetLastError>:
-    646c7b88:	jmp    *0x6666(%rip)        # 646ce1f4 <__imp_GetLastError>
+00000000646c7b88 <_unlock>:
+    646c7b88:	jmp    *0x672e(%rip)        # 646ce2bc <__imp__unlock>
     646c7b8e:	nop
     646c7b8f:	nop
 
-00000000646c7b90 <GetCurrentThreadId>:
-    646c7b90:	jmp    *0x6656(%rip)        # 646ce1ec <__imp_GetCurrentThreadId>
+00000000646c7b90 <_lock>:
+    646c7b90:	jmp    *0x6716(%rip)        # 646ce2ac <__imp__lock>
     646c7b96:	nop
     646c7b97:	nop
 
-00000000646c7b98 <GetCurrentProcessId>:
-    646c7b98:	jmp    *0x6646(%rip)        # 646ce1e4 <__imp_GetCurrentProcessId>
+00000000646c7b98 <__iob_func>:
+    646c7b98:	jmp    *0x66e6(%rip)        # 646ce284 <__imp___iob_func>
     646c7b9e:	nop
     646c7b9f:	nop
 
-00000000646c7ba0 <GetCurrentProcess>:
-    646c7ba0:	jmp    *0x6636(%rip)        # 646ce1dc <__imp_GetCurrentProcess>
+00000000646c7ba0 <VirtualQuery>:
+    646c7ba0:	jmp    *0x66ce(%rip)        # 646ce274 <__imp_VirtualQuery>
     646c7ba6:	nop
     646c7ba7:	nop
 
-00000000646c7ba8 <EnterCriticalSection>:
-    646c7ba8:	jmp    *0x6626(%rip)        # 646ce1d4 <__imp_EnterCriticalSection>
+00000000646c7ba8 <VirtualProtect>:
+    646c7ba8:	jmp    *0x66be(%rip)        # 646ce26c <__imp_VirtualProtect>
     646c7bae:	nop
     646c7baf:	nop
 
-00000000646c7bb0 <DeleteCriticalSection>:
-    646c7bb0:	jmp    *0x6616(%rip)        # 646ce1cc <__IAT_start__>
+00000000646c7bb0 <UnhandledExceptionFilter>:
+    646c7bb0:	jmp    *0x66ae(%rip)        # 646ce264 <__imp_UnhandledExceptionFilter>
     646c7bb6:	nop
     646c7bb7:	nop
-    646c7bb8:	nopl   0x0(%rax,%rax,1)
 
-00000000646c7bc0 <__mingw_raise_matherr>:
-    646c7bc0:	sub    $0x58,%rsp
-    646c7bc4:	mov    0x4fa5(%rip),%rax        # 646ccb70 <stUserMathErr>
-    646c7bcb:	test   %rax,%rax
-    646c7bce:	je     646c7bfc <__mingw_raise_matherr+0x3c>
-    646c7bd0:	movsd  0x80(%rsp),%xmm0
-    646c7bd9:	mov    %ecx,0x20(%rsp)
-    646c7bdd:	lea    0x20(%rsp),%rcx
-    646c7be2:	mov    %rdx,0x28(%rsp)
-    646c7be7:	movsd  %xmm2,0x30(%rsp)
-    646c7bed:	movsd  %xmm3,0x38(%rsp)
-    646c7bf3:	movsd  %xmm0,0x40(%rsp)
-    646c7bf9:	call   *%rax
-    646c7bfb:	nop
-    646c7bfc:	add    $0x58,%rsp
-    646c7c00:	ret
-    646c7c01:	nopl   0x0(%rax,%rax,1)
-    646c7c06:	cs nopw 0x0(%rax,%rax,1)
-
-00000000646c7c10 <__mingw_setusermatherr>:
-    646c7c10:	mov    %rcx,0x4f59(%rip)        # 646ccb70 <stUserMathErr>
-    646c7c17:	jmp    646c7d20 <__setusermatherr>
-    646c7c1c:	nopl   0x0(%rax)
-
-00000000646c7c20 <_matherr>:
-    646c7c20:	push   %rsi
-    646c7c21:	push   %rbx
-    646c7c22:	sub    $0x78,%rsp
-    646c7c26:	movaps %xmm6,0x40(%rsp)
-    646c7c2b:	movaps %xmm7,0x50(%rsp)
-    646c7c30:	movaps %xmm8,0x60(%rsp)
-    646c7c36:	cmpl   $0x6,(%rcx)
-    646c7c39:	ja     646c7d10 <_matherr+0xf0>
-    646c7c3f:	mov    (%rcx),%eax
-    646c7c41:	lea    0x197c(%rip),%rdx        # 646c95c4 <.rdata+0x124>
-    646c7c48:	movslq (%rdx,%rax,4),%rax
-    646c7c4c:	add    %rdx,%rax
-    646c7c4f:	jmp    *%rax
-    646c7c51:	lea    0x1848(%rip),%rbx        # 646c94a0 <.rdata>
-    646c7c58:	mov    0x8(%rcx),%rsi
-    646c7c5c:	movsd  0x20(%rcx),%xmm8
-    646c7c62:	movsd  0x18(%rcx),%xmm7
-    646c7c67:	movsd  0x10(%rcx),%xmm6
-    646c7c6c:	mov    $0x2,%ecx
-    646c7c71:	call   646c7ad0 <__acrt_iob_func>
-    646c7c76:	movsd  %xmm8,0x30(%rsp)
-    646c7c7d:	mov    %rsi,%r9
-    646c7c80:	mov    %rbx,%r8
-    646c7c83:	movsd  %xmm7,0x28(%rsp)
-    646c7c89:	lea    0x1908(%rip),%rdx        # 646c9598 <.rdata+0xf8>
-    646c7c90:	mov    %rax,%rcx
-    646c7c93:	movsd  %xmm6,0x20(%rsp)
-    646c7c99:	call   646c7900 <fprintf>
-    646c7c9e:	nop
-    646c7c9f:	movaps 0x40(%rsp),%xmm6
-    646c7ca4:	xor    %eax,%eax
-    646c7ca6:	movaps 0x50(%rsp),%xmm7
-    646c7cab:	movaps 0x60(%rsp),%xmm8
-    646c7cb1:	add    $0x78,%rsp
-    646c7cb5:	pop    %rbx
-    646c7cb6:	pop    %rsi
-    646c7cb7:	ret
-    646c7cb8:	nopl   0x0(%rax,%rax,1)
-    646c7cc0:	lea    0x17f8(%rip),%rbx        # 646c94bf <.rdata+0x1f>
-    646c7cc7:	jmp    646c7c58 <_matherr+0x38>
-    646c7cc9:	nopl   0x0(%rax)
-    646c7cd0:	lea    0x1809(%rip),%rbx        # 646c94e0 <.rdata+0x40>
-    646c7cd7:	jmp    646c7c58 <_matherr+0x38>
-    646c7cdc:	nopl   0x0(%rax)
-    646c7ce0:	lea    0x1869(%rip),%rbx        # 646c9550 <.rdata+0xb0>
-    646c7ce7:	jmp    646c7c58 <_matherr+0x38>
-    646c7cec:	nopl   0x0(%rax)
-    646c7cf0:	lea    0x1831(%rip),%rbx        # 646c9528 <.rdata+0x88>
-    646c7cf7:	jmp    646c7c58 <_matherr+0x38>
-    646c7cfc:	nopl   0x0(%rax)
-    646c7d00:	lea    0x17f9(%rip),%rbx        # 646c9500 <.rdata+0x60>
-    646c7d07:	jmp    646c7c58 <_matherr+0x38>
-    646c7d0c:	nopl   0x0(%rax)
-    646c7d10:	lea    0x186f(%rip),%rbx        # 646c9586 <.rdata+0xe6>
-    646c7d17:	jmp    646c7c58 <_matherr+0x38>
-    646c7d1c:	nop
-    646c7d1d:	nop
-    646c7d1e:	nop
-    646c7d1f:	nop
-
-00000000646c7d20 <__setusermatherr>:
-    646c7d20:	jmp    *0x6566(%rip)        # 646ce28c <__imp___setusermatherr>
-    646c7d26:	nop
-    646c7d27:	nop
-    646c7d28:	nopl   0x0(%rax,%rax,1)
-
-00000000646c7d30 <__report_error>:
-    646c7d30:	push   %rsi
-    646c7d31:	push   %rbx
-    646c7d32:	sub    $0x38,%rsp
-    646c7d36:	lea    0x58(%rsp),%rax
-    646c7d3b:	mov    %rcx,%rbx
-    646c7d3e:	mov    $0x2,%ecx
-    646c7d43:	mov    %rdx,0x58(%rsp)
-    646c7d48:	mov    %r8,0x60(%rsp)
-    646c7d4d:	mov    %r9,0x68(%rsp)
-    646c7d52:	mov    %rax,0x28(%rsp)
-    646c7d57:	call   646c7ad0 <__acrt_iob_func>
-    646c7d5c:	mov    $0x1b,%r8d
-    646c7d62:	mov    $0x1,%edx
-    646c7d67:	lea    0x1492(%rip),%rcx        # 646c9200 <.rdata>
-    646c7d6e:	mov    %rax,%r9
-    646c7d71:	call   646c78f0 <fwrite>
-    646c7d76:	mov    0x28(%rsp),%rsi
-    646c7d7b:	mov    $0x2,%ecx
-    646c7d80:	call   646c7ad0 <__acrt_iob_func>
-    646c7d85:	mov    %rbx,%rdx
-    646c7d88:	mov    %rax,%rcx
-    646c7d8b:	mov    %rsi,%r8
-    646c7d8e:	call   646c78b0 <vfprintf>
-    646c7d93:	call   646c7928 <abort>
-    646c7d98:	nop
-    646c7d99:	nop
-    646c7d9a:	nop
-    646c7d9b:	nop
-    646c7d9c:	nop
-    646c7d9d:	nop
-    646c7d9e:	nop
-    646c7d9f:	nop
-
-00000000646c7da0 <register_frame_ctor>:
-    646c7da0:	jmp    646c1390 <__gcc_register_frame>
-    646c7da5:	nop
-    646c7da6:	nop
-    646c7da7:	nop
-    646c7da8:	nop
-    646c7da9:	nop
-    646c7daa:	nop
-    646c7dab:	nop
+00000000646c7bb8 <TlsGetValue>:
+    646c7bb8:	jmp    *0x669e(%rip)        # 646ce25c <__imp_TlsGetValue>
+    646c7bbe:	nop
+    646c7bbf:	nop
+
+00000000646c7bc0 <TerminateProcess>:
+    646c7bc0:	jmp    *0x668e(%rip)        # 646ce254 <__imp_TerminateProcess>
+    646c7bc6:	nop
+    646c7bc7:	nop
+
+00000000646c7bc8 <SetUnhandledExceptionFilter>:
+    646c7bc8:	jmp    *0x6676(%rip)        # 646ce244 <__imp_SetUnhandledExceptionFilter>
+    646c7bce:	nop
+    646c7bcf:	nop
+
+00000000646c7bd0 <RtlVirtualUnwind>:
+    646c7bd0:	jmp    *0x6666(%rip)        # 646ce23c <__imp_RtlVirtualUnwind>
+    646c7bd6:	nop
+    646c7bd7:	nop
+
+00000000646c7bd8 <RtlLookupFunctionEntry>:
+    646c7bd8:	jmp    *0x6656(%rip)        # 646ce234 <__imp_RtlLookupFunctionEntry>
+    646c7bde:	nop
+    646c7bdf:	nop
+
+00000000646c7be0 <RtlCaptureContext>:
+    646c7be0:	jmp    *0x6646(%rip)        # 646ce22c <__imp_RtlCaptureContext>
+    646c7be6:	nop
+    646c7be7:	nop
+
+00000000646c7be8 <RtlAddFunctionTable>:
+    646c7be8:	jmp    *0x6636(%rip)        # 646ce224 <__imp_RtlAddFunctionTable>
+    646c7bee:	nop
+    646c7bef:	nop
+
+00000000646c7bf0 <QueryPerformanceCounter>:
+    646c7bf0:	jmp    *0x6626(%rip)        # 646ce21c <__imp_QueryPerformanceCounter>
+    646c7bf6:	nop
+    646c7bf7:	nop
+
+00000000646c7bf8 <LeaveCriticalSection>:
+    646c7bf8:	jmp    *0x6616(%rip)        # 646ce214 <__imp_LeaveCriticalSection>
+    646c7bfe:	nop
+    646c7bff:	nop
+
+00000000646c7c00 <InitializeCriticalSection>:
+    646c7c00:	jmp    *0x6606(%rip)        # 646ce20c <__imp_InitializeCriticalSection>
+    646c7c06:	nop
+    646c7c07:	nop
+
+00000000646c7c08 <GetTickCount>:
+    646c7c08:	jmp    *0x65f6(%rip)        # 646ce204 <__imp_GetTickCount>
+    646c7c0e:	nop
+    646c7c0f:	nop
+
+00000000646c7c10 <GetSystemTimeAsFileTime>:
+    646c7c10:	jmp    *0x65e6(%rip)        # 646ce1fc <__imp_GetSystemTimeAsFileTime>
+    646c7c16:	nop
+    646c7c17:	nop
+
+00000000646c7c18 <GetLastError>:
+    646c7c18:	jmp    *0x65d6(%rip)        # 646ce1f4 <__imp_GetLastError>
+    646c7c1e:	nop
+    646c7c1f:	nop
+
+00000000646c7c20 <GetCurrentThreadId>:
+    646c7c20:	jmp    *0x65c6(%rip)        # 646ce1ec <__imp_GetCurrentThreadId>
+    646c7c26:	nop
+    646c7c27:	nop
+
+00000000646c7c28 <GetCurrentProcessId>:
+    646c7c28:	jmp    *0x65b6(%rip)        # 646ce1e4 <__imp_GetCurrentProcessId>
+    646c7c2e:	nop
+    646c7c2f:	nop
+
+00000000646c7c30 <GetCurrentProcess>:
+    646c7c30:	jmp    *0x65a6(%rip)        # 646ce1dc <__imp_GetCurrentProcess>
+    646c7c36:	nop
+    646c7c37:	nop
+
+00000000646c7c38 <EnterCriticalSection>:
+    646c7c38:	jmp    *0x6596(%rip)        # 646ce1d4 <__imp_EnterCriticalSection>
+    646c7c3e:	nop
+    646c7c3f:	nop
+
+00000000646c7c40 <DeleteCriticalSection>:
+    646c7c40:	jmp    *0x6586(%rip)        # 646ce1cc <__IAT_start__>
+    646c7c46:	nop
+    646c7c47:	nop
+    646c7c48:	nopl   0x0(%rax,%rax,1)
+
+00000000646c7c50 <__mingw_raise_matherr>:
+    646c7c50:	sub    $0x58,%rsp
+    646c7c54:	mov    0x4f15(%rip),%rax        # 646ccb70 <stUserMathErr>
+    646c7c5b:	test   %rax,%rax
+    646c7c5e:	je     646c7c8c <__mingw_raise_matherr+0x3c>
+    646c7c60:	movsd  0x80(%rsp),%xmm0
+    646c7c69:	mov    %ecx,0x20(%rsp)
+    646c7c6d:	lea    0x20(%rsp),%rcx
+    646c7c72:	mov    %rdx,0x28(%rsp)
+    646c7c77:	movsd  %xmm2,0x30(%rsp)
+    646c7c7d:	movsd  %xmm3,0x38(%rsp)
+    646c7c83:	movsd  %xmm0,0x40(%rsp)
+    646c7c89:	call   *%rax
+    646c7c8b:	nop
+    646c7c8c:	add    $0x58,%rsp
+    646c7c90:	ret
+    646c7c91:	nopl   0x0(%rax,%rax,1)
+    646c7c96:	cs nopw 0x0(%rax,%rax,1)
+
+00000000646c7ca0 <__mingw_setusermatherr>:
+    646c7ca0:	mov    %rcx,0x4ec9(%rip)        # 646ccb70 <stUserMathErr>
+    646c7ca7:	jmp    646c7db0 <__setusermatherr>
+    646c7cac:	nopl   0x0(%rax)
+
+00000000646c7cb0 <_matherr>:
+    646c7cb0:	push   %rsi
+    646c7cb1:	push   %rbx
+    646c7cb2:	sub    $0x78,%rsp
+    646c7cb6:	movaps %xmm6,0x40(%rsp)
+    646c7cbb:	movaps %xmm7,0x50(%rsp)
+    646c7cc0:	movaps %xmm8,0x60(%rsp)
+    646c7cc6:	cmpl   $0x6,(%rcx)
+    646c7cc9:	ja     646c7da0 <_matherr+0xf0>
+    646c7ccf:	mov    (%rcx),%eax
+    646c7cd1:	lea    0x18ec(%rip),%rdx        # 646c95c4 <.rdata+0x124>
+    646c7cd8:	movslq (%rdx,%rax,4),%rax
+    646c7cdc:	add    %rdx,%rax
+    646c7cdf:	jmp    *%rax
+    646c7ce1:	lea    0x17b8(%rip),%rbx        # 646c94a0 <.rdata>
+    646c7ce8:	mov    0x8(%rcx),%rsi
+    646c7cec:	movsd  0x20(%rcx),%xmm8
+    646c7cf2:	movsd  0x18(%rcx),%xmm7
+    646c7cf7:	movsd  0x10(%rcx),%xmm6
+    646c7cfc:	mov    $0x2,%ecx
+    646c7d01:	call   646c7b60 <__acrt_iob_func>
+    646c7d06:	movsd  %xmm8,0x30(%rsp)
+    646c7d0d:	mov    %rsi,%r9
+    646c7d10:	mov    %rbx,%r8
+    646c7d13:	movsd  %xmm7,0x28(%rsp)
+    646c7d19:	lea    0x1878(%rip),%rdx        # 646c9598 <.rdata+0xf8>
+    646c7d20:	mov    %rax,%rcx
+    646c7d23:	movsd  %xmm6,0x20(%rsp)
+    646c7d29:	call   646c7990 <fprintf>
+    646c7d2e:	nop
+    646c7d2f:	movaps 0x40(%rsp),%xmm6
+    646c7d34:	xor    %eax,%eax
+    646c7d36:	movaps 0x50(%rsp),%xmm7
+    646c7d3b:	movaps 0x60(%rsp),%xmm8
+    646c7d41:	add    $0x78,%rsp
+    646c7d45:	pop    %rbx
+    646c7d46:	pop    %rsi
+    646c7d47:	ret
+    646c7d48:	nopl   0x0(%rax,%rax,1)
+    646c7d50:	lea    0x1768(%rip),%rbx        # 646c94bf <.rdata+0x1f>
+    646c7d57:	jmp    646c7ce8 <_matherr+0x38>
+    646c7d59:	nopl   0x0(%rax)
+    646c7d60:	lea    0x1779(%rip),%rbx        # 646c94e0 <.rdata+0x40>
+    646c7d67:	jmp    646c7ce8 <_matherr+0x38>
+    646c7d6c:	nopl   0x0(%rax)
+    646c7d70:	lea    0x17d9(%rip),%rbx        # 646c9550 <.rdata+0xb0>
+    646c7d77:	jmp    646c7ce8 <_matherr+0x38>
+    646c7d7c:	nopl   0x0(%rax)
+    646c7d80:	lea    0x17a1(%rip),%rbx        # 646c9528 <.rdata+0x88>
+    646c7d87:	jmp    646c7ce8 <_matherr+0x38>
+    646c7d8c:	nopl   0x0(%rax)
+    646c7d90:	lea    0x1769(%rip),%rbx        # 646c9500 <.rdata+0x60>
+    646c7d97:	jmp    646c7ce8 <_matherr+0x38>
+    646c7d9c:	nopl   0x0(%rax)
+    646c7da0:	lea    0x17df(%rip),%rbx        # 646c9586 <.rdata+0xe6>
+    646c7da7:	jmp    646c7ce8 <_matherr+0x38>
     646c7dac:	nop
     646c7dad:	nop
     646c7dae:	nop
     646c7daf:	nop
 
-00000000646c7db0 <__CTOR_LIST__>:
-    646c7db0:	(bad)
-    646c7db1:	(bad)
-    646c7db2:	(bad)
-    646c7db3:	(bad)
-    646c7db4:	(bad)
-    646c7db5:	(bad)
-    646c7db6:	(bad)
-    646c7db7:	jmp    *0x646c7d(%rax)
-
-00000000646c7db8 <.ctors.65535>:
-    646c7db8:	movabs 0x646c7d,%al
-    646c7dc1:	add    %al,(%rax)
-    646c7dc3:	add    %al,(%rax)
-    646c7dc5:	add    %al,(%rax)
-	...
-
-00000000646c7dc8 <__DTOR_LIST__>:
-    646c7dc8:	(bad)
-    646c7dc9:	(bad)
-    646c7dca:	(bad)
-    646c7dcb:	(bad)
-    646c7dcc:	(bad)
-    646c7dcd:	(bad)
-    646c7dce:	(bad)
-    646c7dcf:	incl   (%rax)
-    646c7dd1:	add    %al,(%rax)
-    646c7dd3:	add    %al,(%rax)
-    646c7dd5:	add    %al,(%rax)
+00000000646c7db0 <__setusermatherr>:
+    646c7db0:	jmp    *0x64d6(%rip)        # 646ce28c <__imp___setusermatherr>
+    646c7db6:	nop
+    646c7db7:	nop
+    646c7db8:	nopl   0x0(%rax,%rax,1)
+
+00000000646c7dc0 <__report_error>:
+    646c7dc0:	push   %rsi
+    646c7dc1:	push   %rbx
+    646c7dc2:	sub    $0x38,%rsp
+    646c7dc6:	lea    0x58(%rsp),%rax
+    646c7dcb:	mov    %rcx,%rbx
+    646c7dce:	mov    $0x2,%ecx
+    646c7dd3:	mov    %rdx,0x58(%rsp)
+    646c7dd8:	mov    %r8,0x60(%rsp)
+    646c7ddd:	mov    %r9,0x68(%rsp)
+    646c7de2:	mov    %rax,0x28(%rsp)
+    646c7de7:	call   646c7b60 <__acrt_iob_func>
+    646c7dec:	mov    $0x1b,%r8d
+    646c7df2:	mov    $0x1,%edx
+    646c7df7:	lea    0x1402(%rip),%rcx        # 646c9200 <.rdata>
+    646c7dfe:	mov    %rax,%r9
+    646c7e01:	call   646c7980 <fwrite>
+    646c7e06:	mov    0x28(%rsp),%rsi
+    646c7e0b:	mov    $0x2,%ecx
+    646c7e10:	call   646c7b60 <__acrt_iob_func>
+    646c7e15:	mov    %rbx,%rdx
+    646c7e18:	mov    %rax,%rcx
+    646c7e1b:	mov    %rsi,%r8
+    646c7e1e:	call   646c7940 <vfprintf>
+    646c7e23:	call   646c79b8 <abort>
+    646c7e28:	nop
+    646c7e29:	nop
+    646c7e2a:	nop
+    646c7e2b:	nop
+    646c7e2c:	nop
+    646c7e2d:	nop
+    646c7e2e:	nop
+    646c7e2f:	nop
+
+00000000646c7e30 <register_frame_ctor>:
+    646c7e30:	jmp    646c1390 <__gcc_register_frame>
+    646c7e35:	nop
+    646c7e36:	nop
+    646c7e37:	nop
+    646c7e38:	nop
+    646c7e39:	nop
+    646c7e3a:	nop
+    646c7e3b:	nop
+    646c7e3c:	nop
+    646c7e3d:	nop
+    646c7e3e:	nop
+    646c7e3f:	nop
+
+00000000646c7e40 <__CTOR_LIST__>:
+    646c7e40:	(bad)
+    646c7e41:	(bad)
+    646c7e42:	(bad)
+    646c7e43:	(bad)
+    646c7e44:	(bad)
+    646c7e45:	(bad)
+    646c7e46:	(bad)
+    646c7e47:	push   (%rax)
+
+00000000646c7e48 <.ctors.65535>:
+    646c7e48:	xor    %bh,0x6c(%rsi)
+    646c7e4b:	add    %al,%fs:(%rax)
+	...
+
+00000000646c7e58 <__DTOR_LIST__>:
+    646c7e58:	(bad)
+    646c7e59:	(bad)
+    646c7e5a:	(bad)
+    646c7e5b:	(bad)
+    646c7e5c:	(bad)
+    646c7e5d:	(bad)
+    646c7e5e:	(bad)
+    646c7e5f:	incl   (%rax)
+    646c7e61:	add    %al,(%rax)
+    646c7e63:	add    %al,(%rax)
+    646c7e65:	add    %al,(%rax)
 	...
 
 Disassembly of section .data:
 
 00000000646c8000 <__data_start__>:
-    646c8000:	sarb   0x6c(%rbp)
+    646c8000:	(bad)
+    646c8001:	jle    646c806f <__imp__initialize_onexit_table+0xf>
     646c8003:	add    %al,%fs:(%rax)
 	...
 
 00000000646c8010 <__native_vcclrit_reason>:
     646c8010:	(bad)
     646c8011:	(bad)
     646c8012:	(bad)
@@ -10664,33 +10703,31 @@
     646c8044:	add    %al,(%rax)
     646c8046:	stos   %al,%es:(%rdi)
     646c8047:	mov    $0x3fff,%eax
     646c804c:	add    %al,(%rax)
 	...
 
 00000000646c8050 <__imp__execute_onexit_table>:
-    646c8050:	(bad)
-    646c8051:	jp     646c80bf <__data_end__+0x1f>
+    646c8050:	lock jp 646c80bf <__data_end__+0x1f>
     646c8053:	add    %al,%fs:(%rax)
 	...
 
 00000000646c8058 <__imp__register_onexit_function>:
-    646c8058:	nop
-    646c8059:	jns    646c80c7 <__data_end__+0x27>
+    646c8058:	and    %bh,0x6c(%rdx)
     646c805b:	add    %al,%fs:(%rax)
 	...
 
 00000000646c8060 <__imp__initialize_onexit_table>:
-    646c8060:	(bad)
-    646c8061:	jns    646c80cf <__data_end__+0x2f>
+    646c8060:	lock jns 646c80cf <__data_end__+0x2f>
     646c8063:	add    %al,%fs:(%rax)
 	...
 
 00000000646c8070 <__imp___acrt_iob_func>:
-    646c8070:	sarb   0x6c(%rdx)
+    646c8070:	(bad)
+    646c8071:	jnp    646c80df <__data_end__+0x3f>
     646c8073:	add    %al,%fs:(%rax)
 	...
 
 00000000646c8080 <__security_cookie>:
     646c8080:	xor    0x2b992ddf(%rdx),%ah
 	...
 
@@ -10752,19 +10789,16 @@
     646c905c:	add    %al,(%rax)
     646c905e:	lock (bad)
 
 00000000646c9060 <.rdata>:
     646c9060:	add    %al,(%rax)
     646c9062:	add    %al,(%rax)
     646c9064:	add    %al,(%rax)
-    646c9066:	lock (bad)
-    646c9068:	add    %al,(%rax)
-    646c906a:	add    %al,(%rax)
-    646c906c:	add    %al,(%rax)
-    646c906e:	loopne 646c90af <.rdata+0x1f>
+    646c9066:	loopne 646c90a7 <.rdata+0x17>
+	...
     646c9070:	(bad)
     646c9071:	(bad)
     646c9072:	(bad)
     646c9073:	(bad)
     646c9074:	(bad)
     646c9075:	(bad)
     646c9076:	(bad)
@@ -10884,17 +10918,15 @@
     646c9180:	add    $0x6c,%bh
     646c9183:	add    %al,%fs:(%rax)
     646c9186:	add    %al,(%rax)
     646c9188:	movabs 0x646cc2,%al
 	...
 
 00000000646c91a0 <__dyn_tls_init_callback>:
-    646c91a0:	lock push %rsi
-    646c91a2:	insb   (%dx),%es:(%rdi)
-    646c91a3:	add    %al,%fs:(%rax)
+    646c91a0:	adcb   $0x64,0x6c(%rdi)
 	...
 
 00000000646c91c0 <_tls_used>:
     646c91c0:	add    %al,(%rax)
     646c91c2:	insl   (%dx),%es:(%rdi)
     646c91c3:	add    %al,%fs:(%rax)
     646c91c6:	add    %al,(%rax)
@@ -11306,35 +11338,31 @@
     646c95b1:	and    $0x20202967,%eax
     646c95b6:	sub    %dh,0x65(%rdx)
     646c95b9:	je     646c9631 <.refptr.__image_base__+0x1>
     646c95bb:	(bad)
     646c95bc:	insb   (%dx),%es:(%rdi)
     646c95bd:	cmp    $0xa296725,%eax
     646c95c2:	add    %al,(%rax)
-    646c95c4:	rex.WR out %eax,$0xff
-    646c95c7:	decl   -0x300001a(%rbp)
-    646c95cd:	out    %al,$0xff
-    646c95cf:	decl   (%rdi,%riz,8)
-    646c95d2:	(bad)
-    646c95d3:	lcall  *(%rdi,%riz,8)
+    646c95c4:	fsub   %st,%st(7)
+    646c95c6:	(bad)
+    646c95c7:	lcall  *-0x73000019(%rip)        # fffffffff16c95b4 <.debug_str+0xffffffff8cff15b4>
+    646c95cd:	out    %eax,$0xff
+    646c95cf:	lcall  *-0x18530001(%rdi,%riz,8)
     646c95d6:	(bad)
-    646c95d7:	ljmp   *(%rdi,%riz,8)
-    646c95da:	(bad)
-    646c95db:	(bad)
-    646c95dc:	cmp    $0xe7,%al
-    646c95de:	(bad)
+    646c95d7:	(bad)
+    646c95d8:	mov    $0xccffffe7,%esp
+    646c95dd:	out    %eax,$0xff
     646c95df:	jmp    *(%rax)
 
 00000000646c95e0 <.refptr._CRT_MT>:
     646c95e0:	and    %al,0x646c(%rax)
 	...
 
 00000000646c95f0 <.refptr.__CTOR_LIST__>:
-    646c95f0:	mov    $0x7d,%al
-    646c95f2:	insb   (%dx),%es:(%rdi)
+    646c95f0:	rex jle 646c965f <.refptr.__native_startup_lock+0xf>
     646c95f3:	add    %al,%fs:(%rax)
 	...
 
 00000000646c9600 <.refptr.__RUNTIME_PSEUDO_RELOC_LIST_END__>:
     646c9600:	add    %bl,0x646c(%rcx)
 	...
 
@@ -11883,458 +11911,459 @@
     646ca1f9:	cs add %al,(%rax)
     646ca1fc:	mov    $0xd800002e,%edx
     646ca201:	mov    $0x0,%cl
 	...
 
 00000000646ca204 <.pdata>:
     646ca204:	shrb   $0x0,(%rsi)
-    646ca207:	add    %al,(%rsi)
-    646ca209:	(bad)
+    646ca207:	add    %ah,(%rdi,%rbp,1)
     646ca20a:	add    %al,(%rax)
-    646ca20c:	call   6a6ca2c2 <.debug_str+0x5ff22c2>
+    646ca20c:	call   886ca2c2 <.debug_str+0x23ff22c2>
     646ca211:	(bad)
     646ca212:	add    %al,(%rax)
-    646ca214:	iret
-    646ca215:	(bad)
-    646ca216:	add    %al,(%rax)
-    646ca218:	lock mov $0x0,%cl
-    646ca21b:	add    %cl,%bh
-    646ca21d:	(bad)
-    646ca21e:	add    %al,(%rax)
-    646ca220:	(bad)  (%rax)
+    646ca214:	cs xor %al,(%rax)
+    646ca217:	add    %dh,%al
+    646ca219:	mov    $0x0,%cl
+    646ca21b:	add    %ch,(%rsi)
+    646ca21d:	xor    %al,(%rax)
+    646ca21f:	add    %bh,0x31(%rbx)
     646ca222:	add    %al,(%rax)
     646ca224:	cld
     646ca225:	mov    $0x0,%cl
 	...
 
 00000000646ca228 <.pdata>:
-    646ca228:	loopne 646ca25a <.pdata+0x32>
-    646ca22a:	add    %al,(%rax)
-    646ca22c:	xchg   %eax,%ecx
-    646ca22d:	xor    %eax,(%rax)
+    646ca228:	xorb   $0x0,(%rcx)
+    646ca22b:	add    %dh,(%rcx)
+    646ca22d:	xor    (%rax),%al
     646ca22f:	add    %cl,(%rax)
     646ca231:	mov    $0x0,%dl
-    646ca233:	add    %dl,-0x42ffffcf(%rcx)
-    646ca239:	xor    %eax,(%rax)
-    646ca23b:	add    %dl,(%rdx,%rsi,4)
+    646ca233:	add    %dh,(%rcx)
+    646ca235:	xor    (%rax),%al
+    646ca237:	add    %bl,0x32(%rbp)
+    646ca23a:	add    %al,(%rax)
+    646ca23c:	adc    $0xb2,%al
     646ca23e:	add    %al,(%rax)
-    646ca240:	mov    $0x13000031,%ebp
-    646ca245:	xor    $0x0,%al
-    646ca247:	add    %bl,(%rdx,%rsi,4)
-    646ca24a:	add    %al,(%rax)
-    646ca24c:	adc    (%rax,%rax,1),%esi
-    646ca24f:	add    %bh,0x28000038(%rip)        # 8c6ca28d <.debug_str+0x27ff228d>
+    646ca240:	pop    %rbp
+    646ca241:	xor    (%rax),%al
+    646ca243:	add    %bh,0x1c000034(%rcx)
+    646ca249:	mov    $0x0,%dl
+    646ca24b:	add    %bh,-0x38ffffcc(%rcx)
+    646ca251:	cmp    %al,(%rax)
+    646ca253:	add    %ch,(%rax)
     646ca255:	mov    $0x0,%dl
-    646ca257:	add    %bh,-0x25ffffc8(%rip)        # 3e6ca295 <__size_of_stack_reserve__+0x3e4ca295>
-    646ca25d:	cmp    %eax,(%rax)
-    646ca25f:	add    %bh,(%rax)
-    646ca261:	mov    $0x0,%dl
-    646ca263:	add    %bl,%dl
-    646ca265:	cmp    %eax,(%rax)
-    646ca267:	add    %ah,(%rbx,%rdi,1)
-    646ca26a:	add    %al,(%rax)
-    646ca26c:	rex.R mov $0x0,%dl
+    646ca257:	add    %al,%bh
+    646ca259:	cmp    %al,(%rax)
+    646ca25b:	add    %bh,0x3a(%rbx)
+    646ca25e:	add    %al,(%rax)
+    646ca260:	cmp    %dh,0x3a7b0000(%rdx)
+    646ca266:	add    %al,(%rax)
+    646ca268:	(bad)
+    646ca26b:	add    %al,0x0(%rdx,%rsi,4)
 	...
 
 00000000646ca270 <.pdata>:
-    646ca270:	xor    %bh,(%rbx)
+    646ca270:	sarb   (%rbx)
     646ca272:	add    %al,(%rax)
-    646ca274:	jp     646ca2b1 <.pdata+0x41>
-    646ca276:	add    %al,(%rax)
-    646ca278:	push   %rax
-    646ca279:	mov    $0x0,%dl
-    646ca27b:	add    %bh,0x3b(%rdx)
-    646ca27e:	add    %al,(%rax)
-    646ca280:	clc
-    646ca281:	ds add %al,(%rax)
-    646ca284:	pop    %rsp
+    646ca274:	sbb    (%rax,%rax,1),%bh
+    646ca277:	add    %dl,-0x4e(%rax)
+    646ca27a:	add    %al,(%rax)
+    646ca27c:	sbb    (%rax,%rax,1),%bh
+    646ca27f:	add    %bl,0x5c00003f(%rax)
     646ca285:	mov    $0x0,%dl
-    646ca287:	add    %bh,%al
-    646ca289:	ds add %al,(%rax)
-    646ca28c:	mov    %eax,0x0(%rdx)
-    646ca28f:	add    %ch,0x0(%rdx,%rsi,4)
-    646ca293:	add    %cl,-0x1effffbe(%rcx)
-    646ca299:	rex.X add %al,(%rax)
-    646ca29c:	js     646ca250 <.pdata+0x28>
-    646ca29e:	add    %al,(%rax)
-    646ca2a0:	loope  646ca2e4 <.pdata+0x8>
-    646ca2a2:	add    %al,(%rax)
-    646ca2a4:	cmp    $0x84000043,%eax
-    646ca2a9:	mov    $0x0,%dl
-    646ca2ab:	add    %bh,-0xfffffbd(%rip)        # 546ca2f4 <__size_of_stack_reserve__+0x544ca2f4>
-    646ca2b1:	rex.XB add %al,(%r8)
+    646ca287:	add    %bl,0x2900003f(%rax)
+    646ca28d:	rex.XB add %al,(%r8)
+    646ca290:	insb   (%dx),%es:(%rdi)
+    646ca291:	mov    $0x0,%dl
+    646ca293:	add    %ch,(%rcx)
+    646ca295:	rex.XB add %al,(%r8)
+    646ca298:	addl   $0xb27800,0x0(%rbx)
+    646ca29f:	add    %al,-0x22ffffbd(%rcx)
+    646ca2a5:	rex.XB add %al,(%r8)
+    646ca2a8:	test   %dh,0x43dd0000(%rdx)
+    646ca2ae:	add    %al,(%rax)
+    646ca2b0:	nop
+    646ca2b1:	add    %r8b,(%rax)
     646ca2b4:	nop
     646ca2b5:	mov    $0x0,%dl
-    646ca2b7:	add    %dh,%al
-    646ca2b9:	rex.XB add %al,(%r8)
-    646ca2bc:	jge    646ca302 <.pdata+0x26>
-    646ca2be:	add    %al,(%rax)
+    646ca2b7:	add    %dl,0x1d000044(%rax)
+    646ca2bd:	add    %r8b,(%r8)
     646ca2c0:	pushf
     646ca2c1:	mov    $0x0,%dl
-    646ca2c3:	add    %bh,0x44(%rbp)
-    646ca2c6:	add    %al,(%rax)
-    646ca2c8:	sub    0x0(%rsi),%eax
-    646ca2cb:	add    %ch,0x300000b2(%rax)
+    646ca2c3:	add    %bl,-0x34ffffbb(%rip)        # 2f6ca30e <__size_of_stack_reserve__+0x2f4ca30e>
+    646ca2c9:	rex.RX add %r8b,(%rax)
+    646ca2cc:	test   $0xb2,%al
+	...
 
 00000000646ca2d0 <.pdata>:
-    646ca2d0:	xor    %al,0x0(%rsi)
-    646ca2d3:	add    %bl,%bh
-    646ca2d5:	rex.RX add %r8b,(%rax)
+    646ca2d0:	rolb   0x0(%rsi)
+    646ca2d3:	add    %bh,0x47(%rdi)
+    646ca2d6:	add    %al,(%rax)
     646ca2d8:	mov    $0xb2,%ah
 	...
 
 00000000646ca2dc <.pdata>:
-    646ca2dc:	loopne 646ca324 <.pdata+0x18>
-    646ca2de:	add    %al,(%rax)
-    646ca2e0:	rex.RB
-    646ca2e1:	rex.RXB add %r8b,(%r8)
-    646ca2e4:	shlb   $0x0,0x47450000(%rdx)
-    646ca2eb:	add    %cl,(%rax)
-    646ca2ed:	rex.WR add %r8b,(%rax)
-    646ca2f0:	int3
+    646ca2dc:	addb   $0x0,0x0(%rdi)
+    646ca2e0:	in     $0x47,%eax
+    646ca2e2:	add    %al,(%rax)
+    646ca2e4:	shlb   $0x0,0x47e50000(%rdx)
+    646ca2eb:	add    %bl,-0x33ffffb4(%rbx)
     646ca2f1:	mov    $0x0,%dl
-    646ca2f3:	add    %cl,(%rax)
-    646ca2f5:	rex.WR add %r8b,(%rax)
-    646ca2f8:	sub    0x0(%rax,%rax,1),%ecx
-    646ca2fc:	fdivs  0x4c2b0000(%rdx)
+    646ca2f3:	add    %bl,-0x41ffffb4(%rbx)
+    646ca2f9:	rex.WR add %r8b,(%rax)
+    646ca2fc:	fdivs  0x4cbe0000(%rdx)
     646ca302:	add    %al,(%rax)
-    646ca304:	test   %ecx,0x0(%rax,%rax,1)
-    646ca308:	in     $0xb2,%al
+    646ca304:	sbb    %cl,0x0(%rbp)
+    646ca307:	add    %ah,%ah
+    646ca309:	mov    $0x0,%dl
 	...
 
 00000000646ca30c <.pdata>:
-    646ca30c:	nop
-    646ca30d:	rex.WR add %r8b,(%rax)
-    646ca310:	and    %cl,0x0(%rsi)
-    646ca313:	add    %dh,%al
+    646ca30c:	and    %cl,0x0(%rbp)
+    646ca30f:	add    %dh,-0xfffffb2(%rax)
     646ca315:	mov    $0x0,%dl
-    646ca317:	add    %ah,(%rax)
-    646ca319:	rex.WRX add %r8b,(%rax)
-    646ca31c:	and    %edx,0x0(%rax)
-    646ca31f:	add    %bh,%ah
+    646ca317:	add    %dh,-0x4effffb2(%rax)
+    646ca31d:	push   %rax
+    646ca31e:	add    %al,(%rax)
+    646ca320:	cld
     646ca321:	mov    $0x0,%dl
-    646ca323:	add    %ah,(%rcx)
-    646ca325:	push   %rax
-    646ca326:	add    %al,(%rax)
-    646ca328:	mov    %dl,0x0(%rax)
-    646ca32b:	add    %cl,(%rax)
-    646ca32d:	mov    $0x0,%bl
-	...
+    646ca323:	add    %dh,0x18000050(%rcx)
+    646ca329:	push   %rcx
+    646ca32a:	add    %al,(%rax)
+    646ca32c:	or     %dh,0x51200000(%rbx)
 
 00000000646ca330 <.pdata>:
-    646ca330:	nop
-    646ca331:	push   %rax
-    646ca332:	add    %al,(%rax)
-    646ca334:	or     $0x53,%al
-    646ca336:	add    %al,(%rax)
-    646ca338:	adc    $0xb3,%al
+    646ca330:	and    %dl,0x0(%rcx)
+    646ca333:	add    %bl,-0x4cec0000(%rbx,%rdx,2)
     646ca33a:	add    %al,(%rax)
-    646ca33c:	or     $0x53,%al
+    646ca33c:	pushf
+    646ca33d:	push   %rbx
     646ca33e:	add    %al,(%rax)
-    646ca340:	hlt
-    646ca341:	push   %rbx
-    646ca342:	add    %al,(%rax)
+    646ca340:	test   %dl,0x0(%rax,%rax,1)
     646ca344:	and    $0xb3,%al
 	...
 
 00000000646ca348 <.pdata>:
-    646ca348:	adc    %dl,0x0(%rax,%rax,1)
-    646ca34c:	rex.RB push %r12
-    646ca34e:	add    %al,(%rax)
-    646ca350:	xor    %dh,0x54500000(%rbx)
+    646ca348:	movabs 0x30000054d5000054,%al
+    646ca351:	mov    $0x0,%bl
+    646ca353:	add    %ah,%al
+    646ca355:	push   %rsp
     646ca356:	add    %al,(%rax)
-    646ca358:	mov    $0x54,%dh
+    646ca358:	rex.RX push %rbp
     646ca35a:	add    %al,(%rax)
-    646ca35c:	cmp    %dh,0x54c00000(%rbx)
+    646ca35c:	cmp    %dh,0x55500000(%rbx)
     646ca362:	add    %al,(%rax)
-    646ca364:	fists  0x0(%rax,%rax,1)
+    646ca364:	outsl  %ds:(%rsi),(%dx)
+    646ca365:	push   %rbp
+    646ca366:	add    %al,(%rax)
     646ca368:	rex.R mov $0x0,%bl
 	...
 
 00000000646ca36c <.pdata>:
-    646ca36c:	loopne 646ca3c2 <.pdata.unlikely+0x2>
+    646ca36c:	jo     646ca3c3 <.pdata.unlikely+0x3>
     646ca36e:	add    %al,(%rax)
-    646ca370:	mov    $0x55,%dh
+    646ca370:	rex.RX push %rsi
     646ca372:	add    %al,(%rax)
     646ca374:	rex.W mov $0x0,%bl
-    646ca377:	add    %al,%al
-    646ca379:	push   %rbp
+    646ca377:	add    %dl,0x56(%rax)
     646ca37a:	add    %al,(%rax)
-    646ca37c:	mov    $0x58000056,%eax
+    646ca37c:	rex.W push %rdi
+    646ca37e:	add    %al,(%rax)
+    646ca380:	pop    %rax
     646ca381:	mov    $0x0,%bl
 	...
 
 00000000646ca384 <.pdata>:
-    646ca384:	rclb   $0x0,0x0(%rsi)
-    646ca388:	out    %eax,(%dx)
-    646ca389:	push   %rsi
+    646ca384:	push   %rax
+    646ca385:	push   %rdi
+    646ca386:	add    %al,(%rax)
+    646ca388:	jg     646ca3e1 <.pdata+0x15>
     646ca38a:	add    %al,(%rax)
-    646ca38c:	push   $0xfffffffff00000b3
-    646ca391:	push   %rsi
+    646ca38c:	push   $0xffffffff800000b3
+    646ca391:	push   %rdi
     646ca392:	add    %al,(%rax)
-    646ca394:	movsxd 0x0(%rdi),%edx
-    646ca397:	add    %dh,-0x4d(%rax)
+    646ca394:	repz push %rdi
+    646ca396:	add    %al,(%rax)
+    646ca398:	jo     646ca34d <.pdata+0x5>
     646ca39a:	add    %al,(%rax)
-    646ca39c:	jo     646ca3f5 <.pdata+0x11>
-    646ca39e:	add    %al,(%rax)
-    646ca3a0:	jae    646ca3f9 <.pdata+0x15>
+    646ca39c:	add    %bl,0x0(%rax)
+    646ca39f:	add    %al,(%rbx)
+    646ca3a1:	pop    %rax
     646ca3a2:	add    %al,(%rax)
     646ca3a4:	jl     646ca359 <.pdata+0x11>
 	...
 
 00000000646ca3a8 <.pdata>:
-    646ca3a8:	adcb   $0x0,0x0(%rdi)
-    646ca3ac:	test   %dl,0x0(%rdi)
-    646ca3af:	add    %al,-0x6fffff4d(%rax)
-    646ca3b5:	push   %rdi
-    646ca3b6:	add    %al,(%rax)
-    646ca3b8:	xchg   %eax,%esp
-    646ca3b9:	push   %rdi
+    646ca3a8:	adc    %bl,0x0(%rax)
+    646ca3ab:	add    %dl,(%rax,%rbx,2)
+    646ca3ae:	add    %al,(%rax)
+    646ca3b0:	xorb   $0x0,0x58200000(%rbx)
+    646ca3b7:	add    %ah,(%rax,%rbx,2)
     646ca3ba:	add    %al,(%rax)
-    646ca3bc:	test   %dh,0x57a00000(%rbx)
+    646ca3bc:	test   %dh,0x58300000(%rbx)
 
 00000000646ca3c0 <.pdata.unlikely>:
-    646ca3c0:	movabs 0x940000596d000057,%al
+    646ca3c0:	xor    %bl,0x0(%rax)
+    646ca3c3:	add    %bh,%ch
+    646ca3c5:	pop    %rcx
+    646ca3c6:	add    %al,(%rax)
+    646ca3c8:	xchg   %eax,%esp
     646ca3c9:	mov    $0x0,%bl
 	...
 
 00000000646ca3cc <.pdata>:
-    646ca3cc:	jo     646ca427 <.pdata+0x1f>
-    646ca3ce:	add    %al,(%rax)
-    646ca3d0:	sub    0x0(%rax,%rax,1),%ebx
-    646ca3d4:	movsb  %ds:(%rsi),%es:(%rdi)
+    646ca3cc:	add    %bl,0x0(%rdx)
+    646ca3cf:	add    %bh,-0x5bffffa4(%rbx)
     646ca3d5:	mov    $0x0,%bl
-    646ca3d7:	add    %dh,(%rax)
+    646ca3d7:	add    %al,%al
     646ca3d9:	pop    %rsp
     646ca3da:	add    %al,(%rax)
-    646ca3dc:	rcrb   0x0(%rbp)
-    646ca3df:	add    %bh,0x5dd00000(%rbx,%rsi,4)
+    646ca3dc:	(bad)
+    646ca3dd:	pop    %rsi
+    646ca3de:	add    %al,(%rax)
+    646ca3e0:	mov    $0x600000b3,%esp
 
 00000000646ca3e4 <.pdata>:
-    646ca3e4:	rcrb   0x0(%rbp)
-    646ca3e7:	add    %bh,-0x4c3c0000(%rsi,%rbx,2)
-    646ca3ee:	add    %al,(%rax)
-    646ca3f0:	rcrb   $0x0,0x0(%rsi)
-    646ca3f4:	cmpsl  %es:(%rdi),%ds:(%rsi)
+    646ca3e4:	(bad)
+    646ca3e5:	pop    %rsi
+    646ca3e6:	add    %al,(%rax)
+    646ca3e8:	rex.WR pop %rdi
+    646ca3ea:	add    %al,(%rax)
+    646ca3ec:	(bad)
+    646ca3ed:	mov    $0x0,%bl
+    646ca3ef:	add    %dl,0x5f(%rax)
+    646ca3f2:	add    %al,(%rax)
+    646ca3f4:	(bad)
     646ca3f5:	(bad)
     646ca3f6:	add    %al,(%rax)
     646ca3f8:	(bad)
     646ca3f9:	mov    $0x0,%bl
-    646ca3fb:	add    %dh,0x1a000060(%rax)
+    646ca3fb:	add    %al,0x61(%rax)
+    646ca3fe:	add    %al,(%rax)
+    646ca400:	stos   %al,%es:(%rdi)
     646ca401:	(bad)
     646ca402:	add    %al,(%rax)
-    646ca404:	fdivl  0x61200000(%rbx)
+    646ca404:	fdivl  0x61b00000(%rbx)
 
 00000000646ca408 <.pdata>:
-    646ca408:	and    %ah,0x0(%rcx)
-    646ca40b:	add    %bl,-0x13ffff9f(%rdi)
+    646ca408:	mov    $0x61,%al
+    646ca40a:	add    %al,(%rax)
+    646ca40c:	(bad)
+    646ca40d:	(bad)
+    646ca40e:	add    %al,(%rax)
+    646ca410:	in     (%dx),%al
     646ca411:	mov    $0x0,%bl
-    646ca413:	add    %ah,0x40000061(%rax)
-    646ca419:	(bad)
-    646ca41a:	add    %al,(%rax)
-    646ca41c:	cld
+    646ca413:	add    %dh,(%rax)
+    646ca415:	(bad)
+    646ca416:	add    %al,(%rax)
+    646ca418:	shlb   0x0(%rdx)
+    646ca41b:	add    %bh,%ah
     646ca41d:	mov    $0x0,%bl
-    646ca41f:	add    %al,0x62(%rax)
+    646ca41f:	add    %dl,%al
+    646ca421:	(bad)
     646ca422:	add    %al,(%rax)
-    646ca424:	sbb    0x0(%rbx),%ah
+    646ca424:	stos   %al,%es:(%rdi)
+    646ca425:	movsxd (%rax),%eax
     646ca427:	add    %al,(%rsp,%rsi,4)
     646ca42a:	add    %al,(%rax)
-    646ca42c:	and    %ah,0x0(%rbx)
-    646ca42f:	add    %bh,(%rsi)
+    646ca42c:	mov    $0x63,%al
+    646ca42e:	add    %al,(%rax)
+    646ca430:	(bad)
     646ca431:	movsxd (%rax),%eax
     646ca433:	add    %cl,(%rsp,%rsi,4)
 	...
 
 00000000646ca438 <.pdata>:
-    646ca438:	rex movsxd (%rax),%eax
-    646ca43b:	add    %dl,0x63(%rdx)
-    646ca43e:	add    %al,(%rax)
-    646ca440:	adc    %dh,0x636000(%rax,%rax,1)
-    646ca447:	add    %ah,-0x4bec0000(%rbx,%riz,2)
+    646ca438:	shlb   0x0(%rbx)
+    646ca43b:	add    %ah,%dl
+    646ca43d:	movsxd (%rax),%eax
+    646ca43f:	add    %dl,(%rax)
+    646ca441:	mov    $0x0,%ah
+    646ca443:	add    %dh,%al
+    646ca445:	movsxd (%rax),%eax
+    646ca447:	add    %dh,(%rsp,%riz,2)
+    646ca44a:	add    %al,(%rax)
+    646ca44c:	adc    $0xb4,%al
     646ca44e:	add    %al,(%rax)
-    646ca450:	mov    $0x63,%al
-    646ca452:	add    %al,(%rax)
-    646ca454:	cmp    $0x18000064,%eax
-    646ca459:	mov    $0x0,%ah
-    646ca45b:	add    %al,0x64(%rax)
-    646ca45e:	add    %al,(%rax)
-    646ca460:	mov    $0x64,%ah
-    646ca462:	add    %al,(%rax)
-    646ca464:	and    $0xb4,%al
+    646ca450:	rex
+    646ca451:	add    %al,%fs:(%rax)
+    646ca454:	int    $0x64
+    646ca456:	add    %al,(%rax)
+    646ca458:	sbb    %dh,0x64d000(%rax,%rax,1)
+    646ca45f:	add    %al,0x0(%rbp,%riz,2)
+    646ca463:	add    %ah,(%rsp,%rsi,4)
     646ca466:	add    %al,(%rax)
-    646ca468:	shlb   $0xfe,0x0(%rax,%rax,1)
-    646ca46d:	add    %al,%fs:(%rax)
-    646ca470:	sub    $0xb4,%al
+    646ca468:	push   %rax
+    646ca469:	add    %al,%gs:(%rax)
+    646ca46c:	mov    0x0(%rbp),%fs
+    646ca46f:	add    %ch,(%rsp,%rsi,4)
     646ca472:	add    %al,(%rax)
-    646ca474:	add    %ah,0x0(%rbp)
-    646ca477:	add    %ch,0x65(%rdi)
-    646ca47a:	add    %al,(%rax)
-    646ca47c:	xor    $0xb4,%al
+    646ca474:	nop
+    646ca475:	add    %al,%gs:(%rax)
+    646ca478:	jmp    *0x0(%rbp)
+    646ca47b:	add    %dh,(%rsp,%rsi,4)
     646ca47e:	add    %al,(%rax)
-    646ca480:	jo     646ca4e7 <.pdata+0x7>
-    646ca482:	add    %al,(%rax)
-    646ca484:	cmpsl  %es:(%rdi),%ds:(%rsi)
-    646ca485:	add    %al,%gs:(%rax)
+    646ca480:	add    %ah,0x0(%rsi)
+    646ca483:	add    %dh,(%rdi)
+    646ca485:	data16 add %al,(%rax)
     646ca488:	cmp    $0xb4,%al
     646ca48a:	add    %al,(%rax)
-    646ca48c:	mov    $0x65,%al
-    646ca48e:	add    %al,(%rax)
-    646ca490:	rex.B
-    646ca491:	data16 add %al,(%rax)
-    646ca494:	rex.R mov $0x0,%spl
-    646ca497:	add    %dl,0x66(%rax)
-    646ca49a:	add    %al,(%rax)
-    646ca49c:	mulb   0x0(%rsi)
+    646ca48c:	rex
+    646ca48d:	data16 add %al,(%rax)
+    646ca490:	shll   0x0(%rsi)
+    646ca493:	add    %al,0x0(%rsp,%rsi,4)
+    646ca497:	add    %ah,%al
+    646ca499:	data16 add %al,(%rax)
+    646ca49c:	xchg   %ah,0x0(%rdi)
     646ca49f:	add    %cl,0x0(%rsp,%rsi,4)
-    646ca4a3:	add    %al,(%rax)
-    646ca4a5:	add    %al,(%eax)
-    646ca4a8:	add    0x0(%rdi),%esp
-    646ca4ab:	add    %dl,0x0(%rsp,%rsi,4)
+    646ca4a3:	add    %dl,-0x6cffff99(%rax)
+    646ca4a9:	add    %al,(%eax)
+    646ca4ac:	push   %rsp
+    646ca4ad:	mov    $0x0,%ah
 	...
 
 00000000646ca4b0 <.pdata>:
-    646ca4b0:	push   %rax
-    646ca4b1:	add    %al,(%eax)
-    646ca4b4:	push   %rsi
-    646ca4b5:	add    %al,(%eax)
+    646ca4b0:	loopne 646ca519 <.pdata+0x9>
+    646ca4b2:	add    %al,(%rax)
+    646ca4b4:	out    %al,$0x67
+    646ca4b6:	add    %al,(%rax)
     646ca4b8:	pop    %rax
     646ca4b9:	mov    $0x0,%ah
 	...
 
 00000000646ca4bc <.pdata>:
-    646ca4bc:	(bad)
-    646ca4bd:	add    %al,(%eax)
-    646ca4c0:	data16 add %al,(%eax)
-    646ca4c4:	pop    %rsp
-    646ca4c5:	mov    $0x0,%ah
+    646ca4bc:	lock add %al,(%eax)
+    646ca4c0:	mulb   0x0(%rdi)
+    646ca4c3:	add    %bl,0x0(%rsp,%rsi,4)
 	...
 
 00000000646ca4c8 <.pdata>:
-    646ca4c8:	jo     646ca531 <.pdata+0x9>
-    646ca4ca:	add    %al,(%rax)
-    646ca4cc:	(bad)
-    646ca4cd:	add    %al,(%eax)
-    646ca4d0:	(bad)
-    646ca4d1:	mov    $0x0,%ah
+    646ca4c8:	add    %ch,0x0(%rax)
+    646ca4cb:	add    %dl,0x0(%rax,%rbp,2)
+    646ca4cf:	add    %ah,-0x4c(%rax)
 	...
 
 00000000646ca4d4 <.pdata>:
-    646ca4d4:	shlb   0x0(%rdi)
-    646ca4d7:	add    %dh,%dh
-    646ca4d9:	push   $0xffffffffb4640000
+    646ca4d4:	(bad)
+    646ca4d5:	push   $0x69860000
+    646ca4da:	add    %al,(%rax)
+    646ca4dc:	fs mov $0x0,%ah
 	...
 
 00000000646ca4e0 <.pdata>:
-    646ca4e0:	add    %ch,0x0(%rcx)
-    646ca4e3:	add    %al,0x70000069(%rip)        # d46ca552 <.debug_str+0x6fff2552>
-    646ca4e9:	mov    $0x0,%ah
+    646ca4e0:	nop
+    646ca4e1:	imul   $0x699500,(%rax),%eax
+    646ca4e7:	add    %dh,-0x4c(%rax)
 	...
 
 00000000646ca4ec <.pdata>:
-    646ca4ec:	adc    %ch,0x0(%rcx)
-    646ca4ef:	add    %ah,%bh
-    646ca4f1:	imul   $0xb47400,(%rax),%eax
+    646ca4ec:	movabs 0x7400006a77000069,%al
+    646ca4f5:	mov    $0x0,%ah
 	...
 
 00000000646ca4f8 <.pdata>:
-    646ca4f8:	lock imul $0x6ae400,(%rax),%eax
-    646ca4ff:	add    %bh,-0x4c(%rax)
+    646ca4f8:	subb   $0x0,0x0(%rdx)
+    646ca4fc:	je     646ca569 <.pdata+0x11>
+    646ca4fe:	add    %al,(%rax)
+    646ca500:	js     646ca4b6 <.pdata+0x6>
 	...
 
 00000000646ca504 <.pdata>:
-    646ca504:	and    %ch,0x0(%rbx)
-    646ca507:	add    %al,-0x4b7c0000(,%rbp,2)
-	...
+    646ca504:	mov    $0x6b,%al
+    646ca506:	add    %al,(%rax)
+    646ca508:	xchg   %eax,%esp
+    646ca509:	insl   (%dx),%es:(%rdi)
+    646ca50a:	add    %al,(%rax)
+    646ca50c:	test   %dh,0x6da000(%rax,%rax,1)
 
 00000000646ca510 <.pdata>:
-    646ca510:	adc    %ch,0x0(%rbp)
-    646ca513:	add    %dh,(%rax)
-    646ca515:	outsb  %ds:(%rsi),(%dx)
-    646ca516:	add    %al,(%rax)
-    646ca518:	nop
+    646ca510:	movabs 0x9000006ec000006d,%al
     646ca519:	mov    $0x0,%ah
 	...
 
 00000000646ca51c <.pdata>:
-    646ca51c:	xor    %ch,0x0(%rsi)
-    646ca51f:	add    %al,%dh
-    646ca521:	outsb  %ds:(%rsi),(%dx)
+    646ca51c:	shrb   $0x0,0x0(%rsi)
+    646ca520:	push   %rsi
+    646ca521:	outsl  %ds:(%rsi),(%dx)
     646ca522:	add    %al,(%rax)
     646ca524:	pushf
     646ca525:	mov    $0x0,%ah
 	...
 
 00000000646ca528 <.pdata>:
-    646ca528:	shrb   0x0(%rsi)
-    646ca52b:	add    %ah,(%rdi)
-    646ca52d:	je     646ca52f <.pdata+0x7>
-    646ca52f:	add    %ah,0x74300000(%rsp,%rsi,4)
-    646ca536:	add    %al,(%rax)
-    646ca538:	scas   %es:(%rdi),%al
-    646ca539:	jbe    646ca53b <.pdata+0x13>
+    646ca528:	(bad)
+    646ca529:	outsl  %ds:(%rsi),(%dx)
+    646ca52a:	add    %al,(%rax)
+    646ca52c:	mov    $0x74,%bh
+    646ca52e:	add    %al,(%rax)
+    646ca530:	movsb  %ds:(%rsi),%es:(%rdi)
+    646ca531:	mov    $0x0,%ah
+    646ca533:	add    %al,%al
+    646ca535:	je     646ca537 <.pdata+0xf>
+    646ca537:	add    %bh,(%rsi)
+    646ca539:	ja     646ca53b <.pdata+0x13>
     646ca53b:	add    %al,%al
     646ca53d:	mov    $0x0,%ah
 	...
 
 00000000646ca540 <.pdata>:
-    646ca540:	xorb   $0x0,0x0(%rdi)
-    646ca544:	js,pt  646ca547 <.pdata+0x7>
+    646ca540:	adc    %bh,0x0(%rax)
+    646ca543:	add    %cl,%dh
+    646ca545:	js     646ca547 <.pdata+0x7>
     646ca547:	add    %cl,%ah
     646ca549:	mov    $0x0,%ah
 	...
 
 00000000646ca54c <.pdata>:
-    646ca54c:	(bad)
-    646ca54d:	jns    646ca54f <.pdata+0x3>
-    646ca54f:	add    %al,-0x2bffff87(%rbp)
+    646ca54c:	lock jns 646ca54f <.pdata+0x3>
+    646ca54f:	add    %dl,-0x2bffff86(%rip)        # 386ca5cf <__size_of_stack_reserve__+0x384ca5cf>
     646ca555:	mov    $0x0,%ah
 	...
 
 00000000646ca558 <.pdata>:
-    646ca558:	nop
-    646ca559:	jns    646ca55b <.pdata+0x3>
-    646ca55b:	add    %bl,0x7a(%rax)
-    646ca55e:	add    %al,(%rax)
-    646ca560:	fdivs  0x7a6000(%rax,%rax,1)
-    646ca567:	add    %cl,%bh
-    646ca569:	jp     646ca56b <.pdata+0x13>
-    646ca56b:	add    %ch,%al
-    646ca56d:	mov    $0x0,%ah
-    646ca56f:	add    %dl,%al
-    646ca571:	jp     646ca573 <.pdata+0x1b>
-    646ca573:	add    %ch,%bh
-    646ca575:	jp     646ca577 <.pdata+0x1f>
-    646ca577:	add    %dh,%ah
+    646ca558:	and    %bh,0x0(%rdx)
+    646ca55b:	add    %ch,%al
+    646ca55d:	jp     646ca55f <.pdata+0x7>
+    646ca55f:	add    %bl,%al
+    646ca561:	mov    $0x0,%ah
+    646ca563:	add    %dh,%al
+    646ca565:	jp     646ca567 <.pdata+0xf>
+    646ca567:	add    %bl,0x7b(%rdi)
+    646ca56a:	add    %al,(%rax)
+    646ca56c:	call   c46ca625 <.debug_str+0x5fff2625>
+    646ca571:	jnp    646ca573 <.pdata+0x1b>
+    646ca573:	add    %bh,0x7b(%rdi)
+    646ca576:	add    %al,(%rax)
+    646ca578:	hlt
     646ca579:	mov    $0x0,%ah
 	...
 
 00000000646ca57c <.pdata>:
-    646ca57c:	sarb   $0x0,0x0(%rbx)
-    646ca580:	add    %edi,0x0(%rax,%rax,1)
-    646ca584:	cld
+    646ca57c:	push   %rax
+    646ca57d:	jl     646ca57f <.pdata+0x3>
+    646ca57f:	add    %dl,-0x3ffff84(%rcx)
     646ca585:	mov    $0x0,%ah
 	...
 
 00000000646ca588 <.pdata>:
-    646ca588:	adc    %bh,0x0(%rax,%rax,1)
-    646ca58c:	sbb    $0x7c,%al
-    646ca58e:	add    %al,(%rax)
-    646ca590:	add    $0xb5,%al
-    646ca592:	add    %al,(%rax)
-    646ca594:	and    %bh,0x0(%rax,%rax,1)
-    646ca598:	sbb    $0x7d,%al
-    646ca59a:	add    %al,(%rax)
-    646ca59c:	or     %dh,0x7d300000(%rbp)
-    646ca5a2:	add    %al,(%rax)
-    646ca5a4:	cltd
-    646ca5a5:	jge    646ca5a7 <.pdata+0x1f>
-    646ca5a7:	add    %cl,-0x5fffff4d(%rax)
+    646ca588:	movabs 0x400007cac00007c,%al
+    646ca591:	mov    $0x0,%ch
+    646ca593:	add    %dh,-0x53ffff84(%rax)
+    646ca599:	jge    646ca59b <.pdata+0x13>
+    646ca59b:	add    %cl,(%rax)
+    646ca59d:	mov    $0x0,%ch
+    646ca59f:	add    %al,%al
+    646ca5a1:	jge    646ca5a3 <.pdata+0x1b>
+    646ca5a3:	add    %ch,(%rcx)
+    646ca5a5:	jle    646ca5a7 <.pdata+0x1f>
+    646ca5a7:	add    %cl,0x300000b3(%rax)
 
 00000000646ca5ac <.pdata.startup>:
-    646ca5ac:	movabs 0x2000007da500007d,%al
+    646ca5ac:	xor    %bh,0x0(%rsi)
+    646ca5af:	add    %dh,0x2000007e(%rip)        # 846ca633 <.debug_str+0x1fff2633>
     646ca5b5:	mov    $0x0,%ch
 	...
 
 Disassembly of section .xdata:
 
 00000000646cb000 <.xdata>:
     646cb000:	add    %eax,(%rax)
@@ -12513,19 +12542,19 @@
     646cb1e0:	or     %dl,0x50010304(%rdx)
 	...
 
 00000000646cb1e8 <.xdata>:
     646cb1e8:	add    %eax,(%rdx,%rax,1)
     646cb1eb:	add    $0x50010304,%eax
     646cb1f0:	add    %ecx,(%rax)
-    646cb1f2:	add    0x3045208(%rip),%eax        # 67710400 <.debug_str+0x3038400>
+    646cb1f2:	add    0x3047208(%rip),%eax        # 67712400 <.debug_str+0x303a400>
     646cb1f8:	add    %edx,0x0(%rax)
     646cb1fb:	add    %al,(%rcx)
     646cb1fd:	or     %al,(%rbx)
-    646cb1ff:	add    $0x3045208,%eax
+    646cb1ff:	add    $0x3047208,%eax
     646cb204:	add    %edx,0x0(%rax)
 	...
 
 00000000646cb208 <.xdata>:
     646cb208:	add    %ecx,(%rax)
     646cb20a:	add    0x3043208(%rip),%eax        # 6770e418 <.debug_str+0x3036418>
     646cb210:	add    %edx,0x0(%rax)
@@ -12535,29 +12564,26 @@
     646cb21c:	add    %ecx,(%rsi)
     646cb21e:	add    $0x85,%al
     646cb220:	(bad)
     646cb221:	add    (%rsi),%eax
     646cb223:	(bad)
     646cb225:	xor    %al,(%rcx)
     646cb227:	push   %rax
-    646cb228:	add    %ecx,0x4680c05(,%rax,1)
+    646cb228:	add    %ecx,0x3680c05(,%rax,1)
     646cb22f:	add    %cl,(%rax)
-    646cb231:	xchg   %eax,%edx
-    646cb232:	add    $0x3,%al
-    646cb234:	add    %edx,0x0(%rax)
-    646cb237:	add    %al,(%rcx)
-    646cb239:	(bad)
-    646cb23a:	add    $0x85,%al
-    646cb23c:	(bad)
-    646cb23d:	add    (%rsi),%eax
-    646cb23f:	(bad)
-    646cb241:	xor    %al,(%rcx)
-    646cb243:	push   %rax
-    646cb244:	add    %ecx,(%rax)
-    646cb246:	add    0x3045208(%rip),%eax        # 67710454 <.debug_str+0x3038454>
+    646cb231:	jb     646cb237 <.xdata+0x2f>
+    646cb233:	add    (%rcx),%eax
+    646cb235:	push   %rax
+    646cb236:	add    %al,(%rax)
+    646cb238:	add    %ecx,(%rax)
+    646cb23a:	add    0x3045208(%rip),%eax        # 67710448 <.debug_str+0x3038448>
+    646cb240:	add    %edx,0x0(%rax)
+    646cb243:	add    %al,(%rcx)
+    646cb245:	or     %al,(%rbx)
+    646cb247:	add    $0x3045208,%eax
     646cb24c:	add    %edx,0x0(%rax)
 	...
 
 00000000646cb250 <.xdata>:
     646cb250:	add    %ecx,(%rax)
     646cb252:	add    0x3045208(%rip),%eax        # 67710460 <.debug_str+0x3038460>
     646cb258:	add    %edx,0x0(%rax)
@@ -12908,18 +12934,18 @@
 
 00000000646cc000 <__bss_start__>:
 	...
 
 00000000646cc018 <__proc_attached>:
 	...
 
-00000000646cc020 <range>:
+00000000646cc020 <model>:
 	...
 
-00000000646cc028 <sill>:
+00000000646cc028 <k_range>:
 	...
 
 00000000646cc030 <estimation>:
 	...
 
 00000000646cc038 <krige_var>:
 	...
@@ -13058,30 +13084,34 @@
 	...
 
 Disassembly of section .edata:
 
 00000000646cd000 <.edata>:
     646cd000:	add    %al,(%rax)
     646cd002:	add    %al,(%rax)
-    646cd004:	pop    %rbp
-    646cd005:	imul   $0x0,(%rsp,%riz,2),%ebx
+    646cd004:	mov    $0x27,%dh
+    646cd006:	outsb  %ds:(%rsi),(%dx)
+    646cd007:	add    %al,%fs:(%rax)
+    646cd00a:	add    %al,(%rax)
     646cd00c:	mov    %dl,%dl
     646cd00e:	add    %al,(%rax)
     646cd010:	add    %eax,(%rax)
     646cd012:	add    %al,(%rax)
     646cd014:	cmp    $0x3d000000,%eax
     646cd019:	add    %al,(%rax)
     646cd01b:	add    %ch,(%rax)
     646cd01d:	rolb   (%rax)
     646cd01f:	add    %bl,(%rcx,%rdx,8)
     646cd022:	add    %al,(%rax)
     646cd024:	adc    %dl,%dl
     646cd026:	add    %al,(%rax)
-    646cd028:	and    %cl,0x0(%rsi)
-    646cd02b:	add    %cl,-0x1dffffbe(%rcx)
+    646cd028:	mov    $0x4e,%al
+    646cd02a:	add    %al,(%rax)
+    646cd02c:	sub    %eax,0x0(%rbx)
+    646cd02f:	add    %ah,%dl
     646cd031:	sbb    %al,(%rax)
     646cd033:	add    %al,(%rdi,%rdx,1)
     646cd036:	add    %al,(%rax)
     646cd038:	mov    $0x13,%al
     646cd03a:	add    %al,(%rax)
     646cd03c:	rex.XB adc $0x278e0000,%eax
     646cd042:	add    %al,(%rax)
@@ -13122,31 +13152,27 @@
     646cd08d:	and    (%rax),%al
     646cd08f:	add    %cl,%al
     646cd091:	sub    %eax,(%rax)
     646cd093:	add    %ch,0x29(%rsi)
     646cd096:	add    %al,(%rax)
     646cd098:	cs sub %eax,(%rax)
     646cd09b:	add    %cl,0x0(%rcx,%rbp,1)
-    646cd09f:	add    %al,(%rsi)
-    646cd0a1:	(bad)
+    646cd09f:	add    %ah,(%rdi,%rbp,1)
     646cd0a2:	add    %al,(%rax)
-    646cd0a4:	iret
-    646cd0a5:	(bad)
-    646cd0a6:	add    %al,(%rax)
-    646cd0a8:	shrb   $0x0,(%rsi)
-    646cd0ab:	add    %ah,%cl
-    646cd0ad:	rex.X add %al,(%rax)
-    646cd0b0:	cmp    $0xda000038,%eax
-    646cd0b5:	cmp    %eax,(%rax)
-    646cd0b7:	add    %bh,-0x7ffffcf(%rbp)
-    646cd0bd:	ds add %al,(%rax)
-    646cd0c0:	jp     646cd0fd <.edata+0xfd>
-    646cd0c2:	add    %al,(%rax)
-    646cd0c4:	lock rex.XB add %al,(%r8)
-    646cd0c8:	scas   %es:(%rdi),%al
+    646cd0a4:	cs xor %al,(%rax)
+    646cd0a7:	add    %al,%al
+    646cd0a9:	cs add %al,(%rax)
+    646cd0ac:	addl   $0x38c700,0x0(%rbx)
+    646cd0b3:	add    %bh,0x3a(%rbx)
+    646cd0b6:	add    %al,(%rax)
+    646cd0b8:	pop    %rbp
+    646cd0b9:	xor    (%rax),%al
+    646cd0bb:	add    %bl,0x1a00003f(%rax)
+    646cd0c1:	cmp    $0x0,%al
+    646cd0c3:	add    %dl,-0x51ffffbc(%rax)
     646cd0c9:	sub    (%rax),%al
     646cd0cb:	add    %bl,0x2d(%rsi)
     646cd0ce:	add    %al,(%rax)
     646cd0d0:	mov    $0x2d,%dl
     646cd0d2:	add    %al,(%rax)
     646cd0d4:	stos   %al,%es:(%rdi)
     646cd0d5:	sub    $0x0,%al
@@ -13154,39 +13180,37 @@
     646cd0d9:	sub    $0x0,%al
     646cd0db:	add    %ch,0x2c(%rbp)
     646cd0de:	add    %al,(%rax)
     646cd0e0:	xor    %ch,(%rdx)
     646cd0e2:	add    %al,(%rax)
     646cd0e4:	(bad)
     646cd0e5:	cs add %al,(%rax)
-    646cd0e8:	cmp    $0x21000043,%eax
-    646cd0ed:	push   %rax
-    646cd0ee:	add    %al,(%rax)
-    646cd0f0:	xor    %al,0x0(%rsi)
-    646cd0f3:	add    %ah,%al
-    646cd0f5:	xor    %al,(%rax)
-    646cd0f7:	add    %dl,0x7d000031(%rcx)
-    646cd0fd:	add    %r8b,(%rax)
-    646cd100:	loopne 646cd148 <.edata+0x148>
-    646cd102:	add    %al,(%rax)
-    646cd104:	rex.RB
-    646cd105:	rex.RXB add %r8b,(%r8)
-    646cd108:	or     %cl,0x0(%rax,%rax,1)
-    646cd10c:	adc    (%rax,%rax,1),%esi
-    646cd10f:	add    %dl,0xc00004c(%rax)
+    646cd0e8:	fldl   0x0(%rbx)
+    646cd0eb:	add    %dh,-0x2fffffb0(%rcx)
+    646cd0f1:	rex.RX add %r8b,(%rax)
+    646cd0f4:	xorb   $0x0,(%rcx)
+    646cd0f7:	add    %dh,(%rcx)
+    646cd0f9:	xor    (%rax),%al
+    646cd0fb:	add    %bl,-0x7fffffbb(%rip)        # ffffffffe46cd146 <.debug_str+0xffffffff7fff5146>
+    646cd101:	rex.RXB add %r8b,(%r8)
+    646cd104:	in     $0x47,%eax
+    646cd106:	add    %al,(%rax)
+    646cd108:	fwait
+    646cd109:	rex.WR add %r8b,(%rax)
+    646cd10c:	mov    $0x20000034,%ecx
+    646cd111:	rex.WRB add %r8b,(%r8)
+    646cd114:	pushf
     646cd115:	push   %rbx
     646cd116:	add    %al,(%rax)
-    646cd118:	nop
-    646cd119:	push   %rax
-    646cd11a:	add    %al,(%rax)
-    646cd11c:	xchg   %eax,%edi
-    646cd11d:	rolb   %cl,(%rax)
-    646cd11f:	add    %ah,-0x55ffff2e(%rbx)
-    646cd125:	rolb   %cl,(%rax)
-    646cd127:	add    %bh,-0x30ffff2e(%rbp)
+    646cd118:	and    %dl,0x0(%rcx)
+    646cd11b:	add    %dl,-0x5cffff2e(%rdi)
+    646cd121:	rolb   %cl,(%rax)
+    646cd123:	add    %ch,-0x42ffff2e(%rdx)
+    646cd129:	rolb   %cl,(%rax)
+    646cd12b:	add    %cl,%bh
     646cd12d:	rolb   %cl,(%rax)
     646cd12f:	add    %bl,%bh
     646cd131:	rolb   %cl,(%rax)
     646cd133:	add    %dh,%ch
     646cd135:	rolb   %cl,(%rax)
     646cd137:	add    %cl,(%rcx)
     646cd139:	roll   %cl,(%rax)
@@ -15114,22 +15138,23 @@
 00000000646cf020 <__xi_z>:
 	...
 
 00000000646cf028 <___crt_xi_end__>:
 	...
 
 00000000646cf030 <__xl_c>:
-    646cf030:	lock push %rsi
-    646cf032:	insb   (%dx),%es:(%rdi)
-    646cf033:	add    %al,%fs:(%rax)
+    646cf030:	adcb   $0x64,0x6c(%rdi)
+    646cf034:	add    %al,(%rax)
 	...
 
 00000000646cf038 <__xl_d>:
-    646cf038:	rclb   $0x64,0x6c(%rsi)
-    646cf03c:	add    %al,(%rax)
+    646cf038:	push   %rax
+    646cf039:	push   %rdi
+    646cf03a:	insb   (%dx),%es:(%rdi)
+    646cf03b:	add    %al,%fs:(%rax)
 	...
 
 00000000646cf040 <__xl_z>:
 	...
 
 00000000646cf048 <___crt_xp_end__>:
 	...
@@ -15147,17 +15172,17 @@
 
 Disassembly of section .reloc:
 
 00000000646d1000 <.reloc>:
     646d1000:	add    %dh,0x0(%rax)
     646d1003:	add    %cl,(%rax,%rax,1)
     646d1006:	add    %al,(%rax)
-    646d1008:	mov    $0xad,%eax
-    646d100d:	addb   $0x0,(%rax)
-    646d1010:	adc    $0x0,%al
+    646d1008:	rex.W scas %es:(%rdi),%al
+    646d100a:	add    %al,(%rax)
+    646d100c:	add    %al,0x140000(%rax)
     646d1012:	add    %al,(%rax)
     646d1014:	add    %ah,-0x5fa75fb0(%rax)
     646d101a:	(bad)
     646d101b:	movabs 0x90000000a070,%al
     646d1024:	xor    $0x0,%al
     646d1026:	add    %al,(%rax)
     646d1028:	andb   $0xc0,-0x5e5f5e78(%rcx)
@@ -15185,18 +15210,15 @@
     646d2002:	add    %al,(%rax)
     646d2004:	add    (%rax),%al
     646d2006:	add    %al,(%rax)
     646d2008:	add    %al,(%rax)
     646d200a:	or     %al,(%rax)
     646d200c:	add    %al,(%rax)
     646d200e:	add    %al,(%rax)
-    646d2010:	adc    %ah,0x6c(%rdi)
-    646d2013:	add    %al,%fs:(%rax)
-    646d2016:	add    %al,(%rax)
-    646d2018:	xor    (%rax),%al
+    646d2010:	movabs 0x3200000000646c67,%al
 	...
 
 00000000646d2030 <.debug_aranges>:
     646d2030:	sbb    $0x0,%al
     646d2032:	add    %al,(%rax)
     646d2034:	add    (%rax),%al
     646d2036:	cs add %al,(%rax)
@@ -15210,18 +15232,15 @@
     646d3002:	add    %al,(%rax)
     646d3004:	add    (%rax),%al
     646d3006:	add    %al,(%rax)
     646d3008:	add    %al,(%rax)
     646d300a:	or     %al,(%rcx)
     646d300c:	add    %al,(%rax)
     646d300e:	add    %al,(%rax)
-    646d3010:	adc    %ah,0x6c(%rdi)
-    646d3013:	add    %al,%fs:(%rax)
-    646d3016:	add    %al,(%rax)
-    646d3018:	rex.X
+    646d3010:	movabs 0xd200000000646c67,%al
     646d3019:	insb   (%dx),%es:(%edi)
     646d301b:	add    %al,%fs:(%rax)
     646d301e:	add    %al,(%rax)
     646d3020:	add    %al,(%rax)
     646d3022:	add    %al,(%rax)
     646d3024:	cmp    %eax,(%rax)
     646d3026:	add    %al,(%rax)
@@ -19338,23 +19357,23 @@
     646d4ed8:	pop    %rdi
     646d4ed9:	add    %cl,(%rax,%rsi,1)
     646d4edc:	adc    %edi,0x0(%rsi,%rbx,1)
     646d4ee0:	add    %bl,(%rax)
     646d4ee2:	xchg   %ebx,(%rsi)
     646d4ee4:	add    %al,(%rax)
     646d4ee6:	or     $0x90a0939,%eax
-    646d4eeb:	add    0x646c7d(%rax),%esi
-    646d4ef1:	add    %al,(%rax)
-    646d4ef3:	add    %bl,(%rax)
-    646d4ef5:	popf
-    646d4ef6:	(bad)
-    646d4ef7:	add    %al,(%rax)
-    646d4ef9:	or     $0x90a093a,%eax
-    646d4efe:	add    %eax,%ecx
-    646d4f00:	jge    646d4f6e <.debug_info+0x1f40>
+    646d4eeb:	add    0x7e(%rax),%eax
+    646d4eee:	insb   (%dx),%es:(%rdi)
+    646d4eef:	add    %al,%fs:(%rax)
+    646d4ef2:	add    %al,(%rax)
+    646d4ef4:	sbb    %bl,0xd00001e(%rbp)
+    646d4efa:	cmp    (%rcx),%cl
+    646d4efc:	or     (%rcx),%cl
+    646d4efe:	add    0x7e(%rax),%ebx
+    646d4f01:	insb   (%dx),%es:(%rdi)
     646d4f02:	add    %al,%fs:(%rax)
     646d4f05:	add    %al,(%rax)
 	...
 
 Disassembly of section .debug_abbrev:
 
 00000000646d5000 <.debug_abbrev>:
@@ -19528,18 +19547,16 @@
     646d604f:	ja     646d60ba <.debug_line+0x3f>
     646d6051:	outsb  %ds:(%rsi),(%dx)
     646d6052:	cs push %rbx
     646d6054:	add    %al,(%rcx)
     646d6056:	add    %al,(%rax)
     646d6058:	add    %al,(%rax)
     646d605a:	or     %eax,(%rdx)
-    646d605c:	adc    %ah,0x6c(%rdi)
-    646d605f:	add    %al,%fs:(%rax)
-    646d6062:	add    %al,(%rax)
-    646d6064:	add    %esp,%esi
+    646d605c:	movabs 0x300000000646c67,%al
+    646d6065:	hlt
     646d6066:	add    %al,(%rcx)
     646d6068:	and    (%rdx),%ah
     646d606a:	addr32 pop %rcx
     646d606c:	xor    %dh,0x4b(%rbp)
     646d606f:	addr32 xor %bh,0x222224c(%eip)        # 668f82c3 <.debug_str+0x22202c3>
     646d6077:	add    %eax,(%rax)
     646d6079:	add    %eax,(%rcx)
@@ -19700,22 +19717,19 @@
     646d700d:	or     $0x7,%al
     646d700f:	or     %ah,0x1(%rax)
     646d7015:	add    %al,(%rax)
     646d7017:	add    %ch,(%rax,%rax,1)
     646d701a:	add    %al,(%rax)
     646d701c:	add    %al,(%rax)
     646d701e:	add    %al,(%rax)
-    646d7020:	adc    %ah,0x6c(%rdi)
-    646d7023:	add    %al,%fs:(%rax)
-    646d7026:	add    %al,(%rax)
-    646d7028:	xor    (%rax),%al
-    646d702a:	add    %al,(%rax)
-    646d702c:	add    %al,(%rax)
-    646d702e:	add    %al,(%rax)
-    646d7030:	rex.B (bad)
+    646d7020:	movabs 0x3200000000646c67,%al
+    646d7029:	add    %al,(%rax)
+    646d702b:	add    %al,(%rax)
+    646d702d:	add    %al,(%rax)
+    646d702f:	add    %al,0xe(%rcx)
     646d7032:	adc    %al,0x180e4102(%rdx)
     646d7038:	addb   $0x6e,(%rbx)
     646d703b:	(bad)
     646d703c:	adc    %al,%al
     646d703e:	rex.B (bad)
     646d7040:	or     %al,%dl
     646d7042:	add    %al,(%rax)
```

### Comparing `uc_sgsim-1.2.0rc0/uc_sgsim/c_core/uc_sgsim.so` & `uc_sgsim-1.2.1/uc_sgsim/c_core/uc_sgsim.so`

 * *File has been modified after NT_GNU_BUILD_ID has been applied.*

 * *Files 13% similar despite different names*

#### readelf --wide --file-header {}

```diff
@@ -4,17 +4,17 @@
   Data:                              2's complement, little endian
   Version:                           1 (current)
   OS/ABI:                            UNIX - System V
   ABI Version:                       0
   Type:                              DYN (Shared object file)
   Machine:                           Advanced Micro Devices X86-64
   Version:                           0x1
-  Entry point address:               0x25c0
+  Entry point address:               0x1aa0
   Start of program headers:          64 (bytes into file)
-  Start of section headers:          39352 (bytes into file)
+  Start of section headers:          35232 (bytes into file)
   Flags:                             0x0
   Size of this header:               64 (bytes)
   Size of program headers:           56 (bytes)
-  Number of program headers:         11
+  Number of program headers:         7
   Size of section headers:           64 (bytes)
-  Number of section headers:         30
-  Section header string table index: 29
+  Number of section headers:         28
+  Section header string table index: 27
```

#### readelf --wide --program-header {}

```diff
@@ -1,32 +1,24 @@
 
 Elf file type is DYN (Shared object file)
-Entry point 0x25c0
-There are 11 program headers, starting at offset 64
+Entry point 0x1aa0
+There are 7 program headers, starting at offset 64
 
 Program Headers:
   Type           Offset   VirtAddr           PhysAddr           FileSiz  MemSiz   Flg Align
-  LOAD           0x000000 0x0000000000000000 0x0000000000000000 0x001778 0x001778 R   0x1000
-  LOAD           0x002000 0x0000000000002000 0x0000000000002000 0x004751 0x004751 R E 0x1000
-  LOAD           0x007000 0x0000000000007000 0x0000000000007000 0x000bf0 0x000bf0 R   0x1000
-  LOAD           0x007e00 0x0000000000008e00 0x0000000000008e00 0x000380 0x000670 RW  0x1000
-  DYNAMIC        0x007e10 0x0000000000008e10 0x0000000000008e10 0x0001d0 0x0001d0 RW  0x8
-  NOTE           0x0002a8 0x00000000000002a8 0x00000000000002a8 0x000020 0x000020 R   0x8
-  NOTE           0x0002c8 0x00000000000002c8 0x00000000000002c8 0x000024 0x000024 R   0x4
-  GNU_PROPERTY   0x0002a8 0x00000000000002a8 0x00000000000002a8 0x000020 0x000020 R   0x8
-  GNU_EH_FRAME   0x007190 0x0000000000007190 0x0000000000007190 0x000214 0x000214 R   0x4
+  LOAD           0x000000 0x0000000000000000 0x0000000000000000 0x006860 0x006860 R E 0x200000
+  LOAD           0x006e00 0x0000000000206e00 0x0000000000206e00 0x000380 0x000670 RW  0x200000
+  DYNAMIC        0x006e10 0x0000000000206e10 0x0000000000206e10 0x0001d0 0x0001d0 RW  0x8
+  NOTE           0x0001c8 0x00000000000001c8 0x00000000000001c8 0x000024 0x000024 R   0x4
+  GNU_EH_FRAME   0x005e20 0x0000000000005e20 0x0000000000005e20 0x00020c 0x00020c R   0x4
   GNU_STACK      0x000000 0x0000000000000000 0x0000000000000000 0x000000 0x000000 RW  0x10
-  GNU_RELRO      0x007e00 0x0000000000008e00 0x0000000000008e00 0x000200 0x000200 R   0x1
+  GNU_RELRO      0x006e00 0x0000000000206e00 0x0000000000206e00 0x000200 0x000200 R   0x1
 
  Section to Segment mapping:
   Segment Sections...
-   00     .note.gnu.property .note.gnu.build-id .gnu.hash .dynsym .dynstr .gnu.version .gnu.version_r .rela.dyn .rela.plt 
-   01     .init .plt .plt.got .plt.sec .text .fini 
-   02     .rodata .eh_frame_hdr .eh_frame 
-   03     .init_array .fini_array .dynamic .got .got.plt .data .bss 
-   04     .dynamic 
-   05     .note.gnu.property 
-   06     .note.gnu.build-id 
-   07     .note.gnu.property 
-   08     .eh_frame_hdr 
-   09     
-   10     .init_array .fini_array .dynamic .got 
+   00     .note.gnu.build-id .gnu.hash .dynsym .dynstr .gnu.version .gnu.version_r .rela.dyn .rela.plt .init .plt .plt.got .text .fini .rodata .eh_frame_hdr .eh_frame 
+   01     .init_array .fini_array .dynamic .got .got.plt .data .bss 
+   02     .dynamic 
+   03     .note.gnu.build-id 
+   04     .eh_frame_hdr 
+   05     
+   06     .init_array .fini_array .dynamic .got
```

#### readelf --wide --sections {}

```diff
@@ -1,39 +1,37 @@
-There are 30 section headers, starting at offset 0x99b8:
+There are 28 section headers, starting at offset 0x89a0:
 
 Section Headers:
   [Nr] Name              Type            Address          Off    Size   ES Flg Lk Inf Al
   [ 0]                   NULL            0000000000000000 000000 000000 00      0   0  0
-  [ 1] .note.gnu.property NOTE            00000000000002a8 0002a8 000020 00   A  0   0  8
-  [ 2] .note.gnu.build-id NOTE            00000000000002c8 0002c8 000024 00   A  0   0  4
-  [ 3] .gnu.hash         GNU_HASH        00000000000002f0 0002f0 0001dc 00   A  4   0  8
-  [ 4] .dynsym           DYNSYM          00000000000004d0 0004d0 000828 18   A  5   1  8
-  [ 5] .dynstr           STRTAB          0000000000000cf8 000cf8 0004d3 00   A  0   0  1
-  [ 6] .gnu.version      VERSYM          00000000000011cc 0011cc 0000ae 02   A  4   0  2
-  [ 7] .gnu.version_r    VERNEED         0000000000001280 001280 000030 00   A  5   1  8
-  [ 8] .rela.dyn         RELA            00000000000012b0 0012b0 0000a8 18   A  4   0  8
-  [ 9] .rela.plt         RELA            0000000000001358 001358 000420 18  AI  4  23  8
-  [10] .init             PROGBITS        0000000000002000 002000 00001b 00  AX  0   0  4
-  [11] .plt              PROGBITS        0000000000002020 002020 0002d0 10  AX  0   0 16
-  [12] .plt.got          PROGBITS        00000000000022f0 0022f0 000010 10  AX  0   0 16
-  [13] .plt.sec          PROGBITS        0000000000002300 002300 0002c0 10  AX  0   0 16
-  [14] .text             PROGBITS        00000000000025c0 0025c0 004184 00  AX  0   0 16
-  [15] .fini             PROGBITS        0000000000006744 006744 00000d 00  AX  0   0  4
-  [16] .rodata           PROGBITS        0000000000007000 007000 000190 00   A  0   0 16
-  [17] .eh_frame_hdr     PROGBITS        0000000000007190 007190 000214 00   A  0   0  4
-  [18] .eh_frame         PROGBITS        00000000000073a8 0073a8 000848 00   A  0   0  8
-  [19] .init_array       INIT_ARRAY      0000000000008e00 007e00 000008 08  WA  0   0  8
-  [20] .fini_array       FINI_ARRAY      0000000000008e08 007e08 000008 08  WA  0   0  8
-  [21] .dynamic          DYNAMIC         0000000000008e10 007e10 0001d0 10  WA  5   0  8
-  [22] .got              PROGBITS        0000000000008fe0 007fe0 000020 08  WA  0   0  8
-  [23] .got.plt          PROGBITS        0000000000009000 008000 000178 08  WA  0   0  8
-  [24] .data             PROGBITS        0000000000009178 008178 000008 00  WA  0   0  8
-  [25] .bss              NOBITS          0000000000009180 008180 0002f0 00  WA  0   0 32
-  [26] .comment          PROGBITS        0000000000000000 008180 00002b 01  MS  0   0  1
-  [27] .symtab           SYMTAB          0000000000000000 0081b0 000f60 18     28  78  8
-  [28] .strtab           STRTAB          0000000000000000 009110 00079b 00      0   0  1
-  [29] .shstrtab         STRTAB          0000000000000000 0098ab 00010d 00      0   0  1
+  [ 1] .note.gnu.build-id NOTE            00000000000001c8 0001c8 000024 00   A  0   0  4
+  [ 2] .gnu.hash         GNU_HASH        00000000000001f0 0001f0 000268 00   A  3   0  8
+  [ 3] .dynsym           DYNSYM          0000000000000458 000458 0008a0 18   A  4   1  8
+  [ 4] .dynstr           STRTAB          0000000000000cf8 000cf8 0004f1 00   A  0   0  1
+  [ 5] .gnu.version      VERSYM          00000000000011ea 0011ea 0000b8 02   A  3   0  2
+  [ 6] .gnu.version_r    VERNEED         00000000000012a8 0012a8 000030 00   A  4   1  8
+  [ 7] .rela.dyn         RELA            00000000000012d8 0012d8 0000a8 18   A  3   0  8
+  [ 8] .rela.plt         RELA            0000000000001380 001380 000420 18  AI  3  21  8
+  [ 9] .init             PROGBITS        00000000000017a0 0017a0 000017 00  AX  0   0  4
+  [10] .plt              PROGBITS        00000000000017c0 0017c0 0002d0 10  AX  0   0 16
+  [11] .plt.got          PROGBITS        0000000000001a90 001a90 000008 08  AX  0   0  8
+  [12] .text             PROGBITS        0000000000001aa0 001aa0 0041d9 00  AX  0   0 16
+  [13] .fini             PROGBITS        0000000000005c7c 005c7c 000009 00  AX  0   0  4
+  [14] .rodata           PROGBITS        0000000000005c90 005c90 000190 00   A  0   0 16
+  [15] .eh_frame_hdr     PROGBITS        0000000000005e20 005e20 00020c 00   A  0   0  4
+  [16] .eh_frame         PROGBITS        0000000000006030 006030 000830 00   A  0   0  8
+  [17] .init_array       INIT_ARRAY      0000000000206e00 006e00 000008 08  WA  0   0  8
+  [18] .fini_array       FINI_ARRAY      0000000000206e08 006e08 000008 08  WA  0   0  8
+  [19] .dynamic          DYNAMIC         0000000000206e10 006e10 0001d0 10  WA  4   0  8
+  [20] .got              PROGBITS        0000000000206fe0 006fe0 000020 08  WA  0   0  8
+  [21] .got.plt          PROGBITS        0000000000207000 007000 000178 08  WA  0   0  8
+  [22] .data             PROGBITS        0000000000207178 007178 000008 00  WA  0   0  8
+  [23] .bss              NOBITS          0000000000207180 007180 0002f0 00  WA  0   0 32
+  [24] .comment          PROGBITS        0000000000000000 007180 000029 01  MS  0   0  1
+  [25] .symtab           SYMTAB          0000000000000000 0071b0 000f60 18     26  73  8
+  [26] .strtab           STRTAB          0000000000000000 008110 00079f 00      0   0  1
+  [27] .shstrtab         STRTAB          0000000000000000 0088af 0000f1 00      0   0  1
 Key to Flags:
   W (write), A (alloc), X (execute), M (merge), S (strings), I (info),
   L (link order), O (extra OS processing required), G (group), T (TLS),
   C (compressed), x (unknown), o (OS specific), E (exclude),
   D (mbind), l (large), p (processor specific)
```

#### readelf --wide --symbols {}

```diff
@@ -1,9 +1,9 @@
 
-Symbol table '.dynsym' contains 87 entries:
+Symbol table '.dynsym' contains 92 entries:
    Num:    Value          Size Type    Bind   Vis      Ndx Name
      0: 0000000000000000     0 NOTYPE  LOCAL  DEFAULT  UND 
      1: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND free@GLIBC_2.2.5 (2)
      2: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __errno_location@GLIBC_2.2.5 (2)
      3: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND _ITM_deregisterTMCloneTable
      4: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND mkdir@GLIBC_2.2.5 (2)
      5: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND ceil
@@ -22,236 +22,241 @@
     18: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND pow
     19: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND perror@GLIBC_2.2.5 (2)
     20: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND log10
     21: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND sqrt
     22: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND exit@GLIBC_2.2.5 (2)
     23: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND _ITM_registerTMCloneTable
     24: 0000000000000000     0 FUNC    WEAK   DEFAULT  UND __cxa_finalize@GLIBC_2.2.5 (2)
-    25: 00000000000051a2   926 FUNC    GLOBAL DEFAULT   14 lu_decomposition
-    26: 000000000000366c   126 FUNC    GLOBAL DEFAULT   14 c_array_var_double
-    27: 0000000000003f52    75 FUNC    GLOBAL DEFAULT   14 mt19937_get_double
-    28: 00000000000056a4   140 FUNC    GLOBAL DEFAULT   14 matrixform
-    29: 0000000000003bf6   125 FUNC    GLOBAL DEFAULT   14 mt19937_init
-    30: 0000000000004612  1060 FUNC    GLOBAL DEFAULT   14 simple_kriging
-    31: 0000000000006323   102 FUNC    GLOBAL DEFAULT   14 quicksort2d
-    32: 0000000000002679   399 FUNC    GLOBAL DEFAULT   14 c_array_max_int
-    33: 0000000000002b9f   479 FUNC    GLOBAL DEFAULT   14 c_array_max_double
-    34: 0000000000002f25   470 FUNC    GLOBAL DEFAULT   14 c_array_min_long_long
-    35: 0000000000002808   445 FUNC    GLOBAL DEFAULT   14 c_array_max_long_long
-    36: 000000000000438a    47 FUNC    GLOBAL DEFAULT   14 sampling_state_update
-    37: 0000000000006389   737 FUNC    GLOBAL DEFAULT   14 variogram
-    38: 0000000000003f9d   108 FUNC    GLOBAL DEFAULT   14 mt19937_get_double_range
-    39: 0000000000003900    44 FUNC    GLOBAL DEFAULT   14 c_array_mean_int
-    40: 00000000000040ec   209 FUNC    GLOBAL DEFAULT   14 cov_model
-    41: 0000000000004a36   415 FUNC    GLOBAL DEFAULT   14 find_neighbor
-    42: 000000000000392c    46 FUNC    GLOBAL DEFAULT   14 c_array_mean_long_long
-    43: 0000000000003e5a    66 FUNC    GLOBAL DEFAULT   14 mt19937_get_int32_range
-    44: 0000000000006123   512 FUNC    GLOBAL DEFAULT   14 Partition2d
-    45: 0000000000005730   454 FUNC    GLOBAL DEFAULT   14 save_1darray
-    46: 000000000000408e    94 FUNC    GLOBAL DEFAULT   14 cov_model_init
-    47: 00000000000035ea   130 FUNC    GLOBAL DEFAULT   14 c_array_var_float
-    48: 00000000000037f6   135 FUNC    GLOBAL DEFAULT   14 c_array_std_float
-    49: 00000000000039ff    77 FUNC    GLOBAL DEFAULT   14 c_array_sum_long
-    50: 0000000000003a4c    90 FUNC    GLOBAL DEFAULT   14 c_array_sum_float
-    51: 00000000000039b6    73 FUNC    GLOBAL DEFAULT   14 c_array_sum_int
-    52: 0000000000002d7e   423 FUNC    GLOBAL DEFAULT   14 c_array_min_int
-    53: 000000000000376f   135 FUNC    GLOBAL DEFAULT   14 c_array_std_long_long
-    54: 0000000000003988    46 FUNC    GLOBAL DEFAULT   14 c_array_mean_double
-    55: 00000000000034e8   128 FUNC    GLOBAL DEFAULT   14 c_array_var_int
-    56: 000000000000387d   131 FUNC    GLOBAL DEFAULT   14 c_array_std_double
-    57: 000000000000666a   218 FUNC    GLOBAL DEFAULT   14 variance
-    58: 0000000000003ee7   107 FUNC    GLOBAL DEFAULT   14 mt19937_get_float_range
-    59: 00000000000032ef   505 FUNC    GLOBAL DEFAULT   14 c_array_min_double
-    60: 00000000000059ae   113 FUNC    GLOBAL DEFAULT   14 sgsim_init
-    61: 0000000000003aa6    90 FUNC    GLOBAL DEFAULT   14 c_array_sum_double
-    62: 0000000000003b9e    88 FUNC    GLOBAL DEFAULT   14 cmpfunc_double
-    63: 00000000000029c5   474 FUNC    GLOBAL DEFAULT   14 c_array_max_float
-    64: 0000000000003b48    86 FUNC    GLOBAL DEFAULT   14 cmpfunc_float
-    65: 00000000000041bd   280 FUNC    GLOBAL DEFAULT   14 cov_model2d
-    66: 00000000000058f6   184 FUNC    GLOBAL DEFAULT   14 randompath
-    67: 0000000000005f96   397 FUNC    GLOBAL DEFAULT   14 swap
-    68: 00000000000092e0   144 OBJECT  GLOBAL DEFAULT   25 st
-    69: 00000000000043b9   601 FUNC    GLOBAL DEFAULT   14 krige_param_setting
-    70: 00000000000030fb   500 FUNC    GLOBAL DEFAULT   14 c_array_min_float
-    71: 0000000000003b00    34 FUNC    GLOBAL DEFAULT   14 cmpfunc_int
-    72: 0000000000003568   130 FUNC    GLOBAL DEFAULT   14 c_array_var_long_long
-    73: 0000000000005540    88 FUNC    GLOBAL DEFAULT   14 arange
-    74: 0000000000005f1d    35 FUNC    GLOBAL DEFAULT   14 sgsim_t_free
-    75: 0000000000003b22    38 FUNC    GLOBAL DEFAULT   14 cmpfunc_long
-    76: 000000000000395a    46 FUNC    GLOBAL DEFAULT   14 c_array_mean_float
-    77: 0000000000004bd5   336 FUNC    GLOBAL DEFAULT   14 krige_memory_free
-    78: 0000000000005a1f  1278 FUNC    GLOBAL DEFAULT   14 sgsim_run
-    79: 00000000000036ea   133 FUNC    GLOBAL DEFAULT   14 c_array_std_int
-    80: 0000000000004009   133 FUNC    GLOBAL DEFAULT   14 mt19937_random_normal
-    81: 0000000000003e9c    75 FUNC    GLOBAL DEFAULT   14 mt19937_get_float
-    82: 0000000000005598    92 FUNC    GLOBAL DEFAULT   14 d_arange
-    83: 0000000000004d25  1149 FUNC    GLOBAL DEFAULT   14 lu_inverse_solver
-    84: 0000000000003c73   487 FUNC    GLOBAL DEFAULT   14 mt19937_generate
-    85: 00000000000042d5   181 FUNC    GLOBAL DEFAULT   14 sampling_state_init
-    86: 00000000000055f4   176 FUNC    GLOBAL DEFAULT   14 pdist
+    25: 0000000000003451    71 FUNC    GLOBAL DEFAULT   12 mt19937_get_double
+    26: 0000000000004af2    88 FUNC    GLOBAL DEFAULT   12 d_arange
+    27: 0000000000002eb5    46 FUNC    GLOBAL DEFAULT   12 c_array_mean_double
+    28: 0000000000002a4d   134 FUNC    GLOBAL DEFAULT   12 c_array_var_long_long
+    29: 0000000000002f28    73 FUNC    GLOBAL DEFAULT   12 c_array_sum_long
+    30: 0000000000002bdb   151 FUNC    GLOBAL DEFAULT   12 c_array_std_int
+    31: 0000000000004f02   109 FUNC    GLOBAL DEFAULT   12 sgsim_init
+    32: 00000000000058b6   737 FUNC    GLOBAL DEFAULT   12 variogram
+    33: 0000000000002fc7    86 FUNC    GLOBAL DEFAULT   12 c_array_sum_double
+    34: 0000000000002b59   130 FUNC    GLOBAL DEFAULT   12 c_array_var_double
+    35: 0000000000003f7d   435 FUNC    GLOBAL DEFAULT   12 find_neighbor
+    36: 0000000000002c72   153 FUNC    GLOBAL DEFAULT   12 c_array_std_long_long
+    37: 000000000000303b    34 FUNC    GLOBAL DEFAULT   12 cmpfunc_long
+    38: 0000000000002ee3    69 FUNC    GLOBAL DEFAULT   12 c_array_sum_int
+    39: 0000000000005658   508 FUNC    GLOBAL DEFAULT   12 Partition2d
+    40: 000000000000335f    68 FUNC    GLOBAL DEFAULT   12 mt19937_get_int32_range
+    41: 0000000000002d0b   153 FUNC    GLOBAL DEFAULT   12 c_array_std_float
+    42: 0000000000005c7c     0 FUNC    GLOBAL DEFAULT   13 _fini
+    43: 0000000000003589   109 FUNC    GLOBAL DEFAULT   12 cov_model_init
+    44: 000000000000317c   483 FUNC    GLOBAL DEFAULT   12 mt19937_generate
+    45: 0000000000004a9e    84 FUNC    GLOBAL DEFAULT   12 arange
+    46: 000000000000427c  1153 FUNC    GLOBAL DEFAULT   12 lu_inverse_solver
+    47: 0000000000002da4   149 FUNC    GLOBAL DEFAULT   12 c_array_std_double
+    48: 00000000000017a0     0 FUNC    GLOBAL DEFAULT    9 _init
+    49: 0000000000003847   177 FUNC    GLOBAL DEFAULT   12 sampling_state_init
+    50: 00000000000029c9   132 FUNC    GLOBAL DEFAULT   12 c_array_var_int
+    51: 0000000000002412   466 FUNC    GLOBAL DEFAULT   12 c_array_min_long_long
+    52: 000000000000545e    31 FUNC    GLOBAL DEFAULT   12 sgsim_t_free
+    53: 000000000000305d    82 FUNC    GLOBAL DEFAULT   12 cmpfunc_float
+    54: 0000000000002094   475 FUNC    GLOBAL DEFAULT   12 c_array_max_double
+    55: 0000000000004e48   186 FUNC    GLOBAL DEFAULT   12 randompath
+    56: 0000000000005854    98 FUNC    GLOBAL DEFAULT   12 quicksort2d
+    57: 0000000000004b4a   171 FUNC    GLOBAL DEFAULT   12 pdist
+    58: 0000000000001d05   441 FUNC    GLOBAL DEFAULT   12 c_array_max_long_long
+    59: 00000000000046fd   929 FUNC    GLOBAL DEFAULT   12 lu_decomposition
+    60: 0000000000004f6f  1263 FUNC    GLOBAL DEFAULT   12 sgsim_run
+    61: 0000000000003103   121 FUNC    GLOBAL DEFAULT   12 mt19937_init
+    62: 00000000000027d4   501 FUNC    GLOBAL DEFAULT   12 c_array_min_double
+    63: 0000000000005b97   226 FUNC    GLOBAL DEFAULT   12 variance
+    64: 0000000000004bf5   135 FUNC    GLOBAL DEFAULT   12 matrixform
+    65: 00000000000054cf   393 FUNC    GLOBAL DEFAULT   12 swap
+    66: 0000000000002f71    86 FUNC    GLOBAL DEFAULT   12 c_array_sum_float
+    67: 00000000000030af    84 FUNC    GLOBAL DEFAULT   12 cmpfunc_double
+    68: 0000000000002ad3   134 FUNC    GLOBAL DEFAULT   12 c_array_var_float
+    69: 00000000002072e0   144 OBJECT  GLOBAL DEFAULT   23 st
+    70: 0000000000003498   104 FUNC    GLOBAL DEFAULT   12 mt19937_get_double_range
+    71: 0000000000002e39    40 FUNC    GLOBAL DEFAULT   12 c_array_mean_int
+    72: 000000000000301d    30 FUNC    GLOBAL DEFAULT   12 cmpfunc_int
+    73: 0000000000207180     0 NOTYPE  GLOBAL DEFAULT   22 _edata
+    74: 00000000000038f8    43 FUNC    GLOBAL DEFAULT   12 sampling_state_update
+    75: 0000000000003b7d  1024 FUNC    GLOBAL DEFAULT   12 simple_kriging
+    76: 0000000000004130   332 FUNC    GLOBAL DEFAULT   12 krige_memory_free
+    77: 0000000000002e8b    42 FUNC    GLOBAL DEFAULT   12 c_array_mean_float
+    78: 00000000000033a3    71 FUNC    GLOBAL DEFAULT   12 mt19937_get_float
+    79: 0000000000001b7a   395 FUNC    GLOBAL DEFAULT   12 c_array_max_int
+    80: 0000000000207470     0 NOTYPE  GLOBAL DEFAULT   23 _end
+    81: 00000000000033ea   103 FUNC    GLOBAL DEFAULT   12 mt19937_get_float_range
+    82: 0000000000002e61    42 FUNC    GLOBAL DEFAULT   12 c_array_mean_long_long
+    83: 00000000000025e4   496 FUNC    GLOBAL DEFAULT   12 c_array_min_float
+    84: 0000000000003500   137 FUNC    GLOBAL DEFAULT   12 mt19937_random_normal
+    85: 0000000000001ebe   470 FUNC    GLOBAL DEFAULT   12 c_array_max_float
+    86: 0000000000004c7c   460 FUNC    GLOBAL DEFAULT   12 save_1darray
+    87: 00000000000036fb   332 FUNC    GLOBAL DEFAULT   12 cov_model2d
+    88: 000000000000226f   419 FUNC    GLOBAL DEFAULT   12 c_array_min_int
+    89: 0000000000003923   602 FUNC    GLOBAL DEFAULT   12 krige_param_setting
+    90: 0000000000207180     0 NOTYPE  GLOBAL DEFAULT   23 __bss_start
+    91: 00000000000035f6   261 FUNC    GLOBAL DEFAULT   12 cov_model
 
 Symbol table '.symtab' contains 164 entries:
    Num:    Value          Size Type    Bind   Vis      Ndx Name
      0: 0000000000000000     0 NOTYPE  LOCAL  DEFAULT  UND 
-     1: 00000000000002a8     0 SECTION LOCAL  DEFAULT    1 .note.gnu.property
-     2: 00000000000002c8     0 SECTION LOCAL  DEFAULT    2 .note.gnu.build-id
-     3: 00000000000002f0     0 SECTION LOCAL  DEFAULT    3 .gnu.hash
-     4: 00000000000004d0     0 SECTION LOCAL  DEFAULT    4 .dynsym
-     5: 0000000000000cf8     0 SECTION LOCAL  DEFAULT    5 .dynstr
-     6: 00000000000011cc     0 SECTION LOCAL  DEFAULT    6 .gnu.version
-     7: 0000000000001280     0 SECTION LOCAL  DEFAULT    7 .gnu.version_r
-     8: 00000000000012b0     0 SECTION LOCAL  DEFAULT    8 .rela.dyn
-     9: 0000000000001358     0 SECTION LOCAL  DEFAULT    9 .rela.plt
-    10: 0000000000002000     0 SECTION LOCAL  DEFAULT   10 .init
-    11: 0000000000002020     0 SECTION LOCAL  DEFAULT   11 .plt
-    12: 00000000000022f0     0 SECTION LOCAL  DEFAULT   12 .plt.got
-    13: 0000000000002300     0 SECTION LOCAL  DEFAULT   13 .plt.sec
-    14: 00000000000025c0     0 SECTION LOCAL  DEFAULT   14 .text
-    15: 0000000000006744     0 SECTION LOCAL  DEFAULT   15 .fini
-    16: 0000000000007000     0 SECTION LOCAL  DEFAULT   16 .rodata
-    17: 0000000000007190     0 SECTION LOCAL  DEFAULT   17 .eh_frame_hdr
-    18: 00000000000073a8     0 SECTION LOCAL  DEFAULT   18 .eh_frame
-    19: 0000000000008e00     0 SECTION LOCAL  DEFAULT   19 .init_array
-    20: 0000000000008e08     0 SECTION LOCAL  DEFAULT   20 .fini_array
-    21: 0000000000008e10     0 SECTION LOCAL  DEFAULT   21 .dynamic
-    22: 0000000000008fe0     0 SECTION LOCAL  DEFAULT   22 .got
-    23: 0000000000009000     0 SECTION LOCAL  DEFAULT   23 .got.plt
-    24: 0000000000009178     0 SECTION LOCAL  DEFAULT   24 .data
-    25: 0000000000009180     0 SECTION LOCAL  DEFAULT   25 .bss
-    26: 0000000000000000     0 SECTION LOCAL  DEFAULT   26 .comment
-    27: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS crtstuff.c
-    28: 00000000000025c0     0 FUNC    LOCAL  DEFAULT   14 deregister_tm_clones
-    29: 00000000000025f0     0 FUNC    LOCAL  DEFAULT   14 register_tm_clones
-    30: 0000000000002630     0 FUNC    LOCAL  DEFAULT   14 __do_global_dtors_aux
-    31: 0000000000009180     1 OBJECT  LOCAL  DEFAULT   25 completed.8061
-    32: 0000000000008e08     0 OBJECT  LOCAL  DEFAULT   20 __do_global_dtors_aux_fini_array_entry
-    33: 0000000000002670     0 FUNC    LOCAL  DEFAULT   14 frame_dummy
-    34: 0000000000008e00     0 OBJECT  LOCAL  DEFAULT   19 __frame_dummy_init_array_entry
-    35: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS c_array.c
-    36: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS c_array_mt.c
-    37: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS cov_model.c
-    38: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS krige.c
-    39: 0000000000009190     8 OBJECT  LOCAL  DEFAULT   25 range
-    40: 0000000000009198     8 OBJECT  LOCAL  DEFAULT   25 sill
-    41: 00000000000091a0     8 OBJECT  LOCAL  DEFAULT   25 estimation
-    42: 00000000000091a8     8 OBJECT  LOCAL  DEFAULT   25 krige_var
-    43: 00000000000091b0     8 OBJECT  LOCAL  DEFAULT   25 fix
-    44: 00000000000091c0    24 OBJECT  LOCAL  DEFAULT   25 location
-    45: 00000000000091e0    24 OBJECT  LOCAL  DEFAULT   25 loc_cov
-    46: 0000000000009200    24 OBJECT  LOCAL  DEFAULT   25 data_temp
-    47: 0000000000009220    24 OBJECT  LOCAL  DEFAULT   25 loc_cov2
-    48: 0000000000009240    24 OBJECT  LOCAL  DEFAULT   25 flatten_temp
-    49: 0000000000009260    24 OBJECT  LOCAL  DEFAULT   25 weights
-    50: 0000000000009280    24 OBJECT  LOCAL  DEFAULT   25 array2d_temp
-    51: 00000000000092a0    24 OBJECT  LOCAL  DEFAULT   25 pdist_temp
-    52: 00000000000092c0    24 OBJECT  LOCAL  DEFAULT   25 datacov
-    53: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS matrix_tools.c
-    54: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS random_tools.c
-    55: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS sgsim.c
-    56: 0000000000009380    24 OBJECT  LOCAL  DEFAULT   25 x_grid
-    57: 00000000000093a0    24 OBJECT  LOCAL  DEFAULT   25 u_array
-    58: 00000000000093c0    24 OBJECT  LOCAL  DEFAULT   25 sampled
-    59: 00000000000093e0    24 OBJECT  LOCAL  DEFAULT   25 variogram_array
-    60: 0000000000009400    24 OBJECT  LOCAL  DEFAULT   25 sgsim_array
-    61: 0000000000009420    72 OBJECT  LOCAL  DEFAULT   25 _sampling
-    62: 0000000000009468     4 OBJECT  LOCAL  DEFAULT   25 flag
-    63: 000000000000946c     4 OBJECT  LOCAL  DEFAULT   25 count
-    64: 0000000000005f40    86 FUNC    LOCAL  DEFAULT   14 sgsim_memory_free
-    65: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS sort_tools.c
-    66: 0000000000006323   102 FUNC    LOCAL  DEFAULT   14 quicksort2d.localalias
-    67: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS variogram.c
-    68: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS crtstuff.c
-    69: 0000000000007bec     0 OBJECT  LOCAL  DEFAULT   18 __FRAME_END__
-    70: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS 
-    71: 0000000000006744     0 FUNC    LOCAL  DEFAULT   15 _fini
-    72: 0000000000009178     0 OBJECT  LOCAL  DEFAULT   24 __dso_handle
-    73: 0000000000008e10     0 OBJECT  LOCAL  DEFAULT   21 _DYNAMIC
-    74: 0000000000007190     0 NOTYPE  LOCAL  DEFAULT   17 __GNU_EH_FRAME_HDR
-    75: 0000000000009180     0 OBJECT  LOCAL  DEFAULT   24 __TMC_END__
-    76: 0000000000009000     0 OBJECT  LOCAL  DEFAULT   23 _GLOBAL_OFFSET_TABLE_
-    77: 0000000000002000     0 FUNC    LOCAL  DEFAULT   10 _init
-    78: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND free@@GLIBC_2.2.5
-    79: 00000000000029c5   474 FUNC    GLOBAL DEFAULT   14 c_array_max_float
-    80: 00000000000034e8   128 FUNC    GLOBAL DEFAULT   14 c_array_var_int
-    81: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __errno_location@@GLIBC_2.2.5
-    82: 0000000000003a4c    90 FUNC    GLOBAL DEFAULT   14 c_array_sum_float
-    83: 0000000000003b00    34 FUNC    GLOBAL DEFAULT   14 cmpfunc_int
-    84: 0000000000006323   102 FUNC    GLOBAL DEFAULT   14 quicksort2d
-    85: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND _ITM_deregisterTMCloneTable
-    86: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND mkdir@@GLIBC_2.2.5
-    87: 00000000000039b6    73 FUNC    GLOBAL DEFAULT   14 c_array_sum_int
-    88: 00000000000058f6   184 FUNC    GLOBAL DEFAULT   14 randompath
-    89: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND ceil
-    90: 0000000000004d25  1149 FUNC    GLOBAL DEFAULT   14 lu_inverse_solver
-    91: 000000000000438a    47 FUNC    GLOBAL DEFAULT   14 sampling_state_update
-    92: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND fclose@@GLIBC_2.2.5
-    93: 0000000000005a1f  1278 FUNC    GLOBAL DEFAULT   14 sgsim_run
-    94: 00000000000092e0   144 OBJECT  GLOBAL DEFAULT   25 st
-    95: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __stack_chk_fail@@GLIBC_2.4
-    96: 0000000000005730   454 FUNC    GLOBAL DEFAULT   14 save_1darray
-    97: 000000000000366c   126 FUNC    GLOBAL DEFAULT   14 c_array_var_double
-    98: 0000000000003900    44 FUNC    GLOBAL DEFAULT   14 c_array_mean_int
-    99: 00000000000030fb   500 FUNC    GLOBAL DEFAULT   14 c_array_min_float
-   100: 00000000000041bd   280 FUNC    GLOBAL DEFAULT   14 cov_model2d
-   101: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND printf@@GLIBC_2.2.5
-   102: 0000000000004a36   415 FUNC    GLOBAL DEFAULT   14 find_neighbor
-   103: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND snprintf@@GLIBC_2.2.5
-   104: 0000000000003b9e    88 FUNC    GLOBAL DEFAULT   14 cmpfunc_double
-   105: 00000000000051a2   926 FUNC    GLOBAL DEFAULT   14 lu_decomposition
-   106: 0000000000005598    92 FUNC    GLOBAL DEFAULT   14 d_arange
-   107: 0000000000006123   512 FUNC    GLOBAL DEFAULT   14 Partition2d
-   108: 0000000000003ee7   107 FUNC    GLOBAL DEFAULT   14 mt19937_get_float_range
-   109: 00000000000040ec   209 FUNC    GLOBAL DEFAULT   14 cov_model
-   110: 00000000000056a4   140 FUNC    GLOBAL DEFAULT   14 matrixform
-   111: 0000000000003c73   487 FUNC    GLOBAL DEFAULT   14 mt19937_generate
-   112: 000000000000392c    46 FUNC    GLOBAL DEFAULT   14 c_array_mean_long_long
-   113: 000000000000666a   218 FUNC    GLOBAL DEFAULT   14 variance
-   114: 0000000000003568   130 FUNC    GLOBAL DEFAULT   14 c_array_var_long_long
-   115: 00000000000036ea   133 FUNC    GLOBAL DEFAULT   14 c_array_std_int
-   116: 0000000000004009   133 FUNC    GLOBAL DEFAULT   14 mt19937_random_normal
-   117: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND calloc@@GLIBC_2.2.5
-   118: 00000000000032ef   505 FUNC    GLOBAL DEFAULT   14 c_array_min_double
-   119: 000000000000408e    94 FUNC    GLOBAL DEFAULT   14 cov_model_init
-   120: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND fprintf@@GLIBC_2.2.5
-   121: 0000000000005f1d    35 FUNC    GLOBAL DEFAULT   14 sgsim_t_free
-   122: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND __gmon_start__
-   123: 0000000000002d7e   423 FUNC    GLOBAL DEFAULT   14 c_array_min_int
-   124: 000000000000387d   131 FUNC    GLOBAL DEFAULT   14 c_array_std_double
-   125: 0000000000002679   399 FUNC    GLOBAL DEFAULT   14 c_array_max_int
-   126: 00000000000043b9   601 FUNC    GLOBAL DEFAULT   14 krige_param_setting
-   127: 00000000000039ff    77 FUNC    GLOBAL DEFAULT   14 c_array_sum_long
-   128: 0000000000003bf6   125 FUNC    GLOBAL DEFAULT   14 mt19937_init
-   129: 0000000000003b48    86 FUNC    GLOBAL DEFAULT   14 cmpfunc_float
-   130: 0000000000004612  1060 FUNC    GLOBAL DEFAULT   14 simple_kriging
-   131: 000000000000395a    46 FUNC    GLOBAL DEFAULT   14 c_array_mean_float
-   132: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND malloc@@GLIBC_2.2.5
-   133: 0000000000005540    88 FUNC    GLOBAL DEFAULT   14 arange
-   134: 0000000000004bd5   336 FUNC    GLOBAL DEFAULT   14 krige_memory_free
-   135: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND exp
-   136: 00000000000035ea   130 FUNC    GLOBAL DEFAULT   14 c_array_var_float
-   137: 0000000000006389   737 FUNC    GLOBAL DEFAULT   14 variogram
-   138: 0000000000002b9f   479 FUNC    GLOBAL DEFAULT   14 c_array_max_double
-   139: 0000000000002f25   470 FUNC    GLOBAL DEFAULT   14 c_array_min_long_long
-   140: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND cos
-   141: 0000000000003e5a    66 FUNC    GLOBAL DEFAULT   14 mt19937_get_int32_range
-   142: 00000000000042d5   181 FUNC    GLOBAL DEFAULT   14 sampling_state_init
-   143: 0000000000003f9d   108 FUNC    GLOBAL DEFAULT   14 mt19937_get_double_range
-   144: 00000000000059ae   113 FUNC    GLOBAL DEFAULT   14 sgsim_init
-   145: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND log
-   146: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND fopen@@GLIBC_2.2.5
-   147: 0000000000003f52    75 FUNC    GLOBAL DEFAULT   14 mt19937_get_double
-   148: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND pow
-   149: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND perror@@GLIBC_2.2.5
-   150: 0000000000003e9c    75 FUNC    GLOBAL DEFAULT   14 mt19937_get_float
-   151: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND log10
-   152: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND sqrt
-   153: 0000000000003b22    38 FUNC    GLOBAL DEFAULT   14 cmpfunc_long
-   154: 00000000000055f4   176 FUNC    GLOBAL DEFAULT   14 pdist
-   155: 000000000000376f   135 FUNC    GLOBAL DEFAULT   14 c_array_std_long_long
-   156: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND exit@@GLIBC_2.2.5
-   157: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND _ITM_registerTMCloneTable
-   158: 0000000000005f96   397 FUNC    GLOBAL DEFAULT   14 swap
-   159: 0000000000003988    46 FUNC    GLOBAL DEFAULT   14 c_array_mean_double
-   160: 00000000000037f6   135 FUNC    GLOBAL DEFAULT   14 c_array_std_float
-   161: 0000000000002808   445 FUNC    GLOBAL DEFAULT   14 c_array_max_long_long
-   162: 0000000000003aa6    90 FUNC    GLOBAL DEFAULT   14 c_array_sum_double
-   163: 0000000000000000     0 FUNC    WEAK   DEFAULT  UND __cxa_finalize@@GLIBC_2.2.5
+     1: 00000000000001c8     0 SECTION LOCAL  DEFAULT    1 .note.gnu.build-id
+     2: 00000000000001f0     0 SECTION LOCAL  DEFAULT    2 .gnu.hash
+     3: 0000000000000458     0 SECTION LOCAL  DEFAULT    3 .dynsym
+     4: 0000000000000cf8     0 SECTION LOCAL  DEFAULT    4 .dynstr
+     5: 00000000000011ea     0 SECTION LOCAL  DEFAULT    5 .gnu.version
+     6: 00000000000012a8     0 SECTION LOCAL  DEFAULT    6 .gnu.version_r
+     7: 00000000000012d8     0 SECTION LOCAL  DEFAULT    7 .rela.dyn
+     8: 0000000000001380     0 SECTION LOCAL  DEFAULT    8 .rela.plt
+     9: 00000000000017a0     0 SECTION LOCAL  DEFAULT    9 .init
+    10: 00000000000017c0     0 SECTION LOCAL  DEFAULT   10 .plt
+    11: 0000000000001a90     0 SECTION LOCAL  DEFAULT   11 .plt.got
+    12: 0000000000001aa0     0 SECTION LOCAL  DEFAULT   12 .text
+    13: 0000000000005c7c     0 SECTION LOCAL  DEFAULT   13 .fini
+    14: 0000000000005c90     0 SECTION LOCAL  DEFAULT   14 .rodata
+    15: 0000000000005e20     0 SECTION LOCAL  DEFAULT   15 .eh_frame_hdr
+    16: 0000000000006030     0 SECTION LOCAL  DEFAULT   16 .eh_frame
+    17: 0000000000206e00     0 SECTION LOCAL  DEFAULT   17 .init_array
+    18: 0000000000206e08     0 SECTION LOCAL  DEFAULT   18 .fini_array
+    19: 0000000000206e10     0 SECTION LOCAL  DEFAULT   19 .dynamic
+    20: 0000000000206fe0     0 SECTION LOCAL  DEFAULT   20 .got
+    21: 0000000000207000     0 SECTION LOCAL  DEFAULT   21 .got.plt
+    22: 0000000000207178     0 SECTION LOCAL  DEFAULT   22 .data
+    23: 0000000000207180     0 SECTION LOCAL  DEFAULT   23 .bss
+    24: 0000000000000000     0 SECTION LOCAL  DEFAULT   24 .comment
+    25: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS crtstuff.c
+    26: 0000000000001aa0     0 FUNC    LOCAL  DEFAULT   12 deregister_tm_clones
+    27: 0000000000001ae0     0 FUNC    LOCAL  DEFAULT   12 register_tm_clones
+    28: 0000000000001b30     0 FUNC    LOCAL  DEFAULT   12 __do_global_dtors_aux
+    29: 0000000000207180     1 OBJECT  LOCAL  DEFAULT   23 completed.7698
+    30: 0000000000206e08     0 OBJECT  LOCAL  DEFAULT   18 __do_global_dtors_aux_fini_array_entry
+    31: 0000000000001b70     0 FUNC    LOCAL  DEFAULT   12 frame_dummy
+    32: 0000000000206e00     0 OBJECT  LOCAL  DEFAULT   17 __frame_dummy_init_array_entry
+    33: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS c_array.c
+    34: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS c_array_mt.c
+    35: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS cov_model.c
+    36: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS krige.c
+    37: 0000000000207190     8 OBJECT  LOCAL  DEFAULT   23 model
+    38: 0000000000207198     8 OBJECT  LOCAL  DEFAULT   23 k_range
+    39: 00000000002071a0     8 OBJECT  LOCAL  DEFAULT   23 estimation
+    40: 00000000002071a8     8 OBJECT  LOCAL  DEFAULT   23 krige_var
+    41: 00000000002071b0     8 OBJECT  LOCAL  DEFAULT   23 fix
+    42: 00000000002071c0    24 OBJECT  LOCAL  DEFAULT   23 location
+    43: 00000000002071e0    24 OBJECT  LOCAL  DEFAULT   23 loc_cov
+    44: 0000000000207200    24 OBJECT  LOCAL  DEFAULT   23 data_temp
+    45: 0000000000207220    24 OBJECT  LOCAL  DEFAULT   23 loc_cov2
+    46: 0000000000207240    24 OBJECT  LOCAL  DEFAULT   23 flatten_temp
+    47: 0000000000207260    24 OBJECT  LOCAL  DEFAULT   23 weights
+    48: 0000000000207280    24 OBJECT  LOCAL  DEFAULT   23 array2d_temp
+    49: 00000000002072a0    24 OBJECT  LOCAL  DEFAULT   23 pdist_temp
+    50: 00000000002072c0    24 OBJECT  LOCAL  DEFAULT   23 datacov
+    51: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS matrix_tools.c
+    52: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS random_tools.c
+    53: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS sgsim.c
+    54: 0000000000207380    24 OBJECT  LOCAL  DEFAULT   23 x_grid
+    55: 00000000002073a0    24 OBJECT  LOCAL  DEFAULT   23 u_array
+    56: 00000000002073c0    24 OBJECT  LOCAL  DEFAULT   23 sampled
+    57: 00000000002073e0    24 OBJECT  LOCAL  DEFAULT   23 variogram_array
+    58: 0000000000207400    24 OBJECT  LOCAL  DEFAULT   23 sgsim_array
+    59: 0000000000207420    72 OBJECT  LOCAL  DEFAULT   23 _sampling
+    60: 0000000000207468     4 OBJECT  LOCAL  DEFAULT   23 flag
+    61: 000000000020746c     4 OBJECT  LOCAL  DEFAULT   23 count
+    62: 000000000000547d    82 FUNC    LOCAL  DEFAULT   12 sgsim_memory_free
+    63: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS sort_tools.c
+    64: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS variogram.c
+    65: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS crtstuff.c
+    66: 000000000000685c     0 OBJECT  LOCAL  DEFAULT   16 __FRAME_END__
+    67: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS 
+    68: 0000000000207178     0 OBJECT  LOCAL  DEFAULT   22 __dso_handle
+    69: 0000000000206e10     0 OBJECT  LOCAL  DEFAULT   19 _DYNAMIC
+    70: 0000000000005e20     0 NOTYPE  LOCAL  DEFAULT   15 __GNU_EH_FRAME_HDR
+    71: 0000000000207180     0 OBJECT  LOCAL  DEFAULT   22 __TMC_END__
+    72: 0000000000207000     0 OBJECT  LOCAL  DEFAULT   21 _GLOBAL_OFFSET_TABLE_
+    73: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND free@@GLIBC_2.2.5
+    74: 0000000000001ebe   470 FUNC    GLOBAL DEFAULT   12 c_array_max_float
+    75: 00000000000029c9   132 FUNC    GLOBAL DEFAULT   12 c_array_var_int
+    76: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __errno_location@@GLIBC_2.2.5
+    77: 0000000000002f71    86 FUNC    GLOBAL DEFAULT   12 c_array_sum_float
+    78: 000000000000301d    30 FUNC    GLOBAL DEFAULT   12 cmpfunc_int
+    79: 0000000000005854    98 FUNC    GLOBAL DEFAULT   12 quicksort2d
+    80: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND _ITM_deregisterTMCloneTable
+    81: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND mkdir@@GLIBC_2.2.5
+    82: 0000000000002ee3    69 FUNC    GLOBAL DEFAULT   12 c_array_sum_int
+    83: 0000000000004e48   186 FUNC    GLOBAL DEFAULT   12 randompath
+    84: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND ceil
+    85: 0000000000207180     0 NOTYPE  GLOBAL DEFAULT   22 _edata
+    86: 000000000000427c  1153 FUNC    GLOBAL DEFAULT   12 lu_inverse_solver
+    87: 00000000000038f8    43 FUNC    GLOBAL DEFAULT   12 sampling_state_update
+    88: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND fclose@@GLIBC_2.2.5
+    89: 0000000000004f6f  1263 FUNC    GLOBAL DEFAULT   12 sgsim_run
+    90: 0000000000005c7c     0 FUNC    GLOBAL DEFAULT   13 _fini
+    91: 00000000002072e0   144 OBJECT  GLOBAL DEFAULT   23 st
+    92: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __stack_chk_fail@@GLIBC_2.4
+    93: 0000000000004c7c   460 FUNC    GLOBAL DEFAULT   12 save_1darray
+    94: 0000000000002b59   130 FUNC    GLOBAL DEFAULT   12 c_array_var_double
+    95: 0000000000002e39    40 FUNC    GLOBAL DEFAULT   12 c_array_mean_int
+    96: 00000000000025e4   496 FUNC    GLOBAL DEFAULT   12 c_array_min_float
+    97: 00000000000036fb   332 FUNC    GLOBAL DEFAULT   12 cov_model2d
+    98: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND printf@@GLIBC_2.2.5
+    99: 0000000000003f7d   435 FUNC    GLOBAL DEFAULT   12 find_neighbor
+   100: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND snprintf@@GLIBC_2.2.5
+   101: 00000000000030af    84 FUNC    GLOBAL DEFAULT   12 cmpfunc_double
+   102: 00000000000046fd   929 FUNC    GLOBAL DEFAULT   12 lu_decomposition
+   103: 0000000000004af2    88 FUNC    GLOBAL DEFAULT   12 d_arange
+   104: 0000000000005658   508 FUNC    GLOBAL DEFAULT   12 Partition2d
+   105: 00000000000033ea   103 FUNC    GLOBAL DEFAULT   12 mt19937_get_float_range
+   106: 00000000000035f6   261 FUNC    GLOBAL DEFAULT   12 cov_model
+   107: 0000000000004bf5   135 FUNC    GLOBAL DEFAULT   12 matrixform
+   108: 000000000000317c   483 FUNC    GLOBAL DEFAULT   12 mt19937_generate
+   109: 0000000000002e61    42 FUNC    GLOBAL DEFAULT   12 c_array_mean_long_long
+   110: 0000000000005b97   226 FUNC    GLOBAL DEFAULT   12 variance
+   111: 0000000000002a4d   134 FUNC    GLOBAL DEFAULT   12 c_array_var_long_long
+   112: 0000000000002bdb   151 FUNC    GLOBAL DEFAULT   12 c_array_std_int
+   113: 0000000000003500   137 FUNC    GLOBAL DEFAULT   12 mt19937_random_normal
+   114: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND calloc@@GLIBC_2.2.5
+   115: 00000000000027d4   501 FUNC    GLOBAL DEFAULT   12 c_array_min_double
+   116: 0000000000003589   109 FUNC    GLOBAL DEFAULT   12 cov_model_init
+   117: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND fprintf@@GLIBC_2.2.5
+   118: 000000000000545e    31 FUNC    GLOBAL DEFAULT   12 sgsim_t_free
+   119: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND __gmon_start__
+   120: 000000000000226f   419 FUNC    GLOBAL DEFAULT   12 c_array_min_int
+   121: 0000000000002da4   149 FUNC    GLOBAL DEFAULT   12 c_array_std_double
+   122: 0000000000001b7a   395 FUNC    GLOBAL DEFAULT   12 c_array_max_int
+   123: 0000000000003923   602 FUNC    GLOBAL DEFAULT   12 krige_param_setting
+   124: 0000000000002f28    73 FUNC    GLOBAL DEFAULT   12 c_array_sum_long
+   125: 0000000000003103   121 FUNC    GLOBAL DEFAULT   12 mt19937_init
+   126: 000000000000305d    82 FUNC    GLOBAL DEFAULT   12 cmpfunc_float
+   127: 0000000000003b7d  1024 FUNC    GLOBAL DEFAULT   12 simple_kriging
+   128: 0000000000002e8b    42 FUNC    GLOBAL DEFAULT   12 c_array_mean_float
+   129: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND malloc@@GLIBC_2.2.5
+   130: 0000000000004a9e    84 FUNC    GLOBAL DEFAULT   12 arange
+   131: 0000000000004130   332 FUNC    GLOBAL DEFAULT   12 krige_memory_free
+   132: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND exp
+   133: 0000000000207470     0 NOTYPE  GLOBAL DEFAULT   23 _end
+   134: 0000000000002ad3   134 FUNC    GLOBAL DEFAULT   12 c_array_var_float
+   135: 0000000000207180     0 NOTYPE  GLOBAL DEFAULT   23 __bss_start
+   136: 00000000000058b6   737 FUNC    GLOBAL DEFAULT   12 variogram
+   137: 0000000000002094   475 FUNC    GLOBAL DEFAULT   12 c_array_max_double
+   138: 0000000000002412   466 FUNC    GLOBAL DEFAULT   12 c_array_min_long_long
+   139: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND cos
+   140: 000000000000335f    68 FUNC    GLOBAL DEFAULT   12 mt19937_get_int32_range
+   141: 0000000000003847   177 FUNC    GLOBAL DEFAULT   12 sampling_state_init
+   142: 0000000000003498   104 FUNC    GLOBAL DEFAULT   12 mt19937_get_double_range
+   143: 0000000000004f02   109 FUNC    GLOBAL DEFAULT   12 sgsim_init
+   144: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND log
+   145: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND fopen@@GLIBC_2.2.5
+   146: 0000000000003451    71 FUNC    GLOBAL DEFAULT   12 mt19937_get_double
+   147: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND pow
+   148: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND perror@@GLIBC_2.2.5
+   149: 00000000000033a3    71 FUNC    GLOBAL DEFAULT   12 mt19937_get_float
+   150: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND log10
+   151: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND sqrt
+   152: 000000000000303b    34 FUNC    GLOBAL DEFAULT   12 cmpfunc_long
+   153: 0000000000004b4a   171 FUNC    GLOBAL DEFAULT   12 pdist
+   154: 0000000000002c72   153 FUNC    GLOBAL DEFAULT   12 c_array_std_long_long
+   155: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND exit@@GLIBC_2.2.5
+   156: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND _ITM_registerTMCloneTable
+   157: 00000000000054cf   393 FUNC    GLOBAL DEFAULT   12 swap
+   158: 0000000000002eb5    46 FUNC    GLOBAL DEFAULT   12 c_array_mean_double
+   159: 0000000000002d0b   153 FUNC    GLOBAL DEFAULT   12 c_array_std_float
+   160: 0000000000001d05   441 FUNC    GLOBAL DEFAULT   12 c_array_max_long_long
+   161: 0000000000002fc7    86 FUNC    GLOBAL DEFAULT   12 c_array_sum_double
+   162: 0000000000000000     0 FUNC    WEAK   DEFAULT  UND __cxa_finalize@@GLIBC_2.2.5
+   163: 00000000000017a0     0 FUNC    GLOBAL DEFAULT    9 _init
```

#### readelf --wide --relocs {}

```diff
@@ -1,57 +1,57 @@
 
-Relocation section '.rela.dyn' at offset 0x12b0 contains 7 entries:
+Relocation section '.rela.dyn' at offset 0x12d8 contains 7 entries:
     Offset             Info             Type               Symbol's Value  Symbol's Name + Addend
-0000000000008e00  0000000000000008 R_X86_64_RELATIVE                         2670
-0000000000008e08  0000000000000008 R_X86_64_RELATIVE                         2630
-0000000000009178  0000000000000008 R_X86_64_RELATIVE                         9178
-0000000000008fe0  0000000300000006 R_X86_64_GLOB_DAT      0000000000000000 _ITM_deregisterTMCloneTable + 0
-0000000000008fe8  0000000c00000006 R_X86_64_GLOB_DAT      0000000000000000 __gmon_start__ + 0
-0000000000008ff0  0000001700000006 R_X86_64_GLOB_DAT      0000000000000000 _ITM_registerTMCloneTable + 0
-0000000000008ff8  0000001800000006 R_X86_64_GLOB_DAT      0000000000000000 __cxa_finalize@GLIBC_2.2.5 + 0
+0000000000206e00  0000000000000008 R_X86_64_RELATIVE                         1b70
+0000000000206e08  0000000000000008 R_X86_64_RELATIVE                         1b30
+0000000000207178  0000000000000008 R_X86_64_RELATIVE                         207178
+0000000000206fe0  0000000300000006 R_X86_64_GLOB_DAT      0000000000000000 _ITM_deregisterTMCloneTable + 0
+0000000000206fe8  0000000c00000006 R_X86_64_GLOB_DAT      0000000000000000 __gmon_start__ + 0
+0000000000206ff0  0000001700000006 R_X86_64_GLOB_DAT      0000000000000000 _ITM_registerTMCloneTable + 0
+0000000000206ff8  0000001800000006 R_X86_64_GLOB_DAT      0000000000000000 __cxa_finalize@GLIBC_2.2.5 + 0
 
-Relocation section '.rela.plt' at offset 0x1358 contains 44 entries:
+Relocation section '.rela.plt' at offset 0x1380 contains 44 entries:
     Offset             Info             Type               Symbol's Value  Symbol's Name + Addend
-0000000000009018  0000000100000007 R_X86_64_JUMP_SLOT     0000000000000000 free@GLIBC_2.2.5 + 0
-0000000000009020  0000000200000007 R_X86_64_JUMP_SLOT     0000000000000000 __errno_location@GLIBC_2.2.5 + 0
-0000000000009028  0000001f00000007 R_X86_64_JUMP_SLOT     0000000000006323 quicksort2d + 0
-0000000000009030  0000000400000007 R_X86_64_JUMP_SLOT     0000000000000000 mkdir@GLIBC_2.2.5 + 0
-0000000000009038  0000004200000007 R_X86_64_JUMP_SLOT     00000000000058f6 randompath + 0
-0000000000009040  0000000500000007 R_X86_64_JUMP_SLOT     0000000000000000 ceil + 0
-0000000000009048  0000005300000007 R_X86_64_JUMP_SLOT     0000000000004d25 lu_inverse_solver + 0
-0000000000009050  0000002400000007 R_X86_64_JUMP_SLOT     000000000000438a sampling_state_update + 0
-0000000000009058  0000000600000007 R_X86_64_JUMP_SLOT     0000000000000000 fclose@GLIBC_2.2.5 + 0
-0000000000009060  0000000700000007 R_X86_64_JUMP_SLOT     0000000000000000 __stack_chk_fail@GLIBC_2.4 + 0
-0000000000009068  0000002d00000007 R_X86_64_JUMP_SLOT     0000000000005730 save_1darray + 0
-0000000000009070  0000004100000007 R_X86_64_JUMP_SLOT     00000000000041bd cov_model2d + 0
-0000000000009078  0000000800000007 R_X86_64_JUMP_SLOT     0000000000000000 printf@GLIBC_2.2.5 + 0
-0000000000009080  0000002900000007 R_X86_64_JUMP_SLOT     0000000000004a36 find_neighbor + 0
-0000000000009088  0000000900000007 R_X86_64_JUMP_SLOT     0000000000000000 snprintf@GLIBC_2.2.5 + 0
-0000000000009090  0000001900000007 R_X86_64_JUMP_SLOT     00000000000051a2 lu_decomposition + 0
-0000000000009098  0000005200000007 R_X86_64_JUMP_SLOT     0000000000005598 d_arange + 0
-00000000000090a0  0000002c00000007 R_X86_64_JUMP_SLOT     0000000000006123 Partition2d + 0
-00000000000090a8  0000002800000007 R_X86_64_JUMP_SLOT     00000000000040ec cov_model + 0
-00000000000090b0  0000001c00000007 R_X86_64_JUMP_SLOT     00000000000056a4 matrixform + 0
-00000000000090b8  0000005400000007 R_X86_64_JUMP_SLOT     0000000000003c73 mt19937_generate + 0
-00000000000090c0  0000005000000007 R_X86_64_JUMP_SLOT     0000000000004009 mt19937_random_normal + 0
-00000000000090c8  0000000a00000007 R_X86_64_JUMP_SLOT     0000000000000000 calloc@GLIBC_2.2.5 + 0
-00000000000090d0  0000000b00000007 R_X86_64_JUMP_SLOT     0000000000000000 fprintf@GLIBC_2.2.5 + 0
-00000000000090d8  0000004500000007 R_X86_64_JUMP_SLOT     00000000000043b9 krige_param_setting + 0
-00000000000090e0  0000001d00000007 R_X86_64_JUMP_SLOT     0000000000003bf6 mt19937_init + 0
-00000000000090e8  0000001e00000007 R_X86_64_JUMP_SLOT     0000000000004612 simple_kriging + 0
-00000000000090f0  0000000d00000007 R_X86_64_JUMP_SLOT     0000000000000000 malloc@GLIBC_2.2.5 + 0
-00000000000090f8  0000004900000007 R_X86_64_JUMP_SLOT     0000000000005540 arange + 0
-0000000000009100  0000004d00000007 R_X86_64_JUMP_SLOT     0000000000004bd5 krige_memory_free + 0
-0000000000009108  0000000e00000007 R_X86_64_JUMP_SLOT     0000000000000000 exp + 0
-0000000000009110  0000002500000007 R_X86_64_JUMP_SLOT     0000000000006389 variogram + 0
-0000000000009118  0000000f00000007 R_X86_64_JUMP_SLOT     0000000000000000 cos + 0
-0000000000009120  0000005500000007 R_X86_64_JUMP_SLOT     00000000000042d5 sampling_state_init + 0
-0000000000009128  0000001000000007 R_X86_64_JUMP_SLOT     0000000000000000 log + 0
-0000000000009130  0000001100000007 R_X86_64_JUMP_SLOT     0000000000000000 fopen@GLIBC_2.2.5 + 0
-0000000000009138  0000001b00000007 R_X86_64_JUMP_SLOT     0000000000003f52 mt19937_get_double + 0
-0000000000009140  0000001200000007 R_X86_64_JUMP_SLOT     0000000000000000 pow + 0
-0000000000009148  0000001300000007 R_X86_64_JUMP_SLOT     0000000000000000 perror@GLIBC_2.2.5 + 0
-0000000000009150  0000001400000007 R_X86_64_JUMP_SLOT     0000000000000000 log10 + 0
-0000000000009158  0000001500000007 R_X86_64_JUMP_SLOT     0000000000000000 sqrt + 0
-0000000000009160  0000005600000007 R_X86_64_JUMP_SLOT     00000000000055f4 pdist + 0
-0000000000009168  0000001600000007 R_X86_64_JUMP_SLOT     0000000000000000 exit@GLIBC_2.2.5 + 0
-0000000000009170  0000004300000007 R_X86_64_JUMP_SLOT     0000000000005f96 swap + 0
+0000000000207018  0000000100000007 R_X86_64_JUMP_SLOT     0000000000000000 free@GLIBC_2.2.5 + 0
+0000000000207020  0000000200000007 R_X86_64_JUMP_SLOT     0000000000000000 __errno_location@GLIBC_2.2.5 + 0
+0000000000207028  0000003800000007 R_X86_64_JUMP_SLOT     0000000000005854 quicksort2d + 0
+0000000000207030  0000000400000007 R_X86_64_JUMP_SLOT     0000000000000000 mkdir@GLIBC_2.2.5 + 0
+0000000000207038  0000003700000007 R_X86_64_JUMP_SLOT     0000000000004e48 randompath + 0
+0000000000207040  0000000500000007 R_X86_64_JUMP_SLOT     0000000000000000 ceil + 0
+0000000000207048  0000002e00000007 R_X86_64_JUMP_SLOT     000000000000427c lu_inverse_solver + 0
+0000000000207050  0000004a00000007 R_X86_64_JUMP_SLOT     00000000000038f8 sampling_state_update + 0
+0000000000207058  0000000600000007 R_X86_64_JUMP_SLOT     0000000000000000 fclose@GLIBC_2.2.5 + 0
+0000000000207060  0000000700000007 R_X86_64_JUMP_SLOT     0000000000000000 __stack_chk_fail@GLIBC_2.4 + 0
+0000000000207068  0000005600000007 R_X86_64_JUMP_SLOT     0000000000004c7c save_1darray + 0
+0000000000207070  0000005700000007 R_X86_64_JUMP_SLOT     00000000000036fb cov_model2d + 0
+0000000000207078  0000000800000007 R_X86_64_JUMP_SLOT     0000000000000000 printf@GLIBC_2.2.5 + 0
+0000000000207080  0000002300000007 R_X86_64_JUMP_SLOT     0000000000003f7d find_neighbor + 0
+0000000000207088  0000000900000007 R_X86_64_JUMP_SLOT     0000000000000000 snprintf@GLIBC_2.2.5 + 0
+0000000000207090  0000003b00000007 R_X86_64_JUMP_SLOT     00000000000046fd lu_decomposition + 0
+0000000000207098  0000001a00000007 R_X86_64_JUMP_SLOT     0000000000004af2 d_arange + 0
+00000000002070a0  0000002700000007 R_X86_64_JUMP_SLOT     0000000000005658 Partition2d + 0
+00000000002070a8  0000005b00000007 R_X86_64_JUMP_SLOT     00000000000035f6 cov_model + 0
+00000000002070b0  0000004000000007 R_X86_64_JUMP_SLOT     0000000000004bf5 matrixform + 0
+00000000002070b8  0000002c00000007 R_X86_64_JUMP_SLOT     000000000000317c mt19937_generate + 0
+00000000002070c0  0000005400000007 R_X86_64_JUMP_SLOT     0000000000003500 mt19937_random_normal + 0
+00000000002070c8  0000000a00000007 R_X86_64_JUMP_SLOT     0000000000000000 calloc@GLIBC_2.2.5 + 0
+00000000002070d0  0000000b00000007 R_X86_64_JUMP_SLOT     0000000000000000 fprintf@GLIBC_2.2.5 + 0
+00000000002070d8  0000005900000007 R_X86_64_JUMP_SLOT     0000000000003923 krige_param_setting + 0
+00000000002070e0  0000003d00000007 R_X86_64_JUMP_SLOT     0000000000003103 mt19937_init + 0
+00000000002070e8  0000004b00000007 R_X86_64_JUMP_SLOT     0000000000003b7d simple_kriging + 0
+00000000002070f0  0000000d00000007 R_X86_64_JUMP_SLOT     0000000000000000 malloc@GLIBC_2.2.5 + 0
+00000000002070f8  0000002d00000007 R_X86_64_JUMP_SLOT     0000000000004a9e arange + 0
+0000000000207100  0000004c00000007 R_X86_64_JUMP_SLOT     0000000000004130 krige_memory_free + 0
+0000000000207108  0000000e00000007 R_X86_64_JUMP_SLOT     0000000000000000 exp + 0
+0000000000207110  0000002000000007 R_X86_64_JUMP_SLOT     00000000000058b6 variogram + 0
+0000000000207118  0000000f00000007 R_X86_64_JUMP_SLOT     0000000000000000 cos + 0
+0000000000207120  0000003100000007 R_X86_64_JUMP_SLOT     0000000000003847 sampling_state_init + 0
+0000000000207128  0000001000000007 R_X86_64_JUMP_SLOT     0000000000000000 log + 0
+0000000000207130  0000001100000007 R_X86_64_JUMP_SLOT     0000000000000000 fopen@GLIBC_2.2.5 + 0
+0000000000207138  0000001900000007 R_X86_64_JUMP_SLOT     0000000000003451 mt19937_get_double + 0
+0000000000207140  0000001200000007 R_X86_64_JUMP_SLOT     0000000000000000 pow + 0
+0000000000207148  0000001300000007 R_X86_64_JUMP_SLOT     0000000000000000 perror@GLIBC_2.2.5 + 0
+0000000000207150  0000001400000007 R_X86_64_JUMP_SLOT     0000000000000000 log10 + 0
+0000000000207158  0000001500000007 R_X86_64_JUMP_SLOT     0000000000000000 sqrt + 0
+0000000000207160  0000003900000007 R_X86_64_JUMP_SLOT     0000000000004b4a pdist + 0
+0000000000207168  0000001600000007 R_X86_64_JUMP_SLOT     0000000000000000 exit@GLIBC_2.2.5 + 0
+0000000000207170  0000004100000007 R_X86_64_JUMP_SLOT     00000000000054cf swap + 0
```

#### readelf --wide --dynamic {}

```diff
@@ -1,28 +1,28 @@
 
-Dynamic section at offset 0x7e10 contains 25 entries:
+Dynamic section at offset 0x6e10 contains 25 entries:
   Tag        Type                         Name/Value
  0x0000000000000001 (NEEDED)             Shared library: [libc.so.6]
  0x000000000000000e (SONAME)             Library soname: [uc_sgsim.so]
- 0x000000000000000c (INIT)               0x2000
- 0x000000000000000d (FINI)               0x6744
- 0x0000000000000019 (INIT_ARRAY)         0x8e00
+ 0x000000000000000c (INIT)               0x17a0
+ 0x000000000000000d (FINI)               0x5c7c
+ 0x0000000000000019 (INIT_ARRAY)         0x206e00
  0x000000000000001b (INIT_ARRAYSZ)       8 (bytes)
- 0x000000000000001a (FINI_ARRAY)         0x8e08
+ 0x000000000000001a (FINI_ARRAY)         0x206e08
  0x000000000000001c (FINI_ARRAYSZ)       8 (bytes)
- 0x000000006ffffef5 (GNU_HASH)           0x2f0
+ 0x000000006ffffef5 (GNU_HASH)           0x1f0
  0x0000000000000005 (STRTAB)             0xcf8
- 0x0000000000000006 (SYMTAB)             0x4d0
- 0x000000000000000a (STRSZ)              1235 (bytes)
+ 0x0000000000000006 (SYMTAB)             0x458
+ 0x000000000000000a (STRSZ)              1265 (bytes)
  0x000000000000000b (SYMENT)             24 (bytes)
- 0x0000000000000003 (PLTGOT)             0x9000
+ 0x0000000000000003 (PLTGOT)             0x207000
  0x0000000000000002 (PLTRELSZ)           1056 (bytes)
  0x0000000000000014 (PLTREL)             RELA
- 0x0000000000000017 (JMPREL)             0x1358
- 0x0000000000000007 (RELA)               0x12b0
+ 0x0000000000000017 (JMPREL)             0x1380
+ 0x0000000000000007 (RELA)               0x12d8
  0x0000000000000008 (RELASZ)             168 (bytes)
  0x0000000000000009 (RELAENT)            24 (bytes)
- 0x000000006ffffffe (VERNEED)            0x1280
+ 0x000000006ffffffe (VERNEED)            0x12a8
  0x000000006fffffff (VERNEEDNUM)         1
- 0x000000006ffffff0 (VERSYM)             0x11cc
+ 0x000000006ffffff0 (VERSYM)             0x11ea
  0x000000006ffffff9 (RELACOUNT)          3
  0x0000000000000000 (NULL)               0x0
```

#### readelf --wide --notes {}

```diff
@@ -1,8 +1,4 @@
 
-Displaying notes found in: .note.gnu.property
-  Owner                Data size 	Description
-  GNU                  0x00000010	NT_GNU_PROPERTY_TYPE_0	      Properties: x86 feature: IBT, SHSTK
-
 Displaying notes found in: .note.gnu.build-id
   Owner                Data size 	Description
-  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: 37a4cd2878d2059672555bf25d625ab3748c7758
+  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: a9d1358c10911257af561997e012a3f6d7611e2d
```

#### readelf --wide --version-info {}

```diff
@@ -1,10 +1,10 @@
 
-Version symbols section '.gnu.version' contains 87 entries:
- Addr: 0x00000000000011cc  Offset: 0x000011cc  Link: 4 (.dynsym)
+Version symbols section '.gnu.version' contains 92 entries:
+ Addr: 0x00000000000011ea  Offset: 0x000011ea  Link: 3 (.dynsym)
   000:   0 (*local*)       2 (GLIBC_2.2.5)   2 (GLIBC_2.2.5)   0 (*local*)    
   004:   2 (GLIBC_2.2.5)   0 (*local*)       2 (GLIBC_2.2.5)   3 (GLIBC_2.4)  
   008:   2 (GLIBC_2.2.5)   2 (GLIBC_2.2.5)   2 (GLIBC_2.2.5)   2 (GLIBC_2.2.5)
   00c:   0 (*local*)       2 (GLIBC_2.2.5)   0 (*local*)       0 (*local*)    
   010:   0 (*local*)       2 (GLIBC_2.2.5)   0 (*local*)       2 (GLIBC_2.2.5)
   014:   0 (*local*)       0 (*local*)       2 (GLIBC_2.2.5)   0 (*local*)    
   018:   2 (GLIBC_2.2.5)   1 (*global*)      1 (*global*)      1 (*global*)   
@@ -18,14 +18,15 @@
   038:   1 (*global*)      1 (*global*)      1 (*global*)      1 (*global*)   
   03c:   1 (*global*)      1 (*global*)      1 (*global*)      1 (*global*)   
   040:   1 (*global*)      1 (*global*)      1 (*global*)      1 (*global*)   
   044:   1 (*global*)      1 (*global*)      1 (*global*)      1 (*global*)   
   048:   1 (*global*)      1 (*global*)      1 (*global*)      1 (*global*)   
   04c:   1 (*global*)      1 (*global*)      1 (*global*)      1 (*global*)   
   050:   1 (*global*)      1 (*global*)      1 (*global*)      1 (*global*)   
-  054:   1 (*global*)      1 (*global*)      1 (*global*)   
+  054:   1 (*global*)      1 (*global*)      1 (*global*)      1 (*global*)   
+  058:   1 (*global*)      1 (*global*)      1 (*global*)      1 (*global*)   
 
 Version needs section '.gnu.version_r' contains 1 entry:
- Addr: 0x0000000000001280  Offset: 0x00001280  Link: 5 (.dynstr)
+ Addr: 0x00000000000012a8  Offset: 0x000012a8  Link: 4 (.dynstr)
   000000: Version: 1  File: libc.so.6  Cnt: 2
   0x0010:   Name: GLIBC_2.4  Flags: none  Version: 3
   0x0020:   Name: GLIBC_2.2.5  Flags: none  Version: 2
```

#### readelf --wide --debug-dump=frames {}

```diff
@@ -9,725 +9,716 @@
   Return address column: 16
   Augmentation data:     1b
   DW_CFA_def_cfa: r7 (rsp) ofs 8
   DW_CFA_offset: r16 (rip) at cfa-8
   DW_CFA_nop
   DW_CFA_nop
 
-00000018 0000000000000024 0000001c FDE cie=00000000 pc=0000000000002020..00000000000022f0
+00000018 0000000000000024 0000001c FDE cie=00000000 pc=00000000000017c0..0000000000001a90
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 6 to 0000000000002026
+  DW_CFA_advance_loc: 6 to 00000000000017c6
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 10 to 0000000000002030
-  DW_CFA_def_cfa_expression (DW_OP_breg7 (rsp): 8; DW_OP_breg16 (rip): 0; DW_OP_lit15; DW_OP_and; DW_OP_lit10; DW_OP_ge; DW_OP_lit3; DW_OP_shl; DW_OP_plus)
+  DW_CFA_advance_loc: 10 to 00000000000017d0
+  DW_CFA_def_cfa_expression (DW_OP_breg7 (rsp): 8; DW_OP_breg16 (rip): 0; DW_OP_lit15; DW_OP_and; DW_OP_lit11; DW_OP_ge; DW_OP_lit3; DW_OP_shl; DW_OP_plus)
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000040 0000000000000014 00000044 FDE cie=00000000 pc=00000000000022f0..0000000000002300
+00000040 0000000000000014 00000044 FDE cie=00000000 pc=0000000000001a90..0000000000001a98
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000058 0000000000000014 0000005c FDE cie=00000000 pc=0000000000002300..00000000000025c0
-  DW_CFA_nop
-  DW_CFA_nop
-  DW_CFA_nop
-  DW_CFA_nop
-  DW_CFA_nop
-  DW_CFA_nop
-  DW_CFA_nop
-
-00000070 000000000000001c 00000074 FDE cie=00000000 pc=0000000000002679..0000000000002808
-  DW_CFA_advance_loc: 5 to 000000000000267e
+00000058 000000000000001c 0000005c FDE cie=00000000 pc=0000000000001b7a..0000000000001d05
+  DW_CFA_advance_loc: 1 to 0000000000001b7b
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r6 (rbp) at cfa-16
-  DW_CFA_advance_loc: 3 to 0000000000002681
+  DW_CFA_advance_loc: 3 to 0000000000001b7e
   DW_CFA_def_cfa_register: r6 (rbp)
-  DW_CFA_advance_loc2: 390 to 0000000000002807
+  DW_CFA_advance_loc2: 390 to 0000000000001d04
   DW_CFA_def_cfa: r7 (rsp) ofs 8
   DW_CFA_nop
 
-00000090 000000000000001c 00000094 FDE cie=00000000 pc=0000000000002808..00000000000029c5
-  DW_CFA_advance_loc: 5 to 000000000000280d
+00000078 000000000000001c 0000007c FDE cie=00000000 pc=0000000000001d05..0000000000001ebe
+  DW_CFA_advance_loc: 1 to 0000000000001d06
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r6 (rbp) at cfa-16
-  DW_CFA_advance_loc: 3 to 0000000000002810
+  DW_CFA_advance_loc: 3 to 0000000000001d09
   DW_CFA_def_cfa_register: r6 (rbp)
-  DW_CFA_advance_loc2: 436 to 00000000000029c4
+  DW_CFA_advance_loc2: 436 to 0000000000001ebd
   DW_CFA_def_cfa: r7 (rsp) ofs 8
   DW_CFA_nop
 
-000000b0 000000000000001c 000000b4 FDE cie=00000000 pc=00000000000029c5..0000000000002b9f
-  DW_CFA_advance_loc: 5 to 00000000000029ca
+00000098 000000000000001c 0000009c FDE cie=00000000 pc=0000000000001ebe..0000000000002094
+  DW_CFA_advance_loc: 1 to 0000000000001ebf
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r6 (rbp) at cfa-16
-  DW_CFA_advance_loc: 3 to 00000000000029cd
+  DW_CFA_advance_loc: 3 to 0000000000001ec2
   DW_CFA_def_cfa_register: r6 (rbp)
-  DW_CFA_advance_loc2: 465 to 0000000000002b9e
+  DW_CFA_advance_loc2: 465 to 0000000000002093
   DW_CFA_def_cfa: r7 (rsp) ofs 8
   DW_CFA_nop
 
-000000d0 000000000000001c 000000d4 FDE cie=00000000 pc=0000000000002b9f..0000000000002d7e
-  DW_CFA_advance_loc: 5 to 0000000000002ba4
+000000b8 000000000000001c 000000bc FDE cie=00000000 pc=0000000000002094..000000000000226f
+  DW_CFA_advance_loc: 1 to 0000000000002095
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r6 (rbp) at cfa-16
-  DW_CFA_advance_loc: 3 to 0000000000002ba7
+  DW_CFA_advance_loc: 3 to 0000000000002098
   DW_CFA_def_cfa_register: r6 (rbp)
-  DW_CFA_advance_loc2: 470 to 0000000000002d7d
+  DW_CFA_advance_loc2: 470 to 000000000000226e
   DW_CFA_def_cfa: r7 (rsp) ofs 8
   DW_CFA_nop
 
-000000f0 000000000000001c 000000f4 FDE cie=00000000 pc=0000000000002d7e..0000000000002f25
-  DW_CFA_advance_loc: 5 to 0000000000002d83
+000000d8 000000000000001c 000000dc FDE cie=00000000 pc=000000000000226f..0000000000002412
+  DW_CFA_advance_loc: 1 to 0000000000002270
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r6 (rbp) at cfa-16
-  DW_CFA_advance_loc: 3 to 0000000000002d86
+  DW_CFA_advance_loc: 3 to 0000000000002273
   DW_CFA_def_cfa_register: r6 (rbp)
-  DW_CFA_advance_loc2: 414 to 0000000000002f24
+  DW_CFA_advance_loc2: 414 to 0000000000002411
   DW_CFA_def_cfa: r7 (rsp) ofs 8
   DW_CFA_nop
 
-00000110 000000000000001c 00000114 FDE cie=00000000 pc=0000000000002f25..00000000000030fb
-  DW_CFA_advance_loc: 5 to 0000000000002f2a
+000000f8 000000000000001c 000000fc FDE cie=00000000 pc=0000000000002412..00000000000025e4
+  DW_CFA_advance_loc: 1 to 0000000000002413
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r6 (rbp) at cfa-16
-  DW_CFA_advance_loc: 3 to 0000000000002f2d
+  DW_CFA_advance_loc: 3 to 0000000000002416
   DW_CFA_def_cfa_register: r6 (rbp)
-  DW_CFA_advance_loc2: 461 to 00000000000030fa
+  DW_CFA_advance_loc2: 461 to 00000000000025e3
   DW_CFA_def_cfa: r7 (rsp) ofs 8
   DW_CFA_nop
 
-00000130 000000000000001c 00000134 FDE cie=00000000 pc=00000000000030fb..00000000000032ef
-  DW_CFA_advance_loc: 5 to 0000000000003100
+00000118 000000000000001c 0000011c FDE cie=00000000 pc=00000000000025e4..00000000000027d4
+  DW_CFA_advance_loc: 1 to 00000000000025e5
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r6 (rbp) at cfa-16
-  DW_CFA_advance_loc: 3 to 0000000000003103
+  DW_CFA_advance_loc: 3 to 00000000000025e8
   DW_CFA_def_cfa_register: r6 (rbp)
-  DW_CFA_advance_loc2: 491 to 00000000000032ee
+  DW_CFA_advance_loc2: 491 to 00000000000027d3
   DW_CFA_def_cfa: r7 (rsp) ofs 8
   DW_CFA_nop
 
-00000150 000000000000001c 00000154 FDE cie=00000000 pc=00000000000032ef..00000000000034e8
-  DW_CFA_advance_loc: 5 to 00000000000032f4
+00000138 000000000000001c 0000013c FDE cie=00000000 pc=00000000000027d4..00000000000029c9
+  DW_CFA_advance_loc: 1 to 00000000000027d5
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r6 (rbp) at cfa-16
-  DW_CFA_advance_loc: 3 to 00000000000032f7
+  DW_CFA_advance_loc: 3 to 00000000000027d8
   DW_CFA_def_cfa_register: r6 (rbp)
-  DW_CFA_advance_loc2: 496 to 00000000000034e7
+  DW_CFA_advance_loc2: 496 to 00000000000029c8
   DW_CFA_def_cfa: r7 (rsp) ofs 8
   DW_CFA_nop
 
-00000170 000000000000001c 00000174 FDE cie=00000000 pc=00000000000034e8..0000000000003568
-  DW_CFA_advance_loc: 5 to 00000000000034ed
+00000158 000000000000001c 0000015c FDE cie=00000000 pc=00000000000029c9..0000000000002a4d
+  DW_CFA_advance_loc: 1 to 00000000000029ca
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r6 (rbp) at cfa-16
-  DW_CFA_advance_loc: 3 to 00000000000034f0
+  DW_CFA_advance_loc: 3 to 00000000000029cd
   DW_CFA_def_cfa_register: r6 (rbp)
-  DW_CFA_advance_loc1: 119 to 0000000000003567
+  DW_CFA_advance_loc1: 127 to 0000000000002a4c
   DW_CFA_def_cfa: r7 (rsp) ofs 8
   DW_CFA_nop
   DW_CFA_nop
 
-00000190 000000000000001c 00000194 FDE cie=00000000 pc=0000000000003568..00000000000035ea
-  DW_CFA_advance_loc: 5 to 000000000000356d
+00000178 000000000000001c 0000017c FDE cie=00000000 pc=0000000000002a4d..0000000000002ad3
+  DW_CFA_advance_loc: 1 to 0000000000002a4e
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r6 (rbp) at cfa-16
-  DW_CFA_advance_loc: 3 to 0000000000003570
+  DW_CFA_advance_loc: 3 to 0000000000002a51
   DW_CFA_def_cfa_register: r6 (rbp)
-  DW_CFA_advance_loc1: 121 to 00000000000035e9
+  DW_CFA_advance_loc1: 129 to 0000000000002ad2
   DW_CFA_def_cfa: r7 (rsp) ofs 8
   DW_CFA_nop
   DW_CFA_nop
 
-000001b0 000000000000001c 000001b4 FDE cie=00000000 pc=00000000000035ea..000000000000366c
-  DW_CFA_advance_loc: 5 to 00000000000035ef
+00000198 000000000000001c 0000019c FDE cie=00000000 pc=0000000000002ad3..0000000000002b59
+  DW_CFA_advance_loc: 1 to 0000000000002ad4
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r6 (rbp) at cfa-16
-  DW_CFA_advance_loc: 3 to 00000000000035f2
+  DW_CFA_advance_loc: 3 to 0000000000002ad7
   DW_CFA_def_cfa_register: r6 (rbp)
-  DW_CFA_advance_loc1: 121 to 000000000000366b
+  DW_CFA_advance_loc1: 129 to 0000000000002b58
   DW_CFA_def_cfa: r7 (rsp) ofs 8
   DW_CFA_nop
   DW_CFA_nop
 
-000001d0 000000000000001c 000001d4 FDE cie=00000000 pc=000000000000366c..00000000000036ea
-  DW_CFA_advance_loc: 5 to 0000000000003671
+000001b8 000000000000001c 000001bc FDE cie=00000000 pc=0000000000002b59..0000000000002bdb
+  DW_CFA_advance_loc: 1 to 0000000000002b5a
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r6 (rbp) at cfa-16
-  DW_CFA_advance_loc: 3 to 0000000000003674
+  DW_CFA_advance_loc: 3 to 0000000000002b5d
   DW_CFA_def_cfa_register: r6 (rbp)
-  DW_CFA_advance_loc1: 117 to 00000000000036e9
+  DW_CFA_advance_loc1: 125 to 0000000000002bda
   DW_CFA_def_cfa: r7 (rsp) ofs 8
   DW_CFA_nop
   DW_CFA_nop
 
-000001f0 000000000000001c 000001f4 FDE cie=00000000 pc=00000000000036ea..000000000000376f
-  DW_CFA_advance_loc: 5 to 00000000000036ef
+000001d8 000000000000001c 000001dc FDE cie=00000000 pc=0000000000002bdb..0000000000002c72
+  DW_CFA_advance_loc: 1 to 0000000000002bdc
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r6 (rbp) at cfa-16
-  DW_CFA_advance_loc: 3 to 00000000000036f2
+  DW_CFA_advance_loc: 3 to 0000000000002bdf
   DW_CFA_def_cfa_register: r6 (rbp)
-  DW_CFA_advance_loc1: 124 to 000000000000376e
+  DW_CFA_advance_loc1: 146 to 0000000000002c71
   DW_CFA_def_cfa: r7 (rsp) ofs 8
   DW_CFA_nop
   DW_CFA_nop
 
-00000210 000000000000001c 00000214 FDE cie=00000000 pc=000000000000376f..00000000000037f6
-  DW_CFA_advance_loc: 5 to 0000000000003774
+000001f8 000000000000001c 000001fc FDE cie=00000000 pc=0000000000002c72..0000000000002d0b
+  DW_CFA_advance_loc: 1 to 0000000000002c73
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r6 (rbp) at cfa-16
-  DW_CFA_advance_loc: 3 to 0000000000003777
+  DW_CFA_advance_loc: 3 to 0000000000002c76
   DW_CFA_def_cfa_register: r6 (rbp)
-  DW_CFA_advance_loc1: 126 to 00000000000037f5
+  DW_CFA_advance_loc1: 148 to 0000000000002d0a
   DW_CFA_def_cfa: r7 (rsp) ofs 8
   DW_CFA_nop
   DW_CFA_nop
 
-00000230 000000000000001c 00000234 FDE cie=00000000 pc=00000000000037f6..000000000000387d
-  DW_CFA_advance_loc: 5 to 00000000000037fb
+00000218 000000000000001c 0000021c FDE cie=00000000 pc=0000000000002d0b..0000000000002da4
+  DW_CFA_advance_loc: 1 to 0000000000002d0c
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r6 (rbp) at cfa-16
-  DW_CFA_advance_loc: 3 to 00000000000037fe
+  DW_CFA_advance_loc: 3 to 0000000000002d0f
   DW_CFA_def_cfa_register: r6 (rbp)
-  DW_CFA_advance_loc1: 126 to 000000000000387c
+  DW_CFA_advance_loc1: 148 to 0000000000002da3
   DW_CFA_def_cfa: r7 (rsp) ofs 8
   DW_CFA_nop
   DW_CFA_nop
 
-00000250 000000000000001c 00000254 FDE cie=00000000 pc=000000000000387d..0000000000003900
-  DW_CFA_advance_loc: 5 to 0000000000003882
+00000238 000000000000001c 0000023c FDE cie=00000000 pc=0000000000002da4..0000000000002e39
+  DW_CFA_advance_loc: 1 to 0000000000002da5
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r6 (rbp) at cfa-16
-  DW_CFA_advance_loc: 3 to 0000000000003885
+  DW_CFA_advance_loc: 3 to 0000000000002da8
   DW_CFA_def_cfa_register: r6 (rbp)
-  DW_CFA_advance_loc1: 122 to 00000000000038ff
+  DW_CFA_advance_loc1: 144 to 0000000000002e38
   DW_CFA_def_cfa: r7 (rsp) ofs 8
   DW_CFA_nop
   DW_CFA_nop
 
-00000270 000000000000001c 00000274 FDE cie=00000000 pc=0000000000003900..000000000000392c
-  DW_CFA_advance_loc: 5 to 0000000000003905
+00000258 000000000000001c 0000025c FDE cie=00000000 pc=0000000000002e39..0000000000002e61
+  DW_CFA_advance_loc: 1 to 0000000000002e3a
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r6 (rbp) at cfa-16
-  DW_CFA_advance_loc: 3 to 0000000000003908
+  DW_CFA_advance_loc: 3 to 0000000000002e3d
   DW_CFA_def_cfa_register: r6 (rbp)
-  DW_CFA_advance_loc: 35 to 000000000000392b
+  DW_CFA_advance_loc: 35 to 0000000000002e60
   DW_CFA_def_cfa: r7 (rsp) ofs 8
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000290 000000000000001c 00000294 FDE cie=00000000 pc=000000000000392c..000000000000395a
-  DW_CFA_advance_loc: 5 to 0000000000003931
+00000278 000000000000001c 0000027c FDE cie=00000000 pc=0000000000002e61..0000000000002e8b
+  DW_CFA_advance_loc: 1 to 0000000000002e62
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r6 (rbp) at cfa-16
-  DW_CFA_advance_loc: 3 to 0000000000003934
+  DW_CFA_advance_loc: 3 to 0000000000002e65
   DW_CFA_def_cfa_register: r6 (rbp)
-  DW_CFA_advance_loc: 37 to 0000000000003959
+  DW_CFA_advance_loc: 37 to 0000000000002e8a
   DW_CFA_def_cfa: r7 (rsp) ofs 8
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-000002b0 000000000000001c 000002b4 FDE cie=00000000 pc=000000000000395a..0000000000003988
-  DW_CFA_advance_loc: 5 to 000000000000395f
+00000298 000000000000001c 0000029c FDE cie=00000000 pc=0000000000002e8b..0000000000002eb5
+  DW_CFA_advance_loc: 1 to 0000000000002e8c
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r6 (rbp) at cfa-16
-  DW_CFA_advance_loc: 3 to 0000000000003962
+  DW_CFA_advance_loc: 3 to 0000000000002e8f
   DW_CFA_def_cfa_register: r6 (rbp)
-  DW_CFA_advance_loc: 37 to 0000000000003987
+  DW_CFA_advance_loc: 37 to 0000000000002eb4
   DW_CFA_def_cfa: r7 (rsp) ofs 8
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-000002d0 000000000000001c 000002d4 FDE cie=00000000 pc=0000000000003988..00000000000039b6
-  DW_CFA_advance_loc: 5 to 000000000000398d
+000002b8 000000000000001c 000002bc FDE cie=00000000 pc=0000000000002eb5..0000000000002ee3
+  DW_CFA_advance_loc: 1 to 0000000000002eb6
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r6 (rbp) at cfa-16
-  DW_CFA_advance_loc: 3 to 0000000000003990
+  DW_CFA_advance_loc: 3 to 0000000000002eb9
   DW_CFA_def_cfa_register: r6 (rbp)
-  DW_CFA_advance_loc: 37 to 00000000000039b5
+  DW_CFA_advance_loc: 41 to 0000000000002ee2
   DW_CFA_def_cfa: r7 (rsp) ofs 8
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-000002f0 000000000000001c 000002f4 FDE cie=00000000 pc=00000000000039b6..00000000000039ff
-  DW_CFA_advance_loc: 5 to 00000000000039bb
+000002d8 000000000000001c 000002dc FDE cie=00000000 pc=0000000000002ee3..0000000000002f28
+  DW_CFA_advance_loc: 1 to 0000000000002ee4
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r6 (rbp) at cfa-16
-  DW_CFA_advance_loc: 3 to 00000000000039be
+  DW_CFA_advance_loc: 3 to 0000000000002ee7
   DW_CFA_def_cfa_register: r6 (rbp)
-  DW_CFA_advance_loc1: 64 to 00000000000039fe
+  DW_CFA_advance_loc1: 64 to 0000000000002f27
   DW_CFA_def_cfa: r7 (rsp) ofs 8
   DW_CFA_nop
   DW_CFA_nop
 
-00000310 000000000000001c 00000314 FDE cie=00000000 pc=00000000000039ff..0000000000003a4c
-  DW_CFA_advance_loc: 5 to 0000000000003a04
+000002f8 000000000000001c 000002fc FDE cie=00000000 pc=0000000000002f28..0000000000002f71
+  DW_CFA_advance_loc: 1 to 0000000000002f29
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r6 (rbp) at cfa-16
-  DW_CFA_advance_loc: 3 to 0000000000003a07
+  DW_CFA_advance_loc: 3 to 0000000000002f2c
   DW_CFA_def_cfa_register: r6 (rbp)
-  DW_CFA_advance_loc1: 68 to 0000000000003a4b
+  DW_CFA_advance_loc1: 68 to 0000000000002f70
   DW_CFA_def_cfa: r7 (rsp) ofs 8
   DW_CFA_nop
   DW_CFA_nop
 
-00000330 000000000000001c 00000334 FDE cie=00000000 pc=0000000000003a4c..0000000000003aa6
-  DW_CFA_advance_loc: 5 to 0000000000003a51
+00000318 000000000000001c 0000031c FDE cie=00000000 pc=0000000000002f71..0000000000002fc7
+  DW_CFA_advance_loc: 1 to 0000000000002f72
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r6 (rbp) at cfa-16
-  DW_CFA_advance_loc: 3 to 0000000000003a54
+  DW_CFA_advance_loc: 3 to 0000000000002f75
   DW_CFA_def_cfa_register: r6 (rbp)
-  DW_CFA_advance_loc1: 81 to 0000000000003aa5
+  DW_CFA_advance_loc1: 81 to 0000000000002fc6
   DW_CFA_def_cfa: r7 (rsp) ofs 8
   DW_CFA_nop
   DW_CFA_nop
 
-00000350 000000000000001c 00000354 FDE cie=00000000 pc=0000000000003aa6..0000000000003b00
-  DW_CFA_advance_loc: 5 to 0000000000003aab
+00000338 000000000000001c 0000033c FDE cie=00000000 pc=0000000000002fc7..000000000000301d
+  DW_CFA_advance_loc: 1 to 0000000000002fc8
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r6 (rbp) at cfa-16
-  DW_CFA_advance_loc: 3 to 0000000000003aae
+  DW_CFA_advance_loc: 3 to 0000000000002fcb
   DW_CFA_def_cfa_register: r6 (rbp)
-  DW_CFA_advance_loc1: 81 to 0000000000003aff
+  DW_CFA_advance_loc1: 81 to 000000000000301c
   DW_CFA_def_cfa: r7 (rsp) ofs 8
   DW_CFA_nop
   DW_CFA_nop
 
-00000370 000000000000001c 00000374 FDE cie=00000000 pc=0000000000003b00..0000000000003b22
-  DW_CFA_advance_loc: 5 to 0000000000003b05
+00000358 000000000000001c 0000035c FDE cie=00000000 pc=000000000000301d..000000000000303b
+  DW_CFA_advance_loc: 1 to 000000000000301e
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r6 (rbp) at cfa-16
-  DW_CFA_advance_loc: 3 to 0000000000003b08
+  DW_CFA_advance_loc: 3 to 0000000000003021
   DW_CFA_def_cfa_register: r6 (rbp)
-  DW_CFA_advance_loc: 25 to 0000000000003b21
+  DW_CFA_advance_loc: 25 to 000000000000303a
   DW_CFA_def_cfa: r7 (rsp) ofs 8
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000390 000000000000001c 00000394 FDE cie=00000000 pc=0000000000003b22..0000000000003b48
-  DW_CFA_advance_loc: 5 to 0000000000003b27
+00000378 000000000000001c 0000037c FDE cie=00000000 pc=000000000000303b..000000000000305d
+  DW_CFA_advance_loc: 1 to 000000000000303c
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r6 (rbp) at cfa-16
-  DW_CFA_advance_loc: 3 to 0000000000003b2a
+  DW_CFA_advance_loc: 3 to 000000000000303f
   DW_CFA_def_cfa_register: r6 (rbp)
-  DW_CFA_advance_loc: 29 to 0000000000003b47
+  DW_CFA_advance_loc: 29 to 000000000000305c
   DW_CFA_def_cfa: r7 (rsp) ofs 8
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-000003b0 000000000000001c 000003b4 FDE cie=00000000 pc=0000000000003b48..0000000000003b9e
-  DW_CFA_advance_loc: 5 to 0000000000003b4d
+00000398 000000000000001c 0000039c FDE cie=00000000 pc=000000000000305d..00000000000030af
+  DW_CFA_advance_loc: 1 to 000000000000305e
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r6 (rbp) at cfa-16
-  DW_CFA_advance_loc: 3 to 0000000000003b50
+  DW_CFA_advance_loc: 3 to 0000000000003061
   DW_CFA_def_cfa_register: r6 (rbp)
-  DW_CFA_advance_loc1: 77 to 0000000000003b9d
+  DW_CFA_advance_loc1: 77 to 00000000000030ae
   DW_CFA_def_cfa: r7 (rsp) ofs 8
   DW_CFA_nop
   DW_CFA_nop
 
-000003d0 000000000000001c 000003d4 FDE cie=00000000 pc=0000000000003b9e..0000000000003bf6
-  DW_CFA_advance_loc: 5 to 0000000000003ba3
+000003b8 000000000000001c 000003bc FDE cie=00000000 pc=00000000000030af..0000000000003103
+  DW_CFA_advance_loc: 1 to 00000000000030b0
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r6 (rbp) at cfa-16
-  DW_CFA_advance_loc: 3 to 0000000000003ba6
+  DW_CFA_advance_loc: 3 to 00000000000030b3
   DW_CFA_def_cfa_register: r6 (rbp)
-  DW_CFA_advance_loc1: 79 to 0000000000003bf5
+  DW_CFA_advance_loc1: 79 to 0000000000003102
   DW_CFA_def_cfa: r7 (rsp) ofs 8
   DW_CFA_nop
   DW_CFA_nop
 
-000003f0 000000000000001c 000003f4 FDE cie=00000000 pc=0000000000003bf6..0000000000003c73
-  DW_CFA_advance_loc: 5 to 0000000000003bfb
+000003d8 000000000000001c 000003dc FDE cie=00000000 pc=0000000000003103..000000000000317c
+  DW_CFA_advance_loc: 1 to 0000000000003104
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r6 (rbp) at cfa-16
-  DW_CFA_advance_loc: 3 to 0000000000003bfe
+  DW_CFA_advance_loc: 3 to 0000000000003107
   DW_CFA_def_cfa_register: r6 (rbp)
-  DW_CFA_advance_loc1: 116 to 0000000000003c72
+  DW_CFA_advance_loc1: 116 to 000000000000317b
   DW_CFA_def_cfa: r7 (rsp) ofs 8
   DW_CFA_nop
   DW_CFA_nop
 
-00000410 000000000000001c 00000414 FDE cie=00000000 pc=0000000000003c73..0000000000003e5a
-  DW_CFA_advance_loc: 5 to 0000000000003c78
+000003f8 000000000000001c 000003fc FDE cie=00000000 pc=000000000000317c..000000000000335f
+  DW_CFA_advance_loc: 1 to 000000000000317d
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r6 (rbp) at cfa-16
-  DW_CFA_advance_loc: 3 to 0000000000003c7b
+  DW_CFA_advance_loc: 3 to 0000000000003180
   DW_CFA_def_cfa_register: r6 (rbp)
-  DW_CFA_advance_loc2: 478 to 0000000000003e59
+  DW_CFA_advance_loc2: 478 to 000000000000335e
   DW_CFA_def_cfa: r7 (rsp) ofs 8
   DW_CFA_nop
 
-00000430 000000000000001c 00000434 FDE cie=00000000 pc=0000000000003e5a..0000000000003e9c
-  DW_CFA_advance_loc: 5 to 0000000000003e5f
+00000418 000000000000001c 0000041c FDE cie=00000000 pc=000000000000335f..00000000000033a3
+  DW_CFA_advance_loc: 1 to 0000000000003360
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r6 (rbp) at cfa-16
-  DW_CFA_advance_loc: 3 to 0000000000003e62
+  DW_CFA_advance_loc: 3 to 0000000000003363
   DW_CFA_def_cfa_register: r6 (rbp)
-  DW_CFA_advance_loc: 57 to 0000000000003e9b
+  DW_CFA_advance_loc: 63 to 00000000000033a2
   DW_CFA_def_cfa: r7 (rsp) ofs 8
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000450 000000000000001c 00000454 FDE cie=00000000 pc=0000000000003e9c..0000000000003ee7
-  DW_CFA_advance_loc: 5 to 0000000000003ea1
+00000438 000000000000001c 0000043c FDE cie=00000000 pc=00000000000033a3..00000000000033ea
+  DW_CFA_advance_loc: 1 to 00000000000033a4
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r6 (rbp) at cfa-16
-  DW_CFA_advance_loc: 3 to 0000000000003ea4
+  DW_CFA_advance_loc: 3 to 00000000000033a7
   DW_CFA_def_cfa_register: r6 (rbp)
-  DW_CFA_advance_loc1: 66 to 0000000000003ee6
+  DW_CFA_advance_loc1: 66 to 00000000000033e9
   DW_CFA_def_cfa: r7 (rsp) ofs 8
   DW_CFA_nop
   DW_CFA_nop
 
-00000470 000000000000001c 00000474 FDE cie=00000000 pc=0000000000003ee7..0000000000003f52
-  DW_CFA_advance_loc: 5 to 0000000000003eec
+00000458 000000000000001c 0000045c FDE cie=00000000 pc=00000000000033ea..0000000000003451
+  DW_CFA_advance_loc: 1 to 00000000000033eb
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r6 (rbp) at cfa-16
-  DW_CFA_advance_loc: 3 to 0000000000003eef
+  DW_CFA_advance_loc: 3 to 00000000000033ee
   DW_CFA_def_cfa_register: r6 (rbp)
-  DW_CFA_advance_loc1: 98 to 0000000000003f51
+  DW_CFA_advance_loc1: 98 to 0000000000003450
   DW_CFA_def_cfa: r7 (rsp) ofs 8
   DW_CFA_nop
   DW_CFA_nop
 
-00000490 000000000000001c 00000494 FDE cie=00000000 pc=0000000000003f52..0000000000003f9d
-  DW_CFA_advance_loc: 5 to 0000000000003f57
+00000478 000000000000001c 0000047c FDE cie=00000000 pc=0000000000003451..0000000000003498
+  DW_CFA_advance_loc: 1 to 0000000000003452
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r6 (rbp) at cfa-16
-  DW_CFA_advance_loc: 3 to 0000000000003f5a
+  DW_CFA_advance_loc: 3 to 0000000000003455
   DW_CFA_def_cfa_register: r6 (rbp)
-  DW_CFA_advance_loc1: 66 to 0000000000003f9c
+  DW_CFA_advance_loc1: 66 to 0000000000003497
   DW_CFA_def_cfa: r7 (rsp) ofs 8
   DW_CFA_nop
   DW_CFA_nop
 
-000004b0 000000000000001c 000004b4 FDE cie=00000000 pc=0000000000003f9d..0000000000004009
-  DW_CFA_advance_loc: 5 to 0000000000003fa2
+00000498 000000000000001c 0000049c FDE cie=00000000 pc=0000000000003498..0000000000003500
+  DW_CFA_advance_loc: 1 to 0000000000003499
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r6 (rbp) at cfa-16
-  DW_CFA_advance_loc: 3 to 0000000000003fa5
+  DW_CFA_advance_loc: 3 to 000000000000349c
   DW_CFA_def_cfa_register: r6 (rbp)
-  DW_CFA_advance_loc1: 99 to 0000000000004008
+  DW_CFA_advance_loc1: 99 to 00000000000034ff
   DW_CFA_def_cfa: r7 (rsp) ofs 8
   DW_CFA_nop
   DW_CFA_nop
 
-000004d0 000000000000001c 000004d4 FDE cie=00000000 pc=0000000000004009..000000000000408e
-  DW_CFA_advance_loc: 5 to 000000000000400e
+000004b8 000000000000001c 000004bc FDE cie=00000000 pc=0000000000003500..0000000000003589
+  DW_CFA_advance_loc: 1 to 0000000000003501
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r6 (rbp) at cfa-16
-  DW_CFA_advance_loc: 3 to 0000000000004011
+  DW_CFA_advance_loc: 3 to 0000000000003504
   DW_CFA_def_cfa_register: r6 (rbp)
-  DW_CFA_advance_loc1: 124 to 000000000000408d
+  DW_CFA_advance_loc1: 132 to 0000000000003588
   DW_CFA_def_cfa: r7 (rsp) ofs 8
   DW_CFA_nop
   DW_CFA_nop
 
-000004f0 000000000000001c 000004f4 FDE cie=00000000 pc=000000000000408e..00000000000040ec
-  DW_CFA_advance_loc: 5 to 0000000000004093
+000004d8 000000000000001c 000004dc FDE cie=00000000 pc=0000000000003589..00000000000035f6
+  DW_CFA_advance_loc: 1 to 000000000000358a
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r6 (rbp) at cfa-16
-  DW_CFA_advance_loc: 3 to 0000000000004096
+  DW_CFA_advance_loc: 3 to 000000000000358d
   DW_CFA_def_cfa_register: r6 (rbp)
-  DW_CFA_advance_loc1: 85 to 00000000000040eb
+  DW_CFA_advance_loc1: 104 to 00000000000035f5
   DW_CFA_def_cfa: r7 (rsp) ofs 8
   DW_CFA_nop
   DW_CFA_nop
 
-00000510 000000000000001c 00000514 FDE cie=00000000 pc=00000000000040ec..00000000000041bd
-  DW_CFA_advance_loc: 5 to 00000000000040f1
+000004f8 000000000000001c 000004fc FDE cie=00000000 pc=00000000000035f6..00000000000036fb
+  DW_CFA_advance_loc: 1 to 00000000000035f7
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r6 (rbp) at cfa-16
-  DW_CFA_advance_loc: 3 to 00000000000040f4
+  DW_CFA_advance_loc: 3 to 00000000000035fa
   DW_CFA_def_cfa_register: r6 (rbp)
-  DW_CFA_advance_loc1: 200 to 00000000000041bc
+  DW_CFA_advance_loc2: 256 to 00000000000036fa
   DW_CFA_def_cfa: r7 (rsp) ofs 8
   DW_CFA_nop
-  DW_CFA_nop
 
-00000530 000000000000001c 00000534 FDE cie=00000000 pc=00000000000041bd..00000000000042d5
-  DW_CFA_advance_loc: 5 to 00000000000041c2
+00000518 000000000000001c 0000051c FDE cie=00000000 pc=00000000000036fb..0000000000003847
+  DW_CFA_advance_loc: 1 to 00000000000036fc
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r6 (rbp) at cfa-16
-  DW_CFA_advance_loc: 3 to 00000000000041c5
+  DW_CFA_advance_loc: 3 to 00000000000036ff
   DW_CFA_def_cfa_register: r6 (rbp)
-  DW_CFA_advance_loc2: 271 to 00000000000042d4
+  DW_CFA_advance_loc2: 327 to 0000000000003846
   DW_CFA_def_cfa: r7 (rsp) ofs 8
   DW_CFA_nop
 
-00000550 000000000000001c 00000554 FDE cie=00000000 pc=00000000000042d5..000000000000438a
-  DW_CFA_advance_loc: 5 to 00000000000042da
+00000538 000000000000001c 0000053c FDE cie=00000000 pc=0000000000003847..00000000000038f8
+  DW_CFA_advance_loc: 1 to 0000000000003848
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r6 (rbp) at cfa-16
-  DW_CFA_advance_loc: 3 to 00000000000042dd
+  DW_CFA_advance_loc: 3 to 000000000000384b
   DW_CFA_def_cfa_register: r6 (rbp)
-  DW_CFA_advance_loc1: 172 to 0000000000004389
+  DW_CFA_advance_loc1: 172 to 00000000000038f7
   DW_CFA_def_cfa: r7 (rsp) ofs 8
   DW_CFA_nop
   DW_CFA_nop
 
-00000570 000000000000001c 00000574 FDE cie=00000000 pc=000000000000438a..00000000000043b9
-  DW_CFA_advance_loc: 5 to 000000000000438f
+00000558 000000000000001c 0000055c FDE cie=00000000 pc=00000000000038f8..0000000000003923
+  DW_CFA_advance_loc: 1 to 00000000000038f9
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r6 (rbp) at cfa-16
-  DW_CFA_advance_loc: 3 to 0000000000004392
+  DW_CFA_advance_loc: 3 to 00000000000038fc
   DW_CFA_def_cfa_register: r6 (rbp)
-  DW_CFA_advance_loc: 38 to 00000000000043b8
+  DW_CFA_advance_loc: 38 to 0000000000003922
   DW_CFA_def_cfa: r7 (rsp) ofs 8
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000590 0000000000000020 00000594 FDE cie=00000000 pc=00000000000043b9..0000000000004612
-  DW_CFA_advance_loc: 5 to 00000000000043be
+00000578 0000000000000020 0000057c FDE cie=00000000 pc=0000000000003923..0000000000003b7d
+  DW_CFA_advance_loc: 1 to 0000000000003924
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r6 (rbp) at cfa-16
-  DW_CFA_advance_loc: 3 to 00000000000043c1
+  DW_CFA_advance_loc: 3 to 0000000000003927
   DW_CFA_def_cfa_register: r6 (rbp)
-  DW_CFA_advance_loc: 5 to 00000000000043c6
+  DW_CFA_advance_loc: 5 to 000000000000392c
   DW_CFA_offset: r3 (rbx) at cfa-24
-  DW_CFA_advance_loc2: 587 to 0000000000004611
+  DW_CFA_advance_loc2: 592 to 0000000000003b7c
   DW_CFA_def_cfa: r7 (rsp) ofs 8
   DW_CFA_nop
   DW_CFA_nop
 
-000005b4 000000000000001c 000005b8 FDE cie=00000000 pc=0000000000004612..0000000000004a36
-  DW_CFA_advance_loc: 5 to 0000000000004617
+0000059c 000000000000001c 000005a0 FDE cie=00000000 pc=0000000000003b7d..0000000000003f7d
+  DW_CFA_advance_loc: 1 to 0000000000003b7e
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r6 (rbp) at cfa-16
-  DW_CFA_advance_loc: 3 to 000000000000461a
+  DW_CFA_advance_loc: 3 to 0000000000003b81
   DW_CFA_def_cfa_register: r6 (rbp)
-  DW_CFA_advance_loc2: 1051 to 0000000000004a35
+  DW_CFA_advance_loc2: 1019 to 0000000000003f7c
   DW_CFA_def_cfa: r7 (rsp) ofs 8
   DW_CFA_nop
 
-000005d4 0000000000000020 000005d8 FDE cie=00000000 pc=0000000000004a36..0000000000004bd5
-  DW_CFA_advance_loc: 5 to 0000000000004a3b
+000005bc 000000000000001c 000005c0 FDE cie=00000000 pc=0000000000003f7d..0000000000004130
+  DW_CFA_advance_loc: 1 to 0000000000003f7e
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r6 (rbp) at cfa-16
-  DW_CFA_advance_loc: 3 to 0000000000004a3e
+  DW_CFA_advance_loc: 3 to 0000000000003f81
   DW_CFA_def_cfa_register: r6 (rbp)
-  DW_CFA_advance_loc: 5 to 0000000000004a43
-  DW_CFA_offset: r3 (rbx) at cfa-24
-  DW_CFA_advance_loc2: 401 to 0000000000004bd4
+  DW_CFA_advance_loc2: 430 to 000000000000412f
   DW_CFA_def_cfa: r7 (rsp) ofs 8
   DW_CFA_nop
-  DW_CFA_nop
 
-000005f8 000000000000001c 000005fc FDE cie=00000000 pc=0000000000004bd5..0000000000004d25
-  DW_CFA_advance_loc: 5 to 0000000000004bda
+000005dc 0000000000000020 000005e0 FDE cie=00000000 pc=0000000000004130..000000000000427c
+  DW_CFA_advance_loc: 1 to 0000000000004131
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r6 (rbp) at cfa-16
-  DW_CFA_advance_loc: 3 to 0000000000004bdd
+  DW_CFA_advance_loc: 3 to 0000000000004134
   DW_CFA_def_cfa_register: r6 (rbp)
-  DW_CFA_advance_loc2: 327 to 0000000000004d24
+  DW_CFA_advance_loc2: 327 to 000000000000427b
   DW_CFA_def_cfa: r7 (rsp) ofs 8
   DW_CFA_nop
+  DW_CFA_nop
+  DW_CFA_nop
+  DW_CFA_nop
+  DW_CFA_nop
 
-00000618 0000000000000020 0000061c FDE cie=00000000 pc=0000000000004d25..00000000000051a2
-  DW_CFA_advance_loc: 5 to 0000000000004d2a
+00000600 0000000000000020 00000604 FDE cie=00000000 pc=000000000000427c..00000000000046fd
+  DW_CFA_advance_loc: 1 to 000000000000427d
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r6 (rbp) at cfa-16
-  DW_CFA_advance_loc: 3 to 0000000000004d2d
+  DW_CFA_advance_loc: 3 to 0000000000004280
   DW_CFA_def_cfa_register: r6 (rbp)
-  DW_CFA_advance_loc: 8 to 0000000000004d35
+  DW_CFA_advance_loc: 8 to 0000000000004288
   DW_CFA_offset: r3 (rbx) at cfa-24
-  DW_CFA_advance_loc2: 1132 to 00000000000051a1
+  DW_CFA_advance_loc2: 1140 to 00000000000046fc
   DW_CFA_def_cfa: r7 (rsp) ofs 8
   DW_CFA_nop
   DW_CFA_nop
 
-0000063c 000000000000001c 00000640 FDE cie=00000000 pc=00000000000051a2..0000000000005540
-  DW_CFA_advance_loc: 5 to 00000000000051a7
+00000624 000000000000001c 00000628 FDE cie=00000000 pc=00000000000046fd..0000000000004a9e
+  DW_CFA_advance_loc: 1 to 00000000000046fe
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r6 (rbp) at cfa-16
-  DW_CFA_advance_loc: 3 to 00000000000051aa
+  DW_CFA_advance_loc: 3 to 0000000000004701
   DW_CFA_def_cfa_register: r6 (rbp)
-  DW_CFA_advance_loc2: 917 to 000000000000553f
+  DW_CFA_advance_loc2: 924 to 0000000000004a9d
   DW_CFA_def_cfa: r7 (rsp) ofs 8
   DW_CFA_nop
 
-0000065c 000000000000001c 00000660 FDE cie=00000000 pc=0000000000005540..0000000000005598
-  DW_CFA_advance_loc: 5 to 0000000000005545
+00000644 000000000000001c 00000648 FDE cie=00000000 pc=0000000000004a9e..0000000000004af2
+  DW_CFA_advance_loc: 1 to 0000000000004a9f
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r6 (rbp) at cfa-16
-  DW_CFA_advance_loc: 3 to 0000000000005548
+  DW_CFA_advance_loc: 3 to 0000000000004aa2
   DW_CFA_def_cfa_register: r6 (rbp)
-  DW_CFA_advance_loc1: 79 to 0000000000005597
+  DW_CFA_advance_loc1: 79 to 0000000000004af1
   DW_CFA_def_cfa: r7 (rsp) ofs 8
   DW_CFA_nop
   DW_CFA_nop
 
-0000067c 000000000000001c 00000680 FDE cie=00000000 pc=0000000000005598..00000000000055f4
-  DW_CFA_advance_loc: 5 to 000000000000559d
+00000664 000000000000001c 00000668 FDE cie=00000000 pc=0000000000004af2..0000000000004b4a
+  DW_CFA_advance_loc: 1 to 0000000000004af3
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r6 (rbp) at cfa-16
-  DW_CFA_advance_loc: 3 to 00000000000055a0
+  DW_CFA_advance_loc: 3 to 0000000000004af6
   DW_CFA_def_cfa_register: r6 (rbp)
-  DW_CFA_advance_loc1: 83 to 00000000000055f3
+  DW_CFA_advance_loc1: 83 to 0000000000004b49
   DW_CFA_def_cfa: r7 (rsp) ofs 8
   DW_CFA_nop
   DW_CFA_nop
 
-0000069c 000000000000001c 000006a0 FDE cie=00000000 pc=00000000000055f4..00000000000056a4
-  DW_CFA_advance_loc: 5 to 00000000000055f9
+00000684 000000000000001c 00000688 FDE cie=00000000 pc=0000000000004b4a..0000000000004bf5
+  DW_CFA_advance_loc: 1 to 0000000000004b4b
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r6 (rbp) at cfa-16
-  DW_CFA_advance_loc: 3 to 00000000000055fc
+  DW_CFA_advance_loc: 3 to 0000000000004b4e
   DW_CFA_def_cfa_register: r6 (rbp)
-  DW_CFA_advance_loc1: 167 to 00000000000056a3
+  DW_CFA_advance_loc1: 166 to 0000000000004bf4
   DW_CFA_def_cfa: r7 (rsp) ofs 8
   DW_CFA_nop
   DW_CFA_nop
 
-000006bc 000000000000001c 000006c0 FDE cie=00000000 pc=00000000000056a4..0000000000005730
-  DW_CFA_advance_loc: 5 to 00000000000056a9
+000006a4 000000000000001c 000006a8 FDE cie=00000000 pc=0000000000004bf5..0000000000004c7c
+  DW_CFA_advance_loc: 1 to 0000000000004bf6
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r6 (rbp) at cfa-16
-  DW_CFA_advance_loc: 3 to 00000000000056ac
+  DW_CFA_advance_loc: 3 to 0000000000004bf9
   DW_CFA_def_cfa_register: r6 (rbp)
-  DW_CFA_advance_loc1: 131 to 000000000000572f
+  DW_CFA_advance_loc1: 130 to 0000000000004c7b
   DW_CFA_def_cfa: r7 (rsp) ofs 8
   DW_CFA_nop
   DW_CFA_nop
 
-000006dc 0000000000000020 000006e0 FDE cie=00000000 pc=0000000000005730..00000000000058f6
-  DW_CFA_advance_loc: 5 to 0000000000005735
+000006c4 0000000000000020 000006c8 FDE cie=00000000 pc=0000000000004c7c..0000000000004e48
+  DW_CFA_advance_loc: 1 to 0000000000004c7d
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r6 (rbp) at cfa-16
-  DW_CFA_advance_loc: 3 to 0000000000005738
+  DW_CFA_advance_loc: 3 to 0000000000004c80
   DW_CFA_def_cfa_register: r6 (rbp)
-  DW_CFA_advance_loc2: 445 to 00000000000058f5
+  DW_CFA_advance_loc2: 455 to 0000000000004e47
   DW_CFA_def_cfa: r7 (rsp) ofs 8
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000700 000000000000001c 00000704 FDE cie=00000000 pc=00000000000058f6..00000000000059ae
-  DW_CFA_advance_loc: 5 to 00000000000058fb
+000006e8 000000000000001c 000006ec FDE cie=00000000 pc=0000000000004e48..0000000000004f02
+  DW_CFA_advance_loc: 1 to 0000000000004e49
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r6 (rbp) at cfa-16
-  DW_CFA_advance_loc: 3 to 00000000000058fe
+  DW_CFA_advance_loc: 3 to 0000000000004e4c
   DW_CFA_def_cfa_register: r6 (rbp)
-  DW_CFA_advance_loc1: 175 to 00000000000059ad
+  DW_CFA_advance_loc1: 181 to 0000000000004f01
   DW_CFA_def_cfa: r7 (rsp) ofs 8
   DW_CFA_nop
   DW_CFA_nop
 
-00000720 000000000000001c 00000724 FDE cie=00000000 pc=00000000000059ae..0000000000005a1f
-  DW_CFA_advance_loc: 5 to 00000000000059b3
+00000708 000000000000001c 0000070c FDE cie=00000000 pc=0000000000004f02..0000000000004f6f
+  DW_CFA_advance_loc: 1 to 0000000000004f03
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r6 (rbp) at cfa-16
-  DW_CFA_advance_loc: 3 to 00000000000059b6
+  DW_CFA_advance_loc: 3 to 0000000000004f06
   DW_CFA_def_cfa_register: r6 (rbp)
-  DW_CFA_advance_loc1: 104 to 0000000000005a1e
+  DW_CFA_advance_loc1: 104 to 0000000000004f6e
   DW_CFA_def_cfa: r7 (rsp) ofs 8
   DW_CFA_nop
   DW_CFA_nop
 
-00000740 000000000000001c 00000744 FDE cie=00000000 pc=0000000000005a1f..0000000000005f1d
-  DW_CFA_advance_loc: 5 to 0000000000005a24
+00000728 000000000000001c 0000072c FDE cie=00000000 pc=0000000000004f6f..000000000000545e
+  DW_CFA_advance_loc: 1 to 0000000000004f70
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r6 (rbp) at cfa-16
-  DW_CFA_advance_loc: 3 to 0000000000005a27
+  DW_CFA_advance_loc: 3 to 0000000000004f73
   DW_CFA_def_cfa_register: r6 (rbp)
-  DW_CFA_advance_loc2: 1269 to 0000000000005f1c
+  DW_CFA_advance_loc2: 1258 to 000000000000545d
   DW_CFA_def_cfa: r7 (rsp) ofs 8
   DW_CFA_nop
 
-00000760 000000000000001c 00000764 FDE cie=00000000 pc=0000000000005f1d..0000000000005f40
-  DW_CFA_advance_loc: 5 to 0000000000005f22
+00000748 000000000000001c 0000074c FDE cie=00000000 pc=000000000000545e..000000000000547d
+  DW_CFA_advance_loc: 1 to 000000000000545f
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r6 (rbp) at cfa-16
-  DW_CFA_advance_loc: 3 to 0000000000005f25
+  DW_CFA_advance_loc: 3 to 0000000000005462
   DW_CFA_def_cfa_register: r6 (rbp)
-  DW_CFA_advance_loc: 26 to 0000000000005f3f
+  DW_CFA_advance_loc: 26 to 000000000000547c
   DW_CFA_def_cfa: r7 (rsp) ofs 8
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000780 000000000000001c 00000784 FDE cie=00000000 pc=0000000000005f40..0000000000005f96
-  DW_CFA_advance_loc: 5 to 0000000000005f45
+00000768 000000000000001c 0000076c FDE cie=00000000 pc=000000000000547d..00000000000054cf
+  DW_CFA_advance_loc: 1 to 000000000000547e
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r6 (rbp) at cfa-16
-  DW_CFA_advance_loc: 3 to 0000000000005f48
+  DW_CFA_advance_loc: 3 to 0000000000005481
   DW_CFA_def_cfa_register: r6 (rbp)
-  DW_CFA_advance_loc1: 77 to 0000000000005f95
+  DW_CFA_advance_loc1: 77 to 00000000000054ce
   DW_CFA_def_cfa: r7 (rsp) ofs 8
   DW_CFA_nop
   DW_CFA_nop
 
-000007a0 000000000000001c 000007a4 FDE cie=00000000 pc=0000000000005f96..0000000000006123
-  DW_CFA_advance_loc: 5 to 0000000000005f9b
+00000788 000000000000001c 0000078c FDE cie=00000000 pc=00000000000054cf..0000000000005658
+  DW_CFA_advance_loc: 1 to 00000000000054d0
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r6 (rbp) at cfa-16
-  DW_CFA_advance_loc: 3 to 0000000000005f9e
+  DW_CFA_advance_loc: 3 to 00000000000054d3
   DW_CFA_def_cfa_register: r6 (rbp)
-  DW_CFA_advance_loc2: 388 to 0000000000006122
+  DW_CFA_advance_loc2: 388 to 0000000000005657
   DW_CFA_def_cfa: r7 (rsp) ofs 8
   DW_CFA_nop
 
-000007c0 000000000000001c 000007c4 FDE cie=00000000 pc=0000000000006123..0000000000006323
-  DW_CFA_advance_loc: 5 to 0000000000006128
+000007a8 000000000000001c 000007ac FDE cie=00000000 pc=0000000000005658..0000000000005854
+  DW_CFA_advance_loc: 1 to 0000000000005659
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r6 (rbp) at cfa-16
-  DW_CFA_advance_loc: 3 to 000000000000612b
+  DW_CFA_advance_loc: 3 to 000000000000565c
   DW_CFA_def_cfa_register: r6 (rbp)
-  DW_CFA_advance_loc2: 503 to 0000000000006322
+  DW_CFA_advance_loc2: 503 to 0000000000005853
   DW_CFA_def_cfa: r7 (rsp) ofs 8
   DW_CFA_nop
 
-000007e0 000000000000001c 000007e4 FDE cie=00000000 pc=0000000000006323..0000000000006389
-  DW_CFA_advance_loc: 5 to 0000000000006328
+000007c8 000000000000001c 000007cc FDE cie=00000000 pc=0000000000005854..00000000000058b6
+  DW_CFA_advance_loc: 1 to 0000000000005855
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r6 (rbp) at cfa-16
-  DW_CFA_advance_loc: 3 to 000000000000632b
+  DW_CFA_advance_loc: 3 to 0000000000005858
   DW_CFA_def_cfa_register: r6 (rbp)
-  DW_CFA_advance_loc1: 93 to 0000000000006388
+  DW_CFA_advance_loc1: 93 to 00000000000058b5
   DW_CFA_def_cfa: r7 (rsp) ofs 8
   DW_CFA_nop
   DW_CFA_nop
 
-00000800 0000000000000020 00000804 FDE cie=00000000 pc=0000000000006389..000000000000666a
-  DW_CFA_advance_loc: 5 to 000000000000638e
+000007e8 0000000000000020 000007ec FDE cie=00000000 pc=00000000000058b6..0000000000005b97
+  DW_CFA_advance_loc: 1 to 00000000000058b7
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r6 (rbp) at cfa-16
-  DW_CFA_advance_loc: 3 to 0000000000006391
+  DW_CFA_advance_loc: 3 to 00000000000058ba
   DW_CFA_def_cfa_register: r6 (rbp)
-  DW_CFA_advance_loc: 8 to 0000000000006399
+  DW_CFA_advance_loc: 8 to 00000000000058c2
   DW_CFA_offset: r3 (rbx) at cfa-24
-  DW_CFA_advance_loc2: 720 to 0000000000006669
+  DW_CFA_advance_loc2: 724 to 0000000000005b96
   DW_CFA_def_cfa: r7 (rsp) ofs 8
   DW_CFA_nop
   DW_CFA_nop
 
-00000824 000000000000001c 00000828 FDE cie=00000000 pc=000000000000666a..0000000000006744
-  DW_CFA_advance_loc: 5 to 000000000000666f
+0000080c 000000000000001c 00000810 FDE cie=00000000 pc=0000000000005b97..0000000000005c79
+  DW_CFA_advance_loc: 1 to 0000000000005b98
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r6 (rbp) at cfa-16
-  DW_CFA_advance_loc: 3 to 0000000000006672
+  DW_CFA_advance_loc: 3 to 0000000000005b9b
   DW_CFA_def_cfa_register: r6 (rbp)
-  DW_CFA_advance_loc1: 209 to 0000000000006743
+  DW_CFA_advance_loc1: 221 to 0000000000005c78
   DW_CFA_def_cfa: r7 (rsp) ofs 8
   DW_CFA_nop
   DW_CFA_nop
 
-00000844 ZERO terminator
+0000082c ZERO terminator
```

#### strings --all --bytes=8 {}

```diff
@@ -60,31 +60,32 @@
 sgsim_init
 sgsim_run
 variogram
 sgsim_t_free
 Partition2d
 variance
 libc.so.6
+__bss_start
 uc_sgsim.so
 GLIBC_2.4
 GLIBC_2.2.5
 %s%s%%0%dd.txt
 Folder already exist!
 Failed to open the file
 %d	%.10f
 Number = %d
 ./Realizations/
 Realizations
 ./Realizations/Variogram/
 Variogram
-GCC: (Ubuntu 9.4.0-1ubuntu1~20.04.1) 9.4.0
+GCC: (Ubuntu 7.5.0-3ubuntu1~18.04) 7.5.0
 crtstuff.c
 deregister_tm_clones
 __do_global_dtors_aux
-completed.8061
+completed.7698
 __do_global_dtors_aux_fini_array_entry
 frame_dummy
 __frame_dummy_init_array_entry
 c_array.c
 c_array_mt.c
 cov_model.c
 estimation
@@ -98,15 +99,14 @@
 matrix_tools.c
 random_tools.c
 variogram_array
 sgsim_array
 _sampling
 sgsim_memory_free
 sort_tools.c
-quicksort2d.localalias
 variogram.c
 __FRAME_END__
 __dso_handle
 _DYNAMIC
 __GNU_EH_FRAME_HDR
 __TMC_END__
 _GLOBAL_OFFSET_TABLE_
@@ -160,14 +160,15 @@
 mt19937_init
 cmpfunc_float
 simple_kriging
 c_array_mean_float
 malloc@@GLIBC_2.2.5
 krige_memory_free
 c_array_var_float
+__bss_start
 variogram
 c_array_max_double
 c_array_min_long_long
 mt19937_get_int32_range
 sampling_state_init
 mt19937_get_double_range
 sgsim_init
@@ -181,23 +182,21 @@
 _ITM_registerTMCloneTable
 c_array_mean_double
 c_array_std_float
 c_array_max_long_long
 c_array_sum_double
 __cxa_finalize@@GLIBC_2.2.5
 .shstrtab
-.note.gnu.property
 .note.gnu.build-id
 .gnu.hash
 .gnu.version
 .gnu.version_r
 .rela.dyn
 .rela.plt
 .plt.got
-.plt.sec
 .eh_frame_hdr
 .eh_frame
 .init_array
 .fini_array
 .dynamic
 .got.plt
 .comment
```

#### readelf --wide --decompress --hex-dump=.gnu.hash {}

```diff
@@ -1,33 +1,42 @@
 
 Hex dump of section '.gnu.hash':
-  0x000002f0 25000000 19000000 08000000 09000000 %...............
-  0x00000300 10e08c22 91803852 09004848 10c20000 ..."..8R..HH....
-  0x00000310 bd501a05 81000cb2 00080008 01128218 .P..............
-  0x00000320 a0010000 04200800 10670c10 08000329 ..... ...g.....)
-  0x00000330 44301940 001a4718 9a406108 e0052005 D0.@..G..@a... .
-  0x00000340 19000000 00000000 1a000000 1c000000 ................
-  0x00000350 00000000 00000000 00000000 1f000000 ................
-  0x00000360 24000000 27000000 28000000 29000000 $...'...(...)...
-  0x00000370 2c000000 2d000000 31000000 32000000 ,...-...1...2...
-  0x00000380 37000000 39000000 3a000000 3e000000 7...9...:...>...
-  0x00000390 3f000000 41000000 42000000 44000000 ?...A...B...D...
-  0x000003a0 46000000 47000000 48000000 49000000 F...G...H...I...
-  0x000003b0 4a000000 4c000000 4e000000 52000000 J...L...N...R...
-  0x000003c0 53000000 54000000 00000000 55000000 S...T.......U...
-  0x000003d0 56000000 23e77c8f e8ad9f13 ed523622 V...#.|......R6"
-  0x000003e0 0efc3a64 8661bfcb 19728efc 80869b07 ..:d.a...r......
-  0x000003f0 34f806f2 0491cb78 26ae3cfe a9d740ac 4......x&.<...@.
-  0x00000400 8298f89e 2c0fda6c 79e3bb76 91293232 ....,..ly..v.)22
-  0x00000410 1da4accf 529b421c 44614063 8dbd42ad ....R.B.Da@c..B.
-  0x00000420 f54b86b6 a61cc108 d04bcb53 62fbf0d9 .K.......K.Sb...
-  0x00000430 8522afcf 49a556a6 2e1abd70 c483c4ed ."..I.V....p....
-  0x00000440 3248fb03 ced54cbf 81082768 f88766a6 2H....L...'h..f.
-  0x00000450 4bb922c1 4fa56b9e b230011b 42c81ce2 K.".O.k..0..B...
-  0x00000460 daeee89d 35a6ef83 cb781915 e06e6e8f ....5....x...nn.
-  0x00000470 e7751b56 3326666d 92a872c6 41269e7c .u.V3&fm..r.A&.|
-  0x00000480 8c795900 059e6eb0 5fb6b6ef bb859a85 .yY...n._.......
-  0x00000490 aded6b56 936569f2 bcc077d4 21e6ec38 ..kV.ei...w.!..8
-  0x000004a0 fa622b87 b163b564 bc64c1e5 9a7eccea .b+..c.d.d...~..
-  0x000004b0 da2bd0ec e70f0566 575ed140 7b11a928 .+.....fW^.@{..(
-  0x000004c0 bd728bf5 938ebb25 695c2210          .r.....%i\".
+  0x000001f0 43000000 19000000 08000000 09000000 C...............
+  0x00000200 10e08c22 91803852 09004848 10c20000 ..."..8R..HH....
+  0x00000210 bd501a05 81000cb2 00080008 01128218 .P..............
+  0x00000220 a0010000 04200800 18670c10 0c000329 ..... ...g.....)
+  0x00000230 44301940 001a4719 9a406109 e0072005 D0.@..G..@a... .
+  0x00000240 19000000 1a000000 1b000000 00000000 ................
+  0x00000250 1c000000 1e000000 20000000 00000000 ........ .......
+  0x00000260 00000000 00000000 00000000 00000000 ................
+  0x00000270 22000000 00000000 25000000 00000000 ".......%.......
+  0x00000280 26000000 27000000 29000000 00000000 &...'...).......
+  0x00000290 2a000000 2b000000 00000000 2c000000 *...+.......,...
+  0x000002a0 00000000 2e000000 30000000 31000000 ........0...1...
+  0x000002b0 00000000 32000000 33000000 00000000 ....2...3.......
+  0x000002c0 34000000 37000000 38000000 3b000000 4...7...8...;...
+  0x000002d0 00000000 3c000000 00000000 3e000000 ....<.......>...
+  0x000002e0 3f000000 00000000 40000000 41000000 ?.......@...A...
+  0x000002f0 42000000 00000000 44000000 45000000 B.......D...E...
+  0x00000300 47000000 00000000 48000000 00000000 G.......H.......
+  0x00000310 00000000 00000000 4b000000 4d000000 ........K...M...
+  0x00000320 4f000000 00000000 51000000 52000000 O.......Q...R...
+  0x00000330 00000000 53000000 54000000 55000000 ....S...T...U...
+  0x00000340 56000000 5a000000 5b000000 ed523622 V...Z...[....R6"
+  0x00000350 575ed140 81082768 aced6b56 49a556a6 W^.@..'h..kVI.V.
+  0x00000360 9a7eccea dbeee89d 2c0fda6c 35a6ef83 .~......,..l5...
+  0x00000370 e8ad9f13 529b421c cfd54cbf 21e6ec38 ....R.B...L.!..8
+  0x00000380 c583c4ed f44b86b6 8dbd42ad 8522afcf .....K....B.."..
+  0x00000390 ebd3ef0e d14bcb53 bc728bf5 936569f2 .....K.S.r...ei.
+  0x000003a0 7a11a928 4bb922c1 b98df10e 938ebb25 z..(K."........%
+  0x000003b0 f98766a6 27ae3cfe bcc077d4 e6751b56 ..f.'.<...w..u.V
+  0x000003c0 0591cb78 93a872c6 80869b07 685c2210 ...x..r.....h\".
+  0x000003d0 a9d740ac 23e77c8f bc64c1e5 8761bfcb ..@.#.|..d...a..
+  0x000003e0 43c81ce2 4fa56b9e 0ffc3a64 41269e7c C...O.k...:dA&.|
+  0x000003f0 2e1abd70 cb781915 63fbf0d9 8c795900 ...p.x..c....yY.
+  0x00000400 79e3bb76 91293232 ba859a85 4245d5ec y..v.)22....BE..
+  0x00000410 8398f89e 18728efc b163b564 fa622b87 .....r...c.d.b+.
+  0x00000420 e70f0566 34f806f2 bbe3927c b330011b ...f4......|.0..
+  0x00000430 45614063 5fb6b6ef db2bd0ec e16e6e8f Ea@c_....+...nn.
+  0x00000440 a61cc108 3226666d 3248fb03 059e6eb0 ....2&fm2H....n.
+  0x00000450 d971581c 1da4accf                   .qX.....
```

#### readelf --wide --decompress --hex-dump=.dynstr {}

```diff
@@ -1,81 +1,83 @@
 
 Hex dump of section '.dynstr':
   0x00000cf8 005f5f67 6d6f6e5f 73746172 745f5f00 .__gmon_start__.
-  0x00000d08 5f49544d 5f646572 65676973 74657254 _ITM_deregisterT
-  0x00000d18 4d436c6f 6e655461 626c6500 5f49544d MCloneTable._ITM
-  0x00000d28 5f726567 69737465 72544d43 6c6f6e65 _registerTMClone
-  0x00000d38 5461626c 65005f5f 6378615f 66696e61 Table.__cxa_fina
-  0x00000d48 6c697a65 00635f61 72726179 5f6d6178 lize.c_array_max
-  0x00000d58 5f696e74 00635f61 72726179 5f6d6178 _int.c_array_max
-  0x00000d68 5f6c6f6e 675f6c6f 6e670063 5f617272 _long_long.c_arr
-  0x00000d78 61795f6d 61785f66 6c6f6174 00635f61 ay_max_float.c_a
-  0x00000d88 72726179 5f6d6178 5f646f75 626c6500 rray_max_double.
-  0x00000d98 635f6172 7261795f 6d696e5f 696e7400 c_array_min_int.
-  0x00000da8 635f6172 7261795f 6d696e5f 6c6f6e67 c_array_min_long
-  0x00000db8 5f6c6f6e 6700635f 61727261 795f6d69 _long.c_array_mi
-  0x00000dc8 6e5f666c 6f617400 635f6172 7261795f n_float.c_array_
-  0x00000dd8 6d696e5f 646f7562 6c650063 5f617272 min_double.c_arr
-  0x00000de8 61795f76 61725f69 6e740070 6f770063 ay_var_int.pow.c
-  0x00000df8 5f617272 61795f76 61725f6c 6f6e675f _array_var_long_
-  0x00000e08 6c6f6e67 00635f61 72726179 5f766172 long.c_array_var
-  0x00000e18 5f666c6f 61740063 5f617272 61795f76 _float.c_array_v
-  0x00000e28 61725f64 6f75626c 6500635f 61727261 ar_double.c_arra
-  0x00000e38 795f7374 645f696e 74007371 72740063 y_std_int.sqrt.c
-  0x00000e48 5f617272 61795f73 74645f6c 6f6e675f _array_std_long_
-  0x00000e58 6c6f6e67 00635f61 72726179 5f737464 long.c_array_std
-  0x00000e68 5f666c6f 61740063 5f617272 61795f73 _float.c_array_s
-  0x00000e78 74645f64 6f75626c 6500635f 61727261 td_double.c_arra
-  0x00000e88 795f6d65 616e5f69 6e740063 5f617272 y_mean_int.c_arr
-  0x00000e98 61795f6d 65616e5f 6c6f6e67 5f6c6f6e ay_mean_long_lon
-  0x00000ea8 6700635f 61727261 795f6d65 616e5f66 g.c_array_mean_f
-  0x00000eb8 6c6f6174 00635f61 72726179 5f6d6561 loat.c_array_mea
-  0x00000ec8 6e5f646f 75626c65 00635f61 72726179 n_double.c_array
-  0x00000ed8 5f73756d 5f696e74 00635f61 72726179 _sum_int.c_array
-  0x00000ee8 5f73756d 5f6c6f6e 6700635f 61727261 _sum_long.c_arra
-  0x00000ef8 795f7375 6d5f666c 6f617400 635f6172 y_sum_float.c_ar
-  0x00000f08 7261795f 73756d5f 646f7562 6c650063 ray_sum_double.c
-  0x00000f18 6d706675 6e635f69 6e740063 6d706675 mpfunc_int.cmpfu
-  0x00000f28 6e635f6c 6f6e6700 636d7066 756e635f nc_long.cmpfunc_
-  0x00000f38 666c6f61 7400636d 7066756e 635f646f float.cmpfunc_do
-  0x00000f48 75626c65 006d7431 39393337 5f696e69 uble.mt19937_ini
-  0x00000f58 74006d74 31393933 375f6765 6e657261 t.mt19937_genera
-  0x00000f68 7465006d 74313939 33375f67 65745f69 te.mt19937_get_i
-  0x00000f78 6e743332 5f72616e 6765006d 74313939 nt32_range.mt199
-  0x00000f88 33375f67 65745f66 6c6f6174 006d7431 37_get_float.mt1
-  0x00000f98 39393337 5f676574 5f666c6f 61745f72 9937_get_float_r
-  0x00000fa8 616e6765 006d7431 39393337 5f676574 ange.mt19937_get
-  0x00000fb8 5f646f75 626c6500 6d743139 3933375f _double.mt19937_
-  0x00000fc8 6765745f 646f7562 6c655f72 616e6765 get_double_range
-  0x00000fd8 006d7431 39393337 5f72616e 646f6d5f .mt19937_random_
-  0x00000fe8 6e6f726d 616c006c 6f670063 6f730063 normal.log.cos.c
-  0x00000ff8 6f765f6d 6f64656c 5f696e69 7400636f ov_model_init.co
-  0x00001008 765f6d6f 64656c00 65787000 636f765f v_model.exp.cov_
-  0x00001018 6d6f6465 6c326400 73616d70 6c696e67 model2d.sampling
-  0x00001028 5f737461 74655f69 6e697400 63616c6c _state_init.call
-  0x00001038 6f630073 616d706c 696e675f 73746174 oc.sampling_stat
-  0x00001048 655f7570 64617465 006b7269 67655f70 e_update.krige_p
-  0x00001058 6172616d 5f736574 74696e67 006d616c aram_setting.mal
-  0x00001068 6c6f6300 73696d70 6c655f6b 72696769 loc.simple_krigi
-  0x00001078 6e670066 696e645f 6e656967 68626f72 ng.find_neighbor
-  0x00001088 00717569 636b736f 72743264 00706469 .quicksort2d.pdi
-  0x00001098 7374006d 61747269 78666f72 6d006c75 st.matrixform.lu
-  0x000010a8 5f696e76 65727365 5f736f6c 76657200 _inverse_solver.
-  0x000010b8 6b726967 655f6d65 6d6f7279 5f667265 krige_memory_fre
-  0x000010c8 65006c75 5f646563 6f6d706f 73697469 e.lu_decompositi
-  0x000010d8 6f6e005f 5f737461 636b5f63 686b5f66 on.__stack_chk_f
-  0x000010e8 61696c00 645f6172 616e6765 00736176 ail.d_arange.sav
-  0x000010f8 655f3164 61727261 79006c6f 67313000 e_1darray.log10.
-  0x00001108 6365696c 00736e70 72696e74 66006d6b ceil.snprintf.mk
-  0x00001118 64697200 5f5f6572 726e6f5f 6c6f6361 dir.__errno_loca
-  0x00001128 74696f6e 00666f70 656e0070 6572726f tion.fopen.perro
-  0x00001138 72006578 69740066 7072696e 74660066 r.exit.fprintf.f
-  0x00001148 636c6f73 65007261 6e646f6d 70617468 close.randompath
-  0x00001158 00736773 696d5f69 6e697400 73677369 .sgsim_init.sgsi
-  0x00001168 6d5f7275 6e007661 72696f67 72616d00 m_run.variogram.
-  0x00001178 73677369 6d5f745f 66726565 00737761 sgsim_t_free.swa
-  0x00001188 70005061 72746974 696f6e32 64007661 p.Partition2d.va
-  0x00001198 7269616e 6365006c 6962632e 736f2e36 riance.libc.so.6
-  0x000011a8 0075635f 73677369 6d2e736f 00474c49 .uc_sgsim.so.GLI
-  0x000011b8 42435f32 2e340047 4c494243 5f322e32 BC_2.4.GLIBC_2.2
-  0x000011c8 2e3500                              .5.
+  0x00000d08 5f66696e 69005f49 544d5f64 65726567 _fini._ITM_dereg
+  0x00000d18 69737465 72544d43 6c6f6e65 5461626c isterTMCloneTabl
+  0x00000d28 65005f49 544d5f72 65676973 74657254 e._ITM_registerT
+  0x00000d38 4d436c6f 6e655461 626c6500 5f5f6378 MCloneTable.__cx
+  0x00000d48 615f6669 6e616c69 7a650063 5f617272 a_finalize.c_arr
+  0x00000d58 61795f6d 61785f69 6e740063 5f617272 ay_max_int.c_arr
+  0x00000d68 61795f6d 61785f6c 6f6e675f 6c6f6e67 ay_max_long_long
+  0x00000d78 00635f61 72726179 5f6d6178 5f666c6f .c_array_max_flo
+  0x00000d88 61740063 5f617272 61795f6d 61785f64 at.c_array_max_d
+  0x00000d98 6f75626c 6500635f 61727261 795f6d69 ouble.c_array_mi
+  0x00000da8 6e5f696e 7400635f 61727261 795f6d69 n_int.c_array_mi
+  0x00000db8 6e5f6c6f 6e675f6c 6f6e6700 635f6172 n_long_long.c_ar
+  0x00000dc8 7261795f 6d696e5f 666c6f61 7400635f ray_min_float.c_
+  0x00000dd8 61727261 795f6d69 6e5f646f 75626c65 array_min_double
+  0x00000de8 00635f61 72726179 5f766172 5f696e74 .c_array_var_int
+  0x00000df8 00706f77 00635f61 72726179 5f766172 .pow.c_array_var
+  0x00000e08 5f6c6f6e 675f6c6f 6e670063 5f617272 _long_long.c_arr
+  0x00000e18 61795f76 61725f66 6c6f6174 00635f61 ay_var_float.c_a
+  0x00000e28 72726179 5f766172 5f646f75 626c6500 rray_var_double.
+  0x00000e38 635f6172 7261795f 7374645f 696e7400 c_array_std_int.
+  0x00000e48 73717274 00635f61 72726179 5f737464 sqrt.c_array_std
+  0x00000e58 5f6c6f6e 675f6c6f 6e670063 5f617272 _long_long.c_arr
+  0x00000e68 61795f73 74645f66 6c6f6174 00635f61 ay_std_float.c_a
+  0x00000e78 72726179 5f737464 5f646f75 626c6500 rray_std_double.
+  0x00000e88 635f6172 7261795f 6d65616e 5f696e74 c_array_mean_int
+  0x00000e98 00635f61 72726179 5f6d6561 6e5f6c6f .c_array_mean_lo
+  0x00000ea8 6e675f6c 6f6e6700 635f6172 7261795f ng_long.c_array_
+  0x00000eb8 6d65616e 5f666c6f 61740063 5f617272 mean_float.c_arr
+  0x00000ec8 61795f6d 65616e5f 646f7562 6c650063 ay_mean_double.c
+  0x00000ed8 5f617272 61795f73 756d5f69 6e740063 _array_sum_int.c
+  0x00000ee8 5f617272 61795f73 756d5f6c 6f6e6700 _array_sum_long.
+  0x00000ef8 635f6172 7261795f 73756d5f 666c6f61 c_array_sum_floa
+  0x00000f08 7400635f 61727261 795f7375 6d5f646f t.c_array_sum_do
+  0x00000f18 75626c65 00636d70 66756e63 5f696e74 uble.cmpfunc_int
+  0x00000f28 00636d70 66756e63 5f6c6f6e 6700636d .cmpfunc_long.cm
+  0x00000f38 7066756e 635f666c 6f617400 636d7066 pfunc_float.cmpf
+  0x00000f48 756e635f 646f7562 6c65006d 74313939 unc_double.mt199
+  0x00000f58 33375f69 6e697400 6d743139 3933375f 37_init.mt19937_
+  0x00000f68 67656e65 72617465 006d7431 39393337 generate.mt19937
+  0x00000f78 5f676574 5f696e74 33325f72 616e6765 _get_int32_range
+  0x00000f88 006d7431 39393337 5f676574 5f666c6f .mt19937_get_flo
+  0x00000f98 6174006d 74313939 33375f67 65745f66 at.mt19937_get_f
+  0x00000fa8 6c6f6174 5f72616e 6765006d 74313939 loat_range.mt199
+  0x00000fb8 33375f67 65745f64 6f75626c 65006d74 37_get_double.mt
+  0x00000fc8 31393933 375f6765 745f646f 75626c65 19937_get_double
+  0x00000fd8 5f72616e 6765006d 74313939 33375f72 _range.mt19937_r
+  0x00000fe8 616e646f 6d5f6e6f 726d616c 006c6f67 andom_normal.log
+  0x00000ff8 00636f73 00636f76 5f6d6f64 656c5f69 .cos.cov_model_i
+  0x00001008 6e697400 636f765f 6d6f6465 6c006578 nit.cov_model.ex
+  0x00001018 7000636f 765f6d6f 64656c32 64007361 p.cov_model2d.sa
+  0x00001028 6d706c69 6e675f73 74617465 5f696e69 mpling_state_ini
+  0x00001038 74006361 6c6c6f63 0073616d 706c696e t.calloc.samplin
+  0x00001048 675f7374 6174655f 75706461 7465006b g_state_update.k
+  0x00001058 72696765 5f706172 616d5f73 65747469 rige_param_setti
+  0x00001068 6e67006d 616c6c6f 63007369 6d706c65 ng.malloc.simple
+  0x00001078 5f6b7269 67696e67 0066696e 645f6e65 _kriging.find_ne
+  0x00001088 69676862 6f720071 7569636b 736f7274 ighbor.quicksort
+  0x00001098 32640070 64697374 006d6174 72697866 2d.pdist.matrixf
+  0x000010a8 6f726d00 6c755f69 6e766572 73655f73 orm.lu_inverse_s
+  0x000010b8 6f6c7665 72006b72 6967655f 6d656d6f olver.krige_memo
+  0x000010c8 72795f66 72656500 6c755f64 65636f6d ry_free.lu_decom
+  0x000010d8 706f7369 74696f6e 005f5f73 7461636b position.__stack
+  0x000010e8 5f63686b 5f666169 6c00645f 6172616e _chk_fail.d_aran
+  0x000010f8 67650073 6176655f 31646172 72617900 ge.save_1darray.
+  0x00001108 6c6f6731 30006365 696c0073 6e707269 log10.ceil.snpri
+  0x00001118 6e746600 6d6b6469 72005f5f 6572726e ntf.mkdir.__errn
+  0x00001128 6f5f6c6f 63617469 6f6e0066 6f70656e o_location.fopen
+  0x00001138 00706572 726f7200 65786974 00667072 .perror.exit.fpr
+  0x00001148 696e7466 0066636c 6f736500 72616e64 intf.fclose.rand
+  0x00001158 6f6d7061 74680073 6773696d 5f696e69 ompath.sgsim_ini
+  0x00001168 74007367 73696d5f 72756e00 76617269 t.sgsim_run.vari
+  0x00001178 6f677261 6d007367 73696d5f 745f6672 ogram.sgsim_t_fr
+  0x00001188 65650073 77617000 50617274 6974696f ee.swap.Partitio
+  0x00001198 6e326400 76617269 616e6365 006c6962 n2d.variance.lib
+  0x000011a8 632e736f 2e36005f 65646174 61005f5f c.so.6._edata.__
+  0x000011b8 6273735f 73746172 74005f65 6e640075 bss_start._end.u
+  0x000011c8 635f7367 73696d2e 736f0047 4c494243 c_sgsim.so.GLIBC
+  0x000011d8 5f322e34 00474c49 42435f32 2e322e35 _2.4.GLIBC_2.2.5
+  0x000011e8 00                                  .
```

#### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.init {}

```diff
@@ -1,15 +1,14 @@
 
 
 
 Disassembly of section .init:
 
-0000000000002000 <_init>:
+00000000000017a0 <_init>:
 _init():
-	endbr64
 	sub    $0x8,%rsp
-	mov    0x6fd9(%rip),%rax        
+	mov    0x20583d(%rip),%rax        
 	test   %rax,%rax
-	je     2016 <_init+0x16>
+	je     17b2 <_init+0x12>
 	call   *%rax
 	add    $0x8,%rsp
 	ret
```

#### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.plt {}

```diff
@@ -1,185 +1,229 @@
 
 
 
 Disassembly of section .plt:
 
-0000000000002020 <.plt>:
-	push   0x6fe2(%rip)        
-	bnd jmp *0x6fe3(%rip)        
-	nopl   (%rax)
-	endbr64
+00000000000017c0 <.plt>:
+	push   0x205842(%rip)        
+	jmp    *0x205844(%rip)        
+	nopl   0x0(%rax)
+
+00000000000017d0 <free@plt>:
+	jmp    *0x205842(%rip)        
 	push   $0x0
-	bnd jmp 2020 <.plt>
-	nop
-	endbr64
+	jmp    17c0 <.plt>
+
+00000000000017e0 <__errno_location@plt>:
+	jmp    *0x20583a(%rip)        
 	push   $0x1
-	bnd jmp 2020 <.plt>
-	nop
-	endbr64
+	jmp    17c0 <.plt>
+
+00000000000017f0 <quicksort2d@plt>:
+	jmp    *0x205832(%rip)        
 	push   $0x2
-	bnd jmp 2020 <.plt>
-	nop
-	endbr64
+	jmp    17c0 <.plt>
+
+0000000000001800 <mkdir@plt>:
+	jmp    *0x20582a(%rip)        
 	push   $0x3
-	bnd jmp 2020 <.plt>
-	nop
-	endbr64
+	jmp    17c0 <.plt>
+
+0000000000001810 <randompath@plt>:
+	jmp    *0x205822(%rip)        
 	push   $0x4
-	bnd jmp 2020 <.plt>
-	nop
-	endbr64
+	jmp    17c0 <.plt>
+
+0000000000001820 <ceil@plt>:
+	jmp    *0x20581a(%rip)        
 	push   $0x5
-	bnd jmp 2020 <.plt>
-	nop
-	endbr64
+	jmp    17c0 <.plt>
+
+0000000000001830 <lu_inverse_solver@plt>:
+	jmp    *0x205812(%rip)        
 	push   $0x6
-	bnd jmp 2020 <.plt>
-	nop
-	endbr64
+	jmp    17c0 <.plt>
+
+0000000000001840 <sampling_state_update@plt>:
+	jmp    *0x20580a(%rip)        
 	push   $0x7
-	bnd jmp 2020 <.plt>
-	nop
-	endbr64
+	jmp    17c0 <.plt>
+
+0000000000001850 <fclose@plt>:
+	jmp    *0x205802(%rip)        
 	push   $0x8
-	bnd jmp 2020 <.plt>
-	nop
-	endbr64
+	jmp    17c0 <.plt>
+
+0000000000001860 <__stack_chk_fail@plt>:
+	jmp    *0x2057fa(%rip)        
 	push   $0x9
-	bnd jmp 2020 <.plt>
-	nop
-	endbr64
+	jmp    17c0 <.plt>
+
+0000000000001870 <save_1darray@plt>:
+	jmp    *0x2057f2(%rip)        
 	push   $0xa
-	bnd jmp 2020 <.plt>
-	nop
-	endbr64
+	jmp    17c0 <.plt>
+
+0000000000001880 <cov_model2d@plt>:
+	jmp    *0x2057ea(%rip)        
 	push   $0xb
-	bnd jmp 2020 <.plt>
-	nop
-	endbr64
+	jmp    17c0 <.plt>
+
+0000000000001890 <printf@plt>:
+	jmp    *0x2057e2(%rip)        
 	push   $0xc
-	bnd jmp 2020 <.plt>
-	nop
-	endbr64
+	jmp    17c0 <.plt>
+
+00000000000018a0 <find_neighbor@plt>:
+	jmp    *0x2057da(%rip)        
 	push   $0xd
-	bnd jmp 2020 <.plt>
-	nop
-	endbr64
+	jmp    17c0 <.plt>
+
+00000000000018b0 <snprintf@plt>:
+	jmp    *0x2057d2(%rip)        
 	push   $0xe
-	bnd jmp 2020 <.plt>
-	nop
-	endbr64
+	jmp    17c0 <.plt>
+
+00000000000018c0 <lu_decomposition@plt>:
+	jmp    *0x2057ca(%rip)        
 	push   $0xf
-	bnd jmp 2020 <.plt>
-	nop
-	endbr64
+	jmp    17c0 <.plt>
+
+00000000000018d0 <d_arange@plt>:
+	jmp    *0x2057c2(%rip)        
 	push   $0x10
-	bnd jmp 2020 <.plt>
-	nop
-	endbr64
+	jmp    17c0 <.plt>
+
+00000000000018e0 <Partition2d@plt>:
+	jmp    *0x2057ba(%rip)        
 	push   $0x11
-	bnd jmp 2020 <.plt>
-	nop
-	endbr64
+	jmp    17c0 <.plt>
+
+00000000000018f0 <cov_model@plt>:
+	jmp    *0x2057b2(%rip)        
 	push   $0x12
-	bnd jmp 2020 <.plt>
-	nop
-	endbr64
+	jmp    17c0 <.plt>
+
+0000000000001900 <matrixform@plt>:
+	jmp    *0x2057aa(%rip)        
 	push   $0x13
-	bnd jmp 2020 <.plt>
-	nop
-	endbr64
+	jmp    17c0 <.plt>
+
+0000000000001910 <mt19937_generate@plt>:
+	jmp    *0x2057a2(%rip)        
 	push   $0x14
-	bnd jmp 2020 <.plt>
-	nop
-	endbr64
+	jmp    17c0 <.plt>
+
+0000000000001920 <mt19937_random_normal@plt>:
+	jmp    *0x20579a(%rip)        
 	push   $0x15
-	bnd jmp 2020 <.plt>
-	nop
-	endbr64
+	jmp    17c0 <.plt>
+
+0000000000001930 <calloc@plt>:
+	jmp    *0x205792(%rip)        
 	push   $0x16
-	bnd jmp 2020 <.plt>
-	nop
-	endbr64
+	jmp    17c0 <.plt>
+
+0000000000001940 <fprintf@plt>:
+	jmp    *0x20578a(%rip)        
 	push   $0x17
-	bnd jmp 2020 <.plt>
-	nop
-	endbr64
+	jmp    17c0 <.plt>
+
+0000000000001950 <krige_param_setting@plt>:
+	jmp    *0x205782(%rip)        
 	push   $0x18
-	bnd jmp 2020 <.plt>
-	nop
-	endbr64
+	jmp    17c0 <.plt>
+
+0000000000001960 <mt19937_init@plt>:
+	jmp    *0x20577a(%rip)        
 	push   $0x19
-	bnd jmp 2020 <.plt>
-	nop
-	endbr64
+	jmp    17c0 <.plt>
+
+0000000000001970 <simple_kriging@plt>:
+	jmp    *0x205772(%rip)        
 	push   $0x1a
-	bnd jmp 2020 <.plt>
-	nop
-	endbr64
+	jmp    17c0 <.plt>
+
+0000000000001980 <malloc@plt>:
+	jmp    *0x20576a(%rip)        
 	push   $0x1b
-	bnd jmp 2020 <.plt>
-	nop
-	endbr64
+	jmp    17c0 <.plt>
+
+0000000000001990 <arange@plt>:
+	jmp    *0x205762(%rip)        
 	push   $0x1c
-	bnd jmp 2020 <.plt>
-	nop
-	endbr64
+	jmp    17c0 <.plt>
+
+00000000000019a0 <krige_memory_free@plt>:
+	jmp    *0x20575a(%rip)        
 	push   $0x1d
-	bnd jmp 2020 <.plt>
-	nop
-	endbr64
+	jmp    17c0 <.plt>
+
+00000000000019b0 <exp@plt>:
+	jmp    *0x205752(%rip)        
 	push   $0x1e
-	bnd jmp 2020 <.plt>
-	nop
-	endbr64
+	jmp    17c0 <.plt>
+
+00000000000019c0 <variogram@plt>:
+	jmp    *0x20574a(%rip)        
 	push   $0x1f
-	bnd jmp 2020 <.plt>
-	nop
-	endbr64
+	jmp    17c0 <.plt>
+
+00000000000019d0 <cos@plt>:
+	jmp    *0x205742(%rip)        
 	push   $0x20
-	bnd jmp 2020 <.plt>
-	nop
-	endbr64
+	jmp    17c0 <.plt>
+
+00000000000019e0 <sampling_state_init@plt>:
+	jmp    *0x20573a(%rip)        
 	push   $0x21
-	bnd jmp 2020 <.plt>
-	nop
-	endbr64
+	jmp    17c0 <.plt>
+
+00000000000019f0 <log@plt>:
+	jmp    *0x205732(%rip)        
 	push   $0x22
-	bnd jmp 2020 <.plt>
-	nop
-	endbr64
+	jmp    17c0 <.plt>
+
+0000000000001a00 <fopen@plt>:
+	jmp    *0x20572a(%rip)        
 	push   $0x23
-	bnd jmp 2020 <.plt>
-	nop
-	endbr64
+	jmp    17c0 <.plt>
+
+0000000000001a10 <mt19937_get_double@plt>:
+	jmp    *0x205722(%rip)        
 	push   $0x24
-	bnd jmp 2020 <.plt>
-	nop
-	endbr64
+	jmp    17c0 <.plt>
+
+0000000000001a20 <pow@plt>:
+	jmp    *0x20571a(%rip)        
 	push   $0x25
-	bnd jmp 2020 <.plt>
-	nop
-	endbr64
+	jmp    17c0 <.plt>
+
+0000000000001a30 <perror@plt>:
+	jmp    *0x205712(%rip)        
 	push   $0x26
-	bnd jmp 2020 <.plt>
-	nop
-	endbr64
+	jmp    17c0 <.plt>
+
+0000000000001a40 <log10@plt>:
+	jmp    *0x20570a(%rip)        
 	push   $0x27
-	bnd jmp 2020 <.plt>
-	nop
-	endbr64
+	jmp    17c0 <.plt>
+
+0000000000001a50 <sqrt@plt>:
+	jmp    *0x205702(%rip)        
 	push   $0x28
-	bnd jmp 2020 <.plt>
-	nop
-	endbr64
+	jmp    17c0 <.plt>
+
+0000000000001a60 <pdist@plt>:
+	jmp    *0x2056fa(%rip)        
 	push   $0x29
-	bnd jmp 2020 <.plt>
-	nop
-	endbr64
+	jmp    17c0 <.plt>
+
+0000000000001a70 <exit@plt>:
+	jmp    *0x2056f2(%rip)        
 	push   $0x2a
-	bnd jmp 2020 <.plt>
-	nop
-	endbr64
+	jmp    17c0 <.plt>
+
+0000000000001a80 <swap@plt>:
+	jmp    *0x2056ea(%rip)        
 	push   $0x2b
-	bnd jmp 2020 <.plt>
-	nop
+	jmp    17c0 <.plt>
```

#### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.plt.got {}

```diff
@@ -1,9 +1,8 @@
 
 
 
 Disassembly of section .plt.got:
 
-00000000000022f0 <__cxa_finalize@plt>:
-	endbr64
-	bnd jmp *0x6cfd(%rip)        
-	nopl   0x0(%rax,%rax,1)
+0000000000001a90 <__cxa_finalize@plt>:
+	jmp    *0x205562(%rip)        
+	xchg   %ax,%ax
```

#### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.text {}

```diff
@@ -1,107 +1,117 @@
 
 
 
 Disassembly of section .text:
 
-00000000000025c0 <deregister_tm_clones>:
+0000000000001aa0 <deregister_tm_clones>:
 deregister_tm_clones():
-	lea    0x6bb9(%rip),%rdi        
-	lea    0x6bb2(%rip),%rax        
+	lea    0x2056d9(%rip),%rdi        
+	push   %rbp
+	lea    0x2056d1(%rip),%rax        
 	cmp    %rdi,%rax
-	je     25e8 <deregister_tm_clones+0x28>
-	mov    0x6a06(%rip),%rax        
+	mov    %rsp,%rbp
+	je     1ad0 <deregister_tm_clones+0x30>
+	mov    0x205522(%rip),%rax        
 	test   %rax,%rax
-	je     25e8 <deregister_tm_clones+0x28>
+	je     1ad0 <deregister_tm_clones+0x30>
+	pop    %rbp
 	jmp    *%rax
-	nopl   0x0(%rax)
+	cs nopw 0x0(%rax,%rax,1)
+	pop    %rbp
 	ret
 	nopl   0x0(%rax)
+	cs nopw 0x0(%rax,%rax,1)
 
-00000000000025f0 <register_tm_clones>:
+0000000000001ae0 <register_tm_clones>:
 register_tm_clones():
-	lea    0x6b89(%rip),%rdi        
-	lea    0x6b82(%rip),%rsi        
+	lea    0x205699(%rip),%rdi        
+	lea    0x205692(%rip),%rsi        
+	push   %rbp
 	sub    %rdi,%rsi
+	mov    %rsp,%rbp
+	sar    $0x3,%rsi
 	mov    %rsi,%rax
-	shr    $0x3f,%rsi
-	sar    $0x3,%rax
+	shr    $0x3f,%rax
 	add    %rax,%rsi
 	sar    %rsi
-	je     2628 <register_tm_clones+0x38>
-	mov    0x69d5(%rip),%rax        
+	je     1b20 <register_tm_clones+0x40>
+	mov    0x2054e1(%rip),%rax        
 	test   %rax,%rax
-	je     2628 <register_tm_clones+0x38>
+	je     1b20 <register_tm_clones+0x40>
+	pop    %rbp
 	jmp    *%rax
 	nopw   0x0(%rax,%rax,1)
+	pop    %rbp
 	ret
 	nopl   0x0(%rax)
+	cs nopw 0x0(%rax,%rax,1)
 
-0000000000002630 <__do_global_dtors_aux>:
+0000000000001b30 <__do_global_dtors_aux>:
 __do_global_dtors_aux():
-	endbr64
-	cmpb   $0x0,0x6b45(%rip)        
-	jne    2668 <__do_global_dtors_aux+0x38>
-	push   %rbp
-	cmpq   $0x0,0x69b2(%rip)        
-	mov    %rsp,%rbp
-	je     2657 <__do_global_dtors_aux+0x27>
-	mov    0x6b26(%rip),%rdi        
-	call   22f0 <__cxa_finalize@plt>
-	call   25c0 <deregister_tm_clones>
-	movb   $0x1,0x6b1d(%rip)        
+	cmpb   $0x0,0x205649(%rip)        
+	jne    1b68 <__do_global_dtors_aux+0x38>
+	cmpq   $0x0,0x2054b7(%rip)        
+	push   %rbp
+	mov    %rsp,%rbp
+	je     1b53 <__do_global_dtors_aux+0x23>
+	mov    0x20562a(%rip),%rdi        
+	call   1a90 <__cxa_finalize@plt>
+	call   1aa0 <deregister_tm_clones>
+	movb   $0x1,0x205621(%rip)        
 	pop    %rbp
 	ret
-	nopl   (%rax)
-	ret
 	nopl   0x0(%rax)
+	repz ret
+	nopw   0x0(%rax,%rax,1)
 
-0000000000002670 <frame_dummy>:
+0000000000001b70 <frame_dummy>:
 frame_dummy():
-	endbr64
-	jmp    25f0 <register_tm_clones>
+	push   %rbp
+	mov    %rsp,%rbp
+	pop    %rbp
+	jmp    1ae0 <register_tm_clones>
 
-0000000000002679 <c_array_max_int>:
+0000000000001b7a <c_array_max_int>:
 c_array_max_int():
-	endbr64
 	push   %rbp
 	mov    %rsp,%rbp
 	mov    %rdi,-0x28(%rbp)
 	mov    %esi,-0x2c(%rbp)
 	mov    -0x2c(%rbp),%eax
 	and    $0x1,%eax
 	mov    %eax,-0x4(%rbp)
 	movl   $0xff000000,-0x18(%rbp)
 	movl   $0xffffff,-0x14(%rbp)
 	cmpl   $0x0,-0x4(%rbp)
-	je     26a9 <c_array_max_int+0x30>
+	je     1ba6 <c_array_max_int+0x2c>
 	subl   $0x1,-0x2c(%rbp)
 	mov    -0x28(%rbp),%rax
 	mov    (%rax),%eax
 	mov    %eax,-0x10(%rbp)
 	mov    -0x28(%rbp),%rax
 	mov    (%rax),%eax
 	mov    %eax,-0xc(%rbp)
 	movl   $0x0,-0x8(%rbp)
-	jmp    2789 <c_array_max_int+0x110>
+	jmp    1c86 <c_array_max_int+0x10c>
 	mov    -0x8(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,4),%rdx
 	mov    -0x28(%rbp),%rax
 	add    %rdx,%rax
 	mov    (%rax),%edx
 	mov    -0x8(%rbp),%eax
 	cltq
 	add    $0x1,%rax
 	lea    0x0(,%rax,4),%rcx
 	mov    -0x28(%rbp),%rax
 	add    %rcx,%rax
 	mov    (%rax),%eax
 	cmp    %eax,%edx
-	jle    2733 <c_array_max_int+0xba>
+	jle    1c30 <c_array_max_int+0xb6>
 	mov    -0x8(%rbp),%eax
 	cltq
 	add    $0x1,%rax
 	lea    0x0(,%rax,4),%rdx
 	mov    -0x28(%rbp),%rax
 	add    %rdx,%rax
 	mov    (%rax),%eax
@@ -109,15 +119,15 @@
 	mov    -0x8(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,4),%rdx
 	mov    -0x28(%rbp),%rax
 	add    %rdx,%rax
 	mov    (%rax),%eax
 	mov    %eax,-0xc(%rbp)
-	jmp    2769 <c_array_max_int+0xf0>
+	jmp    1c66 <c_array_max_int+0xec>
 	mov    -0x8(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,4),%rdx
 	mov    -0x28(%rbp),%rax
 	add    %rdx,%rax
 	mov    (%rax),%eax
 	mov    %eax,-0x10(%rbp)
@@ -127,102 +137,101 @@
 	lea    0x0(,%rax,4),%rdx
 	mov    -0x28(%rbp),%rax
 	add    %rdx,%rax
 	mov    (%rax),%eax
 	mov    %eax,-0xc(%rbp)
 	mov    -0xc(%rbp),%eax
 	cmp    -0x18(%rbp),%eax
-	jle    2777 <c_array_max_int+0xfe>
+	jle    1c74 <c_array_max_int+0xfa>
 	mov    -0xc(%rbp),%eax
 	mov    %eax,-0x18(%rbp)
 	mov    -0x10(%rbp),%eax
 	cmp    -0x14(%rbp),%eax
-	jge    2785 <c_array_max_int+0x10c>
+	jge    1c82 <c_array_max_int+0x108>
 	mov    -0x10(%rbp),%eax
 	mov    %eax,-0x14(%rbp)
 	addl   $0x2,-0x8(%rbp)
 	mov    -0x8(%rbp),%eax
 	cmp    -0x2c(%rbp),%eax
-	jl     26c7 <c_array_max_int+0x4e>
+	jl     1bc4 <c_array_max_int+0x4a>
 	cmpl   $0x0,-0x4(%rbp)
-	je     2803 <c_array_max_int+0x18a>
+	je     1d00 <c_array_max_int+0x186>
 	mov    -0x2c(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,4),%rdx
 	mov    -0x28(%rbp),%rax
 	add    %rdx,%rax
 	mov    (%rax),%eax
 	cmp    %eax,-0x18(%rbp)
-	jge    27cf <c_array_max_int+0x156>
+	jge    1ccc <c_array_max_int+0x152>
 	mov    -0x2c(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,4),%rdx
 	mov    -0x28(%rbp),%rax
 	add    %rdx,%rax
 	mov    (%rax),%eax
 	mov    %eax,-0x18(%rbp)
 	mov    -0x2c(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,4),%rdx
 	mov    -0x28(%rbp),%rax
 	add    %rdx,%rax
 	mov    (%rax),%eax
 	cmp    %eax,-0x14(%rbp)
-	jle    2803 <c_array_max_int+0x18a>
+	jle    1d00 <c_array_max_int+0x186>
 	mov    -0x2c(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,4),%rdx
 	mov    -0x28(%rbp),%rax
 	add    %rdx,%rax
 	mov    (%rax),%eax
 	mov    %eax,-0x14(%rbp)
 	mov    -0x18(%rbp),%eax
 	pop    %rbp
 	ret
 
-0000000000002808 <c_array_max_long_long>:
+0000000000001d05 <c_array_max_long_long>:
 c_array_max_long_long():
-	endbr64
 	push   %rbp
 	mov    %rsp,%rbp
 	mov    %rdi,-0x38(%rbp)
 	mov    %esi,-0x3c(%rbp)
 	mov    -0x3c(%rbp),%eax
 	and    $0x1,%eax
 	mov    %eax,-0x24(%rbp)
 	movabs $0xff00000000000000,%rax
 	mov    %rax,-0x20(%rbp)
 	movabs $0x100000000000000,%rax
 	mov    %rax,-0x18(%rbp)
 	cmpl   $0x0,-0x24(%rbp)
-	je     2846 <c_array_max_long_long+0x3e>
+	je     1d3f <c_array_max_long_long+0x3a>
 	subl   $0x1,-0x3c(%rbp)
 	mov    -0x38(%rbp),%rax
 	mov    (%rax),%rax
 	mov    %rax,-0x10(%rbp)
 	mov    -0x38(%rbp),%rax
 	mov    (%rax),%rax
 	mov    %rax,-0x8(%rbp)
 	movl   $0x0,-0x28(%rbp)
-	jmp    293d <c_array_max_long_long+0x135>
+	jmp    1e36 <c_array_max_long_long+0x131>
 	mov    -0x28(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,8),%rdx
 	mov    -0x38(%rbp),%rax
 	add    %rdx,%rax
 	mov    (%rax),%rdx
 	mov    -0x28(%rbp),%eax
 	cltq
 	add    $0x1,%rax
 	lea    0x0(,%rax,8),%rcx
 	mov    -0x38(%rbp),%rax
 	add    %rcx,%rax
 	mov    (%rax),%rax
 	cmp    %rax,%rdx
-	jle    28db <c_array_max_long_long+0xd3>
+	jle    1dd4 <c_array_max_long_long+0xcf>
 	mov    -0x28(%rbp),%eax
 	cltq
 	add    $0x1,%rax
 	lea    0x0(,%rax,8),%rdx
 	mov    -0x38(%rbp),%rax
 	add    %rdx,%rax
 	mov    (%rax),%rax
@@ -230,15 +239,15 @@
 	mov    -0x28(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,8),%rdx
 	mov    -0x38(%rbp),%rax
 	add    %rdx,%rax
 	mov    (%rax),%rax
 	mov    %rax,-0x8(%rbp)
-	jmp    2915 <c_array_max_long_long+0x10d>
+	jmp    1e0e <c_array_max_long_long+0x109>
 	mov    -0x28(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,8),%rdx
 	mov    -0x38(%rbp),%rax
 	add    %rdx,%rax
 	mov    (%rax),%rax
 	mov    %rax,-0x10(%rbp)
@@ -248,102 +257,101 @@
 	lea    0x0(,%rax,8),%rdx
 	mov    -0x38(%rbp),%rax
 	add    %rdx,%rax
 	mov    (%rax),%rax
 	mov    %rax,-0x8(%rbp)
 	mov    -0x8(%rbp),%rax
 	cmp    -0x20(%rbp),%rax
-	jle    2927 <c_array_max_long_long+0x11f>
+	jle    1e20 <c_array_max_long_long+0x11b>
 	mov    -0x8(%rbp),%rax
 	mov    %rax,-0x20(%rbp)
 	mov    -0x10(%rbp),%rax
 	cmp    -0x18(%rbp),%rax
-	jge    2939 <c_array_max_long_long+0x131>
+	jge    1e32 <c_array_max_long_long+0x12d>
 	mov    -0x10(%rbp),%rax
 	mov    %rax,-0x18(%rbp)
 	addl   $0x2,-0x28(%rbp)
 	mov    -0x28(%rbp),%eax
 	cmp    -0x3c(%rbp),%eax
-	jl     2868 <c_array_max_long_long+0x60>
+	jl     1d61 <c_array_max_long_long+0x5c>
 	cmpl   $0x0,-0x24(%rbp)
-	je     29bf <c_array_max_long_long+0x1b7>
+	je     1eb8 <c_array_max_long_long+0x1b3>
 	mov    -0x3c(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,8),%rdx
 	mov    -0x38(%rbp),%rax
 	add    %rdx,%rax
 	mov    (%rax),%rax
 	cmp    %rax,-0x20(%rbp)
-	jge    2987 <c_array_max_long_long+0x17f>
+	jge    1e80 <c_array_max_long_long+0x17b>
 	mov    -0x3c(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,8),%rdx
 	mov    -0x38(%rbp),%rax
 	add    %rdx,%rax
 	mov    (%rax),%rax
 	mov    %rax,-0x20(%rbp)
 	mov    -0x3c(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,8),%rdx
 	mov    -0x38(%rbp),%rax
 	add    %rdx,%rax
 	mov    (%rax),%rax
 	cmp    %rax,-0x18(%rbp)
-	jle    29bf <c_array_max_long_long+0x1b7>
+	jle    1eb8 <c_array_max_long_long+0x1b3>
 	mov    -0x3c(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,8),%rdx
 	mov    -0x38(%rbp),%rax
 	add    %rdx,%rax
 	mov    (%rax),%rax
 	mov    %rax,-0x18(%rbp)
 	mov    -0x20(%rbp),%rax
 	pop    %rbp
 	ret
 
-00000000000029c5 <c_array_max_float>:
+0000000000001ebe <c_array_max_float>:
 c_array_max_float():
-	endbr64
 	push   %rbp
 	mov    %rsp,%rbp
 	mov    %rdi,-0x28(%rbp)
 	mov    %esi,-0x2c(%rbp)
 	mov    -0x2c(%rbp),%eax
 	and    $0x1,%eax
 	mov    %eax,-0x4(%rbp)
-	movss  0x4623(%rip),%xmm0        
+	movss  0x3dbe(%rip),%xmm0        
 	movss  %xmm0,-0x18(%rbp)
-	movss  0x461a(%rip),%xmm0        
+	movss  0x3db5(%rip),%xmm0        
 	movss  %xmm0,-0x14(%rbp)
 	cmpl   $0x0,-0x4(%rbp)
-	je     2a01 <c_array_max_float+0x3c>
+	je     1ef6 <c_array_max_float+0x38>
 	subl   $0x1,-0x2c(%rbp)
 	mov    -0x28(%rbp),%rax
 	movss  (%rax),%xmm0
 	movss  %xmm0,-0x10(%rbp)
 	mov    -0x28(%rbp),%rax
 	movss  (%rax),%xmm0
 	movss  %xmm0,-0xc(%rbp)
 	movl   $0x0,-0x8(%rbp)
-	jmp    2b0c <c_array_max_float+0x147>
+	jmp    2001 <c_array_max_float+0x143>
 	mov    -0x8(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,4),%rdx
 	mov    -0x28(%rbp),%rax
 	add    %rdx,%rax
 	movss  (%rax),%xmm0
 	mov    -0x8(%rbp),%eax
 	cltq
 	add    $0x1,%rax
 	lea    0x0(,%rax,4),%rdx
 	mov    -0x28(%rbp),%rax
 	add    %rdx,%rax
 	movss  (%rax),%xmm1
-	comiss %xmm1,%xmm0
-	jbe    2aa0 <c_array_max_float+0xdb>
+	ucomiss %xmm1,%xmm0
+	jbe    1f95 <c_array_max_float+0xd7>
 	mov    -0x8(%rbp),%eax
 	cltq
 	add    $0x1,%rax
 	lea    0x0(,%rax,4),%rdx
 	mov    -0x28(%rbp),%rax
 	add    %rdx,%rax
 	movss  (%rax),%xmm0
@@ -351,15 +359,15 @@
 	mov    -0x8(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,4),%rdx
 	mov    -0x28(%rbp),%rax
 	add    %rdx,%rax
 	movss  (%rax),%xmm0
 	movss  %xmm0,-0xc(%rbp)
-	jmp    2ade <c_array_max_float+0x119>
+	jmp    1fd3 <c_array_max_float+0x115>
 	mov    -0x8(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,4),%rdx
 	mov    -0x28(%rbp),%rax
 	add    %rdx,%rax
 	movss  (%rax),%xmm0
 	movss  %xmm0,-0x10(%rbp)
@@ -368,104 +376,103 @@
 	add    $0x1,%rax
 	lea    0x0(,%rax,4),%rdx
 	mov    -0x28(%rbp),%rax
 	add    %rdx,%rax
 	movss  (%rax),%xmm0
 	movss  %xmm0,-0xc(%rbp)
 	movss  -0xc(%rbp),%xmm0
-	comiss -0x18(%rbp),%xmm0
-	jbe    2af3 <c_array_max_float+0x12e>
+	ucomiss -0x18(%rbp),%xmm0
+	jbe    1fe8 <c_array_max_float+0x12a>
 	movss  -0xc(%rbp),%xmm0
 	movss  %xmm0,-0x18(%rbp)
 	movss  -0x14(%rbp),%xmm0
-	comiss -0x10(%rbp),%xmm0
-	jbe    2b08 <c_array_max_float+0x143>
+	ucomiss -0x10(%rbp),%xmm0
+	jbe    1ffd <c_array_max_float+0x13f>
 	movss  -0x10(%rbp),%xmm0
 	movss  %xmm0,-0x14(%rbp)
 	addl   $0x2,-0x8(%rbp)
 	mov    -0x8(%rbp),%eax
 	cmp    -0x2c(%rbp),%eax
-	jl     2a27 <c_array_max_float+0x62>
+	jl     1f1c <c_array_max_float+0x5e>
 	cmpl   $0x0,-0x4(%rbp)
-	je     2b98 <c_array_max_float+0x1d3>
+	je     208d <c_array_max_float+0x1cf>
 	mov    -0x2c(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,4),%rdx
 	mov    -0x28(%rbp),%rax
 	add    %rdx,%rax
 	movss  (%rax),%xmm0
-	comiss -0x18(%rbp),%xmm0
-	jbe    2b59 <c_array_max_float+0x194>
+	ucomiss -0x18(%rbp),%xmm0
+	jbe    204e <c_array_max_float+0x190>
 	mov    -0x2c(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,4),%rdx
 	mov    -0x28(%rbp),%rax
 	add    %rdx,%rax
 	movss  (%rax),%xmm0
 	movss  %xmm0,-0x18(%rbp)
 	mov    -0x2c(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,4),%rdx
 	mov    -0x28(%rbp),%rax
 	add    %rdx,%rax
 	movss  (%rax),%xmm1
 	movss  -0x14(%rbp),%xmm0
-	comiss %xmm1,%xmm0
-	jbe    2b98 <c_array_max_float+0x1d3>
+	ucomiss %xmm1,%xmm0
+	jbe    208d <c_array_max_float+0x1cf>
 	mov    -0x2c(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,4),%rdx
 	mov    -0x28(%rbp),%rax
 	add    %rdx,%rax
 	movss  (%rax),%xmm0
 	movss  %xmm0,-0x14(%rbp)
 	movss  -0x18(%rbp),%xmm0
 	pop    %rbp
 	ret
 
-0000000000002b9f <c_array_max_double>:
+0000000000002094 <c_array_max_double>:
 c_array_max_double():
-	endbr64
 	push   %rbp
 	mov    %rsp,%rbp
 	mov    %rdi,-0x38(%rbp)
 	mov    %esi,-0x3c(%rbp)
 	mov    -0x3c(%rbp),%eax
 	and    $0x1,%eax
 	mov    %eax,-0x24(%rbp)
-	movsd  0x4451(%rip),%xmm0        
+	movsd  0x3bf0(%rip),%xmm0        
 	movsd  %xmm0,-0x20(%rbp)
-	movsd  0x444c(%rip),%xmm0        
+	movsd  0x3beb(%rip),%xmm0        
 	movsd  %xmm0,-0x18(%rbp)
 	cmpl   $0x0,-0x24(%rbp)
-	je     2bdb <c_array_max_double+0x3c>
+	je     20cc <c_array_max_double+0x38>
 	subl   $0x1,-0x3c(%rbp)
 	mov    -0x38(%rbp),%rax
 	movsd  (%rax),%xmm0
 	movsd  %xmm0,-0x10(%rbp)
 	mov    -0x38(%rbp),%rax
 	movsd  (%rax),%xmm0
 	movsd  %xmm0,-0x8(%rbp)
 	movl   $0x0,-0x28(%rbp)
-	jmp    2ce9 <c_array_max_double+0x14a>
+	jmp    21da <c_array_max_double+0x146>
 	mov    -0x28(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,8),%rdx
 	mov    -0x38(%rbp),%rax
 	add    %rdx,%rax
 	movsd  (%rax),%xmm0
 	mov    -0x28(%rbp),%eax
 	cltq
 	add    $0x1,%rax
 	lea    0x0(,%rax,8),%rdx
 	mov    -0x38(%rbp),%rax
 	add    %rdx,%rax
 	movsd  (%rax),%xmm1
-	comisd %xmm1,%xmm0
-	jbe    2c7b <c_array_max_double+0xdc>
+	ucomisd %xmm1,%xmm0
+	jbe    216c <c_array_max_double+0xd8>
 	mov    -0x28(%rbp),%eax
 	cltq
 	add    $0x1,%rax
 	lea    0x0(,%rax,8),%rdx
 	mov    -0x38(%rbp),%rax
 	add    %rdx,%rax
 	movsd  (%rax),%xmm0
@@ -473,15 +480,15 @@
 	mov    -0x28(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,8),%rdx
 	mov    -0x38(%rbp),%rax
 	add    %rdx,%rax
 	movsd  (%rax),%xmm0
 	movsd  %xmm0,-0x8(%rbp)
-	jmp    2cb9 <c_array_max_double+0x11a>
+	jmp    21aa <c_array_max_double+0x116>
 	mov    -0x28(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,8),%rdx
 	mov    -0x38(%rbp),%rax
 	add    %rdx,%rax
 	movsd  (%rax),%xmm0
 	movsd  %xmm0,-0x10(%rbp)
@@ -490,102 +497,101 @@
 	add    $0x1,%rax
 	lea    0x0(,%rax,8),%rdx
 	mov    -0x38(%rbp),%rax
 	add    %rdx,%rax
 	movsd  (%rax),%xmm0
 	movsd  %xmm0,-0x8(%rbp)
 	movsd  -0x8(%rbp),%xmm0
-	comisd -0x20(%rbp),%xmm0
-	jbe    2ccf <c_array_max_double+0x130>
+	ucomisd -0x20(%rbp),%xmm0
+	jbe    21c0 <c_array_max_double+0x12c>
 	movsd  -0x8(%rbp),%xmm0
 	movsd  %xmm0,-0x20(%rbp)
 	movsd  -0x18(%rbp),%xmm0
-	comisd -0x10(%rbp),%xmm0
-	jbe    2ce5 <c_array_max_double+0x146>
+	ucomisd -0x10(%rbp),%xmm0
+	jbe    21d6 <c_array_max_double+0x142>
 	movsd  -0x10(%rbp),%xmm0
 	movsd  %xmm0,-0x18(%rbp)
 	addl   $0x2,-0x28(%rbp)
 	mov    -0x28(%rbp),%eax
 	cmp    -0x3c(%rbp),%eax
-	jl     2c01 <c_array_max_double+0x62>
+	jl     20f2 <c_array_max_double+0x5e>
 	cmpl   $0x0,-0x24(%rbp)
-	je     2d77 <c_array_max_double+0x1d8>
+	je     2268 <c_array_max_double+0x1d4>
 	mov    -0x3c(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,8),%rdx
 	mov    -0x38(%rbp),%rax
 	add    %rdx,%rax
 	movsd  (%rax),%xmm0
-	comisd -0x20(%rbp),%xmm0
-	jbe    2d37 <c_array_max_double+0x198>
+	ucomisd -0x20(%rbp),%xmm0
+	jbe    2228 <c_array_max_double+0x194>
 	mov    -0x3c(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,8),%rdx
 	mov    -0x38(%rbp),%rax
 	add    %rdx,%rax
 	movsd  (%rax),%xmm0
 	movsd  %xmm0,-0x20(%rbp)
 	mov    -0x3c(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,8),%rdx
 	mov    -0x38(%rbp),%rax
 	add    %rdx,%rax
 	movsd  (%rax),%xmm1
 	movsd  -0x18(%rbp),%xmm0
-	comisd %xmm1,%xmm0
-	jbe    2d77 <c_array_max_double+0x1d8>
+	ucomisd %xmm1,%xmm0
+	jbe    2268 <c_array_max_double+0x1d4>
 	mov    -0x3c(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,8),%rdx
 	mov    -0x38(%rbp),%rax
 	add    %rdx,%rax
 	movsd  (%rax),%xmm0
 	movsd  %xmm0,-0x18(%rbp)
 	movsd  -0x20(%rbp),%xmm0
 	pop    %rbp
 	ret
 
-0000000000002d7e <c_array_min_int>:
+000000000000226f <c_array_min_int>:
 c_array_min_int():
-	endbr64
 	push   %rbp
 	mov    %rsp,%rbp
 	mov    %rdi,-0x28(%rbp)
 	mov    %esi,-0x2c(%rbp)
 	mov    -0x2c(%rbp),%eax
 	and    $0x1,%eax
 	mov    %eax,-0x4(%rbp)
 	movl   $0xff000000,-0x18(%rbp)
 	movl   $0xffffff,-0x14(%rbp)
 	cmpl   $0x0,-0x4(%rbp)
-	je     2dae <c_array_min_int+0x30>
+	je     229b <c_array_min_int+0x2c>
 	subl   $0x1,-0x2c(%rbp)
 	mov    -0x28(%rbp),%rax
 	mov    (%rax),%eax
 	mov    %eax,-0x10(%rbp)
 	mov    -0x28(%rbp),%rax
 	mov    (%rax),%eax
 	mov    %eax,-0xc(%rbp)
 	movl   $0x0,-0x8(%rbp)
-	jmp    2e8e <c_array_min_int+0x110>
+	jmp    237b <c_array_min_int+0x10c>
 	mov    -0x8(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,4),%rdx
 	mov    -0x28(%rbp),%rax
 	add    %rdx,%rax
 	mov    (%rax),%edx
 	mov    -0x8(%rbp),%eax
 	cltq
 	add    $0x1,%rax
 	lea    0x0(,%rax,4),%rcx
 	mov    -0x28(%rbp),%rax
 	add    %rcx,%rax
 	mov    (%rax),%eax
 	cmp    %eax,%edx
-	jle    2e38 <c_array_min_int+0xba>
+	jle    2325 <c_array_min_int+0xb6>
 	mov    -0x8(%rbp),%eax
 	cltq
 	add    $0x1,%rax
 	lea    0x0(,%rax,4),%rdx
 	mov    -0x28(%rbp),%rax
 	add    %rdx,%rax
 	mov    (%rax),%eax
@@ -593,15 +599,15 @@
 	mov    -0x8(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,4),%rdx
 	mov    -0x28(%rbp),%rax
 	add    %rdx,%rax
 	mov    (%rax),%eax
 	mov    %eax,-0xc(%rbp)
-	jmp    2e6e <c_array_min_int+0xf0>
+	jmp    235b <c_array_min_int+0xec>
 	mov    -0x8(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,4),%rdx
 	mov    -0x28(%rbp),%rax
 	add    %rdx,%rax
 	mov    (%rax),%eax
 	mov    %eax,-0x10(%rbp)
@@ -611,108 +617,107 @@
 	lea    0x0(,%rax,4),%rdx
 	mov    -0x28(%rbp),%rax
 	add    %rdx,%rax
 	mov    (%rax),%eax
 	mov    %eax,-0xc(%rbp)
 	mov    -0xc(%rbp),%eax
 	cmp    -0x18(%rbp),%eax
-	jle    2e7c <c_array_min_int+0xfe>
+	jle    2369 <c_array_min_int+0xfa>
 	mov    -0xc(%rbp),%eax
 	mov    %eax,-0x18(%rbp)
 	mov    -0x10(%rbp),%eax
 	cmp    -0x14(%rbp),%eax
-	jge    2e8a <c_array_min_int+0x10c>
+	jge    2377 <c_array_min_int+0x108>
 	mov    -0x10(%rbp),%eax
 	mov    %eax,-0x14(%rbp)
 	addl   $0x2,-0x8(%rbp)
 	mov    -0x8(%rbp),%eax
 	cmp    -0x2c(%rbp),%eax
-	jl     2dcc <c_array_min_int+0x4e>
+	jl     22b9 <c_array_min_int+0x4a>
 	cmpl   $0x0,-0x4(%rbp)
-	je     2f08 <c_array_min_int+0x18a>
+	je     23f5 <c_array_min_int+0x186>
 	mov    -0x2c(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,4),%rdx
 	mov    -0x28(%rbp),%rax
 	add    %rdx,%rax
 	mov    (%rax),%eax
 	cmp    %eax,-0x18(%rbp)
-	jge    2ed4 <c_array_min_int+0x156>
+	jge    23c1 <c_array_min_int+0x152>
 	mov    -0x2c(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,4),%rdx
 	mov    -0x28(%rbp),%rax
 	add    %rdx,%rax
 	mov    (%rax),%eax
 	mov    %eax,-0x18(%rbp)
 	mov    -0x2c(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,4),%rdx
 	mov    -0x28(%rbp),%rax
 	add    %rdx,%rax
 	mov    (%rax),%eax
 	cmp    %eax,-0x14(%rbp)
-	jle    2f08 <c_array_min_int+0x18a>
+	jle    23f5 <c_array_min_int+0x186>
 	mov    -0x2c(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,4),%rdx
 	mov    -0x28(%rbp),%rax
 	add    %rdx,%rax
 	mov    (%rax),%eax
 	mov    %eax,-0x14(%rbp)
-	lea    0x40f1(%rip),%rdx        
-	lea    0x40ee(%rip),%rax        
+	lea    0x3894(%rip),%rdx        
+	lea    0x3891(%rip),%rax        
 	cmp    %rax,%rdx
-	jne    2f20 <c_array_min_int+0x1a2>
+	jne    240d <c_array_min_int+0x19e>
 	mov    -0x18(%rbp),%eax
-	jmp    2f23 <c_array_min_int+0x1a5>
+	jmp    2410 <c_array_min_int+0x1a1>
 	mov    -0x14(%rbp),%eax
 	pop    %rbp
 	ret
 
-0000000000002f25 <c_array_min_long_long>:
+0000000000002412 <c_array_min_long_long>:
 c_array_min_long_long():
-	endbr64
 	push   %rbp
 	mov    %rsp,%rbp
 	mov    %rdi,-0x38(%rbp)
 	mov    %esi,-0x3c(%rbp)
 	mov    -0x3c(%rbp),%eax
 	and    $0x1,%eax
 	mov    %eax,-0x24(%rbp)
 	movabs $0xff00000000000000,%rax
 	mov    %rax,-0x20(%rbp)
 	movabs $0x100000000000000,%rax
 	mov    %rax,-0x18(%rbp)
 	cmpl   $0x0,-0x24(%rbp)
-	je     2f63 <c_array_min_long_long+0x3e>
+	je     244c <c_array_min_long_long+0x3a>
 	subl   $0x1,-0x3c(%rbp)
 	mov    -0x38(%rbp),%rax
 	mov    (%rax),%rax
 	mov    %rax,-0x10(%rbp)
 	mov    -0x38(%rbp),%rax
 	mov    (%rax),%rax
 	mov    %rax,-0x8(%rbp)
 	movl   $0x0,-0x28(%rbp)
-	jmp    305a <c_array_min_long_long+0x135>
+	jmp    2543 <c_array_min_long_long+0x131>
 	mov    -0x28(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,8),%rdx
 	mov    -0x38(%rbp),%rax
 	add    %rdx,%rax
 	mov    (%rax),%rdx
 	mov    -0x28(%rbp),%eax
 	cltq
 	add    $0x1,%rax
 	lea    0x0(,%rax,8),%rcx
 	mov    -0x38(%rbp),%rax
 	add    %rcx,%rax
 	mov    (%rax),%rax
 	cmp    %rax,%rdx
-	jle    2ff8 <c_array_min_long_long+0xd3>
+	jle    24e1 <c_array_min_long_long+0xcf>
 	mov    -0x28(%rbp),%eax
 	cltq
 	add    $0x1,%rax
 	lea    0x0(,%rax,8),%rdx
 	mov    -0x38(%rbp),%rax
 	add    %rdx,%rax
 	mov    (%rax),%rax
@@ -720,15 +725,15 @@
 	mov    -0x28(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,8),%rdx
 	mov    -0x38(%rbp),%rax
 	add    %rdx,%rax
 	mov    (%rax),%rax
 	mov    %rax,-0x8(%rbp)
-	jmp    3032 <c_array_min_long_long+0x10d>
+	jmp    251b <c_array_min_long_long+0x109>
 	mov    -0x28(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,8),%rdx
 	mov    -0x38(%rbp),%rax
 	add    %rdx,%rax
 	mov    (%rax),%rax
 	mov    %rax,-0x10(%rbp)
@@ -738,108 +743,107 @@
 	lea    0x0(,%rax,8),%rdx
 	mov    -0x38(%rbp),%rax
 	add    %rdx,%rax
 	mov    (%rax),%rax
 	mov    %rax,-0x8(%rbp)
 	mov    -0x8(%rbp),%rax
 	cmp    -0x20(%rbp),%rax
-	jle    3044 <c_array_min_long_long+0x11f>
+	jle    252d <c_array_min_long_long+0x11b>
 	mov    -0x8(%rbp),%rax
 	mov    %rax,-0x20(%rbp)
 	mov    -0x10(%rbp),%rax
 	cmp    -0x18(%rbp),%rax
-	jge    3056 <c_array_min_long_long+0x131>
+	jge    253f <c_array_min_long_long+0x12d>
 	mov    -0x10(%rbp),%rax
 	mov    %rax,-0x18(%rbp)
 	addl   $0x2,-0x28(%rbp)
 	mov    -0x28(%rbp),%eax
 	cmp    -0x3c(%rbp),%eax
-	jl     2f85 <c_array_min_long_long+0x60>
+	jl     246e <c_array_min_long_long+0x5c>
 	cmpl   $0x0,-0x24(%rbp)
-	je     30dc <c_array_min_long_long+0x1b7>
+	je     25c5 <c_array_min_long_long+0x1b3>
 	mov    -0x3c(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,8),%rdx
 	mov    -0x38(%rbp),%rax
 	add    %rdx,%rax
 	mov    (%rax),%rax
 	cmp    %rax,-0x20(%rbp)
-	jge    30a4 <c_array_min_long_long+0x17f>
+	jge    258d <c_array_min_long_long+0x17b>
 	mov    -0x3c(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,8),%rdx
 	mov    -0x38(%rbp),%rax
 	add    %rdx,%rax
 	mov    (%rax),%rax
 	mov    %rax,-0x20(%rbp)
 	mov    -0x3c(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,8),%rdx
 	mov    -0x38(%rbp),%rax
 	add    %rdx,%rax
 	mov    (%rax),%rax
 	cmp    %rax,-0x18(%rbp)
-	jle    30dc <c_array_min_long_long+0x1b7>
+	jle    25c5 <c_array_min_long_long+0x1b3>
 	mov    -0x3c(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,8),%rdx
 	mov    -0x38(%rbp),%rax
 	add    %rdx,%rax
 	mov    (%rax),%rax
 	mov    %rax,-0x18(%rbp)
-	lea    0x3f1d(%rip),%rdx        
-	lea    0x3f1a(%rip),%rax        
+	lea    0x36c4(%rip),%rdx        
+	lea    0x36c1(%rip),%rax        
 	cmp    %rax,%rdx
-	jne    30f5 <c_array_min_long_long+0x1d0>
+	jne    25de <c_array_min_long_long+0x1cc>
 	mov    -0x20(%rbp),%rax
-	jmp    30f9 <c_array_min_long_long+0x1d4>
+	jmp    25e2 <c_array_min_long_long+0x1d0>
 	mov    -0x18(%rbp),%rax
 	pop    %rbp
 	ret
 
-00000000000030fb <c_array_min_float>:
+00000000000025e4 <c_array_min_float>:
 c_array_min_float():
-	endbr64
 	push   %rbp
 	mov    %rsp,%rbp
 	mov    %rdi,-0x28(%rbp)
 	mov    %esi,-0x2c(%rbp)
 	mov    -0x2c(%rbp),%eax
 	and    $0x1,%eax
 	mov    %eax,-0x4(%rbp)
-	movss  0x3eed(%rip),%xmm0        
+	movss  0x3698(%rip),%xmm0        
 	movss  %xmm0,-0x18(%rbp)
-	movss  0x3ee4(%rip),%xmm0        
+	movss  0x368f(%rip),%xmm0        
 	movss  %xmm0,-0x14(%rbp)
 	cmpl   $0x0,-0x4(%rbp)
-	je     3137 <c_array_min_float+0x3c>
+	je     261c <c_array_min_float+0x38>
 	subl   $0x1,-0x2c(%rbp)
 	mov    -0x28(%rbp),%rax
 	movss  (%rax),%xmm0
 	movss  %xmm0,-0x10(%rbp)
 	mov    -0x28(%rbp),%rax
 	movss  (%rax),%xmm0
 	movss  %xmm0,-0xc(%rbp)
 	movl   $0x0,-0x8(%rbp)
-	jmp    3242 <c_array_min_float+0x147>
+	jmp    2727 <c_array_min_float+0x143>
 	mov    -0x8(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,4),%rdx
 	mov    -0x28(%rbp),%rax
 	add    %rdx,%rax
 	movss  (%rax),%xmm0
 	mov    -0x8(%rbp),%eax
 	cltq
 	add    $0x1,%rax
 	lea    0x0(,%rax,4),%rdx
 	mov    -0x28(%rbp),%rax
 	add    %rdx,%rax
 	movss  (%rax),%xmm1
-	comiss %xmm1,%xmm0
-	jbe    31d6 <c_array_min_float+0xdb>
+	ucomiss %xmm1,%xmm0
+	jbe    26bb <c_array_min_float+0xd7>
 	mov    -0x8(%rbp),%eax
 	cltq
 	add    $0x1,%rax
 	lea    0x0(,%rax,4),%rdx
 	mov    -0x28(%rbp),%rax
 	add    %rdx,%rax
 	movss  (%rax),%xmm0
@@ -847,15 +851,15 @@
 	mov    -0x8(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,4),%rdx
 	mov    -0x28(%rbp),%rax
 	add    %rdx,%rax
 	movss  (%rax),%xmm0
 	movss  %xmm0,-0xc(%rbp)
-	jmp    3214 <c_array_min_float+0x119>
+	jmp    26f9 <c_array_min_float+0x115>
 	mov    -0x8(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,4),%rdx
 	mov    -0x28(%rbp),%rax
 	add    %rdx,%rax
 	movss  (%rax),%xmm0
 	movss  %xmm0,-0x10(%rbp)
@@ -864,110 +868,109 @@
 	add    $0x1,%rax
 	lea    0x0(,%rax,4),%rdx
 	mov    -0x28(%rbp),%rax
 	add    %rdx,%rax
 	movss  (%rax),%xmm0
 	movss  %xmm0,-0xc(%rbp)
 	movss  -0xc(%rbp),%xmm0
-	comiss -0x18(%rbp),%xmm0
-	jbe    3229 <c_array_min_float+0x12e>
+	ucomiss -0x18(%rbp),%xmm0
+	jbe    270e <c_array_min_float+0x12a>
 	movss  -0xc(%rbp),%xmm0
 	movss  %xmm0,-0x18(%rbp)
 	movss  -0x14(%rbp),%xmm0
-	comiss -0x10(%rbp),%xmm0
-	jbe    323e <c_array_min_float+0x143>
+	ucomiss -0x10(%rbp),%xmm0
+	jbe    2723 <c_array_min_float+0x13f>
 	movss  -0x10(%rbp),%xmm0
 	movss  %xmm0,-0x14(%rbp)
 	addl   $0x2,-0x8(%rbp)
 	mov    -0x8(%rbp),%eax
 	cmp    -0x2c(%rbp),%eax
-	jl     315d <c_array_min_float+0x62>
+	jl     2642 <c_array_min_float+0x5e>
 	cmpl   $0x0,-0x4(%rbp)
-	je     32ce <c_array_min_float+0x1d3>
+	je     27b3 <c_array_min_float+0x1cf>
 	mov    -0x2c(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,4),%rdx
 	mov    -0x28(%rbp),%rax
 	add    %rdx,%rax
 	movss  (%rax),%xmm0
-	comiss -0x18(%rbp),%xmm0
-	jbe    328f <c_array_min_float+0x194>
+	ucomiss -0x18(%rbp),%xmm0
+	jbe    2774 <c_array_min_float+0x190>
 	mov    -0x2c(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,4),%rdx
 	mov    -0x28(%rbp),%rax
 	add    %rdx,%rax
 	movss  (%rax),%xmm0
 	movss  %xmm0,-0x18(%rbp)
 	mov    -0x2c(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,4),%rdx
 	mov    -0x28(%rbp),%rax
 	add    %rdx,%rax
 	movss  (%rax),%xmm1
 	movss  -0x14(%rbp),%xmm0
-	comiss %xmm1,%xmm0
-	jbe    32ce <c_array_min_float+0x1d3>
+	ucomiss %xmm1,%xmm0
+	jbe    27b3 <c_array_min_float+0x1cf>
 	mov    -0x2c(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,4),%rdx
 	mov    -0x28(%rbp),%rax
 	add    %rdx,%rax
 	movss  (%rax),%xmm0
 	movss  %xmm0,-0x14(%rbp)
-	lea    0x3d2b(%rip),%rdx        
-	lea    0x3d28(%rip),%rax        
+	lea    0x34d6(%rip),%rdx        
+	lea    0x34d3(%rip),%rax        
 	cmp    %rax,%rdx
-	jne    32e8 <c_array_min_float+0x1ed>
+	jne    27cd <c_array_min_float+0x1e9>
 	movss  -0x18(%rbp),%xmm0
-	jmp    32ed <c_array_min_float+0x1f2>
+	jmp    27d2 <c_array_min_float+0x1ee>
 	movss  -0x14(%rbp),%xmm0
 	pop    %rbp
 	ret
 
-00000000000032ef <c_array_min_double>:
+00000000000027d4 <c_array_min_double>:
 c_array_min_double():
-	endbr64
 	push   %rbp
 	mov    %rsp,%rbp
 	mov    %rdi,-0x38(%rbp)
 	mov    %esi,-0x3c(%rbp)
 	mov    -0x3c(%rbp),%eax
 	and    $0x1,%eax
 	mov    %eax,-0x24(%rbp)
-	movsd  0x3d01(%rip),%xmm0        
+	movsd  0x34b0(%rip),%xmm0        
 	movsd  %xmm0,-0x20(%rbp)
-	movsd  0x3cfc(%rip),%xmm0        
+	movsd  0x34ab(%rip),%xmm0        
 	movsd  %xmm0,-0x18(%rbp)
 	cmpl   $0x0,-0x24(%rbp)
-	je     332b <c_array_min_double+0x3c>
+	je     280c <c_array_min_double+0x38>
 	subl   $0x1,-0x3c(%rbp)
 	mov    -0x38(%rbp),%rax
 	movsd  (%rax),%xmm0
 	movsd  %xmm0,-0x10(%rbp)
 	mov    -0x38(%rbp),%rax
 	movsd  (%rax),%xmm0
 	movsd  %xmm0,-0x8(%rbp)
 	movl   $0x0,-0x28(%rbp)
-	jmp    3439 <c_array_min_double+0x14a>
+	jmp    291a <c_array_min_double+0x146>
 	mov    -0x28(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,8),%rdx
 	mov    -0x38(%rbp),%rax
 	add    %rdx,%rax
 	movsd  (%rax),%xmm0
 	mov    -0x28(%rbp),%eax
 	cltq
 	add    $0x1,%rax
 	lea    0x0(,%rax,8),%rdx
 	mov    -0x38(%rbp),%rax
 	add    %rdx,%rax
 	movsd  (%rax),%xmm1
-	comisd %xmm1,%xmm0
-	jbe    33cb <c_array_min_double+0xdc>
+	ucomisd %xmm1,%xmm0
+	jbe    28ac <c_array_min_double+0xd8>
 	mov    -0x28(%rbp),%eax
 	cltq
 	add    $0x1,%rax
 	lea    0x0(,%rax,8),%rdx
 	mov    -0x38(%rbp),%rax
 	add    %rdx,%rax
 	movsd  (%rax),%xmm0
@@ -975,15 +978,15 @@
 	mov    -0x28(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,8),%rdx
 	mov    -0x38(%rbp),%rax
 	add    %rdx,%rax
 	movsd  (%rax),%xmm0
 	movsd  %xmm0,-0x8(%rbp)
-	jmp    3409 <c_array_min_double+0x11a>
+	jmp    28ea <c_array_min_double+0x116>
 	mov    -0x28(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,8),%rdx
 	mov    -0x38(%rbp),%rax
 	add    %rdx,%rax
 	movsd  (%rax),%xmm0
 	movsd  %xmm0,-0x10(%rbp)
@@ -992,631 +995,639 @@
 	add    $0x1,%rax
 	lea    0x0(,%rax,8),%rdx
 	mov    -0x38(%rbp),%rax
 	add    %rdx,%rax
 	movsd  (%rax),%xmm0
 	movsd  %xmm0,-0x8(%rbp)
 	movsd  -0x8(%rbp),%xmm0
-	comisd -0x20(%rbp),%xmm0
-	jbe    341f <c_array_min_double+0x130>
+	ucomisd -0x20(%rbp),%xmm0
+	jbe    2900 <c_array_min_double+0x12c>
 	movsd  -0x8(%rbp),%xmm0
 	movsd  %xmm0,-0x20(%rbp)
 	movsd  -0x18(%rbp),%xmm0
-	comisd -0x10(%rbp),%xmm0
-	jbe    3435 <c_array_min_double+0x146>
+	ucomisd -0x10(%rbp),%xmm0
+	jbe    2916 <c_array_min_double+0x142>
 	movsd  -0x10(%rbp),%xmm0
 	movsd  %xmm0,-0x18(%rbp)
 	addl   $0x2,-0x28(%rbp)
 	mov    -0x28(%rbp),%eax
 	cmp    -0x3c(%rbp),%eax
-	jl     3351 <c_array_min_double+0x62>
+	jl     2832 <c_array_min_double+0x5e>
 	cmpl   $0x0,-0x24(%rbp)
-	je     34c7 <c_array_min_double+0x1d8>
+	je     29a8 <c_array_min_double+0x1d4>
 	mov    -0x3c(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,8),%rdx
 	mov    -0x38(%rbp),%rax
 	add    %rdx,%rax
 	movsd  (%rax),%xmm0
-	comisd -0x20(%rbp),%xmm0
-	jbe    3487 <c_array_min_double+0x198>
+	ucomisd -0x20(%rbp),%xmm0
+	jbe    2968 <c_array_min_double+0x194>
 	mov    -0x3c(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,8),%rdx
 	mov    -0x38(%rbp),%rax
 	add    %rdx,%rax
 	movsd  (%rax),%xmm0
 	movsd  %xmm0,-0x20(%rbp)
 	mov    -0x3c(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,8),%rdx
 	mov    -0x38(%rbp),%rax
 	add    %rdx,%rax
 	movsd  (%rax),%xmm1
 	movsd  -0x18(%rbp),%xmm0
-	comisd %xmm1,%xmm0
-	jbe    34c7 <c_array_min_double+0x1d8>
+	ucomisd %xmm1,%xmm0
+	jbe    29a8 <c_array_min_double+0x1d4>
 	mov    -0x3c(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,8),%rdx
 	mov    -0x38(%rbp),%rax
 	add    %rdx,%rax
 	movsd  (%rax),%xmm0
 	movsd  %xmm0,-0x18(%rbp)
-	lea    0x3b32(%rip),%rdx        
-	lea    0x3b2f(%rip),%rax        
+	lea    0x32e1(%rip),%rdx        
+	lea    0x32de(%rip),%rax        
 	cmp    %rax,%rdx
-	jne    34e1 <c_array_min_double+0x1f2>
+	jne    29c2 <c_array_min_double+0x1ee>
 	movsd  -0x20(%rbp),%xmm0
-	jmp    34e6 <c_array_min_double+0x1f7>
+	jmp    29c7 <c_array_min_double+0x1f3>
 	movsd  -0x18(%rbp),%xmm0
 	pop    %rbp
 	ret
 
-00000000000034e8 <c_array_var_int>:
+00000000000029c9 <c_array_var_int>:
 c_array_var_int():
-	endbr64
 	push   %rbp
 	mov    %rsp,%rbp
 	sub    $0x30,%rsp
 	mov    %rdi,-0x18(%rbp)
 	mov    %esi,-0x1c(%rbp)
 	movsd  %xmm0,-0x28(%rbp)
 	pxor   %xmm0,%xmm0
 	movsd  %xmm0,-0x8(%rbp)
 	movl   $0x0,-0xc(%rbp)
-	jmp    3550 <c_array_var_int+0x68>
+	jmp    2a31 <c_array_var_int+0x68>
 	mov    -0xc(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,4),%rdx
 	mov    -0x18(%rbp),%rax
 	add    %rdx,%rax
 	mov    (%rax),%eax
 	cvtsi2sd %eax,%xmm0
 	subsd  -0x28(%rbp),%xmm0
-	movsd  0x3ae7(%rip),%xmm1        
-	call   2550 <pow@plt>
-	movsd  -0x8(%rbp),%xmm1
+	movsd  0x329a(%rip),%xmm1        
+	call   1a20 <pow@plt>
+	movapd %xmm0,%xmm1
+	movsd  -0x8(%rbp),%xmm0
 	addsd  %xmm1,%xmm0
 	movsd  %xmm0,-0x8(%rbp)
 	addl   $0x1,-0xc(%rbp)
 	mov    -0xc(%rbp),%eax
 	cmp    -0x1c(%rbp),%eax
-	jl     3512 <c_array_var_int+0x2a>
-	cvtsi2sdl -0x1c(%rbp),%xmm1
-	movsd  -0x8(%rbp),%xmm0
-	divsd  %xmm1,%xmm0
+	jl     29ef <c_array_var_int+0x26>
+	cvtsi2sdl -0x1c(%rbp),%xmm0
+	movsd  -0x8(%rbp),%xmm1
+	divsd  %xmm0,%xmm1
+	movapd %xmm1,%xmm0
 	leave
 	ret
 
-0000000000003568 <c_array_var_long_long>:
+0000000000002a4d <c_array_var_long_long>:
 c_array_var_long_long():
-	endbr64
 	push   %rbp
 	mov    %rsp,%rbp
 	sub    $0x30,%rsp
 	mov    %rdi,-0x18(%rbp)
 	mov    %esi,-0x1c(%rbp)
 	movsd  %xmm0,-0x28(%rbp)
 	pxor   %xmm0,%xmm0
 	movsd  %xmm0,-0x8(%rbp)
 	movl   $0x0,-0xc(%rbp)
-	jmp    35d2 <c_array_var_long_long+0x6a>
+	jmp    2ab7 <c_array_var_long_long+0x6a>
 	mov    -0xc(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,8),%rdx
 	mov    -0x18(%rbp),%rax
 	add    %rdx,%rax
 	mov    (%rax),%rax
 	cvtsi2sd %rax,%xmm0
 	subsd  -0x28(%rbp),%xmm0
-	movsd  0x3a65(%rip),%xmm1        
-	call   2550 <pow@plt>
-	movsd  -0x8(%rbp),%xmm1
+	movsd  0x3214(%rip),%xmm1        
+	call   1a20 <pow@plt>
+	movapd %xmm0,%xmm1
+	movsd  -0x8(%rbp),%xmm0
 	addsd  %xmm1,%xmm0
 	movsd  %xmm0,-0x8(%rbp)
 	addl   $0x1,-0xc(%rbp)
 	mov    -0xc(%rbp),%eax
 	cmp    -0x1c(%rbp),%eax
-	jl     3592 <c_array_var_long_long+0x2a>
-	cvtsi2sdl -0x1c(%rbp),%xmm1
-	movsd  -0x8(%rbp),%xmm0
-	divsd  %xmm1,%xmm0
+	jl     2a73 <c_array_var_long_long+0x26>
+	cvtsi2sdl -0x1c(%rbp),%xmm0
+	movsd  -0x8(%rbp),%xmm1
+	divsd  %xmm0,%xmm1
+	movapd %xmm1,%xmm0
 	leave
 	ret
 
-00000000000035ea <c_array_var_float>:
+0000000000002ad3 <c_array_var_float>:
 c_array_var_float():
-	endbr64
 	push   %rbp
 	mov    %rsp,%rbp
 	sub    $0x30,%rsp
 	mov    %rdi,-0x18(%rbp)
 	mov    %esi,-0x1c(%rbp)
 	movsd  %xmm0,-0x28(%rbp)
 	pxor   %xmm0,%xmm0
 	movsd  %xmm0,-0x8(%rbp)
 	movl   $0x0,-0xc(%rbp)
-	jmp    3654 <c_array_var_float+0x6a>
+	jmp    2b3d <c_array_var_float+0x6a>
 	mov    -0xc(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,4),%rdx
 	mov    -0x18(%rbp),%rax
 	add    %rdx,%rax
 	movss  (%rax),%xmm0
 	cvtss2sd %xmm0,%xmm0
 	subsd  -0x28(%rbp),%xmm0
-	movsd  0x39e3(%rip),%xmm1        
-	call   2550 <pow@plt>
-	movsd  -0x8(%rbp),%xmm1
+	movsd  0x318e(%rip),%xmm1        
+	call   1a20 <pow@plt>
+	movapd %xmm0,%xmm1
+	movsd  -0x8(%rbp),%xmm0
 	addsd  %xmm1,%xmm0
 	movsd  %xmm0,-0x8(%rbp)
 	addl   $0x1,-0xc(%rbp)
 	mov    -0xc(%rbp),%eax
 	cmp    -0x1c(%rbp),%eax
-	jl     3614 <c_array_var_float+0x2a>
-	cvtsi2sdl -0x1c(%rbp),%xmm1
-	movsd  -0x8(%rbp),%xmm0
-	divsd  %xmm1,%xmm0
+	jl     2af9 <c_array_var_float+0x26>
+	cvtsi2sdl -0x1c(%rbp),%xmm0
+	movsd  -0x8(%rbp),%xmm1
+	divsd  %xmm0,%xmm1
+	movapd %xmm1,%xmm0
 	leave
 	ret
 
-000000000000366c <c_array_var_double>:
+0000000000002b59 <c_array_var_double>:
 c_array_var_double():
-	endbr64
 	push   %rbp
 	mov    %rsp,%rbp
 	sub    $0x30,%rsp
 	mov    %rdi,-0x18(%rbp)
 	mov    %esi,-0x1c(%rbp)
 	movsd  %xmm0,-0x28(%rbp)
 	pxor   %xmm0,%xmm0
 	movsd  %xmm0,-0x8(%rbp)
 	movl   $0x0,-0xc(%rbp)
-	jmp    36d2 <c_array_var_double+0x66>
+	jmp    2bbf <c_array_var_double+0x66>
 	mov    -0xc(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,8),%rdx
 	mov    -0x18(%rbp),%rax
 	add    %rdx,%rax
 	movsd  (%rax),%xmm0
 	subsd  -0x28(%rbp),%xmm0
-	movsd  0x3965(%rip),%xmm1        
-	call   2550 <pow@plt>
-	movsd  -0x8(%rbp),%xmm1
+	movsd  0x310c(%rip),%xmm1        
+	call   1a20 <pow@plt>
+	movapd %xmm0,%xmm1
+	movsd  -0x8(%rbp),%xmm0
 	addsd  %xmm1,%xmm0
 	movsd  %xmm0,-0x8(%rbp)
 	addl   $0x1,-0xc(%rbp)
 	mov    -0xc(%rbp),%eax
 	cmp    -0x1c(%rbp),%eax
-	jl     3696 <c_array_var_double+0x2a>
-	cvtsi2sdl -0x1c(%rbp),%xmm1
-	movsd  -0x8(%rbp),%xmm0
-	divsd  %xmm1,%xmm0
+	jl     2b7f <c_array_var_double+0x26>
+	cvtsi2sdl -0x1c(%rbp),%xmm0
+	movsd  -0x8(%rbp),%xmm1
+	divsd  %xmm0,%xmm1
+	movapd %xmm1,%xmm0
 	leave
 	ret
 
-00000000000036ea <c_array_std_int>:
+0000000000002bdb <c_array_std_int>:
 c_array_std_int():
-	endbr64
 	push   %rbp
 	mov    %rsp,%rbp
 	sub    $0x30,%rsp
 	mov    %rdi,-0x18(%rbp)
 	mov    %esi,-0x1c(%rbp)
 	movsd  %xmm0,-0x28(%rbp)
 	pxor   %xmm0,%xmm0
 	movsd  %xmm0,-0x8(%rbp)
 	movl   $0x0,-0xc(%rbp)
-	jmp    3752 <c_array_std_int+0x68>
+	jmp    2c43 <c_array_std_int+0x68>
 	mov    -0xc(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,4),%rdx
 	mov    -0x18(%rbp),%rax
 	add    %rdx,%rax
 	mov    (%rax),%eax
 	cvtsi2sd %eax,%xmm0
 	subsd  -0x28(%rbp),%xmm0
-	movsd  0x38e5(%rip),%xmm1        
-	call   2550 <pow@plt>
-	movsd  -0x8(%rbp),%xmm1
+	movsd  0x3088(%rip),%xmm1        
+	call   1a20 <pow@plt>
+	movapd %xmm0,%xmm1
+	movsd  -0x8(%rbp),%xmm0
 	addsd  %xmm1,%xmm0
 	movsd  %xmm0,-0x8(%rbp)
 	addl   $0x1,-0xc(%rbp)
 	mov    -0xc(%rbp),%eax
 	cmp    -0x1c(%rbp),%eax
-	jl     3714 <c_array_std_int+0x2a>
-	cvtsi2sdl -0x1c(%rbp),%xmm1
-	movsd  -0x8(%rbp),%xmm0
-	divsd  %xmm1,%xmm0
-	call   2580 <sqrt@plt>
+	jl     2c01 <c_array_std_int+0x26>
+	cvtsi2sdl -0x1c(%rbp),%xmm0
+	movsd  -0x8(%rbp),%xmm1
+	divsd  %xmm0,%xmm1
+	movapd %xmm1,%xmm0
+	call   1a50 <sqrt@plt>
+	movq   %xmm0,%rax
+	mov    %rax,-0x30(%rbp)
+	movsd  -0x30(%rbp),%xmm0
 	leave
 	ret
 
-000000000000376f <c_array_std_long_long>:
+0000000000002c72 <c_array_std_long_long>:
 c_array_std_long_long():
-	endbr64
 	push   %rbp
 	mov    %rsp,%rbp
 	sub    $0x30,%rsp
 	mov    %rdi,-0x18(%rbp)
 	mov    %esi,-0x1c(%rbp)
 	movsd  %xmm0,-0x28(%rbp)
 	pxor   %xmm0,%xmm0
 	movsd  %xmm0,-0x8(%rbp)
 	movl   $0x0,-0xc(%rbp)
-	jmp    37d9 <c_array_std_long_long+0x6a>
+	jmp    2cdc <c_array_std_long_long+0x6a>
 	mov    -0xc(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,8),%rdx
 	mov    -0x18(%rbp),%rax
 	add    %rdx,%rax
 	mov    (%rax),%rax
 	cvtsi2sd %rax,%xmm0
 	subsd  -0x28(%rbp),%xmm0
-	movsd  0x385e(%rip),%xmm1        
-	call   2550 <pow@plt>
-	movsd  -0x8(%rbp),%xmm1
+	movsd  0x2fef(%rip),%xmm1        
+	call   1a20 <pow@plt>
+	movapd %xmm0,%xmm1
+	movsd  -0x8(%rbp),%xmm0
 	addsd  %xmm1,%xmm0
 	movsd  %xmm0,-0x8(%rbp)
 	addl   $0x1,-0xc(%rbp)
 	mov    -0xc(%rbp),%eax
 	cmp    -0x1c(%rbp),%eax
-	jl     3799 <c_array_std_long_long+0x2a>
-	cvtsi2sdl -0x1c(%rbp),%xmm1
-	movsd  -0x8(%rbp),%xmm0
-	divsd  %xmm1,%xmm0
-	call   2580 <sqrt@plt>
+	jl     2c98 <c_array_std_long_long+0x26>
+	cvtsi2sdl -0x1c(%rbp),%xmm0
+	movsd  -0x8(%rbp),%xmm1
+	divsd  %xmm0,%xmm1
+	movapd %xmm1,%xmm0
+	call   1a50 <sqrt@plt>
+	movq   %xmm0,%rax
+	mov    %rax,-0x30(%rbp)
+	movsd  -0x30(%rbp),%xmm0
 	leave
 	ret
 
-00000000000037f6 <c_array_std_float>:
+0000000000002d0b <c_array_std_float>:
 c_array_std_float():
-	endbr64
 	push   %rbp
 	mov    %rsp,%rbp
 	sub    $0x30,%rsp
 	mov    %rdi,-0x18(%rbp)
 	mov    %esi,-0x1c(%rbp)
 	movsd  %xmm0,-0x28(%rbp)
 	pxor   %xmm0,%xmm0
 	movsd  %xmm0,-0x8(%rbp)
 	movl   $0x0,-0xc(%rbp)
-	jmp    3860 <c_array_std_float+0x6a>
+	jmp    2d75 <c_array_std_float+0x6a>
 	mov    -0xc(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,4),%rdx
 	mov    -0x18(%rbp),%rax
 	add    %rdx,%rax
 	movss  (%rax),%xmm0
 	cvtss2sd %xmm0,%xmm0
 	subsd  -0x28(%rbp),%xmm0
-	movsd  0x37d7(%rip),%xmm1        
-	call   2550 <pow@plt>
-	movsd  -0x8(%rbp),%xmm1
+	movsd  0x2f56(%rip),%xmm1        
+	call   1a20 <pow@plt>
+	movapd %xmm0,%xmm1
+	movsd  -0x8(%rbp),%xmm0
 	addsd  %xmm1,%xmm0
 	movsd  %xmm0,-0x8(%rbp)
 	addl   $0x1,-0xc(%rbp)
 	mov    -0xc(%rbp),%eax
 	cmp    -0x1c(%rbp),%eax
-	jl     3820 <c_array_std_float+0x2a>
-	cvtsi2sdl -0x1c(%rbp),%xmm1
-	movsd  -0x8(%rbp),%xmm0
-	divsd  %xmm1,%xmm0
-	call   2580 <sqrt@plt>
+	jl     2d31 <c_array_std_float+0x26>
+	cvtsi2sdl -0x1c(%rbp),%xmm0
+	movsd  -0x8(%rbp),%xmm1
+	divsd  %xmm0,%xmm1
+	movapd %xmm1,%xmm0
+	call   1a50 <sqrt@plt>
+	movq   %xmm0,%rax
+	mov    %rax,-0x30(%rbp)
+	movsd  -0x30(%rbp),%xmm0
 	leave
 	ret
 
-000000000000387d <c_array_std_double>:
+0000000000002da4 <c_array_std_double>:
 c_array_std_double():
-	endbr64
 	push   %rbp
 	mov    %rsp,%rbp
 	sub    $0x30,%rsp
 	mov    %rdi,-0x18(%rbp)
 	mov    %esi,-0x1c(%rbp)
 	movsd  %xmm0,-0x28(%rbp)
 	pxor   %xmm0,%xmm0
 	movsd  %xmm0,-0x8(%rbp)
 	movl   $0x0,-0xc(%rbp)
-	jmp    38e3 <c_array_std_double+0x66>
+	jmp    2e0a <c_array_std_double+0x66>
 	mov    -0xc(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,8),%rdx
 	mov    -0x18(%rbp),%rax
 	add    %rdx,%rax
 	movsd  (%rax),%xmm0
 	subsd  -0x28(%rbp),%xmm0
-	movsd  0x3754(%rip),%xmm1        
-	call   2550 <pow@plt>
-	movsd  -0x8(%rbp),%xmm1
+	movsd  0x2ec1(%rip),%xmm1        
+	call   1a20 <pow@plt>
+	movapd %xmm0,%xmm1
+	movsd  -0x8(%rbp),%xmm0
 	addsd  %xmm1,%xmm0
 	movsd  %xmm0,-0x8(%rbp)
 	addl   $0x1,-0xc(%rbp)
 	mov    -0xc(%rbp),%eax
 	cmp    -0x1c(%rbp),%eax
-	jl     38a7 <c_array_std_double+0x2a>
-	cvtsi2sdl -0x1c(%rbp),%xmm1
-	movsd  -0x8(%rbp),%xmm0
-	divsd  %xmm1,%xmm0
-	call   2580 <sqrt@plt>
+	jl     2dca <c_array_std_double+0x26>
+	cvtsi2sdl -0x1c(%rbp),%xmm0
+	movsd  -0x8(%rbp),%xmm1
+	divsd  %xmm0,%xmm1
+	movapd %xmm1,%xmm0
+	call   1a50 <sqrt@plt>
+	movq   %xmm0,%rax
+	mov    %rax,-0x30(%rbp)
+	movsd  -0x30(%rbp),%xmm0
 	leave
 	ret
 
-0000000000003900 <c_array_mean_int>:
+0000000000002e39 <c_array_mean_int>:
 c_array_mean_int():
-	endbr64
 	push   %rbp
 	mov    %rsp,%rbp
 	mov    %rdi,-0x18(%rbp)
 	mov    %esi,-0x1c(%rbp)
 	mov    %edx,-0x20(%rbp)
 	cvtsi2sdl -0x20(%rbp),%xmm0
 	cvtsi2sdl -0x1c(%rbp),%xmm1
 	divsd  %xmm1,%xmm0
 	movsd  %xmm0,-0x8(%rbp)
 	movsd  -0x8(%rbp),%xmm0
 	pop    %rbp
 	ret
 
-000000000000392c <c_array_mean_long_long>:
+0000000000002e61 <c_array_mean_long_long>:
 c_array_mean_long_long():
-	endbr64
 	push   %rbp
 	mov    %rsp,%rbp
 	mov    %rdi,-0x18(%rbp)
 	mov    %esi,-0x1c(%rbp)
 	mov    %rdx,-0x28(%rbp)
 	cvtsi2sdq -0x28(%rbp),%xmm0
 	cvtsi2sdl -0x1c(%rbp),%xmm1
 	divsd  %xmm1,%xmm0
 	movsd  %xmm0,-0x8(%rbp)
 	movsd  -0x8(%rbp),%xmm0
 	pop    %rbp
 	ret
 
-000000000000395a <c_array_mean_float>:
+0000000000002e8b <c_array_mean_float>:
 c_array_mean_float():
-	endbr64
 	push   %rbp
 	mov    %rsp,%rbp
 	mov    %rdi,-0x18(%rbp)
 	mov    %esi,-0x1c(%rbp)
 	movss  %xmm0,-0x20(%rbp)
 	cvtss2sd -0x20(%rbp),%xmm0
 	cvtsi2sdl -0x1c(%rbp),%xmm1
 	divsd  %xmm1,%xmm0
 	movsd  %xmm0,-0x8(%rbp)
 	movsd  -0x8(%rbp),%xmm0
 	pop    %rbp
 	ret
 
-0000000000003988 <c_array_mean_double>:
+0000000000002eb5 <c_array_mean_double>:
 c_array_mean_double():
-	endbr64
 	push   %rbp
 	mov    %rsp,%rbp
 	mov    %rdi,-0x18(%rbp)
 	mov    %esi,-0x1c(%rbp)
 	movsd  %xmm0,-0x28(%rbp)
-	cvtsi2sdl -0x1c(%rbp),%xmm1
-	movsd  -0x28(%rbp),%xmm0
-	divsd  %xmm1,%xmm0
+	cvtsi2sdl -0x1c(%rbp),%xmm0
+	movsd  -0x28(%rbp),%xmm1
+	divsd  %xmm0,%xmm1
+	movapd %xmm1,%xmm0
 	movsd  %xmm0,-0x8(%rbp)
 	movsd  -0x8(%rbp),%xmm0
 	pop    %rbp
 	ret
 
-00000000000039b6 <c_array_sum_int>:
+0000000000002ee3 <c_array_sum_int>:
 c_array_sum_int():
-	endbr64
 	push   %rbp
 	mov    %rsp,%rbp
 	mov    %rdi,-0x18(%rbp)
 	mov    %esi,-0x1c(%rbp)
 	movl   $0x0,-0x8(%rbp)
 	movl   $0x0,-0x4(%rbp)
-	jmp    39f2 <c_array_sum_int+0x3c>
+	jmp    2f1b <c_array_sum_int+0x38>
 	mov    -0x4(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,4),%rdx
 	mov    -0x18(%rbp),%rax
 	add    %rdx,%rax
 	mov    (%rax),%eax
 	add    %eax,-0x8(%rbp)
 	addl   $0x1,-0x4(%rbp)
 	mov    -0x4(%rbp),%eax
 	cmp    -0x1c(%rbp),%eax
-	jl     39d5 <c_array_sum_int+0x1f>
+	jl     2efe <c_array_sum_int+0x1b>
 	mov    -0x8(%rbp),%eax
 	pop    %rbp
 	ret
 
-00000000000039ff <c_array_sum_long>:
+0000000000002f28 <c_array_sum_long>:
 c_array_sum_long():
-	endbr64
 	push   %rbp
 	mov    %rsp,%rbp
 	mov    %rdi,-0x18(%rbp)
 	mov    %esi,-0x1c(%rbp)
 	movq   $0x0,-0x8(%rbp)
 	movl   $0x0,-0xc(%rbp)
-	jmp    3a3e <c_array_sum_long+0x3f>
+	jmp    2f63 <c_array_sum_long+0x3b>
 	mov    -0xc(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,8),%rdx
 	mov    -0x18(%rbp),%rax
 	add    %rdx,%rax
 	mov    (%rax),%rax
 	add    %rax,-0x8(%rbp)
 	addl   $0x1,-0xc(%rbp)
 	mov    -0xc(%rbp),%eax
 	cmp    -0x1c(%rbp),%eax
-	jl     3a1f <c_array_sum_long+0x20>
+	jl     2f44 <c_array_sum_long+0x1c>
 	mov    -0x8(%rbp),%rax
 	pop    %rbp
 	ret
 
-0000000000003a4c <c_array_sum_float>:
+0000000000002f71 <c_array_sum_float>:
 c_array_sum_float():
-	endbr64
 	push   %rbp
 	mov    %rsp,%rbp
 	mov    %rdi,-0x18(%rbp)
 	mov    %esi,-0x1c(%rbp)
 	pxor   %xmm0,%xmm0
 	movss  %xmm0,-0x8(%rbp)
 	movl   $0x0,-0x4(%rbp)
-	jmp    3a97 <c_array_sum_float+0x4b>
+	jmp    2fb8 <c_array_sum_float+0x47>
 	mov    -0x4(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,4),%rdx
 	mov    -0x18(%rbp),%rax
 	add    %rdx,%rax
 	movss  (%rax),%xmm0
 	movss  -0x8(%rbp),%xmm1
 	addss  %xmm1,%xmm0
 	movss  %xmm0,-0x8(%rbp)
 	addl   $0x1,-0x4(%rbp)
 	mov    -0x4(%rbp),%eax
 	cmp    -0x1c(%rbp),%eax
-	jl     3a6d <c_array_sum_float+0x21>
+	jl     2f8e <c_array_sum_float+0x1d>
 	movss  -0x8(%rbp),%xmm0
 	pop    %rbp
 	ret
 
-0000000000003aa6 <c_array_sum_double>:
+0000000000002fc7 <c_array_sum_double>:
 c_array_sum_double():
-	endbr64
 	push   %rbp
 	mov    %rsp,%rbp
 	mov    %rdi,-0x18(%rbp)
 	mov    %esi,-0x1c(%rbp)
 	pxor   %xmm0,%xmm0
 	movsd  %xmm0,-0x8(%rbp)
 	movl   $0x0,-0xc(%rbp)
-	jmp    3af1 <c_array_sum_double+0x4b>
+	jmp    300e <c_array_sum_double+0x47>
 	mov    -0xc(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,8),%rdx
 	mov    -0x18(%rbp),%rax
 	add    %rdx,%rax
 	movsd  (%rax),%xmm0
 	movsd  -0x8(%rbp),%xmm1
 	addsd  %xmm1,%xmm0
 	movsd  %xmm0,-0x8(%rbp)
 	addl   $0x1,-0xc(%rbp)
 	mov    -0xc(%rbp),%eax
 	cmp    -0x1c(%rbp),%eax
-	jl     3ac7 <c_array_sum_double+0x21>
+	jl     2fe4 <c_array_sum_double+0x1d>
 	movsd  -0x8(%rbp),%xmm0
 	pop    %rbp
 	ret
 
-0000000000003b00 <cmpfunc_int>:
+000000000000301d <cmpfunc_int>:
 cmpfunc_int():
-	endbr64
 	push   %rbp
 	mov    %rsp,%rbp
 	mov    %rdi,-0x8(%rbp)
 	mov    %rsi,-0x10(%rbp)
 	mov    -0x8(%rbp),%rax
 	mov    (%rax),%edx
 	mov    -0x10(%rbp),%rax
 	mov    (%rax),%eax
 	sub    %eax,%edx
 	mov    %edx,%eax
 	pop    %rbp
 	ret
 
-0000000000003b22 <cmpfunc_long>:
+000000000000303b <cmpfunc_long>:
 cmpfunc_long():
-	endbr64
 	push   %rbp
 	mov    %rsp,%rbp
 	mov    %rdi,-0x8(%rbp)
 	mov    %rsi,-0x10(%rbp)
 	mov    -0x8(%rbp),%rax
 	mov    (%rax),%rax
 	mov    %eax,%edx
 	mov    -0x10(%rbp),%rax
 	mov    (%rax),%rax
 	sub    %eax,%edx
 	mov    %edx,%eax
 	pop    %rbp
 	ret
 
-0000000000003b48 <cmpfunc_float>:
+000000000000305d <cmpfunc_float>:
 cmpfunc_float():
-	endbr64
 	push   %rbp
 	mov    %rsp,%rbp
 	mov    %rdi,-0x18(%rbp)
 	mov    %rsi,-0x20(%rbp)
 	mov    -0x18(%rbp),%rax
 	movss  (%rax),%xmm0
 	mov    -0x20(%rbp),%rax
 	movss  (%rax),%xmm1
 	subss  %xmm1,%xmm0
 	movss  %xmm0,-0x4(%rbp)
 	movss  -0x4(%rbp),%xmm0
 	pxor   %xmm1,%xmm1
-	comiss %xmm1,%xmm0
-	jbe    3b86 <cmpfunc_float+0x3e>
+	ucomiss %xmm1,%xmm0
+	jbe    3097 <cmpfunc_float+0x3a>
 	mov    $0x1,%eax
-	jmp    3b9c <cmpfunc_float+0x54>
+	jmp    30ad <cmpfunc_float+0x50>
 	pxor   %xmm0,%xmm0
-	comiss -0x4(%rbp),%xmm0
-	jbe    3b97 <cmpfunc_float+0x4f>
+	ucomiss -0x4(%rbp),%xmm0
+	jbe    30a8 <cmpfunc_float+0x4b>
 	mov    $0xffffffff,%eax
-	jmp    3b9c <cmpfunc_float+0x54>
+	jmp    30ad <cmpfunc_float+0x50>
 	mov    $0x0,%eax
 	pop    %rbp
 	ret
 
-0000000000003b9e <cmpfunc_double>:
+00000000000030af <cmpfunc_double>:
 cmpfunc_double():
-	endbr64
 	push   %rbp
 	mov    %rsp,%rbp
 	mov    %rdi,-0x18(%rbp)
 	mov    %rsi,-0x20(%rbp)
 	mov    -0x18(%rbp),%rax
 	movsd  (%rax),%xmm0
 	mov    -0x20(%rbp),%rax
 	movsd  (%rax),%xmm1
 	subsd  %xmm1,%xmm0
 	movsd  %xmm0,-0x8(%rbp)
 	movsd  -0x8(%rbp),%xmm0
 	pxor   %xmm1,%xmm1
-	comisd %xmm1,%xmm0
-	jbe    3bdd <cmpfunc_double+0x3f>
+	ucomisd %xmm1,%xmm0
+	jbe    30ea <cmpfunc_double+0x3b>
 	mov    $0x1,%eax
-	jmp    3bf4 <cmpfunc_double+0x56>
+	jmp    3101 <cmpfunc_double+0x52>
 	pxor   %xmm0,%xmm0
-	comisd -0x8(%rbp),%xmm0
-	jbe    3bef <cmpfunc_double+0x51>
+	ucomisd -0x8(%rbp),%xmm0
+	jbe    30fc <cmpfunc_double+0x4d>
 	mov    $0xffffffff,%eax
-	jmp    3bf4 <cmpfunc_double+0x56>
+	jmp    3101 <cmpfunc_double+0x52>
 	mov    $0x0,%eax
 	pop    %rbp
 	ret
 
-0000000000003bf6 <mt19937_init>:
+0000000000003103 <mt19937_init>:
 mt19937_init():
-	endbr64
 	push   %rbp
 	mov    %rsp,%rbp
 	mov    %rdi,-0x18(%rbp)
 	mov    %esi,-0x1c(%rbp)
 	mov    -0x18(%rbp),%rax
 	mov    -0x1c(%rbp),%edx
 	mov    %edx,(%rax)
 	movl   $0x1,-0x4(%rbp)
-	jmp    3c59 <mt19937_init+0x63>
+	jmp    3162 <mt19937_init+0x5f>
 	mov    -0x4(%rbp),%eax
 	lea    -0x1(%rax),%edx
 	mov    -0x18(%rbp),%rax
 	movslq %edx,%rdx
 	mov    (%rax,%rdx,4),%ecx
 	mov    -0x4(%rbp),%eax
 	lea    -0x1(%rax),%edx
@@ -1630,33 +1641,32 @@
 	lea    (%rdx,%rax,1),%ecx
 	mov    -0x18(%rbp),%rax
 	mov    -0x4(%rbp),%edx
 	movslq %edx,%rdx
 	mov    %ecx,(%rax,%rdx,4)
 	addl   $0x1,-0x4(%rbp)
 	cmpl   $0x26f,-0x4(%rbp)
-	jle    3c17 <mt19937_init+0x21>
+	jle    3120 <mt19937_init+0x1d>
 	mov    -0x18(%rbp),%rax
 	movl   $0x270,0x9c0(%rax)
 	nop
 	pop    %rbp
 	ret
 
-0000000000003c73 <mt19937_generate>:
+000000000000317c <mt19937_generate>:
 mt19937_generate():
-	endbr64
 	push   %rbp
 	mov    %rsp,%rbp
 	mov    %rdi,-0x38(%rbp)
 	mov    -0x38(%rbp),%rax
 	mov    0x9c0(%rax),%eax
 	cmp    $0x26f,%eax
-	jle    3df4 <mt19937_generate+0x181>
+	jle    32f9 <mt19937_generate+0x17d>
 	movl   $0x0,-0x28(%rbp)
-	jmp    3d0c <mt19937_generate+0x99>
+	jmp    3211 <mt19937_generate+0x95>
 	mov    -0x38(%rbp),%rax
 	mov    -0x28(%rbp),%edx
 	movslq %edx,%rdx
 	mov    (%rax,%rdx,4),%eax
 	and    $0x80000000,%eax
 	mov    %eax,%ecx
 	mov    -0x28(%rbp),%eax
@@ -1683,17 +1693,17 @@
 	xor    %eax,%ecx
 	mov    -0x38(%rbp),%rax
 	mov    -0x28(%rbp),%edx
 	movslq %edx,%rdx
 	mov    %ecx,(%rax,%rdx,4)
 	addl   $0x1,-0x28(%rbp)
 	cmpl   $0xe2,-0x28(%rbp)
-	jle    3c9d <mt19937_generate+0x2a>
+	jle    31a2 <mt19937_generate+0x26>
 	movl   $0xe3,-0x24(%rbp)
-	jmp    3d8d <mt19937_generate+0x11a>
+	jmp    3292 <mt19937_generate+0x116>
 	mov    -0x38(%rbp),%rax
 	mov    -0x24(%rbp),%edx
 	movslq %edx,%rdx
 	mov    (%rax,%rdx,4),%eax
 	and    $0x80000000,%eax
 	mov    %eax,%ecx
 	mov    -0x24(%rbp),%eax
@@ -1720,15 +1730,15 @@
 	xor    %eax,%ecx
 	mov    -0x38(%rbp),%rax
 	mov    -0x24(%rbp),%edx
 	movslq %edx,%rdx
 	mov    %ecx,(%rax,%rdx,4)
 	addl   $0x1,-0x24(%rbp)
 	cmpl   $0x26e,-0x24(%rbp)
-	jle    3d1e <mt19937_generate+0xab>
+	jle    3223 <mt19937_generate+0xa7>
 	mov    -0x38(%rbp),%rax
 	mov    0x9bc(%rax),%eax
 	and    $0x80000000,%eax
 	mov    %eax,%edx
 	mov    -0x38(%rbp),%rax
 	mov    (%rax),%eax
 	and    $0x7fffffff,%eax
@@ -1772,197 +1782,195 @@
 	mov    -0x8(%rbp),%rax
 	shr    $0x12,%rax
 	xor    %rax,-0x8(%rbp)
 	mov    -0x8(%rbp),%rax
 	pop    %rbp
 	ret
 
-0000000000003e5a <mt19937_get_int32_range>:
+000000000000335f <mt19937_get_int32_range>:
 mt19937_get_int32_range():
-	endbr64
 	push   %rbp
 	mov    %rsp,%rbp
 	sub    $0x10,%rsp
 	mov    %rdi,-0x8(%rbp)
 	mov    %esi,-0xc(%rbp)
 	mov    %edx,-0x10(%rbp)
 	mov    -0x8(%rbp),%rax
 	mov    %rax,%rdi
-	call   2440 <mt19937_generate@plt>
-	mov    -0x10(%rbp),%edx
-	sub    -0xc(%rbp),%edx
-	add    $0x1,%edx
-	movslq %edx,%rcx
+	call   1910 <mt19937_generate@plt>
+	mov    %rax,%rdx
+	mov    -0x10(%rbp),%eax
+	sub    -0xc(%rbp),%eax
+	add    $0x1,%eax
+	movslq %eax,%rcx
+	mov    %rdx,%rax
 	mov    $0x0,%edx
 	div    %rcx
 	mov    %rdx,%rax
 	mov    %eax,%edx
 	mov    -0xc(%rbp),%eax
 	add    %edx,%eax
 	leave
 	ret
 
-0000000000003e9c <mt19937_get_float>:
+00000000000033a3 <mt19937_get_float>:
 mt19937_get_float():
-	endbr64
 	push   %rbp
 	mov    %rsp,%rbp
 	sub    $0x10,%rsp
 	mov    %rdi,-0x8(%rbp)
 	mov    -0x8(%rbp),%rax
 	mov    %rax,%rdi
-	call   2440 <mt19937_generate@plt>
+	call   1910 <mt19937_generate@plt>
 	test   %rax,%rax
-	js     3ec4 <mt19937_get_float+0x28>
+	js     33c7 <mt19937_get_float+0x24>
 	cvtsi2ss %rax,%xmm0
-	jmp    3ed9 <mt19937_get_float+0x3d>
+	jmp    33dc <mt19937_get_float+0x39>
 	mov    %rax,%rdx
 	shr    %rdx
 	and    $0x1,%eax
 	or     %rax,%rdx
 	cvtsi2ss %rdx,%xmm0
 	addss  %xmm0,%xmm0
-	movss  0x3147(%rip),%xmm1        
+	movss  0x28d4(%rip),%xmm1        
 	divss  %xmm1,%xmm0
 	leave
 	ret
 
-0000000000003ee7 <mt19937_get_float_range>:
+00000000000033ea <mt19937_get_float_range>:
 mt19937_get_float_range():
-	endbr64
 	push   %rbp
 	mov    %rsp,%rbp
 	sub    $0x10,%rsp
 	mov    %rdi,-0x8(%rbp)
 	movss  %xmm0,-0xc(%rbp)
 	movss  %xmm1,-0x10(%rbp)
 	mov    -0x8(%rbp),%rax
 	mov    %rax,%rdi
-	call   2440 <mt19937_generate@plt>
+	call   1910 <mt19937_generate@plt>
 	test   %rax,%rax
-	js     3f19 <mt19937_get_float_range+0x32>
+	js     3418 <mt19937_get_float_range+0x2e>
 	cvtsi2ss %rax,%xmm0
-	jmp    3f2e <mt19937_get_float_range+0x47>
+	jmp    342d <mt19937_get_float_range+0x43>
 	mov    %rax,%rdx
 	shr    %rdx
 	and    $0x1,%eax
 	or     %rax,%rdx
 	cvtsi2ss %rdx,%xmm0
 	addss  %xmm0,%xmm0
-	movss  0x30f2(%rip),%xmm1        
+	movss  0x2883(%rip),%xmm1        
 	divss  %xmm1,%xmm0
 	movaps %xmm0,%xmm1
 	movss  -0x10(%rbp),%xmm0
 	subss  -0xc(%rbp),%xmm0
 	mulss  %xmm1,%xmm0
 	addss  -0xc(%rbp),%xmm0
 	leave
 	ret
 
-0000000000003f52 <mt19937_get_double>:
+0000000000003451 <mt19937_get_double>:
 mt19937_get_double():
-	endbr64
 	push   %rbp
 	mov    %rsp,%rbp
 	sub    $0x10,%rsp
 	mov    %rdi,-0x8(%rbp)
 	mov    -0x8(%rbp),%rax
 	mov    %rax,%rdi
-	call   2440 <mt19937_generate@plt>
+	call   1910 <mt19937_generate@plt>
 	test   %rax,%rax
-	js     3f7a <mt19937_get_double+0x28>
+	js     3475 <mt19937_get_double+0x24>
 	cvtsi2sd %rax,%xmm0
-	jmp    3f8f <mt19937_get_double+0x3d>
+	jmp    348a <mt19937_get_double+0x39>
 	mov    %rax,%rdx
 	shr    %rdx
 	and    $0x1,%eax
 	or     %rax,%rdx
 	cvtsi2sd %rdx,%xmm0
 	addsd  %xmm0,%xmm0
-	movsd  0x3099(%rip),%xmm1        
+	movsd  0x282e(%rip),%xmm1        
 	divsd  %xmm1,%xmm0
 	leave
 	ret
 
-0000000000003f9d <mt19937_get_double_range>:
+0000000000003498 <mt19937_get_double_range>:
 mt19937_get_double_range():
-	endbr64
 	push   %rbp
 	mov    %rsp,%rbp
 	sub    $0x20,%rsp
 	mov    %rdi,-0x8(%rbp)
 	movsd  %xmm0,-0x10(%rbp)
 	movsd  %xmm1,-0x18(%rbp)
 	mov    -0x8(%rbp),%rax
 	mov    %rax,%rdi
-	call   2440 <mt19937_generate@plt>
+	call   1910 <mt19937_generate@plt>
 	test   %rax,%rax
-	js     3fcf <mt19937_get_double_range+0x32>
+	js     34c6 <mt19937_get_double_range+0x2e>
 	cvtsi2sd %rax,%xmm0
-	jmp    3fe4 <mt19937_get_double_range+0x47>
+	jmp    34db <mt19937_get_double_range+0x43>
 	mov    %rax,%rdx
 	shr    %rdx
 	and    $0x1,%eax
 	or     %rax,%rdx
 	cvtsi2sd %rdx,%xmm0
 	addsd  %xmm0,%xmm0
-	movsd  0x3044(%rip),%xmm1        
+	movsd  0x27dd(%rip),%xmm1        
 	divsd  %xmm1,%xmm0
 	movapd %xmm0,%xmm1
 	movsd  -0x18(%rbp),%xmm0
 	subsd  -0x10(%rbp),%xmm0
 	mulsd  %xmm1,%xmm0
 	addsd  -0x10(%rbp),%xmm0
 	leave
 	ret
 
-0000000000004009 <mt19937_random_normal>:
+0000000000003500 <mt19937_random_normal>:
 mt19937_random_normal():
-	endbr64
 	push   %rbp
 	mov    %rsp,%rbp
 	sub    $0x30,%rsp
 	mov    %rdi,-0x28(%rbp)
 	mov    -0x28(%rbp),%rax
 	mov    %rax,%rdi
-	call   2540 <mt19937_get_double@plt>
+	call   1a10 <mt19937_get_double@plt>
 	movq   %xmm0,%rax
 	mov    %rax,-0x18(%rbp)
 	mov    -0x28(%rbp),%rax
 	mov    %rax,%rdi
-	call   2540 <mt19937_get_double@plt>
+	call   1a10 <mt19937_get_double@plt>
 	movq   %xmm0,%rax
 	mov    %rax,-0x10(%rbp)
 	mov    -0x18(%rbp),%rax
-	movq   %rax,%xmm0
-	call   2520 <log@plt>
-	movsd  0x2fdf(%rip),%xmm1        
+	mov    %rax,-0x30(%rbp)
+	movsd  -0x30(%rbp),%xmm0
+	call   19f0 <log@plt>
+	movapd %xmm0,%xmm1
+	movsd  0x2774(%rip),%xmm0        
 	mulsd  %xmm1,%xmm0
-	call   2580 <sqrt@plt>
+	call   1a50 <sqrt@plt>
 	movsd  %xmm0,-0x30(%rbp)
 	movsd  -0x10(%rbp),%xmm1
-	movsd  0x2fcc(%rip),%xmm0        
+	movsd  0x2761(%rip),%xmm0        
 	mulsd  %xmm1,%xmm0
-	call   2500 <cos@plt>
+	call   19d0 <cos@plt>
 	mulsd  -0x30(%rbp),%xmm0
 	movsd  %xmm0,-0x8(%rbp)
 	movsd  -0x8(%rbp),%xmm0
 	leave
 	ret
 
-000000000000408e <cov_model_init>:
+0000000000003589 <cov_model_init>:
 cov_model_init():
-	endbr64
 	push   %rbp
 	mov    %rsp,%rbp
 	mov    %rdi,-0x8(%rbp)
 	mov    %esi,-0xc(%rbp)
 	mov    %edx,-0x10(%rbp)
 	movsd  %xmm0,-0x18(%rbp)
 	movsd  %xmm1,-0x20(%rbp)
+	movsd  %xmm2,-0x28(%rbp)
 	mov    -0x8(%rbp),%rax
 	mov    -0xc(%rbp),%edx
 	mov    %edx,(%rax)
 	mov    -0x8(%rbp),%rax
 	mov    -0x10(%rbp),%edx
 	mov    %edx,0x4(%rax)
 	mov    -0xc(%rbp),%eax
@@ -1973,151 +1981,175 @@
 	mov    %edx,0x8(%rax)
 	mov    -0x8(%rbp),%rax
 	movsd  -0x18(%rbp),%xmm0
 	movsd  %xmm0,0x10(%rax)
 	mov    -0x8(%rbp),%rax
 	movsd  -0x20(%rbp),%xmm0
 	movsd  %xmm0,0x18(%rax)
+	mov    -0x8(%rbp),%rax
+	movsd  -0x28(%rbp),%xmm0
+	movsd  %xmm0,0x20(%rax)
 	nop
 	pop    %rbp
 	ret
 
-00000000000040ec <cov_model>:
+00000000000035f6 <cov_model>:
 cov_model():
-	endbr64
 	push   %rbp
 	mov    %rsp,%rbp
 	sub    $0x40,%rsp
-	mov    %rdi,-0x18(%rbp)
-	mov    %rsi,-0x20(%rbp)
-	mov    %edx,-0x24(%rbp)
-	movsd  %xmm0,-0x30(%rbp)
-	movsd  %xmm1,-0x38(%rbp)
-	movl   $0x0,-0x4(%rbp)
-	jmp    41ad <cov_model+0xc1>
-	mov    -0x4(%rbp),%eax
+	mov    %rdi,-0x28(%rbp)
+	mov    %rsi,-0x30(%rbp)
+	mov    %edx,-0x34(%rbp)
+	mov    %rcx,-0x40(%rbp)
+	mov    -0x40(%rbp),%rax
+	movsd  0x18(%rax),%xmm0
+	mov    -0x40(%rbp),%rax
+	movsd  0x20(%rax),%xmm1
+	subsd  %xmm1,%xmm0
+	movsd  %xmm0,-0x10(%rbp)
+	movl   $0x0,-0x14(%rbp)
+	jmp    36ec <cov_model+0xf6>
+	mov    -0x14(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,8),%rdx
-	mov    -0x18(%rbp),%rax
+	mov    -0x28(%rbp),%rax
 	add    %rdx,%rax
 	movsd  (%rax),%xmm1
-	mov    -0x4(%rbp),%eax
+	mov    -0x14(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,8),%rdx
-	mov    -0x18(%rbp),%rax
+	mov    -0x28(%rbp),%rax
 	add    %rdx,%rax
 	movsd  (%rax),%xmm0
-	mulsd  %xmm0,%xmm1
-	movsd  0x2ef3(%rip),%xmm0        
-	mulsd  %xmm0,%xmm1
-	movsd  -0x30(%rbp),%xmm0
-	mulsd  %xmm0,%xmm0
-	divsd  %xmm0,%xmm1
-	movapd %xmm1,%xmm0
-	call   24e0 <exp@plt>
-	movsd  0x2ed9(%rip),%xmm1        
+	mulsd  %xmm1,%xmm0
+	movsd  0x2668(%rip),%xmm1        
+	mulsd  %xmm1,%xmm0
+	mov    -0x40(%rbp),%rax
+	movsd  0x10(%rax),%xmm2
+	mov    -0x40(%rbp),%rax
+	movsd  0x10(%rax),%xmm1
+	mulsd  %xmm2,%xmm1
+	divsd  %xmm1,%xmm0
+	call   19b0 <exp@plt>
+	movapd %xmm0,%xmm1
+	movsd  0x2641(%rip),%xmm0        
+	subsd  %xmm1,%xmm0
+	movsd  %xmm0,-0x8(%rbp)
+	mov    -0x40(%rbp),%rax
+	movsd  0x18(%rax),%xmm1
+	movsd  -0x10(%rbp),%xmm0
+	mulsd  -0x8(%rbp),%xmm0
 	subsd  %xmm0,%xmm1
 	movapd %xmm1,%xmm0
-	movapd %xmm0,%xmm1
-	mulsd  -0x38(%rbp),%xmm1
-	mov    -0x4(%rbp),%eax
+	mov    -0x40(%rbp),%rax
+	movsd  0x20(%rax),%xmm1
+	mov    -0x14(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,8),%rdx
-	mov    -0x20(%rbp),%rax
+	mov    -0x30(%rbp),%rax
 	add    %rdx,%rax
-	movsd  -0x38(%rbp),%xmm0
-	subsd  %xmm1,%xmm0
+	addsd  %xmm1,%xmm0
 	movsd  %xmm0,(%rax)
-	addl   $0x1,-0x4(%rbp)
-	mov    -0x4(%rbp),%eax
-	cmp    -0x24(%rbp),%eax
-	jl     4119 <cov_model+0x2d>
-	nop
+	addl   $0x1,-0x14(%rbp)
+	mov    -0x14(%rbp),%eax
+	cmp    -0x34(%rbp),%eax
+	jl     3634 <cov_model+0x3e>
 	nop
 	leave
 	ret
 
-00000000000041bd <cov_model2d>:
+00000000000036fb <cov_model2d>:
 cov_model2d():
-	endbr64
 	push   %rbp
 	mov    %rsp,%rbp
 	sub    $0x40,%rsp
-	mov    %rdi,-0x18(%rbp)
-	mov    %rsi,-0x20(%rbp)
-	mov    %edx,-0x24(%rbp)
-	movsd  %xmm0,-0x30(%rbp)
-	movsd  %xmm1,-0x38(%rbp)
-	movl   $0x0,-0x8(%rbp)
-	jmp    42c5 <cov_model2d+0x108>
-	movl   $0x0,-0x4(%rbp)
-	jmp    42b5 <cov_model2d+0xf8>
-	mov    -0x8(%rbp),%eax
+	mov    %rdi,-0x28(%rbp)
+	mov    %rsi,-0x30(%rbp)
+	mov    %edx,-0x34(%rbp)
+	mov    %rcx,-0x40(%rbp)
+	mov    -0x40(%rbp),%rax
+	movsd  0x18(%rax),%xmm0
+	mov    -0x40(%rbp),%rax
+	movsd  0x20(%rax),%xmm1
+	subsd  %xmm1,%xmm0
+	movsd  %xmm0,-0x10(%rbp)
+	movl   $0x0,-0x18(%rbp)
+	jmp    3838 <cov_model2d+0x13d>
+	movl   $0x0,-0x14(%rbp)
+	jmp    3828 <cov_model2d+0x12d>
+	mov    -0x18(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,8),%rdx
-	mov    -0x18(%rbp),%rax
+	mov    -0x28(%rbp),%rax
 	add    %rdx,%rax
 	mov    (%rax),%rax
-	mov    -0x4(%rbp),%edx
+	mov    -0x14(%rbp),%edx
 	movslq %edx,%rdx
 	shl    $0x3,%rdx
 	add    %rdx,%rax
 	movsd  (%rax),%xmm1
-	mov    -0x8(%rbp),%eax
+	mov    -0x18(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,8),%rdx
-	mov    -0x18(%rbp),%rax
+	mov    -0x28(%rbp),%rax
 	add    %rdx,%rax
 	mov    (%rax),%rax
-	mov    -0x4(%rbp),%edx
+	mov    -0x14(%rbp),%edx
 	movslq %edx,%rdx
 	shl    $0x3,%rdx
 	add    %rdx,%rax
 	movsd  (%rax),%xmm0
-	mulsd  %xmm0,%xmm1
-	movsd  0x2df6(%rip),%xmm0        
-	mulsd  %xmm0,%xmm1
-	movsd  -0x30(%rbp),%xmm0
-	mulsd  %xmm0,%xmm0
-	divsd  %xmm0,%xmm1
-	movapd %xmm1,%xmm0
-	call   24e0 <exp@plt>
-	movsd  0x2ddc(%rip),%xmm1        
+	mulsd  %xmm1,%xmm0
+	movsd  0x2537(%rip),%xmm1        
+	mulsd  %xmm1,%xmm0
+	mov    -0x40(%rbp),%rax
+	movsd  0x10(%rax),%xmm2
+	mov    -0x40(%rbp),%rax
+	movsd  0x10(%rax),%xmm1
+	mulsd  %xmm2,%xmm1
+	divsd  %xmm1,%xmm0
+	call   19b0 <exp@plt>
+	movapd %xmm0,%xmm1
+	movsd  0x2510(%rip),%xmm0        
+	subsd  %xmm1,%xmm0
+	movsd  %xmm0,-0x8(%rbp)
+	mov    -0x40(%rbp),%rax
+	movsd  0x18(%rax),%xmm1
+	movsd  -0x10(%rbp),%xmm0
+	mulsd  -0x8(%rbp),%xmm0
 	subsd  %xmm0,%xmm1
 	movapd %xmm1,%xmm0
-	movapd %xmm0,%xmm1
-	mulsd  -0x38(%rbp),%xmm1
-	mov    -0x24(%rbp),%eax
-	imul   -0x8(%rbp),%eax
+	mov    -0x40(%rbp),%rax
+	movsd  0x20(%rax),%xmm1
+	mov    -0x34(%rbp),%eax
+	imul   -0x18(%rbp),%eax
 	mov    %eax,%edx
-	mov    -0x4(%rbp),%eax
+	mov    -0x14(%rbp),%eax
 	add    %edx,%eax
 	cltq
 	lea    0x0(,%rax,8),%rdx
-	mov    -0x20(%rbp),%rax
+	mov    -0x30(%rbp),%rax
 	add    %rdx,%rax
-	movsd  -0x38(%rbp),%xmm0
-	subsd  %xmm1,%xmm0
+	addsd  %xmm1,%xmm0
 	movsd  %xmm0,(%rax)
-	addl   $0x1,-0x4(%rbp)
-	mov    -0x4(%rbp),%eax
-	cmp    -0x24(%rbp),%eax
-	jl     41f6 <cov_model2d+0x39>
-	addl   $0x1,-0x8(%rbp)
-	mov    -0x8(%rbp),%eax
-	cmp    -0x24(%rbp),%eax
-	jl     41ea <cov_model2d+0x2d>
-	nop
+	addl   $0x1,-0x14(%rbp)
+	mov    -0x14(%rbp),%eax
+	cmp    -0x34(%rbp),%eax
+	jl     3745 <cov_model2d+0x4a>
+	addl   $0x1,-0x18(%rbp)
+	mov    -0x18(%rbp),%eax
+	cmp    -0x34(%rbp),%eax
+	jl     3739 <cov_model2d+0x3e>
 	nop
 	leave
 	ret
 
-00000000000042d5 <sampling_state_init>:
+0000000000003847 <sampling_state_init>:
 sampling_state_init():
-	endbr64
 	push   %rbp
 	mov    %rsp,%rbp
 	sub    $0x10,%rsp
 	mov    %rdi,-0x8(%rbp)
 	mov    %esi,-0xc(%rbp)
 	mov    -0x8(%rbp),%rax
 	movl   $0x0,(%rax)
@@ -2136,15 +2168,15 @@
 	movslq %eax,%rdx
 	mov    -0x8(%rbp),%rax
 	mov    %rdx,0x28(%rax)
 	mov    -0xc(%rbp),%eax
 	cltq
 	mov    $0x8,%esi
 	mov    %rax,%rdi
-	call   2460 <calloc@plt>
+	call   1930 <calloc@plt>
 	mov    %rax,%rdx
 	mov    -0x8(%rbp),%rax
 	mov    %rdx,0x18(%rax)
 	mov    -0xc(%rbp),%eax
 	movslq %eax,%rdx
 	mov    -0x8(%rbp),%rax
 	mov    %rdx,0x38(%rax)
@@ -2152,25 +2184,24 @@
 	movslq %eax,%rdx
 	mov    -0x8(%rbp),%rax
 	mov    %rdx,0x40(%rax)
 	mov    -0xc(%rbp),%eax
 	cltq
 	mov    $0x8,%esi
 	mov    %rax,%rdi
-	call   2460 <calloc@plt>
+	call   1930 <calloc@plt>
 	mov    %rax,%rdx
 	mov    -0x8(%rbp),%rax
 	mov    %rdx,0x30(%rax)
 	nop
 	leave
 	ret
 
-000000000000438a <sampling_state_update>:
+00000000000038f8 <sampling_state_update>:
 sampling_state_update():
-	endbr64
 	push   %rbp
 	mov    %rsp,%rbp
 	mov    %rdi,-0x8(%rbp)
 	movsd  %xmm0,-0x10(%rbp)
 	mov    %esi,-0x14(%rbp)
 	mov    -0x8(%rbp),%rax
 	movsd  -0x10(%rbp),%xmm0
@@ -2178,151 +2209,155 @@
 	mov    -0x8(%rbp),%rax
 	mov    -0x14(%rbp),%edx
 	mov    %edx,0x8(%rax)
 	nop
 	pop    %rbp
 	ret
 
-00000000000043b9 <krige_param_setting>:
+0000000000003923 <krige_param_setting>:
 krige_param_setting():
-	endbr64
 	push   %rbp
 	mov    %rsp,%rbp
 	push   %rbx
 	sub    $0x28,%rsp
-	movsd  %xmm0,-0x28(%rbp)
-	movsd  %xmm1,-0x30(%rbp)
-	movsd  -0x28(%rbp),%xmm0
-	movsd  %xmm0,0x4db3(%rip)        
-	movsd  -0x30(%rbp),%xmm0
-	movsd  %xmm0,0x4dae(%rip)        
-	movq   $0xa,0x4dd3(%rip)        
-	movq   $0xa,0x4dd0(%rip)        
+	mov    %edi,-0x24(%rbp)
+	mov    %rsi,-0x30(%rbp)
+	mov    -0x30(%rbp),%rax
+	mov    %rax,0x203852(%rip)        
+	mov    -0x30(%rbp),%rax
+	movsd  0x10(%rax),%xmm0
+	movsd  %xmm0,0x203849(%rip)        
+	movq   $0xa,0x20386e(%rip)        
+	movq   $0xa,0x20386b(%rip)        
 	mov    $0x8,%esi
 	mov    $0xa,%edi
-	call   2460 <calloc@plt>
-	mov    %rax,0x4daa(%rip)        
-	movq   $0xa,0x4dc7(%rip)        
-	movq   $0xa,0x4dc4(%rip)        
+	call   1930 <calloc@plt>
+	mov    %rax,0x203845(%rip)        
+	movq   $0xa,0x203862(%rip)        
+	movq   $0xa,0x20385f(%rip)        
 	mov    $0x8,%esi
 	mov    $0xa,%edi
-	call   2460 <calloc@plt>
-	mov    %rax,0x4d9e(%rip)        
-	movq   $0xa,0x4ddb(%rip)        
-	movq   $0xa,0x4dd8(%rip)        
+	call   1930 <calloc@plt>
+	mov    %rax,0x203839(%rip)        
+	movq   $0xa,0x203876(%rip)        
+	movq   $0xa,0x203873(%rip)        
 	mov    $0x8,%esi
 	mov    $0xa,%edi
-	call   2460 <calloc@plt>
-	mov    %rax,0x4db2(%rip)        
-	movq   $0xa,0x4def(%rip)        
-	movq   $0xa,0x4dec(%rip)        
+	call   1930 <calloc@plt>
+	mov    %rax,0x20384d(%rip)        
+	movq   $0xa,0x20388a(%rip)        
+	movq   $0xa,0x203887(%rip)        
 	mov    $0x8,%esi
 	mov    $0xa,%edi
-	call   2460 <calloc@plt>
-	mov    %rax,0x4dc6(%rip)        
-	movq   $0x64,0x4da3(%rip)        
-	movq   $0x64,0x4da0(%rip)        
+	call   1930 <calloc@plt>
+	mov    %rax,0x203861(%rip)        
+	movq   $0x64,0x20383e(%rip)        
+	movq   $0x64,0x20383b(%rip)        
 	mov    $0x8,%esi
 	mov    $0x64,%edi
-	call   2460 <calloc@plt>
-	mov    %rax,0x4d7a(%rip)        
-	movq   $0xa,0x4d37(%rip)        
-	movq   $0xa,0x4d34(%rip)        
+	call   1930 <calloc@plt>
+	mov    %rax,0x203815(%rip)        
+	movq   $0xa,0x2037d2(%rip)        
+	movq   $0xa,0x2037cf(%rip)        
 	mov    $0x8,%esi
 	mov    $0xa,%edi
-	call   2460 <calloc@plt>
-	mov    %rax,0x4d0e(%rip)        
-	movq   $0xa,0x4dab(%rip)        
-	movq   $0xa,0x4da8(%rip)        
+	call   1930 <calloc@plt>
+	mov    %rax,0x2037a9(%rip)        
+	movq   $0xa,0x203846(%rip)        
+	movq   $0xa,0x203843(%rip)        
 	mov    $0x50,%edi
-	call   24b0 <malloc@plt>
-	mov    %rax,0x4d87(%rip)        
+	call   1980 <malloc@plt>
+	mov    %rax,0x203822(%rip)        
 	movl   $0x0,-0x1c(%rbp)
-	jmp    4548 <krige_param_setting+0x18f>
-	mov    0x4d77(%rip),%rax        
+	jmp    3aad <krige_param_setting+0x18a>
+	mov    0x203812(%rip),%rax        
 	mov    -0x1c(%rbp),%edx
 	movslq %edx,%rdx
 	shl    $0x3,%rdx
 	lea    (%rax,%rdx,1),%rbx
 	mov    $0x50,%edi
-	call   24b0 <malloc@plt>
+	call   1980 <malloc@plt>
 	mov    %rax,(%rbx)
 	addl   $0x1,-0x1c(%rbp)
 	cmpl   $0x9,-0x1c(%rbp)
-	jle    4522 <krige_param_setting+0x169>
-	movq   $0xa,0x4d6f(%rip)        
-	movq   $0xa,0x4d6c(%rip)        
+	jle    3a87 <krige_param_setting+0x164>
+	movq   $0xa,0x20380a(%rip)        
+	movq   $0xa,0x203807(%rip)        
 	mov    $0x50,%edi
-	call   24b0 <malloc@plt>
-	mov    %rax,0x4d4b(%rip)        
+	call   1980 <malloc@plt>
+	mov    %rax,0x2037e6(%rip)        
 	movl   $0x0,-0x18(%rbp)
-	jmp    45a4 <krige_param_setting+0x1eb>
-	mov    0x4d3b(%rip),%rax        
+	jmp    3b09 <krige_param_setting+0x1e6>
+	mov    0x2037d6(%rip),%rax        
 	mov    -0x18(%rbp),%edx
 	movslq %edx,%rdx
 	shl    $0x3,%rdx
 	lea    (%rax,%rdx,1),%rbx
 	mov    $0x50,%edi
-	call   24b0 <malloc@plt>
+	call   1980 <malloc@plt>
 	mov    %rax,(%rbx)
 	addl   $0x1,-0x18(%rbp)
 	cmpl   $0x9,-0x18(%rbp)
-	jle    457e <krige_param_setting+0x1c5>
-	movq   $0x96,0x4cd3(%rip)        
-	movq   $0x3,0x4cd0(%rip)        
-	mov    $0x4b0,%edi
-	call   24b0 <malloc@plt>
-	mov    %rax,0x4caf(%rip)        
+	jle    3ae3 <krige_param_setting+0x1c0>
+	mov    -0x24(%rbp),%eax
+	cltq
+	mov    %rax,0x20376d(%rip)        
+	movq   $0x3,0x20376a(%rip)        
+	mov    -0x24(%rbp),%eax
+	cltq
+	shl    $0x3,%rax
+	mov    %rax,%rdi
+	call   1980 <malloc@plt>
+	mov    %rax,0x203742(%rip)        
 	movl   $0x0,-0x14(%rbp)
-	jmp    4600 <krige_param_setting+0x247>
-	mov    0x4c9f(%rip),%rax        
+	jmp    3b6d <krige_param_setting+0x24a>
+	mov    0x203732(%rip),%rax        
 	mov    -0x14(%rbp),%edx
 	movslq %edx,%rdx
 	shl    $0x3,%rdx
 	lea    (%rax,%rdx,1),%rbx
 	mov    $0x18,%edi
-	call   24b0 <malloc@plt>
+	call   1980 <malloc@plt>
 	mov    %rax,(%rbx)
 	addl   $0x1,-0x14(%rbp)
-	cmpl   $0x95,-0x14(%rbp)
-	jle    45da <krige_param_setting+0x221>
-	nop
+	mov    -0x14(%rbp),%eax
+	cmp    -0x24(%rbp),%eax
+	jl     3b47 <krige_param_setting+0x224>
 	nop
 	add    $0x28,%rsp
 	pop    %rbx
 	pop    %rbp
 	ret
 
-0000000000004612 <simple_kriging>:
+0000000000003b7d <simple_kriging>:
 simple_kriging():
-	endbr64
 	push   %rbp
 	mov    %rsp,%rbp
-	sub    $0x30,%rsp
+	sub    $0x40,%rsp
 	mov    %rdi,-0x18(%rbp)
 	mov    %rsi,-0x20(%rbp)
 	mov    %rdx,-0x28(%rbp)
 	mov    -0x28(%rbp),%rdx
 	mov    -0x20(%rbp),%rcx
 	mov    -0x18(%rbp),%rax
 	mov    %rcx,%rsi
 	mov    %rax,%rdi
-	call   23d0 <find_neighbor@plt>
+	call   18a0 <find_neighbor@plt>
 	mov    %eax,-0x4(%rbp)
 	cmpl   $0x0,-0x4(%rbp)
-	je     4a33 <simple_kriging+0x421>
+	je     3f7a <simple_kriging+0x3fd>
 	movl   $0x0,-0x10(%rbp)
-	jmp    471b <simple_kriging+0x109>
+	jmp    3c82 <simple_kriging+0x105>
 	mov    -0x20(%rbp),%rax
 	mov    0x18(%rax),%rax
 	mov    -0x10(%rbp),%edx
 	movslq %edx,%rdx
 	shl    $0x3,%rdx
 	add    %rax,%rdx
-	mov    0x4c0a(%rip),%rax        
+	mov    0x2036a3(%rip),%rax        
 	mov    -0x10(%rbp),%ecx
 	movslq %ecx,%rcx
 	shl    $0x3,%rcx
 	add    %rcx,%rax
 	mov    (%rax),%rax
 	movsd  (%rdx),%xmm0
 	movsd  %xmm0,(%rax)
@@ -2334,515 +2369,510 @@
 	add    %rdx,%rax
 	movsd  (%rax),%xmm0
 	cvttsd2si %xmm0,%eax
 	cltq
 	lea    0x0(,%rax,8),%rdx
 	mov    -0x18(%rbp),%rax
 	add    %rax,%rdx
-	mov    0x4bbd(%rip),%rax        
+	mov    0x203656(%rip),%rax        
 	mov    -0x10(%rbp),%ecx
 	movslq %ecx,%rcx
 	shl    $0x3,%rcx
 	add    %rcx,%rax
 	mov    (%rax),%rax
 	add    $0x8,%rax
 	movsd  (%rdx),%xmm0
 	movsd  %xmm0,(%rax)
 	mov    -0x20(%rbp),%rax
 	mov    0x30(%rax),%rax
 	mov    -0x10(%rbp),%edx
 	movslq %edx,%rdx
 	shl    $0x3,%rdx
 	add    %rax,%rdx
-	mov    0x4b85(%rip),%rax        
+	mov    0x20361e(%rip),%rax        
 	mov    -0x10(%rbp),%ecx
 	movslq %ecx,%rcx
 	shl    $0x3,%rcx
 	add    %rcx,%rax
 	mov    (%rax),%rax
 	add    $0x10,%rax
 	movsd  (%rdx),%xmm0
 	movsd  %xmm0,(%rax)
 	addl   $0x1,-0x10(%rbp)
 	mov    -0x20(%rbp),%rax
 	mov    0x4(%rax),%eax
 	cmp    %eax,-0x10(%rbp)
-	jl     465a <simple_kriging+0x48>
+	jl     3bc1 <simple_kriging+0x44>
 	mov    -0x20(%rbp),%rax
 	mov    (%rax),%eax
 	cmp    $0x1,%eax
-	jle    4754 <simple_kriging+0x142>
+	jle    3cbb <simple_kriging+0x13e>
 	mov    -0x20(%rbp),%rax
 	mov    0x4(%rax),%eax
 	lea    -0x1(%rax),%edx
-	mov    0x4b39(%rip),%rax        
+	mov    0x2035d2(%rip),%rax        
 	mov    $0x0,%esi
 	mov    %rax,%rdi
-	call   2320 <quicksort2d@plt>
+	call   17f0 <quicksort2d@plt>
 	movl   $0x0,-0xc(%rbp)
-	jmp    47c8 <simple_kriging+0x1b6>
-	mov    0x4b1c(%rip),%rax        
+	jmp    3d2f <simple_kriging+0x1b2>
+	mov    0x2035b5(%rip),%rax        
 	mov    -0xc(%rbp),%edx
 	movslq %edx,%rdx
 	shl    $0x3,%rdx
 	add    %rdx,%rax
 	mov    (%rax),%rax
-	mov    0x4a45(%rip),%rdx        
+	mov    0x2034de(%rip),%rdx        
 	mov    -0xc(%rbp),%ecx
 	movslq %ecx,%rcx
 	shl    $0x3,%rcx
 	add    %rcx,%rdx
 	movsd  (%rax),%xmm0
 	movsd  %xmm0,(%rdx)
-	mov    0x4ae9(%rip),%rax        
+	mov    0x203582(%rip),%rax        
 	mov    -0xc(%rbp),%edx
 	movslq %edx,%rdx
 	shl    $0x3,%rdx
 	add    %rdx,%rax
 	mov    (%rax),%rax
-	mov    0x4a72(%rip),%rdx        
+	mov    0x20350b(%rip),%rdx        
 	mov    -0xc(%rbp),%ecx
 	movslq %ecx,%rcx
 	shl    $0x3,%rcx
 	add    %rcx,%rdx
 	movsd  0x10(%rax),%xmm0
 	movsd  %xmm0,(%rdx)
 	addl   $0x1,-0xc(%rbp)
 	mov    -0x20(%rbp),%rax
 	mov    (%rax),%eax
 	cmp    %eax,-0xc(%rbp)
-	jl     475d <simple_kriging+0x14b>
+	jl     3cc4 <simple_kriging+0x147>
 	mov    -0x20(%rbp),%rax
 	mov    (%rax),%edx
-	mov    0x4ac0(%rip),%rcx        
-	mov    0x49d9(%rip),%rax        
+	mov    0x203559(%rip),%rcx        
+	mov    0x203472(%rip),%rax        
 	mov    %rcx,%rsi
 	mov    %rax,%rdi
-	call   2590 <pdist@plt>
-	movsd  0x499e(%rip),%xmm0        
-	mov    0x498f(%rip),%rsi        
+	call   1a60 <pdist@plt>
+	mov    0x203430(%rip),%rcx        
 	mov    -0x20(%rbp),%rax
 	mov    (%rax),%edx
-	mov    0x4a32(%rip),%rcx        
-	mov    0x4a8b(%rip),%rax        
-	movapd %xmm0,%xmm1
-	movq   %rsi,%xmm0
-	mov    %rcx,%rsi
+	mov    0x2034d3(%rip),%rsi        
+	mov    0x20352c(%rip),%rax        
 	mov    %rax,%rdi
-	call   23b0 <cov_model2d@plt>
+	call   1880 <cov_model2d@plt>
 	mov    -0x20(%rbp),%rax
 	mov    (%rax),%edx
-	mov    0x4a8a(%rip),%rcx        
-	mov    0x4a03(%rip),%rax        
+	mov    0x203537(%rip),%rcx        
+	mov    0x2034b0(%rip),%rax        
 	mov    %rcx,%rsi
 	mov    %rax,%rdi
-	call   2430 <matrixform@plt>
-	movsd  0x4948(%rip),%xmm0        
-	mov    0x4939(%rip),%rsi        
+	call   1900 <matrixform@plt>
+	mov    0x2033ee(%rip),%rcx        
 	mov    -0x20(%rbp),%rax
 	mov    (%rax),%edx
-	mov    0x497c(%rip),%rcx        
-	mov    0x49b5(%rip),%rax        
-	movapd %xmm0,%xmm1
-	movq   %rsi,%xmm0
-	mov    %rcx,%rsi
+	mov    0x203431(%rip),%rsi        
+	mov    0x20346a(%rip),%rax        
 	mov    %rax,%rdi
-	call   2420 <cov_model@plt>
+	call   18f0 <cov_model@plt>
 	mov    -0x20(%rbp),%rax
 	mov    (%rax),%eax
 	test   %eax,%eax
-	jle    48ac <simple_kriging+0x29a>
+	jle    3deb <simple_kriging+0x26e>
 	mov    -0x20(%rbp),%rax
 	mov    (%rax),%ecx
-	mov    0x49ca(%rip),%rdx        
-	mov    0x4943(%rip),%rsi        
-	mov    0x4a1c(%rip),%rax        
+	mov    0x20348b(%rip),%rdx        
+	mov    0x203404(%rip),%rsi        
+	mov    0x2034dd(%rip),%rax        
 	mov    %rax,%rdi
-	call   2360 <lu_inverse_solver@plt>
+	call   1830 <lu_inverse_solver@plt>
 	pxor   %xmm0,%xmm0
-	movsd  %xmm0,0x48e8(%rip)        
+	movsd  %xmm0,0x2033a9(%rip)        
 	pxor   %xmm0,%xmm0
-	movsd  %xmm0,0x48e4(%rip)        
+	movsd  %xmm0,0x2033a5(%rip)        
 	pxor   %xmm0,%xmm0
-	movsd  %xmm0,0x48e0(%rip)        
+	movsd  %xmm0,0x2033a1(%rip)        
 	movl   $0x0,-0x8(%rbp)
-	jmp    4977 <simple_kriging+0x365>
-	mov    0x499d(%rip),%rax        
+	jmp    3eb6 <simple_kriging+0x339>
+	mov    0x20345e(%rip),%rax        
 	mov    -0x8(%rbp),%edx
 	movslq %edx,%rdx
 	shl    $0x3,%rdx
 	add    %rdx,%rax
 	mov    (%rax),%rax
 	add    $0x8,%rax
 	movsd  (%rax),%xmm1
-	mov    0x495e(%rip),%rax        
+	mov    0x20341f(%rip),%rax        
 	mov    -0x8(%rbp),%edx
 	movslq %edx,%rdx
 	shl    $0x3,%rdx
 	add    %rdx,%rax
 	movsd  (%rax),%xmm0
-	mulsd  %xmm0,%xmm1
-	movsd  0x4881(%rip),%xmm0        
+	mulsd  %xmm1,%xmm0
+	movsd  0x203342(%rip),%xmm1        
 	addsd  %xmm1,%xmm0
-	movsd  %xmm0,0x4875(%rip)        
-	mov    0x48ae(%rip),%rax        
+	movsd  %xmm0,0x203336(%rip)        
+	mov    0x20336f(%rip),%rax        
 	mov    -0x8(%rbp),%edx
 	movslq %edx,%rdx
 	shl    $0x3,%rdx
 	add    %rdx,%rax
 	movsd  (%rax),%xmm1
-	mov    0x4916(%rip),%rax        
+	mov    0x2033d7(%rip),%rax        
 	mov    -0x8(%rbp),%edx
 	movslq %edx,%rdx
 	shl    $0x3,%rdx
 	add    %rdx,%rax
 	movsd  (%rax),%xmm0
-	mulsd  %xmm0,%xmm1
-	movsd  0x4841(%rip),%xmm0        
+	mulsd  %xmm1,%xmm0
+	movsd  0x203302(%rip),%xmm1        
 	addsd  %xmm1,%xmm0
-	movsd  %xmm0,0x4835(%rip)        
+	movsd  %xmm0,0x2032f6(%rip)        
 	addl   $0x1,-0x8(%rbp)
 	mov    -0x20(%rbp),%rax
 	mov    (%rax),%eax
 	cmp    %eax,-0x8(%rbp)
-	jl     48dc <simple_kriging+0x2ca>
-	movsd  0x481a(%rip),%xmm1        
-	movsd  0x26ca(%rip),%xmm0        
+	jl     3e1b <simple_kriging+0x29e>
+	mov    0x2032c4(%rip),%rax        
+	movsd  0x18(%rax),%xmm0
+	movsd  0x2032cf(%rip),%xmm1        
 	subsd  %xmm1,%xmm0
-	movsd  %xmm0,0x4806(%rip)        
-	movsd  0x47fe(%rip),%xmm1        
+	movsd  %xmm0,0x2032c3(%rip)        
+	movsd  0x2032bb(%rip),%xmm1        
 	pxor   %xmm0,%xmm0
-	comisd %xmm1,%xmm0
-	jbe    49c0 <simple_kriging+0x3ae>
+	ucomisd %xmm1,%xmm0
+	jbe    3f03 <simple_kriging+0x386>
 	pxor   %xmm0,%xmm0
-	movsd  %xmm0,0x47e8(%rip)        
+	movsd  %xmm0,0x2032a5(%rip)        
 	mov    -0x28(%rbp),%rax
 	mov    %rax,%rdi
-	call   2450 <mt19937_random_normal@plt>
+	call   1920 <mt19937_random_normal@plt>
 	movsd  %xmm0,-0x30(%rbp)
-	mov    0x47d0(%rip),%rax        
-	movsd  0x2688(%rip),%xmm0        
+	mov    0x20328d(%rip),%rax        
+	movsd  0x1dcd(%rip),%xmm0        
 	movapd %xmm0,%xmm1
-	movq   %rax,%xmm0
-	call   2550 <pow@plt>
+	mov    %rax,-0x38(%rbp)
+	movsd  -0x38(%rbp),%xmm0
+	call   1a20 <pow@plt>
 	mulsd  -0x30(%rbp),%xmm0
-	movsd  %xmm0,0x47b5(%rip)        
-	movsd  0x479d(%rip),%xmm1        
-	movsd  0x47a5(%rip),%xmm0        
+	movsd  %xmm0,0x20326e(%rip)        
+	movsd  0x203256(%rip),%xmm1        
+	movsd  0x20325e(%rip),%xmm0        
 	mov    -0x20(%rbp),%rax
 	movsd  0x10(%rax),%xmm2
 	cvttsd2si %xmm2,%eax
 	cltq
 	lea    0x0(,%rax,8),%rdx
 	mov    -0x18(%rbp),%rax
 	add    %rdx,%rax
 	addsd  %xmm1,%xmm0
 	movsd  %xmm0,(%rax)
-	jmp    4a34 <simple_kriging+0x422>
+	jmp    3f7b <simple_kriging+0x3fe>
 	nop
 	leave
 	ret
 
-0000000000004a36 <find_neighbor>:
+0000000000003f7d <find_neighbor>:
 find_neighbor():
-	endbr64
 	push   %rbp
 	mov    %rsp,%rbp
-	push   %rbx
-	sub    $0x38,%rsp
-	mov    %rdi,-0x28(%rbp)
-	mov    %rsi,-0x30(%rbp)
-	mov    %rdx,-0x38(%rbp)
-	mov    -0x30(%rbp),%rax
+	sub    $0x30,%rsp
+	mov    %rdi,-0x18(%rbp)
+	mov    %rsi,-0x20(%rbp)
+	mov    %rdx,-0x28(%rbp)
+	mov    -0x20(%rbp),%rax
 	mov    (%rax),%eax
 	test   %eax,%eax
-	jne    4abb <find_neighbor+0x85>
-	mov    -0x30(%rbp),%rax
-	movsd  0x10(%rax),%xmm0
-	cvttsd2si %xmm0,%eax
-	cltq
-	lea    0x0(,%rax,8),%rdx
+	jne    400c <find_neighbor+0x8f>
 	mov    -0x28(%rbp),%rax
-	lea    (%rdx,%rax,1),%rbx
-	mov    -0x38(%rbp),%rax
 	mov    %rax,%rdi
-	call   2450 <mt19937_random_normal@plt>
-	movq   %xmm0,%rax
-	mov    %rax,(%rbx)
-	mov    -0x30(%rbp),%rax
+	call   1920 <mt19937_random_normal@plt>
+	movapd %xmm0,%xmm1
+	mov    0x2031de(%rip),%rax        
+	movsd  0x18(%rax),%xmm0
+	mov    -0x20(%rbp),%rax
+	movsd  0x10(%rax),%xmm2
+	cvttsd2si %xmm2,%eax
+	cltq
+	lea    0x0(,%rax,8),%rdx
+	mov    -0x18(%rbp),%rax
+	add    %rdx,%rax
+	mulsd  %xmm1,%xmm0
+	movsd  %xmm0,(%rax)
+	mov    -0x20(%rbp),%rax
 	mov    0x18(%rax),%rdx
-	mov    -0x30(%rbp),%rax
+	mov    -0x20(%rbp),%rax
 	mov    0x8(%rax),%eax
 	cltq
 	shl    $0x3,%rax
 	add    %rax,%rdx
-	mov    -0x30(%rbp),%rax
+	mov    -0x20(%rbp),%rax
 	movsd  0x10(%rax),%xmm0
 	movsd  %xmm0,(%rdx)
 	mov    $0x0,%eax
-	jmp    4bce <find_neighbor+0x198>
-	movl   $0x0,-0x18(%rbp)
-	movl   $0x0,-0x14(%rbp)
-	jmp    4b54 <find_neighbor+0x11e>
-	mov    -0x30(%rbp),%rax
+	jmp    412e <find_neighbor+0x1b1>
+	movl   $0x0,-0x8(%rbp)
+	movl   $0x0,-0x4(%rbp)
+	jmp    40a5 <find_neighbor+0x128>
+	mov    -0x20(%rbp),%rax
 	mov    0x18(%rax),%rax
-	mov    -0x14(%rbp),%edx
+	mov    -0x4(%rbp),%edx
 	movslq %edx,%rdx
 	shl    $0x3,%rdx
 	add    %rdx,%rax
 	movsd  (%rax),%xmm0
-	mov    -0x30(%rbp),%rax
+	mov    -0x20(%rbp),%rax
 	movsd  0x10(%rax),%xmm1
 	subsd  %xmm1,%xmm0
-	mov    -0x30(%rbp),%rax
+	mov    -0x20(%rbp),%rax
 	mov    0x30(%rax),%rax
-	mov    -0x14(%rbp),%edx
+	mov    -0x4(%rbp),%edx
 	movslq %edx,%rdx
 	shl    $0x3,%rdx
 	add    %rdx,%rax
-	movq   0x255f(%rip),%xmm1        
+	movq   0x1c9e(%rip),%xmm1        
 	andpd  %xmm1,%xmm0
 	movsd  %xmm0,(%rax)
-	mov    -0x30(%rbp),%rax
+	mov    -0x20(%rbp),%rax
 	mov    0x30(%rax),%rax
-	mov    -0x14(%rbp),%edx
+	mov    -0x4(%rbp),%edx
 	movslq %edx,%rdx
 	shl    $0x3,%rdx
 	add    %rdx,%rax
 	movsd  (%rax),%xmm1
-	movsd  0x4656(%rip),%xmm2        
-	movsd  0x253e(%rip),%xmm0        
+	movsd  0x20310d(%rip),%xmm2        
+	movsd  0x1c7d(%rip),%xmm0        
 	mulsd  %xmm2,%xmm0
-	comisd %xmm1,%xmm0
-	jbe    4b50 <find_neighbor+0x11a>
-	addl   $0x1,-0x18(%rbp)
-	addl   $0x1,-0x14(%rbp)
-	mov    -0x30(%rbp),%rax
+	ucomisd %xmm1,%xmm0
+	jbe    40a1 <find_neighbor+0x124>
+	addl   $0x1,-0x8(%rbp)
+	addl   $0x1,-0x4(%rbp)
+	mov    -0x20(%rbp),%rax
 	mov    0x4(%rax),%eax
-	cmp    %eax,-0x14(%rbp)
-	jl     4ace <find_neighbor+0x98>
-	cmpl   $0x0,-0x18(%rbp)
-	jne    4bc9 <find_neighbor+0x193>
-	mov    -0x30(%rbp),%rax
-	movsd  0x10(%rax),%xmm0
-	cvttsd2si %xmm0,%eax
-	cltq
-	lea    0x0(,%rax,8),%rdx
+	cmp    %eax,-0x4(%rbp)
+	jl     401f <find_neighbor+0xa2>
+	cmpl   $0x0,-0x8(%rbp)
+	jne    4129 <find_neighbor+0x1ac>
 	mov    -0x28(%rbp),%rax
-	lea    (%rdx,%rax,1),%rbx
-	mov    -0x38(%rbp),%rax
 	mov    %rax,%rdi
-	call   2450 <mt19937_random_normal@plt>
-	movq   %xmm0,%rax
-	mov    %rax,(%rbx)
-	mov    -0x30(%rbp),%rax
+	call   1920 <mt19937_random_normal@plt>
+	movapd %xmm0,%xmm1
+	mov    0x2030be(%rip),%rax        
+	movsd  0x18(%rax),%xmm0
+	mov    -0x20(%rbp),%rax
+	movsd  0x10(%rax),%xmm2
+	cvttsd2si %xmm2,%eax
+	cltq
+	lea    0x0(,%rax,8),%rdx
+	mov    -0x18(%rbp),%rax
+	add    %rdx,%rax
+	mulsd  %xmm1,%xmm0
+	movsd  %xmm0,(%rax)
+	mov    -0x20(%rbp),%rax
 	mov    0x18(%rax),%rdx
-	mov    -0x30(%rbp),%rax
+	mov    -0x20(%rbp),%rax
 	mov    0x8(%rax),%eax
 	cltq
 	shl    $0x3,%rax
 	add    %rax,%rdx
-	mov    -0x30(%rbp),%rax
+	mov    -0x20(%rbp),%rax
 	movsd  0x10(%rax),%xmm0
 	movsd  %xmm0,(%rdx)
 	mov    $0x0,%eax
-	jmp    4bce <find_neighbor+0x198>
+	jmp    412e <find_neighbor+0x1b1>
 	mov    $0x1,%eax
-	add    $0x38,%rsp
-	pop    %rbx
-	pop    %rbp
+	leave
 	ret
 
-0000000000004bd5 <krige_memory_free>:
+0000000000004130 <krige_memory_free>:
 krige_memory_free():
-	endbr64
 	push   %rbp
 	mov    %rsp,%rbp
 	sub    $0x10,%rsp
-	mov    0x45d8(%rip),%rax        
+	mov    0x203081(%rip),%rax        
 	mov    %rax,%rdi
-	call   2300 <free@plt>
-	mov    0x45e9(%rip),%rax        
+	call   17d0 <free@plt>
+	mov    0x203092(%rip),%rax        
 	mov    %rax,%rdi
-	call   2300 <free@plt>
-	mov    0x45fa(%rip),%rax        
+	call   17d0 <free@plt>
+	mov    0x2030a3(%rip),%rax        
 	mov    %rax,%rdi
-	call   2300 <free@plt>
-	mov    0x460b(%rip),%rax        
+	call   17d0 <free@plt>
+	mov    0x2030b4(%rip),%rax        
 	mov    %rax,%rdi
-	call   2300 <free@plt>
-	mov    0x461c(%rip),%rax        
+	call   17d0 <free@plt>
+	mov    0x2030c5(%rip),%rax        
 	mov    %rax,%rdi
-	call   2300 <free@plt>
-	mov    0x462d(%rip),%rax        
+	call   17d0 <free@plt>
+	mov    0x2030d6(%rip),%rax        
 	mov    %rax,%rdi
-	call   2300 <free@plt>
+	call   17d0 <free@plt>
 	movl   $0x0,-0xc(%rbp)
-	jmp    4c67 <krige_memory_free+0x92>
-	mov    0x4635(%rip),%rax        
+	jmp    41be <krige_memory_free+0x8e>
+	mov    0x2030de(%rip),%rax        
 	mov    -0xc(%rbp),%edx
 	movslq %edx,%rdx
 	shl    $0x3,%rdx
 	add    %rdx,%rax
 	mov    (%rax),%rax
 	mov    %rax,%rdi
-	call   2300 <free@plt>
+	call   17d0 <free@plt>
 	addl   $0x1,-0xc(%rbp)
 	mov    -0xc(%rbp),%eax
 	movslq %eax,%rdx
-	mov    0x4614(%rip),%rax        
+	mov    0x2030bd(%rip),%rax        
 	cmp    %rax,%rdx
-	jb     4c44 <krige_memory_free+0x6f>
-	mov    0x4600(%rip),%rax        
+	jb     419b <krige_memory_free+0x6b>
+	mov    0x2030a9(%rip),%rax        
 	mov    %rax,%rdi
-	call   2300 <free@plt>
+	call   17d0 <free@plt>
 	movl   $0x0,-0x8(%rbp)
-	jmp    4cb4 <krige_memory_free+0xdf>
-	mov    0x4608(%rip),%rax        
+	jmp    420b <krige_memory_free+0xdb>
+	mov    0x2030b1(%rip),%rax        
 	mov    -0x8(%rbp),%edx
 	movslq %edx,%rdx
 	shl    $0x3,%rdx
 	add    %rdx,%rax
 	mov    (%rax),%rax
 	mov    %rax,%rdi
-	call   2300 <free@plt>
+	call   17d0 <free@plt>
 	addl   $0x1,-0x8(%rbp)
 	mov    -0x8(%rbp),%eax
 	movslq %eax,%rdx
-	mov    0x45e7(%rip),%rax        
+	mov    0x203090(%rip),%rax        
 	cmp    %rax,%rdx
-	jb     4c91 <krige_memory_free+0xbc>
-	mov    0x45d3(%rip),%rax        
+	jb     41e8 <krige_memory_free+0xb8>
+	mov    0x20307c(%rip),%rax        
 	mov    %rax,%rdi
-	call   2300 <free@plt>
+	call   17d0 <free@plt>
 	movl   $0x0,-0x4(%rbp)
-	jmp    4d01 <krige_memory_free+0x12c>
-	mov    0x45db(%rip),%rax        
+	jmp    4258 <krige_memory_free+0x128>
+	mov    0x203084(%rip),%rax        
 	mov    -0x4(%rbp),%edx
 	movslq %edx,%rdx
 	shl    $0x3,%rdx
 	add    %rdx,%rax
 	mov    (%rax),%rax
 	mov    %rax,%rdi
-	call   2300 <free@plt>
+	call   17d0 <free@plt>
 	addl   $0x1,-0x4(%rbp)
 	mov    -0x4(%rbp),%eax
 	movslq %eax,%rdx
-	mov    0x45ba(%rip),%rax        
+	mov    0x203063(%rip),%rax        
 	cmp    %rax,%rdx
-	jb     4cde <krige_memory_free+0x109>
-	mov    0x45a6(%rip),%rax        
+	jb     4235 <krige_memory_free+0x105>
+	mov    0x20304f(%rip),%rax        
 	mov    %rax,%rdi
-	call   2300 <free@plt>
+	call   17d0 <free@plt>
 	nop
 	leave
 	ret
 
-0000000000004d25 <lu_inverse_solver>:
+000000000000427c <lu_inverse_solver>:
 lu_inverse_solver():
-	endbr64
 	push   %rbp
 	mov    %rsp,%rbp
 	push   %rbx
 	sub    $0xe8,%rsp
 	mov    %rdi,-0xd8(%rbp)
 	mov    %rsi,-0xe0(%rbp)
 	mov    %rdx,-0xe8(%rbp)
 	mov    %ecx,-0xec(%rbp)
 	mov    %fs:0x28,%rax
 	mov    %rax,-0x18(%rbp)
 	xor    %eax,%eax
 	movq   $0xa,-0xa8(%rbp)
 	movq   $0xa,-0xa0(%rbp)
 	mov    $0x50,%edi
-	call   24b0 <malloc@plt>
+	call   1980 <malloc@plt>
 	mov    %rax,-0xb0(%rbp)
 	movl   $0x0,-0xd0(%rbp)
-	jmp    4dbe <lu_inverse_solver+0x99>
+	jmp    4311 <lu_inverse_solver+0x95>
 	mov    -0xb0(%rbp),%rax
 	mov    -0xd0(%rbp),%edx
 	movslq %edx,%rdx
 	shl    $0x3,%rdx
 	lea    (%rax,%rdx,1),%rbx
 	mov    $0x50,%edi
-	call   24b0 <malloc@plt>
+	call   1980 <malloc@plt>
 	mov    %rax,(%rbx)
 	addl   $0x1,-0xd0(%rbp)
 	cmpl   $0x9,-0xd0(%rbp)
-	jle    4d92 <lu_inverse_solver+0x6d>
+	jle    42e5 <lu_inverse_solver+0x69>
 	movq   $0xa,-0x88(%rbp)
 	movq   $0xa,-0x80(%rbp)
 	mov    $0x50,%edi
-	call   24b0 <malloc@plt>
+	call   1980 <malloc@plt>
 	mov    %rax,-0x90(%rbp)
 	movl   $0x0,-0xcc(%rbp)
-	jmp    4e23 <lu_inverse_solver+0xfe>
+	jmp    4376 <lu_inverse_solver+0xfa>
 	mov    -0x90(%rbp),%rax
 	mov    -0xcc(%rbp),%edx
 	movslq %edx,%rdx
 	shl    $0x3,%rdx
 	lea    (%rax,%rdx,1),%rbx
 	mov    $0x50,%edi
-	call   24b0 <malloc@plt>
+	call   1980 <malloc@plt>
 	mov    %rax,(%rbx)
 	addl   $0x1,-0xcc(%rbp)
 	cmpl   $0x9,-0xcc(%rbp)
-	jle    4df7 <lu_inverse_solver+0xd2>
+	jle    434a <lu_inverse_solver+0xce>
 	mov    -0x90(%rbp),%rdx
 	mov    -0xb0(%rbp),%rsi
 	mov    -0xec(%rbp),%ecx
 	mov    -0xd8(%rbp),%rax
 	mov    %rax,%rdi
-	call   23f0 <lu_decomposition@plt>
+	call   18c0 <lu_decomposition@plt>
 	mov    -0xe0(%rbp),%rax
 	movsd  (%rax),%xmm0
 	mov    -0xb0(%rbp),%rax
 	mov    (%rax),%rax
 	movsd  (%rax),%xmm1
 	divsd  %xmm1,%xmm0
 	movsd  %xmm0,-0x70(%rbp)
 	movl   $0x1,-0xc8(%rbp)
-	jmp    4f82 <lu_inverse_solver+0x25d>
+	jmp    44d9 <lu_inverse_solver+0x25d>
 	mov    -0xc8(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,8),%rdx
 	mov    -0xe0(%rbp),%rax
 	add    %rdx,%rax
 	movsd  (%rax),%xmm0
 	mov    -0xc8(%rbp),%eax
 	cltq
 	movsd  %xmm0,-0x70(%rbp,%rax,8)
 	movl   $0x0,-0xc4(%rbp)
-	jmp    4f1f <lu_inverse_solver+0x1fa>
+	jmp    4476 <lu_inverse_solver+0x1fa>
 	mov    -0xc8(%rbp),%eax
 	cltq
-	movsd  -0x70(%rbp,%rax,8),%xmm0
+	movsd  -0x70(%rbp,%rax,8),%xmm1
 	mov    -0xb0(%rbp),%rax
 	mov    -0xc8(%rbp),%edx
 	movslq %edx,%rdx
 	shl    $0x3,%rdx
 	add    %rdx,%rax
 	mov    (%rax),%rax
 	mov    -0xc4(%rbp),%edx
 	movslq %edx,%rdx
 	shl    $0x3,%rdx
 	add    %rdx,%rax
 	movsd  (%rax),%xmm2
 	mov    -0xc4(%rbp),%eax
 	cltq
-	movsd  -0x70(%rbp,%rax,8),%xmm1
-	mulsd  %xmm2,%xmm1
-	subsd  %xmm1,%xmm0
+	movsd  -0x70(%rbp,%rax,8),%xmm0
+	mulsd  %xmm2,%xmm0
+	subsd  %xmm0,%xmm1
+	movapd %xmm1,%xmm0
 	mov    -0xc8(%rbp),%eax
 	cltq
 	movsd  %xmm0,-0x70(%rbp,%rax,8)
 	addl   $0x1,-0xc4(%rbp)
 	mov    -0xc4(%rbp),%eax
 	cmp    -0xc8(%rbp),%eax
-	jl     4eb8 <lu_inverse_solver+0x193>
+	jl     440b <lu_inverse_solver+0x18f>
 	mov    -0xc8(%rbp),%eax
 	cltq
 	movsd  -0x70(%rbp,%rax,8),%xmm0
 	mov    -0xb0(%rbp),%rax
 	mov    -0xc8(%rbp),%edx
 	movslq %edx,%rdx
 	shl    $0x3,%rdx
@@ -2856,47 +2886,47 @@
 	divsd  %xmm1,%xmm0
 	mov    -0xc8(%rbp),%eax
 	cltq
 	movsd  %xmm0,-0x70(%rbp,%rax,8)
 	addl   $0x1,-0xc8(%rbp)
 	mov    -0xc8(%rbp),%eax
 	cmp    -0xec(%rbp),%eax
-	jl     4e80 <lu_inverse_solver+0x15b>
+	jl     43d3 <lu_inverse_solver+0x157>
 	mov    -0xec(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,8),%rdx
 	mov    -0xe8(%rbp),%rax
 	add    %rax,%rdx
 	mov    -0xec(%rbp),%eax
 	cltq
 	movsd  -0x70(%rbp,%rax,8),%xmm0
 	movsd  %xmm0,(%rdx)
 	mov    -0xec(%rbp),%eax
 	sub    $0x1,%eax
 	mov    %eax,-0xc0(%rbp)
-	jmp    50c4 <lu_inverse_solver+0x39f>
+	jmp    461f <lu_inverse_solver+0x3a3>
 	mov    -0xc0(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,8),%rdx
 	mov    -0xe8(%rbp),%rax
 	add    %rax,%rdx
 	mov    -0xc0(%rbp),%eax
 	cltq
 	movsd  -0x70(%rbp,%rax,8),%xmm0
 	movsd  %xmm0,(%rdx)
 	mov    -0xc0(%rbp),%eax
 	add    $0x1,%eax
 	mov    %eax,-0xbc(%rbp)
-	jmp    50ab <lu_inverse_solver+0x386>
+	jmp    4606 <lu_inverse_solver+0x38a>
 	mov    -0xc0(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,8),%rdx
 	mov    -0xe8(%rbp),%rax
 	add    %rdx,%rax
-	movsd  (%rax),%xmm0
+	movsd  (%rax),%xmm1
 	mov    -0x90(%rbp),%rax
 	mov    -0xc0(%rbp),%edx
 	movslq %edx,%rdx
 	shl    $0x3,%rdx
 	add    %rdx,%rax
 	mov    (%rax),%rax
 	mov    -0xbc(%rbp),%edx
@@ -2905,107 +2935,107 @@
 	add    %rdx,%rax
 	movsd  (%rax),%xmm2
 	mov    -0xbc(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,8),%rdx
 	mov    -0xe8(%rbp),%rax
 	add    %rdx,%rax
-	movsd  (%rax),%xmm1
-	mulsd  %xmm2,%xmm1
+	movsd  (%rax),%xmm0
+	mulsd  %xmm2,%xmm0
 	mov    -0xc0(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,8),%rdx
 	mov    -0xe8(%rbp),%rax
 	add    %rdx,%rax
-	subsd  %xmm1,%xmm0
+	subsd  %xmm0,%xmm1
+	movapd %xmm1,%xmm0
 	movsd  %xmm0,(%rax)
 	addl   $0x1,-0xbc(%rbp)
 	mov    -0xbc(%rbp),%eax
 	cmp    -0xec(%rbp),%eax
-	jl     5014 <lu_inverse_solver+0x2ef>
+	jl     456b <lu_inverse_solver+0x2ef>
 	subl   $0x1,-0xc0(%rbp)
 	cmpl   $0x0,-0xc0(%rbp)
-	jns    4fd4 <lu_inverse_solver+0x2af>
+	jns    452b <lu_inverse_solver+0x2af>
 	movl   $0x0,-0xb8(%rbp)
-	jmp    5106 <lu_inverse_solver+0x3e1>
+	jmp    4661 <lu_inverse_solver+0x3e5>
 	mov    -0xb0(%rbp),%rax
 	mov    -0xb8(%rbp),%edx
 	movslq %edx,%rdx
 	shl    $0x3,%rdx
 	add    %rdx,%rax
 	mov    (%rax),%rax
 	mov    %rax,%rdi
-	call   2300 <free@plt>
+	call   17d0 <free@plt>
 	addl   $0x1,-0xb8(%rbp)
 	mov    -0xb8(%rbp),%eax
 	movslq %eax,%rdx
 	mov    -0xa8(%rbp),%rax
 	cmp    %rax,%rdx
-	jb     50dd <lu_inverse_solver+0x3b8>
+	jb     4638 <lu_inverse_solver+0x3bc>
 	mov    -0xb0(%rbp),%rax
 	mov    %rax,%rdi
-	call   2300 <free@plt>
+	call   17d0 <free@plt>
 	movl   $0x0,-0xb4(%rbp)
-	jmp    515f <lu_inverse_solver+0x43a>
+	jmp    46ba <lu_inverse_solver+0x43e>
 	mov    -0x90(%rbp),%rax
 	mov    -0xb4(%rbp),%edx
 	movslq %edx,%rdx
 	shl    $0x3,%rdx
 	add    %rdx,%rax
 	mov    (%rax),%rax
 	mov    %rax,%rdi
-	call   2300 <free@plt>
+	call   17d0 <free@plt>
 	addl   $0x1,-0xb4(%rbp)
 	mov    -0xb4(%rbp),%eax
 	movslq %eax,%rdx
 	mov    -0x88(%rbp),%rax
 	cmp    %rax,%rdx
-	jb     5136 <lu_inverse_solver+0x411>
+	jb     4691 <lu_inverse_solver+0x415>
 	mov    -0x90(%rbp),%rax
 	mov    %rax,%rdi
-	call   2300 <free@plt>
+	call   17d0 <free@plt>
 	nop
 	mov    -0x18(%rbp),%rax
 	xor    %fs:0x28,%rax
-	je     5198 <lu_inverse_solver+0x473>
-	call   2390 <__stack_chk_fail@plt>
+	je     46f3 <lu_inverse_solver+0x477>
+	call   1860 <__stack_chk_fail@plt>
 	add    $0xe8,%rsp
 	pop    %rbx
 	pop    %rbp
 	ret
 
-00000000000051a2 <lu_decomposition>:
+00000000000046fd <lu_decomposition>:
 lu_decomposition():
-	endbr64
 	push   %rbp
 	mov    %rsp,%rbp
 	mov    %rdi,-0x28(%rbp)
 	mov    %rsi,-0x30(%rbp)
 	mov    %rdx,-0x38(%rbp)
 	mov    %ecx,-0x3c(%rbp)
 	movl   $0x0,-0x14(%rbp)
-	jmp    5530 <lu_decomposition+0x38e>
+	jmp    4a8f <lu_decomposition+0x392>
 	movl   $0x0,-0x10(%rbp)
-	jmp    5322 <lu_decomposition+0x180>
+	jmp    487d <lu_decomposition+0x180>
 	mov    -0x10(%rbp),%eax
 	cmp    -0x14(%rbp),%eax
-	jge    520a <lu_decomposition+0x68>
+	jge    4761 <lu_decomposition+0x64>
 	mov    -0x10(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,8),%rdx
 	mov    -0x30(%rbp),%rax
 	add    %rdx,%rax
 	mov    (%rax),%rax
 	mov    -0x14(%rbp),%edx
 	movslq %edx,%rdx
 	shl    $0x3,%rdx
 	add    %rdx,%rax
 	pxor   %xmm0,%xmm0
 	movsd  %xmm0,(%rax)
-	jmp    531e <lu_decomposition+0x17c>
+	jmp    4879 <lu_decomposition+0x17c>
 	mov    -0x10(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,8),%rdx
 	mov    -0x28(%rbp),%rax
 	add    %rdx,%rax
 	mov    (%rax),%rax
 	mov    -0x14(%rbp),%edx
@@ -3021,26 +3051,26 @@
 	mov    -0x14(%rbp),%ecx
 	movslq %ecx,%rcx
 	shl    $0x3,%rcx
 	add    %rcx,%rax
 	movsd  (%rdx),%xmm0
 	movsd  %xmm0,(%rax)
 	movl   $0x0,-0xc(%rbp)
-	jmp    5312 <lu_decomposition+0x170>
+	jmp    486d <lu_decomposition+0x170>
 	mov    -0x10(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,8),%rdx
 	mov    -0x30(%rbp),%rax
 	add    %rdx,%rax
 	mov    (%rax),%rax
 	mov    -0x14(%rbp),%edx
 	movslq %edx,%rdx
 	shl    $0x3,%rdx
 	add    %rdx,%rax
-	movsd  (%rax),%xmm0
+	movsd  (%rax),%xmm1
 	mov    -0x10(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,8),%rdx
 	mov    -0x30(%rbp),%rax
 	add    %rdx,%rax
 	mov    (%rax),%rax
 	mov    -0xc(%rbp),%edx
@@ -3054,70 +3084,71 @@
 	mov    -0x38(%rbp),%rax
 	add    %rdx,%rax
 	mov    (%rax),%rax
 	mov    -0x14(%rbp),%edx
 	movslq %edx,%rdx
 	shl    $0x3,%rdx
 	add    %rdx,%rax
-	movsd  (%rax),%xmm1
-	mulsd  %xmm2,%xmm1
+	movsd  (%rax),%xmm0
+	mulsd  %xmm2,%xmm0
 	mov    -0x10(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,8),%rdx
 	mov    -0x30(%rbp),%rax
 	add    %rdx,%rax
 	mov    (%rax),%rax
 	mov    -0x14(%rbp),%edx
 	movslq %edx,%rdx
 	shl    $0x3,%rdx
 	add    %rdx,%rax
-	subsd  %xmm1,%xmm0
+	subsd  %xmm0,%xmm1
+	movapd %xmm1,%xmm0
 	movsd  %xmm0,(%rax)
 	addl   $0x1,-0xc(%rbp)
 	mov    -0xc(%rbp),%eax
 	cmp    -0x14(%rbp),%eax
-	jl     5266 <lu_decomposition+0xc4>
+	jl     47bd <lu_decomposition+0xc0>
 	addl   $0x1,-0x10(%rbp)
 	mov    -0x10(%rbp),%eax
 	cmp    -0x3c(%rbp),%eax
-	jl     51d1 <lu_decomposition+0x2f>
+	jl     4728 <lu_decomposition+0x2b>
 	movl   $0x0,-0x8(%rbp)
-	jmp    5520 <lu_decomposition+0x37e>
+	jmp    4a7f <lu_decomposition+0x382>
 	mov    -0x8(%rbp),%eax
 	cmp    -0x14(%rbp),%eax
-	jge    5373 <lu_decomposition+0x1d1>
+	jge    48ce <lu_decomposition+0x1d1>
 	mov    -0x14(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,8),%rdx
 	mov    -0x38(%rbp),%rax
 	add    %rdx,%rax
 	mov    (%rax),%rax
 	mov    -0x8(%rbp),%edx
 	movslq %edx,%rdx
 	shl    $0x3,%rdx
 	add    %rdx,%rax
 	pxor   %xmm0,%xmm0
 	movsd  %xmm0,(%rax)
-	jmp    551c <lu_decomposition+0x37a>
+	jmp    4a7b <lu_decomposition+0x37e>
 	mov    -0x8(%rbp),%eax
 	cmp    -0x14(%rbp),%eax
-	jne    53b0 <lu_decomposition+0x20e>
+	jne    490b <lu_decomposition+0x20e>
 	mov    -0x14(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,8),%rdx
 	mov    -0x38(%rbp),%rax
 	add    %rdx,%rax
 	mov    (%rax),%rax
 	mov    -0x8(%rbp),%edx
 	movslq %edx,%rdx
 	shl    $0x3,%rdx
 	add    %rdx,%rax
-	movsd  0x1d39(%rip),%xmm0        
+	movsd  0x146e(%rip),%xmm0        
 	movsd  %xmm0,(%rax)
-	jmp    551c <lu_decomposition+0x37a>
+	jmp    4a7b <lu_decomposition+0x37e>
 	mov    -0x14(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,8),%rdx
 	mov    -0x28(%rbp),%rax
 	add    %rdx,%rax
 	mov    (%rax),%rax
 	mov    -0x8(%rbp),%edx
@@ -3145,26 +3176,26 @@
 	mov    -0x8(%rbp),%edx
 	movslq %edx,%rdx
 	shl    $0x3,%rdx
 	add    %rdx,%rax
 	divsd  %xmm1,%xmm0
 	movsd  %xmm0,(%rax)
 	movl   $0x0,-0x4(%rbp)
-	jmp    5510 <lu_decomposition+0x36e>
+	jmp    4a6f <lu_decomposition+0x372>
 	mov    -0x14(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,8),%rdx
 	mov    -0x38(%rbp),%rax
 	add    %rdx,%rax
 	mov    (%rax),%rax
 	mov    -0x8(%rbp),%edx
 	movslq %edx,%rdx
 	shl    $0x3,%rdx
 	add    %rdx,%rax
-	movsd  (%rax),%xmm0
+	movsd  (%rax),%xmm1
 	mov    -0x14(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,8),%rdx
 	mov    -0x30(%rbp),%rax
 	add    %rdx,%rax
 	mov    (%rax),%rax
 	mov    -0x4(%rbp),%edx
@@ -3178,129 +3209,126 @@
 	mov    -0x38(%rbp),%rax
 	add    %rdx,%rax
 	mov    (%rax),%rax
 	mov    -0x8(%rbp),%edx
 	movslq %edx,%rdx
 	shl    $0x3,%rdx
 	add    %rdx,%rax
-	movsd  (%rax),%xmm1
-	mulsd  %xmm2,%xmm1
+	movsd  (%rax),%xmm0
+	mulsd  %xmm2,%xmm0
 	mov    -0x14(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,8),%rdx
 	mov    -0x30(%rbp),%rax
 	add    %rdx,%rax
 	mov    (%rax),%rax
 	mov    -0x14(%rbp),%edx
 	movslq %edx,%rdx
 	shl    $0x3,%rdx
 	add    %rdx,%rax
 	movsd  (%rax),%xmm2
-	divsd  %xmm2,%xmm1
+	divsd  %xmm2,%xmm0
 	mov    -0x14(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,8),%rdx
 	mov    -0x38(%rbp),%rax
 	add    %rdx,%rax
 	mov    (%rax),%rax
 	mov    -0x8(%rbp),%edx
 	movslq %edx,%rdx
 	shl    $0x3,%rdx
 	add    %rdx,%rax
-	subsd  %xmm1,%xmm0
+	subsd  %xmm0,%xmm1
+	movapd %xmm1,%xmm0
 	movsd  %xmm0,(%rax)
 	addl   $0x1,-0x4(%rbp)
 	mov    -0x4(%rbp),%eax
 	cmp    -0x14(%rbp),%eax
-	jl     5438 <lu_decomposition+0x296>
+	jl     4993 <lu_decomposition+0x296>
 	addl   $0x1,-0x8(%rbp)
 	mov    -0x8(%rbp),%eax
 	cmp    -0x3c(%rbp),%eax
-	jl     533a <lu_decomposition+0x198>
+	jl     4895 <lu_decomposition+0x198>
 	addl   $0x1,-0x14(%rbp)
 	mov    -0x14(%rbp),%eax
 	cmp    -0x3c(%rbp),%eax
-	jl     51c5 <lu_decomposition+0x23>
-	nop
+	jl     471c <lu_decomposition+0x1f>
 	nop
 	pop    %rbp
 	ret
 
-0000000000005540 <arange>:
+0000000000004a9e <arange>:
 arange():
-	endbr64
 	push   %rbp
 	mov    %rsp,%rbp
 	sub    $0x20,%rsp
 	mov    %edi,-0x14(%rbp)
 	mov    -0x14(%rbp),%eax
 	cltq
 	shl    $0x2,%rax
 	mov    %rax,%rdi
-	call   24b0 <malloc@plt>
+	call   1980 <malloc@plt>
 	mov    %rax,-0x8(%rbp)
 	movl   $0x0,-0xc(%rbp)
-	jmp    558a <arange+0x4a>
+	jmp    4ae4 <arange+0x46>
 	mov    -0xc(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,4),%rdx
 	mov    -0x8(%rbp),%rax
 	add    %rax,%rdx
 	mov    -0xc(%rbp),%eax
 	mov    %eax,(%rdx)
 	addl   $0x1,-0xc(%rbp)
 	mov    -0xc(%rbp),%eax
 	cmp    -0x14(%rbp),%eax
-	jl     556d <arange+0x2d>
+	jl     4ac7 <arange+0x29>
 	mov    -0x8(%rbp),%rax
 	leave
 	ret
 
-0000000000005598 <d_arange>:
+0000000000004af2 <d_arange>:
 d_arange():
-	endbr64
 	push   %rbp
 	mov    %rsp,%rbp
 	sub    $0x20,%rsp
 	mov    %edi,-0x14(%rbp)
 	mov    -0x14(%rbp),%eax
 	cltq
 	shl    $0x3,%rax
 	mov    %rax,%rdi
-	call   24b0 <malloc@plt>
+	call   1980 <malloc@plt>
 	mov    %rax,-0x8(%rbp)
 	movl   $0x0,-0xc(%rbp)
-	jmp    55e6 <d_arange+0x4e>
+	jmp    4b3c <d_arange+0x4a>
 	mov    -0xc(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,8),%rdx
 	mov    -0x8(%rbp),%rax
 	add    %rdx,%rax
 	cvtsi2sdl -0xc(%rbp),%xmm0
 	movsd  %xmm0,(%rax)
 	addl   $0x1,-0xc(%rbp)
 	mov    -0xc(%rbp),%eax
 	cmp    -0x14(%rbp),%eax
-	jl     55c5 <d_arange+0x2d>
+	jl     4b1b <d_arange+0x29>
 	mov    -0x8(%rbp),%rax
 	leave
 	ret
 
-00000000000055f4 <pdist>:
+0000000000004b4a <pdist>:
 pdist():
-	endbr64
 	push   %rbp
 	mov    %rsp,%rbp
 	mov    %rdi,-0x18(%rbp)
 	mov    %rsi,-0x20(%rbp)
 	mov    %edx,-0x24(%rbp)
 	movl   $0x0,-0x8(%rbp)
-	jmp    5694 <pdist+0xa0>
+	jmp    4be6 <pdist+0x9c>
 	movl   $0x0,-0x4(%rbp)
-	jmp    5688 <pdist+0x94>
+	jmp    4bda <pdist+0x90>
 	mov    -0x4(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,8),%rdx
 	mov    -0x18(%rbp),%rax
 	add    %rdx,%rax
 	movsd  (%rax),%xmm0
 	mov    -0x8(%rbp),%eax
@@ -3316,42 +3344,40 @@
 	mov    -0x20(%rbp),%rax
 	add    %rdx,%rax
 	mov    (%rax),%rax
 	mov    -0x4(%rbp),%edx
 	movslq %edx,%rdx
 	shl    $0x3,%rdx
 	add    %rdx,%rax
-	movq   0x1a74(%rip),%xmm1        
+	movq   0x11b2(%rip),%xmm1        
 	andpd  %xmm1,%xmm0
 	movsd  %xmm0,(%rax)
 	addl   $0x1,-0x4(%rbp)
 	mov    -0x4(%rbp),%eax
 	cmp    -0x24(%rbp),%eax
-	jl     561c <pdist+0x28>
+	jl     4b6e <pdist+0x24>
 	addl   $0x1,-0x8(%rbp)
 	mov    -0x8(%rbp),%eax
 	cmp    -0x24(%rbp),%eax
-	jl     5613 <pdist+0x1f>
-	nop
+	jl     4b65 <pdist+0x1b>
 	nop
 	pop    %rbp
 	ret
 
-00000000000056a4 <matrixform>:
+0000000000004bf5 <matrixform>:
 matrixform():
-	endbr64
 	push   %rbp
 	mov    %rsp,%rbp
 	mov    %rdi,-0x18(%rbp)
 	mov    %rsi,-0x20(%rbp)
 	mov    %edx,-0x24(%rbp)
 	movl   $0x0,-0x8(%rbp)
-	jmp    5724 <matrixform+0x80>
+	jmp    4c71 <matrixform+0x7c>
 	movl   $0x0,-0x4(%rbp)
-	jmp    5718 <matrixform+0x74>
+	jmp    4c65 <matrixform+0x70>
 	mov    -0x24(%rbp),%eax
 	imul   -0x8(%rbp),%eax
 	mov    %eax,%edx
 	mov    -0x4(%rbp),%eax
 	add    %edx,%eax
 	cltq
 	lea    0x0(,%rax,8),%rdx
@@ -3368,136 +3394,136 @@
 	shl    $0x3,%rcx
 	add    %rcx,%rax
 	movsd  (%rdx),%xmm0
 	movsd  %xmm0,(%rax)
 	addl   $0x1,-0x4(%rbp)
 	mov    -0x4(%rbp),%eax
 	cmp    -0x24(%rbp),%eax
-	jl     56c9 <matrixform+0x25>
+	jl     4c16 <matrixform+0x21>
 	addl   $0x1,-0x8(%rbp)
 	mov    -0x8(%rbp),%eax
 	cmp    -0x24(%rbp),%eax
-	jl     56c0 <matrixform+0x1c>
-	nop
+	jl     4c0d <matrixform+0x18>
 	nop
 	pop    %rbp
 	ret
 
-0000000000005730 <save_1darray>:
+0000000000004c7c <save_1darray>:
 save_1darray():
-	endbr64
 	push   %rbp
 	mov    %rsp,%rbp
 	sub    $0x1e0,%rsp
 	mov    %rdi,-0x1b8(%rbp)
 	mov    %esi,-0x1bc(%rbp)
 	mov    %rdx,-0x1c8(%rbp)
 	mov    %rcx,-0x1d0(%rbp)
 	mov    %r8d,-0x1c0(%rbp)
 	mov    %r9d,-0x1d4(%rbp)
 	mov    %fs:0x28,%rax
 	mov    %rax,-0x8(%rbp)
 	xor    %eax,%eax
 	cvtsi2sdl -0x1c0(%rbp),%xmm0
-	call   2570 <log10@plt>
-	call   2350 <ceil@plt>
+	call   1a40 <log10@plt>
+	call   1820 <ceil@plt>
 	cvttsd2si %xmm0,%eax
 	add    $0x1,%eax
 	mov    %eax,-0x1ac(%rbp)
 	mov    -0x1ac(%rbp),%esi
 	mov    -0x1c8(%rbp),%rcx
 	mov    -0x1d0(%rbp),%rdx
 	lea    -0x1a0(%rbp),%rax
 	mov    %esi,%r9d
 	mov    %rcx,%r8
 	mov    %rdx,%rcx
-	lea    0x18cf(%rip),%rdx        
+	lea    0x1017(%rip),%rdx        
 	mov    $0xc8,%esi
 	mov    %rax,%rdi
 	mov    $0x0,%eax
-	call   23e0 <snprintf@plt>
+	call   18b0 <snprintf@plt>
 	mov    -0x1d0(%rbp),%rax
 	mov    $0x1f8,%esi
 	mov    %rax,%rdi
-	call   2330 <mkdir@plt>
+	call   1800 <mkdir@plt>
 	cmp    $0xffffffff,%eax
-	jne    5809 <save_1darray+0xd9>
-	call   2310 <__errno_location@plt>
+	jne    4d51 <save_1darray+0xd5>
+	call   17e0 <__errno_location@plt>
 	mov    (%rax),%eax
 	cmp    $0x11,%eax
-	je     5809 <save_1darray+0xd9>
-	lea    0x18a0(%rip),%rdi        
+	je     4d51 <save_1darray+0xd5>
+	lea    0xfe8(%rip),%rdi        
 	mov    $0x0,%eax
-	call   23c0 <printf@plt>
+	call   1890 <printf@plt>
 	mov    -0x1d4(%rbp),%ecx
 	lea    -0x1a0(%rbp),%rdx
 	lea    -0xd0(%rbp),%rax
 	mov    $0xc8,%esi
 	mov    %rax,%rdi
 	mov    $0x0,%eax
-	call   23e0 <snprintf@plt>
+	call   18b0 <snprintf@plt>
 	lea    -0xd0(%rbp),%rax
-	lea    0x1878(%rip),%rsi        
+	lea    0xfc0(%rip),%rsi        
 	mov    %rax,%rdi
-	call   2530 <fopen@plt>
+	call   1a00 <fopen@plt>
 	mov    %rax,-0x1a8(%rbp)
 	cmpq   $0x0,-0x1a8(%rbp)
-	jne    586c <save_1darray+0x13c>
-	lea    0x185a(%rip),%rdi        
-	call   2560 <perror@plt>
+	jne    4db4 <save_1darray+0x138>
+	lea    0xfa2(%rip),%rdi        
+	call   1a30 <perror@plt>
 	mov    $0x1,%edi
-	call   25a0 <exit@plt>
+	call   1a70 <exit@plt>
 	movl   $0x0,-0x1b0(%rbp)
-	jmp    58c2 <save_1darray+0x192>
+	jmp    4e14 <save_1darray+0x198>
 	mov    -0x1b0(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,8),%rdx
 	mov    -0x1b8(%rbp),%rax
 	add    %rdx,%rax
 	mov    (%rax),%rcx
 	mov    -0x1b0(%rbp),%edx
 	mov    -0x1a8(%rbp),%rax
-	movq   %rcx,%xmm0
-	lea    0x1821(%rip),%rsi        
+	mov    %rcx,-0x1e0(%rbp)
+	movsd  -0x1e0(%rbp),%xmm0
+	lea    0xf5f(%rip),%rsi        
 	mov    %rax,%rdi
 	mov    $0x1,%eax
-	call   2470 <fprintf@plt>
+	call   1940 <fprintf@plt>
 	addl   $0x1,-0x1b0(%rbp)
 	mov    -0x1b0(%rbp),%eax
 	cmp    -0x1bc(%rbp),%eax
-	jl     5878 <save_1darray+0x148>
+	jl     4dc0 <save_1darray+0x144>
 	mov    -0x1a8(%rbp),%rax
 	mov    %rax,%rdi
-	call   2380 <fclose@plt>
+	call   1850 <fclose@plt>
 	nop
 	mov    -0x8(%rbp),%rax
 	xor    %fs:0x28,%rax
-	je     58f4 <save_1darray+0x1c4>
-	call   2390 <__stack_chk_fail@plt>
+	je     4e46 <save_1darray+0x1ca>
+	call   1860 <__stack_chk_fail@plt>
 	leave
 	ret
 
-00000000000058f6 <randompath>:
+0000000000004e48 <randompath>:
 randompath():
-	endbr64
 	push   %rbp
 	mov    %rsp,%rbp
 	sub    $0x30,%rsp
 	mov    %rdi,-0x18(%rbp)
 	mov    %esi,-0x1c(%rbp)
 	mov    %rdx,-0x28(%rbp)
 	mov    -0x1c(%rbp),%eax
 	sub    $0x1,%eax
 	mov    %eax,-0xc(%rbp)
-	jmp    599e <randompath+0xa8>
+	jmp    4ef2 <randompath+0xaa>
 	mov    -0x28(%rbp),%rax
 	mov    %rax,%rdi
-	call   2440 <mt19937_generate@plt>
-	mov    -0xc(%rbp),%edx
-	movslq %edx,%rcx
+	call   1910 <mt19937_generate@plt>
+	mov    %rax,%rdx
+	mov    -0xc(%rbp),%eax
+	movslq %eax,%rcx
+	mov    %rdx,%rax
 	mov    $0x0,%edx
 	div    %rcx
 	mov    %rdx,%rax
 	mov    %eax,-0x8(%rbp)
 	mov    -0x8(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,4),%rdx
@@ -3522,22 +3548,21 @@
 	lea    0x0(,%rax,4),%rdx
 	mov    -0x18(%rbp),%rax
 	add    %rax,%rdx
 	mov    -0x4(%rbp),%eax
 	mov    %eax,(%rdx)
 	subl   $0x1,-0xc(%rbp)
 	cmpl   $0x0,-0xc(%rbp)
-	jne    591b <randompath+0x25>
+	jne    4e69 <randompath+0x21>
 	mov    -0x18(%rbp),%rax
 	leave
 	ret
 
-00000000000059ae <sgsim_init>:
+0000000000004f02 <sgsim_init>:
 sgsim_init():
-	endbr64
 	push   %rbp
 	mov    %rsp,%rbp
 	sub    $0x30,%rsp
 	mov    %rdi,-0x18(%rbp)
 	mov    %esi,-0x1c(%rbp)
 	mov    %edx,-0x20(%rbp)
 	mov    %ecx,-0x24(%rbp)
@@ -3548,35 +3573,34 @@
 	mov    -0x18(%rbp),%rax
 	mov    -0x20(%rbp),%edx
 	mov    %edx,0x4(%rax)
 	mov    -0x18(%rbp),%rax
 	mov    -0x24(%rbp),%edx
 	mov    %edx,0x8(%rax)
 	cmpl   $0x1,-0x28(%rbp)
-	jne    5a1c <sgsim_init+0x6e>
+	jne    4f6c <sgsim_init+0x6a>
 	mov    -0x1c(%rbp),%eax
 	movslq %eax,%rdx
 	mov    -0x20(%rbp),%eax
 	cltq
 	imul   %rdx,%rax
 	mov    %rax,-0x8(%rbp)
 	mov    -0x8(%rbp),%rax
 	shl    $0x3,%rax
 	mov    %rax,%rdi
-	call   24b0 <malloc@plt>
+	call   1980 <malloc@plt>
 	mov    %rax,%rdx
 	mov    -0x18(%rbp),%rax
 	mov    %rdx,0x10(%rax)
 	nop
 	leave
 	ret
 
-0000000000005a1f <sgsim_run>:
+0000000000004f6f <sgsim_run>:
 sgsim_run():
-	endbr64
 	push   %rbp
 	mov    %rsp,%rbp
 	sub    $0xa00,%rsp
 	mov    %rdi,-0x9e8(%rbp)
 	mov    %rsi,-0x9f0(%rbp)
 	mov    %edx,-0x9f4(%rbp)
 	mov    %fs:0x28,%rax
@@ -3584,312 +3608,308 @@
 	xor    %eax,%eax
 	mov    -0x9e8(%rbp),%rax
 	mov    0x8(%rax),%eax
 	mov    %eax,%edx
 	lea    -0x9d0(%rbp),%rax
 	mov    %edx,%esi
 	mov    %rax,%rdi
-	call   2490 <mt19937_init@plt>
+	call   1960 <mt19937_init@plt>
 	mov    -0x9e8(%rbp),%rax
 	mov    (%rax),%eax
 	mov    %eax,%esi
-	lea    0x39a0(%rip),%rdi        
-	call   2510 <sampling_state_init@plt>
+	lea    0x202454(%rip),%rdi        
+	call   19e0 <sampling_state_init@plt>
 	mov    -0x9f0(%rbp),%rax
 	mov    0x8(%rax),%eax
 	cltq
-	mov    %rax,0x3950(%rip)        
+	mov    %rax,0x202404(%rip)        
 	mov    -0x9f0(%rbp),%rax
 	mov    0x8(%rax),%eax
 	cltq
-	mov    %rax,0x3945(%rip)        
+	mov    %rax,0x2023f9(%rip)        
 	mov    -0x9f0(%rbp),%rax
 	mov    0x8(%rax),%eax
 	cltq
 	mov    $0x8,%esi
 	mov    %rax,%rdi
-	call   2460 <calloc@plt>
-	mov    %rax,0x3915(%rip)        
+	call   1930 <calloc@plt>
+	mov    %rax,0x2023c9(%rip)        
 	mov    -0x9e8(%rbp),%rax
 	mov    (%rax),%eax
 	cltq
-	mov    %rax,0x392b(%rip)        
+	mov    %rax,0x2023df(%rip)        
 	mov    -0x9e8(%rbp),%rax
 	mov    (%rax),%eax
 	cltq
-	mov    %rax,0x3921(%rip)        
+	mov    %rax,0x2023d5(%rip)        
 	mov    -0x9e8(%rbp),%rax
 	mov    (%rax),%eax
 	cltq
 	mov    $0x8,%esi
 	mov    %rax,%rdi
-	call   2460 <calloc@plt>
-	mov    %rax,0x38f2(%rip)        
-	mov    -0x9f0(%rbp),%rax
-	movsd  0x18(%rax),%xmm0
-	mov    -0x9f0(%rbp),%rax
-	mov    0x10(%rax),%rax
-	movapd %xmm0,%xmm1
-	movq   %rax,%xmm0
-	call   2480 <krige_param_setting@plt>
+	call   1930 <calloc@plt>
+	mov    %rax,0x2023a6(%rip)        
+	mov    -0x9e8(%rbp),%rax
+	mov    (%rax),%eax
+	mov    -0x9f0(%rbp),%rdx
+	mov    %rdx,%rsi
+	mov    %eax,%edi
+	call   1950 <krige_param_setting@plt>
 	mov    -0x9e8(%rbp),%rax
 	mov    (%rax),%eax
 	mov    %eax,%edi
-	call   24c0 <arange@plt>
-	mov    %rax,0x3836(%rip)        
-	movl   $0x0,0x3918(%rip)        
-	jmp    5eda <sgsim_run+0x4bb>
-	mov    0x390d(%rip),%eax        
+	call   1990 <arange@plt>
+	mov    %rax,0x2022f5(%rip)        
+	movl   $0x0,0x2023d7(%rip)        
+	jmp    541b <sgsim_run+0x4ac>
+	mov    0x2023cc(%rip),%eax        
 	mov    %eax,%esi
-	lea    0x1598(%rip),%rdi        
+	lea    0xce7(%rip),%rdi        
 	mov    $0x0,%eax
-	call   23c0 <printf@plt>
-	movl   $0x0,0x38a8(%rip)        
-	movl   $0x0,0x389a(%rip)        
-	movl   $0x0,0x38d8(%rip)        
+	call   1890 <printf@plt>
+	movl   $0x0,0x202367(%rip)        
+	movl   $0x0,0x202359(%rip)        
+	movl   $0x0,0x202397(%rip)        
 	mov    -0x9e8(%rbp),%rax
 	mov    (%rax),%ecx
-	mov    0x37e0(%rip),%rax        
+	mov    0x20229f(%rip),%rax        
 	lea    -0x9d0(%rbp),%rdx
 	mov    %ecx,%esi
 	mov    %rax,%rdi
-	call   2340 <randompath@plt>
-	mov    %rax,0x37c8(%rip)        
+	call   1810 <randompath@plt>
+	mov    %rax,0x202287(%rip)        
 	movl   $0x0,-0x9d8(%rbp)
-	jmp    5c2c <sgsim_run+0x20d>
-	mov    0x3835(%rip),%rax        
+	jmp    516d <sgsim_run+0x1fe>
+	mov    0x2022f4(%rip),%rax        
 	mov    -0x9d8(%rbp),%edx
 	movslq %edx,%rdx
 	shl    $0x3,%rdx
 	add    %rdx,%rax
 	pxor   %xmm0,%xmm0
 	movsd  %xmm0,(%rax)
-	mov    0x384e(%rip),%rax        
+	mov    0x20230d(%rip),%rax        
 	mov    -0x9d8(%rbp),%edx
 	movslq %edx,%rdx
 	shl    $0x3,%rdx
 	add    %rdx,%rax
 	pxor   %xmm0,%xmm0
 	movsd  %xmm0,(%rax)
-	mov    0x3847(%rip),%rax        
+	mov    0x202306(%rip),%rax        
 	mov    -0x9d8(%rbp),%edx
 	movslq %edx,%rdx
 	shl    $0x3,%rdx
 	add    %rdx,%rax
-	movsd  0x152f(%rip),%xmm0        
+	movsd  0xc7e(%rip),%xmm0        
 	movsd  %xmm0,(%rax)
 	addl   $0x1,-0x9d8(%rbp)
 	mov    -0x9e8(%rbp),%rax
 	mov    (%rax),%eax
 	cmp    %eax,-0x9d8(%rbp)
-	jl     5bc4 <sgsim_run+0x1a5>
+	jl     5105 <sgsim_run+0x196>
 	movl   $0x0,-0x9d4(%rbp)
-	jmp    5dd7 <sgsim_run+0x3b8>
-	mov    0x372d(%rip),%rax        
+	jmp    5318 <sgsim_run+0x3a9>
+	mov    0x2021ec(%rip),%rax        
 	mov    -0x9d4(%rbp),%edx
 	movslq %edx,%rdx
 	shl    $0x2,%rdx
 	add    %rdx,%rax
 	mov    (%rax),%eax
 	cvtsi2sd %eax,%xmm0
 	mov    -0x9d4(%rbp),%eax
 	mov    %eax,%esi
-	lea    0x37a8(%rip),%rdi        
-	call   2370 <sampling_state_update@plt>
-	mov    0x377c(%rip),%rax        
+	lea    0x202267(%rip),%rdi        
+	call   1840 <sampling_state_update@plt>
+	mov    0x20223b(%rip),%rax        
 	lea    -0x9d0(%rbp),%rdx
-	lea    0x378e(%rip),%rsi        
+	lea    0x20224d(%rip),%rsi        
 	mov    %rax,%rdi
-	call   24a0 <simple_kriging@plt>
-	mov    0x375f(%rip),%rax        
-	mov    0x36d8(%rip),%rdx        
+	call   1970 <simple_kriging@plt>
+	mov    0x20221e(%rip),%rax        
+	mov    0x202197(%rip),%rdx        
 	mov    -0x9d4(%rbp),%ecx
 	movslq %ecx,%rcx
 	shl    $0x2,%rcx
 	add    %rcx,%rdx
 	mov    (%rdx),%edx
 	movslq %edx,%rdx
 	shl    $0x3,%rdx
 	add    %rax,%rdx
 	mov    -0x9e8(%rbp),%rax
 	mov    0x10(%rax),%rcx
-	mov    0x36aa(%rip),%rax        
+	mov    0x202169(%rip),%rax        
 	mov    -0x9d4(%rbp),%esi
 	movslq %esi,%rsi
 	shl    $0x2,%rsi
 	add    %rsi,%rax
 	mov    (%rax),%esi
 	mov    -0x9e8(%rbp),%rax
 	mov    (%rax),%edi
-	mov    0x3775(%rip),%eax        
+	mov    0x202234(%rip),%eax        
 	imul   %edi,%eax
 	add    %esi,%eax
 	cltq
 	shl    $0x3,%rax
 	add    %rcx,%rax
 	movsd  (%rdx),%xmm0
 	movsd  %xmm0,(%rax)
-	mov    0x370d(%rip),%eax        
+	mov    0x2021cc(%rip),%eax        
 	cmp    $0x7,%eax
-	jg     5d27 <sgsim_run+0x308>
-	mov    0x3702(%rip),%eax        
+	jg     5268 <sgsim_run+0x2f9>
+	mov    0x2021c1(%rip),%eax        
 	add    $0x1,%eax
-	mov    %eax,0x36f9(%rip)        
-	mov    0x3652(%rip),%rax        
+	mov    %eax,0x2021b8(%rip)        
+	mov    0x202111(%rip),%rax        
 	mov    -0x9d4(%rbp),%edx
 	movslq %edx,%rdx
 	shl    $0x2,%rdx
 	add    %rdx,%rax
 	mov    (%rax),%ecx
-	mov    0x36f1(%rip),%rax        
+	mov    0x2021b0(%rip),%rax        
 	mov    -0x9d4(%rbp),%edx
 	movslq %edx,%rdx
 	shl    $0x3,%rdx
 	add    %rdx,%rax
 	cvtsi2sd %ecx,%xmm0
 	movsd  %xmm0,(%rax)
-	mov    0x36bf(%rip),%eax        
+	mov    0x20217e(%rip),%eax        
 	add    $0x1,%eax
-	mov    %eax,0x36b6(%rip)        
-	mov    0x368b(%rip),%rax        
-	mov    0x3604(%rip),%rdx        
+	mov    %eax,0x202175(%rip)        
+	mov    0x20214a(%rip),%rax        
+	mov    0x2020c3(%rip),%rdx        
 	mov    -0x9d4(%rbp),%ecx
 	movslq %ecx,%rcx
 	shl    $0x2,%rcx
 	add    %rcx,%rdx
 	mov    (%rdx),%edx
 	movslq %edx,%rdx
 	shl    $0x3,%rdx
 	add    %rdx,%rax
-	movsd  (%rax),%xmm0
-	movq   0x13bc(%rip),%xmm1        
-	andpd  %xmm0,%xmm1
-	movsd  0x13c0(%rip),%xmm0        
-	ucomisd %xmm1,%xmm0
+	movsd  (%rax),%xmm1
+	movq   0xb0b(%rip),%xmm0        
+	andpd  %xmm1,%xmm0
+	movsd  0xb0f(%rip),%xmm1        
+	ucomisd %xmm0,%xmm1
 	setb   %al
 	xor    $0x1,%eax
 	movzbl %al,%eax
 	test   %eax,%eax
-	jne    5dd0 <sgsim_run+0x3b1>
-	mov    0x36a1(%rip),%eax        
+	jne    5311 <sgsim_run+0x3a2>
+	mov    0x202160(%rip),%eax        
 	add    $0x1,%eax
-	mov    %eax,0x3698(%rip)        
+	mov    %eax,0x202157(%rip)        
 	addl   $0x1,-0x9d4(%rbp)
 	mov    -0x9e8(%rbp),%rax
 	mov    (%rax),%eax
 	cmp    %eax,-0x9d4(%rbp)
-	jl     5c4c <sgsim_run+0x22d>
-	mov    0x367a(%rip),%eax        
+	jl     518d <sgsim_run+0x21e>
+	mov    0x202139(%rip),%eax        
 	add    $0x1,%eax
-	mov    %eax,0x3671(%rip)        
+	mov    %eax,0x202130(%rip)        
 	cmpl   $0x1,-0x9f4(%rbp)
-	jne    5e3a <sgsim_run+0x41b>
+	jne    537b <sgsim_run+0x40c>
 	mov    -0x9f0(%rbp),%rax
 	mov    0x4(%rax),%edi
 	mov    -0x9f0(%rbp),%rax
 	mov    0x8(%rax),%ecx
 	mov    -0x9e8(%rbp),%rax
 	mov    (%rax),%edx
-	mov    0x35b8(%rip),%rsi        
-	mov    0x35d1(%rip),%rax        
+	mov    0x202077(%rip),%rsi        
+	mov    0x202090(%rip),%rax        
 	mov    %edi,%r8d
 	mov    %rax,%rdi
-	call   24f0 <variogram@plt>
-	mov    0x3628(%rip),%eax        
+	call   19c0 <variogram@plt>
+	mov    0x2020e7(%rip),%eax        
 	test   %eax,%eax
-	jle    5e58 <sgsim_run+0x439>
-	mov    0x3622(%rip),%eax        
+	jle    5399 <sgsim_run+0x42a>
+	mov    0x2020e1(%rip),%eax        
 	sub    $0x1,%eax
-	mov    %eax,0x3619(%rip)        
-	jmp    5eda <sgsim_run+0x4bb>
-	mov    0x360e(%rip),%ecx        
+	mov    %eax,0x2020d8(%rip)        
+	jmp    541b <sgsim_run+0x4ac>
+	mov    0x2020cd(%rip),%ecx        
 	mov    -0x9e8(%rbp),%rax
 	mov    0x4(%rax),%edx
 	mov    -0x9e8(%rbp),%rax
 	mov    (%rax),%esi
-	mov    0x3588(%rip),%rax        
+	mov    0x202047(%rip),%rax        
 	mov    %ecx,%r9d
 	mov    %edx,%r8d
-	lea    0x1288(%rip),%rcx        
-	lea    0x1291(%rip),%rdx        
+	lea    0x9d7(%rip),%rcx        
+	lea    0x9e0(%rip),%rdx        
 	mov    %rax,%rdi
-	call   23a0 <save_1darray@plt>
+	call   1870 <save_1darray@plt>
 	cmpl   $0x1,-0x9f4(%rbp)
-	jne    5eda <sgsim_run+0x4bb>
-	mov    0x35c9(%rip),%ecx        
+	jne    541b <sgsim_run+0x4ac>
+	mov    0x202088(%rip),%ecx        
 	mov    -0x9e8(%rbp),%rax
 	mov    0x4(%rax),%edx
 	mov    -0x9f0(%rbp),%rax
 	mov    0x8(%rax),%esi
-	mov    0x3522(%rip),%rax        
+	mov    0x201fe1(%rip),%rax        
 	mov    %ecx,%r9d
 	mov    %edx,%r8d
-	lea    0x125f(%rip),%rcx        
-	lea    0x1272(%rip),%rdx        
+	lea    0x9ae(%rip),%rcx        
+	lea    0x9c1(%rip),%rdx        
 	mov    %rax,%rdi
-	call   23a0 <save_1darray@plt>
+	call   1870 <save_1darray@plt>
 	mov    -0x9e8(%rbp),%rax
 	mov    0x4(%rax),%edx
-	mov    0x3582(%rip),%eax        
+	mov    0x202041(%rip),%eax        
 	cmp    %eax,%edx
-	jg     5b59 <sgsim_run+0x13a>
+	jg     509a <sgsim_run+0x12b>
 	mov    $0x0,%eax
-	call   24d0 <krige_memory_free@plt>
+	call   19a0 <krige_memory_free@plt>
 	mov    $0x0,%eax
-	call   5f40 <sgsim_memory_free>
+	call   547d <sgsim_memory_free>
 	nop
 	mov    -0x8(%rbp),%rax
 	xor    %fs:0x28,%rax
-	je     5f1b <sgsim_run+0x4fc>
-	call   2390 <__stack_chk_fail@plt>
+	je     545c <sgsim_run+0x4ed>
+	call   1860 <__stack_chk_fail@plt>
 	leave
 	ret
 
-0000000000005f1d <sgsim_t_free>:
+000000000000545e <sgsim_t_free>:
 sgsim_t_free():
-	endbr64
 	push   %rbp
 	mov    %rsp,%rbp
 	sub    $0x10,%rsp
 	mov    %rdi,-0x8(%rbp)
 	mov    -0x8(%rbp),%rax
 	mov    0x10(%rax),%rax
 	mov    %rax,%rdi
-	call   2300 <free@plt>
+	call   17d0 <free@plt>
 	nop
 	leave
 	ret
 
-0000000000005f40 <sgsim_memory_free>:
+000000000000547d <sgsim_memory_free>:
 sgsim_memory_free():
-	endbr64
 	push   %rbp
 	mov    %rsp,%rbp
-	mov    0x34e9(%rip),%rax        
+	mov    0x201fb0(%rip),%rax        
 	mov    %rax,%rdi
-	call   2300 <free@plt>
-	mov    0x34f2(%rip),%rax        
+	call   17d0 <free@plt>
+	mov    0x201fb9(%rip),%rax        
 	mov    %rax,%rdi
-	call   2300 <free@plt>
-	mov    0x3493(%rip),%rax        
+	call   17d0 <free@plt>
+	mov    0x201f5a(%rip),%rax        
 	mov    %rax,%rdi
-	call   2300 <free@plt>
-	mov    0x3404(%rip),%rax        
+	call   17d0 <free@plt>
+	mov    0x201ecb(%rip),%rax        
 	mov    %rax,%rdi
-	call   2300 <free@plt>
-	mov    0x3455(%rip),%rax        
+	call   17d0 <free@plt>
+	mov    0x201f1c(%rip),%rax        
 	mov    %rax,%rdi
-	call   2300 <free@plt>
+	call   17d0 <free@plt>
 	nop
 	pop    %rbp
 	ret
 
-0000000000005f96 <swap>:
+00000000000054cf <swap>:
 swap():
-	endbr64
 	push   %rbp
 	mov    %rsp,%rbp
 	mov    %rdi,-0x28(%rbp)
 	mov    %esi,-0x2c(%rbp)
 	mov    %edx,-0x30(%rbp)
 	mov    -0x30(%rbp),%eax
 	cltq
@@ -3985,17 +4005,16 @@
 	add    $0x10,%rax
 	movsd  -0x8(%rbp),%xmm0
 	movsd  %xmm0,(%rax)
 	nop
 	pop    %rbp
 	ret
 
-0000000000006123 <Partition2d>:
+0000000000005658 <Partition2d>:
 Partition2d():
-	endbr64
 	push   %rbp
 	mov    %rsp,%rbp
 	sub    $0x20,%rsp
 	mov    %rdi,-0x18(%rbp)
 	mov    %esi,-0x1c(%rbp)
 	mov    %edx,-0x20(%rbp)
 	mov    -0x20(%rbp),%eax
@@ -4020,22 +4039,22 @@
 	cltq
 	lea    0x0(,%rax,8),%rdx
 	mov    -0x18(%rbp),%rax
 	add    %rdx,%rax
 	mov    (%rax),%rax
 	add    $0x10,%rax
 	movsd  (%rax),%xmm1
-	comisd %xmm1,%xmm0
-	jbe    61aa <Partition2d+0x87>
+	ucomisd %xmm1,%xmm0
+	jbe    56db <Partition2d+0x83>
 	mov    -0x20(%rbp),%edx
 	mov    -0x1c(%rbp),%ecx
 	mov    -0x18(%rbp),%rax
 	mov    %ecx,%esi
 	mov    %rax,%rdi
-	call   25b0 <swap@plt>
+	call   1a80 <swap@plt>
 	mov    -0xc(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,8),%rdx
 	mov    -0x18(%rbp),%rax
 	add    %rdx,%rax
 	mov    (%rax),%rax
 	add    $0x10,%rax
@@ -4044,22 +4063,22 @@
 	cltq
 	lea    0x0(,%rax,8),%rdx
 	mov    -0x18(%rbp),%rax
 	add    %rdx,%rax
 	mov    (%rax),%rax
 	add    $0x10,%rax
 	movsd  (%rax),%xmm1
-	comisd %xmm1,%xmm0
-	jbe    6202 <Partition2d+0xdf>
+	ucomisd %xmm1,%xmm0
+	jbe    5733 <Partition2d+0xdb>
 	mov    -0x20(%rbp),%edx
 	mov    -0xc(%rbp),%ecx
 	mov    -0x18(%rbp),%rax
 	mov    %ecx,%esi
 	mov    %rax,%rdi
-	call   25b0 <swap@plt>
+	call   1a80 <swap@plt>
 	mov    -0xc(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,8),%rdx
 	mov    -0x18(%rbp),%rax
 	add    %rdx,%rax
 	mov    (%rax),%rax
 	add    $0x10,%rax
@@ -4068,120 +4087,118 @@
 	cltq
 	lea    0x0(,%rax,8),%rdx
 	mov    -0x18(%rbp),%rax
 	add    %rdx,%rax
 	mov    (%rax),%rax
 	add    $0x10,%rax
 	movsd  (%rax),%xmm1
-	comisd %xmm1,%xmm0
-	jbe    625a <Partition2d+0x137>
+	ucomisd %xmm1,%xmm0
+	jbe    578b <Partition2d+0x133>
 	mov    -0x1c(%rbp),%edx
 	mov    -0xc(%rbp),%ecx
 	mov    -0x18(%rbp),%rax
 	mov    %ecx,%esi
 	mov    %rax,%rdi
-	call   25b0 <swap@plt>
+	call   1a80 <swap@plt>
 	mov    -0x1c(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,8),%rdx
 	mov    -0x18(%rbp),%rax
 	add    %rdx,%rax
 	mov    (%rax),%rax
 	movsd  0x10(%rax),%xmm0
 	movsd  %xmm0,-0x8(%rbp)
-	jmp    6312 <Partition2d+0x1ef>
+	jmp    5843 <Partition2d+0x1eb>
 	subl   $0x1,-0x20(%rbp)
 	mov    -0x1c(%rbp),%eax
 	cmp    -0x20(%rbp),%eax
-	jge    62b2 <Partition2d+0x18f>
+	jge    57e3 <Partition2d+0x18b>
 	mov    -0x20(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,8),%rdx
 	mov    -0x18(%rbp),%rax
 	add    %rdx,%rax
 	mov    (%rax),%rax
 	add    $0x10,%rax
 	movsd  (%rax),%xmm0
-	comisd -0x8(%rbp),%xmm0
-	jae    6280 <Partition2d+0x15d>
+	ucomisd -0x8(%rbp),%xmm0
+	jae    57b1 <Partition2d+0x159>
 	mov    -0x20(%rbp),%edx
 	mov    -0x1c(%rbp),%ecx
 	mov    -0x18(%rbp),%rax
 	mov    %ecx,%esi
 	mov    %rax,%rdi
-	call   25b0 <swap@plt>
-	jmp    62cc <Partition2d+0x1a9>
+	call   1a80 <swap@plt>
+	jmp    57fd <Partition2d+0x1a5>
 	addl   $0x1,-0x1c(%rbp)
 	mov    -0x1c(%rbp),%eax
 	cmp    -0x20(%rbp),%eax
-	jge    62fe <Partition2d+0x1db>
+	jge    582f <Partition2d+0x1d7>
 	mov    -0x1c(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,8),%rdx
 	mov    -0x18(%rbp),%rax
 	add    %rdx,%rax
 	mov    (%rax),%rax
 	add    $0x10,%rax
 	movsd  (%rax),%xmm1
 	movsd  -0x8(%rbp),%xmm0
-	comisd %xmm1,%xmm0
-	jae    62c8 <Partition2d+0x1a5>
+	ucomisd %xmm1,%xmm0
+	jae    57f9 <Partition2d+0x1a1>
 	mov    -0x20(%rbp),%edx
 	mov    -0x1c(%rbp),%ecx
 	mov    -0x18(%rbp),%rax
 	mov    %ecx,%esi
 	mov    %rax,%rdi
-	call   25b0 <swap@plt>
+	call   1a80 <swap@plt>
 	mov    -0x1c(%rbp),%eax
 	cmp    -0x20(%rbp),%eax
-	jl     6284 <Partition2d+0x161>
+	jl     57b5 <Partition2d+0x15d>
 	mov    -0x1c(%rbp),%eax
 	leave
 	ret
 
-0000000000006323 <quicksort2d>:
-quicksort2d.localalias():
-	endbr64
+0000000000005854 <quicksort2d>:
+quicksort2d():
 	push   %rbp
 	mov    %rsp,%rbp
 	sub    $0x20,%rsp
 	mov    %rdi,-0x18(%rbp)
 	mov    %esi,-0x1c(%rbp)
 	mov    %edx,-0x20(%rbp)
 	mov    -0x1c(%rbp),%eax
 	cmp    -0x20(%rbp),%eax
-	jge    6386 <quicksort2d+0x63>
+	jge    58b3 <quicksort2d+0x5f>
 	mov    -0x20(%rbp),%edx
 	mov    -0x1c(%rbp),%ecx
 	mov    -0x18(%rbp),%rax
 	mov    %ecx,%esi
 	mov    %rax,%rdi
-	call   2410 <Partition2d@plt>
+	call   18e0 <Partition2d@plt>
 	mov    %eax,-0x4(%rbp)
 	mov    -0x4(%rbp),%eax
 	lea    -0x1(%rax),%edx
 	mov    -0x1c(%rbp),%ecx
 	mov    -0x18(%rbp),%rax
 	mov    %ecx,%esi
 	mov    %rax,%rdi
-	call   6323 <quicksort2d>
+	call   17f0 <quicksort2d@plt>
 	mov    -0x4(%rbp),%eax
 	lea    0x1(%rax),%ecx
 	mov    -0x20(%rbp),%edx
 	mov    -0x18(%rbp),%rax
 	mov    %ecx,%esi
 	mov    %rax,%rdi
-	call   6323 <quicksort2d>
+	call   17f0 <quicksort2d@plt>
 	nop
 	leave
 	ret
 
-0000000000006389 <variogram>:
+00000000000058b6 <variogram>:
 variogram():
-	endbr64
 	push   %rbp
 	mov    %rsp,%rbp
 	push   %rbx
 	sub    $0x98,%rsp
 	mov    %rdi,-0x88(%rbp)
 	mov    %rsi,-0x90(%rbp)
 	mov    %edx,-0x94(%rbp)
@@ -4196,71 +4213,71 @@
 	mov    -0x94(%rbp),%eax
 	cltq
 	mov    %rax,-0x20(%rbp)
 	mov    -0x94(%rbp),%eax
 	cltq
 	shl    $0x3,%rax
 	mov    %rax,%rdi
-	call   24b0 <malloc@plt>
+	call   1980 <malloc@plt>
 	mov    %rax,-0x30(%rbp)
 	movl   $0x0,-0x74(%rbp)
-	jmp    642f <variogram+0xa6>
+	jmp    5958 <variogram+0xa2>
 	mov    -0x94(%rbp),%eax
 	cltq
 	shl    $0x3,%rax
 	mov    -0x30(%rbp),%rdx
 	mov    -0x74(%rbp),%ecx
 	movslq %ecx,%rcx
 	shl    $0x3,%rcx
 	lea    (%rdx,%rcx,1),%rbx
 	mov    %rax,%rdi
-	call   24b0 <malloc@plt>
+	call   1980 <malloc@plt>
 	mov    %rax,(%rbx)
 	addl   $0x1,-0x74(%rbp)
 	mov    -0x74(%rbp),%eax
 	cmp    -0x94(%rbp),%eax
-	jl     6402 <variogram+0x79>
+	jl     592b <variogram+0x75>
 	mov    -0x94(%rbp),%eax
 	mov    %eax,%edi
-	call   2400 <d_arange@plt>
+	call   18d0 <d_arange@plt>
 	mov    %rax,-0x50(%rbp)
 	mov    -0x30(%rbp),%rcx
 	mov    -0x50(%rbp),%rax
 	mov    -0x94(%rbp),%edx
 	mov    %rcx,%rsi
 	mov    %rax,%rdi
-	call   2590 <pdist@plt>
+	call   1a60 <pdist@plt>
 	movl   $0x0,-0x70(%rbp)
-	jmp    65ec <variogram+0x263>
+	jmp    5b19 <variogram+0x263>
 	pxor   %xmm0,%xmm0
 	movsd  %xmm0,-0x60(%rbp)
 	pxor   %xmm0,%xmm0
 	movsd  %xmm0,-0x58(%rbp)
 	movl   $0x0,-0x6c(%rbp)
-	jmp    6594 <variogram+0x20b>
+	jmp    5ac1 <variogram+0x20b>
 	mov    -0x6c(%rbp),%eax
 	add    $0x1,%eax
 	mov    %eax,-0x68(%rbp)
-	jmp    6581 <variogram+0x1f8>
+	jmp    5aae <variogram+0x1f8>
 	mov    -0x30(%rbp),%rax
 	mov    -0x6c(%rbp),%edx
 	movslq %edx,%rdx
 	shl    $0x3,%rdx
 	add    %rdx,%rax
 	mov    (%rax),%rax
 	mov    -0x68(%rbp),%edx
 	movslq %edx,%rdx
 	shl    $0x3,%rdx
 	add    %rdx,%rax
-	movsd  (%rax),%xmm0
+	movsd  (%rax),%xmm1
 	mov    -0x70(%rbp),%eax
 	sub    -0x9c(%rbp),%eax
-	cvtsi2sd %eax,%xmm1
-	comisd %xmm1,%xmm0
-	jb     657d <variogram+0x1f4>
+	cvtsi2sd %eax,%xmm0
+	ucomisd %xmm0,%xmm1
+	jb     5aaa <variogram+0x1f4>
 	mov    -0x30(%rbp),%rax
 	mov    -0x6c(%rbp),%edx
 	movslq %edx,%rdx
 	shl    $0x3,%rdx
 	add    %rdx,%rax
 	mov    (%rax),%rax
 	mov    -0x68(%rbp),%edx
@@ -4268,146 +4285,149 @@
 	shl    $0x3,%rdx
 	add    %rdx,%rax
 	movsd  (%rax),%xmm1
 	mov    -0x70(%rbp),%edx
 	mov    -0x9c(%rbp),%eax
 	add    %edx,%eax
 	cvtsi2sd %eax,%xmm0
-	comisd %xmm1,%xmm0
-	jb     657d <variogram+0x1f4>
+	ucomisd %xmm1,%xmm0
+	jb     5aaa <variogram+0x1f4>
 	mov    -0x6c(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,8),%rdx
 	mov    -0x88(%rbp),%rax
 	add    %rdx,%rax
 	movsd  (%rax),%xmm0
 	mov    -0x68(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,8),%rdx
 	mov    -0x88(%rbp),%rax
 	add    %rdx,%rax
 	movsd  (%rax),%xmm1
 	subsd  %xmm1,%xmm0
-	movsd  0xc24(%rip),%xmm1        
-	call   2550 <pow@plt>
-	movsd  -0x60(%rbp),%xmm1
+	movsd  0x38b(%rip),%xmm1        
+	call   1a20 <pow@plt>
+	movapd %xmm0,%xmm1
+	movsd  -0x60(%rbp),%xmm0
 	addsd  %xmm1,%xmm0
 	movsd  %xmm0,-0x60(%rbp)
 	movsd  -0x58(%rbp),%xmm1
-	movsd  0xc0c(%rip),%xmm0        
+	movsd  0x36f(%rip),%xmm0        
 	addsd  %xmm1,%xmm0
 	movsd  %xmm0,-0x58(%rbp)
 	addl   $0x1,-0x68(%rbp)
 	mov    -0x68(%rbp),%eax
 	cmp    -0x94(%rbp),%eax
-	jl     649c <variogram+0x113>
+	jl     59c5 <variogram+0x10f>
 	addl   $0x1,-0x6c(%rbp)
 	mov    -0x6c(%rbp),%eax
 	cmp    -0x94(%rbp),%eax
-	jl     648e <variogram+0x105>
+	jl     59b7 <variogram+0x101>
 	movsd  -0x60(%rbp),%xmm0
-	comisd 0xbd8(%rip),%xmm0        
-	jb     65e3 <variogram+0x25a>
+	ucomisd 0x33b(%rip),%xmm0        
+	jb     5b10 <variogram+0x25a>
 	movsd  -0x58(%rbp),%xmm0
-	movapd %xmm0,%xmm1
-	addsd  %xmm0,%xmm1
+	addsd  %xmm0,%xmm0
 	mov    -0x70(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,8),%rdx
 	mov    -0x90(%rbp),%rax
 	add    %rdx,%rax
-	movsd  -0x60(%rbp),%xmm0
-	divsd  %xmm1,%xmm0
+	movsd  -0x60(%rbp),%xmm1
+	divsd  %xmm0,%xmm1
+	movapd %xmm1,%xmm0
 	movsd  %xmm0,(%rax)
 	mov    -0x9c(%rbp),%eax
 	add    %eax,-0x70(%rbp)
 	mov    -0x70(%rbp),%eax
 	cmp    -0x98(%rbp),%eax
-	jl     6470 <variogram+0xe7>
+	jl     5999 <variogram+0xe3>
 	mov    -0x50(%rbp),%rax
 	mov    %rax,%rdi
-	call   2300 <free@plt>
+	call   17d0 <free@plt>
 	movl   $0x0,-0x64(%rbp)
-	jmp    6630 <variogram+0x2a7>
+	jmp    5b5d <variogram+0x2a7>
 	mov    -0x30(%rbp),%rax
 	mov    -0x64(%rbp),%edx
 	movslq %edx,%rdx
 	shl    $0x3,%rdx
 	add    %rdx,%rax
 	mov    (%rax),%rax
 	mov    %rax,%rdi
-	call   2300 <free@plt>
+	call   17d0 <free@plt>
 	addl   $0x1,-0x64(%rbp)
 	mov    -0x64(%rbp),%eax
 	movslq %eax,%rdx
 	mov    -0x28(%rbp),%rax
 	cmp    %rax,%rdx
-	jb     6610 <variogram+0x287>
+	jb     5b3d <variogram+0x287>
 	mov    -0x30(%rbp),%rax
 	mov    %rax,%rdi
-	call   2300 <free@plt>
+	call   17d0 <free@plt>
 	nop
 	mov    -0x18(%rbp),%rax
 	xor    %fs:0x28,%rax
-	je     6660 <variogram+0x2d7>
-	call   2390 <__stack_chk_fail@plt>
+	je     5b8d <variogram+0x2d7>
+	call   1860 <__stack_chk_fail@plt>
 	add    $0x98,%rsp
 	pop    %rbx
 	pop    %rbp
 	ret
 
-000000000000666a <variance>:
+0000000000005b97 <variance>:
 variance():
-	endbr64
 	push   %rbp
 	mov    %rsp,%rbp
 	sub    $0x30,%rsp
 	mov    %rdi,-0x28(%rbp)
 	mov    %esi,-0x2c(%rbp)
 	pxor   %xmm0,%xmm0
 	movsd  %xmm0,-0x10(%rbp)
 	pxor   %xmm0,%xmm0
 	movsd  %xmm0,-0x8(%rbp)
 	movl   $0x0,-0x18(%rbp)
-	jmp    66c2 <variance+0x58>
+	jmp    5beb <variance+0x54>
 	mov    -0x18(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,8),%rdx
 	mov    -0x28(%rbp),%rax
 	add    %rdx,%rax
 	movsd  (%rax),%xmm0
 	movsd  -0x10(%rbp),%xmm1
 	addsd  %xmm1,%xmm0
 	movsd  %xmm0,-0x10(%rbp)
 	addl   $0x1,-0x18(%rbp)
 	mov    -0x18(%rbp),%eax
 	cmp    -0x2c(%rbp),%eax
-	jl     6698 <variance+0x2e>
-	cvtsi2sdl -0x2c(%rbp),%xmm1
-	movsd  -0x10(%rbp),%xmm0
-	divsd  %xmm1,%xmm0
+	jl     5bc1 <variance+0x2a>
+	cvtsi2sdl -0x2c(%rbp),%xmm0
+	movsd  -0x10(%rbp),%xmm1
+	divsd  %xmm0,%xmm1
+	movapd %xmm1,%xmm0
 	movsd  %xmm0,-0x10(%rbp)
 	movl   $0x0,-0x14(%rbp)
-	jmp    6722 <variance+0xb8>
+	jmp    5c53 <variance+0xbc>
 	mov    -0x14(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,8),%rdx
 	mov    -0x28(%rbp),%rax
 	add    %rdx,%rax
 	movsd  (%rax),%xmm0
 	subsd  -0x10(%rbp),%xmm0
-	movsd  0xa6d(%rip),%xmm1        
-	call   2550 <pow@plt>
-	movsd  -0x8(%rbp),%xmm1
+	movsd  0x1d0(%rip),%xmm1        
+	call   1a20 <pow@plt>
+	movapd %xmm0,%xmm1
+	movsd  -0x8(%rbp),%xmm0
 	addsd  %xmm1,%xmm0
 	movsd  %xmm0,-0x8(%rbp)
 	addl   $0x1,-0x14(%rbp)
 	mov    -0x14(%rbp),%eax
 	cmp    -0x2c(%rbp),%eax
-	jl     66e6 <variance+0x7c>
-	cvtsi2sdl -0x2c(%rbp),%xmm1
-	movsd  -0x8(%rbp),%xmm0
-	divsd  %xmm1,%xmm0
+	jl     5c13 <variance+0x7c>
+	cvtsi2sdl -0x2c(%rbp),%xmm0
+	movsd  -0x8(%rbp),%xmm1
+	divsd  %xmm0,%xmm1
+	movapd %xmm1,%xmm0
 	movsd  %xmm0,-0x8(%rbp)
 	movsd  -0x8(%rbp),%xmm0
 	leave
 	ret
```

#### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.fini {}

```diff
@@ -1,11 +1,10 @@
 
 
 
 Disassembly of section .fini:
 
-0000000000006744 <_fini>:
+0000000000005c7c <_fini>:
 _fini():
-	endbr64
 	sub    $0x8,%rsp
 	add    $0x8,%rsp
 	ret
```

#### readelf --wide --decompress --hex-dump=.rodata {}

```diff
@@ -1,28 +1,28 @@
 
 Hex dump of section '.rodata':
-  0x00007000 6d696e00 6d617800 000080cb ffff7f4b min.max........K
-  0x00007010 00000000 000070c3 00000000 00007043 ......p.......pC
-  0x00007020 00000000 00000040 0000804f 00000000 .......@...O....
-  0x00007030 00000000 0000f041 00000000 000000c0 .......A........
-  0x00007040 182d4454 fb211940 00000000 000008c0 .-DT.!.@........
-  0x00007050 00000000 0000f03f 00000000 00000000 .......?........
-  0x00007060 00000000 0000f03f 00000000 0000e03f .......?.......?
-  0x00007070 ffffffff ffffff7f 00000000 00000000 ................
-  0x00007080 83c0caa1 45b6fb3f 00000000 00000000 ....E..?........
-  0x00007090 25732573 25253025 64642e74 78740046 %s%s%%0%dd.txt.F
-  0x000070a0 6f6c6465 7220616c 72656164 79206578 older already ex
-  0x000070b0 69737421 00770046 61696c65 6420746f ist!.w.Failed to
-  0x000070c0 206f7065 6e207468 65206669 6c650025  open the file.%
-  0x000070d0 6409252e 3130660a 00000000 00000000 d.%.10f.........
-  0x000070e0 00000000 0000f03f 00000000 00000000 .......?........
-  0x000070f0 ffffffff ffffff7f 00000000 00000000 ................
-  0x00007100 4e756d62 6572203d 2025640a 002e2f52 Number = %d.../R
-  0x00007110 65616c69 7a617469 6f6e732f 00526561 ealizations/.Rea
-  0x00007120 6c697a61 74696f6e 73002e2f 5265616c lizations../Real
-  0x00007130 697a6174 696f6e73 2f566172 696f6772 izations/Variogr
-  0x00007140 616d2f00 56617269 6f677261 6d000000 am/.Variogram...
-  0x00007150 00000000 0000f0bf 00000000 00000000 ................
-  0x00007160 ffffffff ffffff7f 00000000 00000000 ................
-  0x00007170 ffffffff ffffef7f 00000000 00000040 ...............@
-  0x00007180 00000000 0000f03f 8dedb5a0 f7c6b03e .......?.......>
+  0x00005c90 6d696e00 6d617800 000080cb ffff7f4b min.max........K
+  0x00005ca0 00000000 000070c3 00000000 00007043 ......p.......pC
+  0x00005cb0 00000000 00000040 0000804f 00000000 .......@...O....
+  0x00005cc0 00000000 0000f041 00000000 000000c0 .......A........
+  0x00005cd0 182d4454 fb211940 00000000 000008c0 .-DT.!.@........
+  0x00005ce0 00000000 0000f03f 00000000 00000000 .......?........
+  0x00005cf0 00000000 0000e03f 00000000 00000000 .......?........
+  0x00005d00 ffffffff ffffff7f 00000000 00000000 ................
+  0x00005d10 83c0caa1 45b6fb3f 00000000 00000000 ....E..?........
+  0x00005d20 25732573 25253025 64642e74 78740046 %s%s%%0%dd.txt.F
+  0x00005d30 6f6c6465 7220616c 72656164 79206578 older already ex
+  0x00005d40 69737421 00770046 61696c65 6420746f ist!.w.Failed to
+  0x00005d50 206f7065 6e207468 65206669 6c650025  open the file.%
+  0x00005d60 6409252e 3130660a 00000000 00000000 d.%.10f.........
+  0x00005d70 00000000 0000f03f 00000000 00000000 .......?........
+  0x00005d80 ffffffff ffffff7f 00000000 00000000 ................
+  0x00005d90 4e756d62 6572203d 2025640a 002e2f52 Number = %d.../R
+  0x00005da0 65616c69 7a617469 6f6e732f 00526561 ealizations/.Rea
+  0x00005db0 6c697a61 74696f6e 73002e2f 5265616c lizations../Real
+  0x00005dc0 697a6174 696f6e73 2f566172 696f6772 izations/Variogr
+  0x00005dd0 616d2f00 56617269 6f677261 6d000000 am/.Variogram...
+  0x00005de0 00000000 0000f0bf 00000000 00000000 ................
+  0x00005df0 ffffffff ffffff7f 00000000 00000000 ................
+  0x00005e00 ffffffff ffffef7f 00000000 00000040 ...............@
+  0x00005e10 00000000 0000f03f 8dedb5a0 f7c6b03e .......?.......>
```

#### readelf --wide --decompress --hex-dump=.eh_frame_hdr {}

```diff
@@ -1,37 +1,36 @@
 
 Hex dump of section '.eh_frame_hdr':
-  0x00007190 011b033b 14020000 41000000 90aeffff ...;....A.......
-  0x000071a0 30020000 60b1ffff 58020000 70b1ffff 0...`...X...p...
-  0x000071b0 70020000 e9b4ffff 88020000 78b6ffff p...........x...
-  0x000071c0 a8020000 35b8ffff c8020000 0fbaffff ....5...........
-  0x000071d0 e8020000 eebbffff 08030000 95bdffff ................
-  0x000071e0 28030000 6bbfffff 48030000 5fc1ffff (...k...H..._...
-  0x000071f0 68030000 58c3ffff 88030000 d8c3ffff h...X...........
-  0x00007200 a8030000 5ac4ffff c8030000 dcc4ffff ....Z...........
-  0x00007210 e8030000 5ac5ffff 08040000 dfc5ffff ....Z...........
-  0x00007220 28040000 66c6ffff 48040000 edc6ffff (...f...H.......
-  0x00007230 68040000 70c7ffff 88040000 9cc7ffff h...p...........
-  0x00007240 a8040000 cac7ffff c8040000 f8c7ffff ................
-  0x00007250 e8040000 26c8ffff 08050000 6fc8ffff ....&.......o...
-  0x00007260 28050000 bcc8ffff 48050000 16c9ffff (.......H.......
-  0x00007270 68050000 70c9ffff 88050000 92c9ffff h...p...........
-  0x00007280 a8050000 b8c9ffff c8050000 0ecaffff ................
-  0x00007290 e8050000 66caffff 08060000 e3caffff ....f...........
-  0x000072a0 28060000 caccffff 48060000 0ccdffff (.......H.......
-  0x000072b0 68060000 57cdffff 88060000 c2cdffff h...W...........
-  0x000072c0 a8060000 0dceffff c8060000 79ceffff ............y...
-  0x000072d0 e8060000 feceffff 08070000 5ccfffff ............\...
-  0x000072e0 28070000 2dd0ffff 48070000 45d1ffff (...-...H...E...
-  0x000072f0 68070000 fad1ffff 88070000 29d2ffff h...........)...
-  0x00007300 a8070000 82d4ffff cc070000 a6d8ffff ................
-  0x00007310 ec070000 45daffff 10080000 95dbffff ....E...........
-  0x00007320 30080000 12e0ffff 54080000 b0e3ffff 0.......T.......
-  0x00007330 74080000 08e4ffff 94080000 64e4ffff t...........d...
-  0x00007340 b4080000 14e5ffff d4080000 a0e5ffff ................
-  0x00007350 f4080000 66e7ffff 18090000 1ee8ffff ....f...........
-  0x00007360 38090000 8fe8ffff 58090000 8dedffff 8.......X.......
-  0x00007370 78090000 b0edffff 98090000 06eeffff x...............
-  0x00007380 b8090000 93efffff d8090000 93f1ffff ................
-  0x00007390 f8090000 f9f1ffff 180a0000 daf4ffff ................
-  0x000073a0 3c0a0000                            <...
+  0x00005e20 011b033b 0c020000 40000000 a0b9ffff ...;....@.......
+  0x00005e30 28020000 70bcffff 50020000 5abdffff (...p...P...Z...
+  0x00005e40 68020000 e5beffff 88020000 9ec0ffff h...............
+  0x00005e50 a8020000 74c2ffff c8020000 4fc4ffff ....t.......O...
+  0x00005e60 e8020000 f2c5ffff 08030000 c4c7ffff ................
+  0x00005e70 28030000 b4c9ffff 48030000 a9cbffff (.......H.......
+  0x00005e80 68030000 2dccffff 88030000 b3ccffff h...-...........
+  0x00005e90 a8030000 39cdffff c8030000 bbcdffff ....9...........
+  0x00005ea0 e8030000 52ceffff 08040000 ebceffff ....R...........
+  0x00005eb0 28040000 84cfffff 48040000 19d0ffff (.......H.......
+  0x00005ec0 68040000 41d0ffff 88040000 6bd0ffff h...A.......k...
+  0x00005ed0 a8040000 95d0ffff c8040000 c3d0ffff ................
+  0x00005ee0 e8040000 08d1ffff 08050000 51d1ffff ............Q...
+  0x00005ef0 28050000 a7d1ffff 48050000 fdd1ffff (.......H.......
+  0x00005f00 68050000 1bd2ffff 88050000 3dd2ffff h...........=...
+  0x00005f10 a8050000 8fd2ffff c8050000 e3d2ffff ................
+  0x00005f20 e8050000 5cd3ffff 08060000 3fd5ffff ....\.......?...
+  0x00005f30 28060000 83d5ffff 48060000 cad5ffff (.......H.......
+  0x00005f40 68060000 31d6ffff 88060000 78d6ffff h...1.......x...
+  0x00005f50 a8060000 e0d6ffff c8060000 69d7ffff ............i...
+  0x00005f60 e8060000 d6d7ffff 08070000 dbd8ffff ................
+  0x00005f70 28070000 27daffff 48070000 d8daffff (...'...H.......
+  0x00005f80 68070000 03dbffff 88070000 5dddffff h...........]...
+  0x00005f90 ac070000 5de1ffff cc070000 10e3ffff ....]...........
+  0x00005fa0 ec070000 5ce4ffff 10080000 dde8ffff ....\...........
+  0x00005fb0 34080000 7eecffff 54080000 d2ecffff 4...~...T.......
+  0x00005fc0 74080000 2aedffff 94080000 d5edffff t...*...........
+  0x00005fd0 b4080000 5ceeffff d4080000 28f0ffff ....\.......(...
+  0x00005fe0 f8080000 e2f0ffff 18090000 4ff1ffff ............O...
+  0x00005ff0 38090000 3ef6ffff 58090000 5df6ffff 8...>...X...]...
+  0x00006000 78090000 aff6ffff 98090000 38f8ffff x...........8...
+  0x00006010 b8090000 34faffff d8090000 96faffff ....4...........
+  0x00006020 f8090000 77fdffff 1c0a0000          ....w.......
```

#### readelf --wide --decompress --hex-dump=.eh_frame {}

```diff
@@ -1,136 +1,134 @@
 
 Hex dump of section '.eh_frame':
-  0x000073a8 14000000 00000000 017a5200 01781001 .........zR..x..
-  0x000073b8 1b0c0708 90010000 24000000 1c000000 ........$.......
-  0x000073c8 58acffff d0020000 000e1046 0e184a0f X..........F..J.
-  0x000073d8 0b770880 003f1a3a 2a332422 00000000 .w...?.:*3$"....
-  0x000073e8 14000000 44000000 00afffff 10000000 ....D...........
-  0x000073f8 00000000 00000000 14000000 5c000000 ............\...
-  0x00007408 f8aeffff c0020000 00000000 00000000 ................
-  0x00007418 1c000000 74000000 59b2ffff 8f010000 ....t...Y.......
-  0x00007428 00450e10 8602430d 06038601 0c070800 .E....C.........
-  0x00007438 1c000000 94000000 c8b3ffff bd010000 ................
-  0x00007448 00450e10 8602430d 0603b401 0c070800 .E....C.........
-  0x00007458 1c000000 b4000000 65b5ffff da010000 ........e.......
-  0x00007468 00450e10 8602430d 0603d101 0c070800 .E....C.........
-  0x00007478 1c000000 d4000000 1fb7ffff df010000 ................
-  0x00007488 00450e10 8602430d 0603d601 0c070800 .E....C.........
-  0x00007498 1c000000 f4000000 deb8ffff a7010000 ................
-  0x000074a8 00450e10 8602430d 06039e01 0c070800 .E....C.........
-  0x000074b8 1c000000 14010000 65baffff d6010000 ........e.......
-  0x000074c8 00450e10 8602430d 0603cd01 0c070800 .E....C.........
-  0x000074d8 1c000000 34010000 1bbcffff f4010000 ....4...........
-  0x000074e8 00450e10 8602430d 0603eb01 0c070800 .E....C.........
-  0x000074f8 1c000000 54010000 efbdffff f9010000 ....T...........
-  0x00007508 00450e10 8602430d 0603f001 0c070800 .E....C.........
-  0x00007518 1c000000 74010000 c8bfffff 80000000 ....t...........
-  0x00007528 00450e10 8602430d 0602770c 07080000 .E....C...w.....
-  0x00007538 1c000000 94010000 28c0ffff 82000000 ........(.......
-  0x00007548 00450e10 8602430d 0602790c 07080000 .E....C...y.....
-  0x00007558 1c000000 b4010000 8ac0ffff 82000000 ................
-  0x00007568 00450e10 8602430d 0602790c 07080000 .E....C...y.....
-  0x00007578 1c000000 d4010000 ecc0ffff 7e000000 ............~...
-  0x00007588 00450e10 8602430d 0602750c 07080000 .E....C...u.....
-  0x00007598 1c000000 f4010000 4ac1ffff 85000000 ........J.......
-  0x000075a8 00450e10 8602430d 06027c0c 07080000 .E....C...|.....
-  0x000075b8 1c000000 14020000 afc1ffff 87000000 ................
-  0x000075c8 00450e10 8602430d 06027e0c 07080000 .E....C...~.....
-  0x000075d8 1c000000 34020000 16c2ffff 87000000 ....4...........
-  0x000075e8 00450e10 8602430d 06027e0c 07080000 .E....C...~.....
-  0x000075f8 1c000000 54020000 7dc2ffff 83000000 ....T...}.......
-  0x00007608 00450e10 8602430d 06027a0c 07080000 .E....C...z.....
-  0x00007618 1c000000 74020000 e0c2ffff 2c000000 ....t.......,...
-  0x00007628 00450e10 8602430d 06630c07 08000000 .E....C..c......
-  0x00007638 1c000000 94020000 ecc2ffff 2e000000 ................
-  0x00007648 00450e10 8602430d 06650c07 08000000 .E....C..e......
-  0x00007658 1c000000 b4020000 fac2ffff 2e000000 ................
-  0x00007668 00450e10 8602430d 06650c07 08000000 .E....C..e......
-  0x00007678 1c000000 d4020000 08c3ffff 2e000000 ................
-  0x00007688 00450e10 8602430d 06650c07 08000000 .E....C..e......
-  0x00007698 1c000000 f4020000 16c3ffff 49000000 ............I...
-  0x000076a8 00450e10 8602430d 0602400c 07080000 .E....C...@.....
-  0x000076b8 1c000000 14030000 3fc3ffff 4d000000 ........?...M...
-  0x000076c8 00450e10 8602430d 0602440c 07080000 .E....C...D.....
-  0x000076d8 1c000000 34030000 6cc3ffff 5a000000 ....4...l...Z...
-  0x000076e8 00450e10 8602430d 0602510c 07080000 .E....C...Q.....
-  0x000076f8 1c000000 54030000 a6c3ffff 5a000000 ....T.......Z...
-  0x00007708 00450e10 8602430d 0602510c 07080000 .E....C...Q.....
-  0x00007718 1c000000 74030000 e0c3ffff 22000000 ....t......."...
-  0x00007728 00450e10 8602430d 06590c07 08000000 .E....C..Y......
-  0x00007738 1c000000 94030000 e2c3ffff 26000000 ............&...
-  0x00007748 00450e10 8602430d 065d0c07 08000000 .E....C..]......
-  0x00007758 1c000000 b4030000 e8c3ffff 56000000 ............V...
-  0x00007768 00450e10 8602430d 06024d0c 07080000 .E....C...M.....
-  0x00007778 1c000000 d4030000 1ec4ffff 58000000 ............X...
-  0x00007788 00450e10 8602430d 06024f0c 07080000 .E....C...O.....
-  0x00007798 1c000000 f4030000 56c4ffff 7d000000 ........V...}...
-  0x000077a8 00450e10 8602430d 0602740c 07080000 .E....C...t.....
-  0x000077b8 1c000000 14040000 b3c4ffff e7010000 ................
-  0x000077c8 00450e10 8602430d 0603de01 0c070800 .E....C.........
-  0x000077d8 1c000000 34040000 7ac6ffff 42000000 ....4...z...B...
-  0x000077e8 00450e10 8602430d 06790c07 08000000 .E....C..y......
-  0x000077f8 1c000000 54040000 9cc6ffff 4b000000 ....T.......K...
-  0x00007808 00450e10 8602430d 0602420c 07080000 .E....C...B.....
-  0x00007818 1c000000 74040000 c7c6ffff 6b000000 ....t.......k...
-  0x00007828 00450e10 8602430d 0602620c 07080000 .E....C...b.....
-  0x00007838 1c000000 94040000 12c7ffff 4b000000 ............K...
-  0x00007848 00450e10 8602430d 0602420c 07080000 .E....C...B.....
-  0x00007858 1c000000 b4040000 3dc7ffff 6c000000 ........=...l...
-  0x00007868 00450e10 8602430d 0602630c 07080000 .E....C...c.....
-  0x00007878 1c000000 d4040000 89c7ffff 85000000 ................
-  0x00007888 00450e10 8602430d 06027c0c 07080000 .E....C...|.....
-  0x00007898 1c000000 f4040000 eec7ffff 5e000000 ............^...
-  0x000078a8 00450e10 8602430d 0602550c 07080000 .E....C...U.....
-  0x000078b8 1c000000 14050000 2cc8ffff d1000000 ........,.......
-  0x000078c8 00450e10 8602430d 0602c80c 07080000 .E....C.........
-  0x000078d8 1c000000 34050000 ddc8ffff 18010000 ....4...........
-  0x000078e8 00450e10 8602430d 06030f01 0c070800 .E....C.........
-  0x000078f8 1c000000 54050000 d5c9ffff b5000000 ....T...........
-  0x00007908 00450e10 8602430d 0602ac0c 07080000 .E....C.........
-  0x00007918 1c000000 74050000 6acaffff 2f000000 ....t...j.../...
-  0x00007928 00450e10 8602430d 06660c07 08000000 .E....C..f......
-  0x00007938 20000000 94050000 79caffff 59020000  .......y...Y...
-  0x00007948 00450e10 8602430d 06458303 034b020c .E....C..E...K..
-  0x00007958 07080000 1c000000 b8050000 aeccffff ................
-  0x00007968 24040000 00450e10 8602430d 06031b04 $....E....C.....
-  0x00007978 0c070800 20000000 d8050000 b2d0ffff .... ...........
-  0x00007988 9f010000 00450e10 8602430d 06458303 .....E....C..E..
-  0x00007998 0391010c 07080000 1c000000 fc050000 ................
-  0x000079a8 2dd2ffff 50010000 00450e10 8602430d -...P....E....C.
-  0x000079b8 06034701 0c070800 20000000 1c060000 ..G..... .......
-  0x000079c8 5dd3ffff 7d040000 00450e10 8602430d ]...}....E....C.
-  0x000079d8 06488303 036c040c 07080000 1c000000 .H...l..........
-  0x000079e8 40060000 b6d7ffff 9e030000 00450e10 @............E..
-  0x000079f8 8602430d 06039503 0c070800 1c000000 ..C.............
-  0x00007a08 60060000 34dbffff 58000000 00450e10 `...4...X....E..
-  0x00007a18 8602430d 06024f0c 07080000 1c000000 ..C...O.........
-  0x00007a28 80060000 6cdbffff 5c000000 00450e10 ....l...\....E..
-  0x00007a38 8602430d 0602530c 07080000 1c000000 ..C...S.........
-  0x00007a48 a0060000 a8dbffff b0000000 00450e10 .............E..
-  0x00007a58 8602430d 0602a70c 07080000 1c000000 ..C.............
-  0x00007a68 c0060000 38dcffff 8c000000 00450e10 ....8........E..
-  0x00007a78 8602430d 0602830c 07080000 20000000 ..C......... ...
-  0x00007a88 e0060000 a4dcffff c6010000 00450e10 .............E..
-  0x00007a98 8602430d 0603bd01 0c070800 00000000 ..C.............
-  0x00007aa8 1c000000 04070000 46deffff b8000000 ........F.......
-  0x00007ab8 00450e10 8602430d 0602af0c 07080000 .E....C.........
-  0x00007ac8 1c000000 24070000 dedeffff 71000000 ....$.......q...
-  0x00007ad8 00450e10 8602430d 0602680c 07080000 .E....C...h.....
-  0x00007ae8 1c000000 44070000 2fdfffff fe040000 ....D.../.......
-  0x00007af8 00450e10 8602430d 0603f504 0c070800 .E....C.........
-  0x00007b08 1c000000 64070000 0de4ffff 23000000 ....d.......#...
-  0x00007b18 00450e10 8602430d 065a0c07 08000000 .E....C..Z......
-  0x00007b28 1c000000 84070000 10e4ffff 56000000 ............V...
-  0x00007b38 00450e10 8602430d 06024d0c 07080000 .E....C...M.....
-  0x00007b48 1c000000 a4070000 46e4ffff 8d010000 ........F.......
-  0x00007b58 00450e10 8602430d 06038401 0c070800 .E....C.........
-  0x00007b68 1c000000 c4070000 b3e5ffff 00020000 ................
-  0x00007b78 00450e10 8602430d 0603f701 0c070800 .E....C.........
-  0x00007b88 1c000000 e4070000 93e7ffff 66000000 ............f...
-  0x00007b98 00450e10 8602430d 06025d0c 07080000 .E....C...].....
-  0x00007ba8 20000000 04080000 d9e7ffff e1020000  ...............
-  0x00007bb8 00450e10 8602430d 06488303 03d0020c .E....C..H......
-  0x00007bc8 07080000 1c000000 28080000 96eaffff ........(.......
-  0x00007bd8 da000000 00450e10 8602430d 0602d10c .....E....C.....
-  0x00007be8 07080000 00000000                   ........
+  0x00006030 14000000 00000000 017a5200 01781001 .........zR..x..
+  0x00006040 1b0c0708 90010000 24000000 1c000000 ........$.......
+  0x00006050 70b7ffff d0020000 000e1046 0e184a0f p..........F..J.
+  0x00006060 0b770880 003f1a3b 2a332422 00000000 .w...?.;*3$"....
+  0x00006070 14000000 44000000 18baffff 08000000 ....D...........
+  0x00006080 00000000 00000000 1c000000 5c000000 ............\...
+  0x00006090 eabaffff 8b010000 00410e10 8602430d .........A....C.
+  0x000060a0 06038601 0c070800 1c000000 7c000000 ............|...
+  0x000060b0 55bcffff b9010000 00410e10 8602430d U........A....C.
+  0x000060c0 0603b401 0c070800 1c000000 9c000000 ................
+  0x000060d0 eebdffff d6010000 00410e10 8602430d .........A....C.
+  0x000060e0 0603d101 0c070800 1c000000 bc000000 ................
+  0x000060f0 a4bfffff db010000 00410e10 8602430d .........A....C.
+  0x00006100 0603d601 0c070800 1c000000 dc000000 ................
+  0x00006110 5fc1ffff a3010000 00410e10 8602430d _........A....C.
+  0x00006120 06039e01 0c070800 1c000000 fc000000 ................
+  0x00006130 e2c2ffff d2010000 00410e10 8602430d .........A....C.
+  0x00006140 0603cd01 0c070800 1c000000 1c010000 ................
+  0x00006150 94c4ffff f0010000 00410e10 8602430d .........A....C.
+  0x00006160 0603eb01 0c070800 1c000000 3c010000 ............<...
+  0x00006170 64c6ffff f5010000 00410e10 8602430d d........A....C.
+  0x00006180 0603f001 0c070800 1c000000 5c010000 ............\...
+  0x00006190 39c8ffff 84000000 00410e10 8602430d 9........A....C.
+  0x000061a0 06027f0c 07080000 1c000000 7c010000 ............|...
+  0x000061b0 9dc8ffff 86000000 00410e10 8602430d .........A....C.
+  0x000061c0 0602810c 07080000 1c000000 9c010000 ................
+  0x000061d0 03c9ffff 86000000 00410e10 8602430d .........A....C.
+  0x000061e0 0602810c 07080000 1c000000 bc010000 ................
+  0x000061f0 69c9ffff 82000000 00410e10 8602430d i........A....C.
+  0x00006200 06027d0c 07080000 1c000000 dc010000 ..}.............
+  0x00006210 cbc9ffff 97000000 00410e10 8602430d .........A....C.
+  0x00006220 0602920c 07080000 1c000000 fc010000 ................
+  0x00006230 42caffff 99000000 00410e10 8602430d B........A....C.
+  0x00006240 0602940c 07080000 1c000000 1c020000 ................
+  0x00006250 bbcaffff 99000000 00410e10 8602430d .........A....C.
+  0x00006260 0602940c 07080000 1c000000 3c020000 ............<...
+  0x00006270 34cbffff 95000000 00410e10 8602430d 4........A....C.
+  0x00006280 0602900c 07080000 1c000000 5c020000 ............\...
+  0x00006290 a9cbffff 28000000 00410e10 8602430d ....(....A....C.
+  0x000062a0 06630c07 08000000 1c000000 7c020000 .c..........|...
+  0x000062b0 b1cbffff 2a000000 00410e10 8602430d ....*....A....C.
+  0x000062c0 06650c07 08000000 1c000000 9c020000 .e..............
+  0x000062d0 bbcbffff 2a000000 00410e10 8602430d ....*....A....C.
+  0x000062e0 06650c07 08000000 1c000000 bc020000 .e..............
+  0x000062f0 c5cbffff 2e000000 00410e10 8602430d .........A....C.
+  0x00006300 06690c07 08000000 1c000000 dc020000 .i..............
+  0x00006310 d3cbffff 45000000 00410e10 8602430d ....E....A....C.
+  0x00006320 0602400c 07080000 1c000000 fc020000 ..@.............
+  0x00006330 f8cbffff 49000000 00410e10 8602430d ....I....A....C.
+  0x00006340 0602440c 07080000 1c000000 1c030000 ..D.............
+  0x00006350 21ccffff 56000000 00410e10 8602430d !...V....A....C.
+  0x00006360 0602510c 07080000 1c000000 3c030000 ..Q.........<...
+  0x00006370 57ccffff 56000000 00410e10 8602430d W...V....A....C.
+  0x00006380 0602510c 07080000 1c000000 5c030000 ..Q.........\...
+  0x00006390 8dccffff 1e000000 00410e10 8602430d .........A....C.
+  0x000063a0 06590c07 08000000 1c000000 7c030000 .Y..........|...
+  0x000063b0 8bccffff 22000000 00410e10 8602430d ...."....A....C.
+  0x000063c0 065d0c07 08000000 1c000000 9c030000 .]..............
+  0x000063d0 8dccffff 52000000 00410e10 8602430d ....R....A....C.
+  0x000063e0 06024d0c 07080000 1c000000 bc030000 ..M.............
+  0x000063f0 bfccffff 54000000 00410e10 8602430d ....T....A....C.
+  0x00006400 06024f0c 07080000 1c000000 dc030000 ..O.............
+  0x00006410 f3ccffff 79000000 00410e10 8602430d ....y....A....C.
+  0x00006420 0602740c 07080000 1c000000 fc030000 ..t.............
+  0x00006430 4ccdffff e3010000 00410e10 8602430d L........A....C.
+  0x00006440 0603de01 0c070800 1c000000 1c040000 ................
+  0x00006450 0fcfffff 44000000 00410e10 8602430d ....D....A....C.
+  0x00006460 067f0c07 08000000 1c000000 3c040000 ............<...
+  0x00006470 33cfffff 47000000 00410e10 8602430d 3...G....A....C.
+  0x00006480 0602420c 07080000 1c000000 5c040000 ..B.........\...
+  0x00006490 5acfffff 67000000 00410e10 8602430d Z...g....A....C.
+  0x000064a0 0602620c 07080000 1c000000 7c040000 ..b.........|...
+  0x000064b0 a1cfffff 47000000 00410e10 8602430d ....G....A....C.
+  0x000064c0 0602420c 07080000 1c000000 9c040000 ..B.............
+  0x000064d0 c8cfffff 68000000 00410e10 8602430d ....h....A....C.
+  0x000064e0 0602630c 07080000 1c000000 bc040000 ..c.............
+  0x000064f0 10d0ffff 89000000 00410e10 8602430d .........A....C.
+  0x00006500 0602840c 07080000 1c000000 dc040000 ................
+  0x00006510 79d0ffff 6d000000 00410e10 8602430d y...m....A....C.
+  0x00006520 0602680c 07080000 1c000000 fc040000 ..h.............
+  0x00006530 c6d0ffff 05010000 00410e10 8602430d .........A....C.
+  0x00006540 06030001 0c070800 1c000000 1c050000 ................
+  0x00006550 abd1ffff 4c010000 00410e10 8602430d ....L....A....C.
+  0x00006560 06034701 0c070800 1c000000 3c050000 ..G.........<...
+  0x00006570 d7d2ffff b1000000 00410e10 8602430d .........A....C.
+  0x00006580 0602ac0c 07080000 1c000000 5c050000 ............\...
+  0x00006590 68d3ffff 2b000000 00410e10 8602430d h...+....A....C.
+  0x000065a0 06660c07 08000000 20000000 7c050000 .f...... ...|...
+  0x000065b0 73d3ffff 5a020000 00410e10 8602430d s...Z....A....C.
+  0x000065c0 06458303 0350020c 07080000 1c000000 .E...P..........
+  0x000065d0 a0050000 a9d5ffff 00040000 00410e10 .............A..
+  0x000065e0 8602430d 0603fb03 0c070800 1c000000 ..C.............
+  0x000065f0 c0050000 89d9ffff b3010000 00410e10 .............A..
+  0x00006600 8602430d 0603ae01 0c070800 20000000 ..C......... ...
+  0x00006610 e0050000 1cdbffff 4c010000 00410e10 ........L....A..
+  0x00006620 8602430d 06034701 0c070800 00000000 ..C...G.........
+  0x00006630 20000000 04060000 44dcffff 81040000  .......D.......
+  0x00006640 00410e10 8602430d 06488303 0374040c .A....C..H...t..
+  0x00006650 07080000 1c000000 28060000 a1e0ffff ........(.......
+  0x00006660 a1030000 00410e10 8602430d 06039c03 .....A....C.....
+  0x00006670 0c070800 1c000000 48060000 22e4ffff ........H..."...
+  0x00006680 54000000 00410e10 8602430d 06024f0c T....A....C...O.
+  0x00006690 07080000 1c000000 68060000 56e4ffff ........h...V...
+  0x000066a0 58000000 00410e10 8602430d 0602530c X....A....C...S.
+  0x000066b0 07080000 1c000000 88060000 8ee4ffff ................
+  0x000066c0 ab000000 00410e10 8602430d 0602a60c .....A....C.....
+  0x000066d0 07080000 1c000000 a8060000 19e5ffff ................
+  0x000066e0 87000000 00410e10 8602430d 0602820c .....A....C.....
+  0x000066f0 07080000 20000000 c8060000 80e5ffff .... ...........
+  0x00006700 cc010000 00410e10 8602430d 0603c701 .....A....C.....
+  0x00006710 0c070800 00000000 1c000000 ec060000 ................
+  0x00006720 28e7ffff ba000000 00410e10 8602430d (........A....C.
+  0x00006730 0602b50c 07080000 1c000000 0c070000 ................
+  0x00006740 c2e7ffff 6d000000 00410e10 8602430d ....m....A....C.
+  0x00006750 0602680c 07080000 1c000000 2c070000 ..h.........,...
+  0x00006760 0fe8ffff ef040000 00410e10 8602430d .........A....C.
+  0x00006770 0603ea04 0c070800 1c000000 4c070000 ............L...
+  0x00006780 deecffff 1f000000 00410e10 8602430d .........A....C.
+  0x00006790 065a0c07 08000000 1c000000 6c070000 .Z..........l...
+  0x000067a0 ddecffff 52000000 00410e10 8602430d ....R....A....C.
+  0x000067b0 06024d0c 07080000 1c000000 8c070000 ..M.............
+  0x000067c0 0fedffff 89010000 00410e10 8602430d .........A....C.
+  0x000067d0 06038401 0c070800 1c000000 ac070000 ................
+  0x000067e0 78eeffff fc010000 00410e10 8602430d x........A....C.
+  0x000067f0 0603f701 0c070800 1c000000 cc070000 ................
+  0x00006800 54f0ffff 62000000 00410e10 8602430d T...b....A....C.
+  0x00006810 06025d0c 07080000 20000000 ec070000 ..]..... .......
+  0x00006820 96f0ffff e1020000 00410e10 8602430d .........A....C.
+  0x00006830 06488303 03d4020c 07080000 1c000000 .H..............
+  0x00006840 10080000 53f3ffff e2000000 00410e10 ....S........A..
+  0x00006850 8602430d 0602dd0c 07080000 00000000 ..C.............
```

#### readelf --wide --decompress --hex-dump=.init_array {}

```diff
@@ -1,4 +1,4 @@
 
 Hex dump of section '.init_array':
-  0x00008e00 70260000 00000000                   p&......
+  0x00206e00 701b0000 00000000                   p.......
```

#### readelf --wide --decompress --hex-dump=.fini_array {}

```diff
@@ -1,4 +1,4 @@
 
 Hex dump of section '.fini_array':
-  0x00008e08 30260000 00000000                   0&......
+  0x00206e08 301b0000 00000000                   0.......
```

#### readelf --wide --decompress --hex-dump=.got {}

```diff
@@ -1,5 +1,5 @@
 
 Hex dump of section '.got':
-  0x00008fe0 00000000 00000000 00000000 00000000 ................
-  0x00008ff0 00000000 00000000 00000000 00000000 ................
+  0x00206fe0 00000000 00000000 00000000 00000000 ................
+  0x00206ff0 00000000 00000000 00000000 00000000 ................
```

#### readelf --wide --decompress --hex-dump=.got.plt {}

```diff
@@ -1,28 +1,28 @@
 
 Hex dump of section '.got.plt':
  NOTE: This section has relocations against it, but these have NOT been applied to this dump.
-  0x00009000 108e0000 00000000 00000000 00000000 ................
-  0x00009010 00000000 00000000 30200000 00000000 ........0 ......
-  0x00009020 40200000 00000000 50200000 00000000 @ ......P ......
-  0x00009030 60200000 00000000 70200000 00000000 ` ......p ......
-  0x00009040 80200000 00000000 90200000 00000000 . ....... ......
-  0x00009050 a0200000 00000000 b0200000 00000000 . ....... ......
-  0x00009060 c0200000 00000000 d0200000 00000000 . ....... ......
-  0x00009070 e0200000 00000000 f0200000 00000000 . ....... ......
-  0x00009080 00210000 00000000 10210000 00000000 .!.......!......
-  0x00009090 20210000 00000000 30210000 00000000  !......0!......
-  0x000090a0 40210000 00000000 50210000 00000000 @!......P!......
-  0x000090b0 60210000 00000000 70210000 00000000 `!......p!......
-  0x000090c0 80210000 00000000 90210000 00000000 .!.......!......
-  0x000090d0 a0210000 00000000 b0210000 00000000 .!.......!......
-  0x000090e0 c0210000 00000000 d0210000 00000000 .!.......!......
-  0x000090f0 e0210000 00000000 f0210000 00000000 .!.......!......
-  0x00009100 00220000 00000000 10220000 00000000 ."......."......
-  0x00009110 20220000 00000000 30220000 00000000  "......0"......
-  0x00009120 40220000 00000000 50220000 00000000 @"......P"......
-  0x00009130 60220000 00000000 70220000 00000000 `"......p"......
-  0x00009140 80220000 00000000 90220000 00000000 ."......."......
-  0x00009150 a0220000 00000000 b0220000 00000000 ."......."......
-  0x00009160 c0220000 00000000 d0220000 00000000 ."......."......
-  0x00009170 e0220000 00000000                   ."......
+  0x00207000 106e2000 00000000 00000000 00000000 .n .............
+  0x00207010 00000000 00000000 d6170000 00000000 ................
+  0x00207020 e6170000 00000000 f6170000 00000000 ................
+  0x00207030 06180000 00000000 16180000 00000000 ................
+  0x00207040 26180000 00000000 36180000 00000000 &.......6.......
+  0x00207050 46180000 00000000 56180000 00000000 F.......V.......
+  0x00207060 66180000 00000000 76180000 00000000 f.......v.......
+  0x00207070 86180000 00000000 96180000 00000000 ................
+  0x00207080 a6180000 00000000 b6180000 00000000 ................
+  0x00207090 c6180000 00000000 d6180000 00000000 ................
+  0x002070a0 e6180000 00000000 f6180000 00000000 ................
+  0x002070b0 06190000 00000000 16190000 00000000 ................
+  0x002070c0 26190000 00000000 36190000 00000000 &.......6.......
+  0x002070d0 46190000 00000000 56190000 00000000 F.......V.......
+  0x002070e0 66190000 00000000 76190000 00000000 f.......v.......
+  0x002070f0 86190000 00000000 96190000 00000000 ................
+  0x00207100 a6190000 00000000 b6190000 00000000 ................
+  0x00207110 c6190000 00000000 d6190000 00000000 ................
+  0x00207120 e6190000 00000000 f6190000 00000000 ................
+  0x00207130 061a0000 00000000 161a0000 00000000 ................
+  0x00207140 261a0000 00000000 361a0000 00000000 &.......6.......
+  0x00207150 461a0000 00000000 561a0000 00000000 F.......V.......
+  0x00207160 661a0000 00000000 761a0000 00000000 f.......v.......
+  0x00207170 861a0000 00000000                   ........
```

#### readelf --wide --decompress --hex-dump=.data {}

```diff
@@ -1,4 +1,4 @@
 
 Hex dump of section '.data':
-  0x00009178 78910000 00000000                   x.......
+  0x00207178 78712000 00000000                   xq .....
```

#### readelf --wide --decompress --string-dump=.comment {}

```diff
@@ -1,4 +1,4 @@
 
 String dump of section '.comment':
-  [     0]  GCC: (Ubuntu 9.4.0-1ubuntu1~20.04.1) 9.4.0
+  [     0]  GCC: (Ubuntu 7.5.0-3ubuntu1~18.04) 7.5.0
```

#### readelf --wide --decompress --hex-dump=.strtab {}

```diff
@@ -1,125 +1,125 @@
 
 Hex dump of section '.strtab':
   0x00000000 00637274 73747566 662e6300 64657265 .crtstuff.c.dere
   0x00000010 67697374 65725f74 6d5f636c 6f6e6573 gister_tm_clones
   0x00000020 005f5f64 6f5f676c 6f62616c 5f64746f .__do_global_dto
   0x00000030 72735f61 75780063 6f6d706c 65746564 rs_aux.completed
-  0x00000040 2e383036 31005f5f 646f5f67 6c6f6261 .8061.__do_globa
+  0x00000040 2e373639 38005f5f 646f5f67 6c6f6261 .7698.__do_globa
   0x00000050 6c5f6474 6f72735f 6175785f 66696e69 l_dtors_aux_fini
   0x00000060 5f617272 61795f65 6e747279 00667261 _array_entry.fra
   0x00000070 6d655f64 756d6d79 005f5f66 72616d65 me_dummy.__frame
   0x00000080 5f64756d 6d795f69 6e69745f 61727261 _dummy_init_arra
   0x00000090 795f656e 74727900 635f6172 7261792e y_entry.c_array.
   0x000000a0 6300635f 61727261 795f6d74 2e630063 c.c_array_mt.c.c
   0x000000b0 6f765f6d 6f64656c 2e63006b 72696765 ov_model.c.krige
-  0x000000c0 2e630073 696c6c00 65737469 6d617469 .c.sill.estimati
-  0x000000d0 6f6e006b 72696765 5f766172 00666978 on.krige_var.fix
-  0x000000e0 006c6f63 6174696f 6e006c6f 635f636f .location.loc_co
-  0x000000f0 76006461 74615f74 656d7000 6c6f635f v.data_temp.loc_
-  0x00000100 636f7632 00666c61 7474656e 5f74656d cov2.flatten_tem
-  0x00000110 70007765 69676874 73006172 72617932 p.weights.array2
-  0x00000120 645f7465 6d700070 64697374 5f74656d d_temp.pdist_tem
-  0x00000130 70006461 7461636f 76006d61 74726978 p.datacov.matrix
-  0x00000140 5f746f6f 6c732e63 0072616e 646f6d5f _tools.c.random_
-  0x00000150 746f6f6c 732e6300 73677369 6d2e6300 tools.c.sgsim.c.
-  0x00000160 785f6772 69640075 5f617272 61790073 x_grid.u_array.s
-  0x00000170 616d706c 65640076 6172696f 6772616d ampled.variogram
-  0x00000180 5f617272 61790073 6773696d 5f617272 _array.sgsim_arr
-  0x00000190 6179005f 73616d70 6c696e67 00666c61 ay._sampling.fla
-  0x000001a0 6700636f 756e7400 73677369 6d5f6d65 g.count.sgsim_me
-  0x000001b0 6d6f7279 5f667265 6500736f 72745f74 mory_free.sort_t
-  0x000001c0 6f6f6c73 2e630071 7569636b 736f7274 ools.c.quicksort
-  0x000001d0 32642e6c 6f63616c 616c6961 73007661 2d.localalias.va
-  0x000001e0 72696f67 72616d2e 63005f5f 4652414d riogram.c.__FRAM
-  0x000001f0 455f454e 445f5f00 5f66696e 69005f5f E_END__._fini.__
-  0x00000200 64736f5f 68616e64 6c65005f 44594e41 dso_handle._DYNA
-  0x00000210 4d494300 5f5f474e 555f4548 5f465241 MIC.__GNU_EH_FRA
-  0x00000220 4d455f48 4452005f 5f544d43 5f454e44 ME_HDR.__TMC_END
-  0x00000230 5f5f005f 474c4f42 414c5f4f 46465345 __._GLOBAL_OFFSE
-  0x00000240 545f5441 424c455f 00667265 65404047 T_TABLE_.free@@G
-  0x00000250 4c494243 5f322e32 2e350063 5f617272 LIBC_2.2.5.c_arr
-  0x00000260 61795f6d 61785f66 6c6f6174 00635f61 ay_max_float.c_a
-  0x00000270 72726179 5f766172 5f696e74 005f5f65 rray_var_int.__e
-  0x00000280 72726e6f 5f6c6f63 6174696f 6e404047 rrno_location@@G
-  0x00000290 4c494243 5f322e32 2e350063 5f617272 LIBC_2.2.5.c_arr
-  0x000002a0 61795f73 756d5f66 6c6f6174 00636d70 ay_sum_float.cmp
-  0x000002b0 66756e63 5f696e74 00717569 636b736f func_int.quickso
-  0x000002c0 72743264 005f4954 4d5f6465 72656769 rt2d._ITM_deregi
-  0x000002d0 73746572 544d436c 6f6e6554 61626c65 sterTMCloneTable
-  0x000002e0 006d6b64 69724040 474c4942 435f322e .mkdir@@GLIBC_2.
-  0x000002f0 322e3500 635f6172 7261795f 73756d5f 2.5.c_array_sum_
-  0x00000300 696e7400 72616e64 6f6d7061 74680063 int.randompath.c
-  0x00000310 65696c00 6c755f69 6e766572 73655f73 eil.lu_inverse_s
-  0x00000320 6f6c7665 72007361 6d706c69 6e675f73 olver.sampling_s
-  0x00000330 74617465 5f757064 61746500 66636c6f tate_update.fclo
-  0x00000340 73654040 474c4942 435f322e 322e3500 se@@GLIBC_2.2.5.
-  0x00000350 73677369 6d5f7275 6e005f5f 73746163 sgsim_run.__stac
-  0x00000360 6b5f6368 6b5f6661 696c4040 474c4942 k_chk_fail@@GLIB
-  0x00000370 435f322e 34007361 76655f31 64617272 C_2.4.save_1darr
-  0x00000380 61790063 5f617272 61795f76 61725f64 ay.c_array_var_d
-  0x00000390 6f75626c 6500635f 61727261 795f6d65 ouble.c_array_me
-  0x000003a0 616e5f69 6e740063 5f617272 61795f6d an_int.c_array_m
-  0x000003b0 696e5f66 6c6f6174 00636f76 5f6d6f64 in_float.cov_mod
-  0x000003c0 656c3264 0066696e 645f6e65 69676862 el2d.find_neighb
-  0x000003d0 6f720073 6e707269 6e746640 40474c49 or.snprintf@@GLI
-  0x000003e0 42435f32 2e322e35 00636d70 66756e63 BC_2.2.5.cmpfunc
-  0x000003f0 5f646f75 626c6500 6c755f64 65636f6d _double.lu_decom
-  0x00000400 706f7369 74696f6e 00645f61 72616e67 position.d_arang
-  0x00000410 65005061 72746974 696f6e32 64006d74 e.Partition2d.mt
-  0x00000420 31393933 375f6765 745f666c 6f61745f 19937_get_float_
-  0x00000430 72616e67 6500636f 765f6d6f 64656c00 range.cov_model.
-  0x00000440 6d617472 6978666f 726d006d 74313939 matrixform.mt199
-  0x00000450 33375f67 656e6572 61746500 635f6172 37_generate.c_ar
-  0x00000460 7261795f 6d65616e 5f6c6f6e 675f6c6f ray_mean_long_lo
-  0x00000470 6e670076 61726961 6e636500 635f6172 ng.variance.c_ar
-  0x00000480 7261795f 7661725f 6c6f6e67 5f6c6f6e ray_var_long_lon
-  0x00000490 6700635f 61727261 795f7374 645f696e g.c_array_std_in
-  0x000004a0 74006d74 31393933 375f7261 6e646f6d t.mt19937_random
-  0x000004b0 5f6e6f72 6d616c00 63616c6c 6f634040 _normal.calloc@@
-  0x000004c0 474c4942 435f322e 322e3500 635f6172 GLIBC_2.2.5.c_ar
-  0x000004d0 7261795f 6d696e5f 646f7562 6c650063 ray_min_double.c
-  0x000004e0 6f765f6d 6f64656c 5f696e69 74006670 ov_model_init.fp
-  0x000004f0 72696e74 66404047 4c494243 5f322e32 rintf@@GLIBC_2.2
-  0x00000500 2e350073 6773696d 5f745f66 72656500 .5.sgsim_t_free.
-  0x00000510 5f5f676d 6f6e5f73 74617274 5f5f0063 __gmon_start__.c
-  0x00000520 5f617272 61795f6d 696e5f69 6e740063 _array_min_int.c
-  0x00000530 5f617272 61795f73 74645f64 6f75626c _array_std_doubl
-  0x00000540 6500635f 61727261 795f6d61 785f696e e.c_array_max_in
-  0x00000550 74006b72 6967655f 70617261 6d5f7365 t.krige_param_se
-  0x00000560 7474696e 6700635f 61727261 795f7375 tting.c_array_su
-  0x00000570 6d5f6c6f 6e67006d 74313939 33375f69 m_long.mt19937_i
-  0x00000580 6e697400 636d7066 756e635f 666c6f61 nit.cmpfunc_floa
-  0x00000590 74007369 6d706c65 5f6b7269 67696e67 t.simple_kriging
-  0x000005a0 00635f61 72726179 5f6d6561 6e5f666c .c_array_mean_fl
-  0x000005b0 6f617400 6d616c6c 6f634040 474c4942 oat.malloc@@GLIB
-  0x000005c0 435f322e 322e3500 6b726967 655f6d65 C_2.2.5.krige_me
-  0x000005d0 6d6f7279 5f667265 65006578 7000635f mory_free.exp.c_
-  0x000005e0 61727261 795f7661 725f666c 6f617400 array_var_float.
-  0x000005f0 76617269 6f677261 6d00635f 61727261 variogram.c_arra
-  0x00000600 795f6d61 785f646f 75626c65 00635f61 y_max_double.c_a
-  0x00000610 72726179 5f6d696e 5f6c6f6e 675f6c6f rray_min_long_lo
-  0x00000620 6e670063 6f73006d 74313939 33375f67 ng.cos.mt19937_g
-  0x00000630 65745f69 6e743332 5f72616e 67650073 et_int32_range.s
-  0x00000640 616d706c 696e675f 73746174 655f696e ampling_state_in
-  0x00000650 6974006d 74313939 33375f67 65745f64 it.mt19937_get_d
-  0x00000660 6f75626c 655f7261 6e676500 73677369 ouble_range.sgsi
-  0x00000670 6d5f696e 6974006c 6f670066 6f70656e m_init.log.fopen
-  0x00000680 4040474c 4942435f 322e322e 35006d74 @@GLIBC_2.2.5.mt
-  0x00000690 31393933 375f6765 745f646f 75626c65 19937_get_double
-  0x000006a0 00706f77 00706572 726f7240 40474c49 .pow.perror@@GLI
-  0x000006b0 42435f32 2e322e35 006d7431 39393337 BC_2.2.5.mt19937
-  0x000006c0 5f676574 5f666c6f 6174006c 6f673130 _get_float.log10
-  0x000006d0 00737172 7400636d 7066756e 635f6c6f .sqrt.cmpfunc_lo
-  0x000006e0 6e670070 64697374 00635f61 72726179 ng.pdist.c_array
-  0x000006f0 5f737464 5f6c6f6e 675f6c6f 6e670065 _std_long_long.e
-  0x00000700 78697440 40474c49 42435f32 2e322e35 xit@@GLIBC_2.2.5
-  0x00000710 005f4954 4d5f7265 67697374 6572544d ._ITM_registerTM
-  0x00000720 436c6f6e 65546162 6c650073 77617000 CloneTable.swap.
-  0x00000730 635f6172 7261795f 6d65616e 5f646f75 c_array_mean_dou
-  0x00000740 626c6500 635f6172 7261795f 7374645f ble.c_array_std_
-  0x00000750 666c6f61 7400635f 61727261 795f6d61 float.c_array_ma
-  0x00000760 785f6c6f 6e675f6c 6f6e6700 635f6172 x_long_long.c_ar
-  0x00000770 7261795f 73756d5f 646f7562 6c65005f ray_sum_double._
-  0x00000780 5f637861 5f66696e 616c697a 65404047 _cxa_finalize@@G
-  0x00000790 4c494243 5f322e32 2e3500            LIBC_2.2.5.
+  0x000000c0 2e63006b 5f72616e 67650065 7374696d .c.k_range.estim
+  0x000000d0 6174696f 6e006b72 6967655f 76617200 ation.krige_var.
+  0x000000e0 66697800 6c6f6361 74696f6e 006c6f63 fix.location.loc
+  0x000000f0 5f636f76 00646174 615f7465 6d70006c _cov.data_temp.l
+  0x00000100 6f635f63 6f763200 666c6174 74656e5f oc_cov2.flatten_
+  0x00000110 74656d70 00776569 67687473 00617272 temp.weights.arr
+  0x00000120 61793264 5f74656d 70007064 6973745f ay2d_temp.pdist_
+  0x00000130 74656d70 00646174 61636f76 006d6174 temp.datacov.mat
+  0x00000140 7269785f 746f6f6c 732e6300 72616e64 rix_tools.c.rand
+  0x00000150 6f6d5f74 6f6f6c73 2e630073 6773696d om_tools.c.sgsim
+  0x00000160 2e630078 5f677269 6400755f 61727261 .c.x_grid.u_arra
+  0x00000170 79007361 6d706c65 64007661 72696f67 y.sampled.variog
+  0x00000180 72616d5f 61727261 79007367 73696d5f ram_array.sgsim_
+  0x00000190 61727261 79005f73 616d706c 696e6700 array._sampling.
+  0x000001a0 666c6167 00636f75 6e740073 6773696d flag.count.sgsim
+  0x000001b0 5f6d656d 6f72795f 66726565 00736f72 _memory_free.sor
+  0x000001c0 745f746f 6f6c732e 63007661 72696f67 t_tools.c.variog
+  0x000001d0 72616d2e 63005f5f 4652414d 455f454e ram.c.__FRAME_EN
+  0x000001e0 445f5f00 5f5f6473 6f5f6861 6e646c65 D__.__dso_handle
+  0x000001f0 005f4459 4e414d49 43005f5f 474e555f ._DYNAMIC.__GNU_
+  0x00000200 45485f46 52414d45 5f484452 005f5f54 EH_FRAME_HDR.__T
+  0x00000210 4d435f45 4e445f5f 005f474c 4f42414c MC_END__._GLOBAL
+  0x00000220 5f4f4646 5345545f 5441424c 455f0066 _OFFSET_TABLE_.f
+  0x00000230 72656540 40474c49 42435f32 2e322e35 ree@@GLIBC_2.2.5
+  0x00000240 00635f61 72726179 5f6d6178 5f666c6f .c_array_max_flo
+  0x00000250 61740063 5f617272 61795f76 61725f69 at.c_array_var_i
+  0x00000260 6e74005f 5f657272 6e6f5f6c 6f636174 nt.__errno_locat
+  0x00000270 696f6e40 40474c49 42435f32 2e322e35 ion@@GLIBC_2.2.5
+  0x00000280 00635f61 72726179 5f73756d 5f666c6f .c_array_sum_flo
+  0x00000290 61740063 6d706675 6e635f69 6e740071 at.cmpfunc_int.q
+  0x000002a0 7569636b 736f7274 3264005f 49544d5f uicksort2d._ITM_
+  0x000002b0 64657265 67697374 6572544d 436c6f6e deregisterTMClon
+  0x000002c0 65546162 6c65006d 6b646972 4040474c eTable.mkdir@@GL
+  0x000002d0 4942435f 322e322e 3500635f 61727261 IBC_2.2.5.c_arra
+  0x000002e0 795f7375 6d5f696e 74007261 6e646f6d y_sum_int.random
+  0x000002f0 70617468 00636569 6c005f65 64617461 path.ceil._edata
+  0x00000300 006c755f 696e7665 7273655f 736f6c76 .lu_inverse_solv
+  0x00000310 65720073 616d706c 696e675f 73746174 er.sampling_stat
+  0x00000320 655f7570 64617465 0066636c 6f736540 e_update.fclose@
+  0x00000330 40474c49 42435f32 2e322e35 00736773 @GLIBC_2.2.5.sgs
+  0x00000340 696d5f72 756e005f 66696e69 005f5f73 im_run._fini.__s
+  0x00000350 7461636b 5f63686b 5f666169 6c404047 tack_chk_fail@@G
+  0x00000360 4c494243 5f322e34 00736176 655f3164 LIBC_2.4.save_1d
+  0x00000370 61727261 7900635f 61727261 795f7661 array.c_array_va
+  0x00000380 725f646f 75626c65 00635f61 72726179 r_double.c_array
+  0x00000390 5f6d6561 6e5f696e 7400635f 61727261 _mean_int.c_arra
+  0x000003a0 795f6d69 6e5f666c 6f617400 636f765f y_min_float.cov_
+  0x000003b0 6d6f6465 6c326400 66696e64 5f6e6569 model2d.find_nei
+  0x000003c0 6768626f 7200736e 7072696e 74664040 ghbor.snprintf@@
+  0x000003d0 474c4942 435f322e 322e3500 636d7066 GLIBC_2.2.5.cmpf
+  0x000003e0 756e635f 646f7562 6c65006c 755f6465 unc_double.lu_de
+  0x000003f0 636f6d70 6f736974 696f6e00 645f6172 composition.d_ar
+  0x00000400 616e6765 00506172 74697469 6f6e3264 ange.Partition2d
+  0x00000410 006d7431 39393337 5f676574 5f666c6f .mt19937_get_flo
+  0x00000420 61745f72 616e6765 00636f76 5f6d6f64 at_range.cov_mod
+  0x00000430 656c006d 61747269 78666f72 6d006d74 el.matrixform.mt
+  0x00000440 31393933 375f6765 6e657261 74650063 19937_generate.c
+  0x00000450 5f617272 61795f6d 65616e5f 6c6f6e67 _array_mean_long
+  0x00000460 5f6c6f6e 67007661 7269616e 63650063 _long.variance.c
+  0x00000470 5f617272 61795f76 61725f6c 6f6e675f _array_var_long_
+  0x00000480 6c6f6e67 00635f61 72726179 5f737464 long.c_array_std
+  0x00000490 5f696e74 006d7431 39393337 5f72616e _int.mt19937_ran
+  0x000004a0 646f6d5f 6e6f726d 616c0063 616c6c6f dom_normal.callo
+  0x000004b0 63404047 4c494243 5f322e32 2e350063 c@@GLIBC_2.2.5.c
+  0x000004c0 5f617272 61795f6d 696e5f64 6f75626c _array_min_doubl
+  0x000004d0 6500636f 765f6d6f 64656c5f 696e6974 e.cov_model_init
+  0x000004e0 00667072 696e7466 4040474c 4942435f .fprintf@@GLIBC_
+  0x000004f0 322e322e 35007367 73696d5f 745f6672 2.2.5.sgsim_t_fr
+  0x00000500 6565005f 5f676d6f 6e5f7374 6172745f ee.__gmon_start_
+  0x00000510 5f00635f 61727261 795f6d69 6e5f696e _.c_array_min_in
+  0x00000520 7400635f 61727261 795f7374 645f646f t.c_array_std_do
+  0x00000530 75626c65 00635f61 72726179 5f6d6178 uble.c_array_max
+  0x00000540 5f696e74 006b7269 67655f70 6172616d _int.krige_param
+  0x00000550 5f736574 74696e67 00635f61 72726179 _setting.c_array
+  0x00000560 5f73756d 5f6c6f6e 67006d74 31393933 _sum_long.mt1993
+  0x00000570 375f696e 69740063 6d706675 6e635f66 7_init.cmpfunc_f
+  0x00000580 6c6f6174 0073696d 706c655f 6b726967 loat.simple_krig
+  0x00000590 696e6700 635f6172 7261795f 6d65616e ing.c_array_mean
+  0x000005a0 5f666c6f 6174006d 616c6c6f 63404047 _float.malloc@@G
+  0x000005b0 4c494243 5f322e32 2e35006b 72696765 LIBC_2.2.5.krige
+  0x000005c0 5f6d656d 6f72795f 66726565 00657870 _memory_free.exp
+  0x000005d0 005f656e 6400635f 61727261 795f7661 ._end.c_array_va
+  0x000005e0 725f666c 6f617400 5f5f6273 735f7374 r_float.__bss_st
+  0x000005f0 61727400 76617269 6f677261 6d00635f art.variogram.c_
+  0x00000600 61727261 795f6d61 785f646f 75626c65 array_max_double
+  0x00000610 00635f61 72726179 5f6d696e 5f6c6f6e .c_array_min_lon
+  0x00000620 675f6c6f 6e670063 6f73006d 74313939 g_long.cos.mt199
+  0x00000630 33375f67 65745f69 6e743332 5f72616e 37_get_int32_ran
+  0x00000640 67650073 616d706c 696e675f 73746174 ge.sampling_stat
+  0x00000650 655f696e 6974006d 74313939 33375f67 e_init.mt19937_g
+  0x00000660 65745f64 6f75626c 655f7261 6e676500 et_double_range.
+  0x00000670 73677369 6d5f696e 6974006c 6f670066 sgsim_init.log.f
+  0x00000680 6f70656e 4040474c 4942435f 322e322e open@@GLIBC_2.2.
+  0x00000690 35006d74 31393933 375f6765 745f646f 5.mt19937_get_do
+  0x000006a0 75626c65 00706f77 00706572 726f7240 uble.pow.perror@
+  0x000006b0 40474c49 42435f32 2e322e35 006d7431 @GLIBC_2.2.5.mt1
+  0x000006c0 39393337 5f676574 5f666c6f 6174006c 9937_get_float.l
+  0x000006d0 6f673130 00737172 7400636d 7066756e og10.sqrt.cmpfun
+  0x000006e0 635f6c6f 6e670070 64697374 00635f61 c_long.pdist.c_a
+  0x000006f0 72726179 5f737464 5f6c6f6e 675f6c6f rray_std_long_lo
+  0x00000700 6e670065 78697440 40474c49 42435f32 ng.exit@@GLIBC_2
+  0x00000710 2e322e35 005f4954 4d5f7265 67697374 .2.5._ITM_regist
+  0x00000720 6572544d 436c6f6e 65546162 6c650073 erTMCloneTable.s
+  0x00000730 77617000 635f6172 7261795f 6d65616e wap.c_array_mean
+  0x00000740 5f646f75 626c6500 635f6172 7261795f _double.c_array_
+  0x00000750 7374645f 666c6f61 7400635f 61727261 std_float.c_arra
+  0x00000760 795f6d61 785f6c6f 6e675f6c 6f6e6700 y_max_long_long.
+  0x00000770 635f6172 7261795f 73756d5f 646f7562 c_array_sum_doub
+  0x00000780 6c65005f 5f637861 5f66696e 616c697a le.__cxa_finaliz
+  0x00000790 65404047 4c494243 5f322e32 2e3500   e@@GLIBC_2.2.5.
```

#### readelf --wide --decompress --hex-dump=.shstrtab {}

```diff
@@ -1,20 +1,19 @@
 
 Hex dump of section '.shstrtab':
   0x00000000 002e7379 6d746162 002e7374 72746162 ..symtab..strtab
   0x00000010 002e7368 73747274 6162002e 6e6f7465 ..shstrtab..note
-  0x00000020 2e676e75 2e70726f 70657274 79002e6e .gnu.property..n
-  0x00000030 6f74652e 676e752e 6275696c 642d6964 ote.gnu.build-id
-  0x00000040 002e676e 752e6861 7368002e 64796e73 ..gnu.hash..dyns
-  0x00000050 796d002e 64796e73 7472002e 676e752e ym..dynstr..gnu.
-  0x00000060 76657273 696f6e00 2e676e75 2e766572 version..gnu.ver
-  0x00000070 73696f6e 5f72002e 72656c61 2e64796e sion_r..rela.dyn
-  0x00000080 002e7265 6c612e70 6c74002e 696e6974 ..rela.plt..init
-  0x00000090 002e706c 742e676f 74002e70 6c742e73 ..plt.got..plt.s
-  0x000000a0 6563002e 74657874 002e6669 6e69002e ec..text..fini..
-  0x000000b0 726f6461 7461002e 65685f66 72616d65 rodata..eh_frame
-  0x000000c0 5f686472 002e6568 5f667261 6d65002e _hdr..eh_frame..
-  0x000000d0 696e6974 5f617272 6179002e 66696e69 init_array..fini
-  0x000000e0 5f617272 6179002e 64796e61 6d696300 _array..dynamic.
-  0x000000f0 2e676f74 2e706c74 002e6461 7461002e .got.plt..data..
-  0x00000100 62737300 2e636f6d 6d656e74 00       bss..comment.
+  0x00000020 2e676e75 2e627569 6c642d69 64002e67 .gnu.build-id..g
+  0x00000030 6e752e68 61736800 2e64796e 73796d00 nu.hash..dynsym.
+  0x00000040 2e64796e 73747200 2e676e75 2e766572 .dynstr..gnu.ver
+  0x00000050 73696f6e 002e676e 752e7665 7273696f sion..gnu.versio
+  0x00000060 6e5f7200 2e72656c 612e6479 6e002e72 n_r..rela.dyn..r
+  0x00000070 656c612e 706c7400 2e696e69 74002e70 ela.plt..init..p
+  0x00000080 6c742e67 6f74002e 74657874 002e6669 lt.got..text..fi
+  0x00000090 6e69002e 726f6461 7461002e 65685f66 ni..rodata..eh_f
+  0x000000a0 72616d65 5f686472 002e6568 5f667261 rame_hdr..eh_fra
+  0x000000b0 6d65002e 696e6974 5f617272 6179002e me..init_array..
+  0x000000c0 66696e69 5f617272 6179002e 64796e61 fini_array..dyna
+  0x000000d0 6d696300 2e676f74 2e706c74 002e6461 mic..got.plt..da
+  0x000000e0 7461002e 62737300 2e636f6d 6d656e74 ta..bss..comment
+  0x000000f0 00                                  .
```

### Comparing `uc_sgsim-1.2.0rc0/uc_sgsim/cov_model/base.py` & `uc_sgsim-1.2.1/uc_sgsim/cov_model/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,21 +4,23 @@
 
 class CovModel:
     def __init__(
         self,
         bandwidth_len: float,
         bandwidth_step: float,
         k_range: float,
-        sill=1,
+        sill: float = 1,
+        nugget: float = 0,
     ):
         self.__bandwidth_len = bandwidth_len
         self.__bandwidth_step = bandwidth_step
         self.__bandwidth = np.arange(0, bandwidth_len, bandwidth_step)
         self.__k_range = k_range
         self.__sill = sill
+        self.__nugget = nugget
 
     @property
     def bandwidth_len(self) -> float:
         return self.__bandwidth_len
 
     @property
     def bandwidth_step(self) -> float:
@@ -32,14 +34,18 @@
     def k_range(self) -> float:
         return self.__k_range
 
     @property
     def sill(self) -> float:
         return self.__sill
 
+    @property
+    def nugget(self) -> float:
+        return self.__nugget
+
     def cov_compute(self, x: np.array) -> np.array:
         cov = np.empty(len(x))
         for i in range(len(x)):
             cov[i] = self.__sill - self.model(x[i])
 
         return cov
```

### Comparing `uc_sgsim-1.2.0rc0/uc_sgsim/krige/base.py` & `uc_sgsim-1.2.1/uc_sgsim/krige/base.py`

 * *Files identical despite different names*

### Comparing `uc_sgsim-1.2.0rc0/uc_sgsim/krige/kriging.py` & `uc_sgsim-1.2.1/uc_sgsim/krige/kriging.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,56 +9,57 @@
         super().__init__(model)
 
     def prediction(self, sample: np.array, unsampled: np.array) -> tuple[float, float]:
         n_sampled = len(sample)
         dist_diff = abs(sample[:, 0] - unsampled)
         dist_diff = dist_diff.reshape(len(dist_diff), 1)
 
-        L = np.hstack([sample, dist_diff])
+        grid = np.hstack([sample, dist_diff])
         meanvalue = 0
 
-        cov_dist = np.matrix(self.model.cov_compute(L[:, 2])).T
-        cov_data = squareform(pdist(L[:, :1])).flatten()
+        cov_dist = np.array(self.model.cov_compute(grid[:, 2])).reshape(-1, 1)
+        cov_data = squareform(pdist(grid[:, :1])).flatten()
         cov_data = np.array(self.model.cov_compute(cov_data))
         cov_data = cov_data.reshape(n_sampled, n_sampled)
 
-        weights = np.linalg.inv(cov_data) * cov_dist
-        residuals = L[:, 1] - meanvalue
+        weights = np.linalg.solve(cov_data, cov_dist)
+
+        residuals = grid[:, 1] - meanvalue
         estimation = np.dot(weights.T, residuals) + meanvalue
-        krige_var = float(1 - np.dot(weights.T, cov_dist))
+        krige_var = float(self.model.sill - np.dot(weights.T, cov_dist))
 
         if krige_var < 0:
             krige_var = 0
 
         krige_std = np.sqrt(krige_var)
 
         return estimation, krige_std
 
-    def simulation(self, x: int, unsampled: int, **kwargs) -> float:
+    def simulation(self, x: np.array, unsampled: np.array, **kwargs) -> float:
         neighbor = kwargs.get('neighbor')
-        if neighbor:
+        if neighbor is not None:
             dist = abs(x[:, 0] - unsampled)
             dist = dist.reshape(len(dist), 1)
             has_neighbor = self.find_neighbor(dist, neighbor)
             if has_neighbor:
                 return has_neighbor
             x = np.hstack([x, dist])
             x = np.array(sorted(x, key=lambda itr: itr[2])[:neighbor])
 
         estimation, krige_std = self.prediction(x, unsampled)
 
         random_fix = np.random.normal(0, krige_std, 1)
         return estimation + random_fix
 
-    def find_neighbor(self, dist: list, neighbor: int) -> float:
+    def find_neighbor(self, dist: list[float], neighbor: int) -> float:
         if neighbor == 0:
-            return np.random.normal(0, 1, 1)
+            return np.random.normal(0, self.model.sill**0.5, 1)
         close_point = 0
 
         criteria = self.k_range * 1.732 if self.model.model_name == 'Gaussian' else self.k_range
 
         for item in dist:
             if item <= criteria:
                 close_point += 1
 
         if close_point == 0:
-            return np.random.normal(0, 1, 1)
+            return np.random.normal(0, self.model.sill**0.5, 1)
```

### Comparing `uc_sgsim-1.2.0rc0/uc_sgsim/plot/base.py` & `uc_sgsim-1.2.1/uc_sgsim/plot/base.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import numpy as np
 
 from uc_sgsim.cov_model.base import CovModel
 
 
 class PlotBase:
-    def __init__(self, model: CovModel, random_field: np.array, figsize=(10, 8)):
+    def __init__(self, model: CovModel, random_field: np.array, figsize: tuple = (10, 8)):
         self.__model = model
         self.__random_field = random_field
         self.__figsize = figsize
         self.__model_name = model.model_name
         self.__bandwidth_step = model.bandwidth_step
         self.__bandwidth = model.bandwidth
         self.__k_range = model.k_range
```

### Comparing `uc_sgsim-1.2.0rc0/uc_sgsim/plot/plot.py` & `uc_sgsim-1.2.1/uc_sgsim/plot/plot.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,40 +8,38 @@
 
 class Visualize(PlotBase):
     xlabel = 'Distance(-)'
 
     def __init__(self, model: CovModel, random_field: np.array):
         super().__init__(model, random_field)
 
-    def mean_plot(self, n, mean=0, std=1) -> None:
+    def mean_plot(self, n, mean=0) -> None:
         realization_number = len(self.random_field[:, 0])
-
         if n == 'ALL':
             for i in range(realization_number):
                 plt.figure(77879, figsize=self.figsize)
-                plt.plot(self.random_field[i, :] * std + mean)
+                plt.plot(self.random_field[i, :] + mean)
                 plt.title('Realizations: ' + self.model_name, fontsize=20)
                 plt.xlabel(self.xlabel, fontsize=20)
                 plt.axhline(y=mean, color='r', linestyle='--', zorder=1)
-                plt.ylabel('S', fontsize=20)
+                plt.ylabel('Y', fontsize=20)
 
         else:
             for item in n:
                 plt.figure(77879, figsize=self.figsize)
-                plt.plot(self.random_field[:, item] * std + mean)
+                plt.plot(self.random_field[:, item] + mean)
                 plt.title('Realizations: ' + self.model_name, fontsize=20)
                 plt.xlabel(self.xlabel, fontsize=20)
                 plt.axhline(y=mean, color='r', linestyle='--', zorder=1)
                 plt.ylabel('Y', fontsize=20)
 
-    def variance_plot(self, mean=0, std=1) -> None:
+    def variance_plot(self, mean=0) -> None:
         zmean = np.zeros(len(self.random_field[0, :]))
-
         for i in range(len(self.random_field[0, :])):
-            zmean[i] = np.mean(self.random_field[:, i] * std + mean)
+            zmean[i] = np.mean(self.random_field[:, i] + mean)
 
         plt.figure(5212, figsize=self.figsize)
         plt.plot(
             zmean,
             '-s',
             color='k',
             markeredgecolor='k',
@@ -51,27 +49,27 @@
         plt.ylabel('Mean', fontsize=20)
         plt.axhline(y=mean, color='r', linestyle='--', zorder=1)
         plt.xticks(fontsize=17), plt.yticks(fontsize=17)
 
         zvar = np.zeros(len(self.random_field[0, :]))
 
         for i in range(len(self.random_field[0, :])):
-            zvar[i] = np.var(self.random_field[:, i] * std)
+            zvar[i] = np.var(self.random_field[:, i])
 
         plt.figure(52712, figsize=self.figsize)
         plt.plot(
             zvar,
             '-o',
             color='k',
             markeredgecolor='k',
             markerfacecolor='r',
         )
         plt.xlabel(self.xlabel, fontsize=20)
         plt.ylabel('Variance', fontsize=20)
-        plt.axhline(y=std**2, color='b', linestyle='--', zorder=1)
+        plt.axhline(y=self.model.sill, color='b', linestyle='--', zorder=1)
         plt.xticks(fontsize=17), plt.yticks(fontsize=17)
 
     def cdf_plot(self, x_location: int) -> None:
 
         X = self.random_field[:, x_location]
 
         mu = np.mean(X)
```

### Comparing `uc_sgsim-1.2.0rc0/uc_sgsim/random_field.py` & `uc_sgsim-1.2.1/uc_sgsim/random_field.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,15 +52,20 @@
     def bandwidth(self) -> np.array:
         return self.__bandwidth
 
     @property
     def bandwidth_step(self) -> int:
         return self.__bandwidth_step
 
-    def save_random_field(self, path: str, file_type='csv', save_single=False) -> None:
+    def save_random_field(
+        self,
+        path: str,
+        file_type: str = 'csv',
+        save_single: bool = False,
+    ) -> None:
         digit = int(np.log10(self.realization_number))
         number_head = ''
         for i in range(digit):
             number_head += '0'
         num_val = 1
         if save_single is False:
             for i in range(self.realization_number):
@@ -74,15 +79,15 @@
                     self.random_field,
                     file_type,
                     'Realizations',
                 )
         else:
             save_as_one_file(path, self.random_field)
 
-    def save_variogram(self, path: str, file_type='csv', save_single=False) -> None:
+    def save_variogram(self, path: str, file_type: str = 'csv', save_single: bool = False) -> None:
         if type(self.variogram) == int:
             raise VariogramDoesNotCompute()
         digit = int(np.log10(self.realization_number))
         number_head = ''
         for i in range(digit):
             number_head += '0'
         num_val = 1
```

### Comparing `uc_sgsim-1.2.0rc0/uc_sgsim/sgsim.py` & `uc_sgsim-1.2.1/uc_sgsim/sgsim.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import time
+from typing import Union
 import sys
 from pathlib import Path
 from ctypes import CDLL, POINTER, c_double, c_int
 from multiprocessing import Pool
 
 import numpy as np
 from uc_sgsim.exception import VariogramDoesNotCompute
@@ -17,125 +18,120 @@
 
 class UCSgsim(RandomField):
     def __init__(
         self,
         x: int,
         model: CovModel,
         realization_number: int,
-        krige_method='SimpleKrige',
+        krige_method: str = 'SimpleKrige',
     ):
         super().__init__(x, model, realization_number)
         self.krige_method = krige_method
 
-    def compute(self, randomseed=0, parallel=False) -> np.array:
+    def _process(self, randomseed: int = 0, parallel: bool = False) -> np.array:
         self.randomseed = randomseed
         if parallel is False:
             self.n_process = 1
 
         if self.krige_method == 'SimpleKrige':
             self.krige = SimpleKrige(self.model)
 
         counts = 0
 
         start_time = time.time()
         np.random.seed(self.randomseed)
         while counts < self.realization_number // self.n_process:
-            unsampled = np.linspace(0, self.x_size - 1, self.x_size)
-
-            y_value = np.random.normal(0, 1, 2).reshape(2, 1)
+            unsampled = np.linspace(1, self.x_size - 2, self.x_size - 2)
+            y_value = np.random.normal(0, self.model.sill**0.5, 2).reshape(2, 1)
             x_grid = np.array([0, self.x_size - 1]).reshape(2, 1)
             z = np.zeros(self.x_size)
             z[0], z[-1] = y_value[0], y_value[1]
-            unsampled = np.delete(unsampled, [0, -1])
             neigh = 0
 
-            L = np.hstack([x_grid, y_value])
+            grid = np.hstack([x_grid, y_value])
 
             randompath = np.random.choice(
                 unsampled,
                 len(unsampled),
                 replace=False,
             )
 
             for i in range(len(unsampled)):
                 z[int(randompath[i])] = self.krige.simulation(
-                    L,
+                    grid,
                     randompath[i],
                     neighbor=neigh,
                 )
                 temp = np.hstack([randompath[i], z[int(randompath[i])]])
-                L = np.vstack([L, temp])
+                grid = np.vstack([grid, temp])
 
                 if neigh < 8:
                     neigh += 1
 
             self.randomseed += 1
 
-            z_gap = abs(z.max() - z.min())
-
-            if 2 < z_gap <= 6.5:
-                self.random_field[counts, :] = z
-                counts = counts + 1
-                print('Progress = %.2f' % (counts / self.realization_number * 100) + '%', end='\r')
+            self.random_field[counts, :] = z
+            counts = counts + 1
+            print('Progress = %.2f' % (counts / self.realization_number * 100) + '%', end='\r')
 
         print('Progress = %.2f' % 100 + '%\n', end='\r')
         end_time = time.time()
         print('Time = %f' % (end_time - start_time), 's\n')
 
         return self.random_field
 
-    def compute_async(self, n_process: int, randomseed: int) -> np.array:
+    def compute(self, n_process: int, randomseed: int) -> np.array:
         pool = Pool(processes=n_process)
         self.n_process = n_process
         self.realization_number = self.realization_number * n_process
         self.random_field = np.empty([self.realization_number, self.x_size])
 
         rand_list = []
         parallel = []
         for i in range(n_process):
             s = randomseed + int(i)
             rand_list.append(int(s))
             parallel.append(True)
 
-        z = pool.starmap(self.compute, zip(rand_list, parallel))
+        z = pool.starmap(self._process, zip(rand_list, parallel))
         pool.close()
         # use pool.join() to measure the coverage of sub process
         pool.join()
 
         for i in range(n_process):
             for j in range(int(self.realization_number / n_process)):
                 start = int(i * self.realization_number / n_process)
                 self.random_field[j + start, :] = z[i][j, :]
 
         return self.random_field
 
-    def variogram_compute(self, n_process=1) -> None:
+    def variogram_compute(self, n_process: int = 1) -> None:
         pool = Pool(processes=n_process)
         model_len = self.x_size
         x = np.linspace(0, self.x_size - 1, model_len).reshape(model_len, 1)
 
-        L = []
+        grid = []
         for i in range(self.realization_number):
-            L.append(
+            grid.append(
                 np.hstack([x, self.random_field[i, :].reshape(model_len, 1)]),
             )
 
-        self.variogram = pool.starmap(self.model.variogram, zip(L))
+        self.variogram = pool.starmap(self.model.variogram, zip(grid))
         pool.close()
         # use pool.join() to measure the coverage of sub process
         pool.join()
         self.variogram = np.array(self.variogram)
 
-    def mean_plot(self, n, mean=0, std=1) -> None:
+    def mean_plot(self, n: Union[str, list[int]], mean: float = 0) -> None:
         m_plot = Visualize(self.model, self.random_field)
-        m_plot.mean_plot(n, mean, std)
+        m_plot.mean_plot(n, mean)
 
-    def variance_plot(self, mean=0, std=1) -> None:
+    def variance_plot(self, mean: float = 0) -> None:
         s_plot = Visualize(self.model, self.random_field)
-        s_plot.variance_plot(mean, std)
+        s_plot.variance_plot(mean)
 
     def cdf_plot(self, x_location: int) -> None:
         c_plot = Visualize(self.model, self.random_field)
         c_plot.cdf_plot(x_location)
 
     def hist_plot(self, x_location: int) -> None:
         h_plot = Visualize(self.model, self.random_field)
@@ -150,28 +146,28 @@
 
 class UCSgsimDLL(UCSgsim):
     def __init__(
         self,
         x: int,
         model: CovModel,
         realization_number: int,
-        krige_method='SimpleKrige',
+        krige_method: str = 'SimpleKrige',
     ):
         super().__init__(x, model, realization_number)
         self.krige_method = krige_method
 
-    def lib_read(self) -> CDLL:
+    def _lib_read(self) -> CDLL:
         if sys.platform.startswith('linux'):
             lib = CDLL(str(BASE_DIR) + r'/c_core/uc_sgsim.so')
         elif sys.platform.startswith('win32'):
             lib = CDLL(str(BASE_DIR) + r'/c_core/uc_sgsim.dll', winmode=0)
         return lib
 
-    def cpdll(self, randomseed: int) -> np.array:
-        lib = self.lib_read()
+    def _cpdll(self, randomseed: int) -> np.array:
+        lib = self._lib_read()
         mlen = int(self.x_size)
         realization_number = int(self.realization_number // self.n_process)
         random_field = np.empty([realization_number, self.x_size])
 
         sgsim_init = lib.sgsim_init
         sgsim_init.argtypes = (
             POINTER(SgsimStructure),
@@ -189,15 +185,22 @@
         cov_init.argtypes = (
             POINTER(CovModelStructure),
             c_int,
             c_int,
             c_double,
             c_double,
         )
-        cov_init(cov_s, 1, 35, 17.32, 1)
+        cov_init(
+            cov_s,
+            self.model.bandwidth_len,
+            self.model.bandwidth_step,
+            self.model.k_range,
+            self.model.sill,
+            self.model.nugget,
+        )
 
         sgsim = lib.sgsim_run
         sgsim.argtypes = (POINTER(SgsimStructure), POINTER(CovModelStructure), c_int)
         sgsim(sgsim_s, cov_s, 0)
 
         # array = as_array(sgsim_s.array, shape=(realization_number * mlen, 1))
         for i in range(realization_number):
@@ -214,29 +217,29 @@
         self.random_field = np.empty([self.realization_number, self.x_size])
 
         rand_list = []
         for i in range(n_process):
             s = randomseed + int(i)
             rand_list.append(int(s))
 
-        z = pool.starmap(self.cpdll, zip(rand_list))
-        print(len(z))
+        z = pool.starmap(self._cpdll, zip(rand_list))
+
         pool.close()
         # use pool.join() to measure the coverage of sub process
         pool.join()
 
         for i in range(n_process):
             for j in range(int(self.realization_number / n_process)):
                 start = int(i * self.realization_number / n_process)
                 self.random_field[j + start, :] = z[i][j, :]
 
         return self.random_field
 
-    def variogram_cpdll(self, cpu_number: int) -> np.array:
-        lib = self.lib_read()
+    def _variogram_cpdll(self, n_process: int) -> np.array:
+        lib = self._lib_read()
         vario = lib.variogram
         vario.argtypes = (
             POINTER(c_double),
             POINTER(c_double),
             c_int,
             c_int,
             c_int,
@@ -250,33 +253,33 @@
 
         vario_array = (c_double * (vario_size))()
         random_field_array = (c_double * (mlen))()
 
         variogram = np.empty([realization_number, vario_size])
 
         for i in range(realization_number):
-            random_field_array[:] = self.random_field[i + cpu_number * realization_number, :]
+            random_field_array[:] = self.random_field[i + n_process * realization_number, :]
             vario(random_field_array, vario_array, mlen, vario_size, 1)
             variogram[i, :] = list(vario_array)
 
         return variogram
 
-    def variogram_compute(self, n_process=1) -> np.array:
+    def variogram_compute(self, n_process: int = 1) -> np.array:
         pool = Pool(processes=n_process)
         self.n_process = n_process
 
-        if n_process < 1:
+        if n_process > 1:
             self.realization_number = self.realization_number * n_process
 
         self.variogram = np.empty([self.realization_number, len(self.bandwidth)])
         cpu_number = []
         for i in range(self.n_process):
             cpu_number.append(i)
 
-        z = pool.starmap(self.variogram_cpdll, zip(cpu_number))
+        z = pool.starmap(self._variogram_cpdll, zip(cpu_number))
         pool.close()
         # use pool.join() to measure the coverage of sub process
         pool.join()
 
         for i in range(n_process):
             for j in range(int(self.realization_number / n_process)):
                 self.variogram[(j + int(i * self.realization_number / n_process)), :] = z[i][j, :]
```

### Comparing `uc_sgsim-1.2.0rc0/uc_sgsim/utils.py` & `uc_sgsim-1.2.1/uc_sgsim/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,8 +45,9 @@
 
 class CovModelStructure(Structure):
     _fields_ = [
         ('bw', c_int),
         ('hs', c_int),
         ('range', c_double),
         ('sill', c_double),
+        ('nugget', c_double),
     ]
```

### Comparing `uc_sgsim-1.2.0rc0/uc_sgsim.egg-info/PKG-INFO` & `uc_sgsim-1.2.1/uc_sgsim.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 Metadata-Version: 2.1
 Name: uc-sgsim
-Version: 1.2.0rc0
+Version: 1.2.1
 Summary: Random Field Generation
 Home-page: https://github.com/Zncl2222/Stochastic_UC_SGSIM
 Author: Zncl2222
 Author-email: 3002shinning@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering :: Mathematics
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 ![licence](https://img.shields.io/github/license/Zncl2222/Stochastic_UC_SGSIM)
 ![python](https://img.shields.io/pypi/pyversions/uc-sgsim)
 ![language](https://img.shields.io/badge/Solutions-black.svg?style=flat&logo=c%2B%2B)
 ![language](https://img.shields.io/badge/Solutions-black.svg?style=flat&logo=python)
 [![ci](https://github.com/Zncl2222/Stochastic_UC_SGSIM/actions/workflows/github-pre-commit.yml/badge.svg)](https://github.com/Zncl2222/Stochastic_UC_SGSIM/actions/workflows/github-pre-commit.yml)
 [![build](https://github.com/Zncl2222/Stochastic_UC_SGSIM/actions/workflows/cmake.yml/badge.svg)](https://github.com/Zncl2222/Stochastic_UC_SGSIM/actions/workflows/cmake.yml)
 [![build](https://github.com/Zncl2222/Stochastic_UC_SGSIM/actions/workflows/codeql.yml/badge.svg)](https://github.com/Zncl2222/Stochastic_UC_SGSIM/actions/workflows/codeql.yml)
-[![codecov](https://codecov.io/github/Zncl2222/Stochastic_UC_SGSIM/branch/main/graph/badge.svg?token=3qZt0OqDNI)](https://app.codecov.io/github/Zncl2222/Stochastic_UC_SGSIM)
+[![codecov](https://codecov.io/gh/Zncl2222/uc_sgsim/branch/main/graph/badge.svg?token=3qZt0OqDNI)](https://codecov.io/gh/Zncl2222/uc_sgsim)
 
 #### Python Sonar Cloud state
 [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=zncl2222_Stochastic_UC_SGSIM_py&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=zncl2222_Stochastic_UC_SGSIM_py)
 [![Reliability Rating](https://sonarcloud.io/api/project_badges/measure?project=zncl2222_Stochastic_UC_SGSIM_py&metric=reliability_rating)](https://sonarcloud.io/summary/new_code?id=zncl2222_Stochastic_UC_SGSIM_py)
 [![Security Rating](https://sonarcloud.io/api/project_badges/measure?project=zncl2222_Stochastic_UC_SGSIM_py&metric=security_rating)](https://sonarcloud.io/summary/new_code?id=zncl2222_Stochastic_UC_SGSIM_py)
 [![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=zncl2222_Stochastic_UC_SGSIM_py&metric=sqale_rating)](https://sonarcloud.io/summary/new_code?id=zncl2222_Stochastic_UC_SGSIM_py)
 
@@ -161,27 +163,27 @@
    <img src="https://github.com/Zncl2222/Stochastic_SGSIM/blob/main/figure/Variogram.png"  width="50%"/>
    <img src="https://github.com/Zncl2222/Stochastic_SGSIM/blob/main/figure/HIST.png"  width="40%"/>
    <img src="https://github.com/Zncl2222/Stochastic_SGSIM/blob/main/figure/CDF.png"  width="50%"/>
 </p>
 
 ## Future plans
 * 2D unconditional randomfield generation
-* GUI mode in pyhton package
+* GUI mode in pyhton
 * More covariance models
 * More kriging methods (etc. Oridinary Kriging)
 * Performance enhancement
 * More completely documents and easy to use designs.
 
 ## Performance
 <p align="center">
 <img src="https://github.com/Zncl2222/Stochastic_SGSIM/blob/main/figure/C_Cpp_py_comparision.png"  width="70%"/>
 </p>
 
 ```
-Parameters for testing:
+Parameters:
 
 model len = 150
 
 number of realizations = 1000
 
 Range scale = 17.32
```

### Comparing `uc_sgsim-1.2.0rc0/uc_sgsim.egg-info/SOURCES.txt` & `uc_sgsim-1.2.1/uc_sgsim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

