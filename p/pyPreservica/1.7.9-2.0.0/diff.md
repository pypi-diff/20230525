# Comparing `tmp/pyPreservica-1.7.9.tar.gz` & `tmp/pyPreservica-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyPreservica-1.7.9.tar", last modified: Wed May 24 09:28:40 2023, max compression
+gzip compressed data, was "pyPreservica-2.0.0.tar", last modified: Thu May 25 10:12:51 2023, max compression
```

## Comparing `pyPreservica-1.7.9.tar` & `pyPreservica-2.0.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 09:28:40.245142 pyPreservica-1.7.9/
--rw-rw-rw-   0        0        0    11558 2020-08-17 10:38:19.000000 pyPreservica-1.7.9/LICENSE.txt
--rw-rw-rw-   0        0        0     2581 2023-05-24 09:28:40.245142 pyPreservica-1.7.9/PKG-INFO
--rw-rw-rw-   0        0        0     1602 2022-03-16 17:04:00.000000 pyPreservica-1.7.9/README.md
-drwxrwxrwx   0        0        0        0 2023-05-24 09:28:40.198273 pyPreservica-1.7.9/pyPreservica/
--rw-rw-rw-   0        0        0     1096 2023-05-24 08:23:27.000000 pyPreservica-1.7.9/pyPreservica/__init__.py
--rw-rw-rw-   0        0        0    37685 2023-05-03 10:58:47.000000 pyPreservica-1.7.9/pyPreservica/adminAPI.py
--rw-rw-rw-   0        0        0    32269 2023-05-03 10:51:09.000000 pyPreservica-1.7.9/pyPreservica/common.py
--rw-rw-rw-   0        0        0    16189 2023-03-01 16:04:47.000000 pyPreservica-1.7.9/pyPreservica/contentAPI.py
--rw-rw-rw-   0        0        0   105699 2023-05-24 08:44:58.000000 pyPreservica-1.7.9/pyPreservica/entityAPI.py
--rw-rw-rw-   0        0        0     6258 2023-05-16 11:37:54.000000 pyPreservica-1.7.9/pyPreservica/monitorAPI.py
--rw-rw-rw-   0        0        0     4875 2022-04-21 08:22:10.000000 pyPreservica-1.7.9/pyPreservica/opex.py
--rw-rw-rw-   0        0        0    10522 2021-11-17 14:16:50.000000 pyPreservica-1.7.9/pyPreservica/parAPI.py
--rw-rw-rw-   0        0        0    23544 2023-05-16 16:46:33.000000 pyPreservica-1.7.9/pyPreservica/retentionAPI.py
--rw-rw-rw-   0        0        0    92445 2023-05-16 11:37:54.000000 pyPreservica-1.7.9/pyPreservica/uploadAPI.py
--rw-rw-rw-   0        0        0     5496 2023-05-17 12:28:12.000000 pyPreservica-1.7.9/pyPreservica/vocabularyAPI.py
--rw-rw-rw-   0        0        0     6736 2023-05-24 08:15:02.000000 pyPreservica-1.7.9/pyPreservica/webHooksAPI.py
--rw-rw-rw-   0        0        0    17812 2023-03-01 16:08:31.000000 pyPreservica-1.7.9/pyPreservica/workflowAPI.py
-drwxrwxrwx   0        0        0        0 2023-05-24 09:28:40.229520 pyPreservica-1.7.9/pyPreservica.egg-info/
--rw-rw-rw-   0        0        0     2581 2023-05-24 09:28:38.000000 pyPreservica-1.7.9/pyPreservica.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      547 2023-05-24 09:28:38.000000 pyPreservica-1.7.9/pyPreservica.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 09:28:38.000000 pyPreservica-1.7.9/pyPreservica.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-05-24 09:28:38.000000 pyPreservica-1.7.9/pyPreservica.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-24 09:28:38.000000 pyPreservica-1.7.9/pyPreservica.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-24 09:28:40.245142 pyPreservica-1.7.9/setup.cfg
--rw-rw-rw-   0        0        0     1645 2023-05-24 08:23:27.000000 pyPreservica-1.7.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-25 10:12:51.060487 pyPreservica-2.0.0/
+-rw-rw-rw-   0        0        0    11558 2020-08-17 10:38:19.000000 pyPreservica-2.0.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     2581 2023-05-25 10:12:51.060487 pyPreservica-2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1602 2022-03-16 17:04:00.000000 pyPreservica-2.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-25 10:12:50.980868 pyPreservica-2.0.0/pyPreservica/
+-rw-rw-rw-   0        0        0     1096 2023-05-24 17:35:07.000000 pyPreservica-2.0.0/pyPreservica/__init__.py
+-rw-rw-rw-   0        0        0    37685 2023-05-03 10:58:47.000000 pyPreservica-2.0.0/pyPreservica/adminAPI.py
+-rw-rw-rw-   0        0        0    34857 2023-05-25 09:06:15.000000 pyPreservica-2.0.0/pyPreservica/common.py
+-rw-rw-rw-   0        0        0    16257 2023-05-24 17:32:04.000000 pyPreservica-2.0.0/pyPreservica/contentAPI.py
+-rw-rw-rw-   0        0        0   105700 2023-05-25 09:37:03.000000 pyPreservica-2.0.0/pyPreservica/entityAPI.py
+-rw-rw-rw-   0        0        0     6258 2023-05-16 11:37:54.000000 pyPreservica-2.0.0/pyPreservica/monitorAPI.py
+-rw-rw-rw-   0        0        0     4875 2022-04-21 08:22:10.000000 pyPreservica-2.0.0/pyPreservica/opex.py
+-rw-rw-rw-   0        0        0    10522 2021-11-17 14:16:50.000000 pyPreservica-2.0.0/pyPreservica/parAPI.py
+-rw-rw-rw-   0        0        0    23612 2023-05-24 17:32:04.000000 pyPreservica-2.0.0/pyPreservica/retentionAPI.py
+-rw-rw-rw-   0        0        0    92445 2023-05-24 11:33:15.000000 pyPreservica-2.0.0/pyPreservica/uploadAPI.py
+-rw-rw-rw-   0        0        0     5496 2023-05-17 12:28:12.000000 pyPreservica-2.0.0/pyPreservica/vocabularyAPI.py
+-rw-rw-rw-   0        0        0     6736 2023-05-24 08:15:02.000000 pyPreservica-2.0.0/pyPreservica/webHooksAPI.py
+-rw-rw-rw-   0        0        0    17862 2023-05-24 17:32:04.000000 pyPreservica-2.0.0/pyPreservica/workflowAPI.py
+drwxrwxrwx   0        0        0        0 2023-05-25 10:12:51.050608 pyPreservica-2.0.0/pyPreservica.egg-info/
+-rw-rw-rw-   0        0        0     2581 2023-05-25 10:12:49.000000 pyPreservica-2.0.0/pyPreservica.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      547 2023-05-25 10:12:49.000000 pyPreservica-2.0.0/pyPreservica.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 10:12:49.000000 pyPreservica-2.0.0/pyPreservica.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2023-05-25 10:12:49.000000 pyPreservica-2.0.0/pyPreservica.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-25 10:12:49.000000 pyPreservica-2.0.0/pyPreservica.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-25 10:12:51.070375 pyPreservica-2.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1654 2023-05-24 17:35:07.000000 pyPreservica-2.0.0/setup.py
```

### Comparing `pyPreservica-1.7.9/LICENSE.txt` & `pyPreservica-2.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyPreservica-1.7.9/PKG-INFO` & `pyPreservica-2.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyPreservica
-Version: 1.7.9
+Version: 2.0.0
 Summary: Python library for the Preservica API
 Home-page: https://pypreservica.readthedocs.io/
 Author: James Carr
 Author-email: drjamescarr@gmail.com
 License: Apache License 2.0
 Project-URL: Documentation, https://pypreservica.readthedocs.io
 Project-URL: Source, https://github.com/carj/pyPreservica
