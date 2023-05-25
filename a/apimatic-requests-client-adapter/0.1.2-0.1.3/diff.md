# Comparing `tmp/apimatic-requests-client-adapter-0.1.2.tar.gz` & `tmp/apimatic-requests-client-adapter-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apimatic-requests-client-adapter-0.1.2.tar", last modified: Thu Feb 16 12:41:29 2023, max compression
+gzip compressed data, was "apimatic-requests-client-adapter-0.1.3.tar", last modified: Tue Apr  4 08:47:19 2023, max compression
```

## Comparing `apimatic-requests-client-adapter-0.1.2.tar` & `apimatic-requests-client-adapter-0.1.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 12:41:29.988920 apimatic-requests-client-adapter-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-02-16 12:41:14.000000 apimatic-requests-client-adapter-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-02-16 12:41:14.000000 apimatic-requests-client-adapter-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-02-16 12:41:29.988920 apimatic-requests-client-adapter-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-02-16 12:41:14.000000 apimatic-requests-client-adapter-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 12:41:29.988920 apimatic-requests-client-adapter-0.1.2/apimatic_requests_client_adapter/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-02-16 12:41:14.000000 apimatic-requests-client-adapter-0.1.2/apimatic_requests_client_adapter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5495 2023-02-16 12:41:14.000000 apimatic-requests-client-adapter-0.1.2/apimatic_requests_client_adapter/requests_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 12:41:29.988920 apimatic-requests-client-adapter-0.1.2/apimatic_requests_client_adapter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-02-16 12:41:29.000000 apimatic-requests-client-adapter-0.1.2/apimatic_requests_client_adapter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-02-16 12:41:29.000000 apimatic-requests-client-adapter-0.1.2/apimatic_requests_client_adapter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-16 12:41:29.000000 apimatic-requests-client-adapter-0.1.2/apimatic_requests_client_adapter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-02-16 12:41:29.000000 apimatic-requests-client-adapter-0.1.2/apimatic_requests_client_adapter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-02-16 12:41:29.000000 apimatic-requests-client-adapter-0.1.2/apimatic_requests_client_adapter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-16 12:41:29.988920 apimatic-requests-client-adapter-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-02-16 12:41:14.000000 apimatic-requests-client-adapter-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 12:41:29.988920 apimatic-requests-client-adapter-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-02-16 12:41:14.000000 apimatic-requests-client-adapter-0.1.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 12:41:29.988920 apimatic-requests-client-adapter-0.1.2/tests/apimatic_requests_client_adapter/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-02-16 12:41:14.000000 apimatic-requests-client-adapter-0.1.2/tests/apimatic_requests_client_adapter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-02-16 12:41:14.000000 apimatic-requests-client-adapter-0.1.2/tests/apimatic_requests_client_adapter/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 12:41:29.988920 apimatic-requests-client-adapter-0.1.2/tests/apimatic_requests_client_adapter/models/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-02-16 12:41:14.000000 apimatic-requests-client-adapter-0.1.2/tests/apimatic_requests_client_adapter/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 12:41:29.988920 apimatic-requests-client-adapter-0.1.2/tests/apimatic_requests_client_adapter/models/external/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-02-16 12:41:14.000000 apimatic-requests-client-adapter-0.1.2/tests/apimatic_requests_client_adapter/models/external/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-02-16 12:41:14.000000 apimatic-requests-client-adapter-0.1.2/tests/apimatic_requests_client_adapter/models/external/http_response.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 12:41:29.988920 apimatic-requests-client-adapter-0.1.2/tests/apimatic_requests_client_adapter/models/internal/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-02-16 12:41:14.000000 apimatic-requests-client-adapter-0.1.2/tests/apimatic_requests_client_adapter/models/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-02-16 12:41:14.000000 apimatic-requests-client-adapter-0.1.2/tests/apimatic_requests_client_adapter/models/internal/http_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-02-16 12:41:14.000000 apimatic-requests-client-adapter-0.1.2/tests/apimatic_requests_client_adapter/models/internal/http_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-02-16 12:41:14.000000 apimatic-requests-client-adapter-0.1.2/tests/apimatic_requests_client_adapter/models/internal/http_response_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 12:41:29.988920 apimatic-requests-client-adapter-0.1.2/tests/apimatic_requests_client_adapter/requests_client_tests/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-02-16 12:41:14.000000 apimatic-requests-client-adapter-0.1.2/tests/apimatic_requests_client_adapter/requests_client_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5726 2023-02-16 12:41:14.000000 apimatic-requests-client-adapter-0.1.2/tests/apimatic_requests_client_adapter/requests_client_tests/test_requests_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 08:47:19.323998 apimatic-requests-client-adapter-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-04 08:47:05.000000 apimatic-requests-client-adapter-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-04 08:47:05.000000 apimatic-requests-client-adapter-0.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-04-04 08:47:19.323998 apimatic-requests-client-adapter-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-04-04 08:47:05.000000 apimatic-requests-client-adapter-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 08:47:19.319998 apimatic-requests-client-adapter-0.1.3/apimatic_requests_client_adapter/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-04 08:47:05.000000 apimatic-requests-client-adapter-0.1.3/apimatic_requests_client_adapter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5495 2023-04-04 08:47:05.000000 apimatic-requests-client-adapter-0.1.3/apimatic_requests_client_adapter/requests_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 08:47:19.323998 apimatic-requests-client-adapter-0.1.3/apimatic_requests_client_adapter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-04-04 08:47:19.000000 apimatic-requests-client-adapter-0.1.3/apimatic_requests_client_adapter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-04-04 08:47:19.000000 apimatic-requests-client-adapter-0.1.3/apimatic_requests_client_adapter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 08:47:19.000000 apimatic-requests-client-adapter-0.1.3/apimatic_requests_client_adapter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-04 08:47:19.000000 apimatic-requests-client-adapter-0.1.3/apimatic_requests_client_adapter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-04 08:47:19.000000 apimatic-requests-client-adapter-0.1.3/apimatic_requests_client_adapter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 08:47:19.323998 apimatic-requests-client-adapter-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-04-04 08:47:05.000000 apimatic-requests-client-adapter-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 08:47:19.323998 apimatic-requests-client-adapter-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-04 08:47:05.000000 apimatic-requests-client-adapter-0.1.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 08:47:19.323998 apimatic-requests-client-adapter-0.1.3/tests/apimatic_requests_client_adapter/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-04 08:47:05.000000 apimatic-requests-client-adapter-0.1.3/tests/apimatic_requests_client_adapter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-04-04 08:47:05.000000 apimatic-requests-client-adapter-0.1.3/tests/apimatic_requests_client_adapter/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 08:47:19.323998 apimatic-requests-client-adapter-0.1.3/tests/apimatic_requests_client_adapter/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-04 08:47:05.000000 apimatic-requests-client-adapter-0.1.3/tests/apimatic_requests_client_adapter/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 08:47:19.323998 apimatic-requests-client-adapter-0.1.3/tests/apimatic_requests_client_adapter/models/external/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-04 08:47:05.000000 apimatic-requests-client-adapter-0.1.3/tests/apimatic_requests_client_adapter/models/external/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-04 08:47:05.000000 apimatic-requests-client-adapter-0.1.3/tests/apimatic_requests_client_adapter/models/external/http_response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 08:47:19.323998 apimatic-requests-client-adapter-0.1.3/tests/apimatic_requests_client_adapter/models/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-04 08:47:05.000000 apimatic-requests-client-adapter-0.1.3/tests/apimatic_requests_client_adapter/models/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-04-04 08:47:05.000000 apimatic-requests-client-adapter-0.1.3/tests/apimatic_requests_client_adapter/models/internal/http_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-04-04 08:47:05.000000 apimatic-requests-client-adapter-0.1.3/tests/apimatic_requests_client_adapter/models/internal/http_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-04 08:47:05.000000 apimatic-requests-client-adapter-0.1.3/tests/apimatic_requests_client_adapter/models/internal/http_response_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 08:47:19.323998 apimatic-requests-client-adapter-0.1.3/tests/apimatic_requests_client_adapter/requests_client_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-04 08:47:05.000000 apimatic-requests-client-adapter-0.1.3/tests/apimatic_requests_client_adapter/requests_client_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5726 2023-04-04 08:47:05.000000 apimatic-requests-client-adapter-0.1.3/tests/apimatic_requests_client_adapter/requests_client_tests/test_requests_client.py
```

### Comparing `apimatic-requests-client-adapter-0.1.2/LICENSE` & `apimatic-requests-client-adapter-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `apimatic-requests-client-adapter-0.1.2/PKG-INFO` & `apimatic-requests-client-adapter-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apimatic-requests-client-adapter
-Version: 0.1.2
+Version: 0.1.3
 Summary: An adapter for requests client library consumed by the SDKs generated with APIMatic
 Home-page: https://github.com/apimatic/requests-client-adapter
 Author: APIMatic
 Author-email: support@apimatic.io
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -15,15 +15,15 @@
 [![Test Coverage][test-coverage-url]][code-climate-url]
 [![Licence][license-badge]][license-url]
 
 ## Introduction
 Requests is a simple, yet elegant, HTTP library. This repository contains the client implementation that uses the requests library for python SDK provided by APIMatic. 
 
 ## Version supported 
-Currenty APIMatic supports  `Python version 3.7 - 3.10`  hence the apimatic-requests-client-adapter will need the same versions to be supported.
+Currenty APIMatic supports  `Python version 3.7 - 3.11`  hence the apimatic-requests-client-adapter will need the same versions to be supported.
 
 ## Installation 
 Simply run the command below in your SDK as the apimatic-requests-client-adapter will be added as a dependency in the SDK.
 ```python
 pip install apimatic-requests-client-adapter
 ```
 **Supported Methods Provided by requests-client**
```

