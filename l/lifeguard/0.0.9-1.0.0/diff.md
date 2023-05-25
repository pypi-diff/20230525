# Comparing `tmp/lifeguard-0.0.9.tar.gz` & `tmp/lifeguard-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lifeguard-0.0.9.tar", last modified: Fri Jan 15 19:17:59 2021, max compression
+gzip compressed data, was "lifeguard-1.0.0.tar", last modified: Thu May 25 14:33:25 2023, max compression
```

## Comparing `lifeguard-0.0.9.tar` & `lifeguard-1.0.0.tar`

### file list

```diff
@@ -1,47 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-15 19:17:59.591395 lifeguard-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (116)      363 2021-01-15 19:17:59.591395 lifeguard-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      404 2021-01-15 19:17:49.000000 lifeguard-0.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-15 19:17:59.587395 lifeguard-0.0.9/bin/
--rwxr-xr-x   0 runner    (1001) docker     (116)     1190 2021-01-15 19:17:49.000000 lifeguard-0.0.9/bin/lifeguard
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-15 19:17:59.591395 lifeguard-0.0.9/lifeguard/
--rw-r--r--   0 runner    (1001) docker     (116)     1312 2021-01-15 19:17:49.000000 lifeguard-0.0.9/lifeguard/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-15 19:17:59.591395 lifeguard-0.0.9/lifeguard/actions/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-01-15 19:17:49.000000 lifeguard-0.0.9/lifeguard/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      457 2021-01-15 19:17:49.000000 lifeguard-0.0.9/lifeguard/actions/database.py
--rw-r--r--   0 runner    (1001) docker     (116)     2994 2021-01-15 19:17:49.000000 lifeguard-0.0.9/lifeguard/actions/notifications.py
--rw-r--r--   0 runner    (1001) docker     (116)     1466 2021-01-15 19:17:49.000000 lifeguard-0.0.9/lifeguard/controllers.py
--rw-r--r--   0 runner    (1001) docker     (116)      778 2021-01-15 19:17:49.000000 lifeguard-0.0.9/lifeguard/http_client.py
--rw-r--r--   0 runner    (1001) docker     (116)     1662 2021-01-15 19:17:49.000000 lifeguard-0.0.9/lifeguard/logger.py
--rw-r--r--   0 runner    (1001) docker     (116)     3584 2021-01-15 19:17:49.000000 lifeguard-0.0.9/lifeguard/notifications.py
--rw-r--r--   0 runner    (1001) docker     (116)     1600 2021-01-15 19:17:49.000000 lifeguard-0.0.9/lifeguard/repositories.py
--rw-r--r--   0 runner    (1001) docker     (116)      854 2021-01-15 19:17:49.000000 lifeguard-0.0.9/lifeguard/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (116)     1377 2021-01-15 19:17:49.000000 lifeguard-0.0.9/lifeguard/server.py
--rw-r--r--   0 runner    (1001) docker     (116)     1596 2021-01-15 19:17:49.000000 lifeguard-0.0.9/lifeguard/settings.py
--rw-r--r--   0 runner    (1001) docker     (116)     3927 2021-01-15 19:17:49.000000 lifeguard-0.0.9/lifeguard/validations.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-15 19:17:59.591395 lifeguard-0.0.9/lifeguard.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)      363 2021-01-15 19:17:59.000000 lifeguard-0.0.9/lifeguard.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      985 2021-01-15 19:17:59.000000 lifeguard-0.0.9/lifeguard.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-01-15 19:17:59.000000 lifeguard-0.0.9/lifeguard.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       33 2021-01-15 19:17:59.000000 lifeguard-0.0.9/lifeguard.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       16 2021-01-15 19:17:59.000000 lifeguard-0.0.9/lifeguard.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)      125 2021-01-15 19:17:59.595395 lifeguard-0.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)      565 2021-01-15 19:17:49.000000 lifeguard-0.0.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-15 19:17:59.591395 lifeguard-0.0.9/tests/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-01-15 19:17:49.000000 lifeguard-0.0.9/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-15 19:17:59.591395 lifeguard-0.0.9/tests/actions/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-01-15 19:17:49.000000 lifeguard-0.0.9/tests/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      661 2021-01-15 19:17:49.000000 lifeguard-0.0.9/tests/actions/test_database.py
--rw-r--r--   0 runner    (1001) docker     (116)     6465 2021-01-15 19:17:49.000000 lifeguard-0.0.9/tests/actions/test_notification.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-15 19:17:59.591395 lifeguard-0.0.9/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-01-15 19:17:49.000000 lifeguard-0.0.9/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)       41 2021-01-15 19:17:49.000000 lifeguard-0.0.9/tests/fixtures/fixtures_repositories.py
--rw-r--r--   0 runner    (1001) docker     (116)      138 2021-01-15 19:17:49.000000 lifeguard-0.0.9/tests/fixtures/mock_lifeguard_settings.py
--rw-r--r--   0 runner    (1001) docker     (116)      764 2021-01-15 19:17:49.000000 lifeguard-0.0.9/tests/test_controllers.py
--rw-r--r--   0 runner    (1001) docker     (116)     1107 2021-01-15 19:17:49.000000 lifeguard-0.0.9/tests/test_http_client.py
--rw-r--r--   0 runner    (1001) docker     (116)     1050 2021-01-15 19:17:49.000000 lifeguard-0.0.9/tests/test_lifeguard_core.py
--rw-r--r--   0 runner    (1001) docker     (116)     1307 2021-01-15 19:17:49.000000 lifeguard-0.0.9/tests/test_notifications.py
--rw-r--r--   0 runner    (1001) docker     (116)     3873 2021-01-15 19:17:49.000000 lifeguard-0.0.9/tests/test_repositories.py
--rw-r--r--   0 runner    (1001) docker     (116)      526 2021-01-15 19:17:49.000000 lifeguard-0.0.9/tests/test_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (116)     2283 2021-01-15 19:17:49.000000 lifeguard-0.0.9/tests/test_server.py
--rw-r--r--   0 runner    (1001) docker     (116)      947 2021-01-15 19:17:49.000000 lifeguard-0.0.9/tests/test_settings.py
--rw-r--r--   0 runner    (1001) docker     (116)     2770 2021-01-15 19:17:49.000000 lifeguard-0.0.9/tests/test_validations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:33:25.948863 lifeguard-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-25 14:33:25.948863 lifeguard-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4566 2023-05-25 14:33:10.000000 lifeguard-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:33:25.940863 lifeguard-1.0.0/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2399 2023-05-25 14:33:10.000000 lifeguard-1.0.0/bin/lifeguard
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:33:25.940863 lifeguard-1.0.0/lifeguard/
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-05-25 14:33:10.000000 lifeguard-1.0.0/lifeguard/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:33:25.944863 lifeguard-1.0.0/lifeguard/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:33:10.000000 lifeguard-1.0.0/lifeguard/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-25 14:33:10.000000 lifeguard-1.0.0/lifeguard/actions/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-05-25 14:33:10.000000 lifeguard-1.0.0/lifeguard/actions/email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6248 2023-05-25 14:33:10.000000 lifeguard-1.0.0/lifeguard/actions/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-05-25 14:33:10.000000 lifeguard-1.0.0/lifeguard/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-05-25 14:33:10.000000 lifeguard-1.0.0/lifeguard/bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-05-25 14:33:10.000000 lifeguard-1.0.0/lifeguard/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:33:25.944863 lifeguard-1.0.0/lifeguard/controllers/
+-rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-05-25 14:33:10.000000 lifeguard-1.0.0/lifeguard/controllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-05-25 14:33:10.000000 lifeguard-1.0.0/lifeguard/controllers/assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-25 14:33:10.000000 lifeguard-1.0.0/lifeguard/http_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-05-25 14:33:10.000000 lifeguard-1.0.0/lifeguard/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4551 2023-05-25 14:33:10.000000 lifeguard-1.0.0/lifeguard/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-05-25 14:33:10.000000 lifeguard-1.0.0/lifeguard/repositories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-05-25 14:33:10.000000 lifeguard-1.0.0/lifeguard/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-05-25 14:33:10.000000 lifeguard-1.0.0/lifeguard/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6810 2023-05-25 14:33:10.000000 lifeguard-1.0.0/lifeguard/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-25 14:33:10.000000 lifeguard-1.0.0/lifeguard/statuses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-25 14:33:10.000000 lifeguard-1.0.0/lifeguard/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5817 2023-05-25 14:33:10.000000 lifeguard-1.0.0/lifeguard/validations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:33:25.944863 lifeguard-1.0.0/lifeguard.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-25 14:33:25.000000 lifeguard-1.0.0/lifeguard.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-05-25 14:33:25.000000 lifeguard-1.0.0/lifeguard.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 14:33:25.000000 lifeguard-1.0.0/lifeguard.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-25 14:33:25.000000 lifeguard-1.0.0/lifeguard.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-25 14:33:25.000000 lifeguard-1.0.0/lifeguard.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-25 14:33:25.948863 lifeguard-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-25 14:33:10.000000 lifeguard-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:33:25.944863 lifeguard-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:33:10.000000 lifeguard-1.0.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:33:25.948863 lifeguard-1.0.0/tests/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:33:10.000000 lifeguard-1.0.0/tests/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-25 14:33:10.000000 lifeguard-1.0.0/tests/actions/test_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5295 2023-05-25 14:33:10.000000 lifeguard-1.0.0/tests/actions/test_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15144 2023-05-25 14:33:10.000000 lifeguard-1.0.0/tests/actions/test_notification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:33:25.948863 lifeguard-1.0.0/tests/controllers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:33:10.000000 lifeguard-1.0.0/tests/controllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-05-25 14:33:10.000000 lifeguard-1.0.0/tests/controllers/test_assets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:33:25.948863 lifeguard-1.0.0/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:33:10.000000 lifeguard-1.0.0/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-25 14:33:10.000000 lifeguard-1.0.0/tests/fixtures/fixtures_repositories.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-25 14:33:10.000000 lifeguard-1.0.0/tests/fixtures/mock_lifeguard_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-05-25 14:33:10.000000 lifeguard-1.0.0/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-25 14:33:10.000000 lifeguard-1.0.0/tests/test_bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11566 2023-05-25 14:33:10.000000 lifeguard-1.0.0/tests/test_controllers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-05-25 14:33:10.000000 lifeguard-1.0.0/tests/test_http_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-05-25 14:33:10.000000 lifeguard-1.0.0/tests/test_lifeguard_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-05-25 14:33:10.000000 lifeguard-1.0.0/tests/test_notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5781 2023-05-25 14:33:10.000000 lifeguard-1.0.0/tests/test_repositories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-05-25 14:33:10.000000 lifeguard-1.0.0/tests/test_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-05-25 14:33:10.000000 lifeguard-1.0.0/tests/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7064 2023-05-25 14:33:10.000000 lifeguard-1.0.0/tests/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6932 2023-05-25 14:33:10.000000 lifeguard-1.0.0/tests/test_validations.py
```

### Comparing `lifeguard-0.0.9/bin/lifeguard` & `lifeguard-1.0.0/bin/lifeguard`

 * *Files 23% similar despite different names*

```diff
@@ -1,33 +1,47 @@
 #!/usr/bin/env python3
