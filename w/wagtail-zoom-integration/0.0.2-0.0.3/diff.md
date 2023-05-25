# Comparing `tmp/wagtail-zoom-integration-0.0.2.tar.gz` & `tmp/wagtail-zoom-integration-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail-zoom-integration-0.0.2.tar", last modified: Thu May 25 14:50:44 2023, max compression
+gzip compressed data, was "wagtail-zoom-integration-0.0.3.tar", last modified: Thu May 25 20:00:45 2023, max compression
```

## Comparing `wagtail-zoom-integration-0.0.2.tar` & `wagtail-zoom-integration-0.0.3.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:50:44.575624 wagtail-zoom-integration-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-25 14:50:29.000000 wagtail-zoom-integration-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6317 2023-05-25 14:50:44.575624 wagtail-zoom-integration-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-05-25 14:50:29.000000 wagtail-zoom-integration-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-25 14:50:29.000000 wagtail-zoom-integration-0.0.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:50:44.559624 wagtail-zoom-integration-0.0.2/sandbox/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:50:29.000000 wagtail-zoom-integration-0.0.2/sandbox/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:50:44.559624 wagtail-zoom-integration-0.0.2/sandbox/home/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:50:29.000000 wagtail-zoom-integration-0.0.2/sandbox/home/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:50:44.563624 wagtail-zoom-integration-0.0.2/sandbox/home/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-05-25 14:50:29.000000 wagtail-zoom-integration-0.0.2/sandbox/home/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-05-25 14:50:29.000000 wagtail-zoom-integration-0.0.2/sandbox/home/migrations/0002_create_homepage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-05-25 14:50:29.000000 wagtail-zoom-integration-0.0.2/sandbox/home/migrations/0003_eventregistrationpage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-05-25 14:50:29.000000 wagtail-zoom-integration-0.0.2/sandbox/home/migrations/0004_formfield.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:50:29.000000 wagtail-zoom-integration-0.0.2/sandbox/home/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-05-25 14:50:29.000000 wagtail-zoom-integration-0.0.2/sandbox/home/models.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      254 2023-05-25 14:50:29.000000 wagtail-zoom-integration-0.0.2/sandbox/manage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:50:44.563624 wagtail-zoom-integration-0.0.2/sandbox/sandbox/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:50:29.000000 wagtail-zoom-integration-0.0.2/sandbox/sandbox/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:50:44.563624 wagtail-zoom-integration-0.0.2/sandbox/sandbox/settings/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:50:29.000000 wagtail-zoom-integration-0.0.2/sandbox/sandbox/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4541 2023-05-25 14:50:29.000000 wagtail-zoom-integration-0.0.2/sandbox/sandbox/settings/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-25 14:50:29.000000 wagtail-zoom-integration-0.0.2/sandbox/sandbox/settings/dev.py
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-25 14:50:29.000000 wagtail-zoom-integration-0.0.2/sandbox/sandbox/settings/production.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-05-25 14:50:29.000000 wagtail-zoom-integration-0.0.2/sandbox/sandbox/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-25 14:50:29.000000 wagtail-zoom-integration-0.0.2/sandbox/sandbox/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:50:44.567624 wagtail-zoom-integration-0.0.2/sandbox/search/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:50:29.000000 wagtail-zoom-integration-0.0.2/sandbox/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-05-25 14:50:29.000000 wagtail-zoom-integration-0.0.2/sandbox/search/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-25 14:50:44.575624 wagtail-zoom-integration-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:50:44.567624 wagtail-zoom-integration-0.0.2/wagtail_zoom_integration.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6317 2023-05-25 14:50:44.000000 wagtail-zoom-integration-0.0.2/wagtail_zoom_integration.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-05-25 14:50:44.000000 wagtail-zoom-integration-0.0.2/wagtail_zoom_integration.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 14:50:44.000000 wagtail-zoom-integration-0.0.2/wagtail_zoom_integration.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-25 14:50:44.000000 wagtail-zoom-integration-0.0.2/wagtail_zoom_integration.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-25 14:50:44.000000 wagtail-zoom-integration-0.0.2/wagtail_zoom_integration.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:50:44.571624 wagtail-zoom-integration-0.0.2/wagtailzoom/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:50:29.000000 wagtail-zoom-integration-0.0.2/wagtailzoom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-25 14:50:29.000000 wagtail-zoom-integration-0.0.2/wagtailzoom/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4760 2023-05-25 14:50:29.000000 wagtail-zoom-integration-0.0.2/wagtailzoom/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-25 14:50:29.000000 wagtail-zoom-integration-0.0.2/wagtailzoom/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-25 14:50:29.000000 wagtail-zoom-integration-0.0.2/wagtailzoom/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-05-25 14:50:29.000000 wagtail-zoom-integration-0.0.2/wagtailzoom/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:50:44.571624 wagtail-zoom-integration-0.0.2/wagtailzoom/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-05-25 14:50:29.000000 wagtail-zoom-integration-0.0.2/wagtailzoom/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:50:29.000000 wagtail-zoom-integration-0.0.2/wagtailzoom/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6153 2023-05-25 14:50:29.000000 wagtail-zoom-integration-0.0.2/wagtailzoom/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:50:44.559624 wagtail-zoom-integration-0.0.2/wagtailzoom/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:50:44.571624 wagtail-zoom-integration-0.0.2/wagtailzoom/templates/wagtailzoom/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:50:44.575624 wagtail-zoom-integration-0.0.2/wagtailzoom/templates/wagtailzoom/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-05-25 14:50:29.000000 wagtail-zoom-integration-0.0.2/wagtailzoom/templates/wagtailzoom/widgets/zoom_event_select_widget.html
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-05-25 14:50:29.000000 wagtail-zoom-integration-0.0.2/wagtailzoom/templates/wagtailzoom/widgets/zoom_event_select_widget_js.html
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-05-25 14:50:29.000000 wagtail-zoom-integration-0.0.2/wagtailzoom/templates/wagtailzoom/zoom_integration_form.html
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-25 14:50:29.000000 wagtail-zoom-integration-0.0.2/wagtailzoom/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-05-25 14:50:29.000000 wagtail-zoom-integration-0.0.2/wagtailzoom/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-05-25 14:50:29.000000 wagtail-zoom-integration-0.0.2/wagtailzoom/wagtail_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-05-25 14:50:29.000000 wagtail-zoom-integration-0.0.2/wagtailzoom/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:00:45.492581 wagtail-zoom-integration-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-25 20:00:29.000000 wagtail-zoom-integration-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6317 2023-05-25 20:00:45.492581 wagtail-zoom-integration-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-05-25 20:00:29.000000 wagtail-zoom-integration-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-25 20:00:29.000000 wagtail-zoom-integration-0.0.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:00:45.480581 wagtail-zoom-integration-0.0.3/sandbox/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 20:00:29.000000 wagtail-zoom-integration-0.0.3/sandbox/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:00:45.480581 wagtail-zoom-integration-0.0.3/sandbox/home/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 20:00:29.000000 wagtail-zoom-integration-0.0.3/sandbox/home/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:00:45.480581 wagtail-zoom-integration-0.0.3/sandbox/home/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-05-25 20:00:29.000000 wagtail-zoom-integration-0.0.3/sandbox/home/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-05-25 20:00:29.000000 wagtail-zoom-integration-0.0.3/sandbox/home/migrations/0002_create_homepage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-05-25 20:00:29.000000 wagtail-zoom-integration-0.0.3/sandbox/home/migrations/0003_eventregistrationpage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-05-25 20:00:29.000000 wagtail-zoom-integration-0.0.3/sandbox/home/migrations/0004_formfield.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 20:00:29.000000 wagtail-zoom-integration-0.0.3/sandbox/home/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-05-25 20:00:29.000000 wagtail-zoom-integration-0.0.3/sandbox/home/models.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      254 2023-05-25 20:00:29.000000 wagtail-zoom-integration-0.0.3/sandbox/manage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:00:45.484581 wagtail-zoom-integration-0.0.3/sandbox/sandbox/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 20:00:29.000000 wagtail-zoom-integration-0.0.3/sandbox/sandbox/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:00:45.484581 wagtail-zoom-integration-0.0.3/sandbox/sandbox/settings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 20:00:29.000000 wagtail-zoom-integration-0.0.3/sandbox/sandbox/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4541 2023-05-25 20:00:29.000000 wagtail-zoom-integration-0.0.3/sandbox/sandbox/settings/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-25 20:00:29.000000 wagtail-zoom-integration-0.0.3/sandbox/sandbox/settings/dev.py
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-25 20:00:29.000000 wagtail-zoom-integration-0.0.3/sandbox/sandbox/settings/production.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-05-25 20:00:29.000000 wagtail-zoom-integration-0.0.3/sandbox/sandbox/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-25 20:00:29.000000 wagtail-zoom-integration-0.0.3/sandbox/sandbox/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:00:45.484581 wagtail-zoom-integration-0.0.3/sandbox/search/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 20:00:29.000000 wagtail-zoom-integration-0.0.3/sandbox/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-05-25 20:00:29.000000 wagtail-zoom-integration-0.0.3/sandbox/search/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-25 20:00:45.492581 wagtail-zoom-integration-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:00:45.484581 wagtail-zoom-integration-0.0.3/wagtail_zoom_integration.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6317 2023-05-25 20:00:45.000000 wagtail-zoom-integration-0.0.3/wagtail_zoom_integration.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-05-25 20:00:45.000000 wagtail-zoom-integration-0.0.3/wagtail_zoom_integration.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 20:00:45.000000 wagtail-zoom-integration-0.0.3/wagtail_zoom_integration.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-25 20:00:45.000000 wagtail-zoom-integration-0.0.3/wagtail_zoom_integration.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-25 20:00:45.000000 wagtail-zoom-integration-0.0.3/wagtail_zoom_integration.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:00:45.488582 wagtail-zoom-integration-0.0.3/wagtailzoom/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 20:00:29.000000 wagtail-zoom-integration-0.0.3/wagtailzoom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-25 20:00:29.000000 wagtail-zoom-integration-0.0.3/wagtailzoom/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4760 2023-05-25 20:00:29.000000 wagtail-zoom-integration-0.0.3/wagtailzoom/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-25 20:00:29.000000 wagtail-zoom-integration-0.0.3/wagtailzoom/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-25 20:00:29.000000 wagtail-zoom-integration-0.0.3/wagtailzoom/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-05-25 20:00:29.000000 wagtail-zoom-integration-0.0.3/wagtailzoom/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:00:45.488582 wagtail-zoom-integration-0.0.3/wagtailzoom/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-05-25 20:00:29.000000 wagtail-zoom-integration-0.0.3/wagtailzoom/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 20:00:29.000000 wagtail-zoom-integration-0.0.3/wagtailzoom/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6187 2023-05-25 20:00:29.000000 wagtail-zoom-integration-0.0.3/wagtailzoom/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:00:45.476581 wagtail-zoom-integration-0.0.3/wagtailzoom/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:00:45.488582 wagtail-zoom-integration-0.0.3/wagtailzoom/templates/wagtailzoom/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:00:45.488582 wagtail-zoom-integration-0.0.3/wagtailzoom/templates/wagtailzoom/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-05-25 20:00:29.000000 wagtail-zoom-integration-0.0.3/wagtailzoom/templates/wagtailzoom/widgets/zoom_event_select_widget.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-05-25 20:00:29.000000 wagtail-zoom-integration-0.0.3/wagtailzoom/templates/wagtailzoom/widgets/zoom_event_select_widget_js.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-05-25 20:00:29.000000 wagtail-zoom-integration-0.0.3/wagtailzoom/templates/wagtailzoom/zoom_integration_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-25 20:00:29.000000 wagtail-zoom-integration-0.0.3/wagtailzoom/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-05-25 20:00:29.000000 wagtail-zoom-integration-0.0.3/wagtailzoom/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-05-25 20:00:29.000000 wagtail-zoom-integration-0.0.3/wagtailzoom/wagtail_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-05-25 20:00:29.000000 wagtail-zoom-integration-0.0.3/wagtailzoom/widgets.py
```

### Comparing `wagtail-zoom-integration-0.0.2/PKG-INFO` & `wagtail-zoom-integration-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-zoom-integration
-Version: 0.0.2
+Version: 0.0.3
 Summary: Integrate Zoom Event registration registration in Wagtail Projects.
 Home-page: https://github.com/wmo-raf/wagtail-zoom-integration
 Author: Erick Otenyo
 Author-email: otenyo.erick@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `wagtail-zoom-integration-0.0.2/README.md` & `wagtail-zoom-integration-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `wagtail-zoom-integration-0.0.2/sandbox/home/migrations/0001_initial.py` & `wagtail-zoom-integration-0.0.3/sandbox/home/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail-zoom-integration-0.0.2/sandbox/home/migrations/0002_create_homepage.py` & `wagtail-zoom-integration-0.0.3/sandbox/home/migrations/0002_create_homepage.py`

 * *Files identical despite different names*

### Comparing `wagtail-zoom-integration-0.0.2/sandbox/home/migrations/0003_eventregistrationpage.py` & `wagtail-zoom-integration-0.0.3/sandbox/home/migrations/0003_eventregistrationpage.py`

 * *Files identical despite different names*

### Comparing `wagtail-zoom-integration-0.0.2/sandbox/home/migrations/0004_formfield.py` & `wagtail-zoom-integration-0.0.3/sandbox/home/migrations/0004_formfield.py`

 * *Files identical despite different names*

### Comparing `wagtail-zoom-integration-0.0.2/sandbox/home/models.py` & `wagtail-zoom-integration-0.0.3/sandbox/home/models.py`

 * *Files identical despite different names*

### Comparing `wagtail-zoom-integration-0.0.2/sandbox/sandbox/settings/base.py` & `wagtail-zoom-integration-0.0.3/sandbox/sandbox/settings/base.py`

 * *Files identical despite different names*

### Comparing `wagtail-zoom-integration-0.0.2/sandbox/sandbox/urls.py` & `wagtail-zoom-integration-0.0.3/sandbox/sandbox/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail-zoom-integration-0.0.2/sandbox/search/views.py` & `wagtail-zoom-integration-0.0.3/sandbox/search/views.py`

 * *Files identical despite different names*

### Comparing `wagtail-zoom-integration-0.0.2/setup.cfg` & `wagtail-zoom-integration-0.0.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = wagtail-zoom-integration
-version = 0.0.2
+version = 0.0.3
 description = Integrate Zoom Event registration registration in Wagtail Projects.
 long_description = file:README.md
 long_description_content_type = text/markdown
 url = https://github.com/wmo-raf/wagtail-zoom-integration
 author = Erick Otenyo
 author_email = otenyo.erick@gmail.com
 license = MIT