### Comparing `apimatic-requests-client-adapter-0.1.2/README.md` & `apimatic-requests-client-adapter-0.1.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [![Test Coverage][test-coverage-url]][code-climate-url]
 [![Licence][license-badge]][license-url]
 
 ## Introduction
 Requests is a simple, yet elegant, HTTP library. This repository contains the client implementation that uses the requests library for python SDK provided by APIMatic. 
 
 ## Version supported 
-Currenty APIMatic supports  `Python version 3.7 - 3.10`  hence the apimatic-requests-client-adapter will need the same versions to be supported.
+Currenty APIMatic supports  `Python version 3.7 - 3.11`  hence the apimatic-requests-client-adapter will need the same versions to be supported.
 
 ## Installation 
 Simply run the command below in your SDK as the apimatic-requests-client-adapter will be added as a dependency in the SDK.
 ```python
 pip install apimatic-requests-client-adapter
 ```
 **Supported Methods Provided by requests-client**
```

### Comparing `apimatic-requests-client-adapter-0.1.2/apimatic_requests_client_adapter/requests_client.py` & `apimatic-requests-client-adapter-0.1.3/apimatic_requests_client_adapter/requests_client.py`

 * *Files identical despite different names*

### Comparing `apimatic-requests-client-adapter-0.1.2/apimatic_requests_client_adapter.egg-info/PKG-INFO` & `apimatic-requests-client-adapter-0.1.3/apimatic_requests_client_adapter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apimatic-requests-client-adapter
-Version: 0.1.2
+Version: 0.1.3
 Summary: An adapter for requests client library consumed by the SDKs generated with APIMatic
 Home-page: https://github.com/apimatic/requests-client-adapter
 Author: APIMatic
 Author-email: support@apimatic.io
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -15,15 +15,15 @@
 [![Test Coverage][test-coverage-url]][code-climate-url]
 [![Licence][license-badge]][license-url]
 
 ## Introduction
 Requests is a simple, yet elegant, HTTP library. This repository contains the client implementation that uses the requests library for python SDK provided by APIMatic. 
 
 ## Version supported 
