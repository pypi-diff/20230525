# Comparing `tmp/msg_explorer-1.6.0.tar.gz` & `tmp/msg_explorer-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msg_explorer-1.6.0.tar", last modified: Mon Mar 20 19:31:17 2023, max compression
+gzip compressed data, was "msg_explorer-1.7.0.tar", last modified: Thu May 25 01:11:39 2023, max compression
```

## Comparing `msg_explorer-1.6.0.tar` & `msg_explorer-1.7.0.tar`

### file list

```diff
@@ -1,75 +1,60 @@
-drwxrwxrwx   0        0        0        0 2023-03-20 19:31:17.063742 msg_explorer-1.6.0/
--rw-rw-rw-   0        0        0     3109 2023-03-20 19:29:46.000000 msg_explorer-1.6.0/CHANGELOG.md
--rw-rw-rw-   0        0        0    35821 2021-10-31 23:47:15.000000 msg_explorer-1.6.0/LICENSE.txt
--rw-rw-rw-   0        0        0      174 2022-06-01 19:20:28.000000 msg_explorer-1.6.0/MANIFEST.in
--rw-rw-rw-   0        0        0     3244 2023-03-20 19:31:17.064740 msg_explorer-1.6.0/PKG-INFO
--rw-rw-rw-   0        0        0     2547 2023-03-20 19:29:46.000000 msg_explorer-1.6.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-03-20 19:31:16.028288 msg_explorer-1.6.0/msg_explorer/
--rw-rw-rw-   0        0        0     1300 2023-03-20 19:29:46.000000 msg_explorer-1.6.0/msg_explorer/__init__.py
--rw-rw-rw-   0        0        0      131 2023-03-20 19:29:46.000000 msg_explorer-1.6.0/msg_explorer/__main__.py
--rw-rw-rw-   0        0        0     1587 2022-05-27 22:32:15.000000 msg_explorer-1.6.0/msg_explorer/_recompile.py
--rw-rw-rw-   0        0        0    93622 2022-06-12 23:42:53.000000 msg_explorer-1.6.0/msg_explorer/app_icons.py
--rw-rw-rw-   0        0        0      106 2022-06-12 23:41:51.000000 msg_explorer-1.6.0/msg_explorer/app_icons.qrc
--rw-rw-rw-   0        0        0     4425 2022-07-04 23:37:56.000000 msg_explorer-1.6.0/msg_explorer/attachments_browser.py
--rw-rw-rw-   0        0        0      635 2022-06-19 00:30:31.000000 msg_explorer-1.6.0/msg_explorer/constants.py
--rw-rw-rw-   0        0        0     1351 2022-05-30 07:47:18.000000 msg_explorer-1.6.0/msg_explorer/font_handler.py
--rw-rw-rw-   0        0        0      557 2022-06-01 01:48:04.000000 msg_explorer-1.6.0/msg_explorer/guid_viewer.py
--rw-rw-rw-   0        0        0     3574 2022-07-13 14:22:26.000000 msg_explorer-1.6.0/msg_explorer/hex_viewer.py
-drwxrwxrwx   0        0        0        0 2023-03-20 19:31:16.043397 msg_explorer-1.6.0/msg_explorer/icon/
--rw-rw-rw-   0        0        0    11156 2022-06-22 00:10:00.000000 msg_explorer-1.6.0/msg_explorer/icon/envelope_1024.png
--rw-rw-rw-   0        0        0      535 2022-06-01 05:33:36.000000 msg_explorer-1.6.0/msg_explorer/logger.py
--rw-rw-rw-   0        0        0      857 2022-06-01 05:29:14.000000 msg_explorer-1.6.0/msg_explorer/logger_widget.py
--rw-rw-rw-   0        0        0      565 2022-06-12 23:41:21.000000 msg_explorer-1.6.0/msg_explorer/main.py
--rw-rw-rw-   0        0        0    10187 2022-12-03 08:56:40.000000 msg_explorer-1.6.0/msg_explorer/main_window.py
--rw-rw-rw-   0        0        0     1511 2022-06-08 22:03:10.000000 msg_explorer-1.6.0/msg_explorer/msg_details_page.py
--rw-rw-rw-   0        0        0     4307 2022-06-19 00:36:02.000000 msg_explorer-1.6.0/msg_explorer/msg_tree_viewer.py
--rw-rw-rw-   0        0        0     1492 2022-06-01 05:08:40.000000 msg_explorer-1.6.0/msg_explorer/multiple_binary_viewer.py
--rw-rw-rw-   0        0        0     1579 2022-06-24 06:12:10.000000 msg_explorer-1.6.0/msg_explorer/multiple_viewer.py
--rw-rw-rw-   0        0        0     5649 2022-07-08 09:14:39.000000 msg_explorer-1.6.0/msg_explorer/named_properties_viewer.py
--rw-rw-rw-   0        0        0     1500 2022-06-11 06:10:16.000000 msg_explorer-1.6.0/msg_explorer/properties_viewer.py
--rw-rw-rw-   0        0        0        0 2023-03-20 19:29:46.000000 msg_explorer-1.6.0/msg_explorer/py.typed
--rw-rw-rw-   0        0        0     6965 2023-03-20 19:29:46.000000 msg_explorer-1.6.0/msg_explorer/stream_viewer.py
--rw-rw-rw-   0        0        0      843 2022-06-08 21:58:34.000000 msg_explorer-1.6.0/msg_explorer/string_viewer.py
-drwxrwxrwx   0        0        0        0 2023-03-20 19:31:17.062742 msg_explorer-1.6.0/msg_explorer/ui/
--rw-rw-rw-   0        0        0        0 2022-05-27 22:32:15.000000 msg_explorer-1.6.0/msg_explorer/ui/__init__.py
--rw-rw-rw-   0        0        0     2039 2022-07-05 01:05:44.000000 msg_explorer-1.6.0/msg_explorer/ui/attachments_browser.ui
--rw-rw-rw-   0        0        0      743 2022-06-01 02:06:32.000000 msg_explorer-1.6.0/msg_explorer/ui/guid_viewer.ui
--rw-rw-rw-   0        0        0      972 2022-06-18 23:50:41.000000 msg_explorer-1.6.0/msg_explorer/ui/hex_viewer.ui
--rw-rw-rw-   0        0        0     1133 2022-05-30 06:17:08.000000 msg_explorer-1.6.0/msg_explorer/ui/loading_screen.ui
--rw-rw-rw-   0        0        0      817 2022-07-05 00:54:55.000000 msg_explorer-1.6.0/msg_explorer/ui/logger_widget.ui
--rw-rw-rw-   0        0        0     4671 2022-12-03 08:46:09.000000 msg_explorer-1.6.0/msg_explorer/ui/main_window.ui
--rw-rw-rw-   0        0        0     3655 2022-06-01 02:06:33.000000 msg_explorer-1.6.0/msg_explorer/ui/msg_details_page.ui
--rw-rw-rw-   0        0        0     1280 2022-07-05 01:05:17.000000 msg_explorer-1.6.0/msg_explorer/ui/msg_tree_viewer.ui
--rw-rw-rw-   0        0        0     1701 2022-06-01 02:06:32.000000 msg_explorer-1.6.0/msg_explorer/ui/multiple_binary_viewer.ui
--rw-rw-rw-   0        0        0     1616 2022-07-05 01:05:33.000000 msg_explorer-1.6.0/msg_explorer/ui/multiple_viewer.ui
--rw-rw-rw-   0        0        0     1718 2022-07-08 09:14:44.000000 msg_explorer-1.6.0/msg_explorer/ui/named_properties_viewer.ui
--rw-rw-rw-   0        0        0     1583 2022-07-05 01:07:21.000000 msg_explorer-1.6.0/msg_explorer/ui/properties_viewer.ui
--rw-rw-rw-   0        0        0     4741 2022-06-01 02:06:33.000000 msg_explorer-1.6.0/msg_explorer/ui/stream_viewer.ui
--rw-rw-rw-   0        0        0      933 2022-06-01 03:00:39.000000 msg_explorer-1.6.0/msg_explorer/ui/string_viewer.ui
--rw-rw-rw-   0        0        0     4585 2022-07-05 03:20:35.000000 msg_explorer-1.6.0/msg_explorer/ui/ui_attachments_browser.py
--rw-rw-rw-   0        0        0     1750 2022-06-01 02:06:33.000000 msg_explorer-1.6.0/msg_explorer/ui/ui_guid_viewer.py
--rw-rw-rw-   0        0        0     1877 2022-06-18 23:51:26.000000 msg_explorer-1.6.0/msg_explorer/ui/ui_hex_viewer.py
--rw-rw-rw-   0        0        0     2186 2022-05-30 06:40:28.000000 msg_explorer-1.6.0/msg_explorer/ui/ui_loading_screen.py
--rw-rw-rw-   0        0        0     1829 2022-07-05 00:54:58.000000 msg_explorer-1.6.0/msg_explorer/ui/ui_logger_widget.py
--rw-rw-rw-   0        0        0     6959 2022-12-03 08:46:17.000000 msg_explorer-1.6.0/msg_explorer/ui/ui_main_window.py
--rw-rw-rw-   0        0        0     5510 2022-06-01 02:06:34.000000 msg_explorer-1.6.0/msg_explorer/ui/ui_msg_details_page.py
--rw-rw-rw-   0        0        0     2232 2022-07-05 03:20:35.000000 msg_explorer-1.6.0/msg_explorer/ui/ui_msg_tree_viewer.py
--rw-rw-rw-   0        0        0     2898 2022-06-01 02:06:34.000000 msg_explorer-1.6.0/msg_explorer/ui/ui_multiple_binary_viewer.py
--rw-rw-rw-   0        0        0     2711 2022-07-05 03:20:35.000000 msg_explorer-1.6.0/msg_explorer/ui/ui_multiple_viewer.py
--rw-rw-rw-   0        0        0     3931 2022-07-08 09:14:49.000000 msg_explorer-1.6.0/msg_explorer/ui/ui_named_properties_viewer.py
--rw-rw-rw-   0        0        0     3194 2022-07-05 03:20:35.000000 msg_explorer-1.6.0/msg_explorer/ui/ui_properties_viewer.py
--rw-rw-rw-   0        0        0     5782 2022-06-01 02:06:34.000000 msg_explorer-1.6.0/msg_explorer/ui/ui_stream_viewer.py
--rw-rw-rw-   0        0        0     1976 2022-06-01 03:09:36.000000 msg_explorer-1.6.0/msg_explorer/ui/ui_string_viewer.py
--rw-rw-rw-   0        0        0     2259 2022-06-01 02:06:34.000000 msg_explorer-1.6.0/msg_explorer/ui/ui_unhandled_exception.py
--rw-rw-rw-   0        0        0     1172 2022-06-01 02:06:32.000000 msg_explorer-1.6.0/msg_explorer/ui/unhandled_exception.ui
--rw-rw-rw-   0        0        0     1134 2022-06-01 02:46:16.000000 msg_explorer-1.6.0/msg_explorer/utils.py
-drwxrwxrwx   0        0        0        0 2023-03-20 19:31:16.041400 msg_explorer-1.6.0/msg_explorer.egg-info/
--rw-rw-rw-   0        0        0     3244 2023-03-20 19:31:09.000000 msg_explorer-1.6.0/msg_explorer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2164 2023-03-20 19:31:09.000000 msg_explorer-1.6.0/msg_explorer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-20 19:31:09.000000 msg_explorer-1.6.0/msg_explorer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2023-03-20 19:31:09.000000 msg_explorer-1.6.0/msg_explorer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       46 2023-03-20 19:31:09.000000 msg_explorer-1.6.0/msg_explorer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-03-20 19:31:09.000000 msg_explorer-1.6.0/msg_explorer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       78 2023-03-20 19:29:46.000000 msg_explorer-1.6.0/requirements.txt
--rw-rw-rw-   0        0        0       74 2023-03-20 19:31:17.066734 msg_explorer-1.6.0/setup.cfg
--rw-rw-rw-   0        0        0     1867 2023-03-20 19:29:46.000000 msg_explorer-1.6.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-25 01:11:39.100165 msg_explorer-1.7.0/
+-rw-rw-rw-   0        0        0     3131 2023-05-25 01:10:58.000000 msg_explorer-1.7.0/CHANGELOG.md
+-rw-rw-rw-   0        0        0    35147 2023-05-25 01:10:58.000000 msg_explorer-1.7.0/LICENSE.txt
+-rw-rw-rw-   0        0        0      167 2023-05-25 01:10:58.000000 msg_explorer-1.7.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     3221 2023-05-25 01:11:39.100165 msg_explorer-1.7.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2453 2023-05-25 01:10:58.000000 msg_explorer-1.7.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-25 01:11:39.060848 msg_explorer-1.7.0/msg_explorer/
+-rw-rw-rw-   0        0        0     1262 2023-05-25 01:10:58.000000 msg_explorer-1.7.0/msg_explorer/__init__.py
+-rw-rw-rw-   0        0        0      123 2023-05-25 01:10:58.000000 msg_explorer-1.7.0/msg_explorer/__main__.py
+-rw-rw-rw-   0        0        0     1545 2023-05-25 01:10:58.000000 msg_explorer-1.7.0/msg_explorer/_recompile.py
+-rw-rw-rw-   0        0        0    91838 2023-05-25 01:10:58.000000 msg_explorer-1.7.0/msg_explorer/app_icons.py
+-rw-rw-rw-   0        0        0      101 2023-05-25 01:10:58.000000 msg_explorer-1.7.0/msg_explorer/app_icons.qrc
+-rw-rw-rw-   0        0        0     4335 2023-05-25 01:10:58.000000 msg_explorer-1.7.0/msg_explorer/attachments_browser.py
+-rw-rw-rw-   0        0        0      621 2023-05-25 01:10:58.000000 msg_explorer-1.7.0/msg_explorer/constants.py
+-rw-rw-rw-   0        0        0     1301 2023-05-25 01:10:58.000000 msg_explorer-1.7.0/msg_explorer/font_handler.py
+-rw-rw-rw-   0        0        0      535 2023-05-25 01:10:58.000000 msg_explorer-1.7.0/msg_explorer/guid_viewer.py
+-rw-rw-rw-   0        0        0     3507 2023-05-25 01:10:58.000000 msg_explorer-1.7.0/msg_explorer/hex_viewer.py
+drwxrwxrwx   0        0        0        0 2023-05-25 01:11:39.075808 msg_explorer-1.7.0/msg_explorer/icon/
+-rw-rw-rw-   0        0        0    11156 2023-05-25 01:10:58.000000 msg_explorer-1.7.0/msg_explorer/icon/envelope_1024.png
+-rw-rw-rw-   0        0        0      516 2023-05-25 01:10:58.000000 msg_explorer-1.7.0/msg_explorer/logger.py
+-rw-rw-rw-   0        0        0      826 2023-05-25 01:10:58.000000 msg_explorer-1.7.0/msg_explorer/logger_widget.py
+-rw-rw-rw-   0        0        0      542 2023-05-25 01:10:58.000000 msg_explorer-1.7.0/msg_explorer/main.py
+-rw-rw-rw-   0        0        0     9939 2023-05-25 01:10:58.000000 msg_explorer-1.7.0/msg_explorer/main_window.py
+-rw-rw-rw-   0        0        0     1471 2023-05-25 01:10:58.000000 msg_explorer-1.7.0/msg_explorer/msg_details_page.py
+-rw-rw-rw-   0        0        0     4184 2023-05-25 01:10:58.000000 msg_explorer-1.7.0/msg_explorer/msg_tree_viewer.py
+-rw-rw-rw-   0        0        0     1446 2023-05-25 01:10:58.000000 msg_explorer-1.7.0/msg_explorer/multiple_binary_viewer.py
+-rw-rw-rw-   0        0        0     1526 2023-05-25 01:10:58.000000 msg_explorer-1.7.0/msg_explorer/multiple_viewer.py
+-rw-rw-rw-   0        0        0     5520 2023-05-25 01:10:58.000000 msg_explorer-1.7.0/msg_explorer/named_properties_viewer.py
+-rw-rw-rw-   0        0        0     1445 2023-05-25 01:10:58.000000 msg_explorer-1.7.0/msg_explorer/properties_viewer.py
+-rw-rw-rw-   0        0        0        0 2023-05-25 01:10:58.000000 msg_explorer-1.7.0/msg_explorer/py.typed
+-rw-rw-rw-   0        0        0     6799 2023-05-25 01:10:58.000000 msg_explorer-1.7.0/msg_explorer/stream_viewer.py
+-rw-rw-rw-   0        0        0      815 2023-05-25 01:10:58.000000 msg_explorer-1.7.0/msg_explorer/string_viewer.py
+drwxrwxrwx   0        0        0        0 2023-05-25 01:11:39.098172 msg_explorer-1.7.0/msg_explorer/ui/
+-rw-rw-rw-   0        0        0        0 2023-05-25 01:10:58.000000 msg_explorer-1.7.0/msg_explorer/ui/__init__.py
+-rw-rw-rw-   0        0        0     1961 2023-05-25 01:10:58.000000 msg_explorer-1.7.0/msg_explorer/ui/attachments_browser.ui
+-rw-rw-rw-   0        0        0      712 2023-05-25 01:10:58.000000 msg_explorer-1.7.0/msg_explorer/ui/guid_viewer.ui
+-rw-rw-rw-   0        0        0      932 2023-05-25 01:10:58.000000 msg_explorer-1.7.0/msg_explorer/ui/hex_viewer.ui
+-rw-rw-rw-   0        0        0     1089 2023-05-25 01:10:58.000000 msg_explorer-1.7.0/msg_explorer/ui/loading_screen.ui
+-rw-rw-rw-   0        0        0      786 2023-05-25 01:10:58.000000 msg_explorer-1.7.0/msg_explorer/ui/logger_widget.ui
+-rw-rw-rw-   0        0        0     4506 2023-05-25 01:10:58.000000 msg_explorer-1.7.0/msg_explorer/ui/main_window.ui
+-rw-rw-rw-   0        0        0     3509 2023-05-25 01:10:58.000000 msg_explorer-1.7.0/msg_explorer/ui/msg_details_page.ui
+-rw-rw-rw-   0        0        0     1232 2023-05-25 01:10:58.000000 msg_explorer-1.7.0/msg_explorer/ui/msg_tree_viewer.ui
+-rw-rw-rw-   0        0        0     1635 2023-05-25 01:10:58.000000 msg_explorer-1.7.0/msg_explorer/ui/multiple_binary_viewer.ui
+-rw-rw-rw-   0        0        0     1554 2023-05-25 01:10:58.000000 msg_explorer-1.7.0/msg_explorer/ui/multiple_viewer.ui
+-rw-rw-rw-   0        0        0     1655 2023-05-25 01:10:58.000000 msg_explorer-1.7.0/msg_explorer/ui/named_properties_viewer.ui
+-rw-rw-rw-   0        0        0     1525 2023-05-25 01:10:58.000000 msg_explorer-1.7.0/msg_explorer/ui/properties_viewer.ui
+-rw-rw-rw-   0        0        0     4575 2023-05-25 01:10:58.000000 msg_explorer-1.7.0/msg_explorer/ui/stream_viewer.ui
+-rw-rw-rw-   0        0        0      895 2023-05-25 01:10:58.000000 msg_explorer-1.7.0/msg_explorer/ui/string_viewer.ui
+-rw-rw-rw-   0        0        0     1128 2023-05-25 01:10:58.000000 msg_explorer-1.7.0/msg_explorer/ui/unhandled_exception.ui
+-rw-rw-rw-   0        0        0     1093 2023-05-25 01:10:58.000000 msg_explorer-1.7.0/msg_explorer/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-25 01:11:39.073820 msg_explorer-1.7.0/msg_explorer.egg-info/
+-rw-rw-rw-   0        0        0     3221 2023-05-25 01:11:38.000000 msg_explorer-1.7.0/msg_explorer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1588 2023-05-25 01:11:38.000000 msg_explorer-1.7.0/msg_explorer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 01:11:38.000000 msg_explorer-1.7.0/msg_explorer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2023-05-25 01:11:38.000000 msg_explorer-1.7.0/msg_explorer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       46 2023-05-25 01:11:38.000000 msg_explorer-1.7.0/msg_explorer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-25 01:11:38.000000 msg_explorer-1.7.0/msg_explorer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       74 2023-05-25 01:10:58.000000 msg_explorer-1.7.0/requirements.txt
+-rw-rw-rw-   0        0        0       74 2023-05-25 01:11:39.103157 msg_explorer-1.7.0/setup.cfg
+-rw-rw-rw-   0        0        0     1810 2023-05-25 01:10:58.000000 msg_explorer-1.7.0/setup.py
```

### Comparing `msg_explorer-1.6.0/CHANGELOG.md` & `msg_explorer-1.7.0/CHANGELOG.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,64 +1,68 @@
-**v1.6.0**
-* Fixed missing import in `__main__.py`.
-* Updated to `extract-msg` version `>=0.39.1, <0.40`.
-* Updated requirements to require Python 3.8 or greater. `extract-msg` will soon be updated to this, this update is preempting that.
-
-**v1.5.0**
-* Attempting to switch to strict semantic versioning. This version contains no breaking changes to API (possible exception is a bump to requirements), only additions.
-* Bump to `extract-msg` version 0.38.4.
-* Added button to export the current MSG file to a file. This works on non-embedded MSG files too.
-* Filtered more of the strings through the `tr` function so that text can be translated in more places.
-
-**v1.4.1**
-* Didn't properly edit the version number for extract-msg last time.
-
-**v1.4.0**
-* Upgraded to `extract-msg` version 0.36.0.
-* Fixed bug in `HexViewer` that caused the offset to be wrong.
-
-**v1.3.0**
-* Upgraded to `extract-msg` version 0.35.0. Named properties viewer has been updated to reflect the new form.
-
-**v1.2.7**
-* Fixed typo that prevented named properties on attachments from being viewed if they were a stream.
-* Removed debug prints that accidentally made it into the release.
-* Changed UI elements to use `ScrollPerPixel` instead of `ScrollPerItem`.
-
-**v1.2.6**
-* Fixed bugs in named property viewer.
-* Fixed a bug where sorting caused various tables to display incorrectly (forgot to turn off sorting while editing them and turn it back on afterwards).
-
-**v1.2.5**
-* Fixed issue that cause the multiple viewer to not clear it's data.
-
-**v1.2.4**
-* Fixed issue with files with non-standard streams from custom attachment types. There were issues with viewing the streams in the tree as well as with opening them in the stream viewer.
-* Switched `HexViewer` from `QPlainTextEdit` to `QTextEdit` to allow for coloring to easily differentiate the headers from the actual data.
-* Added the ability to drag and drop an MSG file onto the window to open it.
-
-**v1.2.3**
-* Added `python_requires` to setup.py.
-
-**v1.2.2**
-* Added app icon.
-
-**v1.2.1**
-* Expanded range of compatible extract-msg versions.
-* Fixed bugs that prevented properly viewing properties.
-
-**v1.2.0**
-* Updated to new version set of extract-msg (>=0.33.0, <0.34.0). Version 0.32.0 was skipped intentionally due to some issues in the code as well as to prioritize the release of version 0.33.0.
-* Fixed issue where double clicking attachments no longer worked (forgot to update the type checks to use the enum).
-* Fixed bug that caused streams in embedded MSG files to not be found if you loaded it to be the current MSG file.
-* Fixed typo that caused string viewer to not clear (forgot to add `.ui` before a ui element name).
-
-**v1.1.0**
-* Updated to new version set of extract-msg (>=0.31.0, <0.32.0).
-* Added sorting to many of the displays. Updated internal way data is handled to help this.
-* Added link to readme for supporting development.
-
-**v1.0.1**
-* Fix `README` to actually be correct. A lot was copied from msg-extractor and I missed a few sections.
-
-**v1.0.0**
-* Initial release.
+**v1.7.0**
+* Updated to `extract-msg` version `>=0.41.1, <0.42`.
+* Fixed a few bugs.
+
+**v1.6.0**
+* Fixed missing import in `__main__.py`.
+* Updated to `extract-msg` version `>=0.39.1, <0.40`.
+* Updated requirements to require Python 3.8 or greater. `extract-msg` will soon be updated to this, this update is preempting that.
+
+**v1.5.0**
+* Attempting to switch to strict semantic versioning. This version contains no breaking changes to API (possible exception is a bump to requirements), only additions.
+* Bump to `extract-msg` version 0.38.4.
+* Added button to export the current MSG file to a file. This works on non-embedded MSG files too.
+* Filtered more of the strings through the `tr` function so that text can be translated in more places.
+
+**v1.4.1**
+* Didn't properly edit the version number for extract-msg last time.
+
+**v1.4.0**
+* Upgraded to `extract-msg` version 0.36.0.
+* Fixed bug in `HexViewer` that caused the offset to be wrong.
+
+**v1.3.0**
+* Upgraded to `extract-msg` version 0.35.0. Named properties viewer has been updated to reflect the new form.
+
+**v1.2.7**
+* Fixed typo that prevented named properties on attachments from being viewed if they were a stream.
+* Removed debug prints that accidentally made it into the release.
+* Changed UI elements to use `ScrollPerPixel` instead of `ScrollPerItem`.
+
+**v1.2.6**
+* Fixed bugs in named property viewer.
+* Fixed a bug where sorting caused various tables to display incorrectly (forgot to turn off sorting while editing them and turn it back on afterwards).
+
+**v1.2.5**
+* Fixed issue that cause the multiple viewer to not clear it's data.
+
+**v1.2.4**
+* Fixed issue with files with non-standard streams from custom attachment types. There were issues with viewing the streams in the tree as well as with opening them in the stream viewer.
+* Switched `HexViewer` from `QPlainTextEdit` to `QTextEdit` to allow for coloring to easily differentiate the headers from the actual data.
+* Added the ability to drag and drop an MSG file onto the window to open it.
+
+**v1.2.3**
+* Added `python_requires` to setup.py.
+
+**v1.2.2**
+* Added app icon.
+
+**v1.2.1**
+* Expanded range of compatible extract-msg versions.
+* Fixed bugs that prevented properly viewing properties.
+
+**v1.2.0**
+* Updated to new version set of extract-msg (>=0.33.0, <0.34.0). Version 0.32.0 was skipped intentionally due to some issues in the code as well as to prioritize the release of version 0.33.0.
+* Fixed issue where double clicking attachments no longer worked (forgot to update the type checks to use the enum).
+* Fixed bug that caused streams in embedded MSG files to not be found if you loaded it to be the current MSG file.
+* Fixed typo that caused string viewer to not clear (forgot to add `.ui` before a ui element name).
+
+**v1.1.0**
+* Updated to new version set of extract-msg (>=0.31.0, <0.32.0).
+* Added sorting to many of the displays. Updated internal way data is handled to help this.
+* Added link to readme for supporting development.
+
+**v1.0.1**
+* Fix `README` to actually be correct. A lot was copied from msg-extractor and I missed a few sections.
+
+**v1.0.0**
+* Initial release.
```

### Comparing `msg_explorer-1.6.0/LICENSE.txt` & `msg_explorer-1.7.0/LICENSE.txt`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,674 +1,674 @@
-                    GNU GENERAL PUBLIC LICENSE
-                       Version 3, 29 June 2007
-
- Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
- Everyone is permitted to copy and distribute verbatim copies
- of this license document, but changing it is not allowed.
-
-                            Preamble
-
-  The GNU General Public License is a free, copyleft license for
-software and other kinds of works.
-
-  The licenses for most software and other practical works are designed
-to take away your freedom to share and change the works.  By contrast,
-the GNU General Public License is intended to guarantee your freedom to
-share and change all versions of a program--to make sure it remains free
-software for all its users.  We, the Free Software Foundation, use the
-GNU General Public License for most of our software; it applies also to
-any other work released this way by its authors.  You can apply it to
-your programs, too.
-
-  When we speak of free software, we are referring to freedom, not
-price.  Our General Public Licenses are designed to make sure that you
-have the freedom to distribute copies of free software (and charge for
-them if you wish), that you receive source code or can get it if you
-want it, that you can change the software or use pieces of it in new
-free programs, and that you know you can do these things.
-
-  To protect your rights, we need to prevent others from denying you
-these rights or asking you to surrender the rights.  Therefore, you have
-certain responsibilities if you distribute copies of the software, or if
-you modify it: responsibilities to respect the freedom of others.
-
-  For example, if you distribute copies of such a program, whether
-gratis or for a fee, you must pass on to the recipients the same
-freedoms that you received.  You must make sure that they, too, receive
-or can get the source code.  And you must show them these terms so they
-know their rights.
-
-  Developers that use the GNU GPL protect your rights with two steps:
-(1) assert copyright on the software, and (2) offer you this License
-giving you legal permission to copy, distribute and/or modify it.
-
-  For the developers' and authors' protection, the GPL clearly explains
-that there is no warranty for this free software.  For both users' and
-authors' sake, the GPL requires that modified versions be marked as
-changed, so that their problems will not be attributed erroneously to
-authors of previous versions.
-
-  Some devices are designed to deny users access to install or run
-modified versions of the software inside them, although the manufacturer
-can do so.  This is fundamentally incompatible with the aim of
-protecting users' freedom to change the software.  The systematic
-pattern of such abuse occurs in the area of products for individuals to
-use, which is precisely where it is most unacceptable.  Therefore, we
-have designed this version of the GPL to prohibit the practice for those
-products.  If such problems arise substantially in other domains, we
-stand ready to extend this provision to those domains in future versions
-of the GPL, as needed to protect the freedom of users.
-
-  Finally, every program is threatened constantly by software patents.
-States should not allow patents to restrict development and use of
-software on general-purpose computers, but in those that do, we wish to
-avoid the special danger that patents applied to a free program could
-make it effectively proprietary.  To prevent this, the GPL assures that
-patents cannot be used to render the program non-free.
-
-  The precise terms and conditions for copying, distribution and
-modification follow.
-
-                       TERMS AND CONDITIONS
-
-  0. Definitions.
-
-  "This License" refers to version 3 of the GNU General Public License.
-
-  "Copyright" also means copyright-like laws that apply to other kinds of
-works, such as semiconductor masks.
-
-  "The Program" refers to any copyrightable work licensed under this
-License.  Each licensee is addressed as "you".  "Licensees" and
-"recipients" may be individuals or organizations.
-
-  To "modify" a work means to copy from or adapt all or part of the work
-in a fashion requiring copyright permission, other than the making of an
-exact copy.  The resulting work is called a "modified version" of the
-earlier work or a work "based on" the earlier work.
-
-  A "covered work" means either the unmodified Program or a work based
-on the Program.
-
-  To "propagate" a work means to do anything with it that, without
-permission, would make you directly or secondarily liable for
-infringement under applicable copyright law, except executing it on a
-computer or modifying a private copy.  Propagation includes copying,
-distribution (with or without modification), making available to the
-public, and in some countries other activities as well.
-
-  To "convey" a work means any kind of propagation that enables other
-parties to make or receive copies.  Mere interaction with a user through
-a computer network, with no transfer of a copy, is not conveying.
-
-  An interactive user interface displays "Appropriate Legal Notices"
-to the extent that it includes a convenient and prominently visible
-feature that (1) displays an appropriate copyright notice, and (2)
-tells the user that there is no warranty for the work (except to the
-extent that warranties are provided), that licensees may convey the
-work under this License, and how to view a copy of this License.  If
-the interface presents a list of user commands or options, such as a
-menu, a prominent item in the list meets this criterion.
-
-  1. Source Code.
-
-  The "source code" for a work means the preferred form of the work
-for making modifications to it.  "Object code" means any non-source
-form of a work.
-
-  A "Standard Interface" means an interface that either is an official
-standard defined by a recognized standards body, or, in the case of
-interfaces specified for a particular programming language, one that
-is widely used among developers working in that language.
-
-  The "System Libraries" of an executable work include anything, other
-than the work as a whole, that (a) is included in the normal form of
-packaging a Major Component, but which is not part of that Major
-Component, and (b) serves only to enable use of the work with that
-Major Component, or to implement a Standard Interface for which an
-implementation is available to the public in source code form.  A
-"Major Component", in this context, means a major essential component
-(kernel, window system, and so on) of the specific operating system
-(if any) on which the executable work runs, or a compiler used to
-produce the work, or an object code interpreter used to run it.
-
-  The "Corresponding Source" for a work in object code form means all
-the source code needed to generate, install, and (for an executable
-work) run the object code and to modify the work, including scripts to
-control those activities.  However, it does not include the work's
-System Libraries, or general-purpose tools or generally available free
-programs which are used unmodified in performing those activities but
-which are not part of the work.  For example, Corresponding Source
-includes interface definition files associated with source files for
-the work, and the source code for shared libraries and dynamically
-linked subprograms that the work is specifically designed to require,
-such as by intimate data communication or control flow between those
-subprograms and other parts of the work.
-
-  The Corresponding Source need not include anything that users
-can regenerate automatically from other parts of the Corresponding
-Source.
-
-  The Corresponding Source for a work in source code form is that
-same work.
-
-  2. Basic Permissions.
-
-  All rights granted under this License are granted for the term of
-copyright on the Program, and are irrevocable provided the stated
-conditions are met.  This License explicitly affirms your unlimited
-permission to run the unmodified Program.  The output from running a
-covered work is covered by this License only if the output, given its
-content, constitutes a covered work.  This License acknowledges your
-rights of fair use or other equivalent, as provided by copyright law.
-
-  You may make, run and propagate covered works that you do not
-convey, without conditions so long as your license otherwise remains
-in force.  You may convey covered works to others for the sole purpose
-of having them make modifications exclusively for you, or provide you
-with facilities for running those works, provided that you comply with
-the terms of this License in conveying all material for which you do
-not control copyright.  Those thus making or running the covered works
-for you must do so exclusively on your behalf, under your direction
-and control, on terms that prohibit them from making any copies of
-your copyrighted material outside their relationship with you.
-
-  Conveying under any other circumstances is permitted solely under
-the conditions stated below.  Sublicensing is not allowed; section 10
-makes it unnecessary.
-
-  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
-
-  No covered work shall be deemed part of an effective technological
-measure under any applicable law fulfilling obligations under article
-11 of the WIPO copyright treaty adopted on 20 December 1996, or
-similar laws prohibiting or restricting circumvention of such
-measures.
-
-  When you convey a covered work, you waive any legal power to forbid
-circumvention of technological measures to the extent such circumvention
-is effected by exercising rights under this License with respect to
-the covered work, and you disclaim any intention to limit operation or
-modification of the work as a means of enforcing, against the work's
-users, your or third parties' legal rights to forbid circumvention of
-technological measures.
-
-  4. Conveying Verbatim Copies.
-
-  You may convey verbatim copies of the Program's source code as you
-receive it, in any medium, provided that you conspicuously and
-appropriately publish on each copy an appropriate copyright notice;
-keep intact all notices stating that this License and any
-non-permissive terms added in accord with section 7 apply to the code;
-keep intact all notices of the absence of any warranty; and give all
-recipients a copy of this License along with the Program.
-
-  You may charge any price or no price for each copy that you convey,
-and you may offer support or warranty protection for a fee.
-
-  5. Conveying Modified Source Versions.
-
-  You may convey a work based on the Program, or the modifications to
-produce it from the Program, in the form of source code under the
-terms of section 4, provided that you also meet all of these conditions:
-
-    a) The work must carry prominent notices stating that you modified
-    it, and giving a relevant date.
-
-    b) The work must carry prominent notices stating that it is
-    released under this License and any conditions added under section
-    7.  This requirement modifies the requirement in section 4 to
-    "keep intact all notices".
-
-    c) You must license the entire work, as a whole, under this
-    License to anyone who comes into possession of a copy.  This
-    License will therefore apply, along with any applicable section 7
-    additional terms, to the whole of the work, and all its parts,
-    regardless of how they are packaged.  This License gives no
-    permission to license the work in any other way, but it does not
-    invalidate such permission if you have separately received it.
-
-    d) If the work has interactive user interfaces, each must display
-    Appropriate Legal Notices; however, if the Program has interactive
-    interfaces that do not display Appropriate Legal Notices, your
-    work need not make them do so.
-
-  A compilation of a covered work with other separate and independent
-works, which are not by their nature extensions of the covered work,
-and which are not combined with it such as to form a larger program,
-in or on a volume of a storage or distribution medium, is called an
-"aggregate" if the compilation and its resulting copyright are not
-used to limit the access or legal rights of the compilation's users
-beyond what the individual works permit.  Inclusion of a covered work
-in an aggregate does not cause this License to apply to the other
-parts of the aggregate.
-
-  6. Conveying Non-Source Forms.
-
-  You may convey a covered work in object code form under the terms
-of sections 4 and 5, provided that you also convey the
-machine-readable Corresponding Source under the terms of this License,
-in one of these ways:
-
-    a) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by the
-    Corresponding Source fixed on a durable physical medium
-    customarily used for software interchange.
-
-    b) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by a
-    written offer, valid for at least three years and valid for as
-    long as you offer spare parts or customer support for that product
-    model, to give anyone who possesses the object code either (1) a
-    copy of the Corresponding Source for all the software in the
-    product that is covered by this License, on a durable physical
-    medium customarily used for software interchange, for a price no
-    more than your reasonable cost of physically performing this
-    conveying of source, or (2) access to copy the
-    Corresponding Source from a network server at no charge.
-
-    c) Convey individual copies of the object code with a copy of the
-    written offer to provide the Corresponding Source.  This
-    alternative is allowed only occasionally and noncommercially, and
-    only if you received the object code with such an offer, in accord
-    with subsection 6b.
-
-    d) Convey the object code by offering access from a designated
-    place (gratis or for a charge), and offer equivalent access to the
-    Corresponding Source in the same way through the same place at no
-    further charge.  You need not require recipients to copy the
-    Corresponding Source along with the object code.  If the place to
-    copy the object code is a network server, the Corresponding Source
-    may be on a different server (operated by you or a third party)
-    that supports equivalent copying facilities, provided you maintain
-    clear directions next to the object code saying where to find the
-    Corresponding Source.  Regardless of what server hosts the
-    Corresponding Source, you remain obligated to ensure that it is
-    available for as long as needed to satisfy these requirements.
-
-    e) Convey the object code using peer-to-peer transmission, provided
-    you inform other peers where the object code and Corresponding
-    Source of the work are being offered to the general public at no
-    charge under subsection 6d.
-
-  A separable portion of the object code, whose source code is excluded
-from the Corresponding Source as a System Library, need not be
-included in conveying the object code work.
-
-  A "User Product" is either (1) a "consumer product", which means any
-tangible personal property which is normally used for personal, family,
-or household purposes, or (2) anything designed or sold for incorporation
-into a dwelling.  In determining whether a product is a consumer product,
-doubtful cases shall be resolved in favor of coverage.  For a particular
-product received by a particular user, "normally used" refers to a
-typical or common use of that class of product, regardless of the status
-of the particular user or of the way in which the particular user
-actually uses, or expects or is expected to use, the product.  A product
-is a consumer product regardless of whether the product has substantial
-commercial, industrial or non-consumer uses, unless such uses represent
-the only significant mode of use of the product.
-
-  "Installation Information" for a User Product means any methods,
-procedures, authorization keys, or other information required to install
-and execute modified versions of a covered work in that User Product from
-a modified version of its Corresponding Source.  The information must
-suffice to ensure that the continued functioning of the modified object
-code is in no case prevented or interfered with solely because
-modification has been made.
-
-  If you convey an object code work under this section in, or with, or
-specifically for use in, a User Product, and the conveying occurs as
-part of a transaction in which the right of possession and use of the
-User Product is transferred to the recipient in perpetuity or for a
-fixed term (regardless of how the transaction is characterized), the
-Corresponding Source conveyed under this section must be accompanied
-by the Installation Information.  But this requirement does not apply
-if neither you nor any third party retains the ability to install
-modified object code on the User Product (for example, the work has
-been installed in ROM).
-
-  The requirement to provide Installation Information does not include a
-requirement to continue to provide support service, warranty, or updates
-for a work that has been modified or installed by the recipient, or for
-the User Product in which it has been modified or installed.  Access to a
-network may be denied when the modification itself materially and
-adversely affects the operation of the network or violates the rules and
-protocols for communication across the network.
-
-  Corresponding Source conveyed, and Installation Information provided,
-in accord with this section must be in a format that is publicly
-documented (and with an implementation available to the public in
-source code form), and must require no special password or key for
-unpacking, reading or copying.
-
-  7. Additional Terms.
-
-  "Additional permissions" are terms that supplement the terms of this
-License by making exceptions from one or more of its conditions.
-Additional permissions that are applicable to the entire Program shall
-be treated as though they were included in this License, to the extent
-that they are valid under applicable law.  If additional permissions
-apply only to part of the Program, that part may be used separately
-under those permissions, but the entire Program remains governed by
-this License without regard to the additional permissions.
-
-  When you convey a copy of a covered work, you may at your option
-remove any additional permissions from that copy, or from any part of
-it.  (Additional permissions may be written to require their own
-removal in certain cases when you modify the work.)  You may place
-additional permissions on material, added by you to a covered work,
-for which you have or can give appropriate copyright permission.
-
-  Notwithstanding any other provision of this License, for material you
-add to a covered work, you may (if authorized by the copyright holders of
-that material) supplement the terms of this License with terms:
-
-    a) Disclaiming warranty or limiting liability differently from the
-    terms of sections 15 and 16 of this License; or
-
-    b) Requiring preservation of specified reasonable legal notices or
-    author attributions in that material or in the Appropriate Legal
-    Notices displayed by works containing it; or
-
-    c) Prohibiting misrepresentation of the origin of that material, or
-    requiring that modified versions of such material be marked in
-    reasonable ways as different from the original version; or
-
-    d) Limiting the use for publicity purposes of names of licensors or
-    authors of the material; or
-
-    e) Declining to grant rights under trademark law for use of some
-    trade names, trademarks, or service marks; or
-
-    f) Requiring indemnification of licensors and authors of that
-    material by anyone who conveys the material (or modified versions of
-    it) with contractual assumptions of liability to the recipient, for
-    any liability that these contractual assumptions directly impose on
-    those licensors and authors.
-
-  All other non-permissive additional terms are considered "further
-restrictions" within the meaning of section 10.  If the Program as you
-received it, or any part of it, contains a notice stating that it is
-governed by this License along with a term that is a further
-restriction, you may remove that term.  If a license document contains
-a further restriction but permits relicensing or conveying under this
-License, you may add to a covered work material governed by the terms
-of that license document, provided that the further restriction does
-not survive such relicensing or conveying.
-
-  If you add terms to a covered work in accord with this section, you
-must place, in the relevant source files, a statement of the
-additional terms that apply to those files, or a notice indicating
-where to find the applicable terms.
-
-  Additional terms, permissive or non-permissive, may be stated in the
-form of a separately written license, or stated as exceptions;
-the above requirements apply either way.
-
-  8. Termination.
-
-  You may not propagate or modify a covered work except as expressly
-provided under this License.  Any attempt otherwise to propagate or
-modify it is void, and will automatically terminate your rights under
-this License (including any patent licenses granted under the third
-paragraph of section 11).
-
-  However, if you cease all violation of this License, then your
-license from a particular copyright holder is reinstated (a)
-provisionally, unless and until the copyright holder explicitly and
-finally terminates your license, and (b) permanently, if the copyright
-holder fails to notify you of the violation by some reasonable means
-prior to 60 days after the cessation.
-
-  Moreover, your license from a particular copyright holder is
-reinstated permanently if the copyright holder notifies you of the
-violation by some reasonable means, this is the first time you have
-received notice of violation of this License (for any work) from that
-copyright holder, and you cure the violation prior to 30 days after
-your receipt of the notice.
-
-  Termination of your rights under this section does not terminate the
-licenses of parties who have received copies or rights from you under
-this License.  If your rights have been terminated and not permanently
-reinstated, you do not qualify to receive new licenses for the same
-material under section 10.
-
-  9. Acceptance Not Required for Having Copies.
-
-  You are not required to accept this License in order to receive or
-run a copy of the Program.  Ancillary propagation of a covered work
-occurring solely as a consequence of using peer-to-peer transmission
-to receive a copy likewise does not require acceptance.  However,
-nothing other than this License grants you permission to propagate or
-modify any covered work.  These actions infringe copyright if you do
-not accept this License.  Therefore, by modifying or propagating a
-covered work, you indicate your acceptance of this License to do so.
-
-  10. Automatic Licensing of Downstream Recipients.
-
-  Each time you convey a covered work, the recipient automatically
-receives a license from the original licensors, to run, modify and
-propagate that work, subject to this License.  You are not responsible
-for enforcing compliance by third parties with this License.
-
-  An "entity transaction" is a transaction transferring control of an
-organization, or substantially all assets of one, or subdividing an
-organization, or merging organizations.  If propagation of a covered
-work results from an entity transaction, each party to that
-transaction who receives a copy of the work also receives whatever
-licenses to the work the party's predecessor in interest had or could
-give under the previous paragraph, plus a right to possession of the
-Corresponding Source of the work from the predecessor in interest, if
-the predecessor has it or can get it with reasonable efforts.
-
-  You may not impose any further restrictions on the exercise of the
-rights granted or affirmed under this License.  For example, you may
-not impose a license fee, royalty, or other charge for exercise of
-rights granted under this License, and you may not initiate litigation
-(including a cross-claim or counterclaim in a lawsuit) alleging that
-any patent claim is infringed by making, using, selling, offering for
-sale, or importing the Program or any portion of it.
-
-  11. Patents.
-
-  A "contributor" is a copyright holder who authorizes use under this
-License of the Program or a work on which the Program is based.  The
-work thus licensed is called the contributor's "contributor version".
-
-  A contributor's "essential patent claims" are all patent claims
-owned or controlled by the contributor, whether already acquired or
-hereafter acquired, that would be infringed by some manner, permitted
-by this License, of making, using, or selling its contributor version,
-but do not include claims that would be infringed only as a
-consequence of further modification of the contributor version.  For
-purposes of this definition, "control" includes the right to grant
-patent sublicenses in a manner consistent with the requirements of
-this License.
-
-  Each contributor grants you a non-exclusive, worldwide, royalty-free
-patent license under the contributor's essential patent claims, to
-make, use, sell, offer for sale, import and otherwise run, modify and
-propagate the contents of its contributor version.
-
-  In the following three paragraphs, a "patent license" is any express
-agreement or commitment, however denominated, not to enforce a patent
-(such as an express permission to practice a patent or covenant not to
-sue for patent infringement).  To "grant" such a patent license to a
-party means to make such an agreement or commitment not to enforce a
-patent against the party.
-
-  If you convey a covered work, knowingly relying on a patent license,
-and the Corresponding Source of the work is not available for anyone
-to copy, free of charge and under the terms of this License, through a
-publicly available network server or other readily accessible means,
-then you must either (1) cause the Corresponding Source to be so
-available, or (2) arrange to deprive yourself of the benefit of the
-patent license for this particular work, or (3) arrange, in a manner
-consistent with the requirements of this License, to extend the patent
-license to downstream recipients.  "Knowingly relying" means you have
-actual knowledge that, but for the patent license, your conveying the
-covered work in a country, or your recipient's use of the covered work
-in a country, would infringe one or more identifiable patents in that
-country that you have reason to believe are valid.
-
-  If, pursuant to or in connection with a single transaction or
-arrangement, you convey, or propagate by procuring conveyance of, a
-covered work, and grant a patent license to some of the parties
-receiving the covered work authorizing them to use, propagate, modify
-or convey a specific copy of the covered work, then the patent license
-you grant is automatically extended to all recipients of the covered
-work and works based on it.
-
-  A patent license is "discriminatory" if it does not include within
-the scope of its coverage, prohibits the exercise of, or is
-conditioned on the non-exercise of one or more of the rights that are
-specifically granted under this License.  You may not convey a covered
-work if you are a party to an arrangement with a third party that is
-in the business of distributing software, under which you make payment
-to the third party based on the extent of your activity of conveying
-the work, and under which the third party grants, to any of the
-parties who would receive the covered work from you, a discriminatory
-patent license (a) in connection with copies of the covered work
-conveyed by you (or copies made from those copies), or (b) primarily
-for and in connection with specific products or compilations that
-contain the covered work, unless you entered into that arrangement,
-or that patent license was granted, prior to 28 March 2007.
-
-  Nothing in this License shall be construed as excluding or limiting
-any implied license or other defenses to infringement that may
-otherwise be available to you under applicable patent law.
-
-  12. No Surrender of Others' Freedom.
-
-  If conditions are imposed on you (whether by court order, agreement or
-otherwise) that contradict the conditions of this License, they do not
-excuse you from the conditions of this License.  If you cannot convey a
-covered work so as to satisfy simultaneously your obligations under this
-License and any other pertinent obligations, then as a consequence you may
-not convey it at all.  For example, if you agree to terms that obligate you
-to collect a royalty for further conveying from those to whom you convey
-the Program, the only way you could satisfy both those terms and this
-License would be to refrain entirely from conveying the Program.
-
-  13. Use with the GNU Affero General Public License.
-
-  Notwithstanding any other provision of this License, you have
-permission to link or combine any covered work with a work licensed
-under version 3 of the GNU Affero General Public License into a single
-combined work, and to convey the resulting work.  The terms of this
-License will continue to apply to the part which is the covered work,
-but the special requirements of the GNU Affero General Public License,
-section 13, concerning interaction through a network will apply to the
-combination as such.
-
-  14. Revised Versions of this License.
-
-  The Free Software Foundation may publish revised and/or new versions of
-the GNU General Public License from time to time.  Such new versions will
-be similar in spirit to the present version, but may differ in detail to
-address new problems or concerns.
-
-  Each version is given a distinguishing version number.  If the
-Program specifies that a certain numbered version of the GNU General
-Public License "or any later version" applies to it, you have the
-option of following the terms and conditions either of that numbered
-version or of any later version published by the Free Software
-Foundation.  If the Program does not specify a version number of the
-GNU General Public License, you may choose any version ever published
-by the Free Software Foundation.
-
-  If the Program specifies that a proxy can decide which future
-versions of the GNU General Public License can be used, that proxy's
-public statement of acceptance of a version permanently authorizes you
-to choose that version for the Program.
-
-  Later license versions may give you additional or different
-permissions.  However, no additional obligations are imposed on any
-author or copyright holder as a result of your choosing to follow a
-later version.
-
-  15. Disclaimer of Warranty.
-
-  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
-APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
-HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
-OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
-THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
-PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
-IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
-ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
-
-  16. Limitation of Liability.
-
-  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
-WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
-THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
-GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
-USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
-DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
-PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
-EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
-SUCH DAMAGES.
-
-  17. Interpretation of Sections 15 and 16.
-
-  If the disclaimer of warranty and limitation of liability provided
-above cannot be given local legal effect according to their terms,
-reviewing courts shall apply local law that most closely approximates
-an absolute waiver of all civil liability in connection with the
-Program, unless a warranty or assumption of liability accompanies a
-copy of the Program in return for a fee.
-
-                     END OF TERMS AND CONDITIONS
-
-            How to Apply These Terms to Your New Programs
-
-  If you develop a new program, and you want it to be of the greatest
-possible use to the public, the best way to achieve this is to make it
-free software which everyone can redistribute and change under these terms.
-
-  To do so, attach the following notices to the program.  It is safest
-to attach them to the start of each source file to most effectively
-state the exclusion of warranty; and each file should have at least
-the "copyright" line and a pointer to where the full notice is found.
-
-    <one line to give the program's name and a brief idea of what it does.>
-    Copyright (C) <year>  <name of author>
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program.  If not, see <http://www.gnu.org/licenses/>.
-
-Also add information on how to contact you by electronic and paper mail.
-
-  If the program does terminal interaction, make it output a short
-notice like this when it starts in an interactive mode:
-
-    <program>  Copyright (C) <year>  <name of author>
-    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
-    This is free software, and you are welcome to redistribute it
-    under certain conditions; type `show c' for details.
-
-The hypothetical commands `show w' and `show c' should show the appropriate
-parts of the General Public License.  Of course, your program's commands
-might be different; for a GUI interface, you would use an "about box".
-
-  You should also get your employer (if you work as a programmer) or school,
-if any, to sign a "copyright disclaimer" for the program, if necessary.
-For more information on this, and how to apply and follow the GNU GPL, see
-<http://www.gnu.org/licenses/>.
-
-  The GNU General Public License does not permit incorporating your program
-into proprietary programs.  If your program is a subroutine library, you
-may consider it more useful to permit linking proprietary applications with
-the library.  If this is what you want to do, use the GNU Lesser General
-Public License instead of this License.  But first, please read
-<http://www.gnu.org/philosophy/why-not-lgpl.html>.
+                    GNU GENERAL PUBLIC LICENSE
+                       Version 3, 29 June 2007
+
+ Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
+ Everyone is permitted to copy and distribute verbatim copies
+ of this license document, but changing it is not allowed.
+
+                            Preamble
+
+  The GNU General Public License is a free, copyleft license for
+software and other kinds of works.
+
+  The licenses for most software and other practical works are designed
+to take away your freedom to share and change the works.  By contrast,
+the GNU General Public License is intended to guarantee your freedom to
+share and change all versions of a program--to make sure it remains free
+software for all its users.  We, the Free Software Foundation, use the
+GNU General Public License for most of our software; it applies also to
+any other work released this way by its authors.  You can apply it to
+your programs, too.
+
+  When we speak of free software, we are referring to freedom, not
+price.  Our General Public Licenses are designed to make sure that you
+have the freedom to distribute copies of free software (and charge for
+them if you wish), that you receive source code or can get it if you
+want it, that you can change the software or use pieces of it in new
+free programs, and that you know you can do these things.
+
+  To protect your rights, we need to prevent others from denying you
+these rights or asking you to surrender the rights.  Therefore, you have
+certain responsibilities if you distribute copies of the software, or if
+you modify it: responsibilities to respect the freedom of others.
+
+  For example, if you distribute copies of such a program, whether
+gratis or for a fee, you must pass on to the recipients the same
+freedoms that you received.  You must make sure that they, too, receive
+or can get the source code.  And you must show them these terms so they
+know their rights.
+
+  Developers that use the GNU GPL protect your rights with two steps:
+(1) assert copyright on the software, and (2) offer you this License
+giving you legal permission to copy, distribute and/or modify it.
+
+  For the developers' and authors' protection, the GPL clearly explains
+that there is no warranty for this free software.  For both users' and
+authors' sake, the GPL requires that modified versions be marked as
+changed, so that their problems will not be attributed erroneously to
+authors of previous versions.
+
+  Some devices are designed to deny users access to install or run
+modified versions of the software inside them, although the manufacturer
+can do so.  This is fundamentally incompatible with the aim of
+protecting users' freedom to change the software.  The systematic
+pattern of such abuse occurs in the area of products for individuals to
+use, which is precisely where it is most unacceptable.  Therefore, we
+have designed this version of the GPL to prohibit the practice for those
+products.  If such problems arise substantially in other domains, we
+stand ready to extend this provision to those domains in future versions
+of the GPL, as needed to protect the freedom of users.
+
+  Finally, every program is threatened constantly by software patents.
+States should not allow patents to restrict development and use of
+software on general-purpose computers, but in those that do, we wish to
+avoid the special danger that patents applied to a free program could
+make it effectively proprietary.  To prevent this, the GPL assures that
+patents cannot be used to render the program non-free.
+
+  The precise terms and conditions for copying, distribution and
+modification follow.
+
+                       TERMS AND CONDITIONS
+
+  0. Definitions.
+
+  "This License" refers to version 3 of the GNU General Public License.
+
+  "Copyright" also means copyright-like laws that apply to other kinds of
+works, such as semiconductor masks.
+
+  "The Program" refers to any copyrightable work licensed under this
+License.  Each licensee is addressed as "you".  "Licensees" and
+"recipients" may be individuals or organizations.
+
+  To "modify" a work means to copy from or adapt all or part of the work
+in a fashion requiring copyright permission, other than the making of an
+exact copy.  The resulting work is called a "modified version" of the
+earlier work or a work "based on" the earlier work.
+
+  A "covered work" means either the unmodified Program or a work based
+on the Program.
+
+  To "propagate" a work means to do anything with it that, without
+permission, would make you directly or secondarily liable for
+infringement under applicable copyright law, except executing it on a
+computer or modifying a private copy.  Propagation includes copying,
+distribution (with or without modification), making available to the
+public, and in some countries other activities as well.
+
+  To "convey" a work means any kind of propagation that enables other
+parties to make or receive copies.  Mere interaction with a user through
+a computer network, with no transfer of a copy, is not conveying.
+
+  An interactive user interface displays "Appropriate Legal Notices"
+to the extent that it includes a convenient and prominently visible
+feature that (1) displays an appropriate copyright notice, and (2)
+tells the user that there is no warranty for the work (except to the
+extent that warranties are provided), that licensees may convey the
+work under this License, and how to view a copy of this License.  If
+the interface presents a list of user commands or options, such as a
+menu, a prominent item in the list meets this criterion.
+
+  1. Source Code.
+
+  The "source code" for a work means the preferred form of the work
+for making modifications to it.  "Object code" means any non-source
+form of a work.
+
+  A "Standard Interface" means an interface that either is an official
+standard defined by a recognized standards body, or, in the case of
+interfaces specified for a particular programming language, one that
+is widely used among developers working in that language.
+
+  The "System Libraries" of an executable work include anything, other
+than the work as a whole, that (a) is included in the normal form of
+packaging a Major Component, but which is not part of that Major
+Component, and (b) serves only to enable use of the work with that
+Major Component, or to implement a Standard Interface for which an
+implementation is available to the public in source code form.  A
+"Major Component", in this context, means a major essential component
+(kernel, window system, and so on) of the specific operating system
+(if any) on which the executable work runs, or a compiler used to
+produce the work, or an object code interpreter used to run it.
+
+  The "Corresponding Source" for a work in object code form means all
+the source code needed to generate, install, and (for an executable
+work) run the object code and to modify the work, including scripts to
+control those activities.  However, it does not include the work's
+System Libraries, or general-purpose tools or generally available free
+programs which are used unmodified in performing those activities but
+which are not part of the work.  For example, Corresponding Source
+includes interface definition files associated with source files for
+the work, and the source code for shared libraries and dynamically
+linked subprograms that the work is specifically designed to require,
+such as by intimate data communication or control flow between those
+subprograms and other parts of the work.
+
+  The Corresponding Source need not include anything that users
+can regenerate automatically from other parts of the Corresponding
+Source.
+
+  The Corresponding Source for a work in source code form is that
+same work.
+
+  2. Basic Permissions.
+
+  All rights granted under this License are granted for the term of
+copyright on the Program, and are irrevocable provided the stated
+conditions are met.  This License explicitly affirms your unlimited
+permission to run the unmodified Program.  The output from running a
+covered work is covered by this License only if the output, given its
+content, constitutes a covered work.  This License acknowledges your
+rights of fair use or other equivalent, as provided by copyright law.
+
+  You may make, run and propagate covered works that you do not
+convey, without conditions so long as your license otherwise remains
+in force.  You may convey covered works to others for the sole purpose
+of having them make modifications exclusively for you, or provide you
+with facilities for running those works, provided that you comply with
+the terms of this License in conveying all material for which you do
+not control copyright.  Those thus making or running the covered works
+for you must do so exclusively on your behalf, under your direction
+and control, on terms that prohibit them from making any copies of
+your copyrighted material outside their relationship with you.
+
+  Conveying under any other circumstances is permitted solely under
+the conditions stated below.  Sublicensing is not allowed; section 10
+makes it unnecessary.
+
+  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
+
+  No covered work shall be deemed part of an effective technological
+measure under any applicable law fulfilling obligations under article
+11 of the WIPO copyright treaty adopted on 20 December 1996, or
+similar laws prohibiting or restricting circumvention of such
+measures.
+
+  When you convey a covered work, you waive any legal power to forbid
+circumvention of technological measures to the extent such circumvention
+is effected by exercising rights under this License with respect to
+the covered work, and you disclaim any intention to limit operation or
+modification of the work as a means of enforcing, against the work's
+users, your or third parties' legal rights to forbid circumvention of
+technological measures.
+
+  4. Conveying Verbatim Copies.
+
+  You may convey verbatim copies of the Program's source code as you
+receive it, in any medium, provided that you conspicuously and
+appropriately publish on each copy an appropriate copyright notice;
+keep intact all notices stating that this License and any
+non-permissive terms added in accord with section 7 apply to the code;
+keep intact all notices of the absence of any warranty; and give all
+recipients a copy of this License along with the Program.
+
+  You may charge any price or no price for each copy that you convey,
+and you may offer support or warranty protection for a fee.
+
+  5. Conveying Modified Source Versions.
+
+  You may convey a work based on the Program, or the modifications to
+produce it from the Program, in the form of source code under the
+terms of section 4, provided that you also meet all of these conditions:
+
+    a) The work must carry prominent notices stating that you modified
+    it, and giving a relevant date.
+
+    b) The work must carry prominent notices stating that it is
+    released under this License and any conditions added under section
+    7.  This requirement modifies the requirement in section 4 to
+    "keep intact all notices".
+
+    c) You must license the entire work, as a whole, under this
+    License to anyone who comes into possession of a copy.  This
+    License will therefore apply, along with any applicable section 7
+    additional terms, to the whole of the work, and all its parts,
+    regardless of how they are packaged.  This License gives no
+    permission to license the work in any other way, but it does not
+    invalidate such permission if you have separately received it.
+
+    d) If the work has interactive user interfaces, each must display
+    Appropriate Legal Notices; however, if the Program has interactive
+    interfaces that do not display Appropriate Legal Notices, your
+    work need not make them do so.
+
+  A compilation of a covered work with other separate and independent
+works, which are not by their nature extensions of the covered work,
+and which are not combined with it such as to form a larger program,
+in or on a volume of a storage or distribution medium, is called an
+"aggregate" if the compilation and its resulting copyright are not
+used to limit the access or legal rights of the compilation's users
+beyond what the individual works permit.  Inclusion of a covered work
+in an aggregate does not cause this License to apply to the other
+parts of the aggregate.
+
+  6. Conveying Non-Source Forms.
+
+  You may convey a covered work in object code form under the terms
+of sections 4 and 5, provided that you also convey the
+machine-readable Corresponding Source under the terms of this License,
+in one of these ways:
+
+    a) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by the
+    Corresponding Source fixed on a durable physical medium
+    customarily used for software interchange.
+
+    b) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by a
+    written offer, valid for at least three years and valid for as
+    long as you offer spare parts or customer support for that product
+    model, to give anyone who possesses the object code either (1) a
+    copy of the Corresponding Source for all the software in the
+    product that is covered by this License, on a durable physical
+    medium customarily used for software interchange, for a price no
+    more than your reasonable cost of physically performing this
+    conveying of source, or (2) access to copy the
+    Corresponding Source from a network server at no charge.
+
+    c) Convey individual copies of the object code with a copy of the
+    written offer to provide the Corresponding Source.  This
+    alternative is allowed only occasionally and noncommercially, and
+    only if you received the object code with such an offer, in accord
+    with subsection 6b.
+
+    d) Convey the object code by offering access from a designated
+    place (gratis or for a charge), and offer equivalent access to the
+    Corresponding Source in the same way through the same place at no
+    further charge.  You need not require recipients to copy the
+    Corresponding Source along with the object code.  If the place to
+    copy the object code is a network server, the Corresponding Source
+    may be on a different server (operated by you or a third party)
+    that supports equivalent copying facilities, provided you maintain
+    clear directions next to the object code saying where to find the
+    Corresponding Source.  Regardless of what server hosts the
+    Corresponding Source, you remain obligated to ensure that it is
+    available for as long as needed to satisfy these requirements.
+
+    e) Convey the object code using peer-to-peer transmission, provided
+    you inform other peers where the object code and Corresponding
+    Source of the work are being offered to the general public at no
+    charge under subsection 6d.
+
+  A separable portion of the object code, whose source code is excluded
+from the Corresponding Source as a System Library, need not be
+included in conveying the object code work.
+
+  A "User Product" is either (1) a "consumer product", which means any
+tangible personal property which is normally used for personal, family,
+or household purposes, or (2) anything designed or sold for incorporation
+into a dwelling.  In determining whether a product is a consumer product,
+doubtful cases shall be resolved in favor of coverage.  For a particular
+product received by a particular user, "normally used" refers to a
+typical or common use of that class of product, regardless of the status
+of the particular user or of the way in which the particular user
+actually uses, or expects or is expected to use, the product.  A product
+is a consumer product regardless of whether the product has substantial
+commercial, industrial or non-consumer uses, unless such uses represent
+the only significant mode of use of the product.
+
+  "Installation Information" for a User Product means any methods,
+procedures, authorization keys, or other information required to install
+and execute modified versions of a covered work in that User Product from
+a modified version of its Corresponding Source.  The information must
+suffice to ensure that the continued functioning of the modified object
+code is in no case prevented or interfered with solely because
+modification has been made.
+
+  If you convey an object code work under this section in, or with, or
+specifically for use in, a User Product, and the conveying occurs as
+part of a transaction in which the right of possession and use of the
+User Product is transferred to the recipient in perpetuity or for a
+fixed term (regardless of how the transaction is characterized), the
+Corresponding Source conveyed under this section must be accompanied
+by the Installation Information.  But this requirement does not apply
+if neither you nor any third party retains the ability to install
+modified object code on the User Product (for example, the work has
+been installed in ROM).
+
+  The requirement to provide Installation Information does not include a
+requirement to continue to provide support service, warranty, or updates
+for a work that has been modified or installed by the recipient, or for
+the User Product in which it has been modified or installed.  Access to a
+network may be denied when the modification itself materially and
+adversely affects the operation of the network or violates the rules and
+protocols for communication across the network.
+
+  Corresponding Source conveyed, and Installation Information provided,
+in accord with this section must be in a format that is publicly
+documented (and with an implementation available to the public in
+source code form), and must require no special password or key for
+unpacking, reading or copying.
+
+  7. Additional Terms.
+
+  "Additional permissions" are terms that supplement the terms of this
+License by making exceptions from one or more of its conditions.
+Additional permissions that are applicable to the entire Program shall
+be treated as though they were included in this License, to the extent
+that they are valid under applicable law.  If additional permissions
+apply only to part of the Program, that part may be used separately
+under those permissions, but the entire Program remains governed by
+this License without regard to the additional permissions.
+
+  When you convey a copy of a covered work, you may at your option
+remove any additional permissions from that copy, or from any part of
+it.  (Additional permissions may be written to require their own
+removal in certain cases when you modify the work.)  You may place
+additional permissions on material, added by you to a covered work,
+for which you have or can give appropriate copyright permission.
+
+  Notwithstanding any other provision of this License, for material you
+add to a covered work, you may (if authorized by the copyright holders of
+that material) supplement the terms of this License with terms:
+
+    a) Disclaiming warranty or limiting liability differently from the
+    terms of sections 15 and 16 of this License; or
+
+    b) Requiring preservation of specified reasonable legal notices or
+    author attributions in that material or in the Appropriate Legal
+    Notices displayed by works containing it; or
+
+    c) Prohibiting misrepresentation of the origin of that material, or
+    requiring that modified versions of such material be marked in
+    reasonable ways as different from the original version; or
+
+    d) Limiting the use for publicity purposes of names of licensors or
+    authors of the material; or
+
+    e) Declining to grant rights under trademark law for use of some
+    trade names, trademarks, or service marks; or
+
+    f) Requiring indemnification of licensors and authors of that
+    material by anyone who conveys the material (or modified versions of
+    it) with contractual assumptions of liability to the recipient, for
+    any liability that these contractual assumptions directly impose on
+    those licensors and authors.
+
+  All other non-permissive additional terms are considered "further
+restrictions" within the meaning of section 10.  If the Program as you
+received it, or any part of it, contains a notice stating that it is
+governed by this License along with a term that is a further
+restriction, you may remove that term.  If a license document contains
+a further restriction but permits relicensing or conveying under this
+License, you may add to a covered work material governed by the terms
+of that license document, provided that the further restriction does
+not survive such relicensing or conveying.
+
+  If you add terms to a covered work in accord with this section, you
+must place, in the relevant source files, a statement of the
+additional terms that apply to those files, or a notice indicating
+where to find the applicable terms.
+
+  Additional terms, permissive or non-permissive, may be stated in the
+form of a separately written license, or stated as exceptions;
+the above requirements apply either way.
+
+  8. Termination.
+
+  You may not propagate or modify a covered work except as expressly
+provided under this License.  Any attempt otherwise to propagate or
+modify it is void, and will automatically terminate your rights under
+this License (including any patent licenses granted under the third
+paragraph of section 11).
+
+  However, if you cease all violation of this License, then your
+license from a particular copyright holder is reinstated (a)
+provisionally, unless and until the copyright holder explicitly and
+finally terminates your license, and (b) permanently, if the copyright
+holder fails to notify you of the violation by some reasonable means
+prior to 60 days after the cessation.
+
+  Moreover, your license from a particular copyright holder is
+reinstated permanently if the copyright holder notifies you of the
+violation by some reasonable means, this is the first time you have
+received notice of violation of this License (for any work) from that
+copyright holder, and you cure the violation prior to 30 days after
+your receipt of the notice.
+
+  Termination of your rights under this section does not terminate the
+licenses of parties who have received copies or rights from you under
+this License.  If your rights have been terminated and not permanently
+reinstated, you do not qualify to receive new licenses for the same
+material under section 10.
+
+  9. Acceptance Not Required for Having Copies.
+
+  You are not required to accept this License in order to receive or
+run a copy of the Program.  Ancillary propagation of a covered work
+occurring solely as a consequence of using peer-to-peer transmission
+to receive a copy likewise does not require acceptance.  However,
+nothing other than this License grants you permission to propagate or
+modify any covered work.  These actions infringe copyright if you do
+not accept this License.  Therefore, by modifying or propagating a
+covered work, you indicate your acceptance of this License to do so.
+
+  10. Automatic Licensing of Downstream Recipients.
+
+  Each time you convey a covered work, the recipient automatically
+receives a license from the original licensors, to run, modify and
+propagate that work, subject to this License.  You are not responsible
+for enforcing compliance by third parties with this License.
+
+  An "entity transaction" is a transaction transferring control of an
+organization, or substantially all assets of one, or subdividing an
+organization, or merging organizations.  If propagation of a covered
+work results from an entity transaction, each party to that
+transaction who receives a copy of the work also receives whatever
+licenses to the work the party's predecessor in interest had or could
+give under the previous paragraph, plus a right to possession of the
+Corresponding Source of the work from the predecessor in interest, if
+the predecessor has it or can get it with reasonable efforts.
+
+  You may not impose any further restrictions on the exercise of the
+rights granted or affirmed under this License.  For example, you may
+not impose a license fee, royalty, or other charge for exercise of
+rights granted under this License, and you may not initiate litigation
+(including a cross-claim or counterclaim in a lawsuit) alleging that
+any patent claim is infringed by making, using, selling, offering for
+sale, or importing the Program or any portion of it.
+
+  11. Patents.
+
+  A "contributor" is a copyright holder who authorizes use under this
+License of the Program or a work on which the Program is based.  The
+work thus licensed is called the contributor's "contributor version".
+
+  A contributor's "essential patent claims" are all patent claims
+owned or controlled by the contributor, whether already acquired or
+hereafter acquired, that would be infringed by some manner, permitted
+by this License, of making, using, or selling its contributor version,
+but do not include claims that would be infringed only as a
+consequence of further modification of the contributor version.  For
+purposes of this definition, "control" includes the right to grant
+patent sublicenses in a manner consistent with the requirements of
+this License.
+
+  Each contributor grants you a non-exclusive, worldwide, royalty-free
+patent license under the contributor's essential patent claims, to
+make, use, sell, offer for sale, import and otherwise run, modify and
+propagate the contents of its contributor version.
+
+  In the following three paragraphs, a "patent license" is any express
+agreement or commitment, however denominated, not to enforce a patent
+(such as an express permission to practice a patent or covenant not to
+sue for patent infringement).  To "grant" such a patent license to a
+party means to make such an agreement or commitment not to enforce a
+patent against the party.
+
+  If you convey a covered work, knowingly relying on a patent license,
+and the Corresponding Source of the work is not available for anyone
+to copy, free of charge and under the terms of this License, through a
+publicly available network server or other readily accessible means,
+then you must either (1) cause the Corresponding Source to be so
+available, or (2) arrange to deprive yourself of the benefit of the
+patent license for this particular work, or (3) arrange, in a manner
+consistent with the requirements of this License, to extend the patent
+license to downstream recipients.  "Knowingly relying" means you have
+actual knowledge that, but for the patent license, your conveying the
+covered work in a country, or your recipient's use of the covered work
+in a country, would infringe one or more identifiable patents in that
+country that you have reason to believe are valid.
+
+  If, pursuant to or in connection with a single transaction or
+arrangement, you convey, or propagate by procuring conveyance of, a
+covered work, and grant a patent license to some of the parties
+receiving the covered work authorizing them to use, propagate, modify
+or convey a specific copy of the covered work, then the patent license
+you grant is automatically extended to all recipients of the covered
+work and works based on it.
+
+  A patent license is "discriminatory" if it does not include within
+the scope of its coverage, prohibits the exercise of, or is
+conditioned on the non-exercise of one or more of the rights that are
+specifically granted under this License.  You may not convey a covered
+work if you are a party to an arrangement with a third party that is
+in the business of distributing software, under which you make payment
+to the third party based on the extent of your activity of conveying
+the work, and under which the third party grants, to any of the
+parties who would receive the covered work from you, a discriminatory
+patent license (a) in connection with copies of the covered work
+conveyed by you (or copies made from those copies), or (b) primarily
+for and in connection with specific products or compilations that
+contain the covered work, unless you entered into that arrangement,
+or that patent license was granted, prior to 28 March 2007.
+
+  Nothing in this License shall be construed as excluding or limiting
+any implied license or other defenses to infringement that may
+otherwise be available to you under applicable patent law.
+
+  12. No Surrender of Others' Freedom.
+
+  If conditions are imposed on you (whether by court order, agreement or
+otherwise) that contradict the conditions of this License, they do not
+excuse you from the conditions of this License.  If you cannot convey a
+covered work so as to satisfy simultaneously your obligations under this
+License and any other pertinent obligations, then as a consequence you may
+not convey it at all.  For example, if you agree to terms that obligate you
+to collect a royalty for further conveying from those to whom you convey
+the Program, the only way you could satisfy both those terms and this
+License would be to refrain entirely from conveying the Program.
+
+  13. Use with the GNU Affero General Public License.
+
+  Notwithstanding any other provision of this License, you have
+permission to link or combine any covered work with a work licensed
+under version 3 of the GNU Affero General Public License into a single
+combined work, and to convey the resulting work.  The terms of this
+License will continue to apply to the part which is the covered work,
+but the special requirements of the GNU Affero General Public License,
+section 13, concerning interaction through a network will apply to the
+combination as such.
+
+  14. Revised Versions of this License.
+
+  The Free Software Foundation may publish revised and/or new versions of
+the GNU General Public License from time to time.  Such new versions will
+be similar in spirit to the present version, but may differ in detail to
+address new problems or concerns.
+
+  Each version is given a distinguishing version number.  If the
+Program specifies that a certain numbered version of the GNU General
+Public License "or any later version" applies to it, you have the
+option of following the terms and conditions either of that numbered
+version or of any later version published by the Free Software
+Foundation.  If the Program does not specify a version number of the
+GNU General Public License, you may choose any version ever published
+by the Free Software Foundation.
+
+  If the Program specifies that a proxy can decide which future
+versions of the GNU General Public License can be used, that proxy's
+public statement of acceptance of a version permanently authorizes you
+to choose that version for the Program.
+
+  Later license versions may give you additional or different
+permissions.  However, no additional obligations are imposed on any
+author or copyright holder as a result of your choosing to follow a
+later version.
+
+  15. Disclaimer of Warranty.
+
+  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
+APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
+HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
+OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
+THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
+PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
+IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
+ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
+
+  16. Limitation of Liability.
+
+  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
+WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
+THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
+GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
+USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
+DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
+PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
+EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
+SUCH DAMAGES.
+
+  17. Interpretation of Sections 15 and 16.
+
+  If the disclaimer of warranty and limitation of liability provided
+above cannot be given local legal effect according to their terms,
+reviewing courts shall apply local law that most closely approximates
+an absolute waiver of all civil liability in connection with the
+Program, unless a warranty or assumption of liability accompanies a
+copy of the Program in return for a fee.
+
+                     END OF TERMS AND CONDITIONS
+
+            How to Apply These Terms to Your New Programs
+
+  If you develop a new program, and you want it to be of the greatest
+possible use to the public, the best way to achieve this is to make it
+free software which everyone can redistribute and change under these terms.
+
+  To do so, attach the following notices to the program.  It is safest
+to attach them to the start of each source file to most effectively
+state the exclusion of warranty; and each file should have at least
+the "copyright" line and a pointer to where the full notice is found.
+
+    <one line to give the program's name and a brief idea of what it does.>
+    Copyright (C) <year>  <name of author>
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program.  If not, see <http://www.gnu.org/licenses/>.
+
+Also add information on how to contact you by electronic and paper mail.
+
+  If the program does terminal interaction, make it output a short
+notice like this when it starts in an interactive mode:
+
+    <program>  Copyright (C) <year>  <name of author>
+    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
+    This is free software, and you are welcome to redistribute it
+    under certain conditions; type `show c' for details.
+
+The hypothetical commands `show w' and `show c' should show the appropriate
+parts of the General Public License.  Of course, your program's commands
+might be different; for a GUI interface, you would use an "about box".
+
+  You should also get your employer (if you work as a programmer) or school,
+if any, to sign a "copyright disclaimer" for the program, if necessary.
+For more information on this, and how to apply and follow the GNU GPL, see
+<http://www.gnu.org/licenses/>.
+
+  The GNU General Public License does not permit incorporating your program
+into proprietary programs.  If your program is a subroutine library, you
+may consider it more useful to permit linking proprietary applications with
+the library.  If this is what you want to do, use the GNU Lesser General
+Public License instead of this License.  But first, please read
+<http://www.gnu.org/philosophy/why-not-lgpl.html>.
```

### Comparing `msg_explorer-1.6.0/PKG-INFO` & `msg_explorer-1.7.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: msg_explorer
-Version: 1.6.0
+Version: 1.7.0
 Summary: A GUI program to allow for exploring MSG files using extract-msg.
 Home-page: https://github.com/TeamMsgExtractor/msg-explorer
+Download-URL: https://github.com/TeamMsgExtractor/msg-explorer/archives/master
 Author: Destiny Peterson
 Author-email: arceusthe@gmail.com
 License: GPL
-Download-URL: https://github.com/TeamMsgExtractor/msg-explorer/archives/master
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
@@ -95,20 +94,18 @@
 -------
 
 `Destiny Peterson (The Elemental of Destruction)`_ - Main Programmer.
 
 .. |License: GPL v3| image:: https://img.shields.io/badge/License-GPLv3-blue.svg
    :target: LICENSE.txt
 
-.. |PyPI3| image:: https://img.shields.io/badge/pypi-1.6.0-blue.svg
-   :target: https://pypi.org/project/msg-explorer/1.6.0/
+.. |PyPI3| image:: https://img.shields.io/badge/pypi-1.7.0-blue.svg
+   :target: https://pypi.org/project/msg-explorer/1.7.0/
 
 .. |PyPI2| image:: https://img.shields.io/badge/python-3.8+-brightgreen.svg
    :target: https://www.python.org/downloads/release/python-3816/
 .. _Destiny Peterson (The Elemental of Destruction): https://github.com/TheElementalOfDestruction
 .. _Discord: https://discord.com/invite/B77McRmzdc
 .. _Buy Me a Coffee: https://www.buymeacoffee.com/DestructionE
 .. _Ko-fi: https://ko-fi.com/destructione
 .. _Patreon: https://www.patreon.com/DestructionE
 .. _Changelog: https://github.com/TeamMsgExtractor/msg-explorer/blob/master/CHANGELOG.md
-
-
```

### Comparing `msg_explorer-1.6.0/README.rst` & `msg_explorer-1.7.0/msg_explorer.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: msg-explorer
+Version: 1.7.0
+Summary: A GUI program to allow for exploring MSG files using extract-msg.
+Home-page: https://github.com/TeamMsgExtractor/msg-explorer
+Download-URL: https://github.com/TeamMsgExtractor/msg-explorer/archives/master
+Author: Destiny Peterson
+Author-email: arceusthe@gmail.com
+License: GPL
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.8
+Description-Content-Type: text/x-rst
+License-File: LICENSE.txt
+
 |License: GPL v3| |PyPI3| |PyPI2|
 
 msg-explorer
 =============
 
 Allows for the graphical browsing of Outlook Message Files and their data.
 
@@ -77,16 +94,16 @@
 -------
 
 `Destiny Peterson (The Elemental of Destruction)`_ - Main Programmer.
 
 .. |License: GPL v3| image:: https://img.shields.io/badge/License-GPLv3-blue.svg
    :target: LICENSE.txt
 
-.. |PyPI3| image:: https://img.shields.io/badge/pypi-1.6.0-blue.svg
-   :target: https://pypi.org/project/msg-explorer/1.6.0/
+.. |PyPI3| image:: https://img.shields.io/badge/pypi-1.7.0-blue.svg
+   :target: https://pypi.org/project/msg-explorer/1.7.0/
 
 .. |PyPI2| image:: https://img.shields.io/badge/python-3.8+-brightgreen.svg
    :target: https://www.python.org/downloads/release/python-3816/
 .. _Destiny Peterson (The Elemental of Destruction): https://github.com/TheElementalOfDestruction
 .. _Discord: https://discord.com/invite/B77McRmzdc
 .. _Buy Me a Coffee: https://www.buymeacoffee.com/DestructionE
 .. _Ko-fi: https://ko-fi.com/destructione
```

### Comparing `msg_explorer-1.6.0/msg_explorer/__init__.py` & `msg_explorer-1.7.0/msg_explorer/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-#!/usr/bin/env python
-# -*- coding: latin-1 -*-
-# Date Format: YYYY-MM-DD
-
-"""
-msg-explorer:
-    A GUI program to explore the contents of an MSG file using extract-msg.
-
-https://github.com/TeamMsgExtractor/msg-explorer
-"""
-
-# --- LICENSE.txt -----------------------------------------------------------------
-#
-#    Copyright 2022 Destiny Peterson
-#
-#    This program is free software: you can redistribute it and/or modify
-#    it under the terms of the GNU General Public License as published by
-#    the Free Software Foundation, either version 3 of the License, or
-#    (at your option) any later version.
-#
-#    This program is distributed in the hope that it will be useful,
-#    but WITHOUT ANY WARRANTY; without even the implied warranty of
-#    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#    GNU General Public License for more details.
-#
-#    You should have received a copy of the GNU General Public License
-#    along with this program.  If not, see <http://www.gnu.org/licenses/>.
-
-__author__ = 'Destiny Peterson'
-__date__ = '2023-02-27'
-__version__ = '1.6.0'
-
-# When this module is imported, we should try to compile the forms. They only
-# compile when they are outdated.
-from ._recompile import compile as _compile
-
-
-_compile()
+#!/usr/bin/env python
+# -*- coding: latin-1 -*-
+# Date Format: YYYY-MM-DD
+
+"""
+msg-explorer:
+    A GUI program to explore the contents of an MSG file using extract-msg.
+
+https://github.com/TeamMsgExtractor/msg-explorer
+"""
+
+# --- LICENSE.txt -----------------------------------------------------------------
+#
+#    Copyright 2022 Destiny Peterson
+#
+#    This program is free software: you can redistribute it and/or modify
+#    it under the terms of the GNU General Public License as published by
+#    the Free Software Foundation, either version 3 of the License, or
+#    (at your option) any later version.
+#
+#    This program is distributed in the hope that it will be useful,
+#    but WITHOUT ANY WARRANTY; without even the implied warranty of
+#    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+#    GNU General Public License for more details.
+#
+#    You should have received a copy of the GNU General Public License
+#    along with this program.  If not, see <http://www.gnu.org/licenses/>.
+
+__author__ = 'Destiny Peterson'
+__date__ = '2023-05-24'
+__version__ = '1.7.0'
+
+# When this module is imported, we should try to compile the forms. They only
+# compile when they are outdated.
+from ._recompile import compile as _compile
+
+
+_compile()
```

### Comparing `msg_explorer-1.6.0/msg_explorer/_recompile.py` & `msg_explorer-1.7.0/msg_explorer/_recompile.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-import os
-import pathlib
-
-
-def compile():
-    # Now, the function we need to call will, unfortunately, try to exit python because
-    # it was written thinking no one would try to run it in a script (foolish). We are
-    # going to briefly override the sys.exit function so that the call to exit does
-    # nothing, then restore the function afterwards.
-    import sys
-
-    lastCode = [0]
-    def __dummyExit(code : int):
-        """
-        Dummy exit function that will store the code into lastCode.
-        """
-        lastCode[0] = code
-
-    __tempExitStore = sys.exit
-    sys.exit = __dummyExit
-
-    # Now that we have replaced the function, let's call the compile calls.
-    from PySide6.scripts.pyside_tool import qt_tool_wrapper
-
-    programPath = pathlib.Path(__file__).resolve().parent / 'ui'
-    for uiFile in programPath.glob('*.ui'):
-        source = os.fspath(uiFile)
-        output = os.fspath(uiFile.with_name(f'ui_{uiFile.stem}').with_suffix('.py'))
-        # Check if the file even needs to be compiled in the first place.
-        if not os.path.exists(output) or isNewer(source, output):
-            qt_tool_wrapper('uic', ['-g', 'python', source, '-o', output], True)
-            if lastCode[0] != 0:
-                raise Exception(f'Failed to compile "{uiFile.name}".')
-
-    # Finally, restore the exit call.
-    sys.exit = __tempExitStore
-
-def isNewer(firstFile, secondFile):
-    """
-    Checks if the first file is newer than the second file.
-    """
-    return os.path.getmtime(firstFile) > os.path.getmtime(secondFile)
+import os
+import pathlib
+
+
+def compile():
+    # Now, the function we need to call will, unfortunately, try to exit python because
+    # it was written thinking no one would try to run it in a script (foolish). We are
+    # going to briefly override the sys.exit function so that the call to exit does
+    # nothing, then restore the function afterwards.
+    import sys
+
+    lastCode = [0]
+    def __dummyExit(code : int):
+        """
+        Dummy exit function that will store the code into lastCode.
+        """
+        lastCode[0] = code
+
+    __tempExitStore = sys.exit
+    sys.exit = __dummyExit
+
+    # Now that we have replaced the function, let's call the compile calls.
+    from PySide6.scripts.pyside_tool import qt_tool_wrapper
+
+    programPath = pathlib.Path(__file__).resolve().parent / 'ui'
+    for uiFile in programPath.glob('*.ui'):
+        source = os.fspath(uiFile)
+        output = os.fspath(uiFile.with_name(f'ui_{uiFile.stem}').with_suffix('.py'))
+        # Check if the file even needs to be compiled in the first place.
+        if not os.path.exists(output) or isNewer(source, output):
+            qt_tool_wrapper('uic', ['-g', 'python', source, '-o', output], True)
+            if lastCode[0] != 0:
+                raise Exception(f'Failed to compile "{uiFile.name}".')
+
+    # Finally, restore the exit call.
+    sys.exit = __tempExitStore
+
+def isNewer(firstFile, secondFile):
+    """
+    Checks if the first file is newer than the second file.
+    """
+    return os.path.getmtime(firstFile) > os.path.getmtime(secondFile)
```

### Comparing `msg_explorer-1.6.0/msg_explorer/app_icons.py` & `msg_explorer-1.7.0/msg_explorer/app_icons.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,1784 +1,1784 @@
-# Resource object code (Python 3)
-# Created by: object code
-# Created by: The Resource Compiler for Qt version 6.3.0
-# WARNING! All changes made in this file will be lost!
-
-from PySide6 import QtCore
-
-qt_resource_data = b"\
-\x00\x00l\xf5\
-\x89\
-PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
-\x00\x04\x00\x00\x00\x04\x00\x08\x06\x00\x00\x00\x7f\x1d+\x83\
-\x00\x00\x01\x84iCCPICC prof\
-ile\x00\x00(\x91}\x91=H\xc3P\x14\x85O\
-S\xb5\x22\x15\x07\x8b\x888d\xa8N\x16\xa4\x8a8J\
-\x15\x8b`\xa1\xb4\x15Zu0y\xe9\x1f4iHR\
-\x5c\x1c\x05\xd7\x82\x83?\x8bU\x07\x17g]\x1d\x5c\x05\
-A\xf0\x07\xc4\xd1\xc9I\xd1EJ\xbc/)\xb4\x88\xf1\
-\xc1\xe5}\x9c\xf7\xce\xe1\xbe\xfb\x00\xa1Qa\xaa\xd95\
-\x09\xa8\x9ae\xa4\xe211\x9b[\x15\x03\xaf\xe8A\x10\
-CTQ\x89\x99z\x22\xbd\x98\x81\xe7\xfa\xba\x87\x8f\xef\
-w\x11\x9e\xe5}\xef\xcf\xd5\xaf\xe4M\x06\xf8D\xe29\
-\xa6\x1b\x16\xf1\x06\xf1\xcc\xa6\xa5s\xde'\x0e\xb1\x92\xa4\
-\x10\x9f\x13O\x18\xd4 \xf1#\xd7e\x97\xdf8\x17\x1d\
-\x16xf\xc8\xc8\xa4\xe6\x89C\xc4b\xb1\x83\xe5\x0ef\
-%C%\x9e&\x0e+\xaaF\xf9B\xd6e\x85\xf3\x16\
-g\xb5Rc\xad>\xf9\x0b\x83ym%\xcdu\xaaQ\
-\xc4\xb1\x84\x04\x92\x10!\xa3\x862*\xb0\x10\xa1]#\
-\xc5D\x8a\xcec\x1e\xfe\x11\xc7\x9f$\x97L\xae2\x18\
-9\x16P\x85\x0a\xc9\xf1\x83\xff\xc1\xef\xd9\x9a\x85\xa9\xa8\
-\x9b\x14\x8c\x01\xdd/\xb6\xfd1\x06\x04v\x81f\xdd\xb6\
-\xbf\x8fm\xbby\x02\xf8\x9f\x81+\xad\xed\xaf6\x80\xd9\
-O\xd2\xebm-|\x04\x0cl\x03\x17\xd7mM\xde\x03\
-.w\x80\xe1']2$G\xf2S\x09\x85\x02\xf0~\
-F\xdf\x94\x03\x06o\x81\xbe5wn\xads\x9c>\x00\
-\x19\x9a\xd5\xf2\x0dpp\x08\x8c\x17){\xdd\xe3\xdd\xbd\
-\x9ds\xfb\xf7Nk~?\x8d\xf4r\xb2n\xdbA\xed\
-\x00\x00\x00\x06bKGD\x00\xff\x00\xff\x00\xff\xa0\xbd\
-\xa7\x93\x00\x00\x00\x09pHYs\x00\x00.#\x00\x00\
-.#\x01x\xa5?v\x00\x00\x00\x07tIME\x07\
-\xe6\x06\x0c\x164\x09\x13\x02\x8c\xb6\x00\x00\x00\x19tE\
-XtComment\x00Create\
-d with GIMPW\x81\x0e\x17\x00\
-\x00 \x00IDATx\xda\xec\xdd{\x945{Y\
-\x1f\xf8\xa7v\xf7\xbe\xf59\x07\x12\x0dF\xcd\x1aoY\
-\x12MFg&\xa0\x06f\x82\xb8&j0\x01G\xc5\
-\xe88\x07\xc5\x83\x198G\x89G\x04\x81\x80\x06\x14\x13\
-\x1c\xd0(\x11\x97\xc9\x8c\x97\x19p\xbc\x1eB\x1c\x5c.\
-\xb9\xa9\xb3\xe2(\x8e\xb7\xc5A.\x19\xc6dn\xca-\
-\x84s\x80\xee\xde\xbb\xbbw\xcd\x1fU\xf5\xee\xdd\xfd\xf6\
-e_\xaajW\xed\xfa|\xd6\xeau\xb8\xbc\xe7}\xf7\
-[\xbd{W=\xdf\xfa\xd5\xf7\x17\x01\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\xd0\x04\xc9\x96\xff\xfc\
-\xcf\x8d\x88'GD\xcf\xb7\x02\x00\x00\x80\x0d=*\x22\
->\xd8\xd0\xd7v\x1c\x11?\xbc\xcd\x17\xb0\xbf\xe5\x03\xf0\
-S\x11\xf1E\xde\xa3\x00\x00\x00\xec\xb84\x22>?\x22\
-\xee\xe9j\x00\xf0I\xf9?\xcf\x22bo\xc3\xdf\xeb$\
-\xff}F%\xbe\xbe\xa3\x88\x187\xe8\x0ds\x16\x11\xb3\
-\xfc?\xcf\xf27P,\xfc3\xc9\xffs\x12\xe7Ww\
-\xf4\x16~}\xb2\xf0\xef\xf7n\xf8\xcf\xc5\xaf\xef-\xfc\
-\xb9\xc5\xff\x9e.\xfcy\x8b\x7fvo\xe1\xdf\xef\x95\xf0\
-}\x05\x00\x00Xe\x86\xeb\xe7sHY+\xde\xcb\x98\
-W\x8b9\xea?\xde\xe6\xc1\xd9v\x00p\x96\x1f\x842\
-\x0e\xe8i\x94\xffHC\xda\xb07\xf3^\xcb\x07\xea\xb3\
-\xfc+Y\xf8\xdeG\xdc\x1c`\x5c\x164,\x1b`\xf4\
-.\xf9>.\x1b`\xb4\xfdx\x03\x00@\xd7\xa4\xf9\x9c\
-;\x8d\x88\x81\xc3\xd1\xac\x00\xe04\xffg/\x22\x0e#\
-\xe2`\xc3\xdfo\x14\xcd\xbbk\xcf\xdc\xe2@\xddo\xd9\
-k_\x0c/\x8a\xff\xbel\x80\x11\x17\xfe\xf7e\xc3\x8c\
-\xcb\x02\x8c\xc5\xf0\xe2\xb2?{1\xc0\xd8\x0f\xfd\x1a\x00\
-\x00tSb6l^\x00p\xb6\xf0:N/\x0c6\
-\x9b|\xa3\xa1l\x17W\x03\xb49\xc0X\x0c/.\x0b\
-\x11\xae\x0b0\x22\xe6!\xc5Ma\xc6M\x01Fz\xe1\
-g\xf6b\x80\xd1\xf7\xf3\x0c\x00\xc0\x9a\xfa\xf9u\xefi\
-\x09s\xef\xce\x5c\x93n;\x008Y\xf8\xcf\xa3\x88\x98\
-D\xc4p\xc3\xdf\xd3*\x00\xb8]\x9bW_D,\xf7\
-\xf8H\xc4j\x01\xc6\xe2\x7f\xbe,\xccH\xf3c\xb6N\
-\xffEq\x9c\x05\x18\x00\x00\xdb3\x8a\xecQ\x00\x1a\x12\
-\x00\x5c|n?\x89lk\x842\x8a\xfc\xcaXM\x00\
-4C\x17\x02\x8c\xab\xc2\x8b\x8b\x9fg7\xf5_,\x86\
-\x13\xeb\x16x\xea\xbf\x00\x00vE?\xca\xb9\xd1,\x00\
-(iH_4\xc8\x03\x80M\x8dK\x0c\x12\x006\xd5\
-\xd5\x00c\x93\x1dH\x8a0C\x80\x01\x00l\xa2\xb8\x06\
-\xb1J\xbc\x01\x01\xc0e\xcaz\x14\xe0\xe2\x05%\x00\xeb\
-Q\xe0Y\xef\x0e$\x0a<\x01\xa0\x5c\xc3\xc8n\x10w\
-~\x95\xf8~C_WZB\x08Pf\x90\x00@;\
-)\xf0\xbc\xba\xc0\xd3\x0e$\x00tI\xd1\x07\xd0\xe9\xad\
-\x01\xf7\x1b\xfc\xcd\x99\x94\x14$\x9c6\xf8\xef\x09\x00\xd7\
-Q\xe0\xb9\x5c\x81\xe7\xc5\x00c\xd9\x02\xcf\xe2\xff\xb3\x03\
-\x09@7\xf4\xa2\xe3\x8f\x024y0\x1e\x94\xf0\xcd\xd1\
-\xfa\x08\x00\xdb\xa3\xc0s\xf5\x02\xcfMw \x19x\xdb\
-\x01\x5c;\xff\x9eF\x87o\x127\xf9/]\x9c0O\
-6\xbchHK\xf8=\x00\x80\xeeQ\xe0\xb9z\x81g\
-\x12v \x01\x9a\xadXm.\x00h\xa0ql~\x07\
-\x7f\x18V\x01\x00\x00\xdd\xd3\xf5\x00c\xf1\xd7\xd4Q\xe0\
-)\xc0\x80\xf6\x18\xc4j}q\xa9\x00\xa0\xde\xd7X\xc6\
-s\x1a\xb6\x05\x04\x00h\x0f;\x90\x9c\x7f4\xe4\xa6\xd5\
-\x18\x0a<ay\xc9\x1a3\xe2N\xec \xd0\x86\x00`\
-q/\xe8u?\x94\x06a\x15\x00\x00\x00\xf5\xb0\x03\xc9\
-\xd5;\x90\x5c\x15f\xdc\x14`(\xf0\xa4l\xabn\x0d\
-8\x8b\x1dX\xe5\xd3\x96\xe7\x1e\xca\xd8\xb2\xa1\xf3\x8d\x8f\
-\x00\x00\xb0\x04;\x90,\xb7\x03\xc9bh\xb1i\x81\xa7\
-\x00\xa3\xf9s\xe6\x99\x00\xa0^\xc9\x86\x03\xfc~\xfeM\
-\x03\x00\x00v\x97\x1dHV\xdf\x81$\xa2\xbb\x05\x9e\xbd\
-X\xeeQ\x80\xd9.\xfcp\xb4)\x00\xe8/\xfc\x00$\
-\x1b\xfc\x1eK\x87\x08\xa3a\xff\xe0xr\xe2#\x14\x00\
-\x00\xa8K\xdb\x03\x8c\xadZc\x86+\xb6\x06\xbcn\xe7\
-\xb8\x22\x0c\x11\x00\xd4\xfd\xfd\x8c\xd5\xda\x1a/\xea\xad\x12\
-\x1e$\xf9/=\x18\x0f\xe3\x8b\xfe\xd3\xcf\x8e\xff\xec\xaf\
-~V\xf4\xf7\x95\xbb\x02\x00\x004\xc1\xc9\xe9Y\xfc\xe1\
-;\xff$\xde\xf6G\xffG\x1c\x1eMn\xcdpk\xcc\
-\x99\xd7u\xc6\x09\x00\xb6l\x93F\xffa,\xb9\x0a\xe0\
-h2=\x8c\x88\x83\xfd\xbd^\xfa\xeb\xbf\xfd\x8e\xe4\xed\
-\xef\xfa\xbf\xe2\xdb\xbe\xf1I\xf1\x9c{\x9e\x1c\x8f\xb8\xf3\
-\xc0O\x1b\x00\x00\xc0\x16\x1c\x1eM\xe2\xbf\xff\xf97\xc7\
-\xcb\x7f\xfcu\xe9\xfb>\xf4\x91\xe4\x91w\x1d\xa4\x11\x91\
-\x143\xdc\x1a\xbf\xe5u[\x03\xee\xc4\x0e\x00\xd1\x80\xbf\
-\xc4\xefF\xc4\x17\x94\x14\x00\xac\xd2\x0f\xb0l\x80p\xee\
-\xcd\xf3\x88;\xc7\xe9\xc3\x1f;J>\xf1\xcf\xdd%\x08\
-\x00\x00\x00h\xc0\xe0\xff\xd0G\x0f\x93\xabf\xb8\x15M\
-\x22{\xd6\x7f|\xc9\xfc\x98\xc6\xe6\x85\xf2\xb3\x88\xf8\xfd\
-\x88\xf8B\x01\xc0\xe6!\xc0\xaa\x05\x81\xcb\xfc\xfaK\xdf\
-<\x0bA@\xfam\xdf\xf8\xa4D\x10\x00\x00\x00\xb0\xd5\
-\xc1\xbf\x8c\x00\xa0\x08\x01\xfaq~\x97\x86\xe3\xfc\x9f\xa3\
-\x0d\xff\x1a\x02\x80\x0d\x02\x80I\xfe\xcf\xe1\x9a\x01\xc02\
-\xab\x00\xae{\xf3\xa4\x8f\xb8s\x1c\x82\x00\x00\x00\x80\xad\
-\x0f\xfee\x05\x00\x11\xb7o\x0dx\x94\xcf\xce\x02\x80\x92\
-\x02\x80u\x9f\xa9\x98l\x10\x00,\x13\x02,\xf3\xe69\
-y\xc4\x9d\xe3\xfe\xc3\x1f;\x0aA\x00\x00\x00\xc0V\x06\
-\xff2\x03\x80\xb3<\x04\x18\x0b\x00\xaa\x09\x00Nc\xbd\
-B\xc2Y\x1e\x02\x8c7\x08\x00\x06q~y\xc7\xbao\
-\x9e\xe9#\xee\x1c\x0f\x04\x01\x00\x00\x00\xb5\x0f\xfee\x06\
-\x00\xc5\xac\xd8\xcb\xe7\xc5\xa3\xfc\x7f\xd3\x01PR\x00p\
-\xdd\x9e\x8b\xcb|c\xf6\xf3\xdfc\xbc\xe6\xbf?*\xf1\
-\xcd3\xc9\x83\x00\x8f\x06\x00\x00\x00\xd43\xf8\x97\x1d\x00\
-D\xccW\x9c\x0b\x00J\x0c\x00\x1e\x9b\x0f\xef\x83\x0d~\
-\x9fi~0\xd7Y\x92q\x9c\x87\x0f{%\xbey\xd2\
-\x98\xaf\x08\x10\x04\x00\x00\x00T;\xf8W\x11\x00\x14!\
-\xc0L\x00\xd0\xac\x00`\x96\xff]\x92\x0d\xbe\xa9\xc3\x0a\
-\xde<g\x91\x95\x05\xee\x09\x02\x00\x00\x00*\x1b\xfc\xab\
-\x0a\x00N\x22{\x14`*\x00(/\x008\x8d\xf5\x1f\
-\x01\xb8h\x9dB\xc1\xe3\xc8V\x00\xf4+z\xf3L\x22\
-bO\x10\x00\x00\x00\x18\xfc+\x19\xfc\xab\x08\x00\x16g\
-\xcb\xabn\x1a\xb7*\x00\xe8\xed\xd2\x9b\xe9\x9b\xbf\xfe\xc9\
-q\xd7|\xa0NW\xf8WG+\xfe\xfaU\x0d#b\
-\xff\xe1\x8f\x1d\x1dE\xc4\xf4\xe4\xf44y\xe9\xab~!\
->\xeb\x89\xf7\xa5/y\xd5\xcf\xc7\xc3\x1f;\xf4I\x00\
-\x00\x00\xec\xf4\xe0\xff#?\xfd+\xf1\x97\xbf\xe4\xbe\xf4\
-\xfe\x97\xfdd\x1cM\xa6\x11\x11Q\xf2\xf0_\x964\x22\
-b<\x1a\xc6S\x9f\xfc_\xee\xd4\xf7\xa1)\x01@)\
-\xdf\xf4\xa7\xfc\xed/\x8e\xf7\xbd\xe3\x8d\xc9\x0f\xbe\xf4\xfe\
-u\x83\x80I\xc5\x7f\xcf\x83\x88\x18,\x04\x01!\x08\x00\
-\x00\x00\x0c\xfe\xcd\x1a\xfc_t\xff=\xf1\xbew\xbc1\
-\xf9o\xbe\xe6I\xa5\xce\xac\x02\x80\x92\x0f\xe6\xc1x\x14\
-\xcfy\xd6\xdd\xeb\x04\x01\x83\x1a\xff\xbe\xe3\xc8V\x04\x9c\
-D\xc4\x89 \x00\x00\x000\xf87g\xf0\x7f\xd9\x0b\xef\
-\x8bG\xdcu\xc7\xce}_zM9\xd8e[3\x08\
-\xe8E\xd6\x07P\xd7\xb1\x1fDD\xfa\xf0\xc7\x8e\xa6\x11\
-q*\x08\x00\x00\x00\x0c\xfe\x06\xff]\x0e\x00*\xb5b\
-\x10\xd0\x8f\xfa\x97v\x0c\x22\xeb\x088\xcd\x83\x80t1\
-\x08\xf8\x81\x7f\xfe/\xe3\xf0h\xe2\x93\x04\x00\x00h\xac\
-\xc9\xf4$\xfe\xc5\xcf\xbdi\x97\x07\xfft\x17\xbeO\xbd\
-\xae\xbc!W\x08\x02\xf6\x22\xe2h\x0b/q\x94\x07\x01\
-\xc7\x0f\x7f,\x9b\xf8ONO\xe3\x05\xafxm|\xda\
-\xdf|\xa6 \x00\x00\x00h\xec\xe0\xff\x19OxV\xfa\
-\xcc\x17\xff\xb8;\xfe\x02\x80\xd6\x05\x01\xfb[>.\xe3\
-<\x0c8\x12\x04\x00\x00\x00\x06\xffF\x0c\xfe;1;\
-\xf7\xba\xfa\x86\xbd!\x08\x18D\xc4\xc9\x96_\xe28\xb2\
-G\x12&\xf9\xa3\x01\x82\x00\x00\x00\xc0\xe0_\xef\xe0_\
-\xb0\x0b\xc0\xae\x05\x01\xafx\xc9\xfdq\xe7\x1d\x07\xc57\
-\xb7\x9f\x7fm\xd3^d\x8f\x05D\x1e\x04\x9c\x09\x02\x00\
-\x00\x00\x83\xff\xb53\xd4\xadY\xefE\xdf\xf1\x8cN.\
-\xf5\x17\x00,\x11\x04<\xf7\xde\xbb\xe3\xfd\x7f\x9c\x05\x01\
-\xe3\xf10\xf2\x00\xa0\x09e\x0f\xc3\xfc\xeb$\x0f\x02B\
-\x10\x00\x00\x00\x18\xfc\xcfI#b8\x1e\x0d\xd3\x17}\
-\xc73\xe2\xcf\x1e\xfc\xb5\xe4e/\xb8\xb7\xac\xc1\xdf#\
-\x00\xbb\x1c\x04|\xe8]o\x89W\xfc\xa3o_v\xfb\
-\xc0\xba\x8c\xf3 \xe08\xb2\xb2\xc0D\x10\x00\x00\x00\x18\
-\xfc#\x06\xfd\xfd\xe4\x05\xff\xe0\xe9\xd9\x1d\xff\xf2\x06\xff\
-\x9d\x22\x00\xb8.\x08\xb8\xefi\xcbn\x1f(\x08\x00\x00\
-\x00\x0c\xfe[\x18\xfc\x87\x83A\xf2\xa2\xfb\xef\x89\x0f\xbe\
-\xeb-\xf1O^\xf4mU\x0d\xfeI\xec\xc0V\x80\x02\
-\x80%\x82\x80%\xb7\x0f\xac[\x12\xd9n\x01{\x111\
-\x89\x88\xa9 \x00\x00\x00\xd8\xf1\xc1\x7fV\xccb\xa3a\
-6\xf8\x7f\xe0\x9do\x8a\x1a\x9e\xf1O\xf2?[\x00P\
-\x82\xc6')\x0d\x0e\x02\xfa\x91\xad\x06\x98E\xc44\x22\
-f\x82\x00\x00\x00`\xc7\x06\xffi>{\xf5\x8aV\xff\
-\xf7\xffq-\x83\xffb\xf0p&\x00\xe8\x98\x06\x07\x01\
-\xa3\xc8\xb6/\x9c\xe4_!\x08\x00\x00\x00Z>\xf8\x17\
-\xc3\xcb`\xbc\xddV\xff4\xac\x00(\xf5`\x0a\x02\xca\
-Q\xf4\x03\x1cF\xc4\x91 \x00\x00\x00h\xd9\xe0\x9f\xe6\
-\x83\xff\xbc\xd5\xff\xfe{\xe2}\xe5\xb6\xfa\xaf\xf3\x9at\
-\x00t5\x00hA\x10p\x90\x07\x01\xd3\xb8bE\xc0\
-\xa7?A\x10\x00\x00\x00]\x1a\xfc?\xf3\x8b\xefm\xf2\
-\xe0\x7f\x1a\xf3;\xfe\xc3b\xa9\xff\x96\xee\xf8\xef\xd4\xdc\
-\xda\xb4\x00 i\xfb\x81lh\x10\xd0\x8b\xec\xb1\x80$\
-\x0f\x02N\x17\x83\x80\xe9\x89 \x00\x00\x00\xba4\xf8\x1f\
-\x1eO\x9a8\xf8\x1f\xe7\xf3\xca^C\x07\xffb\xaek\
-\xfd\xdcj\x05@7\x82\x80A\xfeu\x12Y\xa26\x13\
-\x04\x00\x00\x80\xc1\x7f\xcb\x0e\xf3\x19e\x18\x11\x83\x86\x0e\
-\xfe;5\xb3\xf6\x1c\xd0N\x05\x01E?\xc0\xad\xa2@\
-A\x00\x00\x00\x18\xfck4\x8b\xac\xabl\x12\xd9c\xcb\
-\xfd\x86\x0f\xfe\x8b\xac\x00(\xf1@\xcev\xf1\x07\xb0\xe1\
-A\xc0q\xfe%\x08\x00\x00\x00\x83\x7f\x95\xa6\xf9\xecq\
-\x1a\xd9\x0ef\xf3r\xbf\xe6\x0f\xfe;C\x00\xd0\xed \
-`\x14\x11\xfd\xb0\x22\x00\x00\x00\x0c\xfe\xd58\xcc\x87\xff\
-^\xb4c\xa9\xbf\x00\xa0\x06{\xb1c\x8f\x00\xb4(\x08\
-\xd8\xcb\x7f\x10#\x0f\x01N\x05\x01\x00\x00`\xf0/a\
-\xf0?\x8el\xf5q?\x22\xf6[>\xf8\xdb\x06\xb0D\
-I\xd7~`\x1b\x18\x04\x0c\xf3\xaf\xa2(0\x04\x01\x00\
-\x00`\xf0_\xc1Y>K\x1c\xc7|[\xf2\xc4\x1d\x7f\
-\x01\x00\xcd\x0d\x02\x8a~\x80\xa3\xfcK\x10\x00\x00\x00\x06\
-\xff\xeb\x14\xdb\xf8\x9d\xc6\xfc\xc6b\x18\xfc\x05\x00\xd7I\
-\xba\xfc\x8dhh\x100\xca\x7f\x98\xad\x08\x00\x00\x00\x83\
-\xffEG\xf9\xe0\xbf\x1f\xf3\xad\xc7\x0d\xfe\x02\x00Z\x1a\
-\x04$y\x08\xd0\xcbC\x80\xa9 \x00\x00\x00:=\xf8\
-\x17\xdb\xf8\x1d\xe7\xb3\xc2 \xb2^1\x83\xbf\x00`\xe5\
-a\x93f\x06\x01\xfd\xc8\x96\xf1\xcc\xf2 `&\x08\x00\
-\x00\x80N\x0d\xfe\xc56~\x93\x98\xaf\x16\x0e\x83\xbf\x00\
-\x80\xdd\x0d\x02Fy\x10pn\xdb@A\x00\x00\x00\xec\
-\xec\xe0\x7f\x9c\x7f\x15\xf3\xc0\xb8\x98E:6\xf8'\xb1\
-\x037\xad\xad\x00\x10\x04\xac\xa3(\x0a\x5c\xfc0\x10\x04\
-\x00\x00\xc0\xee\x0c\xfe\xc52\xffA\xcc\x97\xfawq\xf0\
-\xdf)V\x00\x08\x026Q|\x10L\x04\x01\x00\x00\xd0\
-\xfa\xc1\x7f\xf1\xf9\xfeb\x99\x7f\xcf\xe0/\x00\xa8\x82\x15\
-\x00\xed\x0c\x02z\x91\xad\x06\xe8\xc5|\xeb\x0fA\x00\x00\
-\x00\xb4g\xf0/\x9e\xef?\x89\xf3\xcf\xf7\x1b\xfc\xe7\xd2\
-]\xf8KX\x01 \x08(K\xb1\xed\xc7i\xfe\x01\x92\
-\x0a\x02\x00\x00\xa0\xd1\x83\xffQd\xaby\x8b\xdd\xbf\x86\
-\x06\xff\xdd\x9e\x9f\x05\x00\x82\x80\xb2\x15\x8f\x05\x14K\x87\
-B\x10\x00\x00\x80\xc1\xbfQ\x83\xffa~\xad>\xcc\xbf\
-\xfa\x06\xffn\x10\x00\x08\x02*{)y\x18p,\x08\
-\x00\x00\xc0\xe0\xbf\xf5\xc1\xfft\xe1\xda\xbc\xb8V\xef\x19\
-\xfcWb\x17\x00\x04\x017\x18E\x96(N\xf3/A\
-\x00\x00\x00\x06\xff\xfa\x1c\xe7\xd7\xe1g\xf9\xb5\xf9h\xe1\
-\xff3\xf8wh\xf8\x17\x00\x08\x02\xea\xb2\x17\xf3mC\
-&\xf9\x87\x8f \x00\x00\x00\x83\x7fu\x0e\xf3k\xef\xfd\
-\xfcZ|h\xf0\xdfxv\xd6\x01\x80 `\x05\xc53\
-F\x93\xfc+\x04\x01\x00\x00\x18\xfcK3\x8b\xf92\xff\
-q~\xed\xbdo\xf0/mv\xf6\x08@\x89R\xef\xa9\
-\xce\x04\x01\x07\xf9\x87\xd1\x95E\x81\x82\x00\x00\x00\x0c\xfe\
-K+\xb6\xf1\x9b\xc4|\x99\x7fb\xf0\xaf$\x00H\xdb\
-\xfe\x97@\x10\xb0\xad `\x1c\xd9r\xa4cA\x00\x00\
-\x00\x06\xff\x95\x1d\xc5\xbcgk\x94__\x87\xc1\xbf2\
-\xb3\xfcK\x00P\x02+\x00\xba\x19\x04\xf4\xf2\x0f\xab\xbd\
-\xc8\x12\xcb\x13A\x00\x00\x00\x06\xff\x1b\x07\xffb\x1b\xbf\
-A\xfee\xf0\xaf\xc7\x99\x00@\x00 \x08\xd8\x5c?\xff\
-\x00;\xcb\x83\x80\x99 \x00\x00\x00\x83\xff\xb9\xc1\xb3\x18\
-\xfc\xc7q~\x1b?\x83\x7f=\xac\x00@\x10P\xb2Q\
-\xcc\x8b\x02\x8f\xaf\xfb\x85\x82\x00\x00\x00:0\xf8\x17\xcf\
-\xf7\x9f.\x0c\xfea\xf0\xdf\x1a\x1d\x00\x0e\xa4 \xa0\x02\
-\xc5\x87\xdb\xd1\xeaA\xc0\xb3\x04\x01\x00\x00\xb4}\xf0?\
-\x8a\xec\xa6X\x12\xf3\x9bd\x06\xff\xed\xcf\xac\x02\x00\x01\
-\x80 \xa0\xe2 \xa0\x1f7l\x1dx>\x088\x11\x04\
-\x00\x00\xd0\xd6\xc1\x7f\xb1\xcd\x7f\x98_\x0b\x1b\xfc\x9b3\
-\xb3\xb6z+\xc0\xa6=\x020\xf3\x9e\x12\x04\x5cb/\
-\xe6\x89\xe7$\xb2\xe5O\x82\x00\x00\x00ve\xf0?\x8d\
-\xf9\xca\xd7b\xf0O\x0c\xfe\xecr\x00\x90D\xcb\x1b\x15\
-\x05\x01\x95\x1b\xe6_\xa7\x91=\x0b\x95\x0a\x02\x00\x00h\
-\xf1\xe0_l\x87}\x16W?\xdfo\xf0o\x16+\x00\
-J\xe41\x00A\xc02F\x91muR|`\x86 \
-\x00\x00\x80\x16\x0d\xfe\x87\x91\xadl\xdd\x8f\xab\x9f\xef7\
-\xf87O\xebW\xac7)\x00\xd8\x13\x00\x08\x02V4\
-\xce?,o,\x0a\x14\x04\x00\x00\x18\xfc\xb7<\xf8\xcf\
-\xf2\xeb\xd6\xa3\x888\xc8\xafc\xf7\x0d\xfet5\x00\xb0\
-%\xa1 `\x1dI\xcc\x8b\x02\xa7\xf9\x97 \x00\x00\x80\
-\xa6\x0c\xfe\xd3\xc8\xee\xf6O\xf3\xeb\xd6\xf15\xbf\xd6\xe0\
-\xdf|v\x01(q\x90C\x10\xb0\xae\xbd\xc8\x1e\x0bH\
-\xf3\x0f\xd7\x1b\x97\xe7\x08\x02\x00\x00\x0c\xfe\x15:\x8c\xf9\
-\xcd\xa9a\x5c\xfd|\xbf\xc1\x9fN\x06\x00B\x00A@\
-\x19\x86\xb1B?\x80 \x00\x00\xc0\xe0_\xb2\xa3\x98o\
-\xe37\xc8\xbf\x0c\xfe\x08\x00\x04\x00\x82\x80*\xff\xe8\xfc\
-Cw\xa9~\x00A\x00\x00\x80\xc1\x7f\x03g1\x7f\xbe\
-\xbf\xe8\xa9\xea\x19\xfc\x11\x00\x08\x00\x04\x01\xf5\x06\x01\xe3\
-\xc8R\xd7\xe2\xd9+A\x00\x00\x80\xc1\xbf,\xc7\xf9u\
-\xe6I\xdc\xfc|\xbf\xc1\x1f\x01\x00\x82\x80\x1a\x82\x80^\
-\x1e\x02$1/`\x11\x04\x00\x00\x18\xfc\xd7U,\xf3\
-/z\xa8F\x06\xffNh\xfd\x0dk+\x00\xe8R\x10\
-0\x88l9\xd6,\xff\xc0^j\x1fOA\x00\x00\x80\
-\xc1?\xbfN-\x1e/\x1d\xe5\xd7\x95}\x83\xbf\x10@\
-\x00\x00\xcd\x0e\x02\x8a\x0f\xecI,\xd9\x0f \x08\x00\x00\
-\xe8\xec\xe0\x7f\x96_7N\x22[\xe2?Zb\x084\
-\xf8\xef\xa6T\x00P.+\x00\x04\x01u\x06\x01\xc5\x07\
-\xf8\xd2E\x81\x82\x00\x00\x80\xce\x0c\xfe\xc5\xaeRgq\
-\xf36~\x06\xff\xee\x10\x00\xc0\x0e\x04\x01\xfd\x98'\xbb\
-\x82\x00\x00\x80\xee\x0e\xfe\xc5\xcd\xa1~\xcc\xb7\xf23\xf8\
-S|\x9f\x05\x00\xb0\x03A\xc0^d\xc9n\xe4!\xc0\
-\xa9 \x00\x00\xa03\x83\xff,\xceo\xe37\xca\xaf\x0f\
-\x0d\xfe\xec\x14\x8f\x00 \x088o\x98\x7f\x9d\xe4A\xc0\
-\xd2\x7f\x8e \x00\x00\xa0u\x83\xff4\xe6[\xf9-\xb3\
-\x8d\x9f\xc1\xbf\xdb\xec\x02P\xb2\xd4{\x8a\x86\x04\x01\xe3\
-<\x08(\x9e\xfdZ\x9a \x00\x00\xa0\xf1\x83\xffa\xcc\
-\xb7\x86\x1e\xc5r\xcf\xf7\x1b\xfc\xe9\x85G\x00@\x10 \
-\x08\x00\x00h\xcd\xe0_l\xe37\x88\xe5\x9e\xef7\xf8\
-S\xd8k\xfb_@\x00\x80 \xe0fI\xcc\x9f\x03\x9b\
-\xc4<-\x16\x04\x00\x004\x7f\xf0?\xcb\x87\xfeID\
-\x1c\xe4\xd7u\xcb\xceA\x06\x7f.\x06\x00V\x00\x94\xc8\
-#\x0049\x08\xe8G\xb6\x1a`\x96\x87\x003A\x00\
-\x00@c\x07\xff\xe2\xd9\xfe\xd3|\xe8\x1f\xae:\x97\x18\
-\xfc\xb9@\x07\x00t0\x08(\x96\x8c\xad\xb4m\xa0 \
-\x00\x000\xf8\xd72\xf8\x1f\xe5\x83\xff~~\xcdf\xf0\
-\xa7\xec\x10\xa0\xb57\xae\xad\x00@\x10\xb0\xbe\xa2\x1f\xe0\
-0?\xd1\x08\x02\x00\x00\xb63\xf8\x17\xdb\xf8->\xdf\
-\xbfo\xf0\xa7\xa2\x99u\xd6\xd6\x17/\x00@\x10P\xc2\
-\x1f\x97\x07\x01\xd3\xb0\x22\x00\x000\xf8\xd79\xf8\x17\xdb\
-\xf8M\x22\xbb93\x8a\xd5\x96i\x1b\xfcYgf=\
-\x13\x00@\xb7\x83\x80^dIs\x12\xf3g\xcd\x04\x01\
-\x00\x80\xc1\xbf\x9a\xc1\x7f\xb1\x98y\x94\x0f\xff\xab\x0eq\
-\x06\x7f\xd6e\x05@I\xac\x00\xa0\xedA@\xb1\x9d\xcc\
-I~bZ\xf9\xc3A\x10\x00\x00\x18\xfc\xafT,\xf3\
-\xef\xc7j\xdb\xf8\x19\xfc)sf\xd5\x01\xe0`\x22\x08\
-8\xa7\xe8\x07X\xab(P\x10\x00\x00\x18\xfco\x99\xe5\
-C\xffQ\xcc\x97\xf9\xaf:\xc7\x18\xfc){n\x15\x00\
-\x94\xe4\xcc\xfb\x89\x1d\x0c\x02\x8e\xf3/A\x00\x00`\xf0\
-_N\xf1|\xffI\xac\xb7\xcc\xdf\xe0OUZ\xbb\x1d\
-`\x13W\x00\xcc\xbc\x9f\xd8\xc1 `\x14\xd9R\xb5\xc5\
-\xe7\xd5\x04\x01\x00\x80\xc1\xffvG\xf95S\x92_C\
-\x0d\xd7\xf8=\x0c\xfeT9\xb3\xb6V\xd3\x02\x80$<\
-\x02\xc0\xee\x06\x01{\xf9\x09,\xcdOj\xa7\xeb\xfc&\
-\x82\x00\x00`G\x07\xff\xc3\xc8\xee\xf8\x0f\xf3\xaf\xbe\xc1\
-\x9f\x06\x9a\x85\x15\x00\xa5\x06\x00\xb0\xebA@qR+\
-\x8a\x02\xd7\x22\x08\x00\x00v`\xf0?\x8dy\xb1\xdfA\
-\xac\xf7|\xbf\xc1\x9f:Y\x01\xb0\xc3\xaf\x07A@\x95\
-A\xc0\xc6\xfd\x00\x82\x00\x00\xa0\xa5\x83\xffqd\x8fE\
-\xceb^\xec\xb7\xf60f\xf0\x87v\x0e\xdc{a\x15\
-\x00\xdd\x0b\x02F\x0bA\x80\x15\x01\x00\xc0.\x0f\xfe\x87\
-\xf9\xf5\xce~\xac\xb7\x8d\x9f\xc1\x9f&\xb0\x0b@I\x0c\
-\xfft5\x08(Jnz\xf9I\xf1D\x10\x00\x00\xec\
-\xc8\xe0_l\xe37\x89l\x99\xff0\x0f\x00\x0c\xfe\xd0\
-\xf1\x00@\x08@\xd7\x83\x80~~R<\xcbO\x92k\
-\xef\x8a!\x08\x00\x00\xb6<\xf8O\x17\x06\xffu\xdb\xfc\
-\x0d\xfe\xb0\xe3\x01\x00\x08\x02\xe6'\xc9Il\xf0X\x80\
- \x00\x00\xd8\xc2\xe0\x7f\x14\xf3m\x8fG\x91=\xe3o\
-\xf0gW\xb4\xfa\x86\xb5\x15\x00\xd0\xec \xa0(\x0a,\
-\xdaq\x05\x01\x00@\x93\x07\xffb\x1b\xbfM\x9e\xef7\
-\xf8\x83\x00\x00:\x1f\x04\x0c\x22[\x0d \x08\x00\x00\x9a\
-2\xf8\x9f-\x0c\xfeE\x9b\xff&3\x86\xc1\x9f6h\
-\xed\xcc\xea\x11\x00hO\x10\xd0\x8b,Q\xefE\xb6\xac\
-\xeeT\x10\x00\x00li\xf0\x9f\xe6_'\xb1\xd96~\
-\x06\x7f\xda&\x15\x00\x94\xcb\x0a\x00\x04\x01\xd7+\x96\xd4\
-\x9d\xe6'\xde\x8d~OA\x00\x00\x18\xfcWp\x14\xd9\
-\x8a\xc4$\xbf\x1e1\xf8\xd3E=/\x5c\x00\x00u\x07\
-\x01\xa3\xfc\xc4\xbbq?\x80 \x00\x00\x0c\xfe78\xce\
-\xbf\x8a\xa2\xe2\xbe\xc1\x9f\x8e\xb2\x02\x00\xd8j\x10p\x90\
-\x9f\x8c\x8f\x05\x01\x00`\xf0/q\xf0?\x8d\xf9\x8d\x86\
-Q\xfe\xb5\xe9\xefi\xf0\xa7\xed\xec\x02\x004\x22\x08\x18\
-E\x96\xc6\x17\xcf\xe4\x09\x02\x00\xc0\xe0\xbf\x8e\xe2\xa6\xc2\
-Y\x94\xf3|\xbf\xc1\x1f\x01\x80\x00\x00\x04\x01\x15\x04\x01\
-{\x91=\x160\x8b\xec\xf9\xbc3A\x00\x00\x18\xfc\x97\
-t\x98_?\xec\xc7|\xa9\xbf\xc1\x1fn\xbf\xde\x16\x00\
-\x94(\xf5\x9eB\x10\xb0\xf1\xcfAq\xd2\xdex\xdb@\
-A\x00\x00\xec\xf4\xe0?\x8bl\x99\xffQd\x8f\x15\x0e\
-\xf3\x00\xc0\xe0\x0fW\x07\x00:\x00\x80F\x06\x01E?\
-@)E\x81\x82\x00\x00\xd8\x99\xc1\x7f\x1a\xd9\x8d\x82b\
-\x1b\xbfqI/\xd7\xe0\xcf\xae\xeby\xf1\xe5\xb2\x02\x00\
-A@\xf9A\xc08\xb2G\x03\x8a\x93\xbd \x00\x00\xba\
-9\xf8\x1f\xc6\xbc+h\x18\xe5,\xf37\xf8\xd35V\
-\x00\x00\x8d\x0f\x02zy\x08\xd0\x8by\xe2/\x08\x00\x80\
-n\x0c\xfeG\xf9\xe0_l#<0\xf8\xc3f\xef{\
-\x01@\xc7\x0f&\xb4$\x08\xe8G\x96\xf6\x9f\xe5A\xc0\
-L\x10\x00\x00;9\xf8\x9f\xc5\xfc1\xc0b5`Y\
-\xd7\xff\x06\x7f\xba,i\xeb\xdcj\x05\x00t7\x08(\
-\xbd(P\x10\x00\x00\x8d\x18\xfc\x8f#\xbb\xdb_<\xdf\
-?*\xf1\xe5\x1a\xfc!\xfb9\x98\xb5\xf1\x85[\x01\x00\
-\x82\x80\xe2\xc2\xa0\xb4\xa2@A\x00\x00lu\xf0/\xb6\
-\x056\xf8Cu3\xebY\x1b_x\xaf\xc1\x07\x14\xa8\
-?\x08\xe8G\xb6\x22\xa0\xb4)]\x10\x00\x00\x95\x0e\xfe\
-i\xccC\xfca>\xf8\xf7\x0d\xfeP9+\x00J\xfc\
-\x90\x99y?\xc1V\x82\x80\xbd\x98\xb7\x01O\x22\xe2T\
-\x10\x00\x00\x8d\x1c\xfc\x8b.\x9f\xe2\xf9\xfeQ\x94\xdbL\
-n\xf0\x87%~F\x04\x00\x9b\x9bEK\x97S\xc0\x0e\
-\x05\x01\xc5\xb6@\xa7\x91-%,\xed\x03N\x10\x00\x80\
-\xc1\x7f\xa3\xc1\xff8\xff:\xcb\xcf\xd5\xe3*\x86\x1a\x83\
-?\xdc\xf8s\x22\x00(Ik\x1b\x15a\x07\x83\x80b\
-\xab\xa0\xe2b\xa34\x82\x00\x00\x0c\xfe+)\x96\xf9\xf7\
-\x17\xce\xcf\x06\x7f\xd8^\x00\x90\xb4\xf1\x857\xf5\x11\x00\
-\x01\x004+\x08\x18Gv\x97\xa1\xd4\xa2@A\x00\x00\
-\x06\xffk\xcd\xf2s\xefQ\xcc\x97\xf9\xef\x19\xfc\xa1\x11\
-3k+\xd9\x06\x10\x04\x01\xcbJb^\x148\xcd\xbf\
-\x04\x01\x00p\xcd\xe0\x9f$\xc9:\x83\xff4\xe6\x8d\xfe\
-\xe3(\x7f\x99\xbf\xc1\x1f6\xff\xf9\xb1\x02\xa0\xc4\xd7\x94\
-xOAc\x83\x80bk\xa14\xbf0)\xb5\xb4S\
-\x10\x00\xc0.\x0d\xfei\xba\xd2\xa9\xf60?\xb7\xf6\x22\
-\xbb\xdb?\xaa\xe0\xe5\x1a\xfc\xa1\xa4\x9f#\x01\x80\x00\x00\
-\xba\x14\x04\x14[\x0d\x95\xde\x0f \x08\x00\xa0\x83\x83\xff\
-q\xcc\x9f\xed\xdf7\xf8\x03]\x09\x00\xf6\x04\x00\xd0\xaa\
- \xe0 \xbf`9\x8c\xec\x19EA\x00\x00\x06\xff\x9b\
-\x9d\xe5C\xffd\xe1\x5cZ\xc5\xb5\xb9\xc1\x1f\xaaa\x17\
-\x80\x92\x18\xfe\xa1\xbdA\xc00\xb2\xa5\x8b\xa5O\xe7\x82\
-\x00\x00vd\xf0/\x9e\xed?\xcd\x87\xfea\x95\xc3\x89\
-\xc1\x1fhz\x00 \x04\x80\xf6\x06\x01\xbd\xc8\x96.&\
-\x0b\x177\x82\x00\x00\x0c\xfe\xd9*\xb9id\xcb\xfb\x07\
-\x06\x7fh\xb5\xd6\xce\xabv\x01\x00\xaa\x08\x02\x06\xf9\xd7\
-Id\xab\x01fe\xbfVA\x00\x00-\x18\xfcg1\
-\xef\xca\xa9\xf2\xf9~\x83?\xd0\xea\x00\xc0\x0a\x00\xd8\x8d\
- `\x1c\xd9\x1d\x8eITP\x14(\x08\x00\xa0\xa1\x83\
-\x7f\xb1\x8d\xdf$\xe6m\xfeU]\xdf\x1a\xfc\xa1~\xb6\
-\x01\x04\x04\x017\x04\x01\xa3\xa8h\xc7\x00A\x00\x00\x0d\
-\x19\xfc'\xf9\xf0\x1f\xf9yo\x5c\xf1\x00b\xf0\x87\xed\
-\x05\x00\xad\x9c\xa5\xad\x00\x00\xea\x0c\x02F\x11\xd1\xcf/\
-\x90*\x99\xcc\x05\x01\x00la\xf0?\x8a,\xe0\xee\xc7\
-\xfc18\x83?\xec6+\x00\x04\x00 \x08X\xc2^\
-\xcc\x8b\x8f&QAQ\xa0 \x00\x80\x1a\x06\xff\xe2\xf9\
-\xfe\xa3\x98\xaft\xab\xf2\xda\xda\xe0\x0ff\xd6\x9d\x0d\x00\
-\x80\xdd\x0f\x02\x86\xf9WQ\x14X\x09A\x00\x00%\x0f\
-\xfe\xc5\xf3\xfd'Q\xfd2\x7f\x83?4w\xf8\x17\x00\
-\x94|@\x81n\x04\x01EQ\xe0\x91 \x00\x80\x06\x0f\
-\xfe\xc5y*\xc9\x07\xffa\xc5/\xd7\xe0\x0f\xe6h/\
-\x1c\xd8\xe9 `\x10\x15\x16\x05\x0a\x02\x00\x0c\xfek\x0c\
-\xfe\x871o\xf3\x1fF\xf6\x9c\xbf\xc1\x1f\xbamO\x00\
-P\xc1\x07\x1f\xd0\xb9 \xa0\xb8\xab\xb2\x17\xe7\x9b\x94\x05\
-\x01\x00\xd49\xf8\x9f\xc6\xbc\xd8\xef \x1f\xfc\xab^\xa1\
-j\xf0\x87v\x05\x00\x1e\x01\x10\x00\x00%\x05\x01\xfd\xfc\
-bk\x96\x87\x003A\x00\x005\x0c\xfe\xc7\x0b\xe7\x9d\
-\xa2\xd8\xaf\x96\xeb^\x83?\xb4J\xd2\xd6\x99\xd5#\x00\
-@\x93\x83\x80Qd\x8f\x05T\xb6m\xa0 \x00\xc0\xe0\
-\x1f\xf3e\xfe\xfbQ\xfd6~\x06\x7f@\x00p\xd9\x07\
-\x22 \x08\xc8\x15E\x81\x87\x91-\xc9\x14\x04\x00\xb0\xe9\
-\xe0_l\xe37\x89\xf92\xff}\x83?\xb0$\x8f\x00\
-\x00T\x1c\x04\x14\x17h\x93\xa8\xb0(P\x10\x00\xb0\xd3\
-\x83\xff4\xe6=3u\xb4\xf9\x1b\xfca7y\x04\xa0\
-\xeb\x07\x13\xa8%\x08\xe8\xe5\x17k\xbd\xfc\xe2\xedT\x10\
-\x00`\xf0_b\xf0?\x8ay\xb9\xec0\xeay\xbe\xdf\
-\xe0\x0f\xbb\xab\x95=\x00\x02\x00\xa0\xadA@\xf1\x8c\xe6\
-idwr*\xfd\xdc\x10\x04\x00\xb4v\xf0/\x96\xf9\
-\x0f\xa3\xbe\xe7\xfb\x0d\xfe\xd0\x0d\xb3\xb6\xbd\xe0\x9e\x83\x09\
-\xb4<\x08(\x96o\x1eE\xc5\xfd\x00\x82\x00\x80\xd6\x0c\
-\xfeg\x0b\xe7\x85\xe2<Q\xd7u\xaf\xc1\x1f\xba\xe3L\
-\x00P\xde\x07\xe7\xa9\xf7\x13\x08\x02V\x08\x02\x0e\x22+\
-\x0b<\x8e\x8a\xfb\x01\x04\x01\x00\x8d\x1d\xfc\xa7\xf9\xd7I\
-~N\x18\xd7|\xfdj\xf0\x87\xeeH\xc3\x0a\x80n\x1f\
-L\xa0\x11A\xc0(\x22\xfa\x0b\x17\x81\x82\x00\x80\xdd\x1f\
-\xfc\x8f\x22[\xe6\x9fD\xb6\xc4\x7fT\xe3\xcb5\xf8C\
-w\x03\x00\x1d\x00\x00\x0d\x08\x02\xf6\xf2\x0b\xc04\xbf \
-\xac|y\x96 \x00\xa0\xf6\xc1?\xcd\x07\xff\xe3\x98/\
-\xf3\xef\x1b\xfc\x01\x01@\xfb\x02\x80V\x1eL\xa0qA\
-\xc00\xff*\xb6|\xaa\x9c \x00\xa0\xf2\xc1\xff4\xe6\
-w\xfc\xc7\xf9\xf0_\xe7~\xdc\x06\x7f\xa0\xf8,H\xda\
-\xf6\xa2{\x0e&\xd0\x81 `\x1c\xf3\xa2\xc0\xe3:^\
-\xab \x00\xa0\xf4\xc1\xbf\xe8x\x99-\x0c\xfeu_\x9f\
-\x1a\xfc\x81e\xaf?\x05\x00+H\x04\x00@EA\xc0\
- \xe6[B\x09\x02\x00\x9a?\xf8\x1f\xe6\x9f\xd9\xc5\xb3\
-\xfd\x83\x9a_\xae\xc1\x1f\xb8\xea\xb3\xc1\x0a\x00\x01\x00\xd0\
-\xf0 \xa0\x97_@\xf6\xf2\x0b\xca\x13A\x00@\xe3\x06\
-\xffY\xcc\xb7\xf1;\x88z\xb7\xf13\xf8\x03K\x7fF\
-\x08\x00\xca\xb1\xe7\xfd\x04T\x1c\x04\xf4\xf3\x0b\xca\xb3<\
-\x08\xa8e\xe7\x91\x22\x0889=\x15\x04\x00\x9d\x1d\xfc\
-\x8f&\xd3\xab\x06\xff\xa2\xb3e\x1b\xdb\xf8\x19\xfc\x81\x9d\
-\xd7\xe4\x00\xc0\x0a\x00\xa0\x8e \xa0h\x8e\x9eDM\x8f\
-\x05DD<\xf4\xd1CA\x00\xd0\xd9\xc1\xff#\x0f\x7f\
-\xfc\xe2\xe0\x7f\x18\xf3\xad[\x8b\x02W\x83?\xd0dI\
-\xd8\x05\xa0\xd4\x83)\x00\x00\xea\x0c\x02j/\x0a\x14\x04\
-\x00\x06\xff8\x8c\xf96~\x83\xa8\xff\xf9~\x83?\xd0\
-)=\x87\x00\x10\x04\xdc\x16\x04\x0c\xc2\x8a\x00\x80\xaa\x06\
-\xff\xe2\xd1\xab\xe3\xc8\x9e\xef\x1fm\xe9\x9a\xd4\xe0\x0fl\
-J\x09`\x97\x0f&\xb03A@/\xb2\xd5\x00Id\
-KRO\x05\x01\x00\x1b\x0f\xfe\xc7\x0b\x9f\xa9\xc3\xa8\x7f\
-\x1b?\x83?P\xf6g\x89\x00@\x00\x00\xecP\x10P\
-,G=\xcd/Zk{\xceK\x10\x00\xec\xe0\xe0\xbf\
-\x9f\x7f\xa6\x0e\xb7\xf4r\x0d\xfe@\xd9\x9f)\xad[Q\
-\xef\x11\x00@\x10ps\x10P<\x9bz\x1c5\xf6\x03\
-\x08\x02\x80\x16\x0f\xfe\xc56~\xc7\xf9\xc0?\xc8\x03\x00\
-\x83?\xb0K\xac\x00\xe8\xf2\xc1\x04v>\x08X,\x0a\
-<\x12\x04\x00\x06\xff\xdb\x06\xffi>\xf4O\xf2\xcf\xcc\
-\xd1\x16\xaf\xe9\x0c\xfe@\xd5\xf3\xaa\x00@\x00\x00\xecx\
-\x10\x90\xc4\xbc(p\x1a\xf3m\xab\x04\x01@\x97\x07\xff\
-\xc5\x15R\xa3\xfcsr[\x0c\xfe@]\xb3\xb4\x00\x00\
-\xa0#A\xc0^\x1e\x02\xa4y\x080\x13\x04\x00\x1d\x1c\
-\xfc\x8be\xfe\xfd\x98?.e\xf0\x07\xba\x12\x00x\xd1\
-\x00\x1d\x0b\x02\x8ag[k\xef\x07\x10\x04\x00[\x1a\xfc\
-\x17\x9f\xef/\x96\xf9\xef\x19\xfc\x81\x8e\xd9o\xe3\x8bn\
-r\x00\x90zO\x01-\x0a\x02\x8a\xbd\xac\x8f\x04\x01\xc0\
-\x8e\x0e\xfe\xc5\xf3\xfd'\x0b\x83\xff\xd6\xaf\x15\x0d\xfe\xc0\
-\x96\xb4\xf2\x91u+\x00\x00\xca\x0d\x02\x16\xfb\x01j\x9f\
-\xbe\x05\x01@\x05\x83\xffa\xfe\x99\xd6\xcb\x87\xfe\xe1\x96\
-_\xae\xc1\x1f`\x07\x03\x00+\x00\x80\xb6\x06\x01\xbd<\
-\x04H\xf2\x10\xe0D\x10\x00\xb4t\xf0?\x8e\xf9\xb3\xfd\
-\xdb^\xeej\xf0\x07\xd8\xe1\x00\x00\xa0\xedA\xc0 \xb2\
-;egy\x100\xab\xfb\xb5\x0a\x02\x80\x15\x07\xff\xb3\
-4M\x8bN\x93\xe2\xd1\xa6m_/\x1a\xfc\x01:\x10\
-\x00\xcc|{\x80\x1d\x09\x02\x8a%\xb3\x93\xd8B?\x80\
- \x00Xb\xf0\x9f\xe4\xcf\xf8\x9f\xe5\x9fY\xa3\x06\xbc\
-\x5c\x83?\xd0t\xb6\x01\x04\x10\x04\x5c\x19\x04\x14\xa5Y\
-[)\x0a\x14\x04\x80\xc1\xff\x92\xc1\xff(M\xd3Id\
-\xcb\xfb\x8bUK\x06\x7f\x80\x15>\xaf\x04\x00\xe5\x1dL\
-=\x00\xc0\xae\x06\x01\xfd\xc8V\x04le\xf2\x16\x04@\
-\xa7\x07\xff4\xbf\xe3_l\xe37\x8cflge\xf0\
-\x07\x84\x00\x1d\x0e\x00\x22\x22N\xbd\x9f\x80\x1d\x0d\x02\xf6\
-b~\xa7m\xb2\xad\xcf;A\x00tj\xf0?]\x18\
-\xfc\x8be\xfeMX\xbej\xf0\x07\xda\xacU\x8f\xae\xf7\
-\x1cL\x80\xad\x06\x01\xc3\xfc\xeb4\xb2m\xb6\xb6\x92\x22\
-\x0b\x02`\xa7\x07\xff\x93\xf3\xfcw\xd2\x00\x00 \x00I\
-DAT\x8f<\xfc\xf1\x934Mg\xf9\xd0?n\xc8\
-\xcb5\xf8\x03\xbb\xe0L\x00P\xdeI\xc1#\x00@W\
-\x82\x80b\x9b\xad\xa2}{+\x04\x01\xb0S\x83\xff4\
-\xbf\xe3\xbf\x97\x7f\xbe\x0c\x0c\xfe\x00\xa5\x7f\x9eY\x01P\
-\x92\x99\x00\x00\xe8`\x10P<\x8f\xbb\xb5\xa2@A\x00\
-\xb4~\xf0?\xc9\x07\xffA4c\x1b?\x83?\xb0\xcb\
-\x01\x80\x0e\x00\x006\x0a\x02\x92<\x08\xd8\x8b\xac\x1f`\
-*\x08\x00\x96\x1c\xfc\xa7i\x9a\xf6\xa3\x19\xdb\xf8\x19\xfc\
-\x01\x01\x80\x00`%\x89\xf7\x14\xd0\xe1 \xa0\x1f\xd9j\
-\x80Y\x1e\x02lm\x89\x99 \x00\x1a?\xf8\x9f\xe6\x83\
-\xff\xb0A/\xd7\xe0\x0ft!\x00h\x95\xa6w\x00\x08\
-\x00\x00A\xc0\xbc\x1f`k\xdb\x06\x0a\x02`\xbb\xa6'\
-\xa7W\x0d\xfe\x91\x0f\xfe}\x83?\x80\x99\xb5\xcd\x01@\
-\x08\x00\x00A\xc0\xb9 \xa0\xe8\x078\x8c\xac#@\x10\
-\x00\x1d\x19\xfc?\xe3\x09\xcf*\x06\xff$\x1f\xfc\x93|\
-\xf0o\xd2\xb5\x92\xc1\x1f\x10\x00\x08\x00v\xf2\xb5\x01l\
-3\x088\xc8\x83\x80iX\x11\x00]\x19\xfc/\xde\xf1\
-o\xda\x05\xb0\xc1\x1f\xe8j\x00\xd0*M\x1e\xb2\xf7\xc2\
-\x0a\x00@\x10pU\x10\xd0\x8b\xec\xb1\x80$\x0f\x02N\
-\x05\x01\xb0\xb3\x83\xff\xd9\xc2\x1d\x7f\x83?@s\xb4n\
-^\x15\x00\x00\xb4;\x08(\xf6\xf6>\x89l5\xc0V\
-\xf7\xa2\x15\x04@\xa9\x83\x7f\xe4\x83\xff\x9e\xc1\x1f\x80]\
-\x0f\x00\x12\x01\x00\xc0\xd2A@\xd1\x0f\xb0\xf5\xa2@A\
-\x00\x946\xf87\xed\xe5\x1a\xfc\x01n\xff\x5c\xd4\x01\x00\
-@#\x82\x80\xe3\x06\x06\x01!\x08\x80v\x0e\xfe\x07\xe3\
-Q\xbc\xe8;\x9ea\xf0\x07\x10\x00T\xc6\x0a\x00\x80\xf5\
-\x82\x80ad\xdb\x825iE\xc0\xd4\x8a\x00\x0c\xfe\x97\
-\x0e\xfe\xd36\xdc\xf1\xff\xb3\x07\x7f-y\xd9\x0b\xee5\
-\xf8\x03\x9c\x9fW\x05\x00\x02\x00\x80F\x04\x01\xbd<\x08\
-\x88<\x048\xdd\xf2K={\xe8\xa3\x87\x93\x888\x11\
-\x04`\xf0?w\xc7\xff\xac\xc9\x83\xbf;\xfe\x00\xbb3\
-\xb3z\x04\x00`\xf7\x83\x80A\x1e\x04\x14E\x81\xdb4\
-\x8c\x88\x99\x8e\x00\x0c\xfe\x9e\xf1\x07\xd8\x91\xe1_\x00P\
-\xf2\x01\x05\xa0\x9c `\x94\x0f\xe0G[\x0e\x02\xfa\xf9\
-kP\x16\x88\xc1\xdf\xe0\x0f\xd0f=\x01\x00\x00m\x08\
-\x02\x06\x91\x95\x04n\xa3(\xb08Y\xde\xda\xb2P\x10\
-\x80\xc1\xdf\xe0\x0f\xd0B\xad\xdb\xba^\x00\x00\xd0\xcd \
- \x89\xf3E\x81\xd3\x9a_\xd6(\xb2G\x12\xce\x11\x04\
-`\xf07\xf8\x03\xb4,\x00h\x15\x01\x00@\xb7\x83\x80\
-\xbd\xc8V\x03$\x91\xad\x06\x98\xd5\xf8\x92\x8a?3\x04\
-\x01\x18\xfc\x0d\xfe\x00\x08\x00R\xdf\x22\x80Z\x82\x80~\
-d+\x02N\xa3\xbe~\x80\x22x\xb8\x92 \x00\x83\xbf\
-\xc1\x1f\x00\x01\x00\x00\xd5\x04\x01\x83\xfc\xeb$\xea\xe9\x07\
-\x18.\xf3\xe7\x5c\x12\x04\x84 \x80-\x0f\xfea\xf0\x07\
-@\x00\x00\xc0.\x04\x01\xc5\x8a\x80\xba\x82\x80\xa5:\x08\
-\xac\x08\xa0\x01\x83\xff\xe2\x1d\xff3\x83?\x00\x02\x80\x92\
-O`\x00l=\x088\xcd\xbf\xaa0Z\xf5_x\xe8\
-\xa3\x87G\x11\x91\x0a\x02\xd8\xd2\xe0\x1f\x1fy\xf8\xe3\xc7\
-i\x9a\x9e\x19\xfc\x01\x10\x00\x00\xb0kA\xc0~d\x85\
-\x81\xa7QM8\xbb\x1f\x11G+\xfe;I\xbe\x22`\
-\x22\x08\xa0\xc6\xc1\xbf\xb8\xe3\x9f\xc65E\x96\x06\x7f\x00\
-\x04\x00\xeb\x9d\xd0\xce|\x9b\x00\x1a\x15\x04D\x5c\xb2\x85\
-_\x09\xe7\xa3$\xd6\xdb\x85`\xf8\xd0G\x0f'\x11q\
-2\x0f\x02\x9e)\x08\xa0\xaa\xc1\x7fQ?\xb6\xbb\xff\xb3\
-\xc1\x1f\x00\x01\x00\x00\xd5\x04\x01\xafx\xc9\xfdq\xe7\x1d\
-\xb7\x1e\x0d(;\x08\x18\xc5\xfa\x8f\x19\x8c\x22b\xff\xa1\
-\x8f\x1e\x9eD\xc4\xec\xe4\xf4L\x10@\x95\x83\xff\xc5\x10\
-\xe0\xa8\xe6\x97k\xf0\x07h\xde\xdc*\x00(\xe9@\xce\
-\xbc\x9f\x00\x9a\x11\x04<\xf7\xde\xbb\xe3\xfd\x7f|kE\
-@\xba\x10\x04\x94\xd9\x0f\xb0\xee\x92\xea$\xb2\x1d\x0c\xa6\
-\x0f}\xf4p\x1a\x11!\x08\xa0\xc2\xc1\x7f\xf1Z\xaa\xae\
-U\x00\x06\x7f\x80fj\xcd\xcc\xda\x86\x0e\x00E\x80\x00\
-\x0d\x0b\x02.<\x1a\x90F\xf6h@\x19\xa1\xed\xa0\x84\
-\x978\xca_\xcb\xf1|\xd7\x00A\x00\xa5\x0f\xfe\x17\xdf\
-sU\xae\x020\xf8\x034{^m\xcd\xaau\xbb\x00\
-\x00PN\x10\x90=\x1a\xd0+\xe1\xb3{\x14\x9b\x17\xab\
-\x8d\x22\xdb\xbd`\x1a\x113A\x00\x15\x0d\xfe\x8b\x92\x0a\
-\xae[\x0c\xfe\x00\xed\x08\x00\xac\x00\x10\x00\x00t,\x08\
-\xc8\x1f\x0d\xb8\xf3\x8eq1\x0dm\xfa\x19\xbei\xbf@\
-\xf1H\xc0I\x11(\x08\x02\x0c\xfe\x15\x0c\xfe\x85QD\
-\x94\xf5F2\xf8\x03\xb4+\x00\xd0\x01P\xe2\xc1L\xbc\
-\xa7\x00\xda\x13\x04\xbc\xff\x8f\xdf\x94\xfc\xe0K\xef\x8f\x83\
-\x83\x8d\x82\x80Q\x89'\xd3a\xfe\xcf[\xab\x0a\x04\x01\
-\x06\xff\x12\x07\xff\x8b6\xe9\xc30\xf8\x03\x08\x00:\x1d\
-\x00\x84\x00\x00\xa0\x9dA\xc0\x07\xde\xf9\xa6\xe4\xe5/~\
-v\x0c\x87\x83\xe2s|\xbc\xe2o\xb5\x1f\xe5=W=\
-\x8a\xbc 0\x16\x96\xe9\x09\x02\x0c\xfe%\x1b\xc5z\xcf\
-\x81\x8e\x22\x22\xee8\x18\xc7\xcb_\xfc\xec\xf8\xd0\xbb\xdf\
-b\xf0\x07hW\x00\xd0\x1a\x02\x00\x00*\x0b\x02\x9e\xff\
-\xeco\x8a7\xfe\xc2\xabo=\x16\xb0\xc69*\x89\xf2\
-\x9e\xab\xeb\xc5\xfc\x91\x80s\xc1\xc2UA\xc0\xd1\xf1\xd4\
-7\xd2\xe0\xbf\xceu\xcb\xaa\x09R2\x1e\x0d\xe3W\x7f\
-\xf6U\xc9\xf3\x9f\xfdMq0\x1e\xf9F\x02\xb4+\x00\
-h\xcd\xcc\xda\xf3\xfd\x02\xa0\x92\xb3a\x9a\xc6+\x7f\xec\
-5\xf1\xc4\xafzf|\xfc\xf08\x8d\xec\xee\xfb\xaaF\
-\xb1y\x17\xc0E\xc5#\x01\xb7\x0di\x17\x83\x80O\xfb\
-\x9b\xff\xad \xa0e\x83\xffg~\xf1\xd6\x06\xff\xc2:\
-;YL\x8f\x8e'\xf1\x84\xaf\xfc\xfb\xf1\xc2\xef\xff\xd1\
-8;\xb3\x032\x80\x00\xa0\x9b\x01@/\x84\x14\x00\xad\
-\xf3\xff\xfc\x7f\xef\x8f\xc7|\xe9\xd3\xd2\xe7\xbd\xf4Gb\
-6\x9b\xa5i\x9a&\xb1\xfe\x169I\x94\xbf\xc5\xda8\
-\x22\xfay\x08\x90\x0a\x02vg\xf0?<\xde\xda\xe0\xbf\
-h/V\xdb\xc9\xa2\xf8\xd9\x98\xbd\xfcU?\x1d\x7f\xed\
-\x09\x7f/\xfd\xb7\xff\xf7\x9f\xfa\xe6\x02\xd0\xb9\x00`\xcf\
-\xb7\x08\xa0]\x1ex\xc3[\xe3\xd1\x8f\xff\xea\xf4\x0f\x1f\
-|w\xb20\xc0ob\x10\xd5$\xeb\xbd\xc8V\x03L\
-\xe2\x8a%\xdb\x82\x00\x83\xff\x9a\xf6\xd7|\xcf\xf6\x22\x22\
-}\xcf{\xff]\xf2W\x1e\xf7\xd5\xf1\xda_\xfaU\xdf\
-h\x80\xe6\xd3\x01Pr\x00\xa0\x03\x00\xa0\x05\x8e\x8e'\
-q\xcf\xfd\xdf\x1bO}\xc6w\xc5\xe4\xb8\xf4\x12\xbdQ\
-\xacvGu\xd5\xdf;\xbd\xee\xf7\x17\x04\x18\xfc\xd7\xd0\
-\x8f\xf5V\xae\xe4\xef\xb5\xd3\xf4i\xdf\xfa\xdd\xf1\xd4{\
-\xbe+>\xf6\xf1C\xdfx\x80f\xf3\x08@\x89\x07R\
-\x00\x00\xd0p\xbf\xf7G\xef\x8c\xcf|\xecS\xd2\x9f\xfa\
-\xd9_\x8e\xc8\xa6\xe9\xaa>\xbbO+\xfa}G\x91\x85\
-\xce\xd7&\x17\x82\x00\x83\xff\x8a\xd7X\x9b\xfc\x1c$\x11\
-q\xf6\xc0\xaf\xbc5>\xfd\xaf\xff\xdd\xf4\x7f\xfb\xdf\xdf\
-\xeeM\x00\xd0Li\xb4\xe8\xb1u\xcf\xd7\x03\xb0\xfe\x19\
-//\xfa\xfb\xa2'==>\xf0\xa1\x0fW\xfd\xc7\xad\
-\xbb\xc5\xda\xb2\xfa\x91=\x120\x15\x04\x18\xfcK|\xcf\
-n\xb2re/\x22\xce>\xfc\x91\x87\x93\xff\xe2\xc9\xcf\
-\x88\x7f\xf8\x8f_\xad \x10\xa0yZu\xd3\xda6\x80\
-\x00\xac\xe5\x8a\xa2\xbf\xaa\xedE\xf9\x85\x80\x17\x0d\xf2\xa0\
-\xe1\xc6\xc1M\x10`\xf0_B\x1a\x9bme\xb9\x17\x11\
-\x91\xa6i\xfaO~\xe4\xa7\xe2\xf3\xbf\xe4\xeb\x15\x04\x02\
- \x00\x00\xa0>\x15\x14\xfd-\xab(W\xab\xba$\xf6\
- \xff3\x96\x9a\xe4\x05\x01\x06\xffk\x8c\xa3\x9c\xad,\
-\x93\x888y\xe7{\xfe$\xf9\x9c\xc7\x7f\x8d\x82@\x80\
-f\xcd\xd4\x1e\x01\x00`\xf7T\x5c\xf4\xb7\xaca\x92$\
-\x83\xa8\xbeu\xb7\x1f\xd9j\x80\x89 \xc0\xe0\xbf M\
-\x92H{\xbdd\xbc\xc2{0-)\x04\xe8G\xc4\xc9\
-\xf4\xe4$\x14\x04\x024F\xab\x8a\xeb\x05\x00\x00,\xa5\
-\xc6\xa2\xbf+%ID\xaf\xd7K\xbe\xfcK\x1e\x97\xde\
-y\xc7\xc1\xe2pUi\xe0\x10Y\xf9\xe0\xd2\x89\x87 \
-`\xa7\x06\xffYd\x8f\x83\x14\xdf\xbcd4\x1a\xc5W\
-\xfe\xed'\x9e\xed\xed\xf5\x92$Y\xea\xc7`T\xe2\xfb\
-\xb4\x9f\xff^\xb3\x07~\xe5\xad\xf1\xe9\x8fy\xb2\x82@\
-\x80\xed\x07\x00\xad!\x00\x00\xe0Z5\x17\xfd]\xebS\
-?\xf9\x93\xd2?x\xf3k\xe3W\x7f\xee\x9f\xa5\xef\x7f\
-\xf0\x8d\xa7?\xf8\xd2\xfb\xe3\xae;k\x09\x02\x8aG\x02\
-VZ\xf6 \x08h\xe5\xe0?\x8b\xacgb\x92\xffs\
-\x16Y\x084\x18\x8f\x86\xe9\x8b\xee\xbf'\xde\xf7\xe0\xaf\
-%\xaf\xfb\xa9WL\x1f\xfc\xcd\x9f\x8f\xcf\xf8\x8f>e\
-\x95\x17[\xd6V\x96I~\x0dw\xf2\xe1\xff\xf0\x90\x82\
-@\x80\xedj\xd5#\xeb\x02\x00\x00\xae\xb4\xa5\xa2\xbf\x8b\
-g\xd54\x22\xe2\xee\xa7~E\xfc\x9b\xdf~]\xf2\x9f\
-\xfc\xb5GG\xccf\xd3\x83;G\xa7\xcfy\xd6\xdd\xf1\
-\xbew\xbc1\xa9)\x08\xd8\xcf\x07\xc1\xa5\x1f\x09\x10\x04\
-\xb4b\xf0?\xc9\x07\xfd\xe3\xfc+\x8d\xec\xb9\xfdad\
-w\xee\xf7\xc7\xa3a\xbc\xe8\xfe{\xe2}\xefxc\xf2\
-\xb2\x17\xde\x17\x8f\xb8\xeb\x8e\x88\x88\xf8\xdc\xcf\xfe\xccx\
-\xd7o\xfdR\xf2\xeco\xf9\xbas\xef\xd5+\x0c*\xb8\
-H\xecG\xc4\xb1\x82@\x00!\x80\x00\x00\x80\x8dl\xb1\
-\xe8\xef\x9c\xf1\xc1(~\xf95?\x14\xafy\xf5\xf7\xc6\
-\xc1x\x94\xbf\x92$\x8d4{=\x07\xe3Q\xd4\x1c\x04\
-\x0cc\xc9]\x02\x04\x01\x8d\x1c\xfc\x17\x07\xfe\xc3\xfcZ\
-h\x9c\x0f\xfb\xa3\xc8Vz\xa4\x11\x11W\x0d\xfe\xe7\xde\
-\x0c\x83A\xbc\xea\xfb\x9f\x17o\xfa\xc5\x1f\x8b\xbb.\xf9\
-\xff/\x19\xd8\xcb\xde\xc5\xa2\xd8\x1e\xf3LA \x00\xbb\
-\x10\x00\xa4\xbeM\x00\xf5iH\xd1_DD<\xee\xb1\
-\x9f\x97\xbe\xf7w^\x9f<\xf9\xcb\x9ep\xd9\xe9\xa1\x17\
-\x0b\xdb\xab\x15A\xc0\x07\xdf\xf5\xe6\xe4\xd5?\xf0\xfc\xaa\
-\x83\x80q~\x0e]kr\xefR\x10\xd0\x80\xc1\xff8\
-\xce/\xe9\xdf_\x18\xf8\x8bG;\xce\xbdW\xc6\xa3a\
-|\xdf\x0b\xee\x8d\x0f\xbd\xfb-W\x0e\xfe\x17\xfd\xad'\
-|a\xbc\xf7m\xafO\x9e\xf8\x9f?\xe6\xba\xf7]U\
-M\xd1\xfb\xf9\xdfc:=9I\x15\x04\x02\xd0\xe6\x00\
-\x00\x80\x9a4\xa3\xe8/I\xf7z\xbdx\xe5K\xee\x8f\
-\xdfz\xc3O&\x9f\xf2\x17\xff\xc2U\xbfr\x10\x91\xde\
-\x96P\x0c\x07\x83\xb8\xef\xe9_{+\x08x\xc4\x9dw\
-T\x15\x04\x0c\xf2\xafid%\x81\x82\x80f\x0c\xfe\x17\
-\x07\xfea\xcc\x97\xf4\x8f\xe3\xf2\xf7t6\xf8\x8f\xe7\x83\
-\xff\x8b\xbf\xe3\x19\xf3\x15'Kz\xd4'\xfe\xf9\xf8\xf5\
-\xd7\xfd\xf3\xf8\x89\x7f\xfa\xdd\xb1\xbf\xb7wUA\xe00\
-\xca_\x05\xb0\xf8\x9e<\x8e\x883\x05\x81\x00\xb45\x00\
-\xb0\x02\x00\xa0\xea\x0f\xdaF\x15\xfd=*~\xff\xcd\xaf\
-\x8d\xef\xbc\xf7\xee\xb8\xb9a=\xb9\xf2<V\x04\x01\x1f\
-x\xd7\x9b\xea\x08\x02Nb\x83\x82\xb7]\x0a\x02\xb60\
-\xf8\x17\xcf\xeeO\xf2\x7f.3\xf0_>\xf8\xbfk\xbd\
-\xc1\xff\xa2{\xbe\xe1+\xe3\xed\xbf\xf9s\xd7\x15\x04&\
-\x15^\xdf\x8c#\x0b\xa4N\xff\xc3G\x1e\x0e\x05\x81\x00\
-\xb41\x00p\xd6\x02\xa8Hc\x8b\xfe\x96?G\x5c\xab\
-\xa6 `\xa3G\x02v!\x08\xa8q\xf0?\x8c\xf3w\
-\xf8\x8bg\xf7\x8b\xd2\xbed\xd9\xf7M\xd9\x83\xff\xa2\x1b\
-\x0a\x02G\xb1\xe2\x8e\x12+\x1aF\xc4^\x9a\xa6\xa7\x0a\
-\x02\x01hc\x00p\xe6[\x05P\xbeF\x17\xfd-g\
-\x14\x91.\xb5\x9c\xba\x86 \xa0x$`\xb2\xe9y\xab\
-MA@\x0d\x83\x7fQ\xd87\xc9\xbf\x0e\xe2\xfc\x1d\xfe\
-U\xaf)*\x1d\xfc/\xbe\xe7n(\x08\xac\xf2\xfa&\
-\x89\xactp\x12\x0a\x02\x01\x10\x00\x00tW{\x8a\xfe\
-\x96\x9asV\x0a-j\x08\x02\x86\xb1\xe1#\x01m\x08\
-\x02*\x1a\xfc\xd3\x98/\xe9/\x86\xfe\xa2\xb0o\x98\x7f\
-\xad\xfb\xfb\xd66\xf8_tEA\xe0(\xd6\xec\x8eX\
-\xd1(\xb2\x95)\x93\x93S\x05\x81\x00\x02\x80v\xd0\x03\
-\x00P\x92v\x15\xfd-s\x86Xo\xda\xac8\x08\x18\
-\xe5\xe7\xd8\xe32\x8eW\x93\x82\x80\x92\x07\xffY\xcc\xef\
-\xf0\x1f\xe5\x03\xf1(\xce/\xeb\xdf\xf8\xfaa<\x1em\
-e\xf0_T\x14\x04\xfe\xe4\x0f\x7fO\xec\xef\xdf*\x08\
-\xdc\x8b\x0d\x1f\x1bY\xd28\x22zi\x9a\xfdY\x0a\x02\
-\x01*\x99W[1\xb3\xf6\x1cL\x80\x8e\x9c\x99\x1aT\
-\xf4\xf7\x97V*\xfa\xbb1M\x18E\xb2~\xabz\x85\
-A\xc0 \x1f`\xa7Q\xd2J\xb6m\x06\x01%\x0d\xfe\
-\xc5\xc0?Y\x18\xf8\x8b;\xfc\xe3\xc8\x96\xac\x97u\xed\
-\xb00\xf8\xbfyk\x83\xffE\xdf\xfc_?%\xde\xfe\
-\x1b\xb7\x0a\x02\xf7\xf3\xbfs\x1d!\x5c?\x7f?N\x22\
-\xe2LA @\xe93k+>Lm\x03\x08\xd0\x01\
-M(\xfa\xcb\x87\xbc\xf8\xc6\xbf\xf7w\xe2=\xab\x15\xfd\
-\xdd\x18\x01D\x09\x7f\x9f\x8a\x82\x80$\xe6[\x05\x96\xb6\
-\xf5[\x9dA\xc0\x86\x83\xffI\xcc\xef\xf0\x1f\xe7\xc7r\
-\xf1\xf9\xfdA\x05\x17`\x8d\x1c\xfc\x17](\x08L\x8a\
-\x9f\x8d\x9a\x0c#b\x9a\xa6\xe9DA @\xa9\xe7\x9f\
-V<\xb6\xde\x86\x00`\x16[*\xa5\x02\xd8\x05\x0f\xbc\
-\xe1-\xf1\xe8\xc7}\xd5\xd6\x8b\xfe\x06\xfd\xfd\xe4\x97\xff\
-\xa7\x1f\x8a\xff\xf1\x9f\xbd\xb4\x82\x81,)m\xa5XE\
-A@\xb1\x1d]\xa9\x85\x0bU\x06\x01k\x0e\xfe\x8b\x03\
-\xffa~\x9dQ\xdc\xe1\x1fE\xb6\xe4\xbd\xaa\x0b\xaf\xc6\
-\x0f\xfe\x17\xdfg\xaf\xfa\xfe\xe7\xc5\x1b\x7f\xfeG\xe3\xae\
-;\x0f\xea^\xe9X\x94'N\x22\x22\x14\x04\x02\x94r\
-\x1e\xb2\x02\xa0\xc4\x83)\x00\x00X\xd1\xd1\xf1$\xfe\xfe\
-s^\x16O}\xc6\xf3c2\xd9Zi\x5c\x1a\x11\xf1\
-\xd7?\xffs\xd2\x7f\xf7\xfbo\x88'\x7f\xf9\x13\xaa\xf9\
-S\x92\x18DZ\xee\xb3\xd4\x15\x04\x01\xa3\x98\xaf\x06(\
-\xf5.A\x99A\xc0\x8a\x83\x7f\xf1\xec~\xb1\xa4\x7f\x7f\
-a\xe0?\xa8p\xe0o\xed\xe0\x7f\xd1\x97>\xf1o\xc4\
-\xff\xf9\xbb\xff\xeabA`\x1d\x16\xdf\x8f3\x05\x81\x00\
-\xe5\x9c\x93\x04\x00e]\xda\x01\xb0\xb4\xa2\xe8\xef\x7f\xf8\
-\x99\xd7\x17g\xa4\xad|\x8e&I\x92\xbc\xe2\x1f}{\
-\xfc\xde\x1b_\xb3Y\xd1\xdf\xcd\xa7\xdc\xbd\x88\xb4\x92\xe4\
-\xbd\xe4 \xa0x$\xe0$*\xd8\x07~\x93 `\xc9\
-\xc1\xff\xe2\xc0_,\xe5/\xfeY\xd7\xfb\xac\xf5\x83\xff\
-\xa2+\x0a\x02\xeb\xba\x0e\x1cD\xc4\x89\x82@\x80\x8d\xcc\
-\x04\x00\x02\x00\x80\xda5\xa4\xe8\xef,\x22\xe2S\xfe\xe2\
-_H\xff\xf0-?\x13\xcf\xbd\xefiQ\xcf@S\xed\
-\x9fQr\x100\x8a\xf9\x96w\xa5[%\x08\xb8a\xf0\
-_\xdc\x8e\xefx\x8b\x03\xffN\x0e\xfe\x17\xcd\x0b\x02?\
-\xb5\xee\x8b\xc8a~\xf1:\x89\x88P\x10\x08\xb0\xbb3\
-\xab\x00\x00`G4\xa0\xe8\xaf\x98\x14\xf6\xee~\xeaW\
-\xc4{\xdf\xf6\xfa2\x8b\xfe\x969S\xf4\x22I+/\
-\xe0)1\x08(\xb6\xb9\x9bFE\xcf\x0d^\x17\x04\x5c\
-2\xf8'I\x92L>\xf2\xf0\xc7\x8f\xd34-\xee\xf0\
-/n\xc77\xda\xe2\xf9x\xa7\x07\xffE\x9f\xfb\xd9\x9f\
-\x19\xef\xfc\xd7\xbf\x98\xfc\x83o\xf9\xfa\xe2\x02\xa8\xae0\
-`\x9c_\x17N\xd24M\x14\x04\x02\xac~\x9e2X\
-\xdf\xecw#\xe217\x04\x11G\x91m]\xb3\x7f\xd3\
-o\xf6/\x7f\xfa\x95\xf1_=\xe9\x89\xde~@\xe7<\
-\xf0\x86\xb7\xc6\xdd\xdf\xfa\xdd\xe9\xf1\xf1d[K\xfdO\
-\xd24\xed\x1f\x8cG\xe9\xcf\xfd\x8b\x7f\x9c<\xf9\xcb\x9e\
-P\xf5\x1fy\x14\xf3\x22\xb3\xc5\xf3\xefQD2\xae\xf3\
-\xef>\x99N\xe3'\xfe\xe7\x7f\x15/\xfc\xbe\x1fM\x1f\
-\xfe\xd8\xc7\x93X\xaf\xbbf\x92\xff{\x95N\xb4\x8f\xbc\
-\xeb }\xe8\xa3\x87\xc9\xa3>\xe1\x11\x11\x91\xc4\x07?\
-\xfcP<\xf2\xae\x83x\xe8\xa3\x87E/\xc1\xb8ao\
-\xed4\x22\x92\x83\xf1(\xfd\x87\xf7\xdf\x93|\xc73\xbf\
-\xa1IC\xffQ\xd5\xc7\xeb\xcd\xff\xeb\xef\xc6\xd7\xdc\xf3\
-\xbc\xf4\xe1\x8f~\xbc\xee\x9f\xebId\xfd\x0d\xfb\x11\x11\
-\x83~?~\xe2\x87\xbf'\xee~\xea\x93|\xd8\x02\x9d\
-\xf3\xfa_\xfd\x8d\xf8\xaa\xa7?\xf7\xa6_V\xac\xe8\xbb\
-\xe9$5\x8b\x88\xdf\x8f\x88/\xdc\xd6\xdf\xa7\x0d+\x00\
-lU\x08p\xd5\x04r\xab\xe8\xef\xbbbr<\xd9\xc6\
-K8\x8b\x88H\xd3\xb4\xff\xb8\xc7~^\xfa\xde\xb7\xbd\
-\xbe\x8e\xe1\xff\xda(\xa2\xee?\xb1\xa4\x15\x01\xc3\x85\xc1\
-\xab2\xc5\x8a\x80Ox\xe4\x9d\xe9'\xfc\xb9;\x8a\xff\
--\x22{\x0e\xbcI\xc3\x7f\x1a\x11q0\x1e\xc5\xcb^\
-x_|\xf0]oN^t\xff=;y\xc7\xff:\
-\x7f\xeb\x09_\x18\xef}\xdb\xeb\xb7Q\x108\x8c\xf9\x8e\
-\x0e\xa1 \x10`\xb9\xf3V\x1b\xb4a\xb8\xde\x0b\x8f\x00\
-\x00\xdc\xa6\x01E\x7f'\x11\xb1\xd7\xeb\xf5\xe2\x95/\xb9\
-?~\xeb\x0d?Ym\xd1\xdfR\xa7\xdf$\xd9\xd6I\
-\xb8\x84 `\x14\xd9\x8a\xb7\xca\x1e\x09(\xbc\xe7\xdf\xfe\
-i\xf2\x9e?i\xe4\xb2\xeesK\xfd\xbb:\xf8/\xda\
-bA`\xd1\xf1p\x9c\xa6\xd9g\xcb\x03\xbf\xf2\xd6\xf8\
-\x0c\x05\x81\x00W\x9d\xbfZq\xe3Z\x00\x00\xd0\xb63\
-\xcc\xf6\x8b\xfeN\xf2\x01\xb5\xff\x97>\xe5\x93\xd2?x\
-\xf3k\xe3;\xef\xbd;\x92\xa4\x01\x1f\xd5I:\x8cH\
-\x8f\xb7\xf9\x126\x0c\x02n\xb5\xb2G~\xf7\xb5C\x17\
-N\x9dx\xc6\x7f]\xf3\x82\xc0O\xa93\xe0Z\xdc*\
-0\x8d\x88\xf8\xb0\x82@\x80+\xafB\x04\x00\x1d:\x90\
-\x00uh@\xd1\xdf$\xb2\xbb\xd4\xbd\xbb\x9f\xfa\x15\xf1\
-o~\xfbu\xf5\x16\xfd-u\xd6H\x1aq\xde\xd80\
-\x08\xa8\xe5\x91\x00\x83\x7f\xbbd\x05\x81\xbfTwA\xe0\
-b(\xa5 \x10\xa0\xe53\xab]\x00\x00Z\xe2\x817\
-\xbc5\x1e\xfd\xf8\xafN\xff\xf0\xc1w'[\xf8l\x9c\
-D\xf6\xbc\xff\xf0\xe0`\x94\xfe\xf2k~(^\xf3\xea\
-\xefm\xe6\xa0\x966\xeb9\xbc\x0d\x82\x80qda\xcb\
-$Z\xf4l\xa1\xc1\xbfZ\xa3\xe1 ~\xe4\xfb\x9f\x1b\
-o\xfa\xc5\x1f\x8b\xbb\xee\xba\xa3\xce?z\x10\xd9\xca\x9f\
-\xe3\xe2\xb3\xe7\x9d\xef\xf9\x93\xe4s\x1e\xff5\xf1\xda_\
-\xfaU\xdf\x18@\x00`\x05\x80\x00\x00\xa0\x0c\x0d(\xfa\
-\x9b\xe6\x17\xff{\x8f{\xec\xe7\xa5\xef\xfd\x9dm\x17\xfd\
-\xddh\x1c\x0d\x5c>\xbff\x10\xd0\x8bl5\xc0$v\
-c5\x80\xc1\xbf$[*\x08,\xb6\x0a\x9c\x16\xff\x83\
-\x82@\x80[\xe7k\x01\x00\x00\x9b\xd9r\xd1\xdf$\xb2\
-e\xbf\x83^\xaf\x97\xfcw\xdf\xf3\xed\xcd(\xfa[N\
-cO\xc2k\x06\x01\xa3\xfc\xff?n\xe9[\xd9\xe0_\
-\x81-\x15\x04\x0e\xf2\xafID\x9c)\x08\x04\x88\x88\x16\
-\xf5\xd6\x09\x00\x00\x9a8-m\xbf\xe8o\x1a\xd9\xf2\xf3\
-[E\x7f\xcf\xfb\xd6\xa75\xe5\xf1\xfae\xc6\xcd\xc6/\
-\x99_#\x08\x18\xe5\x17\x18mZ\x09`\xf0\xaf\xc1\x96\
-\x0a\x02\x8b\xad\x02o\x85R\x0a\x02\x01\x01\x80\x00\x00\x80\
-\x15m\xb9\xe8\xefxa\xf8on\xd1\xdfM\x92\x18E\
-$\xad\x18\x94W\x0c\x02\xfa\xf9\xe05mx\x10`\xf0\
-\xaf\xd9\x96\x0a\x02G\x0b\x9f\x1b\xa1 \x10@\x00\x00\xc0\
-\x0a\x1ex\xc3[\xe3\xafl\xa7\xe8/\x8d\x88I\x92$\
-\xfd\x88\x18\x1c\x1c\x8c\xa2\xd1E\x7f\xcbD\x00\xe9\xacU\
-\xc5y+\x06\x01\x83\xc8J\x19\x9b\xf6H\x80\xc1\x7f\x8b\
-\xb6T\x10Xl\x158Y\xfc\xccR\x10\x08 \x00\x00\
-\xe0\x0a\x8bE\x7f\xc7\xf5\x17\xfd\x1dE\xc4iD\x0c\xd3\
-4mK\xd1\xdf\xceZ!\x088\x88l\xc9\xe1\xd4\xe0\
-\xcf\xa2-\x14\x04.\x96U*\x08\x04\xba\xca#\x00e\
-_X\x00\xec\xa2-\x16\xfd\xcd\xf2\x0b\xf6~\x92$\xfb\
-\xbd^/ZV\xf4w\xd3yx/\xd2\xf4l\xc7\x83\
-\x80~\xcc\xef\xben#\x080\xf87\xd4\x96\x0a\x02\x87\
-\x91\x85\x89\xf9#\x01\x0a\x02\x01\x04\x00\x00d\x93\xd3v\
-\x8b\xfe\x0e#+\xf0\x1aF\xc4\xfe\xa7~\xf2\xa3\xa2u\
-E\x7f7\xce\xff\xd1\x8f\xa47m\xfb_\xa3\x08\x02>\
-\xf8\xee7_\x17\x04\x14\x83W]\xcbGn\x0d\xfe/\
-{\xe1}\x06\xff\x06\xdbBA\xe0A~}y\xee\xbd\
-\xa8 \x10@\x00\xb0\xd6\xc5\x06\xc0.\xd8b\xd1\xdfY\
-~a>L\xb2;\xc7\xd1\xda\xa2\xbf\xa5\xcc\x92]\xf9\
-\x9b\x0c\xfa\xfd\x9b\x82\x80K\x07\xaf\xaa\x07\xff\x17\xdd\x7f\
-\x8f\xc1\xbf\xe1\xb6P\x10Xl\x158\xcd?s\x14\x04\
-\x02\x08\x00V\xbe\xe08\xf3\xed\x02v\xc1\x16\x8b\xfe\x8e\
-b~\xd7\x7fo\xdc\xfe\xa2\xbfeNsI$\xb1S\
-\xb7\x1bo\x0b\x02\xee:\x17\x04,\xee\x12P\xe6\xea\x87\
-4\x22\xe2\xc0\xe0\xdfZ[(\x08L\xf2\x10`q\xab\
-@\x05\x81\x00\x02\x00\x01\x00\xd0\x0d[,\xfa;\xc9\x87\
-\xc1a\xe4\xdbvu\xa7\xe8/\x1d\xc6,&\xbb\xf87\
-\xbb\x15\x04\xbc\xeb\xd2 \xa0\xac]\x02\xce\x0d\xfe\x1f4\
-\xf8\xb7\xde\x16\x0a\x02\x8b7\xcb\xb9\x9fC\x05\x81\x00\x02\
-\x80\x9b.@<0\x06\xb4\xd6\x16\x8b\xfe\x8a\x86\xffA\
-\x92$I\xaf\xd7\x8b\xef{\xfe\xbd\xf1\xaf\xff\x97\x9f\xd8\
-\x91\xa2\xbf\xa5\xcet\xc9.\xff\xf5.\x06\x01\x8f|\xc4\
-\x9d\x8b\x83\xd7~\xac\xb7\x12\xc0\xe0\xbf\xc3\x1e\xf5\x89\x7f\
->\xde\xfa\xc0\x8f\xc7\x8f\xfd\xc0\x0b\xea*\x08\x1cE\xb6\
-:\xe5V\x08\xa0 \x10\xd8A\xadxd\xbdM\x01\x80\
-\x0e\x00\xa0}g\x82\xed\x15\xfd\x15\xad\xf0\xa3\x88\x18G\
-D\x14E\x7f/~\xce3\xa2\xd7\xebP\x07\xec\xac\x1b\
-\xe7\x8f\x22\x08\xf8\xc0;\xdf\xb4\x18\x04\xec\xe7\x83\xd7i\
-\xfe\xb5\xd2\xe0\xff\xa1w\xbf\xc5\xe0\xbf\xa3\x92$\x89{\
-\x9f\xfe\xd4:\x0b\x02/\xdd*0BA  \x00\x10\
-\x00\x00\xec\x80-\x16\xfd\x15\xcb\xbe\x07\xc5\x1f\xb8\xdbE\
-\x7f7M:1\x8el%D'\x9c\x0b\x02^~\xeb\
-\xd1\x80\xfd\xfc\xebd\x95\xc1\x7f<\x1a\xfaA\xdeq[\
-(\x08<\xb7U`\x84\x82@@\x08 \x00\xb8\xfc@\
-&\xdeO@[l\xa9\xe8\xef8\xb2\xbbk\xa3\xfc\x22\
-;\xbaQ\xf4\xb7d\x0c\xd01\x83~?\xee\xfb\xe6s\
-\x8f\x06\x14%\x81\xa9\xc1\x9fE[(\x08\xbcl\xc7\x0a\
-\x05\x81\xc0.\x0c\xff\x8d\xef\xadkS\x00\x00\xd0x[\
-,\xfa\x9b\xe4\x17\xd0\xb7&\xb7\xee\x14\xfd9\x8f\xdc\x18\
-\x04<\xfdk\xe3\xcf\x1e\xfc\xb5\xe4\x95/\xb9?\xee8\
-\x18\xdf\xfa\xff\xee\xbc\xe3 ^\xf9\x92\xfb\x0d\xfeDD\
-\xed\x05\x81\x8b[\x05\x9e[\xf7\xaf \x10h\xf1\xb5F\
-\xe3\x9fc\xb2\x02\x00\xa0$[*\xfa;\xca\x87\xffa\
-D\x0c\x93$I;Y\xf4w\xf3Yd\x14\xe9\xc6\x8d\
-\xf8\xad6\x1e\x0d\xe3;\xef\xbd;>\xf8\xae7'?\
-\xfd\xaa\x97\xc4O\xfc\xd3\xef9\xfd\xc0;\xdf\x94|\xe7\
-\xbdw\x1b\xfc\xb9\xa5(\x08|\xf5\xcb\x9f\x1f\xfb{\x95\
-\x17\x04^\xb6U\xa0\x82@@\x00 \x00\x10\x00\x00\x0d\
-\xfe\x80\xdaN\xd1_\x1a\xd9\x9d\xb3\xfdX\xb8\xeb\xdf\xd9\
-\xa2\xbf\x9b\xc7\x8c\xc4b\xb2y\x10\xf0M_\xf7w\xe3\
-\x9eox\xca\x9e\xc1\x9fK\x7f\x5c\x92$\xee\xfb\xe6\xaf\
-\x8d\xb7\xfffm\x05\x81\xc3\xfc3\xed\xb6\x90NA \
-\xd0\xb2\x00@\x07@\xa9\x97o\x00\x0d\xb3\xa5\xa2\xbf\xe2\
-\xae\xff \x22\xfa\xc5d\xdb\xe9\xa2\xbf\xe5\xa6\x1a\xc7\xe0\
-\xe2\x85J\x92\x9c8\x0c\x5c\xa5\xe6\x82\xc0q\x5c\xb2m\
-\xa5\x82@\xa0\x85!\x80\x00@\x00\x00\xec\xa2-\x14\xfd\
-\xcd\xf2\x8b\xe3~dE\x7f\xd9U\xb3\xa2\xbf%\xcf\x22\
-\xe9\xbe\x81\xf7\xc25\xc0lv\xe60p\x9d\x9a\x0b\x02\
-\xf7#\x0b6'q~\xc7\x0a\x05\x81@[\x86\xff\xc6\
-\xcf\xac\x02\x00\x80\x15m\xa9\xe8\xef(\x1f\xfe\x07\xf9E\
-rD(\xfa[\xed\xb4\x9c\xecG\x9a\x9e:\x10N\xad\
-\xac\xae\xe6\x82\xc0b\xab\xc0\xdb\xb6\xefT\x10\x084<\
-\x00h\xbc\xb6\x04\x00\x89\xab\x14\xa0\x09\xb6P\xf4w\x12\
-\xf3\x92\xbfQD\x84\xa2\xbf\xcdR\x00\xc7\xe0\xdc\xe9u\
-\x10\xd1\xedrD\x96WsA\xe08\xbf\xf6;\x97\xb2\
-*\x08\x04\x1a\x1e\x004~\xbenS\x00\x00\xb0\xbdO\
-\xf4\xed\x14\xfd\x1dG\xb6\xec\x7f\xb8\xf8y\xad\xe8o\x93\
-od/\x89H4\x89\xdd:\xbb\xa6\xde@\xac\xf6\x96\
-\xa9\xb7 p\x14Wl\x15\x18\xa1 \x10hd\x00\xe0\
-\x11\x80\x92\xecE\xbb\x1eW\x00v\xc8\x16\x8a\xfe\xa61\
-/\xf9\x1bF\xcc\xcb\xb7\x14\xfdm<\xf0\x0e#\xd2\x89\
-\x03\xb1x\xb9\x92\xda\x1e\x81\x95\x15\x05\x81\xcf\xfe\x96\xaf\
-\x8b\xc5\xcf\xa8*~j\x17B\x80\x0b\xab\x01\x14\x04\x02\
-\xecr\x00\x00P\xbb-\x14\xfd\x1dGv!}\xee\xae\
-\xbf\xa2\xbfR\xc7\x09\xab\xca\xce\x1d\x8fd\x1c\x91\x1e9\
-\x10\xacj4\x1c\xc4\xab\xbe\xffyu\x15\x04\x8e\xe2\xf2\
-\xad\x02\xcf\x15\x04\xfe\xcc\x03\x0a\x02\x81-^aX\x01\
-\xd0\xad\x83\x09\xec\x8e-\x14\xfdM\xf2\x0b\xdbQ>\xfc\
-\xdf\xf27\x1e\xa3\xe8\xafTnx_rL\x12\xab\xec\
-X[\x8d\x05\x81\xa3\xc8n\x0a]\xfa\xa1|rz\x92\
-\xde}\x9f\x82@\xc0l\xbd\x0b\x01\x00@m\xb6P\xf4\
-7]\xb8\xb8\x8d\x88\xf3E\x7f\xbf\xf5\x06E\x7f\xe5J\
-F\x91\x86;\xde\xe7\x0eI\x1a\x91\xe8F`}5\x16\
-\x04\xf6#\x0bI\xa7\x91\xed\x14p\x8b\x82@`\xcb\xf6\
-\xc2\x0a\x00\x80\xf6\xd8B\xd1\xdfq\x5cx\xd6\xbf\xa0\xe8\
-\xaf\xea\x81\xd7\xaa\xb2\x0b\x07d\x18\xa9n\x046|\x17\
-\xd5[\x108\x88l\x97\x94Kw\xb1P\x10\x08\x08\x00\
-\x04\x00\x00W\xaa\xb9\xe8/\xcd\x07\xffdq\xf0W\xf4\
-W\xab4<\x09p\xf1\x90\x08E(E\x8d\x05\x81\xc5\
-V\x81\xb7\x85\x00\x0a\x02\x81-\xd0\x01P\xc1\x053@\
-\xe9j.\xfa;\x8al\xe9\xea0.\xdc\xf5W\xf4W\
-\xeb)z\x18\xc9\xe5w\x0e\xbb{L\x92\xbdH\xe2\xc4\
-\x81\xa0\x0c5\x16\x04\x16\x9f\xa5\x97m\x15\xa8 \x10\xa0\
-\xc5\x01\x00@\xb9\x93x\xbdE\x7f\xb3\xc8\xee\xfa\xef]\
-\x1c\xfc#\x14\xfd\xd5.u\xfe\xbb\xe4\x98\xf4#\x8d3\
-\x07\x822\xd5T\x10x\xe5V\x81\x05\x05\x81@M\xac\
-\x00\x00h\xa2\x9a\x8b\xfe\x0ec~\xd7\x7fp\xeb\x0c\xa1\
-\xe8o\xeb\x13/\x0e\x0a\xd5\xbb\xbd \xb0\xb2?j\x14\
-Y\xd8z\xc9#\x01\x0a\x02\x01\x01\x80\x00\x00\xe8\xdet\
-So\xd1\xdfY>\xf8\x0fb\xa1\xe1\xbf\xa0\xe8o\xeb\
-\xe7\xe8~\xa4\x96\xbc_\xb8l\x19Fb\x87\x04*x\
-k\x9d+\x08\xfc\xd4*\x83\xa6qD\xec\xc7\x15+\x01\
-\x22\x14\x04\x02\xdd\xe6\x8a\x13\xe8\x8c\x9a\x8b\xfe\x0e#k\
-\xa8\x1e\xe4\x17\xa3\xf9|\xa5\xe8\xafA\xf6\xa2w~\x1b\
-\xb1\xceK\xa3\x173\xd7\x06T\xa7\xa6\x82\xc0\xfd\xc8V\
-\x5cM\x22n\xff\x19W\x10\x08\x08\x00\xda\xc3\xb3\x89\xc0\
-Zj,\xfa;\x89\xec\xae\xff(.\xb9\xeb\xaf\xe8\xaf\
-q\x03\xaf\xe6\xfb\x8b\x92pK\x94J\xd5\x5c\x10x\x1a\
-\x97\xaf\x06P\x10\x08\x08\x00\x1a\x7f\x99&\x00\x00VT\
-s\xd1\xdfQ~\xb19\xb8\xec\xf3U\xd1_#\xcf,\
-\xbd\x08\x03\xef\x05\xe3H=\x06@\xf5j*\x08\x1c\xe5\
-\xbf\xef\x95\xbb~(\x08\x04\x04\x00\xcd\x0d\x00\x5c\xa4\x01\
-K\xab\xb1\xe8o\x12\xf3\xbb\xfe\xe3\xc5\xffC\xd1_\xc3\
-%1\x88H'\x0eD\xab\xaf\x0fh\xb1\x9a\x0a\x02G\
-1\xdf%\xe0\xb6\x90AA P\xf2\xcc\xea\x04_\xe2\
-\xc1\xd4N\x0c\xdc\xfcaQo\xd1\xdfq\xfe\xd94\x88\
-K\x02\x06E\x7f\xadH\x01|c.g\xd5\x1d\xf5\xfc\
-\x04\xd6S\x10\xd8\x8b\x1b\xb6\x0a\x8cP\x10\x08\x08\x00\x04\
-\x00@\xab\xbc\xef\x03\xff>\x1e\xf7\x15\xdf\x5cG\xd1\xdf\
-q\xfeu\xdb\xb3\xfe\x8a\xfeZw\xaavn\xb9m\x22\
-\x8b\xa1\x1d\x12\xa8[M\x05\x81\xc3\xb8b\xab\xc0\x88\xf3\
-\x05\x81\x8f\xfd\xb2\xa7\xa5\xff\xef\x9f~\xc07\x06\xd8)\
-m\x0b\x00\x00\xae\xf4\xc0\x1b\xde\x1a\x9f\xf5\x05OI\xdf\
-\xf6\x07\xef\xa8\xba\xe8o\x9a\x7f~^\xda\xe2\xa7\xe8\xaf\
-u\xc3\xee(\x22\xf5\xcc\xfb\xed\xc7\x05jWSA\xe0\
-8\x7f\x87O\xaf{\xf7\xff\xd1;\xde\x93\xfc\xe5/\xfc\
-J\x05\x81\xc0N\xcd\xacm\x0b\x00\x5c\x8e\x00\xb7\xa9\xb1\
-\xe8\xef0\xb2\xbbF\x83\xfc\xeb6\x8a\xfeZ;\xed:\
-\xbf\xdcn?\xd2+\x07$\xa8T\x0d\x05\x81\xc3\xfcs\
-|\x12\xd7<\xee\xa2 \x10\xd8\xb5\x10@\x00\x00\xb4\xda\
-\xef\xfd\xd1;\xe3\xb3\xbe\xa0\xf2\xa2\xbf4\xb2;E\xfb\
-q\xc9]\x7fE\x7f\xbbp\xaaN\xad2\xbb,\x00H\
-R\x0fA\xb355\x15\x04\x0e#\xdb\xbeur\xf9G\
-\x83\x82@`\xe5k\xc6Fw\xe8(>\x02Z;\xaf\
-\x15E\x7f\xef\xff`\xa5E\x7fG\xf9\xf0\x7f\xe5]\x7f\
-E\x7f; IF\x91^\xbdMX\x87\x0f\x8c`\x84\
--\xffh\xd6R\x10x\xe3V\x81\x11\x0a\x02\x81\xa5\x03\
-\x80F\x7f@\xb8R\x05Z\xa7\xa6\xa2\xbfYdw\x84\
-\xfa\x91\xdd!:\x7fQ\xaa\xe8o\xe7\xe6\x0ck\xcc\xae\
-\x1c\x8c\xf4#\xb0u5\x14\x04^\xbbU`\x84\x82@\
-@\x00\xb0\x8d\x83\xe9\xf2\x0c:\xae\xa6\xa2\xbf\xe2\xae\xff\
-0\xb2e\xff\xb7Q\xf4\xb7\xb3'm\xceKl\x93H\
-S\xd4P\x10\xb8\xccV\x81\x0a\x02\x81V_O\x08\x00\
-\x80V\xa8\xa9\xe8\xafx\x0et\x10W4\xfcG(\xfa\
-\xdb\xe1Qw\xa0\xf4\xee\xb2\xb3\xef,\xf5(\x00MR\
-SA\xe0Y\xdc\xf0H\x80\x82@\xe0\x8a\x99U\x00P\
-\xea\xe5\x19\xd095\x15\xfd\x1d\xe7\x17|\xc3\x88\xd8\xbb\
-\xed\xc3G\xd1_\x17N\xd9{\x11J\xefn?\xf3&\
-\xa3\x88\x99~\x04\x1a\xa5\x86\x82\xc0\x83\xfc:\xf9\xca\xc4\
-YA pE\x00\xd0\xe8\x19\xbbM\x01@\x22\x00\x80\
-\x8e}\x82\xd6S\xf4W,\xf5\xbc\xf6\xae\xbf\xa2\xbf\xce\
-L\xbb\x0e\xc1\xe5\xc7\xc5\x9b\x9e\xe6\xbd+\xab/\x08,\
-\xca_\xa7qC\xab\xb7\x82@`!\x00h4\x01\x00\
-\xd0H5\x15\xfd\x1d\xe7\x1f\xd4\xc3\xcb>\x0f\x15\xfdu\
-r\xfe\xefE\x92\x9e9\x10\xb7]\xcf$\x91$\xa7\x8e\
-\x03MTqA`\x92\x87\x00'q\xcd#\x01\x0a\x02\
-\x81\x0b\x9f\x1b\x02\x00\x01\x00\xb0\xac\x1a\x8a\xfe&\x91\xdd\
-\xd1\x19\xc5%\x0d\xff\x05E\x7f\x9d\xa4\x07\xe0\xf2S\xf0\
- \x22=q\x1ch\xaa\x1a\x0a\x02G\x0b\xe7\x8fk/\
-\xfa\x15\x04\x02\x02\x80r\xec\x09\x00`\xb7\xd5T\xf4w\
-|k\xd0\xbb\x86\xa2\xbfN\x9f\x1a-w\xbf\xcc,u\
-\x0e\xa6\xf1*.\x08\x1cE\xb65\xec\x8d'(\x05\x81\
-\xd0YI\xe8\x00(5\x00\x00vT\x0dE\x7f\xc7\xf9\
-E\xdb\x95w\xfd\x15\xfd\x91\x0d\xba\xa5\x0f\x0d\xbb\xa1\x17\
-\xfd\x88d\xe2@\xd0t\x15\x17\x04\xf6\xf2sH\xb1\x92\
-\xecR\x0a\x02\xa1\xb3\x1a?\xb3\xb6\xed\x11\x00`\xc7\xd4\
-P\xf4\x97\xe6\x17jI\x5c\xb3\xdc?B\xd1\x1f\xc5\x99\
-1\x1dF\x1aZ\xefo\xfbIJ\xf6\x22R\xc1\x08\xed\
-\xb8h\xac\xbe p\xa9\xad\x02#\x14\x04B\x07\x03\x00\
-\x1d\x00\x00\x97\xa9\xa1\xe8\xef(\xb2;4\xc3\xab\x86\x7f\
-E\x7f\x5c>=\x08\x9d\xaf\x8a\x01\x1c\x02\xda\xa4\xe2\x82\
-\xc0q\xdc\xb0U`\x84\x82@\xe8\x98\x9e\x00\x00\xe0\x12\
-\x15\x17\xfd\xcd\xf2\x0b\xb2^\xdcp\xd7_\xd1\x1f\x06\xdd\
-\x95\x07\x9e#\x87\x816\xa9\xb8 pq\xab\xc0\xebn\
-\xef+\x08\x04\x04\x00.\xc8\xa0{j(\xfa\xbb\xf1\xae\
-\x7fA\xd1\x1f\x06\xdd\xb5\xce\xc4n\x1e\xd0J\x15\x16\x04\
-&\x0b!\xc0\x8d\x8f\x04(\x08\x84\x9dg\x05@W\x0e\
-&p\xbd\x8a\x8b\xfe\xce\xf2\x8b\xaf~\xcc\xb7k\xba\xfd\
-CD\xd1\x1f\xce9\x9b\x1e\x954\x92D O+U\
-\x5c\x108\xcaC\x85kC\x00\x05\x81\x80\x00\x00\xd8i\
-5\x14\xfd\x1dF\xc4Idw`\xf6\xaf\xfb\x85\x8a\xfe\
-X\xfe\x8dk\xd5\xd9\x95CN\x9a*I\xa4\xb5*.\
-\x08\x1c\xe7\xe7\xa1\xe92\xbfXA \xec\xe6\xc7\x8c\x00\
-\x00\xe8\xac\x8a\x8b\xfeN\xf3\x8b\xacQ\x5cw\xd7_\xd1\
-\x1f\xeb%\x00#\xdb\xde\xb5\xf3\xe2\x06\x96QaA\xe0\
-~d\x81\xf4$\xb2p\xfa\xeaO\x19\x05\x81\xe0\x1c)\
-\x00\xb8\xf9\x8a\xcc{\x0a\xda\xa1\xe2\xa2\xbf\xa3<\x00\x18\
-\xdc\xf4Y\xa6\xe8\x8f\xf5N\xdfI\x12\xe9\xcc9\xe7\xf2\
-\xab\x87^\xfe\xf3\x07\xadV\x14\x04\xbe\xf1\x17^]E\
-A\xe00\xff9\xb9i\xc5\x8c\x82@@\x00p\x0d\x17\
-\x1c\xd0p\x15\x17\xfdM\xf2\xafk\xef\xfa\x17\x14\xfdA\
-\x05f1\x884u>fg|\xe9\x17\x7fQU\x05\
-\x81Km\x15XP\x10\x08\x08\x00\xceK\xe3\xfa-V\
-\x80-\xab\xb8\xe8\xef8\xff\x1c\x18\xc65\xbf\xaf\xa2?\
-\xca\x93\xecE\x9a\x9e9\x0e\x97\x1d\x1a\x87\x80\xddRa\
-A\xe0\xb2[\x05*\x08\x04\x04\x00\x02\x00h\xc9\x0fg\
-\xb5E\x7f\xc7\xf9\xd7Rw\xfd\x15\xfdQ\xe2\x90\xdb\x8f\
-$\x99:\x10\x97\x1e\x9cA,\xb1\xe5\x19\xb4\xea]]\
-]A`\xb1U\xe0I,\xb9\xc5\xa8\x82@h\xefe\
-\xb1\x00\xa0\xdc\x83\xe9yLh\x98\x8a\x8b\xfe\xa6\xf9\x85\
-\xd3\xe8\x86++E\x7fT\x17\x03p\xf95\x84#\xc3\
-\x8e\xaa\xb0 p\x98\xff\xf3\xc6\xf0l\xb1 \xf0\x0b\xbe\
-\x5cA \xd0\xdd\x00\x00h\x90\x0a\x8b\xfe\x8a\xbb\xfe\x83\
-\x85\x0b\xa6+)\xfa\xa3\xc2\xf9?\x89\xc4\xea\xb3+\xce\
-\xca\xce\xcb\xec\xac\x0a\x0b\x02\x8b\xad\x02\x97\xe9\x05H\x22\
-\x22\xfe\xf0A\x05\x81`f\xedf\x000\x0bwb\xa0\
-\x11*,\xfaK#\xbb\xeb\xdf\x8b%\x96\xfbG(\xfa\
-\xa3\xf2\xf3\xf80\xd2\xd4v\x80W\x0d2\xe9r\xcb\x99\
-\xa1\xad**\x08\xdc\x8f,\xdc\x9e\xc6\x92\x05\xd7\x0a\x02\
-A\x00\xd0\xc5\x00 \x15\x00\xc0\xf6UX\xf4w\x94_\
-\x0c\x15\x85IWR\xf4G\xad\xca\xac\x03\xdb=\x8a6\
-\xd8y\x15\x17\x04\x9e\xc4R\x8f\x04(\x08\x04\x01@7\
-\x03\x00`9\x0f\x86E\x00\x00 \x00IDAT[\
-?\x80\xd5\x15\xfd\xcd\x22[\x0a\xd9\x8f%\x96\xfbG(\
-\xfa\xa3f3\xe7\x9f\xab?\x18\x92\x88H<\x22\xc1\xce\
-\xab\xb0 p\x1cY\x90\xbet\xe1\xa8\x82@h\xfc\xcc\
-\xda\xd8\xeb\x06W\xcd\xc0R*,\xfa;\x8a\xec\xee\xc7\
-0\xb2%\x91W_|)\xfackW\xfe1\x8e\xb0\
-\xd4\xfd\xf2+\x09\x8fH\xd0-\x15\x15\x04\x0e#\x0b\xc1\
-o\xdc*0BA \xb4@c\xb7\x10n[\x00\x90\
-\x84U\x00P\xbb\x8a\x8a\xfeNb\xc5\xbb\xfe\x8a\xfeh\
-\xc09\x88K\x8fL\xea\xd8\xd0)\x15\x15\x04\x16[\x05\
-NCA \xb4Y\xa3\xb7\xaeo\xe3\x0a\x00\x17\x19P\
-\x93\x0a\x8b\xfe\x8e\x22KFo\xbc\xeb_P\xf4GC\
-N\xe8\x5c~j\xde\x8bHO\x1c\x07\xba\xa6\xa2\x82\xc0\
-Q><\x1c/\xfb/(\x08\x84\xc6\x11\x00\x94x\xf1\
-%\x00\x80\x1aTT\xf4W\xdc\xf5\x1f\xc6\x12\x0d\xff\x8a\
-\xfeh\xd8\x19h\x14\xe9\xf2\x17\xe4\x1d\xd3\x8f\xb4\xb9\xcb\
-\x1d\xa1J\x15\x15\x04\x8e#b/\x96[\x09\xa0 \x10\
-\x9a7\xfc\xeb\x00\x10\x00@K~\xc8\xaa+\xfa;\xce\
-?\x10\x87\xcb~\xf6(\xfa\xa3Q\x12\xe7\x9f\xeb\x8fO\
-b\x85\x04\x1d~\xfbWR\x10X<\x227\x89%\xb7\
-\x0a\x8cP\x10\x08\xecV\x00\x10\x02\x00\xa8NEE\x7f\
-\x93\xc8\x9eg\x1c\xc5\x12\xcf\xfa+\xfa\xa3\xd9g 3\
-\xee\xd5W\x14\xbd\xa1\x15\x12t]\x85\x05\x81\xd3X\xf2\
-\x91\x00\x05\x81\xb0u\x8d\xbei\xdd\xc6\x12@\x01\x00T\
-\xa0\xa2\xa2\xbfI\xfe!8X\xf6_P\xf4G\xc3\xcf\
-B\xfb\x11\xe9\xa9\x03q\x89\xd9\xac\x17=\xa7h\xa8\xa8\
- \xf0 \xff\xe7\xb2!\x9b\x82@@\x00\x00\xdc\xae\xa2\
-\xa2\xbf\xe3X\xe1Y\xff\x82\xa2?\x1a/M\xf6#I\
-\x94\xdd]\x1d\x028\x06\x90\xab\xa0 p\x14Y\xa0~\
-\x12+\x14\x8c)\x08\x84\xad\xcc\xac\x8d\x9d\xb3\x05\x00\xd0\
-a\x15\x14\xfd\xa5\xf9\xe0\xdf\x8b%\xb7\xf6S\xf4G\xfb\
-B\x00[\xde]\xf3\x03=\x8al\x97\x0f *)\x08\
-\xecE\xd6\x0dP\x94\xea.\xf1\x91\xa5 \x10\xb60\xb3\
-6V\xdb\x02\x80=\xef'(c~\xa9\xa4\xe8\xef(\
-\xb2g\x14\x87\xb1\xc2\x92\x7fE\x7f\xb4\xef\x07(\xe9E\
-$nu_y|\xc2\x0f2,N\x02\xd5\x14\x04\x0e\
-#[\x05\xb0\xd2\xd2=\x05\x81P\x8b\xfd\xd0\x01 \x00\
-\x80\xa6\xa8\xa0\xe8o\x96\x0f\xfe{\xb1\xec]\x7fE\x7f\
-\xb4\xfaj>\x06\x11\xe9\xc4\x81\xb8\xfa\x07<\x1a\xbc\xff\
-1lK\x05\x05\x81\xe3\xfcZ~\xe9\xcf#\x05\x81`\
-fm\xe3#\x00\xc0\x9a^\xf7+\xbf^v\xd1\xdfa\
->\xfc\x0fB\xd1\x1f\xdd\x1ar\x9d\x8f\xae6\x8c\x15\xef\
-JBWTP\x10\xb8\xceV\x81\x0a\x02\xa1\xc3s\xab\
-ez\xd0\x01E\xd1\xdf\xd7\xdc\xf3\xbc\xb2\x8a\xfe\xce\x16\
-\x06\xff\x95&xE\x7f\xec\x84\xd4v\x80m\xbd\xf0\x81\
-&\xa8\xa0 \xb0\xd8*p\xa5\x93\xbc\x82@\x10\x00\x00\
-;\xa6\x82\xa2\xbf\xa3\x85\xe1\x7f\x7f\xa9O@E\x7f\xec\
-\xdey]\xd9\xdd\xf5\x97=\xfb\x91\xc6\xd4\x81\x80\xabU\
-P\x10x\x90\x07\x09\xcbn\x15\xa8 \x10\x04\x00\xc0\xae\
-\xa8\xa0\xe8\xef4\xe6%\x7f\xe3U\xfeEE\x7f8\xb9\
-w\xed\x03(\xf6C\x0f\x00\xdc\xfc!R~A`\xb1\
-U\xe04V\x5cU\xa0 \x10\xba\xc1\x958\xec\xa0\x0a\
-\x8a\xfe\x8e\xf2\x00`\xb0\xec\xe7\x86\xa2?:0\xe5\xa6\
-\xe1I\x80\xebc\x00`)%\x17\x04\xf6\xf2\xf3\xf5\xd2\
-[\x05f\x9fh\x0a\x02\xa1DV\x00\xb8\xa8\x80z\x94\
-\x5c\xf47\xc9\xbfF\xb1\xe2\xb3\xfe\x8a\xfe\xe8\xc0\xb9}\
-\x14Iz\xec8\x5cux\x92QD\xea1\x09XR\
-\x05\x05\x81\x83\xc8V\xe2\xac\xf29\xa5 \x10v\x5c[\
-\x03\x803\xdf:8\xaf\x82\xa2\xbf\xe27\x19\xae\x1a\x22\
-(\xfa\xa3+#n\xa4\x9e\x02\xb8Z\x9aD\x19O5\
-C\xc7\x94\x5c\x10Xl\x15\xb8r'\x87\x82@\xd8\xf0\
-\x1aA\x00 \x00\x80\xaa\x94\x5c\xf4w\x94\x0f\xff\xc3\xfc\
-k\xb9O\xb9$\x14\xfd\xd1\xc1\xd3\xbb\x05i\xd7\x9a9\
->\xb0\x8e\xc5\x82\xc0\xbd\xbd\xbdM\x93\xb4b\xab\xde\xe9\
-*\xd7\xd0\x0a\x02a7\xb51\x00HC\xb1\x10\xe4'\
-\xe7\xd2\x8b\xfe\xa6\xf9\xe7\xc2p\xd5\x7f\xf1S?\xf9\x93\
-\x14\xfd\xd1E\xfdH\xe3\xc4a\xb8B\x92\x8c\x22\xb5[\
-\x02\xac\xf7\xe3\x93\x15\x04>\xf8\x9b?\x17\x9f\xf1i\xa5\
-\x14\x04\x16\xbd\x00+?\xba\xa4 \x10\x04\x00\xdb\x0e\x00\
-\xdcR\xa0\xf3J.\xfa;\xce\xbf\x06\xab\x0c\xff\x8a\xfe\
- \xd9\x8b^r\xea8\x5c{\xa5\xe11\x00\xd8@\xc9\
-\x05\x81\xa3\x85\xf3\xfe\xf2\x17\xdf\x0a\x02a\x9d\x99U\x00\
-\xb0\xeb\x07\x13\xeaRb\xd1_\x1a\xf3\xbb\xfe+7\xf5\
-)\xfa\x83\x88H\x15\x01\x5ck\x96$\x91\xa4\x1e\xdd\x83\
-M\xa6\xf6r\x0b\x02\x17\xb7\x0a\x5c\x85\x82@\xd8\x01\x02\
-\x00h\x91\x92\x8b\xfe\x8ag\xfd\x8bg\x03W\xa2\xe8\x0f\
-n\x9d\x95z\xe1\xd1\xb4kF\x86t\x18i2u \
-`s%\x16\x04\x16[\x05NBA tjfm\
-c\x000\x8b\xb0\x9c\x90\xee)\xb1\xe8o\x96\x9f\xf0\xf7\
-b\xc5\xbb\xfe\x8a\xfe\xe0\xb2\x1f\x8c\x18D\xa4\x13\x07\xe2\
-\xba\xcb \xab$\xa0,%\x17\x04\x0e#+\x06\x5c\xf1\
-\x91\x00\x05\x81 \x00\xa8\xf7`\xba\x90\xa0C\xd7\xcd\xa5\
-\x16\xfd\x1dEV\x004\x8c5\xee\xfa+\xfa\x83+S\
-\x00?\x10\xd7\x1e\x9e\xa4\x1f\xf3\xadE\x81\x8d\x7f\xa4\xb2\
-\x82\xc0\xb7\xff\xc6\xcf\x96Q\x10Xl\x15\xb8\xd6\xcf\xa8\
-\x82@\x10\x00\x00%y\xdf\x07\xfe}<\xfe\xef\xdcS\
-F\xd1\xdfI~b\xef\xc7\x8a\x0d\xff\x8a\xfe`\xa9\xd3\
-\xbc\xc7\xd3\xae\xb7\x17\x91:FP\xb2\xbf\xfa\xe8\xcf*\
-\xab p\xad\xad\x02#\x14\x04B\xdb\xb45\x00p\x11\
-\xc1\xce+\x8a\xfe~\xe7\xf7\x1f\xdc\xb4\xe8\xef(?\x99\
-\x0f#b\x7f\xd5\x7fY\xd1\x1f,!\x89QDj\xbb\
-\xbb\xeb\x0f\x92\x98\x04*PbA`\x12\xebo\x15\xa8\
- \x10n\x9fW\x1by\xd6kc\x00`\xf9?;\xad\
-\xc4\xa2\xbf\x93\xc8\x92\xfca\xac\xd1\xf0\x1f\xa1\xe8\x0fV\
-<=9?]o\x1cI\x08I\xa0\x22%\x16\x04\xae\
-\xb5U\xe0\xad\x8b\x0f\x05\x81P\xfc\xfc5r\x07\x1c\x8f\
-\x00@\x83\x94X\xf4w\x98\x7f\xe8\x0cV\xfd9W\xf4\
-\x07\xeb\x9e\xea-q_\xe2r\xc8u\x07T\xa8\xc4\x82\
-\xc0b\xab\xc0\x95\xefD(\x08\x84[\x04\x00%r\x97\
-\x85\x9d\x9b\x1bJ*\xfa+\xb6\xf3\x19\xc7\x9aw\xfd\x15\
-\xfd\xc1\xbag\xa6d\x14\xe9zw\xcc\xba\xf4i\x17\x89\
-\x07\x01\xa0\xda\x8f\xa2\xd2\x0a\x02{\x91\xad\x22\x9cD\xb6\
-\xaape\x0a\x02\xe9\xb0\xc6\xbe\xe1\xed\x02\x00[\xf6\xff\
-\xb7ww\xa1\xd6m\xe7]\xc0\x9f\xb9\xf6\xde\xeb\xe3\x18\
-/D\x0aZL\xcd\x87\x04\xa9\x01\xb1\xc99\x07\xb4\x90\
-\x1bkB\xdb\xd8\x8b\xa6\x085\xa6\x98\xd6\x8b\x22^(\
-4J\xedU\xad\xadB\x10jz\x0a\x85R1\xc1j\
-E\x0f\xb66 \xf5\x22*\xb4%i\x13H\x14r\x90\
-\x04z\xe1E\xd3\x98(\xa8g\x7f\xbekx1\xe7:\
-\xefz\xdf\xb3\xf7^k\xce9\xe6\x5c\xf3\xe3\xf7\x83M\
-r\x92s\xde\xb3\xf6Xk\xcd1\xc63\xc6\xf8\x8f\x8c\
-A\x7f\xd7\xd5\xf7cY\xf7;\x22\xe8\x0f\xf2\x8c\xbbE\
-\xd4\x1c\x9c\x99(\x92@O2\x06\x04\xae\xa2Y.\x80\
-\x80@\xe6N\x06@\xdeA\x16\x8c_\xa6\xa0\xbf\xabj\
-\xf2\xdf\xf8\xac\xbf\xa0?\xc86\xc1U\x018<\x1c\xb2\
-\xb5\x08z\x921 \xf0\x85h~U\xa0\x80@\x14\x00\
-\x14\x00Z7\xa4\x02\x00\xa3\x961\xe8\xef\xba\xfa>\xac\
-\x9a\xfe\x01\x82\xfe g\x01 \x96\x91\xe2FC<\xda\
-FE,\xe2NC@\x7f2\x05\x04\xee_\x15\xd8h\
-{\xb3\x80@ff\xe1E\xe5\x1a:(\x000b\x99\
-\x82\xfe.\xe3\xe9\xaa\x7f\xed\xc9\xbf\xa0?\xe8H\x8a\xb3\
-\x88\xe4\xa0\xeb\xa1ID*n5\x03\xf4+S@\xe0\
-\xfeU\x81\x02\x02\xe1\xf1\xef\xca )\x00@_\xf3\x82\
-g\x82\xfe\xbe\xd1\xf4\x8f\xd9FYy?\x8b\x16\xab\xfe\
-\x82\xfe\x80\xd3>\x10\xb7\xfaq8\xc5 :_@\xe0\
-\xaa\x1a\x934\xce\xf4\x10\x10\xc8\xc4-\x86:g\x1dk\
-\x01\x00F\xe5\xcdA\x7f\x8d>\xc7\xafW\x93\xff\xdd\x16\
-\xbc\xba_\x1cA\x7f\xd0K/\xb5XD\x91\x9eh\x88\
-Gg!\x17\x91\xe2ZC\xc0id\x0a\x08\xdcD\xc4\
-y56\xa9M@ \x13w\xae\x00\x90\xcf\x99\xcf\x13\
-c\x92!\xe8\xef\xc9\xde\xc4\xbfqB\x9f\xa0?\xe8K\
-Z\xc6V\x0e\xc0\xe3M\x14g\xae\x03\x84\xd3\xca\x14\x10\
-x^\x8dO\x9a^\x15( \x90\xa9r\x04@\x01\x80\
-\xb9\xc9\x14\xf4wYu\xa8\xcb\xaa\x93mD\xd0\x1f\xf4\
-\xdd\xbb.\xecV;\x5c\x05P\x00\x80\x01\xc8\x14\x10\xb8\
-\x8a\x88\xbbj\xdc\xd2\x88\x80@\x14\x01\x14\x00F\xd5\x90\
-\xb0/C\xd0\xdf.\x5c\xa7\xf1\xd5~\x82\xfe\xe0\x84\x9e\
-D\x11a\x85\xfb\xc0Sj\x13\xa9\xf9d\x01\xc8'S\
-@\xe0\xa6\x1a\xa77Z\xf5\x10\x10\x88\x02\x80\x02\x00\x8c\
-N\xa6\xa0\xbf\xcb(\xab\xe8\xab6\xdfQA\x7fp\xca\
-\xde5\xad\x22\xa5+\x0da\x1c\x02\xa3\x99\xa9\xe4\x09\x08\
-\x5cG\xcb\xab\x02#\x04\x04\x82\x8e\x17F C\xd0\xdf\
-u<]\xf5\xdf4\xea\xbc\x05\xfd\xc1\xb0F\xd3\x1c\x92\
-\xdaL\x12\x80\xfc2\x04\x04\x16{E\x80\x86\xbb\x01\x04\
-\x042\x8d\x91\x80\x02\x00LT\x86\xa0\xbf]\x07\xd9j\
-\xd5_\xd0\x1f\x0cjn\xeb\x08\xc0\xe1\xa1\xd1:\x22\xb9\
-\x0d\x00\x06&S@\xe0:\xca\xe2\xc1U\xe3'D\x08\
-\x08\x04\x05\x80\xa7\xac\x18pr\x19\x82\xfe\xae\xab\x8eq\
-U\xfd4\xf6\xf2{\xde-\xe8\x0f\x865\xbb\xddD\x14\
-\xce\xb8\x1fl&;%`\xa82\x04\x04\xae\xa3\x0c\xf0\
-nU\xe8\x13\x10\xc8X{8\x05\x80\xbc\xee|\xa68\
-\xa5\x0cA\x7f7{\x9dc\xc3q\xf3\xd3\xa0\xbf\xdf\xfa\
-\xf5_\x12\xf4\x07\x83\x93Ln\x0f6Q,\xa2(n\
-5\x04\x0cS\x86\x80\xc0\x8b(\x179n\x9a\x8e\xdf\x05\
-\x04\xa2\x00\xa0\x00\x10a\x07\x00\xa7\x1a\xab\xb6\x0f\xfa\xbb\
-\x8a\xb2\x12\xbe\x8c\x96\xab\xfe\x82\xfe`\xf0\x93[\xc7\x00\
-\x0e[\xc6v\xfbD3\xc0\x80g1y\x02\x02\x97Q\
-\xder\xd4* U@ \xcc\xb3\x00\x90\xc2\xf5J\x9c\
-@\xcb\xa0\xbfTM\xfc\x17m&\xfe\x82\xfe`T\xdd\
-\xd5:\xa2p\xc6\xfd\x98'\x1b0x\x19\x02\x02wW\
-\x056.\x02\x08\x08ddsV\x05\x80\xa97(\xd3\
-\xd52\xe8\xef2\xca\xado\xab(+\xe0\x8d\x09\xfa\x83\
-1\xcdk\x8b\x22\x920\xc0#\x1aj\x19-W\x05\x81\
-~d\x08\x08\xdc\xe5\x1e\xb5\xb9*P@ \xcc\xac\x00\
-`0EoZ\x06\xfdm\xa3\x5c\xf5?\x8b\x96\xdb\xfd\
-#\x04\xfd\x81.k\xaa\xf3\xff\xe4\x0c\x13\x8cL\xcb\x80\
-\xc0\xd6W\x05\xee\x08\x08\xc4\x00`\x1e\x05\x80m\xd8/\
-H\x0fZ\x06\xfd]Fy\xd6\xad\xd5\xaa\xbf\xa0?\x18\
-\xfd\xec\xf6,Rr\xc6\xfd\xf08I\xa5\x04F&C\
-@\xe0\xba\x1a\xd7\xb78\x12  \x10\x05\x00\x05\x00h\
-=\x0cm\x15\xf4\xf7$\xcaj\xf6.\xf5\xb6\x15A\x7f\
-0\xf6\xf9\x7f\x5cDH\xb9?\xa2\xa16\x11\xc9\xb5\x89\
-0\xb6on\xfb\x80\xc0MD\x9cG\xcb\x9d\x00\x11\x02\
-\x02a\xca\x05\x00\xe8L\xcb\xa0\xbf\xfdU\xff\xf3\xe6\xf3\
-\x05A\x7f0\xad\xdeV\xcd\xfa(I\x95\x13\xc6\xaae\
-@\xe0y5v\xba\x8e\x16W}\x0b\x08dh\xbd\x9a\
-\x02\xc0\x0c\x1a\x94qk\x11\xf4w\x1bOC\xfeZ'\
-\xf3\x09\xfa\x83\xa9\x0d\x01R\x11\x85\xebk\x0f*\xb6\x11\
-E\xa1\x9d`\xa42\x05\x04\xdeE\xbb\xdd\x00\x02\x02a\
-\xa2\x05\x00\xc8\xa6e\xd0\xdf\xebQn\xfb_\xe6\xf8N\
-\x09\xfa\x83IZEJ\xae\x03<<n_\xc5v\xab\
-\x9d`\xe4Z\x06\x04\xae\xab\xbf\xbf\xf5\xcd \x02\x029\
-1;\x00`\x88>\xff\xc5/7\x0d\xfa\xbb\x8er\xd5\
-\x7f\x13-W\xfd\x05\xfd\xc1\x1c\xe6\xb6\x85s\x00G\xb5\
-\x93\x8c\x1f\x98\x82\x96\x01\x81\xebxzK@\xe3I\xd4\
-\xf3\x01\x81\xbf\xfd\xbb\x02\x02Q\x04\x18k\x01\xc0\xe0\x80\
-\xf6\xdf\xc6*\xe8\xef\xa5\x0f\xfcP\x93\xa0\xbf]Uz\
-\x99\xe3\xf3(\xe8\x0ff1\x04pt\xed\xa8\x1e\xbe8\
-\x8b\xf2X\x150\xfa\xafs\xab\x80\xc0Ed\xba*0\
-\xa2\x0c\x08\xfc\x0b\xdf+ \x90\xde'\xff\x83\xbb\x05\xc8\
-L\x83Yj\x11\xf4wUuB\xebh\x99\xf0/\xe8\
-\x0ffg\x13eP(\x8f\x0f\x97.\x22\x85k\x13a\
-BZ\x06\x04\xae\xa2\xe5U\x81\x11\x02\x029Y\x01`\
-p\xd5\xa61\x17\x00\xec\x02\xa0\x91\x16A\x7f\xd7\xd5\xdf\
-\xbb\xca\xf1:6\x1bA\x7f0C\xfa\xae\xa3Z)\xd9\
--\x01\x13\xf3L@\xe0[j\x07\x04n\xaay\xcbM\
-\x8eg\xb0\x80@z,\x008\x02\x90\xb11\x0d\xa2\xa8\
-\xa5E\xd0\xdfe5\xf9_\xe5\x9a\xfc\xbf\xfc\x1d\xefN\
-_\xf9\xac\xa0?\x98\xe9`\x80\x83C\xf4b\x15\x85\xdd\
-\x120E\xdf\xf5\xbe\x97\xe3+\x9fk\x14\x10\xb8\xac~\
-\xae#\xc3\xb6j\x01\x81\xcc\x95\x1d\x00\xccB\xc3\xa0\xbf\
-\x14e\xa5\xf9<\xc7\xc4\xff\x99\xa0\xbfO\x0b\xfa\x83\x99\
-ZE\x86d\xeb\xc9K\xb1\x88\xa4\x9f\x87\xa9j\x19\x10\
-\xb8\x8a2'\xa4U.\x80\x80@z\x9a\xaf\xda\x01\x90\
-mh\xa0\x00\xc0Q\x0f\xf7\xc6A\x7f\xbbU\xffeD\
-\x5c\xe4x-\x82\xfe\x80\x88X\xd8\x03P\xab\xaf\x07\xa6\
-:3j\x17\x10\x98\xed\xaa\xc0\x08\x01\x81tZ\x00\x18\
-\xe0@Dc2Q\x0d\x83\xfe\xb6Q\xae\xfa_D\xcb\
-\xab\xfd\xaa\x0f\xaa\xa0?@\x09\xa0\x99M$\xc7\x00`\
-\xeaZ\x04\x04f\xb9*0B@ \x9d9\x1b\xe2|\
-{\xcc\x05\x00E\x00\x1e\xd40\xe8\xef\xb2\xeaD\x96Q\
-n\xfbo?z\x15\xf4\x07\xbcy\xa8y\x11\x85k\xee\
-&>N\x01jh\x11\x10\x98\xf3\xaa@\x01\x81tQ\
-\x00\x18\xdc\x9cu\xac\x1d\xebB\x01\x80{g\xf0\xcd\x82\
-\xfev\xe7\xc8V\x91a\xd5\x7fG\xd0\x1fp\xff\xfc\xbf\
-8\x8f\x14w\x1a\xe2h\xae\x04\x84\x99h\x11\x10\xb8\xaa\
-\x9e\x15Y\x8e\x04\x08\x08d\xca\x16^7S\xd10\xe8\
-\xef*\xcam\xff\xab\x1c\x9f+A\x7f\xc0\xb1\x8f\x0bM\
-pT+\xad\xa2\xfd\xb5_\xc0\x88\xb4\x08\x08|\xa1\x1a\
-\xcb\xb5\xdd\x09  \x90I\xf7\xf7c\x9dH\x0fr;\
-\x05\xa7\xd10\xe8o\xb7Ul\x19\x99\xae\xf6\x8b\x10\xf4\
-\x07\x1ci\x1b\x8bH\xb2\x00\x8e{\xc8\xeb\xefav3\
-\xa6\xe6\x01\x81\xbb\xab\x02o\x22\xd3\xee!\x01\x81L\xcd\
-\x983\x00\x0c\x9ch\x1a\xf4wU}~\xf2\xac\xfa\x0b\
-\xfa\x03\xea\xf7\xbe\xcb(\x5c\x07x\xdcC6\x9dG\xb2\
-\x0b\x00\xe6\xa8a@`Q\x15\x01n#\xc3\x91\x00\x01\
-\x81d\x98\xb7*\x00@\x0e\x0d\x82\xfe\xae\xab\x8e`\x1d\
-\x19W\xfd\x05\xfd\x01\x0d\x87\x04V\xb6\x8fk\xa8\xf3(\
-\x92e7\x98\xa9\x16\x01\x81\xeb\xbd\xf1_\x96I\x9c\x80\
-@\xa6`\xec\x05\x00\xbb\x00f\xa8a\xd0\xdf\xcds\x9d\
-A\x16\x82\xfe\x80\xc6\xb6\xba\xb0\x1aco\x8d\x053\xd7\
-0 p\x1d\xe5\xd5\xce\xd7\xb9^\x87\x80@\xeav`\
-\x0a\x00y'\xff\x92\x81g\xa6A\xd0\xdfUd>\xeb\
-/\xe8\x0f\xc83$(\xd6\x11\xc9=\xf7\xc7YGy\
-U+0c\x0d\x03\x02\x17\xd5\x18\xf0:2\x84\x8a\x0a\
-\x08d\xec\xc6\xbe\x03@\x01`&\x1a\x04\xfd\xa5\xeaA\
-_D\xc6\xed\xfe\x11\x82\xfe\x80\xbcU\x00mp\x5cC\
-E*<p\x816\x01\x81Y\xaf\x0a\x8c\x10\x10\xc8\x91\
-\xfd\x97\x02@\xbe9a\x94\xd7\xb71q\x0d\x82\xfe.\
-\xa3\x0c~Y\xe5\x9a\xfc\x0b\xfa\x03:\xea\xca\xdc\x05P\
-\xa7\xad\x1c\x05\x00*\x0d\x03\x027\x91\xe9\xaa\xc0\xf2\xa9\
-$ \x90\xf1QMg\xd0j\x06\xfdm\xab\x07\xfaY\
-\x94[\xfe\xb3\x11\xf4\x07t\xa3XG\x91\xdc\x06pT\
-S\xc5:B[\x01O5\x0c\x08\xdc\xbf*0\xc7b\
-\xa2\x80@\x14\x00zd%`\xa2\x1a\x04\xfd\xbd\x1eO\
-W\xfd\xb3N\xfe\x05\xfd\x01\x9dNk]\x060\xa7q\
-\x0b\xd0\x81\x06\x01\x81\xc5^\x11 [aQ@ c\
-\x98\xaf\x8e\xfd\x08\x80Q\xd3\x04\xd5\x0c\xfa{R=\xbc\
-\xb3\x85\xfcE\x08\xfa\x03\xe6<4\x18t[\x15Q\x14\
-w\x1a\x02x^\xc3\x80\xc0u\xf5\x14\xceR\x04x&\
- \xf0\xbd\x02\x02\x19\xa61\x17\x00\x9c\xff\x9f\xda\xb8\xae\
-~\xd0\xdfn\xd5\x7f\x19\x11\xe79_\x8b\xa0?\xa07\
-E\xba\x88\x14\xb7\x1a\xe2\x98\xb6\x8aeD\xd2V\xc0\xfd\
-\x8f\x88f\x01\x81\x9bj\x1cy\x93\xf3\xb5|\xf3\x7f\x09\
-\x08\xa4\x9c\xe2(\x00\xe4mL;\x00&\xa2f\xd0\xdf\
-m\xf5\x90^W?\x99\xc6\x95\x82\xfe\x80\x93\x0cY\xcf\
-baU\xfbh[}?\xf0\xb8\x06\x01\x81\xe7Q.\
-(]W\xe3\xcc\xf6\x13\x15\x01\x81\x0c\x94\xa5MN\xae\
-f\xd0\xdfeD\xdcU\x0f\xe9\xac\x9f_A\x7f\xc0\xc9\
-\xa4dR{\xf4\xc8%]D\x14\xd7\x1a\x02xL\xc3\
-\x80\xc0U5\xce\xcc\x95\x0b  \x10;\x00\xa6\xde\xa0\
-\x1c\xaff\xd0\xdfu<]\xf5\xdf\xe4~-\x82\xfe\x80\
-\xd3*\x16Qf\x9ap\xb0\xe7/\xce\xca+\x01\x01\x0e\
-k\x10\x10\x98\xf5\xaa\xc0\x1d\x01\x81\x0a\x00\x0a\x00\xccZ\
-\xcd\xa0\xbf]\x15v\x19\x19\x8f}\x08\xfa\x03\x064>\
-XF\xca{\xfe\xd4\x80\x0a\xa0\xd4  0\xf7U\x81\
-\x02\x02Q\x00`\xa6#\xb6zA\x7fW\xd5\xcf:2\
-&\xfc\xef\x08\xfa\x03\x06\xa5(<\x88\x8e\xb7\x89\x14\x97\
-\x9a\x018\xfe\x11[; pwU\xe0mD\xde\xe7\
-\x8d\x80\xc0yM\x7f\x14\x00\x98\xad\x9aA\x7f7\xd5\xe7\
-3\xeba|A\x7f\xc0p\x87\x08[\xab\xda\xf5\x9e\xe8\
-\xc60@m\x0d\x02\x02w\x8bP\xb9r\x01\x04\x04\xce\
-\xaf\x000\xa8\xfe}\xcc\x9d\xa7\xc0\xa4\x11\xa9\x11\xf4\xf7\
-z\xf5\x80\xddm\xbd\xcaJ\xd0\x1f0\xdc^\xadXG\
-X\xd5>\xbe\xbd\xd2\xe0\x06U\xc084\x08\x08\xdc]\
-\x15\x983\x17@@\xe0|\x0c*\xe3G\xf5\x9cN\xd5\
-\x08\xfaKQ\xae\xfa\x9fG\xe6U\xff\x1dA\x7f\xc0\x18\
-\xa6\xb5\x9a\xe0\xf81|d\x5c\x91\x03\xe6\xa7f@\xe0\
-y\x94\xbb\x01n\xa2\xbc) \x1b\x01\x81\x937\xa8s\
-\x1ec/\x00\x18(\x0dX\x8d\xa0\xbf\xcb\xe8h\xd5_\
-\xd0\x1f0*\xc9\x8av\xcd\xf6\xb2\x90\x01\xb4\xd20 \
-\xf06\xb2\x1e\x09\x10\x10\x88\x02\xc0q\xdd\xbe\x1d\x0c\xc3\
-|c\x8e\x0f\xfa\xdbFYE\xbd\x88\x0e\xae\xf6\x8b\x10\
-\xf4\x07\x8cL\x11\xebHV\xb5\x8fo\xaf\xa2\x88Hw\
-\x1a\x02h\xfb(\xa9\x19\x10\xb8\x89ra+\xfb\xed-\
-\x02\x02'\xd8\xb3\xcb\x00`\xcaj\x04\xfd]V\x0f\xcd\
-e\x94[\xaar~\xcb\x04\xfd\x01#\x1e(\xd8\x04p\
-\xbc\xb4\x8c\x14\x0a\x00@\x165\x03\x02WQ.be\
-\xbb*0B@\xe0\x04-\xbc\xa0\x8c\xbd\xbe\xcf\xd3\xb0\
-\x1c\x19\xf4w\x1be\x80\xca2::\xeb/\xe8\x0f\x18\
-w\x09\xa0\xd0\xbf\xd5j/M\x00\xe4S3 pw\
-U\xe0Mt\x18\x10\xf8\xcb\x02\x02\xc7\xecL\x01 \xef\
-\x17C\xb7?\x00\xcf\x04\xfd]?\xfa\xec\xbb\x8a2\x05\
-s\xd5\xd5\x97A\xd0\x1f0\xfe\x09mZF\xca\xbf\xad\
-t\xba\x16\xcb\x10\x06\x08dV3 p\x1d\xe5.\x80\
-\xec7\xb9\xdc\xde\xdd\xa5\xbf* p\xd4\xbd\xfa\xd0\xe6\
-\xac\xae\x01\xa4\x957\x05\xfd\xdd\xbf\xe5\x7fW\x15\xedd\
-\xd5_\xd0\x1f0)\xa98\x8bH\x0e~\x1e\xdf`\x8e\
-3\x02\x9d\xa8\x19\x10\xd8\xc5U\x81\x91R\x12\x108\x8d\
-\x22\x80\x02@\xa6\xd7\xae\x08p\xaa\xe1\xd6\xf1A\x7fW\
-QVLW]}\xde\x04\xfd\x01\xe8\x964\x01\xd0\xc9\
-\xcc\xad^@\xe0E5\xe6\xbd\x8e\xc8\x9fO\x22 \x10\
-\x05\x00\x05\x80\x9382\xe8\xef\xba\xfaYW\x0f\xc2\xbc\
-\x0fcA\x7f\xc0\xa4G\x9c\x8bE\x14\xe9\x89\x868\xda\
-&R\xfe\xad\xb7\x00;\x0d\x02\x02o\x22\xf3\xf1$\x01\
-\x81\xe3\xed\xd5\x15\x00\xf28S\x00\xe8\xdf\x91A\x7fW\
-{\x0f\xbfnFz\x82\xfe\x80IK\xcb\xd8\xca\x01\x98\
-\xd1\x98\x06\x18\x81\x9a\x01\x81/<7.\xce:\x99\x14\
-\x10\xa8\x000\xc7\xceR\x08`\x8f\x8e\x0c\xfa\xbb\x8a\x0e\
-W\xfdw\x04\xfd\x01\xf3\x18.\x14\xfa\xb8:R\x11\x11\
-\x85=\xb1@\xe7j\x04\x04\xae\xa3\xcc\xc0\xba\x8d\x8cW\
-\x05\xee\x08\x08dn\x05\x80\xa8\xbeH\xb6Hv\xec\x88\
-\xa0\xbfTM\xfc\x8b\xae&\xfe\x82\xfe\x809\x96\x00\xc2\
-\xd9\xf6\x1a#\x9a\xb4\x8aH\xd7\x1a\x02\xe8C\x8d\x80\xc0\
-E\x94\xd9\x00\xbb\xab\xb0\xb3\x11\x10\xc8\x1c\x0b\x00I\x01\
-\xa0\xc3\xc6=.\xe8\xef2\xca3N\xab\xe8p\xd5_\
-\xd0\x1f0C\xabH\xc9\xf5v\xf5\xd85\x01\xf4\xf7\xc0\
-\xa9\x17\x10\xb8\x8ar\xf1\xb2\x93B\xa5\x80@}\xd3\x9c\
-\x0a\x00>\xe1\x1d8\x22\xe8o\xf7\x00;\xebj\xe2/\
-\xe8\x0f0dp\x0c\xa0f\xc7q\x16\x91n5\x04\xd0\
-\xa7\x1a\x01\x81\x9bj\xfe\x95\xbd\x08  \x90\xb9\x14\x00\
-vE\x002:\x22\xe8o\x7f\xd5\x7f\xd9\xd5\xeb\x10\xf4\
-\x07\x90\xf4q\xf5F\x04\x17\x91\xec\x0c\x04\xfaW# \
-\xb0\xcb\xab\x02\x05\x042\xf9\x02\x80\x81QFG\x04\xfd\
-=\xa9&\xfe\x17Q\x86\x9atF\xd0\x1f@DD\xb1\
-\x89p\xbd]\xbd&+\x8c\x0d\x80\x93\xa9\x11\x10\xb8\xbb\
-*\xb0\x93#\x01\x02\x02\x99j\x01@\x11 \x93#\x82\
-\xfe^\x8f2\xbcd\x19\x11\xe7\xdd\x8c\xd9\x04\xfd\x01\xdc\
-\xd3\xcd9\x06Pkd\xb3XE\xc8N\x00N\xa7F\
-@\xe0\x0b\xd5\x5c&\xfb3K@ S-\x00\xa4\x10\
-\xf8\xd3\xf6\xe1p(\xe8\xef.\xca\xea\xe4::^\xf5\
-\x17\xf4\x07p\xef\xfc_\xa1\xbb\x8e\xedv\x11\xa2\x13\x80\
-\x13\xab\x11\x10\xb8\xbb*\xf0&:Z\xd8\x14\x10\x88\x02\
-\x00\x11\x11\xf1\xb5\xaf\x7f\xf3P\xd0\xdfeU\x00Xv\
-\xf5Y\x11\xf4\x07p\xb0\xab[GG[D\xa7[\x04\
-P3\x01\x86\xe1\xc8\x80\xc0E5\xde\xce~U`\x84\
-\x80\xc0\x81\xccY\x15\x008\xadW?\xfd\x99x\xfb{\
-?\xf8P\xd0\xdf\xee<R\xe7\xab\xfe\x82\xfe\x00\x0e(\
-\x8a\x22\x92\xe3n5\xdbl\x1d\xb2\x13\x80\x81\xd8\x0f\x08\
-|\xcb\xe3\x01\x81\xcb(o\xda\xea\xe2\x18\x93\x80@&\
-Q\x00H!\x03\xa0\x96#\x82\xfe\xae\xaa\x07\xcf*:\
-\xde]!\xe8\x0f\x80\xee\x8a\x00v\x08\x02\xc3\xf2]\xef\
-{9\xbez8 pwU\xe0MW\xafC@\xe0\
-I\xe6\xac\x0a\x00\xf4\xef@\xd0\xdfU\xf5\xd3\xe9\xaa\xbf\
-\xa0?\x80FO\xcf\xb3H\xc9\xf5v\xf5\x87\x5c\x0e\xbb\
-\x02\x83rd@\xe02\x9e\xe6\x02d\x7f\xf6\x0b\x08\x9c\
-7\x05\x809\x8c\x7f\x0e\x07\xfd\xddD\xb9\xda\xdf\xf9\x1e\
-|A\x7f\x00M\xe6\xff\xe9\x22\x8a\xe2FC\xd4\x9a\xfc\
-\xaf\xa3\x90\x9d\x00\x0c\xf0\x91~|@\xe0.\x17\xa0\xb3\
-\x9bM\x04\x04\xf6\xd4#)\x00\xd0\x97\x03A\x7f\xbbU\
-\xffe\x94[\xfe\xbby\xc8\x09\xfa\x03\xc81|\xd0g\
-\xd7o3\xc7\x00\x80\xc1:2 p\xbd7n\xcf\xff\
-\x98\x14\x10\xa8\x00\xc0t<\x12\xf4\x97\xa2\x5c\xf5_D\
-\x0f\xab\xfe\x82\xfe\x002(\x22\xa2\xb0\xa5\xbd\xe6(\xe7\
-<R\xd89\x01\x0c\xd6\x91\x01\x81\xfbW\x05v\xd5\xc3\
-\x08\x08T\x00`\xac\x0e\x04\xfd]V\x0f\x8f\xdd\xd9\xa2\
-N\x09\xfa\x03\xc8f\x15)\xd9\xd2^o\xc8u\x1e\xa1\
-h\x02\x0c\xdf\x11\x01\x81\xbb\xab\x02\xafC@\xa0\x22\xc0\
-\x8c\x0b\x00\xb6\xf6=\xe7\x91\xa0\xbfm\xf5\xc0\xb8\x88\x0e\
-\xb7\xfbG\x08\xfa\x03\xe8\xee\x01\xbb\xd0\xef\x8dx\xd0\x05\
-\xf0\x98#\x03\x02WQ\x06\x03vv$ B@`\
-\x07\x06S\x8c\x9e\xc2\x0e\x00\x83\xa18\x18\xf4w\x19e\
-\x80\xc8*\x22\xce\xbb~-\x82\xfe\x00\xba\x1a>$\x93\
-\xd9\xfa\xa3\x84uD\xba\xd4\x10\xc0(\x1eY\xc7\x05\x04\
-\xee\xae\x0a\xectW\x98\x80\xc0\xac\xf3U\x05\x00\xf2y\
-$\xe8\xef6\xfaZ\xf5\x17\xf4\x07\xd0\xc7\x10b\x13e\
-Q\x97:\xadV\x14\x16\x0b\x80Q9\x22 \xb0\xd3\xab\
-\x02#\x04\x04f\x9es;\x02\x90\xebs\x193\xdf\x01\
-\xf0H\xd0\xdfU\xf50\xe8e\xd5_\xd0\x1f@\x8f\x13\
-Z\xea\xd9\xda8\x01\x8c\xcf\x11\x01\x81Et\x7fU\xa0\
-\x80\xc0\x89\xcd\xb9\xed\x00\x18\xa9G\x82\xfev\xab\xfe\xcb\
-\xe8!\xe1?B\xd0\x1f@\xcf\xccfk\x0f_\x8bu\
-$;'\x80q:\x22 \xb0\xd3\xab\x02\xdf\x98d\x08\
-\x08l3\xe7\xb6\x03 \xe3 hv+!\x8f\x04\xfd\
-]Ey\xbed\xd5\xf5{+\xe8\x0f\xe0dV]\x0f\
-\xf2\xa69\xfcr\x0c\x00\x18\xaf#\x02\x02wW\x05v\
-\x96\x0b  \xb0\xdd\xf4I\x01 _C\xce\xa6C\x7f\
-$\xe8ow\x1d\xc8::>\xeb\xbf#\xe8\x0f\xe0\x84\
-}\xb7=\x00\xf5m\xa3\x88\x22=\xd1\x10\xc0h'>\
-\x87\x03\x02\x17\xd5\x5c\xe0:\xca]\xc1\x9d\x11\x10\xa8\x00\
-\xa0\x00\xd0\xb1G\x82\xfev\xab@\xcb\x1e\x1a[\xd0\x1f\
-\xc00z?%\x80\xdam\x96V\x91\x8a\x1b\x0d\x01\x8c\
-\xdd\x11\x01\x81\xab\xe86\x17@@\xe0\x88-&\xf0\xfa\
-'_\x00x \xe8\xef*\xca\xea^o\xab\xfe\x82\xfe\
-\x00\x862\x99-.\xa2\xe8vug\x92\xaa\xed\xab\x00\
-cwD@\xe0\x0b\xd1\xfdU\x81\x02\x02k\xb6\x95\x02\
-@\x9e\xd7?\xd9\xfd\xe7\x0f\x04\xfd\xa5\xea\x8b\xbc\xe8k\
-\xe2\x1f!\xe8\x0f``\x13\xd9\xf3\x88\xb8\xd3\x10\xb5G\
-\x0d\x17\x1d\x0f\x86\x01zu  p\xff\xaa\xc0N\xf7\
-\xe9\x0b\x08T\x00\xe8\xcbY\xd5\x98\x93;x\xf2@\xd0\
-\xdfe\xf5\x05^E\x1f[\xfe\x05\xfd\x01\x0c\xb8\x08\xe0\
-:\xc0\xfamV\x9c\x85[\x14\x80\x899\x10\x10\xd8\xc7\
-U\x81\x02\x02Gd\x0a\x19\x00iJ\x05\x80\x07\x82\xfe\
-\xb6Q\xaeX\x9cE\x8f\xab\xfe\x82\xfe\x00\x06l\x1b\x8b\
-H\x85\xe4\xa5\x06]\xad\x12\x0005G\x04\x04\xae\xaa\
-yS\xe7\xb7\xc8\x08\x08|p\xde\xaa\x00\x90m\x084\
-\x91\x02\xc0\x03A\x7f\xfd\xae\xfa\x0b\xfa\x03\x18\x87E,\
-\xa3H\xb6\xb3\xd7\xb7\x89\x22.5\x030E\x07\x02\x02\
-7\x11q\x1e\x1d\x1f\x85\xda\x0f\x08|\xe9\x03\x1f\x11\x10\
-8\xb8\xe1\xc34\x0a\x00\xa3\xaf\xe5\xdf\x13\xf4\xb7\xad&\
-\xfe\x17Q\x06\xfd\xf53*\x12\xf4\x070\x1e\x85\xbb\xed\
-\x1b\x0eOmk\x03&\xeb@@\xe0y\xf4sU`\
-\x11\x11\xf1\x85/\xbdV\xbc\xf3\xa5\xef\x8b\x7f\xf9\xea\x7f\
-\xf0\xc6(\x00\xe4\xeb\xc5\xc7\xfc\xe2\x1f\x08\xfa\xdb\xad\xfa\
-/\xab/i/\x04\xfd\x01\x8c\xad\x07L6\xb37\x1d\
-;\xb8J\x11\x98\xb8]@\xe0\xfb\xfe\xfc\xbd\x01\x81\xab\
-(\xc3d;\xdf\x11u{w\x97~\xf0G\x7fB@\
-\xa0\x02\x80\x02\xc0=A\x7fO\xe2\xe9v\xffM\x1f\xaf\
-A\xd0\x1f\xc0\xa8m\xfa\x18\xbcMO\xb1\x8e\xd4\xfd9\
-X\x80S\xfb\x96?\xfaG\xe23\xaf>\x18\x10\xb8\x89\
-r\xa5\xbe\xf3#\x01\x11\x02\x02\x15\x00f\x5c\x00x \
-\xe8\xef2\xca*\xdc\xb2\xcf\xf7E\xd0\x1f\xc0\xf8g\xb3\
-\x9a`\xb6c \x80\xc3\x9d\xc4\xe3\x01\x81\xeb\xe8\xe9\xaa\
-\xc0\x08\x01\x81:\xbf\x19\x0e~\xee\x09\xfa\xbb\x8d\xb2\xea\
-\xb6\x8e\x9e\xce\xfa\x0b\xfa\x03\x98\x90$\xd5\xbea\xc3-\
-\xa2Hw\xda\x01\x98\x8bG\x02\x02\x8b\xbd\x22\x80\x80@\
-\x05\x00r\xb9'\xe8\xef&\xca/\xde*z,b\x08\
-\xfa\x03\x98\x90\x22\xd6\x11\xb6\xb37h\xb8\x8b\x88\xc5\xad\
-v\x00\xe6\xe4@@\xe0:\xfa\xb9*p\x8e\x01\x81\x83\
-)\xd5+\x00\xf4\xe0\x9e\xa0\xbf\xeb\xeagU\xfd\xf4F\
-\xd0\x1f\xc0\x04K\x00\x0e\x01\x8c}<\x06\xd0\xabG\x02\
-\x02\xd7\x11q\x16\x1d\xef\x04\xd8\x11\x10\xa8\x000\xb9\x1e\
-\xfc\x9e\xa0\xbf\xddjCo\x13\x7fA\x7f\x00\xe6\xb1\xdc\
-k\x19\xa9\x9fA.\xc0\xd0<\x12\x10xQ\xcdUn\
-\xa2\xcc(\xeb\xae\xfb\x9aO@\xa0\x1d\x00S\x1f\xf6<\
-\x17\xf4WDy\xcf\xe6U\x94\xe7kz]\xf5\x17\xf4\
-\x070y\x17\x91\xc2v\xf6\xfa#\x883\xd7\x01\x02s\
-v  p\xb97\x87\xe9\xdc~@\xe0v+ P\
-\x01`D\x1e\x08\xfaK\xd1S\xc8_\x84\xa0?\x80y\
-\x8d\xe0\xe2,\x22\x9eh\x88FE\x00\x05\x00`\xf6\x1e\
-\x09\x08\xdc]\x15\xd8y\x11`? \xf0\xc5\xf7O.\
- \xd0\x0e\x80\xa9z.\xe8\xef.\xca\xad3\x17QV\
-\xd0z#\xe8\x0f`~3Y\x1a(b\x13).5\
-\x040w\x8f\x04\x04\xae\xaa\xf9L\x1fW\x05\xce1 \
-P\x01`\x8c\xf6\x83\xfe.\xaf\xae#\x9eM\xf8\xef\x95\
-\xa0?\x809Nd\x17\x8b\xb0\x0b\xc0x\x08\xa0\xa5\x07\
-\x02\x02\xcf\xa2\xa7\xab\x02w&\x16\x10h\x07\xc0\x94<\
-\x17\xf4\xb7\xad\xbe\x18\xcb(+e\xfd\x8c\xfb\x04\xfd\x01\
-\xcc\x5cZF\x8a\x1b\xed\xd0t`V8p\x0aPy\
-S@\xe0\xd3\x84\xc0u5\xdf\xe9\xe5H@\xc4,\x02\
-\x02\x15\x00\x9a\xcc\x7fO2Z\xd8\x0b\xfa\xfb\xfd?\xf8\
-\xc6n\xcb\xff6N\xb0\xea/\xe8\x0f\x80X\x14.\x04\
-l6\x8aXGJn\x03\x00\xd8\x7f4\xee\x07\x04\xbe\
-\xf5\x99\x80\xc0MD\x9cG\xf4w\x8b\xcaD\x02\x02\x07\
-\xb1\x0b`\x0a3\xc5\x93\x0cv\x9e\x0f\xfa\xab\xbe\x00\xe7\
-\xd5O_\xbf\xb8\xa0?\x00\x9e\xdanC\xaa}\xd3N\
-5)\x9e\x00\xdc\xe3\x81\x80\xc0\xf3(\x17=\xaf\xa3\xe3\
-\xab\x02#&\x11\x10XD\xf7\xf9\x09\xb3)\x00D\xf4\
-\x5cMy.\xe8o\x1b':\xeb/\xe8\x0f\x80g\x87\
-\x17\xc5:R?\xd75MN*\x16Q\x14\xaeR\x04\
-\xb8\xc7\x81\x80\xc0\xbb\xe8g7\xc0\x98\x03\x02\x17\x0a\x00\
-#tyu\x1d?\xfc\xb7\xff\xc1.\xe8\xaf\x88\xf2\xac\
-\xff\xe2\x14\xed(\xe8\x0f\x80\xc7\x06H\xd4n\xb5el\
-\xb7B\x14\x01\x1e\xf1@@\xe0\xba\xfa\xcf\xde\x0a\xd0#\
-\x0c\x08\x5c\x84#\x00\xd9\xa4>\x06;\xbb\xa0\xbf_\xfa\
-\xe5_\x8d\xbd7\xaf\xd7\xab\xfd\x04\xfd\x01pD\xb7\xe8\
-\x08@\x8b*\x00\x00\x8f{  p\x1dOo\x09\xe8\
-\xbc\x1f\x1aa@\xe0`:\x18!\x80\x87?\x5cU\xd0\
-\xdfGvA\x7f\xb7\xa7z\x03\x05\xfd\x01pD\x97\xb8\
-\x89p\xaf}C\xcb\x08G(\x00\x0e\xf64\xf7\x07\x04\
-.\xa2\xe7\xab\x02#F\x15\x108\x88\x22\x80\x1d\x00\x8f\
-x6\xe8\xef\x8d\x15\x95\x8b\x9e?%\x82\xfe\x00\xa8\xd9\
-3\x0a\xb4k\xd8\xe9\xaa\xae\x03\xd4\xf0@@\xe0*z\
-\xba*\xb0\xec\xf2F\x13\x10\xe8\x08@\xbe9r\xfe\x02\
-\xc0\xab\x9f\xfeL\xbc\xed=\xdf\xbb\x0b\xfa{\x12'\xaa\
-\xd8\xac7\xab\xf8\xb5O\x0a\xfa\x03\xa0N\xcfX8\x06\
-0\xf2\x01\x1a\xc0X<\x10\x10\xb8\xa9\xe6\x9a7=\xce\
-\x09\x87\x1e\x10h\x07\xc0\x10\x0b\x00\xfbA\x7fW\xd7o\
-|^\xcfN\xf1\x8b\xbd\xfc\x1d\xefN_\xfd\xec\xaf\x16\
-\x1f|\xbf\xa0?\x00\xea\xf4\x8ci\x19\xa9\xb7A\xd7\xd4\
-l\x22\x92#\x14\x005\xdd\x13\x10x\x11\xe5\x91\x80\xeb\
-(\x17T{1\xe0\x80@\x05\x80\x8c\xbfC\x96\xdf\xe3\
-\xf3_\xfcr|\xdb\x9f\xfb\x9e]\xd0\xdf\xf6\x14o\x92\
-\xa0?\x00ZK\xc5YD\xdaj\x88\xa6\xed'h\x07\
-\xa0\x89\x07\x02\x02WQ\xe6\xa8\xf5\x92\x0b0\xc2\x80@\
-\x05\x80\x9a\xce2|H\xe2\x1f\x7f\xe2\x9f\xc7\x8b\xef\xff\
-H\xfc\xcfo\xfe\xef\xe2\x94m#\xe8\x0f\x00Nm\x1b\
-Q\x14\x0a(\x00\x0d<\x10\x10\xb8;\xcb\xdck\xd0\xea\
-. \xb0\xcct;\xf9c\xdd\x0e\x80!\xfc\x0e\xbb\xa0\
-\xbf\xbf\xf7S\x9f\x88\x94NsuRQ\x94\xe7\x0d\xff\
-\xda\x0f\x08\xfa\x03 [\xe7r\x16\x8b\xb8\xd3\x10\x8d\xda\
-n\x15\xdb\xed\xb5\x86\x00h\xee\x9e\x80\xc0e<\xbd%\
-\xa0\x17\xbb\x80\xc0\x8f\xff\xfc\xa7\xe2\xc5\xbf4\xe8\x80@\
-\x05\x80:\xddt\x94\xdb\xf5k{\xb5\xda\x16R\x05\xfd\
-\xdd\xc5\xa9\x82\xfe\xd6e\xd0\xdf'\x7fN\xd0\x1f\x00\xd9\
-\x5c\xc46n5C\xe3\x22\x80\x9b\x14\x00\xda\xces\xde\
-\x1c\x10\xb8\xbb*\xf0:\xfa\xbb*\xb0\x88\x88\xed\x17\xfe\
-\xebk\xc5;_\x1el@\xa0\x02@M\xb5V\xee/\
-\xaf\xae\xe3o\xfc\x9d\x9f\x8a\xef\xff\xe8\xc7\xe2\xfa\xfa\x8d\
-\xcf\xddI\x06I\x82\xfe\x00\xe8x\xd0C\xb3\x96;;\
-\xd5\xd8\x00`j\xee\x09\x08\x5cF\x8fW\x05F\xb9\xeb\
-\xe0\xfa\xf6v\xb0\x01\x81\x0a\x00]\x15\x00>\xff\xc5/\
-\xc7;^\xfc\xcb\xe9\x17\xff\xc5\xbf+\xff\xc1$\xe8\x0f\
-\x80I\x17\x00\x5ck\xd7ldq\x11)=\xd1\x10\x00\
-y\xdc\x13\x10\xb8\x89\x88\xf3\xe8g'@\x8a\x88$ \
-pF\x05\x80\x94R|\xfc\xe7?\x15/}\xe0\x87\xe2\
-k_\xff\xc6I_\xac\xa0?\x00z\xb2\x8a\x94\xae4\
-CC\x85\xe2\x09@\xd6\xc7\xea\x9b\x03\x02\xcf\xa3\xbc%\
-\xe0&\xba\xbf*p\x19{;\x0ev\x01\x81?\xfe\xd3\
-\xaf\x0c! P\x01\xa0\xa6G\xdf\xb1\xaf}\xfd\x9b\xf1\
-\x9d\x1f\xfc\x91T\xa5?\xa6\x93\xac\xfaWE\x8a\x0f\x7f\
-H\xd0\x1f\x00=\x8f\xb6h\xdav\xabH\xa1\x80\x02\x90\
-\xd9=\x01\x81\x17U\x01\xa0\xcbg\xee3\xd7\xc7\xef\x02\
-\x02\x7f\xe6g\xffY\xbc\xf8\xfe\xf9\x04\x04N~\xf9\xf9\
-\xd5O\x7f&\xde\xfe\xde\x0f\xa6\xdf\xfa\x9d/\x16O\xe7\
-\xe2\xfd[o\xca\xa0\xbfO\xbd\x22\xe8\x0f\x80>%\xab\
-\xd8\x8d\x9b.\x16R\x14\x00:\x9a\x1f\xbd9 p\x19\
-e!\xa0\xcb#\x01\xdbxv\xf1\xb8\x88\x88\xf8\xc2\x97\
-^+\xde\xf9\xf2\xf7\xa59\x04\x04N\xb6\x00\xf04\xe8\
-\xef\xc7\xe2\xea\xfa\xb47\xf9\x08\xfa\x03\xe0t\x8aMD\
-\x5cj\x87\xc6\xed\xa7\x80\x02\xd0\xa1\xe7\x02\x02\xcf\xa2\xdb\
-\xab\x02\xd7\xf1@\x81\xe1\xf6\xf6.~\xf0G\x7f\x22>\
-\xf4\xc3\xd3\x0e\x08\x9cJ\x01\xe0\x99\xfa\xbc\xa0?\x00\xe7\
-B\x01a\x00\x00\x0a\xa9IDAT\xd8\x97\xacc7\
-o\xbbM\xa4\xa4\x80\x02\xd0\xa1\xe7\x03\x02\xab\x22\xc0]\
-G\x85\x80{\xfb\xc47\x02\x02\x7f}\xda\x01\x81\x93\xda\
-\x01 \xe8\x0f\x00\xee\x9d\xff[\xc5n7V\xd4\x91\x03\
-t\xfd\xa4\xdd\x0b\x08|\xfb\xb7\xbd\x11\x10x\x1e\xf9s\
-\x01\x0e\x1e3\xd8\x05\x04\xfe\xfd\x9f~%R\xde\x93t\
-'/\xc8\x9f\xfa\x05|.\x22\xde\x13\xed\x0b\x117\x11\
-\xb1\xfc\xd3\x7f\xeam\xf1\xdaW~/\xa2\x0c\xdc\xab\xfb\
-\xbb]F\xc4\xa6ec\xa6\x14Q|\xf8C\xdf\x1d\xbf\
-\xf0\xf1\x1fw\xd6\x1f\xa0;\xad\x9f\xd9\xf3*\x00\xa4\x14\
-Eq\x13e\xd22\xb5\xdb/\xae\xa3\x88\xf3(\xb7\xa6\
-\xfa\x0c\x02t\xec\xea\xfa&>\xf6\x93?\x1b\x9f\xf8\xc5\
-_\xd9\xfdO\xb7\xd5\xc4=\xd7\xb8\xe1*\xca\xe3\x00\x8f\
-?\xfd#\x8aw\xbe\xedO\xa4\xaf\xfe\xde\xff\xc81o\
-\xbe\xab\xfa\x91\xdf\x8d\x88\x97\x14\x00\xda\xb9\xce0\xa8i\
-\xdd\x91o6\xab\xf4+\xbf\xf03\xce\xfa\x03(\x00\x0c\
-q\x12{\x15E\xa8L\xe7\xfb\xcc\xf9\x0c\x02t\xec?\
-\xfe\xe7\xcf\xc6\xf7\x7f\xf4c\xe9\xff\xfc\xdf\xffW\xc4\xd3\
-\xf0\xbe&s\xc7!<\xc3o\xa3\xdc\xd1p\xd2\x02\xc0\
-\x94\xae\x01|>\xd1\xb1W\x82\xfe\x00`\xca\xe4(\x00\
-\xf4\xed\xb9\x80\xc0E\x94\x0b\xd89\x12\xde\xeb\x06\xe4\xa6\
-(\xaf)\x1c\xbd)\x9di\xbb\x89\xb2\xaa\xd2\x1bA\x7f\
-\x00\x8cF\x11g\x91\xd2\x13\x0d\xd1\xd8y\xa4\xceR\xa9\
-\x01x\xc0=\x01\x81\xabL\xf3\xbe:s\xe1\xeb\x0c\x05\
-\x80A\xe4\xf1L\xa9\x00\xb0k\xd0\xbb\xbe\xfe\x85\x82\xfe\
-\x00\x18\x91\x8b*\x07\x80F\x8a\xf3(N\xb7\xd3\x10`\
-\xd6O\xe0\xbd\x80\xc0\xb7\xbd\xf5[S\x94y\x00m'\
-\xd4E\x8dB\xc2.cn\xf4\xb7\xc2Lm\xd6\xba\x8a\
-\x8e\x8f\x01\x14\xd5\x07\xed\xc3\x1f\xfa\xee\xf8\xef\xbf\xfdj\
-\xf1g\xff\xcc\xbb|#\x01\x18\xcd\x18J\x13\xb4j=\
-\xb7)\x00\x9c\xd0\xb7\xbf\xeb\x1d\xf1\xe5\xdf\xfc7\xc5\xdf\
-\xfa\x91\xbf\xb2\xdf\xa75]\x00^F\xbdU\xfd\x8b\x96\
-\xf3\xe7b\x08\xfd\xf0\x14\x97\xadSDw[\xf4\xd6\x9b\
-U\xfc\xda'\xffI|\xea\x95\x9f\x94\xf2\x0f\xc0\xf8\xa6\
-\xffEa\x15\xbb\xf9\x08c\x1d\x13X\xfd\x01\x18\xb3\xf5\
-j\x19\xff\xf4\x1f\xfeX\xfc\xc6\xbf~%\xfe\xf0[\xfe\
-\xd0\xee\xba\xc0\xa6\xdb\xf3\xeb\x16vW\xd1\xfcZ\xc2A\
-\x14\xe1\xa7R\x00(\x9e{S:!\xe8\x0f\x80\xd1O\
-`S\xba\xd6\x10-\xc6\x1b\x850@\x80!x. \
-\xf0,\x9a\x1d\x09hZ\xd8m\xb2\xe0|\xa6\x00\xd0\xad\
-\xab\x1c\x7f\x88\xa0?\x00\xa65\x85-L`\xdb\xd8\x16\
-\x11\xe1(\x00\xc0\x10\xec\x02\x02\x7f\xee\x1f\xfd\xdd8;\
-[\xec\xfa\xb7:\xcf\xe8\xa2\xc1\x9cx\xdd\xb0\x1f\xb0\x03\
-\xa0C\xcb\x5c\x0d,\xe8\x0f\x80iM`\x93\xc9k\x1b\
-E\xac#\xd3\x22\x03\x00\x19\x1e\xcbE\x11\x7f\xf3\xaf\xff\
-@|\xe9?\xfd\xab\xf8\x93o\xfd\xe3\xbb\xb0\xbe\xbaG\
-\x02\xea\x1e\x8f\xbb\x18k_0\x95\x19m\xba\xe7w9\
-\x8f\x86\xe7\xf4\x04\xfd\x010\xe1\x09\xec&\x8ap\x1d`\
-\xdb\xf1Sr\x14\x00`H\xbe\xfd]\xef\x88\xd7~\xf3\
-\xdf\xee\x02\x02\xeb\x1c\x09XE\xfd-\xfd\x8b\x86\x85\x03\
-\x05\x80\xacC\x9ag\x9d5\xfd\xfd\x04\xfd\x010i\xc9\
-m\x00\xad\xdb\xaf(.4\x04\xc0\xb0\xec\x07\x04\xf60\
-\x8f[G\x8fW\xd0w5i\xee\xdb\xe7\x22\xe2=\xd1\
-\xbe\x10\xf1z\x94\xdb0\x9e\xef\x8c\xb7\x11q\x1d\x11\x9b\
-\xa3\xba\xf3\x88\xe2[\xff\xd8\xb7\xc4\xf7\xfc\xc5\xef4\xf1\
-\x07\x18\xb0\xedv\xfbd\xb1X\x9ci\x89\x86\xf3\xd7\x94\
-\xb6EQ8\xd7\xd6\xb2\x0a\xe0VE\x80\xe1z\xfd\xf2\
-*\xfe\xfdo\xfc\x97\xf8\xfd?\xf8\xc61\x0f\xed'\xd5\
-d\xfe\xa1@\xf9\xcb\x07\xe6\x947\xd5\x9c\xb3\xce\xe4\xf1\
-w\x22\xe2%\x05\x80v.\xab\xc9\xff\xf9=\xff\xdfU\
-\xcd7\x04\x00\x00\x80\x89(\x8a\x22\xa5\xc3G\xb7\xae\x1b\
-\x14\x00\x0e\xfds\x83+\x00\x9cO\xe5=\x8d\x87\x8b\x19\
-\xeb#\x8b\x00\x8f\xbd\xa9\xa7\xf6\xa4\xfa)\xf6\xfezw\
-\xa6%\xed\xb5A\xba\xa7-\x8a{\xfe\x9em<{n\
-\xe5\xbe\xff\xbe\xcbU(\xe2\xd9\xb3-i\xef\xdf\xf3\xfc\
-\x9f\xbb\xd8\xfb\xe7\xcfb W]\x00\x00\x00\xf3\x95R\
-\xba:b\xae\xd74$w\x15#Zt\x9eJ\x01\xe0\
-\x98\x1d\x04c\xde\xab\xf7\xfcdz\x8c\xe7\x0e\xf7\x8b\x18\
-u\x0a\x18\xf7\xbd\x7f\x8f\x15-\x8a\xbd?+U\xedv\
-L\x01c\xf7\xff\xed\x171.\xc2\xfeN\x00\x00\x98\x83\
-u\xb4[\x14\xbe\x89\xf26:\x05\x80\x9e&\xc8\x87\xde\
-LG\x01N\xff\x1e\x9d\xedM\xac\xc7\xe6\x98\x02\xc6\xee\
-\xaf\xef+b\xdcW\xc08\xb4#cW\x90H\xcf\xfd\
-9q\xcf_\xdb\x85\x01\x00\x00\xed4=\x9a\xbe\x8e\xf2\
-(\xc0\xe0Mi\x07\xc01W0lcZ7\x1f\xd0\
-\x9f)\x150v\x7f\xdd\xc71\x92\xe2\x9e\xef\xe7\xb1\xc7\
-H\x22FPE\x05\x00`R\x05\x80\xdb\x86\xe3\xfd\xb3\
-\x18\xc1\xa2\xf3\x942\x00\x0e\xd9UeV>\xd7\xcc\x90\
-c$\x87\x8f\x91\xec\x1f\x1dY\x84c$\x00\x00ss\
-QM\xe2\x9b\x8c\x95\xcf\xa3\xbcI`\xd0G\xcf\xcfg\
-\xf8\xa6\xde\xcd\xf4\xf7\x86\xb1\x9b\xea1\x92\xe7u}\x8c\
-d\xf7\xbf\x0b\xf3\x04\x00\xb8\x7f,\xd6\xd4\xe0\x17\x9d\xa7\
-4\x11>\xa6\xca\xb2\x8a2\x9c\x01\xa0os>F\xb2\
-\x7f\x0c\xc41\x12\x00`\xc86\xd1\xfe\x86\xb8\xc1\x1e\x05\
-\x98\xe3Jx\x8a\x91$4\x02\x0c\x88c$\x8e\x91\x00\
-\xc0\x5c\xb4\xc9\x8d[\xc5\x80\x03\x01\xe7X\x00\xb0\x0b\x00\
-`\x9e\x1c#q\x8c\x04\x00\xea\xf4\xbbM\xfb\xb0e\x0c\
-t\x17\xc0\x5c\xcf\xc2\x17\xe1Z@\x00\xc6\xc51\x92g\
-\xff\x1e\xc7H\x00\xe8\xca\xaa\x9a/6-\x00\xec\xfa\xb0\
-\xc1\xe5\xcf\xcd\xb5\x00p\x11\xc7]\x1b\x08\x00\xe4\xe1\x18\
-\x89c$\x00s\xb2\x0b\x04T\x00\x18\xd0\xef\xde6\xdc\
-\x01\x00\x98\x0f\xc7H\x1c#\x01\xe6#\xc76\xfe\xc5=\
-s\xce\x93\x16e\xe7\x5c\x008\x8bv\xe1\x0e\x00\x00c\
-\x1b\xfb8F\xe2\x18\x09p\xfc\xe4\xbd\xedd\xfd\xa2z\
-V\xed?;N:\x07?\x9f\xf9\x9bz\x11v\x01\x00\
-\x00\x8c\x81c$\x8e\x91@\xdf\xb6\xf1\xf0n\xa9c\xed\
-\x8e\x02\xac\x860\x07\x9fR\x01\xa0\xc9\x1b\x93\xa3\xaa\x03\
-\x00\x00\xc7p\x8c\xc41\x12\xc6e\x13\xe5\x82q\x8e\xb9\
-\xeau\x94;\x82\x14\x00Nl\x9d\xe9M\x05\x00\x80)\
-s\x8c\xe4\xd9\xbf\xc71\x92y\xb8\xaf\x00\xd5d\xcey\
-\xbd\xf7=\x9au\x01\xa0\x18\xc8\x9b*\x0f\x00\x00\x00\xa6\
-k*\xc7Hv\x85\x84\xfd\xed\xe9C>Fr>\x80\
-9_\x9b\x7f\x7f\xae\xb9\xe2\xee8\xcd\xac\x0b\x00\xff-\
-\x22^\xcc\xf8\x85nj\xe5y\x08\x00\x00\x0c\x9c#\x0d\
-\xcd\xb4I\xf2\xcfU(\xda\x15\x11\xbe>\xe7\x02\xc0G\
-#\xe2K-\xdf\x10\x00\x00\x00\x18\xbamD|Z3\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x1c\xf0\xff\x01\
-\xf5tm\xa3\x8e]\x9cb\x00\x00\x00\x00IEND\
-\xaeB`\x82\
-"
-
-qt_resource_name = b"\
-\x00\x04\
-\x00\x06\xfa^\
-\x00i\
-\x00c\x00o\x00n\
-\x00\x11\
-\x04+@\xc7\
-\x00e\
-\x00n\x00v\x00e\x00l\x00o\x00p\x00e\x00_\x001\x000\x002\x004\x00.\x00p\x00n\x00g\
-\
-"
-
-qt_resource_struct = b"\
-\x00\x00\x00\x00\x00\x02\x00\x00\x00\x01\x00\x00\x00\x01\
-\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x02\x00\x00\x00\x01\x00\x00\x00\x02\
-\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x0e\x00\x00\x00\x00\x00\x01\x00\x00\x00\x00\
-\x00\x00\x01\x81Z\x1e\x12E\
-"
-
-def qInitResources():
-    QtCore.qRegisterResourceData(0x03, qt_resource_struct, qt_resource_name, qt_resource_data)
-
-def qCleanupResources():
-    QtCore.qUnregisterResourceData(0x03, qt_resource_struct, qt_resource_name, qt_resource_data)
-
-qInitResources()
+# Resource object code (Python 3)
+# Created by: object code
+# Created by: The Resource Compiler for Qt version 6.3.0
+# WARNING! All changes made in this file will be lost!
+
+from PySide6 import QtCore
+
+qt_resource_data = b"\
+\x00\x00l\xf5\
+\x89\
+PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
+\x00\x04\x00\x00\x00\x04\x00\x08\x06\x00\x00\x00\x7f\x1d+\x83\
+\x00\x00\x01\x84iCCPICC prof\
+ile\x00\x00(\x91}\x91=H\xc3P\x14\x85O\
+S\xb5\x22\x15\x07\x8b\x888d\xa8N\x16\xa4\x8a8J\
+\x15\x8b`\xa1\xb4\x15Zu0y\xe9\x1f4iHR\
+\x5c\x1c\x05\xd7\x82\x83?\x8bU\x07\x17g]\x1d\x5c\x05\
+A\xf0\x07\xc4\xd1\xc9I\xd1EJ\xbc/)\xb4\x88\xf1\
+\xc1\xe5}\x9c\xf7\xce\xe1\xbe\xfb\x00\xa1Qa\xaa\xd95\
+\x09\xa8\x9ae\xa4\xe211\x9b[\x15\x03\xaf\xe8A\x10\
+CTQ\x89\x99z\x22\xbd\x98\x81\xe7\xfa\xba\x87\x8f\xef\
+w\x11\x9e\xe5}\xef\xcf\xd5\xaf\xe4M\x06\xf8D\xe29\
+\xa6\x1b\x16\xf1\x06\xf1\xcc\xa6\xa5s\xde'\x0e\xb1\x92\xa4\
+\x10\x9f\x13O\x18\xd4 \xf1#\xd7e\x97\xdf8\x17\x1d\
+\x16xf\xc8\xc8\xa4\xe6\x89C\xc4b\xb1\x83\xe5\x0ef\
+%C%\x9e&\x0e+\xaaF\xf9B\xd6e\x85\xf3\x16\
+g\xb5Rc\xad>\xf9\x0b\x83ym%\xcdu\xaaQ\
+\xc4\xb1\x84\x04\x92\x10!\xa3\x862*\xb0\x10\xa1]#\
+\xc5D\x8a\xcec\x1e\xfe\x11\xc7\x9f$\x97L\xae2\x18\
+9\x16P\x85\x0a\xc9\xf1\x83\xff\xc1\xef\xd9\x9a\x85\xa9\xa8\
+\x9b\x14\x8c\x01\xdd/\xb6\xfd1\x06\x04v\x81f\xdd\xb6\
+\xbf\x8fm\xbby\x02\xf8\x9f\x81+\xad\xed\xaf6\x80\xd9\
+O\xd2\xebm-|\x04\x0cl\x03\x17\xd7mM\xde\x03\
+.w\x80\xe1']2$G\xf2S\x09\x85\x02\xf0~\
+F\xdf\x94\x03\x06o\x81\xbe5wn\xads\x9c>\x00\
+\x19\x9a\xd5\xf2\x0dpp\x08\x8c\x17){\xdd\xe3\xdd\xbd\
+\x9ds\xfb\xf7Nk~?\x8d\xf4r\xb2n\xdbA\xed\
+\x00\x00\x00\x06bKGD\x00\xff\x00\xff\x00\xff\xa0\xbd\
+\xa7\x93\x00\x00\x00\x09pHYs\x00\x00.#\x00\x00\
+.#\x01x\xa5?v\x00\x00\x00\x07tIME\x07\
+\xe6\x06\x0c\x164\x09\x13\x02\x8c\xb6\x00\x00\x00\x19tE\
+XtComment\x00Create\
+d with GIMPW\x81\x0e\x17\x00\
+\x00 \x00IDATx\xda\xec\xdd{\x945{Y\
+\x1f\xf8\xa7v\xf7\xbe\xf59\x07\x12\x0dF\xcd\x1aoY\
+\x12MFg&\xa0\x06f\x82\xb8&j0\x01G\xc5\
+\xe88\x07\xc5\x83\x198G\x89G\x04\x81\x80\x06\x14\x13\
+\x1c\xd0(\x11\x97\xc9\x8c\x97\x19p\xbc\x1eB\x1c\x5c.\
+\xb9\xa9\xb3\xe2(\x8e\xb7\xc5A.\x19\xc6dn\xca-\
+\x84s\x80\xee\xde\xbb\xbbw\xcd\x1fU\xf5\xee\xdd\xfd\xf6\
+e_\xaajW\xed\xfa|\xd6\xeau\xb8\xbc\xe7}\xf7\
+[\xbd{W=\xdf\xfa\xd5\xf7\x17\x01\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\xd0\x04\xc9\x96\xff\xfc\
+\xcf\x8d\x88'GD\xcf\xb7\x02\x00\x00\x80\x0d=*\x22\
+>\xd8\xd0\xd7v\x1c\x11?\xbc\xcd\x17\xb0\xbf\xe5\x03\xf0\
+S\x11\xf1E\xde\xa3\x00\x00\x00\xec\xb84\x22>?\x22\
+\xee\xe9j\x00\xf0I\xf9?\xcf\x22bo\xc3\xdf\xeb$\
+\xff}F%\xbe\xbe\xa3\x88\x187\xe8\x0ds\x16\x11\xb3\
+\xfc?\xcf\xf27P,\xfc3\xc9\xffs\x12\xe7Ww\
+\xf4\x16~}\xb2\xf0\xef\xf7n\xf8\xcf\xc5\xaf\xef-\xfc\
+\xb9\xc5\xff\x9e.\xfcy\x8b\x7fvo\xe1\xdf\xef\x95\xf0\
+}\x05\x00\x00Xe\x86\xeb\xe7sHY+\xde\xcb\x98\
+W\x8b9\xea?\xde\xe6\xc1\xd9v\x00p\x96\x1f\x842\
+\x0e\xe8i\x94\xffHC\xda\xb07\xf3^\xcb\x07\xea\xb3\
+\xfc+Y\xf8\xdeG\xdc\x1c`\x5c\x164,\x1b`\xf4\
+.\xf9>.\x1b`\xb4\xfdx\x03\x00@\xd7\xa4\xf9\x9c\
+;\x8d\x88\x81\xc3\xd1\xac\x00\xe04\xffg/\x22\x0e#\
+\xe2`\xc3\xdfo\x14\xcd\xbbk\xcf\xdc\xe2@\xddo\xd9\
+k_\x0c/\x8a\xff\xbel\x80\x11\x17\xfe\xf7e\xc3\x8c\
+\xcb\x02\x8c\xc5\xf0\xe2\xb2?{1\xc0\xd8\x0f\xfd\x1a\x00\
+\x00tSb6l^\x00p\xb6\xf0:N/\x0c6\
+\x9b|\xa3\xa1l\x17W\x03\xb49\xc0X\x0c/.\x0b\
+\x11\xae\x0b0\x22\xe6!\xc5Ma\xc6M\x01Fz\xe1\
+g\xf6b\x80\xd1\xf7\xf3\x0c\x00\xc0\x9a\xfa\xf9u\xefi\
+\x09s\xef\xce\x5c\x93n;\x008Y\xf8\xcf\xa3\x88\x98\
+D\xc4p\xc3\xdf\xd3*\x00\xb8]\x9bW_D,\xf7\
+\xf8H\xc4j\x01\xc6\xe2\x7f\xbe,\xccH\xf3c\xb6N\
+\xffEq\x9c\x05\x18\x00\x00\xdb3\x8a\xecQ\x00\x1a\x12\
+\x00\x5c|n?\x89lk\x842\x8a\xfc\xcaXM\x00\
+4C\x17\x02\x8c\xab\xc2\x8b\x8b\x9fg7\xf5_,\x86\
+\x13\xeb\x16x\xea\xbf\x00\x00vE?\xca\xb9\xd1,\x00\
+(iH_4\xc8\x03\x80M\x8dK\x0c\x12\x006\xd5\
+\xd5\x00c\x93\x1dH\x8a0C\x80\x01\x00l\xa2\xb8\x06\
+\xb1J\xbc\x01\x01\xc0e\xcaz\x14\xe0\xe2\x05%\x00\xeb\
+Q\xe0Y\xef\x0e$\x0a<\x01\xa0\x5c\xc3\xc8n\x10w\
+~\x95\xf8~C_WZB\x08Pf\x90\x00@;\
+)\xf0\xbc\xba\xc0\xd3\x0e$\x00tI\xd1\x07\xd0\xe9\xad\
+\x01\xf7\x1b\xfc\xcd\x99\x94\x14$\x9c6\xf8\xef\x09\x00\xd7\
+Q\xe0\xb9\x5c\x81\xe7\xc5\x00c\xd9\x02\xcf\xe2\xff\xb3\x03\
+\x09@7\xf4\xa2\xe3\x8f\x024y0\x1e\x94\xf0\xcd\xd1\
+\xfa\x08\x00\xdb\xa3\xc0s\xf5\x02\xcfMw \x19x\xdb\
+\x01\x5c;\xff\x9eF\x87o\x127\xf9/]\x9c0O\
+6\xbchHK\xf8=\x00\x80\xeeQ\xe0\xb9z\x81g\
+\x12v \x01\x9a\xadXm.\x00h\xa0ql~\x07\
+\x7f\x18V\x01\x00\x00\xdd\xd3\xf5\x00c\xf1\xd7\xd4Q\xe0\
+)\xc0\x80\xf6\x18\xc4j}q\xa9\x00\xa0\xde\xd7X\xc6\
+s\x1a\xb6\x05\x04\x00h\x0f;\x90\x9c\x7f4\xe4\xa6\xd5\
+\x18\x0a<ay\xc9\x1a3\xe2N\xec \xd0\x86\x00`\
+q/\xe8u?\x94\x06a\x15\x00\x00\x00\xf5\xb0\x03\xc9\
+\xd5;\x90\x5c\x15f\xdc\x14`(\xf0\xa4l\xabn\x0d\
+8\x8b\x1dX\xe5\xd3\x96\xe7\x1e\xca\xd8\xb2\xa1\xf3\x8d\x8f\
+\x00\x00\xb0\x04;\x90,\xb7\x03\xc9bh\xb1i\x81\xa7\
+\x00\xa3\xf9s\xe6\x99\x00\xa0^\xc9\x86\x03\xfc~\xfeM\
+\x03\x00\x00v\x97\x1dHV\xdf\x81$\xa2\xbb\x05\x9e\xbd\
+X\xeeQ\x80\xd9.\xfcp\xb4)\x00\xe8/\xfc\x00$\
+\x1b\xfc\x1eK\x87\x08\xa3a\xff\xe0xr\xe2#\x14\x00\
+\x00\xa8K\xdb\x03\x8c\xadZc\x86+\xb6\x06\xbcn\xe7\
+\xb8\x22\x0c\x11\x00\xd4\xfd\xfd\x8c\xd5\xda\x1a/\xea\xad\x12\
+\x1e$\xf9/=\x18\x0f\xe3\x8b\xfe\xd3\xcf\x8e\xff\xec\xaf\
+~V\xf4\xf7\x95\xbb\x02\x00\x004\xc1\xc9\xe9Y\xfc\xe1\
+;\xff$\xde\xf6G\xffG\x1c\x1eMn\xcdpk\xcc\
+\x99\xd7u\xc6\x09\x00\xb6l\x93F\xffa,\xb9\x0a\xe0\
+h2=\x8c\x88\x83\xfd\xbd^\xfa\xeb\xbf\xfd\x8e\xe4\xed\
+\xef\xfa\xbf\xe2\xdb\xbe\xf1I\xf1\x9c{\x9e\x1c\x8f\xb8\xf3\
+\xc0O\x1b\x00\x00\xc0\x16\x1c\x1eM\xe2\xbf\xff\xf97\xc7\
+\xcb\x7f\xfcu\xe9\xfb>\xf4\x91\xe4\x91w\x1d\xa4\x11\x91\
+\x143\xdc\x1a\xbf\xe5u[\x03\xee\xc4\x0e\x00\xd1\x80\xbf\
+\xc4\xefF\xc4\x17\x94\x14\x00\xac\xd2\x0f\xb0l\x80p\xee\
+\xcd\xf3\x88;\xc7\xe9\xc3\x1f;J>\xf1\xcf\xdd%\x08\
+\x00\x00\x00h\xc0\xe0\xff\xd0G\x0f\x93\xabf\xb8\x15M\
+\x22{\xd6\x7f|\xc9\xfc\x98\xc6\xe6\x85\xf2\xb3\x88\xf8\xfd\
+\x88\xf8B\x01\xc0\xe6!\xc0\xaa\x05\x81\xcb\xfc\xfaK\xdf\
+<\x0bA@\xfam\xdf\xf8\xa4D\x10\x00\x00\x00\xb0\xd5\
+\xc1\xbf\x8c\x00\xa0\x08\x01\xfaq~\x97\x86\xe3\xfc\x9f\xa3\
+\x0d\xff\x1a\x02\x80\x0d\x02\x80I\xfe\xcf\xe1\x9a\x01\xc02\
+\xab\x00\xae{\xf3\xa4\x8f\xb8s\x1c\x82\x00\x00\x00\x80\xad\
+\x0f\xfee\x05\x00\x11\xb7o\x0dx\x94\xcf\xce\x02\x80\x92\
+\x02\x80u\x9f\xa9\x98l\x10\x00,\x13\x02,\xf3\xe69\
+y\xc4\x9d\xe3\xfe\xc3\x1f;\x0aA\x00\x00\x00\xc0V\x06\
+\xff2\x03\x80\xb3<\x04\x18\x0b\x00\xaa\x09\x00Nc\xbd\
+B\xc2Y\x1e\x02\x8c7\x08\x00\x06q~y\xc7\xbao\
+\x9e\xe9#\xee\x1c\x0f\x04\x01\x00\x00\x00\xb5\x0f\xfee\x06\
+\x00\xc5\xac\xd8\xcb\xe7\xc5\xa3\xfc\x7f\xd3\x01PR\x00p\
+\xdd\x9e\x8b\xcb|c\xf6\xf3\xdfc\xbc\xe6\xbf?*\xf1\
+\xcd3\xc9\x83\x00\x8f\x06\x00\x00\x00\xd43\xf8\x97\x1d\x00\
+D\xccW\x9c\x0b\x00J\x0c\x00\x1e\x9b\x0f\xef\x83\x0d~\
+\x9fi~0\xd7Y\x92q\x9c\x87\x0f{%\xbey\xd2\
+\x98\xaf\x08\x10\x04\x00\x00\x00T;\xf8W\x11\x00\x14!\
+\xc0L\x00\xd0\xac\x00`\x96\xff]\x92\x0d\xbe\xa9\xc3\x0a\
+\xde<g\x91\x95\x05\xee\x09\x02\x00\x00\x00*\x1b\xfc\xab\
+\x0a\x00N\x22{\x14`*\x00(/\x008\x8d\xf5\x1f\
+\x01\xb8h\x9dB\xc1\xe3\xc8V\x00\xf4+z\xf3L\x22\
+bO\x10\x00\x00\x00\x18\xfc+\x19\xfc\xab\x08\x00\x16g\
+\xcb\xabn\x1a\xb7*\x00\xe8\xed\xd2\x9b\xe9\x9b\xbf\xfe\xc9\
+q\xd7|\xa0NW\xf8WG+\xfe\xfaU\x0d#b\
+\xff\xe1\x8f\x1d\x1dE\xc4\xf4\xe4\xf44y\xe9\xab~!\
+>\xeb\x89\xf7\xa5/y\xd5\xcf\xc7\xc3\x1f;\xf4I\x00\
+\x00\x00\xec\xf4\xe0\xff#?\xfd+\xf1\x97\xbf\xe4\xbe\xf4\
+\xfe\x97\xfdd\x1cM\xa6\x11\x11Q\xf2\xf0_\x964\x22\
+b<\x1a\xc6S\x9f\xfc_\xee\xd4\xf7\xa1)\x01@)\
+\xdf\xf4\xa7\xfc\xed/\x8e\xf7\xbd\xe3\x8d\xc9\x0f\xbe\xf4\xfe\
+u\x83\x80I\xc5\x7f\xcf\x83\x88\x18,\x04\x01!\x08\x00\
+\x00\x00\x0c\xfe\xcd\x1a\xfc_t\xff=\xf1\xbew\xbc1\
+\xf9o\xbe\xe6I\xa5\xce\xac\x02\x80\x92\x0f\xe6\xc1x\x14\
+\xcfy\xd6\xdd\xeb\x04\x01\x83\x1a\xff\xbe\xe3\xc8V\x04\x9c\
+D\xc4\x89 \x00\x00\x000\xf87g\xf0\x7f\xd9\x0b\xef\
+\x8bG\xdcu\xc7\xce}_zM9\xd8e[3\x08\
+\xe8E\xd6\x07P\xd7\xb1\x1fDD\xfa\xf0\xc7\x8e\xa6\x11\
+q*\x08\x00\x00\x00\x0c\xfe\x06\xff]\x0e\x00*\xb5b\
+\x10\xd0\x8f\xfa\x97v\x0c\x22\xeb\x088\xcd\x83\x80t1\
+\x08\xf8\x81\x7f\xfe/\xe3\xf0h\xe2\x93\x04\x00\x00h\xac\
+\xc9\xf4$\xfe\xc5\xcf\xbdi\x97\x07\xfft\x17\xbeO\xbd\
+\xae\xbc!W\x08\x02\xf6\x22\xe2h\x0b/q\x94\x07\x01\
+\xc7\x0f\x7f,\x9b\xf8ONO\xe3\x05\xafxm|\xda\
+\xdf|\xa6 \x00\x00\x00h\xec\xe0\xff\x19OxV\xfa\
+\xcc\x17\xff\xb8;\xfe\x02\x80\xd6\x05\x01\xfb[>.\xe3\
+<\x0c8\x12\x04\x00\x00\x00\x06\xffF\x0c\xfe;1;\
+\xf7\xba\xfa\x86\xbd!\x08\x18D\xc4\xc9\x96_\xe28\xb2\
+G\x12&\xf9\xa3\x01\x82\x00\x00\x00\xc0\xe0_\xef\xe0_\
+\xb0\x0b\xc0\xae\x05\x01\xafx\xc9\xfdq\xe7\x1d\x07\xc57\
+\xb7\x9f\x7fm\xd3^d\x8f\x05D\x1e\x04\x9c\x09\x02\x00\
+\x00\x00\x83\xff\xb53\xd4\xadY\xefE\xdf\xf1\x8cN.\
+\xf5\x17\x00,\x11\x04<\xf7\xde\xbb\xe3\xfd\x7f\x9c\x05\x01\
+\xe3\xf10\xf2\x00\xa0\x09e\x0f\xc3\xfc\xeb$\x0f\x02B\
+\x10\x00\x00\x00\x18\xfc\xcfI#b8\x1e\x0d\xd3\x17}\
+\xc73\xe2\xcf\x1e\xfc\xb5\xe4e/\xb8\xb7\xac\xc1\xdf#\
+\x00\xbb\x1c\x04|\xe8]o\x89W\xfc\xa3o_v\xfb\
+\xc0\xba\x8c\xf3 \xe08\xb2\xb2\xc0D\x10\x00\x00\x00\x18\
+\xfc#\x06\xfd\xfd\xe4\x05\xff\xe0\xe9\xd9\x1d\xff\xf2\x06\xff\
+\x9d\x22\x00\xb8.\x08\xb8\xefi\xcbn\x1f(\x08\x00\x00\
+\x00\x0c\xfe[\x18\xfc\x87\x83A\xf2\xa2\xfb\xef\x89\x0f\xbe\
+\xeb-\xf1O^\xf4mU\x0d\xfeI\xec\xc0V\x80\x02\
+\x80%\x82\x80%\xb7\x0f\xac[\x12\xd9n\x01{\x111\
+\x89\x88\xa9 \x00\x00\x00\xd8\xf1\xc1\x7fV\xccb\xa3a\
+6\xf8\x7f\xe0\x9do\x8a\x1a\x9e\xf1O\xf2?[\x00P\
+\x82\xc6')\x0d\x0e\x02\xfa\x91\xad\x06\x98E\xc44\x22\
+f\x82\x00\x00\x00`\xc7\x06\xffi>{\xf5\x8aV\xff\
+\xf7\xffq-\x83\xffb\xf0p&\x00\xe8\x98\x06\x07\x01\
+\xa3\xc8\xb6/\x9c\xe4_!\x08\x00\x00\x00Z>\xf8\x17\
+\xc3\xcb`\xbc\xddV\xff4\xac\x00(\xf5`\x0a\x02\xca\
+Q\xf4\x03\x1cF\xc4\x91 \x00\x00\x00h\xd9\xe0\x9f\xe6\
+\x83\xff\xbc\xd5\xff\xfe{\xe2}\xe5\xb6\xfa\xaf\xf3\x9at\
+\x00t5\x00hA\x10p\x90\x07\x01\xd3\xb8bE\xc0\
+\xa7?A\x10\x00\x00\x00]\x1a\xfc?\xf3\x8b\xefm\xf2\
+\xe0\x7f\x1a\xf3;\xfe\xc3b\xa9\xff\x96\xee\xf8\xef\xd4\xdc\
+\xda\xb4\x00 i\xfb\x81lh\x10\xd0\x8b\xec\xb1\x80$\
+\x0f\x02N\x17\x83\x80\xe9\x89 \x00\x00\x00\xba4\xf8\x1f\
+\x1eO\x9a8\xf8\x1f\xe7\xf3\xca^C\x07\xffb\xaek\
+\xfd\xdcj\x05@7\x82\x80A\xfeu\x12Y\xa26\x13\
+\x04\x00\x00\x80\xc1\x7f\xcb\x0e\xf3\x19e\x18\x11\x83\x86\x0e\
+\xfe;5\xb3\xf6\x1c\xd0N\x05\x01E?\xc0\xad\xa2@\
+A\x00\x00\x00\x18\xfck4\x8b\xac\xabl\x12\xd9c\xcb\
+\xfd\x86\x0f\xfe\x8b\xac\x00(\xf1@\xcev\xf1\x07\xb0\xe1\
+A\xc0q\xfe%\x08\x00\x00\x00\x83\x7f\x95\xa6\xf9\xecq\
+\x1a\xd9\x0ef\xf3r\xbf\xe6\x0f\xfe;C\x00\xd0\xed \
+`\x14\x11\xfd\xb0\x22\x00\x00\x00\x0c\xfe\xd58\xcc\x87\xff\
+^\xb4c\xa9\xbf\x00\xa0\x06{\xb1c\x8f\x00\xb4(\x08\
+\xd8\xcb\x7f\x10#\x0f\x01N\x05\x01\x00\x00`\xf0/a\
+\xf0?\x8el\xf5q?\x22\xf6[>\xf8\xdb\x06\xb0D\
+I\xd7~`\x1b\x18\x04\x0c\xf3\xaf\xa2(0\x04\x01\x00\
+\x00`\xf0_\xc1Y>K\x1c\xc7|[\xf2\xc4\x1d\x7f\
+\x01\x00\xcd\x0d\x02\x8a~\x80\xa3\xfcK\x10\x00\x00\x00\x06\
+\xff\xeb\x14\xdb\xf8\x9d\xc6\xfc\xc6b\x18\xfc\x05\x00\xd7I\
+\xba\xfc\x8dhh\x100\xca\x7f\x98\xad\x08\x00\x00\x00\x83\
+\xffEG\xf9\xe0\xbf\x1f\xf3\xad\xc7\x0d\xfe\x02\x00Z\x1a\
+\x04$y\x08\xd0\xcbC\x80\xa9 \x00\x00\x00:=\xf8\
+\x17\xdb\xf8\x1d\xe7\xb3\xc2 \xb2^1\x83\xbf\x00`\xe5\
+a\x93f\x06\x01\xfd\xc8\x96\xf1\xcc\xf2 `&\x08\x00\
+\x00\x80N\x0d\xfe\xc56~\x93\x98\xaf\x16\x0e\x83\xbf\x00\
+\x80\xdd\x0d\x02Fy\x10pn\xdb@A\x00\x00\x00\xec\
+\xec\xe0\x7f\x9c\x7f\x15\xf3\xc0\xb8\x98E:6\xf8'\xb1\
+\x037\xad\xad\x00\x10\x04\xac\xa3(\x0a\x5c\xfc0\x10\x04\
+\x00\x00\xc0\xee\x0c\xfe\xc52\xffA\xcc\x97\xfawq\xf0\
+\xdf)V\x00\x08\x026Q|\x10L\x04\x01\x00\x00\xd0\
+\xfa\xc1\x7f\xf1\xf9\xfeb\x99\x7f\xcf\xe0/\x00\xa8\x82\x15\
+\x00\xed\x0c\x02z\x91\xad\x06\xe8\xc5|\xeb\x0fA\x00\x00\
+\x00\xb4g\xf0/\x9e\xef?\x89\xf3\xcf\xf7\x1b\xfc\xe7\xd2\
+]\xf8KX\x01 \x08(K\xb1\xed\xc7i\xfe\x01\x92\
+\x0a\x02\x00\x00\xa0\xd1\x83\xffQd\xaby\x8b\xdd\xbf\x86\
+\x06\xff\xdd\x9e\x9f\x05\x00\x82\x80\xb2\x15\x8f\x05\x14K\x87\
+B\x10\x00\x00\x80\xc1\xbfQ\x83\xffa~\xad>\xcc\xbf\
+\xfa\x06\xffn\x10\x00\x08\x02*{)y\x18p,\x08\
+\x00\x00\xc0\xe0\xbf\xf5\xc1\xfft\xe1\xda\xbc\xb8V\xef\x19\
+\xfcWb\x17\x00\x04\x017\x18E\x96(N\xf3/A\
+\x00\x00\x00\x06\xff\xfa\x1c\xe7\xd7\xe1g\xf9\xb5\xf9h\xe1\
+\xff3\xf8wh\xf8\x17\x00\x08\x02\xea\xb2\x17\xf3mC\
+&\xf9\x87\x8f \x00\x00\x00\x83\x7fu\x0e\xf3k\xef\xfd\
+\xfcZ|h\xf0\xdfxv\xd6\x01\x80 `\x05\xc53\
+F\x93\xfc+\x04\x01\x00\x00\x18\xfcK3\x8b\xf92\xff\
+q~\xed\xbdo\xf0/mv\xf6\x08@\x89R\xef\xa9\
+\xce\x04\x01\x07\xf9\x87\xd1\x95E\x81\x82\x00\x00\x00\x0c\xfe\
+K+\xb6\xf1\x9b\xc4|\x99\x7fb\xf0\xaf$\x00H\xdb\
+\xfe\x97@\x10\xb0\xad `\x1c\xd9r\xa4cA\x00\x00\
+\x00\x06\xff\x95\x1d\xc5\xbcgk\x94__\x87\xc1\xbf2\
+\xb3\xfcK\x00P\x02+\x00\xba\x19\x04\xf4\xf2\x0f\xab\xbd\
+\xc8\x12\xcb\x13A\x00\x00\x00\x06\xff\x1b\x07\xffb\x1b\xbf\
+A\xfee\xf0\xaf\xc7\x99\x00@\x00 \x08\xd8\x5c?\xff\
+\x00;\xcb\x83\x80\x99 \x00\x00\x00\x83\xff\xb9\xc1\xb3\x18\
+\xfc\xc7q~\x1b?\x83\x7f=\xac\x00@\x10P\xb2Q\
+\xcc\x8b\x02\x8f\xaf\xfb\x85\x82\x00\x00\x00:0\xf8\x17\xcf\
+\xf7\x9f.\x0c\xfea\xf0\xdf\x1a\x1d\x00\x0e\xa4 \xa0\x02\
+\xc5\x87\xdb\xd1\xeaA\xc0\xb3\x04\x01\x00\x00\xb4}\xf0?\
+\x8a\xec\xa6X\x12\xf3\x9bd\x06\xff\xed\xcf\xac\x02\x00\x01\
+\x80 \xa0\xe2 \xa0\x1f7l\x1dx>\x088\x11\x04\
+\x00\x00\xd0\xd6\xc1\x7f\xb1\xcd\x7f\x98_\x0b\x1b\xfc\x9b3\
+\xb3\xb6z+\xc0\xa6=\x020\xf3\x9e\x12\x04\x5cb/\
+\xe6\x89\xe7$\xb2\xe5O\x82\x00\x00\x00ve\xf0?\x8d\
+\xf9\xca\xd7b\xf0O\x0c\xfe\xecr\x00\x90D\xcb\x1b\x15\
+\x05\x01\x95\x1b\xe6_\xa7\x91=\x0b\x95\x0a\x02\x00\x00h\
+\xf1\xe0_l\x87}\x16W?\xdfo\xf0o\x16+\x00\
+J\xe41\x00A\xc02F\x91muR|`\x86 \
+\x00\x00\x80\x16\x0d\xfe\x87\x91\xadl\xdd\x8f\xab\x9f\xef7\
+\xf87O\xebW\xac7)\x00\xd8\x13\x00\x08\x02V4\
+\xce?,o,\x0a\x14\x04\x00\x00\x18\xfc\xb7<\xf8\xcf\
+\xf2\xeb\xd6\xa3\x888\xc8\xafc\xf7\x0d\xfet5\x00\xb0\
+%\xa1 `\x1dI\xcc\x8b\x02\xa7\xf9\x97 \x00\x00\x80\
+\xa6\x0c\xfe\xd3\xc8\xee\xf6O\xf3\xeb\xd6\xf15\xbf\xd6\xe0\
+\xdf|v\x01(q\x90C\x10\xb0\xae\xbd\xc8\x1e\x0bH\
+\xf3\x0f\xd7\x1b\x97\xe7\x08\x02\x00\x00\x0c\xfe\x15:\x8c\xf9\
+\xcd\xa9a\x5c\xfd|\xbf\xc1\x9fN\x06\x00B\x00A@\
+\x19\x86\xb1B?\x80 \x00\x00\xc0\xe0_\xb2\xa3\x98o\
+\xe37\xc8\xbf\x0c\xfe\x08\x00\x04\x00\x82\x80*\xff\xe8\xfc\
+Cw\xa9~\x00A\x00\x00\x80\xc1\x7f\x03g1\x7f\xbe\
+\xbf\xe8\xa9\xea\x19\xfc\x11\x00\x08\x00\x04\x01\xf5\x06\x01\xe3\
+\xc8R\xd7\xe2\xd9+A\x00\x00\x80\xc1\xbf,\xc7\xf9u\
+\xe6I\xdc\xfc|\xbf\xc1\x1f\x01\x00\x82\x80\x1a\x82\x80^\
+\x1e\x02$1/`\x11\x04\x00\x00\x18\xfc\xd7U,\xf3\
+/z\xa8F\x06\xffNh\xfd\x0dk+\x00\xe8R\x10\
+0\x88l9\xd6,\xff\xc0^j\x1fOA\x00\x00\x80\
+\xc1?\xbfN-\x1e/\x1d\xe5\xd7\x95}\x83\xbf\x10@\
+\x00\x00\xcd\x0e\x02\x8a\x0f\xecI,\xd9\x0f \x08\x00\x00\
+\xe8\xec\xe0\x7f\x96_7N\x22[\xe2?Zb\x084\
+\xf8\xef\xa6T\x00P.+\x00\x04\x01u\x06\x01\xc5\x07\
+\xf8\xd2E\x81\x82\x00\x00\x80\xce\x0c\xfe\xc5\xaeRgq\
+\xf36~\x06\xff\xee\x10\x00\xc0\x0e\x04\x01\xfd\x98'\xbb\
+\x82\x00\x00\x80\xee\x0e\xfe\xc5\xcd\xa1~\xcc\xb7\xf23\xf8\
+S|\x9f\x05\x00\xb0\x03A\xc0^d\xc9n\xe4!\xc0\
+\xa9 \x00\x00\xa03\x83\xff,\xceo\xe37\xca\xaf\x0f\
+\x0d\xfe\xec\x14\x8f\x00 \x088o\x98\x7f\x9d\xe4A\xc0\
+\xd2\x7f\x8e \x00\x00\xa0u\x83\xff4\xe6[\xf9-\xb3\
+\x8d\x9f\xc1\xbf\xdb\xec\x02P\xb2\xd4{\x8a\x86\x04\x01\xe3\
+<\x08(\x9e\xfdZ\x9a \x00\x00\xa0\xf1\x83\xffa\xcc\
+\xb7\x86\x1e\xc5r\xcf\xf7\x1b\xfc\xe9\x85G\x00@\x10 \
+\x08\x00\x00h\xcd\xe0_l\xe37\x88\xe5\x9e\xef7\xf8\
+S\xd8k\xfb_@\x00\x80 \xe0fI\xcc\x9f\x03\x9b\
+\xc4<-\x16\x04\x00\x004\x7f\xf0?\xcb\x87\xfeID\
+\x1c\xe4\xd7u\xcb\xceA\x06\x7f.\x06\x00V\x00\x94\xc8\
+#\x0049\x08\xe8G\xb6\x1a`\x96\x87\x003A\x00\
+\x00@c\x07\xff\xe2\xd9\xfe\xd3|\xe8\x1f\xae:\x97\x18\
+\xfc\xb9@\x07\x00t0\x08(\x96\x8c\xad\xb4m\xa0 \
+\x00\x000\xf8\xd72\xf8\x1f\xe5\x83\xff~~\xcdf\xf0\
+\xa7\xec\x10\xa0\xb57\xae\xad\x00@\x10\xb0\xbe\xa2\x1f\xe0\
+0?\xd1\x08\x02\x00\x00\xb63\xf8\x17\xdb\xf8->\xdf\
+\xbfo\xf0\xa7\xa2\x99u\xd6\xd6\x17/\x00@\x10P\xc2\
+\x1f\x97\x07\x01\xd3\xb0\x22\x00\x000\xf8\xd79\xf8\x17\xdb\
+\xf8M\x22\xbb93\x8a\xd5\x96i\x1b\xfcYgf=\
+\x13\x00@\xb7\x83\x80^dIs\x12\xf3g\xcd\x04\x01\
+\x00\x80\xc1\xbf\x9a\xc1\x7f\xb1\x98y\x94\x0f\xff\xab\x0eq\
+\x06\x7f\xd6e\x05@I\xac\x00\xa0\xedA@\xb1\x9d\xcc\
+I~bZ\xf9\xc3A\x10\x00\x00\x18\xfc\xafT,\xf3\
+\xef\xc7j\xdb\xf8\x19\xfc)sf\xd5\x01\xe0`\x22\x08\
+8\xa7\xe8\x07X\xab(P\x10\x00\x00\x18\xfco\x99\xe5\
+C\xffQ\xcc\x97\xf9\xaf:\xc7\x18\xfc){n\x15\x00\
+\x94\xe4\xcc\xfb\x89\x1d\x0c\x02\x8e\xf3/A\x00\x00`\xf0\
+_N\xf1|\xffI\xac\xb7\xcc\xdf\xe0OUZ\xbb\x1d\
+`\x13W\x00\xcc\xbc\x9f\xd8\xc1 `\x14\xd9R\xb5\xc5\
+\xe7\xd5\x04\x01\x00\x80\xc1\xffvG\xf95S\x92_C\
+\x0d\xd7\xf8=\x0c\xfeT9\xb3\xb6V\xd3\x02\x80$<\
+\x02\xc0\xee\x06\x01{\xf9\x09,\xcdOj\xa7\xeb\xfc&\
+\x82\x00\x00`G\x07\xff\xc3\xc8\xee\xf8\x0f\xf3\xaf\xbe\xc1\
+\x9f\x06\x9a\x85\x15\x00\xa5\x06\x00\xb0\xebA@qR+\
+\x8a\x02\xd7\x22\x08\x00\x00v`\xf0?\x8dy\xb1\xdfA\
+\xac\xf7|\xbf\xc1\x9f:Y\x01\xb0\xc3\xaf\x07A@\x95\
+A\xc0\xc6\xfd\x00\x82\x00\x00\xa0\xa5\x83\xffqd\x8fE\
+\xceb^\xec\xb7\xf60f\xf0\x87v\x0e\xdc{a\x15\
+\x00\xdd\x0b\x02F\x0bA\x80\x15\x01\x00\xc0.\x0f\xfe\x87\
+\xf9\xf5\xce~\xac\xb7\x8d\x9f\xc1\x9f&\xb0\x0b@I\x0c\
+\xfft5\x08(Jnz\xf9I\xf1D\x10\x00\x00\xec\
+\xc8\xe0_l\xe37\x89l\x99\xff0\x0f\x00\x0c\xfe\xd0\
+\xf1\x00@\x08@\xd7\x83\x80~~R<\xcbO\x92k\
+\xef\x8a!\x08\x00\x00\xb6<\xf8O\x17\x06\xffu\xdb\xfc\
+\x0d\xfe\xb0\xe3\x01\x00\x08\x02\xe6'\xc9Il\xf0X\x80\
+ \x00\x00\xd8\xc2\xe0\x7f\x14\xf3m\x8fG\x91=\xe3o\
+\xf0gW\xb4\xfa\x86\xb5\x15\x00\xd0\xec \xa0(\x0a,\
+\xdaq\x05\x01\x00@\x93\x07\xffb\x1b\xbfM\x9e\xef7\
+\xf8\x83\x00\x00:\x1f\x04\x0c\x22[\x0d \x08\x00\x00\x9a\
+2\xf8\x9f-\x0c\xfeE\x9b\xff&3\x86\xc1\x9f6h\
+\xed\xcc\xea\x11\x00hO\x10\xd0\x8b,Q\xefE\xb6\xac\
+\xeeT\x10\x00\x00li\xf0\x9f\xe6_'\xb1\xd96~\
+\x06\x7f\xda&\x15\x00\x94\xcb\x0a\x00\x04\x01\xd7+\x96\xd4\
+\x9d\xe6'\xde\x8d~OA\x00\x00\x18\xfcWp\x14\xd9\
+\x8a\xc4$\xbf\x1e1\xf8\xd3E=/\x5c\x00\x00u\x07\
+\x01\xa3\xfc\xc4\xbbq?\x80 \x00\x00\x0c\xfe78\xce\
+\xbf\x8a\xa2\xe2\xbe\xc1\x9f\x8e\xb2\x02\x00\xd8j\x10p\x90\
+\x9f\x8c\x8f\x05\x01\x00`\xf0/q\xf0?\x8d\xf9\x8d\x86\
+Q\xfe\xb5\xe9\xefi\xf0\xa7\xed\xec\x02\x004\x22\x08\x18\
+E\x96\xc6\x17\xcf\xe4\x09\x02\x00\xc0\xe0\xbf\x8e\xe2\xa6\xc2\
+Y\x94\xf3|\xbf\xc1\x1f\x01\x80\x00\x00\x04\x01\x15\x04\x01\
+{\x91=\x160\x8b\xec\xf9\xbc3A\x00\x00\x18\xfc\x97\
+t\x98_?\xec\xc7|\xa9\xbf\xc1\x1fn\xbf\xde\x16\x00\
+\x94(\xf5\x9eB\x10\xb0\xf1\xcfAq\xd2\xdex\xdb@\
+A\x00\x00\xec\xf4\xe0?\x8bl\x99\xffQd\x8f\x15\x0e\
+\xf3\x00\xc0\xe0\x0fW\x07\x00:\x00\x80F\x06\x01E?\
+@)E\x81\x82\x00\x00\xd8\x99\xc1\x7f\x1a\xd9\x8d\x82b\
+\x1b\xbfqI/\xd7\xe0\xcf\xae\xeby\xf1\xe5\xb2\x02\x00\
+A@\xf9A\xc08\xb2G\x03\x8a\x93\xbd \x00\x00\xba\
+9\xf8\x1f\xc6\xbc+h\x18\xe5,\xf37\xf8\xd35V\
+\x00\x00\x8d\x0f\x02zy\x08\xd0\x8by\xe2/\x08\x00\x80\
+n\x0c\xfeG\xf9\xe0_l#<0\xf8\xc3f\xef{\
+\x01@\xc7\x0f&\xb4$\x08\xe8G\x96\xf6\x9f\xe5A\xc0\
+L\x10\x00\x00;9\xf8\x9f\xc5\xfc1\xc0b5`Y\
+\xd7\xff\x06\x7f\xba,i\xeb\xdcj\x05\x00t7\x08(\
+\xbd(P\x10\x00\x00\x8d\x18\xfc\x8f#\xbb\xdb_<\xdf\
+?*\xf1\xe5\x1a\xfc!\xfb9\x98\xb5\xf1\x85[\x01\x00\
+\x82\x80\xe2\xc2\xa0\xb4\xa2@A\x00\x00lu\xf0/\xb6\
+\x056\xf8Cu3\xebY\x1b_x\xaf\xc1\x07\x14\xa8\
+?\x08\xe8G\xb6\x22\xa0\xb4)]\x10\x00\x00\x95\x0e\xfe\
+i\xccC\xfca>\xf8\xf7\x0d\xfeP9+\x00J\xfc\
+\x90\x99y?\xc1V\x82\x80\xbd\x98\xb7\x01O\x22\xe2T\
+\x10\x00\x00\x8d\x1c\xfc\x8b.\x9f\xe2\xf9\xfeQ\x94\xdbL\
+n\xf0\x87%~F\x04\x00\x9b\x9bEK\x97S\xc0\x0e\
+\x05\x01\xc5\xb6@\xa7\x91-%,\xed\x03N\x10\x00\x80\
+\xc1\x7f\xa3\xc1\xff8\xff:\xcb\xcf\xd5\xe3*\x86\x1a\x83\
+?\xdc\xf8s\x22\x00(Ik\x1b\x15a\x07\x83\x80b\
+\xab\xa0\xe2b\xa34\x82\x00\x00\x0c\xfe+)\x96\xf9\xf7\
+\x17\xce\xcf\x06\x7f\xd8^\x00\x90\xb4\xf1\x857\xf5\x11\x00\
+\x01\x004+\x08\x18Gv\x97\xa1\xd4\xa2@A\x00\x00\
+\x06\xffk\xcd\xf2s\xefQ\xcc\x97\xf9\xef\x19\xfc\xa1\x11\
+3k+\xd9\x06\x10\x04\x01\xcbJb^\x148\xcd\xbf\
+\x04\x01\x00p\xcd\xe0\x9f$\xc9:\x83\xff4\xe6\x8d\xfe\
+\xe3(\x7f\x99\xbf\xc1\x1f6\xff\xf9\xb1\x02\xa0\xc4\xd7\x94\
+xOAc\x83\x80bk\xa14\xbf0)\xb5\xb4S\
+\x10\x00\xc0.\x0d\xfei\xba\xd2\xa9\xf60?\xb7\xf6\x22\
+\xbb\xdb?\xaa\xe0\xe5\x1a\xfc\xa1\xa4\x9f#\x01\x80\x00\x00\
+\xba\x14\x04\x14[\x0d\x95\xde\x0f \x08\x00\xa0\x83\x83\xff\
+q\xcc\x9f\xed\xdf7\xf8\x03]\x09\x00\xf6\x04\x00\xd0\xaa\
+ \xe0 \xbf`9\x8c\xec\x19EA\x00\x00\x06\xff\x9b\
+\x9d\xe5C\xffd\xe1\x5cZ\xc5\xb5\xb9\xc1\x1f\xaaa\x17\
+\x80\x92\x18\xfe\xa1\xbdA\xc00\xb2\xa5\x8b\xa5O\xe7\x82\
+\x00\x00vd\xf0/\x9e\xed?\xcd\x87\xfea\x95\xc3\x89\
+\xc1\x1fhz\x00 \x04\x80\xf6\x06\x01\xbd\xc8\x96.&\
+\x0b\x177\x82\x00\x00\x0c\xfe\xd9*\xb9id\xcb\xfb\x07\
+\x06\x7fh\xb5\xd6\xce\xabv\x01\x00\xaa\x08\x02\x06\xf9\xd7\
+Id\xab\x01fe\xbfVA\x00\x00-\x18\xfcg1\
+\xef\xca\xa9\xf2\xf9~\x83?\xd0\xea\x00\xc0\x0a\x00\xd8\x8d\
+ `\x1c\xd9\x1d\x8eITP\x14(\x08\x00\xa0\xa1\x83\
+\x7f\xb1\x8d\xdf$\xe6m\xfeU]\xdf\x1a\xfc\xa1~\xb6\
+\x01\x04\x04\x017\x04\x01\xa3\xa8h\xc7\x00A\x00\x00\x0d\
+\x19\xfc'\xf9\xf0\x1f\xf9yo\x5c\xf1\x00b\xf0\x87\xed\
+\x05\x00\xad\x9c\xa5\xad\x00\x00\xea\x0c\x02F\x11\xd1\xcf/\
+\x90*\x99\xcc\x05\x01\x00la\xf0?\x8a,\xe0\xee\xc7\
+\xfc18\x83?\xec6+\x00\x04\x00 \x08X\xc2^\
+\xcc\x8b\x8f&QAQ\xa0 \x00\x80\x1a\x06\xff\xe2\xf9\
+\xfe\xa3\x98\xaft\xab\xf2\xda\xda\xe0\x0ff\xd6\x9d\x0d\x00\
+\x80\xdd\x0f\x02\x86\xf9WQ\x14X\x09A\x00\x00%\x0f\
+\xfe\xc5\xf3\xfd'Q\xfd2\x7f\x83?4w\xf8\x17\x00\
+\x94|@\x81n\x04\x01EQ\xe0\x91 \x00\x80\x06\x0f\
+\xfe\xc5y*\xc9\x07\xffa\xc5/\xd7\xe0\x0f\xe6h/\
+\x1c\xd8\xe9 `\x10\x15\x16\x05\x0a\x02\x00\x0c\xfek\x0c\
+\xfe\x871o\xf3\x1fF\xf6\x9c\xbf\xc1\x1f\xbamO\x00\
+P\xc1\x07\x1f\xd0\xb9 \xa0\xb8\xab\xb2\x17\xe7\x9b\x94\x05\
+\x01\x00\xd49\xf8\x9f\xc6\xbc\xd8\xef \x1f\xfc\xab^\xa1\
+j\xf0\x87v\x05\x00\x1e\x01\x10\x00\x00%\x05\x01\xfd\xfc\
+bk\x96\x87\x003A\x00\x005\x0c\xfe\xc7\x0b\xe7\x9d\
+\xa2\xd8\xaf\x96\xeb^\x83?\xb4J\xd2\xd6\x99\xd5#\x00\
+@\x93\x83\x80Qd\x8f\x05T\xb6m\xa0 \x00\xc0\xe0\
+\x1f\xf3e\xfe\xfbQ\xfd6~\x06\x7f@\x00p\xd9\x07\
+\x22 \x08\xc8\x15E\x81\x87\x91-\xc9\x14\x04\x00\xb0\xe9\
+\xe0_l\xe37\x89\xf92\xff}\x83?\xb0$\x8f\x00\
+\x00T\x1c\x04\x14\x17h\x93\xa8\xb0(P\x10\x00\xb0\xd3\
+\x83\xff4\xe6=3u\xb4\xf9\x1b\xfca7y\x04\xa0\
+\xeb\x07\x13\xa8%\x08\xe8\xe5\x17k\xbd\xfc\xe2\xedT\x10\
+\x00`\xf0_b\xf0?\x8ay\xb9\xec0\xeay\xbe\xdf\
+\xe0\x0f\xbb\xab\x95=\x00\x02\x00\xa0\xadA@\xf1\x8c\xe6\
+idwr*\xfd\xdc\x10\x04\x00\xb4v\xf0/\x96\xf9\
+\x0f\xa3\xbe\xe7\xfb\x0d\xfe\xd0\x0d\xb3\xb6\xbd\xe0\x9e\x83\x09\
+\xb4<\x08(\x96o\x1eE\xc5\xfd\x00\x82\x00\x80\xd6\x0c\
+\xfeg\x0b\xe7\x85\xe2<Q\xd7u\xaf\xc1\x1f\xba\xe3L\
+\x00P\xde\x07\xe7\xa9\xf7\x13\x08\x02V\x08\x02\x0e\x22+\
+\x0b<\x8e\x8a\xfb\x01\x04\x01\x00\x8d\x1d\xfc\xa7\xf9\xd7I\
+~N\x18\xd7|\xfdj\xf0\x87\xeeH\xc3\x0a\x80n\x1f\
+L\xa0\x11A\xc0(\x22\xfa\x0b\x17\x81\x82\x00\x80\xdd\x1f\
+\xfc\x8f\x22[\xe6\x9fD\xb6\xc4\x7fT\xe3\xcb5\xf8C\
+w\x03\x00\x1d\x00\x00\x0d\x08\x02\xf6\xf2\x0b\xc04\xbf \
+\xac|y\x96 \x00\xa0\xf6\xc1?\xcd\x07\xff\xe3\x98/\
+\xf3\xef\x1b\xfc\x01\x01@\xfb\x02\x80V\x1eL\xa0qA\
+\xc00\xff*\xb6|\xaa\x9c \x00\xa0\xf2\xc1\xff4\xe6\
+w\xfc\xc7\xf9\xf0_\xe7~\xdc\x06\x7f\xa0\xf8,H\xda\
+\xf6\xa2{\x0e&\xd0\x81 `\x1c\xf3\xa2\xc0\xe3:^\
+\xab \x00\xa0\xf4\xc1\xbf\xe8x\x99-\x0c\xfeu_\x9f\
+\x1a\xfc\x81e\xaf?\x05\x00+H\x04\x00@EA\xc0\
+ \xe6[B\x09\x02\x00\x9a?\xf8\x1f\xe6\x9f\xd9\xc5\xb3\
+\xfd\x83\x9a_\xae\xc1\x1f\xb8\xea\xb3\xc1\x0a\x00\x01\x00\xd0\
+\xf0 \xa0\x97_@\xf6\xf2\x0b\xca\x13A\x00@\xe3\x06\
+\xffY\xcc\xb7\xf1;\x88z\xb7\xf13\xf8\x03K\x7fF\
+\x08\x00\xca\xb1\xe7\xfd\x04T\x1c\x04\xf4\xf3\x0b\xca\xb3<\
+\x08\xa8e\xe7\x91\x22\x0889=\x15\x04\x00\x9d\x1d\xfc\
+\x8f&\xd3\xab\x06\xff\xa2\xb3e\x1b\xdb\xf8\x19\xfc\x81\x9d\
+\xd7\xe4\x00\xc0\x0a\x00\xa0\x8e \xa0h\x8e\x9eDM\x8f\
+\x05DD<\xf4\xd1CA\x00\xd0\xd9\xc1\xff#\x0f\x7f\
+\xfc\xe2\xe0\x7f\x18\xf3\xad[\x8b\x02W\x83?\xd0dI\
+\xd8\x05\xa0\xd4\x83)\x00\x00\xea\x0c\x02j/\x0a\x14\x04\
+\x00\x06\xff8\x8c\xf96~\x83\xa8\xff\xf9~\x83?\xd0\
+)=\x87\x00\x10\x04\xdc\x16\x04\x0c\xc2\x8a\x00\x80\xaa\x06\
+\xff\xe2\xd1\xab\xe3\xc8\x9e\xef\x1fm\xe9\x9a\xd4\xe0\x0fl\
+J\x09`\x97\x0f&\xb03A@/\xb2\xd5\x00Id\
+KRO\x05\x01\x00\x1b\x0f\xfe\xc7\x0b\x9f\xa9\xc3\xa8\x7f\
+\x1b?\x83?P\xf6g\x89\x00@\x00\x00\xecP\x10P\
+,G=\xcd/Zk{\xceK\x10\x00\xec\xe0\xe0\xbf\
+\x9f\x7f\xa6\x0e\xb7\xf4r\x0d\xfe@\xd9\x9f)\xad[Q\
+\xef\x11\x00@\x10ps\x10P<\x9bz\x1c5\xf6\x03\
+\x08\x02\x80\x16\x0f\xfe\xc56~\xc7\xf9\xc0?\xc8\x03\x00\
+\x83?\xb0K\xac\x00\xe8\xf2\xc1\x04v>\x08X,\x0a\
+<\x12\x04\x00\x06\xff\xdb\x06\xffi>\xf4O\xf2\xcf\xcc\
+\xd1\x16\xaf\xe9\x0c\xfe@\xd5\xf3\xaa\x00@\x00\x00\xecx\
+\x10\x90\xc4\xbc(p\x1a\xf3m\xab\x04\x01@\x97\x07\xff\
+\xc5\x15R\xa3\xfcsr[\x0c\xfe@]\xb3\xb4\x00\x00\
+\xa0#A\xc0^\x1e\x02\xa4y\x080\x13\x04\x00\x1d\x1c\
+\xfc\x8be\xfe\xfd\x98?.e\xf0\x07\xba\x12\x00x\xd1\
+\x00\x1d\x0b\x02\x8ag[k\xef\x07\x10\x04\x00[\x1a\xfc\
+\x17\x9f\xef/\x96\xf9\xef\x19\xfc\x81\x8e\xd9o\xe3\x8bn\
+r\x00\x90zO\x01-\x0a\x02\x8a\xbd\xac\x8f\x04\x01\xc0\
+\x8e\x0e\xfe\xc5\xf3\xfd'\x0b\x83\xff\xd6\xaf\x15\x0d\xfe\xc0\
+\x96\xb4\xf2\x91u+\x00\x00\xca\x0d\x02\x16\xfb\x01j\x9f\
+\xbe\x05\x01@\x05\x83\xffa\xfe\x99\xd6\xcb\x87\xfe\xe1\x96\
+_\xae\xc1\x1f`\x07\x03\x00+\x00\x80\xb6\x06\x01\xbd<\
+\x04H\xf2\x10\xe0D\x10\x00\xb4t\xf0?\x8e\xf9\xb3\xfd\
+\xdb^\xeej\xf0\x07\xd8\xe1\x00\x00\xa0\xedA\xc0 \xb2\
+;egy\x100\xab\xfb\xb5\x0a\x02\x80\x15\x07\xff\xb3\
+4M\x8bN\x93\xe2\xd1\xa6m_/\x1a\xfc\x01:\x10\
+\x00\xcc|{\x80\x1d\x09\x02\x8a%\xb3\x93\xd8B?\x80\
+ \x00Xb\xf0\x9f\xe4\xcf\xf8\x9f\xe5\x9fY\xa3\x06\xbc\
+\x5c\x83?\xd0t\xb6\x01\x04\x10\x04\x5c\x19\x04\x14\xa5Y\
+[)\x0a\x14\x04\x80\xc1\xff\x92\xc1\xff(M\xd3Id\
+\xcb\xfb\x8bUK\x06\x7f\x80\x15>\xaf\x04\x00\xe5\x1dL\
+=\x00\xc0\xae\x06\x01\xfd\xc8V\x04le\xf2\x16\x04@\
+\xa7\x07\xff4\xbf\xe3_l\xe37\x8cflge\xf0\
+\x07\x84\x00\x1d\x0e\x00\x22\x22N\xbd\x9f\x80\x1d\x0d\x02\xf6\
+b~\xa7m\xb2\xad\xcf;A\x00tj\xf0?]\x18\
+\xfc\x8be\xfeMX\xbej\xf0\x07\xda\xacU\x8f\xae\xf7\
+\x1cL\x80\xad\x06\x01\xc3\xfc\xeb4\xb2m\xb6\xb6\x92\x22\
+\x0b\x02`\xa7\x07\xff\x93\xf3\xfcw\xd2\x00\x00 \x00I\
+DAT\x8f<\xfc\xf1\x934Mg\xf9\xd0?n\xc8\
+\xcb5\xf8\x03\xbb\xe0L\x00P\xdeI\xc1#\x00@W\
+\x82\x80b\x9b\xad\xa2}{+\x04\x01\xb0S\x83\xff4\
+\xbf\xe3\xbf\x97\x7f\xbe\x0c\x0c\xfe\x00\xa5\x7f\x9eY\x01P\
+\x92\x99\x00\x00\xe8`\x10P<\x8f\xbb\xb5\xa2@A\x00\
+\xb4~\xf0?\xc9\x07\xffA4c\x1b?\x83?\xb0\xcb\
+\x01\x80\x0e\x00\x006\x0a\x02\x92<\x08\xd8\x8b\xac\x1f`\
+*\x08\x00\x96\x1c\xfc\xa7i\x9a\xf6\xa3\x19\xdb\xf8\x19\xfc\
+\x01\x01\x80\x00`%\x89\xf7\x14\xd0\xe1 \xa0\x1f\xd9j\
+\x80Y\x1e\x02lm\x89\x99 \x00\x1a?\xf8\x9f\xe6\x83\
+\xff\xb0A/\xd7\xe0\x0ft!\x00h\x95\xa6w\x00\x08\
+\x00\x00A\xc0\xbc\x1f`k\xdb\x06\x0a\x02`\xbb\xa6'\
+\xa7W\x0d\xfe\x91\x0f\xfe}\x83?\x80\x99\xb5\xcd\x01@\
+\x08\x00\x00A\xc0\xb9 \xa0\xe8\x078\x8c\xac#@\x10\
+\x00\x1d\x19\xfc?\xe3\x09\xcf*\x06\xff$\x1f\xfc\x93|\
+\xf0o\xd2\xb5\x92\xc1\x1f\x10\x00\x08\x00v\xf2\xb5\x01l\
+3\x088\xc8\x83\x80iX\x11\x00]\x19\xfc/\xde\xf1\
+o\xda\x05\xb0\xc1\x1f\xe8j\x00\xd0*M\x1e\xb2\xf7\xc2\
+\x0a\x00@\x10pU\x10\xd0\x8b\xec\xb1\x80$\x0f\x02N\
+\x05\x01\xb0\xb3\x83\xff\xd9\xc2\x1d\x7f\x83?@s\xb4n\
+^\x15\x00\x00\xb4;\x08(\xf6\xf6>\x89l5\xc0V\
+\xf7\xa2\x15\x04@\xa9\x83\x7f\xe4\x83\xff\x9e\xc1\x1f\x80]\
+\x0f\x00\x12\x01\x00\xc0\xd2A@\xd1\x0f\xb0\xf5\xa2@A\
+\x00\x946\xf87\xed\xe5\x1a\xfc\x01n\xff\x5c\xd4\x01\x00\
+@#\x82\x80\xe3\x06\x06\x01!\x08\x80v\x0e\xfe\x07\xe3\
+Q\xbc\xe8;\x9ea\xf0\x07\x10\x00T\xc6\x0a\x00\x80\xf5\
+\x82\x80ad\xdb\x825iE\xc0\xd4\x8a\x00\x0c\xfe\x97\
+\x0e\xfe\xd36\xdc\xf1\xff\xb3\x07\x7f-y\xd9\x0b\xee5\
+\xf8\x03\x9c\x9fW\x05\x00\x02\x00\x80F\x04\x01\xbd<\x08\
+\x88<\x048\xdd\xf2K={\xe8\xa3\x87\x93\x888\x11\
+\x04`\xf0?w\xc7\xff\xac\xc9\x83\xbf;\xfe\x00\xbb3\
+\xb3z\x04\x00`\xf7\x83\x80A\x1e\x04\x14E\x81\xdb4\
+\x8c\x88\x99\x8e\x00\x0c\xfe\x9e\xf1\x07\xd8\x91\xe1_\x00P\
+\xf2\x01\x05\xa0\x9c `\x94\x0f\xe0G[\x0e\x02\xfa\xf9\
+kP\x16\x88\xc1\xdf\xe0\x0f\xd0f=\x01\x00\x00m\x08\
+\x02\x06\x91\x95\x04n\xa3(\xb08Y\xde\xda\xb2P\x10\
+\x80\xc1\xdf\xe0\x0f\xd0B\xad\xdb\xba^\x00\x00\xd0\xcd \
+ \x89\xf3E\x81\xd3\x9a_\xd6(\xb2G\x12\xce\x11\x04\
+`\xf07\xf8\x03\xb4,\x00h\x15\x01\x00@\xb7\x83\x80\
+\xbd\xc8V\x03$\x91\xad\x06\x98\xd5\xf8\x92\x8a?3\x04\
+\x01\x18\xfc\x0d\xfe\x00\x08\x00R\xdf\x22\x80Z\x82\x80~\
+d+\x02N\xa3\xbe~\x80\x22x\xb8\x92 \x00\x83\xbf\
+\xc1\x1f\x00\x01\x00\x00\xd5\x04\x01\x83\xfc\xeb$\xea\xe9\x07\
+\x18.\xf3\xe7\x5c\x12\x04\x84 \x80-\x0f\xfea\xf0\x07\
+@\x00\x00\xc0.\x04\x01\xc5\x8a\x80\xba\x82\x80\xa5:\x08\
+\xac\x08\xa0\x01\x83\xff\xe2\x1d\xff3\x83?\x00\x02\x80\x92\
+O`\x00l=\x088\xcd\xbf\xaa0Z\xf5_x\xe8\
+\xa3\x87G\x11\x91\x0a\x02\xd8\xd2\xe0\x1f\x1fy\xf8\xe3\xc7\
+i\x9a\x9e\x19\xfc\x01\x10\x00\x00\xb0kA\xc0~d\x85\
+\x81\xa7QM8\xbb\x1f\x11G+\xfe;I\xbe\x22`\
+\x22\x08\xa0\xc6\xc1\xbf\xb8\xe3\x9f\xc65E\x96\x06\x7f\x00\
+\x04\x00\xeb\x9d\xd0\xce|\x9b\x00\x1a\x15\x04D\x5c\xb2\x85\
+_\x09\xe7\xa3$\xd6\xdb\x85`\xf8\xd0G\x0f'\x11q\
+2\x0f\x02\x9e)\x08\xa0\xaa\xc1\x7fQ?\xb6\xbb\xff\xb3\
+\xc1\x1f\x00\x01\x00\x00\xd5\x04\x01\xafx\xc9\xfdq\xe7\x1d\
+\xb7\x1e\x0d(;\x08\x18\xc5\xfa\x8f\x19\x8c\x22b\xff\xa1\
+\x8f\x1e\x9eD\xc4\xec\xe4\xf4L\x10@\x95\x83\xff\xc5\x10\
+\xe0\xa8\xe6\x97k\xf0\x07h\xde\xdc*\x00(\xe9@\xce\
+\xbc\x9f\x00\x9a\x11\x04<\xf7\xde\xbb\xe3\xfd\x7f|kE\
+@\xba\x10\x04\x94\xd9\x0f\xb0\xee\x92\xea$\xb2\x1d\x0c\xa6\
+\x0f}\xf4p\x1a\x11!\x08\xa0\xc2\xc1\x7f\xf1Z\xaa\xae\
+U\x00\x06\x7f\x80fj\xcd\xcc\xda\x86\x0e\x00E\x80\x00\
+\x0d\x0b\x02.<\x1a\x90F\xf6h@\x19\xa1\xed\xa0\x84\
+\x978\xca_\xcb\xf1|\xd7\x00A\x00\xa5\x0f\xfe\x17\xdf\
+sU\xae\x020\xf8\x034{^m\xcd\xaau\xbb\x00\
+\x00PN\x10\x90=\x1a\xd0+\xe1\xb3{\x14\x9b\x17\xab\
+\x8d\x22\xdb\xbd`\x1a\x113A\x00\x15\x0d\xfe\x8b\x92\x0a\
+\xae[\x0c\xfe\x00\xed\x08\x00\xac\x00\x10\x00\x00t,\x08\
+\xc8\x1f\x0d\xb8\xf3\x8eq1\x0dm\xfa\x19\xbei\xbf@\
+\xf1H\xc0I\x11(\x08\x02\x0c\xfe\x15\x0c\xfe\x85QD\
+\x94\xf5F2\xf8\x03\xb4+\x00\xd0\x01P\xe2\xc1L\xbc\
+\xa7\x00\xda\x13\x04\xbc\xff\x8f\xdf\x94\xfc\xe0K\xef\x8f\x83\
+\x83\x8d\x82\x80Q\x89'\xd3a\xfe\xcf[\xab\x0a\x04\x01\
+\x06\xff\x12\x07\xff\x8b6\xe9\xc30\xf8\x03\x08\x00:\x1d\
+\x00\x84\x00\x00\xa0\x9dA\xc0\x07\xde\xf9\xa6\xe4\xe5/~\
+v\x0c\x87\x83\xe2s|\xbc\xe2o\xb5\x1f\xe5=W=\
+\x8a\xbc 0\x16\x96\xe9\x09\x02\x0c\xfe%\x1b\xc5z\xcf\
+\x81\x8e\x22\x22\xee8\x18\xc7\xcb_\xfc\xec\xf8\xd0\xbb\xdf\
+b\xf0\x07hW\x00\xd0\x1a\x02\x00\x00*\x0b\x02\x9e\xff\
+\xeco\x8a7\xfe\xc2\xabo=\x16\xb0\xc69*\x89\xf2\
+\x9e\xab\xeb\xc5\xfc\x91\x80s\xc1\xc2UA\xc0\xd1\xf1\xd4\
+7\xd2\xe0\xbf\xceu\xcb\xaa\x09R2\x1e\x0d\xe3W\x7f\
+\xf6U\xc9\xf3\x9f\xfdMq0\x1e\xf9F\x02\xb4+\x00\
+h\xcd\xcc\xda\xf3\xfd\x02\xa0\x92\xb3a\x9a\xc6+\x7f\xec\
+5\xf1\xc4\xafzf|\xfc\xf08\x8d\xec\xee\xfb\xaaF\
+\xb1y\x17\xc0E\xc5#\x01\xb7\x0di\x17\x83\x80O\xfb\
+\x9b\xff\xad \xa0e\x83\xffg~\xf1\xd6\x06\xff\xc2:\
+;YL\x8f\x8e'\xf1\x84\xaf\xfc\xfb\xf1\xc2\xef\xff\xd1\
+8;\xb3\x032\x80\x00\xa0\x9b\x01@/\x84\x14\x00\xad\
+\xf3\xff\xfc\x7f\xef\x8f\xc7|\xe9\xd3\xd2\xe7\xbd\xf4Gb\
+6\x9b\xa5i\x9a&\xb1\xfe\x169I\x94\xbf\xc5\xda8\
+\x22\xfay\x08\x90\x0a\x02vg\xf0?<\xde\xda\xe0\xbf\
+h/V\xdb\xc9\xa2\xf8\xd9\x98\xbd\xfcU?\x1d\x7f\xed\
+\x09\x7f/\xfd\xb7\xff\xf7\x9f\xfa\xe6\x02\xd0\xb9\x00`\xcf\
+\xb7\x08\xa0]\x1ex\xc3[\xe3\xd1\x8f\xff\xea\xf4\x0f\x1f\
+|w\xb20\xc0ob\x10\xd5$\xeb\xbd\xc8V\x03L\
+\xe2\x8a%\xdb\x82\x00\x83\xff\x9a\xf6\xd7|\xcf\xf6\x22\x22\
+}\xcf{\xff]\xf2W\x1e\xf7\xd5\xf1\xda_\xfaU\xdf\
+h\x80\xe6\xd3\x01Pr\x00\xa0\x03\x00\xa0\x05\x8e\x8e'\
+q\xcf\xfd\xdf\x1bO}\xc6w\xc5\xe4\xb8\xf4\x12\xbdQ\
+\xacvGu\xd5\xdf;\xbd\xee\xf7\x17\x04\x18\xfc\xd7\xd0\
+\x8f\xf5V\xae\xe4\xef\xb5\xd3\xf4i\xdf\xfa\xdd\xf1\xd4{\
+\xbe+>\xf6\xf1C\xdfx\x80f\xf3\x08@\x89\x07R\
+\x00\x00\xd0p\xbf\xf7G\xef\x8c\xcf|\xecS\xd2\x9f\xfa\
+\xd9_\x8e\xc8\xa6\xe9\xaa>\xbbO+\xfa}G\x91\x85\
+\xce\xd7&\x17\x82\x00\x83\xff\x8a\xd7X\x9b\xfc\x1c$\x11\
+q\xf6\xc0\xaf\xbc5>\xfd\xaf\xff\xdd\xf4\x7f\xfb\xdf\xdf\
+\xeeM\x00\xd0Li\xb4\xe8\xb1u\xcf\xd7\x03\xb0\xfe\x19\
+//\xfa\xfb\xa2'==>\xf0\xa1\x0fW\xfd\xc7\xad\
+\xbb\xc5\xda\xb2\xfa\x91=\x120\x15\x04\x18\xfcK|\xcf\
+n\xb2re/\x22\xce>\xfc\x91\x87\x93\xff\xe2\xc9\xcf\
+\x88\x7f\xf8\x8f_\xad \x10\xa0yZu\xd3\xda6\x80\
+\x00\xac\xe5\x8a\xa2\xbf\xaa\xedE\xf9\x85\x80\x17\x0d\xf2\xa0\
+\xe1\xc6\xc1M\x10`\xf0_B\x1a\x9bme\xb9\x17\x11\
+\x91\xa6i\xfaO~\xe4\xa7\xe2\xf3\xbf\xe4\xeb\x15\x04\x02\
+ \x00\x00\xa0>\x15\x14\xfd-\xab(W\xab\xba$\xf6\
+ \xff3\x96\x9a\xe4\x05\x01\x06\xffk\x8c\xa3\x9c\xad,\
+\x93\x888y\xe7{\xfe$\xf9\x9c\xc7\x7f\x8d\x82@\x80\
+f\xcd\xd4\x1e\x01\x00`\xf7T\x5c\xf4\xb7\xaca\x92$\
+\x83\xa8\xbeu\xb7\x1f\xd9j\x80\x89 \xc0\xe0\xbf M\
+\x92H{\xbdd\xbc\xc2{0-)\x04\xe8G\xc4\xc9\
+\xf4\xe4$\x14\x04\x024F\xab\x8a\xeb\x05\x00\x00,\xa5\
+\xc6\xa2\xbf+%ID\xaf\xd7K\xbe\xfcK\x1e\x97\xde\
+y\xc7\xc1\xe2pUi\xe0\x10Y\xf9\xe0\xd2\x89\x87 \
+`\xa7\x06\xffYd\x8f\x83\x14\xdf\xbcd4\x1a\xc5W\
+\xfe\xed'\x9e\xed\xed\xf5\x92$Y\xea\xc7`T\xe2\xfb\
+\xb4\x9f\xff^\xb3\x07~\xe5\xad\xf1\xe9\x8fy\xb2\x82@\
+\x80\xed\x07\x00\xad!\x00\x00\xe0Z5\x17\xfd]\xebS\
+?\xf9\x93\xd2?x\xf3k\xe3W\x7f\xee\x9f\xa5\xef\x7f\
+\xf0\x8d\xa7?\xf8\xd2\xfb\xe3\xae;k\x09\x02\x8aG\x02\
+VZ\xf6 \x08h\xe5\xe0?\x8b\xacgb\x92\xffs\
+\x16Y\x084\x18\x8f\x86\xe9\x8b\xee\xbf'\xde\xf7\xe0\xaf\
+%\xaf\xfb\xa9WL\x1f\xfc\xcd\x9f\x8f\xcf\xf8\x8f>e\
+\x95\x17[\xd6V\x96I~\x0dw\xf2\xe1\xff\xf0\x90\x82\
+@\x80\xedj\xd5#\xeb\x02\x00\x00\xae\xb4\xa5\xa2\xbf\x8b\
+g\xd54\x22\xe2\xee\xa7~E\xfc\x9b\xdf~]\xf2\x9f\
+\xfc\xb5GG\xccf\xd3\x83;G\xa7\xcfy\xd6\xdd\xf1\
+\xbew\xbc1\xa9)\x08\xd8\xcf\x07\xc1\xa5\x1f\x09\x10\x04\
+\xb4b\xf0?\xc9\x07\xfd\xe3\xfc+\x8d\xec\xb9\xfdad\
+w\xee\xf7\xc7\xa3a\xbc\xe8\xfe{\xe2}\xefxc\xf2\
+\xb2\x17\xde\x17\x8f\xb8\xeb\x8e\x88\x88\xf8\xdc\xcf\xfe\xccx\
+\xd7o\xfdR\xf2\xeco\xf9\xbas\xef\xd5+\x0c*\xb8\
+H\xecG\xc4\xb1\x82@\x00!\x80\x00\x00\x80\x8dl\xb1\
+\xe8\xef\x9c\xf1\xc1(~\xf95?\x14\xafy\xf5\xf7\xc6\
+\xc1x\x94\xbf\x92$\x8d4{=\x07\xe3Q\xd4\x1c\x04\
+\x0cc\xc9]\x02\x04\x01\x8d\x1c\xfc\x17\x07\xfe\xc3\xfcZ\
+h\x9c\x0f\xfb\xa3\xc8Vz\xa4\x11\x11W\x0d\xfe\xe7\xde\
+\x0c\x83A\xbc\xea\xfb\x9f\x17o\xfa\xc5\x1f\x8b\xbb.\xf9\
+\xff/\x19\xd8\xcb\xde\xc5\xa2\xd8\x1e\xf3LA \x00\xbb\
+\x10\x00\xa4\xbeM\x00\xf5iH\xd1_DD<\xee\xb1\
+\x9f\x97\xbe\xf7w^\x9f<\xf9\xcb\x9ep\xd9\xe9\xa1\x17\
+\x0b\xdb\xab\x15A\xc0\x07\xdf\xf5\xe6\xe4\xd5?\xf0\xfc\xaa\
+\x83\x80q~\x0e]kr\xefR\x10\xd0\x80\xc1\xff8\
+\xce/\xe9\xdf_\x18\xf8\x8bG;\xce\xbdW\xc6\xa3a\
+|\xdf\x0b\xee\x8d\x0f\xbd\xfb-W\x0e\xfe\x17\xfd\xad'\
+|a\xbc\xf7m\xafO\x9e\xf8\x9f?\xe6\xba\xf7]U\
+M\xd1\xfb\xf9\xdfc:=9I\x15\x04\x02\xd0\xe6\x00\
+\x00\x80\x9a4\xa3\xe8/I\xf7z\xbdx\xe5K\xee\x8f\
+\xdfz\xc3O&\x9f\xf2\x17\xff\xc2U\xbfr\x10\x91\xde\
+\x96P\x0c\x07\x83\xb8\xef\xe9_{+\x08x\xc4\x9dw\
+T\x15\x04\x0c\xf2\xafid%\x81\x82\x80f\x0c\xfe\x17\
+\x07\xfea\xcc\x97\xf4\x8f\xe3\xf2\xf7t6\xf8\x8f\xe7\x83\
+\xff\x8b\xbf\xe3\x19\xf3\x15'Kz\xd4'\xfe\xf9\xf8\xf5\
+\xd7\xfd\xf3\xf8\x89\x7f\xfa\xdd\xb1\xbf\xb7wUA\xe00\
+\xca_\x05\xb0\xf8\x9e<\x8e\x883\x05\x81\x00\xb45\x00\
+\xb0\x02\x00\xa0\xea\x0f\xdaF\x15\xfd=*~\xff\xcd\xaf\
+\x8d\xef\xbc\xf7\xee\xb8\xb9a=\xb9\xf2<V\x04\x01\x1f\
+x\xd7\x9b\xea\x08\x02Nb\x83\x82\xb7]\x0a\x02\xb60\
+\xf8\x17\xcf\xeeO\xf2\x7f.3\xf0_>\xf8\xbfk\xbd\
+\xc1\xff\xa2{\xbe\xe1+\xe3\xed\xbf\xf9s\xd7\x15\x04&\
+\x15^\xdf\x8c#\x0b\xa4N\xff\xc3G\x1e\x0e\x05\x81\x00\
+\xb41\x00p\xd6\x02\xa8Hc\x8b\xfe\x96?G\x5c\xab\
+\xa6 `\xa3G\x02v!\x08\xa8q\xf0?\x8c\xf3w\
+\xf8\x8bg\xf7\x8b\xd2\xbed\xd9\xf7M\xd9\x83\xff\xa2\x1b\
+\x0a\x02G\xb1\xe2\x8e\x12+\x1aF\xc4^\x9a\xa6\xa7\x0a\
+\x02\x01hc\x00p\xe6[\x05P\xbeF\x17\xfd-g\
+\x14\x91.\xb5\x9c\xba\x86 \xa0x$`\xb2\xe9y\xab\
+MA@\x0d\x83\x7fQ\xd87\xc9\xbf\x0e\xe2\xfc\x1d\xfe\
+U\xaf)*\x1d\xfc/\xbe\xe7n(\x08\xac\xf2\xfa&\
+\x89\xactp\x12\x0a\x02\x01\x10\x00\x00tW{\x8a\xfe\
+\x96\x9asV\x0a-j\x08\x02\x86\xb1\xe1#\x01m\x08\
+\x02*\x1a\xfc\xd3\x98/\xe9/\x86\xfe\xa2\xb0o\x98\x7f\
+\xad\xfb\xfb\xd66\xf8_tEA\xe0(\xd6\xec\x8eX\
+\xd1(\xb2\x95)\x93\x93S\x05\x81\x00\x02\x80v\xd0\x03\
+\x00P\x92v\x15\xfd-s\x86Xo\xda\xac8\x08\x18\
+\xe5\xe7\xd8\xe32\x8eW\x93\x82\x80\x92\x07\xffY\xcc\xef\
+\xf0\x1f\xe5\x03\xf1(\xce/\xeb\xdf\xf8\xfaa<\x1em\
+e\xf0_T\x14\x04\xfe\xe4\x0f\x7fO\xec\xef\xdf*\x08\
+\xdc\x8b\x0d\x1f\x1bY\xd28\x22zi\x9a\xfdY\x0a\x02\
+\x01*\x99W[1\xb3\xf6\x1cL\x80\x8e\x9c\x99\x1aT\
+\xf4\xf7\x97V*\xfa\xbb1M\x18E\xb2~\xabz\x85\
+A\xc0 \x1f`\xa7Q\xd2J\xb6m\x06\x01%\x0d\xfe\
+\xc5\xc0?Y\x18\xf8\x8b;\xfc\xe3\xc8\x96\xac\x97u\xed\
+\xb00\xf8\xbfyk\x83\xffE\xdf\xfc_?%\xde\xfe\
+\x1b\xb7\x0a\x02\xf7\xf3\xbfs\x1d!\x5c?\x7f?N\x22\
+\xe2LA @\xe93k+>Lm\x03\x08\xd0\x01\
+M(\xfa\xcb\x87\xbc\xf8\xc6\xbf\xf7w\xe2=\xab\x15\xfd\
+\xdd\x18\x01D\x09\x7f\x9f\x8a\x82\x80$\xe6[\x05\x96\xb6\
+\xf5[\x9dA\xc0\x86\x83\xffI\xcc\xef\xf0\x1f\xe7\xc7r\
+\xf1\xf9\xfdA\x05\x17`\x8d\x1c\xfc\x17](\x08L\x8a\
+\x9f\x8d\x9a\x0c#b\x9a\xa6\xe9DA @\xa9\xe7\x9f\
+V<\xb6\xde\x86\x00`\x16[*\xa5\x02\xd8\x05\x0f\xbc\
+\xe1-\xf1\xe8\xc7}\xd5\xd6\x8b\xfe\x06\xfd\xfd\xe4\x97\xff\
+\xa7\x1f\x8a\xff\xf1\x9f\xbd\xb4\x82\x81,)m\xa5XE\
+A@\xb1\x1d]\xa9\x85\x0bU\x06\x01k\x0e\xfe\x8b\x03\
+\xffa~\x9dQ\xdc\xe1\x1fE\xb6\xe4\xbd\xaa\x0b\xaf\xc6\
+\x0f\xfe\x17\xdfg\xaf\xfa\xfe\xe7\xc5\x1b\x7f\xfeG\xe3\xae\
+;\x0f\xea^\xe9X\x94'N\x22\x22\x14\x04\x02\x94r\
+\x1e\xb2\x02\xa0\xc4\x83)\x00\x00X\xd1\xd1\xf1$\xfe\xfe\
+s^\x16O}\xc6\xf3c2\xd9Zi\x5c\x1a\x11\xf1\
+\xd7?\xffs\xd2\x7f\xf7\xfbo\x88'\x7f\xf9\x13\xaa\xf9\
+S\x92\x18DZ\xee\xb3\xd4\x15\x04\x01\xa3\x98\xaf\x06(\
+\xf5.A\x99A\xc0\x8a\x83\x7f\xf1\xec~\xb1\xa4\x7f\x7f\
+a\xe0?\xa8p\xe0o\xed\xe0\x7f\xd1\x97>\xf1o\xc4\
+\xff\xf9\xbb\xff\xeabA`\x1d\x16\xdf\x8f3\x05\x81\x00\
+\xe5\x9c\x93\x04\x00e]\xda\x01\xb0\xb4\xa2\xe8\xef\x7f\xf8\
+\x99\xd7\x17g\xa4\xad|\x8e&I\x92\xbc\xe2\x1f}{\
+\xfc\xde\x1b_\xb3Y\xd1\xdf\xcd\xa7\xdc\xbd\x88\xb4\x92\xe4\
+\xbd\xe4 \xa0x$\xe0$*\xd8\x07~\x93 `\xc9\
+\xc1\xff\xe2\xc0_,\xe5/\xfeY\xd7\xfb\xac\xf5\x83\xff\
+\xa2+\x0a\x02\xeb\xba\x0e\x1cD\xc4\x89\x82@\x80\x8d\xcc\
+\x04\x00\x02\x00\x80\xda5\xa4\xe8\xef,\x22\xe2S\xfe\xe2\
+_H\xff\xf0-?\x13\xcf\xbd\xefiQ\xcf@S\xed\
+\x9fQr\x100\x8a\xf9\x96w\xa5[%\x08\xb8a\xf0\
+_\xdc\x8e\xefx\x8b\x03\xffN\x0e\xfe\x17\xcd\x0b\x02?\
+\xb5\xee\x8b\xc8a~\xf1:\x89\x88P\x10\x08\xb0\xbb3\
+\xab\x00\x00`G4\xa0\xe8\xaf\x98\x14\xf6\xee~\xeaW\
+\xc4{\xdf\xf6\xfa2\x8b\xfe\x969S\xf4\x22I+/\
+\xe0)1\x08(\xb6\xb9\x9bFE\xcf\x0d^\x17\x04\x5c\
+2\xf8'I\x92L>\xf2\xf0\xc7\x8f\xd34-\xee\xf0\
+/n\xc77\xda\xe2\xf9x\xa7\x07\xffE\x9f\xfb\xd9\x9f\
+\x19\xef\xfc\xd7\xbf\x98\xfc\x83o\xf9\xfa\xe2\x02\xa8\xae0\
+`\x9c_\x17N\xd24M\x14\x04\x02\xac~\x9e2X\
+\xdf\xecw#\xe217\x04\x11G\x91m]\xb3\x7f\xd3\
+o\xf6/\x7f\xfa\x95\xf1_=\xe9\x89\xde~@\xe7<\
+\xf0\x86\xb7\xc6\xdd\xdf\xfa\xdd\xe9\xf1\xf1d[K\xfdO\
+\xd24\xed\x1f\x8cG\xe9\xcf\xfd\x8b\x7f\x9c<\xf9\xcb\x9e\
+P\xf5\x1fy\x14\xf3\x22\xb3\xc5\xf3\xefQD2\xae\xf3\
+\xef>\x99N\xe3'\xfe\xe7\x7f\x15/\xfc\xbe\x1fM\x1f\
+\xfe\xd8\xc7\x93X\xaf\xbbf\x92\xff{\x95N\xb4\x8f\xbc\
+\xeb }\xe8\xa3\x87\xc9\xa3>\xe1\x11\x11\x91\xc4\x07?\
+\xfcP<\xf2\xae\x83x\xe8\xa3\x87E/\xc1\xb8ao\
+\xed4\x22\x92\x83\xf1(\xfd\x87\xf7\xdf\x93|\xc73\xbf\
+\xa1IC\xffQ\xd5\xc7\xeb\xcd\xff\xeb\xef\xc6\xd7\xdc\xf3\
+\xbc\xf4\xe1\x8f~\xbc\xee\x9f\xebId\xfd\x0d\xfb\x11\x11\
+\x83~?~\xe2\x87\xbf'\xee~\xea\x93|\xd8\x02\x9d\
+\xf3\xfa_\xfd\x8d\xf8\xaa\xa7?\xf7\xa6_V\xac\xe8\xbb\
+\xe9$5\x8b\x88\xdf\x8f\x88/\xdc\xd6\xdf\xa7\x0d+\x00\
+lU\x08p\xd5\x04r\xab\xe8\xef\xbbbr<\xd9\xc6\
+K8\x8b\x88H\xd3\xb4\xff\xb8\xc7~^\xfa\xde\xb7\xbd\
+\xbe\x8e\xe1\xff\xda(\xa2\xee?\xb1\xa4\x15\x01\xc3\x85\xc1\
+\xab2\xc5\x8a\x80Ox\xe4\x9d\xe9'\xfc\xb9;\x8a\xff\
+-\x22{\x0e\xbcI\xc3\x7f\x1a\x11q0\x1e\xc5\xcb^\
+x_|\xf0]oN^t\xff=;y\xc7\xff:\
+\x7f\xeb\x09_\x18\xef}\xdb\xeb\xb7Q\x108\x8c\xf9\x8e\
+\x0e\xa1 \x10`\xb9\xf3V\x1b\xb4a\xb8\xde\x0b\x8f\x00\
+\x00\xdc\xa6\x01E\x7f'\x11\xb1\xd7\xeb\xf5\xe2\x95/\xb9\
+?~\xeb\x0d?Ym\xd1\xdfR\xa7\xdf$\xd9\xd6I\
+\xb8\x84 `\x14\xd9\x8a\xb7\xca\x1e\x09(\xbc\xe7\xdf\xfe\
+i\xf2\x9e?i\xe4\xb2\xeesK\xfd\xbb:\xf8/\xda\
+bA`\xd1\xf1p\x9c\xa6\xd9g\xcb\x03\xbf\xf2\xd6\xf8\
+\x0c\x05\x81\x00W\x9d\xbfZq\xe3Z\x00\x00\xd0\xb63\
+\xcc\xf6\x8b\xfeN\xf2\x01\xb5\xff\x97>\xe5\x93\xd2?x\
+\xf3k\xe3;\xef\xbd;\x92\xa4\x01\x1f\xd5I:\x8cH\
+\x8f\xb7\xf9\x126\x0c\x02n\xb5\xb2G~\xf7\xb5C\x17\
+N\x9dx\xc6\x7f]\xf3\x82\xc0O\xa93\xe0Z\xdc*\
+0\x8d\x88\xf8\xb0\x82@\x80+\xafB\x04\x00\x1d:\x90\
+\x00uh@\xd1\xdf$\xb2\xbb\xd4\xbd\xbb\x9f\xfa\x15\xf1\
+o~\xfbu\xf5\x16\xfd-u\xd6H\x1aq\xde\xd80\
+\x08\xa8\xe5\x91\x00\x83\x7f\xbbd\x05\x81\xbfTwA\xe0\
+b(\xa5 \x10\xa0\xe53\xab]\x00\x00Z\xe2\x817\
+\xbc5\x1e\xfd\xf8\xafN\xff\xf0\xc1w'[\xf8l\x9c\
+D\xf6\xbc\xff\xf0\xe0`\x94\xfe\xf2k~(^\xf3\xea\
+\xefm\xe6\xa0\x966\xeb9\xbc\x0d\x82\x80qda\xcb\
+$Z\xf4l\xa1\xc1\xbfZ\xa3\xe1 ~\xe4\xfb\x9f\x1b\
+o\xfa\xc5\x1f\x8b\xbb\xee\xba\xa3\xce?z\x10\xd9\xca\x9f\
+\xe3\xe2\xb3\xe7\x9d\xef\xf9\x93\xe4s\x1e\xff5\xf1\xda_\
+\xfaU\xdf\x18@\x00`\x05\x80\x00\x00\xa0\x0c\x0d(\xfa\
+\x9b\xe6\x17\xff{\x8f{\xec\xe7\xa5\xef\xfd\x9dm\x17\xfd\
+\xddh\x1c\x0d\x5c>\xbff\x10\xd0\x8bl5\xc0$v\
+c5\x80\xc1\xbf$[*\x08,\xb6\x0a\x9c\x16\xff\x83\
+\x82@\x80[\xe7k\x01\x00\x00\x9b\xd9r\xd1\xdf$\xb2\
+e\xbf\x83^\xaf\x97\xfcw\xdf\xf3\xed\xcd(\xfa[N\
+cO\xc2k\x06\x01\xa3\xfc\xff?n\xe9[\xd9\xe0_\
+\x81-\x15\x04\x0e\xf2\xafID\x9c)\x08\x04\x88\x88\x16\
+\xf5\xd6\x09\x00\x00\x9a8-m\xbf\xe8o\x1a\xd9\xf2\xf3\
+[E\x7f\xcf\xfb\xd6\xa75\xe5\xf1\xfae\xc6\xcd\xc6/\
+\x99_#\x08\x18\xe5\x17\x18mZ\x09`\xf0\xaf\xc1\x96\
+\x0a\x02\x8b\xad\x02o\x85R\x0a\x02\x01\x01\x80\x00\x00\x80\
+\x15m\xb9\xe8\xefxa\xf8on\xd1\xdfM\x92\x18E\
+$\xad\x18\x94W\x0c\x02\xfa\xf9\xe05mx\x10`\xf0\
+\xaf\xd9\x96\x0a\x02G\x0b\x9f\x1b\xa1 \x10@\x00\x00\xc0\
+\x0a\x1ex\xc3[\xe3\xafl\xa7\xe8/\x8d\x88I\x92$\
+\xfd\x88\x18\x1c\x1c\x8c\xa2\xd1E\x7f\xcbD\x00\xe9\xacU\
+\xc5y+\x06\x01\x83\xc8J\x19\x9b\xf6H\x80\xc1\x7f\x8b\
+\xb6T\x10Xl\x158Y\xfc\xccR\x10\x08 \x00\x00\
+\xe0\x0a\x8bE\x7f\xc7\xf5\x17\xfd\x1dE\xc4iD\x0c\xd3\
+4mK\xd1\xdf\xceZ!\x088\x88l\xc9\xe1\xd4\xe0\
+\xcf\xa2-\x14\x04.\x96U*\x08\x04\xba\xca#\x00e\
+_X\x00\xec\xa2-\x16\xfd\xcd\xf2\x0b\xf6~\x92$\xfb\
+\xbd^/ZV\xf4w\xd3yx/\xd2\xf4l\xc7\x83\
+\x80~\xcc\xef\xben#\x080\xf87\xd4\x96\x0a\x02\x87\
+\x91\x85\x89\xf9#\x01\x0a\x02\x01\x04\x00\x00d\x93\xd3v\
+\x8b\xfe\x0e#+\xf0\x1aF\xc4\xfe\xa7~\xf2\xa3\xa2u\
+E\x7f7\xce\xff\xd1\x8f\xa47m\xfb_\xa3\x08\x02>\
+\xf8\xee7_\x17\x04\x14\x83W]\xcbGn\x0d\xfe/\
+{\xe1}\x06\xff\x06\xdbBA\xe0A~}y\xee\xbd\
+\xa8 \x10@\x00\xb0\xd6\xc5\x06\xc0.\xd8b\xd1\xdfY\
+~a>L\xb2;\xc7\xd1\xda\xa2\xbf\xa5\xcc\x92]\xf9\
+\x9b\x0c\xfa\xfd\x9b\x82\x80K\x07\xaf\xaa\x07\xff\x17\xdd\x7f\
+\x8f\xc1\xbf\xe1\xb6P\x10Xl\x158\xcd?s\x14\x04\
+\x02\x08\x00V\xbe\xe08\xf3\xed\x02v\xc1\x16\x8b\xfe\x8e\
+b~\xd7\x7fo\xdc\xfe\xa2\xbfeNsI$\xb1S\
+\xb7\x1bo\x0b\x02\xee:\x17\x04,\xee\x12P\xe6\xea\x87\
+4\x22\xe2\xc0\xe0\xdfZ[(\x08L\xf2\x10`q\xab\
+@\x05\x81\x00\x02\x00\x01\x00\xd0\x0d[,\xfa;\xc9\x87\
+\xc1a\xe4\xdbvu\xa7\xe8/\x1d\xc6,&\xbb\xf87\
+\xbb\x15\x04\xbc\xeb\xd2 \xa0\xac]\x02\xce\x0d\xfe\x1f4\
+\xf8\xb7\xde\x16\x0a\x02\x8b7\xcb\xb9\x9fC\x05\x81\x00\x02\
+\x80\x9b.@<0\x06\xb4\xd6\x16\x8b\xfe\x8a\x86\xffA\
+\x92$I\xaf\xd7\x8b\xef{\xfe\xbd\xf1\xaf\xff\x97\x9f\xd8\
+\x91\xa2\xbf\xa5\xcet\xc9.\xff\xf5.\x06\x01\x8f|\xc4\
+\x9d\x8b\x83\xd7~\xac\xb7\x12\xc0\xe0\xbf\xc3\x1e\xf5\x89\x7f\
+>\xde\xfa\xc0\x8f\xc7\x8f\xfd\xc0\x0b\xea*\x08\x1cE\xb6\
+:\xe5V\x08\xa0 \x10\xd8A\xadxd\xbdM\x01\x80\
+\x0e\x00\xa0}g\x82\xed\x15\xfd\x15\xad\xf0\xa3\x88\x18G\
+D\x14E\x7f/~\xce3\xa2\xd7\xebP\x07\xec\xac\x1b\
+\xe7\x8f\x22\x08\xf8\xc0;\xdf\xb4\x18\x04\xec\xe7\x83\xd7i\
+\xfe\xb5\xd2\xe0\xff\xa1w\xbf\xc5\xe0\xbf\xa3\x92$\x89{\
+\x9f\xfe\xd4:\x0b\x02/\xdd*0BA  \x00\x10\
+\x00\x00\xec\x80-\x16\xfd\x15\xcb\xbe\x07\xc5\x1f\xb8\xdbE\
+\x7f7M:1\x8el%D'\x9c\x0b\x02^~\xeb\
+\xd1\x80\xfd\xfc\xebd\x95\xc1\x7f<\x1a\xfaA\xdeq[\
+(\x08<\xb7U`\x84\x82@@\x08 \x00\xb8\xfc@\
+&\xdeO@[l\xa9\xe8\xef8\xb2\xbbk\xa3\xfc\x22\
+;\xbaQ\xf4\xb7d\x0c\xd01\x83~?\xee\xfb\xe6s\
+\x8f\x06\x14%\x81\xa9\xc1\x9fE[(\x08\xbcl\xc7\x0a\
+\x05\x81\xc0.\x0c\xff\x8d\xef\xadkS\x00\x00\xd0x[\
+,\xfa\x9b\xe4\x17\xd0\xb7&\xb7\xee\x14\xfd9\x8f\xdc\x18\
+\x04<\xfdk\xe3\xcf\x1e\xfc\xb5\xe4\x95/\xb9?\xee8\
+\x18\xdf\xfa\xff\xee\xbc\xe3 ^\xf9\x92\xfb\x0d\xfeDD\
+\xed\x05\x81\x8b[\x05\x9e[\xf7\xaf \x10h\xf1\xb5F\
+\xe3\x9fc\xb2\x02\x00\xa0$[*\xfa;\xca\x87\xffa\
+D\x0c\x93$I;Y\xf4w\xf3Yd\x14\xe9\xc6\x8d\
+\xf8\xad6\x1e\x0d\xe3;\xef\xbd;>\xf8\xae7'?\
+\xfd\xaa\x97\xc4O\xfc\xd3\xef9\xfd\xc0;\xdf\x94|\xe7\
+\xbdw\x1b\xfc\xb9\xa5(\x08|\xf5\xcb\x9f\x1f\xfb{\x95\
+\x17\x04^\xb6U\xa0\x82@@\x00 \x00\x10\x00\x00\x0d\
+\xfe\x80\xdaN\xd1_\x1a\xd9\x9d\xb3\xfdX\xb8\xeb\xdf\xd9\
+\xa2\xbf\x9b\xc7\x8c\xc4b\xb2y\x10\xf0M_\xf7w\xe3\
+\x9eox\xca\x9e\xc1\x9fK\x7f\x5c\x92$\xee\xfb\xe6\xaf\
+\x8d\xb7\xfffm\x05\x81\xc3\xfc3\xed\xb6\x90NA \
+\xd0\xb2\x00@\x07@\xa9\x97o\x00\x0d\xb3\xa5\xa2\xbf\xe2\
+\xae\xff \x22\xfa\xc5d\xdb\xe9\xa2\xbf\xe5\xa6\x1a\xc7\xe0\
+\xe2\x85J\x92\x9c8\x0c\x5c\xa5\xe6\x82\xc0q\x5c\xb2m\
+\xa5\x82@\xa0\x85!\x80\x00@\x00\x00\xec\xa2-\x14\xfd\
+\xcd\xf2\x8b\xe3~dE\x7f\xd9U\xb3\xa2\xbf%\xcf\x22\
+\xe9\xbe\x81\xf7\xc25\xc0lv\xe60p\x9d\x9a\x0b\x02\
+\xf7#\x0b6'q~\xc7\x0a\x05\x81@[\x86\xff\xc6\
+\xcf\xac\x02\x00\x80\x15m\xa9\xe8\xef(\x1f\xfe\x07\xf9E\
+rD(\xfa[\xed\xb4\x9c\xecG\x9a\x9e:\x10N\xad\
+\xac\xae\xe6\x82\xc0b\xab\xc0\xdb\xb6\xefT\x10\x084<\
+\x00h\xbc\xb6\x04\x00\x89\xab\x14\xa0\x09\xb6P\xf4w\x12\
+\xf3\x92\xbfQD\x84\xa2\xbf\xcdR\x00\xc7\xe0\xdc\xe9u\
+\x10\xd1\xedrD\x96WsA\xe08\xbf\xf6;\x97\xb2\
+*\x08\x04\x1a\x1e\x004~\xbenS\x00\x00\xb0\xbdO\
+\xf4\xed\x14\xfd\x1dG\xb6\xec\x7f\xb8\xf8y\xad\xe8o\x93\
+od/\x89H4\x89\xdd:\xbb\xa6\xde@\xac\xf6\x96\
+\xa9\xb7 p\x14Wl\x15\x18\xa1 \x10hd\x00\xe0\
+\x11\x80\x92\xecE\xbb\x1eW\x00v\xc8\x16\x8a\xfe\xa61\
+/\xf9\x1bF\xcc\xcb\xb7\x14\xfdm<\xf0\x0e#\xd2\x89\
+\x03\xb1x\xb9\x92\xda\x1e\x81\x95\x15\x05\x81\xcf\xfe\x96\xaf\
+\x8b\xc5\xcf\xa8*~j\x17B\x80\x0b\xab\x01\x14\x04\x02\
+\xecr\x00\x00P\xbb-\x14\xfd\x1dGv!}\xee\xae\
+\xbf\xa2\xbfR\xc7\x09\xab\xca\xce\x1d\x8fd\x1c\x91\x1e9\
+\x10\xacj4\x1c\xc4\xab\xbe\xffyu\x15\x04\x8e\xe2\xf2\
+\xad\x02\xcf\x15\x04\xfe\xcc\x03\x0a\x02\x81-^aX\x01\
+\xd0\xad\x83\x09\xec\x8e-\x14\xfdM\xf2\x0b\xdbQ>\xfc\
+\xdf\xf27\x1e\xa3\xe8\xafTnx_rL\x12\xab\xec\
+X[\x8d\x05\x81\xa3\xc8n\x0a]\xfa\xa1|rz\x92\
+\xde}\x9f\x82@\xc0l\xbd\x0b\x01\x00@m\xb6P\xf4\
+7]\xb8\xb8\x8d\x88\xf3E\x7f\xbf\xf5\x06E\x7f\xe5J\
+F\x91\x86;\xde\xe7\x0eI\x1a\x91\xe8F`}5\x16\
+\x04\xf6#\x0bI\xa7\x91\xed\x14p\x8b\x82@`\xcb\xf6\
+\xc2\x0a\x00\x80\xf6\xd8B\xd1\xdfq\x5cx\xd6\xbf\xa0\xe8\
+\xaf\xea\x81\xd7\xaa\xb2\x0b\x07d\x18\xa9n\x046|\x17\
+\xd5[\x108\x88l\x97\x94Kw\xb1P\x10\x08\x08\x00\
+\x04\x00\x00W\xaa\xb9\xe8/\xcd\x07\xffdq\xf0W\xf4\
+W\xab4<\x09p\xf1\x90\x08E(E\x8d\x05\x81\xc5\
+V\x81\xb7\x85\x00\x0a\x02\x81-\xd0\x01P\xc1\x053@\
+\xe9j.\xfa;\x8al\xe9\xea0.\xdc\xf5W\xf4W\
+\xeb)z\x18\xc9\xe5w\x0e\xbb{L\x92\xbdH\xe2\xc4\
+\x81\xa0\x0c5\x16\x04\x16\x9f\xa5\x97m\x15\xa8 \x10\xa0\
+\xc5\x01\x00@\xb9\x93x\xbdE\x7f\xb3\xc8\xee\xfa\xef]\
+\x1c\xfc#\x14\xfd\xd5.u\xfe\xbb\xe4\x98\xf4#\x8d3\
+\x07\x822\xd5T\x10x\xe5V\x81\x05\x05\x81@M\xac\
+\x00\x00h\xa2\x9a\x8b\xfe\x0ec~\xd7\x7fp\xeb\x0c\xa1\
+\xe8o\xeb\x13/\x0e\x0a\xd5\xbb\xbd \xb0\xb2?j\x14\
+Y\xd8z\xc9#\x01\x0a\x02\x01\x01\x80\x00\x00\xe8\xdet\
+So\xd1\xdfY>\xf8\x0fb\xa1\xe1\xbf\xa0\xe8o\xeb\
+\xe7\xe8~\xa4\x96\xbc_\xb8l\x19Fb\x87\x04*x\
+k\x9d+\x08\xfc\xd4*\x83\xa6qD\xec\xc7\x15+\x01\
+\x22\x14\x04\x02\xdd\xe6\x8a\x13\xe8\x8c\x9a\x8b\xfe\x0e#k\
+\xa8\x1e\xe4\x17\xa3\xf9|\xa5\xe8\xafA\xf6\xa2w~\x1b\
+\xb1\xceK\xa3\x173\xd7\x06T\xa7\xa6\x82\xc0\xfd\xc8V\
+\x5cM\x22n\xff\x19W\x10\x08\x08\x00\xda\xc3\xb3\x89\xc0\
+Zj,\xfa;\x89\xec\xae\xff(.\xb9\xeb\xaf\xe8\xaf\
+q\x03\xaf\xe6\xfb\x8b\x92pK\x94J\xd5\x5c\x10x\x1a\
+\x97\xaf\x06P\x10\x08\x08\x00\x1a\x7f\x99&\x00\x00VT\
+s\xd1\xdfQ~\xb19\xb8\xec\xf3U\xd1_#\xcf,\
+\xbd\x08\x03\xef\x05\xe3H=\x06@\xf5j*\x08\x1c\xe5\
+\xbf\xef\x95\xbb~(\x08\x04\x04\x00\xcd\x0d\x00\x5c\xa4\x01\
+K\xab\xb1\xe8o\x12\xf3\xbb\xfe\xe3\xc5\xffC\xd1_\xc3\
+%1\x88H'\x0eD\xab\xaf\x0fh\xb1\x9a\x0a\x02G\
+1\xdf%\xe0\xb6\x90AA P\xf2\xcc\xea\x04_\xe2\
+\xc1\xd4N\x0c\xdc\xfcaQo\xd1\xdfq\xfe\xd94\x88\
+K\x02\x06E\x7f\xadH\x01|c.g\xd5\x1d\xf5\xfc\
+\x04\xd6S\x10\xd8\x8b\x1b\xb6\x0a\x8cP\x10\x08\x08\x00\x04\
+\x00@\xab\xbc\xef\x03\xff>\x1e\xf7\x15\xdf\x5cG\xd1\xdf\
+q\xfeu\xdb\xb3\xfe\x8a\xfeZw\xaavn\xb9m\x22\
+\x8b\xa1\x1d\x12\xa8[M\x05\x81\xc3\xb8b\xab\xc0\x88\xf3\
+\x05\x81\x8f\xfd\xb2\xa7\xa5\xff\xef\x9f~\xc07\x06\xd8)\
+m\x0b\x00\x00\xae\xf4\xc0\x1b\xde\x1a\x9f\xf5\x05OI\xdf\
+\xf6\x07\xef\xa8\xba\xe8o\x9a\x7f~^\xda\xe2\xa7\xe8\xaf\
+u\xc3\xee(\x22\xf5\xcc\xfb\xed\xc7\x05jWSA\xe0\
+8\x7f\x87O\xaf{\xf7\xff\xd1;\xde\x93\xfc\xe5/\xfc\
+J\x05\x81\xc0N\xcd\xacm\x0b\x00\x5c\x8e\x00\xb7\xa9\xb1\
+\xe8\xef0\xb2\xbbF\x83\xfc\xeb6\x8a\xfeZ;\xed:\
+\xbf\xdcn?\xd2+\x07$\xa8T\x0d\x05\x81\xc3\xfcs\
+|\x12\xd7<\xee\xa2 \x10\xd8\xb5\x10@\x00\x00\xb4\xda\
+\xef\xfd\xd1;\xe3\xb3\xbe\xa0\xf2\xa2\xbf4\xb2;E\xfb\
+q\xc9]\x7fE\x7f\xbbp\xaaN\xad2\xbb,\x00H\
+R\x0fA\xb355\x15\x04\x0e#\xdb\xbeur\xf9G\
+\x83\x82@`\xe5k\xc6Fw\xe8(>\x02Z;\xaf\
+\x15E\x7f\xef\xff`\xa5E\x7fG\xf9\xf0\x7f\xe5]\x7f\
+E\x7f; IF\x91^\xbdMX\x87\x0f\x8c`\x84\
+-\xffh\xd6R\x10x\xe3V\x81\x11\x0a\x02\x81\xa5\x03\
+\x80F\x7f@\xb8R\x05Z\xa7\xa6\xa2\xbfYdw\x84\
+\xfa\x91\xdd!:\x7fQ\xaa\xe8o\xe7\xe6\x0ck\xcc\xae\
+\x1c\x8c\xf4#\xb0u5\x14\x04^\xbbU`\x84\x82@\
+@\x00\xb0\x8d\x83\xe9\xf2\x0c:\xae\xa6\xa2\xbf\xe2\xae\xff\
+0\xb2e\xff\xb7Q\xf4\xb7\xb3'm\xceKl\x93H\
+S\xd4P\x10\xb8\xccV\x81\x0a\x02\x81V_O\x08\x00\
+\x80V\xa8\xa9\xe8\xafx\x0et\x10W4\xfcG(\xfa\
+\xdb\xe1Qw\xa0\xf4\xee\xb2\xb3\xef,\xf5(\x00MR\
+SA\xe0Y\xdc\xf0H\x80\x82@\xe0\x8a\x99U\x00P\
+\xea\xe5\x19\xd095\x15\xfd\x1d\xe7\x17|\xc3\x88\xd8\xbb\
+\xed\xc3G\xd1_\x17N\xd9{\x11J\xefn?\xf3&\
+\xa3\x88\x99~\x04\x1a\xa5\x86\x82\xc0\x83\xfc:\xf9\xca\xc4\
+YA pE\x00\xd0\xe8\x19\xbbM\x01@\x22\x00\x80\
+\x8e}\x82\xd6S\xf4W,\xf5\xbc\xf6\xae\xbf\xa2\xbf\xce\
+L\xbb\x0e\xc1\xe5\xc7\xc5\x9b\x9e\xe6\xbd+\xab/\x08,\
+\xca_\xa7qC\xab\xb7\x82@`!\x00h4\x01\x00\
+\xd0H5\x15\xfd\x1d\xe7\x1f\xd4\xc3\xcb>\x0f\x15\xfdu\
+r\xfe\xefE\x92\x9e9\x10\xb7]\xcf$\x91$\xa7\x8e\
+\x03MTqA`\x92\x87\x00'q\xcd#\x01\x0a\x02\
+\x81\x0b\x9f\x1b\x02\x00\x01\x00\xb0\xac\x1a\x8a\xfe&\x91\xdd\
+\xd1\x19\xc5%\x0d\xff\x05E\x7f\x9d\xa4\x07\xe0\xf2S\xf0\
+ \x22=q\x1ch\xaa\x1a\x0a\x02G\x0b\xe7\x8fk/\
+\xfa\x15\x04\x02\x02\x80r\xec\x09\x00`\xb7\xd5T\xf4w\
+|k\xd0\xbb\x86\xa2\xbfN\x9f\x1a-w\xbf\xcc,u\
+\x0e\xa6\xf1*.\x08\x1cE\xb65\xec\x8d'(\x05\x81\
+\xd0YI\xe8\x00(5\x00\x00vT\x0dE\x7f\xc7\xf9\
+E\xdb\x95w\xfd\x15\xfd\x91\x0d\xba\xa5\x0f\x0d\xbb\xa1\x17\
+\xfd\x88d\xe2@\xd0t\x15\x17\x04\xf6\xf2sH\xb1\x92\
+\xecR\x0a\x02\xa1\xb3\x1a?\xb3\xb6\xed\x11\x00`\xc7\xd4\
+P\xf4\x97\xe6\x17jI\x5c\xb3\xdc?B\xd1\x1f\xc5\x99\
+1\x1dF\x1aZ\xefo\xfbIJ\xf6\x22R\xc1\x08\xed\
+\xb8h\xac\xbe p\xa9\xad\x02#\x14\x04B\x07\x03\x00\
+\x1d\x00\x00\x97\xa9\xa1\xe8\xef(\xb2;4\xc3\xab\x86\x7f\
+E\x7f\x5c>=\x08\x9d\xaf\x8a\x01\x1c\x02\xda\xa4\xe2\x82\
+\xc0q\xdc\xb0U`\x84\x82@\xe8\x98\x9e\x00\x00\xe0\x12\
+\x15\x17\xfd\xcd\xf2\x0b\xb2^\xdcp\xd7_\xd1\x1f\x06\xdd\
+\x95\x07\x9e#\x87\x816\xa9\xb8 pq\xab\xc0\xebn\
+\xef+\x08\x04\x04\x00.\xc8\xa0{j(\xfa\xbb\xf1\xae\
+\x7fA\xd1\x1f\x06\xdd\xb5\xce\xc4n\x1e\xd0J\x15\x16\x04\
+&\x0b!\xc0\x8d\x8f\x04(\x08\x84\x9dg\x05@W\x0e\
+&p\xbd\x8a\x8b\xfe\xce\xf2\x8b\xaf~\xcc\xb7k\xba\xfd\
+CD\xd1\x1f\xce9\x9b\x1e\x954\x92D O+U\
+\x5c\x108\xcaC\x85kC\x00\x05\x81\x80\x00\x00\xd8i\
+5\x14\xfd\x1dF\xc4Idw`\xf6\xaf\xfb\x85\x8a\xfe\
+X\xfe\x8dk\xd5\xd9\x95CN\x9a*I\xa4\xb5*.\
+\x08\x1c\xe7\xe7\xa1\xe92\xbfXA \xec\xe6\xc7\x8c\x00\
+\x00\xe8\xac\x8a\x8b\xfeN\xf3\x8b\xacQ\x5cw\xd7_\xd1\
+\x1f\xeb%\x00#\xdb\xde\xb5\xf3\xe2\x06\x96QaA\xe0\
+~d\x81\xf4$\xb2p\xfa\xeaO\x19\x05\x81\xe0\x1c)\
+\x00\xb8\xf9\x8a\xcc{\x0a\xda\xa1\xe2\xa2\xbf\xa3<\x00\x18\
+\xdc\xf4Y\xa6\xe8\x8f\xf5N\xdfI\x12\xe9\xcc9\xe7\xf2\
+\xab\x87^\xfe\xf3\x07\xadV\x14\x04\xbe\xf1\x17^]E\
+A\xe00\xff9\xb9i\xc5\x8c\x82@@\x00p\x0d\x17\
+\x1c\xd0p\x15\x17\xfdM\xf2\xafk\xef\xfa\x17\x14\xfdA\
+\x05f1\x884u>fg|\xe9\x17\x7fQU\x05\
+\x81Km\x15XP\x10\x08\x08\x00\xceK\xe3\xfa-V\
+\x80-\xab\xb8\xe8\xef8\xff\x1c\x18\xc65\xbf\xaf\xa2?\
+\xca\x93\xecE\x9a\x9e9\x0e\x97\x1d\x1a\x87\x80\xddRa\
+A\xe0\xb2[\x05*\x08\x04\x04\x00\x02\x00h\xc9\x0fg\
+\xb5E\x7f\xc7\xf9\xd7Rw\xfd\x15\xfdQ\xe2\x90\xdb\x8f\
+$\x99:\x10\x97\x1e\x9cA,\xb1\xe5\x19\xb4\xea]]\
+]A`\xb1U\xe0I,\xb9\xc5\xa8\x82@h\xefe\
+\xb1\x00\xa0\xdc\x83\xe9yLh\x98\x8a\x8b\xfe\xa6\xf9\x85\
+\xd3\xe8\x86++E\x7fT\x17\x03p\xf95\x84#\xc3\
+\x8e\xaa\xb0 p\x98\xff\xf3\xc6\xf0l\xb1 \xf0\x0b\xbe\
+\x5cA \xd0\xdd\x00\x00h\x90\x0a\x8b\xfe\x8a\xbb\xfe\x83\
+\x85\x0b\xa6+)\xfa\xa3\xc2\xf9?\x89\xc4\xea\xb3+\xce\
+\xca\xce\xcb\xec\xac\x0a\x0b\x02\x8b\xad\x02\x97\xe9\x05H\x22\
+\x22\xfe\xf0A\x05\x81`f\xedf\x000\x0bwb\xa0\
+\x11*,\xfaK#\xbb\xeb\xdf\x8b%\x96\xfbG(\xfa\
+\xa3\xf2\xf3\xf80\xd2\xd4v\x80W\x0d2\xe9r\xcb\x99\
+\xa1\xad**\x08\xdc\x8f,\xdc\x9e\xc6\x92\x05\xd7\x0a\x02\
+A\x00\xd0\xc5\x00 \x15\x00\xc0\xf6UX\xf4w\x94_\
+\x0c\x15\x85IWR\xf4G\xad\xca\xac\x03\xdb=\x8a6\
+\xd8y\x15\x17\x04\x9e\xc4R\x8f\x04(\x08\x04\x01@7\
+\x03\x00`9\x0f\x86E\x00\x00 \x00IDAT[\
+?\x80\xd5\x15\xfd\xcd\x22[\x0a\xd9\x8f%\x96\xfbG(\
+\xfa\xa3f3\xe7\x9f\xab?\x18\x92\x88H<\x22\xc1\xce\
+\xab\xb0 p\x1cY\x90\xbet\xe1\xa8\x82@h\xfc\xcc\
+\xda\xd8\xeb\x06W\xcd\xc0R*,\xfa;\x8a\xec\xee\xc7\
+0\xb2%\x91W_|)\xfackW\xfe1\x8e\xb0\
+\xd4\xfd\xf2+\x09\x8fH\xd0-\x15\x15\x04\x0e#\x0b\xc1\
+o\xdc*0BA \xb4@c\xb7\x10n[\x00\x90\
+\x84U\x00P\xbb\x8a\x8a\xfeNb\xc5\xbb\xfe\x8a\xfeh\
+\xc09\x88K\x8fL\xea\xd8\xd0)\x15\x15\x04\x16[\x05\
+NCA \xb4Y\xa3\xb7\xaeo\xe3\x0a\x00\x17\x19P\
+\x93\x0a\x8b\xfe\x8e\x22KFo\xbc\xeb_P\xf4GC\
+N\xe8\x5c~j\xde\x8bHO\x1c\x07\xba\xa6\xa2\x82\xc0\
+Q><\x1c/\xfb/(\x08\x84\xc6\x11\x00\x94x\xf1\
+%\x00\x80\x1aTT\xf4W\xdc\xf5\x1f\xc6\x12\x0d\xff\x8a\
+\xfeh\xd8\x19h\x14\xe9\xf2\x17\xe4\x1d\xd3\x8f\xb4\xb9\xcb\
+\x1d\xa1J\x15\x15\x04\x8e#b/\x96[\x09\xa0 \x10\
+\x9a7\xfc\xeb\x00\x10\x00@K~\xc8\xaa+\xfa;\xce\
+?\x10\x87\xcb~\xf6(\xfa\xa3Q\x12\xe7\x9f\xeb\x8fO\
+b\x85\x04\x1d~\xfbWR\x10X<\x227\x89%\xb7\
+\x0a\x8cP\x10\x08\xecV\x00\x10\x02\x00\xa8NEE\x7f\
+\x93\xc8\x9eg\x1c\xc5\x12\xcf\xfa+\xfa\xa3\xd9g 3\
+\xee\xd5W\x14\xbd\xa1\x15\x12t]\x85\x05\x81\xd3X\xf2\
+\x91\x00\x05\x81\xb0u\x8d\xbei\xdd\xc6\x12@\x01\x00T\
+\xa0\xa2\xa2\xbfI\xfe!8X\xf6_P\xf4G\xc3\xcf\
+B\xfb\x11\xe9\xa9\x03q\x89\xd9\xac\x17=\xa7h\xa8\xa8\
+ \xf0 \xff\xe7\xb2!\x9b\x82@@\x00\x00\xdc\xae\xa2\
+\xa2\xbf\xe3X\xe1Y\xff\x82\xa2?\x1a/M\xf6#I\
+\x94\xdd]\x1d\x028\x06\x90\xab\xa0 p\x14Y\xa0~\
+\x12+\x14\x8c)\x08\x84\xad\xcc\xac\x8d\x9d\xb3\x05\x00\xd0\
+a\x15\x14\xfd\xa5\xf9\xe0\xdf\x8b%\xb7\xf6S\xf4G\xfb\
+B\x00[\xde]\xf3\x03=\x8al\x97\x0f *)\x08\
+\xecE\xd6\x0dP\x94\xea.\xf1\x91\xa5 \x10\xb60\xb3\
+6V\xdb\x02\x80=\xef'(c~\xa9\xa4\xe8\xef(\
+\xb2g\x14\x87\xb1\xc2\x92\x7fE\x7f\xb4\xef\x07(\xe9E\
+$nu_y|\xc2\x0f2,N\x02\xd5\x14\x04\x0e\
+#[\x05\xb0\xd2\xd2=\x05\x81P\x8b\xfd\xd0\x01 \x00\
+\x80\xa6\xa8\xa0\xe8o\x96\x0f\xfe{\xb1\xec]\x7fE\x7f\
+\xb4\xfaj>\x06\x11\xe9\xc4\x81\xb8\xfa\x07<\x1a\xbc\xff\
+1lK\x05\x05\x81\xe3\xfcZ~\xe9\xcf#\x05\x81`\
+fm\xe3#\x00\xc0\x9a^\xf7+\xbf^v\xd1\xdfa\
+>\xfc\x0fB\xd1\x1f\xdd\x1ar\x9d\x8f\xae6\x8c\x15\xef\
+JBWTP\x10\xb8\xceV\x81\x0a\x02\xa1\xc3s\xab\
+ez\xd0\x01E\xd1\xdf\xd7\xdc\xf3\xbc\xb2\x8a\xfe\xce\x16\
+\x06\xff\x95&xE\x7f\xec\x84\xd4v\x80m\xbd\xf0\x81\
+&\xa8\xa0 \xb0\xd8*p\xa5\x93\xbc\x82@\x10\x00\x00\
+;\xa6\x82\xa2\xbf\xa3\x85\xe1\x7f\x7f\xa9O@E\x7f\xec\
+\xdey]\xd9\xdd\xf5\x97=\xfb\x91\xc6\xd4\x81\x80\xabU\
+P\x10x\x90\x07\x09\xcbn\x15\xa8 \x10\x04\x00\xc0\xae\
+\xa8\xa0\xe8\xef4\xe6%\x7f\xe3U\xfeEE\x7f8\xb9\
+w\xed\x03(\xf6C\x0f\x00\xdc\xfc!R~A`\xb1\
+U\xe04V\x5cU\xa0 \x10\xba\xc1\x958\xec\xa0\x0a\
+\x8a\xfe\x8e\xf2\x00`\xb0\xec\xe7\x86\xa2?:0\xe5\xa6\
+\xe1I\x80\xebc\x00`)%\x17\x04\xf6\xf2\xf3\xf5\xd2\
+[\x05f\x9fh\x0a\x02\xa1DV\x00\xb8\xa8\x80z\x94\
+\x5c\xf47\xc9\xbfF\xb1\xe2\xb3\xfe\x8a\xfe\xe8\xc0\xb9}\
+\x14Iz\xec8\x5cux\x92QD\xea1\x09XR\
+\x05\x05\x81\x83\xc8V\xe2\xac\xf29\xa5 \x10v\x5c[\
+\x03\x803\xdf:8\xaf\x82\xa2\xbf\xe27\x19\xae\x1a\x22\
+(\xfa\xa3+#n\xa4\x9e\x02\xb8Z\x9aD\x19O5\
+C\xc7\x94\x5c\x10Xl\x15\xb8r'\x87\x82@\xd8\xf0\
+\x1aA\x00 \x00\x80\xaa\x94\x5c\xf4w\x94\x0f\xff\xc3\xfc\
+k\xb9O\xb9$\x14\xfd\xd1\xc1\xd3\xbb\x05i\xd7\x9a9\
+>\xb0\x8e\xc5\x82\xc0\xbd\xbd\xbdM\x93\xb4b\xab\xde\xe9\
+*\xd7\xd0\x0a\x02a7\xb51\x00HC\xb1\x10\xe4'\
+\xe7\xd2\x8b\xfe\xa6\xf9\xe7\xc2p\xd5\x7f\xf1S?\xf9\x93\
+\x14\xfd\xd1E\xfdH\xe3\xc4a\xb8B\x92\x8c\x22\xb5[\
+\x02\xac\xf7\xe3\x93\x15\x04>\xf8\x9b?\x17\x9f\xf1i\xa5\
+\x14\x04\x16\xbd\x00+?\xba\xa4 \x10\x04\x00\xdb\x0e\x00\
+\xdcR\xa0\xf3J.\xfa;\xce\xbf\x06\xab\x0c\xff\x8a\xfe\
+ \xd9\x8b^r\xea8\x5c{\xa5\xe11\x00\xd8@\xc9\
+\x05\x81\xa3\x85\xf3\xfe\xf2\x17\xdf\x0a\x02a\x9d\x99U\x00\
+\xb0\xeb\x07\x13\xeaRb\xd1_\x1a\xf3\xbb\xfe+7\xf5\
+)\xfa\x83\x88H\x15\x01\x5ck\x96$\x91\xa4\x1e\xdd\x83\
+M\xa6\xf6r\x0b\x02\x17\xb7\x0a\x5c\x85\x82@\xd8\x01\x02\
+\x00h\x91\x92\x8b\xfe\x8ag\xfd\x8bg\x03W\xa2\xe8\x0f\
+n\x9d\x95z\xe1\xd1\xb4kF\x86t\x18i2u \
+`s%\x16\x04\x16[\x05NBA tjfm\
+c\x000\x8b\xb0\x9c\x90\xee)\xb1\xe8o\x96\x9f\xf0\xf7\
+b\xc5\xbb\xfe\x8a\xfe\xe0\xb2\x1f\x8c\x18D\xa4\x13\x07\xe2\
+\xba\xcb \xab$\xa0,%\x17\x04\x0e#+\x06\x5c\xf1\
+\x91\x00\x05\x81 \x00\xa8\xf7`\xba\x90\xa0C\xd7\xcd\xa5\
+\x16\xfd\x1dEV\x004\x8c5\xee\xfa+\xfa\x83+S\
+\x00?\x10\xd7\x1e\x9e\xa4\x1f\xf3\xadE\x81\x8d\x7f\xa4\xb2\
+\x82\xc0\xb7\xff\xc6\xcf\x96Q\x10Xl\x15\xb8\xd6\xcf\xa8\
+\x82@\x10\x00\x00%y\xdf\x07\xfe}<\xfe\xef\xdcS\
+F\xd1\xdfI~b\xef\xc7\x8a\x0d\xff\x8a\xfe`\xa9\xd3\
+\xbc\xc7\xd3\xae\xb7\x17\x91:FP\xb2\xbf\xfa\xe8\xcf*\
+\xab p\xad\xad\x02#\x14\x04B\xdb\xb45\x00p\x11\
+\xc1\xce+\x8a\xfe~\xe7\xf7\x1f\xdc\xb4\xe8\xef(?\x99\
+\x0f#b\x7f\xd5\x7fY\xd1\x1f,!\x89QDj\xbb\
+\xbb\xeb\x0f\x92\x98\x04*PbA`\x12\xebo\x15\xa8\
+ \x10n\x9fW\x1by\xd6kc\x00`\xf9?;\xad\
+\xc4\xa2\xbf\x93\xc8\x92\xfca\xac\xd1\xf0\x1f\xa1\xe8\x0fV\
+<=9?]o\x1cI\x08I\xa0\x22%\x16\x04\xae\
+\xb5U\xe0\xad\x8b\x0f\x05\x81P\xfc\xfc5r\x07\x1c\x8f\
+\x00@\x83\x94X\xf4w\x98\x7f\xe8\x0cV\xfd9W\xf4\
+\x07\xeb\x9e\xea-q_\xe2r\xc8u\x07T\xa8\xc4\x82\
+\xc0b\xab\xc0\x95\xefD(\x08\x84[\x04\x00%r\x97\
+\x85\x9d\x9b\x1bJ*\xfa+\xb6\xf3\x19\xc7\x9aw\xfd\x15\
+\xfd\xc1\xbag\xa6d\x14\xe9zw\xcc\xba\xf4i\x17\x89\
+\x07\x01\xa0\xda\x8f\xa2\xd2\x0a\x02{\x91\xad\x22\x9cD\xb6\
+\xaape\x0a\x02\xe9\xb0\xc6\xbe\xe1\xed\x02\x00[\xf6\xff\
+\xb7ww\xa1\xd6m\xe7]\xc0\x9f\xb9\xf6\xde\xeb\xe3\x18\
+/D\x0aZL\xcd\x87\x04\xa9\x01\xb1\xc99\x07\xb4\x90\
+\x1bkB\xdb\xd8\x8b\xa6\x085\xa6\x98\xd6\x8b\x22^(\
+4J\xedU\xad\xadB\x10jz\x0a\x85R1\xc1j\
+E\x0f\xb66 \xf5\x22*\xb4%i\x13H\x14r\x90\
+\x04z\xe1E\xd3\x98(\xa8g\x7f\xbekx1\xe7:\
+\xefz\xdf\xb3\xf7^k\xce9\xe6\x5c\xf3\xe3\xf7\x83M\
+r\x92s\xde\xb3\xf6Xk\xcd1\xc63\xc6\xf8\x8f\x8c\
+A\x7f\xd7\xd5\xf7cY\xf7;\x22\xe8\x0f\xf2\x8c\xbbE\
+\xd4\x1c\x9c\x99(\x92@O2\x06\x04\xae\xa2Y.\x80\
+\x80@\xe6N\x06@\xdeA\x16\x8c_\xa6\xa0\xbf\xabj\
+\xf2\xdf\xf8\xac\xbf\xa0?\xc86\xc1U\x018<\x1c\xb2\
+\xb5\x08z\x921 \xf0\x85h~U\xa0\x80@\x14\x00\
+\x14\x00Z7\xa4\x02\x00\xa3\x961\xe8\xef\xba\xfa>\xac\
+\x9a\xfe\x01\x82\xfe g\x01 \x96\x91\xe2FC<\xda\
+FE,\xe2NC@\x7f2\x05\x04\xee_\x15\xd8h\
+{\xb3\x80@ff\xe1E\xe5\x1a:(\x000b\x99\
+\x82\xfe.\xe3\xe9\xaa\x7f\xed\xc9\xbf\xa0?\xe8H\x8a\xb3\
+\x88\xe4\xa0\xeb\xa1ID*n5\x03\xf4+S@\xe0\
+\xfeU\x81\x02\x02\xe1\xf1\xef\xca )\x00@_\xf3\x82\
+g\x82\xfe\xbe\xd1\xf4\x8f\xd9FYy?\x8b\x16\xab\xfe\
+\x82\xfe\x80\xd3>\x10\xb7\xfaq8\xc5 :_@\xe0\
+\xaa\x1a\x934\xce\xf4\x10\x10\xc8\xc4-\x86:g\x1dk\
+\x01\x00F\xe5\xcdA\x7f\x8d>\xc7\xafW\x93\xff\xdd\x16\
+\xbc\xba_\x1cA\x7f\xd0K/\xb5XD\x91\x9eh\x88\
+Gg!\x17\x91\xe2ZC\xc0id\x0a\x08\xdcD\xc4\
+y56\xa9M@ \x13w\xae\x00\x90\xcf\x99\xcf\x13\
+c\x92!\xe8\xef\xc9\xde\xc4\xbfqB\x9f\xa0?\xe8K\
+Z\xc6V\x0e\xc0\xe3M\x14g\xae\x03\x84\xd3\xca\x14\x10\
+x^\x8dO\x9a^\x15( \x90\xa9r\x04@\x01\x80\
+\xb9\xc9\x14\xf4wYu\xa8\xcb\xaa\x93mD\xd0\x1f\xf4\
+\xdd\xbb.\xecV;\x5c\x05P\x00\x80\x01\xc8\x14\x10\xb8\
+\x8a\x88\xbbj\xdc\xd2\x88\x80@\x14\x01\x14\x00F\xd5\x90\
+\xb0/C\xd0\xdf.\x5c\xa7\xf1\xd5~\x82\xfe\xe0\x84\x9e\
+D\x11a\x85\xfb\xc0Sj\x13\xa9\xf9d\x01\xc8'S\
+@\xe0\xa6\x1a\xa77Z\xf5\x10\x10\x88\x02\x80\x02\x00\x8c\
+N\xa6\xa0\xbf\xcb(\xab\xe8\xab6\xdfQA\x7fp\xca\
+\xde5\xad\x22\xa5+\x0da\x1c\x02\xa3\x99\xa9\xe4\x09\x08\
+\x5cG\xcb\xab\x02#\x04\x04\x82\x8e\x17F C\xd0\xdf\
+u<]\xf5\xdf4\xea\xbc\x05\xfd\xc1\xb0F\xd3\x1c\x92\
+\xdaL\x12\x80\xfc2\x04\x04\x16{E\x80\x86\xbb\x01\x04\
+\x042\x8d\x91\x80\x02\x00LT\x86\xa0\xbf]\x07\xd9j\
+\xd5_\xd0\x1f\x0cjn\xeb\x08\xc0\xe1\xa1\xd1:\x22\xb9\
+\x0d\x00\x06&S@\xe0:\xca\xe2\xc1U\xe3'D\x08\
+\x08\x04\x05\x80\xa7\xac\x18pr\x19\x82\xfe\xae\xab\x8eq\
+U\xfd4\xf6\xf2{\xde-\xe8\x0f\x865\xbb\xddD\x14\
+\xce\xb8\x1fl&;%`\xa82\x04\x04\xae\xa3\x0c\xf0\
+nU\xe8\x13\x10\xc8X{8\x05\x80\xbc\xee|\xa68\
+\xa5\x0cA\x7f7{\x9dc\xc3q\xf3\xd3\xa0\xbf\xdf\xfa\
+\xf5_\x12\xf4\x07\x83\x93Ln\x0f6Q,\xa2(n\
+5\x04\x0cS\x86\x80\xc0\x8b(\x179n\x9a\x8e\xdf\x05\
+\x04\xa2\x00\xa0\x00\x10a\x07\x00\xa7\x1a\xab\xb6\x0f\xfa\xbb\
+\x8a\xb2\x12\xbe\x8c\x96\xab\xfe\x82\xfe`\xf0\x93[\xc7\x00\
+\x0e[\xc6v\xfbD3\xc0\x80g1y\x02\x02\x97Q\
+\xder\xd4* U@ \xcc\xb3\x00\x90\xc2\xf5J\x9c\
+@\xcb\xa0\xbfTM\xfc\x17m&\xfe\x82\xfe`T\xdd\
+\xd5:\xa2p\xc6\xfd\x98'\x1b0x\x19\x02\x02wW\
+\x056.\x02\x08\x08ddsV\x05\x80\xa97(\xd3\
+\xd52\xe8\xef2\xca\xado\xab(+\xe0\x8d\x09\xfa\x83\
+1\xcdk\x8b\x22\x920\xc0#\x1aj\x19-W\x05\x81\
+~d\x08\x08\xdc\xe5\x1e\xb5\xb9*P@ \xcc\xac\x00\
+`0EoZ\x06\xfdm\xa3\x5c\xf5?\x8b\x96\xdb\xfd\
+#\x04\xfd\x81.k\xaa\xf3\xff\xe4\x0c\x13\x8cL\xcb\x80\
+\xc0\xd6W\x05\xee\x08\x08\xc4\x00`\x1e\x05\x80m\xd8/\
+H\x0fZ\x06\xfd]Fy\xd6\xad\xd5\xaa\xbf\xa0?\x18\
+\xfd\xec\xf6,Rr\xc6\xfd\xf08I\xa5\x04F&C\
+@\xe0\xba\x1a\xd7\xb78\x12  \x10\x05\x00\x05\x00h\
+=\x0cm\x15\xf4\xf7$\xcaj\xf6.\xf5\xb6\x15A\x7f\
+0\xf6\xf9\x7f\x5cDH\xb9?\xa2\xa16\x11\xc9\xb5\x89\
+0\xb6on\xfb\x80\xc0MD\x9cG\xcb\x9d\x00\x11\x02\
+\x02a\xca\x05\x00\xe8L\xcb\xa0\xbf\xfdU\xff\xf3\xe6\xf3\
+\x05A\x7f0\xad\xdeV\xcd\xfa(I\x95\x13\xc6\xaae\
+@\xe0y5v\xba\x8e\x16W}\x0b\x08dh\xbd\x9a\
+\x02\xc0\x0c\x1a\x94qk\x11\xf4w\x1bOC\xfeZ'\
+\xf3\x09\xfa\x83\xa9\x0d\x01R\x11\x85\xebk\x0f*\xb6\x11\
+E\xa1\x9d`\xa42\x05\x04\xdeE\xbb\xdd\x00\x02\x02a\
+\xa2\x05\x00\xc8\xa6e\xd0\xdf\xebQn\xfb_\xe6\xf8N\
+\x09\xfa\x83IZEJ\xae\x03<<n_\xc5v\xab\
+\x9d`\xe4Z\x06\x04\xae\xab\xbf\xbf\xf5\xcd \x02\x029\
+1;\x00`\x88>\xff\xc5/7\x0d\xfa\xbb\x8er\xd5\
+\x7f\x13-W\xfd\x05\xfd\xc1\x1c\xe6\xb6\x85s\x00G\xb5\
+\x93\x8c\x1f\x98\x82\x96\x01\x81\xebxzK@\xe3I\xd4\
+\xf3\x01\x81\xbf\xfd\xbb\x02\x02Q\x04\x18k\x01\xc0\xe0\x80\
+\xf6\xdf\xc6*\xe8\xef\xa5\x0f\xfcP\x93\xa0\xbf]Uz\
+\x99\xe3\xf3(\xe8\x0ff1\x04pt\xed\xa8\x1e\xbe8\
+\x8b\xf2X\x150\xfa\xafs\xab\x80\xc0Ed\xba*0\
+\xa2\x0c\x08\xfc\x0b\xdf+ \x90\xde'\xff\x83\xbb\x05\xc8\
+L\x83Yj\x11\xf4wUuB\xebh\x99\xf0/\xe8\
+\x0ffg\x13eP(\x8f\x0f\x97.\x22\x85k\x13a\
+BZ\x06\x04\xae\xa2\xe5U\x81\x11\x02\x029Y\x01`\
+p\xd5\xa61\x17\x00\xec\x02\xa0\x91\x16A\x7f\xd7\xd5\xdf\
+\xbb\xca\xf1:6\x1bA\x7f0C\xfa\xae\xa3Z)\xd9\
+-\x01\x13\xf3L@\xe0[j\x07\x04n\xaay\xcbM\
+\x8eg\xb0\x80@z,\x008\x02\x90\xb11\x0d\xa2\xa8\
+\xa5E\xd0\xdfe5\xf9_\xe5\x9a\xfc\xbf\xfc\x1d\xefN\
+_\xf9\xac\xa0?\x98\xe9`\x80\x83C\xf4b\x15\x85\xdd\
+\x120E\xdf\xf5\xbe\x97\xe3+\x9fk\x14\x10\xb8\xac~\
+\xae#\xc3\xb6j\x01\x81\xcc\x95\x1d\x00\xccB\xc3\xa0\xbf\
+\x14e\xa5\xf9<\xc7\xc4\xff\x99\xa0\xbfO\x0b\xfa\x83\x99\
+ZE\x86d\xeb\xc9K\xb1\x88\xa4\x9f\x87\xa9j\x19\x10\
+\xb8\x8a2'\xa4U.\x80\x80@z\x9a\xaf\xda\x01\x90\
+mh\xa0\x00\xc0Q\x0f\xf7\xc6A\x7f\xbbU\xffeD\
+\x5c\xe4x-\x82\xfe\x80\x88X\xd8\x03P\xab\xaf\x07\xa6\
+:3j\x17\x10\x98\xed\xaa\xc0\x08\x01\x81tZ\x00\x18\
+\xe0@Dc2Q\x0d\x83\xfe\xb6Q\xae\xfa_D\xcb\
+\xab\xfd\xaa\x0f\xaa\xa0?@\x09\xa0\x99M$\xc7\x00`\
+\xeaZ\x04\x04f\xb9*0B@ \x9d9\x1b\xe2|\
+{\xcc\x05\x00E\x00\x1e\xd40\xe8\xef\xb2\xeaD\x96Q\
+n\xfbo?z\x15\xf4\x07\xbcy\xa8y\x11\x85k\xee\
+&>N\x01jh\x11\x10\x98\xf3\xaa@\x01\x81tQ\
+\x00\x18\xdc\x9cu\xac\x1d\xebB\x01\x80{g\xf0\xcd\x82\
+\xfev\xe7\xc8V\x91a\xd5\x7fG\xd0\x1fp\xff\xfc\xbf\
+8\x8f\x14w\x1a\xe2h\xae\x04\x84\x99h\x11\x10\xb8\xaa\
+\x9e\x15Y\x8e\x04\x08\x08d\xca\x16^7S\xd10\xe8\
+\xef*\xcam\xff\xab\x1c\x9f+A\x7f\xc0\xb1\x8f\x0bM\
+pT+\xad\xa2\xfd\xb5_\xc0\x88\xb4\x08\x08|\xa1\x1a\
+\xcb\xb5\xdd\x09  \x90I\xf7\xf7c\x9dH\x0fr;\
+\x05\xa7\xd10\xe8o\xb7Ul\x19\x99\xae\xf6\x8b\x10\xf4\
+\x07\x1ci\x1b\x8bH\xb2\x00\x8e{\xc8\xeb\xefav3\
+\xa6\xe6\x01\x81\xbb\xab\x02o\x22\xd3\xee!\x01\x81L\xcd\
+\x983\x00\x0c\x9ch\x1a\xf4wU}~\xf2\xac\xfa\x0b\
+\xfa\x03\xea\xf7\xbe\xcb(\x5c\x07x\xdcC6\x9dG\xb2\
+\x0b\x00\xe6\xa8a@`Q\x15\x01n#\xc3\x91\x00\x01\
+\x81d\x98\xb7*\x00@\x0e\x0d\x82\xfe\xae\xab\x8e`\x1d\
+\x19W\xfd\x05\xfd\x01\x0d\x87\x04V\xb6\x8fk\xa8\xf3(\
+\x92e7\x98\xa9\x16\x01\x81\xeb\xbd\xf1_\x96I\x9c\x80\
+@\xa6`\xec\x05\x00\xbb\x00f\xa8a\xd0\xdf\xcds\x9d\
+A\x16\x82\xfe\x80\xc6\xb6\xba\xb0\x1aco\x8d\x053\xd7\
+0 p\x1d\xe5\xd5\xce\xd7\xb9^\x87\x80@\xeav`\
+\x0a\x00y'\xff\x92\x81g\xa6A\xd0\xdfUd>\xeb\
+/\xe8\x0f\xc83$(\xd6\x11\xc9=\xf7\xc7YGy\
+U+0c\x0d\x03\x02\x17\xd5\x18\xf0:2\x84\x8a\x0a\
+\x08d\xec\xc6\xbe\x03@\x01`&\x1a\x04\xfd\xa5\xeaA\
+_D\xc6\xed\xfe\x11\x82\xfe\x80\xbcU\x00mp\x5cC\
+E*<p\x816\x01\x81Y\xaf\x0a\x8c\x10\x10\xc8\x91\
+\xfd\x97\x02@\xbe9a\x94\xd7\xb71q\x0d\x82\xfe.\
+\xa3\x0c~Y\xe5\x9a\xfc\x0b\xfa\x03:\xea\xca\xdc\x05P\
+\xa7\xad\x1c\x05\x00*\x0d\x03\x027\x91\xe9\xaa\xc0\xf2\xa9\
+$ \x90\xf1QMg\xd0j\x06\xfdm\xab\x07\xfaY\
+\x94[\xfe\xb3\x11\xf4\x07t\xa3XG\x91\xdc\x06pT\
+S\xc5:B[\x01O5\x0c\x08\xdc\xbf*0\xc7b\
+\xa2\x80@\x14\x00zd%`\xa2\x1a\x04\xfd\xbd\x1eO\
+W\xfd\xb3N\xfe\x05\xfd\x01\x9dNk]\x060\xa7q\
+\x0b\xd0\x81\x06\x01\x81\xc5^\x11 [aQ@ c\
+\x98\xaf\x8e\xfd\x08\x80Q\xd3\x04\xd5\x0c\xfa{R=\xbc\
+\xb3\x85\xfcE\x08\xfa\x03\xe6<4\x18t[\x15Q\x14\
+w\x1a\x02x^\xc3\x80\xc0u\xf5\x14\xceR\x04x&\
+ \xf0\xbd\x02\x02\x19\xa61\x17\x00\x9c\xff\x9f\xda\xb8\xae\
+~\xd0\xdfn\xd5\x7f\x19\x11\xe79_\x8b\xa0?\xa07\
+E\xba\x88\x14\xb7\x1a\xe2\x98\xb6\x8aeD\xd2V\xc0\xfd\
+\x8f\x88f\x01\x81\x9bj\x1cy\x93\xf3\xb5|\xf3\x7f\x09\
+\x08\xa4\x9c\xe2(\x00\xe4mL;\x00&\xa2f\xd0\xdf\
+m\xf5\x90^W?\x99\xc6\x95\x82\xfe\x80\x93\x0cY\xcf\
+baU\xfbh[}?\xf0\xb8\x06\x01\x81\xe7Q.\
+(]W\xe3\xcc\xf6\x13\x15\x01\x81\x0c\x94\xa5MN\xae\
+f\xd0\xdfeD\xdcU\x0f\xe9\xac\x9f_A\x7f\xc0\xc9\
+\xa4dR{\xf4\xc8%]D\x14\xd7\x1a\x02xL\xc3\
+\x80\xc0U5\xce\xcc\x95\x0b  \x10;\x00\xa6\xde\xa0\
+\x1c\xaff\xd0\xdfu<]\xf5\xdf\xe4~-\x82\xfe\x80\
+\xd3*\x16Qf\x9ap\xb0\xe7/\xce\xca+\x01\x01\x0e\
+k\x10\x10\x98\xf5\xaa\xc0\x1d\x01\x81\x0a\x00\x0a\x00\xccZ\
+\xcd\xa0\xbf]\x15v\x19\x19\x8f}\x08\xfa\x03\x064>\
+XF\xca{\xfe\xd4\x80\x0a\xa0\xd4  0\xf7U\x81\
+\x02\x02Q\x00`\xa6#\xb6zA\x7fW\xd5\xcf:2\
+&\xfc\xef\x08\xfa\x03\x06\xa5(<\x88\x8e\xb7\x89\x14\x97\
+\x9a\x018\xfe\x11[; pwU\xe0mD\xde\xe7\
+\x8d\x80\xc0yM\x7f\x14\x00\x98\xad\x9aA\x7f7\xd5\xe7\
+3\xeba|A\x7f\xc0p\x87\x08[\xab\xda\xf5\x9e\xe8\
+\xc60@m\x0d\x02\x02w\x8bP\xb9r\x01\x04\x04\xce\
+\xaf\x000\xa8\xfe}\xcc\x9d\xa7\xc0\xa4\x11\xa9\x11\xf4\xf7\
+z\xf5\x80\xddm\xbd\xcaJ\xd0\x1f0\xdc^\xadXG\
+X\xd5>\xbe\xbd\xd2\xe0\x06U\xc084\x08\x08\xdc]\
+\x15\x983\x17@@\xe0|\x0c*\xe3G\xf5\x9cN\xd5\
+\x08\xfaKQ\xae\xfa\x9fG\xe6U\xff\x1dA\x7f\xc0\x18\
+\xa6\xb5\x9a\xe0\xf81|d\x5c\x91\x03\xe6\xa7f@\xe0\
+y\x94\xbb\x01n\xa2\xbc) \x1b\x01\x81\x937\xa8s\
+\x1ec/\x00\x18(\x0dX\x8d\xa0\xbf\xcb\xe8h\xd5_\
+\xd0\x1f0*\xc9\x8av\xcd\xf6\xb2\x90\x01\xb4\xd20 \
+\xf06\xb2\x1e\x09\x10\x10\x88\x02\xc0q\xdd\xbe\x1d\x0c\xc3\
+|c\x8e\x0f\xfa\xdbFYE\xbd\x88\x0e\xae\xf6\x8b\x10\
+\xf4\x07\x8cL\x11\xebHV\xb5\x8fo\xaf\xa2\x88Hw\
+\x1a\x02h\xfb(\xa9\x19\x10\xb8\x89ra+\xfb\xed-\
+\x02\x02'\xd8\xb3\xcb\x00`\xcaj\x04\xfd]V\x0f\xcd\
+e\x94[\xaar~\xcb\x04\xfd\x01#\x1e(\xd8\x04p\
+\xbc\xb4\x8c\x14\x0a\x00@\x165\x03\x02WQ.be\
+\xbb*0B@\xe0\x04-\xbc\xa0\x8c\xbd\xbe\xcf\xd3\xb0\
+\x1c\x19\xf4w\x1be\x80\xca2::\xeb/\xe8\x0f\x18\
+w\x09\xa0\xd0\xbf\xd5j/M\x00\xe4S3 pw\
+U\xe0Mt\x18\x10\xf8\xcb\x02\x02\xc7\xecL\x01 \xef\
+\x17C\xb7?\x00\xcf\x04\xfd]?\xfa\xec\xbb\x8a2\x05\
+s\xd5\xd5\x97A\xd0\x1f0\xfe\x09mZF\xca\xbf\xad\
+t\xba\x16\xcb\x10\x06\x08dV3 p\x1d\xe5.\x80\
+\xec7\xb9\xdc\xde\xdd\xa5\xbf* p\xd4\xbd\xfa\xd0\xe6\
+\xac\xae\x01\xa4\x957\x05\xfd\xdd\xbf\xe5\x7fW\x15\xedd\
+\xd5_\xd0\x1f0)\xa98\x8bH\x0e~\x1e\xdf`\x8e\
+3\x02\x9d\xa8\x19\x10\xd8\xc5U\x81\x91R\x12\x108\x8d\
+\x22\x80\x02@\xa6\xd7\xae\x08p\xaa\xe1\xd6\xf1A\x7fW\
+QVLW]}\xde\x04\xfd\x01\xe8\x964\x01\xd0\xc9\
+\xcc\xad^@\xe0E5\xe6\xbd\x8e\xc8\x9fO\x22 \x10\
+\x05\x00\x05\x80\x9382\xe8\xef\xba\xfaYW\x0f\xc2\xbc\
+\x0fcA\x7f\xc0\xa4G\x9c\x8bE\x14\xe9\x89\x868\xda\
+&R\xfe\xad\xb7\x00;\x0d\x02\x02o\x22\xf3\xf1$\x01\
+\x81\xe3\xed\xd5\x15\x00\xf28S\x00\xe8\xdf\x91A\x7fW\
+{\x0f\xbfnFz\x82\xfe\x80IK\xcb\xd8\xca\x01\x98\
+\xd1\x98\x06\x18\x81\x9a\x01\x81/<7.\xce:\x99\x14\
+\x10\xa8\x000\xc7\xceR\x08`\x8f\x8e\x0c\xfa\xbb\x8a\x0e\
+W\xfdw\x04\xfd\x01\xf3\x18.\x14\xfa\xb8:R\x11\x11\
+\x85=\xb1@\xe7j\x04\x04\xae\xa3\xcc\xc0\xba\x8d\x8cW\
+\x05\xee\x08\x08dn\x05\x80\xa8\xbeH\xb6Hv\xec\x88\
+\xa0\xbfTM\xfc\x8b\xae&\xfe\x82\xfe\x809\x96\x00\xc2\
+\xd9\xf6\x1a#\x9a\xb4\x8aH\xd7\x1a\x02\xe8C\x8d\x80\xc0\
+E\x94\xd9\x00\xbb\xab\xb0\xb3\x11\x10\xc8\x1c\x0b\x00I\x01\
+\xa0\xc3\xc6=.\xe8\xef2\xca3N\xab\xe8p\xd5_\
+\xd0\x1f0C\xabH\xc9\xf5v\xf5\xd85\x01\xf4\xf7\xc0\
+\xa9\x17\x10\xb8\x8ar\xf1\xb2\x93B\xa5\x80@}\xd3\x9c\
+\x0a\x00>\xe1\x1d8\x22\xe8o\xf7\x00;\xebj\xe2/\
+\xe8\x0f0dp\x0c\xa0f\xc7q\x16\x91n5\x04\xd0\
+\xa7\x1a\x01\x81\x9bj\xfe\x95\xbd\x08  \x90\xb9\x14\x00\
+vE\x002:\x22\xe8o\x7f\xd5\x7f\xd9\xd5\xeb\x10\xf4\
+\x07\x90\xf4q\xf5F\x04\x17\x91\xec\x0c\x04\xfaW# \
+\xb0\xcb\xab\x02\x05\x042\xf9\x02\x80\x81QFG\x04\xfd\
+=\xa9&\xfe\x17Q\x86\x9atF\xd0\x1f@DD\xb1\
+\x89p\xbd]\xbd&+\x8c\x0d\x80\x93\xa9\x11\x10\xb8\xbb\
+*\xb0\x93#\x01\x02\x02\x99j\x01@\x11 \x93#\x82\
+\xfe^\x8f2\xbcd\x19\x11\xe7\xdd\x8c\xd9\x04\xfd\x01\xdc\
+\xd3\xcd9\x06Pkd\xb3XE\xc8N\x00N\xa7F\
+@\xe0\x0b\xd5\x5c&\xfb3K@ S-\x00\xa4\x10\
+\xf8\xd3\xf6\xe1p(\xe8\xef.\xca\xea\xe4::^\xf5\
+\x17\xf4\x07p\xef\xfc_\xa1\xbb\x8e\xedv\x11\xa2\x13\x80\
+\x13\xab\x11\x10\xb8\xbb*\xf0&:Z\xd8\x14\x10\x88\x02\
+\x00\x11\x11\xf1\xb5\xaf\x7f\xf3P\xd0\xdfeU\x00Xv\
+\xf5Y\x11\xf4\x07p\xb0\xab[GG[D\xa7[\x04\
+P3\x01\x86\xe1\xc8\x80\xc0E5\xde\xce~U`\x84\
+\x80\xc0\x81\xccY\x15\x008\xadW?\xfd\x99x\xfb{\
+?\xf8P\xd0\xdf\xee<R\xe7\xab\xfe\x82\xfe\x00\x0e(\
+\x8a\x22\x92\xe3n5\xdbl\x1d\xb2\x13\x80\x81\xd8\x0f\x08\
+|\xcb\xe3\x01\x81\xcb(o\xda\xea\xe2\x18\x93\x80@&\
+Q\x00H!\x03\xa0\x96#\x82\xfe\xae\xaa\x07\xcf*:\
+\xde]!\xe8\x0f\x80\xee\x8a\x00v\x08\x02\xc3\xf2]\xef\
+{9\xbez8 pwU\xe0MW\xafC@\xe0\
+I\xe6\xac\x0a\x00\xf4\xef@\xd0\xdfU\xf5\xd3\xe9\xaa\xbf\
+\xa0?\x80FO\xcf\xb3H\xc9\xf5v\xf5\x87\x5c\x0e\xbb\
+\x02\x83rd@\xe02\x9e\xe6\x02d\x7f\xf6\x0b\x08\x9c\
+7\x05\x809\x8c\x7f\x0e\x07\xfd\xddD\xb9\xda\xdf\xf9\x1e\
+|A\x7f\x00M\xe6\xff\xe9\x22\x8a\xe2FC\xd4\x9a\xfc\
+\xaf\xa3\x90\x9d\x00\x0c\xf0\x91~|@\xe0.\x17\xa0\xb3\
+\x9bM\x04\x04\xf6\xd4#)\x00\xd0\x97\x03A\x7f\xbbU\
+\xffe\x94[\xfe\xbby\xc8\x09\xfa\x03\xc81|\xd0g\
+\xd7o3\xc7\x00\x80\xc1:2 p\xbd7n\xcf\xff\
+\x98\x14\x10\xa8\x00\xc0t<\x12\xf4\x97\xa2\x5c\xf5_D\
+\x0f\xab\xfe\x82\xfe\x002(\x22\xa2\xb0\xa5\xbd\xe6(\xe7\
+<R\xd89\x01\x0c\xd6\x91\x01\x81\xfbW\x05v\xd5\xc3\
+\x08\x08T\x00`\xac\x0e\x04\xfd]V\x0f\x8f\xdd\xd9\xa2\
+N\x09\xfa\x03\xc8f\x15)\xd9\xd2^o\xc8u\x1e\xa1\
+h\x02\x0c\xdf\x11\x01\x81\xbb\xab\x02\xafC@\xa0\x22\xc0\
+\x8c\x0b\x00\xb6\xf6=\xe7\x91\xa0\xbfm\xf5\xc0\xb8\x88\x0e\
+\xb7\xfbG\x08\xfa\x03\xe8\xee\x01\xbb\xd0\xef\x8dx\xd0\x05\
+\xf0\x98#\x03\x02WQ\x06\x03vv$ B@`\
+\x07\x06S\x8c\x9e\xc2\x0e\x00\x83\xa18\x18\xf4w\x19e\
+\x80\xc8*\x22\xce\xbb~-\x82\xfe\x00\xba\x1a>$\x93\
+\xd9\xfa\xa3\x84uD\xba\xd4\x10\xc0(\x1eY\xc7\x05\x04\
+\xee\xae\x0a\xectW\x98\x80\xc0\xac\xf3U\x05\x00\xf2y\
+$\xe8\xef6\xfaZ\xf5\x17\xf4\x07\xd0\xc7\x10b\x13e\
+Q\x97:\xadV\x14\x16\x0b\x80Q9\x22 \xb0\xd3\xab\
+\x02#\x04\x04f\x9es;\x02\x90\xebs\x193\xdf\x01\
+\xf0H\xd0\xdfU\xf50\xe8e\xd5_\xd0\x1f@\x8f\x13\
+Z\xea\xd9\xda8\x01\x8c\xcf\x11\x01\x81Et\x7fU\xa0\
+\x80\xc0\x89\xcd\xb9\xed\x00\x18\xa9G\x82\xfev\xab\xfe\xcb\
+\xe8!\xe1?B\xd0\x1f@\xcf\xccfk\x0f_\x8bu\
+$;'\x80q:\x22 \xb0\xd3\xab\x02\xdf\x98d\x08\
+\x08l3\xe7\xb6\x03 \xe3 hv+!\x8f\x04\xfd\
+]Ey\xbed\xd5\xf5{+\xe8\x0f\xe0dV]\x0f\
+\xf2\xa69\xfcr\x0c\x00\x18\xaf#\x02\x02wW\x05v\
+\x96\x0b  \xb0\xdd\xf4I\x01 _C\xce\xa6C\x7f\
+$\xe8ow\x1d\xc8::>\xeb\xbf#\xe8\x0f\xe0\x84\
+}\xb7=\x00\xf5m\xa3\x88\x22=\xd1\x10\xc0h'>\
+\x87\x03\x02\x17\xd5\x5c\xe0:\xca]\xc1\x9d\x11\x10\xa8\x00\
+\xa0\x00\xd0\xb1G\x82\xfev\xab@\xcb\x1e\x1a[\xd0\x1f\
+\xc00z?%\x80\xdam\x96V\x91\x8a\x1b\x0d\x01\x8c\
+\xdd\x11\x01\x81\xab\xe86\x17@@\xe0\x88-&\xf0\xfa\
+'_\x00x \xe8\xef*\xca\xea^o\xab\xfe\x82\xfe\
+\x00\x862\x99-.\xa2\xe8vug\x92\xaa\xed\xab\x00\
+cwD@\xe0\x0b\xd1\xfdU\x81\x02\x02k\xb6\x95\x02\
+@\x9e\xd7?\xd9\xfd\xe7\x0f\x04\xfd\xa5\xea\x8b\xbc\xe8k\
+\xe2\x1f!\xe8\x0f``\x13\xd9\xf3\x88\xb8\xd3\x10\xb5G\
+\x0d\x17\x1d\x0f\x86\x01zu  p\xff\xaa\xc0N\xf7\
+\xe9\x0b\x08T\x00\xe8\xcbY\xd5\x98\x93;x\xf2@\xd0\
+\xdfe\xf5\x05^E\x1f[\xfe\x05\xfd\x01\x0c\xb8\x08\xe0\
+:\xc0\xfamV\x9c\x85[\x14\x80\x899\x10\x10\xd8\xc7\
+U\x81\x02\x02Gd\x0a\x19\x00iJ\x05\x80\x07\x82\xfe\
+\xb6Q\xaeX\x9cE\x8f\xab\xfe\x82\xfe\x00\x06l\x1b\x8b\
+H\x85\xe4\xa5\x06]\xad\x12\x0005G\x04\x04\xae\xaa\
+yS\xe7\xb7\xc8\x08\x08|p\xde\xaa\x00\x90m\x084\
+\x91\x02\xc0\x03A\x7f\xfd\xae\xfa\x0b\xfa\x03\x18\x87E,\
+\xa3H\xb6\xb3\xd7\xb7\x89\x22.5\x030E\x07\x02\x02\
+7\x11q\x1e\x1d\x1f\x85\xda\x0f\x08|\xe9\x03\x1f\x11\x10\
+8\xb8\xe1\xc34\x0a\x00\xa3\xaf\xe5\xdf\x13\xf4\xb7\xad&\
+\xfe\x17Q\x06\xfd\xf53*\x12\xf4\x070\x1e\x85\xbb\xed\
+\x1b\x0eOmk\x03&\xeb@@\xe0y\xf4sU`\
+\x11\x11\xf1\x85/\xbdV\xbc\xf3\xa5\xef\x8b\x7f\xf9\xea\x7f\
+\xf0\xc6(\x00\xe4\xeb\xc5\xc7\xfc\xe2\x1f\x08\xfa\xdb\xad\xfa\
+/\xab/i/\x04\xfd\x01\x8c\xad\x07L6\xb37\x1d\
+;\xb8J\x11\x98\xb8]@\xe0\xfb\xfe\xfc\xbd\x01\x81\xab\
+(\xc3d;\xdf\x11u{w\x97~\xf0G\x7fB@\
+\xa0\x02\x80\x02\xc0=A\x7fO\xe2\xe9v\xffM\x1f\xaf\
+A\xd0\x1f\xc0\xa8m\xfa\x18\xbcMO\xb1\x8e\xd4\xfd9\
+X\x80S\xfb\x96?\xfaG\xe23\xaf>\x18\x10\xb8\x89\
+r\xa5\xbe\xf3#\x01\x11\x02\x02\x15\x00f\x5c\x00x \
+\xe8\xef2\xca*\xdc\xb2\xcf\xf7E\xd0\x1f\xc0\xf8g\xb3\
+\x9a`\xb6c \x80\xc3\x9d\xc4\xe3\x01\x81\xeb\xe8\xe9\xaa\
+\xc0\x08\x01\x81:\xbf\x19\x0e~\xee\x09\xfa\xbb\x8d\xb2\xea\
+\xb6\x8e\x9e\xce\xfa\x0b\xfa\x03\x98\x90$\xd5\xbea\xc3-\
+\xa2Hw\xda\x01\x98\x8bG\x02\x02\x8b\xbd\x22\x80\x80@\
+\x05\x00r\xb9'\xe8\xef&\xca/\xde*z,b\x08\
+\xfa\x03\x98\x90\x22\xd6\x11\xb6\xb37h\xb8\x8b\x88\xc5\xad\
+v\x00\xe6\xe4@@\xe0:\xfa\xb9*p\x8e\x01\x81\x83\
+)\xd5+\x00\xf4\xe0\x9e\xa0\xbf\xeb\xeagU\xfd\xf4F\
+\xd0\x1f\xc0\x04K\x00\x0e\x01\x8c}<\x06\xd0\xabG\x02\
+\x02\xd7\x11q\x16\x1d\xef\x04\xd8\x11\x10\xa8\x000\xb9\x1e\
+\xfc\x9e\xa0\xbf\xddjCo\x13\x7fA\x7f\x00\xe6\xb1\xdc\
+k\x19\xa9\x9fA.\xc0\xd0<\x12\x10xQ\xcdUn\
+\xa2\xcc(\xeb\xae\xfb\x9aO@\xa0\x1d\x00S\x1f\xf6<\
+\x17\xf4WDy\xcf\xe6U\x94\xe7kz]\xf5\x17\xf4\
+\x070y\x17\x91\xc2v\xf6\xfa#\x883\xd7\x01\x02s\
+v  p\xb97\x87\xe9\xdc~@\xe0v+ P\
+\x01`D\x1e\x08\xfaK\xd1S\xc8_\x84\xa0?\x80y\
+\x8d\xe0\xe2,\x22\x9eh\x88FE\x00\x05\x00`\xf6\x1e\
+\x09\x08\xdc]\x15\xd8y\x11`? \xf0\xc5\xf7O.\
+ \xd0\x0e\x80\xa9z.\xe8\xef.\xca\xad3\x17QV\
+\xd0z#\xe8\x0f`~3Y\x1a(b\x13).5\
+\x040w\x8f\x04\x04\xae\xaa\xf9L\x1fW\x05\xce1 \
+P\x01`\x8c\xf6\x83\xfe.\xaf\xae#\x9eM\xf8\xef\x95\
+\xa0?\x809Nd\x17\x8b\xb0\x0b\xc0x\x08\xa0\xa5\x07\
+\x02\x02\xcf\xa2\xa7\xab\x02w&\x16\x10h\x07\xc0\x94<\
+\x17\xf4\xb7\xad\xbe\x18\xcb(+e\xfd\x8c\xfb\x04\xfd\x01\
+\xcc\x5cZF\x8a\x1b\xed\xd0t`V8p\x0aPy\
+S@\xe0\xd3\x84\xc0u5\xdf\xe9\xe5H@\xc4,\x02\
+\x02\x15\x00\x9a\xcc\x7fO2Z\xd8\x0b\xfa\xfb\xfd?\xf8\
+\xc6n\xcb\xff6N\xb0\xea/\xe8\x0f\x80X\x14.\x04\
+l6\x8aXGJn\x03\x00\xd8\x7f4\xee\x07\x04\xbe\
+\xf5\x99\x80\xc0MD\x9cG\xf4w\x8b\xcaD\x02\x02\x07\
+\xb1\x0b`\x0a3\xc5\x93\x0cv\x9e\x0f\xfa\xab\xbe\x00\xe7\
+\xd5O_\xbf\xb8\xa0?\x00\x9e\xdanC\xaa}\xd3N\
+5)\x9e\x00\xdc\xe3\x81\x80\xc0\xf3(\x17=\xaf\xa3\xe3\
+\xab\x02#&\x11\x10XD\xf7\xf9\x09\xb3)\x00D\xf4\
+\x5cMy.\xe8o\x1b':\xeb/\xe8\x0f\x80g\x87\
+\x17\xc5:R?\xd75MN*\x16Q\x14\xaeR\x04\
+\xb8\xc7\x81\x80\xc0\xbb\xe8g7\xc0\x98\x03\x02\x17\x0a\x00\
+#tyu\x1d?\xfc\xb7\xff\xc1.\xe8\xaf\x88\xf2\xac\
+\xff\xe2\x14\xed(\xe8\x0f\x80\xc7\x06H\xd4n\xb5el\
+\xb7B\x14\x01\x1e\xf1@@\xe0\xba\xfa\xcf\xde\x0a\xd0#\
+\x0c\x08\x5c\x84#\x00\xd9\xa4>\x06;\xbb\xa0\xbf_\xfa\
+\xe5_\x8d\xbd7\xaf\xd7\xab\xfd\x04\xfd\x01pD\xb7\xe8\
+\x08@\x8b*\x00\x00\x8f{  p\x1dOo\x09\xe8\
+\xbc\x1f\x1aa@\xe0`:\x18!\x80\x87?\x5cU\xd0\
+\xdfGvA\x7f\xb7\xa7z\x03\x05\xfd\x01pD\x97\xb8\
+\x89p\xaf}C\xcb\x08G(\x00\x0e\xf64\xf7\x07\x04\
+.\xa2\xe7\xab\x02#F\x15\x108\x88\x22\x80\x1d\x00\x8f\
+x6\xe8\xef\x8d\x15\x95\x8b\x9e?%\x82\xfe\x00\xa8\xd9\
+3\x0a\xb4k\xd8\xe9\xaa\xae\x03\xd4\xf0@@\xe0*z\
+\xba*\xb0\xec\xf2F\x13\x10\xe8\x08@\xbe9r\xfe\x02\
+\xc0\xab\x9f\xfeL\xbc\xed=\xdf\xbb\x0b\xfa{\x12'\xaa\
+\xd8\xac7\xab\xf8\xb5O\x0a\xfa\x03\xa0N\xcfX8\x06\
+0\xf2\x01\x1a\xc0X<\x10\x10\xb8\xa9\xe6\x9a7=\xce\
+\x09\x87\x1e\x10h\x07\xc0\x10\x0b\x00\xfbA\x7fW\xd7o\
+|^\xcfN\xf1\x8b\xbd\xfc\x1d\xefN_\xfd\xec\xaf\x16\
+\x1f|\xbf\xa0?\x00\xea\xf4\x8ci\x19\xa9\xb7A\xd7\xd4\
+l\x22\x92#\x14\x005\xdd\x13\x10x\x11\xe5\x91\x80\xeb\
+(\x17T{1\xe0\x80@\x05\x80\x8c\xbfC\x96\xdf\xe3\
+\xf3_\xfcr|\xdb\x9f\xfb\x9e]\xd0\xdf\xf6\x14o\x92\
+\xa0?\x00ZK\xc5YD\xdaj\x88\xa6\xed'h\x07\
+\xa0\x89\x07\x02\x02WQ\xe6\xa8\xf5\x92\x0b0\xc2\x80@\
+\x05\x80\x9a\xce2|H\xe2\x1f\x7f\xe2\x9f\xc7\x8b\xef\xff\
+H\xfc\xcfo\xfe\xef\xe2\x94m#\xe8\x0f\x00Nm\x1b\
+Q\x14\x0a(\x00\x0d<\x10\x10\xb8;\xcb\xdck\xd0\xea\
+. \xb0\xcct;\xf9c\xdd\x0e\x80!\xfc\x0e\xbb\xa0\
+\xbf\xbf\xf7S\x9f\x88\x94NsuRQ\x94\xe7\x0d\xff\
+\xda\x0f\x08\xfa\x03 [\xe7r\x16\x8b\xb8\xd3\x10\x8d\xda\
+n\x15\xdb\xed\xb5\x86\x00h\xee\x9e\x80\xc0e<\xbd%\
+\xa0\x17\xbb\x80\xc0\x8f\xff\xfc\xa7\xe2\xc5\xbf4\xe8\x80@\
+\x05\x80:\xddt\x94\xdb\xf5k{\xb5\xda\x16R\x05\xfd\
+\xdd\xc5\xa9\x82\xfe\xd6e\xd0\xdf'\x7fN\xd0\x1f\x00\xd9\
+\x5c\xc46n5C\xe3\x22\x80\x9b\x14\x00\xda\xces\xde\
+\x1c\x10\xb8\xbb*\xf0:\xfa\xbb*\xb0\x88\x88\xed\x17\xfe\
+\xebk\xc5;_\x1el@\xa0\x02@M\xb5V\xee/\
+\xaf\xae\xe3o\xfc\x9d\x9f\x8a\xef\xff\xe8\xc7\xe2\xfa\xfa\x8d\
+\xcf\xddI\x06I\x82\xfe\x00\xe8x\xd0C\xb3\x96;;\
+\xd5\xd8\x00`j\xee\x09\x08\x5cF\x8fW\x05F\xb9\xeb\
+\xe0\xfa\xf6v\xb0\x01\x81\x0a\x00]\x15\x00>\xff\xc5/\
+\xc7;^\xfc\xcb\xe9\x17\xff\xc5\xbf+\xff\xc1$\xe8\x0f\
+\x80I\x17\x00\x5ck\xd7ldq\x11)=\xd1\x10\x00\
+y\xdc\x13\x10\xb8\x89\x88\xf3\xe8g'@\x8a\x88$ \
+pF\x05\x80\x94R|\xfc\xe7?\x15/}\xe0\x87\xe2\
+k_\xff\xc6I_\xac\xa0?\x00z\xb2\x8a\x94\xae4\
+CC\x85\xe2\x09@\xd6\xc7\xea\x9b\x03\x02\xcf\xa3\xbc%\
+\xe0&\xba\xbf*p\x19{;\x0ev\x01\x81?\xfe\xd3\
+\xaf\x0c! P\x01\xa0\xa6G\xdf\xb1\xaf}\xfd\x9b\xf1\
+\x9d\x1f\xfc\x91T\xa5?\xa6\x93\xac\xfaWE\x8a\x0f\x7f\
+H\xd0\x1f\x00=\x8f\xb6h\xdav\xabH\xa1\x80\x02\x90\
+\xd9=\x01\x81\x17U\x01\xa0\xcbg\xee3\xd7\xc7\xef\x02\
+\x02\x7f\xe6g\xffY\xbc\xf8\xfe\xf9\x04\x04N~\xf9\xf9\
+\xd5O\x7f&\xde\xfe\xde\x0f\xa6\xdf\xfa\x9d/\x16O\xe7\
+\xe2\xfd[o\xca\xa0\xbfO\xbd\x22\xe8\x0f\x80>%\xab\
+\xd8\x8d\x9b.\x16R\x14\x00:\x9a\x1f\xbd9 p\x19\
+e!\xa0\xcb#\x01\xdbxv\xf1\xb8\x88\x88\xf8\xc2\x97\
+^+\xde\xf9\xf2\xf7\xa59\x04\x04N\xb6\x00\xf04\xe8\
+\xef\xc7\xe2\xea\xfa\xb47\xf9\x08\xfa\x03\xe0t\x8aMD\
+\x5cj\x87\xc6\xed\xa7\x80\x02\xd0\xa1\xe7\x02\x02\xcf\xa2\xdb\
+\xab\x02\xd7\xf1@\x81\xe1\xf6\xf6.~\xf0G\x7f\x22>\
+\xf4\xc3\xd3\x0e\x08\x9cJ\x01\xe0\x99\xfa\xbc\xa0?\x00\xe7\
+B\x01a\x00\x00\x0a\xa9IDAT\xd8\x97\xacc7\
+o\xbbM\xa4\xa4\x80\x02\xd0\xa1\xe7\x03\x02\xab\x22\xc0]\
+G\x85\x80{\xfb\xc47\x02\x02\x7f}\xda\x01\x81\x93\xda\
+\x01 \xe8\x0f\x00\xee\x9d\xff[\xc5n7V\xd4\x91\x03\
+t\xfd\xa4\xdd\x0b\x08|\xfb\xb7\xbd\x11\x10x\x1e\xf9s\
+\x01\x0e\x1e3\xd8\x05\x04\xfe\xfd\x9f~%R\xde\x93t\
+'/\xc8\x9f\xfa\x05|.\x22\xde\x13\xed\x0b\x117\x11\
+\xb1\xfc\xd3\x7f\xeam\xf1\xdaW~/\xa2\x0c\xdc\xab\xfb\
+\xbb]F\xc4\xa6ec\xa6\x14Q|\xf8C\xdf\x1d\xbf\
+\xf0\xf1\x1fw\xd6\x1f\xa0;\xad\x9f\xd9\xf3*\x00\xa4\x14\
+Eq\x13e\xd22\xb5\xdb/\xae\xa3\x88\xf3(\xb7\xa6\
+\xfa\x0c\x02t\xec\xea\xfa&>\xf6\x93?\x1b\x9f\xf8\xc5\
+_\xd9\xfdO\xb7\xd5\xc4=\xd7\xb8\xe1*\xca\xe3\x00\x8f\
+?\xfd#\x8aw\xbe\xedO\xa4\xaf\xfe\xde\xff\xc81o\
+\xbe\xab\xfa\x91\xdf\x8d\x88\x97\x14\x00\xda\xb9\xce0\xa8i\
+\xdd\x91o6\xab\xf4+\xbf\xf03\xce\xfa\x03(\x00\x0c\
+q\x12{\x15E\xa8L\xe7\xfb\xcc\xf9\x0c\x02t\xec?\
+\xfe\xe7\xcf\xc6\xf7\x7f\xf4c\xe9\xff\xfc\xdf\xffW\xc4\xd3\
+\xf0\xbe&s\xc7!<\xc3o\xa3\xdc\xd1p\xd2\x02\xc0\
+\x94\xae\x01|>\xd1\xb1W\x82\xfe\x00`\xca\xe4(\x00\
+\xf4\xed\xb9\x80\xc0E\x94\x0b\xd89\x12\xde\xeb\x06\xe4\xa6\
+(\xaf)\x1c\xbd)\x9di\xbb\x89\xb2\xaa\xd2\x1bA\x7f\
+\x00\x8cF\x11g\x91\xd2\x13\x0d\xd1\xd8y\xa4\xceR\xa9\
+\x01x\xc0=\x01\x81\xabL\xf3\xbe:s\xe1\xeb\x0c\x05\
+\x80A\xe4\xf1L\xa9\x00\xb0k\xd0\xbb\xbe\xfe\x85\x82\xfe\
+\x00\x18\x91\x8b*\x07\x80F\x8a\xf3(N\xb7\xd3\x10`\
+\xd6O\xe0\xbd\x80\xc0\xb7\xbd\xf5[S\x94y\x00m'\
+\xd4E\x8dB\xc2.cn\xf4\xb7\xc2Lm\xd6\xba\x8a\
+\x8e\x8f\x01\x14\xd5\x07\xed\xc3\x1f\xfa\xee\xf8\xef\xbf\xfdj\
+\xf1g\xff\xcc\xbb|#\x01\x18\xcd\x18J\x13\xb4j=\
+\xb7)\x00\x9c\xd0\xb7\xbf\xeb\x1d\xf1\xe5\xdf\xfc7\xc5\xdf\
+\xfa\x91\xbf\xb2\xdf\xa75]\x00^F\xbdU\xfd\x8b\x96\
+\xf3\xe7b\x08\xfd\xf0\x14\x97\xadSDw[\xf4\xd6\x9b\
+U\xfc\xda'\xffI|\xea\x95\x9f\x94\xf2\x0f\xc0\xf8\xa6\
+\xffEa\x15\xbb\xf9\x08c\x1d\x13X\xfd\x01\x18\xb3\xf5\
+j\x19\xff\xf4\x1f\xfeX\xfc\xc6\xbf~%\xfe\xf0[\xfe\
+\xd0\xee\xba\xc0\xa6\xdb\xf3\xeb\x16vW\xd1\xfcZ\xc2A\
+\x14\xe1\xa7R\x00(\x9e{S:!\xe8\x0f\x80\xd1O\
+`S\xba\xd6\x10-\xc6\x1b\x850@\x80!x. \
+\xf0,\x9a\x1d\x09hZ\xd8m\xb2\xe0|\xa6\x00\xd0\xad\
+\xab\x1c\x7f\x88\xa0?\x00\xa65\x85-L`\xdb\xd8\x16\
+\x11\xe1(\x00\xc0\x10\xec\x02\x02\x7f\xee\x1f\xfd\xdd8;\
+[\xec\xfa\xb7:\xcf\xe8\xa2\xc1\x9cx\xdd\xb0\x1f\xb0\x03\
+\xa0C\xcb\x5c\x0d,\xe8\x0f\x80iM`\x93\xc9k\x1b\
+E\xac#\xd3\x22\x03\x00\x19\x1e\xcbE\x11\x7f\xf3\xaf\xff\
+@|\xe9?\xfd\xab\xf8\x93o\xfd\xe3\xbb\xb0\xbe\xbaG\
+\x02\xea\x1e\x8f\xbb\x18k_0\x95\x19m\xba\xe7w9\
+\x8f\x86\xe7\xf4\x04\xfd\x010\xe1\x09\xec&\x8ap\x1d`\
+\xdb\xf1Sr\x14\x00`H\xbe\xfd]\xef\x88\xd7~\xf3\
+\xdf\xee\x02\x02\xeb\x1c\x09XE\xfd-\xfd\x8b\x86\x85\x03\
+\x05\x80\xacC\x9ag\x9d5\xfd\xfd\x04\xfd\x010i\xc9\
+m\x00\xad\xdb\xaf(.4\x04\xc0\xb0\xec\x07\x04\xf60\
+\x8f[G\x8fW\xd0w5i\xee\xdb\xe7\x22\xe2=\xd1\
+\xbe\x10\xf1z\x94\xdb0\x9e\xef\x8c\xb7\x11q\x1d\x11\x9b\
+\xa3\xba\xf3\x88\xe2[\xff\xd8\xb7\xc4\xf7\xfc\xc5\xef4\xf1\
+\x07\x18\xb0\xedv\xfbd\xb1X\x9ci\x89\x86\xf3\xd7\x94\
+\xb6EQ8\xd7\xd6\xb2\x0a\xe0VE\x80\xe1z\xfd\xf2\
+*\xfe\xfdo\xfc\x97\xf8\xfd?\xf8\xc61\x0f\xed'\xd5\
+d\xfe\xa1@\xf9\xcb\x07\xe6\x947\xd5\x9c\xb3\xce\xe4\xf1\
+w\x22\xe2%\x05\x80v.\xab\xc9\xff\xf9=\xff\xdfU\
+\xcd7\x04\x00\x00\x80\x89(\x8a\x22\xa5\xc3G\xb7\xae\x1b\
+\x14\x00\x0e\xfds\x83+\x00\x9cO\xe5=\x8d\x87\x8b\x19\
+\xeb#\x8b\x00\x8f\xbd\xa9\xa7\xf6\xa4\xfa)\xf6\xfezw\
+\xa6%\xed\xb5A\xba\xa7-\x8a{\xfe\x9em<{n\
+\xe5\xbe\xff\xbe\xcbU(\xe2\xd9\xb3-i\xef\xdf\xf3\xfc\
+\x9f\xbb\xd8\xfb\xe7\xcfb W]\x00\x00\x00\xf3\x95R\
+\xba:b\xae\xd74$w\x15#Zt\x9eJ\x01\xe0\
+\x98\x1d\x04c\xde\xab\xf7\xfcdz\x8c\xe7\x0e\xf7\x8b\x18\
+u\x0a\x18\xf7\xbd\x7f\x8f\x15-\x8a\xbd?+U\xedv\
+L\x01c\xf7\xff\xed\x171.\xc2\xfeN\x00\x00\x98\x83\
+u\xb4[\x14\xbe\x89\xf26:\x05\x80\x9e&\xc8\x87\xde\
+LG\x01N\xff\x1e\x9d\xedM\xac\xc7\xe6\x98\x02\xc6\xee\
+\xaf\xef+b\xdcW\xc08\xb4#cW\x90H\xcf\xfd\
+9q\xcf_\xdb\x85\x01\x00\x00\xed4=\x9a\xbe\x8e\xf2\
+(\xc0\xe0Mi\x07\xc01W0lcZ7\x1f\xd0\
+\x9f)\x150v\x7f\xdd\xc71\x92\xe2\x9e\xef\xe7\xb1\xc7\
+H\x22FPE\x05\x00`R\x05\x80\xdb\x86\xe3\xfd\xb3\
+\x18\xc1\xa2\xf3\x942\x00\x0e\xd9UeV>\xd7\xcc\x90\
+c$\x87\x8f\x91\xec\x1f\x1dY\x84c$\x00\x00ss\
+QM\xe2\x9b\x8c\x95\xcf\xa3\xbcI`\xd0G\xcf\xcfg\
+\xf8\xa6\xde\xcd\xf4\xf7\x86\xb1\x9b\xea1\x92\xe7u}\x8c\
+d\xf7\xbf\x0b\xf3\x04\x00\xb8\x7f,\xd6\xd4\xe0\x17\x9d\xa7\
+4\x11>\xa6\xca\xb2\x8a2\x9c\x01\xa0os>F\xb2\
+\x7f\x0c\xc41\x12\x00`\xc86\xd1\xfe\x86\xb8\xc1\x1e\x05\
+\x98\xe3Jx\x8a\x91$4\x02\x0c\x88c$\x8e\x91\x00\
+\xc0\x5c\xb4\xc9\x8d[\xc5\x80\x03\x01\xe7X\x00\xb0\x0b\x00\
+`\x9e\x1c#q\x8c\x04\x00\xea\xf4\xbbM\xfb\xb0e\x0c\
+t\x17\xc0\x5c\xcf\xc2\x17\xe1Z@\x00\xc6\xc51\x92g\
+\xff\x1e\xc7H\x00\xe8\xca\xaa\x9a/6-\x00\xec\xfa\xb0\
+\xc1\xe5\xcf\xcd\xb5\x00p\x11\xc7]\x1b\x08\x00\xe4\xe1\x18\
+\x89c$\x00s\xb2\x0b\x04T\x00\x18\xd0\xef\xde6\xdc\
+\x01\x00\x98\x0f\xc7H\x1c#\x01\xe6#\xc76\xfe\xc5=\
+s\xce\x93\x16e\xe7\x5c\x008\x8bv\xe1\x0e\x00\x00c\
+\x1b\xfb8F\xe2\x18\x09p\xfc\xe4\xbd\xedd\xfd\xa2z\
+V\xed?;N:\x07?\x9f\xf9\x9bz\x11v\x01\x00\
+\x00\x8c\x81c$\x8e\x91@\xdf\xb6\xf1\xf0n\xa9c\xed\
+\x8e\x02\xac\x860\x07\x9fR\x01\xa0\xc9\x1b\x93\xa3\xaa\x03\
+\x00\x00\xc7p\x8c\xc41\x12\xc6e\x13\xe5\x82q\x8e\xb9\
+\xeau\x94;\x82\x14\x00Nl\x9d\xe9M\x05\x00\x80)\
+s\x8c\xe4\xd9\xbf\xc71\x92y\xb8\xaf\x00\xd5d\xcey\
+\xbd\xf7=\x9au\x01\xa0\x18\xc8\x9b*\x0f\x00\x00\x00\xa6\
+k*\xc7Hv\x85\x84\xfd\xed\xe9C>Fr>\x80\
+9_\x9b\x7f\x7f\xae\xb9\xe2\xee8\xcd\xac\x0b\x00\xff-\
+\x22^\xcc\xf8\x85nj\xe5y\x08\x00\x00\x0c\x9c#\x0d\
+\xcd\xb4I\xf2\xcfU(\xda\x15\x11\xbe>\xe7\x02\xc0G\
+#\xe2K-\xdf\x10\x00\x00\x00\x18\xbamD|Z3\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x1c\xf0\xff\x01\
+\xf5tm\xa3\x8e]\x9cb\x00\x00\x00\x00IEND\
+\xaeB`\x82\
+"
+
+qt_resource_name = b"\
+\x00\x04\
+\x00\x06\xfa^\
+\x00i\
+\x00c\x00o\x00n\
+\x00\x11\
+\x04+@\xc7\
+\x00e\
+\x00n\x00v\x00e\x00l\x00o\x00p\x00e\x00_\x001\x000\x002\x004\x00.\x00p\x00n\x00g\
+\
+"
+
+qt_resource_struct = b"\
+\x00\x00\x00\x00\x00\x02\x00\x00\x00\x01\x00\x00\x00\x01\
+\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x02\x00\x00\x00\x01\x00\x00\x00\x02\
+\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x0e\x00\x00\x00\x00\x00\x01\x00\x00\x00\x00\
+\x00\x00\x01\x81Z\x1e\x12E\
+"
+
+def qInitResources():
+    QtCore.qRegisterResourceData(0x03, qt_resource_struct, qt_resource_name, qt_resource_data)
+
+def qCleanupResources():
+    QtCore.qUnregisterResourceData(0x03, qt_resource_struct, qt_resource_name, qt_resource_data)
+
+qInitResources()
```

### Comparing `msg_explorer-1.6.0/msg_explorer/attachments_browser.py` & `msg_explorer-1.7.0/msg_explorer/attachments_browser.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,90 +1,90 @@
-# This Python file uses the following encoding: utf-8
-import logging
-
-import extract_msg
-
-from PySide6 import QtCore
-from PySide6 import QtWidgets
-from PySide6.QtCore import Signal, SIGNAL, Slot, SLOT
-from PySide6.QtWidgets import QTableWidgetItem
-
-from .ui.ui_attachments_browser import Ui_AttachmentsBrowser
-
-
-logger = logging.getLogger(__name__)
-logger.addHandler(logging.NullHandler())
-
-
-class AttachmentsBrowser(QtWidgets.QWidget):
-    # Signals that an attachment was double clicked.
-    attachmentSelected = Signal(int)
-    signedAttachmentSelected = Signal(int)
-    def __init__(self, parent = None):
-        super().__init__(parent)
-
-        self.ui = Ui_AttachmentsBrowser()
-        self.ui.setupUi(self)
-
-        self.ui.tableAttachments.cellDoubleClicked.connect(self._cellDoubleClicked)
-        self.__isSigned = False
-
-    @Slot()
-    def msgClosed(self):
-        self.ui.tableAttachments.clearContents()
-        self.ui.tableAttachments.setRowCount(0)
-
-    @Slot(extract_msg.msg.MSGFile)
-    def msgOpened(self, msgFile):
-        self.__isSigned = isinstance(msgFile, extract_msg.MessageSignedBase)
-        totalAttachments = len(msgFile.attachments)
-        if self.__isSigned:
-            totalAttachments += len(msgFile._rawAttachments)
-        self.ui.tableAttachments.setRowCount(totalAttachments)
-        indexPostfix = ' (Regular)' if self.__isSigned else ''
-        count = 0
-        self.ui.tableAttachments.setSortingEnabled(False)
-        for index, att in enumerate(msgFile._rawAttachments if self.__isSigned else msgFile.attachments):
-            self.ui.tableAttachments.setItem(index, 0, QTableWidgetItem(str(index) + indexPostfix))
-            if isinstance(att, extract_msg.Attachment):
-                self.ui.tableAttachments.setItem(index, 1, QTableWidgetItem("OK"))
-            elif isinstance(att, extract_msg.attachment.BrokenAttachment):
-                self.ui.tableAttachments.setItem(index, 1, QTableWidgetItem("Broken"))
-            elif isinstance(att, extract_msg.attachment.UnsupportedAttachment):
-                self.ui.tableAttachments.setItem(index, 1, QTableWidgetItem("Unsupported"))
-            else:
-                self.ui.tableAttachments.setItem(index, 1, QTableWidgetItem("Unknown Type"))
-            self.ui.tableAttachments.setItem(index, 2, QTableWidgetItem(att.shortFilename))
-            self.ui.tableAttachments.setItem(index, 3, QTableWidgetItem(att.longFilename))
-            self.ui.tableAttachments.setItem(index, 4, QTableWidgetItem(att.cid))
-            self.ui.tableAttachments.setItem(index, 5, QTableWidgetItem(att.mimetype))
-            self.ui.tableAttachments.setItem(index, 6, QTableWidgetItem("Not Rendered" if att.renderingPosition and att.renderingPosition == 0xFFFFFFFF else str(att.renderingPosition)))
-            count += 1
-        if self.__isSigned:
-            # If it's signed, also display the regular attachments.
-            for index, att in enumerate(msgFile.attachments):
-                self.ui.tableAttachments.setItem(count + index, 0, QTableWidgetItem(str(index)))
-                self.ui.tableAttachments.setItem(count + index, 1, QTableWidgetItem("OK (Signed)"))
-                self.ui.tableAttachments.setItem(count + index, 2, QTableWidgetItem(att.name))
-                self.ui.tableAttachments.setItem(count + index, 3, QTableWidgetItem(att.name))
-                self.ui.tableAttachments.setItem(count + index, 5, QTableWidgetItem(att.mimetype))
-
-        self.ui.tableAttachments.setSortingEnabled(True)
-
-    @Slot(int, int)
-    def _cellDoubleClicked(self, row : int, column : int):
-        """
-        Handle a cell being double clicked to emit the attachmentSelected signal.
-        """
-        if row < self.ui.tableAttachments.rowCount():
-            data = self.ui.tableAttachments.item(row, 0).data(0)
-            if self.__isSigned:
-                if data.endswith(')'):
-                    # Regular attachment.
-                    self.attachmentSelected.emit(data.split(' ')[0])
-                else:
-                    # Signed attachment.
-                    self.signedAttachmentSelected.emit(int(data))
-            else:
-                self.attachmentSelected.emit(int(data))
-        else:
-            logger.warn(f'Received index on cell double click that was outside of table (row: {row}, colunn {column}).')
+# This Python file uses the following encoding: utf-8
+import logging
+
+import extract_msg
+
+from PySide6 import QtCore
+from PySide6 import QtWidgets
+from PySide6.QtCore import Signal, SIGNAL, Slot, SLOT
+from PySide6.QtWidgets import QTableWidgetItem
+
+from .ui.ui_attachments_browser import Ui_AttachmentsBrowser
+
+
+logger = logging.getLogger(__name__)
+logger.addHandler(logging.NullHandler())
+
+
+class AttachmentsBrowser(QtWidgets.QWidget):
+    # Signals that an attachment was double clicked.
+    attachmentSelected = Signal(int)
+    signedAttachmentSelected = Signal(int)
+    def __init__(self, parent = None):
+        super().__init__(parent)
+
+        self.ui = Ui_AttachmentsBrowser()
+        self.ui.setupUi(self)
+
+        self.ui.tableAttachments.cellDoubleClicked.connect(self._cellDoubleClicked)
+        self.__isSigned = False
+
+    @Slot()
+    def msgClosed(self):
+        self.ui.tableAttachments.clearContents()
+        self.ui.tableAttachments.setRowCount(0)
+
+    @Slot(extract_msg.msg.MSGFile)
+    def msgOpened(self, msgFile):
+        self.__isSigned = isinstance(msgFile, extract_msg.MessageSignedBase)
+        totalAttachments = len(msgFile.attachments)
+        if self.__isSigned:
+            totalAttachments += len(msgFile._rawAttachments)
+        self.ui.tableAttachments.setRowCount(totalAttachments)
+        indexPostfix = ' (Regular)' if self.__isSigned else ''
+        count = 0
+        self.ui.tableAttachments.setSortingEnabled(False)
+        for index, att in enumerate(msgFile._rawAttachments if self.__isSigned else msgFile.attachments):
+            self.ui.tableAttachments.setItem(index, 0, QTableWidgetItem(str(index) + indexPostfix))
+            if isinstance(att, extract_msg.Attachment):
+                self.ui.tableAttachments.setItem(index, 1, QTableWidgetItem("OK"))
+            elif isinstance(att, extract_msg.attachment.BrokenAttachment):
+                self.ui.tableAttachments.setItem(index, 1, QTableWidgetItem("Broken"))
+            elif isinstance(att, extract_msg.attachment.UnsupportedAttachment):
+                self.ui.tableAttachments.setItem(index, 1, QTableWidgetItem("Unsupported"))
+            else:
+                self.ui.tableAttachments.setItem(index, 1, QTableWidgetItem("Unknown Type"))
+            self.ui.tableAttachments.setItem(index, 2, QTableWidgetItem(att.shortFilename))
+            self.ui.tableAttachments.setItem(index, 3, QTableWidgetItem(att.longFilename))
+            self.ui.tableAttachments.setItem(index, 4, QTableWidgetItem(att.cid))
+            self.ui.tableAttachments.setItem(index, 5, QTableWidgetItem(att.mimetype))
+            self.ui.tableAttachments.setItem(index, 6, QTableWidgetItem("Not Rendered" if att.renderingPosition and att.renderingPosition == 0xFFFFFFFF else str(att.renderingPosition)))
+            count += 1
+        if self.__isSigned:
+            # If it's signed, also display the regular attachments.
+            for index, att in enumerate(msgFile.attachments):
+                self.ui.tableAttachments.setItem(count + index, 0, QTableWidgetItem(str(index)))
+                self.ui.tableAttachments.setItem(count + index, 1, QTableWidgetItem("OK (Signed)"))
+                self.ui.tableAttachments.setItem(count + index, 2, QTableWidgetItem(att.name))
+                self.ui.tableAttachments.setItem(count + index, 3, QTableWidgetItem(att.name))
+                self.ui.tableAttachments.setItem(count + index, 5, QTableWidgetItem(att.mimetype))
+
+        self.ui.tableAttachments.setSortingEnabled(True)
+
+    @Slot(int, int)
+    def _cellDoubleClicked(self, row : int, column : int):
+        """
+        Handle a cell being double clicked to emit the attachmentSelected signal.
+        """
+        if row < self.ui.tableAttachments.rowCount():
+            data = self.ui.tableAttachments.item(row, 0).data(0)
+            if self.__isSigned:
+                if data.endswith(')'):
+                    # Regular attachment.
+                    self.attachmentSelected.emit(data.split(' ')[0])
+                else:
+                    # Signed attachment.
+                    self.signedAttachmentSelected.emit(int(data))
+            else:
+                self.attachmentSelected.emit(int(data))
+        else:
+            logger.warn(f'Received index on cell double click that was outside of table (row: {row}, colunn {column}).')
```

### Comparing `msg_explorer-1.6.0/msg_explorer/constants.py` & `msg_explorer-1.7.0/msg_explorer/constants.py`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-import re
-import string
-
-
-# This expression will match any non-ascii character.
-RE_SPECIAL_CHAR = re.compile(f'[^{string.printable}]|[\t\n\r\x0B\x0C]')
-
-# This expression will match any standard file name in an MSG file.
-# For files that are inside of custom attachment types, this will
-# not match.
-RE_STANDARD_FILE = re.compile(r'^(__properties_version1\.0)|(__substg1\.0_[0-9a-fA-F]{8}(\-[0-9a-fA-F]{8})?)$')
-
-# This expression will match any standard folder name in an MSG file.
-RE_STANDARD_FOLDER = re.compile(r'^(__attach_version1\.0_#[0-9a-fA-F]{8})|(__nameid_version1\.0)|(__recip_version1\.0_#[0-9a-fA-F]{8})$')
+import re
+import string
+
+
+# This expression will match any non-ascii character.
+RE_SPECIAL_CHAR = re.compile(f'[^{string.printable}]|[\t\n\r\x0B\x0C]')
+
+# This expression will match any standard file name in an MSG file.
+# For files that are inside of custom attachment types, this will
+# not match.
+RE_STANDARD_FILE = re.compile(r'^(__properties_version1\.0)|(__substg1\.0_[0-9a-fA-F]{8}(\-[0-9a-fA-F]{8})?)$')
+
+# This expression will match any standard folder name in an MSG file.
+RE_STANDARD_FOLDER = re.compile(r'^(__attach_version1\.0_#[0-9a-fA-F]{8})|(__nameid_version1\.0)|(__recip_version1\.0_#[0-9a-fA-F]{8})$')
```

### Comparing `msg_explorer-1.6.0/msg_explorer/font_handler.py` & `msg_explorer-1.7.0/msg_explorer/font_handler.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,54 +1,54 @@
-from PySide6.QtCore import QObject, Slot
-
-
-class _FontHandler(QObject):
-    """
-    Helper class to help with fonts so they can be globally increased
-    or decreased.
-    """
-    def __init__(self):
-        self.__fonts = []
-
-    @Slot()
-    def clearFonts():
-        """
-        Removes all fonts from the handler.
-        """
-        self.__fonts.clear()
-
-    def registerFont(self, getter, setter):
-        """
-        Adds a font getter and setter function for the font to handle.
-        """
-        self.__fonts.append((getter, setter))
-
-    @Slot()
-    def increaseFonts(self, amount = 1):
-        """
-        Increases the fonts by the specified amount (default: 1).
-        """
-        for font in self.__fonts:
-            newFont = font[0]()
-            newFont.setPointSize(newFont.pointSize() + amount)
-            font[1](newFont)
-
-    @Slot()
-    def decreaseFonts(self, amount = 1):
-        """
-        Decreases the fonts by the specified amount (default: 1).
-        """
-        for font in self.__fonts:
-            newFont = font[0]()
-            newFont.setPointSize(newFont.pointSize() - amount)
-            font[1](newFont)
-
-
-
-_fontHandler = _FontHandler()
-
-
-def getFontHandler():
-    """
-    Gets the instance of the singleton FontHandler.
-    """
-    return _fontHandler
+from PySide6.QtCore import QObject, Slot
+
+
+class _FontHandler(QObject):
+    """
+    Helper class to help with fonts so they can be globally increased
+    or decreased.
+    """
+    def __init__(self):
+        self.__fonts = []
+
+    @Slot()
+    def clearFonts(self):
+        """
+        Removes all fonts from the handler.
+        """
+        self.__fonts.clear()
+
+    def registerFont(self, getter, setter):
+        """
+        Adds a font getter and setter function for the font to handle.
+        """
+        self.__fonts.append((getter, setter))
+
+    @Slot()
+    def increaseFonts(self, amount = 1):
+        """
+        Increases the fonts by the specified amount (default: 1).
+        """
+        for font in self.__fonts:
+            newFont = font[0]()
+            newFont.setPointSize(newFont.pointSize() + amount)
+            font[1](newFont)
+
+    @Slot()
+    def decreaseFonts(self, amount = 1):
+        """
+        Decreases the fonts by the specified amount (default: 1).
+        """
+        for font in self.__fonts:
+            newFont = font[0]()
+            newFont.setPointSize(newFont.pointSize() - amount)
+            font[1](newFont)
+
+
+
+_fontHandler = _FontHandler()
+
+
+def getFontHandler():
+    """
+    Gets the instance of the singleton FontHandler.
+    """
+    return _fontHandler
```

### Comparing `msg_explorer-1.6.0/msg_explorer/guid_viewer.py` & `msg_explorer-1.7.0/msg_explorer/string_viewer.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,28 @@
-# This Python file uses the following encoding: utf-8
-from PySide6 import QtCore
-from PySide6 import QtWidgets
-from PySide6.QtCore import Signal, SIGNAL, Slot, SLOT
-
-from .ui.ui_guid_viewer import Ui_GuidViewer
-
-
-class GuidViewer(QtWidgets.QWidget):
-    def __init__(self):
-        super().__init__()
-        
-        self.ui = Ui_GuidViewer()
-        self.ui.setupUi(self)
-
-    @Slot()
-    def clear(self):
-        self.ui.labelGuid.setText('')
-
-    @Slot(object)
-    def loadGuid(self, guid):
-        self.ui.labelGuid.setText(guid)
+# This Python file uses the following encoding: utf-8
+from PySide6 import QtCore
+from PySide6 import QtWidgets
+from PySide6.QtCore import Signal, SIGNAL, Slot, SLOT
+
+from .ui.ui_string_viewer import Ui_StringViewer
+
+
+class StringViewer(QtWidgets.QWidget):
+    def __init__(self):
+        super().__init__()
+        
+        self.ui = Ui_StringViewer()
+        self.ui.setupUi(self)
+
+    @Slot()
+    def clear(self):
+        self.ui.labelType.setText('')
+        self.ui.textDisplay.setPlainText('')
+
+    @Slot(str, str)
+    def loadString(self, data, _type):
+        """
+        Displays the specified string as well as the exact
+        type the data was.
+        """
+        self.ui.labelType.setText('UTF-16-LE String' if _type == '001F' else 'Non-Unicode String')
+        self.ui.textDisplay.setPlainText(data)
```

### Comparing `msg_explorer-1.6.0/msg_explorer/hex_viewer.py` & `msg_explorer-1.7.0/msg_explorer/hex_viewer.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,67 +1,67 @@
-# This Python file uses the following encoding: utf-8
-from PySide6 import QtCore
-from PySide6 import QtWidgets
-from PySide6.QtCore import Slot
-from PySide6.QtGui import QFont
-
-from . import font_handler
-from .ui.ui_hex_viewer import Ui_HexViewer
-
-
-HEX_LINE_LEN = 0x10
-
-_CHARS = (
-    '.', '.', '.', '.', '.', '.', '.', '.', '.', '.', '.', '.', '.', '.', '.', '.',
-    '.', '.', '.', '.', '.', '.', '.', '.', '.', '.', '.', '.', '.', '.', '.', '.',
-    ' ', '!', '&quot;', '#', '$', '%', '&amp;', '&apos;', '(', ')', '*', '+', ',', '-', '.', '/',
-    '0', '1', '2', '3', '4', '5', '6', '7', '8', '9', ':', ';', '&lt;', '=', '&gt;', '?',
-    '@', 'A', 'B', 'C', 'D', 'E', 'F', 'G', 'H', 'I', 'J', 'K', 'L', 'M', 'N', 'O',
-    'P', 'Q', 'R', 'S', 'T', 'U', 'V', 'W', 'X', 'Y', 'Z', '[', '\\', ']', '^', '_',
-    '`', 'a', 'b', 'c', 'd', 'e', 'f', 'g', 'h', 'i', 'j', 'k', 'l', 'm', 'n', 'o',
-    'p', 'q', 'r', 's', 't', 'u', 'v', 'w', 'x', 'y', 'z', '{', '|', '}', '~', '.',
-    '€', '.', '‚', 'ƒ', '„', '…', '†', '‡', 'ˆ', '‰', 'Š', '‹', 'Œ', '.', 'Ž', '.',
-    '.', '‘', '’', '“', '”', '•', '–', '—', '˜', '™', 'š', '›', 'œ', '.', 'ž', 'Ÿ',
-    ' ', '¡', '¢', '£', '¤', '¥', '¦', '§', '¨', '©', 'ª', '«', '¬', '.', '®', '¯',
-    '°', '±', '²', '³', '´', 'µ', '¶', '·', '¸', '¹', 'º', '»', '¼', '½', '¾', '¿',
-    'À', 'Á', 'Â', 'Ã', 'Ä', 'Å', 'Æ', 'Ç', 'È', 'É', 'Ê', 'Ë', 'Ì', 'Í', 'Î', 'Ï',
-    'Ð', 'Ñ', 'Ò', 'Ó', 'Ô', 'Õ', 'Ö', '×', 'Ø', 'Ù', 'Ú', 'Û', 'Ü', 'Ý', 'Þ', 'ß',
-    'à', 'á', 'â', 'ã', 'ä', 'å', 'æ', 'ç', 'è', 'é', 'ê', 'ë', 'ì', 'í', 'î', 'ï',
-    'ð', 'ñ', 'ò', 'ó', 'ô', 'õ', 'ö', '÷', 'ø', 'ù', 'ú', 'û', 'ü', 'ý', 'þ', 'ÿ',
-)
-
-
-class HexViewer(QtWidgets.QWidget):
-    def __init__(self, parent = None):
-        super().__init__(parent)
-        
-        self.ui = Ui_HexViewer()
-        self.ui.setupUi(self)
-
-        font_handler.getFontHandler().registerFont(self.ui.hexViewer.font, self.ui.hexViewer.setFont)
-
-    @Slot()
-    def clear(self):
-        self.ui.hexViewer.setPlainText('')
-
-    @Slot(bytes)
-    def loadHexData(self, data):
-        # First we need to convert the bytes into a hex stream.
-        hexStream = [f'{x:02X}' for x in data]
-        lines = [hexStream[HEX_LINE_LEN * x: HEX_LINE_LEN * (x + 1)] for x in range((len(hexStream) + HEX_LINE_LEN - 1) // HEX_LINE_LEN)]
-        rawDataLines = [data[HEX_LINE_LEN * x: HEX_LINE_LEN * (x + 1)] for x in range((len(data) + HEX_LINE_LEN - 1) // HEX_LINE_LEN)]
-
-        # Process the raw data lines so they properly render. We want to
-        # convert any bad characters into periods.
-        rawDataLines = tuple(''.join(_CHARS[x] for x in line) for line in rawDataLines)
-
-        # Pad out the last line if it is not 16 bytes.
-        if lines:
-            if len(lines[-1]) != 16:
-                lines[-1] += ['  '] * (16 - len(lines[-1]))
-
-        # First setup the start of the data.
-        finalHexData = '<html><head><style>span { color: #0000AA; }</style></head><body>'
-        finalHexData += '<span>Offset    00 01 02 03 04 05 06 07 08 09 0A 0B 0C 0D 0E 0F    Decoded Text</span>\n<br>'.replace(' ', '&nbsp;')
-        finalHexData += '<br>\n'.join(f'<span>{index * 16:08X}</span>  {" ".join(line)}    {rawDataLines[index]}' for index, line in enumerate(lines)).replace(' ', '&nbsp;')
-        finalHexData += '</body></html>'
-        self.ui.hexViewer.setHtml(finalHexData)
+# This Python file uses the following encoding: utf-8
+from PySide6 import QtCore
+from PySide6 import QtWidgets
+from PySide6.QtCore import Slot
+from PySide6.QtGui import QFont
+
+from . import font_handler
+from .ui.ui_hex_viewer import Ui_HexViewer
+
+
+HEX_LINE_LEN = 0x10
+
+_CHARS = (
+    '.', '.', '.', '.', '.', '.', '.', '.', '.', '.', '.', '.', '.', '.', '.', '.',
+    '.', '.', '.', '.', '.', '.', '.', '.', '.', '.', '.', '.', '.', '.', '.', '.',
+    ' ', '!', '&quot;', '#', '$', '%', '&amp;', '&apos;', '(', ')', '*', '+', ',', '-', '.', '/',
+    '0', '1', '2', '3', '4', '5', '6', '7', '8', '9', ':', ';', '&lt;', '=', '&gt;', '?',
+    '@', 'A', 'B', 'C', 'D', 'E', 'F', 'G', 'H', 'I', 'J', 'K', 'L', 'M', 'N', 'O',
+    'P', 'Q', 'R', 'S', 'T', 'U', 'V', 'W', 'X', 'Y', 'Z', '[', '\\', ']', '^', '_',
+    '`', 'a', 'b', 'c', 'd', 'e', 'f', 'g', 'h', 'i', 'j', 'k', 'l', 'm', 'n', 'o',
+    'p', 'q', 'r', 's', 't', 'u', 'v', 'w', 'x', 'y', 'z', '{', '|', '}', '~', '.',
+    '€', '.', '‚', 'ƒ', '„', '…', '†', '‡', 'ˆ', '‰', 'Š', '‹', 'Œ', '.', 'Ž', '.',
+    '.', '‘', '’', '“', '”', '•', '–', '—', '˜', '™', 'š', '›', 'œ', '.', 'ž', 'Ÿ',
+    ' ', '¡', '¢', '£', '¤', '¥', '¦', '§', '¨', '©', 'ª', '«', '¬', '.', '®', '¯',
+    '°', '±', '²', '³', '´', 'µ', '¶', '·', '¸', '¹', 'º', '»', '¼', '½', '¾', '¿',
+    'À', 'Á', 'Â', 'Ã', 'Ä', 'Å', 'Æ', 'Ç', 'È', 'É', 'Ê', 'Ë', 'Ì', 'Í', 'Î', 'Ï',
+    'Ð', 'Ñ', 'Ò', 'Ó', 'Ô', 'Õ', 'Ö', '×', 'Ø', 'Ù', 'Ú', 'Û', 'Ü', 'Ý', 'Þ', 'ß',
+    'à', 'á', 'â', 'ã', 'ä', 'å', 'æ', 'ç', 'è', 'é', 'ê', 'ë', 'ì', 'í', 'î', 'ï',
+    'ð', 'ñ', 'ò', 'ó', 'ô', 'õ', 'ö', '÷', 'ø', 'ù', 'ú', 'û', 'ü', 'ý', 'þ', 'ÿ',
+)
+
+
+class HexViewer(QtWidgets.QWidget):
+    def __init__(self, parent = None):
+        super().__init__(parent)
+        
+        self.ui = Ui_HexViewer()
+        self.ui.setupUi(self)
+
+        font_handler.getFontHandler().registerFont(self.ui.hexViewer.font, self.ui.hexViewer.setFont)
+
+    @Slot()
+    def clear(self):
+        self.ui.hexViewer.setPlainText('')
+
+    @Slot(bytes)
+    def loadHexData(self, data):
+        # First we need to convert the bytes into a hex stream.
+        hexStream = [f'{x:02X}' for x in data]
+        lines = [hexStream[HEX_LINE_LEN * x: HEX_LINE_LEN * (x + 1)] for x in range((len(hexStream) + HEX_LINE_LEN - 1) // HEX_LINE_LEN)]
+        rawDataLines = [data[HEX_LINE_LEN * x: HEX_LINE_LEN * (x + 1)] for x in range((len(data) + HEX_LINE_LEN - 1) // HEX_LINE_LEN)]
+
+        # Process the raw data lines so they properly render. We want to
+        # convert any bad characters into periods.
+        rawDataLines = tuple(''.join(_CHARS[x] for x in line) for line in rawDataLines)
+
+        # Pad out the last line if it is not 16 bytes.
+        if lines:
+            if len(lines[-1]) != 16:
+                lines[-1] += ['  '] * (16 - len(lines[-1]))
+
+        # First setup the start of the data.
+        finalHexData = '<html><head><style>span { color: #0000AA; }</style></head><body>'
+        finalHexData += '<span>Offset    00 01 02 03 04 05 06 07 08 09 0A 0B 0C 0D 0E 0F    Decoded Text</span>\n<br>'.replace(' ', '&nbsp;')
+        finalHexData += '<br>\n'.join(f'<span>{index * 16:08X}</span>  {" ".join(line)}    {rawDataLines[index]}' for index, line in enumerate(lines)).replace(' ', '&nbsp;')
+        finalHexData += '</body></html>'
+        self.ui.hexViewer.setHtml(finalHexData)
```

### Comparing `msg_explorer-1.6.0/msg_explorer/icon/envelope_1024.png` & `msg_explorer-1.7.0/msg_explorer/icon/envelope_1024.png`

 * *Files identical despite different names*

### Comparing `msg_explorer-1.6.0/msg_explorer/logger.py` & `msg_explorer-1.7.0/msg_explorer/logger.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-import logging
-
-
-class WidgetLogger(logging.Handler):
-    def __init__(self, widget):
-        super().__init__()
-        self.__widget = widget
-        self.setLevel(5)
-        self.setFormatter(logging.Formatter('%(asctime)s - %(name)s - %(levelname)s - %(message)s'))
-
-    def emit(self, record):
-        """
-        Actually handle logging the record.
-        """
-        try:
-            msg = self.format(record)
-            self.__widget.log(msg)
-        except Exception:
-            self.handleError(record)
+import logging
+
+
+class WidgetLogger(logging.Handler):
+    def __init__(self, widget):
+        super().__init__()
+        self.__widget = widget
+        self.setLevel(5)
+        self.setFormatter(logging.Formatter('%(asctime)s - %(name)s - %(levelname)s - %(message)s'))
+
+    def emit(self, record):
+        """
+        Actually handle logging the record.
+        """
+        try:
+            msg = self.format(record)
+            self.__widget.log(msg)
+        except Exception:
+            self.handleError(record)
```

### Comparing `msg_explorer-1.6.0/msg_explorer/main_window.py` & `msg_explorer-1.7.0/msg_explorer/main_window.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,238 +1,238 @@
-# This Python file uses the following encoding: utf-8
-import os
-import pathlib
-import threading
-
-import extract_msg
-
-from PySide6.QtCore import QEventLoop, Signal, SIGNAL, Slot, SLOT
-from PySide6.QtGui import QIcon, QPixmap
-from PySide6.QtWidgets import QApplication, QFileDialog, QMainWindow, QMessageBox, QWidget
-
-from . import app_icons, font_handler, hex_viewer, utils, __version__
-from .logger_widget import LoggerWidget
-from .ui.ui_main_window import Ui_MainWindow
-from .ui.ui_loading_screen import Ui_LoadingScreen
-
-
-class MainWindow(QMainWindow):
-    # A signal that announces the msg file has been closed. Makes it easier
-    # to communicate to any components that need it so the close function
-    # doesn't have to be modified, just the signal/slot connections.
-    msgClosed = Signal()
-    msgOpened = Signal(extract_msg.msg.MSGFile)
-    # A signal which announces a desire to have the event loop process once.
-    processEventLoop = Signal()
-
-    def __init__(self, parent = None):
-        super().__init__(parent)
-
-        # Register the ui with this widget.
-        self.ui = Ui_MainWindow()
-        self.ui.setupUi(self)
-
-        # Connect the menu bar slots.
-        self.ui.actionLoad_Msg_File.triggered.connect(self.loadMsgFile)
-        self.ui.actionLoad_Parent_Msg.triggered.connect(self.loadParent)
-        self.ui.actionClose_Current_File.triggered.connect(self.closeFile)
-        self.ui.actionOpen_Log.triggered.connect(self._showLogWindow)
-        self.ui.actionExport_Current_File.triggered.connect(self.exportFile)
-
-        # Connect the pages to the opening and closing of the msg file.
-        self.msgOpened.connect(self.ui.pageBasicInformation.msgOpened)
-        self.msgOpened.connect(self.ui.pageTreeView.msgOpened)
-        self.msgOpened.connect(self.ui.pageAttachments.msgOpened)
-        self.msgOpened.connect(self.ui.pageNamedProperties.msgOpened)
-        self.msgOpened.connect(self.ui.pageStreamView.msgOpened)
-        self.msgClosed.connect(self.ui.pageBasicInformation.msgClosed)
-        self.msgClosed.connect(self.ui.pageTreeView.msgClosed)
-        self.msgClosed.connect(self.ui.pageAttachments.msgClosed)
-        self.msgClosed.connect(self.ui.pageNamedProperties.msgClosed)
-        self.msgClosed.connect(self.ui.pageStreamView.msgClosed)
-
-        # Connect the double click from the tree to the stream view.
-        self.ui.pageTreeView.fileDoubleClicked.connect(self.ui.pageStreamView.openStream)
-        self.ui.pageTreeView.fileDoubleClicked.connect(self._streamSelected)
-        self.ui.pageNamedProperties.namedPropertySelected.connect(self.ui.pageStreamView.openStream)
-        self.ui.pageNamedProperties.namedPropertySelected.connect(self._streamSelected)
-
-        self.ui.actionIncrease_Font.triggered.connect(self.increaseFont)
-        self.ui.actionDecrease_Font.triggered.connect(self.decreaseFont)
-
-        self.ui.pageAttachments.attachmentSelected.connect(self.attachmentSelected)
-        self.ui.pageAttachments.signedAttachmentSelected.connect(self.signedAttachmentSelected)
-
-        font_handler.getFontHandler().registerFont(self.font, self.setFont)
-
-        self.__msg = None
-        self.__parentMsgs = []
-
-        self.__logger = LoggerWidget()
-
-        self.mainIcon = QIcon(QPixmap(":/icon/envelope_1024.png"))
-        self.setWindowIcon(self.mainIcon)
-
-        # Attempt to set the actual icon on the taskbar in windows.
-        if os.name == 'nt':
-            import ctypes
-            appid = f'TeamMsgExtractor.MSGExplorer.{__version__}'
-            ctypes.windll.shell32.SetCurrentProcessExplicitAppUserModelID(appid)
-
-    def closeEvent(self, event):
-        """
-        Override the default close function to cause all windows to be
-        closed by this function before running default close.
-        """
-        QApplication.closeAllWindows()
-
-    def dragEnterEvent(self, event):
-        # Handle a file being drag and dropped onto this window.
-        mime = event.mimeData()
-        if mime.hasUrls() and len(mime.urls()) == 1 and mime.urls()[0].isLocalFile():
-            # We know it has exactly one local url, so let's check it.
-            f = pathlib.Path(mime.urls()[0].toLocalFile())
-            if f.suffix.lower() == '.msg' and f.is_file():
-                event.acceptProposedAction()
-
-    def dropEvent(self, event):
-        if QMessageBox.question(self, self.tr('Open Msg?'), self.tr('Are you sure you want to open this MSG file?')) == QMessageBox.Yes:
-            event.acceptProposedAction()
-            self.loadMsgFile(event.mimeData().urls()[0].toLocalFile())
-
-    @Slot(int)
-    def attachmentSelected(self, index):
-        if isinstance(self.__msg, extract_msg.MessageSignedBase):
-            attachment = self.__msg._rawAttachments[index]
-        else:
-            attachment = self.__msg.attachments[index]
-
-        if isinstance(attachment, extract_msg.Attachment):
-            if attachment.type == extract_msg.enums.AttachmentType.DATA:
-                self.ui.pageStreamView.openStream(attachment.dir.split('/') + ['__substg1.0_37010102'])
-                self.ui.tabWidget.setCurrentWidget(self.ui.pageStreamView)
-            elif attachment.type == extract_msg.enums.AttachmentType.MSG:
-                if QMessageBox.question(self, self.tr('Open Embedded Msg'), self.tr('Would you like to open the embedded MSG file?')) == QMessageBox.Yes:
-                    self.__parentMsgs.append(self.__msg)
-                    self.__msg = attachment.data
-                    self.msgClosed.emit()
-                    self.msgOpened.emit(self.__msg)
-                    self.ui.actionLoad_Parent_Msg.setEnabled(True)
-
-    @Slot()
-    def closeFile(self):
-        """
-        Closes the current MSG file and cleans up all the UI components.
-        """
-        if self.__msg:
-            if self.__parentMsgs:
-                self.__parentMsgs[0].close()
-                self.__parentMsgs.clear()
-            else:
-                self.__msg.close()
-            self.__msg = None
-            self.msgClosed.emit()
-            self.ui.actionClose_Current_File.setEnabled(False)
-            self.ui.actionLoad_Parent_Msg.setEnabled(False)
-            self.ui.actionExport_Current_File.setEnabled(False)
-
-    @Slot()
-    def exportFile(self):
-        """
-        Export the currently opened MSG file to the location the user provides.
-        """
-        filename = QFileDialog.getSaveFileName(self, self.tr('Export File'), filter = self.tr('MSG files (*.msg)'))
-        if filename[0]:
-            try:
-                self.__msg.export(filename[0])
-                QMessageBox.information(self, self.tr('Export Complete'), f'Exported to "{filename[0]}"')
-            except Exception as e:
-                utils.displayException(e)
-
-    @Slot()
-    def loadMsgFile(self, path = None):
-        """
-        Brings up a dialog to load a specific MSG file.
-        """
-        if path:
-            msgPath = path
-        else:
-            msgPath = QFileDialog.getOpenFileName(filter = self.tr('MSG files (*.msg)'))[0]
-        if msgPath:
-            # Create a popup for the loading screen.
-            loadingScreenWidget = QWidget()
-            loadingScreen = Ui_LoadingScreen()
-            loadingScreen.setupUi(loadingScreenWidget)
-            loadingScreenWidget.show()
-
-            # We run the loading in a new thread so the ui can still update.
-            output = [None]
-            thread = threading.Thread(target = self._loadMsgThread, args = (msgPath, output,), daemon = True)
-            thread.start()
-
-            # Wait for the thread to finish and keep updating the ui.
-            while thread.is_alive():
-                self.processEventLoop.emit()
-
-            # Check for an error from the thread.
-            if isinstance(output[0], Exception):
-                if isinstance(output[0], extract_msg.exceptions.InvalidFileFormatError):
-                    QMessageBox.critical(self, self.tr('Error'), self.tr('File is not an MSG file.'))
-                else:
-                    utils.displayException(output[0])
-            else:
-                self.closeFile()
-                self.__msg = output[0]
-                loadingScreen.loadingMessage.setText(self.tr('Finishing up...'))
-                self.processEventLoop.emit()
-                self.msgOpened.emit(self.__msg)
-
-            del loadingScreenWidget
-
-            self.ui.actionClose_Current_File.setEnabled(True)
-            self.ui.actionExport_Current_File.setEnabled(True)
-
-    @Slot()
-    def loadParent(self):
-        """
-        Moves to the parent msg file.
-        """
-        if self.__parentMsgs:
-            self.__msg = self.__parentMsgs.pop()
-            self.msgClosed.emit()
-            self.msgOpened.emit(self.__msg)
-            if not self.__parentMsgs:
-                self.ui.actionLoad_Parent_Msg.setEnabled(False)
-        else:
-            QMessageBox.critical(self, self.tr('Error'), self.tr('No parent MSG file.'))
-
-    def _loadMsgThread(self, msgPath, output):
-        try:
-            msgFile = extract_msg.openMsg(msgPath, attachmentErrorBehavior = extract_msg.enums.AttachErrorBehavior.BROKEN, strict = False)
-            output[0] = msgFile
-        except Exception as e:
-            output[0] = e
-
-    @Slot(int)
-    def signedAttachmentSelected(self, index : int):
-        """
-        Handle a signed attachment being selected.
-        """
-        att = self.__msg.attachments[index]
-        self.ui.pageStreamView.openStreamBytes(f'Signed Attachment: {att.name}', att.data)
-        self.ui.tabWidget.setCurrentWidget(self.ui.pageStreamView)
-
-    @Slot()
-    def _showLogWindow(self):
-        self.__logger.show()
-
-    @Slot(object)
-    def _streamSelected(self, *args):
-        self.ui.tabWidget.setCurrentWidget(self.ui.pageStreamView)
-
-    @Slot()
-    def increaseFont(self):
-        font_handler.getFontHandler().increaseFonts()
-
-    @Slot()
-    def decreaseFont(self):
-        font_handler.getFontHandler().decreaseFonts()
+# This Python file uses the following encoding: utf-8
+import os
+import pathlib
+import threading
+
+import extract_msg
+
+from PySide6.QtCore import QEventLoop, Signal, SIGNAL, Slot, SLOT
+from PySide6.QtGui import QIcon, QPixmap
+from PySide6.QtWidgets import QApplication, QFileDialog, QMainWindow, QMessageBox, QWidget
+
+from . import app_icons, font_handler, hex_viewer, utils, __version__
+from .logger_widget import LoggerWidget
+from .ui.ui_main_window import Ui_MainWindow
+from .ui.ui_loading_screen import Ui_LoadingScreen
+
+
+class MainWindow(QMainWindow):
+    # A signal that announces the msg file has been closed. Makes it easier
+    # to communicate to any components that need it so the close function
+    # doesn't have to be modified, just the signal/slot connections.
+    msgClosed = Signal()
+    msgOpened = Signal(extract_msg.msg.MSGFile)
+    # A signal which announces a desire to have the event loop process once.
+    processEventLoop = Signal()
+
+    def __init__(self, parent = None):
+        super().__init__(parent)
+
+        # Register the ui with this widget.
+        self.ui = Ui_MainWindow()
+        self.ui.setupUi(self)
+
+        # Connect the menu bar slots.
+        self.ui.actionLoad_Msg_File.triggered.connect(self.loadMsgFile)
+        self.ui.actionLoad_Parent_Msg.triggered.connect(self.loadParent)
+        self.ui.actionClose_Current_File.triggered.connect(self.closeFile)
+        self.ui.actionOpen_Log.triggered.connect(self._showLogWindow)
+        self.ui.actionExport_Current_File.triggered.connect(self.exportFile)
+
+        # Connect the pages to the opening and closing of the msg file.
+        self.msgOpened.connect(self.ui.pageBasicInformation.msgOpened)
+        self.msgOpened.connect(self.ui.pageTreeView.msgOpened)
+        self.msgOpened.connect(self.ui.pageAttachments.msgOpened)
+        self.msgOpened.connect(self.ui.pageNamedProperties.msgOpened)
+        self.msgOpened.connect(self.ui.pageStreamView.msgOpened)
+        self.msgClosed.connect(self.ui.pageBasicInformation.msgClosed)
+        self.msgClosed.connect(self.ui.pageTreeView.msgClosed)
+        self.msgClosed.connect(self.ui.pageAttachments.msgClosed)
+        self.msgClosed.connect(self.ui.pageNamedProperties.msgClosed)
+        self.msgClosed.connect(self.ui.pageStreamView.msgClosed)
+
+        # Connect the double click from the tree to the stream view.
+        self.ui.pageTreeView.fileDoubleClicked.connect(self.ui.pageStreamView.openStream)
+        self.ui.pageTreeView.fileDoubleClicked.connect(self._streamSelected)
+        self.ui.pageNamedProperties.namedPropertySelected.connect(self.ui.pageStreamView.openStream)
+        self.ui.pageNamedProperties.namedPropertySelected.connect(self._streamSelected)
+
+        self.ui.actionIncrease_Font.triggered.connect(self.increaseFont)
+        self.ui.actionDecrease_Font.triggered.connect(self.decreaseFont)
+
+        self.ui.pageAttachments.attachmentSelected.connect(self.attachmentSelected)
+        self.ui.pageAttachments.signedAttachmentSelected.connect(self.signedAttachmentSelected)
+
+        font_handler.getFontHandler().registerFont(self.font, self.setFont)
+
+        self.__msg = None
+        self.__parentMsgs = []
+
+        self.__logger = LoggerWidget()
+
+        self.mainIcon = QIcon(QPixmap(":/icon/envelope_1024.png"))
+        self.setWindowIcon(self.mainIcon)
+
+        # Attempt to set the actual icon on the taskbar in windows.
+        if os.name == 'nt':
+            import ctypes
+            appid = f'TeamMsgExtractor.MSGExplorer.{__version__}'
+            ctypes.windll.shell32.SetCurrentProcessExplicitAppUserModelID(appid)
+
+    def closeEvent(self, event):
+        """
+        Override the default close function to cause all windows to be
+        closed by this function before running default close.
+        """
+        QApplication.closeAllWindows()
+
+    def dragEnterEvent(self, event):
+        # Handle a file being drag and dropped onto this window.
+        mime = event.mimeData()
+        if mime.hasUrls() and len(mime.urls()) == 1 and mime.urls()[0].isLocalFile():
+            # We know it has exactly one local url, so let's check it.
+            f = pathlib.Path(mime.urls()[0].toLocalFile())
+            if f.suffix.lower() == '.msg' and f.is_file():
+                event.acceptProposedAction()
+
+    def dropEvent(self, event):
+        if QMessageBox.question(self, self.tr('Open Msg?'), self.tr('Are you sure you want to open this MSG file?')) == QMessageBox.Yes:
+            event.acceptProposedAction()
+            self.loadMsgFile(event.mimeData().urls()[0].toLocalFile())
+
+    @Slot(int)
+    def attachmentSelected(self, index):
+        if isinstance(self.__msg, extract_msg.MessageSignedBase):
+            attachment = self.__msg._rawAttachments[index]
+        else:
+            attachment = self.__msg.attachments[index]
+
+        if isinstance(attachment, extract_msg.Attachment):
+            if attachment.type == extract_msg.enums.AttachmentType.DATA:
+                self.ui.pageStreamView.openStream(attachment.dir.split('/') + ['__substg1.0_37010102'])
+                self.ui.tabWidget.setCurrentWidget(self.ui.pageStreamView)
+            elif attachment.type == extract_msg.enums.AttachmentType.MSG:
+                if QMessageBox.question(self, self.tr('Open Embedded Msg'), self.tr('Would you like to open the embedded MSG file?')) == QMessageBox.Yes:
+                    self.__parentMsgs.append(self.__msg)
+                    self.__msg = attachment.data
+                    self.msgClosed.emit()
+                    self.msgOpened.emit(self.__msg)
+                    self.ui.actionLoad_Parent_Msg.setEnabled(True)
+
+    @Slot()
+    def closeFile(self):
+        """
+        Closes the current MSG file and cleans up all the UI components.
+        """
+        if self.__msg:
+            if self.__parentMsgs:
+                self.__parentMsgs[0].close()
+                self.__parentMsgs.clear()
+            else:
+                self.__msg.close()
+            self.__msg = None
+            self.msgClosed.emit()
+            self.ui.actionClose_Current_File.setEnabled(False)
+            self.ui.actionLoad_Parent_Msg.setEnabled(False)
+            self.ui.actionExport_Current_File.setEnabled(False)
+
+    @Slot()
+    def exportFile(self):
+        """
+        Export the currently opened MSG file to the location the user provides.
+        """
+        filename = QFileDialog.getSaveFileName(self, self.tr('Export File'), filter = self.tr('MSG files (*.msg)'))
+        if filename[0]:
+            try:
+                self.__msg.export(filename[0])
+                QMessageBox.information(self, self.tr('Export Complete'), f'Exported to "{filename[0]}"')
+            except Exception as e:
+                utils.displayException(e)
+
+    @Slot()
+    def loadMsgFile(self, path = None):
+        """
+        Brings up a dialog to load a specific MSG file.
+        """
+        if path:
+            msgPath = path
+        else:
+            msgPath = QFileDialog.getOpenFileName(filter = self.tr('MSG files (*.msg)'))[0]
+        if msgPath:
+            # Create a popup for the loading screen.
+            loadingScreenWidget = QWidget()
+            loadingScreen = Ui_LoadingScreen()
+            loadingScreen.setupUi(loadingScreenWidget)
+            loadingScreenWidget.show()
+
+            # We run the loading in a new thread so the ui can still update.
+            output = [None]
+            thread = threading.Thread(target = self._loadMsgThread, args = (msgPath, output,), daemon = True)
+            thread.start()
+
+            # Wait for the thread to finish and keep updating the ui.
+            while thread.is_alive():
+                self.processEventLoop.emit()
+
+            # Check for an error from the thread.
+            if isinstance(output[0], Exception):
+                if isinstance(output[0], extract_msg.exceptions.InvalidFileFormatError):
+                    QMessageBox.critical(self, self.tr('Error'), self.tr('File is not an MSG file.'))
+                else:
+                    utils.displayException(output[0])
+            else:
+                self.closeFile()
+                self.__msg = output[0]
+                loadingScreen.loadingMessage.setText(self.tr('Finishing up...'))
+                self.processEventLoop.emit()
+                self.msgOpened.emit(self.__msg)
+
+            del loadingScreenWidget
+
+            self.ui.actionClose_Current_File.setEnabled(True)
+            self.ui.actionExport_Current_File.setEnabled(True)
+
+    @Slot()
+    def loadParent(self):
+        """
+        Moves to the parent msg file.
+        """
+        if self.__parentMsgs:
+            self.__msg = self.__parentMsgs.pop()
+            self.msgClosed.emit()
+            self.msgOpened.emit(self.__msg)
+            if not self.__parentMsgs:
+                self.ui.actionLoad_Parent_Msg.setEnabled(False)
+        else:
+            QMessageBox.critical(self, self.tr('Error'), self.tr('No parent MSG file.'))
+
+    def _loadMsgThread(self, msgPath, output):
+        try:
+            msgFile = extract_msg.openMsg(msgPath, errorBehavior = extract_msg.enums.ErrorBehavior.SUPPRESS_ALL, strict = False)
+            output[0] = msgFile
+        except Exception as e:
+            output[0] = e
+
+    @Slot(int)
+    def signedAttachmentSelected(self, index : int):
+        """
+        Handle a signed attachment being selected.
+        """
+        att = self.__msg.attachments[index]
+        self.ui.pageStreamView.openStreamBytes(f'Signed Attachment: {att.name}', att.data)
+        self.ui.tabWidget.setCurrentWidget(self.ui.pageStreamView)
+
+    @Slot()
+    def _showLogWindow(self):
+        self.__logger.show()
+
+    @Slot(object)
+    def _streamSelected(self, *args):
+        self.ui.tabWidget.setCurrentWidget(self.ui.pageStreamView)
+
+    @Slot()
+    def increaseFont(self):
+        font_handler.getFontHandler().increaseFonts()
+
+    @Slot()
+    def decreaseFont(self):
+        font_handler.getFontHandler().decreaseFonts()
```

### Comparing `msg_explorer-1.6.0/msg_explorer/msg_details_page.py` & `msg_explorer-1.7.0/msg_explorer/msg_details_page.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-# This Python file uses the following encoding: utf-8
-import extract_msg
-
-from PySide6 import QtCore
-from PySide6 import QtWidgets
-from PySide6.QtCore import Signal, SIGNAL, Slot, SLOT
-
-from .ui.ui_msg_details_page import Ui_MSGDetailsPage
-
-
-class MSGDetailsPage(QtWidgets.QWidget):
-    def __init__(self, parent = None):
-        super().__init__(parent)
-        
-        self.ui = Ui_MSGDetailsPage()
-        self.ui.setupUi(self)
-
-    @Slot()
-    def msgClosed(self):
-        self.ui.labelPath.setText('No File Loaded')
-        self.ui.labelPrefix.setText('')
-        self.ui.labelClass.setText('')
-        self.ui.labelClassType.setText('')
-        self.ui.labelEncoding.setText('')
-        self.ui.labelAttachCount.setText('')
-        self.ui.labelRecipCount.setText('')
-        self.ui.labelSubject.setText('')
-
-    @Slot(extract_msg.msg.MSGFile)
-    def msgOpened(self, msgFile):
-        if len(msgFile.path) < 1536:
-            self.ui.labelPath.setText(msgFile.path)
-        self.ui.labelPrefix.setText(msgFile.prefix)
-        self.ui.labelClass.setText(msgFile.__class__.__name__)
-        self.ui.labelClassType.setText(msgFile.classType)
-        self.ui.labelEncoding.setText(msgFile.stringEncoding)
-        self.ui.labelAttachCount.setText(str(len(msgFile.attachments)))
-        if isinstance(msgFile, extract_msg.MessageBase):
-            self.ui.labelRecipCount.setText(str(len(msgFile.recipients)))
-            self.ui.labelSubject.setText(msgFile.subject)
+# This Python file uses the following encoding: utf-8
+import extract_msg
+
+from PySide6 import QtCore
+from PySide6 import QtWidgets
+from PySide6.QtCore import Signal, SIGNAL, Slot, SLOT
+
+from .ui.ui_msg_details_page import Ui_MSGDetailsPage
+
+
+class MSGDetailsPage(QtWidgets.QWidget):
+    def __init__(self, parent = None):
+        super().__init__(parent)
+        
+        self.ui = Ui_MSGDetailsPage()
+        self.ui.setupUi(self)
+
+    @Slot()
+    def msgClosed(self):
+        self.ui.labelPath.setText('No File Loaded')
+        self.ui.labelPrefix.setText('')
+        self.ui.labelClass.setText('')
+        self.ui.labelClassType.setText('')
+        self.ui.labelEncoding.setText('')
+        self.ui.labelAttachCount.setText('')
+        self.ui.labelRecipCount.setText('')
+        self.ui.labelSubject.setText('')
+
+    @Slot(extract_msg.msg.MSGFile)
+    def msgOpened(self, msgFile):
+        if len(msgFile.path) < 1536:
+            self.ui.labelPath.setText(msgFile.path)
+        self.ui.labelPrefix.setText(msgFile.prefix)
+        self.ui.labelClass.setText(msgFile.__class__.__name__)
+        self.ui.labelClassType.setText(msgFile.classType)
+        self.ui.labelEncoding.setText(msgFile.stringEncoding)
+        self.ui.labelAttachCount.setText(str(len(msgFile.attachments)))
+        if isinstance(msgFile, extract_msg.MessageBase):
+            self.ui.labelRecipCount.setText(str(len(msgFile.recipients)))
+            self.ui.labelSubject.setText(msgFile.subject)
```

### Comparing `msg_explorer-1.6.0/msg_explorer/msg_tree_viewer.py` & `msg_explorer-1.7.0/msg_explorer/msg_tree_viewer.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,123 +1,123 @@
-# This Python file uses the following encoding: utf-8
-import enum
-import pprint
-
-import extract_msg
-
-from PySide6 import QtCore
-from PySide6 import QtWidgets
-from PySide6.QtCore import Signal, SIGNAL, Slot, SLOT
-from PySide6.QtWidgets import QTreeWidgetItem
-
-from . import constants, utils
-from .ui.ui_msg_tree_viewer import Ui_MSGTreeViewer
-
-
-class _DataTypeEnum(enum.Enum):
-    FILE = 0
-    FOLDER = 1
-
-
-
-class MsgTreeItem(QTreeWidgetItem):
-    def __init__(self, text : str, _type : _DataTypeEnum):
-        # First thing is first, check the text to see if it needs to be corrected.
-        self.__rawText = text
-        text = constants.RE_SPECIAL_CHAR.sub(lambda match : f'[{ord(match.group())}]', text)
-        super().__init__((text,))
-        self.__entryType = _type
-
-    def __lt__(self, treeItem : "MsgTreeItem"):
-        if self.__entryType == treeItem.__entryType:
-            return self.data(0, 0) < treeItem.data(0, 0)
-        else:
-            # If they are not the same type, folder is always less than file.
-            return self.__entryType == _DataTypeEnum.FOLDER
-
-    @property
-    def entryType(self) -> _DataTypeEnum:
-        return self.__entryType
-
-    @property
-    def rawText(self) -> str:
-        return self.__rawText
-
-
-
-class MSGTreeViewer(QtWidgets.QWidget):
-    # Signal to indicate a file has been double clicked.
-    fileDoubleClicked = Signal(list)
-
-    def __init__(self, parent = None):
-        super().__init__(parent)
-
-        self.ui = Ui_MSGTreeViewer()
-        self.ui.setupUi(self)
-
-        self.iconProvider = QtWidgets.QFileIconProvider()
-
-        self.ui.treeWidget.itemDoubleClicked.connect(self._treeItemDoubleClicked)
-        self.ui.treeWidget.sortItems(0, QtCore.Qt.SortOrder.AscendingOrder)
-
-    @Slot()
-    def msgClosed(self):
-        self.ui.treeWidget.clear()
-
-    @Slot(extract_msg.msg.MSGFile)
-    def msgOpened(self, msgFile):
-        folderIcon = self.iconProvider.icon(QtWidgets.QFileIconProvider.Folder)
-        fileIcon = fileIcon = self.iconProvider.icon(QtWidgets.QFileIconProvider.File)
-        # First handle all of the storages. These will be the base
-        # for all streams.
-        storages = {}
-        prefixLen = msgFile.prefixLen
-        prefixTuple = tuple(msgFile.prefixList)
-        for path in msgFile.listDir(False, True):
-            # Only add if part of the local file.
-            path = path[prefixLen:]
-            storages[tuple(path)] = MsgTreeItem(path[-1], _DataTypeEnum.FOLDER)
-            storages[tuple(path)].setIcon(0, folderIcon)
-
-        # Now connect all of the parents together properly.
-        for path in storages:
-            if len(path) > 1:
-                try:
-                    parent = storages[path[:-1]]
-                    parent.addChild(storages[path])
-                except KeyError as e:
-                    utils.displayException(e, 'Issue in MSG file detected: Storage directory exists but it\'s parent does not.')
-
-        # Now add the top level ones to the tree.
-        for path in storages:
-            if len(path) == 1:
-                self.ui.treeWidget.addTopLevelItem(storages[path])
-
-        # Now we add the files.
-        for path in msgFile.listDir(True, False):
-            path = path[prefixLen:]
-            item = MsgTreeItem(path[-1], _DataTypeEnum.FILE)
-            item.setIcon(0, fileIcon)
-            if len(path) > 1:
-                try:
-                    storages[tuple(path[:-1])].addChild(item)
-                except KeyError as e:
-                    utils.displayException(e, 'Issue in MSG file detected: stream exists but it\'s parent does not.')
-            else:
-                self.ui.treeWidget.addTopLevelItem(item)
-
-    @Slot(QtWidgets.QTreeWidgetItem, int)
-    def _treeItemDoubleClicked(self, item, column):
-        """
-        Handles a stream in the tree being double clicked.
-        """
-        # Check if the item clicked was a stream. If it was, then continue.
-        if item.entryType == _DataTypeEnum.FILE:
-            path = [item.rawText]
-            while item.parent():
-                item = item.parent()
-                path.insert(0, item.rawText)
-
-            self.fileDoubleClicked.emit(path)
-
-
-
+# This Python file uses the following encoding: utf-8
+import enum
+import pprint
+
+import extract_msg
+
+from PySide6 import QtCore
+from PySide6 import QtWidgets
+from PySide6.QtCore import Signal, SIGNAL, Slot, SLOT
+from PySide6.QtWidgets import QTreeWidgetItem
+
+from . import constants, utils
+from .ui.ui_msg_tree_viewer import Ui_MSGTreeViewer
+
+
+class _DataTypeEnum(enum.Enum):
+    FILE = 0
+    FOLDER = 1
+
+
+
+class MsgTreeItem(QTreeWidgetItem):
+    def __init__(self, text : str, _type : _DataTypeEnum):
+        # First thing is first, check the text to see if it needs to be corrected.
+        self.__rawText = text
+        text = constants.RE_SPECIAL_CHAR.sub(lambda match : f'[{ord(match.group())}]', text)
+        super().__init__((text,))
+        self.__entryType = _type
+
+    def __lt__(self, treeItem : "MsgTreeItem"):
+        if self.__entryType == treeItem.__entryType:
+            return self.data(0, 0) < treeItem.data(0, 0)
+        else:
+            # If they are not the same type, folder is always less than file.
+            return self.__entryType == _DataTypeEnum.FOLDER
+
+    @property
+    def entryType(self) -> _DataTypeEnum:
+        return self.__entryType
+
+    @property
+    def rawText(self) -> str:
+        return self.__rawText
+
+
+
+class MSGTreeViewer(QtWidgets.QWidget):
+    # Signal to indicate a file has been double clicked.
+    fileDoubleClicked = Signal(list)
+
+    def __init__(self, parent = None):
+        super().__init__(parent)
+
+        self.ui = Ui_MSGTreeViewer()
+        self.ui.setupUi(self)
+
+        self.iconProvider = QtWidgets.QFileIconProvider()
+
+        self.ui.treeWidget.itemDoubleClicked.connect(self._treeItemDoubleClicked)
+        self.ui.treeWidget.sortItems(0, QtCore.Qt.SortOrder.AscendingOrder)
+
+    @Slot()
+    def msgClosed(self):
+        self.ui.treeWidget.clear()
+
+    @Slot(extract_msg.msg.MSGFile)
+    def msgOpened(self, msgFile):
+        folderIcon = self.iconProvider.icon(QtWidgets.QFileIconProvider.Folder)
+        fileIcon = fileIcon = self.iconProvider.icon(QtWidgets.QFileIconProvider.File)
+        # First handle all of the storages. These will be the base
+        # for all streams.
+        storages = {}
+        prefixLen = msgFile.prefixLen
+        prefixTuple = tuple(msgFile.prefixList)
+        for path in msgFile.listDir(False, True):
+            # Only add if part of the local file.
+            path = path[prefixLen:]
+            storages[tuple(path)] = MsgTreeItem(path[-1], _DataTypeEnum.FOLDER)
+            storages[tuple(path)].setIcon(0, folderIcon)
+
+        # Now connect all of the parents together properly.
+        for path in storages:
+            if len(path) > 1:
+                try:
+                    parent = storages[path[:-1]]
+                    parent.addChild(storages[path])
+                except KeyError as e:
+                    utils.displayException(e, 'Issue in MSG file detected: Storage directory exists but it\'s parent does not.')
+
+        # Now add the top level ones to the tree.
+        for path in storages:
+            if len(path) == 1:
+                self.ui.treeWidget.addTopLevelItem(storages[path])
+
+        # Now we add the files.
+        for path in msgFile.listDir(True, False):
+            path = path[prefixLen:]
+            item = MsgTreeItem(path[-1], _DataTypeEnum.FILE)
+            item.setIcon(0, fileIcon)
+            if len(path) > 1:
+                try:
+                    storages[tuple(path[:-1])].addChild(item)
+                except KeyError as e:
+                    utils.displayException(e, 'Issue in MSG file detected: stream exists but it\'s parent does not.')
+            else:
+                self.ui.treeWidget.addTopLevelItem(item)
+
+    @Slot(QtWidgets.QTreeWidgetItem, int)
+    def _treeItemDoubleClicked(self, item, column):
+        """
+        Handles a stream in the tree being double clicked.
+        """
+        # Check if the item clicked was a stream. If it was, then continue.
+        if item.entryType == _DataTypeEnum.FILE:
+            path = [item.rawText]
+            while item.parent():
+                item = item.parent()
+                path.insert(0, item.rawText)
+
+            self.fileDoubleClicked.emit(path)
+
+
+
```

### Comparing `msg_explorer-1.6.0/msg_explorer/named_properties_viewer.py` & `msg_explorer-1.7.0/msg_explorer/named_properties_viewer.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,129 +1,129 @@
-# This Python file uses the following encoding: utf-8
-import logging
-
-import extract_msg
-
-from PySide6 import QtCore
-from PySide6 import QtWidgets
-from PySide6.QtCore import Signal, SIGNAL, Slot, SLOT
-from PySide6.QtWidgets import QMessageBox, QTableWidgetItem
-
-from . import utils
-from .ui.ui_named_properties_viewer import Ui_NamedPropertiesViewer
-
-
-logger = logging.getLogger(__name__)
-logger.addHandler(logging.NullHandler())
-
-
-class NamedPIDItem(QTableWidgetItem):
-    """
-    Little bit of a hack to force the Named PID column to sort properly.
-    """
-    def __lt__(self, item):
-        return int(self.data(0)) < int(item.data(0))
-
-
-
-class NamedPropertiesViewer(QtWidgets.QWidget):
-    namedPropertySelected = Signal(list)
-    def __init__(self, parent = None):
-        super().__init__(parent)
-        
-        self.ui = Ui_NamedPropertiesViewer()
-        self.ui.setupUi(self)
-        self.__loading = False
-        self.__msg = None
-        # This is the named instance for the MSG file. It is used to get a list
-        # of all available properties.
-        self.__named : extract_msg.Named = None
-        self.__attachments = None
-
-        self.ui.tableNamedProperties.cellDoubleClicked.connect(self._cellDoubleClicked)
-        self.ui.comboBoxInstance.currentTextChanged.connect(self._comboBoxChanged)
-
-    def loadNamed(self):
-        """
-        Load the named properties instance. This loads the main sections for each
-        property, not the data.
-        """
-        self.ui.tableNamedProperties.setRowCount(len(self.__named))
-        self.ui.tableNamedProperties.setSortingEnabled(False)
-        for index, key in enumerate(self.__named):
-            self.ui.tableNamedProperties.setItem(index, 0, QTableWidgetItem(key[0]))
-            self.ui.tableNamedProperties.setItem(index, 1, QTableWidgetItem(key[1]))
-            self.ui.tableNamedProperties.setItem(index, 2, NamedPIDItem(str(self.__named[key].namedPropertyID)))
-        self.ui.tableNamedProperties.setSortingEnabled(True)
-
-    @Slot()
-    def msgClosed(self):
-        self.ui.comboBoxInstance.clear()
-        self.ui.tableNamedProperties.clearContents()
-        self.ui.tableNamedProperties.setRowCount(0)
-        self.__msg = None
-        self.__named = None
-        self.__attachments = None
-
-    @Slot(extract_msg.MSGFile)
-    def msgOpened(self, msgFile):
-        self.__loading = True
-        self.__msg = msgFile
-        self.__named = msgFile.named
-        self.__attachments = msgFile._rawAttachments if isinstance(msgFile, extract_msg.MessageSignedBase) else msgFile.attachments
-        self.ui.comboBoxInstance.addItem('MSG File')
-        self.ui.comboBoxInstance.addItems((f'Attachment {x}' for x in range(len(self.__attachments))))
-        self.loadNamed()
-        self.__loading = False
-        self._comboBoxChanged('MSG File')
-
-    @Slot(int, int)
-    def _cellDoubleClicked(self, row, column):
-        if self.ui.tableNamedProperties.item(row, 3).data(0) == '[Stream]':
-            name = self.ui.tableNamedProperties.item(row, 0).data(0)
-            code = 0x8000 + int(self.ui.tableNamedProperties.item(row, 2).data(0))
-            if self.ui.comboBoxInstance.currentText() == 'MSG File':
-                start = ['']
-            else:
-                start = [f'__attach_version1.0_#{int(self.ui.comboBoxInstance.currentText().split(" ")[1]):08X}', '']
-
-            # Now we need to determine the type so we can generate the
-            # path to give to the signal.
-            for _type in extract_msg.constants.PTYPES:
-                start[-1] = f'__substg1.0_{code:04X}{_type:04X}'
-                logger.info(f'Checking for named property stream at {start}')
-                if self.__msg.exists(start):
-                    return self.namedPropertySelected.emit(start)
-            else:
-                QMessageBox.information(self, 'Notice', 'Stream for property was not found.')
-
-    @Slot(str)
-    def _comboBoxChanged(self, entry):
-        # Prevent this from running while data is being loaded.
-        if self.__loading:
-            return
-        if entry:
-            if entry == 'MSG File':
-                getData = self.__msg.namedProperties.get
-                getStream = self.__msg._getTypedStream
-            else:
-                attachment = self.__attachments[int(entry.split(' ')[-1])]
-                getData = attachment.namedProperties.get
-                getStream = attachment._getTypedStream
-
-            self.ui.tableNamedProperties.setSortingEnabled(False)
-            for index in range(self.ui.tableNamedProperties.rowCount()):
-                key = (self.ui.tableNamedProperties.item(index, 0).data(0),
-                       self.ui.tableNamedProperties.item(index, 1).data(0))
-                # We need to figure out what to display for the data.
-                data = getData(self.__named[key])
-                if isinstance(data, (int, float, bool, None.__class__)):
-                    # This helps to shortcut a bunch of properties.
-                    self.ui.tableNamedProperties.setItem(index, 3, QTableWidgetItem(utils.dataToString(data)))
-                elif isinstance(data, (bytes, list, tuple)) or getStream(f'__substg1.0_{self.__named[key].propertyStreamID}')[0]:
-                    self.ui.tableNamedProperties.setItem(index, 3, QTableWidgetItem('[Stream]'))
-                else:
-                    self.ui.tableNamedProperties.setItem(index, 3, QTableWidgetItem(utils.dataToString(data)))
-            self.ui.tableNamedProperties.setSortingEnabled(True)
-
-
-
+# This Python file uses the following encoding: utf-8
+import logging
+
+import extract_msg
+
+from PySide6 import QtCore
+from PySide6 import QtWidgets
+from PySide6.QtCore import Signal, SIGNAL, Slot, SLOT
+from PySide6.QtWidgets import QMessageBox, QTableWidgetItem
+
+from . import utils
+from .ui.ui_named_properties_viewer import Ui_NamedPropertiesViewer
+
+
+logger = logging.getLogger(__name__)
+logger.addHandler(logging.NullHandler())
+
+
+class NamedPIDItem(QTableWidgetItem):
+    """
+    Little bit of a hack to force the Named PID column to sort properly.
+    """
+    def __lt__(self, item):
+        return int(self.data(0)) < int(item.data(0))
+
+
+
+class NamedPropertiesViewer(QtWidgets.QWidget):
+    namedPropertySelected = Signal(list)
+    def __init__(self, parent = None):
+        super().__init__(parent)
+        
+        self.ui = Ui_NamedPropertiesViewer()
+        self.ui.setupUi(self)
+        self.__loading = False
+        self.__msg = None
+        # This is the named instance for the MSG file. It is used to get a list
+        # of all available properties.
+        self.__named : extract_msg.Named = None
+        self.__attachments = None
+
+        self.ui.tableNamedProperties.cellDoubleClicked.connect(self._cellDoubleClicked)
+        self.ui.comboBoxInstance.currentTextChanged.connect(self._comboBoxChanged)
+
+    def loadNamed(self):
+        """
+        Load the named properties instance. This loads the main sections for each
+        property, not the data.
+        """
+        self.ui.tableNamedProperties.setRowCount(len(self.__named))
+        self.ui.tableNamedProperties.setSortingEnabled(False)
+        for index, key in enumerate(self.__named):
+            self.ui.tableNamedProperties.setItem(index, 0, QTableWidgetItem(key[0]))
+            self.ui.tableNamedProperties.setItem(index, 1, QTableWidgetItem(key[1]))
+            self.ui.tableNamedProperties.setItem(index, 2, NamedPIDItem(str(self.__named[key].namedPropertyID)))
+        self.ui.tableNamedProperties.setSortingEnabled(True)
+
+    @Slot()
+    def msgClosed(self):
+        self.ui.comboBoxInstance.clear()
+        self.ui.tableNamedProperties.clearContents()
+        self.ui.tableNamedProperties.setRowCount(0)
+        self.__msg = None
+        self.__named = None
+        self.__attachments = None
+
+    @Slot(extract_msg.MSGFile)
+    def msgOpened(self, msgFile):
+        self.__loading = True
+        self.__msg = msgFile
+        self.__named = msgFile.named
+        self.__attachments = msgFile._rawAttachments if isinstance(msgFile, extract_msg.MessageSignedBase) else msgFile.attachments
+        self.ui.comboBoxInstance.addItem('MSG File')
+        self.ui.comboBoxInstance.addItems((f'Attachment {x}' for x in range(len(self.__attachments))))
+        self.loadNamed()
+        self.__loading = False
+        self._comboBoxChanged('MSG File')
+
+    @Slot(int, int)
+    def _cellDoubleClicked(self, row, column):
+        if self.ui.tableNamedProperties.item(row, 3).data(0) == '[Stream]':
+            name = self.ui.tableNamedProperties.item(row, 0).data(0)
+            code = 0x8000 + int(self.ui.tableNamedProperties.item(row, 2).data(0))
+            if self.ui.comboBoxInstance.currentText() == 'MSG File':
+                start = ['']
+            else:
+                start = [f'__attach_version1.0_#{int(self.ui.comboBoxInstance.currentText().split(" ")[1]):08X}', '']
+
+            # Now we need to determine the type so we can generate the
+            # path to give to the signal.
+            for _type in extract_msg.constants.PTYPES:
+                start[-1] = f'__substg1.0_{code:04X}{_type:04X}'
+                logger.info(f'Checking for named property stream at {start}')
+                if self.__msg.exists(start):
+                    return self.namedPropertySelected.emit(start)
+            else:
+                QMessageBox.information(self, 'Notice', 'Stream for property was not found.')
+
+    @Slot(str)
+    def _comboBoxChanged(self, entry):
+        # Prevent this from running while data is being loaded.
+        if self.__loading:
+            return
+        if entry:
+            if entry == 'MSG File':
+                getData = self.__msg.namedProperties.get
+                getStream = self.__msg._getTypedStream
+            else:
+                attachment = self.__attachments[int(entry.split(' ')[-1])]
+                getData = attachment.namedProperties.get
+                getStream = attachment._getTypedStream
+
+            self.ui.tableNamedProperties.setSortingEnabled(False)
+            for index in range(self.ui.tableNamedProperties.rowCount()):
+                key = (self.ui.tableNamedProperties.item(index, 0).data(0),
+                       self.ui.tableNamedProperties.item(index, 1).data(0))
+                # We need to figure out what to display for the data.
+                data = getData(self.__named[key])
+                if isinstance(data, (int, float, bool, None.__class__)):
+                    # This helps to shortcut a bunch of properties.
+                    self.ui.tableNamedProperties.setItem(index, 3, QTableWidgetItem(utils.dataToString(data)))
+                elif isinstance(data, (bytes, list, tuple)) or getStream(f'__substg1.0_{self.__named[key].propertyStreamID}')[0]:
+                    self.ui.tableNamedProperties.setItem(index, 3, QTableWidgetItem('[Stream]'))
+                else:
+                    self.ui.tableNamedProperties.setItem(index, 3, QTableWidgetItem(utils.dataToString(data)))
+            self.ui.tableNamedProperties.setSortingEnabled(True)
+
+
+
```

### Comparing `msg_explorer-1.6.0/msg_explorer/properties_viewer.py` & `msg_explorer-1.7.0/msg_explorer/properties_viewer.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,55 +1,55 @@
-# This Python file uses the following encoding: utf-8
-import extract_msg
-
-from PySide6 import QtCore
-from PySide6 import QtWidgets
-from PySide6.QtCore import Signal, SIGNAL, Slot, SLOT
-
-from . import utils
-from .ui.ui_properties_viewer import Ui_PropertiesViewer
-
-
-_DISPLAY_PROPS = (
-    '0000',
-    '0001',
-    '0002',
-    '0003',
-    '0004',
-    '0005',
-    '0006',
-    '0007',
-    '000A',
-    '000B',
-    '0014',
-    '0040',
-    '0048',
-    '00FB',
-    '00FD',
-    '00FE',
-)
-
-
-class PropertiesViewer(QtWidgets.QWidget):
-    def __init__(self, parent = None):
-        super().__init__(parent)
-        
-        self.ui = Ui_PropertiesViewer()
-        self.ui.setupUi(self)
-
-    @Slot()
-    def clear(self):
-        pass
-
-    @Slot(extract_msg.Properties)
-    def loadProperties(self, props):
-        # We don't really need to load all of the properties,
-        # so just load all of the relevant ones.
-        self.ui.tableProps.clearContents()
-        count = 0
-        for prop in sorted(props.keys()):
-            if prop[4:] in _DISPLAY_PROPS:
-                count += 1
-                self.ui.tableProps.setRowCount(count)
-                self.ui.tableProps.setItem(count - 1, 0, QtWidgets.QTableWidgetItem(prop[:4]))
-                self.ui.tableProps.setItem(count - 1, 1, QtWidgets.QTableWidgetItem(prop[4:]))
-                self.ui.tableProps.setItem(count - 1, 2, QtWidgets.QTableWidgetItem(utils.dataToString(props[prop].value)))
+# This Python file uses the following encoding: utf-8
+import extract_msg
+
+from PySide6 import QtCore
+from PySide6 import QtWidgets
+from PySide6.QtCore import Signal, SIGNAL, Slot, SLOT
+
+from . import utils
+from .ui.ui_properties_viewer import Ui_PropertiesViewer
+
+
+_DISPLAY_PROPS = (
+    '0000',
+    '0001',
+    '0002',
+    '0003',
+    '0004',
+    '0005',
+    '0006',
+    '0007',
+    '000A',
+    '000B',
+    '0014',
+    '0040',
+    '0048',
+    '00FB',
+    '00FD',
+    '00FE',
+)
+
+
+class PropertiesViewer(QtWidgets.QWidget):
+    def __init__(self, parent = None):
+        super().__init__(parent)
+        
+        self.ui = Ui_PropertiesViewer()
+        self.ui.setupUi(self)
+
+    @Slot()
+    def clear(self):
+        pass
+
+    @Slot(extract_msg.Properties)
+    def loadProperties(self, props):
+        # We don't really need to load all of the properties,
+        # so just load all of the relevant ones.
+        self.ui.tableProps.clearContents()
+        count = 0
+        for prop in sorted(props.keys()):
+            if prop[4:] in _DISPLAY_PROPS:
+                count += 1
+                self.ui.tableProps.setRowCount(count)
+                self.ui.tableProps.setItem(count - 1, 0, QtWidgets.QTableWidgetItem(prop[:4]))
+                self.ui.tableProps.setItem(count - 1, 1, QtWidgets.QTableWidgetItem(prop[4:]))
+                self.ui.tableProps.setItem(count - 1, 2, QtWidgets.QTableWidgetItem(utils.dataToString(props[prop].value)))
```

### Comparing `msg_explorer-1.6.0/msg_explorer/stream_viewer.py` & `msg_explorer-1.7.0/msg_explorer/stream_viewer.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,166 +1,166 @@
-# This Python file uses the following encoding: utf-8
-import copy
-import logging
-import sys
-
-import extract_msg
-
-from PySide6 import QtCore
-from PySide6 import QtWidgets
-from PySide6.QtCore import Signal, SIGNAL, Slot, SLOT
-
-from . import constants, utils
-from .ui.ui_stream_viewer import Ui_StreamViewer
-
-
-logger = logging.getLogger(__name__)
-logger.addHandler(logging.NullHandler())
-
-
-class StreamViewer(QtWidgets.QWidget):
-    def __init__(self, parent = None):
-        super().__init__(parent)
-
-        self.ui = Ui_StreamViewer()
-        self.ui.setupUi(self)
-        self.__msg = None
-        self.__dataViewerPage = None
-
-        self.ui.buttonParsedView.toggled.connect(self._changeViewType)
-
-        self.__currentPage = self.ui.pageParsedNoData
-
-        self.__typePages = {
-            'prop': self.ui.pageParsedProperties,
-            '001E': self.ui.pageParsedString,
-            '001F': self.ui.pageParsedString,
-            '0048': self.ui.pageParsedGuidViewer,
-            '0102': self.ui.pageHexViewer,
-            '1002': self.ui.pageParsedMultiple,
-            '1003': self.ui.pageParsedMultiple,
-            '1004': self.ui.pageParsedMultiple,
-            '1005': self.ui.pageParsedMultiple,
-            '1006': self.ui.pageParsedMultiple,
-            '1007': self.ui.pageParsedMultiple,
-            '1014': self.ui.pageParsedMultiple,
-            '101E': self.ui.pageParsedMultiple,
-            '101F': self.ui.pageParsedMultiple,
-            '1040': self.ui.pageParsedMultiple,
-            '1048': self.ui.pageParsedMultiple,
-            '1102': self.ui.pageParsedMultipleBinary,
-        }
-
-    @Slot()
-    def _changeViewType(self):
-        """
-        Change the view type when the radio buttons are changed.
-        """
-        if self.ui.buttonParsedView.isChecked():
-            self.ui.stackedWidget.setCurrentWidget(self.__currentPage)
-        else:
-            self.ui.stackedWidget.setCurrentWidget(self.ui.pageHexViewer)
-
-    @Slot()
-    def msgClosed(self):
-        """
-        Clean up the data when the msg file is closed.
-        """
-        self.__msg = None
-        self.ui.labelStreamName.setText('None')
-        self.ui.pageHexViewer.clear()
-        if self.__currentPage != self.ui.pageParsedNoData:
-            self.__currentPage.clear()
-            self.__currentPage = self.ui.pageParsedNoData
-        self._changeViewType()
-
-    @Slot(extract_msg.msg.MSGFile)
-    def msgOpened(self, msgFile):
-        self.__msg = msgFile
-
-    @Slot(list)
-    def openStream(self, name, prefix = True):
-        """
-        Loads the data for the specified stream. Will automatically
-        determine how best to show it.
-        """
-        name = self.__msg.fixPath(name, prefix).split('/')
-        # First thing is first, handle a multiple stream part being selected.
-        if len(name[-1]) == 29:
-            # A multiple stream part has 9 extra characters on the name. We are
-            # just telling the function to run again with the main stream.
-            return self.openStream(name[:-1] + [name[-1][:-9]])
-
-        self.ui.pageHexViewer.loadHexData(self.__msg._getStream(name, False))
-        # Make sure the path we use is local to the current file.
-        self.ui.labelStreamName.setText('/'.join(name[self.__msg.prefixLen:]))
-        # Now determine how to load the rest of the data.
-        if name[-1] == '__properties_version1.0':
-            _type = 'prop'
-            source = self.__msg
-            # Second part is to cut out the prefix for traversal.
-            path = name[self.__msg.prefixLen:]
-            # This is necessary for some operations.
-            currentPath = []
-
-            try:
-                while len(path) > 1:
-                    if path[0].startswith('__attach'):
-                        source = source.attachments[int(path[0][-8:], 16)]
-                    elif path[0].startswith('__recip'):
-                        if isinstance(self.__msg, extract_msg.message_base.MessageBase):
-                            # If it is a message base then the recipients already exist.
-                            source = source.recipients[int(path[0][-8:], 16)]
-                        else:
-                            # Otherwise, they do not and we need to create one.
-                            source = extract_msg.recipient.Recipient(currentPath + [path[0]], source)
-                    elif path[0] == '__substg1.0_3701000D':
-                        source = source.data
-                    currentPath.append(path.pop(0))
-            except Exception as e:
-                utils.displayException(e)
-                return
-            props = source.props
-            self.ui.pageParsedProperties.loadProperties(props)
-        else:
-            _type = name[-1][-4:]
-            path = name[:-1] + [name[-1][:-4]]
-            if constants.RE_STANDARD_FILE.match(name[-1]):
-                data = self.__msg._getTypedStream(path, False, _type)[1]
-                if _type in ('001E', '001F'): # String.
-                    self.ui.pageParsedString.loadString(data, _type)
-                elif _type == '0048': # GUID.
-                    self.ui.pageParsedGuidViewer.loadGuid(data)
-                elif _type == '0102': # Binary.
-                    # For binary, we just show the hex viewer.
-                    pass
-                elif _type == '1102': # Multiple Binary.
-                    # For multiple binary we load a page with a list
-                    # of entries and a hex viewer that shows the
-                    # currently selected one.
-                    self.ui.pageParsedMultipleBinary.loadMultiple(data)
-                elif _type.startswith('1'): # Other multiples.
-                    self.ui.pageParsedMultiple.loadMultiple(data, _type)
-
-        # First, check to make sure we are not opening a special custom attachment
-        # file. If we are, this regular expression won't match it, and we just
-        # treat it as binary data.
-        if constants.RE_STANDARD_FILE.match(name[-1]):
-            try:
-                self.__currentPage = self.__typePages[_type]
-            except KeyError as e:
-                utils.displayException(e)
-        else:
-            logger.info(f'Attempting to view non-standard stream "{"/".join(name)}". Interpretting as plain binary data.')
-            self.__currentPage = self.ui.pageHexViewer
-        self._changeViewType()
-
-    @Slot(str, bytes)
-    def openStreamBytes(self, name : str, data : bytes):
-        """
-        Open a stream, overriding the behavior used for handling it. Used for
-        displaying streams that are not accessible through normal means.
-        """
-        self.__currentPage = self.__typePages['0102']
-        self.ui.labelStreamName = name
-        self.ui.pageHexViewer.loadHexData(data)
-        self._changeViewType()
+# This Python file uses the following encoding: utf-8
+import copy
+import logging
+import sys
+
+import extract_msg
+
+from PySide6 import QtCore
+from PySide6 import QtWidgets
+from PySide6.QtCore import Signal, SIGNAL, Slot, SLOT
+
+from . import constants, utils
+from .ui.ui_stream_viewer import Ui_StreamViewer
+
+
+logger = logging.getLogger(__name__)
+logger.addHandler(logging.NullHandler())
+
+
+class StreamViewer(QtWidgets.QWidget):
+    def __init__(self, parent = None):
+        super().__init__(parent)
+
+        self.ui = Ui_StreamViewer()
+        self.ui.setupUi(self)
+        self.__msg = None
+        self.__dataViewerPage = None
+
+        self.ui.buttonParsedView.toggled.connect(self._changeViewType)
+
+        self.__currentPage = self.ui.pageParsedNoData
+
+        self.__typePages = {
+            'prop': self.ui.pageParsedProperties,
+            '001E': self.ui.pageParsedString,
+            '001F': self.ui.pageParsedString,
+            '0048': self.ui.pageParsedGuidViewer,
+            '0102': self.ui.pageHexViewer,
+            '1002': self.ui.pageParsedMultiple,
+            '1003': self.ui.pageParsedMultiple,
+            '1004': self.ui.pageParsedMultiple,
+            '1005': self.ui.pageParsedMultiple,
+            '1006': self.ui.pageParsedMultiple,
+            '1007': self.ui.pageParsedMultiple,
+            '1014': self.ui.pageParsedMultiple,
+            '101E': self.ui.pageParsedMultiple,
+            '101F': self.ui.pageParsedMultiple,
+            '1040': self.ui.pageParsedMultiple,
+            '1048': self.ui.pageParsedMultiple,
+            '1102': self.ui.pageParsedMultipleBinary,
+        }
+
+    @Slot()
+    def _changeViewType(self):
+        """
+        Change the view type when the radio buttons are changed.
+        """
+        if self.ui.buttonParsedView.isChecked():
+            self.ui.stackedWidget.setCurrentWidget(self.__currentPage)
+        else:
+            self.ui.stackedWidget.setCurrentWidget(self.ui.pageHexViewer)
+
+    @Slot()
+    def msgClosed(self):
+        """
+        Clean up the data when the msg file is closed.
+        """
+        self.__msg = None
+        self.ui.labelStreamName.setText('None')
+        self.ui.pageHexViewer.clear()
+        if self.__currentPage != self.ui.pageParsedNoData:
+            self.__currentPage.clear()
+            self.__currentPage = self.ui.pageParsedNoData
+        self._changeViewType()
+
+    @Slot(extract_msg.msg.MSGFile)
+    def msgOpened(self, msgFile):
+        self.__msg = msgFile
+
+    @Slot(list)
+    def openStream(self, name, prefix = True):
+        """
+        Loads the data for the specified stream. Will automatically
+        determine how best to show it.
+        """
+        name = self.__msg.fixPath(name, prefix).split('/')
+        # First thing is first, handle a multiple stream part being selected.
+        if len(name[-1]) == 29:
+            # A multiple stream part has 9 extra characters on the name. We are
+            # just telling the function to run again with the main stream.
+            return self.openStream(name[:-1] + [name[-1][:-9]])
+
+        self.ui.pageHexViewer.loadHexData(self.__msg._getStream(name, False))
+        # Make sure the path we use is local to the current file.
+        self.ui.labelStreamName.setText('/'.join(name[self.__msg.prefixLen:]))
+        # Now determine how to load the rest of the data.
+        if name[-1] == '__properties_version1.0':
+            _type = 'prop'
+            source = self.__msg
+            # Second part is to cut out the prefix for traversal.
+            path = name[self.__msg.prefixLen:]
+            # This is necessary for some operations.
+            currentPath = []
+
+            try:
+                while len(path) > 1:
+                    if path[0].startswith('__attach'):
+                        source = source.attachments[int(path[0][-8:], 16)]
+                    elif path[0].startswith('__recip'):
+                        if isinstance(self.__msg, extract_msg.message_base.MessageBase):
+                            # If it is a message base then the recipients already exist.
+                            source = source.recipients[int(path[0][-8:], 16)]
+                        else:
+                            # Otherwise, they do not and we need to create one.
+                            source = extract_msg.recipient.Recipient(currentPath + [path[0]], source)
+                    elif path[0] == '__substg1.0_3701000D':
+                        source = source.data
+                    currentPath.append(path.pop(0))
+            except Exception as e:
+                utils.displayException(e)
+                return
+            props = source.props
+            self.ui.pageParsedProperties.loadProperties(props)
+        else:
+            _type = name[-1][-4:]
+            path = name[:-1] + [name[-1][:-4]]
+            if constants.RE_STANDARD_FILE.match(name[-1]):
+                data = self.__msg._getTypedStream(path, False, _type)[1]
+                if _type in ('001E', '001F'): # String.
+                    self.ui.pageParsedString.loadString(data, _type)
+                elif _type == '0048': # GUID.
+                    self.ui.pageParsedGuidViewer.loadGuid(data)
+                elif _type == '0102': # Binary.
+                    # For binary, we just show the hex viewer.
+                    pass
+                elif _type == '1102': # Multiple Binary.
+                    # For multiple binary we load a page with a list
+                    # of entries and a hex viewer that shows the
+                    # currently selected one.
+                    self.ui.pageParsedMultipleBinary.loadMultiple(data)
+                elif _type.startswith('1'): # Other multiples.
+                    self.ui.pageParsedMultiple.loadMultiple(data, _type)
+
+        # First, check to make sure we are not opening a special custom attachment
+        # file. If we are, this regular expression won't match it, and we just
+        # treat it as binary data.
+        if constants.RE_STANDARD_FILE.match(name[-1]):
+            try:
+                self.__currentPage = self.__typePages[_type]
+            except KeyError as e:
+                utils.displayException(e)
+        else:
+            logger.info(f'Attempting to view non-standard stream "{"/".join(name)}". Interpretting as plain binary data.')
+            self.__currentPage = self.ui.pageHexViewer
+        self._changeViewType()
+
+    @Slot(str, bytes)
+    def openStreamBytes(self, name : str, data : bytes):
+        """
+        Open a stream, overriding the behavior used for handling it. Used for
+        displaying streams that are not accessible through normal means.
+        """
+        self.__currentPage = self.__typePages['0102']
+        self.ui.labelStreamName = name
+        self.ui.pageHexViewer.loadHexData(data)
+        self._changeViewType()
```

### Comparing `msg_explorer-1.6.0/msg_explorer/ui/guid_viewer.ui` & `msg_explorer-1.7.0/msg_explorer/ui/logger_widget.ui`

 * *Files 22% similar despite different names*

#### Comparing `msg_explorer-1.6.0/msg_explorer/ui/guid_viewer.ui` & `msg_explorer-1.7.0/msg_explorer/ui/logger_widget.ui`

```diff
@@ -1,30 +1,30 @@
 <?xml version="1.0" encoding="utf-8"?>
 <ui version="4.0">
-  <class>GuidViewer</class>
-  <widget class="QWidget" name="GuidViewer">
+  <class>LoggerWidget</class>
+  <widget class="QWidget" name="LoggerWidget">
     <property name="geometry">
       <rect>
         <x>0</x>
         <y>0</y>
         <width>800</width>
         <height>600</height>
       </rect>
     </property>
     <property name="windowTitle">
-      <string>GuidViewer</string>
+      <string>LoggerWidget</string>
     </property>
     <layout class="QGridLayout" name="gridLayout">
       <item row="0" column="0">
-        <widget class="QLabel" name="labelGuid">
-          <property name="text">
-            <string>TextLabel</string>
+        <widget class="QListWidget" name="listLog">
+          <property name="verticalScrollMode">
+            <enum>QAbstractItemView::ScrollPerPixel</enum>
           </property>
-          <property name="alignment">
-            <set>Qt::AlignCenter</set>
+          <property name="horizontalScrollMode">
+            <enum>QAbstractItemView::ScrollPerPixel</enum>
           </property>
         </widget>
       </item>
     </layout>
   </widget>
   <resources/>
   <connections/>
```

### Comparing `msg_explorer-1.6.0/msg_explorer/ui/hex_viewer.ui` & `msg_explorer-1.7.0/msg_explorer/ui/hex_viewer.ui`

 * *Format-specific differences are supported for XML files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: XML 1.0 document, ASCII text, with CRLF line terminators*

 * *Files 17% similar despite different names*

```diff
@@ -1,61 +1,59 @@
 00000000: 3c3f 786d 6c20 7665 7273 696f 6e3d 2231  <?xml version="1
 00000010: 2e30 2220 656e 636f 6469 6e67 3d22 5554  .0" encoding="UT
-00000020: 462d 3822 3f3e 0d0a 3c75 6920 7665 7273  F-8"?>..<ui vers
-00000030: 696f 6e3d 2234 2e30 223e 0d0a 203c 636c  ion="4.0">.. <cl
-00000040: 6173 733e 4865 7856 6965 7765 723c 2f63  ass>HexViewer</c
-00000050: 6c61 7373 3e0d 0a20 3c77 6964 6765 7420  lass>.. <widget 
-00000060: 636c 6173 733d 2251 5769 6467 6574 2220  class="QWidget" 
-00000070: 6e61 6d65 3d22 4865 7856 6965 7765 7222  name="HexViewer"
-00000080: 3e0d 0a20 203c 7072 6f70 6572 7479 206e  >..  <property n
-00000090: 616d 653d 2267 656f 6d65 7472 7922 3e0d  ame="geometry">.
-000000a0: 0a20 2020 3c72 6563 743e 0d0a 2020 2020  .   <rect>..    
-000000b0: 3c78 3e30 3c2f 783e 0d0a 2020 2020 3c79  <x>0</x>..    <y
-000000c0: 3e30 3c2f 793e 0d0a 2020 2020 3c77 6964  >0</y>..    <wid
-000000d0: 7468 3e38 3030 3c2f 7769 6474 683e 0d0a  th>800</width>..
-000000e0: 2020 2020 3c68 6569 6768 743e 3630 303c      <height>600<
-000000f0: 2f68 6569 6768 743e 0d0a 2020 203c 2f72  /height>..   </r
-00000100: 6563 743e 0d0a 2020 3c2f 7072 6f70 6572  ect>..  </proper
-00000110: 7479 3e0d 0a20 203c 7072 6f70 6572 7479  ty>..  <property
-00000120: 206e 616d 653d 2277 696e 646f 7754 6974   name="windowTit
-00000130: 6c65 223e 0d0a 2020 203c 7374 7269 6e67  le">..   <string
-00000140: 3e48 6578 5669 6577 6572 3c2f 7374 7269  >HexViewer</stri
-00000150: 6e67 3e0d 0a20 203c 2f70 726f 7065 7274  ng>..  </propert
-00000160: 793e 0d0a 2020 3c6c 6179 6f75 7420 636c  y>..  <layout cl
-00000170: 6173 733d 2251 4772 6964 4c61 796f 7574  ass="QGridLayout
-00000180: 2220 6e61 6d65 3d22 6772 6964 4c61 796f  " name="gridLayo
-00000190: 7574 223e 0d0a 2020 203c 6974 656d 2072  ut">..   <item r
-000001a0: 6f77 3d22 3022 2063 6f6c 756d 6e3d 2230  ow="0" column="0
-000001b0: 223e 0d0a 2020 2020 3c77 6964 6765 7420  ">..    <widget 
-000001c0: 636c 6173 733d 2251 5465 7874 4564 6974  class="QTextEdit
-000001d0: 2220 6e61 6d65 3d22 6865 7856 6965 7765  " name="hexViewe
-000001e0: 7222 3e0d 0a20 2020 2020 3c70 726f 7065  r">..     <prope
-000001f0: 7274 7920 6e61 6d65 3d22 666f 6e74 223e  rty name="font">
-00000200: 0d0a 2020 2020 2020 3c66 6f6e 743e 0d0a  ..      <font>..
-00000210: 2020 2020 2020 203c 6661 6d69 6c79 3e43         <family>C
-00000220: 6f6e 736f 6c61 733c 2f66 616d 696c 793e  onsolas</family>
-00000230: 0d0a 2020 2020 2020 203c 706f 696e 7473  ..       <points
-00000240: 697a 653e 393c 2f70 6f69 6e74 7369 7a65  ize>9</pointsize
-00000250: 3e0d 0a20 2020 2020 203c 2f66 6f6e 743e  >..      </font>
-00000260: 0d0a 2020 2020 203c 2f70 726f 7065 7274  ..     </propert
-00000270: 793e 0d0a 2020 2020 203c 7072 6f70 6572  y>..     <proper
-00000280: 7479 206e 616d 653d 2275 6e64 6f52 6564  ty name="undoRed
-00000290: 6f45 6e61 626c 6564 223e 0d0a 2020 2020  oEnabled">..    
-000002a0: 2020 3c62 6f6f 6c3e 6661 6c73 653c 2f62    <bool>false</b
-000002b0: 6f6f 6c3e 0d0a 2020 2020 203c 2f70 726f  ool>..     </pro
-000002c0: 7065 7274 793e 0d0a 2020 2020 203c 7072  perty>..     <pr
-000002d0: 6f70 6572 7479 206e 616d 653d 226c 696e  operty name="lin
-000002e0: 6557 7261 704d 6f64 6522 3e0d 0a20 2020  eWrapMode">..   
-000002f0: 2020 203c 656e 756d 3e51 5465 7874 4564     <enum>QTextEd
-00000300: 6974 3a3a 4e6f 5772 6170 3c2f 656e 756d  it::NoWrap</enum
-00000310: 3e0d 0a20 2020 2020 3c2f 7072 6f70 6572  >..     </proper
-00000320: 7479 3e0d 0a20 2020 2020 3c70 726f 7065  ty>..     <prope
-00000330: 7274 7920 6e61 6d65 3d22 7265 6164 4f6e  rty name="readOn
-00000340: 6c79 223e 0d0a 2020 2020 2020 3c62 6f6f  ly">..      <boo
-00000350: 6c3e 7472 7565 3c2f 626f 6f6c 3e0d 0a20  l>true</bool>.. 
-00000360: 2020 2020 3c2f 7072 6f70 6572 7479 3e0d      </property>.
-00000370: 0a20 2020 203c 2f77 6964 6765 743e 0d0a  .    </widget>..
-00000380: 2020 203c 2f69 7465 6d3e 0d0a 2020 3c2f     </item>..  </
-00000390: 6c61 796f 7574 3e0d 0a20 3c2f 7769 6467  layout>.. </widg
-000003a0: 6574 3e0d 0a20 3c72 6573 6f75 7263 6573  et>.. <resources
-000003b0: 2f3e 0d0a 203c 636f 6e6e 6563 7469 6f6e  />.. <connection
-000003c0: 732f 3e0d 0a3c 2f75 693e 0d0a            s/>..</ui>..
+00000020: 462d 3822 3f3e 0a3c 7569 2076 6572 7369  F-8"?>.<ui versi
+00000030: 6f6e 3d22 342e 3022 3e0a 203c 636c 6173  on="4.0">. <clas
+00000040: 733e 4865 7856 6965 7765 723c 2f63 6c61  s>HexViewer</cla
+00000050: 7373 3e0a 203c 7769 6467 6574 2063 6c61  ss>. <widget cla
+00000060: 7373 3d22 5157 6964 6765 7422 206e 616d  ss="QWidget" nam
+00000070: 653d 2248 6578 5669 6577 6572 223e 0a20  e="HexViewer">. 
+00000080: 203c 7072 6f70 6572 7479 206e 616d 653d   <property name=
+00000090: 2267 656f 6d65 7472 7922 3e0a 2020 203c  "geometry">.   <
+000000a0: 7265 6374 3e0a 2020 2020 3c78 3e30 3c2f  rect>.    <x>0</
+000000b0: 783e 0a20 2020 203c 793e 303c 2f79 3e0a  x>.    <y>0</y>.
+000000c0: 2020 2020 3c77 6964 7468 3e38 3030 3c2f      <width>800</
+000000d0: 7769 6474 683e 0a20 2020 203c 6865 6967  width>.    <heig
+000000e0: 6874 3e36 3030 3c2f 6865 6967 6874 3e0a  ht>600</height>.
+000000f0: 2020 203c 2f72 6563 743e 0a20 203c 2f70     </rect>.  </p
+00000100: 726f 7065 7274 793e 0a20 203c 7072 6f70  roperty>.  <prop
+00000110: 6572 7479 206e 616d 653d 2277 696e 646f  erty name="windo
+00000120: 7754 6974 6c65 223e 0a20 2020 3c73 7472  wTitle">.   <str
+00000130: 696e 673e 4865 7856 6965 7765 723c 2f73  ing>HexViewer</s
+00000140: 7472 696e 673e 0a20 203c 2f70 726f 7065  tring>.  </prope
+00000150: 7274 793e 0a20 203c 6c61 796f 7574 2063  rty>.  <layout c
+00000160: 6c61 7373 3d22 5147 7269 644c 6179 6f75  lass="QGridLayou
+00000170: 7422 206e 616d 653d 2267 7269 644c 6179  t" name="gridLay
+00000180: 6f75 7422 3e0a 2020 203c 6974 656d 2072  out">.   <item r
+00000190: 6f77 3d22 3022 2063 6f6c 756d 6e3d 2230  ow="0" column="0
+000001a0: 223e 0a20 2020 203c 7769 6467 6574 2063  ">.    <widget c
+000001b0: 6c61 7373 3d22 5154 6578 7445 6469 7422  lass="QTextEdit"
+000001c0: 206e 616d 653d 2268 6578 5669 6577 6572   name="hexViewer
+000001d0: 223e 0a20 2020 2020 3c70 726f 7065 7274  ">.     <propert
+000001e0: 7920 6e61 6d65 3d22 666f 6e74 223e 0a20  y name="font">. 
+000001f0: 2020 2020 203c 666f 6e74 3e0a 2020 2020       <font>.    
+00000200: 2020 203c 6661 6d69 6c79 3e43 6f6e 736f     <family>Conso
+00000210: 6c61 733c 2f66 616d 696c 793e 0a20 2020  las</family>.   
+00000220: 2020 2020 3c70 6f69 6e74 7369 7a65 3e39      <pointsize>9
+00000230: 3c2f 706f 696e 7473 697a 653e 0a20 2020  </pointsize>.   
+00000240: 2020 203c 2f66 6f6e 743e 0a20 2020 2020     </font>.     
+00000250: 3c2f 7072 6f70 6572 7479 3e0a 2020 2020  </property>.    
+00000260: 203c 7072 6f70 6572 7479 206e 616d 653d   <property name=
+00000270: 2275 6e64 6f52 6564 6f45 6e61 626c 6564  "undoRedoEnabled
+00000280: 223e 0a20 2020 2020 203c 626f 6f6c 3e66  ">.      <bool>f
+00000290: 616c 7365 3c2f 626f 6f6c 3e0a 2020 2020  alse</bool>.    
+000002a0: 203c 2f70 726f 7065 7274 793e 0a20 2020   </property>.   
+000002b0: 2020 3c70 726f 7065 7274 7920 6e61 6d65    <property name
+000002c0: 3d22 6c69 6e65 5772 6170 4d6f 6465 223e  ="lineWrapMode">
+000002d0: 0a20 2020 2020 203c 656e 756d 3e51 5465  .      <enum>QTe
+000002e0: 7874 4564 6974 3a3a 4e6f 5772 6170 3c2f  xtEdit::NoWrap</
+000002f0: 656e 756d 3e0a 2020 2020 203c 2f70 726f  enum>.     </pro
+00000300: 7065 7274 793e 0a20 2020 2020 3c70 726f  perty>.     <pro
+00000310: 7065 7274 7920 6e61 6d65 3d22 7265 6164  perty name="read
+00000320: 4f6e 6c79 223e 0a20 2020 2020 203c 626f  Only">.      <bo
+00000330: 6f6c 3e74 7275 653c 2f62 6f6f 6c3e 0a20  ol>true</bool>. 
+00000340: 2020 2020 3c2f 7072 6f70 6572 7479 3e0a      </property>.
+00000350: 2020 2020 3c2f 7769 6467 6574 3e0a 2020      </widget>.  
+00000360: 203c 2f69 7465 6d3e 0a20 203c 2f6c 6179   </item>.  </lay
+00000370: 6f75 743e 0a20 3c2f 7769 6467 6574 3e0a  out>. </widget>.
+00000380: 203c 7265 736f 7572 6365 732f 3e0a 203c   <resources/>. <
+00000390: 636f 6e6e 6563 7469 6f6e 732f 3e0a 3c2f  connections/>.</
+000003a0: 7569 3e0a                                ui>.
```

### Comparing `msg_explorer-1.6.0/msg_explorer/ui/loading_screen.ui` & `msg_explorer-1.7.0/msg_explorer/ui/named_properties_viewer.ui`

 * *Files 26% similar despite different names*

#### Comparing `msg_explorer-1.6.0/msg_explorer/ui/loading_screen.ui` & `msg_explorer-1.7.0/msg_explorer/ui/named_properties_viewer.ui`

```diff
@@ -1,44 +1,63 @@
 <?xml version="1.0" encoding="utf-8"?>
 <ui version="4.0">
-  <class>LoadingScreen</class>
-  <widget class="QWidget" name="LoadingScreen">
+  <class>NamedPropertiesViewer</class>
+  <widget class="QWidget" name="NamedPropertiesViewer">
     <property name="geometry">
       <rect>
         <x>0</x>
         <y>0</y>
-        <width>400</width>
-        <height>150</height>
+        <width>800</width>
+        <height>600</height>
       </rect>
     </property>
     <property name="windowTitle">
-      <string>Loading...</string>
+      <string>NamedPropertiesViewer</string>
     </property>
     <layout class="QGridLayout" name="gridLayout">
-      <item row="0" column="0">
-        <widget class="QLabel" name="loadingMessage">
-          <property name="layoutDirection">
-            <enum>Qt::LeftToRight</enum>
-          </property>
-          <property name="text">
-            <string>Loading MSG file, please wait...</string>
+      <item row="1" column="0">
+        <widget class="QTableWidget" name="tableNamedProperties">
+          <property name="editTriggers">
+            <set>QAbstractItemView::NoEditTriggers</set>
           </property>
-          <property name="alignment">
-            <set>Qt::AlignCenter</set>
+          <property name="verticalScrollMode">
+            <enum>QAbstractItemView::ScrollPerPixel</enum>
           </property>
-        </widget>
-      </item>
-      <item row="1" column="0">
-        <widget class="QProgressBar" name="progressBar">
-          <property name="maximum">
-            <number>0</number>
+          <property name="horizontalScrollMode">
+            <enum>QAbstractItemView::ScrollPerPixel</enum>
           </property>
-          <property name="value">
-            <number>-1</number>
+          <property name="sortingEnabled">
+            <bool>true</bool>
           </property>
+          <attribute name="horizontalHeaderDefaultSectionSize">
+            <number>300</number>
+          </attribute>
+          <column>
+            <property name="text">
+              <string>Property ID</string>
+            </property>
+          </column>
+          <column>
+            <property name="text">
+              <string>Property Set GUID</string>
+            </property>
+          </column>
+          <column>
+            <property name="text">
+              <string>Named PID</string>
+            </property>
+          </column>
+          <column>
+            <property name="text">
+              <string>Data</string>
+            </property>
+          </column>
         </widget>
       </item>
+      <item row="0" column="0">
+        <widget class="QComboBox" name="comboBoxInstance"/>
+      </item>
     </layout>
   </widget>
   <resources/>
   <connections/>
 </ui>
```

### Comparing `msg_explorer-1.6.0/msg_explorer/ui/logger_widget.ui` & `msg_explorer-1.7.0/msg_explorer/ui/multiple_viewer.ui`

 * *Files 27% similar despite different names*

#### Comparing `msg_explorer-1.6.0/msg_explorer/ui/logger_widget.ui` & `msg_explorer-1.7.0/msg_explorer/ui/multiple_viewer.ui`

```diff
@@ -1,25 +1,56 @@
 <?xml version="1.0" encoding="utf-8"?>
 <ui version="4.0">
-  <class>LoggerWidget</class>
-  <widget class="QWidget" name="LoggerWidget">
+  <class>MultipleViewer</class>
+  <widget class="QWidget" name="MultipleViewer">
     <property name="geometry">
       <rect>
         <x>0</x>
         <y>0</y>
         <width>800</width>
         <height>600</height>
       </rect>
     </property>
     <property name="windowTitle">
-      <string>LoggerWidget</string>
+      <string>MultipleViewer</string>
     </property>
     <layout class="QGridLayout" name="gridLayout">
       <item row="0" column="0">
-        <widget class="QListWidget" name="listLog">
+        <layout class="QHBoxLayout" name="horizontalLayout">
+          <item>
+            <widget class="QLabel" name="label">
+              <property name="text">
+                <string>Data Type:</string>
+              </property>
+            </widget>
+          </item>
+          <item>
+            <widget class="QLabel" name="labelType">
+              <property name="text">
+                <string/>
+              </property>
+            </widget>
+          </item>
+          <item>
+            <spacer name="horizontalSpacer">
+              <property name="orientation">
+                <enum>Qt::Horizontal</enum>
+              </property>
+              <property name="sizeHint" stdset="0">
+                <size>
+                  <width>40</width>
+                  <height>20</height>
+                </size>
+              </property>
+            </spacer>
+          </item>
+        </layout>
+      </item>
+      <item row="1" column="0">
+        <widget class="QListWidget" name="listEntries">
           <property name="verticalScrollMode">
             <enum>QAbstractItemView::ScrollPerPixel</enum>
           </property>
           <property name="horizontalScrollMode">
             <enum>QAbstractItemView::ScrollPerPixel</enum>
           </property>
         </widget>
```

### Comparing `msg_explorer-1.6.0/msg_explorer/ui/msg_tree_viewer.ui` & `msg_explorer-1.7.0/msg_explorer/ui/string_viewer.ui`

 * *Files 21% similar despite different names*

#### Comparing `msg_explorer-1.6.0/msg_explorer/ui/msg_tree_viewer.ui` & `msg_explorer-1.7.0/msg_explorer/ui/string_viewer.ui`

```diff
@@ -1,48 +1,38 @@
 <?xml version="1.0" encoding="utf-8"?>
 <ui version="4.0">
-  <class>MSGTreeViewer</class>
-  <widget class="QWidget" name="MSGTreeViewer">
+  <class>StringViewer</class>
+  <widget class="QWidget" name="StringViewer">
     <property name="geometry">
       <rect>
         <x>0</x>
         <y>0</y>
-        <width>400</width>
-        <height>300</height>
+        <width>800</width>
+        <height>600</height>
       </rect>
     </property>
     <property name="windowTitle">
-      <string>Form</string>
+      <string>StringViewer</string>
     </property>
     <layout class="QGridLayout" name="gridLayout">
       <item row="0" column="0">
-        <widget class="QTreeWidget" name="treeWidget">
-          <property name="editTriggers">
-            <set>QAbstractItemView::NoEditTriggers</set>
+        <widget class="QLabel" name="labelType">
+          <property name="text">
+            <string/>
           </property>
-          <property name="verticalScrollMode">
-            <enum>QAbstractItemView::ScrollPerPixel</enum>
+        </widget>
+      </item>
+      <item row="1" column="0">
+        <widget class="QPlainTextEdit" name="textDisplay">
+          <property name="lineWrapMode">
+            <enum>QPlainTextEdit::NoWrap</enum>
           </property>
-          <property name="sortingEnabled">
+          <property name="readOnly">
             <bool>true</bool>
           </property>
-          <property name="headerHidden">
-            <bool>false</bool>
-          </property>
-          <attribute name="headerDefaultSectionSize">
-            <number>400</number>
-          </attribute>
-          <attribute name="headerStretchLastSection">
-            <bool>true</bool>
-          </attribute>
-          <column>
-            <property name="text">
-              <string notr="true">Name</string>
-            </property>
-          </column>
         </widget>
       </item>
     </layout>
   </widget>
   <resources/>
   <connections/>
 </ui>
```

### Comparing `msg_explorer-1.6.0/msg_explorer/ui/named_properties_viewer.ui` & `msg_explorer-1.7.0/msg_explorer/ui/attachments_browser.ui`

 * *Files 22% similar despite different names*

#### Comparing `msg_explorer-1.6.0/msg_explorer/ui/named_properties_viewer.ui` & `msg_explorer-1.7.0/msg_explorer/ui/attachments_browser.ui`

```diff
@@ -1,63 +1,78 @@
 <?xml version="1.0" encoding="utf-8"?>
 <ui version="4.0">
-  <class>NamedPropertiesViewer</class>
-  <widget class="QWidget" name="NamedPropertiesViewer">
+  <class>AttachmentsBrowser</class>
+  <widget class="QWidget" name="AttachmentsBrowser">
     <property name="geometry">
       <rect>
         <x>0</x>
         <y>0</y>
         <width>800</width>
         <height>600</height>
       </rect>
     </property>
     <property name="windowTitle">
-      <string>NamedPropertiesViewer</string>
+      <string>AttachmentsBrowser</string>
     </property>
     <layout class="QGridLayout" name="gridLayout">
-      <item row="1" column="0">
-        <widget class="QTableWidget" name="tableNamedProperties">
+      <item row="0" column="0">
+        <widget class="QTableWidget" name="tableAttachments">
           <property name="editTriggers">
             <set>QAbstractItemView::NoEditTriggers</set>
           </property>
           <property name="verticalScrollMode">
             <enum>QAbstractItemView::ScrollPerPixel</enum>
           </property>
           <property name="horizontalScrollMode">
             <enum>QAbstractItemView::ScrollPerPixel</enum>
           </property>
           <property name="sortingEnabled">
             <bool>true</bool>
           </property>
           <attribute name="horizontalHeaderDefaultSectionSize">
-            <number>300</number>
+            <number>150</number>
+          </attribute>
+          <attribute name="verticalHeaderVisible">
+            <bool>false</bool>
           </attribute>
           <column>
             <property name="text">
-              <string>Property ID</string>
+              <string>ID</string>
+            </property>
+          </column>
+          <column>
+            <property name="text">
+              <string>Status</string>
+            </property>
+          </column>
+          <column>
+            <property name="text">
+              <string>Short Name</string>
+            </property>
+          </column>
+          <column>
+            <property name="text">
+              <string>Long Name</string>
             </property>
           </column>
           <column>
             <property name="text">
-              <string>Property Set GUID</string>
+              <string>Content ID</string>
             </property>
           </column>
           <column>
             <property name="text">
-              <string>Named PID</string>
+              <string>Mime Type</string>
             </property>
           </column>
           <column>
             <property name="text">
-              <string>Data</string>
+              <string>Rendering Position</string>
             </property>
           </column>
         </widget>
       </item>
-      <item row="0" column="0">
-        <widget class="QComboBox" name="comboBoxInstance"/>
-      </item>
     </layout>
   </widget>
   <resources/>
   <connections/>
 </ui>
```

### Comparing `msg_explorer-1.6.0/msg_explorer/ui/properties_viewer.ui` & `msg_explorer-1.7.0/msg_explorer/ui/unhandled_exception.ui`

 * *Files 21% similar despite different names*

#### Comparing `msg_explorer-1.6.0/msg_explorer/ui/properties_viewer.ui` & `msg_explorer-1.7.0/msg_explorer/ui/unhandled_exception.ui`

```diff
@@ -1,58 +1,44 @@
 <?xml version="1.0" encoding="utf-8"?>
 <ui version="4.0">
-  <class>PropertiesViewer</class>
-  <widget class="QWidget" name="PropertiesViewer">
+  <class>UnhandledException</class>
+  <widget class="QDialog" name="UnhandledException">
     <property name="geometry">
       <rect>
         <x>0</x>
         <y>0</y>
-        <width>800</width>
-        <height>600</height>
+        <width>588</width>
+        <height>479</height>
       </rect>
     </property>
     <property name="windowTitle">
-      <string>PropertiesViewer</string>
+      <string>Unhandled Exception</string>
     </property>
     <layout class="QGridLayout" name="gridLayout">
-      <item row="0" column="0">
-        <widget class="QTableWidget" name="tableProps">
-          <property name="editTriggers">
-            <set>QAbstractItemView::NoEditTriggers</set>
+      <item row="1" column="0">
+        <widget class="QPlainTextEdit" name="traceback">
+          <property name="lineWrapMode">
+            <enum>QPlainTextEdit::NoWrap</enum>
           </property>
-          <property name="verticalScrollMode">
-            <enum>QAbstractItemView::ScrollPerPixel</enum>
+          <property name="readOnly">
+            <bool>true</bool>
           </property>
-          <property name="horizontalScrollMode">
-            <enum>QAbstractItemView::ScrollPerPixel</enum>
+          <property name="plainText">
+            <string/>
           </property>
-          <attribute name="horizontalHeaderDefaultSectionSize">
-            <number>100</number>
-          </attribute>
-          <attribute name="horizontalHeaderStretchLastSection">
+        </widget>
+      </item>
+      <item row="0" column="0">
+        <widget class="QLabel" name="label">
+          <property name="text">
+            <string>An unhandled exception has occured. Please report this to the developers.</string>
+          </property>
+          <property name="wordWrap">
             <bool>true</bool>
-          </attribute>
-          <attribute name="verticalHeaderStretchLastSection">
-            <bool>false</bool>
-          </attribute>
-          <column>
-            <property name="text">
-              <string>ID</string>
-            </property>
-          </column>
-          <column>
-            <property name="text">
-              <string>Type</string>
-            </property>
-          </column>
-          <column>
-            <property name="text">
-              <string>Value</string>
-            </property>
-          </column>
+          </property>
         </widget>
       </item>
     </layout>
   </widget>
   <resources/>
   <connections/>
 </ui>
```

### Comparing `msg_explorer-1.6.0/msg_explorer/ui/stream_viewer.ui` & `msg_explorer-1.7.0/msg_explorer/ui/stream_viewer.ui`

 * *Format-specific differences are supported for XML files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: XML 1.0 document, ASCII text, with CRLF line terminators*

 * *Files 26% similar despite different names*

```diff
@@ -1,297 +1,286 @@
 00000000: 3c3f 786d 6c20 7665 7273 696f 6e3d 2231  <?xml version="1
 00000010: 2e30 2220 656e 636f 6469 6e67 3d22 5554  .0" encoding="UT
-00000020: 462d 3822 3f3e 0d0a 3c75 6920 7665 7273  F-8"?>..<ui vers
-00000030: 696f 6e3d 2234 2e30 223e 0d0a 203c 636c  ion="4.0">.. <cl
-00000040: 6173 733e 5374 7265 616d 5669 6577 6572  ass>StreamViewer
-00000050: 3c2f 636c 6173 733e 0d0a 203c 7769 6467  </class>.. <widg
-00000060: 6574 2063 6c61 7373 3d22 5157 6964 6765  et class="QWidge
-00000070: 7422 206e 616d 653d 2253 7472 6561 6d56  t" name="StreamV
-00000080: 6965 7765 7222 3e0d 0a20 203c 7072 6f70  iewer">..  <prop
-00000090: 6572 7479 206e 616d 653d 2267 656f 6d65  erty name="geome
-000000a0: 7472 7922 3e0d 0a20 2020 3c72 6563 743e  try">..   <rect>
-000000b0: 0d0a 2020 2020 3c78 3e30 3c2f 783e 0d0a  ..    <x>0</x>..
-000000c0: 2020 2020 3c79 3e30 3c2f 793e 0d0a 2020      <y>0</y>..  
-000000d0: 2020 3c77 6964 7468 3e38 3030 3c2f 7769    <width>800</wi
-000000e0: 6474 683e 0d0a 2020 2020 3c68 6569 6768  dth>..    <heigh
-000000f0: 743e 3630 303c 2f68 6569 6768 743e 0d0a  t>600</height>..
-00000100: 2020 203c 2f72 6563 743e 0d0a 2020 3c2f     </rect>..  </
-00000110: 7072 6f70 6572 7479 3e0d 0a20 203c 7072  property>..  <pr
-00000120: 6f70 6572 7479 206e 616d 653d 2277 696e  operty name="win
-00000130: 646f 7754 6974 6c65 223e 0d0a 2020 203c  dowTitle">..   <
-00000140: 7374 7269 6e67 3e53 7472 6561 6d56 6965  string>StreamVie
-00000150: 7765 723c 2f73 7472 696e 673e 0d0a 2020  wer</string>..  
-00000160: 3c2f 7072 6f70 6572 7479 3e0d 0a20 203c  </property>..  <
-00000170: 6c61 796f 7574 2063 6c61 7373 3d22 5147  layout class="QG
-00000180: 7269 644c 6179 6f75 7422 206e 616d 653d  ridLayout" name=
-00000190: 2267 7269 644c 6179 6f75 7422 3e0d 0a20  "gridLayout">.. 
-000001a0: 2020 3c70 726f 7065 7274 7920 6e61 6d65    <property name
-000001b0: 3d22 6c65 6674 4d61 7267 696e 223e 0d0a  ="leftMargin">..
-000001c0: 2020 2020 3c6e 756d 6265 723e 303c 2f6e      <number>0</n
-000001d0: 756d 6265 723e 0d0a 2020 203c 2f70 726f  umber>..   </pro
-000001e0: 7065 7274 793e 0d0a 2020 203c 7072 6f70  perty>..   <prop
-000001f0: 6572 7479 206e 616d 653d 2274 6f70 4d61  erty name="topMa
-00000200: 7267 696e 223e 0d0a 2020 2020 3c6e 756d  rgin">..    <num
-00000210: 6265 723e 303c 2f6e 756d 6265 723e 0d0a  ber>0</number>..
-00000220: 2020 203c 2f70 726f 7065 7274 793e 0d0a     </property>..
-00000230: 2020 203c 7072 6f70 6572 7479 206e 616d     <property nam
-00000240: 653d 2272 6967 6874 4d61 7267 696e 223e  e="rightMargin">
-00000250: 0d0a 2020 2020 3c6e 756d 6265 723e 303c  ..    <number>0<
-00000260: 2f6e 756d 6265 723e 0d0a 2020 203c 2f70  /number>..   </p
-00000270: 726f 7065 7274 793e 0d0a 2020 203c 7072  roperty>..   <pr
-00000280: 6f70 6572 7479 206e 616d 653d 2262 6f74  operty name="bot
-00000290: 746f 6d4d 6172 6769 6e22 3e0d 0a20 2020  tomMargin">..   
-000002a0: 203c 6e75 6d62 6572 3e30 3c2f 6e75 6d62   <number>0</numb
-000002b0: 6572 3e0d 0a20 2020 3c2f 7072 6f70 6572  er>..   </proper
-000002c0: 7479 3e0d 0a20 2020 3c69 7465 6d20 726f  ty>..   <item ro
-000002d0: 773d 2234 2220 636f 6c75 6d6e 3d22 3022  w="4" column="0"
-000002e0: 3e0d 0a20 2020 203c 6c61 796f 7574 2063  >..    <layout c
-000002f0: 6c61 7373 3d22 5148 426f 784c 6179 6f75  lass="QHBoxLayou
-00000300: 7422 206e 616d 653d 2268 6f72 697a 6f6e  t" name="horizon
-00000310: 7461 6c4c 6179 6f75 7422 3e0d 0a20 2020  talLayout">..   
-00000320: 2020 3c69 7465 6d3e 0d0a 2020 2020 2020    <item>..      
-00000330: 3c77 6964 6765 7420 636c 6173 733d 2251  <widget class="Q
-00000340: 5261 6469 6f42 7574 746f 6e22 206e 616d  RadioButton" nam
-00000350: 653d 2262 7574 746f 6e50 6172 7365 6456  e="buttonParsedV
-00000360: 6965 7722 3e0d 0a20 2020 2020 2020 3c70  iew">..       <p
-00000370: 726f 7065 7274 7920 6e61 6d65 3d22 7465  roperty name="te
-00000380: 7874 223e 0d0a 2020 2020 2020 2020 3c73  xt">..        <s
-00000390: 7472 696e 673e 5061 7273 6564 2056 6965  tring>Parsed Vie
-000003a0: 773c 2f73 7472 696e 673e 0d0a 2020 2020  w</string>..    
-000003b0: 2020 203c 2f70 726f 7065 7274 793e 0d0a     </property>..
-000003c0: 2020 2020 2020 203c 7072 6f70 6572 7479         <property
-000003d0: 206e 616d 653d 2263 6865 636b 6564 223e   name="checked">
-000003e0: 0d0a 2020 2020 2020 2020 3c62 6f6f 6c3e  ..        <bool>
-000003f0: 7472 7565 3c2f 626f 6f6c 3e0d 0a20 2020  true</bool>..   
-00000400: 2020 2020 3c2f 7072 6f70 6572 7479 3e0d      </property>.
-00000410: 0a20 2020 2020 203c 2f77 6964 6765 743e  .      </widget>
-00000420: 0d0a 2020 2020 203c 2f69 7465 6d3e 0d0a  ..     </item>..
-00000430: 2020 2020 203c 6974 656d 3e0d 0a20 2020       <item>..   
-00000440: 2020 203c 7769 6467 6574 2063 6c61 7373     <widget class
-00000450: 3d22 5152 6164 696f 4275 7474 6f6e 2220  ="QRadioButton" 
-00000460: 6e61 6d65 3d22 6275 7474 6f6e 4865 7856  name="buttonHexV
-00000470: 6965 7722 3e0d 0a20 2020 2020 2020 3c70  iew">..       <p
-00000480: 726f 7065 7274 7920 6e61 6d65 3d22 7465  roperty name="te
-00000490: 7874 223e 0d0a 2020 2020 2020 2020 3c73  xt">..        <s
-000004a0: 7472 696e 673e 4865 7820 5669 6577 3c2f  tring>Hex View</
-000004b0: 7374 7269 6e67 3e0d 0a20 2020 2020 2020  string>..       
-000004c0: 3c2f 7072 6f70 6572 7479 3e0d 0a20 2020  </property>..   
-000004d0: 2020 2020 3c70 726f 7065 7274 7920 6e61      <property na
-000004e0: 6d65 3d22 6368 6563 6b65 6422 3e0d 0a20  me="checked">.. 
-000004f0: 2020 2020 2020 203c 626f 6f6c 3e66 616c         <bool>fal
-00000500: 7365 3c2f 626f 6f6c 3e0d 0a20 2020 2020  se</bool>..     
-00000510: 2020 3c2f 7072 6f70 6572 7479 3e0d 0a20    </property>.. 
-00000520: 2020 2020 203c 2f77 6964 6765 743e 0d0a       </widget>..
-00000530: 2020 2020 203c 2f69 7465 6d3e 0d0a 2020       </item>..  
-00000540: 2020 203c 6974 656d 3e0d 0a20 2020 2020     <item>..     
-00000550: 203c 7370 6163 6572 206e 616d 653d 2268   <spacer name="h
-00000560: 6f72 697a 6f6e 7461 6c53 7061 6365 7222  orizontalSpacer"
-00000570: 3e0d 0a20 2020 2020 2020 3c70 726f 7065  >..       <prope
-00000580: 7274 7920 6e61 6d65 3d22 6f72 6965 6e74  rty name="orient
-00000590: 6174 696f 6e22 3e0d 0a20 2020 2020 2020  ation">..       
-000005a0: 203c 656e 756d 3e51 743a 3a48 6f72 697a   <enum>Qt::Horiz
-000005b0: 6f6e 7461 6c3c 2f65 6e75 6d3e 0d0a 2020  ontal</enum>..  
-000005c0: 2020 2020 203c 2f70 726f 7065 7274 793e       </property>
-000005d0: 0d0a 2020 2020 2020 203c 7072 6f70 6572  ..       <proper
-000005e0: 7479 206e 616d 653d 2273 697a 6548 696e  ty name="sizeHin
-000005f0: 7422 2073 7464 7365 743d 2230 223e 0d0a  t" stdset="0">..
-00000600: 2020 2020 2020 2020 3c73 697a 653e 0d0a          <size>..
-00000610: 2020 2020 2020 2020 203c 7769 6474 683e           <width>
-00000620: 3430 3c2f 7769 6474 683e 0d0a 2020 2020  40</width>..    
-00000630: 2020 2020 203c 6865 6967 6874 3e32 303c       <height>20<
-00000640: 2f68 6569 6768 743e 0d0a 2020 2020 2020  /height>..      
-00000650: 2020 3c2f 7369 7a65 3e0d 0a20 2020 2020    </size>..     
-00000660: 2020 3c2f 7072 6f70 6572 7479 3e0d 0a20    </property>.. 
-00000670: 2020 2020 203c 2f73 7061 6365 723e 0d0a       </spacer>..
-00000680: 2020 2020 203c 2f69 7465 6d3e 0d0a 2020       </item>..  
-00000690: 2020 3c2f 6c61 796f 7574 3e0d 0a20 2020    </layout>..   
-000006a0: 3c2f 6974 656d 3e0d 0a20 2020 3c69 7465  </item>..   <ite
-000006b0: 6d20 726f 773d 2235 2220 636f 6c75 6d6e  m row="5" column
-000006c0: 3d22 3022 3e0d 0a20 2020 203c 7769 6467  ="0">..    <widg
-000006d0: 6574 2063 6c61 7373 3d22 5153 7461 636b  et class="QStack
-000006e0: 6564 5769 6467 6574 2220 6e61 6d65 3d22  edWidget" name="
-000006f0: 7374 6163 6b65 6457 6964 6765 7422 3e0d  stackedWidget">.
-00000700: 0a20 2020 2020 3c77 6964 6765 7420 636c  .     <widget cl
-00000710: 6173 733d 2251 5769 6467 6574 2220 6e61  ass="QWidget" na
-00000720: 6d65 3d22 7061 6765 5061 7273 6564 4e6f  me="pageParsedNo
-00000730: 4461 7461 223e 0d0a 2020 2020 2020 3c6c  Data">..      <l
-00000740: 6179 6f75 7420 636c 6173 733d 2251 4772  ayout class="QGr
-00000750: 6964 4c61 796f 7574 2220 6e61 6d65 3d22  idLayout" name="
-00000760: 6772 6964 4c61 796f 7574 5f33 223e 0d0a  gridLayout_3">..
-00000770: 2020 2020 2020 203c 6974 656d 2072 6f77         <item row
-00000780: 3d22 3022 2063 6f6c 756d 6e3d 2230 223e  ="0" column="0">
-00000790: 0d0a 2020 2020 2020 2020 3c77 6964 6765  ..        <widge
-000007a0: 7420 636c 6173 733d 2251 4c61 6265 6c22  t class="QLabel"
-000007b0: 206e 616d 653d 226c 6162 656c 223e 0d0a   name="label">..
-000007c0: 2020 2020 2020 2020 203c 7072 6f70 6572           <proper
-000007d0: 7479 206e 616d 653d 2274 6578 7422 3e0d  ty name="text">.
-000007e0: 0a20 2020 2020 2020 2020 203c 7374 7269  .          <stri
-000007f0: 6e67 3e4e 6f20 7374 7265 616d 2068 6173  ng>No stream has
-00000800: 2062 6565 6e20 6c6f 6164 6564 2e20 5472   been loaded. Tr
-00000810: 7920 646f 7562 6c65 2063 6c69 636b 696e  y double clickin
-00000820: 6720 6f6e 6520 696e 2074 6865 2074 7265  g one in the tre
-00000830: 6520 7669 6577 2e3c 2f73 7472 696e 673e  e view.</string>
-00000840: 0d0a 2020 2020 2020 2020 203c 2f70 726f  ..         </pro
-00000850: 7065 7274 793e 0d0a 2020 2020 2020 2020  perty>..        
-00000860: 203c 7072 6f70 6572 7479 206e 616d 653d   <property name=
-00000870: 2261 6c69 676e 6d65 6e74 223e 0d0a 2020  "alignment">..  
-00000880: 2020 2020 2020 2020 3c73 6574 3e51 743a          <set>Qt:
-00000890: 3a41 6c69 676e 4365 6e74 6572 3c2f 7365  :AlignCenter</se
-000008a0: 743e 0d0a 2020 2020 2020 2020 203c 2f70  t>..         </p
-000008b0: 726f 7065 7274 793e 0d0a 2020 2020 2020  roperty>..      
-000008c0: 2020 203c 7072 6f70 6572 7479 206e 616d     <property nam
-000008d0: 653d 2277 6f72 6457 7261 7022 3e0d 0a20  e="wordWrap">.. 
-000008e0: 2020 2020 2020 2020 203c 626f 6f6c 3e74           <bool>t
-000008f0: 7275 653c 2f62 6f6f 6c3e 0d0a 2020 2020  rue</bool>..    
-00000900: 2020 2020 203c 2f70 726f 7065 7274 793e       </property>
-00000910: 0d0a 2020 2020 2020 2020 3c2f 7769 6467  ..        </widg
-00000920: 6574 3e0d 0a20 2020 2020 2020 3c2f 6974  et>..       </it
-00000930: 656d 3e0d 0a20 2020 2020 203c 2f6c 6179  em>..      </lay
-00000940: 6f75 743e 0d0a 2020 2020 203c 2f77 6964  out>..     </wid
-00000950: 6765 743e 0d0a 2020 2020 203c 7769 6467  get>..     <widg
-00000960: 6574 2063 6c61 7373 3d22 5374 7269 6e67  et class="String
-00000970: 5669 6577 6572 2220 6e61 6d65 3d22 7061  Viewer" name="pa
-00000980: 6765 5061 7273 6564 5374 7269 6e67 222f  geParsedString"/
-00000990: 3e0d 0a20 2020 2020 3c77 6964 6765 7420  >..     <widget 
-000009a0: 636c 6173 733d 224d 756c 7469 706c 6556  class="MultipleV
-000009b0: 6965 7765 7222 206e 616d 653d 2270 6167  iewer" name="pag
-000009c0: 6550 6172 7365 644d 756c 7469 706c 6522  eParsedMultiple"
-000009d0: 2f3e 0d0a 2020 2020 203c 7769 6467 6574  />..     <widget
-000009e0: 2063 6c61 7373 3d22 4d75 6c74 6970 6c65   class="Multiple
-000009f0: 4269 6e61 7279 5669 6577 6572 2220 6e61  BinaryViewer" na
-00000a00: 6d65 3d22 7061 6765 5061 7273 6564 4d75  me="pageParsedMu
-00000a10: 6c74 6970 6c65 4269 6e61 7279 222f 3e0d  ltipleBinary"/>.
-00000a20: 0a20 2020 2020 3c77 6964 6765 7420 636c  .     <widget cl
-00000a30: 6173 733d 2250 726f 7065 7274 6965 7356  ass="PropertiesV
-00000a40: 6965 7765 7222 206e 616d 653d 2270 6167  iewer" name="pag
-00000a50: 6550 6172 7365 6450 726f 7065 7274 6965  eParsedPropertie
-00000a60: 7322 2f3e 0d0a 2020 2020 203c 7769 6467  s"/>..     <widg
-00000a70: 6574 2063 6c61 7373 3d22 4775 6964 5669  et class="GuidVi
-00000a80: 6577 6572 2220 6e61 6d65 3d22 7061 6765  ewer" name="page
-00000a90: 5061 7273 6564 4775 6964 5669 6577 6572  ParsedGuidViewer
-00000aa0: 222f 3e0d 0a20 2020 2020 3c77 6964 6765  "/>..     <widge
-00000ab0: 7420 636c 6173 733d 2248 6578 5669 6577  t class="HexView
-00000ac0: 6572 2220 6e61 6d65 3d22 7061 6765 4865  er" name="pageHe
-00000ad0: 7856 6965 7765 7222 2f3e 0d0a 2020 2020  xViewer"/>..    
-00000ae0: 3c2f 7769 6467 6574 3e0d 0a20 2020 3c2f  </widget>..   </
-00000af0: 6974 656d 3e0d 0a20 2020 3c69 7465 6d20  item>..   <item 
-00000b00: 726f 773d 2233 2220 636f 6c75 6d6e 3d22  row="3" column="
-00000b10: 3022 3e0d 0a20 2020 203c 6c61 796f 7574  0">..    <layout
-00000b20: 2063 6c61 7373 3d22 5148 426f 784c 6179   class="QHBoxLay
-00000b30: 6f75 7422 206e 616d 653d 2268 6f72 697a  out" name="horiz
-00000b40: 6f6e 7461 6c4c 6179 6f75 745f 3322 3e0d  ontalLayout_3">.
-00000b50: 0a20 2020 2020 3c69 7465 6d3e 0d0a 2020  .     <item>..  
-00000b60: 2020 2020 3c77 6964 6765 7420 636c 6173      <widget clas
-00000b70: 733d 2251 4c61 6265 6c22 206e 616d 653d  s="QLabel" name=
-00000b80: 226c 6162 656c 5f32 223e 0d0a 2020 2020  "label_2">..    
-00000b90: 2020 203c 7072 6f70 6572 7479 206e 616d     <property nam
-00000ba0: 653d 2274 6578 7422 3e0d 0a20 2020 2020  e="text">..     
-00000bb0: 2020 203c 7374 7269 6e67 3e43 7572 7265     <string>Curre
-00000bc0: 6e74 2053 7472 6561 6d3a 3c2f 7374 7269  nt Stream:</stri
-00000bd0: 6e67 3e0d 0a20 2020 2020 2020 3c2f 7072  ng>..       </pr
-00000be0: 6f70 6572 7479 3e0d 0a20 2020 2020 203c  operty>..      <
-00000bf0: 2f77 6964 6765 743e 0d0a 2020 2020 203c  /widget>..     <
-00000c00: 2f69 7465 6d3e 0d0a 2020 2020 203c 6974  /item>..     <it
-00000c10: 656d 3e0d 0a20 2020 2020 203c 7769 6467  em>..      <widg
-00000c20: 6574 2063 6c61 7373 3d22 514c 6162 656c  et class="QLabel
-00000c30: 2220 6e61 6d65 3d22 6c61 6265 6c53 7472  " name="labelStr
-00000c40: 6561 6d4e 616d 6522 3e0d 0a20 2020 2020  eamName">..     
-00000c50: 2020 3c70 726f 7065 7274 7920 6e61 6d65    <property name
-00000c60: 3d22 7465 7874 223e 0d0a 2020 2020 2020  ="text">..      
-00000c70: 2020 3c73 7472 696e 673e 4e6f 6e65 3c2f    <string>None</
-00000c80: 7374 7269 6e67 3e0d 0a20 2020 2020 2020  string>..       
-00000c90: 3c2f 7072 6f70 6572 7479 3e0d 0a20 2020  </property>..   
-00000ca0: 2020 203c 2f77 6964 6765 743e 0d0a 2020     </widget>..  
-00000cb0: 2020 203c 2f69 7465 6d3e 0d0a 2020 2020     </item>..    
-00000cc0: 203c 6974 656d 3e0d 0a20 2020 2020 203c   <item>..      <
-00000cd0: 7370 6163 6572 206e 616d 653d 2268 6f72  spacer name="hor
-00000ce0: 697a 6f6e 7461 6c53 7061 6365 725f 3222  izontalSpacer_2"
-00000cf0: 3e0d 0a20 2020 2020 2020 3c70 726f 7065  >..       <prope
-00000d00: 7274 7920 6e61 6d65 3d22 6f72 6965 6e74  rty name="orient
-00000d10: 6174 696f 6e22 3e0d 0a20 2020 2020 2020  ation">..       
-00000d20: 203c 656e 756d 3e51 743a 3a48 6f72 697a   <enum>Qt::Horiz
-00000d30: 6f6e 7461 6c3c 2f65 6e75 6d3e 0d0a 2020  ontal</enum>..  
-00000d40: 2020 2020 203c 2f70 726f 7065 7274 793e       </property>
-00000d50: 0d0a 2020 2020 2020 203c 7072 6f70 6572  ..       <proper
-00000d60: 7479 206e 616d 653d 2273 697a 6548 696e  ty name="sizeHin
-00000d70: 7422 2073 7464 7365 743d 2230 223e 0d0a  t" stdset="0">..
-00000d80: 2020 2020 2020 2020 3c73 697a 653e 0d0a          <size>..
-00000d90: 2020 2020 2020 2020 203c 7769 6474 683e           <width>
-00000da0: 3430 3c2f 7769 6474 683e 0d0a 2020 2020  40</width>..    
-00000db0: 2020 2020 203c 6865 6967 6874 3e32 303c       <height>20<
-00000dc0: 2f68 6569 6768 743e 0d0a 2020 2020 2020  /height>..      
-00000dd0: 2020 3c2f 7369 7a65 3e0d 0a20 2020 2020    </size>..     
-00000de0: 2020 3c2f 7072 6f70 6572 7479 3e0d 0a20    </property>.. 
-00000df0: 2020 2020 203c 2f73 7061 6365 723e 0d0a       </spacer>..
-00000e00: 2020 2020 203c 2f69 7465 6d3e 0d0a 2020       </item>..  
-00000e10: 2020 3c2f 6c61 796f 7574 3e0d 0a20 2020    </layout>..   
-00000e20: 3c2f 6974 656d 3e0d 0a20 203c 2f6c 6179  </item>..  </lay
-00000e30: 6f75 743e 0d0a 203c 2f77 6964 6765 743e  out>.. </widget>
-00000e40: 0d0a 203c 6375 7374 6f6d 7769 6467 6574  .. <customwidget
-00000e50: 733e 0d0a 2020 3c63 7573 746f 6d77 6964  s>..  <customwid
-00000e60: 6765 743e 0d0a 2020 203c 636c 6173 733e  get>..   <class>
-00000e70: 4865 7856 6965 7765 723c 2f63 6c61 7373  HexViewer</class
-00000e80: 3e0d 0a20 2020 3c65 7874 656e 6473 3e51  >..   <extends>Q
-00000e90: 5769 6467 6574 3c2f 6578 7465 6e64 733e  Widget</extends>
-00000ea0: 0d0a 2020 203c 6865 6164 6572 3e2e 2e68  ..   <header>..h
-00000eb0: 6578 5f76 6965 7765 723c 2f68 6561 6465  ex_viewer</heade
-00000ec0: 723e 0d0a 2020 203c 636f 6e74 6169 6e65  r>..   <containe
-00000ed0: 723e 313c 2f63 6f6e 7461 696e 6572 3e0d  r>1</container>.
-00000ee0: 0a20 203c 2f63 7573 746f 6d77 6964 6765  .  </customwidge
-00000ef0: 743e 0d0a 2020 3c63 7573 746f 6d77 6964  t>..  <customwid
-00000f00: 6765 743e 0d0a 2020 203c 636c 6173 733e  get>..   <class>
-00000f10: 4d75 6c74 6970 6c65 4269 6e61 7279 5669  MultipleBinaryVi
-00000f20: 6577 6572 3c2f 636c 6173 733e 0d0a 2020  ewer</class>..  
-00000f30: 203c 6578 7465 6e64 733e 5157 6964 6765   <extends>QWidge
-00000f40: 743c 2f65 7874 656e 6473 3e0d 0a20 2020  t</extends>..   
-00000f50: 3c68 6561 6465 723e 2e2e 6d75 6c74 6970  <header>..multip
-00000f60: 6c65 5f62 696e 6172 795f 7669 6577 6572  le_binary_viewer
-00000f70: 3c2f 6865 6164 6572 3e0d 0a20 2020 3c63  </header>..   <c
-00000f80: 6f6e 7461 696e 6572 3e31 3c2f 636f 6e74  ontainer>1</cont
-00000f90: 6169 6e65 723e 0d0a 2020 3c2f 6375 7374  ainer>..  </cust
-00000fa0: 6f6d 7769 6467 6574 3e0d 0a20 203c 6375  omwidget>..  <cu
-00000fb0: 7374 6f6d 7769 6467 6574 3e0d 0a20 2020  stomwidget>..   
-00000fc0: 3c63 6c61 7373 3e4d 756c 7469 706c 6556  <class>MultipleV
-00000fd0: 6965 7765 723c 2f63 6c61 7373 3e0d 0a20  iewer</class>.. 
-00000fe0: 2020 3c65 7874 656e 6473 3e51 5769 6467    <extends>QWidg
-00000ff0: 6574 3c2f 6578 7465 6e64 733e 0d0a 2020  et</extends>..  
-00001000: 203c 6865 6164 6572 3e2e 2e6d 756c 7469   <header>..multi
-00001010: 706c 655f 7669 6577 6572 3c2f 6865 6164  ple_viewer</head
-00001020: 6572 3e0d 0a20 2020 3c63 6f6e 7461 696e  er>..   <contain
-00001030: 6572 3e31 3c2f 636f 6e74 6169 6e65 723e  er>1</container>
-00001040: 0d0a 2020 3c2f 6375 7374 6f6d 7769 6467  ..  </customwidg
-00001050: 6574 3e0d 0a20 203c 6375 7374 6f6d 7769  et>..  <customwi
-00001060: 6467 6574 3e0d 0a20 2020 3c63 6c61 7373  dget>..   <class
-00001070: 3e53 7472 696e 6756 6965 7765 723c 2f63  >StringViewer</c
-00001080: 6c61 7373 3e0d 0a20 2020 3c65 7874 656e  lass>..   <exten
-00001090: 6473 3e51 5769 6467 6574 3c2f 6578 7465  ds>QWidget</exte
-000010a0: 6e64 733e 0d0a 2020 203c 6865 6164 6572  nds>..   <header
-000010b0: 3e2e 2e73 7472 696e 675f 7669 6577 6572  >..string_viewer
-000010c0: 3c2f 6865 6164 6572 3e0d 0a20 2020 3c63  </header>..   <c
-000010d0: 6f6e 7461 696e 6572 3e31 3c2f 636f 6e74  ontainer>1</cont
-000010e0: 6169 6e65 723e 0d0a 2020 3c2f 6375 7374  ainer>..  </cust
-000010f0: 6f6d 7769 6467 6574 3e0d 0a20 203c 6375  omwidget>..  <cu
-00001100: 7374 6f6d 7769 6467 6574 3e0d 0a20 2020  stomwidget>..   
-00001110: 3c63 6c61 7373 3e50 726f 7065 7274 6965  <class>Propertie
-00001120: 7356 6965 7765 723c 2f63 6c61 7373 3e0d  sViewer</class>.
-00001130: 0a20 2020 3c65 7874 656e 6473 3e51 5769  .   <extends>QWi
-00001140: 6467 6574 3c2f 6578 7465 6e64 733e 0d0a  dget</extends>..
-00001150: 2020 203c 6865 6164 6572 3e2e 2e70 726f     <header>..pro
-00001160: 7065 7274 6965 735f 7669 6577 6572 3c2f  perties_viewer</
-00001170: 6865 6164 6572 3e0d 0a20 2020 3c63 6f6e  header>..   <con
-00001180: 7461 696e 6572 3e31 3c2f 636f 6e74 6169  tainer>1</contai
-00001190: 6e65 723e 0d0a 2020 3c2f 6375 7374 6f6d  ner>..  </custom
-000011a0: 7769 6467 6574 3e0d 0a20 203c 6375 7374  widget>..  <cust
-000011b0: 6f6d 7769 6467 6574 3e0d 0a20 2020 3c63  omwidget>..   <c
-000011c0: 6c61 7373 3e47 7569 6456 6965 7765 723c  lass>GuidViewer<
-000011d0: 2f63 6c61 7373 3e0d 0a20 2020 3c65 7874  /class>..   <ext
-000011e0: 656e 6473 3e51 5769 6467 6574 3c2f 6578  ends>QWidget</ex
-000011f0: 7465 6e64 733e 0d0a 2020 203c 6865 6164  tends>..   <head
-00001200: 6572 3e2e 2e67 7569 645f 7669 6577 6572  er>..guid_viewer
-00001210: 3c2f 6865 6164 6572 3e0d 0a20 2020 3c63  </header>..   <c
-00001220: 6f6e 7461 696e 6572 3e31 3c2f 636f 6e74  ontainer>1</cont
-00001230: 6169 6e65 723e 0d0a 2020 3c2f 6375 7374  ainer>..  </cust
-00001240: 6f6d 7769 6467 6574 3e0d 0a20 3c2f 6375  omwidget>.. </cu
-00001250: 7374 6f6d 7769 6467 6574 733e 0d0a 203c  stomwidgets>.. <
-00001260: 7265 736f 7572 6365 732f 3e0d 0a20 3c63  resources/>.. <c
-00001270: 6f6e 6e65 6374 696f 6e73 2f3e 0d0a 3c2f  onnections/>..</
-00001280: 7569 3e0d 0a                             ui>..
+00000020: 462d 3822 3f3e 0a3c 7569 2076 6572 7369  F-8"?>.<ui versi
+00000030: 6f6e 3d22 342e 3022 3e0a 203c 636c 6173  on="4.0">. <clas
+00000040: 733e 5374 7265 616d 5669 6577 6572 3c2f  s>StreamViewer</
+00000050: 636c 6173 733e 0a20 3c77 6964 6765 7420  class>. <widget 
+00000060: 636c 6173 733d 2251 5769 6467 6574 2220  class="QWidget" 
+00000070: 6e61 6d65 3d22 5374 7265 616d 5669 6577  name="StreamView
+00000080: 6572 223e 0a20 203c 7072 6f70 6572 7479  er">.  <property
+00000090: 206e 616d 653d 2267 656f 6d65 7472 7922   name="geometry"
+000000a0: 3e0a 2020 203c 7265 6374 3e0a 2020 2020  >.   <rect>.    
+000000b0: 3c78 3e30 3c2f 783e 0a20 2020 203c 793e  <x>0</x>.    <y>
+000000c0: 303c 2f79 3e0a 2020 2020 3c77 6964 7468  0</y>.    <width
+000000d0: 3e38 3030 3c2f 7769 6474 683e 0a20 2020  >800</width>.   
+000000e0: 203c 6865 6967 6874 3e36 3030 3c2f 6865   <height>600</he
+000000f0: 6967 6874 3e0a 2020 203c 2f72 6563 743e  ight>.   </rect>
+00000100: 0a20 203c 2f70 726f 7065 7274 793e 0a20  .  </property>. 
+00000110: 203c 7072 6f70 6572 7479 206e 616d 653d   <property name=
+00000120: 2277 696e 646f 7754 6974 6c65 223e 0a20  "windowTitle">. 
+00000130: 2020 3c73 7472 696e 673e 5374 7265 616d    <string>Stream
+00000140: 5669 6577 6572 3c2f 7374 7269 6e67 3e0a  Viewer</string>.
+00000150: 2020 3c2f 7072 6f70 6572 7479 3e0a 2020    </property>.  
+00000160: 3c6c 6179 6f75 7420 636c 6173 733d 2251  <layout class="Q
+00000170: 4772 6964 4c61 796f 7574 2220 6e61 6d65  GridLayout" name
+00000180: 3d22 6772 6964 4c61 796f 7574 223e 0a20  ="gridLayout">. 
+00000190: 2020 3c70 726f 7065 7274 7920 6e61 6d65    <property name
+000001a0: 3d22 6c65 6674 4d61 7267 696e 223e 0a20  ="leftMargin">. 
+000001b0: 2020 203c 6e75 6d62 6572 3e30 3c2f 6e75     <number>0</nu
+000001c0: 6d62 6572 3e0a 2020 203c 2f70 726f 7065  mber>.   </prope
+000001d0: 7274 793e 0a20 2020 3c70 726f 7065 7274  rty>.   <propert
+000001e0: 7920 6e61 6d65 3d22 746f 704d 6172 6769  y name="topMargi
+000001f0: 6e22 3e0a 2020 2020 3c6e 756d 6265 723e  n">.    <number>
+00000200: 303c 2f6e 756d 6265 723e 0a20 2020 3c2f  0</number>.   </
+00000210: 7072 6f70 6572 7479 3e0a 2020 203c 7072  property>.   <pr
+00000220: 6f70 6572 7479 206e 616d 653d 2272 6967  operty name="rig
+00000230: 6874 4d61 7267 696e 223e 0a20 2020 203c  htMargin">.    <
+00000240: 6e75 6d62 6572 3e30 3c2f 6e75 6d62 6572  number>0</number
+00000250: 3e0a 2020 203c 2f70 726f 7065 7274 793e  >.   </property>
+00000260: 0a20 2020 3c70 726f 7065 7274 7920 6e61  .   <property na
+00000270: 6d65 3d22 626f 7474 6f6d 4d61 7267 696e  me="bottomMargin
+00000280: 223e 0a20 2020 203c 6e75 6d62 6572 3e30  ">.    <number>0
+00000290: 3c2f 6e75 6d62 6572 3e0a 2020 203c 2f70  </number>.   </p
+000002a0: 726f 7065 7274 793e 0a20 2020 3c69 7465  roperty>.   <ite
+000002b0: 6d20 726f 773d 2234 2220 636f 6c75 6d6e  m row="4" column
+000002c0: 3d22 3022 3e0a 2020 2020 3c6c 6179 6f75  ="0">.    <layou
+000002d0: 7420 636c 6173 733d 2251 4842 6f78 4c61  t class="QHBoxLa
+000002e0: 796f 7574 2220 6e61 6d65 3d22 686f 7269  yout" name="hori
+000002f0: 7a6f 6e74 616c 4c61 796f 7574 223e 0a20  zontalLayout">. 
+00000300: 2020 2020 3c69 7465 6d3e 0a20 2020 2020      <item>.     
+00000310: 203c 7769 6467 6574 2063 6c61 7373 3d22   <widget class="
+00000320: 5152 6164 696f 4275 7474 6f6e 2220 6e61  QRadioButton" na
+00000330: 6d65 3d22 6275 7474 6f6e 5061 7273 6564  me="buttonParsed
+00000340: 5669 6577 223e 0a20 2020 2020 2020 3c70  View">.       <p
+00000350: 726f 7065 7274 7920 6e61 6d65 3d22 7465  roperty name="te
+00000360: 7874 223e 0a20 2020 2020 2020 203c 7374  xt">.        <st
+00000370: 7269 6e67 3e50 6172 7365 6420 5669 6577  ring>Parsed View
+00000380: 3c2f 7374 7269 6e67 3e0a 2020 2020 2020  </string>.      
+00000390: 203c 2f70 726f 7065 7274 793e 0a20 2020   </property>.   
+000003a0: 2020 2020 3c70 726f 7065 7274 7920 6e61      <property na
+000003b0: 6d65 3d22 6368 6563 6b65 6422 3e0a 2020  me="checked">.  
+000003c0: 2020 2020 2020 3c62 6f6f 6c3e 7472 7565        <bool>true
+000003d0: 3c2f 626f 6f6c 3e0a 2020 2020 2020 203c  </bool>.       <
+000003e0: 2f70 726f 7065 7274 793e 0a20 2020 2020  /property>.     
+000003f0: 203c 2f77 6964 6765 743e 0a20 2020 2020   </widget>.     
+00000400: 3c2f 6974 656d 3e0a 2020 2020 203c 6974  </item>.     <it
+00000410: 656d 3e0a 2020 2020 2020 3c77 6964 6765  em>.      <widge
+00000420: 7420 636c 6173 733d 2251 5261 6469 6f42  t class="QRadioB
+00000430: 7574 746f 6e22 206e 616d 653d 2262 7574  utton" name="but
+00000440: 746f 6e48 6578 5669 6577 223e 0a20 2020  tonHexView">.   
+00000450: 2020 2020 3c70 726f 7065 7274 7920 6e61      <property na
+00000460: 6d65 3d22 7465 7874 223e 0a20 2020 2020  me="text">.     
+00000470: 2020 203c 7374 7269 6e67 3e48 6578 2056     <string>Hex V
+00000480: 6965 773c 2f73 7472 696e 673e 0a20 2020  iew</string>.   
+00000490: 2020 2020 3c2f 7072 6f70 6572 7479 3e0a      </property>.
+000004a0: 2020 2020 2020 203c 7072 6f70 6572 7479         <property
+000004b0: 206e 616d 653d 2263 6865 636b 6564 223e   name="checked">
+000004c0: 0a20 2020 2020 2020 203c 626f 6f6c 3e66  .        <bool>f
+000004d0: 616c 7365 3c2f 626f 6f6c 3e0a 2020 2020  alse</bool>.    
+000004e0: 2020 203c 2f70 726f 7065 7274 793e 0a20     </property>. 
+000004f0: 2020 2020 203c 2f77 6964 6765 743e 0a20       </widget>. 
+00000500: 2020 2020 3c2f 6974 656d 3e0a 2020 2020      </item>.    
+00000510: 203c 6974 656d 3e0a 2020 2020 2020 3c73   <item>.      <s
+00000520: 7061 6365 7220 6e61 6d65 3d22 686f 7269  pacer name="hori
+00000530: 7a6f 6e74 616c 5370 6163 6572 223e 0a20  zontalSpacer">. 
+00000540: 2020 2020 2020 3c70 726f 7065 7274 7920        <property 
+00000550: 6e61 6d65 3d22 6f72 6965 6e74 6174 696f  name="orientatio
+00000560: 6e22 3e0a 2020 2020 2020 2020 3c65 6e75  n">.        <enu
+00000570: 6d3e 5174 3a3a 486f 7269 7a6f 6e74 616c  m>Qt::Horizontal
+00000580: 3c2f 656e 756d 3e0a 2020 2020 2020 203c  </enum>.       <
+00000590: 2f70 726f 7065 7274 793e 0a20 2020 2020  /property>.     
+000005a0: 2020 3c70 726f 7065 7274 7920 6e61 6d65    <property name
+000005b0: 3d22 7369 7a65 4869 6e74 2220 7374 6473  ="sizeHint" stds
+000005c0: 6574 3d22 3022 3e0a 2020 2020 2020 2020  et="0">.        
+000005d0: 3c73 697a 653e 0a20 2020 2020 2020 2020  <size>.         
+000005e0: 3c77 6964 7468 3e34 303c 2f77 6964 7468  <width>40</width
+000005f0: 3e0a 2020 2020 2020 2020 203c 6865 6967  >.         <heig
+00000600: 6874 3e32 303c 2f68 6569 6768 743e 0a20  ht>20</height>. 
+00000610: 2020 2020 2020 203c 2f73 697a 653e 0a20         </size>. 
+00000620: 2020 2020 2020 3c2f 7072 6f70 6572 7479        </property
+00000630: 3e0a 2020 2020 2020 3c2f 7370 6163 6572  >.      </spacer
+00000640: 3e0a 2020 2020 203c 2f69 7465 6d3e 0a20  >.     </item>. 
+00000650: 2020 203c 2f6c 6179 6f75 743e 0a20 2020     </layout>.   
+00000660: 3c2f 6974 656d 3e0a 2020 203c 6974 656d  </item>.   <item
+00000670: 2072 6f77 3d22 3522 2063 6f6c 756d 6e3d   row="5" column=
+00000680: 2230 223e 0a20 2020 203c 7769 6467 6574  "0">.    <widget
+00000690: 2063 6c61 7373 3d22 5153 7461 636b 6564   class="QStacked
+000006a0: 5769 6467 6574 2220 6e61 6d65 3d22 7374  Widget" name="st
+000006b0: 6163 6b65 6457 6964 6765 7422 3e0a 2020  ackedWidget">.  
+000006c0: 2020 203c 7769 6467 6574 2063 6c61 7373     <widget class
+000006d0: 3d22 5157 6964 6765 7422 206e 616d 653d  ="QWidget" name=
+000006e0: 2270 6167 6550 6172 7365 644e 6f44 6174  "pageParsedNoDat
+000006f0: 6122 3e0a 2020 2020 2020 3c6c 6179 6f75  a">.      <layou
+00000700: 7420 636c 6173 733d 2251 4772 6964 4c61  t class="QGridLa
+00000710: 796f 7574 2220 6e61 6d65 3d22 6772 6964  yout" name="grid
+00000720: 4c61 796f 7574 5f33 223e 0a20 2020 2020  Layout_3">.     
+00000730: 2020 3c69 7465 6d20 726f 773d 2230 2220    <item row="0" 
+00000740: 636f 6c75 6d6e 3d22 3022 3e0a 2020 2020  column="0">.    
+00000750: 2020 2020 3c77 6964 6765 7420 636c 6173      <widget clas
+00000760: 733d 2251 4c61 6265 6c22 206e 616d 653d  s="QLabel" name=
+00000770: 226c 6162 656c 223e 0a20 2020 2020 2020  "label">.       
+00000780: 2020 3c70 726f 7065 7274 7920 6e61 6d65    <property name
+00000790: 3d22 7465 7874 223e 0a20 2020 2020 2020  ="text">.       
+000007a0: 2020 203c 7374 7269 6e67 3e4e 6f20 7374     <string>No st
+000007b0: 7265 616d 2068 6173 2062 6565 6e20 6c6f  ream has been lo
+000007c0: 6164 6564 2e20 5472 7920 646f 7562 6c65  aded. Try double
+000007d0: 2063 6c69 636b 696e 6720 6f6e 6520 696e   clicking one in
+000007e0: 2074 6865 2074 7265 6520 7669 6577 2e3c   the tree view.<
+000007f0: 2f73 7472 696e 673e 0a20 2020 2020 2020  /string>.       
+00000800: 2020 3c2f 7072 6f70 6572 7479 3e0a 2020    </property>.  
+00000810: 2020 2020 2020 203c 7072 6f70 6572 7479         <property
+00000820: 206e 616d 653d 2261 6c69 676e 6d65 6e74   name="alignment
+00000830: 223e 0a20 2020 2020 2020 2020 203c 7365  ">.          <se
+00000840: 743e 5174 3a3a 416c 6967 6e43 656e 7465  t>Qt::AlignCente
+00000850: 723c 2f73 6574 3e0a 2020 2020 2020 2020  r</set>.        
+00000860: 203c 2f70 726f 7065 7274 793e 0a20 2020   </property>.   
+00000870: 2020 2020 2020 3c70 726f 7065 7274 7920        <property 
+00000880: 6e61 6d65 3d22 776f 7264 5772 6170 223e  name="wordWrap">
+00000890: 0a20 2020 2020 2020 2020 203c 626f 6f6c  .          <bool
+000008a0: 3e74 7275 653c 2f62 6f6f 6c3e 0a20 2020  >true</bool>.   
+000008b0: 2020 2020 2020 3c2f 7072 6f70 6572 7479        </property
+000008c0: 3e0a 2020 2020 2020 2020 3c2f 7769 6467  >.        </widg
+000008d0: 6574 3e0a 2020 2020 2020 203c 2f69 7465  et>.       </ite
+000008e0: 6d3e 0a20 2020 2020 203c 2f6c 6179 6f75  m>.      </layou
+000008f0: 743e 0a20 2020 2020 3c2f 7769 6467 6574  t>.     </widget
+00000900: 3e0a 2020 2020 203c 7769 6467 6574 2063  >.     <widget c
+00000910: 6c61 7373 3d22 5374 7269 6e67 5669 6577  lass="StringView
+00000920: 6572 2220 6e61 6d65 3d22 7061 6765 5061  er" name="pagePa
+00000930: 7273 6564 5374 7269 6e67 222f 3e0a 2020  rsedString"/>.  
+00000940: 2020 203c 7769 6467 6574 2063 6c61 7373     <widget class
+00000950: 3d22 4d75 6c74 6970 6c65 5669 6577 6572  ="MultipleViewer
+00000960: 2220 6e61 6d65 3d22 7061 6765 5061 7273  " name="pagePars
+00000970: 6564 4d75 6c74 6970 6c65 222f 3e0a 2020  edMultiple"/>.  
+00000980: 2020 203c 7769 6467 6574 2063 6c61 7373     <widget class
+00000990: 3d22 4d75 6c74 6970 6c65 4269 6e61 7279  ="MultipleBinary
+000009a0: 5669 6577 6572 2220 6e61 6d65 3d22 7061  Viewer" name="pa
+000009b0: 6765 5061 7273 6564 4d75 6c74 6970 6c65  geParsedMultiple
+000009c0: 4269 6e61 7279 222f 3e0a 2020 2020 203c  Binary"/>.     <
+000009d0: 7769 6467 6574 2063 6c61 7373 3d22 5072  widget class="Pr
+000009e0: 6f70 6572 7469 6573 5669 6577 6572 2220  opertiesViewer" 
+000009f0: 6e61 6d65 3d22 7061 6765 5061 7273 6564  name="pageParsed
+00000a00: 5072 6f70 6572 7469 6573 222f 3e0a 2020  Properties"/>.  
+00000a10: 2020 203c 7769 6467 6574 2063 6c61 7373     <widget class
+00000a20: 3d22 4775 6964 5669 6577 6572 2220 6e61  ="GuidViewer" na
+00000a30: 6d65 3d22 7061 6765 5061 7273 6564 4775  me="pageParsedGu
+00000a40: 6964 5669 6577 6572 222f 3e0a 2020 2020  idViewer"/>.    
+00000a50: 203c 7769 6467 6574 2063 6c61 7373 3d22   <widget class="
+00000a60: 4865 7856 6965 7765 7222 206e 616d 653d  HexViewer" name=
+00000a70: 2270 6167 6548 6578 5669 6577 6572 222f  "pageHexViewer"/
+00000a80: 3e0a 2020 2020 3c2f 7769 6467 6574 3e0a  >.    </widget>.
+00000a90: 2020 203c 2f69 7465 6d3e 0a20 2020 3c69     </item>.   <i
+00000aa0: 7465 6d20 726f 773d 2233 2220 636f 6c75  tem row="3" colu
+00000ab0: 6d6e 3d22 3022 3e0a 2020 2020 3c6c 6179  mn="0">.    <lay
+00000ac0: 6f75 7420 636c 6173 733d 2251 4842 6f78  out class="QHBox
+00000ad0: 4c61 796f 7574 2220 6e61 6d65 3d22 686f  Layout" name="ho
+00000ae0: 7269 7a6f 6e74 616c 4c61 796f 7574 5f33  rizontalLayout_3
+00000af0: 223e 0a20 2020 2020 3c69 7465 6d3e 0a20  ">.     <item>. 
+00000b00: 2020 2020 203c 7769 6467 6574 2063 6c61       <widget cla
+00000b10: 7373 3d22 514c 6162 656c 2220 6e61 6d65  ss="QLabel" name
+00000b20: 3d22 6c61 6265 6c5f 3222 3e0a 2020 2020  ="label_2">.    
+00000b30: 2020 203c 7072 6f70 6572 7479 206e 616d     <property nam
+00000b40: 653d 2274 6578 7422 3e0a 2020 2020 2020  e="text">.      
+00000b50: 2020 3c73 7472 696e 673e 4375 7272 656e    <string>Curren
+00000b60: 7420 5374 7265 616d 3a3c 2f73 7472 696e  t Stream:</strin
+00000b70: 673e 0a20 2020 2020 2020 3c2f 7072 6f70  g>.       </prop
+00000b80: 6572 7479 3e0a 2020 2020 2020 3c2f 7769  erty>.      </wi
+00000b90: 6467 6574 3e0a 2020 2020 203c 2f69 7465  dget>.     </ite
+00000ba0: 6d3e 0a20 2020 2020 3c69 7465 6d3e 0a20  m>.     <item>. 
+00000bb0: 2020 2020 203c 7769 6467 6574 2063 6c61       <widget cla
+00000bc0: 7373 3d22 514c 6162 656c 2220 6e61 6d65  ss="QLabel" name
+00000bd0: 3d22 6c61 6265 6c53 7472 6561 6d4e 616d  ="labelStreamNam
+00000be0: 6522 3e0a 2020 2020 2020 203c 7072 6f70  e">.       <prop
+00000bf0: 6572 7479 206e 616d 653d 2274 6578 7422  erty name="text"
+00000c00: 3e0a 2020 2020 2020 2020 3c73 7472 696e  >.        <strin
+00000c10: 673e 4e6f 6e65 3c2f 7374 7269 6e67 3e0a  g>None</string>.
+00000c20: 2020 2020 2020 203c 2f70 726f 7065 7274         </propert
+00000c30: 793e 0a20 2020 2020 203c 2f77 6964 6765  y>.      </widge
+00000c40: 743e 0a20 2020 2020 3c2f 6974 656d 3e0a  t>.     </item>.
+00000c50: 2020 2020 203c 6974 656d 3e0a 2020 2020       <item>.    
+00000c60: 2020 3c73 7061 6365 7220 6e61 6d65 3d22    <spacer name="
+00000c70: 686f 7269 7a6f 6e74 616c 5370 6163 6572  horizontalSpacer
+00000c80: 5f32 223e 0a20 2020 2020 2020 3c70 726f  _2">.       <pro
+00000c90: 7065 7274 7920 6e61 6d65 3d22 6f72 6965  perty name="orie
+00000ca0: 6e74 6174 696f 6e22 3e0a 2020 2020 2020  ntation">.      
+00000cb0: 2020 3c65 6e75 6d3e 5174 3a3a 486f 7269    <enum>Qt::Hori
+00000cc0: 7a6f 6e74 616c 3c2f 656e 756d 3e0a 2020  zontal</enum>.  
+00000cd0: 2020 2020 203c 2f70 726f 7065 7274 793e       </property>
+00000ce0: 0a20 2020 2020 2020 3c70 726f 7065 7274  .       <propert
+00000cf0: 7920 6e61 6d65 3d22 7369 7a65 4869 6e74  y name="sizeHint
+00000d00: 2220 7374 6473 6574 3d22 3022 3e0a 2020  " stdset="0">.  
+00000d10: 2020 2020 2020 3c73 697a 653e 0a20 2020        <size>.   
+00000d20: 2020 2020 2020 3c77 6964 7468 3e34 303c        <width>40<
+00000d30: 2f77 6964 7468 3e0a 2020 2020 2020 2020  /width>.        
+00000d40: 203c 6865 6967 6874 3e32 303c 2f68 6569   <height>20</hei
+00000d50: 6768 743e 0a20 2020 2020 2020 203c 2f73  ght>.        </s
+00000d60: 697a 653e 0a20 2020 2020 2020 3c2f 7072  ize>.       </pr
+00000d70: 6f70 6572 7479 3e0a 2020 2020 2020 3c2f  operty>.      </
+00000d80: 7370 6163 6572 3e0a 2020 2020 203c 2f69  spacer>.     </i
+00000d90: 7465 6d3e 0a20 2020 203c 2f6c 6179 6f75  tem>.    </layou
+00000da0: 743e 0a20 2020 3c2f 6974 656d 3e0a 2020  t>.   </item>.  
+00000db0: 3c2f 6c61 796f 7574 3e0a 203c 2f77 6964  </layout>. </wid
+00000dc0: 6765 743e 0a20 3c63 7573 746f 6d77 6964  get>. <customwid
+00000dd0: 6765 7473 3e0a 2020 3c63 7573 746f 6d77  gets>.  <customw
+00000de0: 6964 6765 743e 0a20 2020 3c63 6c61 7373  idget>.   <class
+00000df0: 3e48 6578 5669 6577 6572 3c2f 636c 6173  >HexViewer</clas
+00000e00: 733e 0a20 2020 3c65 7874 656e 6473 3e51  s>.   <extends>Q
+00000e10: 5769 6467 6574 3c2f 6578 7465 6e64 733e  Widget</extends>
+00000e20: 0a20 2020 3c68 6561 6465 723e 2e2e 6865  .   <header>..he
+00000e30: 785f 7669 6577 6572 3c2f 6865 6164 6572  x_viewer</header
+00000e40: 3e0a 2020 203c 636f 6e74 6169 6e65 723e  >.   <container>
+00000e50: 313c 2f63 6f6e 7461 696e 6572 3e0a 2020  1</container>.  
+00000e60: 3c2f 6375 7374 6f6d 7769 6467 6574 3e0a  </customwidget>.
+00000e70: 2020 3c63 7573 746f 6d77 6964 6765 743e    <customwidget>
+00000e80: 0a20 2020 3c63 6c61 7373 3e4d 756c 7469  .   <class>Multi
+00000e90: 706c 6542 696e 6172 7956 6965 7765 723c  pleBinaryViewer<
+00000ea0: 2f63 6c61 7373 3e0a 2020 203c 6578 7465  /class>.   <exte
+00000eb0: 6e64 733e 5157 6964 6765 743c 2f65 7874  nds>QWidget</ext
+00000ec0: 656e 6473 3e0a 2020 203c 6865 6164 6572  ends>.   <header
+00000ed0: 3e2e 2e6d 756c 7469 706c 655f 6269 6e61  >..multiple_bina
+00000ee0: 7279 5f76 6965 7765 723c 2f68 6561 6465  ry_viewer</heade
+00000ef0: 723e 0a20 2020 3c63 6f6e 7461 696e 6572  r>.   <container
+00000f00: 3e31 3c2f 636f 6e74 6169 6e65 723e 0a20  >1</container>. 
+00000f10: 203c 2f63 7573 746f 6d77 6964 6765 743e   </customwidget>
+00000f20: 0a20 203c 6375 7374 6f6d 7769 6467 6574  .  <customwidget
+00000f30: 3e0a 2020 203c 636c 6173 733e 4d75 6c74  >.   <class>Mult
+00000f40: 6970 6c65 5669 6577 6572 3c2f 636c 6173  ipleViewer</clas
+00000f50: 733e 0a20 2020 3c65 7874 656e 6473 3e51  s>.   <extends>Q
+00000f60: 5769 6467 6574 3c2f 6578 7465 6e64 733e  Widget</extends>
+00000f70: 0a20 2020 3c68 6561 6465 723e 2e2e 6d75  .   <header>..mu
+00000f80: 6c74 6970 6c65 5f76 6965 7765 723c 2f68  ltiple_viewer</h
+00000f90: 6561 6465 723e 0a20 2020 3c63 6f6e 7461  eader>.   <conta
+00000fa0: 696e 6572 3e31 3c2f 636f 6e74 6169 6e65  iner>1</containe
+00000fb0: 723e 0a20 203c 2f63 7573 746f 6d77 6964  r>.  </customwid
+00000fc0: 6765 743e 0a20 203c 6375 7374 6f6d 7769  get>.  <customwi
+00000fd0: 6467 6574 3e0a 2020 203c 636c 6173 733e  dget>.   <class>
+00000fe0: 5374 7269 6e67 5669 6577 6572 3c2f 636c  StringViewer</cl
+00000ff0: 6173 733e 0a20 2020 3c65 7874 656e 6473  ass>.   <extends
+00001000: 3e51 5769 6467 6574 3c2f 6578 7465 6e64  >QWidget</extend
+00001010: 733e 0a20 2020 3c68 6561 6465 723e 2e2e  s>.   <header>..
+00001020: 7374 7269 6e67 5f76 6965 7765 723c 2f68  string_viewer</h
+00001030: 6561 6465 723e 0a20 2020 3c63 6f6e 7461  eader>.   <conta
+00001040: 696e 6572 3e31 3c2f 636f 6e74 6169 6e65  iner>1</containe
+00001050: 723e 0a20 203c 2f63 7573 746f 6d77 6964  r>.  </customwid
+00001060: 6765 743e 0a20 203c 6375 7374 6f6d 7769  get>.  <customwi
+00001070: 6467 6574 3e0a 2020 203c 636c 6173 733e  dget>.   <class>
+00001080: 5072 6f70 6572 7469 6573 5669 6577 6572  PropertiesViewer
+00001090: 3c2f 636c 6173 733e 0a20 2020 3c65 7874  </class>.   <ext
+000010a0: 656e 6473 3e51 5769 6467 6574 3c2f 6578  ends>QWidget</ex
+000010b0: 7465 6e64 733e 0a20 2020 3c68 6561 6465  tends>.   <heade
+000010c0: 723e 2e2e 7072 6f70 6572 7469 6573 5f76  r>..properties_v
+000010d0: 6965 7765 723c 2f68 6561 6465 723e 0a20  iewer</header>. 
+000010e0: 2020 3c63 6f6e 7461 696e 6572 3e31 3c2f    <container>1</
+000010f0: 636f 6e74 6169 6e65 723e 0a20 203c 2f63  container>.  </c
+00001100: 7573 746f 6d77 6964 6765 743e 0a20 203c  ustomwidget>.  <
+00001110: 6375 7374 6f6d 7769 6467 6574 3e0a 2020  customwidget>.  
+00001120: 203c 636c 6173 733e 4775 6964 5669 6577   <class>GuidView
+00001130: 6572 3c2f 636c 6173 733e 0a20 2020 3c65  er</class>.   <e
+00001140: 7874 656e 6473 3e51 5769 6467 6574 3c2f  xtends>QWidget</
+00001150: 6578 7465 6e64 733e 0a20 2020 3c68 6561  extends>.   <hea
+00001160: 6465 723e 2e2e 6775 6964 5f76 6965 7765  der>..guid_viewe
+00001170: 723c 2f68 6561 6465 723e 0a20 2020 3c63  r</header>.   <c
+00001180: 6f6e 7461 696e 6572 3e31 3c2f 636f 6e74  ontainer>1</cont
+00001190: 6169 6e65 723e 0a20 203c 2f63 7573 746f  ainer>.  </custo
+000011a0: 6d77 6964 6765 743e 0a20 3c2f 6375 7374  mwidget>. </cust
+000011b0: 6f6d 7769 6467 6574 733e 0a20 3c72 6573  omwidgets>. <res
+000011c0: 6f75 7263 6573 2f3e 0a20 3c63 6f6e 6e65  ources/>. <conne
+000011d0: 6374 696f 6e73 2f3e 0a3c 2f75 693e 0a    ctions/>.</ui>.
```

### Comparing `msg_explorer-1.6.0/msg_explorer/ui/string_viewer.ui` & `msg_explorer-1.7.0/msg_explorer/ui/loading_screen.ui`

 * *Files 23% similar despite different names*

#### Comparing `msg_explorer-1.6.0/msg_explorer/ui/string_viewer.ui` & `msg_explorer-1.7.0/msg_explorer/ui/loading_screen.ui`

```diff
@@ -1,37 +1,43 @@
 <?xml version="1.0" encoding="utf-8"?>
 <ui version="4.0">
-  <class>StringViewer</class>
-  <widget class="QWidget" name="StringViewer">
+  <class>LoadingScreen</class>
+  <widget class="QWidget" name="LoadingScreen">
     <property name="geometry">
       <rect>
         <x>0</x>
         <y>0</y>
-        <width>800</width>
-        <height>600</height>
+        <width>400</width>
+        <height>150</height>
       </rect>
     </property>
     <property name="windowTitle">
-      <string>StringViewer</string>
+      <string>Loading...</string>
     </property>
     <layout class="QGridLayout" name="gridLayout">
       <item row="0" column="0">
-        <widget class="QLabel" name="labelType">
+        <widget class="QLabel" name="loadingMessage">
+          <property name="layoutDirection">
+            <enum>Qt::LeftToRight</enum>
+          </property>
           <property name="text">
-            <string/>
+            <string>Loading MSG file, please wait...</string>
+          </property>
+          <property name="alignment">
+            <set>Qt::AlignCenter</set>
           </property>
         </widget>
       </item>
       <item row="1" column="0">
-        <widget class="QPlainTextEdit" name="textDisplay">
-          <property name="lineWrapMode">
-            <enum>QPlainTextEdit::NoWrap</enum>
+        <widget class="QProgressBar" name="progressBar">
+          <property name="maximum">
+            <number>0</number>
           </property>
-          <property name="readOnly">
-            <bool>true</bool>
+          <property name="value">
+            <number>-1</number>
           </property>
         </widget>
       </item>
     </layout>
   </widget>
   <resources/>
   <connections/>
```

### Comparing `msg_explorer-1.6.0/msg_explorer/ui/unhandled_exception.ui` & `msg_explorer-1.7.0/msg_explorer/ui/msg_tree_viewer.ui`

 * *Files 23% similar despite different names*

#### Comparing `msg_explorer-1.6.0/msg_explorer/ui/unhandled_exception.ui` & `msg_explorer-1.7.0/msg_explorer/ui/msg_tree_viewer.ui`

```diff
@@ -1,44 +1,48 @@
 <?xml version="1.0" encoding="utf-8"?>
 <ui version="4.0">
-  <class>UnhandledException</class>
-  <widget class="QDialog" name="UnhandledException">
+  <class>MSGTreeViewer</class>
+  <widget class="QWidget" name="MSGTreeViewer">
     <property name="geometry">
       <rect>
         <x>0</x>
         <y>0</y>
-        <width>588</width>
-        <height>479</height>
+        <width>400</width>
+        <height>300</height>
       </rect>
     </property>
     <property name="windowTitle">
-      <string>Unhandled Exception</string>
+      <string>Form</string>
     </property>
     <layout class="QGridLayout" name="gridLayout">
-      <item row="1" column="0">
-        <widget class="QPlainTextEdit" name="traceback">
-          <property name="lineWrapMode">
-            <enum>QPlainTextEdit::NoWrap</enum>
+      <item row="0" column="0">
+        <widget class="QTreeWidget" name="treeWidget">
+          <property name="editTriggers">
+            <set>QAbstractItemView::NoEditTriggers</set>
+          </property>
+          <property name="verticalScrollMode">
+            <enum>QAbstractItemView::ScrollPerPixel</enum>
           </property>
-          <property name="readOnly">
+          <property name="sortingEnabled">
             <bool>true</bool>
           </property>
-          <property name="plainText">
-            <string/>
+          <property name="headerHidden">
+            <bool>false</bool>
           </property>
-        </widget>
-      </item>
-      <item row="0" column="0">
-        <widget class="QLabel" name="label">
-          <property name="text">
-            <string>An unhandled exception has occured. Please report this to the developers.</string>
-          </property>
-          <property name="wordWrap">
+          <attribute name="headerDefaultSectionSize">
+            <number>400</number>
+          </attribute>
+          <attribute name="headerStretchLastSection">
             <bool>true</bool>
-          </property>
+          </attribute>
+          <column>
+            <property name="text">
+              <string notr="true">Name</string>
+            </property>
+          </column>
         </widget>
       </item>
     </layout>
   </widget>
   <resources/>
   <connections/>
 </ui>
```

### Comparing `msg_explorer-1.6.0/msg_explorer.egg-info/PKG-INFO` & `msg_explorer-1.7.0/README.rst`

 * *Files 15% similar despite different names*

```diff
@@ -1,114 +1,94 @@
-Metadata-Version: 2.1
-Name: msg-explorer
-Version: 1.6.0
-Summary: A GUI program to allow for exploring MSG files using extract-msg.
-Home-page: https://github.com/TeamMsgExtractor/msg-explorer
-Author: Destiny Peterson
-Author-email: arceusthe@gmail.com
-License: GPL
-Download-URL: https://github.com/TeamMsgExtractor/msg-explorer/archives/master
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
-Description-Content-Type: text/x-rst
-License-File: LICENSE.txt
-
-|License: GPL v3| |PyPI3| |PyPI2|
-
-msg-explorer
-=============
-
-Allows for the graphical browsing of Outlook Message Files and their data.
-
-While normally intended as a development tool, it is fine to use as a normal
-user.
-
-If you'd like to help provide translations, you can contact me on the Discord.
-
-NOTICE
-======
-
-This module has a Discord server for general discussion. It is the same Discord
-as msg-extractor. You can find it here: `Discord`_
-
-
-Changelog
----------
--  `Changelog`_
-
-Usage
------
-
-The module installs a script called msg_explorer but can also be run using the
-following command:
-::
-
-     python -m msg_explorer
-
-
-If you have any questions feel free to contact me, Destiny, at arceusthe [at]
-gmail [dot] com.
-
-If you have issues, it would be best to get help for them by opening a
-new github issue.
-
-Error Reporting
----------------
-
-Should you encounter an error that has not already been reported, please
-do the following when reporting it: \* Make sure you are using the
-latest version of msg-explorer (check the version on PyPi). \* State your
-Python version. \* Include the code, if any, that you used. \* Include a
-copy of the traceback.
-
-Supporting The Module
----------------------
-
-If you'd like to donate to help support the development of the module, you can
-donate to Destiny using one of the following services:
-
-* `Buy Me a Coffee`_
-* `Ko-fi`_
-* `Patreon`_
-
-Installation
-------------
-
-You can install using pip:
-
--  Pypi
-
-.. code:: bash
-
-       pip install msg-explorer
-
--  Github
-
-.. code:: sh
-
-     pip install git+https://github.com/TeamMsgExtractor/msg-explorer
-
-Credits
--------
-
-`Destiny Peterson (The Elemental of Destruction)`_ - Main Programmer.
-
-.. |License: GPL v3| image:: https://img.shields.io/badge/License-GPLv3-blue.svg
-   :target: LICENSE.txt
-
-.. |PyPI3| image:: https://img.shields.io/badge/pypi-1.6.0-blue.svg
-   :target: https://pypi.org/project/msg-explorer/1.6.0/
-
-.. |PyPI2| image:: https://img.shields.io/badge/python-3.8+-brightgreen.svg
-   :target: https://www.python.org/downloads/release/python-3816/
-.. _Destiny Peterson (The Elemental of Destruction): https://github.com/TheElementalOfDestruction
-.. _Discord: https://discord.com/invite/B77McRmzdc
-.. _Buy Me a Coffee: https://www.buymeacoffee.com/DestructionE
-.. _Ko-fi: https://ko-fi.com/destructione
-.. _Patreon: https://www.patreon.com/DestructionE
-.. _Changelog: https://github.com/TeamMsgExtractor/msg-explorer/blob/master/CHANGELOG.md
-
-
+|License: GPL v3| |PyPI3| |PyPI2|
+
+msg-explorer
+=============
+
+Allows for the graphical browsing of Outlook Message Files and their data.
+
+While normally intended as a development tool, it is fine to use as a normal
+user.
+
+If you'd like to help provide translations, you can contact me on the Discord.
+
+NOTICE
+======
+
+This module has a Discord server for general discussion. It is the same Discord
+as msg-extractor. You can find it here: `Discord`_
+
+
+Changelog
+---------
+-  `Changelog`_
+
+Usage
+-----
+
+The module installs a script called msg_explorer but can also be run using the
+following command:
+::
+
+     python -m msg_explorer
+
+
+If you have any questions feel free to contact me, Destiny, at arceusthe [at]
+gmail [dot] com.
+
+If you have issues, it would be best to get help for them by opening a
+new github issue.
+
+Error Reporting
+---------------
+
+Should you encounter an error that has not already been reported, please
+do the following when reporting it: \* Make sure you are using the
+latest version of msg-explorer (check the version on PyPi). \* State your
+Python version. \* Include the code, if any, that you used. \* Include a
+copy of the traceback.
+
+Supporting The Module
+---------------------
+
+If you'd like to donate to help support the development of the module, you can
+donate to Destiny using one of the following services:
+
+* `Buy Me a Coffee`_
+* `Ko-fi`_
+* `Patreon`_
+
+Installation
+------------
+
+You can install using pip:
+
+-  Pypi
+
+.. code:: bash
+
+       pip install msg-explorer
+
+-  Github
+
+.. code:: sh
+
+     pip install git+https://github.com/TeamMsgExtractor/msg-explorer
+
+Credits
+-------
+
+`Destiny Peterson (The Elemental of Destruction)`_ - Main Programmer.
+
+.. |License: GPL v3| image:: https://img.shields.io/badge/License-GPLv3-blue.svg
+   :target: LICENSE.txt
+
+.. |PyPI3| image:: https://img.shields.io/badge/pypi-1.7.0-blue.svg
+   :target: https://pypi.org/project/msg-explorer/1.7.0/
+
+.. |PyPI2| image:: https://img.shields.io/badge/python-3.8+-brightgreen.svg
+   :target: https://www.python.org/downloads/release/python-3816/
+.. _Destiny Peterson (The Elemental of Destruction): https://github.com/TheElementalOfDestruction
+.. _Discord: https://discord.com/invite/B77McRmzdc
+.. _Buy Me a Coffee: https://www.buymeacoffee.com/DestructionE
+.. _Ko-fi: https://ko-fi.com/destructione
+.. _Patreon: https://www.patreon.com/DestructionE
+.. _Changelog: https://github.com/TeamMsgExtractor/msg-explorer/blob/master/CHANGELOG.md
```

### Comparing `msg_explorer-1.6.0/setup.py` & `msg_explorer-1.7.0/setup.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,57 +1,57 @@
-import os
-from setuptools import setup
-import re
-
-
-# A handful of variables that are used a couple of times.
-github_url = 'https://github.com/TeamMsgExtractor/msg-explorer'
-main_module = 'msg_explorer'
-
-# Read in the description from README.
-with open('README.rst', 'rb') as stream:
-    long_description = stream.read().decode('utf-8').replace('\r', '')
-
-# Get the version this way to avoid import issues.
-version_re = re.compile("__version__ = '(?P<version>[0-9\\.]*)'")
-with open('msg_explorer/__init__.py', 'r') as stream:
-    contents = stream.read()
-match = version_re.search(contents)
-version = match.groupdict()['version']
-
-# Read in the dependencies from the virtualenv requirements file.
-dependencies = []
-filename = os.path.join('requirements.txt')
-with open(filename, 'r') as stream:
-    for line in stream:
-        package = line.strip().split('#')[0]
-        if package:
-            dependencies.append(package)
-
-classifiers = [
-    'Development Status :: 5 - Production/Stable',
-    'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
-    'Operating System :: OS Independent',
-    'Programming Language :: Python :: 3',
-]
-
-
-
-setup(
-    name=main_module,
-    version=version,
-    description="A GUI program to allow for exploring MSG files using extract-msg.",
-    long_description=long_description,
-    long_description_content_type='text/x-rst',
-    url=github_url,
-    download_url='%s/archives/master' % github_url,
-    author='Destiny Peterson',
-    author_email='arceusthe@gmail.com',
-    license='GPL',
-    packages=[main_module],
-    py_modules=[main_module],
-    entry_points={'console_scripts': ['msg_explorer = msg_explorer.main:mainRunner',]},
-    include_package_data=True,
-    install_requires=dependencies,
-    classifiers=classifiers,
-    python_requires='>=3.8'
-)
+import os
+from setuptools import setup
+import re
+
+
+# A handful of variables that are used a couple of times.
+github_url = 'https://github.com/TeamMsgExtractor/msg-explorer'
+main_module = 'msg_explorer'
+
+# Read in the description from README.
+with open('README.rst', 'rb') as stream:
+    long_description = stream.read().decode('utf-8').replace('\r', '')
+
+# Get the version this way to avoid import issues.
+version_re = re.compile("__version__ = '(?P<version>[0-9\\.]*)'")
+with open('msg_explorer/__init__.py', 'r') as stream:
+    contents = stream.read()
+match = version_re.search(contents)
+version = match.groupdict()['version']
+
+# Read in the dependencies from the virtualenv requirements file.
+dependencies = []
+filename = os.path.join('requirements.txt')
+with open(filename, 'r') as stream:
+    for line in stream:
+        package = line.strip().split('#')[0]
+        if package:
+            dependencies.append(package)
+
+classifiers = [
+    'Development Status :: 5 - Production/Stable',
+    'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
+    'Operating System :: OS Independent',
+    'Programming Language :: Python :: 3',
+]
+
+
+
+setup(
+    name=main_module,
+    version=version,
+    description="A GUI program to allow for exploring MSG files using extract-msg.",
+    long_description=long_description,
+    long_description_content_type='text/x-rst',
+    url=github_url,
+    download_url='%s/archives/master' % github_url,
+    author='Destiny Peterson',
+    author_email='arceusthe@gmail.com',
+    license='GPL',
+    packages=[main_module],
+    py_modules=[main_module],
+    entry_points={'console_scripts': ['msg_explorer = msg_explorer.main:mainRunner',]},
+    include_package_data=True,
+    install_requires=dependencies,
+    classifiers=classifiers,
+    python_requires='>=3.8'
+)
```

