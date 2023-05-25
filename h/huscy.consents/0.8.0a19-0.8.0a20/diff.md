# Comparing `tmp/huscy.consents-0.8.0a19.tar.gz` & `tmp/huscy.consents-0.8.0a20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huscy.consents-0.8.0a19.tar", last modified: Mon May 22 14:55:32 2023, max compression
+gzip compressed data, was "huscy.consents-0.8.0a20.tar", last modified: Thu May 25 15:55:28 2023, max compression
```

## Comparing `huscy.consents-0.8.0a19.tar` & `huscy.consents-0.8.0a20.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-05-22 14:55:32.156561 huscy.consents-0.8.0a19/
--rw-r--r--   0 jenkins    (111) jenkins    (115)       59 2022-11-22 11:01:15.000000 huscy.consents-0.8.0a19/MANIFEST.in
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1072 2023-05-22 14:55:32.156561 huscy.consents-0.8.0a19/PKG-INFO
--rw-r--r--   0 jenkins    (111) jenkins    (115)       17 2022-07-26 09:43:57.000000 huscy.consents-0.8.0a19/README.md
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-05-22 14:55:32.140561 huscy.consents-0.8.0a19/huscy/
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-05-22 14:55:32.140561 huscy.consents-0.8.0a19/huscy/consents/
--rwxr-xr-x   0 jenkins    (111) jenkins    (115)       82 2023-05-16 11:02:46.000000 huscy.consents-0.8.0a19/huscy/consents/__init__.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      597 2023-03-10 09:59:30.000000 huscy.consents-0.8.0a19/huscy/consents/admin.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      319 2023-01-20 13:15:27.000000 huscy.consents-0.8.0a19/huscy/consents/api_urls.py
--rwxr-xr-x   0 jenkins    (111) jenkins    (115)      186 2022-07-26 09:43:57.000000 huscy.consents-0.8.0a19/huscy/consents/apps.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1557 2023-04-03 08:38:05.000000 huscy.consents-0.8.0a19/huscy/consents/forms.py
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-05-22 14:55:32.144561 huscy.consents-0.8.0a19/huscy/consents/migrations/
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1519 2023-05-22 14:55:31.000000 huscy.consents-0.8.0a19/huscy/consents/migrations/0001_initial.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)        0 2022-11-15 15:35:43.000000 huscy.consents-0.8.0a19/huscy/consents/migrations/__init__.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      638 2023-03-10 09:59:30.000000 huscy.consents-0.8.0a19/huscy/consents/models.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      938 2023-01-20 13:15:27.000000 huscy.consents-0.8.0a19/huscy/consents/serializer.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     7037 2023-05-16 11:02:46.000000 huscy.consents-0.8.0a19/huscy/consents/services.py
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-05-22 14:55:32.140561 huscy.consents-0.8.0a19/huscy/consents/static/
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-05-22 14:55:32.140561 huscy.consents-0.8.0a19/huscy/consents/static/consents/
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-05-22 14:55:32.144561 huscy.consents-0.8.0a19/huscy/consents/static/consents/css/
--rw-r--r--   0 jenkins    (111) jenkins    (115)  1611020 2023-04-14 09:53:34.000000 huscy.consents-0.8.0a19/huscy/consents/static/consents/css/fomantic.min.css
--rw-r--r--   0 jenkins    (111) jenkins    (115)  1611020 2023-04-14 09:53:34.000000 huscy.consents-0.8.0a19/huscy/consents/static/consents/css/fomantic2.9.0.min.css
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-05-22 14:55:32.144561 huscy.consents-0.8.0a19/huscy/consents/static/consents/img/
--rw-r--r--   0 jenkins    (111) jenkins    (115)    33728 2023-04-14 09:53:34.000000 huscy.consents-0.8.0a19/huscy/consents/static/consents/img/logo.svg
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-05-22 14:55:32.152561 huscy.consents-0.8.0a19/huscy/consents/static/consents/js/
--rw-r--r--   0 jenkins    (111) jenkins    (115)   403124 2023-04-14 09:53:34.000000 huscy.consents-0.8.0a19/huscy/consents/static/consents/js/fomantic.min.js
--rw-r--r--   0 jenkins    (111) jenkins    (115)   403124 2023-04-14 09:53:34.000000 huscy.consents-0.8.0a19/huscy/consents/static/consents/js/fomantic2.9.0.min.js
--rw-r--r--   0 jenkins    (111) jenkins    (115)    89664 2023-04-14 09:53:34.000000 huscy.consents-0.8.0a19/huscy/consents/static/consents/js/jquery.min.js
--rw-r--r--   0 jenkins    (111) jenkins    (115)    89664 2023-04-14 09:53:34.000000 huscy.consents-0.8.0a19/huscy/consents/static/consents/js/jquery3.6.1.min.js
--rw-r--r--   0 jenkins    (111) jenkins    (115)    21233 2023-04-14 09:53:34.000000 huscy.consents-0.8.0a19/huscy/consents/static/consents/js/popper.min.js
--rw-r--r--   0 jenkins    (111) jenkins    (115)    21233 2023-04-14 09:53:34.000000 huscy.consents-0.8.0a19/huscy/consents/static/consents/js/popper1.16.1.min.js
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-05-22 14:55:32.140561 huscy.consents-0.8.0a19/huscy/consents/templates/
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-05-22 14:55:32.152561 huscy.consents-0.8.0a19/huscy/consents/templates/consents/
--rw-r--r--   0 jenkins    (111) jenkins    (115)      599 2023-04-14 09:53:34.000000 huscy.consents-0.8.0a19/huscy/consents/templates/consents/base.html
--rw-r--r--   0 jenkins    (111) jenkins    (115)     6660 2023-01-20 13:15:27.000000 huscy.consents-0.8.0a19/huscy/consents/templates/consents/create_consent.html
--rwxr-xr-x   0 jenkins    (111) jenkins    (115)     4342 2023-04-14 09:53:34.000000 huscy.consents-0.8.0a19/huscy/consents/templates/consents/sign_consent.html
--rwxr-xr-x   0 jenkins    (111) jenkins    (115)     3129 2023-04-14 09:53:34.000000 huscy.consents-0.8.0a19/huscy/consents/templates/consents/signed_consent.html
--rw-r--r--   0 jenkins    (111) jenkins    (115)        8 2022-11-15 15:35:43.000000 huscy.consents-0.8.0a19/huscy/consents/templates/consents/success.html
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-05-22 14:55:32.156561 huscy.consents-0.8.0a19/huscy/consents/templates/consents/text_fragments/
--rw-r--r--   0 jenkins    (111) jenkins    (115)      275 2023-04-03 08:38:05.000000 huscy.consents-0.8.0a19/huscy/consents/templates/consents/text_fragments/checkbox.html
--rw-r--r--   0 jenkins    (111) jenkins    (115)      113 2023-05-16 11:02:46.000000 huscy.consents-0.8.0a19/huscy/consents/templates/consents/text_fragments/heading.html
--rw-r--r--   0 jenkins    (111) jenkins    (115)       72 2023-05-16 11:02:46.000000 huscy.consents-0.8.0a19/huscy/consents/templates/consents/text_fragments/markdown.html
--rw-r--r--   0 jenkins    (111) jenkins    (115)      176 2023-01-10 14:57:17.000000 huscy.consents-0.8.0a19/huscy/consents/templates/consents/text_fragments/paragraph.html
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-05-22 14:55:32.156561 huscy.consents-0.8.0a19/huscy/consents/templates/consents/widgets/
--rw-r--r--   0 jenkins    (111) jenkins    (115)      165 2022-11-15 15:35:43.000000 huscy.consents-0.8.0a19/huscy/consents/templates/consents/widgets/select_date.html
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-05-22 14:55:32.156561 huscy.consents-0.8.0a19/huscy/consents/templatetags/
--rw-r--r--   0 jenkins    (111) jenkins    (115)        0 2023-04-03 08:38:05.000000 huscy.consents-0.8.0a19/huscy/consents/templatetags/__init__.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      155 2023-04-03 08:38:05.000000 huscy.consents-0.8.0a19/huscy/consents/templatetags/dict_extras.py
--rwxr-xr-x   0 jenkins    (111) jenkins    (115)      436 2022-11-15 15:35:43.000000 huscy.consents-0.8.0a19/huscy/consents/urls.py
--rwxr-xr-x   0 jenkins    (111) jenkins    (115)     4544 2023-04-03 08:38:05.000000 huscy.consents-0.8.0a19/huscy/consents/views.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      580 2023-01-20 13:15:27.000000 huscy.consents-0.8.0a19/huscy/consents/viewsets.py
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-05-22 14:55:32.140561 huscy.consents-0.8.0a19/huscy.consents.egg-info/
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1072 2023-05-22 14:55:32.000000 huscy.consents-0.8.0a19/huscy.consents.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1685 2023-05-22 14:55:32.000000 huscy.consents-0.8.0a19/huscy.consents.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (111) jenkins    (115)        1 2023-05-22 14:55:32.000000 huscy.consents-0.8.0a19/huscy.consents.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (111) jenkins    (115)      208 2023-05-22 14:55:32.000000 huscy.consents-0.8.0a19/huscy.consents.egg-info/requires.txt
--rw-r--r--   0 jenkins    (111) jenkins    (115)        6 2023-05-22 14:55:32.000000 huscy.consents-0.8.0a19/huscy.consents.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (111) jenkins    (115)       38 2023-05-22 14:55:32.156561 huscy.consents-0.8.0a19/setup.cfg
--rwxr-xr-x   0 jenkins    (111) jenkins    (115)     1766 2023-05-16 11:02:46.000000 huscy.consents-0.8.0a19/setup.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-05-25 15:55:28.335811 huscy.consents-0.8.0a20/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)       59 2022-11-22 11:01:15.000000 huscy.consents-0.8.0a20/MANIFEST.in
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1072 2023-05-25 15:55:28.335811 huscy.consents-0.8.0a20/PKG-INFO
+-rw-r--r--   0 jenkins    (111) jenkins    (115)       17 2022-07-26 09:43:57.000000 huscy.consents-0.8.0a20/README.md
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-05-25 15:55:28.315811 huscy.consents-0.8.0a20/huscy/
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-05-25 15:55:28.319811 huscy.consents-0.8.0a20/huscy/consents/
+-rwxr-xr-x   0 jenkins    (111) jenkins    (115)       82 2023-05-25 10:06:04.000000 huscy.consents-0.8.0a20/huscy/consents/__init__.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      597 2023-03-10 09:59:30.000000 huscy.consents-0.8.0a20/huscy/consents/admin.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      319 2023-01-20 13:15:27.000000 huscy.consents-0.8.0a20/huscy/consents/api_urls.py
+-rwxr-xr-x   0 jenkins    (111) jenkins    (115)      186 2022-07-26 09:43:57.000000 huscy.consents-0.8.0a20/huscy/consents/apps.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1557 2023-04-03 08:38:05.000000 huscy.consents-0.8.0a20/huscy/consents/forms.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-05-25 15:55:28.319811 huscy.consents-0.8.0a20/huscy/consents/migrations/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1519 2023-05-25 15:55:27.000000 huscy.consents-0.8.0a20/huscy/consents/migrations/0001_initial.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)        0 2022-11-15 15:35:43.000000 huscy.consents-0.8.0a20/huscy/consents/migrations/__init__.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      638 2023-03-10 09:59:30.000000 huscy.consents-0.8.0a20/huscy/consents/models.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      938 2023-01-20 13:15:27.000000 huscy.consents-0.8.0a20/huscy/consents/serializer.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     6695 2023-05-25 10:06:04.000000 huscy.consents-0.8.0a20/huscy/consents/services.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-05-25 15:55:28.315811 huscy.consents-0.8.0a20/huscy/consents/static/
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-05-25 15:55:28.315811 huscy.consents-0.8.0a20/huscy/consents/static/consents/
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-05-25 15:55:28.319811 huscy.consents-0.8.0a20/huscy/consents/static/consents/css/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)  1611020 2023-04-14 09:53:34.000000 huscy.consents-0.8.0a20/huscy/consents/static/consents/css/fomantic.min.css
+-rw-r--r--   0 jenkins    (111) jenkins    (115)  1611020 2023-04-14 09:53:34.000000 huscy.consents-0.8.0a20/huscy/consents/static/consents/css/fomantic2.9.0.min.css
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-05-25 15:55:28.323811 huscy.consents-0.8.0a20/huscy/consents/static/consents/img/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)    33728 2023-04-14 09:53:34.000000 huscy.consents-0.8.0a20/huscy/consents/static/consents/img/logo.svg
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-05-25 15:55:28.327811 huscy.consents-0.8.0a20/huscy/consents/static/consents/js/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)   403124 2023-04-14 09:53:34.000000 huscy.consents-0.8.0a20/huscy/consents/static/consents/js/fomantic.min.js
+-rw-r--r--   0 jenkins    (111) jenkins    (115)   403124 2023-04-14 09:53:34.000000 huscy.consents-0.8.0a20/huscy/consents/static/consents/js/fomantic2.9.0.min.js
+-rw-r--r--   0 jenkins    (111) jenkins    (115)    89664 2023-04-14 09:53:34.000000 huscy.consents-0.8.0a20/huscy/consents/static/consents/js/jquery.min.js
+-rw-r--r--   0 jenkins    (111) jenkins    (115)    89664 2023-04-14 09:53:34.000000 huscy.consents-0.8.0a20/huscy/consents/static/consents/js/jquery3.6.1.min.js
+-rw-r--r--   0 jenkins    (111) jenkins    (115)    21233 2023-04-14 09:53:34.000000 huscy.consents-0.8.0a20/huscy/consents/static/consents/js/popper.min.js
+-rw-r--r--   0 jenkins    (111) jenkins    (115)    21233 2023-04-14 09:53:34.000000 huscy.consents-0.8.0a20/huscy/consents/static/consents/js/popper1.16.1.min.js
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-05-25 15:55:28.315811 huscy.consents-0.8.0a20/huscy/consents/templates/
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-05-25 15:55:28.331811 huscy.consents-0.8.0a20/huscy/consents/templates/consents/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      599 2023-04-14 09:53:34.000000 huscy.consents-0.8.0a20/huscy/consents/templates/consents/base.html
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     6660 2023-01-20 13:15:27.000000 huscy.consents-0.8.0a20/huscy/consents/templates/consents/create_consent.html
+-rwxr-xr-x   0 jenkins    (111) jenkins    (115)     4342 2023-04-14 09:53:34.000000 huscy.consents-0.8.0a20/huscy/consents/templates/consents/sign_consent.html
+-rwxr-xr-x   0 jenkins    (111) jenkins    (115)     3129 2023-04-14 09:53:34.000000 huscy.consents-0.8.0a20/huscy/consents/templates/consents/signed_consent.html
+-rw-r--r--   0 jenkins    (111) jenkins    (115)        8 2022-11-15 15:35:43.000000 huscy.consents-0.8.0a20/huscy/consents/templates/consents/success.html
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-05-25 15:55:28.335811 huscy.consents-0.8.0a20/huscy/consents/templates/consents/text_fragments/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      275 2023-04-03 08:38:05.000000 huscy.consents-0.8.0a20/huscy/consents/templates/consents/text_fragments/checkbox.html
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      113 2023-05-16 11:02:46.000000 huscy.consents-0.8.0a20/huscy/consents/templates/consents/text_fragments/heading.html
+-rw-r--r--   0 jenkins    (111) jenkins    (115)       72 2023-05-16 11:02:46.000000 huscy.consents-0.8.0a20/huscy/consents/templates/consents/text_fragments/markdown.html
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      176 2023-01-10 14:57:17.000000 huscy.consents-0.8.0a20/huscy/consents/templates/consents/text_fragments/paragraph.html
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-05-25 15:55:28.335811 huscy.consents-0.8.0a20/huscy/consents/templates/consents/widgets/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      165 2022-11-15 15:35:43.000000 huscy.consents-0.8.0a20/huscy/consents/templates/consents/widgets/select_date.html
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-05-25 15:55:28.335811 huscy.consents-0.8.0a20/huscy/consents/templatetags/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)        0 2023-04-03 08:38:05.000000 huscy.consents-0.8.0a20/huscy/consents/templatetags/__init__.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      155 2023-04-03 08:38:05.000000 huscy.consents-0.8.0a20/huscy/consents/templatetags/dict_extras.py
+-rwxr-xr-x   0 jenkins    (111) jenkins    (115)      436 2022-11-15 15:35:43.000000 huscy.consents-0.8.0a20/huscy/consents/urls.py
+-rwxr-xr-x   0 jenkins    (111) jenkins    (115)     4544 2023-04-03 08:38:05.000000 huscy.consents-0.8.0a20/huscy/consents/views.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      580 2023-01-20 13:15:27.000000 huscy.consents-0.8.0a20/huscy/consents/viewsets.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-05-25 15:55:28.319811 huscy.consents-0.8.0a20/huscy.consents.egg-info/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1072 2023-05-25 15:55:28.000000 huscy.consents-0.8.0a20/huscy.consents.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1685 2023-05-25 15:55:28.000000 huscy.consents-0.8.0a20/huscy.consents.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)        1 2023-05-25 15:55:28.000000 huscy.consents-0.8.0a20/huscy.consents.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      208 2023-05-25 15:55:28.000000 huscy.consents-0.8.0a20/huscy.consents.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)        6 2023-05-25 15:55:28.000000 huscy.consents-0.8.0a20/huscy.consents.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)       38 2023-05-25 15:55:28.335811 huscy.consents-0.8.0a20/setup.cfg
+-rwxr-xr-x   0 jenkins    (111) jenkins    (115)     1766 2023-05-16 11:02:46.000000 huscy.consents-0.8.0a20/setup.py
```

### Comparing `huscy.consents-0.8.0a19/PKG-INFO` & `huscy.consents-0.8.0a20/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: huscy.consents
-Version: 0.8.0a19
+Version: 0.8.0a20
 Summary: consents
 Home-page: https://bitbucket.org/huscy/consents
 Author: Gefan Qian, Stefan Bunde
 Author-email: gefan.qian@gmail.com, stefanbunde+git@posteo.de
 License: AGPLv3+
 Description: # huscy.consents
