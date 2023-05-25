# Comparing `tmp/simple_openid_connect-0.2.2.tar.gz` & `tmp/simple_openid_connect-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_openid_connect-0.2.2.tar", last modified: Fri May 12 10:42:36 2023, max compression
+gzip compressed data, was "simple_openid_connect-0.2.3.tar", last modified: Thu May 25 12:22:25 2023, max compression
```

## Comparing `simple_openid_connect-0.2.2.tar` & `simple_openid_connect-0.2.3.tar`

### file list

```diff
@@ -1,76 +1,76 @@
--rw-r--r--   0        0        0       50 2022-11-30 14:49:54.727128 simple_openid_connect-0.2.2/.gitattributes
--rw-r--r--   0        0        0     1584 2022-12-08 12:24:29.349860 simple_openid_connect-0.2.2/.github/workflows/checks.yml
--rw-r--r--   0        0        0      136 2022-11-24 12:36:21.336726 simple_openid_connect-0.2.2/.gitignore
--rw-r--r--   0        0        0      795 2023-05-01 11:17:06.824014 simple_openid_connect-0.2.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      177 2022-11-12 20:14:29.642701 simple_openid_connect-0.2.2/.readthedocs.yaml
--rw-r--r--   0        0        0      298 2023-05-01 11:41:49.264155 simple_openid_connect-0.2.2/DEVELOPMENT.md
--rw-r--r--   0        0        0     1116 2022-11-11 18:16:08.603350 simple_openid_connect-0.2.2/LICENSE
--rw-r--r--   0        0        0     4447 2023-05-01 11:17:53.814441 simple_openid_connect-0.2.2/README.md
--rw-r--r--   0        0        0      679 2022-11-13 10:21:55.698024 simple_openid_connect-0.2.2/docs/Makefile
--rw-r--r--   0        0        0        0 2022-11-11 18:16:08.603350 simple_openid_connect-0.2.2/docs/_static/.gitkeep
--rw-r--r--   0        0        0        0 2022-11-11 18:16:08.603350 simple_openid_connect-0.2.2/docs/_templates/.gitkeep
--rw-r--r--   0        0        0      320 2022-12-01 10:05:47.886671 simple_openid_connect-0.2.2/docs/api.rst
--rw-r--r--   0        0        0     1790 2022-12-08 12:24:29.349860 simple_openid_connect-0.2.2/docs/conf.py
--rw-r--r--   0        0        0     5429 2022-12-08 12:24:29.349860 simple_openid_connect-0.2.2/docs/django-integration.rst
--rw-r--r--   0        0        0     2615 2022-12-08 12:24:29.349860 simple_openid_connect-0.2.2/docs/drf-integration.rst
--rw-r--r--   0        0        0      708 2022-12-08 12:24:29.349860 simple_openid_connect-0.2.2/docs/index.rst
--rw-r--r--   0        0        0     1247 2023-05-01 09:33:59.061101 simple_openid_connect-0.2.2/docs/installation.rst
--rw-r--r--   0        0        0     4868 2022-11-30 16:29:18.260734 simple_openid_connect-0.2.2/docs/usage.rst
--rw-r--r--   0        0        0     2391 2022-12-08 12:24:29.349860 simple_openid_connect-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      211 2022-12-08 12:24:29.349860 simple_openid_connect-0.2.2/requirements.dev.txt
--rw-r--r--   0        0        0      127 2023-05-12 10:38:56.522715 simple_openid_connect-0.2.2/src/simple_openid_connect/__init__.py
--rw-r--r--   0        0        0     4204 2022-12-08 12:24:29.349860 simple_openid_connect-0.2.2/src/simple_openid_connect/base_data.py
--rw-r--r--   0        0        0    10682 2023-05-12 10:38:37.245804 simple_openid_connect-0.2.2/src/simple_openid_connect/client.py
--rw-r--r--   0        0        0     3443 2022-11-16 07:19:49.333600 simple_openid_connect-0.2.2/src/simple_openid_connect/client_authentication.py
--rw-r--r--   0        0        0    57231 2023-05-01 11:33:35.079663 simple_openid_connect-0.2.2/src/simple_openid_connect/data.py
--rw-r--r--   0        0        0     1819 2022-11-30 12:04:05.293339 simple_openid_connect-0.2.2/src/simple_openid_connect/discovery.py
--rw-r--r--   0        0        0     1174 2022-12-01 11:36:58.020255 simple_openid_connect-0.2.2/src/simple_openid_connect/exceptions.py
--rw-r--r--   0        0        0      343 2023-05-01 11:17:53.814441 simple_openid_connect-0.2.2/src/simple_openid_connect/flows/__init__.py
--rw-r--r--   0        0        0     5631 2022-11-16 07:19:49.333600 simple_openid_connect-0.2.2/src/simple_openid_connect/flows/authorization_code_flow/__init__.py
--rw-r--r--   0        0        0     6115 2022-12-01 11:36:58.243589 simple_openid_connect-0.2.2/src/simple_openid_connect/flows/authorization_code_flow/client.py
--rw-r--r--   0        0        0     2208 2023-05-01 11:18:30.258106 simple_openid_connect-0.2.2/src/simple_openid_connect/flows/direct_access_grant/__init__.py
--rw-r--r--   0        0        0     1583 2023-05-01 11:18:30.258106 simple_openid_connect-0.2.2/src/simple_openid_connect/flows/direct_access_grant/client.py
--rw-r--r--   0        0        0       53 2022-12-08 12:24:29.349860 simple_openid_connect-0.2.2/src/simple_openid_connect/integrations/__init__.py
--rw-r--r--   0        0        0       61 2022-12-01 10:05:47.886671 simple_openid_connect-0.2.2/src/simple_openid_connect/integrations/django/__init__.py
--rw-r--r--   0        0        0     5467 2023-05-01 11:22:04.083382 simple_openid_connect-0.2.2/src/simple_openid_connect/integrations/django/apps.py
--rw-r--r--   0        0        0     4555 2022-12-01 10:05:47.886671 simple_openid_connect-0.2.2/src/simple_openid_connect/integrations/django/decorators.py
--rw-r--r--   0        0        0     2630 2023-05-01 11:22:04.076716 simple_openid_connect-0.2.2/src/simple_openid_connect/integrations/django/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2022-12-01 10:05:47.886671 simple_openid_connect-0.2.2/src/simple_openid_connect/integrations/django/migrations/__init__.py
--rw-r--r--   0        0        0     5728 2022-12-01 11:42:37.006937 simple_openid_connect-0.2.2/src/simple_openid_connect/integrations/django/models.py
--rw-r--r--   0        0        0      381 2022-12-01 10:05:47.886671 simple_openid_connect-0.2.2/src/simple_openid_connect/integrations/django/templates/simple_openid_connect/login_failed.html
--rw-r--r--   0        0        0      729 2022-12-08 12:24:29.349860 simple_openid_connect-0.2.2/src/simple_openid_connect/integrations/django/urls.py
--rw-r--r--   0        0        0     2338 2022-12-01 10:05:47.886671 simple_openid_connect-0.2.2/src/simple_openid_connect/integrations/django/user_mapping.py
--rw-r--r--   0        0        0     4222 2023-05-01 16:41:31.144271 simple_openid_connect-0.2.2/src/simple_openid_connect/integrations/django/views.py
--rw-r--r--   0        0        0      306 2022-12-08 12:24:29.353193 simple_openid_connect-0.2.2/src/simple_openid_connect/integrations/djangorestframework/__init__.py
--rw-r--r--   0        0        0     4648 2022-12-08 12:24:29.353193 simple_openid_connect-0.2.2/src/simple_openid_connect/integrations/djangorestframework/authentication.py
--rw-r--r--   0        0        0      957 2022-12-08 12:24:29.353193 simple_openid_connect-0.2.2/src/simple_openid_connect/integrations/djangorestframework/drf_spectacular_schema.py
--rw-r--r--   0        0        0     2531 2022-12-08 12:24:29.353193 simple_openid_connect-0.2.2/src/simple_openid_connect/integrations/djangorestframework/permissions.py
--rw-r--r--   0        0        0      472 2022-11-16 07:19:49.333600 simple_openid_connect-0.2.2/src/simple_openid_connect/jwk.py
--rw-r--r--   0        0        0      621 2022-11-16 07:19:49.333600 simple_openid_connect-0.2.2/src/simple_openid_connect/rp_initiated_logout.py
--rw-r--r--   0        0        0     1509 2022-11-16 07:19:49.333600 simple_openid_connect-0.2.2/src/simple_openid_connect/token_introspection.py
--rw-r--r--   0        0        0     1566 2022-11-16 07:19:49.333600 simple_openid_connect-0.2.2/src/simple_openid_connect/token_refresh.py
--rw-r--r--   0        0        0     1393 2022-11-12 19:48:31.467498 simple_openid_connect-0.2.2/src/simple_openid_connect/userinfo.py
--rw-r--r--   0        0        0      781 2022-11-16 07:19:49.333600 simple_openid_connect-0.2.2/src/simple_openid_connect/utils.py
--rw-r--r--   0        0        0    16938 2022-12-08 12:24:29.353193 simple_openid_connect-0.2.2/tests/conftest.py
--rw-r--r--   0        0        0        0 2022-11-16 07:19:49.333600 simple_openid_connect-0.2.2/tests/django_test_project/django_test_project/__init__.py
--rw-r--r--   0        0        0     2785 2022-12-01 10:05:47.890004 simple_openid_connect-0.2.2/tests/django_test_project/django_test_project/settings.py
--rw-r--r--   0        0        0     2586 2022-12-08 12:24:29.353193 simple_openid_connect-0.2.2/tests/django_test_project/django_test_project/tests/conftest.py
--rw-r--r--   0        0        0     1541 2022-12-08 12:24:29.353193 simple_openid_connect-0.2.2/tests/django_test_project/django_test_project/tests/test_access_token_protected_view.py
--rw-r--r--   0        0        0      633 2022-12-08 12:24:29.353193 simple_openid_connect-0.2.2/tests/django_test_project/django_test_project/tests/test_frontchannel_logout_notifications.py
--rw-r--r--   0        0        0     5390 2022-12-08 12:24:29.353193 simple_openid_connect-0.2.2/tests/django_test_project/django_test_project/tests/test_login.py
--rw-r--r--   0        0        0      687 2022-12-08 12:24:29.353193 simple_openid_connect-0.2.2/tests/django_test_project/django_test_project/tests/test_logout.py
--rw-r--r--   0        0        0     1248 2022-12-01 10:05:47.890004 simple_openid_connect-0.2.2/tests/django_test_project/django_test_project/urls.py
--rw-r--r--   0        0        0      639 2022-12-01 10:05:47.890004 simple_openid_connect-0.2.2/tests/django_test_project/django_test_project/views.py
--rw-r--r--   0        0        0      415 2022-11-16 07:19:49.333600 simple_openid_connect-0.2.2/tests/django_test_project/django_test_project/wsgi.py
--rwxr-xr-x   0        0        0      675 2022-11-16 07:19:49.333600 simple_openid_connect-0.2.2/tests/django_test_project/manage.py
--rw-r--r--   0        0        0     1746 2022-11-30 13:30:16.836909 simple_openid_connect-0.2.2/tests/interactive_tests/conftest.py
--rw-r--r--   0        0        0     2001 2022-12-08 12:24:29.353193 simple_openid_connect-0.2.2/tests/interactive_tests/test_google.py
--rw-r--r--   0        0        0     1668 2022-12-08 12:24:29.366526 simple_openid_connect-0.2.2/tests/test_authorization_code_flow.py
--rw-r--r--   0        0        0     5139 2023-05-12 10:35:13.267423 simple_openid_connect-0.2.2/tests/test_client.py
--rw-r--r--   0        0        0      934 2022-12-08 12:24:29.366526 simple_openid_connect-0.2.2/tests/test_client_auth.py
--rw-r--r--   0        0        0     1378 2023-05-01 11:18:29.554766 simple_openid_connect-0.2.2/tests/test_direct_access_grant.py
--rw-r--r--   0        0        0     1541 2022-12-08 12:24:29.366526 simple_openid_connect-0.2.2/tests/test_discovery.py
--rw-r--r--   0        0        0      590 2022-12-08 12:24:29.366526 simple_openid_connect-0.2.2/tests/test_jwk.py
--rw-r--r--   0        0        0     2274 2022-11-13 10:28:27.455234 simple_openid_connect-0.2.2/tests/test_message_encoding.py
--rw-r--r--   0        0        0      581 2022-11-12 19:48:31.434164 simple_openid_connect-0.2.2/tests/test_rp_initiated_logout.py
--rw-r--r--   0        0        0     5760 1970-01-01 00:00:00.000000 simple_openid_connect-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0       50 2022-11-30 14:49:54.727128 simple_openid_connect-0.2.3/.gitattributes
+-rw-r--r--   0        0        0     1584 2022-12-08 12:24:29.349860 simple_openid_connect-0.2.3/.github/workflows/checks.yml
+-rw-r--r--   0        0        0      136 2022-11-24 12:36:21.336726 simple_openid_connect-0.2.3/.gitignore
+-rw-r--r--   0        0        0      795 2023-05-01 11:17:06.824014 simple_openid_connect-0.2.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      177 2022-11-12 20:14:29.642701 simple_openid_connect-0.2.3/.readthedocs.yaml
+-rw-r--r--   0        0        0      298 2023-05-01 11:41:49.264155 simple_openid_connect-0.2.3/DEVELOPMENT.md
+-rw-r--r--   0        0        0     1116 2022-11-11 18:16:08.603350 simple_openid_connect-0.2.3/LICENSE
+-rw-r--r--   0        0        0     4447 2023-05-01 11:17:53.814441 simple_openid_connect-0.2.3/README.md
+-rw-r--r--   0        0        0      679 2022-11-13 10:21:55.698024 simple_openid_connect-0.2.3/docs/Makefile
+-rw-r--r--   0        0        0        0 2022-11-11 18:16:08.603350 simple_openid_connect-0.2.3/docs/_static/.gitkeep
+-rw-r--r--   0        0        0        0 2022-11-11 18:16:08.603350 simple_openid_connect-0.2.3/docs/_templates/.gitkeep
+-rw-r--r--   0        0        0      320 2022-12-01 10:05:47.886671 simple_openid_connect-0.2.3/docs/api.rst
+-rw-r--r--   0        0        0     1790 2022-12-08 12:24:29.349860 simple_openid_connect-0.2.3/docs/conf.py
+-rw-r--r--   0        0        0     5754 2023-05-25 12:20:30.617684 simple_openid_connect-0.2.3/docs/django-integration.rst
+-rw-r--r--   0        0        0     2615 2022-12-08 12:24:29.349860 simple_openid_connect-0.2.3/docs/drf-integration.rst
+-rw-r--r--   0        0        0      708 2022-12-08 12:24:29.349860 simple_openid_connect-0.2.3/docs/index.rst
+-rw-r--r--   0        0        0     1247 2023-05-01 09:33:59.061101 simple_openid_connect-0.2.3/docs/installation.rst
+-rw-r--r--   0        0        0     4868 2022-11-30 16:29:18.260734 simple_openid_connect-0.2.3/docs/usage.rst
+-rw-r--r--   0        0        0     2391 2022-12-08 12:24:29.349860 simple_openid_connect-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      211 2022-12-08 12:24:29.349860 simple_openid_connect-0.2.3/requirements.dev.txt
+-rw-r--r--   0        0        0      127 2023-05-25 12:20:52.367848 simple_openid_connect-0.2.3/src/simple_openid_connect/__init__.py
+-rw-r--r--   0        0        0     4204 2022-12-08 12:24:29.349860 simple_openid_connect-0.2.3/src/simple_openid_connect/base_data.py
+-rw-r--r--   0        0        0    10682 2023-05-12 10:38:37.245804 simple_openid_connect-0.2.3/src/simple_openid_connect/client.py
+-rw-r--r--   0        0        0     3443 2022-11-16 07:19:49.333600 simple_openid_connect-0.2.3/src/simple_openid_connect/client_authentication.py
+-rw-r--r--   0        0        0    57273 2023-05-25 12:20:30.621017 simple_openid_connect-0.2.3/src/simple_openid_connect/data.py
+-rw-r--r--   0        0        0     1819 2022-11-30 12:04:05.293339 simple_openid_connect-0.2.3/src/simple_openid_connect/discovery.py
+-rw-r--r--   0        0        0     1174 2022-12-01 11:36:58.020255 simple_openid_connect-0.2.3/src/simple_openid_connect/exceptions.py
+-rw-r--r--   0        0        0      343 2023-05-01 11:17:53.814441 simple_openid_connect-0.2.3/src/simple_openid_connect/flows/__init__.py
+-rw-r--r--   0        0        0     5631 2022-11-16 07:19:49.333600 simple_openid_connect-0.2.3/src/simple_openid_connect/flows/authorization_code_flow/__init__.py
+-rw-r--r--   0        0        0     6115 2022-12-01 11:36:58.243589 simple_openid_connect-0.2.3/src/simple_openid_connect/flows/authorization_code_flow/client.py
+-rw-r--r--   0        0        0     2208 2023-05-01 11:18:30.258106 simple_openid_connect-0.2.3/src/simple_openid_connect/flows/direct_access_grant/__init__.py
+-rw-r--r--   0        0        0     1583 2023-05-01 11:18:30.258106 simple_openid_connect-0.2.3/src/simple_openid_connect/flows/direct_access_grant/client.py
+-rw-r--r--   0        0        0       53 2022-12-08 12:24:29.349860 simple_openid_connect-0.2.3/src/simple_openid_connect/integrations/__init__.py
+-rw-r--r--   0        0        0       61 2022-12-01 10:05:47.886671 simple_openid_connect-0.2.3/src/simple_openid_connect/integrations/django/__init__.py
+-rw-r--r--   0        0        0     5467 2023-05-01 11:22:04.083382 simple_openid_connect-0.2.3/src/simple_openid_connect/integrations/django/apps.py
+-rw-r--r--   0        0        0     4555 2022-12-01 10:05:47.886671 simple_openid_connect-0.2.3/src/simple_openid_connect/integrations/django/decorators.py
+-rw-r--r--   0        0        0     2630 2023-05-01 11:22:04.076716 simple_openid_connect-0.2.3/src/simple_openid_connect/integrations/django/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2022-12-01 10:05:47.886671 simple_openid_connect-0.2.3/src/simple_openid_connect/integrations/django/migrations/__init__.py
+-rw-r--r--   0        0        0     5728 2022-12-01 11:42:37.006937 simple_openid_connect-0.2.3/src/simple_openid_connect/integrations/django/models.py
+-rw-r--r--   0        0        0      381 2022-12-01 10:05:47.886671 simple_openid_connect-0.2.3/src/simple_openid_connect/integrations/django/templates/simple_openid_connect/login_failed.html
+-rw-r--r--   0        0        0      729 2022-12-08 12:24:29.349860 simple_openid_connect-0.2.3/src/simple_openid_connect/integrations/django/urls.py
+-rw-r--r--   0        0        0     2338 2022-12-01 10:05:47.886671 simple_openid_connect-0.2.3/src/simple_openid_connect/integrations/django/user_mapping.py
+-rw-r--r--   0        0        0     4522 2023-05-25 12:20:30.621017 simple_openid_connect-0.2.3/src/simple_openid_connect/integrations/django/views.py
+-rw-r--r--   0        0        0      306 2022-12-08 12:24:29.353193 simple_openid_connect-0.2.3/src/simple_openid_connect/integrations/djangorestframework/__init__.py
+-rw-r--r--   0        0        0     4648 2022-12-08 12:24:29.353193 simple_openid_connect-0.2.3/src/simple_openid_connect/integrations/djangorestframework/authentication.py
+-rw-r--r--   0        0        0      957 2022-12-08 12:24:29.353193 simple_openid_connect-0.2.3/src/simple_openid_connect/integrations/djangorestframework/drf_spectacular_schema.py
+-rw-r--r--   0        0        0     2531 2022-12-08 12:24:29.353193 simple_openid_connect-0.2.3/src/simple_openid_connect/integrations/djangorestframework/permissions.py
+-rw-r--r--   0        0        0      472 2022-11-16 07:19:49.333600 simple_openid_connect-0.2.3/src/simple_openid_connect/jwk.py
+-rw-r--r--   0        0        0      621 2022-11-16 07:19:49.333600 simple_openid_connect-0.2.3/src/simple_openid_connect/rp_initiated_logout.py
+-rw-r--r--   0        0        0     1509 2022-11-16 07:19:49.333600 simple_openid_connect-0.2.3/src/simple_openid_connect/token_introspection.py
+-rw-r--r--   0        0        0     1566 2022-11-16 07:19:49.333600 simple_openid_connect-0.2.3/src/simple_openid_connect/token_refresh.py
+-rw-r--r--   0        0        0     1393 2022-11-12 19:48:31.467498 simple_openid_connect-0.2.3/src/simple_openid_connect/userinfo.py
+-rw-r--r--   0        0        0      781 2022-11-16 07:19:49.333600 simple_openid_connect-0.2.3/src/simple_openid_connect/utils.py
+-rw-r--r--   0        0        0    16938 2022-12-08 12:24:29.353193 simple_openid_connect-0.2.3/tests/conftest.py
+-rw-r--r--   0        0        0        0 2022-11-16 07:19:49.333600 simple_openid_connect-0.2.3/tests/django_test_project/django_test_project/__init__.py
+-rw-r--r--   0        0        0     2785 2022-12-01 10:05:47.890004 simple_openid_connect-0.2.3/tests/django_test_project/django_test_project/settings.py
+-rw-r--r--   0        0        0     2586 2022-12-08 12:24:29.353193 simple_openid_connect-0.2.3/tests/django_test_project/django_test_project/tests/conftest.py
+-rw-r--r--   0        0        0     1541 2022-12-08 12:24:29.353193 simple_openid_connect-0.2.3/tests/django_test_project/django_test_project/tests/test_access_token_protected_view.py
+-rw-r--r--   0        0        0      633 2022-12-08 12:24:29.353193 simple_openid_connect-0.2.3/tests/django_test_project/django_test_project/tests/test_frontchannel_logout_notifications.py
+-rw-r--r--   0        0        0     5390 2022-12-08 12:24:29.353193 simple_openid_connect-0.2.3/tests/django_test_project/django_test_project/tests/test_login.py
+-rw-r--r--   0        0        0      687 2022-12-08 12:24:29.353193 simple_openid_connect-0.2.3/tests/django_test_project/django_test_project/tests/test_logout.py
+-rw-r--r--   0        0        0     1248 2022-12-01 10:05:47.890004 simple_openid_connect-0.2.3/tests/django_test_project/django_test_project/urls.py
+-rw-r--r--   0        0        0      639 2022-12-01 10:05:47.890004 simple_openid_connect-0.2.3/tests/django_test_project/django_test_project/views.py
+-rw-r--r--   0        0        0      415 2022-11-16 07:19:49.333600 simple_openid_connect-0.2.3/tests/django_test_project/django_test_project/wsgi.py
+-rwxr-xr-x   0        0        0      675 2022-11-16 07:19:49.333600 simple_openid_connect-0.2.3/tests/django_test_project/manage.py
+-rw-r--r--   0        0        0     1746 2022-11-30 13:30:16.836909 simple_openid_connect-0.2.3/tests/interactive_tests/conftest.py
+-rw-r--r--   0        0        0     2001 2022-12-08 12:24:29.353193 simple_openid_connect-0.2.3/tests/interactive_tests/test_google.py
+-rw-r--r--   0        0        0     1668 2022-12-08 12:24:29.366526 simple_openid_connect-0.2.3/tests/test_authorization_code_flow.py
+-rw-r--r--   0        0        0     5139 2023-05-12 10:35:13.267423 simple_openid_connect-0.2.3/tests/test_client.py
+-rw-r--r--   0        0        0      934 2022-12-08 12:24:29.366526 simple_openid_connect-0.2.3/tests/test_client_auth.py
+-rw-r--r--   0        0        0     1378 2023-05-01 11:18:29.554766 simple_openid_connect-0.2.3/tests/test_direct_access_grant.py
+-rw-r--r--   0        0        0     1541 2022-12-08 12:24:29.366526 simple_openid_connect-0.2.3/tests/test_discovery.py
+-rw-r--r--   0        0        0      590 2022-12-08 12:24:29.366526 simple_openid_connect-0.2.3/tests/test_jwk.py
+-rw-r--r--   0        0        0     2274 2022-11-13 10:28:27.455234 simple_openid_connect-0.2.3/tests/test_message_encoding.py
+-rw-r--r--   0        0        0      581 2022-11-12 19:48:31.434164 simple_openid_connect-0.2.3/tests/test_rp_initiated_logout.py
+-rw-r--r--   0        0        0     5760 1970-01-01 00:00:00.000000 simple_openid_connect-0.2.3/PKG-INFO
```

### Comparing `simple_openid_connect-0.2.2/.github/workflows/checks.yml` & `simple_openid_connect-0.2.3/.github/workflows/checks.yml`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.2/.pre-commit-config.yaml` & `simple_openid_connect-0.2.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.2/LICENSE` & `simple_openid_connect-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.2/README.md` & `simple_openid_connect-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.2/docs/Makefile` & `simple_openid_connect-0.2.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.2/docs/conf.py` & `simple_openid_connect-0.2.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.2/docs/django-integration.rst` & `simple_openid_connect-0.2.3/docs/django-integration.rst`

 * *Files 5% similar despite different names*

