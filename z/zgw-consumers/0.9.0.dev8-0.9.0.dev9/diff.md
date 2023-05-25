# Comparing `tmp/zgw-consumers-0.9.0.dev8.tar.gz` & `tmp/zgw-consumers-0.9.0.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/zgw-consumers-0.9.0.dev8.tar", last modified: Wed Apr 15 08:33:29 2020, max compression
+gzip compressed data, was "dist/zgw-consumers-0.9.0.dev9.tar", last modified: Thu Apr 30 11:39:55 2020, max compression
```

## Comparing `zgw-consumers-0.9.0.dev8.tar` & `zgw-consumers-0.9.0.dev9.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 bbt       (1000) users      (100)        0 2020-04-15 08:33:29.000000 zgw-consumers-0.9.0.dev8/
--rw-r--r--   0 bbt       (1000) users      (100)     1061 2020-04-01 07:30:51.000000 zgw-consumers-0.9.0.dev8/LICENSE
--rw-r--r--   0 bbt       (1000) users      (100)      196 2020-04-01 07:30:51.000000 zgw-consumers-0.9.0.dev8/MANIFEST.in
--rw-r--r--   0 bbt       (1000) users      (100)     3310 2020-04-15 08:33:29.000000 zgw-consumers-0.9.0.dev8/PKG-INFO
--rw-r--r--   0 bbt       (1000) users      (100)     1733 2020-04-01 13:15:26.000000 zgw-consumers-0.9.0.dev8/README.rst
--rw-r--r--   0 bbt       (1000) users      (100)     1782 2020-04-15 08:33:29.000000 zgw-consumers-0.9.0.dev8/setup.cfg
--rw-r--r--   0 bbt       (1000) users      (100)       38 2020-04-01 07:30:51.000000 zgw-consumers-0.9.0.dev8/setup.py
-drwxr-xr-x   0 bbt       (1000) users      (100)        0 2020-04-15 08:33:29.000000 zgw-consumers-0.9.0.dev8/testapp/
--rw-r--r--   0 bbt       (1000) users      (100)        0 2020-04-01 07:30:51.000000 zgw-consumers-0.9.0.dev8/testapp/__init__.py
--rw-r--r--   0 bbt       (1000) users      (100)     1370 2020-04-01 09:51:41.000000 zgw-consumers-0.9.0.dev8/testapp/settings.py
--rw-r--r--   0 bbt       (1000) users      (100)      111 2020-04-01 07:30:51.000000 zgw-consumers-0.9.0.dev8/testapp/urls.py
-drwxr-xr-x   0 bbt       (1000) users      (100)        0 2020-04-15 08:33:29.000000 zgw-consumers-0.9.0.dev8/tests/
--rw-r--r--   0 bbt       (1000) users      (100)        0 2020-04-01 07:30:51.000000 zgw-consumers-0.9.0.dev8/tests/__init__.py
--rw-r--r--   0 bbt       (1000) users      (100)       84 2020-04-01 07:30:51.000000 zgw-consumers-0.9.0.dev8/tests/conftest.py
-drwxr-xr-x   0 bbt       (1000) users      (100)        0 2020-04-15 08:33:29.000000 zgw-consumers-0.9.0.dev8/zgw_consumers/
--rw-r--r--   0 bbt       (1000) users      (100)       61 2020-04-01 07:30:51.000000 zgw-consumers-0.9.0.dev8/zgw_consumers/__init__.py
--rw-r--r--   0 bbt       (1000) users      (100)      642 2020-04-01 08:27:59.000000 zgw-consumers-0.9.0.dev8/zgw_consumers/admin.py
--rw-r--r--   0 bbt       (1000) users      (100)     2132 2020-04-08 09:17:34.000000 zgw-consumers-0.9.0.dev8/zgw_consumers/admin_fields.py
-drwxr-xr-x   0 bbt       (1000) users      (100)        0 2020-04-15 08:33:29.000000 zgw-consumers-0.9.0.dev8/zgw_consumers/api_models/
--rw-r--r--   0 bbt       (1000) users      (100)        0 2020-04-01 13:15:26.000000 zgw-consumers-0.9.0.dev8/zgw_consumers/api_models/__init__.py
--rw-r--r--   0 bbt       (1000) users      (100)     3136 2020-04-01 13:15:26.000000 zgw-consumers-0.9.0.dev8/zgw_consumers/api_models/_camel_case.py
--rw-r--r--   0 bbt       (1000) users      (100)     2931 2020-04-01 13:15:26.000000 zgw-consumers-0.9.0.dev8/zgw_consumers/api_models/base.py
--rw-r--r--   0 bbt       (1000) users      (100)     3339 2020-04-14 10:33:43.000000 zgw-consumers-0.9.0.dev8/zgw_consumers/api_models/catalogi.py
--rw-r--r--   0 bbt       (1000) users      (100)      629 2020-04-01 13:15:26.000000 zgw-consumers-0.9.0.dev8/zgw_consumers/api_models/constants.py
--rw-r--r--   0 bbt       (1000) users      (100)      835 2020-04-01 13:15:26.000000 zgw-consumers-0.9.0.dev8/zgw_consumers/api_models/documenten.py
--rw-r--r--   0 bbt       (1000) users      (100)      596 2020-04-01 13:15:26.000000 zgw-consumers-0.9.0.dev8/zgw_consumers/api_models/selectielijst.py
--rw-r--r--   0 bbt       (1000) users      (100)      183 2020-04-01 13:15:26.000000 zgw-consumers-0.9.0.dev8/zgw_consumers/api_models/types.py
--rw-r--r--   0 bbt       (1000) users      (100)     1616 2020-04-15 08:14:37.000000 zgw-consumers-0.9.0.dev8/zgw_consumers/api_models/zaken.py
--rw-r--r--   0 bbt       (1000) users      (100)      100 2020-04-01 07:30:51.000000 zgw-consumers-0.9.0.dev8/zgw_consumers/apps.py
--rw-r--r--   0 bbt       (1000) users      (100)     1398 2020-04-01 08:27:59.000000 zgw-consumers-0.9.0.dev8/zgw_consumers/client.py
--rw-r--r--   0 bbt       (1000) users      (100)      756 2020-04-01 08:27:59.000000 zgw-consumers-0.9.0.dev8/zgw_consumers/constants.py
--rw-r--r--   0 bbt       (1000) users      (100)      747 2020-04-08 09:58:57.000000 zgw-consumers-0.9.0.dev8/zgw_consumers/fields.py
-drwxr-xr-x   0 bbt       (1000) users      (100)        0 2020-04-15 08:33:29.000000 zgw-consumers-0.9.0.dev8/zgw_consumers/migrations/
--rw-r--r--   0 bbt       (1000) users      (100)     2184 2020-04-01 07:30:51.000000 zgw-consumers-0.9.0.dev8/zgw_consumers/migrations/0001_initial.py
--rw-r--r--   0 bbt       (1000) users      (100)      614 2020-04-01 07:30:51.000000 zgw-consumers-0.9.0.dev8/zgw_consumers/migrations/0002_auto_20190514_0944.py
--rw-r--r--   0 bbt       (1000) users      (100)      838 2020-04-01 07:30:51.000000 zgw-consumers-0.9.0.dev8/zgw_consumers/migrations/0003_auto_20190514_1009.py
--rw-r--r--   0 bbt       (1000) users      (100)      909 2020-04-01 07:30:51.000000 zgw-consumers-0.9.0.dev8/zgw_consumers/migrations/0004_auto_20200113_1728.py
--rw-r--r--   0 bbt       (1000) users      (100)     1469 2020-04-01 08:27:59.000000 zgw-consumers-0.9.0.dev8/zgw_consumers/migrations/0005_auto_20200326_1040.py
--rw-r--r--   0 bbt       (1000) users      (100)      517 2020-04-01 08:27:59.000000 zgw-consumers-0.9.0.dev8/zgw_consumers/migrations/0006_update_oas_auth.py
--rw-r--r--   0 bbt       (1000) users      (100)      532 2020-04-01 08:27:59.000000 zgw-consumers-0.9.0.dev8/zgw_consumers/migrations/0007_service_nlx.py
--rw-r--r--   0 bbt       (1000) users      (100)     1237 2020-04-01 08:27:59.000000 zgw-consumers-0.9.0.dev8/zgw_consumers/migrations/0008_auto_20200331_1400.py
--rw-r--r--   0 bbt       (1000) users      (100)     1013 2020-04-01 13:15:45.000000 zgw-consumers-0.9.0.dev8/zgw_consumers/migrations/0009_auto_20200401_0829.py
--rw-r--r--   0 bbt       (1000) users      (100)        0 2020-04-01 07:30:51.000000 zgw-consumers-0.9.0.dev8/zgw_consumers/migrations/__init__.py
--rw-r--r--   0 bbt       (1000) users      (100)     5813 2020-04-01 13:15:46.000000 zgw-consumers-0.9.0.dev8/zgw_consumers/models.py
--rw-r--r--   0 bbt       (1000) users      (100)     3710 2020-04-01 09:51:41.000000 zgw-consumers-0.9.0.dev8/zgw_consumers/nlx.py
--rw-r--r--   0 bbt       (1000) users      (100)     1114 2020-04-01 13:15:26.000000 zgw-consumers-0.9.0.dev8/zgw_consumers/query.py
--rw-r--r--   0 bbt       (1000) users      (100)     2288 2020-04-10 14:48:54.000000 zgw-consumers-0.9.0.dev8/zgw_consumers/service.py
-drwxr-xr-x   0 bbt       (1000) users      (100)        0 2020-04-15 08:33:29.000000 zgw-consumers-0.9.0.dev8/zgw_consumers.egg-info/
--rw-r--r--   0 bbt       (1000) users      (100)     3310 2020-04-15 08:33:28.000000 zgw-consumers-0.9.0.dev8/zgw_consumers.egg-info/PKG-INFO
--rw-r--r--   0 bbt       (1000) users      (100)     1448 2020-04-15 08:33:28.000000 zgw-consumers-0.9.0.dev8/zgw_consumers.egg-info/SOURCES.txt
--rw-r--r--   0 bbt       (1000) users      (100)        1 2020-04-15 08:33:28.000000 zgw-consumers-0.9.0.dev8/zgw_consumers.egg-info/dependency_links.txt
--rw-r--r--   0 bbt       (1000) users      (100)        1 2019-05-14 07:31:52.000000 zgw-consumers-0.9.0.dev8/zgw_consumers.egg-info/not-zip-safe
--rw-r--r--   0 bbt       (1000) users      (100)      236 2020-04-15 08:33:28.000000 zgw-consumers-0.9.0.dev8/zgw_consumers.egg-info/requires.txt
--rw-r--r--   0 bbt       (1000) users      (100)       14 2020-04-15 08:33:28.000000 zgw-consumers-0.9.0.dev8/zgw_consumers.egg-info/top_level.txt
+drwxr-xr-x   0 bbt       (1000) users      (100)        0 2020-04-30 11:39:55.000000 zgw-consumers-0.9.0.dev9/
+-rw-r--r--   0 bbt       (1000) users      (100)     1061 2020-04-01 07:30:51.000000 zgw-consumers-0.9.0.dev9/LICENSE
+-rw-r--r--   0 bbt       (1000) users      (100)      196 2020-04-01 07:30:51.000000 zgw-consumers-0.9.0.dev9/MANIFEST.in
+-rw-r--r--   0 bbt       (1000) users      (100)     3310 2020-04-30 11:39:55.000000 zgw-consumers-0.9.0.dev9/PKG-INFO
+-rw-r--r--   0 bbt       (1000) users      (100)     1733 2020-04-30 11:30:37.000000 zgw-consumers-0.9.0.dev9/README.rst
+-rw-r--r--   0 bbt       (1000) users      (100)     1782 2020-04-30 11:39:55.000000 zgw-consumers-0.9.0.dev9/setup.cfg
+-rw-r--r--   0 bbt       (1000) users      (100)       38 2020-04-01 07:30:51.000000 zgw-consumers-0.9.0.dev9/setup.py
+drwxr-xr-x   0 bbt       (1000) users      (100)        0 2020-04-30 11:39:55.000000 zgw-consumers-0.9.0.dev9/testapp/
+-rw-r--r--   0 bbt       (1000) users      (100)        0 2020-04-01 07:30:51.000000 zgw-consumers-0.9.0.dev9/testapp/__init__.py
+-rw-r--r--   0 bbt       (1000) users      (100)     1370 2020-04-01 09:51:41.000000 zgw-consumers-0.9.0.dev9/testapp/settings.py
+-rw-r--r--   0 bbt       (1000) users      (100)      111 2020-04-01 07:30:51.000000 zgw-consumers-0.9.0.dev9/testapp/urls.py
+drwxr-xr-x   0 bbt       (1000) users      (100)        0 2020-04-30 11:39:55.000000 zgw-consumers-0.9.0.dev9/tests/
+-rw-r--r--   0 bbt       (1000) users      (100)        0 2020-04-01 07:30:51.000000 zgw-consumers-0.9.0.dev9/tests/__init__.py
+-rw-r--r--   0 bbt       (1000) users      (100)       84 2020-04-01 07:30:51.000000 zgw-consumers-0.9.0.dev9/tests/conftest.py
+drwxr-xr-x   0 bbt       (1000) users      (100)        0 2020-04-30 11:39:55.000000 zgw-consumers-0.9.0.dev9/zgw_consumers/
+-rw-r--r--   0 bbt       (1000) users      (100)       61 2020-04-01 07:30:51.000000 zgw-consumers-0.9.0.dev9/zgw_consumers/__init__.py
+-rw-r--r--   0 bbt       (1000) users      (100)      642 2020-04-01 08:27:59.000000 zgw-consumers-0.9.0.dev9/zgw_consumers/admin.py
+-rw-r--r--   0 bbt       (1000) users      (100)     2132 2020-04-08 09:17:34.000000 zgw-consumers-0.9.0.dev9/zgw_consumers/admin_fields.py
+drwxr-xr-x   0 bbt       (1000) users      (100)        0 2020-04-30 11:39:55.000000 zgw-consumers-0.9.0.dev9/zgw_consumers/api_models/
+-rw-r--r--   0 bbt       (1000) users      (100)        0 2020-04-01 13:15:26.000000 zgw-consumers-0.9.0.dev9/zgw_consumers/api_models/__init__.py
+-rw-r--r--   0 bbt       (1000) users      (100)     3136 2020-04-01 13:15:26.000000 zgw-consumers-0.9.0.dev9/zgw_consumers/api_models/_camel_case.py
+-rw-r--r--   0 bbt       (1000) users      (100)     2931 2020-04-01 13:15:26.000000 zgw-consumers-0.9.0.dev9/zgw_consumers/api_models/base.py
+-rw-r--r--   0 bbt       (1000) users      (100)     3412 2020-04-30 11:20:58.000000 zgw-consumers-0.9.0.dev9/zgw_consumers/api_models/catalogi.py
+-rw-r--r--   0 bbt       (1000) users      (100)     2522 2020-04-30 11:20:58.000000 zgw-consumers-0.9.0.dev9/zgw_consumers/api_models/constants.py
+-rw-r--r--   0 bbt       (1000) users      (100)      835 2020-04-01 13:15:26.000000 zgw-consumers-0.9.0.dev9/zgw_consumers/api_models/documenten.py
+-rw-r--r--   0 bbt       (1000) users      (100)      596 2020-04-01 13:15:26.000000 zgw-consumers-0.9.0.dev9/zgw_consumers/api_models/selectielijst.py
+-rw-r--r--   0 bbt       (1000) users      (100)      183 2020-04-01 13:15:26.000000 zgw-consumers-0.9.0.dev9/zgw_consumers/api_models/types.py
+-rw-r--r--   0 bbt       (1000) users      (100)     2162 2020-04-30 11:20:58.000000 zgw-consumers-0.9.0.dev9/zgw_consumers/api_models/zaken.py
+-rw-r--r--   0 bbt       (1000) users      (100)      100 2020-04-01 07:30:51.000000 zgw-consumers-0.9.0.dev9/zgw_consumers/apps.py
+-rw-r--r--   0 bbt       (1000) users      (100)     1398 2020-04-01 08:27:59.000000 zgw-consumers-0.9.0.dev9/zgw_consumers/client.py
+-rw-r--r--   0 bbt       (1000) users      (100)      756 2020-04-01 08:27:59.000000 zgw-consumers-0.9.0.dev9/zgw_consumers/constants.py
+-rw-r--r--   0 bbt       (1000) users      (100)      747 2020-04-08 09:58:57.000000 zgw-consumers-0.9.0.dev9/zgw_consumers/fields.py
+drwxr-xr-x   0 bbt       (1000) users      (100)        0 2020-04-30 11:39:55.000000 zgw-consumers-0.9.0.dev9/zgw_consumers/migrations/
+-rw-r--r--   0 bbt       (1000) users      (100)     2184 2020-04-01 07:30:51.000000 zgw-consumers-0.9.0.dev9/zgw_consumers/migrations/0001_initial.py
+-rw-r--r--   0 bbt       (1000) users      (100)      614 2020-04-01 07:30:51.000000 zgw-consumers-0.9.0.dev9/zgw_consumers/migrations/0002_auto_20190514_0944.py
+-rw-r--r--   0 bbt       (1000) users      (100)      838 2020-04-01 07:30:51.000000 zgw-consumers-0.9.0.dev9/zgw_consumers/migrations/0003_auto_20190514_1009.py
+-rw-r--r--   0 bbt       (1000) users      (100)      909 2020-04-01 07:30:51.000000 zgw-consumers-0.9.0.dev9/zgw_consumers/migrations/0004_auto_20200113_1728.py
+-rw-r--r--   0 bbt       (1000) users      (100)     1469 2020-04-01 08:27:59.000000 zgw-consumers-0.9.0.dev9/zgw_consumers/migrations/0005_auto_20200326_1040.py
+-rw-r--r--   0 bbt       (1000) users      (100)      517 2020-04-01 08:27:59.000000 zgw-consumers-0.9.0.dev9/zgw_consumers/migrations/0006_update_oas_auth.py
+-rw-r--r--   0 bbt       (1000) users      (100)      532 2020-04-01 08:27:59.000000 zgw-consumers-0.9.0.dev9/zgw_consumers/migrations/0007_service_nlx.py
+-rw-r--r--   0 bbt       (1000) users      (100)     1237 2020-04-01 08:27:59.000000 zgw-consumers-0.9.0.dev9/zgw_consumers/migrations/0008_auto_20200331_1400.py
+-rw-r--r--   0 bbt       (1000) users      (100)     1013 2020-04-01 13:15:45.000000 zgw-consumers-0.9.0.dev9/zgw_consumers/migrations/0009_auto_20200401_0829.py
+-rw-r--r--   0 bbt       (1000) users      (100)        0 2020-04-01 07:30:51.000000 zgw-consumers-0.9.0.dev9/zgw_consumers/migrations/__init__.py
+-rw-r--r--   0 bbt       (1000) users      (100)     5813 2020-04-01 13:15:46.000000 zgw-consumers-0.9.0.dev9/zgw_consumers/models.py
+-rw-r--r--   0 bbt       (1000) users      (100)     3710 2020-04-01 09:51:41.000000 zgw-consumers-0.9.0.dev9/zgw_consumers/nlx.py
+-rw-r--r--   0 bbt       (1000) users      (100)     1114 2020-04-01 13:15:26.000000 zgw-consumers-0.9.0.dev9/zgw_consumers/query.py
+-rw-r--r--   0 bbt       (1000) users      (100)     2587 2020-04-29 14:03:00.000000 zgw-consumers-0.9.0.dev9/zgw_consumers/service.py
+drwxr-xr-x   0 bbt       (1000) users      (100)        0 2020-04-30 11:39:55.000000 zgw-consumers-0.9.0.dev9/zgw_consumers.egg-info/
+-rw-r--r--   0 bbt       (1000) users      (100)     3310 2020-04-30 11:39:55.000000 zgw-consumers-0.9.0.dev9/zgw_consumers.egg-info/PKG-INFO
+-rw-r--r--   0 bbt       (1000) users      (100)     1448 2020-04-30 11:39:55.000000 zgw-consumers-0.9.0.dev9/zgw_consumers.egg-info/SOURCES.txt
+-rw-r--r--   0 bbt       (1000) users      (100)        1 2020-04-30 11:39:55.000000 zgw-consumers-0.9.0.dev9/zgw_consumers.egg-info/dependency_links.txt
+-rw-r--r--   0 bbt       (1000) users      (100)        1 2019-05-14 07:31:52.000000 zgw-consumers-0.9.0.dev9/zgw_consumers.egg-info/not-zip-safe
+-rw-r--r--   0 bbt       (1000) users      (100)      236 2020-04-30 11:39:55.000000 zgw-consumers-0.9.0.dev9/zgw_consumers.egg-info/requires.txt
+-rw-r--r--   0 bbt       (1000) users      (100)       14 2020-04-30 11:39:55.000000 zgw-consumers-0.9.0.dev9/zgw_consumers.egg-info/top_level.txt
```

### Comparing `zgw-consumers-0.9.0.dev8/LICENSE` & `zgw-consumers-0.9.0.dev9/LICENSE`

 * *Files identical despite different names*

### Comparing `zgw-consumers-0.9.0.dev8/PKG-INFO` & `zgw-consumers-0.9.0.dev9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: zgw-consumers
-Version: 0.9.0.dev8
+Version: 0.9.0.dev9
 Summary: Reusable code for consumers of ZGW APIs
 Home-page: https://github.com/maykinmedia/zgw_consumers
 Author: Maykin Media
 Author-email: support@maykinmedia.nl
 License: MIT
 Description: 
         
         .. zgw_consumers documentation master file, created by startproject.
            You can adapt this file completely to your liking, but it should at least
            contain the root `toctree` directive.
         
         Welcome to zgw_consumers's documentation!
         =================================================
         
