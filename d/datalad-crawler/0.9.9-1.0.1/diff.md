# Comparing `tmp/datalad_crawler-0.9.9.tar.gz` & `tmp/datalad_crawler-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/datalad-crawler/datalad-crawler/dist/tmpec6lbmqa/datalad_crawler-0.9.9.tar", last modified: Mon Oct 31 19:56:04 2022, max compression
+gzip compressed data, was "datalad_crawler-1.0.1.tar", last modified: Thu May 25 17:49:44 2023, max compression
```

## Comparing `datalad_crawler-0.9.9.tar` & `datalad_crawler-1.0.1.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 19:56:04.000000 datalad_crawler-0.9.9/
--rw-r--r--   0 runner    (1001) docker     (121)    10446 2022-10-31 19:55:46.000000 datalad_crawler-0.9.9/formatters.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-31 19:56:04.000000 datalad_crawler-0.9.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     5226 2022-10-31 19:55:46.000000 datalad_crawler-0.9.9/setup_support.py
--rw-r--r--   0 runner    (1001) docker     (121)     3805 2022-10-31 19:55:46.000000 datalad_crawler-0.9.9/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       39 2022-10-31 19:55:46.000000 datalad_crawler-0.9.9/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 19:56:04.000000 datalad_crawler-0.9.9/datalad_crawler/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 19:56:04.000000 datalad_crawler-0.9.9/datalad_crawler/dbs/
--rw-r--r--   0 runner    (1001) docker     (121)     3158 2022-10-31 19:55:46.000000 datalad_crawler-0.9.9/datalad_crawler/dbs/versions.py
--rw-r--r--   0 runner    (1001) docker     (121)     5242 2022-10-31 19:55:46.000000 datalad_crawler-0.9.9/datalad_crawler/dbs/files.py
--rw-r--r--   0 runner    (1001) docker     (121)     7232 2022-10-31 19:55:46.000000 datalad_crawler-0.9.9/datalad_crawler/dbs/base.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 19:56:04.000000 datalad_crawler-0.9.9/datalad_crawler/dbs/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     5225 2022-10-31 19:55:46.000000 datalad_crawler-0.9.9/datalad_crawler/dbs/tests/test_files.py
--rw-r--r--   0 runner    (1001) docker     (121)      389 2022-10-31 19:55:46.000000 datalad_crawler-0.9.9/datalad_crawler/dbs/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      461 2022-10-31 19:55:46.000000 datalad_crawler-0.9.9/datalad_crawler/dbs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8094 2022-10-31 19:55:46.000000 datalad_crawler-0.9.9/datalad_crawler/crawl.py
--rw-r--r--   0 runner    (1001) docker     (121)     1026 2022-10-31 19:55:46.000000 datalad_crawler-0.9.9/datalad_crawler/consts.py
--rw-r--r--   0 runner    (1001) docker     (121)     1974 2022-10-31 19:55:46.000000 datalad_crawler-0.9.9/datalad_crawler/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 19:56:04.000000 datalad_crawler-0.9.9/datalad_crawler/pipelines/
--rw-r--r--   0 runner    (1001) docker     (121)    11412 2022-10-31 19:55:46.000000 datalad_crawler-0.9.9/datalad_crawler/pipelines/crcns.py
--rw-r--r--   0 runner    (1001) docker     (121)     1767 2022-10-31 19:55:46.000000 datalad_crawler-0.9.9/datalad_crawler/pipelines/stanford_lib.py
--rw-r--r--   0 runner    (1001) docker     (121)     7074 2022-10-31 19:55:46.000000 datalad_crawler-0.9.9/datalad_crawler/pipelines/fcptable.py
--rw-r--r--   0 runner    (1001) docker     (121)     4081 2022-10-31 19:55:46.000000 datalad_crawler-0.9.9/datalad_crawler/pipelines/openfmri_s3.py
--rw-r--r--   0 runner    (1001) docker     (121)    13443 2022-10-31 19:55:46.000000 datalad_crawler-0.9.9/datalad_crawler/pipelines/xnat.py
--rw-r--r--   0 runner    (1001) docker     (121)     6373 2022-10-31 19:55:46.000000 datalad_crawler-0.9.9/datalad_crawler/pipelines/simple_s3.py
--rw-r--r--   0 runner    (1001) docker     (121)     9890 2022-10-31 19:55:46.000000 datalad_crawler-0.9.9/datalad_crawler/pipelines/balsa.py
--rw-r--r--   0 runner    (1001) docker     (121)     6045 2022-10-31 19:55:46.000000 datalad_crawler-0.9.9/datalad_crawler/pipelines/nda.py
--rw-r--r--   0 runner    (1001) docker     (121)    14182 2022-10-31 19:55:46.000000 datalad_crawler-0.9.9/datalad_crawler/pipelines/openfmri.py
--rw-r--r--   0 runner    (1001) docker     (121)     9392 2022-10-31 19:55:46.000000 datalad_crawler-0.9.9/datalad_crawler/pipelines/gh.py
--rw-r--r--   0 runner    (1001) docker     (121)     5490 2022-10-31 19:55:46.000000 datalad_crawler-0.9.9/datalad_crawler/pipelines/simple_with_archives.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 19:56:04.000000 datalad_crawler-0.9.9/datalad_crawler/pipelines/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     1030 2022-10-31 19:55:46.000000 datalad_crawler-0.9.9/datalad_crawler/pipelines/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     1132 2022-10-31 19:55:46.000000 datalad_crawler-0.9.9/datalad_crawler/pipelines/tests/test_gh.py
--rw-r--r--   0 runner    (1001) docker     (121)     4496 2022-10-31 19:55:46.000000 datalad_crawler-0.9.9/datalad_crawler/pipelines/tests/test_simple_s3.py
--rw-r--r--   0 runner    (1001) docker     (121)     3011 2022-10-31 19:55:46.000000 datalad_crawler-0.9.9/datalad_crawler/pipelines/tests/test_openfmri_collection.py
--rw-r--r--   0 runner    (1001) docker     (121)    12921 2022-10-31 19:55:46.000000 datalad_crawler-0.9.9/datalad_crawler/pipelines/tests/test_balsa.py
--rw-r--r--   0 runner    (1001) docker     (121)     1104 2022-10-31 19:55:46.000000 datalad_crawler-0.9.9/datalad_crawler/pipelines/tests/test_nda.py
--rw-r--r--   0 runner    (1001) docker     (121)     1885 2022-10-31 19:55:46.000000 datalad_crawler-0.9.9/datalad_crawler/pipelines/tests/test_crcns.py
--rw-r--r--   0 runner    (1001) docker     (121)     5554 2022-10-31 19:55:46.000000 datalad_crawler-0.9.9/datalad_crawler/pipelines/tests/test_xnat.py
--rw-r--r--   0 runner    (1001) docker     (121)    27478 2022-10-31 19:55:46.000000 datalad_crawler-0.9.9/datalad_crawler/pipelines/tests/test_openfmri.py
--rw-r--r--   0 runner    (1001) docker     (121)     5090 2022-10-31 19:55:46.000000 datalad_crawler-0.9.9/datalad_crawler/pipelines/tests/test_simple_with_archives.py
--rw-r--r--   0 runner    (1001) docker     (121)     3146 2022-10-31 19:55:46.000000 datalad_crawler-0.9.9/datalad_crawler/pipelines/tests/test_fcptable.py
--rw-r--r--   0 runner    (1001) docker     (121)      191 2022-10-31 19:55:46.000000 datalad_crawler-0.9.9/datalad_crawler/pipelines/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1017 2022-10-31 19:55:46.000000 datalad_crawler-0.9.9/datalad_crawler/pipelines/template.py
--rw-r--r--   0 runner    (1001) docker     (121)      458 2022-10-31 19:55:46.000000 datalad_crawler-0.9.9/datalad_crawler/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3175 2022-10-31 19:55:46.000000 datalad_crawler-0.9.9/datalad_crawler/pipelines/abstractsonline.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 19:56:04.000000 datalad_crawler-0.9.9/datalad_crawler/nodes/
--rw-r--r--   0 runner    (1001) docker     (121)    69530 2022-10-31 19:55:46.000000 datalad_crawler-0.9.9/datalad_crawler/nodes/annex.py
--rw-r--r--   0 runner    (1001) docker     (121)     6857 2022-10-31 19:55:46.000000 datalad_crawler-0.9.9/datalad_crawler/nodes/crawl_url.py
--rw-r--r--   0 runner    (1001) docker     (121)    13233 2022-10-31 19:55:46.000000 datalad_crawler-0.9.9/datalad_crawler/nodes/s3.py
--rw-r--r--   0 runner    (1001) docker     (121)     7406 2022-10-31 19:55:46.000000 datalad_crawler-0.9.9/datalad_crawler/nodes/matches.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 19:56:04.000000 datalad_crawler-0.9.9/datalad_crawler/nodes/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     4136 2022-10-31 19:55:46.000000 datalad_crawler-0.9.9/datalad_crawler/nodes/tests/test_matches.py
--rw-r--r--   0 runner    (1001) docker     (121)     2993 2022-10-31 19:55:46.000000 datalad_crawler-0.9.9/datalad_crawler/nodes/tests/test_crawl_url.py
--rw-r--r--   0 runner    (1001) docker     (121)    16825 2022-10-31 19:55:46.000000 datalad_crawler-0.9.9/datalad_crawler/nodes/tests/test_annex.py
--rw-r--r--   0 runner    (1001) docker     (121)    17845 2022-10-31 19:55:46.000000 datalad_crawler-0.9.9/datalad_crawler/nodes/tests/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (121)     9465 2022-10-31 19:55:46.000000 datalad_crawler-0.9.9/datalad_crawler/nodes/tests/test_s3.py
--rw-r--r--   0 runner    (1001) docker     (121)      509 2022-10-31 19:55:46.000000 datalad_crawler-0.9.9/datalad_crawler/nodes/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    18903 2022-10-31 19:55:46.000000 datalad_crawler-0.9.9/datalad_crawler/nodes/misc.py
--rw-r--r--   0 runner    (1001) docker     (121)      894 2022-10-31 19:55:46.000000 datalad_crawler-0.9.9/datalad_crawler/nodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      503 2022-10-31 19:55:46.000000 datalad_crawler-0.9.9/datalad_crawler/base.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 19:56:04.000000 datalad_crawler-0.9.9/datalad_crawler/support/
--rw-r--r--   0 runner    (1001) docker     (121)     6912 2022-10-31 19:55:46.000000 datalad_crawler-0.9.9/datalad_crawler/support/versions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 19:56:04.000000 datalad_crawler-0.9.9/datalad_crawler/support/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     6028 2022-10-31 19:55:46.000000 datalad_crawler-0.9.9/datalad_crawler/support/tests/test_versions.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-31 19:55:46.000000 datalad_crawler-0.9.9/datalad_crawler/support/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-31 19:55:46.000000 datalad_crawler-0.9.9/datalad_crawler/support/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      494 2022-10-31 19:55:46.000000 datalad_crawler-0.9.9/datalad_crawler/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-10-31 19:55:46.000000 datalad_crawler-0.9.9/datalad_crawler/version.py
--rw-r--r--   0 runner    (1001) docker     (121)     4056 2022-10-31 19:55:46.000000 datalad_crawler-0.9.9/datalad_crawler/crawl_init.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 19:56:04.000000 datalad_crawler-0.9.9/datalad_crawler/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     1067 2022-10-31 19:55:46.000000 datalad_crawler-0.9.9/datalad_crawler/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     3964 2022-10-31 19:55:46.000000 datalad_crawler-0.9.9/datalad_crawler/tests/test_crawl.py
--rw-r--r--   0 runner    (1001) docker     (121)     3462 2022-10-31 19:55:46.000000 datalad_crawler-0.9.9/datalad_crawler/tests/test_crawl_init.py
--rw-r--r--   0 runner    (1001) docker     (121)    10010 2022-10-31 19:55:46.000000 datalad_crawler-0.9.9/datalad_crawler/tests/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (121)       82 2022-10-31 19:55:46.000000 datalad_crawler-0.9.9/datalad_crawler/tests/test_register.py
--rw-r--r--   0 runner    (1001) docker     (121)      580 2022-10-31 19:55:46.000000 datalad_crawler-0.9.9/datalad_crawler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    21807 2022-10-31 19:55:46.000000 datalad_crawler-0.9.9/datalad_crawler/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (121)      952 2022-10-31 19:55:46.000000 datalad_crawler-0.9.9/datalad_crawler/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2482 2022-10-31 19:55:46.000000 datalad_crawler-0.9.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-31 19:56:04.000000 datalad_crawler-0.9.9/datalad_crawler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-10-31 19:56:03.000000 datalad_crawler-0.9.9/datalad_crawler.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      318 2022-10-31 19:56:03.000000 datalad_crawler-0.9.9/datalad_crawler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-31 19:56:03.000000 datalad_crawler-0.9.9/datalad_crawler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2695 2022-10-31 19:56:03.000000 datalad_crawler-0.9.9/datalad_crawler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4255 2022-10-31 19:56:03.000000 datalad_crawler-0.9.9/datalad_crawler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-10-31 19:56:03.000000 datalad_crawler-0.9.9/datalad_crawler.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1300 2022-10-31 19:55:46.000000 datalad_crawler-0.9.9/COPYING
--rw-r--r--   0 runner    (1001) docker     (121)     4255 2022-10-31 19:56:04.000000 datalad_crawler-0.9.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:49:44.588412 datalad_crawler-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-05-25 17:49:44.588412 datalad_crawler-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3805 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:49:44.576411 datalad_crawler-1.0.1/datalad_crawler/
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8094 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/crawl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/crawl_init.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:49:44.580411 datalad_crawler-1.0.1/datalad_crawler/dbs/
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/dbs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7232 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/dbs/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/dbs/files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:49:44.580411 datalad_crawler-1.0.1/datalad_crawler/dbs/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/dbs/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5225 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/dbs/tests/test_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/dbs/versions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:49:44.580411 datalad_crawler-1.0.1/datalad_crawler/nodes/
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/nodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69530 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/nodes/annex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6857 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/nodes/crawl_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7406 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/nodes/matches.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18903 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/nodes/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13234 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/nodes/s3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:49:44.580411 datalad_crawler-1.0.1/datalad_crawler/nodes/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/nodes/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16822 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/nodes/tests/test_annex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/nodes/tests/test_crawl_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/nodes/tests/test_matches.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17845 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/nodes/tests/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9465 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/nodes/tests/test_s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21807 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:49:44.584411 datalad_crawler-1.0.1/datalad_crawler/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/pipelines/abstractsonline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9890 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/pipelines/balsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11412 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/pipelines/crcns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7075 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/pipelines/fcptable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9392 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/pipelines/gh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6045 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/pipelines/nda.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14182 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/pipelines/openfmri.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/pipelines/openfmri_s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6373 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/pipelines/simple_s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/pipelines/simple_with_archives.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/pipelines/stanford_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/pipelines/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:49:44.584411 datalad_crawler-1.0.1/datalad_crawler/pipelines/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/pipelines/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12921 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/pipelines/tests/test_balsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/pipelines/tests/test_crcns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/pipelines/tests/test_fcptable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/pipelines/tests/test_gh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/pipelines/tests/test_nda.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27478 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/pipelines/tests/test_openfmri.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/pipelines/tests/test_openfmri_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/pipelines/tests/test_simple_s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/pipelines/tests/test_simple_with_archives.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/pipelines/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5554 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/pipelines/tests/test_xnat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13444 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/pipelines/xnat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:49:44.584411 datalad_crawler-1.0.1/datalad_crawler/support/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/support/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:49:44.584411 datalad_crawler-1.0.1/datalad_crawler/support/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/support/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6028 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/support/tests/test_versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/support/versions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:49:44.588412 datalad_crawler-1.0.1/datalad_crawler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/tests/test_crawl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/tests/test_crawl_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10010 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/tests/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/tests/test_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/datalad_crawler/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:49:44.580411 datalad_crawler-1.0.1/datalad_crawler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-05-25 17:49:44.000000 datalad_crawler-1.0.1/datalad_crawler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-05-25 17:49:44.000000 datalad_crawler-1.0.1/datalad_crawler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 17:49:44.000000 datalad_crawler-1.0.1/datalad_crawler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-25 17:49:44.000000 datalad_crawler-1.0.1/datalad_crawler.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-25 17:49:44.000000 datalad_crawler-1.0.1/datalad_crawler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-25 17:49:44.000000 datalad_crawler-1.0.1/datalad_crawler.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10447 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/formatters.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 17:49:44.588412 datalad_crawler-1.0.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2482 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-05-25 17:49:27.000000 datalad_crawler-1.0.1/setup_support.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `datalad_crawler-0.9.9/formatters.py` & `datalad_crawler-1.0.1/formatters.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,15 @@
     def _mk_title(self, prog):
         name_version = "\"{0} {1}\"".format(prog, self._version)
         return '.TH {0} {1} {2} {3}\n'.format(prog, self._section,
                                               self._today, name_version)
 
     def _make_name(self, parser):
         """
-        this method is in consitent with others ... it relies on
+        this method is in consistent with others ... it relies on
         distribution
         """
         return '.SH NAME\n%s \\- %s\n' % (parser.prog,
                                           parser.description)
 
     def _mk_description(self, parser):
         desc = parser.description
```

