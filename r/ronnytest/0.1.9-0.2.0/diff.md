# Comparing `tmp/ronnytest-0.1.9.tar.gz` & `tmp/ronnytest-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ronnytest-0.1.9.tar", last modified: Thu May 25 07:38:40 2023, max compression
+gzip compressed data, was "dist/ronnytest-0.2.0.tar", last modified: Thu May 25 08:04:07 2023, max compression
```

## Comparing `ronnytest-0.1.9.tar` & `ronnytest-0.2.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 07:38:40.000000 ronnytest-0.1.9/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 07:38:40.000000 ronnytest-0.1.9/ronnytest.egg-info/
--rw-r--r--   0 root         (0) root         (0)      220 2023-05-25 07:38:40.000000 ronnytest-0.1.9/ronnytest.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 07:38:40.000000 ronnytest-0.1.9/ronnytest.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      158 2023-05-25 07:38:40.000000 ronnytest-0.1.9/ronnytest.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 07:38:40.000000 ronnytest-0.1.9/ronnytest.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      122 2023-05-25 03:55:14.000000 ronnytest-0.1.9/README.md
--rw-r--r--   0 root         (0) root         (0)     1073 2023-05-25 03:55:14.000000 ronnytest-0.1.9/LICENSE
--rw-r--r--   0 root         (0) root         (0)      220 2023-05-25 07:38:40.000000 ronnytest-0.1.9/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-25 07:38:40.000000 ronnytest-0.1.9/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      464 2023-05-25 07:38:16.000000 ronnytest-0.1.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 08:04:07.000000 ronnytest-0.2.0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 08:04:07.000000 ronnytest-0.2.0/ronnytest.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      220 2023-05-25 08:04:07.000000 ronnytest-0.2.0/ronnytest.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 08:04:07.000000 ronnytest-0.2.0/ronnytest.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      158 2023-05-25 08:04:07.000000 ronnytest-0.2.0/ronnytest.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 08:04:07.000000 ronnytest-0.2.0/ronnytest.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      122 2023-05-25 03:55:14.000000 ronnytest-0.2.0/README.md
+-rw-r--r--   0 root         (0) root         (0)     1073 2023-05-25 03:55:14.000000 ronnytest-0.2.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      220 2023-05-25 08:04:07.000000 ronnytest-0.2.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-25 08:04:07.000000 ronnytest-0.2.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1038 2023-05-25 08:01:17.000000 ronnytest-0.2.0/setup.py
```

### Comparing `ronnytest-0.1.9/LICENSE` & `ronnytest-0.2.0/LICENSE`

 * *Files identical despite different names*

