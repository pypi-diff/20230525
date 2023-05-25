# Comparing `tmp/fhict_cb_01-0.1.tar.gz` & `tmp/fhict_cb_01-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fhict_cb_01-0.1.tar", last modified: Tue Jun 28 11:26:36 2022, max compression
+gzip compressed data, was "fhict_cb_01-0.2.tar", last modified: Thu May 25 13:15:58 2023, max compression
```

## Comparing `fhict_cb_01-0.1.tar` & `fhict_cb_01-0.2.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxrwxrwx   0        0        0        0 2022-06-28 11:26:36.437060 fhict_cb_01-0.1/
--rw-rw-rw-   0        0        0     1081 2022-06-28 09:16:20.000000 fhict_cb_01-0.1/LICENSE.txt
--rw-rw-rw-   0        0        0      254 2022-06-28 11:26:36.438056 fhict_cb_01-0.1/PKG-INFO
--rw-rw-rw-   0        0        0      589 2022-06-28 09:16:20.000000 fhict_cb_01-0.1/README.md
--rw-rw-rw-   0        0        0      115 2022-06-28 11:26:36.439058 fhict_cb_01-0.1/setup.cfg
--rw-rw-rw-   0        0        0      608 2022-06-28 11:26:11.000000 fhict_cb_01-0.1/setup.py
-drwxrwxrwx   0        0        0        0 2022-06-28 11:26:36.409055 fhict_cb_01-0.1/src/
-drwxrwxrwx   0        0        0        0 2022-06-28 11:26:36.425055 fhict_cb_01-0.1/src/fhict_cb_01/
--rw-rw-rw-   0        0        0     1749 2022-06-28 11:25:56.000000 fhict_cb_01-0.1/src/fhict_cb_01/CustomPymata4.py
--rw-rw-rw-   0        0        0        0 2022-06-28 09:16:20.000000 fhict_cb_01-0.1/src/fhict_cb_01/__init__.py
--rw-rw-rw-   0        0        0       74 2022-06-28 11:21:47.000000 fhict_cb_01-0.1/src/fhict_cb_01/flask.py
-drwxrwxrwx   0        0        0        0 2022-06-28 11:26:36.435056 fhict_cb_01-0.1/src/fhict_cb_01.egg-info/
--rw-rw-rw-   0        0        0      254 2022-06-28 11:26:35.000000 fhict_cb_01-0.1/src/fhict_cb_01.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      320 2022-06-28 11:26:36.000000 fhict_cb_01-0.1/src/fhict_cb_01.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-06-28 11:26:35.000000 fhict_cb_01-0.1/src/fhict_cb_01.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2022-06-28 11:26:36.000000 fhict_cb_01-0.1/src/fhict_cb_01.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2022-06-28 11:26:36.000000 fhict_cb_01-0.1/src/fhict_cb_01.egg-info/top_level.txt
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-05-25 13:15:58.838276 fhict_cb_01-0.2/
+-rw-rw-r--   0 mark      (1000) mark      (1000)       27 2023-05-25 13:12:47.000000 fhict_cb_01-0.2/LICENSE.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)      311 2023-05-25 13:15:58.838276 fhict_cb_01-0.2/PKG-INFO
+-rw-rw-r--   0 mark      (1000) mark      (1000)      358 2023-05-25 13:13:41.000000 fhict_cb_01-0.2/README.md
+-rw-rw-r--   0 mark      (1000) mark      (1000)      107 2023-05-25 13:15:58.838276 fhict_cb_01-0.2/setup.cfg
+-rw-rw-r--   0 mark      (1000) mark      (1000)      528 2023-05-25 13:15:56.000000 fhict_cb_01-0.2/setup.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-05-25 13:15:58.838276 fhict_cb_01-0.2/src/
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-05-25 13:15:58.838276 fhict_cb_01-0.2/src/fhict_cb_01/
+-rw-rw-r--   0 mark      (1000) mark      (1000)        0 2023-05-25 13:03:22.000000 fhict_cb_01-0.2/src/fhict_cb_01/__init__.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     3742 2023-05-25 13:07:19.000000 fhict_cb_01-0.2/src/fhict_cb_01/custom_telemetrix.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-05-25 13:15:58.838276 fhict_cb_01-0.2/src/fhict_cb_01.egg-info/
+-rw-rw-r--   0 mark      (1000) mark      (1000)      311 2023-05-25 13:15:58.000000 fhict_cb_01-0.2/src/fhict_cb_01.egg-info/PKG-INFO
+-rw-rw-r--   0 mark      (1000) mark      (1000)      299 2023-05-25 13:15:58.000000 fhict_cb_01-0.2/src/fhict_cb_01.egg-info/SOURCES.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)        1 2023-05-25 13:15:58.000000 fhict_cb_01-0.2/src/fhict_cb_01.egg-info/dependency_links.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)       64 2023-05-25 13:15:58.000000 fhict_cb_01-0.2/src/fhict_cb_01.egg-info/requires.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)       12 2023-05-25 13:15:58.000000 fhict_cb_01-0.2/src/fhict_cb_01.egg-info/top_level.txt
```