-Currenty APIMatic supports  `Python version 3.7 - 3.10`  hence the apimatic-requests-client-adapter will need the same versions to be supported.
+Currenty APIMatic supports  `Python version 3.7 - 3.11`  hence the apimatic-requests-client-adapter will need the same versions to be supported.
 
 ## Installation 
 Simply run the command below in your SDK as the apimatic-requests-client-adapter will be added as a dependency in the SDK.
 ```python
 pip install apimatic-requests-client-adapter
 ```
 **Supported Methods Provided by requests-client**
```

### Comparing `apimatic-requests-client-adapter-0.1.2/apimatic_requests_client_adapter.egg-info/SOURCES.txt` & `apimatic-requests-client-adapter-0.1.3/apimatic_requests_client_adapter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apimatic-requests-client-adapter-0.1.2/setup.py` & `apimatic-requests-client-adapter-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,26 +8,26 @@
         long_description = fh.read()
 else:
     with open('README.md', 'r', encoding='utf-8') as fh:
         long_description = fh.read()
 
 setup(
     name='apimatic-requests-client-adapter',
-    version='0.1.2',
+    version='0.1.3',
     description='An adapter for requests client library consumed by the SDKs generated with APIMatic',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='APIMatic',
     author_email='support@apimatic.io',
     license='MIT',
     url='https://github.com/apimatic/requests-client-adapter',
     packages=find_packages(),
     install_requires=[
         'apimatic-core-interfaces~=0.1.0',
         'requests~=2.25',
         'cachecontrol~=0.12.6'
     ],
     tests_require=[
-        'pytest~=7.1.3',
-        'pytest-cov~=3.0.0'
+        'pytest~=7.2.2',
+        'pytest-cov~=4.0.0'
     ]
 )
```

### Comparing `apimatic-requests-client-adapter-0.1.2/tests/apimatic_requests_client_adapter/base.py` & `apimatic-requests-client-adapter-0.1.3/tests/apimatic_requests_client_adapter/base.py`

 * *Files identical despite different names*

### Comparing `apimatic-requests-client-adapter-0.1.2/tests/apimatic_requests_client_adapter/models/internal/http_request.py` & `apimatic-requests-client-adapter-0.1.3/tests/apimatic_requests_client_adapter/models/internal/http_request.py`

 * *Files identical despite different names*

### Comparing `apimatic-requests-client-adapter-0.1.2/tests/apimatic_requests_client_adapter/models/internal/http_response.py` & `apimatic-requests-client-adapter-0.1.3/tests/apimatic_requests_client_adapter/models/internal/http_response.py`

 * *Files identical despite different names*

### Comparing `apimatic-requests-client-adapter-0.1.2/tests/apimatic_requests_client_adapter/requests_client_tests/test_requests_client.py` & `apimatic-requests-client-adapter-0.1.3/tests/apimatic_requests_client_adapter/requests_client_tests/test_requests_client.py`

 * *Files identical despite different names*

