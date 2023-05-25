# Comparing `tmp/ronnytest-0.2.3.tar.gz` & `tmp/ronnytest-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ronnytest-0.2.3.tar", last modified: Thu May 25 08:32:28 2023, max compression
+gzip compressed data, was "dist/ronnytest-0.2.4.tar", last modified: Thu May 25 11:40:43 2023, max compression
```

## Comparing `ronnytest-0.2.3.tar` & `ronnytest-0.2.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 08:32:28.000000 ronnytest-0.2.3/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 08:32:28.000000 ronnytest-0.2.3/ronnytest.egg-info/
--rw-r--r--   0 root         (0) root         (0)      220 2023-05-25 08:32:28.000000 ronnytest-0.2.3/ronnytest.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 08:32:28.000000 ronnytest-0.2.3/ronnytest.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      158 2023-05-25 08:32:28.000000 ronnytest-0.2.3/ronnytest.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 08:32:28.000000 ronnytest-0.2.3/ronnytest.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      122 2023-05-25 03:55:14.000000 ronnytest-0.2.3/README.md
--rw-r--r--   0 root         (0) root         (0)     1073 2023-05-25 03:55:14.000000 ronnytest-0.2.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)      220 2023-05-25 08:32:28.000000 ronnytest-0.2.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-25 08:32:28.000000 ronnytest-0.2.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      963 2023-05-25 08:32:09.000000 ronnytest-0.2.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 11:40:43.000000 ronnytest-0.2.4/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 11:40:43.000000 ronnytest-0.2.4/ronnytest.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      220 2023-05-25 11:40:43.000000 ronnytest-0.2.4/ronnytest.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 11:40:43.000000 ronnytest-0.2.4/ronnytest.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      158 2023-05-25 11:40:43.000000 ronnytest-0.2.4/ronnytest.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 11:40:43.000000 ronnytest-0.2.4/ronnytest.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      122 2023-05-25 03:55:14.000000 ronnytest-0.2.4/README.md
+-rw-r--r--   0 root         (0) root         (0)     1073 2023-05-25 03:55:14.000000 ronnytest-0.2.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      220 2023-05-25 11:40:43.000000 ronnytest-0.2.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-25 11:40:43.000000 ronnytest-0.2.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1694 2023-05-25 11:40:41.000000 ronnytest-0.2.4/setup.py
```

### Comparing `ronnytest-0.2.3/LICENSE` & `ronnytest-0.2.4/LICENSE`

 * *Files identical despite different names*

