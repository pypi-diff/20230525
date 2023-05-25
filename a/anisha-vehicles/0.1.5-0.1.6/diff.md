# Comparing `tmp/anisha_vehicles-0.1.5.tar.gz` & `tmp/anisha_vehicles-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anisha_vehicles-0.1.5.tar", max compression
+gzip compressed data, was "anisha_vehicles-0.1.6.tar", max compression
```

## Comparing `anisha_vehicles-0.1.5.tar` & `anisha_vehicles-0.1.6.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      367 2023-05-25 00:25:39.575383 anisha_vehicles-0.1.5/pyproject.toml
--rw-r--r--   0        0        0       23 2023-05-24 23:40:34.652548 anisha_vehicles-0.1.5/README.md
--rw-r--r--   0        0        0       58 2023-05-25 00:17:07.782351 anisha_vehicles-0.1.5/src/anisha_vehicles/__init__.py
--rw-r--r--   0        0        0      434 2023-05-24 23:52:28.229263 anisha_vehicles-0.1.5/src/anisha_vehicles/new_car.py
--rw-r--r--   0        0        0      433 2023-05-25 00:25:16.446436 anisha_vehicles-0.1.5/src/anisha_vehicles/old_car.py
--rw-r--r--   0        0        0      516 1970-01-01 00:00:00.000000 anisha_vehicles-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      367 2023-05-25 00:26:51.088882 anisha_vehicles-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0       23 2023-05-24 23:40:34.652548 anisha_vehicles-0.1.6/README.md
+-rw-r--r--   0        0        0       58 2023-05-25 00:17:07.782351 anisha_vehicles-0.1.6/src/anisha_vehicles/__init__.py
+-rw-r--r--   0        0        0      434 2023-05-24 23:52:28.229263 anisha_vehicles-0.1.6/src/anisha_vehicles/new_car.py
+-rw-r--r--   0        0        0      439 2023-05-25 00:26:45.763476 anisha_vehicles-0.1.6/src/anisha_vehicles/old_car.py
+-rw-r--r--   0        0        0      516 1970-01-01 00:00:00.000000 anisha_vehicles-0.1.6/PKG-INFO
```

### Comparing `anisha_vehicles-0.1.5/PKG-INFO` & `anisha_vehicles-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anisha-vehicles
-Version: 0.1.5
+Version: 0.1.6
 Summary: A test project to illustrate concepts.
 Author: Rishi Latchmepersad
 Author-email: latchmepersad@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

