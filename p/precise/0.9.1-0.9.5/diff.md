# Comparing `tmp/precise-0.9.1.tar.gz` & `tmp/precise-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "precise-0.9.1.tar", last modified: Thu Jul 14 04:34:26 2022, max compression
+gzip compressed data, was "precise-0.9.5.tar", last modified: Mon Jul 18 15:05:55 2022, max compression
```

## Comparing `precise-0.9.1.tar` & `precise-0.9.5.tar`

### file list

```diff
@@ -1,212 +1,215 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 04:34:26.415895 precise-0.9.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1198 2022-07-14 04:34:18.000000 precise-0.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-07-14 04:34:18.000000 precise-0.9.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    15085 2022-07-14 04:34:26.415895 precise-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    14600 2022-07-14 04:34:18.000000 precise-0.9.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 04:34:26.379895 precise-0.9.1/precise/
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-07-14 04:34:18.000000 precise-0.9.1/precise/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 04:34:26.379895 precise-0.9.1/precise/skaters/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skaters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 04:34:26.387895 precise-0.9.1/precise/skaters/covariance/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skaters/covariance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3089 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skaters/covariance/allcovskaters.py
--rw-r--r--   0 runner    (1001) docker     (121)      895 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skaters/covariance/avgfactory.py
--rw-r--r--   0 runner    (1001) docker     (121)      564 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skaters/covariance/avgtop.py
--rw-r--r--   0 runner    (1001) docker     (121)     1944 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skaters/covariance/bufemp.py
--rw-r--r--   0 runner    (1001) docker     (121)      994 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skaters/covariance/bufempfactory.py
--rw-r--r--   0 runner    (1001) docker     (121)     4288 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skaters/covariance/buffactory.py
--rw-r--r--   0 runner    (1001) docker     (121)     2124 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skaters/covariance/bufhuber.py
--rw-r--r--   0 runner    (1001) docker     (121)     1012 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skaters/covariance/bufhuberfactory.py
--rw-r--r--   0 runner    (1001) docker     (121)     9420 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skaters/covariance/bufsk.py
--rw-r--r--   0 runner    (1001) docker     (121)     1704 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skaters/covariance/bufskfactory.py
--rw-r--r--   0 runner    (1001) docker     (121)     1367 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skaters/covariance/ewaemp.py
--rw-r--r--   0 runner    (1001) docker     (121)     2913 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skaters/covariance/ewaempfactory.py
--rw-r--r--   0 runner    (1001) docker     (121)     1088 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skaters/covariance/ewalw.py
--rw-r--r--   0 runner    (1001) docker     (121)     3032 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skaters/covariance/ewalwfactory.py
--rw-r--r--   0 runner    (1001) docker     (121)      756 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skaters/covariance/ewalz.py
--rw-r--r--   0 runner    (1001) docker     (121)     7545 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skaters/covariance/ewalzfactory.py
--rw-r--r--   0 runner    (1001) docker     (121)     2833 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skaters/covariance/ewapm.py
--rw-r--r--   0 runner    (1001) docker     (121)     3291 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skaters/covariance/ewapmfactory.py
--rw-r--r--   0 runner    (1001) docker     (121)      220 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skaters/covariance/identity.py
--rw-r--r--   0 runner    (1001) docker     (121)     1399 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skaters/covariance/runemp.py
--rw-r--r--   0 runner    (1001) docker     (121)     2316 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skaters/covariance/runempfactory.py
--rw-r--r--   0 runner    (1001) docker     (121)      699 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skaters/covariance/weakboot.py
--rw-r--r--   0 runner    (1001) docker     (121)     1254 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skaters/covariance/weakewa.py
--rw-r--r--   0 runner    (1001) docker     (121)     1912 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skaters/covariance/weakfactory.py
--rw-r--r--   0 runner    (1001) docker     (121)      762 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skaters/covariance/weaklz.py
--rw-r--r--   0 runner    (1001) docker     (121)      548 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skaters/covariance/weakpm.py
--rw-r--r--   0 runner    (1001) docker     (121)      898 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skaters/covariance/weaksk.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 04:34:26.387895 precise-0.9.1/precise/skaters/covarianceutil/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skaters/covarianceutil/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1015 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skaters/covarianceutil/adjacency.py
--rw-r--r--   0 runner    (1001) docker     (121)      626 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skaters/covarianceutil/conventions.py
--rw-r--r--   0 runner    (1001) docker     (121)     2281 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skaters/covarianceutil/covdecomposition.py
--rw-r--r--   0 runner    (1001) docker     (121)    12204 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skaters/covarianceutil/covfunctions.py
--rw-r--r--   0 runner    (1001) docker     (121)      616 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skaters/covarianceutil/covrandom.py
--rw-r--r--   0 runner    (1001) docker     (121)     2940 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skaters/covarianceutil/datafunctions.py
--rw-r--r--   0 runner    (1001) docker     (121)      963 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skaters/covarianceutil/datascatterfunctions.py
--rw-r--r--   0 runner    (1001) docker     (121)      549 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skaters/covarianceutil/differencing.py
--rw-r--r--   0 runner    (1001) docker     (121)     1096 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skaters/covarianceutil/hubercov.py
--rw-r--r--   0 runner    (1001) docker     (121)     4734 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skaters/covarianceutil/likelihood.py
--rw-r--r--   0 runner    (1001) docker     (121)     3680 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skaters/covarianceutil/pdutil.py
--rw-r--r--   0 runner    (1001) docker     (121)     1073 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skaters/covarianceutil/statefunctions.py
--rw-r--r--   0 runner    (1001) docker     (121)      392 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skaters/covarianceutil/statemutations.py
--rw-r--r--   0 runner    (1001) docker     (121)      145 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skaters/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 04:34:26.387895 precise-0.9.1/precise/skaters/location/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skaters/location/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1514 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skaters/location/averagingpre.py
--rw-r--r--   0 runner    (1001) docker     (121)     1362 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skaters/location/buffermedianpre.py
--rw-r--r--   0 runner    (1001) docker     (121)      891 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skaters/location/empirical.py
--rw-r--r--   0 runner    (1001) docker     (121)      230 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skaters/location/empricalpre.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 04:34:26.391895 precise-0.9.1/precise/skaters/locationutil/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skaters/locationutil/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1397 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skaters/locationutil/bisection.py
--rw-r--r--   0 runner    (1001) docker     (121)     5164 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skaters/locationutil/hubermean.py
--rw-r--r--   0 runner    (1001) docker     (121)      713 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skaters/locationutil/vectorfunctions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 04:34:26.395895 precise-0.9.1/precise/skaters/managers/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skaters/managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2008 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skaters/managers/allmanagers.py
--rw-r--r--   0 runner    (1001) docker     (121)     2142 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skaters/managers/buyandholdfactory.py
--rw-r--r--   0 runner    (1001) docker     (121)     3415 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skaters/managers/covmanagerfactory.py
--rw-r--r--   0 runner    (1001) docker     (121)     1304 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skaters/managers/equalmanagers.py
--rw-r--r--   0 runner    (1001) docker     (121)     1564 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skaters/managers/hrpmanagers.py
--rw-r--r--   0 runner    (1001) docker     (121)     1284 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skaters/managers/ldpmanagers.py
--rw-r--r--   0 runner    (1001) docker     (121)     1716 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skaters/managers/molybogamanagers.py
--rw-r--r--   0 runner    (1001) docker     (121)     1521 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skaters/managers/ppomanagerfactory.py
--rw-r--r--   0 runner    (1001) docker     (121)     5202 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skaters/managers/ppomanagers.py
--rw-r--r--   0 runner    (1001) docker     (121)     1893 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skaters/managers/rflmanagerfactory.py
--rw-r--r--   0 runner    (1001) docker     (121)     5292 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skaters/managers/rflmanagers.py
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skaters/managers/rpmanagerfactory.py
--rw-r--r--   0 runner    (1001) docker     (121)     3487 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skaters/managers/rpmanagers.py
--rw-r--r--   0 runner    (1001) docker     (121)    12413 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skaters/managers/schurmanagerfactory.py
--rw-r--r--   0 runner    (1001) docker     (121)    17870 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skaters/managers/schurmanagers.py
--rw-r--r--   0 runner    (1001) docker     (121)     1459 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skaters/managers/weakmanagerfactory.py
--rw-r--r--   0 runner    (1001) docker     (121)     4553 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skaters/managers/weakmanagers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 04:34:26.399895 precise-0.9.1/precise/skaters/managerutil/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skaters/managerutil/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2153 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skaters/managerutil/managerstats.py
--rw-r--r--   0 runner    (1001) docker     (121)     1954 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skaters/managerutil/managertesting.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 04:34:26.407895 precise-0.9.1/precise/skaters/portfoliostatic/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skaters/portfoliostatic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      237 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skaters/portfoliostatic/allstaticalloc.py
--rw-r--r--   0 runner    (1001) docker     (121)     1265 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skaters/portfoliostatic/allstaticport.py
--rw-r--r--   0 runner    (1001) docker     (121)      219 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skaters/portfoliostatic/diagalloc.py
--rw-r--r--   0 runner    (1001) docker     (121)     1165 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skaters/portfoliostatic/diagallocfactory.py
--rw-r--r--   0 runner    (1001) docker     (121)      249 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skaters/portfoliostatic/diagport.py
--rw-r--r--   0 runner    (1001) docker     (121)     1356 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skaters/portfoliostatic/diagportfactory.py
--rw-r--r--   0 runner    (1001) docker     (121)      788 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skaters/portfoliostatic/equalport.py
--rw-r--r--   0 runner    (1001) docker     (121)     2512 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skaters/portfoliostatic/hrpport.py
--rw-r--r--   0 runner    (1001) docker     (121)      559 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skaters/portfoliostatic/hrpportfactory.py
--rw-r--r--   0 runner    (1001) docker     (121)      346 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skaters/portfoliostatic/porttesting.py
--rw-r--r--   0 runner    (1001) docker     (121)     1464 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skaters/portfoliostatic/ppoport.py
--rw-r--r--   0 runner    (1001) docker     (121)     6397 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skaters/portfoliostatic/ppoportfactory.py
--rw-r--r--   0 runner    (1001) docker     (121)     1408 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skaters/portfoliostatic/rpport.py
--rw-r--r--   0 runner    (1001) docker     (121)      712 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skaters/portfoliostatic/rpportfactory.py
--rw-r--r--   0 runner    (1001) docker     (121)     3130 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skaters/portfoliostatic/schurport.py
--rw-r--r--   0 runner    (1001) docker     (121)     9513 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skaters/portfoliostatic/schurportfactory.py
--rw-r--r--   0 runner    (1001) docker     (121)     1177 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skaters/portfoliostatic/schurportutil.py
--rw-r--r--   0 runner    (1001) docker     (121)      230 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skaters/portfoliostatic/unitalloc.py
--rw-r--r--   0 runner    (1001) docker     (121)     1043 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skaters/portfoliostatic/unitallocfactory.py
--rw-r--r--   0 runner    (1001) docker     (121)      262 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skaters/portfoliostatic/unitport.py
--rw-r--r--   0 runner    (1001) docker     (121)     1643 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skaters/portfoliostatic/unitportfactory.py
--rw-r--r--   0 runner    (1001) docker     (121)      205 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skaters/portfoliostatic/volalloc.py
--rw-r--r--   0 runner    (1001) docker     (121)     1210 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skaters/portfoliostatic/volallocfactory.py
--rw-r--r--   0 runner    (1001) docker     (121)      517 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skaters/portfoliostatic/weakalloc.py
--rw-r--r--   0 runner    (1001) docker     (121)     1223 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skaters/portfoliostatic/weakallocfactory.py
--rw-r--r--   0 runner    (1001) docker     (121)     1616 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skaters/portfoliostatic/weakport.py
--rw-r--r--   0 runner    (1001) docker     (121)     4248 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skaters/portfoliostatic/weakportfactory.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 04:34:26.407895 precise-0.9.1/precise/skaters/portfolioutil/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skaters/portfolioutil/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6585 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skaters/portfolioutil/portcomparison.py
--rw-r--r--   0 runner    (1001) docker     (121)     3350 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skaters/portfolioutil/portfunctions.py
--rw-r--r--   0 runner    (1001) docker     (121)      977 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skaters/portfolioutil/portsuggestion.py
--rw-r--r--   0 runner    (1001) docker     (121)        3 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skaters/portfolioutil/seriation.py
--rw-r--r--   0 runner    (1001) docker     (121)      715 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skaters/portfolioutil/unitlemmas.py
--rw-r--r--   0 runner    (1001) docker     (121)     3372 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skaters/portfolioutil/unittransforms.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 04:34:26.411895 precise-0.9.1/precise/skaters/scalarutil/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skaters/scalarutil/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1402 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skaters/scalarutil/runningmedian.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 04:34:26.411895 precise-0.9.1/precise/skatertools/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skatertools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 04:34:26.411895 precise-0.9.1/precise/skatertools/data/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skatertools/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1705 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skatertools/data/equityhistorical.py
--rw-r--r--   0 runner    (1001) docker     (121)     5107 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skatertools/data/equitylive.py
--rw-r--r--   0 runner    (1001) docker     (121)     2793 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skatertools/data/etflists.py
--rw-r--r--   0 runner    (1001) docker     (121)     2082 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skatertools/data/skaterresiduals.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 04:34:26.411895 precise-0.9.1/precise/skatertools/ensembling/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skatertools/ensembling/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 04:34:26.411895 precise-0.9.1/precise/skatertools/m6/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skatertools/m6/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3897 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skatertools/m6/competition.py
--rw-r--r--   0 runner    (1001) docker     (121)     1837 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skatertools/m6/covarianceforecasting.py
--rw-r--r--   0 runner    (1001) docker     (121)     1697 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skatertools/m6/quintileprobabilities.py
--rw-r--r--   0 runner    (1001) docker     (121)      807 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skatertools/m6/tilting.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 04:34:26.411895 precise-0.9.1/precise/skatertools/syntheticdata/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skatertools/syntheticdata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1167 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skatertools/syntheticdata/factor.py
--rw-r--r--   0 runner    (1001) docker     (121)      469 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skatertools/syntheticdata/miscellaneous.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 04:34:26.411895 precise-0.9.1/precise/skatervaluation/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skatervaluation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 04:34:26.411895 precise-0.9.1/precise/skatervaluation/battlelatex/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skatervaluation/battlelatex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4009 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skatervaluation/battlelatex/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 04:34:26.411895 precise-0.9.1/precise/skatervaluation/battlescripts/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skatervaluation/battlescripts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 04:34:26.411895 precise-0.9.1/precise/skatervaluation/battlescripts/cov_likelihood/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skatervaluation/battlescripts/cov_likelihood/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      304 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skatervaluation/battlescripts/cov_likelihood/m6?topic=m6&n_dim=int:100&n_obs=int:225&n_burn=int:200&interval=d&etf=int:1&implied=int:1.py
--rw-r--r--   0 runner    (1001) docker     (121)      304 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skatervaluation/battlescripts/cov_likelihood/m6?topic=m6&n_dim=int:100&n_obs=int:225&n_burn=int:200&interval=d&etf=int:1.py
--rw-r--r--   0 runner    (1001) docker     (121)      304 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skatervaluation/battlescripts/cov_likelihood/m6?topic=m6&n_dim=int:20&n_obs=int:36&n_burn=int:24&interval=m&etf=int:-1.py
--rw-r--r--   0 runner    (1001) docker     (121)      304 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skatervaluation/battlescripts/cov_likelihood/m6?topic=m6&n_dim=int:5&n_obs=int:356&n_burn=int:300&interval=d&etf=int:0.py
--rw-r--r--   0 runner    (1001) docker     (121)      304 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skatervaluation/battlescripts/cov_likelihood/stocks?topic=stocks&n_dim=int:199&n_obs=int:60&n_burn=int:50&k=20.py
--rw-r--r--   0 runner    (1001) docker     (121)      304 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skatervaluation/battlescripts/cov_likelihood/stocks?topic=stocks&n_dim=int:25&n_obs=int:30&n_burn=int:20&k=5.py
--rw-r--r--   0 runner    (1001) docker     (121)      304 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skatervaluation/battlescripts/cov_likelihood/stocks?topic=stocks&n_dim=int:499&n_obs=int:60&n_burn=int:50&k=5.py
--rw-r--r--   0 runner    (1001) docker     (121)      304 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skatervaluation/battlescripts/cov_likelihood/stocks?topic=stocks&n_dim=int:50&n_obs=int:200&n_burn=int:150&k=5.py
--rw-r--r--   0 runner    (1001) docker     (121)      304 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skatervaluation/battlescripts/cov_likelihood/stocks?topic=stocks&n_dim=int:500&n_obs=int:600&n_burn=int:500&k=1.py
--rw-r--r--   0 runner    (1001) docker     (121)      304 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skatervaluation/battlescripts/cov_likelihood/tm?topic=tm&n_dim=int:100&n_obs=int:250&n_burn=int:200.py
--rw-r--r--   0 runner    (1001) docker     (121)      304 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skatervaluation/battlescripts/cov_likelihood/tm?topic=tm&n_dim=int:20&n_obs=int:500&n_burn=int:400.py
--rw-r--r--   0 runner    (1001) docker     (121)      304 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skatervaluation/battlescripts/cov_likelihood/tm?topic=tm&n_dim=int:25&n_obs=int:250&n_burn=int:200.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 04:34:26.411895 precise-0.9.1/precise/skatervaluation/battlescripts/manager_info/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skatervaluation/battlescripts/manager_info/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      300 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skatervaluation/battlescripts/manager_info/stocks?topic=stocks&n_dim=int:100&n_obs=int:125&n_burn=int:100&k=int:20.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 04:34:26.411895 precise-0.9.1/precise/skatervaluation/battlescripts/manager_var/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skatervaluation/battlescripts/manager_var/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      298 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skatervaluation/battlescripts/manager_var/m6?topic=m6&n_dim=int:100&n_obs=int:225&n_burn=int:200&interval=d&etf=int:1&implied=int:1.py
--rw-r--r--   0 runner    (1001) docker     (121)      298 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skatervaluation/battlescripts/manager_var/m6?topic=m6&n_dim=int:100&n_obs=int:225&n_burn=int:200&interval=d&etf=int:1.py
--rw-r--r--   0 runner    (1001) docker     (121)      298 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skatervaluation/battlescripts/manager_var/m6?topic=m6&n_dim=int:25&n_obs=int:200&n_burn=int:100&interval=d&etf=int:0.py
--rw-r--r--   0 runner    (1001) docker     (121)      298 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skatervaluation/battlescripts/manager_var/m6?topic=m6&n_dim=int:35&n_obs=int:356&n_burn=int:300&interval=d&etf=int:1.py
--rw-r--r--   0 runner    (1001) docker     (121)      298 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skatervaluation/battlescripts/manager_var/m6?topic=m6&n_dim=int:45&n_obs=int:60&n_burn=int:50&interval=m&etf=int:1.py
--rw-r--r--   0 runner    (1001) docker     (121)      298 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skatervaluation/battlescripts/manager_var/m6?topic=m6&n_dim=int:5&n_obs=int:356&n_burn=int:300&interval=d&etf=int:0.py
--rw-r--r--   0 runner    (1001) docker     (121)      298 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skatervaluation/battlescripts/manager_var/stocks?topic=stocks&n_dim=int:100&n_obs=int:125&n_burn=int:100&k=int:20.py
--rw-r--r--   0 runner    (1001) docker     (121)      298 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skatervaluation/battlescripts/manager_var/stocks?topic=stocks&n_dim=int:2&n_obs=int:70&n_burn=int:60&k=int:20.py
--rw-r--r--   0 runner    (1001) docker     (121)      298 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skatervaluation/battlescripts/manager_var/stocks?topic=stocks&n_dim=int:200&n_obs=int:225&n_burn=int:200&k=int:1.py
--rw-r--r--   0 runner    (1001) docker     (121)      298 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skatervaluation/battlescripts/manager_var/stocks?topic=stocks&n_dim=int:50&n_obs=int:125&n_burn=int:100&k=int:20.py
--rw-r--r--   0 runner    (1001) docker     (121)      298 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skatervaluation/battlescripts/manager_var/stocks?topic=stocks&n_dim=int:500&n_obs=int:225&n_burn=int:200&k=int:5.py
--rw-r--r--   0 runner    (1001) docker     (121)      304 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skatervaluation/battlescripts/manager_var/tm?topic=tm&n_dim=int:20&n_obs=int:450&n_burn=int:400.py
--rw-r--r--   0 runner    (1001) docker     (121)      304 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skatervaluation/battlescripts/manager_var/tm?topic=tm&n_dim=int:25&n_obs=int:250&n_burn=int:200.py
--rw-r--r--   0 runner    (1001) docker     (121)      298 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skatervaluation/battlescripts/manager_var/tm?topic=tm&n_dim=int:500&n_obs=int:250&n_burn=int:200&collinear=int:0.py
--rw-r--r--   0 runner    (1001) docker     (121)      298 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skatervaluation/battlescripts/manager_var/tm?topic=tm&n_dim=int:500&n_obs=int:250&n_burn=int:200&collinear=int:1.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 04:34:26.415895 precise-0.9.1/precise/skatervaluation/battleutil/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skatervaluation/battleutil/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5366 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skatervaluation/battleutil/arrangingbattles.py
--rw-r--r--   0 runner    (1001) docker     (121)     1281 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skatervaluation/battleutil/battleio.py
--rw-r--r--   0 runner    (1001) docker     (121)     4822 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skatervaluation/battleutil/compilingeloratings.py
--rw-r--r--   0 runner    (1001) docker     (121)      130 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skatervaluation/battleutil/createelocsv.py
--rw-r--r--   0 runner    (1001) docker     (121)        2 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skatervaluation/battleutil/datasources.py
--rw-r--r--   0 runner    (1001) docker     (121)      790 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skatervaluation/battleutil/eloformulas.py
--rw-r--r--   0 runner    (1001) docker     (121)     2248 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skatervaluation/battleutil/speed.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 04:34:26.415895 precise-0.9.1/precise/skatervaluation/queues/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-14 04:34:18.000000 precise-0.9.1/precise/skatervaluation/queues/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1276 2022-07-14 04:34:18.000000 precise-0.9.1/precise/whereami.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 04:34:26.415895 precise-0.9.1/precise/z/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-14 04:34:18.000000 precise-0.9.1/precise/z/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 04:34:26.379895 precise-0.9.1/precise.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    15085 2022-07-14 04:34:26.000000 precise-0.9.1/precise.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    10018 2022-07-14 04:34:26.000000 precise-0.9.1/precise.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-14 04:34:26.000000 precise-0.9.1/precise.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       51 2022-07-14 04:34:26.000000 precise-0.9.1/precise.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      156 2022-07-14 04:34:26.000000 precise-0.9.1/precise.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-07-14 04:34:26.000000 precise-0.9.1/precise.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-07-14 04:34:26.415895 precise-0.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2286 2022-07-14 04:34:18.000000 precise-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 15:05:55.395214 precise-0.9.5/
+-rw-r--r--   0 runner    (1001) docker     (121)     1198 2022-07-18 15:05:46.000000 precise-0.9.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-07-18 15:05:46.000000 precise-0.9.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)    15085 2022-07-18 15:05:55.395214 precise-0.9.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    14600 2022-07-18 15:05:46.000000 precise-0.9.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 15:05:55.367213 precise-0.9.5/precise/
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-07-18 15:05:46.000000 precise-0.9.5/precise/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 15:05:55.367213 precise-0.9.5/precise/skaters/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 15:05:55.371214 precise-0.9.5/precise/skaters/covariance/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/covariance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3089 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/covariance/allcovskaters.py
+-rw-r--r--   0 runner    (1001) docker     (121)      895 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/covariance/avgfactory.py
+-rw-r--r--   0 runner    (1001) docker     (121)      564 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/covariance/avgtop.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1944 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/covariance/bufemp.py
+-rw-r--r--   0 runner    (1001) docker     (121)      994 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/covariance/bufempfactory.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4288 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/covariance/buffactory.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2124 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/covariance/bufhuber.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1012 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/covariance/bufhuberfactory.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9420 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/covariance/bufsk.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1704 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/covariance/bufskfactory.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1367 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/covariance/ewaemp.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2913 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/covariance/ewaempfactory.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1088 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/covariance/ewalw.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3032 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/covariance/ewalwfactory.py
+-rw-r--r--   0 runner    (1001) docker     (121)      756 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/covariance/ewalz.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7545 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/covariance/ewalzfactory.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2833 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/covariance/ewapm.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3291 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/covariance/ewapmfactory.py
+-rw-r--r--   0 runner    (1001) docker     (121)      220 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/covariance/identity.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1399 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/covariance/runemp.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2316 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/covariance/runempfactory.py
+-rw-r--r--   0 runner    (1001) docker     (121)      699 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/covariance/weakboot.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1254 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/covariance/weakewa.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1912 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/covariance/weakfactory.py
+-rw-r--r--   0 runner    (1001) docker     (121)      762 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/covariance/weaklz.py
+-rw-r--r--   0 runner    (1001) docker     (121)      548 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/covariance/weakpm.py
+-rw-r--r--   0 runner    (1001) docker     (121)      898 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/covariance/weaksk.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 15:05:55.371214 precise-0.9.5/precise/skaters/covarianceutil/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/covarianceutil/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1015 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/covarianceutil/adjacency.py
+-rw-r--r--   0 runner    (1001) docker     (121)      626 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/covarianceutil/conventions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2281 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/covarianceutil/covdecomposition.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12222 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/covarianceutil/covfunctions.py
+-rw-r--r--   0 runner    (1001) docker     (121)      616 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/covarianceutil/covrandom.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2940 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/covarianceutil/datafunctions.py
+-rw-r--r--   0 runner    (1001) docker     (121)      963 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/covarianceutil/datascatterfunctions.py
+-rw-r--r--   0 runner    (1001) docker     (121)      549 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/covarianceutil/differencing.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1096 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/covarianceutil/hubercov.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4734 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/covarianceutil/likelihood.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3680 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/covarianceutil/pdutil.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1073 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/covarianceutil/statefunctions.py
+-rw-r--r--   0 runner    (1001) docker     (121)      392 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/covarianceutil/statemutations.py
+-rw-r--r--   0 runner    (1001) docker     (121)      145 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 15:05:55.375213 precise-0.9.5/precise/skaters/location/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/location/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1514 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/location/averagingpre.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1362 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/location/buffermedianpre.py
+-rw-r--r--   0 runner    (1001) docker     (121)      891 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/location/empirical.py
+-rw-r--r--   0 runner    (1001) docker     (121)      230 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/location/empricalpre.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 15:05:55.375213 precise-0.9.5/precise/skaters/locationutil/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/locationutil/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1397 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/locationutil/bisection.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5164 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/locationutil/hubermean.py
+-rw-r--r--   0 runner    (1001) docker     (121)      713 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/locationutil/vectorfunctions.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 15:05:55.375213 precise-0.9.5/precise/skaters/managers/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2116 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/managers/allmanagers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2142 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/managers/buyandholdfactory.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3415 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/managers/covmanagerfactory.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1304 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/managers/equalmanagers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1564 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/managers/hrpmanagers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1284 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/managers/ldpmanagers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2096 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/managers/molybogamanagerfactory.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3214 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/managers/molybogamanagers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1521 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/managers/ppomanagerfactory.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5202 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/managers/ppomanagers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1893 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/managers/rflmanagerfactory.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5292 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/managers/rflmanagers.py
+-rw-r--r--   0 runner    (1001) docker     (121)       22 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/managers/rpmanagerfactory.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3487 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/managers/rpmanagers.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12548 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/managers/schurmanagerfactory.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17870 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/managers/schurmanagers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1633 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/managers/slurpmanagerfactory.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3318 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/managers/slurpmanagers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1459 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/managers/weakmanagerfactory.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4553 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/managers/weakmanagers.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 15:05:55.379214 precise-0.9.5/precise/skaters/managerutil/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/managerutil/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2153 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/managerutil/managerstats.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1954 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/managerutil/managertesting.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 15:05:55.383214 precise-0.9.5/precise/skaters/portfoliostatic/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/portfoliostatic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      237 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/portfoliostatic/allstaticalloc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1265 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/portfoliostatic/allstaticport.py
+-rw-r--r--   0 runner    (1001) docker     (121)      219 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/portfoliostatic/diagalloc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1165 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/portfoliostatic/diagallocfactory.py
+-rw-r--r--   0 runner    (1001) docker     (121)      249 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/portfoliostatic/diagport.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1356 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/portfoliostatic/diagportfactory.py
+-rw-r--r--   0 runner    (1001) docker     (121)      788 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/portfoliostatic/equalport.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2512 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/portfoliostatic/hrpport.py
+-rw-r--r--   0 runner    (1001) docker     (121)      559 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/portfoliostatic/hrpportfactory.py
+-rw-r--r--   0 runner    (1001) docker     (121)      346 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/portfoliostatic/porttesting.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1464 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/portfoliostatic/ppoport.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6397 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/portfoliostatic/ppoportfactory.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1408 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/portfoliostatic/rpport.py
+-rw-r--r--   0 runner    (1001) docker     (121)      862 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/portfoliostatic/rpportfactory.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3130 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/portfoliostatic/schurport.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9513 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/portfoliostatic/schurportfactory.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1177 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/portfoliostatic/schurportutil.py
+-rw-r--r--   0 runner    (1001) docker     (121)      230 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/portfoliostatic/unitalloc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1043 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/portfoliostatic/unitallocfactory.py
+-rw-r--r--   0 runner    (1001) docker     (121)      262 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/portfoliostatic/unitport.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1643 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/portfoliostatic/unitportfactory.py
+-rw-r--r--   0 runner    (1001) docker     (121)      205 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/portfoliostatic/volalloc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1210 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/portfoliostatic/volallocfactory.py
+-rw-r--r--   0 runner    (1001) docker     (121)      517 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/portfoliostatic/weakalloc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1223 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/portfoliostatic/weakallocfactory.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1616 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/portfoliostatic/weakport.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4248 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/portfoliostatic/weakportfactory.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 15:05:55.383214 precise-0.9.5/precise/skaters/portfolioutil/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/portfolioutil/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6585 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/portfolioutil/portcomparison.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3350 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/portfolioutil/portfunctions.py
+-rw-r--r--   0 runner    (1001) docker     (121)      977 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/portfolioutil/portsuggestion.py
+-rw-r--r--   0 runner    (1001) docker     (121)        3 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/portfolioutil/seriation.py
+-rw-r--r--   0 runner    (1001) docker     (121)      715 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/portfolioutil/unitlemmas.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3372 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/portfolioutil/unittransforms.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 15:05:55.383214 precise-0.9.5/precise/skaters/scalarutil/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/scalarutil/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1402 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skaters/scalarutil/runningmedian.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 15:05:55.383214 precise-0.9.5/precise/skatertools/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skatertools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 15:05:55.383214 precise-0.9.5/precise/skatertools/data/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skatertools/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1705 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skatertools/data/equityhistorical.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5107 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skatertools/data/equitylive.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2793 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skatertools/data/etflists.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2082 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skatertools/data/skaterresiduals.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 15:05:55.383214 precise-0.9.5/precise/skatertools/ensembling/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skatertools/ensembling/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 15:05:55.387214 precise-0.9.5/precise/skatertools/m6/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skatertools/m6/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3897 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skatertools/m6/competition.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1837 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skatertools/m6/covarianceforecasting.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1697 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skatertools/m6/quintileprobabilities.py
+-rw-r--r--   0 runner    (1001) docker     (121)      807 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skatertools/m6/tilting.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 15:05:55.387214 precise-0.9.5/precise/skatertools/syntheticdata/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skatertools/syntheticdata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1167 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skatertools/syntheticdata/factor.py
+-rw-r--r--   0 runner    (1001) docker     (121)      469 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skatertools/syntheticdata/miscellaneous.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 15:05:55.387214 precise-0.9.5/precise/skatervaluation/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skatervaluation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 15:05:55.387214 precise-0.9.5/precise/skatervaluation/battlelatex/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skatervaluation/battlelatex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4009 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skatervaluation/battlelatex/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 15:05:55.387214 precise-0.9.5/precise/skatervaluation/battlescripts/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skatervaluation/battlescripts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 15:05:55.387214 precise-0.9.5/precise/skatervaluation/battlescripts/cov_likelihood/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skatervaluation/battlescripts/cov_likelihood/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      304 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skatervaluation/battlescripts/cov_likelihood/m6?topic=m6&n_dim=int:100&n_obs=int:225&n_burn=int:200&interval=d&etf=int:1&implied=int:1.py
+-rw-r--r--   0 runner    (1001) docker     (121)      304 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skatervaluation/battlescripts/cov_likelihood/m6?topic=m6&n_dim=int:100&n_obs=int:225&n_burn=int:200&interval=d&etf=int:1.py
+-rw-r--r--   0 runner    (1001) docker     (121)      304 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skatervaluation/battlescripts/cov_likelihood/m6?topic=m6&n_dim=int:20&n_obs=int:36&n_burn=int:24&interval=m&etf=int:-1.py
+-rw-r--r--   0 runner    (1001) docker     (121)      304 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skatervaluation/battlescripts/cov_likelihood/m6?topic=m6&n_dim=int:5&n_obs=int:356&n_burn=int:300&interval=d&etf=int:0.py
+-rw-r--r--   0 runner    (1001) docker     (121)      304 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skatervaluation/battlescripts/cov_likelihood/stocks?topic=stocks&n_dim=int:199&n_obs=int:60&n_burn=int:50&k=20.py
+-rw-r--r--   0 runner    (1001) docker     (121)      304 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skatervaluation/battlescripts/cov_likelihood/stocks?topic=stocks&n_dim=int:25&n_obs=int:30&n_burn=int:20&k=5.py
+-rw-r--r--   0 runner    (1001) docker     (121)      304 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skatervaluation/battlescripts/cov_likelihood/stocks?topic=stocks&n_dim=int:499&n_obs=int:60&n_burn=int:50&k=5.py
+-rw-r--r--   0 runner    (1001) docker     (121)      304 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skatervaluation/battlescripts/cov_likelihood/stocks?topic=stocks&n_dim=int:50&n_obs=int:200&n_burn=int:150&k=5.py
+-rw-r--r--   0 runner    (1001) docker     (121)      304 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skatervaluation/battlescripts/cov_likelihood/stocks?topic=stocks&n_dim=int:500&n_obs=int:600&n_burn=int:500&k=1.py
+-rw-r--r--   0 runner    (1001) docker     (121)      304 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skatervaluation/battlescripts/cov_likelihood/tm?topic=tm&n_dim=int:100&n_obs=int:250&n_burn=int:200.py
+-rw-r--r--   0 runner    (1001) docker     (121)      304 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skatervaluation/battlescripts/cov_likelihood/tm?topic=tm&n_dim=int:20&n_obs=int:500&n_burn=int:400.py
+-rw-r--r--   0 runner    (1001) docker     (121)      304 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skatervaluation/battlescripts/cov_likelihood/tm?topic=tm&n_dim=int:25&n_obs=int:250&n_burn=int:200.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 15:05:55.387214 precise-0.9.5/precise/skatervaluation/battlescripts/manager_info/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skatervaluation/battlescripts/manager_info/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      300 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skatervaluation/battlescripts/manager_info/stocks?topic=stocks&n_dim=int:100&n_obs=int:125&n_burn=int:100&k=int:20.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 15:05:55.391214 precise-0.9.5/precise/skatervaluation/battlescripts/manager_var/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skatervaluation/battlescripts/manager_var/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      298 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skatervaluation/battlescripts/manager_var/m6?topic=m6&n_dim=int:100&n_obs=int:225&n_burn=int:200&interval=d&etf=int:1&implied=int:1.py
+-rw-r--r--   0 runner    (1001) docker     (121)      298 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skatervaluation/battlescripts/manager_var/m6?topic=m6&n_dim=int:100&n_obs=int:225&n_burn=int:200&interval=d&etf=int:1.py
+-rw-r--r--   0 runner    (1001) docker     (121)      298 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skatervaluation/battlescripts/manager_var/m6?topic=m6&n_dim=int:25&n_obs=int:200&n_burn=int:100&interval=d&etf=int:0.py
+-rw-r--r--   0 runner    (1001) docker     (121)      298 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skatervaluation/battlescripts/manager_var/m6?topic=m6&n_dim=int:35&n_obs=int:356&n_burn=int:300&interval=d&etf=int:1.py
+-rw-r--r--   0 runner    (1001) docker     (121)      298 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skatervaluation/battlescripts/manager_var/m6?topic=m6&n_dim=int:45&n_obs=int:60&n_burn=int:50&interval=m&etf=int:1.py
+-rw-r--r--   0 runner    (1001) docker     (121)      298 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skatervaluation/battlescripts/manager_var/m6?topic=m6&n_dim=int:5&n_obs=int:356&n_burn=int:300&interval=d&etf=int:0.py
+-rw-r--r--   0 runner    (1001) docker     (121)      298 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skatervaluation/battlescripts/manager_var/stocks?topic=stocks&n_dim=int:100&n_obs=int:125&n_burn=int:100&k=int:20.py
+-rw-r--r--   0 runner    (1001) docker     (121)      298 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skatervaluation/battlescripts/manager_var/stocks?topic=stocks&n_dim=int:2&n_obs=int:70&n_burn=int:60&k=int:20.py
+-rw-r--r--   0 runner    (1001) docker     (121)      298 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skatervaluation/battlescripts/manager_var/stocks?topic=stocks&n_dim=int:200&n_obs=int:225&n_burn=int:200&k=int:1.py
+-rw-r--r--   0 runner    (1001) docker     (121)      298 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skatervaluation/battlescripts/manager_var/stocks?topic=stocks&n_dim=int:50&n_obs=int:125&n_burn=int:100&k=int:20.py
+-rw-r--r--   0 runner    (1001) docker     (121)      298 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skatervaluation/battlescripts/manager_var/stocks?topic=stocks&n_dim=int:500&n_obs=int:225&n_burn=int:200&k=int:5.py
+-rw-r--r--   0 runner    (1001) docker     (121)      304 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skatervaluation/battlescripts/manager_var/tm?topic=tm&n_dim=int:20&n_obs=int:450&n_burn=int:400.py
+-rw-r--r--   0 runner    (1001) docker     (121)      304 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skatervaluation/battlescripts/manager_var/tm?topic=tm&n_dim=int:25&n_obs=int:250&n_burn=int:200.py
+-rw-r--r--   0 runner    (1001) docker     (121)      298 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skatervaluation/battlescripts/manager_var/tm?topic=tm&n_dim=int:500&n_obs=int:250&n_burn=int:200&collinear=int:0.py
+-rw-r--r--   0 runner    (1001) docker     (121)      298 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skatervaluation/battlescripts/manager_var/tm?topic=tm&n_dim=int:500&n_obs=int:250&n_burn=int:200&collinear=int:1.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 15:05:55.395214 precise-0.9.5/precise/skatervaluation/battleutil/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skatervaluation/battleutil/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5366 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skatervaluation/battleutil/arrangingbattles.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1281 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skatervaluation/battleutil/battleio.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4822 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skatervaluation/battleutil/compilingeloratings.py
+-rw-r--r--   0 runner    (1001) docker     (121)      130 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skatervaluation/battleutil/createelocsv.py
+-rw-r--r--   0 runner    (1001) docker     (121)        2 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skatervaluation/battleutil/datasources.py
+-rw-r--r--   0 runner    (1001) docker     (121)      790 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skatervaluation/battleutil/eloformulas.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2248 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skatervaluation/battleutil/speed.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 15:05:55.395214 precise-0.9.5/precise/skatervaluation/queues/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-18 15:05:46.000000 precise-0.9.5/precise/skatervaluation/queues/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1276 2022-07-18 15:05:46.000000 precise-0.9.5/precise/whereami.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 15:05:55.395214 precise-0.9.5/precise/z/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-18 15:05:46.000000 precise-0.9.5/precise/z/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-18 15:05:55.367213 precise-0.9.5/precise.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    15085 2022-07-18 15:05:55.000000 precise-0.9.5/precise.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    10159 2022-07-18 15:05:55.000000 precise-0.9.5/precise.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-18 15:05:55.000000 precise-0.9.5/precise.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       51 2022-07-18 15:05:55.000000 precise-0.9.5/precise.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      156 2022-07-18 15:05:55.000000 precise-0.9.5/precise.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        8 2022-07-18 15:05:55.000000 precise-0.9.5/precise.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-07-18 15:05:55.395214 precise-0.9.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2286 2022-07-18 15:05:46.000000 precise-0.9.5/setup.py
```

### Comparing `precise-0.9.1/LICENSE` & `precise-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `precise-0.9.1/PKG-INFO` & `precise-0.9.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: precise
-Version: 0.9.1
+Version: 0.9.5
 Summary: Online covariance, precision, portfolios and ensembles
 Home-page: https://github.com/microprediction/precise
 Author: microprediction
 Author-email: peter.cotton@microprediction.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `precise-0.9.1/README.md` & `precise-0.9.5/README.md`

 * *Files identical despite different names*

### Comparing `precise-0.9.1/precise/skaters/covariance/allcovskaters.py` & `precise-0.9.5/precise/skaters/covariance/allcovskaters.py`

 * *Files identical despite different names*

### Comparing `precise-0.9.1/precise/skaters/covariance/avgfactory.py` & `precise-0.9.5/precise/skaters/covariance/avgfactory.py`

 * *Files identical despite different names*

### Comparing `precise-0.9.1/precise/skaters/covariance/avgtop.py` & `precise-0.9.5/precise/skaters/covariance/avgtop.py`

 * *Files identical despite different names*

### Comparing `precise-0.9.1/precise/skaters/covariance/bufemp.py` & `precise-0.9.5/precise/skaters/covariance/bufemp.py`

 * *Files identical despite different names*

### Comparing `precise-0.9.1/precise/skaters/covariance/bufempfactory.py` & `precise-0.9.5/precise/skaters/covariance/bufempfactory.py`

 * *Files identical despite different names*

### Comparing `precise-0.9.1/precise/skaters/covariance/buffactory.py` & `precise-0.9.5/precise/skaters/covariance/buffactory.py`

 * *Files identical despite different names*

### Comparing `precise-0.9.1/precise/skaters/covariance/bufhuber.py` & `precise-0.9.5/precise/skaters/covariance/bufhuber.py`

 * *Files identical despite different names*

### Comparing `precise-0.9.1/precise/skaters/covariance/bufhuberfactory.py` & `precise-0.9.5/precise/skaters/covariance/bufhuberfactory.py`

 * *Files identical despite different names*

### Comparing `precise-0.9.1/precise/skaters/covariance/bufsk.py` & `precise-0.9.5/precise/skaters/covariance/bufsk.py`

 * *Files identical despite different names*

### Comparing `precise-0.9.1/precise/skaters/covariance/bufskfactory.py` & `precise-0.9.5/precise/skaters/covariance/bufskfactory.py`

 * *Files identical despite different names*

### Comparing `precise-0.9.1/precise/skaters/covariance/ewaemp.py` & `precise-0.9.5/precise/skaters/covariance/ewaemp.py`

 * *Files identical despite different names*

### Comparing `precise-0.9.1/precise/skaters/covariance/ewaempfactory.py` & `precise-0.9.5/precise/skaters/covariance/ewaempfactory.py`

 * *Files identical despite different names*

### Comparing `precise-0.9.1/precise/skaters/covariance/ewalw.py` & `precise-0.9.5/precise/skaters/covariance/ewalw.py`

 * *Files identical despite different names*

### Comparing `precise-0.9.1/precise/skaters/covariance/ewalwfactory.py` & `precise-0.9.5/precise/skaters/covariance/ewalwfactory.py`

 * *Files identical despite different names*

### Comparing `precise-0.9.1/precise/skaters/covariance/ewalz.py` & `precise-0.9.5/precise/skaters/covariance/ewalz.py`

 * *Files identical despite different names*

### Comparing `precise-0.9.1/precise/skaters/covariance/ewalzfactory.py` & `precise-0.9.5/precise/skaters/covariance/ewalzfactory.py`

 * *Files identical despite different names*

### Comparing `precise-0.9.1/precise/skaters/covariance/ewapm.py` & `precise-0.9.5/precise/skaters/covariance/ewapm.py`

 * *Files identical despite different names*

### Comparing `precise-0.9.1/precise/skaters/covariance/ewapmfactory.py` & `precise-0.9.5/precise/skaters/covariance/ewapmfactory.py`

 * *Files identical despite different names*

### Comparing `precise-0.9.1/precise/skaters/covariance/runemp.py` & `precise-0.9.5/precise/skaters/covariance/runemp.py`

 * *Files identical despite different names*

### Comparing `precise-0.9.1/precise/skaters/covariance/runempfactory.py` & `precise-0.9.5/precise/skaters/covariance/runempfactory.py`

 * *Files identical despite different names*

### Comparing `precise-0.9.1/precise/skaters/covariance/weakboot.py` & `precise-0.9.5/precise/skaters/covariance/weakboot.py`

 * *Files identical despite different names*

### Comparing `precise-0.9.1/precise/skaters/covariance/weakewa.py` & `precise-0.9.5/precise/skaters/covariance/weakewa.py`

 * *Files identical despite different names*

### Comparing `precise-0.9.1/precise/skaters/covariance/weakfactory.py` & `precise-0.9.5/precise/skaters/covariance/weakfactory.py`

 * *Files identical despite different names*

### Comparing `precise-0.9.1/precise/skaters/covariance/weaklz.py` & `precise-0.9.5/precise/skaters/covariance/weaklz.py`

 * *Files identical despite different names*

### Comparing `precise-0.9.1/precise/skaters/covariance/weakpm.py` & `precise-0.9.5/precise/skaters/covariance/weakpm.py`

 * *Files identical despite different names*

### Comparing `precise-0.9.1/precise/skaters/covariance/weaksk.py` & `precise-0.9.5/precise/skaters/covariance/weaksk.py`

 * *Files identical despite different names*

### Comparing `precise-0.9.1/precise/skaters/covarianceutil/adjacency.py` & `precise-0.9.5/precise/skaters/covarianceutil/adjacency.py`

 * *Files identical despite different names*

### Comparing `precise-0.9.1/precise/skaters/covarianceutil/conventions.py` & `precise-0.9.5/precise/skaters/covarianceutil/conventions.py`

 * *Files identical despite different names*

### Comparing `precise-0.9.1/precise/skaters/covarianceutil/covdecomposition.py` & `precise-0.9.5/precise/skaters/covarianceutil/covdecomposition.py`

 * *Files identical despite different names*

### Comparing `precise-0.9.1/precise/skaters/covarianceutil/covfunctions.py` & `precise-0.9.5/precise/skaters/covarianceutil/covfunctions.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,19 +4,32 @@
 from precise.skaters.covarianceutil.pdutil import square_to_square_dataframe, square_to_column_series, square_to_index_series
 from scipy.cluster.hierarchy import linkage, leaves_list
 from scipy.spatial.distance import squareform
 
 # Functions acting on cov, corrcoef matrices and other square matrices
 # If square pd.DataFrame are supplied instead, index and columns are preserved
 
