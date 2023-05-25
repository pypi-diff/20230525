# Comparing `tmp/Subsearch-2.35.0rc2.tar.gz` & `tmp/Subsearch-2.35.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Subsearch-2.35.0rc2.tar", last modified: Thu May 25 14:05:56 2023, max compression
+gzip compressed data, was "Subsearch-2.35.0rc3.tar", last modified: Thu May 25 15:05:10 2023, max compression
```

## Comparing `Subsearch-2.35.0rc2.tar` & `Subsearch-2.35.0rc3.tar`

### file list

```diff
@@ -1,112 +1,112 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:05:56.372914 Subsearch-2.35.0rc2/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-25 14:05:37.000000 Subsearch-2.35.0rc2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-25 14:05:37.000000 Subsearch-2.35.0rc2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7970 2023-05-25 14:05:56.372914 Subsearch-2.35.0rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7202 2023-05-25 14:05:37.000000 Subsearch-2.35.0rc2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-05-25 14:05:37.000000 Subsearch-2.35.0rc2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 14:05:56.372914 Subsearch-2.35.0rc2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-05-25 14:05:37.000000 Subsearch-2.35.0rc2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:05:56.356914 Subsearch-2.35.0rc2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:05:56.360914 Subsearch-2.35.0rc2/src/Subsearch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7970 2023-05-25 14:05:56.000000 Subsearch-2.35.0rc2/src/Subsearch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-05-25 14:05:56.000000 Subsearch-2.35.0rc2/src/Subsearch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 14:05:56.000000 Subsearch-2.35.0rc2/src/Subsearch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-25 14:05:56.000000 Subsearch-2.35.0rc2/src/Subsearch.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 14:05:56.000000 Subsearch-2.35.0rc2/src/Subsearch.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-25 14:05:56.000000 Subsearch-2.35.0rc2/src/Subsearch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-25 14:05:56.000000 Subsearch-2.35.0rc2/src/Subsearch.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:05:56.360914 Subsearch-2.35.0rc2/src/subsearch/
--rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-05-25 14:05:37.000000 Subsearch-2.35.0rc2/src/subsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 14:05:37.000000 Subsearch-2.35.0rc2/src/subsearch/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9672 2023-05-25 14:05:37.000000 Subsearch-2.35.0rc2/src/subsearch/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:05:56.364914 Subsearch-2.35.0rc2/src/subsearch/data/
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-25 14:05:37.000000 Subsearch-2.35.0rc2/src/subsearch/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-05-25 14:05:37.000000 Subsearch-2.35.0rc2/src/subsearch/data/data_initializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9637 2023-05-25 14:05:37.000000 Subsearch-2.35.0rc2/src/subsearch/data/data_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-25 14:05:37.000000 Subsearch-2.35.0rc2/src/subsearch/data/guid.py
--rw-r--r--   0 runner    (1001) docker     (123)     7597 2023-05-25 14:05:37.000000 Subsearch-2.35.0rc2/src/subsearch/data/languages.json
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-25 14:05:37.000000 Subsearch-2.35.0rc2/src/subsearch/data/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:05:56.364914 Subsearch-2.35.0rc2/src/subsearch/gui/
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-05-25 14:05:37.000000 Subsearch-2.35.0rc2/src/subsearch/gui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:05:56.364914 Subsearch-2.35.0rc2/src/subsearch/gui/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:05:56.364914 Subsearch-2.35.0rc2/src/subsearch/gui/assets/btn/
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-25 14:05:37.000000 Subsearch-2.35.0rc2/src/subsearch/gui/assets/btn/btn_disabled.png
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-25 14:05:37.000000 Subsearch-2.35.0rc2/src/subsearch/gui/assets/btn/btn_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-25 14:05:37.000000 Subsearch-2.35.0rc2/src/subsearch/gui/assets/btn/btn_pressed.png
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-25 14:05:37.000000 Subsearch-2.35.0rc2/src/subsearch/gui/assets/btn/btn_rest.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:05:56.364914 Subsearch-2.35.0rc2/src/subsearch/gui/assets/checkbox/
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-25 14:05:37.000000 Subsearch-2.35.0rc2/src/subsearch/gui/assets/checkbox/check_disabled.png
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-25 14:05:37.000000 Subsearch-2.35.0rc2/src/subsearch/gui/assets/checkbox/check_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-25 14:05:37.000000 Subsearch-2.35.0rc2/src/subsearch/gui/assets/checkbox/check_pressed.png
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-25 14:05:37.000000 Subsearch-2.35.0rc2/src/subsearch/gui/assets/checkbox/check_rest.png
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-25 14:05:37.000000 Subsearch-2.35.0rc2/src/subsearch/gui/assets/checkbox/check_tri_disabled.png
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-25 14:05:37.000000 Subsearch-2.35.0rc2/src/subsearch/gui/assets/checkbox/check_tri_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-25 14:05:37.000000 Subsearch-2.35.0rc2/src/subsearch/gui/assets/checkbox/check_tri_pressed.png
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-25 14:05:37.000000 Subsearch-2.35.0rc2/src/subsearch/gui/assets/checkbox/check_tri_rest.png
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-25 14:05:37.000000 Subsearch-2.35.0rc2/src/subsearch/gui/assets/checkbox/check_unsel_disabled.png
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-25 14:05:37.000000 Subsearch-2.35.0rc2/src/subsearch/gui/assets/checkbox/check_unsel_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-25 14:05:37.000000 Subsearch-2.35.0rc2/src/subsearch/gui/assets/checkbox/check_unsel_pressed.png
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-25 14:05:37.000000 Subsearch-2.35.0rc2/src/subsearch/gui/assets/checkbox/check_unsel_rest.png
--rw-r--r--   0 runner    (1001) docker     (123)     5379 2023-05-25 14:05:37.000000 Subsearch-2.35.0rc2/src/subsearch/gui/assets/dark.tcl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:05:56.364914 Subsearch-2.35.0rc2/src/subsearch/gui/assets/icon/
--rw-r--r--   0 runner    (1001) docker     (123)   105808 2023-05-25 14:05:37.000000 Subsearch-2.35.0rc2/src/subsearch/gui/assets/icon/subsearch.ico
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-25 14:05:37.000000 Subsearch-2.35.0rc2/src/subsearch/gui/assets/icon/subsearch.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:05:56.368914 Subsearch-2.35.0rc2/src/subsearch/gui/assets/scale/
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-25 14:05:37.000000 Subsearch-2.35.0rc2/src/subsearch/gui/assets/scale/scale_thumb_disabled.png
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-25 14:05:37.000000 Subsearch-2.35.0rc2/src/subsearch/gui/assets/scale/scale_thumb_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-25 14:05:37.000000 Subsearch-2.35.0rc2/src/subsearch/gui/assets/scale/scale_thumb_pressed.png
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-25 14:05:37.000000 Subsearch-2.35.0rc2/src/subsearch/gui/assets/scale/scale_thumb_rest.png
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-25 14:05:37.000000 Subsearch-2.35.0rc2/src/subsearch/gui/assets/scale/scale_trough_hor.png
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-25 14:05:37.000000 Subsearch-2.35.0rc2/src/subsearch/gui/assets/scale/scale_trough_vert.png
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-25 14:05:37.000000 Subsearch-2.35.0rc2/src/subsearch/gui/assets/scale/separator.png
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-25 14:05:37.000000 Subsearch-2.35.0rc2/src/subsearch/gui/assets/scale/sizegrip.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:05:56.368914 Subsearch-2.35.0rc2/src/subsearch/gui/assets/scrollbar/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-25 14:05:37.000000 Subsearch-2.35.0rc2/src/subsearch/gui/assets/scrollbar/scroll_down.png
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-25 14:05:37.000000 Subsearch-2.35.0rc2/src/subsearch/gui/assets/scrollbar/scroll_hor_thumb.png
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-25 14:05:37.000000 Subsearch-2.35.0rc2/src/subsearch/gui/assets/scrollbar/scroll_hor_trough.png
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-25 14:05:37.000000 Subsearch-2.35.0rc2/src/subsearch/gui/assets/scrollbar/scroll_left.png
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-25 14:05:37.000000 Subsearch-2.35.0rc2/src/subsearch/gui/assets/scrollbar/scroll_right.png
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-25 14:05:37.000000 Subsearch-2.35.0rc2/src/subsearch/gui/assets/scrollbar/scroll_up.png
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-25 14:05:37.000000 Subsearch-2.35.0rc2/src/subsearch/gui/assets/scrollbar/scroll_vert_thumb.png
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-25 14:05:37.000000 Subsearch-2.35.0rc2/src/subsearch/gui/assets/scrollbar/scroll_vert_trough.png
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-25 14:05:37.000000 Subsearch-2.35.0rc2/src/subsearch/gui/assets/scrollbar/separator.png
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-25 14:05:37.000000 Subsearch-2.35.0rc2/src/subsearch/gui/assets/scrollbar/sizegrip.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:05:56.368914 Subsearch-2.35.0rc2/src/subsearch/gui/assets/tabs/
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-25 14:05:37.000000 Subsearch-2.35.0rc2/src/subsearch/gui/assets/tabs/download_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-05-25 14:05:37.000000 Subsearch-2.35.0rc2/src/subsearch/gui/assets/tabs/download_press.png
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-25 14:05:37.000000 Subsearch-2.35.0rc2/src/subsearch/gui/assets/tabs/download_rest.png
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-25 14:05:37.000000 Subsearch-2.35.0rc2/src/subsearch/gui/assets/tabs/language_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-25 14:05:37.000000 Subsearch-2.35.0rc2/src/subsearch/gui/assets/tabs/language_press.png
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-25 14:05:37.000000 Subsearch-2.35.0rc2/src/subsearch/gui/assets/tabs/language_rest.png
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-25 14:05:37.000000 Subsearch-2.35.0rc2/src/subsearch/gui/assets/tabs/search_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-25 14:05:37.000000 Subsearch-2.35.0rc2/src/subsearch/gui/assets/tabs/search_press.png
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-25 14:05:37.000000 Subsearch-2.35.0rc2/src/subsearch/gui/assets/tabs/search_rest.png
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-25 14:05:37.000000 Subsearch-2.35.0rc2/src/subsearch/gui/assets/tabs/settings_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-25 14:05:37.000000 Subsearch-2.35.0rc2/src/subsearch/gui/assets/tabs/settings_press.png
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-25 14:05:37.000000 Subsearch-2.35.0rc2/src/subsearch/gui/assets/tabs/settings_rest.png
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-05-25 14:05:37.000000 Subsearch-2.35.0rc2/src/subsearch/gui/assets/ttk_style.tcl
--rw-r--r--   0 runner    (1001) docker     (123)     8641 2023-05-25 14:05:37.000000 Subsearch-2.35.0rc2/src/subsearch/gui/tab_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:05:56.368914 Subsearch-2.35.0rc2/src/subsearch/gui/tabs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:05:37.000000 Subsearch-2.35.0rc2/src/subsearch/gui/tabs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-05-25 14:05:37.000000 Subsearch-2.35.0rc2/src/subsearch/gui/tabs/dowload_tab.py
--rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-05-25 14:05:37.000000 Subsearch-2.35.0rc2/src/subsearch/gui/tabs/language_tab.py
--rw-r--r--   0 runner    (1001) docker     (123)     9397 2023-05-25 14:05:37.000000 Subsearch-2.35.0rc2/src/subsearch/gui/tabs/search_tab.py
--rw-r--r--   0 runner    (1001) docker     (123)     7251 2023-05-25 14:05:37.000000 Subsearch-2.35.0rc2/src/subsearch/gui/tabs/settings_tab.py
--rw-r--r--   0 runner    (1001) docker     (123)    13667 2023-05-25 14:05:37.000000 Subsearch-2.35.0rc2/src/subsearch/gui/tkinter_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:05:56.372914 Subsearch-2.35.0rc2/src/subsearch/providers/
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-05-25 14:05:37.000000 Subsearch-2.35.0rc2/src/subsearch/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5591 2023-05-25 14:05:37.000000 Subsearch-2.35.0rc2/src/subsearch/providers/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4102 2023-05-25 14:05:37.000000 Subsearch-2.35.0rc2/src/subsearch/providers/opensubtitles.py
--rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-05-25 14:05:37.000000 Subsearch-2.35.0rc2/src/subsearch/providers/subscene.py
--rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-05-25 14:05:37.000000 Subsearch-2.35.0rc2/src/subsearch/providers/yifysubtitles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:05:56.372914 Subsearch-2.35.0rc2/src/subsearch/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-05-25 14:05:37.000000 Subsearch-2.35.0rc2/src/subsearch/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-05-25 14:05:37.000000 Subsearch-2.35.0rc2/src/subsearch/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6042 2023-05-25 14:05:37.000000 Subsearch-2.35.0rc2/src/subsearch/utils/file_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-05-25 14:05:37.000000 Subsearch-2.35.0rc2/src/subsearch/utils/imdb_lookup.py
--rw-r--r--   0 runner    (1001) docker     (123)     5763 2023-05-25 14:05:37.000000 Subsearch-2.35.0rc2/src/subsearch/utils/io_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-05-25 14:05:37.000000 Subsearch-2.35.0rc2/src/subsearch/utils/io_winreg.py
--rw-r--r--   0 runner    (1001) docker     (123)     7249 2023-05-25 14:05:37.000000 Subsearch-2.35.0rc2/src/subsearch/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-25 14:05:37.000000 Subsearch-2.35.0rc2/src/subsearch/utils/mutex_synchronizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11259 2023-05-25 14:05:37.000000 Subsearch-2.35.0rc2/src/subsearch/utils/string_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3185 2023-05-25 14:05:37.000000 Subsearch-2.35.0rc2/src/subsearch/utils/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:05:10.907729 Subsearch-2.35.0rc3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-25 15:04:48.000000 Subsearch-2.35.0rc3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-25 15:04:48.000000 Subsearch-2.35.0rc3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8016 2023-05-25 15:05:10.907729 Subsearch-2.35.0rc3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7237 2023-05-25 15:04:48.000000 Subsearch-2.35.0rc3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-05-25 15:04:48.000000 Subsearch-2.35.0rc3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 15:05:10.907729 Subsearch-2.35.0rc3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-05-25 15:04:48.000000 Subsearch-2.35.0rc3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:05:10.895729 Subsearch-2.35.0rc3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:05:10.899729 Subsearch-2.35.0rc3/src/Subsearch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8016 2023-05-25 15:05:10.000000 Subsearch-2.35.0rc3/src/Subsearch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-05-25 15:05:10.000000 Subsearch-2.35.0rc3/src/Subsearch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 15:05:10.000000 Subsearch-2.35.0rc3/src/Subsearch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-25 15:05:10.000000 Subsearch-2.35.0rc3/src/Subsearch.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 15:05:10.000000 Subsearch-2.35.0rc3/src/Subsearch.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-25 15:05:10.000000 Subsearch-2.35.0rc3/src/Subsearch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-25 15:05:10.000000 Subsearch-2.35.0rc3/src/Subsearch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:05:10.899729 Subsearch-2.35.0rc3/src/subsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-05-25 15:04:48.000000 Subsearch-2.35.0rc3/src/subsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 15:04:48.000000 Subsearch-2.35.0rc3/src/subsearch/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9672 2023-05-25 15:04:48.000000 Subsearch-2.35.0rc3/src/subsearch/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:05:10.899729 Subsearch-2.35.0rc3/src/subsearch/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-25 15:04:48.000000 Subsearch-2.35.0rc3/src/subsearch/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-05-25 15:04:48.000000 Subsearch-2.35.0rc3/src/subsearch/data/data_initializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9637 2023-05-25 15:04:48.000000 Subsearch-2.35.0rc3/src/subsearch/data/data_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-25 15:04:48.000000 Subsearch-2.35.0rc3/src/subsearch/data/guid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7597 2023-05-25 15:04:48.000000 Subsearch-2.35.0rc3/src/subsearch/data/languages.json
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-25 15:04:48.000000 Subsearch-2.35.0rc3/src/subsearch/data/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:05:10.899729 Subsearch-2.35.0rc3/src/subsearch/gui/
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-05-25 15:04:48.000000 Subsearch-2.35.0rc3/src/subsearch/gui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:05:10.899729 Subsearch-2.35.0rc3/src/subsearch/gui/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:05:10.899729 Subsearch-2.35.0rc3/src/subsearch/gui/assets/btn/
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-25 15:04:48.000000 Subsearch-2.35.0rc3/src/subsearch/gui/assets/btn/btn_disabled.png
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-25 15:04:48.000000 Subsearch-2.35.0rc3/src/subsearch/gui/assets/btn/btn_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-25 15:04:48.000000 Subsearch-2.35.0rc3/src/subsearch/gui/assets/btn/btn_pressed.png
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-25 15:04:48.000000 Subsearch-2.35.0rc3/src/subsearch/gui/assets/btn/btn_rest.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:05:10.903729 Subsearch-2.35.0rc3/src/subsearch/gui/assets/checkbox/
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-25 15:04:48.000000 Subsearch-2.35.0rc3/src/subsearch/gui/assets/checkbox/check_disabled.png
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-25 15:04:48.000000 Subsearch-2.35.0rc3/src/subsearch/gui/assets/checkbox/check_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-25 15:04:48.000000 Subsearch-2.35.0rc3/src/subsearch/gui/assets/checkbox/check_pressed.png
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-25 15:04:48.000000 Subsearch-2.35.0rc3/src/subsearch/gui/assets/checkbox/check_rest.png
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-25 15:04:48.000000 Subsearch-2.35.0rc3/src/subsearch/gui/assets/checkbox/check_tri_disabled.png
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-25 15:04:48.000000 Subsearch-2.35.0rc3/src/subsearch/gui/assets/checkbox/check_tri_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-25 15:04:48.000000 Subsearch-2.35.0rc3/src/subsearch/gui/assets/checkbox/check_tri_pressed.png
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-25 15:04:48.000000 Subsearch-2.35.0rc3/src/subsearch/gui/assets/checkbox/check_tri_rest.png
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-25 15:04:48.000000 Subsearch-2.35.0rc3/src/subsearch/gui/assets/checkbox/check_unsel_disabled.png
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-25 15:04:48.000000 Subsearch-2.35.0rc3/src/subsearch/gui/assets/checkbox/check_unsel_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-25 15:04:48.000000 Subsearch-2.35.0rc3/src/subsearch/gui/assets/checkbox/check_unsel_pressed.png
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-25 15:04:48.000000 Subsearch-2.35.0rc3/src/subsearch/gui/assets/checkbox/check_unsel_rest.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5379 2023-05-25 15:04:48.000000 Subsearch-2.35.0rc3/src/subsearch/gui/assets/dark.tcl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:05:10.903729 Subsearch-2.35.0rc3/src/subsearch/gui/assets/icon/
+-rw-r--r--   0 runner    (1001) docker     (123)   105808 2023-05-25 15:04:48.000000 Subsearch-2.35.0rc3/src/subsearch/gui/assets/icon/subsearch.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-25 15:04:48.000000 Subsearch-2.35.0rc3/src/subsearch/gui/assets/icon/subsearch.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:05:10.903729 Subsearch-2.35.0rc3/src/subsearch/gui/assets/scale/
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-25 15:04:48.000000 Subsearch-2.35.0rc3/src/subsearch/gui/assets/scale/scale_thumb_disabled.png
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-25 15:04:48.000000 Subsearch-2.35.0rc3/src/subsearch/gui/assets/scale/scale_thumb_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-25 15:04:48.000000 Subsearch-2.35.0rc3/src/subsearch/gui/assets/scale/scale_thumb_pressed.png
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-25 15:04:48.000000 Subsearch-2.35.0rc3/src/subsearch/gui/assets/scale/scale_thumb_rest.png
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-25 15:04:48.000000 Subsearch-2.35.0rc3/src/subsearch/gui/assets/scale/scale_trough_hor.png
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-25 15:04:48.000000 Subsearch-2.35.0rc3/src/subsearch/gui/assets/scale/scale_trough_vert.png
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-25 15:04:48.000000 Subsearch-2.35.0rc3/src/subsearch/gui/assets/scale/separator.png
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-25 15:04:48.000000 Subsearch-2.35.0rc3/src/subsearch/gui/assets/scale/sizegrip.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:05:10.903729 Subsearch-2.35.0rc3/src/subsearch/gui/assets/scrollbar/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-25 15:04:48.000000 Subsearch-2.35.0rc3/src/subsearch/gui/assets/scrollbar/scroll_down.png
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-25 15:04:48.000000 Subsearch-2.35.0rc3/src/subsearch/gui/assets/scrollbar/scroll_hor_thumb.png
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-25 15:04:48.000000 Subsearch-2.35.0rc3/src/subsearch/gui/assets/scrollbar/scroll_hor_trough.png
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-25 15:04:48.000000 Subsearch-2.35.0rc3/src/subsearch/gui/assets/scrollbar/scroll_left.png
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-25 15:04:48.000000 Subsearch-2.35.0rc3/src/subsearch/gui/assets/scrollbar/scroll_right.png
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-25 15:04:48.000000 Subsearch-2.35.0rc3/src/subsearch/gui/assets/scrollbar/scroll_up.png
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-25 15:04:48.000000 Subsearch-2.35.0rc3/src/subsearch/gui/assets/scrollbar/scroll_vert_thumb.png
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-25 15:04:48.000000 Subsearch-2.35.0rc3/src/subsearch/gui/assets/scrollbar/scroll_vert_trough.png
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-25 15:04:48.000000 Subsearch-2.35.0rc3/src/subsearch/gui/assets/scrollbar/separator.png
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-25 15:04:48.000000 Subsearch-2.35.0rc3/src/subsearch/gui/assets/scrollbar/sizegrip.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:05:10.907729 Subsearch-2.35.0rc3/src/subsearch/gui/assets/tabs/
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-25 15:04:48.000000 Subsearch-2.35.0rc3/src/subsearch/gui/assets/tabs/download_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-05-25 15:04:48.000000 Subsearch-2.35.0rc3/src/subsearch/gui/assets/tabs/download_press.png
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-25 15:04:48.000000 Subsearch-2.35.0rc3/src/subsearch/gui/assets/tabs/download_rest.png
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-25 15:04:48.000000 Subsearch-2.35.0rc3/src/subsearch/gui/assets/tabs/language_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-25 15:04:48.000000 Subsearch-2.35.0rc3/src/subsearch/gui/assets/tabs/language_press.png
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-25 15:04:48.000000 Subsearch-2.35.0rc3/src/subsearch/gui/assets/tabs/language_rest.png
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-25 15:04:48.000000 Subsearch-2.35.0rc3/src/subsearch/gui/assets/tabs/search_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-25 15:04:48.000000 Subsearch-2.35.0rc3/src/subsearch/gui/assets/tabs/search_press.png
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-25 15:04:48.000000 Subsearch-2.35.0rc3/src/subsearch/gui/assets/tabs/search_rest.png
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-25 15:04:48.000000 Subsearch-2.35.0rc3/src/subsearch/gui/assets/tabs/settings_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-25 15:04:48.000000 Subsearch-2.35.0rc3/src/subsearch/gui/assets/tabs/settings_press.png
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-25 15:04:48.000000 Subsearch-2.35.0rc3/src/subsearch/gui/assets/tabs/settings_rest.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-05-25 15:04:48.000000 Subsearch-2.35.0rc3/src/subsearch/gui/assets/ttk_style.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)     8641 2023-05-25 15:04:48.000000 Subsearch-2.35.0rc3/src/subsearch/gui/tab_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:05:10.907729 Subsearch-2.35.0rc3/src/subsearch/gui/tabs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:04:48.000000 Subsearch-2.35.0rc3/src/subsearch/gui/tabs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-05-25 15:04:48.000000 Subsearch-2.35.0rc3/src/subsearch/gui/tabs/dowload_tab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-05-25 15:04:48.000000 Subsearch-2.35.0rc3/src/subsearch/gui/tabs/language_tab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9397 2023-05-25 15:04:48.000000 Subsearch-2.35.0rc3/src/subsearch/gui/tabs/search_tab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7251 2023-05-25 15:04:48.000000 Subsearch-2.35.0rc3/src/subsearch/gui/tabs/settings_tab.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13667 2023-05-25 15:04:48.000000 Subsearch-2.35.0rc3/src/subsearch/gui/tkinter_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:05:10.907729 Subsearch-2.35.0rc3/src/subsearch/providers/
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-05-25 15:04:48.000000 Subsearch-2.35.0rc3/src/subsearch/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5591 2023-05-25 15:04:48.000000 Subsearch-2.35.0rc3/src/subsearch/providers/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4102 2023-05-25 15:04:48.000000 Subsearch-2.35.0rc3/src/subsearch/providers/opensubtitles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-05-25 15:04:48.000000 Subsearch-2.35.0rc3/src/subsearch/providers/subscene.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-05-25 15:04:48.000000 Subsearch-2.35.0rc3/src/subsearch/providers/yifysubtitles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:05:10.907729 Subsearch-2.35.0rc3/src/subsearch/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-05-25 15:04:48.000000 Subsearch-2.35.0rc3/src/subsearch/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-05-25 15:04:48.000000 Subsearch-2.35.0rc3/src/subsearch/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6042 2023-05-25 15:04:48.000000 Subsearch-2.35.0rc3/src/subsearch/utils/file_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-05-25 15:04:48.000000 Subsearch-2.35.0rc3/src/subsearch/utils/imdb_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5763 2023-05-25 15:04:48.000000 Subsearch-2.35.0rc3/src/subsearch/utils/io_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-05-25 15:04:48.000000 Subsearch-2.35.0rc3/src/subsearch/utils/io_winreg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7249 2023-05-25 15:04:48.000000 Subsearch-2.35.0rc3/src/subsearch/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-25 15:04:48.000000 Subsearch-2.35.0rc3/src/subsearch/utils/mutex_synchronizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11259 2023-05-25 15:04:48.000000 Subsearch-2.35.0rc3/src/subsearch/utils/string_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-05-25 15:04:48.000000 Subsearch-2.35.0rc3/src/subsearch/utils/update.py
```

### Comparing `Subsearch-2.35.0rc2/LICENSE` & `Subsearch-2.35.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `Subsearch-2.35.0rc2/PKG-INFO` & `Subsearch-2.35.0rc3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: Subsearch
-Version: 2.35.0rc2
-Summary: Download subtitles for movies and shows, automatically with one easy mouse click.
+Version: 2.35.0rc3
+Summary: Subsearch - Download subtitles for movies and shows, automatically with one easy mouse click.
 Author: vagabondHustler
 Author-email: vagabondHustler.github@gmail.com
 License: MIT license
 Project-URL: repository, https://github.com/vagabondHustler/subsearch
 Keywords: subsearch,subscene,opensubtitles,yifysubtitles,download,subtitles,movies,shows,automatically,scrape
 Platform: win32
 Classifier: Programming Language :: Python :: 3.10
@@ -115,14 +115,15 @@
 - Install Subsearch by running `pip install -e <local project path>[package-index-options]`. For example, run `pip install -e .` for only required dependencies or `pip install -e .[dev, optional]` for dev/optional dependencies.
 - Build the executable and MSI installer by running `python setup.py bdist_msi`.
 
 #### Subsearch .msi Installer <a name = "msi"></a>
 
 - Download `SubSearch-x.x.x-win64.msi` from the Subsearch releases [page](https://github.com/vagabondHustler/SubSearch/releases)
 - Install the .msi file.
+- Run Subsearch.exe at least once
 - To update from a previous version, download and run the new installer in the same directory. If installed in a different directory, delete the old registry key (see Wiki for details).the same directory. Else you might have to delete the old registry key, (see [Wiki](https://github.com/vagabondHustler/subsearch/wiki/Fixing-Context-Menu-Issue-in-Subsearch) for details).
 - If you receive a PUA message, click `More info`.
 
 <details>
 <summary>Screenshots of PUA message<a name = "code"></a></summary>
 
 ![prtsc_moreinfo](https://raw.githubusercontent.com/vagabondHustler/SubSearch/main/assets/moreinfo.png)
```

