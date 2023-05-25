# Comparing `tmp/vstutils-5.4.7.tar.gz` & `tmp/vstutils-5.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vstutils-5.4.7.tar", last modified: Thu May 25 05:01:23 2023, max compression
+gzip compressed data, was "vstutils-5.4.8.tar", last modified: Thu May 25 15:50:43 2023, max compression
```

## Comparing `vstutils-5.4.7.tar` & `vstutils-5.4.8.tar`

### file list

```diff
@@ -1,252 +1,252 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 05:01:23.735427 vstutils-5.4.7/
--rw-rw-rw-   0 root         (0) root         (0)    11344 2022-12-19 05:37:08.000000 vstutils-5.4.7/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)      770 2023-05-24 07:40:20.000000 vstutils-5.4.7/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)      592 2023-05-24 07:40:20.000000 vstutils-5.4.7/NOTICE
--rw-r--r--   0 root         (0) root         (0)     4459 2023-05-25 05:01:23.735427 vstutils-5.4.7/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2393 2023-05-24 07:40:20.000000 vstutils-5.4.7/README.rst
--rw-rw-rw-   0 root         (0) root         (0)      237 2023-05-25 00:37:14.000000 vstutils-5.4.7/requirements-doc.txt
--rw-rw-rw-   0 root         (0) root         (0)       85 2022-12-19 05:37:08.000000 vstutils-5.4.7/requirements-git.txt
--rw-rw-rw-   0 root         (0) root         (0)       51 2022-12-19 05:37:08.000000 vstutils-5.4.7/requirements-ldap.txt
--rw-rw-rw-   0 root         (0) root         (0)      185 2023-05-24 07:40:20.000000 vstutils-5.4.7/requirements-prod.txt
--rw-rw-rw-   0 root         (0) root         (0)       83 2023-05-24 07:40:20.000000 vstutils-5.4.7/requirements-rpc.txt
--rw-rw-rw-   0 root         (0) root         (0)      231 2023-05-24 07:40:20.000000 vstutils-5.4.7/requirements-stubs.txt
--rw-rw-rw-   0 root         (0) root         (0)      135 2023-05-24 07:40:20.000000 vstutils-5.4.7/requirements-test.txt
--rw-rw-rw-   0 root         (0) root         (0)      538 2023-05-24 07:40:20.000000 vstutils-5.4.7/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)     2313 2023-05-25 05:01:23.735427 vstutils-5.4.7/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)    16893 2023-05-24 07:40:20.000000 vstutils-5.4.7/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 05:01:23.695427 vstutils-5.4.7/vstutils/
--rw-rw-rw-   0 root         (0) root         (0)       66 2023-05-25 04:31:45.000000 vstutils-5.4.7/vstutils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      158 2022-12-19 05:37:08.000000 vstutils-5.4.7/vstutils/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 05:01:23.703427 vstutils-5.4.7/vstutils/api/
--rw-rw-rw-   0 root         (0) root         (0)      176 2022-12-19 05:37:08.000000 vstutils-5.4.7/vstutils/api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15370 2023-05-24 07:40:20.000000 vstutils-5.4.7/vstutils/api/actions.py
--rw-rw-rw-   0 root         (0) root         (0)     1492 2023-05-24 07:40:20.000000 vstutils-5.4.7/vstutils/api/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      413 2022-12-19 05:37:08.000000 vstutils-5.4.7/vstutils/api/apps.py
--rw-rw-rw-   0 root         (0) root         (0)    13063 2023-05-24 07:40:20.000000 vstutils-5.4.7/vstutils/api/auth.py
--rw-rw-rw-   0 root         (0) root         (0)    28141 2023-05-25 04:31:45.000000 vstutils-5.4.7/vstutils/api/base.py
--rw-rw-rw-   0 root         (0) root         (0)    24054 2023-05-24 21:58:37.000000 vstutils-5.4.7/vstutils/api/decorators.py
--rw-rw-rw-   0 root         (0) root         (0)     6672 2023-05-24 07:40:20.000000 vstutils-5.4.7/vstutils/api/decorators.pyi
--rw-rw-rw-   0 root         (0) root         (0)    15852 2023-05-24 07:40:20.000000 vstutils-5.4.7/vstutils/api/doc_generator.py
--rw-rw-rw-   0 root         (0) root         (0)    18802 2023-05-24 07:40:20.000000 vstutils-5.4.7/vstutils/api/endpoint.py
--rw-rw-rw-   0 root         (0) root         (0)    51728 2023-05-24 21:58:37.000000 vstutils-5.4.7/vstutils/api/fields.py
--rw-rw-rw-   0 root         (0) root         (0)    11754 2023-05-24 07:40:20.000000 vstutils-5.4.7/vstutils/api/filter_backends.py
--rw-rw-rw-   0 root         (0) root         (0)     4991 2023-05-24 21:58:37.000000 vstutils-5.4.7/vstutils/api/filters.py
--rw-rw-rw-   0 root         (0) root         (0)     2531 2022-12-19 05:37:08.000000 vstutils-5.4.7/vstutils/api/health.py
--rw-rw-rw-   0 root         (0) root         (0)      574 2022-12-19 05:37:08.000000 vstutils-5.4.7/vstutils/api/meta.py
--rw-rw-rw-   0 root         (0) root         (0)     4230 2023-05-24 07:40:20.000000 vstutils-5.4.7/vstutils/api/metrics.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 05:01:23.703427 vstutils-5.4.7/vstutils/api/migrations/
--rw-rw-rw-   0 root         (0) root         (0)      554 2022-12-19 05:37:08.000000 vstutils-5.4.7/vstutils/api/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)     1285 2022-12-19 05:37:08.000000 vstutils-5.4.7/vstutils/api/migrations/0002_two_factor.py
--rw-rw-rw-   0 root         (0) root         (0)      598 2022-12-19 05:37:08.000000 vstutils-5.4.7/vstutils/api/migrations/0003_tfa_indexes.py
--rw-rw-rw-   0 root         (0) root         (0)     1348 2022-12-19 05:37:08.000000 vstutils-5.4.7/vstutils/api/migrations/0004_user_settings.py
--rw-rw-rw-   0 root         (0) root         (0)      866 2022-12-19 05:37:08.000000 vstutils-5.4.7/vstutils/api/migrations/0005_db_translations.py
--rw-rw-rw-   0 root         (0) root         (0)      698 2022-12-19 05:37:08.000000 vstutils-5.4.7/vstutils/api/migrations/0006_fix_user_settings.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:37:08.000000 vstutils-5.4.7/vstutils/api/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4591 2023-05-24 07:40:20.000000 vstutils-5.4.7/vstutils/api/models.py
--rw-rw-rw-   0 root         (0) root         (0)      869 2022-12-19 05:37:08.000000 vstutils-5.4.7/vstutils/api/pagination.py
--rw-rw-rw-   0 root         (0) root         (0)      812 2022-12-19 05:37:08.000000 vstutils-5.4.7/vstutils/api/parsers.py
--rw-rw-rw-   0 root         (0) root         (0)     1509 2023-05-24 07:40:20.000000 vstutils-5.4.7/vstutils/api/permissions.py
--rw-rw-rw-   0 root         (0) root         (0)     1596 2022-12-19 05:37:08.000000 vstutils-5.4.7/vstutils/api/renderers.py
--rw-rw-rw-   0 root         (0) root         (0)     1090 2023-05-24 07:40:20.000000 vstutils-5.4.7/vstutils/api/responses.py
--rw-rw-rw-   0 root         (0) root         (0)    10364 2022-12-19 05:37:08.000000 vstutils-5.4.7/vstutils/api/responses.pyi
--rw-rw-rw-   0 root         (0) root         (0)     9015 2023-05-24 07:40:20.000000 vstutils-5.4.7/vstutils/api/routers.py
--rw-rw-rw-   0 root         (0) root         (0)     1998 2023-05-24 07:40:20.000000 vstutils-5.4.7/vstutils/api/routers.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 05:01:23.703427 vstutils-5.4.7/vstutils/api/schema/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:37:08.000000 vstutils-5.4.7/vstutils/api/schema/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5850 2023-05-24 07:40:20.000000 vstutils-5.4.7/vstutils/api/schema/generators.py
--rw-rw-rw-   0 root         (0) root         (0)     1649 2023-05-24 07:40:20.000000 vstutils-5.4.7/vstutils/api/schema/info.py
--rw-rw-rw-   0 root         (0) root         (0)    26465 2023-05-24 07:40:20.000000 vstutils-5.4.7/vstutils/api/schema/inspectors.py
--rw-rw-rw-   0 root         (0) root         (0)     9648 2023-05-24 07:40:20.000000 vstutils-5.4.7/vstutils/api/schema/schema.py
--rw-rw-rw-   0 root         (0) root         (0)      253 2022-12-19 05:37:08.000000 vstutils-5.4.7/vstutils/api/schema/views.py
--rw-rw-rw-   0 root         (0) root         (0)     7340 2023-05-24 21:58:37.000000 vstutils-5.4.7/vstutils/api/serializers.py
--rw-rw-rw-   0 root         (0) root         (0)     2289 2023-05-24 07:40:20.000000 vstutils-5.4.7/vstutils/api/throttling.py
--rw-rw-rw-   0 root         (0) root         (0)    10784 2023-05-24 21:58:37.000000 vstutils-5.4.7/vstutils/api/validators.py
--rw-rw-rw-   0 root         (0) root         (0)     5660 2023-05-24 07:40:20.000000 vstutils-5.4.7/vstutils/api/views.py
--rw-rw-rw-   0 root         (0) root         (0)      255 2023-05-24 07:40:20.000000 vstutils-5.4.7/vstutils/api/views.pyi
--rw-rw-rw-   0 root         (0) root         (0)     1363 2023-05-24 07:40:20.000000 vstutils-5.4.7/vstutils/asgi.py
--rw-rw-rw-   0 root         (0) root         (0)     1744 2023-05-24 07:40:20.000000 vstutils-5.4.7/vstutils/asgi_worker.py
--rw-rw-rw-   0 root         (0) root         (0)     4232 2023-05-24 07:40:20.000000 vstutils-5.4.7/vstutils/auth.py
--rw-rw-rw-   0 root         (0) root         (0)     2162 2023-05-24 07:40:20.000000 vstutils-5.4.7/vstutils/auth.pyi
--rw-rw-rw-   0 root         (0) root         (0)     2790 2023-05-24 07:40:20.000000 vstutils-5.4.7/vstutils/celery_beat_scheduler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 05:01:23.683427 vstutils-5.4.7/vstutils/doc_themes/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 05:01:23.703427 vstutils-5.4.7/vstutils/doc_themes/vst-sphinx-theme/
--rw-rw-rw-   0 root         (0) root         (0)      927 2022-12-19 05:37:08.000000 vstutils-5.4.7/vstutils/doc_themes/vst-sphinx-theme/layout.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 05:01:23.707427 vstutils-5.4.7/vstutils/doc_themes/vst-sphinx-theme/static/
--rw-rw-rw-   0 root         (0) root         (0)      172 2023-05-25 05:01:23.743428 vstutils-5.4.7/vstutils/doc_themes/vst-sphinx-theme/static/basic.css
--rw-rw-rw-   0 root         (0) root         (0)      147 2022-12-19 05:37:08.000000 vstutils-5.4.7/vstutils/doc_themes/vst-sphinx-theme/theme.conf
--rw-rw-rw-   0 root         (0) root         (0)     2387 2023-05-24 07:40:20.000000 vstutils-5.4.7/vstutils/environment.py
--rw-rw-rw-   0 root         (0) root         (0)      355 2022-12-19 05:37:08.000000 vstutils-5.4.7/vstutils/environment.pyi
--rw-rw-rw-   0 root         (0) root         (0)      743 2022-12-19 05:37:08.000000 vstutils-5.4.7/vstutils/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 05:01:23.707427 vstutils-5.4.7/vstutils/gui/
--rwxrwxrwx   0 root         (0) root         (0)        0 2022-12-19 05:37:08.000000 vstutils-5.4.7/vstutils/gui/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3467 2023-05-25 04:31:45.000000 vstutils-5.4.7/vstutils/gui/context.py
--rw-rw-rw-   0 root         (0) root         (0)     7501 2023-05-24 07:40:20.000000 vstutils-5.4.7/vstutils/gui/forms.py
--rw-rw-rw-   0 root         (0) root         (0)     1026 2022-12-19 05:37:08.000000 vstutils-5.4.7/vstutils/gui/pwa_manifest.py
--rw-rw-rw-   0 root         (0) root         (0)     5023 2023-05-24 07:40:20.000000 vstutils-5.4.7/vstutils/gui/views.py
--rw-rw-rw-   0 root         (0) root         (0)     6436 2022-12-19 05:37:08.000000 vstutils-5.4.7/vstutils/ldap_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 05:01:23.707427 vstutils-5.4.7/vstutils/management/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:37:08.000000 vstutils-5.4.7/vstutils/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 05:01:23.707427 vstutils-5.4.7/vstutils/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:37:08.000000 vstutils-5.4.7/vstutils/management/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7832 2023-05-24 07:40:20.000000 vstutils-5.4.7/vstutils/management/commands/_base.py
--rw-rw-rw-   0 root         (0) root         (0)     1344 2023-05-24 07:40:20.000000 vstutils-5.4.7/vstutils/management/commands/celery_inspect.py
--rw-rw-rw-   0 root         (0) root         (0)      367 2022-12-19 05:37:08.000000 vstutils-5.4.7/vstutils/management/commands/dockermigrate.py
--rw-rw-rw-   0 root         (0) root         (0)     1167 2022-12-19 05:37:08.000000 vstutils-5.4.7/vstutils/management/commands/dockerrun.py
--rw-rw-rw-   0 root         (0) root         (0)     4975 2023-05-24 07:40:20.000000 vstutils-5.4.7/vstutils/management/commands/newproject.py
--rw-rw-rw-   0 root         (0) root         (0)     1670 2022-12-19 05:37:08.000000 vstutils-5.4.7/vstutils/management/commands/run_task.py
--rw-rw-rw-   0 root         (0) root         (0)     1165 2023-05-24 07:40:20.000000 vstutils-5.4.7/vstutils/management/commands/runrpc.py
--rw-rw-rw-   0 root         (0) root         (0)     1639 2023-05-24 07:40:20.000000 vstutils-5.4.7/vstutils/management/commands/runserver.py
--rw-rw-rw-   0 root         (0) root         (0)     7286 2023-05-24 07:40:20.000000 vstutils-5.4.7/vstutils/management/commands/web.py
--rw-rw-rw-   0 root         (0) root         (0)    10646 2023-05-24 07:40:20.000000 vstutils-5.4.7/vstutils/middleware.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 05:01:23.711427 vstutils-5.4.7/vstutils/models/
--rw-rw-rw-   0 root         (0) root         (0)    10704 2023-05-24 21:58:37.000000 vstutils-5.4.7/vstutils/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    25308 2023-05-24 07:40:20.000000 vstutils-5.4.7/vstutils/models/base.py
--rw-rw-rw-   0 root         (0) root         (0)     4130 2023-05-24 07:40:20.000000 vstutils-5.4.7/vstutils/models/cent_notify.py
--rw-rw-rw-   0 root         (0) root         (0)    11620 2023-05-24 07:40:20.000000 vstutils-5.4.7/vstutils/models/custom_model.py
--rw-rw-rw-   0 root         (0) root         (0)     2534 2023-05-24 07:40:20.000000 vstutils-5.4.7/vstutils/models/custom_model.pyi
--rw-rw-rw-   0 root         (0) root         (0)     2344 2022-12-19 05:37:08.000000 vstutils-5.4.7/vstutils/models/decorators.py
--rw-rw-rw-   0 root         (0) root         (0)     7971 2023-05-24 21:58:37.000000 vstutils-5.4.7/vstutils/models/fields.py
--rw-rw-rw-   0 root         (0) root         (0)      293 2022-12-19 05:37:08.000000 vstutils-5.4.7/vstutils/models/model.py
--rw-rw-rw-   0 root         (0) root         (0)     8200 2023-05-24 07:40:20.000000 vstutils-5.4.7/vstutils/models/queryset.py
--rw-rw-rw-   0 root         (0) root         (0)       64 2022-12-19 05:37:08.000000 vstutils-5.4.7/vstutils/py.typed
--rw-rw-rw-   0 root         (0) root         (0)      472 2022-12-19 05:37:08.000000 vstutils-5.4.7/vstutils/session.py
--rw-rw-rw-   0 root         (0) root         (0)     4270 2022-12-19 05:37:08.000000 vstutils-5.4.7/vstutils/settings.ini
--rw-rw-rw-   0 root         (0) root         (0)    54947 2023-05-24 07:40:20.000000 vstutils-5.4.7/vstutils/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 05:01:23.687427 vstutils-5.4.7/vstutils/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 05:01:23.719427 vstutils-5.4.7/vstutils/static/bundle/
--rw-r--r--   0 root         (0) root         (0)      155 2023-05-25 05:00:17.000000 vstutils-5.4.7/vstutils/static/bundle/157.chunk.js
--rw-r--r--   0 root         (0) root         (0)   126295 2023-05-25 05:00:17.000000 vstutils-5.4.7/vstutils/static/bundle/281.chunk.js
--rw-r--r--   0 root         (0) root         (0)      171 2023-05-25 05:00:17.000000 vstutils-5.4.7/vstutils/static/bundle/281.chunk.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)     1553 2023-05-25 05:00:17.000000 vstutils-5.4.7/vstutils/static/bundle/296.chunk.js
--rw-r--r--   0 root         (0) root         (0)      151 2023-05-25 05:00:17.000000 vstutils-5.4.7/vstutils/static/bundle/296.chunk.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)   136100 2023-05-25 05:00:17.000000 vstutils-5.4.7/vstutils/static/bundle/345.chunk.js
--rw-r--r--   0 root         (0) root         (0)    15726 2023-05-25 05:00:17.000000 vstutils-5.4.7/vstutils/static/bundle/368.chunk.js
--rw-r--r--   0 root         (0) root         (0)  1066719 2023-05-25 05:00:17.000000 vstutils-5.4.7/vstutils/static/bundle/421.js
--rw-r--r--   0 root         (0) root         (0)     1500 2023-05-25 05:00:17.000000 vstutils-5.4.7/vstutils/static/bundle/421.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      321 2023-05-25 05:00:17.000000 vstutils-5.4.7/vstutils/static/bundle/463.chunk.js
--rw-r--r--   0 root         (0) root         (0)      330 2023-05-25 05:00:17.000000 vstutils-5.4.7/vstutils/static/bundle/564.chunk.js
--rw-r--r--   0 root         (0) root         (0)    38336 2023-05-25 05:00:17.000000 vstutils-5.4.7/vstutils/static/bundle/618.js
--rw-r--r--   0 root         (0) root         (0)       93 2023-05-25 05:00:17.000000 vstutils-5.4.7/vstutils/static/bundle/618.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)     2235 2023-05-25 05:00:17.000000 vstutils-5.4.7/vstutils/static/bundle/683.chunk.js
--rw-r--r--   0 root         (0) root         (0)      151 2023-05-25 05:00:17.000000 vstutils-5.4.7/vstutils/static/bundle/683.chunk.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)    71086 2023-05-25 05:00:17.000000 vstutils-5.4.7/vstutils/static/bundle/686.js
--rw-r--r--   0 root         (0) root         (0)   536206 2023-05-25 05:00:17.000000 vstutils-5.4.7/vstutils/static/bundle/742.chunk.js
--rw-r--r--   0 root         (0) root         (0)     1142 2023-05-25 05:00:17.000000 vstutils-5.4.7/vstutils/static/bundle/742.chunk.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)    89997 2023-05-25 05:00:17.000000 vstutils-5.4.7/vstutils/static/bundle/755.js
--rw-r--r--   0 root         (0) root         (0)      476 2023-05-25 05:00:17.000000 vstutils-5.4.7/vstutils/static/bundle/755.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)   355788 2023-05-25 05:00:17.000000 vstutils-5.4.7/vstutils/static/bundle/826.chunk.js
--rw-r--r--   0 root         (0) root         (0)     1142 2023-05-25 05:00:17.000000 vstutils-5.4.7/vstutils/static/bundle/826.chunk.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)   177828 2023-05-25 05:00:17.000000 vstutils-5.4.7/vstutils/static/bundle/844.js
--rw-r--r--   0 root         (0) root         (0)  1798980 2023-05-25 05:00:17.000000 vstutils-5.4.7/vstutils/static/bundle/959.js
--rw-r--r--   0 root         (0) root         (0)     2191 2023-05-25 05:00:17.000000 vstutils-5.4.7/vstutils/static/bundle/959.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)    77026 2023-05-25 05:00:17.000000 vstutils-5.4.7/vstutils/static/bundle/app_loader.js
--rw-r--r--   0 root         (0) root         (0)   303656 2023-05-25 05:00:17.000000 vstutils-5.4.7/vstutils/static/bundle/base.js
--rw-r--r--   0 root         (0) root         (0)    16276 2023-05-25 05:00:17.000000 vstutils-5.4.7/vstutils/static/bundle/bb58e57c48a3e911f15f.woff
--rw-r--r--   0 root         (0) root         (0)   101648 2023-05-25 05:00:17.000000 vstutils-5.4.7/vstutils/static/bundle/eeccf4f66002c6f2ba24.woff
--rw-r--r--   0 root         (0) root         (0)      748 2023-05-25 05:01:23.000000 vstutils-5.4.7/vstutils/static/bundle/output.json
--rw-r--r--   0 root         (0) root         (0)     3597 2023-05-25 05:00:17.000000 vstutils-5.4.7/vstutils/static/bundle/spa.js
--rw-r--r--   0 root         (0) root         (0)   432611 2023-05-25 05:00:17.000000 vstutils-5.4.7/vstutils/static/bundle/vstutils.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 05:01:23.719427 vstutils-5.4.7/vstutils/static/img/
--rw-rw-rw-   0 root         (0) root         (0)     1323 2022-12-19 05:37:08.000000 vstutils-5.4.7/vstutils/static/img/anonymous.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 05:01:23.723427 vstutils-5.4.7/vstutils/static/img/logo/
--rw-rw-rw-   0 root         (0) root         (0)      384 2022-12-19 05:37:08.000000 vstutils-5.4.7/vstutils/static/img/logo/favicon.ico
--rw-rw-rw-   0 root         (0) root         (0)     2203 2023-05-24 07:40:20.000000 vstutils-5.4.7/vstutils/static_files.py
--rw-rw-rw-   0 root         (0) root         (0)     5181 2023-05-24 21:58:37.000000 vstutils-5.4.7/vstutils/tasks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 05:01:23.723427 vstutils-5.4.7/vstutils/templates/
--rw-rw-rw-   0 root         (0) root         (0)      262 2023-05-24 07:40:20.000000 vstutils-5.4.7/vstutils/templates/400.html
--rw-rw-rw-   0 root         (0) root         (0)      230 2023-05-24 07:40:20.000000 vstutils-5.4.7/vstutils/templates/403.html
--rw-rw-rw-   0 root         (0) root         (0)      227 2023-05-24 07:40:20.000000 vstutils-5.4.7/vstutils/templates/404.html
--rw-rw-rw-   0 root         (0) root         (0)      183 2023-05-24 07:40:20.000000 vstutils-5.4.7/vstutils/templates/500.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 05:01:23.723427 vstutils-5.4.7/vstutils/templates/auth/
--rwxrwxrwx   0 root         (0) root         (0)     2568 2022-12-19 05:37:08.000000 vstutils-5.4.7/vstutils/templates/auth/base.html
--rw-rw-rw-   0 root         (0) root         (0)      729 2022-12-19 05:37:08.000000 vstutils-5.4.7/vstutils/templates/auth/language_selector.html
--rw-rw-rw-   0 root         (0) root         (0)       30 2022-12-19 05:37:08.000000 vstutils-5.4.7/vstutils/templates/auth/login.html
--rw-rw-rw-   0 root         (0) root         (0)     1240 2022-12-19 05:37:08.000000 vstutils-5.4.7/vstutils/templates/auth/tfa.html
--rwxrwxrwx   0 root         (0) root         (0)     2845 2023-02-21 07:56:30.000000 vstutils-5.4.7/vstutils/templates/base.html
--rw-rw-rw-   0 root         (0) root         (0)      313 2023-05-24 07:40:20.000000 vstutils-5.4.7/vstutils/templates/base_error.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 05:01:23.723427 vstutils-5.4.7/vstutils/templates/configs/
--rw-rw-rw-   0 root         (0) root         (0)       76 2022-12-19 05:37:08.000000 vstutils-5.4.7/vstutils/templates/configs/config.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 05:01:23.723427 vstutils-5.4.7/vstutils/templates/drf-yasg/
--rw-rw-rw-   0 root         (0) root         (0)      134 2022-12-19 05:37:08.000000 vstutils-5.4.7/vstutils/templates/drf-yasg/swagger-ui.html
--rw-rw-rw-   0 root         (0) root         (0)      434 2023-05-24 07:40:20.000000 vstutils-5.4.7/vstutils/templates/go_back_button.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 05:01:23.723427 vstutils-5.4.7/vstutils/templates/gui/
--rw-rw-rw-   0 root         (0) root         (0)     1482 2022-12-19 05:37:08.000000 vstutils-5.4.7/vstutils/templates/gui/base.html
--rwxrwxrwx   0 root         (0) root         (0)       29 2022-12-19 05:37:08.000000 vstutils-5.4.7/vstutils/templates/gui/gui.html
--rw-rw-rw-   0 root         (0) root         (0)      154 2022-12-19 05:37:08.000000 vstutils-5.4.7/vstutils/templates/gui/manifest.json
--rw-rw-rw-   0 root         (0) root         (0)     1731 2022-12-19 05:37:08.000000 vstutils-5.4.7/vstutils/templates/gui/offline.html
--rw-rw-rw-   0 root         (0) root         (0)     1531 2022-12-19 05:37:08.000000 vstutils-5.4.7/vstutils/templates/gui/service-worker.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 05:01:23.727427 vstutils-5.4.7/vstutils/templates/newproject/
--rw-rw-rw-   0 root         (0) root         (0)      280 2022-12-19 05:37:08.000000 vstutils-5.4.7/vstutils/templates/newproject/.coveragerc.template
--rw-rw-rw-   0 root         (0) root         (0)     2290 2022-12-19 05:37:08.000000 vstutils-5.4.7/vstutils/templates/newproject/.gitignore.template
--rw-rw-rw-   0 root         (0) root         (0)      235 2022-12-19 05:37:08.000000 vstutils-5.4.7/vstutils/templates/newproject/.pep8.template
--rw-rw-rw-   0 root         (0) root         (0)      210 2022-12-19 05:37:08.000000 vstutils-5.4.7/vstutils/templates/newproject/MANIFEST.in.template
--rw-rw-rw-   0 root         (0) root         (0)      445 2022-12-19 05:37:08.000000 vstutils-5.4.7/vstutils/templates/newproject/README.rst.template
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 05:01:23.727427 vstutils-5.4.7/vstutils/templates/newproject/frontend_src/
--rw-rw-rw-   0 root         (0) root         (0)      123 2022-12-19 05:37:08.000000 vstutils-5.4.7/vstutils/templates/newproject/frontend_src/.babelrc.js.template
--rw-rw-rw-   0 root         (0) root         (0)      157 2022-12-19 05:37:08.000000 vstutils-5.4.7/vstutils/templates/newproject/frontend_src/.editorconfig.template
--rw-rw-rw-   0 root         (0) root         (0)      794 2022-12-19 05:37:08.000000 vstutils-5.4.7/vstutils/templates/newproject/frontend_src/.eslintrc.js.template
--rw-rw-rw-   0 root         (0) root         (0)      449 2022-12-19 05:37:08.000000 vstutils-5.4.7/vstutils/templates/newproject/frontend_src/.prettierrc.template
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 05:01:23.727427 vstutils-5.4.7/vstutils/templates/newproject/frontend_src/app/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:37:08.000000 vstutils-5.4.7/vstutils/templates/newproject/frontend_src/app/index.js.template
--rw-rw-rw-   0 root         (0) root         (0)     1078 2022-12-19 05:37:08.000000 vstutils-5.4.7/vstutils/templates/newproject/package.json.template
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 05:01:23.731428 vstutils-5.4.7/vstutils/templates/newproject/project_name/
--rw-rw-rw-   0 root         (0) root         (0)      496 2022-12-19 05:37:08.000000 vstutils-5.4.7/vstutils/templates/newproject/project_name/__init__.py.template
--rw-rw-rw-   0 root         (0) root         (0)      115 2022-12-19 05:37:08.000000 vstutils-5.4.7/vstutils/templates/newproject/project_name/__main__.py.template
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 05:01:23.731428 vstutils-5.4.7/vstutils/templates/newproject/project_name/models/
--rw-rw-rw-   0 root         (0) root         (0)       92 2022-12-19 05:37:08.000000 vstutils-5.4.7/vstutils/templates/newproject/project_name/models/__init__.py.template
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:37:08.000000 vstutils-5.4.7/vstutils/templates/newproject/project_name/settings.ini.template
--rw-rw-rw-   0 root         (0) root         (0)      565 2022-12-19 05:37:08.000000 vstutils-5.4.7/vstutils/templates/newproject/project_name/settings.py.template
--rw-rw-rw-   0 root         (0) root         (0)       66 2022-12-19 05:37:08.000000 vstutils-5.4.7/vstutils/templates/newproject/project_name/web.ini.template
--rw-rw-rw-   0 root         (0) root         (0)      120 2022-12-19 05:37:08.000000 vstutils-5.4.7/vstutils/templates/newproject/project_name/wsgi.py.template
--rw-rw-rw-   0 root         (0) root         (0)       75 2022-12-19 05:37:08.000000 vstutils-5.4.7/vstutils/templates/newproject/requirements-test.txt.template
--rw-rw-rw-   0 root         (0) root         (0)      101 2022-12-19 05:37:08.000000 vstutils-5.4.7/vstutils/templates/newproject/requirements.txt.template
--rw-rw-rw-   0 root         (0) root         (0)     1073 2023-05-24 07:40:20.000000 vstutils-5.4.7/vstutils/templates/newproject/setup.cfg.template
--rw-rw-rw-   0 root         (0) root         (0)    14520 2023-05-24 07:40:20.000000 vstutils-5.4.7/vstutils/templates/newproject/setup.py.template
--rw-rw-rw-   0 root         (0) root         (0)      572 2022-12-19 05:37:08.000000 vstutils-5.4.7/vstutils/templates/newproject/test.py.template
--rw-rw-rw-   0 root         (0) root         (0)     2234 2023-05-24 07:40:20.000000 vstutils-5.4.7/vstutils/templates/newproject/tox.ini.template
--rw-rw-rw-   0 root         (0) root         (0)      705 2022-12-19 05:37:08.000000 vstutils-5.4.7/vstutils/templates/newproject/tox_build.ini.template
--rw-rw-rw-   0 root         (0) root         (0)     2262 2022-12-19 05:37:08.000000 vstutils-5.4.7/vstutils/templates/newproject/webpack.config.js.default.template
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 05:01:23.731428 vstutils-5.4.7/vstutils/templates/registration/
--rw-rw-rw-   0 root         (0) root         (0)       57 2022-12-19 05:37:08.000000 vstutils-5.4.7/vstutils/templates/registration/base.html
--rw-rw-rw-   0 root         (0) root         (0)      459 2022-12-19 05:37:08.000000 vstutils-5.4.7/vstutils/templates/registration/base_agreements.html
--rw-rw-rw-   0 root         (0) root         (0)    11731 2023-05-24 07:40:20.000000 vstutils-5.4.7/vstutils/templates/registration/confirm_email.html
--rw-rw-rw-   0 root         (0) root         (0)      352 2022-12-19 05:37:08.000000 vstutils-5.4.7/vstutils/templates/registration/password_reset_complete.html
--rw-rw-rw-   0 root         (0) root         (0)     1618 2022-12-19 05:37:08.000000 vstutils-5.4.7/vstutils/templates/registration/password_reset_confirm.html
--rw-rw-rw-   0 root         (0) root         (0)      463 2022-12-19 05:37:08.000000 vstutils-5.4.7/vstutils/templates/registration/password_reset_done.html
--rw-rw-rw-   0 root         (0) root         (0)      831 2022-12-19 05:37:08.000000 vstutils-5.4.7/vstutils/templates/registration/password_reset_form.html
--rw-rw-rw-   0 root         (0) root         (0)     1736 2022-12-19 05:37:08.000000 vstutils-5.4.7/vstutils/templates/registration/user_registration.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 05:01:23.731428 vstutils-5.4.7/vstutils/templates/rest_framework/
--rw-rw-rw-   0 root         (0) root         (0)     9228 2022-12-19 05:37:08.000000 vstutils-5.4.7/vstutils/templates/rest_framework/admin.html
--rw-rw-rw-   0 root         (0) root         (0)      225 2022-12-19 05:37:08.000000 vstutils-5.4.7/vstutils/templates/rest_framework/api.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 05:01:23.731428 vstutils-5.4.7/vstutils/templates/vst_inclusion_tags/
--rw-rw-rw-   0 root         (0) root         (0)      107 2022-12-19 05:37:08.000000 vstutils-5.4.7/vstutils/templates/vst_inclusion_tags/b64_img_from_json_string.html
--rw-rw-rw-   0 root         (0) root         (0)      834 2022-12-19 05:37:08.000000 vstutils-5.4.7/vstutils/templates/vst_inclusion_tags/bootstrap_form.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 05:01:23.731428 vstutils-5.4.7/vstutils/templates/widgets/
--rw-rw-rw-   0 root         (0) root         (0)     1405 2022-12-19 05:37:08.000000 vstutils-5.4.7/vstutils/templates/widgets/agreement_widget.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 05:01:23.735427 vstutils-5.4.7/vstutils/templatetags/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:37:08.000000 vstutils-5.4.7/vstutils/templatetags/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1482 2023-05-24 07:40:20.000000 vstutils-5.4.7/vstutils/templatetags/request_static.py
--rw-rw-rw-   0 root         (0) root         (0)     2866 2022-12-19 05:37:08.000000 vstutils-5.4.7/vstutils/templatetags/translation.py
--rw-rw-rw-   0 root         (0) root         (0)      823 2022-12-19 05:37:08.000000 vstutils-5.4.7/vstutils/templatetags/vst_gravatar.py
--rw-rw-rw-   0 root         (0) root         (0)     2107 2023-05-24 07:40:20.000000 vstutils-5.4.7/vstutils/templatetags/vst_html_tags.py
--rw-rw-rw-   0 root         (0) root         (0)     1133 2022-12-19 05:37:08.000000 vstutils-5.4.7/vstutils/templatetags/vstconfigs.py
--rw-rw-rw-   0 root         (0) root         (0)    17731 2023-05-24 21:58:37.000000 vstutils-5.4.7/vstutils/tests.py
--rw-rw-rw-   0 root         (0) root         (0)      612 2022-12-19 05:37:08.000000 vstutils-5.4.7/vstutils/tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 05:01:23.735427 vstutils-5.4.7/vstutils/translations/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:37:08.000000 vstutils-5.4.7/vstutils/translations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    16196 2023-05-24 07:40:20.000000 vstutils-5.4.7/vstutils/translations/cn.py
--rw-rw-rw-   0 root         (0) root         (0)      420 2022-12-19 05:37:08.000000 vstutils-5.4.7/vstutils/translations/en.py
--rw-rw-rw-   0 root         (0) root         (0)    23941 2023-05-24 07:40:20.000000 vstutils-5.4.7/vstutils/translations/ru.py
--rw-rw-rw-   0 root         (0) root         (0)    18983 2023-05-24 07:40:20.000000 vstutils-5.4.7/vstutils/translations/vi.py
--rw-rw-rw-   0 root         (0) root         (0)     2721 2023-05-24 07:40:20.000000 vstutils-5.4.7/vstutils/urls.py
--rw-rw-rw-   0 root         (0) root         (0)    44730 2023-05-24 21:58:37.000000 vstutils-5.4.7/vstutils/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1482 2023-05-24 07:40:20.000000 vstutils-5.4.7/vstutils/web.ini
--rw-rw-rw-   0 root         (0) root         (0)      843 2022-12-19 05:37:08.000000 vstutils-5.4.7/vstutils/wsgi.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 05:01:23.695427 vstutils-5.4.7/vstutils.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4459 2023-05-25 05:01:23.000000 vstutils-5.4.7/vstutils.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7644 2023-05-25 05:01:23.000000 vstutils-5.4.7/vstutils.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       85 2023-05-25 05:01:23.000000 vstutils-5.4.7/vstutils.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       64 2023-05-25 05:01:23.000000 vstutils-5.4.7/vstutils.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 05:00:17.000000 vstutils-5.4.7/vstutils.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)     1941 2023-05-25 05:01:23.000000 vstutils-5.4.7/vstutils.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-05-25 05:01:23.000000 vstutils-5.4.7/vstutils.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 15:50:43.759326 vstutils-5.4.8/
+-rw-rw-rw-   0 root         (0) root         (0)    11344 2022-12-19 05:43:06.000000 vstutils-5.4.8/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)      770 2023-02-03 10:03:13.000000 vstutils-5.4.8/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)      592 2023-03-29 01:47:58.000000 vstutils-5.4.8/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     4459 2023-05-25 15:50:43.759326 vstutils-5.4.8/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2393 2022-12-19 05:43:06.000000 vstutils-5.4.8/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)      237 2023-05-25 10:44:35.000000 vstutils-5.4.8/requirements-doc.txt
+-rw-rw-rw-   0 root         (0) root         (0)       85 2022-12-19 05:43:06.000000 vstutils-5.4.8/requirements-git.txt
+-rw-rw-rw-   0 root         (0) root         (0)       51 2022-12-19 05:43:06.000000 vstutils-5.4.8/requirements-ldap.txt
+-rw-rw-rw-   0 root         (0) root         (0)      185 2023-05-13 04:11:10.000000 vstutils-5.4.8/requirements-prod.txt
+-rw-rw-rw-   0 root         (0) root         (0)       83 2023-03-18 02:33:32.000000 vstutils-5.4.8/requirements-rpc.txt
+-rw-rw-rw-   0 root         (0) root         (0)      231 2023-03-29 01:47:58.000000 vstutils-5.4.8/requirements-stubs.txt
+-rw-rw-rw-   0 root         (0) root         (0)      135 2023-05-13 04:11:10.000000 vstutils-5.4.8/requirements-test.txt
+-rw-rw-rw-   0 root         (0) root         (0)      538 2023-05-13 04:11:10.000000 vstutils-5.4.8/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)     2313 2023-05-25 15:50:43.759326 vstutils-5.4.8/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)    16893 2023-04-13 03:48:29.000000 vstutils-5.4.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 15:50:43.715326 vstutils-5.4.8/vstutils/
+-rw-rw-rw-   0 root         (0) root         (0)       66 2023-05-25 10:44:35.000000 vstutils-5.4.8/vstutils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      158 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 15:50:43.723326 vstutils-5.4.8/vstutils/api/
+-rw-rw-rw-   0 root         (0) root         (0)      176 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15370 2023-02-03 10:03:13.000000 vstutils-5.4.8/vstutils/api/actions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1492 2023-02-03 10:03:13.000000 vstutils-5.4.8/vstutils/api/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      413 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/api/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)    13063 2023-02-06 06:25:26.000000 vstutils-5.4.8/vstutils/api/auth.py
+-rw-rw-rw-   0 root         (0) root         (0)    28141 2023-05-25 10:44:35.000000 vstutils-5.4.8/vstutils/api/base.py
+-rw-rw-rw-   0 root         (0) root         (0)    24054 2023-05-25 10:44:35.000000 vstutils-5.4.8/vstutils/api/decorators.py
+-rw-rw-rw-   0 root         (0) root         (0)     6672 2023-02-03 10:03:13.000000 vstutils-5.4.8/vstutils/api/decorators.pyi
+-rw-rw-rw-   0 root         (0) root         (0)    15852 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/api/doc_generator.py
+-rw-rw-rw-   0 root         (0) root         (0)    18802 2023-02-07 05:18:57.000000 vstutils-5.4.8/vstutils/api/endpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)    51728 2023-05-25 10:44:35.000000 vstutils-5.4.8/vstutils/api/fields.py
+-rw-rw-rw-   0 root         (0) root         (0)    11754 2023-05-13 04:11:10.000000 vstutils-5.4.8/vstutils/api/filter_backends.py
+-rw-rw-rw-   0 root         (0) root         (0)     4991 2023-05-25 10:44:35.000000 vstutils-5.4.8/vstutils/api/filters.py
+-rw-rw-rw-   0 root         (0) root         (0)     2531 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/api/health.py
+-rw-rw-rw-   0 root         (0) root         (0)      574 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/api/meta.py
+-rw-rw-rw-   0 root         (0) root         (0)     4230 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/api/metrics.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 15:50:43.723326 vstutils-5.4.8/vstutils/api/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)      554 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/api/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)     1285 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/api/migrations/0002_two_factor.py
+-rw-rw-rw-   0 root         (0) root         (0)      598 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/api/migrations/0003_tfa_indexes.py
+-rw-rw-rw-   0 root         (0) root         (0)     1348 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/api/migrations/0004_user_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)      866 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/api/migrations/0005_db_translations.py
+-rw-rw-rw-   0 root         (0) root         (0)      698 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/api/migrations/0006_fix_user_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/api/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4591 2023-02-06 06:25:26.000000 vstutils-5.4.8/vstutils/api/models.py
+-rw-rw-rw-   0 root         (0) root         (0)      869 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/api/pagination.py
+-rw-rw-rw-   0 root         (0) root         (0)      812 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/api/parsers.py
+-rw-rw-rw-   0 root         (0) root         (0)     1509 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/api/permissions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1596 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/api/renderers.py
+-rw-rw-rw-   0 root         (0) root         (0)     1090 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/api/responses.py
+-rw-rw-rw-   0 root         (0) root         (0)    10364 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/api/responses.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     9015 2023-02-06 06:25:26.000000 vstutils-5.4.8/vstutils/api/routers.py
+-rw-rw-rw-   0 root         (0) root         (0)     1998 2023-02-03 10:03:13.000000 vstutils-5.4.8/vstutils/api/routers.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 15:50:43.723326 vstutils-5.4.8/vstutils/api/schema/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/api/schema/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5850 2023-02-06 06:25:26.000000 vstutils-5.4.8/vstutils/api/schema/generators.py
+-rw-rw-rw-   0 root         (0) root         (0)     1649 2023-02-03 10:03:13.000000 vstutils-5.4.8/vstutils/api/schema/info.py
+-rw-rw-rw-   0 root         (0) root         (0)    26465 2023-03-17 01:28:59.000000 vstutils-5.4.8/vstutils/api/schema/inspectors.py
+-rw-rw-rw-   0 root         (0) root         (0)     9648 2023-02-06 06:25:26.000000 vstutils-5.4.8/vstutils/api/schema/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)      253 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/api/schema/views.py
+-rw-rw-rw-   0 root         (0) root         (0)     7340 2023-05-25 10:44:35.000000 vstutils-5.4.8/vstutils/api/serializers.py
+-rw-rw-rw-   0 root         (0) root         (0)     2289 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/api/throttling.py
+-rw-rw-rw-   0 root         (0) root         (0)    10784 2023-05-25 10:44:35.000000 vstutils-5.4.8/vstutils/api/validators.py
+-rw-rw-rw-   0 root         (0) root         (0)     5660 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/api/views.py
+-rw-rw-rw-   0 root         (0) root         (0)      255 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/api/views.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     1363 2023-02-20 07:13:28.000000 vstutils-5.4.8/vstutils/asgi.py
+-rw-rw-rw-   0 root         (0) root         (0)     1744 2023-02-13 06:24:20.000000 vstutils-5.4.8/vstutils/asgi_worker.py
+-rw-rw-rw-   0 root         (0) root         (0)     4232 2023-02-06 06:25:26.000000 vstutils-5.4.8/vstutils/auth.py
+-rw-rw-rw-   0 root         (0) root         (0)     2162 2023-02-06 06:25:26.000000 vstutils-5.4.8/vstutils/auth.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     2790 2023-02-06 06:25:26.000000 vstutils-5.4.8/vstutils/celery_beat_scheduler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 15:50:43.703326 vstutils-5.4.8/vstutils/doc_themes/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 15:50:43.727326 vstutils-5.4.8/vstutils/doc_themes/vst-sphinx-theme/
+-rw-rw-rw-   0 root         (0) root         (0)      927 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/doc_themes/vst-sphinx-theme/layout.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 15:50:43.727326 vstutils-5.4.8/vstutils/doc_themes/vst-sphinx-theme/static/
+-rw-rw-rw-   0 root         (0) root         (0)      172 2023-05-25 15:50:43.763326 vstutils-5.4.8/vstutils/doc_themes/vst-sphinx-theme/static/basic.css
+-rw-rw-rw-   0 root         (0) root         (0)      147 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/doc_themes/vst-sphinx-theme/theme.conf
+-rw-rw-rw-   0 root         (0) root         (0)     2387 2023-02-03 10:03:13.000000 vstutils-5.4.8/vstutils/environment.py
+-rw-rw-rw-   0 root         (0) root         (0)      355 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/environment.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      743 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 15:50:43.727326 vstutils-5.4.8/vstutils/gui/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/gui/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3467 2023-05-25 10:44:35.000000 vstutils-5.4.8/vstutils/gui/context.py
+-rw-rw-rw-   0 root         (0) root         (0)     7501 2023-02-06 06:25:26.000000 vstutils-5.4.8/vstutils/gui/forms.py
+-rw-rw-rw-   0 root         (0) root         (0)     1026 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/gui/pwa_manifest.py
+-rw-rw-rw-   0 root         (0) root         (0)     5023 2023-02-06 06:25:26.000000 vstutils-5.4.8/vstutils/gui/views.py
+-rw-rw-rw-   0 root         (0) root         (0)     6436 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/ldap_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 15:50:43.727326 vstutils-5.4.8/vstutils/management/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 15:50:43.727326 vstutils-5.4.8/vstutils/management/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/management/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7832 2023-03-16 06:05:23.000000 vstutils-5.4.8/vstutils/management/commands/_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1344 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/management/commands/celery_inspect.py
+-rw-rw-rw-   0 root         (0) root         (0)      367 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/management/commands/dockermigrate.py
+-rw-rw-rw-   0 root         (0) root         (0)     1167 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/management/commands/dockerrun.py
+-rw-rw-rw-   0 root         (0) root         (0)     4975 2023-02-06 06:25:26.000000 vstutils-5.4.8/vstutils/management/commands/newproject.py
+-rw-rw-rw-   0 root         (0) root         (0)     1670 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/management/commands/run_task.py
+-rw-rw-rw-   0 root         (0) root         (0)     1165 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/management/commands/runrpc.py
+-rw-rw-rw-   0 root         (0) root         (0)     1639 2023-03-17 01:28:59.000000 vstutils-5.4.8/vstutils/management/commands/runserver.py
+-rw-rw-rw-   0 root         (0) root         (0)     7286 2023-02-06 06:25:26.000000 vstutils-5.4.8/vstutils/management/commands/web.py
+-rw-rw-rw-   0 root         (0) root         (0)    10646 2023-02-13 06:24:20.000000 vstutils-5.4.8/vstutils/middleware.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 15:50:43.731326 vstutils-5.4.8/vstutils/models/
+-rw-rw-rw-   0 root         (0) root         (0)    10704 2023-05-25 10:44:35.000000 vstutils-5.4.8/vstutils/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    25308 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/models/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     4130 2023-02-06 06:25:26.000000 vstutils-5.4.8/vstutils/models/cent_notify.py
+-rw-rw-rw-   0 root         (0) root         (0)    11620 2023-02-03 10:03:13.000000 vstutils-5.4.8/vstutils/models/custom_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     2534 2023-02-06 06:25:26.000000 vstutils-5.4.8/vstutils/models/custom_model.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     2344 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/models/decorators.py
+-rw-rw-rw-   0 root         (0) root         (0)     7971 2023-05-25 10:44:35.000000 vstutils-5.4.8/vstutils/models/fields.py
+-rw-rw-rw-   0 root         (0) root         (0)      293 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/models/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     8200 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/models/queryset.py
+-rw-rw-rw-   0 root         (0) root         (0)       64 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)      472 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/session.py
+-rw-rw-rw-   0 root         (0) root         (0)     4270 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/settings.ini
+-rw-rw-rw-   0 root         (0) root         (0)    54947 2023-04-13 03:48:29.000000 vstutils-5.4.8/vstutils/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 15:50:43.703326 vstutils-5.4.8/vstutils/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 15:50:43.743326 vstutils-5.4.8/vstutils/static/bundle/
+-rw-r--r--   0 root         (0) root         (0)      155 2023-05-25 15:49:30.000000 vstutils-5.4.8/vstutils/static/bundle/157.chunk.js
+-rw-r--r--   0 root         (0) root         (0)   126295 2023-05-25 15:49:30.000000 vstutils-5.4.8/vstutils/static/bundle/281.chunk.js
+-rw-r--r--   0 root         (0) root         (0)      171 2023-05-25 15:49:30.000000 vstutils-5.4.8/vstutils/static/bundle/281.chunk.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)     1553 2023-05-25 15:49:30.000000 vstutils-5.4.8/vstutils/static/bundle/296.chunk.js
+-rw-r--r--   0 root         (0) root         (0)      151 2023-05-25 15:49:30.000000 vstutils-5.4.8/vstutils/static/bundle/296.chunk.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)   136100 2023-05-25 15:49:30.000000 vstutils-5.4.8/vstutils/static/bundle/345.chunk.js
+-rw-r--r--   0 root         (0) root         (0)    15726 2023-05-25 15:49:30.000000 vstutils-5.4.8/vstutils/static/bundle/368.chunk.js
+-rw-r--r--   0 root         (0) root         (0)  1066719 2023-05-25 15:49:30.000000 vstutils-5.4.8/vstutils/static/bundle/421.js
+-rw-r--r--   0 root         (0) root         (0)     1500 2023-05-25 15:49:30.000000 vstutils-5.4.8/vstutils/static/bundle/421.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      321 2023-05-25 15:49:30.000000 vstutils-5.4.8/vstutils/static/bundle/463.chunk.js
+-rw-r--r--   0 root         (0) root         (0)      330 2023-05-25 15:49:30.000000 vstutils-5.4.8/vstutils/static/bundle/564.chunk.js
+-rw-r--r--   0 root         (0) root         (0)    38336 2023-05-25 15:49:30.000000 vstutils-5.4.8/vstutils/static/bundle/618.js
+-rw-r--r--   0 root         (0) root         (0)       93 2023-05-25 15:49:30.000000 vstutils-5.4.8/vstutils/static/bundle/618.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)     2235 2023-05-25 15:49:30.000000 vstutils-5.4.8/vstutils/static/bundle/683.chunk.js
+-rw-r--r--   0 root         (0) root         (0)      151 2023-05-25 15:49:30.000000 vstutils-5.4.8/vstutils/static/bundle/683.chunk.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)    71086 2023-05-25 15:49:30.000000 vstutils-5.4.8/vstutils/static/bundle/686.js
+-rw-r--r--   0 root         (0) root         (0)   536206 2023-05-25 15:49:30.000000 vstutils-5.4.8/vstutils/static/bundle/742.chunk.js
+-rw-r--r--   0 root         (0) root         (0)     1142 2023-05-25 15:49:30.000000 vstutils-5.4.8/vstutils/static/bundle/742.chunk.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)    89997 2023-05-25 15:49:30.000000 vstutils-5.4.8/vstutils/static/bundle/755.js
+-rw-r--r--   0 root         (0) root         (0)      476 2023-05-25 15:49:30.000000 vstutils-5.4.8/vstutils/static/bundle/755.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)   355788 2023-05-25 15:49:30.000000 vstutils-5.4.8/vstutils/static/bundle/826.chunk.js
+-rw-r--r--   0 root         (0) root         (0)     1142 2023-05-25 15:49:30.000000 vstutils-5.4.8/vstutils/static/bundle/826.chunk.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)   177828 2023-05-25 15:49:30.000000 vstutils-5.4.8/vstutils/static/bundle/844.js
+-rw-r--r--   0 root         (0) root         (0)  1798980 2023-05-25 15:49:30.000000 vstutils-5.4.8/vstutils/static/bundle/959.js
+-rw-r--r--   0 root         (0) root         (0)     2191 2023-05-25 15:49:30.000000 vstutils-5.4.8/vstutils/static/bundle/959.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)    77026 2023-05-25 15:49:30.000000 vstutils-5.4.8/vstutils/static/bundle/app_loader.js
+-rw-r--r--   0 root         (0) root         (0)   303656 2023-05-25 15:49:30.000000 vstutils-5.4.8/vstutils/static/bundle/base.js
+-rw-r--r--   0 root         (0) root         (0)    16276 2023-05-25 15:49:30.000000 vstutils-5.4.8/vstutils/static/bundle/bb58e57c48a3e911f15f.woff
+-rw-r--r--   0 root         (0) root         (0)   101648 2023-05-25 15:49:30.000000 vstutils-5.4.8/vstutils/static/bundle/eeccf4f66002c6f2ba24.woff
+-rw-r--r--   0 root         (0) root         (0)      748 2023-05-25 15:50:43.000000 vstutils-5.4.8/vstutils/static/bundle/output.json
+-rw-r--r--   0 root         (0) root         (0)     3597 2023-05-25 15:49:30.000000 vstutils-5.4.8/vstutils/static/bundle/spa.js
+-rw-r--r--   0 root         (0) root         (0)   432625 2023-05-25 15:49:30.000000 vstutils-5.4.8/vstutils/static/bundle/vstutils.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 15:50:43.743326 vstutils-5.4.8/vstutils/static/img/
+-rw-rw-rw-   0 root         (0) root         (0)     1323 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/static/img/anonymous.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 15:50:43.743326 vstutils-5.4.8/vstutils/static/img/logo/
+-rw-rw-rw-   0 root         (0) root         (0)      384 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/static/img/logo/favicon.ico
+-rw-rw-rw-   0 root         (0) root         (0)     2203 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/static_files.py
+-rw-rw-rw-   0 root         (0) root         (0)     5181 2023-05-25 10:44:35.000000 vstutils-5.4.8/vstutils/tasks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 15:50:43.743326 vstutils-5.4.8/vstutils/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      262 2023-02-21 08:49:07.000000 vstutils-5.4.8/vstutils/templates/400.html
+-rw-rw-rw-   0 root         (0) root         (0)      230 2023-02-21 08:49:07.000000 vstutils-5.4.8/vstutils/templates/403.html
+-rw-rw-rw-   0 root         (0) root         (0)      227 2023-02-21 08:49:07.000000 vstutils-5.4.8/vstutils/templates/404.html
+-rw-rw-rw-   0 root         (0) root         (0)      183 2023-02-21 08:00:17.000000 vstutils-5.4.8/vstutils/templates/500.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 15:50:43.743326 vstutils-5.4.8/vstutils/templates/auth/
+-rwxrwxrwx   0 root         (0) root         (0)     2568 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/templates/auth/base.html
+-rw-rw-rw-   0 root         (0) root         (0)      729 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/templates/auth/language_selector.html
+-rw-rw-rw-   0 root         (0) root         (0)       30 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/templates/auth/login.html
+-rw-rw-rw-   0 root         (0) root         (0)     1240 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/templates/auth/tfa.html
+-rwxrwxrwx   0 root         (0) root         (0)     2845 2023-02-21 08:00:17.000000 vstutils-5.4.8/vstutils/templates/base.html
+-rw-rw-rw-   0 root         (0) root         (0)      313 2023-02-21 06:43:08.000000 vstutils-5.4.8/vstutils/templates/base_error.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 15:50:43.747326 vstutils-5.4.8/vstutils/templates/configs/
+-rw-rw-rw-   0 root         (0) root         (0)       76 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/templates/configs/config.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 15:50:43.747326 vstutils-5.4.8/vstutils/templates/drf-yasg/
+-rw-rw-rw-   0 root         (0) root         (0)      134 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/templates/drf-yasg/swagger-ui.html
+-rw-rw-rw-   0 root         (0) root         (0)      434 2023-02-21 08:49:07.000000 vstutils-5.4.8/vstutils/templates/go_back_button.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 15:50:43.747326 vstutils-5.4.8/vstutils/templates/gui/
+-rw-rw-rw-   0 root         (0) root         (0)     1482 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/templates/gui/base.html
+-rwxrwxrwx   0 root         (0) root         (0)       29 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/templates/gui/gui.html
+-rw-rw-rw-   0 root         (0) root         (0)      154 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/templates/gui/manifest.json
+-rw-rw-rw-   0 root         (0) root         (0)     1731 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/templates/gui/offline.html
+-rw-rw-rw-   0 root         (0) root         (0)     1531 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/templates/gui/service-worker.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 15:50:43.751326 vstutils-5.4.8/vstutils/templates/newproject/
+-rw-rw-rw-   0 root         (0) root         (0)      280 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/templates/newproject/.coveragerc.template
+-rw-rw-rw-   0 root         (0) root         (0)     2290 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/templates/newproject/.gitignore.template
+-rw-rw-rw-   0 root         (0) root         (0)      235 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/templates/newproject/.pep8.template
+-rw-rw-rw-   0 root         (0) root         (0)      210 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/templates/newproject/MANIFEST.in.template
+-rw-rw-rw-   0 root         (0) root         (0)      445 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/templates/newproject/README.rst.template
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 15:50:43.751326 vstutils-5.4.8/vstutils/templates/newproject/frontend_src/
+-rw-rw-rw-   0 root         (0) root         (0)      123 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/templates/newproject/frontend_src/.babelrc.js.template
+-rw-rw-rw-   0 root         (0) root         (0)      157 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/templates/newproject/frontend_src/.editorconfig.template
+-rw-rw-rw-   0 root         (0) root         (0)      794 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/templates/newproject/frontend_src/.eslintrc.js.template
+-rw-rw-rw-   0 root         (0) root         (0)      449 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/templates/newproject/frontend_src/.prettierrc.template
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 15:50:43.751326 vstutils-5.4.8/vstutils/templates/newproject/frontend_src/app/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/templates/newproject/frontend_src/app/index.js.template
+-rw-rw-rw-   0 root         (0) root         (0)     1078 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/templates/newproject/package.json.template
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 15:50:43.751326 vstutils-5.4.8/vstutils/templates/newproject/project_name/
+-rw-rw-rw-   0 root         (0) root         (0)      496 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/templates/newproject/project_name/__init__.py.template
+-rw-rw-rw-   0 root         (0) root         (0)      115 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/templates/newproject/project_name/__main__.py.template
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 15:50:43.751326 vstutils-5.4.8/vstutils/templates/newproject/project_name/models/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/templates/newproject/project_name/models/__init__.py.template
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/templates/newproject/project_name/settings.ini.template
+-rw-rw-rw-   0 root         (0) root         (0)      565 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/templates/newproject/project_name/settings.py.template
+-rw-rw-rw-   0 root         (0) root         (0)       66 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/templates/newproject/project_name/web.ini.template
+-rw-rw-rw-   0 root         (0) root         (0)      120 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/templates/newproject/project_name/wsgi.py.template
+-rw-rw-rw-   0 root         (0) root         (0)       75 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/templates/newproject/requirements-test.txt.template
+-rw-rw-rw-   0 root         (0) root         (0)      101 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/templates/newproject/requirements.txt.template
+-rw-rw-rw-   0 root         (0) root         (0)     1073 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/templates/newproject/setup.cfg.template
+-rw-rw-rw-   0 root         (0) root         (0)    14520 2022-12-19 06:05:53.000000 vstutils-5.4.8/vstutils/templates/newproject/setup.py.template
+-rw-rw-rw-   0 root         (0) root         (0)      572 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/templates/newproject/test.py.template
+-rw-rw-rw-   0 root         (0) root         (0)     2234 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/templates/newproject/tox.ini.template
+-rw-rw-rw-   0 root         (0) root         (0)      705 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/templates/newproject/tox_build.ini.template
+-rw-rw-rw-   0 root         (0) root         (0)     2262 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/templates/newproject/webpack.config.js.default.template
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 15:50:43.755326 vstutils-5.4.8/vstutils/templates/registration/
+-rw-rw-rw-   0 root         (0) root         (0)       57 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/templates/registration/base.html
+-rw-rw-rw-   0 root         (0) root         (0)      459 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/templates/registration/base_agreements.html
+-rw-rw-rw-   0 root         (0) root         (0)    11731 2022-12-29 11:28:36.000000 vstutils-5.4.8/vstutils/templates/registration/confirm_email.html
+-rw-rw-rw-   0 root         (0) root         (0)      352 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/templates/registration/password_reset_complete.html
+-rw-rw-rw-   0 root         (0) root         (0)     1618 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/templates/registration/password_reset_confirm.html
+-rw-rw-rw-   0 root         (0) root         (0)      463 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/templates/registration/password_reset_done.html
+-rw-rw-rw-   0 root         (0) root         (0)      831 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/templates/registration/password_reset_form.html
+-rw-rw-rw-   0 root         (0) root         (0)     1736 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/templates/registration/user_registration.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 15:50:43.755326 vstutils-5.4.8/vstutils/templates/rest_framework/
+-rw-rw-rw-   0 root         (0) root         (0)     9228 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/templates/rest_framework/admin.html
+-rw-rw-rw-   0 root         (0) root         (0)      225 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/templates/rest_framework/api.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 15:50:43.755326 vstutils-5.4.8/vstutils/templates/vst_inclusion_tags/
+-rw-rw-rw-   0 root         (0) root         (0)      107 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/templates/vst_inclusion_tags/b64_img_from_json_string.html
+-rw-rw-rw-   0 root         (0) root         (0)      834 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/templates/vst_inclusion_tags/bootstrap_form.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 15:50:43.755326 vstutils-5.4.8/vstutils/templates/widgets/
+-rw-rw-rw-   0 root         (0) root         (0)     1405 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/templates/widgets/agreement_widget.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 15:50:43.755326 vstutils-5.4.8/vstutils/templatetags/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/templatetags/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1482 2023-02-03 10:03:13.000000 vstutils-5.4.8/vstutils/templatetags/request_static.py
+-rw-rw-rw-   0 root         (0) root         (0)     2866 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/templatetags/translation.py
+-rw-rw-rw-   0 root         (0) root         (0)      823 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/templatetags/vst_gravatar.py
+-rw-rw-rw-   0 root         (0) root         (0)     2107 2023-02-03 10:03:13.000000 vstutils-5.4.8/vstutils/templatetags/vst_html_tags.py
+-rw-rw-rw-   0 root         (0) root         (0)     1133 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/templatetags/vstconfigs.py
+-rw-rw-rw-   0 root         (0) root         (0)    17731 2023-05-25 10:44:35.000000 vstutils-5.4.8/vstutils/tests.py
+-rw-rw-rw-   0 root         (0) root         (0)      612 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 15:50:43.755326 vstutils-5.4.8/vstutils/translations/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/translations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    16196 2023-03-15 02:43:46.000000 vstutils-5.4.8/vstutils/translations/cn.py
+-rw-rw-rw-   0 root         (0) root         (0)      420 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/translations/en.py
+-rw-rw-rw-   0 root         (0) root         (0)    23941 2023-03-15 02:43:46.000000 vstutils-5.4.8/vstutils/translations/ru.py
+-rw-rw-rw-   0 root         (0) root         (0)    18983 2023-03-15 02:43:46.000000 vstutils-5.4.8/vstutils/translations/vi.py
+-rw-rw-rw-   0 root         (0) root         (0)     2721 2023-02-06 06:25:26.000000 vstutils-5.4.8/vstutils/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)    44730 2023-05-25 10:44:35.000000 vstutils-5.4.8/vstutils/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1482 2023-02-06 06:25:26.000000 vstutils-5.4.8/vstutils/web.ini
+-rw-rw-rw-   0 root         (0) root         (0)      843 2022-12-19 05:43:06.000000 vstutils-5.4.8/vstutils/wsgi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 15:50:43.719326 vstutils-5.4.8/vstutils.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4459 2023-05-25 15:50:43.000000 vstutils-5.4.8/vstutils.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7644 2023-05-25 15:50:43.000000 vstutils-5.4.8/vstutils.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       85 2023-05-25 15:50:43.000000 vstutils-5.4.8/vstutils.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       64 2023-05-25 15:50:43.000000 vstutils-5.4.8/vstutils.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 15:49:30.000000 vstutils-5.4.8/vstutils.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)     1941 2023-05-25 15:50:43.000000 vstutils-5.4.8/vstutils.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-05-25 15:50:43.000000 vstutils-5.4.8/vstutils.egg-info/top_level.txt
```

### Comparing `vstutils-5.4.7/LICENSE` & `vstutils-5.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/MANIFEST.in` & `vstutils-5.4.8/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/NOTICE` & `vstutils-5.4.8/NOTICE`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/PKG-INFO` & `vstutils-5.4.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vstutils
-Version: 5.4.7
+Version: 5.4.8
 Summary: VST Utils Framework for fast create web-application
 Home-page: https://github.com/vstconsulting/vstutils
 Author: VST Consulting
 Author-email: sergey.k@vstconsulting.net
 License: Apache License 2.0
 Project-URL: Issue Tracker, https://gitlab.com/vstconsulting/vstutils/issues
 Project-URL: Source Code, https://gitlab.com/vstconsulting/vstutils
```

