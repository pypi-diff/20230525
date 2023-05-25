# Comparing `tmp/msumastro-1.2.3.tar.gz` & `tmp/msumastro-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msumastro-1.2.3.tar", last modified: Wed Nov 30 16:13:20 2022, max compression
+gzip compressed data, was "msumastro-1.2.4.tar", last modified: Thu May 25 21:36:41 2023, max compression
```

## Comparing `msumastro-1.2.3.tar` & `msumastro-1.2.4.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 mattcraig   (501) staff       (20)        0 2022-11-30 16:13:20.463204 msumastro-1.2.3/
--rw-r--r--   0 mattcraig   (501) staff       (20)       35 2019-11-17 18:02:38.000000 msumastro-1.2.3/.gitattributes
--rw-r--r--   0 mattcraig   (501) staff       (20)      187 2022-06-02 14:15:16.000000 msumastro-1.2.3/.gitignore
--rw-r--r--   0 mattcraig   (501) staff       (20)      143 2019-12-24 20:04:16.000000 msumastro-1.2.3/.readthedocs.yml
--rw-r--r--   0 mattcraig   (501) staff       (20)     1254 2019-12-28 23:51:25.000000 msumastro-1.2.3/.travis.yml
--rw-r--r--   0 mattcraig   (501) staff       (20)     1573 2019-11-17 18:02:38.000000 msumastro-1.2.3/LICENSE.rst
--rw-r--r--   0 mattcraig   (501) staff       (20)      125 2019-11-17 18:02:38.000000 msumastro-1.2.3/MANIFEST.in
--rw-r--r--   0 mattcraig   (501) staff       (20)      612 2022-11-30 16:13:20.463297 msumastro-1.2.3/PKG-INFO
--rw-r--r--   0 mattcraig   (501) staff       (20)      976 2019-12-29 00:43:53.000000 msumastro-1.2.3/README.rst
-drwxr-xr-x   0 mattcraig   (501) staff       (20)        0 2022-11-30 16:13:20.454953 msumastro-1.2.3/docs/
--rw-r--r--   0 mattcraig   (501) staff       (20)     4658 2019-11-17 18:02:38.000000 msumastro-1.2.3/docs/Makefile
-drwxr-xr-x   0 mattcraig   (501) staff       (20)        0 2022-11-30 16:13:20.450791 msumastro-1.2.3/docs/_templates/
-drwxr-xr-x   0 mattcraig   (501) staff       (20)        0 2022-11-30 16:13:20.455390 msumastro-1.2.3/docs/_templates/autosummary/
--rw-r--r--   0 mattcraig   (501) staff       (20)       42 2019-11-17 18:02:38.000000 msumastro-1.2.3/docs/_templates/autosummary/base.rst
--rw-r--r--   0 mattcraig   (501) staff       (20)       43 2019-11-17 18:02:38.000000 msumastro-1.2.3/docs/_templates/autosummary/class.rst
--rw-r--r--   0 mattcraig   (501) staff       (20)       44 2019-11-17 18:02:38.000000 msumastro-1.2.3/docs/_templates/autosummary/module.rst
--rw-r--r--   0 mattcraig   (501) staff       (20)     7761 2019-12-28 23:22:47.000000 msumastro-1.2.3/docs/conf.py
-drwxr-xr-x   0 mattcraig   (501) staff       (20)        0 2022-11-30 16:13:20.455521 msumastro-1.2.3/docs/header_processing/
--rw-r--r--   0 mattcraig   (501) staff       (20)      772 2019-11-17 18:02:38.000000 msumastro-1.2.3/docs/header_processing/index.rst
--rw-r--r--   0 mattcraig   (501) staff       (20)      478 2019-12-28 22:48:14.000000 msumastro-1.2.3/docs/index.rst
--rw-r--r--   0 mattcraig   (501) staff       (20)     4186 2019-11-17 18:02:38.000000 msumastro-1.2.3/docs/installation.rst
--rw-r--r--   0 mattcraig   (501) staff       (20)     2099 2019-12-28 22:47:46.000000 msumastro-1.2.3/docs/overview.rst
--rw-r--r--   0 mattcraig   (501) staff       (20)       53 2019-12-28 23:16:52.000000 msumastro-1.2.3/docs/rtd-pip-requirements
-drwxr-xr-x   0 mattcraig   (501) staff       (20)        0 2022-11-30 16:13:20.456096 msumastro-1.2.3/docs/scripts/
--rw-r--r--   0 mattcraig   (501) staff       (20)    10924 2019-11-17 18:02:38.000000 msumastro-1.2.3/docs/scripts/automated_scripts.rst
--rw-r--r--   0 mattcraig   (501) staff       (20)     2665 2019-11-17 18:02:38.000000 msumastro-1.2.3/docs/scripts/manual_processing.rst
--rw-r--r--   0 mattcraig   (501) staff       (20)     3825 2019-11-17 18:02:38.000000 msumastro-1.2.3/docs/scripts/scripts.rst
--rw-r--r--   0 mattcraig   (501) staff       (20)       55 2019-11-17 18:02:38.000000 msumastro-1.2.3/docs/xref.rst
-drwxr-xr-x   0 mattcraig   (501) staff       (20)        0 2022-11-30 16:13:20.456581 msumastro-1.2.3/msumastro/
--rw-r--r--   0 mattcraig   (501) staff       (20)       34 2022-11-26 19:41:35.000000 msumastro-1.2.3/msumastro/__init__.py
--rw-r--r--   0 mattcraig   (501) staff       (20)     5135 2019-12-28 22:27:32.000000 msumastro-1.2.3/msumastro/conftest.py
--rw-r--r--   0 mattcraig   (501) staff       (20)     2814 2019-12-28 22:27:43.000000 msumastro-1.2.3/msumastro/customlogger.py
-drwxr-xr-x   0 mattcraig   (501) staff       (20)        0 2022-11-30 16:13:20.457865 msumastro-1.2.3/msumastro/header_processing/
--rw-r--r--   0 mattcraig   (501) staff       (20)      150 2019-12-28 22:28:03.000000 msumastro-1.2.3/msumastro/header_processing/__init__.py
--rw-r--r--   0 mattcraig   (501) staff       (20)    15954 2022-11-27 19:18:36.000000 msumastro-1.2.3/msumastro/header_processing/astrometry.py
--rw-r--r--   0 mattcraig   (501) staff       (20)    18645 2022-06-02 14:13:07.000000 msumastro-1.2.3/msumastro/header_processing/feder.py
--rw-r--r--   0 mattcraig   (501) staff       (20)     6568 2019-12-28 22:26:17.000000 msumastro-1.2.3/msumastro/header_processing/fitskeyword.py
--rw-r--r--   0 mattcraig   (501) staff       (20)    30937 2022-06-02 14:13:07.000000 msumastro-1.2.3/msumastro/header_processing/patchers.py
-drwxr-xr-x   0 mattcraig   (501) staff       (20)        0 2022-11-30 16:13:20.458293 msumastro-1.2.3/msumastro/header_processing/tests/
--rw-r--r--   0 mattcraig   (501) staff       (20)        0 2019-11-17 18:02:38.000000 msumastro-1.2.3/msumastro/header_processing/tests/__init__.py
--rw-r--r--   0 mattcraig   (501) staff       (20)     1209 2019-12-28 22:28:23.000000 msumastro-1.2.3/msumastro/header_processing/tests/test_feder.py
--rw-r--r--   0 mattcraig   (501) staff       (20)     5359 2019-12-28 22:28:33.000000 msumastro-1.2.3/msumastro/header_processing/tests/test_fitskeyword.py
--rw-r--r--   0 mattcraig   (501) staff       (20)    25392 2022-06-02 14:13:07.000000 msumastro-1.2.3/msumastro/header_processing/tests/test_patchers.py
-drwxr-xr-x   0 mattcraig   (501) staff       (20)        0 2022-11-30 16:13:20.459131 msumastro-1.2.3/msumastro/scripts/
--rw-r--r--   0 mattcraig   (501) staff       (20)        0 2019-11-17 18:02:38.000000 msumastro-1.2.3/msumastro/scripts/__init__.py
--rw-r--r--   0 mattcraig   (501) staff       (20)     4570 2019-12-28 22:26:08.000000 msumastro-1.2.3/msumastro/scripts/quick_add_keys_to_file.py
--rw-r--r--   0 mattcraig   (501) staff       (20)    11249 2022-11-26 18:59:43.000000 msumastro-1.2.3/msumastro/scripts/run_astrometry.py
--rw-r--r--   0 mattcraig   (501) staff       (20)     7815 2019-12-28 22:28:56.000000 msumastro-1.2.3/msumastro/scripts/run_patch.py
--rw-r--r--   0 mattcraig   (501) staff       (20)     9260 2020-08-11 21:37:08.000000 msumastro-1.2.3/msumastro/scripts/run_standard_header_process.py
--rw-r--r--   0 mattcraig   (501) staff       (20)    13461 2022-06-03 19:12:49.000000 msumastro-1.2.3/msumastro/scripts/run_triage.py
--rw-r--r--   0 mattcraig   (501) staff       (20)     4983 2019-12-28 22:29:33.000000 msumastro-1.2.3/msumastro/scripts/script_helpers.py
--rw-r--r--   0 mattcraig   (501) staff       (20)     7342 2019-12-28 22:35:19.000000 msumastro-1.2.3/msumastro/scripts/sort_files.py
-drwxr-xr-x   0 mattcraig   (501) staff       (20)        0 2022-11-30 16:13:20.459316 msumastro-1.2.3/msumastro/scripts/tests/
--rw-r--r--   0 mattcraig   (501) staff       (20)        0 2019-11-17 18:02:38.000000 msumastro-1.2.3/msumastro/scripts/tests/__init__.py
--rw-r--r--   0 mattcraig   (501) staff       (20)    25943 2022-06-03 18:59:29.000000 msumastro-1.2.3/msumastro/scripts/tests/test_scripts.py
--rw-r--r--   0 mattcraig   (501) staff       (20)     6344 2022-06-02 14:13:07.000000 msumastro-1.2.3/msumastro/table_tree.py
-drwxr-xr-x   0 mattcraig   (501) staff       (20)        0 2022-11-30 16:13:20.459632 msumastro-1.2.3/msumastro/tests/
--rw-r--r--   0 mattcraig   (501) staff       (20)        0 2019-11-17 18:02:38.000000 msumastro-1.2.3/msumastro/tests/__init__.py
-drwxr-xr-x   0 mattcraig   (501) staff       (20)        0 2022-11-30 16:13:20.463110 msumastro-1.2.3/msumastro/tests/data/
--rw-r--r--   0 mattcraig   (501) staff       (20)    25920 2019-11-17 18:02:38.000000 msumastro-1.2.3/msumastro/tests/data/aspen_trimmed.fit
--rw-r--r--   0 mattcraig   (501) staff       (20)    43200 2019-11-17 18:02:38.000000 msumastro-1.2.3/msumastro/tests/data/biastest1.fit
--rw-r--r--   0 mattcraig   (501) staff       (20)    43200 2019-11-17 18:02:38.000000 msumastro-1.2.3/msumastro/tests/data/biastest2.fit
--rw-r--r--   0 mattcraig   (501) staff       (20)    43200 2019-11-17 18:02:38.000000 msumastro-1.2.3/msumastro/tests/data/biastest3.fit
--rw-r--r--   0 mattcraig   (501) staff       (20)    43200 2019-11-17 18:02:38.000000 msumastro-1.2.3/msumastro/tests/data/biastest4.fit
--rw-r--r--   0 mattcraig   (501) staff       (20)    43200 2019-11-17 18:02:38.000000 msumastro-1.2.3/msumastro/tests/data/biastest5.fit
--rw-r--r--   0 mattcraig   (501) staff       (20)     5760 2019-11-17 18:02:38.000000 msumastro-1.2.3/msumastro/tests/data/celestron_nightscape_10100_astro_fx_v106.fit
--rw-r--r--   0 mattcraig   (501) staff       (20)    43200 2019-11-17 18:02:38.000000 msumastro-1.2.3/msumastro/tests/data/darktest1.fit
--rw-r--r--   0 mattcraig   (501) staff       (20)    43200 2019-11-17 18:02:38.000000 msumastro-1.2.3/msumastro/tests/data/darktest2.fit
--rw-r--r--   0 mattcraig   (501) staff       (20)    43200 2019-11-17 18:02:38.000000 msumastro-1.2.3/msumastro/tests/data/darktest3.fit
--rw-r--r--   0 mattcraig   (501) staff       (20)    43200 2019-11-17 18:02:38.000000 msumastro-1.2.3/msumastro/tests/data/darktest4.fit
--rw-r--r--   0 mattcraig   (501) staff       (20)    43200 2019-11-17 18:02:38.000000 msumastro-1.2.3/msumastro/tests/data/darktest5.fit
--rw-r--r--   0 mattcraig   (501) staff       (20)    83520 2019-11-17 18:02:38.000000 msumastro-1.2.3/msumastro/tests/data/flattest.fit
--rw-r--r--   0 mattcraig   (501) staff       (20)     8640 2019-11-17 18:02:38.000000 msumastro-1.2.3/msumastro/tests/data/maximdl_5_21_header.fit
--rw-r--r--   0 mattcraig   (501) staff       (20)    46080 2019-11-17 18:02:38.000000 msumastro-1.2.3/msumastro/tests/data/maximdl_5_23_header.fit
--rw-r--r--   0 mattcraig   (501) staff       (20)    46080 2019-11-17 18:02:38.000000 msumastro-1.2.3/msumastro/tests/data/maximdl_6_16_header.fit
--rw-r--r--   0 mattcraig   (501) staff       (20)    31680 2019-11-17 18:02:38.000000 msumastro-1.2.3/msumastro/tests/data/maximdl_6_18_header.fit
--rw-r--r--   0 mattcraig   (501) staff       (20)   786240 2019-11-17 18:02:38.000000 msumastro-1.2.3/msumastro/tests/data/neon-on-dome-10-sec-high-res-though-scope.fit
--rw-r--r--   0 mattcraig   (501) staff       (20)     5760 2019-11-17 18:02:38.000000 msumastro-1.2.3/msumastro/tests/data/uint16.fit
--rw-r--r--   0 mattcraig   (501) staff       (20)     5760 2019-11-17 18:02:38.000000 msumastro-1.2.3/msumastro/tests/data/uint16_missing_filter.fit
--rw-r--r--   0 mattcraig   (501) staff       (20)     5760 2019-11-17 18:02:38.000000 msumastro-1.2.3/msumastro/tests/data/uint16_no_pointing.fit
--rw-r--r--   0 mattcraig   (501) staff       (20)     5760 2019-11-17 18:02:38.000000 msumastro-1.2.3/msumastro/tests/data/uint16_not_m101.fit
--rw-r--r--   0 mattcraig   (501) staff       (20)      537 2019-12-28 22:29:44.000000 msumastro-1.2.3/msumastro/tests/data.py
--rw-r--r--   0 mattcraig   (501) staff       (20)     7168 2019-12-28 22:25:21.000000 msumastro-1.2.3/msumastro/tests/test_image_grouper.py
-drwxr-xr-x   0 mattcraig   (501) staff       (20)        0 2022-11-30 16:13:20.457311 msumastro-1.2.3/msumastro.egg-info/
--rw-r--r--   0 mattcraig   (501) staff       (20)      612 2022-11-30 16:13:20.000000 msumastro-1.2.3/msumastro.egg-info/PKG-INFO
--rw-r--r--   0 mattcraig   (501) staff       (20)     2570 2022-11-30 16:13:20.000000 msumastro-1.2.3/msumastro.egg-info/SOURCES.txt
--rw-r--r--   0 mattcraig   (501) staff       (20)        1 2022-11-30 16:13:20.000000 msumastro-1.2.3/msumastro.egg-info/dependency_links.txt
--rw-r--r--   0 mattcraig   (501) staff       (20)      416 2022-11-30 16:13:20.000000 msumastro-1.2.3/msumastro.egg-info/entry_points.txt
--rw-r--r--   0 mattcraig   (501) staff       (20)        1 2022-11-30 16:13:20.000000 msumastro-1.2.3/msumastro.egg-info/not-zip-safe
--rw-r--r--   0 mattcraig   (501) staff       (20)      111 2022-11-30 16:13:20.000000 msumastro-1.2.3/msumastro.egg-info/requires.txt
--rw-r--r--   0 mattcraig   (501) staff       (20)       10 2022-11-30 16:13:20.000000 msumastro-1.2.3/msumastro.egg-info/top_level.txt
--rw-r--r--   0 mattcraig   (501) staff       (20)      132 2022-11-27 17:07:54.000000 msumastro-1.2.3/pyproject.toml
--rw-r--r--   0 mattcraig   (501) staff       (20)     1529 2022-11-30 16:13:20.463658 msumastro-1.2.3/setup.cfg
--rw-r--r--   0 mattcraig   (501) staff       (20)     1039 2022-11-26 19:17:27.000000 msumastro-1.2.3/setup.py
+drwxr-xr-x   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        0 2023-05-25 21:36:41.599059 msumastro-1.2.4/
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)       35 2022-04-01 18:50:53.000000 msumastro-1.2.4/.gitattributes
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)      187 2023-05-25 21:23:47.000000 msumastro-1.2.4/.gitignore
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)      143 2022-04-01 18:50:53.000000 msumastro-1.2.4/.readthedocs.yml
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     1254 2022-04-01 18:50:53.000000 msumastro-1.2.4/.travis.yml
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     1573 2022-04-01 18:50:53.000000 msumastro-1.2.4/LICENSE.rst
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)      125 2022-04-01 18:50:53.000000 msumastro-1.2.4/MANIFEST.in
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)      612 2023-05-25 21:36:41.599248 msumastro-1.2.4/PKG-INFO
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)      976 2022-04-01 18:50:53.000000 msumastro-1.2.4/README.rst
+drwxr-xr-x   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        0 2023-05-25 21:36:41.552060 msumastro-1.2.4/docs/
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     4658 2022-04-01 18:50:53.000000 msumastro-1.2.4/docs/Makefile
+drwxr-xr-x   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        0 2023-05-25 21:36:41.540445 msumastro-1.2.4/docs/_templates/
+drwxr-xr-x   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        0 2023-05-25 21:36:41.553553 msumastro-1.2.4/docs/_templates/autosummary/
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)       42 2022-04-01 18:50:53.000000 msumastro-1.2.4/docs/_templates/autosummary/base.rst
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)       43 2022-04-01 18:50:53.000000 msumastro-1.2.4/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)       44 2022-04-01 18:50:53.000000 msumastro-1.2.4/docs/_templates/autosummary/module.rst
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     7761 2022-04-01 18:50:53.000000 msumastro-1.2.4/docs/conf.py
+drwxr-xr-x   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        0 2023-05-25 21:36:41.554084 msumastro-1.2.4/docs/header_processing/
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)      772 2022-04-01 18:50:53.000000 msumastro-1.2.4/docs/header_processing/index.rst
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)      478 2022-04-01 18:50:53.000000 msumastro-1.2.4/docs/index.rst
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     4186 2022-04-01 18:50:53.000000 msumastro-1.2.4/docs/installation.rst
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     2099 2022-04-01 18:50:53.000000 msumastro-1.2.4/docs/overview.rst
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)       53 2022-04-01 18:50:53.000000 msumastro-1.2.4/docs/rtd-pip-requirements
+drwxr-xr-x   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        0 2023-05-25 21:36:41.555711 msumastro-1.2.4/docs/scripts/
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)    10924 2022-04-01 18:50:53.000000 msumastro-1.2.4/docs/scripts/automated_scripts.rst
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     2665 2022-04-01 18:50:53.000000 msumastro-1.2.4/docs/scripts/manual_processing.rst
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     3825 2022-04-01 18:50:53.000000 msumastro-1.2.4/docs/scripts/scripts.rst
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)       55 2022-04-01 18:50:53.000000 msumastro-1.2.4/docs/xref.rst
+drwxr-xr-x   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        0 2023-05-25 21:36:41.557714 msumastro-1.2.4/msumastro/
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)       34 2023-05-25 21:23:47.000000 msumastro-1.2.4/msumastro/__init__.py
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     5135 2022-04-01 18:50:53.000000 msumastro-1.2.4/msumastro/conftest.py
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     2814 2022-04-01 18:50:53.000000 msumastro-1.2.4/msumastro/customlogger.py
+drwxr-xr-x   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        0 2023-05-25 21:36:41.564090 msumastro-1.2.4/msumastro/header_processing/
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)      150 2022-04-01 18:50:53.000000 msumastro-1.2.4/msumastro/header_processing/__init__.py
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)    15954 2023-05-25 21:23:47.000000 msumastro-1.2.4/msumastro/header_processing/astrometry.py
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)    18704 2023-05-25 21:27:40.000000 msumastro-1.2.4/msumastro/header_processing/feder.py
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     6568 2022-04-01 18:50:53.000000 msumastro-1.2.4/msumastro/header_processing/fitskeyword.py
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)    30937 2022-06-01 17:57:03.000000 msumastro-1.2.4/msumastro/header_processing/patchers.py
+drwxr-xr-x   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        0 2023-05-25 21:36:41.567532 msumastro-1.2.4/msumastro/header_processing/tests/
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        0 2022-04-01 18:50:53.000000 msumastro-1.2.4/msumastro/header_processing/tests/__init__.py
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     1209 2022-04-01 18:50:53.000000 msumastro-1.2.4/msumastro/header_processing/tests/test_feder.py
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     5359 2022-04-01 18:50:53.000000 msumastro-1.2.4/msumastro/header_processing/tests/test_fitskeyword.py
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)    25392 2022-06-01 17:57:03.000000 msumastro-1.2.4/msumastro/header_processing/tests/test_patchers.py
+drwxr-xr-x   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        0 2023-05-25 21:36:41.574177 msumastro-1.2.4/msumastro/scripts/
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        0 2022-04-01 18:50:53.000000 msumastro-1.2.4/msumastro/scripts/__init__.py
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     4570 2022-04-01 18:50:53.000000 msumastro-1.2.4/msumastro/scripts/quick_add_keys_to_file.py
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)    11249 2023-05-25 21:23:47.000000 msumastro-1.2.4/msumastro/scripts/run_astrometry.py
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     7815 2022-04-01 18:50:53.000000 msumastro-1.2.4/msumastro/scripts/run_patch.py
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     9260 2022-04-01 18:50:53.000000 msumastro-1.2.4/msumastro/scripts/run_standard_header_process.py
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)    13461 2023-05-25 21:23:47.000000 msumastro-1.2.4/msumastro/scripts/run_triage.py
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     4983 2022-04-01 18:50:53.000000 msumastro-1.2.4/msumastro/scripts/script_helpers.py
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     7342 2022-04-01 18:50:53.000000 msumastro-1.2.4/msumastro/scripts/sort_files.py
+drwxr-xr-x   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        0 2023-05-25 21:36:41.575309 msumastro-1.2.4/msumastro/scripts/tests/
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        0 2022-04-01 18:50:53.000000 msumastro-1.2.4/msumastro/scripts/tests/__init__.py
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)    25943 2022-04-01 18:50:53.000000 msumastro-1.2.4/msumastro/scripts/tests/test_scripts.py
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     6344 2022-04-01 21:53:04.000000 msumastro-1.2.4/msumastro/table_tree.py
+drwxr-xr-x   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        0 2023-05-25 21:36:41.577580 msumastro-1.2.4/msumastro/tests/
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        0 2022-04-01 18:50:53.000000 msumastro-1.2.4/msumastro/tests/__init__.py
+drwxr-xr-x   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        0 2023-05-25 21:36:41.598636 msumastro-1.2.4/msumastro/tests/data/
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)    25920 2022-04-01 18:50:53.000000 msumastro-1.2.4/msumastro/tests/data/aspen_trimmed.fit
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)    43200 2022-04-01 18:50:53.000000 msumastro-1.2.4/msumastro/tests/data/biastest1.fit
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)    43200 2022-04-01 18:50:53.000000 msumastro-1.2.4/msumastro/tests/data/biastest2.fit
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)    43200 2022-04-01 18:50:53.000000 msumastro-1.2.4/msumastro/tests/data/biastest3.fit
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)    43200 2022-04-01 18:50:53.000000 msumastro-1.2.4/msumastro/tests/data/biastest4.fit
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)    43200 2022-04-01 18:50:53.000000 msumastro-1.2.4/msumastro/tests/data/biastest5.fit
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     5760 2022-04-01 18:50:53.000000 msumastro-1.2.4/msumastro/tests/data/celestron_nightscape_10100_astro_fx_v106.fit
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)    43200 2022-04-01 18:50:53.000000 msumastro-1.2.4/msumastro/tests/data/darktest1.fit
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)    43200 2022-04-01 18:50:53.000000 msumastro-1.2.4/msumastro/tests/data/darktest2.fit
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)    43200 2022-04-01 18:50:53.000000 msumastro-1.2.4/msumastro/tests/data/darktest3.fit
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)    43200 2022-04-01 18:50:53.000000 msumastro-1.2.4/msumastro/tests/data/darktest4.fit
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)    43200 2022-04-01 18:50:53.000000 msumastro-1.2.4/msumastro/tests/data/darktest5.fit
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)    83520 2022-04-01 18:50:53.000000 msumastro-1.2.4/msumastro/tests/data/flattest.fit
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     8640 2022-04-01 18:50:53.000000 msumastro-1.2.4/msumastro/tests/data/maximdl_5_21_header.fit
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)    46080 2022-04-01 18:50:53.000000 msumastro-1.2.4/msumastro/tests/data/maximdl_5_23_header.fit
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)    46080 2022-04-01 18:50:53.000000 msumastro-1.2.4/msumastro/tests/data/maximdl_6_16_header.fit
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)    31680 2022-04-01 18:50:53.000000 msumastro-1.2.4/msumastro/tests/data/maximdl_6_18_header.fit
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)   786240 2022-04-01 18:50:53.000000 msumastro-1.2.4/msumastro/tests/data/neon-on-dome-10-sec-high-res-though-scope.fit
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     5760 2022-04-01 18:50:53.000000 msumastro-1.2.4/msumastro/tests/data/uint16.fit
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     5760 2022-04-01 18:50:53.000000 msumastro-1.2.4/msumastro/tests/data/uint16_missing_filter.fit
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     5760 2022-04-01 18:50:53.000000 msumastro-1.2.4/msumastro/tests/data/uint16_no_pointing.fit
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     5760 2022-04-01 18:50:53.000000 msumastro-1.2.4/msumastro/tests/data/uint16_not_m101.fit
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)      537 2022-04-01 18:50:53.000000 msumastro-1.2.4/msumastro/tests/data.py
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     7168 2022-04-01 18:50:53.000000 msumastro-1.2.4/msumastro/tests/test_image_grouper.py
+drwxr-xr-x   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        0 2023-05-25 21:36:41.560437 msumastro-1.2.4/msumastro.egg-info/
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)      612 2023-05-25 21:36:41.000000 msumastro-1.2.4/msumastro.egg-info/PKG-INFO
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     2570 2023-05-25 21:36:41.000000 msumastro-1.2.4/msumastro.egg-info/SOURCES.txt
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        1 2023-05-25 21:36:41.000000 msumastro-1.2.4/msumastro.egg-info/dependency_links.txt
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)      416 2023-05-25 21:36:41.000000 msumastro-1.2.4/msumastro.egg-info/entry_points.txt
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)        1 2023-05-25 21:36:41.000000 msumastro-1.2.4/msumastro.egg-info/not-zip-safe
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)      111 2023-05-25 21:36:41.000000 msumastro-1.2.4/msumastro.egg-info/requires.txt
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)       10 2023-05-25 21:36:41.000000 msumastro-1.2.4/msumastro.egg-info/top_level.txt
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)      132 2023-05-25 21:23:47.000000 msumastro-1.2.4/pyproject.toml
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     1529 2023-05-25 21:36:41.600008 msumastro-1.2.4/setup.cfg
+-rw-r--r--   0 jv8699qa (145084326) MNSTATE\Domain Users (2132868096)     1039 2023-05-25 21:23:47.000000 msumastro-1.2.4/setup.py
```

### Comparing `msumastro-1.2.3/.travis.yml` & `msumastro-1.2.4/.travis.yml`

 * *Files identical despite different names*

### Comparing `msumastro-1.2.3/LICENSE.rst` & `msumastro-1.2.4/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `msumastro-1.2.3/PKG-INFO` & `msumastro-1.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msumastro
-Version: 1.2.3
+Version: 1.2.4
 Summary: Process FITS files
 Home-page: http://github.com/mwcraig/msumastro
 Author: Matt Craig
 Author-email: mattwcraig@gmail.com
 License: BSD 3-Clause
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `msumastro-1.2.3/README.rst` & `msumastro-1.2.4/README.rst`

 * *Files identical despite different names*

### Comparing `msumastro-1.2.3/docs/Makefile` & `msumastro-1.2.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `msumastro-1.2.3/docs/conf.py` & `msumastro-1.2.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `msumastro-1.2.3/docs/header_processing/index.rst` & `msumastro-1.2.4/docs/header_processing/index.rst`

 * *Files identical despite different names*

### Comparing `msumastro-1.2.3/docs/installation.rst` & `msumastro-1.2.4/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `msumastro-1.2.3/docs/overview.rst` & `msumastro-1.2.4/docs/overview.rst`

 * *Files identical despite different names*

