# Comparing `tmp/duty-board-0.1.0.tar.gz` & `tmp/duty-board-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duty-board-0.1.0.tar", last modified: Mon Jan 23 08:47:07 2023, max compression
+gzip compressed data, was "duty-board-0.2.1.tar", last modified: Thu May 25 14:26:33 2023, max compression
```

## Comparing `duty-board-0.1.0.tar` & `duty-board-0.2.1.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 08:47:07.881435 duty-board-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-01-23 08:46:25.000000 duty-board-0.1.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-01-23 08:46:25.000000 duty-board-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-01-23 08:46:25.000000 duty-board-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    17349 2023-01-23 08:47:07.881435 duty-board-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-01-23 08:46:25.000000 duty-board-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 08:47:07.865435 duty-board-0.1.0/duty_board/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-01-23 08:46:25.000000 duty-board-0.1.0/duty_board/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 08:47:07.869434 duty-board-0.1.0/duty_board/alchemy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-23 08:46:25.000000 duty-board-0.1.0/duty_board/alchemy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6354 2023-01-23 08:46:25.000000 duty-board-0.1.0/duty_board/alchemy/add_sqladmin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6374 2023-01-23 08:46:25.000000 duty-board-0.1.0/duty_board/alchemy/queries.py
--rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-01-23 08:46:25.000000 duty-board-0.1.0/duty_board/alchemy/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-01-23 08:46:25.000000 duty-board-0.1.0/duty_board/alchemy/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-01-23 08:46:25.000000 duty-board-0.1.0/duty_board/alchemy/sqlalchemy_types.py
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-01-23 08:46:25.000000 duty-board-0.1.0/duty_board/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-01-23 08:46:25.000000 duty-board-0.1.0/duty_board/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 08:47:07.869434 duty-board-0.1.0/duty_board/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-23 08:46:25.000000 duty-board-0.1.0/duty_board/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-01-23 08:46:25.000000 duty-board-0.1.0/duty_board/models/calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-01-23 08:46:25.000000 duty-board-0.1.0/duty_board/models/generate_fake_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-01-23 08:46:25.000000 duty-board-0.1.0/duty_board/models/on_call_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-01-23 08:46:25.000000 duty-board-0.1.0/duty_board/models/person.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-01-23 08:46:25.000000 duty-board-0.1.0/duty_board/models/token.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 08:47:07.869434 duty-board-0.1.0/duty_board/plugin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-23 08:46:25.000000 duty-board-0.1.0/duty_board/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-01-23 08:46:25.000000 duty-board-0.1.0/duty_board/plugin/abstract_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 08:47:07.869434 duty-board-0.1.0/duty_board/plugin/example/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-23 08:46:25.000000 duty-board-0.1.0/duty_board/plugin/example/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36934 2023-01-23 08:46:25.000000 duty-board-0.1.0/duty_board/plugin/example/example_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-01-23 08:46:25.000000 duty-board-0.1.0/duty_board/plugin/example/example_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-01-23 08:46:25.000000 duty-board-0.1.0/duty_board/plugin/example/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 08:47:07.869434 duty-board-0.1.0/duty_board/plugin/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-23 08:46:25.000000 duty-board-0.1.0/duty_board/plugin/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-01-23 08:46:25.000000 duty-board-0.1.0/duty_board/plugin/helpers/duty_calendar_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-01-23 08:46:25.000000 duty-board-0.1.0/duty_board/plugin/helpers/plugin_fetcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     5084 2023-01-23 08:46:25.000000 duty-board-0.1.0/duty_board/plugin/ical_plugin_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     7409 2023-01-23 08:46:25.000000 duty-board-0.1.0/duty_board/plugin/ldap_plugin_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4676 2023-01-23 08:46:25.000000 duty-board-0.1.0/duty_board/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 08:47:07.869434 duty-board-0.1.0/duty_board/web_helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-23 08:46:25.000000 duty-board-0.1.0/duty_board/web_helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-01-23 08:46:25.000000 duty-board-0.1.0/duty_board/web_helpers/generate_typescript_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-01-23 08:46:25.000000 duty-board-0.1.0/duty_board/web_helpers/gzip_static_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-01-23 08:46:25.000000 duty-board-0.1.0/duty_board/web_helpers/response_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     6541 2023-01-23 08:46:25.000000 duty-board-0.1.0/duty_board/worker_loop.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 08:47:07.865435 duty-board-0.1.0/duty_board/www/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 08:47:07.877435 duty-board-0.1.0/duty_board/www/dist/
--rw-r--r--   0 runner    (1001) docker     (123)  1383284 2023-01-23 08:46:56.000000 duty-board-0.1.0/duty_board/www/dist/809.js
--rw-r--r--   0 runner    (1001) docker     (123)   434278 2023-01-23 08:46:56.000000 duty-board-0.1.0/duty_board/www/dist/809.js.gz
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-01-23 08:46:56.000000 duty-board-0.1.0/duty_board/www/dist/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-01-23 08:46:56.000000 duty-board-0.1.0/duty_board/www/dist/index.html.gz
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-01-23 08:46:56.000000 duty-board-0.1.0/duty_board/www/dist/main.0b8533bbfe9fae93806d.css
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-01-23 08:46:56.000000 duty-board-0.1.0/duty_board/www/dist/main.0b8533bbfe9fae93806d.css.gz
--rw-r--r--   0 runner    (1001) docker     (123)  2803865 2023-01-23 08:46:56.000000 duty-board-0.1.0/duty_board/www/dist/main.js
--rw-r--r--   0 runner    (1001) docker     (123)   780970 2023-01-23 08:46:56.000000 duty-board-0.1.0/duty_board/www/dist/main.js.gz
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-01-23 08:46:56.000000 duty-board-0.1.0/duty_board/www/dist/manifest.json
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-01-23 08:46:56.000000 duty-board-0.1.0/duty_board/www/dist/manifest.json.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 08:47:07.877435 duty-board-0.1.0/duty_board/www/static/
--rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-01-23 08:46:25.000000 duty-board-0.1.0/duty_board/www/static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     7614 2023-01-23 08:46:25.000000 duty-board-0.1.0/duty_board/www/static/logo192.png
--rw-r--r--   0 runner    (1001) docker     (123)    39164 2023-01-23 08:46:25.000000 duty-board-0.1.0/duty_board/www/static/logo512.png
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-01-23 08:46:25.000000 duty-board-0.1.0/duty_board/www/static/manifest.json
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-01-23 08:46:25.000000 duty-board-0.1.0/duty_board/www/static/robots.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 08:47:07.881435 duty-board-0.1.0/duty_board/www/user_images/
--rw-r--r--   0 runner    (1001) docker     (123)   680501 2023-01-23 08:46:25.000000 duty-board-0.1.0/duty_board/www/user_images/bert.jpeg
--rw-r--r--   0 runner    (1001) docker     (123)   317870 2023-01-23 08:46:25.000000 duty-board-0.1.0/duty_board/www/user_images/bert2.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 08:47:07.865435 duty-board-0.1.0/duty_board.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17349 2023-01-23 08:47:07.000000 duty-board-0.1.0/duty_board.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-01-23 08:47:07.000000 duty-board-0.1.0/duty_board.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-23 08:47:07.000000 duty-board-0.1.0/duty_board.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-01-23 08:47:07.000000 duty-board-0.1.0/duty_board.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-01-23 08:47:07.000000 duty-board-0.1.0/duty_board.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-01-23 08:47:07.000000 duty-board-0.1.0/duty_board.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-01-23 08:46:25.000000 duty-board-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-23 08:47:07.881435 duty-board-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:26:33.344520 duty-board-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-05-25 14:25:55.000000 duty-board-0.2.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-25 14:25:55.000000 duty-board-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-25 14:25:55.000000 duty-board-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    17349 2023-05-25 14:26:33.344520 duty-board-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-05-25 14:25:55.000000 duty-board-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:26:33.332520 duty-board-0.2.1/duty_board/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-25 14:25:55.000000 duty-board-0.2.1/duty_board/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:26:33.332520 duty-board-0.2.1/duty_board/alchemy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:25:55.000000 duty-board-0.2.1/duty_board/alchemy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6354 2023-05-25 14:25:55.000000 duty-board-0.2.1/duty_board/alchemy/add_sqladmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6377 2023-05-25 14:25:55.000000 duty-board-0.2.1/duty_board/alchemy/queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-05-25 14:25:55.000000 duty-board-0.2.1/duty_board/alchemy/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-05-25 14:25:55.000000 duty-board-0.2.1/duty_board/alchemy/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-05-25 14:25:55.000000 duty-board-0.2.1/duty_board/alchemy/sqlalchemy_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-25 14:25:55.000000 duty-board-0.2.1/duty_board/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-05-25 14:25:55.000000 duty-board-0.2.1/duty_board/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:26:33.332520 duty-board-0.2.1/duty_board/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:25:55.000000 duty-board-0.2.1/duty_board/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-05-25 14:25:55.000000 duty-board-0.2.1/duty_board/models/calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-05-25 14:25:55.000000 duty-board-0.2.1/duty_board/models/generate_fake_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-05-25 14:25:55.000000 duty-board-0.2.1/duty_board/models/on_call_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-05-25 14:25:55.000000 duty-board-0.2.1/duty_board/models/person.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-25 14:25:55.000000 duty-board-0.2.1/duty_board/models/token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:26:33.332520 duty-board-0.2.1/duty_board/plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:25:55.000000 duty-board-0.2.1/duty_board/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-05-25 14:25:55.000000 duty-board-0.2.1/duty_board/plugin/abstract_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:26:33.332520 duty-board-0.2.1/duty_board/plugin/example/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:25:55.000000 duty-board-0.2.1/duty_board/plugin/example/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36934 2023-05-25 14:25:55.000000 duty-board-0.2.1/duty_board/plugin/example/example_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-25 14:25:55.000000 duty-board-0.2.1/duty_board/plugin/example/example_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-05-25 14:25:55.000000 duty-board-0.2.1/duty_board/plugin/example/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:26:33.332520 duty-board-0.2.1/duty_board/plugin/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:25:55.000000 duty-board-0.2.1/duty_board/plugin/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-05-25 14:25:55.000000 duty-board-0.2.1/duty_board/plugin/helpers/duty_calendar_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-05-25 14:25:55.000000 duty-board-0.2.1/duty_board/plugin/helpers/plugin_fetcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5084 2023-05-25 14:25:55.000000 duty-board-0.2.1/duty_board/plugin/ical_plugin_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7409 2023-05-25 14:25:55.000000 duty-board-0.2.1/duty_board/plugin/ldap_plugin_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-05-25 14:25:55.000000 duty-board-0.2.1/duty_board/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:26:33.336520 duty-board-0.2.1/duty_board/web_helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:25:55.000000 duty-board-0.2.1/duty_board/web_helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-05-25 14:25:55.000000 duty-board-0.2.1/duty_board/web_helpers/generate_typescript_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-05-25 14:25:55.000000 duty-board-0.2.1/duty_board/web_helpers/gzip_static_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-05-25 14:25:55.000000 duty-board-0.2.1/duty_board/web_helpers/response_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6541 2023-05-25 14:25:55.000000 duty-board-0.2.1/duty_board/worker_loop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:26:33.328520 duty-board-0.2.1/duty_board/www/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:26:33.340520 duty-board-0.2.1/duty_board/www/dist/
+-rw-r--r--   0 runner    (1001) docker     (123)  1383284 2023-05-25 14:26:24.000000 duty-board-0.2.1/duty_board/www/dist/809.js
+-rw-r--r--   0 runner    (1001) docker     (123)   434278 2023-05-25 14:26:24.000000 duty-board-0.2.1/duty_board/www/dist/809.js.gz
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-25 14:26:24.000000 duty-board-0.2.1/duty_board/www/dist/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-25 14:26:24.000000 duty-board-0.2.1/duty_board/www/dist/index.html.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-05-25 14:26:24.000000 duty-board-0.2.1/duty_board/www/dist/main.e82352a304d245533b70.css
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-05-25 14:26:24.000000 duty-board-0.2.1/duty_board/www/dist/main.e82352a304d245533b70.css.gz
+-rw-r--r--   0 runner    (1001) docker     (123)  2807276 2023-05-25 14:26:24.000000 duty-board-0.2.1/duty_board/www/dist/main.js
+-rw-r--r--   0 runner    (1001) docker     (123)   781676 2023-05-25 14:26:24.000000 duty-board-0.2.1/duty_board/www/dist/main.js.gz
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-25 14:26:24.000000 duty-board-0.2.1/duty_board/www/dist/manifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-25 14:26:24.000000 duty-board-0.2.1/duty_board/www/dist/manifest.json.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:26:33.340520 duty-board-0.2.1/duty_board/www/static/
+-rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-05-25 14:25:55.000000 duty-board-0.2.1/duty_board/www/static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     7614 2023-05-25 14:25:55.000000 duty-board-0.2.1/duty_board/www/static/logo192.png
+-rw-r--r--   0 runner    (1001) docker     (123)    39164 2023-05-25 14:25:55.000000 duty-board-0.2.1/duty_board/www/static/logo512.png
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-25 14:25:55.000000 duty-board-0.2.1/duty_board/www/static/manifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-25 14:25:55.000000 duty-board-0.2.1/duty_board/www/static/robots.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:26:33.344520 duty-board-0.2.1/duty_board/www/user_images/
+-rw-r--r--   0 runner    (1001) docker     (123)   680501 2023-05-25 14:25:55.000000 duty-board-0.2.1/duty_board/www/user_images/bert.jpeg
+-rw-r--r--   0 runner    (1001) docker     (123)   317870 2023-05-25 14:25:55.000000 duty-board-0.2.1/duty_board/www/user_images/bert2.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:26:33.332520 duty-board-0.2.1/duty_board.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17349 2023-05-25 14:26:33.000000 duty-board-0.2.1/duty_board.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-05-25 14:26:33.000000 duty-board-0.2.1/duty_board.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 14:26:33.000000 duty-board-0.2.1/duty_board.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-25 14:26:33.000000 duty-board-0.2.1/duty_board.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-25 14:26:33.000000 duty-board-0.2.1/duty_board.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-25 14:26:33.000000 duty-board-0.2.1/duty_board.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-05-25 14:25:55.000000 duty-board-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 14:26:33.344520 duty-board-0.2.1/setup.cfg
```

### Comparing `duty-board-0.1.0/CONTRIBUTING.md` & `duty-board-0.2.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `duty-board-0.1.0/LICENSE` & `duty-board-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `duty-board-0.1.0/PKG-INFO` & `duty-board-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duty-board
-Version: 0.1.0
+Version: 0.2.1
 Summary: Package to display an overview of all active Duty rosters you have at your Company using iCalendars.
 Author-email: Jorrick Sleijster <jorricks3@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `duty-board-0.1.0/README.md` & `duty-board-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `duty-board-0.1.0/duty_board/alchemy/add_sqladmin.py` & `duty-board-0.2.1/duty_board/alchemy/add_sqladmin.py`

 * *Files identical despite different names*

### Comparing `duty-board-0.1.0/duty_board/alchemy/queries.py` & `duty-board-0.2.1/duty_board/alchemy/queries.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     _PersonEssentials,
     PersonResponse,
 )
 
 
 def format_datetime_for_timezone(dt: datetime.datetime, timezone: BaseTzInfo) -> str:
     dt_tz_aware = dt.astimezone(timezone)
