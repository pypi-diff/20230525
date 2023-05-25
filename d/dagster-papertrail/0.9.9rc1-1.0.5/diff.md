# Comparing `tmp/dagster-papertrail-0.9.9rc1.tar.gz` & `tmp/dagster-papertrail-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dagster-papertrail-0.9.9rc1.tar", last modified: Thu Sep 17 21:08:00 2020, max compression
+gzip compressed data, was "dagster-papertrail-1.0.5.tar", last modified: Fri Aug 26 13:44:22 2022, max compression
```

## Comparing `dagster-papertrail-0.9.9rc1.tar` & `dagster-papertrail-1.0.5.tar`

### file list

```diff
@@ -1,22 +1,19 @@
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:00.000000 dagster-papertrail-0.9.9rc1/
--rw-r--r--   0 bobchen    (501) staff       (20)    11357 2020-09-17 21:04:59.000000 dagster-papertrail-0.9.9rc1/LICENSE
--rw-r--r--   0 bobchen    (501) staff       (20)       34 2020-09-17 21:04:59.000000 dagster-papertrail-0.9.9rc1/MANIFEST.in
--rw-r--r--   0 bobchen    (501) staff       (20)      601 2020-09-17 21:08:00.000000 dagster-papertrail-0.9.9rc1/PKG-INFO
--rw-r--r--   0 bobchen    (501) staff       (20)      140 2020-09-17 21:04:59.000000 dagster-papertrail-0.9.9rc1/README.md
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:00.000000 dagster-papertrail-0.9.9rc1/dagster_papertrail/
--rw-r--r--   0 bobchen    (501) staff       (20)      233 2020-09-17 21:04:59.000000 dagster-papertrail-0.9.9rc1/dagster_papertrail/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)     2296 2020-09-17 21:04:59.000000 dagster-papertrail-0.9.9rc1/dagster_papertrail/loggers.py
--rw-r--r--   0 bobchen    (501) staff       (20)       27 2020-09-17 21:04:59.000000 dagster-papertrail-0.9.9rc1/dagster_papertrail/version.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:00.000000 dagster-papertrail-0.9.9rc1/dagster_papertrail.egg-info/
--rw-r--r--   0 bobchen    (501) staff       (20)      601 2020-09-17 21:08:00.000000 dagster-papertrail-0.9.9rc1/dagster_papertrail.egg-info/PKG-INFO
--rw-r--r--   0 bobchen    (501) staff       (20)      508 2020-09-17 21:08:00.000000 dagster-papertrail-0.9.9rc1/dagster_papertrail.egg-info/SOURCES.txt
--rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:08:00.000000 dagster-papertrail-0.9.9rc1/dagster_papertrail.egg-info/dependency_links.txt
--rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:08:00.000000 dagster-papertrail-0.9.9rc1/dagster_papertrail.egg-info/not-zip-safe
--rw-r--r--   0 bobchen    (501) staff       (20)        8 2020-09-17 21:08:00.000000 dagster-papertrail-0.9.9rc1/dagster_papertrail.egg-info/requires.txt
--rw-r--r--   0 bobchen    (501) staff       (20)       44 2020-09-17 21:08:00.000000 dagster-papertrail-0.9.9rc1/dagster_papertrail.egg-info/top_level.txt
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:00.000000 dagster-papertrail-0.9.9rc1/dagster_papertrail_tests/
--rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:04:59.000000 dagster-papertrail-0.9.9rc1/dagster_papertrail_tests/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)     1601 2020-09-17 21:04:59.000000 dagster-papertrail-0.9.9rc1/dagster_papertrail_tests/test_loggers.py
--rw-r--r--   0 bobchen    (501) staff       (20)       96 2020-09-17 21:04:59.000000 dagster-papertrail-0.9.9rc1/dagster_papertrail_tests/test_version.py
--rw-r--r--   0 bobchen    (501) staff       (20)       74 2020-09-17 21:08:00.000000 dagster-papertrail-0.9.9rc1/setup.cfg
--rw-r--r--   0 bobchen    (501) staff       (20)     1046 2020-09-17 21:04:59.000000 dagster-papertrail-0.9.9rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:44:22.248097 dagster-papertrail-1.0.5/
+-rw-r--r--   0 root         (0) root         (0)    11357 2022-08-26 13:33:01.000000 dagster-papertrail-1.0.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       70 2022-08-26 13:33:01.000000 dagster-papertrail-1.0.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      660 2022-08-26 13:44:22.248097 dagster-papertrail-1.0.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      140 2022-08-26 13:33:01.000000 dagster-papertrail-1.0.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:44:22.248097 dagster-papertrail-1.0.5/dagster_papertrail/
+-rw-r--r--   0 root         (0) root         (0)      234 2022-08-26 13:33:01.000000 dagster-papertrail-1.0.5/dagster_papertrail/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2384 2022-08-26 13:33:01.000000 dagster-papertrail-1.0.5/dagster_papertrail/loggers.py
+-rw-r--r--   0 root         (0) root         (0)        8 2022-08-26 13:33:01.000000 dagster-papertrail-1.0.5/dagster_papertrail/py.typed
+-rw-r--r--   0 root         (0) root         (0)       22 2022-08-26 13:33:01.000000 dagster-papertrail-1.0.5/dagster_papertrail/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:44:22.248097 dagster-papertrail-1.0.5/dagster_papertrail.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      660 2022-08-26 13:44:22.000000 dagster-papertrail-1.0.5/dagster_papertrail.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      417 2022-08-26 13:44:22.000000 dagster-papertrail-1.0.5/dagster_papertrail.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-08-26 13:44:22.000000 dagster-papertrail-1.0.5/dagster_papertrail.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-08-26 13:44:22.000000 dagster-papertrail-1.0.5/dagster_papertrail.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       15 2022-08-26 13:44:22.000000 dagster-papertrail-1.0.5/dagster_papertrail.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2022-08-26 13:44:22.000000 dagster-papertrail-1.0.5/dagster_papertrail.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      165 2022-08-26 13:44:22.252097 dagster-papertrail-1.0.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1315 2022-08-26 13:33:01.000000 dagster-papertrail-1.0.5/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `dagster-papertrail-0.9.9rc1/LICENSE` & `dagster-papertrail-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-papertrail-0.9.9rc1/PKG-INFO` & `dagster-papertrail-1.0.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,19 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: dagster-papertrail
-Version: 0.9.9rc1
+Version: 1.0.5
 Summary: Package for papertrail Dagster framework components.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-papertrail
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

### Comparing `dagster-papertrail-0.9.9rc1/dagster_papertrail.egg-info/PKG-INFO` & `dagster-papertrail-1.0.5/dagster_papertrail.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,19 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: dagster-papertrail
-Version: 0.9.9rc1
+Version: 1.0.5
 Summary: Package for papertrail Dagster framework components.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-papertrail
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

### Comparing `dagster-papertrail-0.9.9rc1/setup.py` & `dagster-papertrail-1.0.5/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,31 +1,37 @@
+from typing import Dict
+
 from setuptools import find_packages, setup
 
 
-def get_version():
-    version = {}
-    with open("dagster_papertrail/version.py") as fp:
+def get_version() -> str:
+    version: Dict[str, str] = {}
+    with open("dagster_papertrail/version.py", encoding="utf8") as fp:
         exec(fp.read(), version)  # pylint: disable=W0122
 
     return version["__version__"]
 
 
 if __name__ == "__main__":
+    ver = get_version()
+    # dont pin dev installs to avoid pip dep resolver issues
+    pin = "" if ver == "0+dev" else f"=={ver}"
     setup(
         name="dagster-papertrail",
-        version=get_version(),
+        version=ver,
         author="Elementl",
         author_email="hello@elementl.com",
         license="Apache-2.0",
         description="Package for papertrail Dagster framework components.",
         url="https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-papertrail",
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
-        install_requires=["dagster"],
+        packages=find_packages(exclude=["dagster_papertrail_tests*"]),
+        install_requires=["dagster==1.0.5"],
         zip_safe=False,
     )
```

