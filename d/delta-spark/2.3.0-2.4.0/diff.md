# Comparing `tmp/delta-spark-2.3.0.tar.gz` & `tmp/delta-spark-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/delta-spark-2.3.0.tar", last modified: Tue Apr  4 20:26:05 2023, max compression
+gzip compressed data, was "dist/delta-spark-2.4.0.tar", last modified: Thu May 25 20:48:39 2023, max compression
```

## Comparing `delta-spark-2.3.0.tar` & `delta-spark-2.4.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 allison.portis  (1000) ubuntu    (1000)        0 2023-04-04 20:26:05.000000 delta-spark-2.3.0/
--rw-r--r--   0 allison.portis  (1000) ubuntu    (1000)     2141 2023-04-04 17:52:04.000000 delta-spark-2.3.0/setup.py
--rw-r--r--   0 allison.portis  (1000) ubuntu    (1000)     9907 2023-04-04 17:52:04.000000 delta-spark-2.3.0/README.md
--rw-r--r--   0 allison.portis  (1000) ubuntu    (1000)     1944 2023-04-04 20:26:05.000000 delta-spark-2.3.0/PKG-INFO
-drwxr-xr-x   0 allison.portis  (1000) ubuntu    (1000)        0 2023-04-04 20:26:05.000000 delta-spark-2.3.0/python/
-drwxr-xr-x   0 allison.portis  (1000) ubuntu    (1000)        0 2023-04-04 20:26:05.000000 delta-spark-2.3.0/python/delta/
--rw-r--r--   0 allison.portis  (1000) ubuntu    (1000)        0 2023-04-04 17:52:04.000000 delta-spark-2.3.0/python/delta/py.typed
--rw-r--r--   0 allison.portis  (1000) ubuntu    (1000)      753 2023-04-04 17:52:04.000000 delta-spark-2.3.0/python/delta/__init__.py
--rw-r--r--   0 allison.portis  (1000) ubuntu    (1000)      870 2023-04-04 17:52:04.000000 delta-spark-2.3.0/python/delta/_typing.py
--rw-r--r--   0 allison.portis  (1000) ubuntu    (1000)     5149 2023-04-04 17:52:04.000000 delta-spark-2.3.0/python/delta/exceptions.py
--rw-r--r--   0 allison.portis  (1000) ubuntu    (1000)    54376 2023-04-04 17:52:04.000000 delta-spark-2.3.0/python/delta/tables.py
--rw-r--r--   0 allison.portis  (1000) ubuntu    (1000)     3254 2023-04-04 17:52:04.000000 delta-spark-2.3.0/python/delta/pip_utils.py
-drwxr-xr-x   0 allison.portis  (1000) ubuntu    (1000)        0 2023-04-04 20:26:05.000000 delta-spark-2.3.0/python/delta_spark.egg-info/
--rw-r--r--   0 allison.portis  (1000) ubuntu    (1000)        6 2023-04-04 20:26:05.000000 delta-spark-2.3.0/python/delta_spark.egg-info/top_level.txt
--rw-r--r--   0 allison.portis  (1000) ubuntu    (1000)      374 2023-04-04 20:26:05.000000 delta-spark-2.3.0/python/delta_spark.egg-info/SOURCES.txt
--rw-r--r--   0 allison.portis  (1000) ubuntu    (1000)     1944 2023-04-04 20:26:05.000000 delta-spark-2.3.0/python/delta_spark.egg-info/PKG-INFO
--rw-r--r--   0 allison.portis  (1000) ubuntu    (1000)        1 2023-04-04 20:26:05.000000 delta-spark-2.3.0/python/delta_spark.egg-info/dependency_links.txt
--rw-r--r--   0 allison.portis  (1000) ubuntu    (1000)       48 2023-04-04 20:26:05.000000 delta-spark-2.3.0/python/delta_spark.egg-info/requires.txt
--rw-r--r--   0 allison.portis  (1000) ubuntu    (1000)       38 2023-04-04 20:26:05.000000 delta-spark-2.3.0/setup.cfg
+drwxr-xr-x   0 allison.portis  (1000) ubuntu    (1000)        0 2023-05-25 20:48:39.000000 delta-spark-2.4.0/
+-rw-r--r--   0 allison.portis  (1000) ubuntu    (1000)     2142 2023-05-24 17:51:45.000000 delta-spark-2.4.0/setup.py
+-rw-r--r--   0 allison.portis  (1000) ubuntu    (1000)    10017 2023-05-24 17:51:45.000000 delta-spark-2.4.0/README.md
+-rw-r--r--   0 allison.portis  (1000) ubuntu    (1000)     1944 2023-05-25 20:48:39.000000 delta-spark-2.4.0/PKG-INFO
+drwxr-xr-x   0 allison.portis  (1000) ubuntu    (1000)        0 2023-05-25 20:48:39.000000 delta-spark-2.4.0/python/
+drwxr-xr-x   0 allison.portis  (1000) ubuntu    (1000)        0 2023-05-25 20:48:39.000000 delta-spark-2.4.0/python/delta/
+-rw-r--r--   0 allison.portis  (1000) ubuntu    (1000)        0 2023-05-24 17:51:45.000000 delta-spark-2.4.0/python/delta/py.typed
+-rw-r--r--   0 allison.portis  (1000) ubuntu    (1000)      753 2023-05-24 17:51:45.000000 delta-spark-2.4.0/python/delta/__init__.py
+-rw-r--r--   0 allison.portis  (1000) ubuntu    (1000)      870 2023-05-24 17:51:45.000000 delta-spark-2.4.0/python/delta/_typing.py
+-rw-r--r--   0 allison.portis  (1000) ubuntu    (1000)     5214 2023-05-24 17:51:45.000000 delta-spark-2.4.0/python/delta/exceptions.py
+-rw-r--r--   0 allison.portis  (1000) ubuntu    (1000)    54376 2023-05-24 17:51:45.000000 delta-spark-2.4.0/python/delta/tables.py
+-rw-r--r--   0 allison.portis  (1000) ubuntu    (1000)     3254 2023-05-24 17:51:45.000000 delta-spark-2.4.0/python/delta/pip_utils.py
+drwxr-xr-x   0 allison.portis  (1000) ubuntu    (1000)        0 2023-05-25 20:48:39.000000 delta-spark-2.4.0/python/delta_spark.egg-info/
+-rw-r--r--   0 allison.portis  (1000) ubuntu    (1000)        6 2023-05-25 20:48:39.000000 delta-spark-2.4.0/python/delta_spark.egg-info/top_level.txt
+-rw-r--r--   0 allison.portis  (1000) ubuntu    (1000)      374 2023-05-25 20:48:39.000000 delta-spark-2.4.0/python/delta_spark.egg-info/SOURCES.txt
+-rw-r--r--   0 allison.portis  (1000) ubuntu    (1000)     1944 2023-05-25 20:48:39.000000 delta-spark-2.4.0/python/delta_spark.egg-info/PKG-INFO
+-rw-r--r--   0 allison.portis  (1000) ubuntu    (1000)        1 2023-05-25 20:48:39.000000 delta-spark-2.4.0/python/delta_spark.egg-info/dependency_links.txt
+-rw-r--r--   0 allison.portis  (1000) ubuntu    (1000)       48 2023-05-25 20:48:39.000000 delta-spark-2.4.0/python/delta_spark.egg-info/requires.txt
+-rw-r--r--   0 allison.portis  (1000) ubuntu    (1000)       38 2023-05-25 20:48:39.000000 delta-spark-2.4.0/setup.cfg
```

### Comparing `delta-spark-2.3.0/setup.py` & `delta-spark-2.4.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/usr/bin/env python
+#!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 import os
 import sys
 
 from setuptools import setup
 from setuptools.command.install import install
 
