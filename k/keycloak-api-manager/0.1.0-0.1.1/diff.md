# Comparing `tmp/keycloak_api_manager-0.1.0.tar.gz` & `tmp/keycloak_api_manager-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keycloak_api_manager-0.1.0.tar", last modified: Thu May 25 13:23:05 2023, max compression
+gzip compressed data, was "keycloak_api_manager-0.1.1.tar", last modified: Thu May 25 13:46:10 2023, max compression
```

## Comparing `keycloak_api_manager-0.1.0.tar` & `keycloak_api_manager-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 13:23:05.420410 keycloak_api_manager-0.1.0/
--rw-rw-rw-   0        0        0     1060 2023-05-25 10:35:55.000000 keycloak_api_manager-0.1.0/LICENSE.txt
--rw-rw-rw-   0        0        0      264 2023-05-25 13:23:05.421987 keycloak_api_manager-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1798 2023-05-25 13:22:09.000000 keycloak_api_manager-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-25 13:23:05.386576 keycloak_api_manager-0.1.0/keycloak_api_manager/
--rw-rw-rw-   0        0        0       56 2023-05-25 13:20:41.000000 keycloak_api_manager-0.1.0/keycloak_api_manager/__init__.py
--rw-rw-rw-   0        0        0     8348 2023-05-25 13:20:04.000000 keycloak_api_manager-0.1.0/keycloak_api_manager/keycloak_api_manager.py
-drwxrwxrwx   0        0        0        0 2023-05-25 13:23:05.419456 keycloak_api_manager-0.1.0/keycloak_api_manager.egg-info/
--rw-rw-rw-   0        0        0      264 2023-05-25 13:23:05.000000 keycloak_api_manager-0.1.0/keycloak_api_manager.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      337 2023-05-25 13:23:05.000000 keycloak_api_manager-0.1.0/keycloak_api_manager.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 13:23:05.000000 keycloak_api_manager-0.1.0/keycloak_api_manager.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-25 13:23:05.000000 keycloak_api_manager-0.1.0/keycloak_api_manager.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-05-25 13:23:05.000000 keycloak_api_manager-0.1.0/keycloak_api_manager.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-25 13:23:05.425688 keycloak_api_manager-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      392 2023-05-25 13:23:03.000000 keycloak_api_manager-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-25 13:46:10.752923 keycloak_api_manager-0.1.1/
+-rw-rw-rw-   0        0        0     1060 2023-05-25 10:35:55.000000 keycloak_api_manager-0.1.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     2601 2023-05-25 13:46:10.751855 keycloak_api_manager-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1798 2023-05-25 13:22:09.000000 keycloak_api_manager-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-25 13:46:10.712156 keycloak_api_manager-0.1.1/keycloak_api_manager/
+-rw-rw-rw-   0        0        0       56 2023-05-25 13:20:41.000000 keycloak_api_manager-0.1.1/keycloak_api_manager/__init__.py
+-rw-rw-rw-   0        0        0     8348 2023-05-25 13:20:04.000000 keycloak_api_manager-0.1.1/keycloak_api_manager/keycloak_api_manager.py
+drwxrwxrwx   0        0        0        0 2023-05-25 13:46:10.750955 keycloak_api_manager-0.1.1/keycloak_api_manager.egg-info/
+-rw-rw-rw-   0        0        0     2601 2023-05-25 13:46:10.000000 keycloak_api_manager-0.1.1/keycloak_api_manager.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      333 2023-05-25 13:46:10.000000 keycloak_api_manager-0.1.1/keycloak_api_manager.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 13:46:10.000000 keycloak_api_manager-0.1.1/keycloak_api_manager.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-25 13:46:10.000000 keycloak_api_manager-0.1.1/keycloak_api_manager.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-05-25 13:46:10.000000 keycloak_api_manager-0.1.1/keycloak_api_manager.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      928 2023-05-25 13:45:41.000000 keycloak_api_manager-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-25 13:46:10.753920 keycloak_api_manager-0.1.1/setup.cfg
```

### Comparing `keycloak_api_manager-0.1.0/LICENSE.txt` & `keycloak_api_manager-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `keycloak_api_manager-0.1.0/README.md` & `keycloak_api_manager-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `keycloak_api_manager-0.1.0/keycloak_api_manager/keycloak_api_manager.py` & `keycloak_api_manager-0.1.1/keycloak_api_manager/keycloak_api_manager.py`

 * *Files identical despite different names*

