# Comparing `tmp/py-pde-0.9.3.tar.gz` & `tmp/py-pde-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/py-pde-0.9.3.tar", last modified: Mon Aug 31 15:02:52 2020, max compression
+gzip compressed data, was "dist/py-pde-0.9.4.tar", last modified: Mon Aug 31 15:34:54 2020, max compression
```

## Comparing `py-pde-0.9.3.tar` & `py-pde-0.9.4.tar`

### file list

```diff
@@ -1,157 +1,157 @@
-drwxr-xr-x   0 dzwicker   (501) staff       (20)        0 2020-08-31 15:02:52.000000 py-pde-0.9.3/
--rw-r--r--   0 dzwicker   (501) staff       (20)     5149 2020-08-31 15:02:52.000000 py-pde-0.9.3/PKG-INFO
--rw-r--r--   0 dzwicker   (501) staff       (20)     3530 2020-08-20 08:52:33.000000 py-pde-0.9.3/README.md
-drwxr-xr-x   0 dzwicker   (501) staff       (20)        0 2020-08-31 15:02:52.000000 py-pde-0.9.3/pde/
--rw-r--r--   0 dzwicker   (501) staff       (20)      519 2020-07-24 07:48:49.000000 py-pde-0.9.3/pde/__init__.py
--rw-r--r--   0 dzwicker   (501) staff       (20)      514 2020-07-26 19:28:11.000000 py-pde-0.9.3/pde/conftest.py
-drwxr-xr-x   0 dzwicker   (501) staff       (20)        0 2020-08-31 15:02:52.000000 py-pde-0.9.3/pde/fields/
--rw-r--r--   0 dzwicker   (501) staff       (20)      661 2020-07-24 07:48:49.000000 py-pde-0.9.3/pde/fields/__init__.py
--rw-r--r--   0 dzwicker   (501) staff       (20)    64991 2020-08-31 12:21:24.000000 py-pde-0.9.3/pde/fields/base.py
--rw-r--r--   0 dzwicker   (501) staff       (20)    19934 2020-08-31 12:21:23.000000 py-pde-0.9.3/pde/fields/collection.py
--rw-r--r--   0 dzwicker   (501) staff       (20)    17316 2020-08-31 12:21:23.000000 py-pde-0.9.3/pde/fields/scalar.py
--rw-r--r--   0 dzwicker   (501) staff       (20)    11746 2020-08-31 12:21:23.000000 py-pde-0.9.3/pde/fields/tensorial.py
-drwxr-xr-x   0 dzwicker   (501) staff       (20)        0 2020-08-31 15:02:52.000000 py-pde-0.9.3/pde/fields/tests/
--rw-r--r--   0 dzwicker   (501) staff       (20)        0 2020-02-06 09:44:40.000000 py-pde-0.9.3/pde/fields/tests/__init__.py
--rw-r--r--   0 dzwicker   (501) staff       (20)     5017 2020-07-24 07:48:49.000000 py-pde-0.9.3/pde/fields/tests/test_collection.py
--rw-r--r--   0 dzwicker   (501) staff       (20)    14786 2020-07-26 11:45:24.000000 py-pde-0.9.3/pde/fields/tests/test_generic.py
--rw-r--r--   0 dzwicker   (501) staff       (20)    14332 2020-07-27 14:10:13.000000 py-pde-0.9.3/pde/fields/tests/test_scalar.py
--rw-r--r--   0 dzwicker   (501) staff       (20)     5416 2020-07-27 14:59:03.000000 py-pde-0.9.3/pde/fields/tests/test_tensorial.py
--rw-r--r--   0 dzwicker   (501) staff       (20)     6688 2020-07-27 14:59:02.000000 py-pde-0.9.3/pde/fields/tests/test_vectorial.py
--rw-r--r--   0 dzwicker   (501) staff       (20)    15572 2020-08-31 12:21:23.000000 py-pde-0.9.3/pde/fields/vectorial.py
-drwxr-xr-x   0 dzwicker   (501) staff       (20)        0 2020-08-31 15:02:52.000000 py-pde-0.9.3/pde/grids/
--rw-r--r--   0 dzwicker   (501) staff       (20)     1305 2020-07-24 07:48:49.000000 py-pde-0.9.3/pde/grids/__init__.py
--rw-r--r--   0 dzwicker   (501) staff       (20)    42635 2020-08-31 14:09:27.000000 py-pde-0.9.3/pde/grids/base.py
-drwxr-xr-x   0 dzwicker   (501) staff       (20)        0 2020-08-31 15:02:52.000000 py-pde-0.9.3/pde/grids/boundaries/
--rw-r--r--   0 dzwicker   (501) staff       (20)     5345 2020-07-24 07:48:50.000000 py-pde-0.9.3/pde/grids/boundaries/__init__.py
--rw-r--r--   0 dzwicker   (501) staff       (20)     9130 2020-08-31 12:21:23.000000 py-pde-0.9.3/pde/grids/boundaries/axes.py
--rw-r--r--   0 dzwicker   (501) staff       (20)    22330 2020-08-31 12:21:23.000000 py-pde-0.9.3/pde/grids/boundaries/axis.py
--rw-r--r--   0 dzwicker   (501) staff       (20)    53280 2020-08-31 12:21:25.000000 py-pde-0.9.3/pde/grids/boundaries/local.py
-drwxr-xr-x   0 dzwicker   (501) staff       (20)        0 2020-08-31 15:02:52.000000 py-pde-0.9.3/pde/grids/boundaries/tests/
--rw-r--r--   0 dzwicker   (501) staff       (20)        0 2020-02-05 16:30:57.000000 py-pde-0.9.3/pde/grids/boundaries/tests/__init__.py
--rw-r--r--   0 dzwicker   (501) staff       (20)     3311 2020-08-24 12:06:50.000000 py-pde-0.9.3/pde/grids/boundaries/tests/test_axes.py
--rw-r--r--   0 dzwicker   (501) staff       (20)     1946 2020-07-27 18:29:53.000000 py-pde-0.9.3/pde/grids/boundaries/tests/test_axis.py
--rw-r--r--   0 dzwicker   (501) staff       (20)     8615 2020-08-24 11:44:41.000000 py-pde-0.9.3/pde/grids/boundaries/tests/test_local.py
--rw-r--r--   0 dzwicker   (501) staff       (20)    30341 2020-08-31 12:22:29.000000 py-pde-0.9.3/pde/grids/cartesian.py
--rw-r--r--   0 dzwicker   (501) staff       (20)    20246 2020-08-31 12:23:09.000000 py-pde-0.9.3/pde/grids/cylindrical.py
-drwxr-xr-x   0 dzwicker   (501) staff       (20)        0 2020-08-31 15:02:52.000000 py-pde-0.9.3/pde/grids/operators/
--rw-r--r--   0 dzwicker   (501) staff       (20)      353 2020-07-24 07:48:49.000000 py-pde-0.9.3/pde/grids/operators/__init__.py
--rw-r--r--   0 dzwicker   (501) staff       (20)    50017 2020-08-31 12:21:25.000000 py-pde-0.9.3/pde/grids/operators/cartesian.py
--rw-r--r--   0 dzwicker   (501) staff       (20)     4565 2020-08-31 12:21:23.000000 py-pde-0.9.3/pde/grids/operators/common.py
--rw-r--r--   0 dzwicker   (501) staff       (20)    14592 2020-08-31 12:21:24.000000 py-pde-0.9.3/pde/grids/operators/cylindrical.py
--rw-r--r--   0 dzwicker   (501) staff       (20)    13411 2020-08-31 12:21:24.000000 py-pde-0.9.3/pde/grids/operators/polar.py
--rw-r--r--   0 dzwicker   (501) staff       (20)    17270 2020-08-31 12:21:24.000000 py-pde-0.9.3/pde/grids/operators/spherical.py
-drwxr-xr-x   0 dzwicker   (501) staff       (20)        0 2020-08-31 15:02:52.000000 py-pde-0.9.3/pde/grids/operators/tests/
--rw-r--r--   0 dzwicker   (501) staff       (20)        0 2019-05-28 08:36:22.000000 py-pde-0.9.3/pde/grids/operators/tests/__init__.py
--rw-r--r--   0 dzwicker   (501) staff       (20)    12471 2020-08-31 12:21:24.000000 py-pde-0.9.3/pde/grids/operators/tests/test_cartesian.py
--rw-r--r--   0 dzwicker   (501) staff       (20)     5968 2020-08-31 12:21:24.000000 py-pde-0.9.3/pde/grids/operators/tests/test_cylindrical.py
--rw-r--r--   0 dzwicker   (501) staff       (20)     4665 2020-07-24 07:48:49.000000 py-pde-0.9.3/pde/grids/operators/tests/test_polar.py
--rw-r--r--   0 dzwicker   (501) staff       (20)     5081 2020-07-24 07:48:49.000000 py-pde-0.9.3/pde/grids/operators/tests/test_spherical.py
--rw-r--r--   0 dzwicker   (501) staff       (20)    23041 2020-08-31 12:21:24.000000 py-pde-0.9.3/pde/grids/spherical.py
-drwxr-xr-x   0 dzwicker   (501) staff       (20)        0 2020-08-31 15:02:52.000000 py-pde-0.9.3/pde/grids/tests/
--rw-r--r--   0 dzwicker   (501) staff       (20)        0 2020-02-05 16:31:17.000000 py-pde-0.9.3/pde/grids/tests/__init__.py
--rw-r--r--   0 dzwicker   (501) staff       (20)    14434 2020-08-31 14:08:06.000000 py-pde-0.9.3/pde/grids/tests/test_cartesian.py
--rw-r--r--   0 dzwicker   (501) staff       (20)     3695 2020-08-31 13:48:01.000000 py-pde-0.9.3/pde/grids/tests/test_cylindrical.py
--rw-r--r--   0 dzwicker   (501) staff       (20)     4163 2020-08-31 14:08:59.000000 py-pde-0.9.3/pde/grids/tests/test_generic.py
--rw-r--r--   0 dzwicker   (501) staff       (20)     7272 2020-08-31 13:48:25.000000 py-pde-0.9.3/pde/grids/tests/test_spherical.py
-drwxr-xr-x   0 dzwicker   (501) staff       (20)        0 2020-08-31 15:02:52.000000 py-pde-0.9.3/pde/pdes/
--rw-r--r--   0 dzwicker   (501) staff       (20)     1437 2020-07-24 07:48:49.000000 py-pde-0.9.3/pde/pdes/__init__.py
--rw-r--r--   0 dzwicker   (501) staff       (20)     3155 2020-08-31 12:21:24.000000 py-pde-0.9.3/pde/pdes/allen_cahn.py
--rw-r--r--   0 dzwicker   (501) staff       (20)    16325 2020-08-31 12:21:24.000000 py-pde-0.9.3/pde/pdes/base.py
--rw-r--r--   0 dzwicker   (501) staff       (20)     3655 2020-08-31 12:21:24.000000 py-pde-0.9.3/pde/pdes/cahn_hilliard.py
--rw-r--r--   0 dzwicker   (501) staff       (20)     3161 2020-08-31 12:21:24.000000 py-pde-0.9.3/pde/pdes/diffusion.py
--rw-r--r--   0 dzwicker   (501) staff       (20)     4010 2020-08-31 12:21:24.000000 py-pde-0.9.3/pde/pdes/kpz_interface.py
--rw-r--r--   0 dzwicker   (501) staff       (20)     4337 2020-08-31 12:21:24.000000 py-pde-0.9.3/pde/pdes/kuramoto_sivashinsky.py
--rw-r--r--   0 dzwicker   (501) staff       (20)     3242 2020-08-31 12:21:24.000000 py-pde-0.9.3/pde/pdes/laplace.py
--rw-r--r--   0 dzwicker   (501) staff       (20)    15144 2020-08-31 12:21:24.000000 py-pde-0.9.3/pde/pdes/pde.py
--rw-r--r--   0 dzwicker   (501) staff       (20)     4664 2020-08-31 12:21:24.000000 py-pde-0.9.3/pde/pdes/swift_hohenberg.py
-drwxr-xr-x   0 dzwicker   (501) staff       (20)        0 2020-08-31 15:02:52.000000 py-pde-0.9.3/pde/pdes/tests/
--rw-r--r--   0 dzwicker   (501) staff       (20)        0 2020-02-06 10:29:51.000000 py-pde-0.9.3/pde/pdes/tests/__init__.py
--rw-r--r--   0 dzwicker   (501) staff       (20)     2038 2020-07-24 07:48:50.000000 py-pde-0.9.3/pde/pdes/tests/test_diffusion.py
--rw-r--r--   0 dzwicker   (501) staff       (20)     1661 2020-08-20 14:35:46.000000 py-pde-0.9.3/pde/pdes/tests/test_generic.py
--rw-r--r--   0 dzwicker   (501) staff       (20)     1933 2020-07-24 07:48:50.000000 py-pde-0.9.3/pde/pdes/tests/test_laplace.py
--rw-r--r--   0 dzwicker   (501) staff       (20)     4777 2020-07-24 07:48:50.000000 py-pde-0.9.3/pde/pdes/tests/test_pde.py
--rw-r--r--   0 dzwicker   (501) staff       (20)      912 2020-08-20 14:41:12.000000 py-pde-0.9.3/pde/pdes/tests/test_wave.py
--rw-r--r--   0 dzwicker   (501) staff       (20)     4047 2020-08-31 12:21:24.000000 py-pde-0.9.3/pde/pdes/wave.py
--rw-r--r--   0 dzwicker   (501) staff       (20)        0 2020-03-02 19:10:53.000000 py-pde-0.9.3/pde/py.typed
-drwxr-xr-x   0 dzwicker   (501) staff       (20)        0 2020-08-31 15:02:52.000000 py-pde-0.9.3/pde/solvers/
--rw-r--r--   0 dzwicker   (501) staff       (20)      854 2020-08-31 12:21:24.000000 py-pde-0.9.3/pde/solvers/__init__.py
--rw-r--r--   0 dzwicker   (501) staff       (20)     4905 2020-08-31 12:21:24.000000 py-pde-0.9.3/pde/solvers/base.py
--rw-r--r--   0 dzwicker   (501) staff       (20)     8368 2020-08-31 12:21:24.000000 py-pde-0.9.3/pde/solvers/controller.py
--rw-r--r--   0 dzwicker   (501) staff       (20)     7632 2020-08-31 12:21:24.000000 py-pde-0.9.3/pde/solvers/explicit.py
--rw-r--r--   0 dzwicker   (501) staff       (20)     5203 2020-08-31 12:21:24.000000 py-pde-0.9.3/pde/solvers/implicit.py
--rw-r--r--   0 dzwicker   (501) staff       (20)     3287 2020-08-31 12:21:24.000000 py-pde-0.9.3/pde/solvers/scipy.py
-drwxr-xr-x   0 dzwicker   (501) staff       (20)        0 2020-08-31 15:02:52.000000 py-pde-0.9.3/pde/solvers/tests/
--rw-r--r--   0 dzwicker   (501) staff       (20)        0 2020-02-10 14:56:16.000000 py-pde-0.9.3/pde/solvers/tests/__init__.py
--rw-r--r--   0 dzwicker   (501) staff       (20)     1858 2020-07-24 07:48:49.000000 py-pde-0.9.3/pde/solvers/tests/test_explicit.py
--rw-r--r--   0 dzwicker   (501) staff       (20)     1334 2020-07-24 07:48:49.000000 py-pde-0.9.3/pde/solvers/tests/test_generic.py
--rw-r--r--   0 dzwicker   (501) staff       (20)      643 2020-07-24 07:48:49.000000 py-pde-0.9.3/pde/solvers/tests/test_scipy.py
-drwxr-xr-x   0 dzwicker   (501) staff       (20)        0 2020-08-31 15:02:52.000000 py-pde-0.9.3/pde/storage/
--rw-r--r--   0 dzwicker   (501) staff       (20)      320 2020-07-24 07:48:49.000000 py-pde-0.9.3/pde/storage/__init__.py
--rw-r--r--   0 dzwicker   (501) staff       (20)    13701 2020-08-31 12:21:25.000000 py-pde-0.9.3/pde/storage/base.py
--rw-r--r--   0 dzwicker   (501) staff       (20)    13816 2020-08-31 12:21:25.000000 py-pde-0.9.3/pde/storage/file.py
--rw-r--r--   0 dzwicker   (501) staff       (20)     8472 2020-08-31 12:21:25.000000 py-pde-0.9.3/pde/storage/memory.py
-drwxr-xr-x   0 dzwicker   (501) staff       (20)        0 2020-08-31 15:02:52.000000 py-pde-0.9.3/pde/storage/tests/
--rw-r--r--   0 dzwicker   (501) staff       (20)        0 2020-02-06 09:53:06.000000 py-pde-0.9.3/pde/storage/tests/__init__.py
--rw-r--r--   0 dzwicker   (501) staff       (20)     5462 2020-08-31 12:21:25.000000 py-pde-0.9.3/pde/storage/tests/test_file.py
--rw-r--r--   0 dzwicker   (501) staff       (20)     4739 2020-07-24 07:48:49.000000 py-pde-0.9.3/pde/storage/tests/test_generic.py
--rw-r--r--   0 dzwicker   (501) staff       (20)     1714 2020-07-24 07:48:50.000000 py-pde-0.9.3/pde/storage/tests/test_memory.py
-drwxr-xr-x   0 dzwicker   (501) staff       (20)        0 2020-08-31 15:02:52.000000 py-pde-0.9.3/pde/tests/
--rw-r--r--   0 dzwicker   (501) staff       (20)        0 2020-02-06 15:46:39.000000 py-pde-0.9.3/pde/tests/__init__.py
--rw-r--r--   0 dzwicker   (501) staff       (20)     2473 2020-07-24 07:48:49.000000 py-pde-0.9.3/pde/tests/test_examples.py
--rw-r--r--   0 dzwicker   (501) staff       (20)     1156 2020-07-24 07:48:49.000000 py-pde-0.9.3/pde/tests/test_integration.py
-drwxr-xr-x   0 dzwicker   (501) staff       (20)        0 2020-08-31 15:02:52.000000 py-pde-0.9.3/pde/tools/
--rw-r--r--   0 dzwicker   (501) staff       (20)      310 2020-07-27 17:51:09.000000 py-pde-0.9.3/pde/tools/__init__.py
--rw-r--r--   0 dzwicker   (501) staff       (20)    20925 2020-08-31 12:21:25.000000 py-pde-0.9.3/pde/tools/cache.py
--rw-r--r--   0 dzwicker   (501) staff       (20)     8008 2020-08-31 12:21:25.000000 py-pde-0.9.3/pde/tools/cuboid.py
--rw-r--r--   0 dzwicker   (501) staff       (20)     7082 2020-08-31 12:21:25.000000 py-pde-0.9.3/pde/tools/docstrings.py
--rw-r--r--   0 dzwicker   (501) staff       (20)    22875 2020-08-31 12:21:25.000000 py-pde-0.9.3/pde/tools/expressions.py
--rw-r--r--   0 dzwicker   (501) staff       (20)     1905 2020-08-31 12:21:25.000000 py-pde-0.9.3/pde/tools/math.py
--rw-r--r--   0 dzwicker   (501) staff       (20)    10150 2020-08-31 12:21:25.000000 py-pde-0.9.3/pde/tools/misc.py
--rw-r--r--   0 dzwicker   (501) staff       (20)    13050 2020-08-31 12:21:25.000000 py-pde-0.9.3/pde/tools/numba.py
--rw-r--r--   0 dzwicker   (501) staff       (20)     5188 2020-08-31 12:21:25.000000 py-pde-0.9.3/pde/tools/output.py
--rw-r--r--   0 dzwicker   (501) staff       (20)    17668 2020-08-31 12:21:25.000000 py-pde-0.9.3/pde/tools/parameters.py
--rw-r--r--   0 dzwicker   (501) staff       (20)     4094 2020-08-31 12:21:25.000000 py-pde-0.9.3/pde/tools/parse_duration.py
--rw-r--r--   0 dzwicker   (501) staff       (20)    26866 2020-08-31 12:21:25.000000 py-pde-0.9.3/pde/tools/plotting.py
--rw-r--r--   0 dzwicker   (501) staff       (20)     2704 2020-08-31 12:21:25.000000 py-pde-0.9.3/pde/tools/spectral.py
--rw-r--r--   0 dzwicker   (501) staff       (20)    21742 2020-08-31 12:21:25.000000 py-pde-0.9.3/pde/tools/spherical.py
-drwxr-xr-x   0 dzwicker   (501) staff       (20)        0 2020-08-31 15:02:52.000000 py-pde-0.9.3/pde/tools/tests/
--rw-r--r--   0 dzwicker   (501) staff       (20)        0 2019-03-15 09:50:41.000000 py-pde-0.9.3/pde/tools/tests/__init__.py
--rw-r--r--   0 dzwicker   (501) staff       (20)    15514 2020-08-31 12:21:26.000000 py-pde-0.9.3/pde/tools/tests/test_cache.py
--rw-r--r--   0 dzwicker   (501) staff       (20)     3914 2020-07-24 07:48:49.000000 py-pde-0.9.3/pde/tools/tests/test_cuboid.py
--rw-r--r--   0 dzwicker   (501) staff       (20)     6956 2020-07-24 07:48:49.000000 py-pde-0.9.3/pde/tools/tests/test_expressions.py
--rw-r--r--   0 dzwicker   (501) staff       (20)      505 2020-07-24 07:48:49.000000 py-pde-0.9.3/pde/tools/tests/test_math.py
--rw-r--r--   0 dzwicker   (501) staff       (20)     2843 2020-07-27 17:52:30.000000 py-pde-0.9.3/pde/tools/tests/test_misc.py
--rw-r--r--   0 dzwicker   (501) staff       (20)     1207 2020-07-24 07:48:49.000000 py-pde-0.9.3/pde/tools/tests/test_numba.py
--rw-r--r--   0 dzwicker   (501) staff       (20)      672 2020-07-27 18:27:46.000000 py-pde-0.9.3/pde/tools/tests/test_output.py
--rw-r--r--   0 dzwicker   (501) staff       (20)     5300 2020-07-27 18:25:53.000000 py-pde-0.9.3/pde/tools/tests/test_parameters.py
--rw-r--r--   0 dzwicker   (501) staff       (20)      356 2020-07-24 07:48:49.000000 py-pde-0.9.3/pde/tools/tests/test_parse_duration.py
--rw-r--r--   0 dzwicker   (501) staff       (20)      706 2020-07-24 07:48:49.000000 py-pde-0.9.3/pde/tools/tests/test_plotting.py
--rw-r--r--   0 dzwicker   (501) staff       (20)     2658 2020-08-31 12:21:25.000000 py-pde-0.9.3/pde/tools/tests/test_spectral.py
--rw-r--r--   0 dzwicker   (501) staff       (20)     5629 2020-07-24 07:48:49.000000 py-pde-0.9.3/pde/tools/tests/test_spherical.py
-drwxr-xr-x   0 dzwicker   (501) staff       (20)        0 2020-08-31 15:02:52.000000 py-pde-0.9.3/pde/trackers/
--rw-r--r--   0 dzwicker   (501) staff       (20)     1027 2020-07-24 07:48:50.000000 py-pde-0.9.3/pde/trackers/__init__.py
--rw-r--r--   0 dzwicker   (501) staff       (20)     8040 2020-08-31 12:21:25.000000 py-pde-0.9.3/pde/trackers/base.py
--rw-r--r--   0 dzwicker   (501) staff       (20)     6706 2020-08-31 12:21:25.000000 py-pde-0.9.3/pde/trackers/intervals.py
-drwxr-xr-x   0 dzwicker   (501) staff       (20)        0 2020-08-31 15:02:52.000000 py-pde-0.9.3/pde/trackers/tests/
--rw-r--r--   0 dzwicker   (501) staff       (20)        0 2020-02-06 10:07:51.000000 py-pde-0.9.3/pde/trackers/tests/__init__.py
--rw-r--r--   0 dzwicker   (501) staff       (20)     1178 2020-07-24 07:48:50.000000 py-pde-0.9.3/pde/trackers/tests/test_intervals.py
--rw-r--r--   0 dzwicker   (501) staff       (20)     7072 2020-08-31 12:21:25.000000 py-pde-0.9.3/pde/trackers/tests/test_trackers.py
--rw-r--r--   0 dzwicker   (501) staff       (20)    33068 2020-08-31 12:21:26.000000 py-pde-0.9.3/pde/trackers/trackers.py
--rw-r--r--   0 dzwicker   (501) staff       (20)      136 2020-08-31 14:16:32.000000 py-pde-0.9.3/pde/version.py
-drwxr-xr-x   0 dzwicker   (501) staff       (20)        0 2020-08-31 15:02:52.000000 py-pde-0.9.3/pde/visualization/
--rw-r--r--   0 dzwicker   (501) staff       (20)      300 2020-07-24 07:48:49.000000 py-pde-0.9.3/pde/visualization/__init__.py
--rw-r--r--   0 dzwicker   (501) staff       (20)     6104 2020-08-31 12:21:25.000000 py-pde-0.9.3/pde/visualization/movies.py
--rw-r--r--   0 dzwicker   (501) staff       (20)    26694 2020-08-31 12:21:26.000000 py-pde-0.9.3/pde/visualization/plotting.py
-drwxr-xr-x   0 dzwicker   (501) staff       (20)        0 2020-08-31 15:02:52.000000 py-pde-0.9.3/pde/visualization/tests/
--rw-r--r--   0 dzwicker   (501) staff       (20)        0 2018-08-01 06:48:43.000000 py-pde-0.9.3/pde/visualization/tests/__init__.py
--rw-r--r--   0 dzwicker   (501) staff       (20)     1485 2020-07-24 07:48:49.000000 py-pde-0.9.3/pde/visualization/tests/test_movies.py
--rw-r--r--   0 dzwicker   (501) staff       (20)     3271 2020-07-24 07:48:49.000000 py-pde-0.9.3/pde/visualization/tests/test_plotting.py
-drwxr-xr-x   0 dzwicker   (501) staff       (20)        0 2020-08-31 15:02:52.000000 py-pde-0.9.3/py_pde.egg-info/
--rw-r--r--   0 dzwicker   (501) staff       (20)     5149 2020-08-31 15:02:52.000000 py-pde-0.9.3/py_pde.egg-info/PKG-INFO
--rw-r--r--   0 dzwicker   (501) staff       (20)     3678 2020-08-31 15:02:52.000000 py-pde-0.9.3/py_pde.egg-info/SOURCES.txt
--rw-r--r--   0 dzwicker   (501) staff       (20)        1 2020-08-31 15:02:52.000000 py-pde-0.9.3/py_pde.egg-info/dependency_links.txt
--rw-r--r--   0 dzwicker   (501) staff       (20)        1 2020-08-31 15:02:52.000000 py-pde-0.9.3/py_pde.egg-info/not-zip-safe
--rw-r--r--   0 dzwicker   (501) staff       (20)      100 2020-08-31 15:02:52.000000 py-pde-0.9.3/py_pde.egg-info/requires.txt
--rw-r--r--   0 dzwicker   (501) staff       (20)        4 2020-08-31 15:02:52.000000 py-pde-0.9.3/py_pde.egg-info/top_level.txt
--rw-r--r--   0 dzwicker   (501) staff       (20)       79 2020-08-31 15:02:52.000000 py-pde-0.9.3/setup.cfg
--rw-r--r--   0 dzwicker   (501) staff       (20)     1748 2020-07-24 09:38:22.000000 py-pde-0.9.3/setup.py
+drwxr-xr-x   0 dzwicker   (501) staff       (20)        0 2020-08-31 15:34:54.000000 py-pde-0.9.4/
+-rw-r--r--   0 dzwicker   (501) staff       (20)     5149 2020-08-31 15:34:54.000000 py-pde-0.9.4/PKG-INFO
+-rw-r--r--   0 dzwicker   (501) staff       (20)     3530 2020-08-20 08:52:33.000000 py-pde-0.9.4/README.md
+drwxr-xr-x   0 dzwicker   (501) staff       (20)        0 2020-08-31 15:34:54.000000 py-pde-0.9.4/pde/
+-rw-r--r--   0 dzwicker   (501) staff       (20)      519 2020-07-24 07:48:49.000000 py-pde-0.9.4/pde/__init__.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)      514 2020-07-26 19:28:11.000000 py-pde-0.9.4/pde/conftest.py
+drwxr-xr-x   0 dzwicker   (501) staff       (20)        0 2020-08-31 15:34:54.000000 py-pde-0.9.4/pde/fields/
+-rw-r--r--   0 dzwicker   (501) staff       (20)      661 2020-07-24 07:48:49.000000 py-pde-0.9.4/pde/fields/__init__.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)    64991 2020-08-31 12:21:24.000000 py-pde-0.9.4/pde/fields/base.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)    19934 2020-08-31 12:21:23.000000 py-pde-0.9.4/pde/fields/collection.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)    17316 2020-08-31 12:21:23.000000 py-pde-0.9.4/pde/fields/scalar.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)    11746 2020-08-31 12:21:23.000000 py-pde-0.9.4/pde/fields/tensorial.py
+drwxr-xr-x   0 dzwicker   (501) staff       (20)        0 2020-08-31 15:34:54.000000 py-pde-0.9.4/pde/fields/tests/
+-rw-r--r--   0 dzwicker   (501) staff       (20)        0 2020-02-06 09:44:40.000000 py-pde-0.9.4/pde/fields/tests/__init__.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)     5017 2020-07-24 07:48:49.000000 py-pde-0.9.4/pde/fields/tests/test_collection.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)    14786 2020-07-26 11:45:24.000000 py-pde-0.9.4/pde/fields/tests/test_generic.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)    14332 2020-07-27 14:10:13.000000 py-pde-0.9.4/pde/fields/tests/test_scalar.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)     5416 2020-07-27 14:59:03.000000 py-pde-0.9.4/pde/fields/tests/test_tensorial.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)     6688 2020-07-27 14:59:02.000000 py-pde-0.9.4/pde/fields/tests/test_vectorial.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)    15572 2020-08-31 12:21:23.000000 py-pde-0.9.4/pde/fields/vectorial.py
+drwxr-xr-x   0 dzwicker   (501) staff       (20)        0 2020-08-31 15:34:54.000000 py-pde-0.9.4/pde/grids/
+-rw-r--r--   0 dzwicker   (501) staff       (20)     1305 2020-07-24 07:48:49.000000 py-pde-0.9.4/pde/grids/__init__.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)    42619 2020-08-31 15:26:37.000000 py-pde-0.9.4/pde/grids/base.py
+drwxr-xr-x   0 dzwicker   (501) staff       (20)        0 2020-08-31 15:34:54.000000 py-pde-0.9.4/pde/grids/boundaries/
+-rw-r--r--   0 dzwicker   (501) staff       (20)     5345 2020-07-24 07:48:50.000000 py-pde-0.9.4/pde/grids/boundaries/__init__.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)     9130 2020-08-31 12:21:23.000000 py-pde-0.9.4/pde/grids/boundaries/axes.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)    22330 2020-08-31 12:21:23.000000 py-pde-0.9.4/pde/grids/boundaries/axis.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)    53280 2020-08-31 12:21:25.000000 py-pde-0.9.4/pde/grids/boundaries/local.py
+drwxr-xr-x   0 dzwicker   (501) staff       (20)        0 2020-08-31 15:34:54.000000 py-pde-0.9.4/pde/grids/boundaries/tests/
+-rw-r--r--   0 dzwicker   (501) staff       (20)        0 2020-02-05 16:30:57.000000 py-pde-0.9.4/pde/grids/boundaries/tests/__init__.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)     3311 2020-08-24 12:06:50.000000 py-pde-0.9.4/pde/grids/boundaries/tests/test_axes.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)     1946 2020-07-27 18:29:53.000000 py-pde-0.9.4/pde/grids/boundaries/tests/test_axis.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)     8615 2020-08-24 11:44:41.000000 py-pde-0.9.4/pde/grids/boundaries/tests/test_local.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)    30341 2020-08-31 12:22:29.000000 py-pde-0.9.4/pde/grids/cartesian.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)    20246 2020-08-31 12:23:09.000000 py-pde-0.9.4/pde/grids/cylindrical.py
+drwxr-xr-x   0 dzwicker   (501) staff       (20)        0 2020-08-31 15:34:54.000000 py-pde-0.9.4/pde/grids/operators/
+-rw-r--r--   0 dzwicker   (501) staff       (20)      353 2020-07-24 07:48:49.000000 py-pde-0.9.4/pde/grids/operators/__init__.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)    50017 2020-08-31 12:21:25.000000 py-pde-0.9.4/pde/grids/operators/cartesian.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)     4565 2020-08-31 12:21:23.000000 py-pde-0.9.4/pde/grids/operators/common.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)    14592 2020-08-31 12:21:24.000000 py-pde-0.9.4/pde/grids/operators/cylindrical.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)    13411 2020-08-31 12:21:24.000000 py-pde-0.9.4/pde/grids/operators/polar.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)    17270 2020-08-31 12:21:24.000000 py-pde-0.9.4/pde/grids/operators/spherical.py
+drwxr-xr-x   0 dzwicker   (501) staff       (20)        0 2020-08-31 15:34:54.000000 py-pde-0.9.4/pde/grids/operators/tests/
+-rw-r--r--   0 dzwicker   (501) staff       (20)        0 2019-05-28 08:36:22.000000 py-pde-0.9.4/pde/grids/operators/tests/__init__.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)    12471 2020-08-31 12:21:24.000000 py-pde-0.9.4/pde/grids/operators/tests/test_cartesian.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)     5968 2020-08-31 12:21:24.000000 py-pde-0.9.4/pde/grids/operators/tests/test_cylindrical.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)     4665 2020-07-24 07:48:49.000000 py-pde-0.9.4/pde/grids/operators/tests/test_polar.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)     5081 2020-07-24 07:48:49.000000 py-pde-0.9.4/pde/grids/operators/tests/test_spherical.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)    23041 2020-08-31 12:21:24.000000 py-pde-0.9.4/pde/grids/spherical.py
+drwxr-xr-x   0 dzwicker   (501) staff       (20)        0 2020-08-31 15:34:54.000000 py-pde-0.9.4/pde/grids/tests/
+-rw-r--r--   0 dzwicker   (501) staff       (20)        0 2020-02-05 16:31:17.000000 py-pde-0.9.4/pde/grids/tests/__init__.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)    14434 2020-08-31 14:08:06.000000 py-pde-0.9.4/pde/grids/tests/test_cartesian.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)     3695 2020-08-31 13:48:01.000000 py-pde-0.9.4/pde/grids/tests/test_cylindrical.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)     4213 2020-08-31 15:26:09.000000 py-pde-0.9.4/pde/grids/tests/test_generic.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)     7272 2020-08-31 13:48:25.000000 py-pde-0.9.4/pde/grids/tests/test_spherical.py
+drwxr-xr-x   0 dzwicker   (501) staff       (20)        0 2020-08-31 15:34:54.000000 py-pde-0.9.4/pde/pdes/
+-rw-r--r--   0 dzwicker   (501) staff       (20)     1437 2020-07-24 07:48:49.000000 py-pde-0.9.4/pde/pdes/__init__.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)     3155 2020-08-31 12:21:24.000000 py-pde-0.9.4/pde/pdes/allen_cahn.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)    16325 2020-08-31 12:21:24.000000 py-pde-0.9.4/pde/pdes/base.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)     3655 2020-08-31 12:21:24.000000 py-pde-0.9.4/pde/pdes/cahn_hilliard.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)     3161 2020-08-31 12:21:24.000000 py-pde-0.9.4/pde/pdes/diffusion.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)     4010 2020-08-31 12:21:24.000000 py-pde-0.9.4/pde/pdes/kpz_interface.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)     4337 2020-08-31 12:21:24.000000 py-pde-0.9.4/pde/pdes/kuramoto_sivashinsky.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)     3242 2020-08-31 12:21:24.000000 py-pde-0.9.4/pde/pdes/laplace.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)    15144 2020-08-31 12:21:24.000000 py-pde-0.9.4/pde/pdes/pde.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)     4664 2020-08-31 12:21:24.000000 py-pde-0.9.4/pde/pdes/swift_hohenberg.py
+drwxr-xr-x   0 dzwicker   (501) staff       (20)        0 2020-08-31 15:34:54.000000 py-pde-0.9.4/pde/pdes/tests/
+-rw-r--r--   0 dzwicker   (501) staff       (20)        0 2020-02-06 10:29:51.000000 py-pde-0.9.4/pde/pdes/tests/__init__.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)     2038 2020-07-24 07:48:50.000000 py-pde-0.9.4/pde/pdes/tests/test_diffusion.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)     1661 2020-08-20 14:35:46.000000 py-pde-0.9.4/pde/pdes/tests/test_generic.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)     1933 2020-07-24 07:48:50.000000 py-pde-0.9.4/pde/pdes/tests/test_laplace.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)     4777 2020-07-24 07:48:50.000000 py-pde-0.9.4/pde/pdes/tests/test_pde.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)      912 2020-08-20 14:41:12.000000 py-pde-0.9.4/pde/pdes/tests/test_wave.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)     4047 2020-08-31 12:21:24.000000 py-pde-0.9.4/pde/pdes/wave.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)        0 2020-03-02 19:10:53.000000 py-pde-0.9.4/pde/py.typed
+drwxr-xr-x   0 dzwicker   (501) staff       (20)        0 2020-08-31 15:34:54.000000 py-pde-0.9.4/pde/solvers/
+-rw-r--r--   0 dzwicker   (501) staff       (20)      854 2020-08-31 12:21:24.000000 py-pde-0.9.4/pde/solvers/__init__.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)     4905 2020-08-31 12:21:24.000000 py-pde-0.9.4/pde/solvers/base.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)     8368 2020-08-31 12:21:24.000000 py-pde-0.9.4/pde/solvers/controller.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)     7632 2020-08-31 12:21:24.000000 py-pde-0.9.4/pde/solvers/explicit.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)     5203 2020-08-31 12:21:24.000000 py-pde-0.9.4/pde/solvers/implicit.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)     3287 2020-08-31 12:21:24.000000 py-pde-0.9.4/pde/solvers/scipy.py
+drwxr-xr-x   0 dzwicker   (501) staff       (20)        0 2020-08-31 15:34:54.000000 py-pde-0.9.4/pde/solvers/tests/
+-rw-r--r--   0 dzwicker   (501) staff       (20)        0 2020-02-10 14:56:16.000000 py-pde-0.9.4/pde/solvers/tests/__init__.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)     1858 2020-07-24 07:48:49.000000 py-pde-0.9.4/pde/solvers/tests/test_explicit.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)     1334 2020-07-24 07:48:49.000000 py-pde-0.9.4/pde/solvers/tests/test_generic.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)      643 2020-07-24 07:48:49.000000 py-pde-0.9.4/pde/solvers/tests/test_scipy.py
+drwxr-xr-x   0 dzwicker   (501) staff       (20)        0 2020-08-31 15:34:54.000000 py-pde-0.9.4/pde/storage/
+-rw-r--r--   0 dzwicker   (501) staff       (20)      320 2020-07-24 07:48:49.000000 py-pde-0.9.4/pde/storage/__init__.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)    13701 2020-08-31 12:21:25.000000 py-pde-0.9.4/pde/storage/base.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)    13816 2020-08-31 12:21:25.000000 py-pde-0.9.4/pde/storage/file.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)     8472 2020-08-31 12:21:25.000000 py-pde-0.9.4/pde/storage/memory.py
+drwxr-xr-x   0 dzwicker   (501) staff       (20)        0 2020-08-31 15:34:54.000000 py-pde-0.9.4/pde/storage/tests/
+-rw-r--r--   0 dzwicker   (501) staff       (20)        0 2020-02-06 09:53:06.000000 py-pde-0.9.4/pde/storage/tests/__init__.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)     5462 2020-08-31 12:21:25.000000 py-pde-0.9.4/pde/storage/tests/test_file.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)     4739 2020-07-24 07:48:49.000000 py-pde-0.9.4/pde/storage/tests/test_generic.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)     1714 2020-07-24 07:48:50.000000 py-pde-0.9.4/pde/storage/tests/test_memory.py
+drwxr-xr-x   0 dzwicker   (501) staff       (20)        0 2020-08-31 15:34:54.000000 py-pde-0.9.4/pde/tests/
+-rw-r--r--   0 dzwicker   (501) staff       (20)        0 2020-02-06 15:46:39.000000 py-pde-0.9.4/pde/tests/__init__.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)     2473 2020-07-24 07:48:49.000000 py-pde-0.9.4/pde/tests/test_examples.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)     1156 2020-07-24 07:48:49.000000 py-pde-0.9.4/pde/tests/test_integration.py
+drwxr-xr-x   0 dzwicker   (501) staff       (20)        0 2020-08-31 15:34:54.000000 py-pde-0.9.4/pde/tools/
+-rw-r--r--   0 dzwicker   (501) staff       (20)      310 2020-07-27 17:51:09.000000 py-pde-0.9.4/pde/tools/__init__.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)    20925 2020-08-31 12:21:25.000000 py-pde-0.9.4/pde/tools/cache.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)     8008 2020-08-31 12:21:25.000000 py-pde-0.9.4/pde/tools/cuboid.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)     7082 2020-08-31 12:21:25.000000 py-pde-0.9.4/pde/tools/docstrings.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)    22875 2020-08-31 12:21:25.000000 py-pde-0.9.4/pde/tools/expressions.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)     1905 2020-08-31 12:21:25.000000 py-pde-0.9.4/pde/tools/math.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)    10150 2020-08-31 12:21:25.000000 py-pde-0.9.4/pde/tools/misc.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)    13050 2020-08-31 12:21:25.000000 py-pde-0.9.4/pde/tools/numba.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)     5188 2020-08-31 12:21:25.000000 py-pde-0.9.4/pde/tools/output.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)    17668 2020-08-31 12:21:25.000000 py-pde-0.9.4/pde/tools/parameters.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)     4094 2020-08-31 12:21:25.000000 py-pde-0.9.4/pde/tools/parse_duration.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)    26866 2020-08-31 12:21:25.000000 py-pde-0.9.4/pde/tools/plotting.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)     2704 2020-08-31 12:21:25.000000 py-pde-0.9.4/pde/tools/spectral.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)    21742 2020-08-31 12:21:25.000000 py-pde-0.9.4/pde/tools/spherical.py
+drwxr-xr-x   0 dzwicker   (501) staff       (20)        0 2020-08-31 15:34:54.000000 py-pde-0.9.4/pde/tools/tests/
+-rw-r--r--   0 dzwicker   (501) staff       (20)        0 2019-03-15 09:50:41.000000 py-pde-0.9.4/pde/tools/tests/__init__.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)    15514 2020-08-31 12:21:26.000000 py-pde-0.9.4/pde/tools/tests/test_cache.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)     3914 2020-07-24 07:48:49.000000 py-pde-0.9.4/pde/tools/tests/test_cuboid.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)     6956 2020-07-24 07:48:49.000000 py-pde-0.9.4/pde/tools/tests/test_expressions.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)      505 2020-07-24 07:48:49.000000 py-pde-0.9.4/pde/tools/tests/test_math.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)     2843 2020-07-27 17:52:30.000000 py-pde-0.9.4/pde/tools/tests/test_misc.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)     1207 2020-07-24 07:48:49.000000 py-pde-0.9.4/pde/tools/tests/test_numba.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)      672 2020-07-27 18:27:46.000000 py-pde-0.9.4/pde/tools/tests/test_output.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)     5300 2020-07-27 18:25:53.000000 py-pde-0.9.4/pde/tools/tests/test_parameters.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)      356 2020-07-24 07:48:49.000000 py-pde-0.9.4/pde/tools/tests/test_parse_duration.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)      706 2020-07-24 07:48:49.000000 py-pde-0.9.4/pde/tools/tests/test_plotting.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)     2658 2020-08-31 12:21:25.000000 py-pde-0.9.4/pde/tools/tests/test_spectral.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)     5629 2020-07-24 07:48:49.000000 py-pde-0.9.4/pde/tools/tests/test_spherical.py
+drwxr-xr-x   0 dzwicker   (501) staff       (20)        0 2020-08-31 15:34:54.000000 py-pde-0.9.4/pde/trackers/
+-rw-r--r--   0 dzwicker   (501) staff       (20)     1027 2020-07-24 07:48:50.000000 py-pde-0.9.4/pde/trackers/__init__.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)     8040 2020-08-31 12:21:25.000000 py-pde-0.9.4/pde/trackers/base.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)     6706 2020-08-31 12:21:25.000000 py-pde-0.9.4/pde/trackers/intervals.py
+drwxr-xr-x   0 dzwicker   (501) staff       (20)        0 2020-08-31 15:34:54.000000 py-pde-0.9.4/pde/trackers/tests/
+-rw-r--r--   0 dzwicker   (501) staff       (20)        0 2020-02-06 10:07:51.000000 py-pde-0.9.4/pde/trackers/tests/__init__.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)     1178 2020-07-24 07:48:50.000000 py-pde-0.9.4/pde/trackers/tests/test_intervals.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)     7072 2020-08-31 12:21:25.000000 py-pde-0.9.4/pde/trackers/tests/test_trackers.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)    33068 2020-08-31 12:21:26.000000 py-pde-0.9.4/pde/trackers/trackers.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)      136 2020-08-31 15:26:54.000000 py-pde-0.9.4/pde/version.py
+drwxr-xr-x   0 dzwicker   (501) staff       (20)        0 2020-08-31 15:34:54.000000 py-pde-0.9.4/pde/visualization/
+-rw-r--r--   0 dzwicker   (501) staff       (20)      300 2020-07-24 07:48:49.000000 py-pde-0.9.4/pde/visualization/__init__.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)     6104 2020-08-31 12:21:25.000000 py-pde-0.9.4/pde/visualization/movies.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)    26694 2020-08-31 12:21:26.000000 py-pde-0.9.4/pde/visualization/plotting.py
+drwxr-xr-x   0 dzwicker   (501) staff       (20)        0 2020-08-31 15:34:54.000000 py-pde-0.9.4/pde/visualization/tests/
+-rw-r--r--   0 dzwicker   (501) staff       (20)        0 2018-08-01 06:48:43.000000 py-pde-0.9.4/pde/visualization/tests/__init__.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)     1485 2020-07-24 07:48:49.000000 py-pde-0.9.4/pde/visualization/tests/test_movies.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)     3271 2020-07-24 07:48:49.000000 py-pde-0.9.4/pde/visualization/tests/test_plotting.py
+drwxr-xr-x   0 dzwicker   (501) staff       (20)        0 2020-08-31 15:34:54.000000 py-pde-0.9.4/py_pde.egg-info/
+-rw-r--r--   0 dzwicker   (501) staff       (20)     5149 2020-08-31 15:34:54.000000 py-pde-0.9.4/py_pde.egg-info/PKG-INFO
+-rw-r--r--   0 dzwicker   (501) staff       (20)     3678 2020-08-31 15:34:54.000000 py-pde-0.9.4/py_pde.egg-info/SOURCES.txt
+-rw-r--r--   0 dzwicker   (501) staff       (20)        1 2020-08-31 15:34:54.000000 py-pde-0.9.4/py_pde.egg-info/dependency_links.txt
+-rw-r--r--   0 dzwicker   (501) staff       (20)        1 2020-08-31 15:34:54.000000 py-pde-0.9.4/py_pde.egg-info/not-zip-safe
+-rw-r--r--   0 dzwicker   (501) staff       (20)      100 2020-08-31 15:34:54.000000 py-pde-0.9.4/py_pde.egg-info/requires.txt
+-rw-r--r--   0 dzwicker   (501) staff       (20)        4 2020-08-31 15:34:54.000000 py-pde-0.9.4/py_pde.egg-info/top_level.txt
+-rw-r--r--   0 dzwicker   (501) staff       (20)       79 2020-08-31 15:34:54.000000 py-pde-0.9.4/setup.cfg
+-rw-r--r--   0 dzwicker   (501) staff       (20)     1748 2020-07-24 09:38:22.000000 py-pde-0.9.4/setup.py
```

### Comparing `py-pde-0.9.3/PKG-INFO` & `py-pde-0.9.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: py-pde
-Version: 0.9.3
+Version: 0.9.4
 Summary: Python package for solving partial differential equations
 Home-page: https://github.com/zwicker-group/py-pde
 Author: David Zwicker
 Author-email: david.zwicker@ds.mpg.de
 License: MIT