### Comparing `datalad_crawler-0.9.9/setup_support.py` & `datalad_crawler-1.0.1/setup_support.py`

 * *Files identical despite different names*

### Comparing `datalad_crawler-0.9.9/README.md` & `datalad_crawler-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `datalad_crawler-0.9.9/datalad_crawler/dbs/versions.py` & `datalad_crawler-1.0.1/datalad_crawler/dbs/versions.py`

 * *Files identical despite different names*

### Comparing `datalad_crawler-0.9.9/datalad_crawler/dbs/files.py` & `datalad_crawler-1.0.1/datalad_crawler/dbs/files.py`

 * *Files identical despite different names*

### Comparing `datalad_crawler-0.9.9/datalad_crawler/dbs/base.py` & `datalad_crawler-1.0.1/datalad_crawler/dbs/base.py`

 * *Files identical despite different names*

### Comparing `datalad_crawler-0.9.9/datalad_crawler/dbs/tests/test_files.py` & `datalad_crawler-1.0.1/datalad_crawler/dbs/tests/test_files.py`

 * *Files identical despite different names*

### Comparing `datalad_crawler-0.9.9/datalad_crawler/crawl.py` & `datalad_crawler-1.0.1/datalad_crawler/crawl.py`

 * *Files identical despite different names*

