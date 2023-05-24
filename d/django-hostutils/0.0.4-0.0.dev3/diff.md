# Comparing `tmp/django-hostutils-0.0.4.tar.gz` & `tmp/django-hostutils-0.0.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-hostutils-0.0.4.tar", last modified: Wed May 24 22:17:32 2023, max compression
+gzip compressed data, was "django-hostutils-0.0.dev3.tar", last modified: Tue Apr 25 00:40:22 2023, max compression
```

## Comparing `django-hostutils-0.0.4.tar` & `django-hostutils-0.0.dev3.tar`

### file list

```diff
@@ -1,48 +1,106 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:17:32.827947 django-hostutils-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-24 22:17:16.000000 django-hostutils-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    44062 2023-05-24 22:17:32.827947 django-hostutils-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-05-24 22:17:16.000000 django-hostutils-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-05-24 22:17:16.000000 django-hostutils-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 22:17:32.827947 django-hostutils-0.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:17:32.827947 django-hostutils-0.0.4/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 22:17:16.000000 django-hostutils-0.0.4/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-24 22:17:32.000000 django-hostutils-0.0.4/src/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:17:32.827947 django-hostutils-0.0.4/src/django_hostutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    44062 2023-05-24 22:17:32.000000 django-hostutils-0.0.4/src/django_hostutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-05-24 22:17:32.000000 django-hostutils-0.0.4/src/django_hostutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 22:17:32.000000 django-hostutils-0.0.4/src/django_hostutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-24 22:17:32.000000 django-hostutils-0.0.4/src/django_hostutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-24 22:17:32.000000 django-hostutils-0.0.4/src/django_hostutils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:17:32.827947 django-hostutils-0.0.4/src/djangoaddicts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 22:17:16.000000 django-hostutils-0.0.4/src/djangoaddicts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:17:32.827947 django-hostutils-0.0.4/src/djangoaddicts/hostutils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 22:17:16.000000 django-hostutils-0.0.4/src/djangoaddicts/hostutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-24 22:17:16.000000 django-hostutils-0.0.4/src/djangoaddicts/hostutils/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-24 22:17:16.000000 django-hostutils-0.0.4/src/djangoaddicts/hostutils/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:17:32.823947 django-hostutils-0.0.4/src/djangoaddicts/hostutils/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:17:32.823947 django-hostutils-0.0.4/src/djangoaddicts/hostutils/templates/hostutils/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:17:32.823947 django-hostutils-0.0.4/src/djangoaddicts/hostutils/templates/hostutils/bs5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:17:32.827947 django-hostutils-0.0.4/src/djangoaddicts/hostutils/templates/hostutils/bs5/ajax/
--rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-05-24 22:17:16.000000 django-hostutils-0.0.4/src/djangoaddicts/hostutils/templates/hostutils/bs5/ajax/get_cpu_stats.htm
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-24 22:17:16.000000 django-hostutils-0.0.4/src/djangoaddicts/hostutils/templates/hostutils/bs5/ajax/get_interface_stats.htm
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-05-24 22:17:16.000000 django-hostutils-0.0.4/src/djangoaddicts/hostutils/templates/hostutils/bs5/ajax/get_partition_stats.htm
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-05-24 22:17:16.000000 django-hostutils-0.0.4/src/djangoaddicts/hostutils/templates/hostutils/bs5/ajax/get_process_stats.htm
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:17:32.827947 django-hostutils-0.0.4/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/
--rw-r--r--   0 runner    (1001) docker     (123)     6894 2023-05-24 22:17:16.000000 django-hostutils-0.0.4/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/cpu.html
--rw-r--r--   0 runner    (1001) docker     (123)    11588 2023-05-24 22:17:16.000000 django-hostutils-0.0.4/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/detail_host.html
--rw-r--r--   0 runner    (1001) docker     (123)     8529 2023-05-24 22:17:16.000000 django-hostutils-0.0.4/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/disk.html
--rw-r--r--   0 runner    (1001) docker     (123)    11180 2023-05-24 22:17:16.000000 django-hostutils-0.0.4/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/memory.html
--rw-r--r--   0 runner    (1001) docker     (123)     8919 2023-05-24 22:17:16.000000 django-hostutils-0.0.4/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/network.html
--rw-r--r--   0 runner    (1001) docker     (123)     5696 2023-05-24 22:17:16.000000 django-hostutils-0.0.4/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/processes.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:17:32.827947 django-hostutils-0.0.4/src/djangoaddicts/hostutils/templates/hostutils/bs5/snippets/
--rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-05-24 22:17:16.000000 django-hostutils-0.0.4/src/djangoaddicts/hostutils/templates/hostutils/bs5/snippets/host_process_card.htm
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-24 22:17:16.000000 django-hostutils-0.0.4/src/djangoaddicts/hostutils/templates/hostutils/bs5/snippets/host_process_card_swap.htm
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-05-24 22:17:16.000000 django-hostutils-0.0.4/src/djangoaddicts/hostutils/templates/hostutils/bs5/snippets/hostutils_nav_menu.htm
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-24 22:17:16.000000 django-hostutils-0.0.4/src/djangoaddicts/hostutils/templates/hostutils/bs5/snippets/processes_results_timestamp.htm
--rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-05-24 22:17:16.000000 django-hostutils-0.0.4/src/djangoaddicts/hostutils/templates/hostutils/bs5/snippets/processes_title_cards.htm
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-24 22:17:16.000000 django-hostutils-0.0.4/src/djangoaddicts/hostutils/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:17:32.827947 django-hostutils-0.0.4/src/djangoaddicts/hostutils/views/
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-24 22:17:16.000000 django-hostutils-0.0.4/src/djangoaddicts/hostutils/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-05-24 22:17:16.000000 django-hostutils-0.0.4/src/djangoaddicts/hostutils/views/ajax.py
--rw-r--r--   0 runner    (1001) docker     (123)     6545 2023-05-24 22:17:16.000000 django-hostutils-0.0.4/src/djangoaddicts/hostutils/views/gui.py
--rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-05-24 22:17:16.000000 django-hostutils-0.0.4/src/djangoaddicts/hostutils/views/htmx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.513207 django-hostutils-0.0.dev3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.505207 django-hostutils-0.0.dev3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.505207 django-hostutils-0.0.dev3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/.github/workflows/bandit.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/.github/workflows/black.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/.github/workflows/mypy.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/.github/workflows/pylint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/.github/workflows/pytest.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-04-25 00:40:22.513207 django-hostutils-0.0.dev3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.505207 django-hostutils-0.0.dev3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/django_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.505207 django-hostutils-0.0.dev3/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.509207 django-hostutils-0.0.dev3/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)   133744 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/source/_static/cpu.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)   131317 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/source/_static/cpu.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   124420 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/source/_static/disk.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   161082 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/source/_static/host.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   100187 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/source/_static/memory.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   154714 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/source/_static/network.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   122738 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/source/_static/process.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/source/about.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/source/features.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.509207 django-hostutils-0.0.dev3/docs/source/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   131317 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/source/images/cpu.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   124420 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/source/images/disk.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   161082 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/source/images/host.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   100187 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/source/images/memory.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   154714 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/source/images/network.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   122738 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/source/images/process.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/source/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/source/internals.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/source/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/source/version_history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-04-25 00:40:22.513207 django-hostutils-0.0.dev3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.509207 django-hostutils-0.0.dev3/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.509207 django-hostutils-0.0.dev3/src/django_hostutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-04-25 00:40:22.000000 django-hostutils-0.0.dev3/src/django_hostutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-04-25 00:40:22.000000 django-hostutils-0.0.dev3/src/django_hostutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 00:40:22.000000 django-hostutils-0.0.dev3/src/django_hostutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-25 00:40:22.000000 django-hostutils-0.0.dev3/src/django_hostutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-25 00:40:22.000000 django-hostutils-0.0.dev3/src/django_hostutils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 00:40:22.000000 django-hostutils-0.0.dev3/src/django_hostutils.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.509207 django-hostutils-0.0.dev3/src/djangoaddicts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.509207 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.505207 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.505207 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.505207 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.509207 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/ajax/
+-rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/ajax/get_cpu_stats.htm
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/ajax/get_interface_stats.htm
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/ajax/get_partition_stats.htm
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/ajax/get_process_stats.htm
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.509207 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/
+-rw-r--r--   0 runner    (1001) docker     (123)     6894 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/cpu.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11588 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/detail_host.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8529 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/disk.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11180 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/memory.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8919 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/network.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5696 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/processes.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.509207 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/snippets/
+-rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/snippets/host_process_card.htm
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/snippets/host_process_card_swap.htm
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/snippets/hostutils_nav_menu.htm
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/snippets/processes_results_timestamp.htm
+-rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/snippets/processes_title_cards.htm
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.513207 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/views/
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/views/ajax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6407 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/views/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/views/htmx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.505207 django-hostutils-0.0.dev3/src/djangoaddicts/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.505207 django-hostutils-0.0.dev3/src/djangoaddicts/templates/hostutils/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.505207 django-hostutils-0.0.dev3/src/djangoaddicts/templates/hostutils/bs5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.513207 django-hostutils-0.0.dev3/src/djangoaddicts/templates/hostutils/bs5/ajax/
+-rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/templates/hostutils/bs5/ajax/host_cpu_stats.htm
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/templates/hostutils/bs5/ajax/host_interface_stats.htm
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/templates/hostutils/bs5/ajax/host_partition_usage.htm
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/templates/hostutils/bs5/ajax/host_process_details.htm
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.513207 django-hostutils-0.0.dev3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.513207 django-hostutils-0.0.dev3/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/tests/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/tests/core/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/tests/core/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.513207 django-hostutils-0.0.dev3/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/tests/unit/test_ajax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/tests/unit/test_gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/tests/unit/test_htmx.py
```

### Comparing `django-hostutils-0.0.4/LICENSE` & `django-hostutils-0.0.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `django-hostutils-0.0.4/README.md` & `django-hostutils-0.0.dev3/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -14,40 +14,27 @@
 |--------------|------|
 | Author       | David Slusser |
 | Description  | Host utilities package for django projects. |
 | Requirements | `Python 3.x` +<br>`Django 3.2.x` + |
 
 <br/>
 
-## Code Quality
+## Code Quality Checks
 | Workflow | Description             | Status                                                                       |
 |----------|-------------------------|------------------------------------------------------------------------------|
 |Bandit|security checks|![Bandit](https://github.com/davidslusser/workflow_tests/actions/workflows/bandit.yaml/badge.svg)|
 |Black|code formatting|![Black](https://github.com/davidslusser/workflow_tests/actions/workflows/black.yaml/badge.svg)|
 |Mypy|static type checking|![Mypy](https://github.com/davidslusser/workflow_tests/actions/workflows/mypy.yaml/badge.svg)|
 |Pylint|static code analysis|![Pylint](https://github.com/davidslusser/workflow_tests/actions/workflows/pylint.yaml/badge.svg)|
 |Pytest|unit testing|![Pytest](https://github.com/davidslusser/workflow_tests/actions/workflows/pytest.yaml/badge.svg)|
 
 <br/>
 
-## Documentation
-| Workflow | Description             | Status                                                                       |
-|----------|-------------------------|------------------------------------------------------------------------------|
-|Docs|ReadTheDocs Build|[![Documentation Status](https://readthedocs.org/projects/django-hostutils/badge/?version=latest)](https://django-hostutils.readthedocs.io/en/latest/?badge=latest)|
-
-Full documentation is available here:
-
-https://django-hostutils.readthedocs.io/en/latest/index.html 
-
-<br/>
-
 ## License
-django-hostutils is licensed under the GNU-3 license (see the LICENSE file for details).
-
-https://github.com/davidslusser/django-hostutils/blob/docs/LICENSE 
+django-userextensions is licensed under the GNU-3 license (see the LICENSE file for details).
 
 <br/>
 
 ## Installation 
 - pip install django-hostutils
 - add the following to your INSTALLED_APPS
 
@@ -56,24 +43,22 @@
     ```
 - add the following to your project-level urls.py:
    
    ```python
    path("hostutils/", include("djangoaddicts.hostutils.urls"), ),
    ```
 