```

### Comparing `wagtail-zoom-integration-0.0.2/wagtail_zoom_integration.egg-info/PKG-INFO` & `wagtail-zoom-integration-0.0.3/wagtail_zoom_integration.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-zoom-integration
-Version: 0.0.2
+Version: 0.0.3
 Summary: Integrate Zoom Event registration registration in Wagtail Projects.
 Home-page: https://github.com/wmo-raf/wagtail-zoom-integration
 Author: Erick Otenyo
 Author-email: otenyo.erick@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `wagtail-zoom-integration-0.0.2/wagtail_zoom_integration.egg-info/SOURCES.txt` & `wagtail-zoom-integration-0.0.3/wagtail_zoom_integration.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wagtail-zoom-integration-0.0.2/wagtailzoom/api.py` & `wagtail-zoom-integration-0.0.3/wagtailzoom/api.py`

 * *Files identical despite different names*

### Comparing `wagtail-zoom-integration-0.0.2/wagtailzoom/forms.py` & `wagtail-zoom-integration-0.0.3/wagtailzoom/forms.py`

 * *Files identical despite different names*

### Comparing `wagtail-zoom-integration-0.0.2/wagtailzoom/migrations/0001_initial.py` & `wagtail-zoom-integration-0.0.3/wagtailzoom/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail-zoom-integration-0.0.2/wagtailzoom/models.py` & `wagtail-zoom-integration-0.0.3/wagtailzoom/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,20 +37,21 @@
         FieldPanel("api_key"),
         FieldPanel("api_secret"),
     ]
 
 
 class AbstractZoomIntegrationForm(AbstractForm):
     zoom_event = models.TextField(blank=True, null=True, verbose_name=_('Zoom Event'), help_text=_('Select Zoom Event'))
