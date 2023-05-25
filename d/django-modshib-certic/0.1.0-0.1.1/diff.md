# Comparing `tmp/django-modshib-CERTIC-0.1.0.tar.gz` & `tmp/django-modshib-CERTIC-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-modshib-CERTIC-0.1.0.tar", max compression
+gzip compressed data, was "django-modshib-CERTIC-0.1.1.tar", max compression
```

## Comparing `django-modshib-CERTIC-0.1.0.tar` & `django-modshib-CERTIC-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0        0 2023-05-19 06:10:59.653227 django-modshib-CERTIC-0.1.0/modshib/__init__.py
--rw-r--r--   0        0        0       63 2023-05-19 06:10:59.654166 django-modshib-CERTIC-0.1.0/modshib/admin.py
--rw-r--r--   0        0        0      146 2023-05-24 09:58:37.360521 django-modshib-CERTIC-0.1.0/modshib/apps.py
--rw-r--r--   0        0        0        0 2023-05-19 06:10:59.656283 django-modshib-CERTIC-0.1.0/modshib/migrations/__init__.py
--rw-r--r--   0        0        0       57 2023-05-19 06:10:59.655746 django-modshib-CERTIC-0.1.0/modshib/models.py
--rw-r--r--   0        0        0      747 2023-05-22 09:55:06.204141 django-modshib-CERTIC-0.1.0/modshib/templates/registration/logged_out.html
--rw-r--r--   0        0        0     1315 2023-05-24 08:51:31.235141 django-modshib-CERTIC-0.1.0/modshib/templates/registration/login.html
--rw-r--r--   0        0        0      838 2023-05-19 07:02:49.960081 django-modshib-CERTIC-0.1.0/modshib/templates/registration/reg_base.html
--rw-r--r--   0        0        0      794 2023-05-24 08:22:05.742051 django-modshib-CERTIC-0.1.0/modshib/templates/registration/sso_fail.html
--rw-r--r--   0        0        0      813 2023-05-24 09:54:48.646844 django-modshib-CERTIC-0.1.0/modshib/templates/registration/sso_no_account.html
--rw-r--r--   0        0        0       60 2023-05-19 06:10:59.655994 django-modshib-CERTIC-0.1.0/modshib/tests.py
--rw-r--r--   0        0        0      117 2023-05-22 09:06:53.828987 django-modshib-CERTIC-0.1.0/modshib/urls.py
--rw-r--r--   0        0        0     2035 2023-05-24 10:11:19.574418 django-modshib-CERTIC-0.1.0/modshib/views.py
--rw-r--r--   0        0        0      550 2023-05-23 16:32:16.102096 django-modshib-CERTIC-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      729 2023-05-24 11:55:41.091976 django-modshib-CERTIC-0.1.0/setup.py
--rw-r--r--   0        0        0      657 2023-05-24 11:55:41.092222 django-modshib-CERTIC-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-19 06:10:59.653227 django-modshib-CERTIC-0.1.1/modshib/__init__.py
+-rw-r--r--   0        0        0       63 2023-05-19 06:10:59.654166 django-modshib-CERTIC-0.1.1/modshib/admin.py
+-rw-r--r--   0        0        0      146 2023-05-24 09:58:37.360521 django-modshib-CERTIC-0.1.1/modshib/apps.py
+-rw-r--r--   0        0        0        0 2023-05-19 06:10:59.656283 django-modshib-CERTIC-0.1.1/modshib/migrations/__init__.py
+-rw-r--r--   0        0        0       57 2023-05-19 06:10:59.655746 django-modshib-CERTIC-0.1.1/modshib/models.py
+-rw-r--r--   0        0        0      747 2023-05-22 09:55:06.204141 django-modshib-CERTIC-0.1.1/modshib/templates/registration/logged_out.html
+-rw-r--r--   0        0        0     1315 2023-05-24 08:51:31.235141 django-modshib-CERTIC-0.1.1/modshib/templates/registration/login.html
+-rw-r--r--   0        0        0      838 2023-05-19 07:02:49.960081 django-modshib-CERTIC-0.1.1/modshib/templates/registration/reg_base.html
+-rw-r--r--   0        0        0      794 2023-05-24 08:22:05.742051 django-modshib-CERTIC-0.1.1/modshib/templates/registration/sso_fail.html
+-rw-r--r--   0        0        0      813 2023-05-24 09:54:48.646844 django-modshib-CERTIC-0.1.1/modshib/templates/registration/sso_no_account.html
+-rw-r--r--   0        0        0       60 2023-05-19 06:10:59.655994 django-modshib-CERTIC-0.1.1/modshib/tests.py
+-rw-r--r--   0        0        0      117 2023-05-22 09:06:53.828987 django-modshib-CERTIC-0.1.1/modshib/urls.py
+-rw-r--r--   0        0        0     2706 2023-05-25 20:13:39.942458 django-modshib-CERTIC-0.1.1/modshib/views.py
+-rw-r--r--   0        0        0      551 2023-05-25 20:11:35.911724 django-modshib-CERTIC-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      722 2023-05-25 20:56:12.103703 django-modshib-CERTIC-0.1.1/setup.py
+-rw-r--r--   0        0        0      700 2023-05-25 20:56:12.103973 django-modshib-CERTIC-0.1.1/PKG-INFO
```

### Comparing `django-modshib-CERTIC-0.1.0/modshib/templates/registration/logged_out.html` & `django-modshib-CERTIC-0.1.1/modshib/templates/registration/logged_out.html`

 * *Files identical despite different names*

### Comparing `django-modshib-CERTIC-0.1.0/modshib/templates/registration/login.html` & `django-modshib-CERTIC-0.1.1/modshib/templates/registration/login.html`

 * *Files identical despite different names*

### Comparing `django-modshib-CERTIC-0.1.0/modshib/templates/registration/reg_base.html` & `django-modshib-CERTIC-0.1.1/modshib/templates/registration/reg_base.html`

 * *Files identical despite different names*

### Comparing `django-modshib-CERTIC-0.1.0/modshib/templates/registration/sso_fail.html` & `django-modshib-CERTIC-0.1.1/modshib/templates/registration/sso_fail.html`

 * *Files identical despite different names*

### Comparing `django-modshib-CERTIC-0.1.0/modshib/templates/registration/sso_no_account.html` & `django-modshib-CERTIC-0.1.1/modshib/templates/registration/sso_no_account.html`

 * *Files identical despite different names*

### Comparing `django-modshib-CERTIC-0.1.0/modshib/views.py` & `django-modshib-CERTIC-0.1.1/modshib/views.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from django.conf import settings
 from django.http import HttpRequest, HttpResponse, HttpResponseRedirect
 from django.contrib.auth import login
