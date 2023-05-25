# Comparing `tmp/starrail-toolkit-0.6.0.tar.gz` & `tmp/starrail-toolkit-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starrail-toolkit-0.6.0.tar", last modified: Mon May 22 18:25:03 2023, max compression
+gzip compressed data, was "starrail-toolkit-0.6.2.tar", last modified: Thu May 25 03:33:54 2023, max compression
```

## Comparing `starrail-toolkit-0.6.0.tar` & `starrail-toolkit-0.6.2.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-22 18:25:03.701978 starrail-toolkit-0.6.0/
--rw-r--r--   0 littlenyima   (501) staff       (20)    35149 2023-05-15 03:28:48.000000 starrail-toolkit-0.6.0/LICENSE
--rw-r--r--   0 littlenyima   (501) staff       (20)     5798 2023-05-22 18:25:03.701849 starrail-toolkit-0.6.0/PKG-INFO
--rw-r--r--   0 littlenyima   (501) staff       (20)     5291 2023-05-22 18:23:19.000000 starrail-toolkit-0.6.0/README.md
--rw-r--r--   0 littlenyima   (501) staff       (20)       38 2023-05-22 18:25:03.702013 starrail-toolkit-0.6.0/setup.cfg
--rw-r--r--   0 littlenyima   (501) staff       (20)     4153 2023-05-15 03:28:48.000000 starrail-toolkit-0.6.0/setup.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-22 18:25:03.695617 starrail-toolkit-0.6.0/starrail/
--rw-r--r--   0 littlenyima   (501) staff       (20)      760 2023-05-22 14:51:07.000000 starrail-toolkit-0.6.0/starrail/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     1838 2023-05-22 14:51:07.000000 starrail-toolkit-0.6.0/starrail/config.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-22 18:25:03.696058 starrail-toolkit-0.6.0/starrail/entry/
--rw-r--r--   0 littlenyima   (501) staff       (20)       49 2023-05-22 14:51:07.000000 starrail-toolkit-0.6.0/starrail/entry/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     3642 2023-05-22 18:23:19.000000 starrail-toolkit-0.6.0/starrail/entry/cli.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     1056 2023-05-22 18:23:19.000000 starrail-toolkit-0.6.0/starrail/entry/gui.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     1494 2023-05-22 14:51:07.000000 starrail-toolkit-0.6.0/starrail/entry/setup.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-22 18:25:03.697224 starrail-toolkit-0.6.0/starrail/gacha/
--rw-r--r--   0 littlenyima   (501) staff       (20)       49 2023-05-22 14:51:07.000000 starrail-toolkit-0.6.0/starrail/gacha/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     3549 2023-05-22 18:23:19.000000 starrail-toolkit-0.6.0/starrail/gacha/autodet.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     6599 2023-05-22 14:51:07.000000 starrail-toolkit-0.6.0/starrail/gacha/database.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     1134 2023-05-22 18:23:19.000000 starrail-toolkit-0.6.0/starrail/gacha/fetch.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     5178 2023-05-22 14:51:07.000000 starrail-toolkit-0.6.0/starrail/gacha/fileio.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     5092 2023-05-22 14:51:07.000000 starrail-toolkit-0.6.0/starrail/gacha/parse.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     4547 2023-05-22 14:51:07.000000 starrail-toolkit-0.6.0/starrail/gacha/service.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      501 2023-05-22 14:51:07.000000 starrail-toolkit-0.6.0/starrail/gacha/type.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     3489 2023-05-22 14:51:07.000000 starrail-toolkit-0.6.0/starrail/gacha/url.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-22 18:25:03.697445 starrail-toolkit-0.6.0/starrail/gui/
--rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-05-22 14:51:07.000000 starrail-toolkit-0.6.0/starrail/gui/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     6480 2023-05-22 18:23:19.000000 starrail-toolkit-0.6.0/starrail/gui/application.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-22 18:25:03.698090 starrail-toolkit-0.6.0/starrail/gui/common/
--rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-05-22 14:51:07.000000 starrail-toolkit-0.6.0/starrail/gui/common/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     1802 2023-05-22 18:23:19.000000 starrail-toolkit-0.6.0/starrail/gui/common/config.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      282 2023-05-22 18:23:19.000000 starrail-toolkit-0.6.0/starrail/gui/common/icon.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      611 2023-05-22 14:51:07.000000 starrail-toolkit-0.6.0/starrail/gui/common/stylesheet.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     1516 2023-05-22 14:51:07.000000 starrail-toolkit-0.6.0/starrail/gui/common/utils.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-22 18:25:03.698845 starrail-toolkit-0.6.0/starrail/gui/interfaces/
--rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-05-22 14:51:07.000000 starrail-toolkit-0.6.0/starrail/gui/interfaces/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     3713 2023-05-22 18:23:19.000000 starrail-toolkit-0.6.0/starrail/gui/interfaces/base.py
--rw-r--r--   0 littlenyima   (501) staff       (20)    13545 2023-05-22 18:23:19.000000 starrail-toolkit-0.6.0/starrail/gui/interfaces/gacha_sync.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     2536 2023-05-22 14:51:07.000000 starrail-toolkit-0.6.0/starrail/gui/interfaces/home.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     5635 2023-05-22 18:23:19.000000 starrail-toolkit-0.6.0/starrail/gui/interfaces/setting.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     4476 2023-05-22 18:23:19.000000 starrail-toolkit-0.6.0/starrail/gui/interfaces/unlock_fps.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      372 2023-05-22 14:51:07.000000 starrail-toolkit-0.6.0/starrail/gui/interfaces/users.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-22 18:25:03.699260 starrail-toolkit-0.6.0/starrail/gui/widgets/
--rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-05-22 14:51:07.000000 starrail-toolkit-0.6.0/starrail/gui/widgets/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     5438 2023-05-22 14:51:07.000000 starrail-toolkit-0.6.0/starrail/gui/widgets/dialog.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     2509 2023-05-22 14:51:07.000000 starrail-toolkit-0.6.0/starrail/gui/widgets/link_card.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     1841 2023-05-22 14:51:07.000000 starrail-toolkit-0.6.0/starrail/gui/widgets/title_bar.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-22 18:25:03.699578 starrail-toolkit-0.6.0/starrail/unlock/
--rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-05-22 18:23:19.000000 starrail-toolkit-0.6.0/starrail/unlock/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     2327 2023-05-22 18:23:19.000000 starrail-toolkit-0.6.0/starrail/unlock/fps.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      182 2023-05-22 18:23:19.000000 starrail-toolkit-0.6.0/starrail/unlock/service.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-22 18:25:03.700163 starrail-toolkit-0.6.0/starrail/utils/
--rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-05-22 14:51:07.000000 starrail-toolkit-0.6.0/starrail/utils/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     1832 2023-05-22 14:51:07.000000 starrail-toolkit-0.6.0/starrail/utils/accounts.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      948 2023-05-22 18:23:19.000000 starrail-toolkit-0.6.0/starrail/utils/auto_update.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-22 18:25:03.701001 starrail-toolkit-0.6.0/starrail/utils/babelfish/
--rw-r--r--   0 littlenyima   (501) staff       (20)     4292 2023-05-22 18:23:19.000000 starrail-toolkit-0.6.0/starrail/utils/babelfish/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      230 2023-05-22 14:51:07.000000 starrail-toolkit-0.6.0/starrail/utils/babelfish/constants.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     9255 2023-05-22 18:23:19.000000 starrail-toolkit-0.6.0/starrail/utils/babelfish/dictionary.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      504 2023-05-22 18:23:19.000000 starrail-toolkit-0.6.0/starrail/utils/babelfish/locale.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      586 2023-05-22 14:51:07.000000 starrail-toolkit-0.6.0/starrail/utils/babelfish/multilingual.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      165 2023-05-22 14:51:07.000000 starrail-toolkit-0.6.0/starrail/utils/babelfish/translate.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      551 2023-05-22 14:51:07.000000 starrail-toolkit-0.6.0/starrail/utils/loggings.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      144 2023-05-22 18:23:19.000000 starrail-toolkit-0.6.0/starrail/utils/misc.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      106 2023-05-22 18:23:19.000000 starrail-toolkit-0.6.0/starrail/version.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-22 18:25:03.701670 starrail-toolkit-0.6.0/starrail_toolkit.egg-info/
--rw-r--r--   0 littlenyima   (501) staff       (20)     5798 2023-05-22 18:25:03.000000 starrail-toolkit-0.6.0/starrail_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 littlenyima   (501) staff       (20)     1669 2023-05-22 18:25:03.000000 starrail-toolkit-0.6.0/starrail_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 littlenyima   (501) staff       (20)        1 2023-05-22 18:25:03.000000 starrail-toolkit-0.6.0/starrail_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 littlenyima   (501) staff       (20)       54 2023-05-22 18:25:03.000000 starrail-toolkit-0.6.0/starrail_toolkit.egg-info/entry_points.txt
--rw-r--r--   0 littlenyima   (501) staff       (20)       87 2023-05-22 18:25:03.000000 starrail-toolkit-0.6.0/starrail_toolkit.egg-info/requires.txt
--rw-r--r--   0 littlenyima   (501) staff       (20)        9 2023-05-22 18:25:03.000000 starrail-toolkit-0.6.0/starrail_toolkit.egg-info/top_level.txt
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-25 03:33:54.218711 starrail-toolkit-0.6.2/
+-rw-r--r--   0 littlenyima   (501) staff       (20)    35149 2023-05-15 03:28:48.000000 starrail-toolkit-0.6.2/LICENSE
+-rw-r--r--   0 littlenyima   (501) staff       (20)     5866 2023-05-25 03:33:54.218558 starrail-toolkit-0.6.2/PKG-INFO
+-rw-r--r--   0 littlenyima   (501) staff       (20)     5359 2023-05-25 03:32:23.000000 starrail-toolkit-0.6.2/README.md
+-rw-r--r--   0 littlenyima   (501) staff       (20)       38 2023-05-25 03:33:54.218752 starrail-toolkit-0.6.2/setup.cfg
+-rw-r--r--   0 littlenyima   (501) staff       (20)     4153 2023-05-15 03:28:48.000000 starrail-toolkit-0.6.2/setup.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-25 03:33:54.210619 starrail-toolkit-0.6.2/starrail/
+-rw-r--r--   0 littlenyima   (501) staff       (20)      760 2023-05-23 14:08:03.000000 starrail-toolkit-0.6.2/starrail/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     1838 2023-05-23 14:08:03.000000 starrail-toolkit-0.6.2/starrail/config.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-25 03:33:54.211212 starrail-toolkit-0.6.2/starrail/entry/
+-rw-r--r--   0 littlenyima   (501) staff       (20)       49 2023-05-23 14:08:03.000000 starrail-toolkit-0.6.2/starrail/entry/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     3650 2023-05-25 03:25:18.000000 starrail-toolkit-0.6.2/starrail/entry/cli.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     1056 2023-05-23 14:08:03.000000 starrail-toolkit-0.6.2/starrail/entry/gui.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     1494 2023-05-23 14:08:03.000000 starrail-toolkit-0.6.2/starrail/entry/setup.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-25 03:33:54.212605 starrail-toolkit-0.6.2/starrail/gacha/
+-rw-r--r--   0 littlenyima   (501) staff       (20)       49 2023-05-23 14:08:03.000000 starrail-toolkit-0.6.2/starrail/gacha/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     3549 2023-05-23 14:08:03.000000 starrail-toolkit-0.6.2/starrail/gacha/autodet.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     6599 2023-05-23 14:08:03.000000 starrail-toolkit-0.6.2/starrail/gacha/database.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     1134 2023-05-23 14:08:03.000000 starrail-toolkit-0.6.2/starrail/gacha/fetch.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     6513 2023-05-25 03:24:42.000000 starrail-toolkit-0.6.2/starrail/gacha/fileio.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     5097 2023-05-25 03:08:53.000000 starrail-toolkit-0.6.2/starrail/gacha/parse.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     4577 2023-05-25 03:29:28.000000 starrail-toolkit-0.6.2/starrail/gacha/service.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      501 2023-05-23 14:08:03.000000 starrail-toolkit-0.6.2/starrail/gacha/type.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     3489 2023-05-23 14:08:03.000000 starrail-toolkit-0.6.2/starrail/gacha/url.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-25 03:33:54.212948 starrail-toolkit-0.6.2/starrail/gui/
+-rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-05-23 14:08:03.000000 starrail-toolkit-0.6.2/starrail/gui/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     6480 2023-05-23 14:08:03.000000 starrail-toolkit-0.6.2/starrail/gui/application.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-25 03:33:54.213885 starrail-toolkit-0.6.2/starrail/gui/common/
+-rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-05-23 14:08:03.000000 starrail-toolkit-0.6.2/starrail/gui/common/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     1802 2023-05-23 14:08:03.000000 starrail-toolkit-0.6.2/starrail/gui/common/config.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      282 2023-05-23 14:08:03.000000 starrail-toolkit-0.6.2/starrail/gui/common/icon.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      611 2023-05-23 14:08:03.000000 starrail-toolkit-0.6.2/starrail/gui/common/stylesheet.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     1516 2023-05-23 14:08:03.000000 starrail-toolkit-0.6.2/starrail/gui/common/utils.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-25 03:33:54.215121 starrail-toolkit-0.6.2/starrail/gui/interfaces/
+-rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-05-23 14:08:03.000000 starrail-toolkit-0.6.2/starrail/gui/interfaces/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     3713 2023-05-23 14:08:03.000000 starrail-toolkit-0.6.2/starrail/gui/interfaces/base.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)    13725 2023-05-25 03:30:12.000000 starrail-toolkit-0.6.2/starrail/gui/interfaces/gacha_sync.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     2536 2023-05-23 14:08:03.000000 starrail-toolkit-0.6.2/starrail/gui/interfaces/home.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     5635 2023-05-23 14:08:03.000000 starrail-toolkit-0.6.2/starrail/gui/interfaces/setting.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     4476 2023-05-23 14:08:03.000000 starrail-toolkit-0.6.2/starrail/gui/interfaces/unlock_fps.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      372 2023-05-23 14:08:03.000000 starrail-toolkit-0.6.2/starrail/gui/interfaces/users.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-25 03:33:54.215708 starrail-toolkit-0.6.2/starrail/gui/widgets/
+-rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-05-23 14:08:03.000000 starrail-toolkit-0.6.2/starrail/gui/widgets/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     5438 2023-05-23 14:08:03.000000 starrail-toolkit-0.6.2/starrail/gui/widgets/dialog.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     2509 2023-05-23 14:08:03.000000 starrail-toolkit-0.6.2/starrail/gui/widgets/link_card.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     1841 2023-05-23 14:08:03.000000 starrail-toolkit-0.6.2/starrail/gui/widgets/title_bar.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-25 03:33:54.216102 starrail-toolkit-0.6.2/starrail/unlock/
+-rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-05-23 14:08:03.000000 starrail-toolkit-0.6.2/starrail/unlock/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     2327 2023-05-23 14:08:03.000000 starrail-toolkit-0.6.2/starrail/unlock/fps.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      182 2023-05-23 14:08:03.000000 starrail-toolkit-0.6.2/starrail/unlock/service.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-25 03:33:54.216763 starrail-toolkit-0.6.2/starrail/utils/
+-rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-05-23 14:08:03.000000 starrail-toolkit-0.6.2/starrail/utils/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     1804 2023-05-25 03:28:51.000000 starrail-toolkit-0.6.2/starrail/utils/accounts.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      948 2023-05-23 14:08:03.000000 starrail-toolkit-0.6.2/starrail/utils/auto_update.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-25 03:33:54.217596 starrail-toolkit-0.6.2/starrail/utils/babelfish/
+-rw-r--r--   0 littlenyima   (501) staff       (20)     4292 2023-05-23 14:08:03.000000 starrail-toolkit-0.6.2/starrail/utils/babelfish/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      230 2023-05-23 14:08:03.000000 starrail-toolkit-0.6.2/starrail/utils/babelfish/constants.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     9255 2023-05-23 14:08:03.000000 starrail-toolkit-0.6.2/starrail/utils/babelfish/dictionary.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      597 2023-05-23 14:08:03.000000 starrail-toolkit-0.6.2/starrail/utils/babelfish/locale.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      765 2023-05-23 14:08:03.000000 starrail-toolkit-0.6.2/starrail/utils/babelfish/multilingual.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      165 2023-05-23 14:08:03.000000 starrail-toolkit-0.6.2/starrail/utils/babelfish/translate.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      551 2023-05-23 14:08:03.000000 starrail-toolkit-0.6.2/starrail/utils/loggings.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      144 2023-05-23 14:08:03.000000 starrail-toolkit-0.6.2/starrail/utils/misc.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      106 2023-05-25 03:31:36.000000 starrail-toolkit-0.6.2/starrail/version.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-25 03:33:54.218376 starrail-toolkit-0.6.2/starrail_toolkit.egg-info/
+-rw-r--r--   0 littlenyima   (501) staff       (20)     5866 2023-05-25 03:33:54.000000 starrail-toolkit-0.6.2/starrail_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 littlenyima   (501) staff       (20)     1669 2023-05-25 03:33:54.000000 starrail-toolkit-0.6.2/starrail_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 littlenyima   (501) staff       (20)        1 2023-05-25 03:33:54.000000 starrail-toolkit-0.6.2/starrail_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 littlenyima   (501) staff       (20)       54 2023-05-25 03:33:54.000000 starrail-toolkit-0.6.2/starrail_toolkit.egg-info/entry_points.txt
+-rw-r--r--   0 littlenyima   (501) staff       (20)       87 2023-05-25 03:33:54.000000 starrail-toolkit-0.6.2/starrail_toolkit.egg-info/requires.txt
+-rw-r--r--   0 littlenyima   (501) staff       (20)        9 2023-05-25 03:33:54.000000 starrail-toolkit-0.6.2/starrail_toolkit.egg-info/top_level.txt
```

### Comparing `starrail-toolkit-0.6.0/LICENSE` & `starrail-toolkit-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.6.0/PKG-INFO` & `starrail-toolkit-0.6.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starrail-toolkit
-Version: 0.6.0
+Version: 0.6.2
 Summary: Honkai Star Rail Toolkit
 Home-page: https://github.com/LittleNyima/honkai-starrail-toolkit
 Author: LittleNyima
 Author-email: littlenyima@163.com
 License: GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -21,21 +21,23 @@
 
 <b><i>有一说一，现在的界面有点太丑了，在改了在改了</i></b>
 
 ## 开发状态
 
 | 主分支版本 | 开发分支版本 | PyPI 版本 | 发行版版本 |
 | :--------: | :----------: | :-------: | :--------: |