-
     zoom_reg_fields_mapping = models.TextField(blank=True, null=True)
 
     integration_panels = [
         FieldPanel("zoom_event", widget=ZoomEventSelectWidget),
     ]
+    
+    integration_name = "zoom"
 
     class Meta:
         abstract = True
 
     @property
     def zoom_event_id(self):
         return self.get_data().get("event_id")
```

### Comparing `wagtail-zoom-integration-0.0.2/wagtailzoom/templates/wagtailzoom/widgets/zoom_event_select_widget.html` & `wagtail-zoom-integration-0.0.3/wagtailzoom/templates/wagtailzoom/widgets/zoom_event_select_widget.html`

 * *Files identical despite different names*

### Comparing `wagtail-zoom-integration-0.0.2/wagtailzoom/templates/wagtailzoom/widgets/zoom_event_select_widget_js.html` & `wagtail-zoom-integration-0.0.3/wagtailzoom/templates/wagtailzoom/widgets/zoom_event_select_widget_js.html`

 * *Files identical despite different names*

### Comparing `wagtail-zoom-integration-0.0.2/wagtailzoom/templates/wagtailzoom/zoom_integration_form.html` & `wagtail-zoom-integration-0.0.3/wagtailzoom/templates/wagtailzoom/zoom_integration_form.html`

 * *Files identical despite different names*

### Comparing `wagtail-zoom-integration-0.0.2/wagtailzoom/views.py` & `wagtail-zoom-integration-0.0.3/wagtailzoom/views.py`

 * *Files identical despite different names*

### Comparing `wagtail-zoom-integration-0.0.2/wagtailzoom/wagtail_hooks.py` & `wagtail-zoom-integration-0.0.3/wagtailzoom/wagtail_hooks.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,40 +2,39 @@
 from django.utils.translation import gettext_lazy as _
 from modelcluster.models import get_all_child_relations
 from wagtail import hooks
 from wagtail.admin import messages
 from wagtail.admin import widgets as wagtail_admin_widgets
 from wagtail.contrib.forms.models import AbstractFormField
 
