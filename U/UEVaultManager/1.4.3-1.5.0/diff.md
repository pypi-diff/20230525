# Comparing `tmp/UEVaultManager-1.4.3.tar.gz` & `tmp/UEVaultManager-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UEVaultManager-1.4.3.tar", last modified: Tue May 23 13:51:01 2023, max compression
+gzip compressed data, was "UEVaultManager-1.5.0.tar", last modified: Thu May 25 09:58:15 2023, max compression
```

## Comparing `UEVaultManager-1.4.3.tar` & `UEVaultManager-1.5.0.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 13:51:01.048076 UEVaultManager-1.4.3/
--rw-rw-rw-   0        0        0    35823 2023-01-05 18:12:15.000000 UEVaultManager-1.4.3/LICENSE
--rw-rw-rw-   0        0        0     6129 2023-05-23 13:51:01.047077 UEVaultManager-1.4.3/PKG-INFO
--rw-rw-rw-   0        0        0     5285 2023-05-23 13:48:41.000000 UEVaultManager-1.4.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-23 13:51:00.878845 UEVaultManager-1.4.3/UEVaultManager/
--rw-rw-rw-   0        0        0      780 2023-05-23 13:49:41.000000 UEVaultManager-1.4.3/UEVaultManager/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-23 13:51:00.916412 UEVaultManager-1.4.3/UEVaultManager/api/
--rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.4.3/UEVaultManager/api/__init__.py
--rw-rw-rw-   0        0        0    25469 2023-05-18 09:30:29.000000 UEVaultManager-1.4.3/UEVaultManager/api/egs.py
--rw-rw-rw-   0        0        0     3142 2023-05-17 13:34:09.000000 UEVaultManager-1.4.3/UEVaultManager/api/uevm.py
-drwxrwxrwx   0        0        0        0 2023-05-23 13:51:00.925891 UEVaultManager-1.4.3/UEVaultManager/assets/
--rw-rw-rw-   0        0        0    20282 2023-05-11 14:38:28.000000 UEVaultManager-1.4.3/UEVaultManager/assets/UEVM_200x200.png
--rw-rw-rw-   0        0        0      432 2023-05-21 17:27:34.000000 UEVaultManager-1.4.3/UEVaultManager/assets/checked_16.png
--rw-rw-rw-   0        0        0     4286 2023-05-11 14:38:28.000000 UEVaultManager-1.4.3/UEVaultManager/assets/main.ico
--rw-rw-rw-   0        0        0      187 2023-05-21 17:27:58.000000 UEVaultManager-1.4.3/UEVaultManager/assets/unchecked_16.png
--rw-rw-rw-   0        0        0    71745 2023-05-22 10:32:14.000000 UEVaultManager-1.4.3/UEVaultManager/cli.py
--rw-rw-rw-   0        0        0    47574 2023-05-22 13:00:35.000000 UEVaultManager-1.4.3/UEVaultManager/core.py
-drwxrwxrwx   0        0        0        0 2023-05-23 13:51:00.931891 UEVaultManager-1.4.3/UEVaultManager/downloader/
--rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.4.3/UEVaultManager/downloader/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-23 13:51:00.945175 UEVaultManager-1.4.3/UEVaultManager/downloader/mp/
--rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.4.3/UEVaultManager/downloader/mp/__init__.py
--rw-rw-rw-   0        0        0    38030 2023-05-15 06:30:52.000000 UEVaultManager-1.4.3/UEVaultManager/downloader/mp/manager.py
--rw-rw-rw-   0        0        0    12365 2023-05-17 13:38:36.000000 UEVaultManager-1.4.3/UEVaultManager/downloader/mp/workers.py
-drwxrwxrwx   0        0        0        0 2023-05-23 13:51:00.963524 UEVaultManager-1.4.3/UEVaultManager/lfs/
--rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.4.3/UEVaultManager/lfs/__init__.py
--rw-rw-rw-   0        0        0     3611 2023-05-11 14:38:28.000000 UEVaultManager-1.4.3/UEVaultManager/lfs/egl.py
--rw-rw-rw-   0        0        0     6428 2023-05-15 06:51:22.000000 UEVaultManager-1.4.3/UEVaultManager/lfs/eos.py
--rw-rw-rw-   0        0        0    23209 2023-05-21 07:37:16.000000 UEVaultManager-1.4.3/UEVaultManager/lfs/uevmlfs.py
--rw-rw-rw-   0        0        0      593 2023-05-15 06:35:46.000000 UEVaultManager-1.4.3/UEVaultManager/lfs/utils.py
--rw-rw-rw-   0        0        0     3122 2023-05-15 06:51:32.000000 UEVaultManager-1.4.3/UEVaultManager/lfs/windows_helpers.py
-drwxrwxrwx   0        0        0        0 2023-05-23 13:51:00.986530 UEVaultManager-1.4.3/UEVaultManager/models/
--rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.4.3/UEVaultManager/models/__init__.py
--rw-rw-rw-   0        0        0     4269 2023-05-17 13:38:36.000000 UEVaultManager-1.4.3/UEVaultManager/models/app.py
--rw-rw-rw-   0        0        0     4478 2023-05-11 14:38:28.000000 UEVaultManager-1.4.3/UEVaultManager/models/chunk.py
--rw-rw-rw-   0        0        0     2703 2023-05-20 09:18:48.000000 UEVaultManager-1.4.3/UEVaultManager/models/config.py
--rw-rw-rw-   0        0        0     2131 2023-05-22 12:33:51.000000 UEVaultManager-1.4.3/UEVaultManager/models/csv.py
--rw-rw-rw-   0        0        0     3627 2023-05-11 14:38:28.000000 UEVaultManager-1.4.3/UEVaultManager/models/downloading.py
--rw-rw-rw-   0        0        0     5094 2023-05-15 06:33:02.000000 UEVaultManager-1.4.3/UEVaultManager/models/egl.py
--rw-rw-rw-   0        0        0      256 2023-05-20 09:20:19.000000 UEVaultManager-1.4.3/UEVaultManager/models/exceptions.py
--rw-rw-rw-   0        0        0     5893 2023-05-15 06:30:52.000000 UEVaultManager-1.4.3/UEVaultManager/models/json_manifest.py
--rw-rw-rw-   0        0        0    30505 2023-05-17 13:38:36.000000 UEVaultManager-1.4.3/UEVaultManager/models/manifest.py
-drwxrwxrwx   0        0        0        0 2023-05-23 13:51:00.993488 UEVaultManager-1.4.3/UEVaultManager/tkgui/
--rw-rw-rw-   0        0        0       16 2023-05-14 16:45:45.000000 UEVaultManager-1.4.3/UEVaultManager/tkgui/__init__.py
--rw-rw-rw-   0        0        0     1123 2023-05-20 07:12:03.000000 UEVaultManager-1.4.3/UEVaultManager/tkgui/main.py
-drwxrwxrwx   0        0        0        0 2023-05-23 13:51:01.025077 UEVaultManager-1.4.3/UEVaultManager/tkgui/modules/
--rw-rw-rw-   0        0        0     6667 2023-05-23 13:36:34.000000 UEVaultManager-1.4.3/UEVaultManager/tkgui/modules/DisplayContentWindowClass.py
--rw-rw-rw-   0        0        0     4562 2023-05-23 13:37:02.000000 UEVaultManager-1.4.3/UEVaultManager/tkgui/modules/EditCellWindowClass.py
--rw-rw-rw-   0        0        0     6553 2023-05-23 13:36:54.000000 UEVaultManager-1.4.3/UEVaultManager/tkgui/modules/EditRowWindowClass.py
--rw-rw-rw-   0        0        0    32447 2023-05-22 17:07:09.000000 UEVaultManager-1.4.3/UEVaultManager/tkgui/modules/EditableTableClass.py
--rw-rw-rw-   0        0        0    14038 2023-05-22 16:36:16.000000 UEVaultManager-1.4.3/UEVaultManager/tkgui/modules/ExtendedWidgetClasses.py
--rw-rw-rw-   0        0        0     2562 2023-05-22 14:44:53.000000 UEVaultManager-1.4.3/UEVaultManager/tkgui/modules/GUISettingsClass.py
--rw-rw-rw-   0        0        0    13947 2023-05-23 13:37:12.000000 UEVaultManager-1.4.3/UEVaultManager/tkgui/modules/ProgressWindowsClass.py
--rw-rw-rw-   0        0        0     2251 2023-05-18 09:28:54.000000 UEVaultManager-1.4.3/UEVaultManager/tkgui/modules/SaferDictClass.py
--rw-rw-rw-   0        0        0     6168 2023-05-23 07:32:20.000000 UEVaultManager-1.4.3/UEVaultManager/tkgui/modules/TaggedLabelFrameClass.py
--rw-rw-rw-   0        0        0    42713 2023-05-23 13:39:57.000000 UEVaultManager-1.4.3/UEVaultManager/tkgui/modules/UEVMGuiClass.py
--rw-rw-rw-   0        0        0      543 2023-05-16 16:57:06.000000 UEVaultManager-1.4.3/UEVaultManager/tkgui/modules/UEVMGuiHiddenRootClass.py
--rw-rw-rw-   0        0        0     2230 2023-05-15 10:13:54.000000 UEVaultManager-1.4.3/UEVaultManager/tkgui/modules/WebImageClass.py
--rw-rw-rw-   0        0        0       16 2023-05-14 16:44:57.000000 UEVaultManager-1.4.3/UEVaultManager/tkgui/modules/__init__.py
--rw-rw-rw-   0        0        0    14641 2023-05-23 13:35:44.000000 UEVaultManager-1.4.3/UEVaultManager/tkgui/modules/functions.py
--rw-rw-rw-   0        0        0     2631 2023-05-23 13:39:29.000000 UEVaultManager-1.4.3/UEVaultManager/tkgui/modules/globals.py
-drwxrwxrwx   0        0        0        0 2023-05-23 13:51:01.046076 UEVaultManager-1.4.3/UEVaultManager/utils/
--rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.4.3/UEVaultManager/utils/__init__.py
--rw-rw-rw-   0        0        0     3478 2023-05-17 13:38:36.000000 UEVaultManager-1.4.3/UEVaultManager/utils/aliasing.py
--rw-rw-rw-   0        0        0     5897 2023-05-18 09:32:02.000000 UEVaultManager-1.4.3/UEVaultManager/utils/cli.py
--rw-rw-rw-   0        0        0     1342 2023-05-15 06:55:20.000000 UEVaultManager-1.4.3/UEVaultManager/utils/custom_parser.py
--rw-rw-rw-   0        0        0    10286 2023-05-15 06:33:02.000000 UEVaultManager-1.4.3/UEVaultManager/utils/egl_crypt.py
--rw-rw-rw-   0        0        0      503 2023-05-15 10:15:48.000000 UEVaultManager-1.4.3/UEVaultManager/utils/env.py
--rw-rw-rw-   0        0        0      752 2023-05-15 06:58:00.000000 UEVaultManager-1.4.3/UEVaultManager/utils/rolling_hash.py
--rw-rw-rw-   0        0        0     7260 2023-05-17 13:34:09.000000 UEVaultManager-1.4.3/UEVaultManager/utils/webview_login.py
-drwxrwxrwx   0        0        0        0 2023-05-23 13:51:00.901492 UEVaultManager-1.4.3/UEVaultManager.egg-info/
--rw-rw-rw-   0        0        0     6129 2023-05-23 13:51:00.000000 UEVaultManager-1.4.3/UEVaultManager.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2295 2023-05-23 13:51:00.000000 UEVaultManager-1.4.3/UEVaultManager.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 13:51:00.000000 UEVaultManager-1.4.3/UEVaultManager.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-05-23 13:51:00.000000 UEVaultManager-1.4.3/UEVaultManager.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      286 2023-05-23 13:51:00.000000 UEVaultManager-1.4.3/UEVaultManager.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-23 13:51:00.000000 UEVaultManager-1.4.3/UEVaultManager.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-23 13:51:01.048076 UEVaultManager-1.4.3/setup.cfg
--rw-rw-rw-   0        0        0     3008 2023-05-23 12:39:50.000000 UEVaultManager-1.4.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-25 09:58:15.558558 UEVaultManager-1.5.0/
+-rw-rw-rw-   0        0        0    35823 2023-01-05 18:12:15.000000 UEVaultManager-1.5.0/LICENSE
+-rw-rw-rw-   0        0        0     6123 2023-05-25 09:58:15.557557 UEVaultManager-1.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5285 2023-05-23 13:48:41.000000 UEVaultManager-1.5.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-25 09:58:15.392405 UEVaultManager-1.5.0/UEVaultManager/
+-rw-rw-rw-   0        0        0      774 2023-05-25 09:54:50.000000 UEVaultManager-1.5.0/UEVaultManager/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 09:58:15.427765 UEVaultManager-1.5.0/UEVaultManager/api/
+-rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.5.0/UEVaultManager/api/__init__.py
+-rw-rw-rw-   0        0        0    25469 2023-05-18 09:30:29.000000 UEVaultManager-1.5.0/UEVaultManager/api/egs.py
+-rw-rw-rw-   0        0        0     3142 2023-05-17 13:34:09.000000 UEVaultManager-1.5.0/UEVaultManager/api/uevm.py
+drwxrwxrwx   0        0        0        0 2023-05-25 09:58:15.438898 UEVaultManager-1.5.0/UEVaultManager/assets/
+-rw-rw-rw-   0        0        0    20282 2023-05-11 14:38:28.000000 UEVaultManager-1.5.0/UEVaultManager/assets/UEVM_200x200.png
+-rw-rw-rw-   0        0        0      432 2023-05-21 17:27:34.000000 UEVaultManager-1.5.0/UEVaultManager/assets/checked_16.png
+-rw-rw-rw-   0        0        0     4286 2023-05-11 14:38:28.000000 UEVaultManager-1.5.0/UEVaultManager/assets/main.ico
+-rw-rw-rw-   0        0        0      187 2023-05-21 17:27:58.000000 UEVaultManager-1.5.0/UEVaultManager/assets/unchecked_16.png
+-rw-rw-rw-   0        0        0    72413 2023-05-25 07:55:46.000000 UEVaultManager-1.5.0/UEVaultManager/cli.py
+-rw-rw-rw-   0        0        0    47576 2023-05-25 07:55:46.000000 UEVaultManager-1.5.0/UEVaultManager/core.py
+drwxrwxrwx   0        0        0        0 2023-05-25 09:58:15.444897 UEVaultManager-1.5.0/UEVaultManager/downloader/
+-rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.5.0/UEVaultManager/downloader/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 09:58:15.458899 UEVaultManager-1.5.0/UEVaultManager/downloader/mp/
+-rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.5.0/UEVaultManager/downloader/mp/__init__.py
+-rw-rw-rw-   0        0        0    38030 2023-05-15 06:30:52.000000 UEVaultManager-1.5.0/UEVaultManager/downloader/mp/manager.py
+-rw-rw-rw-   0        0        0    12365 2023-05-17 13:38:36.000000 UEVaultManager-1.5.0/UEVaultManager/downloader/mp/workers.py
+drwxrwxrwx   0        0        0        0 2023-05-25 09:58:15.475898 UEVaultManager-1.5.0/UEVaultManager/lfs/
+-rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.5.0/UEVaultManager/lfs/__init__.py
+-rw-rw-rw-   0        0        0     3611 2023-05-11 14:38:28.000000 UEVaultManager-1.5.0/UEVaultManager/lfs/egl.py
+-rw-rw-rw-   0        0        0     6428 2023-05-15 06:51:22.000000 UEVaultManager-1.5.0/UEVaultManager/lfs/eos.py
+-rw-rw-rw-   0        0        0    23506 2023-05-25 07:24:32.000000 UEVaultManager-1.5.0/UEVaultManager/lfs/uevmlfs.py
+-rw-rw-rw-   0        0        0      593 2023-05-15 06:35:46.000000 UEVaultManager-1.5.0/UEVaultManager/lfs/utils.py
+-rw-rw-rw-   0        0        0     3122 2023-05-15 06:51:32.000000 UEVaultManager-1.5.0/UEVaultManager/lfs/windows_helpers.py
+drwxrwxrwx   0        0        0        0 2023-05-25 09:58:15.497841 UEVaultManager-1.5.0/UEVaultManager/models/
+-rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.5.0/UEVaultManager/models/__init__.py
+-rw-rw-rw-   0        0        0     4269 2023-05-17 13:38:36.000000 UEVaultManager-1.5.0/UEVaultManager/models/app.py
+-rw-rw-rw-   0        0        0     4478 2023-05-11 14:38:28.000000 UEVaultManager-1.5.0/UEVaultManager/models/chunk.py
+-rw-rw-rw-   0        0        0     2703 2023-05-20 09:18:48.000000 UEVaultManager-1.5.0/UEVaultManager/models/config.py
+-rw-rw-rw-   0        0        0     2133 2023-05-25 07:55:46.000000 UEVaultManager-1.5.0/UEVaultManager/models/csv.py
+-rw-rw-rw-   0        0        0     3627 2023-05-11 14:38:28.000000 UEVaultManager-1.5.0/UEVaultManager/models/downloading.py
+-rw-rw-rw-   0        0        0     5094 2023-05-15 06:33:02.000000 UEVaultManager-1.5.0/UEVaultManager/models/egl.py
+-rw-rw-rw-   0        0        0      256 2023-05-20 09:20:19.000000 UEVaultManager-1.5.0/UEVaultManager/models/exceptions.py
+-rw-rw-rw-   0        0        0     5893 2023-05-15 06:30:52.000000 UEVaultManager-1.5.0/UEVaultManager/models/json_manifest.py
+-rw-rw-rw-   0        0        0    30505 2023-05-17 13:38:36.000000 UEVaultManager-1.5.0/UEVaultManager/models/manifest.py
+drwxrwxrwx   0        0        0        0 2023-05-25 09:58:15.505843 UEVaultManager-1.5.0/UEVaultManager/tkgui/
+-rw-rw-rw-   0        0        0       16 2023-05-14 16:45:45.000000 UEVaultManager-1.5.0/UEVaultManager/tkgui/__init__.py
+-rw-rw-rw-   0        0        0     1622 2023-05-25 07:54:00.000000 UEVaultManager-1.5.0/UEVaultManager/tkgui/main.py
+drwxrwxrwx   0        0        0        0 2023-05-25 09:58:15.535939 UEVaultManager-1.5.0/UEVaultManager/tkgui/modules/
+-rw-rw-rw-   0        0        0     6667 2023-05-23 13:36:34.000000 UEVaultManager-1.5.0/UEVaultManager/tkgui/modules/DisplayContentWindowClass.py
+-rw-rw-rw-   0        0        0     4551 2023-05-25 07:55:46.000000 UEVaultManager-1.5.0/UEVaultManager/tkgui/modules/EditCellWindowClass.py
+-rw-rw-rw-   0        0        0     6542 2023-05-25 07:55:46.000000 UEVaultManager-1.5.0/UEVaultManager/tkgui/modules/EditRowWindowClass.py
+-rw-rw-rw-   0        0        0    33763 2023-05-25 09:25:25.000000 UEVaultManager-1.5.0/UEVaultManager/tkgui/modules/EditableTableClass.py
+-rw-rw-rw-   0        0        0    14038 2023-05-22 16:36:16.000000 UEVaultManager-1.5.0/UEVaultManager/tkgui/modules/ExtendedWidgetClasses.py
+-rw-rw-rw-   0        0        0     2562 2023-05-25 09:51:53.000000 UEVaultManager-1.5.0/UEVaultManager/tkgui/modules/GUISettingsClass.py
+-rw-rw-rw-   0        0        0    13936 2023-05-25 07:55:46.000000 UEVaultManager-1.5.0/UEVaultManager/tkgui/modules/ProgressWindowsClass.py
+-rw-rw-rw-   0        0        0     2251 2023-05-18 09:28:54.000000 UEVaultManager-1.5.0/UEVaultManager/tkgui/modules/SaferDictClass.py
+-rw-rw-rw-   0        0        0     6168 2023-05-23 07:32:20.000000 UEVaultManager-1.5.0/UEVaultManager/tkgui/modules/TaggedLabelFrameClass.py
+-rw-rw-rw-   0        0        0    42713 2023-05-23 13:39:57.000000 UEVaultManager-1.5.0/UEVaultManager/tkgui/modules/UEVMGuiClass.py
+-rw-rw-rw-   0        0        0      543 2023-05-16 16:57:06.000000 UEVaultManager-1.5.0/UEVaultManager/tkgui/modules/UEVMGuiHiddenRootClass.py
+-rw-rw-rw-   0        0        0     2230 2023-05-15 10:13:54.000000 UEVaultManager-1.5.0/UEVaultManager/tkgui/modules/WebImageClass.py
+-rw-rw-rw-   0        0        0       16 2023-05-14 16:44:57.000000 UEVaultManager-1.5.0/UEVaultManager/tkgui/modules/__init__.py
+-rw-rw-rw-   0        0        0    14911 2023-05-25 08:25:00.000000 UEVaultManager-1.5.0/UEVaultManager/tkgui/modules/functions.py
+-rw-rw-rw-   0        0        0     2631 2023-05-23 13:39:29.000000 UEVaultManager-1.5.0/UEVaultManager/tkgui/modules/globals.py
+drwxrwxrwx   0        0        0        0 2023-05-25 09:58:15.556561 UEVaultManager-1.5.0/UEVaultManager/utils/
+-rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.5.0/UEVaultManager/utils/__init__.py
+-rw-rw-rw-   0        0        0     3478 2023-05-17 13:38:36.000000 UEVaultManager-1.5.0/UEVaultManager/utils/aliasing.py
+-rw-rw-rw-   0        0        0     5897 2023-05-18 09:32:02.000000 UEVaultManager-1.5.0/UEVaultManager/utils/cli.py
+-rw-rw-rw-   0        0        0     1342 2023-05-15 06:55:20.000000 UEVaultManager-1.5.0/UEVaultManager/utils/custom_parser.py
+-rw-rw-rw-   0        0        0    10286 2023-05-15 06:33:02.000000 UEVaultManager-1.5.0/UEVaultManager/utils/egl_crypt.py
+-rw-rw-rw-   0        0        0      503 2023-05-15 10:15:48.000000 UEVaultManager-1.5.0/UEVaultManager/utils/env.py
+-rw-rw-rw-   0        0        0      752 2023-05-15 06:58:00.000000 UEVaultManager-1.5.0/UEVaultManager/utils/rolling_hash.py
+-rw-rw-rw-   0        0        0     7260 2023-05-17 13:34:09.000000 UEVaultManager-1.5.0/UEVaultManager/utils/webview_login.py
+drwxrwxrwx   0        0        0        0 2023-05-25 09:58:15.414917 UEVaultManager-1.5.0/UEVaultManager.egg-info/
+-rw-rw-rw-   0        0        0     6123 2023-05-25 09:58:15.000000 UEVaultManager-1.5.0/UEVaultManager.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2295 2023-05-25 09:58:15.000000 UEVaultManager-1.5.0/UEVaultManager.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 09:58:15.000000 UEVaultManager-1.5.0/UEVaultManager.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-05-25 09:58:15.000000 UEVaultManager-1.5.0/UEVaultManager.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      286 2023-05-25 09:58:15.000000 UEVaultManager-1.5.0/UEVaultManager.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-25 09:58:15.000000 UEVaultManager-1.5.0/UEVaultManager.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-25 09:58:15.558558 UEVaultManager-1.5.0/setup.cfg
+-rw-rw-rw-   0        0        0     3008 2023-05-23 12:39:50.000000 UEVaultManager-1.5.0/setup.py
```

### Comparing `UEVaultManager-1.4.3/LICENSE` & `UEVaultManager-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.3/PKG-INFO` & `UEVaultManager-1.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UEVaultManager
-Version: 1.4.3
+Version: 1.5.0
 Summary: Free and open-source replacement for the Epic Games Launcher application, mainly to manage the assets for Unreal Engine
 Home-page: https://github.com/LaurentOngaro/UEVaultManager
 Author: Laurent Ongaro
 Author-email: laurent@gameamea.com
 License: GPL-3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.9
