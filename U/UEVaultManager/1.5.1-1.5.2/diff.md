# Comparing `tmp/UEVaultManager-1.5.1.tar.gz` & `tmp/UEVaultManager-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UEVaultManager-1.5.1.tar", last modified: Thu May 25 10:10:16 2023, max compression
+gzip compressed data, was "UEVaultManager-1.5.2.tar", last modified: Thu May 25 10:16:32 2023, max compression
```

## Comparing `UEVaultManager-1.5.1.tar` & `UEVaultManager-1.5.2.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 10:10:16.405048 UEVaultManager-1.5.1/
--rw-rw-rw-   0        0        0    35823 2023-01-05 18:12:15.000000 UEVaultManager-1.5.1/LICENSE
--rw-rw-rw-   0        0        0     6125 2023-05-25 10:10:16.404047 UEVaultManager-1.5.1/PKG-INFO
--rw-rw-rw-   0        0        0     5285 2023-05-23 13:48:41.000000 UEVaultManager-1.5.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-25 10:10:16.238111 UEVaultManager-1.5.1/UEVaultManager/
--rw-rw-rw-   0        0        0      776 2023-05-25 10:08:13.000000 UEVaultManager-1.5.1/UEVaultManager/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 10:10:16.272492 UEVaultManager-1.5.1/UEVaultManager/api/
--rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.5.1/UEVaultManager/api/__init__.py
--rw-rw-rw-   0        0        0    25469 2023-05-18 09:30:29.000000 UEVaultManager-1.5.1/UEVaultManager/api/egs.py
--rw-rw-rw-   0        0        0     3142 2023-05-17 13:34:09.000000 UEVaultManager-1.5.1/UEVaultManager/api/uevm.py
-drwxrwxrwx   0        0        0        0 2023-05-25 10:10:16.283492 UEVaultManager-1.5.1/UEVaultManager/assets/
--rw-rw-rw-   0        0        0    20282 2023-05-11 14:38:28.000000 UEVaultManager-1.5.1/UEVaultManager/assets/UEVM_200x200.png
--rw-rw-rw-   0        0        0      432 2023-05-21 17:27:34.000000 UEVaultManager-1.5.1/UEVaultManager/assets/checked_16.png
--rw-rw-rw-   0        0        0     4286 2023-05-11 14:38:28.000000 UEVaultManager-1.5.1/UEVaultManager/assets/main.ico
--rw-rw-rw-   0        0        0      187 2023-05-21 17:27:58.000000 UEVaultManager-1.5.1/UEVaultManager/assets/unchecked_16.png
--rw-rw-rw-   0        0        0    72475 2023-05-25 10:05:55.000000 UEVaultManager-1.5.1/UEVaultManager/cli.py
--rw-rw-rw-   0        0        0    47576 2023-05-25 07:55:46.000000 UEVaultManager-1.5.1/UEVaultManager/core.py
-drwxrwxrwx   0        0        0        0 2023-05-25 10:10:16.289041 UEVaultManager-1.5.1/UEVaultManager/downloader/
--rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.5.1/UEVaultManager/downloader/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 10:10:16.302503 UEVaultManager-1.5.1/UEVaultManager/downloader/mp/
--rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.5.1/UEVaultManager/downloader/mp/__init__.py
--rw-rw-rw-   0        0        0    38030 2023-05-15 06:30:52.000000 UEVaultManager-1.5.1/UEVaultManager/downloader/mp/manager.py
--rw-rw-rw-   0        0        0    12365 2023-05-17 13:38:36.000000 UEVaultManager-1.5.1/UEVaultManager/downloader/mp/workers.py
-drwxrwxrwx   0        0        0        0 2023-05-25 10:10:16.319896 UEVaultManager-1.5.1/UEVaultManager/lfs/
--rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.5.1/UEVaultManager/lfs/__init__.py
--rw-rw-rw-   0        0        0     3611 2023-05-11 14:38:28.000000 UEVaultManager-1.5.1/UEVaultManager/lfs/egl.py
--rw-rw-rw-   0        0        0     6428 2023-05-15 06:51:22.000000 UEVaultManager-1.5.1/UEVaultManager/lfs/eos.py
--rw-rw-rw-   0        0        0    23506 2023-05-25 07:24:32.000000 UEVaultManager-1.5.1/UEVaultManager/lfs/uevmlfs.py
--rw-rw-rw-   0        0        0      593 2023-05-15 06:35:46.000000 UEVaultManager-1.5.1/UEVaultManager/lfs/utils.py
--rw-rw-rw-   0        0        0     3122 2023-05-15 06:51:32.000000 UEVaultManager-1.5.1/UEVaultManager/lfs/windows_helpers.py
-drwxrwxrwx   0        0        0        0 2023-05-25 10:10:16.344050 UEVaultManager-1.5.1/UEVaultManager/models/
--rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.5.1/UEVaultManager/models/__init__.py
--rw-rw-rw-   0        0        0     4269 2023-05-17 13:38:36.000000 UEVaultManager-1.5.1/UEVaultManager/models/app.py
--rw-rw-rw-   0        0        0     4478 2023-05-11 14:38:28.000000 UEVaultManager-1.5.1/UEVaultManager/models/chunk.py
--rw-rw-rw-   0        0        0     2703 2023-05-20 09:18:48.000000 UEVaultManager-1.5.1/UEVaultManager/models/config.py
--rw-rw-rw-   0        0        0     2133 2023-05-25 07:55:46.000000 UEVaultManager-1.5.1/UEVaultManager/models/csv.py
--rw-rw-rw-   0        0        0     3627 2023-05-11 14:38:28.000000 UEVaultManager-1.5.1/UEVaultManager/models/downloading.py
--rw-rw-rw-   0        0        0     5094 2023-05-15 06:33:02.000000 UEVaultManager-1.5.1/UEVaultManager/models/egl.py
--rw-rw-rw-   0        0        0      256 2023-05-20 09:20:19.000000 UEVaultManager-1.5.1/UEVaultManager/models/exceptions.py
--rw-rw-rw-   0        0        0     5893 2023-05-15 06:30:52.000000 UEVaultManager-1.5.1/UEVaultManager/models/json_manifest.py
--rw-rw-rw-   0        0        0    30505 2023-05-17 13:38:36.000000 UEVaultManager-1.5.1/UEVaultManager/models/manifest.py
-drwxrwxrwx   0        0        0        0 2023-05-25 10:10:16.351046 UEVaultManager-1.5.1/UEVaultManager/tkgui/
--rw-rw-rw-   0        0        0       16 2023-05-14 16:45:45.000000 UEVaultManager-1.5.1/UEVaultManager/tkgui/__init__.py
--rw-rw-rw-   0        0        0     1622 2023-05-25 07:54:00.000000 UEVaultManager-1.5.1/UEVaultManager/tkgui/main.py
-drwxrwxrwx   0        0        0        0 2023-05-25 10:10:16.383046 UEVaultManager-1.5.1/UEVaultManager/tkgui/modules/
--rw-rw-rw-   0        0        0     6667 2023-05-23 13:36:34.000000 UEVaultManager-1.5.1/UEVaultManager/tkgui/modules/DisplayContentWindowClass.py
--rw-rw-rw-   0        0        0     4551 2023-05-25 07:55:46.000000 UEVaultManager-1.5.1/UEVaultManager/tkgui/modules/EditCellWindowClass.py
--rw-rw-rw-   0        0        0     6542 2023-05-25 07:55:46.000000 UEVaultManager-1.5.1/UEVaultManager/tkgui/modules/EditRowWindowClass.py
--rw-rw-rw-   0        0        0    33763 2023-05-25 09:25:25.000000 UEVaultManager-1.5.1/UEVaultManager/tkgui/modules/EditableTableClass.py
--rw-rw-rw-   0        0        0    14038 2023-05-22 16:36:16.000000 UEVaultManager-1.5.1/UEVaultManager/tkgui/modules/ExtendedWidgetClasses.py
--rw-rw-rw-   0        0        0     2562 2023-05-25 09:51:53.000000 UEVaultManager-1.5.1/UEVaultManager/tkgui/modules/GUISettingsClass.py
--rw-rw-rw-   0        0        0    13936 2023-05-25 07:55:46.000000 UEVaultManager-1.5.1/UEVaultManager/tkgui/modules/ProgressWindowsClass.py
--rw-rw-rw-   0        0        0     2251 2023-05-18 09:28:54.000000 UEVaultManager-1.5.1/UEVaultManager/tkgui/modules/SaferDictClass.py
--rw-rw-rw-   0        0        0     6168 2023-05-23 07:32:20.000000 UEVaultManager-1.5.1/UEVaultManager/tkgui/modules/TaggedLabelFrameClass.py
--rw-rw-rw-   0        0        0    42713 2023-05-23 13:39:57.000000 UEVaultManager-1.5.1/UEVaultManager/tkgui/modules/UEVMGuiClass.py
--rw-rw-rw-   0        0        0      543 2023-05-16 16:57:06.000000 UEVaultManager-1.5.1/UEVaultManager/tkgui/modules/UEVMGuiHiddenRootClass.py
--rw-rw-rw-   0        0        0     2230 2023-05-15 10:13:54.000000 UEVaultManager-1.5.1/UEVaultManager/tkgui/modules/WebImageClass.py
--rw-rw-rw-   0        0        0       16 2023-05-14 16:44:57.000000 UEVaultManager-1.5.1/UEVaultManager/tkgui/modules/__init__.py
--rw-rw-rw-   0        0        0    14911 2023-05-25 08:25:00.000000 UEVaultManager-1.5.1/UEVaultManager/tkgui/modules/functions.py
--rw-rw-rw-   0        0        0     2631 2023-05-23 13:39:29.000000 UEVaultManager-1.5.1/UEVaultManager/tkgui/modules/globals.py
-drwxrwxrwx   0        0        0        0 2023-05-25 10:10:16.403046 UEVaultManager-1.5.1/UEVaultManager/utils/
--rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.5.1/UEVaultManager/utils/__init__.py
--rw-rw-rw-   0        0        0     3478 2023-05-17 13:38:36.000000 UEVaultManager-1.5.1/UEVaultManager/utils/aliasing.py
--rw-rw-rw-   0        0        0     5897 2023-05-18 09:32:02.000000 UEVaultManager-1.5.1/UEVaultManager/utils/cli.py
--rw-rw-rw-   0        0        0     1342 2023-05-15 06:55:20.000000 UEVaultManager-1.5.1/UEVaultManager/utils/custom_parser.py
--rw-rw-rw-   0        0        0    10286 2023-05-15 06:33:02.000000 UEVaultManager-1.5.1/UEVaultManager/utils/egl_crypt.py
--rw-rw-rw-   0        0        0      503 2023-05-15 10:15:48.000000 UEVaultManager-1.5.1/UEVaultManager/utils/env.py
--rw-rw-rw-   0        0        0      752 2023-05-15 06:58:00.000000 UEVaultManager-1.5.1/UEVaultManager/utils/rolling_hash.py
--rw-rw-rw-   0        0        0     7260 2023-05-17 13:34:09.000000 UEVaultManager-1.5.1/UEVaultManager/utils/webview_login.py
-drwxrwxrwx   0        0        0        0 2023-05-25 10:10:16.259455 UEVaultManager-1.5.1/UEVaultManager.egg-info/
--rw-rw-rw-   0        0        0     6125 2023-05-25 10:10:16.000000 UEVaultManager-1.5.1/UEVaultManager.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2295 2023-05-25 10:10:16.000000 UEVaultManager-1.5.1/UEVaultManager.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 10:10:16.000000 UEVaultManager-1.5.1/UEVaultManager.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-05-25 10:10:16.000000 UEVaultManager-1.5.1/UEVaultManager.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      286 2023-05-25 10:10:16.000000 UEVaultManager-1.5.1/UEVaultManager.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-25 10:10:16.000000 UEVaultManager-1.5.1/UEVaultManager.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-25 10:10:16.405048 UEVaultManager-1.5.1/setup.cfg
--rw-rw-rw-   0        0        0     3008 2023-05-23 12:39:50.000000 UEVaultManager-1.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-25 10:16:32.443056 UEVaultManager-1.5.2/
+-rw-rw-rw-   0        0        0    35823 2023-01-05 18:12:15.000000 UEVaultManager-1.5.2/LICENSE
+-rw-rw-rw-   0        0        0     6125 2023-05-25 10:16:32.443056 UEVaultManager-1.5.2/PKG-INFO
+-rw-rw-rw-   0        0        0     5285 2023-05-23 13:48:41.000000 UEVaultManager-1.5.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-25 10:16:32.274194 UEVaultManager-1.5.2/UEVaultManager/
+-rw-rw-rw-   0        0        0      776 2023-05-25 10:15:06.000000 UEVaultManager-1.5.2/UEVaultManager/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 10:16:32.311191 UEVaultManager-1.5.2/UEVaultManager/api/
+-rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.5.2/UEVaultManager/api/__init__.py
+-rw-rw-rw-   0        0        0    25469 2023-05-18 09:30:29.000000 UEVaultManager-1.5.2/UEVaultManager/api/egs.py
+-rw-rw-rw-   0        0        0     3142 2023-05-17 13:34:09.000000 UEVaultManager-1.5.2/UEVaultManager/api/uevm.py
+drwxrwxrwx   0        0        0        0 2023-05-25 10:16:32.323705 UEVaultManager-1.5.2/UEVaultManager/assets/
+-rw-rw-rw-   0        0        0    20282 2023-05-11 14:38:28.000000 UEVaultManager-1.5.2/UEVaultManager/assets/UEVM_200x200.png
+-rw-rw-rw-   0        0        0      432 2023-05-21 17:27:34.000000 UEVaultManager-1.5.2/UEVaultManager/assets/checked_16.png
+-rw-rw-rw-   0        0        0     4286 2023-05-11 14:38:28.000000 UEVaultManager-1.5.2/UEVaultManager/assets/main.ico
+-rw-rw-rw-   0        0        0      187 2023-05-21 17:27:58.000000 UEVaultManager-1.5.2/UEVaultManager/assets/unchecked_16.png
+-rw-rw-rw-   0        0        0    72499 2023-05-25 10:13:03.000000 UEVaultManager-1.5.2/UEVaultManager/cli.py
+-rw-rw-rw-   0        0        0    47576 2023-05-25 07:55:46.000000 UEVaultManager-1.5.2/UEVaultManager/core.py
+drwxrwxrwx   0        0        0        0 2023-05-25 10:16:32.331241 UEVaultManager-1.5.2/UEVaultManager/downloader/
+-rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.5.2/UEVaultManager/downloader/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 10:16:32.344239 UEVaultManager-1.5.2/UEVaultManager/downloader/mp/
+-rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.5.2/UEVaultManager/downloader/mp/__init__.py
+-rw-rw-rw-   0        0        0    38030 2023-05-15 06:30:52.000000 UEVaultManager-1.5.2/UEVaultManager/downloader/mp/manager.py
+-rw-rw-rw-   0        0        0    12365 2023-05-17 13:38:36.000000 UEVaultManager-1.5.2/UEVaultManager/downloader/mp/workers.py
+drwxrwxrwx   0        0        0        0 2023-05-25 10:16:32.361383 UEVaultManager-1.5.2/UEVaultManager/lfs/
+-rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.5.2/UEVaultManager/lfs/__init__.py
+-rw-rw-rw-   0        0        0     3611 2023-05-11 14:38:28.000000 UEVaultManager-1.5.2/UEVaultManager/lfs/egl.py
+-rw-rw-rw-   0        0        0     6428 2023-05-15 06:51:22.000000 UEVaultManager-1.5.2/UEVaultManager/lfs/eos.py
+-rw-rw-rw-   0        0        0    23506 2023-05-25 07:24:32.000000 UEVaultManager-1.5.2/UEVaultManager/lfs/uevmlfs.py
+-rw-rw-rw-   0        0        0      593 2023-05-15 06:35:46.000000 UEVaultManager-1.5.2/UEVaultManager/lfs/utils.py
+-rw-rw-rw-   0        0        0     3122 2023-05-15 06:51:32.000000 UEVaultManager-1.5.2/UEVaultManager/lfs/windows_helpers.py
+drwxrwxrwx   0        0        0        0 2023-05-25 10:16:32.385850 UEVaultManager-1.5.2/UEVaultManager/models/
+-rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.5.2/UEVaultManager/models/__init__.py
+-rw-rw-rw-   0        0        0     4269 2023-05-17 13:38:36.000000 UEVaultManager-1.5.2/UEVaultManager/models/app.py
+-rw-rw-rw-   0        0        0     4478 2023-05-11 14:38:28.000000 UEVaultManager-1.5.2/UEVaultManager/models/chunk.py
+-rw-rw-rw-   0        0        0     2703 2023-05-20 09:18:48.000000 UEVaultManager-1.5.2/UEVaultManager/models/config.py
+-rw-rw-rw-   0        0        0     2133 2023-05-25 07:55:46.000000 UEVaultManager-1.5.2/UEVaultManager/models/csv.py
+-rw-rw-rw-   0        0        0     3627 2023-05-11 14:38:28.000000 UEVaultManager-1.5.2/UEVaultManager/models/downloading.py
+-rw-rw-rw-   0        0        0     5094 2023-05-15 06:33:02.000000 UEVaultManager-1.5.2/UEVaultManager/models/egl.py
+-rw-rw-rw-   0        0        0      256 2023-05-20 09:20:19.000000 UEVaultManager-1.5.2/UEVaultManager/models/exceptions.py
+-rw-rw-rw-   0        0        0     5893 2023-05-15 06:30:52.000000 UEVaultManager-1.5.2/UEVaultManager/models/json_manifest.py
+-rw-rw-rw-   0        0        0    30505 2023-05-17 13:38:36.000000 UEVaultManager-1.5.2/UEVaultManager/models/manifest.py
+drwxrwxrwx   0        0        0        0 2023-05-25 10:16:32.392852 UEVaultManager-1.5.2/UEVaultManager/tkgui/
+-rw-rw-rw-   0        0        0       16 2023-05-14 16:45:45.000000 UEVaultManager-1.5.2/UEVaultManager/tkgui/__init__.py
+-rw-rw-rw-   0        0        0     1622 2023-05-25 07:54:00.000000 UEVaultManager-1.5.2/UEVaultManager/tkgui/main.py
+drwxrwxrwx   0        0        0        0 2023-05-25 10:16:32.421319 UEVaultManager-1.5.2/UEVaultManager/tkgui/modules/
+-rw-rw-rw-   0        0        0     6667 2023-05-23 13:36:34.000000 UEVaultManager-1.5.2/UEVaultManager/tkgui/modules/DisplayContentWindowClass.py
+-rw-rw-rw-   0        0        0     4551 2023-05-25 07:55:46.000000 UEVaultManager-1.5.2/UEVaultManager/tkgui/modules/EditCellWindowClass.py
+-rw-rw-rw-   0        0        0     6542 2023-05-25 07:55:46.000000 UEVaultManager-1.5.2/UEVaultManager/tkgui/modules/EditRowWindowClass.py
+-rw-rw-rw-   0        0        0    33763 2023-05-25 09:25:25.000000 UEVaultManager-1.5.2/UEVaultManager/tkgui/modules/EditableTableClass.py
+-rw-rw-rw-   0        0        0    14038 2023-05-22 16:36:16.000000 UEVaultManager-1.5.2/UEVaultManager/tkgui/modules/ExtendedWidgetClasses.py
+-rw-rw-rw-   0        0        0     2562 2023-05-25 09:51:53.000000 UEVaultManager-1.5.2/UEVaultManager/tkgui/modules/GUISettingsClass.py
+-rw-rw-rw-   0        0        0    13936 2023-05-25 07:55:46.000000 UEVaultManager-1.5.2/UEVaultManager/tkgui/modules/ProgressWindowsClass.py
+-rw-rw-rw-   0        0        0     2251 2023-05-18 09:28:54.000000 UEVaultManager-1.5.2/UEVaultManager/tkgui/modules/SaferDictClass.py
+-rw-rw-rw-   0        0        0     6168 2023-05-23 07:32:20.000000 UEVaultManager-1.5.2/UEVaultManager/tkgui/modules/TaggedLabelFrameClass.py
+-rw-rw-rw-   0        0        0    42713 2023-05-23 13:39:57.000000 UEVaultManager-1.5.2/UEVaultManager/tkgui/modules/UEVMGuiClass.py
+-rw-rw-rw-   0        0        0      543 2023-05-16 16:57:06.000000 UEVaultManager-1.5.2/UEVaultManager/tkgui/modules/UEVMGuiHiddenRootClass.py
+-rw-rw-rw-   0        0        0     2230 2023-05-15 10:13:54.000000 UEVaultManager-1.5.2/UEVaultManager/tkgui/modules/WebImageClass.py
+-rw-rw-rw-   0        0        0       16 2023-05-14 16:44:57.000000 UEVaultManager-1.5.2/UEVaultManager/tkgui/modules/__init__.py
+-rw-rw-rw-   0        0        0    14911 2023-05-25 08:25:00.000000 UEVaultManager-1.5.2/UEVaultManager/tkgui/modules/functions.py
+-rw-rw-rw-   0        0        0     2631 2023-05-23 13:39:29.000000 UEVaultManager-1.5.2/UEVaultManager/tkgui/modules/globals.py
+drwxrwxrwx   0        0        0        0 2023-05-25 10:16:32.441057 UEVaultManager-1.5.2/UEVaultManager/utils/
+-rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.5.2/UEVaultManager/utils/__init__.py
+-rw-rw-rw-   0        0        0     3478 2023-05-17 13:38:36.000000 UEVaultManager-1.5.2/UEVaultManager/utils/aliasing.py
+-rw-rw-rw-   0        0        0     5897 2023-05-18 09:32:02.000000 UEVaultManager-1.5.2/UEVaultManager/utils/cli.py
+-rw-rw-rw-   0        0        0     1342 2023-05-15 06:55:20.000000 UEVaultManager-1.5.2/UEVaultManager/utils/custom_parser.py
+-rw-rw-rw-   0        0        0    10286 2023-05-15 06:33:02.000000 UEVaultManager-1.5.2/UEVaultManager/utils/egl_crypt.py
+-rw-rw-rw-   0        0        0      503 2023-05-15 10:15:48.000000 UEVaultManager-1.5.2/UEVaultManager/utils/env.py
+-rw-rw-rw-   0        0        0      752 2023-05-15 06:58:00.000000 UEVaultManager-1.5.2/UEVaultManager/utils/rolling_hash.py
+-rw-rw-rw-   0        0        0     7260 2023-05-17 13:34:09.000000 UEVaultManager-1.5.2/UEVaultManager/utils/webview_login.py
+drwxrwxrwx   0        0        0        0 2023-05-25 10:16:32.298106 UEVaultManager-1.5.2/UEVaultManager.egg-info/
+-rw-rw-rw-   0        0        0     6125 2023-05-25 10:16:32.000000 UEVaultManager-1.5.2/UEVaultManager.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2295 2023-05-25 10:16:32.000000 UEVaultManager-1.5.2/UEVaultManager.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 10:16:32.000000 UEVaultManager-1.5.2/UEVaultManager.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-05-25 10:16:32.000000 UEVaultManager-1.5.2/UEVaultManager.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      286 2023-05-25 10:16:32.000000 UEVaultManager-1.5.2/UEVaultManager.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-25 10:16:32.000000 UEVaultManager-1.5.2/UEVaultManager.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-25 10:16:32.443056 UEVaultManager-1.5.2/setup.cfg
+-rw-rw-rw-   0        0        0     3008 2023-05-23 12:39:50.000000 UEVaultManager-1.5.2/setup.py
```

### Comparing `UEVaultManager-1.5.1/LICENSE` & `UEVaultManager-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.5.1/PKG-INFO` & `UEVaultManager-1.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UEVaultManager
-Version: 1.5.1
+Version: 1.5.2
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
 
 
- UEVaultManager ## version:1.5.1 ## codename: Leo+1
+ UEVaultManager ## version:1.5.2 ## codename: Leo+2
```

### Comparing `UEVaultManager-1.5.1/README.md` & `UEVaultManager-1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.5.1/UEVaultManager/__init__.py` & `UEVaultManager-1.5.2/UEVaultManager/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 UEVaultManager setup file.
 """
 import datetime
 
 year = datetime.date.today().year
 
 __name__ = 'UEVaultManager'
-__version__ = '1.5.1'
+__version__ = '1.5.2'
 # 0 Pegasus Seiya
 # 1 Dragon Shiryu
 # 2 Cygnus Hyoga
 # 3 Andromeda Shun
 # 4 Phoenix Ikki
 # 5 Leo Aiolia
-__codename__ = 'Leo+1'
+__codename__ = 'Leo+2'
 # 5 Virgo Shaka
 # 6 Libra Dohko
 # 7 Scorpio Milo
 # 8 Sagittarius Aiolos
 # 9 Capricorn Shura
 # 10 Aquarius Camus
 # 11 Pisces Aphrodite
```

### Comparing `UEVaultManager-1.5.1/UEVaultManager/api/egs.py` & `UEVaultManager-1.5.2/UEVaultManager/api/egs.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.5.1/UEVaultManager/api/uevm.py` & `UEVaultManager-1.5.2/UEVaultManager/api/uevm.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.5.1/UEVaultManager/assets/UEVM_200x200.png` & `UEVaultManager-1.5.2/UEVaultManager/assets/UEVM_200x200.png`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.5.1/UEVaultManager/assets/main.ico` & `UEVaultManager-1.5.2/UEVaultManager/assets/main.ico`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.5.1/UEVaultManager/cli.py` & `UEVaultManager-1.5.2/UEVaultManager/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -1411,24 +1411,23 @@
             cli.info(args)
         elif args.subparser_name == 'cleanup':
             cli.cleanup(args)
         elif args.subparser_name == 'get-token':
             cli.get_token(args)
         elif args.subparser_name in {'edit', 'edit-assets'}:
             cli.edit_assets(args)
+        elif start_in_edit_mode:
+            args.subparser_name = 'edit'
+            args.input = cli.core.uevmlfs.config.get('UEVaultManager', 'edit_file', fallback=None)
+            args.gui = True
+            args.input = init_gui(False)
+            cli.edit_assets(args)
     except KeyboardInterrupt:
         cli.logger.info('Command was aborted via KeyboardInterrupt, cleaning up...')
 
-    if start_in_edit_mode:
-        args.subparser_name = 'edit'
-        args.input = cli.core.uevmlfs.config.get('UEVaultManager', 'edit_file', fallback=None)
-        args.gui = True
-        args.input = init_gui(False)
-        cli.edit_assets(args)
-
     # Disable the update message if JSON/TSV/CSV outputs are used
     disable_update_message = False
     if hasattr(args, 'json'):
         disable_update_message = args.json
     if not disable_update_message and hasattr(args, 'tsv'):
         disable_update_message = args.tsv
     if not disable_update_message and hasattr(args, 'csv'):
```

### Comparing `UEVaultManager-1.5.1/UEVaultManager/core.py` & `UEVaultManager-1.5.2/UEVaultManager/core.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.5.1/UEVaultManager/downloader/mp/manager.py` & `UEVaultManager-1.5.2/UEVaultManager/downloader/mp/manager.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.5.1/UEVaultManager/downloader/mp/workers.py` & `UEVaultManager-1.5.2/UEVaultManager/downloader/mp/workers.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.5.1/UEVaultManager/lfs/egl.py` & `UEVaultManager-1.5.2/UEVaultManager/lfs/egl.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.5.1/UEVaultManager/lfs/eos.py` & `UEVaultManager-1.5.2/UEVaultManager/lfs/eos.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.5.1/UEVaultManager/lfs/uevmlfs.py` & `UEVaultManager-1.5.2/UEVaultManager/lfs/uevmlfs.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.5.1/UEVaultManager/lfs/utils.py` & `UEVaultManager-1.5.2/UEVaultManager/lfs/utils.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.5.1/UEVaultManager/lfs/windows_helpers.py` & `UEVaultManager-1.5.2/UEVaultManager/lfs/windows_helpers.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.5.1/UEVaultManager/models/app.py` & `UEVaultManager-1.5.2/UEVaultManager/models/app.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.5.1/UEVaultManager/models/chunk.py` & `UEVaultManager-1.5.2/UEVaultManager/models/chunk.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.5.1/UEVaultManager/models/config.py` & `UEVaultManager-1.5.2/UEVaultManager/models/config.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.5.1/UEVaultManager/models/csv.py` & `UEVaultManager-1.5.2/UEVaultManager/models/csv.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.5.1/UEVaultManager/models/downloading.py` & `UEVaultManager-1.5.2/UEVaultManager/models/downloading.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.5.1/UEVaultManager/models/egl.py` & `UEVaultManager-1.5.2/UEVaultManager/models/egl.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.5.1/UEVaultManager/models/json_manifest.py` & `UEVaultManager-1.5.2/UEVaultManager/models/json_manifest.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.5.1/UEVaultManager/models/manifest.py` & `UEVaultManager-1.5.2/UEVaultManager/models/manifest.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.5.1/UEVaultManager/tkgui/main.py` & `UEVaultManager-1.5.2/UEVaultManager/tkgui/main.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.5.1/UEVaultManager/tkgui/modules/DisplayContentWindowClass.py` & `UEVaultManager-1.5.2/UEVaultManager/tkgui/modules/DisplayContentWindowClass.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.5.1/UEVaultManager/tkgui/modules/EditCellWindowClass.py` & `UEVaultManager-1.5.2/UEVaultManager/tkgui/modules/EditCellWindowClass.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.5.1/UEVaultManager/tkgui/modules/EditRowWindowClass.py` & `UEVaultManager-1.5.2/UEVaultManager/tkgui/modules/EditRowWindowClass.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.5.1/UEVaultManager/tkgui/modules/EditableTableClass.py` & `UEVaultManager-1.5.2/UEVaultManager/tkgui/modules/EditableTableClass.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.5.1/UEVaultManager/tkgui/modules/ExtendedWidgetClasses.py` & `UEVaultManager-1.5.2/UEVaultManager/tkgui/modules/ExtendedWidgetClasses.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.5.1/UEVaultManager/tkgui/modules/GUISettingsClass.py` & `UEVaultManager-1.5.2/UEVaultManager/tkgui/modules/GUISettingsClass.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.5.1/UEVaultManager/tkgui/modules/ProgressWindowsClass.py` & `UEVaultManager-1.5.2/UEVaultManager/tkgui/modules/ProgressWindowsClass.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.5.1/UEVaultManager/tkgui/modules/SaferDictClass.py` & `UEVaultManager-1.5.2/UEVaultManager/tkgui/modules/SaferDictClass.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.5.1/UEVaultManager/tkgui/modules/TaggedLabelFrameClass.py` & `UEVaultManager-1.5.2/UEVaultManager/tkgui/modules/TaggedLabelFrameClass.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.5.1/UEVaultManager/tkgui/modules/UEVMGuiClass.py` & `UEVaultManager-1.5.2/UEVaultManager/tkgui/modules/UEVMGuiClass.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.5.1/UEVaultManager/tkgui/modules/UEVMGuiHiddenRootClass.py` & `UEVaultManager-1.5.2/UEVaultManager/tkgui/modules/UEVMGuiHiddenRootClass.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.5.1/UEVaultManager/tkgui/modules/WebImageClass.py` & `UEVaultManager-1.5.2/UEVaultManager/tkgui/modules/WebImageClass.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.5.1/UEVaultManager/tkgui/modules/functions.py` & `UEVaultManager-1.5.2/UEVaultManager/tkgui/modules/functions.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.5.1/UEVaultManager/tkgui/modules/globals.py` & `UEVaultManager-1.5.2/UEVaultManager/tkgui/modules/globals.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.5.1/UEVaultManager/utils/aliasing.py` & `UEVaultManager-1.5.2/UEVaultManager/utils/aliasing.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.5.1/UEVaultManager/utils/cli.py` & `UEVaultManager-1.5.2/UEVaultManager/utils/cli.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.5.1/UEVaultManager/utils/custom_parser.py` & `UEVaultManager-1.5.2/UEVaultManager/utils/custom_parser.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.5.1/UEVaultManager/utils/egl_crypt.py` & `UEVaultManager-1.5.2/UEVaultManager/utils/egl_crypt.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.5.1/UEVaultManager/utils/rolling_hash.py` & `UEVaultManager-1.5.2/UEVaultManager/utils/rolling_hash.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.5.1/UEVaultManager/utils/webview_login.py` & `UEVaultManager-1.5.2/UEVaultManager/utils/webview_login.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.5.1/UEVaultManager.egg-info/PKG-INFO` & `UEVaultManager-1.5.2/UEVaultManager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UEVaultManager
-Version: 1.5.1
+Version: 1.5.2
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
 
 
- UEVaultManager ## version:1.5.1 ## codename: Leo+1
+ UEVaultManager ## version:1.5.2 ## codename: Leo+2
```

### Comparing `UEVaultManager-1.5.1/UEVaultManager.egg-info/SOURCES.txt` & `UEVaultManager-1.5.2/UEVaultManager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.5.1/setup.py` & `UEVaultManager-1.5.2/setup.py`

 * *Files identical despite different names*