+def is_symmetric(a, rtol=1e-05, atol=1e-08):
+    if isinstance(a, pd.DataFrame):
+        return is_symmetric(a.values, rtol=rtol, atol=atol)
+    else:
+        return np.allclose(a, a.T, rtol=rtol, atol=atol)
+
+
+def to_symmetric(a):
+    if isinstance(a, pd.DataFrame):
+        return square_to_square_dataframe(a, to_symmetric)
+    else:
+        return (a + a.T) / 2.0
+
 
 def seriation(cov, d=None):
     if d is None:
         d = cov_distance(cov=cov)
-    d_square = squareform(d)
+    d_square = to_symmetric( squareform(d) )
     clusters = linkage(d_square, method='single',optimal_ordering=True)
     return leaves_list(clusters)
 
 
 def cov_to_corrcoef(a):
     if isinstance(a, pd.DataFrame):
         return square_to_square_dataframe(a, cov_to_corrcoef)
@@ -120,26 +133,15 @@
         return square_to_square_dataframe(a, affine_shrink, phi=phi, lmbd=lmbd)
     else:
         ridge_cov = multiply_diag(a, phi=phi, copy=copy)
         shrunk_cov = grand_shrink(ridge_cov, lmbd=lmbd, copy=copy)
         return shrunk_cov
 
 