```

### Comparing `pyPreservica-1.7.9/README.md` & `pyPreservica-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `pyPreservica-1.7.9/pyPreservica/__init__.py` & `pyPreservica-2.0.0/pyPreservica/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,10 +19,10 @@
 from .webHooksAPI import WebHooksAPI, TriggerType, WebHookHandler
 from .vocabularyAPI import ControlledVocabularyAPI, Table
 
 
 __author__ = "James Carr (drjamescarr@gmail.com)"
 
 # Version of the Preservica API package
-__version__ = "1.7.9"
+__version__ = "2.0.0"
 
 __license__ = "Apache License Version 2.0"
```

### Comparing `pyPreservica-1.7.9/pyPreservica/adminAPI.py` & `pyPreservica-2.0.0/pyPreservica/adminAPI.py`

 * *Files identical despite different names*

### Comparing `pyPreservica-1.7.9/pyPreservica/common.py` & `pyPreservica-2.0.0/pyPreservica/common.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 import sys
 import threading
 import time
 import unicodedata
 import xml.etree.ElementTree
 from enum import Enum
 from pathlib import Path
+import pyotp
 
 import requests
 
 import pyPreservica
 
 logger = logging.getLogger(__name__)
 
@@ -708,15 +709,16 @@
                 self.admin_ns = f"{NS_ADMIN}/v{self.major_version}.{self.minor_version}"
 
     def __version_number__(self):
         """
         Determine the version number of the server
         """
         headers = {HEADER_TOKEN: self.token}
