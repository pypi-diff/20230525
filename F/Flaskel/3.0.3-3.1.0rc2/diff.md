# Comparing `tmp/Flaskel-3.0.3.tar.gz` & `tmp/Flaskel-3.1.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Flaskel-3.0.3.tar", last modified: Sun Jun 19 21:12:32 2022, max compression
+gzip compressed data, was "Flaskel-3.1.0rc2.tar", last modified: Thu May 25 21:39:53 2023, max compression
```

## Comparing `Flaskel-3.0.3.tar` & `Flaskel-3.1.0rc2.tar`

### file list

```diff
@@ -1,171 +1,171 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-19 21:12:32.384130 Flaskel-3.0.3/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-19 21:12:32.341126 Flaskel-3.0.3/Flaskel.egg-info/
--rw-r--r--   0 root         (0) root         (0)    15615 2022-06-19 21:12:32.000000 Flaskel-3.0.3/Flaskel.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4585 2022-06-19 21:12:32.000000 Flaskel-3.0.3/Flaskel.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-06-19 21:12:32.000000 Flaskel-3.0.3/Flaskel.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       53 2022-06-19 21:12:32.000000 Flaskel-3.0.3/Flaskel.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-06-19 21:12:32.000000 Flaskel-3.0.3/Flaskel.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      907 2022-06-19 21:12:32.000000 Flaskel-3.0.3/Flaskel.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2022-06-19 21:12:32.000000 Flaskel-3.0.3/Flaskel.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      123 2022-06-19 21:12:15.000000 Flaskel-3.0.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    15615 2022-06-19 21:12:32.383129 Flaskel-3.0.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    14795 2022-06-19 21:12:15.000000 Flaskel-3.0.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-19 21:12:32.343126 Flaskel-3.0.3/flaskel/
--rw-rw-rw-   0 root         (0) root         (0)      712 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12165 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/builder.py
--rw-rw-rw-   0 root         (0) root         (0)     9054 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/config.py
--rw-rw-rw-   0 root         (0) root         (0)     1188 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/converters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-19 21:12:32.347127 Flaskel-3.0.3/flaskel/ext/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/ext/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7328 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/ext/auth.py
--rw-rw-rw-   0 root         (0) root         (0)     4245 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/ext/caching.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-19 21:12:32.348127 Flaskel-3.0.3/flaskel/ext/crypto/
--rw-rw-rw-   0 root         (0) root         (0)       26 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/ext/crypto/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1725 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/ext/crypto/argon.py
--rw-rw-rw-   0 root         (0) root         (0)      886 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/ext/datetime.py
--rw-rw-rw-   0 root         (0) root         (0)     1278 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/ext/default.py
--rw-rw-rw-   0 root         (0) root         (0)      646 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/ext/errors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-19 21:12:32.349127 Flaskel-3.0.3/flaskel/ext/healthcheck/
--rw-rw-rw-   0 root         (0) root         (0)      203 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/ext/healthcheck/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6601 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/ext/healthcheck/checkers.py
--rw-rw-rw-   0 root         (0) root         (0)     4962 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/ext/healthcheck/health.py
--rw-rw-rw-   0 root         (0) root         (0)     7831 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/ext/ipban.py
--rw-rw-rw-   0 root         (0) root         (0)     5419 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/ext/jobs.py
--rw-rw-rw-   0 root         (0) root         (0)     1309 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/ext/limit.py
--rw-rw-rw-   0 root         (0) root         (0)     6072 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/ext/mongo.py
--rw-rw-rw-   0 root         (0) root         (0)     1045 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/ext/redis.py
--rw-rw-rw-   0 root         (0) root         (0)     1605 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/ext/sendmail.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-19 21:12:32.352127 Flaskel-3.0.3/flaskel/ext/sqlalchemy/
--rw-rw-rw-   0 root         (0) root         (0)       83 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/ext/sqlalchemy/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2286 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/ext/sqlalchemy/model.py
--rw-rw-rw-   0 root         (0) root         (0)     1020 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/ext/useragent.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-19 21:12:32.352127 Flaskel-3.0.3/flaskel/ext/websocket/
--rw-rw-rw-   0 root         (0) root         (0)      526 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/ext/websocket/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-19 21:12:32.353127 Flaskel-3.0.3/flaskel/extra/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/extra/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8920 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/extra/account.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-19 21:12:32.353127 Flaskel-3.0.3/flaskel/extra/apidoc/
--rw-rw-rw-   0 root         (0) root         (0)       54 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/extra/apidoc/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2515 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/extra/apidoc/template.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-19 21:12:32.355127 Flaskel-3.0.3/flaskel/extra/media/
--rw-rw-rw-   0 root         (0) root         (0)      111 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/extra/media/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       82 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/extra/media/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     2127 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/extra/media/repo.py
--rw-rw-rw-   0 root         (0) root         (0)     2214 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/extra/media/service.py
--rw-rw-rw-   0 root         (0) root         (0)     1081 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/extra/media/view.py
--rw-rw-rw-   0 root         (0) root         (0)    11301 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/extra/mobile_support.py
--rw-rw-rw-   0 root         (0) root         (0)     5132 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/extra/notification.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-19 21:12:32.355127 Flaskel-3.0.3/flaskel/extra/payments/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/extra/payments/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-19 21:12:32.357128 Flaskel-3.0.3/flaskel/extra/payments/stripe/
--rw-rw-rw-   0 root         (0) root         (0)      135 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/extra/payments/stripe/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3521 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/extra/payments/stripe/handler.py
--rw-rw-rw-   0 root         (0) root         (0)     2808 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/extra/payments/stripe/repo.py
--rw-rw-rw-   0 root         (0) root         (0)     1311 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/extra/payments/stripe/view.py
--rw-rw-rw-   0 root         (0) root         (0)     4511 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/flaskel.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-19 21:12:32.358127 Flaskel-3.0.3/flaskel/http/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/http/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2587 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/http/client.py
--rw-rw-rw-   0 root         (0) root         (0)     9019 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/http/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     7162 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/middlewares.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-19 21:12:32.359128 Flaskel-3.0.3/flaskel/scripts/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/scripts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      253 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/scripts/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     1425 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/scripts/init_app.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-19 21:12:32.336126 Flaskel-3.0.3/flaskel/scripts/skeleton/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-19 21:12:32.363128 Flaskel-3.0.3/flaskel/scripts/skeleton/resources/
--rw-rw-rw-   0 root         (0) root         (0)      305 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/scripts/skeleton/resources/Caddyfile.example
--rw-rw-rw-   0 root         (0) root         (0)      532 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/scripts/skeleton/resources/conf.yaml
--rw-rw-rw-   0 root         (0) root         (0)     2271 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/scripts/skeleton/resources/log.yaml
--rw-rw-rw-   0 root         (0) root         (0)      757 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/scripts/skeleton/resources/manage.sh
--rw-rw-rw-   0 root         (0) root         (0)      414 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/scripts/skeleton/resources/nginx.example
--rw-rw-rw-   0 root         (0) root         (0)     1561 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/scripts/skeleton/resources/nuisances.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1325 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/scripts/skeleton/resources/schemas.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1775 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/scripts/skeleton/resources/settings.ini.sample
--rw-rw-rw-   0 root         (0) root         (0)      492 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/scripts/skeleton/resources/supervisor.example
--rw-rw-rw-   0 root         (0) root         (0)    14323 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/scripts/skeleton/resources/swagger.yaml
--rw-rw-rw-   0 root         (0) root         (0)      139 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/scripts/skeleton/resources/uwsgi.yaml.example
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-19 21:12:32.363128 Flaskel-3.0.3/flaskel/scripts/skeleton/skel/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-19 21:12:32.364128 Flaskel-3.0.3/flaskel/scripts/skeleton/skel/ext/
--rw-rw-rw-   0 root         (0) root         (0)     1768 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/scripts/skeleton/skel/ext/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      434 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/scripts/skeleton/skel/ext/auth.py
--rw-rw-rw-   0 root         (0) root         (0)       63 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/scripts/skeleton/skel/ext/database.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-19 21:12:32.364128 Flaskel-3.0.3/flaskel/scripts/skeleton/skel/forms/
--rw-rw-rw-   0 root         (0) root         (0)      330 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/scripts/skeleton/skel/forms/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-19 21:12:32.365128 Flaskel-3.0.3/flaskel/scripts/skeleton/skel/models/
--rw-rw-rw-   0 root         (0) root         (0)       69 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/scripts/skeleton/skel/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      189 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/scripts/skeleton/skel/models/user.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-19 21:12:32.366128 Flaskel-3.0.3/flaskel/scripts/skeleton/skel/scripts/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/scripts/skeleton/skel/scripts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      685 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/scripts/skeleton/skel/scripts/cli.py
--rw-rw-rw-   0 root         (0) root         (0)      504 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/scripts/skeleton/skel/scripts/config.py
--rw-rw-rw-   0 root         (0) root         (0)      915 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/scripts/skeleton/skel/scripts/ws.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-19 21:12:32.367128 Flaskel-3.0.3/flaskel/scripts/skeleton/skel/tasks/
--rw-rw-rw-   0 root         (0) root         (0)       57 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/scripts/skeleton/skel/tasks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      252 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/scripts/skeleton/skel/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-19 21:12:32.368128 Flaskel-3.0.3/flaskel/scripts/skeleton/skel/views/
--rw-rw-rw-   0 root         (0) root         (0)      856 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/scripts/skeleton/skel/views/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1010 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/scripts/skeleton/skel/views/blueprints.py
--rw-rw-rw-   0 root         (0) root         (0)     1672 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/scripts/skeleton/skel/views/common.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-19 21:12:32.334126 Flaskel-3.0.3/flaskel/scripts/skeleton/skel/views/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-19 21:12:32.368128 Flaskel-3.0.3/flaskel/scripts/skeleton/skel/views/static/css/
--rw-rw-rw-   0 root         (0) root         (0)      190 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/scripts/skeleton/skel/views/static/css/main.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-19 21:12:32.369128 Flaskel-3.0.3/flaskel/scripts/skeleton/skel/views/static/img/
--rw-rw-rw-   0 root         (0) root         (0)      318 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/scripts/skeleton/skel/views/static/img/favicon.ico
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-19 21:12:32.369128 Flaskel-3.0.3/flaskel/scripts/skeleton/skel/views/static/js/
--rw-rw-rw-   0 root         (0) root         (0)       35 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/scripts/skeleton/skel/views/static/js/main.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-19 21:12:32.369128 Flaskel-3.0.3/flaskel/scripts/skeleton/skel/views/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-19 21:12:32.370128 Flaskel-3.0.3/flaskel/scripts/skeleton/skel/views/templates/core/
--rw-rw-rw-   0 root         (0) root         (0)      206 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/scripts/skeleton/skel/views/templates/core/error.html
--rw-rw-rw-   0 root         (0) root         (0)     1103 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/scripts/skeleton/skel/views/templates/core/head.html
--rw-rw-rw-   0 root         (0) root         (0)      655 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/scripts/skeleton/skel/views/templates/core/scripts.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-19 21:12:32.371129 Flaskel-3.0.3/flaskel/scripts/skeleton/skel/views/templates/emails/
--rw-rw-rw-   0 root         (0) root         (0)      220 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/scripts/skeleton/skel/views/templates/emails/forgot.html
--rw-rw-rw-   0 root         (0) root         (0)      225 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/scripts/skeleton/skel/views/templates/emails/registration.html
--rw-rw-rw-   0 root         (0) root         (0)    13479 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/scripts/skeleton/skel/views/templates/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-19 21:12:32.372129 Flaskel-3.0.3/flaskel/scripts/skeleton/skel/views/templates/layout/
--rw-rw-rw-   0 root         (0) root         (0)      458 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/scripts/skeleton/skel/views/templates/layout/base.html
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/scripts/skeleton/skel/views/templates/layout/container.html
--rw-rw-rw-   0 root         (0) root         (0)       20 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/scripts/skeleton/skel/views/templates/layout/footer.html
--rw-rw-rw-   0 root         (0) root         (0)       20 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/scripts/skeleton/skel/views/templates/layout/header.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-19 21:12:32.374129 Flaskel-3.0.3/flaskel/scripts/skeleton/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/scripts/skeleton/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2433 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/scripts/skeleton/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)      190 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/scripts/skeleton/tests/helpers.py
--rw-rw-rw-   0 root         (0) root         (0)     2167 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/scripts/skeleton/tests/test_smoke.py
--rw-rw-rw-   0 root         (0) root         (0)     5319 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/standalone.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-19 21:12:32.375129 Flaskel-3.0.3/flaskel/tester/
--rw-rw-rw-   0 root         (0) root         (0)       31 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/tester/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1432 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/tester/client.py
--rw-rw-rw-   0 root         (0) root         (0)     7347 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/tester/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-19 21:12:32.377129 Flaskel-3.0.3/flaskel/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2551 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/utils/datastruct.py
--rw-rw-rw-   0 root         (0) root         (0)     3433 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/utils/logger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-19 21:12:32.377129 Flaskel-3.0.3/flaskel/utils/schemas/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/utils/schemas/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5018 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/utils/schemas/default.py
--rw-rw-rw-   0 root         (0) root         (0)    34444 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/utils/schemas/openapi3.py
--rw-rw-rw-   0 root         (0) root         (0)     1263 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/utils/validator.py
--rw-rw-rw-   0 root         (0) root         (0)     2765 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/utils/webargs.py
--rw-rw-rw-   0 root         (0) root         (0)      252 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-19 21:12:32.380129 Flaskel-3.0.3/flaskel/views/
--rw-rw-rw-   0 root         (0) root         (0)      105 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/views/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7003 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/views/base.py
--rw-rw-rw-   0 root         (0) root         (0)     9044 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/views/proxy.py
--rw-rw-rw-   0 root         (0) root         (0)     7823 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/views/resource.py
--rw-rw-rw-   0 root         (0) root         (0)     5646 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/views/rpc.py
--rw-rw-rw-   0 root         (0) root         (0)     1210 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/views/static.py
--rw-rw-rw-   0 root         (0) root         (0)     1155 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/views/template.py
--rw-rw-rw-   0 root         (0) root         (0)     2756 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/views/token.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-19 21:12:32.383129 Flaskel-3.0.3/flaskel/wsgi/
--rw-rw-rw-   0 root         (0) root         (0)      102 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/wsgi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      861 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/wsgi/base.py
--rw-rw-rw-   0 root         (0) root         (0)      790 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/wsgi/factory.py
--rw-rw-rw-   0 root         (0) root         (0)      584 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/wsgi/wsgi_gevent.py
--rw-rw-rw-   0 root         (0) root         (0)     4389 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/wsgi/wsgi_gunicorn.py
--rw-rw-rw-   0 root         (0) root         (0)      656 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/wsgi/wsgi_tornado.py
--rw-rw-rw-   0 root         (0) root         (0)      856 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/wsgi/wsgi_twisted.py
--rw-rw-rw-   0 root         (0) root         (0)      411 2022-06-19 21:12:15.000000 Flaskel-3.0.3/flaskel/wsgi/wsgi_waitress.py
--rw-r--r--   0 root         (0) root         (0)       38 2022-06-19 21:12:32.384130 Flaskel-3.0.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     4627 2022-06-19 21:12:15.000000 Flaskel-3.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 21:39:53.264777 Flaskel-3.1.0rc2/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 21:39:53.243777 Flaskel-3.1.0rc2/Flaskel.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    15616 2023-05-25 21:39:53.000000 Flaskel-3.1.0rc2/Flaskel.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4585 2023-05-25 21:39:53.000000 Flaskel-3.1.0rc2/Flaskel.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 21:39:53.000000 Flaskel-3.1.0rc2/Flaskel.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       52 2023-05-25 21:39:53.000000 Flaskel-3.1.0rc2/Flaskel.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 21:39:53.000000 Flaskel-3.1.0rc2/Flaskel.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      893 2023-05-25 21:39:53.000000 Flaskel-3.1.0rc2/Flaskel.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-25 21:39:53.000000 Flaskel-3.1.0rc2/Flaskel.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      123 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    15616 2023-05-25 21:39:53.264777 Flaskel-3.1.0rc2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    14795 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 21:39:53.244777 Flaskel-3.1.0rc2/flaskel/
+-rw-rw-rw-   0 root         (0) root         (0)      712 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12156 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/builder.py
+-rw-rw-rw-   0 root         (0) root         (0)     9054 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     1188 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/converters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 21:39:53.247777 Flaskel-3.1.0rc2/flaskel/ext/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/ext/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7321 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/ext/auth.py
+-rw-rw-rw-   0 root         (0) root         (0)     4245 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/ext/caching.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 21:39:53.247777 Flaskel-3.1.0rc2/flaskel/ext/crypto/
+-rw-rw-rw-   0 root         (0) root         (0)       26 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/ext/crypto/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1777 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/ext/crypto/argon.py
+-rw-rw-rw-   0 root         (0) root         (0)      885 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/ext/datetime.py
+-rw-rw-rw-   0 root         (0) root         (0)     1278 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/ext/default.py
+-rw-rw-rw-   0 root         (0) root         (0)      646 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/ext/errors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 21:39:53.247777 Flaskel-3.1.0rc2/flaskel/ext/healthcheck/
+-rw-rw-rw-   0 root         (0) root         (0)      203 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/ext/healthcheck/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6601 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/ext/healthcheck/checkers.py
+-rw-rw-rw-   0 root         (0) root         (0)     4957 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/ext/healthcheck/health.py
+-rw-rw-rw-   0 root         (0) root         (0)     7842 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/ext/ipban.py
+-rw-rw-rw-   0 root         (0) root         (0)     5419 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/ext/jobs.py
+-rw-rw-rw-   0 root         (0) root         (0)     1309 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/ext/limit.py
+-rw-rw-rw-   0 root         (0) root         (0)     6072 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/ext/mongo.py
+-rw-rw-rw-   0 root         (0) root         (0)     1045 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/ext/redis.py
+-rw-rw-rw-   0 root         (0) root         (0)     1605 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/ext/sendmail.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 21:39:53.248777 Flaskel-3.1.0rc2/flaskel/ext/sqlalchemy/
+-rw-rw-rw-   0 root         (0) root         (0)       83 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/ext/sqlalchemy/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2402 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/ext/sqlalchemy/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     1020 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/ext/useragent.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 21:39:53.248777 Flaskel-3.1.0rc2/flaskel/ext/websocket/
+-rw-rw-rw-   0 root         (0) root         (0)      526 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/ext/websocket/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 21:39:53.249777 Flaskel-3.1.0rc2/flaskel/extra/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/extra/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8963 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/extra/account.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 21:39:53.249777 Flaskel-3.1.0rc2/flaskel/extra/apidoc/
+-rw-rw-rw-   0 root         (0) root         (0)       54 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/extra/apidoc/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2515 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/extra/apidoc/template.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 21:39:53.250777 Flaskel-3.1.0rc2/flaskel/extra/media/
+-rw-rw-rw-   0 root         (0) root         (0)      111 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/extra/media/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       82 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/extra/media/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     2127 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/extra/media/repo.py
+-rw-rw-rw-   0 root         (0) root         (0)     2214 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/extra/media/service.py
+-rw-rw-rw-   0 root         (0) root         (0)     1144 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/extra/media/view.py
+-rw-rw-rw-   0 root         (0) root         (0)    11414 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/extra/mobile_support.py
+-rw-rw-rw-   0 root         (0) root         (0)     5218 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/extra/notification.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 21:39:53.250777 Flaskel-3.1.0rc2/flaskel/extra/payments/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/extra/payments/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 21:39:53.251777 Flaskel-3.1.0rc2/flaskel/extra/payments/stripe/
+-rw-rw-rw-   0 root         (0) root         (0)      135 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/extra/payments/stripe/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3529 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/extra/payments/stripe/handler.py
+-rw-rw-rw-   0 root         (0) root         (0)     2831 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/extra/payments/stripe/repo.py
+-rw-rw-rw-   0 root         (0) root         (0)     1374 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/extra/payments/stripe/view.py
+-rw-rw-rw-   0 root         (0) root         (0)     4678 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/flaskel.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 21:39:53.251777 Flaskel-3.1.0rc2/flaskel/http/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/http/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2223 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/http/client.py
+-rw-rw-rw-   0 root         (0) root         (0)     9019 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/http/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     7168 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/middlewares.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 21:39:53.252777 Flaskel-3.1.0rc2/flaskel/scripts/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/scripts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      253 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/scripts/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     1425 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/scripts/init_app.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 21:39:53.241777 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 21:39:53.253777 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/resources/
+-rw-rw-rw-   0 root         (0) root         (0)      305 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/resources/Caddyfile.example
+-rw-rw-rw-   0 root         (0) root         (0)      532 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/resources/conf.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     2271 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/resources/log.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      757 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/resources/manage.sh
+-rw-rw-rw-   0 root         (0) root         (0)      414 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/resources/nginx.example
+-rw-rw-rw-   0 root         (0) root         (0)     1561 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/resources/nuisances.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1325 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/resources/schemas.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1775 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/resources/settings.ini.sample
+-rw-rw-rw-   0 root         (0) root         (0)      492 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/resources/supervisor.example
+-rw-rw-rw-   0 root         (0) root         (0)    14323 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/resources/swagger.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      139 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/resources/uwsgi.yaml.example
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 21:39:53.254777 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/skel/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 21:39:53.254777 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/skel/ext/
+-rw-rw-rw-   0 root         (0) root         (0)     1768 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/skel/ext/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      434 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/skel/ext/auth.py
+-rw-rw-rw-   0 root         (0) root         (0)       63 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/skel/ext/database.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 21:39:53.254777 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/skel/forms/
+-rw-rw-rw-   0 root         (0) root         (0)      330 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/skel/forms/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 21:39:53.255777 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/skel/models/
+-rw-rw-rw-   0 root         (0) root         (0)       69 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/skel/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      189 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/skel/models/user.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 21:39:53.255777 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/skel/scripts/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/skel/scripts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      685 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/skel/scripts/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      504 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/skel/scripts/config.py
+-rw-rw-rw-   0 root         (0) root         (0)      915 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/skel/scripts/ws.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 21:39:53.255777 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/skel/tasks/
+-rw-rw-rw-   0 root         (0) root         (0)       57 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/skel/tasks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      252 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/skel/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 21:39:53.256777 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/skel/views/
+-rw-rw-rw-   0 root         (0) root         (0)      856 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/skel/views/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1010 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/skel/views/blueprints.py
+-rw-rw-rw-   0 root         (0) root         (0)     1672 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/skel/views/common.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 21:39:53.240777 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/skel/views/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 21:39:53.256777 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/skel/views/static/css/
+-rw-rw-rw-   0 root         (0) root         (0)      190 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/skel/views/static/css/main.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 21:39:53.256777 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/skel/views/static/img/
+-rw-rw-rw-   0 root         (0) root         (0)      318 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/skel/views/static/img/favicon.ico
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 21:39:53.256777 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/skel/views/static/js/
+-rw-rw-rw-   0 root         (0) root         (0)       35 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/skel/views/static/js/main.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 21:39:53.257777 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/skel/views/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 21:39:53.257777 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/skel/views/templates/core/
+-rw-rw-rw-   0 root         (0) root         (0)      206 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/skel/views/templates/core/error.html
+-rw-rw-rw-   0 root         (0) root         (0)     1103 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/skel/views/templates/core/head.html
+-rw-rw-rw-   0 root         (0) root         (0)      655 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/skel/views/templates/core/scripts.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 21:39:53.257777 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/skel/views/templates/emails/
+-rw-rw-rw-   0 root         (0) root         (0)      220 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/skel/views/templates/emails/forgot.html
+-rw-rw-rw-   0 root         (0) root         (0)      225 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/skel/views/templates/emails/registration.html
+-rw-rw-rw-   0 root         (0) root         (0)    13479 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/skel/views/templates/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 21:39:53.258777 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/skel/views/templates/layout/
+-rw-rw-rw-   0 root         (0) root         (0)      458 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/skel/views/templates/layout/base.html
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/skel/views/templates/layout/container.html
+-rw-rw-rw-   0 root         (0) root         (0)       20 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/skel/views/templates/layout/footer.html
+-rw-rw-rw-   0 root         (0) root         (0)       20 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/skel/views/templates/layout/header.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 21:39:53.259777 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2433 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)      190 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/tests/helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)     2167 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/tests/test_smoke.py
+-rw-rw-rw-   0 root         (0) root         (0)     5319 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/standalone.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 21:39:53.259777 Flaskel-3.1.0rc2/flaskel/tester/
+-rw-rw-rw-   0 root         (0) root         (0)       31 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/tester/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1432 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/tester/client.py
+-rw-rw-rw-   0 root         (0) root         (0)     7354 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/tester/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 21:39:53.260777 Flaskel-3.1.0rc2/flaskel/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2551 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/utils/datastruct.py
+-rw-rw-rw-   0 root         (0) root         (0)     3433 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/utils/logger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 21:39:53.261777 Flaskel-3.1.0rc2/flaskel/utils/schemas/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/utils/schemas/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5018 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/utils/schemas/default.py
+-rw-rw-rw-   0 root         (0) root         (0)    34444 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/utils/schemas/openapi3.py
+-rw-rw-rw-   0 root         (0) root         (0)     1263 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/utils/validator.py
+-rw-rw-rw-   0 root         (0) root         (0)     2765 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/utils/webargs.py
+-rw-rw-rw-   0 root         (0) root         (0)      256 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 21:39:53.262777 Flaskel-3.1.0rc2/flaskel/views/
+-rw-rw-rw-   0 root         (0) root         (0)      105 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/views/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7046 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/views/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     9130 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/views/proxy.py
+-rw-rw-rw-   0 root         (0) root         (0)     7866 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/views/resource.py
+-rw-rw-rw-   0 root         (0) root         (0)     5689 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/views/rpc.py
+-rw-rw-rw-   0 root         (0) root         (0)     1210 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/views/static.py
+-rw-rw-rw-   0 root         (0) root         (0)     1185 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/views/template.py
+-rw-rw-rw-   0 root         (0) root         (0)     2820 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/views/token.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 21:39:53.263777 Flaskel-3.1.0rc2/flaskel/wsgi/
+-rw-rw-rw-   0 root         (0) root         (0)      102 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/wsgi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      861 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/wsgi/base.py
+-rw-rw-rw-   0 root         (0) root         (0)      790 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/wsgi/factory.py
+-rw-rw-rw-   0 root         (0) root         (0)      584 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/wsgi/wsgi_gevent.py
+-rw-rw-rw-   0 root         (0) root         (0)     4389 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/wsgi/wsgi_gunicorn.py
+-rw-rw-rw-   0 root         (0) root         (0)      656 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/wsgi/wsgi_tornado.py
+-rw-rw-rw-   0 root         (0) root         (0)      856 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/wsgi/wsgi_twisted.py
+-rw-rw-rw-   0 root         (0) root         (0)      411 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/wsgi/wsgi_waitress.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-25 21:39:53.264777 Flaskel-3.1.0rc2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     4611 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/setup.py
```

### Comparing `Flaskel-3.0.3/Flaskel.egg-info/PKG-INFO` & `Flaskel-3.1.0rc2/Flaskel.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flaskel
-Version: 3.0.3
+Version: 3.1.0rc2
 Summary: Skeleton for flask applications
 Home-page: https://github.com/cs91chris/flaskel
 Author: cs91chris
 Author-email: cs91chris@voidbrain.me
 License: MIT
 Platform: any
 Classifier: Environment :: Web Environment