-def is_symmetric(a, rtol=1e-05, atol=1e-08):
-    if isinstance(a, pd.DataFrame):
-        return is_symmetric(a.values, rtol=rtol, atol=atol)
-    else:
-        return np.allclose(a, a.T, rtol=rtol, atol=atol)
-
 
-def to_symmetric(a):
-    if isinstance(a, pd.DataFrame):
-        return square_to_square_dataframe(a, to_symmetric)
-    else:
-        return (a + a.T) / 2.0
 
 
 def dense_weights_from_dict(d:dict, shape=None, n_dim:int=None):
     """ Convert {1:3.141,0:123} -> [ 123, 3.141 ]
     :param d: Dictionary whose keys should be 0..n
     :param shape:
     :param n_dim:
```

### Comparing `precise-0.9.1/precise/skaters/covarianceutil/covrandom.py` & `precise-0.9.5/precise/skaters/covarianceutil/covrandom.py`

 * *Files identical despite different names*

### Comparing `precise-0.9.1/precise/skaters/covarianceutil/datafunctions.py` & `precise-0.9.5/precise/skaters/covarianceutil/datafunctions.py`

 * *Files identical despite different names*

### Comparing `precise-0.9.1/precise/skaters/covarianceutil/datascatterfunctions.py` & `precise-0.9.5/precise/skaters/covarianceutil/datascatterfunctions.py`

 * *Files identical despite different names*

### Comparing `precise-0.9.1/precise/skaters/covarianceutil/differencing.py` & `precise-0.9.5/precise/skaters/covarianceutil/differencing.py`

 * *Files identical despite different names*

### Comparing `precise-0.9.1/precise/skaters/covarianceutil/hubercov.py` & `precise-0.9.5/precise/skaters/covarianceutil/hubercov.py`

 * *Files identical despite different names*

### Comparing `precise-0.9.1/precise/skaters/covarianceutil/likelihood.py` & `precise-0.9.5/precise/skaters/covarianceutil/likelihood.py`

 * *Files identical despite different names*

### Comparing `precise-0.9.1/precise/skaters/covarianceutil/pdutil.py` & `precise-0.9.5/precise/skaters/covarianceutil/pdutil.py`

 * *Files identical despite different names*

### Comparing `precise-0.9.1/precise/skaters/covarianceutil/statefunctions.py` & `precise-0.9.5/precise/skaters/covarianceutil/statefunctions.py`

 * *Files identical despite different names*

### Comparing `precise-0.9.1/precise/skaters/location/averagingpre.py` & `precise-0.9.5/precise/skaters/location/averagingpre.py`

 * *Files identical despite different names*

### Comparing `precise-0.9.1/precise/skaters/location/buffermedianpre.py` & `precise-0.9.5/precise/skaters/location/buffermedianpre.py`

 * *Files identical despite different names*

### Comparing `precise-0.9.1/precise/skaters/location/empirical.py` & `precise-0.9.5/precise/skaters/location/empirical.py`

 * *Files identical despite different names*

### Comparing `precise-0.9.1/precise/skaters/locationutil/bisection.py` & `precise-0.9.5/precise/skaters/locationutil/bisection.py`

 * *Files identical despite different names*

### Comparing `precise-0.9.1/precise/skaters/locationutil/hubermean.py` & `precise-0.9.5/precise/skaters/locationutil/hubermean.py`

 * *Files identical despite different names*

### Comparing `precise-0.9.1/precise/skaters/locationutil/vectorfunctions.py` & `precise-0.9.5/precise/skaters/locationutil/vectorfunctions.py`

 * *Files identical despite different names*

### Comparing `precise-0.9.1/precise/skaters/managers/allmanagers.py` & `precise-0.9.5/precise/skaters/managers/allmanagers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from precise.skaters.managers.weakmanagers import WEAK_LONG_MANAGERS
 from precise.skaters.managers.ppomanagers import PPO_LONG_MANGERS
 from precise.skaters.managers.hrpmanagers import HRP_LONG_MANAGERS
 from precise.skaters.managers.schurmanagers import SCHUR_LONG_MANAGERS
 #from precise.skaters.managers.rflmanagers import RFL_HRP_LONG_MANAGERS
 from precise.skaters.managers.equalmanagers import EQUAL_LONG_MANAGERS
 from precise.skaters.managers.ldpmanagers import LDP_LONG_MANAGERS
-from precise.skaters.managers.molybogamanagers import MOLYBOGA_LONG_MANAGERS
+from precise.skaters.managers.molybogamanagers import MOLYBOGA_LONG_MANGERS
+from precise.skaters.managers.slurpmanagers import SLURP_LONG_MANAGERS
 from precise.skaters.managers.rpmanagers import RP_LONG_MANAGERS
 from tomark import Tomark
 import random
 
 # d0 managers unless otherwise stated
 
 LONG_MANAGERS = WEAK_LONG_MANAGERS + PPO_LONG_MANGERS + HRP_LONG_MANAGERS + SCHUR_LONG_MANAGERS
-LONG_MANAGERS = WEAK_LONG_MANAGERS + PPO_LONG_MANGERS[:100] + HRP_LONG_MANAGERS +\
-SCHUR_LONG_MANAGERS + EQUAL_LONG_MANAGERS + LDP_LONG_MANAGERS + MOLYBOGA_LONG_MANAGERS + RP_LONG_MANAGERS
+LONG_MANAGERS = WEAK_LONG_MANAGERS + PPO_LONG_MANGERS[:100] + HRP_LONG_MANAGERS + \
+                SCHUR_LONG_MANAGERS + EQUAL_LONG_MANAGERS + LDP_LONG_MANAGERS + MOLYBOGA_LONG_MANGERS + SLURP_LONG_MANAGERS + RP_LONG_MANAGERS
 
 RELIABLE_LONG_MANAGERS = [ m for m in LONG_MANAGERS if not 'ppo' in m.__name__]
 
 LS_MANAGERS = []
 MANAGERS = LONG_MANAGERS + LS_MANAGERS
```

### Comparing `precise-0.9.1/precise/skaters/managers/buyandholdfactory.py` & `precise-0.9.5/precise/skaters/managers/buyandholdfactory.py`

 * *Files identical despite different names*

### Comparing `precise-0.9.1/precise/skaters/managers/covmanagerfactory.py` & `precise-0.9.5/precise/skaters/managers/covmanagerfactory.py`

 * *Files identical despite different names*

### Comparing `precise-0.9.1/precise/skaters/managers/equalmanagers.py` & `precise-0.9.5/precise/skaters/managers/equalmanagers.py`

 * *Files identical despite different names*

### Comparing `precise-0.9.1/precise/skaters/managers/hrpmanagers.py` & `precise-0.9.5/precise/skaters/managers/hrpmanagers.py`

 * *Files identical despite different names*

### Comparing `precise-0.9.1/precise/skaters/managers/ldpmanagers.py` & `precise-0.9.5/precise/skaters/managers/ldpmanagers.py`

 * *Files identical despite different names*

### Comparing `precise-0.9.1/precise/skaters/managers/ppomanagerfactory.py` & `precise-0.9.5/precise/skaters/managers/ppomanagerfactory.py`

 * *Files identical despite different names*

### Comparing `precise-0.9.1/precise/skaters/managers/ppomanagers.py` & `precise-0.9.5/precise/skaters/managers/ppomanagers.py`

 * *Files identical despite different names*

### Comparing `precise-0.9.1/precise/skaters/managers/rflmanagerfactory.py` & `precise-0.9.5/precise/skaters/managers/rflmanagerfactory.py`

 * *Files identical despite different names*

### Comparing `precise-0.9.1/precise/skaters/managers/rflmanagers.py` & `precise-0.9.5/precise/skaters/managers/rflmanagers.py`

 * *Files identical despite different names*

### Comparing `precise-0.9.1/precise/skaters/managers/rpmanagers.py` & `precise-0.9.5/precise/skaters/managers/rpmanagers.py`

 * *Files identical despite different names*

### Comparing `precise-0.9.1/precise/skaters/managers/schurmanagerfactory.py` & `precise-0.9.5/precise/skaters/managers/schurmanagerfactory.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from precise.skaters.managers.covmanagerfactory import static_cov_manager_factory_d0
 from precise.skaters.covariance.ewapm import ewa_pm_factory
 from precise.skaters.covariance.bufempfactory import buf_emp_pcov_d0_factory
+from precise.skaters.covariance.ewalwfactory import ewa_lw_scov_factory
 from precise.skaters.portfoliostatic.schurportfactory import schur_portfolio_factory
 from precise.skaters.portfoliostatic.weakportfactory import weak_portfolio_factory
 from precise.skaters.portfoliostatic.weakalloc import weak_allocation_factory
 from precise.skaters.portfoliostatic.diagalloc import diagonal_allocation_factory
 from precise.skaters.portfoliostatic.diagport import diagonal_portfolio_factory
 from precise.skaters.portfoliostatic.volalloc import vol_allocation_factory
 from precise.skaters.portfoliostatic.ppoportfactory import ppo_vol_port
+from precise.skaters.portfoliostatic.rpport import rp_port_p20
 from precise.skaters.covariance.ewaempfactory import ewa_emp_pcov_factory
 from precise.skaters.portfoliostatic.equalport import equal_long_port
 from functools import partial
 from precise.skaters.portfoliostatic.weakportfactory import BIG_H
 
 
 # Convenience functions for Schur managers
```

### Comparing `precise-0.9.1/precise/skaters/managers/schurmanagers.py` & `precise-0.9.5/precise/skaters/managers/schurmanagers.py`

 * *Files identical despite different names*

### Comparing `precise-0.9.1/precise/skaters/managers/weakmanagerfactory.py` & `precise-0.9.5/precise/skaters/managers/weakmanagerfactory.py`

 * *Files identical despite different names*

### Comparing `precise-0.9.1/precise/skaters/managers/weakmanagers.py` & `precise-0.9.5/precise/skaters/managers/weakmanagers.py`

 * *Files identical despite different names*

### Comparing `precise-0.9.1/precise/skaters/managerutil/managerstats.py` & `precise-0.9.5/precise/skaters/managerutil/managerstats.py`

 * *Files identical despite different names*

### Comparing `precise-0.9.1/precise/skaters/managerutil/managertesting.py` & `precise-0.9.5/precise/skaters/managerutil/managertesting.py`

 * *Files identical despite different names*

### Comparing `precise-0.9.1/precise/skaters/portfoliostatic/allstaticport.py` & `precise-0.9.5/precise/skaters/portfoliostatic/allstaticport.py`

 * *Files identical despite different names*

### Comparing `precise-0.9.1/precise/skaters/portfoliostatic/diagallocfactory.py` & `precise-0.9.5/precise/skaters/portfoliostatic/diagallocfactory.py`

 * *Files identical despite different names*

### Comparing `precise-0.9.1/precise/skaters/portfoliostatic/diagportfactory.py` & `precise-0.9.5/precise/skaters/portfoliostatic/diagportfactory.py`

 * *Files identical despite different names*

### Comparing `precise-0.9.1/precise/skaters/portfoliostatic/equalport.py` & `precise-0.9.5/precise/skaters/portfoliostatic/equalport.py`

 * *Files identical despite different names*

### Comparing `precise-0.9.1/precise/skaters/portfoliostatic/hrpport.py` & `precise-0.9.5/precise/skaters/portfoliostatic/hrpport.py`

 * *Files identical despite different names*

### Comparing `precise-0.9.1/precise/skaters/portfoliostatic/hrpportfactory.py` & `precise-0.9.5/precise/skaters/portfoliostatic/hrpportfactory.py`

 * *Files identical despite different names*

### Comparing `precise-0.9.1/precise/skaters/portfoliostatic/ppoport.py` & `precise-0.9.5/precise/skaters/portfoliostatic/ppoport.py`

 * *Files identical despite different names*

### Comparing `precise-0.9.1/precise/skaters/portfoliostatic/ppoportfactory.py` & `precise-0.9.5/precise/skaters/portfoliostatic/ppoportfactory.py`

 * *Files identical despite different names*

### Comparing `precise-0.9.1/precise/skaters/portfoliostatic/rpport.py` & `precise-0.9.5/precise/skaters/portfoliostatic/rpport.py`

 * *Files identical despite different names*

### Comparing `precise-0.9.1/precise/skaters/portfoliostatic/rpportfactory.py` & `precise-0.9.5/precise/skaters/portfoliostatic/rpportfactory.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 
 import numpy as np
 from precise.skaters.covarianceutil.covfunctions import try_invert
 import riskparityportfolio as rp
 from precise.skaters.portfolioutil.portfunctions import var_scaled_returns
 import pandas as pd
 from precise.skaters.covarianceutil.covfunctions import multiply_off_diag
+from precise.skaters.portfoliostatic.equalport import equal_long_port
 
 # Thin wrapper for riskparityportfolio package
 
 
 def rp_portfolio_factory(pre=None, cov=None, mu=0.02, risk_free_rate=0.02, phi=1.0):
     """ Signed min var portfolio summing to unity """
 
     if cov is None:
         cov = try_invert(pre)
     cov = multiply_off_diag(cov,phi=phi)
     expected_returns = var_scaled_returns(cov=cov,mu=mu,r=risk_free_rate)
     w = rp.vanilla.design(cov, b=expected_returns)
+    if any([np.isnan(wi) for wi in w]):
+        return equal_long_port(cov=cov)
     return w
```

### Comparing `precise-0.9.1/precise/skaters/portfoliostatic/schurport.py` & `precise-0.9.5/precise/skaters/portfoliostatic/schurport.py`

 * *Files identical despite different names*

### Comparing `precise-0.9.1/precise/skaters/portfoliostatic/schurportfactory.py` & `precise-0.9.5/precise/skaters/portfoliostatic/schurportfactory.py`

 * *Files identical despite different names*

### Comparing `precise-0.9.1/precise/skaters/portfoliostatic/schurportutil.py` & `precise-0.9.5/precise/skaters/portfoliostatic/schurportutil.py`

 * *Files identical despite different names*

### Comparing `precise-0.9.1/precise/skaters/portfoliostatic/unitallocfactory.py` & `precise-0.9.5/precise/skaters/portfoliostatic/unitallocfactory.py`

 * *Files identical despite different names*

### Comparing `precise-0.9.1/precise/skaters/portfoliostatic/unitportfactory.py` & `precise-0.9.5/precise/skaters/portfoliostatic/unitportfactory.py`

 * *Files identical despite different names*

### Comparing `precise-0.9.1/precise/skaters/portfoliostatic/volallocfactory.py` & `precise-0.9.5/precise/skaters/portfoliostatic/volallocfactory.py`

 * *Files identical despite different names*

### Comparing `precise-0.9.1/precise/skaters/portfoliostatic/weakalloc.py` & `precise-0.9.5/precise/skaters/portfoliostatic/weakalloc.py`

 * *Files identical despite different names*

### Comparing `precise-0.9.1/precise/skaters/portfoliostatic/weakallocfactory.py` & `precise-0.9.5/precise/skaters/portfoliostatic/weakallocfactory.py`

 * *Files identical despite different names*

### Comparing `precise-0.9.1/precise/skaters/portfoliostatic/weakport.py` & `precise-0.9.5/precise/skaters/portfoliostatic/weakport.py`

 * *Files identical despite different names*

### Comparing `precise-0.9.1/precise/skaters/portfoliostatic/weakportfactory.py` & `precise-0.9.5/precise/skaters/portfoliostatic/weakportfactory.py`

 * *Files identical despite different names*

### Comparing `precise-0.9.1/precise/skaters/portfolioutil/portcomparison.py` & `precise-0.9.5/precise/skaters/portfolioutil/portcomparison.py`

 * *Files identical despite different names*

### Comparing `precise-0.9.1/precise/skaters/portfolioutil/portfunctions.py` & `precise-0.9.5/precise/skaters/portfolioutil/portfunctions.py`

 * *Files identical despite different names*

### Comparing `precise-0.9.1/precise/skaters/portfolioutil/portsuggestion.py` & `precise-0.9.5/precise/skaters/portfolioutil/portsuggestion.py`

 * *Files identical despite different names*

### Comparing `precise-0.9.1/precise/skaters/portfolioutil/unitlemmas.py` & `precise-0.9.5/precise/skaters/portfolioutil/unitlemmas.py`

 * *Files identical despite different names*

### Comparing `precise-0.9.1/precise/skaters/portfolioutil/unittransforms.py` & `precise-0.9.5/precise/skaters/portfolioutil/unittransforms.py`

 * *Files identical despite different names*

### Comparing `precise-0.9.1/precise/skaters/scalarutil/runningmedian.py` & `precise-0.9.5/precise/skaters/scalarutil/runningmedian.py`

 * *Files identical despite different names*

### Comparing `precise-0.9.1/precise/skatertools/data/equityhistorical.py` & `precise-0.9.5/precise/skatertools/data/equityhistorical.py`

 * *Files identical despite different names*

### Comparing `precise-0.9.1/precise/skatertools/data/equitylive.py` & `precise-0.9.5/precise/skatertools/data/equitylive.py`

 * *Files identical despite different names*

### Comparing `precise-0.9.1/precise/skatertools/data/etflists.py` & `precise-0.9.5/precise/skatertools/data/etflists.py`

 * *Files identical despite different names*

### Comparing `precise-0.9.1/precise/skatertools/data/skaterresiduals.py` & `precise-0.9.5/precise/skatertools/data/skaterresiduals.py`

 * *Files identical despite different names*

### Comparing `precise-0.9.1/precise/skatertools/m6/competition.py` & `precise-0.9.5/precise/skatertools/m6/competition.py`

 * *Files identical despite different names*

### Comparing `precise-0.9.1/precise/skatertools/m6/covarianceforecasting.py` & `precise-0.9.5/precise/skatertools/m6/covarianceforecasting.py`

 * *Files identical despite different names*

### Comparing `precise-0.9.1/precise/skatertools/m6/quintileprobabilities.py` & `precise-0.9.5/precise/skatertools/m6/quintileprobabilities.py`

 * *Files identical despite different names*

### Comparing `precise-0.9.1/precise/skatertools/m6/tilting.py` & `precise-0.9.5/precise/skatertools/m6/tilting.py`

 * *Files identical despite different names*

### Comparing `precise-0.9.1/precise/skatertools/syntheticdata/factor.py` & `precise-0.9.5/precise/skatertools/syntheticdata/factor.py`

 * *Files identical despite different names*

### Comparing `precise-0.9.1/precise/skatervaluation/battlelatex/tables.py` & `precise-0.9.5/precise/skatervaluation/battlelatex/tables.py`

 * *Files identical despite different names*

### Comparing `precise-0.9.1/precise/skatervaluation/battleutil/arrangingbattles.py` & `precise-0.9.5/precise/skatervaluation/battleutil/arrangingbattles.py`

 * *Files identical despite different names*

### Comparing `precise-0.9.1/precise/skatervaluation/battleutil/battleio.py` & `precise-0.9.5/precise/skatervaluation/battleutil/battleio.py`

 * *Files identical despite different names*

### Comparing `precise-0.9.1/precise/skatervaluation/battleutil/compilingeloratings.py` & `precise-0.9.5/precise/skatervaluation/battleutil/compilingeloratings.py`

 * *Files identical despite different names*

### Comparing `precise-0.9.1/precise/skatervaluation/battleutil/eloformulas.py` & `precise-0.9.5/precise/skatervaluation/battleutil/eloformulas.py`

 * *Files identical despite different names*

### Comparing `precise-0.9.1/precise/skatervaluation/battleutil/speed.py` & `precise-0.9.5/precise/skatervaluation/battleutil/speed.py`

 * *Files identical despite different names*

### Comparing `precise-0.9.1/precise/whereami.py` & `precise-0.9.5/precise/whereami.py`

 * *Files identical despite different names*

### Comparing `precise-0.9.1/precise.egg-info/PKG-INFO` & `precise-0.9.5/precise.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: precise
-Version: 0.9.1
+Version: 0.9.5
 Summary: Online covariance, precision, portfolios and ensembles
 Home-page: https://github.com/microprediction/precise
 Author: microprediction
 Author-email: peter.cotton@microprediction.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `precise-0.9.1/precise.egg-info/SOURCES.txt` & `precise-0.9.5/precise.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -66,23 +66,26 @@
 precise/skaters/managers/__init__.py
 precise/skaters/managers/allmanagers.py
 precise/skaters/managers/buyandholdfactory.py
 precise/skaters/managers/covmanagerfactory.py
 precise/skaters/managers/equalmanagers.py
 precise/skaters/managers/hrpmanagers.py
 precise/skaters/managers/ldpmanagers.py
+precise/skaters/managers/molybogamanagerfactory.py
 precise/skaters/managers/molybogamanagers.py
 precise/skaters/managers/ppomanagerfactory.py
 precise/skaters/managers/ppomanagers.py
 precise/skaters/managers/rflmanagerfactory.py
 precise/skaters/managers/rflmanagers.py
 precise/skaters/managers/rpmanagerfactory.py
 precise/skaters/managers/rpmanagers.py
 precise/skaters/managers/schurmanagerfactory.py
 precise/skaters/managers/schurmanagers.py
+precise/skaters/managers/slurpmanagerfactory.py
+precise/skaters/managers/slurpmanagers.py
 precise/skaters/managers/weakmanagerfactory.py
 precise/skaters/managers/weakmanagers.py
 precise/skaters/managerutil/__init__.py
 precise/skaters/managerutil/managerstats.py
 precise/skaters/managerutil/managertesting.py
 precise/skaters/portfoliostatic/__init__.py
 precise/skaters/portfoliostatic/allstaticalloc.py
```

### Comparing `precise-0.9.1/setup.py` & `precise-0.9.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 HERE = pathlib.Path(__file__).parent
 
 README = (HERE / "README.md").read_text()
 
 setup(
     name="precise",
-    version="0.9.1",
+    version="0.9.5",
     description="Online covariance, precision, portfolios and ensembles",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/microprediction/precise",
     author="microprediction",
     author_email="peter.cotton@microprediction.com",
     license="MIT",
```

