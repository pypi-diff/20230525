# Comparing `tmp/SiteScraper-0.2.1.tar.gz` & `tmp/SiteScraper-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SiteScraper-0.2.1.tar", last modified: Wed May  3 17:18:41 2023, max compression
+gzip compressed data, was "SiteScraper-0.2.2.tar", last modified: Thu May  4 14:10:15 2023, max compression
```

## Comparing `SiteScraper-0.2.1.tar` & `SiteScraper-0.2.2.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 17:18:41.739139 SiteScraper-0.2.1/
--rw-rw-rw-   0        0        0      159 2023-05-03 17:18:41.738141 SiteScraper-0.2.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-03 17:18:41.730465 SiteScraper-0.2.1/SiteScraper/
--rw-rw-rw-   0        0        0     8875 2023-05-03 17:15:01.000000 SiteScraper-0.2.1/SiteScraper/SiteScraper.py
--rw-rw-rw-   0        0        0       35 2023-05-01 18:12:54.000000 SiteScraper-0.2.1/SiteScraper/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 17:18:41.737144 SiteScraper-0.2.1/SiteScraper.egg-info/
--rw-rw-rw-   0        0        0      159 2023-05-03 17:18:41.000000 SiteScraper-0.2.1/SiteScraper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      233 2023-05-03 17:18:41.000000 SiteScraper-0.2.1/SiteScraper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 17:18:41.000000 SiteScraper-0.2.1/SiteScraper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-03 17:18:41.000000 SiteScraper-0.2.1/SiteScraper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-03 17:18:41.000000 SiteScraper-0.2.1/SiteScraper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-03 17:18:41.739139 SiteScraper-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0      341 2023-05-03 17:17:45.000000 SiteScraper-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 14:10:15.175120 SiteScraper-0.2.2/
+-rw-rw-rw-   0        0        0     1948 2023-05-04 14:10:15.175120 SiteScraper-0.2.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-04 14:10:15.170133 SiteScraper-0.2.2/SiteScraper/
+-rw-rw-rw-   0        0        0     8875 2023-05-03 17:15:01.000000 SiteScraper-0.2.2/SiteScraper/SiteScraper.py
+-rw-rw-rw-   0        0        0       35 2023-05-01 18:12:54.000000 SiteScraper-0.2.2/SiteScraper/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 14:10:15.174123 SiteScraper-0.2.2/SiteScraper.egg-info/
+-rw-rw-rw-   0        0        0     1948 2023-05-04 14:10:15.000000 SiteScraper-0.2.2/SiteScraper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      267 2023-05-04 14:10:15.000000 SiteScraper-0.2.2/SiteScraper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 14:10:15.000000 SiteScraper-0.2.2/SiteScraper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-04 14:10:15.000000 SiteScraper-0.2.2/SiteScraper.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        9 2023-05-04 14:10:15.000000 SiteScraper-0.2.2/SiteScraper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-04 14:10:15.000000 SiteScraper-0.2.2/SiteScraper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-04 14:10:15.175120 SiteScraper-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0      497 2023-05-04 13:58:14.000000 SiteScraper-0.2.2/setup.py
```

### Comparing `SiteScraper-0.2.1/SiteScraper/SiteScraper.py` & `SiteScraper-0.2.2/SiteScraper/SiteScraper.py`

 * *Files identical despite different names*

