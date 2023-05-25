# Comparing `tmp/spatialpandas-0.4.8.tar.gz` & `tmp/spatialpandas-0.4.8a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spatialpandas-0.4.8.tar", last modified: Thu May 25 14:48:50 2023, max compression
+gzip compressed data, was "spatialpandas-0.4.8a1.tar", last modified: Tue May 16 13:26:08 2023, max compression
```

## Comparing `spatialpandas-0.4.8.tar` & `spatialpandas-0.4.8a1.tar`

### file list

```diff
@@ -1,106 +1,106 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:48:50.948542 spatialpandas-0.4.8/
--rw-r--r--   0 runner    (1001) docker     (123)     7382 2023-05-25 14:41:22.000000 spatialpandas-0.4.8/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-05-25 14:41:22.000000 spatialpandas-0.4.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-25 14:41:22.000000 spatialpandas-0.4.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-05-25 14:41:22.000000 spatialpandas-0.4.8/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-05-25 14:48:50.948542 spatialpandas-0.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-05-25 14:41:22.000000 spatialpandas-0.4.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-25 14:41:22.000000 spatialpandas-0.4.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-25 14:48:50.948542 spatialpandas-0.4.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-05-25 14:41:22.000000 spatialpandas-0.4.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:48:50.936541 spatialpandas-0.4.8/spatialpandas/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-25 14:48:50.000000 spatialpandas-0.4.8/spatialpandas/.version
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-25 14:41:22.000000 spatialpandas-0.4.8/spatialpandas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-25 14:41:22.000000 spatialpandas-0.4.8/spatialpandas/_optional_imports.py
--rw-r--r--   0 runner    (1001) docker     (123)    24478 2023-05-25 14:41:22.000000 spatialpandas-0.4.8/spatialpandas/dask.py
--rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-05-25 14:41:22.000000 spatialpandas-0.4.8/spatialpandas/geodataframe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:48:50.936541 spatialpandas-0.4.8/spatialpandas/geometry/
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-25 14:41:22.000000 spatialpandas-0.4.8/spatialpandas/geometry/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:48:50.936541 spatialpandas-0.4.8/spatialpandas/geometry/_algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:41:22.000000 spatialpandas-0.4.8/spatialpandas/geometry/_algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-05-25 14:41:22.000000 spatialpandas-0.4.8/spatialpandas/geometry/_algorithms/bounds.py
--rw-r--r--   0 runner    (1001) docker     (123)    17743 2023-05-25 14:41:22.000000 spatialpandas-0.4.8/spatialpandas/geometry/_algorithms/intersection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-05-25 14:41:22.000000 spatialpandas-0.4.8/spatialpandas/geometry/_algorithms/measures.py
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-05-25 14:41:22.000000 spatialpandas-0.4.8/spatialpandas/geometry/_algorithms/orientation.py
--rw-r--r--   0 runner    (1001) docker     (123)    28546 2023-05-25 14:41:22.000000 spatialpandas-0.4.8/spatialpandas/geometry/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7847 2023-05-25 14:41:22.000000 spatialpandas-0.4.8/spatialpandas/geometry/basefixed.py
--rw-r--r--   0 runner    (1001) docker     (123)    10828 2023-05-25 14:41:22.000000 spatialpandas-0.4.8/spatialpandas/geometry/baselist.py
--rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-05-25 14:41:22.000000 spatialpandas-0.4.8/spatialpandas/geometry/line.py
--rw-r--r--   0 runner    (1001) docker     (123)     5206 2023-05-25 14:41:22.000000 spatialpandas-0.4.8/spatialpandas/geometry/multiline.py
--rw-r--r--   0 runner    (1001) docker     (123)     4076 2023-05-25 14:41:22.000000 spatialpandas-0.4.8/spatialpandas/geometry/multipoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     8624 2023-05-25 14:41:22.000000 spatialpandas-0.4.8/spatialpandas/geometry/multipolygon.py
--rw-r--r--   0 runner    (1001) docker     (123)    10271 2023-05-25 14:41:22.000000 spatialpandas-0.4.8/spatialpandas/geometry/point.py
--rw-r--r--   0 runner    (1001) docker     (123)     7717 2023-05-25 14:41:22.000000 spatialpandas-0.4.8/spatialpandas/geometry/polygon.py
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-05-25 14:41:22.000000 spatialpandas-0.4.8/spatialpandas/geometry/ring.py
--rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-05-25 14:41:22.000000 spatialpandas-0.4.8/spatialpandas/geoseries.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:48:50.940542 spatialpandas-0.4.8/spatialpandas/io/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-25 14:41:22.000000 spatialpandas-0.4.8/spatialpandas/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19063 2023-05-25 14:41:22.000000 spatialpandas-0.4.8/spatialpandas/io/parquet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-05-25 14:41:22.000000 spatialpandas-0.4.8/spatialpandas/io/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:48:50.940542 spatialpandas-0.4.8/spatialpandas/spatialindex/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-25 14:41:22.000000 spatialpandas-0.4.8/spatialpandas/spatialindex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-05-25 14:41:22.000000 spatialpandas-0.4.8/spatialpandas/spatialindex/hilbert_curve.py
--rw-r--r--   0 runner    (1001) docker     (123)    17228 2023-05-25 14:41:22.000000 spatialpandas-0.4.8/spatialpandas/spatialindex/rtree.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:48:50.940542 spatialpandas-0.4.8/spatialpandas/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:41:22.000000 spatialpandas-0.4.8/spatialpandas/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-05-25 14:41:22.000000 spatialpandas-0.4.8/spatialpandas/tests/_create_testdata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:48:50.940542 spatialpandas-0.4.8/spatialpandas/tests/geometry/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:41:22.000000 spatialpandas-0.4.8/spatialpandas/tests/geometry/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:48:50.940542 spatialpandas-0.4.8/spatialpandas/tests/geometry/algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:41:22.000000 spatialpandas-0.4.8/spatialpandas/tests/geometry/algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7545 2023-05-25 14:41:22.000000 spatialpandas-0.4.8/spatialpandas/tests/geometry/algorithms/test_intersection.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-25 14:41:22.000000 spatialpandas-0.4.8/spatialpandas/tests/geometry/algorithms/test_measures.py
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-25 14:41:22.000000 spatialpandas-0.4.8/spatialpandas/tests/geometry/algorithms/test_orientation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:48:50.940542 spatialpandas-0.4.8/spatialpandas/tests/geometry/intersection/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:41:22.000000 spatialpandas-0.4.8/spatialpandas/tests/geometry/intersection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9338 2023-05-25 14:41:22.000000 spatialpandas-0.4.8/spatialpandas/tests/geometry/intersection/test_point_intersection.py
--rw-r--r--   0 runner    (1001) docker     (123)     7966 2023-05-25 14:41:22.000000 spatialpandas-0.4.8/spatialpandas/tests/geometry/strategies.py
--rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-05-25 14:41:22.000000 spatialpandas-0.4.8/spatialpandas/tests/geometry/test_construction.py
--rw-r--r--   0 runner    (1001) docker     (123)     5554 2023-05-25 14:41:22.000000 spatialpandas-0.4.8/spatialpandas/tests/geometry/test_cx.py
--rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-05-25 14:41:22.000000 spatialpandas-0.4.8/spatialpandas/tests/geometry/test_geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-05-25 14:41:22.000000 spatialpandas-0.4.8/spatialpandas/tests/geometry/test_to_geopandas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:48:50.940542 spatialpandas-0.4.8/spatialpandas/tests/spatialindex/
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-05-25 14:41:22.000000 spatialpandas-0.4.8/spatialpandas/tests/spatialindex/test_hilbert_curve.py
--rw-r--r--   0 runner    (1001) docker     (123)     7000 2023-05-25 14:41:22.000000 spatialpandas-0.4.8/spatialpandas/tests/spatialindex/test_rtree.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-25 14:41:22.000000 spatialpandas-0.4.8/spatialpandas/tests/test_dask_autoimport.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:48:50.940542 spatialpandas-0.4.8/spatialpandas/tests/test_data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:48:50.944542 spatialpandas-0.4.8/spatialpandas/tests/test_data/dask_5.0.0.parq/
--rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-05-25 14:41:22.000000 spatialpandas-0.4.8/spatialpandas/tests/test_data/dask_5.0.0.parq/_common_metadata
--rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-05-25 14:41:22.000000 spatialpandas-0.4.8/spatialpandas/tests/test_data/dask_5.0.0.parq/_metadata
--rw-r--r--   0 runner    (1001) docker     (123)     4222 2023-05-25 14:41:22.000000 spatialpandas-0.4.8/spatialpandas/tests/test_data/dask_5.0.0.parq/part.0.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-05-25 14:41:22.000000 spatialpandas-0.4.8/spatialpandas/tests/test_data/dask_5.0.0.parq/part.1.parquet
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:48:50.944542 spatialpandas-0.4.8/spatialpandas/tests/test_data/dask_8.0.0.parq/
--rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-05-25 14:41:22.000000 spatialpandas-0.4.8/spatialpandas/tests/test_data/dask_8.0.0.parq/_common_metadata
--rw-r--r--   0 runner    (1001) docker     (123)     3746 2023-05-25 14:41:22.000000 spatialpandas-0.4.8/spatialpandas/tests/test_data/dask_8.0.0.parq/_metadata
--rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-05-25 14:41:22.000000 spatialpandas-0.4.8/spatialpandas/tests/test_data/dask_8.0.0.parq/part.0.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-05-25 14:41:22.000000 spatialpandas-0.4.8/spatialpandas/tests/test_data/dask_8.0.0.parq/part.1.parquet
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:48:50.944542 spatialpandas-0.4.8/spatialpandas/tests/test_data/dask_repart_5.0.0.parq/
--rw-r--r--   0 runner    (1001) docker     (123)     6283 2023-05-25 14:41:22.000000 spatialpandas-0.4.8/spatialpandas/tests/test_data/dask_repart_5.0.0.parq/_common_metadata
--rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-05-25 14:41:22.000000 spatialpandas-0.4.8/spatialpandas/tests/test_data/dask_repart_5.0.0.parq/_metadata
--rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-05-25 14:41:22.000000 spatialpandas-0.4.8/spatialpandas/tests/test_data/dask_repart_5.0.0.parq/part.0.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-05-25 14:41:22.000000 spatialpandas-0.4.8/spatialpandas/tests/test_data/dask_repart_5.0.0.parq/part.1.parquet
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:48:50.948542 spatialpandas-0.4.8/spatialpandas/tests/test_data/dask_repart_8.0.0.parq/
--rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-05-25 14:41:22.000000 spatialpandas-0.4.8/spatialpandas/tests/test_data/dask_repart_8.0.0.parq/_common_metadata
--rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-05-25 14:41:22.000000 spatialpandas-0.4.8/spatialpandas/tests/test_data/dask_repart_8.0.0.parq/_metadata
--rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-05-25 14:41:22.000000 spatialpandas-0.4.8/spatialpandas/tests/test_data/dask_repart_8.0.0.parq/part.0.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-05-25 14:41:22.000000 spatialpandas-0.4.8/spatialpandas/tests/test_data/dask_repart_8.0.0.parq/part.1.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-05-25 14:41:22.000000 spatialpandas-0.4.8/spatialpandas/tests/test_data/serial_5.0.0.parq
--rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-05-25 14:41:22.000000 spatialpandas-0.4.8/spatialpandas/tests/test_data/serial_8.0.0.parq
--rw-r--r--   0 runner    (1001) docker     (123)     6910 2023-05-25 14:41:22.000000 spatialpandas-0.4.8/spatialpandas/tests/test_fixedextensionarray.py
--rw-r--r--   0 runner    (1001) docker     (123)     5773 2023-05-25 14:41:22.000000 spatialpandas-0.4.8/spatialpandas/tests/test_geodataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     6905 2023-05-25 14:41:22.000000 spatialpandas-0.4.8/spatialpandas/tests/test_listextensionarray.py
--rw-r--r--   0 runner    (1001) docker     (123)    15338 2023-05-25 14:41:22.000000 spatialpandas-0.4.8/spatialpandas/tests/test_parquet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-05-25 14:41:22.000000 spatialpandas-0.4.8/spatialpandas/tests/test_parquet_s3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:48:50.948542 spatialpandas-0.4.8/spatialpandas/tests/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:41:22.000000 spatialpandas-0.4.8/spatialpandas/tests/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-05-25 14:41:22.000000 spatialpandas-0.4.8/spatialpandas/tests/tools/test_sjoin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:48:50.948542 spatialpandas-0.4.8/spatialpandas/tools/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-25 14:41:22.000000 spatialpandas-0.4.8/spatialpandas/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9237 2023-05-25 14:41:22.000000 spatialpandas-0.4.8/spatialpandas/tools/sjoin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-05-25 14:41:22.000000 spatialpandas-0.4.8/spatialpandas/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:48:50.936541 spatialpandas-0.4.8/spatialpandas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-05-25 14:48:50.000000 spatialpandas-0.4.8/spatialpandas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-05-25 14:48:50.000000 spatialpandas-0.4.8/spatialpandas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 14:48:50.000000 spatialpandas-0.4.8/spatialpandas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-25 14:48:50.000000 spatialpandas-0.4.8/spatialpandas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-25 14:48:50.000000 spatialpandas-0.4.8/spatialpandas.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:08.558910 spatialpandas-0.4.8a1/
+-rw-r--r--   0 runner    (1001) docker     (123)     7382 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-05-16 13:26:08.558910 spatialpandas-0.4.8a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-16 13:26:08.558910 spatialpandas-0.4.8a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:08.542909 spatialpandas-0.4.8a1/spatialpandas/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-16 13:26:08.000000 spatialpandas-0.4.8a1/spatialpandas/.version
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/_optional_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24478 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/dask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/geodataframe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:08.546910 spatialpandas-0.4.8a1/spatialpandas/geometry/
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/geometry/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:08.546910 spatialpandas-0.4.8a1/spatialpandas/geometry/_algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/geometry/_algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/geometry/_algorithms/bounds.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17743 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/geometry/_algorithms/intersection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/geometry/_algorithms/measures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/geometry/_algorithms/orientation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28546 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/geometry/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7847 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/geometry/basefixed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10828 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/geometry/baselist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/geometry/line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5206 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/geometry/multiline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4076 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/geometry/multipoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8624 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/geometry/multipolygon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10271 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/geometry/point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7717 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/geometry/polygon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/geometry/ring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/geoseries.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:08.546910 spatialpandas-0.4.8a1/spatialpandas/io/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19063 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/io/parquet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/io/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:08.550910 spatialpandas-0.4.8a1/spatialpandas/spatialindex/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/spatialindex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/spatialindex/hilbert_curve.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17228 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/spatialindex/rtree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:08.550910 spatialpandas-0.4.8a1/spatialpandas/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/tests/_create_testdata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:08.550910 spatialpandas-0.4.8a1/spatialpandas/tests/geometry/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/tests/geometry/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:08.554910 spatialpandas-0.4.8a1/spatialpandas/tests/geometry/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/tests/geometry/algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7545 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/tests/geometry/algorithms/test_intersection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/tests/geometry/algorithms/test_measures.py
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/tests/geometry/algorithms/test_orientation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:08.554910 spatialpandas-0.4.8a1/spatialpandas/tests/geometry/intersection/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/tests/geometry/intersection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9338 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/tests/geometry/intersection/test_point_intersection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7966 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/tests/geometry/strategies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/tests/geometry/test_construction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5554 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/tests/geometry/test_cx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/tests/geometry/test_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/tests/geometry/test_to_geopandas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:08.554910 spatialpandas-0.4.8a1/spatialpandas/tests/spatialindex/
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/tests/spatialindex/test_hilbert_curve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7000 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/tests/spatialindex/test_rtree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/tests/test_dask_autoimport.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:08.554910 spatialpandas-0.4.8a1/spatialpandas/tests/test_data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:08.554910 spatialpandas-0.4.8a1/spatialpandas/tests/test_data/dask_5.0.0.parq/
+-rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/tests/test_data/dask_5.0.0.parq/_common_metadata
+-rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/tests/test_data/dask_5.0.0.parq/_metadata
+-rw-r--r--   0 runner    (1001) docker     (123)     4222 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/tests/test_data/dask_5.0.0.parq/part.0.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/tests/test_data/dask_5.0.0.parq/part.1.parquet
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:08.554910 spatialpandas-0.4.8a1/spatialpandas/tests/test_data/dask_8.0.0.parq/
+-rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/tests/test_data/dask_8.0.0.parq/_common_metadata
+-rw-r--r--   0 runner    (1001) docker     (123)     3746 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/tests/test_data/dask_8.0.0.parq/_metadata
+-rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/tests/test_data/dask_8.0.0.parq/part.0.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/tests/test_data/dask_8.0.0.parq/part.1.parquet
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:08.554910 spatialpandas-0.4.8a1/spatialpandas/tests/test_data/dask_repart_5.0.0.parq/
+-rw-r--r--   0 runner    (1001) docker     (123)     6283 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/tests/test_data/dask_repart_5.0.0.parq/_common_metadata
+-rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/tests/test_data/dask_repart_5.0.0.parq/_metadata
+-rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/tests/test_data/dask_repart_5.0.0.parq/part.0.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/tests/test_data/dask_repart_5.0.0.parq/part.1.parquet
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:08.558910 spatialpandas-0.4.8a1/spatialpandas/tests/test_data/dask_repart_8.0.0.parq/
+-rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/tests/test_data/dask_repart_8.0.0.parq/_common_metadata
+-rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/tests/test_data/dask_repart_8.0.0.parq/_metadata
+-rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/tests/test_data/dask_repart_8.0.0.parq/part.0.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/tests/test_data/dask_repart_8.0.0.parq/part.1.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/tests/test_data/serial_5.0.0.parq
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/tests/test_data/serial_8.0.0.parq
+-rw-r--r--   0 runner    (1001) docker     (123)     6910 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/tests/test_fixedextensionarray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5773 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/tests/test_geodataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6905 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/tests/test_listextensionarray.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16268 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/tests/test_parquet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/tests/test_parquet_s3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:08.558910 spatialpandas-0.4.8a1/spatialpandas/tests/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/tests/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/tests/tools/test_sjoin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:08.558910 spatialpandas-0.4.8a1/spatialpandas/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9237 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/tools/sjoin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:08.546910 spatialpandas-0.4.8a1/spatialpandas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-05-16 13:26:08.000000 spatialpandas-0.4.8a1/spatialpandas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-05-16 13:26:08.000000 spatialpandas-0.4.8a1/spatialpandas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 13:26:08.000000 spatialpandas-0.4.8a1/spatialpandas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-16 13:26:08.000000 spatialpandas-0.4.8a1/spatialpandas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-16 13:26:08.000000 spatialpandas-0.4.8a1/spatialpandas.egg-info/top_level.txt
```

### Comparing `spatialpandas-0.4.8/CHANGELOG.md` & `spatialpandas-0.4.8a1/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.8/LICENSE` & `spatialpandas-0.4.8a1/LICENSE`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.8/NOTICE` & `spatialpandas-0.4.8a1/NOTICE`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.8/PKG-INFO` & `spatialpandas-0.4.8a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spatialpandas
-Version: 0.4.8
+Version: 0.4.8a1
 Summary: Pandas extension arrays for spatial/geometric operations
 Home-page: https://github.com/holoviz/spatialpandas
 Maintainer: HoloViz developers
 Maintainer-email: developers@holoviz.org
 License: BSD-2-Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `spatialpandas-0.4.8/README.md` & `spatialpandas-0.4.8a1/README.md`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.8/setup.py` & `spatialpandas-0.4.8a1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,38 +9,37 @@
         'hilbertcurve',
         'geopandas',
         'hypothesis',
         'keyring',
         'moto[s3,server]',
         'pytest-cov',
         'pytest',
