# Comparing `tmp/nobinobi-observation-0.1.3.tar.gz` & `tmp/nobinobi-observation-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\nobinobi-observation-0.1.3.tar", last modified: Tue Dec 14 14:31:53 2021, max compression
+gzip compressed data, was "dist\nobinobi-observation-0.1.4.tar", last modified: Thu May 25 16:09:54 2023, max compression
```

## Comparing `nobinobi-observation-0.1.3.tar` & `nobinobi-observation-0.1.4.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxrwxrwx   0        0        0        0 2021-12-14 14:31:53.547254 nobinobi-observation-0.1.3/
--rw-rw-rw-   0        0        0      166 2021-09-24 06:35:40.000000 nobinobi-observation-0.1.3/AUTHORS.rst
--rw-rw-rw-   0        0        0     3447 2021-09-24 06:35:40.000000 nobinobi-observation-0.1.3/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0      484 2021-12-14 14:31:00.000000 nobinobi-observation-0.1.3/HISTORY.rst
--rw-rw-rw-   0        0        0    35184 2021-09-23 20:32:29.000000 nobinobi-observation-0.1.3/LICENSE
--rw-rw-rw-   0        0        0      490 2021-09-24 14:15:56.000000 nobinobi-observation-0.1.3/MANIFEST.in
--rw-rw-rw-   0        0        0     4892 2021-12-14 14:31:53.547254 nobinobi-observation-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     2555 2021-09-24 06:35:40.000000 nobinobi-observation-0.1.3/README.rst
-drwxrwxrwx   0        0        0        0 2021-12-14 14:31:53.518253 nobinobi-observation-0.1.3/nobinobi_observation/
--rw-rw-rw-   0        0        0       99 2021-12-14 14:31:00.000000 nobinobi-observation-0.1.3/nobinobi_observation/__init__.py
--rw-rw-rw-   0        0        0     1349 2021-09-24 12:51:43.000000 nobinobi-observation-0.1.3/nobinobi_observation/admin.py
--rw-rw-rw-   0        0        0     1309 2021-09-24 12:51:43.000000 nobinobi-observation-0.1.3/nobinobi_observation/apps.py
--rw-rw-rw-   0        0        0     4954 2021-12-14 14:30:59.000000 nobinobi-observation-0.1.3/nobinobi_observation/forms.py
-drwxrwxrwx   0        0        0        0 2021-12-14 14:31:53.496258 nobinobi-observation-0.1.3/nobinobi_observation/locale/
-drwxrwxrwx   0        0        0        0 2021-12-14 14:31:53.496258 nobinobi-observation-0.1.3/nobinobi_observation/locale/en/
-drwxrwxrwx   0        0        0        0 2021-12-14 14:31:53.526255 nobinobi-observation-0.1.3/nobinobi_observation/locale/en/LC_MESSAGES/
--rw-rw-rw-   0        0        0     4203 2021-09-24 06:35:40.000000 nobinobi-observation-0.1.3/nobinobi_observation/locale/en/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2021-12-14 14:31:53.497259 nobinobi-observation-0.1.3/nobinobi_observation/locale/fr/
-drwxrwxrwx   0        0        0        0 2021-12-14 14:31:53.528254 nobinobi-observation-0.1.3/nobinobi_observation/locale/fr/LC_MESSAGES/
--rw-rw-rw-   0        0        0     2539 2021-09-24 14:15:56.000000 nobinobi-observation-0.1.3/nobinobi_observation/locale/fr/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0     5102 2021-09-24 06:35:40.000000 nobinobi-observation-0.1.3/nobinobi_observation/locale/fr/LC_MESSAGES/django.po
--rw-rw-rw-   0        0        0     1961 2021-09-24 12:51:43.000000 nobinobi-observation-0.1.3/nobinobi_observation/menus.py
-drwxrwxrwx   0        0        0        0 2021-12-14 14:31:53.533259 nobinobi-observation-0.1.3/nobinobi_observation/migrations/
--rw-rw-rw-   0        0        0     1978 2021-09-24 06:35:40.000000 nobinobi-observation-0.1.3/nobinobi_observation/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      829 2021-09-24 06:35:40.000000 nobinobi-observation-0.1.3/nobinobi_observation/migrations/0002_auto_20190611_1051.py
--rw-rw-rw-   0        0        0      753 2021-09-24 06:35:40.000000 nobinobi-observation-0.1.3/nobinobi_observation/migrations/0003_auto_20200219_1049.py
--rw-rw-rw-   0        0        0        0 2021-09-24 06:35:40.000000 nobinobi-observation-0.1.3/nobinobi_observation/migrations/__init__.py
--rw-rw-rw-   0        0        0     2547 2021-09-24 12:51:43.000000 nobinobi-observation-0.1.3/nobinobi_observation/models.py
--rw-rw-rw-   0        0        0     1524 2021-09-24 12:51:43.000000 nobinobi-observation-0.1.3/nobinobi_observation/serializers.py
--rw-rw-rw-   0        0        0     3423 2021-09-24 12:51:43.000000 nobinobi-observation-0.1.3/nobinobi_observation/signals.py
-drwxrwxrwx   0        0        0        0 2021-12-14 14:31:53.500258 nobinobi-observation-0.1.3/nobinobi_observation/static/
-drwxrwxrwx   0        0        0        0 2021-12-14 14:31:53.534253 nobinobi-observation-0.1.3/nobinobi_observation/static/css/
--rw-rw-rw-   0        0        0        0 2021-09-24 06:35:40.000000 nobinobi-observation-0.1.3/nobinobi_observation/static/css/nobinobi_observation.css
-drwxrwxrwx   0        0        0        0 2021-12-14 14:31:53.534253 nobinobi-observation-0.1.3/nobinobi_observation/static/img/
--rw-rw-rw-   0        0        0        0 2021-09-24 06:35:40.000000 nobinobi-observation-0.1.3/nobinobi_observation/static/img/.gitignore
-drwxrwxrwx   0        0        0        0 2021-12-14 14:31:53.535253 nobinobi-observation-0.1.3/nobinobi_observation/static/js/
--rw-rw-rw-   0        0        0        0 2021-09-24 06:35:40.000000 nobinobi-observation-0.1.3/nobinobi_observation/static/js/nobinobi_observation.js
-drwxrwxrwx   0        0        0        0 2021-12-14 14:31:53.500258 nobinobi-observation-0.1.3/nobinobi_observation/templates/
-drwxrwxrwx   0        0        0        0 2021-12-14 14:31:53.541256 nobinobi-observation-0.1.3/nobinobi_observation/templates/nobinobi_observation/
--rw-rw-rw-   0        0        0      735 2021-09-24 06:35:40.000000 nobinobi-observation-0.1.3/nobinobi_observation/templates/nobinobi_observation/observation_choice.html
--rw-rw-rw-   0        0        0      748 2021-09-24 06:35:40.000000 nobinobi-observation-0.1.3/nobinobi_observation/templates/nobinobi_observation/observation_confirm_delete.html
--rw-rw-rw-   0        0        0      931 2021-09-24 06:35:40.000000 nobinobi-observation-0.1.3/nobinobi_observation/templates/nobinobi_observation/observation_detail.html
--rw-rw-rw-   0        0        0     7970 2021-09-24 06:35:40.000000 nobinobi-observation-0.1.3/nobinobi_observation/templates/nobinobi_observation/observation_detail_list.html
--rw-rw-rw-   0        0        0      813 2021-09-24 06:35:40.000000 nobinobi-observation-0.1.3/nobinobi_observation/templates/nobinobi_observation/observation_form.html
--rw-rw-rw-   0        0        0      306 2021-09-24 06:35:40.000000 nobinobi-observation-0.1.3/nobinobi_observation/templates/nobinobi_observation/observation_list.html
--rw-rw-rw-   0        0        0     1541 2021-09-24 06:35:40.000000 nobinobi-observation-0.1.3/nobinobi_observation/templates/nobinobi_observation/observation_update.html
-drwxrwxrwx   0        0        0        0 2021-12-14 14:31:53.542255 nobinobi-observation-0.1.3/nobinobi_observation/test_utils/
--rw-rw-rw-   0        0        0        0 2021-09-24 06:35:40.000000 nobinobi-observation-0.1.3/nobinobi_observation/test_utils/__init__.py
-drwxrwxrwx   0        0        0        0 2021-12-14 14:31:53.546255 nobinobi-observation-0.1.3/nobinobi_observation/test_utils/test_app/
--rw-rw-rw-   0        0        0        0 2021-09-24 06:35:40.000000 nobinobi-observation-0.1.3/nobinobi_observation/test_utils/test_app/__init__.py
--rw-rw-rw-   0        0        0       75 2021-09-24 06:35:40.000000 nobinobi-observation-0.1.3/nobinobi_observation/test_utils/test_app/admin.py
--rw-rw-rw-   0        0        0       95 2021-09-24 06:35:40.000000 nobinobi-observation-0.1.3/nobinobi_observation/test_utils/test_app/apps.py
-drwxrwxrwx   0        0        0        0 2021-12-14 14:31:53.546255 nobinobi-observation-0.1.3/nobinobi_observation/test_utils/test_app/migrations/
--rw-rw-rw-   0        0        0        0 2021-09-24 06:35:40.000000 nobinobi-observation-0.1.3/nobinobi_observation/test_utils/test_app/migrations/__init__.py
--rw-rw-rw-   0        0        0       63 2021-09-24 06:35:40.000000 nobinobi-observation-0.1.3/nobinobi_observation/test_utils/test_app/models.py
--rw-rw-rw-   0        0        0     2375 2021-09-24 12:51:43.000000 nobinobi-observation-0.1.3/nobinobi_observation/urls.py
--rw-rw-rw-   0        0        0      903 2021-09-24 12:51:43.000000 nobinobi-observation-0.1.3/nobinobi_observation/utils.py
--rw-rw-rw-   0        0        0     4083 2021-09-24 12:51:43.000000 nobinobi-observation-0.1.3/nobinobi_observation/views.py
-drwxrwxrwx   0        0        0        0 2021-12-14 14:31:53.525256 nobinobi-observation-0.1.3/nobinobi_observation.egg-info/
--rw-rw-rw-   0        0        0     4892 2021-12-14 14:31:53.000000 nobinobi-observation-0.1.3/nobinobi_observation.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2128 2021-12-14 14:31:53.000000 nobinobi-observation-0.1.3/nobinobi_observation.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-12-14 14:31:53.000000 nobinobi-observation-0.1.3/nobinobi_observation.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2021-12-14 14:31:53.000000 nobinobi-observation-0.1.3/nobinobi_observation.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       24 2021-12-14 14:31:53.000000 nobinobi-observation-0.1.3/nobinobi_observation.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2021-12-14 14:31:53.000000 nobinobi-observation-0.1.3/nobinobi_observation.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       60 2021-09-24 06:35:40.000000 nobinobi-observation-0.1.3/requirements.txt
--rw-rw-rw-   0        0        0      114 2021-09-24 12:42:44.000000 nobinobi-observation-0.1.3/requirements_dev.txt
--rw-rw-rw-   0        0        0      201 2021-09-24 06:35:40.000000 nobinobi-observation-0.1.3/requirements_test.txt
--rw-rw-rw-   0        0        0      420 2021-12-14 14:31:53.548254 nobinobi-observation-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     2372 2021-09-24 14:15:56.000000 nobinobi-observation-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-25 16:09:54.643458 nobinobi-observation-0.1.4/
+-rw-rw-rw-   0        0        0      166 2021-09-24 06:35:40.000000 nobinobi-observation-0.1.4/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3447 2021-09-24 06:35:40.000000 nobinobi-observation-0.1.4/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0      602 2023-05-25 16:09:15.000000 nobinobi-observation-0.1.4/HISTORY.rst
+-rw-rw-rw-   0        0        0    35184 2021-09-23 20:32:29.000000 nobinobi-observation-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0      490 2021-09-24 14:15:56.000000 nobinobi-observation-0.1.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     5050 2023-05-25 16:09:54.643458 nobinobi-observation-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2555 2021-09-24 06:35:40.000000 nobinobi-observation-0.1.4/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-25 16:09:54.487838 nobinobi-observation-0.1.4/nobinobi_observation/
+-rw-rw-rw-   0        0        0       99 2023-05-25 16:09:15.000000 nobinobi-observation-0.1.4/nobinobi_observation/__init__.py
+-rw-rw-rw-   0        0        0     1349 2021-09-24 12:51:43.000000 nobinobi-observation-0.1.4/nobinobi_observation/admin.py
+-rw-rw-rw-   0        0        0     1309 2021-09-24 12:51:43.000000 nobinobi-observation-0.1.4/nobinobi_observation/apps.py
+-rw-rw-rw-   0        0        0     4954 2021-12-14 14:30:59.000000 nobinobi-observation-0.1.4/nobinobi_observation/forms.py
+drwxrwxrwx   0        0        0        0 2023-05-25 16:09:54.313684 nobinobi-observation-0.1.4/nobinobi_observation/locale/
+drwxrwxrwx   0        0        0        0 2023-05-25 16:09:54.313684 nobinobi-observation-0.1.4/nobinobi_observation/locale/en/
+drwxrwxrwx   0        0        0        0 2023-05-25 16:09:54.508290 nobinobi-observation-0.1.4/nobinobi_observation/locale/en/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     4203 2021-09-24 06:35:40.000000 nobinobi-observation-0.1.4/nobinobi_observation/locale/en/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2023-05-25 16:09:54.314723 nobinobi-observation-0.1.4/nobinobi_observation/locale/fr/
+drwxrwxrwx   0        0        0        0 2023-05-25 16:09:54.534237 nobinobi-observation-0.1.4/nobinobi_observation/locale/fr/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     2539 2021-09-24 14:15:56.000000 nobinobi-observation-0.1.4/nobinobi_observation/locale/fr/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0     5102 2021-09-24 06:35:40.000000 nobinobi-observation-0.1.4/nobinobi_observation/locale/fr/LC_MESSAGES/django.po
+-rw-rw-rw-   0        0        0     1961 2021-09-24 12:51:43.000000 nobinobi-observation-0.1.4/nobinobi_observation/menus.py
+drwxrwxrwx   0        0        0        0 2023-05-25 16:09:54.561663 nobinobi-observation-0.1.4/nobinobi_observation/migrations/
+-rw-rw-rw-   0        0        0     1978 2021-09-24 06:35:40.000000 nobinobi-observation-0.1.4/nobinobi_observation/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      829 2021-09-24 06:35:40.000000 nobinobi-observation-0.1.4/nobinobi_observation/migrations/0002_auto_20190611_1051.py
+-rw-rw-rw-   0        0        0      753 2021-09-24 06:35:40.000000 nobinobi-observation-0.1.4/nobinobi_observation/migrations/0003_auto_20200219_1049.py
+-rw-rw-rw-   0        0        0        0 2021-09-24 06:35:40.000000 nobinobi-observation-0.1.4/nobinobi_observation/migrations/__init__.py
+-rw-rw-rw-   0        0        0     2547 2021-09-24 12:51:43.000000 nobinobi-observation-0.1.4/nobinobi_observation/models.py
+-rw-rw-rw-   0        0        0     1524 2021-09-24 12:51:43.000000 nobinobi-observation-0.1.4/nobinobi_observation/serializers.py
+-rw-rw-rw-   0        0        0     3423 2021-09-24 12:51:43.000000 nobinobi-observation-0.1.4/nobinobi_observation/signals.py
+drwxrwxrwx   0        0        0        0 2023-05-25 16:09:54.316669 nobinobi-observation-0.1.4/nobinobi_observation/static/
+drwxrwxrwx   0        0        0        0 2023-05-25 16:09:54.562662 nobinobi-observation-0.1.4/nobinobi_observation/static/css/
+-rw-rw-rw-   0        0        0        0 2021-09-24 06:35:40.000000 nobinobi-observation-0.1.4/nobinobi_observation/static/css/nobinobi_observation.css
+drwxrwxrwx   0        0        0        0 2023-05-25 16:09:54.563708 nobinobi-observation-0.1.4/nobinobi_observation/static/img/
+-rw-rw-rw-   0        0        0        0 2021-09-24 06:35:40.000000 nobinobi-observation-0.1.4/nobinobi_observation/static/img/.gitignore
+drwxrwxrwx   0        0        0        0 2023-05-25 16:09:54.564702 nobinobi-observation-0.1.4/nobinobi_observation/static/js/
+-rw-rw-rw-   0        0        0        0 2021-09-24 06:35:40.000000 nobinobi-observation-0.1.4/nobinobi_observation/static/js/nobinobi_observation.js
+drwxrwxrwx   0        0        0        0 2023-05-25 16:09:54.316669 nobinobi-observation-0.1.4/nobinobi_observation/templates/
+drwxrwxrwx   0        0        0        0 2023-05-25 16:09:54.635611 nobinobi-observation-0.1.4/nobinobi_observation/templates/nobinobi_observation/
+-rw-rw-rw-   0        0        0      735 2021-09-24 06:35:40.000000 nobinobi-observation-0.1.4/nobinobi_observation/templates/nobinobi_observation/observation_choice.html
+-rw-rw-rw-   0        0        0      748 2021-09-24 06:35:40.000000 nobinobi-observation-0.1.4/nobinobi_observation/templates/nobinobi_observation/observation_confirm_delete.html
+-rw-rw-rw-   0        0        0      931 2021-09-24 06:35:40.000000 nobinobi-observation-0.1.4/nobinobi_observation/templates/nobinobi_observation/observation_detail.html
+-rw-rw-rw-   0        0        0     8119 2023-05-25 16:09:14.000000 nobinobi-observation-0.1.4/nobinobi_observation/templates/nobinobi_observation/observation_detail_list.html
+-rw-rw-rw-   0        0        0      813 2021-09-24 06:35:40.000000 nobinobi-observation-0.1.4/nobinobi_observation/templates/nobinobi_observation/observation_form.html
+-rw-rw-rw-   0        0        0      306 2021-09-24 06:35:40.000000 nobinobi-observation-0.1.4/nobinobi_observation/templates/nobinobi_observation/observation_list.html
+-rw-rw-rw-   0        0        0     1541 2021-09-24 06:35:40.000000 nobinobi-observation-0.1.4/nobinobi_observation/templates/nobinobi_observation/observation_update.html
+drwxrwxrwx   0        0        0        0 2023-05-25 16:09:54.637481 nobinobi-observation-0.1.4/nobinobi_observation/test_utils/
+-rw-rw-rw-   0        0        0        0 2021-09-24 06:35:40.000000 nobinobi-observation-0.1.4/nobinobi_observation/test_utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 16:09:54.641460 nobinobi-observation-0.1.4/nobinobi_observation/test_utils/test_app/
+-rw-rw-rw-   0        0        0        0 2021-09-24 06:35:40.000000 nobinobi-observation-0.1.4/nobinobi_observation/test_utils/test_app/__init__.py
+-rw-rw-rw-   0        0        0       75 2021-09-24 06:35:40.000000 nobinobi-observation-0.1.4/nobinobi_observation/test_utils/test_app/admin.py
+-rw-rw-rw-   0        0        0       95 2021-09-24 06:35:40.000000 nobinobi-observation-0.1.4/nobinobi_observation/test_utils/test_app/apps.py
+drwxrwxrwx   0        0        0        0 2023-05-25 16:09:54.642498 nobinobi-observation-0.1.4/nobinobi_observation/test_utils/test_app/migrations/
+-rw-rw-rw-   0        0        0        0 2021-09-24 06:35:40.000000 nobinobi-observation-0.1.4/nobinobi_observation/test_utils/test_app/migrations/__init__.py
+-rw-rw-rw-   0        0        0       63 2021-09-24 06:35:40.000000 nobinobi-observation-0.1.4/nobinobi_observation/test_utils/test_app/models.py
+-rw-rw-rw-   0        0        0     2375 2021-09-24 12:51:43.000000 nobinobi-observation-0.1.4/nobinobi_observation/urls.py
+-rw-rw-rw-   0        0        0      903 2021-09-24 12:51:43.000000 nobinobi-observation-0.1.4/nobinobi_observation/utils.py
+-rw-rw-rw-   0        0        0     4083 2021-09-24 12:51:43.000000 nobinobi-observation-0.1.4/nobinobi_observation/views.py
+drwxrwxrwx   0        0        0        0 2023-05-25 16:09:54.507293 nobinobi-observation-0.1.4/nobinobi_observation.egg-info/
+-rw-rw-rw-   0        0        0     5050 2023-05-25 16:09:53.000000 nobinobi-observation-0.1.4/nobinobi_observation.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2128 2023-05-25 16:09:53.000000 nobinobi-observation-0.1.4/nobinobi_observation.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 16:09:53.000000 nobinobi-observation-0.1.4/nobinobi_observation.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-25 16:07:46.000000 nobinobi-observation-0.1.4/nobinobi_observation.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       24 2023-05-25 16:09:53.000000 nobinobi-observation-0.1.4/nobinobi_observation.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-05-25 16:09:53.000000 nobinobi-observation-0.1.4/nobinobi_observation.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       60 2021-09-24 06:35:40.000000 nobinobi-observation-0.1.4/requirements.txt
+-rw-rw-rw-   0        0        0      114 2021-09-24 12:42:44.000000 nobinobi-observation-0.1.4/requirements_dev.txt
+-rw-rw-rw-   0        0        0      201 2021-09-24 06:35:40.000000 nobinobi-observation-0.1.4/requirements_test.txt
+-rw-rw-rw-   0        0        0      417 2023-05-25 16:09:54.644329 nobinobi-observation-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     2372 2021-09-24 14:15:56.000000 nobinobi-observation-0.1.4/setup.py
```

### Comparing `nobinobi-observation-0.1.3/CONTRIBUTING.rst` & `nobinobi-observation-0.1.4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `nobinobi-observation-0.1.3/LICENSE` & `nobinobi-observation-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nobinobi-observation-0.1.3/PKG-INFO` & `nobinobi-observation-0.1.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: nobinobi-observation
-Version: 0.1.3
+Version: 0.1.4
 Summary: Application Observation for Nobinobi
 Home-page: https://github.com/prolibre-ch/nobinobi-observation
 Author: Florian Alu
 Author-email: alu@prolibre.com
 License: UNKNOWN
 Description: =============================
         Nobinobi Observation
@@ -114,14 +114,19 @@
         
         
         
         
         History
         -------
         
+        0.1.4 (2023-05-25)
+        ++++++++++++++++++
+        
+        * 6b7fd8a - Fix error when no staff filled in observation detail display
+        
         0.1.3 (2021-12-14)
         ++++++++++++++++++
         
         * 9f6c9d0 - fix error with new version of bootstrap datetimepicker
         
         
         0.1.2 (2021-09-24)
```

