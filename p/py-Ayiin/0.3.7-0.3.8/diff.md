# Comparing `tmp/py-Ayiin-0.3.7.tar.gz` & `tmp/py-Ayiin-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-Ayiin-0.3.7.tar", last modified: Thu May 25 01:36:01 2023, max compression
+gzip compressed data, was "py-Ayiin-0.3.8.tar", last modified: Thu May 25 05:52:43 2023, max compression
```

## Comparing `py-Ayiin-0.3.7.tar` & `py-Ayiin-0.3.8.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 01:36:01.969534 py-Ayiin-0.3.7/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-05-25 01:36:01.969534 py-Ayiin-0.3.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 01:36:01.961534 py-Ayiin-0.3.7/pyAyiin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 01:36:01.961534 py-Ayiin-0.3.7/pyAyiin/Clients/
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/pyAyiin/Clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12568 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/pyAyiin/Clients/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6130 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/pyAyiin/Clients/pytgcalls.py
--rw-r--r--   0 runner    (1001) docker     (123)    38642 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/pyAyiin/Clients/startup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/pyAyiin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/pyAyiin/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/pyAyiin/assistant.py
--rw-r--r--   0 runner    (1001) docker     (123)     5126 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/pyAyiin/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 01:36:01.965534 py-Ayiin-0.3.7/pyAyiin/dB/
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/pyAyiin/dB/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/pyAyiin/dB/_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/pyAyiin/dB/absen.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/pyAyiin/dB/admins.py
--rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/pyAyiin/dB/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/pyAyiin/dB/blacklistfilter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/pyAyiin/dB/blacklistgcast.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/pyAyiin/dB/blacklistuser.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/pyAyiin/dB/gban.py
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/pyAyiin/dB/langs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/pyAyiin/dB/logdb.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/pyAyiin/dB/pmpermit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/pyAyiin/dB/premium.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/pyAyiin/dB/start.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/pyAyiin/dB/sudo.py
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/pyAyiin/dB/variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/pyAyiin/dB/videocalls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/pyAyiin/dB/welcome.py
--rw-r--r--   0 runner    (1001) docker     (123)    33254 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/pyAyiin/decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/pyAyiin/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 01:36:01.965534 py-Ayiin-0.3.7/pyAyiin/methods/
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/pyAyiin/methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/pyAyiin/methods/_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/pyAyiin/methods/changer.py
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/pyAyiin/methods/converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6903 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/pyAyiin/methods/func.py
--rw-r--r--   0 runner    (1001) docker     (123)     6181 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/pyAyiin/methods/funcb.py
--rw-r--r--   0 runner    (1001) docker     (123)     8828 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/pyAyiin/methods/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/pyAyiin/methods/hosting.py
--rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/pyAyiin/methods/inlinebot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/pyAyiin/methods/queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     5968 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/pyAyiin/methods/thumbnail.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 01:36:01.969534 py-Ayiin-0.3.7/pyAyiin/pyrogram/
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/pyAyiin/pyrogram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/pyAyiin/pyrogram/_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)    13157 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/pyAyiin/pyrogram/func.py
--rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/pyAyiin/pyrogram/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/pyAyiin/pyrogram/pastebin.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/pyAyiin/pyrogram/sections.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/pyAyiin/pyrogram/toolbot.py
--rw-r--r--   0 runner    (1001) docker     (123)     8684 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/pyAyiin/pyrogram/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 01:36:01.969534 py-Ayiin-0.3.7/pyAyiin/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/pyAyiin/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 01:36:01.969534 py-Ayiin-0.3.7/pyAyiin/telethon/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/pyAyiin/telethon/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 01:36:01.969534 py-Ayiin-0.3.7/pyAyiin/telethon/ayiin/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/pyAyiin/telethon/ayiin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/pyAyiin/telethon/ayiin/_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/pyAyiin/telethon/ayiin/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/pyAyiin/telethon/ayiin/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    17263 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/pyAyiin/xd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 01:36:01.969534 py-Ayiin-0.3.7/py_Ayiin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-05-25 01:36:01.000000 py-Ayiin-0.3.7/py_Ayiin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-05-25 01:36:01.000000 py-Ayiin-0.3.7/py_Ayiin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 01:36:01.000000 py-Ayiin-0.3.7/py_Ayiin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-25 01:36:01.000000 py-Ayiin-0.3.7/py_Ayiin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-25 01:36:01.000000 py-Ayiin-0.3.7/py_Ayiin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 01:36:01.969534 py-Ayiin-0.3.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-25 01:35:50.000000 py-Ayiin-0.3.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 05:52:43.413308 py-Ayiin-0.3.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-05-25 05:52:43.413308 py-Ayiin-0.3.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 05:52:43.405308 py-Ayiin-0.3.8/pyAyiin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 05:52:43.409308 py-Ayiin-0.3.8/pyAyiin/Clients/
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/pyAyiin/Clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12528 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/pyAyiin/Clients/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/pyAyiin/Clients/pytgcalls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38642 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/pyAyiin/Clients/startup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/pyAyiin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/pyAyiin/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6216 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/pyAyiin/assistant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5126 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/pyAyiin/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 05:52:43.409308 py-Ayiin-0.3.8/pyAyiin/dB/
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/pyAyiin/dB/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/pyAyiin/dB/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/pyAyiin/dB/absen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/pyAyiin/dB/admins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/pyAyiin/dB/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/pyAyiin/dB/blacklistfilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/pyAyiin/dB/blacklistgcast.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/pyAyiin/dB/blacklistuser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/pyAyiin/dB/gban.py
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/pyAyiin/dB/langs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/pyAyiin/dB/logdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/pyAyiin/dB/pmpermit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/pyAyiin/dB/premium.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/pyAyiin/dB/start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/pyAyiin/dB/sudo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/pyAyiin/dB/variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/pyAyiin/dB/videocalls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/pyAyiin/dB/welcome.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33262 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/pyAyiin/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/pyAyiin/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 05:52:43.409308 py-Ayiin-0.3.8/pyAyiin/methods/
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/pyAyiin/methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/pyAyiin/methods/_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/pyAyiin/methods/changer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/pyAyiin/methods/converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6903 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/pyAyiin/methods/func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6185 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/pyAyiin/methods/funcb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8830 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/pyAyiin/methods/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/pyAyiin/methods/hosting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/pyAyiin/methods/inlinebot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/pyAyiin/methods/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5968 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/pyAyiin/methods/thumbnail.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 05:52:43.409308 py-Ayiin-0.3.8/pyAyiin/pyrogram/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/pyAyiin/pyrogram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/pyAyiin/pyrogram/_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13161 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/pyAyiin/pyrogram/func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/pyAyiin/pyrogram/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/pyAyiin/pyrogram/pastebin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/pyAyiin/pyrogram/sections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/pyAyiin/pyrogram/toolbot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8688 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/pyAyiin/pyrogram/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 05:52:43.409308 py-Ayiin-0.3.8/pyAyiin/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/pyAyiin/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 05:52:43.409308 py-Ayiin-0.3.8/pyAyiin/telethon/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/pyAyiin/telethon/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 05:52:43.413308 py-Ayiin-0.3.8/pyAyiin/telethon/ayiin/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/pyAyiin/telethon/ayiin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/pyAyiin/telethon/ayiin/_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/pyAyiin/telethon/ayiin/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/pyAyiin/telethon/ayiin/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17269 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/pyAyiin/xd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 05:52:43.413308 py-Ayiin-0.3.8/py_Ayiin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-05-25 05:52:43.000000 py-Ayiin-0.3.8/py_Ayiin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-05-25 05:52:43.000000 py-Ayiin-0.3.8/py_Ayiin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 05:52:43.000000 py-Ayiin-0.3.8/py_Ayiin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-25 05:52:43.000000 py-Ayiin-0.3.8/py_Ayiin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-25 05:52:43.000000 py-Ayiin-0.3.8/py_Ayiin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 05:52:43.413308 py-Ayiin-0.3.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/setup.py
```

### Comparing `py-Ayiin-0.3.7/LICENSE` & `py-Ayiin-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.7/NOTICE` & `py-Ayiin-0.3.8/NOTICE`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.7/PKG-INFO` & `py-Ayiin-0.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-Ayiin
-Version: 0.3.7
+Version: 0.3.8
 Summary: A Secure and Powerful Python-Telethon Based and Python-Pyrogram Based Library For Your Userbot Module.
 Home-page: https://github.com/AyiinXd/AyiinXd
 Author: AyiinXd
 Author-email: ayingaming98@gmail.com
 License: GNU General Public License v3.0 (GPL-3.0)
 Project-URL: Bug Tracker, https://github.com/AyiinXd/AyiinXd/issues
 Project-URL: Source Code, https://github.com/AyiinXd/AyiinXd
```

