# Comparing `tmp/dagster-snowflake-pandas-0.19.6.tar.gz` & `tmp/dagster-snowflake-pandas-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-snowflake-pandas-0.19.6.tar", last modified: Thu May 25 17:24:28 2023, max compression
+gzip compressed data, was "dagster-snowflake-pandas-1.0.5.tar", last modified: Fri Aug 26 13:46:17 2022, max compression
```

## Comparing `dagster-snowflake-pandas-0.19.6.tar` & `dagster-snowflake-pandas-1.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:24:28.009431 dagster-snowflake-pandas-0.19.6/
--rw-r--r--   0 root         (0) root         (0)    11344 2023-05-25 17:16:50.000000 dagster-snowflake-pandas-0.19.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)       76 2023-05-25 17:16:50.000000 dagster-snowflake-pandas-0.19.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      702 2023-05-25 17:24:28.013430 dagster-snowflake-pandas-0.19.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      158 2023-05-25 17:16:50.000000 dagster-snowflake-pandas-0.19.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:24:28.009431 dagster-snowflake-pandas-0.19.6/dagster_snowflake_pandas/
--rw-r--r--   0 root         (0) root         (0)      413 2023-05-25 17:16:50.000000 dagster-snowflake-pandas-0.19.6/dagster_snowflake_pandas/__init__.py
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-25 17:16:50.000000 dagster-snowflake-pandas-0.19.6/dagster_snowflake_pandas/py.typed
--rw-r--r--   0 root         (0) root         (0)    11677 2023-05-25 17:16:50.000000 dagster-snowflake-pandas-0.19.6/dagster_snowflake_pandas/snowflake_pandas_type_handler.py
--rw-r--r--   0 root         (0) root         (0)       23 2023-05-25 17:16:50.000000 dagster-snowflake-pandas-0.19.6/dagster_snowflake_pandas/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:24:28.009431 dagster-snowflake-pandas-0.19.6/dagster_snowflake_pandas.egg-info/
--rw-r--r--   0 root         (0) root         (0)      702 2023-05-25 17:24:27.000000 dagster-snowflake-pandas-0.19.6/dagster_snowflake_pandas.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      499 2023-05-25 17:24:27.000000 dagster-snowflake-pandas-0.19.6/dagster_snowflake_pandas.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 17:24:27.000000 dagster-snowflake-pandas-0.19.6/dagster_snowflake_pandas.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 17:24:27.000000 dagster-snowflake-pandas-0.19.6/dagster_snowflake_pandas.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      137 2023-05-25 17:24:27.000000 dagster-snowflake-pandas-0.19.6/dagster_snowflake_pandas.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2023-05-25 17:24:27.000000 dagster-snowflake-pandas-0.19.6/dagster_snowflake_pandas.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      171 2023-05-25 17:24:28.013430 dagster-snowflake-pandas-0.19.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1586 2023-05-25 17:16:50.000000 dagster-snowflake-pandas-0.19.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:46:17.804731 dagster-snowflake-pandas-1.0.5/
+-rw-r--r--   0 root         (0) root         (0)    11357 2022-08-26 13:33:01.000000 dagster-snowflake-pandas-1.0.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       76 2022-08-26 13:33:01.000000 dagster-snowflake-pandas-1.0.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      678 2022-08-26 13:46:17.804731 dagster-snowflake-pandas-1.0.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      158 2022-08-26 13:33:01.000000 dagster-snowflake-pandas-1.0.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:46:17.800732 dagster-snowflake-pandas-1.0.5/dagster_snowflake_pandas/
+-rw-r--r--   0 root         (0) root         (0)      280 2022-08-26 13:33:01.000000 dagster-snowflake-pandas-1.0.5/dagster_snowflake_pandas/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        8 2022-08-26 13:33:01.000000 dagster-snowflake-pandas-1.0.5/dagster_snowflake_pandas/py.typed
+-rw-r--r--   0 root         (0) root         (0)     3970 2022-08-26 13:33:01.000000 dagster-snowflake-pandas-1.0.5/dagster_snowflake_pandas/snowflake_pandas_type_handler.py
+-rw-r--r--   0 root         (0) root         (0)       22 2022-08-26 13:33:01.000000 dagster-snowflake-pandas-1.0.5/dagster_snowflake_pandas/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:46:17.804731 dagster-snowflake-pandas-1.0.5/dagster_snowflake_pandas.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      678 2022-08-26 13:46:17.000000 dagster-snowflake-pandas-1.0.5/dagster_snowflake_pandas.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      499 2022-08-26 13:46:17.000000 dagster-snowflake-pandas-1.0.5/dagster_snowflake_pandas.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-08-26 13:46:17.000000 dagster-snowflake-pandas-1.0.5/dagster_snowflake_pandas.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-08-26 13:46:17.000000 dagster-snowflake-pandas-1.0.5/dagster_snowflake_pandas.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      112 2022-08-26 13:46:17.000000 dagster-snowflake-pandas-1.0.5/dagster_snowflake_pandas.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2022-08-26 13:46:17.000000 dagster-snowflake-pandas-1.0.5/dagster_snowflake_pandas.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      171 2022-08-26 13:46:17.804731 dagster-snowflake-pandas-1.0.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1540 2022-08-26 13:33:01.000000 dagster-snowflake-pandas-1.0.5/setup.py
```

### Comparing `dagster-snowflake-pandas-0.19.6/LICENSE` & `dagster-snowflake-pandas-1.0.5/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -182,15 +182,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright 2023 Elementl, Inc.
+   Copyright {yyyy} {name of copyright owner}
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `dagster-snowflake-pandas-0.19.6/PKG-INFO` & `dagster-snowflake-pandas-1.0.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 Metadata-Version: 2.1
 Name: dagster-snowflake-pandas
-Version: 0.19.6
+Version: 1.0.5
 Summary: Package for integrating Snowflake and Pandas with Dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-snowflake-pandas
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 License-File: LICENSE
+
+UNKNOWN
+
```

