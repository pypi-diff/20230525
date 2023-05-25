# Comparing `tmp/py-Ayiin-0.3.6.tar.gz` & `tmp/py-Ayiin-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-Ayiin-0.3.6.tar", last modified: Wed May 24 16:22:41 2023, max compression
+gzip compressed data, was "py-Ayiin-0.3.7.tar", last modified: Thu May 25 01:36:01 2023, max compression
```

## Comparing `py-Ayiin-0.3.6.tar` & `py-Ayiin-0.3.7.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:22:41.602433 py-Ayiin-0.3.6/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-24 16:22:21.000000 py-Ayiin-0.3.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-24 16:22:21.000000 py-Ayiin-0.3.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-24 16:22:21.000000 py-Ayiin-0.3.6/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-05-24 16:22:41.602433 py-Ayiin-0.3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-05-24 16:22:21.000000 py-Ayiin-0.3.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:22:41.598433 py-Ayiin-0.3.6/pyAyiin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:22:41.598433 py-Ayiin-0.3.6/pyAyiin/Clients/
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-24 16:22:21.000000 py-Ayiin-0.3.6/pyAyiin/Clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12137 2023-05-24 16:22:21.000000 py-Ayiin-0.3.6/pyAyiin/Clients/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-05-24 16:22:21.000000 py-Ayiin-0.3.6/pyAyiin/Clients/pytgcalls.py
--rw-r--r--   0 runner    (1001) docker     (123)    38642 2023-05-24 16:22:21.000000 py-Ayiin-0.3.6/pyAyiin/Clients/startup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-05-24 16:22:21.000000 py-Ayiin-0.3.6/pyAyiin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-05-24 16:22:21.000000 py-Ayiin-0.3.6/pyAyiin/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-05-24 16:22:21.000000 py-Ayiin-0.3.6/pyAyiin/assistant.py
--rw-r--r--   0 runner    (1001) docker     (123)     5126 2023-05-24 16:22:21.000000 py-Ayiin-0.3.6/pyAyiin/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:22:41.598433 py-Ayiin-0.3.6/pyAyiin/dB/
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-05-24 16:22:21.000000 py-Ayiin-0.3.6/pyAyiin/dB/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-24 16:22:21.000000 py-Ayiin-0.3.6/pyAyiin/dB/_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-05-24 16:22:21.000000 py-Ayiin-0.3.6/pyAyiin/dB/absen.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-24 16:22:21.000000 py-Ayiin-0.3.6/pyAyiin/dB/admins.py
--rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-05-24 16:22:21.000000 py-Ayiin-0.3.6/pyAyiin/dB/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-05-24 16:22:21.000000 py-Ayiin-0.3.6/pyAyiin/dB/blacklistfilter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-24 16:22:21.000000 py-Ayiin-0.3.6/pyAyiin/dB/blacklistgcast.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-24 16:22:21.000000 py-Ayiin-0.3.6/pyAyiin/dB/blacklistuser.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-24 16:22:21.000000 py-Ayiin-0.3.6/pyAyiin/dB/gban.py
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-05-24 16:22:21.000000 py-Ayiin-0.3.6/pyAyiin/dB/langs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-24 16:22:21.000000 py-Ayiin-0.3.6/pyAyiin/dB/logdb.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-24 16:22:21.000000 py-Ayiin-0.3.6/pyAyiin/dB/pmpermit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-05-24 16:22:21.000000 py-Ayiin-0.3.6/pyAyiin/dB/premium.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-24 16:22:21.000000 py-Ayiin-0.3.6/pyAyiin/dB/start.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-24 16:22:21.000000 py-Ayiin-0.3.6/pyAyiin/dB/sudo.py
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-24 16:22:21.000000 py-Ayiin-0.3.6/pyAyiin/dB/variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-05-24 16:22:21.000000 py-Ayiin-0.3.6/pyAyiin/dB/videocalls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-05-24 16:22:21.000000 py-Ayiin-0.3.6/pyAyiin/dB/welcome.py
--rw-r--r--   0 runner    (1001) docker     (123)    33254 2023-05-24 16:22:21.000000 py-Ayiin-0.3.6/pyAyiin/decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-24 16:22:21.000000 py-Ayiin-0.3.6/pyAyiin/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:22:41.598433 py-Ayiin-0.3.6/pyAyiin/methods/
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-24 16:22:21.000000 py-Ayiin-0.3.6/pyAyiin/methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-05-24 16:22:21.000000 py-Ayiin-0.3.6/pyAyiin/methods/_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-05-24 16:22:21.000000 py-Ayiin-0.3.6/pyAyiin/methods/changer.py
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-24 16:22:21.000000 py-Ayiin-0.3.6/pyAyiin/methods/converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-05-24 16:22:21.000000 py-Ayiin-0.3.6/pyAyiin/methods/func.py
--rw-r--r--   0 runner    (1001) docker     (123)     6181 2023-05-24 16:22:21.000000 py-Ayiin-0.3.6/pyAyiin/methods/funcb.py
--rw-r--r--   0 runner    (1001) docker     (123)     8828 2023-05-24 16:22:21.000000 py-Ayiin-0.3.6/pyAyiin/methods/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-05-24 16:22:21.000000 py-Ayiin-0.3.6/pyAyiin/methods/hosting.py
--rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-05-24 16:22:21.000000 py-Ayiin-0.3.6/pyAyiin/methods/inlinebot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-05-24 16:22:21.000000 py-Ayiin-0.3.6/pyAyiin/methods/queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     5704 2023-05-24 16:22:21.000000 py-Ayiin-0.3.6/pyAyiin/methods/thumbnail.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:22:41.598433 py-Ayiin-0.3.6/pyAyiin/pyrogram/
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-24 16:22:21.000000 py-Ayiin-0.3.6/pyAyiin/pyrogram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-05-24 16:22:21.000000 py-Ayiin-0.3.6/pyAyiin/pyrogram/_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)    13157 2023-05-24 16:22:21.000000 py-Ayiin-0.3.6/pyAyiin/pyrogram/func.py
--rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-05-24 16:22:21.000000 py-Ayiin-0.3.6/pyAyiin/pyrogram/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-05-24 16:22:21.000000 py-Ayiin-0.3.6/pyAyiin/pyrogram/pastebin.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-24 16:22:21.000000 py-Ayiin-0.3.6/pyAyiin/pyrogram/sections.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-05-24 16:22:21.000000 py-Ayiin-0.3.6/pyAyiin/pyrogram/toolbot.py
--rw-r--r--   0 runner    (1001) docker     (123)     8684 2023-05-24 16:22:21.000000 py-Ayiin-0.3.6/pyAyiin/pyrogram/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:22:41.598433 py-Ayiin-0.3.6/pyAyiin/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 16:22:21.000000 py-Ayiin-0.3.6/pyAyiin/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:22:41.602433 py-Ayiin-0.3.6/pyAyiin/telethon/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-24 16:22:21.000000 py-Ayiin-0.3.6/pyAyiin/telethon/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:22:41.602433 py-Ayiin-0.3.6/pyAyiin/telethon/ayiin/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-24 16:22:21.000000 py-Ayiin-0.3.6/pyAyiin/telethon/ayiin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-05-24 16:22:21.000000 py-Ayiin-0.3.6/pyAyiin/telethon/ayiin/_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-05-24 16:22:21.000000 py-Ayiin-0.3.6/pyAyiin/telethon/ayiin/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-05-24 16:22:21.000000 py-Ayiin-0.3.6/pyAyiin/telethon/ayiin/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    17263 2023-05-24 16:22:21.000000 py-Ayiin-0.3.6/pyAyiin/xd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:22:41.602433 py-Ayiin-0.3.6/py_Ayiin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-05-24 16:22:41.000000 py-Ayiin-0.3.6/py_Ayiin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-05-24 16:22:41.000000 py-Ayiin-0.3.6/py_Ayiin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 16:22:41.000000 py-Ayiin-0.3.6/py_Ayiin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-24 16:22:41.000000 py-Ayiin-0.3.6/py_Ayiin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-24 16:22:41.000000 py-Ayiin-0.3.6/py_Ayiin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-24 16:22:21.000000 py-Ayiin-0.3.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 16:22:41.602433 py-Ayiin-0.3.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-24 16:22:21.000000 py-Ayiin-0.3.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 01:36:01.969534 py-Ayiin-0.3.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-05-25 01:36:01.969534 py-Ayiin-0.3.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 01:36:01.961534 py-Ayiin-0.3.7/pyAyiin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 01:36:01.961534 py-Ayiin-0.3.7/pyAyiin/Clients/
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/pyAyiin/Clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12568 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/pyAyiin/Clients/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6130 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/pyAyiin/Clients/pytgcalls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38642 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/pyAyiin/Clients/startup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/pyAyiin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/pyAyiin/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/pyAyiin/assistant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5126 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/pyAyiin/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 01:36:01.965534 py-Ayiin-0.3.7/pyAyiin/dB/
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/pyAyiin/dB/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/pyAyiin/dB/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/pyAyiin/dB/absen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/pyAyiin/dB/admins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/pyAyiin/dB/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/pyAyiin/dB/blacklistfilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/pyAyiin/dB/blacklistgcast.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/pyAyiin/dB/blacklistuser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/pyAyiin/dB/gban.py
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/pyAyiin/dB/langs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/pyAyiin/dB/logdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/pyAyiin/dB/pmpermit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/pyAyiin/dB/premium.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/pyAyiin/dB/start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/pyAyiin/dB/sudo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/pyAyiin/dB/variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/pyAyiin/dB/videocalls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/pyAyiin/dB/welcome.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33254 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/pyAyiin/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/pyAyiin/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 01:36:01.965534 py-Ayiin-0.3.7/pyAyiin/methods/
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/pyAyiin/methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/pyAyiin/methods/_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/pyAyiin/methods/changer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/pyAyiin/methods/converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6903 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/pyAyiin/methods/func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6181 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/pyAyiin/methods/funcb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8828 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/pyAyiin/methods/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/pyAyiin/methods/hosting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/pyAyiin/methods/inlinebot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/pyAyiin/methods/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5968 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/pyAyiin/methods/thumbnail.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 01:36:01.969534 py-Ayiin-0.3.7/pyAyiin/pyrogram/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/pyAyiin/pyrogram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/pyAyiin/pyrogram/_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13157 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/pyAyiin/pyrogram/func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/pyAyiin/pyrogram/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/pyAyiin/pyrogram/pastebin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/pyAyiin/pyrogram/sections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/pyAyiin/pyrogram/toolbot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8684 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/pyAyiin/pyrogram/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 01:36:01.969534 py-Ayiin-0.3.7/pyAyiin/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/pyAyiin/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 01:36:01.969534 py-Ayiin-0.3.7/pyAyiin/telethon/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/pyAyiin/telethon/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 01:36:01.969534 py-Ayiin-0.3.7/pyAyiin/telethon/ayiin/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/pyAyiin/telethon/ayiin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/pyAyiin/telethon/ayiin/_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/pyAyiin/telethon/ayiin/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/pyAyiin/telethon/ayiin/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17263 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/pyAyiin/xd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 01:36:01.969534 py-Ayiin-0.3.7/py_Ayiin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-05-25 01:36:01.000000 py-Ayiin-0.3.7/py_Ayiin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-05-25 01:36:01.000000 py-Ayiin-0.3.7/py_Ayiin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 01:36:01.000000 py-Ayiin-0.3.7/py_Ayiin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-25 01:36:01.000000 py-Ayiin-0.3.7/py_Ayiin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-25 01:36:01.000000 py-Ayiin-0.3.7/py_Ayiin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 01:36:01.969534 py-Ayiin-0.3.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/setup.py
```

### Comparing `py-Ayiin-0.3.6/LICENSE` & `py-Ayiin-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.6/NOTICE` & `py-Ayiin-0.3.7/NOTICE`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.6/PKG-INFO` & `py-Ayiin-0.3.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-Ayiin
-Version: 0.3.6
+Version: 0.3.7
 Summary: A Secure and Powerful Python-Telethon Based and Python-Pyrogram Based Library For Your Userbot Module.
 Home-page: https://github.com/AyiinXd/AyiinXd
 Author: AyiinXd
 Author-email: ayingaming98@gmail.com
 License: GNU General Public License v3.0 (GPL-3.0)
 Project-URL: Bug Tracker, https://github.com/AyiinXd/AyiinXd/issues
 Project-URL: Source Code, https://github.com/AyiinXd/AyiinXd
```