-
+import argparse
 import _thread
 import sys
 import multiprocessing
 import gunicorn.app.base
+from tabulate import tabulate
 
 sys.path.append(".")
 
 from lifeguard import setup
+from lifeguard.bootstrap import generate_base_project
+from lifeguard.context import LIFEGUARD_CONTEXT
 from lifeguard.scheduler import start_scheduler
-from lifeguard.settings import LIFEGUARD_SERVER_PORT
+from lifeguard.settings import LIFEGUARD_SERVER_PORT, SETTINGS_MANAGER, SettingsManager
 
-setup()
 
-# Scheduler
-_thread.start_new_thread(start_scheduler, ())
+def display_settings():
+    data = {"Name": [], "Description": [], "Value": []}
 
-# Server
-from lifeguard.server import APP
+    settings_manager = SettingsManager(SETTINGS_MANAGER.settings)
+
+    for entry in settings_manager.settings:
+        data["Name"].append(entry)
+        data["Description"].append(settings_manager.settings[entry]["description"])
+        data["Value"].append(settings_manager.read_value(entry))
+
+    print(tabulate(data, headers="keys"))
 
 
 def number_of_workers():
     return (multiprocessing.cpu_count() * 2) + 1
 
 
+# Scheduler
+def scheduler():
+    _thread.start_new_thread(start_scheduler, ())
+
+
+# Server
 class StandaloneApplication(gunicorn.app.base.BaseApplication):
     def __init__(self, app, options=None):
         self.options = options or {}
         self.application = app
         super().__init__()
 
     def load_config(self):