```diff
@@ -52,18 +52,21 @@
 - ``OPENID_CLIENT_SECRET``
     The client secret that was issued to you from your Openid provider if this is a confidential client.
 
 - ``OPENID_SCOPE``
     The Openid scopes which are requested from the provider when a user logs in.
     It should be a list of scopes as space separated string and should contain the ``openid`` scope.
 
-- ``LOGIN_URL`` (`django docs <LOGIN_URL>`_)
+- ``LOGIN_URL`` (`django docs <https://docs.djangoproject.com/en/dev/ref/settings/#login-url>`_)
     This is recommended to be set to ``simple_openid_connect_django:login`` to serve this libraries login page which handles Openid authentication.
     If additional authentication methods are also used, don't do this.
 
+- ``LOGOUT_REDIRECT_URL`` (`django docs <https://docs.djangoproject.com/en/dev/ref/settings/#logout-redirect-url>`_)
+    This is the url the user is redirected to after logging out. If it is not set, some Openid providers do not redirect the user back to the application.
+
 Usage
 =====
 
 After setup is done, this library is very *hands off*.
 It authenticates users using Openid-Connect, parses retrieved user information, automatically creates or updates user
 objects as required and then authenticates the current session.
 It interoperates with Django's builtin authentication so things like the ``login_required`` decorator can still be used.
