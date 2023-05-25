# Comparing `tmp/irails-1.3.25.tar.gz` & `tmp/irails-1.3.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irails-1.3.25.tar", last modified: Wed May 24 15:00:12 2023, max compression
+gzip compressed data, was "irails-1.3.26.tar", last modified: Wed May 24 15:41:38 2023, max compression
```

## Comparing `irails-1.3.25.tar` & `irails-1.3.26.tar`

### file list

```diff
@@ -1,104 +1,104 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 15:00:12.897792 irails-1.3.25/
--rw-rw-rw-   0        0        0       83 2023-05-04 04:10:30.000000 irails-1.3.25/MANIFEST.in
--rw-rw-rw-   0        0        0     4878 2023-05-24 15:00:12.896807 irails-1.3.25/PKG-INFO
--rw-rw-rw-   0        0        0     4096 2023-05-22 07:06:26.000000 irails-1.3.25/README.md
-drwxrwxrwx   0        0        0        0 2023-05-24 15:00:12.818476 irails-1.3.25/irails/
--rw-rw-rw-   0        0        0      307 2023-05-24 14:59:48.000000 irails-1.3.25/irails/__init__.py
--rw-rw-rw-   0        0        0     4887 2023-05-21 14:33:24.000000 irails-1.3.25/irails/_i18n.py
--rw-rw-rw-   0        0        0     2878 2023-05-21 08:27:23.000000 irails-1.3.25/irails/_loader.py
--rw-rw-rw-   0        0        0     5253 2023-05-20 14:13:50.000000 irails-1.3.25/irails/_utils.py
--rw-rw-rw-   0        0        0    12042 2023-05-20 06:44:17.000000 irails-1.3.25/irails/auth.py
--rw-rw-rw-   0        0        0    12705 2023-05-18 07:46:03.000000 irails-1.3.25/irails/base_controller.py
-drwxrwxrwx   0        0        0        0 2023-05-24 15:00:12.826454 irails-1.3.25/irails/casbin_adapters/
-drwxrwxrwx   0        0        0        0 2023-05-24 15:00:12.827452 irails-1.3.25/irails/casbin_adapters/__pycache__/
--rw-rw-rw-   0        0        0    17834 2023-04-30 14:29:09.000000 irails-1.3.25/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc
--rw-rw-rw-   0        0        0    10589 2023-05-13 05:03:07.000000 irails-1.3.25/irails/casbin_adapters/sqlalchemy_adapter.py
--rw-rw-rw-   0        0        0     4381 2023-02-25 09:43:32.000000 irails-1.3.25/irails/cbv.py
--rw-rw-rw-   0        0        0     6174 2023-05-19 07:06:13.000000 irails-1.3.25/irails/config.py
--rw-rw-rw-   0        0        0    12478 2023-05-12 05:56:24.000000 irails-1.3.25/irails/controller_utils.py
--rw-rw-rw-   0        0        0    24918 2023-05-19 11:59:51.000000 irails-1.3.25/irails/core.py
--rw-rw-rw-   0        0        0    20051 2023-05-24 14:56:19.000000 irails-1.3.25/irails/database.py
--rw-rw-rw-   0        0        0     1459 2023-05-11 15:27:11.000000 irails-1.3.25/irails/log.py
--rw-rw-rw-   0        0        0     8736 2023-05-21 14:38:31.000000 irails-1.3.25/irails/midware.py
--rw-rw-rw-   0        0        0     2141 2023-04-03 14:30:15.000000 irails-1.3.25/irails/midware_casbin.py
--rw-rw-rw-   0        0        0     9103 2023-05-16 08:16:43.000000 irails-1.3.25/irails/midware_session.py
--rw-rw-rw-   0        0        0     4208 2023-05-16 08:12:27.000000 irails-1.3.25/irails/mvc_router.py
-drwxrwxrwx   0        0        0        0 2023-05-24 15:00:12.839419 irails-1.3.25/irails/scripts/
--rw-rw-rw-   0        0        0        0 2023-04-26 07:44:41.000000 irails-1.3.25/irails/scripts/__init__.py
--rw-rw-rw-   0        0        0     7862 2023-05-13 15:04:27.000000 irails-1.3.25/irails/scripts/_app.py
--rw-rw-rw-   0        0        0     6892 2023-05-19 07:21:20.000000 irails-1.3.25/irails/scripts/_controller.py
--rw-rw-rw-   0        0        0     7763 2023-05-21 13:57:03.000000 irails-1.3.25/irails/scripts/_i18n.py
--rw-rw-rw-   0        0        0     1332 2023-05-21 08:39:33.000000 irails-1.3.25/irails/scripts/_migrate.py
--rw-rw-rw-   0        0        0     3774 2023-05-14 13:34:33.000000 irails-1.3.25/irails/scripts/_model.py
--rw-rw-rw-   0        0        0     2301 2023-05-03 14:35:33.000000 irails-1.3.25/irails/scripts/_project.py
--rw-rw-rw-   0        0        0     1600 2023-05-11 15:45:21.000000 irails-1.3.25/irails/scripts/_run.py
--rw-rw-rw-   0        0        0     2288 2023-05-11 14:15:32.000000 irails-1.3.25/irails/scripts/_shell.py
--rw-rw-rw-   0        0        0     4930 2023-05-21 14:27:15.000000 irails-1.3.25/irails/scripts/_test.py
--rw-rw-rw-   0        0        0     2900 2023-05-21 08:16:21.000000 irails-1.3.25/irails/scripts/main.py
-drwxrwxrwx   0        0        0        0 2023-05-24 15:00:12.786318 irails-1.3.25/irails/scripts/tpls/
-drwxrwxrwx   0        0        0        0 2023-05-24 15:00:12.849403 irails-1.3.25/irails/scripts/tpls/app/
--rw-rw-rw-   0        0        0      223 2023-05-09 15:18:47.000000 irails-1.3.25/irails/scripts/tpls/app/controller.tpl
--rw-rw-rw-   0        0        0        0 2023-04-28 06:03:05.000000 irails-1.3.25/irails/scripts/tpls/app/css.tpl
--rw-rw-rw-   0        0        0      791 2023-04-25 10:42:10.000000 irails-1.3.25/irails/scripts/tpls/app/home.css.tpl
--rw-rw-rw-   0        0        0     1293 2023-05-05 10:16:42.000000 irails-1.3.25/irails/scripts/tpls/app/home.tpl
--rw-rw-rw-   0        0        0     1023 2023-05-19 12:27:03.000000 irails-1.3.25/irails/scripts/tpls/app/model.jinja
--rw-rw-rw-   0        0        0      197 2023-05-24 11:06:24.000000 irails-1.3.25/irails/scripts/tpls/app/service.jinja
--rw-rw-rw-   0        0        0      237 2023-05-13 13:54:20.000000 irails-1.3.25/irails/scripts/tpls/app/test_controller.jinja
--rw-rw-rw-   0        0        0      908 2023-05-24 14:14:47.000000 irails-1.3.25/irails/scripts/tpls/app/test_service.jinja
--rw-rw-rw-   0        0        0       18 2023-05-02 08:56:04.000000 irails-1.3.25/irails/scripts/tpls/app/view.tpl
-drwxrwxrwx   0        0        0        0 2023-05-24 15:00:12.852385 irails-1.3.25/irails/scripts/tpls/project/
--rw-rw-rw-   0        0        0      139 2023-04-23 09:46:24.000000 irails-1.3.25/irails/scripts/tpls/project/.gitignore
-drwxrwxrwx   0        0        0        0 2023-05-24 15:00:12.853383 irails-1.3.25/irails/scripts/tpls/project/apps/
--rw-rw-rw-   0        0        0        0 2023-04-26 09:58:51.000000 irails-1.3.25/irails/scripts/tpls/project/apps/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-24 15:00:12.862359 irails-1.3.25/irails/scripts/tpls/project/configs/
--rw-rw-rw-   0        0        0      746 2023-05-09 06:45:34.000000 irails-1.3.25/irails/scripts/tpls/project/configs/alembic.ini
--rw-rw-rw-   0        0        0      179 2023-05-13 09:22:15.000000 irails-1.3.25/irails/scripts/tpls/project/configs/authencation.yaml
--rw-rw-rw-   0        0        0        0 2023-03-06 08:27:07.000000 irails-1.3.25/irails/scripts/tpls/project/configs/cache.yaml
--rw-rw-rw-   0        0        0      104 2023-05-04 05:06:32.000000 irails-1.3.25/irails/scripts/tpls/project/configs/casbin-adapter.csv
--rw-rw-rw-   0        0        0      302 2023-05-04 05:24:51.000000 irails-1.3.25/irails/scripts/tpls/project/configs/casbin-model.conf
-drwxrwxrwx   0        0        0        0 2023-05-24 15:00:12.875323 irails-1.3.25/irails/scripts/tpls/project/configs/casbin_templates/
--rw-rw-rw-   0        0        0      204 2023-05-18 07:46:03.000000 irails-1.3.25/irails/scripts/tpls/project/configs/casbin_templates/ALC.conf
--rw-rw-rw-   0        0        0       37 2023-05-18 07:46:03.000000 irails-1.3.25/irails/scripts/tpls/project/configs/casbin_templates/ALC.csv
--rw-rw-rw-   0        0        0      236 2023-05-18 07:46:03.000000 irails-1.3.25/irails/scripts/tpls/project/configs/casbin_templates/RBAC.conf
--rw-rw-rw-   0        0        0      125 2023-05-18 07:46:03.000000 irails-1.3.25/irails/scripts/tpls/project/configs/casbin_templates/RBAC.csv
--rw-rw-rw-   0        0        0      249 2023-05-18 07:46:03.000000 irails-1.3.25/irails/scripts/tpls/project/configs/casbin_templates/RBACR.conf
--rw-rw-rw-   0        0        0      159 2023-05-18 07:46:03.000000 irails-1.3.25/irails/scripts/tpls/project/configs/casbin_templates/RBACR.csv
--rw-rw-rw-   0        0        0      274 2023-05-18 07:46:03.000000 irails-1.3.25/irails/scripts/tpls/project/configs/casbin_templates/RBACT.conf
--rw-rw-rw-   0        0        0      178 2023-05-18 07:46:03.000000 irails-1.3.25/irails/scripts/tpls/project/configs/casbin_templates/RBACT.csv
--rw-rw-rw-   0        0        0      222 2023-05-18 07:46:03.000000 irails-1.3.25/irails/scripts/tpls/project/configs/casbin_templates/RESTFUL.conf
--rw-rw-rw-   0        0        0      152 2023-05-18 07:46:03.000000 irails-1.3.25/irails/scripts/tpls/project/configs/casbin_templates/RESTFUL.csv
--rw-rw-rw-   0        0        0      817 2023-05-10 10:45:36.000000 irails-1.3.25/irails/scripts/tpls/project/configs/database.yaml
--rw-rw-rw-   0        0        0      748 2023-05-11 05:35:06.000000 irails-1.3.25/irails/scripts/tpls/project/configs/general.yaml
--rw-rw-rw-   0        0        0      337 2023-04-22 10:54:12.000000 irails-1.3.25/irails/scripts/tpls/project/configs/session.yaml
--rw-rw-rw-   0        0        0      272 2023-05-09 06:44:59.000000 irails-1.3.25/irails/scripts/tpls/project/configs/upload.yaml
-drwxrwxrwx   0        0        0        0 2023-05-24 15:00:12.789309 irails-1.3.25/irails/scripts/tpls/project/data/
-drwxrwxrwx   0        0        0        0 2023-05-24 15:00:12.879312 irails-1.3.25/irails/scripts/tpls/project/data/alembic/
--rw-rw-rw-   0        0        0       38 2023-04-09 12:01:20.000000 irails-1.3.25/irails/scripts/tpls/project/data/alembic/README
--rw-rw-rw-   0        0        0     2144 2023-04-30 09:03:04.000000 irails-1.3.25/irails/scripts/tpls/project/data/alembic/env.py
--rw-rw-rw-   0        0        0      510 2023-04-09 12:01:20.000000 irails-1.3.25/irails/scripts/tpls/project/data/alembic/script.py.mako
--rw-rw-rw-   0        0        0      231 2023-05-11 15:42:13.000000 irails-1.3.25/irails/scripts/tpls/project/main.py
-drwxrwxrwx   0        0        0        0 2023-05-24 15:00:12.883323 irails-1.3.25/irails/scripts/tpls/project/public/
--rw-rw-rw-   0        0        0     1233 2023-05-02 08:46:22.000000 irails-1.3.25/irails/scripts/tpls/project/public/error_404.html
--rw-rw-rw-   0        0        0     1083 2023-05-02 08:46:46.000000 irails-1.3.25/irails/scripts/tpls/project/public/error_500.html
-drwxrwxrwx   0        0        0        0 2023-05-24 15:00:12.886818 irails-1.3.25/irails/scripts/tpls/project/public/libs/
-drwxrwxrwx   0        0        0        0 2023-05-24 15:00:12.792149 irails-1.3.25/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/
-drwxrwxrwx   0        0        0        0 2023-05-24 15:00:12.888815 irails-1.3.25/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/
--rw-rw-rw-   0        0        0  1970121 2023-04-23 08:02:36.000000 irails-1.3.25/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js
-drwxrwxrwx   0        0        0        0 2023-05-24 15:00:12.892804 irails-1.3.25/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/
--rw-rw-rw-   0        0        0   323666 2023-04-23 08:04:13.000000 irails-1.3.25/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css
--rw-rw-rw-   0        0        0      725 2023-04-21 12:39:53.000000 irails-1.3.25/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js
--rw-rw-rw-   0        0        0  1441055 2023-04-21 07:36:37.000000 irails-1.3.25/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js
-drwxrwxrwx   0        0        0        0 2023-05-24 15:00:12.793147 irails-1.3.25/irails/scripts/tpls/project/public/vue@3.2.36/
-drwxrwxrwx   0        0        0        0 2023-05-24 15:00:12.893802 irails-1.3.25/irails/scripts/tpls/project/public/vue@3.2.36/dist/
--rw-rw-rw-   0        0        0   640610 2023-04-21 07:36:07.000000 irails-1.3.25/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js
--rw-rw-rw-   0        0        0     1585 2023-05-24 07:01:16.000000 irails-1.3.25/irails/unit_test.py
--rw-rw-rw-   0        0        0     3034 2023-05-16 08:15:25.000000 irails-1.3.25/irails/view.py
-drwxrwxrwx   0        0        0        0 2023-05-24 15:00:12.824459 irails-1.3.25/irails.egg-info/
--rw-rw-rw-   0        0        0     4878 2023-05-24 15:00:12.000000 irails-1.3.25/irails.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3115 2023-05-24 15:00:12.000000 irails-1.3.25/irails.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 15:00:12.000000 irails-1.3.25/irails.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-05-24 15:00:12.000000 irails-1.3.25/irails.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      367 2023-05-24 15:00:12.000000 irails-1.3.25/irails.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-24 15:00:12.000000 irails-1.3.25/irails.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-24 15:00:12.897792 irails-1.3.25/setup.cfg
--rw-rw-rw-   0        0        0     2551 2023-05-09 11:27:27.000000 irails-1.3.25/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-24 15:41:38.246890 irails-1.3.26/
+-rw-rw-rw-   0        0        0       83 2023-05-04 04:10:30.000000 irails-1.3.26/MANIFEST.in
+-rw-rw-rw-   0        0        0     4878 2023-05-24 15:41:38.245893 irails-1.3.26/PKG-INFO
+-rw-rw-rw-   0        0        0     4096 2023-05-22 07:06:26.000000 irails-1.3.26/README.md
+drwxrwxrwx   0        0        0        0 2023-05-24 15:41:38.168095 irails-1.3.26/irails/
+-rw-rw-rw-   0        0        0      307 2023-05-24 15:41:25.000000 irails-1.3.26/irails/__init__.py
+-rw-rw-rw-   0        0        0     4887 2023-05-21 14:33:24.000000 irails-1.3.26/irails/_i18n.py
+-rw-rw-rw-   0        0        0     2878 2023-05-21 08:27:23.000000 irails-1.3.26/irails/_loader.py
+-rw-rw-rw-   0        0        0     5253 2023-05-20 14:13:50.000000 irails-1.3.26/irails/_utils.py
+-rw-rw-rw-   0        0        0    12042 2023-05-20 06:44:17.000000 irails-1.3.26/irails/auth.py
+-rw-rw-rw-   0        0        0    12705 2023-05-18 07:46:03.000000 irails-1.3.26/irails/base_controller.py
+drwxrwxrwx   0        0        0        0 2023-05-24 15:41:38.178072 irails-1.3.26/irails/casbin_adapters/
+drwxrwxrwx   0        0        0        0 2023-05-24 15:41:38.179072 irails-1.3.26/irails/casbin_adapters/__pycache__/
+-rw-rw-rw-   0        0        0    17834 2023-04-30 14:29:09.000000 irails-1.3.26/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc
+-rw-rw-rw-   0        0        0    10589 2023-05-13 05:03:07.000000 irails-1.3.26/irails/casbin_adapters/sqlalchemy_adapter.py
+-rw-rw-rw-   0        0        0     4381 2023-02-25 09:43:32.000000 irails-1.3.26/irails/cbv.py
+-rw-rw-rw-   0        0        0     6174 2023-05-19 07:06:13.000000 irails-1.3.26/irails/config.py
+-rw-rw-rw-   0        0        0    12478 2023-05-12 05:56:24.000000 irails-1.3.26/irails/controller_utils.py
+-rw-rw-rw-   0        0        0    24918 2023-05-19 11:59:51.000000 irails-1.3.26/irails/core.py
+-rw-rw-rw-   0        0        0    20117 2023-05-24 15:40:12.000000 irails-1.3.26/irails/database.py
+-rw-rw-rw-   0        0        0     1459 2023-05-11 15:27:11.000000 irails-1.3.26/irails/log.py
+-rw-rw-rw-   0        0        0     8736 2023-05-21 14:38:31.000000 irails-1.3.26/irails/midware.py
+-rw-rw-rw-   0        0        0     2141 2023-04-03 14:30:15.000000 irails-1.3.26/irails/midware_casbin.py
+-rw-rw-rw-   0        0        0     9103 2023-05-16 08:16:43.000000 irails-1.3.26/irails/midware_session.py
+-rw-rw-rw-   0        0        0     4208 2023-05-16 08:12:27.000000 irails-1.3.26/irails/mvc_router.py
+drwxrwxrwx   0        0        0        0 2023-05-24 15:41:38.191040 irails-1.3.26/irails/scripts/
+-rw-rw-rw-   0        0        0        0 2023-04-26 07:44:41.000000 irails-1.3.26/irails/scripts/__init__.py
+-rw-rw-rw-   0        0        0     7862 2023-05-13 15:04:27.000000 irails-1.3.26/irails/scripts/_app.py
+-rw-rw-rw-   0        0        0     6892 2023-05-19 07:21:20.000000 irails-1.3.26/irails/scripts/_controller.py
+-rw-rw-rw-   0        0        0     7763 2023-05-21 13:57:03.000000 irails-1.3.26/irails/scripts/_i18n.py
+-rw-rw-rw-   0        0        0     1332 2023-05-21 08:39:33.000000 irails-1.3.26/irails/scripts/_migrate.py
+-rw-rw-rw-   0        0        0     3774 2023-05-14 13:34:33.000000 irails-1.3.26/irails/scripts/_model.py
+-rw-rw-rw-   0        0        0     2301 2023-05-03 14:35:33.000000 irails-1.3.26/irails/scripts/_project.py
+-rw-rw-rw-   0        0        0     1600 2023-05-11 15:45:21.000000 irails-1.3.26/irails/scripts/_run.py
+-rw-rw-rw-   0        0        0     2288 2023-05-11 14:15:32.000000 irails-1.3.26/irails/scripts/_shell.py
+-rw-rw-rw-   0        0        0     4930 2023-05-21 14:27:15.000000 irails-1.3.26/irails/scripts/_test.py
+-rw-rw-rw-   0        0        0     2900 2023-05-21 08:16:21.000000 irails-1.3.26/irails/scripts/main.py
+drwxrwxrwx   0        0        0        0 2023-05-24 15:41:38.139606 irails-1.3.26/irails/scripts/tpls/
+drwxrwxrwx   0        0        0        0 2023-05-24 15:41:38.200016 irails-1.3.26/irails/scripts/tpls/app/
+-rw-rw-rw-   0        0        0      223 2023-05-09 15:18:47.000000 irails-1.3.26/irails/scripts/tpls/app/controller.tpl
+-rw-rw-rw-   0        0        0        0 2023-04-28 06:03:05.000000 irails-1.3.26/irails/scripts/tpls/app/css.tpl
+-rw-rw-rw-   0        0        0      791 2023-04-25 10:42:10.000000 irails-1.3.26/irails/scripts/tpls/app/home.css.tpl
+-rw-rw-rw-   0        0        0     1293 2023-05-05 10:16:42.000000 irails-1.3.26/irails/scripts/tpls/app/home.tpl
+-rw-rw-rw-   0        0        0     1023 2023-05-19 12:27:03.000000 irails-1.3.26/irails/scripts/tpls/app/model.jinja
+-rw-rw-rw-   0        0        0      197 2023-05-24 11:06:24.000000 irails-1.3.26/irails/scripts/tpls/app/service.jinja
+-rw-rw-rw-   0        0        0      237 2023-05-13 13:54:20.000000 irails-1.3.26/irails/scripts/tpls/app/test_controller.jinja
+-rw-rw-rw-   0        0        0      908 2023-05-24 14:14:47.000000 irails-1.3.26/irails/scripts/tpls/app/test_service.jinja
+-rw-rw-rw-   0        0        0       18 2023-05-02 08:56:04.000000 irails-1.3.26/irails/scripts/tpls/app/view.tpl
+drwxrwxrwx   0        0        0        0 2023-05-24 15:41:38.203014 irails-1.3.26/irails/scripts/tpls/project/
+-rw-rw-rw-   0        0        0      139 2023-04-23 09:46:24.000000 irails-1.3.26/irails/scripts/tpls/project/.gitignore
+drwxrwxrwx   0        0        0        0 2023-05-24 15:41:38.205005 irails-1.3.26/irails/scripts/tpls/project/apps/
+-rw-rw-rw-   0        0        0        0 2023-04-26 09:58:51.000000 irails-1.3.26/irails/scripts/tpls/project/apps/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-24 15:41:38.214976 irails-1.3.26/irails/scripts/tpls/project/configs/
+-rw-rw-rw-   0        0        0      746 2023-05-09 06:45:34.000000 irails-1.3.26/irails/scripts/tpls/project/configs/alembic.ini
+-rw-rw-rw-   0        0        0      179 2023-05-13 09:22:15.000000 irails-1.3.26/irails/scripts/tpls/project/configs/authencation.yaml
+-rw-rw-rw-   0        0        0        0 2023-03-06 08:27:07.000000 irails-1.3.26/irails/scripts/tpls/project/configs/cache.yaml
+-rw-rw-rw-   0        0        0      104 2023-05-04 05:06:32.000000 irails-1.3.26/irails/scripts/tpls/project/configs/casbin-adapter.csv
+-rw-rw-rw-   0        0        0      302 2023-05-04 05:24:51.000000 irails-1.3.26/irails/scripts/tpls/project/configs/casbin-model.conf
+drwxrwxrwx   0        0        0        0 2023-05-24 15:41:38.226944 irails-1.3.26/irails/scripts/tpls/project/configs/casbin_templates/
+-rw-rw-rw-   0        0        0      204 2023-05-18 07:46:03.000000 irails-1.3.26/irails/scripts/tpls/project/configs/casbin_templates/ALC.conf
+-rw-rw-rw-   0        0        0       37 2023-05-18 07:46:03.000000 irails-1.3.26/irails/scripts/tpls/project/configs/casbin_templates/ALC.csv
+-rw-rw-rw-   0        0        0      236 2023-05-18 07:46:03.000000 irails-1.3.26/irails/scripts/tpls/project/configs/casbin_templates/RBAC.conf
+-rw-rw-rw-   0        0        0      125 2023-05-18 07:46:03.000000 irails-1.3.26/irails/scripts/tpls/project/configs/casbin_templates/RBAC.csv
+-rw-rw-rw-   0        0        0      249 2023-05-18 07:46:03.000000 irails-1.3.26/irails/scripts/tpls/project/configs/casbin_templates/RBACR.conf
+-rw-rw-rw-   0        0        0      159 2023-05-18 07:46:03.000000 irails-1.3.26/irails/scripts/tpls/project/configs/casbin_templates/RBACR.csv
+-rw-rw-rw-   0        0        0      274 2023-05-18 07:46:03.000000 irails-1.3.26/irails/scripts/tpls/project/configs/casbin_templates/RBACT.conf
+-rw-rw-rw-   0        0        0      178 2023-05-18 07:46:03.000000 irails-1.3.26/irails/scripts/tpls/project/configs/casbin_templates/RBACT.csv
+-rw-rw-rw-   0        0        0      222 2023-05-18 07:46:03.000000 irails-1.3.26/irails/scripts/tpls/project/configs/casbin_templates/RESTFUL.conf
+-rw-rw-rw-   0        0        0      152 2023-05-18 07:46:03.000000 irails-1.3.26/irails/scripts/tpls/project/configs/casbin_templates/RESTFUL.csv
+-rw-rw-rw-   0        0        0      817 2023-05-10 10:45:36.000000 irails-1.3.26/irails/scripts/tpls/project/configs/database.yaml
+-rw-rw-rw-   0        0        0      748 2023-05-11 05:35:06.000000 irails-1.3.26/irails/scripts/tpls/project/configs/general.yaml
+-rw-rw-rw-   0        0        0      337 2023-04-22 10:54:12.000000 irails-1.3.26/irails/scripts/tpls/project/configs/session.yaml
+-rw-rw-rw-   0        0        0      272 2023-05-09 06:44:59.000000 irails-1.3.26/irails/scripts/tpls/project/configs/upload.yaml
+drwxrwxrwx   0        0        0        0 2023-05-24 15:41:38.143162 irails-1.3.26/irails/scripts/tpls/project/data/
+drwxrwxrwx   0        0        0        0 2023-05-24 15:41:38.229936 irails-1.3.26/irails/scripts/tpls/project/data/alembic/
+-rw-rw-rw-   0        0        0       38 2023-04-09 12:01:20.000000 irails-1.3.26/irails/scripts/tpls/project/data/alembic/README
+-rw-rw-rw-   0        0        0     2144 2023-04-30 09:03:04.000000 irails-1.3.26/irails/scripts/tpls/project/data/alembic/env.py
+-rw-rw-rw-   0        0        0      510 2023-04-09 12:01:20.000000 irails-1.3.26/irails/scripts/tpls/project/data/alembic/script.py.mako
+-rw-rw-rw-   0        0        0      231 2023-05-11 15:42:13.000000 irails-1.3.26/irails/scripts/tpls/project/main.py
+drwxrwxrwx   0        0        0        0 2023-05-24 15:41:38.231932 irails-1.3.26/irails/scripts/tpls/project/public/
+-rw-rw-rw-   0        0        0     1233 2023-05-02 08:46:22.000000 irails-1.3.26/irails/scripts/tpls/project/public/error_404.html
+-rw-rw-rw-   0        0        0     1083 2023-05-02 08:46:46.000000 irails-1.3.26/irails/scripts/tpls/project/public/error_500.html
+drwxrwxrwx   0        0        0        0 2023-05-24 15:41:38.233926 irails-1.3.26/irails/scripts/tpls/project/public/libs/
+drwxrwxrwx   0        0        0        0 2023-05-24 15:41:38.146155 irails-1.3.26/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/
+drwxrwxrwx   0        0        0        0 2023-05-24 15:41:38.238931 irails-1.3.26/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/
+-rw-rw-rw-   0        0        0  1970121 2023-04-23 08:02:36.000000 irails-1.3.26/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js
+drwxrwxrwx   0        0        0        0 2023-05-24 15:41:38.242901 irails-1.3.26/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/
+-rw-rw-rw-   0        0        0   323666 2023-04-23 08:04:13.000000 irails-1.3.26/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css
+-rw-rw-rw-   0        0        0      725 2023-04-21 12:39:53.000000 irails-1.3.26/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js
+-rw-rw-rw-   0        0        0  1441055 2023-04-21 07:36:37.000000 irails-1.3.26/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js
+drwxrwxrwx   0        0        0        0 2023-05-24 15:41:38.147152 irails-1.3.26/irails/scripts/tpls/project/public/vue@3.2.36/
+drwxrwxrwx   0        0        0        0 2023-05-24 15:41:38.244896 irails-1.3.26/irails/scripts/tpls/project/public/vue@3.2.36/dist/
+-rw-rw-rw-   0        0        0   640610 2023-04-21 07:36:07.000000 irails-1.3.26/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js
+-rw-rw-rw-   0        0        0     1585 2023-05-24 07:01:16.000000 irails-1.3.26/irails/unit_test.py
+-rw-rw-rw-   0        0        0     3034 2023-05-16 08:15:25.000000 irails-1.3.26/irails/view.py
+drwxrwxrwx   0        0        0        0 2023-05-24 15:41:38.175077 irails-1.3.26/irails.egg-info/
+-rw-rw-rw-   0        0        0     4878 2023-05-24 15:41:37.000000 irails-1.3.26/irails.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3115 2023-05-24 15:41:37.000000 irails-1.3.26/irails.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 15:41:37.000000 irails-1.3.26/irails.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-05-24 15:41:37.000000 irails-1.3.26/irails.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      367 2023-05-24 15:41:37.000000 irails-1.3.26/irails.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-24 15:41:37.000000 irails-1.3.26/irails.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-24 15:41:38.246890 irails-1.3.26/setup.cfg
+-rw-rw-rw-   0        0        0     2551 2023-05-09 11:27:27.000000 irails-1.3.26/setup.py
```

### Comparing `irails-1.3.25/PKG-INFO` & `irails-1.3.26/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irails
-Version: 1.3.25
+Version: 1.3.26
 Summary: Simple and elegant use of FastApi in MVC mode
 Home-page: https://github.com/smjkzsl/irails
 Author: Bruce chou
 Author-email: smjkzsl@gmail.com
 License: Apache License 2.0
 Keywords: web framework,mvc framework,fastapi framework
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `irails-1.3.25/README.md` & `irails-1.3.26/README.md`

 * *Files identical despite different names*