@@ -451,9 +451,7 @@
 
 - flaskel.extra.media.service.MediaService
   - ``MEDIA``: *(dict)*
     - ``ALLOWED_EXTENSIONS``: *(default: [png,jpg])*
     - ``UPLOAD_FOLDER``:
     - ``EXTERNAL_URL``:
 
-
-
```

### Comparing `Flaskel-3.0.3/Flaskel.egg-info/SOURCES.txt` & `Flaskel-3.1.0rc2/Flaskel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Flaskel-3.0.3/Flaskel.egg-info/requires.txt` & `Flaskel-3.1.0rc2/Flaskel.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,14 @@
 webargs
 aiohttp
 nest-asyncio
 vbcore[all]
 pyfcm
 stripe
 redis
-rejson
 hiredis
 Flask-Mail
 Flask-APScheduler
 flask_pymongo
 
 [test]
 Flask
@@ -57,15 +56,14 @@
 webargs
 aiohttp
 nest-asyncio
 vbcore[all]
 pyfcm
 stripe
 redis
-rejson
 hiredis
 Flask-Mail
 Flask-APScheduler
 flask_pymongo
 coverage
 pytest
 pytest-cov
```

### Comparing `Flaskel-3.0.3/PKG-INFO` & `Flaskel-3.1.0rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flaskel
-Version: 3.0.3
+Version: 3.1.0rc2
 Summary: Skeleton for flask applications
 Home-page: https://github.com/cs91chris/flaskel
 Author: cs91chris
 Author-email: cs91chris@voidbrain.me
 License: MIT
 Platform: any
 Classifier: Environment :: Web Environment