-<br/>
-
 ## Usage
 Several pages are available. If you have a Bootstrap 5 nav-menu you can add the following snippet in your navbar where appropriate:
 
-```
-{% include 'hostutils/bs5/snippets/hostutils_nav_menu.htm' %}
-```
+    ```
+    {% include 'hostutils/bs5/snippets/hostutils_nav_menu.htm' %}
+    ```
 
-Individual pages can also be linked directly:
+Alternatively, individual pages can linked directly:
 
 - Host overview page: 
 
     ```
     {% url 'hostutils:host_details' %}
     ```
```

### Comparing `django-hostutils-0.0.4/src/djangoaddicts/hostutils/forms.py` & `django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/forms.py`

 * *Files identical despite different names*

### Comparing `django-hostutils-0.0.4/src/djangoaddicts/hostutils/templates/hostutils/bs5/ajax/get_cpu_stats.htm` & `django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/ajax/get_cpu_stats.htm`

 * *Files identical despite different names*

### Comparing `django-hostutils-0.0.4/src/djangoaddicts/hostutils/templates/hostutils/bs5/ajax/get_interface_stats.htm` & `django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/ajax/get_interface_stats.htm`

 * *Files identical despite different names*

### Comparing `django-hostutils-0.0.4/src/djangoaddicts/hostutils/templates/hostutils/bs5/ajax/get_partition_stats.htm` & `django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/ajax/get_partition_stats.htm`

 * *Files identical despite different names*

### Comparing `django-hostutils-0.0.4/src/djangoaddicts/hostutils/templates/hostutils/bs5/ajax/get_process_stats.htm` & `django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/ajax/get_process_stats.htm`

 * *Files identical despite different names*

### Comparing `django-hostutils-0.0.4/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/cpu.html` & `django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/cpu.html`

 * *Files identical despite different names*

### Comparing `django-hostutils-0.0.4/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/detail_host.html` & `django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/detail_host.html`

 * *Files identical despite different names*

### Comparing `django-hostutils-0.0.4/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/disk.html` & `django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/disk.html`

 * *Files identical despite different names*

### Comparing `django-hostutils-0.0.4/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/memory.html` & `django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/memory.html`

 * *Files identical despite different names*

### Comparing `django-hostutils-0.0.4/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/network.html` & `django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/network.html`

 * *Files identical despite different names*

### Comparing `django-hostutils-0.0.4/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/processes.html` & `django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/processes.html`

 * *Files identical despite different names*

### Comparing `django-hostutils-0.0.4/src/djangoaddicts/hostutils/templates/hostutils/bs5/snippets/host_process_card.htm` & `django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/snippets/host_process_card.htm`

 * *Files identical despite different names*

### Comparing `django-hostutils-0.0.4/src/djangoaddicts/hostutils/templates/hostutils/bs5/snippets/hostutils_nav_menu.htm` & `django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/snippets/hostutils_nav_menu.htm`

 * *Files identical despite different names*

### Comparing `django-hostutils-0.0.4/src/djangoaddicts/hostutils/templates/hostutils/bs5/snippets/processes_title_cards.htm` & `django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/snippets/processes_title_cards.htm`

 * *Files identical despite different names*

### Comparing `django-hostutils-0.0.4/src/djangoaddicts/hostutils/urls.py` & `django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/urls.py`

 * *Files identical despite different names*

### Comparing `django-hostutils-0.0.4/src/djangoaddicts/hostutils/views/__init__.py` & `django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/views/__init__.py`

 * *Files identical despite different names*

### Comparing `django-hostutils-0.0.4/src/djangoaddicts/hostutils/views/ajax.py` & `django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/views/ajax.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-from typing import Union
+import psutil
 
 from django.http import HttpResponse
 from django.template import loader
 
 from handyhelpers.views.ajax import AjaxGetView
