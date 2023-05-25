# Comparing `tmp/AlienUpgrade-0.0.1.tar.gz` & `tmp/AlienUpgrade-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AlienUpgrade-0.0.1.tar", last modified: Wed May 24 14:55:41 2023, max compression
+gzip compressed data, was "AlienUpgrade-0.0.2.tar", last modified: Thu May 25 15:23:46 2023, max compression
```

## Comparing `AlienUpgrade-0.0.1.tar` & `AlienUpgrade-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 14:55:41.617858 AlienUpgrade-0.0.1/
-drwxrwxrwx   0        0        0        0 2023-05-24 14:55:41.603355 AlienUpgrade-0.0.1/AlienUpgrade/
--rw-rw-rw-   0        0        0       28 2023-05-24 14:34:31.000000 AlienUpgrade-0.0.1/AlienUpgrade/__init__.py
--rw-rw-rw-   0        0        0       36 2023-05-24 14:31:37.000000 AlienUpgrade-0.0.1/AlienUpgrade/ultimate.py
-drwxrwxrwx   0        0        0        0 2023-05-24 14:55:41.615860 AlienUpgrade-0.0.1/AlienUpgrade.egg-info/
--rw-rw-rw-   0        0        0      471 2023-05-24 14:55:41.000000 AlienUpgrade-0.0.1/AlienUpgrade.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      212 2023-05-24 14:55:41.000000 AlienUpgrade-0.0.1/AlienUpgrade.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 14:55:41.000000 AlienUpgrade-0.0.1/AlienUpgrade.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-05-24 14:55:41.000000 AlienUpgrade-0.0.1/AlienUpgrade.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      471 2023-05-24 14:55:41.616860 AlienUpgrade-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0        8 2023-05-24 14:55:34.000000 AlienUpgrade-0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-05-24 14:55:41.617858 AlienUpgrade-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1006 2023-05-24 14:51:15.000000 AlienUpgrade-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-25 15:23:46.938883 AlienUpgrade-0.0.2/
+drwxrwxrwx   0        0        0        0 2023-05-25 15:23:46.930886 AlienUpgrade-0.0.2/AlienUpgrade/
+-rw-rw-rw-   0        0        0       41 2023-05-25 14:17:09.000000 AlienUpgrade-0.0.2/AlienUpgrade/__init__.py
+-rw-rw-rw-   0        0        0       66 2023-05-25 14:48:14.000000 AlienUpgrade-0.0.2/AlienUpgrade/ultimate.py
+drwxrwxrwx   0        0        0        0 2023-05-25 15:23:46.938883 AlienUpgrade-0.0.2/AlienUpgrade.egg-info/
+-rw-rw-rw-   0        0        0      662 2023-05-25 15:23:46.000000 AlienUpgrade-0.0.2/AlienUpgrade.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      212 2023-05-25 15:23:46.000000 AlienUpgrade-0.0.2/AlienUpgrade.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 15:23:46.000000 AlienUpgrade-0.0.2/AlienUpgrade.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-25 15:23:46.000000 AlienUpgrade-0.0.2/AlienUpgrade.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      662 2023-05-25 15:23:46.938883 AlienUpgrade-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      193 2023-05-25 15:13:21.000000 AlienUpgrade-0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-25 15:23:46.938883 AlienUpgrade-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1006 2023-05-25 15:17:39.000000 AlienUpgrade-0.0.2/setup.py
```

### Comparing `AlienUpgrade-0.0.1/setup.py` & `AlienUpgrade-0.0.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'Recover Deleted Files'
 LONG_DESCRIPTION = 'A package that allows to recover deleted files'
 
 # Setting up
 setup(
     name="AlienUpgrade",
     version=VERSION,
```