### Comparing `vstutils-5.4.7/README.rst` & `vstutils-5.4.8/README.rst`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/requirements.txt` & `vstutils-5.4.8/requirements.txt`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/setup.cfg` & `vstutils-5.4.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/setup.py` & `vstutils-5.4.8/setup.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/api/actions.py` & `vstutils-5.4.8/vstutils/api/actions.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/api/admin.py` & `vstutils-5.4.8/vstutils/api/admin.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/api/auth.py` & `vstutils-5.4.8/vstutils/api/auth.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/api/base.py` & `vstutils-5.4.8/vstutils/api/base.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/api/decorators.py` & `vstutils-5.4.8/vstutils/api/decorators.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/api/decorators.pyi` & `vstutils-5.4.8/vstutils/api/decorators.pyi`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/api/doc_generator.py` & `vstutils-5.4.8/vstutils/api/doc_generator.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/api/endpoint.py` & `vstutils-5.4.8/vstutils/api/endpoint.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/api/fields.py` & `vstutils-5.4.8/vstutils/api/fields.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/api/filter_backends.py` & `vstutils-5.4.8/vstutils/api/filter_backends.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/api/filters.py` & `vstutils-5.4.8/vstutils/api/filters.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/api/health.py` & `vstutils-5.4.8/vstutils/api/health.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/api/meta.py` & `vstutils-5.4.8/vstutils/api/meta.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/api/metrics.py` & `vstutils-5.4.8/vstutils/api/metrics.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/api/migrations/0001_initial.py` & `vstutils-5.4.8/vstutils/api/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/api/migrations/0002_two_factor.py` & `vstutils-5.4.8/vstutils/api/migrations/0002_two_factor.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/api/migrations/0003_tfa_indexes.py` & `vstutils-5.4.8/vstutils/api/migrations/0003_tfa_indexes.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/api/migrations/0004_user_settings.py` & `vstutils-5.4.8/vstutils/api/migrations/0004_user_settings.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/api/migrations/0005_db_translations.py` & `vstutils-5.4.8/vstutils/api/migrations/0005_db_translations.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/api/migrations/0006_fix_user_settings.py` & `vstutils-5.4.8/vstutils/api/migrations/0006_fix_user_settings.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/api/models.py` & `vstutils-5.4.8/vstutils/api/models.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/api/pagination.py` & `vstutils-5.4.8/vstutils/api/pagination.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/api/parsers.py` & `vstutils-5.4.8/vstutils/api/parsers.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/api/permissions.py` & `vstutils-5.4.8/vstutils/api/permissions.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/api/renderers.py` & `vstutils-5.4.8/vstutils/api/renderers.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/api/responses.py` & `vstutils-5.4.8/vstutils/api/responses.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/api/responses.pyi` & `vstutils-5.4.8/vstutils/api/responses.pyi`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/api/routers.py` & `vstutils-5.4.8/vstutils/api/routers.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/api/routers.pyi` & `vstutils-5.4.8/vstutils/api/routers.pyi`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/api/schema/generators.py` & `vstutils-5.4.8/vstutils/api/schema/generators.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/api/schema/info.py` & `vstutils-5.4.8/vstutils/api/schema/info.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/api/schema/inspectors.py` & `vstutils-5.4.8/vstutils/api/schema/inspectors.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/api/schema/schema.py` & `vstutils-5.4.8/vstutils/api/schema/schema.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/api/serializers.py` & `vstutils-5.4.8/vstutils/api/serializers.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/api/throttling.py` & `vstutils-5.4.8/vstutils/api/throttling.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/api/validators.py` & `vstutils-5.4.8/vstutils/api/validators.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/api/views.py` & `vstutils-5.4.8/vstutils/api/views.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/asgi.py` & `vstutils-5.4.8/vstutils/asgi.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/asgi_worker.py` & `vstutils-5.4.8/vstutils/asgi_worker.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/auth.py` & `vstutils-5.4.8/vstutils/auth.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/auth.pyi` & `vstutils-5.4.8/vstutils/auth.pyi`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/celery_beat_scheduler.py` & `vstutils-5.4.8/vstutils/celery_beat_scheduler.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/doc_themes/vst-sphinx-theme/layout.html` & `vstutils-5.4.8/vstutils/doc_themes/vst-sphinx-theme/layout.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/environment.py` & `vstutils-5.4.8/vstutils/environment.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/exceptions.py` & `vstutils-5.4.8/vstutils/exceptions.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/gui/context.py` & `vstutils-5.4.8/vstutils/gui/context.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/gui/forms.py` & `vstutils-5.4.8/vstutils/gui/forms.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/gui/pwa_manifest.py` & `vstutils-5.4.8/vstutils/gui/pwa_manifest.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/gui/views.py` & `vstutils-5.4.8/vstutils/gui/views.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/ldap_utils.py` & `vstutils-5.4.8/vstutils/ldap_utils.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/management/commands/_base.py` & `vstutils-5.4.8/vstutils/management/commands/_base.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/management/commands/celery_inspect.py` & `vstutils-5.4.8/vstutils/management/commands/celery_inspect.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/management/commands/dockerrun.py` & `vstutils-5.4.8/vstutils/management/commands/dockerrun.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/management/commands/newproject.py` & `vstutils-5.4.8/vstutils/management/commands/newproject.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/management/commands/run_task.py` & `vstutils-5.4.8/vstutils/management/commands/run_task.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/management/commands/runrpc.py` & `vstutils-5.4.8/vstutils/management/commands/runrpc.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/management/commands/runserver.py` & `vstutils-5.4.8/vstutils/management/commands/runserver.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/management/commands/web.py` & `vstutils-5.4.8/vstutils/management/commands/web.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/middleware.py` & `vstutils-5.4.8/vstutils/middleware.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/models/__init__.py` & `vstutils-5.4.8/vstutils/models/__init__.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/models/base.py` & `vstutils-5.4.8/vstutils/models/base.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/models/cent_notify.py` & `vstutils-5.4.8/vstutils/models/cent_notify.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/models/custom_model.py` & `vstutils-5.4.8/vstutils/models/custom_model.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/models/custom_model.pyi` & `vstutils-5.4.8/vstutils/models/custom_model.pyi`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/models/decorators.py` & `vstutils-5.4.8/vstutils/models/decorators.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/models/fields.py` & `vstutils-5.4.8/vstutils/models/fields.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/models/queryset.py` & `vstutils-5.4.8/vstutils/models/queryset.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/settings.ini` & `vstutils-5.4.8/vstutils/settings.ini`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/settings.py` & `vstutils-5.4.8/vstutils/settings.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/static/bundle/281.chunk.js` & `vstutils-5.4.8/vstutils/static/bundle/281.chunk.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/static/bundle/296.chunk.js` & `vstutils-5.4.8/vstutils/static/bundle/296.chunk.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/static/bundle/345.chunk.js` & `vstutils-5.4.8/vstutils/static/bundle/345.chunk.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/static/bundle/368.chunk.js` & `vstutils-5.4.8/vstutils/static/bundle/368.chunk.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/static/bundle/421.js` & `vstutils-5.4.8/vstutils/static/bundle/421.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/static/bundle/421.js.LICENSE.txt` & `vstutils-5.4.8/vstutils/static/bundle/421.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/static/bundle/618.js` & `vstutils-5.4.8/vstutils/static/bundle/618.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/static/bundle/683.chunk.js` & `vstutils-5.4.8/vstutils/static/bundle/683.chunk.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/static/bundle/686.js` & `vstutils-5.4.8/vstutils/static/bundle/686.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/static/bundle/742.chunk.js` & `vstutils-5.4.8/vstutils/static/bundle/742.chunk.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/static/bundle/742.chunk.js.LICENSE.txt` & `vstutils-5.4.8/vstutils/static/bundle/742.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/static/bundle/755.js` & `vstutils-5.4.8/vstutils/static/bundle/755.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/static/bundle/826.chunk.js` & `vstutils-5.4.8/vstutils/static/bundle/826.chunk.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/static/bundle/826.chunk.js.LICENSE.txt` & `vstutils-5.4.8/vstutils/static/bundle/826.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/static/bundle/844.js` & `vstutils-5.4.8/vstutils/static/bundle/844.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/static/bundle/959.js` & `vstutils-5.4.8/vstutils/static/bundle/959.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/static/bundle/959.js.LICENSE.txt` & `vstutils-5.4.8/vstutils/static/bundle/959.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/static/bundle/app_loader.js` & `vstutils-5.4.8/vstutils/static/bundle/app_loader.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/static/bundle/base.js` & `vstutils-5.4.8/vstutils/static/bundle/base.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/static/bundle/bb58e57c48a3e911f15f.woff` & `vstutils-5.4.8/vstutils/static/bundle/bb58e57c48a3e911f15f.woff`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/static/bundle/eeccf4f66002c6f2ba24.woff` & `vstutils-5.4.8/vstutils/static/bundle/eeccf4f66002c6f2ba24.woff`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/static/bundle/output.json` & `vstutils-5.4.8/vstutils/static/bundle/output.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9964192708333334%*

 * *Differences: {"'entrypoints'": "{'spa': {'assets': {0: {'size': 432625}}, 'assetsSize': 3679168}}"}*

