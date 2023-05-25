# Comparing `tmp/dagster-datadog-0.9.9rc1.tar.gz` & `tmp/dagster-datadog-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dagster-datadog-0.9.9rc1.tar", last modified: Thu Sep 17 21:08:35 2020, max compression
+gzip compressed data, was "dagster-datadog-1.0.5.tar", last modified: Fri Aug 26 13:46:12 2022, max compression
```

## Comparing `dagster-datadog-0.9.9rc1.tar` & `dagster-datadog-1.0.5.tar`

### file list

```diff
@@ -1,22 +1,19 @@
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:35.000000 dagster-datadog-0.9.9rc1/
--rw-r--r--   0 bobchen    (501) staff       (20)    11357 2020-09-17 21:04:59.000000 dagster-datadog-0.9.9rc1/LICENSE
--rw-r--r--   0 bobchen    (501) staff       (20)       34 2020-09-17 21:04:59.000000 dagster-datadog-0.9.9rc1/MANIFEST.in
--rw-r--r--   0 bobchen    (501) staff       (20)      592 2020-09-17 21:08:35.000000 dagster-datadog-0.9.9rc1/PKG-INFO
--rw-r--r--   0 bobchen    (501) staff       (20)      131 2020-09-17 21:04:59.000000 dagster-datadog-0.9.9rc1/README.md
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:35.000000 dagster-datadog-0.9.9rc1/dagster_datadog/
--rw-r--r--   0 bobchen    (501) staff       (20)      230 2020-09-17 21:04:59.000000 dagster-datadog-0.9.9rc1/dagster_datadog/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)     2800 2020-09-17 21:04:59.000000 dagster-datadog-0.9.9rc1/dagster_datadog/resources.py
--rw-r--r--   0 bobchen    (501) staff       (20)       27 2020-09-17 21:04:59.000000 dagster-datadog-0.9.9rc1/dagster_datadog/version.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:35.000000 dagster-datadog-0.9.9rc1/dagster_datadog.egg-info/
--rw-r--r--   0 bobchen    (501) staff       (20)      592 2020-09-17 21:08:35.000000 dagster-datadog-0.9.9rc1/dagster_datadog.egg-info/PKG-INFO
--rw-r--r--   0 bobchen    (501) staff       (20)      476 2020-09-17 21:08:35.000000 dagster-datadog-0.9.9rc1/dagster_datadog.egg-info/SOURCES.txt
--rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:08:35.000000 dagster-datadog-0.9.9rc1/dagster_datadog.egg-info/dependency_links.txt
--rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:08:35.000000 dagster-datadog-0.9.9rc1/dagster_datadog.egg-info/not-zip-safe
--rw-r--r--   0 bobchen    (501) staff       (20)       16 2020-09-17 21:08:35.000000 dagster-datadog-0.9.9rc1/dagster_datadog.egg-info/requires.txt
--rw-r--r--   0 bobchen    (501) staff       (20)       38 2020-09-17 21:08:35.000000 dagster-datadog-0.9.9rc1/dagster_datadog.egg-info/top_level.txt
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:35.000000 dagster-datadog-0.9.9rc1/dagster_datadog_tests/
--rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:04:59.000000 dagster-datadog-0.9.9rc1/dagster_datadog_tests/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)     2741 2020-09-17 21:04:59.000000 dagster-datadog-0.9.9rc1/dagster_datadog_tests/test_resources.py
--rw-r--r--   0 bobchen    (501) staff       (20)       93 2020-09-17 21:04:59.000000 dagster-datadog-0.9.9rc1/dagster_datadog_tests/test_version.py
--rw-r--r--   0 bobchen    (501) staff       (20)       74 2020-09-17 21:08:35.000000 dagster-datadog-0.9.9rc1/setup.cfg
--rw-r--r--   0 bobchen    (501) staff       (20)     1045 2020-09-17 21:04:59.000000 dagster-datadog-0.9.9rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:46:12.764704 dagster-datadog-1.0.5/
+-rw-r--r--   0 root         (0) root         (0)    11357 2022-08-26 13:33:01.000000 dagster-datadog-1.0.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       67 2022-08-26 13:33:01.000000 dagster-datadog-1.0.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      651 2022-08-26 13:46:12.764704 dagster-datadog-1.0.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      131 2022-08-26 13:33:01.000000 dagster-datadog-1.0.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:46:12.760704 dagster-datadog-1.0.5/dagster_datadog/
+-rw-r--r--   0 root         (0) root         (0)      231 2022-08-26 13:33:01.000000 dagster-datadog-1.0.5/dagster_datadog/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        8 2022-08-26 13:33:01.000000 dagster-datadog-1.0.5/dagster_datadog/py.typed
+-rw-r--r--   0 root         (0) root         (0)     2743 2022-08-26 13:33:01.000000 dagster-datadog-1.0.5/dagster_datadog/resources.py
+-rw-r--r--   0 root         (0) root         (0)       22 2022-08-26 13:33:01.000000 dagster-datadog-1.0.5/dagster_datadog/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:46:12.764704 dagster-datadog-1.0.5/dagster_datadog.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      651 2022-08-26 13:46:12.000000 dagster-datadog-1.0.5/dagster_datadog.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      389 2022-08-26 13:46:12.000000 dagster-datadog-1.0.5/dagster_datadog.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-08-26 13:46:12.000000 dagster-datadog-1.0.5/dagster_datadog.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-08-26 13:46:12.000000 dagster-datadog-1.0.5/dagster_datadog.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       23 2022-08-26 13:46:12.000000 dagster-datadog-1.0.5/dagster_datadog.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2022-08-26 13:46:12.000000 dagster-datadog-1.0.5/dagster_datadog.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      162 2022-08-26 13:46:12.764704 dagster-datadog-1.0.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1311 2022-08-26 13:33:01.000000 dagster-datadog-1.0.5/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `dagster-datadog-0.9.9rc1/LICENSE` & `dagster-datadog-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-datadog-0.9.9rc1/PKG-INFO` & `dagster-datadog-1.0.5/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,19 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: dagster-datadog
-Version: 0.9.9rc1
+Version: 1.0.5
 Summary: Package for datadog Dagster framework components.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-datadog
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

### Comparing `dagster-datadog-0.9.9rc1/dagster_datadog/resources.py` & `dagster-datadog-1.0.5/dagster_datadog/resources.py`

 * *Files 8% similar despite different names*

```diff
@@ -46,16 +46,16 @@
     `DataDog documentation <https://docs.datadoghq.com/developers/dogstatsd/>`_ for how to use this
     resource.
 
     Examples:
 
         .. code-block:: python
 