### Comparing `msumastro-1.2.3/docs/scripts/automated_scripts.rst` & `msumastro-1.2.4/docs/scripts/automated_scripts.rst`

 * *Files identical despite different names*

### Comparing `msumastro-1.2.3/docs/scripts/manual_processing.rst` & `msumastro-1.2.4/docs/scripts/manual_processing.rst`

 * *Files identical despite different names*

### Comparing `msumastro-1.2.3/docs/scripts/scripts.rst` & `msumastro-1.2.4/docs/scripts/scripts.rst`

 * *Files identical despite different names*

### Comparing `msumastro-1.2.3/msumastro/conftest.py` & `msumastro-1.2.4/msumastro/conftest.py`

 * *Files identical despite different names*

### Comparing `msumastro-1.2.3/msumastro/customlogger.py` & `msumastro-1.2.4/msumastro/customlogger.py`

 * *Files identical despite different names*

### Comparing `msumastro-1.2.3/msumastro/header_processing/astrometry.py` & `msumastro-1.2.4/msumastro/header_processing/astrometry.py`

 * *Files identical despite different names*

### Comparing `msumastro-1.2.3/msumastro/header_processing/feder.py` & `msumastro-1.2.4/msumastro/header_processing/feder.py`

 * *Files 1% similar despite different names*

