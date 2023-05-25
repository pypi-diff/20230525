# Comparing `tmp/django-listable-0.8.0.tar.gz` & `tmp/django-listable-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-listable-0.8.0.tar", last modified: Tue Apr 18 13:35:56 2023, max compression
+gzip compressed data, was "django-listable-0.8.1.tar", last modified: Thu May 25 15:06:17 2023, max compression
```

## Comparing `django-listable-0.8.0.tar` & `django-listable-0.8.1.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxrwxr-x   0 randlet   (1000) randlet   (1000)        0 2023-04-18 13:35:56.299035 django-listable-0.8.0/
--rw-r--r--   0 randlet   (1000) randlet   (1000)      161 2022-05-16 05:54:23.000000 django-listable-0.8.0/AUTHORS.rst
--rw-r--r--   0 randlet   (1000) randlet   (1000)     3279 2022-05-16 05:54:23.000000 django-listable-0.8.0/CONTRIBUTING.rst
--rw-rw-r--   0 randlet   (1000) randlet   (1000)     2410 2023-04-18 13:33:01.000000 django-listable-0.8.0/HISTORY.rst
--rw-r--r--   0 randlet   (1000) randlet   (1000)     1478 2022-05-16 05:54:23.000000 django-listable-0.8.0/LICENSE
--rw-r--r--   0 randlet   (1000) randlet   (1000)      176 2022-05-16 05:54:23.000000 django-listable-0.8.0/MANIFEST.in
--rw-rw-r--   0 randlet   (1000) randlet   (1000)    20049 2023-04-18 13:35:56.299035 django-listable-0.8.0/PKG-INFO
--rw-rw-r--   0 randlet   (1000) randlet   (1000)    16896 2023-04-18 13:33:01.000000 django-listable-0.8.0/README.rst
-drwxrwxr-x   0 randlet   (1000) randlet   (1000)        0 2023-04-18 13:35:56.291036 django-listable-0.8.0/django_listable.egg-info/
--rw-r--r--   0 randlet   (1000) randlet   (1000)    20049 2023-04-18 13:35:56.000000 django-listable-0.8.0/django_listable.egg-info/PKG-INFO
--rw-r--r--   0 randlet   (1000) randlet   (1000)     2404 2023-04-18 13:35:56.000000 django-listable-0.8.0/django_listable.egg-info/SOURCES.txt
--rw-r--r--   0 randlet   (1000) randlet   (1000)        1 2023-04-18 13:35:56.000000 django-listable-0.8.0/django_listable.egg-info/dependency_links.txt
--rw-r--r--   0 randlet   (1000) randlet   (1000)        1 2022-05-16 05:54:23.000000 django-listable-0.8.0/django_listable.egg-info/not-zip-safe
--rw-r--r--   0 randlet   (1000) randlet   (1000)        9 2023-04-18 13:35:56.000000 django-listable-0.8.0/django_listable.egg-info/top_level.txt
-drwxrwxr-x   0 randlet   (1000) randlet   (1000)        0 2023-04-18 13:35:56.291036 django-listable-0.8.0/listable/
--rw-rw-r--   0 randlet   (1000) randlet   (1000)       22 2023-04-18 13:33:01.000000 django-listable-0.8.0/listable/__init__.py
--rw-r--r--   0 randlet   (1000) randlet   (1000)       24 2022-05-16 05:54:23.000000 django-listable-0.8.0/listable/models.py
--rw-r--r--   0 randlet   (1000) randlet   (1000)      993 2022-05-16 05:54:23.000000 django-listable-0.8.0/listable/settings.py
-drwxrwxr-x   0 randlet   (1000) randlet   (1000)        0 2023-04-18 13:35:56.287036 django-listable-0.8.0/listable/static/
-drwxrwxr-x   0 randlet   (1000) randlet   (1000)        0 2023-04-18 13:35:56.287036 django-listable-0.8.0/listable/static/listable/
-drwxrwxr-x   0 randlet   (1000) randlet   (1000)        0 2023-04-18 13:35:56.291036 django-listable-0.8.0/listable/static/listable/css/
--rw-r--r--   0 randlet   (1000) randlet   (1000)    15809 2022-05-16 05:54:23.000000 django-listable-0.8.0/listable/static/listable/css/bootstrap-datepicker.min.css
--rw-r--r--   0 randlet   (1000) randlet   (1000)     1148 2022-05-16 05:54:23.000000 django-listable-0.8.0/listable/static/listable/css/bootstrap.multiselect.css
--rw-r--r--   0 randlet   (1000) randlet   (1000)     8133 2022-05-16 05:54:23.000000 django-listable-0.8.0/listable/static/listable/css/daterangepicker.css
--rw-r--r--   0 randlet   (1000) randlet   (1000)     1765 2022-05-16 05:54:23.000000 django-listable-0.8.0/listable/static/listable/css/demo_page.css
--rw-r--r--   0 randlet   (1000) randlet   (1000)    10732 2022-05-16 05:54:23.000000 django-listable-0.8.0/listable/static/listable/css/demo_table.css
--rw-r--r--   0 randlet   (1000) randlet   (1000)     8446 2022-05-16 05:54:23.000000 django-listable-0.8.0/listable/static/listable/css/demo_table_jui.css
--rw-r--r--   0 randlet   (1000) randlet   (1000)    29063 2022-05-16 05:54:23.000000 django-listable-0.8.0/listable/static/listable/css/font-awesome.min.css
--rw-r--r--   0 randlet   (1000) randlet   (1000)     1115 2022-05-16 05:54:23.000000 django-listable-0.8.0/listable/static/listable/css/jquery.dataTables.bootstrap.css
--rw-r--r--   0 randlet   (1000) randlet   (1000)     4520 2022-05-16 05:54:23.000000 django-listable-0.8.0/listable/static/listable/css/jquery.dataTables.css
--rw-r--r--   0 randlet   (1000) randlet   (1000)     4541 2022-05-16 05:54:23.000000 django-listable-0.8.0/listable/static/listable/css/jquery.dataTables_themeroller.css
--rw-r--r--   0 randlet   (1000) randlet   (1000)      499 2022-05-16 05:54:23.000000 django-listable-0.8.0/listable/static/listable/css/listable.css
-drwxrwxr-x   0 randlet   (1000) randlet   (1000)        0 2023-04-18 13:35:56.291036 django-listable-0.8.0/listable/static/listable/fonts/
--rw-r--r--   0 randlet   (1000) randlet   (1000)   391622 2022-05-16 05:54:23.000000 django-listable-0.8.0/listable/static/listable/fonts/fontawesome-webfont.svg
-drwxrwxr-x   0 randlet   (1000) randlet   (1000)        0 2023-04-18 13:35:56.291036 django-listable-0.8.0/listable/static/listable/img/
--rw-r--r--   0 randlet   (1000) randlet   (1000)     1361 2022-05-16 05:54:23.000000 django-listable-0.8.0/listable/static/listable/img/back_disabled.png
--rw-r--r--   0 randlet   (1000) randlet   (1000)     1379 2022-05-16 05:54:23.000000 django-listable-0.8.0/listable/static/listable/img/back_enabled.png
--rw-r--r--   0 randlet   (1000) randlet   (1000)     1375 2022-05-16 05:54:23.000000 django-listable-0.8.0/listable/static/listable/img/back_enabled_hover.png
--rw-r--r--   0 randlet   (1000) randlet   (1000)     1363 2022-05-16 05:54:23.000000 django-listable-0.8.0/listable/static/listable/img/forward_disabled.png
--rw-r--r--   0 randlet   (1000) randlet   (1000)     1380 2022-05-16 05:54:23.000000 django-listable-0.8.0/listable/static/listable/img/forward_enabled.png
--rw-r--r--   0 randlet   (1000) randlet   (1000)     1379 2022-05-16 05:54:23.000000 django-listable-0.8.0/listable/static/listable/img/forward_enabled_hover.png
--rw-r--r--   0 randlet   (1000) randlet   (1000)     1118 2022-05-16 05:54:23.000000 django-listable-0.8.0/listable/static/listable/img/sort_asc.png
--rw-r--r--   0 randlet   (1000) randlet   (1000)     1050 2022-05-16 05:54:23.000000 django-listable-0.8.0/listable/static/listable/img/sort_asc_disabled.png
--rw-r--r--   0 randlet   (1000) randlet   (1000)     1136 2022-05-16 05:54:23.000000 django-listable-0.8.0/listable/static/listable/img/sort_both.png
--rw-r--r--   0 randlet   (1000) randlet   (1000)     1127 2022-05-16 05:54:23.000000 django-listable-0.8.0/listable/static/listable/img/sort_desc.png
--rw-r--r--   0 randlet   (1000) randlet   (1000)     1045 2022-05-16 05:54:23.000000 django-listable-0.8.0/listable/static/listable/img/sort_desc_disabled.png
-drwxrwxr-x   0 randlet   (1000) randlet   (1000)        0 2023-04-18 13:35:56.299035 django-listable-0.8.0/listable/static/listable/js/
--rw-r--r--   0 randlet   (1000) randlet   (1000)    34174 2022-05-16 05:54:23.000000 django-listable-0.8.0/listable/static/listable/js/bootstrap-datepicker.min.js
--rw-r--r--   0 randlet   (1000) randlet   (1000)    63315 2022-05-16 05:54:23.000000 django-listable-0.8.0/listable/static/listable/js/bootstrap.multiselect.js
--rw-r--r--   0 randlet   (1000) randlet   (1000)    68583 2022-05-16 05:54:23.000000 django-listable-0.8.0/listable/static/listable/js/daterangepicker.js
--rw-r--r--   0 randlet   (1000) randlet   (1000)     6316 2022-05-16 05:54:23.000000 django-listable-0.8.0/listable/static/listable/js/jquery.dataTables.bootstrap.js
--rw-r--r--   0 randlet   (1000) randlet   (1000)    34181 2022-05-16 05:54:23.000000 django-listable-0.8.0/listable/static/listable/js/jquery.dataTables.columnFilter.js
--rw-r--r--   0 randlet   (1000) randlet   (1000)   373929 2022-05-16 05:54:23.000000 django-listable-0.8.0/listable/static/listable/js/jquery.dataTables.js
--rw-r--r--   0 randlet   (1000) randlet   (1000)    70879 2022-05-16 05:54:23.000000 django-listable-0.8.0/listable/static/listable/js/jquery.dataTables.min.js
--rw-r--r--   0 randlet   (1000) randlet   (1000)     1628 2022-05-16 05:54:23.000000 django-listable-0.8.0/listable/static/listable/js/jquery.dataTables.searchPlugins.js
--rw-r--r--   0 randlet   (1000) randlet   (1000)     4782 2022-05-16 05:54:23.000000 django-listable-0.8.0/listable/static/listable/js/jquery.dataTables.sort.js
--rw-r--r--   0 randlet   (1000) randlet   (1000)    93434 2022-05-16 05:54:23.000000 django-listable-0.8.0/listable/static/listable/js/jquery.js
--rw-r--r--   0 randlet   (1000) randlet   (1000)    11927 2022-05-16 05:54:23.000000 django-listable-0.8.0/listable/static/listable/js/listable.js
--rw-r--r--   0 randlet   (1000) randlet   (1000)   134906 2022-05-16 05:54:23.000000 django-listable-0.8.0/listable/static/listable/js/moment.js
--rw-r--r--   0 randlet   (1000) randlet   (1000)    46645 2022-05-16 05:54:23.000000 django-listable-0.8.0/listable/static/listable/js/moment.min.js
-drwxrwxr-x   0 randlet   (1000) randlet   (1000)        0 2023-04-18 13:35:56.287036 django-listable-0.8.0/listable/templates/
-drwxrwxr-x   0 randlet   (1000) randlet   (1000)        0 2023-04-18 13:35:56.299035 django-listable-0.8.0/listable/templates/listable/
--rw-r--r--   0 randlet   (1000) randlet   (1000)      712 2022-05-16 05:54:23.000000 django-listable-0.8.0/listable/templates/listable/_table.html
--rw-r--r--   0 randlet   (1000) randlet   (1000)      662 2022-05-16 05:54:23.000000 django-listable-0.8.0/listable/templates/listable/base.html
-drwxrwxr-x   0 randlet   (1000) randlet   (1000)        0 2023-04-18 13:35:56.299035 django-listable-0.8.0/listable/templatetags/
--rw-r--r--   0 randlet   (1000) randlet   (1000)        0 2022-05-16 05:54:23.000000 django-listable-0.8.0/listable/templatetags/__init__.py
--rw-r--r--   0 randlet   (1000) randlet   (1000)     8762 2022-10-03 20:43:12.000000 django-listable-0.8.0/listable/templatetags/listable.py
--rw-r--r--   0 randlet   (1000) randlet   (1000)     2105 2022-05-16 05:54:23.000000 django-listable-0.8.0/listable/utils.py
--rw-rw-r--   0 randlet   (1000) randlet   (1000)    20434 2023-04-18 13:33:01.000000 django-listable-0.8.0/listable/views.py
--rw-rw-r--   0 randlet   (1000) randlet   (1000)       68 2023-04-18 13:35:56.299035 django-listable-0.8.0/setup.cfg
--rw-rw-r--   0 randlet   (1000) randlet   (1000)     1608 2023-04-18 13:33:01.000000 django-listable-0.8.0/setup.py
-drwxrwxr-x   0 randlet   (1000) randlet   (1000)        0 2023-04-18 13:35:56.299035 django-listable-0.8.0/tests/
--rw-r--r--   0 randlet   (1000) randlet   (1000)     1129 2022-05-16 05:54:23.000000 django-listable-0.8.0/tests/test_tags.py
--rw-r--r--   0 randlet   (1000) randlet   (1000)      543 2022-05-16 05:54:23.000000 django-listable-0.8.0/tests/test_utils.py
--rw-rw-r--   0 randlet   (1000) randlet   (1000)    16228 2023-04-18 13:33:01.000000 django-listable-0.8.0/tests/test_views.py
--rw-r--r--   0 randlet   (1000) randlet   (1000)      136 2022-05-16 05:54:23.000000 django-listable-0.8.0/tests/tests.py
+drwxrwxr-x   0 randlet   (1000) randlet   (1000)        0 2023-05-25 15:06:17.524935 django-listable-0.8.1/
+-rw-r--r--   0 randlet   (1000) randlet   (1000)      161 2022-05-16 05:54:23.000000 django-listable-0.8.1/AUTHORS.rst
+-rw-r--r--   0 randlet   (1000) randlet   (1000)     3279 2022-05-16 05:54:23.000000 django-listable-0.8.1/CONTRIBUTING.rst
+-rw-rw-r--   0 randlet   (1000) randlet   (1000)     2650 2023-05-25 15:04:12.000000 django-listable-0.8.1/HISTORY.rst
+-rw-r--r--   0 randlet   (1000) randlet   (1000)     1478 2022-05-16 05:54:23.000000 django-listable-0.8.1/LICENSE
+-rw-r--r--   0 randlet   (1000) randlet   (1000)      176 2022-05-16 05:54:23.000000 django-listable-0.8.1/MANIFEST.in
+-rw-rw-r--   0 randlet   (1000) randlet   (1000)    20289 2023-05-25 15:06:17.524935 django-listable-0.8.1/PKG-INFO
+-rw-rw-r--   0 randlet   (1000) randlet   (1000)    16896 2023-04-18 13:33:01.000000 django-listable-0.8.1/README.rst
+drwxrwxr-x   0 randlet   (1000) randlet   (1000)        0 2023-05-25 15:06:17.520935 django-listable-0.8.1/django_listable.egg-info/
+-rw-r--r--   0 randlet   (1000) randlet   (1000)    20289 2023-05-25 15:06:17.000000 django-listable-0.8.1/django_listable.egg-info/PKG-INFO
+-rw-r--r--   0 randlet   (1000) randlet   (1000)     2404 2023-05-25 15:06:17.000000 django-listable-0.8.1/django_listable.egg-info/SOURCES.txt
+-rw-r--r--   0 randlet   (1000) randlet   (1000)        1 2023-05-25 15:06:17.000000 django-listable-0.8.1/django_listable.egg-info/dependency_links.txt
+-rw-r--r--   0 randlet   (1000) randlet   (1000)        1 2022-05-16 05:54:23.000000 django-listable-0.8.1/django_listable.egg-info/not-zip-safe
+-rw-r--r--   0 randlet   (1000) randlet   (1000)        9 2023-05-25 15:06:17.000000 django-listable-0.8.1/django_listable.egg-info/top_level.txt
+drwxrwxr-x   0 randlet   (1000) randlet   (1000)        0 2023-05-25 15:06:17.520935 django-listable-0.8.1/listable/
+-rw-rw-r--   0 randlet   (1000) randlet   (1000)       22 2023-05-25 15:05:05.000000 django-listable-0.8.1/listable/__init__.py
+-rw-r--r--   0 randlet   (1000) randlet   (1000)       24 2022-05-16 05:54:23.000000 django-listable-0.8.1/listable/models.py
+-rw-r--r--   0 randlet   (1000) randlet   (1000)      993 2022-05-16 05:54:23.000000 django-listable-0.8.1/listable/settings.py
+drwxrwxr-x   0 randlet   (1000) randlet   (1000)        0 2023-05-25 15:06:17.516935 django-listable-0.8.1/listable/static/
+drwxrwxr-x   0 randlet   (1000) randlet   (1000)        0 2023-05-25 15:06:17.516935 django-listable-0.8.1/listable/static/listable/
+drwxrwxr-x   0 randlet   (1000) randlet   (1000)        0 2023-05-25 15:06:17.520935 django-listable-0.8.1/listable/static/listable/css/
+-rw-r--r--   0 randlet   (1000) randlet   (1000)    15809 2022-05-16 05:54:23.000000 django-listable-0.8.1/listable/static/listable/css/bootstrap-datepicker.min.css
+-rw-r--r--   0 randlet   (1000) randlet   (1000)     1148 2022-05-16 05:54:23.000000 django-listable-0.8.1/listable/static/listable/css/bootstrap.multiselect.css
+-rw-r--r--   0 randlet   (1000) randlet   (1000)     8133 2022-05-16 05:54:23.000000 django-listable-0.8.1/listable/static/listable/css/daterangepicker.css
+-rw-r--r--   0 randlet   (1000) randlet   (1000)     1765 2022-05-16 05:54:23.000000 django-listable-0.8.1/listable/static/listable/css/demo_page.css
+-rw-r--r--   0 randlet   (1000) randlet   (1000)    10732 2022-05-16 05:54:23.000000 django-listable-0.8.1/listable/static/listable/css/demo_table.css
+-rw-r--r--   0 randlet   (1000) randlet   (1000)     8446 2022-05-16 05:54:23.000000 django-listable-0.8.1/listable/static/listable/css/demo_table_jui.css
+-rw-r--r--   0 randlet   (1000) randlet   (1000)    29063 2022-05-16 05:54:23.000000 django-listable-0.8.1/listable/static/listable/css/font-awesome.min.css
+-rw-r--r--   0 randlet   (1000) randlet   (1000)     1115 2022-05-16 05:54:23.000000 django-listable-0.8.1/listable/static/listable/css/jquery.dataTables.bootstrap.css
+-rw-r--r--   0 randlet   (1000) randlet   (1000)     4520 2022-05-16 05:54:23.000000 django-listable-0.8.1/listable/static/listable/css/jquery.dataTables.css
+-rw-r--r--   0 randlet   (1000) randlet   (1000)     4541 2022-05-16 05:54:23.000000 django-listable-0.8.1/listable/static/listable/css/jquery.dataTables_themeroller.css
+-rw-r--r--   0 randlet   (1000) randlet   (1000)      499 2022-05-16 05:54:23.000000 django-listable-0.8.1/listable/static/listable/css/listable.css
+drwxrwxr-x   0 randlet   (1000) randlet   (1000)        0 2023-05-25 15:06:17.520935 django-listable-0.8.1/listable/static/listable/fonts/
+-rw-r--r--   0 randlet   (1000) randlet   (1000)   391622 2022-05-16 05:54:23.000000 django-listable-0.8.1/listable/static/listable/fonts/fontawesome-webfont.svg
+drwxrwxr-x   0 randlet   (1000) randlet   (1000)        0 2023-05-25 15:06:17.520935 django-listable-0.8.1/listable/static/listable/img/
+-rw-r--r--   0 randlet   (1000) randlet   (1000)     1361 2022-05-16 05:54:23.000000 django-listable-0.8.1/listable/static/listable/img/back_disabled.png
+-rw-r--r--   0 randlet   (1000) randlet   (1000)     1379 2022-05-16 05:54:23.000000 django-listable-0.8.1/listable/static/listable/img/back_enabled.png
+-rw-r--r--   0 randlet   (1000) randlet   (1000)     1375 2022-05-16 05:54:23.000000 django-listable-0.8.1/listable/static/listable/img/back_enabled_hover.png
+-rw-r--r--   0 randlet   (1000) randlet   (1000)     1363 2022-05-16 05:54:23.000000 django-listable-0.8.1/listable/static/listable/img/forward_disabled.png
+-rw-r--r--   0 randlet   (1000) randlet   (1000)     1380 2022-05-16 05:54:23.000000 django-listable-0.8.1/listable/static/listable/img/forward_enabled.png
+-rw-r--r--   0 randlet   (1000) randlet   (1000)     1379 2022-05-16 05:54:23.000000 django-listable-0.8.1/listable/static/listable/img/forward_enabled_hover.png
+-rw-r--r--   0 randlet   (1000) randlet   (1000)     1118 2022-05-16 05:54:23.000000 django-listable-0.8.1/listable/static/listable/img/sort_asc.png
+-rw-r--r--   0 randlet   (1000) randlet   (1000)     1050 2022-05-16 05:54:23.000000 django-listable-0.8.1/listable/static/listable/img/sort_asc_disabled.png
+-rw-r--r--   0 randlet   (1000) randlet   (1000)     1136 2022-05-16 05:54:23.000000 django-listable-0.8.1/listable/static/listable/img/sort_both.png
+-rw-r--r--   0 randlet   (1000) randlet   (1000)     1127 2022-05-16 05:54:23.000000 django-listable-0.8.1/listable/static/listable/img/sort_desc.png
+-rw-r--r--   0 randlet   (1000) randlet   (1000)     1045 2022-05-16 05:54:23.000000 django-listable-0.8.1/listable/static/listable/img/sort_desc_disabled.png
+drwxrwxr-x   0 randlet   (1000) randlet   (1000)        0 2023-05-25 15:06:17.524935 django-listable-0.8.1/listable/static/listable/js/
+-rw-r--r--   0 randlet   (1000) randlet   (1000)    34174 2022-05-16 05:54:23.000000 django-listable-0.8.1/listable/static/listable/js/bootstrap-datepicker.min.js
+-rw-r--r--   0 randlet   (1000) randlet   (1000)    63315 2022-05-16 05:54:23.000000 django-listable-0.8.1/listable/static/listable/js/bootstrap.multiselect.js
+-rw-r--r--   0 randlet   (1000) randlet   (1000)    68583 2022-05-16 05:54:23.000000 django-listable-0.8.1/listable/static/listable/js/daterangepicker.js
+-rw-r--r--   0 randlet   (1000) randlet   (1000)     6316 2022-05-16 05:54:23.000000 django-listable-0.8.1/listable/static/listable/js/jquery.dataTables.bootstrap.js
+-rw-r--r--   0 randlet   (1000) randlet   (1000)    34183 2023-05-25 14:58:15.000000 django-listable-0.8.1/listable/static/listable/js/jquery.dataTables.columnFilter.js
+-rw-r--r--   0 randlet   (1000) randlet   (1000)   373929 2022-05-16 05:54:23.000000 django-listable-0.8.1/listable/static/listable/js/jquery.dataTables.js
+-rw-r--r--   0 randlet   (1000) randlet   (1000)    70879 2022-05-16 05:54:23.000000 django-listable-0.8.1/listable/static/listable/js/jquery.dataTables.min.js
+-rw-r--r--   0 randlet   (1000) randlet   (1000)     1628 2022-05-16 05:54:23.000000 django-listable-0.8.1/listable/static/listable/js/jquery.dataTables.searchPlugins.js
+-rw-r--r--   0 randlet   (1000) randlet   (1000)     4782 2022-05-16 05:54:23.000000 django-listable-0.8.1/listable/static/listable/js/jquery.dataTables.sort.js
+-rw-r--r--   0 randlet   (1000) randlet   (1000)    93434 2022-05-16 05:54:23.000000 django-listable-0.8.1/listable/static/listable/js/jquery.js
+-rw-r--r--   0 randlet   (1000) randlet   (1000)    11927 2022-05-16 05:54:23.000000 django-listable-0.8.1/listable/static/listable/js/listable.js
+-rw-r--r--   0 randlet   (1000) randlet   (1000)   134906 2022-05-16 05:54:23.000000 django-listable-0.8.1/listable/static/listable/js/moment.js
+-rw-r--r--   0 randlet   (1000) randlet   (1000)    46645 2022-05-16 05:54:23.000000 django-listable-0.8.1/listable/static/listable/js/moment.min.js
+drwxrwxr-x   0 randlet   (1000) randlet   (1000)        0 2023-05-25 15:06:17.516935 django-listable-0.8.1/listable/templates/
+drwxrwxr-x   0 randlet   (1000) randlet   (1000)        0 2023-05-25 15:06:17.524935 django-listable-0.8.1/listable/templates/listable/
+-rw-r--r--   0 randlet   (1000) randlet   (1000)      712 2022-05-16 05:54:23.000000 django-listable-0.8.1/listable/templates/listable/_table.html
+-rw-r--r--   0 randlet   (1000) randlet   (1000)      662 2022-05-16 05:54:23.000000 django-listable-0.8.1/listable/templates/listable/base.html
+drwxrwxr-x   0 randlet   (1000) randlet   (1000)        0 2023-05-25 15:06:17.524935 django-listable-0.8.1/listable/templatetags/
+-rw-r--r--   0 randlet   (1000) randlet   (1000)        0 2022-05-16 05:54:23.000000 django-listable-0.8.1/listable/templatetags/__init__.py
+-rw-r--r--   0 randlet   (1000) randlet   (1000)     8762 2022-10-03 20:43:12.000000 django-listable-0.8.1/listable/templatetags/listable.py
+-rw-r--r--   0 randlet   (1000) randlet   (1000)     2105 2022-05-16 05:54:23.000000 django-listable-0.8.1/listable/utils.py
+-rw-rw-r--   0 randlet   (1000) randlet   (1000)    20436 2023-05-25 14:58:39.000000 django-listable-0.8.1/listable/views.py
+-rw-rw-r--   0 randlet   (1000) randlet   (1000)       68 2023-05-25 15:06:17.524935 django-listable-0.8.1/setup.cfg
+-rw-rw-r--   0 randlet   (1000) randlet   (1000)     1608 2023-05-25 15:04:29.000000 django-listable-0.8.1/setup.py
+drwxrwxr-x   0 randlet   (1000) randlet   (1000)        0 2023-05-25 15:06:17.524935 django-listable-0.8.1/tests/
+-rw-r--r--   0 randlet   (1000) randlet   (1000)     1129 2022-05-16 05:54:23.000000 django-listable-0.8.1/tests/test_tags.py
+-rw-r--r--   0 randlet   (1000) randlet   (1000)      543 2022-05-16 05:54:23.000000 django-listable-0.8.1/tests/test_utils.py
+-rw-rw-r--   0 randlet   (1000) randlet   (1000)    16228 2023-04-18 13:33:01.000000 django-listable-0.8.1/tests/test_views.py
+-rw-r--r--   0 randlet   (1000) randlet   (1000)      136 2022-05-16 05:54:23.000000 django-listable-0.8.1/tests/tests.py
```

### Comparing `django-listable-0.8.0/CONTRIBUTING.rst` & `django-listable-0.8.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `django-listable-0.8.0/HISTORY.rst` & `django-listable-0.8.1/HISTORY.rst`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,20 @@
 .. :changelog:
 
 =======
 History
 =======
 