@@ -40,14 +54,43 @@
             self.cfg.set(key.lower(), value)
 
     def load(self):
         return self.application
 
 
 if __name__ == "__main__":
+
+    parser = argparse.ArgumentParser()
+    parser.add_argument(
+        "-d", "--settings", help="display all plugins settings", action="store_true"
+    )
+    parser.add_argument(
+        "-g",
+        "--generate",
+        help="generate base of lifeguard instance project",
+        action="store_true",
+    )
+    args = parser.parse_args()
+
+    if args.generate:
+        generate_base_project()
+        sys.exit(0)
+
+    LIFEGUARD_CONTEXT.only_settings = args.settings
+
+    setup(LIFEGUARD_CONTEXT)
+
+    if args.settings:
+        display_settings()
+        sys.exit(0)
+
+    scheduler()
+
+    from lifeguard.server import APP
+
     StandaloneApplication(
         APP,
         {
             "bind": "{}:{}".format("0.0.0.0", LIFEGUARD_SERVER_PORT),
             "workers": number_of_workers(),
         },
     ).run()
```

### Comparing `lifeguard-0.0.9/lifeguard/http_client.py` & `lifeguard-1.0.0/lifeguard/http_client.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,29 +2,38 @@
 Wrapper for http requests
 """
 import requests
 
 from lifeguard.settings import HTTP_PROXY, HTTPS_PROXY
 
 
-def post(url, data=None, headers=None):
+def get(url, headers=None, auth=None):
+    """
+    :param url:
+    :param headers:
+
+    :return: :class:`Response <Response>` object
+    :rtype: requests.Response
+    """
+    request_args = {"url": url, "headers": headers, "auth": auth}
+    __append_proxies(request_args)
+    return requests.get(**request_args)
+
+
+def post(url, data=None, headers=None, auth=None):
     """
     :param url:
     :param data:
     :param headers:
 
     :return: :class:`Response <Response>` object
     :rtype: requests.Response
     """
 
-    request_args = {
-        "url": url,
-        "headers": headers,
-        "data": data,
-    }
+    request_args = {"url": url, "headers": headers, "data": data, "auth": auth}
     __append_proxies(request_args)
     return requests.post(**request_args)
 
 
 def __append_proxies(request_args):
     proxies = {
         "http": HTTP_PROXY,
```

### Comparing `lifeguard-0.0.9/lifeguard/logger.py` & `lifeguard-1.0.0/lifeguard/logger.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,16 +2,17 @@
 Settings for application logging
 """
 import json
 import logging
 import sys
 import time
 from datetime import datetime