```diff
@@ -311,20 +311,21 @@
     def __init__(self):
         bad_keys = ['OBJECT', 'JD', 'JD-HELIO', 'OBJCTALT', 'OBJCTAZ',
                     'OBJCTHA', 'AIRMASS', 'OBSERVER']
         fits_name = ['MaxIm DL Version 6.16 190601 00KPP',
                      'MaxIm DL Version 6.17 190601 00KPP',
                      'MaxIm DL Version 6.18 190601 00KPP',
                      'MaxIm DL Version 6.27 220525 26KU2',
-                     'MaxIm DL Version 6.29 220525 26KU2'
+                     'MaxIm DL Version 6.29 220525 26KU2',
+                     'MaxIm DL Version 6.30 220525 26KU2'
                      ]
         super(MaximDL6, self).__init__("MaxImDL",
                                        fits_name=fits_name,
                                        major_version=6,
-                                       minor_version=29,
+                                       minor_version=30,
                                        bad_keywords=bad_keys,
                                        fits_keyword='SWCREATE'
                                        )
 
 
 class SBIGCCDOps(ImageSoftware):
     """
```

### Comparing `msumastro-1.2.3/msumastro/header_processing/fitskeyword.py` & `msumastro-1.2.4/msumastro/header_processing/fitskeyword.py`

 * *Files identical despite different names*