-        'python-snappy',
         'rfc3986',
         's3fs',
         'scipy',
         'shapely',
         'twine',
     ],
     'examples': [
         'datashader',
-        'distributed',
         'descartes',
         'geopandas',
         'holoviews',
         'matplotlib',
     ]
 }
 
 install_requires = [
     'dask',
     'fsspec',
     'numba',
     'pandas',
     'param',
     'pyarrow >=1.0',
+    'python-snappy',
     'retrying',
 ]
 
 setup_args = dict(
     name='spatialpandas',
     version=param.version.get_setup_version(
         __file__,
```

### Comparing `spatialpandas-0.4.8/spatialpandas/__init__.py` & `spatialpandas-0.4.8a1/spatialpandas/__init__.py`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.8/spatialpandas/dask.py` & `spatialpandas-0.4.8a1/spatialpandas/dask.py`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.8/spatialpandas/geodataframe.py` & `spatialpandas-0.4.8a1/spatialpandas/geodataframe.py`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.8/spatialpandas/geometry/__init__.py` & `spatialpandas-0.4.8a1/spatialpandas/geometry/__init__.py`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.8/spatialpandas/geometry/_algorithms/bounds.py` & `spatialpandas-0.4.8a1/spatialpandas/geometry/_algorithms/bounds.py`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.8/spatialpandas/geometry/_algorithms/intersection.py` & `spatialpandas-0.4.8a1/spatialpandas/geometry/_algorithms/intersection.py`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.8/spatialpandas/geometry/_algorithms/measures.py` & `spatialpandas-0.4.8a1/spatialpandas/geometry/_algorithms/measures.py`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.8/spatialpandas/geometry/_algorithms/orientation.py` & `spatialpandas-0.4.8a1/spatialpandas/geometry/_algorithms/orientation.py`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.8/spatialpandas/geometry/base.py` & `spatialpandas-0.4.8a1/spatialpandas/geometry/base.py`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.8/spatialpandas/geometry/basefixed.py` & `spatialpandas-0.4.8a1/spatialpandas/geometry/basefixed.py`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.8/spatialpandas/geometry/baselist.py` & `spatialpandas-0.4.8a1/spatialpandas/geometry/baselist.py`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.8/spatialpandas/geometry/line.py` & `spatialpandas-0.4.8a1/spatialpandas/geometry/line.py`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.8/spatialpandas/geometry/multiline.py` & `spatialpandas-0.4.8a1/spatialpandas/geometry/multiline.py`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.8/spatialpandas/geometry/multipoint.py` & `spatialpandas-0.4.8a1/spatialpandas/geometry/multipoint.py`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.8/spatialpandas/geometry/multipolygon.py` & `spatialpandas-0.4.8a1/spatialpandas/geometry/multipolygon.py`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.8/spatialpandas/geometry/point.py` & `spatialpandas-0.4.8a1/spatialpandas/geometry/point.py`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.8/spatialpandas/geometry/polygon.py` & `spatialpandas-0.4.8a1/spatialpandas/geometry/polygon.py`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.8/spatialpandas/geometry/ring.py` & `spatialpandas-0.4.8a1/spatialpandas/geometry/ring.py`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.8/spatialpandas/geoseries.py` & `spatialpandas-0.4.8a1/spatialpandas/geoseries.py`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.8/spatialpandas/io/parquet.py` & `spatialpandas-0.4.8a1/spatialpandas/io/parquet.py`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.8/spatialpandas/io/utils.py` & `spatialpandas-0.4.8a1/spatialpandas/io/utils.py`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.8/spatialpandas/spatialindex/hilbert_curve.py` & `spatialpandas-0.4.8a1/spatialpandas/spatialindex/hilbert_curve.py`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.8/spatialpandas/spatialindex/rtree.py` & `spatialpandas-0.4.8a1/spatialpandas/spatialindex/rtree.py`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.8/spatialpandas/tests/_create_testdata.py` & `spatialpandas-0.4.8a1/spatialpandas/tests/_create_testdata.py`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.8/spatialpandas/tests/geometry/algorithms/test_intersection.py` & `spatialpandas-0.4.8a1/spatialpandas/tests/geometry/algorithms/test_intersection.py`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.8/spatialpandas/tests/geometry/algorithms/test_measures.py` & `spatialpandas-0.4.8a1/spatialpandas/tests/geometry/algorithms/test_measures.py`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.8/spatialpandas/tests/geometry/algorithms/test_orientation.py` & `spatialpandas-0.4.8a1/spatialpandas/tests/geometry/algorithms/test_orientation.py`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.8/spatialpandas/tests/geometry/intersection/test_point_intersection.py` & `spatialpandas-0.4.8a1/spatialpandas/tests/geometry/intersection/test_point_intersection.py`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.8/spatialpandas/tests/geometry/strategies.py` & `spatialpandas-0.4.8a1/spatialpandas/tests/geometry/strategies.py`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.8/spatialpandas/tests/geometry/test_construction.py` & `spatialpandas-0.4.8a1/spatialpandas/tests/geometry/test_construction.py`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.8/spatialpandas/tests/geometry/test_cx.py` & `spatialpandas-0.4.8a1/spatialpandas/tests/geometry/test_cx.py`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.8/spatialpandas/tests/geometry/test_geometry.py` & `spatialpandas-0.4.8a1/spatialpandas/tests/geometry/test_geometry.py`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.8/spatialpandas/tests/geometry/test_to_geopandas.py` & `spatialpandas-0.4.8a1/spatialpandas/tests/geometry/test_to_geopandas.py`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.8/spatialpandas/tests/spatialindex/test_hilbert_curve.py` & `spatialpandas-0.4.8a1/spatialpandas/tests/spatialindex/test_hilbert_curve.py`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.8/spatialpandas/tests/spatialindex/test_rtree.py` & `spatialpandas-0.4.8a1/spatialpandas/tests/spatialindex/test_rtree.py`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.8/spatialpandas/tests/test_data/dask_5.0.0.parq/_common_metadata` & `spatialpandas-0.4.8a1/spatialpandas/tests/test_data/dask_5.0.0.parq/_common_metadata`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.8/spatialpandas/tests/test_data/dask_5.0.0.parq/_metadata` & `spatialpandas-0.4.8a1/spatialpandas/tests/test_data/dask_5.0.0.parq/_metadata`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.8/spatialpandas/tests/test_data/dask_5.0.0.parq/part.0.parquet` & `spatialpandas-0.4.8a1/spatialpandas/tests/test_data/dask_5.0.0.parq/part.0.parquet`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.8/spatialpandas/tests/test_data/dask_5.0.0.parq/part.1.parquet` & `spatialpandas-0.4.8a1/spatialpandas/tests/test_data/dask_5.0.0.parq/part.1.parquet`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.8/spatialpandas/tests/test_data/dask_8.0.0.parq/_common_metadata` & `spatialpandas-0.4.8a1/spatialpandas/tests/test_data/dask_8.0.0.parq/_common_metadata`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.8/spatialpandas/tests/test_data/dask_8.0.0.parq/_metadata` & `spatialpandas-0.4.8a1/spatialpandas/tests/test_data/dask_8.0.0.parq/_metadata`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.8/spatialpandas/tests/test_data/dask_8.0.0.parq/part.0.parquet` & `spatialpandas-0.4.8a1/spatialpandas/tests/test_data/dask_8.0.0.parq/part.0.parquet`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.8/spatialpandas/tests/test_data/dask_8.0.0.parq/part.1.parquet` & `spatialpandas-0.4.8a1/spatialpandas/tests/test_data/dask_8.0.0.parq/part.1.parquet`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.8/spatialpandas/tests/test_data/dask_repart_5.0.0.parq/_common_metadata` & `spatialpandas-0.4.8a1/spatialpandas/tests/test_data/dask_repart_5.0.0.parq/_common_metadata`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.8/spatialpandas/tests/test_data/dask_repart_5.0.0.parq/_metadata` & `spatialpandas-0.4.8a1/spatialpandas/tests/test_data/dask_repart_5.0.0.parq/_metadata`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.8/spatialpandas/tests/test_data/dask_repart_5.0.0.parq/part.0.parquet` & `spatialpandas-0.4.8a1/spatialpandas/tests/test_data/dask_repart_5.0.0.parq/part.0.parquet`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.8/spatialpandas/tests/test_data/dask_repart_5.0.0.parq/part.1.parquet` & `spatialpandas-0.4.8a1/spatialpandas/tests/test_data/dask_repart_5.0.0.parq/part.1.parquet`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.8/spatialpandas/tests/test_data/dask_repart_8.0.0.parq/_common_metadata` & `spatialpandas-0.4.8a1/spatialpandas/tests/test_data/dask_repart_8.0.0.parq/_common_metadata`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.8/spatialpandas/tests/test_data/dask_repart_8.0.0.parq/_metadata` & `spatialpandas-0.4.8a1/spatialpandas/tests/test_data/dask_repart_8.0.0.parq/_metadata`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.8/spatialpandas/tests/test_data/dask_repart_8.0.0.parq/part.0.parquet` & `spatialpandas-0.4.8a1/spatialpandas/tests/test_data/dask_repart_8.0.0.parq/part.0.parquet`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.8/spatialpandas/tests/test_data/dask_repart_8.0.0.parq/part.1.parquet` & `spatialpandas-0.4.8a1/spatialpandas/tests/test_data/dask_repart_8.0.0.parq/part.1.parquet`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.8/spatialpandas/tests/test_data/serial_5.0.0.parq` & `spatialpandas-0.4.8a1/spatialpandas/tests/test_data/serial_5.0.0.parq`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.8/spatialpandas/tests/test_data/serial_8.0.0.parq` & `spatialpandas-0.4.8a1/spatialpandas/tests/test_data/serial_8.0.0.parq`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.8/spatialpandas/tests/test_fixedextensionarray.py` & `spatialpandas-0.4.8a1/spatialpandas/tests/test_fixedextensionarray.py`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.8/spatialpandas/tests/test_geodataframe.py` & `spatialpandas-0.4.8a1/spatialpandas/tests/test_geodataframe.py`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.8/spatialpandas/tests/test_listextensionarray.py` & `spatialpandas-0.4.8a1/spatialpandas/tests/test_listextensionarray.py`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.8/spatialpandas/tests/test_parquet.py` & `spatialpandas-0.4.8a1/spatialpandas/tests/test_parquet.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,108 +29,108 @@
 @given(
     gp_point=st_point_array(min_size=1, geoseries=True),
     gp_multipoint=st_multipoint_array(min_size=1, geoseries=True),
     gp_multiline=st_multiline_array(min_size=1, geoseries=True),
 )
 @hyp_settings
 def test_parquet(gp_point, gp_multipoint, gp_multiline, tmp_path_factory):
-    tmp_path = tmp_path_factory.mktemp("spatialpandas", numbered=True)
-    # Build dataframe
-    n = min(len(gp_multipoint), len(gp_multiline))
-    df = GeoDataFrame({
-        'point': GeoSeries(gp_point[:n]),
-        'multipoint': GeoSeries(gp_multipoint[:n]),
-        'multiline': GeoSeries(gp_multiline[:n]),
-        'a': list(range(n))
-    })
-
-    df.index.name = 'range_idx'
-
-    path = tmp_path / 'df.parq'
-    to_parquet(df, path)
-    df_read = read_parquet(str(path), columns=['point', 'multipoint', 'multiline', 'a'])
-    assert isinstance(df_read, GeoDataFrame)
-    pd.testing.assert_frame_equal(df, df_read)
-    assert df_read.index.name == df.index.name
+    with tmp_path_factory.mktemp("spatialpandas", numbered=True) as tmp_path:
+        # Build dataframe
+        n = min(len(gp_multipoint), len(gp_multiline))
+        df = GeoDataFrame({
+            'point': GeoSeries(gp_point[:n]),
+            'multipoint': GeoSeries(gp_multipoint[:n]),
+            'multiline': GeoSeries(gp_multiline[:n]),
+            'a': list(range(n))
+        })
+
+        df.index.name = 'range_idx'
+
+        path = tmp_path / 'df.parq'
+        to_parquet(df, path)
+        df_read = read_parquet(str(path), columns=['point', 'multipoint', 'multiline', 'a'])
+        assert isinstance(df_read, GeoDataFrame)
+        pd.testing.assert_frame_equal(df, df_read)
+        assert df_read.index.name == df.index.name
 
 
 @given(
     gp_point=st_point_array(min_size=1, geoseries=True),
     gp_multipoint=st_multipoint_array(min_size=1, geoseries=True),
     gp_multiline=st_multiline_array(min_size=1, geoseries=True),
 )
 @hyp_settings
 def test_parquet_columns(gp_point, gp_multipoint, gp_multiline,
                          tmp_path_factory):
-    tmp_path = tmp_path_factory.mktemp("spatialpandas", numbered=True)
-    # Build dataframe
-    n = min(len(gp_multipoint), len(gp_multiline))
-    df = GeoDataFrame({
-        'point': GeoSeries(gp_point[:n]),
-        'multipoint': GeoSeries(gp_multipoint[:n]),
-        'multiline': GeoSeries(gp_multiline[:n]),
-        'a': list(range(n))
-    })
-
-    path = tmp_path / 'df.parq'
-    to_parquet(df, path)
-    columns = ['a', 'multiline']
-    df_read = read_parquet(str(path), columns=columns)
-    assert isinstance(df_read, GeoDataFrame)
-    pd.testing.assert_frame_equal(df[columns], df_read)
+    with tmp_path_factory.mktemp("spatialpandas", numbered=True) as tmp_path:
+        # Build dataframe
+        n = min(len(gp_multipoint), len(gp_multiline))
+        df = GeoDataFrame({
+            'point': GeoSeries(gp_point[:n]),
+            'multipoint': GeoSeries(gp_multipoint[:n]),
+            'multiline': GeoSeries(gp_multiline[:n]),
+            'a': list(range(n))
+        })
+
+        path = tmp_path / 'df.parq'
+        to_parquet(df, path)
+        columns = ['a', 'multiline']
+        df_read = read_parquet(str(path), columns=columns)
+        assert isinstance(df_read, GeoDataFrame)
+        pd.testing.assert_frame_equal(df[columns], df_read)
 
 
 @given(
     gp_multipoint=st_multipoint_array(min_size=1, geoseries=True),
     gp_multiline=st_multiline_array(min_size=1, geoseries=True),
 )
 @hyp_settings
 def test_parquet_dask(gp_multipoint, gp_multiline, tmp_path_factory):
-    tmp_path = tmp_path_factory.mktemp("spatialpandas", numbered=True)
-    # Build dataframe
-    n = min(len(gp_multipoint), len(gp_multiline))
-    df = GeoDataFrame({
-        'points': GeoSeries(gp_multipoint[:n]),
-        'lines': GeoSeries(gp_multiline[:n]),
-        'a': list(range(n))
-    })
-    ddf = dd.from_pandas(df, npartitions=3)
+    with tmp_path_factory.mktemp("spatialpandas", numbered=True) as tmp_path:
+        # Build dataframe
+        n = min(len(gp_multipoint), len(gp_multiline))
+        df = GeoDataFrame({
+            'points': GeoSeries(gp_multipoint[:n]),
+            'lines': GeoSeries(gp_multiline[:n]),
+            'a': list(range(n))
+        })
+        ddf = dd.from_pandas(df, npartitions=3)
+
+        path = tmp_path / 'ddf.parq'
+        ddf.to_parquet(str(path))
+        ddf_read = read_parquet_dask(str(path))
+
+        # Check type
+        assert isinstance(ddf_read, DaskGeoDataFrame)
+
+        # Check that partition bounds were loaded
+        nonempty = np.nonzero(
+            np.asarray(ddf.map_partitions(len).compute() > 0)
+        )[0]
+        assert set(ddf_read._partition_bounds) == {'points', 'lines'}
+        expected_partition_bounds = (
+            ddf['points'].partition_bounds.iloc[nonempty].reset_index(drop=True)
+        )
+        expected_partition_bounds.index.name = 'partition'
+
+        pd.testing.assert_frame_equal(
+            expected_partition_bounds,
+            ddf_read._partition_bounds['points'],
+        )
+
+        expected_partition_bounds = (
+            ddf['lines'].partition_bounds.iloc[nonempty].reset_index(drop=True)
+        )
+        expected_partition_bounds.index.name = 'partition'
+        pd.testing.assert_frame_equal(
+            expected_partition_bounds,
+            ddf_read._partition_bounds['lines'],
+        )
 
-    path = tmp_path / 'ddf.parq'
-    ddf.to_parquet(str(path))
-    ddf_read = read_parquet_dask(str(path))
-
-    # Check type
-    assert isinstance(ddf_read, DaskGeoDataFrame)
-
-    # Check that partition bounds were loaded
-    nonempty = np.nonzero(
-        np.asarray(ddf.map_partitions(len).compute() > 0)
-    )[0]
-    assert set(ddf_read._partition_bounds) == {'points', 'lines'}
-    expected_partition_bounds = (
-        ddf['points'].partition_bounds.iloc[nonempty].reset_index(drop=True)
-    )
-    expected_partition_bounds.index.name = 'partition'
-
-    pd.testing.assert_frame_equal(
-        expected_partition_bounds,
-        ddf_read._partition_bounds['points'],
-    )
-
-    expected_partition_bounds = (
-        ddf['lines'].partition_bounds.iloc[nonempty].reset_index(drop=True)
-    )
-    expected_partition_bounds.index.name = 'partition'
-    pd.testing.assert_frame_equal(
-        expected_partition_bounds,
-        ddf_read._partition_bounds['lines'],
-    )
-
-    assert ddf_read.geometry.name == 'points'
+        assert ddf_read.geometry.name == 'points'
 
 
 @given(
     gp_multipoint=st_multipoint_array(min_size=10, max_size=40, geoseries=True),
     gp_multiline=st_multiline_array(min_size=10, max_size=40, geoseries=True),
 )
 @settings(deadline=None, max_examples=30)
@@ -180,136 +180,136 @@
         Phase.generate,
         Phase.target
     ],
     verbosity=Verbosity.verbose,
 )
 def test_pack_partitions_to_parquet(gp_multipoint, gp_multiline,
                                     use_temp_format, tmp_path_factory):
