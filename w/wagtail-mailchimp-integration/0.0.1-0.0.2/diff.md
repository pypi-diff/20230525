# Comparing `tmp/wagtail-mailchimp-integration-0.0.1.tar.gz` & `tmp/wagtail-mailchimp-integration-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail-mailchimp-integration-0.0.1.tar", last modified: Wed May 24 11:04:02 2023, max compression
+gzip compressed data, was "wagtail-mailchimp-integration-0.0.2.tar", last modified: Thu May 25 11:15:08 2023, max compression
```

## Comparing `wagtail-mailchimp-integration-0.0.1.tar` & `wagtail-mailchimp-integration-0.0.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:04:02.641164 wagtail-mailchimp-integration-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-24 11:03:45.000000 wagtail-mailchimp-integration-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-24 11:03:45.000000 wagtail-mailchimp-integration-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7815 2023-05-24 11:04:02.641164 wagtail-mailchimp-integration-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6886 2023-05-24 11:03:45.000000 wagtail-mailchimp-integration-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-24 11:03:45.000000 wagtail-mailchimp-integration-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-05-24 11:04:02.641164 wagtail-mailchimp-integration-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:04:02.637164 wagtail-mailchimp-integration-0.0.1/wagtail_mailchimp_integration.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7815 2023-05-24 11:04:02.000000 wagtail-mailchimp-integration-0.0.1/wagtail_mailchimp_integration.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-05-24 11:04:02.000000 wagtail-mailchimp-integration-0.0.1/wagtail_mailchimp_integration.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 11:04:02.000000 wagtail-mailchimp-integration-0.0.1/wagtail_mailchimp_integration.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-24 11:04:02.000000 wagtail-mailchimp-integration-0.0.1/wagtail_mailchimp_integration.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-24 11:04:02.000000 wagtail-mailchimp-integration-0.0.1/wagtail_mailchimp_integration.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:04:02.637164 wagtail-mailchimp-integration-0.0.1/wagtailmailchimp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 11:03:45.000000 wagtail-mailchimp-integration-0.0.1/wagtailmailchimp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-24 11:03:45.000000 wagtail-mailchimp-integration-0.0.1/wagtailmailchimp/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-05-24 11:03:45.000000 wagtail-mailchimp-integration-0.0.1/wagtailmailchimp/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-24 11:03:45.000000 wagtail-mailchimp-integration-0.0.1/wagtailmailchimp/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)    10374 2023-05-24 11:03:45.000000 wagtail-mailchimp-integration-0.0.1/wagtailmailchimp/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:04:02.637164 wagtail-mailchimp-integration-0.0.1/wagtailmailchimp/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-24 11:03:45.000000 wagtail-mailchimp-integration-0.0.1/wagtailmailchimp/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 11:03:45.000000 wagtail-mailchimp-integration-0.0.1/wagtailmailchimp/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12047 2023-05-24 11:03:45.000000 wagtail-mailchimp-integration-0.0.1/wagtailmailchimp/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:04:02.637164 wagtail-mailchimp-integration-0.0.1/wagtailmailchimp/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:04:02.637164 wagtail-mailchimp-integration-0.0.1/wagtailmailchimp/templates/wagtailmailchimp/
--rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-05-24 11:03:45.000000 wagtail-mailchimp-integration-0.0.1/wagtailmailchimp/templates/wagtailmailchimp/mailchimp_integration_form.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:04:02.637164 wagtail-mailchimp-integration-0.0.1/wagtailmailchimp/templates/wagtailmailchimp/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-05-24 11:03:45.000000 wagtail-mailchimp-integration-0.0.1/wagtailmailchimp/templates/wagtailmailchimp/widgets/subscriber_optin_widget.html
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-24 11:03:45.000000 wagtail-mailchimp-integration-0.0.1/wagtailmailchimp/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    11372 2023-05-24 11:03:45.000000 wagtail-mailchimp-integration-0.0.1/wagtailmailchimp/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-24 11:03:45.000000 wagtail-mailchimp-integration-0.0.1/wagtailmailchimp/wagtail_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-05-24 11:03:45.000000 wagtail-mailchimp-integration-0.0.1/wagtailmailchimp/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:15:08.755812 wagtail-mailchimp-integration-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-25 11:14:49.000000 wagtail-mailchimp-integration-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-25 11:14:49.000000 wagtail-mailchimp-integration-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7815 2023-05-25 11:15:08.755812 wagtail-mailchimp-integration-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6886 2023-05-25 11:14:49.000000 wagtail-mailchimp-integration-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-25 11:14:49.000000 wagtail-mailchimp-integration-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-05-25 11:15:08.755812 wagtail-mailchimp-integration-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:15:08.751811 wagtail-mailchimp-integration-0.0.2/wagtail_mailchimp_integration.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7815 2023-05-25 11:15:08.000000 wagtail-mailchimp-integration-0.0.2/wagtail_mailchimp_integration.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-05-25 11:15:08.000000 wagtail-mailchimp-integration-0.0.2/wagtail_mailchimp_integration.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 11:15:08.000000 wagtail-mailchimp-integration-0.0.2/wagtail_mailchimp_integration.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-25 11:15:08.000000 wagtail-mailchimp-integration-0.0.2/wagtail_mailchimp_integration.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-25 11:15:08.000000 wagtail-mailchimp-integration-0.0.2/wagtail_mailchimp_integration.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:15:08.751811 wagtail-mailchimp-integration-0.0.2/wagtailmailchimp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 11:14:49.000000 wagtail-mailchimp-integration-0.0.2/wagtailmailchimp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-25 11:14:49.000000 wagtail-mailchimp-integration-0.0.2/wagtailmailchimp/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-05-25 11:14:49.000000 wagtail-mailchimp-integration-0.0.2/wagtailmailchimp/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-25 11:14:49.000000 wagtail-mailchimp-integration-0.0.2/wagtailmailchimp/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10374 2023-05-25 11:14:49.000000 wagtail-mailchimp-integration-0.0.2/wagtailmailchimp/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:15:08.751811 wagtail-mailchimp-integration-0.0.2/wagtailmailchimp/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-05-25 11:14:49.000000 wagtail-mailchimp-integration-0.0.2/wagtailmailchimp/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 11:14:49.000000 wagtail-mailchimp-integration-0.0.2/wagtailmailchimp/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12047 2023-05-25 11:14:49.000000 wagtail-mailchimp-integration-0.0.2/wagtailmailchimp/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:15:08.743811 wagtail-mailchimp-integration-0.0.2/wagtailmailchimp/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:15:08.751811 wagtail-mailchimp-integration-0.0.2/wagtailmailchimp/templates/wagtailmailchimp/
+-rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-05-25 11:14:49.000000 wagtail-mailchimp-integration-0.0.2/wagtailmailchimp/templates/wagtailmailchimp/mailchimp_integration_form.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:15:08.755812 wagtail-mailchimp-integration-0.0.2/wagtailmailchimp/templates/wagtailmailchimp/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-05-25 11:14:49.000000 wagtail-mailchimp-integration-0.0.2/wagtailmailchimp/templates/wagtailmailchimp/widgets/subscriber_optin_widget.html
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-25 11:14:49.000000 wagtail-mailchimp-integration-0.0.2/wagtailmailchimp/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11372 2023-05-25 11:14:49.000000 wagtail-mailchimp-integration-0.0.2/wagtailmailchimp/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-25 11:14:49.000000 wagtail-mailchimp-integration-0.0.2/wagtailmailchimp/wagtail_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-05-25 11:14:49.000000 wagtail-mailchimp-integration-0.0.2/wagtailmailchimp/widgets.py
```

### Comparing `wagtail-mailchimp-integration-0.0.1/LICENSE` & `wagtail-mailchimp-integration-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail-mailchimp-integration-0.0.1/PKG-INFO` & `wagtail-mailchimp-integration-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-mailchimp-integration
-Version: 0.0.1
+Version: 0.0.2
 Summary: Integration of Mailchimp Email Marketing in Wagtail Projects.
 Home-page: https://github.com/wmo-raf/wagtail-mailchimp-integration
 Author: Erick Otenyo
 Author-email: otenyo.erick@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `wagtail-mailchimp-integration-0.0.1/README.md` & `wagtail-mailchimp-integration-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `wagtail-mailchimp-integration-0.0.1/setup.cfg` & `wagtail-mailchimp-integration-0.0.2/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = wagtail-mailchimp-integration