-from django.contrib.auth.models import User
+from django.contrib.auth.models import User, Group
 from django.shortcuts import render
 from logging import Logger, INFO
 
 logger = Logger(name=__name__, level=INFO)
 
+
 try:
     CREATE_ACCOUNT = bool(settings.MODSHIB_CREATE_ACCOUNT)
 except AttributeError:
     CREATE_ACCOUNT = False
 
 try:
     ACTIVATE_ACCOUNT = bool(settings.MODSHIB_ACTIVATE_ACCOUNT)
@@ -24,29 +25,45 @@
         logger.info(
             f"User already authenticated, redirecting to {settings.LOGIN_REDIRECT_URL}"
         )
         return HttpResponseRedirect(settings.LOGIN_REDIRECT_URL)
 
     # fetch EPPN from headers, injected by mod_shib
     eppn = request.META.get("HTTP_EPPN", None)
+    supann_etablissement = request.META.get("HTTP_SUPANNETABLISSEMENT", None)
+    # display_name = request.META.get("HTTP_DISPLAYNAME", None)
+    mail = request.META.get("HTTP_MAIL", None)
+    last_name = request.META.get("HTTP_SN", None)
+    first_name = request.META.get("HTTP_GIVENNAME", None)
     if not eppn:
         return render(
             request,
             "registration/sso_fail.html",
             {"login_redirect": settings.LOGIN_URL},
         )
 
     # find account
     eppn = eppn.strip()
     user = User.objects.filter(username=eppn).first()
     if not user and CREATE_ACCOUNT:
         logger.info(f"user {eppn} not found, creating account")
         user = User.objects.create_user(eppn)
         user.is_active = False
+        if mail:
+            user.email = mail
+        if last_name:
+            user.last_name = last_name
+        if first_name:
+            user.first_name = first_name
         user.save()
+        if supann_etablissement:
+            group, created = Group.objects.get_or_create(
+                name=f"supann_{supann_etablissement}"
+            )
+            user.groups.add(group)
     if not user:
         logger.info(f"user {eppn} not found, rejecting auth")
         return render(request, "registration/sso_no_account.html")
     if not user.is_active and ACTIVATE_ACCOUNT:
         logger.info(f"user {eppn} not active, activating")
         user.is_active = True
         user.save()
```

### Comparing `django-modshib-CERTIC-0.1.0/pyproject.toml` & `django-modshib-CERTIC-0.1.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "django-modshib-CERTIC"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = ["Mickaël Desfrênes <mickael.desfrenes@unicaen.fr>"]
 license = "Cecill-B"
 packages = [
     { include = "modshib"},
 ]
 homepage = "https://www.certic.unicaen.fr"
 repository = "https://git.unicaen.fr/certic/django-modshib"
 
 [tool.poetry.dependencies]
-python = ">=3.8"
+python = ">=3.7"
 Django = ">=4.0"
-django-auth-cli-certic = "^0.1.3"
+django-auth-cli-certic = ">=0.1.3"
 
 [tool.poetry.dev-dependencies]
 black = "^23.3.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `django-modshib-CERTIC-0.1.0/setup.py` & `django-modshib-CERTIC-0.1.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,27 +4,27 @@
 packages = \
 ['modshib', 'modshib.migrations']
 
 package_data = \
 {'': ['*'], 'modshib': ['templates/registration/*']}
 
 install_requires = \
-['Django>=4.0', 'django-auth-cli-certic>=0.1.3,<0.2.0']
+['Django>=4.0', 'django-auth-cli-certic>=0.1.3']
 
 setup_kwargs = {
     'name': 'django-modshib-certic',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': '',
     'long_description': None,
     'author': 'Mickaël Desfrênes',
     'author_email': 'mickael.desfrenes@unicaen.fr',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://www.certic.unicaen.fr',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.8',
+    'python_requires': '>=3.7',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `django-modshib-CERTIC-0.1.0/PKG-INFO` & `django-modshib-CERTIC-0.1.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: django-modshib-certic
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Home-page: https://www.certic.unicaen.fr
 License: CECILL-B
 Author: Mickaël Desfrênes
 Author-email: mickael.desfrenes@unicaen.fr
-Requires-Python: >=3.8
+Requires-Python: >=3.7
 Classifier: License :: CeCILL-B Free Software License Agreement (CECILL-B)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: Django (>=4.0)
-Requires-Dist: django-auth-cli-certic (>=0.1.3,<0.2.0)
+Requires-Dist: django-auth-cli-certic (>=0.1.3)
 Project-URL: Repository, https://git.unicaen.fr/certic/django-modshib
```

