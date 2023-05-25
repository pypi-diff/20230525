# Comparing `tmp/SpyWare-1.0.4.tar.gz` & `tmp/SpyWare-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SpyWare-1.0.4.tar", last modified: Thu Jan  5 08:11:31 2023, max compression
+gzip compressed data, was "SpyWare-1.0.5.tar", last modified: Thu May 25 19:22:55 2023, max compression
```

## Comparing `SpyWare-1.0.4.tar` & `SpyWare-1.0.5.tar`

### file list

```diff
@@ -1,63 +1,65 @@
-drwxrwxr-x   0 christophe  (1001) christophe  (1001)        0 2023-01-05 08:11:31.378724 SpyWare-1.0.4/
--rw-rw-r--   0 christophe  (1001) christophe  (1001)    35821 2023-01-04 17:40:06.000000 SpyWare-1.0.4/LICENSE.txt
--rw-rw-r--   0 christophe  (1001) christophe  (1001)      154 2023-01-04 17:40:06.000000 SpyWare-1.0.4/MANIFEST.in
--rw-rw-r--   0 christophe  (1001) christophe  (1001)    16496 2023-01-05 08:11:31.378724 SpyWare-1.0.4/PKG-INFO
--rw-rw-r--   0 christophe  (1001) christophe  (1001)    98362 2023-01-04 17:40:06.000000 SpyWare-1.0.4/PyAudio-0.2.11-cp310-cp310-win32.whl
--rw-rw-r--   0 christophe  (1001) christophe  (1001)   113705 2023-01-04 17:40:06.000000 SpyWare-1.0.4/PyAudio-0.2.11-cp310-cp310-win_amd64.whl
--rw-rw-r--   0 christophe  (1001) christophe  (1001)    98389 2023-01-04 17:40:06.000000 SpyWare-1.0.4/PyAudio-0.2.11-cp38-cp38-win32.whl
--rw-rw-r--   0 christophe  (1001) christophe  (1001)   113700 2023-01-04 17:40:06.000000 SpyWare-1.0.4/PyAudio-0.2.11-cp38-cp38-win_amd64.whl
--rw-rw-r--   0 christophe  (1001) christophe  (1001)    96271 2023-01-04 17:40:06.000000 SpyWare-1.0.4/PyAudio-0.2.11-cp39-cp39-win32.whl
--rw-rw-r--   0 christophe  (1001) christophe  (1001)   110308 2023-01-04 17:40:06.000000 SpyWare-1.0.4/PyAudio-0.2.11-cp39-cp39-win_amd64.whl
--rw-rw-r--   0 christophe  (1001) christophe  (1001)    11138 2023-01-04 17:40:06.000000 SpyWare-1.0.4/README.md
-drwxrwxr-x   0 christophe  (1001) christophe  (1001)        0 2023-01-05 08:11:31.374724 SpyWare-1.0.4/SpyWare/
-drwxrwxr-x   0 christophe  (1001) christophe  (1001)        0 2023-01-05 08:11:31.374724 SpyWare-1.0.4/SpyWare/AudioLogger/
--rw-rw-r--   0 christophe  (1001) christophe  (1001)     6254 2023-01-04 17:40:06.000000 SpyWare-1.0.4/SpyWare/AudioLogger/AudioLogger.py
--rw-rw-r--   0 christophe  (1001) christophe  (1001)     2262 2023-01-04 17:40:06.000000 SpyWare-1.0.4/SpyWare/AudioLogger/__init__.py
--rw-rw-r--   0 christophe  (1001) christophe  (1001)     1748 2023-01-04 17:40:06.000000 SpyWare-1.0.4/SpyWare/AudioLogger/__main__.py
--rw-rw-r--   0 christophe  (1001) christophe  (1001)       94 2023-01-04 17:40:06.000000 SpyWare-1.0.4/SpyWare/AudioLogger/audioSpy.conf
-drwxrwxr-x   0 christophe  (1001) christophe  (1001)        0 2023-01-05 08:11:31.374724 SpyWare-1.0.4/SpyWare/ClipboardLogger/
--rw-rw-r--   0 christophe  (1001) christophe  (1001)     5989 2023-01-04 17:40:06.000000 SpyWare-1.0.4/SpyWare/ClipboardLogger/ClipboardLogger.py
--rw-rw-r--   0 christophe  (1001) christophe  (1001)     2354 2023-01-04 17:40:06.000000 SpyWare-1.0.4/SpyWare/ClipboardLogger/__init__.py
--rw-rw-r--   0 christophe  (1001) christophe  (1001)     1766 2023-01-04 17:40:06.000000 SpyWare-1.0.4/SpyWare/ClipboardLogger/__main__.py
--rw-rw-r--   0 christophe  (1001) christophe  (1001)       58 2023-01-04 17:40:06.000000 SpyWare-1.0.4/SpyWare/ClipboardLogger/clipboardSpy.conf
-drwxrwxr-x   0 christophe  (1001) christophe  (1001)        0 2023-01-05 08:11:31.374724 SpyWare-1.0.4/SpyWare/DomainsLogger/
--rw-rw-r--   0 christophe  (1001) christophe  (1001)    11782 2023-01-05 08:07:38.000000 SpyWare-1.0.4/SpyWare/DomainsLogger/DomainsLogger.py
--rw-rw-r--   0 christophe  (1001) christophe  (1001)     2384 2023-01-05 08:08:29.000000 SpyWare-1.0.4/SpyWare/DomainsLogger/__init__.py
--rw-rw-r--   0 christophe  (1001) christophe  (1001)     1749 2023-01-05 08:08:52.000000 SpyWare-1.0.4/SpyWare/DomainsLogger/__main__.py
--rw-rw-r--   0 christophe  (1001) christophe  (1001)      141 2023-01-04 17:40:06.000000 SpyWare-1.0.4/SpyWare/DomainsLogger/domainsSpy.conf
-drwxrwxr-x   0 christophe  (1001) christophe  (1001)        0 2023-01-05 08:11:31.374724 SpyWare-1.0.4/SpyWare/FilesLogger/
--rw-rw-r--   0 christophe  (1001) christophe  (1001)     8149 2023-01-04 17:40:06.000000 SpyWare-1.0.4/SpyWare/FilesLogger/FilesLogger.py
--rw-rw-r--   0 christophe  (1001) christophe  (1001)     2209 2023-01-04 17:40:06.000000 SpyWare-1.0.4/SpyWare/FilesLogger/__init__.py
--rw-rw-r--   0 christophe  (1001) christophe  (1001)     2042 2023-01-04 17:40:06.000000 SpyWare-1.0.4/SpyWare/FilesLogger/__main__.py
--rw-rw-r--   0 christophe  (1001) christophe  (1001)      106 2023-01-04 17:40:06.000000 SpyWare-1.0.4/SpyWare/FilesLogger/filesSpy.conf
-drwxrwxr-x   0 christophe  (1001) christophe  (1001)        0 2023-01-05 08:11:31.374724 SpyWare-1.0.4/SpyWare/KeyLogger/
--rw-rw-r--   0 christophe  (1001) christophe  (1001)     7104 2023-01-04 17:40:06.000000 SpyWare-1.0.4/SpyWare/KeyLogger/KeyLogger.py
--rw-rw-r--   0 christophe  (1001) christophe  (1001)     1643 2023-01-04 17:40:06.000000 SpyWare-1.0.4/SpyWare/KeyLogger/__init__.py
--rw-rw-r--   0 christophe  (1001) christophe  (1001)     1665 2023-01-04 17:40:06.000000 SpyWare-1.0.4/SpyWare/KeyLogger/__main__.py
--rw-rw-r--   0 christophe  (1001) christophe  (1001)      107 2023-01-04 17:40:06.000000 SpyWare-1.0.4/SpyWare/KeyLogger/keySpy.conf
-drwxrwxr-x   0 christophe  (1001) christophe  (1001)        0 2023-01-05 08:11:31.378724 SpyWare-1.0.4/SpyWare/ScreenLogger/
--rw-rw-r--   0 christophe  (1001) christophe  (1001)     4911 2023-01-04 17:40:06.000000 SpyWare-1.0.4/SpyWare/ScreenLogger/ScreenLogger.py
--rw-rw-r--   0 christophe  (1001) christophe  (1001)     1719 2023-01-04 17:40:06.000000 SpyWare-1.0.4/SpyWare/ScreenLogger/__init__.py
--rw-rw-r--   0 christophe  (1001) christophe  (1001)     1720 2023-01-04 17:40:06.000000 SpyWare-1.0.4/SpyWare/ScreenLogger/__main__.py
--rw-rw-r--   0 christophe  (1001) christophe  (1001)       95 2023-01-04 17:40:06.000000 SpyWare-1.0.4/SpyWare/ScreenLogger/screenSpy.conf
--rw-rw-r--   0 christophe  (1001) christophe  (1001)    16391 2023-01-05 08:10:58.000000 SpyWare-1.0.4/SpyWare/SpyWare.py
-drwxrwxr-x   0 christophe  (1001) christophe  (1001)        0 2023-01-05 08:11:31.378724 SpyWare-1.0.4/SpyWare/WebcamLogger/
--rw-rw-r--   0 christophe  (1001) christophe  (1001)     5007 2023-01-04 17:40:06.000000 SpyWare-1.0.4/SpyWare/WebcamLogger/WebcamLogger.py
--rw-rw-r--   0 christophe  (1001) christophe  (1001)     1731 2023-01-04 17:40:06.000000 SpyWare-1.0.4/SpyWare/WebcamLogger/__init__.py
--rw-rw-r--   0 christophe  (1001) christophe  (1001)     1732 2023-01-04 17:40:06.000000 SpyWare-1.0.4/SpyWare/WebcamLogger/__main__.py
--rw-rw-r--   0 christophe  (1001) christophe  (1001)       85 2023-01-04 17:40:06.000000 SpyWare-1.0.4/SpyWare/WebcamLogger/webcamSpy.conf
--rw-rw-r--   0 christophe  (1001) christophe  (1001)     2256 2023-01-05 08:11:12.000000 SpyWare-1.0.4/SpyWare/__init__.py
--rw-rw-r--   0 christophe  (1001) christophe  (1001)     1667 2023-01-05 08:11:04.000000 SpyWare-1.0.4/SpyWare/__main__.py
-drwxrwxr-x   0 christophe  (1001) christophe  (1001)        0 2023-01-05 08:11:31.374724 SpyWare-1.0.4/SpyWare.egg-info/
--rw-rw-r--   0 christophe  (1001) christophe  (1001)    16496 2023-01-05 08:11:31.000000 SpyWare-1.0.4/SpyWare.egg-info/PKG-INFO
--rw-rw-r--   0 christophe  (1001) christophe  (1001)     1544 2023-01-05 08:11:31.000000 SpyWare-1.0.4/SpyWare.egg-info/SOURCES.txt
--rw-rw-r--   0 christophe  (1001) christophe  (1001)        1 2023-01-05 08:11:31.000000 SpyWare-1.0.4/SpyWare.egg-info/dependency_links.txt
--rw-rw-r--   0 christophe  (1001) christophe  (1001)       45 2023-01-05 08:11:31.000000 SpyWare-1.0.4/SpyWare.egg-info/entry_points.txt
--rw-rw-r--   0 christophe  (1001) christophe  (1001)       48 2023-01-05 08:11:31.000000 SpyWare-1.0.4/SpyWare.egg-info/requires.txt
--rw-rw-r--   0 christophe  (1001) christophe  (1001)        8 2023-01-05 08:11:31.000000 SpyWare-1.0.4/SpyWare.egg-info/top_level.txt
--rw-rw-r--   0 christophe  (1001) christophe  (1001)    16191 2023-01-04 17:40:06.000000 SpyWare-1.0.4/SpyWare.ico
--rw-rw-r--   0 christophe  (1001) christophe  (1001)       98 2023-01-04 17:40:06.000000 SpyWare-1.0.4/compilateur.bat
--rw-rw-r--   0 christophe  (1001) christophe  (1001)      232 2023-01-04 17:40:06.000000 SpyWare-1.0.4/compile.bat
--rw-rw-r--   0 christophe  (1001) christophe  (1001)      889 2023-01-04 17:40:06.000000 SpyWare-1.0.4/file_version_info.txt
--rw-rw-r--   0 christophe  (1001) christophe  (1001)       38 2023-01-05 08:11:31.378724 SpyWare-1.0.4/setup.cfg
--rw-rw-r--   0 christophe  (1001) christophe  (1001)     4978 2023-01-05 08:10:35.000000 SpyWare-1.0.4/setup.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-05-25 19:22:55.783665 SpyWare-1.0.5/
+-rw-r--r--   0 kali      (1000) kali      (1000)    35821 2023-05-26 01:17:24.000000 SpyWare-1.0.5/LICENSE.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)      154 2023-05-26 01:17:24.000000 SpyWare-1.0.5/MANIFEST.in
+-rw-r--r--   0 kali      (1000) kali      (1000)    13877 2023-05-25 19:22:55.783665 SpyWare-1.0.5/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)    98362 2023-05-26 01:17:24.000000 SpyWare-1.0.5/PyAudio-0.2.11-cp310-cp310-win32.whl
+-rw-r--r--   0 kali      (1000) kali      (1000)   113705 2023-05-26 01:17:24.000000 SpyWare-1.0.5/PyAudio-0.2.11-cp310-cp310-win_amd64.whl
+-rw-r--r--   0 kali      (1000) kali      (1000)    98389 2023-05-26 01:17:24.000000 SpyWare-1.0.5/PyAudio-0.2.11-cp38-cp38-win32.whl
+-rw-r--r--   0 kali      (1000) kali      (1000)   113700 2023-05-26 01:17:24.000000 SpyWare-1.0.5/PyAudio-0.2.11-cp38-cp38-win_amd64.whl
+-rw-r--r--   0 kali      (1000) kali      (1000)    96271 2023-05-26 01:17:24.000000 SpyWare-1.0.5/PyAudio-0.2.11-cp39-cp39-win32.whl
+-rw-r--r--   0 kali      (1000) kali      (1000)   110308 2023-05-26 01:17:24.000000 SpyWare-1.0.5/PyAudio-0.2.11-cp39-cp39-win_amd64.whl
+-rw-r--r--   0 kali      (1000) kali      (1000)   144626 2023-05-26 01:20:22.000000 SpyWare-1.0.5/PyAudio-0.2.13-cp311-cp311-win32.whl
+-rw-r--r--   0 kali      (1000) kali      (1000)   164070 2023-05-26 01:20:20.000000 SpyWare-1.0.5/PyAudio-0.2.13-cp311-cp311-win_amd64.whl
+-rw-r--r--   0 kali      (1000) kali      (1000)    11138 2023-05-26 01:17:24.000000 SpyWare-1.0.5/README.md
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-05-25 19:22:55.775661 SpyWare-1.0.5/SpyWare/
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-05-25 19:22:55.779662 SpyWare-1.0.5/SpyWare/AudioLogger/
+-rw-r--r--   0 kali      (1000) kali      (1000)     6254 2023-05-26 01:17:24.000000 SpyWare-1.0.5/SpyWare/AudioLogger/AudioLogger.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     2262 2023-05-26 01:17:24.000000 SpyWare-1.0.5/SpyWare/AudioLogger/__init__.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     1748 2023-05-26 01:17:24.000000 SpyWare-1.0.5/SpyWare/AudioLogger/__main__.py
+-rw-r--r--   0 kali      (1000) kali      (1000)       94 2023-05-26 01:17:24.000000 SpyWare-1.0.5/SpyWare/AudioLogger/audioSpy.conf
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-05-25 19:22:55.779662 SpyWare-1.0.5/SpyWare/ClipboardLogger/
+-rw-r--r--   0 kali      (1000) kali      (1000)     5989 2023-05-26 01:17:24.000000 SpyWare-1.0.5/SpyWare/ClipboardLogger/ClipboardLogger.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     2354 2023-05-26 01:17:24.000000 SpyWare-1.0.5/SpyWare/ClipboardLogger/__init__.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     1766 2023-05-26 01:17:24.000000 SpyWare-1.0.5/SpyWare/ClipboardLogger/__main__.py
+-rw-r--r--   0 kali      (1000) kali      (1000)       58 2023-05-26 01:17:24.000000 SpyWare-1.0.5/SpyWare/ClipboardLogger/clipboardSpy.conf
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-05-25 19:22:55.779662 SpyWare-1.0.5/SpyWare/DomainsLogger/
+-rw-r--r--   0 kali      (1000) kali      (1000)    11782 2023-05-26 01:17:24.000000 SpyWare-1.0.5/SpyWare/DomainsLogger/DomainsLogger.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     2384 2023-05-26 01:17:24.000000 SpyWare-1.0.5/SpyWare/DomainsLogger/__init__.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     1749 2023-05-26 01:17:24.000000 SpyWare-1.0.5/SpyWare/DomainsLogger/__main__.py
+-rw-r--r--   0 kali      (1000) kali      (1000)      141 2023-05-26 01:17:24.000000 SpyWare-1.0.5/SpyWare/DomainsLogger/domainsSpy.conf
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-05-25 19:22:55.779662 SpyWare-1.0.5/SpyWare/FilesLogger/
+-rw-r--r--   0 kali      (1000) kali      (1000)     8149 2023-05-26 01:17:24.000000 SpyWare-1.0.5/SpyWare/FilesLogger/FilesLogger.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     2209 2023-05-26 01:17:24.000000 SpyWare-1.0.5/SpyWare/FilesLogger/__init__.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     2042 2023-05-26 01:17:24.000000 SpyWare-1.0.5/SpyWare/FilesLogger/__main__.py
+-rw-r--r--   0 kali      (1000) kali      (1000)      106 2023-05-26 01:17:26.000000 SpyWare-1.0.5/SpyWare/FilesLogger/filesSpy.conf
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-05-25 19:22:55.783665 SpyWare-1.0.5/SpyWare/KeyLogger/
+-rw-r--r--   0 kali      (1000) kali      (1000)     7104 2023-05-26 01:17:26.000000 SpyWare-1.0.5/SpyWare/KeyLogger/KeyLogger.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     1643 2023-05-26 01:17:26.000000 SpyWare-1.0.5/SpyWare/KeyLogger/__init__.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     1665 2023-05-26 01:17:26.000000 SpyWare-1.0.5/SpyWare/KeyLogger/__main__.py
+-rw-r--r--   0 kali      (1000) kali      (1000)      107 2023-05-26 01:17:26.000000 SpyWare-1.0.5/SpyWare/KeyLogger/keySpy.conf
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-05-25 19:22:55.783665 SpyWare-1.0.5/SpyWare/ScreenLogger/
+-rw-r--r--   0 kali      (1000) kali      (1000)     4911 2023-05-26 01:17:26.000000 SpyWare-1.0.5/SpyWare/ScreenLogger/ScreenLogger.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     1719 2023-05-26 01:17:26.000000 SpyWare-1.0.5/SpyWare/ScreenLogger/__init__.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     1720 2023-05-26 01:17:26.000000 SpyWare-1.0.5/SpyWare/ScreenLogger/__main__.py
+-rw-r--r--   0 kali      (1000) kali      (1000)       95 2023-05-26 01:17:26.000000 SpyWare-1.0.5/SpyWare/ScreenLogger/screenSpy.conf
+-rw-r--r--   0 kali      (1000) kali      (1000)    16391 2023-05-26 01:17:24.000000 SpyWare-1.0.5/SpyWare/SpyWare.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-05-25 19:22:55.783665 SpyWare-1.0.5/SpyWare/WebcamLogger/
+-rw-r--r--   0 kali      (1000) kali      (1000)     5007 2023-05-26 01:17:26.000000 SpyWare-1.0.5/SpyWare/WebcamLogger/WebcamLogger.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     1731 2023-05-26 01:17:26.000000 SpyWare-1.0.5/SpyWare/WebcamLogger/__init__.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     1732 2023-05-26 01:17:26.000000 SpyWare-1.0.5/SpyWare/WebcamLogger/__main__.py
+-rw-r--r--   0 kali      (1000) kali      (1000)       85 2023-05-26 01:17:26.000000 SpyWare-1.0.5/SpyWare/WebcamLogger/webcamSpy.conf
+-rw-r--r--   0 kali      (1000) kali      (1000)     2256 2023-05-26 01:18:46.000000 SpyWare-1.0.5/SpyWare/__init__.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     1667 2023-05-26 01:17:24.000000 SpyWare-1.0.5/SpyWare/__main__.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-05-25 19:22:55.779662 SpyWare-1.0.5/SpyWare.egg-info/
+-rw-r--r--   0 kali      (1000) kali      (1000)    13877 2023-05-25 19:22:55.000000 SpyWare-1.0.5/SpyWare.egg-info/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)     1632 2023-05-25 19:22:55.000000 SpyWare-1.0.5/SpyWare.egg-info/SOURCES.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-05-25 19:22:55.000000 SpyWare-1.0.5/SpyWare.egg-info/dependency_links.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       44 2023-05-25 19:22:55.000000 SpyWare-1.0.5/SpyWare.egg-info/entry_points.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       48 2023-05-25 19:22:55.000000 SpyWare-1.0.5/SpyWare.egg-info/requires.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        8 2023-05-25 19:22:55.000000 SpyWare-1.0.5/SpyWare.egg-info/top_level.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)    16191 2023-05-26 01:17:24.000000 SpyWare-1.0.5/SpyWare.ico
+-rw-r--r--   0 kali      (1000) kali      (1000)       98 2023-05-26 01:17:24.000000 SpyWare-1.0.5/compilateur.bat
+-rw-r--r--   0 kali      (1000) kali      (1000)      232 2023-05-26 01:17:24.000000 SpyWare-1.0.5/compile.bat
+-rw-r--r--   0 kali      (1000) kali      (1000)      889 2023-05-26 01:17:24.000000 SpyWare-1.0.5/file_version_info.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       38 2023-05-25 19:22:55.783665 SpyWare-1.0.5/setup.cfg
+-rw-r--r--   0 kali      (1000) kali      (1000)     4977 2023-05-26 01:18:28.000000 SpyWare-1.0.5/setup.py
```

### Comparing `SpyWare-1.0.4/LICENSE.txt` & `SpyWare-1.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `SpyWare-1.0.4/PyAudio-0.2.11-cp310-cp310-win32.whl` & `SpyWare-1.0.5/PyAudio-0.2.11-cp310-cp310-win32.whl`

 * *Files identical despite different names*