-        request = self.session.get(f'{self.protocol}://{self.server}/api/entity/versiondetails/version', headers=headers)
+        request = self.session.get(f'{self.protocol}://{self.server}/api/entity/versiondetails/version',
+                                   headers=headers)
         if request.status_code == requests.codes.ok:
             xml_ = str(request.content.decode('utf-8'))
             version = xml_[xml_.find("<CurrentVersion>") + len("<CurrentVersion>"):xml_.find("</CurrentVersion>")]
             version_numbers = version.split(".")
             self.major_version = int(version_numbers[0])
             self.minor_version = int(version_numbers[1])
             self.patch_version = int(version_numbers[2])
@@ -737,14 +739,17 @@
     def __repr__(self):
         return self.__str__()
 
     def save_config(self):
         config = configparser.RawConfigParser(interpolation=None)
         config['credentials'] = {'username': self.username, 'password': self.password, 'tenant': self.tenant,
                                  'server': self.server}
+        if self.two_fa_secret_key is not None:
+            config['credentials']['twoFactorToken'] = self.two_fa_secret_key
+
         with open('credentials.properties', 'wt', encoding="utf-8") as configfile:
             config.write(configfile)
 
     def manager_token(self, username: str, password: str):
         data = {'username': username, 'password': password, 'tenant': self.tenant}
         response = self.session.post(f'{self.protocol}://{self.server}/api/accesstoken/login', data=data)
         if response.status_code == requests.codes.ok:
@@ -765,14 +770,44 @@
                 data = {'username': self.username, 'password': self.password, 'tenant': self.tenant}
             response = self.session.post(f'{self.protocol}://{self.server}/api/accesstoken/login', data=data)
             if response.status_code == requests.codes.ok:
                 if self.tenant is None:
                     self.tenant = response.json()['tenant']
                 return response.json()['token']
             else:
+                if 'message' in response.json():
+                    if response.json()['message'] == "needs.2fa":
+                        logger.debug("2FA Found")
+                        if self.tenant is None:
+                            self.tenant = response.json()['tenant']
+                        if self.two_fa_secret_key:
+                            totp = pyotp.TOTP(self.two_fa_secret_key)
+                            data = {'username': self.username,
+                                    'continuationToken': response.json()['continuationToken'],
+                                    'tenant': self.tenant, 'twoFactorToken': totp.now()}
+                            response_2fa = self.session.post(
+                                f'{self.protocol}://{self.server}/api/accesstoken/complete-2fa',
+                                data=data)
+                            if response_2fa.status_code == requests.codes.ok:
+                                return response_2fa.json()['token']
+                            else:
+                                msg = "Failed to create a 2FA authentication token. Check your credentials are correct"
+                                logger.error(msg)
+                                logger.error(str(response.content))
+                                raise RuntimeError(response.status_code, msg)
+                        else:
+                            msg = "2FA twoFactorToken required to authenticate against this account using 2FA"
+                            logger.error(msg)
+                            logger.error(str(response.content))
+                            raise RuntimeError(response.status_code, msg)
+                    if response.json()['message'] == "needs.2fa.setup":
+                        msg = "2FA is activated but not yet set up"
+                        logger.error(msg)
+                        logger.error(str(response.content))
+                        raise RuntimeError(response.status_code, msg)
                 msg = "Failed to create a password based authentication token. Check your credentials are correct"
                 logger.error(msg)
                 logger.error(str(response.content))
                 raise RuntimeError(response.status_code, msg)
 
         if self.shared_secret is True:
             endpoint = "api/accesstoken/acquire-external"
