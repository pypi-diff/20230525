# Comparing `tmp/nxselector-3.18.4.tar.gz` & `tmp/nxselector-3.19.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nxselector-3.18.4.tar", last modified: Thu Dec  8 08:37:31 2022, max compression
+gzip compressed data, was "nxselector-3.19.0.tar", last modified: Thu May 25 14:20:18 2023, max compression
```

## Comparing `nxselector-3.18.4.tar` & `nxselector-3.19.0.tar`

### file list

```diff
@@ -1,59 +1,58 @@
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2022-12-08 08:37:31.000000 nxselector-3.18.4/
--rw-r--r--   0 jkotan   (15949) irc         (39)    35147 2015-04-27 14:05:27.000000 nxselector-3.18.4/COPYRIGHT
--rw-r--r--   0 jkotan   (15949) irc         (39)      184 2016-05-31 11:55:41.000000 nxselector-3.18.4/MANIFEST.in
--rw-r--r--   0 jkotan   (15949) irc         (39)    13808 2022-12-08 08:37:31.000000 nxselector-3.18.4/PKG-INFO
--rw-r--r--   0 jkotan   (15949) irc         (39)    10354 2022-12-08 07:21:53.000000 nxselector-3.18.4/README.rst
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2022-12-08 08:37:31.000000 nxselector-3.18.4/man/
--rw-r--r--   0 jkotan   (15949) irc         (39)      875 2016-02-22 11:01:13.000000 nxselector-3.18.4/man/nxselector.1
--rwxr-xr-x   0 jkotan   (15949) irc         (39)     1068 2019-10-16 18:20:14.000000 nxselector-3.18.4/nxselector
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2022-12-08 08:37:31.000000 nxselector-3.18.4/nxselector.egg-info/
--rw-r--r--   0 jkotan   (15949) irc         (39)    13808 2022-12-08 08:37:31.000000 nxselector-3.18.4/nxselector.egg-info/PKG-INFO
--rw-r--r--   0 jkotan   (15949) irc         (39)     1247 2022-12-08 08:37:31.000000 nxselector-3.18.4/nxselector.egg-info/SOURCES.txt
--rw-r--r--   0 jkotan   (15949) irc         (39)        1 2022-12-08 08:37:31.000000 nxselector-3.18.4/nxselector.egg-info/dependency_links.txt
--rw-r--r--   0 jkotan   (15949) irc         (39)        1 2022-12-08 08:36:31.000000 nxselector-3.18.4/nxselector.egg-info/not-zip-safe
--rw-r--r--   0 jkotan   (15949) irc         (39)        7 2022-12-08 08:37:31.000000 nxselector-3.18.4/nxselector.egg-info/requires.txt
--rw-r--r--   0 jkotan   (15949) irc         (39)       43 2022-12-08 08:37:31.000000 nxselector-3.18.4/nxselector.egg-info/top_level.txt
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2022-12-08 08:37:31.000000 nxselector-3.18.4/nxsselector/
--rw-r--r--   0 jkotan   (15949) irc         (39)     5920 2020-03-09 13:50:16.000000 nxselector-3.18.4/nxsselector/AddDataSourceDlg.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     2208 2019-01-16 11:55:28.000000 nxselector-3.18.4/nxsselector/CommandThread.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     3391 2019-01-16 11:55:28.000000 nxselector-3.18.4/nxsselector/Data.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    10030 2021-09-02 06:43:42.000000 nxselector-3.18.4/nxsselector/Descriptions.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    12784 2022-03-31 08:45:32.000000 nxselector-3.18.4/nxsselector/Detectors.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     4060 2019-01-16 11:55:28.000000 nxselector-3.18.4/nxsselector/DynamicTools.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     4082 2019-01-16 11:55:28.000000 nxselector-3.18.4/nxsselector/EdDataDlg.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     9561 2020-08-10 09:35:40.000000 nxselector-3.18.4/nxsselector/EdListDlg.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    12723 2019-01-16 10:26:31.000000 nxselector-3.18.4/nxsselector/Element.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    20267 2020-07-21 15:17:27.000000 nxselector-3.18.4/nxsselector/ElementModel.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     4895 2019-01-16 11:55:28.000000 nxselector-3.18.4/nxsselector/Frames.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     6093 2020-03-09 13:50:16.000000 nxselector-3.18.4/nxsselector/GroupsDlg.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     1920 2019-01-16 11:55:28.000000 nxselector-3.18.4/nxsselector/InfoDlg.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    10574 2022-08-16 12:07:32.000000 nxselector-3.18.4/nxsselector/LDataDlg.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     3434 2022-12-08 07:21:53.000000 nxselector-3.18.4/nxsselector/MessageBox.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     6011 2019-01-16 11:55:28.000000 nxselector-3.18.4/nxsselector/OrderDlg.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    19833 2022-12-08 07:21:53.000000 nxselector-3.18.4/nxsselector/Preferences.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    11086 2019-05-17 11:28:21.000000 nxselector-3.18.4/nxsselector/PropertiesDlg.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    54798 2022-06-01 06:32:50.000000 nxselector-3.18.4/nxsselector/Selector.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    46421 2022-12-08 07:21:53.000000 nxselector-3.18.4/nxsselector/ServerState.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    34029 2022-06-01 06:32:50.000000 nxselector-3.18.4/nxsselector/Storage.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    35317 2022-12-08 08:35:56.000000 nxselector-3.18.4/nxsselector/Views.py
--rw-r--r--   0 jkotan   (15949) irc         (39)      976 2022-12-08 08:35:56.000000 nxselector-3.18.4/nxsselector/__init__.py
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2022-12-08 08:37:31.000000 nxselector-3.18.4/nxsselector/images/
--rw-r--r--   0 jkotan   (15949) irc         (39)    23015 2016-02-22 11:01:13.000000 nxselector-3.18.4/nxsselector/images/network_folder.png
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2022-12-08 08:37:31.000000 nxselector-3.18.4/nxsselector/qrc/
--rw-r--r--   0 jkotan   (15949) irc         (39)      819 2017-03-16 07:56:31.000000 nxselector-3.18.4/nxsselector/qrc/__init__.py
--rw-r--r--   0 jkotan   (15949) irc         (39)      272 2016-02-22 11:01:13.000000 nxselector-3.18.4/nxsselector/qrc/resources.qrc
--rw-r--r--   0 jkotan   (15949) irc         (39)     1216 2022-06-01 06:32:50.000000 nxselector-3.18.4/nxsselector/qtapi.py
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2022-12-08 08:37:31.000000 nxselector-3.18.4/nxsselector/ui/
--rw-r--r--   0 jkotan   (15949) irc         (39)     3274 2018-10-11 11:16:52.000000 nxselector-3.18.4/nxsselector/ui/AddDataSourceDlg.ui
--rw-r--r--   0 jkotan   (15949) irc         (39)     2924 2019-09-05 14:04:55.000000 nxselector-3.18.4/nxsselector/ui/EdDataDlg.ui
--rw-r--r--   0 jkotan   (15949) irc         (39)     1142 2016-02-22 11:01:13.000000 nxselector-3.18.4/nxsselector/ui/EdListWg.ui
--rw-r--r--   0 jkotan   (15949) irc         (39)     1125 2018-10-11 11:16:52.000000 nxselector-3.18.4/nxsselector/ui/GroupsDlg.ui
--rw-r--r--   0 jkotan   (15949) irc         (39)     4108 2016-02-22 11:01:13.000000 nxselector-3.18.4/nxsselector/ui/InfoDlg.ui
--rw-r--r--   0 jkotan   (15949) irc         (39)     9738 2019-09-05 13:56:28.000000 nxselector-3.18.4/nxsselector/ui/LDataDlg.ui
--rw-r--r--   0 jkotan   (15949) irc         (39)     1147 2016-02-22 11:01:13.000000 nxselector-3.18.4/nxsselector/ui/OrderDlg.ui
--rw-r--r--   0 jkotan   (15949) irc         (39)    52079 2022-03-24 09:03:06.000000 nxselector-3.18.4/nxsselector/ui/Selector.ui
--rw-r--r--   0 jkotan   (15949) irc         (39)      819 2017-03-16 07:56:31.000000 nxselector-3.18.4/nxsselector/ui/__init__.py
--rw-r--r--   0 jkotan   (15949) irc         (39)      207 2022-12-08 08:37:31.000000 nxselector-3.18.4/setup.cfg
--rw-r--r--   0 jkotan   (15949) irc         (39)     7237 2022-12-08 08:37:00.000000 nxselector-3.18.4/setup.py
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2022-12-08 08:37:31.000000 nxselector-3.18.4/test/
--rw-r--r--   0 jkotan   (15949) irc         (39)     2182 2019-10-16 16:59:28.000000 nxselector-3.18.4/test/testmy.py
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-05-25 14:20:18.569716 nxselector-3.19.0/
+-rw-r--r--   0 jkotan   (15949) irc         (39)    35147 2015-04-27 14:05:27.000000 nxselector-3.19.0/COPYRIGHT
+-rw-r--r--   0 jkotan   (15949) irc         (39)      184 2023-05-22 08:52:51.000000 nxselector-3.19.0/MANIFEST.in
+-rw-r--r--   0 jkotan   (15949) irc         (39)    13808 2023-05-25 14:20:18.569716 nxselector-3.19.0/PKG-INFO
+-rw-r--r--   0 jkotan   (15949) irc         (39)    10354 2023-05-22 08:52:51.000000 nxselector-3.19.0/README.rst
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-05-25 14:20:18.565716 nxselector-3.19.0/man/
+-rw-r--r--   0 jkotan   (15949) irc         (39)      875 2023-05-22 08:52:51.000000 nxselector-3.19.0/man/nxselector.1
+-rwxr-xr-x   0 jkotan   (15949) irc         (39)     1068 2023-05-22 08:52:51.000000 nxselector-3.19.0/nxselector
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-05-25 14:20:18.565716 nxselector-3.19.0/nxselector.egg-info/
+-rw-r--r--   0 jkotan   (15949) irc         (39)    13808 2023-05-25 14:20:18.000000 nxselector-3.19.0/nxselector.egg-info/PKG-INFO
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1214 2023-05-25 14:20:18.000000 nxselector-3.19.0/nxselector.egg-info/SOURCES.txt
+-rw-r--r--   0 jkotan   (15949) irc         (39)        1 2023-05-25 14:20:18.000000 nxselector-3.19.0/nxselector.egg-info/dependency_links.txt
+-rw-r--r--   0 jkotan   (15949) irc         (39)        1 2022-12-08 08:36:31.000000 nxselector-3.19.0/nxselector.egg-info/not-zip-safe
+-rw-r--r--   0 jkotan   (15949) irc         (39)       43 2023-05-25 14:20:18.000000 nxselector-3.19.0/nxselector.egg-info/top_level.txt
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-05-25 14:20:18.569716 nxselector-3.19.0/nxsselector/
+-rw-r--r--   0 jkotan   (15949) irc         (39)     5920 2023-05-22 08:52:51.000000 nxselector-3.19.0/nxsselector/AddDataSourceDlg.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     2208 2023-05-22 08:52:51.000000 nxselector-3.19.0/nxsselector/CommandThread.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3391 2023-05-22 08:52:51.000000 nxselector-3.19.0/nxsselector/Data.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    10030 2023-05-22 08:52:51.000000 nxselector-3.19.0/nxsselector/Descriptions.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    12784 2023-05-22 08:52:51.000000 nxselector-3.19.0/nxsselector/Detectors.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     4060 2023-05-22 08:52:51.000000 nxselector-3.19.0/nxsselector/DynamicTools.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     4082 2023-05-22 08:52:51.000000 nxselector-3.19.0/nxsselector/EdDataDlg.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     9561 2023-05-22 08:52:51.000000 nxselector-3.19.0/nxsselector/EdListDlg.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    12723 2023-05-22 08:52:51.000000 nxselector-3.19.0/nxsselector/Element.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    20267 2023-05-22 08:52:51.000000 nxselector-3.19.0/nxsselector/ElementModel.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     4895 2023-05-22 08:52:51.000000 nxselector-3.19.0/nxsselector/Frames.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     6093 2023-05-22 08:52:51.000000 nxselector-3.19.0/nxsselector/GroupsDlg.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1920 2023-05-22 08:52:51.000000 nxselector-3.19.0/nxsselector/InfoDlg.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    10574 2023-05-22 08:52:51.000000 nxselector-3.19.0/nxsselector/LDataDlg.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3434 2023-05-22 08:52:51.000000 nxselector-3.19.0/nxsselector/MessageBox.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     6011 2023-05-22 08:52:51.000000 nxselector-3.19.0/nxsselector/OrderDlg.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    20113 2023-05-25 14:20:10.000000 nxselector-3.19.0/nxsselector/Preferences.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    11086 2023-05-22 08:52:51.000000 nxselector-3.19.0/nxsselector/PropertiesDlg.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    56155 2023-05-25 11:34:47.000000 nxselector-3.19.0/nxsselector/Selector.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    46631 2023-05-25 11:34:47.000000 nxselector-3.19.0/nxsselector/ServerState.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    34549 2023-05-25 11:34:47.000000 nxselector-3.19.0/nxsselector/Storage.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    37141 2023-05-25 14:20:10.000000 nxselector-3.19.0/nxsselector/Views.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)      976 2023-05-25 11:34:47.000000 nxselector-3.19.0/nxsselector/__init__.py
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-05-25 14:20:18.569716 nxselector-3.19.0/nxsselector/images/
+-rw-r--r--   0 jkotan   (15949) irc         (39)    23015 2023-05-22 08:52:51.000000 nxselector-3.19.0/nxsselector/images/network_folder.png
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-05-25 14:20:18.569716 nxselector-3.19.0/nxsselector/qrc/
+-rw-r--r--   0 jkotan   (15949) irc         (39)      819 2023-05-22 08:52:51.000000 nxselector-3.19.0/nxsselector/qrc/__init__.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)      272 2023-05-22 08:52:51.000000 nxselector-3.19.0/nxsselector/qrc/resources.qrc
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1216 2023-05-22 08:52:51.000000 nxselector-3.19.0/nxsselector/qtapi.py
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-05-25 14:20:18.569716 nxselector-3.19.0/nxsselector/ui/
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3274 2023-05-22 08:52:51.000000 nxselector-3.19.0/nxsselector/ui/AddDataSourceDlg.ui
+-rw-r--r--   0 jkotan   (15949) irc         (39)     2924 2023-05-22 08:52:51.000000 nxselector-3.19.0/nxsselector/ui/EdDataDlg.ui
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1142 2023-05-22 08:52:51.000000 nxselector-3.19.0/nxsselector/ui/EdListWg.ui
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1125 2023-05-22 08:52:51.000000 nxselector-3.19.0/nxsselector/ui/GroupsDlg.ui
+-rw-r--r--   0 jkotan   (15949) irc         (39)     4108 2023-05-22 08:52:51.000000 nxselector-3.19.0/nxsselector/ui/InfoDlg.ui
+-rw-r--r--   0 jkotan   (15949) irc         (39)     9738 2023-05-22 08:52:51.000000 nxselector-3.19.0/nxsselector/ui/LDataDlg.ui
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1147 2023-05-22 08:52:51.000000 nxselector-3.19.0/nxsselector/ui/OrderDlg.ui
+-rw-r--r--   0 jkotan   (15949) irc         (39)    54547 2023-05-25 11:34:47.000000 nxselector-3.19.0/nxsselector/ui/Selector.ui
+-rw-r--r--   0 jkotan   (15949) irc         (39)      819 2023-05-22 08:52:51.000000 nxselector-3.19.0/nxsselector/ui/__init__.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)      207 2023-05-25 14:20:18.573716 nxselector-3.19.0/setup.cfg
+-rw-r--r--   0 jkotan   (15949) irc         (39)     7239 2023-05-25 11:34:47.000000 nxselector-3.19.0/setup.py
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-05-25 14:20:18.569716 nxselector-3.19.0/test/
+-rw-r--r--   0 jkotan   (15949) irc         (39)     2182 2019-10-16 16:59:28.000000 nxselector-3.19.0/test/testmy.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `nxselector-3.18.4/COPYRIGHT` & `nxselector-3.19.0/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `nxselector-3.18.4/PKG-INFO` & `nxselector-3.19.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: nxselector
-Version: 3.18.4
+Version: 3.19.0
 Summary: GUI for Setting Nexus Sardana Recorder
 Home-page: https://github.com/nexdatas/nxselector
 Author: Jan Kotanski
 Author-email: jankotan@gmail.com
 Maintainer: Jan Kotanski
 Maintainer-email: jankotan@gmail.com
 License: GNU GENERAL PUBLIC LICENSE, version 3