### Comparing `irails-1.3.25/irails/_i18n.py` & `irails-1.3.26/irails/_i18n.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.25/irails/_loader.py` & `irails-1.3.26/irails/_loader.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.25/irails/_utils.py` & `irails-1.3.26/irails/_utils.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.25/irails/auth.py` & `irails-1.3.26/irails/auth.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.25/irails/base_controller.py` & `irails-1.3.26/irails/base_controller.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.25/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc` & `irails-1.3.26/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `irails-1.3.25/irails/casbin_adapters/sqlalchemy_adapter.py` & `irails-1.3.26/irails/casbin_adapters/sqlalchemy_adapter.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.25/irails/cbv.py` & `irails-1.3.26/irails/cbv.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.25/irails/config.py` & `irails-1.3.26/irails/config.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.25/irails/controller_utils.py` & `irails-1.3.26/irails/controller_utils.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.25/irails/core.py` & `irails-1.3.26/irails/core.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.25/irails/database.py` & `irails-1.3.26/irails/database.py`

 * *Files 2% similar despite different names*

```diff
@@ -176,27 +176,31 @@
 class ListPager:
     def __init__(self,query:Query,size:int=None ) -> None: 
         self.query = query
         if size:
             self.page_size = size
         else:
             self.page_size = page_size 
-         
+    def order(self,*args):
+        query = self.query.order_by(*args)     
+        return ListPager(query=query,size=self.page_size)
+    
     def count_all(self)->int:
         return self.query.count()
     
     def page_count(self)->int:
         import math
         return math.ceil(self.count_all()/self.page_size)
     
     def page(self,page_num=1)->Query:
         return self.query.limit(self.page_size).offset(self.page_size*(page_num-1))
     
-    def get_rows(self,page_num=1)->List[Base]:
+    def get(self,page_num=1)->List[Base]:
         return self.query.limit(self.page_size).offset(self.page_size*(page_num-1)).all()
+    
 class Service(metaclass=_serviceMeta):
     __all_generated = {}
     _session:Session = None
     _ = _ #the i18n traslation object ,it's will auto redirect the `app_name/locales` dir i18n configure
     @contextmanager      
     @staticmethod 
     def get_session():
@@ -234,38 +238,54 @@
             q = session.query(model).filter_by(**kwargs).one()
         except sqlalchemy.exc.NoResultFound as e: 
             return False
         except sqlalchemy.orm.exc.MultipleResultsFound:
             return True
         return not q  is None
     @classmethod
-    def query(self,model:Base,*args,**kwargs)->Query:
-        '''Get a query object with auto passed is_deleted rows'''
-        session = self.session()
+    def __check_is_deleted_param(self,model:Base,**kwargs):
         if hasattr(model,is_deleted_field):
             if not kwargs:kwargs = {}
             if not is_deleted_field in kwargs:
                 kwargs[is_deleted_field] = False
+            else:
+                if kwargs[is_deleted_field]=='all':
+                    del kwargs[is_deleted_field]
+        return kwargs
+    @classmethod
+    def query(self,model:Base,*args,**kwargs)->Query:
+        '''Get a query object with auto passed is_deleted rows'''
+        session = self.session()
+        kwargs = self.__check_is_deleted_param(model,**kwargs)
         query = session.query(model).filter(*args).filter_by(**kwargs)
         return query
     
     @classmethod
     def select(self,model:Base,*where,**kwargs)->List[Base]:
         ''' Auto pass if row has is_deleted field
             execute select statement with :where condition on :model
             :return rows of result
         '''
-        if hasattr(model,is_deleted_field):
-            if not kwargs:kwargs = {}
-            if not is_deleted_field in kwargs:
-                kwargs[is_deleted_field] = False
+        kwargs = self.__check_is_deleted_param(model,**kwargs)
         stmt = select(model).where(*where).filter_by(**kwargs)
         with engine.begin() as conn:
             ret = conn.execute(stmt)
-            return ret.fetchall()     
+            return ret.fetchall()    
+    @classmethod
+    def list(self,model:Base,*args, **kwargs)->List[Base]:
+        '''Auto pass is_deleted if model has is_deleted field'''
+        kwargs = self.__check_is_deleted_param(model,**kwargs)
+        session = self.session()  
+        query = session.query(model) 
+        if args:
+            query = query.filter(*args)
+        if kwargs:
+            query = query.filter_by(**kwargs) 
+        return query.all()
+     
     @classmethod
     def update(self,model:Base,*where,**values)->int:
         '''
             execute update :model with :values on :model by :where
             :return rowcount
         '''
         q = self.query(model,*where) 
@@ -281,18 +301,15 @@
             raise e
         return cnt
     @classmethod
     def count(self,model:Base,*args,**kwargs)->int:
         ''' Auto pass if row has is_deleted field
             :return count by givened :args on :model
         '''
-        if hasattr(model,is_deleted_field):
-                if not kwargs:kwargs = {}
-                if not is_deleted_field in kwargs:
-                    kwargs[is_deleted_field] = False
+        kwargs = self.__check_is_deleted_param(model,**kwargs)
         
         if hasattr(model,'id'):
             
             q = self.query(func.count(model.id),*args,**kwargs)
             return q.scalar()
         else:
             return len(self.list( model,*args,**kwargs))
@@ -314,28 +331,15 @@
             session.merge(m,load=False)
             return m
         return None
     @classmethod
     def add_all(self,values:List['Base']):
         with self.get_session() as session: 
             session.add_all(values) 
-    @classmethod
-    def list(self,model:Base,*args, **kwargs)->List[Base]:
-        '''Auto pass is_deleted if model has is_deleted field'''
-        if hasattr(model,is_deleted_field):
-            if not kwargs:kwargs = {}
-            if not is_deleted_field in kwargs:
-                kwargs[is_deleted_field] = False
-        session = self.session()  
-        query = session.query(model) 
-        if args:
-            query = query.filter(*args)
-        if kwargs:
-            query = query.filter_by(**kwargs) 
-        return query.all()
+    
     
     
     @classmethod
     def delete(self,model:Base,*args,**kwargs)->int:  
         '''Soft delete if model has is_deleted field Else real delete'''
         with self.get_session() as session:
             query = session.query(model).filter(*args).filter_by(**kwargs)
```