```diff
@@ -26,15 +26,15 @@
             "filteredAuxiliaryAssets": 0,
             "name": "base"
         },
         "spa": {
             "assets": [
                 {
                     "name": "vstutils.js",
-                    "size": 432611
+                    "size": 432625
                 },
                 {
                     "name": "755.js",
                     "size": 89997
                 },
                 {
                     "name": "421.js",
@@ -57,15 +57,15 @@
                     "size": 1798980
                 },
                 {
                     "name": "spa.js",
                     "size": 3597
                 }
             ],
-            "assetsSize": 3679154,
+            "assetsSize": 3679168,
             "auxiliaryAssetsSize": 117924,
             "filteredAssets": 0,
             "filteredAuxiliaryAssets": 2,
             "name": "spa"
         }
     },
     "errors": []
```

### Comparing `vstutils-5.4.7/vstutils/static/bundle/spa.js` & `vstutils-5.4.8/vstutils/static/bundle/spa.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/static/bundle/vstutils.js` & `vstutils-5.4.8/vstutils/static/bundle/vstutils.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -194,15 +194,15 @@
             });
             var a = n(14412),
                 r = n(64723),
                 o = n(41657),
                 l = n(36446),
                 u = n(33159),
                 d = n(5459),
-                c = n(39560),
+                c = n(51916),
                 p = n(89451),
                 f = n(9536),
                 h = n(69165),
                 m = n(47858),
                 v = function() {
                     var e = this,
                         t = e._self._c;
@@ -4476,15 +4476,15 @@
                         return s.__notFound = !0, s
                     })) : Promise.resolve(e)));
                 return s.execute(), Promise.all(o)
             }
 
             function f(e, t, n) {
                 const i = [];
-                for (const s of t) !h(s) || !s.usePrefetch && null != n && n.isPrefetch ? s instanceof o.ArrayField ? i.push(v(s, e)) : s instanceof l.DynamicField ? i.push(g(s, e)) : s instanceof d.a && i.push(_(s, e)) : i.push(m(s, e));
+                for (const s of t) !h(s) || !s.usePrefetch && null != n && n.isPrefetch ? s instanceof o.ArrayField ? i.push(v(s, e, n)) : s instanceof l.DynamicField ? i.push(g(s, e, n)) : s instanceof d.a && i.push(_(s, e, n)) : i.push(m(s, e));
                 return Promise.all(i)
             }
 
             function h(e) {
                 return "_canBeFetched" in e
             }
             async function m(e, t) {
@@ -4492,58 +4492,58 @@
                     i = await p(n, e);
                 for (let n = 0; n < i.length; n++) t[n].sandbox.set({
                     field: e.name,
                     value: i[n],
                     markChanged: !1
                 })
             }
