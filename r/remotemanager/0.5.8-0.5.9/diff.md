# Comparing `tmp/remotemanager-0.5.8.tar.gz` & `tmp/remotemanager-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remotemanager-0.5.8.tar", last modified: Wed Feb 15 12:09:31 2023, max compression
+gzip compressed data, was "remotemanager-0.5.9.tar", last modified: Wed Feb 22 15:27:01 2023, max compression
```

## Comparing `remotemanager-0.5.8.tar` & `remotemanager-0.5.9.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-15 12:09:31.275756 remotemanager-0.5.8/
--rw-rw-rw-   0 root         (0) root         (0)     1067 2023-01-06 13:15:38.000000 remotemanager-0.5.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1279 2023-02-15 12:09:31.275756 remotemanager-0.5.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      865 2023-01-06 13:15:38.000000 remotemanager-0.5.8/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1047 2023-01-11 09:45:34.000000 remotemanager-0.5.8/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-15 12:09:31.275756 remotemanager-0.5.8/remotemanager/
--rw-rw-rw-   0 root         (0) root         (0)      483 2023-02-10 11:39:19.000000 remotemanager-0.5.8/remotemanager/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-15 12:09:31.275756 remotemanager-0.5.8/remotemanager/connection/
--rw-rw-rw-   0 root         (0) root         (0)       64 2023-01-06 13:15:38.000000 remotemanager-0.5.8/remotemanager/connection/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13686 2023-01-06 13:15:38.000000 remotemanager-0.5.8/remotemanager/connection/cmd.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-15 12:09:31.275756 remotemanager-0.5.8/remotemanager/connection/computers/
--rw-rw-rw-   0 root         (0) root         (0)      165 2023-01-06 13:15:38.000000 remotemanager-0.5.8/remotemanager/connection/computers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7574 2023-02-10 14:11:39.000000 remotemanager-0.5.8/remotemanager/connection/computers/base.py
--rw-rw-rw-   0 root         (0) root         (0)     2618 2023-01-06 13:15:38.000000 remotemanager-0.5.8/remotemanager/connection/computers/example.py
--rw-rw-rw-   0 root         (0) root         (0)    18139 2023-02-09 12:50:27.000000 remotemanager-0.5.8/remotemanager/connection/url.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-15 12:09:31.275756 remotemanager-0.5.8/remotemanager/dataset/
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-01-06 13:15:38.000000 remotemanager-0.5.8/remotemanager/dataset/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    39983 2023-02-15 10:02:59.000000 remotemanager-0.5.8/remotemanager/dataset/dataset.py
--rw-rw-rw-   0 root         (0) root         (0)     3901 2023-01-12 15:45:00.000000 remotemanager-0.5.8/remotemanager/dataset/dependency.py
--rw-rw-rw-   0 root         (0) root         (0)    22511 2023-02-15 11:45:19.000000 remotemanager-0.5.8/remotemanager/dataset/runner.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-15 12:09:31.275756 remotemanager-0.5.8/remotemanager/jupyter/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-06 13:15:38.000000 remotemanager-0.5.8/remotemanager/jupyter/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2545 2023-02-10 11:39:19.000000 remotemanager-0.5.8/remotemanager/jupyter/magic.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-15 12:09:31.275756 remotemanager-0.5.8/remotemanager/logging/
--rw-rw-rw-   0 root         (0) root         (0)     4384 2023-01-17 11:17:36.000000 remotemanager-0.5.8/remotemanager/logging/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6719 2023-01-06 13:15:38.000000 remotemanager-0.5.8/remotemanager/logging/log.py
--rw-rw-rw-   0 root         (0) root         (0)      266 2023-01-17 11:17:36.000000 remotemanager-0.5.8/remotemanager/logging/quiet.py
--rw-rw-rw-   0 root         (0) root         (0)     2183 2023-01-06 13:15:38.000000 remotemanager-0.5.8/remotemanager/logging/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2321 2023-01-06 13:15:38.000000 remotemanager-0.5.8/remotemanager/logging/verbosity.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-15 12:09:31.275756 remotemanager-0.5.8/remotemanager/serialisation/
--rw-rw-rw-   0 root         (0) root         (0)      484 2023-01-06 13:15:38.000000 remotemanager-0.5.8/remotemanager/serialisation/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4076 2023-01-06 13:15:38.000000 remotemanager-0.5.8/remotemanager/serialisation/serial.py
--rw-rw-rw-   0 root         (0) root         (0)      402 2023-01-06 13:15:38.000000 remotemanager-0.5.8/remotemanager/serialisation/serialdill.py
--rw-rw-rw-   0 root         (0) root         (0)      427 2023-01-06 13:15:38.000000 remotemanager-0.5.8/remotemanager/serialisation/serialjson.py
--rw-rw-rw-   0 root         (0) root         (0)     1613 2023-01-06 13:15:38.000000 remotemanager-0.5.8/remotemanager/serialisation/serialjsonpickle.py
--rw-rw-rw-   0 root         (0) root         (0)     1012 2023-01-06 13:15:38.000000 remotemanager-0.5.8/remotemanager/serialisation/serialyaml.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-15 12:09:31.275756 remotemanager-0.5.8/remotemanager/storage/
--rw-rw-rw-   0 root         (0) root         (0)      164 2023-01-06 13:15:38.000000 remotemanager-0.5.8/remotemanager/storage/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5398 2023-01-06 13:15:38.000000 remotemanager-0.5.8/remotemanager/storage/database.py
--rw-rw-rw-   0 root         (0) root         (0)     5031 2023-01-11 09:45:34.000000 remotemanager-0.5.8/remotemanager/storage/function.py
--rw-rw-rw-   0 root         (0) root         (0)     1053 2023-01-06 13:15:38.000000 remotemanager-0.5.8/remotemanager/storage/remotefunction.py
--rw-rw-rw-   0 root         (0) root         (0)    11103 2023-01-12 13:15:14.000000 remotemanager-0.5.8/remotemanager/storage/sendablemixin.py
--rw-rw-rw-   0 root         (0) root         (0)      927 2023-02-10 11:39:19.000000 remotemanager-0.5.8/remotemanager/storage/trackedfile.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-15 12:09:31.275756 remotemanager-0.5.8/remotemanager/transport/
--rw-rw-rw-   0 root         (0) root         (0)      181 2023-01-06 13:15:38.000000 remotemanager-0.5.8/remotemanager/transport/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      595 2023-01-13 16:10:22.000000 remotemanager-0.5.8/remotemanager/transport/cp.py
--rw-rw-rw-   0 root         (0) root         (0)     2322 2023-02-09 14:46:30.000000 remotemanager-0.5.8/remotemanager/transport/rsync.py
--rw-rw-rw-   0 root         (0) root         (0)     2113 2023-02-09 14:46:30.000000 remotemanager-0.5.8/remotemanager/transport/scp.py
--rw-rw-rw-   0 root         (0) root         (0)     9217 2023-02-09 14:46:30.000000 remotemanager-0.5.8/remotemanager/transport/transport.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-15 12:09:31.275756 remotemanager-0.5.8/remotemanager/utils/
--rw-rw-rw-   0 root         (0) root         (0)     3822 2023-01-06 13:15:38.000000 remotemanager-0.5.8/remotemanager/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4593 2023-01-06 13:15:38.000000 remotemanager-0.5.8/remotemanager/utils/flags.py
--rw-rw-rw-   0 root         (0) root         (0)      149 2023-01-06 13:15:38.000000 remotemanager-0.5.8/remotemanager/utils/uuid.py
--rw-rw-rw-   0 root         (0) root         (0)     2154 2023-01-06 13:15:38.000000 remotemanager-0.5.8/remotemanager/utils/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-15 12:09:31.275756 remotemanager-0.5.8/remotemanager.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1279 2023-02-15 12:09:31.000000 remotemanager-0.5.8/remotemanager.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1605 2023-02-15 12:09:31.000000 remotemanager-0.5.8/remotemanager.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-15 12:09:31.000000 remotemanager-0.5.8/remotemanager.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      154 2023-02-15 12:09:31.000000 remotemanager-0.5.8/remotemanager.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-02-15 12:09:31.000000 remotemanager-0.5.8/remotemanager.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-02-15 12:09:31.275756 remotemanager-0.5.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-01-06 13:15:38.000000 remotemanager-0.5.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-22 15:27:01.865754 remotemanager-0.5.9/
+-rw-rw-rw-   0 root         (0) root         (0)     1067 2023-01-06 13:15:38.000000 remotemanager-0.5.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1279 2023-02-22 15:27:01.865754 remotemanager-0.5.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      865 2023-01-06 13:15:38.000000 remotemanager-0.5.9/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1047 2023-01-11 09:45:34.000000 remotemanager-0.5.9/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-22 15:27:01.865754 remotemanager-0.5.9/remotemanager/
+-rw-rw-rw-   0 root         (0) root         (0)      483 2023-02-22 14:25:08.000000 remotemanager-0.5.9/remotemanager/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-22 15:27:01.865754 remotemanager-0.5.9/remotemanager/connection/
+-rw-rw-rw-   0 root         (0) root         (0)       64 2023-01-06 13:15:38.000000 remotemanager-0.5.9/remotemanager/connection/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13686 2023-02-21 15:14:25.000000 remotemanager-0.5.9/remotemanager/connection/cmd.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-22 15:27:01.865754 remotemanager-0.5.9/remotemanager/connection/computers/
+-rw-rw-rw-   0 root         (0) root         (0)      165 2023-01-06 13:15:38.000000 remotemanager-0.5.9/remotemanager/connection/computers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7574 2023-02-10 14:11:39.000000 remotemanager-0.5.9/remotemanager/connection/computers/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     2618 2023-01-06 13:15:38.000000 remotemanager-0.5.9/remotemanager/connection/computers/example.py
+-rw-rw-rw-   0 root         (0) root         (0)    21160 2023-02-22 14:52:36.000000 remotemanager-0.5.9/remotemanager/connection/url.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-22 15:27:01.865754 remotemanager-0.5.9/remotemanager/dataset/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-01-06 13:15:38.000000 remotemanager-0.5.9/remotemanager/dataset/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    41634 2023-02-22 14:25:08.000000 remotemanager-0.5.9/remotemanager/dataset/dataset.py
+-rw-rw-rw-   0 root         (0) root         (0)     3901 2023-01-12 15:45:00.000000 remotemanager-0.5.9/remotemanager/dataset/dependency.py
+-rw-rw-rw-   0 root         (0) root         (0)    22511 2023-02-21 15:14:25.000000 remotemanager-0.5.9/remotemanager/dataset/runner.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-22 15:27:01.865754 remotemanager-0.5.9/remotemanager/jupyter/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-06 13:15:38.000000 remotemanager-0.5.9/remotemanager/jupyter/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2545 2023-02-10 11:39:19.000000 remotemanager-0.5.9/remotemanager/jupyter/magic.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-22 15:27:01.865754 remotemanager-0.5.9/remotemanager/logging/
+-rw-rw-rw-   0 root         (0) root         (0)     4384 2023-01-17 11:17:36.000000 remotemanager-0.5.9/remotemanager/logging/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6719 2023-01-06 13:15:38.000000 remotemanager-0.5.9/remotemanager/logging/log.py
+-rw-rw-rw-   0 root         (0) root         (0)      266 2023-01-17 11:17:36.000000 remotemanager-0.5.9/remotemanager/logging/quiet.py
+-rw-rw-rw-   0 root         (0) root         (0)     2183 2023-01-06 13:15:38.000000 remotemanager-0.5.9/remotemanager/logging/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2321 2023-01-06 13:15:38.000000 remotemanager-0.5.9/remotemanager/logging/verbosity.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-22 15:27:01.865754 remotemanager-0.5.9/remotemanager/serialisation/
+-rw-rw-rw-   0 root         (0) root         (0)      484 2023-01-06 13:15:38.000000 remotemanager-0.5.9/remotemanager/serialisation/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4076 2023-01-06 13:15:38.000000 remotemanager-0.5.9/remotemanager/serialisation/serial.py
+-rw-rw-rw-   0 root         (0) root         (0)      402 2023-01-06 13:15:38.000000 remotemanager-0.5.9/remotemanager/serialisation/serialdill.py
+-rw-rw-rw-   0 root         (0) root         (0)      427 2023-01-06 13:15:38.000000 remotemanager-0.5.9/remotemanager/serialisation/serialjson.py
+-rw-rw-rw-   0 root         (0) root         (0)     1613 2023-01-06 13:15:38.000000 remotemanager-0.5.9/remotemanager/serialisation/serialjsonpickle.py
+-rw-rw-rw-   0 root         (0) root         (0)     1012 2023-01-06 13:15:38.000000 remotemanager-0.5.9/remotemanager/serialisation/serialyaml.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-22 15:27:01.865754 remotemanager-0.5.9/remotemanager/storage/
+-rw-rw-rw-   0 root         (0) root         (0)      164 2023-01-06 13:15:38.000000 remotemanager-0.5.9/remotemanager/storage/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5398 2023-01-06 13:15:38.000000 remotemanager-0.5.9/remotemanager/storage/database.py
+-rw-rw-rw-   0 root         (0) root         (0)     5031 2023-01-11 09:45:34.000000 remotemanager-0.5.9/remotemanager/storage/function.py
+-rw-rw-rw-   0 root         (0) root         (0)     1053 2023-01-06 13:15:38.000000 remotemanager-0.5.9/remotemanager/storage/remotefunction.py
+-rw-rw-rw-   0 root         (0) root         (0)    11103 2023-01-12 13:15:14.000000 remotemanager-0.5.9/remotemanager/storage/sendablemixin.py
+-rw-rw-rw-   0 root         (0) root         (0)      927 2023-02-10 11:39:19.000000 remotemanager-0.5.9/remotemanager/storage/trackedfile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-22 15:27:01.865754 remotemanager-0.5.9/remotemanager/transport/
+-rw-rw-rw-   0 root         (0) root         (0)      181 2023-01-06 13:15:38.000000 remotemanager-0.5.9/remotemanager/transport/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      595 2023-01-13 16:10:22.000000 remotemanager-0.5.9/remotemanager/transport/cp.py
+-rw-rw-rw-   0 root         (0) root         (0)     2322 2023-02-09 14:46:30.000000 remotemanager-0.5.9/remotemanager/transport/rsync.py
+-rw-rw-rw-   0 root         (0) root         (0)     2113 2023-02-09 14:46:30.000000 remotemanager-0.5.9/remotemanager/transport/scp.py
+-rw-rw-rw-   0 root         (0) root         (0)     9217 2023-02-21 15:14:25.000000 remotemanager-0.5.9/remotemanager/transport/transport.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-22 15:27:01.865754 remotemanager-0.5.9/remotemanager/utils/
+-rw-rw-rw-   0 root         (0) root         (0)     3822 2023-02-21 15:14:25.000000 remotemanager-0.5.9/remotemanager/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4593 2023-01-06 13:15:38.000000 remotemanager-0.5.9/remotemanager/utils/flags.py
+-rw-rw-rw-   0 root         (0) root         (0)      149 2023-01-06 13:15:38.000000 remotemanager-0.5.9/remotemanager/utils/uuid.py
+-rw-rw-rw-   0 root         (0) root         (0)     2154 2023-01-06 13:15:38.000000 remotemanager-0.5.9/remotemanager/utils/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-22 15:27:01.865754 remotemanager-0.5.9/remotemanager.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1279 2023-02-22 15:27:01.000000 remotemanager-0.5.9/remotemanager.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1605 2023-02-22 15:27:01.000000 remotemanager-0.5.9/remotemanager.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-02-22 15:27:01.000000 remotemanager-0.5.9/remotemanager.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      154 2023-02-22 15:27:01.000000 remotemanager-0.5.9/remotemanager.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-02-22 15:27:01.000000 remotemanager-0.5.9/remotemanager.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-02-22 15:27:01.865754 remotemanager-0.5.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-01-06 13:15:38.000000 remotemanager-0.5.9/setup.py
```

### Comparing `remotemanager-0.5.8/LICENSE` & `remotemanager-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `remotemanager-0.5.8/PKG-INFO` & `remotemanager-0.5.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remotemanager
-Version: 0.5.8
+Version: 0.5.9
 Summary: remote run management tool
 Author-email: Louis Beal <louis.j.beal@gmail.com>
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dill
```