+from logging.handlers import RotatingFileHandler
 
-from lifeguard.settings import LOG_LEVEL
+from lifeguard.settings import LOG_LEVEL, LOG_FILE, LOG_BACKUP_COUNT, LOG_MAX_BYTES
 
 
 class CustomFormatter(logging.Formatter):
     def __init__(self):
         super(CustomFormatter, self).__init__()
 
     def format(self, record):
@@ -51,11 +52,19 @@
 
 
 logging.setLoggerClass(CustomLogger)
 lifeguard_logger = logging.getLogger("lifeguard")
 lifeguard_logger.propagate = 0
 lifeguard_logger.setLevel(getattr(logging, LOG_LEVEL))
 
+if LOG_FILE:
+    LIFEGUARD_FILE_HANDLER = RotatingFileHandler(
+        LOG_FILE, maxBytes=LOG_MAX_BYTES, backupCount=LOG_BACKUP_COUNT
+    )
+    LIFEGUARD_FILE_HANDLER.setFormatter(CustomFormatter())
+    lifeguard_logger.addHandler(LIFEGUARD_FILE_HANDLER)
+
+
 LIFEGUARD_HANDLER = logging.StreamHandler()
 LIFEGUARD_HANDLER.setFormatter(CustomFormatter())
 
 lifeguard_logger.addHandler(LIFEGUARD_HANDLER)
