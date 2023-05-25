# Comparing `tmp/percy-appium-app-1.2.0.tar.gz` & `tmp/percy-appium-app-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "percy-appium-app-1.2.0.tar", last modified: Wed Apr 12 12:27:28 2023, max compression
+gzip compressed data, was "percy-appium-app-1.2.1.tar", last modified: Thu May 25 11:53:48 2023, max compression
```

## Comparing `percy-appium-app-1.2.0.tar` & `percy-appium-app-1.2.1.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:27:28.524994 percy-appium-app-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-12 12:27:06.000000 percy-appium-app-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5136 2023-04-12 12:27:28.524994 percy-appium-app-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-04-12 12:27:06.000000 percy-appium-app-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:27:28.516994 percy-appium-app-1.2.0/percy/
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-12 12:27:06.000000 percy-appium-app-1.2.0/percy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:27:28.516994 percy-appium-app-1.2.0/percy/common/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-12 12:27:06.000000 percy-appium-app-1.2.0/percy/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:27:28.516994 percy-appium-app-1.2.0/percy/configs/
--rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-04-12 12:27:06.000000 percy-appium-app-1.2.0/percy/configs/devices.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:27:28.516994 percy-appium-app-1.2.0/percy/errors/
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-12 12:27:06.000000 percy-appium-app-1.2.0/percy/errors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:27:28.520994 percy-appium-app-1.2.0/percy/lib/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-12 12:27:06.000000 percy-appium-app-1.2.0/percy/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-04-12 12:27:06.000000 percy-appium-app-1.2.0/percy/lib/app_percy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-04-12 12:27:06.000000 percy-appium-app-1.2.0/percy/lib/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-04-12 12:27:06.000000 percy-appium-app-1.2.0/percy/lib/cli_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-04-12 12:27:06.000000 percy-appium-app-1.2.0/percy/lib/ignore_region.py
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-04-12 12:27:06.000000 percy-appium-app-1.2.0/percy/lib/percy_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-04-12 12:27:06.000000 percy-appium-app-1.2.0/percy/lib/tile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:27:28.520994 percy-appium-app-1.2.0/percy/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-12 12:27:06.000000 percy-appium-app-1.2.0/percy/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-04-12 12:27:06.000000 percy-appium-app-1.2.0/percy/metadata/android_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-04-12 12:27:06.000000 percy-appium-app-1.2.0/percy/metadata/ios_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-04-12 12:27:06.000000 percy-appium-app-1.2.0/percy/metadata/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-12 12:27:06.000000 percy-appium-app-1.2.0/percy/metadata/metadata_resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:27:28.520994 percy-appium-app-1.2.0/percy/providers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 12:27:06.000000 percy-appium-app-1.2.0/percy/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-04-12 12:27:06.000000 percy-appium-app-1.2.0/percy/providers/app_automate.py
--rw-r--r--   0 runner    (1001) docker     (123)     7253 2023-04-12 12:27:06.000000 percy-appium-app-1.2.0/percy/providers/generic_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-12 12:27:06.000000 percy-appium-app-1.2.0/percy/providers/provider_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-04-12 12:27:06.000000 percy-appium-app-1.2.0/percy/screenshot.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-12 12:27:06.000000 percy-appium-app-1.2.0/percy/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:27:28.520994 percy-appium-app-1.2.0/percy_appium_app.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5136 2023-04-12 12:27:28.000000 percy-appium-app-1.2.0/percy_appium_app.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-04-12 12:27:28.000000 percy-appium-app-1.2.0/percy_appium_app.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 12:27:28.000000 percy-appium-app-1.2.0/percy_appium_app.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 12:27:28.000000 percy-appium-app-1.2.0/percy_appium_app.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-12 12:27:28.000000 percy-appium-app-1.2.0/percy_appium_app.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-12 12:27:28.000000 percy-appium-app-1.2.0/percy_appium_app.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 12:27:28.524994 percy-appium-app-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-04-12 12:27:06.000000 percy-appium-app-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:27:28.520994 percy-appium-app-1.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-04-12 12:27:06.000000 percy-appium-app-1.2.0/tests/test_android_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     4900 2023-04-12 12:27:06.000000 percy-appium-app-1.2.0/tests/test_app_automate.py
--rw-r--r--   0 runner    (1001) docker     (123)     8709 2023-04-12 12:27:06.000000 percy-appium-app-1.2.0/tests/test_app_percy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-04-12 12:27:06.000000 percy-appium-app-1.2.0/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-04-12 12:27:06.000000 percy-appium-app-1.2.0/tests/test_cli_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    13581 2023-04-12 12:27:06.000000 percy-appium-app-1.2.0/tests/test_generic_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-04-12 12:27:06.000000 percy-appium-app-1.2.0/tests/test_ignore_region.py
--rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-04-12 12:27:06.000000 percy-appium-app-1.2.0/tests/test_ios_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-04-12 12:27:06.000000 percy-appium-app-1.2.0/tests/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-12 12:27:06.000000 percy-appium-app-1.2.0/tests/test_metadata_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     6178 2023-04-12 12:27:06.000000 percy-appium-app-1.2.0/tests/test_percy_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     8196 2023-04-12 12:27:06.000000 percy-appium-app-1.2.0/tests/test_screenshot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-04-12 12:27:06.000000 percy-appium-app-1.2.0/tests/test_tile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:53:48.358613 percy-appium-app-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-25 11:53:26.000000 percy-appium-app-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5334 2023-05-25 11:53:48.358613 percy-appium-app-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4577 2023-05-25 11:53:26.000000 percy-appium-app-1.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:53:48.354613 percy-appium-app-1.2.1/percy/
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-25 11:53:26.000000 percy-appium-app-1.2.1/percy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:53:48.354613 percy-appium-app-1.2.1/percy/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-25 11:53:26.000000 percy-appium-app-1.2.1/percy/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:53:48.354613 percy-appium-app-1.2.1/percy/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-05-25 11:53:26.000000 percy-appium-app-1.2.1/percy/configs/devices.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:53:48.354613 percy-appium-app-1.2.1/percy/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-25 11:53:26.000000 percy-appium-app-1.2.1/percy/errors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:53:48.354613 percy-appium-app-1.2.1/percy/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-25 11:53:26.000000 percy-appium-app-1.2.1/percy/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-05-25 11:53:26.000000 percy-appium-app-1.2.1/percy/lib/app_percy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-05-25 11:53:26.000000 percy-appium-app-1.2.1/percy/lib/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-05-25 11:53:26.000000 percy-appium-app-1.2.1/percy/lib/cli_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-25 11:53:26.000000 percy-appium-app-1.2.1/percy/lib/ignore_region.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-05-25 11:53:26.000000 percy-appium-app-1.2.1/percy/lib/percy_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-05-25 11:53:26.000000 percy-appium-app-1.2.1/percy/lib/tile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:53:48.354613 percy-appium-app-1.2.1/percy/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-25 11:53:26.000000 percy-appium-app-1.2.1/percy/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-05-25 11:53:26.000000 percy-appium-app-1.2.1/percy/metadata/android_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-05-25 11:53:26.000000 percy-appium-app-1.2.1/percy/metadata/ios_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-05-25 11:53:26.000000 percy-appium-app-1.2.1/percy/metadata/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-25 11:53:26.000000 percy-appium-app-1.2.1/percy/metadata/metadata_resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:53:48.354613 percy-appium-app-1.2.1/percy/providers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 11:53:26.000000 percy-appium-app-1.2.1/percy/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5350 2023-05-25 11:53:26.000000 percy-appium-app-1.2.1/percy/providers/app_automate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7253 2023-05-25 11:53:26.000000 percy-appium-app-1.2.1/percy/providers/generic_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-25 11:53:26.000000 percy-appium-app-1.2.1/percy/providers/provider_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-05-25 11:53:26.000000 percy-appium-app-1.2.1/percy/screenshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-25 11:53:26.000000 percy-appium-app-1.2.1/percy/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:53:48.354613 percy-appium-app-1.2.1/percy_appium_app.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5334 2023-05-25 11:53:48.000000 percy-appium-app-1.2.1/percy_appium_app.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-25 11:53:48.000000 percy-appium-app-1.2.1/percy_appium_app.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 11:53:48.000000 percy-appium-app-1.2.1/percy_appium_app.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 11:53:48.000000 percy-appium-app-1.2.1/percy_appium_app.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-25 11:53:48.000000 percy-appium-app-1.2.1/percy_appium_app.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-25 11:53:48.000000 percy-appium-app-1.2.1/percy_appium_app.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 11:53:48.358613 percy-appium-app-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-05-25 11:53:26.000000 percy-appium-app-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:53:48.358613 percy-appium-app-1.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-05-25 11:53:26.000000 percy-appium-app-1.2.1/tests/test_android_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5576 2023-05-25 11:53:26.000000 percy-appium-app-1.2.1/tests/test_app_automate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8709 2023-05-25 11:53:26.000000 percy-appium-app-1.2.1/tests/test_app_percy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-05-25 11:53:26.000000 percy-appium-app-1.2.1/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-05-25 11:53:26.000000 percy-appium-app-1.2.1/tests/test_cli_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13581 2023-05-25 11:53:26.000000 percy-appium-app-1.2.1/tests/test_generic_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-05-25 11:53:26.000000 percy-appium-app-1.2.1/tests/test_ignore_region.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-05-25 11:53:26.000000 percy-appium-app-1.2.1/tests/test_ios_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-05-25 11:53:26.000000 percy-appium-app-1.2.1/tests/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-25 11:53:26.000000 percy-appium-app-1.2.1/tests/test_metadata_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6178 2023-05-25 11:53:26.000000 percy-appium-app-1.2.1/tests/test_percy_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8196 2023-05-25 11:53:26.000000 percy-appium-app-1.2.1/tests/test_screenshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-05-25 11:53:26.000000 percy-appium-app-1.2.1/tests/test_tile.py
```

### Comparing `percy-appium-app-1.2.0/LICENSE` & `percy-appium-app-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.2.0/PKG-INFO` & `percy-appium-app-1.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: percy-appium-app
-Version: 1.2.0
+Version: 1.2.1
 Summary: Python client for visual testing with Percy for mobile apps
 Home-page: https://github.com/percy/percy-appium-python
 Author: Perceptual Inc.
 Author-email: team@percy.io
 License: MIT
 Keywords: appium percy visual testing
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -36,14 +36,16 @@
 pip install Percy appium package:
 
 ```ssh-session
 $ pip install percy-appium-app
 ```
 > Note: This package is tested on Python versions 3.6, 3.8, 3.9 as part of unit tests. It should ideally work on all Python 3.6+ versions
 
