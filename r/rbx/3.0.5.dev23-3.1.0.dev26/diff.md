# Comparing `tmp/rbx-3.0.5.dev23.tar.gz` & `tmp/rbx-3.1.0.dev26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rbx-3.0.5.dev23.tar", last modified: Wed Apr 26 06:37:26 2023, max compression
+gzip compressed data, was "rbx-3.1.0.dev26.tar", last modified: Thu May 25 11:59:24 2023, max compression
```

## Comparing `rbx-3.0.5.dev23.tar` & `rbx-3.1.0.dev26.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:37:26.787090 rbx-3.0.5.dev23/
--rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-04-26 06:37:11.000000 rbx-3.0.5.dev23/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-04-26 06:37:26.787090 rbx-3.0.5.dev23/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-26 06:37:11.000000 rbx-3.0.5.dev23/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:37:26.783090 rbx-3.0.5.dev23/rbx/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 06:37:11.000000 rbx-3.0.5.dev23/rbx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:37:26.783090 rbx-3.0.5.dev23/rbx/auth/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-26 06:37:11.000000 rbx-3.0.5.dev23/rbx/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-04-26 06:37:11.000000 rbx-3.0.5.dev23/rbx/auth/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     5172 2023-04-26 06:37:11.000000 rbx-3.0.5.dev23/rbx/auth/keystore.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:37:26.783090 rbx-3.0.5.dev23/rbx/aws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 06:37:11.000000 rbx-3.0.5.dev23/rbx/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5656 2023-04-26 06:37:11.000000 rbx-3.0.5.dev23/rbx/aws/s3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:37:26.783090 rbx-3.0.5.dev23/rbx/buildtools/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-26 06:37:11.000000 rbx-3.0.5.dev23/rbx/buildtools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-26 06:37:25.000000 rbx-3.0.5.dev23/rbx/buildtools/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:37:26.783090 rbx-3.0.5.dev23/rbx/buildtools/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-26 06:37:11.000000 rbx-3.0.5.dev23/rbx/buildtools/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-04-26 06:37:11.000000 rbx-3.0.5.dev23/rbx/buildtools/tasks/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-04-26 06:37:11.000000 rbx-3.0.5.dev23/rbx/buildtools/tasks/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-04-26 06:37:11.000000 rbx-3.0.5.dev23/rbx/buildtools/tasks/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-04-26 06:37:11.000000 rbx-3.0.5.dev23/rbx/buildtools/tasks/pypi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:37:26.783090 rbx-3.0.5.dev23/rbx/clients/
--rw-r--r--   0 runner    (1001) docker     (123)     8013 2023-04-26 06:37:11.000000 rbx-3.0.5.dev23/rbx/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7171 2023-04-26 06:37:11.000000 rbx-3.0.5.dev23/rbx/clients/adsquare.py
--rw-r--r--   0 runner    (1001) docker     (123)    10486 2023-04-26 06:37:11.000000 rbx-3.0.5.dev23/rbx/clients/broadsign.py
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-04-26 06:37:11.000000 rbx-3.0.5.dev23/rbx/clients/oxr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-04-26 06:37:11.000000 rbx-3.0.5.dev23/rbx/clients/panels.py
--rw-r--r--   0 runner    (1001) docker     (123)     6386 2023-04-26 06:37:11.000000 rbx-3.0.5.dev23/rbx/clients/reporting.py
--rw-r--r--   0 runner    (1001) docker     (123)     7884 2023-04-26 06:37:11.000000 rbx-3.0.5.dev23/rbx/clients/retry.py
--rw-r--r--   0 runner    (1001) docker     (123)     5817 2023-04-26 06:37:11.000000 rbx-3.0.5.dev23/rbx/clients/uslicer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-04-26 06:37:11.000000 rbx-3.0.5.dev23/rbx/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:37:26.783090 rbx-3.0.5.dev23/rbx/gcp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 06:37:11.000000 rbx-3.0.5.dev23/rbx/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-04-26 06:37:11.000000 rbx-3.0.5.dev23/rbx/gcp/cloud_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-04-26 06:37:11.000000 rbx-3.0.5.dev23/rbx/gcp/pubsub.py
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-04-26 06:37:11.000000 rbx-3.0.5.dev23/rbx/gcp/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:37:26.787090 rbx-3.0.5.dev23/rbx/geo/
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-04-26 06:37:11.000000 rbx-3.0.5.dev23/rbx/geo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-04-26 06:37:11.000000 rbx-3.0.5.dev23/rbx/geo/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-04-26 06:37:11.000000 rbx-3.0.5.dev23/rbx/geo/maps.py
--rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-04-26 06:37:11.000000 rbx-3.0.5.dev23/rbx/geo/packer.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-26 06:37:11.000000 rbx-3.0.5.dev23/rbx/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:37:26.787090 rbx-3.0.5.dev23/rbx/manifest/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 06:37:11.000000 rbx-3.0.5.dev23/rbx/manifest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-04-26 06:37:11.000000 rbx-3.0.5.dev23/rbx/manifest/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    18854 2023-04-26 06:37:11.000000 rbx-3.0.5.dev23/rbx/manifest/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-04-26 06:37:11.000000 rbx-3.0.5.dev23/rbx/manifest/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:37:26.787090 rbx-3.0.5.dev23/rbx/queues/
--rw-r--r--   0 runner    (1001) docker     (123)    11448 2023-04-26 06:37:11.000000 rbx-3.0.5.dev23/rbx/queues/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-04-26 06:37:11.000000 rbx-3.0.5.dev23/rbx/queues/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-04-26 06:37:11.000000 rbx-3.0.5.dev23/rbx/queues/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-04-26 06:37:11.000000 rbx-3.0.5.dev23/rbx/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:37:26.787090 rbx-3.0.5.dev23/rbx/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-04-26 06:37:11.000000 rbx-3.0.5.dev23/rbx/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-26 06:37:11.000000 rbx-3.0.5.dev23/rbx/utils/mdm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:37:26.787090 rbx-3.0.5.dev23/rbx/web/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 06:37:11.000000 rbx-3.0.5.dev23/rbx/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-04-26 06:37:11.000000 rbx-3.0.5.dev23/rbx/web/handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:37:26.783090 rbx-3.0.5.dev23/rbx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-04-26 06:37:26.000000 rbx-3.0.5.dev23/rbx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-04-26 06:37:26.000000 rbx-3.0.5.dev23/rbx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 06:37:26.000000 rbx-3.0.5.dev23/rbx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-26 06:37:26.000000 rbx-3.0.5.dev23/rbx.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-04-26 06:37:26.000000 rbx-3.0.5.dev23/rbx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-26 06:37:26.000000 rbx-3.0.5.dev23/rbx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 06:37:26.787090 rbx-3.0.5.dev23/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-04-26 06:37:25.000000 rbx-3.0.5.dev23/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:59:24.507608 rbx-3.1.0.dev26/
+-rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-05-25 11:59:11.000000 rbx-3.1.0.dev26/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-25 11:59:24.507608 rbx-3.1.0.dev26/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-25 11:59:11.000000 rbx-3.1.0.dev26/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:59:24.503608 rbx-3.1.0.dev26/rbx/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 11:59:11.000000 rbx-3.1.0.dev26/rbx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:59:24.503608 rbx-3.1.0.dev26/rbx/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-25 11:59:11.000000 rbx-3.1.0.dev26/rbx/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-05-25 11:59:11.000000 rbx-3.1.0.dev26/rbx/auth/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5172 2023-05-25 11:59:11.000000 rbx-3.1.0.dev26/rbx/auth/keystore.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:59:24.503608 rbx-3.1.0.dev26/rbx/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 11:59:11.000000 rbx-3.1.0.dev26/rbx/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5656 2023-05-25 11:59:11.000000 rbx-3.1.0.dev26/rbx/aws/s3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:59:24.503608 rbx-3.1.0.dev26/rbx/buildtools/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-25 11:59:11.000000 rbx-3.1.0.dev26/rbx/buildtools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-25 11:59:24.000000 rbx-3.1.0.dev26/rbx/buildtools/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:59:24.503608 rbx-3.1.0.dev26/rbx/buildtools/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-25 11:59:11.000000 rbx-3.1.0.dev26/rbx/buildtools/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-05-25 11:59:11.000000 rbx-3.1.0.dev26/rbx/buildtools/tasks/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-05-25 11:59:11.000000 rbx-3.1.0.dev26/rbx/buildtools/tasks/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-25 11:59:11.000000 rbx-3.1.0.dev26/rbx/buildtools/tasks/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-25 11:59:11.000000 rbx-3.1.0.dev26/rbx/buildtools/tasks/pypi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:59:24.507608 rbx-3.1.0.dev26/rbx/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)     8013 2023-05-25 11:59:11.000000 rbx-3.1.0.dev26/rbx/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7171 2023-05-25 11:59:11.000000 rbx-3.1.0.dev26/rbx/clients/adsquare.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10486 2023-05-25 11:59:11.000000 rbx-3.1.0.dev26/rbx/clients/broadsign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-05-25 11:59:11.000000 rbx-3.1.0.dev26/rbx/clients/oxr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-05-25 11:59:11.000000 rbx-3.1.0.dev26/rbx/clients/panels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6646 2023-05-25 11:59:11.000000 rbx-3.1.0.dev26/rbx/clients/reporting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7884 2023-05-25 11:59:11.000000 rbx-3.1.0.dev26/rbx/clients/retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5817 2023-05-25 11:59:11.000000 rbx-3.1.0.dev26/rbx/clients/uslicer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-05-25 11:59:11.000000 rbx-3.1.0.dev26/rbx/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:59:24.507608 rbx-3.1.0.dev26/rbx/gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 11:59:11.000000 rbx-3.1.0.dev26/rbx/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-05-25 11:59:11.000000 rbx-3.1.0.dev26/rbx/gcp/cloud_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-05-25 11:59:11.000000 rbx-3.1.0.dev26/rbx/gcp/pubsub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-05-25 11:59:11.000000 rbx-3.1.0.dev26/rbx/gcp/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:59:24.507608 rbx-3.1.0.dev26/rbx/geo/
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-05-25 11:59:11.000000 rbx-3.1.0.dev26/rbx/geo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-05-25 11:59:11.000000 rbx-3.1.0.dev26/rbx/geo/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-05-25 11:59:11.000000 rbx-3.1.0.dev26/rbx/geo/maps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-05-25 11:59:11.000000 rbx-3.1.0.dev26/rbx/geo/packer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-25 11:59:11.000000 rbx-3.1.0.dev26/rbx/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:59:24.507608 rbx-3.1.0.dev26/rbx/manifest/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 11:59:11.000000 rbx-3.1.0.dev26/rbx/manifest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-05-25 11:59:11.000000 rbx-3.1.0.dev26/rbx/manifest/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18854 2023-05-25 11:59:11.000000 rbx-3.1.0.dev26/rbx/manifest/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-05-25 11:59:11.000000 rbx-3.1.0.dev26/rbx/manifest/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:59:24.507608 rbx-3.1.0.dev26/rbx/queues/
+-rw-r--r--   0 runner    (1001) docker     (123)    11448 2023-05-25 11:59:11.000000 rbx-3.1.0.dev26/rbx/queues/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-05-25 11:59:11.000000 rbx-3.1.0.dev26/rbx/queues/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-05-25 11:59:11.000000 rbx-3.1.0.dev26/rbx/queues/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-25 11:59:11.000000 rbx-3.1.0.dev26/rbx/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:59:24.507608 rbx-3.1.0.dev26/rbx/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-05-25 11:59:11.000000 rbx-3.1.0.dev26/rbx/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-25 11:59:11.000000 rbx-3.1.0.dev26/rbx/utils/mdm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:59:24.507608 rbx-3.1.0.dev26/rbx/web/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 11:59:11.000000 rbx-3.1.0.dev26/rbx/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-05-25 11:59:11.000000 rbx-3.1.0.dev26/rbx/web/handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:59:24.503608 rbx-3.1.0.dev26/rbx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-25 11:59:24.000000 rbx-3.1.0.dev26/rbx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-25 11:59:24.000000 rbx-3.1.0.dev26/rbx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 11:59:24.000000 rbx-3.1.0.dev26/rbx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-25 11:59:24.000000 rbx-3.1.0.dev26/rbx.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-05-25 11:59:24.000000 rbx-3.1.0.dev26/rbx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-25 11:59:24.000000 rbx-3.1.0.dev26/rbx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 11:59:24.507608 rbx-3.1.0.dev26/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-05-25 11:59:24.000000 rbx-3.1.0.dev26/setup.py
```

### Comparing `rbx-3.0.5.dev23/LICENSE` & `rbx-3.1.0.dev26/LICENSE`

 * *Files identical despite different names*

### Comparing `rbx-3.0.5.dev23/PKG-INFO` & `rbx-3.1.0.dev26/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rbx
-Version: 3.0.5.dev23
+Version: 3.1.0.dev26
 Summary: Scoota Platform utilities
 Home-page: http://scoota.com/
 Author: The Scoota Engineering Team
 Author-email: engineering@scoota.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `rbx-3.0.5.dev23/rbx/auth/decorators.py` & `rbx-3.1.0.dev26/rbx/auth/decorators.py`

 * *Files identical despite different names*