```

### Comparing `nxselector-3.18.4/README.rst` & `nxselector-3.19.0/README.rst`

 * *Files identical despite different names*

### Comparing `nxselector-3.18.4/man/nxselector.1` & `nxselector-3.19.0/man/nxselector.1`

 * *Files identical despite different names*

### Comparing `nxselector-3.18.4/nxselector` & `nxselector-3.19.0/nxselector`

 * *Files identical despite different names*

### Comparing `nxselector-3.18.4/nxselector.egg-info/PKG-INFO` & `nxselector-3.19.0/nxselector.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: nxselector
-Version: 3.18.4
+Version: 3.19.0
 Summary: GUI for Setting Nexus Sardana Recorder
 Home-page: https://github.com/nexdatas/nxselector
 Author: Jan Kotanski
 Author-email: jankotan@gmail.com
 Maintainer: Jan Kotanski
 Maintainer-email: jankotan@gmail.com
 License: GNU GENERAL PUBLIC LICENSE, version 3
```

### Comparing `nxselector-3.18.4/nxselector.egg-info/SOURCES.txt` & `nxselector-3.19.0/nxselector.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 setup.cfg
 setup.py
 man/nxselector.1
 nxselector.egg-info/PKG-INFO
 nxselector.egg-info/SOURCES.txt
 nxselector.egg-info/dependency_links.txt
 nxselector.egg-info/not-zip-safe
