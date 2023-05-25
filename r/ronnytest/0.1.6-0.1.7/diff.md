# Comparing `tmp/ronnytest-0.1.6.tar.gz` & `tmp/ronnytest-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ronnytest-0.1.6.tar", last modified: Thu May 25 06:46:51 2023, max compression
+gzip compressed data, was "dist/ronnytest-0.1.7.tar", last modified: Thu May 25 06:58:57 2023, max compression
```

## Comparing `ronnytest-0.1.6.tar` & `ronnytest-0.1.7.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 06:46:51.000000 ronnytest-0.1.6/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 06:46:51.000000 ronnytest-0.1.6/ronnytest.egg-info/
--rw-r--r--   0 root         (0) root         (0)      220 2023-05-25 06:46:51.000000 ronnytest-0.1.6/ronnytest.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 06:46:51.000000 ronnytest-0.1.6/ronnytest.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      158 2023-05-25 06:46:51.000000 ronnytest-0.1.6/ronnytest.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 06:46:51.000000 ronnytest-0.1.6/ronnytest.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      122 2023-05-25 03:55:14.000000 ronnytest-0.1.6/README.md
--rw-r--r--   0 root         (0) root         (0)     1073 2023-05-25 03:55:14.000000 ronnytest-0.1.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)      220 2023-05-25 06:46:51.000000 ronnytest-0.1.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-25 06:46:51.000000 ronnytest-0.1.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      454 2023-05-25 06:46:32.000000 ronnytest-0.1.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 06:58:57.000000 ronnytest-0.1.7/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 06:58:57.000000 ronnytest-0.1.7/ronnytest.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      220 2023-05-25 06:58:57.000000 ronnytest-0.1.7/ronnytest.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 06:58:57.000000 ronnytest-0.1.7/ronnytest.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      158 2023-05-25 06:58:57.000000 ronnytest-0.1.7/ronnytest.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 06:58:57.000000 ronnytest-0.1.7/ronnytest.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      122 2023-05-25 03:55:14.000000 ronnytest-0.1.7/README.md
+-rw-r--r--   0 root         (0) root         (0)     1073 2023-05-25 03:55:14.000000 ronnytest-0.1.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      220 2023-05-25 06:58:57.000000 ronnytest-0.1.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-25 06:58:57.000000 ronnytest-0.1.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      503 2023-05-25 06:58:34.000000 ronnytest-0.1.7/setup.py
```

### Comparing `ronnytest-0.1.6/LICENSE` & `ronnytest-0.1.7/LICENSE`

 * *Files identical despite different names*

