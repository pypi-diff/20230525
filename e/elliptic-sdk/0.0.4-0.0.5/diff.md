# Comparing `tmp/elliptic_sdk-0.0.4.tar.gz` & `tmp/elliptic_sdk-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elliptic_sdk-0.0.4.tar", max compression
+gzip compressed data, was "elliptic_sdk-0.0.5.tar", max compression
```

## Comparing `elliptic_sdk-0.0.4.tar` & `elliptic_sdk-0.0.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1075 2023-04-19 13:23:40.198775 elliptic_sdk-0.0.4/LICENSE
--rw-r--r--   0        0        0       66 2023-04-30 16:15:34.229645 elliptic_sdk-0.0.4/elliptic_sdk/__init__.py
--rw-r--r--   0        0        0     1538 2023-04-30 16:15:34.230285 elliptic_sdk-0.0.4/elliptic_sdk/aml.py
--rw-r--r--   0        0        0     1947 2023-04-30 16:15:34.230389 elliptic_sdk-0.0.4/elliptic_sdk/auth.py
--rw-r--r--   0        0        0      329 2023-04-30 16:15:34.230482 elliptic_sdk-0.0.4/elliptic_sdk/client.py
--rw-r--r--   0        0        0      446 2023-04-30 16:15:34.230615 elliptic_sdk-0.0.4/elliptic_sdk/enums.py
--rw-r--r--   0        0        0     1766 2023-04-30 16:15:34.230754 elliptic_sdk-0.0.4/elliptic_sdk/schemas.py
--rw-r--r--   0        0        0      379 2023-04-30 16:15:34.230977 elliptic_sdk-0.0.4/elliptic_sdk/settings.py
--rw-r--r--   0        0        0      484 2023-04-30 16:15:50.386263 elliptic_sdk-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      449 1970-01-01 00:00:00.000000 elliptic_sdk-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-04-19 13:23:40.198775 elliptic_sdk-0.0.5/LICENSE
+-rw-r--r--   0        0        0       66 2023-04-30 16:15:34.229645 elliptic_sdk-0.0.5/elliptic_sdk/__init__.py
+-rw-r--r--   0        0        0     1538 2023-04-30 16:15:34.230285 elliptic_sdk-0.0.5/elliptic_sdk/aml.py
+-rw-r--r--   0        0        0     1947 2023-04-30 16:15:34.230389 elliptic_sdk-0.0.5/elliptic_sdk/auth.py
+-rw-r--r--   0        0        0      386 2023-05-25 11:15:52.060008 elliptic_sdk-0.0.5/elliptic_sdk/client.py
+-rw-r--r--   0        0        0      446 2023-04-30 16:15:34.230615 elliptic_sdk-0.0.5/elliptic_sdk/enums.py
+-rw-r--r--   0        0        0     1766 2023-04-30 16:15:34.230754 elliptic_sdk-0.0.5/elliptic_sdk/schemas.py
+-rw-r--r--   0        0        0      386 2023-05-25 11:15:52.060126 elliptic_sdk-0.0.5/elliptic_sdk/settings.py
+-rw-r--r--   0        0        0      484 2023-05-25 11:16:10.932465 elliptic_sdk-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      449 1970-01-01 00:00:00.000000 elliptic_sdk-0.0.5/PKG-INFO
```

### Comparing `elliptic_sdk-0.0.4/LICENSE` & `elliptic_sdk-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `elliptic_sdk-0.0.4/elliptic_sdk/aml.py` & `elliptic_sdk-0.0.5/elliptic_sdk/aml.py`

 * *Files identical despite different names*

### Comparing `elliptic_sdk-0.0.4/elliptic_sdk/auth.py` & `elliptic_sdk-0.0.5/elliptic_sdk/auth.py`

 * *Files identical despite different names*

### Comparing `elliptic_sdk-0.0.4/elliptic_sdk/schemas.py` & `elliptic_sdk-0.0.5/elliptic_sdk/schemas.py`

 * *Files identical despite different names*