-            @solid(required_resource_keys={'datadog'})
-            def datadog_solid(context):
+            @op(required_resource_keys={'datadog'})
+            def datadog_op(context):
                 dd = context.resources.datadog
 
                 dd.event('Man down!', 'This server needs assistance.')
                 dd.gauge('users.online', 1001, tags=["protocol:http"])
                 dd.increment('page.views')
                 dd.decrement('page.views')
                 dd.histogram('album.photo.count', 26, tags=["gender:female"])
@@ -67,20 +67,19 @@
                 # Use timed decorator
                 @dd.timed('run_fn')
                 def run_fn():
                     pass
 
                 run_fn()
 
-            @pipeline(mode_defs=[ModeDefinition(resource_defs={'datadog': datadog_resource})])
-            def dd_pipeline():
-                datadog_solid()
-
-            result = execute_pipeline(
-                dd_pipeline,
-                {'resources': {'datadog': {'config': {'api_key': 'YOUR_KEY', 'app_key': 'YOUR_KEY'}}}},
+            @job(resource_defs={'datadog': datadog_resource})
+            def dd_job():
+                datadog_op()
+
+            result = dd_job.execute_in_process(
+                run_config={'resources': {'datadog': {'config': {'api_key': 'YOUR_KEY', 'app_key': 'YOUR_KEY'}}}}
             )
 
     """
     return DataDogResource(
         context.resource_config.get("api_key"), context.resource_config.get("app_key")
     )
```

### Comparing `dagster-datadog-0.9.9rc1/dagster_datadog.egg-info/PKG-INFO` & `dagster-datadog-1.0.5/dagster_datadog.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,19 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: dagster-datadog
-Version: 0.9.9rc1
+Version: 1.0.5
 Summary: Package for datadog Dagster framework components.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-datadog
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

### Comparing `dagster-datadog-0.9.9rc1/setup.py` & `dagster-datadog-1.0.5/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,37 @@
+from typing import Dict
+
 from setuptools import find_packages, setup
 
 
-def get_version():
-    version = {}
-    with open("dagster_datadog/version.py") as fp:
+def get_version() -> str:
+    version: Dict[str, str] = {}
+    with open("dagster_datadog/version.py", encoding="utf8") as fp:
         exec(fp.read(), version)  # pylint: disable=W0122
 
     return version["__version__"]
 
 
 if __name__ == "__main__":
+    ver = get_version()
+    # dont pin dev installs to avoid pip dep resolver issues
+    pin = "" if ver == "0+dev" else f"=={ver}"
     setup(
         name="dagster-datadog",
-        version=get_version(),
+        version=ver,
         author="Elementl",
         author_email="hello@elementl.com",
         license="Apache-2.0",
         description="Package for datadog Dagster framework components.",
         url="https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-datadog",
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
-        install_requires=["dagster", "datadog"],
+        packages=find_packages(exclude=["dagster_datadog_tests*"]),
+        install_requires=["dagster==1.0.5", "datadog"],
         zip_safe=False,
     )
```