-    return dt_tz_aware.strftime("%Y-%m-%d %H:%M:%S")
+    return dt_tz_aware.strftime("%Y-%m-%d %H:%M:%S %Z")
 
 
 def _get_events_ending_from_now_onwards(
     session: SASession, all_encountered_person_uids: Set[int], timezone: BaseTzInfo
 ) -> Dict[str, List[_Events]]:
     result = session.query(OnCallEvent).filter(OnCallEvent.end_event_utc >= DateTime.utcnow()).all()
     mapped: Dict[str, List[_Events]] = defaultdict(list)
```

### Comparing `duty-board-0.1.0/duty_board/alchemy/session.py` & `duty-board-0.2.1/duty_board/alchemy/session.py`

 * *Files identical despite different names*

### Comparing `duty-board-0.1.0/duty_board/alchemy/settings.py` & `duty-board-0.2.1/duty_board/alchemy/settings.py`

 * *Files identical despite different names*

### Comparing `duty-board-0.1.0/duty_board/alchemy/sqlalchemy_types.py` & `duty-board-0.2.1/duty_board/alchemy/sqlalchemy_types.py`

 * *Files identical despite different names*

### Comparing `duty-board-0.1.0/duty_board/main.py` & `duty-board-0.2.1/duty_board/main.py`

 * *Files identical despite different names*

### Comparing `duty-board-0.1.0/duty_board/models/calendar.py` & `duty-board-0.2.1/duty_board/models/calendar.py`

 * *Files identical despite different names*

### Comparing `duty-board-0.1.0/duty_board/models/generate_fake_data.py` & `duty-board-0.2.1/duty_board/models/generate_fake_data.py`

 * *Files identical despite different names*

### Comparing `duty-board-0.1.0/duty_board/models/on_call_event.py` & `duty-board-0.2.1/duty_board/models/on_call_event.py`

 * *Files identical despite different names*

### Comparing `duty-board-0.1.0/duty_board/models/person.py` & `duty-board-0.2.1/duty_board/models/person.py`

 * *Files identical despite different names*

### Comparing `duty-board-0.1.0/duty_board/models/token.py` & `duty-board-0.2.1/duty_board/models/token.py`

 * *Files identical despite different names*

### Comparing `duty-board-0.1.0/duty_board/plugin/abstract_plugin.py` & `duty-board-0.2.1/duty_board/plugin/abstract_plugin.py`

 * *Files 20% similar despite different names*

```diff
@@ -20,16 +20,29 @@
     text_color_hex: str = "white"
     absolute_path_to_favicon_ico: Path | None = None
     absolute_path_to_company_logo_png: Path | None = None
     # Path on the back-end to the user images folder.
     absolute_path_to_user_images_folder: Path | None = None
     category_order: List[str] = []
     duty_calendar_configurations: List[DutyCalendarConfig] = []
