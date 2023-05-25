# Comparing `tmp/roxbot-0.0.3.tar.gz` & `tmp/roxbot-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roxbot-0.0.3.tar", last modified: Thu May 25 17:40:09 2023, max compression
+gzip compressed data, was "roxbot-0.1.1.tar", last modified: Thu May 25 17:52:26 2023, max compression
```

## Comparing `roxbot-0.0.3.tar` & `roxbot-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2023-05-25 17:40:09.629574 roxbot-0.0.3/
--rw-rw-r--   0 dev       (1000) dev       (1000)     1106 2023-05-25 16:43:03.000000 roxbot-0.0.3/LICENCE
--rw-r--r--   0 dev       (1000) dev       (1000)      384 2023-05-25 17:40:09.629574 roxbot-0.0.3/PKG-INFO
--rw-rw-r--   0 dev       (1000) dev       (1000)     1598 2023-05-25 17:37:09.000000 roxbot-0.0.3/README.md
--rw-rw-r--   0 dev       (1000) dev       (1000)      360 2023-05-25 17:40:09.629574 roxbot-0.0.3/setup.cfg
--rw-rw-r--   0 dev       (1000) dev       (1000)     1467 2023-05-25 17:37:15.000000 roxbot-0.0.3/setup.py
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2023-05-25 17:40:09.621574 roxbot-0.0.3/src/
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2023-05-25 17:40:09.625574 roxbot-0.0.3/src/roxbot/
--rw-rw-r--   0 dev       (1000) dev       (1000)       22 2023-05-25 17:17:16.000000 roxbot-0.0.3/src/roxbot/__init__.py
--rw-rw-r--   0 dev       (1000) dev       (1000)      302 2023-05-25 17:37:15.000000 roxbot-0.0.3/src/roxbot/cli.py
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2023-05-25 17:40:09.629574 roxbot-0.0.3/src/roxbot.egg-info/
--rw-r--r--   0 dev       (1000) dev       (1000)      384 2023-05-25 17:40:09.000000 roxbot-0.0.3/src/roxbot.egg-info/PKG-INFO
--rw-r--r--   0 dev       (1000) dev       (1000)      301 2023-05-25 17:40:09.000000 roxbot-0.0.3/src/roxbot.egg-info/SOURCES.txt
--rw-r--r--   0 dev       (1000) dev       (1000)        1 2023-05-25 17:40:09.000000 roxbot-0.0.3/src/roxbot.egg-info/dependency_links.txt
--rw-r--r--   0 dev       (1000) dev       (1000)       42 2023-05-25 17:40:09.000000 roxbot-0.0.3/src/roxbot.egg-info/entry_points.txt
--rw-r--r--   0 dev       (1000) dev       (1000)        6 2023-05-25 17:40:09.000000 roxbot-0.0.3/src/roxbot.egg-info/requires.txt
--rw-r--r--   0 dev       (1000) dev       (1000)        7 2023-05-25 17:40:09.000000 roxbot-0.0.3/src/roxbot.egg-info/top_level.txt
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2023-05-25 17:40:09.629574 roxbot-0.0.3/tests/
--rw-rw-r--   0 dev       (1000) dev       (1000)      462 2023-05-25 17:37:15.000000 roxbot-0.0.3/tests/test_cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:52:26.588015 roxbot-0.1.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1106 2023-05-25 17:52:14.000000 roxbot-0.1.1/LICENCE
+-rw-r--r--   0 root         (0) root         (0)      384 2023-05-25 17:52:26.588015 roxbot-0.1.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1598 2023-05-25 17:52:14.000000 roxbot-0.1.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      360 2023-05-25 17:52:26.589015 roxbot-0.1.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1467 2023-05-25 17:52:14.000000 roxbot-0.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:52:26.585015 roxbot-0.1.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:52:26.587015 roxbot-0.1.1/src/roxbot/
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-05-25 17:52:14.000000 roxbot-0.1.1/src/roxbot/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      302 2023-05-25 17:52:14.000000 roxbot-0.1.1/src/roxbot/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:52:26.588015 roxbot-0.1.1/src/roxbot.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      384 2023-05-25 17:52:26.000000 roxbot-0.1.1/src/roxbot.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      301 2023-05-25 17:52:26.000000 roxbot-0.1.1/src/roxbot.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 17:52:26.000000 roxbot-0.1.1/src/roxbot.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       42 2023-05-25 17:52:26.000000 roxbot-0.1.1/src/roxbot.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-05-25 17:52:26.000000 roxbot-0.1.1/src/roxbot.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-05-25 17:52:26.000000 roxbot-0.1.1/src/roxbot.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:52:26.588015 roxbot-0.1.1/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      462 2023-05-25 17:52:14.000000 roxbot-0.1.1/tests/test_cli.py
```

### Comparing `roxbot-0.0.3/LICENCE` & `roxbot-0.1.1/LICENCE`

 * *Files identical despite different names*

### Comparing `roxbot-0.0.3/README.md` & `roxbot-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `roxbot-0.0.3/setup.py` & `roxbot-0.1.1/setup.py`

 * *Files identical despite different names*

