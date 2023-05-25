# Comparing `tmp/influxql_client-0.0.1.tar.gz` & `tmp/influxql_client-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "influxql_client-0.0.1.tar", last modified: Fri May 12 16:20:50 2023, max compression
+gzip compressed data, was "influxql_client-0.0.2.tar", last modified: Thu May 25 14:57:58 2023, max compression
```

## Comparing `influxql_client-0.0.1.tar` & `influxql_client-0.0.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:20:50.787895 influxql_client-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-12 16:20:37.000000 influxql_client-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-12 16:20:50.787895 influxql_client-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-12 16:20:37.000000 influxql_client-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:20:50.783895 influxql_client-0.0.1/influxdb_influxql_client/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-12 16:20:37.000000 influxql_client-0.0.1/influxdb_influxql_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:20:50.783895 influxql_client-0.0.1/influxdb_influxql_client/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 16:20:37.000000 influxql_client-0.0.1/influxdb_influxql_client/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-12 16:20:37.000000 influxql_client-0.0.1/influxdb_influxql_client/client/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-12 16:20:37.000000 influxql_client-0.0.1/influxdb_influxql_client/client/influxdb_influxql_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:20:50.787895 influxql_client-0.0.1/influxdb_influxql_client/client/models/
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-12 16:20:37.000000 influxql_client-0.0.1/influxdb_influxql_client/client/models/Results.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 16:20:37.000000 influxql_client-0.0.1/influxdb_influxql_client/client/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-12 16:20:37.000000 influxql_client-0.0.1/influxdb_influxql_client/client/query_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:20:50.787895 influxql_client-0.0.1/influxdb_influxql_client/client/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 16:20:37.000000 influxql_client-0.0.1/influxdb_influxql_client/client/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-12 16:20:37.000000 influxql_client-0.0.1/influxdb_influxql_client/client/util/request_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:20:50.787895 influxql_client-0.0.1/influxql_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-12 16:20:50.000000 influxql_client-0.0.1/influxql_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-05-12 16:20:50.000000 influxql_client-0.0.1/influxql_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 16:20:50.000000 influxql_client-0.0.1/influxql_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-12 16:20:50.000000 influxql_client-0.0.1/influxql_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-12 16:20:50.000000 influxql_client-0.0.1/influxql_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 16:20:50.787895 influxql_client-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-12 16:20:37.000000 influxql_client-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:20:50.787895 influxql_client-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-05-12 16:20:37.000000 influxql_client-0.0.1/tests/test_basic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:57:58.981175 influxql_client-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-25 14:57:48.000000 influxql_client-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-05-25 14:57:58.981175 influxql_client-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-25 14:57:48.000000 influxql_client-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:57:58.981175 influxql_client-0.0.2/influxdb_influxql_client/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-25 14:57:48.000000 influxql_client-0.0.2/influxdb_influxql_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:57:58.981175 influxql_client-0.0.2/influxdb_influxql_client/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:57:48.000000 influxql_client-0.0.2/influxdb_influxql_client/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-25 14:57:48.000000 influxql_client-0.0.2/influxdb_influxql_client/client/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-25 14:57:48.000000 influxql_client-0.0.2/influxdb_influxql_client/client/influxdb_influxql_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:57:58.981175 influxql_client-0.0.2/influxdb_influxql_client/client/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-25 14:57:48.000000 influxql_client-0.0.2/influxdb_influxql_client/client/models/Results.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:57:48.000000 influxql_client-0.0.2/influxdb_influxql_client/client/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-25 14:57:48.000000 influxql_client-0.0.2/influxdb_influxql_client/client/query_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:57:58.981175 influxql_client-0.0.2/influxdb_influxql_client/client/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:57:48.000000 influxql_client-0.0.2/influxdb_influxql_client/client/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-25 14:57:48.000000 influxql_client-0.0.2/influxdb_influxql_client/client/util/request_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:57:58.981175 influxql_client-0.0.2/influxql_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-05-25 14:57:58.000000 influxql_client-0.0.2/influxql_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-05-25 14:57:58.000000 influxql_client-0.0.2/influxql_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 14:57:58.000000 influxql_client-0.0.2/influxql_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-25 14:57:58.000000 influxql_client-0.0.2/influxql_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-25 14:57:58.000000 influxql_client-0.0.2/influxql_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 14:57:58.981175 influxql_client-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-25 14:57:48.000000 influxql_client-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:57:58.981175 influxql_client-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-05-25 14:57:48.000000 influxql_client-0.0.2/tests/test_basic.py
```

### Comparing `influxql_client-0.0.1/LICENSE` & `influxql_client-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `influxql_client-0.0.1/PKG-INFO` & `influxql_client-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: influxql_client
-Version: 0.0.1
+Version: 0.0.2
 Summary: InfluxDB InfluxQL Basic Library
+Home-page: https://github.com/delrey1/influxdb-influxql-client
 Keywords: InfluxDB,InfluxDB Python Client,InfluxQL
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `influxql_client-0.0.1/README.md` & `influxql_client-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `influxql_client-0.0.1/influxdb_influxql_client/client/query_api.py` & `influxql_client-0.0.2/influxdb_influxql_client/client/query_api.py`

 * *Files identical despite different names*

### Comparing `influxql_client-0.0.1/influxql_client.egg-info/PKG-INFO` & `influxql_client-0.0.2/influxql_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: influxql-client
-Version: 0.0.1
+Version: 0.0.2
 Summary: InfluxDB InfluxQL Basic Library
+Home-page: https://github.com/delrey1/influxdb-influxql-client
 Keywords: InfluxDB,InfluxDB Python Client,InfluxQL
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `influxql_client-0.0.1/influxql_client.egg-info/SOURCES.txt` & `influxql_client-0.0.2/influxql_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `influxql_client-0.0.1/setup.py` & `influxql_client-0.0.2/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -8,24 +8,25 @@
 
 readme = open('README.md').read()
 
 NAME = "influxql_client"
 
 setup(
     name=NAME,
-    version='0.0.1',
+    version='0.0.2',
     description="InfluxDB InfluxQL Basic Library",
     keywords=["InfluxDB", "InfluxDB Python Client", "InfluxQL"],
     long_description=readme,
     long_description_content_type="text/markdown",
     install_requires=requires,
     packages=find_packages(exclude=('tests*',)),
     test_suite='tests',
     python_requires='>=3.7',
     include_package_data=True,
+    url="https://github.com/delrey1/influxdb-influxql-client",
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Libraries',
         'Topic :: Software Development :: Libraries :: Python Modules',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
```

### Comparing `influxql_client-0.0.1/tests/test_basic.py` & `influxql_client-0.0.2/tests/test_basic.py`

 * *Files identical despite different names*

