# Comparing `tmp/testgear-importer-allure-1.3.1.tar.gz` & `tmp/testgear-importer-allure-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testgear-importer-allure-1.3.1.tar", last modified: Thu Apr 20 14:05:16 2023, max compression
+gzip compressed data, was "testgear-importer-allure-1.3.2.tar", last modified: Thu May 25 11:34:58 2023, max compression
```

## Comparing `testgear-importer-allure-1.3.1.tar` & `testgear-importer-allure-1.3.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 dmitry.gridnev (1970307760) TESTIT\Пользователи домена (1761955536)        0 2023-04-20 14:05:16.681979 testgear-importer-allure-1.3.1/
--rw-r--r--   0 dmitry.gridnev (1970307760) TESTIT\Пользователи домена (1761955536)     2893 2023-04-20 14:05:16.681839 testgear-importer-allure-1.3.1/PKG-INFO
--rw-r--r--   0 dmitry.gridnev (1970307760) TESTIT\Пользователи домена (1761955536)     2384 2023-01-20 12:57:55.000000 testgear-importer-allure-1.3.1/README.md
--rw-r--r--   0 dmitry.gridnev (1970307760) TESTIT\Пользователи домена (1761955536)      231 2023-01-20 12:57:55.000000 testgear-importer-allure-1.3.1/connection_config.ini
--rw-r--r--   0 dmitry.gridnev (1970307760) TESTIT\Пользователи домена (1761955536)       38 2023-04-20 14:05:16.682020 testgear-importer-allure-1.3.1/setup.cfg
--rw-r--r--   0 dmitry.gridnev (1970307760) TESTIT\Пользователи домена (1761955536)     1225 2023-04-20 14:00:51.000000 testgear-importer-allure-1.3.1/setup.py
-drwxr-xr-x   0 dmitry.gridnev (1970307760) TESTIT\Пользователи домена (1761955536)        0 2023-04-20 14:05:16.680469 testgear-importer-allure-1.3.1/src/
--rw-r--r--   0 dmitry.gridnev (1970307760) TESTIT\Пользователи домена (1761955536)        0 2022-09-01 11:13:09.000000 testgear-importer-allure-1.3.1/src/__init__.py
--rw-r--r--   0 dmitry.gridnev (1970307760) TESTIT\Пользователи домена (1761955536)     1268 2023-01-20 12:57:55.000000 testgear-importer-allure-1.3.1/src/__main__.py
--rw-r--r--   0 dmitry.gridnev (1970307760) TESTIT\Пользователи домена (1761955536)     3681 2023-01-20 12:57:55.000000 testgear-importer-allure-1.3.1/src/apiclient.py
--rw-r--r--   0 dmitry.gridnev (1970307760) TESTIT\Пользователи домена (1761955536)    11733 2023-04-20 14:00:15.000000 testgear-importer-allure-1.3.1/src/configurator.py
--rw-r--r--   0 dmitry.gridnev (1970307760) TESTIT\Пользователи домена (1761955536)     7176 2023-04-20 14:00:15.000000 testgear-importer-allure-1.3.1/src/converter.py
--rw-r--r--   0 dmitry.gridnev (1970307760) TESTIT\Пользователи домена (1761955536)      253 2023-01-20 12:57:55.000000 testgear-importer-allure-1.3.1/src/filedto.py
--rw-r--r--   0 dmitry.gridnev (1970307760) TESTIT\Пользователи домена (1761955536)     1557 2023-04-20 14:00:39.000000 testgear-importer-allure-1.3.1/src/filereader.py
--rw-r--r--   0 dmitry.gridnev (1970307760) TESTIT\Пользователи домена (1761955536)    11405 2023-04-20 14:00:15.000000 testgear-importer-allure-1.3.1/src/importer.py
--rw-r--r--   0 dmitry.gridnev (1970307760) TESTIT\Пользователи домена (1761955536)     1615 2023-01-20 12:57:55.000000 testgear-importer-allure-1.3.1/src/minioreader.py
--rw-r--r--   0 dmitry.gridnev (1970307760) TESTIT\Пользователи домена (1761955536)     2588 2023-01-20 12:57:55.000000 testgear-importer-allure-1.3.1/src/parser.py
--rw-r--r--   0 dmitry.gridnev (1970307760) TESTIT\Пользователи домена (1761955536)      885 2023-01-20 12:57:55.000000 testgear-importer-allure-1.3.1/src/rabbitmq.py
--rw-r--r--   0 dmitry.gridnev (1970307760) TESTIT\Пользователи домена (1761955536)      281 2023-01-20 12:57:55.000000 testgear-importer-allure-1.3.1/src/reader.py
-drwxr-xr-x   0 dmitry.gridnev (1970307760) TESTIT\Пользователи домена (1761955536)        0 2023-04-20 14:05:16.681647 testgear-importer-allure-1.3.1/testgear_importer_allure.egg-info/
--rw-r--r--   0 dmitry.gridnev (1970307760) TESTIT\Пользователи домена (1761955536)     2893 2023-04-20 14:05:16.000000 testgear-importer-allure-1.3.1/testgear_importer_allure.egg-info/PKG-INFO
--rw-r--r--   0 dmitry.gridnev (1970307760) TESTIT\Пользователи домена (1761955536)      535 2023-04-20 14:05:16.000000 testgear-importer-allure-1.3.1/testgear_importer_allure.egg-info/SOURCES.txt
--rw-r--r--   0 dmitry.gridnev (1970307760) TESTIT\Пользователи домена (1761955536)        1 2023-04-20 14:05:16.000000 testgear-importer-allure-1.3.1/testgear_importer_allure.egg-info/dependency_links.txt
--rw-r--r--   0 dmitry.gridnev (1970307760) TESTIT\Пользователи домена (1761955536)      144 2023-04-20 14:05:16.000000 testgear-importer-allure-1.3.1/testgear_importer_allure.egg-info/entry_points.txt
--rw-r--r--   0 dmitry.gridnev (1970307760) TESTIT\Пользователи домена (1761955536)       65 2023-04-20 14:05:16.000000 testgear-importer-allure-1.3.1/testgear_importer_allure.egg-info/requires.txt
--rw-r--r--   0 dmitry.gridnev (1970307760) TESTIT\Пользователи домена (1761955536)       25 2023-04-20 14:05:16.000000 testgear-importer-allure-1.3.1/testgear_importer_allure.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:34:58.826497 testgear-importer-allure-1.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-05-25 11:34:58.826497 testgear-importer-allure-1.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-05-25 11:34:47.000000 testgear-importer-allure-1.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-25 11:34:47.000000 testgear-importer-allure-1.3.2/connection_config.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 11:34:58.826497 testgear-importer-allure-1.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-05-25 11:34:47.000000 testgear-importer-allure-1.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:34:58.822497 testgear-importer-allure-1.3.2/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 11:34:47.000000 testgear-importer-allure-1.3.2/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-05-25 11:34:47.000000 testgear-importer-allure-1.3.2/src/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-05-25 11:34:47.000000 testgear-importer-allure-1.3.2/src/apiclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12592 2023-05-25 11:34:47.000000 testgear-importer-allure-1.3.2/src/configurator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7222 2023-05-25 11:34:47.000000 testgear-importer-allure-1.3.2/src/converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-25 11:34:47.000000 testgear-importer-allure-1.3.2/src/filedto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-05-25 11:34:47.000000 testgear-importer-allure-1.3.2/src/filereader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11469 2023-05-25 11:34:47.000000 testgear-importer-allure-1.3.2/src/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-05-25 11:34:47.000000 testgear-importer-allure-1.3.2/src/minioreader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-05-25 11:34:47.000000 testgear-importer-allure-1.3.2/src/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-05-25 11:34:47.000000 testgear-importer-allure-1.3.2/src/rabbitmq.py
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-25 11:34:47.000000 testgear-importer-allure-1.3.2/src/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:34:58.822497 testgear-importer-allure-1.3.2/testgear_importer_allure.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-05-25 11:34:58.000000 testgear-importer-allure-1.3.2/testgear_importer_allure.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-25 11:34:58.000000 testgear-importer-allure-1.3.2/testgear_importer_allure.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 11:34:58.000000 testgear-importer-allure-1.3.2/testgear_importer_allure.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-25 11:34:58.000000 testgear-importer-allure-1.3.2/testgear_importer_allure.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-25 11:34:58.000000 testgear-importer-allure-1.3.2/testgear_importer_allure.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-25 11:34:58.000000 testgear-importer-allure-1.3.2/testgear_importer_allure.egg-info/top_level.txt
```

### Comparing `testgear-importer-allure-1.3.1/PKG-INFO` & `testgear-importer-allure-1.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testgear-importer-allure
-Version: 1.3.1
+Version: 1.3.2
 Summary: Allure report importer for TestGear
 Home-page: https://pypi.org/project/testgear-importer-allure/
 Author: Integration team
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `testgear-importer-allure-1.3.1/README.md` & `testgear-importer-allure-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `testgear-importer-allure-1.3.1/setup.py` & `testgear-importer-allure-1.3.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='testgear-importer-allure',
-    version='1.3.1',
+    version='1.3.2',
     description='Allure report importer for TestGear',
     long_description=open('README.md', "r").read(),
     long_description_content_type="text/markdown",
     url='https://pypi.org/project/testgear-importer-allure/',
     author='Integration team',
     license='Apache-2.0',
     classifiers=[
```

### Comparing `testgear-importer-allure-1.3.1/src/__main__.py` & `testgear-importer-allure-1.3.2/src/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,30 +11,30 @@
     config = Configurator()
 
     if config.get_path() is None:
         return
 
     reader = FileReader(config.get_path())
     parser = Parser(reader)
-    api_client = ApiClient(config.get_url(), config.get_private_token())
+    api_client = ApiClient(config.get_url(), config.get_private_token(), config.get_cert_validation())
 
     importer = Importer(parser, api_client, config)
     importer.send_result()
 
 
 def consumer_main():
     config = Configurator()
     rabbitmq = RabbitMQ(config.get_rabbitmq_url(), config.get_rabbitmq_user(), config.get_rabbitmq_password(),
                         config.get_rabbitmq_exchange())
 
     def callback(ch, method, properties, body):
         reader = MinioReader(config.get_minio_url(), config.get_minio_access_key(), config.get_minio_secret_key(),
                              body.decode("utf-8"))
         parser = Parser(reader)
-        api_client = ApiClient(config.get_url(), config.get_private_token())
+        api_client = ApiClient(config.get_url(), config.get_private_token(), config.get_cert_validation())
 
         importer = Importer(parser, api_client, config)
         importer.send_result()
 
     rabbitmq.consume(callback)
```

### Comparing `testgear-importer-allure-1.3.1/src/apiclient.py` & `testgear-importer-allure-1.3.2/src/apiclient.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,17 +13,22 @@
 from testgear_api_client.apis import AttachmentsApi
 
 from .converter import Converter
 
 
 class ApiClient:
     """Class representing a api client"""
-    def __init__(self, url: str, token: str):
+    def __init__(self, url: str, token: str, cert_validation: str):
+        client_config = Configuration(host=url)
+
+        if cert_validation == 'false':
+            client_config.verify_ssl = False
+
         client = TmsClient(
-            configuration=Configuration(host=url),
+            configuration=client_config,
             header_name='Authorization',
             header_value='PrivateToken ' + token
         )
         logging.basicConfig(format='%(levelname)s:%(message)s', level=logging.INFO)
         self.__test_run_api = TestRunsApi(api_client=client)
         self.__autotest_api = AutoTestsApi(api_client=client)
         self.__attachments_api = AttachmentsApi(api_client=client)
```

### Comparing `testgear-importer-allure-1.3.1/src/configurator.py` & `testgear-importer-allure-1.3.2/src/configurator.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import re
 
 CONFIG_SECTION = 'testgear'
 CONFIG_URL = 'url'
 CONFIG_PRIVATE_TOKEN = 'privateToken'
 CONFIG_PROJECT_ID = 'projectID'
 CONFIG_CONFIGURATION_ID = 'configurationID'
+CONFIG_CERT_VALIDATION = 'certValidation'
 CONFIG_NAME = 'connection_config.ini'
 
 RABBITMQ_CONFIG_SECTION = 'rabbitmq'
 RABBITMQ_CONFIG_URL = 'host'
 RABBITMQ_CONFIG_USER = 'user'
 RABBITMQ_CONFIG_PASSWORD = 'password'
 RABBITMQ_CONFIG_EXCHANGE = 'exchange'
@@ -52,14 +53,21 @@
         """Function returns project id."""
         return self.config.get(CONFIG_SECTION, CONFIG_PROJECT_ID)
 
     def get_configuration_id(self):
         """Function returns configuration id."""
         return self.config.get(CONFIG_SECTION, CONFIG_CONFIGURATION_ID)
 
+    def get_cert_validation(self):
+        """Function returns cert validation."""
+        if not self.config.has_option(CONFIG_SECTION, CONFIG_CERT_VALIDATION):
+            return
+
+        return self.config.get(CONFIG_SECTION, CONFIG_CERT_VALIDATION)
+
     def get_rabbitmq_url(self):
         """Function returns rabbit mq url."""
         return self.config.get(RABBITMQ_CONFIG_SECTION, RABBITMQ_CONFIG_URL)
 
     def get_rabbitmq_user(self):
         """Function returns rabbit mq user."""
         return self.config.get(RABBITMQ_CONFIG_SECTION, RABBITMQ_CONFIG_USER)
@@ -131,14 +139,22 @@
             '--testrunid',
             action="store",
             dest="set_testrun",
             metavar="3802f329-190c-4617-8bb0-2c3696abeb8f",
             help='Set test run ID'
         )
         self.parser.add_argument(
+            '-cv',
+            '--certvalidation',
+            action="store",
+            dest="set_cert_validation",
+            metavar="false",
+            help='Enables/disables certificate validation'
+        )
+        self.parser.add_argument(
             '-sh',
             '--show',
             action='store_true',
             dest="show_settings",
             help='Show the connection_config.ini file'
         )
         self.parser.add_argument(
@@ -223,14 +239,17 @@
 
         if 'TMS_PROJECT_ID' in os.environ.keys():
             self.config.set(CONFIG_SECTION, CONFIG_PROJECT_ID, os.environ.get('TMS_PROJECT_ID'))
 
         if 'TMS_CONFIGURATION_ID' in os.environ.keys():
             self.config.set(CONFIG_SECTION, CONFIG_CONFIGURATION_ID, os.environ.get('TMS_CONFIGURATION_ID'))
 
+        if f'TMS_CERT_VALIDATION' in os.environ.keys():
+            self.config.set(CONFIG_SECTION, CONFIG_CERT_VALIDATION, os.environ.get('TMS_CERT_VALIDATION').lower())
+
         if 'MINIO_API_HOST' in os.environ.keys():
             self.config.set(MINIO_CONFIG_SECTION, MINIO_CONFIG_URL, os.environ.get('MINIO_API_HOST'))
 
         if 'MINIO_ACCESS_KEY' in os.environ.keys():
             self.config.set(MINIO_CONFIG_SECTION, MINIO_CONFIG_ACCESS_KEY, os.environ.get('MINIO_ACCESS_KEY'))
 
         if 'MINIO_SECRET_KEY' in os.environ.keys():
@@ -283,14 +302,17 @@
             if not re.fullmatch(r'[a-zA-Z\d]{8}-[a-zA-Z\d]{4}-[a-zA-Z\d]{4}-[a-zA-Z\d]{4}-[a-zA-Z\d]{12}',
                                 args.set_testrun):
                 print('The wrong testrun ID!')
                 raise SystemExit
 
             self.specified_testrun = args.set_testrun
 
+        if args.set_cert_validation:
+            self.config.set(CONFIG_SECTION, CONFIG_CERT_VALIDATION, args.set_cert_validation.lower())
+
         if args.alluredir:
             self.path_to_results = args.alluredir
 
         if args.set_rabbitmqhost:
             self.config.set(RABBITMQ_CONFIG_SECTION, RABBITMQ_CONFIG_URL, args.set_rabbitmqhost)
 
         if args.set_rabbitmquser:
```

### Comparing `testgear-importer-allure-1.3.1/src/converter.py` & `testgear-importer-allure-1.3.2/src/converter.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,16 @@
             steps=cls.step_results_to_autotest_steps_model(test_result['steps']),
             setup=cls.step_results_to_autotest_steps_model(test_result['setup']),
             teardown=cls.step_results_to_autotest_steps_model(test_result['teardown']),
             namespace=test_result['namespace'],
             classname=test_result['classname'],
             description=test_result['description'],
             links=cls.links_to_links_put_model(test_result['links']),
-            labels=test_result['labels']
+            labels=test_result['labels'],
+            is_flaky=test_result['is_flaky']
         )
 
     @classmethod
     def test_result_to_testrun_result_post_model(
             cls,
             test_result: dict,
             configuration_id: str):
