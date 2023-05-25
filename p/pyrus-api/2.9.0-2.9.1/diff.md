# Comparing `tmp/pyrus-api-2.9.0.tar.gz` & `tmp/pyrus-api-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrus-api-2.9.0.tar", last modified: Fri Apr 29 12:09:08 2022, max compression
+gzip compressed data, was "pyrus-api-2.9.1.tar", last modified: Fri Jun  3 13:26:46 2022, max compression
```

## Comparing `pyrus-api-2.9.0.tar` & `pyrus-api-2.9.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2022-04-29 12:09:08.928382 pyrus-api-2.9.0/
--rw-rw-rw-   0        0        0     1083 2021-12-28 09:57:19.000000 pyrus-api-2.9.0/LICENSE.txt
--rw-rw-rw-   0        0        0     4409 2022-04-29 12:09:08.928382 pyrus-api-2.9.0/PKG-INFO
--rw-rw-rw-   0        0        0     4026 2022-04-29 12:08:55.000000 pyrus-api-2.9.0/README.rst
-drwxrwxrwx   0        0        0        0 2022-04-29 12:09:08.906442 pyrus-api-2.9.0/pyrus/
--rw-rw-rw-   0        0        0       30 2021-12-28 09:57:19.000000 pyrus-api-2.9.0/pyrus/__init__.py
--rw-rw-rw-   0        0        0    22896 2022-04-29 11:27:51.000000 pyrus-api-2.9.0/pyrus/client.py
-drwxrwxrwx   0        0        0        0 2022-04-29 12:09:08.914445 pyrus-api-2.9.0/pyrus/models/
--rw-rw-rw-   0        0        0        0 2021-12-28 09:57:19.000000 pyrus-api-2.9.0/pyrus/models/__init__.py
--rw-rw-rw-   0        0        0       88 2021-12-28 09:57:19.000000 pyrus-api-2.9.0/pyrus/models/constants.py
--rw-rw-rw-   0        0        0     1522 2021-12-28 09:57:19.000000 pyrus-api-2.9.0/pyrus/models/customhandlers.py
--rw-rw-rw-   0        0        0    47285 2022-04-29 11:27:51.000000 pyrus-api-2.9.0/pyrus/models/entities.py
--rw-rw-rw-   0        0        0    37411 2022-04-29 11:27:51.000000 pyrus-api-2.9.0/pyrus/models/requests.py
--rw-rw-rw-   0        0        0    13722 2022-04-29 11:27:51.000000 pyrus-api-2.9.0/pyrus/models/responses.py
-drwxrwxrwx   0        0        0        0 2022-04-29 12:09:08.926389 pyrus-api-2.9.0/pyrus_api.egg-info/
--rw-rw-rw-   0        0        0     4409 2022-04-29 12:09:08.000000 pyrus-api-2.9.0/pyrus_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      415 2022-04-29 12:09:08.000000 pyrus-api-2.9.0/pyrus_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-04-29 12:09:08.000000 pyrus-api-2.9.0/pyrus_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2022-04-29 12:09:08.000000 pyrus-api-2.9.0/pyrus_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2022-04-29 12:09:08.000000 pyrus-api-2.9.0/pyrus_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2021-12-28 09:58:22.000000 pyrus-api-2.9.0/pyrus_api.egg-info/zip-safe
--rw-rw-rw-   0        0        0       42 2022-04-29 12:09:08.928382 pyrus-api-2.9.0/setup.cfg
--rw-rw-rw-   0        0        0      690 2022-04-29 11:27:51.000000 pyrus-api-2.9.0/setup.py
+drwxrwxrwx   0        0        0        0 2022-06-03 13:26:46.042850 pyrus-api-2.9.1/
+-rw-rw-rw-   0        0        0     1083 2022-05-31 22:24:16.000000 pyrus-api-2.9.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     4409 2022-06-03 13:26:46.041845 pyrus-api-2.9.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4026 2022-05-31 22:24:16.000000 pyrus-api-2.9.1/README.rst
+drwxrwxrwx   0        0        0        0 2022-06-03 13:26:46.036821 pyrus-api-2.9.1/pyrus/
+-rw-rw-rw-   0        0        0       30 2022-05-31 22:24:16.000000 pyrus-api-2.9.1/pyrus/__init__.py
+-rw-rw-rw-   0        0        0    22888 2022-06-03 13:26:44.000000 pyrus-api-2.9.1/pyrus/client.py
+drwxrwxrwx   0        0        0        0 2022-06-03 13:26:46.039845 pyrus-api-2.9.1/pyrus/models/
+-rw-rw-rw-   0        0        0        0 2022-05-31 22:24:16.000000 pyrus-api-2.9.1/pyrus/models/__init__.py
+-rw-rw-rw-   0        0        0       88 2022-05-31 22:24:16.000000 pyrus-api-2.9.1/pyrus/models/constants.py
+-rw-rw-rw-   0        0        0     1522 2022-05-31 22:24:16.000000 pyrus-api-2.9.1/pyrus/models/customhandlers.py
+-rw-rw-rw-   0        0        0    47285 2022-05-31 22:24:16.000000 pyrus-api-2.9.1/pyrus/models/entities.py
+-rw-rw-rw-   0        0        0    37411 2022-05-31 22:24:16.000000 pyrus-api-2.9.1/pyrus/models/requests.py
+-rw-rw-rw-   0        0        0    13722 2022-05-31 22:24:16.000000 pyrus-api-2.9.1/pyrus/models/responses.py
+drwxrwxrwx   0        0        0        0 2022-06-03 13:26:46.041845 pyrus-api-2.9.1/pyrus_api.egg-info/
+-rw-rw-rw-   0        0        0     4409 2022-06-03 13:26:45.000000 pyrus-api-2.9.1/pyrus_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      415 2022-06-03 13:26:45.000000 pyrus-api-2.9.1/pyrus_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-06-03 13:26:45.000000 pyrus-api-2.9.1/pyrus_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2022-06-03 13:26:45.000000 pyrus-api-2.9.1/pyrus_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2022-06-03 13:26:45.000000 pyrus-api-2.9.1/pyrus_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2022-05-31 22:24:17.000000 pyrus-api-2.9.1/pyrus_api.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       42 2022-06-03 13:26:46.042850 pyrus-api-2.9.1/setup.cfg
+-rw-rw-rw-   0        0        0      690 2022-06-03 13:26:44.000000 pyrus-api-2.9.1/setup.py
```

### Comparing `pyrus-api-2.9.0/LICENSE.txt` & `pyrus-api-2.9.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyrus-api-2.9.0/PKG-INFO` & `pyrus-api-2.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrus-api
-Version: 2.9.0
+Version: 2.9.1
 Summary: Python Pyrus API client
 Home-page: https://pyrus.com/en/help/api
 Author: Pyrus
 Author-email: contact@pyrus.com
 License: MIT License
 Project-URL: GitHub Project, https://github.com/simplygoodsoftware/pyrusapi-python
 Keywords: pyrus api
