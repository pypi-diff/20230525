# Comparing `tmp/dagster-prometheus-0.9.9rc1.tar.gz` & `tmp/dagster-prometheus-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dagster-prometheus-0.9.9rc1.tar", last modified: Thu Sep 17 21:08:59 2020, max compression
+gzip compressed data, was "dagster-prometheus-1.0.5.tar", last modified: Fri Aug 26 13:46:37 2022, max compression
```

## Comparing `dagster-prometheus-0.9.9rc1.tar` & `dagster-prometheus-1.0.5.tar`

### file list

```diff
@@ -1,22 +1,19 @@
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:59.000000 dagster-prometheus-0.9.9rc1/
--rw-r--r--   0 bobchen    (501) staff       (20)    11357 2020-09-17 21:04:59.000000 dagster-prometheus-0.9.9rc1/LICENSE
--rw-r--r--   0 bobchen    (501) staff       (20)       34 2020-09-17 21:04:59.000000 dagster-prometheus-0.9.9rc1/MANIFEST.in
--rw-r--r--   0 bobchen    (501) staff       (20)      585 2020-09-17 21:08:59.000000 dagster-prometheus-0.9.9rc1/PKG-INFO
--rw-r--r--   0 bobchen    (501) staff       (20)      140 2020-09-17 21:04:59.000000 dagster-prometheus-0.9.9rc1/README.md
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:59.000000 dagster-prometheus-0.9.9rc1/dagster_prometheus/
--rw-r--r--   0 bobchen    (501) staff       (20)      239 2020-09-17 21:04:59.000000 dagster-prometheus-0.9.9rc1/dagster_prometheus/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)     5524 2020-09-17 21:04:59.000000 dagster-prometheus-0.9.9rc1/dagster_prometheus/resources.py
--rw-r--r--   0 bobchen    (501) staff       (20)       27 2020-09-17 21:04:59.000000 dagster-prometheus-0.9.9rc1/dagster_prometheus/version.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:59.000000 dagster-prometheus-0.9.9rc1/dagster_prometheus.egg-info/
--rw-r--r--   0 bobchen    (501) staff       (20)      585 2020-09-17 21:08:59.000000 dagster-prometheus-0.9.9rc1/dagster_prometheus.egg-info/PKG-INFO
--rw-r--r--   0 bobchen    (501) staff       (20)      502 2020-09-17 21:08:59.000000 dagster-prometheus-0.9.9rc1/dagster_prometheus.egg-info/SOURCES.txt
--rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:08:59.000000 dagster-prometheus-0.9.9rc1/dagster_prometheus.egg-info/dependency_links.txt
--rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:08:59.000000 dagster-prometheus-0.9.9rc1/dagster_prometheus.egg-info/not-zip-safe
--rw-r--r--   0 bobchen    (501) staff       (20)       26 2020-09-17 21:08:59.000000 dagster-prometheus-0.9.9rc1/dagster_prometheus.egg-info/requires.txt
--rw-r--r--   0 bobchen    (501) staff       (20)       44 2020-09-17 21:08:59.000000 dagster-prometheus-0.9.9rc1/dagster_prometheus.egg-info/top_level.txt
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:59.000000 dagster-prometheus-0.9.9rc1/dagster_prometheus_tests/
--rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:04:59.000000 dagster-prometheus-0.9.9rc1/dagster_prometheus_tests/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)     4529 2020-09-17 21:04:59.000000 dagster-prometheus-0.9.9rc1/dagster_prometheus_tests/test_resources.py
--rw-r--r--   0 bobchen    (501) staff       (20)       96 2020-09-17 21:04:59.000000 dagster-prometheus-0.9.9rc1/dagster_prometheus_tests/test_version.py
--rw-r--r--   0 bobchen    (501) staff       (20)       38 2020-09-17 21:08:59.000000 dagster-prometheus-0.9.9rc1/setup.cfg
--rw-r--r--   0 bobchen    (501) staff       (20)     1051 2020-09-17 21:04:59.000000 dagster-prometheus-0.9.9rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:46:37.168837 dagster-prometheus-1.0.5/
+-rw-r--r--   0 root         (0) root         (0)    11357 2022-08-26 13:33:01.000000 dagster-prometheus-1.0.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       70 2022-08-26 13:33:01.000000 dagster-prometheus-1.0.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      644 2022-08-26 13:46:37.168837 dagster-prometheus-1.0.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      140 2022-08-26 13:33:01.000000 dagster-prometheus-1.0.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:46:37.168837 dagster-prometheus-1.0.5/dagster_prometheus/
+-rw-r--r--   0 root         (0) root         (0)      240 2022-08-26 13:33:01.000000 dagster-prometheus-1.0.5/dagster_prometheus/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        8 2022-08-26 13:33:01.000000 dagster-prometheus-1.0.5/dagster_prometheus/py.typed
+-rw-r--r--   0 root         (0) root         (0)     5559 2022-08-26 13:33:01.000000 dagster-prometheus-1.0.5/dagster_prometheus/resources.py
+-rw-r--r--   0 root         (0) root         (0)       22 2022-08-26 13:33:01.000000 dagster-prometheus-1.0.5/dagster_prometheus/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:46:37.168837 dagster-prometheus-1.0.5/dagster_prometheus.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      644 2022-08-26 13:46:37.000000 dagster-prometheus-1.0.5/dagster_prometheus.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      419 2022-08-26 13:46:37.000000 dagster-prometheus-1.0.5/dagster_prometheus.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-08-26 13:46:37.000000 dagster-prometheus-1.0.5/dagster_prometheus.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-08-26 13:46:37.000000 dagster-prometheus-1.0.5/dagster_prometheus.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       33 2022-08-26 13:46:37.000000 dagster-prometheus-1.0.5/dagster_prometheus.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2022-08-26 13:46:37.000000 dagster-prometheus-1.0.5/dagster_prometheus.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      129 2022-08-26 13:46:37.172837 dagster-prometheus-1.0.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1320 2022-08-26 13:33:01.000000 dagster-prometheus-1.0.5/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `dagster-prometheus-0.9.9rc1/LICENSE` & `dagster-prometheus-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-prometheus-0.9.9rc1/PKG-INFO` & `dagster-prometheus-1.0.5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,19 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: dagster-prometheus
-Version: 0.9.9rc1
+Version: 1.0.5
 Summary: A Dagster integration for prometheus
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-prometheus
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
-Description: UNKNOWN
 Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
+License-File: LICENSE
+
+UNKNOWN
+
```

