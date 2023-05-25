# Comparing `tmp/dissect.thumbcache-1.4.dev1.tar.gz` & `tmp/dissect.thumbcache-1.4.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dissect.thumbcache-1.4.dev1.tar", last modified: Mon May 15 12:48:41 2023, max compression
+gzip compressed data, was "dissect.thumbcache-1.4.dev2.tar", last modified: Tue May 16 13:27:03 2023, max compression
```

## Comparing `dissect.thumbcache-1.4.dev1.tar` & `dissect.thumbcache-1.4.dev2.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:41.603667 dissect.thumbcache-1.4.dev1/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-05-15 12:48:41.603667 dissect.thumbcache-1.4.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:41.571665 dissect.thumbcache-1.4.dev1/dissect/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:41.575666 dissect.thumbcache-1.4.dev1/dissect/thumbcache/
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/dissect/thumbcache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/dissect/thumbcache/c_thumbcache.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/dissect/thumbcache/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5572 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/dissect/thumbcache/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/dissect/thumbcache/thumbcache.py
--rw-r--r--   0 runner    (1001) docker     (123)     5091 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/dissect/thumbcache/thumbcache_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:41.575666 dissect.thumbcache-1.4.dev1/dissect/thumbcache/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/dissect/thumbcache/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/dissect/thumbcache/tools/extract_images.py
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/dissect/thumbcache/tools/extract_with_index.py
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/dissect/thumbcache/tools/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/dissect/thumbcache/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:41.575666 dissect.thumbcache-1.4.dev1/dissect.thumbcache.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-05-15 12:48:41.000000 dissect.thumbcache-1.4.dev1/dissect.thumbcache.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-05-15 12:48:41.000000 dissect.thumbcache-1.4.dev1/dissect.thumbcache.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 12:48:41.000000 dissect.thumbcache-1.4.dev1/dissect.thumbcache.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-15 12:48:41.000000 dissect.thumbcache-1.4.dev1/dissect.thumbcache.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-15 12:48:41.000000 dissect.thumbcache-1.4.dev1/dissect.thumbcache.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-15 12:48:41.000000 dissect.thumbcache-1.4.dev1/dissect.thumbcache.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-15 12:48:29.000000 dissect.thumbcache-1.4.dev1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 12:48:41.603667 dissect.thumbcache-1.4.dev1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:41.575666 dissect.thumbcache-1.4.dev1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:41.571665 dissect.thumbcache-1.4.dev1/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:41.587666 dissect.thumbcache-1.4.dev1/tests/data/windows_10/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/data/windows_10/thumbcache_1280.db
--rw-r--r--   0 runner    (1001) docker     (123)  1048576 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/data/windows_10/thumbcache_16.db
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/data/windows_10/thumbcache_1920.db
--rw-r--r--   0 runner    (1001) docker     (123)  1048576 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/data/windows_10/thumbcache_256.db
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/data/windows_10/thumbcache_2560.db
--rw-r--r--   0 runner    (1001) docker     (123)  1048576 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/data/windows_10/thumbcache_32.db
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/data/windows_10/thumbcache_48.db
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/data/windows_10/thumbcache_768.db
--rw-r--r--   0 runner    (1001) docker     (123)  3145728 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/data/windows_10/thumbcache_96.db
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/data/windows_10/thumbcache_custom_stream.db
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/data/windows_10/thumbcache_exif.db
--rw-r--r--   0 runner    (1001) docker     (123)    14688 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/data/windows_10/thumbcache_idx.db
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/data/windows_10/thumbcache_sr.db
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/data/windows_10/thumbcache_wide.db
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/data/windows_10/thumbcache_wide_alternate.db
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:41.595667 dissect.thumbcache-1.4.dev1/tests/data/windows_11/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/data/windows_11/thumbcache_1280.db
--rw-r--r--   0 runner    (1001) docker     (123)  1048576 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/data/windows_11/thumbcache_16.db
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/data/windows_11/thumbcache_1920.db
--rw-r--r--   0 runner    (1001) docker     (123)  1048576 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/data/windows_11/thumbcache_256.db
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/data/windows_11/thumbcache_2560.db
--rw-r--r--   0 runner    (1001) docker     (123)  1048576 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/data/windows_11/thumbcache_32.db
--rw-r--r--   0 runner    (1001) docker     (123)  1048576 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/data/windows_11/thumbcache_48.db
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/data/windows_11/thumbcache_768.db
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/data/windows_11/thumbcache_96.db
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/data/windows_11/thumbcache_custom_stream.db
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/data/windows_11/thumbcache_exif.db
--rw-r--r--   0 runner    (1001) docker     (123)     7416 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/data/windows_11/thumbcache_idx.db
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/data/windows_11/thumbcache_sr.db
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/data/windows_11/thumbcache_wide.db
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/data/windows_11/thumbcache_wide_alternate.db
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:41.595667 dissect.thumbcache-1.4.dev1/tests/data/windows_7/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/data/windows_7/thumbcache_1024.db
--rw-r--r--   0 runner    (1001) docker     (123)  1048576 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/data/windows_7/thumbcache_256.db
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/data/windows_7/thumbcache_32.db
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/data/windows_7/thumbcache_96.db
--rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/data/windows_7/thumbcache_idx.db
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/data/windows_7/thumbcache_sr.db
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:41.599667 dissect.thumbcache-1.4.dev1/tests/data/windows_81/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/data/windows_81/thumbcache_1024.db
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/data/windows_81/thumbcache_16.db
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/data/windows_81/thumbcache_1600.db
--rw-r--r--   0 runner    (1001) docker     (123)  1048576 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/data/windows_81/thumbcache_256.db
--rw-r--r--   0 runner    (1001) docker     (123)  1048576 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/data/windows_81/thumbcache_32.db
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/data/windows_81/thumbcache_48.db
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/data/windows_81/thumbcache_96.db
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/data/windows_81/thumbcache_exif.db
--rw-r--r--   0 runner    (1001) docker     (123)     6584 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/data/windows_81/thumbcache_idx.db
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/data/windows_81/thumbcache_sr.db
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/data/windows_81/thumbcache_wide.db
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/data/windows_81/thumbcache_wide_alternate.db
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:41.603667 dissect.thumbcache-1.4.dev1/tests/data/windows_vista/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/data/windows_vista/thumbcache_1024.db
--rw-r--r--   0 runner    (1001) docker     (123)  1048576 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/data/windows_vista/thumbcache_256.db
--rw-r--r--   0 runner    (1001) docker     (123)  1048576 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/data/windows_vista/thumbcache_32.db
--rw-r--r--   0 runner    (1001) docker     (123)  1048576 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/data/windows_vista/thumbcache_96.db
--rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/data/windows_vista/thumbcache_idx.db
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/data/windows_vista/thumbcache_sr.db
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:41.603667 dissect.thumbcache-1.4.dev1/tests/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/test_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/test_thumbcache.py
--rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tests/test_thumbcachefile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-15 12:48:23.000000 dissect.thumbcache-1.4.dev1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:27:03.923299 dissect.thumbcache-1.4.dev2/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-05-16 13:27:03.919299 dissect.thumbcache-1.4.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:27:03.879299 dissect.thumbcache-1.4.dev2/dissect/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:27:03.883299 dissect.thumbcache-1.4.dev2/dissect/thumbcache/
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/dissect/thumbcache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/dissect/thumbcache/c_thumbcache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/dissect/thumbcache/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5572 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/dissect/thumbcache/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/dissect/thumbcache/thumbcache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5091 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/dissect/thumbcache/thumbcache_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:27:03.883299 dissect.thumbcache-1.4.dev2/dissect/thumbcache/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/dissect/thumbcache/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/dissect/thumbcache/tools/extract_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/dissect/thumbcache/tools/extract_with_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/dissect/thumbcache/tools/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/dissect/thumbcache/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:27:03.883299 dissect.thumbcache-1.4.dev2/dissect.thumbcache.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-05-16 13:27:03.000000 dissect.thumbcache-1.4.dev2/dissect.thumbcache.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-05-16 13:27:03.000000 dissect.thumbcache-1.4.dev2/dissect.thumbcache.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 13:27:03.000000 dissect.thumbcache-1.4.dev2/dissect.thumbcache.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-16 13:27:03.000000 dissect.thumbcache-1.4.dev2/dissect.thumbcache.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-16 13:27:03.000000 dissect.thumbcache-1.4.dev2/dissect.thumbcache.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-16 13:27:03.000000 dissect.thumbcache-1.4.dev2/dissect.thumbcache.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-16 13:26:50.000000 dissect.thumbcache-1.4.dev2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 13:27:03.923299 dissect.thumbcache-1.4.dev2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:27:03.887299 dissect.thumbcache-1.4.dev2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:27:03.879299 dissect.thumbcache-1.4.dev2/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:27:03.899299 dissect.thumbcache-1.4.dev2/tests/data/windows_10/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/data/windows_10/thumbcache_1280.db
+-rw-r--r--   0 runner    (1001) docker     (123)  1048576 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/data/windows_10/thumbcache_16.db
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/data/windows_10/thumbcache_1920.db
+-rw-r--r--   0 runner    (1001) docker     (123)  1048576 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/data/windows_10/thumbcache_256.db
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/data/windows_10/thumbcache_2560.db
+-rw-r--r--   0 runner    (1001) docker     (123)  1048576 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/data/windows_10/thumbcache_32.db
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/data/windows_10/thumbcache_48.db
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/data/windows_10/thumbcache_768.db
+-rw-r--r--   0 runner    (1001) docker     (123)  3145728 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/data/windows_10/thumbcache_96.db
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/data/windows_10/thumbcache_custom_stream.db
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/data/windows_10/thumbcache_exif.db
+-rw-r--r--   0 runner    (1001) docker     (123)    14688 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/data/windows_10/thumbcache_idx.db
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/data/windows_10/thumbcache_sr.db
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/data/windows_10/thumbcache_wide.db
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/data/windows_10/thumbcache_wide_alternate.db
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:27:03.907299 dissect.thumbcache-1.4.dev2/tests/data/windows_11/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/data/windows_11/thumbcache_1280.db
+-rw-r--r--   0 runner    (1001) docker     (123)  1048576 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/data/windows_11/thumbcache_16.db
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/data/windows_11/thumbcache_1920.db
+-rw-r--r--   0 runner    (1001) docker     (123)  1048576 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/data/windows_11/thumbcache_256.db
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/data/windows_11/thumbcache_2560.db
+-rw-r--r--   0 runner    (1001) docker     (123)  1048576 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/data/windows_11/thumbcache_32.db
+-rw-r--r--   0 runner    (1001) docker     (123)  1048576 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/data/windows_11/thumbcache_48.db
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/data/windows_11/thumbcache_768.db
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/data/windows_11/thumbcache_96.db
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/data/windows_11/thumbcache_custom_stream.db
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/data/windows_11/thumbcache_exif.db
+-rw-r--r--   0 runner    (1001) docker     (123)     7416 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/data/windows_11/thumbcache_idx.db
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/data/windows_11/thumbcache_sr.db
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/data/windows_11/thumbcache_wide.db
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/data/windows_11/thumbcache_wide_alternate.db
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:27:03.911299 dissect.thumbcache-1.4.dev2/tests/data/windows_7/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/data/windows_7/thumbcache_1024.db
+-rw-r--r--   0 runner    (1001) docker     (123)  1048576 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/data/windows_7/thumbcache_256.db
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/data/windows_7/thumbcache_32.db
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/data/windows_7/thumbcache_96.db
+-rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/data/windows_7/thumbcache_idx.db
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/data/windows_7/thumbcache_sr.db
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:27:03.915299 dissect.thumbcache-1.4.dev2/tests/data/windows_81/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/data/windows_81/thumbcache_1024.db
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/data/windows_81/thumbcache_16.db
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/data/windows_81/thumbcache_1600.db
+-rw-r--r--   0 runner    (1001) docker     (123)  1048576 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/data/windows_81/thumbcache_256.db
+-rw-r--r--   0 runner    (1001) docker     (123)  1048576 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/data/windows_81/thumbcache_32.db
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/data/windows_81/thumbcache_48.db
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/data/windows_81/thumbcache_96.db
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/data/windows_81/thumbcache_exif.db
+-rw-r--r--   0 runner    (1001) docker     (123)     6584 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/data/windows_81/thumbcache_idx.db
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/data/windows_81/thumbcache_sr.db
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/data/windows_81/thumbcache_wide.db
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/data/windows_81/thumbcache_wide_alternate.db
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:27:03.919299 dissect.thumbcache-1.4.dev2/tests/data/windows_vista/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/data/windows_vista/thumbcache_1024.db
+-rw-r--r--   0 runner    (1001) docker     (123)  1048576 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/data/windows_vista/thumbcache_256.db
+-rw-r--r--   0 runner    (1001) docker     (123)  1048576 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/data/windows_vista/thumbcache_32.db
+-rw-r--r--   0 runner    (1001) docker     (123)  1048576 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/data/windows_vista/thumbcache_96.db
+-rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/data/windows_vista/thumbcache_idx.db
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/data/windows_vista/thumbcache_sr.db
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:27:03.919299 dissect.thumbcache-1.4.dev2/tests/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/test_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/test_thumbcache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tests/test_thumbcachefile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-16 13:26:44.000000 dissect.thumbcache-1.4.dev2/tox.ini
```

### Comparing `dissect.thumbcache-1.4.dev1/LICENSE` & `dissect.thumbcache-1.4.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.4.dev1/PKG-INFO` & `dissect.thumbcache-1.4.dev2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.thumbcache
-Version: 1.4.dev1
+Version: 1.4.dev2
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.thumbcache
 Project-URL: repository, https://github.com/fox-it/dissect.thumbcache
 Classifier: Programming Language :: Python :: 3
 Requires-Python: ~=3.9