### Comparing `Subsearch-2.35.0rc2/README.md` & `Subsearch-2.35.0rc3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -92,14 +92,15 @@
 - Install Subsearch by running `pip install -e <local project path>[package-index-options]`. For example, run `pip install -e .` for only required dependencies or `pip install -e .[dev, optional]` for dev/optional dependencies.
 - Build the executable and MSI installer by running `python setup.py bdist_msi`.
 
 #### Subsearch .msi Installer <a name = "msi"></a>
 
 - Download `SubSearch-x.x.x-win64.msi` from the Subsearch releases [page](https://github.com/vagabondHustler/SubSearch/releases)
 - Install the .msi file.
+- Run Subsearch.exe at least once
 - To update from a previous version, download and run the new installer in the same directory. If installed in a different directory, delete the old registry key (see Wiki for details).the same directory. Else you might have to delete the old registry key, (see [Wiki](https://github.com/vagabondHustler/subsearch/wiki/Fixing-Context-Menu-Issue-in-Subsearch) for details).
 - If you receive a PUA message, click `More info`.
 
 <details>
 <summary>Screenshots of PUA message<a name = "code"></a></summary>
 
 ![prtsc_moreinfo](https://raw.githubusercontent.com/vagabondHustler/SubSearch/main/assets/moreinfo.png)
```

### Comparing `Subsearch-2.35.0rc2/pyproject.toml` & `Subsearch-2.35.0rc3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=65.5", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "Subsearch"
-description = "Download subtitles for movies and shows, automatically with one easy mouse click."
+description = "Subsearch - Download subtitles for movies and shows, automatically with one easy mouse click."
 readme = "README.md"
 requires-python = ">=3.10"
 license = {text = "MIT license"}
 keywords = ["subsearch", "subscene", "opensubtitles", "yifysubtitles", "download", "subtitles", "movies", "shows", "automatically", "scrape"]
 authors = [
   {email = "vagabondHustler.github@gmail.com"},
   {name = "vagabondHustler"}
```

### Comparing `Subsearch-2.35.0rc2/setup.py` & `Subsearch-2.35.0rc3/setup.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.35.0rc2/src/Subsearch.egg-info/PKG-INFO` & `Subsearch-2.35.0rc3/src/Subsearch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: Subsearch
-Version: 2.35.0rc2
-Summary: Download subtitles for movies and shows, automatically with one easy mouse click.
+Version: 2.35.0rc3
+Summary: Subsearch - Download subtitles for movies and shows, automatically with one easy mouse click.
 Author: vagabondHustler
 Author-email: vagabondHustler.github@gmail.com
 License: MIT license
 Project-URL: repository, https://github.com/vagabondHustler/subsearch
 Keywords: subsearch,subscene,opensubtitles,yifysubtitles,download,subtitles,movies,shows,automatically,scrape
 Platform: win32
 Classifier: Programming Language :: Python :: 3.10
@@ -115,14 +115,15 @@
 - Install Subsearch by running `pip install -e <local project path>[package-index-options]`. For example, run `pip install -e .` for only required dependencies or `pip install -e .[dev, optional]` for dev/optional dependencies.
 - Build the executable and MSI installer by running `python setup.py bdist_msi`.
 
 #### Subsearch .msi Installer <a name = "msi"></a>
 
 - Download `SubSearch-x.x.x-win64.msi` from the Subsearch releases [page](https://github.com/vagabondHustler/SubSearch/releases)
 - Install the .msi file.
+- Run Subsearch.exe at least once
 - To update from a previous version, download and run the new installer in the same directory. If installed in a different directory, delete the old registry key (see Wiki for details).the same directory. Else you might have to delete the old registry key, (see [Wiki](https://github.com/vagabondHustler/subsearch/wiki/Fixing-Context-Menu-Issue-in-Subsearch) for details).
 - If you receive a PUA message, click `More info`.
 
 <details>
 <summary>Screenshots of PUA message<a name = "code"></a></summary>
 
 ![prtsc_moreinfo](https://raw.githubusercontent.com/vagabondHustler/SubSearch/main/assets/moreinfo.png)
```

### Comparing `Subsearch-2.35.0rc2/src/Subsearch.egg-info/SOURCES.txt` & `Subsearch-2.35.0rc3/src/Subsearch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Subsearch-2.35.0rc2/src/subsearch/__init__.py` & `Subsearch-2.35.0rc3/src/subsearch/__init__.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.35.0rc2/src/subsearch/core.py` & `Subsearch-2.35.0rc3/src/subsearch/core.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.35.0rc2/src/subsearch/data/data_initializer.py` & `Subsearch-2.35.0rc3/src/subsearch/data/data_initializer.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.35.0rc2/src/subsearch/data/data_objects.py` & `Subsearch-2.35.0rc3/src/subsearch/data/data_objects.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.35.0rc2/src/subsearch/data/languages.json` & `Subsearch-2.35.0rc3/src/subsearch/data/languages.json`

 * *Files identical despite different names*

### Comparing `Subsearch-2.35.0rc2/src/subsearch/gui/__init__.py` & `Subsearch-2.35.0rc3/src/subsearch/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.35.0rc2/src/subsearch/gui/assets/dark.tcl` & `Subsearch-2.35.0rc3/src/subsearch/gui/assets/dark.tcl`

 * *Files identical despite different names*

### Comparing `Subsearch-2.35.0rc2/src/subsearch/gui/assets/icon/subsearch.ico` & `Subsearch-2.35.0rc3/src/subsearch/gui/assets/icon/subsearch.ico`

 * *Files identical despite different names*

### Comparing `Subsearch-2.35.0rc2/src/subsearch/gui/assets/scale/scale_thumb_disabled.png` & `Subsearch-2.35.0rc3/src/subsearch/gui/assets/scale/scale_thumb_disabled.png`

 * *Files identical despite different names*

### Comparing `Subsearch-2.35.0rc2/src/subsearch/gui/assets/scale/scale_thumb_hover.png` & `Subsearch-2.35.0rc3/src/subsearch/gui/assets/scale/scale_thumb_hover.png`

 * *Files identical despite different names*

### Comparing `Subsearch-2.35.0rc2/src/subsearch/gui/assets/scale/scale_thumb_pressed.png` & `Subsearch-2.35.0rc3/src/subsearch/gui/assets/scale/scale_thumb_pressed.png`

 * *Files identical despite different names*

### Comparing `Subsearch-2.35.0rc2/src/subsearch/gui/assets/scale/scale_thumb_rest.png` & `Subsearch-2.35.0rc3/src/subsearch/gui/assets/scale/scale_thumb_rest.png`

 * *Files identical despite different names*

### Comparing `Subsearch-2.35.0rc2/src/subsearch/gui/assets/tabs/download_hover.png` & `Subsearch-2.35.0rc3/src/subsearch/gui/assets/tabs/download_hover.png`

 * *Files identical despite different names*

### Comparing `Subsearch-2.35.0rc2/src/subsearch/gui/assets/tabs/download_press.png` & `Subsearch-2.35.0rc3/src/subsearch/gui/assets/tabs/download_press.png`

 * *Files identical despite different names*

### Comparing `Subsearch-2.35.0rc2/src/subsearch/gui/assets/tabs/download_rest.png` & `Subsearch-2.35.0rc3/src/subsearch/gui/assets/tabs/download_rest.png`

 * *Files identical despite different names*

### Comparing `Subsearch-2.35.0rc2/src/subsearch/gui/assets/tabs/search_hover.png` & `Subsearch-2.35.0rc3/src/subsearch/gui/assets/tabs/search_hover.png`

 * *Files identical despite different names*

### Comparing `Subsearch-2.35.0rc2/src/subsearch/gui/assets/tabs/search_press.png` & `Subsearch-2.35.0rc3/src/subsearch/gui/assets/tabs/search_press.png`

 * *Files identical despite different names*

### Comparing `Subsearch-2.35.0rc2/src/subsearch/gui/assets/tabs/search_rest.png` & `Subsearch-2.35.0rc3/src/subsearch/gui/assets/tabs/search_rest.png`

 * *Files identical despite different names*

### Comparing `Subsearch-2.35.0rc2/src/subsearch/gui/assets/tabs/settings_hover.png` & `Subsearch-2.35.0rc3/src/subsearch/gui/assets/tabs/settings_hover.png`

 * *Files identical despite different names*

### Comparing `Subsearch-2.35.0rc2/src/subsearch/gui/assets/tabs/settings_press.png` & `Subsearch-2.35.0rc3/src/subsearch/gui/assets/tabs/settings_press.png`

 * *Files identical despite different names*

### Comparing `Subsearch-2.35.0rc2/src/subsearch/gui/assets/tabs/settings_rest.png` & `Subsearch-2.35.0rc3/src/subsearch/gui/assets/tabs/settings_rest.png`

 * *Files identical despite different names*

### Comparing `Subsearch-2.35.0rc2/src/subsearch/gui/assets/ttk_style.tcl` & `Subsearch-2.35.0rc3/src/subsearch/gui/assets/ttk_style.tcl`

 * *Files identical despite different names*

### Comparing `Subsearch-2.35.0rc2/src/subsearch/gui/tab_manager.py` & `Subsearch-2.35.0rc3/src/subsearch/gui/tab_manager.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.35.0rc2/src/subsearch/gui/tabs/dowload_tab.py` & `Subsearch-2.35.0rc3/src/subsearch/gui/tabs/dowload_tab.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.35.0rc2/src/subsearch/gui/tabs/language_tab.py` & `Subsearch-2.35.0rc3/src/subsearch/gui/tabs/language_tab.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.35.0rc2/src/subsearch/gui/tabs/search_tab.py` & `Subsearch-2.35.0rc3/src/subsearch/gui/tabs/search_tab.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.35.0rc2/src/subsearch/gui/tabs/settings_tab.py` & `Subsearch-2.35.0rc3/src/subsearch/gui/tabs/settings_tab.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.35.0rc2/src/subsearch/gui/tkinter_utils.py` & `Subsearch-2.35.0rc3/src/subsearch/gui/tkinter_utils.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.35.0rc2/src/subsearch/providers/generic.py` & `Subsearch-2.35.0rc3/src/subsearch/providers/generic.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.35.0rc2/src/subsearch/providers/opensubtitles.py` & `Subsearch-2.35.0rc3/src/subsearch/providers/opensubtitles.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.35.0rc2/src/subsearch/providers/subscene.py` & `Subsearch-2.35.0rc3/src/subsearch/providers/subscene.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.35.0rc2/src/subsearch/providers/yifysubtitles.py` & `Subsearch-2.35.0rc3/src/subsearch/providers/yifysubtitles.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.35.0rc2/src/subsearch/utils/exceptions.py` & `Subsearch-2.35.0rc3/src/subsearch/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.35.0rc2/src/subsearch/utils/file_manager.py` & `Subsearch-2.35.0rc3/src/subsearch/utils/file_manager.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.35.0rc2/src/subsearch/utils/imdb_lookup.py` & `Subsearch-2.35.0rc3/src/subsearch/utils/imdb_lookup.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.35.0rc2/src/subsearch/utils/io_json.py` & `Subsearch-2.35.0rc3/src/subsearch/utils/io_json.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.35.0rc2/src/subsearch/utils/io_winreg.py` & `Subsearch-2.35.0rc3/src/subsearch/utils/io_winreg.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.35.0rc2/src/subsearch/utils/log.py` & `Subsearch-2.35.0rc3/src/subsearch/utils/log.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.35.0rc2/src/subsearch/utils/mutex_synchronizer.py` & `Subsearch-2.35.0rc3/src/subsearch/utils/mutex_synchronizer.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.35.0rc2/src/subsearch/utils/string_parser.py` & `Subsearch-2.35.0rc3/src/subsearch/utils/string_parser.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.35.0rc2/src/subsearch/utils/update.py` & `Subsearch-2.35.0rc3/src/subsearch/utils/update.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,16 +15,16 @@
     Args:
         version (str): The input version string. This could be any string containing a semantic version,
             but it is expected that there will be only one such version in the string.
 
     Returns:
         str: The extracted semantic version string.
     """
-    # semantic expression https://regex101.com/r/M4qItH/2
-    pattern = '"(\d*\.\d*\.\d*-\w*\d*)"|"(\d*\.\d*\.\d*-\w*\.\d*)"|"(\d*\.\d*\.\d*)"'
+    # semantic expression https://regex101.com/r/M4qItH/
+    pattern = r'(?<=__version__ = ")(\d+\.\d+\.\d+[a-zA-Z]*\d*).*?(?=")'
     version_semantic = "".join(re.findall(pattern, version)[0])
     return version_semantic
 
 
 def scrape_github() -> str:
     """
     Scrape the latest version of the subsearch application from the subsearch GitHub repository.
@@ -72,30 +72,30 @@
             repo_is_prerelease = True
         new_repo_avail = True
 
     return new_repo_avail, repo_is_prerelease
 
 
 # Work in progress
-# def find_sha256(url):
-#     response = requests.get(url)
-#     html_content = response.text
-
-#     parser = selectolax.parser.HTMLParser(html_content)
-#     selector_lst = [
-#         ".clearfix",
-#         "div:nth-child(3)",
-#         "section:nth-child(1)",
-#         "div:nth-child(2)",
-#         "div:nth-child(2)",
-#         "div:nth-child(1)",
-#         "div:nth-child(1)",
-#         "div:nth-child(2)",
-#         "h6:nth-child(5)",
-#         "p:nth-child(2)",
-#     ]
-
-#     css_selector = " > ".join(selector_lst)
-
-#     element = parser.css(css_selector)
-#     match = re.search(r"([A-Fa-f0-9]{64})", element[0].html)
-#     return match[0]
+def find_sha256(url):
+    response = requests.get(url)
+    html_content = response.text
+
+    parser = selectolax.parser.HTMLParser(html_content)
+    selector_lst = [
+        ".clearfix",
+        "div:nth-child(3)",
+        "section:nth-child(1)",
+        "div:nth-child(2)",
+        "div:nth-child(2)",
+        "div:nth-child(1)",
+        "div:nth-child(1)",
+        "div:nth-child(2)",
+        "h6:nth-child(5)",
+        "p:nth-child(2)",
+    ]
+
+    css_selector = " > ".join(selector_lst)
+
+    element = parser.css(css_selector)
+    match = re.search(r"([A-Fa-f0-9]{64})", element[0].html)
+    return match[0]
```