```

### Comparing `lifeguard-0.0.9/lifeguard/notifications.py` & `lifeguard-1.0.0/lifeguard/notifications.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,80 @@
 """
 Base of notification system
 """
 
 from datetime import datetime
-from json import JSONEncoder
 
 from lifeguard.logger import lifeguard_logger as logger
 
 NOTIFICATION_METHODS = []
 
+SINGLE_MESSAGE_NOTIFICATION = "single"
+INIT_THREAD_MESSAGE_NOTIFICATION = "init_thread"
+UPDATE_THREAD_MESSAGE_NOTIFICATION = "update_thread"
+CLOSE_THREAD_MESSAGE_NOTIFICATION = "close_thread"
+NOTIFICATION_TYPE = []
+
+
+class NotificationOccurrence:
+    """
+    Notification history entry
+    """
+
+    def __init__(
+        self, validation_name, details, status, notification_type, created_at=None
+    ):
+        self._validation_name = validation_name
+        self._details = details
+        self._status = status
+        self._notification_type = notification_type
+        self._created_at = created_at if created_at else datetime.now()
+
+    @property
+    def validation_name(self):
+        """
+        Return validation name
+        """
+        return self._validation_name
+
+    @property
+    def details(self):
+        """
+        Return details
+        """
+        return self._details
+
+    @property
+    def status(self):
+        """
+        Return status
+        """
+        return self._status
+
+    @property
+    def notification_type(self):
+        """
+        Return notification type
+        """
+        return self._notification_type
+
+    @property
+    def created_at(self):
+        """
+        Return created_at
+        """
+        return self._created_at
+
 
 class NotificationStatus:
     """
     Notification status class
     """
 
-    def __init__(self, validation_name, thread_ids, options=None):
+    def __init__(self, validation_name, thread_ids, options=None, content=None):
         self._validation_name = validation_name
         self._thread_ids = thread_ids
         self._options = options
         self._opened = True
         self._last_notification = datetime.now()
 
     @property
@@ -98,27 +153,14 @@
             )
         return attributes
 
     def __str__(self):
         return str(self.get_attributes())
 
 
-class ValidationResponseEncoder(JSONEncoder):
-    """
-    Enconder for Validation Response
-    """
-
-    def default(self, validation_response):
-        """
-        Default implementation for validation response encoder
-        """
-
-        return validation_response.get_attributes()
-
-
 class NotificationBase:
     """
     Base of notification
     """
 
     @property
     def name(self):
```

### Comparing `lifeguard-0.0.9/lifeguard/repositories.py` & `lifeguard-1.0.0/lifeguard/repositories.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,30 +20,52 @@
     def save_validation_result(self, validation_result):
         validation_result.last_execution = datetime.now()
         self.__implementation__.save_validation_result(validation_result)
 
     def fetch_last_validation_result(self, validation_name):
         return self.__implementation__.fetch_last_validation_result(validation_name)
 
