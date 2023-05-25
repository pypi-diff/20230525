# Comparing `tmp/lifeguard-1.0.0.tar.gz` & `tmp/lifeguard-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lifeguard-1.0.0.tar", last modified: Thu May 25 14:33:25 2023, max compression
+gzip compressed data, was "lifeguard-1.0.1.tar", last modified: Thu May 25 15:04:40 2023, max compression
```

## Comparing `lifeguard-1.0.0.tar` & `lifeguard-1.0.1.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:33:25.948863 lifeguard-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-25 14:33:25.948863 lifeguard-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4566 2023-05-25 14:33:10.000000 lifeguard-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:33:25.940863 lifeguard-1.0.0/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2399 2023-05-25 14:33:10.000000 lifeguard-1.0.0/bin/lifeguard
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:33:25.940863 lifeguard-1.0.0/lifeguard/
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-05-25 14:33:10.000000 lifeguard-1.0.0/lifeguard/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:33:25.944863 lifeguard-1.0.0/lifeguard/actions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:33:10.000000 lifeguard-1.0.0/lifeguard/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-25 14:33:10.000000 lifeguard-1.0.0/lifeguard/actions/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-05-25 14:33:10.000000 lifeguard-1.0.0/lifeguard/actions/email.py
--rw-r--r--   0 runner    (1001) docker     (123)     6248 2023-05-25 14:33:10.000000 lifeguard-1.0.0/lifeguard/actions/notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-05-25 14:33:10.000000 lifeguard-1.0.0/lifeguard/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-05-25 14:33:10.000000 lifeguard-1.0.0/lifeguard/bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-05-25 14:33:10.000000 lifeguard-1.0.0/lifeguard/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:33:25.944863 lifeguard-1.0.0/lifeguard/controllers/
--rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-05-25 14:33:10.000000 lifeguard-1.0.0/lifeguard/controllers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-05-25 14:33:10.000000 lifeguard-1.0.0/lifeguard/controllers/assets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-25 14:33:10.000000 lifeguard-1.0.0/lifeguard/http_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-05-25 14:33:10.000000 lifeguard-1.0.0/lifeguard/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     4551 2023-05-25 14:33:10.000000 lifeguard-1.0.0/lifeguard/notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-05-25 14:33:10.000000 lifeguard-1.0.0/lifeguard/repositories.py
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-05-25 14:33:10.000000 lifeguard-1.0.0/lifeguard/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-05-25 14:33:10.000000 lifeguard-1.0.0/lifeguard/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     6810 2023-05-25 14:33:10.000000 lifeguard-1.0.0/lifeguard/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-25 14:33:10.000000 lifeguard-1.0.0/lifeguard/statuses.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-25 14:33:10.000000 lifeguard-1.0.0/lifeguard/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5817 2023-05-25 14:33:10.000000 lifeguard-1.0.0/lifeguard/validations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:33:25.944863 lifeguard-1.0.0/lifeguard.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-25 14:33:25.000000 lifeguard-1.0.0/lifeguard.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-05-25 14:33:25.000000 lifeguard-1.0.0/lifeguard.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 14:33:25.000000 lifeguard-1.0.0/lifeguard.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-25 14:33:25.000000 lifeguard-1.0.0/lifeguard.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-25 14:33:25.000000 lifeguard-1.0.0/lifeguard.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-25 14:33:25.948863 lifeguard-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-25 14:33:10.000000 lifeguard-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:33:25.944863 lifeguard-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:33:10.000000 lifeguard-1.0.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:33:25.948863 lifeguard-1.0.0/tests/actions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:33:10.000000 lifeguard-1.0.0/tests/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-25 14:33:10.000000 lifeguard-1.0.0/tests/actions/test_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     5295 2023-05-25 14:33:10.000000 lifeguard-1.0.0/tests/actions/test_email.py
--rw-r--r--   0 runner    (1001) docker     (123)    15144 2023-05-25 14:33:10.000000 lifeguard-1.0.0/tests/actions/test_notification.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:33:25.948863 lifeguard-1.0.0/tests/controllers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:33:10.000000 lifeguard-1.0.0/tests/controllers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-05-25 14:33:10.000000 lifeguard-1.0.0/tests/controllers/test_assets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:33:25.948863 lifeguard-1.0.0/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:33:10.000000 lifeguard-1.0.0/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-25 14:33:10.000000 lifeguard-1.0.0/tests/fixtures/fixtures_repositories.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-25 14:33:10.000000 lifeguard-1.0.0/tests/fixtures/mock_lifeguard_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-05-25 14:33:10.000000 lifeguard-1.0.0/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-25 14:33:10.000000 lifeguard-1.0.0/tests/test_bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)    11566 2023-05-25 14:33:10.000000 lifeguard-1.0.0/tests/test_controllers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-05-25 14:33:10.000000 lifeguard-1.0.0/tests/test_http_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-05-25 14:33:10.000000 lifeguard-1.0.0/tests/test_lifeguard_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-05-25 14:33:10.000000 lifeguard-1.0.0/tests/test_notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)     5781 2023-05-25 14:33:10.000000 lifeguard-1.0.0/tests/test_repositories.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-05-25 14:33:10.000000 lifeguard-1.0.0/tests/test_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-05-25 14:33:10.000000 lifeguard-1.0.0/tests/test_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     7064 2023-05-25 14:33:10.000000 lifeguard-1.0.0/tests/test_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     6932 2023-05-25 14:33:10.000000 lifeguard-1.0.0/tests/test_validations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:04:40.246731 lifeguard-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-05-25 15:04:40.246731 lifeguard-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4419 2023-05-25 15:04:29.000000 lifeguard-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:04:40.242731 lifeguard-1.0.1/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2399 2023-05-25 15:04:29.000000 lifeguard-1.0.1/bin/lifeguard
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:04:40.242731 lifeguard-1.0.1/lifeguard/
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-05-25 15:04:29.000000 lifeguard-1.0.1/lifeguard/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:04:40.246731 lifeguard-1.0.1/lifeguard/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:04:29.000000 lifeguard-1.0.1/lifeguard/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-25 15:04:29.000000 lifeguard-1.0.1/lifeguard/actions/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-05-25 15:04:29.000000 lifeguard-1.0.1/lifeguard/actions/email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6248 2023-05-25 15:04:29.000000 lifeguard-1.0.1/lifeguard/actions/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-05-25 15:04:29.000000 lifeguard-1.0.1/lifeguard/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-05-25 15:04:29.000000 lifeguard-1.0.1/lifeguard/bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-05-25 15:04:29.000000 lifeguard-1.0.1/lifeguard/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:04:40.246731 lifeguard-1.0.1/lifeguard/controllers/
+-rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-05-25 15:04:29.000000 lifeguard-1.0.1/lifeguard/controllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-05-25 15:04:29.000000 lifeguard-1.0.1/lifeguard/controllers/assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-25 15:04:29.000000 lifeguard-1.0.1/lifeguard/http_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-05-25 15:04:29.000000 lifeguard-1.0.1/lifeguard/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4551 2023-05-25 15:04:29.000000 lifeguard-1.0.1/lifeguard/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-05-25 15:04:29.000000 lifeguard-1.0.1/lifeguard/repositories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-05-25 15:04:29.000000 lifeguard-1.0.1/lifeguard/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-05-25 15:04:29.000000 lifeguard-1.0.1/lifeguard/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6810 2023-05-25 15:04:29.000000 lifeguard-1.0.1/lifeguard/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-25 15:04:29.000000 lifeguard-1.0.1/lifeguard/statuses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-25 15:04:29.000000 lifeguard-1.0.1/lifeguard/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5817 2023-05-25 15:04:29.000000 lifeguard-1.0.1/lifeguard/validations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:04:40.242731 lifeguard-1.0.1/lifeguard.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-05-25 15:04:40.000000 lifeguard-1.0.1/lifeguard.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-05-25 15:04:40.000000 lifeguard-1.0.1/lifeguard.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 15:04:40.000000 lifeguard-1.0.1/lifeguard.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-25 15:04:40.000000 lifeguard-1.0.1/lifeguard.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-25 15:04:40.000000 lifeguard-1.0.1/lifeguard.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-25 15:04:40.246731 lifeguard-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-25 15:04:29.000000 lifeguard-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:04:40.246731 lifeguard-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:04:29.000000 lifeguard-1.0.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:04:40.246731 lifeguard-1.0.1/tests/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:04:29.000000 lifeguard-1.0.1/tests/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-25 15:04:29.000000 lifeguard-1.0.1/tests/actions/test_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5295 2023-05-25 15:04:29.000000 lifeguard-1.0.1/tests/actions/test_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15144 2023-05-25 15:04:29.000000 lifeguard-1.0.1/tests/actions/test_notification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:04:40.246731 lifeguard-1.0.1/tests/controllers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:04:29.000000 lifeguard-1.0.1/tests/controllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-05-25 15:04:29.000000 lifeguard-1.0.1/tests/controllers/test_assets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:04:40.246731 lifeguard-1.0.1/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:04:29.000000 lifeguard-1.0.1/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-25 15:04:29.000000 lifeguard-1.0.1/tests/fixtures/fixtures_repositories.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-25 15:04:29.000000 lifeguard-1.0.1/tests/fixtures/mock_lifeguard_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-05-25 15:04:29.000000 lifeguard-1.0.1/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-25 15:04:29.000000 lifeguard-1.0.1/tests/test_bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11566 2023-05-25 15:04:29.000000 lifeguard-1.0.1/tests/test_controllers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-05-25 15:04:29.000000 lifeguard-1.0.1/tests/test_http_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-05-25 15:04:29.000000 lifeguard-1.0.1/tests/test_lifeguard_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-05-25 15:04:29.000000 lifeguard-1.0.1/tests/test_notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5781 2023-05-25 15:04:29.000000 lifeguard-1.0.1/tests/test_repositories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-05-25 15:04:29.000000 lifeguard-1.0.1/tests/test_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-05-25 15:04:29.000000 lifeguard-1.0.1/tests/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7064 2023-05-25 15:04:29.000000 lifeguard-1.0.1/tests/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6932 2023-05-25 15:04:29.000000 lifeguard-1.0.1/tests/test_validations.py
```

### Comparing `lifeguard-1.0.0/README.md` & `lifeguard-1.0.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # Lifeguard
 
 ![Build Status](https://github.com/LifeguardSystem/lifeguard/workflows/Lifeguard%20Core%20CI/badge.svg)
 ![Lifeguard Core Publish](https://github.com/LifeguardSystem/lifeguard/workflows/Lifeguard%20Core%20Publish/badge.svg)
 [![PyPI version](https://badge.fury.io/py/lifeguard.svg)](https://badge.fury.io/py/lifeguard)
-[![SourceLevel](https://app.sourcelevel.io/github/LifeguardSystem/-/lifeguard.svg)](https://app.sourcelevel.io/github/LifeguardSystem/-/lifeguard)
 
 ## Examples of Usage
 
 See a complete example at: https://github.com/LifeguardSystem/lifeguard-example
 
 ### Settings File
```

### Comparing `lifeguard-1.0.0/bin/lifeguard` & `lifeguard-1.0.1/bin/lifeguard`

 * *Files identical despite different names*

### Comparing `lifeguard-1.0.0/lifeguard/__init__.py` & `lifeguard-1.0.1/lifeguard/__init__.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.0.0/lifeguard/actions/email.py` & `lifeguard-1.0.1/lifeguard/actions/email.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.0.0/lifeguard/actions/notifications.py` & `lifeguard-1.0.1/lifeguard/actions/notifications.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.0.0/lifeguard/auth.py` & `lifeguard-1.0.1/lifeguard/auth.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.0.0/lifeguard/context.py` & `lifeguard-1.0.1/lifeguard/context.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.0.0/lifeguard/controllers/__init__.py` & `lifeguard-1.0.1/lifeguard/controllers/__init__.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.0.0/lifeguard/controllers/assets.py` & `lifeguard-1.0.1/lifeguard/controllers/assets.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.0.0/lifeguard/http_client.py` & `lifeguard-1.0.1/lifeguard/http_client.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.0.0/lifeguard/logger.py` & `lifeguard-1.0.1/lifeguard/logger.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.0.0/lifeguard/notifications.py` & `lifeguard-1.0.1/lifeguard/notifications.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.0.0/lifeguard/repositories.py` & `lifeguard-1.0.1/lifeguard/repositories.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.0.0/lifeguard/scheduler.py` & `lifeguard-1.0.1/lifeguard/scheduler.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.0.0/lifeguard/server.py` & `lifeguard-1.0.1/lifeguard/server.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.0.0/lifeguard/settings.py` & `lifeguard-1.0.1/lifeguard/settings.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.0.0/lifeguard/validations.py` & `lifeguard-1.0.1/lifeguard/validations.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.0.0/lifeguard.egg-info/SOURCES.txt` & `lifeguard-1.0.1/lifeguard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lifeguard-1.0.0/tests/actions/test_database.py` & `lifeguard-1.0.1/tests/actions/test_database.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.0.0/tests/actions/test_email.py` & `lifeguard-1.0.1/tests/actions/test_email.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.0.0/tests/actions/test_notification.py` & `lifeguard-1.0.1/tests/actions/test_notification.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.0.0/tests/controllers/test_assets.py` & `lifeguard-1.0.1/tests/controllers/test_assets.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.0.0/tests/test_auth.py` & `lifeguard-1.0.1/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.0.0/tests/test_bootstrap.py` & `lifeguard-1.0.1/tests/test_bootstrap.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.0.0/tests/test_controllers.py` & `lifeguard-1.0.1/tests/test_controllers.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.0.0/tests/test_http_client.py` & `lifeguard-1.0.1/tests/test_http_client.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.0.0/tests/test_lifeguard_core.py` & `lifeguard-1.0.1/tests/test_lifeguard_core.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.0.0/tests/test_notifications.py` & `lifeguard-1.0.1/tests/test_notifications.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.0.0/tests/test_repositories.py` & `lifeguard-1.0.1/tests/test_repositories.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.0.0/tests/test_scheduler.py` & `lifeguard-1.0.1/tests/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.0.0/tests/test_server.py` & `lifeguard-1.0.1/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.0.0/tests/test_settings.py` & `lifeguard-1.0.1/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.0.0/tests/test_validations.py` & `lifeguard-1.0.1/tests/test_validations.py`

 * *Files identical despite different names*