-|   0.6.0    |    0.6.0     |   0.6.0   |   0.6.0    |
+|   0.6.0    |    0.6.2     |   0.6.2   |   0.6.0    |
 
 目前第一阶段开发已完成，历史开发计划见[该页面](docs/history-dev-plan.md)。
 
 - [x] 支持更多的可设置选项
 - [ ] 支持国际服
 - [x] 支持解锁120帧
+- [x] 支持以 SRGF 标准导出
+- [ ] 支持以 SRGF 标准导入
 - [ ] 支持手动设置 API URL
 - [x] 支持夜间模式
 - [ ] 支持多用户切换
 - [ ] 美化程序界面
 
 ## 常见问题解答
```

### Comparing `starrail-toolkit-0.6.0/README.md` & `starrail-toolkit-0.6.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -6,21 +6,23 @@
 
 <b><i>有一说一，现在的界面有点太丑了，在改了在改了</i></b>
 
 ## 开发状态
 
 | 主分支版本 | 开发分支版本 | PyPI 版本 | 发行版版本 |
 | :--------: | :----------: | :-------: | :--------: |
-|   0.6.0    |    0.6.0     |   0.6.0   |   0.6.0    |
+|   0.6.0    |    0.6.2     |   0.6.2   |   0.6.0    |
 
 目前第一阶段开发已完成，历史开发计划见[该页面](docs/history-dev-plan.md)。
 
 - [x] 支持更多的可设置选项
 - [ ] 支持国际服
 - [x] 支持解锁120帧
