# Comparing `tmp/spai-0.1.0.tar.gz` & `tmp/spai-2023.5.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spai-0.1.0.tar", max compression
+gzip compressed data, was "spai-2023.5.25.tar", max compression
```

## Comparing `spai-0.1.0.tar` & `spai-2023.5.25.tar`

### file list

```diff
@@ -1,5 +1,28 @@
--rw-r--r--   0        0        0        0 2023-05-05 12:23:03.552010 spai-0.1.0/README.md
--rw-r--r--   0        0        0      259 2023-05-05 12:23:03.556010 spai-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-05 12:23:03.552010 spai-0.1.0/spai/__init__.py
--rw-r--r--   0        0        0       32 2023-05-05 12:23:32.112166 spai-0.1.0/spai/hello.py
--rw-r--r--   0        0        0      429 1970-01-01 00:00:00.000000 spai-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-12 05:51:22.950543 spai-2023.5.25/README.md
+-rw-r--r--   0        0        0      264 2023-05-25 06:41:35.471523 spai-2023.5.25/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-25 05:56:52.038729 spai-2023.5.25/spai/__init__.py
+-rw-r--r--   0        0        0      140 2023-05-21 10:11:30.915314 spai-2023.5.25/spai/cli/__init__.py
+-rw-r--r--   0        0        0     1297 2023-05-21 08:39:35.055997 spai-2023.5.25/spai/cli/cloud.py
+-rw-r--r--   0        0        0        0 2023-05-12 05:53:50.146413 spai-2023.5.25/spai/cli/commands/__init__.py
+-rw-r--r--   0        0        0      266 2023-05-12 05:59:27.734580 spai-2023.5.25/spai/cli/commands/hello.py
+-rw-r--r--   0        0        0     5533 2023-05-21 10:50:31.176515 spai-2023.5.25/spai/cli/local.py
+-rw-r--r--   0        0        0     2495 2023-05-21 09:35:01.310684 spai-2023.5.25/spai/cli/validate.py
+-rw-r--r--   0        0        0        0 2023-05-19 06:35:36.838003 spai-2023.5.25/spai/data/__init__.py
+-rw-r--r--   0        0        0       93 2023-05-25 06:12:52.855484 spai-2023.5.25/spai/data/satellite/__init__.py
+-rw-r--r--   0        0        0     2129 2023-05-25 06:27:31.453555 spai-2023.5.25/spai/data/satellite/download.py
+-rw-r--r--   0        0        0     1264 2023-05-25 06:15:22.923801 spai-2023.5.25/spai/data/satellite/explore.py
+-rw-r--r--   0        0        0     3400 2023-05-25 06:20:08.928458 spai-2023.5.25/spai/data/satellite/sentinelhub/SHDownloader.py
+-rw-r--r--   0        0        0     2434 2023-05-25 06:09:12.743073 spai-2023.5.25/spai/data/satellite/sentinelhub/SHExplorer.py
+-rw-r--r--   0        0        0     1209 2023-05-25 06:16:32.727955 spai-2023.5.25/spai/data/satellite/sentinelhub/SHS2Downloader.py
+-rw-r--r--   0        0        0      276 2023-05-25 05:49:51.650010 spai-2023.5.25/spai/data/satellite/sentinelhub/SHS2L2ADownloader.py
+-rw-r--r--   0        0        0       84 2023-05-25 05:50:35.998156 spai-2023.5.25/spai/data/satellite/sentinelhub/__init__.py
+-rw-r--r--   0        0        0       29 2023-05-25 06:31:59.119564 spai-2023.5.25/spai/image/__init__.py
+-rw-r--r--   0        0        0      603 2023-05-25 06:36:00.653454 spai-2023.5.25/spai/image/utils.py
+-rw-r--r--   0        0        0     3892 2023-05-19 06:36:13.726144 spai-2023.5.25/spai/main.bck
+-rw-r--r--   0        0        0     1006 2023-05-22 09:43:14.295844 spai-2023.5.25/spai/main.py
+-rw-r--r--   0        0        0       84 2023-05-25 06:27:12.053506 spai-2023.5.25/spai/models.py
+-rw-r--r--   0        0        0      433 2023-05-25 06:28:52.517762 spai-2023.5.25/spai/storage/Storage.py
+-rw-r--r--   0        0        0       29 2023-05-25 06:29:06.645887 spai-2023.5.25/spai/storage/__init__.py
+-rw-r--r--   0        0        0      372 2023-05-25 05:43:36.956784 spai-2023.5.25/spai/storage/minio.py
+-rw-r--r--   0        0        0      633 1970-01-01 00:00:00.000000 spai-2023.5.25/setup.py
+-rw-r--r--   0        0        0      382 1970-01-01 00:00:00.000000 spai-2023.5.25/PKG-INFO
```