### Comparing `SpyWare-1.0.4/PyAudio-0.2.11-cp310-cp310-win_amd64.whl` & `SpyWare-1.0.5/PyAudio-0.2.11-cp310-cp310-win_amd64.whl`

 * *Files identical despite different names*

### Comparing `SpyWare-1.0.4/PyAudio-0.2.11-cp38-cp38-win32.whl` & `SpyWare-1.0.5/PyAudio-0.2.11-cp38-cp38-win32.whl`

 * *Files identical despite different names*

### Comparing `SpyWare-1.0.4/PyAudio-0.2.11-cp38-cp38-win_amd64.whl` & `SpyWare-1.0.5/PyAudio-0.2.11-cp38-cp38-win_amd64.whl`

 * *Files identical despite different names*

### Comparing `SpyWare-1.0.4/PyAudio-0.2.11-cp39-cp39-win32.whl` & `SpyWare-1.0.5/PyAudio-0.2.11-cp39-cp39-win32.whl`

 * *Files identical despite different names*

### Comparing `SpyWare-1.0.4/PyAudio-0.2.11-cp39-cp39-win_amd64.whl` & `SpyWare-1.0.5/PyAudio-0.2.11-cp39-cp39-win_amd64.whl`

 * *Files identical despite different names*

### Comparing `SpyWare-1.0.4/README.md` & `SpyWare-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `SpyWare-1.0.4/SpyWare/AudioLogger/AudioLogger.py` & `SpyWare-1.0.5/SpyWare/AudioLogger/AudioLogger.py`

 * *Files identical despite different names*