-
-import psutil
+from typing import Union
 
 
 class GetHostCpuStats(AjaxGetView):
     """
     Description:
         Get CPU status for a given cpu on the host machine.
     Args:
@@ -84,15 +83,15 @@
     Returns:
         HttpResponse: JSON formatted response.
     """
 
     template = loader.get_template("hostutils/bs5/ajax/get_process_stats.htm")
 
     def get(self, request, *args, **kwargs) -> HttpResponse:
-        self.data: Union[dict, psutil.Process]
+        self.data: Union[dict, psutil.Process] 
         try:
             proc = request.GET["client_response"]
             self.data = psutil.Process(int(proc))
         except psutil.AccessDenied:
             self.data = {}
         except Exception:
             return HttpResponse("Invalid request inputs", status=400)
```

### Comparing `django-hostutils-0.0.4/src/djangoaddicts/hostutils/views/gui.py` & `django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/views/gui.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,21 +9,20 @@
 from djangoaddicts.hostutils.forms import HostProcessFilterForm
 
 
 class ShowHost(View):
     """Display dashboard like page showing an overview of host data"""
 
     template_name = "hostutils/bs5/detail/detail_host.html"
-    title = "Host Dashboard"
 
     def get(self, request, *args, **kwargs):
         """allow get method"""
         now = datetime.datetime.now()
         context = {}