### Comparing `dagster-snowflake-pandas-0.19.6/dagster_snowflake_pandas.egg-info/PKG-INFO` & `dagster-snowflake-pandas-1.0.5/dagster_snowflake_pandas.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 Metadata-Version: 2.1
 Name: dagster-snowflake-pandas
-Version: 0.19.6
+Version: 1.0.5
 Summary: Package for integrating Snowflake and Pandas with Dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-snowflake-pandas
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 License-File: LICENSE
+
+UNKNOWN
+
```

### Comparing `dagster-snowflake-pandas-0.19.6/setup.py` & `dagster-snowflake-pandas-1.0.5/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,46 +1,44 @@
-from pathlib import Path
 from typing import Dict
 
 from setuptools import find_packages, setup
 
 
 def get_version() -> str:
     version: Dict[str, str] = {}
-    with open(Path(__file__).parent / "dagster_snowflake_pandas/version.py", encoding="utf8") as fp:
-        exec(fp.read(), version)
+    with open("dagster_snowflake_pandas/version.py", encoding="utf8") as fp:
+        exec(fp.read(), version)  # pylint: disable=W0122
 
     return version["__version__"]
 
 
-ver = get_version()
-# dont pin dev installs to avoid pip dep resolver issues
-pin = "" if ver == "1!0+dev" else f"=={ver}"
-setup(
-    name="dagster-snowflake-pandas",
-    version=ver,
-    author="Elementl",
-    author_email="hello@elementl.com",
-    license="Apache-2.0",
-    description="Package for integrating Snowflake and Pandas with Dagster.",
-    url="https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-snowflake-pandas",
-    classifiers=[
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
-        "Programming Language :: Python :: 3.11",
-        "License :: OSI Approved :: Apache Software License",
-        "Operating System :: OS Independent",
-    ],
-    packages=find_packages(exclude=["dagster_snowflake_pandas_tests*"]),
-    install_requires=[
-        "dagster==1.3.6",
-        "dagster-snowflake==0.19.6",
-        "pandas",
-        "requests",
-        "snowflake-connector-python[pandas]",
-        "sqlalchemy!=1.4.42",  # workaround for https://github.com/snowflakedb/snowflake-sqlalchemy/issues/350
-        "snowflake-sqlalchemy>=1.2",
-    ],
-    zip_safe=False,
-)
+if __name__ == "__main__":
+    ver = get_version()
+    # dont pin dev installs to avoid pip dep resolver issues
+    pin = "" if ver == "0+dev" else f"=={ver}"
+    setup(
+        name="dagster-snowflake-pandas",
+        version=ver,
+        author="Elementl",
+        author_email="hello@elementl.com",
+        license="Apache-2.0",
+        description="Package for integrating Snowflake and Pandas with Dagster.",
+        url="https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-snowflake-pandas",
+        classifiers=[
+            "Programming Language :: Python :: 3.7",
+            "Programming Language :: Python :: 3.8",
+            "Programming Language :: Python :: 3.9",
+            "Programming Language :: Python :: 3.10",
+            "License :: OSI Approved :: Apache Software License",
+            "Operating System :: OS Independent",
+        ],
+        packages=find_packages(exclude=["dagster_snowflake_pandas_tests*"]),
+        install_requires=[
+            "dagster==1.0.5",
+            "dagster-snowflake==1.0.5",
+            "pandas",
+            "requests",
+            "snowflake-connector-python[pandas]",
+            "snowflake-sqlalchemy",
+        ],
+        zip_safe=False,
+    )
```

