# Comparing `tmp/wagtail-mailchimp-integration-0.0.5.tar.gz` & `tmp/wagtail-mailchimp-integration-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail-mailchimp-integration-0.0.5.tar", last modified: Thu May 25 20:13:56 2023, max compression
+gzip compressed data, was "wagtail-mailchimp-integration-0.0.6.tar", last modified: Thu May 25 20:22:33 2023, max compression
```

## Comparing `wagtail-mailchimp-integration-0.0.5.tar` & `wagtail-mailchimp-integration-0.0.6.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:13:56.161316 wagtail-mailchimp-integration-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-25 20:13:34.000000 wagtail-mailchimp-integration-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-25 20:13:34.000000 wagtail-mailchimp-integration-0.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7815 2023-05-25 20:13:56.161316 wagtail-mailchimp-integration-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6886 2023-05-25 20:13:34.000000 wagtail-mailchimp-integration-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-25 20:13:34.000000 wagtail-mailchimp-integration-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-05-25 20:13:56.161316 wagtail-mailchimp-integration-0.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:13:56.161316 wagtail-mailchimp-integration-0.0.5/wagtail_mailchimp_integration.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7815 2023-05-25 20:13:56.000000 wagtail-mailchimp-integration-0.0.5/wagtail_mailchimp_integration.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-05-25 20:13:56.000000 wagtail-mailchimp-integration-0.0.5/wagtail_mailchimp_integration.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 20:13:56.000000 wagtail-mailchimp-integration-0.0.5/wagtail_mailchimp_integration.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-25 20:13:56.000000 wagtail-mailchimp-integration-0.0.5/wagtail_mailchimp_integration.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-25 20:13:56.000000 wagtail-mailchimp-integration-0.0.5/wagtail_mailchimp_integration.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:13:56.161316 wagtail-mailchimp-integration-0.0.5/wagtailmailchimp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 20:13:34.000000 wagtail-mailchimp-integration-0.0.5/wagtailmailchimp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-25 20:13:34.000000 wagtail-mailchimp-integration-0.0.5/wagtailmailchimp/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-05-25 20:13:34.000000 wagtail-mailchimp-integration-0.0.5/wagtailmailchimp/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-25 20:13:34.000000 wagtail-mailchimp-integration-0.0.5/wagtailmailchimp/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)    10374 2023-05-25 20:13:34.000000 wagtail-mailchimp-integration-0.0.5/wagtailmailchimp/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:13:56.161316 wagtail-mailchimp-integration-0.0.5/wagtailmailchimp/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-05-25 20:13:34.000000 wagtail-mailchimp-integration-0.0.5/wagtailmailchimp/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 20:13:34.000000 wagtail-mailchimp-integration-0.0.5/wagtailmailchimp/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12378 2023-05-25 20:13:34.000000 wagtail-mailchimp-integration-0.0.5/wagtailmailchimp/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:13:56.157316 wagtail-mailchimp-integration-0.0.5/wagtailmailchimp/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:13:56.161316 wagtail-mailchimp-integration-0.0.5/wagtailmailchimp/templates/wagtailmailchimp/
--rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-05-25 20:13:34.000000 wagtail-mailchimp-integration-0.0.5/wagtailmailchimp/templates/wagtailmailchimp/mailchimp_integration_form.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:13:56.161316 wagtail-mailchimp-integration-0.0.5/wagtailmailchimp/templates/wagtailmailchimp/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-05-25 20:13:34.000000 wagtail-mailchimp-integration-0.0.5/wagtailmailchimp/templates/wagtailmailchimp/widgets/subscriber_optin_widget.html
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-25 20:13:34.000000 wagtail-mailchimp-integration-0.0.5/wagtailmailchimp/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    11432 2023-05-25 20:13:34.000000 wagtail-mailchimp-integration-0.0.5/wagtailmailchimp/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-25 20:13:34.000000 wagtail-mailchimp-integration-0.0.5/wagtailmailchimp/wagtail_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-05-25 20:13:34.000000 wagtail-mailchimp-integration-0.0.5/wagtailmailchimp/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:22:33.975623 wagtail-mailchimp-integration-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-25 20:22:14.000000 wagtail-mailchimp-integration-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-25 20:22:14.000000 wagtail-mailchimp-integration-0.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7815 2023-05-25 20:22:33.975623 wagtail-mailchimp-integration-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6886 2023-05-25 20:22:14.000000 wagtail-mailchimp-integration-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-25 20:22:14.000000 wagtail-mailchimp-integration-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-05-25 20:22:33.975623 wagtail-mailchimp-integration-0.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:22:33.971623 wagtail-mailchimp-integration-0.0.6/wagtail_mailchimp_integration.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7815 2023-05-25 20:22:33.000000 wagtail-mailchimp-integration-0.0.6/wagtail_mailchimp_integration.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-05-25 20:22:33.000000 wagtail-mailchimp-integration-0.0.6/wagtail_mailchimp_integration.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 20:22:33.000000 wagtail-mailchimp-integration-0.0.6/wagtail_mailchimp_integration.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-25 20:22:33.000000 wagtail-mailchimp-integration-0.0.6/wagtail_mailchimp_integration.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-25 20:22:33.000000 wagtail-mailchimp-integration-0.0.6/wagtail_mailchimp_integration.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:22:33.971623 wagtail-mailchimp-integration-0.0.6/wagtailmailchimp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 20:22:14.000000 wagtail-mailchimp-integration-0.0.6/wagtailmailchimp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-25 20:22:14.000000 wagtail-mailchimp-integration-0.0.6/wagtailmailchimp/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-05-25 20:22:14.000000 wagtail-mailchimp-integration-0.0.6/wagtailmailchimp/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-25 20:22:14.000000 wagtail-mailchimp-integration-0.0.6/wagtailmailchimp/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10374 2023-05-25 20:22:14.000000 wagtail-mailchimp-integration-0.0.6/wagtailmailchimp/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:22:33.975623 wagtail-mailchimp-integration-0.0.6/wagtailmailchimp/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-05-25 20:22:14.000000 wagtail-mailchimp-integration-0.0.6/wagtailmailchimp/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 20:22:14.000000 wagtail-mailchimp-integration-0.0.6/wagtailmailchimp/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12351 2023-05-25 20:22:14.000000 wagtail-mailchimp-integration-0.0.6/wagtailmailchimp/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:22:33.971623 wagtail-mailchimp-integration-0.0.6/wagtailmailchimp/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:22:33.975623 wagtail-mailchimp-integration-0.0.6/wagtailmailchimp/templates/wagtailmailchimp/
+-rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-05-25 20:22:14.000000 wagtail-mailchimp-integration-0.0.6/wagtailmailchimp/templates/wagtailmailchimp/mailchimp_integration_form.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:22:33.975623 wagtail-mailchimp-integration-0.0.6/wagtailmailchimp/templates/wagtailmailchimp/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-05-25 20:22:14.000000 wagtail-mailchimp-integration-0.0.6/wagtailmailchimp/templates/wagtailmailchimp/widgets/subscriber_optin_widget.html
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-25 20:22:14.000000 wagtail-mailchimp-integration-0.0.6/wagtailmailchimp/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11432 2023-05-25 20:22:14.000000 wagtail-mailchimp-integration-0.0.6/wagtailmailchimp/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-25 20:22:14.000000 wagtail-mailchimp-integration-0.0.6/wagtailmailchimp/wagtail_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-05-25 20:22:14.000000 wagtail-mailchimp-integration-0.0.6/wagtailmailchimp/widgets.py
```

### Comparing `wagtail-mailchimp-integration-0.0.5/LICENSE` & `wagtail-mailchimp-integration-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail-mailchimp-integration-0.0.5/PKG-INFO` & `wagtail-mailchimp-integration-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-mailchimp-integration
-Version: 0.0.5
+Version: 0.0.6
 Summary: Integration of Mailchimp Email Marketing in Wagtail Projects.
 Home-page: https://github.com/wmo-raf/wagtail-mailchimp-integration
 Author: Erick Otenyo
 Author-email: otenyo.erick@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `wagtail-mailchimp-integration-0.0.5/README.md` & `wagtail-mailchimp-integration-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `wagtail-mailchimp-integration-0.0.5/setup.cfg` & `wagtail-mailchimp-integration-0.0.6/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = wagtail-mailchimp-integration
