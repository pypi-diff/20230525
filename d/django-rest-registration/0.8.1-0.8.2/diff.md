# Comparing `tmp/django-rest-registration-0.8.1.tar.gz` & `tmp/django-rest-registration-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-rest-registration-0.8.1.tar", last modified: Thu May  4 10:00:56 2023, max compression
+gzip compressed data, was "django-rest-registration-0.8.2.tar", last modified: Thu May 25 21:02:36 2023, max compression
```

## Comparing `django-rest-registration-0.8.1.tar` & `django-rest-registration-0.8.2.tar`

### file list

```diff
@@ -1,104 +1,108 @@
-drwxr-xr-x   0 andrzejpragacz   (502) staff       (20)        0 2023-05-04 10:00:56.632416 django-rest-registration-0.8.1/
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)     1088 2022-09-21 08:03:05.000000 django-rest-registration-0.8.1/LICENSE
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)      173 2023-05-04 09:44:58.000000 django-rest-registration-0.8.1/MANIFEST.in
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)     5936 2023-05-04 10:00:56.632730 django-rest-registration-0.8.1/PKG-INFO
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)     4560 2022-09-21 08:03:05.000000 django-rest-registration-0.8.1/README.md
-drwxr-xr-x   0 andrzejpragacz   (502) staff       (20)        0 2023-05-04 10:00:56.560482 django-rest-registration-0.8.1/django_rest_registration.egg-info/
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)     5936 2023-05-04 10:00:56.000000 django-rest-registration-0.8.1/django_rest_registration.egg-info/PKG-INFO
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)     3321 2023-05-04 10:00:56.000000 django-rest-registration-0.8.1/django_rest_registration.egg-info/SOURCES.txt
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)        1 2023-05-04 10:00:56.000000 django-rest-registration-0.8.1/django_rest_registration.egg-info/dependency_links.txt
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)       37 2023-05-04 10:00:56.000000 django-rest-registration-0.8.1/django_rest_registration.egg-info/requires.txt
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)       18 2023-05-04 10:00:56.000000 django-rest-registration-0.8.1/django_rest_registration.egg-info/top_level.txt
-drwxr-xr-x   0 andrzejpragacz   (502) staff       (20)        0 2023-05-04 10:00:56.577063 django-rest-registration-0.8.1/rest_registration/
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)      135 2023-03-30 09:35:45.000000 django-rest-registration-0.8.1/rest_registration/__init__.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)       22 2023-05-04 10:00:34.000000 django-rest-registration-0.8.1/rest_registration/_version.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)        0 2019-06-21 10:41:29.000000 django-rest-registration-0.8.1/rest_registration/admin.py
-drwxr-xr-x   0 andrzejpragacz   (502) staff       (20)        0 2023-05-04 10:00:56.580275 django-rest-registration-0.8.1/rest_registration/api/
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)        0 2019-06-21 10:41:29.000000 django-rest-registration-0.8.1/rest_registration/api/__init__.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)     4738 2022-09-21 08:03:05.000000 django-rest-registration-0.8.1/rest_registration/api/serializers.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)      946 2022-09-21 08:03:05.000000 django-rest-registration-0.8.1/rest_registration/api/urls.py
-drwxr-xr-x   0 andrzejpragacz   (502) staff       (20)        0 2023-05-04 10:00:56.588471 django-rest-registration-0.8.1/rest_registration/api/views/
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)      333 2019-06-21 10:41:29.000000 django-rest-registration-0.8.1/rest_registration/api/views/__init__.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)     1498 2022-10-04 22:18:47.000000 django-rest-registration-0.8.1/rest_registration/api/views/base.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)     2099 2022-10-04 22:18:47.000000 django-rest-registration-0.8.1/rest_registration/api/views/change_password.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)     4012 2022-10-04 22:18:47.000000 django-rest-registration-0.8.1/rest_registration/api/views/login.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)     1369 2022-10-04 22:18:47.000000 django-rest-registration-0.8.1/rest_registration/api/views/profile.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)     4685 2023-04-27 22:36:54.000000 django-rest-registration-0.8.1/rest_registration/api/views/register.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)     4519 2023-03-29 17:45:06.000000 django-rest-registration-0.8.1/rest_registration/api/views/register_email.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)     4510 2022-10-04 22:18:47.000000 django-rest-registration-0.8.1/rest_registration/api/views/reset_password.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)      149 2019-08-01 20:03:57.000000 django-rest-registration-0.8.1/rest_registration/apps.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)     3054 2023-04-28 08:37:06.000000 django-rest-registration-0.8.1/rest_registration/auth_token_managers.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)    12298 2023-03-29 17:45:06.000000 django-rest-registration-0.8.1/rest_registration/checks.py
-drwxr-xr-x   0 andrzejpragacz   (502) staff       (20)        0 2023-05-04 10:00:56.589345 django-rest-registration-0.8.1/rest_registration/contrib/
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)        0 2022-09-21 08:03:05.000000 django-rest-registration-0.8.1/rest_registration/contrib/__init__.py
-drwxr-xr-x   0 andrzejpragacz   (502) staff       (20)        0 2023-05-04 10:00:56.596274 django-rest-registration-0.8.1/rest_registration/contrib/verification_redirects/
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)        0 2019-06-21 10:41:29.000000 django-rest-registration-0.8.1/rest_registration/contrib/verification_redirects/__init__.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)        0 2019-06-21 10:41:29.000000 django-rest-registration-0.8.1/rest_registration/contrib/verification_redirects/admin.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)      225 2019-06-21 10:41:29.000000 django-rest-registration-0.8.1/rest_registration/contrib/verification_redirects/apps.py
-drwxr-xr-x   0 andrzejpragacz   (502) staff       (20)        0 2023-05-04 10:00:56.597141 django-rest-registration-0.8.1/rest_registration/contrib/verification_redirects/migrations/
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)        0 2019-06-21 10:41:29.000000 django-rest-registration-0.8.1/rest_registration/contrib/verification_redirects/migrations/__init__.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)        0 2019-06-21 10:41:29.000000 django-rest-registration-0.8.1/rest_registration/contrib/verification_redirects/models.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)      834 2023-03-29 17:45:06.000000 django-rest-registration-0.8.1/rest_registration/contrib/verification_redirects/settings.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)      393 2022-09-21 08:03:05.000000 django-rest-registration-0.8.1/rest_registration/contrib/verification_redirects/urls.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)     1975 2022-09-21 08:03:05.000000 django-rest-registration-0.8.1/rest_registration/contrib/verification_redirects/views.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)     1593 2022-09-21 08:03:05.000000 django-rest-registration-0.8.1/rest_registration/enums.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)     3010 2023-03-29 17:45:06.000000 django-rest-registration-0.8.1/rest_registration/exceptions.py
-drwxr-xr-x   0 andrzejpragacz   (502) staff       (20)        0 2023-05-04 10:00:56.542505 django-rest-registration-0.8.1/rest_registration/locale/
-drwxr-xr-x   0 andrzejpragacz   (502) staff       (20)        0 2023-05-04 10:00:56.541282 django-rest-registration-0.8.1/rest_registration/locale/fr/
-drwxr-xr-x   0 andrzejpragacz   (502) staff       (20)        0 2023-05-04 10:00:56.598172 django-rest-registration-0.8.1/rest_registration/locale/fr/LC_MESSAGES/
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)     2537 2022-12-08 11:12:05.000000 django-rest-registration-0.8.1/rest_registration/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 andrzejpragacz   (502) staff       (20)        0 2023-05-04 10:00:56.542094 django-rest-registration-0.8.1/rest_registration/locale/id/
-drwxr-xr-x   0 andrzejpragacz   (502) staff       (20)        0 2023-05-04 10:00:56.598971 django-rest-registration-0.8.1/rest_registration/locale/id/LC_MESSAGES/
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)     3159 2023-03-29 17:45:06.000000 django-rest-registration-0.8.1/rest_registration/locale/id/LC_MESSAGES/django.po
-drwxr-xr-x   0 andrzejpragacz   (502) staff       (20)        0 2023-05-04 10:00:56.542909 django-rest-registration-0.8.1/rest_registration/locale/pt_BR/
-drwxr-xr-x   0 andrzejpragacz   (502) staff       (20)        0 2023-05-04 10:00:56.599645 django-rest-registration-0.8.1/rest_registration/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)     2304 2022-09-21 08:03:05.000000 django-rest-registration-0.8.1/rest_registration/locale/pt_BR/LC_MESSAGES/django.po
-drwxr-xr-x   0 andrzejpragacz   (502) staff       (20)        0 2023-05-04 10:00:56.600594 django-rest-registration-0.8.1/rest_registration/migrations/
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)        0 2019-06-21 10:41:29.000000 django-rest-registration-0.8.1/rest_registration/migrations/__init__.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)        0 2019-06-21 10:41:29.000000 django-rest-registration-0.8.1/rest_registration/models.py
-drwxr-xr-x   0 andrzejpragacz   (502) staff       (20)        0 2023-05-04 10:00:56.602492 django-rest-registration-0.8.1/rest_registration/notifications/
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)      133 2019-06-21 10:41:29.000000 django-rest-registration-0.8.1/rest_registration/notifications/__init__.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)     2426 2022-09-21 08:03:05.000000 django-rest-registration-0.8.1/rest_registration/notifications/email.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)      204 2019-10-08 08:40:56.000000 django-rest-registration-0.8.1/rest_registration/notifications/enums.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)      678 2023-03-29 17:45:06.000000 django-rest-registration-0.8.1/rest_registration/settings.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)    21417 2022-09-21 08:03:05.000000 django-rest-registration-0.8.1/rest_registration/settings_fields.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)      316 2022-09-21 08:03:05.000000 django-rest-registration-0.8.1/rest_registration/signals.py
-drwxr-xr-x   0 andrzejpragacz   (502) staff       (20)        0 2023-05-04 10:00:56.605583 django-rest-registration-0.8.1/rest_registration/signers/
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)        0 2022-09-21 08:03:05.000000 django-rest-registration-0.8.1/rest_registration/signers/__init__.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)     1405 2022-09-21 08:03:05.000000 django-rest-registration-0.8.1/rest_registration/signers/register.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)      428 2022-09-21 08:03:05.000000 django-rest-registration-0.8.1/rest_registration/signers/register_email.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)     1293 2022-09-21 08:03:05.000000 django-rest-registration-0.8.1/rest_registration/signers/reset_password.py
-drwxr-xr-x   0 andrzejpragacz   (502) staff       (20)        0 2023-05-04 10:00:56.545236 django-rest-registration-0.8.1/rest_registration/templates/
-drwxr-xr-x   0 andrzejpragacz   (502) staff       (20)        0 2023-05-04 10:00:56.546743 django-rest-registration-0.8.1/rest_registration/templates/rest_registration/
-drwxr-xr-x   0 andrzejpragacz   (502) staff       (20)        0 2023-05-04 10:00:56.608298 django-rest-registration-0.8.1/rest_registration/templates/rest_registration/register/
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)      255 2019-10-08 08:40:56.000000 django-rest-registration-0.8.1/rest_registration/templates/rest_registration/register/body.html
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)       84 2019-06-21 10:41:29.000000 django-rest-registration-0.8.1/rest_registration/templates/rest_registration/register/body.txt
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)       27 2019-06-21 10:41:29.000000 django-rest-registration-0.8.1/rest_registration/templates/rest_registration/register/subject.txt
-drwxr-xr-x   0 andrzejpragacz   (502) staff       (20)        0 2023-05-04 10:00:56.610847 django-rest-registration-0.8.1/rest_registration/templates/rest_registration/register_email/
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)      689 2019-10-08 08:40:56.000000 django-rest-registration-0.8.1/rest_registration/templates/rest_registration/register_email/body.html
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)      380 2019-10-08 08:40:56.000000 django-rest-registration-0.8.1/rest_registration/templates/rest_registration/register_email/body.txt
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)      102 2019-10-08 08:40:56.000000 django-rest-registration-0.8.1/rest_registration/templates/rest_registration/register_email/subject.txt
-drwxr-xr-x   0 andrzejpragacz   (502) staff       (20)        0 2023-05-04 10:00:56.613991 django-rest-registration-0.8.1/rest_registration/templates/rest_registration/reset_password/
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)      258 2019-10-08 08:40:56.000000 django-rest-registration-0.8.1/rest_registration/templates/rest_registration/reset_password/body.html
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)       85 2019-06-21 10:41:29.000000 django-rest-registration-0.8.1/rest_registration/templates/rest_registration/reset_password/body.txt
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)       29 2019-06-21 10:41:29.000000 django-rest-registration-0.8.1/rest_registration/templates/rest_registration/reset_password/subject.txt
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)        0 2019-06-21 10:41:29.000000 django-rest-registration-0.8.1/rest_registration/tests.py
-drwxr-xr-x   0 andrzejpragacz   (502) staff       (20)        0 2023-05-04 10:00:56.630781 django-rest-registration-0.8.1/rest_registration/utils/
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)        0 2019-06-21 10:41:29.000000 django-rest-registration-0.8.1/rest_registration/utils/__init__.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)     1038 2022-09-21 08:03:05.000000 django-rest-registration-0.8.1/rest_registration/utils/auth_backends.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)     2996 2023-03-29 17:45:06.000000 django-rest-registration-0.8.1/rest_registration/utils/checks.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)     1581 2022-09-21 08:03:05.000000 django-rest-registration-0.8.1/rest_registration/utils/common.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)     6751 2022-09-21 08:03:05.000000 django-rest-registration-0.8.1/rest_registration/utils/email.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)      955 2022-09-21 08:03:05.000000 django-rest-registration-0.8.1/rest_registration/utils/functools.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)     2706 2022-09-21 08:03:05.000000 django-rest-registration-0.8.1/rest_registration/utils/html.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)     1997 2022-09-21 08:03:05.000000 django-rest-registration-0.8.1/rest_registration/utils/nested_settings.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)      734 2022-09-21 08:03:05.000000 django-rest-registration-0.8.1/rest_registration/utils/responses.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)     3162 2023-03-29 17:45:06.000000 django-rest-registration-0.8.1/rest_registration/utils/signers.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)      600 2023-03-29 17:45:06.000000 django-rest-registration-0.8.1/rest_registration/utils/types.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)    11638 2023-03-29 17:45:06.000000 django-rest-registration-0.8.1/rest_registration/utils/users.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)     4364 2023-03-29 17:45:06.000000 django-rest-registration-0.8.1/rest_registration/utils/validation.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)     3731 2023-03-29 17:45:06.000000 django-rest-registration-0.8.1/rest_registration/utils/verification.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)     3520 2022-09-21 08:03:05.000000 django-rest-registration-0.8.1/rest_registration/verification_notifications.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)        0 2019-06-21 10:41:29.000000 django-rest-registration-0.8.1/rest_registration/views.py
--rw-r--r--   0 andrzejpragacz   (502) staff       (20)     3145 2023-05-04 10:00:56.634470 django-rest-registration-0.8.1/setup.cfg
--rwxr-xr-x   0 andrzejpragacz   (502) staff       (20)      176 2023-04-27 22:36:38.000000 django-rest-registration-0.8.1/setup.py
+drwxr-xr-x   0 andrzej    (503) staff       (20)        0 2023-05-25 21:02:36.639087 django-rest-registration-0.8.2/
+-rw-r--r--   0 andrzej    (503) staff       (20)     1088 2023-05-25 20:52:54.000000 django-rest-registration-0.8.2/LICENSE
+-rw-r--r--   0 andrzej    (503) staff       (20)      173 2023-05-04 20:06:39.000000 django-rest-registration-0.8.2/MANIFEST.in
+-rw-r--r--   0 andrzej    (503) staff       (20)     7150 2023-05-25 21:02:36.636000 django-rest-registration-0.8.2/PKG-INFO
+-rw-r--r--   0 andrzej    (503) staff       (20)     4560 2021-12-24 09:22:04.000000 django-rest-registration-0.8.2/README.md
+drwxr-xr-x   0 andrzej    (503) staff       (20)        0 2023-05-25 21:02:36.497877 django-rest-registration-0.8.2/django_rest_registration.egg-info/
+-rw-r--r--   0 andrzej    (503) staff       (20)     7150 2023-05-25 21:02:36.000000 django-rest-registration-0.8.2/django_rest_registration.egg-info/PKG-INFO
+-rw-r--r--   0 andrzej    (503) staff       (20)     3376 2023-05-25 21:02:36.000000 django-rest-registration-0.8.2/django_rest_registration.egg-info/SOURCES.txt
+-rw-r--r--   0 andrzej    (503) staff       (20)        1 2023-05-25 21:02:36.000000 django-rest-registration-0.8.2/django_rest_registration.egg-info/dependency_links.txt
+-rw-r--r--   0 andrzej    (503) staff       (20)       37 2023-05-25 21:02:36.000000 django-rest-registration-0.8.2/django_rest_registration.egg-info/requires.txt
+-rw-r--r--   0 andrzej    (503) staff       (20)       18 2023-05-25 21:02:36.000000 django-rest-registration-0.8.2/django_rest_registration.egg-info/top_level.txt
+-rw-r--r--   0 andrzej    (503) staff       (20)     3412 2023-05-08 21:35:32.000000 django-rest-registration-0.8.2/pyproject.toml
+drwxr-xr-x   0 andrzej    (503) staff       (20)        0 2023-05-25 21:02:36.525082 django-rest-registration-0.8.2/rest_registration/
+-rw-r--r--   0 andrzej    (503) staff       (20)      135 2023-04-01 20:11:42.000000 django-rest-registration-0.8.2/rest_registration/__init__.py
+-rw-r--r--   0 andrzej    (503) staff       (20)       22 2023-05-25 21:01:47.000000 django-rest-registration-0.8.2/rest_registration/_version.py
+-rw-r--r--   0 andrzej    (503) staff       (20)        0 2021-10-12 00:14:12.000000 django-rest-registration-0.8.2/rest_registration/admin.py
+drwxr-xr-x   0 andrzej    (503) staff       (20)        0 2023-05-25 21:02:36.530737 django-rest-registration-0.8.2/rest_registration/api/
+-rw-r--r--   0 andrzej    (503) staff       (20)        0 2021-10-12 00:14:12.000000 django-rest-registration-0.8.2/rest_registration/api/__init__.py
+-rw-r--r--   0 andrzej    (503) staff       (20)     4738 2021-10-12 00:14:12.000000 django-rest-registration-0.8.2/rest_registration/api/serializers.py
+-rw-r--r--   0 andrzej    (503) staff       (20)      946 2021-12-24 09:22:04.000000 django-rest-registration-0.8.2/rest_registration/api/urls.py
+drwxr-xr-x   0 andrzej    (503) staff       (20)        0 2023-05-25 21:02:36.540664 django-rest-registration-0.8.2/rest_registration/api/views/
+-rw-r--r--   0 andrzej    (503) staff       (20)      333 2021-10-12 00:14:12.000000 django-rest-registration-0.8.2/rest_registration/api/views/__init__.py
+-rw-r--r--   0 andrzej    (503) staff       (20)     1498 2022-10-02 23:02:43.000000 django-rest-registration-0.8.2/rest_registration/api/views/base.py
+-rw-r--r--   0 andrzej    (503) staff       (20)     2099 2022-10-02 23:02:43.000000 django-rest-registration-0.8.2/rest_registration/api/views/change_password.py
+-rw-r--r--   0 andrzej    (503) staff       (20)     4012 2022-10-02 23:02:43.000000 django-rest-registration-0.8.2/rest_registration/api/views/login.py
+-rw-r--r--   0 andrzej    (503) staff       (20)     1369 2022-10-02 23:02:43.000000 django-rest-registration-0.8.2/rest_registration/api/views/profile.py
+-rw-r--r--   0 andrzej    (503) staff       (20)     4685 2023-05-05 22:14:18.000000 django-rest-registration-0.8.2/rest_registration/api/views/register.py
+-rw-r--r--   0 andrzej    (503) staff       (20)     4519 2023-04-01 20:11:42.000000 django-rest-registration-0.8.2/rest_registration/api/views/register_email.py
+-rw-r--r--   0 andrzej    (503) staff       (20)     4510 2022-10-02 23:02:43.000000 django-rest-registration-0.8.2/rest_registration/api/views/reset_password.py
+-rw-r--r--   0 andrzej    (503) staff       (20)      149 2021-10-12 00:14:12.000000 django-rest-registration-0.8.2/rest_registration/apps.py
+-rw-r--r--   0 andrzej    (503) staff       (20)     3082 2023-05-08 21:35:32.000000 django-rest-registration-0.8.2/rest_registration/auth_token_managers.py
+-rw-r--r--   0 andrzej    (503) staff       (20)    12042 2023-05-08 21:35:32.000000 django-rest-registration-0.8.2/rest_registration/checks.py
+drwxr-xr-x   0 andrzej    (503) staff       (20)        0 2023-05-25 21:02:36.541542 django-rest-registration-0.8.2/rest_registration/contrib/
+-rw-r--r--   0 andrzej    (503) staff       (20)        0 2021-10-12 00:14:12.000000 django-rest-registration-0.8.2/rest_registration/contrib/__init__.py
+drwxr-xr-x   0 andrzej    (503) staff       (20)        0 2023-05-25 21:02:36.550380 django-rest-registration-0.8.2/rest_registration/contrib/verification_redirects/
+-rw-r--r--   0 andrzej    (503) staff       (20)        0 2021-10-12 00:14:12.000000 django-rest-registration-0.8.2/rest_registration/contrib/verification_redirects/__init__.py
+-rw-r--r--   0 andrzej    (503) staff       (20)        0 2021-10-12 00:14:12.000000 django-rest-registration-0.8.2/rest_registration/contrib/verification_redirects/admin.py
+-rw-r--r--   0 andrzej    (503) staff       (20)      225 2021-10-12 00:14:12.000000 django-rest-registration-0.8.2/rest_registration/contrib/verification_redirects/apps.py
+drwxr-xr-x   0 andrzej    (503) staff       (20)        0 2023-05-25 21:02:36.551253 django-rest-registration-0.8.2/rest_registration/contrib/verification_redirects/migrations/
+-rw-r--r--   0 andrzej    (503) staff       (20)        0 2021-10-12 00:14:12.000000 django-rest-registration-0.8.2/rest_registration/contrib/verification_redirects/migrations/__init__.py
+-rw-r--r--   0 andrzej    (503) staff       (20)        0 2021-10-12 00:14:12.000000 django-rest-registration-0.8.2/rest_registration/contrib/verification_redirects/models.py
+-rw-r--r--   0 andrzej    (503) staff       (20)      834 2023-03-18 23:27:11.000000 django-rest-registration-0.8.2/rest_registration/contrib/verification_redirects/settings.py
+-rw-r--r--   0 andrzej    (503) staff       (20)      393 2021-12-24 09:22:04.000000 django-rest-registration-0.8.2/rest_registration/contrib/verification_redirects/urls.py
+-rw-r--r--   0 andrzej    (503) staff       (20)     1975 2021-10-12 00:14:12.000000 django-rest-registration-0.8.2/rest_registration/contrib/verification_redirects/views.py
+-rw-r--r--   0 andrzej    (503) staff       (20)     1608 2023-05-08 21:35:32.000000 django-rest-registration-0.8.2/rest_registration/enums.py
+-rw-r--r--   0 andrzej    (503) staff       (20)     3767 2023-05-08 21:35:32.000000 django-rest-registration-0.8.2/rest_registration/exceptions.py
+drwxr-xr-x   0 andrzej    (503) staff       (20)        0 2023-05-25 21:02:36.463606 django-rest-registration-0.8.2/rest_registration/locale/
+drwxr-xr-x   0 andrzej    (503) staff       (20)        0 2023-05-25 21:02:36.461438 django-rest-registration-0.8.2/rest_registration/locale/de/
+drwxr-xr-x   0 andrzej    (503) staff       (20)        0 2023-05-25 21:02:36.553468 django-rest-registration-0.8.2/rest_registration/locale/de/LC_MESSAGES/
+-rw-r--r--   0 andrzej    (503) staff       (20)     3248 2023-05-25 20:57:44.000000 django-rest-registration-0.8.2/rest_registration/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 andrzej    (503) staff       (20)        0 2023-05-25 21:02:36.462200 django-rest-registration-0.8.2/rest_registration/locale/fr/
+drwxr-xr-x   0 andrzej    (503) staff       (20)        0 2023-05-25 21:02:36.554498 django-rest-registration-0.8.2/rest_registration/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 andrzej    (503) staff       (20)     2537 2022-12-18 10:57:04.000000 django-rest-registration-0.8.2/rest_registration/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 andrzej    (503) staff       (20)        0 2023-05-25 21:02:36.463039 django-rest-registration-0.8.2/rest_registration/locale/id/
+drwxr-xr-x   0 andrzej    (503) staff       (20)        0 2023-05-25 21:02:36.555928 django-rest-registration-0.8.2/rest_registration/locale/id/LC_MESSAGES/
+-rw-r--r--   0 andrzej    (503) staff       (20)     3159 2023-03-18 23:27:11.000000 django-rest-registration-0.8.2/rest_registration/locale/id/LC_MESSAGES/django.po
+drwxr-xr-x   0 andrzej    (503) staff       (20)        0 2023-05-25 21:02:36.464033 django-rest-registration-0.8.2/rest_registration/locale/pt_BR/
+drwxr-xr-x   0 andrzej    (503) staff       (20)        0 2023-05-25 21:02:36.558080 django-rest-registration-0.8.2/rest_registration/locale/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 andrzej    (503) staff       (20)     2304 2021-10-12 00:14:12.000000 django-rest-registration-0.8.2/rest_registration/locale/pt_BR/LC_MESSAGES/django.po
+drwxr-xr-x   0 andrzej    (503) staff       (20)        0 2023-05-25 21:02:36.559526 django-rest-registration-0.8.2/rest_registration/migrations/
+-rw-r--r--   0 andrzej    (503) staff       (20)        0 2021-10-12 00:14:12.000000 django-rest-registration-0.8.2/rest_registration/migrations/__init__.py
+-rw-r--r--   0 andrzej    (503) staff       (20)        0 2021-10-12 00:14:12.000000 django-rest-registration-0.8.2/rest_registration/models.py
+drwxr-xr-x   0 andrzej    (503) staff       (20)        0 2023-05-25 21:02:36.564628 django-rest-registration-0.8.2/rest_registration/notifications/
+-rw-r--r--   0 andrzej    (503) staff       (20)      133 2021-10-12 00:14:12.000000 django-rest-registration-0.8.2/rest_registration/notifications/__init__.py
+-rw-r--r--   0 andrzej    (503) staff       (20)     2426 2021-10-12 00:14:12.000000 django-rest-registration-0.8.2/rest_registration/notifications/email.py
+-rw-r--r--   0 andrzej    (503) staff       (20)      204 2021-10-12 00:14:12.000000 django-rest-registration-0.8.2/rest_registration/notifications/enums.py
+-rw-r--r--   0 andrzej    (503) staff       (20)      678 2023-03-18 23:27:11.000000 django-rest-registration-0.8.2/rest_registration/settings.py
+-rw-r--r--   0 andrzej    (503) staff       (20)    21417 2022-09-25 00:02:12.000000 django-rest-registration-0.8.2/rest_registration/settings_fields.py
+-rw-r--r--   0 andrzej    (503) staff       (20)      316 2021-12-24 09:22:04.000000 django-rest-registration-0.8.2/rest_registration/signals.py
+drwxr-xr-x   0 andrzej    (503) staff       (20)        0 2023-05-25 21:02:36.571159 django-rest-registration-0.8.2/rest_registration/signers/
+-rw-r--r--   0 andrzej    (503) staff       (20)        0 2021-10-12 00:14:12.000000 django-rest-registration-0.8.2/rest_registration/signers/__init__.py
+-rw-r--r--   0 andrzej    (503) staff       (20)     1405 2021-10-12 00:14:12.000000 django-rest-registration-0.8.2/rest_registration/signers/register.py
+-rw-r--r--   0 andrzej    (503) staff       (20)      428 2021-10-12 00:14:12.000000 django-rest-registration-0.8.2/rest_registration/signers/register_email.py
+-rw-r--r--   0 andrzej    (503) staff       (20)     1293 2021-10-12 00:14:12.000000 django-rest-registration-0.8.2/rest_registration/signers/reset_password.py
+drwxr-xr-x   0 andrzej    (503) staff       (20)        0 2023-05-25 21:02:36.466809 django-rest-registration-0.8.2/rest_registration/templates/
+drwxr-xr-x   0 andrzej    (503) staff       (20)        0 2023-05-25 21:02:36.469335 django-rest-registration-0.8.2/rest_registration/templates/rest_registration/
+drwxr-xr-x   0 andrzej    (503) staff       (20)        0 2023-05-25 21:02:36.577106 django-rest-registration-0.8.2/rest_registration/templates/rest_registration/register/
+-rw-r--r--   0 andrzej    (503) staff       (20)      255 2021-10-12 00:14:12.000000 django-rest-registration-0.8.2/rest_registration/templates/rest_registration/register/body.html
+-rw-r--r--   0 andrzej    (503) staff       (20)       84 2021-10-12 00:14:12.000000 django-rest-registration-0.8.2/rest_registration/templates/rest_registration/register/body.txt
+-rw-r--r--   0 andrzej    (503) staff       (20)       27 2021-10-12 00:14:12.000000 django-rest-registration-0.8.2/rest_registration/templates/rest_registration/register/subject.txt
+drwxr-xr-x   0 andrzej    (503) staff       (20)        0 2023-05-25 21:02:36.581598 django-rest-registration-0.8.2/rest_registration/templates/rest_registration/register_email/
+-rw-r--r--   0 andrzej    (503) staff       (20)      689 2021-10-12 00:14:12.000000 django-rest-registration-0.8.2/rest_registration/templates/rest_registration/register_email/body.html
+-rw-r--r--   0 andrzej    (503) staff       (20)      380 2021-10-12 00:14:12.000000 django-rest-registration-0.8.2/rest_registration/templates/rest_registration/register_email/body.txt
+-rw-r--r--   0 andrzej    (503) staff       (20)      102 2021-10-12 00:14:12.000000 django-rest-registration-0.8.2/rest_registration/templates/rest_registration/register_email/subject.txt
+drwxr-xr-x   0 andrzej    (503) staff       (20)        0 2023-05-25 21:02:36.592220 django-rest-registration-0.8.2/rest_registration/templates/rest_registration/reset_password/
+-rw-r--r--   0 andrzej    (503) staff       (20)      258 2021-10-12 00:14:12.000000 django-rest-registration-0.8.2/rest_registration/templates/rest_registration/reset_password/body.html
+-rw-r--r--   0 andrzej    (503) staff       (20)       85 2021-10-12 00:14:12.000000 django-rest-registration-0.8.2/rest_registration/templates/rest_registration/reset_password/body.txt
+-rw-r--r--   0 andrzej    (503) staff       (20)       29 2021-10-12 00:14:12.000000 django-rest-registration-0.8.2/rest_registration/templates/rest_registration/reset_password/subject.txt
+-rw-r--r--   0 andrzej    (503) staff       (20)        0 2021-10-12 00:14:12.000000 django-rest-registration-0.8.2/rest_registration/tests.py
+drwxr-xr-x   0 andrzej    (503) staff       (20)        0 2023-05-25 21:02:36.634793 django-rest-registration-0.8.2/rest_registration/utils/
+-rw-r--r--   0 andrzej    (503) staff       (20)        0 2021-10-12 00:14:12.000000 django-rest-registration-0.8.2/rest_registration/utils/__init__.py
+-rw-r--r--   0 andrzej    (503) staff       (20)     1038 2022-09-25 00:02:12.000000 django-rest-registration-0.8.2/rest_registration/utils/auth_backends.py
+-rw-r--r--   0 andrzej    (503) staff       (20)     2996 2023-03-18 23:27:11.000000 django-rest-registration-0.8.2/rest_registration/utils/checks.py
+-rw-r--r--   0 andrzej    (503) staff       (20)     1581 2021-12-25 23:58:02.000000 django-rest-registration-0.8.2/rest_registration/utils/common.py
+-rw-r--r--   0 andrzej    (503) staff       (20)     6751 2021-10-12 00:14:12.000000 django-rest-registration-0.8.2/rest_registration/utils/email.py
+-rw-r--r--   0 andrzej    (503) staff       (20)      955 2021-10-12 00:14:12.000000 django-rest-registration-0.8.2/rest_registration/utils/functools.py
+-rw-r--r--   0 andrzej    (503) staff       (20)     2706 2021-10-12 00:14:12.000000 django-rest-registration-0.8.2/rest_registration/utils/html.py
+-rw-r--r--   0 andrzej    (503) staff       (20)     1997 2022-03-12 09:20:39.000000 django-rest-registration-0.8.2/rest_registration/utils/nested_settings.py
+-rw-r--r--   0 andrzej    (503) staff       (20)      734 2021-10-12 00:14:12.000000 django-rest-registration-0.8.2/rest_registration/utils/responses.py
+-rw-r--r--   0 andrzej    (503) staff       (20)     3162 2023-03-18 23:27:11.000000 django-rest-registration-0.8.2/rest_registration/utils/signers.py
+-rw-r--r--   0 andrzej    (503) staff       (20)      599 2023-05-08 21:35:32.000000 django-rest-registration-0.8.2/rest_registration/utils/types.py
+-rw-r--r--   0 andrzej    (503) staff       (20)    11639 2023-05-08 21:35:32.000000 django-rest-registration-0.8.2/rest_registration/utils/users.py
+-rw-r--r--   0 andrzej    (503) staff       (20)     4364 2023-03-18 23:27:11.000000 django-rest-registration-0.8.2/rest_registration/utils/validation.py
+-rw-r--r--   0 andrzej    (503) staff       (20)     3731 2023-03-18 23:27:11.000000 django-rest-registration-0.8.2/rest_registration/utils/verification.py
+-rw-r--r--   0 andrzej    (503) staff       (20)     3520 2021-10-12 00:14:12.000000 django-rest-registration-0.8.2/rest_registration/verification_notifications.py
+-rw-r--r--   0 andrzej    (503) staff       (20)        0 2021-10-12 00:14:12.000000 django-rest-registration-0.8.2/rest_registration/views.py
+-rw-r--r--   0 andrzej    (503) staff       (20)       38 2023-05-25 21:02:36.639312 django-rest-registration-0.8.2/setup.cfg
+-rwxr-xr-x   0 andrzej    (503) staff       (20)      107 2023-05-08 21:35:32.000000 django-rest-registration-0.8.2/setup.py
```

### Comparing `django-rest-registration-0.8.1/LICENSE` & `django-rest-registration-0.8.2/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The MIT License (MIT)
 