```

### Comparing `simple_openid_connect-0.2.2/docs/drf-integration.rst` & `simple_openid_connect-0.2.3/docs/drf-integration.rst`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.2/docs/index.rst` & `simple_openid_connect-0.2.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.2/docs/installation.rst` & `simple_openid_connect-0.2.3/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.2/docs/usage.rst` & `simple_openid_connect-0.2.3/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.2/pyproject.toml` & `simple_openid_connect-0.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.2/src/simple_openid_connect/base_data.py` & `simple_openid_connect-0.2.3/src/simple_openid_connect/base_data.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.2/src/simple_openid_connect/client.py` & `simple_openid_connect-0.2.3/src/simple_openid_connect/client.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.2/src/simple_openid_connect/client_authentication.py` & `simple_openid_connect-0.2.3/src/simple_openid_connect/client_authentication.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.2/src/simple_openid_connect/data.py` & `simple_openid_connect-0.2.3/src/simple_openid_connect/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -621,30 +621,30 @@
 
 
 class RpInitiatedLogoutRequest(OpenidBaseModel):
     """
     Request which a Relying-Party sends to the OP to initiate a user logout
     """
 
-    id_token_hint: Optional[str]
+    id_token_hint: Optional[str] = None
     "RECOMMENDED. ID Token previously issued by the OP to the RP passed to the Logout Endpoint as a hint about the End-User's current authenticated session with the Client. This is used as an indication of the identity of the End-User that the RP is requesting be logged out by the OP. "
 
-    logout_hint: Optional[str]
+    logout_hint: Optional[str] = None
     "OPTIONAL. Hint to the Authorization Server about the End-User that is logging out. The value and meaning of this parameter is left up to the OP's discretion. For instance, the value might contain an email address, phone number, username, or session identifier pertaining to the RP's session with the OP for the End-User."
 
-    client_id: Optional[str]
+    client_id: Optional[str] = None
     "OPTIONAL. Client Identifier valid at the Authorization Server. When both client_id and id_token_hint are present, the id token MUST have been issued to this client. The most common use case for this parameter is to specify the Client Identifier when post_logout_redirect_uri is used but id_token_hint is not. Another use is for symmetrically encrypted ID Tokens used as id_token_hint values that require the Client Identifier to be specified by other means, so that the ID Tokens can be decrypted by the OP. "
 
-    post_logout_redirect_uri: Optional[str]
+    post_logout_redirect_uri: Optional[str] = None
     "OPTIONAL. URI to which the RP is requesting that the End-User's User Agent be redirected after a logout has been performed. This URI SHOULD use the https scheme; however, it MAY use the http scheme, provided that the Client Type is confidential, and provided the OP allows the use of http RP URIs. The URI MAY use an alternate scheme, such as one that is intended to identify a callback into a native application. The value MUST have been previously registered with the OP, either using the post_logout_redirect_uris Registration parameter or via another mechanism. An id_token_hint is also RECOMMENDED when this parameter is included."
 
-    state: Optional[str]
+    state: Optional[str] = None
     "OPTIONAL. Opaque value used by the RP to maintain state between the logout request and the callback to the endpoint specified by the post_logout_redirect_uri parameter. If included in the logout request, the OP passes this value back to the RP using the state parameter when redirecting the User Agent back to the RP."
 
-    ui_locales: Optional[List[str]]
+    ui_locales: Optional[List[str]] = None
     'OPTIONAL. End-User\'s preferred languages and scripts for the user interface, represented as a space-separated list of BCP47 [RFC5646] language tag values, ordered by preference. For instance, the value "fr-CA fr en" represents a preference for French as spoken in Canada, then French (without a region designation), followed by English (without a region designation). An error SHOULD NOT result if some or all of the requested locales are not supported by the OpenID Provider. '
 
 
 class FrontChannelLogoutNotification(OpenidBaseModel):
     """
     A notification which the Relying-Party receives when a user logs out.
```

