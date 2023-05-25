# Comparing `tmp/Subsearch-2.34.0rc1.tar.gz` & `tmp/Subsearch-2.35.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Subsearch-2.34.0rc1.tar", last modified: Mon May  8 15:46:32 2023, max compression
+gzip compressed data, was "Subsearch-2.35.0rc1.tar", last modified: Thu May 25 13:09:46 2023, max compression
```

## Comparing `Subsearch-2.34.0rc1.tar` & `Subsearch-2.35.0rc1.tar`

### file list

```diff
@@ -1,113 +1,112 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:46:32.860054 Subsearch-2.34.0rc1/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7970 2023-05-08 15:46:32.860054 Subsearch-2.34.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7202 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 15:46:32.860054 Subsearch-2.34.0rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:46:32.844054 Subsearch-2.34.0rc1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:46:32.848054 Subsearch-2.34.0rc1/src/Subsearch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7970 2023-05-08 15:46:32.000000 Subsearch-2.34.0rc1/src/Subsearch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-05-08 15:46:32.000000 Subsearch-2.34.0rc1/src/Subsearch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 15:46:32.000000 Subsearch-2.34.0rc1/src/Subsearch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-08 15:46:32.000000 Subsearch-2.34.0rc1/src/Subsearch.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 15:46:32.000000 Subsearch-2.34.0rc1/src/Subsearch.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-08 15:46:32.000000 Subsearch-2.34.0rc1/src/Subsearch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-08 15:46:32.000000 Subsearch-2.34.0rc1/src/Subsearch.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:46:32.848054 Subsearch-2.34.0rc1/src/subsearch/
--rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9476 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:46:32.852054 Subsearch-2.34.0rc1/src/subsearch/data/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/data/application_config.json
--rw-r--r--   0 runner    (1001) docker     (123)     9139 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/data/data_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/data/guid.py
--rw-r--r--   0 runner    (1001) docker     (123)     7597 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/data/languages.json
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/data/set_data.py
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/data/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:46:32.852054 Subsearch-2.34.0rc1/src/subsearch/gui/
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:46:32.852054 Subsearch-2.34.0rc1/src/subsearch/gui/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:46:32.852054 Subsearch-2.34.0rc1/src/subsearch/gui/assets/btn/
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/assets/btn/btn_disabled.png
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/assets/btn/btn_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/assets/btn/btn_pressed.png
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/assets/btn/btn_rest.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:46:32.856054 Subsearch-2.34.0rc1/src/subsearch/gui/assets/checkbox/
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/assets/checkbox/check_disabled.png
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/assets/checkbox/check_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/assets/checkbox/check_pressed.png
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/assets/checkbox/check_rest.png
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/assets/checkbox/check_tri_disabled.png
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/assets/checkbox/check_tri_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/assets/checkbox/check_tri_pressed.png
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/assets/checkbox/check_tri_rest.png
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/assets/checkbox/check_unsel_disabled.png
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/assets/checkbox/check_unsel_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/assets/checkbox/check_unsel_pressed.png
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/assets/checkbox/check_unsel_rest.png
--rw-r--r--   0 runner    (1001) docker     (123)     5379 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/assets/dark.tcl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:46:32.856054 Subsearch-2.34.0rc1/src/subsearch/gui/assets/icon/
--rw-r--r--   0 runner    (1001) docker     (123)   105808 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/assets/icon/subsearch.ico
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/assets/icon/subsearch.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:46:32.856054 Subsearch-2.34.0rc1/src/subsearch/gui/assets/scale/
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/assets/scale/scale_thumb_disabled.png
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/assets/scale/scale_thumb_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/assets/scale/scale_thumb_pressed.png
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/assets/scale/scale_thumb_rest.png
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/assets/scale/scale_trough_hor.png
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/assets/scale/scale_trough_vert.png
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/assets/scale/separator.png
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/assets/scale/sizegrip.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:46:32.856054 Subsearch-2.34.0rc1/src/subsearch/gui/assets/scrollbar/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/assets/scrollbar/scroll_down.png
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/assets/scrollbar/scroll_hor_thumb.png
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/assets/scrollbar/scroll_hor_trough.png
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/assets/scrollbar/scroll_left.png
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/assets/scrollbar/scroll_right.png
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/assets/scrollbar/scroll_up.png
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/assets/scrollbar/scroll_vert_thumb.png
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/assets/scrollbar/scroll_vert_trough.png
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/assets/scrollbar/separator.png
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/assets/scrollbar/sizegrip.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:46:32.856054 Subsearch-2.34.0rc1/src/subsearch/gui/assets/tabs/
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/assets/tabs/download_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/assets/tabs/download_press.png
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/assets/tabs/download_rest.png
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/assets/tabs/language_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/assets/tabs/language_press.png
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/assets/tabs/language_rest.png
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/assets/tabs/search_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/assets/tabs/search_press.png
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/assets/tabs/search_rest.png
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/assets/tabs/settings_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/assets/tabs/settings_press.png
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/assets/tabs/settings_rest.png
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/assets/ttk_style.tcl
--rw-r--r--   0 runner    (1001) docker     (123)     9105 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/tab_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:46:32.860054 Subsearch-2.34.0rc1/src/subsearch/gui/tabs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/tabs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/tabs/dowload_tab.py
--rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/tabs/language_tab.py
--rw-r--r--   0 runner    (1001) docker     (123)     9346 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/tabs/search_tab.py
--rw-r--r--   0 runner    (1001) docker     (123)     8108 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/tabs/settings_tab.py
--rw-r--r--   0 runner    (1001) docker     (123)    13667 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/gui/tkinter_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:46:32.860054 Subsearch-2.34.0rc1/src/subsearch/providers/
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5830 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/providers/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/providers/opensubtitles.py
--rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/providers/subscene.py
--rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/providers/yifysubtitles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:46:32.860054 Subsearch-2.34.0rc1/src/subsearch/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6197 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/utils/file_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/utils/imdb_lookup.py
--rw-r--r--   0 runner    (1001) docker     (123)     5636 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/utils/io_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/utils/io_winreg.py
--rw-r--r--   0 runner    (1001) docker     (123)     7224 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/utils/mutex_synchronizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11259 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/utils/string_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-05-08 15:46:17.000000 Subsearch-2.34.0rc1/src/subsearch/utils/updates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:09:46.184146 Subsearch-2.35.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-25 13:09:23.000000 Subsearch-2.35.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-25 13:09:23.000000 Subsearch-2.35.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7970 2023-05-25 13:09:46.184146 Subsearch-2.35.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7202 2023-05-25 13:09:23.000000 Subsearch-2.35.0rc1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-05-25 13:09:23.000000 Subsearch-2.35.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 13:09:46.184146 Subsearch-2.35.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-05-25 13:09:23.000000 Subsearch-2.35.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:09:46.164146 Subsearch-2.35.0rc1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:09:46.168146 Subsearch-2.35.0rc1/src/Subsearch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7970 2023-05-25 13:09:46.000000 Subsearch-2.35.0rc1/src/Subsearch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-05-25 13:09:46.000000 Subsearch-2.35.0rc1/src/Subsearch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 13:09:46.000000 Subsearch-2.35.0rc1/src/Subsearch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-25 13:09:46.000000 Subsearch-2.35.0rc1/src/Subsearch.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 13:09:45.000000 Subsearch-2.35.0rc1/src/Subsearch.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-25 13:09:46.000000 Subsearch-2.35.0rc1/src/Subsearch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-25 13:09:46.000000 Subsearch-2.35.0rc1/src/Subsearch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:09:46.168146 Subsearch-2.35.0rc1/src/subsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-05-25 13:09:23.000000 Subsearch-2.35.0rc1/src/subsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 13:09:23.000000 Subsearch-2.35.0rc1/src/subsearch/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9672 2023-05-25 13:09:23.000000 Subsearch-2.35.0rc1/src/subsearch/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:09:46.172146 Subsearch-2.35.0rc1/src/subsearch/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-25 13:09:23.000000 Subsearch-2.35.0rc1/src/subsearch/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-05-25 13:09:23.000000 Subsearch-2.35.0rc1/src/subsearch/data/data_initializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9637 2023-05-25 13:09:23.000000 Subsearch-2.35.0rc1/src/subsearch/data/data_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-25 13:09:23.000000 Subsearch-2.35.0rc1/src/subsearch/data/guid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7597 2023-05-25 13:09:23.000000 Subsearch-2.35.0rc1/src/subsearch/data/languages.json
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-25 13:09:23.000000 Subsearch-2.35.0rc1/src/subsearch/data/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:09:46.172146 Subsearch-2.35.0rc1/src/subsearch/gui/
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-05-25 13:09:23.000000 Subsearch-2.35.0rc1/src/subsearch/gui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:09:46.172146 Subsearch-2.35.0rc1/src/subsearch/gui/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:09:46.172146 Subsearch-2.35.0rc1/src/subsearch/gui/assets/btn/
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-25 13:09:23.000000 Subsearch-2.35.0rc1/src/subsearch/gui/assets/btn/btn_disabled.png
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-25 13:09:23.000000 Subsearch-2.35.0rc1/src/subsearch/gui/assets/btn/btn_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-25 13:09:23.000000 Subsearch-2.35.0rc1/src/subsearch/gui/assets/btn/btn_pressed.png
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-25 13:09:23.000000 Subsearch-2.35.0rc1/src/subsearch/gui/assets/btn/btn_rest.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:09:46.176146 Subsearch-2.35.0rc1/src/subsearch/gui/assets/checkbox/
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-25 13:09:23.000000 Subsearch-2.35.0rc1/src/subsearch/gui/assets/checkbox/check_disabled.png
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-25 13:09:23.000000 Subsearch-2.35.0rc1/src/subsearch/gui/assets/checkbox/check_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-25 13:09:23.000000 Subsearch-2.35.0rc1/src/subsearch/gui/assets/checkbox/check_pressed.png
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-25 13:09:23.000000 Subsearch-2.35.0rc1/src/subsearch/gui/assets/checkbox/check_rest.png
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-25 13:09:23.000000 Subsearch-2.35.0rc1/src/subsearch/gui/assets/checkbox/check_tri_disabled.png
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-25 13:09:23.000000 Subsearch-2.35.0rc1/src/subsearch/gui/assets/checkbox/check_tri_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-25 13:09:23.000000 Subsearch-2.35.0rc1/src/subsearch/gui/assets/checkbox/check_tri_pressed.png
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-25 13:09:23.000000 Subsearch-2.35.0rc1/src/subsearch/gui/assets/checkbox/check_tri_rest.png
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-25 13:09:23.000000 Subsearch-2.35.0rc1/src/subsearch/gui/assets/checkbox/check_unsel_disabled.png
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-25 13:09:23.000000 Subsearch-2.35.0rc1/src/subsearch/gui/assets/checkbox/check_unsel_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-25 13:09:23.000000 Subsearch-2.35.0rc1/src/subsearch/gui/assets/checkbox/check_unsel_pressed.png
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-25 13:09:23.000000 Subsearch-2.35.0rc1/src/subsearch/gui/assets/checkbox/check_unsel_rest.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5379 2023-05-25 13:09:23.000000 Subsearch-2.35.0rc1/src/subsearch/gui/assets/dark.tcl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:09:46.176146 Subsearch-2.35.0rc1/src/subsearch/gui/assets/icon/
+-rw-r--r--   0 runner    (1001) docker     (123)   105808 2023-05-25 13:09:23.000000 Subsearch-2.35.0rc1/src/subsearch/gui/assets/icon/subsearch.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-25 13:09:23.000000 Subsearch-2.35.0rc1/src/subsearch/gui/assets/icon/subsearch.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:09:46.176146 Subsearch-2.35.0rc1/src/subsearch/gui/assets/scale/
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-25 13:09:23.000000 Subsearch-2.35.0rc1/src/subsearch/gui/assets/scale/scale_thumb_disabled.png
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-25 13:09:23.000000 Subsearch-2.35.0rc1/src/subsearch/gui/assets/scale/scale_thumb_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-25 13:09:23.000000 Subsearch-2.35.0rc1/src/subsearch/gui/assets/scale/scale_thumb_pressed.png
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-25 13:09:23.000000 Subsearch-2.35.0rc1/src/subsearch/gui/assets/scale/scale_thumb_rest.png
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-25 13:09:23.000000 Subsearch-2.35.0rc1/src/subsearch/gui/assets/scale/scale_trough_hor.png
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-25 13:09:23.000000 Subsearch-2.35.0rc1/src/subsearch/gui/assets/scale/scale_trough_vert.png
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-25 13:09:23.000000 Subsearch-2.35.0rc1/src/subsearch/gui/assets/scale/separator.png
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-25 13:09:23.000000 Subsearch-2.35.0rc1/src/subsearch/gui/assets/scale/sizegrip.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:09:46.180146 Subsearch-2.35.0rc1/src/subsearch/gui/assets/scrollbar/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-25 13:09:23.000000 Subsearch-2.35.0rc1/src/subsearch/gui/assets/scrollbar/scroll_down.png
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-25 13:09:23.000000 Subsearch-2.35.0rc1/src/subsearch/gui/assets/scrollbar/scroll_hor_thumb.png
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-25 13:09:23.000000 Subsearch-2.35.0rc1/src/subsearch/gui/assets/scrollbar/scroll_hor_trough.png
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-25 13:09:23.000000 Subsearch-2.35.0rc1/src/subsearch/gui/assets/scrollbar/scroll_left.png
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-25 13:09:23.000000 Subsearch-2.35.0rc1/src/subsearch/gui/assets/scrollbar/scroll_right.png
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-25 13:09:23.000000 Subsearch-2.35.0rc1/src/subsearch/gui/assets/scrollbar/scroll_up.png
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-25 13:09:23.000000 Subsearch-2.35.0rc1/src/subsearch/gui/assets/scrollbar/scroll_vert_thumb.png
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-25 13:09:23.000000 Subsearch-2.35.0rc1/src/subsearch/gui/assets/scrollbar/scroll_vert_trough.png
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-25 13:09:23.000000 Subsearch-2.35.0rc1/src/subsearch/gui/assets/scrollbar/separator.png
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-25 13:09:23.000000 Subsearch-2.35.0rc1/src/subsearch/gui/assets/scrollbar/sizegrip.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:09:46.180146 Subsearch-2.35.0rc1/src/subsearch/gui/assets/tabs/
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-25 13:09:23.000000 Subsearch-2.35.0rc1/src/subsearch/gui/assets/tabs/download_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-05-25 13:09:23.000000 Subsearch-2.35.0rc1/src/subsearch/gui/assets/tabs/download_press.png
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-25 13:09:23.000000 Subsearch-2.35.0rc1/src/subsearch/gui/assets/tabs/download_rest.png
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-25 13:09:23.000000 Subsearch-2.35.0rc1/src/subsearch/gui/assets/tabs/language_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-25 13:09:23.000000 Subsearch-2.35.0rc1/src/subsearch/gui/assets/tabs/language_press.png
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-25 13:09:23.000000 Subsearch-2.35.0rc1/src/subsearch/gui/assets/tabs/language_rest.png
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-25 13:09:23.000000 Subsearch-2.35.0rc1/src/subsearch/gui/assets/tabs/search_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-25 13:09:23.000000 Subsearch-2.35.0rc1/src/subsearch/gui/assets/tabs/search_press.png
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-25 13:09:23.000000 Subsearch-2.35.0rc1/src/subsearch/gui/assets/tabs/search_rest.png
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-25 13:09:23.000000 Subsearch-2.35.0rc1/src/subsearch/gui/assets/tabs/settings_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-25 13:09:23.000000 Subsearch-2.35.0rc1/src/subsearch/gui/assets/tabs/settings_press.png
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-25 13:09:23.000000 Subsearch-2.35.0rc1/src/subsearch/gui/assets/tabs/settings_rest.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-05-25 13:09:23.000000 Subsearch-2.35.0rc1/src/subsearch/gui/assets/ttk_style.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)     9156 2023-05-25 13:09:23.000000 Subsearch-2.35.0rc1/src/subsearch/gui/tab_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:09:46.180146 Subsearch-2.35.0rc1/src/subsearch/gui/tabs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 13:09:23.000000 Subsearch-2.35.0rc1/src/subsearch/gui/tabs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-05-25 13:09:23.000000 Subsearch-2.35.0rc1/src/subsearch/gui/tabs/dowload_tab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-05-25 13:09:23.000000 Subsearch-2.35.0rc1/src/subsearch/gui/tabs/language_tab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9397 2023-05-25 13:09:23.000000 Subsearch-2.35.0rc1/src/subsearch/gui/tabs/search_tab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7251 2023-05-25 13:09:23.000000 Subsearch-2.35.0rc1/src/subsearch/gui/tabs/settings_tab.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13667 2023-05-25 13:09:23.000000 Subsearch-2.35.0rc1/src/subsearch/gui/tkinter_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:09:46.184146 Subsearch-2.35.0rc1/src/subsearch/providers/
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-05-25 13:09:23.000000 Subsearch-2.35.0rc1/src/subsearch/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5591 2023-05-25 13:09:23.000000 Subsearch-2.35.0rc1/src/subsearch/providers/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4102 2023-05-25 13:09:23.000000 Subsearch-2.35.0rc1/src/subsearch/providers/opensubtitles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-05-25 13:09:23.000000 Subsearch-2.35.0rc1/src/subsearch/providers/subscene.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-05-25 13:09:23.000000 Subsearch-2.35.0rc1/src/subsearch/providers/yifysubtitles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:09:46.184146 Subsearch-2.35.0rc1/src/subsearch/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-05-25 13:09:23.000000 Subsearch-2.35.0rc1/src/subsearch/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-05-25 13:09:23.000000 Subsearch-2.35.0rc1/src/subsearch/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6042 2023-05-25 13:09:23.000000 Subsearch-2.35.0rc1/src/subsearch/utils/file_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-05-25 13:09:23.000000 Subsearch-2.35.0rc1/src/subsearch/utils/imdb_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5763 2023-05-25 13:09:23.000000 Subsearch-2.35.0rc1/src/subsearch/utils/io_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-05-25 13:09:23.000000 Subsearch-2.35.0rc1/src/subsearch/utils/io_winreg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7249 2023-05-25 13:09:23.000000 Subsearch-2.35.0rc1/src/subsearch/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-25 13:09:23.000000 Subsearch-2.35.0rc1/src/subsearch/utils/mutex_synchronizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11259 2023-05-25 13:09:23.000000 Subsearch-2.35.0rc1/src/subsearch/utils/string_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3185 2023-05-25 13:09:23.000000 Subsearch-2.35.0rc1/src/subsearch/utils/update.py
```

### Comparing `Subsearch-2.34.0rc1/LICENSE` & `Subsearch-2.35.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `Subsearch-2.34.0rc1/PKG-INFO` & `Subsearch-2.35.0rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Subsearch
-Version: 2.34.0rc1
+Version: 2.35.0rc1
 Summary: Download subtitles for movies and shows, automatically with one easy mouse click.
 Author: vagabondHustler
 Author-email: vagabondHustler.github@gmail.com
 License: MIT license
 Project-URL: repository, https://github.com/vagabondHustler/subsearch
 Keywords: subsearch,subscene,opensubtitles,yifysubtitles,download,subtitles,movies,shows,automatically,scrape
 Platform: win32
```