-Download-URL: https://github.com/zwicker-group/py-pde/archive/v0.9.3.tar.gz
+Download-URL: https://github.com/zwicker-group/py-pde/archive/v0.9.4.tar.gz
 Description: # py-pde
         
         [![PyPI version](https://badge.fury.io/py/py-pde.svg)](https://badge.fury.io/py/py-pde)
         [![Documentation Status](https://readthedocs.org/projects/py-pde/badge/?version=latest)](https://py-pde.readthedocs.io/en/latest/?badge=latest)
         [![DOI](https://joss.theoj.org/papers/10.21105/joss.02158/status.svg)](https://doi.org/10.21105/joss.02158)
         [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/zwicker-group/py-pde/master?filepath=examples%2Fjupyter)
```

### Comparing `py-pde-0.9.3/README.md` & `py-pde-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `py-pde-0.9.3/pde/__init__.py` & `py-pde-0.9.4/pde/__init__.py`

 * *Files identical despite different names*

### Comparing `py-pde-0.9.3/pde/conftest.py` & `py-pde-0.9.4/pde/conftest.py`

 * *Files identical despite different names*

### Comparing `py-pde-0.9.3/pde/fields/__init__.py` & `py-pde-0.9.4/pde/fields/__init__.py`

 * *Files identical despite different names*

### Comparing `py-pde-0.9.3/pde/fields/base.py` & `py-pde-0.9.4/pde/fields/base.py`

 * *Files identical despite different names*

### Comparing `py-pde-0.9.3/pde/fields/collection.py` & `py-pde-0.9.4/pde/fields/collection.py`

 * *Files identical despite different names*

### Comparing `py-pde-0.9.3/pde/fields/scalar.py` & `py-pde-0.9.4/pde/fields/scalar.py`

 * *Files identical despite different names*

### Comparing `py-pde-0.9.3/pde/fields/tensorial.py` & `py-pde-0.9.4/pde/fields/tensorial.py`

 * *Files identical despite different names*

### Comparing `py-pde-0.9.3/pde/fields/tests/test_collection.py` & `py-pde-0.9.4/pde/fields/tests/test_collection.py`

 * *Files identical despite different names*

### Comparing `py-pde-0.9.3/pde/fields/tests/test_generic.py` & `py-pde-0.9.4/pde/fields/tests/test_generic.py`

 * *Files identical despite different names*

### Comparing `py-pde-0.9.3/pde/fields/tests/test_scalar.py` & `py-pde-0.9.4/pde/fields/tests/test_scalar.py`

 * *Files identical despite different names*

### Comparing `py-pde-0.9.3/pde/fields/tests/test_tensorial.py` & `py-pde-0.9.4/pde/fields/tests/test_tensorial.py`

 * *Files identical despite different names*

### Comparing `py-pde-0.9.3/pde/fields/tests/test_vectorial.py` & `py-pde-0.9.4/pde/fields/tests/test_vectorial.py`

 * *Files identical despite different names*

### Comparing `py-pde-0.9.3/pde/fields/vectorial.py` & `py-pde-0.9.4/pde/fields/vectorial.py`

 * *Files identical despite different names*

### Comparing `py-pde-0.9.3/pde/grids/__init__.py` & `py-pde-0.9.4/pde/grids/__init__.py`

 * *Files identical despite different names*

### Comparing `py-pde-0.9.3/pde/grids/base.py` & `py-pde-0.9.4/pde/grids/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1096,15 +1096,15 @@
             callable: A function that takes a numpy array and returns the integral with
             the correct weights given by the cell volumes.
         """
         num_axes = self.num_axes
 
         if self.uniform_cell_volumes:
             # all cells have the same volume
-            cell_volume = functools.reduce(np.outer, self.cell_volume_data)
+            cell_volume = np.product(self.cell_volume_data)
 
             @jit
             def integrate(arr: np.ndarray) -> Union[float, np.ndarray]:
                 """ function that integrates data over a uniform grid """
                 assert arr.ndim == num_axes
                 return cell_volume * arr.sum()
```

### Comparing `py-pde-0.9.3/pde/grids/boundaries/__init__.py` & `py-pde-0.9.4/pde/grids/boundaries/__init__.py`

 * *Files identical despite different names*

### Comparing `py-pde-0.9.3/pde/grids/boundaries/axes.py` & `py-pde-0.9.4/pde/grids/boundaries/axes.py`

 * *Files identical despite different names*

### Comparing `py-pde-0.9.3/pde/grids/boundaries/axis.py` & `py-pde-0.9.4/pde/grids/boundaries/axis.py`

 * *Files identical despite different names*

### Comparing `py-pde-0.9.3/pde/grids/boundaries/local.py` & `py-pde-0.9.4/pde/grids/boundaries/local.py`

 * *Files identical despite different names*

### Comparing `py-pde-0.9.3/pde/grids/boundaries/tests/test_axes.py` & `py-pde-0.9.4/pde/grids/boundaries/tests/test_axes.py`

 * *Files identical despite different names*

### Comparing `py-pde-0.9.3/pde/grids/boundaries/tests/test_axis.py` & `py-pde-0.9.4/pde/grids/boundaries/tests/test_axis.py`

 * *Files identical despite different names*

### Comparing `py-pde-0.9.3/pde/grids/boundaries/tests/test_local.py` & `py-pde-0.9.4/pde/grids/boundaries/tests/test_local.py`

 * *Files identical despite different names*

### Comparing `py-pde-0.9.3/pde/grids/cartesian.py` & `py-pde-0.9.4/pde/grids/cartesian.py`

 * *Files identical despite different names*

### Comparing `py-pde-0.9.3/pde/grids/cylindrical.py` & `py-pde-0.9.4/pde/grids/cylindrical.py`

 * *Files identical despite different names*

### Comparing `py-pde-0.9.3/pde/grids/operators/cartesian.py` & `py-pde-0.9.4/pde/grids/operators/cartesian.py`

 * *Files identical despite different names*

### Comparing `py-pde-0.9.3/pde/grids/operators/common.py` & `py-pde-0.9.4/pde/grids/operators/common.py`

 * *Files identical despite different names*

### Comparing `py-pde-0.9.3/pde/grids/operators/cylindrical.py` & `py-pde-0.9.4/pde/grids/operators/cylindrical.py`

 * *Files identical despite different names*

### Comparing `py-pde-0.9.3/pde/grids/operators/polar.py` & `py-pde-0.9.4/pde/grids/operators/polar.py`

 * *Files identical despite different names*

### Comparing `py-pde-0.9.3/pde/grids/operators/spherical.py` & `py-pde-0.9.4/pde/grids/operators/spherical.py`

 * *Files identical despite different names*

### Comparing `py-pde-0.9.3/pde/grids/operators/tests/test_cartesian.py` & `py-pde-0.9.4/pde/grids/operators/tests/test_cartesian.py`

 * *Files identical despite different names*

### Comparing `py-pde-0.9.3/pde/grids/operators/tests/test_cylindrical.py` & `py-pde-0.9.4/pde/grids/operators/tests/test_cylindrical.py`

 * *Files identical despite different names*

### Comparing `py-pde-0.9.3/pde/grids/operators/tests/test_polar.py` & `py-pde-0.9.4/pde/grids/operators/tests/test_polar.py`

 * *Files identical despite different names*

### Comparing `py-pde-0.9.3/pde/grids/operators/tests/test_spherical.py` & `py-pde-0.9.4/pde/grids/operators/tests/test_spherical.py`

 * *Files identical despite different names*

### Comparing `py-pde-0.9.3/pde/grids/spherical.py` & `py-pde-0.9.4/pde/grids/spherical.py`

 * *Files identical despite different names*

### Comparing `py-pde-0.9.3/pde/grids/tests/test_cartesian.py` & `py-pde-0.9.4/pde/grids/tests/test_cartesian.py`

 * *Files identical despite different names*

### Comparing `py-pde-0.9.3/pde/grids/tests/test_cylindrical.py` & `py-pde-0.9.4/pde/grids/tests/test_cylindrical.py`

 * *Files identical despite different names*

### Comparing `py-pde-0.9.3/pde/grids/tests/test_generic.py` & `py-pde-0.9.4/pde/grids/tests/test_generic.py`

 * *Files 4% similar despite different names*

```diff
@@ -90,15 +90,17 @@
         assert grid.cell_to_point(p_emtpy).size == 0
 
 
 def test_integration():
     """ test integration of fields """
     for grid in iter_grids():
         arr = np.random.randn(*grid.shape)
-        assert grid.make_integrator()(arr) == pytest.approx(grid.integrate(arr))
+        res = grid.make_integrator()(arr)
+        assert np.isscalar(res)
+        assert res == pytest.approx(grid.integrate(arr))
 
 
 @skipUnlessModule("matplotlib")
 def test_grid_plotting():
     """ test plotting of grids """
     grids.UnitGrid([4]).plot()
     grids.UnitGrid([4, 4]).plot()
```

### Comparing `py-pde-0.9.3/pde/grids/tests/test_spherical.py` & `py-pde-0.9.4/pde/grids/tests/test_spherical.py`

 * *Files identical despite different names*

### Comparing `py-pde-0.9.3/pde/pdes/__init__.py` & `py-pde-0.9.4/pde/pdes/__init__.py`

 * *Files identical despite different names*

### Comparing `py-pde-0.9.3/pde/pdes/allen_cahn.py` & `py-pde-0.9.4/pde/pdes/allen_cahn.py`

 * *Files identical despite different names*

### Comparing `py-pde-0.9.3/pde/pdes/base.py` & `py-pde-0.9.4/pde/pdes/base.py`

 * *Files identical despite different names*

### Comparing `py-pde-0.9.3/pde/pdes/cahn_hilliard.py` & `py-pde-0.9.4/pde/pdes/cahn_hilliard.py`

 * *Files identical despite different names*

### Comparing `py-pde-0.9.3/pde/pdes/diffusion.py` & `py-pde-0.9.4/pde/pdes/diffusion.py`

 * *Files identical despite different names*

### Comparing `py-pde-0.9.3/pde/pdes/kpz_interface.py` & `py-pde-0.9.4/pde/pdes/kpz_interface.py`

 * *Files identical despite different names*

### Comparing `py-pde-0.9.3/pde/pdes/kuramoto_sivashinsky.py` & `py-pde-0.9.4/pde/pdes/kuramoto_sivashinsky.py`

 * *Files identical despite different names*

### Comparing `py-pde-0.9.3/pde/pdes/laplace.py` & `py-pde-0.9.4/pde/pdes/laplace.py`

 * *Files identical despite different names*

### Comparing `py-pde-0.9.3/pde/pdes/pde.py` & `py-pde-0.9.4/pde/pdes/pde.py`

 * *Files identical despite different names*

### Comparing `py-pde-0.9.3/pde/pdes/swift_hohenberg.py` & `py-pde-0.9.4/pde/pdes/swift_hohenberg.py`

 * *Files identical despite different names*

### Comparing `py-pde-0.9.3/pde/pdes/tests/test_diffusion.py` & `py-pde-0.9.4/pde/pdes/tests/test_diffusion.py`

 * *Files identical despite different names*

### Comparing `py-pde-0.9.3/pde/pdes/tests/test_generic.py` & `py-pde-0.9.4/pde/pdes/tests/test_generic.py`

 * *Files identical despite different names*

### Comparing `py-pde-0.9.3/pde/pdes/tests/test_laplace.py` & `py-pde-0.9.4/pde/pdes/tests/test_laplace.py`

 * *Files identical despite different names*

### Comparing `py-pde-0.9.3/pde/pdes/tests/test_pde.py` & `py-pde-0.9.4/pde/pdes/tests/test_pde.py`

 * *Files identical despite different names*

### Comparing `py-pde-0.9.3/pde/pdes/tests/test_wave.py` & `py-pde-0.9.4/pde/pdes/tests/test_wave.py`

 * *Files identical despite different names*

### Comparing `py-pde-0.9.3/pde/pdes/wave.py` & `py-pde-0.9.4/pde/pdes/wave.py`

 * *Files identical despite different names*

### Comparing `py-pde-0.9.3/pde/solvers/__init__.py` & `py-pde-0.9.4/pde/solvers/__init__.py`

 * *Files identical despite different names*

### Comparing `py-pde-0.9.3/pde/solvers/base.py` & `py-pde-0.9.4/pde/solvers/base.py`

 * *Files identical despite different names*

### Comparing `py-pde-0.9.3/pde/solvers/controller.py` & `py-pde-0.9.4/pde/solvers/controller.py`

 * *Files identical despite different names*

### Comparing `py-pde-0.9.3/pde/solvers/explicit.py` & `py-pde-0.9.4/pde/solvers/explicit.py`

 * *Files identical despite different names*

### Comparing `py-pde-0.9.3/pde/solvers/implicit.py` & `py-pde-0.9.4/pde/solvers/implicit.py`

 * *Files identical despite different names*

### Comparing `py-pde-0.9.3/pde/solvers/scipy.py` & `py-pde-0.9.4/pde/solvers/scipy.py`

 * *Files identical despite different names*

### Comparing `py-pde-0.9.3/pde/solvers/tests/test_explicit.py` & `py-pde-0.9.4/pde/solvers/tests/test_explicit.py`

 * *Files identical despite different names*

### Comparing `py-pde-0.9.3/pde/solvers/tests/test_generic.py` & `py-pde-0.9.4/pde/solvers/tests/test_generic.py`

 * *Files identical despite different names*

### Comparing `py-pde-0.9.3/pde/solvers/tests/test_scipy.py` & `py-pde-0.9.4/pde/solvers/tests/test_scipy.py`

 * *Files identical despite different names*

### Comparing `py-pde-0.9.3/pde/storage/base.py` & `py-pde-0.9.4/pde/storage/base.py`

 * *Files identical despite different names*

### Comparing `py-pde-0.9.3/pde/storage/file.py` & `py-pde-0.9.4/pde/storage/file.py`

 * *Files identical despite different names*

### Comparing `py-pde-0.9.3/pde/storage/memory.py` & `py-pde-0.9.4/pde/storage/memory.py`

 * *Files identical despite different names*

### Comparing `py-pde-0.9.3/pde/storage/tests/test_file.py` & `py-pde-0.9.4/pde/storage/tests/test_file.py`

 * *Files identical despite different names*

### Comparing `py-pde-0.9.3/pde/storage/tests/test_generic.py` & `py-pde-0.9.4/pde/storage/tests/test_generic.py`

 * *Files identical despite different names*

### Comparing `py-pde-0.9.3/pde/storage/tests/test_memory.py` & `py-pde-0.9.4/pde/storage/tests/test_memory.py`

 * *Files identical despite different names*

### Comparing `py-pde-0.9.3/pde/tests/test_examples.py` & `py-pde-0.9.4/pde/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `py-pde-0.9.3/pde/tests/test_integration.py` & `py-pde-0.9.4/pde/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `py-pde-0.9.3/pde/tools/cache.py` & `py-pde-0.9.4/pde/tools/cache.py`

 * *Files identical despite different names*

### Comparing `py-pde-0.9.3/pde/tools/cuboid.py` & `py-pde-0.9.4/pde/tools/cuboid.py`

 * *Files identical despite different names*

### Comparing `py-pde-0.9.3/pde/tools/docstrings.py` & `py-pde-0.9.4/pde/tools/docstrings.py`

 * *Files identical despite different names*

### Comparing `py-pde-0.9.3/pde/tools/expressions.py` & `py-pde-0.9.4/pde/tools/expressions.py`

 * *Files identical despite different names*

### Comparing `py-pde-0.9.3/pde/tools/math.py` & `py-pde-0.9.4/pde/tools/math.py`

 * *Files identical despite different names*

### Comparing `py-pde-0.9.3/pde/tools/misc.py` & `py-pde-0.9.4/pde/tools/misc.py`

 * *Files identical despite different names*

### Comparing `py-pde-0.9.3/pde/tools/numba.py` & `py-pde-0.9.4/pde/tools/numba.py`

 * *Files identical despite different names*

### Comparing `py-pde-0.9.3/pde/tools/output.py` & `py-pde-0.9.4/pde/tools/output.py`

 * *Files identical despite different names*

### Comparing `py-pde-0.9.3/pde/tools/parameters.py` & `py-pde-0.9.4/pde/tools/parameters.py`

 * *Files identical despite different names*

### Comparing `py-pde-0.9.3/pde/tools/parse_duration.py` & `py-pde-0.9.4/pde/tools/parse_duration.py`

 * *Files identical despite different names*

### Comparing `py-pde-0.9.3/pde/tools/plotting.py` & `py-pde-0.9.4/pde/tools/plotting.py`

 * *Files identical despite different names*

### Comparing `py-pde-0.9.3/pde/tools/spectral.py` & `py-pde-0.9.4/pde/tools/spectral.py`

 * *Files identical despite different names*

### Comparing `py-pde-0.9.3/pde/tools/spherical.py` & `py-pde-0.9.4/pde/tools/spherical.py`

 * *Files identical despite different names*

### Comparing `py-pde-0.9.3/pde/tools/tests/test_cache.py` & `py-pde-0.9.4/pde/tools/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `py-pde-0.9.3/pde/tools/tests/test_cuboid.py` & `py-pde-0.9.4/pde/tools/tests/test_cuboid.py`

 * *Files identical despite different names*

### Comparing `py-pde-0.9.3/pde/tools/tests/test_expressions.py` & `py-pde-0.9.4/pde/tools/tests/test_expressions.py`

 * *Files identical despite different names*

### Comparing `py-pde-0.9.3/pde/tools/tests/test_misc.py` & `py-pde-0.9.4/pde/tools/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `py-pde-0.9.3/pde/tools/tests/test_numba.py` & `py-pde-0.9.4/pde/tools/tests/test_numba.py`

 * *Files identical despite different names*

### Comparing `py-pde-0.9.3/pde/tools/tests/test_output.py` & `py-pde-0.9.4/pde/tools/tests/test_output.py`

 * *Files identical despite different names*

### Comparing `py-pde-0.9.3/pde/tools/tests/test_parameters.py` & `py-pde-0.9.4/pde/tools/tests/test_parameters.py`

 * *Files identical despite different names*

### Comparing `py-pde-0.9.3/pde/tools/tests/test_plotting.py` & `py-pde-0.9.4/pde/tools/tests/test_plotting.py`

 * *Files identical despite different names*

### Comparing `py-pde-0.9.3/pde/tools/tests/test_spectral.py` & `py-pde-0.9.4/pde/tools/tests/test_spectral.py`

 * *Files identical despite different names*

### Comparing `py-pde-0.9.3/pde/tools/tests/test_spherical.py` & `py-pde-0.9.4/pde/tools/tests/test_spherical.py`

 * *Files identical despite different names*

### Comparing `py-pde-0.9.3/pde/trackers/__init__.py` & `py-pde-0.9.4/pde/trackers/__init__.py`

 * *Files identical despite different names*

### Comparing `py-pde-0.9.3/pde/trackers/base.py` & `py-pde-0.9.4/pde/trackers/base.py`

 * *Files identical despite different names*

### Comparing `py-pde-0.9.3/pde/trackers/intervals.py` & `py-pde-0.9.4/pde/trackers/intervals.py`

 * *Files identical despite different names*

### Comparing `py-pde-0.9.3/pde/trackers/tests/test_intervals.py` & `py-pde-0.9.4/pde/trackers/tests/test_intervals.py`

 * *Files identical despite different names*

### Comparing `py-pde-0.9.3/pde/trackers/tests/test_trackers.py` & `py-pde-0.9.4/pde/trackers/tests/test_trackers.py`

 * *Files identical despite different names*

### Comparing `py-pde-0.9.3/pde/trackers/trackers.py` & `py-pde-0.9.4/pde/trackers/trackers.py`

 * *Files identical despite different names*

### Comparing `py-pde-0.9.3/pde/visualization/movies.py` & `py-pde-0.9.4/pde/visualization/movies.py`

 * *Files identical despite different names*

### Comparing `py-pde-0.9.3/pde/visualization/plotting.py` & `py-pde-0.9.4/pde/visualization/plotting.py`

 * *Files identical despite different names*

### Comparing `py-pde-0.9.3/pde/visualization/tests/test_movies.py` & `py-pde-0.9.4/pde/visualization/tests/test_movies.py`

 * *Files identical despite different names*

### Comparing `py-pde-0.9.3/pde/visualization/tests/test_plotting.py` & `py-pde-0.9.4/pde/visualization/tests/test_plotting.py`

 * *Files identical despite different names*

### Comparing `py-pde-0.9.3/py_pde.egg-info/PKG-INFO` & `py-pde-0.9.4/py_pde.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: py-pde
-Version: 0.9.3
+Version: 0.9.4
 Summary: Python package for solving partial differential equations
 Home-page: https://github.com/zwicker-group/py-pde
 Author: David Zwicker
 Author-email: david.zwicker@ds.mpg.de
 License: MIT
-Download-URL: https://github.com/zwicker-group/py-pde/archive/v0.9.3.tar.gz
+Download-URL: https://github.com/zwicker-group/py-pde/archive/v0.9.4.tar.gz
 Description: # py-pde
         
         [![PyPI version](https://badge.fury.io/py/py-pde.svg)](https://badge.fury.io/py/py-pde)
         [![Documentation Status](https://readthedocs.org/projects/py-pde/badge/?version=latest)](https://py-pde.readthedocs.io/en/latest/?badge=latest)
         [![DOI](https://joss.theoj.org/papers/10.21105/joss.02158/status.svg)](https://doi.org/10.21105/joss.02158)
         [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/zwicker-group/py-pde/master?filepath=examples%2Fjupyter)
```

### Comparing `py-pde-0.9.3/py_pde.egg-info/SOURCES.txt` & `py-pde-0.9.4/py_pde.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py-pde-0.9.3/setup.py` & `py-pde-0.9.4/setup.py`

 * *Files identical despite different names*