@@ -451,9 +451,7 @@
 
 - flaskel.extra.media.service.MediaService
   - ``MEDIA``: *(dict)*
     - ``ALLOWED_EXTENSIONS``: *(default: [png,jpg])*
     - ``UPLOAD_FOLDER``:
     - ``EXTERNAL_URL``:
 
-
-
```

### Comparing `Flaskel-3.0.3/README.md` & `Flaskel-3.1.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `Flaskel-3.0.3/flaskel/__init__.py` & `Flaskel-3.1.0rc2/flaskel/__init__.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.0.3/flaskel/builder.py` & `Flaskel-3.1.0rc2/flaskel/builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import sys
 import typing as t
 
 from flask import Blueprint
 from flask.typing import AfterRequestCallable, BeforeRequestCallable
 from jinja2 import ChoiceLoader, FileSystemLoader
-from vbcore.db.events import register_engine_events
+from vbcore.db.support import SQLASupport
 from vbcore.misc import random_string
 from werkzeug.middleware.lint import LintMiddleware
 from werkzeug.middleware.profiler import ProfilerMiddleware
 from werkzeug.routing import BaseConverter
 
 from flaskel import config, flaskel
 
@@ -276,16 +276,16 @@
         if self._app is not None:
             self._app.logger.debug("Registered routes:\n%s", DumpUrls(self._app))
 
     def init_db(self):
         try:
             sqlalchemy = self._app.extensions.get("sqlalchemy")
             if sqlalchemy is not None:
-                register_engine_events(sqlalchemy.db.engine)
-                sqlalchemy.db.create_all(app=self._app)
+                SQLASupport.register_custom_handlers(sqlalchemy.db.engine)
+                sqlalchemy.db.create_all()
         except Exception as exc:  # pylint: disable=broad-except
             self._app.logger.exception(exc)
 
     def after_create_hook(self):
         self.dump_urls()
 
         if self._app.debug:
```

