# Comparing `tmp/mitol-django-google-sheets-deferrals-2023.5.23.tar.gz` & `tmp/mitol-django-google-sheets-deferrals-2023.5.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mitol-django-google-sheets-deferrals-2023.5.23.tar", last modified: Tue May 23 13:20:13 2023, max compression
+gzip compressed data, was "mitol-django-google-sheets-deferrals-2023.5.25.tar", last modified: Thu May 25 10:53:11 2023, max compression
```

## Comparing `mitol-django-google-sheets-deferrals-2023.5.23.tar` & `mitol-django-google-sheets-deferrals-2023.5.25.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 13:20:13.346642 mitol-django-google-sheets-deferrals-2023.5.23/
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-05-23 13:20:12.000000 mitol-django-google-sheets-deferrals-2023.5.23/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     4652 2023-05-23 13:20:13.346642 mitol-django-google-sheets-deferrals-2023.5.23/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      625 2023-05-23 13:20:12.000000 mitol-django-google-sheets-deferrals-2023.5.23/backend_shim.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 13:20:13.346642 mitol-django-google-sheets-deferrals-2023.5.23/mitol/
--rw-r--r--   0 runner    (1001) docker     (122)       56 2023-05-23 13:20:12.000000 mitol-django-google-sheets-deferrals-2023.5.23/mitol/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 13:20:13.346642 mitol-django-google-sheets-deferrals-2023.5.23/mitol/google_sheets_deferrals/
--rw-r--r--   0 runner    (1001) docker     (122)      384 2023-05-23 13:20:12.000000 mitol-django-google-sheets-deferrals-2023.5.23/mitol/google_sheets_deferrals/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (122)     4105 2023-05-23 13:20:12.000000 mitol-django-google-sheets-deferrals-2023.5.23/mitol/google_sheets_deferrals/README.md
--rw-r--r--   0 runner    (1001) docker     (122)      210 2023-05-23 13:20:12.000000 mitol-django-google-sheets-deferrals-2023.5.23/mitol/google_sheets_deferrals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4958 2023-05-23 13:20:12.000000 mitol-django-google-sheets-deferrals-2023.5.23/mitol/google_sheets_deferrals/api.py
--rw-r--r--   0 runner    (1001) docker     (122)      454 2023-05-23 13:20:12.000000 mitol-django-google-sheets-deferrals-2023.5.23/mitol/google_sheets_deferrals/apps.py
--rw-r--r--   0 runner    (1001) docker     (122)      276 2023-05-23 13:20:12.000000 mitol-django-google-sheets-deferrals-2023.5.23/mitol/google_sheets_deferrals/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)      838 2023-05-23 13:20:12.000000 mitol-django-google-sheets-deferrals-2023.5.23/mitol/google_sheets_deferrals/hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 13:20:13.346642 mitol-django-google-sheets-deferrals-2023.5.23/mitol/google_sheets_deferrals/management/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 13:20:13.346642 mitol-django-google-sheets-deferrals-2023.5.23/mitol/google_sheets_deferrals/management/commands/
--rw-r--r--   0 runner    (1001) docker     (122)     1067 2023-05-23 13:20:12.000000 mitol-django-google-sheets-deferrals-2023.5.23/mitol/google_sheets_deferrals/management/commands/process_deferral_requests.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 13:20:13.346642 mitol-django-google-sheets-deferrals-2023.5.23/mitol/google_sheets_deferrals/migrations/
--rw-r--r--   0 runner    (1001) docker     (122)     1081 2023-05-23 13:20:12.000000 mitol-django-google-sheets-deferrals-2023.5.23/mitol/google_sheets_deferrals/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-23 13:20:12.000000 mitol-django-google-sheets-deferrals-2023.5.23/mitol/google_sheets_deferrals/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      400 2023-05-23 13:20:12.000000 mitol-django-google-sheets-deferrals-2023.5.23/mitol/google_sheets_deferrals/models.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-23 13:20:12.000000 mitol-django-google-sheets-deferrals-2023.5.23/mitol/google_sheets_deferrals/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 13:20:13.346642 mitol-django-google-sheets-deferrals-2023.5.23/mitol/google_sheets_deferrals/settings/
--rw-r--r--   0 runner    (1001) docker     (122)     1942 2023-05-23 13:20:12.000000 mitol-django-google-sheets-deferrals-2023.5.23/mitol/google_sheets_deferrals/settings/google_sheets_deferrals.py
--rw-r--r--   0 runner    (1001) docker     (122)     4433 2023-05-23 13:20:12.000000 mitol-django-google-sheets-deferrals-2023.5.23/mitol/google_sheets_deferrals/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 13:20:13.346642 mitol-django-google-sheets-deferrals-2023.5.23/mitol_django_google_sheets_deferrals.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     4652 2023-05-23 13:20:13.000000 mitol-django-google-sheets-deferrals-2023.5.23/mitol_django_google_sheets_deferrals.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1132 2023-05-23 13:20:13.000000 mitol-django-google-sheets-deferrals-2023.5.23/mitol_django_google_sheets_deferrals.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-23 13:20:13.000000 mitol-django-google-sheets-deferrals-2023.5.23/mitol_django_google_sheets_deferrals.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-05-23 13:20:13.000000 mitol-django-google-sheets-deferrals-2023.5.23/mitol_django_google_sheets_deferrals.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (122)       93 2023-05-23 13:20:13.000000 mitol-django-google-sheets-deferrals-2023.5.23/mitol_django_google_sheets_deferrals.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-05-23 13:20:13.000000 mitol-django-google-sheets-deferrals-2023.5.23/mitol_django_google_sheets_deferrals.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-23 13:20:13.000000 mitol-django-google-sheets-deferrals-2023.5.23/mitol_django_google_sheets_deferrals.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-23 13:20:13.346642 mitol-django-google-sheets-deferrals-2023.5.23/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     5673 2023-05-23 13:20:12.000000 mitol-django-google-sheets-deferrals-2023.5.23/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:53:11.146418 mitol-django-google-sheets-deferrals-2023.5.25/
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-05-25 10:53:10.000000 mitol-django-google-sheets-deferrals-2023.5.25/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     4652 2023-05-25 10:53:11.146418 mitol-django-google-sheets-deferrals-2023.5.25/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      625 2023-05-25 10:53:10.000000 mitol-django-google-sheets-deferrals-2023.5.25/backend_shim.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:53:11.146418 mitol-django-google-sheets-deferrals-2023.5.25/mitol/
+-rw-r--r--   0 runner    (1001) docker     (122)       56 2023-05-25 10:53:10.000000 mitol-django-google-sheets-deferrals-2023.5.25/mitol/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:53:11.146418 mitol-django-google-sheets-deferrals-2023.5.25/mitol/google_sheets_deferrals/
+-rw-r--r--   0 runner    (1001) docker     (122)      600 2023-05-25 10:53:10.000000 mitol-django-google-sheets-deferrals-2023.5.25/mitol/google_sheets_deferrals/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (122)     4105 2023-05-25 10:53:10.000000 mitol-django-google-sheets-deferrals-2023.5.25/mitol/google_sheets_deferrals/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      210 2023-05-25 10:53:10.000000 mitol-django-google-sheets-deferrals-2023.5.25/mitol/google_sheets_deferrals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4958 2023-05-25 10:53:10.000000 mitol-django-google-sheets-deferrals-2023.5.25/mitol/google_sheets_deferrals/api.py
+-rw-r--r--   0 runner    (1001) docker     (122)      511 2023-05-25 10:53:10.000000 mitol-django-google-sheets-deferrals-2023.5.25/mitol/google_sheets_deferrals/apps.py
+-rw-r--r--   0 runner    (1001) docker     (122)      276 2023-05-25 10:53:10.000000 mitol-django-google-sheets-deferrals-2023.5.25/mitol/google_sheets_deferrals/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)      838 2023-05-25 10:53:10.000000 mitol-django-google-sheets-deferrals-2023.5.25/mitol/google_sheets_deferrals/hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:53:11.142418 mitol-django-google-sheets-deferrals-2023.5.25/mitol/google_sheets_deferrals/management/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:53:11.146418 mitol-django-google-sheets-deferrals-2023.5.25/mitol/google_sheets_deferrals/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)     1067 2023-05-25 10:53:10.000000 mitol-django-google-sheets-deferrals-2023.5.25/mitol/google_sheets_deferrals/management/commands/process_deferral_requests.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:53:11.146418 mitol-django-google-sheets-deferrals-2023.5.25/mitol/google_sheets_deferrals/migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)     1081 2023-05-25 10:53:10.000000 mitol-django-google-sheets-deferrals-2023.5.25/mitol/google_sheets_deferrals/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 10:53:10.000000 mitol-django-google-sheets-deferrals-2023.5.25/mitol/google_sheets_deferrals/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      400 2023-05-25 10:53:10.000000 mitol-django-google-sheets-deferrals-2023.5.25/mitol/google_sheets_deferrals/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 10:53:10.000000 mitol-django-google-sheets-deferrals-2023.5.25/mitol/google_sheets_deferrals/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:53:11.146418 mitol-django-google-sheets-deferrals-2023.5.25/mitol/google_sheets_deferrals/settings/
+-rw-r--r--   0 runner    (1001) docker     (122)     1942 2023-05-25 10:53:10.000000 mitol-django-google-sheets-deferrals-2023.5.25/mitol/google_sheets_deferrals/settings/google_sheets_deferrals.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4433 2023-05-25 10:53:10.000000 mitol-django-google-sheets-deferrals-2023.5.25/mitol/google_sheets_deferrals/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:53:11.146418 mitol-django-google-sheets-deferrals-2023.5.25/mitol_django_google_sheets_deferrals.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     4652 2023-05-25 10:53:11.000000 mitol-django-google-sheets-deferrals-2023.5.25/mitol_django_google_sheets_deferrals.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1132 2023-05-25 10:53:11.000000 mitol-django-google-sheets-deferrals-2023.5.25/mitol_django_google_sheets_deferrals.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-25 10:53:11.000000 mitol-django-google-sheets-deferrals-2023.5.25/mitol_django_google_sheets_deferrals.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-05-25 10:53:11.000000 mitol-django-google-sheets-deferrals-2023.5.25/mitol_django_google_sheets_deferrals.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       93 2023-05-25 10:53:11.000000 mitol-django-google-sheets-deferrals-2023.5.25/mitol_django_google_sheets_deferrals.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-05-25 10:53:11.000000 mitol-django-google-sheets-deferrals-2023.5.25/mitol_django_google_sheets_deferrals.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-25 10:53:11.000000 mitol-django-google-sheets-deferrals-2023.5.25/mitol_django_google_sheets_deferrals.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-25 10:53:11.146418 mitol-django-google-sheets-deferrals-2023.5.25/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     5673 2023-05-25 10:53:10.000000 mitol-django-google-sheets-deferrals-2023.5.25/setup.py
```

### Comparing `mitol-django-google-sheets-deferrals-2023.5.23/PKG-INFO` & `mitol-django-google-sheets-deferrals-2023.5.25/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mitol-django-google-sheets-deferrals
-Version: 2023.5.23
+Version: 2023.5.25
 Summary: Library to handle Deferral requests using Google Sheets integrations in Django
 License: BSD 3-Clause License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `mitol-django-google-sheets-deferrals-2023.5.23/backend_shim.py` & `mitol-django-google-sheets-deferrals-2023.5.25/backend_shim.py`

 * *Files identical despite different names*

