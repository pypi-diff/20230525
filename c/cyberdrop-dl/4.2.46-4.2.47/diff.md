# Comparing `tmp/cyberdrop-dl-4.2.46.tar.gz` & `tmp/cyberdrop-dl-4.2.47.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyberdrop-dl-4.2.46.tar", last modified: Wed May 24 01:38:05 2023, max compression
+gzip compressed data, was "cyberdrop-dl-4.2.47.tar", last modified: Thu May 25 00:49:45 2023, max compression
```

## Comparing `cyberdrop-dl-4.2.46.tar` & `cyberdrop-dl-4.2.47.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 01:38:05.560829 cyberdrop-dl-4.2.46/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-24 01:37:50.000000 cyberdrop-dl-4.2.46/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18155 2023-05-24 01:38:05.560829 cyberdrop-dl-4.2.46/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17720 2023-05-24 01:37:50.000000 cyberdrop-dl-4.2.46/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 01:38:05.556828 cyberdrop-dl-4.2.46/cyberdrop_dl/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-24 01:37:50.000000 cyberdrop-dl-4.2.46/cyberdrop_dl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 01:38:05.556828 cyberdrop-dl-4.2.46/cyberdrop_dl/base_functions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 01:37:50.000000 cyberdrop-dl-4.2.46/cyberdrop_dl/base_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6659 2023-05-24 01:37:50.000000 cyberdrop-dl-4.2.46/cyberdrop_dl/base_functions/base_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-05-24 01:37:50.000000 cyberdrop-dl-4.2.46/cyberdrop_dl/base_functions/config_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-05-24 01:37:50.000000 cyberdrop-dl-4.2.46/cyberdrop_dl/base_functions/config_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     8468 2023-05-24 01:37:50.000000 cyberdrop-dl-4.2.46/cyberdrop_dl/base_functions/data_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-24 01:37:50.000000 cyberdrop-dl-4.2.46/cyberdrop_dl/base_functions/error_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-05-24 01:37:50.000000 cyberdrop-dl-4.2.46/cyberdrop_dl/base_functions/sorting_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12707 2023-05-24 01:37:50.000000 cyberdrop-dl-4.2.46/cyberdrop_dl/base_functions/sql_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 01:38:05.556828 cyberdrop-dl-4.2.46/cyberdrop_dl/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 01:37:50.000000 cyberdrop-dl-4.2.46/cyberdrop_dl/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10285 2023-05-24 01:37:50.000000 cyberdrop-dl-4.2.46/cyberdrop_dl/client/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 01:38:05.560829 cyberdrop-dl-4.2.46/cyberdrop_dl/crawlers/
--rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-05-24 01:37:50.000000 cyberdrop-dl-4.2.46/cyberdrop_dl/crawlers/Anonfiles_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     8196 2023-05-24 01:37:50.000000 cyberdrop-dl-4.2.46/cyberdrop_dl/crawlers/Bunkr_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     7922 2023-05-24 01:37:50.000000 cyberdrop-dl-4.2.46/cyberdrop_dl/crawlers/Coomeno_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)    12903 2023-05-24 01:37:50.000000 cyberdrop-dl-4.2.46/cyberdrop_dl/crawlers/CyberFile_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-05-24 01:37:50.000000 cyberdrop-dl-4.2.46/cyberdrop_dl/crawlers/Cyberdrop_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-05-24 01:37:50.000000 cyberdrop-dl-4.2.46/cyberdrop_dl/crawlers/EHentai_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-05-24 01:37:50.000000 cyberdrop-dl-4.2.46/cyberdrop_dl/crawlers/Erome_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-05-24 01:37:50.000000 cyberdrop-dl-4.2.46/cyberdrop_dl/crawlers/Fapello_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-05-24 01:37:50.000000 cyberdrop-dl-4.2.46/cyberdrop_dl/crawlers/Gfycat_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     5821 2023-05-24 01:37:50.000000 cyberdrop-dl-4.2.46/cyberdrop_dl/crawlers/GoFile_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-05-24 01:37:50.000000 cyberdrop-dl-4.2.46/cyberdrop_dl/crawlers/HGameCG_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-05-24 01:37:50.000000 cyberdrop-dl-4.2.46/cyberdrop_dl/crawlers/ImgBox_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-05-24 01:37:50.000000 cyberdrop-dl-4.2.46/cyberdrop_dl/crawlers/LoveFap_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-05-24 01:37:50.000000 cyberdrop-dl-4.2.46/cyberdrop_dl/crawlers/NSFWXXX_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-05-24 01:37:50.000000 cyberdrop-dl-4.2.46/cyberdrop_dl/crawlers/PimpAndHost_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-05-24 01:37:50.000000 cyberdrop-dl-4.2.46/cyberdrop_dl/crawlers/PixelDrain_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-05-24 01:37:50.000000 cyberdrop-dl-4.2.46/cyberdrop_dl/crawlers/PostImg_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-05-24 01:37:50.000000 cyberdrop-dl-4.2.46/cyberdrop_dl/crawlers/Saint_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     9157 2023-05-24 01:37:50.000000 cyberdrop-dl-4.2.46/cyberdrop_dl/crawlers/ShareX_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-05-24 01:37:50.000000 cyberdrop-dl-4.2.46/cyberdrop_dl/crawlers/XBunkr_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)    13919 2023-05-24 01:37:50.000000 cyberdrop-dl-4.2.46/cyberdrop_dl/crawlers/Xenforo_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 01:37:50.000000 cyberdrop-dl-4.2.46/cyberdrop_dl/crawlers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 01:38:05.560829 cyberdrop-dl-4.2.46/cyberdrop_dl/downloader/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 01:37:50.000000 cyberdrop-dl-4.2.46/cyberdrop_dl/downloader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-05-24 01:37:50.000000 cyberdrop-dl-4.2.46/cyberdrop_dl/downloader/downloader_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    18627 2023-05-24 01:37:50.000000 cyberdrop-dl-4.2.46/cyberdrop_dl/downloader/downloaders.py
--rw-r--r--   0 runner    (1001) docker     (123)    12870 2023-05-24 01:37:50.000000 cyberdrop-dl-4.2.46/cyberdrop_dl/downloader/old_downloaders.py
--rw-r--r--   0 runner    (1001) docker     (123)    17799 2023-05-24 01:37:50.000000 cyberdrop-dl-4.2.46/cyberdrop_dl/downloader/progress_definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)    20508 2023-05-24 01:37:50.000000 cyberdrop-dl-4.2.46/cyberdrop_dl/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 01:38:05.560829 cyberdrop-dl-4.2.46/cyberdrop_dl/scraper/
--rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-05-24 01:37:50.000000 cyberdrop-dl-4.2.46/cyberdrop_dl/scraper/JDownloader_Integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    20625 2023-05-24 01:37:50.000000 cyberdrop-dl-4.2.46/cyberdrop_dl/scraper/Scraper.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 01:37:50.000000 cyberdrop-dl-4.2.46/cyberdrop_dl/scraper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 01:38:05.556828 cyberdrop-dl-4.2.46/cyberdrop_dl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18155 2023-05-24 01:38:05.000000 cyberdrop-dl-4.2.46/cyberdrop_dl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-24 01:38:05.000000 cyberdrop-dl-4.2.46/cyberdrop_dl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 01:38:05.000000 cyberdrop-dl-4.2.46/cyberdrop_dl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-24 01:38:05.000000 cyberdrop-dl-4.2.46/cyberdrop_dl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-24 01:38:05.000000 cyberdrop-dl-4.2.46/cyberdrop_dl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-24 01:38:05.000000 cyberdrop-dl-4.2.46/cyberdrop_dl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-24 01:37:50.000000 cyberdrop-dl-4.2.46/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-24 01:38:05.560829 cyberdrop-dl-4.2.46/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 01:37:50.000000 cyberdrop-dl-4.2.46/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 00:49:45.051749 cyberdrop-dl-4.2.47/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-25 00:49:36.000000 cyberdrop-dl-4.2.47/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18155 2023-05-25 00:49:45.051749 cyberdrop-dl-4.2.47/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17720 2023-05-25 00:49:36.000000 cyberdrop-dl-4.2.47/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 00:49:45.043748 cyberdrop-dl-4.2.47/cyberdrop_dl/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-25 00:49:36.000000 cyberdrop-dl-4.2.47/cyberdrop_dl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 00:49:45.047748 cyberdrop-dl-4.2.47/cyberdrop_dl/base_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 00:49:36.000000 cyberdrop-dl-4.2.47/cyberdrop_dl/base_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6659 2023-05-25 00:49:36.000000 cyberdrop-dl-4.2.47/cyberdrop_dl/base_functions/base_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-05-25 00:49:36.000000 cyberdrop-dl-4.2.47/cyberdrop_dl/base_functions/config_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-05-25 00:49:36.000000 cyberdrop-dl-4.2.47/cyberdrop_dl/base_functions/config_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8468 2023-05-25 00:49:36.000000 cyberdrop-dl-4.2.47/cyberdrop_dl/base_functions/data_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-25 00:49:36.000000 cyberdrop-dl-4.2.47/cyberdrop_dl/base_functions/error_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-05-25 00:49:36.000000 cyberdrop-dl-4.2.47/cyberdrop_dl/base_functions/sorting_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12707 2023-05-25 00:49:36.000000 cyberdrop-dl-4.2.47/cyberdrop_dl/base_functions/sql_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 00:49:45.047748 cyberdrop-dl-4.2.47/cyberdrop_dl/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 00:49:36.000000 cyberdrop-dl-4.2.47/cyberdrop_dl/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10285 2023-05-25 00:49:36.000000 cyberdrop-dl-4.2.47/cyberdrop_dl/client/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 00:49:45.051749 cyberdrop-dl-4.2.47/cyberdrop_dl/crawlers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-05-25 00:49:36.000000 cyberdrop-dl-4.2.47/cyberdrop_dl/crawlers/Anonfiles_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8196 2023-05-25 00:49:36.000000 cyberdrop-dl-4.2.47/cyberdrop_dl/crawlers/Bunkr_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7922 2023-05-25 00:49:36.000000 cyberdrop-dl-4.2.47/cyberdrop_dl/crawlers/Coomeno_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12903 2023-05-25 00:49:36.000000 cyberdrop-dl-4.2.47/cyberdrop_dl/crawlers/CyberFile_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-05-25 00:49:36.000000 cyberdrop-dl-4.2.47/cyberdrop_dl/crawlers/Cyberdrop_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-05-25 00:49:36.000000 cyberdrop-dl-4.2.47/cyberdrop_dl/crawlers/EHentai_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-05-25 00:49:36.000000 cyberdrop-dl-4.2.47/cyberdrop_dl/crawlers/Erome_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-05-25 00:49:36.000000 cyberdrop-dl-4.2.47/cyberdrop_dl/crawlers/Fapello_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-05-25 00:49:36.000000 cyberdrop-dl-4.2.47/cyberdrop_dl/crawlers/Gfycat_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5821 2023-05-25 00:49:36.000000 cyberdrop-dl-4.2.47/cyberdrop_dl/crawlers/GoFile_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-05-25 00:49:36.000000 cyberdrop-dl-4.2.47/cyberdrop_dl/crawlers/HGameCG_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-05-25 00:49:36.000000 cyberdrop-dl-4.2.47/cyberdrop_dl/crawlers/ImgBox_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-05-25 00:49:36.000000 cyberdrop-dl-4.2.47/cyberdrop_dl/crawlers/LoveFap_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-05-25 00:49:36.000000 cyberdrop-dl-4.2.47/cyberdrop_dl/crawlers/NSFWXXX_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-05-25 00:49:36.000000 cyberdrop-dl-4.2.47/cyberdrop_dl/crawlers/PimpAndHost_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-05-25 00:49:36.000000 cyberdrop-dl-4.2.47/cyberdrop_dl/crawlers/PixelDrain_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-05-25 00:49:36.000000 cyberdrop-dl-4.2.47/cyberdrop_dl/crawlers/PostImg_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-05-25 00:49:36.000000 cyberdrop-dl-4.2.47/cyberdrop_dl/crawlers/Saint_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9157 2023-05-25 00:49:36.000000 cyberdrop-dl-4.2.47/cyberdrop_dl/crawlers/ShareX_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-05-25 00:49:36.000000 cyberdrop-dl-4.2.47/cyberdrop_dl/crawlers/XBunkr_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13919 2023-05-25 00:49:36.000000 cyberdrop-dl-4.2.47/cyberdrop_dl/crawlers/Xenforo_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 00:49:36.000000 cyberdrop-dl-4.2.47/cyberdrop_dl/crawlers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 00:49:45.051749 cyberdrop-dl-4.2.47/cyberdrop_dl/downloader/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 00:49:36.000000 cyberdrop-dl-4.2.47/cyberdrop_dl/downloader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-05-25 00:49:36.000000 cyberdrop-dl-4.2.47/cyberdrop_dl/downloader/downloader_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18627 2023-05-25 00:49:36.000000 cyberdrop-dl-4.2.47/cyberdrop_dl/downloader/downloaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12870 2023-05-25 00:49:36.000000 cyberdrop-dl-4.2.47/cyberdrop_dl/downloader/old_downloaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17799 2023-05-25 00:49:36.000000 cyberdrop-dl-4.2.47/cyberdrop_dl/downloader/progress_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20508 2023-05-25 00:49:36.000000 cyberdrop-dl-4.2.47/cyberdrop_dl/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 00:49:45.051749 cyberdrop-dl-4.2.47/cyberdrop_dl/scraper/
+-rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-05-25 00:49:36.000000 cyberdrop-dl-4.2.47/cyberdrop_dl/scraper/JDownloader_Integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20625 2023-05-25 00:49:36.000000 cyberdrop-dl-4.2.47/cyberdrop_dl/scraper/Scraper.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 00:49:36.000000 cyberdrop-dl-4.2.47/cyberdrop_dl/scraper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 00:49:45.043748 cyberdrop-dl-4.2.47/cyberdrop_dl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18155 2023-05-25 00:49:45.000000 cyberdrop-dl-4.2.47/cyberdrop_dl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-25 00:49:45.000000 cyberdrop-dl-4.2.47/cyberdrop_dl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 00:49:45.000000 cyberdrop-dl-4.2.47/cyberdrop_dl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-25 00:49:45.000000 cyberdrop-dl-4.2.47/cyberdrop_dl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-25 00:49:45.000000 cyberdrop-dl-4.2.47/cyberdrop_dl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-25 00:49:45.000000 cyberdrop-dl-4.2.47/cyberdrop_dl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-25 00:49:36.000000 cyberdrop-dl-4.2.47/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-25 00:49:45.051749 cyberdrop-dl-4.2.47/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 00:49:36.000000 cyberdrop-dl-4.2.47/setup.py
```

### Comparing `cyberdrop-dl-4.2.46/LICENSE` & `cyberdrop-dl-4.2.47/LICENSE`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.46/PKG-INFO` & `cyberdrop-dl-4.2.47/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyberdrop-dl
-Version: 4.2.46
+Version: 4.2.47
 Summary: Bulk downloader for multiple file hosts and forum sites
 Home-page: https://github.com/Jules-WinnfieldX/CyberDropDownloader
 Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com
 Project-URL: Bug Tracker, https://github.com/Jules-WinnfieldX/CyberDropDownloader/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.2.46 Summary: Bulk
+Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.2.47 Summary: Bulk
 downloader for multiple file hosts and forum sites Home-page: https://
 github.com/Jules-WinnfieldX/CyberDropDownloader Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com Project-URL: Bug Tracker, https:/
 /github.com/Jules-WinnfieldX/CyberDropDownloader/issues Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE # `cyberdrop-dl`
 **Bulk downloader for multiple file hosts** [![PyPI version](https://
 badge.fury.io/py/cyberdrop-dl.svg)](https://badge.fury.io/py/cyberdrop-dl) [!
```