-        context["title"] = self.title
+        context["title"] = "Host Dashboard"
         context["subtitle"] = psutil.os.uname()[1]
         context["cpu_count"] = psutil.cpu_count(logical=False)
         context["memory"] = psutil.virtual_memory()
         context["disk_usage"] = psutil.disk_usage("/")
         context["disk_io_counters"] = psutil.disk_io_counters()
         context["network"] = psutil.net_connections()
         context["pids"] = psutil.pids()
@@ -37,128 +36,123 @@
         )
 
         context["platform"] = psutil.os.uname()
 
         return render(request, self.template_name, context=context)
 
 
-class ShowHostCpu(View):
-    """Display dashboard like page showing host cpu data"""
+class ShowHostProcesses(View):
+    """Display dashboard like page showing host process data"""
 
-    template_name = "hostutils/bs5/detail/cpu.html"
-    title = "CPU Dashboard"
+    template_name = "hostutils/bs5/detail/processes.html"
 
     def get(self, request, *args, **kwargs):
-        """CPU Dashboard"""
+        """allow get method"""
         context = {}
-        context["title"] = self.title
+        context["title"] = "Host Processes"
+        context["now"] = datetime.datetime.now()
         context["subtitle"] = psutil.os.uname()[1]
-        context["stats"] = psutil.cpu_stats()
-        context["physical_count"] = psutil.cpu_count(logical=False)
-        context["logical_count"] = psutil.cpu_count(logical=True)
-        context["percent"] = psutil.cpu_percent(interval=None)
-        context["times_list"] = psutil.cpu_times(percpu=True)
-        context["times_percent_list"] = psutil.cpu_times_percent(percpu=True)
-        context["percent_list"] = psutil.cpu_percent(interval=None, percpu=True)
-        context["frequency_list"] = psutil.cpu_freq(percpu=True)
-        context["cpu_range"] = list(range(psutil.cpu_count(logical=True)))
-        cpu_data = {}
-        for i in range(context["logical_count"]):
-            cpu_data[i] = {
-                "times": context["times_list"][i],
-                "time_percent": context["times_percent_list"][i],
-                "percent": context["percent_list"][i],
-                "frequency": context["frequency_list"][i],
-            }
-        context["cpu_data"] = cpu_data
-        context["load_avg_1"], context["load_avg_5"], context["load_avg_15"] = [
-            round(x / psutil.cpu_count() * 100, 2) for x in psutil.getloadavg()
-        ]
+        process_list = list(psutil.process_iter())
+        context["process_list"] = process_list
+        counts = {
+            "running": len([i for i in process_list if i.status() == "running"]),
+            "sleeping": len([i for i in process_list if i.status() == "sleeping"]),
+            "idle": len([i for i in process_list if i.status() == "idle"]),
+            "stopped": len([i for i in process_list if i.status() == "stopped"]),
+            "zombie": len([i for i in process_list if i.status() == "zombie"]),
+            "dead": len([i for i in process_list if i.status() == "dead"]),
+        }
+        context["counts"] = counts
+        filter_form = {}
+        filter_form["form"] = HostProcessFilterForm(request.GET or None)
+        filter_form["modal_name"] = "filter_processes"
+        filter_form["modal_size"] = "modal-lg"
+        filter_form["modal_title"] = "Filter Host Processes"
+        filter_form["hx_method"] = "hx-get"
+        filter_form["hx_url"] = "/hostutils/get_host_processes"
+        filter_form["hx_target"] = "id_process_list_container"
+        filter_form["method"] = "GET"
+        filter_form["action"] = "Filter"
+        context["filter_form"] = filter_form
+        return render(request, self.template_name, context=context)
+
+
+class ShowHostNetwork(View):
+    """Display dashboard like page showing host network data"""
+
+    template_name = "hostutils/bs5/detail/network.html"
+
+    def get(self, request, *args, **kwargs):
+        """allow get method"""
+        context = {}
+        context["title"] = "Network Dashboard"
+        context["subtitle"] = psutil.os.uname()[1]
+        context["connection_list"] = psutil.net_connections()
+        context["interface_list"] = psutil.net_if_addrs()
+        context["stats_list"] = psutil.net_if_stats()
+        context["counters"] = psutil.net_io_counters()
         return render(request, self.template_name, context=context)
 
 
 class ShowHostDisk(View):
     """Display dashboard like page showing host disk data"""
 
     template_name = "hostutils/bs5/detail/disk.html"
