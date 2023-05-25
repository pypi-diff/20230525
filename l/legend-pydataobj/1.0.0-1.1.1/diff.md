# Comparing `tmp/legend_pydataobj-1.0.0.tar.gz` & `tmp/legend_pydataobj-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "legend_pydataobj-1.0.0.tar", last modified: Tue May 23 10:43:52 2023, max compression
+gzip compressed data, was "legend_pydataobj-1.1.1.tar", last modified: Thu May 25 12:32:21 2023, max compression
```

## Comparing `legend_pydataobj-1.0.0.tar` & `legend_pydataobj-1.1.1.tar`

### file list

```diff
@@ -1,65 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:43:52.893440 legend_pydataobj-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-23 10:43:42.000000 legend_pydataobj-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-05-23 10:43:52.893440 legend_pydataobj-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-05-23 10:43:42.000000 legend_pydataobj-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-23 10:43:42.000000 legend_pydataobj-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-05-23 10:43:52.897440 legend_pydataobj-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-23 10:43:42.000000 legend_pydataobj-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:43:52.885440 legend_pydataobj-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:43:52.885440 legend_pydataobj-1.0.0/src/legend_pydataobj.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-05-23 10:43:52.000000 legend_pydataobj-1.0.0/src/legend_pydataobj.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-05-23 10:43:52.000000 legend_pydataobj-1.0.0/src/legend_pydataobj.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 10:43:52.000000 legend_pydataobj-1.0.0/src/legend_pydataobj.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 10:43:52.000000 legend_pydataobj-1.0.0/src/legend_pydataobj.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-23 10:43:52.000000 legend_pydataobj-1.0.0/src/legend_pydataobj.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-23 10:43:52.000000 legend_pydataobj-1.0.0/src/legend_pydataobj.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:43:52.885440 legend_pydataobj-1.0.0/src/lgdo/
--rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-05-23 10:43:42.000000 legend_pydataobj-1.0.0/src/lgdo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-23 10:43:52.000000 legend_pydataobj-1.0.0/src/lgdo/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:43:52.889440 legend_pydataobj-1.0.0/src/lgdo/compression/
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-23 10:43:42.000000 legend_pydataobj-1.0.0/src/lgdo/compression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-23 10:43:42.000000 legend_pydataobj-1.0.0/src/lgdo/compression/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-05-23 10:43:42.000000 legend_pydataobj-1.0.0/src/lgdo/compression/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)    19312 2023-05-23 10:43:42.000000 legend_pydataobj-1.0.0/src/lgdo/compression/radware.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-23 10:43:42.000000 legend_pydataobj-1.0.0/src/lgdo/compression/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    14497 2023-05-23 10:43:42.000000 legend_pydataobj-1.0.0/src/lgdo/compression/varlen.py
--rw-r--r--   0 runner    (1001) docker     (123)     5596 2023-05-23 10:43:42.000000 legend_pydataobj-1.0.0/src/lgdo/lgdo_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    68252 2023-05-23 10:43:42.000000 legend_pydataobj-1.0.0/src/lgdo/lh5_store.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:43:52.889440 legend_pydataobj-1.0.0/src/lgdo/types/
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-05-23 10:43:42.000000 legend_pydataobj-1.0.0/src/lgdo/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-05-23 10:43:42.000000 legend_pydataobj-1.0.0/src/lgdo/types/array.py
--rw-r--r--   0 runner    (1001) docker     (123)     4492 2023-05-23 10:43:42.000000 legend_pydataobj-1.0.0/src/lgdo/types/arrayofequalsizedarrays.py
--rw-r--r--   0 runner    (1001) docker     (123)    11302 2023-05-23 10:43:42.000000 legend_pydataobj-1.0.0/src/lgdo/types/encoded.py
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-05-23 10:43:42.000000 legend_pydataobj-1.0.0/src/lgdo/types/fixedsizearray.py
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-05-23 10:43:42.000000 legend_pydataobj-1.0.0/src/lgdo/types/lgdo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-05-23 10:43:42.000000 legend_pydataobj-1.0.0/src/lgdo/types/scalar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-05-23 10:43:42.000000 legend_pydataobj-1.0.0/src/lgdo/types/struct.py
--rw-r--r--   0 runner    (1001) docker     (123)    12531 2023-05-23 10:43:42.000000 legend_pydataobj-1.0.0/src/lgdo/types/table.py
--rw-r--r--   0 runner    (1001) docker     (123)    21859 2023-05-23 10:43:42.000000 legend_pydataobj-1.0.0/src/lgdo/types/vectorofvectors.py
--rw-r--r--   0 runner    (1001) docker     (123)     9407 2023-05-23 10:43:42.000000 legend_pydataobj-1.0.0/src/lgdo/types/waveform_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:43:52.889440 legend_pydataobj-1.0.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:43:52.893440 legend_pydataobj-1.0.0/tests/compression/
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-23 10:43:42.000000 legend_pydataobj-1.0.0/tests/compression/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:43:52.893440 legend_pydataobj-1.0.0/tests/compression/sigcompress/
--rw-r--r--   0 runner    (1001) docker     (123)    23516 2023-05-23 10:43:42.000000 legend_pydataobj-1.0.0/tests/compression/sigcompress/LDQTA_r117_20200110T105115Z_cal_geds_raw-0.dat
--rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-05-23 10:43:42.000000 legend_pydataobj-1.0.0/tests/compression/sigcompress/special-wf-clipped.dat
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-23 10:43:42.000000 legend_pydataobj-1.0.0/tests/compression/test_compression.py
--rw-r--r--   0 runner    (1001) docker     (123)    47002 2023-05-23 10:43:42.000000 legend_pydataobj-1.0.0/tests/compression/test_radware_sigcompress.py
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-23 10:43:42.000000 legend_pydataobj-1.0.0/tests/compression/test_str2wfcodec.py
--rw-r--r--   0 runner    (1001) docker     (123)     4606 2023-05-23 10:43:42.000000 legend_pydataobj-1.0.0/tests/compression/test_uleb128_zigzag_diff.py
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-05-23 10:43:42.000000 legend_pydataobj-1.0.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-05-23 10:43:42.000000 legend_pydataobj-1.0.0/tests/test_lgdo_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-05-23 10:43:42.000000 legend_pydataobj-1.0.0/tests/test_lh5_iterator.py
--rw-r--r--   0 runner    (1001) docker     (123)    25820 2023-05-23 10:43:42.000000 legend_pydataobj-1.0.0/tests/test_lh5_store.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:43:52.893440 legend_pydataobj-1.0.0/tests/types/
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-05-23 10:43:42.000000 legend_pydataobj-1.0.0/tests/types/test_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-05-23 10:43:42.000000 legend_pydataobj-1.0.0/tests/types/test_arrayofequalsizedarrays.py
--rw-r--r--   0 runner    (1001) docker     (123)     5874 2023-05-23 10:43:42.000000 legend_pydataobj-1.0.0/tests/types/test_encoded.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-23 10:43:42.000000 legend_pydataobj-1.0.0/tests/types/test_fixedsizearray.py
--rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-05-23 10:43:42.000000 legend_pydataobj-1.0.0/tests/types/test_representations.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-05-23 10:43:42.000000 legend_pydataobj-1.0.0/tests/types/test_scalar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-05-23 10:43:42.000000 legend_pydataobj-1.0.0/tests/types/test_struct.py
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-05-23 10:43:42.000000 legend_pydataobj-1.0.0/tests/types/test_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-05-23 10:43:42.000000 legend_pydataobj-1.0.0/tests/types/test_table_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     7267 2023-05-23 10:43:42.000000 legend_pydataobj-1.0.0/tests/types/test_vectorofvectors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-05-23 10:43:42.000000 legend_pydataobj-1.0.0/tests/types/test_waveform_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:32:21.103440 legend_pydataobj-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-25 12:32:13.000000 legend_pydataobj-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-05-25 12:32:21.103440 legend_pydataobj-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-05-25 12:32:13.000000 legend_pydataobj-1.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-25 12:32:13.000000 legend_pydataobj-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-05-25 12:32:21.107438 legend_pydataobj-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-25 12:32:13.000000 legend_pydataobj-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:32:21.099441 legend_pydataobj-1.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:32:21.099441 legend_pydataobj-1.1.1/src/legend_pydataobj.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-05-25 12:32:21.000000 legend_pydataobj-1.1.1/src/legend_pydataobj.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-05-25 12:32:21.000000 legend_pydataobj-1.1.1/src/legend_pydataobj.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 12:32:21.000000 legend_pydataobj-1.1.1/src/legend_pydataobj.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-25 12:32:21.000000 legend_pydataobj-1.1.1/src/legend_pydataobj.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 12:32:20.000000 legend_pydataobj-1.1.1/src/legend_pydataobj.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-25 12:32:21.000000 legend_pydataobj-1.1.1/src/legend_pydataobj.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-25 12:32:21.000000 legend_pydataobj-1.1.1/src/legend_pydataobj.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:32:21.099441 legend_pydataobj-1.1.1/src/lgdo/
+-rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-05-25 12:32:13.000000 legend_pydataobj-1.1.1/src/lgdo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-25 12:32:21.000000 legend_pydataobj-1.1.1/src/lgdo/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-05-25 12:32:13.000000 legend_pydataobj-1.1.1/src/lgdo/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:32:21.103440 legend_pydataobj-1.1.1/src/lgdo/compression/
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-25 12:32:13.000000 legend_pydataobj-1.1.1/src/lgdo/compression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-25 12:32:13.000000 legend_pydataobj-1.1.1/src/lgdo/compression/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-05-25 12:32:13.000000 legend_pydataobj-1.1.1/src/lgdo/compression/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19312 2023-05-25 12:32:13.000000 legend_pydataobj-1.1.1/src/lgdo/compression/radware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-25 12:32:13.000000 legend_pydataobj-1.1.1/src/lgdo/compression/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14497 2023-05-25 12:32:13.000000 legend_pydataobj-1.1.1/src/lgdo/compression/varlen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5596 2023-05-25 12:32:13.000000 legend_pydataobj-1.1.1/src/lgdo/lgdo_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68396 2023-05-25 12:32:13.000000 legend_pydataobj-1.1.1/src/lgdo/lh5_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-25 12:32:13.000000 legend_pydataobj-1.1.1/src/lgdo/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:32:21.103440 legend_pydataobj-1.1.1/src/lgdo/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-05-25 12:32:13.000000 legend_pydataobj-1.1.1/src/lgdo/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-05-25 12:32:13.000000 legend_pydataobj-1.1.1/src/lgdo/types/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4492 2023-05-25 12:32:13.000000 legend_pydataobj-1.1.1/src/lgdo/types/arrayofequalsizedarrays.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11302 2023-05-25 12:32:13.000000 legend_pydataobj-1.1.1/src/lgdo/types/encoded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-05-25 12:32:13.000000 legend_pydataobj-1.1.1/src/lgdo/types/fixedsizearray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-05-25 12:32:13.000000 legend_pydataobj-1.1.1/src/lgdo/types/lgdo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-05-25 12:32:13.000000 legend_pydataobj-1.1.1/src/lgdo/types/scalar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-05-25 12:32:13.000000 legend_pydataobj-1.1.1/src/lgdo/types/struct.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12531 2023-05-25 12:32:13.000000 legend_pydataobj-1.1.1/src/lgdo/types/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21859 2023-05-25 12:32:13.000000 legend_pydataobj-1.1.1/src/lgdo/types/vectorofvectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9407 2023-05-25 12:32:13.000000 legend_pydataobj-1.1.1/src/lgdo/types/waveform_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:32:21.103440 legend_pydataobj-1.1.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:32:21.103440 legend_pydataobj-1.1.1/tests/compression/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-25 12:32:13.000000 legend_pydataobj-1.1.1/tests/compression/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:32:21.103440 legend_pydataobj-1.1.1/tests/compression/sigcompress/
+-rw-r--r--   0 runner    (1001) docker     (123)    23516 2023-05-25 12:32:13.000000 legend_pydataobj-1.1.1/tests/compression/sigcompress/LDQTA_r117_20200110T105115Z_cal_geds_raw-0.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-05-25 12:32:13.000000 legend_pydataobj-1.1.1/tests/compression/sigcompress/special-wf-clipped.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-25 12:32:13.000000 legend_pydataobj-1.1.1/tests/compression/test_compression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47002 2023-05-25 12:32:13.000000 legend_pydataobj-1.1.1/tests/compression/test_radware_sigcompress.py
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-25 12:32:13.000000 legend_pydataobj-1.1.1/tests/compression/test_str2wfcodec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4606 2023-05-25 12:32:13.000000 legend_pydataobj-1.1.1/tests/compression/test_uleb128_zigzag_diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-25 12:32:13.000000 legend_pydataobj-1.1.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-05-25 12:32:13.000000 legend_pydataobj-1.1.1/tests/test_lgdo_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-05-25 12:32:13.000000 legend_pydataobj-1.1.1/tests/test_lh5_iterator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26637 2023-05-25 12:32:13.000000 legend_pydataobj-1.1.1/tests/test_lh5_store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:32:21.103440 legend_pydataobj-1.1.1/tests/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-05-25 12:32:13.000000 legend_pydataobj-1.1.1/tests/types/test_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-05-25 12:32:13.000000 legend_pydataobj-1.1.1/tests/types/test_arrayofequalsizedarrays.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5874 2023-05-25 12:32:13.000000 legend_pydataobj-1.1.1/tests/types/test_encoded.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-25 12:32:13.000000 legend_pydataobj-1.1.1/tests/types/test_fixedsizearray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-05-25 12:32:13.000000 legend_pydataobj-1.1.1/tests/types/test_representations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-05-25 12:32:13.000000 legend_pydataobj-1.1.1/tests/types/test_scalar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-05-25 12:32:13.000000 legend_pydataobj-1.1.1/tests/types/test_struct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-05-25 12:32:13.000000 legend_pydataobj-1.1.1/tests/types/test_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-05-25 12:32:13.000000 legend_pydataobj-1.1.1/tests/types/test_table_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7267 2023-05-25 12:32:13.000000 legend_pydataobj-1.1.1/tests/types/test_vectorofvectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-05-25 12:32:13.000000 legend_pydataobj-1.1.1/tests/types/test_waveform_table.py
```

### Comparing `legend_pydataobj-1.0.0/LICENSE` & `legend_pydataobj-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.0.0/PKG-INFO` & `legend_pydataobj-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: legend_pydataobj
-Version: 1.0.0
+Version: 1.1.1
 Summary: LEGEND Python Data Objects
 Home-page: https://github.com/legend-exp/legend-pydataobj
 Author: The LEGEND Collaboration
 Maintainer: The LEGEND Collaboration
 License: GPL-3.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `legend_pydataobj-1.0.0/README.md` & `legend_pydataobj-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.0.0/setup.cfg` & `legend_pydataobj-1.1.1/setup.cfg`

 * *Files 21% similar despite different names*