### Comparing `datalad_crawler-0.9.9/datalad_crawler/consts.py` & `datalad_crawler-1.0.1/datalad_crawler/consts.py`

 * *Files identical despite different names*

### Comparing `datalad_crawler-0.9.9/datalad_crawler/utils.py` & `datalad_crawler-1.0.1/datalad_crawler/utils.py`

 * *Files identical despite different names*

### Comparing `datalad_crawler-0.9.9/datalad_crawler/pipelines/crcns.py` & `datalad_crawler-1.0.1/datalad_crawler/pipelines/crcns.py`

 * *Files identical despite different names*

### Comparing `datalad_crawler-0.9.9/datalad_crawler/pipelines/stanford_lib.py` & `datalad_crawler-1.0.1/datalad_crawler/pipelines/stanford_lib.py`

 * *Files identical despite different names*

### Comparing `datalad_crawler-0.9.9/datalad_crawler/pipelines/fcptable.py` & `datalad_crawler-1.0.1/datalad_crawler/pipelines/fcptable.py`

 * *Files 0% similar despite different names*

```diff
@@ -137,15 +137,15 @@
                     extract_readme,
                     annex,
                 ],
                 a_href_match('.*'),
                 switch(
                     'url',
                     {
-                        # e.g. for Cleveland CCF -- we need to crawl one of thos pages
+                        # e.g. for Cleveland CCF -- we need to crawl one of those pages
                         '(http://fcon_1000.projects.nitrc.org/indi/'
                         # or it might lead to the nitrc project page
                         '|http://www.nitrc.org/projects/'
                         '|http://www.nitrc.org/frs/downloadlink.php/1635$)':
                             [
                                 {'output': 'outputs'},
                                 crawl_url(matchers=[a_href_match(r'http://www.nitrc.org/frs/\?group_id=[0-9]+$')]),
```