-    title = "Disk Dashboard"
 
     def get(self, request, *args, **kwargs):
         """allow get method"""
         context = {}
-        context["title"] = self.title
+        context["title"] = "Disk Dashboard"
         context["subtitle"] = psutil.os.uname()[1]
         context["usage"] = psutil.disk_usage("/")
         context["io_counters"] = psutil.disk_io_counters()
         context["partition_lists"] = psutil.disk_partitions()
         return render(request, self.template_name, context=context)
 
 
 class ShowHostMemory(View):
     """Display dashboard like page showing host memory data"""
 
     template_name = "hostutils/bs5/detail/memory.html"
-    title = "Memory Dashboard"
 
     def get(self, request, *args, **kwargs):
         """allow get method"""
         context = {}
-        context["title"] = self.title
+        context["title"] = "Memory Dashboard"
         context["subtitle"] = psutil.os.uname()[1]
         context["virtual"] = psutil.virtual_memory()
         context["swap"] = psutil.swap_memory()
         return render(request, self.template_name, context=context)
 
 
-class ShowHostNetwork(View):
-    """Display dashboard like page showing host network data"""
-
-    template_name = "hostutils/bs5/detail/network.html"
-    title = "Network Dashboard"
-
-    def get(self, request, *args, **kwargs):
-        """allow get method"""
-        context = {}
-        context["title"] = self.title
-        context["subtitle"] = psutil.os.uname()[1]
-        context["connection_list"] = psutil.net_connections()
-        context["interface_list"] = psutil.net_if_addrs()
-        context["stats_list"] = psutil.net_if_stats()
-        context["counters"] = psutil.net_io_counters()
-        return render(request, self.template_name, context=context)
-
-
-class ShowHostProcesses(View):
-    """Display dashboard like page showing host process data"""
+class ShowHostCpu(View):
+    """Display dashboard like page showing host cpu data"""
 
