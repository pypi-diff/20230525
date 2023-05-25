# Comparing `tmp/uptime_kuma_api-0.9.0.tar.gz` & `tmp/uptime_kuma_api-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/uptime_kuma_api-0.9.0.tar", last modified: Tue Jan 17 20:39:01 2023, max compression
+gzip compressed data, was "uptime_kuma_api-1.0.0.tar", last modified: Thu May 25 19:36:58 2023, max compression
```

## Comparing `uptime_kuma_api-0.9.0.tar` & `uptime_kuma_api-1.0.0.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 lucas     (1000) users      (985)        0 2023-01-17 20:39:01.000000 uptime_kuma_api-0.9.0/
--rw-r--r--   0 lucas     (1000) users      (985)     1067 2023-01-17 20:03:37.000000 uptime_kuma_api-0.9.0/LICENSE
--rw-r--r--   0 lucas     (1000) users      (985)     3151 2023-01-17 20:39:01.000000 uptime_kuma_api-0.9.0/PKG-INFO
--rw-r--r--   0 lucas     (1000) users      (985)     1584 2023-01-17 19:52:46.000000 uptime_kuma_api-0.9.0/README.md
--rw-r--r--   0 lucas     (1000) users      (985)       38 2023-01-17 20:39:01.000000 uptime_kuma_api-0.9.0/setup.cfg
--rw-r--r--   0 lucas     (1000) users      (985)     1858 2022-09-07 09:55:07.000000 uptime_kuma_api-0.9.0/setup.py
-drwxr-xr-x   0 lucas     (1000) users      (985)        0 2023-01-17 20:39:01.000000 uptime_kuma_api-0.9.0/uptime_kuma_api/
--rw-r--r--   0 lucas     (1000) users      (985)      541 2022-12-27 20:21:19.000000 uptime_kuma_api-0.9.0/uptime_kuma_api/__init__.py
--rw-r--r--   0 lucas     (1000) users      (985)      142 2023-01-17 20:03:37.000000 uptime_kuma_api-0.9.0/uptime_kuma_api/__version__.py
--rw-r--r--   0 lucas     (1000) users      (985)   114396 2023-01-17 19:52:38.000000 uptime_kuma_api-0.9.0/uptime_kuma_api/api.py
--rw-r--r--   0 lucas     (1000) users      (985)      276 2022-12-16 20:42:20.000000 uptime_kuma_api-0.9.0/uptime_kuma_api/auth_method.py
--rw-r--r--   0 lucas     (1000) users      (985)      169 2022-12-16 20:42:20.000000 uptime_kuma_api-0.9.0/uptime_kuma_api/docker_type.py
--rw-r--r--   0 lucas     (1000) users      (985)    26782 2023-01-17 19:52:38.000000 uptime_kuma_api-0.9.0/uptime_kuma_api/docstrings.py
--rw-r--r--   0 lucas     (1000) users      (985)      618 2022-12-27 13:49:50.000000 uptime_kuma_api-0.9.0/uptime_kuma_api/event.py
--rw-r--r--   0 lucas     (1000) users      (985)      142 2022-12-16 20:42:20.000000 uptime_kuma_api-0.9.0/uptime_kuma_api/exceptions.py
--rw-r--r--   0 lucas     (1000) users      (985)      324 2022-12-16 20:42:20.000000 uptime_kuma_api-0.9.0/uptime_kuma_api/incident_style.py
--rw-r--r--   0 lucas     (1000) users      (985)      470 2022-12-28 14:09:19.000000 uptime_kuma_api-0.9.0/uptime_kuma_api/maintenance_strategy.py
--rw-r--r--   0 lucas     (1000) users      (985)      705 2022-12-27 12:48:20.000000 uptime_kuma_api-0.9.0/uptime_kuma_api/monitor_type.py
--rw-r--r--   0 lucas     (1000) users      (985)    11175 2023-01-17 19:52:38.000000 uptime_kuma_api-0.9.0/uptime_kuma_api/notification_providers.py
--rw-r--r--   0 lucas     (1000) users      (985)      336 2022-12-27 13:47:50.000000 uptime_kuma_api-0.9.0/uptime_kuma_api/proxy_protocol.py
-drwxr-xr-x   0 lucas     (1000) users      (985)        0 2023-01-17 20:39:01.000000 uptime_kuma_api-0.9.0/uptime_kuma_api.egg-info/
--rw-r--r--   0 lucas     (1000) users      (985)     3151 2023-01-17 20:39:01.000000 uptime_kuma_api-0.9.0/uptime_kuma_api.egg-info/PKG-INFO
--rw-r--r--   0 lucas     (1000) users      (985)      631 2023-01-17 20:39:01.000000 uptime_kuma_api-0.9.0/uptime_kuma_api.egg-info/SOURCES.txt
--rw-r--r--   0 lucas     (1000) users      (985)        1 2023-01-17 20:39:01.000000 uptime_kuma_api-0.9.0/uptime_kuma_api.egg-info/dependency_links.txt
--rw-r--r--   0 lucas     (1000) users      (985)       41 2023-01-17 20:39:01.000000 uptime_kuma_api-0.9.0/uptime_kuma_api.egg-info/requires.txt
--rw-r--r--   0 lucas     (1000) users      (985)       16 2023-01-17 20:39:01.000000 uptime_kuma_api-0.9.0/uptime_kuma_api.egg-info/top_level.txt
+drwxr-xr-x   0 lucas     (1000) users      (985)        0 2023-05-25 19:36:58.984835 uptime_kuma_api-1.0.0/
+-rw-r--r--   0 lucas     (1000) users      (985)     1067 2023-04-07 19:52:49.000000 uptime_kuma_api-1.0.0/LICENSE
+-rw-r--r--   0 lucas     (1000) users      (985)     3186 2023-05-25 19:36:58.984835 uptime_kuma_api-1.0.0/PKG-INFO
+-rw-r--r--   0 lucas     (1000) users      (985)     2057 2023-05-20 17:41:15.000000 uptime_kuma_api-1.0.0/README.md
+-rw-r--r--   0 lucas     (1000) users      (985)       38 2023-05-25 19:36:58.984835 uptime_kuma_api-1.0.0/setup.cfg
+-rw-r--r--   0 lucas     (1000) users      (985)     1818 2023-05-25 17:51:04.000000 uptime_kuma_api-1.0.0/setup.py
+drwxr-xr-x   0 lucas     (1000) users      (985)        0 2023-05-25 19:36:58.981501 uptime_kuma_api-1.0.0/uptime_kuma_api/
+-rw-r--r--   0 lucas     (1000) users      (985)      592 2023-05-19 12:02:01.000000 uptime_kuma_api-1.0.0/uptime_kuma_api/__init__.py
+-rw-r--r--   0 lucas     (1000) users      (985)      142 2023-05-20 18:50:23.000000 uptime_kuma_api-1.0.0/uptime_kuma_api/__version__.py
+-rw-r--r--   0 lucas     (1000) users      (985)   149300 2023-05-25 19:16:46.000000 uptime_kuma_api-1.0.0/uptime_kuma_api/api.py
+-rw-r--r--   0 lucas     (1000) users      (985)      326 2023-04-07 19:52:49.000000 uptime_kuma_api-1.0.0/uptime_kuma_api/auth_method.py
+-rw-r--r--   0 lucas     (1000) users      (985)      169 2023-04-07 19:52:49.000000 uptime_kuma_api-1.0.0/uptime_kuma_api/docker_type.py
+-rw-r--r--   0 lucas     (1000) users      (985)    29259 2023-05-20 13:03:51.000000 uptime_kuma_api-1.0.0/uptime_kuma_api/docstrings.py
+-rw-r--r--   0 lucas     (1000) users      (985)      650 2023-04-07 19:52:49.000000 uptime_kuma_api-1.0.0/uptime_kuma_api/event.py
+-rw-r--r--   0 lucas     (1000) users      (985)      252 2023-05-19 12:02:01.000000 uptime_kuma_api-1.0.0/uptime_kuma_api/exceptions.py
+-rw-r--r--   0 lucas     (1000) users      (985)      324 2023-04-07 19:52:49.000000 uptime_kuma_api-1.0.0/uptime_kuma_api/incident_style.py
+-rw-r--r--   0 lucas     (1000) users      (985)      515 2023-05-01 18:17:19.000000 uptime_kuma_api-1.0.0/uptime_kuma_api/maintenance_strategy.py
+-rw-r--r--   0 lucas     (1000) users      (985)      226 2023-05-19 12:02:01.000000 uptime_kuma_api-1.0.0/uptime_kuma_api/monitor_status.py
+-rw-r--r--   0 lucas     (1000) users      (985)      828 2023-04-07 19:52:49.000000 uptime_kuma_api-1.0.0/uptime_kuma_api/monitor_type.py
+-rw-r--r--   0 lucas     (1000) users      (985)    14475 2023-05-20 12:16:15.000000 uptime_kuma_api-1.0.0/uptime_kuma_api/notification_providers.py
+-rw-r--r--   0 lucas     (1000) users      (985)      336 2023-04-07 19:52:49.000000 uptime_kuma_api-1.0.0/uptime_kuma_api/proxy_protocol.py
+drwxr-xr-x   0 lucas     (1000) users      (985)        0 2023-05-25 19:36:58.984835 uptime_kuma_api-1.0.0/uptime_kuma_api.egg-info/
+-rw-r--r--   0 lucas     (1000) users      (985)     3186 2023-05-25 19:36:58.000000 uptime_kuma_api-1.0.0/uptime_kuma_api.egg-info/PKG-INFO
+-rw-r--r--   0 lucas     (1000) users      (985)      665 2023-05-25 19:36:58.000000 uptime_kuma_api-1.0.0/uptime_kuma_api.egg-info/SOURCES.txt
+-rw-r--r--   0 lucas     (1000) users      (985)        1 2023-05-25 19:36:58.000000 uptime_kuma_api-1.0.0/uptime_kuma_api.egg-info/dependency_links.txt
+-rw-r--r--   0 lucas     (1000) users      (985)       41 2023-05-25 19:36:58.000000 uptime_kuma_api-1.0.0/uptime_kuma_api.egg-info/requires.txt
+-rw-r--r--   0 lucas     (1000) users      (985)       16 2023-05-25 19:36:58.000000 uptime_kuma_api-1.0.0/uptime_kuma_api.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `uptime_kuma_api-0.9.0/LICENSE` & `uptime_kuma_api-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `uptime_kuma_api-0.9.0/PKG-INFO` & `uptime_kuma_api-1.0.0/uptime_kuma_api.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,80 +1,101 @@
 Metadata-Version: 2.1
-Name: uptime_kuma_api
-Version: 0.9.0
+Name: uptime-kuma-api
+Version: 1.0.0
 Summary: A python wrapper for the Uptime Kuma WebSocket API
 Home-page: https://github.com/lucasheld/uptime-kuma-api
 Author: Lucas Held
 Author-email: lucasheld@hotmail.de
 License: MIT