+- [x] 支持以 SRGF 标准导出
+- [ ] 支持以 SRGF 标准导入
 - [ ] 支持手动设置 API URL
 - [x] 支持夜间模式
 - [ ] 支持多用户切换
 - [ ] 美化程序界面
 
 ## 常见问题解答
```

### Comparing `starrail-toolkit-0.6.0/setup.py` & `starrail-toolkit-0.6.2/setup.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.6.0/starrail/__init__.py` & `starrail-toolkit-0.6.2/starrail/__init__.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.6.0/starrail/config.py` & `starrail-toolkit-0.6.2/starrail/config.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.6.0/starrail/entry/cli.py` & `starrail-toolkit-0.6.2/starrail/entry/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     gacha = subparsers.add_parser('gacha')
     gacha.add_argument(
         '--api', type=str,
         help='URL of the gacha api, please refer to README.md for details.',
     )
     gacha.add_argument(
         '--export', nargs='+', type=str, default=['all'],
-        choices=['all', 'csv', 'html', 'json', 'md', 'xlsx'],
+        choices=['all', 'csv', 'html', 'json', 'md', 'srgf', 'xlsx'],
         help='Types of expected export formats.',
     )
     gacha.add_argument(
         '--request-interval', type=float, default=0.1,
         help='Minimum interval (seconds) between two requests.',
     )
