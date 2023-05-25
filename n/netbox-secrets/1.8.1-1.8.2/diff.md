# Comparing `tmp/netbox-secrets-1.8.1.tar.gz` & `tmp/netbox-secrets-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox-secrets-1.8.1.tar", last modified: Mon May  8 19:34:27 2023, max compression
+gzip compressed data, was "netbox-secrets-1.8.2.tar", last modified: Thu May 25 16:36:13 2023, max compression
```

## Comparing `netbox-secrets-1.8.1.tar` & `netbox-secrets-1.8.2.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:34:27.942855 netbox-secrets-1.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-05-08 19:34:16.000000 netbox-secrets-1.8.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-08 19:34:16.000000 netbox-secrets-1.8.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-08 19:34:27.942855 netbox-secrets-1.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-05-08 19:34:16.000000 netbox-secrets-1.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:34:27.934855 netbox-secrets-1.8.1/netbox_secrets/
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-05-08 19:34:16.000000 netbox-secrets-1.8.1/netbox_secrets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-05-08 19:34:16.000000 netbox-secrets-1.8.1/netbox_secrets/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:34:27.934855 netbox-secrets-1.8.1/netbox_secrets/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 19:34:16.000000 netbox-secrets-1.8.1/netbox_secrets/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-05-08 19:34:16.000000 netbox-secrets-1.8.1/netbox_secrets/api/nested_serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5078 2023-05-08 19:34:16.000000 netbox-secrets-1.8.1/netbox_secrets/api/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-08 19:34:16.000000 netbox-secrets-1.8.1/netbox_secrets/api/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)    12149 2023-05-08 19:34:16.000000 netbox-secrets-1.8.1/netbox_secrets/api/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-08 19:34:16.000000 netbox-secrets-1.8.1/netbox_secrets/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-08 19:34:16.000000 netbox-secrets-1.8.1/netbox_secrets/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4571 2023-05-08 19:34:16.000000 netbox-secrets-1.8.1/netbox_secrets/filtersets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:34:27.934855 netbox-secrets-1.8.1/netbox_secrets/forms/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-08 19:34:16.000000 netbox-secrets-1.8.1/netbox_secrets/forms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-08 19:34:16.000000 netbox-secrets-1.8.1/netbox_secrets/forms/bulk_edit.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-08 19:34:16.000000 netbox-secrets-1.8.1/netbox_secrets/forms/bulk_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-05-08 19:34:16.000000 netbox-secrets-1.8.1/netbox_secrets/forms/filterset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-05-08 19:34:16.000000 netbox-secrets-1.8.1/netbox_secrets/forms/model_forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:34:27.934855 netbox-secrets-1.8.1/netbox_secrets/graphql/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-08 19:34:16.000000 netbox-secrets-1.8.1/netbox_secrets/graphql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-08 19:34:16.000000 netbox-secrets-1.8.1/netbox_secrets/graphql/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-05-08 19:34:16.000000 netbox-secrets-1.8.1/netbox_secrets/graphql/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-08 19:34:16.000000 netbox-secrets-1.8.1/netbox_secrets/hashers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:34:27.938855 netbox-secrets-1.8.1/netbox_secrets/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     4996 2023-05-08 19:34:16.000000 netbox-secrets-1.8.1/netbox_secrets/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-05-08 19:34:16.000000 netbox-secrets-1.8.1/netbox_secrets/migrations/0002_populate_userkeys.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-05-08 19:34:16.000000 netbox-secrets-1.8.1/netbox_secrets/migrations/0003_populate_secretroles.py
--rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-05-08 19:34:16.000000 netbox-secrets-1.8.1/netbox_secrets/migrations/0004_populate_secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-08 19:34:16.000000 netbox-secrets-1.8.1/netbox_secrets/migrations/0005_alter_secret_custom_field_data_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-08 19:34:16.000000 netbox-secrets-1.8.1/netbox_secrets/migrations/0006_alter_userkey_created_alter_userkey_last_updated.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-05-08 19:34:16.000000 netbox-secrets-1.8.1/netbox_secrets/migrations/0007_secret__object_repr_secret_comments_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 19:34:16.000000 netbox-secrets-1.8.1/netbox_secrets/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:34:27.938855 netbox-secrets-1.8.1/netbox_secrets/models/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-08 19:34:16.000000 netbox-secrets-1.8.1/netbox_secrets/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14680 2023-05-08 19:34:16.000000 netbox-secrets-1.8.1/netbox_secrets/models/secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-08 19:34:16.000000 netbox-secrets-1.8.1/netbox_secrets/navigation.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-08 19:34:16.000000 netbox-secrets-1.8.1/netbox_secrets/querysets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:34:27.930855 netbox-secrets-1.8.1/netbox_secrets/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:34:27.938855 netbox-secrets-1.8.1/netbox_secrets/static/netbox_secrets/
--rw-r--r--   0 runner    (1001) docker     (123)     8341 2023-05-08 19:34:16.000000 netbox-secrets-1.8.1/netbox_secrets/static/netbox_secrets/secrets.js
--rw-r--r--   0 runner    (1001) docker     (123)    29495 2023-05-08 19:34:16.000000 netbox-secrets-1.8.1/netbox_secrets/static/netbox_secrets/secrets.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-05-08 19:34:16.000000 netbox-secrets-1.8.1/netbox_secrets/tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-05-08 19:34:16.000000 netbox-secrets-1.8.1/netbox_secrets/template_content.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:34:27.930855 netbox-secrets-1.8.1/netbox_secrets/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:34:27.938855 netbox-secrets-1.8.1/netbox_secrets/templates/netbox_secrets/
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-08 19:34:16.000000 netbox-secrets-1.8.1/netbox_secrets/templates/netbox_secrets/activate_keys.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:34:27.938855 netbox-secrets-1.8.1/netbox_secrets/templates/netbox_secrets/inc/
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-05-08 19:34:16.000000 netbox-secrets-1.8.1/netbox_secrets/templates/netbox_secrets/inc/private_key_modal.html
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-05-08 19:34:16.000000 netbox-secrets-1.8.1/netbox_secrets/templates/netbox_secrets/inc/secret_actions.html
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-08 19:34:16.000000 netbox-secrets-1.8.1/netbox_secrets/templates/netbox_secrets/inc/secret_add_button.html
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-05-08 19:34:16.000000 netbox-secrets-1.8.1/netbox_secrets/templates/netbox_secrets/inc/secrets_panel.html
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-08 19:34:16.000000 netbox-secrets-1.8.1/netbox_secrets/templates/netbox_secrets/inc/view_tab.html
--rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-05-08 19:34:16.000000 netbox-secrets-1.8.1/netbox_secrets/templates/netbox_secrets/secret.html
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-08 19:34:16.000000 netbox-secrets-1.8.1/netbox_secrets/templates/netbox_secrets/secret_edit.html
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-05-08 19:34:16.000000 netbox-secrets-1.8.1/netbox_secrets/templates/netbox_secrets/secretrole.html
--rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-05-08 19:34:16.000000 netbox-secrets-1.8.1/netbox_secrets/templates/netbox_secrets/userkey.html
--rw-r--r--   0 runner    (1001) docker     (123)     4738 2023-05-08 19:34:16.000000 netbox-secrets-1.8.1/netbox_secrets/templates/netbox_secrets/userkey_edit.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:34:27.938855 netbox-secrets-1.8.1/netbox_secrets/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 19:34:16.000000 netbox-secrets-1.8.1/netbox_secrets/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-05-08 19:34:16.000000 netbox-secrets-1.8.1/netbox_secrets/tests/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    11064 2023-05-08 19:34:16.000000 netbox-secrets-1.8.1/netbox_secrets/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-05-08 19:34:16.000000 netbox-secrets-1.8.1/netbox_secrets/tests/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-08 19:34:16.000000 netbox-secrets-1.8.1/netbox_secrets/tests/test_form.py
--rw-r--r--   0 runner    (1001) docker     (123)     7464 2023-05-08 19:34:16.000000 netbox-secrets-1.8.1/netbox_secrets/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-05-08 19:34:16.000000 netbox-secrets-1.8.1/netbox_secrets/tests/test_views.py
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-05-08 19:34:16.000000 netbox-secrets-1.8.1/netbox_secrets/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:34:27.938855 netbox-secrets-1.8.1/netbox_secrets/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-08 19:34:16.000000 netbox-secrets-1.8.1/netbox_secrets/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-08 19:34:16.000000 netbox-secrets-1.8.1/netbox_secrets/utils/crypto.py
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-08 19:34:16.000000 netbox-secrets-1.8.1/netbox_secrets/utils/hashers.py
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-08 19:34:16.000000 netbox-secrets-1.8.1/netbox_secrets/utils/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    13203 2023-05-08 19:34:16.000000 netbox-secrets-1.8.1/netbox_secrets/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:34:27.934855 netbox-secrets-1.8.1/netbox_secrets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-08 19:34:27.000000 netbox-secrets-1.8.1/netbox_secrets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-05-08 19:34:27.000000 netbox-secrets-1.8.1/netbox_secrets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 19:34:27.000000 netbox-secrets-1.8.1/netbox_secrets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 19:34:27.000000 netbox-secrets-1.8.1/netbox_secrets.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-08 19:34:27.000000 netbox-secrets-1.8.1/netbox_secrets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-08 19:34:27.000000 netbox-secrets-1.8.1/netbox_secrets.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-08 19:34:16.000000 netbox-secrets-1.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 19:34:27.942855 netbox-secrets-1.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-05-08 19:34:16.000000 netbox-secrets-1.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:36:13.880566 netbox-secrets-1.8.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-25 16:36:13.880566 netbox-secrets-1.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:36:13.872565 netbox-secrets-1.8.2/netbox_secrets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:36:13.872565 netbox-secrets-1.8.2/netbox_secrets/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/api/nested_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5078 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/api/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12415 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/api/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4680 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/filtersets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:36:13.876565 netbox-secrets-1.8.2/netbox_secrets/forms/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/forms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/forms/bulk_edit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/forms/bulk_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/forms/filterset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/forms/model_forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:36:13.876565 netbox-secrets-1.8.2/netbox_secrets/graphql/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/graphql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/graphql/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/graphql/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/hashers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:36:13.876565 netbox-secrets-1.8.2/netbox_secrets/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     4996 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/migrations/0002_populate_userkeys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/migrations/0003_populate_secretroles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/migrations/0004_populate_secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/migrations/0005_alter_secret_custom_field_data_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/migrations/0006_alter_userkey_created_alter_userkey_last_updated.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/migrations/0007_secret__object_repr_secret_comments_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:36:13.876565 netbox-secrets-1.8.2/netbox_secrets/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14680 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/models/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/navigation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/querysets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:36:13.872565 netbox-secrets-1.8.2/netbox_secrets/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:36:13.876565 netbox-secrets-1.8.2/netbox_secrets/static/netbox_secrets/
+-rw-r--r--   0 runner    (1001) docker     (123)     8341 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/static/netbox_secrets/secrets.js
+-rw-r--r--   0 runner    (1001) docker     (123)    29495 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/static/netbox_secrets/secrets.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/template_content.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:36:13.872565 netbox-secrets-1.8.2/netbox_secrets/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:36:13.876565 netbox-secrets-1.8.2/netbox_secrets/templates/netbox_secrets/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/templates/netbox_secrets/activate_keys.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:36:13.876565 netbox-secrets-1.8.2/netbox_secrets/templates/netbox_secrets/inc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/templates/netbox_secrets/inc/private_key_modal.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/templates/netbox_secrets/inc/secret_actions.html
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/templates/netbox_secrets/inc/secret_add_button.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/templates/netbox_secrets/inc/secrets_panel.html
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/templates/netbox_secrets/inc/view_tab.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/templates/netbox_secrets/secret.html
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/templates/netbox_secrets/secret_edit.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/templates/netbox_secrets/secretrole.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/templates/netbox_secrets/userkey.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4738 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/templates/netbox_secrets/userkey_edit.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:36:13.880566 netbox-secrets-1.8.2/netbox_secrets/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/tests/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11064 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/tests/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/tests/test_form.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7464 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/tests/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:36:13.880566 netbox-secrets-1.8.2/netbox_secrets/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/utils/crypto.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/utils/hashers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/utils/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13567 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/netbox_secrets/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:36:13.872565 netbox-secrets-1.8.2/netbox_secrets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-25 16:36:13.000000 netbox-secrets-1.8.2/netbox_secrets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-05-25 16:36:13.000000 netbox-secrets-1.8.2/netbox_secrets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 16:36:13.000000 netbox-secrets-1.8.2/netbox_secrets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 16:36:13.000000 netbox-secrets-1.8.2/netbox_secrets.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-25 16:36:13.000000 netbox-secrets-1.8.2/netbox_secrets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-25 16:36:13.000000 netbox-secrets-1.8.2/netbox_secrets.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 16:36:13.880566 netbox-secrets-1.8.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-05-25 16:36:02.000000 netbox-secrets-1.8.2/setup.py
```

### Comparing `netbox-secrets-1.8.1/LICENSE.md` & `netbox-secrets-1.8.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.1/README.md` & `netbox-secrets-1.8.2/README.md`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.1/netbox_secrets/__init__.py` & `netbox-secrets-1.8.2/netbox_secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.1/netbox_secrets/admin.py` & `netbox-secrets-1.8.2/netbox_secrets/admin.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.1/netbox_secrets/api/nested_serializers.py` & `netbox-secrets-1.8.2/netbox_secrets/api/nested_serializers.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.1/netbox_secrets/api/serializers.py` & `netbox-secrets-1.8.2/netbox_secrets/api/serializers.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.1/netbox_secrets/api/urls.py` & `netbox-secrets-1.8.2/netbox_secrets/api/urls.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.1/netbox_secrets/api/views.py` & `netbox-secrets-1.8.2/netbox_secrets/api/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import base64
 
 from Crypto.PublicKey import RSA
 from django.conf import settings
 from django.http import HttpResponseBadRequest
 from drf_spectacular import utils as drf_utils
-from netbox.api.viewsets import BaseViewSet, NetBoxModelViewSet, mixins
 from rest_framework import mixins as drf_mixins
 from rest_framework.exceptions import ValidationError
 from rest_framework.parsers import FormParser, JSONParser, MultiPartParser
 from rest_framework.permissions import IsAuthenticated
 from rest_framework.response import Response
 from rest_framework.routers import APIRootView
 from rest_framework.viewsets import ModelViewSet, ViewSet
-from utilities.utils import count_related
 
-from .. import constants, exceptions, filtersets, models
+from netbox.api.viewsets import BaseViewSet, mixins, NetBoxModelViewSet
+from utilities.utils import count_related
 from . import serializers
+from .. import constants, exceptions, filtersets, models
 
 plugin_settings = settings.PLUGINS_CONFIG.get('netbox_secrets', {})
 public_key_size = plugin_settings.get('public_key_size')
 
 ERR_USERKEY_MISSING = "No UserKey found for the current user."
 ERR_USERKEY_INACTIVE = "UserKey has not been activated for decryption."
 ERR_PRIVKEY_MISSING = "Private key was not provided."
@@ -39,15 +39,15 @@
 # User Key
 #
 class UserKeyViewSet(ModelViewSet):
     queryset = models.UserKey.objects.all()
     serializer_class = serializers.UserKeySerializer
 
     def get_queryset(self):
-        return models.UserKey.objects.filter(user=self.request.user)
+        return super().get_queryset().filter(user=self.request.user)
 
 
 #
 # Secret Roles
 #
 
 
@@ -145,21 +145,27 @@
 #
 class SessionKeyViewSet(
     drf_mixins.ListModelMixin,
     drf_mixins.RetrieveModelMixin,
     drf_mixins.DestroyModelMixin,
     mixins.BriefModeMixin,
     mixins.BulkDestroyModelMixin,
+    mixins.ObjectValidationMixin,
     BaseViewSet,
 ):
     queryset = models.SessionKey.objects.prefetch_related('userkey__user')
     serializer_class = serializers.SessionKeySerializer
 
     def get_queryset(self):
-        return models.SessionKey.objects.filter(userkey__user=self.request.user)
+        if self.request.user.is_authenticated:
+            # Overrides self.queryset to always return the restricted key filtered by the request.user
+            self.queryset = super().get_queryset().filter(userkey__user=self.request.user)
+            return self.queryset
+
+        return super().get_queryset()
 
     @drf_utils.extend_schema(
         request=serializers.SessionKeyCreateSerializer,
         responses={
             201: drf_utils.OpenApiResponse(
                 description="Session key created successfully.",
                 response=serializers.SessionKeySerializer,
```

