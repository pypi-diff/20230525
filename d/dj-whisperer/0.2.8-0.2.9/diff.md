# Comparing `tmp/dj-whisperer-0.2.8.tar.gz` & `tmp/dj-whisperer-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dj-whisperer-0.2.8.tar", last modified: Mon Mar 22 11:04:57 2021, max compression
+gzip compressed data, was "dist/dj-whisperer-0.2.9.tar", last modified: Fri May 21 09:40:05 2021, max compression
```

## Comparing `dj-whisperer-0.2.8.tar` & `dj-whisperer-0.2.9.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2021-03-22 11:04:57.000000 dj-whisperer-0.2.8/
--rw-rw-rw-   0 root         (0) root         (0)     1259 2021-03-22 11:04:00.000000 dj-whisperer-0.2.8/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      113 2021-03-22 11:04:00.000000 dj-whisperer-0.2.8/.isort.cfg
--rw-rw-rw-   0 root         (0) root         (0)       28 2021-03-22 11:04:00.000000 dj-whisperer-0.2.8/CHANGELOG.md
--rw-rw-rw-   0 root         (0) root         (0)     1050 2021-03-22 11:04:00.000000 dj-whisperer-0.2.8/LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)     5137 2021-03-22 11:04:57.000000 dj-whisperer-0.2.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3025 2021-03-22 11:04:00.000000 dj-whisperer-0.2.8/README.md
--rw-rw-rw-   0 root         (0) root         (0)     2373 2021-03-22 11:04:00.000000 dj-whisperer-0.2.8/bitbucket-pipelines.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2021-03-22 11:04:57.000000 dj-whisperer-0.2.8/dj_whisperer.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     5137 2021-03-22 11:04:57.000000 dj-whisperer-0.2.8/dj_whisperer.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1399 2021-03-22 11:04:57.000000 dj-whisperer-0.2.8/dj_whisperer.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2021-03-22 11:04:57.000000 dj-whisperer-0.2.8/dj_whisperer.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2021-03-22 11:04:57.000000 dj-whisperer-0.2.8/dj_whisperer.egg-info/not-zip-safe
--rw-rw-rw-   0 root         (0) root         (0)       10 2021-03-22 11:04:57.000000 dj-whisperer-0.2.8/dj_whisperer.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2021-03-22 11:04:57.000000 dj-whisperer-0.2.8/docs/
--rw-rw-rw-   0 root         (0) root         (0)      634 2021-03-22 11:04:00.000000 dj-whisperer-0.2.8/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)     4339 2021-03-22 11:04:00.000000 dj-whisperer-0.2.8/docs/advanced.rst
--rw-rw-rw-   0 root         (0) root         (0)     2077 2021-03-22 11:04:00.000000 dj-whisperer-0.2.8/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)     1186 2021-03-22 11:04:00.000000 dj-whisperer-0.2.8/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      806 2021-03-22 11:04:00.000000 dj-whisperer-0.2.8/docs/introduction.rst
--rw-rw-rw-   0 root         (0) root         (0)      795 2021-03-22 11:04:00.000000 dj-whisperer-0.2.8/docs/make.bat
--rw-rw-rw-   0 root         (0) root         (0)     2658 2021-03-22 11:04:00.000000 dj-whisperer-0.2.8/docs/quickstart.rst
--rw-rw-rw-   0 root         (0) root         (0)      310 2021-03-22 11:04:00.000000 dj-whisperer-0.2.8/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      238 2021-03-22 11:04:00.000000 dj-whisperer-0.2.8/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      410 2021-03-22 11:04:00.000000 dj-whisperer-0.2.8/runtests.py
--rw-rw-rw-   0 root         (0) root         (0)       38 2021-03-22 11:04:57.000000 dj-whisperer-0.2.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2064 2021-03-22 11:04:00.000000 dj-whisperer-0.2.8/setup.py
--rw-rw-rw-   0 root         (0) root         (0)     1427 2021-03-22 11:04:00.000000 dj-whisperer-0.2.8/tox.ini
-drwxrwxrwx   0 root         (0) root         (0)        0 2021-03-22 11:04:57.000000 dj-whisperer-0.2.8/whisperer/
--rw-rw-rw-   0 root         (0) root         (0)      328 2021-03-22 11:04:00.000000 dj-whisperer-0.2.8/whisperer/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      362 2021-03-22 11:04:00.000000 dj-whisperer-0.2.8/whisperer/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      150 2021-03-22 11:04:00.000000 dj-whisperer-0.2.8/whisperer/apps.py
--rw-rw-rw-   0 root         (0) root         (0)     1746 2021-03-22 11:04:00.000000 dj-whisperer-0.2.8/whisperer/client.py
--rw-rw-rw-   0 root         (0) root         (0)      624 2021-03-22 11:04:00.000000 dj-whisperer-0.2.8/whisperer/codes.py
--rw-rw-rw-   0 root         (0) root         (0)      336 2021-03-22 11:04:00.000000 dj-whisperer-0.2.8/whisperer/conf.py
--rw-rw-rw-   0 root         (0) root         (0)     1832 2021-03-22 11:04:00.000000 dj-whisperer-0.2.8/whisperer/countdown.py
--rw-rw-rw-   0 root         (0) root         (0)     1494 2021-03-22 11:04:00.000000 dj-whisperer-0.2.8/whisperer/events.py
--rw-rw-rw-   0 root         (0) root         (0)     1778 2021-03-22 11:04:00.000000 dj-whisperer-0.2.8/whisperer/exceptions.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2021-03-22 11:04:57.000000 dj-whisperer-0.2.8/whisperer/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     2704 2021-03-22 11:04:00.000000 dj-whisperer-0.2.8/whisperer/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      452 2021-03-22 11:04:00.000000 dj-whisperer-0.2.8/whisperer/migrations/0002_webhook_additional_headers.py
--rw-rw-rw-   0 root         (0) root         (0)      827 2021-03-22 11:04:00.000000 dj-whisperer-0.2.8/whisperer/migrations/0003_auto_20200505_0853.py
--rw-rw-rw-   0 root         (0) root         (0)      648 2021-03-22 11:04:00.000000 dj-whisperer-0.2.8/whisperer/migrations/0004_webhook_retry_count.py
--rw-rw-rw-   0 root         (0) root         (0)      518 2021-03-22 11:04:00.000000 dj-whisperer-0.2.8/whisperer/migrations/0005_webhook_config.py
--rw-rw-rw-   0 root         (0) root         (0)      638 2021-03-22 11:04:00.000000 dj-whisperer-0.2.8/whisperer/migrations/0006_auto_20200925_1710.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-03-22 11:04:00.000000 dj-whisperer-0.2.8/whisperer/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2967 2021-03-22 11:04:00.000000 dj-whisperer-0.2.8/whisperer/models.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2021-03-22 11:04:57.000000 dj-whisperer-0.2.8/whisperer/resources/
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-03-22 11:04:00.000000 dj-whisperer-0.2.8/whisperer/resources/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2318 2021-03-22 11:04:00.000000 dj-whisperer-0.2.8/whisperer/resources/filters.py
--rw-rw-rw-   0 root         (0) root         (0)     1316 2021-03-22 11:04:00.000000 dj-whisperer-0.2.8/whisperer/resources/serializers.py
--rw-rw-rw-   0 root         (0) root         (0)     1451 2021-03-22 11:04:00.000000 dj-whisperer-0.2.8/whisperer/resources/views.py
--rw-rw-rw-   0 root         (0) root         (0)     1403 2021-03-22 11:04:00.000000 dj-whisperer-0.2.8/whisperer/services.py
--rw-rw-rw-   0 root         (0) root         (0)     6442 2021-03-22 11:04:00.000000 dj-whisperer-0.2.8/whisperer/tasks.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2021-03-22 11:04:57.000000 dj-whisperer-0.2.8/whisperer/tests/
--rw-rw-rw-   0 root         (0) root         (0)      119 2021-03-22 11:04:00.000000 dj-whisperer-0.2.8/whisperer/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      209 2021-03-22 11:04:00.000000 dj-whisperer-0.2.8/whisperer/tests/celery.py
--rw-rw-rw-   0 root         (0) root         (0)     1473 2021-03-22 11:04:00.000000 dj-whisperer-0.2.8/whisperer/tests/models.py
--rw-rw-rw-   0 root         (0) root         (0)      200 2021-03-22 11:04:00.000000 dj-whisperer-0.2.8/whisperer/tests/serializers.py
--rw-rw-rw-   0 root         (0) root         (0)      465 2021-03-22 11:04:00.000000 dj-whisperer-0.2.8/whisperer/tests/test_settings.py
--rw-rw-rw-   0 root         (0) root         (0)    20134 2021-03-22 11:04:00.000000 dj-whisperer-0.2.8/whisperer/tests/tests.py
--rw-rw-rw-   0 root         (0) root         (0)      769 2021-03-22 11:04:00.000000 dj-whisperer-0.2.8/whisperer/tests/webhooks.py
--rw-rw-rw-   0 root         (0) root         (0)      440 2021-03-22 11:04:00.000000 dj-whisperer-0.2.8/whisperer/urls.py
--rw-rw-rw-   0 root         (0) root         (0)     1648 2021-03-22 11:04:00.000000 dj-whisperer-0.2.8/whisperer/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1516 2021-03-22 11:04:00.000000 dj-whisperer-0.2.8/whisperer/validators.py
--rw-rw-rw-   0 root         (0) root         (0)       63 2021-03-22 11:04:00.000000 dj-whisperer-0.2.8/whisperer/views.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2021-05-21 09:40:05.000000 dj-whisperer-0.2.9/
+-rw-rw-rw-   0 root         (0) root         (0)     1259 2021-05-21 09:39:00.000000 dj-whisperer-0.2.9/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      113 2021-05-21 09:39:00.000000 dj-whisperer-0.2.9/.isort.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       28 2021-05-21 09:39:00.000000 dj-whisperer-0.2.9/CHANGELOG.md
+-rw-rw-rw-   0 root         (0) root         (0)     1050 2021-05-21 09:39:00.000000 dj-whisperer-0.2.9/LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)     5137 2021-05-21 09:40:05.000000 dj-whisperer-0.2.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3025 2021-05-21 09:39:00.000000 dj-whisperer-0.2.9/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     2373 2021-05-21 09:39:00.000000 dj-whisperer-0.2.9/bitbucket-pipelines.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2021-05-21 09:40:05.000000 dj-whisperer-0.2.9/dj_whisperer.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     5137 2021-05-21 09:40:05.000000 dj-whisperer-0.2.9/dj_whisperer.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1399 2021-05-21 09:40:05.000000 dj-whisperer-0.2.9/dj_whisperer.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2021-05-21 09:40:05.000000 dj-whisperer-0.2.9/dj_whisperer.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2021-05-21 09:40:05.000000 dj-whisperer-0.2.9/dj_whisperer.egg-info/not-zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)       10 2021-05-21 09:40:05.000000 dj-whisperer-0.2.9/dj_whisperer.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2021-05-21 09:40:05.000000 dj-whisperer-0.2.9/docs/
+-rw-rw-rw-   0 root         (0) root         (0)      634 2021-05-21 09:39:00.000000 dj-whisperer-0.2.9/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)     4339 2021-05-21 09:39:00.000000 dj-whisperer-0.2.9/docs/advanced.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2077 2021-05-21 09:39:00.000000 dj-whisperer-0.2.9/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)     1186 2021-05-21 09:39:00.000000 dj-whisperer-0.2.9/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      806 2021-05-21 09:39:00.000000 dj-whisperer-0.2.9/docs/introduction.rst
+-rw-rw-rw-   0 root         (0) root         (0)      795 2021-05-21 09:39:00.000000 dj-whisperer-0.2.9/docs/make.bat
+-rw-rw-rw-   0 root         (0) root         (0)     2658 2021-05-21 09:39:00.000000 dj-whisperer-0.2.9/docs/quickstart.rst
+-rw-rw-rw-   0 root         (0) root         (0)      310 2021-05-21 09:39:00.000000 dj-whisperer-0.2.9/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      238 2021-05-21 09:39:00.000000 dj-whisperer-0.2.9/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)      410 2021-05-21 09:39:00.000000 dj-whisperer-0.2.9/runtests.py
+-rw-rw-rw-   0 root         (0) root         (0)       38 2021-05-21 09:40:05.000000 dj-whisperer-0.2.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2064 2021-05-21 09:39:00.000000 dj-whisperer-0.2.9/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)     1427 2021-05-21 09:39:00.000000 dj-whisperer-0.2.9/tox.ini
+drwxrwxrwx   0 root         (0) root         (0)        0 2021-05-21 09:40:05.000000 dj-whisperer-0.2.9/whisperer/
+-rw-rw-rw-   0 root         (0) root         (0)      328 2021-05-21 09:39:00.000000 dj-whisperer-0.2.9/whisperer/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      362 2021-05-21 09:39:00.000000 dj-whisperer-0.2.9/whisperer/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      150 2021-05-21 09:39:00.000000 dj-whisperer-0.2.9/whisperer/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)     1746 2021-05-21 09:39:00.000000 dj-whisperer-0.2.9/whisperer/client.py
+-rw-rw-rw-   0 root         (0) root         (0)      624 2021-05-21 09:39:00.000000 dj-whisperer-0.2.9/whisperer/codes.py
+-rw-rw-rw-   0 root         (0) root         (0)      336 2021-05-21 09:39:00.000000 dj-whisperer-0.2.9/whisperer/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)     1887 2021-05-21 09:39:00.000000 dj-whisperer-0.2.9/whisperer/countdown.py
+-rw-rw-rw-   0 root         (0) root         (0)     1494 2021-05-21 09:39:00.000000 dj-whisperer-0.2.9/whisperer/events.py
+-rw-rw-rw-   0 root         (0) root         (0)     1778 2021-05-21 09:39:00.000000 dj-whisperer-0.2.9/whisperer/exceptions.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2021-05-21 09:40:05.000000 dj-whisperer-0.2.9/whisperer/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     2704 2021-05-21 09:39:00.000000 dj-whisperer-0.2.9/whisperer/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)      452 2021-05-21 09:39:00.000000 dj-whisperer-0.2.9/whisperer/migrations/0002_webhook_additional_headers.py
+-rw-rw-rw-   0 root         (0) root         (0)      827 2021-05-21 09:39:00.000000 dj-whisperer-0.2.9/whisperer/migrations/0003_auto_20200505_0853.py
+-rw-rw-rw-   0 root         (0) root         (0)      648 2021-05-21 09:39:00.000000 dj-whisperer-0.2.9/whisperer/migrations/0004_webhook_retry_count.py
+-rw-rw-rw-   0 root         (0) root         (0)      518 2021-05-21 09:39:00.000000 dj-whisperer-0.2.9/whisperer/migrations/0005_webhook_config.py
+-rw-rw-rw-   0 root         (0) root         (0)      638 2021-05-21 09:39:00.000000 dj-whisperer-0.2.9/whisperer/migrations/0006_auto_20200925_1710.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2021-05-21 09:39:00.000000 dj-whisperer-0.2.9/whisperer/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2967 2021-05-21 09:39:00.000000 dj-whisperer-0.2.9/whisperer/models.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2021-05-21 09:40:05.000000 dj-whisperer-0.2.9/whisperer/resources/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2021-05-21 09:39:00.000000 dj-whisperer-0.2.9/whisperer/resources/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2318 2021-05-21 09:39:00.000000 dj-whisperer-0.2.9/whisperer/resources/filters.py
+-rw-rw-rw-   0 root         (0) root         (0)     1316 2021-05-21 09:39:00.000000 dj-whisperer-0.2.9/whisperer/resources/serializers.py
+-rw-rw-rw-   0 root         (0) root         (0)     1451 2021-05-21 09:39:00.000000 dj-whisperer-0.2.9/whisperer/resources/views.py
+-rw-rw-rw-   0 root         (0) root         (0)     1403 2021-05-21 09:39:00.000000 dj-whisperer-0.2.9/whisperer/services.py
+-rw-rw-rw-   0 root         (0) root         (0)     6442 2021-05-21 09:39:00.000000 dj-whisperer-0.2.9/whisperer/tasks.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2021-05-21 09:40:05.000000 dj-whisperer-0.2.9/whisperer/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      119 2021-05-21 09:39:00.000000 dj-whisperer-0.2.9/whisperer/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      209 2021-05-21 09:39:00.000000 dj-whisperer-0.2.9/whisperer/tests/celery.py
+-rw-rw-rw-   0 root         (0) root         (0)     1473 2021-05-21 09:39:00.000000 dj-whisperer-0.2.9/whisperer/tests/models.py
+-rw-rw-rw-   0 root         (0) root         (0)      200 2021-05-21 09:39:00.000000 dj-whisperer-0.2.9/whisperer/tests/serializers.py
+-rw-rw-rw-   0 root         (0) root         (0)      465 2021-05-21 09:39:00.000000 dj-whisperer-0.2.9/whisperer/tests/test_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)    20204 2021-05-21 09:39:00.000000 dj-whisperer-0.2.9/whisperer/tests/tests.py
+-rw-rw-rw-   0 root         (0) root         (0)      769 2021-05-21 09:39:00.000000 dj-whisperer-0.2.9/whisperer/tests/webhooks.py
+-rw-rw-rw-   0 root         (0) root         (0)      440 2021-05-21 09:39:00.000000 dj-whisperer-0.2.9/whisperer/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)     1648 2021-05-21 09:39:00.000000 dj-whisperer-0.2.9/whisperer/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1594 2021-05-21 09:39:00.000000 dj-whisperer-0.2.9/whisperer/validators.py
+-rw-rw-rw-   0 root         (0) root         (0)       63 2021-05-21 09:39:00.000000 dj-whisperer-0.2.9/whisperer/views.py
```

### Comparing `dj-whisperer-0.2.8/.gitignore` & `dj-whisperer-0.2.9/.gitignore`

 * *Files identical despite different names*

### Comparing `dj-whisperer-0.2.8/LICENSE.txt` & `dj-whisperer-0.2.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dj-whisperer-0.2.8/PKG-INFO` & `dj-whisperer-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dj-whisperer
-Version: 0.2.8
+Version: 0.2.9
 Summary: Stay informed of it
 Home-page: https://bitbucket.org/akinonteam/dj-whisperer
 Author: Akinon
 Author-email: dev@akinon.com
 Maintainer: Akinon
 Maintainer-email: dev@akinon.com
 License: MIT
