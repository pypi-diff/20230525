# Comparing `tmp/pir_client-1.1.0-py3-none-any.whl.zip` & `tmp/pir_client-1.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 3273 bytes, number of entries: 6
--rw-r--r--  2.0 unx        0 b- defN 19-Sep-20 13:17 pir_client/__init__.py
--rw-r--r--  2.0 unx     3368 b- defN 19-Sep-20 13:17 pir_client/client.py
--rw-r--r--  2.0 unx     2369 b- defN 19-Sep-20 13:18 pir_client-1.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 19-Sep-20 13:18 pir_client-1.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 19-Sep-20 13:18 pir_client-1.1.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      463 b- defN 19-Sep-20 13:18 pir_client-1.1.0.dist-info/RECORD
-6 files, 6303 bytes uncompressed, 2431 bytes compressed:  61.4%
+Zip file size: 3266 bytes, number of entries: 6
+-rw-r--r--  2.0 unx        0 b- defN 23-May-25 09:58 pir_client/__init__.py
+-rw-r--r--  2.0 unx     3368 b- defN 23-May-25 09:58 pir_client/client.py
+-rw-r--r--  2.0 unx     2402 b- defN 23-May-25 09:58 pir_client-1.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-25 09:58 pir_client-1.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-May-25 09:58 pir_client-1.2.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      463 b- defN 23-May-25 09:58 pir_client-1.2.0.dist-info/RECORD
+6 files, 6336 bytes uncompressed, 2424 bytes compressed:  61.7%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: pir_client/__init__.py
 Comment: 
 
 Filename: pir_client/client.py
 Comment: 
 
-Filename: pir_client-1.1.0.dist-info/METADATA
+Filename: pir_client-1.2.0.dist-info/METADATA
 Comment: 
 
-Filename: pir_client-1.1.0.dist-info/WHEEL
+Filename: pir_client-1.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: pir_client-1.1.0.dist-info/top_level.txt
+Filename: pir_client-1.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: pir_client-1.1.0.dist-info/RECORD
+Filename: pir_client-1.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `pir_client-1.1.0.dist-info/METADATA` & `pir_client-1.2.0.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pir-client
-Version: 1.1.0
+Version: 1.2.0
 Summary: API client for PIR
 Home-page: https://github.com/uktrade/invest-pir-api-client
 Author: Department for International Trade
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -14,27 +14,29 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 1.11
 Classifier: Framework :: Django :: 2.0
 Classifier: Framework :: Django :: 2.1
 Classifier: Framework :: Django :: 2.2
+Classifier: Framework :: Django :: 4.2
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
-Requires-Dist: directory-client-core (<7.0.0,>=6.1.0)
+Requires-Dist: directory-client-core (<=7.2.2,>=6.1.0)
 Provides-Extra: test
-Requires-Dist: pytest (==3.0.2) ; extra == 'test'
-Requires-Dist: pytest-cov (==2.3.1) ; extra == 'test'
-Requires-Dist: pytest-sugar (==0.8.0) ; extra == 'test'
-Requires-Dist: flake8 (==3.0.4) ; extra == 'test'
+Requires-Dist: pytest (==5.4.0) ; extra == 'test'
+Requires-Dist: pytest-codecov ; extra == 'test'
+Requires-Dist: pytest-cov ; extra == 'test'
+Requires-Dist: GitPython ; extra == 'test'
+Requires-Dist: pytest-sugar (==0.9.5) ; extra == 'test'
+Requires-Dist: flake8 (==5.0.4) ; extra == 'test'
 Requires-Dist: requests-mock (==1.1.0) ; extra == 'test'
-Requires-Dist: codecov (==2.0.9) ; extra == 'test'
-Requires-Dist: twine (<2.0.0,>=1.11.0) ; extra == 'test'
+Requires-Dist: twine ; extra == 'test'
 Requires-Dist: wheel (<1.0.0,>=0.31.0) ; extra == 'test'
-Requires-Dist: setuptools (<39.0.0,>=38.6.0) ; extra == 'test'
+Requires-Dist: setuptools ; extra == 'test'
 Requires-Dist: httpretty ; extra == 'test'
 
 # Invest PIR API Client
 [![CircleCI](https://circleci.com/gh/uktrade/invest-pir-api-client.svg?style=svg)](https://circleci.com/gh/uktrade/invest-pir-api-client)
 [![codecov](https://codecov.io/gh/uktrade/invest-pir-api-client/branch/master/graph/badge.svg)](https://codecov.io/gh/uktrade/invest-pir-api-client)
 [![PyPI](https://img.shields.io/pypi/v/pir-client.svg)](https://pypi.org/project/pir-client/)
```