### Comparing `remotemanager-0.5.8/README.md` & `remotemanager-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `remotemanager-0.5.8/pyproject.toml` & `remotemanager-0.5.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `remotemanager-0.5.8/remotemanager/connection/cmd.py` & `remotemanager-0.5.9/remotemanager/connection/cmd.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.5.8/remotemanager/connection/computers/base.py` & `remotemanager-0.5.9/remotemanager/connection/computers/base.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.5.8/remotemanager/connection/computers/example.py` & `remotemanager-0.5.9/remotemanager/connection/computers/example.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.5.8/remotemanager/connection/url.py` & `remotemanager-0.5.9/remotemanager/connection/url.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 URL base class for connecting to remote systems
 """
 import logging
 import os
+import time
 import typing
 
 from remotemanager.logging.utils import format_iterable
 from remotemanager.connection.cmd import CMD
 from remotemanager.storage.sendablemixin import SendableMixin
 from remotemanager.utils import ensure_list
 from remotemanager.logging import LoggingMixin
@@ -254,14 +255,72 @@
         host = self.host
         if host == URL._localhost:
             return True
         elif host.startswith('127.'):
             return True
         return False
 
+    def ping(self,
+             n: int = 5,
+             timeout: int = 30) -> float:
+        """
+        Perform and monitor a ping command
+
+        Args:
+            n (int): number of pings to aim for
+            timeout (int): kill the process and return 0 if
+                this period is elapsed
+
+        Returns:
+            (float) latency in ms
+        """
+        self._logger.runtime(f"pinging {self.host}")
+
+        def process_line(line: str) -> float:
+            line = line.split('time=')[1].strip()  # get timing
+            val = float(line.split()[0])
+            self._logger.debug(f'parsed line {line} -> {val}')
+            return val
+
+        def cleanup(process):
+            process.kill()
+            try:
+                os.remove("tmp_ping")
+                self._logger.debug('removed temporary file')
+            except FileNotFoundError:
+                self._logger.debug('temporary ping file could not be found')
+
+        ping = self.cmd(f"ping {self.host}",
+                        local=True,
+                        stdout='tmp_ping',
+                        asynchronous=True)
+
+        lines = []
+        t0 = time.time()
+        while len(lines) < n + 1:
+            with open('tmp_ping', 'r') as o:
+                lines = o.readlines()
+
+            time.sleep(0.5)
+
+            if time.time() - t0 > timeout:
+                self._logger.warning(f'ping timed out after {timeout} seconds')
+                cleanup(ping)
+                return -1
+
+        cleanup(ping)
+
+        times = []
+        for line in lines[1:]:
+            times.append(process_line(line))
+
+        avg = sum(times) / n
+        self._logger.runtime(f'ping times: {times} -> {avg}')
+        return avg
+
     def cmd(self,
             cmd: str,
             asynchronous: bool = False,
             local: [bool, None] = None,
             stdout: str = None,
             stderr: str = None,
             timeout: int = None,
@@ -349,15 +408,16 @@
         self._logger.info(f'creating a utils extension to parent: {parent}')
 
         self._parent = parent
 
     def file_mtime(self,
                    files: list,
                    local: bool = None,
-                   python: bool = False) -> dict:
+                   python: bool = False,
+                   dry_run: bool = False) -> dict:
         """
         Check file modification times of [files]
 
         Args:
             files (list):
                 list of paths to files
             local (bool):