### Comparing `Flaskel-3.0.3/flaskel/config.py` & `Flaskel-3.1.0rc2/flaskel/config.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.0.3/flaskel/converters.py` & `Flaskel-3.1.0rc2/flaskel/converters.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.0.3/flaskel/ext/auth.py` & `Flaskel-3.1.0rc2/flaskel/ext/auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,16 @@
     create_refresh_token,
     decode_token,
     get_jwt,
     get_jwt_identity,
     jwt_required,
     JWTManager,
 )
-from vbcore.datastruct import DataClassDictable, ObjectDict
+from vbcore.base import BaseDTO
+from vbcore.datastruct import ObjectDict
 from vbcore.db.mixins import StandardMixin
 from vbcore.http import httpcode
 
 from flaskel.flaskel import cap
 from flaskel.http.exceptions import abort
 
 token_auth: JWTManager = JWTManager()
@@ -49,27 +50,27 @@
     @classmethod
     def is_block_listed(cls, jti: str) -> bool:
         # noinspection PyUnresolvedReferences
         return bool(cls.query.filter_by(jti=jti).first())
 
 
 @dataclasses.dataclass(frozen=True)
-class TokenInfo(DataClassDictable):
+class TokenInfo(BaseDTO):
     fresh: bool
     expires_in: int
     issued_at: int
     token_type: str
     type: str
     jti: str
     identity: dict
     scope: t.Optional[str] = None
 
 
 @dataclasses.dataclass(frozen=True)