-nxselector.egg-info/requires.txt
 nxselector.egg-info/top_level.txt
 nxsselector/AddDataSourceDlg.py
 nxsselector/CommandThread.py
 nxsselector/Data.py
 nxsselector/Descriptions.py
 nxsselector/Detectors.py
 nxsselector/DynamicTools.py
```

### Comparing `nxselector-3.18.4/nxsselector/AddDataSourceDlg.py` & `nxselector-3.19.0/nxsselector/AddDataSourceDlg.py`

 * *Files identical despite different names*

### Comparing `nxselector-3.18.4/nxsselector/CommandThread.py` & `nxselector-3.19.0/nxsselector/CommandThread.py`

 * *Files identical despite different names*

### Comparing `nxselector-3.18.4/nxsselector/Data.py` & `nxselector-3.19.0/nxsselector/Data.py`

 * *Files identical despite different names*

### Comparing `nxselector-3.18.4/nxsselector/Descriptions.py` & `nxselector-3.19.0/nxsselector/Descriptions.py`

 * *Files identical despite different names*

### Comparing `nxselector-3.18.4/nxsselector/Detectors.py` & `nxselector-3.19.0/nxsselector/Detectors.py`

 * *Files identical despite different names*

### Comparing `nxselector-3.18.4/nxsselector/DynamicTools.py` & `nxselector-3.19.0/nxsselector/DynamicTools.py`

 * *Files identical despite different names*

### Comparing `nxselector-3.18.4/nxsselector/EdDataDlg.py` & `nxselector-3.19.0/nxsselector/EdDataDlg.py`

 * *Files identical despite different names*

### Comparing `nxselector-3.18.4/nxsselector/EdListDlg.py` & `nxselector-3.19.0/nxsselector/EdListDlg.py`

 * *Files identical despite different names*

### Comparing `nxselector-3.18.4/nxsselector/Element.py` & `nxselector-3.19.0/nxsselector/Element.py`

 * *Files identical despite different names*

### Comparing `nxselector-3.18.4/nxsselector/ElementModel.py` & `nxselector-3.19.0/nxsselector/ElementModel.py`

 * *Files identical despite different names*

### Comparing `nxselector-3.18.4/nxsselector/Frames.py` & `nxselector-3.19.0/nxsselector/Frames.py`

 * *Files identical despite different names*

### Comparing `nxselector-3.18.4/nxsselector/GroupsDlg.py` & `nxselector-3.19.0/nxsselector/GroupsDlg.py`

 * *Files identical despite different names*

### Comparing `nxselector-3.18.4/nxsselector/InfoDlg.py` & `nxselector-3.19.0/nxsselector/InfoDlg.py`

 * *Files identical despite different names*

### Comparing `nxselector-3.18.4/nxsselector/LDataDlg.py` & `nxselector-3.19.0/nxsselector/LDataDlg.py`

 * *Files identical despite different names*

### Comparing `nxselector-3.18.4/nxsselector/MessageBox.py` & `nxselector-3.19.0/nxsselector/MessageBox.py`

 * *Files identical despite different names*

### Comparing `nxselector-3.18.4/nxsselector/OrderDlg.py` & `nxselector-3.19.0/nxsselector/OrderDlg.py`

 * *Files identical despite different names*

### Comparing `nxselector-3.18.4/nxsselector/Preferences.py` & `nxselector-3.19.0/nxsselector/Preferences.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,17 @@
                     CheckerViewNL, RadioViewNL, ButtonViewNL,
                     LeftCheckerViewNL, LeftRadioViewNL,
                     CheckerViewNN, RadioViewNN, ButtonViewNN,
                     LeftCheckerViewNN, LeftRadioViewNN,
                     CheckDisView, RadioDisView,
                     CheckDisViewNL, RadioDisViewNL,
                     CheckDisViewNN, RadioDisViewNN,