### Comparing `py-Ayiin-0.3.7/README.md` & `py-Ayiin-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.7/pyAyiin/Clients/__init__.py` & `py-Ayiin-0.3.8/pyAyiin/Clients/__init__.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.7/pyAyiin/Clients/client.py` & `py-Ayiin-0.3.8/pyAyiin/Clients/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import logging
 
-from pyrogram import Client as PyroClient
-from fipper import Client
+from pyrogram import Client
 
 from telethon import TelegramClient
 from telethon.sessions import MemorySession
 
 from . import *
 
 from ..config import Var as Variable
```

### Comparing `py-Ayiin-0.3.7/pyAyiin/Clients/pytgcalls.py` & `py-Ayiin-0.3.8/pyAyiin/Clients/pytgcalls.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,19 +16,19 @@
 
 import asyncio
 import os
 import yt_dlp
 
 from typing import Optional, Union
 
-from fipper.types import Message
-from fipper.raw.functions.channels import GetFullChannel
-from fipper.raw.functions.messages import GetFullChat
-from fipper.raw.functions.phone import CreateGroupCall, DiscardGroupCall, EditGroupCallTitle
-from fipper.raw.types import InputGroupCall, InputPeerChannel, InputPeerChat
+from pyrogram.types import Message
+from pyrogram.raw.functions.channels import GetFullChannel
+from pyrogram.raw.functions.messages import GetFullChat
+from pyrogram.raw.functions.phone import CreateGroupCall, DiscardGroupCall, EditGroupCallTitle
+from pyrogram.raw.types import InputGroupCall, InputPeerChannel, InputPeerChat
 
 from pytgcalls.exceptions import GroupCallNotFoundError
 
 from ..methods.queue import Queues, QUEUE
 
 from .client import *
