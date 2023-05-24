# Comparing `tmp/sloth-framework-0.1.5.tar.gz` & `tmp/sloth-framework-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sloth-framework-0.1.5.tar", last modified: Mon May 15 21:57:26 2023, max compression
+gzip compressed data, was "sloth-framework-0.1.6.tar", last modified: Wed May 24 23:12:28 2023, max compression
```

## Comparing `sloth-framework-0.1.5.tar` & `sloth-framework-0.1.6.tar`

### file list

```diff
@@ -1,299 +1,311 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.364170 sloth-framework-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-15 21:57:26.364170 sloth-framework-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 21:57:26.364170 sloth-framework-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.336169 sloth-framework-0.1.5/sloth/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6095 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.336169 sloth-framework-0.1.5/sloth/actions/
--rw-r--r--   0 runner    (1001) docker     (123)    39352 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/actions/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/actions/inputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.340170 sloth-framework-0.1.5/sloth/api/
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18627 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/actions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.340170 sloth-framework-0.1.5/sloth/api/backends/
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16195 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/dashboard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.340170 sloth-framework-0.1.5/sloth/api/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/exceptions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.340170 sloth-framework-0.1.5/sloth/api/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.340170 sloth-framework-0.1.5/sloth/api/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/management/commands/cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/management/commands/query.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/management/commands/reset_passwords.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/management/commands/selenium.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/management/commands/send_web_push_notification.py
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/management/commands/startserver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/management/commands/sync.py
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/management/commands/sync_roles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.340170 sloth-framework-0.1.5/sloth/api/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/migrations/0002_role_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/migrations/0003_alter_application_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/migrations/0004_task.py
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/migrations/0005_task_stopped_alter_task_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/migrations/0006_role_active_alter_role_name_alter_role_scope_key_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/migrations/0007_alter_scope_description_alter_task_error.py
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/migrations/0008_alter_application_available_scopes_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/migrations/0009_pushnotification.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/migrations/0010_alter_pushnotification_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/migrations/0011_alter_application_client_secret.py
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/migrations/0012_authcode.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/migrations/0013_task_partial_task_total.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/migrations/0014_email.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11023 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.336169 sloth-framework-0.1.5/sloth/api/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.344169 sloth-framework-0.1.5/sloth/api/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)    58578 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/css/all.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    67289 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/css/bootstrap-icons.css
--rw-r--r--   0 runner    (1001) docker     (123)   155845 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/css/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/css/colorpick.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.344169 sloth-framework-0.1.5/sloth/api/static/css/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)   107280 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/css/fonts/Eina02-Bold.f8011405.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   116316 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/css/fonts/Eina02-Regular.2e682693.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   112880 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/css/fonts/Eina02-SemiBold.c5f9b8e3.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   111976 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/css/fonts/bootstrap-icons.woff
--rw-r--r--   0 runner    (1001) docker     (123)    83304 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/css/fonts/bootstrap-icons.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    30702 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/css/icons.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.344169 sloth-framework-0.1.5/sloth/api/static/css/images/
--rw-r--r--   0 runner    (1001) docker     (123)     6992 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/css/images/ui-icons_444444_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)     6988 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/css/images/ui-icons_555555_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)    35973 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/css/jquery-ui.css
--rw-r--r--   0 runner    (1001) docker     (123)    14670 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/css/leaflet.css
--rw-r--r--   0 runner    (1001) docker     (123)    16264 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/css/select2.min.css
--rw-r--r--   0 runner    (1001) docker     (123)     9009 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/css/sloth.css
--rw-r--r--   0 runner    (1001) docker     (123)    17867 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/css/trumbowyg.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.336169 sloth-framework-0.1.5/sloth/api/static/icons/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.344169 sloth-framework-0.1.5/sloth/api/static/icons/fontawesome/
--rw-r--r--   0 runner    (1001) docker     (123)   100170 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/icons/fontawesome/fontawesome.min.css
--rw-r--r--   0 runner    (1001) docker     (123)  1726692 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/icons/fontawesome/fontawesome.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.348169 sloth-framework-0.1.5/sloth/api/static/icons/fontawesome/webfonts/
--rw-r--r--   0 runner    (1001) docker     (123)   181852 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/icons/fontawesome/webfonts/fa-brands-400.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   105536 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/icons/fontawesome/webfonts/fa-brands-400.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    60520 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/icons/fontawesome/webfonts/fa-regular-400.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    23940 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/icons/fontawesome/webfonts/fa-regular-400.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    10556 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/icons/fontawesome/webfonts/fa-v4compatibility.ttf
--rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/icons/fontawesome/webfonts/fa-v4compatibility.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.348169 sloth-framework-0.1.5/sloth/api/static/icons/materialicons/
--rw-r--r--   0 runner    (1001) docker     (123)   174176 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/icons/materialicons/LDItaoyNOAY6Uewc665JcIzCKsKc_M9flwmPq_HTTw.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   127220 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/icons/materialicons/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   155604 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/icons/materialicons/gok-H7zzDkdnRel8-DQ6KAXJ69wP1tGnf4ZGhUcel5euIg.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/icons/materialicons/materialicons.css
--rw-r--r--   0 runner    (1001) docker     (123)   135988 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/icons/materialicons/oPWQ_lt5nv4pWNJpghLP75WiFR4kLh3kvmvRImcycg.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.348169 sloth-framework-0.1.5/sloth/api/static/images/
--rw-r--r--   0 runner    (1001) docker     (123)    57420 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/images/click.png
--rw-r--r--   0 runner    (1001) docker     (123)    55448 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/images/hand.png
--rw-r--r--   0 runner    (1001) docker     (123)    10276 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/images/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/images/icon.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.348169 sloth-framework-0.1.5/sloth/api/static/images/images/
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/images/images/badge.png
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/images/images/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)    45136 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/images/login.jpeg
--rw-r--r--   0 runner    (1001) docker     (123)    22817 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/images/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/images/logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)    21495 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/images/no-image.png
--rw-r--r--   0 runner    (1001) docker     (123)    23102 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/images/sloth.png
--rw-r--r--   0 runner    (1001) docker     (123)    13670 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/images/user.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.352170 sloth-framework-0.1.5/sloth/api/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/js/api.js
--rw-r--r--   0 runner    (1001) docker     (123)    78743 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/js/bootstrap.bundle.min.js
--rwxr-xr-x   0 runner    (1001) docker     (123)     4098 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/js/colorpick.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.352170 sloth-framework-0.1.5/sloth/api/static/js/i18n/
--rwxr-xr-x   0 runner    (1001) docker     (123)      853 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/js/i18n/pt-BR.js
--rw-r--r--   0 runner    (1001) docker     (123)    89501 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/js/jquery-3.6.0.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   520714 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/js/jquery-ui.js
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/js/jquery.binarytransport.js
--rw-r--r--   0 runner    (1001) docker     (123)     8327 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/js/jquery.mask.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    80794 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/js/jquery.timepicker.js
--rw-r--r--   0 runner    (1001) docker     (123)   147555 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/js/leaflet.js
--rw-r--r--   0 runner    (1001) docker     (123)    24103 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/js/masonry.pkgd.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    18453 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/js/popper.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    43994 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/js/qr-scanner-worker.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    15538 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/js/qr-scanner.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    19927 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/js/qrcode.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    73163 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/js/select2.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    16580 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/js/sloth.js
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/js/sw.js
--rw-r--r--   0 runner    (1001) docker     (123)    10852 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/js/tests.js
--rw-r--r--   0 runner    (1001) docker     (123)    28280 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/js/trumbowyg.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/js/wpn.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.352170 sloth-framework-0.1.5/sloth/api/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/tasks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.336169 sloth-framework-0.1.5/sloth/api/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.352170 sloth-framework-0.1.5/sloth/api/templates/actions/
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/actions/execute_query.html
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/actions/execute_script.html
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/actions/show_icons.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.352170 sloth-framework-0.1.5/sloth/api/templates/api/
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/api/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.352170 sloth-framework-0.1.5/sloth/api/templates/charts/
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/charts/bar.html
--rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/charts/column.html
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/charts/donut.html
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/charts/legend.html
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/charts/pie.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.356170 sloth-framework-0.1.5/sloth/api/templates/dashboard/
--rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/dashboard/actions.html
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/dashboard/apps.html
--rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/dashboard/base.html
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/dashboard/bottom.html
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/dashboard/cards.html
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/dashboard/dashboards.html
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/dashboard/default.html
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/dashboard/footer.html
--rw-r--r--   0 runner    (1001) docker     (123)     7123 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/dashboard/form.html
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/dashboard/grids.html
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/dashboard/header.html
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/dashboard/links.html
--rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/dashboard/menu.html
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/dashboard/messages.html
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/dashboard/modal.html
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/dashboard/plus.html
--rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/dashboard/report.html
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/dashboard/search.html
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/dashboard/settings.html
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/dashboard/shortcuts.html
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/dashboard/tasks.html
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/dashboard/tools.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.356170 sloth-framework-0.1.5/sloth/api/templates/inputs/
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/inputs/picker.html
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/inputs/qrcode.html
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/inputs/select.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.356170 sloth-framework-0.1.5/sloth/api/templates/queryset/
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/queryset/accordion.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.356170 sloth-framework-0.1.5/sloth/api/templates/queryset/actions/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/queryset/actions/actions.html
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/queryset/actions/batch.html
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/queryset/actions/global.html
--rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/queryset/calendar.html
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/queryset/cards.html
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/queryset/checkbox.html
--rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/queryset/datatable.html
--rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/queryset/filter.html
--rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/queryset/filters.html
--rw-r--r--   0 runner    (1001) docker     (123)    11362 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/queryset/queryset.html
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/queryset/rows.html
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/queryset/scroll.html
--rw-r--r--   0 runner    (1001) docker     (123)     6364 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/queryset/statistics.html
--rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/queryset/timeline.html
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/queryset/tree.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.336169 sloth-framework-0.1.5/sloth/api/templates/renderers/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.356170 sloth-framework-0.1.5/sloth/api/templates/renderers/badges/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/renderers/badges/badge.html
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/renderers/badges/boolean.html
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/renderers/badges/danger.html
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/renderers/badges/primary.html
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/renderers/badges/status.html
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/renderers/badges/warning.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.356170 sloth-framework-0.1.5/sloth/api/templates/renderers/boolean/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/renderers/boolean/thumb.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.356170 sloth-framework-0.1.5/sloth/api/templates/renderers/calendar/
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/renderers/calendar/calendar.html
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/renderers/calendar/events.html
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/renderers/calendar/legend.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.356170 sloth-framework-0.1.5/sloth/api/templates/renderers/documents/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/renderers/documents/document.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.356170 sloth-framework-0.1.5/sloth/api/templates/renderers/images/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/renderers/images/banner.html
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/renderers/images/group.html
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/renderers/images/image.html
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/renderers/images/round.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.356170 sloth-framework-0.1.5/sloth/api/templates/renderers/links/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/renderers/links/file.html
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/renderers/links/url.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.356170 sloth-framework-0.1.5/sloth/api/templates/renderers/maps/
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/renderers/maps/geolocation.html
--rw-r--r--   0 runner    (1001) docker     (123)     4551 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/renderers/maps/map.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.360170 sloth-framework-0.1.5/sloth/api/templates/renderers/messages/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/renderers/messages/custom.html
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/renderers/messages/danger.html
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/renderers/messages/message.html
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/renderers/messages/primary.html
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/renderers/messages/success.html
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/renderers/messages/warning.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.360170 sloth-framework-0.1.5/sloth/api/templates/renderers/photos/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/renderers/photos/photo.html
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/renderers/photos/round.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.360170 sloth-framework-0.1.5/sloth/api/templates/renderers/programing/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/renderers/programing/strtable.html
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/renderers/programing/terminal.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.360170 sloth-framework-0.1.5/sloth/api/templates/renderers/progress/
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/renderers/progress/primary.html
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/renderers/progress/success.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.360170 sloth-framework-0.1.5/sloth/api/templates/renderers/tags/
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/renderers/tags/primary.html
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/renderers/tags/tags.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.360170 sloth-framework-0.1.5/sloth/api/templates/renderers/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/renderers/utils/formatted.html
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/renderers/utils/progress.html
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/renderers/utils/qrcode.html
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/renderers/utils/steps.html
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/renderers/utils/table.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.360170 sloth-framework-0.1.5/sloth/api/templates/themes/
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/themes/dark.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.360170 sloth-framework-0.1.5/sloth/api/templates/valueset/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/valueset/2-column.html
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/valueset/field.html
--rw-r--r--   0 runner    (1001) docker     (123)     3576 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/valueset/fieldset-group.html
--rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/valueset/fieldset-list.html
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/valueset/fieldset-tab.html
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/valueset/fieldset.html
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/valueset/primitive.html
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/valueset/value.html
--rw-r--r--   0 runner    (1001) docker     (123)     6265 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/valueset/valueset.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.360170 sloth-framework-0.1.5/sloth/api/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9090 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templatetags/tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)    11965 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.360170 sloth-framework-0.1.5/sloth/cloud/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/cloud/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      688 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/cloud/printer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6116 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/cloud/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.360170 sloth-framework-0.1.5/sloth/conf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/conf/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.360170 sloth-framework-0.1.5/sloth/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21661 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/core/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    42845 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/core/queryset.py
--rw-r--r--   0 runner    (1001) docker     (123)    11540 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/core/statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/core/validation.py
--rw-r--r--   0 runner    (1001) docker     (123)    20797 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/core/valueset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.360170 sloth-framework-0.1.5/sloth/db/
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/db/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.360170 sloth-framework-0.1.5/sloth/db/models/
--rw-r--r--   0 runner    (1001) docker     (123)    12155 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/db/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.360170 sloth-framework-0.1.5/sloth/test/
--rw-r--r--   0 runner    (1001) docker     (123)     3185 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.360170 sloth-framework-0.1.5/sloth/test/selenium/
--rw-r--r--   0 runner    (1001) docker     (123)     4566 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/test/selenium/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10656 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/test/selenium/browser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.360170 sloth-framework-0.1.5/sloth/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.360170 sloth-framework-0.1.5/sloth/utils/formatter/
--rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/utils/formatter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.360170 sloth-framework-0.1.5/sloth/utils/http/
--rw-r--r--   0 runner    (1001) docker     (123)     5317 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/utils/http/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.364170 sloth-framework-0.1.5/sloth/utils/icons/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/utils/icons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28753 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/utils/icons/bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)    53105 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/utils/icons/fontawesome.py
--rw-r--r--   0 runner    (1001) docker     (123)    20959 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/utils/icons/materialicons.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.364170 sloth-framework-0.1.5/sloth/utils/log/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/utils/log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/utils/log/sql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.364170 sloth-framework-0.1.5/sloth_framework.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-15 21:57:26.000000 sloth-framework-0.1.5/sloth_framework.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9734 2023-05-15 21:57:26.000000 sloth-framework-0.1.5/sloth_framework.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 21:57:26.000000 sloth-framework-0.1.5/sloth_framework.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-15 21:57:26.000000 sloth-framework-0.1.5/sloth_framework.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-15 21:57:26.000000 sloth-framework-0.1.5/sloth_framework.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.821168 sloth-framework-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-24 23:12:28.821168 sloth-framework-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 23:12:28.821168 sloth-framework-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.785169 sloth-framework-0.1.6/sloth/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6095 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.785169 sloth-framework-0.1.6/sloth/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)    40271 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/actions/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/actions/inputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.785169 sloth-framework-0.1.6/sloth/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20587 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/actions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.785169 sloth-framework-0.1.6/sloth/api/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16718 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/dashboard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.785169 sloth-framework-0.1.6/sloth/api/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/exceptions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.785169 sloth-framework-0.1.6/sloth/api/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.785169 sloth-framework-0.1.6/sloth/api/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/management/commands/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/management/commands/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/management/commands/reset_passwords.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/management/commands/selenium.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/management/commands/send_web_push_notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/management/commands/startserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/management/commands/sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/management/commands/sync_roles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.789168 sloth-framework-0.1.6/sloth/api/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/migrations/0002_role_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/migrations/0003_alter_application_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/migrations/0004_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/migrations/0005_task_stopped_alter_task_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/migrations/0006_role_active_alter_role_name_alter_role_scope_key_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/migrations/0007_alter_scope_description_alter_task_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/migrations/0008_alter_application_available_scopes_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/migrations/0009_pushnotification.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/migrations/0010_alter_pushnotification_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/migrations/0011_alter_application_client_secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/migrations/0012_authcode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/migrations/0013_task_partial_task_total.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/migrations/0014_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11090 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.781169 sloth-framework-0.1.6/sloth/api/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.789168 sloth-framework-0.1.6/sloth/api/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)    58578 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/css/all.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    67289 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/css/bootstrap-icons.css
+-rw-r--r--   0 runner    (1001) docker     (123)   155845 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/css/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    33038 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/css/bpmn.css
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/css/colorpick.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.789168 sloth-framework-0.1.6/sloth/api/static/css/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)   107280 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/css/fonts/Eina02-Bold.f8011405.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   116316 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/css/fonts/Eina02-Regular.2e682693.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   112880 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/css/fonts/Eina02-SemiBold.c5f9b8e3.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   111976 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/css/fonts/bootstrap-icons.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    83304 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/css/fonts/bootstrap-icons.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    47832 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/css/fonts/bpmn.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   133048 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/css/fonts/bpmn.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    47680 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/css/fonts/bpmn.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    16004 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/css/fonts/bpmn.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    13028 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/css/fonts/bpmn.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    30702 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/css/icons.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.789168 sloth-framework-0.1.6/sloth/api/static/css/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     6992 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/css/images/ui-icons_444444_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6988 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/css/images/ui-icons_555555_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)    35973 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/css/jquery-ui.css
+-rw-r--r--   0 runner    (1001) docker     (123)    14670 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/css/leaflet.css
+-rw-r--r--   0 runner    (1001) docker     (123)    16264 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/css/select2.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)     9481 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/css/sloth.css
+-rw-r--r--   0 runner    (1001) docker     (123)    17867 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/css/trumbowyg.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.781169 sloth-framework-0.1.6/sloth/api/static/icons/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.789168 sloth-framework-0.1.6/sloth/api/static/icons/fontawesome/
+-rw-r--r--   0 runner    (1001) docker     (123)   100170 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/icons/fontawesome/fontawesome.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)  1726692 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/icons/fontawesome/fontawesome.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.793168 sloth-framework-0.1.6/sloth/api/static/icons/fontawesome/webfonts/
+-rw-r--r--   0 runner    (1001) docker     (123)   181852 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/icons/fontawesome/webfonts/fa-brands-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   105536 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/icons/fontawesome/webfonts/fa-brands-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    60520 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/icons/fontawesome/webfonts/fa-regular-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    23940 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/icons/fontawesome/webfonts/fa-regular-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    10556 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/icons/fontawesome/webfonts/fa-v4compatibility.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/icons/fontawesome/webfonts/fa-v4compatibility.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.793168 sloth-framework-0.1.6/sloth/api/static/icons/materialicons/
+-rw-r--r--   0 runner    (1001) docker     (123)   174176 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/icons/materialicons/LDItaoyNOAY6Uewc665JcIzCKsKc_M9flwmPq_HTTw.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   127220 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/icons/materialicons/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   155604 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/icons/materialicons/gok-H7zzDkdnRel8-DQ6KAXJ69wP1tGnf4ZGhUcel5euIg.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/icons/materialicons/materialicons.css
+-rw-r--r--   0 runner    (1001) docker     (123)   135988 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/icons/materialicons/oPWQ_lt5nv4pWNJpghLP75WiFR4kLh3kvmvRImcycg.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.793168 sloth-framework-0.1.6/sloth/api/static/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    57420 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/images/click.png
+-rw-r--r--   0 runner    (1001) docker     (123)    55448 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/images/hand.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10276 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/images/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/images/icon.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.797168 sloth-framework-0.1.6/sloth/api/static/images/images/
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/images/images/badge.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/images/images/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)    45136 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/images/login.jpeg
+-rw-r--r--   0 runner    (1001) docker     (123)    22817 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/images/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    21495 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/images/no-image.png
+-rw-r--r--   0 runner    (1001) docker     (123)    23102 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/images/sloth.png
+-rw-r--r--   0 runner    (1001) docker     (123)    13670 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/images/user.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.801168 sloth-framework-0.1.6/sloth/api/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/js/api.js
+-rw-r--r--   0 runner    (1001) docker     (123)    78743 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/js/bootstrap.bundle.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)  1665279 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/js/bpmn.js
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4098 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/js/colorpick.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.801168 sloth-framework-0.1.6/sloth/api/static/js/i18n/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      853 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/js/i18n/pt-BR.js
+-rw-r--r--   0 runner    (1001) docker     (123)    89501 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/js/jquery-3.6.0.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   520714 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/js/jquery-ui.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/js/jquery.binarytransport.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8327 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/js/jquery.mask.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    80794 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/js/jquery.timepicker.js
+-rw-r--r--   0 runner    (1001) docker     (123)   147555 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/js/leaflet.js
+-rw-r--r--   0 runner    (1001) docker     (123)    24103 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/js/masonry.pkgd.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    18453 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/js/popper.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    43994 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/js/qr-scanner-worker.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    15538 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/js/qr-scanner.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    19927 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/js/qrcode.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    73163 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/js/select2.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    17257 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/js/sloth.js
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/js/sw.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10842 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/js/tests.js
+-rw-r--r--   0 runner    (1001) docker     (123)    28280 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/js/trumbowyg.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/static/js/wpn.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.801168 sloth-framework-0.1.6/sloth/api/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/tasks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.785169 sloth-framework-0.1.6/sloth/api/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.801168 sloth-framework-0.1.6/sloth/api/templates/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/actions/execute_query.html
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/actions/execute_script.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/actions/show_icons.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6028 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/actions/workflow.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.801168 sloth-framework-0.1.6/sloth/api/templates/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/api/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.801168 sloth-framework-0.1.6/sloth/api/templates/charts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/charts/bar.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/charts/column.html
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/charts/donut.html
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/charts/legend.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/charts/pie.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.805168 sloth-framework-0.1.6/sloth/api/templates/dashboard/
+-rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/dashboard/actions.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/dashboard/apps.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/dashboard/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/dashboard/bottom.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/dashboard/cards.html
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/dashboard/dashboards.html
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/dashboard/default.html
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/dashboard/footer.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7123 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/dashboard/form.html
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/dashboard/grids.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/dashboard/header.html
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/dashboard/links.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/dashboard/menu.html
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/dashboard/messages.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/dashboard/modal.html
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/dashboard/plus.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/dashboard/report.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/dashboard/search.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/dashboard/settings.html
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/dashboard/shortcuts.html
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/dashboard/tasks.html
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/dashboard/tools.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.805168 sloth-framework-0.1.6/sloth/api/templates/inputs/
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/inputs/picker.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/inputs/qrcode.html
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/inputs/select.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.809168 sloth-framework-0.1.6/sloth/api/templates/queryset/
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/queryset/accordion.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.809168 sloth-framework-0.1.6/sloth/api/templates/queryset/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/queryset/actions/actions.html
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/queryset/actions/batch.html
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/queryset/actions/global.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/queryset/calendar.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/queryset/cards.html
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/queryset/checkbox.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/queryset/datatable.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/queryset/filter.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/queryset/filters.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11362 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/queryset/queryset.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/queryset/rows.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/queryset/scroll.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6364 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/queryset/statistics.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/queryset/timeline.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/queryset/tree.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.785169 sloth-framework-0.1.6/sloth/api/templates/renderers/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.809168 sloth-framework-0.1.6/sloth/api/templates/renderers/badges/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/renderers/badges/badge.html
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/renderers/badges/boolean.html
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/renderers/badges/danger.html
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/renderers/badges/primary.html
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/renderers/badges/status.html
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/renderers/badges/warning.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.809168 sloth-framework-0.1.6/sloth/api/templates/renderers/boolean/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/renderers/boolean/thumb.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.809168 sloth-framework-0.1.6/sloth/api/templates/renderers/calendar/
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/renderers/calendar/calendar.html
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/renderers/calendar/events.html
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/renderers/calendar/legend.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.809168 sloth-framework-0.1.6/sloth/api/templates/renderers/documents/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/renderers/documents/document.html
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/renderers/documents/popup.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.809168 sloth-framework-0.1.6/sloth/api/templates/renderers/images/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/renderers/images/banner.html
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/renderers/images/group.html
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/renderers/images/image.html
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/renderers/images/round.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.809168 sloth-framework-0.1.6/sloth/api/templates/renderers/links/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/renderers/links/file.html
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/renderers/links/url.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.809168 sloth-framework-0.1.6/sloth/api/templates/renderers/maps/
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/renderers/maps/geolocation.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4551 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/renderers/maps/map.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.813168 sloth-framework-0.1.6/sloth/api/templates/renderers/messages/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/renderers/messages/custom.html
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/renderers/messages/danger.html
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/renderers/messages/message.html
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/renderers/messages/primary.html
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/renderers/messages/success.html
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/renderers/messages/warning.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.813168 sloth-framework-0.1.6/sloth/api/templates/renderers/photos/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/renderers/photos/photo.html
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/renderers/photos/round.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.813168 sloth-framework-0.1.6/sloth/api/templates/renderers/programing/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/renderers/programing/strtable.html
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/renderers/programing/terminal.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.813168 sloth-framework-0.1.6/sloth/api/templates/renderers/progress/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/renderers/progress/primary.html
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/renderers/progress/success.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.813168 sloth-framework-0.1.6/sloth/api/templates/renderers/steps/
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/renderers/steps/check.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.813168 sloth-framework-0.1.6/sloth/api/templates/renderers/tags/
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/renderers/tags/primary.html
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/renderers/tags/tags.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.813168 sloth-framework-0.1.6/sloth/api/templates/renderers/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/renderers/utils/formatted.html
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/renderers/utils/progress.html
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/renderers/utils/qrcode.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/renderers/utils/steps.html
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/renderers/utils/table.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.813168 sloth-framework-0.1.6/sloth/api/templates/themes/
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/themes/dark.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.813168 sloth-framework-0.1.6/sloth/api/templates/valueset/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/valueset/2-column.html
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/valueset/field.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3576 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/valueset/fieldset-group.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/valueset/fieldset-list.html
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/valueset/fieldset-tab.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/valueset/fieldset.html
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/valueset/primitive.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/valueset/value.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6431 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templates/valueset/valueset.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.817168 sloth-framework-0.1.6/sloth/api/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9090 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/templatetags/tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12451 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/api/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.817168 sloth-framework-0.1.6/sloth/cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/cloud/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      688 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/cloud/printer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6116 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/cloud/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.817168 sloth-framework-0.1.6/sloth/conf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/conf/local_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/conf/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.817168 sloth-framework-0.1.6/sloth/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21773 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/core/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42840 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/core/queryset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11540 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/core/statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/core/validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21103 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/core/valueset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.817168 sloth-framework-0.1.6/sloth/db/
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/db/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.817168 sloth-framework-0.1.6/sloth/db/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    12631 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/db/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.817168 sloth-framework-0.1.6/sloth/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     3185 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.817168 sloth-framework-0.1.6/sloth/test/selenium/
+-rw-r--r--   0 runner    (1001) docker     (123)     4596 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/test/selenium/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10483 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/test/selenium/browser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.817168 sloth-framework-0.1.6/sloth/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.817168 sloth-framework-0.1.6/sloth/utils/formatter/
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/utils/formatter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.817168 sloth-framework-0.1.6/sloth/utils/http/
+-rw-r--r--   0 runner    (1001) docker     (123)     5317 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/utils/http/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.817168 sloth-framework-0.1.6/sloth/utils/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/utils/icons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28753 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/utils/icons/bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53105 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/utils/icons/fontawesome.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20959 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/utils/icons/materialicons.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.821168 sloth-framework-0.1.6/sloth/utils/log/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/utils/log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-24 23:12:24.000000 sloth-framework-0.1.6/sloth/utils/log/sql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:12:28.821168 sloth-framework-0.1.6/sloth_framework.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-24 23:12:28.000000 sloth-framework-0.1.6/sloth_framework.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10144 2023-05-24 23:12:28.000000 sloth-framework-0.1.6/sloth_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 23:12:28.000000 sloth-framework-0.1.6/sloth_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-24 23:12:28.000000 sloth-framework-0.1.6/sloth_framework.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-24 23:12:28.000000 sloth-framework-0.1.6/sloth_framework.egg-info/top_level.txt
```

### Comparing `sloth-framework-0.1.5/PKG-INFO` & `sloth-framework-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sloth-framework
-Version: 0.1.5
+Version: 0.1.6
 Summary: Metadata-based web framework for the development of management information systems
 Home-page: http://sloth.aplicativo.click/
 Author: Breno Silva
 Author-email: brenokcc@yahoo.com.br
 License: BSD License
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

