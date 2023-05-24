# Comparing `tmp/pynose-1.4.4.tar.gz` & `tmp/pynose-1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynose-1.4.4.tar", last modified: Wed May  3 01:50:57 2023, max compression
+gzip compressed data, was "pynose-1.4.5.tar", last modified: Wed May 24 22:17:19 2023, max compression
```

## Comparing `pynose-1.4.4.tar` & `pynose-1.4.5.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-03 01:50:57.931771 pynose-1.4.4/
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-03 01:50:57.924183 pynose-1.4.4/.github/
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-03 01:50:57.925764 pynose-1.4.4/.github/workflows/
--rw-r--r--   0 michael    (501) staff       (20)     1332 2023-03-01 21:40:49.000000 pynose-1.4.4/.github/workflows/python-package-legacy.yml
--rw-r--r--   0 michael    (501) staff       (20)     1357 2023-03-01 21:40:46.000000 pynose-1.4.4/.github/workflows/python-package.yml
--rw-r--r--   0 michael    (501) staff       (20)     1799 2023-02-28 01:46:25.000000 pynose-1.4.4/.gitignore
--rw-r--r--   0 michael    (501) staff       (20)     1070 2023-02-28 01:46:25.000000 pynose-1.4.4/LICENSE
--rw-r--r--   0 michael    (501) staff       (20)      135 2023-02-28 03:14:47.000000 pynose-1.4.4/MANIFEST.in
--rw-r--r--   0 michael    (501) staff       (20)    18375 2023-05-03 01:50:57.931832 pynose-1.4.4/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)    16918 2023-05-03 01:50:30.000000 pynose-1.4.4/README.md
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-03 01:50:57.926234 pynose-1.4.4/bin/
--rwxr-xr-x   0 michael    (501) staff       (20)       84 2012-09-29 08:18:54.000000 pynose-1.4.4/bin/nosetests
--rwxr-xr-x   0 michael    (501) staff       (20)       84 2012-09-29 08:18:54.000000 pynose-1.4.4/bin/pynose
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-03 01:50:57.928581 pynose-1.4.4/nose/
--rw-r--r--   0 michael    (501) staff       (20)      643 2023-03-02 04:16:39.000000 pynose-1.4.4/nose/__init__.py
--rw-r--r--   0 michael    (501) staff       (20)      144 2022-11-25 20:24:40.000000 pynose-1.4.4/nose/__main__.py
--rwxr-xr-x   0 michael    (501) staff       (20)       44 2023-05-03 01:50:30.000000 pynose-1.4.4/nose/__version__.py
--rw-r--r--   0 michael    (501) staff       (20)    11881 2023-05-02 02:01:52.000000 pynose-1.4.4/nose/case.py
--rw-r--r--   0 michael    (501) staff       (20)     5538 2023-03-02 14:29:59.000000 pynose-1.4.4/nose/commands.py
--rw-r--r--   0 michael    (501) staff       (20)    24529 2023-03-02 15:02:07.000000 pynose-1.4.4/nose/config.py
--rw-r--r--   0 michael    (501) staff       (20)    12087 2023-03-02 13:46:19.000000 pynose-1.4.4/nose/core.py
--rw-r--r--   0 michael    (501) staff       (20)      390 2023-02-26 21:55:15.000000 pynose-1.4.4/nose/exc.py
--rw-r--r--   0 michael    (501) staff       (20)     1258 2023-02-26 21:54:35.000000 pynose-1.4.4/nose/failure.py
--rw-r--r--   0 michael    (501) staff       (20)     9007 2023-05-02 02:01:52.000000 pynose-1.4.4/nose/importer.py
--rw-r--r--   0 michael    (501) staff       (20)     5535 2023-03-02 04:00:31.000000 pynose-1.4.4/nose/inspector.py
--rw-r--r--   0 michael    (501) staff       (20)    21758 2023-03-02 14:53:46.000000 pynose-1.4.4/nose/loader.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-03 01:50:57.930744 pynose-1.4.4/nose/plugins/
--rw-r--r--   0 michael    (501) staff       (20)     5421 2023-03-02 16:20:15.000000 pynose-1.4.4/nose/plugins/__init__.py
--rw-r--r--   0 michael    (501) staff       (20)     1007 2023-03-02 15:57:56.000000 pynose-1.4.4/nose/plugins/allmodules.py
--rw-r--r--   0 michael    (501) staff       (20)     8189 2023-03-02 16:10:06.000000 pynose-1.4.4/nose/plugins/attrib.py
--rw-r--r--   0 michael    (501) staff       (20)    23205 2023-04-30 16:29:19.000000 pynose-1.4.4/nose/plugins/base.py
--rw-r--r--   0 michael    (501) staff       (20)     1024 2023-02-26 20:00:18.000000 pynose-1.4.4/nose/plugins/builtin.py
--rw-r--r--   0 michael    (501) staff       (20)     3280 2023-05-03 01:50:30.000000 pynose-1.4.4/nose/plugins/capture.py
--rw-r--r--   0 michael    (501) staff       (20)     2739 2023-03-02 15:58:25.000000 pynose-1.4.4/nose/plugins/collect.py
--rw-r--r--   0 michael    (501) staff       (20)    10668 2023-03-02 16:16:16.000000 pynose-1.4.4/nose/plugins/cover.py
--rw-r--r--   0 michael    (501) staff       (20)     2163 2023-03-02 15:14:11.000000 pynose-1.4.4/nose/plugins/debug.py
--rw-r--r--   0 michael    (501) staff       (20)     1435 2023-03-02 15:57:16.000000 pynose-1.4.4/nose/plugins/deprecated.py
--rw-r--r--   0 michael    (501) staff       (20)    16001 2023-03-02 16:44:33.000000 pynose-1.4.4/nose/plugins/doctests.py
--rw-r--r--   0 michael    (501) staff       (20)     6390 2023-03-02 15:59:48.000000 pynose-1.4.4/nose/plugins/errorclass.py
--rw-r--r--   0 michael    (501) staff       (20)     1495 2023-03-02 15:59:22.000000 pynose-1.4.4/nose/plugins/failuredetail.py
--rw-r--r--   0 michael    (501) staff       (20)     3401 2023-02-28 06:09:15.000000 pynose-1.4.4/nose/plugins/isolate.py
--rw-r--r--   0 michael    (501) staff       (20)     8666 2023-03-02 15:25:15.000000 pynose-1.4.4/nose/plugins/logcapture.py
--rw-r--r--   0 michael    (501) staff       (20)    14221 2023-03-02 15:10:12.000000 pynose-1.4.4/nose/plugins/manager.py
--rw-r--r--   0 michael    (501) staff       (20)    31375 2023-03-02 19:07:14.000000 pynose-1.4.4/nose/plugins/multiprocess.py
--rw-r--r--   0 michael    (501) staff       (20)    13083 2023-03-02 15:51:36.000000 pynose-1.4.4/nose/plugins/plugintest.py
--rw-r--r--   0 michael    (501) staff       (20)     1487 2023-03-02 16:00:21.000000 pynose-1.4.4/nose/plugins/skip.py
--rw-r--r--   0 michael    (501) staff       (20)     9318 2023-03-02 16:04:30.000000 pynose-1.4.4/nose/plugins/testid.py
--rw-r--r--   0 michael    (501) staff       (20)    11044 2023-03-02 15:37:08.000000 pynose-1.4.4/nose/plugins/xunit.py
--rw-r--r--   0 michael    (501) staff       (20)     5964 2023-02-28 05:29:54.000000 pynose-1.4.4/nose/proxy.py
--rw-r--r--   0 michael    (501) staff       (20)     3665 2023-03-02 14:54:42.000000 pynose-1.4.4/nose/pyversion.py
--rw-r--r--   0 michael    (501) staff       (20)     5808 2023-05-02 02:01:52.000000 pynose-1.4.4/nose/result.py
--rw-r--r--   0 michael    (501) staff       (20)     9081 2023-03-02 14:46:58.000000 pynose-1.4.4/nose/selector.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-03 01:50:57.930939 pynose-1.4.4/nose/sphinx/
--rw-r--r--   0 michael    (501) staff       (20)        5 2022-11-25 20:24:40.000000 pynose-1.4.4/nose/sphinx/__init__.py
--rw-r--r--   0 michael    (501) staff       (20)     5348 2023-03-02 17:41:29.000000 pynose-1.4.4/nose/sphinx/pluginopts.py
--rw-r--r--   0 michael    (501) staff       (20)    18253 2023-03-02 15:00:20.000000 pynose-1.4.4/nose/suite.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-03 01:50:57.931256 pynose-1.4.4/nose/tools/
--rw-r--r--   0 michael    (501) staff       (20)      465 2023-02-26 23:14:39.000000 pynose-1.4.4/nose/tools/__init__.py
--rw-r--r--   0 michael    (501) staff       (20)     4080 2023-02-28 03:39:28.000000 pynose-1.4.4/nose/tools/nontrivial.py
--rw-r--r--   0 michael    (501) staff       (20)     1083 2023-02-28 03:40:01.000000 pynose-1.4.4/nose/tools/trivial.py
--rw-r--r--   0 michael    (501) staff       (20)     4981 2023-03-02 14:56:46.000000 pynose-1.4.4/nose/twistedtools.py
--rw-r--r--   0 michael    (501) staff       (20)     3698 2023-02-28 06:39:10.000000 pynose-1.4.4/nose/usage.txt
--rw-r--r--   0 michael    (501) staff       (20)    18791 2023-02-28 06:40:27.000000 pynose-1.4.4/nose/util.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-03 01:50:57.931678 pynose-1.4.4/pynose.egg-info/
--rw-r--r--   0 michael    (501) staff       (20)    18375 2023-05-03 01:50:57.000000 pynose-1.4.4/pynose.egg-info/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)     1240 2023-05-03 01:50:57.000000 pynose-1.4.4/pynose.egg-info/SOURCES.txt
--rw-r--r--   0 michael    (501) staff       (20)        1 2023-05-03 01:50:57.000000 pynose-1.4.4/pynose.egg-info/dependency_links.txt
--rw-r--r--   0 michael    (501) staff       (20)        5 2023-05-03 01:50:57.000000 pynose-1.4.4/pynose.egg-info/top_level.txt
--rw-r--r--   0 michael    (501) staff       (20)       86 2023-05-03 01:50:57.932062 pynose-1.4.4/setup.cfg
--rw-r--r--   0 michael    (501) staff       (20)     4567 2023-03-02 17:36:06.000000 pynose-1.4.4/setup.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-24 22:17:19.465227 pynose-1.4.5/
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-24 22:17:19.456223 pynose-1.4.5/.github/
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-24 22:17:19.457916 pynose-1.4.5/.github/workflows/
+-rw-r--r--   0 michael    (501) staff       (20)     1332 2023-03-01 21:40:49.000000 pynose-1.4.5/.github/workflows/python-package-legacy.yml
+-rw-r--r--   0 michael    (501) staff       (20)     1357 2023-03-01 21:40:46.000000 pynose-1.4.5/.github/workflows/python-package.yml
+-rw-r--r--   0 michael    (501) staff       (20)     1799 2023-02-28 01:46:25.000000 pynose-1.4.5/.gitignore
+-rw-r--r--   0 michael    (501) staff       (20)     1070 2023-02-28 01:46:25.000000 pynose-1.4.5/LICENSE
+-rw-r--r--   0 michael    (501) staff       (20)      135 2023-02-28 03:14:47.000000 pynose-1.4.5/MANIFEST.in
+-rw-r--r--   0 michael    (501) staff       (20)    18449 2023-05-24 22:17:19.465311 pynose-1.4.5/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)    16992 2023-05-24 22:14:10.000000 pynose-1.4.5/README.md
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-24 22:17:19.458377 pynose-1.4.5/bin/
+-rwxr-xr-x   0 michael    (501) staff       (20)       84 2012-09-29 08:18:54.000000 pynose-1.4.5/bin/nosetests
+-rwxr-xr-x   0 michael    (501) staff       (20)       84 2012-09-29 08:18:54.000000 pynose-1.4.5/bin/pynose
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-24 22:17:19.461132 pynose-1.4.5/nose/
+-rw-r--r--   0 michael    (501) staff       (20)      643 2023-03-02 04:16:39.000000 pynose-1.4.5/nose/__init__.py
+-rw-r--r--   0 michael    (501) staff       (20)      144 2022-11-25 20:24:40.000000 pynose-1.4.5/nose/__main__.py
+-rwxr-xr-x   0 michael    (501) staff       (20)       44 2023-05-24 22:14:10.000000 pynose-1.4.5/nose/__version__.py
+-rw-r--r--   0 michael    (501) staff       (20)    11881 2023-05-02 02:01:52.000000 pynose-1.4.5/nose/case.py
+-rw-r--r--   0 michael    (501) staff       (20)     5538 2023-03-02 14:29:59.000000 pynose-1.4.5/nose/commands.py
+-rw-r--r--   0 michael    (501) staff       (20)    24529 2023-03-02 15:02:07.000000 pynose-1.4.5/nose/config.py
+-rw-r--r--   0 michael    (501) staff       (20)    12087 2023-03-02 13:46:19.000000 pynose-1.4.5/nose/core.py
+-rw-r--r--   0 michael    (501) staff       (20)      390 2023-02-26 21:55:15.000000 pynose-1.4.5/nose/exc.py
+-rw-r--r--   0 michael    (501) staff       (20)     1258 2023-02-26 21:54:35.000000 pynose-1.4.5/nose/failure.py
+-rw-r--r--   0 michael    (501) staff       (20)     9007 2023-05-02 02:01:52.000000 pynose-1.4.5/nose/importer.py
+-rw-r--r--   0 michael    (501) staff       (20)     5535 2023-03-02 04:00:31.000000 pynose-1.4.5/nose/inspector.py
+-rw-r--r--   0 michael    (501) staff       (20)    21758 2023-03-02 14:53:46.000000 pynose-1.4.5/nose/loader.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-24 22:17:19.463871 pynose-1.4.5/nose/plugins/
+-rw-r--r--   0 michael    (501) staff       (20)     5421 2023-03-02 16:20:15.000000 pynose-1.4.5/nose/plugins/__init__.py
+-rw-r--r--   0 michael    (501) staff       (20)     1007 2023-03-02 15:57:56.000000 pynose-1.4.5/nose/plugins/allmodules.py
+-rw-r--r--   0 michael    (501) staff       (20)     8189 2023-03-02 16:10:06.000000 pynose-1.4.5/nose/plugins/attrib.py
+-rw-r--r--   0 michael    (501) staff       (20)    23205 2023-04-30 16:29:19.000000 pynose-1.4.5/nose/plugins/base.py
+-rw-r--r--   0 michael    (501) staff       (20)     1024 2023-02-26 20:00:18.000000 pynose-1.4.5/nose/plugins/builtin.py
+-rw-r--r--   0 michael    (501) staff       (20)     3280 2023-05-03 01:50:30.000000 pynose-1.4.5/nose/plugins/capture.py
+-rw-r--r--   0 michael    (501) staff       (20)     2739 2023-03-02 15:58:25.000000 pynose-1.4.5/nose/plugins/collect.py
+-rw-r--r--   0 michael    (501) staff       (20)    10668 2023-03-02 16:16:16.000000 pynose-1.4.5/nose/plugins/cover.py
+-rw-r--r--   0 michael    (501) staff       (20)     2163 2023-03-02 15:14:11.000000 pynose-1.4.5/nose/plugins/debug.py
+-rw-r--r--   0 michael    (501) staff       (20)     1435 2023-03-02 15:57:16.000000 pynose-1.4.5/nose/plugins/deprecated.py
+-rw-r--r--   0 michael    (501) staff       (20)    16001 2023-03-02 16:44:33.000000 pynose-1.4.5/nose/plugins/doctests.py
+-rw-r--r--   0 michael    (501) staff       (20)     6390 2023-03-02 15:59:48.000000 pynose-1.4.5/nose/plugins/errorclass.py
+-rw-r--r--   0 michael    (501) staff       (20)     1495 2023-03-02 15:59:22.000000 pynose-1.4.5/nose/plugins/failuredetail.py
+-rw-r--r--   0 michael    (501) staff       (20)     3401 2023-02-28 06:09:15.000000 pynose-1.4.5/nose/plugins/isolate.py
+-rw-r--r--   0 michael    (501) staff       (20)     8666 2023-03-02 15:25:15.000000 pynose-1.4.5/nose/plugins/logcapture.py
+-rw-r--r--   0 michael    (501) staff       (20)    14331 2023-05-24 22:14:10.000000 pynose-1.4.5/nose/plugins/manager.py
+-rw-r--r--   0 michael    (501) staff       (20)    31375 2023-03-02 19:07:14.000000 pynose-1.4.5/nose/plugins/multiprocess.py
+-rw-r--r--   0 michael    (501) staff       (20)    13083 2023-03-02 15:51:36.000000 pynose-1.4.5/nose/plugins/plugintest.py
+-rw-r--r--   0 michael    (501) staff       (20)     1487 2023-03-02 16:00:21.000000 pynose-1.4.5/nose/plugins/skip.py
+-rw-r--r--   0 michael    (501) staff       (20)     9318 2023-03-02 16:04:30.000000 pynose-1.4.5/nose/plugins/testid.py
+-rw-r--r--   0 michael    (501) staff       (20)    11044 2023-03-02 15:37:08.000000 pynose-1.4.5/nose/plugins/xunit.py
+-rw-r--r--   0 michael    (501) staff       (20)     5964 2023-02-28 05:29:54.000000 pynose-1.4.5/nose/proxy.py
+-rw-r--r--   0 michael    (501) staff       (20)     3665 2023-03-02 14:54:42.000000 pynose-1.4.5/nose/pyversion.py
+-rw-r--r--   0 michael    (501) staff       (20)     5808 2023-05-02 02:01:52.000000 pynose-1.4.5/nose/result.py
+-rw-r--r--   0 michael    (501) staff       (20)     9081 2023-03-02 14:46:58.000000 pynose-1.4.5/nose/selector.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-24 22:17:19.464105 pynose-1.4.5/nose/sphinx/
+-rw-r--r--   0 michael    (501) staff       (20)        5 2022-11-25 20:24:40.000000 pynose-1.4.5/nose/sphinx/__init__.py
+-rw-r--r--   0 michael    (501) staff       (20)     5348 2023-03-02 17:41:29.000000 pynose-1.4.5/nose/sphinx/pluginopts.py
+-rw-r--r--   0 michael    (501) staff       (20)    18253 2023-03-02 15:00:20.000000 pynose-1.4.5/nose/suite.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-24 22:17:19.464576 pynose-1.4.5/nose/tools/
+-rw-r--r--   0 michael    (501) staff       (20)      465 2023-02-26 23:14:39.000000 pynose-1.4.5/nose/tools/__init__.py
+-rw-r--r--   0 michael    (501) staff       (20)     4080 2023-02-28 03:39:28.000000 pynose-1.4.5/nose/tools/nontrivial.py
+-rw-r--r--   0 michael    (501) staff       (20)     1083 2023-02-28 03:40:01.000000 pynose-1.4.5/nose/tools/trivial.py
+-rw-r--r--   0 michael    (501) staff       (20)     4981 2023-03-02 14:56:46.000000 pynose-1.4.5/nose/twistedtools.py
+-rw-r--r--   0 michael    (501) staff       (20)     3698 2023-02-28 06:39:10.000000 pynose-1.4.5/nose/usage.txt
+-rw-r--r--   0 michael    (501) staff       (20)    18927 2023-05-24 22:14:10.000000 pynose-1.4.5/nose/util.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-24 22:17:19.465114 pynose-1.4.5/pynose.egg-info/
+-rw-r--r--   0 michael    (501) staff       (20)    18449 2023-05-24 22:17:19.000000 pynose-1.4.5/pynose.egg-info/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)     1240 2023-05-24 22:17:19.000000 pynose-1.4.5/pynose.egg-info/SOURCES.txt
+-rw-r--r--   0 michael    (501) staff       (20)        1 2023-05-24 22:17:19.000000 pynose-1.4.5/pynose.egg-info/dependency_links.txt
+-rw-r--r--   0 michael    (501) staff       (20)        5 2023-05-24 22:17:19.000000 pynose-1.4.5/pynose.egg-info/top_level.txt
+-rw-r--r--   0 michael    (501) staff       (20)       86 2023-05-24 22:17:19.465774 pynose-1.4.5/setup.cfg
+-rw-r--r--   0 michael    (501) staff       (20)     4567 2023-03-02 17:36:06.000000 pynose-1.4.5/setup.py
```

### Comparing `pynose-1.4.4/.github/workflows/python-package-legacy.yml` & `pynose-1.4.5/.github/workflows/python-package-legacy.yml`

 * *Files identical despite different names*

### Comparing `pynose-1.4.4/.github/workflows/python-package.yml` & `pynose-1.4.5/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `pynose-1.4.4/.gitignore` & `pynose-1.4.5/.gitignore`

 * *Files identical despite different names*