```

### Comparing `dj-whisperer-0.2.8/README.md` & `dj-whisperer-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `dj-whisperer-0.2.8/bitbucket-pipelines.yml` & `dj-whisperer-0.2.9/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `dj-whisperer-0.2.8/dj_whisperer.egg-info/PKG-INFO` & `dj-whisperer-0.2.9/dj_whisperer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dj-whisperer
-Version: 0.2.8
+Version: 0.2.9
 Summary: Stay informed of it
 Home-page: https://bitbucket.org/akinonteam/dj-whisperer
 Author: Akinon
 Author-email: dev@akinon.com
 Maintainer: Akinon
 Maintainer-email: dev@akinon.com
 License: MIT
```

### Comparing `dj-whisperer-0.2.8/dj_whisperer.egg-info/SOURCES.txt` & `dj-whisperer-0.2.9/dj_whisperer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dj-whisperer-0.2.8/docs/Makefile` & `dj-whisperer-0.2.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dj-whisperer-0.2.8/docs/advanced.rst` & `dj-whisperer-0.2.9/docs/advanced.rst`

 * *Files identical despite different names*

### Comparing `dj-whisperer-0.2.8/docs/conf.py` & `dj-whisperer-0.2.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dj-whisperer-0.2.8/docs/index.rst` & `dj-whisperer-0.2.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `dj-whisperer-0.2.8/docs/introduction.rst` & `dj-whisperer-0.2.9/docs/introduction.rst`

 * *Files identical despite different names*