-version = 0.0.1
+version = 0.0.2
 description = Integration of Mailchimp Email Marketing in Wagtail Projects.
 long_description = file:README.md
 long_description_content_type = text/markdown
 url = https://github.com/wmo-raf/wagtail-mailchimp-integration
 author = Erick Otenyo
 author_email = otenyo.erick@gmail.com
 license = MIT
```

### Comparing `wagtail-mailchimp-integration-0.0.1/wagtail_mailchimp_integration.egg-info/PKG-INFO` & `wagtail-mailchimp-integration-0.0.2/wagtail_mailchimp_integration.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-mailchimp-integration
-Version: 0.0.1
+Version: 0.0.2
 Summary: Integration of Mailchimp Email Marketing in Wagtail Projects.
 Home-page: https://github.com/wmo-raf/wagtail-mailchimp-integration
 Author: Erick Otenyo
 Author-email: otenyo.erick@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `wagtail-mailchimp-integration-0.0.1/wagtail_mailchimp_integration.egg-info/SOURCES.txt` & `wagtail-mailchimp-integration-0.0.2/wagtail_mailchimp_integration.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wagtail-mailchimp-integration-0.0.1/wagtailmailchimp/api.py` & `wagtail-mailchimp-integration-0.0.2/wagtailmailchimp/api.py`

 * *Files identical despite different names*