+0.8.1 (2023-05-25)
+------------------
+
+* In order to allow ``|`` characters in searches, the search term separator for
+  multi selects has been updated to use ```|``` which is a 3 character sequence
+  unlikely to apply in normal searches.
+
 0.8.0 (2023-04-18)
 ------------------
 
 * Added a loose_text_search setting to views.  Set ``loose_text_search = True``
   on your view to enable partial matching in your text searches. For example
   "Fo Ba" will match "Foo Bar".
```

### Comparing `django-listable-0.8.0/LICENSE` & `django-listable-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-listable-0.8.0/PKG-INFO` & `django-listable-0.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-listable
-Version: 0.8.0
+Version: 0.8.1
 Summary: A reusable Django app to make integrations with the DataTables javascript library easy.
 Home-page: https://github.com/randlet/django-listable
 Author: Randle Taylor
 Author-email: randle.taylor@gmail.com
 License: BSD
 Keywords: django-listable
 Classifier: Development Status :: 4 - Beta
@@ -631,14 +631,21 @@
 
 
 
 =======
 History
 =======
 
+0.8.1 (2023-05-25)
+------------------
+
+* In order to allow ``|`` characters in searches, the search term separator for
+  multi selects has been updated to use ```|``` which is a 3 character sequence
+  unlikely to apply in normal searches.
+
 0.8.0 (2023-04-18)
 ------------------
 
 * Added a loose_text_search setting to views.  Set ``loose_text_search = True``
   on your view to enable partial matching in your text searches. For example
   "Fo Ba" will match "Foo Bar".