### Comparing `irails-1.3.25/irails/log.py` & `irails-1.3.26/irails/log.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.25/irails/midware.py` & `irails-1.3.26/irails/midware.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.25/irails/midware_casbin.py` & `irails-1.3.26/irails/midware_casbin.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.25/irails/midware_session.py` & `irails-1.3.26/irails/midware_session.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.25/irails/mvc_router.py` & `irails-1.3.26/irails/mvc_router.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.25/irails/scripts/_app.py` & `irails-1.3.26/irails/scripts/_app.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.25/irails/scripts/_controller.py` & `irails-1.3.26/irails/scripts/_controller.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.25/irails/scripts/_i18n.py` & `irails-1.3.26/irails/scripts/_i18n.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.25/irails/scripts/_migrate.py` & `irails-1.3.26/irails/scripts/_migrate.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.25/irails/scripts/_model.py` & `irails-1.3.26/irails/scripts/_model.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.25/irails/scripts/_project.py` & `irails-1.3.26/irails/scripts/_project.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.25/irails/scripts/_run.py` & `irails-1.3.26/irails/scripts/_run.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.25/irails/scripts/_shell.py` & `irails-1.3.26/irails/scripts/_shell.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.25/irails/scripts/_test.py` & `irails-1.3.26/irails/scripts/_test.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.25/irails/scripts/main.py` & `irails-1.3.26/irails/scripts/main.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.25/irails/scripts/tpls/app/home.css.tpl` & `irails-1.3.26/irails/scripts/tpls/app/home.css.tpl`

 * *Files identical despite different names*