```

### Comparing `starrail-toolkit-0.6.0/starrail/entry/gui.py` & `starrail-toolkit-0.6.2/starrail/entry/gui.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.6.0/starrail/entry/setup.py` & `starrail-toolkit-0.6.2/starrail/entry/setup.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.6.0/starrail/gacha/autodet.py` & `starrail-toolkit-0.6.2/starrail/gacha/autodet.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.6.0/starrail/gacha/database.py` & `starrail-toolkit-0.6.2/starrail/gacha/database.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.6.0/starrail/gacha/fetch.py` & `starrail-toolkit-0.6.2/starrail/gacha/fetch.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.6.0/starrail/gacha/fileio.py` & `starrail-toolkit-0.6.2/starrail/gacha/fileio.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import json
+import time
 
 import pandas as pd
 
+import starrail
 import starrail.utils.babelfish as babelfish
 from starrail.gacha.database import DatabaseFactory
 from starrail.gacha.parse import GachaDataManager
 from starrail.gacha.type import GachaType
 from starrail.utils import loggings
 
 logger = loggings.get_logger(__file__)
@@ -119,7 +121,44 @@
     )
     html = (
         f'<html lang="zh"><head><title>{title}</title><meta charset="UTF-8">'
         f'{style}</head><body>{content}</body></html>'
     )
     with open(output_path, 'w', encoding='utf-8') as fout:
         fout.write(html)
