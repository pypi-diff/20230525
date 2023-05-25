# Comparing `tmp/testit-cli-0.1.4.tar.gz` & `tmp/testit-cli-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testit-cli-0.1.4.tar", last modified: Wed Apr  5 08:10:15 2023, max compression
+gzip compressed data, was "testit-cli-0.1.5.tar", last modified: Thu May 25 13:41:30 2023, max compression
```

## Comparing `testit-cli-0.1.4.tar` & `testit-cli-0.1.5.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 08:10:15.032276 testit-cli-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-05 08:10:00.000000 testit-cli-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-04-05 08:10:15.032276 testit-cli-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-05 08:10:00.000000 testit-cli-0.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-05 08:10:15.032276 testit-cli-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-05 08:10:00.000000 testit-cli-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 08:10:15.028276 testit-cli-0.1.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 08:10:15.032276 testit-cli-0.1.4/src/testit_cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 08:10:00.000000 testit-cli-0.1.4/src/testit_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-04-05 08:10:00.000000 testit-cli-0.1.4/src/testit_cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4221 2023-04-05 08:10:00.000000 testit-cli-0.1.4/src/testit_cli/apiclient.py
--rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-04-05 08:10:00.000000 testit-cli-0.1.4/src/testit_cli/args_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-04-05 08:10:00.000000 testit-cli-0.1.4/src/testit_cli/configurator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-04-05 08:10:00.000000 testit-cli-0.1.4/src/testit_cli/converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-04-05 08:10:00.000000 testit-cli-0.1.4/src/testit_cli/importer.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-05 08:10:00.000000 testit-cli-0.1.4/src/testit_cli/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 08:10:15.032276 testit-cli-0.1.4/src/testit_cli/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 08:10:00.000000 testit-cli-0.1.4/src/testit_cli/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-04-05 08:10:00.000000 testit-cli-0.1.4/src/testit_cli/models/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-05 08:10:00.000000 testit-cli-0.1.4/src/testit_cli/models/mode.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-05 08:10:00.000000 testit-cli-0.1.4/src/testit_cli/models/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-04-05 08:10:00.000000 testit-cli-0.1.4/src/testit_cli/models/testcase.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-05 08:10:00.000000 testit-cli-0.1.4/src/testit_cli/models/testrun.py
--rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-04-05 08:10:00.000000 testit-cli-0.1.4/src/testit_cli/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-04-05 08:10:00.000000 testit-cli-0.1.4/src/testit_cli/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 08:10:15.032276 testit-cli-0.1.4/src/testit_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-04-05 08:10:15.000000 testit-cli-0.1.4/src/testit_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-04-05 08:10:15.000000 testit-cli-0.1.4/src/testit_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 08:10:15.000000 testit-cli-0.1.4/src/testit_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-05 08:10:15.000000 testit-cli-0.1.4/src/testit_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-05 08:10:15.000000 testit-cli-0.1.4/src/testit_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-05 08:10:15.000000 testit-cli-0.1.4/src/testit_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:41:30.878831 testit-cli-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-25 13:41:16.000000 testit-cli-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-25 13:41:30.878831 testit-cli-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-25 13:41:16.000000 testit-cli-0.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 13:41:30.878831 testit-cli-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-25 13:41:16.000000 testit-cli-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:41:30.874830 testit-cli-0.1.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:41:30.874830 testit-cli-0.1.5/src/testit_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 13:41:16.000000 testit-cli-0.1.5/src/testit_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-25 13:41:16.000000 testit-cli-0.1.5/src/testit_cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4221 2023-05-25 13:41:16.000000 testit-cli-0.1.5/src/testit_cli/apiclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-05-25 13:41:16.000000 testit-cli-0.1.5/src/testit_cli/args_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-05-25 13:41:16.000000 testit-cli-0.1.5/src/testit_cli/configurator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-25 13:41:16.000000 testit-cli-0.1.5/src/testit_cli/converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-05-25 13:41:16.000000 testit-cli-0.1.5/src/testit_cli/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-25 13:41:16.000000 testit-cli-0.1.5/src/testit_cli/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:41:30.878831 testit-cli-0.1.5/src/testit_cli/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 13:41:16.000000 testit-cli-0.1.5/src/testit_cli/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-25 13:41:16.000000 testit-cli-0.1.5/src/testit_cli/models/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-25 13:41:16.000000 testit-cli-0.1.5/src/testit_cli/models/mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-25 13:41:16.000000 testit-cli-0.1.5/src/testit_cli/models/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-05-25 13:41:16.000000 testit-cli-0.1.5/src/testit_cli/models/testcase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-25 13:41:16.000000 testit-cli-0.1.5/src/testit_cli/models/testrun.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-05-25 13:41:16.000000 testit-cli-0.1.5/src/testit_cli/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-05-25 13:41:16.000000 testit-cli-0.1.5/src/testit_cli/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:41:30.878831 testit-cli-0.1.5/src/testit_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-25 13:41:30.000000 testit-cli-0.1.5/src/testit_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-25 13:41:30.000000 testit-cli-0.1.5/src/testit_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 13:41:30.000000 testit-cli-0.1.5/src/testit_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-25 13:41:30.000000 testit-cli-0.1.5/src/testit_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-25 13:41:30.000000 testit-cli-0.1.5/src/testit_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-25 13:41:30.000000 testit-cli-0.1.5/src/testit_cli.egg-info/top_level.txt
```

### Comparing `testit-cli-0.1.4/LICENSE` & `testit-cli-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `testit-cli-0.1.4/PKG-INFO` & `testit-cli-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testit-cli
-Version: 0.1.4
+Version: 0.1.5
 Summary: This tool is the command line wrapper of Test IT allowing you to upload the test results in real time to Test IT
 Home-page: https://pypi.org/project/testit/
 Author: Integration team
 Author-email: integrations@testit.software
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `testit-cli-0.1.4/setup.py` & `testit-cli-0.1.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='testit-cli',
-    version='0.1.4',
+    version='0.1.5',
     description='This tool is the command line wrapper of Test IT allowing you to upload the test results in real time '
                 'to Test IT',
     long_description=open('README.md', "r").read(),
     long_description_content_type="text/markdown",
     url='https://pypi.org/project/testit/',
     author='Integration team',
     author_email='integrations@testit.software',