-        :Version: 0.6.0.dev2
+        :Version: 0.9.0.dev9
         :Source: https://github.com/maykinmedia/zgw_consumers
         :Keywords: ``<keywords>``
         :PythonVersion: 3.6
         
         |build-status| |requirements| |coverage|
         
         |python-versions| |django-versions| |pypi-version|
```

### Comparing `zgw-consumers-0.9.0.dev8/README.rst` & `zgw-consumers-0.9.0.dev9/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 .. zgw_consumers documentation master file, created by startproject.
    You can adapt this file completely to your liking, but it should at least
    contain the root `toctree` directive.
 
 Welcome to zgw_consumers's documentation!
 =================================================
 
-:Version: 0.6.0.dev2
+:Version: 0.9.0.dev9
 :Source: https://github.com/maykinmedia/zgw_consumers
 :Keywords: ``<keywords>``
 :PythonVersion: 3.6
 
 |build-status| |requirements| |coverage|
 
 |python-versions| |django-versions| |pypi-version|
```

### Comparing `zgw-consumers-0.9.0.dev8/setup.cfg` & `zgw-consumers-0.9.0.dev9/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = zgw-consumers
-version = 0.9.0.dev8
+version = 0.9.0.dev9
 description = Reusable code for consumers of ZGW APIs
 long_description = file: README.rst
 url = https://github.com/maykinmedia/zgw_consumers
 license = MIT
 author = Maykin Media
 author_email = support@maykinmedia.nl
 keywords = ZGW, Common Ground, GEMMA, VNG, API