-version = 0.0.5
+version = 0.0.6
 description = Integration of Mailchimp Email Marketing in Wagtail Projects.
 long_description = file:README.md
 long_description_content_type = text/markdown
 url = https://github.com/wmo-raf/wagtail-mailchimp-integration
 author = Erick Otenyo
 author_email = otenyo.erick@gmail.com
 license = MIT
```

### Comparing `wagtail-mailchimp-integration-0.0.5/wagtail_mailchimp_integration.egg-info/PKG-INFO` & `wagtail-mailchimp-integration-0.0.6/wagtail_mailchimp_integration.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-mailchimp-integration
-Version: 0.0.5
+Version: 0.0.6
 Summary: Integration of Mailchimp Email Marketing in Wagtail Projects.
 Home-page: https://github.com/wmo-raf/wagtail-mailchimp-integration
 Author: Erick Otenyo
 Author-email: otenyo.erick@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `wagtail-mailchimp-integration-0.0.5/wagtail_mailchimp_integration.egg-info/SOURCES.txt` & `wagtail-mailchimp-integration-0.0.6/wagtail_mailchimp_integration.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wagtail-mailchimp-integration-0.0.5/wagtailmailchimp/api.py` & `wagtail-mailchimp-integration-0.0.6/wagtailmailchimp/api.py`

 * *Files identical despite different names*