```

### Comparing `django-listable-0.8.0/README.rst` & `django-listable-0.8.1/README.rst`

 * *Files identical despite different names*

### Comparing `django-listable-0.8.0/django_listable.egg-info/PKG-INFO` & `django-listable-0.8.1/django_listable.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-listable
-Version: 0.8.0
+Version: 0.8.1
 Summary: A reusable Django app to make integrations with the DataTables javascript library easy.
 Home-page: https://github.com/randlet/django-listable
 Author: Randle Taylor
 Author-email: randle.taylor@gmail.com
 License: BSD
 Keywords: django-listable
 Classifier: Development Status :: 4 - Beta
@@ -631,14 +631,21 @@
 
 
 
 =======
 History
 =======
 
+0.8.1 (2023-05-25)
+------------------
+
+* In order to allow ``|`` characters in searches, the search term separator for
+  multi selects has been updated to use ```|``` which is a 3 character sequence
+  unlikely to apply in normal searches.
+
 0.8.0 (2023-04-18)
 ------------------
 
 * Added a loose_text_search setting to views.  Set ``loose_text_search = True``
   on your view to enable partial matching in your text searches. For example
   "Fo Ba" will match "Foo Bar".
```

### Comparing `django-listable-0.8.0/django_listable.egg-info/SOURCES.txt` & `django-listable-0.8.1/django_listable.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-listable-0.8.0/listable/settings.py` & `django-listable-0.8.1/listable/settings.py`

 * *Files identical despite different names*

### Comparing `django-listable-0.8.0/listable/static/listable/css/bootstrap-datepicker.min.css` & `django-listable-0.8.1/listable/static/listable/css/bootstrap-datepicker.min.css`

 * *Files identical despite different names*

### Comparing `django-listable-0.8.0/listable/static/listable/css/bootstrap.multiselect.css` & `django-listable-0.8.1/listable/static/listable/css/bootstrap.multiselect.css`

 * *Files identical despite different names*

### Comparing `django-listable-0.8.0/listable/static/listable/css/daterangepicker.css` & `django-listable-0.8.1/listable/static/listable/css/daterangepicker.css`

 * *Files identical despite different names*

### Comparing `django-listable-0.8.0/listable/static/listable/css/demo_page.css` & `django-listable-0.8.1/listable/static/listable/css/demo_page.css`

 * *Files identical despite different names*

### Comparing `django-listable-0.8.0/listable/static/listable/css/demo_table.css` & `django-listable-0.8.1/listable/static/listable/css/demo_table.css`

 * *Files identical despite different names*

### Comparing `django-listable-0.8.0/listable/static/listable/css/demo_table_jui.css` & `django-listable-0.8.1/listable/static/listable/css/demo_table_jui.css`

 * *Files identical despite different names*

### Comparing `django-listable-0.8.0/listable/static/listable/css/font-awesome.min.css` & `django-listable-0.8.1/listable/static/listable/css/font-awesome.min.css`

 * *Files identical despite different names*

### Comparing `django-listable-0.8.0/listable/static/listable/css/jquery.dataTables.bootstrap.css` & `django-listable-0.8.1/listable/static/listable/css/jquery.dataTables.bootstrap.css`

 * *Files identical despite different names*

### Comparing `django-listable-0.8.0/listable/static/listable/css/jquery.dataTables.css` & `django-listable-0.8.1/listable/static/listable/css/jquery.dataTables.css`

 * *Files identical despite different names*

### Comparing `django-listable-0.8.0/listable/static/listable/css/jquery.dataTables_themeroller.css` & `django-listable-0.8.1/listable/static/listable/css/jquery.dataTables_themeroller.css`

 * *Files identical despite different names*

### Comparing `django-listable-0.8.0/listable/static/listable/fonts/fontawesome-webfont.svg` & `django-listable-0.8.1/listable/static/listable/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `django-listable-0.8.0/listable/static/listable/img/back_disabled.png` & `django-listable-0.8.1/listable/static/listable/img/back_disabled.png`

 * *Files identical despite different names*

