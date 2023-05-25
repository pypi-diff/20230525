# Comparing `tmp/T1TV-0.1.tar.gz` & `tmp/T1TV-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "T1TV-0.1.tar", last modified: Wed May 24 16:10:34 2023, max compression
+gzip compressed data, was "T1TV-0.2.tar", last modified: Thu May 25 18:22:06 2023, max compression
```

## Comparing `T1TV-0.1.tar` & `T1TV-0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-24 16:10:34.309828 T1TV-0.1/
--rw-rw----   0 root         (0) everybody  (9997)       20 2023-05-23 23:06:22.000000 T1TV-0.1/LICENSE.txt
--rw-rw----   0 root         (0) everybody  (9997)      356 2023-05-24 16:10:34.285828 T1TV-0.1/PKG-INFO
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-24 16:10:34.157828 T1TV-0.1/T1TV/
--rw-rw----   0 root         (0) everybody  (9997)     2690 2023-05-23 22:58:57.000000 T1TV-0.1/T1TV/__init__.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-24 16:10:34.265828 T1TV-0.1/T1TV.egg-info/
--rw-rw----   0 root         (0) everybody  (9997)      356 2023-05-24 16:10:33.000000 T1TV-0.1/T1TV.egg-info/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)      149 2023-05-24 16:10:34.000000 T1TV-0.1/T1TV.egg-info/SOURCES.txt
--rw-rw----   0 root         (0) everybody  (9997)        1 2023-05-24 16:10:33.000000 T1TV-0.1/T1TV.egg-info/dependency_links.txt
--rw-rw----   0 root         (0) everybody  (9997)        5 2023-05-24 16:10:33.000000 T1TV-0.1/T1TV.egg-info/top_level.txt
--rw-rw----   0 root         (0) everybody  (9997)       38 2023-05-24 16:10:34.309828 T1TV-0.1/setup.cfg
--rw-rw----   0 root         (0) everybody  (9997)      397 2023-05-24 16:10:20.000000 T1TV-0.1/setup.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-25 18:22:06.921646 T1TV-0.2/
+-rw-rw----   0 root         (0) everybody  (9997)       20 2023-05-23 23:06:22.000000 T1TV-0.2/LICENSE.txt
+-rw-rw----   0 root         (0) everybody  (9997)      356 2023-05-25 18:22:06.901646 T1TV-0.2/PKG-INFO
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-25 18:22:06.781646 T1TV-0.2/T1TV/
+-rw-rw----   0 root         (0) everybody  (9997)     3760 2023-05-25 18:21:37.000000 T1TV-0.2/T1TV/__init__.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-25 18:22:06.877646 T1TV-0.2/T1TV.egg-info/
+-rw-rw----   0 root         (0) everybody  (9997)      356 2023-05-25 18:22:06.000000 T1TV-0.2/T1TV.egg-info/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)      149 2023-05-25 18:22:06.000000 T1TV-0.2/T1TV.egg-info/SOURCES.txt
+-rw-rw----   0 root         (0) everybody  (9997)        1 2023-05-25 18:22:06.000000 T1TV-0.2/T1TV.egg-info/dependency_links.txt
+-rw-rw----   0 root         (0) everybody  (9997)        5 2023-05-25 18:22:06.000000 T1TV-0.2/T1TV.egg-info/top_level.txt
+-rw-rw----   0 root         (0) everybody  (9997)       38 2023-05-25 18:22:06.925646 T1TV-0.2/setup.cfg
+-rw-rw----   0 root         (0) everybody  (9997)      397 2023-05-25 17:47:41.000000 T1TV-0.2/setup.py
```