### Comparing `sloth-framework-0.1.5/setup.py` & `sloth-framework-0.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 with open(os.path.join(root_dir, 'sloth/requirements.txt')) as file:
     requirements = file.read().strip().splitlines()
 
 os.chdir(root_dir)
 
 setup(
     name='sloth-framework',
-    version='0.1.5',
+    version='0.1.6',
     packages=find_packages(),
     install_requires=requirements,
     extras_require={
         'dev': [],
         'production': [],
     },
     include_package_data=True,
```

### Comparing `sloth-framework-0.1.5/sloth/Dockerfile` & `sloth-framework-0.1.6/sloth/Dockerfile`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/__init__.py` & `sloth-framework-0.1.6/sloth/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,17 +51,17 @@
                     else:
                         return True
         return False
 
 
 def meta(verbose_name=None, renderer=None, **metadata):
     def decorate(func):
-        if verbose_name:
+        if verbose_name is not None:
             setattr(func, '__verbose_name__', verbose_name)
-        if renderer:
+        if renderer is not None:
             setattr(func, '__template__', renderer)
         if metadata:
             setattr(func, '__metadata__', metadata)
 
         return func
     return decorate
```

### Comparing `sloth-framework-0.1.5/sloth/__main__.py` & `sloth-framework-0.1.6/sloth/__main__.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/actions/__init__.py` & `sloth-framework-0.1.6/sloth/actions/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -83,14 +83,33 @@
     def clean(self, value):
         if value:
             value = value.replace('.', '').replace(',', '.')
         value = super().clean(value)
         return value
 
 
+class TextField(forms.CharField):
+    def __init__(self, *args, **kwargs):
+        kwargs.update(widget=forms.Textarea())
+        super().__init__(*args, **kwargs)
+
+
+class BooleanChoiceField(forms.ChoiceField):
+    def __init__(self, *args, **kwargs):
+        kwargs.update(widget=forms.Select(), choices=[['', ''], [1, 'Sim'], [0, 'Não']])
+        super().__init__(*args, **kwargs)
+
+    def clean(self, value):
+        if value == '':
+            if self.required:
+                raise ValidationError('Selecione uma opção')
+            return None
+        return bool(int(value))
+
+
 class RegionalDateWidget(DateInput):
     input_type = 'date'
 
     def render(self, name, value, attrs=None, renderer=None):
         if isinstance(value, datetime.date):
             value = value.isoformat()
         attrs = attrs or {}
@@ -173,20 +192,23 @@
             setattr(self.instance, related_field_name, self.instantiator)
             if related_field_name in self.fields:
                 del self.fields[related_field_name]
 
         for field_name in self.fields:
             field = self.fields[field_name]
             if hasattr(field, 'queryset'):
-                if not self.request.user.is_superuser and getattr(field, 'username_lookup', None):
+                if getattr(field, 'username_lookup', None):
                     pks = list(field.queryset.filter(**{field.username_lookup: self.request.user}).values_list('pk', flat=True)[0:2])
                     if len(pks) == 1:
                         field.queryset = field.queryset.model.objects.filter(pk=pks[0])
                         field.initial = pks[0]
-                        field.widget = forms.HiddenInput()
+                        self.initial[field_name] = field.initial
+                        # field.widget = forms.HiddenInput()
+                        field.widget.attrs['class'] = '{} disabled'.format(field.widget.attrs.get('class', ''))
+                        field.widget.attrs['readonly'] = 'readonly'
                 else:
                     field.queryset = field.queryset.contextualize(self.request).apply_role_lookups(self.request.user)
 
         self.response = {}
         self.fieldsets = {}
         self.one_to_one = {}
         self.one_to_many = {}
@@ -225,22 +247,21 @@
         if text:
             self.content['alert'].append(text)
 
     def danger(self, text):
         if text:
             self.content['danger'].append(text)
 
-    def parameters(self, index):
-        values = None
+    def parameter(self, name, default=None):
         for token in self.request.path.split('/'):
-            if values is not None:
-                values.append((token))
-            if token.lower() == self.get_api_name():
-                values = []
-        return values[index] if values and len(values)>index else None
+            if '=' in token:
+                k, v = token.split('=')
+                if k == name:
+                    return v
+        return default
 
     def objects(self, model_name):
         return apps.get_model(model_name).objects.contextualize(self.request)
 
     def clear(self):
         self.show_form = False
         for k, v in self.content.items():
@@ -563,15 +584,16 @@
         return user.is_superuser or self.has_permission(user)
 
     @classmethod
     def check_fake_permission(cls, request, instance=None, instantiator=None):
         if request:  # and not request.user.is_superuser
             checker = PermissionChecker(request, instance, instantiator, getattr(cls, 'Meta', None))
             has_permission = cls.has_permission(checker, request.user)
-            return cls.check_permission(checker, request.user) if has_permission is None else has_permission
+            return has_permission
+            ### return cls.check_permission(checker, request.user) if has_permission is None else has_permission
         return True
 
     def __str__(self):
         return self.html()
 
     def get_alternative_links(self):
         return []
@@ -785,16 +807,17 @@
                         value = self.request.GET.getlist(name)
                     else:
                         value = self.request.GET.get(name)
                         if value:
                             setattr(self.instance, name, self.fields[name].clean(value))
         else:
             attr = getattr(self, 'get_{}_queryset'.format(field_name), None)
-        qs = field.queryset if attr is None else attr(field.queryset)
         self.data.update(self.request.GET)
+        qs = field.queryset if attr is None else attr(field.queryset)
+
         total = qs.count()
         qs = qs.search(q=q) if q else qs
         items = [dict(id=value.id, text=str(value), html=value.get_select_display()) for value in qs[0:25]]
         return dict(total=total, page=1, pages=math.ceil((1.0 * total) / 25), q=q, items=items )
 
     def dispose(self, milleseconds=2000):
         self.response.update(dispose=milleseconds)
@@ -912,10 +935,14 @@
 
     def contextualize(self, request):
         return self
 
     def apply_role_lookups(self, user):
         return self
 
+    def send_mail(self, to, subject, content, from_email=None):
+        from sloth.api.models import Email
+        Email.objects.send(to, subject, content, from_email)
+
 
 class ActionView(Action):
     pass
```

### Comparing `sloth-framework-0.1.5/sloth/actions/fields.py` & `sloth-framework-0.1.6/sloth/actions/fields.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/actions/inputs.py` & `sloth-framework-0.1.6/sloth/actions/inputs.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/__init__.py` & `sloth-framework-0.1.6/sloth/api/__init__.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/actions.py` & `sloth-framework-0.1.6/sloth/api/actions.py`

 * *Files 6% similar despite different names*

```diff
@@ -527,8 +527,50 @@
         style = 'primary'
 
     def view(self):
         obj = self.instance or self.instances or self.queryset
         return PdfReportResponse(self.request, obj.contextualize(self.request).html(print=True))
 
     def has_permission(self, user):
-        return self
+        return self
+
+
+class Workflow(actions.ActionView):
+    INITIAL_CONTENT = '''
+            <?xml version="1.0" encoding="UTF-8"?>
+            <bpmn:definitions xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:bpmn="http://www.omg.org/spec/BPMN/20100524/MODEL" xmlns:bpmndi="http://www.omg.org/spec/BPMN/20100524/DI" xmlns:dc="http://www.omg.org/spec/DD/20100524/DC" id="Definitions_0nf790r" targetNamespace="http://bpmn.io/schema/bpmn" exporter="bpmn-js (https://demo.bpmn.io)" exporterVersion="12.0.0">
+              <bpmn:process id="Process_0rezp77" isExecutable="false">
+                <bpmn:startEvent id="StartEvent_0disvw0" />
+              </bpmn:process>
+              <bpmndi:BPMNDiagram id="BPMNDiagram_1">
+                <bpmndi:BPMNPlane id="BPMNPlane_1" bpmnElement="Process_0rezp77">
+                  <bpmndi:BPMNShape id="_BPMNShape_StartEvent_2" bpmnElement="StartEvent_0disvw0">
+                    <dc:Bounds x="156" y="82" width="36" height="36" />
+                  </bpmndi:BPMNShape>
+                </bpmndi:BPMNPlane>
+              </bpmndi:BPMNDiagram>
+            </bpmn:definitions>
+        '''
+
+    class Meta:
+        icon = 'diagram-3'
+        verbose_name = 'Fluxograma'
+        modal = False
+        style = 'primary'
+
+    def view(self):
+        if self.request.POST:
+            content = self.request.POST['xml']
+            with open('workflow.xml', 'w') as file:
+                file.write(self.request.POST['xml'])
+            with open('workflow.png', 'wb') as file:
+                file.write(base64.b64decode(self.request.POST['png']))
+        else:
+            if os.path.exists('workflow.xml'):
+                with open('workflow.xml') as file:
+                    content = file.read()
+            else:
+                content = Workflow.INITIAL_CONTENT
+        return self.render('actions/workflow.html', title='Fluxograma', content=content)
+
+    def has_permission(self, user):
+        return user.is_superuser
```

### Comparing `sloth-framework-0.1.5/sloth/api/backends/__init__.py` & `sloth-framework-0.1.6/sloth/api/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/dashboard.py` & `sloth-framework-0.1.6/sloth/api/dashboard.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
     def __init__(self, request):
         self.redirect_url = None
         self.redirect_message = None
         self.request = request
         self.data = dict(
             info=[], warning=[], search=[], menu=[], links=[], shortcuts=[], cards=[], plus=[], navbar={},
-            floating=[], navigation=[], settings=[], center=[], right=[], actions=[], tools=[], header={}, footer={},
+            floating=[], navigation=[], settings=[], top=[], center=[], right=[], bottom=[], actions=[], tools=[], header={}, footer={},
             styles=[], scripts=[]
         )
         self.defined_apps = {}
         self.enabled_apps = set()
         if self.request.user.is_authenticated:
             self.load(request)
         if self.request.path == '/app/dashboard/':
@@ -286,15 +286,15 @@
 
     def __init__(self, request):
         self.apps = {}
         self.dashboards = []
         self.request = request
         self.data = dict(
             info=[], warning=[], search=[], menu=[], links=[], shortcuts=[], cards=[], tasks=[], plus=[], navbar={},
-            floating=[], navigation=[], settings=[], center=[], right=[], actions=[], tools=[], header={}, footer={},
+            floating=[], navigation=[], settings=[], top=[], center=[], right=[], bottom=[], actions=[], tools=[], header={}, footer={},
             styles=[], scripts=[]
         )
         self.data['navigation'].append(
             dict(url='/app/dashboard/', label='Principal', icon='house', app=None)
         )
         for cls in DASHBOARDS:
             dashboard = cls(request)
@@ -319,14 +319,19 @@
                     request.session.save()
                     break
             raise ReadyResponseException(HttpResponseRedirect('/app/dashboard/'))
 
         if self.request.user.is_superuser:
             self.superuser()
 
+        if self.request.path.startswith('/app/'):
+            self.data['menu'] = self.create_menu(render=True)
+        else:
+            self.data['menu'] = self.create_menu(render=False)
+
     def main(self):
         for dashboard in self.dashboards:
             if dashboard.view.__func__ != Dashboard.view:
                 return dashboard
 
     def superuser(self):
         from django.apps import apps
@@ -341,15 +346,15 @@
                 add_item = True
                 for item in self.data['search']:
                     add_item = add_item and not item['url'] == url
                 if add_item:
                     item = dict(label=pretty(str(model_verbose_name_plural)), description=None, url=url, icon=icon, subitems=[], app=None)
                     self.data['search'].append(item)
 
-    def render_menu(self):
+    def create_menu(self, render=True):
         icons = {}
         default_icon = 'record2'
         def create_submenu(hierarchy, item, level=0):
             tokens = item['hierarchy'].split('::')
             if len(tokens) == 1:
                 if level == 0:
                     icons[tokens[0]] = item['menu_icon'] or item['icon'] or default_icon
@@ -371,14 +376,17 @@
         for item in self.data['menu']:
             if item['hierarchy']:
                 create_submenu(menu, item)
             else:
                 menu[item['label']] = item
                 icons[item['label']] = item['icon'] or 'record-circle'
 
+        if not render:
+            return dict(icons=icons, items=menu)
+
         html = []
         def append_html(label, item, level=0):
             ident = '\t' * level
             nbsp = '&nbsp;' * level * 3
             html.append('{}<li>'.format(ident))
             icon = '<i class="bi bi-{} menu-item-icon"></i> '.format(icons[label]) if level == 0 else ''
             if 'url' in item:
@@ -388,8 +396,15 @@
                 html.append('{}<ul>'.format(ident))
                 for sublabel, subitem in item.items():
                     append_html(sublabel, subitem, level+1)
                 html.append('{}</ul>'.format(ident))
             html.append('{}</li>'.format(ident))
         for label, item in menu.items():
             append_html(label, item, 0)
-        return mark_safe('\n'.join(html))
+        return mark_safe('\n'.join(html))
+
+    def serialize(self, data):
+        for k, v in data.items():
+            pass # print(k, v)
+        for k, v in data.get('append', {}).items():
+            self.data[k].append(v)
+        return self.data
```

### Comparing `sloth-framework-0.1.5/sloth/api/management/commands/cloud.py` & `sloth-framework-0.1.6/sloth/api/management/commands/cloud.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/management/commands/query.py` & `sloth-framework-0.1.6/sloth/api/management/commands/query.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/management/commands/send_web_push_notification.py` & `sloth-framework-0.1.6/sloth/api/management/commands/send_web_push_notification.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/management/commands/startserver.py` & `sloth-framework-0.1.6/sloth/api/management/commands/startserver.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/management/commands/sync.py` & `sloth-framework-0.1.6/sloth/api/management/commands/sync.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/migrations/0001_initial.py` & `sloth-framework-0.1.6/sloth/api/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/migrations/0002_role_user.py` & `sloth-framework-0.1.6/sloth/api/migrations/0002_role_user.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/migrations/0003_alter_application_user.py` & `sloth-framework-0.1.6/sloth/api/migrations/0003_alter_application_user.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/migrations/0004_task.py` & `sloth-framework-0.1.6/sloth/api/migrations/0004_task.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/migrations/0005_task_stopped_alter_task_message.py` & `sloth-framework-0.1.6/sloth/api/migrations/0005_task_stopped_alter_task_message.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/migrations/0006_role_active_alter_role_name_alter_role_scope_key_and_more.py` & `sloth-framework-0.1.6/sloth/api/migrations/0006_role_active_alter_role_name_alter_role_scope_key_and_more.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/migrations/0007_alter_scope_description_alter_task_error.py` & `sloth-framework-0.1.6/sloth/api/migrations/0007_alter_scope_description_alter_task_error.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/migrations/0008_alter_application_available_scopes_and_more.py` & `sloth-framework-0.1.6/sloth/api/migrations/0008_alter_application_available_scopes_and_more.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/migrations/0009_pushnotification.py` & `sloth-framework-0.1.6/sloth/api/migrations/0009_pushnotification.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/migrations/0010_alter_pushnotification_user.py` & `sloth-framework-0.1.6/sloth/api/migrations/0010_alter_pushnotification_user.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/migrations/0011_alter_application_client_secret.py` & `sloth-framework-0.1.6/sloth/api/migrations/0011_alter_application_client_secret.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/migrations/0012_authcode.py` & `sloth-framework-0.1.6/sloth/api/migrations/0012_authcode.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/migrations/0013_task_partial_task_total.py` & `sloth-framework-0.1.6/sloth/api/migrations/0013_task_partial_task_total.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/migrations/0014_email.py` & `sloth-framework-0.1.6/sloth/api/migrations/0014_email.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/models.py` & `sloth-framework-0.1.6/sloth/api/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # -*- coding: utf-8 -*-
+import sys
 import json
 from datetime import datetime
 from django.apps import apps
 from django.conf import settings
 from oauth2_provider.models import AbstractApplication
 from django.contrib.auth.models import User as DjangoUser, AnonymousUser
 from sloth.db import models, meta
@@ -189,15 +190,15 @@
 
     def view(self):
         return self.value_set('general_data', 'access_data', 'default_scopes', 'available_scopes')
 
 
 class TaskManager(models.Manager):
     def all(self):
-        return self.display(
+        return self.lookups(user__username='username').display(
             'id', 'user', 'name', 'start', 'end', 'get_progress', 'message'
         ).attach(
             'running', 'finished', 'unfinished', 'stopped'
         ).global_actions('ManageTaskExecution')
 
     @meta('Em Execução')
     def running(self):
@@ -284,15 +285,15 @@
 
 class EmailManager(models.Manager):
     def all(self):
         return self.rows()
 
     def send(self, to, subject, content, from_email=None):
         to = [to] if isinstance(to, str) else list(to)
-        return self.create(from_email=from_email, to=', '.join(to), subject=subject, content=content)
+        return self.create(from_email=from_email or 'no-replay@mail.com', to=', '.join(to), subject=subject, content=content)
 
 
 class Email(models.Model):
     from_email = models.EmailField('Remetente')
     to = models.TextField('Destinatário', help_text='Separar endereços de e-mail por ",".')
     subject = models.CharField('Assunto')
     content = models.TextField('Conteúdo', formatted=True)
@@ -312,17 +313,16 @@
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
     def __str__(self):
         return self.subject
 
     def save(self, *args, **kwargs):
-        super().save(*args, **kwargs)
         to = [email.strip() for email in self.to.split(',')]
         msg = EmailMultiAlternatives(self.subject, strip_tags(self.content), self.from_email, to)
         msg.attach_alternative(self.content, "text/html")
-        if msg.send(fail_silently=False):
+        if settings.DEBUG or 'test' in sys.argv or msg.send(fail_silently=True):
             self.sent_at = datetime.now()
-            super().save(*args, **kwargs)
+        super().save(*args, **kwargs)
 
 
 setattr(AnonymousUser, 'roles', Role.objects.none())
```

### Comparing `sloth-framework-0.1.5/sloth/api/static/css/all.min.css` & `sloth-framework-0.1.6/sloth/api/static/css/all.min.css`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/static/css/bootstrap-icons.css` & `sloth-framework-0.1.6/sloth/api/static/css/bootstrap-icons.css`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/static/css/bootstrap.min.css` & `sloth-framework-0.1.6/sloth/api/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/static/css/colorpick.min.css` & `sloth-framework-0.1.6/sloth/api/static/css/colorpick.min.css`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/static/css/fonts/Eina02-Bold.f8011405.ttf` & `sloth-framework-0.1.6/sloth/api/static/css/fonts/Eina02-Bold.f8011405.ttf`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/static/css/fonts/Eina02-Regular.2e682693.ttf` & `sloth-framework-0.1.6/sloth/api/static/css/fonts/Eina02-Regular.2e682693.ttf`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/static/css/fonts/Eina02-SemiBold.c5f9b8e3.ttf` & `sloth-framework-0.1.6/sloth/api/static/css/fonts/Eina02-SemiBold.c5f9b8e3.ttf`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/static/css/fonts/bootstrap-icons.woff` & `sloth-framework-0.1.6/sloth/api/static/css/fonts/bootstrap-icons.woff`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/static/css/fonts/bootstrap-icons.woff2` & `sloth-framework-0.1.6/sloth/api/static/css/fonts/bootstrap-icons.woff2`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/static/css/icons.svg` & `sloth-framework-0.1.6/sloth/api/static/css/icons.svg`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/static/css/images/ui-icons_444444_256x240.png` & `sloth-framework-0.1.6/sloth/api/static/css/images/ui-icons_444444_256x240.png`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/static/css/images/ui-icons_555555_256x240.png` & `sloth-framework-0.1.6/sloth/api/static/css/images/ui-icons_555555_256x240.png`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/static/css/jquery-ui.css` & `sloth-framework-0.1.6/sloth/api/static/css/jquery-ui.css`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/static/css/leaflet.css` & `sloth-framework-0.1.6/sloth/api/static/css/leaflet.css`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/static/css/select2.min.css` & `sloth-framework-0.1.6/sloth/api/static/css/select2.min.css`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/static/css/sloth.css` & `sloth-framework-0.1.6/sloth/api/static/css/sloth.css`

 * *Files 7% similar despite different names*

```diff
@@ -232,14 +232,27 @@
     width: calc(100% - 200px);
 }
 .select2-selection__clear span{
     position: relative;
     color: #CCC;
     top: -8px;
 }
+select[readonly].select2-hidden-accessible + .select2-container {
+    pointer-events: none;
+    touch-action: none;
+}
+
+select[readonly].select2-hidden-accessible + .select2-container .select2-selection {
+    background: #eee;
+    box-shadow: none;
+}
+
+select[readonly].select2-hidden-accessible + .select2-container .select2-selection__arrow, select[readonly].select2-hidden-accessible + .select2-container .select2-selection__clear {
+    display: none;
+}
 .messages{
     position: fixed;
     top: 0;
     left: 0;
     width: 100%;
     z-index: 999;
     border-radius: 0;
@@ -397,15 +410,15 @@
 }
 .material-icons{
     position: relative;
     top: 2px;
 	font-size: 16px;
 }
 
-.reloadable-fieldset, .reloadable-queryset{
+.reloadable-fieldset, .reloadable-queryset, .fieldset-group{
     margin-bottom: 10px;
 }
 
 body{
     background-color: #FCFCFC;
     font-family: Eina02-Regular;
 }
```

### Comparing `sloth-framework-0.1.5/sloth/api/static/css/trumbowyg.min.css` & `sloth-framework-0.1.6/sloth/api/static/css/trumbowyg.min.css`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/static/icons/fontawesome/fontawesome.min.css` & `sloth-framework-0.1.6/sloth/api/static/icons/fontawesome/fontawesome.min.css`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/static/icons/fontawesome/fontawesome.min.js` & `sloth-framework-0.1.6/sloth/api/static/icons/fontawesome/fontawesome.min.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/static/icons/fontawesome/webfonts/fa-brands-400.ttf` & `sloth-framework-0.1.6/sloth/api/static/icons/fontawesome/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/static/icons/fontawesome/webfonts/fa-brands-400.woff2` & `sloth-framework-0.1.6/sloth/api/static/icons/fontawesome/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/static/icons/fontawesome/webfonts/fa-regular-400.ttf` & `sloth-framework-0.1.6/sloth/api/static/icons/fontawesome/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/static/icons/fontawesome/webfonts/fa-regular-400.woff2` & `sloth-framework-0.1.6/sloth/api/static/icons/fontawesome/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/static/icons/fontawesome/webfonts/fa-v4compatibility.ttf` & `sloth-framework-0.1.6/sloth/api/static/icons/fontawesome/webfonts/fa-v4compatibility.ttf`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/static/icons/fontawesome/webfonts/fa-v4compatibility.woff2` & `sloth-framework-0.1.6/sloth/api/static/icons/fontawesome/webfonts/fa-v4compatibility.woff2`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/static/icons/materialicons/LDItaoyNOAY6Uewc665JcIzCKsKc_M9flwmPq_HTTw.woff2` & `sloth-framework-0.1.6/sloth/api/static/icons/materialicons/LDItaoyNOAY6Uewc665JcIzCKsKc_M9flwmPq_HTTw.woff2`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/static/icons/materialicons/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2` & `sloth-framework-0.1.6/sloth/api/static/icons/materialicons/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/static/icons/materialicons/gok-H7zzDkdnRel8-DQ6KAXJ69wP1tGnf4ZGhUcel5euIg.woff2` & `sloth-framework-0.1.6/sloth/api/static/icons/materialicons/gok-H7zzDkdnRel8-DQ6KAXJ69wP1tGnf4ZGhUcel5euIg.woff2`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/static/icons/materialicons/materialicons.css` & `sloth-framework-0.1.6/sloth/api/static/icons/materialicons/materialicons.css`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/static/icons/materialicons/oPWQ_lt5nv4pWNJpghLP75WiFR4kLh3kvmvRImcycg.woff2` & `sloth-framework-0.1.6/sloth/api/static/icons/materialicons/oPWQ_lt5nv4pWNJpghLP75WiFR4kLh3kvmvRImcycg.woff2`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/static/images/click.png` & `sloth-framework-0.1.6/sloth/api/static/images/click.png`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/static/images/hand.png` & `sloth-framework-0.1.6/sloth/api/static/images/hand.png`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/static/images/icon.png` & `sloth-framework-0.1.6/sloth/api/static/images/icon.png`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/static/images/icon.svg` & `sloth-framework-0.1.6/sloth/api/static/images/icon.svg`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/static/images/images/badge.png` & `sloth-framework-0.1.6/sloth/api/static/images/images/badge.png`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/static/images/images/icon.png` & `sloth-framework-0.1.6/sloth/api/static/images/images/icon.png`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/static/images/login.jpeg` & `sloth-framework-0.1.6/sloth/api/static/images/login.jpeg`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/static/images/logo.png` & `sloth-framework-0.1.6/sloth/api/static/images/logo.png`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/static/images/logo.svg` & `sloth-framework-0.1.6/sloth/api/static/images/logo.svg`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/static/images/no-image.png` & `sloth-framework-0.1.6/sloth/api/static/images/no-image.png`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/static/images/sloth.png` & `sloth-framework-0.1.6/sloth/api/static/images/sloth.png`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/static/images/user.png` & `sloth-framework-0.1.6/sloth/api/static/images/user.png`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/static/js/api.js` & `sloth-framework-0.1.6/sloth/api/static/js/api.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/static/js/bootstrap.bundle.min.js` & `sloth-framework-0.1.6/sloth/api/static/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/static/js/colorpick.min.js` & `sloth-framework-0.1.6/sloth/api/static/js/colorpick.min.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/static/js/i18n/pt-BR.js` & `sloth-framework-0.1.6/sloth/api/static/js/i18n/pt-BR.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/static/js/jquery-3.6.0.min.js` & `sloth-framework-0.1.6/sloth/api/static/js/jquery-3.6.0.min.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/static/js/jquery-ui.js` & `sloth-framework-0.1.6/sloth/api/static/js/jquery-ui.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/static/js/jquery.binarytransport.js` & `sloth-framework-0.1.6/sloth/api/static/js/jquery.binarytransport.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/static/js/jquery.mask.min.js` & `sloth-framework-0.1.6/sloth/api/static/js/jquery.mask.min.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/static/js/jquery.timepicker.js` & `sloth-framework-0.1.6/sloth/api/static/js/jquery.timepicker.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/static/js/leaflet.js` & `sloth-framework-0.1.6/sloth/api/static/js/leaflet.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/static/js/masonry.pkgd.min.js` & `sloth-framework-0.1.6/sloth/api/static/js/masonry.pkgd.min.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/static/js/popper.min.js` & `sloth-framework-0.1.6/sloth/api/static/js/popper.min.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/static/js/qr-scanner-worker.min.js` & `sloth-framework-0.1.6/sloth/api/static/js/qr-scanner-worker.min.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/static/js/qr-scanner.min.js` & `sloth-framework-0.1.6/sloth/api/static/js/qr-scanner.min.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/static/js/qrcode.min.js` & `sloth-framework-0.1.6/sloth/api/static/js/qrcode.min.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/static/js/select2.min.js` & `sloth-framework-0.1.6/sloth/api/static/js/select2.min.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/static/js/sloth.js` & `sloth-framework-0.1.6/sloth/api/static/js/sloth.js`

 * *Files 12% similar despite different names*

#### js-beautify {}

```diff
@@ -56,36 +56,51 @@
         });
     },
     open: function(url, method, data) {
         $(this).request(url, method || 'GET', data || {}, function(html) {
             $('main').html(html).initialize();
         });
     },