+                    CheckDisSelView,
+                    CheckDisSelViewNL,
+                    CheckDisSelViewNN,
                     CheckPropView,
                     CheckPropViewNL,
                     CheckPropViewNN,
                     CheckExPropView,
                     CheckExPropViewNL,
                     CheckExPropViewNN,
                     )
@@ -139,14 +142,17 @@
             "RadioButtons (N)": LeftRadioViewNL,
             "Buttons (N)": ButtonViewNL,
             "CentralCheckBoxes": CheckerViewNN,
             "CheckBoxes": LeftCheckerViewNN,
             "CentralRadioButtons": RadioViewNN,
             "RadioButtons": LeftRadioViewNN,
             "Buttons": ButtonViewNN,
+            "CheckBoxes Dis Sel": CheckDisSelView,
+            "CheckBoxes Dis Sel (A)": CheckDisSelViewNN,
+            "CheckBoxes Dis Sel (N)": CheckDisSelViewNL,
             "CheckBoxes Dis (A)": CheckDisView,
             "CheckBoxes Prop (A)": CheckPropView,
             "CheckBoxes Synch (A)": CheckExPropView,
             "RadioButtons Dis (A)": RadioDisView,
             "CheckBoxes Dis (N)": CheckDisViewNL,
             "CheckBoxes Prop (N)": CheckPropViewNL,
             "CheckBoxes Synch (N)": CheckExPropViewNL,
```

### Comparing `nxselector-3.18.4/nxsselector/PropertiesDlg.py` & `nxselector-3.19.0/nxsselector/PropertiesDlg.py`

 * *Files identical despite different names*

### Comparing `nxselector-3.18.4/nxsselector/Selector.py` & `nxselector-3.19.0/nxsselector/Selector.py`

 * *Files 2% similar despite different names*

```diff
@@ -240,14 +240,22 @@
         try:
             self.scanFileExtStatus = int(
                 settings.value('Preferences/ScanFileExtStatus', 2))
         except Exception:
             self.scanFileExtStatus = int(
                 settings.value(
                     'Preferences/ScanFileExtStatus', 2).toInt()[0])
+        try:
+            scanIDEditable = int(
+                settings.value('Preferences/ScanIDEditable', 0))
+        except Exception:
+            scanIDEditable = int(
+                settings.value(
+                    'Preferences/ScanIDEditable', 0).toInt()[0])
+        self.state.scanIDEditable = bool(scanIDEditable)
         cnffile = settings.value("Selector/CnfFile", "./")
         if hasattr(cnffile, "toString"):
             self.cnfFile = str(cnffile.toString())
         else:
             self.cnfFile = str(cnffile)
         self.__addButtonBoxes()
 
@@ -375,14 +383,22 @@
             self.__scanFileExtStatusChanged(int(
                 settings.value('Preferences/ScanFileExtStatus', 2)))
         except Exception:
             self.__scanFileExtStatusChanged(int(
                 settings.value('Preferences/ScanFileExtStatus', 2).toInt()[0]))
         self.ui.fileExtScanCheckBox.setChecked(
             self.scanFileExtStatus != 0)
+        try:
+            self.__scanIDEditableChanged(int(
+                settings.value('Preferences/ScanIDEditable', 0)))
+        except Exception:
+            self.__scanIDEditableChanged(int(
+                settings.value('Preferences/ScanIDEditable', 0).toInt()[0]))
+        self.ui.scanIDEditableCheckBox.setChecked(
+            self.state.scanIDEditable != 0)
 
         self.__settingsloaded = True
         self.__skipconfig = False
         logger.debug("settings END")
 
     def createGUI(self):
         """ creates GUI for the main window
@@ -486,14 +502,16 @@
         cid = self.ui.viewComboBox.findText(str(self.userView))
         if cid >= 0:
             self.ui.viewComboBox.setCurrentIndex(cid)
         self.ui.rowMaxSpinBox.setValue(self.rowMax)
         self.ui.fontSizeSpinBox.setValue(self.fontSize)
         self.ui.statusCheckBox.setChecked(self.displayStatus != 0)
         self.ui.fileExtScanCheckBox.setChecked(self.scanFileExtStatus != 0)
+        self.ui.scanIDEditableCheckBox.setChecked(
+            self.state.scanIDEditable != 0)
 
     def __hideWidgets(self):
         """ hides widgets according to set user mode
         """
         if not self.expert:
             self.ui.groupGroupBox.hide()
             self.ui.frameGroupBox.hide()
@@ -547,14 +565,16 @@
         self.ui.viewComboBox.currentIndexChanged.connect(self.resetViews)
         self.ui.rowMaxSpinBox.editingFinished.connect(self.resetRows)
         self.ui.fontSizeSpinBox.editingFinished.connect(self.resetRows)
         self.ui.statusCheckBox.stateChanged.connect(
             self.__displayStatusChanged)
         self.ui.fileExtScanCheckBox.stateChanged.connect(
             self.__scanFileExtStatusChanged)
+        self.ui.scanIDEditableCheckBox.stateChanged.connect(
+            self.__scanIDEditableChanged)
 
         self.detectors.dirty.connect(self.setDirty)
         self.preferences.dirty.connect(self.setDirty)
         self.descriptions.componentChecked.connect(self.__componentChanged)
         self.data.dirty.connect(self.setDirty)
         self.storage.dirty.connect(self.setDirty)
         self.storage.resetViews.connect(self.resetViews)
@@ -639,14 +659,17 @@
         settings.setValue(
             "Preferences/DisplayStatus",
             (2 if self.ui.statusCheckBox.isChecked() else 0))
         settings.setValue(
             "Preferences/ScanFileExtStatus",
             (2 if self.ui.fileExtScanCheckBox.isChecked() else 0))
         settings.setValue(
+            "Preferences/ScanIDEditable",
+            (2 if self.ui.scanIDEditableCheckBox.isChecked() else 0))
+        settings.setValue(
             "Preferences/Groups",
             (str(self.preferences.mgroups)))
         settings.setValue(
             "Preferences/Frames",
             (str(self.preferences.frames)))
         settings.setValue(
             "Preferences/FramesHints",
@@ -1302,14 +1325,25 @@
             self.ui.fileExtScanLineEdit.hide()
             self.ui.fileExtScanLabel.hide()
             self.state.scanFile = self.storage.fileNames(False, True)
             # self.storage.apply()
             self.storage.updateForm(False)
         self.setDirty(self.__dirty)
 
+    @Qt.pyqtSlot(int)
+    def __scanIDEditableChanged(self, state):
+        """  scanID editable status
+
+        :param state:  status state
+        :type index: :obj:`int`
+        """
+        self.state.scanIDEditable = state
+        self.storage.updateForm(self.scanFileExtStatus != 0)
+        self.setDirty(self.__dirty)
+
     def closeApply(self):
         """ close action for apply command """
         self.storage.showErrors()
         if not self.closeReset():
             self.setDirty(True)
         else:
             self.setDirty(False)
```

### Comparing `nxselector-3.18.4/nxsselector/ServerState.py` & `nxselector-3.19.0/nxsselector/ServerState.py`

 * *Files 0% similar despite different names*

```diff
@@ -226,14 +226,16 @@
 
         #: (:obj:`str`) scan directory
         self.scanDir = None
         #: (:obj:`list`<:obj:`str`>) scan file names
         self.scanFile = []
         #: (:obj:`int`) scan id
         self.scanID = 0
+        #: (:obj:`int`) editable scanid
+        self.scanIDEditable = 2
 
         #: (:obj:`list`<:obj:`str`>) timers
         self.timers = []
         #: (:obj:`str`) measurement group name
         self.mntgrp = None
         #: (:obj:`str`) door  device name
         self.door = None
@@ -604,14 +606,18 @@
         """
         params = {"ScanDir": "scanDir",
                   "ScanFile": "scanFile",
                   "NeXusSelectorDevice": "server",
                   # "ScanID": "scanID"
                   }
 