-            async function v(e, t) {
-                const n = new Map;
-                for (const i of t) {
-                    const t = e._deserializeValue(i._data),
-                        s = i.constructor;
+            async function v(e, t, n) {
+                const i = new Map;
+                for (const n of t) {
+                    const t = e._deserializeValue(n._data),
+                        s = n.constructor;
                     class a extends s {}
                     a.fields = new Map(a.fields), a.fields.set(e.name, e.itemField);
-                    const o = t.map((t => new a((0, r.createPropertyProxy)(i._data, e.name, t))));
-                    n.set(i, o)
+                    const o = t.map((t => new a((0, r.createPropertyProxy)(n._data, e.name, t))));
+                    i.set(n, o)
                 }
-                const i = Array.from(n.values()).flat(),
-                    s = e.itemField;
-                await f(i, [s]);
-                for (const [t, i] of n) t.sandbox.set({
+                const s = Array.from(i.values()).flat(),
+                    a = e.itemField;
+                await f(s, [a], n);
+                for (const [t, n] of i) t.sandbox.set({
                     field: e.name,
-                    value: i.map((t => e.getValue(t.sandbox.value))),
+                    value: n.map((t => e.getValue(t.sandbox.value))),
                     markChanged: !1
                 })
             }
-            async function g(e, t) {
-                const n = new Map;
-                for (const i of t) {
-                    const t = e.getRealField(i.sandbox.value),
-                        s = Array.from(n.keys()).find((e => t.isEqual(e)));
-                    s ? n.get(s).push(i) : n.set(t, [i])
-                }
-                const i = Array.from(n.entries()).map((e => {
-                    let [t, n] = e;
-                    return f(n, [t])
+            async function g(e, t, n) {
+                const i = new Map;
+                for (const n of t) {
+                    const t = e.getRealField(n.sandbox.value),
+                        s = Array.from(i.keys()).find((e => t.isEqual(e)));
+                    s ? i.get(s).push(n) : i.set(t, [n])
+                }
+                const s = Array.from(i.entries()).map((e => {
+                    let [t, i] = e;
+                    return f(i, [t], n)
                 }));
-                return Promise.all(i)
+                return Promise.all(s)
             }
-            async function _(e, t) {
-                const n = e.itemsModel;
-                for (const s of t) {
-                    var i;
-                    const t = null !== (i = e.getValue(s._data)) && void 0 !== i ? i : [];
-                    s.sandbox.set({
+            async function _(e, t, n) {
+                const i = e.itemsModel;
+                for (const n of t) {
+                    var s;
+                    const t = null !== (s = e.getValue(n._data)) && void 0 !== s ? s : [];
+                    n.sandbox.set({
                         field: e.name,
-                        value: t.map((e => new n(e))),
+                        value: t.map((e => new i(e))),
                         markChanged: !1
                     })
                 }
-                return c(t.flatMap((t => e.getValue(t.sandbox.value))))
+                return c(t.flatMap((t => e.getValue(t.sandbox.value))), n)
             }
         },
         97348: function(e, t, n) {
             n.r(t), n.d(t, {
                 ArrayField: function() {
                     return pe
                 },
@@ -15297,14 +15297,21 @@
                                 }))))), v.guiPopUp.success(g.a.t(v.pop_up_msg.instance.success.removeMany))
                             } catch (e) {
                                 const t = i.error_handler.errorToString(e),
                                     n = g.a.t(v.pop_up_msg.instance.error.removeMany, [t]);
                                 i.error_handler.showError(n, t)
                             }
                             _.unselectIds(a)
+                        },
+                        executeMultiAction: async function(e) {
+                            const t = h.value.filter((e => _.selection.value.includes(e.getPkValue())));
+                            await i.actions.execute({
+                                action: e,
+                                instances: t
+                            })
                         }
                     }
                 },
                 w = e => {
                     const t = (0, l.VS)(e),
                         n = (0, l.vG)(e),
                         i = (0, l.go)(e),
@@ -16018,15 +16025,15 @@
                     return b
                 }
             });
             var i = n(4942),
                 s = (n(10072), n(23042), n(99137), n(71957), n(96306), n(103), n(74592), n(58276), n(35082), n(12813), n(18222), n(38563), n(50336), n(7512), n(33948), n(15306), n(57658), n(67476)),
                 a = n(70538),
                 r = n(59198),
-                o = n(39560),
+                o = n(51916),
                 l = n(89045),
                 u = n(56039),
                 d = n(56716);
             const c = (0, r.createUniqueIdGenerator)();
             class p {
                 constructor(e, t) {
                     var n, s, a, r, o;
@@ -16558,20 +16565,20 @@
         67599: function(e, t, n) {
             var i = n(8081),
                 s = n.n(i),
                 a = n(23645),
                 r = n.n(a)()(s());
             r.push([e.id, ".pk-column{display:none}", ""]), t.Z = r
         },
-        50615: function(e, t, n) {
+        48906: function(e, t, n) {
             var i = n(8081),
                 s = n.n(i),
                 a = n(23645),
                 r = n.n(a)()(s());
-            r.push([e.id, ".filters-buttons[data-v-7bd46eaf]{display:flex;justify-content:space-between;margin-bottom:5px}.search-form[data-v-7bd46eaf]{display:flex;position:relative}.search-input[data-v-7bd46eaf]{padding:0 30px 0 8px}.search-button[data-v-7bd46eaf]{position:relative;right:30px;top:auto;border:none;background-color:rgba(0,0,0,0)}.slide-from-left-leave-active[data-v-7bd46eaf],.slide-from-left-enter-active[data-v-7bd46eaf]{transition:all .5s ease}.slide-from-left-enter[data-v-7bd46eaf],.slide-from-left-leave-to[data-v-7bd46eaf]{transform:translate(-120%, 0);opacity:0}", ""]), t.Z = r
+            r.push([e.id, ".filters-buttons[data-v-5f12835b]{display:flex;justify-content:space-between;margin-bottom:5px}.search-form[data-v-5f12835b]{display:flex;position:relative}.search-input[data-v-5f12835b]{padding:0 30px 0 8px}.search-button[data-v-5f12835b]{position:relative;right:30px;top:auto;border:none;background-color:rgba(0,0,0,0)}.slide-from-left-leave-active[data-v-5f12835b],.slide-from-left-enter-active[data-v-5f12835b]{transition:all .5s ease}.slide-from-left-enter[data-v-5f12835b],.slide-from-left-leave-to[data-v-5f12835b]{transform:translate(-120%, 0);opacity:0}", ""]), t.Z = r
         },
         47: function(e, t, n) {
             var i = n(8081),
                 s = n.n(i),
                 a = n(23645),
                 r = n.n(a)()(s());
             r.push([e.id, ".dropdown[data-v-adb9306e]{display:inline-block}", ""]), t.Z = r
@@ -19675,18 +19682,18 @@
                 x = {};
             x.styleTagTransform = y(), x.setAttributes = v(), x.insert = h().bind(null, "head"), x.domAPI = p(), x.insertStyleElement = _(), d()(w.Z, x), w.Z && w.Z.locals && w.Z.locals;
             var C = n(67599),
                 S = {};
             S.styleTagTransform = y(), S.setAttributes = v(), S.insert = h().bind(null, "head"), S.domAPI = p(), S.insertStyleElement = _(), d()(C.Z, S), C.Z && C.Z.locals && C.Z.locals;
             var k = (0, n(51900).Z)(l, i, [], !1, null, "39493925", null).exports
         },
-        39560: function(e, t, n) {
+        51916: function(e, t, n) {
             n.d(t, {
                 Z: function() {
-                    return T
+                    return A
                 }
             });
             var i = function() {
                 var e = this,
                     t = e._self._c,
                     n = e._self._setupProxy;
                 return t("div", [e.view.enableSearch && n.searchField ? t("portal", {
@@ -19792,36 +19799,37 @@
                     class: n.multiActionsClasses.uniq.value,
                     attrs: {
                         "multi-actions": n.multiActions,
                         selected: n.selection,
                         instances: n.instances
                     },
                     on: {
-                        "execute-multi-action": n.executeMultiAction
+                        "execute-multi-action": function(e) {
+                            return n.store.executeMultiAction(e)
+                        }
                     }
                 }) : e._e()], 1), e._v(" "), t(n.Pagination, {
                     staticStyle: {
                         float: "right"
                     },
                     attrs: {
                         items: n.paginationItems
                     }
                 })], 1)]], 2)], 1)
             };
             i._withStripped = !0, n(33948), n(57658), n(88921), n(96248), n(13599), n(11477), n(64362), n(15389), n(90401), n(45164), n(91238), n(54837), n(87485), n(56767), n(76651), n(61437), n(35285), n(39865), n(88449), n(2490), n(59849);
             var s = n(70538),
                 a = n(67476),