-Copyright (c) 2015-2021 Andrzej Pragacz
+Copyright (c) 2015-2023 Andrzej Pragacz
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `django-rest-registration-0.8.1/PKG-INFO` & `django-rest-registration-0.8.2/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,38 +1,7 @@
-Metadata-Version: 2.1
-Name: django-rest-registration
-Version: 0.8.1
-Summary: User registration REST API, based on django-rest-framework
-Home-page: https://github.com/apragacz/django-rest-registration
-Author: Andrzej Pragacz
-Author-email: apragacz@o2.pl
-License: MIT
-Project-URL: Bug Tracker, https://github.com/apragacz/django-rest-registration/issues
-Project-URL: Documentation, https://django-rest-registration.readthedocs.io/
-Project-URL: Source Code, https://github.com/apragacz/django-rest-registration
-Keywords: django,rest,api,auth,rest-framework,registration,register,login,reset-password,register-email,change-email,sign-up,sign-in
-Classifier: Development Status :: 4 - Beta
-Classifier: Environment :: Web Environment
-Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.0
-Classifier: Framework :: Django :: 3.0
-Classifier: Framework :: Django :: 4.0
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: POSIX
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Topic :: Internet
-Classifier: Topic :: Internet :: WWW/HTTP
-Requires-Python: >=3.5
-Description-Content-Type: text/markdown; charset=UTF-8
-License-File: LICENSE
-
 # Django REST Registration
 
 [![CircleCI Build Status](https://circleci.com/gh/apragacz/django-rest-registration.svg?style=shield)](https://circleci.com/gh/apragacz/django-rest-registration)
 [![Codecov Coverage](https://codecov.io/gh/apragacz/django-rest-registration/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/apragacz/django-rest-registration?branch=master)
 [![PyPi Version](https://badge.fury.io/py/django-rest-registration.svg)](https://pypi.python.org/pypi/django-rest-registration/)
 [![Documentation Status](https://readthedocs.org/projects/django-rest-registration/badge/?version=latest)](https://django-rest-registration.readthedocs.io/en/latest/?badge=latest)
```