### Comparing `irails-1.3.25/irails/scripts/tpls/app/home.tpl` & `irails-1.3.26/irails/scripts/tpls/app/home.tpl`

 * *Files identical despite different names*

### Comparing `irails-1.3.25/irails/scripts/tpls/app/model.jinja` & `irails-1.3.26/irails/scripts/tpls/app/model.jinja`

 * *Files identical despite different names*

### Comparing `irails-1.3.25/irails/scripts/tpls/app/test_service.jinja` & `irails-1.3.26/irails/scripts/tpls/app/test_service.jinja`

 * *Files identical despite different names*

### Comparing `irails-1.3.25/irails/scripts/tpls/project/configs/alembic.ini` & `irails-1.3.26/irails/scripts/tpls/project/configs/alembic.ini`

 * *Files identical despite different names*

### Comparing `irails-1.3.25/irails/scripts/tpls/project/configs/database.yaml` & `irails-1.3.26/irails/scripts/tpls/project/configs/database.yaml`

 * *Files identical despite different names*

### Comparing `irails-1.3.25/irails/scripts/tpls/project/configs/general.yaml` & `irails-1.3.26/irails/scripts/tpls/project/configs/general.yaml`

 * *Files identical despite different names*

### Comparing `irails-1.3.25/irails/scripts/tpls/project/data/alembic/env.py` & `irails-1.3.26/irails/scripts/tpls/project/data/alembic/env.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.25/irails/scripts/tpls/project/public/error_404.html` & `irails-1.3.26/irails/scripts/tpls/project/public/error_404.html`

 * *Files identical despite different names*

