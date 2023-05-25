# Comparing `tmp/oranchada-0.0.8.tar.gz` & `tmp/oranchada-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oranchada-0.0.8.tar", last modified: Tue May 16 00:02:25 2023, max compression
+gzip compressed data, was "oranchada-0.0.9.tar", last modified: Thu May 25 14:49:52 2023, max compression
```

## Comparing `oranchada-0.0.8.tar` & `oranchada-0.0.9.tar`

### file list

```diff
@@ -1,68 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:02:25.339974 oranchada-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-16 00:02:14.000000 oranchada-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-16 00:02:14.000000 oranchada-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-05-16 00:02:25.339974 oranchada-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5544 2023-05-16 00:02:14.000000 oranchada-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-16 00:02:14.000000 oranchada-0.0.8/README.pypi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:02:25.331974 oranchada-0.0.8/oranchada.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-05-16 00:02:25.000000 oranchada-0.0.8/oranchada.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-05-16 00:02:25.000000 oranchada-0.0.8/oranchada.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 00:02:25.000000 oranchada-0.0.8/oranchada.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-16 00:02:25.000000 oranchada-0.0.8/oranchada.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-16 00:02:25.000000 oranchada-0.0.8/oranchada.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 00:02:25.000000 oranchada-0.0.8/oranchada.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-16 00:02:25.000000 oranchada-0.0.8/oranchada.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-16 00:02:25.000000 oranchada-0.0.8/oranchada.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:02:25.331974 oranchada-0.0.8/orangecontrib/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-16 00:02:14.000000 oranchada-0.0.8/orangecontrib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:02:25.331974 oranchada-0.0.8/orangecontrib/oranchada/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 00:02:14.000000 oranchada-0.0.8/orangecontrib/oranchada/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:02:25.331974 oranchada-0.0.8/orangecontrib/oranchada/base_widget/
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-16 00:02:14.000000 oranchada-0.0.8/orangecontrib/oranchada/base_widget/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-16 00:02:14.000000 oranchada-0.0.8/orangecontrib/oranchada/base_widget/arithmetic_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-05-16 00:02:14.000000 oranchada-0.0.8/orangecontrib/oranchada/base_widget/base_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-16 00:02:14.000000 oranchada-0.0.8/orangecontrib/oranchada/base_widget/creator_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-16 00:02:14.000000 oranchada-0.0.8/orangecontrib/oranchada/base_widget/filter_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-16 00:02:14.000000 oranchada-0.0.8/orangecontrib/oranchada/base_widget/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:02:25.331974 oranchada-0.0.8/orangecontrib/oranchada/processings/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 00:02:14.000000 oranchada-0.0.8/orangecontrib/oranchada/processings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-05-16 00:02:14.000000 oranchada-0.0.8/orangecontrib/oranchada/processings/add_baseline.py
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-16 00:02:14.000000 oranchada-0.0.8/orangecontrib/oranchada/processings/add_noise.py
--rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-05-16 00:02:14.000000 oranchada-0.0.8/orangecontrib/oranchada/processings/gen_spe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:02:25.335974 oranchada-0.0.8/orangecontrib/oranchada/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 00:02:14.000000 oranchada-0.0.8/orangecontrib/oranchada/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-05-16 00:02:14.000000 oranchada-0.0.8/orangecontrib/oranchada/tests/process_spectra_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:02:25.335974 oranchada-0.0.8/orangecontrib/oranchada/widgets_easy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 00:02:14.000000 oranchada-0.0.8/orangecontrib/oranchada/widgets_easy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-05-16 00:02:14.000000 oranchada-0.0.8/orangecontrib/oranchada/widgets_easy/gen_noisy_spe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:02:25.335974 oranchada-0.0.8/orangecontrib/oranchada/widgets_easy/icons/
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-16 00:02:14.000000 oranchada-0.0.8/orangecontrib/oranchada/widgets_easy/icons/spectra.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:02:25.339974 oranchada-0.0.8/orangecontrib/oranchada/widgets_pro/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 00:02:14.000000 oranchada-0.0.8/orangecontrib/oranchada/widgets_pro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-05-16 00:02:14.000000 oranchada-0.0.8/orangecontrib/oranchada/widgets_pro/add_baseline.py
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-16 00:02:14.000000 oranchada-0.0.8/orangecontrib/oranchada/widgets_pro/add_noise.py
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-16 00:02:14.000000 oranchada-0.0.8/orangecontrib/oranchada/widgets_pro/arithmetics_add.py
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-16 00:02:14.000000 oranchada-0.0.8/orangecontrib/oranchada/widgets_pro/arithmetics_subtract.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-05-16 00:02:14.000000 oranchada-0.0.8/orangecontrib/oranchada/widgets_pro/find_peaks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-05-16 00:02:14.000000 oranchada-0.0.8/orangecontrib/oranchada/widgets_pro/fit_peaks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-05-16 00:02:14.000000 oranchada-0.0.8/orangecontrib/oranchada/widgets_pro/gen_spe.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-16 00:02:14.000000 oranchada-0.0.8/orangecontrib/oranchada/widgets_pro/hdr_merge.py
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-16 00:02:14.000000 oranchada-0.0.8/orangecontrib/oranchada/widgets_pro/hht_sharpening.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:02:25.339974 oranchada-0.0.8/orangecontrib/oranchada/widgets_pro/icons/
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-16 00:02:14.000000 oranchada-0.0.8/orangecontrib/oranchada/widgets_pro/icons/spectra.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-05-16 00:02:14.000000 oranchada-0.0.8/orangecontrib/oranchada/widgets_pro/load_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-16 00:02:14.000000 oranchada-0.0.8/orangecontrib/oranchada/widgets_pro/load_file_names.py
--rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-05-16 00:02:14.000000 oranchada-0.0.8/orangecontrib/oranchada/widgets_pro/load_test_spectra.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-05-16 00:02:14.000000 oranchada-0.0.8/orangecontrib/oranchada/widgets_pro/merger.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-16 00:02:14.000000 oranchada-0.0.8/orangecontrib/oranchada/widgets_pro/moving_minimum.py
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-16 00:02:14.000000 oranchada-0.0.8/orangecontrib/oranchada/widgets_pro/normalize.py
--rw-r--r--   0 runner    (1001) docker     (123)     6773 2023-05-16 00:02:14.000000 oranchada-0.0.8/orangecontrib/oranchada/widgets_pro/process_spectra.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-16 00:02:14.000000 oranchada-0.0.8/orangecontrib/oranchada/widgets_pro/raman_shift_to_wavelength.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-05-16 00:02:14.000000 oranchada-0.0.8/orangecontrib/oranchada/widgets_pro/remove_spikes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-05-16 00:02:14.000000 oranchada-0.0.8/orangecontrib/oranchada/widgets_pro/resample_NUDFT.py
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-16 00:02:14.000000 oranchada-0.0.8/orangecontrib/oranchada/widgets_pro/select.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-05-16 00:02:14.000000 oranchada-0.0.8/orangecontrib/oranchada/widgets_pro/set_xaxis.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-16 00:02:14.000000 oranchada-0.0.8/orangecontrib/oranchada/widgets_pro/wavelength_to_raman_shift.py
--rw-r--r--   0 runner    (1001) docker     (123)     7609 2023-05-16 00:02:14.000000 oranchada-0.0.8/orangecontrib/oranchada/widgets_pro/xaxis_fine_calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 00:02:25.339974 oranchada-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4881 2023-05-16 00:02:14.000000 oranchada-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:49:52.144660 oranchada-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-25 14:49:40.000000 oranchada-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-25 14:49:40.000000 oranchada-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-05-25 14:49:52.144660 oranchada-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5546 2023-05-25 14:49:40.000000 oranchada-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-25 14:49:40.000000 oranchada-0.0.9/README.pypi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:49:52.136660 oranchada-0.0.9/oranchada.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-05-25 14:49:52.000000 oranchada-0.0.9/oranchada.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-05-25 14:49:52.000000 oranchada-0.0.9/oranchada.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 14:49:52.000000 oranchada-0.0.9/oranchada.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-25 14:49:52.000000 oranchada-0.0.9/oranchada.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-25 14:49:52.000000 oranchada-0.0.9/oranchada.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 14:49:51.000000 oranchada-0.0.9/oranchada.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-25 14:49:52.000000 oranchada-0.0.9/oranchada.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-25 14:49:52.000000 oranchada-0.0.9/oranchada.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:49:52.140660 oranchada-0.0.9/orangecontrib/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-25 14:49:40.000000 oranchada-0.0.9/orangecontrib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:49:52.140660 oranchada-0.0.9/orangecontrib/oranchada/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:49:40.000000 oranchada-0.0.9/orangecontrib/oranchada/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:49:52.140660 oranchada-0.0.9/orangecontrib/oranchada/base_widget/
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-25 14:49:40.000000 oranchada-0.0.9/orangecontrib/oranchada/base_widget/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-25 14:49:40.000000 oranchada-0.0.9/orangecontrib/oranchada/base_widget/arithmetic_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5171 2023-05-25 14:49:40.000000 oranchada-0.0.9/orangecontrib/oranchada/base_widget/base_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-25 14:49:40.000000 oranchada-0.0.9/orangecontrib/oranchada/base_widget/creator_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-25 14:49:40.000000 oranchada-0.0.9/orangecontrib/oranchada/base_widget/filter_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-25 14:49:40.000000 oranchada-0.0.9/orangecontrib/oranchada/base_widget/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:49:52.140660 oranchada-0.0.9/orangecontrib/oranchada/processings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:49:40.000000 oranchada-0.0.9/orangecontrib/oranchada/processings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-05-25 14:49:40.000000 oranchada-0.0.9/orangecontrib/oranchada/processings/add_baseline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-25 14:49:40.000000 oranchada-0.0.9/orangecontrib/oranchada/processings/add_noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-05-25 14:49:40.000000 oranchada-0.0.9/orangecontrib/oranchada/processings/gen_spe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:49:52.140660 oranchada-0.0.9/orangecontrib/oranchada/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:49:40.000000 oranchada-0.0.9/orangecontrib/oranchada/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-05-25 14:49:40.000000 oranchada-0.0.9/orangecontrib/oranchada/tests/process_spectra_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:49:52.140660 oranchada-0.0.9/orangecontrib/oranchada/widgets_easy/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-25 14:49:40.000000 oranchada-0.0.9/orangecontrib/oranchada/widgets_easy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-05-25 14:49:40.000000 oranchada-0.0.9/orangecontrib/oranchada/widgets_easy/gen_noisy_spe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:49:52.140660 oranchada-0.0.9/orangecontrib/oranchada/widgets_easy/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-05-25 14:49:40.000000 oranchada-0.0.9/orangecontrib/oranchada/widgets_easy/icons/CHARISMA_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-25 14:49:40.000000 oranchada-0.0.9/orangecontrib/oranchada/widgets_easy/icons/spectra.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:49:52.144660 oranchada-0.0.9/orangecontrib/oranchada/widgets_pro/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-25 14:49:40.000000 oranchada-0.0.9/orangecontrib/oranchada/widgets_pro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-05-25 14:49:40.000000 oranchada-0.0.9/orangecontrib/oranchada/widgets_pro/add_baseline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-25 14:49:40.000000 oranchada-0.0.9/orangecontrib/oranchada/widgets_pro/add_noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-25 14:49:40.000000 oranchada-0.0.9/orangecontrib/oranchada/widgets_pro/arithmetics_add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-25 14:49:40.000000 oranchada-0.0.9/orangecontrib/oranchada/widgets_pro/arithmetics_subtract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-05-25 14:49:40.000000 oranchada-0.0.9/orangecontrib/oranchada/widgets_pro/find_peaks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4313 2023-05-25 14:49:40.000000 oranchada-0.0.9/orangecontrib/oranchada/widgets_pro/fit_peaks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-05-25 14:49:40.000000 oranchada-0.0.9/orangecontrib/oranchada/widgets_pro/gen_spe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-25 14:49:40.000000 oranchada-0.0.9/orangecontrib/oranchada/widgets_pro/hdr_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-25 14:49:40.000000 oranchada-0.0.9/orangecontrib/oranchada/widgets_pro/hht_sharpening.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:49:52.144660 oranchada-0.0.9/orangecontrib/oranchada/widgets_pro/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-05-25 14:49:40.000000 oranchada-0.0.9/orangecontrib/oranchada/widgets_pro/icons/CHARISMA_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-25 14:49:40.000000 oranchada-0.0.9/orangecontrib/oranchada/widgets_pro/icons/spectra.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-05-25 14:49:40.000000 oranchada-0.0.9/orangecontrib/oranchada/widgets_pro/load_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-25 14:49:40.000000 oranchada-0.0.9/orangecontrib/oranchada/widgets_pro/load_file_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-05-25 14:49:40.000000 oranchada-0.0.9/orangecontrib/oranchada/widgets_pro/load_test_spectra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-05-25 14:49:40.000000 oranchada-0.0.9/orangecontrib/oranchada/widgets_pro/merger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-05-25 14:49:40.000000 oranchada-0.0.9/orangecontrib/oranchada/widgets_pro/metadata_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-25 14:49:40.000000 oranchada-0.0.9/orangecontrib/oranchada/widgets_pro/moving_minimum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-25 14:49:40.000000 oranchada-0.0.9/orangecontrib/oranchada/widgets_pro/normalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6778 2023-05-25 14:49:40.000000 oranchada-0.0.9/orangecontrib/oranchada/widgets_pro/process_spectra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-05-25 14:49:40.000000 oranchada-0.0.9/orangecontrib/oranchada/widgets_pro/raman_shift_to_wavelength.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-05-25 14:49:40.000000 oranchada-0.0.9/orangecontrib/oranchada/widgets_pro/remove_spikes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-05-25 14:49:40.000000 oranchada-0.0.9/orangecontrib/oranchada/widgets_pro/resample_NUDFT.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-25 14:49:40.000000 oranchada-0.0.9/orangecontrib/oranchada/widgets_pro/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-05-25 14:49:40.000000 oranchada-0.0.9/orangecontrib/oranchada/widgets_pro/set_xaxis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-25 14:49:40.000000 oranchada-0.0.9/orangecontrib/oranchada/widgets_pro/wavelength_to_raman_shift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7684 2023-05-25 14:49:40.000000 oranchada-0.0.9/orangecontrib/oranchada/widgets_pro/xaxis_fine_calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 14:49:52.144660 oranchada-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4881 2023-05-25 14:49:40.000000 oranchada-0.0.9/setup.py
```

### Comparing `oranchada-0.0.8/LICENSE` & `oranchada-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `oranchada-0.0.8/PKG-INFO` & `oranchada-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oranchada
-Version: 0.0.8
+Version: 0.0.9
 Summary: Orange add-on for Raman spectroscopy
 Home-page: https://github.com/h2020charisma/oranchada
 Author: IDEAconsult Ltd.
 Author-email: dev-charisma@ideaconsult.net
 License: MIT
 Keywords: Raman,oranchada,orange3 add-on,spectroscopy
 Classifier: Development Status :: 4 - Beta
```