### Comparing `simple_openid_connect-0.2.2/src/simple_openid_connect/discovery.py` & `simple_openid_connect-0.2.3/src/simple_openid_connect/discovery.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.2/src/simple_openid_connect/exceptions.py` & `simple_openid_connect-0.2.3/src/simple_openid_connect/exceptions.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.2/src/simple_openid_connect/flows/authorization_code_flow/__init__.py` & `simple_openid_connect-0.2.3/src/simple_openid_connect/flows/authorization_code_flow/__init__.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.2/src/simple_openid_connect/flows/authorization_code_flow/client.py` & `simple_openid_connect-0.2.3/src/simple_openid_connect/flows/authorization_code_flow/client.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.2/src/simple_openid_connect/flows/direct_access_grant/__init__.py` & `simple_openid_connect-0.2.3/src/simple_openid_connect/flows/direct_access_grant/__init__.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.2/src/simple_openid_connect/flows/direct_access_grant/client.py` & `simple_openid_connect-0.2.3/src/simple_openid_connect/flows/direct_access_grant/client.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.2/src/simple_openid_connect/integrations/django/apps.py` & `simple_openid_connect-0.2.3/src/simple_openid_connect/integrations/django/apps.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.2/src/simple_openid_connect/integrations/django/decorators.py` & `simple_openid_connect-0.2.3/src/simple_openid_connect/integrations/django/decorators.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.2/src/simple_openid_connect/integrations/django/migrations/0001_initial.py` & `simple_openid_connect-0.2.3/src/simple_openid_connect/integrations/django/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.2/src/simple_openid_connect/integrations/django/models.py` & `simple_openid_connect-0.2.3/src/simple_openid_connect/integrations/django/models.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.2/src/simple_openid_connect/integrations/django/urls.py` & `simple_openid_connect-0.2.3/src/simple_openid_connect/integrations/django/urls.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.2/src/simple_openid_connect/integrations/django/user_mapping.py` & `simple_openid_connect-0.2.3/src/simple_openid_connect/integrations/django/user_mapping.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.2/src/simple_openid_connect/integrations/django/views.py` & `simple_openid_connect-0.2.3/src/simple_openid_connect/integrations/django/views.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from django.utils.decorators import method_decorator
 from django.views import View
 from django.views.decorators.cache import cache_control
 
 from simple_openid_connect.data import (
     FrontChannelLogoutNotification,
     IdToken,
+    RpInitiatedLogoutRequest,
     TokenSuccessResponse,
 )
 from simple_openid_connect.integrations.django.apps import OpenidAppConfig
 from simple_openid_connect.integrations.django.models import OpenidUser
 
 logger = logging.getLogger(__name__)
 