+    def fetch_all_validation_results(self):
+        return self.__implementation__.fetch_all_validation_results()
+
 
 class NotificationRepository(BaseRepository):
     def __init__(self):
         BaseRepository.__init_repository__(self, "notification")
 
     def save_last_notification_for_a_validation(self, notification):
         self.__implementation__.save_last_notification_for_a_validation(notification)
 
     def fetch_last_notification_for_a_validation(self, validation_name):
         return self.__implementation__.fetch_last_notification_for_a_validation(
             validation_name
         )
 
 
-def declare_implementation(repository, implementation):
+class HistoryRepository(BaseRepository):
+    def __init__(self):
+        BaseRepository.__init_repository__(self, "history")
+
+    def append_notification(self, notification_occurrence):
+        self.__implementation__.append_notification(notification_occurrence)
+
+    def fetch_notifications(
+        self, start_interval, end_interval, filters={}, page=None, limit=None
+    ):
+        return self.__implementation__.fetch_notifications(
+            start_interval, end_interval, filters, page, limit
+        )
+
+    def count_notifications(self, start_interval=None, end_interval=None, filters={}):
+        return self.__implementation__.count_notifications(
+            start_interval, end_interval, filters
+        )
 
+
+def declare_implementation(repository, implementation):
     if repository in IMPLEMENTATIONS:
         logger.warning("overwriting implementation for respository %s", repository)
     logger.info(
         "loading implementation %s for repository %s",
         implementation.__name__,
         repository,
     )
```

### Comparing `lifeguard-0.0.9/lifeguard.egg-info/SOURCES.txt` & `lifeguard-1.0.0/lifeguard.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,50 @@
 README.md
 setup.cfg
 setup.py
 bin/lifeguard
 lifeguard/__init__.py
-lifeguard/controllers.py
+lifeguard/auth.py
+lifeguard/bootstrap.py
+lifeguard/context.py
 lifeguard/http_client.py
 lifeguard/logger.py
 lifeguard/notifications.py
 lifeguard/repositories.py
 lifeguard/scheduler.py
 lifeguard/server.py
 lifeguard/settings.py
+lifeguard/statuses.py
+lifeguard/utils.py
 lifeguard/validations.py
 lifeguard.egg-info/PKG-INFO
 lifeguard.egg-info/SOURCES.txt
 lifeguard.egg-info/dependency_links.txt
 lifeguard.egg-info/requires.txt
 lifeguard.egg-info/top_level.txt
 lifeguard/actions/__init__.py
 lifeguard/actions/database.py
+lifeguard/actions/email.py
 lifeguard/actions/notifications.py
+lifeguard/controllers/__init__.py
+lifeguard/controllers/assets.py
 tests/__init__.py
+tests/test_auth.py
+tests/test_bootstrap.py
 tests/test_controllers.py
 tests/test_http_client.py
 tests/test_lifeguard_core.py
 tests/test_notifications.py
 tests/test_repositories.py
 tests/test_scheduler.py
 tests/test_server.py
 tests/test_settings.py
 tests/test_validations.py
 tests/actions/__init__.py
 tests/actions/test_database.py
+tests/actions/test_email.py
 tests/actions/test_notification.py
+tests/controllers/__init__.py
+tests/controllers/test_assets.py
 tests/fixtures/__init__.py
 tests/fixtures/fixtures_repositories.py
 tests/fixtures/mock_lifeguard_settings.py
```

### Comparing `lifeguard-0.0.9/setup.py` & `lifeguard-1.0.0/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-from setuptools import setup, find_packages
+from setuptools import find_packages, setup
 
 setup(
     name="lifeguard",
-    version="0.0.9",
+    version="1.0.0",
     url="https://github.com/LifeguardSystem/lifeguard",
     author="Diego Rubin",
     author_email="contact@diegorubin.dev",
     license="GPL2",
     scripts=["bin/lifeguard"],
     include_package_data=True,
     description="Application to monitor your systems and give you the security to sleep peacefully at night",
-    install_requires=["flask", "schedule", "gunicorn", "requests"],
+    install_requires=["flask", "schedule", "gunicorn", "requests", "tabulate"],
     classifiers=["Development Status :: 3 - Alpha"],
     packages=find_packages(),
 )