```

### Comparing `testgear-importer-allure-1.3.1/src/filereader.py` & `testgear-importer-allure-1.3.2/src/filereader.py`

 * *Files identical despite different names*

### Comparing `testgear-importer-allure-1.3.1/src/importer.py` & `testgear-importer-allure-1.3.2/src/importer.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,14 +61,16 @@
                 autotest_id = self.__api_client.create_autotest(
                     Converter.test_result_to_autotest_post_model(test, self.__project_id)
                 )
             else:
                 autotest_id = autotest[0]['id']
 
                 if test['outcome'] == 'Passed':
+                    test['is_flaky'] = autotest[0]['is_flaky']
+
                     self.__api_client.update_autotest(
                         Converter.test_result_to_autotest_put_model(test, self.__project_id)
                     )
                 else:
                     autotest[0]['links'] = test['links']
 
                     for i in range(0, len(autotest[0]['labels'])):
```

### Comparing `testgear-importer-allure-1.3.1/src/minioreader.py` & `testgear-importer-allure-1.3.2/src/minioreader.py`

 * *Files identical despite different names*

### Comparing `testgear-importer-allure-1.3.1/src/parser.py` & `testgear-importer-allure-1.3.2/src/parser.py`

 * *Files identical despite different names*

### Comparing `testgear-importer-allure-1.3.1/src/rabbitmq.py` & `testgear-importer-allure-1.3.2/src/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `testgear-importer-allure-1.3.1/testgear_importer_allure.egg-info/PKG-INFO` & `testgear-importer-allure-1.3.2/testgear_importer_allure.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testgear-importer-allure
-Version: 1.3.1
+Version: 1.3.2
 Summary: Allure report importer for TestGear
 Home-page: https://pypi.org/project/testgear-importer-allure/
 Author: Integration team
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `testgear-importer-allure-1.3.1/testgear_importer_allure.egg-info/SOURCES.txt` & `testgear-importer-allure-1.3.2/testgear_importer_allure.egg-info/SOURCES.txt`

 * *Files identical despite different names*