-from .models import AbstractZoomIntegrationForm
 from .views import zoom_integration_view
 
 
 @hooks.register('register_admin_urls')
 def urlconf_wagtail_zoom():
     return [
         path('zoom-integration/<int:page_id>', zoom_integration_view, name="zoom_integration_view"),
     ]
 
 
 @hooks.register('register_page_listing_buttons')
 def page_listing_buttons(page, page_perms, next_url=None):
-    if isinstance(page, AbstractZoomIntegrationForm):
+    if hasattr(page, "integration_name") and page.integration_name == "zoom":
         if page.zoom_event_id:
             url = reverse("zoom_integration_view", args=[page.pk, ])
             yield wagtail_admin_widgets.PageListingButton(
                 "Zoom Integration",
                 url,
                 priority=40
             )
 
 
 @hooks.register('after_publish_page')
 def show_zoom_integration_fields_warning(request, page):
-    if isinstance(page, AbstractZoomIntegrationForm):
+    if hasattr(page, "integration_name") and page.integration_name == "zoom":
         form_fields_changed = False
 
         if page.zoom_event_id:
             if page.zoom_reg_fields_mapping:
                 form_fields_rel_name = None
                 # get form fields relation name
                 relations = get_all_child_relations(page)
```

### Comparing `wagtail-zoom-integration-0.0.2/wagtailzoom/widgets.py` & `wagtail-zoom-integration-0.0.3/wagtailzoom/widgets.py`

 * *Files identical despite different names*