+    ipopup: function(url) {
+        var html = '<iframe src="' + url + '" width="100%" height="500px"></iframe>';
+        $('#modal').find('.modal-body').html(html);
+        $('#modal').modal('show');
+        $('#modal').find('.modal-body').css('visibility', 'visible');
+    },
     popup: function(url, method, data) {
         $('.alert-dismissible').hide();
         if (url.indexOf('?') > 0) url = url += '&modal=1'
         else url += '?modal=1'
 
         if (window['POPUP_STACK'] == null) {
             window['POPUP_STACK'] = [];
+            window['POPUP_STACK_SELECT2'] = [];
             $('#modal').on('hidden.bs.modal', function(e) {
                 if (window['POPUP_STACK'].length > 0) {
                     $('#modal .modal-body').replaceWith(window['POPUP_STACK'].pop().initialize());
                     $('#modal').modal('show');
                     $('#modal').find('.modal-body').css('visibility', 'visible');
+                    var vals = window['POPUP_STACK_SELECT2'].pop();
+                    for (k in vals) {
+                        $('#' + k).val(vals[k]).trigger('change')
+                    }
                 } else $('#modal').find('.modal-body').html('');
             });
             $('#modal').on('shown.bs.modal', function(e) {
                 $('#modal').responsive();
             });
         }
         if ($('#modal').find('.modal-body').html().trim()) {
             $('#modal').find('.modal-body').css('visibility', 'hidden');
             $('#modal .modal-body .select2-hidden-accessible').select2("destroy");
             window['POPUP_STACK'].push($('#modal').find('.modal-body').clone());
+            var vals = {};
+            var elements = $('.modal-body select');
+            for (var i = 0; i < elements.length; i++) vals[elements[i].id] = $(elements[i]).val();
+            window['POPUP_STACK_SELECT2'].push(vals);
         }
         $(this).request(url, method || 'GET', data || {}, function(html) {
             $('#modal').find('.modal-body').html(html).initialize();
             if ($('.modal-body input[type=text]:first').length > 0) {
                 window.setTimeout(function() {
                     //$('.modal-body').find('input[type=text], input[type=number]').first().focus();
                 }, 200);
```

### Comparing `sloth-framework-0.1.5/sloth/api/static/js/sw.js` & `sloth-framework-0.1.6/sloth/api/static/js/sw.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/static/js/tests.js` & `sloth-framework-0.1.6/sloth/api/static/js/tests.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -229,15 +229,15 @@
         if (tokens.length == 3 && value[2] == '/' && value[5] == '/') value = tokens[2] + '-' + tokens[1] + '-' + tokens[0];
         var element = $(cursor || document).find("input[name='" + name + "'], textarea[name='" + name + "']").not("input[type='checkbox']").not("input[type='hidden']").first();
         if (!element[0]) element = $(cursor || document).find("label").filter(function() {
             return $(this).text().trim().replace('*', '') === name;
         }).parent().find('input, textarea').not("input[type='checkbox']").first();
         $('input[name=hidden-upload-value]').remove();
         if (element.prop("type") == 'file') {
-            $('<input type="hidden" name="hidden-upload-value" value="' + element[0].id + ':' + value + '">').appendTo(document.body);
+            $('<input type="hidden" name="hidden-upload-value" value="' + element[0].id + '">').appendTo(document.body);
             return element;
         }
 
         if (recursively(element)) {
             return enter(name, value, submit);
         } else if (element.length > 0) {
             function afterScrool() {
```

### Comparing `sloth-framework-0.1.5/sloth/api/static/js/trumbowyg.min.js` & `sloth-framework-0.1.6/sloth/api/static/js/trumbowyg.min.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/static/js/wpn.js` & `sloth-framework-0.1.6/sloth/api/static/js/wpn.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/tasks/__init__.py` & `sloth-framework-0.1.6/sloth/api/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/templates/actions/execute_query.html` & `sloth-framework-0.1.6/sloth/api/templates/actions/execute_query.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/templates/actions/show_icons.html` & `sloth-framework-0.1.6/sloth/api/templates/actions/show_icons.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/templates/api/index.html` & `sloth-framework-0.1.6/sloth/api/templates/api/index.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/templates/charts/bar.html` & `sloth-framework-0.1.6/sloth/api/templates/charts/bar.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/templates/charts/column.html` & `sloth-framework-0.1.6/sloth/api/templates/charts/column.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/templates/charts/pie.html` & `sloth-framework-0.1.6/sloth/api/templates/charts/pie.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/templates/dashboard/actions.html` & `sloth-framework-0.1.6/sloth/api/templates/dashboard/actions.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/templates/dashboard/apps.html` & `sloth-framework-0.1.6/sloth/api/templates/dashboard/apps.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/templates/dashboard/base.html` & `sloth-framework-0.1.6/sloth/api/templates/dashboard/base.html`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     {% for url in dashboard.data.scripts %}
       <script src="{{ url }}?version={{ dashboard.data.footer.version }}"></script>
     {% endfor %}
     {% block extrahead %} {% endblock %}
 
   </head>
   <body id="{{ request.path|url_slug }}">
-    {% include "dashboard/menu.html" with menu=dashboard.render_menu %}
+    {% include "dashboard/menu.html" with menu=dashboard.data.menu %}
     {% block header %}{% include "dashboard/header.html" %}{% endblock %}
     {% include "dashboard/links.html" with data=dashboard.data %}
 
       <main>
 {% endif %}
 
 {% block content %}
```

#### html2text {}

```diff
@@ -16,15 +16,15 @@
  {% endif %} {% if dashboard.data.navbar.favicon %}
  {% endif %}
  {% if 0 %} {% include "themes/dark.html" %} {% endif %} {% for url in
 dashboard.data.styles %}
  {% endfor %}
  {% for url in dashboard.data.scripts %}
  {% endfor %} {% block extrahead %} {% endblock %}
-{% include "dashboard/menu.html" with menu=dashboard.render_menu %} {% block
+{% include "dashboard/menu.html" with menu=dashboard.data.menu %} {% block
 header %}{% include "dashboard/header.html" %}{% endblock %} {% include
 "dashboard/links.html" with data=dashboard.data %}  {% endif %} {% block
 content %} {% endblock %} {% include "dashboard/messages.html" %} {% if not
 request|is_ajax %}
   {% block footer %} {% include "dashboard/footer.html" %} {% endblock %} {%
 include "dashboard/modal.html" %} {% include "dashboard/bottom.html" %}
 {% endif %}
```

### Comparing `sloth-framework-0.1.5/sloth/api/templates/dashboard/bottom.html` & `sloth-framework-0.1.6/sloth/api/templates/dashboard/bottom.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/templates/dashboard/cards.html` & `sloth-framework-0.1.6/sloth/api/templates/dashboard/cards.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/templates/dashboard/footer.html` & `sloth-framework-0.1.6/sloth/api/templates/dashboard/footer.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/templates/dashboard/form.html` & `sloth-framework-0.1.6/sloth/api/templates/dashboard/form.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/templates/dashboard/grids.html` & `sloth-framework-0.1.6/sloth/api/templates/dashboard/grids.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/templates/dashboard/header.html` & `sloth-framework-0.1.6/sloth/api/templates/dashboard/header.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/templates/dashboard/links.html` & `sloth-framework-0.1.6/sloth/api/templates/dashboard/links.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/templates/dashboard/menu.html` & `sloth-framework-0.1.6/sloth/api/templates/dashboard/menu.html`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,15 @@
     width:0px;
     height:100vh;
     position:absolute;
     top:0;
     left:0;
     z-index: 999;
     margin-left:-250px;
+    display:none;
     width: 250;
     overflow-y: scroll;
   }
   .side-menu .bi-x{
     cursor: pointer;
     margin-top:10px;
     margin-right:15px;
@@ -75,16 +76,16 @@
     <i class="bi bi-x"></i>
     <ul class="open">
         {{ menu }}
     </ul>
 </div>
 <script>
 $( document ).ready(function() {
-    $('#menu-toogler').click(function(){$('.side-menu').animate({'margin-left': '0px'},'slow');});
-    $('.side-menu .bi-x').click(function() {$('.side-menu').animate({'margin-left': '-250px'},'slow');});
+    $('#menu-toogler').click(function(){$('.side-menu').animate({'margin-left': '0px'},'slow').show();});
+    $('.side-menu .bi-x').click(function() {$('.side-menu').animate({'margin-left': '-250px'},'slow').hide();});
     $('.side-menu').mouseleave(function(){$(this).find('.bi-x').click()});
     $('.side-menu a').click(function(){
         var opened = $(this).parent().parent().find('ul.open');
         opened.slideUp();
         $(opened).parent().find('> a > i.bi-chevron-left').removeClass('bi-chevron-left').addClass('bi-chevron-down');
         if($(this).parent().find('> ul').hasClass('open')){
             $(this).parent().find('> ul').slideUp().toggleClass('open');
```

### Comparing `sloth-framework-0.1.5/sloth/api/templates/dashboard/messages.html` & `sloth-framework-0.1.6/sloth/api/templates/dashboard/messages.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/templates/dashboard/modal.html` & `sloth-framework-0.1.6/sloth/api/templates/dashboard/modal.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/templates/dashboard/plus.html` & `sloth-framework-0.1.6/sloth/api/templates/dashboard/plus.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/templates/dashboard/report.html` & `sloth-framework-0.1.6/sloth/api/templates/dashboard/report.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/templates/dashboard/search.html` & `sloth-framework-0.1.6/sloth/api/templates/dashboard/search.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/templates/dashboard/settings.html` & `sloth-framework-0.1.6/sloth/api/templates/dashboard/settings.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/templates/dashboard/shortcuts.html` & `sloth-framework-0.1.6/sloth/api/templates/dashboard/shortcuts.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/templates/dashboard/tasks.html` & `sloth-framework-0.1.6/sloth/api/templates/dashboard/tasks.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/templates/dashboard/tools.html` & `sloth-framework-0.1.6/sloth/api/templates/dashboard/tools.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/templates/inputs/picker.html` & `sloth-framework-0.1.6/sloth/api/templates/inputs/picker.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/templates/inputs/qrcode.html` & `sloth-framework-0.1.6/sloth/api/templates/inputs/qrcode.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/templates/inputs/select.html` & `sloth-framework-0.1.6/sloth/api/templates/inputs/select.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/templates/queryset/accordion.html` & `sloth-framework-0.1.6/sloth/api/templates/queryset/accordion.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/templates/queryset/calendar.html` & `sloth-framework-0.1.6/sloth/api/templates/queryset/calendar.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/templates/queryset/cards.html` & `sloth-framework-0.1.6/sloth/api/templates/queryset/cards.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/templates/queryset/datatable.html` & `sloth-framework-0.1.6/sloth/api/templates/queryset/datatable.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/templates/queryset/filter.html` & `sloth-framework-0.1.6/sloth/api/templates/queryset/filter.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/templates/queryset/filters.html` & `sloth-framework-0.1.6/sloth/api/templates/queryset/filters.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/templates/queryset/queryset.html` & `sloth-framework-0.1.6/sloth/api/templates/queryset/queryset.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/templates/queryset/rows.html` & `sloth-framework-0.1.6/sloth/api/templates/queryset/rows.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/templates/queryset/scroll.html` & `sloth-framework-0.1.6/sloth/api/templates/queryset/scroll.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/templates/queryset/statistics.html` & `sloth-framework-0.1.6/sloth/api/templates/queryset/statistics.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/templates/queryset/timeline.html` & `sloth-framework-0.1.6/sloth/api/templates/queryset/timeline.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/templates/queryset/tree.html` & `sloth-framework-0.1.6/sloth/api/templates/queryset/tree.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/templates/renderers/calendar/calendar.html` & `sloth-framework-0.1.6/sloth/api/templates/renderers/calendar/calendar.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/templates/renderers/maps/map.html` & `sloth-framework-0.1.6/sloth/api/templates/renderers/maps/map.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/templates/renderers/programing/strtable.html` & `sloth-framework-0.1.6/sloth/api/templates/renderers/programing/strtable.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/templates/renderers/utils/steps.html` & `sloth-framework-0.1.6/sloth/api/templates/renderers/utils/steps.html`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 {% load tags %}
 <style>
-    .steps-horizontal{
+    .steps-horizontal-{{ key }}{
         overflow-x: hidden;
         min-width: {{ value|length|add:2 }}00;
     }
-	.steps-horizontal .step{
+	.steps-horizontal-{{ key }} .step{
 		vertical-align: top;
 		display: inline-block;
 		text-align: center;
 		width: 100;
 	}
 	.step .cicle{
 		width: 50px;
@@ -30,53 +30,53 @@
 		width: 100;
 		margin-top: 10;
 		font-size: 80%;
 	}
 	.step .text-date{
 	    font-weight: bold;
 	}
-	.steps-horizontal .divider{
+	.steps-horizontal-{{ key }} .divider{
 		border-top: solid 1px;
 		width: {{ value|length|add:-1 }}00;
 		position: relative;
 		top: 25;
 		border-color: #BBB;
 
 	}
-	.steps-vertical{
+	.steps-vertical-{{ key }}{
 		width: 100;
 		margin-left: calc(50% - 100px);
 	}
-	.steps-vertical .step{
+	.steps-vertical-{{ key }} .step{
 		display: inline-flex;
 		width: 200;
 	}
-	.steps-vertical .divider{
+	.steps-vertical-{{ key }} .divider{
 		height: 20;
 		border-left: solid 1px;
 		border-color: #BBB;
 		width: 1;
 		margin: auto;
 	}
 </style>
 
 {% if request|mobile or compact or request.GET.compact %}
-<div class="steps-vertical">
+<div class="steps-vertical-{{ key }}">
     {% for step, date in value %}
         <div class="step">
             <div class="cicle {% if date %}active bg-primary border border-primary{% endif %}">{{ forloop.counter }}</div>
             <div class="text">{{ step }} {% if date %}<div class="text-date">{{ date }}</div>{% endif %}</div>
         </div>
         {% if not forloop.last %}
             <div class="divider"></div>
         {% endif %}
     {% endfor %}
 </div>
 {% else %}
-<div class="steps-horizontal" align="center">
+<div class="steps-horizontal-{{ key }}" align="center">
     <div class="divider"></div>
     {% for step, date in value %}
         <div class="step">
             <div class="cicle {% if date %}active bg-primary border border-primary{% endif %}">{{ forloop.counter }}</div>
             <div class="text">{{ step }} {% if date %}<div class="text-date">{{ date }}</div>{% endif %}</div>
         </div>
     {% endfor %}
```

### Comparing `sloth-framework-0.1.5/sloth/api/templates/renderers/utils/table.html` & `sloth-framework-0.1.6/sloth/api/templates/renderers/utils/table.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/templates/themes/dark.html` & `sloth-framework-0.1.6/sloth/api/templates/themes/dark.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/templates/valueset/fieldset-group.html` & `sloth-framework-0.1.6/sloth/api/templates/valueset/fieldset-group.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/templates/valueset/fieldset-list.html` & `sloth-framework-0.1.6/sloth/api/templates/valueset/fieldset-list.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/templates/valueset/fieldset.html` & `sloth-framework-0.1.6/sloth/api/templates/valueset/fieldset.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/templates/valueset/value.html` & `sloth-framework-0.1.6/sloth/api/templates/valueset/value.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/templates/valueset/valueset.html` & `sloth-framework-0.1.6/sloth/api/templates/valueset/valueset.html`

 * *Files 1% similar despite different names*

```diff
@@ -95,15 +95,17 @@
                             {% include 'valueset/fieldset.html' with data=item %}
                         {% endif %}
                         {% if item.type == 'statistics' %}
                             {% include 'valueset/fieldset.html' with data=item %}
                         {% endif %}
                         {% if item.type == 'primitive' %}
                             {% if item.template %}
-                                {% include item.template with value=item.value metadata=item.metadata %}
+                                <div class="reloadable-fieldset" id="{{ item.key }}" data-path="{{ item.path }}">
+                                {% include item.template with value=item.value metadata=item.metadata key=item.key %}
+                                </div>
                             {% else %}
                                 <div class="reloadable-fieldset box responsive-container" id="{{ item.key }}" data-path="{{ item.path }}">
                                     {% include 'valueset/field.html' with v=item %}
                                 </div>
                             {% endif %}
                         {% endif %}
                     {% endfor %}
```

### Comparing `sloth-framework-0.1.5/sloth/api/templatetags/tags.py` & `sloth-framework-0.1.6/sloth/api/templatetags/tags.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/api/urls.py` & `sloth-framework-0.1.6/sloth/api/urls.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,19 +19,20 @@
     urlpatterns.append(re_path(r'^api/{}/(?P<path>.*)/$'.format(model_name), views.api_model_dispatcher))
     urlpatterns.append(re_path(r'^meta/{}/(?P<path>.*)/$'.format(model_name), views.api_model_dispatcher))
 
 urlpatterns.append(re_path(r'^api/(?P<path>.*)/$', views.api_dispatcher))
 urlpatterns.append(re_path(r'^meta/(?P<path>.*)/$', views.api_dispatcher))
 
 urlpatterns.extend(static(settings.STATIC_URL, document_root=settings.STATIC_ROOT))
-urlpatterns.extend(static(settings.MEDIA_URL, document_root=settings.MEDIA_ROOT))
+# urlpatterns.extend(static(settings.MEDIA_URL, document_root=settings.MEDIA_ROOT))
 
 
 urlpatterns.extend([
     path('', views.index),
     path('app/', views.index),
     path('app/manifest/', views.manifest),
     path('icon', views.icon),
     path('favicon.ico', views.favicon),
     re_path(r'^apple-touch.*', views.icon),
     re_path(r'^app/(?P<path>.*)/$', views.app),
+    re_path(r'^media/(?P<path>.*)/$', views.media),
 ])
```

### Comparing `sloth-framework-0.1.5/sloth/api/views.py` & `sloth-framework-0.1.6/sloth/api/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 # -*- coding: utf-8 -*-
 import json
 import base64
 import traceback
 from datetime import datetime
+
+from django.views import static
+
 from sloth import threadlocals
 from django.core.cache import cache
 from django.http import QueryDict
 from django.apps import apps
 from oauth2_provider.oauth2_backends import get_oauthlib_core
 from ..core.valueset import ValueSet
 from ..utils.http import ApiResponse
@@ -38,14 +41,18 @@
         response = func(request, *args, **kwargs)
         if threadlocals.transaction['diff']:
             print(json.dumps(threadlocals.transaction, ensure_ascii=False))
         return response
     return decorate
 
 
+def media(request, path):
+    return static.serve(request, path, document_root=settings.MEDIA_ROOT)
+
+
 @logger
 def app(request, path):
     if request.user.is_authenticated and settings.FORCE_PASSWORD_DEFINITION:
         default_password = settings.DEFAULT_PASSWORD(request.user)
         if request.user.check_password(default_password):
             messages.warning(request, 'Altere sua senha padrão')
             return HttpResponseRedirect('/app/dashboard/change_password/')
@@ -122,14 +129,17 @@
 def endpoint(func):
     def decorate(request, *args, **kwargs):
         try:
             if is_authenticated(request):
                 data = func(request, *args, **kwargs)
                 wrap = request.path.startswith('/meta')
                 serialized = data.serialize(wrap=wrap)
+                if request.path == '/meta/dashboard/':
+                    dashboard = Dashboards(request)
+                    serialized = dashboard.serialize(serialized)
                 # from pprint import pprint; pprint(serialized)
                 return ApiResponse(serialized, safe=False)
             else:
                 return ApiResponse(
                     dict(type='message', text='Usuário não autenticado', style='warning'), status=403
                 )
         except JsonReadyResponseException as e:
@@ -207,15 +217,15 @@
 def dispatcher(request, path):
     allowed_attrs = []
     extra_attrs = []
     instance = None
     instances = None
     instantiator = None
     queryset = None
-    tokens = path.split('/')
+    tokens = [token for token in path.split('/') if '=' not in token]
     token = tokens.pop(0)
     if token == 'dashboard':
         obj = Dashboards(request).main()
         if tokens:
             allowed_attrs = obj.view().get_allowed_attrs()
         else:
             obj = obj.view()
@@ -232,15 +242,15 @@
             raise PermissionDenied()
     else:
         raise PermissionDenied()
     for i, token in enumerate(tokens):
         if i == 0:
             allowed_attrs.extend(EXPOSE)
         if not request.user.is_authenticated and token not in allowed_attrs and token not in extra_attrs and not token.isdigit() and '-' not in token:
-            print(token, type(obj).__name__, allowed_attrs, extra_attrs)
+            # print(token, type(obj).__name__, allowed_attrs, extra_attrs)
             raise PermissionDenied()
         if token.isdigit():
             if isinstance(obj, Dashboard):
                 obj = obj.view()
             extra_attrs = obj.metadata['actions'] + obj.metadata['inline_actions'] + ['view' if view['name'] == 'self' else view['name'] for view in obj.metadata['view']]
             obj = obj.contextualize(request).apply_role_lookups(request.user).filter(pk=token).first()
             if obj:
@@ -259,15 +269,15 @@
         elif token in ACTIONS or token in ('add', 'edit', 'delete'):
             if token in ('edit', 'delete') and instance is None and instances is None:
                 raise PermissionDenied()
             if token == 'add' and isinstance(obj, QuerySet) and obj.metadata['related_field']:
                 form_cls = obj.model.relation_form_cls(obj.metadata['related_field'])
             else:
                 form_cls = obj.action_form_cls(token)
-            # print(dict(action=form_cls, instantiator=instantiator, instance=instance, instances=instances, queryset=queryset))
+            # print(token, dict(action=form_cls, instantiator=instantiator, instance=instance, instances=instances, queryset=queryset))
             form = form_cls(
                 request=request, instantiator=instantiator, instance=instance, instances=instances, queryset=queryset
             )
             if form.check_permission(request.user):
                 if form.is_valid():
                     result = form.process()
                     if result is not None and form.has_url_posted_data():
@@ -288,14 +298,17 @@
                 if isinstance(obj, ValueSet):
                     instantiator = obj.instance
                     obj = getattr(obj.instance, token)()
                 else:
                     instantiator = obj
                     obj = getattr(obj, token)()
                 if isinstance(obj, ValueSet):
-                    instance = instantiator
+                    instance = obj.instance
                 if isinstance(obj, QuerySet):
                     queryset = obj
                     if 'global_action' in request.GET:
                         queryset = obj.process_request(request, uuid=token).apply_role_lookups(request.user)
         allowed_attrs = obj.get_allowed_attrs()
-    return obj.contextualize(request).apply_role_lookups(request.user)
+    obj = obj.contextualize(request).apply_role_lookups(request.user)
+    if request.path.startswith('/api/') and isinstance(obj, QuerySet):
+        obj = obj.process_request(request)
+    return obj
```

### Comparing `sloth-framework-0.1.5/sloth/cloud/printer.py` & `sloth-framework-0.1.6/sloth/cloud/printer.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/cloud/server.py` & `sloth-framework-0.1.6/sloth/cloud/server.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/conf/settings.py` & `sloth-framework-0.1.6/sloth/conf/settings.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/core/base.py` & `sloth-framework-0.1.6/sloth/core/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,20 +51,21 @@
         return user.is_superuser or self.has_permission(user) or self.is_autouser(user)
 
     def has_attr_permission(self, user, name):
         attr = getattr(self, 'has_{}_permission'.format(name), None)
         return attr is None or user.is_superuser or attr(user)
 
     def has_view_attr_permission(self, user, name):
+        has_permission = False
         if user.is_superuser or self.has_permission(user):
-            return True
+            has_permission = True
         if self.is_view_attr(name) and self.has_view_permission(user):
-            return True
+            has_permission = True
         attr = getattr(self, 'has_{}_permission'.format(name), None)
-        return attr(user) if attr else False
+        return attr(user) if attr else has_permission
 
     def is_view_attr(self, name):
         if not hasattr(self.__class__, '__view__'):
             attr_names = []
 
             def append_attr_names(valueset):
                 names = list(valueset.metadata['names'].keys())
@@ -132,15 +133,16 @@
                     lookups.append(role['name'])
                 values = model.objects.filter(pk=self.pk).values(*set(lookups))
                 for value in values:
                     username = value[role['username']]
                     email = value[role['email']] if role['email'] else None
                     if username:
                         scope_name = value[role['name']] if role['name'].islower() else role['name']
-                        tuples.add((username, email, scope_name, None, None, None))
+                        if not role['scopes']:
+                            tuples.add((username, email, scope_name, None, None, None))
                         for scope_key, lookup in role['scopes'].items():
                             scope_type = model if lookup in ('pk', 'id', 'self') else model.get_field(lookup).related_model
                             scope_value = value[lookup]
                             tuples.add((username, email, scope_name, scope_type, scope_key, scope_value))
                     # else:
                     #     raise ValidationError('O "login" do usuário ({}) deve ser informado.'.format(role['username'].upper().replace('__', '->')))
         # print('----- {} -----'.format(self))
@@ -273,15 +275,15 @@
         _related_field = related_field
 
         class Add(Action):
             class Meta:
                 icon = 'plus'
                 modal = True
                 model = cls.get_field(_related_field).model
-                style = 'success'
+                style = 'primary'
                 related_field = _related_field
                 verbose_name = 'Adicionar {}'.format(cls.get_field(_related_field).model.metaclass().verbose_name)
                 fieldsets = getattr(cls.get_field(_related_field).model.metaclass(), 'fieldsets', None)
 
             def has_permission(self, user):
                 return user.is_superuser or self.instantiator.has_edit_permission(user) or self.instantiator.has_permission(user)
 
@@ -314,15 +316,15 @@
                 except FieldDoesNotExist:
                     pass
         return None
 
     @classmethod
     def default_list_fields(cls):
         list_display = getattr(cls.metaclass(), 'list_display', None)
-        return list_display or [field.name for field in cls.metaclass().fields[0:5] if field.name != 'id' and '_ptr' not in field.name]
+        return list_display or [field.name for field in cls.metaclass().fields[0:10] if field.name != 'id' and '_ptr' not in field.name]
 
     @classmethod
     def default_filter_fields(cls, exclude=None):
         filters = getattr(cls.metaclass(), 'list_filter', None)
         if filters is None:
             filters = []
             for field in cls.metaclass().fields:
```

### Comparing `sloth-framework-0.1.5/sloth/core/queryset.py` & `sloth-framework-0.1.6/sloth/core/queryset.py`

 * *Files 0% similar despite different names*

```diff
@@ -310,15 +310,15 @@
         field = self.model.get_field(filter_lookup)
         ids = self.apply_role_lookups(request.user).values_list(
             filter_lookup, flat=True
         ).order_by(filter_lookup).distinct()
         if field.null:
             items.append(dict(id='null', text='Indefinido'))
         if field.related_model:
-            qs = field.related_model.objects.filter(pk__in=ids)
+            qs = field.related_model.objects.all().filter(pk__in=ids)
             qs = qs.search(q=q) if q else qs
             total = 25
             items.extend([dict(id=value.id, text=str(value)) for value in qs[0:25]])
         else:
             total = ids.count()
             items.extend([dict(id=value, text=str(value)) for value in values])
         return dict(
@@ -402,15 +402,15 @@
             actions = self.get_obj_actions(obj)
             if self.request:
                 for view in self.metadata['view']:
                     if view['name'] == 'self':
                         has_view_permission = obj.has_view_permission(self.request.user)
                     else:
                         has_view_permission = obj.has_view_attr_permission(self.request.user, view['name'])
-                    if self.request.user.is_superuser or has_view_permission or obj.has_permission(self.request.user):
+                    if has_view_permission:
                         actions.append(view['name'])
             item = obj.value_set(*self.get_list_display(add_id=add_id)).contextualize(self.request).load(wrap=False, detail=detail)
             data.append(dict(id=obj.id, description=str(obj), data=item, actions=actions) if wrap else item)
         return data
 
     def export(self, limit=100):
         data = []
@@ -558,15 +558,15 @@
                 if template is None:
                     template = getattr(self.model.metaclass(), 'list_template', None)
                 if template:
                     template = template if template.endswith('.html') else '{}.html'.format(template)
                     data.update(template=template)
             # from pprint import pprint; pprint(data)
             return data
-        return self.to_list(detail=False)
+        return self.paginate().to_list(detail=False)
 
     def debug(self):
         print(json.dumps(self.serialize(wrap=True), indent=4, ensure_ascii=False))
 
     # metadata functions
 
     def admin(self):
@@ -827,15 +827,15 @@
         return super().__str__()
 
     # request functions
     def contextualize(self, request):
         self.request = request
         if request and request.user.is_superuser and 'autouser' in self.metadata['ignore']:
             self.metadata['ignore'].remove('autouser')
-        if request and self.metadata['uuid'] == request.GET.get('uuid'):
+        if request and self.metadata['uuid'] == request.GET.get('uuid'): #  or (request and request.path.startswith('/api/'))
             if 'choices' in request.GET:
                 raise JsonReadyResponseException(
                     self.process_request(request).choices(request)
                 )
             if 'tree-nodes' in request.GET:
                 raise JsonReadyResponseException(
                     self.process_request(request).tree_nodes()
```

### Comparing `sloth-framework-0.1.5/sloth/core/statistics.py` & `sloth-framework-0.1.6/sloth/core/statistics.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/core/validation.py` & `sloth-framework-0.1.6/sloth/core/validation.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/core/valueset.py` & `sloth-framework-0.1.6/sloth/core/valueset.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,15 +103,15 @@
 
     def attach(self, *names):
         self.metadata['attach'] = [to_snake_case(name) for name in names]
         return self
 
     def image(self, image):
         image_attr = getattr(self.instance, image)
-        self.metadata['image'] = image_attr() if callable(image_attr) else image_attr
+        self.metadata['image'] = (image_attr() if callable(image_attr) else image_attr) or '/static/images/no-image.png'
         return self
 
     def title(self, title):
         self.metadata['title'] = title
         return self
 
     def subtitle(self, subtitle):
@@ -247,15 +247,17 @@
                     if self.request and self.request.META.get('QUERY_STRING') and 'only' not in self.request.META.get('QUERY_STRING'):
                         path = '{}?{}'.format(path, self.request.META.get('QUERY_STRING').replace('?tab=1', ''))
                     if isinstance(value, QuerySet) or hasattr(value, '_queryset_class'):  # RelatedManager
                         qs = value if isinstance(value, QuerySet) else value.filter() # ManyRelatedManager
                         qs.instantiator = self.instance
                         qs.metadata['uuid'] = attr_name
                         qs.metadata['path'] = path
-                        verbose_name = getattr(attr, '__verbose_name__', qs.metadata['verbose_name'] or pretty(attr_name))
+                        verbose_name = getattr(attr, '__verbose_name__', qs.metadata['verbose_name'])
+                        if verbose_name is None:
+                            verbose_name = pretty(attr_name)
                         template = getattr(attr, '__template__', None)
                         template = 'renderers/{}.html'.format(template) if template else None
                         if self.request:
                             qs = qs.contextualize(self.request).apply_role_lookups(self.request.user)
                         if wrap:
                             if template or (self.metadata['primitive'] and deep > 0):
                                 data = dict(value=serialize(qs), width=width, type='primitive', path=path, template=template)
@@ -265,21 +267,25 @@
                         else:
                             if self.metadata['primitive']:  # one-to-many or many-to-many (and deep > 0)
                                 data = dict(value=serialize(qs), width=width, type='primitive', path=path, template=template)
                             else:
                                 data = qs.to_list(detail=False)
                     elif isinstance(value, QuerySetStatistics):
                         statistics = value
-                        verbose_name = getattr(attr, '__verbose_name__', statistics.metadata['verbose_name'] or pretty(attr_name))
+                        verbose_name = getattr(attr, '__verbose_name__', statistics.metadata['verbose_name'])
+                        if verbose_name is None:
+                            verbose_name = pretty(attr_name)
                         statistics.contextualize(self.request)
                         data = statistics.serialize(path=path, wrap=wrap, lazy=lazy)
                         data.update(name=verbose_name, key=attr_name) if wrap else None
                     elif isinstance(value, ValueSet):
                         valueset = value
-                        verbose_name = getattr(attr, '__verbose_name__', valueset.metadata['verbose_name'] or pretty(attr_name))
+                        verbose_name = getattr(attr, '__verbose_name__', valueset.metadata['verbose_name'])
+                        if verbose_name is None:
+                            verbose_name = pretty(attr_name)
                         valueset.contextualize(self.request)
                         value.metadata['printing'] = self.metadata['printing']
                         key = attr_name
                         inner_deep = 0 if self.metadata['attr'] or (deep==1 and i==0) else deep+1
                         valueset.path = path
                         valueset.load(wrap=wrap, detail=wrap or detail, deep=inner_deep)
                         if not valueset:
@@ -291,15 +297,15 @@
                         ) if wrap else valueset
                         if self.request and self.request.path.startswith('/app/'):
                             data.update(instance=valueset.instance)
                         if wrap:
                             for action_type in ('actions', 'inline_actions'):
                                 for form_name in valueset.metadata[action_type]:
                                     form_cls = self.instance.action_form_cls(form_name)
-                                    if form_cls.check_fake_permission(self.request, self.instance, self.instance):
+                                    if form_cls.check_fake_permission(self.request, valueset.instance, self.instance):
                                         data[action_type].append(form_cls.get_metadata(path))
                             data.update(path=path)
                             if valueset.metadata['image']:
                                 image = valueset.metadata['image']
                                 if image:
                                     image = str(image)
                                     if not image.startswith('/') and not image.startswith('http'):
```

### Comparing `sloth-framework-0.1.5/sloth/db/models/__init__.py` & `sloth-framework-0.1.6/sloth/db/models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,14 +124,24 @@
     def formfield(self, **kwargs):
         field = super().formfield(**kwargs)
         field.widget.mask = self.mask
         field.widget.rmask = self.rmask
         return field
 
 
+class BooleanChoiceField(BooleanField):
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+
+    def formfield(self, **kwargs):
+        from ...actions import BooleanChoiceField
+        kwargs.update(form_class=BooleanChoiceField)
+        return super().formfield(**kwargs)
+
+
 class BrCepField(CharField):
     def __init__(self, *args, **kwargs):
         kwargs.update(mask='00.000-000')
         super().__init__(*args, **kwargs)
 
 
 class BrCpfField(CharField):
@@ -345,7 +355,12 @@
                 )
 
     def __str__(self):
         for field in self.metaclass().fields:
             if isinstance(field, models.CharField):
                 return getattr(self, field.name)
         return '{} #{}'.format(self.metaclass().verbose_name, self.pk)
+
+
+    def send_mail(self, to, subject, content, from_email=None):
+        from sloth.api.models import Email
+        Email.objects.send(to, subject, content, from_email)
```

### Comparing `sloth-framework-0.1.5/sloth/test/__init__.py` & `sloth-framework-0.1.6/sloth/test/__init__.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/test/selenium/__init__.py` & `sloth-framework-0.1.6/sloth/test/selenium/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,14 +37,15 @@
         cls.browser.open('/')
         for app_label in settings.INSTALLED_APPS:
             app_module = __import__(app_label)
             app_dir = os.path.dirname(app_module.__file__)
             fixture_path = os.path.join(app_dir, 'fixtures', 'test.json')
             if os.path.exists(fixture_path):
                 call_command('loaddata', fixture_path)
+        settings.DEBUG = True
 
     def create_superuser(self, username, password):
         if not User.objects.filter(username=username).exists():
             User.objects.create_superuser(username, None, password)
 
     def wait(self, seconds=1):
         self.browser.wait(seconds)
```

### Comparing `sloth-framework-0.1.5/sloth/test/selenium/browser.py` & `sloth-framework-0.1.6/sloth/test/selenium/browser.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,18 +85,16 @@
         try:
             if submit:
                 self.execute_script("enter('{}', '{}', 1)".format(name, value))
             else:
                 self.execute_script("enter('{}', '{}')".format(name, value))
                 elements = self.find_elements(By.NAME, 'hidden-upload-value')
                 for element in elements:
-                    element_id, file_path = element.get_property('value').split(':')
-                    if file_path.startswith('/static'):
-                        file_path = '{}/{}/{}'.format(settings.BASE_DIR, settings.PROJECT_NAME, file_path)
-                    self.find_element(By.ID, element_id).send_keys(file_path)
+                    self.find_element(By.ID, element.get_property('value')).send_keys(os.path.join(settings.BASE_DIR, value))
+                    return
         except WebDriverException as e:
             if count:
                 self.wait()
                 self.enter(name, value, submit, count - 1)
             else:
                 self.watch(e)
         if self.slowly:
```

### Comparing `sloth-framework-0.1.5/sloth/utils/__init__.py` & `sloth-framework-0.1.6/sloth/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/utils/formatter/__init__.py` & `sloth-framework-0.1.6/sloth/utils/formatter/__init__.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/utils/http/__init__.py` & `sloth-framework-0.1.6/sloth/utils/http/__init__.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/utils/icons/bootstrap.py` & `sloth-framework-0.1.6/sloth/utils/icons/bootstrap.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/utils/icons/fontawesome.py` & `sloth-framework-0.1.6/sloth/utils/icons/fontawesome.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/utils/icons/materialicons.py` & `sloth-framework-0.1.6/sloth/utils/icons/materialicons.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth/utils/log/sql.py` & `sloth-framework-0.1.6/sloth/utils/log/sql.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.5/sloth_framework.egg-info/PKG-INFO` & `sloth-framework-0.1.6/sloth_framework.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sloth-framework
-Version: 0.1.5
+Version: 0.1.6
 Summary: Metadata-based web framework for the development of management information systems
 Home-page: http://sloth.aplicativo.click/
 Author: Breno Silva
 Author-email: brenokcc@yahoo.com.br
 License: BSD License
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

### Comparing `sloth-framework-0.1.5/sloth_framework.egg-info/SOURCES.txt` & `sloth-framework-0.1.6/sloth_framework.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -40,26 +40,32 @@
 sloth/api/migrations/0012_authcode.py
 sloth/api/migrations/0013_task_partial_task_total.py
 sloth/api/migrations/0014_email.py
 sloth/api/migrations/__init__.py
 sloth/api/static/css/all.min.css
 sloth/api/static/css/bootstrap-icons.css
 sloth/api/static/css/bootstrap.min.css
+sloth/api/static/css/bpmn.css
 sloth/api/static/css/colorpick.min.css
 sloth/api/static/css/icons.svg
 sloth/api/static/css/jquery-ui.css
 sloth/api/static/css/leaflet.css
 sloth/api/static/css/select2.min.css
 sloth/api/static/css/sloth.css
 sloth/api/static/css/trumbowyg.min.css
 sloth/api/static/css/fonts/Eina02-Bold.f8011405.ttf
 sloth/api/static/css/fonts/Eina02-Regular.2e682693.ttf
 sloth/api/static/css/fonts/Eina02-SemiBold.c5f9b8e3.ttf
 sloth/api/static/css/fonts/bootstrap-icons.woff
 sloth/api/static/css/fonts/bootstrap-icons.woff2
+sloth/api/static/css/fonts/bpmn.eot
+sloth/api/static/css/fonts/bpmn.svg
+sloth/api/static/css/fonts/bpmn.ttf
+sloth/api/static/css/fonts/bpmn.woff
+sloth/api/static/css/fonts/bpmn.woff2
 sloth/api/static/css/images/ui-icons_444444_256x240.png
 sloth/api/static/css/images/ui-icons_555555_256x240.png
 sloth/api/static/icons/fontawesome/fontawesome.min.css
 sloth/api/static/icons/fontawesome/fontawesome.min.js
 sloth/api/static/icons/fontawesome/webfonts/fa-brands-400.ttf
 sloth/api/static/icons/fontawesome/webfonts/fa-brands-400.woff2
 sloth/api/static/icons/fontawesome/webfonts/fa-regular-400.ttf
@@ -81,14 +87,15 @@
 sloth/api/static/images/no-image.png
 sloth/api/static/images/sloth.png
 sloth/api/static/images/user.png
 sloth/api/static/images/images/badge.png
 sloth/api/static/images/images/icon.png
 sloth/api/static/js/api.js
 sloth/api/static/js/bootstrap.bundle.min.js
+sloth/api/static/js/bpmn.js
 sloth/api/static/js/colorpick.min.js
 sloth/api/static/js/jquery-3.6.0.min.js
 sloth/api/static/js/jquery-ui.js
 sloth/api/static/js/jquery.binarytransport.js
 sloth/api/static/js/jquery.mask.min.js
 sloth/api/static/js/jquery.timepicker.js
 sloth/api/static/js/leaflet.js
@@ -104,14 +111,15 @@
 sloth/api/static/js/trumbowyg.min.js
 sloth/api/static/js/wpn.js
 sloth/api/static/js/i18n/pt-BR.js
 sloth/api/tasks/__init__.py
 sloth/api/templates/actions/execute_query.html
 sloth/api/templates/actions/execute_script.html
 sloth/api/templates/actions/show_icons.html
+sloth/api/templates/actions/workflow.html
 sloth/api/templates/api/index.html
 sloth/api/templates/charts/bar.html
 sloth/api/templates/charts/column.html
 sloth/api/templates/charts/donut.html
 sloth/api/templates/charts/legend.html
 sloth/api/templates/charts/pie.html
 sloth/api/templates/dashboard/actions.html
@@ -162,14 +170,15 @@
 sloth/api/templates/renderers/badges/status.html
 sloth/api/templates/renderers/badges/warning.html
 sloth/api/templates/renderers/boolean/thumb.html
 sloth/api/templates/renderers/calendar/calendar.html
 sloth/api/templates/renderers/calendar/events.html
 sloth/api/templates/renderers/calendar/legend.html
 sloth/api/templates/renderers/documents/document.html
+sloth/api/templates/renderers/documents/popup.html
 sloth/api/templates/renderers/images/banner.html
 sloth/api/templates/renderers/images/group.html
 sloth/api/templates/renderers/images/image.html
 sloth/api/templates/renderers/images/round.html
 sloth/api/templates/renderers/links/file.html
 sloth/api/templates/renderers/links/url.html
 sloth/api/templates/renderers/maps/geolocation.html
@@ -182,14 +191,15 @@
 sloth/api/templates/renderers/messages/warning.html
 sloth/api/templates/renderers/photos/photo.html
 sloth/api/templates/renderers/photos/round.html
 sloth/api/templates/renderers/programing/strtable.html
 sloth/api/templates/renderers/programing/terminal.html
 sloth/api/templates/renderers/progress/primary.html
 sloth/api/templates/renderers/progress/success.html
+sloth/api/templates/renderers/steps/check.html
 sloth/api/templates/renderers/tags/primary.html
 sloth/api/templates/renderers/tags/tags.html
 sloth/api/templates/renderers/utils/formatted.html
 sloth/api/templates/renderers/utils/progress.html
 sloth/api/templates/renderers/utils/qrcode.html
 sloth/api/templates/renderers/utils/steps.html
 sloth/api/templates/renderers/utils/table.html
@@ -205,14 +215,15 @@
 sloth/api/templates/valueset/valueset.html
 sloth/api/templatetags/__init__.py
 sloth/api/templatetags/tags.py
 sloth/cloud/__init__.py
 sloth/cloud/printer.py
 sloth/cloud/server.py
 sloth/conf/__init__.py
+sloth/conf/local_settings.py
 sloth/conf/settings.py
 sloth/core/__init__.py
 sloth/core/base.py
 sloth/core/queryset.py
 sloth/core/statistics.py
 sloth/core/validation.py
 sloth/core/valueset.py
```