@@ -786,22 +821,30 @@
                 return response.json()['token']
             else:
                 msg = "Failed to create a shared secret authentication token. Check your credentials are correct"
                 logger.error(msg)
                 raise RuntimeError(response.status_code, msg)
 
     def __init__(self, username: str = None, password: str = None, tenant: str = None, server: str = None,
-                 use_shared_secret: bool = False, protocol: str = "https"):
+                 use_shared_secret: bool = False, two_fa_secret_key: str = None, protocol: str = "https"):
 
         config = configparser.ConfigParser(interpolation=configparser.Interpolation())
         config.read('credentials.properties', encoding='utf-8')
         self.session = requests.Session()
         self.shared_secret = bool(use_shared_secret)
         self.protocol = protocol
 
+        if not two_fa_secret_key:
+            two_fa_secret_key = os.environ.get('PRESERVICA_2FA_TOKEN')
+            if two_fa_secret_key is None:
+                try:
+                    two_fa_secret_key = config['credentials']['twoFactorToken']
+                except KeyError:
+                    pass
+        self.two_fa_secret_key = two_fa_secret_key
         if not username:
             username = os.environ.get('PRESERVICA_USERNAME')
             if username is None:
                 try:
                     username = config['credentials']['username']
                 except KeyError:
                     pass
```

### Comparing `pyPreservica-1.7.9/pyPreservica/contentAPI.py` & `pyPreservica-2.0.0/pyPreservica/contentAPI.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,16 +14,17 @@
 from pyPreservica.common import *
 
 logger = logging.getLogger(__name__)
 
 
 class ContentAPI(AuthenticatedAPI):
 
-    def __init__(self, username=None, password=None, tenant=None, server=None, use_shared_secret=False, protocol: str = "https"):
-        super().__init__(username, password, tenant, server, use_shared_secret, protocol)
+    def __init__(self, username=None, password=None, tenant=None, server=None, use_shared_secret=False,
+                 two_fa_secret_key: str = None, protocol: str = "https"):
+        super().__init__(username, password, tenant, server, use_shared_secret, two_fa_secret_key, protocol)
         self.callback = None
 
     class SearchResult:
         def __init__(self, metadata, refs, hits, results_list, next_start):
             self.metadata = metadata
             self.refs = refs
             self.hits = int(hits)
```

### Comparing `pyPreservica-1.7.9/pyPreservica/entityAPI.py` & `pyPreservica-2.0.0/pyPreservica/entityAPI.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,16 +27,16 @@
 
             The EntityAPI allows users to interact with the Preservica repository
 
 
     """
 
     def __init__(self, username: str = None, password: str = None, tenant: str = None, server: str = None,
-                 use_shared_secret: bool = False, protocol: str = "https") -> object:
-        super().__init__(username, password, tenant, server, use_shared_secret, protocol)
+                 use_shared_secret: bool = False, two_fa_secret_key: str = None, protocol: str = "https"):
+        super().__init__(username, password, tenant, server, use_shared_secret, two_fa_secret_key, protocol)
         xml.etree.ElementTree.register_namespace("oai_dc", "http://www.openarchives.org/OAI/2.0/oai_dc/")
         xml.etree.ElementTree.register_namespace("ead", "urn:isbn:1-931666-22-9")
 
     def user_security_tags(self, with_permissions: bool = False) -> dict:
         """
              Return  security tags available for the  current user
 
@@ -1688,15 +1688,14 @@
         """
          Retrieve list of entities below a folder in the repository
 
          Returns list
 
          :param folder: The folder to find children of
          """
-        self.token = self.__token__()
         for entity in self.descendants(folder=folder):
             yield entity
             if entity.entity_type == EntityType.FOLDER:
                 yield from self.all_descendants(folder=entity)
 
     def descendants(self, folder: Union[str, Folder] = None) -> Generator:
         maximum = 100
```

### Comparing `pyPreservica-1.7.9/pyPreservica/monitorAPI.py` & `pyPreservica-2.0.0/pyPreservica/monitorAPI.py`

 * *Files identical despite different names*

### Comparing `pyPreservica-1.7.9/pyPreservica/opex.py` & `pyPreservica-2.0.0/pyPreservica/opex.py`

 * *Files identical despite different names*

### Comparing `pyPreservica-1.7.9/pyPreservica/parAPI.py` & `pyPreservica-2.0.0/pyPreservica/parAPI.py`

 * *Files identical despite different names*

### Comparing `pyPreservica-1.7.9/pyPreservica/retentionAPI.py` & `pyPreservica-2.0.0/pyPreservica/retentionAPI.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,16 +54,17 @@
 
     def __repr__(self):
         return self.__str__()
 
 
 class RetentionAPI(AuthenticatedAPI):
 