### Comparing `pynose-1.4.4/LICENSE` & `pynose-1.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pynose-1.4.4/PKG-INFO` & `pynose-1.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynose
-Version: 1.4.4
+Version: 1.4.5
 Summary: pynose fixes nose to extend unittest and make testing easier
 Home-page: https://github.com/mdmintz/pynose
 Author: Michael Mintz
 Author-email: mdmintz@gmail.com
 License: MIT
 Project-URL: Download, https://pypi.org/project/pynose/#files
 Project-URL: PyPI, https://pypi.org/project/pynose/
@@ -43,17 +43,18 @@
 
 ``pynose`` is an updated version of ``nose``, originally made by Jason Pellerin.
 
 This version of ``nose`` is compatible with Python 3.6+ (including 3.12 & up).
 
 Changes in ``pynose`` from legacy ``nose`` include:
 * Fixes "AttributeError: module 'collections' has no attribute 'Callable'."
-* Fixes all ``flake8`` issues from the original ``nose``.
+* Fixes "AttributeError: module 'inspect' has no attribute 'getargspec'."
 * Fixes "ImportError: cannot import name '_TextTestResult' from 'unittest'."
 * Fixes "RuntimeWarning: TestResult has no addDuration method."
+* Fixes all ``flake8`` issues from the original ``nose``.
 * Replaces the ``imp`` module with the newer ``importlib`` module.
 * The default logging level now hides "debug" logs for less noise.
 * The ``-s`` option is always active to see the output of ``print()``.
 * Adds ``--co`` as a shortcut to using ``--collect-only``.
 
 --------
