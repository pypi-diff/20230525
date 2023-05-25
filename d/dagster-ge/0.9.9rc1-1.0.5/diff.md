# Comparing `tmp/dagster-ge-0.9.9rc1.tar.gz` & `tmp/dagster-ge-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dagster-ge-0.9.9rc1.tar", last modified: Thu Sep 17 21:08:11 2020, max compression
+gzip compressed data, was "dagster-ge-1.0.5.tar", last modified: Fri Aug 26 13:45:04 2022, max compression
```

## Comparing `dagster-ge-0.9.9rc1.tar` & `dagster-ge-1.0.5.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:11.000000 dagster-ge-0.9.9rc1/
--rw-r--r--   0 bobchen    (501) staff       (20)    11357 2020-09-17 21:04:59.000000 dagster-ge-0.9.9rc1/LICENSE
--rw-r--r--   0 bobchen    (501) staff       (20)       16 2020-09-17 21:04:59.000000 dagster-ge-0.9.9rc1/MANIFEST.in
--rw-r--r--   0 bobchen    (501) staff       (20)      544 2020-09-17 21:08:11.000000 dagster-ge-0.9.9rc1/PKG-INFO
--rw-r--r--   0 bobchen    (501) staff       (20)      115 2020-09-17 21:04:59.000000 dagster-ge-0.9.9rc1/README.md
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:11.000000 dagster-ge-0.9.9rc1/dagster_ge/
--rw-r--r--   0 bobchen    (501) staff       (20)       92 2020-09-17 21:04:59.000000 dagster-ge-0.9.9rc1/dagster_ge/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)     3835 2020-09-17 21:04:59.000000 dagster-ge-0.9.9rc1/dagster_ge/factory.py
--rw-r--r--   0 bobchen    (501) staff       (20)       27 2020-09-17 21:04:59.000000 dagster-ge-0.9.9rc1/dagster_ge/version.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:11.000000 dagster-ge-0.9.9rc1/dagster_ge.egg-info/
--rw-r--r--   0 bobchen    (501) staff       (20)      544 2020-09-17 21:08:10.000000 dagster-ge-0.9.9rc1/dagster_ge.egg-info/PKG-INFO
--rw-r--r--   0 bobchen    (501) staff       (20)      317 2020-09-17 21:08:10.000000 dagster-ge-0.9.9rc1/dagster_ge.egg-info/SOURCES.txt
--rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:08:10.000000 dagster-ge-0.9.9rc1/dagster_ge.egg-info/dependency_links.txt
--rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:08:10.000000 dagster-ge-0.9.9rc1/dagster_ge.egg-info/not-zip-safe
--rw-r--r--   0 bobchen    (501) staff       (20)       57 2020-09-17 21:08:10.000000 dagster-ge-0.9.9rc1/dagster_ge.egg-info/requires.txt
--rw-r--r--   0 bobchen    (501) staff       (20)       11 2020-09-17 21:08:10.000000 dagster-ge-0.9.9rc1/dagster_ge.egg-info/top_level.txt
--rw-r--r--   0 bobchen    (501) staff       (20)       74 2020-09-17 21:08:11.000000 dagster-ge-0.9.9rc1/setup.cfg
--rw-r--r--   0 bobchen    (501) staff       (20)     1045 2020-09-17 21:04:59.000000 dagster-ge-0.9.9rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:45:04.548328 dagster-ge-1.0.5/
+-rw-r--r--   0 root         (0) root         (0)    11357 2022-08-26 13:33:01.000000 dagster-ge-1.0.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       43 2022-08-26 13:33:01.000000 dagster-ge-1.0.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      577 2022-08-26 13:45:04.548328 dagster-ge-1.0.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      115 2022-08-26 13:33:01.000000 dagster-ge-1.0.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:45:04.544328 dagster-ge-1.0.5/dagster_ge/
+-rw-r--r--   0 root         (0) root         (0)       86 2022-08-26 13:33:01.000000 dagster-ge-1.0.5/dagster_ge/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9695 2022-08-26 13:33:01.000000 dagster-ge-1.0.5/dagster_ge/factory.py
+-rw-r--r--   0 root         (0) root         (0)        8 2022-08-26 13:33:01.000000 dagster-ge-1.0.5/dagster_ge/py.typed
+-rw-r--r--   0 root         (0) root         (0)       22 2022-08-26 13:33:01.000000 dagster-ge-1.0.5/dagster_ge/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:45:04.548328 dagster-ge-1.0.5/dagster_ge.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      577 2022-08-26 13:45:04.000000 dagster-ge-1.0.5/dagster_ge.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      337 2022-08-26 13:45:04.000000 dagster-ge-1.0.5/dagster_ge.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-08-26 13:45:04.000000 dagster-ge-1.0.5/dagster_ge.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-08-26 13:45:04.000000 dagster-ge-1.0.5/dagster_ge.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      100 2022-08-26 13:45:04.000000 dagster-ge-1.0.5/dagster_ge.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2022-08-26 13:45:04.000000 dagster-ge-1.0.5/dagster_ge.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      192 2022-08-26 13:45:04.548328 dagster-ge-1.0.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1400 2022-08-26 13:33:01.000000 dagster-ge-1.0.5/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `dagster-ge-0.9.9rc1/LICENSE` & `dagster-ge-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-ge-0.9.9rc1/PKG-INFO` & `dagster-ge-1.0.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,17 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: dagster-ge
-Version: 0.9.9rc1
-Summary: Package for GE-specific Dagster framework solid and resource components.
+Version: 1.0.5
+Summary: Package for GE-specific Dagster framework op and resource components.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-ge
 Author: Elementl
-Author-email: UNKNOWN
 License: Apache-2.0
-Description: UNKNOWN
 Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
+License-File: LICENSE
+
+UNKNOWN
+
```