+        if self.scanIDEditable:
+            params["ScanID"] = "scanID"
+        elif "ScanID" in params:
+            params.pop("ScanID")
         if not self.__dp:
             self.setServer()
 
         value = {}
         for var, attr in params.items():
             value[var] = getattr(self, attr)
         jvalue = json.dumps(value)
```

### Comparing `nxselector-3.18.4/nxsselector/Storage.py` & `nxselector-3.19.0/nxsselector/Storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,15 +104,16 @@
                 self.__fileChanged)
             self.ui.fileScanDirLineEdit.textEdited.disconnect(
                 self.__dirty)
             self.ui.fileScanLineEdit.textEdited.disconnect(
                 self.__dirty)
             self.ui.fileExtScanLineEdit.textEdited.disconnect(
                 self.__dirty)
-            # measurement group
+            self.ui.fileScanIDSpinBox.valueChanged.disconnect(
+                self.__scanIDChanged)
 
             self.ui.mntTimerComboBox.currentIndexChanged.disconnect(self.apply)
             for cb in self.__tWidgets:
                 cb.currentIndexChanged.disconnect(self.apply)
 
             if hasattr(self.ui, "timerDelPushButton"):
                 self.ui.timerDelPushButton.clicked.disconnect(self.__delTimer)
@@ -155,14 +156,15 @@
         """
         logger.debug("connect signals")
         self.__connected = True
         self.ui.fileScanDirToolButton.pressed.connect(self.__setDir)
         self.ui.fileScanDirLineEdit.editingFinished.connect(self.__dirChanged)
         self.ui.fileScanLineEdit.editingFinished.connect(self.__fileChanged)
         self.ui.fileExtScanLineEdit.editingFinished.connect(self.__fileChanged)
+        self.ui.fileScanIDSpinBox.valueChanged.connect(self.__scanIDChanged)
         self.ui.fileScanDirLineEdit.textEdited.connect(self.__dirty)
         self.ui.fileScanLineEdit.textEdited.connect(self.__dirty)
         self.ui.fileExtScanLineEdit.textEdited.connect(self.__dirty)
         # measurement group
 
         self.ui.mntTimerComboBox.currentIndexChanged.connect(self.apply)
         for cb in self.__tWidgets:
@@ -625,15 +627,16 @@
             self.__updating = True
             # file group
             if status is None:
                 status = self.ui.fileExtScanCheckBox.isChecked()
             if self.state.scanDir is not None:
                 self.ui.fileScanDirLineEdit.setText(self.state.scanDir)
             self.ui.fileScanIDSpinBox.setValue(self.state.scanID)
-            self.ui.fileScanIDSpinBox.setEnabled(False)
+            self.ui.fileScanIDSpinBox.setEnabled(
+                self.state.scanIDEditable != 0)
 
             sfile = ""
             if self.state.scanFile:
                 scanFile = self.state.scanFile
                 sfile, sext = self._splitext(scanFile, status)
                 self.ui.fileScanLineEdit.setText(sfile)
                 if status:
@@ -800,14 +803,23 @@
         fnames = self.fileNames(False)
         sfile, _ = self._splitext(
             fnames, self.ui.fileExtScanCheckBox.isChecked())
         if json.dumps(self.state.scanFile) != json.dumps(fnames) or \
            str(self.ui.fileScanLineEdit.text()) != sfile:
             self.apply()
 
+    @Qt.pyqtSlot()
+    def __scanIDChanged(self):
+        """ updates application state on a scan id change
+        """
+        if self.state.scanIDEditable:
+            scanid = self.ui.fileScanIDSpinBox.value()
+            if self.state.scanID != scanid:
+                self.apply()
+
     def fileNames(self, message=True, status=None):
         """ corrects the scan file name lists
 
         :param message: message on false
         :type message: :obj:`str`
         :param status: scan file extension status
         :type status: :obj:`bool` or :obj:`int`
@@ -888,15 +900,16 @@
             self.state.door = str(self.ui.mntServerLineEdit.text())
 
             # device group
             self.state.writerDevice = str(self.ui.devWriterLineEdit.text())
             self.state.configDevice = str(self.ui.devConfigLineEdit.text())
 
             self.state.scanDir = str(self.ui.fileScanDirLineEdit.text())
-    #        self.state.scanID = int(self.ui.fileScanIDSpinBox.value())
+            if self.state.scanIDEditable:
+                self.state.scanID = int(self.ui.fileScanIDSpinBox.value())
             self.state.scanFile = self.fileNames()
             # dynamic component group
             self.state.dynamicComponents = True
             self.state.dynamicLinks = self.ui.dcLinksCheckBox.isChecked()
             self.state.dynamicPath = str(self.ui.dcPathLineEdit.text())
 
             # others group
```

### Comparing `nxselector-3.18.4/nxsselector/Views.py` & `nxselector-3.19.0/nxsselector/Views.py`

 * *Files 2% similar despite different names*

```diff
@@ -245,14 +245,16 @@
         #: (:obj:`int`) selected widget row (widget id)
         self.selectedWidgetRow = None
         #: (:obj:`bool`) if name labels should be shown
         self.showLabels = True
         #: (:obj:`bool`) if names should be shown
         self.showNames = True
         self.setContextMenuPolicy(Qt.Qt.PreventContextMenu)
+        #: (:obj:`bool`) switch checkboxes flag
+        self.switchCheckboxes = False
 
     def close(self):
         """ widget close method which disconnect signals """
 
         self.mapper.mapped.disconnect(self.checked)
         if self.model:
             self.model.dataChanged.disconnect(self.reset)
@@ -452,23 +454,35 @@
             else:
                 lrow = row
                 lcol = 0
             if self.dmapper:
                 lrow = lrow + 1
                 lcol = 2 * lcol
 
-                if lrow == 1:
-                    self.glayout.addWidget(
-                        Qt.QLabel(self.slabel), 0, lcol, 1, 1)
-                    self.glayout.addWidget(
-                        Qt.QLabel(self.dlabel), 0, lcol + 1, 1, 1,
-                        Qt.Qt.AlignCenter)
-                self.glayout.addWidget(ds, lrow, lcol + 1, 1, 1,
-                                       Qt.Qt.AlignCenter)
-            self.glayout.addWidget(cb, lrow, lcol, 1, 1)
+                if not self.switchCheckboxes:
+                    if lrow == 1:
+                        self.glayout.addWidget(
+                            Qt.QLabel(self.slabel), 0, lcol, 1, 1)
+                        self.glayout.addWidget(
+                            Qt.QLabel(self.dlabel), 0, lcol + 1, 1, 1,
+                            Qt.Qt.AlignCenter)
+                    self.glayout.addWidget(ds, lrow, lcol + 1, 1, 1,
+                                           Qt.Qt.AlignCenter)
+                else:
+                    if lrow == 1:
+                        self.glayout.addWidget(
+                            Qt.QLabel(self.slabel), 0, lcol + 1, 1, 1)
+                        self.glayout.addWidget(
+                            Qt.QLabel(self.dlabel), 0, lcol, 1, 1)
+                    self.glayout.addWidget(ds, lrow, lcol, 1, 1,
+                                           Qt.Qt.AlignCenter)
+            if not self.switchCheckboxes:
+                self.glayout.addWidget(cb, lrow, lcol, 1, 1)
+            else:
+                self.glayout.addWidget(cb, lrow, lcol + 1, 1, 1)
             self.widgets.append(cb)
 
             if hasattr(cb, "clicked"):
                 cb.clicked.connect(self.mapper.map)
             self.mapper.setMapping(cb, self.widgets.index(cb))
             if self.dmapper:
                 self.displays.append(ds)