@@ -370,15 +430,20 @@
         """
 
         self._logger.info(f'performing stat on files: {files}')
         if local is None:
             local = self._parent.is_local
 
         files = ensure_list(files)
-        times, error = self._file_mtime(files, local, python)
+        times, error = self._file_mtime(files, local, python, dry_run)
+
+        if dry_run:
+            # in this instance "times" is simply the command
+            return times
+
         self._logger.info('received:')
         self._logger.info(times)
         self._logger.info(error)
         output = {}
         for file in files:
             if file in times:
                 output[file] = times[file]
@@ -386,16 +451,17 @@
             else:
                 output[file] = None
 
         return output
 
     def _file_mtime(self,
                     files: list,
-                    local: bool = None,
-                    python: bool = False):
+                    local: bool,
+                    python: bool,
+                    dry_run: bool):
         """
         Perform the "stat -c %Y" command on a list of files,
         returning the result. Uses a python command backup if this fails
 
         Args:
             files (list):
                 list of files to check
@@ -415,15 +481,19 @@
             if len(files) == 1:
                 cmd = f'{basecmd} {files[0]}'
             else:
                 cmd = f'{basecmd} {{' + ','.join(files) + '}'
 
             ret = self._parent.cmd(cmd,
                                    local=local,
-                                   raise_errors=False)
+                                   raise_errors=False,
+                                   dry_run=dry_run)
+
+            if dry_run:
+                return ret, '', '', ''
 
             times = {}
             for line in ret.stdout.split('\n'):
                 try:
                     times[line.split(sep)[0]] = int(float(line.split(sep)[1]))
                 except IndexError:
                     pass