### Comparing `py-Ayiin-0.3.6/README.md` & `py-Ayiin-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.6/pyAyiin/Clients/__init__.py` & `py-Ayiin-0.3.7/pyAyiin/Clients/__init__.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.6/pyAyiin/Clients/client.py` & `py-Ayiin-0.3.7/pyAyiin/Clients/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,29 @@
+import logging
+
 from pyrogram import Client as PyroClient
 from fipper import Client
 
 from telethon import TelegramClient
 from telethon.sessions import MemorySession
 
 from . import *
 
 from ..config import Var as Variable
 
+
+logs = logging.getLogger('[ Import Error ] -')
+
+try:
+    import pytgcalls
+except ImportError:
+    logs.info("'pytgcalls' not found")
+    pytgcalls = None
+
+
 Var = Variable()
 
 
 hndlr = f"{Var.HNDLR[0]} {Var.HNDLR[1]} {Var.HNDLR[2]} {Var.HNDLR[3]} {Var.HNDLR[4]} {Var.HNDLR[5]}"
 
 
 
@@ -684,7 +696,16 @@
         AYIIN46,
         AYIIN47,
         AYIIN48,
         AYIIN49,
         AYIIN50,
     ] if bot
 ]
+
+
+if pytgcalls is not None:
+    for bot in Bots:
+        if not hasattr(bot, "group_call"):
+            try:
+                setattr(bot, "group_call", pytgcalls.GroupCallFactory(bot).get_group_call())
+            except AttributeError:
+                pass
```

### Comparing `py-Ayiin-0.3.6/pyAyiin/Clients/startup.py` & `py-Ayiin-0.3.7/pyAyiin/Clients/startup.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.6/pyAyiin/__init__.py` & `py-Ayiin-0.3.7/pyAyiin/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
 
 logs = logging.getLogger(__name__)
 
 
 __copyright__ = "Copyright (C) 2022-present AyiinXd <https://github.com/AyiinXd>"
 __license__ = "GNU General Public License v3.0 (GPL-3.0)"