```

### Comparing `huscy.consents-0.8.0a19/huscy/consents/admin.py` & `huscy.consents-0.8.0a20/huscy/consents/admin.py`

 * *Files identical despite different names*

### Comparing `huscy.consents-0.8.0a19/huscy/consents/forms.py` & `huscy.consents-0.8.0a20/huscy/consents/forms.py`

 * *Files identical despite different names*

### Comparing `huscy.consents-0.8.0a19/huscy/consents/migrations/0001_initial.py` & `huscy.consents-0.8.0a20/huscy/consents/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `huscy.consents-0.8.0a19/huscy/consents/models.py` & `huscy.consents-0.8.0a20/huscy/consents/models.py`

 * *Files identical despite different names*

### Comparing `huscy.consents-0.8.0a19/huscy/consents/serializer.py` & `huscy.consents-0.8.0a20/huscy/consents/serializer.py`

 * *Files identical despite different names*

### Comparing `huscy.consents-0.8.0a19/huscy/consents/services.py` & `huscy.consents-0.8.0a20/huscy/consents/services.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,142 +1,174 @@
 import jsonschema
 
 from huscy.consents.models import Consent, ConsentCategory, ConsentFile
 
 
-TEXT_FRAGMENTS_SCHEMA = {
-    "$defs": {
-        "checkbox": {
+CHECKBOX = {
+    "type": "object",
+    "properties": {
+        "type": {
+            "description": "The type must be 'checkbox'.",
+            "type": "string",
+            "pattern": "checkbox",
+        },
+        "is_mandatory": {
+            "description": "This field indicates whether this text fragment is mandatory.",
+            "type": "boolean",
+        },
+        "properties": {
+            "description": "The checkbox has the following properties.",
             "type": "object",
             "properties": {
-                "type": {
-                    "description": "The type must be 'checkbox'.",
+                "text": {
+                    "description": ("This property contains the displayed text of the "
+                                    "checkbox."),
                     "type": "string",
-                    "pattern": "checkbox",
                 },
-                "is_mandatory": {
-                    "description": "This field indicates whether this text fragment is mandatory.",
+                "required": {
+                    "description": ("This property indicates whether checking the checkbox "
+                                    "is mandatory."),
                     "type": "boolean",
                 },
-                "properties": {
-                    "description": "The checkbox has the following properties.",
-                    "type": "object",
-                    "properties": {
-                        "text": {
-                            "description": ("This property contains the displayed text of the "
-                                            "checkbox."),
-                            "type": "string",
-                        },
-                        "required": {
-                            "description": ("This property indicates whether checking the checkbox "
-                                            "is mandatory."),
-                            "type": "boolean",
-                        },
-                    },
-                    "required": ["text", "required"],
-                },
             },
-            "required": ["properties", "type"],
+            "required": ["text", "required"],
+        },
+    },
+    "required": ["properties", "type"],
+}
+
+
+HEADING = {
+    "type": "object",
+    "properties": {
+        "type": {
+            "description": "The type must be 'heading'.",
+            "type": "string",
+            "pattern": "heading",
         },
-        "heading": {
+        "is_mandatory": {
+            "description": "This field indicates whether this text fragment is mandatory.",
+            "type": "boolean",
+        },
+        "properties": {
+            "description": "The heading has the following properties.",
             "type": "object",
             "properties": {
-                "type": {
-                    "description": "The type must be 'heading'.",
+                "text": {
+                    "description": ("This property contains the displayed text of the "
+                                    "heading."),
                     "type": "string",
-                    "pattern": "heading",
-                },
-                "is_mandatory": {
-                    "description": "This field indicates whether this text fragment is mandatory.",
-                    "type": "boolean",
                 },
-                "properties": {
-                    "description": "The heading has the following properties.",
-                    "type": "object",
-                    "properties": {
-                        "text": {
-                            "description": ("This property contains the displayed text of the "
-                                            "heading."),
-                            "type": "string",
-                        },
-                        "size": {
-                            "description": "This property specifies the size of the heading.",
-                            "type": "integer",
-                            "minimum": 1,
-                            "maximum": 5,
-                        },
-                    },
-                    "required": ["text", "size"],
+                "size": {
+                    "description": "This property specifies the size of the heading.",
+                    "type": "integer",
+                    "minimum": 1,
+                    "maximum": 5,
                 },
             },
-            "required": ["properties", "type"],
+            "required": ["text", "size"],
+        },
+    },
+    "required": ["properties", "type"],
+}
+
+
+MARKDOWN = {
+    "type": "object",
+    "properties": {
+        "type": {
+            "description": "The type must be 'markdown'",
+            "type": "string",
+            "pattern": "markdown",
         },
-        "markdown": {
+        "properties": {
+            "description": "The markdown text has the following properties.",
             "type": "object",
             "properties": {
-                "type": {
-                    "description": "The type must be 'markdown'",
+                "text": {
+                    "description": ("This property contains the displayed text as "
+                                    "markdown text"),
                     "type": "string",
-                    "pattern": "markdown",
-                },
-                "properties": {
-                    "description": "The markdown text has the following properties.",
-                    "type": "object",
-                    "properties": {
-                        "text": {
-                            "description": ("This property contains the displayed text as "
-                                            "markdown text"),
-                            "type": "string",
-                        },
-                    },
-                    "required": ["text"],
                 },
             },
-            "required": ["properties", "type"],
+            "required": ["text"],
         },
-        "paragraph": {
+    },
+    "required": ["properties", "type"],
+}
+
+
+PAGE_BREAK = {
+    "type": "object",
+    "properties": {
+        "type": {
+            "description": "Should force the renderer to add a page break",
+            "type": "string",
+            "pattern": "page-break",
+        },
+        "properties": {
+            "description": "This node has no properties.",
+            "type": "object",
+            "properties": {},
+        },
+    },
+    "required": ["type"],
+}
+
+
+PARAGRAPH = {
+    "type": "object",
+    "properties": {
+        "type": {
+            "description": "The type must be 'paragraph'.",
+            "type": "string",
+            "pattern": "paragraph",
+        },
+        "is_mandatory": {
+            "description": "This field indicates whether this text fragment is mandatory.",
+            "type": "boolean",
+        },
+        "properties": {
+            "decsription": "The paragraph has the following properties.",
             "type": "object",
             "properties": {
-                "type": {
-                    "description": "The type must be 'paragraph'.",
+                "text": {
+                    "description": ("This property contains the displayed text of the "
+                                    "checkbox."),
                     "type": "string",
-                    "pattern": "paragraph",
                 },
-                "is_mandatory": {
-                    "description": "This field indicates whether this text fragment is mandatory.",
+                "boldface": {
+                    "description": ("This property indicates whether the displayed text "
+                                    "will be printed in bold type."),
                     "type": "boolean",
                 },
-                "properties": {
-                    "decsription": "The paragraph has the following properties.",
-                    "type": "object",
-                    "properties": {
-                        "text": {
-                            "description": ("This property contains the displayed text of the "
-                                            "checkbox."),
-                            "type": "string",
-                        },
-                        "boldface": {
-                            "description": ("This property indicates whether the displayed text "
-                                            "will be printed in bold type."),
-                            "type": "boolean",
-                        },
-                    },
-                    "required": ["text", "boldface"],
-                },
             },
-            "required": ["properties", "type"],
+            "required": ["text", "boldface"],
         },
     },
+    "required": ["properties", "type"],
+}
+
+
+TEXT_FRAGMENTS_SCHEMA = {
+    "$defs": {
+        "checkbox": CHECKBOX,
+        "heading": HEADING,
+        "markdown": MARKDOWN,
+        "page-break": PAGE_BREAK,
+        "paragraph": PARAGRAPH,
+    },
 
     "type": "array",
     "items": {
         "anyOf": [
             {"$ref": "#/$defs/checkbox"},
             {"$ref": "#/$defs/heading"},
             {"$ref": "#/$defs/markdown"},
+            {"$ref": "#/$defs/page-break"},
             {"$ref": "#/$defs/paragraph"},
         ],
     },
     "minItems": 1,
 }
```

### Comparing `huscy.consents-0.8.0a19/huscy/consents/static/consents/css/fomantic.min.css` & `huscy.consents-0.8.0a20/huscy/consents/static/consents/css/fomantic.min.css`

 * *Files identical despite different names*

### Comparing `huscy.consents-0.8.0a19/huscy/consents/static/consents/css/fomantic2.9.0.min.css` & `huscy.consents-0.8.0a20/huscy/consents/static/consents/css/fomantic2.9.0.min.css`

 * *Files identical despite different names*

### Comparing `huscy.consents-0.8.0a19/huscy/consents/static/consents/img/logo.svg` & `huscy.consents-0.8.0a20/huscy/consents/static/consents/img/logo.svg`

 * *Files identical despite different names*

### Comparing `huscy.consents-0.8.0a19/huscy/consents/static/consents/js/fomantic.min.js` & `huscy.consents-0.8.0a20/huscy/consents/static/consents/js/fomantic.min.js`

 * *Files identical despite different names*

### Comparing `huscy.consents-0.8.0a19/huscy/consents/static/consents/js/fomantic2.9.0.min.js` & `huscy.consents-0.8.0a20/huscy/consents/static/consents/js/fomantic2.9.0.min.js`

 * *Files identical despite different names*

### Comparing `huscy.consents-0.8.0a19/huscy/consents/static/consents/js/jquery.min.js` & `huscy.consents-0.8.0a20/huscy/consents/static/consents/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `huscy.consents-0.8.0a19/huscy/consents/static/consents/js/jquery3.6.1.min.js` & `huscy.consents-0.8.0a20/huscy/consents/static/consents/js/jquery3.6.1.min.js`

 * *Files identical despite different names*

### Comparing `huscy.consents-0.8.0a19/huscy/consents/static/consents/js/popper.min.js` & `huscy.consents-0.8.0a20/huscy/consents/static/consents/js/popper.min.js`

 * *Files identical despite different names*

### Comparing `huscy.consents-0.8.0a19/huscy/consents/static/consents/js/popper1.16.1.min.js` & `huscy.consents-0.8.0a20/huscy/consents/static/consents/js/popper1.16.1.min.js`

 * *Files identical despite different names*

### Comparing `huscy.consents-0.8.0a19/huscy/consents/templates/consents/base.html` & `huscy.consents-0.8.0a20/huscy/consents/templates/consents/base.html`

 * *Files identical despite different names*

### Comparing `huscy.consents-0.8.0a19/huscy/consents/templates/consents/create_consent.html` & `huscy.consents-0.8.0a20/huscy/consents/templates/consents/create_consent.html`

 * *Files identical despite different names*

### Comparing `huscy.consents-0.8.0a19/huscy/consents/templates/consents/sign_consent.html` & `huscy.consents-0.8.0a20/huscy/consents/templates/consents/sign_consent.html`

 * *Files identical despite different names*

### Comparing `huscy.consents-0.8.0a19/huscy/consents/templates/consents/signed_consent.html` & `huscy.consents-0.8.0a20/huscy/consents/templates/consents/signed_consent.html`

 * *Files identical despite different names*

### Comparing `huscy.consents-0.8.0a19/huscy/consents/views.py` & `huscy.consents-0.8.0a20/huscy/consents/views.py`

 * *Files identical despite different names*

### Comparing `huscy.consents-0.8.0a19/huscy/consents/viewsets.py` & `huscy.consents-0.8.0a20/huscy/consents/viewsets.py`

 * *Files identical despite different names*

### Comparing `huscy.consents-0.8.0a19/huscy.consents.egg-info/PKG-INFO` & `huscy.consents-0.8.0a20/huscy.consents.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: huscy.consents
-Version: 0.8.0a19
+Version: 0.8.0a20
 Summary: consents
 Home-page: https://bitbucket.org/huscy/consents
 Author: Gefan Qian, Stefan Bunde
 Author-email: gefan.qian@gmail.com, stefanbunde+git@posteo.de
 License: AGPLv3+
 Description: # huscy.consents
```

### Comparing `huscy.consents-0.8.0a19/huscy.consents.egg-info/SOURCES.txt` & `huscy.consents-0.8.0a20/huscy.consents.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `huscy.consents-0.8.0a19/setup.py` & `huscy.consents-0.8.0a20/setup.py`

 * *Files identical despite different names*