### Comparing `SpyWare-1.0.4/SpyWare/AudioLogger/__init__.py` & `SpyWare-1.0.5/SpyWare/AudioLogger/__init__.py`

 * *Files identical despite different names*

### Comparing `SpyWare-1.0.4/SpyWare/AudioLogger/__main__.py` & `SpyWare-1.0.5/SpyWare/AudioLogger/__main__.py`

 * *Files identical despite different names*

### Comparing `SpyWare-1.0.4/SpyWare/ClipboardLogger/ClipboardLogger.py` & `SpyWare-1.0.5/SpyWare/ClipboardLogger/ClipboardLogger.py`

 * *Files identical despite different names*

### Comparing `SpyWare-1.0.4/SpyWare/ClipboardLogger/__init__.py` & `SpyWare-1.0.5/SpyWare/ClipboardLogger/__init__.py`

 * *Files identical despite different names*

### Comparing `SpyWare-1.0.4/SpyWare/ClipboardLogger/__main__.py` & `SpyWare-1.0.5/SpyWare/ClipboardLogger/__main__.py`

 * *Files identical despite different names*

### Comparing `SpyWare-1.0.4/SpyWare/DomainsLogger/DomainsLogger.py` & `SpyWare-1.0.5/SpyWare/DomainsLogger/DomainsLogger.py`

 * *Files identical despite different names*