```

### Comparing `zgw-consumers-0.9.0.dev8/testapp/settings.py` & `zgw-consumers-0.9.0.dev9/testapp/settings.py`

 * *Files identical despite different names*

### Comparing `zgw-consumers-0.9.0.dev8/zgw_consumers/admin.py` & `zgw-consumers-0.9.0.dev9/zgw_consumers/admin.py`

 * *Files identical despite different names*

### Comparing `zgw-consumers-0.9.0.dev8/zgw_consumers/admin_fields.py` & `zgw-consumers-0.9.0.dev9/zgw_consumers/admin_fields.py`

 * *Files identical despite different names*

### Comparing `zgw-consumers-0.9.0.dev8/zgw_consumers/api_models/_camel_case.py` & `zgw-consumers-0.9.0.dev9/zgw_consumers/api_models/_camel_case.py`

 * *Files identical despite different names*

### Comparing `zgw-consumers-0.9.0.dev8/zgw_consumers/api_models/base.py` & `zgw-consumers-0.9.0.dev9/zgw_consumers/api_models/base.py`

 * *Files identical despite different names*

### Comparing `zgw-consumers-0.9.0.dev8/zgw_consumers/api_models/catalogi.py` & `zgw-consumers-0.9.0.dev9/zgw_consumers/api_models/catalogi.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from decimal import Decimal
 from typing import Optional, Union
 
 from dateutil.parser import parse
 from dateutil.relativedelta import relativedelta
 
 from .base import Model, ZGWModel, factory