### Comparing `rbx-3.0.5.dev23/rbx/auth/keystore.py` & `rbx-3.1.0.dev26/rbx/auth/keystore.py`

 * *Files identical despite different names*

### Comparing `rbx-3.0.5.dev23/rbx/aws/s3.py` & `rbx-3.1.0.dev26/rbx/aws/s3.py`

 * *Files identical despite different names*

### Comparing `rbx-3.0.5.dev23/rbx/buildtools/tasks/deploy.py` & `rbx-3.1.0.dev26/rbx/buildtools/tasks/deploy.py`

 * *Files identical despite different names*

### Comparing `rbx-3.0.5.dev23/rbx/buildtools/tasks/image.py` & `rbx-3.1.0.dev26/rbx/buildtools/tasks/image.py`

 * *Files identical despite different names*

### Comparing `rbx-3.0.5.dev23/rbx/buildtools/tasks/misc.py` & `rbx-3.1.0.dev26/rbx/buildtools/tasks/misc.py`

 * *Files identical despite different names*

### Comparing `rbx-3.0.5.dev23/rbx/clients/__init__.py` & `rbx-3.1.0.dev26/rbx/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `rbx-3.0.5.dev23/rbx/clients/adsquare.py` & `rbx-3.1.0.dev26/rbx/clients/adsquare.py`

 * *Files identical despite different names*