### Comparing `oranchada-0.0.8/README.md` & `oranchada-0.0.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -36,25 +36,26 @@
 
 1. Orange will then proceed with the installation. When ready, it will suggest to restart itself. Click **OK**.
 
     ![image](https://github.com/h2020charisma/oranchada/assets/1084155/2d300f92-559a-400f-b0ed-e5972feae3a0)
 
 1. Once Orange restarts, you should see an **Oranchada Easy** and **Pro** categories in the left panel. Click them to reveal all widgets.
 
-    ![image](https://github.com/h2020charisma/oranchada/assets/1084155/a860944f-3bbd-452e-a5fb-def9cff3bac7)
+    ![image](https://github.com/h2020charisma/oranchada/assets/1084155/329aba14-d714-4a22-95d1-6fb03ee168a2)
 
 
 ### Manual installation
 
 If your network connection has very tight security that severely restricts what sites you can access, the usual installation method via **Options** ➡️ **Add-ons** might not work for you. It may be possible to circumvent the problem by installing *oranchada* manually:
 
 1. Open https://pypi.org/project/oranchada/#files and download the "Built Distribution" `.whl` file.
 1. Open **Options** ➡️ **Add-ons** then drag & drop the downloaded `.whl` file to the add-ons window.
 1. Proceed with the general instructions above, starting from step 5 ("scroll down the list until you find **oranchada**").
 
+
 ## Updating
 
 1. Open **Options** ➡️ **Add-ons**. If there's a new version of *oranchada* or *Orange* itself, they will be listed at the top, with your installed version and the latest available one indicated (e.g. you have `0.0.6` installed and `0.0.7` is the latest available version that you can update to).
 
     ![image](https://github.com/h2020charisma/oranchada/assets/1084155/d4f6281a-4513-4b29-ac79-c907c034b54e)
 
 1. Click the box(es) next to the available updates so that a check mark appears and *Update* is displayed in the **Action** column, then click **OK**.
@@ -67,14 +68,15 @@
 
     ![image](https://github.com/h2020charisma/oranchada/assets/1084155/83e40eb7-fe70-45c9-82ce-7b42fd1a1edb)
 
     2. **IMPORTANT**: In case the upgrade fails, click **OK** and repeat the steps above—it should work on the second attempt. Do **NOT** close *Orange* here without repeating the steps! If you do this, you will most likely not be able to start *Orange* again and will have to install it anew from the beginning, possibly losing some of your settings.
 
     ![image](https://github.com/h2020charisma/oranchada/assets/1084155/78419dcc-73f7-4573-9c80-2cb738ee3f56)
 
+
 ## For developers
 
 If you would like to install from cloned git repository, run
 
     pip install .
 
 To register this add-on with Orange, but keep the code in the development
```

### Comparing `oranchada-0.0.8/oranchada.egg-info/PKG-INFO` & `oranchada-0.0.9/oranchada.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oranchada
-Version: 0.0.8
+Version: 0.0.9
 Summary: Orange add-on for Raman spectroscopy
 Home-page: https://github.com/h2020charisma/oranchada
 Author: IDEAconsult Ltd.
 Author-email: dev-charisma@ideaconsult.net
 License: MIT
 Keywords: Raman,oranchada,orange3 add-on,spectroscopy
 Classifier: Development Status :: 4 - Beta
```

### Comparing `oranchada-0.0.8/oranchada.egg-info/SOURCES.txt` & `oranchada-0.0.9/oranchada.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 orangecontrib/oranchada/processings/add_baseline.py
 orangecontrib/oranchada/processings/add_noise.py
 orangecontrib/oranchada/processings/gen_spe.py
 orangecontrib/oranchada/tests/__init__.py
 orangecontrib/oranchada/tests/process_spectra_test.py
 orangecontrib/oranchada/widgets_easy/__init__.py
 orangecontrib/oranchada/widgets_easy/gen_noisy_spe.py
+orangecontrib/oranchada/widgets_easy/icons/CHARISMA_logo.svg
 orangecontrib/oranchada/widgets_easy/icons/spectra.svg
 orangecontrib/oranchada/widgets_pro/__init__.py
 orangecontrib/oranchada/widgets_pro/add_baseline.py
 orangecontrib/oranchada/widgets_pro/add_noise.py
 orangecontrib/oranchada/widgets_pro/arithmetics_add.py
 orangecontrib/oranchada/widgets_pro/arithmetics_subtract.py
 orangecontrib/oranchada/widgets_pro/find_peaks.py
@@ -38,18 +39,20 @@
 orangecontrib/oranchada/widgets_pro/gen_spe.py
 orangecontrib/oranchada/widgets_pro/hdr_merge.py
 orangecontrib/oranchada/widgets_pro/hht_sharpening.py
 orangecontrib/oranchada/widgets_pro/load_file.py
 orangecontrib/oranchada/widgets_pro/load_file_names.py
 orangecontrib/oranchada/widgets_pro/load_test_spectra.py
 orangecontrib/oranchada/widgets_pro/merger.py
+orangecontrib/oranchada/widgets_pro/metadata_editor.py
 orangecontrib/oranchada/widgets_pro/moving_minimum.py
 orangecontrib/oranchada/widgets_pro/normalize.py
 orangecontrib/oranchada/widgets_pro/process_spectra.py
 orangecontrib/oranchada/widgets_pro/raman_shift_to_wavelength.py
 orangecontrib/oranchada/widgets_pro/remove_spikes.py
 orangecontrib/oranchada/widgets_pro/resample_NUDFT.py
 orangecontrib/oranchada/widgets_pro/select.py
 orangecontrib/oranchada/widgets_pro/set_xaxis.py
 orangecontrib/oranchada/widgets_pro/wavelength_to_raman_shift.py
 orangecontrib/oranchada/widgets_pro/xaxis_fine_calibration.py
+orangecontrib/oranchada/widgets_pro/icons/CHARISMA_logo.svg
 orangecontrib/oranchada/widgets_pro/icons/spectra.svg
```

### Comparing `oranchada-0.0.8/orangecontrib/oranchada/base_widget/filter_widget.py` & `oranchada-0.0.9/orangecontrib/oranchada/base_widget/filter_widget.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,10 +14,13 @@
 
     @Inputs.in_spe
     def set_in_spe(self, spe):
         self.should_auto_plot = False
         if spe:
             self.in_spe = spe
             self.auto_process()
+            self.info.set_input_summary(f'{len(self.in_spe)} RC2Spectra',
+                                        '\n'.join([f'· {repr(i)}' for i in self.in_spe]))
         else:
             self.in_spe = RC2Spectra()
+            self.info.set_input_summary(self.info.NoInput)
         self.input_hook()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `oranchada-0.0.8/orangecontrib/oranchada/processings/add_baseline.py` & `oranchada-0.0.9/orangecontrib/oranchada/processings/add_baseline.py`

 * *Files identical despite different names*

### Comparing `oranchada-0.0.8/orangecontrib/oranchada/processings/add_noise.py` & `oranchada-0.0.9/orangecontrib/oranchada/processings/add_noise.py`

 * *Files identical despite different names*

### Comparing `oranchada-0.0.8/orangecontrib/oranchada/processings/gen_spe.py` & `oranchada-0.0.9/orangecontrib/oranchada/processings/gen_spe.py`

 * *Files identical despite different names*

### Comparing `oranchada-0.0.8/orangecontrib/oranchada/tests/process_spectra_test.py` & `oranchada-0.0.9/orangecontrib/oranchada/tests/process_spectra_test.py`

 * *Files identical despite different names*

### Comparing `oranchada-0.0.8/orangecontrib/oranchada/widgets_easy/gen_noisy_spe.py` & `oranchada-0.0.9/orangecontrib/oranchada/widgets_easy/gen_noisy_spe.py`

 * *Files identical despite different names*

### Comparing `oranchada-0.0.8/orangecontrib/oranchada/widgets_easy/icons/spectra.svg` & `oranchada-0.0.9/orangecontrib/oranchada/widgets_easy/icons/spectra.svg`

 * *Files identical despite different names*

### Comparing `oranchada-0.0.8/orangecontrib/oranchada/widgets_pro/add_baseline.py` & `oranchada-0.0.9/orangecontrib/oranchada/widgets_pro/add_baseline.py`

 * *Files identical despite different names*

### Comparing `oranchada-0.0.8/orangecontrib/oranchada/widgets_pro/add_noise.py` & `oranchada-0.0.9/orangecontrib/oranchada/widgets_pro/add_noise.py`

 * *Files identical despite different names*

### Comparing `oranchada-0.0.8/orangecontrib/oranchada/widgets_pro/arithmetics_add.py` & `oranchada-0.0.9/orangecontrib/oranchada/widgets_pro/arithmetics_add.py`

 * *Files identical despite different names*

### Comparing `oranchada-0.0.8/orangecontrib/oranchada/widgets_pro/arithmetics_subtract.py` & `oranchada-0.0.9/orangecontrib/oranchada/widgets_pro/arithmetics_subtract.py`

 * *Files identical despite different names*

### Comparing `oranchada-0.0.8/orangecontrib/oranchada/widgets_pro/find_peaks.py` & `oranchada-0.0.9/orangecontrib/oranchada/widgets_pro/find_peaks.py`

 * *Files identical despite different names*

### Comparing `oranchada-0.0.8/orangecontrib/oranchada/widgets_pro/gen_spe.py` & `oranchada-0.0.9/orangecontrib/oranchada/widgets_pro/gen_spe.py`

 * *Files identical despite different names*

### Comparing `oranchada-0.0.8/orangecontrib/oranchada/widgets_pro/hht_sharpening.py` & `oranchada-0.0.9/orangecontrib/oranchada/widgets_pro/hht_sharpening.py`

 * *Files identical despite different names*

### Comparing `oranchada-0.0.8/orangecontrib/oranchada/widgets_pro/icons/spectra.svg` & `oranchada-0.0.9/orangecontrib/oranchada/widgets_pro/icons/spectra.svg`

 * *Files identical despite different names*

### Comparing `oranchada-0.0.8/orangecontrib/oranchada/widgets_pro/load_file.py` & `oranchada-0.0.9/orangecontrib/oranchada/widgets_pro/load_file.py`

 * *Files 12% similar despite different names*

```diff
@@ -37,14 +37,17 @@
             initialFilter=filters[-2],
             )
         if filenames:
             self.filenames = filenames
             self.auto_process()
 
     def process(self):
-        self.out_spe = [
-            rc2.spectrum.from_local_file(fname,
-                                         filetype=(self.fileformat if self.fileformat != 'Auto' else None),
-                                         )
-            for fname in self.filenames
-            ]
+        self.out_spe = []
+        for fname in self.filenames:
+            spe = rc2.spectrum.from_local_file(fname,
+                                               filetype=(self.fileformat if self.fileformat != 'Auto' else None),
+                                               )
+            meta_dct = spe.meta.dict()['__root__']
+            meta_dct['xlabel'] = 'Raman shift [cm¯¹]'
+            spe.meta = meta_dct
+            self.out_spe.append(spe)
         self.send_outputs()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `oranchada-0.0.8/orangecontrib/oranchada/widgets_pro/load_file_names.py` & `oranchada-0.0.9/orangecontrib/oranchada/widgets_pro/load_file_names.py`

 * *Files identical despite different names*

### Comparing `oranchada-0.0.8/orangecontrib/oranchada/widgets_pro/load_test_spectra.py` & `oranchada-0.0.9/orangecontrib/oranchada/widgets_pro/load_test_spectra.py`

 * *Files 6% similar despite different names*

```diff
@@ -54,9 +54,12 @@
         self.selected_filenames = [fn_item.text() for fn_item in self.list_box_filename.selectedItems()]
         self.auto_process()
 
     def process(self):
         self.out_spe = list()
         for fn in data.prepend_prefix(self.selected_filenames):
             spe = rc2.spectrum.from_local_file(fn)
+            meta_dct = spe.meta.dict()['__root__']
+            meta_dct['xlabel'] = 'Raman shift [cm¯¹]'
+            spe.meta = meta_dct
             self.out_spe.append(spe)
         self.send_outputs()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `oranchada-0.0.8/orangecontrib/oranchada/widgets_pro/merger.py` & `oranchada-0.0.9/orangecontrib/oranchada/widgets_pro/merger.py`

 * *Files identical despite different names*

### Comparing `oranchada-0.0.8/orangecontrib/oranchada/widgets_pro/moving_minimum.py` & `oranchada-0.0.9/orangecontrib/oranchada/widgets_pro/moving_minimum.py`

 * *Files identical despite different names*

### Comparing `oranchada-0.0.8/orangecontrib/oranchada/widgets_pro/normalize.py` & `oranchada-0.0.9/orangecontrib/oranchada/widgets_pro/normalize.py`

 * *Files identical despite different names*

### Comparing `oranchada-0.0.8/orangecontrib/oranchada/widgets_pro/process_spectra.py` & `oranchada-0.0.9/orangecontrib/oranchada/widgets_pro/process_spectra.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     logging.root.removeHandler(handler)
 logging.basicConfig(handlers=[logging.FileHandler("charisma.log", mode='w')], level=logging.NOTSET)
 logging.root.setLevel(logging.NOTSET)
 log = logging.getLogger("charisma")
 log.info("log hijack for debugging")
 
 
-class ProcessSpectraWidget(OWWidget):
+class ProcessSpectraWidget:  # (OWWidget):
     # Define the widget's name, category, and outputs
     name = "Process Spectra"
     description = "Process spectra provided as Orange data table"
     icon = "icons/spectra.svg"
     priority = 10
     # want_main_area = False
     # resizing_enabled = False
```

### Comparing `oranchada-0.0.8/orangecontrib/oranchada/widgets_pro/remove_spikes.py` & `oranchada-0.0.9/orangecontrib/oranchada/widgets_pro/remove_spikes.py`

 * *Files identical despite different names*

### Comparing `oranchada-0.0.8/orangecontrib/oranchada/widgets_pro/resample_NUDFT.py` & `oranchada-0.0.9/orangecontrib/oranchada/widgets_pro/resample_NUDFT.py`

 * *Files identical despite different names*

### Comparing `oranchada-0.0.8/orangecontrib/oranchada/widgets_pro/select.py` & `oranchada-0.0.9/orangecontrib/oranchada/widgets_pro/select.py`

 * *Files identical despite different names*

### Comparing `oranchada-0.0.8/orangecontrib/oranchada/widgets_pro/set_xaxis.py` & `oranchada-0.0.9/orangecontrib/oranchada/widgets_pro/set_xaxis.py`

 * *Files identical despite different names*

### Comparing `oranchada-0.0.8/orangecontrib/oranchada/widgets_pro/wavelength_to_raman_shift.py` & `oranchada-0.0.9/orangecontrib/oranchada/widgets_pro/wavelength_to_raman_shift.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from Orange.widgets import gui
 from Orange.widgets.settings import Setting
+from Orange.widgets.widget import Msg
 
 from ..base_widget import FilterWidget
 
 
 class WL2RS(FilterWidget):
     name = "WL to RS"
     description = "Wavelength to Raman shift"
@@ -13,14 +14,23 @@
 
     def __init__(self):
         super().__init__()
         box = gui.widgetBox(self.controlArea, self.name)
         gui.doubleSpin(box, self, 'laser_wl', 0, 5000, decimals=5, step=1, callback=self.auto_process,
                        label='Laser Wavelength [nm]')
 
+    class Warning(FilterWidget.Warning):
+        x_label_not_wavelength = Msg('Expected spectra with wavelengths on xaxis')
+
     def process(self):
         self.out_spe = list()
         for spe in self.in_spe:
+            if 'xlabel' in spe.meta.__root__:
+                if spe.meta['xlabel'] != 'Wavelength [nm]':
+                    self.Warning.x_label_not_wavelength()
+                meta_dct = spe.meta.dict()['__root__']
+                meta_dct['xlabel'] = 'Raman shift [cm¯¹]'
+                spe.meta = meta_dct
             self.out_spe.append(
                 spe.abs_nm_to_shift_cm_1_filter(laser_wave_length_nm=self.laser_wl)
             )
         self.send_outputs()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `oranchada-0.0.8/orangecontrib/oranchada/widgets_pro/xaxis_fine_calibration.py` & `oranchada-0.0.9/orangecontrib/oranchada/widgets_pro/xaxis_fine_calibration.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,14 +126,16 @@
         y_lb = y - yerr
         y_ub = np.mean(y_ub) + np.std(y_ub)*3
         y_lb = np.mean(y_lb) - np.std(y_lb)*3
         self.axes[2].set_ylim(y_lb, y_ub)
         self.axes[0].set_title('Before calibration')
         self.axes[1].set_title('After calibration')
         self.axes[2].set_title('Difference')
+        self.axes[2].set_xlabel(ax.get_xlabel())
+        ax.set_xlabel('')
 
     def plot_create_axes(self):
         self.axes = self.figure.subplots(nrows=3, sharex=True)
         return self.axes[1]
 
     def diff(self, spe, ref_pos):
         if isinstance(ref_pos, dict):
```

### Comparing `oranchada-0.0.8/setup.py` & `oranchada-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from os import path, walk
 
 from setuptools import find_packages, setup
 
 NAME = 'oranchada'
 
-VERSION = '0.0.8'
+VERSION = '0.0.9'
 
 DESCRIPTION = 'Orange add-on for Raman spectroscopy'
 README_FILE = path.join(path.dirname(__file__), 'README.pypi')
 LONG_DESCRIPTION = open(README_FILE, 'r', encoding='utf-8').read()
 LONG_DESCRIPTION_CONTENT_TYPE = 'text/markdown'
 URL = 'https://github.com/h2020charisma/oranchada'
 AUTHOR = 'IDEAconsult Ltd.'
@@ -38,15 +38,15 @@
 
 INSTALL_REQUIRES = [
     'Orange3>=3.31.0',
     'numpy>=1.18.0',
     'orange-canvas-core>=0.1.24',
     'orange-widget-base>=4.16.1',
     'pip>=9.0',  # same as for Orange 3.28
-    'ramanchada2~=0.0.6',
+    'ramanchada2~=0.0.7',
     'setuptools>=36.3',  # same as for Orange 3.28
     # 'AnyQt>=0.0.6',
     # 'bottleneck',
     # 'colorcet',
     # 'extranormal3 >=0.0.3',
     # 'h5py',
     # 'lmfit>=1.0.2',
```