### Comparing `mitol-django-google-sheets-deferrals-2023.5.23/mitol/google_sheets_deferrals/README.md` & `mitol-django-google-sheets-deferrals-2023.5.25/mitol/google_sheets_deferrals/README.md`

 * *Files identical despite different names*

### Comparing `mitol-django-google-sheets-deferrals-2023.5.23/mitol/google_sheets_deferrals/api.py` & `mitol-django-google-sheets-deferrals-2023.5.25/mitol/google_sheets_deferrals/api.py`

 * *Files identical despite different names*

### Comparing `mitol-django-google-sheets-deferrals-2023.5.23/mitol/google_sheets_deferrals/hooks.py` & `mitol-django-google-sheets-deferrals-2023.5.25/mitol/google_sheets_deferrals/hooks.py`

 * *Files identical despite different names*

### Comparing `mitol-django-google-sheets-deferrals-2023.5.23/mitol/google_sheets_deferrals/management/commands/process_deferral_requests.py` & `mitol-django-google-sheets-deferrals-2023.5.25/mitol/google_sheets_deferrals/management/commands/process_deferral_requests.py`

 * *Files identical despite different names*

### Comparing `mitol-django-google-sheets-deferrals-2023.5.23/mitol/google_sheets_deferrals/migrations/0001_initial.py` & `mitol-django-google-sheets-deferrals-2023.5.25/mitol/google_sheets_deferrals/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `mitol-django-google-sheets-deferrals-2023.5.23/mitol/google_sheets_deferrals/settings/google_sheets_deferrals.py` & `mitol-django-google-sheets-deferrals-2023.5.25/mitol/google_sheets_deferrals/settings/google_sheets_deferrals.py`

 * *Files identical despite different names*