```

### Comparing `testit-cli-0.1.4/src/testit_cli/__main__.py` & `testit-cli-0.1.5/src/testit_cli/__main__.py`

 * *Files identical despite different names*

### Comparing `testit-cli-0.1.4/src/testit_cli/apiclient.py` & `testit-cli-0.1.5/src/testit_cli/apiclient.py`

 * *Files identical despite different names*

### Comparing `testit-cli-0.1.4/src/testit_cli/args_parser.py` & `testit-cli-0.1.5/src/testit_cli/args_parser.py`

 * *Files identical despite different names*

### Comparing `testit-cli-0.1.4/src/testit_cli/configurator.py` & `testit-cli-0.1.5/src/testit_cli/configurator.py`

 * *Files identical despite different names*

### Comparing `testit-cli-0.1.4/src/testit_cli/converter.py` & `testit-cli-0.1.5/src/testit_cli/converter.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     def test_result_to_autotest_put_model(result, external_id: str, project_id: str):
         return AutoTestPutModel(
             external_id,
             project_id,
             result.get_name(),
             namespace=result.get_name_space(),
             classname=result.get_class_name(),
+            is_flaky=result.get_is_flaky()
         )
 
     @staticmethod
     def test_result_to_testrun_result_post_model(
         result, external_id: str, configuration_id: str
     ):
         return AutoTestResultsForTestRunModel(
```

### Comparing `testit-cli-0.1.4/src/testit_cli/importer.py` & `testit-cli-0.1.5/src/testit_cli/importer.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,14 +28,16 @@
             if not autotest:
                 self.__api_client.create_autotest(
                     Converter.test_result_to_autotest_post_model(
                         result, external_id, self.__config.get_project_id()
                     )
                 )
             else:
+                result.set_is_flaky(autotest[0]['is_flaky'])
+
                 self.__api_client.update_autotest(
                     Converter.test_result_to_autotest_put_model(
                         result, external_id, self.__config.get_project_id()
                     )
                 )
 
             self.__api_client.send_test_result(
```

### Comparing `testit-cli-0.1.4/src/testit_cli/models/testcase.py` & `testit-cli-0.1.5/src/testit_cli/models/testcase.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     __name: str = None
     __name_space: str = None
     __class_name: str = None
     __duration: timedelta = None
     __status: Status = None
     __message: str = None
     __trace: str = None
+    __is_flaky: bool = None
 
     def __init__(self, name, name_space, class_name, duration):
         self.__name = name
         self.__name_space = name_space
         self.__class_name = class_name
         self.__duration = timedelta(seconds=float(duration))
         self.__status = Status.PASSED
@@ -46,7 +47,13 @@
         self.__trace = value
 
     def get_status(self):
         return AvailableTestResultOutcome(self.__status.value)
 
     def set_status(self, value: Status):
         self.__status = value
+
+    def get_is_flaky(self) -> bool:
+        return self.__is_flaky
+
+    def set_is_flaky(self, value: bool):
+        self.__is_flaky = value
```

### Comparing `testit-cli-0.1.4/src/testit_cli/parser.py` & `testit-cli-0.1.5/src/testit_cli/parser.py`

 * *Files identical despite different names*

### Comparing `testit-cli-0.1.4/src/testit_cli/service.py` & `testit-cli-0.1.5/src/testit_cli/service.py`

 * *Files identical despite different names*

### Comparing `testit-cli-0.1.4/src/testit_cli.egg-info/PKG-INFO` & `testit-cli-0.1.5/src/testit_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testit-cli
-Version: 0.1.4
+Version: 0.1.5
 Summary: This tool is the command line wrapper of Test IT allowing you to upload the test results in real time to Test IT
 Home-page: https://pypi.org/project/testit/
 Author: Integration team
 Author-email: integrations@testit.software
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `testit-cli-0.1.4/src/testit_cli.egg-info/SOURCES.txt` & `testit-cli-0.1.5/src/testit_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

