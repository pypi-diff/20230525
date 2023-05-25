# Comparing `tmp/py-Ayiin-0.3.8.tar.gz` & `tmp/py-Ayiin-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-Ayiin-0.3.8.tar", last modified: Thu May 25 05:52:43 2023, max compression
+gzip compressed data, was "py-Ayiin-0.3.9.tar", last modified: Thu May 25 07:00:41 2023, max compression
```

## Comparing `py-Ayiin-0.3.8.tar` & `py-Ayiin-0.3.9.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 05:52:43.413308 py-Ayiin-0.3.8/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-05-25 05:52:43.413308 py-Ayiin-0.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 05:52:43.405308 py-Ayiin-0.3.8/pyAyiin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 05:52:43.409308 py-Ayiin-0.3.8/pyAyiin/Clients/
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/pyAyiin/Clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12528 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/pyAyiin/Clients/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/pyAyiin/Clients/pytgcalls.py
--rw-r--r--   0 runner    (1001) docker     (123)    38642 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/pyAyiin/Clients/startup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/pyAyiin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/pyAyiin/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6216 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/pyAyiin/assistant.py
--rw-r--r--   0 runner    (1001) docker     (123)     5126 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/pyAyiin/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 05:52:43.409308 py-Ayiin-0.3.8/pyAyiin/dB/
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/pyAyiin/dB/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/pyAyiin/dB/_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/pyAyiin/dB/absen.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/pyAyiin/dB/admins.py
--rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/pyAyiin/dB/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/pyAyiin/dB/blacklistfilter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/pyAyiin/dB/blacklistgcast.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/pyAyiin/dB/blacklistuser.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/pyAyiin/dB/gban.py
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/pyAyiin/dB/langs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/pyAyiin/dB/logdb.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/pyAyiin/dB/pmpermit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/pyAyiin/dB/premium.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/pyAyiin/dB/start.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/pyAyiin/dB/sudo.py
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/pyAyiin/dB/variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/pyAyiin/dB/videocalls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/pyAyiin/dB/welcome.py
--rw-r--r--   0 runner    (1001) docker     (123)    33262 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/pyAyiin/decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/pyAyiin/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 05:52:43.409308 py-Ayiin-0.3.8/pyAyiin/methods/
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/pyAyiin/methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/pyAyiin/methods/_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/pyAyiin/methods/changer.py
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/pyAyiin/methods/converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6903 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/pyAyiin/methods/func.py
--rw-r--r--   0 runner    (1001) docker     (123)     6185 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/pyAyiin/methods/funcb.py
--rw-r--r--   0 runner    (1001) docker     (123)     8830 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/pyAyiin/methods/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/pyAyiin/methods/hosting.py
--rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/pyAyiin/methods/inlinebot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/pyAyiin/methods/queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     5968 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/pyAyiin/methods/thumbnail.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 05:52:43.409308 py-Ayiin-0.3.8/pyAyiin/pyrogram/
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/pyAyiin/pyrogram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/pyAyiin/pyrogram/_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)    13161 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/pyAyiin/pyrogram/func.py
--rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/pyAyiin/pyrogram/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/pyAyiin/pyrogram/pastebin.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/pyAyiin/pyrogram/sections.py
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/pyAyiin/pyrogram/toolbot.py
--rw-r--r--   0 runner    (1001) docker     (123)     8688 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/pyAyiin/pyrogram/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 05:52:43.409308 py-Ayiin-0.3.8/pyAyiin/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/pyAyiin/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 05:52:43.409308 py-Ayiin-0.3.8/pyAyiin/telethon/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/pyAyiin/telethon/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 05:52:43.413308 py-Ayiin-0.3.8/pyAyiin/telethon/ayiin/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/pyAyiin/telethon/ayiin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/pyAyiin/telethon/ayiin/_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/pyAyiin/telethon/ayiin/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/pyAyiin/telethon/ayiin/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    17269 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/pyAyiin/xd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 05:52:43.413308 py-Ayiin-0.3.8/py_Ayiin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-05-25 05:52:43.000000 py-Ayiin-0.3.8/py_Ayiin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-05-25 05:52:43.000000 py-Ayiin-0.3.8/py_Ayiin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 05:52:43.000000 py-Ayiin-0.3.8/py_Ayiin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-25 05:52:43.000000 py-Ayiin-0.3.8/py_Ayiin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-25 05:52:43.000000 py-Ayiin-0.3.8/py_Ayiin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 05:52:43.413308 py-Ayiin-0.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-25 05:52:34.000000 py-Ayiin-0.3.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:00:41.387870 py-Ayiin-0.3.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-25 07:00:28.000000 py-Ayiin-0.3.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-25 07:00:28.000000 py-Ayiin-0.3.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-25 07:00:28.000000 py-Ayiin-0.3.9/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-05-25 07:00:41.387870 py-Ayiin-0.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-05-25 07:00:28.000000 py-Ayiin-0.3.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:00:41.383870 py-Ayiin-0.3.9/pyAyiin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:00:41.383870 py-Ayiin-0.3.9/pyAyiin/Clients/
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-25 07:00:28.000000 py-Ayiin-0.3.9/pyAyiin/Clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12528 2023-05-25 07:00:28.000000 py-Ayiin-0.3.9/pyAyiin/Clients/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-05-25 07:00:28.000000 py-Ayiin-0.3.9/pyAyiin/Clients/pytgcalls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38642 2023-05-25 07:00:28.000000 py-Ayiin-0.3.9/pyAyiin/Clients/startup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-05-25 07:00:28.000000 py-Ayiin-0.3.9/pyAyiin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-05-25 07:00:28.000000 py-Ayiin-0.3.9/pyAyiin/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6216 2023-05-25 07:00:28.000000 py-Ayiin-0.3.9/pyAyiin/assistant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5126 2023-05-25 07:00:28.000000 py-Ayiin-0.3.9/pyAyiin/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:00:41.383870 py-Ayiin-0.3.9/pyAyiin/dB/
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-05-25 07:00:28.000000 py-Ayiin-0.3.9/pyAyiin/dB/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-25 07:00:28.000000 py-Ayiin-0.3.9/pyAyiin/dB/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-05-25 07:00:28.000000 py-Ayiin-0.3.9/pyAyiin/dB/absen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-25 07:00:28.000000 py-Ayiin-0.3.9/pyAyiin/dB/admins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-05-25 07:00:28.000000 py-Ayiin-0.3.9/pyAyiin/dB/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-05-25 07:00:28.000000 py-Ayiin-0.3.9/pyAyiin/dB/blacklistfilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-25 07:00:28.000000 py-Ayiin-0.3.9/pyAyiin/dB/blacklistgcast.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-25 07:00:28.000000 py-Ayiin-0.3.9/pyAyiin/dB/blacklistuser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-25 07:00:28.000000 py-Ayiin-0.3.9/pyAyiin/dB/gban.py
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-05-25 07:00:28.000000 py-Ayiin-0.3.9/pyAyiin/dB/langs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-25 07:00:28.000000 py-Ayiin-0.3.9/pyAyiin/dB/logdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-25 07:00:28.000000 py-Ayiin-0.3.9/pyAyiin/dB/pmpermit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-05-25 07:00:28.000000 py-Ayiin-0.3.9/pyAyiin/dB/premium.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-25 07:00:28.000000 py-Ayiin-0.3.9/pyAyiin/dB/start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-25 07:00:28.000000 py-Ayiin-0.3.9/pyAyiin/dB/sudo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-25 07:00:28.000000 py-Ayiin-0.3.9/pyAyiin/dB/variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-05-25 07:00:28.000000 py-Ayiin-0.3.9/pyAyiin/dB/videocalls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-05-25 07:00:28.000000 py-Ayiin-0.3.9/pyAyiin/dB/welcome.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33262 2023-05-25 07:00:28.000000 py-Ayiin-0.3.9/pyAyiin/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-25 07:00:28.000000 py-Ayiin-0.3.9/pyAyiin/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:00:41.387870 py-Ayiin-0.3.9/pyAyiin/methods/
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-25 07:00:28.000000 py-Ayiin-0.3.9/pyAyiin/methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-05-25 07:00:28.000000 py-Ayiin-0.3.9/pyAyiin/methods/_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-05-25 07:00:28.000000 py-Ayiin-0.3.9/pyAyiin/methods/changer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-25 07:00:28.000000 py-Ayiin-0.3.9/pyAyiin/methods/converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6909 2023-05-25 07:00:28.000000 py-Ayiin-0.3.9/pyAyiin/methods/func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6185 2023-05-25 07:00:28.000000 py-Ayiin-0.3.9/pyAyiin/methods/funcb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8830 2023-05-25 07:00:28.000000 py-Ayiin-0.3.9/pyAyiin/methods/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-05-25 07:00:28.000000 py-Ayiin-0.3.9/pyAyiin/methods/hosting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-05-25 07:00:28.000000 py-Ayiin-0.3.9/pyAyiin/methods/inlinebot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-05-25 07:00:28.000000 py-Ayiin-0.3.9/pyAyiin/methods/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5968 2023-05-25 07:00:28.000000 py-Ayiin-0.3.9/pyAyiin/methods/thumbnail.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:00:41.387870 py-Ayiin-0.3.9/pyAyiin/pyrogram/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-25 07:00:28.000000 py-Ayiin-0.3.9/pyAyiin/pyrogram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-05-25 07:00:28.000000 py-Ayiin-0.3.9/pyAyiin/pyrogram/_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13161 2023-05-25 07:00:28.000000 py-Ayiin-0.3.9/pyAyiin/pyrogram/func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-05-25 07:00:28.000000 py-Ayiin-0.3.9/pyAyiin/pyrogram/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-05-25 07:00:28.000000 py-Ayiin-0.3.9/pyAyiin/pyrogram/pastebin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-25 07:00:28.000000 py-Ayiin-0.3.9/pyAyiin/pyrogram/sections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-05-25 07:00:28.000000 py-Ayiin-0.3.9/pyAyiin/pyrogram/toolbot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8688 2023-05-25 07:00:28.000000 py-Ayiin-0.3.9/pyAyiin/pyrogram/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:00:41.387870 py-Ayiin-0.3.9/pyAyiin/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:00:28.000000 py-Ayiin-0.3.9/pyAyiin/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:00:41.387870 py-Ayiin-0.3.9/pyAyiin/telethon/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-25 07:00:28.000000 py-Ayiin-0.3.9/pyAyiin/telethon/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:00:41.387870 py-Ayiin-0.3.9/pyAyiin/telethon/ayiin/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-25 07:00:28.000000 py-Ayiin-0.3.9/pyAyiin/telethon/ayiin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-05-25 07:00:28.000000 py-Ayiin-0.3.9/pyAyiin/telethon/ayiin/_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-05-25 07:00:28.000000 py-Ayiin-0.3.9/pyAyiin/telethon/ayiin/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-05-25 07:00:28.000000 py-Ayiin-0.3.9/pyAyiin/telethon/ayiin/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17269 2023-05-25 07:00:28.000000 py-Ayiin-0.3.9/pyAyiin/xd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:00:41.387870 py-Ayiin-0.3.9/py_Ayiin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-05-25 07:00:41.000000 py-Ayiin-0.3.9/py_Ayiin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-05-25 07:00:41.000000 py-Ayiin-0.3.9/py_Ayiin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 07:00:41.000000 py-Ayiin-0.3.9/py_Ayiin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-25 07:00:41.000000 py-Ayiin-0.3.9/py_Ayiin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-25 07:00:41.000000 py-Ayiin-0.3.9/py_Ayiin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-25 07:00:28.000000 py-Ayiin-0.3.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 07:00:41.387870 py-Ayiin-0.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-25 07:00:28.000000 py-Ayiin-0.3.9/setup.py
```

### Comparing `py-Ayiin-0.3.8/LICENSE` & `py-Ayiin-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.8/NOTICE` & `py-Ayiin-0.3.9/NOTICE`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.8/PKG-INFO` & `py-Ayiin-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-Ayiin
-Version: 0.3.8
+Version: 0.3.9
 Summary: A Secure and Powerful Python-Telethon Based and Python-Pyrogram Based Library For Your Userbot Module.
 Home-page: https://github.com/AyiinXd/AyiinXd
 Author: AyiinXd
 Author-email: ayingaming98@gmail.com
 License: GNU General Public License v3.0 (GPL-3.0)
 Project-URL: Bug Tracker, https://github.com/AyiinXd/AyiinXd/issues
 Project-URL: Source Code, https://github.com/AyiinXd/AyiinXd
```

