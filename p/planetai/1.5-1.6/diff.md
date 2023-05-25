# Comparing `tmp/planetai-1.5.tar.gz` & `tmp/planetai-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "planetai-1.5.tar", last modified: Sat Apr 15 12:35:33 2023, max compression
+gzip compressed data, was "planetai-1.6.tar", last modified: Thu May 25 13:43:54 2023, max compression
```

## Comparing `planetai-1.5.tar` & `planetai-1.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 12:35:33.068872 planetai-1.5/
--rw-rw-rw-   0        0        0      137 2023-04-15 12:35:33.068872 planetai-1.5/PKG-INFO
--rw-rw-rw-   0        0        0      317 2023-04-15 11:11:06.000000 planetai-1.5/README.md
--rw-rw-rw-   0        0        0     1065 2023-04-15 12:32:27.000000 planetai-1.5/license.txt
-drwxrwxrwx   0        0        0        0 2023-04-15 12:35:33.029676 planetai-1.5/planetai/
--rw-rw-rw-   0        0        0       27 2023-04-15 11:31:24.000000 planetai-1.5/planetai/__init__.py
--rw-rw-rw-   0        0        0       35 2023-04-15 11:10:33.000000 planetai-1.5/planetai/main.py
--rw-rw-rw-   0        0        0     3037 2023-04-15 12:22:18.000000 planetai-1.5/planetai/planet.py
-drwxrwxrwx   0        0        0        0 2023-04-15 12:35:33.066872 planetai-1.5/planetai.egg-info/
--rw-rw-rw-   0        0        0      137 2023-04-15 12:35:32.000000 planetai-1.5/planetai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      256 2023-04-15 12:35:32.000000 planetai-1.5/planetai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 12:35:32.000000 planetai-1.5/planetai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-15 12:35:32.000000 planetai-1.5/planetai.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        9 2023-04-15 12:35:32.000000 planetai-1.5/planetai.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-04-15 12:35:33.071873 planetai-1.5/setup.cfg
--rw-rw-rw-   0        0        0      331 2023-04-15 12:35:21.000000 planetai-1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-25 13:43:54.898284 planetai-1.6/
+-rw-rw-rw-   0        0        0      137 2023-05-25 13:43:54.899319 planetai-1.6/PKG-INFO
+-rw-rw-rw-   0        0        0      317 2023-04-15 11:11:06.000000 planetai-1.6/README.md
+-rw-rw-rw-   0        0        0     1065 2023-04-15 12:32:27.000000 planetai-1.6/license.txt
+drwxrwxrwx   0        0        0        0 2023-05-25 13:43:54.850807 planetai-1.6/planetai/
+-rw-rw-rw-   0        0        0       56 2023-05-25 13:04:17.000000 planetai-1.6/planetai/__init__.py
+-rw-rw-rw-   0        0        0       66 2023-05-25 13:03:52.000000 planetai-1.6/planetai/main.py
+-rw-rw-rw-   0        0        0    10232 2023-05-25 13:04:25.000000 planetai-1.6/planetai/planet.py
+drwxrwxrwx   0        0        0        0 2023-05-25 13:43:54.898284 planetai-1.6/planetai.egg-info/
+-rw-rw-rw-   0        0        0      137 2023-05-25 13:43:54.000000 planetai-1.6/planetai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      256 2023-05-25 13:43:54.000000 planetai-1.6/planetai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 13:43:54.000000 planetai-1.6/planetai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-15 12:35:32.000000 planetai-1.6/planetai.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        9 2023-05-25 13:43:54.000000 planetai-1.6/planetai.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-05-25 13:43:54.899319 planetai-1.6/setup.cfg
+-rw-rw-rw-   0        0        0      331 2023-05-25 13:05:18.000000 planetai-1.6/setup.py
```

### Comparing `planetai-1.5/license.txt` & `planetai-1.6/license.txt`

 * *Files identical despite different names*

