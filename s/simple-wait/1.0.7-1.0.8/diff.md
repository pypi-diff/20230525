# Comparing `tmp/simple-wait-1.0.7.tar.gz` & `tmp/simple-wait-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple-wait-1.0.7.tar", last modified: Tue May 23 11:05:40 2023, max compression
+gzip compressed data, was "simple-wait-1.0.8.tar", last modified: Thu May 25 11:39:05 2023, max compression
```

## Comparing `simple-wait-1.0.7.tar` & `simple-wait-1.0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:05:40.900806 simple-wait-1.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-23 11:05:29.000000 simple-wait-1.0.7/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-05-23 11:05:40.900806 simple-wait-1.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-23 11:05:29.000000 simple-wait-1.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-05-23 11:05:29.000000 simple-wait-1.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 11:05:40.900806 simple-wait-1.0.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:05:40.900806 simple-wait-1.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:05:40.900806 simple-wait-1.0.7/src/simple_wait/
--rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-05-23 11:05:29.000000 simple-wait-1.0.7/src/simple_wait/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:05:40.900806 simple-wait-1.0.7/src/simple_wait.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-05-23 11:05:40.000000 simple-wait-1.0.7/src/simple_wait.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-23 11:05:40.000000 simple-wait-1.0.7/src/simple_wait.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 11:05:40.000000 simple-wait-1.0.7/src/simple_wait.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-23 11:05:40.000000 simple-wait-1.0.7/src/simple_wait.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:05:40.900806 simple-wait-1.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-05-23 11:05:29.000000 simple-wait-1.0.7/tests/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:39:05.153510 simple-wait-1.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-25 11:38:51.000000 simple-wait-1.0.8/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-05-25 11:39:05.153510 simple-wait-1.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-05-25 11:38:51.000000 simple-wait-1.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-05-25 11:38:51.000000 simple-wait-1.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 11:39:05.153510 simple-wait-1.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:39:05.149510 simple-wait-1.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:39:05.153510 simple-wait-1.0.8/src/simple_wait/
+-rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-05-25 11:38:51.000000 simple-wait-1.0.8/src/simple_wait/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:39:05.153510 simple-wait-1.0.8/src/simple_wait.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-05-25 11:39:05.000000 simple-wait-1.0.8/src/simple_wait.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-25 11:39:05.000000 simple-wait-1.0.8/src/simple_wait.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 11:39:05.000000 simple-wait-1.0.8/src/simple_wait.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-25 11:39:05.000000 simple-wait-1.0.8/src/simple_wait.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:39:05.153510 simple-wait-1.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-05-25 11:38:51.000000 simple-wait-1.0.8/tests/tests.py
```

### Comparing `simple-wait-1.0.7/LICENSE.txt` & `simple-wait-1.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `simple-wait-1.0.7/pyproject.toml` & `simple-wait-1.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `simple-wait-1.0.7/src/simple_wait/__init__.py` & `simple-wait-1.0.8/src/simple_wait/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 __author__ = "ipetrash"
-__version__ = "1.0.7"
+__version__ = "1.0.8"
 
 
 import sys
 import time
 
 from datetime import datetime, timedelta
 from itertools import cycle
 from io import TextIOWrapper
 from typing import Iterable, Callable
 
 
 def str_timedelta(td: timedelta) -> str:
+    """
+    Returns a string description of the datetime.timedelta object
+
+    """
+
     td = str(td)
 
     # Remove ms
     # 0:01:40.123000 -> 0:01:40
     if "." in td:
         td = td[: td.rindex(".")]
 
@@ -35,14 +40,19 @@
     seconds: int = 0,
     microseconds: int = 0,
     milliseconds: int = 0,
     minutes: int = 0,
     hours: int = 0,
     weeks: int = 0,
 ) -> datetime:
+    """
+    Returns a new datetime.datetime object with the modified date
+
+    """
+
     if date is None:
         date = datetime.today()
 
     return date + timedelta(
         days=days,
         seconds=seconds,
         microseconds=microseconds,
@@ -65,14 +75,18 @@
     delay_seconds: float = 1,
     log_pattern_progress: str = "[{progress_bar}] Time left to wait: {left}",
     log_pattern_cancel: str = "\nWaiting canceled\n",
     log_pattern_clear_line: str = "\r" + " " * 100 + "\r",
     log: TextIOWrapper = sys.stdout,
     is_need_stop: Callable[[], bool] = lambda: False,
 ):
+    """
+    The function calls the wait for the specified period.
+
+    """
     try:
         progress_bar = cycle(progress_bar)
 
         today = datetime.today()
         timeout_date = get_timeout_date(
             date=today,
             days=days,
```

### Comparing `simple-wait-1.0.7/tests/tests.py` & `simple-wait-1.0.8/tests/tests.py`

 * *Files identical despite different names*