### Comparing `datalad_crawler-0.9.9/datalad_crawler/pipelines/openfmri_s3.py` & `datalad_crawler-1.0.1/datalad_crawler/pipelines/openfmri_s3.py`

 * *Files identical despite different names*

### Comparing `datalad_crawler-0.9.9/datalad_crawler/pipelines/xnat.py` & `datalad_crawler-1.0.1/datalad_crawler/pipelines/xnat.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,15 +130,15 @@
         limit: {'public', 'protected', 'private', None} or list of thereof
            'private' -- projects you have no any access to. 'protected' -- you could
            fetch description but not the data. None - would list all the projects
 
         drop_empty: bool
           whether to drop projects with no experiments.  Implies
           limit = 'public' since we need access to projects to determine if they
-          are empty.  If drop_empty is set nd limit is None, limit is set to
+          are empty.  If drop_empty is set and limit is None, limit is set to
           'public'
         """
 
         limit = assure_list(limit)
 
         if drop_empty:
             # TODO: rework this logic/restriction
```

### Comparing `datalad_crawler-0.9.9/datalad_crawler/pipelines/simple_s3.py` & `datalad_crawler-1.0.1/datalad_crawler/pipelines/simple_s3.py`

 * *Files identical despite different names*

### Comparing `datalad_crawler-0.9.9/datalad_crawler/pipelines/balsa.py` & `datalad_crawler-1.0.1/datalad_crawler/pipelines/balsa.py`

 * *Files identical despite different names*

### Comparing `datalad_crawler-0.9.9/datalad_crawler/pipelines/nda.py` & `datalad_crawler-1.0.1/datalad_crawler/pipelines/nda.py`

 * *Files identical despite different names*

### Comparing `datalad_crawler-0.9.9/datalad_crawler/pipelines/openfmri.py` & `datalad_crawler-1.0.1/datalad_crawler/pipelines/openfmri.py`

 * *Files identical despite different names*

### Comparing `datalad_crawler-0.9.9/datalad_crawler/pipelines/gh.py` & `datalad_crawler-1.0.1/datalad_crawler/pipelines/gh.py`

 * *Files identical despite different names*

### Comparing `datalad_crawler-0.9.9/datalad_crawler/pipelines/simple_with_archives.py` & `datalad_crawler-1.0.1/datalad_crawler/pipelines/simple_with_archives.py`

 * *Files identical despite different names*

### Comparing `datalad_crawler-0.9.9/datalad_crawler/pipelines/tests/test_utils.py` & `datalad_crawler-1.0.1/datalad_crawler/pipelines/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `datalad_crawler-0.9.9/datalad_crawler/pipelines/tests/test_gh.py` & `datalad_crawler-1.0.1/datalad_crawler/pipelines/tests/test_gh.py`

 * *Files identical despite different names*

### Comparing `datalad_crawler-0.9.9/datalad_crawler/pipelines/tests/test_simple_s3.py` & `datalad_crawler-1.0.1/datalad_crawler/pipelines/tests/test_simple_s3.py`

 * *Files identical despite different names*

### Comparing `datalad_crawler-0.9.9/datalad_crawler/pipelines/tests/test_openfmri_collection.py` & `datalad_crawler-1.0.1/datalad_crawler/pipelines/tests/test_openfmri_collection.py`

 * *Files identical despite different names*

### Comparing `datalad_crawler-0.9.9/datalad_crawler/pipelines/tests/test_balsa.py` & `datalad_crawler-1.0.1/datalad_crawler/pipelines/tests/test_balsa.py`

 * *Files identical despite different names*

### Comparing `datalad_crawler-0.9.9/datalad_crawler/pipelines/tests/test_nda.py` & `datalad_crawler-1.0.1/datalad_crawler/pipelines/tests/test_nda.py`

 * *Files identical despite different names*

### Comparing `datalad_crawler-0.9.9/datalad_crawler/pipelines/tests/test_crcns.py` & `datalad_crawler-1.0.1/datalad_crawler/pipelines/tests/test_crcns.py`

 * *Files identical despite different names*

### Comparing `datalad_crawler-0.9.9/datalad_crawler/pipelines/tests/test_xnat.py` & `datalad_crawler-1.0.1/datalad_crawler/pipelines/tests/test_xnat.py`

 * *Files identical despite different names*

### Comparing `datalad_crawler-0.9.9/datalad_crawler/pipelines/tests/test_openfmri.py` & `datalad_crawler-1.0.1/datalad_crawler/pipelines/tests/test_openfmri.py`

 * *Files identical despite different names*

### Comparing `datalad_crawler-0.9.9/datalad_crawler/pipelines/tests/test_simple_with_archives.py` & `datalad_crawler-1.0.1/datalad_crawler/pipelines/tests/test_simple_with_archives.py`

 * *Files identical despite different names*

### Comparing `datalad_crawler-0.9.9/datalad_crawler/pipelines/tests/test_fcptable.py` & `datalad_crawler-1.0.1/datalad_crawler/pipelines/tests/test_fcptable.py`

 * *Files identical despite different names*

### Comparing `datalad_crawler-0.9.9/datalad_crawler/pipelines/template.py` & `datalad_crawler-1.0.1/datalad_crawler/pipelines/template.py`

 * *Files identical despite different names*

### Comparing `datalad_crawler-0.9.9/datalad_crawler/pipelines/abstractsonline.py` & `datalad_crawler-1.0.1/datalad_crawler/pipelines/abstractsonline.py`

 * *Files identical despite different names*

### Comparing `datalad_crawler-0.9.9/datalad_crawler/nodes/annex.py` & `datalad_crawler-1.0.1/datalad_crawler/nodes/annex.py`

 * *Files identical despite different names*

### Comparing `datalad_crawler-0.9.9/datalad_crawler/nodes/crawl_url.py` & `datalad_crawler-1.0.1/datalad_crawler/nodes/crawl_url.py`

 * *Files identical despite different names*

### Comparing `datalad_crawler-0.9.9/datalad_crawler/nodes/s3.py` & `datalad_crawler-1.0.1/datalad_crawler/nodes/s3.py`

 * *Files 0% similar despite different names*

```diff
@@ -262,15 +262,15 @@
                     # Since git doesn't care about empty directories for us makes sense only
                     # in the case when DeleteMarker is not pointing to the subdirectory
                     # and not empty (if original directory was removed)
                     if filename and not filename.endswith('/'):
                         yield updated(data, {'filename': filename, 'datalad_action': 'remove'})
                     else:
                         # Situation there is much trickier since it seems that "directory"
-                        # could also be a key itself and created/removed which somewhat interfers with
+                        # could also be a key itself and created/removed which somewhat interferes with
                         # all our logic here
                         # For an interesting example see
                         #  s3://openneuro/ds000217/ds000217_R1.0.0/compressed
                         lgr.info("Ignoring DeleteMarker for %s", filename)
 
                 update_versiondb(e)
             elif isinstance(e, Prefix):
```

### Comparing `datalad_crawler-0.9.9/datalad_crawler/nodes/matches.py` & `datalad_crawler-1.0.1/datalad_crawler/nodes/matches.py`

 * *Files identical despite different names*

### Comparing `datalad_crawler-0.9.9/datalad_crawler/nodes/tests/test_matches.py` & `datalad_crawler-1.0.1/datalad_crawler/nodes/tests/test_matches.py`

 * *Files identical despite different names*

### Comparing `datalad_crawler-0.9.9/datalad_crawler/nodes/tests/test_crawl_url.py` & `datalad_crawler-1.0.1/datalad_crawler/nodes/tests/test_crawl_url.py`

 * *Files identical despite different names*

### Comparing `datalad_crawler-0.9.9/datalad_crawler/nodes/tests/test_annex.py` & `datalad_crawler-1.0.1/datalad_crawler/nodes/tests/test_annex.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,17 +52,17 @@
     eq_(sorted(listdir(outdir)), sorted(['.myfile', '.git']))
 
 
 @with_tempfile(mkdir=True)
 @with_tempfile()
 def test_initiate_dataset(path=None, path2=None):
     dataset_path = opj(path, 'test')
-    datas = list(initiate_dataset('template', 'testdataset', path=dataset_path)())
-    assert_equal(len(datas), 1)
-    data = datas[0]
+    data = list(initiate_dataset('template', 'testdataset', path=dataset_path)())
+    assert_equal(len(data), 1)
+    data = data[0]
     eq_(data['dataset_path'], dataset_path)
     crawl_cfg = opj(dataset_path, CRAWLER_META_CONFIG_PATH)
     ok_(exists, crawl_cfg)
     pipeline = load_pipeline_from_config(crawl_cfg)
 
     # by default we should initiate to MD5E backend
     fname = 'test.dat'
```

### Comparing `datalad_crawler-0.9.9/datalad_crawler/nodes/tests/test_misc.py` & `datalad_crawler-1.0.1/datalad_crawler/nodes/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `datalad_crawler-0.9.9/datalad_crawler/nodes/tests/test_s3.py` & `datalad_crawler-1.0.1/datalad_crawler/nodes/tests/test_s3.py`

 * *Files identical despite different names*

### Comparing `datalad_crawler-0.9.9/datalad_crawler/nodes/misc.py` & `datalad_crawler-1.0.1/datalad_crawler/nodes/misc.py`

 * *Files identical despite different names*

### Comparing `datalad_crawler-0.9.9/datalad_crawler/nodes/__init__.py` & `datalad_crawler-1.0.1/datalad_crawler/nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `datalad_crawler-0.9.9/datalad_crawler/support/versions.py` & `datalad_crawler-1.0.1/datalad_crawler/support/versions.py`

 * *Files identical despite different names*

### Comparing `datalad_crawler-0.9.9/datalad_crawler/support/tests/test_versions.py` & `datalad_crawler-1.0.1/datalad_crawler/support/tests/test_versions.py`

 * *Files identical despite different names*

### Comparing `datalad_crawler-0.9.9/datalad_crawler/crawl_init.py` & `datalad_crawler-1.0.1/datalad_crawler/crawl_init.py`

 * *Files identical despite different names*

### Comparing `datalad_crawler-0.9.9/datalad_crawler/tests/test_utils.py` & `datalad_crawler-1.0.1/datalad_crawler/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `datalad_crawler-0.9.9/datalad_crawler/tests/test_crawl.py` & `datalad_crawler-1.0.1/datalad_crawler/tests/test_crawl.py`

 * *Files identical despite different names*

### Comparing `datalad_crawler-0.9.9/datalad_crawler/tests/test_crawl_init.py` & `datalad_crawler-1.0.1/datalad_crawler/tests/test_crawl_init.py`

 * *Files identical despite different names*

### Comparing `datalad_crawler-0.9.9/datalad_crawler/tests/test_pipeline.py` & `datalad_crawler-1.0.1/datalad_crawler/tests/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `datalad_crawler-0.9.9/datalad_crawler/tests/__init__.py` & `datalad_crawler-1.0.1/datalad_crawler/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `datalad_crawler-0.9.9/datalad_crawler/pipeline.py` & `datalad_crawler-1.0.1/datalad_crawler/pipeline.py`

 * *Files identical despite different names*

### Comparing `datalad_crawler-0.9.9/datalad_crawler/__init__.py` & `datalad_crawler-1.0.1/datalad_crawler/__init__.py`

 * *Files identical despite different names*

### Comparing `datalad_crawler-0.9.9/setup.py` & `datalad_crawler-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `datalad_crawler-0.9.9/datalad_crawler.egg-info/SOURCES.txt` & `datalad_crawler-1.0.1/datalad_crawler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datalad_crawler-0.9.9/datalad_crawler.egg-info/PKG-INFO` & `datalad_crawler-1.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 Metadata-Version: 2.1
-Name: datalad-crawler
-Version: 0.9.9
+Name: datalad_crawler
+Version: 1.0.1
 Summary: DataLad extension package for crawling external web resources into an automated data distribution
-Home-page: UNKNOWN
 Author: The DataLad Team and Contributors
 Author-email: team@datalad.org
-License: UNKNOWN
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 Provides-Extra: core
 Provides-Extra: devel-docs
 Provides-Extra: tests
 Provides-Extra: devel
 License-File: COPYING
 
@@ -72,9 +69,7 @@
 deployment logistics into a federated 'data distribution'" (Halchenko/Hanke),
 co-funded by the US National Science Foundation (NSF 1429999) and the German
 Federal Ministry of Education and Research (BMBF 01GQ1411). Additional support
 is provided by the German federal state of Saxony-Anhalt and the European
 Regional Development Fund (ERDF), Project: Center for Behavioral Brain
 Sciences, Imaging Platform.  This work is further facilitated by the ReproNim
 project (NIH 1P41EB019936-01A1).
-
-
```

### Comparing `datalad_crawler-0.9.9/COPYING` & `datalad_crawler-1.0.1/COPYING`

 * *Files identical despite different names*

### Comparing `datalad_crawler-0.9.9/PKG-INFO` & `datalad_crawler-1.0.1/datalad_crawler.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 Metadata-Version: 2.1
-Name: datalad_crawler
-Version: 0.9.9
+Name: datalad-crawler
+Version: 1.0.1
 Summary: DataLad extension package for crawling external web resources into an automated data distribution
-Home-page: UNKNOWN
 Author: The DataLad Team and Contributors
 Author-email: team@datalad.org
-License: UNKNOWN
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 Provides-Extra: core
 Provides-Extra: devel-docs
 Provides-Extra: tests
 Provides-Extra: devel
 License-File: COPYING
 
@@ -72,9 +69,7 @@
 deployment logistics into a federated 'data distribution'" (Halchenko/Hanke),
 co-funded by the US National Science Foundation (NSF 1429999) and the German
 Federal Ministry of Education and Research (BMBF 01GQ1411). Additional support
 is provided by the German federal state of Saxony-Anhalt and the European
 Regional Development Fund (ERDF), Project: Center for Behavioral Brain
 Sciences, Imaging Platform.  This work is further facilitated by the ReproNim
 project (NIH 1P41EB019936-01A1).
-
-
```