### Comparing `irails-1.3.25/irails/scripts/tpls/project/public/error_500.html` & `irails-1.3.26/irails/scripts/tpls/project/public/error_500.html`

 * *Files identical despite different names*

### Comparing `irails-1.3.25/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js` & `irails-1.3.26/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js`

 * *Files identical despite different names*

### Comparing `irails-1.3.25/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css` & `irails-1.3.26/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css`

 * *Files identical despite different names*

### Comparing `irails-1.3.25/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js` & `irails-1.3.26/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js`

 * *Files identical despite different names*

### Comparing `irails-1.3.25/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js` & `irails-1.3.26/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js`

 * *Files identical despite different names*

### Comparing `irails-1.3.25/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js` & `irails-1.3.26/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js`

 * *Files identical despite different names*

### Comparing `irails-1.3.25/irails/unit_test.py` & `irails-1.3.26/irails/unit_test.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.25/irails/view.py` & `irails-1.3.26/irails/view.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.25/irails.egg-info/PKG-INFO` & `irails-1.3.26/irails.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irails
-Version: 1.3.25
+Version: 1.3.26
 Summary: Simple and elegant use of FastApi in MVC mode
 Home-page: https://github.com/smjkzsl/irails
 Author: Bruce chou
 Author-email: smjkzsl@gmail.com
 License: Apache License 2.0
 Keywords: web framework,mvc framework,fastapi framework
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `irails-1.3.25/irails.egg-info/SOURCES.txt` & `irails-1.3.26/irails.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `irails-1.3.25/setup.py` & `irails-1.3.26/setup.py`

 * *Files identical despite different names*