### Comparing `msumastro-1.2.3/msumastro/header_processing/patchers.py` & `msumastro-1.2.4/msumastro/header_processing/patchers.py`

 * *Files identical despite different names*

### Comparing `msumastro-1.2.3/msumastro/header_processing/tests/test_feder.py` & `msumastro-1.2.4/msumastro/header_processing/tests/test_feder.py`

 * *Files identical despite different names*

### Comparing `msumastro-1.2.3/msumastro/header_processing/tests/test_fitskeyword.py` & `msumastro-1.2.4/msumastro/header_processing/tests/test_fitskeyword.py`

 * *Files identical despite different names*

### Comparing `msumastro-1.2.3/msumastro/header_processing/tests/test_patchers.py` & `msumastro-1.2.4/msumastro/header_processing/tests/test_patchers.py`

 * *Files identical despite different names*

### Comparing `msumastro-1.2.3/msumastro/scripts/quick_add_keys_to_file.py` & `msumastro-1.2.4/msumastro/scripts/quick_add_keys_to_file.py`

 * *Files identical despite different names*

### Comparing `msumastro-1.2.3/msumastro/scripts/run_astrometry.py` & `msumastro-1.2.4/msumastro/scripts/run_astrometry.py`

 * *Files identical despite different names*

### Comparing `msumastro-1.2.3/msumastro/scripts/run_patch.py` & `msumastro-1.2.4/msumastro/scripts/run_patch.py`

 * *Files identical despite different names*