-    enable_admin_button: bool = True
+    enable_admin_button: bool = False
     git_repository_url: Optional[str] = "https://github.com/Jorricks/DutyBoard"
+    footer_html: Optional[
+        str
+    ] = """
+    Welcome to DutyBoard. <br>
+    In case you want to know more check <a href="https://github.com/Jorricks/DutyBoard">here</a>.<br>
+    Cheers!
+    """
+
+    announcement_background_color_hex: str = "#FF0000"
+    announcement_text_color_hex: str = "#FFFFFF"
+    announcements: List[str] = [
+        "This is a debug setup. Please disable this announcement in your plugin by overwriting announcements variable.",
+    ]
 
     def __init__(self, *args, **kwargs):
         super(AbstractPlugin, self).__init__(*args, **kwargs)
 
     @abstractmethod
     def sync_person(self, person: Person, session: SASession) -> Person:
         pass
```

### Comparing `duty-board-0.1.0/duty_board/plugin/example/example_logo.png` & `duty-board-0.2.1/duty_board/plugin/example/example_logo.png`

 * *Files identical despite different names*

### Comparing `duty-board-0.1.0/duty_board/plugin/example/example_plugin.py` & `duty-board-0.2.1/duty_board/plugin/example/example_plugin.py`

 * *Files identical despite different names*

### Comparing `duty-board-0.1.0/duty_board/plugin/example/favicon.ico` & `duty-board-0.2.1/duty_board/plugin/example/favicon.ico`

 * *Files identical despite different names*

### Comparing `duty-board-0.1.0/duty_board/plugin/helpers/duty_calendar_config.py` & `duty-board-0.2.1/duty_board/plugin/helpers/duty_calendar_config.py`

 * *Files identical despite different names*

### Comparing `duty-board-0.1.0/duty_board/plugin/helpers/plugin_fetcher.py` & `duty-board-0.2.1/duty_board/plugin/helpers/plugin_fetcher.py`

 * *Files identical despite different names*

### Comparing `duty-board-0.1.0/duty_board/plugin/ical_plugin_mixin.py` & `duty-board-0.2.1/duty_board/plugin/ical_plugin_mixin.py`

 * *Files identical despite different names*

### Comparing `duty-board-0.1.0/duty_board/plugin/ldap_plugin_mixin.py` & `duty-board-0.2.1/duty_board/plugin/ldap_plugin_mixin.py`

 * *Files identical despite different names*

### Comparing `duty-board-0.1.0/duty_board/server.py` & `duty-board-0.2.1/duty_board/server.py`

 * *Files 5% similar despite different names*

```diff
@@ -64,14 +64,18 @@
 def _get_config_object(timezone_object: BaseTzInfo) -> _Config:
     return _Config(
         text_color=plugin.text_color_hex,
         background_color=plugin.background_color_hex,
         categories=plugin.category_order,
         git_repository_url=plugin.git_repository_url,
         enable_admin_button=plugin.enable_admin_button,
+        announcement_text_color=plugin.announcement_text_color_hex,
+        announcement_background_color=plugin.announcement_background_color_hex,
+        announcements=plugin.announcements,
+        footer_html=plugin.footer_html,
         timezone=timezone_object.zone,
     )
 
 
 @app.get("/get_schedule", response_model=CurrentSchedule)
 async def get_schedule(timezone: str):
     timezone_object = _parse_timezone_str(timezone)
