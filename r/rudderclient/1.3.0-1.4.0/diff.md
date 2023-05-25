# Comparing `tmp/rudderclient-1.3.0.tar.gz` & `tmp/rudderclient-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rudderclient-1.3.0.tar", last modified: Tue May 23 14:27:26 2023, max compression
+gzip compressed data, was "rudderclient-1.4.0.tar", last modified: Thu May 25 10:53:47 2023, max compression
```

## Comparing `rudderclient-1.3.0.tar` & `rudderclient-1.4.0.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxrwxr-x   0 soniaqg   (1001) soniaqg   (1001)        0 2023-05-23 14:27:26.646374 rudderclient-1.3.0/
--rw-rw-r--   0 soniaqg   (1001) soniaqg   (1001)     1069 2023-05-17 06:37:36.000000 rudderclient-1.3.0/LICENSE
--rw-rw-r--   0 soniaqg   (1001) soniaqg   (1001)     1968 2023-05-23 14:27:26.646374 rudderclient-1.3.0/PKG-INFO
--rw-rw-r--   0 soniaqg   (1001) soniaqg   (1001)      224 2023-05-22 12:05:46.000000 rudderclient-1.3.0/README.md
--rw-rw-r--   0 soniaqg   (1001) soniaqg   (1001)      681 2023-05-23 14:26:14.000000 rudderclient-1.3.0/pyproject.toml
--rw-rw-r--   0 soniaqg   (1001) soniaqg   (1001)       38 2023-05-23 14:27:26.646374 rudderclient-1.3.0/setup.cfg
-drwxrwxr-x   0 soniaqg   (1001) soniaqg   (1001)        0 2023-05-23 14:27:26.646374 rudderclient-1.3.0/src/
-drwxrwxr-x   0 soniaqg   (1001) soniaqg   (1001)        0 2023-05-23 14:27:26.646374 rudderclient-1.3.0/src/rudderclient/
-drwxrwxr-x   0 soniaqg   (1001) soniaqg   (1001)        0 2023-05-23 14:27:26.646374 rudderclient-1.3.0/src/rudderclient/gcp/
--rw-rw-r--   0 soniaqg   (1001) soniaqg   (1001)        0 2023-05-23 09:45:20.000000 rudderclient-1.3.0/src/rudderclient/gcp/__init__.py
--rw-rw-r--   0 soniaqg   (1001) soniaqg   (1001)     1256 2023-05-23 14:24:33.000000 rudderclient-1.3.0/src/rudderclient/gcp/auth.py
--rw-rw-r--   0 soniaqg   (1001) soniaqg   (1001)      381 2023-05-23 12:23:14.000000 rudderclient-1.3.0/src/rudderclient/gcp/http_requests.py
--rw-rw-r--   0 soniaqg   (1001) soniaqg   (1001)      448 2023-05-23 14:03:56.000000 rudderclient-1.3.0/src/rudderclient/gcp/pubsub.py
-drwxrwxr-x   0 soniaqg   (1001) soniaqg   (1001)        0 2023-05-23 14:27:26.646374 rudderclient-1.3.0/src/rudderclient/tools/
--rw-rw-r--   0 soniaqg   (1001) soniaqg   (1001)     5118 2023-05-23 09:45:20.000000 rudderclient-1.3.0/src/rudderclient/tools/send_account_email.py
-drwxrwxr-x   0 soniaqg   (1001) soniaqg   (1001)        0 2023-05-23 14:27:26.646374 rudderclient-1.3.0/src/rudderclient.egg-info/
--rw-rw-r--   0 soniaqg   (1001) soniaqg   (1001)     1968 2023-05-23 14:27:26.000000 rudderclient-1.3.0/src/rudderclient.egg-info/PKG-INFO
--rw-rw-r--   0 soniaqg   (1001) soniaqg   (1001)      407 2023-05-23 14:27:26.000000 rudderclient-1.3.0/src/rudderclient.egg-info/SOURCES.txt
--rw-rw-r--   0 soniaqg   (1001) soniaqg   (1001)        1 2023-05-23 14:27:26.000000 rudderclient-1.3.0/src/rudderclient.egg-info/dependency_links.txt
--rw-rw-r--   0 soniaqg   (1001) soniaqg   (1001)       28 2023-05-23 14:27:26.000000 rudderclient-1.3.0/src/rudderclient.egg-info/requires.txt
--rw-rw-r--   0 soniaqg   (1001) soniaqg   (1001)       13 2023-05-23 14:27:26.000000 rudderclient-1.3.0/src/rudderclient.egg-info/top_level.txt
+drwxrwxr-x   0 soniaqg   (1001) soniaqg   (1001)        0 2023-05-25 10:53:47.803764 rudderclient-1.4.0/
+-rw-rw-r--   0 soniaqg   (1001) soniaqg   (1001)     1069 2023-05-17 06:37:36.000000 rudderclient-1.4.0/LICENSE
+-rw-rw-r--   0 soniaqg   (1001) soniaqg   (1001)     1968 2023-05-25 10:53:47.803764 rudderclient-1.4.0/PKG-INFO
+-rw-rw-r--   0 soniaqg   (1001) soniaqg   (1001)      224 2023-05-22 12:05:46.000000 rudderclient-1.4.0/README.md
+-rw-rw-r--   0 soniaqg   (1001) soniaqg   (1001)      681 2023-05-25 10:53:06.000000 rudderclient-1.4.0/pyproject.toml
+-rw-rw-r--   0 soniaqg   (1001) soniaqg   (1001)       38 2023-05-25 10:53:47.803764 rudderclient-1.4.0/setup.cfg
+drwxrwxr-x   0 soniaqg   (1001) soniaqg   (1001)        0 2023-05-25 10:53:47.799764 rudderclient-1.4.0/src/
+drwxrwxr-x   0 soniaqg   (1001) soniaqg   (1001)        0 2023-05-25 10:53:47.799764 rudderclient-1.4.0/src/rudderclient/
+drwxrwxr-x   0 soniaqg   (1001) soniaqg   (1001)        0 2023-05-25 10:53:47.799764 rudderclient-1.4.0/src/rudderclient/aws/
+-rw-rw-r--   0 soniaqg   (1001) soniaqg   (1001)     1997 2023-05-25 09:52:05.000000 rudderclient-1.4.0/src/rudderclient/aws/requests.py
+drwxrwxr-x   0 soniaqg   (1001) soniaqg   (1001)        0 2023-05-25 10:53:47.799764 rudderclient-1.4.0/src/rudderclient/gcp/
+-rw-rw-r--   0 soniaqg   (1001) soniaqg   (1001)        0 2023-05-23 09:45:20.000000 rudderclient-1.4.0/src/rudderclient/gcp/__init__.py
+-rw-rw-r--   0 soniaqg   (1001) soniaqg   (1001)     1256 2023-05-25 09:35:18.000000 rudderclient-1.4.0/src/rudderclient/gcp/auth.py
+-rw-rw-r--   0 soniaqg   (1001) soniaqg   (1001)      381 2023-05-23 12:23:14.000000 rudderclient-1.4.0/src/rudderclient/gcp/http_requests.py
+-rw-rw-r--   0 soniaqg   (1001) soniaqg   (1001)      448 2023-05-25 09:35:18.000000 rudderclient-1.4.0/src/rudderclient/gcp/pubsub.py
+drwxrwxr-x   0 soniaqg   (1001) soniaqg   (1001)        0 2023-05-25 10:53:47.803764 rudderclient-1.4.0/src/rudderclient/tools/
+-rw-rw-r--   0 soniaqg   (1001) soniaqg   (1001)     5118 2023-05-23 09:45:20.000000 rudderclient-1.4.0/src/rudderclient/tools/send_account_email.py
+drwxrwxr-x   0 soniaqg   (1001) soniaqg   (1001)        0 2023-05-25 10:53:47.799764 rudderclient-1.4.0/src/rudderclient.egg-info/
+-rw-rw-r--   0 soniaqg   (1001) soniaqg   (1001)     1968 2023-05-25 10:53:47.000000 rudderclient-1.4.0/src/rudderclient.egg-info/PKG-INFO
+-rw-rw-r--   0 soniaqg   (1001) soniaqg   (1001)      440 2023-05-25 10:53:47.000000 rudderclient-1.4.0/src/rudderclient.egg-info/SOURCES.txt
+-rw-rw-r--   0 soniaqg   (1001) soniaqg   (1001)        1 2023-05-25 10:53:47.000000 rudderclient-1.4.0/src/rudderclient.egg-info/dependency_links.txt
+-rw-rw-r--   0 soniaqg   (1001) soniaqg   (1001)       28 2023-05-25 10:53:47.000000 rudderclient-1.4.0/src/rudderclient.egg-info/requires.txt
+-rw-rw-r--   0 soniaqg   (1001) soniaqg   (1001)       13 2023-05-25 10:53:47.000000 rudderclient-1.4.0/src/rudderclient.egg-info/top_level.txt
```

### Comparing `rudderclient-1.3.0/LICENSE` & `rudderclient-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rudderclient-1.3.0/PKG-INFO` & `rudderclient-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rudderclient
-Version: 1.3.0
+Version: 1.4.0
 Summary: Shared helpers for rudder application functions code
 Author-email: Rudder Team <rudder@realnaut.com>
 License: MIT License
         
         Copyright (c) 2023 RealNaut Ops
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `rudderclient-1.3.0/pyproject.toml` & `rudderclient-1.4.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "rudderclient"
-version = "1.3.0"
+version = "1.4.0"
 description = "Shared helpers for rudder application functions code"
 readme = "README.md"
 authors = [{ name = "Rudder Team", email = "rudder@realnaut.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `rudderclient-1.3.0/src/rudderclient/gcp/auth.py` & `rudderclient-1.4.0/src/rudderclient/gcp/auth.py`

 * *Files identical despite different names*

### Comparing `rudderclient-1.3.0/src/rudderclient/tools/send_account_email.py` & `rudderclient-1.4.0/src/rudderclient/tools/send_account_email.py`

 * *Files identical despite different names*

### Comparing `rudderclient-1.3.0/src/rudderclient.egg-info/PKG-INFO` & `rudderclient-1.4.0/src/rudderclient.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rudderclient
-Version: 1.3.0
+Version: 1.4.0
 Summary: Shared helpers for rudder application functions code
 Author-email: Rudder Team <rudder@realnaut.com>
 License: MIT License
         
         Copyright (c) 2023 RealNaut Ops
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