### Comparing `django-listable-0.8.0/listable/static/listable/img/back_enabled.png` & `django-listable-0.8.1/listable/static/listable/img/back_enabled.png`

 * *Files identical despite different names*

### Comparing `django-listable-0.8.0/listable/static/listable/img/back_enabled_hover.png` & `django-listable-0.8.1/listable/static/listable/img/back_enabled_hover.png`

 * *Files identical despite different names*

### Comparing `django-listable-0.8.0/listable/static/listable/img/forward_disabled.png` & `django-listable-0.8.1/listable/static/listable/img/forward_disabled.png`

 * *Files identical despite different names*

### Comparing `django-listable-0.8.0/listable/static/listable/img/forward_enabled.png` & `django-listable-0.8.1/listable/static/listable/img/forward_enabled.png`

 * *Files identical despite different names*

### Comparing `django-listable-0.8.0/listable/static/listable/img/forward_enabled_hover.png` & `django-listable-0.8.1/listable/static/listable/img/forward_enabled_hover.png`

 * *Files identical despite different names*

### Comparing `django-listable-0.8.0/listable/static/listable/img/sort_asc.png` & `django-listable-0.8.1/listable/static/listable/img/sort_asc.png`

 * *Files identical despite different names*

### Comparing `django-listable-0.8.0/listable/static/listable/img/sort_asc_disabled.png` & `django-listable-0.8.1/listable/static/listable/img/sort_asc_disabled.png`

 * *Files identical despite different names*