+
+
+def export_as_srgf(manager: GachaDataManager, output_path: str) -> None:
+    gacha_list = []
+    for gacha_type in GachaType:
+        gacha_list.extend(manager.gacha[gacha_type.value].tolist())
+    gacha_list.sort(key=lambda x: x['id'])
+    uid = gacha_list[0]['uid'] if gacha_list else manager.uid
+    lang = gacha_list[0]['lang'] if gacha_list else 'zh-cn'
+    timezone = time.localtime().tm_gmtoff // 3600
+    timestamp = int(time.time())
+    data = dict(
+        info=dict(
+            uid=uid,
+            lang=lang,
+            region_time_zone=timezone,
+            export_timestamp=timestamp,
+            export_app='StarRailToolkit',
+            export_app_version=starrail.__version__,
+            srgf_version='v1.0',
+        ),
+        list=[
+            dict(
+                gacha_id=item['gacha_id'],
+                gacha_type=item['gacha_type'],
+                item_id=item['item_id'],
+                count=item['count'],
+                time=item['time'],
+                name=item['name'],
+                item_type=item['item_type'],
+                rank_type=item['rank_type'],
+                id=item['id'],
+            ) for item in gacha_list
+        ],
+    )
+    with open(output_path, 'w', encoding='utf-8') as fout:
+        json.dump(data, fout, indent=2, ensure_ascii=False)
```

### Comparing `starrail-toolkit-0.6.0/starrail/gacha/parse.py` & `starrail-toolkit-0.6.2/starrail/gacha/parse.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,15 +94,15 @@
             average=f'{(total_items - since_last) / count:.2f}',
         )
 
 
 class GachaDataManager:
 
     def __init__(self, uid):