@@ -705,14 +719,24 @@
 
     def __init__(self, parent=None):
         CheckPropView.__init__(self, parent)
         #: (:obj:`bool`) if widget are centered
         self.propdlg = LExDataDlg
 
 
+class CheckDisSelView(CheckPropView):
+    """ element view with switched checkboxes
+    """
+
+    def __init__(self, parent=None):
+        CheckPropView.__init__(self, parent)
+        #: (:obj:`bool`) if widget are centered
+        self.switchCheckboxes = True
+
+
 class RadioView(CheckerView):
     """ element view with radio checkboxes
     """
 
     def __init__(self, parent=None):
         """ constructor
 
@@ -994,14 +1018,30 @@
         :type parent: :class:`taurus.qt.Qt.QObject`
         """
         CheckExPropView.__init__(self, parent)
         #: (:obj:`bool`) if name labels should be shown
         self.showLabels = False
 
 
+class CheckDisSelViewNL(CheckDisSelView):
+    """ element view with checkboxes and properties
+    without name labels
+    """
+
+    def __init__(self, parent=None):
+        """ constructor
+
+        :param parent: parent object
+        :type parent: :class:`taurus.qt.Qt.QObject`
+        """
+        CheckDisSelView.__init__(self, parent)
+        #: (:obj:`bool`) if name labels should be shown
+        self.showLabels = False
+
+
 class ButtonDisViewNL(ButtonDisView):
     """ element view with left button checkboxes and display boxes
     without name labels
     """
 
     def __init__(self, parent=None):
         """ constructor
@@ -1057,14 +1097,30 @@
         :type parent: :class:`taurus.qt.Qt.QObject`
         """
         CheckPropView.__init__(self, parent)
         #: (:obj:`bool`) if names should be shown
         self.showNames = False
 
 