### Comparing `wagtail-mailchimp-integration-0.0.5/wagtailmailchimp/forms.py` & `wagtail-mailchimp-integration-0.0.6/wagtailmailchimp/forms.py`

 * *Files identical despite different names*

### Comparing `wagtail-mailchimp-integration-0.0.5/wagtailmailchimp/migrations/0001_initial.py` & `wagtail-mailchimp-integration-0.0.6/wagtailmailchimp/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail-mailchimp-integration-0.0.5/wagtailmailchimp/models.py` & `wagtail-mailchimp-integration-0.0.6/wagtailmailchimp/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from wagtail.contrib.settings.models import BaseSiteSetting
 from wagtail.contrib.settings.registry import register_setting
 
 from .api import MailchimpApi
 from .widgets import MailchimpSubscriberOptinWidget, MailchimpAudienceListWidget
 
 
-@register_setting(icon="cogs")
+@register_setting
 class MailchimpSettings(BaseSiteSetting):
     api_key = models.CharField(verbose_name=_("Mailchimp API Key"), max_length=50, blank=True, null=True,
                                help_text=_("Mailchimp API Key "))
     default_audience_id = models.CharField(verbose_name=_("Default Mailchimp Audience Id"), max_length=100, blank=True,
                                            null=True,
                                            help_text=_("Default Mailchimp Audience Id"))
 
@@ -82,15 +82,15 @@
             ], classname='label-above'),
             FieldPanel('success_redirect_page')
         ], (_('MailChimp Settings'))),
         FieldPanel('thank_you_text')
     ]
 
 
-class AbstractMailchimpIntegrationForm(AbstractForm, models.Model):
+class AbstractMailchimpIntegrationForm(AbstractForm):
     class Meta:
         abstract = True
 
     mailchimp_field_name = 'mailchimp_subscribe_check'
     mailchimp_interests_field_name = 'mailchimp_interests_check'
     default_mailing_list_checkbox_label = _("Join Our Mailing List")
```

### Comparing `wagtail-mailchimp-integration-0.0.5/wagtailmailchimp/templates/wagtailmailchimp/mailchimp_integration_form.html` & `wagtail-mailchimp-integration-0.0.6/wagtailmailchimp/templates/wagtailmailchimp/mailchimp_integration_form.html`

 * *Files identical despite different names*

### Comparing `wagtail-mailchimp-integration-0.0.5/wagtailmailchimp/templates/wagtailmailchimp/widgets/subscriber_optin_widget.html` & `wagtail-mailchimp-integration-0.0.6/wagtailmailchimp/templates/wagtailmailchimp/widgets/subscriber_optin_widget.html`

 * *Files identical despite different names*

### Comparing `wagtail-mailchimp-integration-0.0.5/wagtailmailchimp/views.py` & `wagtail-mailchimp-integration-0.0.6/wagtailmailchimp/views.py`

 * *Files identical despite different names*

### Comparing `wagtail-mailchimp-integration-0.0.5/wagtailmailchimp/wagtail_hooks.py` & `wagtail-mailchimp-integration-0.0.6/wagtailmailchimp/wagtail_hooks.py`

 * *Files identical despite different names*

### Comparing `wagtail-mailchimp-integration-0.0.5/wagtailmailchimp/widgets.py` & `wagtail-mailchimp-integration-0.0.6/wagtailmailchimp/widgets.py`

 * *Files identical despite different names*