-__version__ = "0.3.6"
+__version__ = "0.3.7"
 ayiin_ver = "0.1.1"
 
 
 DEVS = [
     607067484, # Ayiin
     997461844, #Ayang_Ayiin
     2130526178, # Alfa
```

### Comparing `py-Ayiin-0.3.6/pyAyiin/__main__.py` & `py-Ayiin-0.3.7/pyAyiin/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from fipper import idle
 
 from pyAyiin import __version__
 
 from . import *
 
 from .config import Var
+from .Clients.client import Bots
 from .Clients.startup import StartPyrogram
 from .exceptions import DependencyMissingError
 
 yinsxd = Var()
 xd = PyrogramXd()
 
 
@@ -26,27 +27,30 @@
 MSG_ON = """
 <b>❏ ᴀʏɪɪɴ - ᴜʙᴏᴛ ʙᴇʀʜᴀsɪʟ ᴅɪᴀᴋᴛɪғᴋᴀɴ</b>
 <b>╭╼┅━━━━━╍━━━━━┅╾</b>
 <b>├▹ Pʏ-Aʏɪɪɴ Vᴇʀsɪᴏɴ</b> - •[<code>{}</code>]•
 <b>├▹ Hᴏsᴛɪɴɢ</b> - <code>{}</code>
 <b>├▹ Usᴇʀʙᴏᴛ Vᴇʀsɪᴏɴ</b> - <code>{}</code>
 <b>├▹ Tᴏᴛᴀʟ Pʟᴜɢɪɴs</b> - <code>{}</code>
+<b>├▹ Tᴏᴛᴀʟ Usᴇʀs</b> - <code>{}</code>
 <b>╰╼┅━━━━━╍━━━━━┅╾</b>
 """
 
+
 async def start_main():
     await StartPyrogram()
     try:
         await tgbot.send_message(
             yinsxd.LOG_CHAT,
             MSG_ON.format(
                 __version__,
                 HOSTED_ON,
                 ayiin_ver, 
                 len(CMD_HELP),
+                len(Bots),
             )
         )
     except BaseException as s:
         print(s)
     print(f"AyiinUbot Version - {ayiin_ver}\n[🔥 BERHASIL DIAKTIFKAN! 🔥]")
     await idle()
     await aiosession.close()
```

### Comparing `py-Ayiin-0.3.6/pyAyiin/assistant.py` & `py-Ayiin-0.3.7/pyAyiin/assistant.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.6/pyAyiin/config.py` & `py-Ayiin-0.3.7/pyAyiin/config.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.6/pyAyiin/dB/__init__.py` & `py-Ayiin-0.3.7/pyAyiin/dB/__init__.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.6/pyAyiin/dB/absen.py` & `py-Ayiin-0.3.7/pyAyiin/dB/absen.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.6/pyAyiin/dB/admins.py` & `py-Ayiin-0.3.7/pyAyiin/dB/admins.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.6/pyAyiin/dB/auth.py` & `py-Ayiin-0.3.7/pyAyiin/dB/auth.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.6/pyAyiin/dB/blacklistfilter.py` & `py-Ayiin-0.3.7/pyAyiin/dB/blacklistfilter.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.6/pyAyiin/dB/blacklistgcast.py` & `py-Ayiin-0.3.7/pyAyiin/dB/blacklistgcast.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.6/pyAyiin/dB/blacklistuser.py` & `py-Ayiin-0.3.7/pyAyiin/dB/blacklistuser.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.6/pyAyiin/dB/gban.py` & `py-Ayiin-0.3.7/pyAyiin/dB/gban.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.6/pyAyiin/dB/langs.py` & `py-Ayiin-0.3.7/pyAyiin/dB/langs.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.6/pyAyiin/dB/logdb.py` & `py-Ayiin-0.3.7/pyAyiin/dB/logdb.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.6/pyAyiin/dB/pmpermit.py` & `py-Ayiin-0.3.7/pyAyiin/dB/pmpermit.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.6/pyAyiin/dB/premium.py` & `py-Ayiin-0.3.7/pyAyiin/dB/premium.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.6/pyAyiin/dB/start.py` & `py-Ayiin-0.3.7/pyAyiin/dB/start.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.6/pyAyiin/dB/sudo.py` & `py-Ayiin-0.3.7/pyAyiin/dB/sudo.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.6/pyAyiin/dB/variable.py` & `py-Ayiin-0.3.7/pyAyiin/dB/variable.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.6/pyAyiin/dB/videocalls.py` & `py-Ayiin-0.3.7/pyAyiin/dB/videocalls.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.6/pyAyiin/dB/welcome.py` & `py-Ayiin-0.3.7/pyAyiin/dB/welcome.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.6/pyAyiin/decorator.py` & `py-Ayiin-0.3.7/pyAyiin/decorator.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.6/pyAyiin/exceptions.py` & `py-Ayiin-0.3.7/pyAyiin/exceptions.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.6/pyAyiin/methods/__init__.py` & `py-Ayiin-0.3.7/pyAyiin/methods/__init__.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.6/pyAyiin/methods/_misc.py` & `py-Ayiin-0.3.7/pyAyiin/methods/_misc.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.6/pyAyiin/methods/changer.py` & `py-Ayiin-0.3.7/pyAyiin/methods/changer.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.6/pyAyiin/methods/converter.py` & `py-Ayiin-0.3.7/pyAyiin/methods/converter.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.6/pyAyiin/methods/funcb.py` & `py-Ayiin-0.3.7/pyAyiin/methods/funcb.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.6/pyAyiin/methods/helpers.py` & `py-Ayiin-0.3.7/pyAyiin/methods/helpers.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.6/pyAyiin/methods/hosting.py` & `py-Ayiin-0.3.7/pyAyiin/methods/hosting.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.6/pyAyiin/methods/inlinebot.py` & `py-Ayiin-0.3.7/pyAyiin/methods/inlinebot.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.6/pyAyiin/methods/queue.py` & `py-Ayiin-0.3.7/pyAyiin/methods/queue.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.6/pyAyiin/methods/thumbnail.py` & `py-Ayiin-0.3.7/pyAyiin/methods/thumbnail.py`

 * *Files 9% similar despite different names*

```diff
@@ -35,17 +35,29 @@
         heightRatio = maxHeight / image.size[1]
         newWidth = int(widthRatio * image.size[0])
         newHeight = int(heightRatio * image.size[1])
         newImage = image.resize((newWidth, newHeight))
         return newImage
 
 
-    async def gen_thumb(self, client, videoid):
-        if os.path.isfile(f"cache/{videoid}.png"):
-            return f"cache/{videoid}.png"
+    async def gen_thumb(
+        self, 
+        client, 
+        videoid,
+        cache,
+        cache_thumb,
+        fonts,
+        fonts2,
+    ):
+        # cache = f"cache/{videoid}.png"
+        # cache_thumb = f"cache/thumb{videoid}.png"
+        # fonts = "assets/font.ttf"
+        # fonts2 = "assets/font2.ttf"
+        if os.path.isfile(cache):
+            return cache
 
         url = f"https://www.youtube.com/watch?v={videoid}"
         try:
             results = VideosSearch(url, limit=1)
             for result in (await results.next())["result"]:
                 try:
                     title = result["title"]
@@ -67,20 +79,20 @@
                 except BaseException:
                     channel = "Unknown Channel"
 
             async with aiohttp.ClientSession() as session:
                 async with session.get(thumbnail) as resp:
                     if resp.status == 200:
                         f = await aiofiles.open(
-                            f"cache/thumb{videoid}.png", mode="wb"
+                            cache_thumb, mode="wb"
                         )
                         await f.write(await resp.read())
                         await f.close()
 
-            youtube = Image.open(f"cache/thumb{videoid}.png")
+            youtube = Image.open(cache_thumb)
             image1 = self.changeImageSize(1280, 720, youtube)
             image2 = image1.convert("RGBA")
             background = image2.filter(filter=ImageFilter.BoxBlur(30))
             enhancer = ImageEnhance.Brightness(background)
             background = enhancer.enhance(0.6)
             Xcenter = youtube.width / 2
             Ycenter = youtube.height / 2
@@ -89,18 +101,18 @@
             x2 = Xcenter + 250
             y2 = Ycenter + 250
             logo = youtube.crop((x1, y1, x2, y2))
             logo.thumbnail((520, 520), Image.ANTIALIAS)
             logo = ImageOps.expand(logo, border=15, fill="white")
             background.paste(logo, (50, 100))
             draw = ImageDraw.Draw(background)
-            font = ImageFont.truetype("assets/font2.ttf", 40)
-            font2 = ImageFont.truetype("assets/font2.ttf", 70)
-            arial = ImageFont.truetype("assets/font2.ttf", 30)
-            name_font = ImageFont.truetype("assets/font.ttf", 35)
+            font = ImageFont.truetype(fonts2, 40)
+            font2 = ImageFont.truetype(fonts2, 70)
+            arial = ImageFont.truetype(fonts2, 30)
+            name_font = ImageFont.truetype(fonts, 35)
             para = textwrap.wrap(title, width=32)
             me = await client.get_me()
             uname = me.username
             music_name = f'{uname.upper()} UBOT' if uname else 'AYIIN UBOT'
             j = 0
             draw.text(
                 (30, 5), f"{music_name}", fill="white", font=name_font
@@ -150,14 +162,17 @@
             draw.text(
                 (600, 550),
                 f"Channel : {channel}",
                 (255, 255, 255),
                 font=arial,
             )
             try:
-                os.remove(f"cache/thumb{videoid}.png")
+                os.remove(cache_thumb)
             except BaseException:
                 pass
-            background.save(f"cache/{videoid}.png")
-            return f"cache/{videoid}.png"
+            background.save(cache)
+            return cache
         except Exception:
-            return 'resources/Youtube.jpeg'
+            results = VideosSearch(url, limit=1)
+            for result in results.result()["result"]:
+                thumbnail = result["thumbnails"][0]["url"].split("?")[0]
+            return thumbnail
```

### Comparing `py-Ayiin-0.3.6/pyAyiin/pyrogram/__init__.py` & `py-Ayiin-0.3.7/pyAyiin/pyrogram/__init__.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.6/pyAyiin/pyrogram/_wrappers.py` & `py-Ayiin-0.3.7/pyAyiin/pyrogram/_wrappers.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.6/pyAyiin/pyrogram/func.py` & `py-Ayiin-0.3.7/pyAyiin/pyrogram/func.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.6/pyAyiin/pyrogram/misc.py` & `py-Ayiin-0.3.7/pyAyiin/pyrogram/misc.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.6/pyAyiin/pyrogram/pastebin.py` & `py-Ayiin-0.3.7/pyAyiin/pyrogram/pastebin.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.6/pyAyiin/pyrogram/sections.py` & `py-Ayiin-0.3.7/pyAyiin/pyrogram/sections.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.6/pyAyiin/pyrogram/toolbot.py` & `py-Ayiin-0.3.7/pyAyiin/pyrogram/toolbot.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.6/pyAyiin/pyrogram/tools.py` & `py-Ayiin-0.3.7/pyAyiin/pyrogram/tools.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.6/pyAyiin/telethon/ayiin/_wrappers.py` & `py-Ayiin-0.3.7/pyAyiin/telethon/ayiin/_wrappers.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.6/pyAyiin/telethon/ayiin/events.py` & `py-Ayiin-0.3.7/pyAyiin/telethon/ayiin/events.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.6/pyAyiin/telethon/ayiin/misc.py` & `py-Ayiin-0.3.7/pyAyiin/telethon/ayiin/misc.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.6/pyAyiin/xd.py` & `py-Ayiin-0.3.7/pyAyiin/xd.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.6/py_Ayiin.egg-info/PKG-INFO` & `py-Ayiin-0.3.7/py_Ayiin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-Ayiin
-Version: 0.3.6
+Version: 0.3.7
 Summary: A Secure and Powerful Python-Telethon Based and Python-Pyrogram Based Library For Your Userbot Module.
 Home-page: https://github.com/AyiinXd/AyiinXd
 Author: AyiinXd
 Author-email: ayingaming98@gmail.com
 License: GNU General Public License v3.0 (GPL-3.0)
 Project-URL: Bug Tracker, https://github.com/AyiinXd/AyiinXd/issues
 Project-URL: Source Code, https://github.com/AyiinXd/AyiinXd
```

### Comparing `py-Ayiin-0.3.6/py_Ayiin.egg-info/SOURCES.txt` & `py-Ayiin-0.3.7/py_Ayiin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.6/setup.py` & `py-Ayiin-0.3.7/setup.py`

 * *Files identical despite different names*