+class CheckDisSelViewNN(CheckDisSelView):
+    """ element view with redefined checkboxes with properties
+    without names
+    """
+
+    def __init__(self, parent=None):
+        """ constructor
+
+        :param parent: parent object
+        :type parent: :class:`taurus.qt.Qt.QObject`
+        """
+        CheckDisSelView.__init__(self, parent)
+        #: (:obj:`bool`) if names should be shown
+        self.showNames = False
+
+
 class CheckExPropViewNN(CheckExPropView):
     """ element view with redefined checkboxes with properties
     without names
     """
 
     def __init__(self, parent=None):
         """ constructor
```

### Comparing `nxselector-3.18.4/nxsselector/__init__.py` & `nxselector-3.19.0/nxsselector/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,8 +18,8 @@
 # package constructor
 
 """ --- NXS Selector --
 GUI for setting Sardana NeXus Recorder
 """
 
 #: (:obj:`str`) version of the application
-__version__ = "3.18.4"
+__version__ = "3.19.0"
```

### Comparing `nxselector-3.18.4/nxsselector/images/network_folder.png` & `nxselector-3.19.0/nxsselector/images/network_folder.png`

 * *Files identical despite different names*

### Comparing `nxselector-3.18.4/nxsselector/qrc/__init__.py` & `nxselector-3.19.0/nxsselector/qrc/__init__.py`

 * *Files identical despite different names*

### Comparing `nxselector-3.18.4/nxsselector/qtapi.py` & `nxselector-3.19.0/nxsselector/qtapi.py`

 * *Files identical despite different names*

### Comparing `nxselector-3.18.4/nxsselector/ui/AddDataSourceDlg.ui` & `nxselector-3.19.0/nxsselector/ui/AddDataSourceDlg.ui`

 * *Files identical despite different names*

### Comparing `nxselector-3.18.4/nxsselector/ui/EdDataDlg.ui` & `nxselector-3.19.0/nxsselector/ui/EdDataDlg.ui`

 * *Files identical despite different names*

### Comparing `nxselector-3.18.4/nxsselector/ui/EdListWg.ui` & `nxselector-3.19.0/nxsselector/ui/EdListWg.ui`

 * *Files identical despite different names*

### Comparing `nxselector-3.18.4/nxsselector/ui/GroupsDlg.ui` & `nxselector-3.19.0/nxsselector/ui/GroupsDlg.ui`

 * *Files identical despite different names*

### Comparing `nxselector-3.18.4/nxsselector/ui/InfoDlg.ui` & `nxselector-3.19.0/nxsselector/ui/InfoDlg.ui`

 * *Files identical despite different names*

### Comparing `nxselector-3.18.4/nxsselector/ui/LDataDlg.ui` & `nxselector-3.19.0/nxsselector/ui/LDataDlg.ui`

 * *Files identical despite different names*

### Comparing `nxselector-3.18.4/nxsselector/ui/OrderDlg.ui` & `nxselector-3.19.0/nxsselector/ui/OrderDlg.ui`

 * *Files identical despite different names*

### Comparing `nxselector-3.18.4/nxsselector/ui/Selector.ui` & `nxselector-3.19.0/nxsselector/ui/Selector.ui`

 * *Files 0% similar despite different names*

#### Comparing `nxselector-3.18.4/nxsselector/ui/Selector.ui` & `nxselector-3.19.0/nxsselector/ui/Selector.ui`

```diff
@@ -2,16 +2,16 @@
 <ui version="4.0">
   <class>Selector</class>
   <widget class="QDialog" name="Selector">
     <property name="geometry">
       <rect>
         <x>0</x>
         <y>0</y>
-        <width>1015</width>
-        <height>583</height>
+        <width>1031</width>
+        <height>762</height>
       </rect>
     </property>
     <property name="windowTitle">
       <string>NeXus Component Selector</string>
     </property>
     <layout class="QGridLayout" name="gridLayout">
       <item row="1" column="0">
@@ -439,16 +439,16 @@
                         <bool>true</bool>
                       </property>
                       <widget class="QWidget" name="detectorsWidget">
                         <property name="geometry">
                           <rect>
                             <x>0</x>
                             <y>0</y>
-                            <width>991</width>
-                            <height>411</height>
+                            <width>1007</width>
+                            <height>593</height>
                           </rect>
                         </property>
                       </widget>
                     </widget>
                   </item>
                 </layout>
               </widget>
@@ -486,16 +486,16 @@
                         <bool>true</bool>
                       </property>
                       <widget class="QWidget" name="descriptionsWidget">
                         <property name="geometry">
                           <rect>
                             <x>0</x>
                             <y>0</y>
-                            <width>991</width>
-                            <height>411</height>
+                            <width>1007</width>
+                            <height>593</height>
                           </rect>
                         </property>
                       </widget>
                     </widget>
                   </item>
                 </layout>
               </widget>
@@ -534,186 +534,236 @@
                                 <property name="toolTip">
                                   <string>View parameters</string>
                                 </property>
                                 <property name="title">
                                   <string>View:</string>
                                 </property>
                                 <layout class="QGridLayout" name="gridLayout_3">
-                                  <item row="1" column="0">
-                                    <layout class="QHBoxLayout" name="horizontalLayout">
-                                      <item>
-                                        <widget class="QCheckBox" name="statusCheckBox">
-                                          <property name="toolTip">
-                                            <string>Show the apply status in the bottom row</string>
-                                          </property>
-                                          <property name="text">
-                                            <string>Status</string>
-                                          </property>
-                                        </widget>
-                                      </item>
-                                      <item>
-                                        <spacer name="horizontalSpacer">
-                                          <property name="orientation">
-                                            <enum>Qt::Horizontal</enum>
-                                          </property>
-                                          <property name="sizeType">
-                                            <enum>QSizePolicy::Minimum</enum>
-                                          </property>
-                                          <property name="sizeHint" stdset="0">
-                                            <size>
-                                              <width>10</width>
-                                              <height>20</height>
-                                            </size>
-                                          </property>
-                                        </spacer>
-                                      </item>
-                                      <item>
-                                        <widget class="QLabel" name="rowMaxLabel">
-                                          <property name="toolTip">
-                                            <string>Maximal number of component rows in the Detectors and Descriptions tabs.</string>
-                                          </property>
-                                          <property name="text">
-                                            <string>Row Max.:</string>
-                                          </property>
-                                          <property name="buddy">
-                                            <cstring>rowMaxSpinBox</cstring>
-                                          </property>
-                                        </widget>
-                                      </item>
-                                      <item>
-                                        <widget class="QSpinBox" name="rowMaxSpinBox"/>
-                                      </item>
+                                  <item row="0" column="0">
+                                    <layout class="QVBoxLayout" name="verticalLayout_3">
                                       <item>
-                                        <spacer name="horizontalSpacer_6">
+                                        <spacer name="verticalSpacer_11">
                                           <property name="orientation">
-                                            <enum>Qt::Horizontal</enum>
+                                            <enum>Qt::Vertical</enum>
                                           </property>
                                           <property name="sizeType">
-                                            <enum>QSizePolicy::Preferred</enum>
+                                            <enum>QSizePolicy::Maximum</enum>
                                           </property>
                                           <property name="sizeHint" stdset="0">
                                             <size>
-                                              <width>40</width>
+                                              <width>20</width>
                                               <height>20</height>
                                             </size>
                                           </property>
                                         </spacer>
                                       </item>
                                       <item>
-                                        <widget class="QLabel" name="fontSizeLabel">
-                                          <property name="text">
-                                            <string>Font Size:</string>
-                                          </property>
-                                          <property name="buddy">
-                                            <cstring>fontSizeSpinBox</cstring>
-                                          </property>
-                                        </widget>
-                                      </item>
-                                      <item>
-                                        <widget class="QSpinBox" name="fontSizeSpinBox"/>
+                                        <layout class="QHBoxLayout" name="horizontalLayout">
+                                          <item>
+                                            <widget class="QCheckBox" name="statusCheckBox">
+                                              <property name="toolTip">
+                                                <string>Show the apply status in the bottom row</string>
+                                              </property>
+                                              <property name="text">
+                                                <string>Status</string>
+                                              </property>
+                                            </widget>
+                                          </item>
+                                          <item>
+                                            <spacer name="horizontalSpacer">
+                                              <property name="orientation">
+                                                <enum>Qt::Horizontal</enum>
+                                              </property>
+                                              <property name="sizeType">
+                                                <enum>QSizePolicy::Minimum</enum>
+                                              </property>
+                                              <property name="sizeHint" stdset="0">
+                                                <size>
+                                                  <width>10</width>
+                                                  <height>20</height>
+                                                </size>
+                                              </property>
+                                            </spacer>
+                                          </item>
+                                          <item>
+                                            <widget class="QLabel" name="rowMaxLabel">
+                                              <property name="toolTip">
+                                                <string>Maximal number of component rows in the Detectors and Descriptions tabs.</string>
+                                              </property>
+                                              <property name="text">
+                                                <string>Row Max.:</string>
+                                              </property>
+                                              <property name="buddy">
+                                                <cstring>rowMaxSpinBox</cstring>
+                                              </property>
+                                            </widget>
+                                          </item>
+                                          <item>
+                                            <widget class="QSpinBox" name="rowMaxSpinBox"/>
+                                          </item>
+                                          <item>
+                                            <spacer name="horizontalSpacer_6">
+                                              <property name="orientation">
+                                                <enum>Qt::Horizontal</enum>
+                                              </property>
+                                              <property name="sizeType">
+                                                <enum>QSizePolicy::Preferred</enum>
+                                              </property>
+                                              <property name="sizeHint" stdset="0">
+                                                <size>
+                                                  <width>40</width>
+                                                  <height>20</height>
+                                                </size>
+                                              </property>
+                                            </spacer>
+                                          </item>
+                                          <item>
+                                            <widget class="QLabel" name="fontSizeLabel">
+                                              <property name="text">
+                                                <string>Font Size:</string>
+                                              </property>
+                                              <property name="buddy">
+                                                <cstring>fontSizeSpinBox</cstring>
+                                              </property>
+                                            </widget>
+                                          </item>
+                                          <item>
+                                            <widget class="QSpinBox" name="fontSizeSpinBox"/>
+                                          </item>
+                                          <item>
+                                            <spacer name="horizontalSpacer_8">
+                                              <property name="orientation">
+                                                <enum>Qt::Horizontal</enum>
+                                              </property>
+                                              <property name="sizeType">
+                                                <enum>QSizePolicy::Preferred</enum>
+                                              </property>
+                                              <property name="sizeHint" stdset="0">
+                                                <size>
+                                                  <width>40</width>
+                                                  <height>20</height>
+                                                </size>
+                                              </property>
+                                            </spacer>
+                                          </item>
+                                          <item>
+                                            <widget class="QCheckBox" name="fileExtScanCheckBox">
+                                              <property name="toolTip">
+                                                <string>&lt;html&gt;&lt;head/&gt;&lt;body&gt;&lt;p&gt;Define scan file extensions separately&lt;/p&gt;&lt;/body&gt;&lt;/html&gt;</string>
+                                              </property>
+                                              <property name="text">
+                                                <string>Scan File Ext. separated</string>
+                                              </property>
+                                            </widget>
+                                          </item>
+                                          <item>
+                                            <spacer name="horizontalSpacer_10">
+                                              <property name="orientation">
+                                                <enum>Qt::Horizontal</enum>
+                                              </property>
+                                              <property name="sizeType">
+                                                <enum>QSizePolicy::Preferred</enum>
+                                              </property>
+                                              <property name="sizeHint" stdset="0">
+                                                <size>
+                                                  <width>40</width>
+                                                  <height>20</height>
+                                                </size>
+                                              </property>
+                                            </spacer>
+                                          </item>
+                                          <item>
+                                            <widget class="QCheckBox" name="scanIDEditableCheckBox">
+                                              <property name="toolTip">
+                                                <string>&lt;html&gt;&lt;head/&gt;&lt;body&gt;&lt;p&gt;Make scanID editable&lt;/p&gt;&lt;/body&gt;&lt;/html&gt;</string>
+                                              </property>
+                                              <property name="text">
+                                                <string>ScanID editable</string>
+                                              </property>
+                                            </widget>
+                                          </item>
+                                          <item>
+                                            <spacer name="horizontalSpacer_11">
+                                              <property name="orientation">
+                                                <enum>Qt::Horizontal</enum>
+                                              </property>
+                                              <property name="sizeType">
+                                                <enum>QSizePolicy::Expanding</enum>
+                                              </property>
+                                              <property name="sizeHint" stdset="0">
+                                                <size>
+                                                  <width>40</width>
+                                                  <height>20</height>
+                                                </size>
+                                              </property>
+                                            </spacer>
+                                          </item>
+                                        </layout>
                                       </item>
                                       <item>
-                                        <spacer name="horizontalSpacer_8">
+                                        <spacer name="verticalSpacer_7">
                                           <property name="orientation">
-                                            <enum>Qt::Horizontal</enum>
+                                            <enum>Qt::Vertical</enum>
                                           </property>
                                           <property name="sizeType">
-                                            <enum>QSizePolicy::Preferred</enum>
+                                            <enum>QSizePolicy::Maximum</enum>
                                           </property>
                                           <property name="sizeHint" stdset="0">
                                             <size>
-                                              <width>40</width>
+                                              <width>20</width>
                                               <height>20</height>
                                             </size>
                                           </property>
                                         </spacer>
                                       </item>
                                       <item>
-                                        <widget class="QCheckBox" name="fileExtScanCheckBox">
-                                          <property name="toolTip">
-                                            <string>&lt;html&gt;&lt;head/&gt;&lt;body&gt;&lt;p&gt;Define scan file extensions separately&lt;/p&gt;&lt;/body&gt;&lt;/html&gt;</string>
-                                          </property>
-                                          <property name="text">
-                                            <string>Scan File Ext. separated</string>
-                                          </property>
-                                        </widget>
+                                        <layout class="QHBoxLayout" name="horizontalLayout_15">
+                                          <item>
+                                            <widget class="QLabel" name="specialCharactersLabel">
+                                              <property name="toolTip">
+                                                <string>&lt;html&gt;&lt;head/&gt;&lt;body&gt;&lt;p&gt;Character of scan file names to be replaced by '_', e.g. '/'&lt;/p&gt;&lt;/body&gt;&lt;/html&gt;</string>
+                                              </property>
+                                              <property name="text">
+                                                <string>Special Characters:</string>
+                                              </property>
+                                              <property name="buddy">
+                                                <cstring>specialCharactersLineEdit</cstring>
+                                              </property>
+                                            </widget>
+                                          </item>
+                                          <item>
+                                            <widget class="QLineEdit" name="specialCharactersLineEdit">
+                                              <property name="toolTip">
+                                                <string>&lt;html&gt;&lt;head/&gt;&lt;body&gt;&lt;p&gt;Character of scan file names to be replaced by '_', e.g. '/'&lt;/p&gt;&lt;/body&gt;&lt;/html&gt;</string>
+                                              </property>
+                                              <property name="text">
+                                                <string>/</string>
+                                              </property>
+                                            </widget>
+                                          </item>
+                                        </layout>
                                       </item>
                                       <item>
-                                        <spacer name="horizontalSpacer_10">
+                                        <spacer name="verticalSpacer_12">
                                           <property name="orientation">
-                                            <enum>Qt::Horizontal</enum>
+                                            <enum>Qt::Vertical</enum>
                                           </property>
                                           <property name="sizeType">
-                                            <enum>QSizePolicy::Preferred</enum>
+                                            <enum>QSizePolicy::Maximum</enum>
                                           </property>
                                           <property name="sizeHint" stdset="0">
                                             <size>
-                                              <width>40</width>
-                                              <height>20</height>
+                                              <width>20</width>
+                                              <height>40</height>
                                             </size>
                                           </property>
                                         </spacer>
                                       </item>
-                                      <item>
-                                        <widget class="QLabel" name="specialCharactersLabel">
-                                          <property name="toolTip">
-                                            <string>&lt;html&gt;&lt;head/&gt;&lt;body&gt;&lt;p&gt;Character of scan file names to be replaced by '_', e.g. '/'&lt;/p&gt;&lt;/body&gt;&lt;/html&gt;</string>
-                                          </property>
-                                          <property name="text">
-                                            <string>Special Characters:</string>
-                                          </property>
-                                          <property name="buddy">
-                                            <cstring>specialCharactersLineEdit</cstring>
-                                          </property>
-                                        </widget>
-                                      </item>
-                                      <item>
-                                        <widget class="QLineEdit" name="specialCharactersLineEdit">
-                                          <property name="toolTip">
-                                            <string>&lt;html&gt;&lt;head/&gt;&lt;body&gt;&lt;p&gt;Character of scan file names to be replaced by '_', e.g. '/'&lt;/p&gt;&lt;/body&gt;&lt;/html&gt;</string>
-                                          </property>
-                                          <property name="text">
-                                            <string>/</string>
-                                          </property>
-                                        </widget>
-                                      </item>
                                     </layout>
                                   </item>
-                                  <item row="2" column="0">
-                                    <spacer name="verticalSpacer_12">
-                                      <property name="orientation">
-                                        <enum>Qt::Vertical</enum>
-                                      </property>
-                                      <property name="sizeType">
-                                        <enum>QSizePolicy::Maximum</enum>
-                                      </property>
-                                      <property name="sizeHint" stdset="0">
-                                        <size>
-                                          <width>20</width>
-                                          <height>40</height>
-                                        </size>
-                                      </property>
-                                    </spacer>
-                                  </item>
-                                  <item row="0" column="0">
-                                    <spacer name="verticalSpacer_11">
-                                      <property name="orientation">
-                                        <enum>Qt::Vertical</enum>
-                                      </property>
-                                      <property name="sizeType">
-                                        <enum>QSizePolicy::Maximum</enum>
-                                      </property>
-                                      <property name="sizeHint" stdset="0">
-                                        <size>
-                                          <width>20</width>
-                                          <height>20</height>
-                                        </size>
-                                      </property>
-                                    </spacer>
-                                  </item>
                                 </layout>
                               </widget>
                             </item>
                           </layout>
                         </widget>
                       </item>
                       <item>
```

### Comparing `nxselector-3.18.4/nxsselector/ui/__init__.py` & `nxselector-3.19.0/nxsselector/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `nxselector-3.18.4/setup.py` & `nxselector-3.19.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 #: (:obj:`list` < :obj:`str` >) executable scripts
 SCRIPTS = ['nxselector']
 
 needs_pytest = set(['test']).intersection(sys.argv)
 pytest_runner = ['pytest-runner'] if needs_pytest else []
 
 install_requires = [
-    'taurus',
+    # 'taurus',
     # 'nxsrecselector',
     # 'pyqt5',
     # 'pytango',
     # 'sardana',
     # 'nxswriter',
     # 'nxstools',
     # 'nxsconfigserver',
```

### Comparing `nxselector-3.18.4/test/testmy.py` & `nxselector-3.19.0/test/testmy.py`

 * *Files identical despite different names*