### Comparing `Subsearch-2.34.0rc1/README.md` & `Subsearch-2.35.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `Subsearch-2.34.0rc1/pyproject.toml` & `Subsearch-2.35.0rc1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     "Programming Language :: Python :: 3.11",
     "Operating System :: Microsoft :: Windows",
     "Topic :: Multimedia :: Video",
     "Topic :: Utilities",
     "Intended Audience :: Developers",
     "Intended Audience :: End Users/Desktop"
 ]
-dependencies = ["selectolax==0.3.13", "cloudscraper==1.2.71", "num2words==0.5.12", "packaging==23.1", "requests==2.30.0"]
+dependencies = ["selectolax==0.3.13", "cloudscraper==1.2.71", "num2words==0.5.12", "packaging==23.1", "requests==2.31.0"]
 dynamic = ["version"]
 
 [project.urls]
 repository = "https://github.com/vagabondHustler/subsearch"
 
 [project.scripts]
 subsearch = "subsearch:main"
@@ -40,16 +40,16 @@
 include = ["subsearch*"]
 exclude = ["examples*", "tools*", "subsearch.test*"]
 
 [tool.setuptools.dynamic]
 version = {attr = "subsearch.data.__version__"}
 
 [project.optional-dependencies]
-optional = ["black==23.3.0", "isort==5.12.0", "twine==4.0.2", "build==0.10.0", "cx_Freeze==6.14.9", "mypy==1.2.0", "pipreqs==0.4.13"]
-dev = ["pytest==7.3.1", "pytest-cov==4.0.0", "tox==4.5.1"]
+optional = ["black==23.3.0", "isort==5.12.0", "twine==4.0.2", "build==0.10.0", "cx_Freeze==6.15.0", "mypy==1.3.0", "pipreqs==0.4.13"]
+dev = ["pytest==7.3.1", "pytest-cov==4.1.0", "tox==4.5.1"]
 
 
 [tool.pytest.ini_options]
 filterwarnings =[
     'ignore::DeprecationWarning'
 ]
 log_cli = true