-class TokenData(DataClassDictable):
+class TokenData(BaseDTO):
     access_token: str
     expires_in: int
     issued_at: int
     token_type: str
     scope: t.Optional[str] = None
     refresh_token: t.Optional[str] = None
```

### Comparing `Flaskel-3.0.3/flaskel/ext/caching.py` & `Flaskel-3.1.0rc2/flaskel/ext/caching.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.0.3/flaskel/ext/crypto/argon.py` & `Flaskel-3.1.0rc2/flaskel/ext/crypto/argon.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import typing as t
 
 import argon2
-from vbcore.crypto.argon import Argon2 as HasherArgon2
+from vbcore.crypto.argon import Argon2 as HasherArgon2, Argon2Options
 
 
 class Argon2:
     CONFIG_PREFIX = "ARGON2_"
     PROFILES: t.Dict[str, argon2.Parameters] = {
         "low": argon2.profiles.RFC_9106_LOW_MEMORY,
         "high": argon2.profiles.RFC_9106_HIGH_MEMORY,
@@ -32,13 +32,15 @@
         app.config.setdefault(f"{cls.CONFIG_PREFIX}HASH_LEN", params.hash_len)
         app.config.setdefault(f"{cls.CONFIG_PREFIX}MEMORY_COST", params.memory_cost)
         app.config.setdefault(f"{cls.CONFIG_PREFIX}PARALLELISM", params.parallelism)
         app.config.setdefault(f"{cls.CONFIG_PREFIX}SALT_LEN", params.salt_len)
 
     def init_app(self, app, argon_class: t.Type[HasherArgon2] = HasherArgon2):
         self.set_default_config(app)
-        self._argon = argon_class(**app.config.get_namespace(self.CONFIG_PREFIX))
+        self._argon = argon_class(
+            Argon2Options(**app.config.get_namespace(self.CONFIG_PREFIX))
+        )
         setattr(app, "extensions", getattr(app, "extensions", {}))
         app.extensions["argon2"] = self
 
     def __getattr__(self, item):
         return getattr(self._argon, item)
```

### Comparing `Flaskel-3.0.3/flaskel/ext/default.py` & `Flaskel-3.1.0rc2/flaskel/ext/default.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.0.3/flaskel/ext/errors.py` & `Flaskel-3.1.0rc2/flaskel/ext/errors.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.0.3/flaskel/ext/healthcheck/checkers.py` & `Flaskel-3.1.0rc2/flaskel/ext/healthcheck/checkers.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.0.3/flaskel/ext/healthcheck/health.py` & `Flaskel-3.1.0rc2/flaskel/ext/healthcheck/health.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import enum
 import typing as t
 from functools import partial, wraps
 
 from flask import Blueprint
 from vbcore.batch import BatchExecutor
-from vbcore.datastruct import LStrEnum
+from vbcore.enums import LStrEnum
 from vbcore.http import httpcode, HttpMethod
 from vbcore.http.headers import ContentTypeEnum, HeaderEnum
 
 from flaskel.flaskel import Flaskel, request
 
 from .checkers import CheckerResponseType
```

### Comparing `Flaskel-3.0.3/flaskel/ext/ipban.py` & `Flaskel-3.1.0rc2/flaskel/ext/ipban.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,15 +150,15 @@
         if self.is_blacklisted(ip):
             return True
 
         return self.repo.attempts(ip) >= self.max_attempts
 
 
 class FlaskIPBan:
-    def __init__(self, app=None, **kwargs):
+    def __init__(self, app=None, **kwargs) -> None:
         self.service: t.Optional[IpBanService] = None
         self.backends: t.Dict[str, t.Type[IBanRepo]] = {}
 
         self.register_backend("local", BanRepoLocal, client_class=ExpiringCache)
         self.register_backend("redis", BanRepoRedis, client=client_redis)
 
         if app is not None:
@@ -225,12 +225,12 @@
             if attempts:
                 cap.logger.info("%s added to ban list with attempts: %s", ip, attempts)
         return response
 
     def before_request_hook(self):
         ip = self.get_ip()
         if self.service.is_banned(ip):
-            cap.logger.warn("%s is banned", ip)
+            cap.logger.warning("%s is banned", ip)
             abort(cap.config.IPBAN_STATUS_CODE)
 
 
 ipban = FlaskIPBan()
```

### Comparing `Flaskel-3.0.3/flaskel/ext/jobs.py` & `Flaskel-3.1.0rc2/flaskel/ext/jobs.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.0.3/flaskel/ext/limit.py` & `Flaskel-3.1.0rc2/flaskel/ext/limit.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.0.3/flaskel/ext/mongo.py` & `Flaskel-3.1.0rc2/flaskel/ext/mongo.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.0.3/flaskel/ext/redis.py` & `Flaskel-3.1.0rc2/flaskel/ext/redis.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.0.3/flaskel/ext/sendmail.py` & `Flaskel-3.1.0rc2/flaskel/ext/sendmail.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.0.3/flaskel/ext/sqlalchemy/model.py` & `Flaskel-3.1.0rc2/flaskel/ext/sqlalchemy/model.py`

 * *Files 22% similar despite different names*

```diff
@@ -54,15 +54,20 @@
     ):
         q = cls.query_collection(*args, **kwargs)
 
         if order_by is not None:
             q = q.order_by(*order_by)
 
         if page or page_size:
-            q = q.paginate(page, page_size, False, max_per_page)
+            q = q.paginate(
+                page=page,
+                per_page=page_size,
+                error_out=False,
+                max_per_page=max_per_page,
+            )
             res = q.items
             if to_dict is False:
                 return q
         else:
             res = q.all()
 
         if to_dict is True:
```

### Comparing `Flaskel-3.0.3/flaskel/ext/useragent.py` & `Flaskel-3.1.0rc2/flaskel/ext/useragent.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.0.3/flaskel/ext/websocket/__init__.py` & `Flaskel-3.1.0rc2/flaskel/ext/websocket/__init__.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.0.3/flaskel/extra/account.py` & `Flaskel-3.1.0rc2/flaskel/extra/account.py`

 * *Files 1% similar despite different names*

```diff
@@ -204,15 +204,15 @@
             cap.logger.exception(exc)
             self.session.rollback()
             abort(httpcode.INTERNAL_SERVER_ERROR)
 
 
 class BaseAccountView(BaseView):
     account_handler: AccountHandler = t.cast(AccountHandler, ExtProxy("account"))