-Description: # uptime-kuma-api
-        
-        A wrapper for the Uptime Kuma Socket.IO API
-        ---
-        uptime-kuma-api is a Python wrapper for the [Uptime Kuma](https://github.com/louislam/uptime-kuma) Socket.IO API.
-        
-        This package was developed to configure Uptime Kuma with Ansible. The Ansible collection can be found at https://github.com/lucasheld/ansible-uptime-kuma.
-        
-        Python version 3.6+ is required.
-        
-        Supported Uptime Kuma versions: 1.17.0 - 1.19.5
-        
-        Installation
-        ---
-        uptime-kuma-api is available on the [Python Package Index (PyPI)](https://pypi.org/project/uptime-kuma-api/).
-        
-        You can install it using pip:
-        
-        ```
-        pip install uptime-kuma-api
-        ```
-        
-        Documentation
-        ---
-        The API Reference is available on [Read the Docs](https://uptime-kuma-api.readthedocs.io).
-        
-        Examples
-        ---
-        Once you have installed the python package, you can use it to communicate with an Uptime Kuma instance.
-        
-        To do so, import `UptimeKumaApi` from the library and specify the Uptime Kuma server url (e.g. 'http://127.0.0.1:3001'), username and password to initialize the connection.
-        
-        ```python
-        >>> from uptime_kuma_api import UptimeKumaApi, MonitorType
-        >>> api = UptimeKumaApi('INSERT_URL')
-        >>> api.login('INSERT_USERNAME', 'INSERT_PASSWORD')
-        ```
-        
-        Now you can call one of the existing methods of the instance. For example create a new monitor:
-        
-        ```python
-        >>> result = api.add_monitor(type=MonitorType.HTTP, name="Google", url="https://google.com")
-        >>> print(result)
-        {'msg': 'Added Successfully.', 'monitorId': 1}
-        ```
-        
-        At the end, the connection to the API must be disconnected so that the program does not block.
-        
-        ```python
-        >>> api.disconnect()
-        ```
-        
 Platform: UNKNOWN
-Classifier: Development Status :: 1 - Planning
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Libraries
-Requires-Python: >=3.6, <4
+Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# uptime-kuma-api
+
+A wrapper for the Uptime Kuma Socket.IO API
+---
+uptime-kuma-api is a Python wrapper for the [Uptime Kuma](https://github.com/louislam/uptime-kuma) Socket.IO API.
+
+This package was developed to configure Uptime Kuma with Ansible. The Ansible collection can be found at https://github.com/lucasheld/ansible-uptime-kuma.
+
+Python version 3.7+ is required.
+
+Supported Uptime Kuma versions:
+
+| Uptime Kuma     | uptime-kuma-api |
+|-----------------|-----------------|
+| 1.21.3          | 1.0.0           |
+| 1.17.0 - 1.21.2 | 0.1.0 - 0.13.0  |
+
+Installation
+---
+uptime-kuma-api is available on the [Python Package Index (PyPI)](https://pypi.org/project/uptime-kuma-api/).
+
+You can install it using pip:
+
+```
+pip install uptime-kuma-api
+```
+
+Documentation
+---
+The API Reference is available on [Read the Docs](https://uptime-kuma-api.readthedocs.io).
+
+Example
+---
+Once you have installed the python package, you can use it to communicate with an Uptime Kuma instance.
+
+To do so, import `UptimeKumaApi` from the library and specify the Uptime Kuma server url (e.g. 'http://127.0.0.1:3001'), username and password to initialize the connection.
+
+```python
+>>> from uptime_kuma_api import UptimeKumaApi, MonitorType
+>>> api = UptimeKumaApi('INSERT_URL')
+>>> api.login('INSERT_USERNAME', 'INSERT_PASSWORD')
+```
+
+Now you can call one of the existing methods of the instance. For example create a new monitor:
+
+```python
+>>> result = api.add_monitor(type=MonitorType.HTTP, name="Google", url="https://google.com")
+>>> print(result)
+{'msg': 'Added Successfully.', 'monitorId': 1}
+```
+
+At the end, the connection to the API must be disconnected so that the program does not block.
+
+```python
+>>> api.disconnect()
+```
+
+With a context manager, the disconnect method is called automatically:
+
+```python
+from uptime_kuma_api import UptimeKumaApi
+
+with UptimeKumaApi('INSERT_URL') as api:
+    api.login('INSERT_USERNAME', 'INSERT_PASSWORD')
+    api.add_monitor(
+        type=MonitorType.HTTP,
+        name="Google",
+        url="https://google.com"
+    )
+```
+
+
```

### Comparing `uptime_kuma_api-0.9.0/README.md` & `uptime_kuma_api-1.0.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -2,17 +2,22 @@
 
 A wrapper for the Uptime Kuma Socket.IO API
 ---
 uptime-kuma-api is a Python wrapper for the [Uptime Kuma](https://github.com/louislam/uptime-kuma) Socket.IO API.
 
 This package was developed to configure Uptime Kuma with Ansible. The Ansible collection can be found at https://github.com/lucasheld/ansible-uptime-kuma.
 
-Python version 3.6+ is required.
+Python version 3.7+ is required.
 
-Supported Uptime Kuma versions: 1.17.0 - 1.19.5
+Supported Uptime Kuma versions:
+
+| Uptime Kuma     | uptime-kuma-api |
+|-----------------|-----------------|
+| 1.21.3          | 1.0.0           |
+| 1.17.0 - 1.21.2 | 0.1.0 - 0.13.0  |
 
 Installation
 ---
 uptime-kuma-api is available on the [Python Package Index (PyPI)](https://pypi.org/project/uptime-kuma-api/).
 
 You can install it using pip:
 
@@ -20,15 +25,15 @@
 pip install uptime-kuma-api
 ```
 
 Documentation
 ---
 The API Reference is available on [Read the Docs](https://uptime-kuma-api.readthedocs.io).
 
-Examples
+Example
 ---
 Once you have installed the python package, you can use it to communicate with an Uptime Kuma instance.
 
 To do so, import `UptimeKumaApi` from the library and specify the Uptime Kuma server url (e.g. 'http://127.0.0.1:3001'), username and password to initialize the connection.
 
 ```python
 >>> from uptime_kuma_api import UptimeKumaApi, MonitorType
@@ -45,7 +50,21 @@
 ```
 
 At the end, the connection to the API must be disconnected so that the program does not block.
 
 ```python
 >>> api.disconnect()
 ```
+
+With a context manager, the disconnect method is called automatically:
+
+```python
+from uptime_kuma_api import UptimeKumaApi
+
+with UptimeKumaApi('INSERT_URL') as api:
+    api.login('INSERT_USERNAME', 'INSERT_PASSWORD')
+    api.add_monitor(
+        type=MonitorType.HTTP,
+        name="Google",
+        url="https://google.com"
+    )
+```
```

### Comparing `uptime_kuma_api-0.9.0/setup.py` & `uptime_kuma_api-1.0.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,29 +25,28 @@
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/lucasheld/uptime-kuma-api",
     author=info["__author__"],
     author_email="lucasheld@hotmail.de",
     license=info["__license__"],
     packages=["uptime_kuma_api"],
-    python_requires=">=3.6, <4",
+    python_requires=">=3.7, <4",
     install_requires=[
         "python-socketio[client]>=5.0.0",
         "packaging"
     ],
     classifiers=[
-        "Development Status :: 1 - Planning",
+        "Development Status :: 5 - Production/Stable",
         "Environment :: Web Environment",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3 :: Only",
         "Topic :: Internet :: WWW/HTTP",
```

### Comparing `uptime_kuma_api-0.9.0/uptime_kuma_api/__init__.py` & `uptime_kuma_api-1.0.0/uptime_kuma_api/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from .__version__ import __title__, __version__, __author__, __copyright__
 from .auth_method import AuthMethod
+from .monitor_status import MonitorStatus
 from .monitor_type import MonitorType
 from .notification_providers import NotificationType, notification_provider_options, notification_provider_conditions
 from .proxy_protocol import ProxyProtocol
 from .incident_style import IncidentStyle
 from .docker_type import DockerType
 from .maintenance_strategy import MaintenanceStrategy
-from .exceptions import UptimeKumaException
+from .exceptions import UptimeKumaException, Timeout
 from .event import Event
 from .api import UptimeKumaApi
```

### Comparing `uptime_kuma_api-0.9.0/uptime_kuma_api/docstrings.py` & `uptime_kuma_api-1.0.0/uptime_kuma_api/docstrings.py`

 * *Files 17% similar despite different names*

```diff
@@ -14,36 +14,42 @@
     return _doc
 
 
 def monitor_docstring(mode) -> str:
     return f"""
         :param MonitorType{", optional" if mode == "edit" else ""} type: Monitor Type
         :param str{", optional" if mode == "edit" else ""} name: Friendly Name
+        :param str, optional description: Description, defaults to None
         :param int, optional interval: Heartbeat Interval, defaults to 60
         :param int, optional retryInterval: Retry every X seconds, defaults to 60
         :param int, optional resendInterval: Resend every X times, defaults to 0
         :param int, optional maxretries: Retries. Maximum retries before the service is marked as down and a notification is sent., defaults to 0
         :param bool, optional upsideDown: Upside Down Mode. Flip the status upside down. If the service is reachable, it is DOWN., defaults to False
         :param list, optional notificationIDList: Notifications, defaults to None
         :param str, optional url: URL, defaults to None
         :param bool, optional expiryNotification: Certificate Expiry Notification, defaults to False
         :param bool, optional ignoreTls: Ignore TLS/SSL error for HTTPS websites, defaults to False
         :param int, optional maxredirects: Max. Redirects. Maximum number of redirects to follow. Set to 0 to disable redirects., defaults to 10
         :param list, optional accepted_statuscodes: Accepted Status Codes. Select status codes which are considered as a successful response., defaults to None
         :param int, optional proxyId: Proxy, defaults to None
         :param str, optional method: Method, defaults to "GET"
+        :param str, optional httpBodyEncoding: Body Encoding, defaults to "json". Allowed values: "json", "xml".
         :param str, optional body: Body, defaults to None
         :param str, optional headers: Headers, defaults to None
         :param AuthMethod, optional authMethod: Method, defaults to :attr:`~.AuthMethod.NONE`
-        :param str, optional basic_auth_user: Username, defaults to None
-        :param str, optional basic_auth_pass: Password, defaults to None
-        :param str, optional authDomain: Domain, defaults to None
-        :param str, optional authWorkstation: Workstation, defaults to None
+        :param str, optional tlsCert: Cert for ``authMethod`` :attr:`~.AuthMethod.MTLS`, defaults to None.
+        :param str, optional tlsKey: Key for ``authMethod`` :attr:`~.AuthMethod.MTLS`, defaults to None.
+        :param str, optional tlsCa: Ca for ``authMethod`` :attr:`~.AuthMethod.MTLS`, defaults to None.
+        :param str, optional basic_auth_user: Username for ``authMethod`` :attr:`~.AuthMethod.HTTP_BASIC` and :attr:`~.AuthMethod.NTLM`, defaults to None
+        :param str, optional basic_auth_pass: Password for ``authMethod`` :attr:`~.AuthMethod.HTTP_BASIC` and :attr:`~.AuthMethod.NTLM`, defaults to None
+        :param str, optional authDomain: Domain for ``authMethod`` :attr:`~.AuthMethod.NTLM`, defaults to None
+        :param str, optional authWorkstation: Workstation for ``authMethod`` :attr:`~.AuthMethod.NTLM`, defaults to None
         :param str, optional keyword: Keyword. Search keyword in plain HTML or JSON response. The search is case-sensitive., defaults to None
         :param str, optional hostname: Hostname, defaults to None
+        :param int, optional packetSize: Packet Size, defaults to None
         :param int, optional port: Port, ``type`` :attr:`~.MonitorType.DNS` defaults to ``53`` and ``type`` :attr:`~.MonitorType.RADIUS` defaults to ``1812``
         :param str, optional dns_resolve_server: Resolver Server, defaults to "1.1.1.1"
         :param str, optional dns_resolve_type: Resource Record Type, defaults to "A"
         :param str, optional mqttUsername: MQTT Username, defaults to None
         :param str, optional mqttPassword: MQTT Password, defaults to None
         :param str, optional mqttTopic: MQTT Topic, defaults to None
         :param str, optional mqttSuccessMessage: MQTT Success Message, defaults to None
@@ -52,205 +58,231 @@
         :param str, optional docker_container: Container Name / ID, defaults to ""
         :param int, optional docker_host: Docker Host, defaults to None
         :param str, optional radiusUsername: Radius Username, defaults to None
         :param str, optional radiusPassword: Radius Password, defaults to None
         :param str, optional radiusSecret: Radius Secret. Shared Secret between client and server., defaults to None
         :param str, optional radiusCalledStationId: Called Station Id. Identifier of the called device., defaults to None
         :param str, optional radiusCallingStationId: Calling Station Id. Identifier of the calling device., defaults to None
+        :param str, optional game: Game, defaults to None
     """
 
 
 def notification_docstring(mode) -> str:
     return f"""
         :param str{", optional" if mode == "edit" else ""} name: Friendly Name        
         :param NotificationType{", optional" if mode == "edit" else ""} type: Notification Type        
         :param bool, optional isDefault: Default enabled. This notification will be enabled by default for new monitors. You can still disable the notification separately for each monitor., defaults to False
         :param bool, optional applyExisting: Apply on all existing monitors, defaults to False
         
-        :param str, optional alertaApiEndpoint: Notification option for ``type`` :attr:`~.NotificationType.ALERTA`
-        :param str, optional alertaApiKey: Notification option for ``type`` :attr:`~.NotificationType.ALERTA`
-        :param str, optional alertaEnvironment: Notification option for ``type`` :attr:`~.NotificationType.ALERTA`
-        :param str, optional alertaAlertState: Notification option for ``type`` :attr:`~.NotificationType.ALERTA`
-        :param str, optional alertaRecoverState: Notification option for ``type`` :attr:`~.NotificationType.ALERTA`
-        :param str, optional phonenumber: Notification option for ``type`` :attr:`~.NotificationType.ALIYUNSMS`
-        :param str, optional templateCode: Notification option for ``type`` :attr:`~.NotificationType.ALIYUNSMS`
-        :param str, optional signName: Notification option for ``type`` :attr:`~.NotificationType.ALIYUNSMS`
-        :param str, optional accessKeyId: Notification option for ``type`` :attr:`~.NotificationType.ALIYUNSMS`
-        :param str, optional secretAccessKey: Notification option for ``type`` :attr:`~.NotificationType.ALIYUNSMS`
-        :param str, optional appriseURL: Notification option for ``type`` :attr:`~.NotificationType.APPRISE`
-        :param str, optional title: Notification option for ``type`` :attr:`~.NotificationType.APPRISE`
-        :param str, optional clicksendsmsLogin: Notification option for ``type`` :attr:`~.NotificationType.CLICKSENDSMS`
-        :param str, optional clicksendsmsPassword: Notification option for ``type`` :attr:`~.NotificationType.CLICKSENDSMS`
-        :param str, optional clicksendsmsToNumber: Notification option for ``type`` :attr:`~.NotificationType.CLICKSENDSMS`
-        :param str, optional clicksendsmsSenderName: Notification option for ``type`` :attr:`~.NotificationType.CLICKSENDSMS`
-        :param str, optional webHookUrl: Notification option for ``type`` :attr:`~.NotificationType.DINGDING`
-        :param str, optional secretKey: Notification option for ``type`` :attr:`~.NotificationType.DINGDING`
-        :param str, optional discordUsername: Notification option for ``type`` :attr:`~.NotificationType.DISCORD`
-        :param str, optional discordWebhookUrl: Notification option for ``type`` :attr:`~.NotificationType.DISCORD`
-        :param str, optional discordPrefixMessage: Notification option for ``type`` :attr:`~.NotificationType.DISCORD`
-        :param str, optional feishuWebHookUrl: Notification option for ``type`` :attr:`~.NotificationType.FEISHU`
-        :param str, optional googleChatWebhookURL: Notification option for ``type`` :attr:`~.NotificationType.GOOGLECHAT`
-        :param str, optional gorushDeviceToken: Notification option for ``type`` :attr:`~.NotificationType.GORUSH`
-        :param str, optional gorushPlatform: Notification option for ``type`` :attr:`~.NotificationType.GORUSH`
-        :param str, optional gorushTitle: Notification option for ``type`` :attr:`~.NotificationType.GORUSH`
-        :param str, optional gorushPriority: Notification option for ``type`` :attr:`~.NotificationType.GORUSH`
-        :param str, optional gorushRetry: Notification option for ``type`` :attr:`~.NotificationType.GORUSH`
-        :param str, optional gorushTopic: Notification option for ``type`` :attr:`~.NotificationType.GORUSH`
-        :param str, optional gorushServerURL: Notification option for ``type`` :attr:`~.NotificationType.GORUSH`
-        :param str, optional gotifyserverurl: Notification option for ``type`` :attr:`~.NotificationType.GOTIFY`
-        :param str, optional gotifyapplicationToken: Notification option for ``type`` :attr:`~.NotificationType.GOTIFY`
-        :param int, optional gotifyPriority: Notification option for ``type`` :attr:`~.NotificationType.GOTIFY`
-        :param str, optional lineChannelAccessToken: Notification option for ``type`` :attr:`~.NotificationType.LINE`
-        :param str, optional lineUserID: Notification option for ``type`` :attr:`~.NotificationType.LINE`
-        :param str, optional lunaseaDevice: Notification option for ``type`` :attr:`~.NotificationType.LUNASEA`
-        :param str, optional internalRoomId: Notification option for ``type`` :attr:`~.NotificationType.MATRIX`
-        :param str, optional accessToken: Notification option for ``type`` :attr:`~.NotificationType.MATRIX`
-        :param str, optional homeserverUrl: Notification option for ``type`` :attr:`~.NotificationType.MATRIX`
-        :param str, optional mattermostusername: Notification option for ``type`` :attr:`~.NotificationType.MATTERMOST`
-        :param str, optional mattermostWebhookUrl: Notification option for ``type`` :attr:`~.NotificationType.MATTERMOST`
-        :param str, optional mattermostchannel: Notification option for ``type`` :attr:`~.NotificationType.MATTERMOST`
-        :param str, optional mattermosticonemo: Notification option for ``type`` :attr:`~.NotificationType.MATTERMOST`
-        :param str, optional mattermosticonurl: Notification option for ``type`` :attr:`~.NotificationType.MATTERMOST`
-        :param str, optional httpAddr: Notification option for ``type`` :attr:`~.NotificationType.ONEBOT`
-        :param str, optional accessToken: Notification option for ``type`` :attr:`~.NotificationType.ONEBOT`
-        :param str, optional msgType: Notification option for ``type`` :attr:`~.NotificationType.ONEBOT`
-        :param str, optional recieverId: Notification option for ``type`` :attr:`~.NotificationType.ONEBOT`
-        :param str, optional pagerdutyAutoResolve: Notification option for ``type`` :attr:`~.NotificationType.PAGERDUTY`
-        :param str, optional pagerdutyIntegrationUrl: Notification option for ``type`` :attr:`~.NotificationType.PAGERDUTY`
-        :param str, optional pagerdutyPriority: Notification option for ``type`` :attr:`~.NotificationType.PAGERDUTY`
-        :param str, optional pagerdutyIntegrationKey: Notification option for ``type`` :attr:`~.NotificationType.PAGERDUTY`
-        :param str, optional promosmsLogin: Notification option for ``type`` :attr:`~.NotificationType.PROMOSMS`
-        :param str, optional promosmsPassword: Notification option for ``type`` :attr:`~.NotificationType.PROMOSMS`
-        :param str, optional promosmsPhoneNumber: Notification option for ``type`` :attr:`~.NotificationType.PROMOSMS`. Phone number (for Polish recipient You can skip area codes).
-        :param str, optional promosmsSMSType: Notification option for ``type`` :attr:`~.NotificationType.PROMOSMS`.
+        :param str, optional alertaApiEndpoint: Notification option for ``type`` :attr:`~.NotificationType.ALERTA`.
+        :param str, optional alertaApiKey: Notification option for ``type`` :attr:`~.NotificationType.ALERTA`.
+        :param str, optional alertaEnvironment: Notification option for ``type`` :attr:`~.NotificationType.ALERTA`.
+        :param str, optional alertaAlertState: Notification option for ``type`` :attr:`~.NotificationType.ALERTA`.
+        :param str, optional alertaRecoverState: Notification option for ``type`` :attr:`~.NotificationType.ALERTA`.
+        :param str, optional alertNowWebhookURL: Notification option for ``type`` :attr:`~.NotificationType.ALERTNOW`.
+        :param str, optional phonenumber: Notification option for ``type`` :attr:`~.NotificationType.ALIYUNSMS`.
+        :param str, optional templateCode: Notification option for ``type`` :attr:`~.NotificationType.ALIYUNSMS`.
+        :param str, optional signName: Notification option for ``type`` :attr:`~.NotificationType.ALIYUNSMS`.
+        :param str, optional accessKeyId: Notification option for ``type`` :attr:`~.NotificationType.ALIYUNSMS`.
+        :param str, optional secretAccessKey: Notification option for ``type`` :attr:`~.NotificationType.ALIYUNSMS`.
+        :param str, optional appriseURL: Notification option for ``type`` :attr:`~.NotificationType.APPRISE`.
+        :param str title: Notification option for ``type`` :attr:`~.NotificationType.APPRISE`.
+        :param str, optional barkEndpoint: Notification option for ``type`` :attr:`~.NotificationType.BARK`.
+        :param str, optional barkGroup: Notification option for ``type`` :attr:`~.NotificationType.BARK`.
+        :param str, optional barkSound: Notification option for ``type`` :attr:`~.NotificationType.BARK`.
+        :param str, optional clicksendsmsLogin: Notification option for ``type`` :attr:`~.NotificationType.CLICKSENDSMS`.
+        :param str, optional clicksendsmsPassword: Notification option for ``type`` :attr:`~.NotificationType.CLICKSENDSMS`.
+        :param str, optional clicksendsmsToNumber: Notification option for ``type`` :attr:`~.NotificationType.CLICKSENDSMS`.
+        :param str clicksendsmsSenderName: Notification option for ``type`` :attr:`~.NotificationType.CLICKSENDSMS`.
+        :param str, optional webHookUrl: Notification option for ``type`` :attr:`~.NotificationType.DINGDING`.
+        :param str, optional secretKey: Notification option for ``type`` :attr:`~.NotificationType.DINGDING`.
+        :param str discordUsername: Notification option for ``type`` :attr:`~.NotificationType.DISCORD`.
+        :param str, optional discordWebhookUrl: Notification option for ``type`` :attr:`~.NotificationType.DISCORD`.
+        :param str discordPrefixMessage: Notification option for ``type`` :attr:`~.NotificationType.DISCORD`.
+        :param str, optional feishuWebHookUrl: Notification option for ``type`` :attr:`~.NotificationType.FEISHU`.
+        :param str, optional freemobileUser: Notification option for ``type`` :attr:`~.NotificationType.FREEMOBILE`.
+        :param str, optional freemobilePass: Notification option for ``type`` :attr:`~.NotificationType.FREEMOBILE`.
+        :param str, optional goAlertBaseURL: Notification option for ``type`` :attr:`~.NotificationType.GOALERT`.
+        :param str, optional goAlertToken: Notification option for ``type`` :attr:`~.NotificationType.GOALERT`.
+        :param str, optional googleChatWebhookURL: Notification option for ``type`` :attr:`~.NotificationType.GOOGLECHAT`.
+        :param str, optional gorushDeviceToken: Notification option for ``type`` :attr:`~.NotificationType.GORUSH`.
+        :param str gorushPlatform: Notification option for ``type`` :attr:`~.NotificationType.GORUSH`.
+        :param str gorushTitle: Notification option for ``type`` :attr:`~.NotificationType.GORUSH`.
+        :param str gorushPriority: Notification option for ``type`` :attr:`~.NotificationType.GORUSH`.
+        :param int gorushRetry: Notification option for ``type`` :attr:`~.NotificationType.GORUSH`.
+        :param str gorushTopic: Notification option for ``type`` :attr:`~.NotificationType.GORUSH`.
+        :param str, optional gorushServerURL: Notification option for ``type`` :attr:`~.NotificationType.GORUSH`.
+        :param str, optional gotifyserverurl: Notification option for ``type`` :attr:`~.NotificationType.GOTIFY`.
+        :param str, optional gotifyapplicationToken: Notification option for ``type`` :attr:`~.NotificationType.GOTIFY`.
+        :param int, optional gotifyPriority: Notification option for ``type`` :attr:`~.NotificationType.GOTIFY`.
+        :param str notificationService: Notification option for ``type`` :attr:`~.NotificationType.HOMEASSISTANT`.
+        :param str, optional homeAssistantUrl: Notification option for ``type`` :attr:`~.NotificationType.HOMEASSISTANT`.
+        :param str, optional longLivedAccessToken: Notification option for ``type`` :attr:`~.NotificationType.HOMEASSISTANT`.
+        :param str, optional kookGuildID: Notification option for ``type`` :attr:`~.NotificationType.KOOK`.
+        :param str, optional kookBotToken: Notification option for ``type`` :attr:`~.NotificationType.KOOK`.
+        :param str, optional lineChannelAccessToken: Notification option for ``type`` :attr:`~.NotificationType.LINE`.
+        :param str, optional lineUserID: Notification option for ``type`` :attr:`~.NotificationType.LINE`.
+        :param str, optional lineNotifyAccessToken: Notification option for ``type`` :attr:`~.NotificationType.LINENOTIFY`.
+        :param str, optional lunaseaTarget: Notification option for ``type`` :attr:`~.NotificationType.LUNASEA`. Allowed values: "device", "user".
+        :param str lunaseaUserID: Notification option for ``type`` :attr:`~.NotificationType.LUNASEA`. User ID.
+        :param str lunaseaDevice: Notification option for ``type`` :attr:`~.NotificationType.LUNASEA`. Device ID.
+        :param str, optional internalRoomId: Notification option for ``type`` :attr:`~.NotificationType.MATRIX`.
+        :param str, optional accessToken: Notification option for ``type`` :attr:`~.NotificationType.MATRIX`.
+        :param str, optional homeserverUrl: Notification option for ``type`` :attr:`~.NotificationType.MATRIX`.
+        :param str mattermostusername: Notification option for ``type`` :attr:`~.NotificationType.MATTERMOST`.
+        :param str, optional mattermostWebhookUrl: Notification option for ``type`` :attr:`~.NotificationType.MATTERMOST`.
+        :param str mattermostchannel: Notification option for ``type`` :attr:`~.NotificationType.MATTERMOST`.
+        :param str mattermosticonemo: Notification option for ``type`` :attr:`~.NotificationType.MATTERMOST`.
+        :param str mattermosticonurl: Notification option for ``type`` :attr:`~.NotificationType.MATTERMOST`.
+        :param str ntfyusername: Notification option for ``type`` :attr:`~.NotificationType.NTFY`.
+        :param str ntfypassword: Notification option for ``type`` :attr:`~.NotificationType.NTFY`.
+        :param str, optional ntfytopic: Notification option for ``type`` :attr:`~.NotificationType.NTFY`.
+        :param int, optional ntfyPriority: Notification option for ``type`` :attr:`~.NotificationType.NTFY`.
+        :param str ntfyIcon: Notification option for ``type`` :attr:`~.NotificationType.NTFY`.
+        :param str, optional ntfyserverurl: Notification option for ``type`` :attr:`~.NotificationType.NTFY`.
+        :param str octopushVersion: Notification option for ``type`` :attr:`~.NotificationType.OCTOPUSH`.
+        :param str, optional octopushAPIKey: Notification option for ``type`` :attr:`~.NotificationType.OCTOPUSH`.
+        :param str, optional octopushLogin: Notification option for ``type`` :attr:`~.NotificationType.OCTOPUSH`.
+        :param str, optional octopushPhoneNumber: Notification option for ``type`` :attr:`~.NotificationType.OCTOPUSH`.
+        :param str octopushSMSType: Notification option for ``type`` :attr:`~.NotificationType.OCTOPUSH`.
+        :param str octopushSenderName: Notification option for ``type`` :attr:`~.NotificationType.OCTOPUSH`.
+        :param str, optional httpAddr: Notification option for ``type`` :attr:`~.NotificationType.ONEBOT`.
+        :param str, optional accessToken: Notification option for ``type`` :attr:`~.NotificationType.ONEBOT`.
+        :param str msgType: Notification option for ``type`` :attr:`~.NotificationType.ONEBOT`.
+        :param str, optional recieverId: Notification option for ``type`` :attr:`~.NotificationType.ONEBOT`.
+        :param int opsgeniePriority: Notification option for ``type`` :attr:`~.NotificationType.OPSGENIE`. Priority. Available values are numbers between ``1`` and ``5``.
+        :param str, optional opsgenieRegion: Notification option for ``type`` :attr:`~.NotificationType.OPSGENIE`. Region. Available values are:
+            
+            - ``us``: US (Default)
+            - ``eu``: EU
+        :param str, optional opsgenieApiKey: Notification option for ``type`` :attr:`~.NotificationType.OPSGENIE`. API Key.
+        :param str pagerdutyAutoResolve: Notification option for ``type`` :attr:`~.NotificationType.PAGERDUTY`.
+        :param str pagerdutyIntegrationUrl: Notification option for ``type`` :attr:`~.NotificationType.PAGERDUTY`.
+        :param str pagerdutyPriority: Notification option for ``type`` :attr:`~.NotificationType.PAGERDUTY`.
+        :param str, optional pagerdutyIntegrationKey: Notification option for ``type`` :attr:`~.NotificationType.PAGERDUTY`.
+        :param str pagertreeAutoResolve: Notification option for ``type`` :attr:`~.NotificationType.PAGERTREE`. 
+        
+            Available values are:
+            
+            - ``0``: Do Nothing
+            - ``resolve``: Auto Resolve
+        :param str pagertreeIntegrationUrl: Notification option for ``type`` :attr:`~.NotificationType.PAGERTREE`.
+        :param str pagertreeUrgency: Notification option for ``type`` :attr:`~.NotificationType.PAGERTREE`. 
         
             Available values are:
             
+            - ``silent``: Silent
+            - ``low``: Low
+            - ``medium``: Medium
+            - ``high``: High
+            - ``critical``: Critical
+        :param bool promosmsAllowLongSMS: Notification option for ``type`` :attr:`~.NotificationType.PROMOSMS`. Allow long SMS.
+        :param str, optional promosmsLogin: Notification option for ``type`` :attr:`~.NotificationType.PROMOSMS`.
+        :param str, optional promosmsPassword: Notification option for ``type`` :attr:`~.NotificationType.PROMOSMS`.
+        :param str, optional promosmsPhoneNumber: Notification option for ``type`` :attr:`~.NotificationType.PROMOSMS`. Phone number (for Polish recipient You can skip area codes).
+        :param str promosmsSMSType: Notification option for ``type`` :attr:`~.NotificationType.PROMOSMS`. 
+            
+            Available values are:
+            
             - ``0``: SMS FLASH - Message will automatically show on recipient device. Limited only to Polish recipients.
             - ``1``: SMS ECO - cheap but slow and often overloaded. Limited only to Polish recipients.
             - ``3``: SMS FULL - Premium tier of SMS, You can use your Sender Name (You need to register name first). Reliable for alerts.
             - ``4``: SMS SPEED - Highest priority in system. Very quick and reliable but costly (about twice of SMS FULL price).
-        :param str, optional promosmsSenderName: Notification option for ``type`` :attr:`~.NotificationType.PROMOSMS`
-        :param bool, optional promosmsAllowLongSMS: Notification option for ``type`` :attr:`~.NotificationType.PROMOSMS`. Allow long SMS.
-        :param str, optional pushbulletAccessToken: Notification option for ``type`` :attr:`~.NotificationType.PUSHBULLET`
-        :param str, optional pushdeerKey: Notification option for ``type`` :attr:`~.NotificationType.PUSHDEER`
-        :param str, optional pushoveruserkey: Notification option for ``type`` :attr:`~.NotificationType.PUSHOVER`
-        :param str, optional pushoverapptoken: Notification option for ``type`` :attr:`~.NotificationType.PUSHOVER`
-        :param str, optional pushoversounds: Notification option for ``type`` :attr:`~.NotificationType.PUSHOVER`
-        :param str, optional pushoverpriority: Notification option for ``type`` :attr:`~.NotificationType.PUSHOVER`
-        :param str, optional pushovertitle: Notification option for ``type`` :attr:`~.NotificationType.PUSHOVER`
-        :param str, optional pushoverdevice: Notification option for ``type`` :attr:`~.NotificationType.PUSHOVER`
-        :param str, optional pushyAPIKey: Notification option for ``type`` :attr:`~.NotificationType.PUSHY`
-        :param str, optional pushyToken: Notification option for ``type`` :attr:`~.NotificationType.PUSHY`
-        :param str, optional rocketchannel: Notification option for ``type`` :attr:`~.NotificationType.ROCKET_CHAT`
-        :param str, optional rocketusername: Notification option for ``type`` :attr:`~.NotificationType.ROCKET_CHAT`
-        :param str, optional rocketiconemo: Notification option for ``type`` :attr:`~.NotificationType.ROCKET_CHAT`
-        :param str, optional rocketwebhookURL: Notification option for ``type`` :attr:`~.NotificationType.ROCKET_CHAT`
-        :param str, optional rocketbutton: Notification option for ``type`` :attr:`~.NotificationType.ROCKET_CHAT`
-        :param str, optional serwersmsUsername: Notification option for ``type`` :attr:`~.NotificationType.SERWERSMS`
-        :param str, optional serwersmsPassword: Notification option for ``type`` :attr:`~.NotificationType.SERWERSMS`
-        :param str, optional serwersmsPhoneNumber: Notification option for ``type`` :attr:`~.NotificationType.SERWERSMS`
-        :param str, optional serwersmsSenderName: Notification option for ``type`` :attr:`~.NotificationType.SERWERSMS`
-        :param str, optional signalNumber: Notification option for ``type`` :attr:`~.NotificationType.SIGNAL`
-        :param str, optional signalRecipients: Notification option for ``type`` :attr:`~.NotificationType.SIGNAL`
-        :param str, optional signalURL: Notification option for ``type`` :attr:`~.NotificationType.SIGNAL`
-        :param str, optional slackbutton: Notification option for ``type`` :attr:`~.NotificationType.SLACK`
-        :param str, optional slackchannel: Notification option for ``type`` :attr:`~.NotificationType.SLACK`
-        :param str, optional slackusername: Notification option for ``type`` :attr:`~.NotificationType.SLACK`
-        :param str, optional slackiconemo: Notification option for ``type`` :attr:`~.NotificationType.SLACK`
-        :param str, optional slackwebhookURL: Notification option for ``type`` :attr:`~.NotificationType.SLACK`
-        :param str, optional smtpHost: Notification option for ``type`` :attr:`~.NotificationType.SMTP`
-        :param int, optional smtpPort: Notification option for ``type`` :attr:`~.NotificationType.SMTP`
-        :param str, optional smtpSecure: Notification option for ``type`` :attr:`~.NotificationType.SMTP`
-        :param str, optional smtpIgnoreTLSError: Notification option for ``type`` :attr:`~.NotificationType.SMTP`
-        :param str, optional smtpDkimDomain: Notification option for ``type`` :attr:`~.NotificationType.SMTP`
-        :param str, optional smtpDkimKeySelector: Notification option for ``type`` :attr:`~.NotificationType.SMTP`
-        :param str, optional smtpDkimPrivateKey: Notification option for ``type`` :attr:`~.NotificationType.SMTP`
-        :param str, optional smtpDkimHashAlgo: Notification option for ``type`` :attr:`~.NotificationType.SMTP`
-        :param str, optional smtpDkimheaderFieldNames: Notification option for ``type`` :attr:`~.NotificationType.SMTP`
-        :param str, optional smtpDkimskipFields: Notification option for ``type`` :attr:`~.NotificationType.SMTP`
-        :param str, optional smtpUsername: Notification option for ``type`` :attr:`~.NotificationType.SMTP`
-        :param str, optional smtpPassword: Notification option for ``type`` :attr:`~.NotificationType.SMTP`
-        :param str, optional customSubject: Notification option for ``type`` :attr:`~.NotificationType.SMTP`
-        :param str, optional smtpFrom: Notification option for ``type`` :attr:`~.NotificationType.SMTP`
-        :param str, optional smtpCC: Notification option for ``type`` :attr:`~.NotificationType.SMTP`
-        :param str, optional smtpBCC: Notification option for ``type`` :attr:`~.NotificationType.SMTP`
-        :param str, optional smtpTo: Notification option for ``type`` :attr:`~.NotificationType.SMTP`
-        :param str, optional stackfieldwebhookURL: Notification option for ``type`` :attr:`~.NotificationType.STACKFIELD`
-        :param str, optional pushAPIKey: Notification option for ``type`` :attr:`~.NotificationType.PUSHBYTECHULUS`
-        :param str, optional telegramBotToken: Notification option for ``type`` :attr:`~.NotificationType.TELEGRAM`
-        :param str, optional telegramChatID: Notification option for ``type`` :attr:`~.NotificationType.TELEGRAM`
-        :param str, optional webhookContentType: Notification option for ``type`` :attr:`~.NotificationType.WEBHOOK`
-        :param str, optional webhookAdditionalHeaders: Notification option for ``type`` :attr:`~.NotificationType.WEBHOOK`
-        :param str, optional webhookURL: Notification option for ``type`` :attr:`~.NotificationType.WEBHOOK`
-        :param str, optional weComBotKey: Notification option for ``type`` :attr:`~.NotificationType.WECOM`
-        :param str, optional alertNowWebhookURL: Notification option for ``type`` :attr:`~.NotificationType.ALERTNOW`
-        :param str, optional homeAssistantUrl: Notification option for ``type`` :attr:`~.NotificationType.HOMEASSISTANT`
-        :param str, optional longLivedAccessToken: Notification option for ``type`` :attr:`~.NotificationType.HOMEASSISTANT`
-        :param str, optional lineNotifyAccessToken: Notification option for ``type`` :attr:`~.NotificationType.LINENOTIFY`
-        :param str, optional barkEndpoint: Notification option for ``type`` :attr:`~.NotificationType.BARK`
-        :param str, optional barkGroup: Notification option for ``type`` :attr:`~.NotificationType.BARK`
-        :param str, optional barkSound: Notification option for ``type`` :attr:`~.NotificationType.BARK`
-        :param str, optional goAlertBaseURL: Notification option for ``type`` :attr:`~.NotificationType.GOALERT`
-        :param str, optional goAlertToken: Notification option for ``type`` :attr:`~.NotificationType.GOALERT`
-        :param str, optional octopushVersion: Notification option for ``type`` :attr:`~.NotificationType.OCTOPUSH`
-        :param str, optional octopushAPIKey: Notification option for ``type`` :attr:`~.NotificationType.OCTOPUSH`
-        :param str, optional octopushLogin: Notification option for ``type`` :attr:`~.NotificationType.OCTOPUSH`
-        :param str, optional octopushPhoneNumber: Notification option for ``type`` :attr:`~.NotificationType.OCTOPUSH`
-        :param str, optional octopushSMSType: Notification option for ``type`` :attr:`~.NotificationType.OCTOPUSH`
-        :param str, optional octopushSenderName: Notification option for ``type`` :attr:`~.NotificationType.OCTOPUSH`
-        :param str, optional octopushDMLogin: Notification option for ``type`` :attr:`~.NotificationType.OCTOPUSH`
-        :param str, optional octopushDMAPIKey: Notification option for ``type`` :attr:`~.NotificationType.OCTOPUSH`
-        :param str, optional octopushDMPhoneNumber: Notification option for ``type`` :attr:`~.NotificationType.OCTOPUSH`
-        :param str, optional octopushDMSenderName: Notification option for ``type`` :attr:`~.NotificationType.OCTOPUSH`
-        :param str, optional octopushDMSMSType: Notification option for ``type`` :attr:`~.NotificationType.OCTOPUSH`
-        :param str, optional serverChanSendKey: Notification option for ``type`` :attr:`~.NotificationType.SERVERCHAN`
-        :param str, optional smsmanagerApiKey: Notification option for ``type`` :attr:`~.NotificationType.SMSMANAGER`
-        :param str, optional numbers: Notification option for ``type`` :attr:`~.NotificationType.SMSMANAGER`
-        :param str, optional messageType: Notification option for ``type`` :attr:`~.NotificationType.SMSMANAGER`
-        :param str, optional squadcastWebhookURL: Notification option for ``type`` :attr:`~.NotificationType.SQUADCAST`
-        :param str, optional webhookUrl: Notification option for ``type`` :attr:`~.NotificationType.TEAMS`
-        :param str, optional freemobileUser: Notification option for ``type`` :attr:`~.NotificationType.FREEMOBILE`
-        :param str, optional freemobilePass: Notification option for ``type`` :attr:`~.NotificationType.FREEMOBILE`
-        :param str, optional ntfyusername: Notification option for ``type`` :attr:`~.NotificationType.NTFY`
-        :param str, optional ntfypassword: Notification option for ``type`` :attr:`~.NotificationType.NTFY`
-        :param str, optional ntfytopic: Notification option for ``type`` :attr:`~.NotificationType.NTFY`
-        :param int, optional ntfyPriority: Notification option for ``type`` :attr:`~.NotificationType.NTFY`
-        :param str, optional ntfyIcon: Notification option for ``type`` :attr:`~.NotificationType.NTFY`
-        :param str, optional ntfyserverurl: Notification option for ``type`` :attr:`~.NotificationType.NTFY`
-        :param bool, optional smseagleEncoding: Notification option for ``type`` :attr:`~.NotificationType.SMSEAGLE`. True to send messages in unicode.
-        :param int, optional smseaglePriority: Notification option for ``type`` :attr:`~.NotificationType.SMSEAGLE`. Message priority (0-9, default = 0).
-        :param str, optional smseagleRecipientType: Notification option for ``type`` :attr:`~.NotificationType.SMSEAGLE`. Recipient type.
-        
+        :param str promosmsSenderName: Notification option for ``type`` :attr:`~.NotificationType.PROMOSMS`.
+        :param str, optional pushbulletAccessToken: Notification option for ``type`` :attr:`~.NotificationType.PUSHBULLET`.
+        :param str, optional pushdeerKey: Notification option for ``type`` :attr:`~.NotificationType.PUSHDEER`.
+        :param str, optional pushoveruserkey: Notification option for ``type`` :attr:`~.NotificationType.PUSHOVER`.
+        :param str, optional pushoverapptoken: Notification option for ``type`` :attr:`~.NotificationType.PUSHOVER`.
+        :param str pushoversounds: Notification option for ``type`` :attr:`~.NotificationType.PUSHOVER`.
+        :param str pushoverpriority: Notification option for ``type`` :attr:`~.NotificationType.PUSHOVER`.
+        :param str pushovertitle: Notification option for ``type`` :attr:`~.NotificationType.PUSHOVER`.
+        :param str pushoverdevice: Notification option for ``type`` :attr:`~.NotificationType.PUSHOVER`.
+        :param str, optional pushyAPIKey: Notification option for ``type`` :attr:`~.NotificationType.PUSHY`.
+        :param str, optional pushyToken: Notification option for ``type`` :attr:`~.NotificationType.PUSHY`.
+        :param str rocketchannel: Notification option for ``type`` :attr:`~.NotificationType.ROCKET_CHAT`.
+        :param str rocketusername: Notification option for ``type`` :attr:`~.NotificationType.ROCKET_CHAT`.
+        :param str rocketiconemo: Notification option for ``type`` :attr:`~.NotificationType.ROCKET_CHAT`.
+        :param str, optional rocketwebhookURL: Notification option for ``type`` :attr:`~.NotificationType.ROCKET_CHAT`.
+        :param str, optional serverChanSendKey: Notification option for ``type`` :attr:`~.NotificationType.SERVERCHAN`.
+        :param str, optional serwersmsUsername: Notification option for ``type`` :attr:`~.NotificationType.SERWERSMS`.
+        :param str, optional serwersmsPassword: Notification option for ``type`` :attr:`~.NotificationType.SERWERSMS`.
+        :param str, optional serwersmsPhoneNumber: Notification option for ``type`` :attr:`~.NotificationType.SERWERSMS`.
+        :param str serwersmsSenderName: Notification option for ``type`` :attr:`~.NotificationType.SERWERSMS`.
+        :param str, optional signalNumber: Notification option for ``type`` :attr:`~.NotificationType.SIGNAL`.
+        :param str, optional signalRecipients: Notification option for ``type`` :attr:`~.NotificationType.SIGNAL`.
+        :param str, optional signalURL: Notification option for ``type`` :attr:`~.NotificationType.SIGNAL`.
+        :param str slackchannel: Notification option for ``type`` :attr:`~.NotificationType.SLACK`.
+        :param str slackusername: Notification option for ``type`` :attr:`~.NotificationType.SLACK`.
+        :param str slackiconemo: Notification option for ``type`` :attr:`~.NotificationType.SLACK`.
+        :param str, optional slackwebhookURL: Notification option for ``type`` :attr:`~.NotificationType.SLACK`.
+        :param bool smseagleEncoding: Notification option for ``type`` :attr:`~.NotificationType.SMSEAGLE`. True to send messages in unicode.
+        :param int smseaglePriority: Notification option for ``type`` :attr:`~.NotificationType.SMSEAGLE`. Message priority (0-9, default = 0).
+        :param str smseagleRecipientType: Notification option for ``type`` :attr:`~.NotificationType.SMSEAGLE`. Recipient type.
+            
             Available values are:
             
             - ``smseagle-to``: Phone number(s)
             - ``smseagle-group``: Phonebook group name(s)
             - ``smseagle-contact``: Phonebook contact name(s)
         :param str, optional smseagleToken: Notification option for ``type`` :attr:`~.NotificationType.SMSEAGLE`. API Access token.
         :param str, optional smseagleRecipient: Notification option for ``type`` :attr:`~.NotificationType.SMSEAGLE`. Recipient(s) (multiple must be separated with comma).
         :param str, optional smseagleUrl: Notification option for ``type`` :attr:`~.NotificationType.SMSEAGLE`. Your SMSEagle device URL.
-        :param str, optional webhookUrl: Notification option for ``type`` :attr:`~.NotificationType.ZOHOCLIQ`
-        :param str, optional kookGuildID: Notification option for ``type`` :attr:`~.NotificationType.KOOK`
-        :param str, optional kookBotToken: Notification option for ``type`` :attr:`~.NotificationType.KOOK`
-        :param str, optional splunkAutoResolve: Notification option for ``type`` :attr:`~.NotificationType.SPLUNK`. Auto resolve or acknowledged.
+        :param str smsmanagerApiKey: Notification option for ``type`` :attr:`~.NotificationType.SMSMANAGER`.
+        :param str numbers: Notification option for ``type`` :attr:`~.NotificationType.SMSMANAGER`.
+        :param str messageType: Notification option for ``type`` :attr:`~.NotificationType.SMSMANAGER`.
+        :param str, optional smtpHost: Notification option for ``type`` :attr:`~.NotificationType.SMTP`.
+        :param int, optional smtpPort: Notification option for ``type`` :attr:`~.NotificationType.SMTP`.
+        :param str smtpSecure: Notification option for ``type`` :attr:`~.NotificationType.SMTP`.
+        :param bool smtpIgnoreTLSError: Notification option for ``type`` :attr:`~.NotificationType.SMTP`.
+        :param str smtpDkimDomain: Notification option for ``type`` :attr:`~.NotificationType.SMTP`.
+        :param str smtpDkimKeySelector: Notification option for ``type`` :attr:`~.NotificationType.SMTP`.
+        :param str smtpDkimPrivateKey: Notification option for ``type`` :attr:`~.NotificationType.SMTP`.
+        :param str smtpDkimHashAlgo: Notification option for ``type`` :attr:`~.NotificationType.SMTP`.
+        :param str smtpDkimheaderFieldNames: Notification option for ``type`` :attr:`~.NotificationType.SMTP`.
+        :param str smtpDkimskipFields: Notification option for ``type`` :attr:`~.NotificationType.SMTP`.
+        :param str smtpUsername: Notification option for ``type`` :attr:`~.NotificationType.SMTP`.
+        :param str smtpPassword: Notification option for ``type`` :attr:`~.NotificationType.SMTP`.
+        :param str customSubject: Notification option for ``type`` :attr:`~.NotificationType.SMTP`.
+        :param str, optional smtpFrom: Notification option for ``type`` :attr:`~.NotificationType.SMTP`.
+        :param str smtpCC: Notification option for ``type`` :attr:`~.NotificationType.SMTP`.
+        :param str smtpBCC: Notification option for ``type`` :attr:`~.NotificationType.SMTP`.
+        :param str smtpTo: Notification option for ``type`` :attr:`~.NotificationType.SMTP`.
+        :param str splunkAutoResolve: Notification option for ``type`` :attr:`~.NotificationType.SPLUNK`. Auto resolve or acknowledged.
         
             Available values are:
             
             - ``0``: do nothing
             - ``ACKNOWLEDGEMENT``: auto acknowledged
             - ``RECOVERY``: auto resolve
-        :param str, optional splunkSeverity: Notification option for ``type`` :attr:`~.NotificationType.SPLUNK`. Severity.
+        :param str splunkSeverity: Notification option for ``type`` :attr:`~.NotificationType.SPLUNK`. Severity.
         
             Available values are:
             
             - ``INFO``
             - ``WARNING``
             - ``CRITICAL``
         :param str, optional splunkRestURL: Notification option for ``type`` :attr:`~.NotificationType.SPLUNK`. Splunk Rest URL.
+        :param str, optional squadcastWebhookURL: Notification option for ``type`` :attr:`~.NotificationType.SQUADCAST`.
+        :param str, optional stackfieldwebhookURL: Notification option for ``type`` :attr:`~.NotificationType.STACKFIELD`.
+        :param str, optional webhookUrl: Notification option for ``type`` :attr:`~.NotificationType.TEAMS`.
+        :param str, optional pushAPIKey: Notification option for ``type`` :attr:`~.NotificationType.PUSHBYTECHULUS`.
+        :param str, optional telegramChatID: Notification option for ``type`` :attr:`~.NotificationType.TELEGRAM`.
+        :param bool telegramSendSilently: Notification option for ``type`` :attr:`~.NotificationType.TELEGRAM`.
+        :param bool telegramProtectContent: Notification option for ``type`` :attr:`~.NotificationType.TELEGRAM`.
+        :param str telegramMessageThreadID: Notification option for ``type`` :attr:`~.NotificationType.TELEGRAM`.
+        :param str, optional telegramBotToken: Notification option for ``type`` :attr:`~.NotificationType.TELEGRAM`.
+        :param str, optional twilioAccountSID: Notification option for ``type`` :attr:`~.NotificationType.TWILIO`. Account SID.
+        :param str, optional twilioAuthToken: Notification option for ``type`` :attr:`~.NotificationType.TWILIO`. Auth Token.
+        :param str, optional twilioToNumber: Notification option for ``type`` :attr:`~.NotificationType.TWILIO`. To Number.
+        :param str, optional twilioFromNumber: Notification option for ``type`` :attr:`~.NotificationType.TWILIO`. From Number.
+        :param str, optional webhookContentType: Notification option for ``type`` :attr:`~.NotificationType.WEBHOOK`.
+        :param str webhookAdditionalHeaders: Notification option for ``type`` :attr:`~.NotificationType.WEBHOOK`.
+        :param str, optional webhookURL: Notification option for ``type`` :attr:`~.NotificationType.WEBHOOK`.
+        :param str, optional weComBotKey: Notification option for ``type`` :attr:`~.NotificationType.WECOM`.
+        :param str, optional webhookUrl: Notification option for ``type`` :attr:`~.NotificationType.ZOHOCLIQ`.
     """
 
 
 def proxy_docstring(mode) -> str:
     return f"""
         :param ProxyProtocol{", optional" if mode == "edit" else ""} protocol: Proxy Protocol
         :param str{", optional" if mode == "edit" else ""} host: Proxy Server
@@ -267,19 +299,30 @@
 def docker_host_docstring(mode) -> str:
     return f"""
         :param str{", optional" if mode == "edit" else ""} name: Friendly Name
         :param DockerType{", optional" if mode == "edit" else ""} dockerType: Connection Type
         :param str, optional dockerDaemon: Docker Daemon, defaults to None
     """
 
+
 def maintenance_docstring(mode) -> str:
     return f"""
         :param str{", optional" if mode == "edit" else ""} title: Title
         :param MaintenanceStrategy{", optional" if mode == "edit" else ""} strategy: Strategy
         :param bool, optional active: True if maintenance is active, defaults to ``True``
         :param str, optional description: Description, defaults to ``""``
         :param list, optional dateRange: DateTime Range, defaults to ``["<current date>"]``
         :param int, optional intervalDay: Interval (Run once every day), defaults to ``1``
         :param list, optional weekdays: List that contains the days of the week on which the maintenance is enabled (Sun = ``0``, Mon = ``1``, ..., Sat = ``6``). Required for ``strategy`` :attr:`~.MaintenanceStrategy.RECURRING_WEEKDAY`., defaults to ``[]``.
-        :param list, optional daysOfMonth: List that contains the days of the month on which the maintenance is enabled (Day 1 = ``1``, Day 2 = ``2``, ..., Day 31 = ``31``) and the last day of the month (Last Day of Month = ``"lastDay1"``, 2nd Last Day of Month = ``"lastDay2"``, 3rd Last Day of Month = ``"lastDay3"``, 4th Last Day of Month = ``"lastDay4"``). Required for ``strategy`` :attr:`~.MaintenanceStrategy.RECURRING_DAY_OF_MONTH`., defaults to ``[]``.
+        :param list, optional daysOfMonth: List that contains the days of the month on which the maintenance is enabled (Day 1 = ``1``, Day 2 = ``2``, ..., Day 31 = ``31``) and the last day of the month (``"lastDay1"``). Required for ``strategy`` :attr:`~.MaintenanceStrategy.RECURRING_DAY_OF_MONTH`., defaults to ``[]``.
         :param list, optional timeRange: Maintenance Time Window of a Day, defaults to ``[{{"hours": 2, "minutes": 0}}, {{"hours": 3, "minutes": 0}}]``.
+        :param str, optional cron: Cron Schedule. Required for ``strategy`` :attr:`~.MaintenanceStrategy.CRON`., defaults to ``"30 3 * * *"``
+        :param int, optional durationMinutes: Duration (Minutes). Required for ``strategy`` :attr:`~.MaintenanceStrategy.CRON`., defaults to ``60``
+        :param str, optional timezone: Timezone, defaults to ``None`` (Server Timezone)
+    """
+
+
+def tag_docstring(mode) -> str:
+    return f"""
+        :param str{", optional" if mode == "edit" else ""} name: Tag name
+        :param str{", optional" if mode == "edit" else ""} color: Tag color
     """
```

### Comparing `uptime_kuma_api-0.9.0/uptime_kuma_api/event.py` & `uptime_kuma_api-1.0.0/uptime_kuma_api/event.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,7 +15,8 @@
     HEARTBEAT = "heartbeat"
     INFO = "info"
     CERT_INFO = "certInfo"
     DOCKER_HOST_LIST = "dockerHostList"
     AUTO_LOGIN = "autoLogin"
     INIT_SERVER_TIMEZONE = "initServerTimezone"
     MAINTENANCE_LIST = "maintenanceList"
+    API_KEY_LIST = "apiKeyList"
```

### Comparing `uptime_kuma_api-0.9.0/uptime_kuma_api/notification_providers.py` & `uptime_kuma_api-1.0.0/uptime_kuma_api/notification_providers.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,59 +3,92 @@
 
 class NotificationType(str, Enum):
     """Enumerate notification types."""
 
     ALERTA = "alerta"
     """Alerta"""
 
+    ALERTNOW = "AlertNow"
+    """AlertNow"""
+
     ALIYUNSMS = "AliyunSMS"
     """AliyunSMS"""
 
     APPRISE = "apprise"
     """Apprise (Support 50+ Notification services)"""
 
+    BARK = "Bark"
+    """Bark"""
+
     CLICKSENDSMS = "clicksendsms"
     """ClickSend SMS"""
 
     DINGDING = "DingDing"
     """DingDing"""
 
     DISCORD = "discord"
     """Discord"""
 
     FEISHU = "Feishu"
     """Feishu"""
 
+    FREEMOBILE = "FreeMobile"
+    """FreeMobile (mobile.free.fr)"""
+
+    GOALERT = "GoAlert"
+    """GoAlert"""
+
     GOOGLECHAT = "GoogleChat"
-    """Google Chat (Google Workspace only)"""
+    """Google Chat (Google Workspace)"""
 
     GORUSH = "gorush"
     """Gorush"""
 
     GOTIFY = "gotify"
     """Gotify"""
 
+    HOMEASSISTANT = "HomeAssistant"
+    """Home Assistant"""
+
+    KOOK = "Kook"
+    """Kook"""
+
     LINE = "line"
-    """Line Messenger"""
+    """LINE Messenger"""
+
+    LINENOTIFY = "LineNotify"
+    """LINE Notify"""
 
     LUNASEA = "lunasea"
     """LunaSea"""
 
     MATRIX = "matrix"
     """Matrix"""
 
     MATTERMOST = "mattermost"
     """Mattermost"""
 
+    NTFY = "ntfy"
+    """Ntfy"""
+
+    OCTOPUSH = "octopush"
+    """Octopush"""
+
     ONEBOT = "OneBot"
     """OneBot"""
 
+    OPSGENIE = "Opsgenie"
+    """Opsgenie"""
+
     PAGERDUTY = "PagerDuty"
     """PagerDuty"""
 
+    PAGERTREE = "PagerTree"
+    """PagerTree"""
+
     PROMOSMS = "promosms"
     """PromoSMS"""
 
     PUSHBULLET = "pushbullet"
     """Pushbullet"""
 
     PUSHDEER = "PushDeer"
@@ -66,356 +99,349 @@
 
     PUSHY = "pushy"
     """Pushy"""
 
     ROCKET_CHAT = "rocket.chat"
     """Rocket.Chat"""
 
+    SERVERCHAN = "ServerChan"
+    """ServerChan"""
+
     SERWERSMS = "serwersms"
     """SerwerSMS.pl"""
 
     SIGNAL = "signal"
     """Signal"""
 
     SLACK = "slack"
     """Slack"""
 
+    SMSEAGLE = "SMSEagle"
+    """SMSEagle"""
+
+    SMSMANAGER = "SMSManager"
+    """SmsManager (smsmanager.cz)"""
+
     SMTP = "smtp"
     """Email (SMTP)"""
 
+    SPLUNK = "Splunk"
+    """Splunk"""
+
+    SQUADCAST = "squadcast"
+    """SquadCast"""
+
     STACKFIELD = "stackfield"
     """Stackfield"""
 
+    TEAMS = "teams"
+    """Microsoft Teams"""
+
     PUSHBYTECHULUS = "PushByTechulus"
     """Push by Techulus"""
 
     TELEGRAM = "telegram"
     """Telegram"""
 
+    TWILIO = "twilio"
+    """Twilio"""
+
     WEBHOOK = "webhook"
     """Webhook"""
 
     WECOM = "WeCom"
     """WeCom"""
 
-    ALERTNOW = "AlertNow"
-    """AlertNow"""
-
-    HOMEASSISTANT = "HomeAssistant"
-    """Home Assistant"""
-
-    LINENOTIFY = "LineNotify"
-    """LineNotify"""
-
-    BARK = "Bark"
-    """Bark"""
-
-    GOALERT = "GoAlert"
-    """GoAlert"""
-
-    OCTOPUSH = "octopush"
-    """Octopush"""
-
-    SERVERCHAN = "ServerChan"
-    """ServerChan"""
-
-    SMSMANAGER = "SMSManager"
-    """SMSManager"""
-
-    SQUADCAST = "squadcast"
-    """Squadcast"""
-
-    TEAMS = "teams"
-    """Microsoft Teams"""
-
-    FREEMOBILE = "FreeMobile"
-    """FreeMobile"""
-
-    NTFY = "ntfy"
-    """ntfy"""
-
-    SMSEAGLE = "SMSEagle"
-    """SMSEagle"""
-
     ZOHOCLIQ = "ZohoCliq"
     """ZohoCliq"""
 
-    KOOK = "Kook"
-    """Kook"""
-
-    SPLUNK = "Splunk"
-    """Splunk"""
-
 
 notification_provider_options = {
     NotificationType.ALERTA: dict(
-        alertaApiEndpoint=dict(
-            type="str"
-        ),
-        alertaApiKey=dict(type="str"),
-        alertaEnvironment=dict(type="str"),
-        alertaAlertState=dict(type="str"),
-        alertaRecoverState=dict(type="str"),
+        alertaApiEndpoint=dict(type="str", required=True),
+        alertaApiKey=dict(type="str", required=True),
+        alertaEnvironment=dict(type="str", required=True),
+        alertaAlertState=dict(type="str", required=True),
+        alertaRecoverState=dict(type="str", required=True),
+    ),
+    NotificationType.ALERTNOW: dict(
+        alertNowWebhookURL=dict(type="str", required=True),
     ),
     NotificationType.ALIYUNSMS: dict(
-        phonenumber=dict(type="str"),
-        templateCode=dict(type="str"),
-        signName=dict(type="str"),
-        accessKeyId=dict(type="str"),
-        secretAccessKey=dict(type="str"),
+        phonenumber=dict(type="str", required=True),
+        templateCode=dict(type="str", required=True),
+        signName=dict(type="str", required=True),
+        accessKeyId=dict(type="str", required=True),
+        secretAccessKey=dict(type="str", required=True),
     ),
     NotificationType.APPRISE: dict(
-        appriseURL=dict(type="str"),
-        title=dict(type="str"),
+        appriseURL=dict(type="str", required=True),
+        title=dict(type="str", required=False),
+    ),
+    NotificationType.BARK: dict(
+        barkEndpoint=dict(type="str", required=True),
+        barkGroup=dict(type="str", required=True),
+        barkSound=dict(type="str", required=True),
     ),
     NotificationType.CLICKSENDSMS: dict(
-        clicksendsmsLogin=dict(type="str"),
-        clicksendsmsPassword=dict(type="str"),
-        clicksendsmsToNumber=dict(type="str"),
-        clicksendsmsSenderName=dict(type="str"),
+        clicksendsmsLogin=dict(type="str", required=True),
+        clicksendsmsPassword=dict(type="str", required=True),
+        clicksendsmsToNumber=dict(type="str", required=True),
+        clicksendsmsSenderName=dict(type="str", required=False),
     ),
     NotificationType.DINGDING: dict(
-        webHookUrl=dict(type="str"),
-        secretKey=dict(type="str"),
+        webHookUrl=dict(type="str", required=True),
+        secretKey=dict(type="str", required=True),
     ),
     NotificationType.DISCORD: dict(
-        discordUsername=dict(type="str"),
-        discordWebhookUrl=dict(type="str"),
-        discordPrefixMessage=dict(type="str"),
+        discordUsername=dict(type="str", required=False),
+        discordWebhookUrl=dict(type="str", required=True),
+        discordPrefixMessage=dict(type="str", required=False),
     ),
     NotificationType.FEISHU: dict(
-        feishuWebHookUrl=dict(type="str"),
+        feishuWebHookUrl=dict(type="str", required=True),
+    ),
+    NotificationType.FREEMOBILE: dict(
+        freemobileUser=dict(type="str", required=True),
+        freemobilePass=dict(type="str", required=True),
+    ),
+    NotificationType.GOALERT: dict(
+        goAlertBaseURL=dict(type="str", required=True),
+        goAlertToken=dict(type="str", required=True),
     ),
     NotificationType.GOOGLECHAT: dict(
-        googleChatWebhookURL=dict(type="str"),
+        googleChatWebhookURL=dict(type="str", required=True),
     ),
     NotificationType.GORUSH: dict(
-        gorushDeviceToken=dict(type="str"),
-        gorushPlatform=dict(type="str"),
-        gorushTitle=dict(type="str"),
-        gorushPriority=dict(type="str"),
-        gorushRetry=dict(type="str"),
-        gorushTopic=dict(type="str"),
-        gorushServerURL=dict(type="str"),
+        gorushDeviceToken=dict(type="str", required=True),
+        gorushPlatform=dict(type="str", required=False),
+        gorushTitle=dict(type="str", required=False),
+        gorushPriority=dict(type="str", required=False),
+        gorushRetry=dict(type="int", required=False),
+        gorushTopic=dict(type="str", required=False),
+        gorushServerURL=dict(type="str", required=True),
     ),
     NotificationType.GOTIFY: dict(
-        gotifyserverurl=dict(type="str"),
-        gotifyapplicationToken=dict(type="str"),
-        gotifyPriority=dict(type="int"),
+        gotifyserverurl=dict(type="str", required=True),
+        gotifyapplicationToken=dict(type="str", required=True),
+        gotifyPriority=dict(type="int", required=True),
+    ),
+    NotificationType.HOMEASSISTANT: dict(
+        notificationService=dict(type="str", required=False),
+        homeAssistantUrl=dict(type="str", required=True),
+        longLivedAccessToken=dict(type="str", required=True),
+    ),
+    NotificationType.KOOK: dict(
+        kookGuildID=dict(type="str", required=True),
+        kookBotToken=dict(type="str", required=True),
     ),
     NotificationType.LINE: dict(
-        lineChannelAccessToken=dict(type="str"),
-        lineUserID=dict(type="str"),
+        lineChannelAccessToken=dict(type="str", required=True),
+        lineUserID=dict(type="str", required=True),
+    ),
+    NotificationType.LINENOTIFY: dict(
+        lineNotifyAccessToken=dict(type="str", required=True),
     ),
     NotificationType.LUNASEA: dict(
-        lunaseaDevice=dict(type="str"),
+        lunaseaTarget=dict(type="str", required=True),
+        lunaseaUserID=dict(type="str", required=False),
+        lunaseaDevice=dict(type="str", required=False),
     ),
     NotificationType.MATRIX: dict(
-        internalRoomId=dict(type="str"),
-        accessToken=dict(type="str"),
-        homeserverUrl=dict(type="str"),
+        internalRoomId=dict(type="str", required=True),
+        accessToken=dict(type="str", required=True),
+        homeserverUrl=dict(type="str", required=True),
     ),
     NotificationType.MATTERMOST: dict(
-        mattermostusername=dict(type="str"),
-        mattermostWebhookUrl=dict(type="str"),
-        mattermostchannel=dict(type="str"),
-        mattermosticonemo=dict(type="str"),
-        mattermosticonurl=dict(type="str"),
+        mattermostusername=dict(type="str", required=False),
+        mattermostWebhookUrl=dict(type="str", required=True),
+        mattermostchannel=dict(type="str", required=False),
+        mattermosticonemo=dict(type="str", required=False),
+        mattermosticonurl=dict(type="str", required=False),
+    ),
+    NotificationType.NTFY: dict(
+        ntfyusername=dict(type="str", required=False),
+        ntfypassword=dict(type="str", required=False),
+        ntfytopic=dict(type="str", required=True),
+        ntfyPriority=dict(type="int", required=True),
+        ntfyIcon=dict(type="str", required=False),
+        ntfyserverurl=dict(type="str", required=True),
+    ),
+    NotificationType.OCTOPUSH: dict(
+        octopushVersion=dict(type="str", required=False),
+        octopushAPIKey=dict(type="str", required=True),
+        octopushLogin=dict(type="str", required=True),
+        octopushPhoneNumber=dict(type="str", required=True),
+        octopushSMSType=dict(type="str", required=False),
+        octopushSenderName=dict(type="str", required=False),
     ),
     NotificationType.ONEBOT: dict(
-        httpAddr=dict(type="str"),
-        accessToken=dict(type="str"),
-        msgType=dict(type="str"),
-        recieverId=dict(type="str"),
+        httpAddr=dict(type="str", required=True),
+        accessToken=dict(type="str", required=True),
+        msgType=dict(type="str", required=False),
+        recieverId=dict(type="str", required=True),
+    ),
+    NotificationType.OPSGENIE: dict(
+        opsgeniePriority=dict(type="int", required=False),
+        opsgenieRegion=dict(type="str", required=True),
+        opsgenieApiKey=dict(type="str", required=True),
     ),
     NotificationType.PAGERDUTY: dict(
-        pagerdutyAutoResolve=dict(type="str"),
-        pagerdutyIntegrationUrl=dict(type="str"),
-        pagerdutyPriority=dict(type="str"),
-        pagerdutyIntegrationKey=dict(type="str"),
+        pagerdutyAutoResolve=dict(type="str", required=False),
+        pagerdutyIntegrationUrl=dict(type="str", required=False),
+        pagerdutyPriority=dict(type="str", required=False),
+        pagerdutyIntegrationKey=dict(type="str", required=True),
+    ),
+    NotificationType.PAGERTREE: dict(
+        pagertreeAutoResolve=dict(type="str", required=False),
+        pagertreeIntegrationUrl=dict(type="str", required=False),
+        pagertreeUrgency=dict(type="str", required=False),
     ),
     NotificationType.PROMOSMS: dict(
-        promosmsLogin=dict(type="str"),
-        promosmsPassword=dict(type="str"),
-        promosmsPhoneNumber=dict(type="str"),
-        promosmsSMSType=dict(type="str"),
-        promosmsSenderName=dict(type="str"),
-        promosmsAllowLongSMS=dict(type="bool"),
+        promosmsAllowLongSMS=dict(type="bool", required=False),
+        promosmsLogin=dict(type="str", required=True),
+        promosmsPassword=dict(type="str", required=True),
+        promosmsPhoneNumber=dict(type="str", required=True),
+        promosmsSMSType=dict(type="str", required=False),
+        promosmsSenderName=dict(type="str", required=False),
     ),
     NotificationType.PUSHBULLET: dict(
-        pushbulletAccessToken=dict(type="str"),
+        pushbulletAccessToken=dict(type="str", required=True),
     ),
     NotificationType.PUSHDEER: dict(
-        pushdeerKey=dict(type="str"),
+        pushdeerKey=dict(type="str", required=True),
     ),
     NotificationType.PUSHOVER: dict(
-        pushoveruserkey=dict(type="str"),
-        pushoverapptoken=dict(type="str"),
-        pushoversounds=dict(type="str"),
-        pushoverpriority=dict(type="str"),
-        pushovertitle=dict(type="str"),
-        pushoverdevice=dict(type="str"),
+        pushoveruserkey=dict(type="str", required=True),
+        pushoverapptoken=dict(type="str", required=True),
+        pushoversounds=dict(type="str", required=False),
+        pushoverpriority=dict(type="str", required=False),
+        pushovertitle=dict(type="str", required=False),
+        pushoverdevice=dict(type="str", required=False),
     ),
     NotificationType.PUSHY: dict(
-        pushyAPIKey=dict(type="str"),
-        pushyToken=dict(type="str"),
+        pushyAPIKey=dict(type="str", required=True),
+        pushyToken=dict(type="str", required=True),
     ),
     NotificationType.ROCKET_CHAT: dict(
-        rocketchannel=dict(type="str"),
-        rocketusername=dict(type="str"),
-        rocketiconemo=dict(type="str"),
-        rocketwebhookURL=dict(type="str"),
-        rocketbutton=dict(type="str"),
+        rocketchannel=dict(type="str", required=False),
+        rocketusername=dict(type="str", required=False),
+        rocketiconemo=dict(type="str", required=False),
+        rocketwebhookURL=dict(type="str", required=True),
+    ),
+    NotificationType.SERVERCHAN: dict(
+        serverChanSendKey=dict(type="str", required=True),
     ),
     NotificationType.SERWERSMS: dict(
-        serwersmsUsername=dict(type="str"),
-        serwersmsPassword=dict(type="str"),
-        serwersmsPhoneNumber=dict(type="str"),
-        serwersmsSenderName=dict(type="str"),
+        serwersmsUsername=dict(type="str", required=True),
+        serwersmsPassword=dict(type="str", required=True),
+        serwersmsPhoneNumber=dict(type="str", required=True),
+        serwersmsSenderName=dict(type="str", required=False),
     ),
     NotificationType.SIGNAL: dict(
-        signalNumber=dict(type="str"),
-        signalRecipients=dict(type="str"),
-        signalURL=dict(type="str"),
+        signalNumber=dict(type="str", required=True),
+        signalRecipients=dict(type="str", required=True),
+        signalURL=dict(type="str", required=True),
     ),
     NotificationType.SLACK: dict(
-        slackbutton=dict(type="str"),
-        slackchannel=dict(type="str"),
-        slackusername=dict(type="str"),
-        slackiconemo=dict(type="str"),
-        slackwebhookURL=dict(type="str"),
+        slackchannel=dict(type="str", required=False),
+        slackusername=dict(type="str", required=False),
+        slackiconemo=dict(type="str", required=False),
+        slackwebhookURL=dict(type="str", required=True),
+    ),
+    NotificationType.SMSEAGLE: dict(
+        smseagleEncoding=dict(type="bool", required=False),
+        smseaglePriority=dict(type="int", required=False),
+        smseagleRecipientType=dict(type="str", required=False),
+        smseagleToken=dict(type="str", required=True),
+        smseagleRecipient=dict(type="str", required=True),
+        smseagleUrl=dict(type="str", required=True),
+    ),
+    NotificationType.SMSMANAGER: dict(
+        smsmanagerApiKey=dict(type="str", required=False),
+        numbers=dict(type="str", required=False),
+        messageType=dict(type="str", required=False),
     ),
     NotificationType.SMTP: dict(
-        smtpHost=dict(type="str"),
-        smtpPort=dict(type="int"),
-        smtpSecure=dict(type="str"),
-        smtpIgnoreTLSError=dict(type="str"),
-        smtpDkimDomain=dict(type="str"),
-        smtpDkimKeySelector=dict(type="str"),
-        smtpDkimPrivateKey=dict(type="str"),
-        smtpDkimHashAlgo=dict(type="str"),
-        smtpDkimheaderFieldNames=dict(type="str"),
-        smtpDkimskipFields=dict(type="str"),
-        smtpUsername=dict(type="str"),
-        smtpPassword=dict(type="str"),
-        customSubject=dict(type="str"),
-        smtpFrom=dict(type="str"),
-        smtpCC=dict(type="str"),
-        smtpBCC=dict(type="str"),
-        smtpTo=dict(type="str"),
+        smtpHost=dict(type="str", required=True),
+        smtpPort=dict(type="int", required=True),
+        smtpSecure=dict(type="str", required=False),
+        smtpIgnoreTLSError=dict(type="bool", required=False),
+        smtpDkimDomain=dict(type="str", required=False),
+        smtpDkimKeySelector=dict(type="str", required=False),
+        smtpDkimPrivateKey=dict(type="str", required=False),
+        smtpDkimHashAlgo=dict(type="str", required=False),
+        smtpDkimheaderFieldNames=dict(type="str", required=False),
+        smtpDkimskipFields=dict(type="str", required=False),
+        smtpUsername=dict(type="str", required=False),
+        smtpPassword=dict(type="str", required=False),
+        customSubject=dict(type="str", required=False),
+        smtpFrom=dict(type="str", required=True),
+        smtpCC=dict(type="str", required=False),
+        smtpBCC=dict(type="str", required=False),
+        smtpTo=dict(type="str", required=False),
+    ),
+    NotificationType.SPLUNK: dict(
+        splunkAutoResolve=dict(type="str", required=False),
+        splunkSeverity=dict(type="str", required=False),
+        splunkRestURL=dict(type="str", required=True),
+    ),
+    NotificationType.SQUADCAST: dict(
+        squadcastWebhookURL=dict(type="str", required=True),
     ),
     NotificationType.STACKFIELD: dict(
-        stackfieldwebhookURL=dict(type="str"),
+        stackfieldwebhookURL=dict(type="str", required=True),
+    ),
+    NotificationType.TEAMS: dict(
+        webhookUrl=dict(type="str", required=True),
     ),
     NotificationType.PUSHBYTECHULUS: dict(
-        pushAPIKey=dict(type="str"),
+        pushAPIKey=dict(type="str", required=True),
     ),
     NotificationType.TELEGRAM: dict(
-        telegramBotToken=dict(type="str"),
-        telegramChatID=dict(type="str"),
+        telegramChatID=dict(type="str", required=True),
+        telegramSendSilently=dict(type="bool", required=False),
+        telegramProtectContent=dict(type="bool", required=False),
+        telegramMessageThreadID=dict(type="str", required=False),
+        telegramBotToken=dict(type="str", required=True),
+    ),
+    NotificationType.TWILIO: dict(
+        twilioAccountSID=dict(type="str", required=True),
+        twilioAuthToken=dict(type="str", required=True),
+        twilioToNumber=dict(type="str", required=True),
+        twilioFromNumber=dict(type="str", required=True),
     ),
     NotificationType.WEBHOOK: dict(
-        webhookContentType=dict(type="str"),
-        webhookAdditionalHeaders=dict(type="str"),
-        webhookURL=dict(type="str"),
+        webhookContentType=dict(type="str", required=True),
+        webhookAdditionalHeaders=dict(type="str", required=False),
+        webhookURL=dict(type="str", required=True),
     ),
     NotificationType.WECOM: dict(
-        weComBotKey=dict(type="str"),
-    ),
-    NotificationType.ALERTNOW: dict(
-        alertNowWebhookURL=dict(type="str"),
-    ),
-    NotificationType.HOMEASSISTANT: dict(
-        homeAssistantUrl=dict(type="str"),
-        longLivedAccessToken=dict(type="str"),
-    ),
-    NotificationType.LINENOTIFY: dict(
-        lineNotifyAccessToken=dict(type="str"),
-    ),
-    NotificationType.BARK: dict(
-        barkEndpoint=dict(type="str"),
-        barkGroup=dict(type="str"),
-        barkSound=dict(type="str"),
-    ),
-    NotificationType.GOALERT: dict(
-        goAlertBaseURL=dict(type="str"),
-        goAlertToken=dict(type="str"),
-    ),
-    NotificationType.OCTOPUSH: dict(
-        octopushVersion=dict(type="str"),
-        octopushAPIKey=dict(type="str"),
-        octopushLogin=dict(type="str"),
-        octopushPhoneNumber=dict(type="str"),
-        octopushSMSType=dict(type="str"),
-        octopushSenderName=dict(type="str"),
-        octopushDMLogin=dict(type="str"),
-        octopushDMAPIKey=dict(type="str"),
-        octopushDMPhoneNumber=dict(type="str"),
-        octopushDMSenderName=dict(type="str"),
-        octopushDMSMSType=dict(type="str"),
-    ),
-    NotificationType.SERVERCHAN: dict(
-        serverChanSendKey=dict(type="str"),
-    ),
-    NotificationType.SMSMANAGER: dict(
-        smsmanagerApiKey=dict(type="str"),
-        numbers=dict(type="str"),
-        messageType=dict(type="str"),
-    ),
-    NotificationType.SQUADCAST: dict(
-        squadcastWebhookURL=dict(type="str"),
-    ),
-    NotificationType.TEAMS: dict(
-        webhookUrl=dict(type="str"),
-    ),
-    NotificationType.FREEMOBILE: dict(
-        freemobileUser=dict(type="str"),
-        freemobilePass=dict(type="str"),
-    ),
-    NotificationType.NTFY: dict(
-        ntfyusername=dict(type="str"),
-        ntfypassword=dict(type="str"),
-        ntfytopic=dict(type="str"),
-        ntfyPriority=dict(type="int"),
-        ntfyIcon=dict(type="str"),
-        ntfyserverurl=dict(type="str"),
-    ),
-    NotificationType.SMSEAGLE: dict(
-        smseagleEncoding=dict(type="bool"),
-        smseaglePriority=dict(type="int"),
-        smseagleRecipientType=dict(type="str"),
-        smseagleToken=dict(type="str"),
-        smseagleRecipient=dict(type="str"),
-        smseagleUrl=dict(type="str")
+        weComBotKey=dict(type="str", required=True),
     ),
     NotificationType.ZOHOCLIQ: dict(
-        webhookUrl=dict(type="str")
-    ),
-    NotificationType.KOOK: dict(
-        kookGuildID=dict(type="str"),
-        kookBotToken=dict(type="str")
+        webhookUrl=dict(type="str", required=True),
     ),
-    NotificationType.SPLUNK: dict(
-        splunkAutoResolve=dict(type="str"),
-        splunkSeverity=dict(type="str"),
-        splunkRestURL=dict(type="str")
-    )
 }
 
 notification_provider_conditions = dict(
     gotifyPriority=dict(
         min=0,
-        max=10
-    ),
-    smtpPort=dict(
-        min=0,
-        max=65535
+        max=10,
     ),
     ntfyPriority=dict(
         min=1,
-        max=5
+        max=5,
+    ),
+    opsgeniePriority=dict(
+        min=1,
+        max=5,
     ),
     smseaglePriority=dict(
         min=0,
-        max=9
-    )
+        max=9,
+    ),
+    smtpPort=dict(
+        min=0,
+        max=65535,
+    ),
 )
```

### Comparing `uptime_kuma_api-0.9.0/uptime_kuma_api.egg-info/PKG-INFO` & `uptime_kuma_api-1.0.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,80 +1,101 @@
 Metadata-Version: 2.1
-Name: uptime-kuma-api
-Version: 0.9.0
+Name: uptime_kuma_api
+Version: 1.0.0
 Summary: A python wrapper for the Uptime Kuma WebSocket API
 Home-page: https://github.com/lucasheld/uptime-kuma-api
 Author: Lucas Held
 Author-email: lucasheld@hotmail.de
 License: MIT
-Description: # uptime-kuma-api
-        
-        A wrapper for the Uptime Kuma Socket.IO API
-        ---
-        uptime-kuma-api is a Python wrapper for the [Uptime Kuma](https://github.com/louislam/uptime-kuma) Socket.IO API.
-        
-        This package was developed to configure Uptime Kuma with Ansible. The Ansible collection can be found at https://github.com/lucasheld/ansible-uptime-kuma.
-        
-        Python version 3.6+ is required.
-        
-        Supported Uptime Kuma versions: 1.17.0 - 1.19.5
-        
-        Installation
-        ---
-        uptime-kuma-api is available on the [Python Package Index (PyPI)](https://pypi.org/project/uptime-kuma-api/).
-        
-        You can install it using pip:
-        
-        ```
-        pip install uptime-kuma-api
-        ```
-        
-        Documentation
-        ---
-        The API Reference is available on [Read the Docs](https://uptime-kuma-api.readthedocs.io).
-        
-        Examples
-        ---
-        Once you have installed the python package, you can use it to communicate with an Uptime Kuma instance.
-        
-        To do so, import `UptimeKumaApi` from the library and specify the Uptime Kuma server url (e.g. 'http://127.0.0.1:3001'), username and password to initialize the connection.
-        
-        ```python
-        >>> from uptime_kuma_api import UptimeKumaApi, MonitorType
-        >>> api = UptimeKumaApi('INSERT_URL')
-        >>> api.login('INSERT_USERNAME', 'INSERT_PASSWORD')
-        ```
-        
-        Now you can call one of the existing methods of the instance. For example create a new monitor:
-        
-        ```python
-        >>> result = api.add_monitor(type=MonitorType.HTTP, name="Google", url="https://google.com")
-        >>> print(result)
-        {'msg': 'Added Successfully.', 'monitorId': 1}
-        ```
-        
-        At the end, the connection to the API must be disconnected so that the program does not block.
-        
-        ```python
-        >>> api.disconnect()
-        ```
-        
 Platform: UNKNOWN
-Classifier: Development Status :: 1 - Planning
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Libraries
-Requires-Python: >=3.6, <4
+Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# uptime-kuma-api
+
+A wrapper for the Uptime Kuma Socket.IO API
+---
+uptime-kuma-api is a Python wrapper for the [Uptime Kuma](https://github.com/louislam/uptime-kuma) Socket.IO API.
+
+This package was developed to configure Uptime Kuma with Ansible. The Ansible collection can be found at https://github.com/lucasheld/ansible-uptime-kuma.
+
+Python version 3.7+ is required.
+
+Supported Uptime Kuma versions:
+
+| Uptime Kuma     | uptime-kuma-api |
+|-----------------|-----------------|
+| 1.21.3          | 1.0.0           |
+| 1.17.0 - 1.21.2 | 0.1.0 - 0.13.0  |
+
+Installation
+---
+uptime-kuma-api is available on the [Python Package Index (PyPI)](https://pypi.org/project/uptime-kuma-api/).
+
+You can install it using pip:
+
+```
+pip install uptime-kuma-api
+```
+
+Documentation
+---
+The API Reference is available on [Read the Docs](https://uptime-kuma-api.readthedocs.io).
+
+Example
+---
+Once you have installed the python package, you can use it to communicate with an Uptime Kuma instance.
+
+To do so, import `UptimeKumaApi` from the library and specify the Uptime Kuma server url (e.g. 'http://127.0.0.1:3001'), username and password to initialize the connection.
+
+```python
+>>> from uptime_kuma_api import UptimeKumaApi, MonitorType
+>>> api = UptimeKumaApi('INSERT_URL')
+>>> api.login('INSERT_USERNAME', 'INSERT_PASSWORD')
+```
+
+Now you can call one of the existing methods of the instance. For example create a new monitor:
+
+```python
+>>> result = api.add_monitor(type=MonitorType.HTTP, name="Google", url="https://google.com")
+>>> print(result)
+{'msg': 'Added Successfully.', 'monitorId': 1}
+```
+
+At the end, the connection to the API must be disconnected so that the program does not block.
+
+```python
+>>> api.disconnect()
+```
+
+With a context manager, the disconnect method is called automatically:
+
+```python
+from uptime_kuma_api import UptimeKumaApi
+
+with UptimeKumaApi('INSERT_URL') as api:
+    api.login('INSERT_USERNAME', 'INSERT_PASSWORD')
+    api.add_monitor(
+        type=MonitorType.HTTP,
+        name="Google",
+        url="https://google.com"
+    )
+```
+
+
```

### Comparing `uptime_kuma_api-0.9.0/uptime_kuma_api.egg-info/SOURCES.txt` & `uptime_kuma_api-1.0.0/uptime_kuma_api.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 uptime_kuma_api/auth_method.py
 uptime_kuma_api/docker_type.py
 uptime_kuma_api/docstrings.py
 uptime_kuma_api/event.py
 uptime_kuma_api/exceptions.py
 uptime_kuma_api/incident_style.py
 uptime_kuma_api/maintenance_strategy.py
+uptime_kuma_api/monitor_status.py
 uptime_kuma_api/monitor_type.py
 uptime_kuma_api/notification_providers.py
 uptime_kuma_api/proxy_protocol.py
 uptime_kuma_api.egg-info/PKG-INFO
 uptime_kuma_api.egg-info/SOURCES.txt
 uptime_kuma_api.egg-info/dependency_links.txt
 uptime_kuma_api.egg-info/requires.txt
```