```diff
@@ -27,15 +27,16 @@
 	Topic :: Scientific/Engineering :: Mathematics
 	Topic :: Scientific/Engineering :: Physics
 	Topic :: Software Development
 
 [options]
 packages = find:
 install_requires = 
-	h5py>=3.2.0
+	colorlog
+	h5py>=3.2
 	hdf5plugin
 	numba!=0.53.*,!=0.54.*
 	numexpr
 	numpy>=1.21
 	pandas>=1.4.4
 	parse
 	pint
@@ -44,14 +45,18 @@
 package_dir = 
 	= src
 zip_safe = False
 
 [options.packages.find]
 where = src
 
+[options.entry_points]
+console_scripts = 
+	lh5ls = lgdo.cli:lh5ls
+
 [options.extras_require]
 all = 
 	legend-pydataobj[docs,test]
 docs = 
 	furo
 	jupyter
 	myst-parser
```

### Comparing `legend_pydataobj-1.0.0/src/legend_pydataobj.egg-info/PKG-INFO` & `legend_pydataobj-1.1.1/src/legend_pydataobj.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: legend-pydataobj
-Version: 1.0.0
+Version: 1.1.1
 Summary: LEGEND Python Data Objects
 Home-page: https://github.com/legend-exp/legend-pydataobj
 Author: The LEGEND Collaboration
 Maintainer: The LEGEND Collaboration
 License: GPL-3.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `legend_pydataobj-1.0.0/src/legend_pydataobj.egg-info/SOURCES.txt` & `legend_pydataobj-1.1.1/src/legend_pydataobj.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -2,21 +2,24 @@
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 src/legend_pydataobj.egg-info/PKG-INFO
 src/legend_pydataobj.egg-info/SOURCES.txt
 src/legend_pydataobj.egg-info/dependency_links.txt
+src/legend_pydataobj.egg-info/entry_points.txt
 src/legend_pydataobj.egg-info/not-zip-safe
 src/legend_pydataobj.egg-info/requires.txt
 src/legend_pydataobj.egg-info/top_level.txt
 src/lgdo/__init__.py
 src/lgdo/_version.py
+src/lgdo/cli.py
 src/lgdo/lgdo_utils.py
 src/lgdo/lh5_store.py
+src/lgdo/logging.py
 src/lgdo/compression/__init__.py
 src/lgdo/compression/base.py
 src/lgdo/compression/generic.py
 src/lgdo/compression/radware.py
 src/lgdo/compression/utils.py
 src/lgdo/compression/varlen.py
 src/lgdo/types/__init__.py
```