```

### Comparing `lifeguard-0.0.9/tests/actions/test_database.py` & `lifeguard-1.0.0/tests/actions/test_database.py`

 * *Files identical despite different names*

### Comparing `lifeguard-0.0.9/tests/test_http_client.py` & `lifeguard-1.0.0/tests/test_http_client.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,72 @@
 import unittest
 from unittest.mock import patch
 
-from lifeguard.http_client import post
+from lifeguard.http_client import post, get
 
 
 class TestHttpClient(unittest.TestCase):
     @patch("lifeguard.http_client.HTTP_PROXY", "http_proxy")
     @patch("lifeguard.http_client.requests")
     def test_call_post_with_http_proxy(self, mock_requests):
         post("url", data="data", headers="headers")
         mock_requests.post.assert_called_with(
-            url="url", headers="headers", data="data", proxies={"http": "http_proxy"}
+            url="url",
+            headers="headers",
+            data="data",
+            auth=None,
+            proxies={"http": "http_proxy"},
         )
 
     @patch("lifeguard.http_client.HTTPS_PROXY", "https_proxy")
     @patch("lifeguard.http_client.requests")
     def test_call_post_with_https_proxy(self, mock_requests):
         post("url", data="data", headers="headers")
         mock_requests.post.assert_called_with(
-            url="url", headers="headers", data="data", proxies={"https": "https_proxy"}
+            url="url",
+            headers="headers",
+            data="data",
+            auth=None,
+            proxies={"https": "https_proxy"},
         )
 
     @patch("lifeguard.http_client.requests")
     def test_call_post_without_proxy(self, mock_requests):
         post("url", data="data", headers="headers")
-        mock_requests.post.assert_called_with(url="url", headers="headers", data="data")
+        mock_requests.post.assert_called_with(
+            url="url", headers="headers", data="data", auth=None
+        )
+
+    @patch("lifeguard.http_client.requests")
+    def test_call_post_with_auth(self, mock_requests):
+        post("url", data="data", headers="headers", auth=("user", "passwd"))
+        mock_requests.post.assert_called_with(
+            url="url", headers="headers", data="data", auth=("user", "passwd")
+        )
+
+    @patch("lifeguard.http_client.HTTP_PROXY", "http_proxy")
+    @patch("lifeguard.http_client.requests")
+    def test_call_get_with_http_proxy(self, mock_requests):
+        get("url", headers="headers")
+        mock_requests.get.assert_called_with(
+            url="url", headers="headers", auth=None, proxies={"http": "http_proxy"}
+        )
+
+    @patch("lifeguard.http_client.HTTPS_PROXY", "https_proxy")
+    @patch("lifeguard.http_client.requests")
+    def test_call_get_with_https_proxy(self, mock_requests):
+        get("url", headers="headers")
+        mock_requests.get.assert_called_with(
+            url="url", headers="headers", auth=None, proxies={"https": "https_proxy"}
+        )
+
+    @patch("lifeguard.http_client.requests")
+    def test_call_get_without_proxy(self, mock_requests):
+        get("url", headers="headers")
+        mock_requests.get.assert_called_with(url="url", headers="headers", auth=None)
+
+    @patch("lifeguard.http_client.requests")
+    def test_call_get_with_auth(self, mock_requests):
+        get("url", headers="headers", auth=("user", "password"))
+        mock_requests.get.assert_called_with(
+            url="url", headers="headers", auth=("user", "password")
+        )
```

### Comparing `lifeguard-0.0.9/tests/test_lifeguard_core.py` & `lifeguard-1.0.0/tests/test_lifeguard_core.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     change_status,
     setup,
     NORMAL,
     WARNING,
     PROBLEM,
     ACTION_STATUSES,
 )
+from lifeguard.context import LIFEGUARD_CONTEXT
 
 from tests.fixtures import mock_lifeguard_settings
 
 
 class TestLifeguardCore(unittest.TestCase):
     def test_statuses(self):
         self.assertEqual(NORMAL, "NORMAL")