### Comparing `msumastro-1.2.3/msumastro/scripts/run_standard_header_process.py` & `msumastro-1.2.4/msumastro/scripts/run_standard_header_process.py`

 * *Files identical despite different names*

### Comparing `msumastro-1.2.3/msumastro/scripts/run_triage.py` & `msumastro-1.2.4/msumastro/scripts/run_triage.py`

 * *Files identical despite different names*

### Comparing `msumastro-1.2.3/msumastro/scripts/script_helpers.py` & `msumastro-1.2.4/msumastro/scripts/script_helpers.py`

 * *Files identical despite different names*

### Comparing `msumastro-1.2.3/msumastro/scripts/sort_files.py` & `msumastro-1.2.4/msumastro/scripts/sort_files.py`

 * *Files identical despite different names*

### Comparing `msumastro-1.2.3/msumastro/scripts/tests/test_scripts.py` & `msumastro-1.2.4/msumastro/scripts/tests/test_scripts.py`

 * *Files identical despite different names*

### Comparing `msumastro-1.2.3/msumastro/table_tree.py` & `msumastro-1.2.4/msumastro/table_tree.py`

 * *Files identical despite different names*

### Comparing `msumastro-1.2.3/msumastro/tests/data/aspen_trimmed.fit` & `msumastro-1.2.4/msumastro/tests/data/aspen_trimmed.fit`

 * *Files identical despite different names*