```

### Comparing `Subsearch-2.34.0rc1/setup.py` & `Subsearch-2.35.0rc1/setup.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.34.0rc1/src/Subsearch.egg-info/PKG-INFO` & `Subsearch-2.35.0rc1/src/Subsearch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Subsearch
-Version: 2.34.0rc1
+Version: 2.35.0rc1
 Summary: Download subtitles for movies and shows, automatically with one easy mouse click.
 Author: vagabondHustler
 Author-email: vagabondHustler.github@gmail.com
 License: MIT license
 Project-URL: repository, https://github.com/vagabondHustler/subsearch
 Keywords: subsearch,subscene,opensubtitles,yifysubtitles,download,subtitles,movies,shows,automatically,scrape
 Platform: win32
```

### Comparing `Subsearch-2.34.0rc1/src/Subsearch.egg-info/SOURCES.txt` & `Subsearch-2.35.0rc1/src/Subsearch.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -10,19 +10,18 @@
 src/Subsearch.egg-info/not-zip-safe
 src/Subsearch.egg-info/requires.txt
 src/Subsearch.egg-info/top_level.txt
 src/subsearch/__init__.py
 src/subsearch/__main__.py
 src/subsearch/core.py
 src/subsearch/data/__init__.py
-src/subsearch/data/application_config.json
+src/subsearch/data/data_initializer.py
 src/subsearch/data/data_objects.py
 src/subsearch/data/guid.py
 src/subsearch/data/languages.json
-src/subsearch/data/set_data.py
 src/subsearch/data/version.py
 src/subsearch/gui/__init__.py
 src/subsearch/gui/tab_manager.py
 src/subsearch/gui/tkinter_utils.py
 src/subsearch/gui/assets/dark.tcl
 src/subsearch/gui/assets/ttk_style.tcl
 src/subsearch/gui/assets/btn/btn_disabled.png
@@ -88,8 +87,8 @@
 src/subsearch/utils/file_manager.py
 src/subsearch/utils/imdb_lookup.py
 src/subsearch/utils/io_json.py
 src/subsearch/utils/io_winreg.py
 src/subsearch/utils/log.py
 src/subsearch/utils/mutex_synchronizer.py
 src/subsearch/utils/string_parser.py
-src/subsearch/utils/updates.py
+src/subsearch/utils/update.py
```

### Comparing `Subsearch-2.34.0rc1/src/subsearch/__init__.py` & `Subsearch-2.35.0rc1/src/subsearch/__init__.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.34.0rc1/src/subsearch/core.py` & `Subsearch-2.35.0rc1/src/subsearch/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 import ctypes
 import time
 
-from subsearch.data import __version__, video_data
-from subsearch.data.data_objects import DownloadMetaData, FormattedMetadata
+from subsearch.data import __version__, app_paths, video_data
+from subsearch.data.data_objects import DownloadData, PrettifiedDownloadData
 from subsearch.gui import tab_manager
 from subsearch.providers import opensubtitles, subscene, yifysubtitles
 from subsearch.utils import file_manager, io_json, io_winreg, log, string_parser
 
 
 class Initializer:
     def __init__(self) -> None:
+        file_manager.create_directory(app_paths.appdata_local)
+        file_manager.create_directory(app_paths.tmpdir)
+        io_json.create_application_config()
         self.app_config = io_json.get_app_config()
         if video_data is not None:
+            file_manager.create_directory(video_data.subs_directory)
             self.file_exist = True
             self.file_hash = file_manager.get_hash(video_data.file_path)
         else:
             self.file_exist = False
             self.file_hash = ""
-        self.results: dict[str, list[DownloadMetaData]] = {}
-        self.skipped_downloads: dict[str, list[FormattedMetadata]] = {}
-        self.skipped_combined: list[FormattedMetadata] = []
+        self.results: dict[str, list[DownloadData]] = {}
+        self.skipped_downloads: dict[str, list[PrettifiedDownloadData]] = {}
+        self.skipped_combined: list[PrettifiedDownloadData] = []
         self.downloads: dict[str, int] = {}
         self.language_data = io_json.get_language_data()
 
         for provider in self.app_config.providers.keys():
             self.results[provider] = []
             self.skipped_downloads[provider] = []
             self.downloads[provider] = 0
@@ -52,31 +56,30 @@
             and self.app_config.providers["opensubtitles_site"] is False
             and self.app_config.providers["opensubtitles_hash"] is False
             and self.app_config.providers["yifysubtitles_site"] is False
         ):
             return True
         return False
 
-    def download_results(self, results: list[DownloadMetaData]) -> int:
+    def download_results(self, results: list[DownloadData]) -> int:
         for result in results:
             downloads = file_manager.download_subtitle(result)
         return downloads
 
 
 class AppSteps(Initializer):
     def __init__(self) -> None:
         self.start = time.perf_counter()
         Initializer.__init__(self)
         ctypes.windll.kernel32.SetConsoleTitleW(f"subsearch - {__version__}")
         if io_winreg.registry_key_exists() is False and io_json.get_json_key("context_menu"):
-            io_json.set_default_json()
+            io_json.create_application_config()
             io_winreg.add_context_menu()
         if io_winreg.registry_key_exists() and io_winreg.key_no_value() and io_json.get_json_key("context_menu"):
             io_winreg.add_context_menu()
-        file_manager.make_necessary_directories()
         if self.file_exist is False:
             tab_manager.open_tab("search")
             return None
 
         if " " in video_data.filename:
             log.warning_spaces_in_filename()
         log.output_header("Search started")
@@ -132,28 +135,28 @@
             self.ran_download_tab = True
         log.output_done_with_tasks(end_new_line=True)
 
     def _extract_zip_files(self) -> None:
         if self.skip_step.extract_zip():
             return None
         log.output_header("Extracting downloads")
-        file_manager.extract_files(video_data.tmp_directory, video_data.subs_directory, ".zip")
+        file_manager.extract_files(app_paths.tmpdir, video_data.subs_directory, ".zip")
         log.output_done_with_tasks(end_new_line=True)
 
     def _clean_up(self) -> None:
         if self.file_exist is False:
             return None
         if self.app_config.rename_best_match:
             log.output_header("Renaming best match")
             file_manager.rename_best_match(f"{self.release_data.release}.srt", video_data.directory_path, ".srt")
             log.output_done_with_tasks(end_new_line=True)
 
         log.output_header("Cleaning up")
         file_manager.clean_up_files(video_data.subs_directory, "nfo")
-        file_manager.del_directory(video_data.tmp_directory)
+        file_manager.delete_temp_files(app_paths.tmpdir)
         if file_manager.directory_is_empty(video_data.subs_directory):
             file_manager.del_directory(video_data.subs_directory)
         log.output_done_with_tasks(end_new_line=True)
 
     def _pre_exit(self) -> None:
         elapsed = time.perf_counter() - self.start
         log.output(f"Finished in {elapsed} seconds")
```

### Comparing `Subsearch-2.34.0rc1/src/subsearch/data/data_objects.py` & `Subsearch-2.35.0rc1/src/subsearch/data/data_objects.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,23 +25,27 @@
         home (Path): The root directory of the application.
         data (Path): The directory where data related to the application is stored.
         gui (Path): The directory containing GUI modules and files.
         providers (Path): The directory containing subtitle provider modules.
         utils (Path): The directory containing utility modules.
         icon (Path): The Path object representing the icon for the application.
         tabs (Path): The directory containing tab icon assets for the GUI.
+        tmpdir(Path): The directory containing temporary files & folders.
+        appdata_local(Path): The directory containing the persistent application files.
     """
 
     home: Path
     data: Path
     gui: Path
     providers: Path
     utils: Path
     icon: Path
     tabs: Path
+    tmpdir: Path
+    appdata_local: Path
 
 
 @dataclass(order=True)
 class FileData:
     """
      Class representing file information.
 
@@ -148,15 +152,15 @@
     subscene: str
     opensubtitles: str
     opensubtitles_hash: str
     yifysubtitles: str
 
 
 @dataclass(frozen=True, order=True)
-class DownloadMetaData:
+class DownloadData:
     """
     A data class representing metadata for the to be downloaded subtitle file.
 
     Attributes:
         provider (str): The subtitle provider used to obtain the subtitle file.
         name (str): The name of the media file associated with the subtitle file.
         file_path (str): The path to the subtitle file on the local filesystem.
@@ -170,17 +174,17 @@
     file_path: str
     url: str
     idx_num: int
     idx_lenght: int
 
 
 @dataclass(frozen=True, order=True)
-class FormattedMetadata:
+class PrettifiedDownloadData:
     """