### Comparing `dagster-ge-0.9.9rc1/dagster_ge.egg-info/PKG-INFO` & `dagster-ge-1.0.5/dagster_ge.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,17 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: dagster-ge
-Version: 0.9.9rc1
-Summary: Package for GE-specific Dagster framework solid and resource components.
+Version: 1.0.5
+Summary: Package for GE-specific Dagster framework op and resource components.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-ge
 Author: Elementl
-Author-email: UNKNOWN
 License: Apache-2.0
-Description: UNKNOWN
 Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
+License-File: LICENSE
+
+UNKNOWN
+
```

### Comparing `dagster-ge-0.9.9rc1/setup.py` & `dagster-ge-1.0.5/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,30 +1,41 @@
+from typing import Dict
+
 from setuptools import find_packages, setup
 
 
-def get_version():
-    version = {}
-    with open("dagster_ge/version.py") as fp:
+def get_version() -> str:
+    version: Dict[str, str] = {}
+    with open("dagster_ge/version.py", encoding="utf8") as fp:
         exec(fp.read(), version)  # pylint: disable=W0122
 
     return version["__version__"]
 
 
 if __name__ == "__main__":
+    ver = get_version()
+    # dont pin dev installs to avoid pip dep resolver issues
+    pin = "" if ver == "0+dev" else f"=={ver}"
     setup(
         name="dagster-ge",
-        version=get_version(),
+        version=ver,
         author="Elementl",
         license="Apache-2.0",
-        description="Package for GE-specific Dagster framework solid and resource components.",
+        description="Package for GE-specific Dagster framework op and resource components.",
         # pylint: disable=line-too-long
         url="https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-ge",
         classifiers=[
-            "Programming Language :: Python :: 3.6",
             "Programming Language :: Python :: 3.7",
+            "Programming Language :: Python :: 3.8",
+            "Programming Language :: Python :: 3.9",
             "License :: OSI Approved :: Apache Software License",
             "Operating System :: OS Independent",
         ],
-        packages=find_packages(exclude=["test"]),
-        install_requires=["dagster", "dagster-pandas", "pandas", "great_expectations >=0.11.9"],
+        packages=find_packages(exclude=["dagster_ge_tests*"]),
+        install_requires=[
+            "dagster==1.0.5",
+            "dagster-pandas==1.0.5",
+            "pandas",
+            "great_expectations >=0.11.9, !=0.12.8, !=0.13.17, !=0.13.27",
+        ],
         zip_safe=False,
     )
```