-    tmp_path = tmp_path_factory.mktemp("spatialpandas", numbered=True)
-    # Build dataframe
-    n = min(len(gp_multipoint), len(gp_multiline))
-    df = GeoDataFrame({
-        'points': GeoSeries(gp_multipoint[:n]),
-        'lines': GeoSeries(gp_multiline[:n]),
-        'a': list(range(n))
-    }).set_geometry('lines')
-    ddf = dd.from_pandas(df, npartitions=3)
-
-    path = tmp_path / 'ddf.parq'
-    if use_temp_format:
-        (tmp_path / 'scratch').mkdir(parents=True, exist_ok=True)
-        tempdir_format = str(tmp_path / 'scratch' / 'part-{uuid}-{partition:03d}')
-    else:
-        tempdir_format = None
-
-    _retry_args = dict(
-        wait_exponential_multiplier=10,
-        wait_exponential_max=20000,
-        stop_max_attempt_number=4
-    )
-
-    ddf_packed = ddf.pack_partitions_to_parquet(
-        str(path),
-        npartitions=12,
-        tempdir_format=tempdir_format,
-        _retry_args=_retry_args,
-    )
-
-    # Check the number of partitions (< 4 can happen in the case of empty partitions)
-    assert ddf_packed.npartitions <= 12
-
-    # Check that rows are now sorted in order of hilbert distance
-    total_bounds = df.lines.total_bounds
-    hilbert_distances = ddf_packed.lines.map_partitions(
-        lambda s: s.hilbert_distance(total_bounds=total_bounds)
-    ).compute().values
-
-    # Compute expected total_bounds
-    expected_distances = np.sort(
-        df.lines.hilbert_distance(total_bounds=total_bounds).values
-    )
-
-    np.testing.assert_equal(expected_distances, hilbert_distances)
-    assert ddf_packed.geometry.name == 'points'
-
-    # Read columns
-    columns = ['a', 'lines']
-    ddf_read_cols = read_parquet_dask(path, columns=columns)
-    pd.testing.assert_frame_equal(
-        ddf_read_cols.compute(), ddf_packed[columns].compute()
-    )
+    with tmp_path_factory.mktemp("spatialpandas", numbered=True) as tmp_path:
+        # Build dataframe
+        n = min(len(gp_multipoint), len(gp_multiline))
+        df = GeoDataFrame({
+            'points': GeoSeries(gp_multipoint[:n]),
+            'lines': GeoSeries(gp_multiline[:n]),
+            'a': list(range(n))
+        }).set_geometry('lines')
+        ddf = dd.from_pandas(df, npartitions=3)
+
+        path = tmp_path / 'ddf.parq'
+        if use_temp_format:
+            (tmp_path / 'scratch').mkdir(parents=True, exist_ok=True)
+            tempdir_format = str(tmp_path / 'scratch' / 'part-{uuid}-{partition:03d}')
+        else:
+            tempdir_format = None
+
+        _retry_args = dict(
+            wait_exponential_multiplier=10,
+            wait_exponential_max=20000,
+            stop_max_attempt_number=4
+        )
+
+        ddf_packed = ddf.pack_partitions_to_parquet(
+            str(path),
+            npartitions=12,
+            tempdir_format=tempdir_format,
+            _retry_args=_retry_args,
+        )
+
+        # Check the number of partitions (< 4 can happen in the case of empty partitions)
+        assert ddf_packed.npartitions <= 12
+
+        # Check that rows are now sorted in order of hilbert distance
+        total_bounds = df.lines.total_bounds
+        hilbert_distances = ddf_packed.lines.map_partitions(
+            lambda s: s.hilbert_distance(total_bounds=total_bounds)
+        ).compute().values
+
+        # Compute expected total_bounds
+        expected_distances = np.sort(
+            df.lines.hilbert_distance(total_bounds=total_bounds).values
+        )
+
+        np.testing.assert_equal(expected_distances, hilbert_distances)
+        assert ddf_packed.geometry.name == 'points'
+
+        # Read columns
+        columns = ['a', 'lines']
+        ddf_read_cols = read_parquet_dask(path, columns=columns)
+        pd.testing.assert_frame_equal(
+            ddf_read_cols.compute(), ddf_packed[columns].compute()
+        )
 
 
 @pytest.mark.slow
 @given(
     gp_multipoint1=st_multipoint_array(min_size=10, max_size=40, geoseries=True),
     gp_multiline1=st_multiline_array(min_size=10, max_size=40, geoseries=True),
     gp_multipoint2=st_multipoint_array(min_size=10, max_size=40, geoseries=True),
     gp_multiline2=st_multiline_array(min_size=10, max_size=40, geoseries=True),
 )
 @settings(deadline=None, max_examples=30, suppress_health_check=[HealthCheck.too_slow])
 def test_pack_partitions_to_parquet_glob(gp_multipoint1, gp_multiline1,
                                          gp_multipoint2, gp_multiline2,
                                          tmp_path_factory):
