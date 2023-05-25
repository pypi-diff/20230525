# Comparing `tmp/miris-manager-client-5.5.tar.gz` & `tmp/miris-manager-client-6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miris-manager-client-5.5.tar", last modified: Wed Mar  8 14:53:07 2023, max compression
+gzip compressed data, was "miris-manager-client-6.0.tar", last modified: Thu May 25 07:57:07 2023, max compression
```

## Comparing `miris-manager-client-5.5.tar` & `miris-manager-client-6.0.tar`

### file list

```diff
@@ -1,25 +1,28 @@
-drwxr-xr-x   0 djdev     (1000) djdev     (1000)        0 2023-03-08 14:53:07.084943 miris-manager-client-5.5/
--rw-rw-r--   0 djdev     (1000) djdev     (1000)     7651 2016-05-28 07:08:30.000000 miris-manager-client-5.5/LICENSE
--rw-r--r--   0 djdev     (1000) djdev     (1000)     3931 2023-03-08 14:53:07.084943 miris-manager-client-5.5/PKG-INFO
--rw-r--r--   0 djdev     (1000) djdev     (1000)     3055 2023-03-08 14:49:03.000000 miris-manager-client-5.5/README.md
-drwxr-xr-x   0 djdev     (1000) djdev     (1000)        0 2023-03-08 14:53:07.084943 miris-manager-client-5.5/miris_manager_client.egg-info/
--rw-r--r--   0 djdev     (1000) djdev     (1000)     3931 2023-03-08 14:53:07.000000 miris-manager-client-5.5/miris_manager_client.egg-info/PKG-INFO
--rw-r--r--   0 djdev     (1000) djdev     (1000)      498 2023-03-08 14:53:07.000000 miris-manager-client-5.5/miris_manager_client.egg-info/SOURCES.txt
--rw-r--r--   0 djdev     (1000) djdev     (1000)        1 2023-03-08 14:53:07.000000 miris-manager-client-5.5/miris_manager_client.egg-info/dependency_links.txt
--rw-r--r--   0 djdev     (1000) djdev     (1000)       29 2023-03-08 14:53:07.000000 miris-manager-client-5.5/miris_manager_client.egg-info/requires.txt
--rw-r--r--   0 djdev     (1000) djdev     (1000)       10 2023-03-08 14:53:07.000000 miris-manager-client-5.5/miris_manager_client.egg-info/top_level.txt
-drwxr-xr-x   0 djdev     (1000) djdev     (1000)        0 2023-03-08 14:53:07.084943 miris-manager-client-5.5/mm_client/
--rw-r--r--   0 djdev     (1000) djdev     (1000)       20 2023-03-08 14:50:37.000000 miris-manager-client-5.5/mm_client/__init__.py
--rw-r--r--   0 djdev     (1000) djdev     (1000)     9651 2023-03-08 14:51:34.000000 miris-manager-client-5.5/mm_client/client.py
--rw-r--r--   0 djdev     (1000) djdev     (1000)     2900 2021-07-30 13:58:37.000000 miris-manager-client-5.5/mm_client/conf.py
-drwxr-xr-x   0 djdev     (1000) djdev     (1000)        0 2023-03-08 14:53:07.084943 miris-manager-client-5.5/mm_client/lib/
--rw-rw-r--   0 djdev     (1000) djdev     (1000)        0 2018-06-08 15:42:33.000000 miris-manager-client-5.5/mm_client/lib/__init__.py
--rw-r--r--   0 djdev     (1000) djdev     (1000)     2722 2023-03-08 14:50:53.000000 miris-manager-client-5.5/mm_client/lib/configuration.py
--rw-r--r--   0 djdev     (1000) djdev     (1000)     1472 2023-03-08 14:50:58.000000 miris-manager-client-5.5/mm_client/lib/info.py
--rw-r--r--   0 djdev     (1000) djdev     (1000)     3757 2023-03-08 14:51:04.000000 miris-manager-client-5.5/mm_client/lib/long_polling.py
--rw-rw-r--   0 djdev     (1000) djdev     (1000)     1907 2023-03-08 14:51:08.000000 miris-manager-client-5.5/mm_client/lib/signing.py
--rw-r--r--   0 djdev     (1000) djdev     (1000)    13191 2023-03-08 14:51:13.000000 miris-manager-client-5.5/mm_client/lib/ssh_tunnel.py
--rw-r--r--   0 djdev     (1000) djdev     (1000)     1121 2023-03-08 14:53:07.084943 miris-manager-client-5.5/setup.cfg
--rwxr-xr-x   0 djdev     (1000) djdev     (1000)       63 2019-05-23 14:56:48.000000 miris-manager-client-5.5/setup.py
-drwxr-xr-x   0 djdev     (1000) djdev     (1000)        0 2023-03-08 14:53:07.084943 miris-manager-client-5.5/tests/
--rw-rw-r--   0 djdev     (1000) djdev     (1000)     1807 2021-07-30 14:29:06.000000 miris-manager-client-5.5/tests/test_client.py
+drwxr-xr-x   0     1000     1000        0 2023-05-25 07:57:07.253495 miris-manager-client-6.0/
+-rw-rw-r--   0     1000     1000     7651 2016-05-28 07:08:30.000000 miris-manager-client-6.0/LICENSE
+-rw-r--r--   0     1000     1000     4360 2023-05-25 07:57:07.253495 miris-manager-client-6.0/PKG-INFO
+-rw-r--r--   0     1000     1000     3484 2023-05-17 08:33:19.000000 miris-manager-client-6.0/README.md
+drwxr-xr-x   0     1000     1000        0 2023-05-25 07:57:07.249495 miris-manager-client-6.0/miris_manager_client.egg-info/
+-rw-r--r--   0     1000     1000     4360 2023-05-25 07:57:07.000000 miris-manager-client-6.0/miris_manager_client.egg-info/PKG-INFO
+-rw-r--r--   0     1000     1000      560 2023-05-25 07:57:07.000000 miris-manager-client-6.0/miris_manager_client.egg-info/SOURCES.txt
+-rw-r--r--   0     1000     1000        1 2023-05-25 07:57:07.000000 miris-manager-client-6.0/miris_manager_client.egg-info/dependency_links.txt
+-rw-r--r--   0     1000     1000       55 2023-05-25 07:57:07.000000 miris-manager-client-6.0/miris_manager_client.egg-info/requires.txt
+-rw-r--r--   0     1000     1000       10 2023-05-25 07:57:07.000000 miris-manager-client-6.0/miris_manager_client.egg-info/top_level.txt
+drwxr-xr-x   0     1000     1000        0 2023-05-25 07:57:07.253495 miris-manager-client-6.0/mm_client/
+-rw-r--r--   0     1000     1000       20 2023-05-10 07:13:18.000000 miris-manager-client-6.0/mm_client/__init__.py
+-rw-r--r--   0     1000     1000    10438 2023-05-17 08:33:19.000000 miris-manager-client-6.0/mm_client/client.py
+-rw-r--r--   0     1000     1000     2900 2021-07-30 13:58:37.000000 miris-manager-client-6.0/mm_client/conf.py
+drwxr-xr-x   0     1000     1000        0 2023-05-25 07:57:07.253495 miris-manager-client-6.0/mm_client/lib/
+-rw-rw-r--   0     1000     1000        0 2018-06-08 15:42:33.000000 miris-manager-client-6.0/mm_client/lib/__init__.py
+-rw-r--r--   0     1000     1000     2900 2023-05-10 07:13:29.000000 miris-manager-client-6.0/mm_client/lib/configuration.py
+-rw-r--r--   0     1000     1000     1472 2023-03-08 14:50:58.000000 miris-manager-client-6.0/mm_client/lib/info.py
+-rw-r--r--   0     1000     1000     4402 2023-05-17 08:33:19.000000 miris-manager-client-6.0/mm_client/lib/long_polling.py
+-rw-r--r--   0     1000     1000     1843 2023-05-17 08:33:19.000000 miris-manager-client-6.0/mm_client/lib/signing.py
+-rw-r--r--   0     1000     1000    14096 2023-05-09 08:52:05.000000 miris-manager-client-6.0/mm_client/lib/ssh_tunnel.py
+-rw-r--r--   0     1000     1000     1150 2023-05-25 07:57:07.253495 miris-manager-client-6.0/setup.cfg
+-rwxr-xr-x   0     1000     1000       63 2019-05-23 14:56:48.000000 miris-manager-client-6.0/setup.py
+drwxr-xr-x   0     1000     1000        0 2023-05-25 07:57:07.253495 miris-manager-client-6.0/tests/
+-rw-r--r--   0     1000     1000     2366 2023-05-17 08:33:19.000000 miris-manager-client-6.0/tests/test_client.py
+-rw-r--r--   0     1000     1000     1903 2023-05-10 07:25:56.000000 miris-manager-client-6.0/tests/test_conf.py
+-rw-r--r--   0     1000     1000      589 2023-05-10 07:24:12.000000 miris-manager-client-6.0/tests/test_info.py
+-rw-r--r--   0     1000     1000     1518 2023-05-17 08:33:19.000000 miris-manager-client-6.0/tests/test_signature.py
```

### Comparing `miris-manager-client-5.5/LICENSE` & `miris-manager-client-6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `miris-manager-client-5.5/PKG-INFO` & `miris-manager-client-6.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miris-manager-client
-Version: 5.5
+Version: 6.0
 Summary: A Python3 client to use Miris Manager remote control
 Home-page: https://www.ubicast.eu/en/solutions/delivery/
 Download-URL: https://github.com/UbiCastTeam/miris-manager-client
 Author: UbiCast
 Author-email: dev@ubicast.eu
 License: LGPLv3
 Keywords: api,client,miris,manager,ubicast
@@ -28,21 +28,21 @@
 A Python3 client to use UbiCast Miris Manager remote control API.
 
 This client is intended to act as a system in Miris Manager so it allows you to integrate a device in order to control it using Miris Manager.
 
 
 ## Requirements
 
-git
-python >= 3.9 (download the latest stable release from https://www.python.org/downloads/)
+* python >= 3.9 (download the latest stable release from https://www.python.org/downloads/)
+* python3-requests >= 2.30
 
 
 ## Important
 
-For production use, it is recommended to use the branch named "stable". The "master" branch is used for development.
+For production use, it is recommended to use the branch named "stable". The "main" branch is used for development.
 
 
 ## Client class instantiation
 
 The client class (`mm_client`.`client`.`MirisManagerClient`) takes two arguments:
 * `local_conf`: This argument can be either a dict or a path (`str` object). The default value is `None`, which means no configuration.
 * `setup_logging`: This argument must be a boolean. If set to `True`, the logging to console will be configured. The default value is `True`.
@@ -64,39 +64,63 @@
 * Replace the import path of `MirisManagerClient` (see example).
 * Replace the class variable `MirisManagerClient`.`LOCAL_CONF` with the class instance argument `MirisManagerClient`.`local_conf`.
 * Check the value of `MirisManagerClient`.`DEFAULT_CONF` because it is now `None` by default.
 * Replace all occurences of `URL` by `SERVER_URL` in all configuration.
 * Replace all occurences of `CHECK_SSL` by `VERIFY_SSL` in all configuration.
 
 
-## Example
+## Examples
 
 ### Ping the server
 
 ``` python
 from mm_client.client import MirisManagerClient
 mmc = MirisManagerClient(local_conf='your-conf.json')
 
 response = mmc.api_request('PING')
 print(response)
 ```
 
-There are more examples in the `examples` directory.
+
+### Recorder system
+
+This example is the use case of a recorder system that can be controlled through the long polling.
+
+[Link to the file](/examples/recorder_controller.py)
+
+
+### Wake on LAN requests
+
+This example is the use case of a client that forwards wake on LAN requests received through the long polling to its network.
+
+[Link to the file](/examples/wol_relay.py)
+
+
+### Other examples
+
+There are more examples in the [examples](/examples) directory.
 
 
 ## Actions
 
 Here is the list of actions that can be sent to the client depending on its supported capabilities:
 
-    # Basic actions
-    SHUTDOWN: capability: shutdown, description: Shutdown system
-    REBOOT: capability: reboot, description: Reboot system
-    UPGRADE: capability: upgrade, description: Upgrade system software
-    # Recording
-    START_RECORDING: capability: record, description: Start recording
-    STOP_RECORDING: capability: record, description: Stop recording
-    LIST_PROFILES: capability: record, description: Refresh profiles list
-    # Publishing
-    START_PUBLISHING: capability: publish, description: Start publishing non published media
-    STOP_PUBLISHING: capability: publish, description: Stop publishing
-    # Wake on lan
-    WAKE_ON_LAN_SEND: capability: send_wake_on_lan, description: Send a wake on LAN network package from this system to wake another system
+**Basic actions**
+
+* `SHUTDOWN`: capability: shutdown, description: Shutdown system
+* `REBOOT`: capability: reboot, description: Reboot system
+* `UPGRADE`: capability: upgrade, description: Upgrade system software
+
+**Recording**
+
+* `START_RECORDING`: capability: record, description: Start recording
+* `STOP_RECORDING`: capability: record, description: Stop recording
+* `LIST_PROFILES`: capability: record, description: Refresh profiles list
+
+**Publishing**
+
+* `START_PUBLISHING`: capability: publish, description: Start publishing non published media
+* `STOP_PUBLISHING`: capability: publish, description: Stop publishing
+
+**Wake on lan**
+
+* `WAKE_ON_LAN_SEND`: capability: send_wake_on_lan, description: Send a wake on LAN network package from this system to wake another system
```