@@ -63,8 +63,8 @@
 * [Configuration](https://uevaultmanager.readthedocs.io/en/latest/configuration.html)
   * [Config folder](https://uevaultmanager.readthedocs.io/en/latest/configuration.html#config-folder)
   * [Config file](https://uevaultmanager.readthedocs.io/en/latest/configuration.html#config-file)
 
 [More info](https://uevaultmanager.readthedocs.io/en/latest/intro.html "UEVaultManager")
 
 
- UEVaultManager ## version:1.4.3 ## codename: Phoenix+3
+ UEVaultManager ## version:1.5.0 ## codename: Leo
```

### Comparing `UEVaultManager-1.4.3/README.md` & `UEVaultManager-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.3/UEVaultManager/__init__.py` & `UEVaultManager-1.5.0/UEVaultManager/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 UEVaultManager setup file.
 """
 import datetime
 
 year = datetime.date.today().year
 
 __name__ = 'UEVaultManager'
-__version__ = '1.4.3'
+__version__ = '1.5.0'
 # 0 Pegasus Seiya
 # 1 Dragon Shiryu
 # 2 Cygnus Hyoga
 # 3 Andromeda Shun
 # 4 Phoenix Ikki
-__codename__ = 'Phoenix+3'
 # 5 Leo Aiolia
+__codename__ = 'Leo'
 # 5 Virgo Shaka
 # 6 Libra Dohko
 # 7 Scorpio Milo
 # 8 Sagittarius Aiolos
 # 9 Capricorn Shura
 # 10 Aquarius Camus
 # 11 Pisces Aphrodite
```

### Comparing `UEVaultManager-1.4.3/UEVaultManager/api/egs.py` & `UEVaultManager-1.5.0/UEVaultManager/api/egs.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.3/UEVaultManager/api/uevm.py` & `UEVaultManager-1.5.0/UEVaultManager/api/uevm.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.3/UEVaultManager/assets/UEVM_200x200.png` & `UEVaultManager-1.5.0/UEVaultManager/assets/UEVM_200x200.png`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.3/UEVaultManager/assets/main.ico` & `UEVaultManager-1.5.0/UEVaultManager/assets/main.ico`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.3/UEVaultManager/cli.py` & `UEVaultManager-1.5.0/UEVaultManager/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,23 +24,24 @@
 # noinspection PyPep8Naming
 from UEVaultManager import __version__ as UEVM_version, __codename__ as UEVM_codename
 from UEVaultManager.api.egs import create_empty_assets_extras, GrabResult
 from UEVaultManager.api.uevm import UpdateSeverity
 from UEVaultManager.core import AppCore
 from UEVaultManager.models.csv import CSV_headings
 from UEVaultManager.models.exceptions import InvalidCredentialsError
+from UEVaultManager.tkgui.main import init_gui
+from UEVaultManager.tkgui.modules.DisplayContentWindowClass import DisplayContentWindow
 from UEVaultManager.tkgui.modules.functions import custom_print  # simplier way to use the custom_print function
 from UEVaultManager.tkgui.modules.functions import json_print_key_val
 from UEVaultManager.tkgui.modules.ProgressWindowsClass import ProgressWindow
+from UEVaultManager.tkgui.modules.SaferDictClass import SaferDict
 from UEVaultManager.tkgui.modules.UEVMGuiClass import UEVMGui
+from UEVaultManager.tkgui.modules.UEVMGuiHiddenRootClass import UEVMGuiHiddenRoot
 from UEVaultManager.utils.cli import str_to_bool, check_and_create_path, create_list_from_string, str_is_bool
 from UEVaultManager.utils.custom_parser import HiddenAliasSubparsersAction
-from UEVaultManager.tkgui.modules.DisplayContentWindowClass import DisplayContentWindow
-from UEVaultManager.tkgui.modules.SaferDictClass import SaferDict
-from UEVaultManager.tkgui.modules.UEVMGuiHiddenRootClass import UEVMGuiHiddenRoot
 
 logging.basicConfig(format='[%(name)s] %(levelname)s: %(message)s', level=logging.INFO)
 
 
 def init_gui_args(args, additional_args=None) -> None:
     """
     Initialize the GUI arguments using the CLI arguments
@@ -1164,15 +1165,17 @@
                     continue
                 custom_print(text=f'\nCommand: {choice}')
                 custom_print(text=subparser.format_help())
         elif os.name == 'nt':
             from UEVaultManager.lfs.windows_helpers import double_clicked
             if double_clicked():
                 custom_print(text='Please note that this is not the intended way to run UEVaultManager.')
-                custom_print(text='Follow https://github.com/LaurentOngaro/UEVaultManager#readme to set it up properly')
+                custom_print(text='If you want to start it without arguments, you can start it in edit mode by default.')
+                custom_print(text='For that, you must set the line start_in_edit_mode=true in the configuration file.')
+                custom_print(text='More info on usage and configuration can be found in https://github.com/LaurentOngaro/UEVaultManager#readme')
                 subprocess.Popen(['cmd', '/K', 'echo>nul'])
         custom_print(keep_mode=False)  # as it, next print will not keep the content
 
         if args.gui and not uewm_gui_exists:
             gui_g.UEVM_gui_ref.mainloop()
 
 
@@ -1349,14 +1352,22 @@
     args, extra = parser.parse_known_args()
 
     if args.version:
         print(f'UEVaultManager version "{UEVM_version}", codename "{UEVM_codename}"')
         exit(0)
 
     cli = UEVaultManagerCLI(override_config=args.config_file, api_timeout=args.api_timeout)
+
+    start_in_edit_mode = str_to_bool(cli.core.uevmlfs.config.get('UEVaultManager', 'start_in_edit_mode', fallback=False))
+    if start_in_edit_mode:
+        args.subparser_name = 'edit'
+        args.input = cli.core.uevmlfs.config.get('UEVaultManager', 'edit_file', fallback=None)
+        args.gui = True
+        args.input = init_gui(False)
+
     if not args.subparser_name or args.full_help:
         cli.print_help(args=args, parser=parser)
         return
 
     ql = cli.setup_threaded_logging()
 
     conf_log_level = cli.core.uevmlfs.config.get('UEVaultManager', 'log_level', fallback='info')
```

### Comparing `UEVaultManager-1.4.3/UEVaultManager/core.py` & `UEVaultManager-1.5.0/UEVaultManager/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 from UEVaultManager.models.json_manifest import JSONManifest
 from UEVaultManager.models.manifest import Manifest
 from UEVaultManager.tkgui.modules.functions import box_message
 from UEVaultManager.utils.cli import check_and_create_path
 from UEVaultManager.utils.egl_crypt import decrypt_epic_data
 from UEVaultManager.utils.env import is_windows_mac_or_pyi
 
+
 # The heading dict contains the title of each column and a boolean value to know if its contents must be preserved if it already exists in the output file (To Avoid overwriting data changed by the user in the file)
 
 # ToDo: instead of true/false return values for success/failure actually raise an exception that the CLI/GUI
 #  can handle to give the user more details. (Not required yet since there's no GUI so log output is fine)
 
 
 class AppCore:
```

### Comparing `UEVaultManager-1.4.3/UEVaultManager/downloader/mp/manager.py` & `UEVaultManager-1.5.0/UEVaultManager/downloader/mp/manager.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.3/UEVaultManager/downloader/mp/workers.py` & `UEVaultManager-1.5.0/UEVaultManager/downloader/mp/workers.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.3/UEVaultManager/lfs/egl.py` & `UEVaultManager-1.5.0/UEVaultManager/lfs/egl.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.3/UEVaultManager/lfs/eos.py` & `UEVaultManager-1.5.0/UEVaultManager/lfs/eos.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.3/UEVaultManager/lfs/uevmlfs.py` & `UEVaultManager-1.5.0/UEVaultManager/lfs/uevmlfs.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,14 +110,18 @@
         # make sure "UEVaultManager" section exists
         has_changed = False
         if 'UEVaultManager' not in self.config:
             self.config.add_section('UEVaultManager')
             has_changed = True
 
         # Add opt-out options with explainers
+        if not self.config.has_option('UEVaultManager', 'start_in_edit_mode'):
+            self.config.set('UEVaultManager', '; start the App in Edit mode (since v1.4.4) with the GUI')
+            self.config.set('UEVaultManager', 'start_in_edit_mode', 'false')
+            has_changed = True
         if not self.config.has_option('UEVaultManager', 'disable_update_check'):
             self.config.set('UEVaultManager', '; Disables the automatic update check')
             self.config.set('UEVaultManager', 'disable_update_check', 'false')
             has_changed = True
         if not self.config.has_option('UEVaultManager', 'disable_update_notice'):
             self.config.set('UEVaultManager', '; Disables the notice about an available update on exit')
             self.config.set('UEVaultManager', 'disable_update_notice', 'false' if is_windows_mac_or_pyi() else 'true')
```

### Comparing `UEVaultManager-1.4.3/UEVaultManager/lfs/utils.py` & `UEVaultManager-1.5.0/UEVaultManager/lfs/utils.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.3/UEVaultManager/lfs/windows_helpers.py` & `UEVaultManager-1.5.0/UEVaultManager/lfs/windows_helpers.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.3/UEVaultManager/models/app.py` & `UEVaultManager-1.5.0/UEVaultManager/models/app.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.3/UEVaultManager/models/chunk.py` & `UEVaultManager-1.5.0/UEVaultManager/models/chunk.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.3/UEVaultManager/models/config.py` & `UEVaultManager-1.5.0/UEVaultManager/models/config.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.3/UEVaultManager/models/csv.py` & `UEVaultManager-1.5.0/UEVaultManager/models/csv.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # coding=utf-8
 """
 Implementation for:
 - CSV_headings: contains the title of each column and a boolean value to know if its contents must be preserved if it already exists in the output file (To Avoid overwriting data changed by the user in the file)
 """
 import uuid
+
 import UEVaultManager.tkgui.modules.globals as gui_g  # using the shortest variable name for globals for convenience
 
 CSV_headings = {
     'Asset_id': False,  # ! important: Do not Rename => this field is used as main key for each asset
     'App name': False,
     'App title': False,
     'Category': False,
```

### Comparing `UEVaultManager-1.4.3/UEVaultManager/models/downloading.py` & `UEVaultManager-1.5.0/UEVaultManager/models/downloading.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.3/UEVaultManager/models/egl.py` & `UEVaultManager-1.5.0/UEVaultManager/models/egl.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.3/UEVaultManager/models/json_manifest.py` & `UEVaultManager-1.5.0/UEVaultManager/models/json_manifest.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.3/UEVaultManager/models/manifest.py` & `UEVaultManager-1.5.0/UEVaultManager/models/manifest.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.3/UEVaultManager/tkgui/modules/DisplayContentWindowClass.py` & `UEVaultManager-1.5.0/UEVaultManager/tkgui/modules/DisplayContentWindowClass.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.3/UEVaultManager/tkgui/modules/EditCellWindowClass.py` & `UEVaultManager-1.5.0/UEVaultManager/tkgui/modules/EditCellWindowClass.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # coding=utf-8
 """
 Implementation for:
 - EditCellWindow: the window to edit a cell
 """
-import os
 import tkinter as tk
 from tkinter import ttk
 
 from ttkbootstrap.constants import *
 
 import UEVaultManager.tkgui.modules.functions as gui_f  # using the shortest variable name for globals for convenience
 import UEVaultManager.tkgui.modules.globals as gui_g  # using the shortest variable name for globals for convenience
```

### Comparing `UEVaultManager-1.4.3/UEVaultManager/tkgui/modules/EditRowWindowClass.py` & `UEVaultManager-1.5.0/UEVaultManager/tkgui/modules/EditRowWindowClass.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # coding=utf-8
 """
 Implementation for:
 - EditRowWindow: the window to edit a row
 """
-import os
 import tkinter as tk
 from tkinter import ttk
 
 from ttkbootstrap.constants import *
 
 import UEVaultManager.tkgui.modules.functions as gui_f  # using the shortest variable name for globals for convenience
 import UEVaultManager.tkgui.modules.globals as gui_g  # using the shortest variable name for globals for convenience
```

### Comparing `UEVaultManager-1.4.3/UEVaultManager/tkgui/modules/EditableTableClass.py` & `UEVaultManager-1.5.0/UEVaultManager/tkgui/modules/EditableTableClass.py`

 * *Files 2% similar despite different names*

```diff
@@ -155,15 +155,18 @@
             for i in range(min(self.rows_per_page, len(mask))):
                 try:
                     if str(mask[i]) == value_to_check:
                         row_indices.append(i)
                 except KeyError:
                     log_debug(f'KeyError for row {i} in color_rows_if')
             if len(row_indices) > 0:  # Check if there are any row indices
-                self.setRowColors(rows=row_indices, clr=color, cols='all')
+                try:
+                    self.setRowColors(rows=row_indices, clr=color, cols='all')
+                except KeyError:
+                    log_debug(f'KeyError for row in color_rows_if')
             return
 
     def set_preferences(self, default_pref=None) -> None:
         """
         Initializes the table preferences.
         :param default_pref: The default preferences to apply to the table.
         """
@@ -171,14 +174,39 @@
         # when sorting the table with pagination enabled
         # see: https://stackoverflow.com/questions/20625582/how-to-deal-with-settingwithcopywarning-in-pandas
         pd.options.mode.chained_assignment = None
 
         if default_pref is not None:
             config.apply_options(default_pref, self)
 
+    def colorRows(self):
+        """
+        Color individual cells in column(s). Requires that the rowcolors
+        dataframe has been set. This needs to be updated if the index is reset
+        Override this method to check indexes when rebuildind data from en empty table
+        """
+        df = self.model.df
+        rc = self.rowcolors
+        rows = self.visiblerows
+        offset = rows[0]
+        idx = df.index[rows]
+
+        for col in self.visiblecols:
+            colname = df.columns[col]
+            if colname in list(rc.columns):
+                try:
+                    colors = rc[colname].loc[idx]
+                except KeyError:
+                    colors = None
+                if colors is not None:
+                    for row in rows:
+                        clr = colors.iloc[row - offset]
+                        if not pd.isnull(clr):
+                            self.drawRect(row, col, color=clr, tag='colorrect', delete=0)
+
     def set_colors(self) -> None:
         """
         Initializes the colors of some cells depending on their values.
         """
         if not gui_g.s.use_colors_for_data:
             self.redraw()
             return
@@ -211,27 +239,31 @@
         """
         Displays the specified page of the table data.
         :param page: The page number to display (zero-based index).
         """
         if page is None:
             page = self.current_page
         if self.pagination_enabled:
+            self.total_pages = min(self.total_pages, len(self.data))
             if page < 0:
                 page = 0
             elif page >= self.total_pages:
                 page = self.total_pages - 1
             # Calculate start and end rows for current page
             self.current_page = page
             start = page * self.rows_per_page
             end = start + self.rows_per_page
+            start = min(start, len(self.data))
+            end = min(end, len(self.data))
             try:
                 # Update table with data for current page
                 self.model.df = self.data.iloc[start:end]
             except AttributeError:
                 # self.redraw()
+                log_debug(f'AttributeError in show_page')
                 self.set_colors()
                 return
         else:
             # Update table with all data
             self.model.df = self.data_filtered
             self.current_page = 0
         # self.redraw()
@@ -364,15 +396,15 @@
         if gui_g.UEVM_cli_ref is None or 'UEVaultManagerCLI' not in str(type(gui_g.UEVM_cli_ref)):
             from_cli_only_message()
             return False
         else:
             gui_g.UEVM_cli_ref.list_assets(gui_g.UEVM_cli_args)
             self.current_page = 0
             self.load_data()
-            self.show_page(self.current_page)
+            self.show_page(0)
             return True
 
     def save_data(self) -> None:
         """
         Saves the current table data to the CSV file.
         """
```

### Comparing `UEVaultManager-1.4.3/UEVaultManager/tkgui/modules/ExtendedWidgetClasses.py` & `UEVaultManager-1.5.0/UEVaultManager/tkgui/modules/ExtendedWidgetClasses.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.3/UEVaultManager/tkgui/modules/GUISettingsClass.py` & `UEVaultManager-1.5.0/UEVaultManager/tkgui/modules/GUISettingsClass.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.3/UEVaultManager/tkgui/modules/ProgressWindowsClass.py` & `UEVaultManager-1.5.0/UEVaultManager/tkgui/modules/ProgressWindowsClass.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # coding=utf-8
 """
 Implementation for:
 - ProgressWindow: window to display the progress of a function
 """
-import os
 import queue
 import threading
 import tkinter as tk
 from tkinter import ttk
 
 import UEVaultManager.tkgui.modules.functions as gui_f  # using the shortest variable name for globals for convenience
 import UEVaultManager.tkgui.modules.globals as gui_g  # using the shortest variable name for globals for convenience
```

### Comparing `UEVaultManager-1.4.3/UEVaultManager/tkgui/modules/SaferDictClass.py` & `UEVaultManager-1.5.0/UEVaultManager/tkgui/modules/SaferDictClass.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.3/UEVaultManager/tkgui/modules/TaggedLabelFrameClass.py` & `UEVaultManager-1.5.0/UEVaultManager/tkgui/modules/TaggedLabelFrameClass.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.3/UEVaultManager/tkgui/modules/UEVMGuiClass.py` & `UEVaultManager-1.5.0/UEVaultManager/tkgui/modules/UEVMGuiClass.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.3/UEVaultManager/tkgui/modules/UEVMGuiHiddenRootClass.py` & `UEVaultManager-1.5.0/UEVaultManager/tkgui/modules/UEVMGuiHiddenRootClass.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.3/UEVaultManager/tkgui/modules/WebImageClass.py` & `UEVaultManager-1.5.0/UEVaultManager/tkgui/modules/WebImageClass.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.3/UEVaultManager/tkgui/modules/functions.py` & `UEVaultManager-1.5.0/UEVaultManager/tkgui/modules/functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 # coding=utf-8
 """
 Utilities functions and tools
 """
+import ctypes as ct
 import datetime
+import logging
 import os
 import time
 import tkinter as tk
 from io import BytesIO
 from tkinter import messagebox
 
-import ctypes as ct
 import requests
 import ttkbootstrap as ttk
 from PIL import ImageTk, Image
 from screeninfo import get_monitors
 from termcolor import colored
 
 from UEVaultManager.tkgui.modules import globals as gui_g
@@ -104,15 +105,20 @@
     """
     Log a debug message. Note that this message will only be logged if the debug mode is enabled
     :param msg: the message to log
     """
     if not gui_g.s.debug_mode:
         return
     if gui_g.UEVM_log_ref is not None:
-        gui_g.UEVM_log_ref.debug(msg)
+        # ensure that the debug messages will be logged even if the log level not set to DEBUG in the cli
+        log_level = gui_g.UEVM_log_ref.level
+        if log_level == logging.DEBUG:
+            gui_g.UEVM_log_ref.debug(msg)
+        else:
+            gui_g.UEVM_log_ref.info(msg)
     else:
         msg = log_format_message(gui_g.s.app_title, 'Debug', colored(msg, 'light_grey'))
         print(msg)
 
 
 def log_warning(msg: str) -> None:
     """
```

### Comparing `UEVaultManager-1.4.3/UEVaultManager/tkgui/modules/globals.py` & `UEVaultManager-1.5.0/UEVaultManager/tkgui/modules/globals.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.3/UEVaultManager/utils/aliasing.py` & `UEVaultManager-1.5.0/UEVaultManager/utils/aliasing.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.3/UEVaultManager/utils/cli.py` & `UEVaultManager-1.5.0/UEVaultManager/utils/cli.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.3/UEVaultManager/utils/custom_parser.py` & `UEVaultManager-1.5.0/UEVaultManager/utils/custom_parser.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.3/UEVaultManager/utils/egl_crypt.py` & `UEVaultManager-1.5.0/UEVaultManager/utils/egl_crypt.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.3/UEVaultManager/utils/rolling_hash.py` & `UEVaultManager-1.5.0/UEVaultManager/utils/rolling_hash.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.3/UEVaultManager/utils/webview_login.py` & `UEVaultManager-1.5.0/UEVaultManager/utils/webview_login.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.3/UEVaultManager.egg-info/PKG-INFO` & `UEVaultManager-1.5.0/UEVaultManager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UEVaultManager
-Version: 1.4.3
+Version: 1.5.0
 Summary: Free and open-source replacement for the Epic Games Launcher application, mainly to manage the assets for Unreal Engine
 Home-page: https://github.com/LaurentOngaro/UEVaultManager
 Author: Laurent Ongaro
 Author-email: laurent@gameamea.com
 License: GPL-3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.9
@@ -63,8 +63,8 @@
 * [Configuration](https://uevaultmanager.readthedocs.io/en/latest/configuration.html)
   * [Config folder](https://uevaultmanager.readthedocs.io/en/latest/configuration.html#config-folder)
   * [Config file](https://uevaultmanager.readthedocs.io/en/latest/configuration.html#config-file)
 
 [More info](https://uevaultmanager.readthedocs.io/en/latest/intro.html "UEVaultManager")
 
 
- UEVaultManager ## version:1.4.3 ## codename: Phoenix+3
+ UEVaultManager ## version:1.5.0 ## codename: Leo
```

### Comparing `UEVaultManager-1.4.3/UEVaultManager.egg-info/SOURCES.txt` & `UEVaultManager-1.5.0/UEVaultManager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.4.3/setup.py` & `UEVaultManager-1.5.0/setup.py`

 * *Files identical despite different names*