### Comparing `py-Ayiin-0.3.8/README.md` & `py-Ayiin-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.8/pyAyiin/Clients/__init__.py` & `py-Ayiin-0.3.9/pyAyiin/Clients/__init__.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.8/pyAyiin/Clients/client.py` & `py-Ayiin-0.3.9/pyAyiin/Clients/client.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.8/pyAyiin/Clients/pytgcalls.py` & `py-Ayiin-0.3.9/pyAyiin/Clients/pytgcalls.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.8/pyAyiin/Clients/startup.py` & `py-Ayiin-0.3.9/pyAyiin/Clients/startup.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.8/pyAyiin/__init__.py` & `py-Ayiin-0.3.9/pyAyiin/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
 
 logs = logging.getLogger(__name__)
 
 
 __copyright__ = "Copyright (C) 2022-present AyiinXd <https://github.com/AyiinXd>"
 __license__ = "GNU General Public License v3.0 (GPL-3.0)"
-__version__ = "0.3.8"
+__version__ = "0.3.9"
 ayiin_ver = "0.1.1"
 
 
 DEVS = [
     607067484, # Ayiin
     997461844, #Ayang_Ayiin
     2130526178, # Alfa
```

### Comparing `py-Ayiin-0.3.8/pyAyiin/__main__.py` & `py-Ayiin-0.3.9/pyAyiin/__main__.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.8/pyAyiin/assistant.py` & `py-Ayiin-0.3.9/pyAyiin/assistant.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.8/pyAyiin/config.py` & `py-Ayiin-0.3.9/pyAyiin/config.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.8/pyAyiin/dB/__init__.py` & `py-Ayiin-0.3.9/pyAyiin/dB/__init__.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.8/pyAyiin/dB/absen.py` & `py-Ayiin-0.3.9/pyAyiin/dB/absen.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.8/pyAyiin/dB/admins.py` & `py-Ayiin-0.3.9/pyAyiin/dB/admins.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.8/pyAyiin/dB/auth.py` & `py-Ayiin-0.3.9/pyAyiin/dB/auth.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.8/pyAyiin/dB/blacklistfilter.py` & `py-Ayiin-0.3.9/pyAyiin/dB/blacklistfilter.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.8/pyAyiin/dB/blacklistgcast.py` & `py-Ayiin-0.3.9/pyAyiin/dB/blacklistgcast.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.8/pyAyiin/dB/blacklistuser.py` & `py-Ayiin-0.3.9/pyAyiin/dB/blacklistuser.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.8/pyAyiin/dB/gban.py` & `py-Ayiin-0.3.9/pyAyiin/dB/gban.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.8/pyAyiin/dB/langs.py` & `py-Ayiin-0.3.9/pyAyiin/dB/langs.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.8/pyAyiin/dB/logdb.py` & `py-Ayiin-0.3.9/pyAyiin/dB/logdb.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.8/pyAyiin/dB/pmpermit.py` & `py-Ayiin-0.3.9/pyAyiin/dB/pmpermit.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.8/pyAyiin/dB/premium.py` & `py-Ayiin-0.3.9/pyAyiin/dB/premium.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.8/pyAyiin/dB/start.py` & `py-Ayiin-0.3.9/pyAyiin/dB/start.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.8/pyAyiin/dB/sudo.py` & `py-Ayiin-0.3.9/pyAyiin/dB/sudo.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.8/pyAyiin/dB/variable.py` & `py-Ayiin-0.3.9/pyAyiin/dB/variable.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.8/pyAyiin/dB/videocalls.py` & `py-Ayiin-0.3.9/pyAyiin/dB/videocalls.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.8/pyAyiin/dB/welcome.py` & `py-Ayiin-0.3.9/pyAyiin/dB/welcome.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.8/pyAyiin/decorator.py` & `py-Ayiin-0.3.9/pyAyiin/decorator.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.8/pyAyiin/exceptions.py` & `py-Ayiin-0.3.9/pyAyiin/exceptions.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.8/pyAyiin/methods/__init__.py` & `py-Ayiin-0.3.9/pyAyiin/methods/__init__.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.8/pyAyiin/methods/_misc.py` & `py-Ayiin-0.3.9/pyAyiin/methods/_misc.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.8/pyAyiin/methods/changer.py` & `py-Ayiin-0.3.9/pyAyiin/methods/changer.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.8/pyAyiin/methods/converter.py` & `py-Ayiin-0.3.9/pyAyiin/methods/converter.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.8/pyAyiin/methods/func.py` & `py-Ayiin-0.3.9/pyAyiin/methods/func.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     from youtubesearchpython import VideosSearch
 except ImportError:
     print("'youtube-search-python' tidak terinstall\nmungkin beberapa modul tidak akan berjalan")
     VideosSearch = None
 
 
 yins = Changers()
+base = "https://www.youtube.com/watch?v="
 
 
 class Funci(object):
     def yt_info_query(self, query: str):
         results = VideosSearch(query, limit=1)
         for result in results.result()["result"]:
             title = result["title"]
@@ -79,23 +80,23 @@
         if stdout:
             return 1, stdout.decode().split("\n")[0]
         else:
             return 0, stderr.decode()
 
 
     async def download(
+        self,
         link: str,
         video: Union[bool, str] = None,
         videoid: Union[bool, str] = None,
         songaudio: Union[bool, str] = None,
         songvideo: Union[bool, str] = None,
         format_id: Union[bool, str] = None,
         title: Union[bool, str] = None,
     ) -> str:
-        base = "https://www.youtube.com/watch?v="
         if videoid:
             link = base + link
         loop = asyncio.get_running_loop()
 
         def audio_dl():
             ydl_optssx = {
                 "format": "bestaudio/best",
```

### Comparing `py-Ayiin-0.3.8/pyAyiin/methods/funcb.py` & `py-Ayiin-0.3.9/pyAyiin/methods/funcb.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.8/pyAyiin/methods/helpers.py` & `py-Ayiin-0.3.9/pyAyiin/methods/helpers.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.8/pyAyiin/methods/hosting.py` & `py-Ayiin-0.3.9/pyAyiin/methods/hosting.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.8/pyAyiin/methods/inlinebot.py` & `py-Ayiin-0.3.9/pyAyiin/methods/inlinebot.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.8/pyAyiin/methods/queue.py` & `py-Ayiin-0.3.9/pyAyiin/methods/queue.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.8/pyAyiin/methods/thumbnail.py` & `py-Ayiin-0.3.9/pyAyiin/methods/thumbnail.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.8/pyAyiin/pyrogram/__init__.py` & `py-Ayiin-0.3.9/pyAyiin/pyrogram/__init__.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.8/pyAyiin/pyrogram/_wrappers.py` & `py-Ayiin-0.3.9/pyAyiin/pyrogram/_wrappers.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.8/pyAyiin/pyrogram/func.py` & `py-Ayiin-0.3.9/pyAyiin/pyrogram/func.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.8/pyAyiin/pyrogram/misc.py` & `py-Ayiin-0.3.9/pyAyiin/pyrogram/misc.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.8/pyAyiin/pyrogram/pastebin.py` & `py-Ayiin-0.3.9/pyAyiin/pyrogram/pastebin.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.8/pyAyiin/pyrogram/sections.py` & `py-Ayiin-0.3.9/pyAyiin/pyrogram/sections.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.8/pyAyiin/pyrogram/toolbot.py` & `py-Ayiin-0.3.9/pyAyiin/pyrogram/toolbot.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.8/pyAyiin/pyrogram/tools.py` & `py-Ayiin-0.3.9/pyAyiin/pyrogram/tools.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.8/pyAyiin/telethon/ayiin/_wrappers.py` & `py-Ayiin-0.3.9/pyAyiin/telethon/ayiin/_wrappers.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.8/pyAyiin/telethon/ayiin/events.py` & `py-Ayiin-0.3.9/pyAyiin/telethon/ayiin/events.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.8/pyAyiin/telethon/ayiin/misc.py` & `py-Ayiin-0.3.9/pyAyiin/telethon/ayiin/misc.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.8/pyAyiin/xd.py` & `py-Ayiin-0.3.9/pyAyiin/xd.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.8/py_Ayiin.egg-info/PKG-INFO` & `py-Ayiin-0.3.9/py_Ayiin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-Ayiin
-Version: 0.3.8
+Version: 0.3.9
 Summary: A Secure and Powerful Python-Telethon Based and Python-Pyrogram Based Library For Your Userbot Module.
 Home-page: https://github.com/AyiinXd/AyiinXd
 Author: AyiinXd
 Author-email: ayingaming98@gmail.com
 License: GNU General Public License v3.0 (GPL-3.0)
 Project-URL: Bug Tracker, https://github.com/AyiinXd/AyiinXd/issues
 Project-URL: Source Code, https://github.com/AyiinXd/AyiinXd
```

### Comparing `py-Ayiin-0.3.8/py_Ayiin.egg-info/SOURCES.txt` & `py-Ayiin-0.3.9/py_Ayiin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.3.8/setup.py` & `py-Ayiin-0.3.9/setup.py`

 * *Files identical despite different names*