### Comparing `nobinobi-observation-0.1.3/README.rst` & `nobinobi-observation-0.1.4/README.rst`

 * *Files identical despite different names*

### Comparing `nobinobi-observation-0.1.3/nobinobi_observation/admin.py` & `nobinobi-observation-0.1.4/nobinobi_observation/admin.py`

 * *Files identical despite different names*

### Comparing `nobinobi-observation-0.1.3/nobinobi_observation/apps.py` & `nobinobi-observation-0.1.4/nobinobi_observation/apps.py`

 * *Files identical despite different names*

### Comparing `nobinobi-observation-0.1.3/nobinobi_observation/forms.py` & `nobinobi-observation-0.1.4/nobinobi_observation/forms.py`

 * *Files identical despite different names*

### Comparing `nobinobi-observation-0.1.3/nobinobi_observation/locale/en/LC_MESSAGES/django.po` & `nobinobi-observation-0.1.4/nobinobi_observation/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `nobinobi-observation-0.1.3/nobinobi_observation/locale/fr/LC_MESSAGES/django.mo` & `nobinobi-observation-0.1.4/nobinobi_observation/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `nobinobi-observation-0.1.3/nobinobi_observation/locale/fr/LC_MESSAGES/django.po` & `nobinobi-observation-0.1.4/nobinobi_observation/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `nobinobi-observation-0.1.3/nobinobi_observation/menus.py` & `nobinobi-observation-0.1.4/nobinobi_observation/menus.py`

 * *Files identical despite different names*