### Comparing `cyberdrop-dl-4.2.46/README.md` & `cyberdrop-dl-4.2.47/README.md`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.46/cyberdrop_dl/base_functions/base_functions.py` & `cyberdrop-dl-4.2.47/cyberdrop_dl/base_functions/base_functions.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.46/cyberdrop_dl/base_functions/config_manager.py` & `cyberdrop-dl-4.2.47/cyberdrop_dl/base_functions/config_manager.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.46/cyberdrop_dl/base_functions/config_schema.py` & `cyberdrop-dl-4.2.47/cyberdrop_dl/base_functions/config_schema.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.46/cyberdrop_dl/base_functions/data_classes.py` & `cyberdrop-dl-4.2.47/cyberdrop_dl/base_functions/data_classes.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.46/cyberdrop_dl/base_functions/error_classes.py` & `cyberdrop-dl-4.2.47/cyberdrop_dl/base_functions/error_classes.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.46/cyberdrop_dl/base_functions/sorting_functions.py` & `cyberdrop-dl-4.2.47/cyberdrop_dl/base_functions/sorting_functions.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.46/cyberdrop_dl/base_functions/sql_helper.py` & `cyberdrop-dl-4.2.47/cyberdrop_dl/base_functions/sql_helper.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.46/cyberdrop_dl/client/client.py` & `cyberdrop-dl-4.2.47/cyberdrop_dl/client/client.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.46/cyberdrop_dl/crawlers/Anonfiles_Spider.py` & `cyberdrop-dl-4.2.47/cyberdrop_dl/crawlers/Anonfiles_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.46/cyberdrop_dl/crawlers/Bunkr_Spider.py` & `cyberdrop-dl-4.2.47/cyberdrop_dl/crawlers/Bunkr_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.46/cyberdrop_dl/crawlers/Coomeno_Spider.py` & `cyberdrop-dl-4.2.47/cyberdrop_dl/crawlers/Coomeno_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.46/cyberdrop_dl/crawlers/CyberFile_Spider.py` & `cyberdrop-dl-4.2.47/cyberdrop_dl/crawlers/CyberFile_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.46/cyberdrop_dl/crawlers/Cyberdrop_Spider.py` & `cyberdrop-dl-4.2.47/cyberdrop_dl/crawlers/Cyberdrop_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.46/cyberdrop_dl/crawlers/EHentai_Spider.py` & `cyberdrop-dl-4.2.47/cyberdrop_dl/crawlers/EHentai_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.46/cyberdrop_dl/crawlers/Erome_Spider.py` & `cyberdrop-dl-4.2.47/cyberdrop_dl/crawlers/Erome_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.46/cyberdrop_dl/crawlers/Fapello_Spider.py` & `cyberdrop-dl-4.2.47/cyberdrop_dl/crawlers/Fapello_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.46/cyberdrop_dl/crawlers/Gfycat_Spider.py` & `cyberdrop-dl-4.2.47/cyberdrop_dl/crawlers/Gfycat_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.46/cyberdrop_dl/crawlers/GoFile_Spider.py` & `cyberdrop-dl-4.2.47/cyberdrop_dl/crawlers/GoFile_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.46/cyberdrop_dl/crawlers/HGameCG_Spider.py` & `cyberdrop-dl-4.2.47/cyberdrop_dl/crawlers/HGameCG_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.46/cyberdrop_dl/crawlers/ImgBox_Spider.py` & `cyberdrop-dl-4.2.47/cyberdrop_dl/crawlers/ImgBox_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.46/cyberdrop_dl/crawlers/LoveFap_Spider.py` & `cyberdrop-dl-4.2.47/cyberdrop_dl/crawlers/LoveFap_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.46/cyberdrop_dl/crawlers/NSFWXXX_Spider.py` & `cyberdrop-dl-4.2.47/cyberdrop_dl/crawlers/NSFWXXX_Spider.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,14 +33,17 @@
         else:
             await self.get_post(session, url, domain_obj)
         await self.SQL_Helper.insert_domain("nsfw.xxx", url, domain_obj)
         return domain_obj
 
     async def get_user(self, session: ScrapeSession, url: URL, domain_obj: DomainItem) -> None:
         """Gets posts for a user profile"""