### Comparing `netbox-secrets-1.8.1/netbox_secrets/filtersets.py` & `netbox-secrets-1.8.2/netbox_secrets/filtersets.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import django_filters
 from django.conf import settings
 from django.contrib.contenttypes.models import ContentType
 from django.db.models import Q
 from django.utils.translation import gettext as _
+
 from netbox.filtersets import NetBoxModelFilterSet
 from tenancy.models import Contact
-from utilities.filters import MultiValueCharFilter
-
+from utilities.filters import ContentTypeFilter, MultiValueCharFilter
 from .constants import SECRET_ASSIGNABLE_MODELS
 from .models import Secret, SecretRole
 
 __all__ = [
     'SecretFilterSet',
     'SecretRoleFilterSet',
 ]
@@ -57,30 +57,32 @@
         role = django_filters.ModelMultipleChoiceFilter(
             field_name='role__slug',
             queryset=SecretRole.objects.all(),
             to_field_name='slug',
             label='Role (slug)',
         )
 
+        assigned_object_type = ContentTypeFilter()
+
         assigned_object_type_id = django_filters.ModelMultipleChoiceFilter(
-            field_name='assigned_object_type',
             queryset=ContentType.objects.filter(SECRET_ASSIGNABLE_MODELS),
             label='Object type (ID)',
         )
 
         contact = django_filters.ModelMultipleChoiceFilter(
             field_name='contacts__contact',
             queryset=Contact.objects.all(),
             label=_('Contact'),
         )
 
         class Meta:
             model = Secret
             fields = [
                 'id',
+                'assigned_object_type',
                 'assigned_object_type_id',
                 'assigned_object_id',
                 'role_id',
                 'role',
                 'name',
                 'contact',
                 'description',
@@ -115,24 +117,26 @@
         role = django_filters.ModelMultipleChoiceFilter(
             field_name='role__slug',
             queryset=SecretRole.objects.all(),
             to_field_name='slug',
             label='Role (slug)',
         )
 
+        assigned_object_type = ContentTypeFilter()
+
         assigned_object_type_id = django_filters.ModelMultipleChoiceFilter(
-            field_name='assigned_object_type',
             queryset=ContentType.objects.filter(SECRET_ASSIGNABLE_MODELS),
             label='Object type (ID)',
         )
 
         class Meta:
             model = Secret
             fields = [
                 'id',
+                'assigned_object_type',
                 'assigned_object_type_id',
                 'assigned_object_id',
                 'role_id',
                 'role',
                 'name',
                 '_object_repr',
                 'description',
```

### Comparing `netbox-secrets-1.8.1/netbox_secrets/forms/bulk_edit.py` & `netbox-secrets-1.8.2/netbox_secrets/forms/bulk_edit.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.1/netbox_secrets/forms/filterset.py` & `netbox-secrets-1.8.2/netbox_secrets/forms/filterset.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.1/netbox_secrets/forms/model_forms.py` & `netbox-secrets-1.8.2/netbox_secrets/forms/model_forms.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.1/netbox_secrets/graphql/types.py` & `netbox-secrets-1.8.2/netbox_secrets/graphql/types.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.1/netbox_secrets/migrations/0001_initial.py` & `netbox-secrets-1.8.2/netbox_secrets/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.1/netbox_secrets/migrations/0002_populate_userkeys.py` & `netbox-secrets-1.8.2/netbox_secrets/migrations/0002_populate_userkeys.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.1/netbox_secrets/migrations/0003_populate_secretroles.py` & `netbox-secrets-1.8.2/netbox_secrets/migrations/0003_populate_secretroles.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.1/netbox_secrets/migrations/0004_populate_secrets.py` & `netbox-secrets-1.8.2/netbox_secrets/migrations/0004_populate_secrets.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.1/netbox_secrets/migrations/0005_alter_secret_custom_field_data_and_more.py` & `netbox-secrets-1.8.2/netbox_secrets/migrations/0005_alter_secret_custom_field_data_and_more.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.1/netbox_secrets/migrations/0006_alter_userkey_created_alter_userkey_last_updated.py` & `netbox-secrets-1.8.2/netbox_secrets/migrations/0006_alter_userkey_created_alter_userkey_last_updated.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.1/netbox_secrets/migrations/0007_secret__object_repr_secret_comments_and_more.py` & `netbox-secrets-1.8.2/netbox_secrets/migrations/0007_secret__object_repr_secret_comments_and_more.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.1/netbox_secrets/models/secrets.py` & `netbox-secrets-1.8.2/netbox_secrets/models/secrets.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.1/netbox_secrets/navigation.py` & `netbox-secrets-1.8.2/netbox_secrets/navigation.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.1/netbox_secrets/static/netbox_secrets/secrets.js` & `netbox-secrets-1.8.2/netbox_secrets/static/netbox_secrets/secrets.js`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.1/netbox_secrets/static/netbox_secrets/secrets.js.map` & `netbox-secrets-1.8.2/netbox_secrets/static/netbox_secrets/secrets.js.map`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.1/netbox_secrets/tables.py` & `netbox-secrets-1.8.2/netbox_secrets/tables.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.1/netbox_secrets/template_content.py` & `netbox-secrets-1.8.2/netbox_secrets/template_content.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.1/netbox_secrets/templates/netbox_secrets/inc/private_key_modal.html` & `netbox-secrets-1.8.2/netbox_secrets/templates/netbox_secrets/inc/private_key_modal.html`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.1/netbox_secrets/templates/netbox_secrets/inc/secret_actions.html` & `netbox-secrets-1.8.2/netbox_secrets/templates/netbox_secrets/inc/secret_actions.html`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.1/netbox_secrets/templates/netbox_secrets/inc/secrets_panel.html` & `netbox-secrets-1.8.2/netbox_secrets/templates/netbox_secrets/inc/secrets_panel.html`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.1/netbox_secrets/templates/netbox_secrets/inc/view_tab.html` & `netbox-secrets-1.8.2/netbox_secrets/templates/netbox_secrets/inc/view_tab.html`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.1/netbox_secrets/templates/netbox_secrets/secret.html` & `netbox-secrets-1.8.2/netbox_secrets/templates/netbox_secrets/secret.html`

 * *Files 3% similar despite different names*

```diff
@@ -68,17 +68,14 @@
               {% include 'netbox_secrets/inc/secret_actions.html' %}
             </div>
           </div>
         </div>
       </div>
       {% include 'inc/panels/tags.html' %}
       {% include 'inc/panels/comments.html' %}
-      {% if object.enable_contacts %}
-        {% include 'inc/panels/contacts.html' %}
-      {% endif %}
       {% plugin_right_page object %}
     </div>
   </div>
   <div class="row">
     <div class="col col-md-12">
       {% plugin_full_width_page object %}
     </div>
```

#### html2text {}

```diff
@@ -13,11 +13,10 @@
 {% include 'inc/panels/custom_fields.html' %} {% plugin_left_page object %}
 ** Secret Data **
 {% csrf_token %}
 Secret
 ********
 {% include 'netbox_secrets/inc/secret_actions.html' %}
 {% include 'inc/panels/tags.html' %} {% include 'inc/panels/comments.html' %}
-{% if object.enable_contacts %} {% include 'inc/panels/contacts.html' %} {%
-endif %} {% plugin_right_page object %}
+{% plugin_right_page object %}
 {% plugin_full_width_page object %}
 {% include 'netbox_secrets/inc/private_key_modal.html' %} {% endblock %}
```

### Comparing `netbox-secrets-1.8.1/netbox_secrets/templates/netbox_secrets/secret_edit.html` & `netbox-secrets-1.8.2/netbox_secrets/templates/netbox_secrets/secret_edit.html`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.1/netbox_secrets/templates/netbox_secrets/secretrole.html` & `netbox-secrets-1.8.2/netbox_secrets/templates/netbox_secrets/secretrole.html`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.1/netbox_secrets/templates/netbox_secrets/userkey.html` & `netbox-secrets-1.8.2/netbox_secrets/templates/netbox_secrets/userkey.html`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.1/netbox_secrets/templates/netbox_secrets/userkey_edit.html` & `netbox-secrets-1.8.2/netbox_secrets/templates/netbox_secrets/userkey_edit.html`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.1/netbox_secrets/tests/constants.py` & `netbox-secrets-1.8.2/netbox_secrets/tests/constants.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.1/netbox_secrets/tests/test_api.py` & `netbox-secrets-1.8.2/netbox_secrets/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.1/netbox_secrets/tests/test_filters.py` & `netbox-secrets-1.8.2/netbox_secrets/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.1/netbox_secrets/tests/test_form.py` & `netbox-secrets-1.8.2/netbox_secrets/tests/test_form.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.1/netbox_secrets/tests/test_models.py` & `netbox-secrets-1.8.2/netbox_secrets/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.1/netbox_secrets/tests/test_views.py` & `netbox-secrets-1.8.2/netbox_secrets/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.1/netbox_secrets/urls.py` & `netbox-secrets-1.8.2/netbox_secrets/urls.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.1/netbox_secrets/utils/crypto.py` & `netbox-secrets-1.8.2/netbox_secrets/utils/crypto.py`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.1/netbox_secrets/views.py` & `netbox-secrets-1.8.2/netbox_secrets/views.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 import logging
 
+from django.conf import settings
 from django.contrib import messages
 from django.contrib.auth.mixins import LoginRequiredMixin
 from django.contrib.contenttypes.models import ContentType
 from django.db import transaction
 from django.shortcuts import get_object_or_404, redirect, render
 from django.utils.html import escape
 from django.utils.safestring import mark_safe
 from django.utils.translation import gettext as _
 from django.views.generic.base import View
 from extras.signals import clear_webhooks
 from netbox.views import generic
+from tenancy.views import ObjectContactsView
 from utilities.exceptions import AbortRequest, PermissionsViolation
 from utilities.forms import restrict_form_fields
 from utilities.utils import count_related, prepare_cloned_fields
 from utilities.views import GetReturnURLMixin, ViewTab, register_model_view
 
 from . import constants, exceptions, filtersets, forms, models, tables, utils
 
+plugin_settings = settings.PLUGINS_CONFIG.get('netbox_secrets')
+
 #
 # Mixins
 #
 
 
 class ObjectChildrenViewMixin(generic.ObjectChildrenView):
     def get_extra_context(self, request, instance):
@@ -278,14 +282,20 @@
 
 class SecretBulkDeleteView(generic.BulkDeleteView):
     queryset = models.Secret.objects.prefetch_related('role', 'tags')
     filterset = filtersets.SecretFilterSet
     table = tables.SecretTable
 
 
+if plugin_settings.get('enable_contacts'):
+    @register_model_view(models.Secret, 'contacts')
+    class SecretContactsView(ObjectContactsView):
+        queryset = models.Secret.objects.prefetch_related('role', 'tags')
+
+
 class UserKeyView(LoginRequiredMixin, View):
     template_name = 'netbox_secrets/userkey.html'
 
     def get(self, request):
         try:
             userkey = models.UserKey.objects.get(user=request.user)
         except models.UserKey.DoesNotExist:
```

### Comparing `netbox-secrets-1.8.1/netbox_secrets.egg-info/SOURCES.txt` & `netbox-secrets-1.8.2/netbox_secrets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `netbox-secrets-1.8.1/setup.py` & `netbox-secrets-1.8.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='netbox-secrets',
-    version='1.8.1',
+    version='1.8.2',
     description='Netbox Secrets',
     long_description='A Secret store for NetBox',
     url='https://github.com/Onemind-Services-LLC/netbox-secrets/',
     author='Daniel Sheppard',
     author_email='dans@dansheps.com',
     license='Apache 2.0',
     install_requires=[
```