-    methods = [
+    methods: t.ClassVar[t.Optional[t.Collection[str]]] = [
         HttpMethod.POST,
         HttpMethod.PUT,
     ]
 
     DEFAULT_SCHEMAS = ObjectDict(
         REGISTER=Fields.object(
             properties={"email": Fields.string, "password": Fields.string}
```

### Comparing `Flaskel-3.0.3/flaskel/extra/apidoc/template.py` & `Flaskel-3.1.0rc2/flaskel/extra/apidoc/template.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.0.3/flaskel/extra/media/repo.py` & `Flaskel-3.1.0rc2/flaskel/extra/media/repo.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.0.3/flaskel/extra/media/service.py` & `Flaskel-3.1.0rc2/flaskel/extra/media/service.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.0.3/flaskel/extra/media/view.py` & `Flaskel-3.1.0rc2/flaskel/extra/media/view.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,22 @@
+import typing as t
+
 from vbcore.http import httpcode, HttpMethod
 
 from flaskel import abort, cap, request
 from flaskel.views import BaseView
 from flaskel.views.static import StaticFileView
 
 from .exceptions import BadMediaError
 from .service import MediaService
 
 
 class ApiMedia(BaseView):
     service = MediaService
-    methods = [
+    methods: t.ClassVar[t.Optional[t.Collection[str]]] = [
         HttpMethod.POST,
         HttpMethod.DELETE,
     ]
     default_urls = (
         "/resources/<int:eid>/media",
         "/resources/<int:eid>/media/<int:res_id>",
     )
```

### Comparing `Flaskel-3.0.3/flaskel/extra/mobile_support.py` & `Flaskel-3.1.0rc2/flaskel/extra/mobile_support.py`

 * *Files 1% similar despite different names*

```diff
@@ -202,15 +202,15 @@
 
 
 class MobileReleaseView(BaseView):
     builder = builder
     ext: MobileVersionCompatibility = t.cast(
         MobileVersionCompatibility, ExtProxy("mobile_version")
     )
-    methods = [
+    methods: t.ClassVar[t.Optional[t.Collection[str]]] = [
         HttpMethod.POST,
         HttpMethod.GET,
         HttpMethod.DELETE,
     ]
 
     default_view_name = "mobile_release"
     default_urls = (
@@ -227,17 +227,18 @@
     )
     def dispatch_request(self, params: dict, *_, ver=None, **__):
         agent = params["agent"]
         if agent not in cap.config.VERSION_AGENTS:
             return abort(
                 httpcode.BAD_REQUEST,
                 response=Response(
-                    dict(
-                        reason="agent not compatible", agents=cap.config.VERSION_AGENTS
-                    )
+                    {
+                        "reason": "agent not compatible",
+                        "agents": cap.config.VERSION_AGENTS,
+                    }
                 ),
             )
 
         if ver == "latest":
             return self.ext.latest(agent) or "", {
                 HeaderEnum.CONTENT_TYPE: ContentTypeEnum.PLAIN
             }
@@ -262,15 +263,15 @@
 
 class MobileLoggerView(BaseView):
     unavailable = "N/A"
     intro = "An exception occurred on mobile app:"
     default_view_name = "mobile_logger"
     default_urls = ("/mobile/logger",)
 
-    methods = [
+    methods: t.ClassVar[t.Optional[t.Collection[str]]] = [
         HttpMethod.POST,
     ]
     decorators = [
         builder.no_content,
         RateLimit.medium(),
         RateLimit.fail(),
     ]
```

### Comparing `Flaskel-3.0.3/flaskel/extra/notification.py` & `Flaskel-3.1.0rc2/flaskel/extra/notification.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,15 +119,15 @@
             )
         except FCMError as exc:  # pragma: no cover
             self.app.logger.exception(exc)
             return None
 
 
 class DeviceRegisterView(BaseView):
-    methods = [HttpMethod.POST]
+    methods: t.ClassVar[t.Optional[t.Collection[str]]] = [HttpMethod.POST]
     default_view_name = "fcm_device_register"
     default_urls = ("/device/register",)
     handler = ExtProxy("fcm_notification")
     schema = "DEVICE_REGISTER"
 
     def get_user_id(self):
         """must be implemented in subclass"""
@@ -141,15 +141,15 @@
             self.handler.register_device,
             args=(payload,),
         )
         return Response.no_content()
 
 
 class SendPushView(BaseView):
-    methods = [HttpMethod.POST]
+    methods: t.ClassVar[t.Optional[t.Collection[str]]] = [HttpMethod.POST]
     default_view_name = "fcm_send"
     default_urls = ("/send/push",)
     handler = ExtProxy("fcm_notification")
     schema = "SEND_PUSH"
 
     def dispatch_request(self, *_, **__):
         payload = PayloadValidator.validate(self.schema)
```

### Comparing `Flaskel-3.0.3/flaskel/extra/payments/stripe/handler.py` & `Flaskel-3.1.0rc2/flaskel/extra/payments/stripe/handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 
 class PaymentHandler:
     handler = stripe
     payment_intent_ok: str = "payment_intent.succeeded"
     payment_intent_ko: str = "payment_intent.payment_failed"
 
-    def __init__(self, app=None, **kwargs):
+    def __init__(self, app=None, **kwargs) -> None:
         self._error: CallbackType = partial(self._not_registered, "on_error")
         self._success: CallbackType = partial(self._not_registered, "on_success")
 
         if app is not None:
             self.init_app(app, **kwargs)
 
     @staticmethod
```

### Comparing `Flaskel-3.0.3/flaskel/extra/payments/stripe/repo.py` & `Flaskel-3.1.0rc2/flaskel/extra/payments/stripe/repo.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 from datetime import datetime
 
 import sqlalchemy as sa
 from sqlalchemy.ext.declarative import declared_attr
 from vbcore import json
-from vbcore.datastruct import IntEnum, ObjectDict
+from vbcore.datastruct import ObjectDict
 from vbcore.db.mixins import CatalogMixin, StandardMixin
 from vbcore.db.sqla import LoaderModel
+from vbcore.enums import IntEnum
 
 
 class PaymentStatusValue(IntEnum):
     WAIT = 1
     SUCCESS = 2
     ERROR = 3
 
 
 class PaymentStatus(CatalogMixin, LoaderModel):
     __abstract__ = True
 
     values = PaymentStatusValue.to_list()
 
     def to_dict(self, **__):
-        return ObjectDict(id=self.id, stato=self.label)
+        return ObjectDict(id=self.id, stato=self.code)
 
 
 class Payment(StandardMixin):
     _status_model = PaymentStatus
 
     request_id = sa.Column(sa.String(255), unique=True, nullable=False)
     response_id = sa.Column(sa.String(255), unique=True)
```

### Comparing `Flaskel-3.0.3/flaskel/extra/payments/stripe/view.py` & `Flaskel-3.1.0rc2/flaskel/extra/payments/stripe/view.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,21 @@
+import typing as t
+
 from vbcore.http import HttpMethod
 
 from flaskel import db_session, ExtProxy, Response
 from flaskel.views import BaseView
 
 from .repo import Payment, PaymentRepo
 
 
 class PaymentView(BaseView):
     model = Payment
     repo_class = PaymentRepo
-    methods = [HttpMethod.POST]
+    methods: t.ClassVar[t.Optional[t.Collection[str]]] = [HttpMethod.POST]
     gateway = ExtProxy("stripe")
 
     def __init__(self, session=None):
         self.repo = self.repo_class(session or db_session, self.model)
 
 
 class PaymentIntentView(PaymentView):
```

### Comparing `Flaskel-3.0.3/flaskel/flaskel.py` & `Flaskel-3.1.0rc2/flaskel/flaskel.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import os.path
 import typing as t
 
 import flask
-from vbcore.datastruct import Dumper, ObjectDict
+from vbcore.datastruct import ObjectDict
+from vbcore.datastruct.lazy import Dumper
 from vbcore.http import httpcode
 from vbcore.http.headers import HeaderEnum
-from vbcore.json import JsonEncoder
+from vbcore.json import JsonDecoder, JsonEncoder
+from vbcore.types import OptStr
 from werkzeug.routing import Rule
 from werkzeug.utils import safe_join
 
 from flaskel.utils.datastruct import Pagination
 
 cap: "Flaskel" = t.cast("Flaskel", flask.current_app)
 request: "Request" = t.cast("Request", flask.request)
@@ -94,18 +96,18 @@
 
         try:
             response = flask.send_file(file_path, etag=True, conditional=True, **kwargs)
         except IOError as exc:
             cap.logger.warning(str(exc))
             return flask.abort(httpcode.NOT_FOUND)
 
-        if cap.use_x_sendfile is True and cap.config.ENABLE_ACCEL is True:
+        if cap.config.USE_X_SENDFILE is True and cap.config.ENABLE_ACCEL is True:
             # following headers works with nginx compatible proxy
-            return cls.set_sendfile_headers(response, file_path)
-        return response
+            return cls.set_sendfile_headers(response, file_path)  # type: ignore
+        return response  # type: ignore
 
     def get_json(self, *args, **kwargs) -> ObjectDict:
         return ObjectDict.normalize(super().get_json(*args, **kwargs))
 
     @classmethod
     def pagination_headers(cls, total: int, pagination: Pagination) -> t.Dict[str, int]:
         return {
@@ -116,13 +118,14 @@
         }
 
 
 class Flaskel(flask.Flask):
     config_class = Config
     request_class = Request
     response_class = Response
-    json_encoder = JsonEncoder
+    _json_encoder = JsonEncoder
+    _json_decoder = JsonDecoder
 
-    def __init__(self, *args, **kwargs):
+    def __init__(self, *args, **kwargs) -> None:
         super().__init__(*args, **kwargs)
-        self.version = None
+        self.version: OptStr = None
         self.config: Config
```

### Comparing `Flaskel-3.0.3/flaskel/http/client.py` & `Flaskel-3.1.0rc2/flaskel/http/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,22 @@
 import typing as t
 
 from requests import exceptions as http_exc
-from vbcore.datastruct import Dumper
 from vbcore.http.batch import HTTPBatch
 from vbcore.http.client import HTTPClient, JsonRPCClient
-from vbcore.http.httpdumper import BaseHTTPDumper
+from vbcore.http.httpdumper import LazyHTTPDumper
 from vbcore.uuid import get_uuid
 
 from flaskel.flaskel import cap, request
 
 HTTPStatusError = (http_exc.HTTPError,)
 NetworkError = (http_exc.ConnectionError, http_exc.Timeout)
 all_errors = (*HTTPStatusError, *NetworkError)
 
 
-class LazyHTTPDumper(BaseHTTPDumper):
-    @classmethod
-    def dump_request(cls, req, *args, **kwargs):
-        return Dumper(req, *args, callback=super().dump_request, **kwargs)
-
-    @classmethod
-    def dump_response(cls, resp, *args, **kwargs):
-        return Dumper(resp, *args, callback=super().dump_response, **kwargs)
-
-
 class FlaskelHTTPDumper(LazyHTTPDumper):
     @classmethod
     def dump_request(cls, req, *_, dump_body=None, **kwargs):
         h = cap.config.LOG_REQ_HEADERS
         return super().dump_request(req, dump_body, only_hdr=h, **kwargs)
 
     @classmethod
```

### Comparing `Flaskel-3.0.3/flaskel/http/exceptions.py` & `Flaskel-3.1.0rc2/flaskel/http/exceptions.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.0.3/flaskel/middlewares.py` & `Flaskel-3.1.0rc2/flaskel/middlewares.py`

 * *Files 1% similar despite different names*

```diff
@@ -188,8 +188,8 @@
         :return: Whether the Request ID is unique or not
         """
         conf = self.get_config()
         prefix = conf.REQUEST_ID_PREFIX or self.request_id_prefix
         if prefix and request_id.startswith(prefix):
             return True  # pragma: no cover
 
-        return uuid.check_uuid(request_id, exc=False)
+        return uuid.check_uuid(request_id, raise_exc=False)
```

### Comparing `Flaskel-3.0.3/flaskel/scripts/init_app.py` & `Flaskel-3.1.0rc2/flaskel/scripts/init_app.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.0.3/flaskel/scripts/skeleton/resources/conf.yaml` & `Flaskel-3.1.0rc2/flaskel/scripts/skeleton/resources/conf.yaml`

 * *Files identical despite different names*

### Comparing `Flaskel-3.0.3/flaskel/scripts/skeleton/resources/log.yaml` & `Flaskel-3.1.0rc2/flaskel/scripts/skeleton/resources/log.yaml`

 * *Files identical despite different names*

### Comparing `Flaskel-3.0.3/flaskel/scripts/skeleton/resources/manage.sh` & `Flaskel-3.1.0rc2/flaskel/scripts/skeleton/resources/manage.sh`

 * *Files identical despite different names*

### Comparing `Flaskel-3.0.3/flaskel/scripts/skeleton/resources/nuisances.yaml` & `Flaskel-3.1.0rc2/flaskel/scripts/skeleton/resources/nuisances.yaml`

 * *Files identical despite different names*

### Comparing `Flaskel-3.0.3/flaskel/scripts/skeleton/resources/schemas.yaml` & `Flaskel-3.1.0rc2/flaskel/scripts/skeleton/resources/schemas.yaml`

 * *Files identical despite different names*

### Comparing `Flaskel-3.0.3/flaskel/scripts/skeleton/resources/settings.ini.sample` & `Flaskel-3.1.0rc2/flaskel/scripts/skeleton/resources/settings.ini.sample`

 * *Files identical despite different names*

### Comparing `Flaskel-3.0.3/flaskel/scripts/skeleton/resources/swagger.yaml` & `Flaskel-3.1.0rc2/flaskel/scripts/skeleton/resources/swagger.yaml`

 * *Files identical despite different names*

### Comparing `Flaskel-3.0.3/flaskel/scripts/skeleton/skel/ext/__init__.py` & `Flaskel-3.1.0rc2/flaskel/scripts/skeleton/skel/ext/__init__.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.0.3/flaskel/scripts/skeleton/skel/scripts/cli.py` & `Flaskel-3.1.0rc2/flaskel/scripts/skeleton/skel/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.0.3/flaskel/scripts/skeleton/skel/scripts/ws.py` & `Flaskel-3.1.0rc2/flaskel/scripts/skeleton/skel/scripts/ws.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.0.3/flaskel/scripts/skeleton/skel/views/__init__.py` & `Flaskel-3.1.0rc2/flaskel/scripts/skeleton/skel/views/__init__.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.0.3/flaskel/scripts/skeleton/skel/views/blueprints.py` & `Flaskel-3.1.0rc2/flaskel/scripts/skeleton/skel/views/blueprints.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.0.3/flaskel/scripts/skeleton/skel/views/common.py` & `Flaskel-3.1.0rc2/flaskel/scripts/skeleton/skel/views/common.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.0.3/flaskel/scripts/skeleton/skel/views/templates/core/head.html` & `Flaskel-3.1.0rc2/flaskel/scripts/skeleton/skel/views/templates/core/head.html`

 * *Files identical despite different names*

### Comparing `Flaskel-3.0.3/flaskel/scripts/skeleton/skel/views/templates/core/scripts.html` & `Flaskel-3.1.0rc2/flaskel/scripts/skeleton/skel/views/templates/core/scripts.html`

 * *Files identical despite different names*

### Comparing `Flaskel-3.0.3/flaskel/scripts/skeleton/skel/views/templates/index.html` & `Flaskel-3.1.0rc2/flaskel/scripts/skeleton/skel/views/templates/index.html`

 * *Files identical despite different names*

### Comparing `Flaskel-3.0.3/flaskel/scripts/skeleton/tests/conftest.py` & `Flaskel-3.1.0rc2/flaskel/scripts/skeleton/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.0.3/flaskel/scripts/skeleton/tests/test_smoke.py` & `Flaskel-3.1.0rc2/flaskel/scripts/skeleton/tests/test_smoke.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.0.3/flaskel/standalone.py` & `Flaskel-3.1.0rc2/flaskel/standalone.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.0.3/flaskel/tester/client.py` & `Flaskel-3.1.0rc2/flaskel/tester/client.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.0.3/flaskel/tester/helpers.py` & `Flaskel-3.1.0rc2/flaskel/tester/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import typing as t
 from functools import partial
 
 import flask
 from vbcore.db.support import SQLASupport
 from vbcore.http import httpcode, HttpMethod
+from vbcore.tester.asserter import Asserter
 from vbcore.tester.helpers import build_url
-from vbcore.tester.mixins import Asserter
 
 from flaskel import TestClient
 from flaskel.utils.datastruct import ConfigProxy
 
 config = ConfigProxy()
 schemas = ConfigProxy("SCHEMAS")
 url_for = partial(flask.url_for, _external=True)
@@ -56,15 +56,15 @@
                 code=(httpcode.SUCCESS - 1, httpcode.MULTIPLE_CHOICES - 1),
             )
 
         if response.data and (mimetype or self.mimetype):
             Asserter.assert_equals(response.mimetype, mimetype or self.mimetype)
 
         if schema:
-            Asserter.assert_schema(response.json, schema)
+            Asserter.assert_json_schema(response.json, schema)
 
         return response
 
     def post(
         self,
         url: t.Optional[str] = None,
         view: t.Optional[str] = None,
```

### Comparing `Flaskel-3.0.3/flaskel/utils/datastruct.py` & `Flaskel-3.1.0rc2/flaskel/utils/datastruct.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.0.3/flaskel/utils/logger.py` & `Flaskel-3.1.0rc2/flaskel/utils/logger.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.0.3/flaskel/utils/schemas/default.py` & `Flaskel-3.1.0rc2/flaskel/utils/schemas/default.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.0.3/flaskel/utils/schemas/openapi3.py` & `Flaskel-3.1.0rc2/flaskel/utils/schemas/openapi3.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.0.3/flaskel/utils/validator.py` & `Flaskel-3.1.0rc2/flaskel/utils/validator.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.0.3/flaskel/utils/webargs.py` & `Flaskel-3.1.0rc2/flaskel/utils/webargs.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.0.3/flaskel/views/base.py` & `Flaskel-3.1.0rc2/flaskel/views/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,19 +15,19 @@
     url: str
     endpoint: t.Optional[str] = None
     options: t.Optional[dict] = None
     provide_automatic_options: t.Optional[bool] = None
 
 
 class ViewSupportMixin:
-    methods = [
-        HttpMethod.GET,
-    ]
     default_view_name: str = ""
     default_urls: UrlsType = ()
+    methods: t.ClassVar[t.Optional[t.Collection[str]]] = [
+        HttpMethod.GET,
+    ]
 
     @staticmethod
     def not_implemented() -> t.NoReturn:  # pragma: no cover
         abort(httpcode.NOT_IMPLEMENTED)
 
     @classmethod
     def normalize_url(cls, url: str) -> str:
```

### Comparing `Flaskel-3.0.3/flaskel/views/proxy.py` & `Flaskel-3.1.0rc2/flaskel/views/proxy.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,15 +137,15 @@
         if not conf:
             cap.logger.warning(f"unable to find conf keys: {self.sep.join(keys)}")
             abort(httpcode.NOT_FOUND)
         return conf
 
 
 class TransparentProxyView(ProxyView):
-    methods = [
+    methods: t.ClassVar[t.Optional[t.Collection[str]]] = [
         HttpMethod.POST,
         HttpMethod.PUT,
         HttpMethod.GET,
         HttpMethod.DELETE,
     ]
 
     def __init__(
@@ -205,15 +205,15 @@
 
 
 class JsonRPCProxy(ProxyView):
     default_view_name: str = "jsonrpc_proxy"
     response_content_type: str = ContentTypeEnum.JSON
     client_class: t.Type[FlaskelJsonRPC] = FlaskelJsonRPC
 
-    methods = [
+    methods: t.ClassVar[t.Optional[t.Collection[str]]] = [
         HttpMethod.GET,
         HttpMethod.POST,
     ]
 
     def __init__(
         self,
         url: t.Optional[str] = None,
```

### Comparing `Flaskel-3.0.3/flaskel/views/resource.py` & `Flaskel-3.1.0rc2/flaskel/views/resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -241,15 +241,15 @@
         return res.to_dict(), status
 
 
 class PatchApiView(Restful):
     methods_subresource = None
     methods_collection = None
     methods_resource = None
-    methods = [
+    methods: t.ClassVar[t.Optional[t.Collection[str]]] = [
         HttpMethod.PATCH,
     ]
 
     @classmethod
     def register(
         cls,
         app,
```

### Comparing `Flaskel-3.0.3/flaskel/views/rpc.py` & `Flaskel-3.1.0rc2/flaskel/views/rpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     version: str = "2.0"
     separator: str = "."
     operations: OperationsType = {}
 
     default_view_name = "jsonrpc"
     default_urls = ("/jsonrpc",)
 
-    methods = [
+    methods: t.ClassVar[t.Optional[t.Collection[str]]] = [
         HttpMethod.POST,
     ]
     decorators = [
         builder.response("json"),
     ]
 
     def __init__(
```

### Comparing `Flaskel-3.0.3/flaskel/views/static.py` & `Flaskel-3.1.0rc2/flaskel/views/static.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.0.3/flaskel/views/template.py` & `Flaskel-3.1.0rc2/flaskel/views/template.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from flaskel.flaskel import Response
 
 from .base import BaseView
 
 
 class RenderTemplate(BaseView):
-    methods: t.List[str] = [
+    methods: t.ClassVar[t.Optional[t.Collection[str]]] = [
         HttpMethod.GET,
         HttpMethod.POST,
     ]
 
     template: str = "index.html"
 
     def __init__(
```

### Comparing `Flaskel-3.0.3/flaskel/views/token.py` & `Flaskel-3.1.0rc2/flaskel/views/token.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import typing as t
+
 import flask_jwt_extended
 from vbcore.datastruct import ObjectDict
 from vbcore.http import httpcode, HttpMethod
 
 from flaskel import abort, cap, request, webargs
 from flaskel.ext.auth import BaseTokenHandler
 from flaskel.ext.default import builder
@@ -10,15 +12,16 @@
 
 
 class BaseTokenAuth(BaseView):
     jwt = flask_jwt_extended
     handler: BaseTokenHandler = BaseTokenHandler()
 
     default_view_name = "token_auth"
-    methods = [
+
+    methods: t.ClassVar[t.Optional[t.Collection[str]]] = [
         HttpMethod.GET,
         HttpMethod.POST,
     ]
 
     """
         NOTE: endpoint should not be change otherwise dispatch_request MUST change
     """
```

### Comparing `Flaskel-3.0.3/flaskel/wsgi/base.py` & `Flaskel-3.1.0rc2/flaskel/wsgi/base.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.0.3/flaskel/wsgi/factory.py` & `Flaskel-3.1.0rc2/flaskel/wsgi/factory.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.0.3/flaskel/wsgi/wsgi_gevent.py` & `Flaskel-3.1.0rc2/flaskel/wsgi/wsgi_gevent.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.0.3/flaskel/wsgi/wsgi_gunicorn.py` & `Flaskel-3.1.0rc2/flaskel/wsgi/wsgi_gunicorn.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.0.3/flaskel/wsgi/wsgi_tornado.py` & `Flaskel-3.1.0rc2/flaskel/wsgi/wsgi_tornado.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.0.3/flaskel/wsgi/wsgi_twisted.py` & `Flaskel-3.1.0rc2/flaskel/wsgi/wsgi_twisted.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.0.3/setup.py` & `Flaskel-3.1.0rc2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,31 +41,30 @@
     "nest-asyncio",
     "vbcore[all]",
 ]
 REQUIRES_EXT = REQUIRES + [
     "pyfcm",
     "stripe",
     "redis",
-    "rejson",
     "hiredis",
     "Flask-Mail",
     "Flask-APScheduler",
     "flask_pymongo",
 ]
 REQUIRES_TEST = REQUIRES_EXT + [
     "coverage",
     "pytest",
     "pytest-cov",
 ]
 
-ENTRY_POINTS = dict(
-    console_scripts=[
+ENTRY_POINTS = {
+    "console_scripts": [
         f"{PKG_NAME}={PKG_SCRIPTS}.cli:cli",
     ]
-)
+}
 
 try:
     # must be after setuptools
     # noinspection PyPackageRequirements
     # noinspection PyPackageRequirements,PyPep8Naming
     import Cython.Compiler.Options as cython_options
     from Cython.Build import cythonize as base_cythonize
@@ -161,15 +160,15 @@
     author_email=grep(VERSION_FILE, "__author_email__"),
     zip_safe=False,
     include_package_data=True,
     packages=find_packages(),
     ext_modules=cythonize(ext_paths(PKG_NAME, skeleton_files())),
     test_suite=PKG_TEST,
     entry_points=ENTRY_POINTS,
-    cmdclass=dict(test=PyTest),
+    cmdclass={"test": PyTest},
     install_requires=REQUIRES,
     extras_require={
         "test": REQUIRES_TEST,
         "all": REQUIRES_EXT,
     },
     classifiers=[
         "Environment :: Web Environment",
```