@@ -438,15 +508,19 @@
 \ttry: print(f'{{f}}{sep}{{os.stat(f).st_mtime}}') 
 \texcept FileNotFoundError: print(f)"""
 
             cmd = f'{self._parent.python} -c "{ex}"'
 
             ret = self._parent.cmd(cmd,
                                    local=local,
-                                   raise_errors=False)
+                                   raise_errors=False,
+                                   dry_run=dry_run)
+
+            if dry_run:
+                return ret, None
 
             times = {}
             error = []
             for line in ret.stdout.split('\n'):
                 try:
                     times[line.split(sep)[0]] = int(float(line.split(sep)[1]))
                 except IndexError:
@@ -464,15 +538,16 @@
 
             return t, e
 
         return pystat()
 
     def file_presence(self,
                       files: list,
-                      local: bool = None) -> dict:
+                      local: bool = None,
+                      dry_run: bool = False) -> dict:
         """
         Search for a list of files, returning a boolean presence dict
 
         Args:
             files (list):
                 list of paths to files
             local (bool):
@@ -484,22 +559,27 @@
         self._logger.info(f'checking for presence of files: {files}')
         if local is None:
             local = self._parent.is_local
 
         files = ensure_list(files)
 
         times = self.file_mtime(files,
-                                local=local)
+                                local=local,
+                                dry_run=dry_run)
+
+        if dry_run:
+            return times
 
         return {f: times[f] is not None for f in files}
 
     def search_folder(self,
                       files: list,
                       folder: str,
-                      local: bool = None) -> dict:
+                      local: bool = None,
+                      dry_run: bool = False) -> dict:
         """
         Search `folder` for `files`, returning a boolean presence dict
 
         Arguments:
             files (list):
                 list of filenames to check for. Optionally, a string for a
                 single file
@@ -509,21 +589,28 @@
                 perform the scan locally (or remotely)
 
         Returns (dict):
             {file: present} dictionary
         """
         if local is None:
             local = self._parent.is_local