-    template_name = "hostutils/bs5/detail/processes.html"
-    title = "Process Dashboard"
+    template_name = "hostutils/bs5/detail/cpu.html"
 
     def get(self, request, *args, **kwargs):
         """allow get method"""
         context = {}
-        context["title"] = self.title
-        context["now"] = datetime.datetime.now()
+        context["title"] = "CPU Dashboard"
         context["subtitle"] = psutil.os.uname()[1]
-        process_list = list(psutil.process_iter())
-        context["process_list"] = process_list
-        counts = {
-            "running": len([i for i in process_list if i.status() == "running"]),
-            "sleeping": len([i for i in process_list if i.status() == "sleeping"]),
-            "idle": len([i for i in process_list if i.status() == "idle"]),
-            "stopped": len([i for i in process_list if i.status() == "stopped"]),
-            "zombie": len([i for i in process_list if i.status() == "zombie"]),
-            "dead": len([i for i in process_list if i.status() == "dead"]),
-        }
-        context["counts"] = counts
-        filter_form = {}
-        filter_form["form"] = HostProcessFilterForm(request.GET or None)
-        filter_form["modal_name"] = "filter_processes"
-        filter_form["modal_size"] = "modal-lg"
-        filter_form["modal_title"] = "Filter Host Processes"
-        filter_form["hx_method"] = "hx-get"
-        filter_form["hx_url"] = "/hostutils/get_host_processes"
-        filter_form["hx_target"] = "id_process_list_container"
-        filter_form["method"] = "GET"
-        filter_form["action"] = "Filter"
-        context["filter_form"] = filter_form
+        context["stats"] = psutil.cpu_stats()
+        context["physical_count"] = psutil.cpu_count(logical=False)
+        context["logical_count"] = psutil.cpu_count(logical=True)
+        context["percent"] = psutil.cpu_percent(interval=None)
+        context["times_list"] = psutil.cpu_times(percpu=True)
+        context["times_percent_list"] = psutil.cpu_times_percent(percpu=True)
+        context["percent_list"] = psutil.cpu_percent(interval=None, percpu=True)
+        context["frequency_list"] = psutil.cpu_freq(percpu=True)
+        context["cpu_range"] = list(range(psutil.cpu_count(logical=True)))
+        cpu_data = {}
+        for i in range(context["logical_count"]):
+            cpu_data[i] = {
+                "times": context["times_list"][i],
+                "time_percent": context["times_percent_list"][i],
+                "percent": context["percent_list"][i],
+                "frequency": context["frequency_list"][i],
+            }
+        context["cpu_data"] = cpu_data
+        context["load_avg_1"], context["load_avg_5"], context["load_avg_15"] = [
+            round(x / psutil.cpu_count() * 100, 2) for x in psutil.getloadavg()
+        ]
         return render(request, self.template_name, context=context)
```

### Comparing `django-hostutils-0.0.4/src/djangoaddicts/hostutils/views/htmx.py` & `django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/views/htmx.py`

 * *Files identical despite different names*