### Comparing `SpyWare-1.0.4/SpyWare/DomainsLogger/__init__.py` & `SpyWare-1.0.5/SpyWare/DomainsLogger/__init__.py`

 * *Files identical despite different names*

### Comparing `SpyWare-1.0.4/SpyWare/DomainsLogger/__main__.py` & `SpyWare-1.0.5/SpyWare/DomainsLogger/__main__.py`

 * *Files identical despite different names*

### Comparing `SpyWare-1.0.4/SpyWare/FilesLogger/FilesLogger.py` & `SpyWare-1.0.5/SpyWare/FilesLogger/FilesLogger.py`

 * *Files identical despite different names*

### Comparing `SpyWare-1.0.4/SpyWare/FilesLogger/__init__.py` & `SpyWare-1.0.5/SpyWare/FilesLogger/__init__.py`

 * *Files identical despite different names*

### Comparing `SpyWare-1.0.4/SpyWare/FilesLogger/__main__.py` & `SpyWare-1.0.5/SpyWare/FilesLogger/__main__.py`

 * *Files identical despite different names*

### Comparing `SpyWare-1.0.4/SpyWare/KeyLogger/KeyLogger.py` & `SpyWare-1.0.5/SpyWare/KeyLogger/KeyLogger.py`

 * *Files identical despite different names*