### Comparing `wagtail-mailchimp-integration-0.0.1/wagtailmailchimp/forms.py` & `wagtail-mailchimp-integration-0.0.2/wagtailmailchimp/forms.py`

 * *Files identical despite different names*

### Comparing `wagtail-mailchimp-integration-0.0.1/wagtailmailchimp/migrations/0001_initial.py` & `wagtail-mailchimp-integration-0.0.2/wagtailmailchimp/migrations/0001_initial.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 # Generated by Django 4.2.1 on 2023-05-23 11:42
 
 from django.db import migrations, models
 import django.db.models.deletion
 
 
 class Migration(migrations.Migration):
-
     initial = True
 
-    dependencies = [
-        ('wagtailcore', '0088_userprofile_formsubmission'),
-    ]
+    dependencies = []
 
     operations = [
         migrations.CreateModel(
             name='MailchimpSettings',
             fields=[
                 ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
-                ('api_key', models.CharField(blank=True, help_text='Mailchimp API Key ', max_length=50, null=True, verbose_name='Mailchimp API Key')),
-                ('default_audience_id', models.CharField(blank=True, help_text='Default Mailchimp Audience Id', max_length=100, null=True, verbose_name='Default Mailchimp Audience Id')),
-                ('site', models.OneToOneField(editable=False, on_delete=django.db.models.deletion.CASCADE, to='wagtailcore.site')),
+                ('api_key', models.CharField(blank=True, help_text='Mailchimp API Key ', max_length=50, null=True,
+                                             verbose_name='Mailchimp API Key')),
+                ('default_audience_id',
+                 models.CharField(blank=True, help_text='Default Mailchimp Audience Id', max_length=100, null=True,
+                                  verbose_name='Default Mailchimp Audience Id')),
+                ('site', models.OneToOneField(editable=False, on_delete=django.db.models.deletion.CASCADE,
+                                              to='wagtailcore.site')),
             ],
             options={
                 'abstract': False,
             },
         ),
     ]
```

### Comparing `wagtail-mailchimp-integration-0.0.1/wagtailmailchimp/models.py` & `wagtail-mailchimp-integration-0.0.2/wagtailmailchimp/models.py`

 * *Files identical despite different names*

### Comparing `wagtail-mailchimp-integration-0.0.1/wagtailmailchimp/templates/wagtailmailchimp/mailchimp_integration_form.html` & `wagtail-mailchimp-integration-0.0.2/wagtailmailchimp/templates/wagtailmailchimp/mailchimp_integration_form.html`

 * *Files identical despite different names*

### Comparing `wagtail-mailchimp-integration-0.0.1/wagtailmailchimp/templates/wagtailmailchimp/widgets/subscriber_optin_widget.html` & `wagtail-mailchimp-integration-0.0.2/wagtailmailchimp/templates/wagtailmailchimp/widgets/subscriber_optin_widget.html`

 * *Files identical despite different names*

### Comparing `wagtail-mailchimp-integration-0.0.1/wagtailmailchimp/views.py` & `wagtail-mailchimp-integration-0.0.2/wagtailmailchimp/views.py`

 * *Files identical despite different names*

### Comparing `wagtail-mailchimp-integration-0.0.1/wagtailmailchimp/wagtail_hooks.py` & `wagtail-mailchimp-integration-0.0.2/wagtailmailchimp/wagtail_hooks.py`

 * *Files identical despite different names*

### Comparing `wagtail-mailchimp-integration-0.0.1/wagtailmailchimp/widgets.py` & `wagtail-mailchimp-integration-0.0.2/wagtailmailchimp/widgets.py`

 * *Files identical despite different names*