### Comparing `dj-whisperer-0.2.8/docs/make.bat` & `dj-whisperer-0.2.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dj-whisperer-0.2.8/docs/quickstart.rst` & `dj-whisperer-0.2.9/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `dj-whisperer-0.2.8/setup.py` & `dj-whisperer-0.2.9/setup.py`

 * *Files identical despite different names*

### Comparing `dj-whisperer-0.2.8/tox.ini` & `dj-whisperer-0.2.9/tox.ini`

 * *Files identical despite different names*

### Comparing `dj-whisperer-0.2.8/whisperer/client.py` & `dj-whisperer-0.2.9/whisperer/client.py`

 * *Files identical despite different names*

### Comparing `dj-whisperer-0.2.8/whisperer/codes.py` & `dj-whisperer-0.2.9/whisperer/codes.py`

 * *Files identical despite different names*

### Comparing `dj-whisperer-0.2.8/whisperer/countdown.py` & `dj-whisperer-0.2.9/whisperer/countdown.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,21 +36,22 @@
         if self.limit is None:
             return count
         return min(count, self.limit)
 
 
 @countdown_classes.register(key='exponential')
 class ExponentialRetryCountdown(BaseRetryCountdown):
-    def __init__(self, base, limit=None):
+    def __init__(self, base, factor=1, limit=None):
         super(ExponentialRetryCountdown, self).__init__()
         self.base = base
         self.limit = limit