```

### Comparing `py-Ayiin-0.3.7/pyAyiin/Clients/startup.py` & `py-Ayiin-0.3.8/pyAyiin/Clients/startup.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.7/pyAyiin/__init__.py` & `py-Ayiin-0.3.8/pyAyiin/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
 
 logs = logging.getLogger(__name__)
 
 
 __copyright__ = "Copyright (C) 2022-present AyiinXd <https://github.com/AyiinXd>"
 __license__ = "GNU General Public License v3.0 (GPL-3.0)"
-__version__ = "0.3.7"
+__version__ = "0.3.8"
 ayiin_ver = "0.1.1"
 
 
 DEVS = [
     607067484, # Ayiin
     997461844, #Ayang_Ayiin
     2130526178, # Alfa
```

### Comparing `py-Ayiin-0.3.7/pyAyiin/__main__.py` & `py-Ayiin-0.3.8/pyAyiin/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import asyncio
 import importlib
 import sys
 
-from fipper import idle
+from pyrogram import idle
 
 from pyAyiin import __version__
 
 from . import *
 
 from .config import Var
 from .Clients.client import Bots
```

### Comparing `py-Ayiin-0.3.7/pyAyiin/assistant.py` & `py-Ayiin-0.3.8/pyAyiin/assistant.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import logging
 from datetime import datetime
 from traceback import format_exc
 import pytz
-from fipper import filters
-from fipper.errors.exceptions.bad_request_400 import (
+from pyrogram import filters
+from pyrogram.errors.exceptions.bad_request_400 import (
     MessageIdInvalid,
     MessageNotModified,
     UserNotParticipant
 )
-from fipper.types import (
+from pyrogram.types import (
     InlineKeyboardButton,
     InlineKeyboardMarkup,
     InlineQueryResultArticle,
     InputTextMessageContent
 )
 
-from fipper.handlers import CallbackQueryHandler, InlineQueryHandler
+from pyrogram.handlers import CallbackQueryHandler, InlineQueryHandler
 
 from .config import Var as Variable
 from .decorator import is_admin_or_owner
 from .Clients import *
 
 
 Var = Variable()
```

### Comparing `py-Ayiin-0.3.7/pyAyiin/config.py` & `py-Ayiin-0.3.8/pyAyiin/config.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.7/pyAyiin/dB/__init__.py` & `py-Ayiin-0.3.8/pyAyiin/dB/__init__.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.7/pyAyiin/dB/absen.py` & `py-Ayiin-0.3.8/pyAyiin/dB/absen.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.7/pyAyiin/dB/admins.py` & `py-Ayiin-0.3.8/pyAyiin/dB/admins.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.7/pyAyiin/dB/auth.py` & `py-Ayiin-0.3.8/pyAyiin/dB/auth.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.7/pyAyiin/dB/blacklistfilter.py` & `py-Ayiin-0.3.8/pyAyiin/dB/blacklistfilter.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.7/pyAyiin/dB/blacklistgcast.py` & `py-Ayiin-0.3.8/pyAyiin/dB/blacklistgcast.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.7/pyAyiin/dB/blacklistuser.py` & `py-Ayiin-0.3.8/pyAyiin/dB/blacklistuser.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.7/pyAyiin/dB/gban.py` & `py-Ayiin-0.3.8/pyAyiin/dB/gban.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.7/pyAyiin/dB/langs.py` & `py-Ayiin-0.3.8/pyAyiin/dB/langs.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.7/pyAyiin/dB/logdb.py` & `py-Ayiin-0.3.8/pyAyiin/dB/logdb.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.7/pyAyiin/dB/pmpermit.py` & `py-Ayiin-0.3.8/pyAyiin/dB/pmpermit.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.7/pyAyiin/dB/premium.py` & `py-Ayiin-0.3.8/pyAyiin/dB/premium.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.7/pyAyiin/dB/start.py` & `py-Ayiin-0.3.8/pyAyiin/dB/start.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.7/pyAyiin/dB/sudo.py` & `py-Ayiin-0.3.8/pyAyiin/dB/sudo.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.7/pyAyiin/dB/variable.py` & `py-Ayiin-0.3.8/pyAyiin/dB/variable.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.7/pyAyiin/dB/videocalls.py` & `py-Ayiin-0.3.8/pyAyiin/dB/videocalls.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.7/pyAyiin/dB/welcome.py` & `py-Ayiin-0.3.8/pyAyiin/dB/welcome.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.7/pyAyiin/decorator.py` & `py-Ayiin-0.3.8/pyAyiin/decorator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import logging
 from datetime import datetime
 from traceback import format_exc
 import pytz
-from fipper import ContinuePropagation, StopPropagation, filters
-from fipper.enums import ChatMemberStatus, ChatType
-from fipper.errors.exceptions.bad_request_400 import (
+from pyrogram import ContinuePropagation, StopPropagation, filters
+from pyrogram.enums import ChatMemberStatus, ChatType
+from pyrogram.errors.exceptions.bad_request_400 import (
     MessageIdInvalid,
     MessageNotModified,
     MessageEmpty,
     UserNotParticipant
 )
-from fipper.handlers import MessageHandler
+from pyrogram.handlers import MessageHandler
 
 from pyAyiin.pyrogram import eor
 
 from . import DEVS
 from .config import Var as Variable
 from .Clients import *
```

### Comparing `py-Ayiin-0.3.7/pyAyiin/exceptions.py` & `py-Ayiin-0.3.8/pyAyiin/exceptions.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.7/pyAyiin/methods/__init__.py` & `py-Ayiin-0.3.8/pyAyiin/methods/__init__.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.7/pyAyiin/methods/_misc.py` & `py-Ayiin-0.3.8/pyAyiin/methods/_misc.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 # ========================×========================
 
 import heroku3
 
 from time import time
 from datetime import datetime
 
-from fipper import __version__ as fip_ver, Client
-from fipper.enums import ParseMode
-from fipper.types import (
+from pyrogram import __version__ as fip_ver, Client
+from pyrogram.enums import ParseMode
+from pyrogram.types import (
     InlineKeyboardButton,
     InlineKeyboardMarkup,
     InlineQueryResultArticle,
     InlineQueryResultPhoto,
     InputTextMessageContent,
 )
 from platform import python_version
```

### Comparing `py-Ayiin-0.3.7/pyAyiin/methods/changer.py` & `py-Ayiin-0.3.8/pyAyiin/methods/changer.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.7/pyAyiin/methods/converter.py` & `py-Ayiin-0.3.8/pyAyiin/methods/converter.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.7/pyAyiin/methods/func.py` & `py-Ayiin-0.3.8/pyAyiin/methods/func.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.7/pyAyiin/methods/funcb.py` & `py-Ayiin-0.3.8/pyAyiin/methods/funcb.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 # ========================×========================
 #            Jangan Hapus Credit Ngentod
 # ========================×========================
 
 import asyncio
 import os
 
-from fipper.errors import FloodWait
-from fipper.types import (
+from pyrogram.errors import FloodWait
+from pyrogram.types import (
     CallbackQuery,
     InlineKeyboardButton,
     InlineKeyboardMarkup, 
     Message,
 )
```

### Comparing `py-Ayiin-0.3.7/pyAyiin/methods/helpers.py` & `py-Ayiin-0.3.8/pyAyiin/methods/helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 import importlib
 import os
 import ssl
 import sys
 from concurrent.futures import ThreadPoolExecutor
 from functools import partial, wraps
 
-from fipper import Client
+from pyrogram import Client
 from ..pyrogram import eor, section
 from ..Clients import *
 
 
 try:
     import certifi
 except ImportError:
```

### Comparing `py-Ayiin-0.3.7/pyAyiin/methods/hosting.py` & `py-Ayiin-0.3.8/pyAyiin/methods/hosting.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.7/pyAyiin/methods/inlinebot.py` & `py-Ayiin-0.3.8/pyAyiin/methods/inlinebot.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 # t.me/AyiinChat & t.me/AyiinSupport
 
 
 # ========================×========================
 #            Jangan Hapus Credit Ngentod
 # ========================×========================
 
-from fipper.enums import ParseMode
-from fipper.types import (
+from pyrogram.enums import ParseMode
+from pyrogram.types import (
     InlineKeyboardButton,
     InlineKeyboardMarkup,
     InlineQueryResultArticle,
     InlineQueryResultPhoto,
     InputTextMessageContent,
 )
```

### Comparing `py-Ayiin-0.3.7/pyAyiin/methods/queue.py` & `py-Ayiin-0.3.8/pyAyiin/methods/queue.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.7/pyAyiin/methods/thumbnail.py` & `py-Ayiin-0.3.8/pyAyiin/methods/thumbnail.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.7/pyAyiin/pyrogram/__init__.py` & `py-Ayiin-0.3.8/pyAyiin/pyrogram/__init__.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.7/pyAyiin/pyrogram/_wrappers.py` & `py-Ayiin-0.3.8/pyAyiin/pyrogram/_wrappers.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 
 from asyncio import sleep
 
-from fipper.enums import MessageServiceType
-from fipper.errors import MessageDeleteForbidden, MessageNotModified
-from fipper.types import Message
+from pyrogram.enums import MessageServiceType
+from pyrogram.errors import MessageDeleteForbidden, MessageNotModified
+from pyrogram.types import Message
 
 
 LOGS = logging.getLogger(__name__)
 
 """
 servis = (
     MessageServiceType.NEW_CHAT_MEMBERS,
```

### Comparing `py-Ayiin-0.3.7/pyAyiin/pyrogram/func.py` & `py-Ayiin-0.3.8/pyAyiin/pyrogram/func.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,16 +22,16 @@
 import shlex
 import textwrap
 from aiohttp import ContentTypeError
 from typing import Tuple, Union
 from io import BytesIO
 
 from pymediainfo import MediaInfo
-from fipper import Client, enums, raw
-from fipper.types import Message, User
+from pyrogram import Client, enums, raw
+from pyrogram.types import Message, User
 from PIL import Image, ImageDraw, ImageFont
 
 
 _entitie = {
     raw.types.MessageEntityPhone: "phone_number",
     raw.types.MessageEntityMention: "mention",
     raw.types.MessageEntityBold: "bold",
```

### Comparing `py-Ayiin-0.3.7/pyAyiin/pyrogram/misc.py` & `py-Ayiin-0.3.8/pyAyiin/pyrogram/misc.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # t.me/SharingUserbot & t.me/Lunatic0de
 
 import os
 import sys
 from re import sub
 from time import time
 
-from fipper import Client, enums
+from pyrogram import Client, enums
 
 admins_in_chat = {}
 
 
 class Misc(object):
     async def list_admins(self, client: Client, chat_id: int):
         global admins_in_chat
```

### Comparing `py-Ayiin-0.3.7/pyAyiin/pyrogram/pastebin.py` & `py-Ayiin-0.3.8/pyAyiin/pyrogram/pastebin.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.7/pyAyiin/pyrogram/sections.py` & `py-Ayiin-0.3.8/pyAyiin/pyrogram/sections.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.7/pyAyiin/pyrogram/toolbot.py` & `py-Ayiin-0.3.8/pyAyiin/pyrogram/toolbot.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import math
 
-from fipper.types import (
+from pyrogram.types import (
     InlineKeyboardButton
 )
 
 
 class ToolBot(object):
     def HelpXd(
         self,
```

### Comparing `py-Ayiin-0.3.7/pyAyiin/pyrogram/tools.py` & `py-Ayiin-0.3.8/pyAyiin/pyrogram/tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,16 +19,16 @@
 import os
 import shlex
 import textwrap
 from typing import Tuple, Union
 from io import BytesIO
 
 from pymediainfo import MediaInfo
-from fipper import Client, enums
-from fipper.types import Message, User
+from pyrogram import Client, enums
+from pyrogram.types import Message, User
 from PIL import Image, ImageDraw, ImageFont
 
 
 class Tools(object):
     async def CheckAdmin(
         self,
         client: Client,
```

### Comparing `py-Ayiin-0.3.7/pyAyiin/telethon/ayiin/_wrappers.py` & `py-Ayiin-0.3.8/pyAyiin/telethon/ayiin/_wrappers.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.7/pyAyiin/telethon/ayiin/events.py` & `py-Ayiin-0.3.8/pyAyiin/telethon/ayiin/events.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.7/pyAyiin/telethon/ayiin/misc.py` & `py-Ayiin-0.3.8/pyAyiin/telethon/ayiin/misc.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.7/pyAyiin/xd.py` & `py-Ayiin-0.3.8/pyAyiin/xd.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import asyncio
 import logging
 
 from asyncio.exceptions import TimeoutError
-from fipper import Client as ClientFipper, filters
-from fipper.types import InlineKeyboardMarkup, InlineKeyboardButton, Message
-from fipper.errors import (
+from pyrogram import Client as ClientFipper, filters
+from pyrogram.types import InlineKeyboardMarkup, InlineKeyboardButton, Message
+from pyrogram.errors import (
     ApiIdInvalid as ApiIdInvalidFipper,
     PhoneNumberInvalid as PhoneNumberInvalidFipper,
     PhoneCodeInvalid as PhoneCodeInvalidFipper,
     PhoneCodeExpired as PhoneCodeExpiredFipper,
     SessionPasswordNeeded as SessionPasswordNeededFipper,
     PasswordHashInvalid as PasswordHashInvalidFipper
 )
```

### Comparing `py-Ayiin-0.3.7/py_Ayiin.egg-info/PKG-INFO` & `py-Ayiin-0.3.8/py_Ayiin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-Ayiin
-Version: 0.3.7
+Version: 0.3.8
 Summary: A Secure and Powerful Python-Telethon Based and Python-Pyrogram Based Library For Your Userbot Module.
 Home-page: https://github.com/AyiinXd/AyiinXd
 Author: AyiinXd
 Author-email: ayingaming98@gmail.com
 License: GNU General Public License v3.0 (GPL-3.0)
 Project-URL: Bug Tracker, https://github.com/AyiinXd/AyiinXd/issues
 Project-URL: Source Code, https://github.com/AyiinXd/AyiinXd
```

### Comparing `py-Ayiin-0.3.7/py_Ayiin.egg-info/SOURCES.txt` & `py-Ayiin-0.3.8/py_Ayiin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.7/setup.py` & `py-Ayiin-0.3.8/setup.py`

 * *Files identical despite different names*

