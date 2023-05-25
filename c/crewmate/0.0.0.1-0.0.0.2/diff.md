# Comparing `tmp/crewmate-0.0.0.1.tar.gz` & `tmp/crewmate-0.0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crewmate-0.0.0.1.tar", last modified: Thu May 25 07:20:55 2023, max compression
+gzip compressed data, was "crewmate-0.0.0.2.tar", last modified: Thu May 25 09:24:43 2023, max compression
```

## Comparing `crewmate-0.0.0.1.tar` & `crewmate-0.0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 07:20:55.827229 crewmate-0.0.0.1/
--rw-rw-rw-   0        0        0      423 2023-05-25 07:20:55.827229 crewmate-0.0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-05-25 06:47:55.000000 crewmate-0.0.0.1/README.md
--rw-rw-rw-   0        0        0      108 2023-05-25 06:50:37.000000 crewmate-0.0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      598 2023-05-25 07:20:55.827522 crewmate-0.0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-25 07:20:55.818157 crewmate-0.0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-25 07:20:55.821337 crewmate-0.0.0.1/src/crewmate/
--rw-rw-rw-   0        0        0        0 2023-05-25 06:41:04.000000 crewmate-0.0.0.1/src/crewmate/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 07:20:55.825942 crewmate-0.0.0.1/src/crewmate.egg-info/
--rw-rw-rw-   0        0        0      423 2023-05-25 07:20:55.000000 crewmate-0.0.0.1/src/crewmate.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      203 2023-05-25 07:20:55.000000 crewmate-0.0.0.1/src/crewmate.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 07:20:55.000000 crewmate-0.0.0.1/src/crewmate.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-25 07:20:55.000000 crewmate-0.0.0.1/src/crewmate.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-25 09:24:43.053292 crewmate-0.0.0.2/
+-rw-rw-rw-   0        0        0      178 2023-05-25 09:24:43.052290 crewmate-0.0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      434 2023-05-25 09:23:08.000000 crewmate-0.0.0.2/README.md
+-rw-rw-rw-   0        0        0      108 2023-05-25 06:50:37.000000 crewmate-0.0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-25 09:24:43.053292 crewmate-0.0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      465 2023-05-25 09:23:09.000000 crewmate-0.0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-25 09:24:43.043127 crewmate-0.0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-05-25 09:24:43.051290 crewmate-0.0.0.2/src/crewmate.egg-info/
+-rw-rw-rw-   0        0        0      178 2023-05-25 09:24:42.000000 crewmate-0.0.0.2/src/crewmate.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      212 2023-05-25 09:24:42.000000 crewmate-0.0.0.2/src/crewmate.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 09:24:42.000000 crewmate-0.0.0.2/src/crewmate.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-05-25 09:24:42.000000 crewmate-0.0.0.2/src/crewmate.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-05-25 09:24:42.000000 crewmate-0.0.0.2/src/crewmate.egg-info/top_level.txt
```