### Comparing `SpyWare-1.0.4/SpyWare/KeyLogger/__init__.py` & `SpyWare-1.0.5/SpyWare/KeyLogger/__init__.py`

 * *Files identical despite different names*

### Comparing `SpyWare-1.0.4/SpyWare/KeyLogger/__main__.py` & `SpyWare-1.0.5/SpyWare/KeyLogger/__main__.py`

 * *Files identical despite different names*

### Comparing `SpyWare-1.0.4/SpyWare/ScreenLogger/ScreenLogger.py` & `SpyWare-1.0.5/SpyWare/ScreenLogger/ScreenLogger.py`

 * *Files identical despite different names*

### Comparing `SpyWare-1.0.4/SpyWare/ScreenLogger/__init__.py` & `SpyWare-1.0.5/SpyWare/ScreenLogger/__init__.py`

 * *Files identical despite different names*

### Comparing `SpyWare-1.0.4/SpyWare/ScreenLogger/__main__.py` & `SpyWare-1.0.5/SpyWare/ScreenLogger/__main__.py`

 * *Files identical despite different names*

### Comparing `SpyWare-1.0.4/SpyWare/SpyWare.py` & `SpyWare-1.0.5/SpyWare/SpyWare.py`

 * *Files identical despite different names*

### Comparing `SpyWare-1.0.4/SpyWare/WebcamLogger/WebcamLogger.py` & `SpyWare-1.0.5/SpyWare/WebcamLogger/WebcamLogger.py`

 * *Files identical despite different names*

