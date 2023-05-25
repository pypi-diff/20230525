# Comparing `tmp/django-intenumfield-1.4.1.tar.gz` & `tmp/django_intenumfield-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-intenumfield-1.4.1.tar", last modified: Fri Dec 17 21:12:46 2021, max compression
+gzip compressed data, was "django_intenumfield-1.5.0.tar", max compression
```

## Comparing `django-intenumfield-1.4.1.tar` & `django_intenumfield-1.5.0.tar`

### file list

```diff
@@ -1,14 +1,5 @@
-drwxr-xr-x   0 benedict  (1000) benedict  (1000)        0 2021-12-17 21:12:46.000000 django-intenumfield-1.4.1/
-drwxr-xr-x   0 benedict  (1000) benedict  (1000)        0 2021-12-17 21:12:46.000000 django-intenumfield-1.4.1/django_intenum/
--rw-r--r--   0 benedict  (1000) benedict  (1000)     1876 2021-12-17 20:53:58.000000 django-intenumfield-1.4.1/django_intenum/__init__.py
-drwxr-xr-x   0 benedict  (1000) benedict  (1000)        0 2021-12-17 21:12:46.000000 django-intenumfield-1.4.1/django_intenumfield.egg-info/
--rw-r--r--   0 benedict  (1000) benedict  (1000)      887 2021-12-17 21:12:46.000000 django-intenumfield-1.4.1/django_intenumfield.egg-info/PKG-INFO
--rw-r--r--   0 benedict  (1000) benedict  (1000)      277 2021-12-17 21:12:46.000000 django-intenumfield-1.4.1/django_intenumfield.egg-info/SOURCES.txt
--rw-r--r--   0 benedict  (1000) benedict  (1000)        1 2021-12-17 21:12:46.000000 django-intenumfield-1.4.1/django_intenumfield.egg-info/dependency_links.txt
--rw-r--r--   0 benedict  (1000) benedict  (1000)       12 2021-12-17 21:12:46.000000 django-intenumfield-1.4.1/django_intenumfield.egg-info/requires.txt
--rw-r--r--   0 benedict  (1000) benedict  (1000)       15 2021-12-17 21:12:46.000000 django-intenumfield-1.4.1/django_intenumfield.egg-info/top_level.txt
--rw-r--r--   0 benedict  (1000) benedict  (1000)     1055 2021-12-17 20:40:19.000000 django-intenumfield-1.4.1/LICENSE
--rw-r--r--   0 benedict  (1000) benedict  (1000)      820 2021-12-17 21:12:32.000000 django-intenumfield-1.4.1/README.md
--rw-r--r--   0 benedict  (1000) benedict  (1000)      815 2021-12-17 21:12:46.000000 django-intenumfield-1.4.1/setup.cfg
--rwxr-xr-x   0 benedict  (1000) benedict  (1000)       62 2021-12-17 20:40:19.000000 django-intenumfield-1.4.1/setup.py
--rw-r--r--   0 benedict  (1000) benedict  (1000)      887 2021-12-17 21:12:46.000000 django-intenumfield-1.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1055 2023-05-25 09:25:00.704374 django_intenumfield-1.5.0/LICENSE
+-rw-r--r--   0        0        0      820 2023-05-25 09:25:00.704374 django_intenumfield-1.5.0/README.md
+-rw-r--r--   0        0        0     1876 2023-05-25 09:25:00.704374 django_intenumfield-1.5.0/django_intenum/__init__.py
+-rw-r--r--   0        0        0      658 2023-05-25 09:25:00.704374 django_intenumfield-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1648 1970-01-01 00:00:00.000000 django_intenumfield-1.5.0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `django-intenumfield-1.4.1/django_intenum/__init__.py` & `django_intenumfield-1.5.0/django_intenum/__init__.py`

 * *Files identical despite different names*

### Comparing `django-intenumfield-1.4.1/LICENSE` & `django_intenumfield-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-intenumfield-1.4.1/README.md` & `django_intenumfield-1.5.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 * Store your multiple-choice options as a smallint (2 bytes) instead of varchar
 * Reuse existing IntEnums as choice values
 * Integrates well with Django's admin app (display and filter)
 
 ## Requirements
 
 * Python 3.6+
-* Django 2.0+
+* Django 2.2+
 
 ## Usage
 
 ```py
 from enum import IntEnum
 from django.db import models
 from django_intenum import IntEnumField
```