### Comparing `django-listable-0.8.0/listable/static/listable/img/sort_both.png` & `django-listable-0.8.1/listable/static/listable/img/sort_both.png`

 * *Files identical despite different names*

### Comparing `django-listable-0.8.0/listable/static/listable/img/sort_desc.png` & `django-listable-0.8.1/listable/static/listable/img/sort_desc.png`

 * *Files identical despite different names*

### Comparing `django-listable-0.8.0/listable/static/listable/img/sort_desc_disabled.png` & `django-listable-0.8.1/listable/static/listable/img/sort_desc_disabled.png`

 * *Files identical despite different names*

### Comparing `django-listable-0.8.0/listable/static/listable/js/bootstrap-datepicker.min.js` & `django-listable-0.8.1/listable/static/listable/js/bootstrap-datepicker.min.js`

 * *Files identical despite different names*

### Comparing `django-listable-0.8.0/listable/static/listable/js/bootstrap.multiselect.js` & `django-listable-0.8.1/listable/static/listable/js/bootstrap.multiselect.js`

 * *Files identical despite different names*

### Comparing `django-listable-0.8.0/listable/static/listable/js/daterangepicker.js` & `django-listable-0.8.1/listable/static/listable/js/daterangepicker.js`

 * *Files identical despite different names*

