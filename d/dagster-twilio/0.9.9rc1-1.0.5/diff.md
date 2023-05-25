# Comparing `tmp/dagster-twilio-0.9.9rc1.tar.gz` & `tmp/dagster-twilio-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dagster-twilio-0.9.9rc1.tar", last modified: Thu Sep 17 21:07:56 2020, max compression
+gzip compressed data, was "dagster-twilio-1.0.5.tar", last modified: Fri Aug 26 13:45:18 2022, max compression
```

## Comparing `dagster-twilio-0.9.9rc1.tar` & `dagster-twilio-1.0.5.tar`

### file list

```diff
@@ -1,22 +1,19 @@
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:07:56.000000 dagster-twilio-0.9.9rc1/
--rw-r--r--   0 bobchen    (501) staff       (20)    11357 2020-09-17 21:04:59.000000 dagster-twilio-0.9.9rc1/LICENSE
--rw-r--r--   0 bobchen    (501) staff       (20)       34 2020-09-17 21:04:59.000000 dagster-twilio-0.9.9rc1/MANIFEST.in
--rw-r--r--   0 bobchen    (501) staff       (20)      573 2020-09-17 21:07:56.000000 dagster-twilio-0.9.9rc1/PKG-INFO
--rw-r--r--   0 bobchen    (501) staff       (20)      128 2020-09-17 21:04:59.000000 dagster-twilio-0.9.9rc1/README.md
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:07:56.000000 dagster-twilio-0.9.9rc1/dagster_twilio/
--rw-r--r--   0 bobchen    (501) staff       (20)      227 2020-09-17 21:04:59.000000 dagster-twilio-0.9.9rc1/dagster_twilio/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)      452 2020-09-17 21:04:59.000000 dagster-twilio-0.9.9rc1/dagster_twilio/resources.py
--rw-r--r--   0 bobchen    (501) staff       (20)       27 2020-09-17 21:04:59.000000 dagster-twilio-0.9.9rc1/dagster_twilio/version.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:07:56.000000 dagster-twilio-0.9.9rc1/dagster_twilio.egg-info/
--rw-r--r--   0 bobchen    (501) staff       (20)      573 2020-09-17 21:07:56.000000 dagster-twilio-0.9.9rc1/dagster_twilio.egg-info/PKG-INFO
--rw-r--r--   0 bobchen    (501) staff       (20)      464 2020-09-17 21:07:56.000000 dagster-twilio-0.9.9rc1/dagster_twilio.egg-info/SOURCES.txt
--rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:07:56.000000 dagster-twilio-0.9.9rc1/dagster_twilio.egg-info/dependency_links.txt
--rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:07:56.000000 dagster-twilio-0.9.9rc1/dagster_twilio.egg-info/not-zip-safe
--rw-r--r--   0 bobchen    (501) staff       (20)       15 2020-09-17 21:07:56.000000 dagster-twilio-0.9.9rc1/dagster_twilio.egg-info/requires.txt
--rw-r--r--   0 bobchen    (501) staff       (20)       36 2020-09-17 21:07:56.000000 dagster-twilio-0.9.9rc1/dagster_twilio.egg-info/top_level.txt
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:07:56.000000 dagster-twilio-0.9.9rc1/dagster_twilio_tests/
--rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:04:59.000000 dagster-twilio-0.9.9rc1/dagster_twilio_tests/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)     1370 2020-09-17 21:04:59.000000 dagster-twilio-0.9.9rc1/dagster_twilio_tests/test_resources.py
--rw-r--r--   0 bobchen    (501) staff       (20)       92 2020-09-17 21:04:59.000000 dagster-twilio-0.9.9rc1/dagster_twilio_tests/test_version.py
--rw-r--r--   0 bobchen    (501) staff       (20)       74 2020-09-17 21:07:56.000000 dagster-twilio-0.9.9rc1/setup.cfg
--rw-r--r--   0 bobchen    (501) staff       (20)     1024 2020-09-17 21:04:59.000000 dagster-twilio-0.9.9rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:45:18.900407 dagster-twilio-1.0.5/
+-rw-r--r--   0 root         (0) root         (0)    11357 2022-08-26 13:33:01.000000 dagster-twilio-1.0.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       66 2022-08-26 13:33:01.000000 dagster-twilio-1.0.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      632 2022-08-26 13:45:18.900407 dagster-twilio-1.0.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      128 2022-08-26 13:33:01.000000 dagster-twilio-1.0.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:45:18.900407 dagster-twilio-1.0.5/dagster_twilio/
+-rw-r--r--   0 root         (0) root         (0)      228 2022-08-26 13:33:01.000000 dagster-twilio-1.0.5/dagster_twilio/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        8 2022-08-26 13:33:01.000000 dagster-twilio-1.0.5/dagster_twilio/py.typed
+-rw-r--r--   0 root         (0) root         (0)      452 2022-08-26 13:33:01.000000 dagster-twilio-1.0.5/dagster_twilio/resources.py
+-rw-r--r--   0 root         (0) root         (0)       22 2022-08-26 13:33:01.000000 dagster-twilio-1.0.5/dagster_twilio/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:45:18.900407 dagster-twilio-1.0.5/dagster_twilio.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      632 2022-08-26 13:45:18.000000 dagster-twilio-1.0.5/dagster_twilio.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      379 2022-08-26 13:45:18.000000 dagster-twilio-1.0.5/dagster_twilio.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-08-26 13:45:18.000000 dagster-twilio-1.0.5/dagster_twilio.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-08-26 13:45:18.000000 dagster-twilio-1.0.5/dagster_twilio.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       22 2022-08-26 13:45:18.000000 dagster-twilio-1.0.5/dagster_twilio.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2022-08-26 13:45:18.000000 dagster-twilio-1.0.5/dagster_twilio.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      161 2022-08-26 13:45:18.904407 dagster-twilio-1.0.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1289 2022-08-26 13:33:01.000000 dagster-twilio-1.0.5/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `dagster-twilio-0.9.9rc1/LICENSE` & `dagster-twilio-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-twilio-0.9.9rc1/PKG-INFO` & `dagster-twilio-1.0.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,19 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: dagster-twilio
-Version: 0.9.9rc1
+Version: 1.0.5
 Summary: A Dagster integration for twilio
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-twilio
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

### Comparing `dagster-twilio-0.9.9rc1/dagster_twilio.egg-info/PKG-INFO` & `dagster-twilio-1.0.5/dagster_twilio.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,19 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: dagster-twilio
-Version: 0.9.9rc1
+Version: 1.0.5
 Summary: A Dagster integration for twilio
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-twilio
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

### Comparing `dagster-twilio-0.9.9rc1/setup.py` & `dagster-twilio-1.0.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,37 @@
+from typing import Dict
+
 from setuptools import find_packages, setup
 
 
-def get_version():
-    version = {}
-    with open("dagster_twilio/version.py") as fp:
+def get_version() -> str:
+    version: Dict[str, str] = {}
+    with open("dagster_twilio/version.py", encoding="utf8") as fp:
         exec(fp.read(), version)  # pylint: disable=W0122
 
     return version["__version__"]
 
 
 if __name__ == "__main__":
+    ver = get_version()
+    # dont pin dev installs to avoid pip dep resolver issues
+    pin = "" if ver == "0+dev" else f"=={ver}"
     setup(
         name="dagster-twilio",
-        version=get_version(),
+        version=ver,
         author="Elementl",
         author_email="hello@elementl.com",
         license="Apache-2.0",
         description="A Dagster integration for twilio",
         url="https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-twilio",
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
-        install_requires=["dagster", "twilio"],
+        packages=find_packages(exclude=["dagster_twilio_tests*"]),
+        install_requires=["dagster==1.0.5", "twilio"],
         zip_safe=False,
     )
```