### Comparing `SpyWare-1.0.4/SpyWare/WebcamLogger/__init__.py` & `SpyWare-1.0.5/SpyWare/WebcamLogger/__init__.py`

 * *Files identical despite different names*

### Comparing `SpyWare-1.0.4/SpyWare/WebcamLogger/__main__.py` & `SpyWare-1.0.5/SpyWare/WebcamLogger/__main__.py`

 * *Files identical despite different names*

### Comparing `SpyWare-1.0.4/SpyWare/__init__.py` & `SpyWare-1.0.5/SpyWare/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 #    along with this program.  If not, see <https://www.gnu.org/licenses/>.
 ###################
 
 """
 This file implements a complete spyware.
 """
 
-__version__ = "1.0.4"
+__version__ = "1.0.5"
 __author__ = "Maurice Lambert"
 __author_email__ = "mauricelambert434@gmail.com"
 __maintainer__ = "Maurice Lambert"
 __maintainer_email__ = "mauricelambert434@gmail.com"
 __description__ = """
 This file implements a complete spyware.
 """
```

### Comparing `SpyWare-1.0.4/SpyWare/__main__.py` & `SpyWare-1.0.5/SpyWare/__main__.py`

 * *Files identical despite different names*

### Comparing `SpyWare-1.0.4/SpyWare.egg-info/SOURCES.txt` & `SpyWare-1.0.5/SpyWare.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -2,19 +2,22 @@
 MANIFEST.in
 PyAudio-0.2.11-cp310-cp310-win32.whl
 PyAudio-0.2.11-cp310-cp310-win_amd64.whl
 PyAudio-0.2.11-cp38-cp38-win32.whl
 PyAudio-0.2.11-cp38-cp38-win_amd64.whl
 PyAudio-0.2.11-cp39-cp39-win32.whl
 PyAudio-0.2.11-cp39-cp39-win_amd64.whl