### Comparing `nobinobi-observation-0.1.3/nobinobi_observation/migrations/0001_initial.py` & `nobinobi-observation-0.1.4/nobinobi_observation/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `nobinobi-observation-0.1.3/nobinobi_observation/migrations/0002_auto_20190611_1051.py` & `nobinobi-observation-0.1.4/nobinobi_observation/migrations/0002_auto_20190611_1051.py`

 * *Files identical despite different names*

### Comparing `nobinobi-observation-0.1.3/nobinobi_observation/migrations/0003_auto_20200219_1049.py` & `nobinobi-observation-0.1.4/nobinobi_observation/migrations/0003_auto_20200219_1049.py`

 * *Files identical despite different names*

### Comparing `nobinobi-observation-0.1.3/nobinobi_observation/models.py` & `nobinobi-observation-0.1.4/nobinobi_observation/models.py`

 * *Files identical despite different names*

### Comparing `nobinobi-observation-0.1.3/nobinobi_observation/serializers.py` & `nobinobi-observation-0.1.4/nobinobi_observation/serializers.py`

 * *Files identical despite different names*

### Comparing `nobinobi-observation-0.1.3/nobinobi_observation/signals.py` & `nobinobi-observation-0.1.4/nobinobi_observation/signals.py`

 * *Files identical despite different names*