+        self.factor = factor
 
     def get_value(self, retry_count):
-        count = self.base ** retry_count
+        count = (self.base ** retry_count) * self.factor
         if self.limit is None:
             return count
         return min(count, self.limit)
 
 
 @countdown_classes.register(key='random')
 class RandomRetryCountdown(BaseRetryCountdown):
```

### Comparing `dj-whisperer-0.2.8/whisperer/events.py` & `dj-whisperer-0.2.9/whisperer/events.py`

 * *Files identical despite different names*

### Comparing `dj-whisperer-0.2.8/whisperer/exceptions.py` & `dj-whisperer-0.2.9/whisperer/exceptions.py`

 * *Files identical despite different names*

### Comparing `dj-whisperer-0.2.8/whisperer/migrations/0001_initial.py` & `dj-whisperer-0.2.9/whisperer/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `dj-whisperer-0.2.8/whisperer/migrations/0003_auto_20200505_0853.py` & `dj-whisperer-0.2.9/whisperer/migrations/0003_auto_20200505_0853.py`

 * *Files identical despite different names*

### Comparing `dj-whisperer-0.2.8/whisperer/migrations/0004_webhook_retry_count.py` & `dj-whisperer-0.2.9/whisperer/migrations/0004_webhook_retry_count.py`

 * *Files identical despite different names*

