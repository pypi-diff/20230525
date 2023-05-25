# Comparing `tmp/macos_application_location-1.0.3.tar.gz` & `tmp/macos_application_location-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macos_application_location-1.0.3.tar", max compression
+gzip compressed data, was "macos_application_location-1.0.4.tar", max compression
```

## Comparing `macos_application_location-1.0.3.tar` & `macos_application_location-1.0.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    16725 2023-05-24 17:18:29.408463 macos_application_location-1.0.3/LICENSE
--rw-r--r--   0        0        0      353 2023-05-24 18:08:11.959269 macos_application_location-1.0.3/README.md
--rw-r--r--   0        0        0       22 2023-05-24 17:18:42.355322 macos_application_location-1.0.3/packages/macos_application_location/__init__.py
--rw-r--r--   0        0        0      331 2023-05-24 18:04:54.723624 macos_application_location-1.0.3/packages/macos_application_location/main.py
--rw-r--r--   0        0        0      537 2023-05-24 18:09:05.762315 macos_application_location-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     1163 1970-01-01 00:00:00.000000 macos_application_location-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0    16725 2023-05-24 17:18:29.408463 macos_application_location-1.0.4/LICENSE
+-rw-r--r--   0        0        0      354 2023-05-25 00:24:38.654897 macos_application_location-1.0.4/README.md
+-rw-r--r--   0        0        0       22 2023-05-24 17:18:42.355322 macos_application_location-1.0.4/packages/macos_application_location/__init__.py
+-rw-r--r--   0        0        0      331 2023-05-24 18:04:54.723624 macos_application_location-1.0.4/packages/macos_application_location/main.py
+-rw-r--r--   0        0        0      543 2023-05-25 00:25:04.183585 macos_application_location-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1170 1970-01-01 00:00:00.000000 macos_application_location-1.0.4/PKG-INFO
```

### Comparing `macos_application_location-1.0.3/LICENSE` & `macos_application_location-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `macos_application_location-1.0.3/PKG-INFO` & `macos_application_location-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: macos-application-location
-Version: 1.0.3
+Version: 1.0.4
 Summary: 
-Home-page: https://github.com/changyuheng/macos-application-location
+Home-page: https://github.com/changyuheng/macos-application-location.py
 License: MPL-2.0
 Author: Johann Chang
 Author-email: mr.changyuheng@gmail.com
 Requires-Python: >=3.5
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Project-URL: Repository, https://github.com/changyuheng/macos-application-location
+Project-URL: Repository, https://github.com/changyuheng/macos-application-location.py
 Description-Content-Type: text/markdown
 
 # macos-application-location.py
 
-This tiny module helps you to obtain the path of an Application (.app) that the current process is running from on macOS.
+This tiny package helps you to obtain the path of an Application (.app) that the current process is running from on macOS.
 
 ## Installation
 
 ```sh
 pip install macos-application-location
 ```
```