-        fpath = os.path.abspath(folder)  # not locally available ?
+        fpath = os.path.abspath(folder) if local else folder
 
         self._logger.debug(f'scanning folder {fpath}')
         self._logger.debug('searching for files:')
         self._logger.debug(f'{format_iterable(files)}')
 
-        ls_return = self.ls(fpath, local=local, as_list=True)
+        ls_return = self.ls(fpath,
+                            local=local,
+                            as_list=True,
+                            dry_run=dry_run)
+
+        if dry_run:
+            self._logger.info('dry run, returning command')
+            return ls_return
 
         scan = [os.path.basename(f) for f in ls_return]
 
         self._logger.debug('scan sees:')
         self._logger.debug(f'{format_iterable(scan)}')
 
         if isinstance(files, str):
@@ -533,90 +620,102 @@
             ret = {file: os.path.basename(file) in scan for file in files}
 
         return ret
 
     def touch(self,
               file: str,
               local: bool = None,
-              raise_errors: bool = None) -> CMD:
+              raise_errors: bool = None,
+              dry_run: bool = False) -> CMD:
         """
         perform unix `touch`, creating or updating `file`
 
         Arguments:
             file (str):
                 filename or path to file
             local (bool):
                 force local (or remote) execution
             raise_errors (bool):
                 raise any stderr encountered
+            dry_run (bool):
+                print command only
 
         Returns (CMD):
             CMD instance for the command
         """
         if local is None:
             local = self._parent.is_local
         self._logger.debug(f'utils touch on file {file}')