### Comparing `dj-whisperer-0.2.8/whisperer/migrations/0005_webhook_config.py` & `dj-whisperer-0.2.9/whisperer/migrations/0005_webhook_config.py`

 * *Files identical despite different names*

### Comparing `dj-whisperer-0.2.8/whisperer/migrations/0006_auto_20200925_1710.py` & `dj-whisperer-0.2.9/whisperer/migrations/0006_auto_20200925_1710.py`

 * *Files identical despite different names*

### Comparing `dj-whisperer-0.2.8/whisperer/models.py` & `dj-whisperer-0.2.9/whisperer/models.py`

 * *Files identical despite different names*

### Comparing `dj-whisperer-0.2.8/whisperer/resources/filters.py` & `dj-whisperer-0.2.9/whisperer/resources/filters.py`

 * *Files identical despite different names*

### Comparing `dj-whisperer-0.2.8/whisperer/resources/serializers.py` & `dj-whisperer-0.2.9/whisperer/resources/serializers.py`

 * *Files identical despite different names*

### Comparing `dj-whisperer-0.2.8/whisperer/resources/views.py` & `dj-whisperer-0.2.9/whisperer/resources/views.py`

 * *Files identical despite different names*

### Comparing `dj-whisperer-0.2.8/whisperer/services.py` & `dj-whisperer-0.2.9/whisperer/services.py`

 * *Files identical despite different names*

### Comparing `dj-whisperer-0.2.8/whisperer/tasks.py` & `dj-whisperer-0.2.9/whisperer/tasks.py`

 * *Files identical despite different names*

### Comparing `dj-whisperer-0.2.8/whisperer/tests/models.py` & `dj-whisperer-0.2.9/whisperer/tests/models.py`

 * *Files identical despite different names*

### Comparing `dj-whisperer-0.2.8/whisperer/tests/tests.py` & `dj-whisperer-0.2.9/whisperer/tests/tests.py`

 * *Files 9% similar despite different names*