```

### Comparing `pynose-1.4.4/README.md` & `pynose-1.4.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -8,17 +8,18 @@
 
 ``pynose`` is an updated version of ``nose``, originally made by Jason Pellerin.
 
 This version of ``nose`` is compatible with Python 3.6+ (including 3.12 & up).
 
 Changes in ``pynose`` from legacy ``nose`` include:
 * Fixes "AttributeError: module 'collections' has no attribute 'Callable'."
-* Fixes all ``flake8`` issues from the original ``nose``.
+* Fixes "AttributeError: module 'inspect' has no attribute 'getargspec'."
 * Fixes "ImportError: cannot import name '_TextTestResult' from 'unittest'."
 * Fixes "RuntimeWarning: TestResult has no addDuration method."
+* Fixes all ``flake8`` issues from the original ``nose``.
 * Replaces the ``imp`` module with the newer ``importlib`` module.
 * The default logging level now hides "debug" logs for less noise.
 * The ``-s`` option is always active to see the output of ``print()``.
 * Adds ``--co`` as a shortcut to using ``--collect-only``.
 
 --------
```

### Comparing `pynose-1.4.4/nose/__init__.py` & `pynose-1.4.5/nose/__init__.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.4/nose/case.py` & `pynose-1.4.5/nose/case.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.4/nose/commands.py` & `pynose-1.4.5/nose/commands.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.4/nose/config.py` & `pynose-1.4.5/nose/config.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.4/nose/core.py` & `pynose-1.4.5/nose/core.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.4/nose/failure.py` & `pynose-1.4.5/nose/failure.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.4/nose/importer.py` & `pynose-1.4.5/nose/importer.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.4/nose/inspector.py` & `pynose-1.4.5/nose/inspector.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.4/nose/loader.py` & `pynose-1.4.5/nose/loader.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.4/nose/plugins/__init__.py` & `pynose-1.4.5/nose/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.4/nose/plugins/allmodules.py` & `pynose-1.4.5/nose/plugins/allmodules.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.4/nose/plugins/attrib.py` & `pynose-1.4.5/nose/plugins/attrib.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.4/nose/plugins/base.py` & `pynose-1.4.5/nose/plugins/base.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.4/nose/plugins/builtin.py` & `pynose-1.4.5/nose/plugins/builtin.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.4/nose/plugins/capture.py` & `pynose-1.4.5/nose/plugins/capture.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.4/nose/plugins/collect.py` & `pynose-1.4.5/nose/plugins/collect.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.4/nose/plugins/cover.py` & `pynose-1.4.5/nose/plugins/cover.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.4/nose/plugins/debug.py` & `pynose-1.4.5/nose/plugins/debug.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.4/nose/plugins/deprecated.py` & `pynose-1.4.5/nose/plugins/deprecated.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.4/nose/plugins/doctests.py` & `pynose-1.4.5/nose/plugins/doctests.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.4/nose/plugins/errorclass.py` & `pynose-1.4.5/nose/plugins/errorclass.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.4/nose/plugins/failuredetail.py` & `pynose-1.4.5/nose/plugins/failuredetail.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.4/nose/plugins/isolate.py` & `pynose-1.4.5/nose/plugins/isolate.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.4/nose/plugins/logcapture.py` & `pynose-1.4.5/nose/plugins/logcapture.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.4/nose/plugins/manager.py` & `pynose-1.4.5/nose/plugins/manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,14 +45,16 @@
 from nose.failure import Failure
 from nose.plugins.base import IPluginInterface
 from nose.pyversion import sort_list
 
 __all__ = ['DefaultPluginManager', 'PluginManager', 'EntryPointPluginManager',
            'BuiltinPluginManager', 'RestrictedPluginManager']
 log = logging.getLogger(__name__)