### Comparing `dagster-prometheus-0.9.9rc1/dagster_prometheus/resources.py` & `dagster-prometheus-1.0.5/dagster_prometheus/resources.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import prometheus_client
 from prometheus_client.exposition import default_handler
 
-from dagster import Field, check, resource
+from dagster import Field
+from dagster import _check as check
+from dagster import resource
 
 
-class PrometheusResource(object):
-    """Integrates with Prometheus via the prometheus_client library.
-    """
+class PrometheusResource:
+    """Integrates with Prometheus via the prometheus_client library."""
 
     def __init__(self, gateway, timeout):
         self.gateway = check.str_param(gateway, "gateway")
         self.timeout = check.opt_int_param(timeout, "timeout")
         self.registry = prometheus_client.CollectorRegistry()
 
     def push_to_gateway(self, job, grouping_key=None, handler=default_handler):
```

### Comparing `dagster-prometheus-0.9.9rc1/dagster_prometheus.egg-info/PKG-INFO` & `dagster-prometheus-1.0.5/dagster_prometheus.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,19 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: dagster-prometheus
-Version: 0.9.9rc1
+Version: 1.0.5
 Summary: A Dagster integration for prometheus
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-prometheus
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
-Description: UNKNOWN
 Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
+License-File: LICENSE
+
+UNKNOWN
+
```

### Comparing `dagster-prometheus-0.9.9rc1/setup.py` & `dagster-prometheus-1.0.5/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,37 @@
+from typing import Dict
+
 from setuptools import find_packages, setup
 
 
-def get_version():
-    version = {}
-    with open("dagster_prometheus/version.py") as fp:
+def get_version() -> str:
+    version: Dict[str, str] = {}
+    with open("dagster_prometheus/version.py", encoding="utf8") as fp:
         exec(fp.read(), version)  # pylint: disable=W0122
 
     return version["__version__"]
 
 
 if __name__ == "__main__":
+    ver = get_version()
+    # dont pin dev installs to avoid pip dep resolver issues
+    pin = "" if ver == "0+dev" else f"=={ver}"
     setup(
         name="dagster-prometheus",
-        version=get_version(),
+        version=ver,
         author="Elementl",
         author_email="hello@elementl.com",
         license="Apache-2.0",
         description="A Dagster integration for prometheus",
         url="https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-prometheus",
         classifiers=[
-            "Programming Language :: Python :: 2.7",
-            "Programming Language :: Python :: 3.6",
             "Programming Language :: Python :: 3.7",
+            "Programming Language :: Python :: 3.8",
+            "Programming Language :: Python :: 3.9",
+            "Programming Language :: Python :: 3.10",
             "License :: OSI Approved :: Apache Software License",
             "Operating System :: OS Independent",
         ],
-        packages=find_packages(exclude=["test"]),
-        install_requires=["dagster", "prometheus_client"],
+        packages=find_packages(exclude=["dagster_prometheus_tests*"]),
+        install_requires=["dagster==1.0.5", "prometheus_client"],
         zip_safe=False,
     )
```

