# Comparing `tmp/DataDoctor-1.0.3.tar.gz` & `tmp/DataDoctor-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DataDoctor-1.0.3.tar", last modified: Thu May 25 01:05:38 2023, max compression
+gzip compressed data, was "DataDoctor-1.0.4.tar", last modified: Thu May 25 15:27:34 2023, max compression
```

## Comparing `DataDoctor-1.0.3.tar` & `DataDoctor-1.0.4.tar`

### file list

```diff
@@ -1,11 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 01:05:38.247070 DataDoctor-1.0.3/
-drwxrwxrwx   0        0        0        0 2023-05-25 01:05:38.246069 DataDoctor-1.0.3/DataDoctor.egg-info/
--rw-rw-rw-   0        0        0     1959 2023-05-25 01:05:38.000000 DataDoctor-1.0.3/DataDoctor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      187 2023-05-25 01:05:38.000000 DataDoctor-1.0.3/DataDoctor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 01:05:38.000000 DataDoctor-1.0.3/DataDoctor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       64 2023-05-25 01:05:38.000000 DataDoctor-1.0.3/DataDoctor.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 01:05:38.000000 DataDoctor-1.0.3/DataDoctor.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1959 2023-05-25 01:05:38.247070 DataDoctor-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1735 2023-05-25 00:58:24.000000 DataDoctor-1.0.3/README.md
--rw-rw-rw-   0        0        0       42 2023-05-25 01:05:38.248070 DataDoctor-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      648 2023-05-25 01:05:29.000000 DataDoctor-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-25 15:27:34.544182 DataDoctor-1.0.4/
+drwxrwxrwx   0        0        0        0 2023-05-25 15:27:34.536963 DataDoctor-1.0.4/DataDoctor.egg-info/
+-rw-rw-rw-   0        0        0     4309 2023-05-25 15:27:34.000000 DataDoctor-1.0.4/DataDoctor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2023-05-25 15:27:34.000000 DataDoctor-1.0.4/DataDoctor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 15:27:34.000000 DataDoctor-1.0.4/DataDoctor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2023-05-25 15:27:34.000000 DataDoctor-1.0.4/DataDoctor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-25 15:27:34.000000 DataDoctor-1.0.4/DataDoctor.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1087 2023-05-25 13:43:05.000000 DataDoctor-1.0.4/LICENSE.md
+-rw-rw-rw-   0        0        0     4309 2023-05-25 15:27:34.541667 DataDoctor-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3429 2023-05-25 15:20:12.000000 DataDoctor-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-25 15:27:34.540659 DataDoctor-1.0.4/data_doctor/
+-rw-rw-rw-   0        0        0        0 2023-05-25 13:44:09.000000 DataDoctor-1.0.4/data_doctor/__init__.py
+-rw-rw-rw-   0        0        0     8399 2023-05-25 00:59:10.000000 DataDoctor-1.0.4/data_doctor/cleaner.py
+-rw-rw-rw-   0        0        0     7391 2023-05-25 13:50:05.000000 DataDoctor-1.0.4/data_doctor/normalizer.py
+-rw-rw-rw-   0        0        0      248 2023-05-25 13:51:08.000000 DataDoctor-1.0.4/data_doctor/utils.py
+-rw-rw-rw-   0        0        0       42 2023-05-25 15:27:34.545031 DataDoctor-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1277 2023-05-25 15:25:59.000000 DataDoctor-1.0.4/setup.py
```