-        self.uid = uid
+        self.uid: str = uid
         self.gacha = self.load_cache(uid)
 
     def load_cache(self, uid: str):
         db_dir = cfg.db_dir
         self.cache_path = os.path.join(db_dir, f'{uid}.sqlite3')
         if os.path.isfile(self.cache_path):
             return parse_cache_from_sql(self.cache_path)
```

### Comparing `starrail-toolkit-0.6.0/starrail/gacha/service.py` & `starrail-toolkit-0.6.2/starrail/gacha/service.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import json
 import os
 import time
-from datetime import datetime
 
 import starrail.gacha.fileio as fileio
 from starrail.gacha.autodet import detect_api_url
 from starrail.gacha.fetch import fetch_json
 from starrail.gacha.parse import GachaDataManager
 from starrail.gacha.type import GachaType
 from starrail.gacha.url import get_api_url, get_url_template
@@ -120,18 +119,20 @@
         csv=fileio.export_as_csv,
         html=fileio.export_as_html,
         json=fileio.export_as_json,
         md=fileio.export_as_md,
         xlsx=fileio.export_as_xlsx,
     )
     if 'all' in export:
-        export = ['csv', 'html', 'json', 'md', 'xlsx']
+        export = ['csv', 'html', 'json', 'md', 'srgf', 'xlsx']
 