+[NOTE] Appium-Python-Client(>= v2.9.0) is having compatibility issues with urllib3 latest versions. To solve the issue it is recommended to add `urllib3>=1.26.15,<2` in your requirements.txt file.
+
 ## Usage
 
 This is an example test using the `percy_screenshot` function.
 
 ``` python
 from appium import webdriver
 from percy import percy_screenshot
```

### Comparing `percy-appium-app-1.2.0/README.md` & `percy-appium-app-1.2.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 pip install Percy appium package:
 
 ```ssh-session
 $ pip install percy-appium-app
 ```
 > Note: This package is tested on Python versions 3.6, 3.8, 3.9 as part of unit tests. It should ideally work on all Python 3.6+ versions
 
+[NOTE] Appium-Python-Client(>= v2.9.0) is having compatibility issues with urllib3 latest versions. To solve the issue it is recommended to add `urllib3>=1.26.15,<2` in your requirements.txt file.
+
 ## Usage
 
 This is an example test using the `percy_screenshot` function.
 
 ``` python
 from appium import webdriver
 from percy import percy_screenshot
```

### Comparing `percy-appium-app-1.2.0/percy/__init__.py` & `percy-appium-app-1.2.1/percy/__init__.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.2.0/percy/configs/devices.json` & `percy-appium-app-1.2.1/percy/configs/devices.json`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.2.0/percy/lib/app_percy.py` & `percy-appium-app-1.2.1/percy/lib/app_percy.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.2.0/percy/lib/cache.py` & `percy-appium-app-1.2.1/percy/lib/cache.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.2.0/percy/lib/cli_wrapper.py` & `percy-appium-app-1.2.1/percy/lib/cli_wrapper.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.2.0/percy/lib/ignore_region.py` & `percy-appium-app-1.2.1/percy/lib/ignore_region.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.2.0/percy/lib/percy_options.py` & `percy-appium-app-1.2.1/percy/lib/percy_options.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.2.0/percy/lib/tile.py` & `percy-appium-app-1.2.1/percy/lib/tile.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.2.0/percy/metadata/android_metadata.py` & `percy-appium-app-1.2.1/percy/metadata/android_metadata.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.2.0/percy/metadata/ios_metadata.py` & `percy-appium-app-1.2.1/percy/metadata/ios_metadata.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.2.0/percy/metadata/metadata.py` & `percy-appium-app-1.2.1/percy/metadata/metadata.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.2.0/percy/providers/app_automate.py` & `percy-appium-app-1.2.1/percy/providers/app_automate.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,16 +4,17 @@
 from percy.lib.tile import Tile
 from percy.providers.generic_provider import GenericProvider
 
 
 class AppAutomate(GenericProvider):
     @staticmethod
     def supports(remote_url) -> bool:
-        if isinstance(remote_url, str) and remote_url.rfind('browserstack') > -1:
-            return True
+        if isinstance(remote_url, str):
+            if remote_url.rfind("browserstack" if os.getenv("AA_DOMAIN") is None else os.getenv("AA_DOMAIN")) > -1:
+                return True
         return False
 
     def screenshot(self, name: str, **kwargs):
         session_details = self.execute_percy_screenshot_begin(name)
         # Device name and OS version retrieval is custom for App Automate users
         if session_details is not None:
             self.metadata._device_name = kwargs.get('device_name') or session_details.get("deviceName")
```

### Comparing `percy-appium-app-1.2.0/percy/providers/generic_provider.py` & `percy-appium-app-1.2.1/percy/providers/generic_provider.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.2.0/percy/providers/provider_resolver.py` & `percy-appium-app-1.2.1/percy/providers/provider_resolver.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.2.0/percy/screenshot.py` & `percy-appium-app-1.2.1/percy/screenshot.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.2.0/percy_appium_app.egg-info/PKG-INFO` & `percy-appium-app-1.2.1/percy_appium_app.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: percy-appium-app
-Version: 1.2.0
+Version: 1.2.1
 Summary: Python client for visual testing with Percy for mobile apps
 Home-page: https://github.com/percy/percy-appium-python
 Author: Perceptual Inc.
 Author-email: team@percy.io
 License: MIT
 Keywords: appium percy visual testing
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -36,14 +36,16 @@
 pip install Percy appium package:
 
 ```ssh-session
 $ pip install percy-appium-app
 ```
 > Note: This package is tested on Python versions 3.6, 3.8, 3.9 as part of unit tests. It should ideally work on all Python 3.6+ versions
 