```

### Comparing `duty-board-0.1.0/duty_board/web_helpers/generate_typescript_api.py` & `duty-board-0.2.1/duty_board/web_helpers/generate_typescript_api.py`

 * *Files identical despite different names*

### Comparing `duty-board-0.1.0/duty_board/web_helpers/gzip_static_files.py` & `duty-board-0.2.1/duty_board/web_helpers/gzip_static_files.py`

 * *Files identical despite different names*

### Comparing `duty-board-0.1.0/duty_board/web_helpers/response_types.py` & `duty-board-0.2.1/duty_board/web_helpers/response_types.py`

 * *Files 23% similar despite different names*

```diff
@@ -30,14 +30,18 @@
 class _Config(BaseModel):
     timezone: str
     text_color: str
     background_color: str
     categories: List[str]
     git_repository_url: Optional[str]
     enable_admin_button: bool
+    announcement_text_color: str
+    announcement_background_color: str
+    announcements: List[str]
+    footer_html: Optional[str]
 
 
 class CurrentSchedule(BaseModel):
     config: _Config
     calendars: List[_Calendar]
     persons: Dict[int, _PersonEssentials]
```

### Comparing `duty-board-0.1.0/duty_board/worker_loop.py` & `duty-board-0.2.1/duty_board/worker_loop.py`

 * *Files identical despite different names*

### Comparing `duty-board-0.1.0/duty_board/www/dist/809.js` & `duty-board-0.2.1/duty_board/www/dist/809.js`

 * *Files identical despite different names*

### Comparing `duty-board-0.1.0/duty_board/www/dist/809.js.gz` & `duty-board-0.2.1/duty_board/www/dist/809.js.gz`

 * *Files identical despite different names*

### Comparing `duty-board-0.1.0/duty_board/www/dist/index.html` & `duty-board-0.2.1/duty_board/www/dist/index.html`

 * *Files 5% similar despite different names*

```diff
@@ -1 +1 @@
-<!doctype html><html lang="en"><head><meta charset="utf-8"/><link rel="icon" href="favicon.ico"/><meta name="viewport" content="width=device-width,initial-scale=1"/><meta name="theme-color" content="#000000"/><meta name="description" content="DutyBoard - See the Duty schedules of your organisation"/><link rel="apple-touch-icon" href="/logo1922.png"/><link rel="manifest" href="/manifest.json"/><title>DutyBoard</title><script defer="defer" src="/dist/main.js"></script><link href="/dist/main.0b8533bbfe9fae93806d.css" rel="stylesheet"></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div></body></html>
+<!doctype html><html lang="en"><head><meta charset="utf-8"/><link rel="icon" href="/favicon.ico"/><meta name="viewport" content="width=device-width,initial-scale=1"/><meta name="theme-color" content="#000000"/><meta name="description" content="DutyBoard - See the Duty schedules of your organisation"/><link rel="apple-touch-icon" href="/logo1922.png"/><link rel="manifest" href="/manifest.json"/><title>DutyBoard</title><script defer="defer" src="/dist/main.js"></script><link href="/dist/main.e82352a304d245533b70.css" rel="stylesheet"></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div></body></html>
```

### Comparing `duty-board-0.1.0/duty_board/www/dist/main.0b8533bbfe9fae93806d.css` & `duty-board-0.2.1/duty_board/www/dist/main.e82352a304d245533b70.css`

 * *Files 2% similar despite different names*

```diff
@@ -1,2 +1,2 @@
 body{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Oxygen,Ubuntu,Cantarell,Fira Sans,Droid Sans,Helvetica Neue,sans-serif;margin:0}code{font-family:source-code-pro,Menlo,Monaco,Consolas,Courier New,monospace}.App{text-align:center}.App-logo{height:40vmin;pointer-events:none}@media (prefers-reduced-motion:no-preference){.App-logo{animation:App-logo-spin 20s linear infinite}}.App-header{align-items:center;background-color:#282c34;color:#fff;display:flex;flex-direction:column;font-size:calc(10px + 2vmin);justify-content:center;min-height:100vh}.App-link{color:#61dafb}@keyframes App-logo-spin{0%{transform:rotate(0deg)}to{transform:rotate(1turn)}}.loader{animation:load8 1.1s linear infinite;border:1.1em solid rgba(0,0,0,.2);border-left-color:#000;border-radius:50%;height:6em;left:calc(50% - 4em);position:absolute;top:calc(50% - 4em);transition:opacity .3s;width:6em}.loader--hide{opacity:0}@keyframes load8{0%{transform:rotate(0deg)}to{transform:rotate(1turn)}}.code-snippet{background:#eee;border-radius:3px;margin-left:2rem;margin-right:2rem;margin-top:2rem;overflow:auto;padding:1rem}.code-snippet .code{word-wrap:normal;line-height:1.5;text-align:left;white-space:pre;word-break:normal;word-spacing:normal}.circular--landscape{border-radius:50%;display:block;height:200px;margin-left:auto;margin-right:auto;overflow:hidden;position:relative;width:200px}.circular--landscape img{height:100%;margin-left:-50px;max-width:none;width:auto}.circular--portrait{border-radius:50%;height:200px;margin-left:auto;margin-right:auto;overflow:hidden;position:relative;width:200px}.circular--portrait img{height:auto;width:100%}
-/*# sourceMappingURL=main.0b8533bbfe9fae93806d.css.map*/
+/*# sourceMappingURL=main.e82352a304d245533b70.css.map*/
```

### Comparing `duty-board-0.1.0/duty_board/www/dist/main.js` & `duty-board-0.2.1/duty_board/www/dist/main.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -47442,16 +47442,16 @@
             };
         }
 
 
 
         var emptyScheduleData = {
             config: {
-                companyColorHex: "#3C9C2D",
-                categories: ["Loading..", "123"]
+                categories: ["Loading..", "123"],
+                announcements: []
             },
             calendars: [],
             persons: {}
         };
         var useGetSchedule = function useGetSchedule() {
             var _query$data;
             var errorToast = utils_useErrorToast();
@@ -77035,41 +77035,109 @@
                 });
             } else {
                 obj[key] = value;
             }
             return obj;
         }
 