@@ -29,9 +30,9 @@
     @patch("lifeguard.load_validations")
     @patch("lifeguard.recover_settings")
     def test_setup_call_load_validations(
         self, mock_recover_settings, mock_load_validations
     ):
         mock_recover_settings.return_value = mock_lifeguard_settings
 
-        setup()
+        setup(LIFEGUARD_CONTEXT)
         mock_load_validations.assert_called()
```

### Comparing `lifeguard-0.0.9/tests/test_notifications.py` & `lifeguard-1.0.0/tests/test_notifications.py`

 * *Files identical despite different names*

### Comparing `lifeguard-0.0.9/tests/test_repositories.py` & `lifeguard-1.0.0/tests/test_repositories.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import unittest
 from unittest.mock import MagicMock, patch
 import sys
 
 from lifeguard.repositories import (
     IMPLEMENTATIONS,
+    HistoryRepository,
     NotificationRepository,
     ValidationRepository,
     declare_implementation,
 )
 
 sys.path.append("tests/fixtures")
 
-NAMES = ["notification", "validation"]
+NAMES = ["history", "notification", "validation"]
 
 
 class TestNotificationRepository(unittest.TestCase):
     def setUp(self):
         for name in NAMES:
             if name in IMPLEMENTATIONS:
                 IMPLEMENTATIONS.pop(name)
@@ -44,14 +45,59 @@
             validation_name
         )
         self.implementation.fetch_last_notification_for_a_validation.assert_called_with(
             validation_name
         )
 
 
+class TestHistoryRepository(unittest.TestCase):
+    def setUp(self):
+        for name in NAMES:
+            if name in IMPLEMENTATIONS:
+                IMPLEMENTATIONS.pop(name)
+
+        self.implementation = MagicMock(name="implementation")
+
+        with patch("lifeguard.repositories.logger"):
+            implementation_class = MagicMock(name="implementation_class")
+            implementation_class.__name__ = "mocked_implementation"
+            implementation_class.return_value = self.implementation
+
+            declare_implementation("history", implementation_class)
+
+        self.history_repository = HistoryRepository()
+
+    def test_append_notification(self):
+        notification_occurrence = MagicMock(name="notification_occurrence")
+        self.history_repository.append_notification(notification_occurrence)
+        self.implementation.append_notification.assert_called_with(
+            notification_occurrence
+        )
+
+    def test_count_notifications(self):
+        result = self.history_repository.count_notifications()
+
+        self.implementation.count_notifications.assert_called_with(None, None, {})
+        self.assertIsNotNone(result)
+
+    def test_fetch_notifications(self):
+        start_interval = MagicMock(name="start_interval")
+        end_interval = MagicMock(name="end_interval")
+        filters = MagicMock(name="filters")
+
+        result = self.history_repository.fetch_notifications(
+            start_interval, end_interval, filters
+        )
+
+        self.implementation.fetch_notifications.assert_called_with(
+            start_interval, end_interval, filters, None, None
+        )
+        self.assertIsNotNone(result)
+
+
 class TestValidationRepositories(unittest.TestCase):
     def setUp(self):
         for name in NAMES:
             if name in IMPLEMENTATIONS:
                 IMPLEMENTATIONS.pop(name)
 
         self.implementation = MagicMock(name="implementation")
@@ -74,14 +120,18 @@
     def test_validation_repository_fetch_last_validation_result(self):
         validation_name = MagicMock(name="validation_name")
         self.validation_repository.fetch_last_validation_result(validation_name)
         self.implementation.fetch_last_validation_result.assert_called_with(
             validation_name
         )
 
+    def test_validation_repository_fetch_all_validation_results(self):
+        self.validation_repository.fetch_all_validation_results()
+        self.implementation.fetch_all_validation_results.assert_called()
+
 
 class TestRepositoriesFunctions(unittest.TestCase):
     def setUp(self):
         if "test" in IMPLEMENTATIONS:
             IMPLEMENTATIONS.pop("test")
         self.implementation = MagicMock(name="implementation")
         self.implementation.__name__ = "test"
```