-    Represents formatted metadata for a movie or TV show release.
+    Represents prettified version of DownloadData.
 
     Attributes:
         provider (str): The name of the metadata provider.
         release (str): The name of the movie or TV show release.
         url (str): The URL from which the subtitle file can be downloaded from.
         pct_result (int): The percentage match between the search query and
             the metadata.
@@ -301,7 +305,25 @@
     size = GUISizes
     pos = GUIPositions
     fonts = GUIFonts
     colors = GUIColors
 
 
 GUI_DATA = GUIData()
+
+SUPPORTED_FILE_EXTENSIONS = [
+    ".avi",
+    ".mp4",
+    ".mkv",
+    ".mpg",
+    ".mpeg",
+    ".mov",
+    ".rm",
+    ".vob",
+    ".wmv",
+    ".flv",
+    ".3gp",
+    ".3g2",
+    ".swf",
+    ".mswmm",
+]
+SUPPORTED_PROVIDERS = ["subscene_site", "opensubtitles_site", "opensubtitles_hash", "yifysubtitles_site"]
```

### Comparing `Subsearch-2.34.0rc1/src/subsearch/data/languages.json` & `Subsearch-2.35.0rc1/src/subsearch/data/languages.json`

 * *Files identical despite different names*

### Comparing `Subsearch-2.34.0rc1/src/subsearch/gui/__init__.py` & `Subsearch-2.35.0rc1/src/subsearch/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.34.0rc1/src/subsearch/gui/assets/dark.tcl` & `Subsearch-2.35.0rc1/src/subsearch/gui/assets/dark.tcl`

 * *Files identical despite different names*

### Comparing `Subsearch-2.34.0rc1/src/subsearch/gui/assets/icon/subsearch.ico` & `Subsearch-2.35.0rc1/src/subsearch/gui/assets/icon/subsearch.ico`

 * *Files identical despite different names*

### Comparing `Subsearch-2.34.0rc1/src/subsearch/gui/assets/scale/scale_thumb_disabled.png` & `Subsearch-2.35.0rc1/src/subsearch/gui/assets/scale/scale_thumb_disabled.png`

 * *Files identical despite different names*

### Comparing `Subsearch-2.34.0rc1/src/subsearch/gui/assets/scale/scale_thumb_hover.png` & `Subsearch-2.35.0rc1/src/subsearch/gui/assets/scale/scale_thumb_hover.png`

 * *Files identical despite different names*

### Comparing `Subsearch-2.34.0rc1/src/subsearch/gui/assets/scale/scale_thumb_pressed.png` & `Subsearch-2.35.0rc1/src/subsearch/gui/assets/scale/scale_thumb_pressed.png`

 * *Files identical despite different names*

### Comparing `Subsearch-2.34.0rc1/src/subsearch/gui/assets/scale/scale_thumb_rest.png` & `Subsearch-2.35.0rc1/src/subsearch/gui/assets/scale/scale_thumb_rest.png`

 * *Files identical despite different names*

### Comparing `Subsearch-2.34.0rc1/src/subsearch/gui/assets/tabs/download_hover.png` & `Subsearch-2.35.0rc1/src/subsearch/gui/assets/tabs/download_hover.png`

 * *Files identical despite different names*

### Comparing `Subsearch-2.34.0rc1/src/subsearch/gui/assets/tabs/download_press.png` & `Subsearch-2.35.0rc1/src/subsearch/gui/assets/tabs/download_press.png`

 * *Files identical despite different names*

### Comparing `Subsearch-2.34.0rc1/src/subsearch/gui/assets/tabs/download_rest.png` & `Subsearch-2.35.0rc1/src/subsearch/gui/assets/tabs/download_rest.png`

 * *Files identical despite different names*

### Comparing `Subsearch-2.34.0rc1/src/subsearch/gui/assets/tabs/search_hover.png` & `Subsearch-2.35.0rc1/src/subsearch/gui/assets/tabs/search_hover.png`

 * *Files identical despite different names*

### Comparing `Subsearch-2.34.0rc1/src/subsearch/gui/assets/tabs/search_press.png` & `Subsearch-2.35.0rc1/src/subsearch/gui/assets/tabs/search_press.png`

 * *Files identical despite different names*

### Comparing `Subsearch-2.34.0rc1/src/subsearch/gui/assets/tabs/search_rest.png` & `Subsearch-2.35.0rc1/src/subsearch/gui/assets/tabs/search_rest.png`

 * *Files identical despite different names*

### Comparing `Subsearch-2.34.0rc1/src/subsearch/gui/assets/tabs/settings_hover.png` & `Subsearch-2.35.0rc1/src/subsearch/gui/assets/tabs/settings_hover.png`

 * *Files identical despite different names*

### Comparing `Subsearch-2.34.0rc1/src/subsearch/gui/assets/tabs/settings_press.png` & `Subsearch-2.35.0rc1/src/subsearch/gui/assets/tabs/settings_press.png`

 * *Files identical despite different names*

### Comparing `Subsearch-2.34.0rc1/src/subsearch/gui/assets/tabs/settings_rest.png` & `Subsearch-2.35.0rc1/src/subsearch/gui/assets/tabs/settings_rest.png`

 * *Files identical despite different names*

### Comparing `Subsearch-2.34.0rc1/src/subsearch/gui/assets/ttk_style.tcl` & `Subsearch-2.35.0rc1/src/subsearch/gui/assets/ttk_style.tcl`

 * *Files identical despite different names*

### Comparing `Subsearch-2.34.0rc1/src/subsearch/gui/tab_manager.py` & `Subsearch-2.35.0rc1/src/subsearch/gui/tab_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import tkinter as tk
 from typing import Any
 
-from subsearch.data import GUI_DATA, app_paths
-from subsearch.data.data_objects import FormattedMetadata
+from subsearch.data import GUI_DATA, __version__, app_paths
+from subsearch.data.data_objects import PrettifiedDownloadData
 from subsearch.gui import set_theme, tkinter_utils
 from subsearch.gui.tabs import dowload_tab, language_tab, search_tab, settings_tab
 from subsearch.utils import file_manager, io_json, io_winreg
 
 
 class TabManager(tk.Frame):
     """
@@ -57,15 +57,15 @@
         tkinter_utils.set_default_grid_size(self)
         self.active_tab = active_tab
         self.activate_tabs()
 
     def activate_tabs(self) -> None:
         self.tabs[self.active_tab].place(x=GUI_DATA.pos.content_x, y=GUI_DATA.pos.content_y, anchor="center")
         tkinter_utils.asset_tab(self.buttons[self.active_tab], self.active_tab, "press")
-        self.parent.title(f"Subsearch - {self.active_tab} tab")
+        self.parent.title(f"Subsearch {__version__} - {self.active_tab} tab")
 
     def release_tab(self, event) -> None:
         btn_key, _btn_widget = self.get_btn(self.buttons, event)
         self.active_tab = btn_key
         self.activate_tabs()
         self.deactivate_tabs()
 
@@ -132,15 +132,15 @@
         if file_manager.running_from_exe() is False:
             settings_tab.ShowTerminalOnSearch(self).pack(anchor="center")
         tk.Frame(self, height=20, bg=GUI_DATA.colors.dark_grey).pack(anchor="center", expand=True)
         settings_tab.CheckForUpdates(self).pack(anchor="center")
 
 
 class TabDownload(tk.Frame):
-    def __init__(self, parent, formatted_data: list[FormattedMetadata]) -> None:
+    def __init__(self, parent, formatted_data: list[PrettifiedDownloadData]) -> None:
         tk.Frame.__init__(self, parent, width=GUI_DATA.size.root_width, height=GUI_DATA.size.root_height)
         self.configure(bg=GUI_DATA.colors.dark_grey)
         dowload_tab.DownloadList(self, formatted_data).pack(anchor="center")
 
 
 def open_tab(active_tab: str, **kwargs) -> None:
     """
@@ -151,15 +151,15 @@
         **kwargs: Arbitrary keyword arguments that should contain "formatted_data",
                   a list of FormattedMetadata.
 
     Returns:
         None: This function does not return anything, it manipulates the GUI instead.
     """
     try:
-        formatted_data: list[FormattedMetadata] = kwargs["formatted_data"]
+        formatted_data: list[PrettifiedDownloadData] = kwargs["formatted_data"]
     except KeyError:
         formatted_data = None  # type: ignore
     root = initalize_root()
     set_theme("dark")
     tkinter_utils.set_custom_btn_styles()
     tabs = {
         "language": TabLanguage(root),
@@ -179,15 +179,15 @@
     If `io_winreg.registry_key_exists()` is `False` and `raw_json.get_config_key("context_menu")` is `True`,
     the default JSON configuration is set using `raw_json.set_default_json()` and a context menu is added to the registry using `io_winreg.add_context_menu()`.
 
     Returns:
       An instance of Tk() class representing the main window of Subsearch application.
     """
     if io_winreg.registry_key_exists() is False and io_json.get_json_key("context_menu"):
-        io_json.set_default_json()
+        io_json.create_application_config()
         io_winreg.add_context_menu()
     root = tk.Tk(className=f"Subsearch")
     root.configure(background=GUI_DATA.colors.dark_grey)
     root.iconbitmap(app_paths.icon)
     root.geometry(tkinter_utils.WindowPosition.set(root))  # type: ignore
     root.resizable(False, False)
     return root
```

### Comparing `Subsearch-2.34.0rc1/src/subsearch/gui/tabs/dowload_tab.py` & `Subsearch-2.35.0rc1/src/subsearch/gui/tabs/dowload_tab.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 import re
 import tkinter as tk
 from tkinter import ttk
 
-from subsearch.data import GUI_DATA, video_data
-from subsearch.data.data_objects import DownloadMetaData, FormattedMetadata
+from subsearch.data import GUI_DATA, app_paths, video_data
+from subsearch.data.data_objects import DownloadData, PrettifiedDownloadData
 from subsearch.providers import subscene
 from subsearch.utils import file_manager, log
 
 
 class DownloadList(tk.Frame):