### Comparing `rbx-3.0.5.dev23/rbx/clients/broadsign.py` & `rbx-3.1.0.dev26/rbx/clients/broadsign.py`

 * *Files identical despite different names*

### Comparing `rbx-3.0.5.dev23/rbx/clients/oxr.py` & `rbx-3.1.0.dev26/rbx/clients/oxr.py`

 * *Files identical despite different names*

### Comparing `rbx-3.0.5.dev23/rbx/clients/panels.py` & `rbx-3.1.0.dev26/rbx/clients/panels.py`

 * *Files identical despite different names*

### Comparing `rbx-3.0.5.dev23/rbx/clients/reporting.py` & `rbx-3.1.0.dev26/rbx/clients/reporting.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,31 +14,44 @@
         self.token = token
 
     @property
     def auth(self):
         """The Reporting Service uses Digest Authentication."""
         return HttpAuth(self.token, key="X-RBX-TOKEN")
 
-    def create_schedule(self, body, campaign, cron, format, name, recipients, reports):
+    def create_schedule(
+        self,
+        body,
+        campaign,
+        cron,
+        format,
+        name,
+        recipients,
+        reports,
+        api_version=None,
+    ):
         """Create a scheduled job.
 
         Return the job_id of the job just created.
         """
-        response = self._post(
-            "/schedule",
-            data={
-                "body": body,
-                "campaign": campaign,
-                "cron": cron,
-                "format": format,
-                "name": name,
-                "recipients": recipients,
-                "reports": reports,
-            },
-        )
+        data = {
+            "body": body,
+            "campaign": campaign,
+            "cron": cron,
+            "format": format,
+            "name": name,
+            "recipients": recipients,
+            "reports": reports,
+        }
+
+        if api_version is not None:
+            data["api_version"] = api_version
+
+        response = self._post("/schedule", data=data)
+
         return response.get("job_id")
 
     def delete_schedule(self, job_id):
         """Create the scheduled job."""
         response = self._post("/schedule/delete", data={"job_id": job_id})
         return response.get("job_id")
 