### Comparing `nobinobi-observation-0.1.3/nobinobi_observation/templates/nobinobi_observation/observation_choice.html` & `nobinobi-observation-0.1.4/nobinobi_observation/templates/nobinobi_observation/observation_choice.html`

 * *Files identical despite different names*

### Comparing `nobinobi-observation-0.1.3/nobinobi_observation/templates/nobinobi_observation/observation_confirm_delete.html` & `nobinobi-observation-0.1.4/nobinobi_observation/templates/nobinobi_observation/observation_confirm_delete.html`

 * *Files identical despite different names*

### Comparing `nobinobi-observation-0.1.3/nobinobi_observation/templates/nobinobi_observation/observation_detail.html` & `nobinobi-observation-0.1.4/nobinobi_observation/templates/nobinobi_observation/observation_detail.html`

 * *Files identical despite different names*

### Comparing `nobinobi-observation-0.1.3/nobinobi_observation/templates/nobinobi_observation/observation_detail_list.html` & `nobinobi-observation-0.1.4/nobinobi_observation/templates/nobinobi_observation/observation_detail_list.html`

 * *Files 2% similar despite different names*

```diff
@@ -119,30 +119,32 @@
                           return date.format('lll');
                       },
                   },
                   {
                       data: "staff",
                       name: "staff__first_name, staff__last_name",
                       render: function (row, index, datatable) {
-                          return row.first_name + " " + row.last_name;
+                          if (row == null || row === 'undefined'){
+                            return "{% trans "Empty" %}";
+                          } else {
+                              return row.first_name + " " + row.last_name;
+                          }
                       },
                   },
                   {
                       data: "status",
                       name: "status",
                       render: function (row, index, datatable) {
                           return '<img width="30px "src="{% static "img/smiley" %}/' + row + '" alt="' + row + '">';
                       },
                   },
                   {
                       data: "_comment_excerpt",
                       name: "_comment_excerpt",
                       render: function (row, index, data) {
-                          console.log(row);
-
                           return row.replace("\n\n", "<br><br>").replace("\n", "<br>");
                       },
                   },
                   {
                       data: null,
                       orderable: false,
                       searchable: false,
```