-    tmp_path = tmp_path_factory.mktemp("spatialpandas", numbered=True)
-    # Build dataframe1
-    n = min(len(gp_multipoint1), len(gp_multiline1))
-    df1 = GeoDataFrame({
-        'points': GeoSeries(gp_multipoint1[:n]),
-        'lines': GeoSeries(gp_multiline1[:n]),
-        'a': list(range(n))
-    }).set_geometry('lines')
-    ddf1 = dd.from_pandas(df1, npartitions=3)
-    path1 = tmp_path / 'ddf1.parq'
-    ddf_packed1 = ddf1.pack_partitions_to_parquet(str(path1), npartitions=3)
-
-    # Build dataframe2
-    n = min(len(gp_multipoint2), len(gp_multiline2))
-    df2 = GeoDataFrame({
-        'points': GeoSeries(gp_multipoint2[:n]),
-        'lines': GeoSeries(gp_multiline2[:n]),
-        'a': list(range(n))
-    }).set_geometry('lines')
-    ddf2 = dd.from_pandas(df2, npartitions=3)
-    path2 = tmp_path / 'ddf2.parq'
-    ddf_packed2 = ddf2.pack_partitions_to_parquet(str(path2), npartitions=4)
-
-    # Load both packed datasets with glob
-    ddf_globbed = read_parquet_dask(tmp_path / "ddf*.parq", geometry="lines")
-
-    # Check the number of partitions (< 7 can happen in the case of empty partitions)
-    assert ddf_globbed.npartitions <= 7
-
-    # Check contents
-    expected_df = pd.concat([ddf_packed1.compute(), ddf_packed2.compute()])
-    df_globbed = ddf_globbed.compute()
-    pd.testing.assert_frame_equal(df_globbed, expected_df)
-
-    # Check partition bounds
-    expected_bounds = {
-        'points': pd.concat([
-            ddf_packed1._partition_bounds['points'],
-            ddf_packed2._partition_bounds['points'],
-        ]).reset_index(drop=True),
-        'lines': pd.concat([
-            ddf_packed1._partition_bounds['lines'],
-            ddf_packed2._partition_bounds['lines'],
-        ]).reset_index(drop=True),
-    }
-    expected_bounds['points'].index.name = 'partition'
-    expected_bounds['lines'].index.name = 'partition'
-    pd.testing.assert_frame_equal(
-        expected_bounds['points'], ddf_globbed._partition_bounds['points']
-    )
-
-    pd.testing.assert_frame_equal(
-        expected_bounds['lines'], ddf_globbed._partition_bounds['lines']
-    )
+    with tmp_path_factory.mktemp("spatialpandas", numbered=True) as tmp_path:
+        # Build dataframe1
+        n = min(len(gp_multipoint1), len(gp_multiline1))
+        df1 = GeoDataFrame({
+            'points': GeoSeries(gp_multipoint1[:n]),
+            'lines': GeoSeries(gp_multiline1[:n]),
+            'a': list(range(n))
+        }).set_geometry('lines')
+        ddf1 = dd.from_pandas(df1, npartitions=3)
+        path1 = tmp_path / 'ddf1.parq'
+        ddf_packed1 = ddf1.pack_partitions_to_parquet(str(path1), npartitions=3)
+
+        # Build dataframe2
+        n = min(len(gp_multipoint2), len(gp_multiline2))
+        df2 = GeoDataFrame({
+            'points': GeoSeries(gp_multipoint2[:n]),
+            'lines': GeoSeries(gp_multiline2[:n]),
+            'a': list(range(n))
+        }).set_geometry('lines')
+        ddf2 = dd.from_pandas(df2, npartitions=3)
+        path2 = tmp_path / 'ddf2.parq'
+        ddf_packed2 = ddf2.pack_partitions_to_parquet(str(path2), npartitions=4)
+
+        # Load both packed datasets with glob
+        ddf_globbed = read_parquet_dask(tmp_path / "ddf*.parq", geometry="lines")
+
+        # Check the number of partitions (< 7 can happen in the case of empty partitions)
+        assert ddf_globbed.npartitions <= 7
+
+        # Check contents
+        expected_df = pd.concat([ddf_packed1.compute(), ddf_packed2.compute()])
+        df_globbed = ddf_globbed.compute()
+        pd.testing.assert_frame_equal(df_globbed, expected_df)
+
+        # Check partition bounds
+        expected_bounds = {
+            'points': pd.concat([
+                ddf_packed1._partition_bounds['points'],
+                ddf_packed2._partition_bounds['points'],
+            ]).reset_index(drop=True),
+            'lines': pd.concat([
+                ddf_packed1._partition_bounds['lines'],
+                ddf_packed2._partition_bounds['lines'],
+            ]).reset_index(drop=True),
+        }
+        expected_bounds['points'].index.name = 'partition'
+        expected_bounds['lines'].index.name = 'partition'
+        pd.testing.assert_frame_equal(
+            expected_bounds['points'], ddf_globbed._partition_bounds['points']
+        )
+
+        pd.testing.assert_frame_equal(
+            expected_bounds['lines'], ddf_globbed._partition_bounds['lines']
+        )
 