### Comparing `msumastro-1.2.3/msumastro/tests/data/biastest1.fit` & `msumastro-1.2.4/msumastro/tests/data/biastest1.fit`

 * *Files identical despite different names*

### Comparing `msumastro-1.2.3/msumastro/tests/data/biastest2.fit` & `msumastro-1.2.4/msumastro/tests/data/biastest2.fit`

 * *Files identical despite different names*

### Comparing `msumastro-1.2.3/msumastro/tests/data/biastest3.fit` & `msumastro-1.2.4/msumastro/tests/data/biastest3.fit`

 * *Files identical despite different names*

### Comparing `msumastro-1.2.3/msumastro/tests/data/biastest4.fit` & `msumastro-1.2.4/msumastro/tests/data/biastest4.fit`

 * *Files identical despite different names*

### Comparing `msumastro-1.2.3/msumastro/tests/data/biastest5.fit` & `msumastro-1.2.4/msumastro/tests/data/biastest5.fit`

 * *Files identical despite different names*

### Comparing `msumastro-1.2.3/msumastro/tests/data/celestron_nightscape_10100_astro_fx_v106.fit` & `msumastro-1.2.4/msumastro/tests/data/celestron_nightscape_10100_astro_fx_v106.fit`

 * *Files identical despite different names*