-from .selectielijst import ProcesType, Resultaat
 
 
 @dataclass
 class Catalogus(ZGWModel):
     url: str
     domein: str
     rsin: str
@@ -134,7 +133,15 @@
         Cast the string value into the appropriate python type based on the spec.
         """
         formaat = self.specificatie.formaat
         assert formaat in EIGENSCHAP_FORMATEN, f"Unknown format {formaat}"
 
         converter = EIGENSCHAP_FORMATEN[formaat]
         return converter(value)
+
+
+@dataclass
+class RolType(ZGWModel):
+    url: str
+    zaaktype: str
+    omschrijving: str
+    omschrijving_generiek: str
```

### Comparing `zgw-consumers-0.9.0.dev8/zgw_consumers/api_models/documenten.py` & `zgw-consumers-0.9.0.dev9/zgw_consumers/api_models/documenten.py`

 * *Files identical despite different names*

### Comparing `zgw-consumers-0.9.0.dev8/zgw_consumers/api_models/selectielijst.py` & `zgw-consumers-0.9.0.dev9/zgw_consumers/api_models/selectielijst.py`

 * *Files identical despite different names*

### Comparing `zgw-consumers-0.9.0.dev8/zgw_consumers/api_models/zaken.py` & `zgw-consumers-0.9.0.dev9/zgw_consumers/api_models/zaken.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from dataclasses import dataclass
 from datetime import date, datetime
 from typing import Any, Optional
 
 from .base import ZGWModel
 from .catalogi import Eigenschap
-from .constants import VertrouwelijkheidsAanduidingen
+from .constants import RolOmschrijving, RolTypes, VertrouwelijkheidsAanduidingen
 
 
 @dataclass
 class Zaak(ZGWModel):
     url: str
     identificatie: str
     bronorganisatie: str
@@ -68,7 +68,28 @@
 
 @dataclass
 class Resultaat(ZGWModel):
     url: str
     zaak: str
     resultaattype: str
     toelichting: str
+
+
+@dataclass
+class Rol(ZGWModel):
+    url: str
+    zaak: str
+    betrokkene: str
+    betrokkene_type: str
+    roltype: str
+    omschrijving: str
+    omschrijving_generiek: str
+    roltoelichting: str
+    registratiedatum: datetime
+    indicatie_machtiging: str
+    betrokkene_identificatie: Optional[dict]
+
+    def get_betrokkene_type_display(self):
+        return RolTypes.values[self.betrokkene_type]
+
+    def get_omschrijving_generiek_display(self):
+        return RolOmschrijving.values[self.omschrijving_generiek]
```

### Comparing `zgw-consumers-0.9.0.dev8/zgw_consumers/client.py` & `zgw-consumers-0.9.0.dev9/zgw_consumers/client.py`

 * *Files identical despite different names*

### Comparing `zgw-consumers-0.9.0.dev8/zgw_consumers/constants.py` & `zgw-consumers-0.9.0.dev9/zgw_consumers/constants.py`

 * *Files identical despite different names*

### Comparing `zgw-consumers-0.9.0.dev8/zgw_consumers/fields.py` & `zgw-consumers-0.9.0.dev9/zgw_consumers/fields.py`

 * *Files identical despite different names*

### Comparing `zgw-consumers-0.9.0.dev8/zgw_consumers/migrations/0001_initial.py` & `zgw-consumers-0.9.0.dev9/zgw_consumers/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `zgw-consumers-0.9.0.dev8/zgw_consumers/migrations/0002_auto_20190514_0944.py` & `zgw-consumers-0.9.0.dev9/zgw_consumers/migrations/0002_auto_20190514_0944.py`

 * *Files identical despite different names*

### Comparing `zgw-consumers-0.9.0.dev8/zgw_consumers/migrations/0003_auto_20190514_1009.py` & `zgw-consumers-0.9.0.dev9/zgw_consumers/migrations/0003_auto_20190514_1009.py`

 * *Files identical despite different names*

### Comparing `zgw-consumers-0.9.0.dev8/zgw_consumers/migrations/0004_auto_20200113_1728.py` & `zgw-consumers-0.9.0.dev9/zgw_consumers/migrations/0004_auto_20200113_1728.py`

 * *Files identical despite different names*

### Comparing `zgw-consumers-0.9.0.dev8/zgw_consumers/migrations/0005_auto_20200326_1040.py` & `zgw-consumers-0.9.0.dev9/zgw_consumers/migrations/0005_auto_20200326_1040.py`

 * *Files identical despite different names*

### Comparing `zgw-consumers-0.9.0.dev8/zgw_consumers/migrations/0006_update_oas_auth.py` & `zgw-consumers-0.9.0.dev9/zgw_consumers/migrations/0006_update_oas_auth.py`

 * *Files identical despite different names*

### Comparing `zgw-consumers-0.9.0.dev8/zgw_consumers/migrations/0007_service_nlx.py` & `zgw-consumers-0.9.0.dev9/zgw_consumers/migrations/0007_service_nlx.py`

 * *Files identical despite different names*

### Comparing `zgw-consumers-0.9.0.dev8/zgw_consumers/migrations/0008_auto_20200331_1400.py` & `zgw-consumers-0.9.0.dev9/zgw_consumers/migrations/0008_auto_20200331_1400.py`

 * *Files identical despite different names*

### Comparing `zgw-consumers-0.9.0.dev8/zgw_consumers/migrations/0009_auto_20200401_0829.py` & `zgw-consumers-0.9.0.dev9/zgw_consumers/migrations/0009_auto_20200401_0829.py`

 * *Files identical despite different names*

### Comparing `zgw-consumers-0.9.0.dev8/zgw_consumers/models.py` & `zgw-consumers-0.9.0.dev9/zgw_consumers/models.py`

 * *Files identical despite different names*

### Comparing `zgw-consumers-0.9.0.dev8/zgw_consumers/nlx.py` & `zgw-consumers-0.9.0.dev9/zgw_consumers/nlx.py`

 * *Files identical despite different names*

### Comparing `zgw-consumers-0.9.0.dev8/zgw_consumers/query.py` & `zgw-consumers-0.9.0.dev9/zgw_consumers/query.py`

 * *Files identical despite different names*

### Comparing `zgw-consumers-0.9.0.dev8/zgw_consumers/service.py` & `zgw-consumers-0.9.0.dev9/zgw_consumers/service.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,50 @@
 from concurrent import futures
-from typing import List, Type
+from typing import List, Optional, Type
 from urllib.parse import parse_qs, urlparse
 
 from .api_models.base import ZGWModel, factory
 from .api_models.catalogi import Catalogus, InformatieObjectType
 from .client import Client
 from .constants import APITypes
 from .models import Service
 
 
-def get_paginated_results(client, resource: str, minimum=None, *args, **kwargs) -> list:
+def get_paginated_results(
+    client: Client,
+    resource: str,
+    minimum: Optional[int] = None,
+    test_func: Optional[callable] = None,
+    *args,
+    **kwargs
+) -> list:
     query_params = kwargs.get("query_params", {})
 
     results = []
     response = client.list(resource, *args, **kwargs)
 
-    results += response["results"]
+    def _get_results(response):
+        _results = response["results"]
+        if test_func:
+            _results = [result for result in _results if test_func(result)]
+        return _results
+
+    results += _get_results(response)
 
     if minimum and len(results) >= minimum:
         return results
 
     while response["next"]:
         next_url = urlparse(response["next"])
         query = parse_qs(next_url.query)
         new_page = int(query["page"][0])
         query_params["page"] = [new_page]
         kwargs["query_params"] = query_params
         response = client.list(resource, *args, **kwargs)
-        results += response["results"]
+        results += _get_results(response)
 
         if minimum and len(results) >= minimum:
             return results
 
     return results
```

### Comparing `zgw-consumers-0.9.0.dev8/zgw_consumers.egg-info/PKG-INFO` & `zgw-consumers-0.9.0.dev9/zgw_consumers.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: zgw-consumers
-Version: 0.9.0.dev8
+Version: 0.9.0.dev9
 Summary: Reusable code for consumers of ZGW APIs
 Home-page: https://github.com/maykinmedia/zgw_consumers
 Author: Maykin Media
 Author-email: support@maykinmedia.nl
 License: MIT
 Description: 
         
         .. zgw_consumers documentation master file, created by startproject.
            You can adapt this file completely to your liking, but it should at least
            contain the root `toctree` directive.
         
         Welcome to zgw_consumers's documentation!
         =================================================
         
-        :Version: 0.6.0.dev2
+        :Version: 0.9.0.dev9
         :Source: https://github.com/maykinmedia/zgw_consumers
         :Keywords: ``<keywords>``
         :PythonVersion: 3.6
         
         |build-status| |requirements| |coverage|
         
         |python-versions| |django-versions| |pypi-version|
```

### Comparing `zgw-consumers-0.9.0.dev8/zgw_consumers.egg-info/SOURCES.txt` & `zgw-consumers-0.9.0.dev9/zgw_consumers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