+[NOTE] Appium-Python-Client(>= v2.9.0) is having compatibility issues with urllib3 latest versions. To solve the issue it is recommended to add `urllib3>=1.26.15,<2` in your requirements.txt file.
+
 ## Usage
 
 This is an example test using the `percy_screenshot` function.
 
 ``` python
 from appium import webdriver
 from percy import percy_screenshot
```

### Comparing `percy-appium-app-1.2.0/percy_appium_app.egg-info/SOURCES.txt` & `percy-appium-app-1.2.1/percy_appium_app.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.2.0/setup.py` & `percy-appium-app-1.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.2.0/tests/test_android_metadata.py` & `percy-appium-app-1.2.1/tests/test_android_metadata.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.2.0/tests/test_app_automate.py` & `percy-appium-app-1.2.1/tests/test_app_automate.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # pylint: disable=[arguments-differ, protected-access]
 import unittest
+import os
 from unittest.mock import MagicMock, patch, PropertyMock
 from appium.webdriver.webdriver import WebDriver
 from percy.providers.app_automate import AppAutomate
 from percy.providers.generic_provider import GenericProvider
 from percy.metadata import AndroidMetadata, Metadata
 from tests.mocks.mock_methods import android_capabilities
 
@@ -25,14 +26,27 @@
 
     @patch.object(Metadata, 'session_id', PropertyMock(return_value='unique_session_id'))
     def test_app_automate_get_debug_url(self):
         self.app_automate.set_debug_url({'deviceName': 'Google Pixel 4', 'osVersion': '12.0', 'buildHash': 'abc', 'sessionHash': 'def'})
         debug_url = self.app_automate.get_debug_url()
         self.assertEqual(debug_url, 'https://app-automate.browserstack.com/dashboard/v2/builds/abc/sessions/def')
 