@@ -19,14 +19,20 @@
 
 For more information, please see [the documentation](https://docs.dissect.tools/en/latest/projects/dissect.thumbcache/index.html).
 
 ## Windows Vista+
 
 The project currently only supports the Windows Vista+ indexed thumbcache. The Windows XP format is currently not implemented.
 
+## Requirements
+
+This project is part of the Dissect framework and requires Python.
+
+Information on the supported Python versions can be found in the Getting Started section of [the documentation](https://docs.dissect.tools/en/latest/index.html#getting-started).
+
 ## Installation
 
 `dissect.thumbcache` is available on [PyPI](https://pypi.org/project/dissect.thumbcache/).
 
 ```bash
 pip install dissect.thumbcache
 ```
@@ -48,20 +54,20 @@
 using the default installed Python version, run:
 
 ```bash
 tox
 ```
 
 For a more elaborate explanation on how to build and test the project, please see [the
-documentation](https://docs.dissect.tools/en/latest/contributing/developing.html#building-testing).
+documentation](https://docs.dissect.tools/en/latest/contributing/tooling.html).
 
 ## Contributing
 
 The Dissect project encourages any contribution to the codebase. To make your contribution fit into the project, please
-refer to [the style guide](https://docs.dissect.tools/en/latest/contributing/style-guide.html).
+refer to [the development guide](https://docs.dissect.tools/en/latest/contributing/developing.html).
 
 ## Copyright and license
 
 Dissect is released as open source by Fox-IT (<https://www.fox-it.com>) part of NCC Group Plc
 (<https://www.nccgroup.com>).
 
 Developed by the Dissect Team (<dissect@fox-it.com>) and made available at <https://github.com/fox-it/dissect>.
```

### Comparing `dissect.thumbcache-1.4.dev1/README.md` & `dissect.thumbcache-1.4.dev2/dissect.thumbcache.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,38 @@
+Metadata-Version: 2.1
+Name: dissect.thumbcache
+Version: 1.4.dev2
+Author-email: Dissect Team <dissect@fox-it.com>
+License: Affero General Public License v3
+Project-URL: homepage, https://dissect.tools
+Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.thumbcache
+Project-URL: repository, https://github.com/fox-it/dissect.thumbcache
+Classifier: Programming Language :: Python :: 3
+Requires-Python: ~=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: COPYRIGHT
+
 # dissect.thumbcache
 
 A Dissect module implementing parsers for the thumbcache of Windows systems.
 This is commonly used to see which files were opened on a system.
 
 For more information, please see [the documentation](https://docs.dissect.tools/en/latest/projects/dissect.thumbcache/index.html).
 
 ## Windows Vista+
 
 The project currently only supports the Windows Vista+ indexed thumbcache. The Windows XP format is currently not implemented.
 
+## Requirements
+
+This project is part of the Dissect framework and requires Python.
+
+Information on the supported Python versions can be found in the Getting Started section of [the documentation](https://docs.dissect.tools/en/latest/index.html#getting-started).
+
 ## Installation
 
 `dissect.thumbcache` is available on [PyPI](https://pypi.org/project/dissect.thumbcache/).
 
 ```bash
 pip install dissect.thumbcache
 ```
@@ -34,20 +54,20 @@
 using the default installed Python version, run:
 
 ```bash
 tox
 ```
 
 For a more elaborate explanation on how to build and test the project, please see [the
-documentation](https://docs.dissect.tools/en/latest/contributing/developing.html#building-testing).
+documentation](https://docs.dissect.tools/en/latest/contributing/tooling.html).
 
 ## Contributing
 
 The Dissect project encourages any contribution to the codebase. To make your contribution fit into the project, please
-refer to [the style guide](https://docs.dissect.tools/en/latest/contributing/style-guide.html).
+refer to [the development guide](https://docs.dissect.tools/en/latest/contributing/developing.html).
 
 ## Copyright and license
 
 Dissect is released as open source by Fox-IT (<https://www.fox-it.com>) part of NCC Group Plc
 (<https://www.nccgroup.com>).
 
 Developed by the Dissect Team (<dissect@fox-it.com>) and made available at <https://github.com/fox-it/dissect>.
```

### Comparing `dissect.thumbcache-1.4.dev1/dissect/thumbcache/c_thumbcache.py` & `dissect.thumbcache-1.4.dev2/dissect/thumbcache/c_thumbcache.py`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.4.dev1/dissect/thumbcache/index.py` & `dissect.thumbcache-1.4.dev2/dissect/thumbcache/index.py`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.4.dev1/dissect/thumbcache/thumbcache.py` & `dissect.thumbcache-1.4.dev2/dissect/thumbcache/thumbcache.py`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.4.dev1/dissect/thumbcache/thumbcache_file.py` & `dissect.thumbcache-1.4.dev2/dissect/thumbcache/thumbcache_file.py`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.4.dev1/dissect/thumbcache/tools/extract_images.py` & `dissect.thumbcache-1.4.dev2/dissect/thumbcache/tools/extract_images.py`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.4.dev1/dissect/thumbcache/tools/extract_with_index.py` & `dissect.thumbcache-1.4.dev2/dissect/thumbcache/tools/extract_with_index.py`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.4.dev1/dissect/thumbcache/tools/utils.py` & `dissect.thumbcache-1.4.dev2/dissect/thumbcache/tools/utils.py`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.4.dev1/dissect.thumbcache.egg-info/PKG-INFO` & `dissect.thumbcache-1.4.dev2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,24 @@
-Metadata-Version: 2.1
-Name: dissect.thumbcache
-Version: 1.4.dev1
-Author-email: Dissect Team <dissect@fox-it.com>
-License: Affero General Public License v3
-Project-URL: homepage, https://dissect.tools
-Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.thumbcache
-Project-URL: repository, https://github.com/fox-it/dissect.thumbcache
-Classifier: Programming Language :: Python :: 3
-Requires-Python: ~=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-License-File: COPYRIGHT
-
 # dissect.thumbcache
 
 A Dissect module implementing parsers for the thumbcache of Windows systems.
 This is commonly used to see which files were opened on a system.
 
 For more information, please see [the documentation](https://docs.dissect.tools/en/latest/projects/dissect.thumbcache/index.html).
 
 ## Windows Vista+
 
 The project currently only supports the Windows Vista+ indexed thumbcache. The Windows XP format is currently not implemented.
 
+## Requirements
+
+This project is part of the Dissect framework and requires Python.
+
+Information on the supported Python versions can be found in the Getting Started section of [the documentation](https://docs.dissect.tools/en/latest/index.html#getting-started).
+
 ## Installation
 
 `dissect.thumbcache` is available on [PyPI](https://pypi.org/project/dissect.thumbcache/).
 
 ```bash
 pip install dissect.thumbcache
 ```
@@ -48,20 +40,20 @@
 using the default installed Python version, run:
 
 ```bash
 tox
 ```
 
 For a more elaborate explanation on how to build and test the project, please see [the
-documentation](https://docs.dissect.tools/en/latest/contributing/developing.html#building-testing).
+documentation](https://docs.dissect.tools/en/latest/contributing/tooling.html).
 
 ## Contributing
 
 The Dissect project encourages any contribution to the codebase. To make your contribution fit into the project, please
-refer to [the style guide](https://docs.dissect.tools/en/latest/contributing/style-guide.html).
+refer to [the development guide](https://docs.dissect.tools/en/latest/contributing/developing.html).
 
 ## Copyright and license
 
 Dissect is released as open source by Fox-IT (<https://www.fox-it.com>) part of NCC Group Plc
 (<https://www.nccgroup.com>).
 
 Developed by the Dissect Team (<dissect@fox-it.com>) and made available at <https://github.com/fox-it/dissect>.
```

### Comparing `dissect.thumbcache-1.4.dev1/dissect.thumbcache.egg-info/SOURCES.txt` & `dissect.thumbcache-1.4.dev2/dissect.thumbcache.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.4.dev1/pyproject.toml` & `dissect.thumbcache-1.4.dev2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.4.dev1/tests/data/windows_10/thumbcache_16.db` & `dissect.thumbcache-1.4.dev2/tests/data/windows_10/thumbcache_16.db`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.4.dev1/tests/data/windows_10/thumbcache_256.db` & `dissect.thumbcache-1.4.dev2/tests/data/windows_10/thumbcache_256.db`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.4.dev1/tests/data/windows_10/thumbcache_32.db` & `dissect.thumbcache-1.4.dev2/tests/data/windows_10/thumbcache_32.db`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.4.dev1/tests/data/windows_10/thumbcache_96.db` & `dissect.thumbcache-1.4.dev2/tests/data/windows_10/thumbcache_96.db`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.4.dev1/tests/data/windows_10/thumbcache_idx.db` & `dissect.thumbcache-1.4.dev2/tests/data/windows_10/thumbcache_idx.db`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.4.dev1/tests/data/windows_11/thumbcache_16.db` & `dissect.thumbcache-1.4.dev2/tests/data/windows_11/thumbcache_16.db`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.4.dev1/tests/data/windows_11/thumbcache_256.db` & `dissect.thumbcache-1.4.dev2/tests/data/windows_11/thumbcache_256.db`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.4.dev1/tests/data/windows_11/thumbcache_32.db` & `dissect.thumbcache-1.4.dev2/tests/data/windows_11/thumbcache_32.db`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.4.dev1/tests/data/windows_11/thumbcache_48.db` & `dissect.thumbcache-1.4.dev2/tests/data/windows_11/thumbcache_48.db`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.4.dev1/tests/data/windows_11/thumbcache_idx.db` & `dissect.thumbcache-1.4.dev2/tests/data/windows_11/thumbcache_idx.db`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.4.dev1/tests/data/windows_7/thumbcache_256.db` & `dissect.thumbcache-1.4.dev2/tests/data/windows_7/thumbcache_256.db`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.4.dev1/tests/data/windows_7/thumbcache_idx.db` & `dissect.thumbcache-1.4.dev2/tests/data/windows_7/thumbcache_idx.db`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.4.dev1/tests/data/windows_81/thumbcache_256.db` & `dissect.thumbcache-1.4.dev2/tests/data/windows_81/thumbcache_256.db`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.4.dev1/tests/data/windows_81/thumbcache_32.db` & `dissect.thumbcache-1.4.dev2/tests/data/windows_81/thumbcache_32.db`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.4.dev1/tests/data/windows_81/thumbcache_idx.db` & `dissect.thumbcache-1.4.dev2/tests/data/windows_81/thumbcache_idx.db`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.4.dev1/tests/data/windows_vista/thumbcache_256.db` & `dissect.thumbcache-1.4.dev2/tests/data/windows_vista/thumbcache_256.db`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.4.dev1/tests/data/windows_vista/thumbcache_32.db` & `dissect.thumbcache-1.4.dev2/tests/data/windows_vista/thumbcache_32.db`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.4.dev1/tests/data/windows_vista/thumbcache_96.db` & `dissect.thumbcache-1.4.dev2/tests/data/windows_vista/thumbcache_96.db`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.4.dev1/tests/data/windows_vista/thumbcache_idx.db` & `dissect.thumbcache-1.4.dev2/tests/data/windows_vista/thumbcache_idx.db`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.4.dev1/tests/docs/Makefile` & `dissect.thumbcache-1.4.dev2/tests/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.4.dev1/tests/docs/conf.py` & `dissect.thumbcache-1.4.dev2/tests/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.4.dev1/tests/test_index.py` & `dissect.thumbcache-1.4.dev2/tests/test_index.py`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.4.dev1/tests/test_thumbcache.py` & `dissect.thumbcache-1.4.dev2/tests/test_thumbcache.py`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.4.dev1/tests/test_thumbcachefile.py` & `dissect.thumbcache-1.4.dev2/tests/test_thumbcachefile.py`

 * *Files identical despite different names*

### Comparing `dissect.thumbcache-1.4.dev1/tox.ini` & `dissect.thumbcache-1.4.dev2/tox.ini`

 * *Files identical despite different names*