+if not hasattr(inspect, "getargspec"):
+    inspect.getargspec = lambda func: inspect.getfullargspec(func)[:4]
 
 
 class PluginProxy(object):
     """Proxy for plugin calls. Essentially a closure bound to the
     given call and plugin list.
     The plugin proxy also must be bound to a particular plugin
     interface specification, so that it knows what calls are available
```

### Comparing `pynose-1.4.4/nose/plugins/multiprocess.py` & `pynose-1.4.5/nose/plugins/multiprocess.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.4/nose/plugins/plugintest.py` & `pynose-1.4.5/nose/plugins/plugintest.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.4/nose/plugins/skip.py` & `pynose-1.4.5/nose/plugins/skip.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.4/nose/plugins/testid.py` & `pynose-1.4.5/nose/plugins/testid.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.4/nose/plugins/xunit.py` & `pynose-1.4.5/nose/plugins/xunit.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.4/nose/proxy.py` & `pynose-1.4.5/nose/proxy.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.4/nose/pyversion.py` & `pynose-1.4.5/nose/pyversion.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.4/nose/result.py` & `pynose-1.4.5/nose/result.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.4/nose/selector.py` & `pynose-1.4.5/nose/selector.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.4/nose/sphinx/pluginopts.py` & `pynose-1.4.5/nose/sphinx/pluginopts.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.4/nose/suite.py` & `pynose-1.4.5/nose/suite.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.4/nose/tools/nontrivial.py` & `pynose-1.4.5/nose/tools/nontrivial.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.4/nose/tools/trivial.py` & `pynose-1.4.5/nose/tools/trivial.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.4/nose/twistedtools.py` & `pynose-1.4.5/nose/twistedtools.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.4/nose/usage.txt` & `pynose-1.4.5/nose/usage.txt`

 * *Files identical despite different names*

### Comparing `pynose-1.4.4/nose/util.py` & `pynose-1.4.5/nose/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 
 log = logging.getLogger('nose')
 ident_re = re.compile(r'^[A-Za-z_][A-Za-z0-9_.]*$')
 class_types = (ClassType, TypeType)
 skip_pattern = (
     r"(?:\.svn)|(?:[^.]+\.py[co])|(?:.*~)|(?:.*\$py\.class)|(?:__pycache__)"
 )
+if not hasattr(inspect, "getargspec"):
+    inspect.getargspec = lambda func: inspect.getfullargspec(func)[:4]
 try:
     set()
 except NameError:
     try:
         from sets import Set as set
     except ImportError:
         pass
@@ -418,16 +420,17 @@
                     # Not a function. If it's callable, call it anyway.
                     if (
                         hasattr(func, '__call__')
                         and not inspect.ismethod(func)
                     ):
                         func = func.__call__
                     try:
-                        args, varargs, varkw, defaults = \
+                        args, varargs, varkw, defaults = (
                             inspect.getargspec(func)
+                        )
                         args.pop(0)  # pop the self off
                     except TypeError:
                         raise TypeError("Attribute %s of %r is not a python "
                                         "function. Only functions or callables"
                                         " may be used as fixtures." %
                                         (name, obj))
                 if len(args):
```

### Comparing `pynose-1.4.4/pynose.egg-info/PKG-INFO` & `pynose-1.4.5/pynose.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynose
-Version: 1.4.4
+Version: 1.4.5
 Summary: pynose fixes nose to extend unittest and make testing easier
 Home-page: https://github.com/mdmintz/pynose
 Author: Michael Mintz
 Author-email: mdmintz@gmail.com
 License: MIT
 Project-URL: Download, https://pypi.org/project/pynose/#files
 Project-URL: PyPI, https://pypi.org/project/pynose/
@@ -43,17 +43,18 @@
 
 ``pynose`` is an updated version of ``nose``, originally made by Jason Pellerin.
 
 This version of ``nose`` is compatible with Python 3.6+ (including 3.12 & up).
 
 Changes in ``pynose`` from legacy ``nose`` include:
 * Fixes "AttributeError: module 'collections' has no attribute 'Callable'."
-* Fixes all ``flake8`` issues from the original ``nose``.
+* Fixes "AttributeError: module 'inspect' has no attribute 'getargspec'."
 * Fixes "ImportError: cannot import name '_TextTestResult' from 'unittest'."
 * Fixes "RuntimeWarning: TestResult has no addDuration method."
+* Fixes all ``flake8`` issues from the original ``nose``.
 * Replaces the ``imp`` module with the newer ``importlib`` module.
 * The default logging level now hides "debug" logs for less noise.
 * The ``-s`` option is always active to see the output of ``print()``.
 * Adds ``--co`` as a shortcut to using ``--collect-only``.
 
 --------
```

### Comparing `pynose-1.4.4/pynose.egg-info/SOURCES.txt` & `pynose-1.4.5/pynose.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pynose-1.4.4/setup.py` & `pynose-1.4.5/setup.py`

 * *Files identical despite different names*