### Comparing `django-rest-registration-0.8.1/README.md` & `django-rest-registration-0.8.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,58 @@
+Metadata-Version: 2.1
+Name: django-rest-registration
+Version: 0.8.2
+Summary: User registration REST API, based on django-rest-framework
+Author-email: Andrzej Pragacz <apragacz@o2.pl>
+License: The MIT License (MIT)
+        
+        Copyright (c) 2015-2023 Andrzej Pragacz
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+        
+Project-URL: homepage, https://github.com/apragacz/django-rest-registration
+Project-URL: Bug Tracker, https://github.com/apragacz/django-rest-registration/issues
+Project-URL: Documentation, https://django-rest-registration.readthedocs.io/
+Project-URL: Source Code, https://github.com/apragacz/django-rest-registration
+Keywords: django,rest,api,auth,rest-framework,registration,register,login,reset-password,register-email,change-email,sign-up,sign-in
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Web Environment
+Classifier: Framework :: Django
+Classifier: Framework :: Django :: 2.0
+Classifier: Framework :: Django :: 3.0
+Classifier: Framework :: Django :: 4.0
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Topic :: Internet
+Classifier: Topic :: Internet :: WWW/HTTP
+Requires-Python: >=3.5
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Django REST Registration
 
 [![CircleCI Build Status](https://circleci.com/gh/apragacz/django-rest-registration.svg?style=shield)](https://circleci.com/gh/apragacz/django-rest-registration)
 [![Codecov Coverage](https://codecov.io/gh/apragacz/django-rest-registration/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/apragacz/django-rest-registration?branch=master)
 [![PyPi Version](https://badge.fury.io/py/django-rest-registration.svg)](https://pypi.python.org/pypi/django-rest-registration/)
 [![Documentation Status](https://readthedocs.org/projects/django-rest-registration/badge/?version=latest)](https://django-rest-registration.readthedocs.io/en/latest/?badge=latest)
```

### Comparing `django-rest-registration-0.8.1/django_rest_registration.egg-info/PKG-INFO` & `django-rest-registration-0.8.2/django_rest_registration.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,36 +1,56 @@
 Metadata-Version: 2.1
 Name: django-rest-registration
-Version: 0.8.1
+Version: 0.8.2
 Summary: User registration REST API, based on django-rest-framework
-Home-page: https://github.com/apragacz/django-rest-registration
-Author: Andrzej Pragacz
-Author-email: apragacz@o2.pl
-License: MIT
+Author-email: Andrzej Pragacz <apragacz@o2.pl>
+License: The MIT License (MIT)
+        
+        Copyright (c) 2015-2023 Andrzej Pragacz
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+        
+Project-URL: homepage, https://github.com/apragacz/django-rest-registration
 Project-URL: Bug Tracker, https://github.com/apragacz/django-rest-registration/issues
 Project-URL: Documentation, https://django-rest-registration.readthedocs.io/
 Project-URL: Source Code, https://github.com/apragacz/django-rest-registration
 Keywords: django,rest,api,auth,rest-framework,registration,register,login,reset-password,register-email,change-email,sign-up,sign-in
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.0
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: POSIX
-Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Internet
 Classifier: Topic :: Internet :: WWW/HTTP
 Requires-Python: >=3.5
-Description-Content-Type: text/markdown; charset=UTF-8
+Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Django REST Registration
 
 [![CircleCI Build Status](https://circleci.com/gh/apragacz/django-rest-registration.svg?style=shield)](https://circleci.com/gh/apragacz/django-rest-registration)
 [![Codecov Coverage](https://codecov.io/gh/apragacz/django-rest-registration/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/apragacz/django-rest-registration?branch=master)
 [![PyPi Version](https://badge.fury.io/py/django-rest-registration.svg)](https://pypi.python.org/pypi/django-rest-registration/)
```

### Comparing `django-rest-registration-0.8.1/django_rest_registration.egg-info/SOURCES.txt` & `django-rest-registration-0.8.2/django_rest_registration.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 LICENSE
 MANIFEST.in
 README.md
-setup.cfg
+pyproject.toml
 setup.py
 django_rest_registration.egg-info/PKG-INFO
 django_rest_registration.egg-info/SOURCES.txt
 django_rest_registration.egg-info/dependency_links.txt
 django_rest_registration.egg-info/requires.txt
 django_rest_registration.egg-info/top_level.txt
 rest_registration/__init__.py
@@ -39,14 +39,15 @@
 rest_registration/contrib/verification_redirects/admin.py
 rest_registration/contrib/verification_redirects/apps.py
 rest_registration/contrib/verification_redirects/models.py
 rest_registration/contrib/verification_redirects/settings.py
 rest_registration/contrib/verification_redirects/urls.py
 rest_registration/contrib/verification_redirects/views.py
 rest_registration/contrib/verification_redirects/migrations/__init__.py
+rest_registration/locale/de/LC_MESSAGES/django.po
 rest_registration/locale/fr/LC_MESSAGES/django.po
 rest_registration/locale/id/LC_MESSAGES/django.po
 rest_registration/locale/pt_BR/LC_MESSAGES/django.po
 rest_registration/migrations/__init__.py
 rest_registration/notifications/__init__.py
 rest_registration/notifications/email.py
 rest_registration/notifications/enums.py
```

### Comparing `django-rest-registration-0.8.1/rest_registration/api/serializers.py` & `django-rest-registration-0.8.2/rest_registration/api/serializers.py`

 * *Files identical despite different names*

### Comparing `django-rest-registration-0.8.1/rest_registration/api/urls.py` & `django-rest-registration-0.8.2/rest_registration/api/urls.py`

 * *Files identical despite different names*

### Comparing `django-rest-registration-0.8.1/rest_registration/api/views/base.py` & `django-rest-registration-0.8.2/rest_registration/api/views/base.py`

 * *Files identical despite different names*

### Comparing `django-rest-registration-0.8.1/rest_registration/api/views/change_password.py` & `django-rest-registration-0.8.2/rest_registration/api/views/change_password.py`

 * *Files identical despite different names*

### Comparing `django-rest-registration-0.8.1/rest_registration/api/views/login.py` & `django-rest-registration-0.8.2/rest_registration/api/views/login.py`

 * *Files identical despite different names*

### Comparing `django-rest-registration-0.8.1/rest_registration/api/views/profile.py` & `django-rest-registration-0.8.2/rest_registration/api/views/profile.py`

 * *Files identical despite different names*

### Comparing `django-rest-registration-0.8.1/rest_registration/api/views/register.py` & `django-rest-registration-0.8.2/rest_registration/api/views/register.py`

 * *Files identical despite different names*

### Comparing `django-rest-registration-0.8.1/rest_registration/api/views/register_email.py` & `django-rest-registration-0.8.2/rest_registration/api/views/register_email.py`

 * *Files identical despite different names*

### Comparing `django-rest-registration-0.8.1/rest_registration/api/views/reset_password.py` & `django-rest-registration-0.8.2/rest_registration/api/views/reset_password.py`

 * *Files identical despite different names*

### Comparing `django-rest-registration-0.8.1/rest_registration/auth_token_managers.py` & `django-rest-registration-0.8.2/rest_registration/auth_token_managers.py`

 * *Files 5% similar despite different names*

```diff
@@ -61,23 +61,25 @@
 
     def get_app_names(self) -> Sequence[str]:
         return [
             'rest_framework.authtoken',
         ]
 
     def provide_token(self, user: 'AbstractBaseUser') -> AuthToken:
-        from rest_framework.authtoken.models import Token  # noqa: E501 pylint: disable=import-outside-toplevel
+        from rest_framework.authtoken.models import \
+            Token  # noqa: E501 pylint: disable=import-outside-toplevel
 
         token_obj, _ = Token.objects.get_or_create(user=user)
         return AuthToken(token_obj.key)
 
     def revoke_token(
             self, user: 'AbstractBaseUser', *,
             token: Optional[AuthToken] = None) -> None:
-        from rest_framework.authtoken.models import Token  # noqa: E501 pylint: disable=import-outside-toplevel
+        from rest_framework.authtoken.models import \
+            Token  # noqa: E501 pylint: disable=import-outside-toplevel
 
         try:
             token_obj = Token.objects.get(user_id=user.pk)  # type: Token
         except Token.DoesNotExist:
             raise AuthTokenNotFound() from None
 
         if token is not None and token_obj.key != token:
```

### Comparing `django-rest-registration-0.8.1/rest_registration/checks.py` & `django-rest-registration-0.8.2/rest_registration/checks.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from functools import partial
 from typing import TYPE_CHECKING, Type
 
 from django.conf import settings
 from django.contrib.auth import get_user_model
 from django.core.checks import register
-from django.core.exceptions import ImproperlyConfigured
 from rest_framework.settings import api_settings
 
 from rest_registration.auth_token_managers import AbstractAuthTokenManager
 from rest_registration.enums import ErrorCode, WarningCode
 from rest_registration.settings import registration_settings
 from rest_registration.utils.auth_backends import get_login_authentication_backend
 from rest_registration.utils.checks import no_exception_check, predicate_check
@@ -208,22 +207,14 @@
                         'REGISTER_EMAIL_VERIFICATION_EMAIL_SENDER'))
     _validate_email_template_config(
         sends_emails,
         registration_settings.REGISTER_EMAIL_VERIFICATION_EMAIL_TEMPLATES,
     )
 
 
-def _is_email_template_config_valid(template_config_data) -> bool:
-    try:
-        parse_template_config(template_config_data)
-    except ImproperlyConfigured:
-        return False
-    return True
-
-
 def _validate_email_template_config(enabled, template_config_data) -> None:
     if not enabled:
         return
     parse_template_config(template_config_data)
 
 
 # The backends below allow inactive users to autenticate, which makes them
```

### Comparing `django-rest-registration-0.8.1/rest_registration/contrib/verification_redirects/settings.py` & `django-rest-registration-0.8.2/rest_registration/contrib/verification_redirects/settings.py`

 * *Files identical despite different names*

### Comparing `django-rest-registration-0.8.1/rest_registration/contrib/verification_redirects/views.py` & `django-rest-registration-0.8.2/rest_registration/contrib/verification_redirects/views.py`

 * *Files identical despite different names*

### Comparing `django-rest-registration-0.8.1/rest_registration/enums.py` & `django-rest-registration-0.8.2/rest_registration/enums.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,17 @@
 
 from rest_registration.utils.checks import CheckCode, CheckMessage
 
 
 class _BaseCheckCodeMixin(CheckCode):  # noqa: E501 pylint: disable=abstract-method
 
     def get_app_name(self) -> str:
-        from rest_registration.apps import RestRegistrationConfig  # noqa: E501 pylint: disable=import-outside-toplevel, cyclic-import
+        from rest_registration.apps import \
+            RestRegistrationConfig  # noqa: E501 pylint: disable=import-outside-toplevel, cyclic-import
+
         return RestRegistrationConfig.name
 
 
 class ErrorCode(_BaseCheckCodeMixin, Enum):
     NO_RESET_PASSWORD_VER_URL = 1
     NO_REGISTER_VER_URL = 2
     NO_REGISTER_EMAIL_VER_URL = 3
```

### Comparing `django-rest-registration-0.8.1/rest_registration/exceptions.py` & `django-rest-registration-0.8.2/rest_registration/exceptions.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,37 @@
-from typing import Any, Dict, List, Optional, Union
+from typing import Any, Dict, List, Mapping, Optional, Sequence, Union
 
 from django.utils.translation import gettext_lazy as _
 from rest_framework.exceptions import APIException as _APIException
+from rest_framework.exceptions import ErrorDetail
 from rest_framework.settings import api_settings
 
 from rest_registration.settings import registration_settings
 from rest_registration.utils.types import StrOrPromise
 
-_DetailType = Union[StrOrPromise, List[str], Dict[str, List[str]]]
+# _Detail = Union[StrOrPromise, List[str], Dict[str, List[str]]]
+_Detail = Union[
+    ErrorDetail,
+    List[ErrorDetail],
+    Dict[str, ErrorDetail],
+]
+_APIExceptionInput = Union[
+    _Detail,
+    StrOrPromise,
+    Sequence["_APIExceptionInput"],
+    Mapping[str, "_APIExceptionInput"],
+    None,
+]
 
 
 class APIException(_APIException):
 
     def __init__(
             self,
-            detail: Optional[_DetailType] = None,
+            detail: Optional[_APIExceptionInput] = None,
             code: Optional[str] = None) -> None:
         if detail is None:
             detail = self.default_detail
         if code is None:
             code = self.default_code
 
         if registration_settings.USE_NON_FIELD_ERRORS_KEY_FROM_DRF_SETTINGS:
@@ -90,13 +103,23 @@
 
 class VerificationTemplatesNotFound(APIException):
     status_code = 500
     default_detail = _("Could not find verification templates")
     default_code = 'verification-templates-not-found'
 
 
-def _wrap_detail_in_dict(detail: _DetailType) -> Dict[str, List[Any]]:
+def _wrap_detail_in_dict(detail: _APIExceptionInput) -> Dict[str, List[Any]]:
     if isinstance(detail, list):
         return {api_settings.NON_FIELD_ERRORS_KEY: detail}
     if isinstance(detail, dict):
-        return detail
+        return {k: _extract_details(v) for k, v in detail.items()}
     return {api_settings.NON_FIELD_ERRORS_KEY: [detail]}
+
+
+def _extract_details(detail: _APIExceptionInput) -> List[Union[_Detail, StrOrPromise]]:
+    if detail is None:
+        return []
+    if isinstance(detail, Mapping):
+        return [ed for d in detail.values() for ed in _extract_details(d)]
+    if isinstance(detail, Sequence) and not isinstance(detail, str):
+        return [ed for d in detail for ed in _extract_details(d)]
+    return [detail]
```

### Comparing `django-rest-registration-0.8.1/rest_registration/locale/fr/LC_MESSAGES/django.po` & `django-rest-registration-0.8.2/rest_registration/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-rest-registration-0.8.1/rest_registration/locale/id/LC_MESSAGES/django.po` & `django-rest-registration-0.8.2/rest_registration/locale/id/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-rest-registration-0.8.1/rest_registration/locale/pt_BR/LC_MESSAGES/django.po` & `django-rest-registration-0.8.2/rest_registration/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-rest-registration-0.8.1/rest_registration/notifications/email.py` & `django-rest-registration-0.8.2/rest_registration/notifications/email.py`

 * *Files identical despite different names*

### Comparing `django-rest-registration-0.8.1/rest_registration/settings.py` & `django-rest-registration-0.8.2/rest_registration/settings.py`

 * *Files identical despite different names*

### Comparing `django-rest-registration-0.8.1/rest_registration/settings_fields.py` & `django-rest-registration-0.8.2/rest_registration/settings_fields.py`

 * *Files identical despite different names*

### Comparing `django-rest-registration-0.8.1/rest_registration/signers/register.py` & `django-rest-registration-0.8.2/rest_registration/signers/register.py`

 * *Files identical despite different names*

### Comparing `django-rest-registration-0.8.1/rest_registration/signers/reset_password.py` & `django-rest-registration-0.8.2/rest_registration/signers/reset_password.py`

 * *Files identical despite different names*

### Comparing `django-rest-registration-0.8.1/rest_registration/templates/rest_registration/register_email/body.html` & `django-rest-registration-0.8.2/rest_registration/templates/rest_registration/register_email/body.html`

 * *Files identical despite different names*

### Comparing `django-rest-registration-0.8.1/rest_registration/utils/auth_backends.py` & `django-rest-registration-0.8.2/rest_registration/utils/auth_backends.py`

 * *Files identical despite different names*

### Comparing `django-rest-registration-0.8.1/rest_registration/utils/checks.py` & `django-rest-registration-0.8.2/rest_registration/utils/checks.py`

 * *Files identical despite different names*

### Comparing `django-rest-registration-0.8.1/rest_registration/utils/common.py` & `django-rest-registration-0.8.2/rest_registration/utils/common.py`

 * *Files identical despite different names*

### Comparing `django-rest-registration-0.8.1/rest_registration/utils/email.py` & `django-rest-registration-0.8.2/rest_registration/utils/email.py`

 * *Files identical despite different names*

### Comparing `django-rest-registration-0.8.1/rest_registration/utils/functools.py` & `django-rest-registration-0.8.2/rest_registration/utils/functools.py`

 * *Files identical despite different names*

### Comparing `django-rest-registration-0.8.1/rest_registration/utils/html.py` & `django-rest-registration-0.8.2/rest_registration/utils/html.py`

 * *Files identical despite different names*

### Comparing `django-rest-registration-0.8.1/rest_registration/utils/nested_settings.py` & `django-rest-registration-0.8.2/rest_registration/utils/nested_settings.py`

 * *Files identical despite different names*

### Comparing `django-rest-registration-0.8.1/rest_registration/utils/responses.py` & `django-rest-registration-0.8.2/rest_registration/utils/responses.py`

 * *Files identical despite different names*

### Comparing `django-rest-registration-0.8.1/rest_registration/utils/signers.py` & `django-rest-registration-0.8.2/rest_registration/utils/signers.py`

 * *Files identical despite different names*

### Comparing `django-rest-registration-0.8.1/rest_registration/utils/types.py` & `django-rest-registration-0.8.2/rest_registration/utils/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from django_stubs_ext import StrOrPromise
-
     # mypy uses typing_extensions by default (Py 3.8); when importing from typing
     # one will get the following error message in mypy:
     #
     #   Incompatible import of "Literal"
     #   (imported name has type "typing_extensions._SpecialForm", local name has type
     #   "typing._SpecialForm")
     from typing_extensions import Literal
```

### Comparing `django-rest-registration-0.8.1/rest_registration/utils/users.py` & `django-rest-registration-0.8.2/rest_registration/utils/users.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 from rest_registration.utils.types import Literal
 
 _DefaultT = TypeVar('_DefaultT')
 _ModelT = TypeVar('_ModelT', bound=Model)
 
 if TYPE_CHECKING:
     from typing import Optional
+
     from django.contrib.auth.base_user import AbstractBaseUser
     from django.contrib.contenttypes.fields import GenericForeignKey
     from django.db.models import Field, ForeignObjectRel
 
     UserField = Union[Field[Any, Any], ForeignObjectRel, GenericForeignKey]
```

### Comparing `django-rest-registration-0.8.1/rest_registration/utils/validation.py` & `django-rest-registration-0.8.2/rest_registration/utils/validation.py`

 * *Files identical despite different names*

### Comparing `django-rest-registration-0.8.1/rest_registration/utils/verification.py` & `django-rest-registration-0.8.2/rest_registration/utils/verification.py`

 * *Files identical despite different names*

### Comparing `django-rest-registration-0.8.1/rest_registration/verification_notifications.py` & `django-rest-registration-0.8.2/rest_registration/verification_notifications.py`

 * *Files identical despite different names*