### Comparing `django-listable-0.8.0/listable/static/listable/js/jquery.dataTables.bootstrap.js` & `django-listable-0.8.1/listable/static/listable/js/jquery.dataTables.bootstrap.js`

 * *Files identical despite different names*

### Comparing `django-listable-0.8.0/listable/static/listable/js/jquery.dataTables.columnFilter.js` & `django-listable-0.8.1/listable/static/listable/js/jquery.dataTables.columnFilter.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -386,15 +386,15 @@
                     var asEscapedFilters = [];
                     if (selectedOptions == null || selectedOptions == []) {
                         var re = '^(.*)$';
                     } else {
                         $.each(selectedOptions, function(i, sFilter) {
                             asEscapedFilters.push(fnRegExpEscape(sFilter));
                         });
-                        var re = '^(' + asEscapedFilters.join('|') + ')$';
+                        var re = '^(' + asEscapedFilters.join('`|`') + ')$';
                     }
 
                     oTable.fnFilter(re, index, true, false);
                 });
             } else {
                 select.change(function() {
                     //var val = $(this).val();
```

### Comparing `django-listable-0.8.0/listable/static/listable/js/jquery.dataTables.js` & `django-listable-0.8.1/listable/static/listable/js/jquery.dataTables.js`

 * *Files identical despite different names*

### Comparing `django-listable-0.8.0/listable/static/listable/js/jquery.dataTables.min.js` & `django-listable-0.8.1/listable/static/listable/js/jquery.dataTables.min.js`

 * *Files identical despite different names*

### Comparing `django-listable-0.8.0/listable/static/listable/js/jquery.dataTables.searchPlugins.js` & `django-listable-0.8.1/listable/static/listable/js/jquery.dataTables.searchPlugins.js`

 * *Files identical despite different names*

### Comparing `django-listable-0.8.0/listable/static/listable/js/jquery.dataTables.sort.js` & `django-listable-0.8.1/listable/static/listable/js/jquery.dataTables.sort.js`

 * *Files identical despite different names*

### Comparing `django-listable-0.8.0/listable/static/listable/js/jquery.js` & `django-listable-0.8.1/listable/static/listable/js/jquery.js`

 * *Files identical despite different names*

### Comparing `django-listable-0.8.0/listable/static/listable/js/listable.js` & `django-listable-0.8.1/listable/static/listable/js/listable.js`

 * *Files identical despite different names*

### Comparing `django-listable-0.8.0/listable/static/listable/js/moment.js` & `django-listable-0.8.1/listable/static/listable/js/moment.js`

 * *Files identical despite different names*

### Comparing `django-listable-0.8.0/listable/static/listable/js/moment.min.js` & `django-listable-0.8.1/listable/static/listable/js/moment.min.js`

 * *Files identical despite different names*

### Comparing `django-listable-0.8.0/listable/templates/listable/_table.html` & `django-listable-0.8.1/listable/templates/listable/_table.html`

 * *Files identical despite different names*

### Comparing `django-listable-0.8.0/listable/templates/listable/base.html` & `django-listable-0.8.1/listable/templates/listable/base.html`

 * *Files identical despite different names*

### Comparing `django-listable-0.8.0/listable/templatetags/listable.py` & `django-listable-0.8.1/listable/templatetags/listable.py`

 * *Files identical despite different names*

### Comparing `django-listable-0.8.0/listable/utils.py` & `django-listable-0.8.1/listable/utils.py`

 * *Files identical despite different names*

### Comparing `django-listable-0.8.0/listable/views.py` & `django-listable-0.8.1/listable/views.py`

 * *Files 0% similar despite different names*

```diff
@@ -303,15 +303,15 @@
                 if widget == SELECT:
                     search_term = [unquote(search_term, encoding=encoding).replace('\\', '')]
 
                 elif widget in [SELECT_MULTI, SELECT_MULTI_FROM_MULTI]:
                     if search_term in ['^(.*)$', '^()$']:
                         search_term = ''
                     else:
-                        search_term = unquote(search_term[2:-2], encoding=encoding).replace('\\', '').split('|')
+                        search_term = unquote(search_term[2:-2], encoding=encoding).replace('\\', '').split('`|`')
 
                 elif widget == DATE_RANGE:
                     start = datetime.datetime.strptime(search_term.split(' - ')[0], '%d %b %Y').replace(hour=0, minute=0, second=0)
                     end = datetime.datetime.strptime(search_term.split(' - ')[1], '%d %b %Y').replace(hour=23, minute=59, second=59)
                     start = cur_tz.localize(start)
                     end = cur_tz.localize(end)
                     search_term = (start, end)
```

### Comparing `django-listable-0.8.0/setup.py` & `django-listable-0.8.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import sys
 
 try:
     from setuptools import setup
 except ImportError:
     from distutils.core import setup
 
-version = '0.8.0'
+version = '0.8.1'
 
 if sys.argv[-1] == 'publish':
     os.system('python setup.py sdist upload')
     print("You probably want to also tag the version now:")
     print("  git tag -a %s -m 'version %s'" % (version, version))
     print("  git push --tags")
     sys.exit()
```

### Comparing `django-listable-0.8.0/tests/test_tags.py` & `django-listable-0.8.1/tests/test_tags.py`

 * *Files identical despite different names*

### Comparing `django-listable-0.8.0/tests/test_utils.py` & `django-listable-0.8.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `django-listable-0.8.0/tests/test_views.py` & `django-listable-0.8.1/tests/test_views.py`

 * *Files identical despite different names*