-    timestamp = datetime.now().strftime('%Y%m%d%H%M%S')
+    timestamp = time.strftime('%Y%m%d%H%M%S')
 
     for format in export:
+        if format == 'srgf':
+            format = 'srgf.json'
         logger.info(f'Exporting gacha data as {format} format')
         output_dir = os.getcwd()
         filename = f'HKSR-export-{uid}-{timestamp}.{format}'
         path = os.path.join(output_dir, filename)
         export_hooks[format](manager, path)
         logger.info(f'Gacha data in {format} format is saved to {path}')
```

### Comparing `starrail-toolkit-0.6.0/starrail/gacha/url.py` & `starrail-toolkit-0.6.2/starrail/gacha/url.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.6.0/starrail/gui/application.py` & `starrail-toolkit-0.6.2/starrail/gui/application.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.6.0/starrail/gui/common/config.py` & `starrail-toolkit-0.6.2/starrail/gui/common/config.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.6.0/starrail/gui/common/stylesheet.py` & `starrail-toolkit-0.6.2/starrail/gui/common/stylesheet.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.6.0/starrail/gui/common/utils.py` & `starrail-toolkit-0.6.2/starrail/gui/common/utils.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.6.0/starrail/gui/interfaces/base.py` & `starrail-toolkit-0.6.2/starrail/gui/interfaces/base.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.6.0/starrail/gui/interfaces/gacha_sync.py` & `starrail-toolkit-0.6.2/starrail/gui/interfaces/gacha_sync.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,18 +125,22 @@
     def run(self):
         manager = service.GachaDataManager(self.uid)
         export_hooks = dict(
             csv=service.fileio.export_as_csv,
             html=service.fileio.export_as_html,
             json=service.fileio.export_as_json,
             md=service.fileio.export_as_md,
+            srgf=service.fileio.export_as_srgf,
             xlsx=service.fileio.export_as_xlsx,
         )
+        timestamp = time.strftime('%Y%m%d%H%M%S')
         for format, hook in export_hooks.items():
-            filename = f'HKSR-export-{self.uid}.{format}'
+            if format == 'srgf':
+                format = 'srgf.json'
+            filename = f'HKSR-export-{self.uid}-{timestamp}.{format}'
             export_path = os.path.join(self.path, filename)
             hook(manager, export_path)
         self.saveSuccessSignal.emit(self.path)
 
 
 class ResultTableWidget(QtWidgets.QWidget):
```

### Comparing `starrail-toolkit-0.6.0/starrail/gui/interfaces/home.py` & `starrail-toolkit-0.6.2/starrail/gui/interfaces/home.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.6.0/starrail/gui/interfaces/setting.py` & `starrail-toolkit-0.6.2/starrail/gui/interfaces/setting.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.6.0/starrail/gui/interfaces/unlock_fps.py` & `starrail-toolkit-0.6.2/starrail/gui/interfaces/unlock_fps.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.6.0/starrail/gui/widgets/dialog.py` & `starrail-toolkit-0.6.2/starrail/gui/widgets/dialog.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.6.0/starrail/gui/widgets/link_card.py` & `starrail-toolkit-0.6.2/starrail/gui/widgets/link_card.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.6.0/starrail/gui/widgets/title_bar.py` & `starrail-toolkit-0.6.2/starrail/gui/widgets/title_bar.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.6.0/starrail/unlock/fps.py` & `starrail-toolkit-0.6.2/starrail/unlock/fps.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.6.0/starrail/utils/accounts.py` & `starrail-toolkit-0.6.2/starrail/utils/accounts.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import json
 import os
