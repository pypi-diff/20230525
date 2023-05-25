# Comparing `tmp/surface-water-network-0.5.tar.gz` & `tmp/surface-water-network-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "surface-water-network-0.5.tar", last modified: Wed Jul 20 09:12:31 2022, max compression
+gzip compressed data, was "surface-water-network-0.6.tar", last modified: Thu May 25 00:34:26 2023, max compression
```

## Comparing `surface-water-network-0.5.tar` & `surface-water-network-0.6.tar`

### file list

```diff
@@ -1,30 +1,111 @@
-drwxrwxr-x   0 mtoews    (2978) mtoews    (2978)        0 2022-07-20 09:12:31.480528 surface-water-network-0.5/
--rw-rw-r--   0 mtoews    (2978) mtoews    (2978)     1510 2021-08-06 03:08:41.000000 surface-water-network-0.5/LICENSE
--rw-rw-r--   0 mtoews    (2978) mtoews    (2978)     4624 2022-07-20 09:12:31.480528 surface-water-network-0.5/PKG-INFO
--rw-rw-r--   0 mtoews    (2978) mtoews    (2978)     3663 2022-07-20 09:10:43.000000 surface-water-network-0.5/README.md
--rw-rw-r--   0 mtoews    (2978) mtoews    (2978)     1546 2022-07-20 09:06:24.000000 surface-water-network-0.5/pyproject.toml
--rw-rw-r--   0 mtoews    (2978) mtoews    (2978)       38 2022-07-20 09:12:31.480528 surface-water-network-0.5/setup.cfg
--rw-rw-r--   0 mtoews    (2978) mtoews    (2978)       38 2022-06-28 22:05:15.000000 surface-water-network-0.5/setup.py
-drwxrwxr-x   0 mtoews    (2978) mtoews    (2978)        0 2022-07-20 09:12:31.476528 surface-water-network-0.5/surface_water_network.egg-info/
--rw-rw-r--   0 mtoews    (2978) mtoews    (2978)     4624 2022-07-20 09:12:31.000000 surface-water-network-0.5/surface_water_network.egg-info/PKG-INFO
--rw-rw-r--   0 mtoews    (2978) mtoews    (2978)      541 2022-07-20 09:12:31.000000 surface-water-network-0.5/surface_water_network.egg-info/SOURCES.txt
--rw-rw-r--   0 mtoews    (2978) mtoews    (2978)        1 2022-07-20 09:12:31.000000 surface-water-network-0.5/surface_water_network.egg-info/dependency_links.txt
--rw-rw-r--   0 mtoews    (2978) mtoews    (2978)      203 2022-07-20 09:12:31.000000 surface-water-network-0.5/surface_water_network.egg-info/requires.txt
--rw-rw-r--   0 mtoews    (2978) mtoews    (2978)        4 2022-07-20 09:12:31.000000 surface-water-network-0.5/surface_water_network.egg-info/top_level.txt
-drwxrwxr-x   0 mtoews    (2978) mtoews    (2978)        0 2022-07-20 09:12:31.476528 surface-water-network-0.5/swn/
--rw-rw-r--   0 mtoews    (2978) mtoews    (2978)      464 2022-05-03 22:52:20.000000 surface-water-network-0.5/swn/__init__.py
--rw-rw-r--   0 mtoews    (2978) mtoews    (2978)       89 2022-07-20 09:06:24.000000 surface-water-network-0.5/swn/_version.py
--rw-rw-r--   0 mtoews    (2978) mtoews    (2978)     1747 2022-05-03 22:52:20.000000 surface-water-network-0.5/swn/compat.py
--rw-rw-r--   0 mtoews    (2978) mtoews    (2978)    82686 2022-07-20 09:06:24.000000 surface-water-network-0.5/swn/core.py
--rw-rw-r--   0 mtoews    (2978) mtoews    (2978)     5704 2022-07-01 04:10:30.000000 surface-water-network-0.5/swn/file.py
--rw-rw-r--   0 mtoews    (2978) mtoews    (2978)      968 2022-05-03 22:52:20.000000 surface-water-network-0.5/swn/logger.py
-drwxrwxr-x   0 mtoews    (2978) mtoews    (2978)        0 2022-07-20 09:12:31.480528 surface-water-network-0.5/swn/modflow/
--rw-rw-r--   0 mtoews    (2978) mtoews    (2978)      270 2022-05-03 22:52:20.000000 surface-water-network-0.5/swn/modflow/__init__.py
--rw-rw-r--   0 mtoews    (2978) mtoews    (2978)    71530 2022-07-20 09:06:24.000000 surface-water-network-0.5/swn/modflow/_base.py
--rw-rw-r--   0 mtoews    (2978) mtoews    (2978)    88302 2022-05-03 22:52:20.000000 surface-water-network-0.5/swn/modflow/_legacy.py
--rw-rw-r--   0 mtoews    (2978) mtoews    (2978)     8740 2022-05-18 09:00:18.000000 surface-water-network-0.5/swn/modflow/_misc.py
--rw-rw-r--   0 mtoews    (2978) mtoews    (2978)    13907 2022-05-03 22:52:20.000000 surface-water-network-0.5/swn/modflow/_modelplot.py
--rw-rw-r--   0 mtoews    (2978) mtoews    (2978)    74126 2022-07-08 03:07:10.000000 surface-water-network-0.5/swn/modflow/_swnmf6.py
--rw-rw-r--   0 mtoews    (2978) mtoews    (2978)    72420 2022-07-08 03:07:10.000000 surface-water-network-0.5/swn/modflow/_swnmodflow.py
--rw-rw-r--   0 mtoews    (2978) mtoews    (2978)    16649 2022-06-23 00:37:34.000000 surface-water-network-0.5/swn/spatial.py
--rw-rw-r--   0 mtoews    (2978) mtoews    (2978)     2714 2022-06-21 22:58:50.000000 surface-water-network-0.5/swn/util.py
+drwxrwxr-x   0 mtoews    (2978) mtoews    (2978)        0 2023-05-25 00:34:26.487498 surface-water-network-0.6/
+-rw-rw-r--   0 mtoews    (2978) mtoews    (2978)      449 2023-01-19 09:12:54.000000 surface-water-network-0.6/.flake8
+drwxrwxr-x   0 mtoews    (2978) mtoews    (2978)        0 2023-05-25 00:34:26.467497 surface-water-network-0.6/.github/
+drwxrwxr-x   0 mtoews    (2978) mtoews    (2978)        0 2023-05-25 00:34:26.471497 surface-water-network-0.6/.github/workflows/
+-rw-rw-r--   0 mtoews    (2978) mtoews    (2978)      815 2022-11-10 23:00:22.000000 surface-water-network-0.6/.github/workflows/pages.yml
+-rw-rw-r--   0 mtoews    (2978) mtoews    (2978)     1582 2023-05-24 23:21:07.000000 surface-water-network-0.6/.github/workflows/tests.yml
+-rw-rw-r--   0 mtoews    (2978) mtoews    (2978)      665 2022-11-10 22:46:06.000000 surface-water-network-0.6/.gitignore
+-rw-rw-r--   0 mtoews    (2978) mtoews    (2978)      829 2023-05-24 23:36:35.000000 surface-water-network-0.6/CITATION.cff
+-rw-rw-r--   0 mtoews    (2978) mtoews    (2978)     1510 2021-08-06 03:08:41.000000 surface-water-network-0.6/LICENSE
+-rw-rw-r--   0 mtoews    (2978) mtoews    (2978)     4776 2023-05-25 00:34:26.487498 surface-water-network-0.6/PKG-INFO
+-rw-rw-r--   0 mtoews    (2978) mtoews    (2978)     3815 2023-02-24 00:13:32.000000 surface-water-network-0.6/README.md
+-rw-rw-r--   0 mtoews    (2978) mtoews    (2978)      408 2023-02-24 00:13:32.000000 surface-water-network-0.6/codecov.yml
+drwxrwxr-x   0 mtoews    (2978) mtoews    (2978)        0 2023-05-25 00:34:26.471497 surface-water-network-0.6/docs/
+-rw-rw-r--   0 mtoews    (2978) mtoews    (2978)      638 2021-08-06 03:32:49.000000 surface-water-network-0.6/docs/Makefile
+-rw-rw-r--   0 mtoews    (2978) mtoews    (2978)      799 2021-08-06 03:32:49.000000 surface-water-network-0.6/docs/make.bat
+drwxrwxr-x   0 mtoews    (2978) mtoews    (2978)        0 2023-05-25 00:34:26.471497 surface-water-network-0.6/docs/source/
+drwxrwxr-x   0 mtoews    (2978) mtoews    (2978)        0 2023-05-25 00:34:26.471497 surface-water-network-0.6/docs/source/_static/
+-rw-rw-r--   0 mtoews    (2978) mtoews    (2978)     6966 2021-08-06 03:32:49.000000 surface-water-network-0.6/docs/source/_static/swn_logo.svg
+-rw-rw-r--   0 mtoews    (2978) mtoews    (2978)     4949 2023-05-25 00:20:11.000000 surface-water-network-0.6/docs/source/changelog.rst
+-rw-rw-r--   0 mtoews    (2978) mtoews    (2978)     2966 2023-02-07 09:45:02.000000 surface-water-network-0.6/docs/source/conf.py
+-rw-rw-r--   0 mtoews    (2978) mtoews    (2978)      220 2023-02-09 23:41:03.000000 surface-water-network-0.6/docs/source/file.rst
+-rw-rw-r--   0 mtoews    (2978) mtoews    (2978)      256 2022-05-03 22:52:20.000000 surface-water-network-0.6/docs/source/index.rst
+-rw-rw-r--   0 mtoews    (2978) mtoews    (2978)     1379 2022-05-19 11:04:30.000000 surface-water-network-0.6/docs/source/quickstart.rst
+-rw-rw-r--   0 mtoews    (2978) mtoews    (2978)      225 2022-05-03 22:52:20.000000 surface-water-network-0.6/docs/source/reference.rst
+-rw-rw-r--   0 mtoews    (2978) mtoews    (2978)      182 2022-06-07 08:24:46.000000 surface-water-network-0.6/docs/source/spatial.rst
+-rw-rw-r--   0 mtoews    (2978) mtoews    (2978)     1302 2022-06-23 12:13:32.000000 surface-water-network-0.6/docs/source/swn.rst
+-rw-rw-r--   0 mtoews    (2978) mtoews    (2978)     1194 2023-02-09 23:41:03.000000 surface-water-network-0.6/docs/source/swnmf6.rst
+-rw-rw-r--   0 mtoews    (2978) mtoews    (2978)     1211 2023-02-23 23:06:29.000000 surface-water-network-0.6/docs/source/swnmodflow.rst
+-rw-rw-r--   0 mtoews    (2978) mtoews    (2978)     1627 2023-02-24 00:13:32.000000 surface-water-network-0.6/pyproject.toml
+-rw-rw-r--   0 mtoews    (2978) mtoews    (2978)       44 2022-06-28 22:05:15.000000 surface-water-network-0.6/pytest.ini
+-rw-rw-r--   0 mtoews    (2978) mtoews    (2978)       38 2023-05-25 00:34:26.487498 surface-water-network-0.6/setup.cfg
+-rw-rw-r--   0 mtoews    (2978) mtoews    (2978)       38 2022-06-28 22:05:15.000000 surface-water-network-0.6/setup.py
+drwxrwxr-x   0 mtoews    (2978) mtoews    (2978)        0 2023-05-25 00:34:26.471497 surface-water-network-0.6/surface_water_network.egg-info/
+-rw-rw-r--   0 mtoews    (2978) mtoews    (2978)     4776 2023-05-25 00:34:26.000000 surface-water-network-0.6/surface_water_network.egg-info/PKG-INFO
+-rw-rw-r--   0 mtoews    (2978) mtoews    (2978)     2528 2023-05-25 00:34:26.000000 surface-water-network-0.6/surface_water_network.egg-info/SOURCES.txt
+-rw-rw-r--   0 mtoews    (2978) mtoews    (2978)        1 2023-05-25 00:34:26.000000 surface-water-network-0.6/surface_water_network.egg-info/dependency_links.txt
+-rw-rw-r--   0 mtoews    (2978) mtoews    (2978)      245 2023-05-25 00:34:26.000000 surface-water-network-0.6/surface_water_network.egg-info/requires.txt
+-rw-rw-r--   0 mtoews    (2978) mtoews    (2978)        4 2023-05-25 00:34:26.000000 surface-water-network-0.6/surface_water_network.egg-info/top_level.txt
+drwxrwxr-x   0 mtoews    (2978) mtoews    (2978)        0 2023-05-25 00:34:26.475498 surface-water-network-0.6/swn/
+-rw-rw-r--   0 mtoews    (2978) mtoews    (2978)      434 2022-07-20 09:34:14.000000 surface-water-network-0.6/swn/__init__.py
+-rw-rw-r--   0 mtoews    (2978) mtoews    (2978)      155 2023-05-25 00:34:26.000000 surface-water-network-0.6/swn/_version.py
+-rw-rw-r--   0 mtoews    (2978) mtoews    (2978)     1747 2022-05-03 22:52:20.000000 surface-water-network-0.6/swn/compat.py
+-rw-rw-r--   0 mtoews    (2978) mtoews    (2978)    83353 2023-05-24 23:20:49.000000 surface-water-network-0.6/swn/core.py
+-rw-rw-r--   0 mtoews    (2978) mtoews    (2978)    13020 2023-05-24 23:20:49.000000 surface-water-network-0.6/swn/file.py
+-rw-rw-r--   0 mtoews    (2978) mtoews    (2978)      968 2022-05-03 22:52:20.000000 surface-water-network-0.6/swn/logger.py
+drwxrwxr-x   0 mtoews    (2978) mtoews    (2978)        0 2023-05-25 00:34:26.475498 surface-water-network-0.6/swn/modflow/
+-rw-rw-r--   0 mtoews    (2978) mtoews    (2978)      235 2023-02-09 23:41:03.000000 surface-water-network-0.6/swn/modflow/__init__.py
+-rw-rw-r--   0 mtoews    (2978) mtoews    (2978)    72338 2023-05-24 23:20:49.000000 surface-water-network-0.6/swn/modflow/_base.py
+-rw-rw-r--   0 mtoews    (2978) mtoews    (2978)     8741 2022-10-06 23:11:41.000000 surface-water-network-0.6/swn/modflow/_misc.py
+-rw-rw-r--   0 mtoews    (2978) mtoews    (2978)    13992 2023-05-24 23:20:49.000000 surface-water-network-0.6/swn/modflow/_modelplot.py
+-rw-rw-r--   0 mtoews    (2978) mtoews    (2978)    87823 2023-05-24 23:20:49.000000 surface-water-network-0.6/swn/modflow/_swnmf6.py
+-rw-rw-r--   0 mtoews    (2978) mtoews    (2978)    85306 2023-02-23 23:06:29.000000 surface-water-network-0.6/swn/modflow/_swnmodflow.py
+-rw-rw-r--   0 mtoews    (2978) mtoews    (2978)    19543 2023-04-05 21:39:31.000000 surface-water-network-0.6/swn/spatial.py
+-rw-rw-r--   0 mtoews    (2978) mtoews    (2978)     2714 2022-10-03 23:41:00.000000 surface-water-network-0.6/swn/util.py
+drwxrwxr-x   0 mtoews    (2978) mtoews    (2978)        0 2023-05-25 00:34:26.475498 surface-water-network-0.6/tests/
+-rw-rw-r--   0 mtoews    (2978) mtoews    (2978)       18 2021-08-06 03:15:02.000000 surface-water-network-0.6/tests/__init__.py
+-rw-rw-r--   0 mtoews    (2978) mtoews    (2978)     4353 2023-05-24 23:20:49.000000 surface-water-network-0.6/tests/conftest.py
+drwxrwxr-x   0 mtoews    (2978) mtoews    (2978)        0 2023-05-25 00:34:26.483498 surface-water-network-0.6/tests/data/
+-rw-rw-r--   0 mtoews    (2978) mtoews    (2978)      176 2022-06-02 03:18:07.000000 surface-water-network-0.6/tests/data/Coastal_points.dbf
+-rw-rw-r--   0 mtoews    (2978) mtoews    (2978)      432 2022-06-02 03:18:07.000000 surface-water-network-0.6/tests/data/Coastal_points.prj
+-rw-rw-r--   0 mtoews    (2978) mtoews    (2978)      380 2022-06-02 03:18:07.000000 surface-water-network-0.6/tests/data/Coastal_points.shp
+-rw-rw-r--   0 mtoews    (2978) mtoews    (2978)      180 2022-06-02 03:18:07.000000 surface-water-network-0.6/tests/data/Coastal_points.shx
+-rw-rw-r--   0 mtoews    (2978) mtoews    (2978)    42513 2019-06-15 01:51:18.000000 surface-water-network-0.6/tests/data/DN2_Coastal_strahler1_vf.dbf
+-rw-rw-r--   0 mtoews    (2978) mtoews    (2978)      432 2019-06-15 01:51:18.000000 surface-water-network-0.6/tests/data/DN2_Coastal_strahler1_vf.prj
+-rw-rw-r--   0 mtoews    (2978) mtoews    (2978)     3332 2019-06-15 01:51:18.000000 surface-water-network-0.6/tests/data/DN2_Coastal_strahler1_vf.sbn
+-rw-rw-r--   0 mtoews    (2978) mtoews    (2978)      452 2019-06-15 01:51:18.000000 surface-water-network-0.6/tests/data/DN2_Coastal_strahler1_vf.sbx
+-rw-rw-r--   0 mtoews    (2978) mtoews    (2978)   473128 2019-06-15 01:51:18.000000 surface-water-network-0.6/tests/data/DN2_Coastal_strahler1_vf.shp
+-rw-rw-r--   0 mtoews    (2978) mtoews    (2978)     2492 2019-06-15 01:51:18.000000 surface-water-network-0.6/tests/data/DN2_Coastal_strahler1_vf.shx
+-rw-rw-r--   0 mtoews    (2978) mtoews    (2978)   111554 2019-05-21 08:56:12.000000 surface-water-network-0.6/tests/data/DN2_Coastal_strahler1z_stream_vf.dbf
+-rw-rw-r--   0 mtoews    (2978) mtoews    (2978)      432 2019-05-21 08:56:12.000000 surface-water-network-0.6/tests/data/DN2_Coastal_strahler1z_stream_vf.prj
+-rw-rw-r--   0 mtoews    (2978) mtoews    (2978)     3412 2019-05-21 08:56:12.000000 surface-water-network-0.6/tests/data/DN2_Coastal_strahler1z_stream_vf.sbn
+-rw-rw-r--   0 mtoews    (2978) mtoews    (2978)      492 2019-05-21 08:56:12.000000 surface-water-network-0.6/tests/data/DN2_Coastal_strahler1z_stream_vf.sbx
+-rw-rw-r--   0 mtoews    (2978) mtoews    (2978)   159876 2019-05-21 08:56:12.000000 surface-water-network-0.6/tests/data/DN2_Coastal_strahler1z_stream_vf.shp
+-rw-rw-r--   0 mtoews    (2978) mtoews    (2978)     2532 2019-05-21 08:56:12.000000 surface-water-network-0.6/tests/data/DN2_Coastal_strahler1z_stream_vf.shx
+-rw-rw-r--   0 mtoews    (2978) mtoews    (2978)      499 2019-05-27 10:22:13.000000 surface-water-network-0.6/tests/data/h.bas
+-rw-rw-r--   0 mtoews    (2978) mtoews    (2978)     1544 2019-05-27 10:08:42.000000 surface-water-network-0.6/tests/data/h.botm1.ref
+-rw-rw-r--   0 mtoews    (2978) mtoews    (2978)     1712 2019-05-27 10:08:42.000000 surface-water-network-0.6/tests/data/h.botm2.ref
+-rw-rw-r--   0 mtoews    (2978) mtoews    (2978)     1734 2019-05-27 10:08:42.000000 surface-water-network-0.6/tests/data/h.botm3.ref
+-rw-rw-r--   0 mtoews    (2978) mtoews    (2978)      610 2019-05-27 10:57:50.000000 surface-water-network-0.6/tests/data/h.dis
+-rw-rw-r--   0 mtoews    (2978) mtoews    (2978)       27 2019-06-10 09:52:23.000000 surface-water-network-0.6/tests/data/h.drn
+-rw-rw-r--   0 mtoews    (2978) mtoews    (2978)      612 2019-05-27 10:25:42.000000 surface-water-network-0.6/tests/data/h.ibound1.inf
+-rw-rw-r--   0 mtoews    (2978) mtoews    (2978)      612 2019-05-27 10:25:42.000000 surface-water-network-0.6/tests/data/h.ibound2.inf
+-rw-rw-r--   0 mtoews    (2978) mtoews    (2978)      612 2019-05-27 10:25:42.000000 surface-water-network-0.6/tests/data/h.ibound3.inf
+-rw-rw-r--   0 mtoews    (2978) mtoews    (2978)      495 2021-08-06 03:32:49.000000 surface-water-network-0.6/tests/data/h.nam
+-rw-rw-r--   0 mtoews    (2978) mtoews    (2978)      147 2019-05-27 10:16:59.000000 surface-water-network-0.6/tests/data/h.nwt
+-rw-rw-r--   0 mtoews    (2978) mtoews    (2978)      103 2019-05-27 10:35:21.000000 surface-water-network-0.6/tests/data/h.oc
+-rw-rw-r--   0 mtoews    (2978) mtoews    (2978)       91 2019-05-27 10:55:56.000000 surface-water-network-0.6/tests/data/h.rch
+-rw-rw-r--   0 mtoews    (2978) mtoews    (2978)     2466 2019-05-27 10:33:49.000000 surface-water-network-0.6/tests/data/h.rech.ref
+-rw-rw-r--   0 mtoews    (2978) mtoews    (2978)     1450 2019-05-27 10:06:12.000000 surface-water-network-0.6/tests/data/h.top.ref
+-rw-rw-r--   0 mtoews    (2978) mtoews    (2978)      757 2019-05-27 10:54:25.000000 surface-water-network-0.6/tests/data/h.upw
+drwxrwxr-x   0 mtoews    (2978) mtoews    (2978)        0 2023-05-25 00:34:26.487498 surface-water-network-0.6/tests/data/mf6_coastal/
+-rw-rw-r--   0 mtoews    (2978) mtoews    (2978)    23875 2021-08-06 03:32:49.000000 surface-water-network-0.6/tests/data/mf6_coastal/h.dis
+-rw-rw-r--   0 mtoews    (2978) mtoews    (2978)      247 2021-08-06 03:32:49.000000 surface-water-network-0.6/tests/data/mf6_coastal/h.drn
+-rw-rw-r--   0 mtoews    (2978) mtoews    (2978)    14150 2021-08-06 03:32:49.000000 surface-water-network-0.6/tests/data/mf6_coastal/h.ic
+-rw-rw-r--   0 mtoews    (2978) mtoews    (2978)      845 2021-08-06 03:32:49.000000 surface-water-network-0.6/tests/data/mf6_coastal/h.ims
+-rw-rw-r--   0 mtoews    (2978) mtoews    (2978)      306 2022-10-03 23:41:00.000000 surface-water-network-0.6/tests/data/mf6_coastal/h.nam
+-rw-rw-r--   0 mtoews    (2978) mtoews    (2978)      422 2021-08-06 03:32:49.000000 surface-water-network-0.6/tests/data/mf6_coastal/h.npf
+-rw-rw-r--   0 mtoews    (2978) mtoews    (2978)      290 2021-08-06 03:32:49.000000 surface-water-network-0.6/tests/data/mf6_coastal/h.oc
+-rw-rw-r--   0 mtoews    (2978) mtoews    (2978)     4776 2021-08-06 03:32:49.000000 surface-water-network-0.6/tests/data/mf6_coastal/h.rch
+-rw-rw-r--   0 mtoews    (2978) mtoews    (2978)      288 2021-08-06 03:32:49.000000 surface-water-network-0.6/tests/data/mf6_coastal/h.tdis
+-rw-rw-r--   0 mtoews    (2978) mtoews    (2978)      267 2021-08-06 03:32:49.000000 surface-water-network-0.6/tests/data/mf6_coastal/mfsim.nam
+-rw-rw-r--   0 mtoews    (2978) mtoews    (2978)    28995 2019-06-15 01:51:18.000000 surface-water-network-0.6/tests/data/streamq_20170115_20170128_topnet_03046727_m3day.csv
+-rw-rw-r--   0 mtoews    (2978) mtoews    (2978)    63813 2019-06-15 01:51:18.000000 surface-water-network-0.6/tests/data/streamq_20170115_20170128_topnet_03046727_strahler1.nc
+-rw-rw-r--   0 mtoews    (2978) mtoews    (2978)    56125 2023-05-24 23:20:49.000000 surface-water-network-0.6/tests/test_basic.py
+-rw-rw-r--   0 mtoews    (2978) mtoews    (2978)     5524 2022-05-03 22:52:20.000000 surface-water-network-0.6/tests/test_complex.py
+-rw-rw-r--   0 mtoews    (2978) mtoews    (2978)     9197 2023-05-24 23:20:49.000000 surface-water-network-0.6/tests/test_file.py
+-rw-rw-r--   0 mtoews    (2978) mtoews    (2978)    74135 2023-05-24 23:20:49.000000 surface-water-network-0.6/tests/test_modflow.py
+-rw-rw-r--   0 mtoews    (2978) mtoews    (2978)    56075 2023-05-24 23:20:49.000000 surface-water-network-0.6/tests/test_modflow6.py
+-rw-rw-r--   0 mtoews    (2978) mtoews    (2978)    50464 2023-05-24 23:20:49.000000 surface-water-network-0.6/tests/test_modflow_base.py
+-rw-rw-r--   0 mtoews    (2978) mtoews    (2978)    16154 2023-02-07 09:45:02.000000 surface-water-network-0.6/tests/test_spatial.py
+-rw-rw-r--   0 mtoews    (2978) mtoews    (2978)     2271 2022-06-21 22:59:13.000000 surface-water-network-0.6/tests/test_util.py
```

### Comparing `surface-water-network-0.5/LICENSE` & `surface-water-network-0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `surface-water-network-0.5/PKG-INFO` & `surface-water-network-0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,47 +1,48 @@
 Metadata-Version: 2.1
 Name: surface-water-network
-Version: 0.5
+Version: 0.6
 Summary: Surface water network
 Author-email: Mike Taves <mwtoews@gmail.com>, Brioch Hemmings <briochh@gmail.com>
 Maintainer-email: Mike Taves <mwtoews@gmail.com>
 License: BSD 3-Clause
 Project-URL: Documentation, https://mwtoews.github.io/surface-water-network/
 Project-URL: Source, https://github.com/mwtoews/surface-water-network
 Keywords: surface water,groundwater,MODFLOW,flopy
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering :: Hydrology
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: doc
 Provides-Extra: extra
 Provides-Extra: lint
 Provides-Extra: test
 License-File: LICENSE
 
 # Surface water network
 [![DOI](https://zenodo.org/badge/187739645.svg)](https://zenodo.org/badge/latestdoi/187739645)
-[![Codacy Badge](https://api.codacy.com/project/badge/Grade/420bcd8896c14f18b2077dd987c78849)](https://app.codacy.com/manual/mwtoews/surface-water-network?utm_source=github.com&utm_medium=referral&utm_content=mwtoews/surface-water-network&utm_campaign=Badge_Grade_Dashboard)
-[![CI](https://github.com/mwtoews/surface-water-network/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/mwtoews/surface-water-network/actions/workflows/ci.yml)
+[![Codacy](https://api.codacy.com/project/badge/Grade/420bcd8896c14f18b2077dd987c78849)](https://app.codacy.com/manual/mwtoews/surface-water-network?utm_source=github.com&utm_medium=referral&utm_content=mwtoews/surface-water-network&utm_campaign=Badge_Grade_Dashboard)
+[![Codcov](https://codecov.io/gh/mwtoews/surface-water-network/branch/main/graph/badge.svg)](https://codecov.io/gh/mwtoews/surface-water-network)
+[![CI](https://github.com/mwtoews/surface-water-network/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/mwtoews/surface-water-network/actions/workflows/tests.yml)
 
 A Python package to create and analyze surface water networks.
 
 
 ## Python packages
 
-Python 3.7+ is required.
+Python 3.8+ is required.
 
 ### Required
 
- - `geopandas` - process spatial data similar to pandas
+ - `geopandas >=0.9` - process spatial data similar to pandas
  - `packaging` - used to check package versions
  - `pandas >=1.2` - tabular data analysis
  - `pyproj >=2.2` - spatial projection support
  - `rtree` - spatial index support
 
 ### Optional
```

