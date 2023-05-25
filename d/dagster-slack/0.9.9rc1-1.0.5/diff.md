# Comparing `tmp/dagster-slack-0.9.9rc1.tar.gz` & `tmp/dagster-slack-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dagster-slack-0.9.9rc1.tar", last modified: Thu Sep 17 21:08:49 2020, max compression
+gzip compressed data, was "dagster-slack-1.0.5.tar", last modified: Fri Aug 26 13:45:09 2022, max compression
```

## Comparing `dagster-slack-0.9.9rc1.tar` & `dagster-slack-1.0.5.tar`

### file list

```diff
@@ -1,22 +1,21 @@
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:49.000000 dagster-slack-0.9.9rc1/
--rw-r--r--   0 bobchen    (501) staff       (20)    11357 2020-09-17 21:04:59.000000 dagster-slack-0.9.9rc1/LICENSE
--rw-r--r--   0 bobchen    (501) staff       (20)       34 2020-09-17 21:04:59.000000 dagster-slack-0.9.9rc1/MANIFEST.in
--rw-r--r--   0 bobchen    (501) staff       (20)      583 2020-09-17 21:08:49.000000 dagster-slack-0.9.9rc1/PKG-INFO
--rw-r--r--   0 bobchen    (501) staff       (20)      125 2020-09-17 21:04:59.000000 dagster-slack-0.9.9rc1/README.md
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:49.000000 dagster-slack-0.9.9rc1/dagster_slack/
--rw-r--r--   0 bobchen    (501) staff       (20)      224 2020-09-17 21:04:59.000000 dagster-slack-0.9.9rc1/dagster_slack/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)     2865 2020-09-17 21:04:59.000000 dagster-slack-0.9.9rc1/dagster_slack/resources.py
--rw-r--r--   0 bobchen    (501) staff       (20)       27 2020-09-17 21:04:59.000000 dagster-slack-0.9.9rc1/dagster_slack/version.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:49.000000 dagster-slack-0.9.9rc1/dagster_slack.egg-info/
--rw-r--r--   0 bobchen    (501) staff       (20)      583 2020-09-17 21:08:49.000000 dagster-slack-0.9.9rc1/dagster_slack.egg-info/PKG-INFO
--rw-r--r--   0 bobchen    (501) staff       (20)      452 2020-09-17 21:08:49.000000 dagster-slack-0.9.9rc1/dagster_slack.egg-info/SOURCES.txt
--rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:08:49.000000 dagster-slack-0.9.9rc1/dagster_slack.egg-info/dependency_links.txt
--rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:08:49.000000 dagster-slack-0.9.9rc1/dagster_slack.egg-info/not-zip-safe
--rw-r--r--   0 bobchen    (501) staff       (20)       26 2020-09-17 21:08:49.000000 dagster-slack-0.9.9rc1/dagster_slack.egg-info/requires.txt
--rw-r--r--   0 bobchen    (501) staff       (20)       34 2020-09-17 21:08:49.000000 dagster-slack-0.9.9rc1/dagster_slack.egg-info/top_level.txt
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:49.000000 dagster-slack-0.9.9rc1/dagster_slack_tests/
--rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:04:59.000000 dagster-slack-0.9.9rc1/dagster_slack_tests/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)     1068 2020-09-17 21:04:59.000000 dagster-slack-0.9.9rc1/dagster_slack_tests/test_resources.py
--rw-r--r--   0 bobchen    (501) staff       (20)       91 2020-09-17 21:04:59.000000 dagster-slack-0.9.9rc1/dagster_slack_tests/test_version.py
--rw-r--r--   0 bobchen    (501) staff       (20)       74 2020-09-17 21:08:49.000000 dagster-slack-0.9.9rc1/setup.cfg
--rw-r--r--   0 bobchen    (501) staff       (20)     1236 2020-09-17 21:04:59.000000 dagster-slack-0.9.9rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:45:09.248354 dagster-slack-1.0.5/
+-rw-r--r--   0 root         (0) root         (0)    11357 2022-08-26 13:33:01.000000 dagster-slack-1.0.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       65 2022-08-26 13:33:01.000000 dagster-slack-1.0.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      642 2022-08-26 13:45:09.248354 dagster-slack-1.0.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      125 2022-08-26 13:33:01.000000 dagster-slack-1.0.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:45:09.244353 dagster-slack-1.0.5/dagster_slack/
+-rw-r--r--   0 root         (0) root         (0)      333 2022-08-26 13:33:01.000000 dagster-slack-1.0.5/dagster_slack/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4024 2022-08-26 13:33:01.000000 dagster-slack-1.0.5/dagster_slack/hooks.py
+-rw-r--r--   0 root         (0) root         (0)        8 2022-08-26 13:33:01.000000 dagster-slack-1.0.5/dagster_slack/py.typed
+-rw-r--r--   0 root         (0) root         (0)     1598 2022-08-26 13:33:01.000000 dagster-slack-1.0.5/dagster_slack/resources.py
+-rw-r--r--   0 root         (0) root         (0)     7242 2022-08-26 13:33:01.000000 dagster-slack-1.0.5/dagster_slack/sensors.py
+-rw-r--r--   0 root         (0) root         (0)       22 2022-08-26 13:33:01.000000 dagster-slack-1.0.5/dagster_slack/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:45:09.248354 dagster-slack-1.0.5/dagster_slack.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      642 2022-08-26 13:45:09.000000 dagster-slack-1.0.5/dagster_slack.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      417 2022-08-26 13:45:09.000000 dagster-slack-1.0.5/dagster_slack.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-08-26 13:45:09.000000 dagster-slack-1.0.5/dagster_slack.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-08-26 13:45:09.000000 dagster-slack-1.0.5/dagster_slack.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       25 2022-08-26 13:45:09.000000 dagster-slack-1.0.5/dagster_slack.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2022-08-26 13:45:09.000000 dagster-slack-1.0.5/dagster_slack.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      160 2022-08-26 13:45:09.248354 dagster-slack-1.0.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1287 2022-08-26 13:33:01.000000 dagster-slack-1.0.5/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `dagster-slack-0.9.9rc1/LICENSE` & `dagster-slack-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-slack-0.9.9rc1/PKG-INFO` & `dagster-slack-1.0.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,19 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: dagster-slack
-Version: 0.9.9rc1
+Version: 1.0.5
 Summary: A Slack client resource for posting to Slack
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-slack
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

### Comparing `dagster-slack-0.9.9rc1/dagster_slack.egg-info/PKG-INFO` & `dagster-slack-1.0.5/dagster_slack.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,19 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: dagster-slack
-Version: 0.9.9rc1
+Version: 1.0.5
 Summary: A Slack client resource for posting to Slack
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-slack
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

### Comparing `dagster-slack-0.9.9rc1/setup.py` & `dagster-slack-1.0.5/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 from setuptools import find_packages, setup
 
 
 def get_version():
     version = {}
-    with open("dagster_slack/version.py") as fp:
+    with open("dagster_slack/version.py", encoding="utf8") as fp:
         exec(fp.read(), version)  # pylint: disable=W0122
 
     return version["__version__"]
 
 
 if __name__ == "__main__":
+    ver = get_version()
+    # dont pin dev installs to avoid pip dep resolver issues
+    pin = "" if ver == "0+dev" else f"=={ver}"
     setup(
         name="dagster-slack",
-        version=get_version(),
+        version=ver,
         author="Elementl",
         author_email="hello@elementl.com",
         license="Apache-2.0",
         description="A Slack client resource for posting to Slack",
         url="https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-slack",
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
+        packages=find_packages(exclude=["dagster_slack_tests*"]),
         install_requires=[
-            "dagster",
-            # Slack 2.x does not support Python 2
-            # https://github.com/slackapi/python-slackclient/wiki/Migrating-to-2.x#minimum-python-versions
-            "slackclient<2.0.0",
+            "dagster==1.0.5",
+            "slack_sdk",
         ],
         zip_safe=False,
     )
```