+        if str(url).endswith("/"):
+            url = url.parent
+
         try:
             model = url.name + " (NSFW.XXX)"
             for page in itertools.count(1):
                 model_name_parts = url.path.split("/")
                 model_name = list(filter(None, model_name_parts))[-1]
                 page_url = URL(f"https://nsfw.xxx/page/{page}?nsfw[]=0&types[]=image&types[]=video&types[]=gallery&slider=1&jsload=1&user={model_name}")
                 page_soup = await session.get_BS4(page_url)
```

### Comparing `cyberdrop-dl-4.2.46/cyberdrop_dl/crawlers/PimpAndHost_Spider.py` & `cyberdrop-dl-4.2.47/cyberdrop_dl/crawlers/PimpAndHost_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.46/cyberdrop_dl/crawlers/PixelDrain_Spider.py` & `cyberdrop-dl-4.2.47/cyberdrop_dl/crawlers/PixelDrain_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.46/cyberdrop_dl/crawlers/PostImg_Spider.py` & `cyberdrop-dl-4.2.47/cyberdrop_dl/crawlers/PostImg_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.46/cyberdrop_dl/crawlers/Saint_Spider.py` & `cyberdrop-dl-4.2.47/cyberdrop_dl/crawlers/Saint_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.46/cyberdrop_dl/crawlers/ShareX_Spider.py` & `cyberdrop-dl-4.2.47/cyberdrop_dl/crawlers/ShareX_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.46/cyberdrop_dl/crawlers/XBunkr_Spider.py` & `cyberdrop-dl-4.2.47/cyberdrop_dl/crawlers/XBunkr_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.46/cyberdrop_dl/crawlers/Xenforo_Spider.py` & `cyberdrop-dl-4.2.47/cyberdrop_dl/crawlers/Xenforo_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.46/cyberdrop_dl/downloader/downloader_utils.py` & `cyberdrop-dl-4.2.47/cyberdrop_dl/downloader/downloader_utils.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.46/cyberdrop_dl/downloader/downloaders.py` & `cyberdrop-dl-4.2.47/cyberdrop_dl/downloader/downloaders.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.46/cyberdrop_dl/downloader/old_downloaders.py` & `cyberdrop-dl-4.2.47/cyberdrop_dl/downloader/old_downloaders.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.46/cyberdrop_dl/downloader/progress_definitions.py` & `cyberdrop-dl-4.2.47/cyberdrop_dl/downloader/progress_definitions.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.46/cyberdrop_dl/main.py` & `cyberdrop-dl-4.2.47/cyberdrop_dl/main.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.46/cyberdrop_dl/scraper/JDownloader_Integration.py` & `cyberdrop-dl-4.2.47/cyberdrop_dl/scraper/JDownloader_Integration.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.46/cyberdrop_dl/scraper/Scraper.py` & `cyberdrop-dl-4.2.47/cyberdrop_dl/scraper/Scraper.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.46/cyberdrop_dl.egg-info/PKG-INFO` & `cyberdrop-dl-4.2.47/cyberdrop_dl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyberdrop-dl
-Version: 4.2.46
+Version: 4.2.47
 Summary: Bulk downloader for multiple file hosts and forum sites
 Home-page: https://github.com/Jules-WinnfieldX/CyberDropDownloader
 Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com
 Project-URL: Bug Tracker, https://github.com/Jules-WinnfieldX/CyberDropDownloader/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.2.46 Summary: Bulk
+Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.2.47 Summary: Bulk
 downloader for multiple file hosts and forum sites Home-page: https://
 github.com/Jules-WinnfieldX/CyberDropDownloader Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com Project-URL: Bug Tracker, https:/
 /github.com/Jules-WinnfieldX/CyberDropDownloader/issues Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE # `cyberdrop-dl`
 **Bulk downloader for multiple file hosts** [![PyPI version](https://
 badge.fury.io/py/cyberdrop-dl.svg)](https://badge.fury.io/py/cyberdrop-dl) [!
```

### Comparing `cyberdrop-dl-4.2.46/cyberdrop_dl.egg-info/SOURCES.txt` & `cyberdrop-dl-4.2.47/cyberdrop_dl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.46/setup.cfg` & `cyberdrop-dl-4.2.47/setup.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -13,23 +13,23 @@
 [options]
 python_requires = >=3.7
 include_package_data = True
 packages = find:
 install_requires = 
 	aiofiles>=23.1.0
 	aiohttp>=3.8.4
-	aiolimiter>=1.0.0
+	aiolimiter>=1.1.0
 	beautifulsoup4>=4.12.2
-	certifi>=2022.12.7
+	certifi>=2023.5.7
 	myjdapi>=1.1.6
 	PyYAML>=6.0
-	rich>=13.3.4
-	setuptools>=67.7.2
-	yarl==1.8.2
+	rich>=13.3.5
+	setuptools>=67.8.0
 	tqdm>=4.65.0
+	yarl>=1.9.2
 
 [options.entry_points]
 console_scripts = 
 	cyberdrop-dl = cyberdrop_dl.main:main
 
 [egg_info]
 tag_build =
```