### Comparing `surface-water-network-0.5/README.md` & `surface-water-network-0.6/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 # Surface water network
 [![DOI](https://zenodo.org/badge/187739645.svg)](https://zenodo.org/badge/latestdoi/187739645)
-[![Codacy Badge](https://api.codacy.com/project/badge/Grade/420bcd8896c14f18b2077dd987c78849)](https://app.codacy.com/manual/mwtoews/surface-water-network?utm_source=github.com&utm_medium=referral&utm_content=mwtoews/surface-water-network&utm_campaign=Badge_Grade_Dashboard)
-[![CI](https://github.com/mwtoews/surface-water-network/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/mwtoews/surface-water-network/actions/workflows/ci.yml)
+[![Codacy](https://api.codacy.com/project/badge/Grade/420bcd8896c14f18b2077dd987c78849)](https://app.codacy.com/manual/mwtoews/surface-water-network?utm_source=github.com&utm_medium=referral&utm_content=mwtoews/surface-water-network&utm_campaign=Badge_Grade_Dashboard)
+[![Codcov](https://codecov.io/gh/mwtoews/surface-water-network/branch/main/graph/badge.svg)](https://codecov.io/gh/mwtoews/surface-water-network)
+[![CI](https://github.com/mwtoews/surface-water-network/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/mwtoews/surface-water-network/actions/workflows/tests.yml)
 
 A Python package to create and analyze surface water networks.
 
 
 ## Python packages
 
-Python 3.7+ is required.
+Python 3.8+ is required.
 
 ### Required
 
- - `geopandas` - process spatial data similar to pandas
+ - `geopandas >=0.9` - process spatial data similar to pandas
  - `packaging` - used to check package versions
  - `pandas >=1.2` - tabular data analysis
  - `pyproj >=2.2` - spatial projection support
  - `rtree` - spatial index support
 
 ### Optional
```

### Comparing `surface-water-network-0.5/pyproject.toml` & `surface-water-network-0.6/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 [build-system]
 requires = [
     "setuptools>=61",
+    "setuptools-scm[toml]>=6.2",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "surface-water-network"
 dynamic = ["version"]
 authors = [
@@ -23,50 +24,53 @@
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: BSD License",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3 :: Only",
     "Topic :: Scientific/Engineering :: Hydrology",
 ]
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 dependencies = [
-    "geopandas",
+    "geopandas >=0.9",
     "packaging",
     "pandas >=1.2",
     "pyproj >=2.2",
     "rtree",
     "shapely",
 ]
 
 [project.optional-dependencies]
 doc = [
     "ipython",
     "matplotlib",
     "numpydoc",
     "pydata-sphinx-theme",
-    "sphinx",
+    "sphinx <6",
     "sphinx-issues",
 ]
 extra = [
     "flopy",
     "matplotlib",
     "netcdf4",
 ]
 lint = [
+    "cffconvert",
     "flake8",
 ]
 test = [
     "pytest >=3.3",
+    "pytest-cov",
+    "pytest-xdist",
 ]
 
 [project.urls]
 Documentation = "https://mwtoews.github.io/surface-water-network/"
 Source = "https://github.com/mwtoews/surface-water-network"
 
 [tool.setuptools.packages.find]
 include = [
     "swn",
     "swn.*",
 ]
 
-[tool.setuptools.dynamic]
-version = {attr = "swn._version.version"}
+[tool.setuptools_scm]
+write_to = "swn/_version.py"
```

### Comparing `surface-water-network-0.5/surface_water_network.egg-info/PKG-INFO` & `surface-water-network-0.6/surface_water_network.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,47 +1,48 @@
 Metadata-Version: 2.1
 Name: surface-water-network
-Version: 0.5
+Version: 0.6
 Summary: Surface water network
 Author-email: Mike Taves <mwtoews@gmail.com>, Brioch Hemmings <briochh@gmail.com>
 Maintainer-email: Mike Taves <mwtoews@gmail.com>
 License: BSD 3-Clause
 Project-URL: Documentation, https://mwtoews.github.io/surface-water-network/
 Project-URL: Source, https://github.com/mwtoews/surface-water-network
 Keywords: surface water,groundwater,MODFLOW,flopy
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering :: Hydrology
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: doc
 Provides-Extra: extra
 Provides-Extra: lint
 Provides-Extra: test
 License-File: LICENSE
 
 # Surface water network
 [![DOI](https://zenodo.org/badge/187739645.svg)](https://zenodo.org/badge/latestdoi/187739645)
-[![Codacy Badge](https://api.codacy.com/project/badge/Grade/420bcd8896c14f18b2077dd987c78849)](https://app.codacy.com/manual/mwtoews/surface-water-network?utm_source=github.com&utm_medium=referral&utm_content=mwtoews/surface-water-network&utm_campaign=Badge_Grade_Dashboard)
-[![CI](https://github.com/mwtoews/surface-water-network/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/mwtoews/surface-water-network/actions/workflows/ci.yml)
+[![Codacy](https://api.codacy.com/project/badge/Grade/420bcd8896c14f18b2077dd987c78849)](https://app.codacy.com/manual/mwtoews/surface-water-network?utm_source=github.com&utm_medium=referral&utm_content=mwtoews/surface-water-network&utm_campaign=Badge_Grade_Dashboard)
+[![Codcov](https://codecov.io/gh/mwtoews/surface-water-network/branch/main/graph/badge.svg)](https://codecov.io/gh/mwtoews/surface-water-network)
+[![CI](https://github.com/mwtoews/surface-water-network/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/mwtoews/surface-water-network/actions/workflows/tests.yml)
 
 A Python package to create and analyze surface water networks.
 
 
 ## Python packages
 
-Python 3.7+ is required.
+Python 3.8+ is required.
 
 ### Required
 
- - `geopandas` - process spatial data similar to pandas
+ - `geopandas >=0.9` - process spatial data similar to pandas
  - `packaging` - used to check package versions
  - `pandas >=1.2` - tabular data analysis
  - `pyproj >=2.2` - spatial projection support
  - `rtree` - spatial index support
 
 ### Optional
```

### Comparing `surface-water-network-0.5/swn/compat.py` & `surface-water-network-0.6/swn/compat.py`

 * *Files identical despite different names*

### Comparing `surface-water-network-0.5/swn/core.py` & `surface-water-network-0.6/swn/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,18 +7,19 @@
 from math import sqrt
 from textwrap import dedent
 from warnings import warn
 
 import geopandas
 import numpy as np
 import pandas as pd
+import shapely
 from shapely.geometry import LineString, Point
 
-from .compat import ignore_shapely_warnings_for_object_array
-from .spatial import bias_substring, get_sindex
+from .compat import ignore_shapely_warnings_for_object_array, SHAPELY_GE_20
+from .spatial import bias_substring
 from .util import abbr_str
 
 
 class SurfaceWaterNetwork:
     """Surface water network class.
 
     Attributes
@@ -180,16 +181,17 @@
             numbers. The geometry is copied to the segments property.
         polygons : geopandas.GeoSeries, optional
             Optional input polygons of surface water catchments. Geometries
             must be ``POLYGON``. Index must be the same as ``segments.index``.
 
         Examples
         --------
+        >>> import geopandas
         >>> import swn
-        >>> lines = swn.spatial.wkt_to_geoseries([
+        >>> lines = geopandas.GeoSeries.from_wkt([
         ...    "LINESTRING (60 100, 60  80)",
         ...    "LINESTRING (40 130, 60 100)",
         ...    "LINESTRING (70 130, 60 100)"])
         >>> lines.index += 100
         >>> n = swn.SurfaceWaterNetwork.from_lines(lines)
         >>> n
         <SurfaceWaterNetwork:
@@ -239,15 +241,15 @@
         to_segnum = to_segnum_l.apply(lambda x: x[0])
         obj.segments.loc[to_segnum.index, "to_segnum"] = to_segnum.values
         headwater = obj.headwater
         outlets = obj.outlets
 
         # A few checks
         sel = to_segnum_l.apply(len) > 1
-        for segnum1, to_segnums in to_segnum_l.loc[sel].iteritems():
+        for segnum1, to_segnums in to_segnum_l.loc[sel].items():
             m = ('segment %s has more than one downstream segments: %s',
                  segnum1, str(to_segnums))
             obj.logger.error(*m)
             obj.errors.append(m[0] % m[1:])
         if obj.has_z:
             # Check if match is in 2D but not 3D
             jxn["start_z"] = start_pts.loc[jxn.start].z.values
@@ -423,16 +425,17 @@
             See :py:meth:`estimate_width` for details.
         diversions : set
             If diversions are defined, this is a set of zero or more indexes
             to which the segment connects to.
 
         Examples
         --------
+        >>> import geopandas
         >>> import swn
-        >>> lines = swn.spatial.wkt_to_geoseries([
+        >>> lines = geopandas.GeoSeries.from_wkt([
         ...    "LINESTRING (60 100, 60  80)",
         ...    "LINESTRING (40 130, 60 100)",
         ...    "LINESTRING (70 130, 60 100)"])
         >>> lines.index += 100
         >>> n = swn.SurfaceWaterNetwork.from_lines(lines)
         >>> n.segments.columns
         Index(['geometry', 'to_segnum', 'from_segnums', 'cat_group', 'num_to_outlet',
@@ -454,21 +457,22 @@
         Catchment polygons are optional, and are set with a GeoSeries with
         a matching index to ``segments.index``.
 
         To unset this property, use ``n.catchments = None``.
 
         Examples
         --------
+        >>> import geopandas
         >>> import swn
-        >>> lines = swn.spatial.wkt_to_geoseries([
+        >>> lines = geopandas.GeoSeries.from_wkt([
         ...    "LINESTRING (60 100, 60  80)",
         ...    "LINESTRING (40 130, 60 100)",
         ...    "LINESTRING (70 130, 60 100)"])
         >>> lines.index += 100
-        >>> polygons = swn.spatial.wkt_to_geoseries([
+        >>> polygons = geopandas.GeoSeries.from_wkt([
         ...    "POLYGON ((35 100, 75 100, 75  80, 35  80, 35 100))",
         ...    "POLYGON ((35 135, 60 135, 60 100, 35 100, 35 135))",
         ...    "POLYGON ((60 135, 75 135, 75 100, 60 100, 60 135))"])
         >>> polygons.index += 100
         >>> n = swn.SurfaceWaterNetwork.from_lines(lines, polygons)
         >>> n
         <SurfaceWaterNetwork: with catchment polygons
@@ -658,15 +662,15 @@
         return self.segments.index[
                 ~self.segments.index.isin(self.segments['to_segnum'])]
 
     @property
     def outlets(self):
         """Return index of outlets.
 
-        Determined where ``n.segments.to_segnum == n.END_SEGNUM`
+        Determined where ``n.segments.to_segnum == n.END_SEGNUM``
         """
         return self.segments.index[
                 self.segments['to_segnum'] == self.END_SEGNUM]
 
     @property
     def to_segnums(self):
         """Return Series of segnum to connect downstream.
@@ -946,22 +950,23 @@
             Resulting GeoDataFrame has columns geometry (always LineString),
             method (override, catchment or nearest), segnum,
             seg_ndist (normalized distance along segment), and
             dist_to_seg (distance to segment).
 
         Examples
         --------
+        >>> import geopandas
         >>> import swn
-        >>> lines = swn.spatial.wkt_to_geoseries([
+        >>> lines = geopandas.GeoSeries.from_wkt([
         ...    "LINESTRING (60 100, 60  80)",
         ...    "LINESTRING (40 130, 60 100)",
         ...    "LINESTRING (70 130, 60 100)"])
         >>> n = swn.SurfaceWaterNetwork.from_lines(lines)
         >>> lines.index += 101
-        >>> obs_gs = swn.spatial.wkt_to_geoseries([
+        >>> obs_gs = geopandas.GeoSeries.from_wkt([
         ...    "POINT (56 103)",
         ...    "LINESTRING (58 90, 62 90)",
         ...    "POLYGON ((60 107, 59 113, 61 113, 60 107))",
         ...    "POINT (55 130)"])
         >>> obs_gs.index += 11
         >>> obs_match = n.locate_geoms(obs_gs, override={14: 2})
         >>> obs_match[["method", "segnum", "seg_ndist", "dist_to_seg"]]
@@ -1137,15 +1142,15 @@
                                 "start", ascending=False, inplace=True)
                         else:
                             sl.sort_values("segnum", inplace=True)
                         match.drop(index=sl.index[1:], inplace=True)
                 res.loc[match.gidx, "segnum"] = match.segnum.values
                 res.loc[match.gidx, "method"] = "nearest"
             else:  # slower method
-                for gidx, g in geom[sel].iteritems():
+                for gidx, g in geom[sel].items():
                     dists = segments_gs.distance(g).sort_values()
                     segnums = dists.index[dists.iloc[0] == dists]
                     if len(segnums) == 1:
                         segnum = segnums[0]
                     else:
                         sg = self.segments.geometry[segnums]
                         sl = pd.DataFrame(index=segnums)
@@ -1177,19 +1182,28 @@
 
         # Add attributes for match
         sel = res.segnum != self.END_SEGNUM
         res["seg_ndist"] = res.loc[sel].apply(
             lambda f: self.segments.geometry[f.segnum].project(
                 f.geometry, normalized=True), axis=1)
         # Line between geometry and line segment
-        with ignore_shapely_warnings_for_object_array():
+        if SHAPELY_GE_20:
+            res["pt2"] = shapely.force_2d(res.loc[sel].apply(
+                lambda f: self.segments.geometry[f.segnum].interpolate(
+                        f.seg_ndist, normalized=True), axis=1))
             res["link"] = res.loc[sel].apply(
-                lambda f: LineString(
-                    [f.geometry, self.segments.geometry[f.segnum].interpolate(
-                        f.seg_ndist, normalized=True)]), axis=1)
+                lambda f: LineString([f.geometry, f.pt2]), axis=1)
+            res.drop(columns="pt2", inplace=True)
+        else:
+            with ignore_shapely_warnings_for_object_array():
+                res["link"] = res.loc[sel].apply(
+                    lambda f: LineString(
+                        [f.geometry,
+                         self.segments.geometry[f.segnum].interpolate(
+                             f.seg_ndist, normalized=True)]), axis=1)
         if (~sel).any():
             linestring_empty = wkt.loads("LINESTRING EMPTY")
             for idx in res[~sel].index:
                 res.at[idx, "link"] = linestring_empty
         res.set_geometry("link", drop=True, inplace=True)
         res["dist_to_seg"] = res[sel].length
         return res
@@ -1488,16 +1502,17 @@
 
         Returns
         -------
         pandas.Series
 
         Examples
         --------
+        >>> import geopandas
         >>> import swn
-        >>> lines = swn.spatial.wkt_to_geoseries([
+        >>> lines = geopandas.GeoSeries.from_wkt([
         ...    "LINESTRING (60 100, 60  80)",
         ...    "LINESTRING (40 130, 60 100)",
         ...    "LINESTRING (70 130, 60 100)"])
         >>> n = swn.SurfaceWaterNetwork.from_lines(lines)
         >>> n.segments_series(1.2)
         0    1.2
         1    1.2
@@ -1550,14 +1565,15 @@
             but will overwrite any other values determined by ``method``.
         name : str, default None
             Base name used for the column names, if provided. For example,
             ``name="foo"`` will create columns "foo1" and "foo2".
         method : str, default "continuous"
             This option determines how ``value_out`` values should be
             determined, if not specified. Choose one of:
+
               - ``continuous`` (default): downstream value is evaluated to be
                 the same as the upstream value it connects to. This allows a
                 continuous network of values along the networks, such as
                 elevation.
               - ``constant`` : ``value_out`` is the same as ``value``.
               - ``additive`` : downstream value is evaluated to be a fraction
                 of tributaries that add to the upstream value it connects to.
@@ -1568,16 +1584,17 @@
         -------
         pandas.DataFrame
             Resulting DataFrame has two columns for top (1) and bottom (2) of
             each segment.
 
         Examples
         --------
+        >>> import geopandas
         >>> import swn
-        >>> lines = swn.spatial.wkt_to_geoseries([
+        >>> lines = geopandas.GeoSeries.from_wkt([
         ...    "LINESTRING (60 100, 60  80)",
         ...    "LINESTRING (40 130, 60 100)",
         ...    "LINESTRING (70 130, 60 100)"])
         >>> n = swn.SurfaceWaterNetwork.from_lines(lines)
         >>> n.pair_segments_frame([3, 4, 5])
            1  2
         0  3  3
@@ -1605,22 +1622,22 @@
         else:
             df.columns += 1
         c1, c2 = df.columns
         if method == "continuous":
             to_segnums = self.to_segnums
             df.loc[to_segnums.index, c2] = df.loc[to_segnums, c1].values
         elif method == "additive":
-            for segnum, from_segnums in self.from_segnums.iteritems():
+            for segnum, from_segnums in self.from_segnums.items():
                 if len(from_segnums) <= 1:
                     continue
                 # get proportions of upstream values
                 from_value1 = df.loc[sorted(from_segnums), c1]
                 from_value1_prop = from_value1 / from_value1.sum()
                 from_value2 = df.loc[segnum, c1] * from_value1_prop
-                for from_segnum, v2 in from_value2.iteritems():
+                for from_segnum, v2 in from_value2.items():
                     df.loc[from_segnum, c2] = v2
         elif method == "constant":
             pass
         if value_out is not None:
             if np.isscalar(value_out):
                 # generate only for outlets
                 value_out = pd.Series(value_out, index=self.outlets)
@@ -1660,15 +1677,15 @@
         modified_d = {}  # key is segnum, value is drop amount (+ve is down)
         self.messages = []
 
         # Build elevation profile list storing three values per coordinate:
         #   [dx, elev], where dx is 2D distance from upstream coord
         #   elev is the adjusted elevation
         profile_d = {}  # key is segnum, value is list of profile tuples
-        for segnum, geom in self.segments.geometry.iteritems():
+        for segnum, geom in self.segments.geometry.items():
             coords = geom.coords[:]  # coordinates
             x0, y0, z0 = coords[0]  # upstream coordinate
             profile = [[0.0, z0]]
             for idx, (x1, y1, z1) in enumerate(coords[1:], 1):
                 dx = sqrt((x0 - x1) ** 2 + (y0 - y1) ** 2)
                 profile.append([dx, z1])
                 x0, y0, z0 = x1, y1, z1
@@ -1870,17 +1887,19 @@
             else:
                 diversion_points = div_seg_pt
             diversion_points.plot(
                 ax=ax, label='diversion', marker='+', color='red')
             if diversions_is_spatial:
                 diversion_lines = []
                 for item in self.diversions.itertuples():
+                    pt2 = div_seg_pt[item.Index]
+                    if SHAPELY_GE_20 and pt2.has_z:
+                        pt2 = shapely.force_2d(pt2)
                     diversion_lines.append(
-                        LineString([item.geometry.centroid,
-                                    div_seg_pt[item.Index]]))
+                        LineString([item.geometry.centroid, pt2]))
                 diversion_lines = geopandas.GeoSeries(diversion_lines)
                 diversion_lines.plot(
                     ax=ax, label='diversion lines',
                     linestyle='--', color='deepskyblue')
         return ax
 
     def to_pickle(self, path, protocol=pickle.HIGHEST_PROTOCOL):
@@ -1909,10 +1928,8 @@
         path : str
             File path where the pickled object will be stored.
 
         See Also
         --------
         to_pickle : Save file.
         """
-        with open(path, "rb") as f:
-            obj = pickle.load(f)
-        return obj
+        return pd.read_pickle(path)
```

### Comparing `surface-water-network-0.5/swn/logger.py` & `surface-water-network-0.6/swn/logger.py`

 * *Files identical despite different names*

### Comparing `surface-water-network-0.5/swn/modflow/_base.py` & `surface-water-network-0.6/swn/modflow/_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import pandas as pd
 from shapely import wkt
 from shapely.geometry import LineString, Point, Polygon, box
 from shapely.ops import linemerge, substring
 
 from ..compat import ignore_shapely_warnings_for_object_array
 from ..core import SurfaceWaterNetwork
-from ..spatial import bias_substring, compare_crs, get_sindex, visible_wkt
+from ..spatial import bias_substring, compare_crs, visible_wkt
 from ..util import is_location_frame
 from ._misc import tile_series_as_frame, transform_data_to_series_or_frame
 
 
 class SwnModflowBase:
     """Abstract class for a surface water network adaptor for MODFLOW.
 
@@ -113,16 +113,15 @@
             File path where the pickled object will be stored.
         swn : swn.SurfaceWaterNetwork, optional
             Instance of a SurfaceWaterNetwork.
         model : flopy.modflow.Modflow or flopy.mf6.ModflowGwf, optional
             Instance of a flopy MODFLOW model.
 
         """
-        with open(path, "rb") as f:
-            obj = pickle.load(f)
+        obj = pd.read_pickle(path)
         if swn is not None:
             obj.swn = swn
         if model is not None:
             obj.model = model
         return obj
 
     @property
@@ -282,15 +281,15 @@
                 raise ValueError("BAS6 package required")
         elif this_class == "SwnMf6":
             if not (isinstance(model, flopy.mf6.mfmodel.MFModel)):
                 raise ValueError(
                     "model must be a flopy.mf6.MFModel object; found " +
                     str(type(model)))
             sim = model.simulation
-            if "tdis" not in sim.package_key_dict.keys():
+            if "tdis" not in sim.package_type_dict.keys():
                 raise ValueError("TDIS package required")
             if "dis" not in model.package_type_dict.keys():
                 raise ValueError("DIS package required")
             if not model.dis.idomain.has_data():
                 raise ValueError("DIS idomain has no data")
         else:
             raise NotImplementedError(this_class)
@@ -388,15 +387,15 @@
         grid_df = pd.DataFrame({"i": rows.flatten(), "j": cols.flatten()})
         grid_df.set_index(["i", "j"], inplace=True)
         grid_df[domain_label] = domain.flatten()
         # Note: modelgrid.get_cell_vertices(i, j) is slow!
         xv = modelgrid.xvertices
         yv = modelgrid.yvertices
         i, j = (np.array(s[1])
-                for s in grid_df.reset_index()[["i", "j"]].iteritems())
+                for s in grid_df.reset_index()[["i", "j"]].items())
         cell_verts = zip(
             zip(xv[i, j], yv[i, j]),
             zip(xv[i, j + 1], yv[i, j + 1]),
             zip(xv[i + 1, j + 1], yv[i + 1, j + 1]),
             zip(xv[i + 1, j], yv[i + 1, j])
         )
         # Add dataframe of model grid cells to object
@@ -461,14 +460,15 @@
         dis = model.dis
         grid_cells = obj.grid_cells.copy()
         if domain_action == "freeze":
             sel = grid_cells[domain_label] != 0
             if sel.any():
                 # Remove any inactive grid cells from analysis
                 grid_cells = grid_cells.loc[sel]
+        _ = grid_cells.sindex  # create spatial index
         num_domain_modified = 0
         if this_class == "SwnModflow":
             domain_label = "ibound"
             domain = model.bas6.ibound[0].array.copy()
         elif this_class == "SwnMf6":
             domain_label = "idomain"
             domain = dis.idomain.array[0].copy()
@@ -484,15 +484,14 @@
         if dis.delc.array.min() != dis.delc.array.max():
             obj.logger.warning(
                 "assuming constant row spacing %s", row_size)
         cell_size = (row_size + col_size) / 2.0
 
         # Break up source segments according to the model grid definition
         obj.logger.debug("evaluating reach data on model grid")
-        grid_sindex = get_sindex(grid_cells)
         reach_include = swn.segments_series(reach_include_fraction) * cell_size
         # Make an empty DataFrame for reaches
         reaches = pd.DataFrame(columns=["geometry"])
         reaches.insert(1, column="i", value=pd.Series(dtype=int))
         reaches.insert(2, column="j", value=pd.Series(dtype=int))
         empty_reach_df = reaches.copy()  # take this before more added
         reaches.insert(
@@ -549,20 +548,20 @@
                 if (item.geometry.distance(reach_geom) < 1e-6 and
                         this_cell_length < other_cell_length):
                     matches.append((item[0], item.geometry))
             if len(matches) == 0:
                 # don't merge, e.g. reach does not connect to adjacent cell
                 pass
             elif len(matches) == 1:
-                # short segment is in one other cell only
+                # short reach is in one other cell only
                 # update new i and j values, keep geometry as it is
                 ij1 = tuple(reach_df.loc[matches[0][0], ["i", "j"]])
                 reach_df.loc[idx, ["i", "j", "moved"]] = ij1 + (True,)
-                # self.logger.debug(
-                #    "moved short segment of %s from %s to %s",
+                # obj.logger.debug(
+                #    "moved short reach of segnum %s from %s to %s",
                 #    segnum, this_ij, ij1)
             elif len(matches) == 2:
                 assert grid_points.geom_type == "MultiPoint", grid_points.wkt
                 if len(grid_points.geoms) != 2:
                     obj.logger.critical(
                         "expected 2 points, found %s", len(grid_points.geoms))
                 # Build a tiny DataFrame of coordinates for this reach
@@ -598,55 +597,49 @@
                 i2, j2 = list(reach_df.loc[matches[1][0], ["i", "j"]])
                 reach_geom2 = LineString(reach_geom.coords[cidx:])
                 # update the first, append the second
                 reach_df.loc[idx, ["i", "j", "length", "moved"]] = \
                     (i1, j1, reach_geom1.length, True)
                 reach_df.at[idx, "geometry"] = reach_geom1
                 append_reach_df(reach_df, i2, j2, reach_geom2, moved=True)
-                # self.logger.debug(
-                #   "split and moved short segment of %s from %s to %s and %s",
+                # obj.logger.debug(
+                #   "split and moved short reach of %s from %s to %s and %s",
                 #   segnum, this_ij, (i1, j1), (i2, j2))
             else:
                 obj.logger.critical(
                     "unhandled assign_short_reach case with %d matches: %s\n"
                     "%s\n%s", len(matches), matches, reach, grid_points.wkt)
 
         def assign_remaining_reach(reach_df, segnum, rem):
             if rem.geom_type == "LineString":
                 threshold = cell_size * 2.0
                 if rem.length > threshold:
                     obj.logger.debug(
-                        "remaining line segment from %s too long to merge "
+                        "remaining line from segnum %s too long to merge "
                         "(%.1f > %.1f)", segnum, rem.length, threshold)
                     return
                 # search full grid for other cells that could match
-                if grid_sindex:
-                    bbox_match = sorted(grid_sindex.intersection(rem.bounds))
-                    sub = grid_cells.geometry.iloc[bbox_match]
-                else:  # slow scan of all cells
-                    sub = grid_cells.geometry
-                assert len(sub) > 0, len(sub)
                 matches = []
-                for (i, j), grid_geom in sub.iteritems():
-                    if grid_geom.touches(rem):
-                        matches.append((i, j, grid_geom))
+                for gc in grid_cells[grid_cells.intersects(rem)].itertuples():
+                    assert gc.geometry.touches(rem)
+                    matches.append((*gc.Index, gc.geometry))
                 if len(matches) == 0:
                     return
                 threshold = reach_include[segnum]
                 # Build a tiny DataFrame for just the remaining coordinates
                 pts = [Point(c) for c in rem.coords[:]]
                 with ignore_shapely_warnings_for_object_array():
                     rem_c = pd.DataFrame({"pt": pts}, dtype=object)
                 if len(matches) == 1:  # merge it with adjacent cell
                     i, j, grid_geom = matches[0]
                     mdist = rem_c["pt"].apply(
                                     lambda p: grid_geom.distance(p)).max()
                     if mdist > threshold:
                         obj.logger.debug(
-                            "remaining line segment from %s too far away to "
+                            "remaining line from segnum %s too far away to "
                             "merge (%.1f > %.1f)", segnum, mdist, threshold)
                         return
                     append_reach_df(reach_df, i, j, rem, moved=True)
                 elif len(matches) == 2:  # complex: need to split it
                     if len(rem_c) == 2:
                         # If this is a simple line with two coords, split it
                         rem_c.index = [0, 2]
@@ -661,15 +654,15 @@
                                     lambda p: p.distance(matches[0][2]))
                     rem_c["d2"] = rem_c["pt"].apply(
                                     lambda p: p.distance(matches[1][2]))
                     rem_c["dm"] = rem_c[["d1", "d2"]].min(1)
                     mdist = rem_c["dm"].max()
                     if mdist > threshold:
                         obj.logger.debug(
-                            "remaining line segment from %s too far away to "
+                            "remaining line from segnum %s too far away to "
                             "merge (%.1f > %.1f)", segnum, mdist, threshold)
                         return
                     # try a simple split where distances switch
                     ds = rem_c["d1"] < rem_c["d2"]
                     cidx = ds[ds].index[-1]
                     # ensure it's not the index of either end
                     if cidx == 0:
@@ -714,34 +707,46 @@
                         obj.logger.warning(
                             "part %s does not cover any segnum %s at %s",
                             part, segnum, ij)
             else:
                 obj.logger.warning(
                     "failed to merge segnum %s at %s: %s", segnum, ij, geom)
 
-        # Looping over each segment breaking down into reaches
-        for segnum, line in segments.geometry.iteritems():
-            remaining_line = line
-            if grid_sindex:
-                bbox_match = sorted(grid_sindex.intersection(line.bounds))
-                if not bbox_match:
-                    continue
-                sub = grid_cells.geometry.iloc[bbox_match]
-            else:  # slow scan of all cells
-                sub = grid_cells.geometry
-            # Find all intersections between segment and grid cells
+        # Break down segments into reaches by overlaying grid
+        df1 = segments[["geometry"]].assign(segnum=segments.index)
+        if segments.has_sindex and not df1.has_sindex:
+            obj.logger.debug("copying sindex from segments")
+            df1.geometry.values._sindex = segments.geometry.values._sindex
+        df2 = grid_cells.reset_index()
+        if grid_cells.has_sindex and not df2.has_sindex:
+            obj.logger.debug("copying sindex from grid_cells")
+            df2.geometry.values._sindex = grid_cells.geometry.values._sindex
+        if df1.crs is None and df2.crs is not None:
+            df1.crs = df2.crs
+        elif df1.crs is not None and df2.crs is None:
+            df2.crs = df1.crs
+        grid_reaches = geopandas.overlay(
+            df1, df2,
+            how="intersection", keep_geom_type=True, make_valid=False)
+        check_geom_type = (
+            (grid_reaches.geom_type == "LineString") |
+            (grid_reaches.geom_type == "MultiLineString"))
+        assert check_geom_type.all()
+        # erase some odd floating point issues
+        grid_reaches["geometry"] = grid_reaches.geometry.apply(visible_wkt)
+
+        # Process each segment
+        for segnum, grid_reaches_df in grid_reaches.groupby("segnum"):
+            remaining_line = line = segments.geometry[segnum]
+            # process all intersections between segment and grid cells
             reach_df = empty_reach_df.copy()
-            for (i, j), grid_geom in sub.iteritems():
-                reach_geom = grid_geom.intersection(line)
-                if reach_geom.is_empty or reach_geom.geom_type == "Point":
-                    continue
-                # erase some odd floating point issues
-                reach_geom = visible_wkt(reach_geom)
+            for gr in grid_reaches_df.itertuples():
+                grid_geom = grid_cells.geometry[gr.i, gr.j]
                 remaining_line = remaining_line.difference(grid_geom)
-                append_reach_df(reach_df, i, j, reach_geom)
+                append_reach_df(reach_df, gr.i, gr.j, gr.geometry)
             # Determine if any remaining portions of the line can be used
             if line is not remaining_line and remaining_line.length > 0:
                 assign_remaining_reach(reach_df, segnum, remaining_line)
             # Reassign short reaches to two or more adjacent grid cells
             # starting with the shortest reach
             reach_lengths = reach_df["length"].loc[
                 reach_df["length"] < reach_include[segnum]]
@@ -757,17 +762,16 @@
                 reach_df.drop(drop_reach_ids, axis=0, inplace=True)
             # TODO: Some reaches match multiple cells if they share a border
             # Add all reaches for this segment
             for reach in reach_df.itertuples():
                 i = reach.i
                 j = reach.j
                 reach_geom = reach.geometry
-                if line.has_z:
-                    # intersection(line) does not preserve Z coords,
-                    # but line.interpolate(d) works as expected
+                if line.has_z and not reach_geom.has_z:
+                    # this should not be necessary, it can be expensive
                     reach_geom = LineString(line.interpolate(
                         line.project(Point(c))) for c in reach_geom.coords)
                 # Get a point from the middle of the reach_geom
                 reach_mid_pt = reach_geom.interpolate(0.5, normalized=True)
                 reach_record = {
                     "geometry": reach_geom,
                     "segnum": segnum,
@@ -846,15 +850,15 @@
             diversions = swn.diversions.copy()
             reaches["diversion"] = False
             reaches["divid"] = diversions.index.dtype.type()
             # Mark diversions that are not used / outside model
             diversions["in_model"] = True
             outside_model = []
             segnum_s = set(reaches.segnum)
-            for divid, from_segnum in diversions.from_segnum.iteritems():
+            for divid, from_segnum in diversions.from_segnum.items():
                 if from_segnum not in segnum_s:
                     # segnum does not exist -- segment is outside model
                     outside_model.append(divid)
             if outside_model:
                 diversions.loc[list(outside_model), "in_model"] = False
                 obj.logger.debug(
                     "added %d diversions, ignoring %d that did not connect to "
@@ -868,41 +872,50 @@
             else:
                 empty_geom = wkt.loads("linestring empty")
             diversions_in_model = diversions[diversions.in_model]
             is_spatial = (
                 isinstance(diversions, geopandas.GeoDataFrame) and
                 "geometry" in diversions.columns and
                 (~diversions_in_model.is_empty).all())
+            if is_spatial:
+                try:
+                    match_s = geopandas.sjoin_nearest(
+                        diversions_in_model, obj.grid_cells,
+                        "inner")[["index_right0", "index_right1"]].rename(
+                        columns={"index_right0": "i", "index_right1": "j"})
+                    match_s.index.name = "divid"
+                    match = match_s.reset_index()
+                    has_sjoin_nearest = True
+                except (AttributeError, NotImplementedError):
+                    has_sjoin_nearest = False
             for divn in diversions_in_model.itertuples():
                 # Use the last upstream reach as a template for a new reach
                 reach_d = dict(reaches.loc[
                     reaches.segnum == divn.from_segnum].iloc[-1])
                 reach_d.update({
                     "segnum": swn.END_SEGNUM,
                     "segndist": 0.0,
                     "diversion": True,
                     "divid": divn.Index,
                     "geometry": empty_geom,
                 })
                 # Assign one reach at grid cell
                 if is_spatial:
                     # Find grid cell nearest to diversion
-                    grid_cells = obj.grid_cells
-                    grid_sindex = get_sindex(grid_cells)
-                    if grid_sindex:
-                        bbox_match = sorted(
-                            grid_sindex.nearest(divn.geometry.bounds))
-                        # more than one nearest can exist! just take one...
-                        num_found = len(bbox_match)
-                        grid_cell = grid_cells.iloc[bbox_match[0]]
+                    if has_sjoin_nearest:
+                        sel = match["divid"] == divn.Index
+                        sel0_ij = tuple(match.loc[sel, ["i", "j"]].iloc[0])
+                        grid_cell = obj.grid_cells.loc[sel0_ij]
                     else:  # slow scan of all cells
-                        sel = grid_cells.intersects(divn.geometry)
-                        num_found = sel.sum()
-                        grid_cell = grid_cells.loc[sel].iloc[0]
+                        sel = obj.grid_cells.intersects(divn.geometry)
+                        # TODO: if it's outside, search nearest distance?
+                        grid_cell = obj.grid_cells.loc[sel].iloc[0]
+                    num_found = sel.sum()
                     if num_found > 1:
+                        # TODO: if non-point, consider using centroid
                         obj.logger.warning(
                             "%d grid cells are nearest to diversion %r, "
                             "but only taking the first %s",
                             num_found, divn.Index, grid_cell)
                     i, j = grid_cell.name
                     reach_d.update({"i": i, "j": j})
                     if not divn.geometry.is_empty:
@@ -929,15 +942,15 @@
         # keep "segndist" for interpolation from segment data
 
         # Add classic ISEG and IREACH, counting from 1
         reaches["iseg"] = 0
         reaches["ireach"] = 0
         iseg = ireach = 0
         prev_segnum = None
-        for idx, segnum in reaches.segnum.iteritems():
+        for idx, segnum in reaches.segnum.items():
             is_diversion = has_diversions and reaches.at[idx, "diversion"]
             if is_diversion:
                 if uses_segments:
                     # Each diversion gets a new segment/reach
                     iseg += 1
                 ireach = 0
             elif segnum != prev_segnum:
@@ -1077,15 +1090,15 @@
         elif self.__class__.__name__ == "SwnMf6":
             expected_shape = dis.nrow.data, dis.ncol.data
         else:
             raise TypeError(
                 f"unsupported subclass {self.__class__.__name__!r}")
         if expected_shape != array.shape:
             raise ValueError("'array' must have shape (nrow, ncol)")
-        self.reaches.loc[:, name] = array[self.reaches["i"], self.reaches["j"]]
+        self.reaches[name] = array[self.reaches["i"], self.reaches["j"]]
 
     def set_reach_slope(self, method: str = "auto", min_slope=1./1000):
         """Set slope for reaches.
 
         This method also adds/updates several attributes for reaches.
         The actual data is stored in "slope" for SwnModflow or
         "rgrd" for SwnMf6 classes.
@@ -1292,30 +1305,31 @@
             - zero-based cell index: k, i, j,
             - one-based reach index: iseg, ireach
             - dist_to_reach
 
         Examples
         --------
         >>> import flopy
+        >>> import geopandas
         >>> import pandas as pd
         >>> import swn
-        >>> lines = swn.spatial.wkt_to_geoseries([
+        >>> lines = geopandas.GeoSeries.from_wkt([
         ...    "LINESTRING (60 100, 60  80)",
         ...    "LINESTRING (40 130, 60 100)",
         ...    "LINESTRING (70 130, 60 100)"])
         >>> lines.index += 100
         >>> n = swn.SurfaceWaterNetwork.from_lines(lines)
         >>> sim = flopy.mf6.MFSimulation()
         >>> _ = flopy.mf6.ModflowTdis(sim, nper=1, time_units="days")
         >>> gwf = flopy.mf6.ModflowGwf(sim)
         >>> _ = flopy.mf6.ModflowGwfdis(
         ...     gwf, nrow=3, ncol=2, delr=20.0, delc=20.0, idomain=1,
         ...     length_units="meters", xorigin=30.0, yorigin=70.0)
         >>> nm = swn.SwnMf6.from_swn_flopy(n, gwf)
-        >>> obs_gs = swn.spatial.wkt_to_geoseries([
+        >>> obs_gs = geopandas.GeoSeries.from_wkt([
         ...    "POINT (56 103)",
         ...    "POINT (62 90)"])
         >>> obs_gs.index += 10
         >>> loc_df = n.locate_geoms(obs_gs)
         >>> r_df = nm.get_location_frame_reach_info(loc_df)
         >>> r_df
             rno  k  i  j  iseg  ireach  dist_to_reach
```

### Comparing `surface-water-network-0.5/swn/modflow/_legacy.py` & `surface-water-network-0.6/swn/modflow/_swnmf6.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,820 +1,252 @@
-# -*- coding: utf-8 -*-
-"""Interface for flopy's implementation for MODFLOW."""
+"""Interface for flopy's implementation for MODFLOW 6."""
 
-__all__ = ["MfSfrNetwork"]
+__all__ = [
+    "SwnMf6",
+]
 
-import pickle
-from itertools import combinations, zip_longest
-from textwrap import dedent
+import os
+from itertools import zip_longest
 
-import geopandas
 import numpy as np
 import pandas as pd
 from shapely import wkt
-from shapely.geometry import LineString, Point, Polygon, box
-from shapely.ops import linemerge
 
-from ..core import SurfaceWaterNetwork
-from ..spatial import compare_crs, get_sindex
+from ..compat import ignore_shapely_warnings_for_object_array
+from ..file import write_formatted_frame
 from ..util import abbr_str
+from ._base import SwnModflowBase
 
 try:
     import matplotlib
 except ImportError:
     matplotlib = False
 
 
-class MfSfrNetwork:
-    """MODFLOW SFR network class.
+class SwnMf6(SwnModflowBase):
+    """Surface water network adaptor for MODFLOW 6.
 
     Attributes
     ----------
-    model : flopy.modflow.mf.Modflow
-        Instance of a flopy MODFLOW model
+    swn : swn.SurfaceWaterNetwork
+        Instance of a SurfaceWaterNetwork.
+    model : flopy.mf6.ModflowGwf
+        Instance of flopy.mf6.ModflowGwf
     segments : geopandas.GeoDataFrame
         Copied from swn.segments, but with additional columns added
-    segment_data : pandas.DataFrame
-        Similar to structure in model.sfr.segment_data, but for one stress
-        period. Transient data (where applicable) will show summary statistics.
-        The index is 'nseg', ordered and starting from 1. An additional column
-        'segnum' is used to identify segments, and if defined,
-        abstraction/diversion identifiers, where iupseg != 0.
     reaches : geopandas.GeoDataFrame
-        Similar to structure in model.sfr.reach_data with index 'reachID',
+        Similar to structure in model.sfr.reaches with index "rno",
         ordered and starting from 1. Contains geometry and other columns
-        not used by flopy. Use get_reach_data() for use with flopy.
+        not used by flopy.
+    tsvar : dict
+        Dataframe of time-varying data for MODFLOW SFR, key is dataset name.
     diversions :  geopandas.GeoDataFrame, pd.DataFrame or None
         Copied from swn.diversions, if set/defined.
     logger : logging.Logger
         Logger to show messages.
 
     """
 
     def __init__(self, logger=None):
-        """Initialise MfSfrNetwork.
+        """Initialise SwnMf6.
 
         Parameters
         ----------
         logger : logging.Logger, optional
             Logger to show messages.
         """
-        from importlib.util import find_spec
-
-        from ..logger import get_logger, logging
-        if logger is None:
-            self.logger = get_logger(self.__class__.__name__)
-        elif isinstance(logger, logging.Logger):
-            self.logger = logger
-        else:
-            raise ValueError(
-                "expected 'logger' to be Logger; found " + str(type(logger)))
-        self.logger.warning(
-            "using legacy MfSfrNetwork; consider using SwnModflow")
-        self.logger.info('creating new %s object', self.__class__.__name__)
-        if not find_spec('flopy'):
-            raise ImportError(self.__class__.__name__ + ' requires flopy')
-        self.segments = None
-        self.segment_data = None
-        self.reaches = None
-        self.diversions = None
+        super().__init__(logger)
+        self.tsvar = {}  # time-varying data
         # all other properties added afterwards
 
     @classmethod
     def from_swn_flopy(
-            cls, swn, model, ibound_action='freeze',
-            reach_include_fraction=0.2, min_slope=1./1000,
-            hyd_cond1=1., hyd_cond_out=None, thickness1=1., thickness_out=None,
-            width1=10., width_out=None, roughch=0.024,
-            abstraction={}, inflow={}, flow={}, runoff={}, etsw={}, pptsw={}):
-        """Create a MODFLOW SFR structure from a surface water network.
+            cls, swn, model, idomain_action="freeze",
+            reach_include_fraction=0.2, diversion_downstream_bias=0.0):
+        """Create a MODFLOW 6 SFR structure from a surface water network.
 
         Parameters
         ----------
         swn : swn.SurfaceWaterNetwork
             Instance of a SurfaceWaterNetwork.
-        model : flopy.modflow.mf.Modflow
-            Instance of a flopy MODFLOW model with DIS and BAS6 packages.
-        ibound_action : str, optional
-            Action to handle IBOUND:
-                - ``freeze`` : Freeze IBOUND, but clip streams to fit bounds.
-                - ``modify`` : Modify IBOUND to fit streams, where possible.
+        model : flopy.mf6.ModflowGwf
+            Instance of a flopy MODFLOW 6 groundwater flow model.
+        idomain_action : str, optional
+            Action to handle IDOMAIN:
+                - ``freeze`` : Freeze IDOMAIN, but clip streams to fit bounds.
+                - ``modify`` : Modify IDOMAIN to fit streams, where possible.
         reach_include_fraction : float or pandas.Series, optional
             Fraction of cell size used as a threshold distance to determine if
             reaches outside the active grid should be included to a cell.
             Based on the furthest distance of the line and cell geometries.
             Default 0.2 (e.g. for a 100 m grid cell, this is 20 m).
-        min_slope : float or pandas.Series, optional
-            Minimum downwards slope imposed on segments. If float, then this is
-            a global value, otherwise it is per-segment with a Series.
-            Default 1./1000 (or 0.001).
-        hyd_cond1 : float or pandas.Series, optional
-            Hydraulic conductivity of the streambed, as a global or per top of
-            each segment. Used for either STRHC1 or HCOND1/HCOND2 outputs.
-            Default 1.
-        hyd_cond_out : None, float or pandas.Series, optional
-            Similar to thickness1, but for the hydraulic conductivity of each
-            segment outlet. If None (default), the same hyd_cond1 value for the
-            top of the outlet segment is used for the bottom.
-        thickness1 : float or pandas.Series, optional
-            Thickness of the streambed, as a global or per top of each segment.
-            Used for either STRTHICK or THICKM1/THICKM2 outputs. Default 1.
-        thickness_out : None, float or pandas.Series, optional
-            Similar to thickness1, but for the bottom of each segment outlet.
-            If None (default), the same thickness1 value for the top of the
-            outlet segment is used for the bottom.
-        width1 : float or pandas.Series, optional
-            Channel width, as a global or per top of each segment. Used for
-            WIDTH1/WIDTH2 outputs. Default 10.
-        width_out : None, float or pandas.Series, optional
-            Similar to width1, but for the bottom of each segment outlet.
-            If None (default), the same width1 value for the top of the
-            outlet segment is used for the bottom.
-        roughch : float or pandas.Series, optional
-            Manning's roughness coefficient for the channel. If float, then
-            this is a global value, otherwise it is per-segment with a Series.
-            Default 0.024.
-        abstraction : dict or pandas.DataFrame, optional
-            See generate_segment_data for details.
-            Default is {} (no abstraction from diversions).
-        inflow : dict or pandas.DataFrame, optional
-            See generate_segment_data for details.
-            Default is {} (no outside inflow added to flow term).
-        flow : dict or pandas.DataFrame, optional
-            See generate_segment_data. Default is {} (zero).
-        runoff : dict or pandas.DataFrame, optional
-            See generate_segment_data. Default is {} (zero).
-        etsw : dict or pandas.DataFrame, optional
-            See generate_segment_data. Default is {} (zero).
-        pptsw : dict or pandas.DataFrame, optional
-            See generate_segment_data. Default is {} (zero).
-        logger : logging.Logger, optional
-            Logger to show messages.
+        diversion_downstream_bias : float, default 0.0
+            A bias used for spatial location matching that increase the
+            likelihood of finding downstream reaches of a segnum if positive,
+            and upstream reaches if negative. Valid range is -1.0 to 1.0.
+            Default 0.0 is no bias, matching to the closest reach.
 
+        Returns
+        -------
+        obj : swn.SwnMf6 object
         """
-        obj = cls()
-        import flopy
-        if not isinstance(swn, SurfaceWaterNetwork):
-            raise ValueError('swn must be a SurfaceWaterNetwork object')
-        elif ibound_action not in ('freeze', 'modify'):
-            raise ValueError('ibound_action must be one of freeze or modify')
-        obj.model = model
-        obj.segments = swn.segments.copy()
-        # Make sure model CRS and segments CRS are the same (if defined)
-        crs = None
-        segments_crs = getattr(obj.segments.geometry, 'crs', None)
-        modelgrid_crs = None
-        modelgrid = obj.model.modelgrid
-        epsg = modelgrid.epsg
-        proj4_str = modelgrid.proj4
-        if epsg is not None:
-            segments_crs, modelgrid_crs, same = compare_crs(segments_crs, epsg)
+        if idomain_action not in ("freeze", "modify"):
+            raise ValueError("idomain_action must be one of freeze or modify")
+
+        obj = super().from_swn_flopy(
+            swn=swn, model=model, domain_action=idomain_action,
+            reach_include_fraction=reach_include_fraction)
+
+        # Evaluate connections, assume only converging network
+        to_segnums_d = swn.to_segnums.to_dict()
+        has_diversions = obj.diversions is not None
+        if has_diversions:
+            reaches_segnum_s = set(obj.reaches[~obj.reaches.diversion].segnum)
         else:
-            segments_crs, modelgrid_crs, same = compare_crs(segments_crs,
-                                                            proj4_str)
-        if (segments_crs is not None and modelgrid_crs is not None and
-                not same):
-            obj.logger.warning(
-                'CRS for segments and modelgrid are different: {0} vs. {1}'
-                .format(segments_crs, modelgrid_crs))
-        crs = segments_crs or modelgrid_crs
-        # Make sure their extents overlap
-        minx, maxx, miny, maxy = modelgrid.extent
-        model_bbox = box(minx, miny, maxx, maxy)
-        rstats = obj.segments.bounds.describe()
-        segments_bbox = box(
-                rstats.loc['min', 'minx'], rstats.loc['min', 'miny'],
-                rstats.loc['max', 'maxx'], rstats.loc['max', 'maxy'])
-        if model_bbox.disjoint(segments_bbox):
-            raise ValueError('modelgrid extent does not cover segments extent')
-        # More careful check of overlap of lines with grid polygons
-        obj.logger.debug('building model grid cell geometries')
-        dis = obj.model.dis
-        cols, rows = np.meshgrid(np.arange(dis.ncol), np.arange(dis.nrow))
-        ibound = obj.model.bas6.ibound[0].array.copy()
-        ibound_modified = 0
-        grid_df = pd.DataFrame({'row': rows.flatten(), 'col': cols.flatten()})
-        grid_df.set_index(['row', 'col'], inplace=True)
-        grid_df['ibound'] = ibound.flatten()
-        if ibound_action == 'freeze' and (ibound == 0).any():
-            # Remove any inactive grid cells from analysis
-            grid_df = grid_df.loc[grid_df['ibound'] != 0]
-        # Determine grid cell size
-        col_size = np.median(dis.delr.array)
-        if dis.delr.array.min() != dis.delr.array.max():
-            obj.logger.warning(
-                'assuming constant column spacing %s', col_size)
-        row_size = np.median(dis.delc.array)
-        if dis.delc.array.min() != dis.delc.array.max():
-            obj.logger.warning(
-                'assuming constant row spacing %s', row_size)
-        cell_size = (row_size + col_size) / 2.0
-        # Note: modelgrid.get_cell_vertices(row, col) is slow!
-        xv = modelgrid.xvertices
-        yv = modelgrid.yvertices
-        r, c = [np.array(s[1])
-                for s in grid_df.reset_index()[['row', 'col']].iteritems()]
-        cell_verts = zip(
-            zip(xv[r, c], yv[r, c]),
-            zip(xv[r, c + 1], yv[r, c + 1]),
-            zip(xv[r + 1, c + 1], yv[r + 1, c + 1]),
-            zip(xv[r + 1, c], yv[r + 1, c])
-        )
-        obj.grid_cells = grid_cells = geopandas.GeoDataFrame(
-            grid_df, geometry=[Polygon(r) for r in cell_verts], crs=crs)
-        obj.logger.debug('evaluating reach data on model grid')
-        grid_sindex = get_sindex(grid_cells)
-        reach_include = swn.segments_series(reach_include_fraction) * cell_size
-        # Make an empty DataFrame for reaches
-        obj.reaches = pd.DataFrame(columns=['geometry'])
-        obj.reaches.insert(1, column='row', value=pd.Series(dtype=int))
-        obj.reaches.insert(2, column='col', value=pd.Series(dtype=int))
-        empty_reach_df = obj.reaches.copy()  # take this before more added
-        obj.reaches.insert(
-            1, column='segnum',
-            value=pd.Series(dtype=obj.segments.index.dtype))
-        obj.reaches.insert(2, column='dist', value=pd.Series(dtype=float))
-        empty_reach_df.insert(3, column='length', value=pd.Series(dtype=float))
-        empty_reach_df.insert(4, column='moved', value=pd.Series(dtype=bool))
-
-        # recursive helper function
-        def append_reach_df(df, row, col, reach_geom, moved=False):
-            if reach_geom.geom_type == 'LineString':
-                df.loc[len(df.index)] = {
-                    'geometry': reach_geom,
-                    'row': row,
-                    'col': col,
-                    'length': reach_geom.length,
-                    'moved': moved,
-                }
-            elif reach_geom.geom_type.startswith('Multi'):
-                for sub_reach_geom in reach_geom.geoms:  # recurse
-                    append_reach_df(df, row, col, sub_reach_geom, moved)
-            else:
-                raise NotImplementedError(reach_geom.geom_type)
+            reaches_segnum_s = set(obj.reaches.segnum)
 
-        # helper function that returns early, if necessary
-        def assign_short_reach(reach_df, idx, segnum):
-            reach = reach_df.loc[idx]
-            reach_geom = reach['geometry']
-            threshold = reach_include[segnum]
-            if reach_geom.length > threshold:
-                return
-            cell_lengths = reach_df.groupby(['row', 'col'])['length'].sum()
-            this_row_col = reach['row'], reach['col']
-            this_cell_length = cell_lengths[this_row_col]
-            if this_cell_length > threshold:
-                return
-            grid_geom = grid_cells.at[(reach['row'], reach['col']), 'geometry']
-            # determine if it is crossing the grid once or twice
-            grid_points = reach_geom.intersection(grid_geom.exterior)
-            split_short = (
-                grid_points.geom_type == 'Point' or
-                (grid_points.geom_type == 'MultiPoint' and
-                 len(grid_points) == 2))
-            if not split_short:
-                return
-            matches = []
-            # sequence scan on reach_df
-            for oidx, orch in reach_df.iterrows():
-                if oidx == idx or orch['moved']:
-                    continue
-                other_row_col = orch['row'], orch['col']
-                other_cell_length = cell_lengths[other_row_col]
-                if (orch['geometry'].distance(reach_geom) < 1e-6 and
-                        this_cell_length < other_cell_length):
-                    matches.append((oidx, orch['geometry']))
-            if len(matches) == 0:
-                # don't merge, e.g. reach does not connect to adjacent cell
-                pass
-            elif len(matches) == 1:
-                # short segment is in one other cell only
-                # update new row and col values, keep geometry as it is
-                row_col1 = tuple(reach_df.loc[matches[0][0], ['row', 'col']])
-                reach_df.loc[idx, ['row', 'col', 'moved']] = row_col1 + (True,)
-                # self.logger.debug(
-                #    'moved short segment of %s from %s to %s',
-                #    segnum, this_row_col, row_col1)
-            elif len(matches) == 2:
-                assert grid_points.geom_type == 'MultiPoint', grid_points.wkt
-                if len(grid_points) != 2:
-                    obj.logger.critical(
-                        'expected 2 points, found %s', len(grid_points))
-                # Build a tiny DataFrame of coordinates for this reach
-                reach_c = pd.DataFrame({
-                    'pt': [Point(c) for c in reach_geom.coords[:]]
-                })
-                if len(reach_c) == 2:
-                    # If this is a simple line with two coords, split it
-                    reach_c.index = [0, 2]
-                    reach_c.loc[1] = {
-                        'pt': reach_geom.interpolate(0.5, normalized=True)}
-                    reach_c.sort_index(inplace=True)
-                    reach_geom = LineString(list(reach_c['pt']))  # rebuild
-                # first match assumed to be touching the start of the line
-                if reach_c.at[0, 'pt'].distance(matches[1][1]) < 1e-6:
-                    matches.reverse()
-                reach_c['d1'] = reach_c['pt'].apply(
-                                lambda p: p.distance(matches[0][1]))
-                reach_c['d2'] = reach_c['pt'].apply(
-                                lambda p: p.distance(matches[1][1]))
-                reach_c['dm'] = reach_c[['d1', 'd2']].min(1)
-                # try a simple split where distances switch
-                ds = reach_c['d1'] < reach_c['d2']
-                cidx = ds[ds].index[-1]
-                # ensure it's not the index of either end
-                if cidx == 0:
-                    cidx = 1
-                elif cidx == len(reach_c) - 1:
-                    cidx = len(reach_c) - 2
-                row1, col1 = list(reach_df.loc[matches[0][0], ['row', 'col']])
-                reach_geom1 = LineString(reach_geom.coords[:(cidx + 1)])
-                row2, col2 = list(reach_df.loc[matches[1][0], ['row', 'col']])
-                reach_geom2 = LineString(reach_geom.coords[cidx:])
-                # update the first, append the second
-                reach_df.loc[idx, ['row', 'col', 'length', 'moved']] = \
-                    (row1, col1, reach_geom1.length, True)
-                reach_df.at[idx, 'geometry'] = reach_geom1
-                append_reach_df(reach_df, row2, col2, reach_geom2, moved=True)
-                # self.logger.debug(
-                #   'split and moved short segment of %s from %s to %s and %s',
-                #   segnum, this_row_col, (row1, col1), (row2, col2))
-            else:
-                obj.logger.critical(
-                    'unhandled assign_short_reach case with %d matches: %s\n'
-                    '%s\n%s', len(matches), matches, reach, grid_points.wkt)
-
-        def assign_remaining_reach(reach_df, segnum, rem):
-            if rem.geom_type == 'LineString':
-                threshold = cell_size * 2.0
-                if rem.length > threshold:
-                    obj.logger.debug(
-                        'remaining line segment from %s too long to merge '
-                        '(%.1f > %.1f)', segnum, rem.length, threshold)
-                    return
-                # search full grid for other cells that could match
-                if grid_sindex:
-                    bbox_match = sorted(grid_sindex.intersection(rem.bounds))
-                    sub = grid_cells.geometry.iloc[bbox_match]
-                else:  # slow scan of all cells
-                    sub = grid_cells.geometry
-                assert len(sub) > 0, len(sub)
-                matches = []
-                for (row, col), grid_geom in sub.iteritems():
-                    if grid_geom.touches(rem):
-                        matches.append((row, col, grid_geom))
-                if len(matches) == 0:
-                    return
-                threshold = reach_include[segnum]
-                # Build a tiny DataFrame for just the remaining coordinates
-                rem_c = pd.DataFrame({
-                    'pt': [Point(c) for c in rem.coords[:]]
-                })
-                if len(matches) == 1:  # merge it with adjacent cell
-                    row, col, grid_geom = matches[0]
-                    mdist = rem_c['pt'].apply(
-                                    lambda p: grid_geom.distance(p)).max()
-                    if mdist > threshold:
-                        obj.logger.debug(
-                            'remaining line segment from %s too far away to '
-                            'merge (%.1f > %.1f)', segnum, mdist, threshold)
-                        return
-                    append_reach_df(reach_df, row, col, rem, moved=True)
-                elif len(matches) == 2:  # complex: need to split it
-                    if len(rem_c) == 2:
-                        # If this is a simple line with two coords, split it
-                        rem_c.index = [0, 2]
-                        rem_c.loc[1] = {
-                            'pt': rem.interpolate(0.5, normalized=True)}
-                        rem_c.sort_index(inplace=True)
-                        rem = LineString(list(rem_c['pt']))  # rebuild
-                    # first match assumed to be touching the start of the line
-                    if rem_c.at[0, 'pt'].touches(matches[1][2]):
-                        matches.reverse()
-                    rem_c['d1'] = rem_c['pt'].apply(
-                                    lambda p: p.distance(matches[0][2]))
-                    rem_c['d2'] = rem_c['pt'].apply(
-                                    lambda p: p.distance(matches[1][2]))
-                    rem_c['dm'] = rem_c[['d1', 'd2']].min(1)
-                    mdist = rem_c['dm'].max()
-                    if mdist > threshold:
-                        obj.logger.debug(
-                            'remaining line segment from %s too far away to '
-                            'merge (%.1f > %.1f)', segnum, mdist, threshold)
-                        return
-                    # try a simple split where distances switch
-                    ds = rem_c['d1'] < rem_c['d2']
-                    cidx = ds[ds].index[-1]
-                    # ensure it's not the index of either end
-                    if cidx == 0:
-                        cidx = 1
-                    elif cidx == len(rem_c) - 1:
-                        cidx = len(rem_c) - 2
-                    row, col = matches[0][0:2]
-                    rem1 = LineString(rem.coords[:(cidx + 1)])
-                    append_reach_df(reach_df, row, col, rem1, moved=True)
-                    row, col = matches[1][0:2]
-                    rem2 = LineString(rem.coords[cidx:])
-                    append_reach_df(reach_df, row, col, rem2, moved=True)
-                else:
-                    obj.logger.critical(
-                        'how does this happen? Segments from %d touching %d '
-                        'grid cells', segnum, len(matches))
-            elif rem.geom_type.startswith('Multi'):
-                for sub_rem_geom in rem.geoms:  # recurse
-                    assign_remaining_reach(reach_df, segnum, sub_rem_geom)
+        def find_next_rno(segnum):
+            if segnum in to_segnums_d:
+                to_segnum = to_segnums_d[segnum]
+                if to_segnum in reaches_segnum_s:
+                    sel = obj.reaches["segnum"] == to_segnum
+                    return obj.reaches[sel].index[0]
+                else:  # recurse downstream
+                    return find_next_rno(to_segnum)
             else:
-                raise NotImplementedError(rem.geom_type)
+                return 0
 
-        for segnum, line in obj.segments.geometry.iteritems():
-            remaining_line = line
-            if grid_sindex:
-                bbox_match = sorted(grid_sindex.intersection(line.bounds))
-                if not bbox_match:
-                    continue
-                sub = grid_cells.geometry.iloc[bbox_match]
-            else:  # slow scan of all cells
-                sub = grid_cells.geometry
-            # Find all intersections between segment and grid cells
-            reach_df = empty_reach_df.copy()
-            for (row, col), grid_geom in sub.iteritems():
-                reach_geom = grid_geom.intersection(line)
-                if reach_geom.is_empty or reach_geom.geom_type == 'Point':
-                    continue
-                remaining_line = remaining_line.difference(grid_geom)
-                append_reach_df(reach_df, row, col, reach_geom)
-            # Determine if any remaining portions of the line can be used
-            if line is not remaining_line and remaining_line.length > 0:
-                assign_remaining_reach(reach_df, segnum, remaining_line)
-            # Reassign short reaches to two or more adjacent grid cells
-            # starting with the shortest reach
-            reach_lengths = reach_df['length'].loc[
-                reach_df['length'] < reach_include[segnum]]
-            for idx in list(reach_lengths.sort_values().index):
-                assign_short_reach(reach_df, idx, segnum)
-            # Potentially merge a few reaches for each row/col of this segnum
-            drop_reach_ids = []
-            gb = reach_df.groupby(['row', 'col'])['geometry'].apply(list)
-            for (row, col), geoms in gb.copy().iteritems():
-                row_col = row, col
-                if len(geoms) > 1:
-                    geom = linemerge(geoms)
-                    if geom.geom_type == 'MultiLineString':
-                        # workaround for odd floating point issue
-                        geom = linemerge([wkt.loads(g.wkt) for g in geoms])
-                    if geom.geom_type == 'LineString':
-                        sel = ((reach_df['row'] == row) &
-                               (reach_df['col'] == col))
-                        drop_reach_ids += list(sel.index[sel])
-                        obj.logger.debug(
-                            'merging %d reaches for segnum %s at %s',
-                            sel.sum(), segnum, row_col)
-                        append_reach_df(reach_df, row, col, geom)
-                    elif any(a.distance(b) < 1e-6
-                             for a, b in combinations(geoms, 2)):
-                        obj.logger.warning(
-                            'failed to merge segnum %s at %s: %s',
-                            segnum, row_col, geom.wkt)
-                    # else: this is probably a meandering MultiLineString
-            if drop_reach_ids:
-                reach_df.drop(drop_reach_ids, axis=0, inplace=True)
-            # TODO: Some reaches match multiple cells if they share a border
-            # Add all reaches for this segment
-            for _, reach in reach_df.iterrows():
-                row, col, reach_geom = reach.loc[['row', 'col', 'geometry']]
-                if line.has_z:
-                    # intersection(line) does not preserve Z coords,
-                    # but line.interpolate(d) works as expected
-                    reach_geom = LineString(line.interpolate(
-                        line.project(Point(c))) for c in reach_geom.coords)
-                # Get a point from the middle of the reach_geom
-                reach_mid_pt = reach_geom.interpolate(0.5, normalized=True)
-                reach_record = {
-                    'geometry': reach_geom,
-                    'segnum': segnum,
-                    'dist': line.project(reach_mid_pt, normalized=True),
-                    'row': row,
-                    'col': col,
-                }
-                obj.reaches.loc[len(obj.reaches.index)] = reach_record
-                if ibound_action == 'modify' and ibound[row, col] == 0:
-                    ibound_modified += 1
-                    ibound[row, col] = 1
-
-        if ibound_action == 'modify':
-            if ibound_modified:
-                obj.logger.debug(
-                    'updating %d cells from IBOUND array for top layer',
-                    ibound_modified)
-                obj.model.bas6.ibound[0] = ibound
-                obj.reaches = obj.reaches.merge(
-                    grid_df[['ibound']],
-                    left_on=['row', 'col'], right_index=True)
-                obj.reaches.rename(
-                        columns={'ibound': 'prev_ibound'}, inplace=True)
+        def get_to_rno():
+            if segnum == next_segnum:
+                return next_rno
             else:
-                obj.reaches['prev_ibound'] = 1
+                return find_next_rno(segnum)
 
-        # Now convert from DataFrame to GeoDataFrame
-        obj.reaches = geopandas.GeoDataFrame(
-                obj.reaches, geometry='geometry', crs=crs)
-
-        # Assign segment data
-        obj.segments['min_slope'] = swn.segments_series(min_slope)
-        if (obj.segments['min_slope'] < 0.0).any():
-            raise ValueError('min_slope must be greater than zero')
-        # Column names common to segments and segment_data
-        segment_cols = [
-            'roughch',
-            'hcond1', 'thickm1', 'elevup', 'width1',
-            'hcond2', 'thickm2', 'elevdn', 'width2']
-        # Tidy any previous attempts
-        for col in segment_cols:
-            if col in obj.segments.columns:
-                del obj.segments[col]
-        # Combine pairs of series for each segment
-        more_segment_columns = pd.concat([
-            swn.pair_segments_frame(hyd_cond1, hyd_cond_out, 'hcond'),
-            swn.pair_segments_frame(thickness1, thickness_out, 'thickm'),
-            swn.pair_segments_frame(width1, width_out, name='width',
-                                    method="constant")
-        ], axis=1, copy=False)
-        for name, series in more_segment_columns.iteritems():
-            obj.segments[name] = series
-        obj.segments['roughch'] = swn.segments_series(roughch)
-        # Mark segments that are not used
-        obj.segments['in_model'] = True
-        outside_model = \
-            set(swn.segments.index).difference(obj.reaches['segnum'])
-        obj.segments.loc[list(outside_model), 'in_model'] = False
-        # Add information from segments
-        obj.reaches = obj.reaches.merge(
-            obj.segments[['sequence', 'min_slope']], 'left',
-            left_on='segnum', right_index=True)
-        obj.reaches.sort_values(['sequence', 'dist'], inplace=True)
-        # Interpolate segment properties to each reach
-        obj.reaches['strthick'] = 0.0
-        obj.reaches['strhc1'] = 0.0
-        for segnum, seg in obj.segments.iterrows():
-            sel = obj.reaches['segnum'] == segnum
-            if seg['thickm1'] == seg['thickm2']:
-                val = seg['thickm1']
-            else:  # linear interpolate to mid points
-                tk1 = seg['thickm1']
-                tk2 = seg['thickm2']
-                dtk = tk2 - tk1
-                val = dtk * obj.reaches.loc[sel, 'dist'] + tk1
-            obj.reaches.loc[sel, 'strthick'] = val
-            if seg['hcond1'] == seg['hcond2']:
-                val = seg['hcond1']
-            else:  # linear interpolate to mid points in log-10 space
-                lhc1 = np.log10(seg['hcond1'])
-                lhc2 = np.log10(seg['hcond2'])
-                dlhc = lhc2 - lhc1
-                val = 10 ** (dlhc * obj.reaches.loc[sel, 'dist'] + lhc1)
-            obj.reaches.loc[sel, 'strhc1'] = val
-        del obj.reaches['sequence']
-        del obj.reaches['dist']
-        # Use MODFLOW SFR dataset 2 terms ISEG and IREACH, counting from 1
-        obj.reaches['iseg'] = 0
-        obj.reaches['ireach'] = 0
-        iseg = ireach = 0
-        prev_segnum = None
-        for idx, segnum in obj.reaches['segnum'].iteritems():
-            if segnum != prev_segnum:
-                iseg += 1
-                ireach = 0
-            ireach += 1
-            obj.reaches.at[idx, 'iseg'] = iseg
-            obj.reaches.at[idx, 'ireach'] = ireach
-            prev_segnum = segnum
-        obj.reaches.reset_index(inplace=True, drop=True)
-        obj.reaches.index += 1  # flopy series starts at one
-        obj.reaches.index.name = 'reachID'
-        obj.reaches['rchlen'] = obj.reaches.geometry.length
-        obj.reaches['strtop'] = 0.0
-        obj.reaches['slope'] = 0.0
-        if swn.has_z:
-            for reachID, item in obj.reaches.iterrows():
-                geom = item.geometry
-                # Get Z from each end
-                z0 = geom.coords[0][2]
-                z1 = geom.coords[-1][2]
-                dz = z0 - z1
-                dx = geom.length
-                slope = dz / dx
-                obj.reaches.at[reachID, 'slope'] = slope
-                # Get strtop from LineString mid-point Z
-                zm = geom.interpolate(0.5, normalized=True).z
-                obj.reaches.at[reachID, 'strtop'] = zm
+        obj.reaches["to_rno"] = -1
+        if has_diversions:
+            segnum_iter = obj.reaches.loc[
+                ~obj.reaches.diversion, "segnum"].items()
         else:
-            r = obj.reaches['row'].values
-            c = obj.reaches['col'].values
-            # Estimate slope from top and grid spacing
-            px, py = np.gradient(dis.top.array, col_size, row_size)
-            grid_slope = np.sqrt(px ** 2 + py ** 2)
-            obj.reaches['slope'] = grid_slope[r, c]
-            # Get stream values from top of model
-            obj.reaches['strtop'] = dis.top.array[r, c]
-        # Enforce min_slope
-        sel = obj.reaches['slope'] < obj.reaches['min_slope']
-        if sel.any():
-            obj.logger.warning(
-                'enforcing min_slope for %d reaches (%.2f%%)',
-                sel.sum(), 100.0 * sel.sum() / len(sel))
-            obj.reaches.loc[sel, 'slope'] = obj.reaches.loc[sel, 'min_slope']
-        if not hasattr(obj.reaches.geometry, 'geom_type'):
-            # workaround needed for reaches.to_file()
-            obj.reaches.geometry.geom_type = obj.reaches.geom_type
-        # Build segment_data for Data Set 6
-        obj.segment_data = obj.reaches[['iseg', 'segnum']]\
-            .drop_duplicates().rename(columns={'iseg': 'nseg'})
-        # index changes from 'reachID', to 'segnum', to finally 'nseg'
-        segnum2nseg_d = obj.segment_data.set_index('segnum')['nseg'].to_dict()
-        obj.segment_data['icalc'] = 1  # assumption for all streams
-        obj.segment_data['outseg'] = obj.segment_data['segnum'].map(
-            lambda x: segnum2nseg_d.get(obj.segments.loc[x, 'to_segnum'], 0))
-        obj.segment_data['iupseg'] = 0  # handle diversions next
-        obj.segment_data['iprior'] = 0
-        obj.segment_data['flow'] = 0.0
-        obj.segment_data['runoff'] = 0.0
-        obj.segment_data['etsw'] = 0.0
-        obj.segment_data['pptsw'] = 0.0
-        # upper elevation from the first and last reachID items from reaches
-        obj.segment_data['elevup'] = \
-            obj.reaches.loc[obj.segment_data.index, 'strtop']
-        obj.segment_data['elevdn'] = obj.reaches.loc[
-            obj.reaches.groupby(['iseg']).ireach.idxmax().values,
-            'strtop'].values
-        obj.segment_data.set_index('segnum', drop=False, inplace=True)
-        # copy several columns over (except 'elevup' and 'elevdn', for now)
-        segment_cols.remove('elevup')
-        segment_cols.remove('elevdn')
-        obj.segment_data[segment_cols] = obj.segments[segment_cols]
-        # now use nseg as primary index, not reachID or segnum
-        obj.segment_data.set_index('nseg', inplace=True)
-        obj.segment_data.sort_index(inplace=True)
-        # Add diversions (i.e. SW takes)
-        if swn.diversions is not None:
-            obj.diversions = swn.diversions.copy()
-            # Mark diversions that are not used / outside model
-            obj.diversions['in_model'] = True
-            outside_model = []
-            # Add columns for ICALC=0
-            obj.segment_data['depth1'] = 0.0
-            obj.segment_data['depth2'] = 0.0
-            # workaround for coercion issue
-            obj.segment_data['foo'] = ''
-            is_spatial = (
-                isinstance(obj.diversions, geopandas.GeoDataFrame) and
-                'geometry' in obj.diversions.columns and
-                (~obj.diversions.is_empty).all())
-            if swn.has_z:
-                empty_geom = wkt.loads('linestring z empty')
-            else:
-                empty_geom = wkt.loads('linestring empty')
-            for divid, divn in obj.diversions.iterrows():
-                if divn.from_segnum not in segnum2nseg_d:
-                    # segnum does not exist -- segment is outside model
-                    outside_model.append(divid)
-                    continue
-                iupseg = segnum2nseg_d[divn.from_segnum]
-                assert iupseg != 0, iupseg
-                nseg = len(obj.segment_data) + 1
-                rchlen = 1.0  # length required
-                thickm = 1.0  # thickness required
-                hcond = 0.0  # don't allow GW exchange
-                seg_d = dict(obj.segment_data.loc[iupseg])
-                seg_d.update({  # index is nseg
-                    'segnum': divid,
-                    'icalc': 0,  # stream depth is specified
-                    'outseg': 0,
-                    'iupseg': iupseg,
-                    'iprior': 0,  # normal behaviour for SW takes
-                    'flow': 0.0,  # abstraction assigned later
-                    'runoff': 0.0,
-                    'etsw': 0.0,
-                    'pptsw': 0.0,
-                    'roughch': 0.0,  # not used
-                    'hcond1': hcond, 'hcond2': hcond,
-                    'thickm1': thickm, 'thickm2': thickm,
-                    'width1': 0.0, 'width2': 0.0,  # not used
-                })
-                # Use the last reach as a template to modify for new reach
-                reach_d = dict(obj.reaches.loc[
-                    obj.reaches.iseg == iupseg].iloc[-1])
+            segnum_iter = obj.reaches["segnum"].items()
+        rno, segnum = next(segnum_iter)
+        for next_rno, next_segnum in segnum_iter:
+            obj.reaches.at[rno, "to_rno"] = get_to_rno()
+            rno, segnum = next_rno, next_segnum
+        next_segnum = swn.END_SEGNUM
+        obj.reaches.at[rno, "to_rno"] = get_to_rno()
+        if has_diversions:
+            obj.reaches.loc[obj.reaches["diversion"], "to_rno"] = 0
+        assert obj.reaches.to_rno.min() >= 0
+
+        # Populate from_rnos set
+        obj.reaches["from_rnos"] = [set() for _ in range(len(obj.reaches))]
+        to_rnos = obj.reaches.loc[obj.reaches["to_rno"] > 0, "to_rno"]
+        for k, v in to_rnos.items():
+            obj.reaches.at[v, "from_rnos"].add(k)
+
+        # Refresh diversions if set
+        if has_diversions:
+            div_sel = obj.diversions["in_model"]
+            # populate (rno, idv) from their match to non-diversion reaches
+            diversions_in_model = obj.diversions[div_sel]
+            r_df = obj.get_location_frame_reach_info(
+                diversions_in_model.rename(columns={"from_segnum": "segnum"})[
+                    ["segnum", "seg_ndist"]],
+                downstream_bias=diversion_downstream_bias,
+                geom_loc_df=getattr(diversions_in_model, "geometry", None))
+            obj.diversions["rno"] = 0  # valid from 1
+            obj.diversions.loc[r_df.index, "rno"] = r_df.rno
+            # evaluate idv, which is betwen 1 and ndv
+            obj.diversions["idv"] = 0
+            obj.diversions.loc[div_sel, "idv"] = 1
+            rno_counts = obj.diversions[div_sel].groupby(
+                "rno").count()["in_model"]
+            for rno, count in rno_counts[rno_counts > 1].items():
+                obj.diversions.loc[obj.diversions["rno"] == rno, "idv"] = \
+                    obj.diversions.idv[obj.diversions["rno"] == rno].cumsum()
+            # cross-reference iconr to rno used as a reach
+            diversion_reaches = obj.reaches.loc[
+                obj.reaches.diversion].reset_index().set_index("divid")
+            obj.diversions["iconr"] = diversion_reaches["rno"]
+            # Also put data into reaches frame
+            obj.reaches["div_from_rno"] = 0
+            rdiv = obj.diversions.loc[div_sel, ["rno", "iconr"]].rename(
+                columns={"rno": "from_rno", "iconr": "rno"}
+                ).reset_index().set_index("rno")
+            obj.reaches.loc[rdiv.index, "div_from_rno"] = rdiv["from_rno"]
+            obj.reaches["div_to_rnos"] = \
+                [set() for _ in range(len(obj.reaches))]
+            to_rnos = obj.reaches.loc[
+                obj.reaches["div_from_rno"] > 0, "div_from_rno"]
+            for k, v in to_rnos.items():
+                obj.reaches.at[v, "div_to_rnos"].add(k)
+
+            # Workaround potential MODFLOW6 bug where diversions cannot attach
+            # to outlet reach, so add another reach
+            sel = (
+                (obj.reaches["to_rno"] == 0) & (~obj.reaches["diversion"]) &
+                (obj.reaches["div_to_rnos"].apply(len) > 0))
+            if sel.any() and "mask" not in obj.reaches.columns:
+                obj.reaches["mask"] = False
+                if swn.has_z:
+                    empty_geom = wkt.loads("linestring z empty")
+                else:
+                    empty_geom = wkt.loads("linestring empty")
+            for rno in sel[sel].index:
+                new_rno = len(obj.reaches) + 1
+                # Correction to this reach
+                obj.reaches.loc[rno, "to_rno"] = new_rno
+                # Use as template for new reach
+                reach_d = obj.reaches.loc[rno].to_dict()
                 reach_d.update({
-                    'segnum': divid,
-                    'iseg': nseg,
-                    'ireach': 1,
-                    'rchlen': rchlen,
-                    'min_slope': 0.0,
-                    'slope': 0.0,
-                    'strthick': thickm,
-                    'strhc1': hcond,
+                    "geometry": empty_geom,
+                    "mask": True,
+                    "ireach": reach_d["ireach"] + 1,
+                    "to_rno": 0,
+                    "from_rnos": {rno},
+                    "div_to_rnos": set(),
                 })
-                # Assign one reach at grid cell
-                if is_spatial:
-                    # Find grid cell nearest to diversion
-                    if grid_sindex:
-                        bbox_match = sorted(
-                            grid_sindex.nearest(divn.geometry.bounds))
-                        # more than one nearest can exist! just take one...
-                        num_found = len(bbox_match)
-                        grid_cell = grid_cells.iloc[bbox_match[0]]
-                    else:  # slow scan of all cells
-                        sel = grid_cells.intersects(divn.geometry)
-                        num_found = sel.sum()
-                        grid_cell = grid_cells.loc[sel].iloc[0]
-                    if num_found > 1:
-                        obj.logger.warning(
-                            '%d grid cells are nearest to diversion %r, '
-                            'but only taking the first %s',
-                            num_found, divid, grid_cell)
-                    row, col = grid_cell.name
-                    strtop = dis.top[row, col]
-                    reach_d.update({
-                        'geometry': empty_geom,  # divn.geometry,
-                        'row': row,
-                        'col': col,
-                        'strtop': strtop,
-                    })
-                else:
-                    strtop = dis.top[reach_d['row'], reach_d['col']]
-                    reach_d['strtop'] = strtop
-                    seg_d.update({
-                        'geometry': empty_geom,
-                        'elevup': strtop,
-                        'elevdn': strtop,
-                    })
-                depth = strtop + thickm
-                seg_d.update({'depth1': depth, 'depth2': depth})
-                obj.reaches.loc[len(obj.reaches) + 1] = reach_d
-                obj.segment_data.loc[nseg] = seg_d
-            if outside_model:
-                obj.diversions.loc[list(outside_model), 'in_model'] = False
-                obj.logger.debug(
-                    'added %d diversions, ignoring %d that did not connect to '
-                    'existing segments',
-                    obj.diversions['in_model'].sum(), len(outside_model))
-            else:
-                obj.logger.debug(
-                    'added all %d diversions', len(obj.diversions))
-            # end of coercion workaround
-            obj.segment_data.drop('foo', axis=1, inplace=True)
-        else:
-            obj.diversions = None
-        # Finally, add/rename a few columns to align with reach_data
-        obj.reaches.insert(2, column='k', value=0)
-        obj.reaches.insert(3, column='outreach', value=pd.Series(dtype=int))
-        obj.reaches.rename(columns={'row': 'i', 'col': 'j'}, inplace=True)
-        # Create flopy Sfr2 package
-        segment_data = obj.set_segment_data(
-            abstraction=abstraction, inflow=inflow,
-            flow=flow, runoff=runoff, etsw=etsw, pptsw=pptsw, return_dict=True)
-        reach_data = obj.get_reach_data()
-        flopy.modflow.mfsfr2.ModflowSfr2(
-            model=obj.model, reach_data=reach_data, segment_data=segment_data)
+                with ignore_shapely_warnings_for_object_array():
+                    obj.reaches.loc[new_rno] = reach_d
+
+        # Set 1.0 for most, 0.0 for head and diversion nodes
+        obj.reaches["ustrf"] = 1.0
+        zero_from_rnos = obj.reaches["from_rnos"].apply(len) == 0
+        obj.reaches.loc[zero_from_rnos, "ustrf"] = 0.0
+
         return obj
 
     def __repr__(self):
-        """Return string representation of MfSfrNetwork object."""
-        is_diversion = self.segment_data['iupseg'] != 0
-        segnum_l = list(self.segment_data.loc[~is_diversion, 'segnum'])
-        segments_line = str(len(segnum_l)) + ' from segments'
-        if set(segnum_l) != set(self.segments.index):
-            segments_line += ' ({:.0%} used)'.format(
-                len(segnum_l) / float(len(self.segments)))
-        segments_line += ': ' + abbr_str(segnum_l, 4)
-        if is_diversion.any() and self.diversions is not None:
-            divid_l = list(self.segment_data.loc[is_diversion, 'segnum'])
-            diversions_line = str(len(divid_l)) + ' from diversions'
-            if set(divid_l) != set(self.diversions.index):
-                diversions_line += ' ({:.0%} used)'.format(
-                    len(divid_l) / float(len(self.diversions)))
-            diversions_line += abbr_str(divid_l, 4)
+        """Return string representation of SwnModflow object."""
+        model = self.model
+        if model is None:
+            model_info = "model not set"
+            sp_info = "model not set"
         else:
-            diversions_line = 'no diversions'
-        nper = self.model.dis.nper
-        return dedent('''\
-            <{}: flopy {} {!r}
-              {} in reaches ({}): {}
-              {} in segment_data ({}): {}
-                {}
-                {}
-              {} stress period{} with perlen: {} />'''.format(
-            self.__class__.__name__, self.model.version, self.model.name,
-            len(self.reaches), self.reaches.index.name,
-            abbr_str(list(self.reaches.index), 4),
-            len(self.segment_data), self.segment_data.index.name,
-            abbr_str(list(self.segment_data.index), 4),
-            segments_line,
-            diversions_line,
-            nper, '' if nper == 1 else 's',
-            abbr_str(list(self.model.dis.perlen), 4)))
+            tdis = self.model.simulation.tdis
+            nper = tdis.nper.data
+            model_info = f"flopy {self.model.version} {self.model.name!r}"
+            sp_info = "{} stress period{} with perlen: {} {}".format(
+                nper, "" if nper == 1 else "s",
+                abbr_str(list(tdis.perioddata.array["perlen"]), 4),
+                tdis.time_units.data)
+        s = f"<{self.__class__.__name__}: {model_info}\n"
+        reaches = self.reaches
+        if reaches is not None:
+            s += "  {} in reaches ({}): {}\n".format(
+                len(reaches), reaches.index.name,
+                abbr_str(list(reaches.index), 4))
+        diversions = self.diversions
+        if diversions is not None:
+            diversions_in_model = self.diversions[self.diversions["in_model"]]
+            s += "  {} in diversions (iconr): {}\n".format(
+                len(diversions_in_model),
+                abbr_str(list(diversions_in_model.iconr), 4))
+        s += f"  {sp_info} />"
+        return s
 
     def __eq__(self, other):
         """Return true if objects are equal."""
         import flopy
         try:
             for (ak, av), (bk, bv) in zip_longest(iter(self), iter(other)):
                 if ak != bk:
@@ -826,1033 +258,1742 @@
                     return False
                 elif type(av) != type(bv):
                     return False
                 elif isinstance(av, pd.DataFrame):
                     pd.testing.assert_frame_equal(av, bv)
                 elif isinstance(av, pd.Series):
                     pd.testing.assert_series_equal(av, bv)
-                elif isinstance(av, flopy.modflow.mf.Modflow):
+                elif isinstance(av, flopy.mf6.MFModel):
                     # basic test
                     assert str(av) == str(bv)
                 else:
                     assert av == bv
             return True
         except (AssertionError, TypeError, ValueError):
             return False
 
     def __iter__(self):
         """Return object datasets with an iterator."""
-        yield "class", self.__class__.__name__
-        yield "segments", self.segments
-        yield "segment_data", self.segment_data
-        yield "reaches", self.reaches
-        yield "diversions", self.diversions
-        yield "model", self.model
-
-    def __getstate__(self):
-        """Serialize object attributes for pickle dumps."""
-        return dict(self)
+        yield from super().__iter__()
+        yield "tsvar", self.tsvar
 
     def __setstate__(self, state):
         """Set object attributes from pickle loads."""
-        if not isinstance(state, dict):
-            raise ValueError("expected 'dict'; found {!r}".format(type(state)))
-        elif "class" not in state:
-            raise KeyError("state does not have 'class' key")
-        elif state["class"] != self.__class__.__name__:
-            raise ValueError("expected state class {!r}; found {!r}"
-                             .format(state["class"], self.__class__.__name__))
-        self.__init__()
-        self.segments = state["segments"]
-        self.segment_data = state["segment_data"]
-        self.reaches = state["reaches"]
-        self.diversions = state["diversions"]
-        # Note: model must be set outsie of this method
-
-    @property
-    def model(self):
-        """Return flopy model object."""
-        try:
-            return getattr(self, '_model')
-        except AttributeError:
-            self.logger.error("'model' property not set")
+        super().__setstate__(state)
+        self.tsvar = state["tsvar"]
 
-    @model.setter
-    def model(self, model):
-        import flopy
-        if not isinstance(model, flopy.modflow.mf.Modflow):
-            raise ValueError(
-                "'model' must be a flopy Modflow object; found " +
-                str(type(model)))
-        elif not model.has_package('DIS'):
-            raise ValueError('DIS package required')
-        elif not model.has_package('BAS6'):
-            raise ValueError('BAS6 package required')
-        if getattr(self, '_model', None) is not model:
-            self.logger.info("swapping 'model' object")
-        self._model = model
-        # Build stress period DataFrame from modflow model
-        stress_df = pd.DataFrame({'perlen': self.model.dis.perlen.array})
-        modeltime = self.model.modeltime
-        stress_df['duration'] = pd.TimedeltaIndex(
-            stress_df['perlen'].cumsum(), modeltime.time_units)
-        stress_df['start'] = pd.to_datetime(modeltime.start_datetime)
-        stress_df['end'] = stress_df['duration'] + stress_df.at[0, 'start']
-        stress_df.loc[1:, 'start'] = stress_df['end'].iloc[:-1].values
-        self._stress_df = stress_df  # keep this for debugging
-        self.time_index = pd.DatetimeIndex(stress_df['start']).copy()
-        self.time_index.name = None
+    def _init_package_df(self, *, style, defcols_names, auxiliary):
+        """Return an initial DataFrame of PACKAGEDATA or STRESS_PERIOD_DATA."""
+        if auxiliary is not None:
+            if isinstance(auxiliary, str):
+                auxiliary = [auxiliary]
+            defcols_names += auxiliary
+        dat = pd.DataFrame(self.reaches.copy())
+        dat["idomain"] = \
+            self.model.dis.idomain.array[dat["k"], dat["i"], dat["j"]]
+        cellid_none = dat["idomain"] < 1
+        if "mask" in dat.columns:
+            cellid_none |= dat["mask"]
+        kij_l = list("kij")
+        if style == "native":
+            # Convert from zero-based to one-based notation
+            dat[kij_l] += 1
+            # use kij unstead of cellid
+            idx = defcols_names.index("cellid")
+            defcols_names[idx:idx + 1] = kij_l
+            # convert kij to str, and store NONE in k, if needed
+            dat[kij_l] = dat[kij_l].astype(str)
+            if cellid_none.any():
+                dat.loc[cellid_none, "k"] = "NONE"
+                dat.loc[cellid_none, ["i", "j"]] = ""
+        elif style == "flopy":
+            # make cellid into tuple
+            dat["cellid"] = dat[kij_l].to_records(index=False).tolist()
+            if cellid_none.any():
+                dat.loc[cellid_none, "cellid"] = "NONE"
+            # Convert rno from one-based to zero-based notation
+            dat.index -= 1
+        else:
+            raise ValueError("'style' must be either 'native' or 'flopy'")
+        return dat
+
+    def _final_package_df(self, what, dat, *, defcols_names, boundname):
+        """Return a final DataFrame of PACKAGEDATA or STRESS_PERIOD_DATA."""
+        if boundname is None:
+            boundname = "boundname" in dat.columns
+        if boundname:
+            defcols_names.append("boundname")
+            if (na := dat["boundname"].isna()).any():
+                dat.loc[~na, "boundname"] = \
+                    dat.loc[~na, "boundname"].astype(str)
+            else:
+                dat["boundname"] = dat["boundname"].astype(str)
+            # Check and enforce 40 character limit
+            sel = dat.boundname.str.len() > 40
+            if sel.any():
+                self.logger.warning(
+                    "clipping %d boundname entries to 40 character limit",
+                    sel.sum())
+                dat.loc[sel, "boundname"] = \
+                    dat.loc[sel, "boundname"].str.slice(stop=40)
+        # check missing columns
+        missing = []
+        for name in defcols_names:
+            if name not in dat.columns:
+                missing.append(name)
+        if missing:
+            missing_list = ", ".join(missing)
+            raise KeyError(f"missing {len(missing)} {what}: {missing_list}")
+        return dat.loc[:, defcols_names]
+
+    def packagedata_frame(
+            self, style: str, auxiliary: list = [], boundname=None):
+        """Return DataFrame of PACKAGEDATA for MODFLOW 6 SFR.
+
+        This DataFrame is derived from the reaches DataFrame.
+
+        Parameters
+        ----------
+        style : str
+            If "native", all indicies (including kij) use one-based notation.
+            Also use k,i,j columns (as str) rather than cellid.
+            If "flopy", all indices (including rno) use zero-based notation.
+            Also use cellid as a tuple.
+        auxiliary : str, list, optional
+            String or list of auxiliary variable names. Default [].
+        boundname : bool, optional
+            Default None will determine if "boundname" column is added if
+            available in reaches.columns.
 
-    def plot(self, column='iseg',
-             cmap='viridis_r', legend=False):
+        Returns
+        -------
+        DataFrame
+
+        See Also
+        --------
+        SwnMf6.write_packagedata : Write native file.
+        SwnMf6.flopy_packagedata : List of lists for flopy.
+
+        Examples
+        --------
+        >>> import flopy
+        >>> import geopandas
+        >>> import swn
+        >>> lines = geopandas.GeoSeries.from_wkt([
+        ...    "LINESTRING (60 100, 60  80)",
+        ...    "LINESTRING (40 130, 60 100)",
+        ...    "LINESTRING (70 130, 60 100)"])
+        >>> lines.index += 100
+        >>> n = swn.SurfaceWaterNetwork.from_lines(lines)
+        >>> sim = flopy.mf6.MFSimulation()
+        >>> _ = flopy.mf6.ModflowTdis(sim, nper=1, time_units="days")
+        >>> gwf = flopy.mf6.ModflowGwf(sim)
+        >>> _ = flopy.mf6.ModflowGwfdis(
+        ...     gwf, nrow=3, ncol=2, delr=20.0, delc=20.0, idomain=1,
+        ...     length_units="meters", xorigin=30.0, yorigin=70.0)
+        >>> nm = swn.SwnMf6.from_swn_flopy(n, gwf)
+        >>> nm.default_packagedata()
+        >>> nm.reaches["boundname"] = nm.reaches["segnum"]
+        >>> nm.reaches["aux1"] = 2.0 + nm.reaches.index / 10.0
+        >>> nm.packagedata_frame("native", auxiliary="aux1")
+             k  i  j       rlen  rwid   rgrd  ...    man  ncon  ustrf  ndv  aux1  boundname
+        rno                                   ...                                          
+        1    1  1  1  18.027756  10.0  0.001  ...  0.024     1    0.0    0   2.1        101
+        2    1  1  2   6.009252  10.0  0.001  ...  0.024     2    1.0    0   2.2        101
+        3    1  2  2  12.018504  10.0  0.001  ...  0.024     2    1.0    0   2.3        101
+        4    1  1  2  21.081851  10.0  0.001  ...  0.024     1    0.0    0   2.4        102
+        5    1  2  2  10.540926  10.0  0.001  ...  0.024     2    1.0    0   2.5        102
+        6    1  2  2  10.000000  10.0  0.001  ...  0.024     3    1.0    0   2.6        100
+        7    1  3  2  10.000000  10.0  0.001  ...  0.024     1    1.0    0   2.7        100
+        <BLANKLINE>
+        [7 rows x 15 columns]
+        >>> nm.packagedata_frame("flopy", boundname=False)
+                cellid       rlen  rwid   rgrd  rtp  rbth  rhk    man  ncon  ustrf  ndv
+        rno                                                                            
+        0    (0, 0, 0)  18.027756  10.0  0.001  1.0   1.0  1.0  0.024     1    0.0    0
+        1    (0, 0, 1)   6.009252  10.0  0.001  1.0   1.0  1.0  0.024     2    1.0    0
+        2    (0, 1, 1)  12.018504  10.0  0.001  1.0   1.0  1.0  0.024     2    1.0    0
+        3    (0, 0, 1)  21.081851  10.0  0.001  1.0   1.0  1.0  0.024     1    0.0    0
+        4    (0, 1, 1)  10.540926  10.0  0.001  1.0   1.0  1.0  0.024     2    1.0    0
+        5    (0, 1, 1)  10.000000  10.0  0.001  1.0   1.0  1.0  0.024     3    1.0    0
+        6    (0, 2, 1)  10.000000  10.0  0.001  1.0   1.0  1.0  0.024     1    1.0    0
+        """  # noqa
+        from flopy.mf6 import ModflowGwfsfr as Mf6Sfr
+        defcols_names = [dt[0] for dt in Mf6Sfr.packagedata.dtype(self.model)]
+        defcols_names.remove("rno")  # this is the index
+        dat = self._init_package_df(
+            style=style, defcols_names=defcols_names, auxiliary=auxiliary)
+        if "rlen" not in dat.columns:
+            dat.loc[:, "rlen"] = dat.geometry.length
+        dat["ncon"] = (
+            dat["from_rnos"].apply(len) +
+            (dat["to_rno"] > 0).astype(int)
+        )
+        dat["ndv"] = 0
+        if self.diversions is not None:
+            dat["ncon"] += (
+                dat["div_to_rnos"].apply(len) +
+                (dat["div_from_rno"] > 0).astype(int)
+            )
+            ndv = self.diversions[
+                self.diversions["in_model"]].groupby("rno").count().in_model
+            if style == "flopy":
+                ndv.index -= 1
+            dat.loc[ndv.index, "ndv"] = ndv
+        return self._final_package_df(
+            "packagedata reaches series", dat,
+            defcols_names=defcols_names, boundname=boundname)
+
+    def write_packagedata(
+            self, fname: str, auxiliary: list = [], boundname=None):
         """
-        Show map of reaches with inflow segments in royalblue.
+        Write PACKAGEDATA file for MODFLOW 6 SFR.
 
         Parameters
         ----------
-        column : str
-            Column from reaches to use with 'cmap'; default 'iseg'.
-            See also 'legend' to help interpret values.
-        cmap : str
-            Matplotlib color map; default 'viridis_r',
-        legend : bool
-            Show legend for 'column'; default False.
+        fname : str
+            Output file name.
+        auxiliary : str, list, optional
+            String or list of auxiliary variable names. Default [].
+        boundname : bool, optional
+            Default None will determine if "boundname" column is added if
+            available in reaches.columns.
 
         Returns
         -------
-        AxesSubplot
+        None
+
+        See Also
+        --------
+        swn.file.read_formatted_frame : Read formatted file as a DataFrame.
 
         """
-        import matplotlib.pyplot as plt
+        pn = self.packagedata_frame(
+            "native", auxiliary=auxiliary, boundname=boundname)
+        write_formatted_frame(pn, fname)
 
-        fig, ax = plt.subplots()
-        ax.set_aspect('equal')
+    def flopy_packagedata(self, auxiliary: list = [], boundname=None):
+        """Return list of lists for flopy.
 
-        self.reaches[~self.reaches.is_empty].plot(
-            column=column, label='reaches', legend=legend, ax=ax, cmap=cmap)
-
-        self.grid_cells.plot(ax=ax, color='whitesmoke', edgecolor='gainsboro')
-        # return ax
-
-        is_diversion = self.segment_data['iupseg'] != 0
-        outlet_sel = (self.segment_data['outseg'] == 0) & (~is_diversion)
-        outlet_points = self.reaches.loc[self.reaches['iseg'].isin(
-            self.segment_data.loc[outlet_sel].index), 'geometry']\
-            .apply(lambda g: Point(g.coords[-1]))
-        outlet_points.plot(
-            ax=ax, label='outlet', marker='o', color='navy')
-        if 'inflow_segnums' in self.segment_data.columns:
-            inflow_sel = ~self.segment_data['inflow_segnums'].isnull()
-            inflow_points = self.reaches.loc[self.reaches['iseg'].isin(
-                self.segment_data.loc[inflow_sel].index), 'geometry']\
-                .apply(lambda g: Point(g.coords[0]))
-            inflow_points.plot(
-                ax=ax, label='inflow points', marker='o', color='royalblue')
+        Parameters
+        ----------
+        auxiliary : str, list, optional
+            String or list of auxiliary variable names. Default [].
+        boundname : bool, optional
+            Default None will determine if "boundname" column is added if
+            available in reaches.columns.
 
-        return ax
+        Returns
+        -------
+        list
 
-    def get_reach_data(self):
-        """Return numpy.recarray for flopy's ModflowSfr2 reach_data.
+        """
+        df = self.packagedata_frame(
+            "flopy", auxiliary=auxiliary, boundname=boundname)
+        return [list(x) for x in df.itertuples()]
+
+    def connectiondata_series(self, style: str):
+        """Return Series of CONNECTIONDATA for MODFLOW 6 SFR.
 
         Parameters
         ----------
-        None
+        style : str
+            If "native", all indicies (including kij) use one-based notation.
+            If "flopy", all indices (including rno) use zero-based notation.
+        """
+        def nonzerolst(x, neg=False):
+            if neg:
+                return [-x] if x > 0 else []
+            else:
+                return [x] if x > 0 else []
+
+        if self.diversions is not None:
+            res = (
+                self.reaches["from_rnos"].apply(sorted) +
+                self.reaches["div_from_rno"].apply(nonzerolst, neg=False) +
+                self.reaches["to_rno"].apply(nonzerolst, neg=True) +
+                self.reaches["div_to_rnos"].apply(sorted).apply(
+                    lambda x: [-i for i in x])
+            )
+        else:
+            res = (
+                self.reaches["from_rnos"].apply(sorted) +
+                self.reaches["to_rno"].apply(nonzerolst, neg=True)
+            )
+
+        if style == "native":
+            # keep one-based notation, but convert list to str
+            return res
+        elif style == "flopy":
+            # Convert rno from one-based to zero-based notation
+            res.index -= 1
+            return res.apply(lambda x: [v - 1 if v > 0 else v + 1 for v in x])
+        else:
+            raise ValueError("'style' must be either 'native' or 'flopy'")
+
+    def write_connectiondata(self, fname: str):
+        """
+        Write CONNECTIONDATA file for MODFLOW 6 SFR.
+
+        Parameters
+        ----------
+        fname : str
+            Output file name.
 
         Returns
         -------
-        numpy.recarray
+        None
 
         """
-        from flopy.modflow.mfsfr2 import ModflowSfr2
+        cn = self.connectiondata_series("native")
+        icn = [f"ic{n+1}" for n in range(cn.apply(len).max())]
+        rowfmt = f"{{:>{len(str(cn.index.max()))}}} {{}}\n"
+        rnolen = 1 + len(str(len(self.reaches)))
+        cn = cn.apply(lambda x: " ".join(str(v).rjust(rnolen) for v in x))
+        with open(fname, "w") as f:
+            f.write(f"# rno {' '.join(icn)}\n")
+            for rno, ic in cn.items():
+                f.write(rowfmt.format(rno, ic))
+
+    def flopy_connectiondata(self):
+        """Return list of lists for flopy.
 
-        # Build reach_data for Data Set 2
-        reach_data_names = []
-        for name in ModflowSfr2.get_default_reach_dtype().names:
-            if name in self.reaches.columns:
-                reach_data_names.append(name)
-        reach_data = pd.DataFrame(self.reaches[reach_data_names])
-        return reach_data.to_records(index=True)
+        Returns
+        -------
+        list
 
-    def set_segment_data(self, abstraction={}, inflow={}, flow={}, runoff={},
-                         etsw={}, pptsw={}, return_dict=False):
         """
-        Set timeseries data in segment_data required for flopy's ModflowSfr2.
+        s = self.connectiondata_series("flopy")
+        return (s.index.to_series().apply(lambda x: list([x])) + s).to_list()
 
-        This method does two things:
+    def diversions_frame(self, style: str):
+        """Return DataFrame of DIVERSIONS for MODFLOW 6 SFR.
 
-            1. Updates sfr.segment_data, which is a dict of rec.array
-               for each stress period.
-            2. Updates summary statistics in segment_data if there are more
-               than one stress period, otherwise values are kept for one
-               stress period.
+        This DataFrame is derived from :py:attr:`diversions`.
 
-        Other stationary data members that are part of segment_data
-        (e.g. hcond1, elevup, etc.) are not modified.
+        Parameters
+        ----------
+        style : str
+            If "native", all indicies use one-based notation.
+            If "flopy", all indices use zero-based notation.
+
+        Returns
+        -------
+        DataFrame
+
+        See Also
+        --------
+        SwnMf6.write_diversions : Write native file.
+        SwnMf6.flopy_diversions : List of lists for flopy.
+
+        Examples
+        --------
+        >>> import flopy
+        >>> import geopandas
+        >>> import swn
+        >>> lines = geopandas.GeoSeries.from_wkt([
+        ...    "LINESTRING (60 100, 60  80)",
+        ...    "LINESTRING (40 130, 60 100)",
+        ...    "LINESTRING (70 130, 60 100)"])
+        >>> lines.index += 100
+        >>> n = swn.SurfaceWaterNetwork.from_lines(lines)
+        >>> diversions = geopandas.GeoSeries.from_wkt([
+        ...    "POINT (58 100)", "POINT (62 100)",
+        ...    "POINT (59 95)", "POINT (61 92)"]).to_frame("geometry")
+        >>> diversions.index += 11
+        >>> n.set_diversions(diversions)
+        >>> sim = flopy.mf6.MFSimulation()
+        >>> _ = flopy.mf6.ModflowTdis(sim, nper=1, time_units="days")
+        >>> gwf = flopy.mf6.ModflowGwf(sim)
+        >>> _ = flopy.mf6.ModflowGwfdis(
+        ...     gwf, nrow=3, ncol=2, delr=20.0, delc=20.0, idomain=1,
+        ...     length_units="meters", xorigin=30.0, yorigin=70.0)
+        >>> nm = swn.SwnMf6.from_swn_flopy(n, gwf)
+        >>> nm.diversions_frame("native")
+            rno  idv  iconr cprior
+        11    3    1      8   upto
+        12    5    1      9   upto
+        13    6    1     10   upto
+        14    6    2     11   upto
+        >>> nm.diversions_frame("flopy")
+            rno  idv  iconr cprior
+        11    2    0      7   upto
+        12    4    0      8   upto
+        13    5    0      9   upto
+        14    5    1     10   upto
+        """  # noqa
+        from flopy.mf6 import ModflowGwfsfr as Mf6Sfr
+        defcols_dtype = Mf6Sfr.diversions.empty(self.model).dtype
+        if self.diversions is None:
+            self.logger.warning("diversions not set")
+            return pd.DataFrame(np.recarray(0, dtype=defcols_dtype))
+        defcols_names = list(defcols_dtype.names)
+        dat = pd.DataFrame(self.diversions[self.diversions["in_model"]].copy())
+        if "cprior" not in dat.columns:
+            self.logger.info("diversions missing cprior; assuming UPTO")
+            dat["cprior"] = "upto"
+        # checking missing columns
+        div_columns = set(dat.columns)
+        missing = set(defcols_names).difference(div_columns)
+        if missing:
+            missing_l = []
+            for name in defcols_names:
+                if name not in div_columns:
+                    missing_l.append(name)
+            raise KeyError(
+                "missing {} diversions dataset(s): {}"
+                .format(len(missing_l), ", ".join(sorted(missing_l))))
+        if style == "native":
+            pass
+        elif style == "flopy":
+            # Convert rno from one-based to zero-based notation
+            dat[["rno", "idv", "iconr"]] -= 1
+        else:
+            raise ValueError("'style' must be either 'native' or 'flopy'")
+        return dat[defcols_names]
+
+    def write_diversions(self, fname: str):
+        """Write DIVERSIONS file for MODFLOW 6 SFR.
+
+        File can be used in a ``OPEN/CLOSE`` statement for a DIVERSIONS block,
+        which can be set with ``diversions={"filename": "diversions.dat"}`` in
+        :py:meth:`set_sfr_obj`.
+
+        This method is based on :py:meth:`diversions_frame`.
 
         Parameters
         ----------
-        abstraction : dict or pandas.DataFrame, optional
-            Surface water abstraction from diversions. Default is {} (zero).
-            Keys are matched to diversions index.
-        inflow : dict or pandas.DataFrame, optional
-            Streamflow at the bottom of each segment, which is used to to
-            determine the streamflow entering the upstream end of a segment if
-            it is not part of the SFR network. Internal flows are ignored.
-            A dict can be used to provide constant values to segnum
-            identifiers. If a DataFrame is passed for a model with more than
-            one stress period, the index must be a DatetimeIndex aligned with
-            the start of each model stress period.
-            Default is {} (no outside inflow added to flow term).
-        flow : dict or pandas.DataFrame, optional
-            Flow to the top of each segment. This is added to any inflow,
-            which is handled separately. This can be negative for withdrawls.
-            Default is {} (zero).
-        runoff : dict or pandas.DataFrame, optional
-            Runoff to each segment. Default is {} (zero).
-        etsw : dict or pandas.DataFrame, optional
-            Evapotranspiration removed from each segment. Default is {} (zero).
-        pptsw : dict or pandas.DataFrame, optional
-            Precipitation added to each segment. Default is {} (zero).
-        return_dict : bool, optional
-            If True, return segment_data instead of setting the sfr object.
-            Default False, which implies that an sfr object exists.
+        fname : str
+            Output file name.
+
+        See Also
+        --------
+        swn.file.read_formatted_frame : Read formatted file as a DataFrame.
+        """
+        dat = self.diversions_frame("native")
+        write_formatted_frame(dat, fname, index=False)
+
+    def flopy_diversions(self):
+        """Return list of lists for flopy.
+
+        This method is based on :py:meth:`diversions_frame`.
 
         Returns
         -------
-        None or dict (if return_dict is True)
+        list
 
         """
-        from flopy.modflow.mfsfr2 import ModflowSfr2
+        dat = self.diversions_frame("flopy")
+        return [list(x) for x in dat.itertuples(index=False)]
 
-        # Build stress period DataFrame from modflow model
-        dis = self.model.dis
-        stress_df = pd.DataFrame({'perlen': dis.perlen.array})
-        modeltime = self.model.modeltime
-        stress_df['duration'] = pd.TimedeltaIndex(
-                stress_df['perlen'].cumsum(), modeltime.time_units)
-        stress_df['start'] = pd.to_datetime(modeltime.start_datetime)
-        stress_df['end'] = stress_df['duration'] + stress_df.at[0, 'start']
-        stress_df.loc[1:, 'start'] = stress_df['end'].iloc[:-1].values
-        # Consider all IDs from segments/diversions
-        segments_segnums = set(self.segments.index)
-        has_diversions = self.diversions is not None
-        if has_diversions:
-            diversions_divids = set(self.diversions.index)
-        else:
-            diversions_divids = set()
+    def package_period_frame(
+            self, package: str, style: str, auxiliary: list = [],
+            boundname=None):
+        """Return DataFrame of PERIOD data for MODFLOW 6 packages.
 
-        def check_ts(data, name):
-            """Return DataFrame with index along nper.
+        This DataFrame is derived from the reaches DataFrame, and is
+        implemented using flopy.mf6 package's ``stress_period_data``.
 
-            Columns are either segnum or divid (checked later).
-            """
-            if isinstance(data, dict):
-                data = pd.DataFrame(data, index=stress_df['start'])
-            elif not isinstance(data, pd.DataFrame):
-                raise ValueError(
-                    '{0} must be a dict or DataFrame'.format(name))
-            data.index.name = name  # handy for debugging
-            if len(data) != dis.nper:
-                raise ValueError(
-                    'length of {0} ({1}) is different than nper ({2})'
-                    .format(name, len(data), dis.nper))
-            if dis.nper > 1:  # check DatetimeIndex
-                if not isinstance(data.index, pd.DatetimeIndex):
-                    raise ValueError(
-                        '{0}.index must be a pandas.DatetimeIndex'
-                        .format(name))
-                elif not (data.index == stress_df['start']).all():
-                    try:
-                        t = stress_df['start'].to_string(
-                                index=False, max_rows=5).replace('\n', ', ')
-                    except TypeError:
-                        t = abbr_str(list(stress_df['start']))
-                    raise ValueError(
-                        '{0}.index does not match expected ({1})'
-                        .format(name, t))
-            # Also do basic check of column IDs against diversions/segments
-            if name == 'abstraction':
-                if not has_diversions:
-                    if len(data.columns) > 0:
-                        self.logger.error(
-                            'abstraction provided, but diversions are not '
-                            'defined for the surface water network')
-                        data.drop(data.columns, axis=1, inplace=True)
-                    return data
-                parent = self.diversions
-                parent_name = 'diversions'
-                parent_s = diversions_divids
-            else:
-                parent = self.segments
-                parent_name = 'segments'
-                parent_s = segments_segnums
-            try:
-                data.columns = data.columns.astype(parent.index.dtype)
-            except (ValueError, TypeError):
-                raise ValueError(
-                    '{0}.columns.dtype must be same as {1}.index.dtype'
-                    .format(name, parent_name))
-            data_id_s = set(data.columns)
-            if len(data_id_s) > 0:
-                if data_id_s.isdisjoint(parent_s):
-                    msg = '{0}.columns (or keys) not found in {1}.index: {2}'\
-                        .format(name, parent_name, abbr_str(data_id_s))
-                    if name == 'inflow':
-                        self.logger.warning(msg)
-                    else:
-                        raise ValueError(msg)
-                if name != 'inflow':  # some segnums accumulate outside flow
-                    not_found = data_id_s.difference(parent_s)
-                    if not data_id_s.issubset(parent_s):
-                        self.logger.warning(
-                            'dropping %s of %s %s.columns, which are '
-                            'not found in %s.index: %s',
-                            len(not_found), len(data_id_s), name,
-                            parent_name, abbr_str(data_id_s))
-                        data.drop(not_found, axis=1, inplace=True)
-            return data
-
-        self.logger.debug('checking timeseries data against modflow model')
-        abstraction = check_ts(abstraction, 'abstraction')
-        inflow = check_ts(inflow, 'inflow')
-        flow = check_ts(flow, 'flow')
-        runoff = check_ts(runoff, 'runoff')
-        etsw = check_ts(etsw, 'etsw')
-        pptsw = check_ts(pptsw, 'pptsw')
-
-        # Translate segnum/divid to nseg
-        is_diversion = self.segment_data['iupseg'] != 0
-        divid2nseg = self.segment_data[is_diversion]\
-            .reset_index().set_index('segnum')['nseg']
-        divid2nseg_d = divid2nseg.to_dict()
-        segnum2nseg = self.segment_data[~is_diversion]\
-            .reset_index().set_index('segnum')['nseg']
-        segnum2nseg_d = segnum2nseg.to_dict()
-        segnum_s = set(segnum2nseg_d.keys())
-
-        def map_nseg(data, name):
-            data_id_s = set(data.columns)
-            if len(data_id_s) == 0:
-                return data
-            if name == 'abstraction':
-                colid2nseg_d = divid2nseg_d
-                parent_descr = 'diversions'
-            else:
-                colid2nseg_d = segnum2nseg_d
-                parent_descr = 'regular segments'
-            colid_s = set(colid2nseg_d.keys())
-            not_found = data_id_s.difference(colid_s)
-            if not data_id_s.issubset(colid_s):
-                self.logger.warning(
-                    'dropping %s of %s %s.columns, which are '
-                    'not found in segment_data.index for %s',
-                    len(not_found), len(data_id_s), name,
-                    parent_descr)
-                data.drop(not_found, axis=1, inplace=True)
-            return data.rename(columns=colid2nseg_d)
-
-        self.logger.debug('mapping segnum/divid to segment_data.index (nseg)')
-        abstraction = map_nseg(abstraction, 'abstraction')
-        flow = map_nseg(flow, 'flow')
-        runoff = map_nseg(runoff, 'runoff')
-        etsw = map_nseg(etsw, 'etsw')
-        pptsw = map_nseg(pptsw, 'pptsw')
-
-        self.logger.debug('accumulating inflow from outside network')
-        # Create an 'inflows' DataFrame calculated from combining 'inflow'
-        inflows = pd.DataFrame(index=inflow.index)
-        has_inflow = len(inflow.columns) > 0
-        missing_inflow_segnums = []
-        if has_inflow:
-            self.segment_data['inflow_segnums'] = None
-        elif 'inflow_segnums' in self.segment_data:
-            self.segment_data.drop('inflow_segnums', axis=1, inplace=True)
-        # Determine upstream flows needed for each SFR segment
-        for segnum in self.segment_data.loc[~is_diversion, 'segnum']:
-            nseg = segnum2nseg_d[segnum]
-            from_segnums = self.segments.at[segnum, 'from_segnums']
-            if not from_segnums:
-                continue
-            # gather segments outside SFR network
-            outside_segnums = from_segnums.difference(segnum_s)
-            if not outside_segnums:
-                continue
-            if has_inflow:
-                inflow_series = pd.Series(0.0, index=inflow.index)
-                inflow_segnums = set()
-                for from_segnum in outside_segnums:
-                    try:
-                        inflow_series += inflow[from_segnum]
-                        inflow_segnums.add(from_segnum)
-                    except KeyError:
-                        self.logger.warning(
-                            'flow from segment %s not provided by inflow term '
-                            '(needed for %s)', from_segnum, segnum)
-                        missing_inflow_segnums.append(from_segnum)
-                if inflow_segnums:
-                    inflows[nseg] = inflow_series
-                    self.segment_data.at[nseg, 'inflow_segnums'] = \
-                        inflow_segnums
-            else:
-                missing_inflow_segnums += outside_segnums
-        if not has_inflow and len(missing_inflow_segnums) > 0:
+        Parameters
+        ----------
+        package : str
+            MODFLOW 6 package name, such as "drn" for DRAIN, or "GWT/SRC" for
+            Mass Source Loading.
+        style : str
+            If "native", all indicies (including kij) use one-based notation.
+            Also use k,i,j columns (as str) rather than cellid.
+            If "flopy", all indices (including rno) use zero-based notation.
+            Also use cellid as a tuple.
+        auxiliary : str, list, optional
+            String or list of auxiliary variable names. Default [].
+        boundname : bool, optional
+            Default None will determine if "boundname" column is added if
+            available in reaches.columns.
+
+        Returns
+        -------
+        DataFrame
+
+        See Also
+        --------
+        SwnMf6.write_package_period : Write native file.
+        SwnMf6.flopy_package_period : Dict of lists of lists for flopy.
+
+        Examples
+        --------
+        >>> import flopy
+        >>> import geopandas
+        >>> import swn
+        >>> lines = geopandas.GeoSeries.from_wkt([
+        ...    "LINESTRING (60 100, 60  80)",
+        ...    "LINESTRING (40 130, 60 100)",
+        ...    "LINESTRING (70 130, 60 100)"])
+        >>> lines.index += 100
+        >>> n = swn.SurfaceWaterNetwork.from_lines(lines)
+        >>> sim = flopy.mf6.MFSimulation()
+        >>> _ = flopy.mf6.ModflowTdis(sim, nper=1, time_units="days")
+        >>> gwf = flopy.mf6.ModflowGwf(sim)
+        >>> _ = flopy.mf6.ModflowGwfdis(
+        ...     gwf, nrow=3, ncol=2, delr=20.0, delc=20.0, top=10, botm=0,
+        ...     idomain=1, length_units="meters", xorigin=30.0, yorigin=70.0)
+        >>> nm = swn.SwnMf6.from_swn_flopy(n, gwf)
+        >>> nm.set_reach_data_from_array("elev", gwf.dis.top.array)
+        >>> nm.reaches["dlen"] = nm.reaches.length
+        >>> nm.reaches["cond"] = nm.reaches.dlen * 10.0
+        >>> nm.reaches["boundname"] = nm.reaches["segnum"]
+        >>> nm.package_period_frame("drn", "native", auxiliary="dlen")
+                 k  i  j  elev        cond       dlen boundname
+        per rno                                                
+        1   1    1  1  1  10.0  180.277564  18.027756       101
+            2    1  1  2  10.0   60.092521   6.009252       101
+            3    1  2  2  10.0  120.185043  12.018504       101
+            4    1  1  2  10.0  210.818511  21.081851       102
+            5    1  2  2  10.0  105.409255  10.540926       102
+            6    1  2  2  10.0  100.000000  10.000000       100
+            7    1  3  2  10.0  100.000000  10.000000       100
+        >>> nm.package_period_frame("drn","flopy", boundname=False)
+                    cellid  elev        cond
+        per rno                             
+        0   0    (0, 0, 0)  10.0  180.277564
+            1    (0, 0, 1)  10.0   60.092521
+            2    (0, 1, 1)  10.0  120.185043
+            3    (0, 0, 1)  10.0  210.818511
+            4    (0, 1, 1)  10.0  105.409255
+            5    (0, 1, 1)  10.0  100.000000
+            6    (0, 2, 1)  10.0  100.000000
+        """  # noqa
+        Mf6pak = get_flopy_mf6_package(package)
+        lst_tpl = Mf6pak.stress_period_data
+        defcols_names = [dt[0] for dt in lst_tpl.dtype(self.model)]
+        dat = self._init_package_df(
+            style=style, defcols_names=defcols_names, auxiliary=auxiliary)
+        dat = self._final_package_df(
+            f"{Mf6pak.__name__} reaches series", dat,
+            defcols_names=defcols_names, boundname=boundname)
+        if self.model.simulation.tdis.nper.data != 1:
             self.logger.warning(
-                'inflow from %d segnums are needed to determine flow from '
-                'outside SFR network: %s', len(missing_inflow_segnums),
-                abbr_str(missing_inflow_segnums))
-        # Append extra columns to segment_data that are used by flopy
-        segment_column_names = []
-        nss = len(self.segment_data)
-        for name, dtype in ModflowSfr2.get_default_segment_dtype().descr:
-            if name == 'nseg':  # skip adding the index
-                continue
-            segment_column_names.append(name)
-            if name not in self.segment_data.columns:
-                self.segment_data[name] = np.zeros(nss, dtype=dtype)
-        # Re-assmble stress period dict for flopy, with iper keys
-        segment_data = {}
-        has_abstraction = len(abstraction.columns) > 0
-        has_inflows = len(inflows.columns) > 0
-        has_flow = len(flow.columns) > 0
-        has_runoff = len(runoff.columns) > 0
-        has_etsw = len(etsw.columns) > 0
-        has_pptsw = len(pptsw.columns) > 0
-        for iper in range(dis.nper):
-            # Store data for each stress period
-            self.segment_data['flow'] = 0.0
-            self.segment_data['runoff'] = 0.0
-            self.segment_data['etsw'] = 0.0
-            self.segment_data['pptsw'] = 0.0
-            if has_abstraction:
-                item = abstraction.iloc[iper]
-                self.segment_data.loc[item.index, 'flow'] = item
-            if has_inflows:
-                item = inflows.iloc[iper]
-                self.segment_data.loc[item.index, 'flow'] += item
-            if has_flow:
-                item = flow.iloc[iper]
-                self.segment_data.loc[item.index, 'flow'] += item
-            if has_runoff:
-                item = runoff.iloc[iper]
-                self.segment_data.loc[item.index, 'runoff'] = item
-            if has_etsw:
-                item = etsw.iloc[iper]
-                self.segment_data.loc[item.index, 'etsw'] = item
-            if has_pptsw:
-                item = pptsw.iloc[iper]
-                self.segment_data.loc[item.index, 'pptsw'] = item
-            segment_data[iper] = self.segment_data[segment_column_names]\
-                .to_records(index=True)  # index is nseg
-
-        # For models with more than one stress period, evaluate summary stats
-        if dis.nper > 1:
-            # Remove time-varying data from last stress period
-            self.segment_data.drop(
-                ['flow', 'runoff', 'etsw', 'pptsw'], axis=1, inplace=True)
-
-            def add_summary_stats(name, df):
-                if len(df.columns) == 0:
-                    return
-                self.segment_data[name + '_min'] = 0.0
-                self.segment_data[name + '_mean'] = 0.0
-                self.segment_data[name + '_max'] = 0.0
-                min_v = df.min(0)
-                mean_v = df.mean(0)
-                max_v = df.max(0)
-                self.segment_data.loc[min_v.index, name + '_min'] = min_v
-                self.segment_data.loc[mean_v.index, name + '_mean'] = mean_v
-                self.segment_data.loc[max_v.index, name + '_max'] = max_v
-
-            add_summary_stats('abstraction', abstraction)
-            add_summary_stats('inflow', inflows)
-            add_summary_stats('flow', flow)
-            add_summary_stats('runoff', runoff)
-            add_summary_stats('etsw', etsw)
-            add_summary_stats('pptsw', pptsw)
+                "only preparing PERIOD data for the first stress period of %s",
+                self.model.simulation.tdis.nper.data)
+        dat["per"] = 1
+        if style == "flopy":
+            dat["per"] -= 1
+        return dat.reset_index().set_index(["per", "rno"])
+
+    def write_package_period(
+            self, package: str, fname, auxiliary: list = [],
+            boundname=None):
+        """
+        Write PERIOD file for MODFLOW 6 packages, to be used within OPEN/CLOSE.
 
-        if return_dict:
-            return segment_data
-        else:
-            self.model.sfr.segment_data = segment_data
+        Parameters
+        ----------
+        package : str
+            MODFLOW 6 package name, such as "drn" for DRAIN, or "GWT/SRC" for
+            Mass Source Loading.
+        fname : str or path-like
+            Output file name, with str formatting for stress period number
+            which starts numbering from 1. For example, "drn_sp{:02d}.txt" to
+            create "drn_sp01.txt" for the first stress period.
+        auxiliary : str, list, optional
+            String or list of auxiliary variable names. Default [].
+        boundname : bool, optional
+            Default None will determine if "boundname" column is added if
+            available in reaches.columns.
 
-    def get_seg_ijk(self):
-        """Get the upstream and downstream segment k,i,j."""
-        topidx = self.reaches['ireach'] == 1
-        kij_df = self.reaches[topidx][['iseg', 'k', 'i', 'j']].sort_values(
-            'iseg')
-        idx_name = self.segment_data.index.name or 'index'
-        self.segment_data = self.segment_data.reset_index().merge(
-            kij_df, left_on='nseg', right_on='iseg', how='left').drop(
-            'iseg', axis=1).set_index(idx_name)
-        self.segment_data.rename(
-            columns={"k": "k_up", "i": "i_up", "j": "j_up"}, inplace=True)
-        # seg bottoms
-        btmidx = self.reaches.groupby('iseg')['ireach'].transform(max) == \
-            self.reaches['ireach']
-        kij_df = self.reaches[btmidx][['iseg', 'k', 'i', 'j']].sort_values(
-            'iseg')
-
-        self.segment_data = self.segment_data.reset_index().merge(
-            kij_df, left_on='nseg', right_on='iseg', how='left').drop(
-            'iseg', axis=1).set_index(idx_name)
-        self.segment_data.rename(
-            columns={"k": "k_dn", "i": "i_dn", "j": "j_dn"}, inplace=True)
-        return self.segment_data[[
-            "k_up", "i_up", "j_up", "k_dn", "i_dn", "j_dn"]]
-
-    def get_top_elevs_at_segs(self, m=None):
-        """
-        Get topsurface elevations associated with segment up and dn elevations.
-
-        Adds elevation of model top at
-        upstream and downstream ends of each segment
-        :param m: modflow model with active dis package
-        :return: Adds 'top_up' and 'top_dn' columns to segment data dataframe
-        """
-        if m is None:
-            m = self.model
-        assert m.sfr is not None, "need sfr package"
-        self.segment_data['top_up'] = m.dis.top.array[
-            tuple(self.segment_data[['i_up', 'j_up']].values.T)]
-        self.segment_data['top_dn'] = m.dis.top.array[
-            tuple(self.segment_data[['i_dn', 'j_dn']].values.T)]
-        return self.segment_data[['top_up', 'top_dn']]
-
-    def get_segment_incision(self):
-        """
-        Calculate the upstream and downstream incision of the segment.
-
-        :return:
-        """
-        self.segment_data['diff_up'] = (self.segment_data['top_up'] -
-                                        self.segment_data['elevup'])
-        self.segment_data['diff_dn'] = (self.segment_data['top_dn'] -
-                                        self.segment_data['elevdn'])
-        return self.segment_data[['diff_up', 'diff_dn']]
-
-    def set_seg_minincise(self, minincise=0.2, max_str_z=None):
-        """
-        Set segment elevation to have the minimum incision from the top.
-
-        :param minincise: Desired minimum incision
-        :param max_str_z: Optional parameter to prevent streams at
-        high elevations (forces incision to max_str_z)
-        :return: incisions at the upstream and downstream end of each segment
-        """
-        sel = self.segment_data['diff_up'] < minincise
-        self.segment_data.loc[sel, 'elevup'] = (self.segment_data.loc[
-                                                    sel, 'top_up'] - minincise)
-        sel = self.segment_data['diff_dn'] < minincise
-        self.segment_data.loc[sel, 'elevdn'] = (self.segment_data.loc[
-                                                    sel, 'top_dn'] - minincise)
-        if max_str_z is not None:
-            sel = self.segment_data['elevup'] > max_str_z
-            self.segment_data.loc[sel, 'elevup'] = max_str_z
-            sel = self.segment_data['elevdn'] > max_str_z
-            self.segment_data.loc[sel, 'elevdn'] = max_str_z
-        # recalculate incisions
-        updown_incision = self.get_segment_incision()
-        return updown_incision
-
-    def get_segment_length(self):
-        """
-        Get segment length from accumulated reach lengths.
-
-        :return:
-        """
-        # extract segment length for calculating minimum drop later
-        reaches = self.reaches[['geometry', 'iseg', 'rchlen']].copy()
-        seglen = reaches.groupby('iseg')['rchlen'].sum()
-        self.segment_data.loc[seglen.index, 'seglen'] = seglen
-        return seglen
-
-    def get_outseg_elev(self):
-        """Get the max elevup from all downstream segments for each segment."""
-        self.segment_data['outseg_elevup'] = self.segment_data.outseg.apply(
-            lambda x: self.segment_data.loc[
-                self.segment_data.index == x].elevup).max(axis=1)
-        return self.segment_data['outseg_elevup']
-
-    def set_outseg_elev_for_seg(self, seg):
-        """Set outseg elevation for segment.
-
-        Gets all the defined outseg_elevup associated with a specific segment
-        (multiple upstream segments route to one segment)
-        Returns a df with all the calculated outseg elevups for each segment.
-        .min(axis=1) is a good way to collapse to a series
-        :param seg: Pandas Series containing one row of seg_data dataframe
-        :return: Returns a df of the outseg_elev up values
-        where current segment is listed as an outseg
-        """
-        # downstreambuffer = 0.001 # 1mm
-        # find where seg is listed as outseg
-        outsegsel = self.segment_data['outseg'] == seg.name
-        # set outseg elevup
-        outseg_elevup = self.segment_data.loc[outsegsel, 'outseg_elevup']
-        return outseg_elevup
-
-    def minslope_seg(self, seg, *args):
-        """
-        Force segment to have minimum slope (check for backward flowing segs).
-
-        Moves downstream end down (vertically, more incision)
-        to achieve minimum slope.
-        :param seg: Pandas Series containing one row of seg_data dataframe
-        :param args: desired minimum slope
-        :return: Pandas Series with new downstream elevation and
-        associated outseg_elevup
-        """
-        # segdata_df = args[0]
-        minslope = args[0]
-        downstreambuffer = 0.001  # 1mm
-        up = seg.elevup
-        dn = np.nan
-        outseg_up = np.nan
-        # prefer slope derived from surface
-        surfslope = (seg.top_up-seg.top_dn)/(10.*seg.seglen)
-        prefslope = np.max([surfslope, minslope])
-        if seg.outseg > 0.0:
-            # select outflow segment for current seg and pull out elevup
-            outsegsel = self.segment_data.index == seg.outseg
-            outseg_elevup = self.segment_data.loc[outsegsel, 'elevup']
-            down = outseg_elevup.values[0]
-            if down >= up - (seg.seglen * prefslope):
-                # downstream elevation too high
-                dn = up - (seg.seglen * prefslope)  # set to minslope
-                outseg_up = up - (seg.seglen * prefslope) - downstreambuffer
-                print('Segment {}, outseg = {}, old outseg_elevup = {}, '
-                      'new outseg_elevup = {}'
-                      .format(seg.name, seg.outseg,
-                              seg.outseg_elevup, outseg_up))
-            else:
-                dn = down
-                outseg_up = down - downstreambuffer
-        else:
-            # must be an outflow segment
-            down = seg.elevdn
-            if down > up - (seg.seglen * prefslope):
-                dn = up - (seg.seglen * prefslope)
-                print('Outflow Segment {}, outseg = {}, old elevdn = {}, '
-                      'new elevdn = {}'
-                      .format(seg.name, seg.outseg, seg.elevdn, dn))
+        Returns
+        -------
+        None
+
+        See Also
+        --------
+        swn.file.read_formatted_frame : Read formatted file as a DataFrame.
+        SwnMf6.package_period_frame : Dataframe generator.
+        SwnMf6.flopy_package_period : Dict of lists of lists for flopy.
+
+        Examples
+        --------
+        >>> import flopy
+        >>> import geopandas
+        >>> import pandas as pd
+        >>> import swn
+        >>> from tempfile import TemporaryDirectory
+        >>> from pathlib import Path
+        >>> lines = geopandas.GeoSeries.from_wkt([
+        ...    "LINESTRING (60 100, 60  80)",
+        ...    "LINESTRING (40 130, 60 100)",
+        ...    "LINESTRING (70 130, 60 100)"])
+        >>> lines.index += 100
+        >>> n = swn.SurfaceWaterNetwork.from_lines(lines)
+        >>> tmp_dir_obj = TemporaryDirectory()
+        >>> dir = Path(tmp_dir_obj.name)
+        >>> sim = flopy.mf6.MFSimulation(sim_ws=str(dir))
+        >>> _ = flopy.mf6.ModflowTdis(sim, nper=1, time_units="days")
+        >>> gwf = flopy.mf6.ModflowGwf(sim)
+        >>> _ = flopy.mf6.ModflowGwfdis(
+        ...     gwf, nrow=3, ncol=2, delr=20.0, delc=20.0, top=10, botm=0,
+        ...     idomain=1, length_units="meters", xorigin=30.0, yorigin=70.0)
+        >>> nm = swn.SwnMf6.from_swn_flopy(n, gwf)
+        >>> nm.set_reach_data_from_array("elev", gwf.dis.top.array)
+        >>> nm.reaches["dlen"] = nm.reaches.length.round(3)
+        >>> nm.reaches["cond"] = 15.0
+        >>> nm.reaches["boundname"] = nm.reaches["segnum"]
+        >>> fname_tpl = dir / "model_drn_{:02d}.dat"
+        >>> fname_01 = dir / "model_drn_01.dat"
+        >>> nm.write_package_period("drn", fname_tpl, auxiliary="dlen")
+        >>> print(fname_01.read_text(), end="")
+        #k  i  j  elev  cond   dlen  boundname
+         1  1  1  10.0  15.0 18.028  101
+         1  1  2  10.0  15.0  6.009  101
+         1  2  2  10.0  15.0 12.019  101
+         1  1  2  10.0  15.0 21.082  102
+         1  2  2  10.0  15.0 10.541  102
+         1  2  2  10.0  15.0 10.000  100
+         1  3  2  10.0  15.0 10.000  100
+        >>> drn = nm.set_package_obj(
+        ...    "drn", pname="swn_drn", auxmultname="dlen",
+        ...    stress_period_data={0: {"filename": fname_01.name}})
+        >>> sim.write_simulation(silent=True)
+        >>> success, buff = sim.run_simulation()  # doctest: +SKIP
+        >>> tmp_dir_obj.cleanup()
+
+        """
+        spdf = self.package_period_frame(
+            package, "native", auxiliary=auxiliary, boundname=boundname)
+        if isinstance(fname, os.PathLike):
+            fname = os.fsdecode(fname)
+        for per, df in spdf.groupby("per"):
+            per_fname = fname.format(per)
+            self.logger.debug("writing period file %s", per_fname)
+            write_formatted_frame(df, per_fname, index=False)
+
+    def flopy_package_period(
+            self, package: str, auxiliary: list = [], boundname=None):
+        """Return dict of lists of lists for flopy's stress_period_data.
+
+        Parameters
+        ----------
+        package : str
+            MODFLOW 6 package name, such as "drn" for DRAIN, or "GWT/SRC" for
+            Mass Source Loading.
+        auxiliary : str, list, optional
+            String or list of auxiliary variable names. Default [].
+        boundname : bool, optional
+            Default None will determine if "boundname" column is added if
+            available in reaches.columns.
+
+        Returns
+        -------
+        dict
+
+        See Also
+        --------
+        SwnMf6.package_period_frame : Dataframe generator.
+        SwnMf6.write_package_period : Write native file.
+
+        Examples
+        --------
+        >>> import flopy
+        >>> import geopandas
+        >>> import pandas as pd
+        >>> import swn
+        >>> lines = geopandas.GeoSeries.from_wkt([
+        ...    "LINESTRING (60 100, 60  80)",
+        ...    "LINESTRING (40 130, 60 100)",
+        ...    "LINESTRING (70 130, 60 100)"])
+        >>> lines.index += 100
+        >>> n = swn.SurfaceWaterNetwork.from_lines(lines)
+        >>> sim = flopy.mf6.MFSimulation()
+        >>> _ = flopy.mf6.ModflowTdis(sim, nper=1, time_units="days")
+        >>> gwf = flopy.mf6.ModflowGwf(sim)
+        >>> _ = flopy.mf6.ModflowGwfdis(
+        ...     gwf, nrow=3, ncol=2, delr=20.0, delc=20.0, top=10, botm=0,
+        ...     idomain=1, length_units="meters", xorigin=30.0, yorigin=70.0)
+        >>> nm = swn.SwnMf6.from_swn_flopy(n, gwf)
+        >>> nm.set_reach_data_from_array("elev", gwf.dis.top.array)
+        >>> nm.reaches["dlen"] = nm.reaches.length.round(3)
+        >>> nm.reaches["cond"] = 15.0
+        >>> nm.reaches["boundname"] = nm.reaches["segnum"]
+        >>> drn = nm.set_package_obj("drn", auxmultname="dlen")
+        >>> pd.DataFrame(drn.stress_period_data.data[0])
+              cellid  elev  cond    dlen boundname
+        0  (0, 0, 0)  10.0  15.0  18.028       101
+        1  (0, 0, 1)  10.0  15.0   6.009       101
+        2  (0, 1, 1)  10.0  15.0  12.019       101
+        3  (0, 0, 1)  10.0  15.0  21.082       102
+        4  (0, 1, 1)  10.0  15.0  10.541       102
+        5  (0, 1, 1)  10.0  15.0  10.000       100
+        6  (0, 2, 1)  10.0  15.0  10.000       100
+
+        """
+        spdf = self.package_period_frame(
+            package, "flopy", auxiliary=auxiliary, boundname=boundname)
+        spd = {}
+        for per, df in spdf.groupby("per"):
+            spd[per] = [list(x) for x in df.itertuples(index=False)]
+        return spd
+
+    _tsvar_meta = pd.DataFrame([
+        ("status", "str"),
+        ("manning", "ts"),
+        ("stage", "ts"),
+        ("inflow", "ts"),
+        ("rainfall", "ts"),
+        ("evaporation", "ts"),
+        ("runoff", "ts"),
+        ("divflow", "ts"),
+        ("upstream_fraction", "float"),
+        ("auxname", "str"),
+        ("auxval", "ts"),
+    ], columns=["name", "type"]).set_index("name")
+
+    def _check_tsvar_name(self, name: str):
+        """Helper method to check name used for set_tsvar_* methods."""
+        # TODO
+        raise NotImplementedError("method is not finished")
+        if not isinstance(name, str):
+            raise ValueError("name must be str type")
+        elif name not in self._tsvar_meta.index:
+            names = ", ".join(repr(n) for n in self._tsvar_meta.index)
+            raise KeyError(f"could not find {name!r} in {names}")
+
+    def set_tsvar_from_segments(self, name: str, data, where: str = "start"):
+        """Set time-varying data from data defined at segments.
+
+        Parameters
+        ----------
+        name : str
+            Name for dataset to use in a tsvar dict.
+        data : dict, pandas.Series or pandas.DataFrame
+            Data to assigned to tsvar, indexed by segnum.
+        where : str, optional, default "start"
+            For segments represented by multiple reaches, pick which reach
+            to represent data. Default "start" is the upper-most reach.
+        """
+        # TODO
+        raise NotImplementedError("method is not finished")
+        self._check_tsvar_name(name)
+        if not np.isscalar(data):
+            raise ValueError("only non-scalar data can be set")
+        if where != "start":
+            raise NotImplementedError("only 'start' is currently implemented")
+
+    def default_packagedata(
+            self, hyd_cond1=1., hyd_cond_out=None,
+            thickness1=1., thickness_out=None, width1=None, width_out=None,
+            roughch=0.024):
+        """High-level function to set MODFLOW 6 SFR PACKAGEDATA defaults.
+
+        Parameters
+        ----------
+        hyd_cond1 : float or pandas.Series, optional
+            Hydraulic conductivity of the streambed, as a global or per top of
+            each segment. Used for reach rhk. Default 1.
+        hyd_cond_out : None, float or pandas.Series, optional
+            Similar to thickness1, but for the hydraulic conductivity of each
+            segment outlet. If None (default), the same hyd_cond1 value for the
+            top of the outlet segment is used for the bottom.
+        thickness1 : float or pandas.Series, optional
+            Thickness of the streambed, as a global or per top of each segment.
+            Used for reach rbth. Default 1.
+        thickness_out : None, float or pandas.Series, optional
+            Similar to thickness1, but for the bottom of each segment outlet.
+            If None (default), the same thickness1 value for the top of the
+            outlet segment is used for the bottom.
+        width1 : float or pandas.Series, optional
+            Channel width, as a global or per top of each segment. Used for
+            reach rwid. Default None will first try finding "width" from
+            "segments", otherwise will use 10.
+        width_out : None, float or pandas.Series, optional
+            Similar to width1, but for the bottom of each segment outlet.
+            If None (default), use a constant width1 value for segment.
+        roughch : float or pandas.Series, optional
+            Manning's roughness coefficient for the channel. If float, then
+            this is a global value, otherwise it is per-segment with a Series.
+            Default 0.024.
+
+        Returns
+        -------
+        None
+        """
+        self.logger.info("default_packagedata: using high-level function")
+
+        if width1 is None:
+            # Determine width based on available data
+            if "width" in self.segments.columns:
+                width1 = self.segments.width
+                action = "taken from segments frame, with range %.3f to %.3f"
+                action_args = width1.min(), width1.max()
             else:
-                dn = down
-        # this returns a DF once the apply is done!
-        return pd.Series({'nseg': seg.name, 'elevdn': dn,
-                          'outseg_elevup': outseg_up})
-
-    def set_forward_segs(self, min_slope=1.e-4):
-        """Set minimum slope in forwards direction.
-
-        Ensure slope of all segment is at least min_slope
-        in the downstream direction.
-        Moves down the network correcting downstream elevations if necessary
-        :param min_slope: Desired minimum slope
-        :return: and updated segment data df
-        """
-        # upper most segments (not referenced as outsegs)
-        # segdata_df = self.segment_data.sort_index(axis=1)
-        segsel = ~self.segment_data.index.isin(self.segment_data['outseg'])
-        while segsel.sum() > 0:
-            print('Checking elevdn and outseg_elevup for {} segments'
-                  .format(segsel.sum()))
-            # get elevdn and outseg_elevups with a minimum slope constraint
-            # index should align with self.segment_data index
-            # not applying directly allows us to filter out nans
-            tmp = self.segment_data.assign(_='').loc[segsel].apply(
-                self.minslope_seg, args=[min_slope], axis=1)
-            ednsel = tmp[tmp['elevdn'].notna()].index
-            oeupsel = tmp[tmp['outseg_elevup'].notna()].index
-            # set elevdn and outseg_elevup
-            self.segment_data.loc[ednsel, 'elevdn'] = tmp.loc[ednsel, 'elevdn']
-            self.segment_data.loc[oeupsel, 'outseg_elevup'] = \
-                tmp.loc[oeupsel, 'outseg_elevup']
-            # get `elevups` for outflow segs from `outseg_elevups`
-            # taking `min` ensures outseg elevup is below all inflow elevdns
-            tmp2 = self.segment_data.apply(
-                self.set_outseg_elev_for_seg, axis=1).min(axis=1)
-            tmp2 = pd.DataFrame(tmp2, columns=['elevup'])
-            # update `elevups`
-            eupsel = tmp2[tmp2.loc[:, 'elevup'].notna()].index
-            self.segment_data.loc[eupsel, 'elevup'] = \
-                tmp2.loc[eupsel, 'elevup']
-            # get list of next outsegs
-            segsel = self.segment_data.index.isin(
-                self.segment_data.loc[segsel, 'outseg'])
-        return self.segment_data
-
-    def fix_segment_elevs(self, min_incise=0.2, min_slope=1.e-4,
-                          max_str_z=None):
-        """
-        Provide wrapper function for calculating SFR segment elevations.
-
-        Calls series of functions to process and move sfr segment elevations,
-        to try to ensure:
-            0. Segments are below the model top
-            1. Segments flow downstream
-            2. Downstream segments are below upstream segments
-        :param min_slope: desired minimum slope for segment
-        :param min_incise: desired minimum incision (in model units)
-        :return: segment data dataframe
-        """
-        kijcols = {"k_up", "i_up", "j_up", "k_dn", "i_dn", "j_dn"}
-        dif = kijcols - set(self.segment_data.columns)
-        if len(dif) > 1:
-            # some missing
-            # drop others
-            others = kijcols - dif
-            self.segment_data.drop(others, axis=0, inplace=True)
-            # get model locations for segments ends
-            _ = self.get_seg_ijk()
-        # get model cell elevations at seg ends
-        _ = self.get_top_elevs_at_segs()
-        # get current segment incision at seg ends
-        _ = self.get_segment_incision()
-        # move segments end elevation down to achieve minimum incision
-        _ = self.set_seg_minincise(minincise=min_incise, max_str_z=max_str_z)
-        # get the elevations of downstream segments
-        _ = self.get_outseg_elev()
-        # get segment length from reach lengths
-        _ = self.get_segment_length()
-        # ensure downstream ends are below upstream ends
-        # and reconcile upstream elevation of downstream segments
-        self.set_forward_segs(min_slope=min_slope)
-        # reassess segment incision after processing.
-        self.get_segment_incision()
-        return self.segment_data
-
-    def reconcile_reach_strtop(self):
-        """
-        Recalculate reach strtop elevations after moving segment elevations.
-
-        :return: None
-        """
-        def reach_elevs(seg):
-            """Return reach properties.
-
-            Calculate reach elevation from segment slope and
-            reach length along segment.
-            :param seg: one row of reach data dataframe grouped by segment
-            :return: reaches by segment with strtop adjusted
-            """
-            segsel = self.segment_data.index == seg.name
-
-            seg_elevup = self.segment_data.loc[segsel, 'elevup'].values[0]
-            seg_slope = self.segment_data.loc[segsel, 'Zslope'].values[0]
-
-            # interpolate reach lengths to cell centres
-            cmids = seg.seglen.shift().fillna(0.0) + seg.rchlen.multiply(0.5)
-            cmids.iat[0] = 0.0
-            cmids.iat[-1] = seg.seglen.iloc[-1]
-            seg['cmids'] = cmids  # cummod+(seg.rchlen *0.5)
-            # calculate reach strtops
-            seg['strtop'] = seg['cmids'].multiply(seg_slope) + seg_elevup
-            # seg['slope']= #!!!!! use m.sfr.get_slopes() method
-            return seg
-        self.segment_data['Zslope'] = \
-            ((self.segment_data['elevdn'] - self.segment_data['elevup']) /
-             self.segment_data['seglen'])
-        segs = self.reaches.groupby('iseg')
-        self.reaches['seglen'] = segs.rchlen.cumsum()
-        self.reaches = segs.apply(reach_elevs)
-        return self.reaches
-
-    def set_topbot_elevs_at_reaches(self, m=None):
-        """
-        Get top and bottom elevation of the cell containing a reach.
-
-        :param m: Modflow model
-        :return: dataframe with reach cell top and bottom elevations
-        """
-        if m is None:
-            m = self.model
-        self.reaches['top'] = m.dis.top.array[
-            tuple(self.reaches[['i', 'j']].values.T)]
-        self.reaches['bot'] = m.dis.botm[0].array[
-            tuple(self.reaches[['i', 'j']].values.T)]
-        return self.reaches[['top', 'bot']]
+                width1 = 10.0
+                action = "not found in segments frame; using default %s"
+                action_args = (width1,)
+            self.logger.info(
+                f"default_packagedata: 'rwd' {action}", *action_args)
+        self.set_reach_data_from_segments(
+            "rwid", width1, width_out, method="constant")
+
+        if "rgrd" not in self.reaches.columns:
+            self.logger.info(
+                "default_packagedata: 'rgrd' not yet evaluated, setting with "
+                "set_reach_slope()")
+            self.set_reach_slope()
+
+        # TODO: add a similar method for rtp? set_reaches_top()?
+
+        # Get stream values from top of model
+        self.set_reach_data_from_array("rtp", self.model.dis.top.array)
+        if "zcoord_avg" in self.reaches.columns:
+            # Created by set_reach_slope(); be aware of NaN
+            nn = ~self.reaches.zcoord_avg.isnull()
+            self.reaches.loc[nn, "rtp"] = self.reaches.loc[nn, "zcoord_avg"]
+
+        # Assign remaining reach datasets
+        self.set_reach_data_from_segments("rbth", thickness1, thickness_out)
+        self.set_reach_data_from_segments("rhk", hyd_cond1, hyd_cond_out, True)
+        self.set_reach_data_from_segments("man", roughch)
+        if self.diversions is not None:
+            diversion_reaches = self.reaches["diversion"]
+            self.reaches.loc[diversion_reaches, "rwid"] = 1.0
+            self.reaches.loc[diversion_reaches, "rhk"] = 0.0
 
-    def fix_reach_elevs(self, minslope=0.0001, fix_dis=True, minthick=0.5):
-        """Fix reach elevations.
+    def set_sfr_obj(self, auxiliary=None, boundnames=None, **kwds):
+        """Set MODFLOW 6 SFR package data to flopy model.
+
+        Parameters
+        ----------
+        auxiliary : list, optional
+            List of auxiliary names, which must be columns in the reaches
+            frame.
+        boundnames : bool, optional
+            Sets the BOUNDAMES option, with names provided by a "boundname"
+            column of the reaches frame. Default None will set this True
+            if column exists.
+        **kwds : dict, optional
+            Passed to flopy.mf6.ModflowGwfsfr.
+
+        Returns
+        -------
+        flopy.mf6.ModflowGwfsfr
+
+        """
+        import flopy
+
+        if auxiliary is not None:
+            kwds["auxiliary"] = auxiliary
+        if boundnames is None:
+            boundnames = "boundname" in self.reaches.columns
+        if boundnames:
+            kwds["boundnames"] = True
+        kwds["nreaches"] = len(self.reaches)
+        if "packagedata" not in kwds:
+            kwds["packagedata"] = self.flopy_packagedata(
+                auxiliary=auxiliary, boundname=boundnames)
+        if "connectiondata" not in kwds:
+            kwds["connectiondata"] = self.flopy_connectiondata()
+        if self.diversions is not None and "diversions" not in kwds:
+            kwds["diversions"] = self.flopy_diversions()
+
+        return flopy.mf6.ModflowGwfsfr(self.model, **kwds)
+
+    def set_package_obj(
+            self, package: str, auxiliary=None, boundnames=None, **kwds):
+        """Set MODFLOW 6 package data to flopy model.
+
+        Parameters
+        ----------
+        package : str
+            MODFLOW 6 package name, such as "drn" for DRAIN, or "GWT/SRC" for
+            Mass Source Loading.
+        auxiliary : list, optional
+            List of auxiliary names, which must be columns in the reaches
+            frame.
+        boundnames : bool, optional
+            Sets the BOUNDAMES option, with names provided by a "boundname"
+            column of the reaches frame. Default None will set this True
+            if column exists.
+        **kwds : dict, optional
+            Passed to flopy.mf6 package.
+
+        Returns
+        -------
+        flopy.mf6.mfpackage.MFPackage
+            Subclass instance.
+
+        """
+        if auxiliary is None and "auxmultname" in kwds:
+            auxiliary = kwds["auxmultname"]
+        if auxiliary is not None:
+            kwds["auxiliary"] = auxiliary
+        if boundnames is None:
+            boundnames = "boundname" in self.reaches.columns
+        if boundnames:
+            kwds["boundnames"] = True
+        if "stress_period_data" not in kwds:
+            kwds["stress_period_data"] = self.flopy_package_period(
+                package=package, auxiliary=auxiliary, boundname=boundnames)
+        if "maxbound" not in kwds:
+            kwds["maxbound"] = len(self.reaches)
+
+        Mf6pak = get_flopy_mf6_package(package)
+        # self.logger.debug("%s called with kwds: %s", package, kwds)
+        return Mf6pak(self.model, **kwds)
+
+    def _segbyseg_elevs(self, minslope=1e-4, fix_dis=True, minthick=0.5,
+                        min_incise=0.2, max_str_z=None):
+        """
+        Fix reach elevations but by using segment definition and setting sane
+        segment elevations first.
 
         Need to ensure reach elevation is:
             0. below the top
             1. below the upstream reach
             2. above the minimum slope to the bottom reach elevation
             3. above the base of layer 1
         segment by segment, reach by reach! Fun!
-
-        :return:
         """
+        raise NotImplementedError("method not finished")
+
         def _check_reach_v_laybot(r, botms, buffer=1.0, rbed_elev=None):
             if rbed_elev is None:
                 rbed_elev = r.strtop - r.strthick
             if (rbed_elev - buffer) < r.bot:
                 # if new strtop is below layer one
                 # drop bottom of layer one to accomodate stream
                 # (top, bed thickness and buffer)
                 new_elev = rbed_elev - buffer
-                print('seg {} reach {} @ {} '
-                      'is below layer 1 bottom @ {}'
-                      .format(seg, r.ireach, rbed_elev,
-                              r.bot))
-                print('    dropping layer 1 bottom to {} '
-                      'to accommodate stream @ i = {}, j = {}'
-                      .format(new_elev, r.i, r.j))
+                self.logger.debug(
+                    "seg %s reach %s @ %s is below layer 1 bottom @ %s",
+                    seg, r.ireach, rbed_elev, r.bot)
+                self.logger.debug((
+                    "dropping layer 1 bottom to %s to accommodate stream "
+                    "@ i = %s, j = %s", new_elev, r.i, r.j))
                 botms[0, r.i, r.j] = new_elev
             return botms
 
+        # fix segments first
+        # 0. Segments are below the model top
+        # 1. Segments flow downstream
+        # 2. Downstream segments are below upstream segments
+        self.fix_segment_elevs(
+            min_incise=min_incise,
+            min_slope=minslope,
+            max_str_z=max_str_z)
+        self.reconcile_reach_strtop()
         buffer = 1.0  # 1 m (buffer to leave at the base of layer 1 -
         # also helps with precision issues)
         # make sure elevations are up-to-date
         # recalculate REACH strtop elevations
         self.reconcile_reach_strtop()
-        _ = self.set_topbot_elevs_at_reaches()
+        self.add_model_topbot_to_reaches()
         # top read from dis as float32 so comparison need to be with like
-        reachsel = self.reaches['top'] <= self.reaches['strtop']
-        reach_ij = tuple(self.reaches[['i', 'j']].values.T)
-        print('{} segments with reaches above model top'.format(
-            self.reaches[reachsel]['iseg'].unique().shape[0]))
+        reachsel = self.reaches["top"] <= self.reaches["strtop"]
+        reach_ij = tuple(self.reaches[["i", "j"]].values.T)
+        self.logger.info(
+            "%s segments with reaches above model top",
+            self.reaches[reachsel]["iseg"].unique().shape[0])
         # get segments with reaches above the top surface
         segsabove = self.reaches[reachsel].groupby(
-            'iseg').size().sort_values(ascending=False)
+            "iseg").size().sort_values(ascending=False)
         # get incision gradient from segment elevups and elevdns
-        # ('diff_up' and 'diff_dn' are the incisions of the top and
+        # ("diff_up" and "diff_dn" are the incisions of the top and
         # bottom reaches from the segment data)
-        self.segment_data['incgrad'] = \
-            ((self.segment_data['diff_up'] - self.segment_data['diff_dn']) /
-             self.segment_data['seglen'])
+        self.segment_data["incgrad"] = \
+            ((self.segment_data["diff_up"] - self.segment_data["diff_dn"]) /
+             self.segment_data["seglen"])
         # copy of layer 1 bottom (for updating to fit in stream reaches)
         layerbots = self.model.dis.botm.array.copy()
         # loop over each segment
         for seg in self.segment_data.index:  # (all segs)
             # selection for segment in reachdata and seg data
-            rsel = self.reaches['iseg'] == seg
+            rsel = self.reaches["iseg"] == seg
             segsel = self.segment_data.index == seg
 
             if seg in segsabove.index:
                 # check top and bottom reaches are above layer 1 bottom
                 # (not adjusting elevations of reaches)
                 for reach in self.reaches[rsel].iloc[[0, -1]].itertuples():
                     layerbots = _check_reach_v_laybot(reach, layerbots, buffer)
                 # apparent optimised incision based
                 # on the incision gradient for the segment
-                self.reaches.loc[rsel, 'strtop_incopt'] = \
-                    self.reaches.loc[rsel, 'top'].subtract(
-                        self.segment_data.loc[segsel, 'diff_up'].values[0]) + \
-                    (self.reaches.loc[rsel, 'cmids'].subtract(
-                        self.reaches.loc[rsel, 'cmids'].values[0]) *
-                     self.segment_data.loc[segsel, 'incgrad'].values[0])
+                self.reaches.loc[rsel, "strtop_incopt"] = \
+                    self.reaches.loc[rsel, "top"].subtract(
+                        self.segment_data.loc[segsel, "diff_up"].values[0]) + \
+                    (self.reaches.loc[rsel, "cmids"].subtract(
+                        self.reaches.loc[rsel, "cmids"].values[0]) *
+                     self.segment_data.loc[segsel, "incgrad"].values[0])
                 # falls apart when the top elevation is not monotonically
                 # decreasing down the segment (/always!)
 
                 # bottom reach elevation:
-                botreach_strtop = self.reaches[rsel]['strtop'].values[-1]
+                botreach_strtop = self.reaches[rsel]["strtop"].values[-1]
                 # total segment length
-                seglen = self.reaches[rsel]['seglen'].values[-1]
+                seglen = self.reaches[rsel]["seglen"].values[-1]
                 # botreach_slope = minslope  # minimum slope of segment
                 # top reach elevation and "length?":
-                upreach_strtop = self.reaches[rsel]['strtop'].values[0]
-                upreach_cmid = self.reaches[rsel]['cmids'].values[0]
+                upreach_strtop = self.reaches[rsel]["strtop"].values[0]
+                upreach_cmid = self.reaches[rsel]["cmids"].values[0]
                 # use top reach as starting point
 
                 # loop over reaches in segement from second to penultimate
                 # (dont want to move elevup or elevdn)
                 for reach in self.reaches[rsel][1:-1].itertuples():
                     # strtop that would result from minimum slope
                     # from upstream reach
                     strtop_withminslope = upreach_strtop - (
                             (reach.cmids - upreach_cmid) * minslope)
                     # strtop that would result from minimum slope
                     # from bottom reach
                     strtop_min2bot = botreach_strtop + (
                             (seglen - reach.cmids) * minslope)
-                    # check 'optimum incision' is below upstream elevation
+                    # check "optimum incision" is below upstream elevation
                     # and above the minimum slope to the bottom reach
                     if reach.strtop_incopt < strtop_min2bot:
                         # strtop would give too shallow a slope to
                         # the bottom reach (not moving bottom reach)
-                        print('seg {} reach {}, incopt is \\/ below minimum '
-                              'slope from bottom reach elevation'
-                              .format(seg, reach.ireach))
-                        print('    setting elevation to minslope from bottom')
+                        self.logger.debug(
+                            "seg %s reach %s, incopt is \\/ below minimum "
+                            "slope from bottom reach elevation",
+                            seg, reach.ireach)
+                        self.logger.debug(
+                            "setting elevation to minslope from bottom")
                         # set to minimum slope from outreach
                         self.reaches.at[
-                            reach.Index, 'strtop'] = strtop_min2bot
+                            reach.Index, "strtop"] = strtop_min2bot
                         # update upreach for next iteration
                         upreach_strtop = strtop_min2bot
                     elif reach.strtop_incopt > strtop_withminslope:
                         # strtop would be above upstream or give
                         # too shallow a slope from upstream
-                        print('seg {} reach {}, incopt /\\ above upstream'
-                              .format(seg, reach.ireach))
-                        print('    setting elevation to minslope from '
-                              'upstream')
+                        self.logger.debug(
+                            "seg %s reach %s, incopt /\\ above upstream",
+                            seg, reach.ireach)
+                        self.logger.debug(
+                            "setting elevation to minslope from upstream")
                         # set to minimum slope from upstream reach
                         self.reaches.at[
-                            reach.Index, 'strtop'] = strtop_withminslope
+                            reach.Index, "strtop"] = strtop_withminslope
                         # update upreach for next iteration
                         upreach_strtop = strtop_withminslope
                     else:
-                        # strtop might be ok to set to 'optimum incision'
-                        print('seg {} reach {}, incopt is -- below upstream '
-                              'reach and above the bottom reach'
-                              .format(seg, reach.ireach))
+                        # strtop might be ok to set to "optimum incision"
+                        self.logger.debug(
+                            "seg %s reach %s, incopt is -- below upstream "
+                            "reach and above the bottom reach",
+                            seg, reach.ireach)
                         # CHECK FIRST:
                         # if optimium incision would place it
                         # below the bottom of layer 1
                         if reach.strtop_incopt - reach.strthick < \
                                 reach.bot + buffer:
                             # opt - stream thickness lower than layer 1 bottom
                             # (with a buffer)
-                            print('seg {} reach {}, incopt - bot is x\\/ '
-                                  'below layer 1 bottom'
-                                  .format(seg, reach.ireach))
+                            self.logger.debug(
+                                "seg %s reach %s, incopt - bot is x\\/ "
+                                "below layer 1 bottom", seg, reach.ireach)
                             if reach.bot + reach.strthick + buffer > \
                                     strtop_withminslope:
                                 # if layer bottom would put reach above
                                 # upstream reach we can only set to
                                 # minimum slope from upstream
-                                print('    setting elevation to minslope '
-                                      'from upstream')
-                                self.reaches.at[reach.Index, 'strtop'] = \
+                                self.logger.debug(
+                                    "setting elevation to minslope "
+                                    "from upstream")
+                                self.reaches.at[reach.Index, "strtop"] = \
                                     strtop_withminslope
                                 upreach_strtop = strtop_withminslope
                             else:
                                 # otherwise we can move reach so that it
                                 # fits into layer 1
                                 new_elev = reach.bot + reach.strthick + buffer
-                                print('    setting elevation to {}, above '
-                                      'layer 1 bottom'.format(new_elev))
+                                self.logger.debug(
+                                    "setting elevation to %s, above "
+                                    "layer 1 bottom", new_elev)
                                 # set reach top so that it is above layer 1
                                 # bottom with a buffer
                                 # (allowing for bed thickness)
-                                self.reaches.at[reach.Index, 'strtop'] = \
+                                self.reaches.at[reach.Index, "strtop"] = \
                                     reach.bot + buffer + reach.strthick
                                 upreach_strtop = new_elev
                         else:
-                            # strtop ok to set to 'optimum incision'
+                            # strtop ok to set to "optimum incision"
                             # set to "optimum incision"
-                            print('    setting elevation to incopt')
+                            self.logger.debug("setting elevation to incopt")
                             self.reaches.at[
-                                reach.Index, 'strtop'] = reach.strtop_incopt
+                                reach.Index, "strtop"] = reach.strtop_incopt
                             upreach_strtop = reach.strtop_incopt
                     # check if new stream top is above layer 1 with a buffer
                     # (allowing for bed thickness)
                     reachbed_elev = upreach_strtop - reach.strthick
                     layerbots = _check_reach_v_laybot(reach, layerbots, buffer,
                                                       reachbed_elev)
                     upreach_cmid = reach.cmids
                     # upreach_slope=reach.slope
             else:
                 # For segments that do not have reaches above top
                 # check if reaches are below layer 1
-                print('seg {} is always downstream and below the top'
-                      .format(seg))
+                self.logger.debug(
+                    "seg %s is always downstream and below the top", seg)
                 for reach in self.reaches[rsel].itertuples():
                     reachbed_elev = reach.strtop - reach.strthick
                     layerbots = _check_reach_v_laybot(reach, layerbots, buffer,
                                                       reachbed_elev)
             # OH CRAP need to update dis bottoms in reach df!
-            # self.reaches['top'] = layerbots[
-            #     tuple(self.reaches[['i', 'j']].values.T)]
-            self.reaches['bot'] = layerbots[0][reach_ij]
+            # self.reaches["top"] = layerbots[
+            #     tuple(self.reaches[["i", "j"]].values.T)]
+            self.reaches["bot"] = layerbots[0][reach_ij]
         if fix_dis:
             # fix dis for incised reaches
-            for lay in range(self.model.dis.nlay - 1):
-                laythick = layerbots[lay] - layerbots[
-                    lay + 1]  # first one is layer 1 bottom - layer 2 bottom
-                print('checking layer {} thicknesses'.format(lay + 2))
+            for k in range(self.model.dis.nlay - 1):
+                laythick = layerbots[k] - layerbots[
+                    k + 1]  # first one is layer 1 bottom - layer 2 bottom
+                self.logger.debug("checking layer %s thicknesses", k + 2)
                 thincells = laythick < minthick
-                print('{} cells less than {}'
-                      .format(thincells.sum(), minthick))
+                self.logger.debug(
+                    "%s cells less than %s", thincells.sum(), minthick)
                 laythick[thincells] = minthick
-                layerbots[lay + 1] = layerbots[lay] - laythick
-            self.model.dis.botm = layerbots
+                layerbots[k + 1] = layerbots[k] - laythick
+            # flopy messing with external file names so apply in wrapper
+            # TODO remove line if flopy is patched (https://github.com/modflowpy/flopy/issues/1534)
+            _flopy_set3darray(self.model.dis.botm, layerbots)
+            # self.model.dis.botm.set_data(layerbots)
+
+    def _reachbyreach_elevs(
+            self, minslope=1e-4, minincise=0.2, minthick=0.5, fix_dis=True,
+            direction="downstream"):
+        """
+        Fix reach elevations by just working from headwater to outlet
+        (ignoring segment divisions).
 
-    def sfr_plot(self, model, sfrar, dem, points=None, points2=None,
-                 label=None):
-        """Plot sfr."""
-        from ._modelplot import ModelPlot
-        p = ModelPlot(model)
-        p._add_plotlayer(dem, label="Elevation (m)")
-        p._add_sfr(sfrar, cat_cmap=False, cbar=True,
-                   label=label)
-        return p
-
-    def plot_reaches_above(self, model, seg, dem=None,
-                           plot_bottom=False, points2=None):
-        """Plot sfr reaches above."""
-        # ensure reach elevations are up-to-date
-        _ = self.set_topbot_elevs_at_reaches()
-        dis = model.dis
-        sfr = model.sfr
-        if dem is None:
-            dem = np.ma.array(
-                dis.top.array, mask=model.bas6.ibound.array[0] == 0)
-        sfrar = np.ma.zeros(dis.top.array.shape, 'f')
-        sfrar.mask = np.ones(sfrar.shape)
-        lay1reaches = self.reaches.loc[
-            self.reaches.k.apply(lambda x: x == 1)]
-        points = None
-        if lay1reaches.shape[0] > 0:
-            points = lay1reaches[['i', 'j']]
-        # segsel=reachdata['iseg'].isin(segsabove.index)
-        if seg == 'all':
-            segsel = np.ones((self.reaches.shape[0]), dtype=bool)
-        else:
-            segsel = self.reaches['iseg'] == seg
-        sfrar[tuple((self.reaches[segsel][['i', 'j']]
-                     .values.T).tolist())] = \
-            (self.reaches[segsel]['top'] -
-             self.reaches[segsel]['strtop']).tolist()
-        # .mask = np.ones(sfrar.shape)
-        vtop = self.sfr_plot(model, sfrar, dem, points=points, points2=points2,
-                             label="str below top (m)")
-        if seg != 'all':
-            sfr.plot_path(seg)
-        if plot_bottom:
-            dembot = np.ma.array(dis.botm.array[0],
-                                 mask=model.bas6.ibound.array[0] == 0)
-            sfrarbot = np.ma.zeros(dis.botm.array[0].shape, 'f')
-            sfrarbot.mask = np.ones(sfrarbot.shape)
-            sfrarbot[tuple((self.reaches[segsel][['i', 'j']]
-                            .values.T).tolist())] = \
-                (self.reaches[segsel]['strtop'] -
-                 self.reaches[segsel]['bot']).tolist()
-            # .mask = np.ones(sfrar.shape)
-            vbot = self.sfr_plot(model, sfrarbot, dembot, points=points,
-                                 points2=points2, label="str above bottom (m)")
+        Need to ensure reach elevation is:
+            0. below the top
+            1. below the upstream reach
+            2. above the minimum slope to the bottom reach elevation
+            3. above the base of layer 1
+        (nwt method went seg-by-seg then reach-by-reach)
+
+        Parameters
+        ----------
+        minslope : float, defai;t 1e-4
+            The minimum allowable slope between adjacent reaches
+            (to be considered flowing downstream).
+        minincise : float, default 0.2
+            The minimum allowable incision of a reach below the model top.
+        minthick : float, default 0.5
+            The minimum thickness of stream bed. Will try to ensure that this
+            is available below stream top before layer bottom.
+        fix_dis : bool, default True
+            Move layer elevations down where it is not possible to honor
+            minimum slope without going below layer 1 bottom.
+        direction : {'upstream', 'downstream'}
+            NOT IMPLEMENTED
+            Select whether elevations are set from ensuring a minimum slope
+            in a upstream or downstream direction.
+            If 'upstream' will honor elevation at outlet reach
+                (if in model layer) and work upstream ensuring minimum slope.
+            If 'downstream' will honor elevation at headwater reach
+                (if in model layer) and work downstream ensuring minimum slope.
+            Default: 'downstream',
+            set elevations from headwaters to outlets.
+
+        Returns
+        -------
+
+        """
+        def _check_reach_v_laybot(r, botms, buffer=1.0, rbed_elev=None):
+            if rbed_elev is None:
+                rbed_elev = r.rtp - r.rbth
+            if (rbed_elev - buffer) < r.bot:
+                # if new strtop is below layer one
+                # drop bottom of layer one to accomodate stream
+                # (top, bed thickness and buffer)
+                new_elev = rbed_elev - buffer
+                name = getattr(r, "Index", None) or getattr(r, "name")
+                self.logger.debug(
+                    "reach %s @ %s is below layer 1 bottom @ %s",
+                    name, rbed_elev, r.bot)
+                self.logger.debug(
+                    "dropping layer 1 bottom to %s to accommodate stream "
+                    "@ i = %s, j = %s", new_elev, r.i, r.j)
+                botms[0, r.i, r.j] = new_elev
+            return botms
+
+        if direction == 'upstream':
+            ustrm = True
         else:
-            vbot = None
-        return vtop, vbot
+            ustrm = False
+        buffer = 1.0  # 1 m (buffer to leave at the base of layer 1 -
+        # also helps with precision issues)
+        # make sure elevations are up-to-date
+        # recalculate REACH strtop elevations
+        # self.reconcile_reach_strtop()
+        self.add_model_topbot_to_reaches()
+        # top read from dis as float32 so comparison need to be with like
+        reachsel = self.reaches["top"] <= self.reaches["rtp"]
+        reach_ij = tuple(self.reaches[["i", "j"]].values.T)
+        self.logger.info("%s reaches above model top", reachsel.sum())
+        # copy of layer 1 bottom (for updating to fit in stream reaches)
+        layerbots = self.model.dis.botm.array.copy()
+        sel = self.reaches["from_rnos"] == set()
+        if self.diversions is not None:
+            sel &= ~self.reaches["diversion"]
+        headreaches = self.reaches.loc[sel]
+        # through reaches DF
+        for hdrch in headreaches.itertuples():
+            # check if head reach above model top
+            if hdrch.rtp > hdrch.top - minincise:
+                # set to below model top
+                upreach_rtp = hdrch.top - minincise
+                self.reaches.at[hdrch.Index, "rtp"] = upreach_rtp
+            else:
+                upreach_rtp = hdrch.rtp
+            inc_up = hdrch.top - upreach_rtp
+            # get profile of reaches from this headwater
+            dsegs = self._swn.gather_segnums(downstream=hdrch.segnum)
+            segs = [hdrch.segnum] + dsegs
+            reaches = self.reaches.loc[
+                self.reaches.segnum.isin(segs)].sort_index()
+            # get outflow reach for this profile
+            # maybe can't rely on it being the last one
+            # the sort_index() should order (assuming rno increases downstream)
+            # so last should be to_rno == 0
+            assert reaches.iloc[-1].to_rno == 0, ("reach numbers possibly not "
+                                                  "increasing downstream")
+            outflow = reaches.iloc[-1]
+            # check if outflow above model top
+            if outflow.rtp > outflow.top - minincise:
+                # set below model top
+                botreach_rtp = outflow.top - minincise
+                self.reaches.at[outflow.name, "rtp"] = botreach_rtp
+            else:
+                botreach_rtp = outflow.rtp
+            inc_dn = outflow.top - botreach_rtp
+            # total profile length
+            totlen = reaches.rlen.sum()
+            reaches['mid_dist'] = \
+                reaches['rlen'].cumsum() - reaches['rlen'] / 2.0
+            if ustrm:  # switch order
+                reaches = reaches.sort_index(ascending=False)
+                prevreach_top = botreach_rtp
+                # get mid length for each reach
+                prevreach_mid = reaches.iloc[0].mid_dist
+            else:
+                prevreach_top = upreach_rtp
+                prevreach_mid = reaches.iloc[0].mid_dist
 
-    def to_pickle(self, path, protocol=pickle.HIGHEST_PROTOCOL):
-        """Pickle (serialize) non-flopy object data to file.
+            # get incision gradient from headwater and outflow incision
+            # ("inc_up" and "inc_dn" are the incisions of the top and
+            # bottom reaches) # TODO is this stil meaningfull?
+            incgrad = ((inc_up - inc_dn) / totlen)
+            # apparent optimised incision based
+            # on the incision gradient for the segment
+            reaches["strtop_incopt"] = (
+                    (reaches.top - inc_up) +
+                    ((reaches.mid_dist - prevreach_mid) * incgrad)
+            )
+            layerbots = _check_reach_v_laybot(
+                reaches.iloc[0], layerbots, buffer)
+            # loop over current profile from second to penultimate
+            # (dont want to move endpoints)
+            # TODO maybe more flexibility on bottom reach incision
+            for reach in reaches.iloc[1:].itertuples():
+                # strtop that would result from minimum slope
+                # from upstream reach
+                rtp = reach.rtp
+                strtop_withminslope = prevreach_top - (
+                        (reach.mid_dist - prevreach_mid) * minslope)
+                if rtp > reach.top - minincise:
+                    # current reach rtp is above the model top
+                    self.logger.debug(
+                        "reach %s, rtp is: /\\ above model top", reach.Index)
+                    minslope_cond = (
+                        reach.strtop_incopt < strtop_withminslope
+                        if ustrm else
+                        reach.strtop_incopt > strtop_withminslope
+                    )
+                    if minslope_cond:
+                        # incision according to incision gradient would be
+                        # above upstream/below downstream or give too shallow
+                        # a slope from previous:
+                        self.logger.debug(
+                            "reach %s, incopt is: %s", reach.Index,
+                            "\\/ below downstream" if ustrm
+                            else "/\\ above upstream")
+                        self.logger.debug(
+                            "setting elevation to minslope from previous")
+                        # set to minimum slope from previous reach
+                        self.reaches.at[reach.Index, "rtp"] = \
+                            strtop_withminslope
+                    else:
+                        # rtp might be ok to set to "optimum incision"
+                        self.logger.debug(
+                            "reach %s, incopt is: %s", reach.Index,
+                            "above downstream" if ustrm else "below upstream")
+                        # CHECK FIRST:
+                        # if optimium incision would place it
+                        # below the bottom of layer 1
+                        if (reach.strtop_incopt - reach.rbth) < reach.bot + buffer:
+                            # opt - stream thickness lower than layer 1 bottom
+                            # (with a buffer)
+                            self.logger.debug(
+                                "reach %s, incopt is: x\\/ "
+                                "below layer 1 bottom", reach.Index)
+                            new_elev = reach.bot + reach.rbth + buffer
+                            minslope_cond = (
+                                new_elev < strtop_withminslope
+                                if ustrm else
+                                new_elev > strtop_withminslope
+                            )
+                            if minslope_cond:
+                                # if layer bottom would put reach above
+                                # upstream reach/below downstream reach we
+                                # can only set to minimum slope from previous
+                                self.logger.debug(
+                                    "setting elevation to minslope "
+                                    "from previous")
+                                self.reaches.at[
+                                    reach.Index, "rtp"] = strtop_withminslope
+                                # this may still leave us below the
+                                # bottom of layer
+                            else:
+                                # otherwise we can move reach so that it
+                                # fits into layer 1
+                                self.logger.debug(
+                                    "setting elevation to %s, "
+                                    "above layer 1 bottom", new_elev)
+                                # set reach top so that it is above layer 1
+                                # bottom with a buffer
+                                # (allowing for bed thickness)
+                                self.reaches.at[reach.Index, "rtp"] = new_elev
+                        else:
+                            # strtop ok to set to "optimum incision"
+                            # set to "optimum incision"
+                            self.logger.debug("setting elevation to incopt")
+                            self.reaches.at[
+                                reach.Index, "rtp"] = reach.strtop_incopt
+                else:
+                    self.logger.debug(
+                        "reach %s, rtp is: below model top", reach.Index)
+                    minslope_cond = (
+                        rtp < strtop_withminslope
+                        if ustrm else
+                        rtp > strtop_withminslope
+                    )
+                    if (rtp - reach.rbth) < reach.bot + buffer:
+                        # rtp is below the bottom of layer 1
+                        self.logger.debug(
+                            "reach %s, rtp is: x\\/ below layer 1 bottom",
+                            reach.Index)
+                        new_elev = reach.bot + reach.rbth + buffer
+                        minslope_cond = (
+                            new_elev < strtop_withminslope
+                            if ustrm else
+                            new_elev > strtop_withminslope
+                        )
+                        if minslope_cond:
+                            # if layer bottom would put reach above
+                            # upstream reach we can only set to
+                            # minimum slope from upstream
+                            self.logger.debug(
+                                "setting elevation to minslope from upstream")
+                            self.reaches.at[
+                                reach.Index, "rtp"] = strtop_withminslope
+                            # this may still leave us below the
+                            # bottom of layer
+                        else:
+                            # otherwise we can move reach so that it
+                            # fits into layer 1
+                            self.logger.debug(
+                                "setting elevation to %s, "
+                                "above layer 1 bottom", new_elev)
+                            # set reach top so that it is above layer 1
+                            # bottom with a buffer
+                            # (allowing for bed thickness)
+                            self.reaches.at[reach.Index, "rtp"] = new_elev
+                    elif minslope_cond:
+                        # (rtp < strtop_withminslope
+                        # if ustrm
+                        # else rtp > strtop_withminslope)
+                        # below top but above/below minslope from
+                        # upstream/downstream
+                        self.logger.debug(
+                            "reach %s, rtp is: /\\ above upstream",
+                            reach.Index)
+                        self.logger.debug(
+                            "setting elevation to minslope from upstream")
+                        # set to minimum slope from previous reach
+                        self.reaches.at[reach.Index, "rtp"] = \
+                            strtop_withminslope
+                    # else it is above above bottom, below top and downstream
+                # update upreach for next iteration
+                prevreach_top = self.reaches.at[reach.Index, "rtp"]
+                # check if new stream top is above layer 1 with a buffer
+                # (allowing for bed thickness)
+                reachbed_elev = prevreach_top - reach.rbth
+                layerbots = _check_reach_v_laybot(reach, layerbots, buffer,
+                                                  reachbed_elev)
+                prevreach_mid = reach.mid_dist
+                # upreach_slope=reach.slope
+            self.reaches["bot"] = layerbots[0][reach_ij]
+        if fix_dis:
+            # fix dis for incised reaches
+            for k in range(self.model.dis.nlay.data - 1):
+                laythick = layerbots[k] - layerbots[
+                    k + 1]  # first one is layer 1 bottom - layer 2 bottom
+                self.logger.debug("checking layer %s thicknesses", k + 2)
+                thincells = laythick < minthick
+                self.logger.debug(
+                    "%s cells less than %s", thincells.sum(), minthick)
+                laythick[thincells] = minthick
+                layerbots[k + 1] = layerbots[k] - laythick
+            # flopy messing with external file names so apply in wrapper
+            # TODO remove line if flopy is patched (https://github.com/modflowpy/flopy/issues/1534)
+            _flopy_set3darray(self.model.dis.botm, layerbots)
+            # self.model.dis.botm.set_data(layerbots)
+
+
+    def _to_rno_elevs(
+            self, minslope=0.0001, minincise=0.2, minthick=0.5, buffer=0.5,
+            fix_dis=True):
+        """
+        Wes's hacky attempt to set reach elevations. Doesn't really ensure
+        anything, but the goal is:
+
+            0. get a list of cells with to_rtp > rtp-minslope*(delr+delc)/2
+            1. drop rtp of downstream reach (to_rno) when higher than rtp
+               (of rno)
+            2. grab all offensive reaches downstream of rno
+            3. check and fix all layer bottoms to be above minthick+buffer
+            4. adjust top, up only, to accomodate minincision or rtp above
+               cell top
 
         Parameters
         ----------
-        path : str
-            File path where the pickled object will be stored.
-        protocol : int
-            Default is pickle.HIGHEST_PROTOCOL.
+        minslope : float, default 1e-4
+            The minimum allowable slope between adjacent reaches
+            (to be considered flowing downstream).
+        minincise : float, default 0.2
+            The minimum allowable incision of a reach below the model top.
+        minthick : float, default 0.5
+            The minimum thickness of stream bed. Will try to ensure that this
+            is available below stream top before layer bottom.
+        buffer : float, default 0.5
+            The minimum cell thickness between the bottom of stream bed
+            (rtp-minthick) and the bottom of the layer 1 cell
+        fix_dis : bool, default True
+            Move layer elevations down where it is not possible to honor
+            minimum slope without going below layer 1 bottom.
+
+        Returns
+        -------
+        None
 
         """
-        with open(path, "wb") as f:
-            pickle.dump(self, f, protocol=protocol)
 
-    @classmethod
-    def from_pickle(cls, path, model):
-        """Read a pickled format from a file.
+        # copy some data
+        top = self.model.dis.top.array.copy()
+        botm = self.model.dis.botm.array.copy()
+        delr = self.model.dis.delr.data.copy()
+        delc = self.model.dis.delc.data.copy()
+        rdf = self.reaches.copy()
+        icols = rdf.columns.to_list()
+
+        # add some columns to rdf
+        rdf["ij"] = rdf.apply(lambda x: (int(x["i"]), int(x["j"])), axis=1)
+        # hopefully this sort of addresses local grid refinement?
+        rdf["mindz"] = minslope * \
+            (delr[rdf.loc[:, "j"]] + delc[rdf.loc[:, "i"]]) / 2.0
+        if "rbth" not in rdf.columns:
+            rdf["rbth"] = minthick
+            icols.append("rbth")
+        if "rtp" not in rdf.columns:
+            rdf["rtp"] = np.nan
+            # add to list of columns to be returned
+            icols.append("rtp")
+        if "incise" not in rdf.columns:
+            rdf["incise"] = minincise
+            icols.append("incise")
+        # reach specific so iterrows?
+        for idx, r in rdf.iterrows():
+            if np.isnan(r["rtp"]):
+                rdf.loc[idx, "rbth"] = np.max([r["rbth"], minthick])
+                rdf.loc[idx, "rtp"] = top[r["ij"]]-minincise
+        for idx, r in rdf.iterrows():
+            trno = int(r["to_rno"])
+            if trno != 0:
+                rdf.loc[idx, "to_rtp"] = rdf.loc[trno, "rtp"]
+        # start loop
+        loop = 0
+        cont = True
+        while cont:
+            bad_reaches = [i for i in rdf.index
+                           if rdf.loc[i, "to_rtp"] > rdf.loc[i, "rtp"] -
+                           rdf.loc[i, "mindz"]]
+            loop += 1
+            chg = 0
+            for br in bad_reaches:
+                rno = br
+                trno = int(rdf.loc[br, "to_rno"])
+                chglist = []
+                if trno != 0:
+                    # count how many downstream reaches offend
+                    # keep track of changes in elev
+                    dz = rdf.loc[rno, "mindz"]
+                    check = rdf.loc[trno, "rtp"] > rdf.loc[rno, "rtp"] - dz
+                    while trno != 0 and check:
+                        # keep list of dz in case another inflowing stream is
+                        # even lower
+                        chglist.append(trno)
+                        nelev = rdf.loc[rno, "rtp"] - dz
+                        # set to_rtp and rtp
+                        rdf.loc[rno, "to_rtp"] = nelev
+                        rdf.loc[trno, "rtp"] = nelev
+                        # move downstream
+                        rno = trno
+                        trno = rdf.loc[rno, "to_rno"]
+                        dz = rdf.loc[rno, "mindz"]
+
+                    # now adjust layering if necessary
+                    if len(chglist) > 0 and fix_dis:
+                        self.logger.debug(
+                            "adjusting top for %s reaches", len(chglist))
+                        for r in chglist:
+                            # bump top elev up to rtp+incise if need be
+                            new_top = rdf.loc[r, "rtp"] + rdf.loc[r, "incise"]
+                            if top[rdf.loc[r, "ij"]] < new_top:
+                                top[rdf.loc[r, "ij"]] = new_top
+                            # bump bottoms down if needed
+                            maxbot = rdf.loc[r, "rtp"] - rdf.loc[r, "rbth"] - buffer
+                            if botm[0][rdf.loc[r, "ij"]] >= maxbot:
+                                botdz = botm[0][rdf.loc[r, "ij"]] - maxbot
+                                for b in range(botm.shape[0]):
+                                    botm[b][rdf.loc[r, "ij"]] = \
+                                        botm[b][rdf.loc[r, "ij"]] - botdz
+
+                chg += len(chglist)
+            if chg == 0:
+                cont = False
+            else:
+                self.logger.debug("%s changed in loop %s", chg, loop)
+        setattr(self, "reaches", rdf[icols + ["to_rtp", "mindz"]])
+        self.model.dis.botm = botm
+        self.model.dis.top = top
+
+    def fix_reach_elevs(
+            self, minslope=1e-4, minincise=0.2, minthick=0.5, buffer=0.1,
+            fix_dis=True, direction="downstream", segbyseg=False,
+            to_rno_elevs=False):
+        """Fix reach elevations.
+
+        Notes
+        -----
+        Need to ensure reach elevation is:
+            0. below the top
+            1. below the upstream reach
+            2. above the minimum slope to the bottom reach elevation
+            3. above the base of layer 1
+        in modflow6 only reaches so maybe we should go just reach by reach
+        (nwt method went seg-by-seg then reach-by-reach)
 
         Parameters
         ----------
-        path : str
-            File path where the pickled object will be stored.
-        model : flopy.modflow.mf.Modflow
-            Instance of a flopy MODFLOW model.
+        minslope : float, default 1e-4
+            The minimum allowable slope between adjacent reaches
+            (to be considered flowing downstream).
+        minincise : float, default 0.2
+            The minimum allowable incision of a reach below the model top.
+        minthick : float, default 0.5
+            The minimum thickness of stream bed. Will try to ensure that this
+            is available below stream top before layer bottom.
+        buffer : float, default 0.5
+            The minimum cell thickness between the bottom of stream bed
+            (rtp-minthick) and the bottom of the layer 1 cell
+        fix_dis : bool, default True
+            Move layer elevations down where it is not possible to honor
+            minimum slope without going below layer 1 bottom.
+        direction : {"upstream", "downstream", "both"}, default "downstream"
+            Select whether elevations are set from ensuring a minimum slope
+            in a upstream or downstream direction.
+            If "upstream" will honor elevation at outlet reach
+                (if in model layer) and work upstream ensuring minimum slope.
+            If "downstream" will honor elevation at headwater reach
+                (if in model layer) and work downstream ensuring minimum slope.
+            If "both" will iterate "upstream" first and then "downstream",
+                handy is no constraint on stream elevations.
+        segbyseg : bool, default False
+            NOT IMPLEMENTED
+            Sets elevation of reaches segment by segment.
+            If True, will attempt to honor the elevations specified at the
+            upstream and downstream ends of each input line segment
+            (if they are in the top model layer and appropriately downstream).
+            If False will only attempt to honor elevations/incision at
+            headwaters and outlets.
+        to_rno_elevs : bool, default False
+            attempt to quickly ensure rtp of the downstream reach
+            is lower than rtp of the upstream reach
+
+        Returns
+        -------
+        None
 
         """
-        with open(path, "rb") as f:
-            obj = pickle.load(f)
-        obj.model = model
-        return obj
+        if segbyseg:
+            raise NotImplementedError("option 'segbyseg=True' not finished")
+            self._segbyseg_elevs(minslope, fix_dis, minthick)
+        elif to_rno_elevs:
+            self._to_rno_elevs(minslope, minincise, minthick, buffer, fix_dis)
+        else:
+            if direction == 'both':
+                direction = ['upstream', 'downstream']
+            else:
+                direction = [direction]
+            for d in direction:
+                self._reachbyreach_elevs(
+                    minslope, minincise, minthick, fix_dis, d)
+        return
+
+    def route_reaches(self, start, end, *, allow_indirect=False):
+        """Return a list of reach numbers that connect a pair of reaches.
+
+        Parameters
+        ----------
+        start, end : any
+            Start and end reach numbers (rno).
+        allow_indirect : bool, default False
+            If True, allow the route to go downstream from start to a
+            confluence, then route upstream to end. Defalut False allows
+            only a direct route along a single direction up or down.
+
+        Returns
+        -------
+        list
+
+        Raises
+        ------
+        IndexError
+            If start and/or end reach numbers are not valid.
+        ConnecionError
+            If start and end reach numbers do not connect.
+
+        Examples
+        --------
+        >>> import flopy
+        >>> import geopandas
+        >>> import swn
+        >>> lines = geopandas.GeoSeries.from_wkt([
+        ...    "LINESTRING (60 100, 60  80)",
+        ...    "LINESTRING (40 130, 60 100)",
+        ...    "LINESTRING (70 130, 60 100)"])
+        >>> lines.index += 100
+        >>> n = swn.SurfaceWaterNetwork.from_lines(lines)
+        >>> sim = flopy.mf6.MFSimulation()
+        >>> _ = flopy.mf6.ModflowTdis(sim, nper=1, time_units="days")
+        >>> gwf = flopy.mf6.ModflowGwf(sim)
+        >>> _ = flopy.mf6.ModflowGwfdis(
+        ...     gwf, nrow=3, ncol=2, delr=20.0, delc=20.0, idomain=1,
+        ...     length_units="meters", xorigin=30.0, yorigin=70.0)
+        >>> nm = swn.SwnMf6.from_swn_flopy(n, gwf)
+        >>> nm.reaches[["iseg", "ireach", "to_rno", "from_rnos", "segnum"]]
+             iseg  ireach  to_rno from_rnos  segnum
+        rno                                        
+        1       1       1       2        {}     101
+        2       1       2       3       {1}     101
+        3       1       3       6       {2}     101
+        4       2       1       5        {}     102
+        5       2       2       6       {4}     102
+        6       3       1       7    {3, 5}     100
+        7       3       2       0       {6}     100
+        >>> nm.route_reaches(1, 7)
+        [1, 2, 3, 6, 7]
+        >>> nm.reaches.loc[nm.route_reaches(1, 7), ["i", "j", "rlen"]]
+             i  j       rlen
+        rno                 
+        1    0  0  18.027756
+        2    0  1   6.009252
+        3    1  1  12.018504
+        6    1  1  10.000000
+        7    2  1  10.000000
+        """  # noqa
+        if start not in self.reaches.index:
+            raise IndexError(f"invalid start rno {start}")
+        if end not in self.reaches.index:
+            raise IndexError(f"invalid end rno {end}")
+        if start == end:
+            return [start]
+        to_rnos = dict(self.reaches.loc[self.reaches["to_rno"] != 0, "to_rno"])
+
+        def go_downstream(rno):
+            yield rno
+            if rno in to_rnos:
+                yield from go_downstream(to_rnos[rno])
+
+        con1 = list(go_downstream(start))
+        try:
+            # start is upstream, end is downstream
+            return con1[:(con1.index(end) + 1)]
+        except ValueError:
+            pass
+        con2 = list(go_downstream(end))
+        set2 = set(con2)
+        set1 = set(con1)
+        if set1.issubset(set2):
+            # start is downstream, end is upstream
+            drop = set1.intersection(set2)
+            drop.remove(start)
+            while drop:
+                drop.remove(con2.pop(-1))
+            return list(reversed(con2))
+        common = list(set1.intersection(set2))
+        if not allow_indirect or not common:
+            msg = f"{start} does not connect to {end}"
+            if not common:
+                msg += " -- reach networks are disjoint"
+            raise ConnectionError(msg)
+        # find the most upstream common rno or "confluence"
+        rno = common.pop()
+        idx1 = con1.index(rno)
+        idx2 = con2.index(rno)
+        while common:
+            rno = common.pop()
+            tmp1 = con1.index(rno)
+            if tmp1 < idx1:
+                idx1 = tmp1
+                idx2 = con2.index(rno)
+        return con1[:idx1] + list(reversed(con2[:idx2]))
+
+
+def _flopy_set3darray(flopyobj, array3d):
+    data = [{"filename": flopyobj[k].fname, "data":ar}
+            if flopyobj[k].fname else {"data": ar}
+            for k, ar in enumerate(array3d)]
+    flopyobj.set_data(data)
+
+
+def get_flopy_mf6_package(name: str):
+    """Returns a flopy.mf6 package.
+
+    Parameters
+    ----------
+    package : str
+        MODFLOW 6 package name, such as "drn" for DRAIN, or "GWT/SRC" for
+        Mass Source Loading.
+
+    Returns
+    -------
+    flopy.mf6.mfpackage.MFPackage
+        Subclass object.
+    """
+    import flopy.mf6
+
+    if not isinstance(name, str):
+        raise ValueError(f"packge must be a str type; found {type(name)!r}")
+    try:
+        return getattr(flopy.mf6, name)
+    except AttributeError:
+        pass
+    # try (e.g.) "GWF-DRN" -> "Gwfdrn"
+    name = "".join(x for x in list(name) if x.isalpha())
+    try:
+        return getattr(flopy.mf6, f"Modflow{name.title()}")
+    except AttributeError:
+        pass
+    # try (e.g.) "DRN" -> "drn"
+    return getattr(flopy.mf6, f"ModflowGwf{name.lower()}")
```

### Comparing `surface-water-network-0.5/swn/modflow/_misc.py` & `surface-water-network-0.6/swn/modflow/_misc.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,15 +147,15 @@
                         idxname, abbr_str(diff_s)))
         return
 
     def return_series(data):
         do_astype = True
         if isinstance(data, dict):
             try:
-                series = pd.Series(data, dtype=dtype)
+                series = pd.Series(data).astype(dtype)
                 do_astype = False
             except ValueError:
                 data = pd.Series(data)
         if do_astype:
             try:
                 series = data.astype(dtype)
             except TypeError:
```

### Comparing `surface-water-network-0.5/swn/modflow/_modelplot.py` & `surface-water-network-0.6/swn/modflow/_modelplot.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import numpy as np
+import pandas as pd
 
 from ..spatial import get_crs
 
 try:
     import matplotlib
     from matplotlib import cm, colors
     from matplotlib import pyplot as plt
@@ -191,15 +192,15 @@
         :param alpha: mpl transparency
         :param cbar: flag to plot with colorbar for layer
         :param label: label for colorbar
         """
         if self.ax is None:
             return
         if cmap is None:
-            cmap = cm.get_cmap('viridis')
+            cmap = matplotlib.colormaps.get_cmap('viridis')
         if self.mprj is None:
             transform = self.ax.transData
         else:
             transform = self.mprj
         if label is None:
             print("No label passed for colour bar")
             label = ""
@@ -234,15 +235,15 @@
             vals = np.ma.unique(x).compressed()
             bounds = np.append(np.sort(vals), vals.max() + 1)
             n = len(vals)
             cmap = colors.ListedColormap(
                 sns.color_palette('Set2', n).as_hex())
             norm = colors.BoundaryNorm(bounds, cmap.N)
         else:
-            cmap = cm.get_cmap(cmap_txt)
+            cmap = matplotlib.colormaps.get_cmap(cmap_txt)
             norm = MidpointNormalize(vmin=vmin, vmax=vmax, midpoint=0)
         self._add_plotlayer(x, cmap=cmap, norm=norm, zorder=zorder,
                             alpha=1, label=label, cbar=cbar)
         # if points is not None:
         #     self.ax.scatter(self.model.modelgrid.xcellcenters[
         #                         points.i, points.j],
         #                     self.model.modelgrid.ycellcenters[
@@ -265,15 +266,15 @@
     def _add_lines(self, lines, zorder=12, cmap_txt="RdGy"):
         import matplotlib.patheffects as pe
         col = [c for c in lines if c != 'geometry']
         if len(col) == 1:
             col = col[0]
             vmin = lines[col].min()
             vmax = lines[col].max()
-            cmap = cm.get_cmap(cmap_txt)
+            cmap = matplotlib.colormaps.get_cmap(cmap_txt)
             norm = MidpointNormalize(vmin=vmin, vmax=vmax, midpoint=0)
             cb = True
         else:
             col = None
             cmap = None
             norm = None
             cb = False
@@ -311,18 +312,19 @@
         sorted_df['csum'] = sorted_df[x].cumsum()
         x = 'csum'
     else:
         # will use this for seg dividers anyway
         sorted_df['csum'] = sorted_df[lentag].cumsum()
     if ax is None:
         fig, ax = plt.subplots(figsize=(8, 6))
-
-    sorted_df[[x] + cols].append(  # make sure we include end of final reach
-        sorted_df.iloc[[-1]][['csum']+cols].rename(
-            columns={'csum': x})).plot(x=x, ax=ax)
+    # make sure we include end of final reach
+    pd.concat([
+        sorted_df[[x] + cols],
+        sorted_df.iloc[[-1]][["csum"] + cols].rename(columns={"csum": x}),
+    ]).plot(x=x, ax=ax)
     # adding some window dressing
     end_seg = sorted_df.segnum.diff(-1) != 0
     start_seg = sorted_df.segnum.diff() != 0
     for _, s in sorted_df[end_seg].iterrows():
         ax.axvline(s["csum"], c='0.5', alpha=0.5, linestyle='--')
     trans = ax.get_xaxis_transform()
     for _, s in sorted_df[start_seg].iterrows():
```

### Comparing `surface-water-network-0.5/swn/modflow/_swnmodflow.py` & `surface-water-network-0.6/swn/modflow/_swnmodflow.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Interface for flopy's implementation for MODFLOW."""
 
 __all__ = ["SwnModflow"]
 
 import inspect
+import os
 from itertools import zip_longest
 
 import numpy as np
 import pandas as pd
 
 from ..util import abbr_str
 from ._base import SwnModflowBase
@@ -84,16 +85,17 @@
         Returns
         -------
         obj : swn.SwnModflow object
 
         Examples
         --------
         >>> import flopy
+        >>> import geopandas
         >>> import swn
-        >>> lines = swn.spatial.wkt_to_geoseries([
+        >>> lines = geopandas.GeoSeries.from_wkt([
         ...    "LINESTRING (60 100, 60  80)",
         ...    "LINESTRING (40 130, 60 100)",
         ...    "LINESTRING (70 130, 60 100)"])
         >>> lines.index += 100
         >>> n = swn.SurfaceWaterNetwork.from_lines(lines)
         >>> m = flopy.modflow.Modflow(version="mf2005")
         >>> _ = flopy.modflow.ModflowDis(
@@ -309,16 +311,17 @@
 
         If :py:attr:`segment_data` is already set, subsequent calls will
         reset the DataFrame and :py:attr:`segment_data_ts`.
 
         Examples
         --------
         >>> import flopy
+        >>> import geopandas
         >>> import swn
-        >>> lines = swn.spatial.wkt_to_geoseries([
+        >>> lines = geopandas.GeoSeries.from_wkt([
         ...    "LINESTRING (60 100, 60  80)",
         ...    "LINESTRING (40 130, 60 100)",
         ...    "LINESTRING (70 130, 60 100)"])
         >>> lines.index += 100
         >>> n = swn.SurfaceWaterNetwork.from_lines(lines)
         >>> m = flopy.modflow.Modflow(version="mf2005")
         >>> _ = flopy.modflow.ModflowDis(
@@ -414,16 +417,17 @@
         which : str, default = "all"
             Determine which segment_data rows should be set as "segments",
             "diversions" (determined from IUPSEG), or "all".
 
         Examples
         --------
         >>> import flopy
+        >>> import geopandas
         >>> import swn
-        >>> lines = swn.spatial.wkt_to_geoseries([
+        >>> lines = geopandas.GeoSeries.from_wkt([
         ...    "LINESTRING (60 100, 60  80)",
         ...    "LINESTRING (40 130, 60 100)",
         ...    "LINESTRING (70 130, 60 100)"])
         >>> lines.index += 100
         >>> n = swn.SurfaceWaterNetwork.from_lines(lines)
         >>> m = flopy.modflow.Modflow(version="mf2005")
         >>> _ = flopy.modflow.ModflowDis(
@@ -507,16 +511,17 @@
             Data to assigned from segments. If a pandas Series, then this is
             applied for each index matched by segnum. If a dict, then
             each item is applied for each key matched by segnum.
 
         Examples
         --------
         >>> import flopy
+        >>> import geopandas
         >>> import swn
-        >>> lines = swn.spatial.wkt_to_geoseries([
+        >>> lines = geopandas.GeoSeries.from_wkt([
         ...    "LINESTRING (60 100, 60  80)",
         ...    "LINESTRING (40 130, 60 100)",
         ...    "LINESTRING (70 130, 60 100)"])
         >>> lines.index += 100
         >>> n = swn.SurfaceWaterNetwork.from_lines(lines)
         >>> m = flopy.modflow.Modflow(version="mf2005")
         >>> _ = flopy.modflow.ModflowDis(
@@ -572,22 +577,23 @@
             Data to assigned from diversions. If a pandas Series, then this is
             applied for each index matched by divid. If a dict, then
             each item is applied for each key matched by divid.
 
         Examples
         --------
         >>> import flopy
+        >>> import geopandas
         >>> import swn
-        >>> lines = swn.spatial.wkt_to_geoseries([
+        >>> lines = geopandas.GeoSeries.from_wkt([
         ...    "LINESTRING (60 100, 60  80)",
         ...    "LINESTRING (40 130, 60 100)",
         ...    "LINESTRING (70 130, 60 100)"])
         >>> lines.index += 100
         >>> n = swn.SurfaceWaterNetwork.from_lines(lines)
-        >>> diversions = swn.spatial.wkt_to_geoseries([
+        >>> diversions = geopandas.GeoSeries.from_wkt([
         ...    "POINT (58 100)",
         ...    "POINT (58 100)"]).to_frame("geometry")
         >>> diversions.index += 10
         >>> diversions["rate"] = [1.1, 2.2]
         >>> n.set_diversions(diversions=diversions)
         >>> m = flopy.modflow.Modflow(version="mf2005")
         >>> _ = flopy.modflow.ModflowDis(
@@ -749,16 +755,17 @@
         Returns
         -------
         None
 
         Examples
         --------
         >>> import flopy
+        >>> import geopandas
         >>> import swn
-        >>> lines = swn.spatial.wkt_to_geoseries([
+        >>> lines = geopandas.GeoSeries.from_wkt([
         ...    "LINESTRING Z (60 100 14, 60  80 12)",
         ...    "LINESTRING Z (40 130 15, 60 100 14)",
         ...    "LINESTRING Z (70 130 15, 60 100 14)"])
         >>> lines.index += 100
         >>> n = swn.SurfaceWaterNetwork.from_lines(lines)
         >>> m = flopy.modflow.Modflow(version="mf2005")
         >>> _ = flopy.modflow.ModflowDis(
@@ -827,15 +834,15 @@
         swn = self._swn
         more_segment_columns = pd.concat([
             swn.pair_segments_frame(hyd_cond1, hyd_cond_out, "hcond"),
             swn.pair_segments_frame(thickness1, thickness_out, "thickm"),
             swn.pair_segments_frame(
                 width1, width_out, name="width", method="constant")
         ], axis=1, copy=False)
-        for name, series in more_segment_columns.iteritems():
+        for name, series in more_segment_columns.items():
             self.segments[name] = series
         self.segments["roughch"] = swn.segments_series(roughch)
 
         # Interpolate segment properties to each reach
         self.set_reach_data_from_segments(
             "thickm", thickness1, thickness_out)
         self.set_reach_data_from_segments(
@@ -889,20 +896,24 @@
             self.set_segment_data_from_scalar("depth2", 1.0, "diversions")
 
     def set_sfr_obj(self, **kwds):
         """Set MODFLOW SFR package data to flopy model.
 
         Parameters
         ----------
-        **kwargs : dict, optional
+        **kwds : dict, optional
             Passed to flopy.modflow.mfsfr2.ModflowSfr2.
+
+        Returns
+        -------
+        flopy.modflow.mfsfr2.ModflowSfr2
         """
         import flopy
 
-        flopy.modflow.mfsfr2.ModflowSfr2(
+        return flopy.modflow.mfsfr2.ModflowSfr2(
             model=self.model,
             reach_data=self.flopy_reach_data(),
             segment_data=self.flopy_segment_data(),
             **kwds)
 
     def get_seg_ijk(self):
         """
@@ -1216,15 +1227,15 @@
             # calculate reach strtops
             seg["strtop"] = seg["cmids"].multiply(seg_slope) + seg_elevup
             # seg["slope"]= #!!!!! use m.sfr.get_slopes() method
             return seg
         self.segment_data["Zslope"] = \
             ((self.segment_data["elevdn"] - self.segment_data["elevup"]) /
              self.segment_data["seglen"])
-        segs = self.reaches.groupby("iseg")
+        segs = self.reaches.groupby("iseg", group_keys=False)
         self.reaches["seglen"] = segs.rchlen.cumsum()
         self.reaches = segs.apply(reach_elevs)
         return self.reaches
 
     def set_topbot_elevs_at_reaches(self):
         """
         Legacy method to add model top and bottom information to reaches.
@@ -1577,16 +1588,17 @@
             If start and/or end reach identifiers are not valid.
         ConnecionError
             If start and end reach identifiers do not connect.
 
         Examples
         --------
         >>> import flopy
+        >>> import geopandas
         >>> import swn
-        >>> lines = swn.spatial.wkt_to_geoseries([
+        >>> lines = geopandas.GeoSeries.from_wkt([
         ...    "LINESTRING (60 100, 60  80)",
         ...    "LINESTRING (40 130, 60 100)",
         ...    "LINESTRING (70 130, 60 100)"])
         >>> lines.index += 100
         >>> n = swn.SurfaceWaterNetwork.from_lines(lines)
         >>> m = flopy.modflow.Modflow(version="mf2005")
         >>> _ = flopy.modflow.ModflowDis(
@@ -1629,15 +1641,15 @@
                 ~self.reaches.diversion, ["segnum", "iseg"]]
         else:
             segnum_iseg_df = self.reaches[["segnum", "iseg"]]
         segnum_iseg = segnum_iseg_df.drop_duplicates().set_index(
             "segnum", verify_integrity=True).iseg
 
         to_reachids = {}
-        for segnum, iseg in segnum_iseg.iteritems():
+        for segnum, iseg in segnum_iseg.items():
             sel = self.reaches.index[self.reaches.iseg == iseg]
             to_reachids.update(dict(zip(sel[0:-1], sel[1:])))
             next_segnum = self.segments.to_segnum[segnum]
             next_reachids = self.reaches.index[
                 self.reaches.segnum == next_segnum]
             if len(next_reachids) > 0:
                 to_reachids[sel[-1]] = next_reachids[0]
@@ -1676,7 +1688,330 @@
         while common:
             reachID = common.pop()
             tmp1 = con1.index(reachID)
             if tmp1 < idx1:
                 idx1 = tmp1
                 idx2 = con2.index(reachID)
         return con1[:idx1] + list(reversed(con2[:idx2]))
+
+    def package_period_frame(
+            self, package: str, style: str, auxiliary=[], **kwds):
+        """Return DataFrame of stress period data for MODFLOW packages.
+
+        This DataFrame is derived from the reaches DataFrame, and is
+        implemented using flopy.modflow package's ``stress_period_data``.
+
+        Parameters
+        ----------
+        package : str
+            MODFLOW package name, such as "drn" for DRAIN.
+        style : str
+            If "native", all indicies (including kij) use one-based notation.
+            Also use k,i,j columns (as str) rather than cellid.
+            If "flopy", all indices (including rno) use zero-based notation.
+            Also use cellid as a tuple.
+        auxiliary : str, list, optional
+            String or list of auxiliary variable names. Default [].
+        **kwds : dict, optional
+            Keyword arguments used for ``get_default_dtype``, if available.
+            A common keyword is ``structured=True``.
+
+        Returns
+        -------
+        DataFrame
+
+        See Also
+        --------
+        SwnModflow.flopy_package_period : Dict of lists of lists for flopy.
+
+        Examples
+        --------
+        >>> import flopy
+        >>> import geopandas
+        >>> import swn
+        >>> lines = geopandas.GeoSeries.from_wkt([
+        ...    "LINESTRING (60 100, 60  80)",
+        ...    "LINESTRING (40 130, 60 100)",
+        ...    "LINESTRING (70 130, 60 100)"])
+        >>> lines.index += 100
+        >>> n = swn.SurfaceWaterNetwork.from_lines(lines)
+        >>> m = flopy.modflow.Modflow(version="mf2005")
+        >>> _ = flopy.modflow.ModflowDis(
+        ...     m, nrow=3, ncol=2, delr=20.0, delc=20.0, xul=30.0, yul=130.0,
+        ...     top=15.0, botm=10.0)
+        >>> _ = flopy.modflow.ModflowBas(m)
+        >>> nm = swn.modflow.SwnModflow.from_swn_flopy(n, m)
+        >>> nm.set_reach_data_from_array("elev", m.dis.top.array)
+        >>> nm.reaches["dlen"] = nm.reaches.length
+        >>> nm.reaches["cond"] = nm.reaches.dlen * 10.0
+        >>> nm.package_period_frame("drn", "native", auxiliary="dlen")
+                     k  i  j  elev        cond       dlen
+        per reachID                                      
+        1   1        1  1  1  15.0  180.277564  18.027756
+            2        1  1  2  15.0   60.092521   6.009252
+            3        1  2  2  15.0  120.185043  12.018504
+            4        1  1  2  15.0  210.818511  21.081851
+            5        1  2  2  15.0  105.409255  10.540926
+            6        1  2  2  15.0  100.000000  10.000000
+            7        1  3  2  15.0  100.000000  10.000000
+        """
+        from inspect import signature
+
+        dat = pd.DataFrame(self.reaches.copy())
+        dat["ibound"] = \
+            self.model.bas6.ibound.array[dat["k"], dat["i"], dat["j"]]
+        if style == "native":
+            # Convert from zero-based to one-based notation
+            dat[list("kij")] += 1
+        elif style == "flopy":
+            pass
+        else:
+            raise ValueError("'style' must be either 'native' or 'flopy'")
+
+        Mfpak = get_flopy_modflow_package(package)
+        sig = signature(Mfpak.get_default_dtype)
+        gdd_kwds = {}
+        for kwarg, value in kwds.items():
+            if kwarg in sig.parameters:
+                gdd_kwds[kwarg] = value
+            else:
+                self.logger.warning(
+                    "%s %r specified, but not part of the "
+                    "get_default_dtype signature", kwarg, value)
+        dtype = Mfpak.get_default_dtype()
+        if auxiliary:
+            dtype = Mfpak.add_to_dtype(dtype, auxiliary, float)
+        # check missing columns
+        missing = []
+        for name in dtype.names:
+            if name not in dat.columns:
+                missing.append(name)
+        if missing:
+            raise KeyError(
+                "missing {} reach series needed for {}: {}"
+                .format(len(missing), Mfpak.__name__, ", ".join(missing)))
+        dat = dat.loc[:, dtype.names]
+        if self.model.dis.nper != 1:
+            self.logger.warning(
+                "only preparing stress period data for the first "
+                "stress period of %s", self.model.dis.nper)
+        dat["per"] = 1
+        if style == "flopy":
+            dat["per"] -= 1
+        return dat.reset_index().set_index(["per", "reachID"])
+
+    def write_package_period(self, package: str, fname, auxiliary=[]):
+        r"""
+        Write PERIOD file for MODFLOW packages, to be used within OPEN/CLOSE.
+
+        Parameters
+        ----------
+        package : str
+            MODFLOW package name, such as "drn" for DRAIN.
+        fname : str or path-like
+            Output file name, with str formatting for stress period number
+            which starts numbering from 1. For example, "drn_sp{:02d}.txt" to
+            create "drn_sp01.txt" for the first stress period.
+        auxiliary : str, list, optional
+            String or list of auxiliary variable names. Default [].
+
+        Returns
+        -------
+        None
+
+        See Also
+        --------
+        SwnModflow.package_period_frame : Dataframe generator.
+        SwnModflow.flopy_package_period : Dict of lists of lists for flopy.
+
+        Examples
+        --------
+        >>> import flopy
+        >>> import geopandas
+        >>> import pandas as pd
+        >>> import swn
+        >>> from tempfile import TemporaryDirectory
+        >>> from pathlib import Path
+        >>> lines = geopandas.GeoSeries.from_wkt([
+        ...    "LINESTRING (60 100, 60  80)",
+        ...    "LINESTRING (40 130, 60 100)",
+        ...    "LINESTRING (70 130, 60 100)"])
+        >>> lines.index += 100
+        >>> n = swn.SurfaceWaterNetwork.from_lines(lines)
+        >>> tmp_dir_obj = TemporaryDirectory()
+        >>> dir = Path(tmp_dir_obj.name)
+        >>> m = flopy.modflow.Modflow("model", version="mf2005", model_ws=str(dir))
+        >>> _ = flopy.modflow.ModflowDis(
+        ...     m, nrow=3, ncol=2, delr=20.0, delc=20.0, xul=30.0, yul=130.0,
+        ...     top=15.0, botm=10.0)
+        >>> _ = flopy.modflow.ModflowBas(m)
+        >>> nm = swn.modflow.SwnModflow.from_swn_flopy(n, m)
+        >>> nm.set_reach_data_from_array("elev", m.dis.top.array)
+        >>> nm.reaches["dlen"] = nm.reaches.length.round(2)
+        >>> nm.reaches["cond"] = (nm.reaches.length * 10.0).round(2)
+        >>> fname_tpl = dir / "model_drn_{:02d}.dat"
+        >>> fname_01 = dir / "model_drn_01.dat"
+        >>> nm.write_package_period("drn", fname_tpl, auxiliary="dlen")
+        >>> print(fname_01.read_text(), end="")
+        1 1 1 15.0 180.28 18.03
+        1 1 2 15.0  60.09  6.01
+        1 2 2 15.0 120.19 12.02
+        1 1 2 15.0 210.82 21.08
+        1 2 2 15.0 105.41 10.54
+        1 2 2 15.0 100.00 10.00
+        1 3 2 15.0 100.00 10.00
+        >>> drn = flopy.modflow.ModflowDrn(
+        ...     m, stress_period_data={
+        ...         0: flopy.modflow.ModflowDrn.get_empty(len(nm.reaches))})
+        >>> m.write_input()
+        >>> with open(dir / "model.drn", "w") as fp:
+        ...     _ = fp.write("7 0 AUX DLEN\n")
+        ...     _ = fp.write("7 0\n")
+        ...     _ = fp.write("OPEN/CLOSE model_drn_01.dat\n")
+        >>> success, buff = m.run_model()  # doctest: +SKIP
+        >>> tmp_dir_obj.cleanup()
+
+        """
+        spdf = self.package_period_frame(
+            package, "native", auxiliary=auxiliary)
+        if isinstance(fname, os.PathLike):
+            fname = os.fsdecode(fname)
+        for per, df in spdf.groupby("per"):
+            per_fname = fname.format(per)
+            self.logger.debug("writing period file %s", per_fname)
+            with open(per_fname, "w") as fp:
+                fp.write(df.to_string(header=False, index=False) + "\n")
+
+    def flopy_package_period(
+            self, package: str, auxiliary=[], **kwds):
+        """Return dict of lists of lists for flopy's stress_period_data.
+
+        Parameters
+        ----------
+        package : str
+            MODFLOW package name, such as "drn" for DRAIN.
+        auxiliary : str, list, optional
+            String or list of auxiliary variable names. Default [].
+        **kwds : dict, optional
+            Keyword arguments used for ``get_default_dtype``, if available.
+            A common keyword is ``structured=True``.
+
+        Returns
+        -------
+        dict
+
+        See Also
+        --------
+        SwnModflow.package_period_frame : Dataframe generator.
+        SwnModflow.set_package_obj : Set MODFLOW package data to flopy model.
+
+        Examples
+        --------
+        >>> import flopy
+        >>> import geopandas
+        >>> import pandas as pd
+        >>> import swn
+        >>> lines = geopandas.GeoSeries.from_wkt([
+        ...    "LINESTRING (60 100, 60  80)",
+        ...    "LINESTRING (40 130, 60 100)",
+        ...    "LINESTRING (70 130, 60 100)"])
+        >>> lines.index += 100
+        >>> n = swn.SurfaceWaterNetwork.from_lines(lines)
+        >>> m = flopy.modflow.Modflow(version="mf2005")
+        >>> _ = flopy.modflow.ModflowDis(
+        ...     m, nrow=3, ncol=2, delr=20.0, delc=20.0, xul=30.0, yul=130.0,
+        ...     top=15.0, botm=10.0)
+        >>> _ = flopy.modflow.ModflowBas(m)
+        >>> nm = swn.modflow.SwnModflow.from_swn_flopy(n, m)
+        >>> nm.set_reach_data_from_array("elev", m.dis.top.array)
+        >>> nm.reaches["dlen"] = nm.reaches.length
+        >>> nm.reaches["cond"] = nm.reaches.dlen * 10.0
+        >>> drn = nm.set_package_obj("drn", auxiliary="dlen")
+        >>> pd.DataFrame(drn.stress_period_data[0])
+           k  i  j  elev        cond       dlen
+        0  0  0  0  15.0  180.277557  18.027756
+        1  0  0  1  15.0   60.092522   6.009252
+        2  0  1  1  15.0  120.185043  12.018504
+        3  0  0  1  15.0  210.818512  21.081852
+        4  0  1  1  15.0  105.409256  10.540926
+        5  0  1  1  15.0  100.000000  10.000000
+        6  0  2  1  15.0  100.000000  10.000000
+        """
+        spdf = self.package_period_frame(
+            package, "flopy", auxiliary=auxiliary, **kwds)
+        Mfpak = get_flopy_modflow_package(package)
+        dtype = Mfpak.get_default_dtype()
+        if auxiliary:
+            dtype = Mfpak.add_to_dtype(dtype, auxiliary, np.float32)
+        # change dtypes
+        for nme, dtp in dtype.descr:
+            if spdf[nme].dtype != dtp:
+                spdf[nme] = spdf[nme].astype(dtp)
+        spd = {}
+        for per, df in spdf.groupby("per"):
+            spd[per] = df.to_records(index=False)
+        return spd
+
+    def set_package_obj(self, package: str, auxiliary=None, **kwds):
+        """Set MODFLOW package data to flopy model.
+
+        Parameters
+        ----------
+        package : str
+            MODFLOW package name, such as "drn" for DRAIN.
+        auxiliary : list, optional
+            List of auxiliary names, which must be columns in the reaches
+            frame.
+        **kwds : dict, optional
+            Passed to flopy.modflow.mfsfr2.ModflowSfr2.
+
+        Notes
+        -----
+        Flopy is sometimes limited with writing "AUX name" in the header to
+        describe auxiliary variables. This stress package file may need to be
+        edited after written by flopy to work as expected.
+
+        See Also
+        --------
+        SwnModflow.flopy_package_period : Used internally to set data.
+
+        Returns
+        -------
+        flopy.pakbase.Package
+        """
+        if "stress_period_data" not in kwds:
+            kwds["stress_period_data"] = self.flopy_package_period(
+                package=package, auxiliary=auxiliary)
+        Mfpak = get_flopy_modflow_package(package)
+        dtype = Mfpak.get_default_dtype()
+        if auxiliary:
+            self.logger.warning(
+                'flopy does not always write "AUX %s" to stress package file',
+                auxiliary)
+            dtype = Mfpak.add_to_dtype(dtype, auxiliary, np.float32)
+        return Mfpak(self.model, dtype=dtype, **kwds)
+
+
+def get_flopy_modflow_package(name: str):
+    """Returns a flopy.modflow package.
+
+    Parameters
+    ----------
+    package : str
+        MODFLOW package name, such as "drn" for DRAIN.
+
+    Returns
+    -------
+    flopy.pakbase.Package
+        Subclass object.
+    """
+    import flopy.modflow
+
+    if not isinstance(name, str):
+        raise ValueError(f"packge must be a str type; found {type(name)!r}")
+    try:
+        return getattr(flopy.modflow, name)
+    except AttributeError:
+        pass
+    # keep only alpha chars, try again
+    name = "".join(x for x in list(name) if x.isalpha())
+    return getattr(flopy.modflow, f"Modflow{name.title()}")
```

### Comparing `surface-water-network-0.5/swn/spatial.py` & `surface-water-network-0.6/swn/spatial.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,49 +1,52 @@
 """Spatial methods."""
 
 __all__ = [
-    "get_sindex", "interp_2d_to_3d",
-    "wkt_to_dataframe", "wkt_to_geodataframe", "wkt_to_geoseries",
+    "interp_2d_to_3d",
     "force_2d", "round_coords", "compare_crs", "get_crs",
     "bias_substring",
     "find_location_pairs", "location_pair_geoms",
 ]
 
 from warnings import warn
 
 import geopandas
 import numpy as np
 import pandas as pd
 import pyproj
-from shapely import wkt
-from shapely.geometry import Point
+import shapely
+from shapely import wkb, wkt
+from shapely.geometry import Point, MultiLineString
 
 try:
     from geopandas.tools import sjoin
 except ImportError:
     sjoin = False
 
 try:
     import rtree
     from rtree.index import Index
 except ImportError:
     rtree = False
 
+from .compat import SHAPELY_GE_20
 from .util import is_location_frame
 
 
 # default threshold size of geometries when Rtree index is built
 rtree_threshold = 100
 
 
 def get_sindex(gdf):
     """Get or build an R-Tree spatial index.
 
-    Particularly useful for geopandas<0.2.0;>0.7.0;0.9.0
+    .. deprecated:: 0.6
+        This method is no longer used.
     """
+    warn("get_sindex is no longer used", DeprecationWarning, stacklevel=2)
     sindex = None
     if (hasattr(gdf, '_rtree_sindex')):
         return getattr(gdf, '_rtree_sindex')
     if (isinstance(gdf, geopandas.GeoDataFrame) and
             hasattr(gdf.geometry, 'sindex')):
         sindex = gdf.geometry.sindex
     elif isinstance(gdf, geopandas.GeoSeries) and hasattr(gdf, 'sindex'):
@@ -93,14 +96,17 @@
     hx = gt[1] / 2.0
     hy = gt[5] / 2.0
     div = gt[1] * gt[5]
     ny, nx = grid.shape
     ar = np.pad(grid, 1, 'symmetric')
 
     def geom2dto3d(geom):
+        if geom.geom_type == "MultiLineString":
+            # Recursive call
+            return MultiLineString([geom2dto3d(part) for part in geom.geoms])
         x, y = geom.xy
         x = np.array(x)
         y = np.array(y)
         # Determine outside points
         outside = (
             (x < gt[0]) | (x > (gt[0] + nx * gt[1])) |
             (y > gt[3]) | (y < (gt[3] + ny * gt[5])))
@@ -130,42 +136,61 @@
              ar[iy2, ix2] * dx1 * dy1 / div)
         return type(geom)(zip(x, y, z))
 
     return gs.apply(geom2dto3d)
 
 
 def wkt_to_dataframe(wkt_list, geom_name='geometry'):
-    """Convert list of WKT strings to a DataFrame."""
+    """Convert list of WKT strings to a DataFrame.
+
+    .. deprecated:: 0.6
+        Use :meth:`geopandas.GeoSeries.from_wkt` with ``pandas.DataFrame``
+    """
+    warn("wkt_to_dataframe: Use geopandas.GeoSeries.from_wkt with "
+         "pandas.DataFrame instead",
+         DeprecationWarning, stacklevel=2)
     df = pd.DataFrame({'wkt': wkt_list})
     df[geom_name] = df['wkt'].apply(wkt.loads)
     return df.drop(columns="wkt")
 
 
 def wkt_to_geodataframe(wkt_list, geom_name='geometry'):
-    """Convert list of WKT strings to a GeoDataFrame."""
-    return geopandas.GeoDataFrame(
-            wkt_to_dataframe(wkt_list, geom_name), geometry=geom_name)
+    """Convert list of WKT strings to a GeoDataFrame.
+
+    .. deprecated:: 0.6
+        Use :meth:`geopandas.GeoSeries.from_wkt` with ``.to_frame("geometry")``
+    """
+    warn("wkt_to_geodataframe: Use geopandas.GeoSeries.from_wkt with "
+         '.to_frame("geometry") instead',
+         DeprecationWarning, stacklevel=2)
+    gdf = geopandas.GeoSeries.from_wkt(wkt_list).to_frame(geom_name)
+    return gdf.set_geometry(geom_name)
 
 
 def wkt_to_geoseries(wkt_list, geom_name=None):
-    """Convert list of WKT strings to a GeoSeries."""
-    geom = geopandas.GeoSeries([wkt.loads(x) for x in wkt_list])
-    if geom_name is not None:
-        geom.name = geom_name
-    return geom
+    """Convert list of WKT strings to a GeoSeries.
+
+    .. deprecated:: 0.6
+        Use :meth:`geopandas.GeoSeries.from_wkt`
+    """
+    warn("wkt_to_geoseries: use geopandas.GeoSeries.from_wkt instead",
+         DeprecationWarning, stacklevel=2)
+    return geopandas.GeoSeries.from_wkt(wkt_list, name=geom_name)
 
 
 def force_2d(gs):
     """Force any geometry GeoSeries as 2D geometries."""
-    return wkt_to_geoseries(gs.apply(wkt.dumps, output_dimension=2))
+    if SHAPELY_GE_20:
+        return gs.apply(shapely.force_2d)
+    return geopandas.GeoSeries.from_wkb(gs.apply(wkb.dumps, output_dimension=2))
 
 
 def round_coords(gs, rounding_precision=3):
     """Round coordinate precision of a GeoSeries."""
-    return wkt_to_geoseries(
+    return geopandas.GeoSeries.from_wkt(
             gs.apply(wkt.dumps, rounding_precision=rounding_precision))
 
 
 def visible_wkt(geom):
     """Re-generate geometry to only visible WKT, erase machine precision."""
     return wkt.loads(geom.wkt)
 
@@ -232,14 +257,16 @@
     ds = 1.0
     if downstream_bias > 0.0:
         ds = 1.0 - downstream_bias
     else:
         us = float(-downstream_bias)
     # move start/end points so they are not exactly at start/end
     args = tuple(np.clip([us, ds], end_cut, 1.0 - end_cut))
+    if SHAPELY_GE_20 and gs.has_z.any():
+        gs = shapely.force_2d(gs)
     return gs.apply(substring, args=args, normalized=True)
 
 
 def find_segnum_in_swn(n, geom):
     """Return segnum within a catchment or nearest a segment to a geometry.
 
     If a catchment polygon is provided, this is used to find if the point
@@ -275,108 +302,142 @@
     res = n.locate_geoms(geom)
     res["is_within_catchment"] = res.method == "catchment"
     res.rename(columns={"dist_to_seg": "dist_to_segnum"}, inplace=True)
     return pd.DataFrame(
         res[["segnum", "dist_to_segnum", "is_within_catchment"]])
 
 
-def find_location_pairs(loc_df, n):
+def find_location_pairs(loc_df, n, *, all_pairs=False, exclude_branches=False):
     r"""Find pairs of locations in a surface water network that are connected.
 
     Parameters
     ----------
     loc_df : geopandas.GeoDataFrame or pandas.DataFrame
         Location [geo] dataframe, usually created by
         :py:meth:`SurfaceWaterNetwork.locate_geoms`.
     n : SurfaceWaterNetwork
         A surface water network to evaluate.
+    all_pairs : bool, default False
+        If True, find all combination pairs, including those that overlap.
+        Default False will find shortest pair combinations only.
+    exclude_branches : bool, default False
+        If True, only pairs without branches between are permitted.
 
     Returns
     -------
     set
         tuple of location index (upstream, downstream).
 
     See Also
     --------
     location_pair_geoms : Extract linestring geometry for location pairs.
 
     Examples
     --------
     >>> import swn
+    >>> import geopandas
     >>> from shapely import wkt
     >>> lines = geopandas.GeoSeries(list(wkt.loads('''\
     ... MULTILINESTRING(
     ...     (380 490, 370 420), (300 460, 370 420), (370 420, 420 330),
     ...     (190 250, 280 270), (225 180, 280 270), (280 270, 420 330),
     ...     (420 330, 584 250), (520 220, 584 250), (584 250, 710 160),
     ...     (740 270, 710 160), (735 350, 740 270), (880 320, 740 270),
     ...     (925 370, 880 320), (974 300, 880 320), (760 460, 735 350),
     ...     (650 430, 735 350), (710 160, 770 100), (700  90, 770 100),
     ...     (770 100, 820  40))''').geoms))
     >>> lines.index += 100
     >>> n = swn.SurfaceWaterNetwork.from_lines(lines)
-    >>> obs_gs = swn.spatial.wkt_to_geoseries([
+    >>> obs_gs = geopandas.GeoSeries.from_wkt([
     ...    "POINT (370 400)",
     ...    "POINT (720 230)",
     ...    "POINT (780 70)",
     ...    "POINT (606 256)",
     ...    "POINT (690 170)"])
     >>> obs_gs.index += 11
     >>> obs_match = n.locate_geoms(obs_gs)
     >>> obs_match[["segnum", "seg_ndist"]]
         segnum  seg_ndist
     11     102   0.169811
     12     109   0.384615
     13     118   0.377049
     14     108   0.093093
     15     108   0.857357
-    >>> pairs = swn.spatial.find_location_pairs(obs_match, n)
-    >>> sorted(pairs)
+    >>> sorted(swn.spatial.find_location_pairs(obs_match, n))
     [(11, 14), (12, 13), (14, 15), (15, 13)]
+    >>> sorted(swn.spatial.find_location_pairs(obs_match, n, all_pairs=True))
+    [(11, 13), (11, 14), (11, 15), (12, 13), (14, 13), (14, 15), (15, 13)]
+    >>> swn.spatial.find_location_pairs(obs_match, n, exclude_branches=True)
+    {(14, 15)}
     """
     from .core import SurfaceWaterNetwork
 
     # Check inputs
     if not isinstance(n, SurfaceWaterNetwork):
         raise TypeError("expected 'n' as an instance of SurfaceWaterNetwork")
     is_location_frame(loc_df, geom_required=False)
     segnum_is_in_index = loc_df.segnum.isin(n.segments.index)
     if not segnum_is_in_index.all():
         raise ValueError(
             "loc_df has segnum values not found in surface water network")
 
     to_segnums = dict(n.to_segnums)
+    if exclude_branches:
+        from_segnums = dict(n.from_segnums)
     loc_df = loc_df[["segnum", "seg_ndist"]].assign(_="")  # also does .copy()
     loc_segnum_s = set(loc_df.segnum)
     loc_df["sequence"] = n.segments.sequence[loc_df.segnum].values
     loc_df.sort_values(["sequence", "seg_ndist"], inplace=True)
     # Start from upstream locations, querying downstream, except last
     pairs = set()
-    for upstream_idx, upstream_segnum in loc_df.segnum.iloc[:-1].iteritems():
-        downstream_idx = None
-        # First case that the downstream segnum is in the same segnum
-        next_loc = loc_df.iloc[loc_df.index.get_loc(upstream_idx) + 1]
-        if next_loc.segnum == upstream_segnum:
-            downstream_idx = next_loc.name
-        else:
-            # otherwise search downstream
-            cur_segnum = upstream_segnum
+    for us_idx, us_segnum in loc_df.segnum.iloc[:-1].items():
+        next_iloc = loc_df.index.get_loc(us_idx) + 1
+        if all_pairs:
+            # find downstream segnums in the same segnum
+            sel = loc_df.iloc[next_iloc:].segnum == us_segnum
+            for ds_idx in sel[sel].index:
+                pairs.add((us_idx, ds_idx))
+            # continue searching downstream
+            cur_segnum = us_segnum
             while True:
                 if cur_segnum in to_segnums:
                     next_segnum = to_segnums[cur_segnum]
-                    if next_segnum in loc_segnum_s:
-                        downstream_idx = loc_df.segnum[
-                            loc_df.segnum == next_segnum].index[0]
-                        break
+                    if (exclude_branches and
+                            len(from_segnums.get(next_segnum, [])) > 1):
+                        break  # stop searching due to branch
+                    sel = loc_df["segnum"] == next_segnum
+                    for ds_idx in sel[sel].index:
+                        pairs.add((us_idx, ds_idx))
                 else:
-                    # print(f"no downstream location from {upstream_idx}")
-                    break
+                    break  # stop searching due to no downstream location
                 cur_segnum = next_segnum
-        if downstream_idx is not None:
-            pairs.add((upstream_idx, downstream_idx))
+        else:
+            ds_idx = None
+            # First case that the downstream segnum is in the same segnum
+            next_loc = loc_df.iloc[next_iloc]
+            if next_loc.segnum == us_segnum:
+                ds_idx = next_loc.name
+            else:
+                # otherwise search downstream
+                cur_segnum = us_segnum
+                while True:
+                    if cur_segnum in to_segnums:
+                        next_segnum = to_segnums[cur_segnum]
+                        if (exclude_branches and
+                                len(from_segnums.get(next_segnum, [])) > 1):
+                            break  # no pair due to branch
+                        if next_segnum in loc_segnum_s:
+                            ds_idx = loc_df.segnum[
+                                loc_df.segnum == next_segnum].index[0]
+                            break  # found pair
+                    else:
+                        break  # no pair due to no downstream location
+                    cur_segnum = next_segnum
+            if ds_idx is not None:
+                pairs.add((us_idx, ds_idx))
     return pairs
 
 
 def location_pair_geoms(pairs, loc_df, n):
     r"""Extract linestring geometry for location pairs, that follow segments.
 
     Parameters
@@ -407,15 +468,15 @@
     ...     (420 330, 584 250), (520 220, 584 250), (584 250, 710 160),
     ...     (740 270, 710 160), (735 350, 740 270), (880 320, 740 270),
     ...     (925 370, 880 320), (974 300, 880 320), (760 460, 735 350),
     ...     (650 430, 735 350), (710 160, 770 100), (700  90, 770 100),
     ...     (770 100, 820  40))''').geoms))
     >>> lines.index += 100
     >>> n = swn.SurfaceWaterNetwork.from_lines(lines)
-    >>> obs_gs = swn.spatial.wkt_to_geoseries([
+    >>> obs_gs = geopandas.GeoSeries.from_wkt([
     ...    "POINT (370 400)",
     ...    "POINT (720 230)",
     ...    "POINT (780 70)",
     ...    "POINT (606 256)",
     ...    "POINT (690 170)"])
     >>> obs_gs.index += 11
     >>> obs_match = n.locate_geoms(obs_gs)
@@ -443,39 +504,43 @@
         raise TypeError("expected 'n' as an instance of SurfaceWaterNetwork")
     is_location_frame(loc_df, geom_required=False)
     segnum_is_in_index = loc_df.segnum.isin(n.segments.index)
     if not segnum_is_in_index.all():
         raise ValueError(
             "loc_df has segnum values not found in surface water network")
 
+    seg_geom = force_2d(n.segments.geometry)
     geoms_d = {}
     for pair in pairs:
         upstream_idx, downstream_idx = pair
         upstream = loc_df.loc[upstream_idx]
         downstream = loc_df.loc[downstream_idx]
         if upstream.segnum == downstream.segnum:
             # pairs are in the same segnum
             geoms_d[pair] = substring(
-                n.segments.geometry[upstream.segnum],
+                seg_geom[upstream.segnum],
                 upstream.seg_ndist, downstream.seg_ndist,
                 normalized=True)
         else:
             try:
                 segnums = n.route_segnums(upstream.segnum, downstream.segnum)
             except ConnectionError:
                 geoms_d[pair] = None
                 continue
             assert segnums[0] == upstream.segnum
             assert segnums[-1] == downstream.segnum
             geoms = [
                 substring(
-                    n.segments.geometry[upstream.segnum],
+                    seg_geom[upstream.segnum],
                     upstream.seg_ndist, 1.0, normalized=True)
             ]
-            geoms.extend(list(n.segments.geometry[segnums[1:-1]]))
+            geoms.extend(list(seg_geom[segnums[1:-1]]))
             geoms.append(
                 substring(
-                    n.segments.geometry[downstream.segnum],
+                    seg_geom[downstream.segnum],
                     0.0, downstream.seg_ndist, normalized=True)
             )
-            geoms_d[pair] = linemerge(unary_union(geoms))
+            geom = unary_union(geoms)
+            if geom.geom_type != "LineString":
+                geom = linemerge(geom)
+            geoms_d[pair] = geom
     return geoms_d
```

### Comparing `surface-water-network-0.5/swn/util.py` & `surface-water-network-0.6/swn/util.py`

 * *Files identical despite different names*