-    assert ddf_globbed.geometry.name == 'lines'
+        assert ddf_globbed.geometry.name == 'lines'
 
 
 @pytest.mark.slow
 @given(
     gp_multipoint1=st_multipoint_array(min_size=10, max_size=40, geoseries=True),
     gp_multiline1=st_multiline_array(min_size=10, max_size=40, geoseries=True),
     gp_multipoint2=st_multipoint_array(min_size=10, max_size=40, geoseries=True),
@@ -318,91 +318,91 @@
 )
 @settings(deadline=None, max_examples=30, suppress_health_check=[HealthCheck.too_slow])
 def test_pack_partitions_to_parquet_list_bounds(
         gp_multipoint1, gp_multiline1,
         gp_multipoint2, gp_multiline2,
         bounds, tmp_path_factory,
 ):
-    tmp_path = tmp_path_factory.mktemp("spatialpandas", numbered=True)
-    # Build dataframe1
-    n = min(len(gp_multipoint1), len(gp_multiline1))
-    df1 = GeoDataFrame({
-        'points': GeoSeries(gp_multipoint1[:n]),
-        'lines': GeoSeries(gp_multiline1[:n]),
-        'a': list(range(n))
-    }).set_geometry('lines')
-    ddf1 = dd.from_pandas(df1, npartitions=3)
-    path1 = tmp_path / 'ddf1.parq'
-    ddf_packed1 = ddf1.pack_partitions_to_parquet(str(path1), npartitions=3)
-
-    # Build dataframe2
-    n = min(len(gp_multipoint2), len(gp_multiline2))
-    df2 = GeoDataFrame({
-        'points': GeoSeries(gp_multipoint2[:n]),
-        'lines': GeoSeries(gp_multiline2[:n]),
-        'a': list(range(n))
-    }).set_geometry('lines')
-    ddf2 = dd.from_pandas(df2, npartitions=3)
-    path2 = tmp_path / 'ddf2.parq'
-    ddf_packed2 = ddf2.pack_partitions_to_parquet(str(path2), npartitions=4)
-
-    # Load both packed datasets with glob
-    ddf_read = read_parquet_dask(
-        [str(tmp_path / "ddf1.parq"), str(tmp_path / "ddf2.parq")],
-        geometry="points", bounds=bounds
-    )
+    with tmp_path_factory.mktemp("spatialpandas", numbered=True) as tmp_path:
+        # Build dataframe1
+        n = min(len(gp_multipoint1), len(gp_multiline1))
+        df1 = GeoDataFrame({
+            'points': GeoSeries(gp_multipoint1[:n]),
+            'lines': GeoSeries(gp_multiline1[:n]),
+            'a': list(range(n))
+        }).set_geometry('lines')
+        ddf1 = dd.from_pandas(df1, npartitions=3)
+        path1 = tmp_path / 'ddf1.parq'
+        ddf_packed1 = ddf1.pack_partitions_to_parquet(str(path1), npartitions=3)
+
+        # Build dataframe2
+        n = min(len(gp_multipoint2), len(gp_multiline2))
+        df2 = GeoDataFrame({
+            'points': GeoSeries(gp_multipoint2[:n]),
+            'lines': GeoSeries(gp_multiline2[:n]),
+            'a': list(range(n))
+        }).set_geometry('lines')
+        ddf2 = dd.from_pandas(df2, npartitions=3)
+        path2 = tmp_path / 'ddf2.parq'
+        ddf_packed2 = ddf2.pack_partitions_to_parquet(str(path2), npartitions=4)
+
+        # Load both packed datasets with glob
+        ddf_read = read_parquet_dask(
+            [str(tmp_path / "ddf1.parq"), str(tmp_path / "ddf2.parq")],
+            geometry="points", bounds=bounds
+        )
+
+        # Check the number of partitions (< 7 can happen in the case of empty partitions)
+        assert ddf_read.npartitions <= 7
+
+        # Check contents
+        xslice = slice(bounds[0], bounds[2])
+        yslice = slice(bounds[1], bounds[3])
+        expected_df = pd.concat([
+            ddf_packed1.cx_partitions[xslice, yslice].compute(),
+            ddf_packed2.cx_partitions[xslice, yslice].compute()
+        ])
+        df_read = ddf_read.compute()
+        pd.testing.assert_frame_equal(df_read, expected_df)
 
