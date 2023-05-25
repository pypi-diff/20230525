# Comparing `tmp/mkdocs-macros-plugin-0.7.0.tar.gz` & `tmp/mkdocs-macros-plugin-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-macros-plugin-0.7.0.tar", last modified: Mon Mar 28 12:44:10 2022, max compression
+gzip compressed data, was "mkdocs-macros-plugin-1.0.1.tar", last modified: Thu May 25 12:11:51 2023, max compression
```

## Comparing `mkdocs-macros-plugin-0.7.0.tar` & `mkdocs-macros-plugin-1.0.1.tar`

### file list

```diff
@@ -1,82 +1,95 @@
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2022-03-28 12:44:10.000000 mkdocs-macros-plugin-0.7.0/
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2022-03-28 12:44:09.000000 mkdocs-macros-plugin-0.7.0/.github/
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2022-03-28 12:44:09.000000 mkdocs-macros-plugin-0.7.0/.github/workflows/
--rw-r--r--   0 laurent    (501) staff       (20)      457 2020-03-10 06:37:22.000000 mkdocs-macros-plugin-0.7.0/.github/workflows/greetings.yml
--rw-rw-r--   0 laurent    (501) staff       (20)      365 2021-04-19 13:38:15.000000 mkdocs-macros-plugin-0.7.0/.gitignore
--rw-r--r--   0 laurent    (501) staff       (20)      601 2021-04-23 13:52:57.000000 mkdocs-macros-plugin-0.7.0/.readthedocs.yml
--rw-r--r--   0 laurent    (501) staff       (20)     3318 2022-03-25 20:04:56.000000 mkdocs-macros-plugin-0.7.0/CHANGELOG.md
--rw-r--r--   0 laurent    (501) staff       (20)     1134 2021-11-23 01:28:45.000000 mkdocs-macros-plugin-0.7.0/LICENSE.md
--rw-r--r--   0 laurent    (501) staff       (20)       64 2020-11-22 09:50:49.000000 mkdocs-macros-plugin-0.7.0/MANIFEST.in
--rw-r--r--   0 laurent    (501) staff       (20)     7486 2022-03-28 12:44:10.000000 mkdocs-macros-plugin-0.7.0/PKG-INFO
--rw-r--r--   0 laurent    (501) staff       (20)     6697 2022-01-26 01:35:47.000000 mkdocs-macros-plugin-0.7.0/README.md
--rw-r--r--   0 laurent    (501) staff       (20)   249520 2020-02-24 19:02:56.000000 mkdocs-macros-plugin-0.7.0/macros_info.png
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2022-03-28 12:44:10.000000 mkdocs-macros-plugin-0.7.0/mkdocs_macros/
--rw-rw-r--   0 laurent    (501) staff       (20)      234 2021-01-04 17:04:12.000000 mkdocs-macros-plugin-0.7.0/mkdocs_macros/__init__.py
--rw-r--r--   0 laurent    (501) staff       (20)    11897 2022-01-25 21:53:40.000000 mkdocs-macros-plugin-0.7.0/mkdocs_macros/context.py
--rw-r--r--   0 laurent    (501) staff       (20)     1596 2022-03-12 15:07:16.000000 mkdocs-macros-plugin-0.7.0/mkdocs_macros/macros_info.md
--rw-r--r--   0 laurent    (501) staff       (20)    25914 2022-03-16 08:04:21.000000 mkdocs-macros-plugin-0.7.0/mkdocs_macros/plugin.py
--rwxr-xr-x   0 laurent    (501) staff       (20)     6562 2022-03-16 08:10:30.000000 mkdocs-macros-plugin-0.7.0/mkdocs_macros/util.py
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2022-03-28 12:44:10.000000 mkdocs-macros-plugin-0.7.0/mkdocs_macros_plugin.egg-info/
--rw-r--r--   0 laurent    (501) staff       (20)     7486 2022-03-28 12:44:07.000000 mkdocs-macros-plugin-0.7.0/mkdocs_macros_plugin.egg-info/PKG-INFO
--rw-r--r--   0 laurent    (501) staff       (20)     1504 2022-03-28 12:44:09.000000 mkdocs-macros-plugin-0.7.0/mkdocs_macros_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 laurent    (501) staff       (20)        1 2022-03-28 12:44:07.000000 mkdocs-macros-plugin-0.7.0/mkdocs_macros_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 laurent    (501) staff       (20)       61 2022-03-28 12:44:07.000000 mkdocs-macros-plugin-0.7.0/mkdocs_macros_plugin.egg-info/entry_points.txt
--rw-r--r--   0 laurent    (501) staff       (20)      132 2022-03-28 12:44:07.000000 mkdocs-macros-plugin-0.7.0/mkdocs_macros_plugin.egg-info/requires.txt
--rw-r--r--   0 laurent    (501) staff       (20)       14 2022-03-28 12:44:07.000000 mkdocs-macros-plugin-0.7.0/mkdocs_macros_plugin.egg-info/top_level.txt
--rw-r--r--   0 laurent    (501) staff       (20)       38 2022-03-28 12:44:10.000000 mkdocs-macros-plugin-0.7.0/setup.cfg
--rw-r--r--   0 laurent    (501) staff       (20)     1923 2022-03-25 19:56:29.000000 mkdocs-macros-plugin-0.7.0/setup.py
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2022-03-28 12:44:10.000000 mkdocs-macros-plugin-0.7.0/test/
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2022-03-28 12:44:10.000000 mkdocs-macros-plugin-0.7.0/test/debug/
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2022-03-28 12:44:10.000000 mkdocs-macros-plugin-0.7.0/test/debug/docs/
--rw-r--r--   0 laurent    (501) staff       (20)      129 2022-03-12 15:07:17.000000 mkdocs-macros-plugin-0.7.0/test/debug/docs/index.md
--rw-r--r--   0 laurent    (501) staff       (20)      223 2022-03-12 15:07:17.000000 mkdocs-macros-plugin-0.7.0/test/debug/mkdocs.yml
--rw-rw-r--   0 laurent    (501) staff       (20)     1277 2020-02-23 06:57:46.000000 mkdocs-macros-plugin-0.7.0/test/main_sample.py
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2022-03-28 12:44:10.000000 mkdocs-macros-plugin-0.7.0/test/module/
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2022-03-28 12:44:10.000000 mkdocs-macros-plugin-0.7.0/test/module/docs/
--rw-r--r--   0 laurent    (501) staff       (20)      346 2022-03-25 19:56:02.000000 mkdocs-macros-plugin-0.7.0/test/module/docs/environment.md
--rw-r--r--   0 laurent    (501) staff       (20)     2372 2022-03-16 08:05:31.000000 mkdocs-macros-plugin-0.7.0/test/module/docs/index.md
--rw-r--r--   0 laurent    (501) staff       (20)      357 2021-04-21 16:34:52.000000 mkdocs-macros-plugin-0.7.0/test/module/docs/literal.md
--rw-r--r--   0 laurent    (501) staff       (20)      128 2020-05-15 07:15:24.000000 mkdocs-macros-plugin-0.7.0/test/module/docs/other.md
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2022-03-28 12:44:10.000000 mkdocs-macros-plugin-0.7.0/test/module/include/
--rw-r--r--   0 laurent    (501) staff       (20)       68 2021-06-19 05:35:28.000000 mkdocs-macros-plugin-0.7.0/test/module/include/foo.md
--rw-r--r--   0 laurent    (501) staff       (20)     1867 2021-11-22 22:54:09.000000 mkdocs-macros-plugin-0.7.0/test/module/main.py
--rw-r--r--   0 laurent    (501) staff       (20)      498 2022-03-25 19:55:51.000000 mkdocs-macros-plugin-0.7.0/test/module/mkdocs.yml
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2022-03-28 12:44:10.000000 mkdocs-macros-plugin-0.7.0/test/module_dir/
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2022-03-28 12:44:10.000000 mkdocs-macros-plugin-0.7.0/test/module_dir/docs/
--rw-r--r--   0 laurent    (501) staff       (20)      237 2022-03-25 19:54:47.000000 mkdocs-macros-plugin-0.7.0/test/module_dir/docs/environment.md
--rw-r--r--   0 laurent    (501) staff       (20)      529 2020-09-25 16:29:39.000000 mkdocs-macros-plugin-0.7.0/test/module_dir/docs/index.md
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2022-03-28 12:44:10.000000 mkdocs-macros-plugin-0.7.0/test/module_dir/include/
--rw-r--r--   0 laurent    (501) staff       (20)       68 2020-03-02 21:15:58.000000 mkdocs-macros-plugin-0.7.0/test/module_dir/include/foo.md
--rw-r--r--   0 laurent    (501) staff       (20)      281 2020-09-25 16:31:43.000000 mkdocs-macros-plugin-0.7.0/test/module_dir/mkdocs.yml
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2022-03-28 12:44:10.000000 mkdocs-macros-plugin-0.7.0/test/module_dir/mymodule/
--rw-r--r--   0 laurent    (501) staff       (20)      685 2021-06-19 08:12:07.000000 mkdocs-macros-plugin-0.7.0/test/module_dir/mymodule/__init__.py
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2022-03-28 12:44:10.000000 mkdocs-macros-plugin-0.7.0/test/new_syntax/
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2022-03-28 12:44:10.000000 mkdocs-macros-plugin-0.7.0/test/new_syntax/docs/
--rw-r--r--   0 laurent    (501) staff       (20)      160 2020-09-28 06:50:54.000000 mkdocs-macros-plugin-0.7.0/test/new_syntax/docs/index.md
--rw-r--r--   0 laurent    (501) staff       (20)      138 2020-03-22 11:26:31.000000 mkdocs-macros-plugin-0.7.0/test/new_syntax/main.py
--rw-r--r--   0 laurent    (501) staff       (20)      336 2020-09-28 06:42:49.000000 mkdocs-macros-plugin-0.7.0/test/new_syntax/mkdocs.yml
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2022-03-28 12:44:10.000000 mkdocs-macros-plugin-0.7.0/test/simple/
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2022-03-28 12:44:10.000000 mkdocs-macros-plugin-0.7.0/test/simple/docs/
--rw-r--r--   0 laurent    (501) staff       (20)       21 2020-03-04 11:55:35.000000 mkdocs-macros-plugin-0.7.0/test/simple/docs/index.md
--rw-r--r--   0 laurent    (501) staff       (20)      138 2020-09-15 20:07:40.000000 mkdocs-macros-plugin-0.7.0/test/simple/main_old.py
--rw-r--r--   0 laurent    (501) staff       (20)       92 2020-02-24 18:30:04.000000 mkdocs-macros-plugin-0.7.0/test/simple/mkdocs.yml
--rwxr-xr-x   0 laurent    (501) staff       (20)     1119 2020-10-03 09:23:32.000000 mkdocs-macros-plugin-0.7.0/update_pypi.sh
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2022-03-28 12:44:10.000000 mkdocs-macros-plugin-0.7.0/webdoc/
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2022-03-28 12:44:10.000000 mkdocs-macros-plugin-0.7.0/webdoc/docs/
--rw-r--r--   0 laurent    (501) staff       (20)    27391 2022-03-25 19:52:04.000000 mkdocs-macros-plugin-0.7.0/webdoc/docs/advanced.md
--rw-r--r--   0 laurent    (501) staff       (20)       50 2021-04-23 09:53:10.000000 mkdocs-macros-plugin-0.7.0/webdoc/docs/changelog.md
--rw-r--r--   0 laurent    (501) staff       (20)     2338 2021-04-24 11:27:05.000000 mkdocs-macros-plugin-0.7.0/webdoc/docs/contribute.md
--rw-r--r--   0 laurent    (501) staff       (20)    23462 2020-05-15 08:53:26.000000 mkdocs-macros-plugin-0.7.0/webdoc/docs/dog-eating.jpg
--rw-r--r--   0 laurent    (501) staff       (20)     3998 2022-01-26 01:22:27.000000 mkdocs-macros-plugin-0.7.0/webdoc/docs/git_info.md
--rw-r--r--   0 laurent    (501) staff       (20)      960 2021-11-23 01:28:45.000000 mkdocs-macros-plugin-0.7.0/webdoc/docs/help.md
--rw-r--r--   0 laurent    (501) staff       (20)     8195 2022-01-26 01:35:47.000000 mkdocs-macros-plugin-0.7.0/webdoc/docs/index.md
--rw-r--r--   0 laurent    (501) staff       (20)     1081 2020-03-10 08:29:58.000000 mkdocs-macros-plugin-0.7.0/webdoc/docs/license.md
--rw-r--r--   0 laurent    (501) staff       (20)    15354 2022-03-12 15:05:56.000000 mkdocs-macros-plugin-0.7.0/webdoc/docs/macros.md
--rw-r--r--   0 laurent    (501) staff       (20)   249520 2020-03-10 08:57:11.000000 mkdocs-macros-plugin-0.7.0/webdoc/docs/macros_info.png
--rw-r--r--   0 laurent    (501) staff       (20)     6725 2022-01-26 01:35:47.000000 mkdocs-macros-plugin-0.7.0/webdoc/docs/pages.md
--rw-r--r--   0 laurent    (501) staff       (20)     5693 2021-09-09 06:43:39.000000 mkdocs-macros-plugin-0.7.0/webdoc/docs/pluglets.md
--rw-r--r--   0 laurent    (501) staff       (20)     7974 2021-04-19 13:34:36.000000 mkdocs-macros-plugin-0.7.0/webdoc/docs/tips.md
--rw-r--r--   0 laurent    (501) staff       (20)     9104 2022-03-25 19:24:38.000000 mkdocs-macros-plugin-0.7.0/webdoc/docs/troubleshooting.md
--rw-r--r--   0 laurent    (501) staff       (20)     7478 2022-01-26 01:35:47.000000 mkdocs-macros-plugin-0.7.0/webdoc/docs/why.md
--rw-r--r--   0 laurent    (501) staff       (20)       51 2021-04-23 13:51:49.000000 mkdocs-macros-plugin-0.7.0/webdoc/extra_requirements.txt
--rw-r--r--   0 laurent    (501) staff       (20)     1288 2022-03-25 19:45:29.000000 mkdocs-macros-plugin-0.7.0/webdoc/mkdocs.yml
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-05-25 12:11:51.000000 mkdocs-macros-plugin-1.0.1/
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-05-25 12:11:26.000000 mkdocs-macros-plugin-1.0.1/.github/
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-05-25 12:11:34.000000 mkdocs-macros-plugin-1.0.1/.github/workflows/
+-rw-r--r--   0 laurent    (501) staff       (20)      457 2020-03-10 06:37:22.000000 mkdocs-macros-plugin-1.0.1/.github/workflows/greetings.yml
+-rw-r--r--   0 laurent    (501) staff       (20)      423 2022-07-22 15:00:04.000000 mkdocs-macros-plugin-1.0.1/.gitignore
+-rw-r--r--   0 laurent    (501) staff       (20)      601 2021-04-23 13:52:57.000000 mkdocs-macros-plugin-1.0.1/.readthedocs.yml
+-rw-r--r--   0 laurent    (501) staff       (20)     4360 2023-04-23 11:03:28.000000 mkdocs-macros-plugin-1.0.1/CHANGELOG.md
+-rw-r--r--   0 laurent    (501) staff       (20)     1134 2021-11-23 01:28:45.000000 mkdocs-macros-plugin-1.0.1/LICENSE.md
+-rw-r--r--   0 laurent    (501) staff       (20)       64 2020-11-22 09:50:49.000000 mkdocs-macros-plugin-1.0.1/MANIFEST.in
+-rw-r--r--   0 laurent    (501) staff       (20)     7462 2023-05-25 12:11:51.000000 mkdocs-macros-plugin-1.0.1/PKG-INFO
+-rw-r--r--   0 laurent    (501) staff       (20)     6692 2022-07-22 15:00:04.000000 mkdocs-macros-plugin-1.0.1/README.md
+-rw-r--r--   0 laurent    (501) staff       (20)   249520 2020-02-24 19:02:56.000000 mkdocs-macros-plugin-1.0.1/macros_info.png
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-05-25 12:11:38.000000 mkdocs-macros-plugin-1.0.1/mkdocs_macros/
+-rw-rw-r--   0 laurent    (501) staff       (20)      234 2021-01-04 17:04:12.000000 mkdocs-macros-plugin-1.0.1/mkdocs_macros/__init__.py
+-rw-r--r--   0 laurent    (501) staff       (20)    11781 2023-04-24 12:12:46.000000 mkdocs-macros-plugin-1.0.1/mkdocs_macros/context.py
+-rw-r--r--   0 laurent    (501) staff       (20)     1073 2022-07-22 15:00:04.000000 mkdocs-macros-plugin-1.0.1/mkdocs_macros/errors.py
+-rw-r--r--   0 laurent    (501) staff       (20)     1604 2023-04-22 15:06:54.000000 mkdocs-macros-plugin-1.0.1/mkdocs_macros/macros_info.md
+-rw-r--r--   0 laurent    (501) staff       (20)    26748 2023-04-23 08:50:05.000000 mkdocs-macros-plugin-1.0.1/mkdocs_macros/plugin.py
+-rwxr-xr-x   0 laurent    (501) staff       (20)     6562 2022-03-16 08:10:30.000000 mkdocs-macros-plugin-1.0.1/mkdocs_macros/util.py
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-05-25 12:11:42.000000 mkdocs-macros-plugin-1.0.1/mkdocs_macros_plugin.egg-info/
+-rw-r--r--   0 laurent    (501) staff       (20)     7462 2023-05-25 12:11:24.000000 mkdocs-macros-plugin-1.0.1/mkdocs_macros_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 laurent    (501) staff       (20)     1759 2023-05-25 12:11:26.000000 mkdocs-macros-plugin-1.0.1/mkdocs_macros_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 laurent    (501) staff       (20)        1 2023-05-25 12:11:24.000000 mkdocs-macros-plugin-1.0.1/mkdocs_macros_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 laurent    (501) staff       (20)       60 2023-05-25 12:11:24.000000 mkdocs-macros-plugin-1.0.1/mkdocs_macros_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 laurent    (501) staff       (20)      132 2023-05-25 12:11:24.000000 mkdocs-macros-plugin-1.0.1/mkdocs_macros_plugin.egg-info/requires.txt
+-rw-r--r--   0 laurent    (501) staff       (20)       14 2023-05-25 12:11:24.000000 mkdocs-macros-plugin-1.0.1/mkdocs_macros_plugin.egg-info/top_level.txt
+-rw-r--r--   0 laurent    (501) staff       (20)       38 2023-05-25 12:11:51.000000 mkdocs-macros-plugin-1.0.1/setup.cfg
+-rw-r--r--   0 laurent    (501) staff       (20)     1923 2023-05-25 12:05:14.000000 mkdocs-macros-plugin-1.0.1/setup.py
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-05-25 12:11:42.000000 mkdocs-macros-plugin-1.0.1/test/
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-05-25 12:11:43.000000 mkdocs-macros-plugin-1.0.1/test/debug/
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-05-25 12:11:43.000000 mkdocs-macros-plugin-1.0.1/test/debug/docs/
+-rw-r--r--   0 laurent    (501) staff       (20)      129 2022-03-12 15:07:17.000000 mkdocs-macros-plugin-1.0.1/test/debug/docs/index.md
+-rw-r--r--   0 laurent    (501) staff       (20)      223 2022-03-12 15:07:17.000000 mkdocs-macros-plugin-1.0.1/test/debug/mkdocs.yml
+-rw-rw-r--   0 laurent    (501) staff       (20)     1277 2020-02-23 06:57:46.000000 mkdocs-macros-plugin-1.0.1/test/main_sample.py
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-05-25 12:11:44.000000 mkdocs-macros-plugin-1.0.1/test/module/
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-05-25 12:11:44.000000 mkdocs-macros-plugin-1.0.1/test/module/docs/
+-rw-r--r--   0 laurent    (501) staff       (20)      346 2022-03-25 19:56:02.000000 mkdocs-macros-plugin-1.0.1/test/module/docs/environment.md
+-rw-r--r--   0 laurent    (501) staff       (20)     2372 2022-03-16 08:05:31.000000 mkdocs-macros-plugin-1.0.1/test/module/docs/index.md
+-rw-r--r--   0 laurent    (501) staff       (20)      357 2021-04-21 16:34:52.000000 mkdocs-macros-plugin-1.0.1/test/module/docs/literal.md
+-rw-r--r--   0 laurent    (501) staff       (20)      128 2020-05-15 07:15:24.000000 mkdocs-macros-plugin-1.0.1/test/module/docs/other.md
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-05-25 12:11:45.000000 mkdocs-macros-plugin-1.0.1/test/module/include/
+-rw-r--r--   0 laurent    (501) staff       (20)       68 2021-06-19 05:35:28.000000 mkdocs-macros-plugin-1.0.1/test/module/include/foo.md
+-rw-r--r--   0 laurent    (501) staff       (20)     2023 2023-04-23 08:53:11.000000 mkdocs-macros-plugin-1.0.1/test/module/main.py
+-rw-r--r--   0 laurent    (501) staff       (20)      498 2022-03-25 19:55:51.000000 mkdocs-macros-plugin-1.0.1/test/module/mkdocs.yml
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-05-25 12:11:45.000000 mkdocs-macros-plugin-1.0.1/test/module_dir/
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-05-25 12:11:46.000000 mkdocs-macros-plugin-1.0.1/test/module_dir/docs/
+-rw-r--r--   0 laurent    (501) staff       (20)      237 2022-03-25 19:54:47.000000 mkdocs-macros-plugin-1.0.1/test/module_dir/docs/environment.md
+-rw-r--r--   0 laurent    (501) staff       (20)      529 2020-09-25 16:29:39.000000 mkdocs-macros-plugin-1.0.1/test/module_dir/docs/index.md
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-05-25 12:11:46.000000 mkdocs-macros-plugin-1.0.1/test/module_dir/include/
+-rw-r--r--   0 laurent    (501) staff       (20)       68 2020-03-02 21:15:58.000000 mkdocs-macros-plugin-1.0.1/test/module_dir/include/foo.md
+-rw-r--r--   0 laurent    (501) staff       (20)      281 2020-09-25 16:31:43.000000 mkdocs-macros-plugin-1.0.1/test/module_dir/mkdocs.yml
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-05-25 12:11:46.000000 mkdocs-macros-plugin-1.0.1/test/module_dir/mymodule/
+-rw-r--r--   0 laurent    (501) staff       (20)      685 2021-06-19 08:12:07.000000 mkdocs-macros-plugin-1.0.1/test/module_dir/mymodule/__init__.py
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-05-25 12:11:47.000000 mkdocs-macros-plugin-1.0.1/test/new_syntax/
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-05-25 12:11:47.000000 mkdocs-macros-plugin-1.0.1/test/new_syntax/docs/
+-rw-r--r--   0 laurent    (501) staff       (20)      160 2020-09-28 06:50:54.000000 mkdocs-macros-plugin-1.0.1/test/new_syntax/docs/index.md
+-rw-r--r--   0 laurent    (501) staff       (20)      138 2020-03-22 11:26:31.000000 mkdocs-macros-plugin-1.0.1/test/new_syntax/main.py
+-rw-r--r--   0 laurent    (501) staff       (20)      336 2020-09-28 06:42:49.000000 mkdocs-macros-plugin-1.0.1/test/new_syntax/mkdocs.yml
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-05-25 12:11:48.000000 mkdocs-macros-plugin-1.0.1/test/opt-in/
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-05-25 12:11:48.000000 mkdocs-macros-plugin-1.0.1/test/opt-in/docs/
+-rw-r--r--   0 laurent    (501) staff       (20)       62 2023-04-22 10:48:15.000000 mkdocs-macros-plugin-1.0.1/test/opt-in/docs/index.md
+-rw-r--r--   0 laurent    (501) staff       (20)       93 2023-04-22 10:49:04.000000 mkdocs-macros-plugin-1.0.1/test/opt-in/docs/page_with_macros.md
+-rw-r--r--   0 laurent    (501) staff       (20)      257 2023-04-22 13:36:25.000000 mkdocs-macros-plugin-1.0.1/test/opt-in/mkdocs.yml
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-05-25 12:11:48.000000 mkdocs-macros-plugin-1.0.1/test/opt-out/
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-05-25 12:11:48.000000 mkdocs-macros-plugin-1.0.1/test/opt-out/docs/
+-rw-r--r--   0 laurent    (501) staff       (20)      160 2023-04-22 11:13:20.000000 mkdocs-macros-plugin-1.0.1/test/opt-out/docs/index.md
+-rw-r--r--   0 laurent    (501) staff       (20)       93 2023-04-22 10:49:04.000000 mkdocs-macros-plugin-1.0.1/test/opt-out/docs/page_with_macros.md
+-rw-r--r--   0 laurent    (501) staff       (20)      255 2023-04-22 13:35:37.000000 mkdocs-macros-plugin-1.0.1/test/opt-out/mkdocs.yml
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-05-25 12:11:48.000000 mkdocs-macros-plugin-1.0.1/test/simple/
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-05-25 12:11:48.000000 mkdocs-macros-plugin-1.0.1/test/simple/docs/
+-rw-r--r--   0 laurent    (501) staff       (20)       21 2020-03-04 11:55:35.000000 mkdocs-macros-plugin-1.0.1/test/simple/docs/index.md
+-rw-r--r--   0 laurent    (501) staff       (20)      138 2020-09-15 20:07:40.000000 mkdocs-macros-plugin-1.0.1/test/simple/main_old.py
+-rw-r--r--   0 laurent    (501) staff       (20)       92 2020-02-24 18:30:04.000000 mkdocs-macros-plugin-1.0.1/test/simple/mkdocs.yml
+-rwxr-xr-x   0 laurent    (501) staff       (20)     1119 2020-10-03 09:23:32.000000 mkdocs-macros-plugin-1.0.1/update_pypi.sh
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-05-25 12:11:49.000000 mkdocs-macros-plugin-1.0.1/webdoc/
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-05-25 12:11:51.000000 mkdocs-macros-plugin-1.0.1/webdoc/docs/
+-rw-r--r--   0 laurent    (501) staff       (20)     7677 2023-04-24 07:59:08.000000 mkdocs-macros-plugin-1.0.1/webdoc/docs/advanced.md
+-rw-r--r--   0 laurent    (501) staff       (20)       50 2021-04-23 09:53:10.000000 mkdocs-macros-plugin-1.0.1/webdoc/docs/changelog.md
+-rw-r--r--   0 laurent    (501) staff       (20)     2338 2021-04-24 11:27:05.000000 mkdocs-macros-plugin-1.0.1/webdoc/docs/contribute.md
+-rw-r--r--   0 laurent    (501) staff       (20)    23462 2020-05-15 08:53:26.000000 mkdocs-macros-plugin-1.0.1/webdoc/docs/dog-eating.jpg
+-rw-r--r--   0 laurent    (501) staff       (20)     3998 2022-01-26 01:22:27.000000 mkdocs-macros-plugin-1.0.1/webdoc/docs/git_info.md
+-rw-r--r--   0 laurent    (501) staff       (20)      960 2021-11-23 01:28:45.000000 mkdocs-macros-plugin-1.0.1/webdoc/docs/help.md
+-rw-r--r--   0 laurent    (501) staff       (20)     9232 2023-04-24 07:30:46.000000 mkdocs-macros-plugin-1.0.1/webdoc/docs/index.md
+-rw-r--r--   0 laurent    (501) staff       (20)     1081 2020-03-10 08:29:58.000000 mkdocs-macros-plugin-1.0.1/webdoc/docs/license.md
+-rw-r--r--   0 laurent    (501) staff       (20)    13954 2023-04-23 09:30:47.000000 mkdocs-macros-plugin-1.0.1/webdoc/docs/macros.md
+-rw-r--r--   0 laurent    (501) staff       (20)   249520 2020-03-10 08:57:11.000000 mkdocs-macros-plugin-1.0.1/webdoc/docs/macros_info.png
+-rw-r--r--   0 laurent    (501) staff       (20)     6724 2023-04-22 15:25:41.000000 mkdocs-macros-plugin-1.0.1/webdoc/docs/pages.md
+-rw-r--r--   0 laurent    (501) staff       (20)     5693 2021-09-09 06:43:39.000000 mkdocs-macros-plugin-1.0.1/webdoc/docs/pluglets.md
+-rw-r--r--   0 laurent    (501) staff       (20)    10756 2023-04-23 11:02:22.000000 mkdocs-macros-plugin-1.0.1/webdoc/docs/post_production.md
+-rw-r--r--   0 laurent    (501) staff       (20)     9834 2023-04-23 14:23:38.000000 mkdocs-macros-plugin-1.0.1/webdoc/docs/rendering.md
+-rw-r--r--   0 laurent    (501) staff       (20)     7974 2021-04-19 13:34:36.000000 mkdocs-macros-plugin-1.0.1/webdoc/docs/tips.md
+-rw-r--r--   0 laurent    (501) staff       (20)    10171 2023-04-23 19:17:25.000000 mkdocs-macros-plugin-1.0.1/webdoc/docs/troubleshooting.md
+-rw-r--r--   0 laurent    (501) staff       (20)     7478 2022-01-26 01:35:47.000000 mkdocs-macros-plugin-1.0.1/webdoc/docs/why.md
+-rw-r--r--   0 laurent    (501) staff       (20)       51 2021-04-23 13:51:49.000000 mkdocs-macros-plugin-1.0.1/webdoc/extra_requirements.txt
+-rw-r--r--   0 laurent    (501) staff       (20)     1383 2023-04-23 14:27:56.000000 mkdocs-macros-plugin-1.0.1/webdoc/mkdocs.yml
```

### Comparing `mkdocs-macros-plugin-0.7.0/.readthedocs.yml` & `mkdocs-macros-plugin-1.0.1/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `mkdocs-macros-plugin-0.7.0/CHANGELOG.md` & `mkdocs-macros-plugin-1.0.1/CHANGELOG.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,41 @@
 # Changelog: mkdocs-macros
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/) and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## 1.1.0-alpha, 2024-04-23
+
+* Improved user guide, with introduction of two new pages:
+    "Controlling macro rendering" and "Post production".
+
+* Fixed: (#158) In modules, `on_pre_page_macros()`, the `env.markdown` 
+    attribute is now available to create a header or footer.
+
+* Changed: In `on_post_page_macros()` use `env.markdown` instead of
+    `env.raw_markdown`, for the same purpose.
+
+* Added: (#162) Allow opt-in of page rendering, by using parameter
+    `render_macros: true` in yaml header of the page
+    (requires `render_by_default:false` in the macro parameters,
+    in the config file).
+
+* Fixed: `macro_info()` now generates a header of category 2,
+    so as to be used with other material in the same page,
+    and not confuse the macro generators.
+
+* Changed: `ignore_macros: true` in page header is deprecated. 
+    Use `render_macros: false` instead.
+
+* Fixed: issues #155 (documentation type), #143 (`git.tab`), 
+    #135 (indicate page where rendering failed).
+
+* Bump version to 1.1.0 to acknowledge that API is stable.
+
 ## 0.7.0, 2022-03-25
 
 * Added: (#133) `on_error_fail` in config file to make build/serve process
         fail in case of macro error, with return code 100.
 
 * Added: (#130) Documentation on the tree structure of a typical 
          macro directory (package) 
@@ -26,15 +54,15 @@
 
 ## 0.6.3, 2021-11-23
 
 * Fixed: Broken build of 0.6.2
 
 ## 0.6.2, 2021-11-22 (yanked)
 
-* Added: `env.raw_markdown` is now modifiable, for use in `on_post_page_macros()`
+* Added: `env.markdown` is now modifiable, for use in `on_post_page_macros()`
 
 ## 0.6.1, 2021-09-09
 
 * Added: auto-install of pluglets (in `module` parameter in config file)
 
 ## 0.6.0, 2021-22-08
```