+PyAudio-0.2.13-cp311-cp311-win32.whl
+PyAudio-0.2.13-cp311-cp311-win_amd64.whl
 README.md
 SpyWare.ico
 compilateur.bat
 compile.bat
 file_version_info.txt
+setup.cfg
 setup.py
 SpyWare/SpyWare.py
 SpyWare/__init__.py
 SpyWare/__main__.py
 SpyWare.egg-info/PKG-INFO
 SpyWare.egg-info/SOURCES.txt
 SpyWare.egg-info/dependency_links.txt
```

### Comparing `SpyWare-1.0.4/SpyWare.ico` & `SpyWare-1.0.5/SpyWare.ico`

 * *Files identical despite different names*

### Comparing `SpyWare-1.0.4/file_version_info.txt` & `SpyWare-1.0.5/file_version_info.txt`

 * *Files identical despite different names*

### Comparing `SpyWare-1.0.4/setup.py` & `SpyWare-1.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,22 @@
 from sys import maxsize, executable, version_info
 from setuptools.command.install import install
 from setuptools import setup, find_packages
 from os import system as exec_command
 from platform import system
 
 
+packages = [
+    "pyautogui",
+    "opencv-python",
+    "pillow",
+    "pyperclip",
+    "pynput",
+]
+
 class PostInstallScript(install):
 
     """
     This class install the PyAudio module.
     """
 
     def is_64bit(self) -> bool:
@@ -46,23 +54,17 @@
 
         self.install_pyaudio()
         install.run(self)
 
 
 setup(
     name="SpyWare",
-    version="1.0.4",
+    version="1.0.5",
     packages=find_packages(include=["SpyWare"]),
-    install_requires=[
-        "pyautogui",
-        "opencv-python",
-        "pillow",
-        "pyperclip",
-        "pynput",
-    ],
+    install_requires=packages,
     author="Maurice Lambert",
     author_email="mauricelambert434@gmail.com",
     maintainer="Maurice Lambert",
     maintainer_email="mauricelambert434@gmail.com",
     description="This package implements a complete SpyWare.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
```