-                r = n(59198),
-                o = n(66523),
-                l = n(56039),
-                u = n(33159),
-                d = n(89451),
-                c = n(9536);
+                r = n(66523),
+                o = n(56039),
+                l = n(33159),
+                u = n(89451),
+                d = n(9536);
 
-            function p() {
+            function c() {
                 let e = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : "";
                 const t = (0, s.ref)([]);
                 return {
                     add: function(n) {
                         "string" == typeof n && (n = [n]);
                         for (const i of n) t.value.push("".concat(e).concat(i))
                     },
@@ -19830,94 +19838,85 @@
                         for (const i of n) {
                             const n = t.value.indexOf("".concat(e).concat(i)); - 1 !== n && t.value.splice(n, 1)
                         }
                     },
                     uniq: (0, s.computed)((() => Array.from(new Set(t.value))))
                 }
             }
-            var f = (0, s.defineComponent)({
+            var p = (0, s.defineComponent)({
                     __name: "ListViewComponent",
-                    props: o.n,
+                    props: r.n,
                     setup(e) {
                         const t = e,
-                            n = (0, r.getApp)(),
-                            i = (0, l.useViewStore)(),
-                            o = p("selected__");
-                        (0, s.provide)("multiActionsClasses", o);
-                        const f = (0, s.computed)((() => {
+                            n = (0, o.useViewStore)(),
+                            i = c("selected__");
+                        (0, s.provide)("multiActionsClasses", i);
+                        const r = (0, s.computed)((() => {
                                 var e, n;
                                 return null === (e = t.view) || void 0 === e || null === (n = e.filters) || void 0 === n ? void 0 : n.__search
                             })),
-                            h = (0, s.computed)((() => {
-                                var e, t, n;
-                                return null !== (e = null === (t = i.instances) || void 0 === t || null === (n = t.extra) || void 0 === n ? void 0 : n.count) && void 0 !== e ? e : -1
+                            p = (0, s.computed)((() => {
+                                var e, t, i;
+                                return null !== (e = null === (t = n.instances) || void 0 === t || null === (i = t.extra) || void 0 === i ? void 0 : i.count) && void 0 !== e ? e : -1
                             })),
-                            m = (0, s.computed)((() => Array.from(i.model.fields.values()).filter((e => !e.hidden)))),
-                            v = (0, s.ref)(""),
+                            f = (0, s.computed)((() => Array.from(n.model.fields.values()).filter((e => !e.hidden)))),
+                            h = (0, s.ref)(""),
                             {
-                                error: g,
-                                instanceActions: _,
-                                instances: b,
-                                instanceSublinks: y,
-                                isEmpty: w,
-                                model: x,
-                                multiActions: C,
-                                paginationItems: S,
-                                selection: k
-                            } = (0, a.storeToRefs)(i);
+                                error: m,
+                                instanceActions: v,
+                                instances: g,
+                                instanceSublinks: _,
+                                isEmpty: b,
+                                model: y,
+                                multiActions: w,
+                                paginationItems: x,
+                                selection: C
+                            } = (0, a.storeToRefs)(n);
                         return {
                             __sfc: !0,
-                            useUniqueCssClasses: p,
+                            useUniqueCssClasses: c,
                             props: t,
-                            app: n,
-                            store: i,
-                            multiActionsClasses: o,
-                            searchField: f,
-                            totalNumberOfInstances: h,
-                            fields: m,
-                            searchFieldValue: v,
-                            executeMultiAction: async function(e) {
-                                const t = i.instances.filter((e => i.selection.includes(e.getPkValue())));
-                                return n.actions.execute({
-                                    action: e,
-                                    instances: t
-                                })
-                            },
-                            error: g,
-                            instanceActions: _,
-                            instances: b,
-                            instanceSublinks: y,
-                            isEmpty: w,
-                            model: x,
-                            multiActions: C,
-                            paginationItems: S,
-                            selection: k,
-                            ListTable: u.Z,
-                            MultiActions: d.Z,
-                            Pagination: c.Z
+                            store: n,
+                            multiActionsClasses: i,
+                            searchField: r,
+                            totalNumberOfInstances: p,
+                            fields: f,
+                            searchFieldValue: h,
+                            error: m,
+                            instanceActions: v,
+                            instances: g,
+                            instanceSublinks: _,
+                            isEmpty: b,
+                            model: y,
+                            multiActions: w,
+                            paginationItems: x,
+                            selection: C,
+                            ListTable: l.Z,
+                            MultiActions: u.Z,
+                            Pagination: d.Z
                         }
                     }
                 }),
-                h = f,
-                m = n(93379),
-                v = n.n(m),
-                g = n(7795),
-                _ = n.n(g),
-                b = n(90569),
-                y = n.n(b),
-                w = n(3565),
-                x = n.n(w),
-                C = n(19216),
-                S = n.n(C),
-                k = n(44589),
-                F = n.n(k),
-                Z = n(50615),
-                A = {};
-            A.styleTagTransform = F(), A.setAttributes = x(), A.insert = y().bind(null, "head"), A.domAPI = _(), A.insertStyleElement = S(), v()(Z.Z, A), Z.Z && Z.Z.locals && Z.Z.locals;
-            var T = (0, n(51900).Z)(h, i, [], !1, null, "7bd46eaf", null).exports
+                f = p,
+                h = n(93379),
+                m = n.n(h),
+                v = n(7795),
+                g = n.n(v),
+                _ = n(90569),
+                b = n.n(_),
+                y = n(3565),
+                w = n.n(y),
+                x = n(19216),
+                C = n.n(x),
+                S = n(44589),
+                k = n.n(S),
+                F = n(48906),
+                Z = {};
+            Z.styleTagTransform = k(), Z.setAttributes = w(), Z.insert = b().bind(null, "head"), Z.domAPI = g(), Z.insertStyleElement = C(), m()(F.Z, Z), F.Z && F.Z.locals && F.Z.locals;
+            var A = (0, n(51900).Z)(f, i, [], !1, null, "5f12835b", null).exports
         },
         89451: function(e, t, n) {
             n.d(t, {
                 Z: function() {
                     return b
                 }
             });
```

### Comparing `vstutils-5.4.7/vstutils/static/img/anonymous.png` & `vstutils-5.4.8/vstutils/static/img/anonymous.png`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/static_files.py` & `vstutils-5.4.8/vstutils/static_files.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/tasks.py` & `vstutils-5.4.8/vstutils/tasks.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/templates/auth/base.html` & `vstutils-5.4.8/vstutils/templates/auth/base.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/templates/auth/language_selector.html` & `vstutils-5.4.8/vstutils/templates/auth/language_selector.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/templates/auth/tfa.html` & `vstutils-5.4.8/vstutils/templates/auth/tfa.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/templates/base.html` & `vstutils-5.4.8/vstutils/templates/base.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/templates/gui/base.html` & `vstutils-5.4.8/vstutils/templates/gui/base.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/templates/gui/offline.html` & `vstutils-5.4.8/vstutils/templates/gui/offline.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/templates/gui/service-worker.js` & `vstutils-5.4.8/vstutils/templates/gui/service-worker.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/templates/newproject/.gitignore.template` & `vstutils-5.4.8/vstutils/templates/newproject/.gitignore.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/templates/newproject/frontend_src/.eslintrc.js.template` & `vstutils-5.4.8/vstutils/templates/newproject/frontend_src/.eslintrc.js.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/templates/newproject/package.json.template` & `vstutils-5.4.8/vstutils/templates/newproject/package.json.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/templates/newproject/project_name/settings.py.template` & `vstutils-5.4.8/vstutils/templates/newproject/project_name/settings.py.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/templates/newproject/setup.cfg.template` & `vstutils-5.4.8/vstutils/templates/newproject/setup.cfg.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/templates/newproject/setup.py.template` & `vstutils-5.4.8/vstutils/templates/newproject/setup.py.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/templates/newproject/test.py.template` & `vstutils-5.4.8/vstutils/templates/newproject/test.py.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/templates/newproject/tox.ini.template` & `vstutils-5.4.8/vstutils/templates/newproject/tox.ini.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/templates/newproject/tox_build.ini.template` & `vstutils-5.4.8/vstutils/templates/newproject/tox_build.ini.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/templates/newproject/webpack.config.js.default.template` & `vstutils-5.4.8/vstutils/templates/newproject/webpack.config.js.default.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/templates/registration/confirm_email.html` & `vstutils-5.4.8/vstutils/templates/registration/confirm_email.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/templates/registration/password_reset_confirm.html` & `vstutils-5.4.8/vstutils/templates/registration/password_reset_confirm.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/templates/registration/password_reset_form.html` & `vstutils-5.4.8/vstutils/templates/registration/password_reset_form.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/templates/registration/user_registration.html` & `vstutils-5.4.8/vstutils/templates/registration/user_registration.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/templates/rest_framework/admin.html` & `vstutils-5.4.8/vstutils/templates/rest_framework/admin.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/templates/vst_inclusion_tags/bootstrap_form.html` & `vstutils-5.4.8/vstutils/templates/vst_inclusion_tags/bootstrap_form.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/templates/widgets/agreement_widget.html` & `vstutils-5.4.8/vstutils/templates/widgets/agreement_widget.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/templatetags/request_static.py` & `vstutils-5.4.8/vstutils/templatetags/request_static.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/templatetags/translation.py` & `vstutils-5.4.8/vstutils/templatetags/translation.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/templatetags/vst_gravatar.py` & `vstutils-5.4.8/vstutils/templatetags/vst_gravatar.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/templatetags/vst_html_tags.py` & `vstutils-5.4.8/vstutils/templatetags/vst_html_tags.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/templatetags/vstconfigs.py` & `vstutils-5.4.8/vstutils/templatetags/vstconfigs.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/tests.py` & `vstutils-5.4.8/vstutils/tests.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/tools.py` & `vstutils-5.4.8/vstutils/tools.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/translations/cn.py` & `vstutils-5.4.8/vstutils/translations/cn.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/translations/ru.py` & `vstutils-5.4.8/vstutils/translations/ru.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/translations/vi.py` & `vstutils-5.4.8/vstutils/translations/vi.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/urls.py` & `vstutils-5.4.8/vstutils/urls.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/utils.py` & `vstutils-5.4.8/vstutils/utils.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/web.ini` & `vstutils-5.4.8/vstutils/web.ini`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils/wsgi.py` & `vstutils-5.4.8/vstutils/wsgi.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils.egg-info/PKG-INFO` & `vstutils-5.4.8/vstutils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vstutils
-Version: 5.4.7
+Version: 5.4.8
 Summary: VST Utils Framework for fast create web-application
 Home-page: https://github.com/vstconsulting/vstutils
 Author: VST Consulting
 Author-email: sergey.k@vstconsulting.net
 License: Apache License 2.0
 Project-URL: Issue Tracker, https://gitlab.com/vstconsulting/vstutils/issues
 Project-URL: Source Code, https://gitlab.com/vstconsulting/vstutils
```

### Comparing `vstutils-5.4.7/vstutils.egg-info/SOURCES.txt` & `vstutils-5.4.8/vstutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.7/vstutils.egg-info/requires.txt` & `vstutils-5.4.8/vstutils.egg-info/requires.txt`

 * *Files identical despite different names*