### Comparing `mkdocs-macros-plugin-0.7.0/LICENSE.md` & `mkdocs-macros-plugin-1.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mkdocs-macros-plugin-0.7.0/PKG-INFO` & `mkdocs-macros-plugin-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: mkdocs-macros-plugin
-Version: 0.7.0
+Version: 1.0.1
 Summary: Unleash the power of MkDocs with macros and variables
 Home-page: https://github.com/fralau/mkdocs_macros_plugin
 Author: Laurent Franceschbetti
 Author-email: info@settlenext.com
 License: MIT
 Keywords: mkdocs python markdown macros
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.5
-Requires-Python: >=3.5
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE.md
 
 # mkdocs-macros-plugin: Unleash the power of MkDocs with variables and macros
 
 
@@ -145,15 +144,15 @@
 To install the extra dependencies required for testing the package, run:
 
 ```
 pip install "mkdocs-macros-plugin[test]"
 ```
 
 ### Declaration of plugin
-Declare the plugin in the the file `mkdocs.yml`:
+Declare the plugin in the file `mkdocs.yml`:
 
 ```yaml
 plugins:
     - search
     - macros
 ```
 
@@ -208,15 +207,15 @@
 distributed through [PyPI](https://pypi.org/).
 
 
 ### How to add a pluglet to an mkdocs project?
 
 Install it: 
 
-```python
+```shell
 pip install <pluglet_name>
 ```
 
 Declare it in the project's config (`mkdocs.yml`) file:
 
 ```yaml
 plugins:
@@ -227,8 +226,7 @@
 ```
 
 ### How to write a pluglet?
 
 [See instructions in the documentation](https://mkdocs-macros-plugin.readthedocs.io/en/latest/pluglets/).
 
 A sample pluglet can be found in [mkdocs-test (github)](https://github.com/fralau/mkdocs-macros-test).
-
```

### Comparing `mkdocs-macros-plugin-0.7.0/README.md` & `mkdocs-macros-plugin-1.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -123,15 +123,15 @@
 To install the extra dependencies required for testing the package, run:
 
 ```
 pip install "mkdocs-macros-plugin[test]"
 ```
 
 ### Declaration of plugin
-Declare the plugin in the the file `mkdocs.yml`:
+Declare the plugin in the file `mkdocs.yml`:
 
 ```yaml
 plugins:
     - search
     - macros
 ```
 
@@ -186,15 +186,15 @@
 distributed through [PyPI](https://pypi.org/).
 
 
 ### How to add a pluglet to an mkdocs project?
 
 Install it: 
 
-```python
+```shell
 pip install <pluglet_name>
 ```
 
 Declare it in the project's config (`mkdocs.yml`) file:
 
 ```yaml
 plugins:
```

### Comparing `mkdocs-macros-plugin-0.7.0/macros_info.png` & `mkdocs-macros-plugin-1.0.1/macros_info.png`

 * *Files identical despite different names*

### Comparing `mkdocs-macros-plugin-0.7.0/mkdocs_macros/context.py` & `mkdocs-macros-plugin-1.0.1/mkdocs_macros/context.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from mkdocs.structure.nav import get_navigation
 from mkdocs.structure.files import File
 import os
 import sys
 import subprocess
 import platform
 import traceback
-import pkg_resources
+from importlib.metadata import version as package_version
 import datetime
 from dateutil.parser import parse as date_parse
 from functools import partial
 
 import mkdocs
 import jinja2
 from jinja2 import Template
@@ -158,18 +158,15 @@
             # NOTE: The 'text' argument is clearer,
             #       but for Python < 3.7, only `universal_newlines`
             #       is accepted
             try:
                 r[var] = subprocess.check_output(command,
                                                  universal_newlines=True,
                                                  stderr=subprocess.DEVNULL).strip()
-                # keep first part
-                if var == 'tag':
-                    r[var] = r[var].split('-')[0]
-                elif var == 'date_ISO':
+                if var == 'date_ISO':
                     r['date'] = date_parse(r[var])
                 r['status'] = True
             except subprocess.CalledProcessError as e:
                 if e.returncode == 128:
                     # generally means "unexpected error"
                     # git status (no repo),
                     # git tag (no tag)
@@ -288,16 +285,15 @@
     # Get data on the environment (versions)
     try:
         environment = {
             'system': system_name(),
             'system_version': system_version(),
             'python_version': python_version(),
             'mkdocs_version': mkdocs.__version__,
-            'macros_plugin_version':
-            pkg_resources.get_distribution(PACKAGE_NAME).version,
+            'macros_plugin_version': package_version(PACKAGE_NAME),
             'jinja2_version': jinja2.__version__,
             # 'site_git_version': site_git_version(),
         }
     except Exception as e:
         # Avoid breaking the system if error in reading the system info:
         environment = ("<i><b>Cannot read system info!</b> %s: %s</i>" %
                        (type(e).__name__, str(e)))
@@ -307,15 +303,15 @@
     env.variables['plugin'] = env.config
 
     # git information:
     env.variables['git'] = get_git_info()
 
     def render_file(filename):
         """
-        Render an external page (filename) containing jinj2 code
+        Render an external page (filename) containing jinja2 code
         Do not declare as macro, as this is pointless.
         """
         SOURCE_FILE = os.path.join(SOURCE_DIR, filename)
         with open(SOURCE_FILE) as f:
             s = f.read()
         # now we need to render the jinja2 directives:
         return env.render(s)
```

### Comparing `mkdocs-macros-plugin-0.7.0/mkdocs_macros/macros_info.md` & `mkdocs-macros-plugin-1.0.1/mkdocs_macros/macros_info.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 {#
 Template for the macro_info() command
 (C) Laurent Franceschetti 2019
 #}
 
 
-# Macros Plugin Environment
+## Macros Plugin Environment
 
-## General List
+### General List
 All available variables and filters within the macros plugin:
 {{ context() | pretty }}
 
-## Config Information
+### Config Information
 Standard MkDocs configuration information. Do not try to modify.
 
 e.g. {{ "`{{ config.docs_dir }}`" }}
 
 See also the [MkDocs documentation on the config object](https://www.MkDocs.org/user-guide/custom-themes/#config).
 
 {{ context(config)| pretty }}
 
-## Macros
+### Macros
 These macros have been defined programmatically for this environment
 (module or pluglets). 
 {{ context(macros)| pretty }}
 
-## Git Information
+### Git Information
 Information available on the last commit and the git repository containing the
 documentation project:
 
 e.g. {{ "`{{ git.message }}`" }}
 
 {{ context(git)| pretty }}
 
-## Page Attributes
+### Page Attributes
 Provided by MkDocs. These attributes change for every page
 (the attributes shown are for this page).
 
 e.g. {{ "`{{ page.title }}`" }}
 
 See also the [MkDocs documentation on the page object](https://www.MkDocs.org/user-guide/custom-themes/#page).
 
@@ -49,17 +49,17 @@
 {% raw %}
 {% for page in navigation.pages %}
 - {{ page.title }}
 {% endfor %}
 {% endraw %}
 ```
 
-## Plugin Filters
+### Plugin Filters
 These filters are provided as a standard by the macros plugin.
 {{ context(filters)| pretty }}
 
-## Builtin Jinja2 Filters
+### Builtin Jinja2 Filters
 These filters are provided by Jinja2 as a standard.
 
 See also the [Jinja2 documentation on builtin filters](https://jinja.palletsprojects.com/en/2.11.x/templates/#builtin-filters)).
 
 {{ context(filters_builtin) | pretty }}
```

### Comparing `mkdocs-macros-plugin-0.7.0/mkdocs_macros/plugin.py` & `mkdocs-macros-plugin-1.0.1/mkdocs_macros/plugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,31 +2,33 @@
 # Main part of the plugin
 # Defines the VariablesPlugin class
 #
 # Laurent Franceschetti (c) 2018
 # MIT License
 # --------------------------------------------
 
+import importlib
 import os
-import traceback
 from copy import copy
-import importlib
-
 
 import yaml
-from jinja2 import (Environment, FileSystemLoader, TemplateSyntaxError,
-                    Undefined, DebugUndefined, StrictUndefined)
-from mkdocs.plugins import BasePlugin
+from jinja2 import (
+    Environment, FileSystemLoader, Undefined, DebugUndefined, StrictUndefined,
+)
 from mkdocs.config import config_options
 from mkdocs.config.config_options import Type as PluginType
+from mkdocs.plugins import BasePlugin
+from mkdocs.structure.pages import Page
 
-
-from .util import (install_package, parse_package, trace, debug,
-        update, SuperDict, import_local_module, format_chatter, LOG)
-from .context import define_env
+from mkdocs_macros.errors import format_error
+from mkdocs_macros.context import define_env
+from mkdocs_macros.util import (
+    install_package, parse_package, trace, debug,
+    update, SuperDict, import_local_module, format_chatter, LOG,
+)
 
 # ------------------------------------------
 # Initialization
 # ------------------------------------------
 
 # The subsets of the YAML file that will be used for the variables:
 YAML_VARIABLES = 'extra'
@@ -78,14 +80,16 @@
     J2_STRING = PluginType(str, default='')
     config_scheme = (
         # main python module:
         ('module_name',  PluginType(str,
                                     default=DEFAULT_MODULE_NAME)),
         ('modules', PluginType(list,
                                default=[])),
+        # How to render pages by default: yes (opt-out), no (opt-in)
+        ('render_by_default', PluginType(bool, default=True)),
         # include directory for templates ({% include ....%}):
         ('include_dir',  J2_STRING),
         # list of additional yaml files:
         ('include_yaml', PluginType(list, default=[])),
         # for altering the j2 markers, in case of need:
         ('j2_block_start_string',    J2_STRING),
         ('j2_block_end_string',      J2_STRING),
@@ -241,35 +245,54 @@
         try:
             return self._page
         except AttributeError:
             raise AttributeError("Too early: page information is not available"
                                  "at this stage!")
 
     @property
-    def raw_markdown(self):
+    def markdown(self):
         """
-        The page information
+        The markdown after interpretation
         """
         try:
-            return self._raw_markdown
+            return self._markdown
         except AttributeError:
             raise AttributeError("Too early: raw markdown is not available"
                                  "at this stage!")
 
-    @raw_markdown.setter
-    def raw_markdown(self, value):
+    @markdown.setter
+    def markdown(self, value):
         """
         Used to set the raw markdown
         """
         if not isinstance(value, str):
-            raise ValueError("Value provided to attribute raw_markdown "
+            raise ValueError("Value provided to attribute markdown "
                              "should be a string")
         # check whether attribute is accessible:
-        self.raw_markdown
-        self._raw_markdown = value
+        self.markdown
+        self._markdown = value
+
+
+    @property
+    def raw_markdown(self):
+        """
+        Cancelled attribute
+        """
+        trace("Property env.raw_markdown is removed "
+                             "as of 1.1.0; use env.markdown instead!")
+        return self.markdown(self)
+    
+    @markdown.setter
+    def raw_markdown(self, value):
+        """
+        Used to set the raw markdown
+        """
+        trace("Property env.raw_markdown is removed "
+             "as of 1.1.0; use env.markdown instead!")
+        self.markdown = value
 
     # ----------------------------------
     # Function lists, for later events
     # ----------------------------------
 
     @property
     def pre_macro_functions(self):
@@ -440,78 +463,82 @@
                 # trace("No module")
                 pass
             else:
                 raise ImportError("Macro plugin could not find custom '%s' "
                                   "module in '%s'." %
                                   (local_module_name, self.project_dir))
 
-    def render(self, markdown):
+    def render(self, markdown: str):
         """
         Render a page through jinja2: it executes the macros
 
         Returns
         -------
         A pure markdown/HTML page.
 
         Notes
         -----
         - Must called by '_on_page_markdown()'
         - If the YAML header of the page contains `ignore_macros: true`
           then NO rendering will be done, and the markdown will be returned
           as is.
         """
+
+        # Process meta_variables
+        # ----------------------
         # copy the page variables and update with the meta data
         # in the YAML header:
         page_variables = copy(self.variables)
         meta_variables = self.variables['page'].meta
-        # it must be possible to completely
+        # Warning this is ternary logique (True, False, None: nothing said)
+        ignore_macros = None
+        render_macros = None
+        
         if meta_variables:
-            # a trick to force of a page NOT to be interpreted,
-            if meta_variables.get('ignore_macros') == True:
+            # determine whether the page will be rendered or not
+            # the two formulations are accepted
+            ignore_macros = meta_variables.get('ignore_macros')
+            render_macros = meta_variables.get('render_macros')
+
+        if self.config['render_by_default']:
+            # opt-out: force of a page NOT to be interpreted,
+            opt_out = ignore_macros == True or render_macros == False
+            if opt_out:
+                return markdown
+        else:
+            # opt-in: force a page to be interpreted
+            opt_in = render_macros == True or ignore_macros == False
+            if not opt_in:
                 return markdown
-            # trace("Metavariables for '%s':" % self.variables['page'].title,
-            #                 meta_variables)
-            page_variables.update(meta_variables)
+        # Update the page with meta variables
+        # i.e. what's in the yaml header of the page
+        page_variables.update(meta_variables)
 
+        # Rendering
+        # ----------------------
         # expand the template
         on_error_fail = self.config['on_error_fail']
         try:
             md_template = self.env.from_string(markdown)
             # Execute the jinja2 template and return
             return md_template.render(**page_variables)
-        except TemplateSyntaxError as e:
-            line = markdown.splitlines()[e.lineno-1]
-            output = ["# _Macro Syntax Error_",
-                      "_Line %s in Markdown file:_ **%s** " %
-                      (e.lineno, e.message),
-                      "```python",
-                      line,
-                      "```"]
-            error = "\n".join(output)
-            trace("ERROR", error)
-            if on_error_fail:
-                exit(ERROR_MACRO)
-            else:
-                # default case
-                return error
-        except Exception as e:
-            output = ["# _Macro Rendering Error_",
-                      "",
-                      "**%s**: %s" % (type(e).__name__, e),
-                      "", "",
-                      "```",
-                      traceback.format_exc(),
-                      "```"]
-            error = "\n".join(output)
-            trace("ERROR", error)
+
+        except Exception as error:
+            error_message = format_error(
+                error,
+                markdown=markdown,
+                page=self.page,
+            )
+
+            trace('ERROR', error_message)
             if on_error_fail:
                 exit(ERROR_MACRO)
+
             else:
-                # default case
-                return error
+                return error_message
 
     # ----------------------------------
     # Standard Hooks for a mkdocs plugin
     # ----------------------------------
 
     def on_config(self, config):
         """
@@ -677,23 +704,28 @@
         if not self.variables:
             return markdown
         else:
             # Update the page info in the document
             # page is an object with a number of properties (title, url, ...)
             # see: https://github.com/mkdocs/mkdocs/blob/master/mkdocs/structure/pages.py
             self.variables["page"] = copy(page)
+            # set the markdown (for the first time)
+            self._markdown = markdown
             # execute the pre-macro functions in the various modules
             for func in self.pre_macro_functions:
                 func(self)
             # render the macros
-            self._raw_markdown = self.render(markdown)
+            self.markdown = self.render(
+                markdown=self.markdown,
+                # page=page,
+            )
             # execute the post-macro functions in the various modules
             for func in self.post_macro_functions:
                 func(self)
-            return self.raw_markdown
+            return self.markdown
 
     def on_post_build(self, config: config_options.Config):
         """
         Hook for post build actions, typically adding
         raw files to the setup.
         """
         # execute the functions in the various modules
```

### Comparing `mkdocs-macros-plugin-0.7.0/mkdocs_macros/util.py` & `mkdocs-macros-plugin-1.0.1/mkdocs_macros/util.py`

 * *Files identical despite different names*

### Comparing `mkdocs-macros-plugin-0.7.0/mkdocs_macros_plugin.egg-info/PKG-INFO` & `mkdocs-macros-plugin-1.0.1/mkdocs_macros_plugin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: mkdocs-macros-plugin
-Version: 0.7.0
+Version: 1.0.1
 Summary: Unleash the power of MkDocs with macros and variables
 Home-page: https://github.com/fralau/mkdocs_macros_plugin
 Author: Laurent Franceschbetti
 Author-email: info@settlenext.com
 License: MIT
 Keywords: mkdocs python markdown macros
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.5
-Requires-Python: >=3.5
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE.md
 
 # mkdocs-macros-plugin: Unleash the power of MkDocs with variables and macros
 
 
@@ -145,15 +144,15 @@
 To install the extra dependencies required for testing the package, run:
 
 ```
 pip install "mkdocs-macros-plugin[test]"
 ```
 
 ### Declaration of plugin
-Declare the plugin in the the file `mkdocs.yml`:
+Declare the plugin in the file `mkdocs.yml`:
 
 ```yaml
 plugins:
     - search
     - macros
 ```
 
@@ -208,15 +207,15 @@
 distributed through [PyPI](https://pypi.org/).
 
 
 ### How to add a pluglet to an mkdocs project?
 
 Install it: 
 
-```python
+```shell
 pip install <pluglet_name>
 ```
 
 Declare it in the project's config (`mkdocs.yml`) file:
 
 ```yaml
 plugins:
@@ -227,8 +226,7 @@
 ```
 
 ### How to write a pluglet?
 
 [See instructions in the documentation](https://mkdocs-macros-plugin.readthedocs.io/en/latest/pluglets/).
 
 A sample pluglet can be found in [mkdocs-test (github)](https://github.com/fralau/mkdocs-macros-test).
-
```

### Comparing `mkdocs-macros-plugin-0.7.0/mkdocs_macros_plugin.egg-info/SOURCES.txt` & `mkdocs-macros-plugin-1.0.1/mkdocs_macros_plugin.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 README.md
 macros_info.png
 setup.py
 update_pypi.sh
 .github/workflows/greetings.yml
 mkdocs_macros/__init__.py
 mkdocs_macros/context.py
+mkdocs_macros/errors.py
 mkdocs_macros/macros_info.md
 mkdocs_macros/plugin.py
 mkdocs_macros/util.py
 mkdocs_macros_plugin.egg-info/PKG-INFO
 mkdocs_macros_plugin.egg-info/SOURCES.txt
 mkdocs_macros_plugin.egg-info/dependency_links.txt
 mkdocs_macros_plugin.egg-info/entry_points.txt
@@ -33,14 +34,20 @@
 test/module_dir/docs/environment.md
 test/module_dir/docs/index.md
 test/module_dir/include/foo.md
 test/module_dir/mymodule/__init__.py
 test/new_syntax/main.py
 test/new_syntax/mkdocs.yml
 test/new_syntax/docs/index.md
+test/opt-in/mkdocs.yml
+test/opt-in/docs/index.md
+test/opt-in/docs/page_with_macros.md
+test/opt-out/mkdocs.yml
+test/opt-out/docs/index.md
+test/opt-out/docs/page_with_macros.md
 test/simple/main_old.py
 test/simple/mkdocs.yml
 test/simple/docs/index.md
 webdoc/extra_requirements.txt
 webdoc/mkdocs.yml
 webdoc/docs/advanced.md
 webdoc/docs/changelog.md
@@ -50,10 +57,12 @@
 webdoc/docs/help.md
 webdoc/docs/index.md
 webdoc/docs/license.md
 webdoc/docs/macros.md
 webdoc/docs/macros_info.png
 webdoc/docs/pages.md
 webdoc/docs/pluglets.md
+webdoc/docs/post_production.md
+webdoc/docs/rendering.md
 webdoc/docs/tips.md
 webdoc/docs/troubleshooting.md
 webdoc/docs/why.md
```

### Comparing `mkdocs-macros-plugin-0.7.0/setup.py` & `mkdocs-macros-plugin-1.0.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from setuptools import setup, find_packages
 
 
 # --------------------
 # Initialization
 # --------------------
 
-VERSION_NUMBER = '0.7.0'
+VERSION_NUMBER = '1.0.1'
 
 # required if you want to run document/test
 # pip install 'mkdocs-macros-plugin[test]'
 TEST_REQUIRE = ['mkdocs-macros-test', 'mkdocs-material>=6.2',
                 'mkdocs-include-markdown-plugin']
 
 # --------------------
@@ -36,15 +36,15 @@
     long_description=read_file('README.md'),
     long_description_content_type='text/markdown',
     keywords='mkdocs python markdown macros',
     url='https://github.com/fralau/mkdocs_macros_plugin',
     author='Laurent Franceschbetti',
     author_email='info@settlenext.com',
     license='MIT',
-    python_requires='>=3.5',
+    python_requires='>=3.8',
     install_requires=[
         'mkdocs>=0.17',
         'jinja2',
         'termcolor',
         'pyyaml',
         'python-dateutil',
     ],
```

### Comparing `mkdocs-macros-plugin-0.7.0/test/main_sample.py` & `mkdocs-macros-plugin-1.0.1/test/main_sample.py`

 * *Files identical despite different names*

### Comparing `mkdocs-macros-plugin-0.7.0/test/module/docs/index.md` & `mkdocs-macros-plugin-1.0.1/test/module/docs/index.md`

 * *Files identical despite different names*

### Comparing `mkdocs-macros-plugin-0.7.0/test/module/main.py` & `mkdocs-macros-plugin-1.0.1/test/module/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -42,21 +42,25 @@
         chatter("Display a button:", label, url)
         url = fix_url(url)
         HTML = """<a class='md-button' href="%s">%s</a>"""
         return HTML % (url, label)
 
     env.variables.special_docs_dir = env.variables.config['docs_dir']
 
+def on_pre_page_macros(env):
+    "Before macros are executed"
+    footer = "\n##Added Footer (Pre-macro)\nBuild hour is {{ now() }}"
+    env.markdown += footer
 
 def on_post_page_macros(env):
     "After macros were executed"
     # This will add a (Markdown or HTML) footer
     footer = '\n'.join(
-        ['', '# Added Footer (Post-build)', 'Name of the page is _%s_' % env.page.title])
-    env.raw_markdown += footer
+        ['', '##Added Footer (Post-macro)', 'Name of the page is _%s_' % env.page.title])
+    env.markdown += footer
 
 
 def on_post_build(env):
     "Post build action"
     # activate trace
     chatter = env.start_chatting("Simple module (post-build)")
     chatter("This means `on_post_build(env)` works")
```

### Comparing `mkdocs-macros-plugin-0.7.0/test/module_dir/docs/index.md` & `mkdocs-macros-plugin-1.0.1/test/module_dir/docs/index.md`

 * *Files identical despite different names*

### Comparing `mkdocs-macros-plugin-0.7.0/test/module_dir/mymodule/__init__.py` & `mkdocs-macros-plugin-1.0.1/test/module_dir/mymodule/__init__.py`

 * *Files identical despite different names*

### Comparing `mkdocs-macros-plugin-0.7.0/update_pypi.sh` & `mkdocs-macros-plugin-1.0.1/update_pypi.sh`

 * *Files identical despite different names*

### Comparing `mkdocs-macros-plugin-0.7.0/webdoc/docs/contribute.md` & `mkdocs-macros-plugin-1.0.1/webdoc/docs/contribute.md`

 * *Files identical despite different names*

### Comparing `mkdocs-macros-plugin-0.7.0/webdoc/docs/dog-eating.jpg` & `mkdocs-macros-plugin-1.0.1/webdoc/docs/dog-eating.jpg`

 * *Files identical despite different names*

### Comparing `mkdocs-macros-plugin-0.7.0/webdoc/docs/git_info.md` & `mkdocs-macros-plugin-1.0.1/webdoc/docs/git_info.md`

 * *Files identical despite different names*

### Comparing `mkdocs-macros-plugin-0.7.0/webdoc/docs/help.md` & `mkdocs-macros-plugin-1.0.1/webdoc/docs/help.md`

 * *Files identical despite different names*

### Comparing `mkdocs-macros-plugin-0.7.0/webdoc/docs/index.md` & `mkdocs-macros-plugin-1.0.1/webdoc/docs/index.md`

 * *Files 15% similar despite different names*

```diff
@@ -234,27 +234,32 @@
 ### Configuration of the plugin
 
 Here are all the possible arguments in the `plugin` section
 of the MkDocs' config file:
 
 | Argument | Default | Description
 | -- | -- | --
-| `module_name` | `main` | [Name of the Python module](python/#local-module) containing macros, filters and variables. Indicate the file or directory, without extension; you may specify a path (e.g. `include/module`). If no `main` module is available, it is ignored.
-| `modules` | `[]`| [List of preinstalled Python modules](python/#adding-pre-installed-modules), i.e. listed by `pip list`.
+|`render_by_default`|`true`|Render macros on all pages by default. If set to false, sets an [opt-in mode](rendering/#solution-2-opt-in-specify-which-pages-must-be-rendered) where only pages marked with `render_macros: true` in header will be displayed.
+| `module_name` | main| [Name of the Python module](macros/#local-module) containing macros, filters and variables. Indicate the file or directory, without extension; you may specify a path (e.g. `include/module`). If no `main` module is available, it is ignored.
+| `modules` | `[]`| [List of pluglets](pluglets) to be added to mkdocs-macros (preinstalled Python modules that can be listed by `pip list`).
 | `include_dir` | | [Directory for including external files](advanced/#changing-the-directory-of-the-includes) 
 | `include_yaml`| `[]` | [List of yaml files or `key: filename` pairs to be included](advanced/#including-external-yaml-files)
-| `j2_block_start_string` | | [Non-standard Jinja2 marker for start of block](advanced/#solution-3-altering-the-syntax-of-jinja2-for-mkdocs-macros)
-| `j2_block_end_string` || [Non-standard Jinja2 marker for end of block](advanced/#solution-3-altering-the-syntax-of-jinja2-for-mkdocs-macros)
-| `j2_variable_start_string` || [Non-standard Jinja2 marker for start of variable](advanced/#solution-3-altering-the-syntax-of-jinja2-for-mkdocs-macros) 
-| `j2_variable_end_string` || [Non-standard Jinja2 marker for end of variable](advanced/#solution-3-altering-the-syntax-of-jinja2-for-mkdocs-macros)
-
+| `j2_block_start_string` | | [Non-standard Jinja2 marker for start of block](rendering/#solution-5-altering-the-syntax-of-jinja2-for-mkdocs-macros)
+| `j2_block_end_string` || [Non-standard Jinja2 marker for end of block](rendering/#solution-5-altering-the-syntax-of-jinja2-for-mkdocs-macros)
+| `j2_variable_start_string` || [Non-standard Jinja2 marker for start of variable](rendering/#solution-5-altering-the-syntax-of-jinja2-for-mkdocs-macros) 
+| `j2_variable_end_string` || [Non-standard Jinja2 marker for end of variable](rendering/#solution-5-altering-the-syntax-of-jinja2-for-mkdocs-macros)
+|`on_error_fail`|`false`| [Make the building process fail in case of an error in macro rendering](/troubleshooting/#make-the-build-process-fail-in-case-of-error) (this is useful when the website is rebuilt automatically and errors must be detected.)
+|`on_undefined`|keep|[Behavior of the macros renderer in case of an undefined variable in a page](troubleshooting/#is-it-possible-to-make-the-building-process-fail-in-case-of-page-error). By default, it leaves the Jinja2 statement untouched (e.g. `{{ foo }}` will appear as such in the page.) Use the value 'strict' to make it fail.
+|`verbose`|`false`| Print [debug (more detailed) statements](troubleshooting/#verbose-debug-statements-in-macros) in the console.
 
 ___
 For example:
 
 ```yaml
 plugins:
   - search
   - macros:
       module_name: mymodule
       include_dir: include
+      on_error_fail: true
+      on_undefined: strict
 ```
```

### Comparing `mkdocs-macros-plugin-0.7.0/webdoc/docs/license.md` & `mkdocs-macros-plugin-1.0.1/webdoc/docs/license.md`

 * *Files identical despite different names*

### Comparing `mkdocs-macros-plugin-0.7.0/webdoc/docs/macros.md` & `mkdocs-macros-plugin-1.0.1/webdoc/docs/macros.md`

 * *Files 12% similar despite different names*

```diff
@@ -241,15 +241,15 @@
 as all objects that could be manipulated.
 
 !!! Note
     `env.config` is thus a superset of the `env.conf` object
     (which is `env.config['config']`).
 
 !!! Caution
-    This is object is **not** accessible as a variable from the markdown pages.
+    This object is **not** accessible as a variable from the markdown pages.
     Exposing it might encourage black magic.
 
 
 ### Validating environment variables in Python code
 
 By design, the call to `define_env()` is the last stage of the config
 process, to create the jinja2 environment that will interpret the jinja2
@@ -362,112 +362,44 @@
 
 Depending on your use case, you may want to give **access to the shell**
 (e.g. for a development team). Or else, may you **want to "sandbox" your
 web pages** (for business applications). 
 
 
 
-The `declare_variables()` function (DEPRECATED)
-----------------------------------------
 
-!!! Warning
-    `declare_variables()` is the old paradigm, before 0.3.0
-    and it is DEPRECATED. 
-    Support for this call will be discontinued in a future version.
-    
-    Use instead the `define_env()` function.
-
-As a first step, you need declare a hook function called
-`declare_variables`, with two arguments:
-
--   `variables`: the dictionary that contains the variables. It is
-    initialized with the values contained in the `extra` section of the
-    `mkdocs.yml` file.
--   `macro`: a decorator function that you can use to declare a Python
-    function as a Jinja2 callable ('macro' for MkDocs).
-
-The example should be self-explanatory:
 
-``` {.python}
-def declare_variables(variables, macro):
-    """
-    This is the hook for the functions
+## What you can and can't do with `define_env()`
 
-    - variables: the dictionary that contains the environment variables
-    - macro: a decorator function, to declare a macro.
-    """
+The fact is that you **cannot** actually access page information
+in the `define_env()` function, since
+it operates at the configuration stage of the page building process 
+(during the [`on_config()` event of MkDocs](https://www.mkdocs.org/user-guide/plugins/#on_config)). 
+At that point, **you don't have access to specific pages**
 
-    variables['baz'] = "John Doe"
 
-    @macro
-    def bar(x):
-        return (2.3 * x) + 7
+!!! Warning "Vital Note on mkdocs-macros" 
+    Of course, you **can** declare **macros**, which **appear** to act on pages. 
+    But realize that these are only **declarations** and that their
+    execution is **deferred**. 
+    The macros will actually be run ** later** 
+    (by MkDocs' [`on_page_markdown()` event](https://www.mkdocs.org/user-guide/plugins/#on_page_markdown)),
+    just before the markdown is rendered. The framework is so organized
+    that, in macros, you are actually "talking" about objects that don't exist yet.
 
+    So you **cannot** influence the rendering process other than by
+    adding macros, variables and filters to `mkdocs_macros`.
 
 
-    # If you wish, you can  declare a macro with a different name:
-    def f(x):
-        return x * x
 
-    macro(f, 'barbaz')
 
-    # or to export some predefined function
-    import math
-    macro(math.floor) # will be exported as 'floor'
-```
 
-Your **registration** of variables or macros for MkDocs should be done
-inside that hook function. On the other hand, nothing prevents you from
-making imports or declarations **outside** of this function.
+!!! Danger "Do not modify system entities in `env.variables`"
 
-> **Note:** You can export a wide range of objects, and their attributes
-> remain accessible (see [more
-> information](http://jinja.pocoo.org/docs/2.10/templates/#variables))
-
-### Accessing variables
-
-In case you need to access some variables defined in the config file
-(under `extra`), use the `variables` dictionary:
-
-Suppose you have:
-
-``` {.yaml}
-extra:
-    price: 12.50
-```
+    Also, the system information in `env.variables`
+    is for **reading** purposes.
+    You could modify it in your Python code, of course (at your own peril).
+    But **by design**, it may have no effect on the mechanics
+    of `mkdocs` (these are shallow copies). 
 
-You could write a macro:
+    Whatever you do in that way, is likely to be branded **black magic**.
 
-``` {.python}
-@macro
-def compare_price(my_price):
-    "Compare the price to the price in config file"
-    if my_price > env.variables['price']:
-        return("Price is higher than standard")
-    else:
-        return("Price is lower than standard")
-```
-
-For your convenience, you may also use the dot notation:
-``` {.python}
-@macro
-def compare_price(my_price):
-    "Compare the price to the price in config file"
-    if my_price > env.variables.price:
-        return("Price is higher than standard")
-    else:
-        return("Price is lower than standard")
-```
-
-### Accessing macros
-!!! Note "A macro is Python variable"
-    Note that since a macro is also a Python 
-    variable (function), you can also "import"
-    it in a module. 
-    For example, `fix_url` is a predefined macro that fixes relative
-    urls (when applicable) so that they point to the root of the site:
-
-
-```
-fix_url = env.macros.fix_url
-my_url = fix_url(url)
-```
```

### Comparing `mkdocs-macros-plugin-0.7.0/webdoc/docs/macros_info.png` & `mkdocs-macros-plugin-1.0.1/webdoc/docs/macros_info.png`

 * *Files identical despite different names*

### Comparing `mkdocs-macros-plugin-0.7.0/webdoc/docs/pages.md` & `mkdocs-macros-plugin-1.0.1/webdoc/docs/pages.md`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 A custom **filter** is a Jinja2 concept. It is essentially a Python
 function used with a different syntax,
 e.g. `{{ 'my text ' | uppercase}}` (supposing there was a custom
 function called `uppercase` and declared as a filter). Just as a
 macro, a filter should return a *string* that can be plain, markdown
 or HTML.
 
-"Batteries included": defaut objects
+"Batteries included": default objects
 --------------------------------------
 
 The following objects are, in particular, available by default,
 with their set of attributes:
 
 | Object | Description
 | -- | --
@@ -186,30 +186,30 @@
     `{% import ..}` directive.
     See explanations under [Advanced Usage](../advanced/#importing-macros-from-a-separate-file).
 
 
 Conditionals, loops, etc.
 -------------------------
 
-With the macros plugin, you may use the [conditional](https://jinja.palletsprojects.com/en/2.11.x/templates/#if)
+With the macros plugin, you may use the [conditional](https://jinja.palletsprojects.com/en/3.0.x/templates/#if)
 statement of Jinja2, e.g.
 
 ``` {.jinja2}
 ### My title
 {% if  == 'bar' %}
 We will write this **first version**
 {% else %}
 _Second version_
 {% endif %}
 ```
 
 You may produce Markdown or any mix of Markdown, HTML, css
 and even javascript that you wish.
 
-Similarly, you could use [for loops](https://jinja.palletsprojects.com/en/2.11.x/templates/#for):
+Similarly, you could use [for loops](https://jinja.palletsprojects.com/en/3.0.x/templates/#for):
 
 ``` {.jinja2}
 ### List of users
 {% set users = ['joe', 'jill', 'david', 'sam'] %}
 {% for user in users %}
 1. {{ user }}
 {% endfor %}
```

#### html2text {}

```diff
@@ -10,16 +10,16 @@
 HTML. Each call to the macro in markdown page will be replaced by that result.
 !!! Note For more information on the full concept of a macro, see [the detailed
 explanation](why.md#use-case-overcoming-the-intrinsic-limitations-of-markdown-
 syntax). ### 3. Filter A custom **filter** is a Jinja2 concept. It is
 essentially a Python function used with a different syntax, e.g.Â `{{ 'my text
 ' | uppercase}}` (supposing there was a custom function called `uppercase` and
 declared as a filter). Just as a macro, a filter should return a *string* that
-can be plain, markdown or HTML. "Batteries included": defaut objects ----------
----------------------------- The following objects are, in particular,
+can be plain, markdown or HTML. "Batteries included": default objects ---------
+----------------------------- The following objects are, in particular,
 available by default, with their set of attributes: | Object | Description | -
 - | -- | `config` | The standard [config](https://www.mkdocs.org/user-guide/
 configuration/#project-information) information on MkDocs' environment. |
 `page` | Info on the current page ([source](https://github.com/mkdocs/mkdocs/
 blob/master/mkdocs/structure/pages.py)) | `navigation` | List of all pages/
 sections of the website; sections are themselves list of pages; ([source]
 (https://github.com/mkdocs/mkdocs/blob/master/mkdocs/structure/nav.py)) |
@@ -71,16 +71,16 @@
 {{ input('username') }}
 {{ input('password', type='password') }}
 ``` !!! Note All definitions will remain **local** to the page. It is possible
 to define Jinja2 macros in a separate file, and to import them from there in
 any page, using the `{% import ..}` directive. See explanations under [Advanced
 Usage](../advanced/#importing-macros-from-a-separate-file). Conditionals,
 loops, etc. ------------------------- With the macros plugin, you may use the
-[conditional](https://jinja.palletsprojects.com/en/2.11.x/templates/#if)
+[conditional](https://jinja.palletsprojects.com/en/3.0.x/templates/#if)
 statement of Jinja2, e.g. ``` {.jinja2} ### My title {% if == 'bar' %} We will
 write this **first version** {% else %} _Second version_ {% endif %} ``` You
 may produce Markdown or any mix of Markdown, HTML, css and even javascript that
 you wish. Similarly, you could use [for loops](https://
-jinja.palletsprojects.com/en/2.11.x/templates/#for): ``` {.jinja2} ### List of
+jinja.palletsprojects.com/en/3.0.x/templates/#for): ``` {.jinja2} ### List of
 users {% set users = ['joe', 'jill', 'david', 'sam'] %} {% for user in users %}
 1. {{ user }} {% endfor %} ``` In fact, you can do [all the fancy footwork you
 want with Jinja2](http://jinja.pocoo.org/docs/2.11/templates/)!
```

### Comparing `mkdocs-macros-plugin-0.7.0/webdoc/docs/pluglets.md` & `mkdocs-macros-plugin-1.0.1/webdoc/docs/pluglets.md`

 * *Files identical despite different names*

### Comparing `mkdocs-macros-plugin-0.7.0/webdoc/docs/tips.md` & `mkdocs-macros-plugin-1.0.1/webdoc/docs/tips.md`

 * *Files identical despite different names*

### Comparing `mkdocs-macros-plugin-0.7.0/webdoc/docs/troubleshooting.md` & `mkdocs-macros-plugin-1.0.1/webdoc/docs/troubleshooting.md`

 * *Files 18% similar despite different names*

```diff
@@ -6,56 +6,130 @@
 
 !!! Important
     Make sure you you have the **last version** of mkdocs-macros.
     Perhaps the issue is already fixed?
 
     Also, check that your version of mkdocs is sufficiently up-to-date.
 
+Error Information in case of module error
+-----------------------------------------
+
+By default a rendering error in a macro will not stop the server, 
+but display the error in the browser's page (as you would expect,
+e.g. with php). 
+The terminal's running log also displays errors when they occur.
+
+
+Is it possible to make the building process fail in case of page error?
+-----------------------------------------------------------
+Yes. In a context of CD/CI (Continuous Development/Continuous Integration)
+the generation of the mkdocs site can be part of a larger script.
+
+In that case, the expected behavior is _not_ to display the error message
+in the respective webpage (default behavior), 
+but to terminate the build process with an error code.
+That is the best way to advertise that something went wrong.
+
+It should then be possible to consult the log (console output)
+and track down the offending markdown file and line number.
+
+To activate that behavior, set the `on_error_fail` parameter to `true`
+in the config file:
+
+```yaml
+plugins:
+  - search
+  - macros:
+      # toggle to true if you are in CD/CI environment
+      on_error_fail: true
+```
+
+In that case, an error in a macro will terminate 
+the mkdocs-macros build or serve process with an **error 100**.
+
+!!! Tip "Make the behavior depend on an environment variable"
+
+    As of version 1.2, [mkdocs incorporates a yaml extension](https://www.mkdocs.org/user-guide/configuration/#environment-variables)
+    that allows the value of a configuration option to be set 
+    to the value of an environment variable.
 
-What happens if a variable or object is unknown?
+You could therefore write:
+
+```yaml
+plugins:
+    - search
+    - macros:
+        on_error_fail: !ENV [MACRO_ERROR_FAIL, false]
+```
+
+Meaning that the parameter "`on_error_fail` should be set to the value of 
+`MACRO_ERROR_FAIL`; or if the environment variable is absent to `false`.
+
+
+!!! Warning "Catching undefined variables"
+    By default, [an undefined variable](#what-happens-if-a-variable-is-undefined),
+    all by itself, does not cause an error, but leaves the jinja2
+    statement as-is (not rendered).
+
+    If you wish to raise an error also in that case, you may want to add:
+        
+            on_undefined: strict
+        
+
+
+What happens if a variable is undefined?
 --------------------------------------
 
-The default behavior is called **keep** (DebugUndefined):
+_New on 0.6.4._
+
+The default behavior in case of undefined variable 
+is called **keep** (DebugUndefined):
 
 1. Unknown variables are rendered as is (`{{ foobar }}` will be printed as such if 
   `foobar` is undefined).
-2. Any other cases (notably unknown attribute, function or object) will cause the page
-   to **fail** (be rendered with an error message plus the traceback).  
+2. Any other cases (notably unknown attribute or function call) will cause the page
+   to **fail** (be rendered with an error message within the page plus the traceback).  
 
-!!! Tip Compatibility with other plugins
+!!! Tip Motivations for default behavior
     There were two reasons for adopting this behavior:
     
-    1. This reduces cognitive overhead in case of misspelled variable.
+    1. This "debug" mode reduces cognitive overhead in case of misspelled variable.
        Anyone will be able to detect this error (it is better having an odd jinja2 statement 
        in the page than having a "blank" that is likely to go unnoticed) 
-    2. Other plugins than
-       mkdocs-macros make use of jinja2 variables (as specified in the config file). In this way, mkdocs-macros
-       will not "eat up" those variables and give other plugins a better chance to work.
+    2. Other plugins than mkdocs-macros make use of jinja2 variables 
+       (as specified in the config file).
+       In this way, mkdocs-macros will not "eat up" those variables; 
+       it will give other plugins a better chance to work.
 
 You may alter this behavior with the `on_undefined` parameter in mkdocs_macros 
 section of the config file (`mkdocs.yaml`):
 
-| Value  | Definition                                                                                   | Undefined Type                             |
-| ------ | -------------------------------------------------------------------------------------------- | ------------------------------------------ |
+| Value  | Definition        | Undefined Type                   |
+| ------ | -------------------------------- | ------------------------- |
 | keep   | (Default) Unknown variables are rendered as-is; all other cases will cause the page to fail. | DebugUndefined                             |
 | silent | Unknown variables are rendered as blank; all other cases will cause the page to fail.        | Undefined                                  |
 | strict | Anything incorrect will cause the page to fail (closest behavior to Python).                 | StrictUndefined                            |
 | lax    | Like silent (blank); will be more tolerant, typically in case of unknown attribute.          | LaxUndefined (_specific to mkdocs-macros_) |
 
+
+For example:
+
+```yaml
+plugins:
+  - search
+  - macros:
+      on_undefined: strict
+```
+
 !!! Warning
     A call to an unknown macro (callable) will always cause the page to fail.
 
 The Undefined Type is the Jinja2 class used to implement that behavior (see [definition in official documentation](https://jinja.palletsprojects.com/en/3.0.x/api/#undefined-types)).
 
-Error Information in case of module error
------------------------------------------
 
-In principle a rendering error in a macro will not stop the server, but
-display the error in the browser's page (as you would expect, e.g. with
-php). The terminal's running log also displays errors when they occur.
 
 `macros_info()` as the go-to tool
 ---------------------------------
 
 Adding following line in a page:
 
     {{ macros_info() }}
@@ -90,29 +164,30 @@
 
     {{ context() | pretty }}
 
 
 Help! mkdocs-macros is breaking down or eating pieces of my documentation!
 ------------------------------------------------
 
-!!! Note 
-    In principle, anything that looks like an unknown variable (e.g. `{{ foo }}`) will be preserved.
-    But in some cases there could be a broken page or  **an empty string where you expected one**.
+![dog eating ice-cream, credit: https://unsplash.com/photos/OYUzC-h1glg](dog-eating.jpg)
+
+1. In principle, anything that looks like an unknown variable (e.g. `{{ foo }}`) will be preserved.
+But in some cases there could be an error page or  **an empty string where you expected one**. [See how you can change the rendering behavior](#what-happens-if-a-variable-is-undefined).
 
-A likely cause to the problem is that mkdocs-macros is believing that statements
+2. Another likely cause of problems is that mkdocs-macros is believing that statements
 of the form `\{\{ .... }}` or `{% ... %}` 
-in your pages, which you want to appear in the HTML output or be processed by another plugin,
-are intended for it.
+in your pages, 
+which you want to appear in the HTML output or be processed by another plugin,
+are intended for it. To solve that problem, see the page 
+[dedicated to that issue](../rendering).
+
+
 
-![dog eating ice-cream, credit: https://unsplash.com/photos/OYUzC-h1glg](dog-eating.jpg)
 
 
-For the solutions to that problem, see 
-[how to prevent interpretation of Jinja-like
-statements](../advanced/#how-to-prevent-interpretation-of-jinja-like-statements).
 
 
 
 Traces on the console
 -------
 
 _From version 0.5.0_
@@ -220,40 +295,7 @@
     `mkdocs serve` (using the `--quiet` option),
     **this will also suppress the trace for your macros**.
 
     **This is intentional, so that the behavior of MkDocs's logging
     remains entirely predictable, even for people who
     never heard of mkdocs-macros (principle of least astonishment)**
 
-
-
-
-Where Can I get Help?
----------------------
-
-### Issues
-
-Check the [issues](https://github.com/fralau/mkdocs_macros_plugin/issues) 
-on the github repo.
-
-
-!!! Tip "Tips"
-
-    - Some issues have the marker **Useful Tip**.
-    - Also check the **closed issues**. It could be that your issue
-      has already been solved and closed!
-    - Also, you could check similar questions, to see if they could
-      point you to the right questions.
-
-
-If you want to add a new issue (for a bug or an enhancement request), 
-or comment on an existing one,
-you are more than welcome!
-
-All issues are carefully reviewed and often get a quick answer.
-
-### If all else fails...
-
-If you still have questions:
-
-- Check the Q&As 🙏 in the [project's Discussions space, on github](https://github.com/fralau/mkdocs_macros_plugin/discussions).
-- Post a Q&A 🙏 item!
```

### Comparing `mkdocs-macros-plugin-0.7.0/webdoc/docs/why.md` & `mkdocs-macros-plugin-1.0.1/webdoc/docs/why.md`

 * *Files identical despite different names*

### Comparing `mkdocs-macros-plugin-0.7.0/webdoc/mkdocs.yml` & `mkdocs-macros-plugin-1.0.1/webdoc/mkdocs.yml`

 * *Files 6% similar despite different names*

```diff
@@ -10,23 +10,25 @@
     - navigation.tabs
   palette:
     scheme: slate
     primary: teal
     accent: teal
 repo_url: https://github.com/fralau/mkdocs_macros_plugin
 edit_uri: edit/master/webdoc/docs/
-copyright: © Laurent Franceschetti, 2020. This work is licensed under CC BY-SA 4.0.
+copyright: © Laurent Franceschetti, 2023. This work is licensed under CC BY-SA 4.0.
 nav:
     - Home: index.md
     - 'User Guide': 
       - "Rich Markdown Pages": pages.md
       - "Git information": git_info.md
       - "Writing modules": macros.md
-      - Writing pluglets: pluglets.md
       - "Advanced usage": advanced.md
+      - Controlling macros rendering: rendering.md
+      - Post-production: post_production.md
+      - Writing pluglets: pluglets.md
     - Faq:
       - "Tips and Tricks": tips.md
       - "Troubleshooting": troubleshooting.md
       - "Asking for help?": help.md
     - Contributing: contribute.md
     - Changelog: changelog.md
     - About:
```