-        fname = os.path.abspath(file)
+        fname = os.path.abspath(file) if local else file
         return self._parent.cmd(f'touch {fname}',
                                 local=local,
-                                raise_errors=raise_errors)
+                                raise_errors=raise_errors,
+                                dry_run=dry_run)
 
     def mkdir(self,
               file: str,
               local: bool = None,
-              raise_errors: bool = None) -> CMD:
+              raise_errors: bool = None,
+              dry_run: bool = False) -> CMD:
         """
         perform unix `mkdir -p`, creating a folder structure
 
         Arguments:
             file (str):
                 name or path to folder
             local (bool):
                 force local (or remote) execution
             raise_errors (bool):
                 raise any stderr encountered
+            dry_run (bool):
+                print command only
 
         Returns (CMD):
             CMD instance for the command
         """
         if local is None:
             local = self._parent.is_local
         self._logger.debug(f'utils mkdir on path {file}')
-        fname = os.path.abspath(file)
+        fname = os.path.abspath(file) if local else file
         # print(f'making dir {fname}')
         return self._parent.cmd(f'mkdir -p {fname}',
                                 local=local,
-                                raise_errors=raise_errors)
+                                raise_errors=raise_errors,
+                                dry_run=dry_run)
 
     def ls(self,
            file: str,
            as_list: bool = True,
            local: bool = None,
-           raise_errors: bool = None) -> [CMD, list]:
+           raise_errors: bool = None,
+           dry_run: bool = False) -> [CMD, list]:
         """
         Identify the files present on the directory
 
         Arguments:
             file (str):
                 name or path to folder.
             as_list (bool):
                 convert to a list format
             local (bool):
                 force local (or remote) execution
             raise_errors (bool):
                 raise any stderr encountered
+            dry_run (bool):
+                print command only
 
         Returns (CMD, list):
             CMD instance for the command, or the list if as_list is True
         """
         if local is None:
             local = self._parent.is_local
         self._logger.debug(f'utils ls on path {file}')
         fname = os.path.abspath(file) if local else file
 
         ret = self._parent.cmd(f'ls {fname}',
                                local=local,
-                               raise_errors=raise_errors)
+                               raise_errors=raise_errors,
+                               dry_run=dry_run)
 