+    def test_app_automate_supports_with_correct_url(self):
+        app_automate_session = self.app_automate.supports('https://hub-cloud.browserstack.com/wd/hub')
+        self.assertEqual(app_automate_session, True)
+
+    def test_app_automate_supports_with_incorrect_url(self):
+        app_automate_session = self.app_automate.supports('https://hub-cloud.generic.com/wd/hub')
+        self.assertEqual(app_automate_session, False)
+
+    @patch.dict(os.environ, {"AA_DOMAIN": "bsstag"})
+    def test_app_automate_supports_with_AA_DOMAIN(self):
+        app_automate_session = self.app_automate.supports('bsstag.com')
+        self.assertEqual(app_automate_session, True)
+
     @patch('percy.providers.app_automate.log')
     def test_app_automate_execute_percy_screenshot_begin(self, _mocked_log):
         self.mock_webdriver.execute_script.return_value = {}
         self.assertIsNone(self.app_automate.execute_percy_screenshot_begin('Screebshot 1'))
         self.mock_webdriver.execute_script.assert_called()
 
     def test_app_automate_execute_percy_screenshot_end(self):
```

### Comparing `percy-appium-app-1.2.0/tests/test_app_percy.py` & `percy-appium-app-1.2.1/tests/test_app_percy.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.2.0/tests/test_cache.py` & `percy-appium-app-1.2.1/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.2.0/tests/test_cli_wrapper.py` & `percy-appium-app-1.2.1/tests/test_cli_wrapper.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.2.0/tests/test_generic_provider.py` & `percy-appium-app-1.2.1/tests/test_generic_provider.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.2.0/tests/test_ignore_region.py` & `percy-appium-app-1.2.1/tests/test_ignore_region.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.2.0/tests/test_ios_metadata.py` & `percy-appium-app-1.2.1/tests/test_ios_metadata.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.2.0/tests/test_metadata.py` & `percy-appium-app-1.2.1/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.2.0/tests/test_metadata_resolver.py` & `percy-appium-app-1.2.1/tests/test_metadata_resolver.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.2.0/tests/test_percy_options.py` & `percy-appium-app-1.2.1/tests/test_percy_options.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.2.0/tests/test_screenshot.py` & `percy-appium-app-1.2.1/tests/test_screenshot.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.2.0/tests/test_tile.py` & `percy-appium-app-1.2.1/tests/test_tile.py`

 * *Files identical despite different names*