@@ -107,15 +108,23 @@
     """
     The view which handles logging a user out.
     """
 
     def get(self, request: HttpRequest) -> HttpResponse:
         logout(request)
         client = OpenidAppConfig.get_instance().get_client(request)
-        return HttpResponseRedirect(client.initiate_logout())
+
+        if settings.LOGOUT_REDIRECT_URL is not None:
+            logout_request = RpInitiatedLogoutRequest(
+                post_logout_redirect_uri=resolve_url(settings.LOGOUT_REDIRECT_URL),
+            )
+        else:
+            logout_request = None
+
+        return HttpResponseRedirect(client.initiate_logout(logout_request))
 
 
 class FrontChannelLogoutNotificationView(View):
     """
     A view which handles Openid front-channel logout notifications by logging out the current session
     """
```

### Comparing `simple_openid_connect-0.2.2/src/simple_openid_connect/integrations/djangorestframework/authentication.py` & `simple_openid_connect-0.2.3/src/simple_openid_connect/integrations/djangorestframework/authentication.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.2/src/simple_openid_connect/integrations/djangorestframework/drf_spectacular_schema.py` & `simple_openid_connect-0.2.3/src/simple_openid_connect/integrations/djangorestframework/drf_spectacular_schema.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.2/src/simple_openid_connect/integrations/djangorestframework/permissions.py` & `simple_openid_connect-0.2.3/src/simple_openid_connect/integrations/djangorestframework/permissions.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.2/src/simple_openid_connect/rp_initiated_logout.py` & `simple_openid_connect-0.2.3/src/simple_openid_connect/rp_initiated_logout.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.2/src/simple_openid_connect/token_introspection.py` & `simple_openid_connect-0.2.3/src/simple_openid_connect/token_introspection.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.2/src/simple_openid_connect/token_refresh.py` & `simple_openid_connect-0.2.3/src/simple_openid_connect/token_refresh.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.2/src/simple_openid_connect/userinfo.py` & `simple_openid_connect-0.2.3/src/simple_openid_connect/userinfo.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.2/src/simple_openid_connect/utils.py` & `simple_openid_connect-0.2.3/src/simple_openid_connect/utils.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.2/tests/conftest.py` & `simple_openid_connect-0.2.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.2/tests/django_test_project/django_test_project/settings.py` & `simple_openid_connect-0.2.3/tests/django_test_project/django_test_project/settings.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.2/tests/django_test_project/django_test_project/tests/conftest.py` & `simple_openid_connect-0.2.3/tests/django_test_project/django_test_project/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.2/tests/django_test_project/django_test_project/tests/test_access_token_protected_view.py` & `simple_openid_connect-0.2.3/tests/django_test_project/django_test_project/tests/test_access_token_protected_view.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.2/tests/django_test_project/django_test_project/tests/test_frontchannel_logout_notifications.py` & `simple_openid_connect-0.2.3/tests/django_test_project/django_test_project/tests/test_frontchannel_logout_notifications.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.2/tests/django_test_project/django_test_project/tests/test_login.py` & `simple_openid_connect-0.2.3/tests/django_test_project/django_test_project/tests/test_login.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.2/tests/django_test_project/django_test_project/tests/test_logout.py` & `simple_openid_connect-0.2.3/tests/django_test_project/django_test_project/tests/test_logout.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.2/tests/django_test_project/django_test_project/urls.py` & `simple_openid_connect-0.2.3/tests/django_test_project/django_test_project/urls.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.2/tests/django_test_project/django_test_project/views.py` & `simple_openid_connect-0.2.3/tests/django_test_project/django_test_project/views.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.2/tests/django_test_project/manage.py` & `simple_openid_connect-0.2.3/tests/django_test_project/manage.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.2/tests/interactive_tests/conftest.py` & `simple_openid_connect-0.2.3/tests/interactive_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.2/tests/interactive_tests/test_google.py` & `simple_openid_connect-0.2.3/tests/interactive_tests/test_google.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.2/tests/test_authorization_code_flow.py` & `simple_openid_connect-0.2.3/tests/test_authorization_code_flow.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.2/tests/test_client.py` & `simple_openid_connect-0.2.3/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.2/tests/test_client_auth.py` & `simple_openid_connect-0.2.3/tests/test_client_auth.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.2/tests/test_direct_access_grant.py` & `simple_openid_connect-0.2.3/tests/test_direct_access_grant.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.2/tests/test_discovery.py` & `simple_openid_connect-0.2.3/tests/test_discovery.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.2/tests/test_jwk.py` & `simple_openid_connect-0.2.3/tests/test_jwk.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.2/tests/test_message_encoding.py` & `simple_openid_connect-0.2.3/tests/test_message_encoding.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.2/tests/test_rp_initiated_logout.py` & `simple_openid_connect-0.2.3/tests/test_rp_initiated_logout.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.2/PKG-INFO` & `simple_openid_connect-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple_openid_connect
-Version: 0.2.2
+Version: 0.2.3
 Summary: Simple and opinionated OpenID-Connect relying party and resource server implementation
 Author-email: Finn-Thorben Sell <dev@finn-thorben.me>
 Requires-Python: ~=3.9
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Other Environment
```