-    # Check the number of partitions (< 7 can happen in the case of empty partitions)
-    assert ddf_read.npartitions <= 7
+        # Compute expected partition bounds
+        points_bounds = pd.concat([
+            ddf_packed1._partition_bounds['points'],
+            ddf_packed2._partition_bounds['points'],
+        ]).reset_index(drop=True)
 
-    # Check contents
-    xslice = slice(bounds[0], bounds[2])
-    yslice = slice(bounds[1], bounds[3])
-    expected_df = pd.concat([
-        ddf_packed1.cx_partitions[xslice, yslice].compute(),
-        ddf_packed2.cx_partitions[xslice, yslice].compute()
-    ])
-    df_read = ddf_read.compute()
-    pd.testing.assert_frame_equal(df_read, expected_df)
-
-    # Compute expected partition bounds
-    points_bounds = pd.concat([
-        ddf_packed1._partition_bounds['points'],
-        ddf_packed2._partition_bounds['points'],
-    ]).reset_index(drop=True)
-
-    x0, y0, x1, y1 = bounds
-    x0, x1 = (x0, x1) if x0 <= x1 else (x1, x0)
-    y0, y1 = (y0, y1) if y0 <= y1 else (y1, y0)
-    partition_inds = ~(
-        (points_bounds.x1 < x0) |
-        (points_bounds.y1 < y0) |
-        (points_bounds.x0 > x1) |
-        (points_bounds.y0 > y1)
-    )
-    points_bounds = points_bounds[partition_inds].reset_index(drop=True)
+        x0, y0, x1, y1 = bounds
+        x0, x1 = (x0, x1) if x0 <= x1 else (x1, x0)
+        y0, y1 = (y0, y1) if y0 <= y1 else (y1, y0)
+        partition_inds = ~(
+            (points_bounds.x1 < x0) |
+            (points_bounds.y1 < y0) |
+            (points_bounds.x0 > x1) |
+            (points_bounds.y0 > y1)
+        )
+        points_bounds = points_bounds[partition_inds].reset_index(drop=True)
 