+        function _slicedToArray(arr, i) {
+            return _arrayWithHoles(arr) || _iterableToArrayLimit(arr, i) || _unsupportedIterableToArray(arr, i) || _nonIterableRest();
+        }
+
+        function _nonIterableRest() {
+            throw new TypeError("Invalid attempt to destructure non-iterable instance.\nIn order to be iterable, non-array objects must have a [Symbol.iterator]() method.");
+        }
+
+        function _unsupportedIterableToArray(o, minLen) {
+            if (!o) return;
+            if (typeof o === "string") return _arrayLikeToArray(o, minLen);
+            var n = Object.prototype.toString.call(o).slice(8, -1);
+            if (n === "Object" && o.constructor) n = o.constructor.name;
+            if (n === "Map" || n === "Set") return Array.from(o);
+            if (n === "Arguments" || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(n)) return _arrayLikeToArray(o, minLen);
+        }
+
+        function _arrayLikeToArray(arr, len) {
+            if (len == null || len > arr.length) len = arr.length;
+            for (var i = 0, arr2 = new Array(len); i < len; i++) {
+                arr2[i] = arr[i];
+            }
+            return arr2;
+        }
+
+        function _iterableToArrayLimit(arr, i) {
+            var _i = arr == null ? null : typeof Symbol !== "undefined" && arr[Symbol.iterator] || arr["@@iterator"];
+            if (_i == null) return;
+            var _arr = [];
+            var _n = true;
+            var _d = false;
+            var _s, _e;
+            try {
+                for (_i = _i.call(arr); !(_n = (_s = _i.next()).done); _n = true) {
+                    _arr.push(_s.value);
+                    if (i && _arr.length === i) break;
+                }
+            } catch (err) {
+                _d = true;
+                _e = err;
+            } finally {
+                try {
+                    if (!_n && _i["return"] != null) _i["return"]();
+                } finally {
+                    if (_d) throw _e;
+                }
+            }
+            return _arr;
+        }
+
+        function _arrayWithHoles(arr) {
+            if (Array.isArray(arr)) return arr;
+        }
+
+
+
 
 
 
 
 
 
 
 
         // Huge credits to https://blog.logrocket.com/create-collapsible-react-components-react-collapsed/
         var SingleCalendar = function SingleCalendar(_ref) {
-            var _firstEvent$personUid, _firstEvent$startEven, _firstEvent$endEvent;
-            var calendar = _ref.calendar,
+            var _firstEvent$personUid, _currentRoute$params, _firstEvent$startEven, _firstEvent$endEvent;
+            var category = _ref.category,
+                calendar = _ref.calendar,
                 persons = _ref.persons;
+            var currentRoute = (0, index_production.useMatch)("/$category/$calendarId", {
+                strict: false
+            });
             var firstEvent = calendar.events.length > 0 ? calendar.events[0] : undefined;
             var firstPersonUid = (_firstEvent$personUid = firstEvent === null || firstEvent === void 0 ? void 0 : firstEvent.personUid) !== null && _firstEvent$personUid !== void 0 ? _firstEvent$personUid : undefined;
             var firstPerson = firstPersonUid ? persons.get(firstPersonUid.toString()) : undefined;
+            var _useState = (0, react.useState)((currentRoute === null || currentRoute === void 0 ? void 0 : (_currentRoute$params = currentRoute.params) === null || _currentRoute$params === void 0 ? void 0 : _currentRoute$params.calendarId) == calendar.uid),
+                _useState2 = _slicedToArray(_useState, 2),
+                isExpanded = _useState2[0],
+                setExpanded = _useState2[1];
             var _useCollapse = useCollapse({
+                    isExpanded: isExpanded,
                     duration: 500
                 }),
                 getCollapseProps = _useCollapse.getCollapseProps,
-                getToggleProps = _useCollapse.getToggleProps,
-                isExpanded = _useCollapse.isExpanded;
+                getToggleProps = _useCollapse.getToggleProps;
             var checked = true;
             var colorTextLight = checked ? "white" : "purple.600";
             var bgColorLight = checked ? "purple.400" : "gray.300";
             var colorTextDark = checked ? "white" : "purple.500";
             var bgColorDark = checked ? "purple.400" : "gray.300";
+            (0, react.useEffect)(function() {
+                var _currentRoute$params2;
+                setExpanded((currentRoute === null || currentRoute === void 0 ? void 0 : (_currentRoute$params2 = currentRoute.params) === null || _currentRoute$params2 === void 0 ? void 0 : _currentRoute$params2.calendarId) == calendar.uid);
+            }, [currentRoute]);
             return /*#__PURE__*/ (0, jsx_runtime.jsxs)(jsx_runtime.Fragment, {
                 children: [ /*#__PURE__*/ (0, jsx_runtime.jsxs)(Stack, {
                     p: 3,
                     py: 3,
                     justifyContent: {
                         base: "flex-start",
                         md: "space-around"
@@ -77145,24 +77213,41 @@
                         })
                     }), /*#__PURE__*/ (0, jsx_runtime.jsx)(Box, {
                         width: {
                             base: "auto",
                             md: "10%"
                         },
                         children: /*#__PURE__*/ (0, jsx_runtime.jsx)(Stack, {
-                            children: /*#__PURE__*/ (0, jsx_runtime.jsx)("div", singleCalendar_objectSpread(singleCalendar_objectSpread({
-                                className: "header"
-                            }, getToggleProps()), {}, {
-                                children: /*#__PURE__*/ (0, jsx_runtime.jsx)(Button, {
-                                    size: "md",
-                                    color: useColorModeValue(colorTextLight, colorTextDark),
-                                    bgColor: useColorModeValue(bgColorLight, bgColorDark),
-                                    children: isExpanded ? "Less" : "More"
+                            children: /*#__PURE__*/ (0, jsx_runtime.jsx)("div", {
+                                className: "header",
+                                children: isExpanded ? /*#__PURE__*/ (0, jsx_runtime.jsx)(index_production.Link, {
+                                    to: "/$category",
+                                    params: {
+                                        category: category
+                                    },
+                                    children: /*#__PURE__*/ (0, jsx_runtime.jsx)(Button, {
+                                        size: "md",
+                                        color: useColorModeValue(colorTextLight, colorTextDark),
+                                        bgColor: useColorModeValue(bgColorLight, bgColorDark),
+                                        children: "Less"
+                                    })
+                                }) : /*#__PURE__*/ (0, jsx_runtime.jsx)(index_production.Link, {
+                                    to: "/$category/$calendarId",
+                                    params: {
+                                        category: category,
+                                        calendarId: calendar.uid
+                                    },
+                                    children: /*#__PURE__*/ (0, jsx_runtime.jsx)(Button, {
+                                        size: "md",
+                                        color: useColorModeValue(colorTextLight, colorTextDark),
+                                        bgColor: useColorModeValue(bgColorLight, bgColorDark),
+                                        children: "More"
+                                    })
                                 })
-                            }))
+                            })
                         })
                     })]
                 }), /*#__PURE__*/ (0, jsx_runtime.jsx)("div", singleCalendar_objectSpread(singleCalendar_objectSpread({}, getCollapseProps()), {}, {
                     children: /*#__PURE__*/ (0, jsx_runtime.jsx)("div", {
                         className: "content",
                         children: /*#__PURE__*/ (0, jsx_runtime.jsx)(expandedCalendarInfo, {
                             calendar: calendar,
@@ -77185,22 +77270,16 @@
                 strict: false
             });
             var _useGetSchedule = api_useGetSchedule(),
                 _useGetSchedule$data = _useGetSchedule.data,
                 config = _useGetSchedule$data.config,
                 calendars = _useGetSchedule$data.calendars,
                 persons = _useGetSchedule$data.persons;
-            console.log({
-                data: data
-            });
             var category = data ? decodeURI(data.params.category) : config.categories[0];
             var personsMap = new Map(Object.entries(persons));
-            console.log({
-                category: category
-            });
 
             // Design heavily influenced by https://chakra-templates.dev/page-sections/pricing
             return /*#__PURE__*/ (0, jsx_runtime.jsx)(Box, {
                 py: 6,
                 px: 5,
                 width: "100%",
                 children: /*#__PURE__*/ (0, jsx_runtime.jsx)(Stack, {
@@ -77208,14 +77287,15 @@
                     width: "100%",
                     direction: "column",
                     children: calendars.filter(function(calendar) {
                         return calendar.category == category;
                     }).map(function(calendar, index) {
                         return /*#__PURE__*/ (0, jsx_runtime.jsxs)(Box, {
                             children: [ /*#__PURE__*/ (0, jsx_runtime.jsx)(Divider, {}), /*#__PURE__*/ (0, jsx_runtime.jsx)(singleCalendar, {
+                                category: category,
                                 calendar: calendar,
                                 persons: personsMap
                             }, "singleCalendarNr" + index)]
                         }, index);
                     })
                 })
             });
@@ -77271,15 +77351,14 @@
         var companyLogo = (CompanyLogo);; // CONCATENATED MODULE: ./js/components/footer.tsx
 
 
 
 
 
 
-
         var SocialButton = function SocialButton(_ref) {
             var children = _ref.children,
                 label = _ref.label,
                 href = _ref.href;
             return /*#__PURE__*/ (0, jsx_runtime.jsxs)(chakra.button, {
                 bg: useColorModeValue("blackAlpha.100", "whiteAlpha.100"),
                 rounded: "full",
@@ -77304,53 +77383,33 @@
         function Footer() {
             var _useGetSchedule = api_useGetSchedule(),
                 config = _useGetSchedule.data.config,
                 isLoading = _useGetSchedule.isLoading;
             return /*#__PURE__*/ (0, jsx_runtime.jsxs)(Box, {
                 bg: config.backgroundColor,
                 color: config.textColor,
-                children: [ /*#__PURE__*/ (0, jsx_runtime.jsxs)(index_esm_Container, {
-                    as: Stack,
-                    maxW: "6xl",
-                    py: 4,
-                    spacing: 4,
-                    justify: "center",
-                    align: "center",
-                    children: [ /*#__PURE__*/ (0, jsx_runtime.jsx)(companyLogo, {
-                        maxWidth: 250,
-                        maxHeight: 150
-                    }), /*#__PURE__*/ (0, jsx_runtime.jsx)(Stack, {
-                        direction: "row",
-                        spacing: 6,
-                        children: config.categories.map(function(aCategory) {
-                            return /*#__PURE__*/ (0, jsx_runtime.jsx)(index_production.Link, {
-                                to: "/$category",
-                                params: {
-                                    category: aCategory
-                                },
-                                activeProps: {
-                                    className: "font-bold"
-                                },
-                                children: aCategory
-                            }, "footer" + aCategory);
-                        })
-                    }), /*#__PURE__*/ (0, jsx_runtime.jsx)(index_esm_Container, {
+                children: [ /*#__PURE__*/ (0, jsx_runtime.jsx)(Box, {
+                    children: /*#__PURE__*/ (0, jsx_runtime.jsxs)(index_esm_Container, {
                         as: Stack,
-                        justify: {
-                            base: "center",
-                            md: "space-between"
-                        },
-                        align: {
-                            base: "center",
-                            md: "center"
-                        },
-                        children: /*#__PURE__*/ (0, jsx_runtime.jsxs)(Text, {
-                            children: ["All dates & times are in your local timezone; ", config.timezone]
-                        })
-                    })]
+                        maxW: "6xl",
+                        py: 4,
+                        spacing: 4,
+                        justify: "center",
+                        align: "center",
+                        children: [ /*#__PURE__*/ (0, jsx_runtime.jsx)(Box, {
+                            dangerouslySetInnerHTML: {
+                                __html: config.footerHtml
+                            },
+                            display: "block",
+                            width: "100%"
+                        }), /*#__PURE__*/ (0, jsx_runtime.jsx)(companyLogo, {
+                            maxWidth: 250,
+                            maxHeight: 150
+                        })]
+                    })
                 }), /*#__PURE__*/ (0, jsx_runtime.jsx)(Box, {
                     borderTopWidth: 1,
                     borderStyle: "solid",
                     borderColor: useColorModeValue("gray.200", "gray.700"),
                     children: /*#__PURE__*/ (0, jsx_runtime.jsxs)(index_esm_Container, {
                         as: Stack,
                         maxW: "6xl",
@@ -79808,39 +79867,72 @@
                                     children: category
                                 }, "mobile" + category);
                             })
                         })
                     }) : null]
                 })
             });
+        }; // CONCATENATED MODULE: ./js/components/announcementBar.tsx
+
+
+
+
+        function AnnouncementBar() {
+            var _useDisclosure = index_esm_useDisclosure(),
+                isOpen = _useDisclosure.isOpen,
+                onOpen = _useDisclosure.onOpen,
+                onClose = _useDisclosure.onClose;
+            var _useGetSchedule = api_useGetSchedule(),
+                config = _useGetSchedule.data.config,
+                isLoading = _useGetSchedule.isLoading;
+            return /*#__PURE__*/ (0, jsx_runtime.jsx)(jsx_runtime.Fragment, {
+                children: /*#__PURE__*/ (0, jsx_runtime.jsx)(Box, {
+                    bg: config.announcementBackgroundColor,
+                    color: config.announcementTextColor,
+                    px: 4,
+                    fontWeight: 700,
+                    children: config.announcements.map(function(announcement, index) {
+                        return /*#__PURE__*/ (0, jsx_runtime.jsx)(HStack, {
+                            spacing: 8,
+                            alignItems: "center",
+                            justifyContent: "center",
+                            children: /*#__PURE__*/ (0, jsx_runtime.jsx)(Text, {
+                                padding: "20px",
+                                children: announcement
+                            })
+                        }, index);
+                    })
+                })
+            });
         }; // CONCATENATED MODULE: ./js/App.tsx
 
 
 
 
 
 
 
 
 
 
+
         var rootRoute = (0, index_production.createRouteConfig)();
         var indexRoute = rootRoute.createRoute({
             path: "/",
             component: schedule
         });
         var categoryRoute = rootRoute.createRoute({
             path: "$category",
             component: schedule
         });
-        var personRoute = categoryRoute.createRoute({
-            path: "$personId",
-            component: personComponent
+        var calendarRoute = categoryRoute.createRoute({
+            path: "$calendarId",
+            component: singleCalendar
         });
-        var routeConfig = rootRoute.addChildren([indexRoute, categoryRoute.addChildren([personRoute])]);
+        var routeConfig = rootRoute.addChildren([indexRoute, categoryRoute.addChildren([calendarRoute])]);
 
         // Set up a ReactRouter instance
         var router = (0, index_production.createReactRouter)({
             routeConfig: routeConfig,
             defaultPreload: "intent"
         });
         var queryClient = new react_query_es.QueryClient({
@@ -79873,15 +79965,15 @@
                         children: /*#__PURE__*/ (0, jsx_runtime.jsxs)("div", {
                             children: [ /*#__PURE__*/ (0, jsx_runtime.jsxs)("div", {
                                 style: {
                                     minHeight: "100vh",
                                     display: "flex",
                                     flexDirection: "column"
                                 },
-                                children: [ /*#__PURE__*/ (0, jsx_runtime.jsx)(Navbar, {}), /*#__PURE__*/ (0, jsx_runtime.jsx)(index_production.Outlet, {}), " ", /*#__PURE__*/ (0, jsx_runtime.jsx)("div", {
+                                children: [ /*#__PURE__*/ (0, jsx_runtime.jsx)(AnnouncementBar, {}), /*#__PURE__*/ (0, jsx_runtime.jsx)(Navbar, {}), /*#__PURE__*/ (0, jsx_runtime.jsx)(index_production.Outlet, {}), " ", /*#__PURE__*/ (0, jsx_runtime.jsx)("div", {
                                     style: {
                                         marginTop: "auto"
                                     },
                                     children: /*#__PURE__*/ (0, jsx_runtime.jsx)(Footer, {})
                                 })]
                             }), /*#__PURE__*/ (0, jsx_runtime.jsx)("div", {})]
                         })
```

### Comparing `duty-board-0.1.0/duty_board/www/static/favicon.ico` & `duty-board-0.2.1/duty_board/www/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `duty-board-0.1.0/duty_board/www/static/logo192.png` & `duty-board-0.2.1/duty_board/www/static/logo192.png`

 * *Files identical despite different names*

### Comparing `duty-board-0.1.0/duty_board/www/static/logo512.png` & `duty-board-0.2.1/duty_board/www/static/logo512.png`

 * *Files identical despite different names*

### Comparing `duty-board-0.1.0/duty_board/www/user_images/bert.jpeg` & `duty-board-0.2.1/duty_board/www/user_images/bert.jpeg`

 * *Files identical despite different names*

### Comparing `duty-board-0.1.0/duty_board/www/user_images/bert2.jpg` & `duty-board-0.2.1/duty_board/www/user_images/bert2.jpg`

 * *Files identical despite different names*

### Comparing `duty-board-0.1.0/duty_board.egg-info/PKG-INFO` & `duty-board-0.2.1/duty_board.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duty-board
-Version: 0.1.0
+Version: 0.2.1
 Summary: Package to display an overview of all active Duty rosters you have at your Company using iCalendars.
 Author-email: Jorrick Sleijster <jorricks3@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `duty-board-0.1.0/duty_board.egg-info/SOURCES.txt` & `duty-board-0.2.1/duty_board.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -41,16 +41,16 @@
 duty_board/web_helpers/generate_typescript_api.py
 duty_board/web_helpers/gzip_static_files.py
 duty_board/web_helpers/response_types.py
 duty_board/www/dist/809.js
 duty_board/www/dist/809.js.gz
 duty_board/www/dist/index.html
 duty_board/www/dist/index.html.gz
-duty_board/www/dist/main.0b8533bbfe9fae93806d.css
-duty_board/www/dist/main.0b8533bbfe9fae93806d.css.gz
+duty_board/www/dist/main.e82352a304d245533b70.css
+duty_board/www/dist/main.e82352a304d245533b70.css.gz
 duty_board/www/dist/main.js
 duty_board/www/dist/main.js.gz
 duty_board/www/dist/manifest.json
 duty_board/www/dist/manifest.json.gz
 duty_board/www/static/favicon.ico
 duty_board/www/static/logo192.png
 duty_board/www/static/logo512.png
```

### Comparing `duty-board-0.1.0/duty_board.egg-info/requires.txt` & `duty-board-0.2.1/duty_board.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `duty-board-0.1.0/pyproject.toml` & `duty-board-0.2.1/pyproject.toml`

 * *Files identical despite different names*