### Comparing `mitol-django-google-sheets-deferrals-2023.5.23/mitol/google_sheets_deferrals/utils.py` & `mitol-django-google-sheets-deferrals-2023.5.25/mitol/google_sheets_deferrals/utils.py`

 * *Files identical despite different names*

### Comparing `mitol-django-google-sheets-deferrals-2023.5.23/mitol_django_google_sheets_deferrals.egg-info/PKG-INFO` & `mitol-django-google-sheets-deferrals-2023.5.25/mitol_django_google_sheets_deferrals.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mitol-django-google-sheets-deferrals
-Version: 2023.5.23
+Version: 2023.5.25
 Summary: Library to handle Deferral requests using Google Sheets integrations in Django
 License: BSD 3-Clause License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `mitol-django-google-sheets-deferrals-2023.5.23/mitol_django_google_sheets_deferrals.egg-info/SOURCES.txt` & `mitol-django-google-sheets-deferrals-2023.5.25/mitol_django_google_sheets_deferrals.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mitol-django-google-sheets-deferrals-2023.5.23/setup.py` & `mitol-django-google-sheets-deferrals-2023.5.25/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -152,10 +152,10 @@
         'mitol',
         'mitol.google_sheets_deferrals',
         'mitol.google_sheets_deferrals.management.commands',
         'mitol.google_sheets_deferrals.migrations',
         'mitol.google_sheets_deferrals.settings',
     ),
     'python_requires': '>=3.8',
-    'version': '2023.5.23',
+    'version': '2023.5.25',
     'zip_safe': True,
 })
```