-    lines_bounds = pd.concat([
-        ddf_packed1._partition_bounds['lines'],
-        ddf_packed2._partition_bounds['lines'],
-    ]).reset_index(drop=True)[partition_inds].reset_index(drop=True)
-    points_bounds.index.name = 'partition'
-    lines_bounds.index.name = 'partition'
-
-    # Check partition bounds
-    pd.testing.assert_frame_equal(
-        points_bounds, ddf_read._partition_bounds['points']
-    )
-
-    pd.testing.assert_frame_equal(
-        lines_bounds, ddf_read._partition_bounds['lines']
-    )
+        lines_bounds = pd.concat([
+            ddf_packed1._partition_bounds['lines'],
+            ddf_packed2._partition_bounds['lines'],
+        ]).reset_index(drop=True)[partition_inds].reset_index(drop=True)
+        points_bounds.index.name = 'partition'
+        lines_bounds.index.name = 'partition'
+
+        # Check partition bounds
+        pd.testing.assert_frame_equal(
+            points_bounds, ddf_read._partition_bounds['points']
+        )
+
+        pd.testing.assert_frame_equal(
+            lines_bounds, ddf_read._partition_bounds['lines']
+        )
 
-    # Check active geometry column
-    assert ddf_read.geometry.name == 'points'
+        # Check active geometry column
+        assert ddf_read.geometry.name == 'points'
 
 
 @pytest.mark.parametrize("filename", ["serial_5.0.0.parq", "serial_8.0.0.parq"])
 def test_read_parquet(filename):
     path = Path(__file__).parent.joinpath("test_data", filename)
     df = read_parquet(str(path))
```

### Comparing `spatialpandas-0.4.8/spatialpandas/tests/test_parquet_s3.py` & `spatialpandas-0.4.8a1/spatialpandas/tests/test_parquet_s3.py`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.8/spatialpandas/tests/tools/test_sjoin.py` & `spatialpandas-0.4.8a1/spatialpandas/tests/tools/test_sjoin.py`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.8/spatialpandas/tools/sjoin.py` & `spatialpandas-0.4.8a1/spatialpandas/tools/sjoin.py`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.8/spatialpandas/utils.py` & `spatialpandas-0.4.8a1/spatialpandas/utils.py`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.8/spatialpandas.egg-info/PKG-INFO` & `spatialpandas-0.4.8a1/spatialpandas.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spatialpandas
-Version: 0.4.8
+Version: 0.4.8a1
 Summary: Pandas extension arrays for spatial/geometric operations
 Home-page: https://github.com/holoviz/spatialpandas
 Maintainer: HoloViz developers
 Maintainer-email: developers@holoviz.org
 License: BSD-2-Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `spatialpandas-0.4.8/spatialpandas.egg-info/SOURCES.txt` & `spatialpandas-0.4.8a1/spatialpandas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

