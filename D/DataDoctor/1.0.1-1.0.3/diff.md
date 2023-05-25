# Comparing `tmp/DataDoctor-1.0.1.tar.gz` & `tmp/DataDoctor-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DataDoctor-1.0.1.tar", last modified: Thu May 25 00:44:15 2023, max compression
+gzip compressed data, was "DataDoctor-1.0.3.tar", last modified: Thu May 25 01:05:38 2023, max compression
```

## Comparing `DataDoctor-1.0.1.tar` & `DataDoctor-1.0.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 00:44:15.469540 DataDoctor-1.0.1/
-drwxrwxrwx   0        0        0        0 2023-05-25 00:44:15.469540 DataDoctor-1.0.1/DataDoctor.egg-info/
--rw-rw-rw-   0        0        0      181 2023-05-25 00:44:15.000000 DataDoctor-1.0.1/DataDoctor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      187 2023-05-25 00:44:15.000000 DataDoctor-1.0.1/DataDoctor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 00:44:15.000000 DataDoctor-1.0.1/DataDoctor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       64 2023-05-25 00:44:15.000000 DataDoctor-1.0.1/DataDoctor.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 00:44:15.000000 DataDoctor-1.0.1/DataDoctor.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      181 2023-05-25 00:44:15.469540 DataDoctor-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1735 2023-05-25 00:44:07.000000 DataDoctor-1.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-05-25 00:44:15.469540 DataDoctor-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      446 2023-05-25 00:33:40.000000 DataDoctor-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-25 01:05:38.247070 DataDoctor-1.0.3/
+drwxrwxrwx   0        0        0        0 2023-05-25 01:05:38.246069 DataDoctor-1.0.3/DataDoctor.egg-info/
+-rw-rw-rw-   0        0        0     1959 2023-05-25 01:05:38.000000 DataDoctor-1.0.3/DataDoctor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      187 2023-05-25 01:05:38.000000 DataDoctor-1.0.3/DataDoctor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 01:05:38.000000 DataDoctor-1.0.3/DataDoctor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2023-05-25 01:05:38.000000 DataDoctor-1.0.3/DataDoctor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 01:05:38.000000 DataDoctor-1.0.3/DataDoctor.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1959 2023-05-25 01:05:38.247070 DataDoctor-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1735 2023-05-25 00:58:24.000000 DataDoctor-1.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-25 01:05:38.248070 DataDoctor-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      648 2023-05-25 01:05:29.000000 DataDoctor-1.0.3/setup.py
```

### Comparing `DataDoctor-1.0.1/README.md` & `DataDoctor-1.0.3/README.md`

 * *Files identical despite different names*