-from datetime import datetime
+import time
 
 from starrail.config import configuration as cfg
 from starrail.utils import babelfish
 
 
 def todict(d, keys):
     return {k: d[k] for k in d if k in keys}
@@ -35,15 +35,15 @@
         with open(self._path, 'w', encoding='utf-8') as f:
             json.dump(
                 dict(meta=self.meta, accounts=self.accounts), f,
                 ensure_ascii=False, indent=2,
             )
 
     def update_timestamp(self, uid):
-        timestamp = datetime.now().strftime(babelfish.constants.TIME_FMT)
+        timestamp = time.strftime(babelfish.constants.TIME_FMT)
         if uid in self.accounts:
             self.accounts[uid]['last_update'] = timestamp
         else:
             self.accounts[uid] = dict(last_update=timestamp)
         self.meta['latest'] = uid
         self.flush()
```

### Comparing `starrail-toolkit-0.6.0/starrail/utils/auto_update.py` & `starrail-toolkit-0.6.2/starrail/utils/auto_update.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.6.0/starrail/utils/babelfish/__init__.py` & `starrail-toolkit-0.6.2/starrail/utils/babelfish/__init__.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.6.0/starrail/utils/babelfish/dictionary.py` & `starrail-toolkit-0.6.2/starrail/utils/babelfish/dictionary.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.6.0/starrail/utils/babelfish/multilingual.py` & `starrail-toolkit-0.6.2/starrail/utils/babelfish/multilingual.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,19 +2,26 @@
 
 from starrail.utils.babelfish.locale import Locale
 from starrail.utils.loggings import get_logger
 
 logger = get_logger(__file__)
 
 
+locale_fallback = ['zhs', 'en']
+
+
 class MultilingualString:
 
     def __init__(self, **kwargs: str):
         self.mapping: Dict[str, str] = dict()
         for key, value in kwargs.items():
             if key not in Locale.available_lang:
                 logger.warn(f'{key} is not a valid language')
             self.mapping[key] = value
 
     def __call__(self, *args, **kwargs):
         lang = Locale.lang
+        if lang not in self.mapping:
+            for lang in locale_fallback:
+                if lang in self.mapping:
+                    break
         return self.mapping[lang].format(*args, **kwargs)
```

### Comparing `starrail-toolkit-0.6.0/starrail/utils/loggings.py` & `starrail-toolkit-0.6.2/starrail/utils/loggings.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.6.0/starrail_toolkit.egg-info/PKG-INFO` & `starrail-toolkit-0.6.2/starrail_toolkit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starrail-toolkit
-Version: 0.6.0
+Version: 0.6.2
 Summary: Honkai Star Rail Toolkit
 Home-page: https://github.com/LittleNyima/honkai-starrail-toolkit
 Author: LittleNyima
 Author-email: littlenyima@163.com
 License: GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -21,21 +21,23 @@
 
 <b><i>有一说一，现在的界面有点太丑了，在改了在改了</i></b>
 
 ## 开发状态
 
 | 主分支版本 | 开发分支版本 | PyPI 版本 | 发行版版本 |
 | :--------: | :----------: | :-------: | :--------: |
-|   0.6.0    |    0.6.0     |   0.6.0   |   0.6.0    |
+|   0.6.0    |    0.6.2     |   0.6.2   |   0.6.0    |
 
 目前第一阶段开发已完成，历史开发计划见[该页面](docs/history-dev-plan.md)。
 
 - [x] 支持更多的可设置选项
 - [ ] 支持国际服
 - [x] 支持解锁120帧
+- [x] 支持以 SRGF 标准导出
+- [ ] 支持以 SRGF 标准导入
 - [ ] 支持手动设置 API URL
 - [x] 支持夜间模式
 - [ ] 支持多用户切换
 - [ ] 美化程序界面
 
 ## 常见问题解答
```

### Comparing `starrail-toolkit-0.6.0/starrail_toolkit.egg-info/SOURCES.txt` & `starrail-toolkit-0.6.2/starrail_toolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