-        if as_list:
+        if as_list and not dry_run:
             ret = [f for f in ret.stdout.split('\n') if f != '']
         return ret
```

### Comparing `remotemanager-0.5.8/remotemanager/dataset/dataset.py` & `remotemanager-0.5.9/remotemanager/dataset/dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import collections
 import gc
 import os
 import typing
+import shutil
 from datetime import datetime
 
 from remotemanager.storage.remotefunction import cached_functions
 from remotemanager.connection.url import URL
 from remotemanager.storage.database import Database
 from remotemanager.storage.function import Function
 from remotemanager.dataset.runner import Runner, localwinerror
@@ -552,14 +553,84 @@
 
         self._uuids = []
         self._runs = {}
 
         self.database._storage[self.uuid]['_runs'] = {}
         self.database.update(self.pack())
 
+    def clear_results(self):
+        """
+        Remove any results from the stored runners and attempt to delete their
+        result files.
+
+        .. warning::
+            This is a potentially destructive action, be careful with this
+            method
+        """
+        for runner in self.runners:
+            runner.clear_result()
+
+    def wipe_local(self):
+        """
+        Clear out the local directory
+
+        Returns:
+            None
+        """
+        locals = [self.local_dir]
+        for runner in self.runners:
+            if runner.local_dir not in locals:
+                locals.append(runner.local_dir)
+        self._logger.warning(f'removing remote_dir(s): {locals}')
+
+        for local in locals:
+            try:
+                shutil.rmtree(local)
+            except FileNotFoundError:
+                self._logger.warning(f'{local} not found')
+
+    def wipe_remote(self):
+        """
+        Clear out the remote directory (including run dir)
+
+        Returns:
+            None
+        """
+        remotes = [self.remote_dir]
+        for runner in self.runners:
+            if runner.remote_dir not in remotes:
+                remotes.append(runner.remote_dir)
+        self._logger.warning(f'removing remote_dir(s): {remotes}')
+
+        if len(remotes) > 1:
+            remotestring = ','.join(remotes)
+            self._logger.info(f'removing several remotes with '
+                              f'string {remotestring}')
+            self.url.cmd(f'rm -r {{{remotestring}}}', raise_errors=False)
+        else:
+            self.url.cmd(f'rm -r {remotes[0]}', raise_errors=False)
+
+    def hard_reset(self):
+        """
+        Hard reset the dataset, including wiping local and remote folders
+
+        Returns:
+            None
+        """
+        self.clear_runs()
+        self.wipe_local()
+        self.wipe_remote()
+
+        try:
+            os.remove(self.dbfile)
+        except FileNotFoundError:
+            pass
+
+        self.clear_runs()
+
     @property
     def runner_dict(self):
         """
         Stored runners in dict form, where the keys are the append id
         """
         return dict(self._runs)
 