### Comparing `miris-manager-client-5.5/README.md` & `miris-manager-client-6.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 A Python3 client to use UbiCast Miris Manager remote control API.
 
 This client is intended to act as a system in Miris Manager so it allows you to integrate a device in order to control it using Miris Manager.
 
 
 ## Requirements
 
-git
-python >= 3.9 (download the latest stable release from https://www.python.org/downloads/)
+* python >= 3.9 (download the latest stable release from https://www.python.org/downloads/)
+* python3-requests >= 2.30
 
 
 ## Important
 
-For production use, it is recommended to use the branch named "stable". The "master" branch is used for development.
+For production use, it is recommended to use the branch named "stable". The "main" branch is used for development.
 
 
 ## Client class instantiation
 
 The client class (`mm_client`.`client`.`MirisManagerClient`) takes two arguments:
 * `local_conf`: This argument can be either a dict or a path (`str` object). The default value is `None`, which means no configuration.
 * `setup_logging`: This argument must be a boolean. If set to `True`, the logging to console will be configured. The default value is `True`.
@@ -42,39 +42,63 @@
 * Replace the import path of `MirisManagerClient` (see example).
 * Replace the class variable `MirisManagerClient`.`LOCAL_CONF` with the class instance argument `MirisManagerClient`.`local_conf`.
 * Check the value of `MirisManagerClient`.`DEFAULT_CONF` because it is now `None` by default.
 * Replace all occurences of `URL` by `SERVER_URL` in all configuration.
 * Replace all occurences of `CHECK_SSL` by `VERIFY_SSL` in all configuration.
 
 
-## Example
+## Examples
 
 ### Ping the server
 
 ``` python
 from mm_client.client import MirisManagerClient
 mmc = MirisManagerClient(local_conf='your-conf.json')
 
 response = mmc.api_request('PING')
 print(response)
 ```
 
-There are more examples in the `examples` directory.
+
+### Recorder system
+
+This example is the use case of a recorder system that can be controlled through the long polling.
+
+[Link to the file](/examples/recorder_controller.py)
+
+
+### Wake on LAN requests
+
+This example is the use case of a client that forwards wake on LAN requests received through the long polling to its network.
+
+[Link to the file](/examples/wol_relay.py)
+
+
+### Other examples
+
+There are more examples in the [examples](/examples) directory.
 
 
 ## Actions
 
 Here is the list of actions that can be sent to the client depending on its supported capabilities:
 
-    # Basic actions
-    SHUTDOWN: capability: shutdown, description: Shutdown system
-    REBOOT: capability: reboot, description: Reboot system
-    UPGRADE: capability: upgrade, description: Upgrade system software
-    # Recording
-    START_RECORDING: capability: record, description: Start recording
-    STOP_RECORDING: capability: record, description: Stop recording
-    LIST_PROFILES: capability: record, description: Refresh profiles list
-    # Publishing
-    START_PUBLISHING: capability: publish, description: Start publishing non published media
-    STOP_PUBLISHING: capability: publish, description: Stop publishing
-    # Wake on lan
-    WAKE_ON_LAN_SEND: capability: send_wake_on_lan, description: Send a wake on LAN network package from this system to wake another system
+**Basic actions**
+
+* `SHUTDOWN`: capability: shutdown, description: Shutdown system
+* `REBOOT`: capability: reboot, description: Reboot system
+* `UPGRADE`: capability: upgrade, description: Upgrade system software
+
+**Recording**
+
+* `START_RECORDING`: capability: record, description: Start recording
+* `STOP_RECORDING`: capability: record, description: Stop recording
+* `LIST_PROFILES`: capability: record, description: Refresh profiles list
+
+**Publishing**
+
+* `START_PUBLISHING`: capability: publish, description: Start publishing non published media
+* `STOP_PUBLISHING`: capability: publish, description: Stop publishing
+
+**Wake on lan**
+
+* `WAKE_ON_LAN_SEND`: capability: send_wake_on_lan, description: Send a wake on LAN network package from this system to wake another system
```

### Comparing `miris-manager-client-5.5/miris_manager_client.egg-info/PKG-INFO` & `miris-manager-client-6.0/miris_manager_client.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miris-manager-client
-Version: 5.5
+Version: 6.0
 Summary: A Python3 client to use Miris Manager remote control
 Home-page: https://www.ubicast.eu/en/solutions/delivery/
 Download-URL: https://github.com/UbiCastTeam/miris-manager-client
 Author: UbiCast
 Author-email: dev@ubicast.eu
 License: LGPLv3
 Keywords: api,client,miris,manager,ubicast
@@ -28,21 +28,21 @@
 A Python3 client to use UbiCast Miris Manager remote control API.
 
 This client is intended to act as a system in Miris Manager so it allows you to integrate a device in order to control it using Miris Manager.
 
 
 ## Requirements
 
-git
-python >= 3.9 (download the latest stable release from https://www.python.org/downloads/)
+* python >= 3.9 (download the latest stable release from https://www.python.org/downloads/)
+* python3-requests >= 2.30
 
 
 ## Important
 
-For production use, it is recommended to use the branch named "stable". The "master" branch is used for development.
+For production use, it is recommended to use the branch named "stable". The "main" branch is used for development.
 
 
 ## Client class instantiation
 
 The client class (`mm_client`.`client`.`MirisManagerClient`) takes two arguments:
 * `local_conf`: This argument can be either a dict or a path (`str` object). The default value is `None`, which means no configuration.
 * `setup_logging`: This argument must be a boolean. If set to `True`, the logging to console will be configured. The default value is `True`.
@@ -64,39 +64,63 @@
 * Replace the import path of `MirisManagerClient` (see example).
 * Replace the class variable `MirisManagerClient`.`LOCAL_CONF` with the class instance argument `MirisManagerClient`.`local_conf`.
 * Check the value of `MirisManagerClient`.`DEFAULT_CONF` because it is now `None` by default.
 * Replace all occurences of `URL` by `SERVER_URL` in all configuration.
 * Replace all occurences of `CHECK_SSL` by `VERIFY_SSL` in all configuration.
 
 
-## Example
+## Examples
 
 ### Ping the server
 
 ``` python
 from mm_client.client import MirisManagerClient
 mmc = MirisManagerClient(local_conf='your-conf.json')
 
 response = mmc.api_request('PING')
 print(response)
 ```
 
-There are more examples in the `examples` directory.
+
+### Recorder system
+
+This example is the use case of a recorder system that can be controlled through the long polling.
+
+[Link to the file](/examples/recorder_controller.py)
+
+
+### Wake on LAN requests
+
+This example is the use case of a client that forwards wake on LAN requests received through the long polling to its network.
+
+[Link to the file](/examples/wol_relay.py)
+
+
+### Other examples
+
+There are more examples in the [examples](/examples) directory.
 
 
 ## Actions
 
 Here is the list of actions that can be sent to the client depending on its supported capabilities:
 
-    # Basic actions
-    SHUTDOWN: capability: shutdown, description: Shutdown system
-    REBOOT: capability: reboot, description: Reboot system
-    UPGRADE: capability: upgrade, description: Upgrade system software
-    # Recording
-    START_RECORDING: capability: record, description: Start recording
-    STOP_RECORDING: capability: record, description: Stop recording
-    LIST_PROFILES: capability: record, description: Refresh profiles list
-    # Publishing
-    START_PUBLISHING: capability: publish, description: Start publishing non published media
-    STOP_PUBLISHING: capability: publish, description: Stop publishing
-    # Wake on lan
-    WAKE_ON_LAN_SEND: capability: send_wake_on_lan, description: Send a wake on LAN network package from this system to wake another system
+**Basic actions**
+
+* `SHUTDOWN`: capability: shutdown, description: Shutdown system
+* `REBOOT`: capability: reboot, description: Reboot system
+* `UPGRADE`: capability: upgrade, description: Upgrade system software
+
+**Recording**
+
+* `START_RECORDING`: capability: record, description: Start recording
+* `STOP_RECORDING`: capability: record, description: Stop recording
+* `LIST_PROFILES`: capability: record, description: Refresh profiles list
+
+**Publishing**
+
+* `START_PUBLISHING`: capability: publish, description: Start publishing non published media
+* `STOP_PUBLISHING`: capability: publish, description: Stop publishing
+
+**Wake on lan**
+
+* `WAKE_ON_LAN_SEND`: capability: send_wake_on_lan, description: Send a wake on LAN network package from this system to wake another system
```

### Comparing `miris-manager-client-5.5/mm_client/client.py` & `miris-manager-client-6.0/mm_client/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 '''
-Miris Manager client class
+Miris Manager client main module
 '''
 import logging
-import os
+from pathlib import Path
+
 import requests
+
 from .lib import configuration as configuration_lib
 from .lib import info as info_lib
 from .lib import long_polling as long_polling_lib
 from .lib import signing as signing_lib
 from .lib import ssh_tunnel as ssh_tunnel_lib
 
 logger = logging.getLogger('mm_client.client')
@@ -66,21 +68,22 @@
             self.conf_checked = True
 
     def get_url_info(self, url_or_action):
         if url_or_action.startswith('/'):
             return {'url': url_or_action}
         if url_or_action not in self.conf['API_CALLS']:
             raise MirisManagerRequestError(
-                'Invalid url requested: %s does not exist in API_CALLS configuration.' % url_or_action,
+                f'Invalid url requested: {url_or_action} does not exist in API_CALLS configuration.',
                 status_code=0,
                 error_code='invalid_url'
             )
         return self.conf['API_CALLS'][url_or_action]
 
-    def _request(self, url, method='get', headers=None, params=None, data=None, files=None, anonymous=None, timeout=None):
+    def _request(self, url, method='get', headers=None, params=None,
+                 data=None, files=None, anonymous=None, timeout=None):
         req = getattr(requests, method)(
             url=self.conf['SERVER_URL'] + url,
             headers=headers,
             params=params,
             data=data,
             files=files,
             proxies=self.conf.get('PROXIES'),
@@ -129,55 +132,75 @@
                 error_code='no_api_key'
             )
         self.update_conf('SECRET_KEY', secret_key)
         self.update_conf('API_KEY', api_key)
         logger.info('System registration done.')
         return True
 
-    def api_request(self, url_or_action, method='get', headers=None, params=None, data=None, files=None, anonymous=None, timeout=None):
+    def api_request(self, url_or_action, method='get', headers=None, params=None,
+                    data=None, files=None, anonymous=None, timeout=None):
         self.check_conf()
         url_info = self.get_url_info(url_or_action)
         if anonymous is None:
             anonymous = bool(url_info.get('anonymous'))
         if anonymous:
             _headers = headers
         else:
             # Register system if no API key and auto registration
             if not self.conf.get('API_KEY'):
                 if not self.conf['AUTO_REGISTRATION']:
-                    raise Exception('The client auto registration is disabled and no API_KEY is set in conf file, please set one or turn on auto registration.')
+                    raise ValueError('The client auto registration is disabled and no API_KEY is set in conf file, '
+                                     'please set one or turn on auto registration.')
                 try:
                     self._register()
                 except Exception as e:
                     logger.error('Registration failed: %s', e)
-                    raise Exception('Registration failed: %s' % e)
+                    raise
             # Add signature in headers
             # headers with "_" are ignored by Django
             _headers = {'api-key': self.conf['API_KEY']}
             if not anonymous:
-                signature = signing_lib.get_signature(self)
+                signature = signing_lib.get_signature(self.conf)
                 if signature:
                     _headers.update(signature)
             if headers:
                 _headers.update(headers)
         # Make API request
-        response = self._request(url_info['url'], method=url_info.get('method', method), headers=_headers, params=params, data=data, files=files, timeout=timeout)
+        response = self._request(
+            url_info['url'],
+            method=url_info.get('method', method),
+            headers=_headers,
+            params=params,
+            data=data,
+            files=files,
+            timeout=timeout
+        )
         return response
 
-    def long_polling_loop(self):
+    def long_polling_loop(self, single_loop=False):
         if not self._long_polling_manager:
             self._long_polling_manager = long_polling_lib.LongPollingManager(self)
-        self._long_polling_manager.loop()
+        self._long_polling_manager.loop(single_loop)
 
-    def handle_action(self, action, params):
-        # Function that should be implemented in your client to process the
-        # long polling responses.
-        # IMPORTANT: Any code written here should not be blocking more than 5s
-        # because of the delay after which the system is considered as offline
-        # in Miris Manager.
+    def handle_action(self, uid, action, params):
+        '''
+        Function that should be implemented in your client to process the long polling responses.
+        IMPORTANT: Any code written here should not be blocking more than 5s because of the
+                   delay after which the system is considered as offline in Miris Manager.
+        Arguments:
+        - uid: The system command unique identifier.
+        - action: The action to run.
+        - params: The action parameters.
+        Must return a tuple: (status, data)
+        - status: The system command status (string). Possible values:
+        - "DONE": The command has been executed successfully.
+        - "IN_PROGRESS": The command has been started but is not yet completed.
+        - "FAILED": The command execution has failed.
+        - data: The command result data (string). It can be a json dump or a message. Empty strings are allowed.
+        '''
         raise NotImplementedError('Your class should override the "handle_action" method.')
 
     def set_command_status(self, command_uid, status='DONE', data=None):
         if not command_uid:
             return
         try:
             self.api_request('SET_COMMAND_STATUS', data=dict(
@@ -199,15 +222,16 @@
         data = {
             'capabilities': ' '.join(self.conf['CAPABILITIES']),
         }
         # Make API request
         response = self.api_request('SET_INFO', data=data)
         return response
 
-    def set_status(self, status=None, status_info=None, status_message=None, profile=None, remaining_space=None, remaining_time=None):
+    def set_status(self, status=None, status_info=None, status_message=None,
+                   profile=None, remaining_space=None, remaining_time=None):
         data = {}
         if status is not None:
             data['status'] = status
         if status_info is not None:
             data['status_info'] = status_info
         if status_message is not None or status is not None:
             data['status_message'] = status_message or ''
@@ -223,15 +247,15 @@
             raise ValueError('No data to update.')
         response = self.api_request('SET_STATUS', data=data)
         return response
 
     def set_screenshot(self, path, file_name=None):
         with open(path, 'rb') as file_obj:
             response = self.api_request('SET_SCREENSHOT', files=dict(
-                screenshot=(file_name or os.path.basename(path), file_obj)
+                screenshot=(file_name or Path(path).name, file_obj)
             ))
         return response
 
     def open_tunnel(self, status_callback=None):
         if not self._ssh_tunnel_manager:
             self._ssh_tunnel_manager = ssh_tunnel_lib.SSHTunnelManager(self, status_callback)
         self._ssh_tunnel_manager.tunnel_loop()
```

### Comparing `miris-manager-client-5.5/mm_client/conf.py` & `miris-manager-client-6.0/mm_client/conf.py`

 * *Files identical despite different names*

### Comparing `miris-manager-client-5.5/mm_client/lib/configuration.py` & `miris-manager-client-6.0/mm_client/lib/configuration.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,68 +1,75 @@
 '''
 Miris Manager client library
 This module is not intended to be used directly, only the client class should be used.
 '''
 import json
 import logging
-import os
 import re
+from pathlib import Path
+
 from ..conf import BASE_CONF
 
 logger = logging.getLogger('mm_client.lib.configuration')
 
 
 def load_conf(default_conf=None, local_conf=None):
     # copy default configuration
     conf = BASE_CONF.copy()
     # update with default and local configuration
     for index, conf_override in enumerate((default_conf, local_conf)):
         if not conf_override:
             continue
+        if isinstance(conf_override, str):
+            conf_override = Path(conf_override)
         if isinstance(conf_override, dict):
             for key, val in conf_override.items():
                 if not key.startswith('_'):
                     conf[key] = val
-        elif isinstance(conf_override, str):
-            if os.path.exists(conf_override):
-                with open(conf_override, 'r') as fo:
-                    content = fo.read()
+        elif isinstance(conf_override, Path):
+            if conf_override.exists():
+                content = conf_override.read_text()
                 content = re.sub(r'\n\s*//.*', '\n', content)  # remove comments
                 conf_mod = json.loads(content) if content else None
                 if not conf_mod:
                     logger.debug('Config file "%s" is empty.', conf_override)
                 else:
                     logger.debug('Config file "%s" loaded.', conf_override)
                     if not isinstance(conf_mod, dict):
-                        raise ValueError('The configuration in "%s" is not a dict.' % conf_override)
+                        raise ValueError(f'The configuration in "{conf_override}" is not a dict.')
                     conf.update(conf_mod)
             else:
                 logger.debug('Config file does not exists, using default config.')
         else:
             raise ValueError('Unsupported type for configuration.')
     if conf['SERVER_URL'].endswith('/'):
         conf['SERVER_URL'] = conf['SERVER_URL'].rstrip('/')
     return conf
 
 
 def update_conf(local_conf, key, value):
-    if not local_conf or not isinstance(local_conf, str):
+    if not local_conf:
+        logger.debug('Cannot update configuration, "local_conf" is not set.')
+        return False
+    if isinstance(local_conf, str):
+        local_conf = Path(local_conf)
+    elif not isinstance(local_conf, Path):
         logger.debug('Cannot update configuration, "local_conf" is not a path.')
-        return
-    content = ''
-    if os.path.isfile(local_conf):
-        with open(local_conf, 'r') as fo:
-            content = fo.read()
-        content = content.strip()
-    data = json.loads(content) if content else dict()
+        return False
+
+    if local_conf.is_file():
+        content = local_conf.read_text().strip()
+    else:
+        content = ''
+    data = json.loads(content) if content else {}
     data[key] = value
     new_content = json.dumps(data, sort_keys=True, indent=4)
-    with open(local_conf, 'w') as fo:
-        fo.write(new_content)
+    local_conf.write_text(new_content)
     logger.debug('Configuration file "%s" updated: "%s" set to "%s".', local_conf, key, value)
+    return True
 
 
 def check_conf(conf):
     # check that mandatory configuration values are set
     if not conf.get('SERVER_URL') or conf['SERVER_URL'] == 'https://mirismanager':
         raise ValueError('The value of "SERVER_URL" is not set. Please configure it.')
     conf['SERVER_URL'] = conf['SERVER_URL'].strip('/')
```

### Comparing `miris-manager-client-5.5/mm_client/lib/info.py` & `miris-manager-client-6.0/mm_client/lib/info.py`

 * *Files identical despite different names*

### Comparing `miris-manager-client-5.5/mm_client/lib/long_polling.py` & `miris-manager-client-6.0/mm_client/lib/long_polling.py`

 * *Files 26% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
     def __init__(self, client):
         self.client = client
         self.run_systemd_notify = False
         self.last_error = None
         self.loop_running = False
 
-    def loop(self):
+    def loop(self, single_loop=False):
         # Check if systemd-notify should be called
         self.run_systemd_notify = self.client.conf.get('WATCHDOG') and os.system('which systemd-notify') == 0
         # Start connection loop
         logger.info('Starting long polling to %s' % self.client.conf['SERVER_URL'])
         self.loop_running = True
 
         def exit_handler(*args, **kwargs):
@@ -37,14 +37,16 @@
 
         signal.signal(signal.SIGINT, exit_handler)
         signal.signal(signal.SIGTERM, exit_handler)
 
         while self.loop_running:
             start = datetime.datetime.utcnow()
             success = self.call_long_polling()
+            if single_loop:
+                break
             if not success:
                 # Avoid starting too often new connections
                 duration = (datetime.datetime.utcnow() - start).seconds
                 if duration < 5:
                     time.sleep(5 - duration)
 
     def call_long_polling(self):
@@ -63,38 +65,45 @@
         else:
             self.last_error = None
             if response:
                 logger.info('Received long polling response: %s', response)
                 success = True
                 uid = response.get('uid')
                 try:
-                    result = self.process_long_polling(response)
+                    status, data = self.process_long_polling(response)
                 except Exception as e:
                     success = False
                     logger.error('Failed to process response: %s\n%s', e, traceback.format_exc())
                     self.client.set_command_status(uid, 'FAILED', str(e))
                     if os.environ.get('CI_PIPELINE_ID'):
-                        # propagate exception so that it can be detected in CI
-                        raise Exception(e)
+                        # Propagate exception so that it can be detected in CI
+                        raise
                 else:
-                    self.client.set_command_status(uid, 'DONE', result)
+                    self.client.set_command_status(uid, status, data)
         finally:
             if self.run_systemd_notify:
                 logger.debug('Notifying systemd watchdog.')
                 os.system('systemd-notify WATCHDOG=1')
         return success
 
     def process_long_polling(self, response):
         logger.debug('Processing response.')
         if self.client.conf.get('API_KEY'):
-            invalid = check_signature(self.client, response)
+            invalid = check_signature(self.client.conf, response)
             if invalid:
-                raise Exception('Invalid signature: %s' % invalid)
+                raise ValueError('Invalid signature: %s' % invalid)
+        uid = response.get('uid')
         action = response.get('action')
         if not action:
-            raise Exception('No action received.')
-        params = response.get('params', dict())
-        logger.debug('Received command "%s": %s.', response.get('uid'), action)
+            raise ValueError('No action received.')
+        params = response.get('params', {})
+        logger.debug('Received command "%s": %s.', uid, action)
         if action == 'PING':
-            pass
-        else:
-            return self.client.handle_action(action, params)
+            return 'DONE', ''
+        status, data = self.client.handle_action(uid=uid, action=action, params=params)
+        if status not in ('DONE', 'IN_PROGRESS', 'FAILED'):
+            logger.error('Your client has returned an invalid status in "handle_action".')
+            raise ValueError('An error occurred during the processing of the action by the client.')
+        if data is not None and not isinstance(data, str):
+            logger.error('Your client has returned an invalid type for data in "handle_action".')
+            raise ValueError('An error occurred during the processing of the action by the client.')
+        return status, data
```

### Comparing `miris-manager-client-5.5/mm_client/lib/signing.py` & `miris-manager-client-6.0/mm_client/lib/signing.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,30 +7,30 @@
 import hashlib
 import hmac
 import logging
 
 logger = logging.getLogger('mm_client.lib.signing')
 
 
-def get_signature(client):
-    if not client.conf.get('SECRET_KEY') or not client.conf.get('API_KEY'):
-        return dict()
+def get_signature(conf):
+    if not conf.get('SECRET_KEY') or not conf.get('API_KEY'):
+        return {}
     utime = datetime.datetime.utcnow().strftime('%Y-%m-%d_%H-%M-%S_%f')
-    to_sign = 'time=%s|api_key=%s' % (utime, client.conf['API_KEY'])
+    to_sign = 'time=%s|api_key=%s' % (utime, conf['API_KEY'])
     hm = hmac.new(
-        client.conf['SECRET_KEY'].encode('utf-8'),
+        conf['SECRET_KEY'].encode('utf-8'),
         msg=to_sign.encode('utf-8'),
         digestmod=hashlib.sha256
     ).digest()
     hm = base64.b64encode(hm).decode('utf-8')
     return {'time': utime, 'hmac': hm}
 
 
-def check_signature(client, rdata):
-    if not client.conf.get('SECRET_KEY') or not client.conf.get('API_KEY'):
+def check_signature(conf, rdata):
+    if not conf.get('SECRET_KEY') or not conf.get('API_KEY'):
         return None
     remote_time = rdata.get('time')
     remote_hmac = rdata.get('hmac')
     if not remote_time or not remote_hmac:
         return 'some mandatory data are missing.'
     try:
         rdate = datetime.datetime.strptime(remote_time, '%Y-%m-%d_%H-%M-%S_%f')
@@ -40,16 +40,16 @@
         rhmac = base64.b64decode(remote_hmac)
     except Exception:
         return 'the received hmac is invalid.'
     utcnow = datetime.datetime.utcnow()
     diff = utcnow - rdate if utcnow > rdate else rdate - utcnow
     if diff.seconds > 300:
         return 'the difference between the request time and the current time is too large.'
-    to_sign = 'time=%s|api_key=%s' % (remote_time, client.conf['API_KEY'])
+    to_sign = 'time=%s|api_key=%s' % (remote_time, conf['API_KEY'])
     hm = hmac.new(
-        client.conf['SECRET_KEY'].encode('utf-8'),
+        conf['SECRET_KEY'].encode('utf-8'),
         msg=to_sign.encode('utf-8'),
         digestmod=hashlib.sha256
     ).digest()
     if rhmac != hm:
         return 'the received and computed HMAC values do not match.'
     return None
```

### Comparing `miris-manager-client-5.5/mm_client/lib/ssh_tunnel.py` & `miris-manager-client-6.0/mm_client/lib/ssh_tunnel.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,51 +1,67 @@
 '''
 Miris Manager SSH tunnel management
 This module is not intended to be used directly, only the client class should be used.
-The SSH tunnel goal is to access the system web interface (HTTPS) from Miris Manager using a connection from the system to the Miris Manager.
+
+The SSH tunnel goal is to access the system web interface (HTTPS) from
+Miris Manager using a connection from the system to the Miris Manager.
 '''
 import logging
 import os
 import subprocess
 import time
 import multiprocessing
 import re
 import signal
+from pathlib import Path
 
 logger = logging.getLogger('mm_client.lib.ssh_tunnel')
 
 
+class MirisManagerTunnelError(Exception):
+    pass
+
+
 def get_ssh_public_key():
-    ssh_key_path = os.path.join(os.path.expanduser('~/.ssh/miris-manager-client-key'))
-    ssh_dir = os.path.dirname(ssh_key_path)
-    if not os.path.exists(ssh_dir):
-        os.makedirs(ssh_dir)
-        os.chmod(ssh_dir, 0o700)
-    if os.path.exists(ssh_key_path):
-        if not os.path.exists(ssh_key_path + '.pub'):
-            raise Exception('Weird state detetected: "%s" exists but not "%s" !' % (ssh_key_path, ssh_key_path + '.pub'))
+    ssh_dir = Path('~/.ssh').expanduser()
+    ssh_key_path = ssh_dir / 'miris-manager-client-key'
+    ssh_pub_path = ssh_dir / 'miris-manager-client-key.pub'
+    if not ssh_dir.exists():
+        ssh_dir.mkdir(parents=True)
+        ssh_dir.chmod(0o700)
+    if ssh_key_path.exists():
+        if not ssh_pub_path.exists():
+            raise MirisManagerTunnelError(
+                f'Weird state detetected: "{ssh_key_path}" exists but not "{ssh_pub_path}" !'
+            )
         logger.debug('Using existing SSH key: "%s".', ssh_key_path)
     else:
         logger.info('Creating new SSH key: "%s".', ssh_key_path)
-        p = subprocess.Popen(['ssh-keygen', '-b', '4096', '-f', ssh_key_path, '-N', ''], stdin=subprocess.PIPE, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
+        p = subprocess.Popen(
+            ['ssh-keygen', '-b', '4096', '-f', str(ssh_key_path), '-N', ''],
+            stdin=subprocess.PIPE,
+            stdout=subprocess.PIPE,
+            stderr=subprocess.STDOUT
+        )
         p.communicate(input=b'\n\n\n')
         if p.returncode != 0:
-            out = p.stdout.decode('utf-8') + '\n' + p.stderr.decode('utf-8')
-            raise Exception('Failed to generate SSH key:\n%s' % out)
-        os.chmod(ssh_key_path, 0o600)
-        os.chmod(ssh_key_path + '.pub', 0o600)
-    with open(ssh_key_path + '.pub', 'r') as fo:
-        public_key = fo.read()
+            out = p.stdout.decode('utf-8').strip()
+            raise MirisManagerTunnelError(
+                f'Failed to generate SSH key:\n{out}'
+            )
+        ssh_key_path.chmod(0o600)
+        ssh_pub_path.chmod(0o600)
+    public_key = ssh_pub_path.read_text()
     return public_key
 
 
 def prepare_ssh_command(host, info):
-    ssh_key_path = os.path.join(os.path.expanduser('~/.ssh/miris-manager-client-key'))
+    ssh_key_path = Path('~/.ssh/miris-manager-client-key').expanduser()
     command = ['ssh',
-               '-i', ssh_key_path,
+               '-i', str(ssh_key_path),
                '-nvNT',
                '-o', 'IdentitiesOnly=yes',
                '-o', 'NumberOfPasswordPrompts=0',
                '-o', 'CheckHostIP=no',
                '-o', 'StrictHostKeyChecking=no',
                '-o', 'ServerAliveInterval=10',
                '-R', '%s:127.0.0.1:443' % info['control_port'],
@@ -57,25 +73,47 @@
 
 class SSHTunnelManager():
 
     def __init__(self, client, status_callback=None):
         self.client = client
         self.status_callback = status_callback
         self.pattern_list = [
-            dict(id='connecting', pattern=re.compile(r'debug1: Connecting to (?P<hostname>[^ ]+) \[(?P<ip>[0-9\.]{7,15})\] port (?P<port>\d{1,5}).\r\n')),
-            dict(id='connected', pattern=re.compile(r'debug1: Connection established.\r\n')),
-            dict(id='authenticated', pattern=re.compile(r'debug1: Authentication succeeded \((?P<method>[^\)]+)\).\r\n')),
-            dict(id='authenticated', pattern=re.compile(r'Authenticated to (?P<hostname>[^ ]+) \(\[(?P<ip>[0-9\.]{7,15})\]:(?P<port>\d{1,5})\).\r\n')),
-            dict(id='running', pattern=re.compile(r'debug1: Entering interactive session.\r\n')),
-            dict(id='not_known', pattern=re.compile(r'ssh: [^:]+: Name or service not known\r\n')),
-            dict(id='port_refused', pattern=re.compile(r'Warning: remote port forwarding failed for listen port (?P<port>\d{1,5})')),
-            dict(id='refused', pattern=re.compile(r'ssh: connect to host [^:]+: Connection refused\r\n')),
-            dict(id='control_refused', pattern=re.compile(r'connect_to (?P<hostname>[^ ]+) port (?P<port>\d{1,5}): failed\.\r\n')),
-            dict(id='denied', pattern=re.compile(r'Permission denied \(publickey,password\).\r\n')),
-            dict(id='closed', pattern=re.compile(r'Connection to (?P<hostname>[^ ]+) closed.\r\n')),
+            dict(id='connecting', pattern=re.compile(
+                r'debug1: Connecting to (?P<hostname>[^ ]+) \[(?P<ip>[0-9\.]{7,15})\] port (?P<port>\d{1,5}).\r\n'
+            )),
+            dict(id='connected', pattern=re.compile(
+                r'debug1: Connection established.\r\n'
+            )),
+            dict(id='authenticated', pattern=re.compile(
+                r'debug1: Authentication succeeded \((?P<method>[^\)]+)\).\r\n'
+            )),
+            dict(id='authenticated', pattern=re.compile(
+                r'Authenticated to (?P<hostname>[^ ]+) \(\[(?P<ip>[0-9\.]{7,15})\]:(?P<port>\d{1,5})\).\r\n'
+            )),
+            dict(id='running', pattern=re.compile(
+                r'debug1: Entering interactive session.\r\n'
+            )),
+            dict(id='not_known', pattern=re.compile(
+                r'ssh: [^:]+: Name or service not known\r\n'
+            )),
+            dict(id='port_refused', pattern=re.compile(
+                r'Warning: remote port forwarding failed for listen port (?P<port>\d{1,5})'
+            )),
+            dict(id='refused', pattern=re.compile(
+                r'ssh: connect to host [^:]+: Connection refused\r\n'
+            )),
+            dict(id='control_refused', pattern=re.compile(
+                r'connect_to (?P<hostname>[^ ]+) port (?P<port>\d{1,5}): failed\.\r\n'
+            )),
+            dict(id='denied', pattern=re.compile(
+                r'Permission denied \(publickey,password\).\r\n'
+            )),
+            dict(id='closed', pattern=re.compile(
+                r'Connection to (?P<hostname>[^ ]+) closed.\r\n'
+            )),
         ]
         self.loop_ssh_tunnel = False
         self.process = None
         self.stdout_queue = None
         self.stdout_reader = None
         self.stderr_reader = None
         self.ssh_tunnel_state = {
@@ -87,28 +125,28 @@
             'command': '',
             'last_tunnel_info': ''
         }
 
     def establish_tunnel(self):
         public_key = None
         response = None
-        logger.debug('Establishing new tunnel to %s' % self.client.conf['SERVER_URL'])
+        logger.debug('Establishing new tunnel to %s', self.client.conf['SERVER_URL'])
         self._stop_reader()
         self._try_closing_process()
         self.update_ssh_state('state', 'prepare tunnel')
         try:
             logger.debug('Prepare tunnel')
             public_key = get_ssh_public_key()
             response = self.client.api_request('PREPARE_TUNNEL', data=dict(public_key=public_key))
         except Exception as e:
             self.update_ssh_state('state', 'prepare tunnel failed')
             self.update_ssh_state('control_port', 0)
             self.update_ssh_state('maintenance_port', 0)
             self.update_ssh_state('command', ['PREPARE_TUNNEL', self.client.conf['SERVER_URL']])
-            logger.error('Cannot prepare ssh tunnel : %s' % str(e))
+            logger.error('Cannot prepare ssh tunnel : %s', str(e))
             return
         ssh_user = response.get('ssh_user')
         if ssh_user and ssh_user != self.ssh_tunnel_state['ssh_user']:
             self.update_ssh_state('ssh_user', response['ssh_user'])
         ssh_port = response.get('ssh_port')
         if ssh_port and ssh_port != self.ssh_tunnel_state['ssh_port']:
             self.update_ssh_state('ssh_port', response['ssh_port'])
@@ -120,31 +158,36 @@
             self.update_ssh_state('control_port', port)
             host = self.client.conf['SERVER_URL'].split('://', 1)[-1]
             host = host.rsplit(':', 1)[0].rstrip('/')
             cmd = prepare_ssh_command(host, self.ssh_tunnel_state)
             self.update_ssh_state('command', cmd)
             logger.info('Starting SSH with command:\n    %s', ' '.join(cmd))
             if self.loop_ssh_tunnel:
-                self.process = subprocess.Popen(cmd, stdout=subprocess.PIPE, stderr=subprocess.PIPE, preexec_fn=os.setsid)
+                self.process = subprocess.Popen(
+                    cmd,
+                    stdout=subprocess.PIPE,
+                    stderr=subprocess.PIPE,
+                    preexec_fn=os.setsid
+                )
                 self.stdout_queue = multiprocessing.Queue()
                 self.stdout_reader = AsynchronousFileReader(self.process.stdout, self.stdout_queue)
                 self.stdout_reader.start()
                 self.stderr_reader = AsynchronousFileReader(self.process.stderr, self.stdout_queue)
                 self.stderr_reader.start()
                 return True
         else:
             logger.debug('No control port provided, not starting ssh tunnel')
 
     def update_ssh_state(self, key, value):
         if key == 'state' and self.ssh_tunnel_state.get('state') != value:
-            logger.info('SSH state changed to %s' % value)
+            logger.info('SSH state changed to %s', value)
         if self.ssh_tunnel_state.get(key) is not None:
             self.ssh_tunnel_state[key] = value
         else:
-            logger.warning('Key %s not exists in ssh state dict' % key)
+            logger.warning('Key %s not exists in ssh state dict', key)
         if self.status_callback:
             self.status_callback(self.ssh_tunnel_state)
 
     def close_tunnel(self, thread_event=None):
         logger.debug('Close ssh tunnel asked')
         self.loop_ssh_tunnel = False
         if thread_event:
@@ -236,15 +279,15 @@
             try:
                 while not self.stdout_queue.empty():
                     ssh_logs += self.stdout_queue.get_nowait()
             except OSError as e:
                 ssh_logs = str(e)
             self.update_ssh_state('state', 'error')
             self.update_ssh_state('last_tunnel_info', ssh_logs)
-            logger.error('SSH tunnel process has terminated with: %s' % ssh_logs)
+            logger.error('SSH tunnel process has terminated with: %s', ssh_logs)
             need_retry = True
         else:
             # process is still alive
             try:
                 while not self.stdout_queue.empty():
                     ssh_stdout = self.stdout_queue.get_nowait()
                     pattern_id_found = None
@@ -252,19 +295,29 @@
                         if pattern_dict['pattern'].match(ssh_stdout):
                             pattern_id_found = pattern_dict['id']
                             self.update_ssh_state('state', pattern_id_found)
                             self.update_ssh_state('last_tunnel_info', ssh_stdout)
                             break
                     if not pattern_id_found:
                         if ssh_stdout.startswith('debug1:') or ssh_stdout.startswith('OpenSSH_'):
-                            logger.debug('[SSH stdout] %s' % ssh_stdout)
+                            logger.debug('[SSH stdout] %s', ssh_stdout)
                         else:
-                            logger.warning('[SSH stdout] %s' % ssh_stdout)
+                            logger.warning('[SSH stdout] %s', ssh_stdout)
                     elif pattern_id_found not in ['connecting', 'connected', 'authenticated', 'running']:
-                        logger.error('Need to retry tunnel (ssh port: {ssh_port}, remote control port: {control_port}, remote maintenance port: {maintenance_port}) because ssh command failed in stdout %s'.format(**self.ssh_tunnel_state) % pattern_id_found)
+                        logger.error(
+                            (
+                                'Need to retry tunnel '
+                                '(ssh port: %s, remote control port: %s, remote maintenance port: %s) '
+                                'because ssh command failed in stdout %s'
+                            ),
+                            self.ssh_tunnel_state.get('ssh_port'),
+                            self.ssh_tunnel_state.get('control_port'),
+                            self.ssh_tunnel_state.get('maintenance_port'),
+                            pattern_id_found
+                        )
                         need_retry = True
                         break
             except OSError as e:
                 logger.error(e)
                 need_retry = True
         return need_retry
```

### Comparing `miris-manager-client-5.5/setup.cfg` & `miris-manager-client-6.0/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -25,25 +25,28 @@
 	Programming Language :: Python :: 3.11
 	Topic :: Multimedia :: Video
 	Topic :: Software Development :: Libraries :: Python Modules
 
 [options]
 include_package_data = True
 install_requires = 
-	requests >= 2.28
+	requests >= 2.30
 packages = 
 	mm_client
 	mm_client.lib
 setup_requires = 
 	setuptools >= 30.3.0
 	wheel
 
 [options.extras_require]
 dev = 
 	flake8
+	pytest
+	pytest-cov
+	vulture
 
 [bdist_wheel]
 universal = 1
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