### Comparing `legend_pydataobj-1.0.0/src/lgdo/__init__.py` & `legend_pydataobj-1.1.1/src/lgdo/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 
 Currently the primary on-disk format for LGDO object is LEGEND HDF5 (LH5) files. IO
 is done via the class :class:`.lh5_store.LH5Store`. LH5 files can also be
 browsed easily in python like any `HDF5 <https://www.hdfgroup.org>`_ file using
 `h5py <https://www.h5py.org>`_.
 """
 
+from ._version import version as __version__
 from .lh5_store import LH5Iterator, LH5Store, load_dfs, load_nda, ls, show
 from .types import (
     LGDO,
     Array,
     ArrayOfEncodedEqualSizedArrays,
     ArrayOfEqualSizedArrays,
     FixedSizeArray,
@@ -67,9 +68,9 @@
     "WaveformTable",
     "LH5Iterator",
     "LH5Store",
     "load_dfs",
     "load_nda",
     "ls",
     "show",
-    "copy",
+    "__version__",
 ]
```

### Comparing `legend_pydataobj-1.0.0/src/lgdo/compression/__init__.py` & `legend_pydataobj-1.1.1/src/lgdo/compression/__init__.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.0.0/src/lgdo/compression/base.py` & `legend_pydataobj-1.1.1/src/lgdo/compression/base.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.0.0/src/lgdo/compression/generic.py` & `legend_pydataobj-1.1.1/src/lgdo/compression/generic.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.0.0/src/lgdo/compression/radware.py` & `legend_pydataobj-1.1.1/src/lgdo/compression/radware.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.0.0/src/lgdo/compression/utils.py` & `legend_pydataobj-1.1.1/src/lgdo/compression/utils.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.0.0/src/lgdo/compression/varlen.py` & `legend_pydataobj-1.1.1/src/lgdo/compression/varlen.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.0.0/src/lgdo/lgdo_utils.py` & `legend_pydataobj-1.1.1/src/lgdo/lgdo_utils.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.0.0/src/lgdo/lh5_store.py` & `legend_pydataobj-1.1.1/src/lgdo/lh5_store.py`

 * *Files 1% similar despite different names*

```diff
@@ -1283,33 +1283,40 @@
     while True:
         val = lh5_file[key]
         # we want to print the LGDO datatype
         dtype = val.attrs.get("datatype", default="no datatype")
         if dtype == "no datatype" and isinstance(val, h5py.Group):
             dtype = "HDF5 group"
 
-        attrs_d = dict(val.attrs)
-        attrs_d.pop("datatype", "")
-        attrs = "── " + str(attrs_d) if attrs_d else ""
+        _attrs = ""
+        if attrs:
+            attrs_d = dict(val.attrs)
+            attrs_d.pop("datatype", "")
+            _attrs = "── " + str(attrs_d) if attrs_d else ""
 
         # is this the last key?
         killme = False
         try:
             k_new = next(it)  # get next key
         except StopIteration:
             char = "└──"
             killme = True  # we'll have to kill this loop later
         else:
             char = "├──"
 
-        print(f"{indent}{char} \033[1m{key}\033[0m · {dtype} {attrs}")  # noqa: T201
+        print(f"{indent}{char} \033[1m{key}\033[0m · {dtype} {_attrs}")  # noqa: T201
 
         # if it's a group, call this function recursively
         if isinstance(val, h5py.Group):
-            show(val, indent=indent + ("    " if killme else "│   "), header=False)
+            show(
+                val,
+                indent=indent + ("    " if killme else "│   "),
+                header=False,
+                attrs=attrs,
+            )
 
         # break or move to next key
         if killme:
             break
         else:
             key = k_new
```

### Comparing `legend_pydataobj-1.0.0/src/lgdo/types/__init__.py` & `legend_pydataobj-1.1.1/src/lgdo/types/__init__.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.0.0/src/lgdo/types/array.py` & `legend_pydataobj-1.1.1/src/lgdo/types/array.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.0.0/src/lgdo/types/arrayofequalsizedarrays.py` & `legend_pydataobj-1.1.1/src/lgdo/types/arrayofequalsizedarrays.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.0.0/src/lgdo/types/encoded.py` & `legend_pydataobj-1.1.1/src/lgdo/types/encoded.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.0.0/src/lgdo/types/fixedsizearray.py` & `legend_pydataobj-1.1.1/src/lgdo/types/fixedsizearray.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.0.0/src/lgdo/types/lgdo.py` & `legend_pydataobj-1.1.1/src/lgdo/types/lgdo.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.0.0/src/lgdo/types/scalar.py` & `legend_pydataobj-1.1.1/src/lgdo/types/scalar.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.0.0/src/lgdo/types/struct.py` & `legend_pydataobj-1.1.1/src/lgdo/types/struct.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.0.0/src/lgdo/types/table.py` & `legend_pydataobj-1.1.1/src/lgdo/types/table.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.0.0/src/lgdo/types/vectorofvectors.py` & `legend_pydataobj-1.1.1/src/lgdo/types/vectorofvectors.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.0.0/src/lgdo/types/waveform_table.py` & `legend_pydataobj-1.1.1/src/lgdo/types/waveform_table.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.0.0/tests/compression/sigcompress/LDQTA_r117_20200110T105115Z_cal_geds_raw-0.dat` & `legend_pydataobj-1.1.1/tests/compression/sigcompress/LDQTA_r117_20200110T105115Z_cal_geds_raw-0.dat`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.0.0/tests/compression/sigcompress/special-wf-clipped.dat` & `legend_pydataobj-1.1.1/tests/compression/sigcompress/special-wf-clipped.dat`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.0.0/tests/compression/test_compression.py` & `legend_pydataobj-1.1.1/tests/compression/test_compression.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.0.0/tests/compression/test_radware_sigcompress.py` & `legend_pydataobj-1.1.1/tests/compression/test_radware_sigcompress.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.0.0/tests/compression/test_str2wfcodec.py` & `legend_pydataobj-1.1.1/tests/compression/test_str2wfcodec.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.0.0/tests/compression/test_uleb128_zigzag_diff.py` & `legend_pydataobj-1.1.1/tests/compression/test_uleb128_zigzag_diff.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.0.0/tests/test_lgdo_utils.py` & `legend_pydataobj-1.1.1/tests/test_lgdo_utils.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.0.0/tests/test_lh5_iterator.py` & `legend_pydataobj-1.1.1/tests/test_lh5_iterator.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.0.0/tests/test_lh5_store.py` & `legend_pydataobj-1.1.1/tests/test_lh5_store.py`

 * *Files 7% similar despite different names*

```diff
@@ -29,21 +29,21 @@
     assert isinstance(f, h5py.File)
     assert store.files[lgnd_file] == f
 
     with pytest.raises(FileNotFoundError):
         store.gimme_file("non-existent-file")
 
 
-def test_gimme_group(lgnd_file):
+def test_gimme_group(lgnd_file, tmptestdir):
     f = h5py.File(lgnd_file)
     store = LH5Store()
     g = store.gimme_group("/geds", f)
     assert isinstance(g, h5py.Group)
 
-    f = h5py.File("/tmp/testfile.lh5", mode="w")
+    f = h5py.File(f"{tmptestdir}/testfile.lh5", mode="w")
     g = store.gimme_group("/geds", f, grp_attrs={"attr1": 1}, overwrite=True)
     assert isinstance(g, h5py.Group)
 
 
 def test_show(lgnd_file):
     lh5.show(lgnd_file)
     lh5.show(lgnd_file, "/geds/raw")
@@ -91,15 +91,15 @@
         idx_list=[[1, 3, 5], [2, 6, 7]],
     )
 
     assert isinstance(dfs, pd.DataFrame)
 
 
 @pytest.fixture(scope="module")
-def lh5_file():
+def lh5_file(tmptestdir):
     store = LH5Store()
 
     struct = lgdo.Struct()
     struct.add_field("scalar", lgdo.Scalar(value=10, attrs={"sth": 1}))
     struct.add_field("array", lgdo.Array(nda=np.array([1, 2, 3, 4, 5])))
     struct.add_field(
         "aoesa",
@@ -157,30 +157,30 @@
             ),
         ),
     )
 
     store.write_object(
         struct,
         "struct",
-        "/tmp/tmp-pygama-lgdo-types.lh5",
+        f"{tmptestdir}/tmp-pygama-lgdo-types.lh5",
         group="/data",
         start_row=1,
         n_rows=3,
         wo_mode="overwrite_file",
     )
 
     store.write_object(
         struct,
         "struct_full",
-        "/tmp/tmp-pygama-lgdo-types.lh5",
+        f"{tmptestdir}/tmp-pygama-lgdo-types.lh5",
         group="/data",
         wo_mode="append",
     )
 
-    return "/tmp/tmp-pygama-lgdo-types.lh5"
+    return f"{tmptestdir}/tmp-pygama-lgdo-types.lh5"
 
 
 def test_write_objects(lh5_file):
     pass
 
 
 def test_read_n_rows(lh5_file):
@@ -473,131 +473,144 @@
         idx=[7, 9, 25, 27, 33, 38, 46, 52, 57, 59, 67, 71, 72, 82, 90, 92, 93, 94, 97],
     )
     assert isinstance(lh5_obj, lgdo.WaveformTable)
     assert len(lh5_obj) == 19
 
 
 @pytest.fixture(scope="module")
-def enc_lgnd_file(lgnd_file):
+def enc_lgnd_file(lgnd_file, tmptestdir):
     store = LH5Store()
     wft, n_rows = store.read_object("/geds/raw/waveform", lgnd_file)
     wft.values.attrs["compression"] = RadwareSigcompress(codec_shift=-32768)
     store.write_object(
         wft,
         "/geds/raw/waveform",
-        "/tmp/tmp-pygama-compressed-wfs.lh5",
+        f"{tmptestdir}/tmp-pygama-compressed-wfs.lh5",
         wo_mode="overwrite_file",
     )
-    return "/tmp/tmp-pygama-compressed-wfs.lh5"
+    return f"{tmptestdir}/tmp-pygama-compressed-wfs.lh5"
 
 
 def test_write_compressed_lgnd_waveform_table(enc_lgnd_file):
     pass
 
 
 def test_read_compressed_lgnd_waveform_table(lgnd_file, enc_lgnd_file):
     store = LH5Store()
     wft, _ = store.read_object("/geds/raw/waveform", enc_lgnd_file)
     assert isinstance(wft.values, lgdo.ArrayOfEqualSizedArrays)
     assert "compression" not in wft.values.attrs
 
 
 # First test that we can overwrite a table with the same name without deleting the original field
-def test_write_object_overwrite_table_no_deletion(caplog):
+def test_write_object_overwrite_table_no_deletion(caplog, tmptestdir):
     caplog.set_level(logging.DEBUG)
     caplog.clear()
 
-    if os.path.exists("/tmp/write_object_overwrite_test.lh5"):
-        os.remove("/tmp/write_object_overwrite_test.lh5")
+    if os.path.exists(f"{tmptestdir}/write_object_overwrite_test.lh5"):
+        os.remove(f"{tmptestdir}/write_object_overwrite_test.lh5")
 
     tb1 = lh5.Table(col_dict={"dset1": lh5.Array(np.zeros(10))})
     tb2 = lh5.Table(
         col_dict={"dset1": lh5.Array(np.ones(10))}
     )  # Same field name, different values
     store = LH5Store()
-    store.write_object(tb1, "my_group", "/tmp/write_object_overwrite_test.lh5")
+    store.write_object(tb1, "my_group", f"{tmptestdir}/write_object_overwrite_test.lh5")
     store.write_object(
-        tb2, "my_group", "/tmp/write_object_overwrite_test.lh5", wo_mode="overwrite"
+        tb2,
+        "my_group",
+        f"{tmptestdir}/write_object_overwrite_test.lh5",
+        wo_mode="overwrite",
     )  # Now, try to overwrite the same field
 
     # If the old field is deleted from the file before writing the new field, then we would get an extra debug statement
     assert "dset1 is not present in new table, deleting field" not in [
         rec.message for rec in caplog.records
     ]
 
     # Now, check that the data were overwritten
-    tb_dat, _ = store.read_object("my_group", "/tmp/write_object_overwrite_test.lh5")
+    tb_dat, _ = store.read_object(
+        "my_group", f"{tmptestdir}/write_object_overwrite_test.lh5"
+    )
     assert np.array_equal(tb_dat["dset1"].nda, np.ones(10))
 
 
 # Second: test that when we overwrite a table with fields with a different name, we delete the original field
-def test_write_object_overwrite_table_with_deletion(caplog):
+def test_write_object_overwrite_table_with_deletion(caplog, tmptestdir):
     caplog.set_level(logging.DEBUG)
     caplog.clear()
 
-    if os.path.exists("/tmp/write_object_overwrite_test.lh5"):
-        os.remove("/tmp/write_object_overwrite_test.lh5")
+    if os.path.exists(f"{tmptestdir}/write_object_overwrite_test.lh5"):
+        os.remove(f"{tmptestdir}/write_object_overwrite_test.lh5")
 
     tb1 = lh5.Table(col_dict={"dset1": lh5.Array(np.zeros(10))})
     tb2 = lh5.Table(
         col_dict={"dset2": lh5.Array(np.ones(10))}
     )  # Same field name, different values
     store = LH5Store()
-    store.write_object(tb1, "my_group", "/tmp/write_object_overwrite_test.lh5")
+    store.write_object(tb1, "my_group", f"{tmptestdir}/write_object_overwrite_test.lh5")
     store.write_object(
-        tb2, "my_group", "/tmp/write_object_overwrite_test.lh5", wo_mode="overwrite"
+        tb2,
+        "my_group",
+        f"{tmptestdir}/write_object_overwrite_test.lh5",
+        wo_mode="overwrite",
     )  # Now, try to overwrite with a different field
 
     # Now, check that the data were overwritten
-    tb_dat, _ = store.read_object("my_group", "/tmp/write_object_overwrite_test.lh5")
+    tb_dat, _ = store.read_object(
+        "my_group", f"{tmptestdir}/write_object_overwrite_test.lh5"
+    )
     assert np.array_equal(tb_dat["dset2"].nda, np.ones(10))
 
     # Also make sure that the first table's fields aren't lurking around the lh5 file!
-    with h5py.File("/tmp/write_object_overwrite_test.lh5", "r") as lh5file:
+    with h5py.File(f"{tmptestdir}/write_object_overwrite_test.lh5", "r") as lh5file:
         assert "dset1" not in list(lh5file["my_group"].keys())
 
     # Make sure the same behavior happens when we nest the table in a group
-    if os.path.exists("/tmp/write_object_overwrite_test.lh5"):
-        os.remove("/tmp/write_object_overwrite_test.lh5")
+    if os.path.exists(f"{tmptestdir}/write_object_overwrite_test.lh5"):
+        os.remove(f"{tmptestdir}/write_object_overwrite_test.lh5")
 
     tb1 = lh5.Table(col_dict={"dset1": lh5.Array(np.zeros(10))})
     tb2 = lh5.Table(
         col_dict={"dset2": lh5.Array(np.ones(10))}
     )  # Same field name, different values
     store = LH5Store()
     store.write_object(
-        tb1, "my_table", "/tmp/write_object_overwrite_test.lh5", group="my_group"
+        tb1,
+        "my_table",
+        f"{tmptestdir}/write_object_overwrite_test.lh5",
+        group="my_group",
     )
     store.write_object(
         tb2,
         "my_table",
-        "/tmp/write_object_overwrite_test.lh5",
+        f"{tmptestdir}/write_object_overwrite_test.lh5",
         group="my_group",
         wo_mode="overwrite",
     )  # Now, try to overwrite with a different field
 
     # Now, check that the data were overwritten
     tb_dat, _ = store.read_object(
-        "my_group/my_table", "/tmp/write_object_overwrite_test.lh5"
+        "my_group/my_table", f"{tmptestdir}/write_object_overwrite_test.lh5"
     )
     assert np.array_equal(tb_dat["dset2"].nda, np.ones(10))
 
     # Also make sure that the first table's fields aren't lurking around the lh5 file!
-    with h5py.File("/tmp/write_object_overwrite_test.lh5", "r") as lh5file:
+    with h5py.File(f"{tmptestdir}/write_object_overwrite_test.lh5", "r") as lh5file:
         assert "dset1" not in list(lh5file["my_group/my_table"].keys())
 
 
 # Third: test that when we overwrite other LGDO classes
-def test_write_object_overwrite_lgdo(caplog):
+def test_write_object_overwrite_lgdo(caplog, tmptestdir):
     caplog.set_level(logging.DEBUG)
     caplog.clear()
 
     # Start with an lgdo.WaveformTable
-    if os.path.exists("/tmp/write_object_overwrite_test.lh5"):
-        os.remove("/tmp/write_object_overwrite_test.lh5")
+    if os.path.exists(f"{tmptestdir}/write_object_overwrite_test.lh5"):
+        os.remove(f"{tmptestdir}/write_object_overwrite_test.lh5")
 
     tb1 = lh5.WaveformTable(
         t0=np.zeros(10),
         t0_units="ns",
         dt=np.zeros(10),
         dt_units="ns",
         values=np.zeros((10, 10)),
@@ -609,187 +622,207 @@
         dt=np.ones(10),
         dt_units="ns",
         values=np.ones((10, 10)),
         values_units="ADC",
     )  # Same field name, different values
     store = LH5Store()
     store.write_object(
-        tb1, "my_table", "/tmp/write_object_overwrite_test.lh5", group="my_group"
+        tb1,
+        "my_table",
+        f"{tmptestdir}/write_object_overwrite_test.lh5",
+        group="my_group",
     )
     store.write_object(
         tb2,
         "my_table",
-        "/tmp/write_object_overwrite_test.lh5",
+        f"{tmptestdir}/write_object_overwrite_test.lh5",
         wo_mode="overwrite",
         group="my_group",
     )
 
     # If the old field is deleted from the file before writing the new field, then we would get a debug statement
     assert "my_table is not present in new table, deleting field" not in [
         rec.message for rec in caplog.records
     ]
 
     # Now, check that the data were overwritten
     tb_dat, _ = store.read_object(
-        "my_group/my_table", "/tmp/write_object_overwrite_test.lh5"
+        "my_group/my_table", f"{tmptestdir}/write_object_overwrite_test.lh5"
     )
     assert np.array_equal(tb_dat["values"].nda, np.ones((10, 10)))
 
     # Now try overwriting an array, and test the write_start argument
     array1 = lh5.Array(nda=np.zeros(10))
     array2 = lh5.Array(nda=np.ones(20))
     store = LH5Store()
-    store.write_object(array1, "my_array", "/tmp/write_object_overwrite_test.lh5")
+    store.write_object(
+        array1, "my_array", f"{tmptestdir}/write_object_overwrite_test.lh5"
+    )
     store.write_object(
         array2,
         "my_array",
-        "/tmp/write_object_overwrite_test.lh5",
+        f"{tmptestdir}/write_object_overwrite_test.lh5",
         wo_mode="overwrite",
         write_start=5,
     )
 
     # Now, check that the data were overwritten
-    array_dat, _ = store.read_object("my_array", "/tmp/write_object_overwrite_test.lh5")
+    array_dat, _ = store.read_object(
+        "my_array", f"{tmptestdir}/write_object_overwrite_test.lh5"
+    )
     expected_out_array = np.append(np.zeros(5), np.ones(20))
 
     assert np.array_equal(array_dat.nda, expected_out_array)
 
     # Now try overwriting a scalar
     scalar1 = lh5.Scalar(0)
     scalar2 = lh5.Scalar(1)
     store = LH5Store()
-    store.write_object(scalar1, "my_scalar", "/tmp/write_object_overwrite_test.lh5")
+    store.write_object(
+        scalar1, "my_scalar", f"{tmptestdir}/write_object_overwrite_test.lh5"
+    )
     store.write_object(
         scalar2,
         "my_scalar",
-        "/tmp/write_object_overwrite_test.lh5",
+        f"{tmptestdir}/write_object_overwrite_test.lh5",
         wo_mode="overwrite",
     )
 
     # Now, check that the data were overwritten
     scalar_dat, _ = store.read_object(
-        "my_scalar", "/tmp/write_object_overwrite_test.lh5"
+        "my_scalar", f"{tmptestdir}/write_object_overwrite_test.lh5"
     )
 
     assert scalar_dat.value == 1
 
     # Finally, try overwriting a vector of vectors
     vov1 = lh5.VectorOfVectors(listoflists=[np.zeros(1), np.ones(2), np.zeros(3)])
     vov2 = lh5.VectorOfVectors(listoflists=[np.ones(1), np.zeros(2), np.ones(3)])
     store = LH5Store()
-    store.write_object(vov1, "my_vector", "/tmp/write_object_overwrite_test.lh5")
+    store.write_object(
+        vov1, "my_vector", f"{tmptestdir}/write_object_overwrite_test.lh5"
+    )
     store.write_object(
         vov2,
         "my_vector",
-        "/tmp/write_object_overwrite_test.lh5",
+        f"{tmptestdir}/write_object_overwrite_test.lh5",
         wo_mode="overwrite",
         write_start=1,
     )  # start overwriting the second list of lists
 
     vector_dat, _ = store.read_object(
-        "my_vector", "/tmp/write_object_overwrite_test.lh5"
+        "my_vector", f"{tmptestdir}/write_object_overwrite_test.lh5"
     )
 
     assert np.array_equal(vector_dat.cumulative_length.nda, [1, 2, 4, 7])
     assert np.array_equal(vector_dat.flattened_data.nda, [0, 1, 0, 0, 1, 1, 1])
 
 
 # Test that when we try to overwrite an existing column in a table we fail
-def test_write_object_append_column():
+def test_write_object_append_column(tmptestdir):
     # Try to append an array to a table
-    if os.path.exists("/tmp/write_object_append_column_test.lh5"):
-        os.remove("/tmp/write_object_append_column_test.lh5")
+    if os.path.exists(f"{tmptestdir}/write_object_append_column_test.lh5"):
+        os.remove(f"{tmptestdir}/write_object_append_column_test.lh5")
 
     array1 = lh5.Array(np.zeros(10))
     tb1 = lh5.Table(col_dict={"dset1`": lh5.Array(np.ones(10))})
     store = LH5Store()
-    store.write_object(array1, "my_table", "/tmp/write_object_append_column_test.lh5")
+    store.write_object(
+        array1, "my_table", f"{tmptestdir}/write_object_append_column_test.lh5"
+    )
     with pytest.raises(RuntimeError) as exc_info:
         store.write_object(
             tb1,
             "my_table",
-            "/tmp/write_object_append_column_test.lh5",
+            f"{tmptestdir}/write_object_append_column_test.lh5",
             wo_mode="append_column",
         )  # Now, try to append a column to an array
 
     assert exc_info.type is RuntimeError
     assert (
         exc_info.value.args[0] == "Trying to append columns to an object of type array"
     )
 
     # Try to append a table that has a same key as the old table
-    if os.path.exists("/tmp/write_object_append_column_test.lh5"):
-        os.remove("/tmp/write_object_append_column_test.lh5")
+    if os.path.exists(f"{tmptestdir}/write_object_append_column_test.lh5"):
+        os.remove(f"{tmptestdir}/write_object_append_column_test.lh5")
 
     tb1 = lh5.Table(
         col_dict={"dset1": lh5.Array(np.zeros(10)), "dset2": lh5.Array(np.zeros(10))}
     )
     tb2 = lh5.Table(
         col_dict={"dset2": lh5.Array(np.ones(10))}
     )  # Same field name, different values
     store = LH5Store()
-    store.write_object(tb1, "my_table", "/tmp/write_object_append_column_test.lh5")
+    store.write_object(
+        tb1, "my_table", f"{tmptestdir}/write_object_append_column_test.lh5"
+    )
     with pytest.raises(ValueError) as exc_info:
         store.write_object(
             tb2,
             "my_table",
-            "/tmp/write_object_append_column_test.lh5",
+            f"{tmptestdir}/write_object_append_column_test.lh5",
             wo_mode="append_column",
         )  # Now, try to append a column with a same field
 
     assert exc_info.type is ValueError
     assert (
         exc_info.value.args[0]
         == "Can't append ['dset2'] column(s) to a table with the same field(s)"
     )
 
     # try appending a column that is larger than one that exists
-    if os.path.exists("/tmp/write_object_append_column_test.lh5"):
-        os.remove("/tmp/write_object_append_column_test.lh5")
+    if os.path.exists(f"{tmptestdir}/write_object_append_column_test.lh5"):
+        os.remove(f"{tmptestdir}/write_object_append_column_test.lh5")
 
     tb1 = lh5.Table(col_dict={"dset1": lh5.Array(np.zeros(10))})
     tb2 = lh5.Table(
         col_dict={"dset2": lh5.Array(np.ones(20))}
     )  # different field name, different size
     store = LH5Store()
-    store.write_object(tb1, "my_table", "/tmp/write_object_append_column_test.lh5")
+    store.write_object(
+        tb1, "my_table", f"{tmptestdir}/write_object_append_column_test.lh5"
+    )
     with pytest.raises(ValueError) as exc_info:
         store.write_object(
             tb2,
             "my_table",
-            "/tmp/write_object_append_column_test.lh5",
+            f"{tmptestdir}/write_object_append_column_test.lh5",
             wo_mode="append_column",
         )  # Now, try to append a column with a different field size
 
     assert exc_info.type is ValueError
     assert (
         exc_info.value.args[0]
         == "Table sizes don't match. Trying to append column of size 20 to a table of size 10."
     )
 
     # Finally successfully append a column
-    if os.path.exists("/tmp/write_object_append_column_test.lh5"):
-        os.remove("/tmp/write_object_append_column_test.lh5")
+    if os.path.exists(f"{tmptestdir}/write_object_append_column_test.lh5"):
+        os.remove(f"{tmptestdir}/write_object_append_column_test.lh5")
 
     tb1 = lh5.Table(col_dict={"dset1": lh5.Array(np.zeros(10))})
     tb2 = lh5.Table(
         col_dict={"dset2": lh5.Array(np.ones(10))}
     )  # different field name, different size
     store = LH5Store()
     store.write_object(
-        tb1, "my_table", "/tmp/write_object_append_column_test.lh5", group="my_group"
+        tb1,
+        "my_table",
+        f"{tmptestdir}/write_object_append_column_test.lh5",
+        group="my_group",
     )
     store.write_object(
         tb2,
         "my_table",
-        "/tmp/write_object_append_column_test.lh5",
+        f"{tmptestdir}/write_object_append_column_test.lh5",
         group="my_group",
         wo_mode="append_column",
     )
 
     # Now, check that the data were appended
     tb_dat, _ = store.read_object(
-        "my_group/my_table", "/tmp/write_object_append_column_test.lh5"
+        "my_group/my_table", f"{tmptestdir}/write_object_append_column_test.lh5"
     )
     assert isinstance(tb_dat, lgdo.Table)
     assert np.array_equal(tb_dat["dset1"].nda, np.zeros(10))
     assert np.array_equal(tb_dat["dset2"].nda, np.ones(10))
```

### Comparing `legend_pydataobj-1.0.0/tests/types/test_array.py` & `legend_pydataobj-1.1.1/tests/types/test_array.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.0.0/tests/types/test_arrayofequalsizedarrays.py` & `legend_pydataobj-1.1.1/tests/types/test_arrayofequalsizedarrays.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.0.0/tests/types/test_encoded.py` & `legend_pydataobj-1.1.1/tests/types/test_encoded.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.0.0/tests/types/test_fixedsizearray.py` & `legend_pydataobj-1.1.1/tests/types/test_fixedsizearray.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.0.0/tests/types/test_representations.py` & `legend_pydataobj-1.1.1/tests/types/test_representations.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.0.0/tests/types/test_scalar.py` & `legend_pydataobj-1.1.1/tests/types/test_scalar.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.0.0/tests/types/test_struct.py` & `legend_pydataobj-1.1.1/tests/types/test_struct.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.0.0/tests/types/test_table.py` & `legend_pydataobj-1.1.1/tests/types/test_table.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.0.0/tests/types/test_table_eval.py` & `legend_pydataobj-1.1.1/tests/types/test_table_eval.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.0.0/tests/types/test_vectorofvectors.py` & `legend_pydataobj-1.1.1/tests/types/test_vectorofvectors.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.0.0/tests/types/test_waveform_table.py` & `legend_pydataobj-1.1.1/tests/types/test_waveform_table.py`

 * *Files identical despite different names*