@@ -61,15 +61,15 @@
     keywords='delta.io',
     package_dir={'': 'python'},
     packages=['delta'],
     package_data={
         'delta': ['py.typed'],
     },
     install_requires=[
-        'pyspark>=3.3.0,<3.4.0',
+        'pyspark>=3.4.0,<3.5.0',
         'importlib_metadata>=1.0.0',
     ],
     python_requires='>=3.6',
     cmdclass={
         'verify': VerifyVersionCommand,
     }
 )
```

### Comparing `delta-spark-2.3.0/README.md` & `delta-spark-2.4.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 <img src="https://docs.delta.io/latest/_static/delta-lake-white.png" width="200" alt="Delta Lake Logo"></img>
 
 [![Test](https://github.com/delta-io/delta/actions/workflows/test.yaml/badge.svg)](https://github.com/delta-io/delta/actions/workflows/test.yaml)
 [![License](https://img.shields.io/badge/license-Apache%202-brightgreen.svg)](https://github.com/delta-io/delta/blob/master/LICENSE.txt)
 [![PyPI](https://img.shields.io/pypi/v/delta-spark.svg)](https://pypi.org/project/delta-spark/)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/delta-spark)](https://pypistats.org/packages/delta-spark)
 
 Delta Lake is an open-source storage framework that enables building a [Lakehouse architecture](http://cidrdb.org/cidr2021/papers/cidr2021_paper17.pdf) with compute engines including Spark, PrestoDB, Flink, Trino, and Hive and APIs for Scala, Java, Rust, Ruby, and Python. 
 * See the [Delta Lake Documentation](https://docs.delta.io) for details.
 * See the [Quick Start Guide](https://docs.delta.io/latest/quick-start.html) to get started with Scala, Java and Python.
 * Note, this repo is one of many Delta Lake repositories in the [delta.io](https://github.com/delta-io) organizations including 
 [connectors](https://github.com/delta-io/connectors),
 [delta](https://github.com/delta-io/delta),
```

### Comparing `delta-spark-2.3.0/PKG-INFO` & `delta-spark-2.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: delta-spark
-Version: 2.3.0
+Version: 2.4.0
 Summary: Python APIs for using Delta Lake with Apache Spark
 Home-page: https://github.com/delta-io/delta/
 Author: The Delta Lake Project Authors
 Author-email: delta-users@googlegroups.com
 License: Apache-2.0
-Project-URL: Source, https://github.com/delta-io/delta
 Project-URL: Issues, https://github.com/delta-io/delta/issues
 Project-URL: Documentation, https://docs.delta.io/latest/index.html
+Project-URL: Source, https://github.com/delta-io/delta
 Description: # Delta Lake
         
         [Delta Lake](https://delta.io) is an open source storage layer that brings reliability to data lakes. Delta Lake provides ACID transactions, scalable metadata handling, and unifies streaming and batch data processing. Delta Lake runs on top of your existing data lake and is fully compatible with Apache Spark APIs.
         
         This PyPi package contains the Python APIs for using Delta Lake with Apache Spark.
         
         ## Installation and usage
```

### Comparing `delta-spark-2.3.0/python/delta/__init__.py` & `delta-spark-2.4.0/python/delta/__init__.py`

 * *Files identical despite different names*

### Comparing `delta-spark-2.3.0/python/delta/_typing.py` & `delta-spark-2.4.0/python/delta/_typing.py`

 * *Files identical despite different names*

### Comparing `delta-spark-2.3.0/python/delta/exceptions.py` & `delta-spark-2.4.0/python/delta/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,18 +13,18 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 from typing import TYPE_CHECKING, Optional
 
 from pyspark import SparkContext
-from pyspark.sql import utils
+from pyspark.errors.exceptions import captured
+from pyspark.errors.exceptions.captured import CapturedException
 from pyspark.sql.utils import (
     AnalysisException,
-    CapturedException,
     IllegalArgumentException,
     ParseException
 )
 from py4j.java_gateway import is_instance_of  # type: ignore[import]
 
 if TYPE_CHECKING:
     from py4j.java_gateway import JavaObject, JVMView  # type: ignore[import]
@@ -147,21 +147,21 @@
 
 
 def _patch_convert_exception() -> None:
     """
     Patch PySpark's exception convert method to convert Delta's Scala concurrent exceptions to the
     corresponding Python exceptions.
     """
-    original_convert_sql_exception = utils.convert_exception
+    original_convert_sql_exception = captured.convert_exception
 
     def convert_delta_exception(e: "JavaObject") -> CapturedException:
         delta_exception = _convert_delta_exception(e)
         if delta_exception is not None:
             return delta_exception
         return original_convert_sql_exception(e)
 
-    utils.convert_exception = convert_delta_exception
+    captured.convert_exception = convert_delta_exception
 
 
 if not _delta_exception_patched:
     _patch_convert_exception()
     _delta_exception_patched = True
```

### Comparing `delta-spark-2.3.0/python/delta/tables.py` & `delta-spark-2.4.0/python/delta/tables.py`

 * *Files identical despite different names*

### Comparing `delta-spark-2.3.0/python/delta/pip_utils.py` & `delta-spark-2.4.0/python/delta/pip_utils.py`

 * *Files identical despite different names*

### Comparing `delta-spark-2.3.0/python/delta_spark.egg-info/PKG-INFO` & `delta-spark-2.4.0/python/delta_spark.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: delta-spark
-Version: 2.3.0
+Version: 2.4.0
 Summary: Python APIs for using Delta Lake with Apache Spark
 Home-page: https://github.com/delta-io/delta/
 Author: The Delta Lake Project Authors
 Author-email: delta-users@googlegroups.com
 License: Apache-2.0
-Project-URL: Source, https://github.com/delta-io/delta
 Project-URL: Issues, https://github.com/delta-io/delta/issues
 Project-URL: Documentation, https://docs.delta.io/latest/index.html
+Project-URL: Source, https://github.com/delta-io/delta
 Description: # Delta Lake
         
         [Delta Lake](https://delta.io) is an open source storage layer that brings reliability to data lakes. Delta Lake provides ACID transactions, scalable metadata handling, and unifies streaming and batch data processing. Delta Lake runs on top of your existing data lake and is fully compatible with Apache Spark APIs.
         
         This PyPi package contains the Python APIs for using Delta Lake with Apache Spark.
         
         ## Installation and usage
```