-    def __init__(self, parent, formatted_data: list[FormattedMetadata]) -> None:
+    def __init__(self, parent, formatted_data: list[PrettifiedDownloadData]) -> None:
         tk.Frame.__init__(self, parent)
         root_posx, root_posy = parent.winfo_reqwidth(), parent.winfo_reqheight()
         self.configure(bg=GUI_DATA.colors.dark_grey, width=root_posx, height=root_posy - 82)
-        # listbox for the subtitles
         if formatted_data is not None:
             formatted_data.sort(key=lambda x: x.pct_result, reverse=True)
         self.formatted_data = formatted_data
         self.subscene_scrape = subscene.SubsceneScraper()
         self.extent = 0
-        # self.sublist = read_tmp_file()
         self.scrollbar = ttk.Scrollbar(self, orient="vertical", style="Vertical.TScrollbar")
         self.sub_listbox = tk.Listbox(
             self,
             height=root_posy,
             bg=GUI_DATA.colors.dark_grey,
             fg=GUI_DATA.colors.light_grey,
             font=GUI_DATA.fonts.cas8b,
@@ -82,23 +80,23 @@
             if enum != int(item_num):
                 continue
             self.sub_listbox.itemconfig(int(enum), {"fg": GUI_DATA.colors.blue})
             if _provider == "subscene":
                 download_url = self.subscene_scrape.get_download_url(_url)
             else:
                 download_url = _url
-            path = f"{video_data.tmp_directory}\\__{_provider}__{item_num}.zip"
-            enum = DownloadMetaData(
+            path = f"{ app_paths.tmpdir}\\__{_provider}__{item_num}.zip"
+            enum = DownloadData(
                 provider=f"Downloading from {_provider}",
                 name=_release,
                 file_path=path,
                 url=download_url,
                 idx_num=1,
                 idx_lenght=1,
             )  # type: ignore
             file_manager.download_subtitle(enum)  # type: ignore
-            file_manager.extract_files(video_data.tmp_directory, video_data.subs_directory, ".zip")
-            file_manager.clean_up_files(video_data.tmp_directory, "zip")
+            file_manager.extract_files(app_paths.tmpdir, video_data.subs_directory, ".zip")
+            file_manager.delete_temp_files(app_paths.tmpdir)
             break
         self.sub_listbox.delete(int(item_num))
         self.sub_listbox.insert(int(item_num), f"✔ {_release}")
         self.sub_listbox.itemconfig(int(item_num), {"fg": GUI_DATA.colors.green})
```

### Comparing `Subsearch-2.34.0rc1/src/subsearch/gui/tabs/language_tab.py` & `Subsearch-2.35.0rc1/src/subsearch/gui/tabs/language_tab.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.34.0rc1/src/subsearch/gui/tabs/search_tab.py` & `Subsearch-2.35.0rc1/src/subsearch/gui/tabs/search_tab.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,29 @@
 import tkinter as tk
 from tkinter import ttk
 
 from subsearch.data import GUI_DATA
 from subsearch.gui import tkinter_utils
 from subsearch.utils import io_json
 
-SUBTILE_TYPE = io_json.get_json_key("subtitle_type")
-PERCENTAGE_THRESHOLD = io_json.get_json_key("percentage_threshold")
-PROVIDERS = io_json.get_json_key("providers")
-
 
 class Providers(tk.Frame):
     def __init__(self, parent) -> None:
         tk.Frame.__init__(self, parent)
         self.configure(bg=GUI_DATA.colors.dark_grey)
+        self.providers = io_json.get_json_key("providers")
         self.data = io_json.get_json_data()
         label = tk.Label(self, text="Search providers")
         label.configure(bg=GUI_DATA.colors.dark_grey, fg=GUI_DATA.colors.white_grey, font=GUI_DATA.fonts.cas8b)
         label.grid(row=1, column=0, sticky="w", padx=2, pady=2)
         self.rownum = 0
         self.colnum = 2
         self.checkbox_value = {}
         self.last_key = ""
-        for key, value in PROVIDERS.items():
+        for key, value in self.providers.items():
             btn_txt = key.split("_")[-1].capitalize()
             lbl_txt = f"{key.split('_')[0]}".capitalize()
             valuevar = tk.BooleanVar()
             valuevar.set(value)
             if self.last_key.startswith(lbl_txt):
                 self.colnum += 1
             if self.last_key != lbl_txt:
@@ -65,46 +62,47 @@
         btn = event.widget
         key = self.checkbox_value[btn][0]
         value = self.checkbox_value[btn][1]
         if value.get() is True:
             self.data["providers"][key] = False
         elif value.get() is False:
             self.data["providers"][key] = True
-        io_json.set_config(self.data)
+        io_json.set_json_data(self.data)
 
     def toggle_providers(self, event) -> None:
         btn = event.widget
         key = btn["text"].replace(" ", "_").lower()
         if self.data["providers"][key] is True:
             self.data["providers"][key] = False
             btn.configure(fg=GUI_DATA.colors.red)
         elif self.data["providers"][key] is False:
             self.data["providers"][key] = True
             btn.configure(fg=GUI_DATA.colors.green)
-        io_json.set_config(self.data)
+        io_json.set_json_data(self.data)
 
 
 class SubtitleType(tk.Frame):
     def __init__(self, parent) -> None:
         tk.Frame.__init__(self, parent)
         self.configure(bg=GUI_DATA.colors.dark_grey)
+        self.subtitle_type = io_json.get_json_key("subtitle_type")
         self.string_var = tk.StringVar()
         self.data = io_json.get_json_data()
         label = tk.Label(self, text="Subtitle type")
         label.configure(bg=GUI_DATA.colors.dark_grey, fg=GUI_DATA.colors.white_grey, font=GUI_DATA.fonts.cas8b)
         label.grid(row=1, column=0, sticky="w", padx=2, pady=2)
         self.clabel = tk.Label(self, textvariable=self.string_var)
         self.clabel.configure(bg=GUI_DATA.colors.dark_grey, font=GUI_DATA.fonts.cas8b)
         self.clabel.grid(row=1, column=1, sticky="nsew", padx=2, pady=2)
         self.sub_type_txt()
         tkinter_utils.VarColorPicker(self.string_var, self.clabel)
         self.rownum = 0
         self.colnum = 2
         self.checkbox_values = {}
-        for key, value in SUBTILE_TYPE.items():
+        for key, value in self.subtitle_type.items():
             if key.startswith("non"):
                 _text = "Regular"
             else:
                 _text = key.replace("_", " ").title()
             valuevar = tk.BooleanVar()
             valuevar.set(value)
             self.rownum += 1
@@ -130,15 +128,15 @@
         btn = event.widget
         key = self.checkbox_values[btn][0]
         value = self.checkbox_values[btn][1]
         if value.get() is True:
             self.data["subtitle_type"][key] = False
         elif value.get() is False:
             self.data["subtitle_type"][key] = True
-        io_json.set_config(self.data)
+        io_json.set_json_data(self.data)
         self.sub_type_txt()
 
     def sub_type_txt(self) -> None:
         hi_sub = self.data["subtitle_type"]["hearing_impaired"]
         nonhi_sub = self.data["subtitle_type"]["non_hearing_impaired"]
         if (hi_sub and nonhi_sub) or (hi_sub is False and nonhi_sub is False):
             self.string_var.set(f"Both")
@@ -149,18 +147,19 @@
         tkinter_utils.VarColorPicker(self.string_var, self.clabel)
 
 
 class SearchThreshold(tk.Frame):
     def __init__(self, parent) -> None:
         tk.Frame.__init__(self, parent)
         self.configure(bg=GUI_DATA.colors.dark_grey)
+        self.pct_threashold = io_json.get_json_key("percentage_threshold")
         self.current_value = tk.IntVar()
-        self.current_value.set(PERCENTAGE_THRESHOLD)
+        self.current_value.set(self.pct_threashold)
         self.string_var = tk.StringVar()
-        self.string_var.set(f"{PERCENTAGE_THRESHOLD} %")
+        self.string_var.set(f"{self.pct_threashold} %")
         label = tk.Label(self, text="Search threshold")
         label.configure(bg=GUI_DATA.colors.dark_grey, fg=GUI_DATA.colors.white_grey, font=GUI_DATA.fonts.cas8b)
         label.grid(row=0, column=0, sticky="w", padx=0, pady=2)
         self.clabel = tk.Label(self, textvariable=self.string_var)
         self.clabel.configure(bg=GUI_DATA.colors.dark_grey, font=GUI_DATA.fonts.cas8b)
         self.clabel.grid(row=0, column=1, sticky="nsew", padx=2, pady=2)
         tkinter_utils.VarColorPicker(self.string_var, self.clabel, True)
```

### Comparing `Subsearch-2.34.0rc1/src/subsearch/gui/tabs/settings_tab.py` & `Subsearch-2.35.0rc1/src/subsearch/gui/tabs/settings_tab.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import tkinter as tk
 import webbrowser
 from tkinter import ttk
 
 from subsearch.data import GUI_DATA, __version__
 from subsearch.gui import tkinter_utils
-from subsearch.utils import io_json, updates
+from subsearch.utils import io_json, update
 
 
 class FileExtensions(tk.Frame):
     def __init__(self, parent) -> None:
         tk.Frame.__init__(self, parent)
         self.configure(bg=GUI_DATA.colors.dark_grey)
         self.data = io_json.get_json_data()
@@ -48,15 +48,15 @@
         btn = event.widget
         key = self.checkbox_value[btn][0]
         value = self.checkbox_value[btn][1]
         if value.get() is True:
             self.data["file_extensions"][key] = False
         elif value.get() is False:
             self.data["file_extensions"][key] = True
-        io_json.set_config(self.data)
+        io_json.set_json_data(self.data)
 
         self.update_registry()
 
     def update_registry(self) -> None:
         from subsearch.utils import io_winreg
 
         io_winreg.write_all_valuex()
@@ -139,59 +139,40 @@
         tkinter_utils.ToggleableFrameButton.__init__(self, parent, "Multiple app instances", "multiple_app_instances")
 
 
 class CheckForUpdates(tk.Frame):
     def __init__(self, parent) -> None:
         tk.Frame.__init__(self, parent)
         self.configure(bg=GUI_DATA.colors.dark_grey)
-        self.string_var = tk.StringVar()
-        self.string_var.set(f"")
-        label = tk.Label(self, text=f"Version {__version__}")
-        label.configure(tkinter_utils.DEFAULT_LABEL_CONFIG)
-        label.grid(tkinter_utils.DEFAULT_LABEL_GRID)
-        self.clabel = tk.Label(self, textvariable=self.string_var)
-        self.clabel.configure(bg=GUI_DATA.colors.dark_grey, fg=GUI_DATA.colors.yellow, font=GUI_DATA.fonts.cas8b)
-        self.clabel.grid(row=0, column=1, sticky="nsew", padx=2, pady=2)
-        btn_check = ttk.Button(
+        self.latest_version = None
+        self.btn_search = ttk.Button(
             self,
-            text="Check for updates",
-            width=18,
+            text="Search for updates",
+            width=40,
         )
-        btn_check.grid(row=0, column=3, pady=2)
-        self.btn_download = ttk.Button(
+        self.btn_visit_release_page = ttk.Button(
             self,
-            text="",
-            width=18,
+            text="Open in webbrowser",
+            width=40,
         )
-        self.btn_download.grid(row=0, column=2, pady=2)
-        btn_check.bind("<Enter>", self.enter_button)
-        self.btn_download.bind("<Enter>", self.enter_button)
+        self.btn_search.grid(row=0, column=2, pady=2)
+        self.btn_search.bind("<Enter>", self.enter_button)
         tkinter_utils.set_default_grid_size(self)
 
     def enter_button(self, event) -> None:
         btn = event.widget
-        if btn["text"] == "Check for updates":
-            btn.bind("<ButtonRelease-1>", self.button_check)
-        if btn["text"].startswith("Get"):
-            btn.bind("<ButtonRelease-1>", self.button_download)
-
-    def button_check(self, event) -> None:
-        self.string_var.set(f"Looking...")
-        new_repo_avail, repo_is_prerelease = updates.is_new_version_avail()
-        latest_version = updates.get_latest_version()
-        if new_repo_avail and repo_is_prerelease:
-            if "-rc" in latest_version:
-                self.string_var.set(f"Release candidate")
-            elif "-alpha" in latest_version:
-                self.string_var.set(f"Alpha release")
-            elif "-beta" in latest_version:
-                self.string_var.set(f"Beta release")
-        elif new_repo_avail and repo_is_prerelease is False:
-            self.string_var.set(f"Stable release")
-        else:
-            self.string_var.set(f"Up to date")
+        if btn == self.btn_search:
+            btn.bind("<ButtonRelease-1>", self.search_button)
 
+    def search_button(self, event) -> None:
+        new_repo_avail, repo_is_prerelease = update.is_new_version_avail()
+        self.latest_version = update.get_latest_version()
         if new_repo_avail:
-            self.btn_download.configure(text=f"Get v{latest_version}")
+            self.sha256_hex = update.find_sha256("https://github.com/vagabondHustler/subsearch/releases")
+            self.btn_search.destroy()
+            self.btn_visit_release_page.grid(row=0, column=2, pady=2)
+            self.btn_visit_release_page.bind("<ButtonRelease-1>", self.visit_repository_button)
+        if not new_repo_avail:
+            self.btn_search["text"] = f"Latest version already installed"
 
-    def button_download(self, event) -> None:
-        webbrowser.open("https://github.com/vagabondHustler/SubSearch/releases")
+    def visit_repository_button(self, event) -> None:
+        webbrowser.open(f"https://github.com/vagabondHustler/subsearch/releases")
```

### Comparing `Subsearch-2.34.0rc1/src/subsearch/gui/tkinter_utils.py` & `Subsearch-2.35.0rc1/src/subsearch/gui/tkinter_utils.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.34.0rc1/src/subsearch/providers/opensubtitles.py` & `Subsearch-2.35.0rc1/src/subsearch/providers/opensubtitles.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import re
 from typing import Any
 
-from subsearch.data import video_data
-from subsearch.data.data_objects import DownloadMetaData, FormattedMetadata
+from subsearch.data import app_paths
+from subsearch.data.data_objects import DownloadData, PrettifiedDownloadData
 from subsearch.providers import generic
 from subsearch.providers.generic import ProviderParameters
 from subsearch.utils import log, string_parser
 
 
 class OpenSubtitlesScraper:
     def __init__(self) -> None:
@@ -48,58 +48,58 @@
         return subtitles
 
 
 class OpenSubtitles(ProviderParameters, OpenSubtitlesScraper):
     def __init__(self, **kwargs):
         ProviderParameters.__init__(self, **kwargs)
         OpenSubtitlesScraper.__init__(self)
-        self.logged_and_sorted: list[FormattedMetadata] = []
+        self.logged_and_sorted: list[PrettifiedDownloadData] = []
 
-    def parse_hash_results(self) -> list | list[DownloadMetaData]:
+    def parse_hash_results(self) -> list | list[DownloadData]:
         # search for hash
         to_be_downloaded = self.with_hash(self.url_opensubtitles_hash, self.release)
 
         # log results
         data_found = True if to_be_downloaded else False
         if data_found is False:
             return []
         log.output_match("opensubtitles", 100, self.release)
 
         # pack download data
-        download_info = generic.pack_download_data("opensubtitles", video_data.tmp_directory, to_be_downloaded)
+        download_info = generic.create_download_data("opensubtitles", app_paths.tmpdir, to_be_downloaded)
         return download_info
 
-    def parse_site_results(self) -> list | list[DownloadMetaData]:
+    def parse_site_results(self) -> list | list[DownloadData]:
         # search for title
         subtitle_data = self.get_subtitles(self.url_opensubtitles)
 
         # log results
         data_found = True if subtitle_data else False
         if data_found is False:
             return []
 
         # search for subtitle
         to_be_downloaded: dict[str, str] = {}
-        to_be_sorted: list[FormattedMetadata] = []
+        to_be_sorted: list[PrettifiedDownloadData] = []
         for key, value in subtitle_data.items():
             pct_result = string_parser.calculate_match(key, self.release)
             log.output_match("opensubtitles", pct_result, key)
-            formatted_data = generic.format_key_value_pct("opensubtitles", key, value, pct_result)
+            formatted_data = generic.prettify_download_data("opensubtitles", key, value, pct_result)
             to_be_sorted.append(formatted_data)
             if self.is_threshold_met(key, pct_result) is False or self.manual_download_mode:
                 continue
             if value in to_be_downloaded.values():
                 continue
             to_be_downloaded[key] = value
 
-        self.sorted_metadata = generic.sort_download_metadata(to_be_sorted)
+        self.sorted_metadata = generic.sort_prettified_data(to_be_sorted)
         log.downlod_metadata("opensubtitles", self.sorted_metadata, self.percentage_threashold)
 
         if not to_be_downloaded:
             return []
 
         # pack download data
-        download_info = generic.pack_download_data("opensubtitles", video_data.tmp_directory, to_be_downloaded)
+        download_info = generic.create_download_data("opensubtitles", app_paths.tmpdir, to_be_downloaded)
         return download_info
 
-    def _sorted_list(self) -> list[FormattedMetadata]:
+    def _sorted_list(self) -> list[PrettifiedDownloadData]:
         return self.sorted_metadata
```

### Comparing `Subsearch-2.34.0rc1/src/subsearch/providers/subscene.py` & `Subsearch-2.35.0rc1/src/subsearch/providers/subscene.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from selectolax.parser import Node
 
-from subsearch.data import video_data
-from subsearch.data.data_objects import DownloadMetaData, FormattedMetadata
+from subsearch.data import app_paths
+from subsearch.data.data_objects import DownloadData, PrettifiedDownloadData
 from subsearch.providers import generic
 from subsearch.providers.generic import ProviderParameters
 from subsearch.utils import log, string_parser
 
 
 class SubsceneScraper:
     def __init__(self) -> None:
@@ -54,57 +54,57 @@
         return download_url
 
 
 class Subscene(ProviderParameters, SubsceneScraper):
     def __init__(self, **kwargs):
         ProviderParameters.__init__(self, **kwargs)
         SubsceneScraper.__init__(self)
-        self.logged_and_sorted: list[FormattedMetadata] = []
+        self.logged_and_sorted: list[PrettifiedDownloadData] = []
 
     def _definitive_match(self) -> list[str]:
         if self.tvseries:
             return [f"{self.title} - {self.season_ordinal} season"]
         return [f"{self.title} ({self.year})", f"{self.title} ({(self.year-1)})"]
 
-    def parse_site_results(self) -> list | list[DownloadMetaData]:
-        to_be_sorted: list[FormattedMetadata] = []
+    def parse_site_results(self) -> list | list[DownloadData]:
+        to_be_sorted: list[PrettifiedDownloadData] = []
         _to_be_downloaded: dict[str, str] = {}
         to_be_downloaded: dict[str, str] = {}
 
         # find title
         definitive_match = self._definitive_match()
         found_title_url = self.find_title(self.url_subscene, self.current_language, definitive_match)
         if not found_title_url:
             return []
 
         # search for subtitles
         subtitle_data = self.find_subtitles(found_title_url, self.hi_sub, self.non_hi_sub)
         for key, value in subtitle_data.items():
             pct_result = string_parser.calculate_match(key, self.release)
             log.output_match("subscene", pct_result, key)
-            formatted_data = generic.format_key_value_pct("subscene", key, value, pct_result)
+            formatted_data = generic.prettify_download_data("subscene", key, value, pct_result)
             to_be_sorted.append(formatted_data)
             if self.is_threshold_met(key, pct_result) is False or self.manual_download_mode:
                 continue
             if key in _to_be_downloaded.keys():
                 continue
             _to_be_downloaded[key] = value
 
-        self.sorted_metadata = generic.sort_download_metadata(to_be_sorted)
+        self.sorted_metadata = generic.sort_prettified_data(to_be_sorted)
         log.downlod_metadata("subscene", self.sorted_metadata, self.percentage_threashold)
         if not _to_be_downloaded:
             return []
 
         # gather subtitle download url
         for release, subtitle_url in _to_be_downloaded.items():
             zip_url = self.get_download_url(subtitle_url)
             to_be_downloaded[release] = zip_url
 
         if not to_be_downloaded:
             return []
 
         # pack download data
-        download_info = generic.pack_download_data("subscene", video_data.tmp_directory, to_be_downloaded)
+        download_info = generic.create_download_data("subscene", app_paths.tmpdir, to_be_downloaded)
         return download_info
 
-    def _sorted_list(self) -> list[FormattedMetadata]:
+    def _sorted_list(self) -> list[PrettifiedDownloadData]:
         return self.sorted_metadata
```

### Comparing `Subsearch-2.34.0rc1/src/subsearch/providers/yifysubtitles.py` & `Subsearch-2.35.0rc1/src/subsearch/providers/yifysubtitles.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,11 @@
 from selectolax.parser import Node
 
-from subsearch.data import video_data
-from subsearch.data.data_objects import (
-    AppConfig,
-    DownloadMetaData,
-    FormattedMetadata,
-    ProviderUrls,
-    ReleaseData,
-)
+from subsearch.data import app_paths
+from subsearch.data.data_objects import DownloadData, PrettifiedDownloadData
 from subsearch.providers import generic
 from subsearch.providers.generic import ProviderParameters
 from subsearch.utils import log, string_parser
 
 
 class YifySubtitlesScraper:
     def __init__(self) -> None:
@@ -46,42 +40,42 @@
         return subtitles
 
 
 class YifiSubtitles(ProviderParameters, YifySubtitlesScraper):
     def __init__(self, **kwargs):
         ProviderParameters.__init__(self, **kwargs)
         YifySubtitlesScraper.__init__(self)
-        self.logged_and_sorted: list[FormattedMetadata] = []
+        self.logged_and_sorted: list[PrettifiedDownloadData] = []
 
-    def parse_site_results(self) -> list | list[DownloadMetaData]:
+    def parse_site_results(self) -> list | list[DownloadData]:
         # search for title
         subtitle_data = self.get_subtitle(self.url_yifysubtitles, self.current_language, self.hi_sub, self.non_hi_sub)
         to_be_downloaded: dict[str, str] = {}
-        to_be_sorted: list[FormattedMetadata] = []
+        to_be_sorted: list[PrettifiedDownloadData] = []
 
         data_found = True if subtitle_data else False
         if data_found is False:
             return []
         # search for subtitle
         for key, value in subtitle_data.items():
             pct_result = string_parser.calculate_match(key, self.release)
             log.output_match("yifysubtitles", pct_result, key)
-            formatted_data = generic.format_key_value_pct("yifysubtitles", key, value, pct_result)
+            formatted_data = generic.prettify_download_data("yifysubtitles", key, value, pct_result)
             to_be_sorted.append(formatted_data)
             if self.is_threshold_met(key, pct_result) is False or self.manual_download_mode:
                 continue
             if value in to_be_downloaded.values():
                 continue
             to_be_downloaded[key] = value
 
-        self.sorted_metadata = generic.sort_download_metadata(to_be_sorted)
+        self.sorted_metadata = generic.sort_prettified_data(to_be_sorted)
         log.downlod_metadata("yifysubtitles", self.sorted_metadata, self.percentage_threashold)
 
         if not to_be_downloaded:
             return []
 
         # pack download data
-        download_info = generic.pack_download_data("yifysubtitles", video_data.tmp_directory, to_be_downloaded)
+        download_info = generic.create_download_data("yifysubtitles", app_paths.tmpdir, to_be_downloaded)
         return download_info
 
-    def _sorted_list(self) -> list[FormattedMetadata]:
+    def _sorted_list(self) -> list[PrettifiedDownloadData]:
         return self.sorted_metadata
```

### Comparing `Subsearch-2.34.0rc1/src/subsearch/utils/exceptions.py` & `Subsearch-2.35.0rc1/src/subsearch/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.34.0rc1/src/subsearch/utils/file_manager.py` & `Subsearch-2.35.0rc1/src/subsearch/utils/file_manager.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import shutil
 import struct
 import sys
 import zipfile
 from pathlib import Path
 
-from subsearch.data import video_data
-from subsearch.data.data_objects import DownloadMetaData
+from subsearch.data import __guid__, app_paths, video_data
+from subsearch.data.data_objects import DownloadData
 from subsearch.providers.generic import get_cloudscraper
 from subsearch.utils import log, string_parser
 
 
 def running_from_exe() -> bool:
     """
     Checks if the module is running from an executable file.
@@ -18,16 +18,17 @@
         bool: True if the module is running from an executable file, False otherwise.
     """
     if sys.argv[0].endswith(".exe"):
         return True
     return False
 
 
-def download_subtitle(data: DownloadMetaData) -> int:
-    """Download the subtitle from the given url.
+def download_subtitle(data: DownloadData) -> int:
+    """
+    Download the subtitle from the given url.
 
     Args:
       data: A DownloadMetaData object that has information about the subtitle file to be downloaded.
 
     Returns:
       An integer value that represents the index number of the subtitle that was downloaded.
 
@@ -105,15 +106,14 @@
     Args:
         cwd (pathlib.Path): The directory path where the files to be deleted reside.
         extension (str): The file extension of the files to be deleted.
 
     Returns:
         None
     """
-
     for file in Path(cwd).glob(f"*{extension}"):
         log.path_action("remove", file)
         file_path = Path(cwd) / file
         file_path.unlink()
 
 
 def del_directory(directory: Path) -> None:
@@ -132,27 +132,14 @@
 
 def directory_is_empty(directory: Path) -> bool:
     if not any(directory.iterdir()):
         return True
     return False
 
 
-def make_necessary_directories() -> None:
-    """
-    Make necessary directories using video object info.
-    """
-
-    if video_data is None:
-        return None
-    if not Path(video_data.tmp_directory).exists():
-        Path.mkdir(video_data.tmp_directory)
-    if not Path(video_data.subs_directory).exists():
-        Path.mkdir(video_data.subs_directory)
-
-
 def get_hash(file_path: Path | None) -> str:
     """
     Calculates and returns the hash value of given file path.
 
     Args:
         file_path: A Path object indicating the location of the input file. If None, returns an all-zero string.
 
@@ -162,35 +149,47 @@
     Examples:
         get_hash(Path("my_folder/my_file.jpg")) returns "d020f52c464caedd"
         get_hash(None) returns ""
     """
     if file_path is None:
         return ""
     try:
-        longlongformat = "<q"  # little-endian long long
+        longlongformat = "<q"
         bytesize = struct.calcsize(longlongformat)
         with open(file_path, "rb") as f:
-            # filesize = os.path.getsize(file_path)
             filesize = file_path.stat().st_size
             hash = filesize
             if filesize < 65536 * 2:
                 log.output(f"SizeError: filesize is {filesize} bytes", False)
                 return ""
             n1 = 65536 // bytesize
             for _x in range(n1):
                 buffer = f.read(bytesize)
                 (l_value,) = struct.unpack(longlongformat, buffer)
                 hash += l_value
-                hash = hash & 0xFFFFFFFFFFFFFFFF  # to remain as 64bit number
+                hash = hash & 0xFFFFFFFFFFFFFFFF
             f.seek(max(0, filesize - 65536), 0)
             n2 = 65536 // bytesize
             for _x in range(n2):
                 buffer = f.read(bytesize)
                 (l_value,) = struct.unpack(longlongformat, buffer)
                 hash += l_value
                 hash = hash & 0xFFFFFFFFFFFFFFFF
 
         returnedhash = "%016x" % hash
         return returnedhash
 
     except IOError:
         return ""
+
+
+def delete_temp_files(temp_path: Path):
+    for item in temp_path.iterdir():
+        log.path_action("remove", item)
+        if item.is_file():
+            item.unlink()
+        if item.is_dir():
+            shutil.rmtree(item)
+
+
+def create_directory(path: Path):
+    path.mkdir(exist_ok=True)
```

### Comparing `Subsearch-2.34.0rc1/src/subsearch/utils/imdb_lookup.py` & `Subsearch-2.35.0rc1/src/subsearch/utils/imdb_lookup.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.34.0rc1/src/subsearch/utils/io_json.py` & `Subsearch-2.35.0rc1/src/subsearch/utils/io_json.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import json
 from pathlib import Path
 from typing import Any, Union
 
-from subsearch.data import app_paths
+from subsearch.data import SUPPORTED_FILE_EXTENSIONS, SUPPORTED_PROVIDERS, app_paths
 from subsearch.data.data_objects import AppConfig, LanguageData, ProviderAlphaCodeData
 from subsearch.utils.exceptions import ProviderNotImplemented
 
-APPLICATION_CONFIG_JSON = Path(app_paths.data) / "application_config.json"
-LANGUAGES_JSON = Path(app_paths.data) / "languages.json"
+APPCON_JSON = Path(app_paths.appdata_local) / "application_config.json"
+LANGS_JSON = Path(app_paths.data) / "languages.json"
 
 
-def get_json_data(json_file: Path = APPLICATION_CONFIG_JSON) -> Any:
+def get_json_data(json_file: Path = APPCON_JSON) -> Any:
     """
     Returns the contents of the json file as a Python object.
 
     Args:
         None
 
     Returns:
@@ -37,82 +37,77 @@
 
     Returns:
         Any: value
     """
     return get_json_data()[f"{key}"]
 
 
-_current_language: str = get_json_key("current_language")
-
-#
-#       subsearch/data/application_config.json
-#
-
-
 def set_config_key_value(key: str, value: Union[str, int, bool]) -> None:
     """
     Set the value of a key in the config.json file to a specified value.
 
     Args:
         key (str): A string that represents the key name to modify.
         value (Union[str, int, bool]): A value of String/Integer/Boolean to assign to the specified key.
 
     Returns:
         None
     """
 
-    with open(APPLICATION_CONFIG_JSON, "r+", encoding="utf-8") as f:
+    with open(APPCON_JSON, "r+", encoding="utf-8") as f:
         data = json.load(f)
         data[key] = value
         f.seek(0)
         json.dump(data, f, indent=4)
         f.truncate()
 
 
-def set_config(data: dict[str, Union[str, int, bool]]) -> None:
+def set_json_data(data: dict[str, Union[str, int, bool]], json_file: Path = APPCON_JSON) -> None:
     """
     Writes the provided configuration data to the config.json file.
 
     Args:
         data: A dictionary containing configuration data with keys as strings and values as an instance
                 of either a string, int or boolean type.
 
     Returns:
         None
     """
-    with open(APPLICATION_CONFIG_JSON, "w") as f:
+    with open(json_file, "w") as f:
         f.seek(0)
         json.dump(data, f, indent=4)
         f.truncate()
 
 
-def set_default_json() -> None:
+def create_application_config() -> None:
     """
-    Sets default values to keys that are present inside config.json file and modifies the same file.
+    Creates application_config.json file and set the default values.
 
     Returns:
         None.
     """
-
-    data = get_json_data()
+    if APPCON_JSON.exists():
+        return None
+    subtitle_types = ["hearing_impaired", "non_hearing_impaired"]
+    data = {}
     data["current_language"] = "english"
-    data["subtitle_type"] = dict.fromkeys(data["subtitle_type"], True)
+    data["subtitle_type"] = dict.fromkeys(subtitle_types, True)
     data["percentage_threshold"] = 90
     data["rename_best_match"] = True
     data["context_menu"] = True
     data["context_menu_icon"] = True
     data["manual_download_fail"] = True
     data["manual_download_mode"] = False
     data["use_threading"] = True
     data["multiple_app_instances"] = False
     data["show_terminal"] = False
     data["log_to_file"] = False
-    data["file_extensions"] = dict.fromkeys(data["file_extensions"], True)
-    data["providers"] = dict.fromkeys(data["providers"], True)
-    with open(APPLICATION_CONFIG_JSON, "r+", encoding="utf-8") as file:
+    data["file_extensions"] = dict.fromkeys(SUPPORTED_FILE_EXTENSIONS, True)
+    data["providers"] = dict.fromkeys(SUPPORTED_PROVIDERS, True)
+    with open(APPCON_JSON, "w", encoding="utf-8") as file:
         file.seek(0)
         json.dump(data, file, indent=4)
         file.truncate()
 
 
 def get_app_config() -> AppConfig:
     """
@@ -126,33 +121,35 @@
         **data,
         hearing_impaired=data["subtitle_type"]["hearing_impaired"],
         non_hearing_impaired=data["subtitle_type"]["non_hearing_impaired"],
     )
     return user_data
 
 
-def get_language_data(language: str = _current_language) -> LanguageData:
+def get_language_data(language: str = "default") -> LanguageData:
     """
     Get the language data object for the provided language from the languages.json configuration file.
 
     Args:
         language: The language for which to retrieve the data. Defaults to the current language stored in the application
                 configuration if not specified.
 
     Returns:
         A LanguageData object containing the data associated with the specified language.
     """
+    if language == "default":
+        language = get_json_key("current_language")
 
-    data = get_json_data(LANGUAGES_JSON)
+    data = get_json_data(LANGS_JSON)
     language_data = LanguageData(**data[language])
     return language_data
 
 
 def get_available_languages() -> dict:
-    return get_json_data(LANGUAGES_JSON)
+    return get_json_data(LANGS_JSON)
 
 
 def get_provider_alpha_code_type(provider: str) -> ProviderAlphaCodeData:
     """
     Generates ProviderAlphaCodeType object containing provider and its associated alpha code.
 
     Args:
@@ -173,15 +170,17 @@
 
 
 def get_provider_alpha_code(provider: str) -> str:
     data = get_provider_alpha_code_type(provider)
     return get_alpha_code(data.alpha_code)
 
 
-def check_language_compatibility(provider: str, language: str = _current_language) -> bool:
+def check_language_compatibility(provider: str, language: str = "default") -> bool:
+    if language == "default":
+        language = get_json_key("current_language")
     data = get_language_data(language)
     if not data.incompatibility:
         return True
 
     elif provider in data.incompatibility:
         return False
     return False
```

### Comparing `Subsearch-2.34.0rc1/src/subsearch/utils/io_winreg.py` & `Subsearch-2.35.0rc1/src/subsearch/utils/io_winreg.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.34.0rc1/src/subsearch/utils/log.py` & `Subsearch-2.35.0rc1/src/subsearch/utils/log.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,26 +3,29 @@
 from datetime import datetime
 from pathlib import Path
 from threading import Lock
 
 from subsearch.data import __version__, video_data
 from subsearch.data.data_objects import (
     AppConfig,
-    FormattedMetadata,
     LanguageData,
+    PrettifiedDownloadData,
     ProviderUrls,
     ReleaseData,
 )
 from subsearch.utils import io_json
 
 NOW = datetime.now()
 DATE = NOW.strftime("%y%m%d")
-LOG_TO_FILE = io_json.get_json_key("log_to_file")
-
+try:
+    LOG_TO_FILE = io_json.get_json_key("log_to_file")
+except FileNotFoundError:
+    pass
 
+lock = Lock()
 logger = logging.getLogger("subsearch")
 logger.setLevel(logging.DEBUG)
 
 release_data: ReleaseData
 app_config: AppConfig
 provider_urls: ProviderUrls
 language_data: LanguageData
@@ -50,23 +53,22 @@
         }
         log_methods[level](msg)
 
     def _to_terminal(msg: str, to_terminal, level: str) -> None:
         if to_terminal is False:
             return
         if level == "info":
-            lock = Lock()
-            lock.acquire()
             print(msg)
-            lock.release()
         else:
             print(f"{level.upper()} - {msg}")
 
     _to_log(msg, level)
+    lock.acquire()
     _to_terminal(msg, terminal, level)
+    lock.release()
 
 
 def warning_spaces_in_filename() -> None:
     name_unresolved = f"{video_data.filename}{video_data.file_extension}"
     output(f"File: '{name_unresolved}' contains spaces", level="warning")
     output(f"Results may vary, use punctuation marks for a more accurate result", level="info")
     output("")
@@ -184,15 +186,15 @@
     global release_data, app_config, provider_urls, language_data
     release_data = kwargs["release_data"]
     app_config = kwargs["app_config"]
     provider_urls = kwargs["provider_urls"]
     language_data = kwargs["language_data"]
 
 
-def downlod_metadata(provider_: str, formatted_metadata_: list[FormattedMetadata], search_threashold: int) -> None:
+def downlod_metadata(provider_: str, formatted_metadata_: list[PrettifiedDownloadData], search_threashold: int) -> None:
     output("")
     output(f"--- [Sorted List from {provider_}] ---", False)
     downloaded_printed = False
     not_downloaded_printed = False
     for data in formatted_metadata_:
         if data.pct_result >= search_threashold and not downloaded_printed:
             output(f"--- Has been downloaded ---\n", False)
```

### Comparing `Subsearch-2.34.0rc1/src/subsearch/utils/mutex_synchronizer.py` & `Subsearch-2.35.0rc1/src/subsearch/utils/mutex_synchronizer.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,16 +18,19 @@
     Raises:
         MultipleInstancesError: If another instance of the application is already running.
 
     """
 
     def wrapper(func: Callable) -> Callable:
         def inner(*args, **kwargs):
-            if io_json.get_json_key("multiple_app_instances"):
-                return func()
+            try:
+                if io_json.get_json_key("multiple_app_instances"):
+                    return func()
+            except FileNotFoundError:
+                pass
             kernel32 = ctypes.WinDLL("kernel32")
             mutex = kernel32.CreateMutexW(None, False, mutex_name)
             last_error = kernel32.GetLastError()
 
             if last_error == 183:
                 raise exceptions.MultipleInstancesError(mutex_name)
             try:
```

### Comparing `Subsearch-2.34.0rc1/src/subsearch/utils/string_parser.py` & `Subsearch-2.35.0rc1/src/subsearch/utils/string_parser.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.34.0rc1/src/subsearch/utils/updates.py` & `Subsearch-2.35.0rc1/src/subsearch/utils/update.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import re
 
 import cloudscraper
+import requests
+import selectolax
 from packaging.version import Version
 
-from subsearch.data import __version__
+from subsearch.data import __guid__, __version__
 
 
 def find_semantic_version(version: str) -> str:
     """
     Parses a version string to extract the semantic version number.
 
     Args:
@@ -67,7 +69,33 @@
 
     if Version(__version__) < Version(released_version):
         if Version(released_version).is_prerelease:
             repo_is_prerelease = True
         new_repo_avail = True
 
     return new_repo_avail, repo_is_prerelease
+
+
+# Work in progress
+# def find_sha256(url):
+#     response = requests.get(url)
+#     html_content = response.text
+
+#     parser = selectolax.parser.HTMLParser(html_content)
+#     selector_lst = [
+#         ".clearfix",
+#         "div:nth-child(3)",
+#         "section:nth-child(1)",
+#         "div:nth-child(2)",
+#         "div:nth-child(2)",
+#         "div:nth-child(1)",
+#         "div:nth-child(1)",
+#         "div:nth-child(2)",
+#         "h6:nth-child(5)",
+#         "p:nth-child(2)",
+#     ]
+
+#     css_selector = " > ".join(selector_lst)
+
+#     element = parser.css(css_selector)
+#     match = re.search(r"([A-Fa-f0-9]{64})", element[0].html)
+#     return match[0]
```

