# Comparing `tmp/aa-charlink-0.4.1.tar.gz` & `tmp/aa-charlink-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aa-charlink-0.4.1.tar", last modified: Sun May 21 17:47:00 2023, max compression
+gzip compressed data, was "aa-charlink-0.5.0.tar", last modified: Thu May 25 12:54:43 2023, max compression
```

## Comparing `aa-charlink-0.4.1.tar` & `aa-charlink-0.5.0.tar`

### file list

```diff
@@ -1,49 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:47:00.355195 aa-charlink-0.4.1/
--rwxr-xr-x   0 runner    (1001) docker     (123)    35149 2023-05-21 17:46:44.000000 aa-charlink-0.4.1/LICENSE
--rwxr-xr-x   0 runner    (1001) docker     (123)      197 2023-05-21 17:46:44.000000 aa-charlink-0.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-05-21 17:47:00.355195 aa-charlink-0.4.1/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     2377 2023-05-21 17:46:44.000000 aa-charlink-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:47:00.351195 aa-charlink-0.4.1/aa_charlink.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-05-21 17:47:00.000000 aa-charlink-0.4.1/aa_charlink.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-05-21 17:47:00.000000 aa-charlink-0.4.1/aa_charlink.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 17:47:00.000000 aa-charlink-0.4.1/aa_charlink.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 17:47:00.000000 aa-charlink-0.4.1/aa_charlink.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-21 17:47:00.000000 aa-charlink-0.4.1/aa_charlink.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-21 17:47:00.000000 aa-charlink-0.4.1/aa_charlink.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:47:00.351195 aa-charlink-0.4.1/charlink/
--rwxr-xr-x   0 runner    (1001) docker     (123)      127 2023-05-21 17:46:44.000000 aa-charlink-0.4.1/charlink/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1451 2023-05-21 17:46:44.000000 aa-charlink-0.4.1/charlink/app_imports.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      108 2023-05-21 17:46:44.000000 aa-charlink-0.4.1/charlink/app_settings.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      148 2023-05-21 17:46:44.000000 aa-charlink-0.4.1/charlink/apps.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      468 2023-05-21 17:46:44.000000 aa-charlink-0.4.1/charlink/auth_hooks.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      494 2023-05-21 17:46:44.000000 aa-charlink-0.4.1/charlink/decorators.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      746 2023-05-21 17:46:44.000000 aa-charlink-0.4.1/charlink/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:47:00.351195 aa-charlink-0.4.1/charlink/imports/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:46:44.000000 aa-charlink-0.4.1/charlink/imports/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:47:00.355195 aa-charlink-0.4.1/charlink/imports/allianceauth/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:46:44.000000 aa-charlink-0.4.1/charlink/imports/allianceauth/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1229 2023-05-21 17:46:44.000000 aa-charlink-0.4.1/charlink/imports/allianceauth/corputils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      662 2023-05-21 17:46:44.000000 aa-charlink-0.4.1/charlink/imports/corptools.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1162 2023-05-21 17:46:44.000000 aa-charlink-0.4.1/charlink/imports/memberaudit.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      687 2023-05-21 17:46:44.000000 aa-charlink-0.4.1/charlink/imports/miningtaxes.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1689 2023-05-21 17:46:44.000000 aa-charlink-0.4.1/charlink/imports/moonmining.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      820 2023-05-21 17:46:44.000000 aa-charlink-0.4.1/charlink/imports/moonstuff.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4419 2023-05-21 17:46:44.000000 aa-charlink-0.4.1/charlink/imports/structures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:47:00.355195 aa-charlink-0.4.1/charlink/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-05-21 17:46:44.000000 aa-charlink-0.4.1/charlink/migrations/0001_initial.py
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:46:44.000000 aa-charlink-0.4.1/charlink/migrations/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      435 2023-05-21 17:46:44.000000 aa-charlink-0.4.1/charlink/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:47:00.347195 aa-charlink-0.4.1/charlink/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:47:00.355195 aa-charlink-0.4.1/charlink/templates/charlink/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3656 2023-05-21 17:46:44.000000 aa-charlink-0.4.1/charlink/templates/charlink/audit.html
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-05-21 17:46:44.000000 aa-charlink-0.4.1/charlink/templates/charlink/base_audit.html
--rwxr-xr-x   0 runner    (1001) docker     (123)     3565 2023-05-21 17:46:44.000000 aa-charlink-0.4.1/charlink/templates/charlink/charlink.html
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-05-21 17:46:44.000000 aa-charlink-0.4.1/charlink/templates/charlink/search.html
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-05-21 17:46:44.000000 aa-charlink-0.4.1/charlink/templates/charlink/user_audit.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:47:00.355195 aa-charlink-0.4.1/charlink/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 17:46:44.000000 aa-charlink-0.4.1/charlink/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-21 17:46:44.000000 aa-charlink-0.4.1/charlink/templatetags/charlinkutils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      429 2023-05-21 17:46:44.000000 aa-charlink-0.4.1/charlink/urls.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7398 2023-05-21 17:46:44.000000 aa-charlink-0.4.1/charlink/views.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      104 2023-05-21 17:46:44.000000 aa-charlink-0.4.1/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1577 2023-05-21 17:47:00.355195 aa-charlink-0.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:54:43.776608 aa-charlink-0.5.0/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    35149 2023-05-25 12:54:23.000000 aa-charlink-0.5.0/LICENSE
+-rwxr-xr-x   0 runner    (1001) docker     (123)      197 2023-05-25 12:54:23.000000 aa-charlink-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-05-25 12:54:43.776608 aa-charlink-0.5.0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2508 2023-05-25 12:54:23.000000 aa-charlink-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:54:43.768608 aa-charlink-0.5.0/aa_charlink.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-05-25 12:54:43.000000 aa-charlink-0.5.0/aa_charlink.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-05-25 12:54:43.000000 aa-charlink-0.5.0/aa_charlink.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 12:54:43.000000 aa-charlink-0.5.0/aa_charlink.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 12:54:43.000000 aa-charlink-0.5.0/aa_charlink.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-25 12:54:43.000000 aa-charlink-0.5.0/aa_charlink.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-25 12:54:43.000000 aa-charlink-0.5.0/aa_charlink.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:54:43.772608 aa-charlink-0.5.0/charlink/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      127 2023-05-25 12:54:23.000000 aa-charlink-0.5.0/charlink/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1703 2023-05-25 12:54:23.000000 aa-charlink-0.5.0/charlink/app_imports.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      108 2023-05-25 12:54:23.000000 aa-charlink-0.5.0/charlink/app_settings.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      148 2023-05-25 12:54:23.000000 aa-charlink-0.5.0/charlink/apps.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      468 2023-05-25 12:54:23.000000 aa-charlink-0.5.0/charlink/auth_hooks.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      494 2023-05-25 12:54:23.000000 aa-charlink-0.5.0/charlink/decorators.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      746 2023-05-25 12:54:23.000000 aa-charlink-0.5.0/charlink/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:54:43.772608 aa-charlink-0.5.0/charlink/imports/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:54:23.000000 aa-charlink-0.5.0/charlink/imports/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:54:43.772608 aa-charlink-0.5.0/charlink/imports/allianceauth/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:54:23.000000 aa-charlink-0.5.0/charlink/imports/allianceauth/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1400 2023-05-25 12:54:23.000000 aa-charlink-0.5.0/charlink/imports/allianceauth/corputils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-05-25 12:54:23.000000 aa-charlink-0.5.0/charlink/imports/corpstats.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      821 2023-05-25 12:54:23.000000 aa-charlink-0.5.0/charlink/imports/corptools.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1319 2023-05-25 12:54:23.000000 aa-charlink-0.5.0/charlink/imports/memberaudit.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      844 2023-05-25 12:54:23.000000 aa-charlink-0.5.0/charlink/imports/miningtaxes.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1860 2023-05-25 12:54:23.000000 aa-charlink-0.5.0/charlink/imports/moonmining.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      982 2023-05-25 12:54:23.000000 aa-charlink-0.5.0/charlink/imports/moonstuff.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4599 2023-05-25 12:54:23.000000 aa-charlink-0.5.0/charlink/imports/structures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:54:43.772608 aa-charlink-0.5.0/charlink/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-05-25 12:54:23.000000 aa-charlink-0.5.0/charlink/migrations/0001_initial.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:54:23.000000 aa-charlink-0.5.0/charlink/migrations/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      435 2023-05-25 12:54:23.000000 aa-charlink-0.5.0/charlink/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:54:43.768608 aa-charlink-0.5.0/charlink/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:54:43.776608 aa-charlink-0.5.0/charlink/templates/charlink/
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-05-25 12:54:23.000000 aa-charlink-0.5.0/charlink/templates/charlink/app_audit.html
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3656 2023-05-25 12:54:23.000000 aa-charlink-0.5.0/charlink/templates/charlink/audit.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-05-25 12:54:23.000000 aa-charlink-0.5.0/charlink/templates/charlink/base_audit.html
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3786 2023-05-25 12:54:23.000000 aa-charlink-0.5.0/charlink/templates/charlink/charlink.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-05-25 12:54:23.000000 aa-charlink-0.5.0/charlink/templates/charlink/search.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-05-25 12:54:23.000000 aa-charlink-0.5.0/charlink/templates/charlink/user_audit.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:54:43.776608 aa-charlink-0.5.0/charlink/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 12:54:23.000000 aa-charlink-0.5.0/charlink/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-25 12:54:23.000000 aa-charlink-0.5.0/charlink/templatetags/charlinkutils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      498 2023-05-25 12:54:23.000000 aa-charlink-0.5.0/charlink/urls.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8715 2023-05-25 12:54:23.000000 aa-charlink-0.5.0/charlink/views.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      104 2023-05-25 12:54:23.000000 aa-charlink-0.5.0/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1577 2023-05-25 12:54:43.776608 aa-charlink-0.5.0/setup.cfg
```

### Comparing `aa-charlink-0.4.1/LICENSE` & `aa-charlink-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aa-charlink-0.4.1/PKG-INFO` & `aa-charlink-0.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aa-charlink
-Version: 0.4.1
+Version: 0.5.0
 Summary: Character Linker for Alliance Auth
 Home-page: https://github.com/Maestro-Zacht/aa-charlink
 Author-email: matteo.ghia@yahoo.it
 License: GNU General Public License v3
 Keywords: allianceauth,allianceauth_charlink,charlink,eveonline
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -45,14 +45,16 @@
 
 ### Auditing
 
 Users with the appropriate permission (see [permissions](#permissions)) can audit the linked characters of the users of their corporation, alliance or auth state. A link will appear on top of the main page of the app and will redirect to a page with a table of all the linked characters of the users of the selected corporation.
 
 A user can be audited by clicking on the link on the `Main Character` column.
 
+NEW: Users can now audit the apps they have access to. Select the app you want to audit from the dropdown menu in the audit page.
+
 ## Installation
 
 1. Install the app with
 
    ```shell
    pip install aa-charlink
    ```
```

### Comparing `aa-charlink-0.4.1/README.md` & `aa-charlink-0.5.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 
 ### Auditing
 
 Users with the appropriate permission (see [permissions](#permissions)) can audit the linked characters of the users of their corporation, alliance or auth state. A link will appear on top of the main page of the app and will redirect to a page with a table of all the linked characters of the users of the selected corporation.
 
 A user can be audited by clicking on the link on the `Main Character` column.
 
+NEW: Users can now audit the apps they have access to. Select the app you want to audit from the dropdown menu in the audit page.
+
 ## Installation
 
 1. Install the app with
 
    ```shell
    pip install aa-charlink
    ```
```

### Comparing `aa-charlink-0.4.1/aa_charlink.egg-info/PKG-INFO` & `aa-charlink-0.5.0/aa_charlink.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aa-charlink
-Version: 0.4.1
+Version: 0.5.0
 Summary: Character Linker for Alliance Auth
 Home-page: https://github.com/Maestro-Zacht/aa-charlink
 Author-email: matteo.ghia@yahoo.it
 License: GNU General Public License v3
 Keywords: allianceauth,allianceauth_charlink,charlink,eveonline
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -45,14 +45,16 @@
 
 ### Auditing
 
 Users with the appropriate permission (see [permissions](#permissions)) can audit the linked characters of the users of their corporation, alliance or auth state. A link will appear on top of the main page of the app and will redirect to a page with a table of all the linked characters of the users of the selected corporation.
 
 A user can be audited by clicking on the link on the `Main Character` column.
 
+NEW: Users can now audit the apps they have access to. Select the app you want to audit from the dropdown menu in the audit page.
+
 ## Installation
 
 1. Install the app with
 
    ```shell
    pip install aa-charlink
    ```
```

### Comparing `aa-charlink-0.4.1/aa_charlink.egg-info/SOURCES.txt` & `aa-charlink-0.5.0/aa_charlink.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -16,24 +16,26 @@
 charlink/auth_hooks.py
 charlink/decorators.py
 charlink/forms.py
 charlink/models.py
 charlink/urls.py
 charlink/views.py
 charlink/imports/__init__.py
+charlink/imports/corpstats.py
 charlink/imports/corptools.py
 charlink/imports/memberaudit.py
 charlink/imports/miningtaxes.py
 charlink/imports/moonmining.py
 charlink/imports/moonstuff.py
 charlink/imports/structures.py
 charlink/imports/allianceauth/__init__.py
 charlink/imports/allianceauth/corputils.py
 charlink/migrations/0001_initial.py
 charlink/migrations/__init__.py
+charlink/templates/charlink/app_audit.html
 charlink/templates/charlink/audit.html
 charlink/templates/charlink/base_audit.html
 charlink/templates/charlink/charlink.html
 charlink/templates/charlink/search.html
 charlink/templates/charlink/user_audit.html
 charlink/templatetags/__init__.py
 charlink/templatetags/charlinkutils.py
```

### Comparing `aa-charlink-0.4.1/charlink/app_imports.py` & `aa-charlink-0.5.0/charlink/app_imports.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 from importlib import import_module
 
 from django.conf import settings
+from django.db.models import Exists, OuterRef
 
 from allianceauth.services.hooks import get_extension_logger
 from allianceauth.authentication.models import CharacterOwnership
 
 logger = get_extension_logger(__name__)
 
 _supported_apps = {
     'add_character': {
         'field_label': 'Add Character (default)',
         'add_character': lambda request, token: None,
         'scopes': ['publicData'],
         'permissions': [],
         'is_character_added': lambda character: CharacterOwnership.objects.filter(character=character).exists(),
+        'is_character_added_annotation': Exists(CharacterOwnership.objects.filter(character_id=OuterRef('pk')))
     }
 }
 
 _imported = False
 
 
 def import_apps():
@@ -32,14 +34,15 @@
                 else:
                     _supported_apps[app] = {
                         'field_label': module.field_label,
                         'add_character': module.add_character,
                         'scopes': module.scopes,
                         'permissions': module.permissions,
                         'is_character_added': module.is_character_added,
+                        'is_character_added_annotation': module.is_character_added_annotation
                     }
 
                     logger.debug(f"Loading of {app} link: success")
 
         _imported = True
 
     return _supported_apps
```

### Comparing `aa-charlink-0.4.1/charlink/forms.py` & `aa-charlink-0.5.0/charlink/forms.py`

 * *Files identical despite different names*

### Comparing `aa-charlink-0.4.1/charlink/imports/allianceauth/corputils.py` & `aa-charlink-0.5.0/charlink/imports/allianceauth/corputils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from django.db.models import Exists, OuterRef
+
 from allianceauth.eveonline.models import EveCharacter, EveCorporationInfo
 from allianceauth.corputils.views import SWAGGER_SPEC_PATH
 from allianceauth.corputils.models import CorpStats
 
 field_label = 'Corporation Stats'
 
 scopes = ['esi-corporations.read_corporation_membership.v1']
@@ -27,7 +29,13 @@
 
 def is_character_added(character: EveCharacter):
     return (
         CorpStats.objects
         .filter(token__character_id=character.character_id)
         .exists()
     )
+
+
+is_character_added_annotation = Exists(
+    CorpStats.objects
+    .filter(token__character_id=OuterRef('character_id'))
+)
```

### Comparing `aa-charlink-0.4.1/charlink/imports/corptools.py` & `aa-charlink-0.5.0/charlink/imports/corptools.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from django.db.models import Exists, OuterRef
+
 from corptools.models import CharacterAudit
 from corptools.tasks import update_character
 from corptools.app_settings import get_character_scopes, CORPTOOLS_APP_NAME
 
 from allianceauth.eveonline.models import EveCharacter
 
 field_label = CORPTOOLS_APP_NAME
@@ -15,7 +17,13 @@
     CharacterAudit.objects.update_or_create(
         character=EveCharacter.objects.get_character_by_id(token.character_id))
     update_character.apply_async(args=[token.character_id], priority=6)
 
 
 def is_character_added(character: EveCharacter):
     return CharacterAudit.objects.filter(character=character).exists()
+
+
+is_character_added_annotation = Exists(
+    CharacterAudit.objects
+    .filter(character_id=OuterRef('pk'))
+)
```

### Comparing `aa-charlink-0.4.1/charlink/imports/memberaudit.py` & `aa-charlink-0.5.0/charlink/imports/memberaudit.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from django.db import transaction
+from django.db.models import Exists, OuterRef
 
 from memberaudit.models import Character, ComplianceGroupDesignation
 from memberaudit.app_settings import MEMBERAUDIT_APP_NAME, MEMBERAUDIT_TASKS_NORMAL_PRIORITY
 from memberaudit import tasks
 
 from allianceauth.eveonline.models import EveCharacter
 
@@ -27,7 +28,13 @@
         tasks.update_compliance_groups_for_user.apply_async(
             args=[request.user.pk], priority=MEMBERAUDIT_TASKS_NORMAL_PRIORITY
         )
 
 
 def is_character_added(character: EveCharacter):
     return Character.objects.filter(eve_character=character).exists()
+
+
+is_character_added_annotation = Exists(
+    Character.objects
+    .filter(eve_character_id=OuterRef('pk'))
+)
```

### Comparing `aa-charlink-0.4.1/charlink/imports/moonmining.py` & `aa-charlink-0.5.0/charlink/imports/moonmining.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from django.db.models import Exists, OuterRef
+
 from moonmining.models import Owner
 from moonmining import __title__, tasks
 from moonmining.app_settings import MOONMINING_ADMIN_NOTIFICATIONS_ENABLED
 
 from app_utils.messages import messages_plus
 from app_utils.allianceauth import notify_admins
 
@@ -43,7 +45,13 @@
         )
 
 
 def is_character_added(character: EveCharacter):
     return Owner.objects.filter(
         character_ownership__character=character
     ).exists()
+
+
+is_character_added_annotation = Exists(
+    Owner.objects
+    .filter(character_ownership__character_id=OuterRef('pk'))
+)
```

### Comparing `aa-charlink-0.4.1/charlink/imports/moonstuff.py` & `aa-charlink-0.5.0/charlink/imports/moonstuff.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from django.db.models import Exists, OuterRef
+
 from moonstuff.providers import ESI_CHARACTER_SCOPES
 from moonstuff.models import TrackingCharacter
 from moonstuff.tasks import import_extraction_data
 
 from allianceauth.eveonline.models import EveCharacter
 
 field_label = 'Moon Tools'
@@ -20,7 +22,13 @@
 
         # Schedule an import task to pull data from the new Tracking Character.
         import_extraction_data.delay()
 
 
 def is_character_added(character: EveCharacter):
     return TrackingCharacter.objects.filter(character=character).exists()
+
+
+is_character_added_annotation = Exists(
+    TrackingCharacter.objects
+    .filter(character_id=OuterRef('pk'))
+)
```

### Comparing `aa-charlink-0.4.1/charlink/imports/structures.py` & `aa-charlink-0.5.0/charlink/imports/structures.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from django.db.models import Exists, OuterRef
+
 from django.utils import translation
 from django.utils.translation import gettext as _
 from django.utils.html import format_html
 
 from structures import __title__, tasks
 from structures.models import Owner, Webhook, OwnerCharacter
 from structures.app_settings import (
@@ -109,7 +111,13 @@
                 )
 
 
 def is_character_added(character: EveCharacter):
     return OwnerCharacter.objects.filter(
         character_ownership__character=character
     ).exists()
+
+
+is_character_added_annotation = Exists(
+    OwnerCharacter.objects
+    .filter(character_ownership__character_id=OuterRef('pk'))
+)
```

### Comparing `aa-charlink-0.4.1/charlink/migrations/0001_initial.py` & `aa-charlink-0.5.0/charlink/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `aa-charlink-0.4.1/charlink/templates/charlink/audit.html` & `aa-charlink-0.5.0/charlink/templates/charlink/audit.html`

 * *Files identical despite different names*

### Comparing `aa-charlink-0.4.1/charlink/templates/charlink/base_audit.html` & `aa-charlink-0.5.0/charlink/templates/charlink/base_audit.html`

 * *Files 10% similar despite different names*

```diff
@@ -12,14 +12,24 @@
                             {% for corp in available %}
                                 <li>
                                     <a href="{% url 'charlink:audit_corp' corp.corporation_id %}">{{ corp.corporation_name }}</a>
                                 </li>
                             {% endfor %}
                         </ul>
                     </li>
+                    <li class="dropdown">
+                        <a href="#" id="appDrop" class="dropdown-toggle" role="button" data-toggle="dropdown" aria-haspopup="false" aria-expanded="false">Apps<span class="caret"></span></a>
+                        <ul class="dropdown-menu" role="menu" aria-labelledby="appDrop">
+                            {% for app, data in available_apps.items %}
+                                <li>
+                                    <a href="{% url 'charlink:audit_app' app %}">{{ data.field_label }}</a>
+                                </li>
+                            {% endfor %}
+                        </ul>
+                    </li>
                 </ul>
                 <form class="navbar-form navbar-right" role="search" action="{% url 'charlink:search' %}" method="GET">
                     <div class="form-group">
                         <input type="text" class="form-control" name="search_string" placeholder="{% if search_string %}{{ search_string }}{% else %}Search character...{% endif %}">
                     </div>
                 </form>
             </div>
```

#### html2text {}

```diff
@@ -1,9 +1,13 @@
 {% extends 'allianceauth/base.html' %} {% block content %}
 ****** Links Audit ******
     * Corporations
           o {% for corp in available %}
           o {{_corp.corporation_name_}}
           o {% endfor %}
+    * Apps
+          o {% for app, data in available_apps.items %}
+          o {{_data.field_label_}}
+          o {% endfor %}
 [search_string       ]
  {% block auditblock %}{% endblock auditblock %}
 {% endblock content %}
```

### Comparing `aa-charlink-0.4.1/charlink/templates/charlink/charlink.html` & `aa-charlink-0.5.0/charlink/templates/charlink/charlink.html`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 {% extends 'allianceauth/base.html' %}
 {% load bootstrap %}
+{% load charlinkutils %}
 
 {% block page_title %}Charlink{% endblock page_title %}
 
 {% block extra_css %}
     <style>
         .glyphicon-ok {
             color: green;
@@ -47,42 +48,44 @@
             <div class="panel-heading">
                 <h3 class="panel-title text-center">Linked Characters</h3>
             </div>
             <div class="panel-body">
                 <table class="table table-aa">
                     <thead>
                         <th class="text-center">Character</th>
-                        {% for app in characters_added.apps %}
-                            <th scope="row" class="text-center">{{ app }}</th>
+                        {% for app in characters_added.apps.values %}
+                            <th scope="row" class="text-center">{{ app.field_label }}</th>
                         {% endfor %}
                     </thead>
                     <tbody>
-                        {% for char, app_list in characters_added.characters.items %}
+                        {% for char in characters_added.characters %}
                             <tr>
                                 <td>{{ char }}</td>
-                                {% for is_added in app_list %}
-                                    {% if is_added %}
-                                        <td><span class="glyphicon glyphicon-ok"></span></td>
-                                    {% else %}
-                                        <td><span class="glyphicon glyphicon-remove"></span></td>
-                                    {% endif %}
+                                {% for app, data in characters_added.apps.items %}
+                                    {% with is_added=char|get_char_attr:app %}
+                                        {% if is_added %}
+                                            <td><span class="glyphicon glyphicon-ok"></span></td>
+                                        {% else %}
+                                            <td><span class="glyphicon glyphicon-remove"></span></td>
+                                        {% endif %}
+                                    {% endwith %}
                                 {% endfor %}
                             </tr>
                         {% endfor %}
                     </tbody>
                 </table>
             </div>
         </div>
 
         <div class="panel panel-success text-center">
             <div class="panel-heading">
                 <h3 class="panel-title text-center">Applications Info</h3>
             </div>
             <div class="panel-body">
-                {% for app in apps %}
+                {% for app in characters_added.apps.values %}
                     <span>{{ app.field_label }}</span>
                     <br><br>
                     <span>Scopes:</span>
                     {{ app.scopes|unordered_list|safe }}
                     {% if not forloop.last %}<hr>{% endif %}
                 {% endfor %}
             </div>
```

#### html2text {}

```diff
@@ -1,9 +1,10 @@
-{% extends 'allianceauth/base.html' %} {% load bootstrap %} {% block page_title
-%}Charlink{% endblock page_title %} {% block extra_css %}
+{% extends 'allianceauth/base.html' %} {% load bootstrap %} {% load
+charlinkutils %} {% block page_title %}Charlink{% endblock page_title %} {%
+block extra_css %}
  {% endblock extra_css %} {% block content %}
 ****** Character Linking ******
 {% if is_auditor %}
 **** Admin Section ****
 Auditing  
 {% endif %}
 **** Login Form ****
@@ -11,13 +12,13 @@
 eveonline website to authenticate and provide the token with all the scopes
 needed.
 
 {% csrf_token %} {{ form|bootstrap }} Login
 **** Linked Characters ****
 {{ char }}
 **** Applications Info ****
-{% for app in apps %} {{ app.field_label }}
+{% for app in characters_added.apps.values %} {{ app.field_label }}
 
 Scopes: {{ app.scopes|unordered_list|safe }} {% if not forloop.last %}
 ===============================================================================
 {% endif %} {% endfor %}
 {% endblock content %}
```

### Comparing `aa-charlink-0.4.1/charlink/templates/charlink/search.html` & `aa-charlink-0.5.0/charlink/templates/charlink/search.html`

 * *Files identical despite different names*

### Comparing `aa-charlink-0.4.1/charlink/views.py` & `aa-charlink-0.5.0/charlink/views.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-from django.shortcuts import render, redirect, get_object_or_404, HttpResponse
+from django.shortcuts import render, redirect, get_object_or_404
 from django.contrib.auth.decorators import login_required
 from django.contrib.auth.models import User
 from django.contrib import messages
 from django.db.models import Exists, OuterRef, Q
 from django.core.exceptions import PermissionDenied
+from django.http import Http404
 
 from allianceauth.services.hooks import get_extension_logger
 from allianceauth.eveonline.models import EveCharacter, EveCorporationInfo
 from allianceauth.authentication.decorators import permissions_required
 from allianceauth.authentication.models import CharacterOwnership
 
 from .forms import LinkForm
@@ -60,31 +61,43 @@
             corps = corps.filter(query)
         else:
             corps = corps.none()
 
     return corps
 
 
-def get_user_linked_chars(user: User):
-    characters = EveCharacter.objects.filter(character_ownership__user=user)
+def chars_annotate_linked_apps(characters, apps: dict):
+    for app, data in apps.items():
+        characters = characters.annotate(
+            **{app: data['is_character_added_annotation']}
+        )
+
+    return characters
+
+
+def get_user_available_apps(user: User):
     imported_apps = import_apps()
-    characters_added = {
-        'apps': [data['field_label'] for app, data in imported_apps.items() if app not in CHARLINK_IGNORE_APPS and user.has_perms(data['permissions'])],
-        'characters': {},
+
+    return {
+        app: data
+        for app, data in imported_apps.items()
+        if app not in CHARLINK_IGNORE_APPS and user.has_perms(data['permissions'])
     }
 
-    for character in characters:
-        characters_added['characters'][character.character_name] = []
-        for app, data in imported_apps.items():
-            if app not in CHARLINK_IGNORE_APPS and user.has_perms(data['permissions']):
-                characters_added['characters'][character.character_name].append(
-                    data['is_character_added'](character)
-                )
 
-    return characters_added
+def get_user_linked_chars(user: User):
+    available_apps = get_user_available_apps(user)
+
+    return {
+        'apps': available_apps,
+        'characters': chars_annotate_linked_apps(
+            EveCharacter.objects.filter(character_ownership__user=user),
+            available_apps
+        )
+    }
 
 
 @login_required
 def index(request):
     imported_apps = import_apps()
 
     if request.method == 'POST':
@@ -109,15 +122,14 @@
             return redirect('charlink:login')
 
     else:
         form = LinkForm(request.user)
 
     context = {
         'form': form,
-        'apps': [data for app, data in imported_apps.items() if app not in CHARLINK_IGNORE_APPS and request.user.has_perms(data['permissions'])],
         'characters_added': get_user_linked_chars(request.user),
         'is_auditor': request.user.has_perm('charlink.view_state') or request.user.has_perm('charlink.view_corp') or request.user.has_perm('charlink.view_alliance'),
     }
 
     return render(request, 'charlink/charlink.html', context=context)
 
 
@@ -166,14 +178,15 @@
             corp = corps.get(corporation_id=char.corporation_id)
         except EveCorporationInfo.DoesNotExist:
             pass
 
     context = {
         'available': corps,
         'selected': corp,
+        'available_apps': get_user_available_apps(request.user),
     }
 
     return render(request, 'charlink/audit.html', context=context)
 
 
 @login_required
 @permissions_required([
@@ -198,14 +211,15 @@
         .select_related('character_ownership__user__profile__main_character')
     )
 
     context = {
         'search_string': search_string,
         'characters': characters,
         'available': corps,
+        'available_apps': get_user_available_apps(request.user),
     }
 
     return render(request, 'charlink/search.html', context=context)
 
 
 @login_required
 @permissions_required([
@@ -230,10 +244,52 @@
         .exists()
     ):
         raise PermissionDenied('You do not have permission to view the selected user statistics.')
 
     context = {
         'characters_added': get_user_linked_chars(user),
         'available': corps,
+        'available_apps': get_user_available_apps(user),
     }
 
     return render(request, 'charlink/user_audit.html', context=context)
+
+
+@login_required
+@permissions_required([
+    'charlink.view_corp',
+    'charlink.view_alliance',
+    'charlink.view_state',
+])
+def audit_app(request, app):
+    imported_apps = import_apps()
+
+    if app not in imported_apps:
+        raise Http404()
+
+    app_data = imported_apps[app]
+
+    if not request.user.has_perms(app_data['permissions']):
+        raise PermissionDenied('You do not have permission to view the selected application statistics.')
+
+    corps = get_visible_corps(request.user)
+
+    visible_characters = EveCharacter.objects.filter(
+        Q(corporation_id__in=corps.values('corporation_id')) |
+        Q(character_ownership__user__profile__main_character__corporation_id__in=corps.values('corporation_id')),
+        character_ownership__isnull=False,
+    ).select_related('character_ownership__user__profile__main_character')
+
+    visible_characters = chars_annotate_linked_apps(
+        visible_characters,
+        {app: app_data}
+    ).order_by(app, 'character_name')
+
+    context = {
+        'characters': visible_characters,
+        'available': corps,
+        'app': app,
+        'app_data': app_data,
+        'available_apps': get_user_available_apps(request.user),
+    }
+
+    return render(request, 'charlink/app_audit.html', context=context)
```

### Comparing `aa-charlink-0.4.1/setup.cfg` & `aa-charlink-0.5.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.4.1
+current_version = 0.5.0
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(b(?P<beta>\d+))?
 serialize = 
 	{major}.{minor}.{patch}b{beta}
 	{major}.{minor}.{patch}
 commit = True
 tag = True
 sign_tags = True
```