@@ -49,30 +62,42 @@
 
     def resume_schedule(self, job_id):
         """Resume the scheduled job."""
         response = self._post("/schedule/resume", data={"job_id": job_id})
         return response.get("job_id")
 
     def update_schedule(
-        self, body, campaign, cron, format, job_id, name, recipients, reports
+        self,
+        body,
+        campaign,
+        cron,
+        format,
+        job_id,
+        name,
+        recipients,
+        reports,
+        api_version=None,
     ):
         """Update the scheduled job."""
-        response = self._post(
-            "/schedule",
-            data={
-                "body": body,
-                "campaign": campaign,
-                "cron": cron,
-                "format": format,
-                "job_id": job_id,
-                "name": name,
-                "recipients": recipients,
-                "reports": reports,
-            },
-        )
+        data = {
+            "body": body,
+            "campaign": campaign,
+            "cron": cron,
+            "format": format,
+            "job_id": job_id,
+            "name": name,
+            "recipients": recipients,
+            "reports": reports,
+        }
+
+        if api_version is not None:
+            data["api_version"] = api_version
+
+        response = self._post("/schedule", data=data)
+
         return response.get("job_id")
 
     def get_report(
         self,
         breakdowns,
         metrics=None,
         custom_metrics=None,
```

### Comparing `rbx-3.0.5.dev23/rbx/clients/retry.py` & `rbx-3.1.0.dev26/rbx/clients/retry.py`

 * *Files identical despite different names*

### Comparing `rbx-3.0.5.dev23/rbx/clients/uslicer.py` & `rbx-3.1.0.dev26/rbx/clients/uslicer.py`

 * *Files identical despite different names*

### Comparing `rbx-3.0.5.dev23/rbx/exceptions.py` & `rbx-3.1.0.dev26/rbx/exceptions.py`

 * *Files identical despite different names*

### Comparing `rbx-3.0.5.dev23/rbx/gcp/cloud_tasks.py` & `rbx-3.1.0.dev26/rbx/gcp/cloud_tasks.py`

 * *Files identical despite different names*

### Comparing `rbx-3.0.5.dev23/rbx/gcp/pubsub.py` & `rbx-3.1.0.dev26/rbx/gcp/pubsub.py`

 * *Files identical despite different names*

### Comparing `rbx-3.0.5.dev23/rbx/gcp/storage.py` & `rbx-3.1.0.dev26/rbx/gcp/storage.py`

 * *Files identical despite different names*

### Comparing `rbx-3.0.5.dev23/rbx/geo/__init__.py` & `rbx-3.1.0.dev26/rbx/geo/__init__.py`

 * *Files identical despite different names*

### Comparing `rbx-3.0.5.dev23/rbx/geo/cli.py` & `rbx-3.1.0.dev26/rbx/geo/cli.py`

 * *Files identical despite different names*

### Comparing `rbx-3.0.5.dev23/rbx/geo/maps.py` & `rbx-3.1.0.dev26/rbx/geo/maps.py`

 * *Files identical despite different names*

### Comparing `rbx-3.0.5.dev23/rbx/geo/packer.py` & `rbx-3.1.0.dev26/rbx/geo/packer.py`

 * *Files identical despite different names*

### Comparing `rbx-3.0.5.dev23/rbx/logging.py` & `rbx-3.1.0.dev26/rbx/logging.py`

 * *Files identical despite different names*

### Comparing `rbx-3.0.5.dev23/rbx/manifest/cli.py` & `rbx-3.1.0.dev26/rbx/manifest/cli.py`

 * *Files identical despite different names*

### Comparing `rbx-3.0.5.dev23/rbx/manifest/processor.py` & `rbx-3.1.0.dev26/rbx/manifest/processor.py`

 * *Files identical despite different names*

### Comparing `rbx-3.0.5.dev23/rbx/manifest/utils.py` & `rbx-3.1.0.dev26/rbx/manifest/utils.py`

 * *Files identical despite different names*

### Comparing `rbx-3.0.5.dev23/rbx/queues/__init__.py` & `rbx-3.1.0.dev26/rbx/queues/__init__.py`

 * *Files identical despite different names*

### Comparing `rbx-3.0.5.dev23/rbx/queues/jobs.py` & `rbx-3.1.0.dev26/rbx/queues/jobs.py`

 * *Files identical despite different names*

### Comparing `rbx-3.0.5.dev23/rbx/queues/scheduler.py` & `rbx-3.1.0.dev26/rbx/queues/scheduler.py`

 * *Files identical despite different names*

### Comparing `rbx-3.0.5.dev23/rbx/utils/__init__.py` & `rbx-3.1.0.dev26/rbx/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `rbx-3.0.5.dev23/rbx/web/handlers.py` & `rbx-3.1.0.dev26/rbx/web/handlers.py`

 * *Files identical despite different names*

### Comparing `rbx-3.0.5.dev23/rbx.egg-info/PKG-INFO` & `rbx-3.1.0.dev26/rbx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rbx
-Version: 3.0.5.dev23
+Version: 3.1.0.dev26
 Summary: Scoota Platform utilities
 Home-page: http://scoota.com/
 Author: The Scoota Engineering Team
 Author-email: engineering@scoota.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `rbx-3.0.5.dev23/rbx.egg-info/SOURCES.txt` & `rbx-3.1.0.dev26/rbx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rbx-3.0.5.dev23/rbx.egg-info/requires.txt` & `rbx-3.1.0.dev26/rbx.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `rbx-3.0.5.dev23/setup.py` & `rbx-3.1.0.dev26/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 ]
 STORAGE = ["google-cloud-storage>=2.1,<3"]
 TASKS = ["google-cloud-tasks>=2.7,<3"]
 
 
 setup(
     name="rbx",
-    version="3.0.5.dev23",
+    version="3.1.0.dev26",
     license="Apache 2.0",
     description="Scoota Platform utilities",
     long_description="A collection of common tools for Scoota services.",
     url="http://scoota.com/",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Web Environment",
```