### Comparing `msumastro-1.2.3/msumastro/tests/data/darktest1.fit` & `msumastro-1.2.4/msumastro/tests/data/darktest1.fit`

 * *Files identical despite different names*

### Comparing `msumastro-1.2.3/msumastro/tests/data/darktest2.fit` & `msumastro-1.2.4/msumastro/tests/data/darktest2.fit`

 * *Files identical despite different names*

### Comparing `msumastro-1.2.3/msumastro/tests/data/darktest3.fit` & `msumastro-1.2.4/msumastro/tests/data/darktest3.fit`

 * *Files identical despite different names*

### Comparing `msumastro-1.2.3/msumastro/tests/data/darktest4.fit` & `msumastro-1.2.4/msumastro/tests/data/darktest4.fit`

 * *Files identical despite different names*

### Comparing `msumastro-1.2.3/msumastro/tests/data/darktest5.fit` & `msumastro-1.2.4/msumastro/tests/data/darktest5.fit`

 * *Files identical despite different names*

### Comparing `msumastro-1.2.3/msumastro/tests/data/flattest.fit` & `msumastro-1.2.4/msumastro/tests/data/flattest.fit`

 * *Files identical despite different names*

### Comparing `msumastro-1.2.3/msumastro/tests/data/maximdl_5_21_header.fit` & `msumastro-1.2.4/msumastro/tests/data/maximdl_5_21_header.fit`

 * *Files identical despite different names*