```diff
@@ -30,168 +30,168 @@
 )
 from whisperer.tests.models import Address, Customer, Order
 from whisperer.utils import LockTask
 
 
 class WebhookTestCase(TestCase):
     def setUp(self):
-        self.user = mommy.make(User, username='test_user')
+        self.user = mommy.make(User, username="test_user")
         self.service = WebhookService()
 
     def test_register_webhook(self):
         webhook = mommy.prepare(
             Webhook,
             user=self.user,
-            target_url='http://example.com/order_create',
-            secret_key='secret',
-            event_type='order-created',
-            retry_countdown_config={'choice': 'exponential', 'kwargs': {'base': 2}},
+            target_url="http://example.com/order_create",
+            secret_key="secret",
+            event_type="order-created",
+            retry_countdown_config={"choice": "exponential", "kwargs": {"base": 2}},
         )
 
         serializer = WebhookSerializer(webhook)
         serializer = WebhookSerializer(data=serializer.data)
         self.assertTrue(serializer.is_valid(raise_exception=True))
         webhook = self.service.register_webhook(
             user=self.user, **serializer.validated_data
         )
-        self.assertEqual(webhook.event_type, 'order-created')
+        self.assertEqual(webhook.event_type, "order-created")
 
         with self.assertRaises(WebhookAlreadyRegistered):
             self.service.register_webhook(user=self.user, **serializer.validated_data)
 
     def test_update_webhook(self):
         webhook = mommy.prepare(
             Webhook,
             user=self.user,
-            target_url='http://example2.com/order_create',
-            secret_key='secret',
-            event_type='order-created',
-            retry_countdown_config={'choice': 'exponential', 'kwargs': {'base': 2}},
+            target_url="http://example2.com/order_create",
+            secret_key="secret",
+            event_type="order-created",
+            retry_countdown_config={"choice": "exponential", "kwargs": {"base": 2}},
         )
 
         serializer = WebhookSerializer(webhook)
         serializer = WebhookSerializer(data=serializer.data)
         self.assertTrue(serializer.is_valid(raise_exception=True))
         webhook_created = self.service.register_webhook(
             user=self.user, **serializer.validated_data
         )
 
         update_data = {
-            'target_url': 'http://example3.com/order_update',
-            'event_type': 'order-update',
-            'retry_countdown_config': {
-                'choice': 'linear',
-                'kwargs': {'base': 1 * 60, 'limit': 5 * 60},
+            "target_url": "http://example3.com/order_update",
+            "event_type": "order-update",
+            "retry_countdown_config": {
+                "choice": "linear",
+                "kwargs": {"base": 1 * 60, "limit": 5 * 60},
             },
         }
         webhook_updated = self.service.update_webhook(
             webhook_created, self.user, **update_data
         )
 
         self.assertNotEqual(webhook.target_url, webhook_updated.target_url)
         self.assertNotEqual(webhook.event_type, webhook_updated.event_type)
 
-        self.assertEqual(webhook_updated.target_url, update_data['target_url'])
-        self.assertEqual(webhook_updated.event_type, 'order-update')
+        self.assertEqual(webhook_updated.target_url, update_data["target_url"])
+        self.assertEqual(webhook_updated.event_type, "order-update")
 
     def test_update_webhook_with_already_registered_one(self):
         webhook = mommy.make(
             Webhook,
             user=self.user,
-            target_url='http://example2.com/order_create',
-            secret_key='secret',
-            event_type='order-created',
-            retry_countdown_config={'choice': 'exponential', 'kwargs': {'base': 2}},
+            target_url="http://example2.com/order_create",
+            secret_key="secret",
+            event_type="order-created",
+            retry_countdown_config={"choice": "exponential", "kwargs": {"base": 2}},
         )
 
         mommy.make(
             Webhook,
             user=self.user,
-            target_url='http://example2.com/order_create',
-            secret_key='secret',
-            event_type='order-update',
-            retry_countdown_config={'choice': 'exponential', 'kwargs': {'base': 2}},
+            target_url="http://example2.com/order_create",
+            secret_key="secret",
+            event_type="order-update",
+            retry_countdown_config={"choice": "exponential", "kwargs": {"base": 2}},
         )
 
-        update_data = {'target_url': webhook.target_url, 'event_type': 'order-update'}
+        update_data = {"target_url": webhook.target_url, "event_type": "order-update"}
 
         with self.assertRaises(WebhookAlreadyRegistered):
             self.service.update_webhook(webhook, self.user, **update_data)
 
-        del update_data['target_url']
+        del update_data["target_url"]
 
         with self.assertRaises(WebhookAlreadyRegistered):
             self.service.update_webhook(webhook, self.user, **update_data)
 
         update_data = {
-            'retry_countdown_config': {
-                'choice': 'linear',
-                'kwargs': {'base': 1 * 60, 'limit': 10 * 60},
+            "retry_countdown_config": {
+                "choice": "linear",
+                "kwargs": {"base": 1 * 60, "limit": 10 * 60},
             },
         }
 
         webhook_updated = self.service.update_webhook(webhook, self.user, **update_data)
         self.assertEqual(
-            webhook_updated.retry_countdown_config['kwargs'],
-            update_data['retry_countdown_config']['kwargs'],
+            webhook_updated.retry_countdown_config["kwargs"],
+            update_data["retry_countdown_config"]["kwargs"],
         )
 
     def test_delete_webhook(self):
         webhook = mommy.make(Webhook, is_active=True)
         self.service.delete_webhook(webhook)
         webhook.refresh_from_db()
         self.assertFalse(webhook.is_active)
 
 
 @override_settings(CELERY_ALWAYS_EAGER=True)
 class WhispererEventTestCase(TestCase):
     def setUp(self):
-        self.target_url = 'http://example.com/order_create'
-        self.user = mommy.make(User, username='test_user')
+        self.target_url = "http://example.com/order_create"
+        self.user = mommy.make(User, username="test_user")
 
         self.webhook = mommy.make(
             Webhook,
             user=self.user,
             target_url=self.target_url,
-            secret_key='secret',
-            event_type='order-created',
-            retry_countdown_config={'choice': 'exponential', 'kwargs': {'base': 2}},
+            secret_key="secret",
+            event_type="order-created",
+            retry_countdown_config={"choice": "exponential", "kwargs": {"base": 2}},
         )
-        self.target_url2 = 'http://example.com/auth_order_update'
+        self.target_url2 = "http://example.com/auth_order_update"
         self.webhook2 = mommy.make(
             Webhook,
             user=self.user,
             target_url=self.target_url2,
-            secret_key='secret',
-            event_type='order-updated',
-            retry_countdown_config={'choice': 'exponential', 'kwargs': {'base': 2}},
+            secret_key="secret",
+            event_type="order-updated",
+            retry_countdown_config={"choice": "exponential", "kwargs": {"base": 2}},
             config={
-                'auth': {
-                    'username': 'username',
-                    'password': '123',
-                    'auth_type': 'basic',
+                "auth": {
+                    "username": "username",
+                    "password": "123",
+                    "auth_type": "basic",
                 }
             },
         )
         self.customer = mommy.make(Customer)
         self.address = mommy.make(Address)
         self.order = mommy.prepare(
             Order,
             customer=self.customer,
             address=self.address,
-            number='1',
-            amount='1',
-            discount_amount='1',
-            shipping_amount='1',
+            number="1",
+            amount="1",
+            discount_amount="1",
+            shipping_amount="1",
         )
 
     def test_deliver_event(self):
         with requests_mock.Mocker() as mock:
             mock.register_uri(
-                'POST', self.target_url, text='Order Created', status_code=200
+                "POST", self.target_url, text="Order Created", status_code=200
             )
             self.order.save()
             webhook_events = WebhookEvent.objects.all()
             self.assertEqual(len(webhook_events), 1)
             self.assertTrue(webhook_events[0].delivered)
 
     def test_deliver_event_sync_with_event_uuid(self):
@@ -202,18 +202,18 @@
             request_payload={},
             retry_count=TASK_RETRY_COUNT,
             delivered=False,
             webhook=self.webhook,
         )
         with requests_mock.Mocker() as mock:
             mock.register_uri(
-                'POST', self.webhook.target_url, text='Order Created', status_code=200
+                "POST", self.webhook.target_url, text="Order Created", status_code=200
             )
             deliver_event(
-                self.order, 'order-created', async_=False, event_uuid=webhookevent.uuid
+                self.order, "order-created", async_=False, event_uuid=webhookevent.uuid
             )
             webhookevent.refresh_from_db()
             self.assertTrue(webhookevent.delivered)
 
     def test_deliver_event_async_with_event_uuid(self):
         webhookevent = mommy.make(
             WebhookEvent,
@@ -222,31 +222,31 @@
             request_payload={},
             retry_count=TASK_RETRY_COUNT,
             delivered=False,
             webhook=self.webhook,
         )
         with requests_mock.Mocker() as mock:
             mock.register_uri(
-                'POST', self.webhook.target_url, text='Order Created', status_code=200
+                "POST", self.webhook.target_url, text="Order Created", status_code=200
             )
-            deliver_event(self.order, 'order-created', event_uuid=webhookevent.uuid)
+            deliver_event(self.order, "order-created", event_uuid=webhookevent.uuid)
             webhookevent.refresh_from_db()
             self.assertTrue(webhookevent.delivered)
 
-    @mock.patch('requests.post')
+    @mock.patch("requests.post")
     def test_http_error(self, post_mock):
-        post_mock.side_effect = requests.exceptions.HTTPError('HTTPError')
+        post_mock.side_effect = requests.exceptions.HTTPError("HTTPError")
         self.order.save()
         webhook_events = WebhookEvent.objects.all()
         self.assertEqual(len(webhook_events), 1)
         self.assertFalse(webhook_events[0].delivered)
         self.assertEqual(webhook_events[0].response_http_status, 500)
         self.assertIn("HTTPError", webhook_events[0].response_content)
 
-    @mock.patch('requests.post')
+    @mock.patch("requests.post")
     def test_unboundlocal_error(self, post_mock):
         post_mock.side_effect = UnboundLocalError()
         self.order.save()
         webhook_events = WebhookEvent.objects.all()
         self.assertEqual(len(webhook_events), 1)
         self.assertFalse(webhook_events[0].delivered)
         self.assertEqual(webhook_events[0].response_http_status, 500)
@@ -254,18 +254,18 @@
 
     def test_undelivered_event_scanner(self):
         date1 = timezone.now() - timedelta(days=1)
         date2 = timezone.now() - timedelta(days=4)
         webhook = mommy.make(
             Webhook,
             user=self.user,
-            target_url='http://example.com/order_update',
-            secret_key='secret',
-            event_type='order-created',
-            retry_countdown_config={'choice': 'exponential', 'kwargs': {'base': 2}},
+            target_url="http://example.com/order_update",
+            secret_key="secret",
+            event_type="order-created",
+            retry_countdown_config={"choice": "exponential", "kwargs": {"base": 2}},
         )
         # unsuitable for event scanner query because of  retry limit
         webhookevent1 = mommy.make(
             WebhookEvent,
             modified_date=timezone.now(),
             created_date=timezone.now(),
             request_payload={},
@@ -310,18 +310,18 @@
         WebhookEvent.objects.filter(id=webhookevent5.id).update(
             created_date=timezone.now()
             - timedelta(2 ** (webhookevent5.retry_count + 1))
         )
 
         with requests_mock.Mocker() as mock:
             mock.register_uri(
-                'POST',
-                'http://example.com/order_update',
+                "POST",
+                "http://example.com/order_update",
                 [
-                    {'text': 'Order created', 'status_code': 200},
+                    {"text": "Order created", "status_code": 200},
                 ],
             )
             undelivered_event_scanner()
         webhookevent1.refresh_from_db()
         webhookevent2.refresh_from_db()
         webhookevent3.refresh_from_db()
         webhookevent4.refresh_from_db()
@@ -352,30 +352,30 @@
             retry_count=0,
             delivered=False,
             uuid=uuid.uuid4(),
             webhook=self.webhook,
         )
         with requests_mock.Mocker() as mock:
             mock.register_uri(
-                'POST', self.target_url, [{'text': 'Bad request', 'status_code': 400}]
+                "POST", self.target_url, [{"text": "Bad request", "status_code": 400}]
             )
             mock_method.return_value = False
             deliver_event_task.delay(
                 hook_id=webhookevent1.webhook_id,
                 event_type=self.webhook.event_type,
                 event_uuid=webhookevent1.uuid,
             )
         webhookevent1.refresh_from_db()
         self.assertEqual(webhookevent1.retry_count, TASK_RETRY_COUNT + 1)
         self.assertFalse(webhookevent1.delivered)
 
         # test new event
         with requests_mock.Mocker() as mock:
             mock.register_uri(
-                'POST', self.target_url, [{'text': 'Bad request', 'status_code': 400}]
+                "POST", self.target_url, [{"text": "Bad request", "status_code": 400}]
             )
             self.order.save()
 
         webhookevent2 = WebhookEvent.objects.last()
         self.assertEqual(webhookevent2.retry_count, TASK_RETRY_COUNT + 1)
         self.assertFalse(webhookevent2.delivered)
         self.assertNotEqual(webhookevent2.id, webhookevent1.id)
@@ -385,17 +385,17 @@
                 webhookevent1.id,
                 webhookevent2.id,
             ]
         ).update(created_date=timezone.now() - timedelta(seconds=2 ** 12))
 
         with requests_mock.Mocker() as mock:
             mock.register_uri(
-                'POST',
+                "POST",
                 self.target_url,
-                [{'text': 'Order event received', 'status_code': 200}],
+                [{"text": "Order event received", "status_code": 200}],
             )
             WebhookEvent.objects.filter(
                 id__in=[webhookevent1.id, webhookevent2.id]
             ).update(modified_date=webhookevent1.modified_date - timedelta(days=1))
             undelivered_event_scanner()
 
         webhookevent1.refresh_from_db()
@@ -408,76 +408,76 @@
         self.assertEqual(webhookevent2.response_http_status, 200)
 
     @requests_mock.mock()
     @mock.patch.object(LockTask, "is_exists_cache_key")
     def test_auth_config(self, m, mock_method):
         mock_method.return_value = False
         self.order.save()
-        self.order.number = '123'
+        self.order.number = "123"
         m.register_uri(
-            'POST', self.target_url2, text=self._auth_test_callback, status_code=200
+            "POST", self.target_url2, text=self._auth_test_callback, status_code=200
         )
         self.order.save()
         event = WebhookEvent.objects.filter(webhook=self.webhook2).last()
         self.assertEqual(event.response_http_status, 200)
         self.assertTrue(event.delivered)
 
         self.webhook2.config = {}
         self.webhook2.save()
 
-        self.order.number = '123123'
+        self.order.number = "123123"
         self.order.save()
         event = WebhookEvent.objects.filter(webhook=self.webhook2).last()
         self.assertEqual(event.response_http_status, 401)
         self.assertFalse(event.delivered)
 
     def _auth_test_callback(self, request, context):
-        if 'Authorization' not in request.headers:
+        if "Authorization" not in request.headers:
             context.status_code = 401
-        return ''
+        return ""
 
 
 def dummy_whisperer_event_callback(response, event_type, instance, payload):
-    """ this function creates customer in test database """
+    """this function creates customer in test database"""
     mommy.make(Customer)
 
 
 @override_settings(CELERY_ALWAYS_EAGER=True)
 class WhispererEventCallbackTestCase(TestCase):
     def setUp(self):
-        self.target_url = 'http://example.com/foo_bar'
-        user = mommy.make(User, username='test_user')
+        self.target_url = "http://example.com/foo_bar"
+        user = mommy.make(User, username="test_user")
         mommy.make(
             Webhook,
             user=user,
             target_url=self.target_url,
-            secret_key='secret',
-            event_type='order-created',
-            retry_countdown_config={'choice': 'exponential', 'kwargs': {'base': 2}},
-            callback='whisperer.tests.tests.dummy_whisperer_event_callback',
+            secret_key="secret",
+            event_type="order-created",
+            retry_countdown_config={"choice": "exponential", "kwargs": {"base": 2}},
+            callback="whisperer.tests.tests.dummy_whisperer_event_callback",
         )
         customer = mommy.make(Customer)
         address = mommy.make(Address)
         self.order = mommy.prepare(
             Order,
             customer=customer,
             address=address,
-            number='1',
-            amount='1',
-            discount_amount='1',
-            shipping_amount='1',
+            number="1",
+            amount="1",
+            discount_amount="1",
+            shipping_amount="1",
         )
 
     def tearDown(self):
         Customer.objects.all().delete()
 
     def test_runs_callback(self):
         with requests_mock.Mocker() as mock:
             mock.register_uri(
-                'POST', self.target_url, text='Request Processed', status_code=200
+                "POST", self.target_url, text="Request Processed", status_code=200
             )
 
             # before callback we have one customer
             self.assertEqual(Customer.objects.count(), 1)
             self.order.save()
             webhook_events = WebhookEvent.objects.all()
             self.assertEqual(len(webhook_events), 1)
@@ -525,19 +525,20 @@
         for _ in range(100):
             retry_count = random.randint(1, 100)
             value = countdown.get_value(retry_count)
             self.assertEqual(value, min(retry_count * base, limit))
 
     def test_exponential_retry_countdown(self):
         base = 2
-        countdown = ExponentialRetryCountdown(base=base)
+        factor = 16
+        countdown = ExponentialRetryCountdown(base=base, factor=factor)
         for _ in range(15):
             retry_count = random.randint(1, 12)
             value = countdown.get_value(retry_count)
-            self.assertEqual(value, base ** retry_count)
+            self.assertEqual(value, (base ** retry_count) * factor)
 
         limit = 20 * 60
-        countdown = ExponentialRetryCountdown(base=base, limit=limit)
+        countdown = ExponentialRetryCountdown(base=base, factor=factor, limit=limit)
         for _ in range(15):
             retry_count = random.randint(1, 12)
             value = countdown.get_value(retry_count)
-            self.assertEqual(value, min(base ** retry_count, limit))
+            self.assertEqual(value, min((base ** retry_count) * factor, limit))
```

### Comparing `dj-whisperer-0.2.8/whisperer/tests/webhooks.py` & `dj-whisperer-0.2.9/whisperer/tests/webhooks.py`

 * *Files identical despite different names*

### Comparing `dj-whisperer-0.2.8/whisperer/utils.py` & `dj-whisperer-0.2.9/whisperer/utils.py`

 * *Files identical despite different names*

### Comparing `dj-whisperer-0.2.8/whisperer/validators.py` & `dj-whisperer-0.2.9/whisperer/validators.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,15 @@
         min_value=0, required=False, allow_null=True, write_only=True
     )
 
 
 @countdown_kwargs_serializers.register(key='exponential')
 class ExponentialRetryCountdownKwargsSerializer(serializers.Serializer):
     base = serializers.IntegerField(min_value=0, write_only=True)
+    factor = serializers.IntegerField(min_value=1, default=1, required=False)
     limit = serializers.IntegerField(
         min_value=0, required=False, allow_null=True, write_only=True
     )
 
 
 @countdown_kwargs_serializers.register(key='random')
 class RandomRetryCountdownKwargsSerializer(serializers.Serializer):
```