-    def __init__(self, username=None, password=None, tenant=None, server=None, use_shared_secret=False, protocol: str = "https"):
-        super().__init__(username, password, tenant, server, use_shared_secret, protocol)
+    def __init__(self, username=None, password=None, tenant=None, server=None, use_shared_secret=False,
+                 two_fa_secret_key: str = None, protocol: str = "https"):
+        super().__init__(username, password, tenant, server, use_shared_secret, two_fa_secret_key, protocol)
         if self.major_version < 7 and self.minor_version < 2:
             raise RuntimeError("Retention API is only available when connected to a v6.2 System")
 
     def policy(self, reference: str) -> RetentionPolicy:
         """
          Return a retention policy by reference
```

### Comparing `pyPreservica-1.7.9/pyPreservica/uploadAPI.py` & `pyPreservica-2.0.0/pyPreservica/uploadAPI.py`

 * *Files identical despite different names*

### Comparing `pyPreservica-1.7.9/pyPreservica/vocabularyAPI.py` & `pyPreservica-2.0.0/pyPreservica/vocabularyAPI.py`

 * *Files identical despite different names*

### Comparing `pyPreservica-1.7.9/pyPreservica/webHooksAPI.py` & `pyPreservica-2.0.0/pyPreservica/webHooksAPI.py`

 * *Files identical despite different names*

### Comparing `pyPreservica-1.7.9/pyPreservica/workflowAPI.py` & `pyPreservica-2.0.0/pyPreservica/workflowAPI.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,16 +95,16 @@
     """
 
     workflow_states = ['Aborted', 'Active', 'Completed', 'Finished_Mixed_Outcome', 'Pending', 'Suspended', 'Unknown',
                        'Failed']
     workflow_types = ['Ingest', 'Access', 'Transformation', 'DataManagement']
 
     def __init__(self, username: str = None, password: str = None, tenant: str = None, server: str = None,
-                 use_shared_secret: bool = False, protocol: str = "https"):
-        super().__init__(username, password, tenant, server, use_shared_secret, protocol)
+                 use_shared_secret: bool = False, two_fa_secret_key: str = None, protocol: str = "https"):
+        super().__init__(username, password, tenant, server, use_shared_secret, two_fa_secret_key, protocol)
         self.base_url = "sdb/rest/workflow"
 
     def get_workflow_contexts_by_type(self, workflow_type: str):
         """
         Return a list of Workflow Contexts which have the same Workflow type
 
         :param workflow_type: The Workflow type  Ingest, Access, Transformation or DataManagement
```

### Comparing `pyPreservica-1.7.9/pyPreservica.egg-info/PKG-INFO` & `pyPreservica-2.0.0/pyPreservica.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyPreservica
-Version: 1.7.9
+Version: 2.0.0
 Summary: Python library for the Preservica API
 Home-page: https://pypreservica.readthedocs.io/
 Author: James Carr
 Author-email: drjamescarr@gmail.com
 License: Apache License 2.0
 Project-URL: Documentation, https://pypreservica.readthedocs.io
 Project-URL: Source, https://github.com/carj/pyPreservica
```

### Comparing `pyPreservica-1.7.9/pyPreservica.egg-info/SOURCES.txt` & `pyPreservica-2.0.0/pyPreservica.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyPreservica-1.7.9/setup.py` & `pyPreservica-2.0.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     os.system('twine upload dist/*')
     sys.exit()
 
 
 # This call to setup() does all the work
 setup(
     name=PKG,
-    version="1.7.9",
+    version="2.0.0",
     description="Python library for the Preservica API",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://pypreservica.readthedocs.io/",
     author="James Carr",
     author_email="drjamescarr@gmail.com",
     license="Apache License 2.0",
@@ -37,14 +37,14 @@
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
         "Topic :: System :: Archiving",
     ],
     keywords='Preservica API Preservation',
-    install_requires=["requests", "certifi", "boto3", "botocore", "s3transfer", "azure-storage-blob", "tqdm"],
+    install_requires=["requests", "certifi", "boto3", "botocore", "s3transfer", "azure-storage-blob", "tqdm", "pyotp"],
     project_urls={
         'Documentation': 'https://pypreservica.readthedocs.io',
         'Source': 'https://github.com/carj/pyPreservica',
         'Discussion Forum': 'https://groups.google.com/g/pypreservica',
     }
 )
```