```

### Comparing `pyrus-api-2.9.0/README.rst` & `pyrus-api-2.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `pyrus-api-2.9.0/pyrus/client.py` & `pyrus-api-2.9.1/pyrus/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         PUT = "PUT"
 
     _host = 'api.pyrus.com'
     _base_path = '/v4'
     access_token = None
     _protocol = 'https'
     _api_name = 'Pyrus'
-    _user_agent = 'Pyrus API python client v 2.9.0'
+    _user_agent = 'Pyrus API python client v 2.9.1'
     proxy = None
     _download_file_base_url = 'https://files.pyrus.com/services/attachment?Id='
 
     def __init__(self, login=None, security_key=None, access_token=None, proxy=None):
         self.security_key = security_key
         self.access_token = access_token
         self.login = login
@@ -320,26 +320,26 @@
         Get all tasks in the list.
 
         Args:
             list_id (:obj:`int`): List id
             task_list_request (:obj:`models.requests.TaskListRequest`, optional): Request filters.
 
         Returns: 
-            class:`models.responses.FormRegisterResponse` object
+            class:`models.responses.TaskListResponse` object
         """
         url = self._create_url('/lists/{}/tasks'.format(list_id))
         if task_list_request:
             if not isinstance(task_list_request, req.TaskListRequest):
                 raise TypeError('task_list_request must be an instance '
                                 'of models.requests.TaskListRequest')
             response = self._perform_post_request(url, task_list_request)
         else:
             response = self._perform_get_request(url)
 
-        return resp.FormRegisterResponse(**response)
+        return resp.TaskListResponse(**response)
 
     def download_file(self, file_id):
         """
         Download the file.
 
         Args:
             file_id (:obj:`int`): File id
```

### Comparing `pyrus-api-2.9.0/pyrus/models/customhandlers.py` & `pyrus-api-2.9.1/pyrus/models/customhandlers.py`

 * *Files identical despite different names*

### Comparing `pyrus-api-2.9.0/pyrus/models/entities.py` & `pyrus-api-2.9.1/pyrus/models/entities.py`

 * *Files identical despite different names*

### Comparing `pyrus-api-2.9.0/pyrus/models/requests.py` & `pyrus-api-2.9.1/pyrus/models/requests.py`

 * *Files identical despite different names*

### Comparing `pyrus-api-2.9.0/pyrus/models/responses.py` & `pyrus-api-2.9.1/pyrus/models/responses.py`

 * *Files identical despite different names*

### Comparing `pyrus-api-2.9.0/pyrus_api.egg-info/PKG-INFO` & `pyrus-api-2.9.1/pyrus_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrus-api
-Version: 2.9.0
+Version: 2.9.1
 Summary: Python Pyrus API client
 Home-page: https://pyrus.com/en/help/api
 Author: Pyrus
 Author-email: contact@pyrus.com
 License: MIT License
 Project-URL: GitHub Project, https://github.com/simplygoodsoftware/pyrusapi-python
 Keywords: pyrus api
```

### Comparing `pyrus-api-2.9.0/setup.py` & `pyrus-api-2.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 from setuptools import setup, find_packages
 
 setup(name="pyrus-api",
-      version="2.9.0",
+      version="2.9.1",
       python_requires='>=3.4',
       description="Python Pyrus API client",
       author="Pyrus",
       long_description=open('README.rst', 'r').read(),
       author_email="contact@pyrus.com",
       url="https://pyrus.com/en/help/api",
       project_urls={
```