@@ -1219,19 +1290,7 @@
         """
         Access the results of the runners
 
         Returns (list):
             runner.result for each runner
         """
         return [r.result for r in self.runners]
-
-    def clear_results(self):
-        """
-        Remove any results from the stored runners and attempt to delete their
-        result files.
-
-        .. warning::
-            This is a potentially destructive action, be careful with this
-            method
-        """
-        for runner in self.runners:
-            runner.clear_result()
```

### Comparing `remotemanager-0.5.8/remotemanager/dataset/dependency.py` & `remotemanager-0.5.9/remotemanager/dataset/dependency.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.5.8/remotemanager/dataset/runner.py` & `remotemanager-0.5.9/remotemanager/dataset/runner.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.5.8/remotemanager/jupyter/magic.py` & `remotemanager-0.5.9/remotemanager/jupyter/magic.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.5.8/remotemanager/logging/__init__.py` & `remotemanager-0.5.9/remotemanager/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.5.8/remotemanager/logging/log.py` & `remotemanager-0.5.9/remotemanager/logging/log.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.5.8/remotemanager/logging/utils.py` & `remotemanager-0.5.9/remotemanager/logging/utils.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.5.8/remotemanager/logging/verbosity.py` & `remotemanager-0.5.9/remotemanager/logging/verbosity.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.5.8/remotemanager/serialisation/serial.py` & `remotemanager-0.5.9/remotemanager/serialisation/serial.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.5.8/remotemanager/serialisation/serialjsonpickle.py` & `remotemanager-0.5.9/remotemanager/serialisation/serialjsonpickle.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.5.8/remotemanager/serialisation/serialyaml.py` & `remotemanager-0.5.9/remotemanager/serialisation/serialyaml.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.5.8/remotemanager/storage/database.py` & `remotemanager-0.5.9/remotemanager/storage/database.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.5.8/remotemanager/storage/function.py` & `remotemanager-0.5.9/remotemanager/storage/function.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.5.8/remotemanager/storage/remotefunction.py` & `remotemanager-0.5.9/remotemanager/storage/remotefunction.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.5.8/remotemanager/storage/sendablemixin.py` & `remotemanager-0.5.9/remotemanager/storage/sendablemixin.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.5.8/remotemanager/storage/trackedfile.py` & `remotemanager-0.5.9/remotemanager/storage/trackedfile.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.5.8/remotemanager/transport/cp.py` & `remotemanager-0.5.9/remotemanager/transport/cp.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.5.8/remotemanager/transport/rsync.py` & `remotemanager-0.5.9/remotemanager/transport/rsync.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.5.8/remotemanager/transport/scp.py` & `remotemanager-0.5.9/remotemanager/transport/scp.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.5.8/remotemanager/transport/transport.py` & `remotemanager-0.5.9/remotemanager/transport/transport.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.5.8/remotemanager/utils/__init__.py` & `remotemanager-0.5.9/remotemanager/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.5.8/remotemanager/utils/flags.py` & `remotemanager-0.5.9/remotemanager/utils/flags.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.5.8/remotemanager/utils/version.py` & `remotemanager-0.5.9/remotemanager/utils/version.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.5.8/remotemanager.egg-info/PKG-INFO` & `remotemanager-0.5.9/remotemanager.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remotemanager
-Version: 0.5.8
+Version: 0.5.9
 Summary: remote run management tool
 Author-email: Louis Beal <louis.j.beal@gmail.com>
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dill
```

### Comparing `remotemanager-0.5.8/remotemanager.egg-info/SOURCES.txt` & `remotemanager-0.5.9/remotemanager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