### Comparing `msumastro-1.2.3/msumastro/tests/data/maximdl_5_23_header.fit` & `msumastro-1.2.4/msumastro/tests/data/maximdl_5_23_header.fit`

 * *Files identical despite different names*

### Comparing `msumastro-1.2.3/msumastro/tests/data/maximdl_6_16_header.fit` & `msumastro-1.2.4/msumastro/tests/data/maximdl_6_16_header.fit`

 * *Files identical despite different names*

### Comparing `msumastro-1.2.3/msumastro/tests/data/maximdl_6_18_header.fit` & `msumastro-1.2.4/msumastro/tests/data/maximdl_6_18_header.fit`

 * *Files identical despite different names*

### Comparing `msumastro-1.2.3/msumastro/tests/data/neon-on-dome-10-sec-high-res-though-scope.fit` & `msumastro-1.2.4/msumastro/tests/data/neon-on-dome-10-sec-high-res-though-scope.fit`

 * *Files identical despite different names*

### Comparing `msumastro-1.2.3/msumastro/tests/data/uint16.fit` & `msumastro-1.2.4/msumastro/tests/data/uint16.fit`

 * *Files identical despite different names*

### Comparing `msumastro-1.2.3/msumastro/tests/data/uint16_missing_filter.fit` & `msumastro-1.2.4/msumastro/tests/data/uint16_missing_filter.fit`

 * *Files identical despite different names*

### Comparing `msumastro-1.2.3/msumastro/tests/data/uint16_no_pointing.fit` & `msumastro-1.2.4/msumastro/tests/data/uint16_no_pointing.fit`

 * *Files identical despite different names*

### Comparing `msumastro-1.2.3/msumastro/tests/data/uint16_not_m101.fit` & `msumastro-1.2.4/msumastro/tests/data/uint16_not_m101.fit`

 * *Files identical despite different names*

### Comparing `msumastro-1.2.3/msumastro/tests/data.py` & `msumastro-1.2.4/msumastro/tests/data.py`

 * *Files identical despite different names*

### Comparing `msumastro-1.2.3/msumastro/tests/test_image_grouper.py` & `msumastro-1.2.4/msumastro/tests/test_image_grouper.py`

 * *Files identical despite different names*

### Comparing `msumastro-1.2.3/msumastro.egg-info/PKG-INFO` & `msumastro-1.2.4/msumastro.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msumastro
-Version: 1.2.3
+Version: 1.2.4
 Summary: Process FITS files
 Home-page: http://github.com/mwcraig/msumastro
 Author: Matt Craig
 Author-email: mattwcraig@gmail.com
 License: BSD 3-Clause
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `msumastro-1.2.3/msumastro.egg-info/SOURCES.txt` & `msumastro-1.2.4/msumastro.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `msumastro-1.2.3/setup.cfg` & `msumastro-1.2.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `msumastro-1.2.3/setup.py` & `msumastro-1.2.4/setup.py`

 * *Files identical despite different names*