### Comparing `nobinobi-observation-0.1.3/nobinobi_observation/templates/nobinobi_observation/observation_form.html` & `nobinobi-observation-0.1.4/nobinobi_observation/templates/nobinobi_observation/observation_form.html`

 * *Files identical despite different names*

### Comparing `nobinobi-observation-0.1.3/nobinobi_observation/templates/nobinobi_observation/observation_update.html` & `nobinobi-observation-0.1.4/nobinobi_observation/templates/nobinobi_observation/observation_update.html`

 * *Files identical despite different names*

### Comparing `nobinobi-observation-0.1.3/nobinobi_observation/urls.py` & `nobinobi-observation-0.1.4/nobinobi_observation/urls.py`

 * *Files identical despite different names*

### Comparing `nobinobi-observation-0.1.3/nobinobi_observation/utils.py` & `nobinobi-observation-0.1.4/nobinobi_observation/utils.py`

 * *Files identical despite different names*

### Comparing `nobinobi-observation-0.1.3/nobinobi_observation/views.py` & `nobinobi-observation-0.1.4/nobinobi_observation/views.py`

 * *Files identical despite different names*

### Comparing `nobinobi-observation-0.1.3/nobinobi_observation.egg-info/PKG-INFO` & `nobinobi-observation-0.1.4/nobinobi_observation.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: nobinobi-observation
-Version: 0.1.3
+Version: 0.1.4
 Summary: Application Observation for Nobinobi
 Home-page: https://github.com/prolibre-ch/nobinobi-observation
 Author: Florian Alu
 Author-email: alu@prolibre.com
 License: UNKNOWN
 Description: =============================
         Nobinobi Observation
@@ -114,14 +114,19 @@
         
         
         
         
         History
         -------
         
+        0.1.4 (2023-05-25)
+        ++++++++++++++++++
+        
+        * 6b7fd8a - Fix error when no staff filled in observation detail display
+        
         0.1.3 (2021-12-14)
         ++++++++++++++++++
         
         * 9f6c9d0 - fix error with new version of bootstrap datetimepicker
         
         
         0.1.2 (2021-09-24)
```

### Comparing `nobinobi-observation-0.1.3/nobinobi_observation.egg-info/SOURCES.txt` & `nobinobi-observation-0.1.4/nobinobi_observation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nobinobi-observation-0.1.3/setup.py` & `nobinobi-observation-0.1.4/setup.py`

 * *Files identical despite different names*

