# Comparing `tmp/bfit-4.9.8.tar.gz` & `tmp/bfit-4.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bfit-4.9.8.tar", last modified: Sat Jul 24 16:50:28 2021, max compression
+gzip compressed data, was "bfit-4.9.9.tar", last modified: Sat Jul 24 21:22:36 2021, max compression
```

## Comparing `bfit-4.9.8.tar` & `bfit-4.9.9.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxrwxr-x   0 fuji      (1000) fuji      (1000)        0 2021-07-24 16:50:28.349630 bfit-4.9.8/
--rw-rw-r--   0 fuji      (1000) fuji      (1000)    35149 2018-09-11 20:25:17.000000 bfit-4.9.8/LICENSE
--rw-r--r--   0 fuji      (1000) fuji      (1000)      212 2021-02-02 03:05:01.000000 bfit-4.9.8/MANIFEST.in
--rw-rw-r--   0 fuji      (1000) fuji      (1000)     8784 2021-07-24 16:50:28.345630 bfit-4.9.8/PKG-INFO
--rw-rw-r--   0 fuji      (1000) fuji      (1000)     8078 2021-06-25 18:16:44.000000 bfit-4.9.8/README.md
-drwxrwxr-x   0 fuji      (1000) fuji      (1000)        0 2021-07-24 16:50:27.977628 bfit-4.9.8/bfit/
--rw-rw-r--   0 fuji      (1000) fuji      (1000)     4468 2021-07-24 16:49:48.000000 bfit-4.9.8/bfit/__init__.py
--rw-r--r--   0 fuji      (1000) fuji      (1000)       67 2020-11-24 12:50:02.000000 bfit-4.9.8/bfit/__main__.py
-drwxrwxr-x   0 fuji      (1000) fuji      (1000)        0 2021-07-24 16:50:27.997628 bfit-4.9.8/bfit/backend/
--rw-r--r--   0 fuji      (1000) fuji      (1000)     4345 2020-11-18 10:08:31.000000 bfit-4.9.8/bfit/backend/ConstrainedFunction.py
--rw-r--r--   0 fuji      (1000) fuji      (1000)    23967 2020-11-18 10:08:29.000000 bfit-4.9.8/bfit/backend/FunctionPlacer.py
--rw-rw-r--   0 fuji      (1000) fuji      (1000)     3167 2020-11-18 10:08:27.000000 bfit-4.9.8/bfit/backend/ParameterFunction.py
--rw-rw-r--   0 fuji      (1000) fuji      (1000)    15162 2021-06-23 20:31:49.000000 bfit-4.9.8/bfit/backend/PltTracker.py
--rw-r--r--   0 fuji      (1000) fuji      (1000)       98 2020-11-18 10:08:28.000000 bfit-4.9.8/bfit/backend/__init__.py
--rw-rw-r--   0 fuji      (1000) fuji      (1000)      475 2020-11-23 09:31:15.000000 bfit-4.9.8/bfit/backend/colors.py
--rw-rw-r--   0 fuji      (1000) fuji      (1000)      732 2020-11-18 10:08:30.000000 bfit-4.9.8/bfit/backend/entry_color_set.py
--rw-rw-r--   0 fuji      (1000) fuji      (1000)     9684 2021-07-24 16:15:01.000000 bfit-4.9.8/bfit/backend/fitdata.py
--rw-rw-r--   0 fuji      (1000) fuji      (1000)      267 2019-07-26 16:41:48.000000 bfit-4.9.8/bfit/backend/raise_window.py
-drwxrwxr-x   0 fuji      (1000) fuji      (1000)        0 2021-07-24 16:50:27.997628 bfit-4.9.8/bfit/data/
--rw-rw-r--   0 fuji      (1000) fuji      (1000)     5282 2018-09-07 03:00:01.000000 bfit-4.9.8/bfit/data/icon.gif
--rw-rw-r--   0 fuji      (1000) fuji      (1000)      314 2020-11-19 07:43:51.000000 bfit-4.9.8/bfit/data/nmr_antenna_data.csv
-drwxrwxr-x   0 fuji      (1000) fuji      (1000)        0 2021-07-24 16:50:28.125629 bfit-4.9.8/bfit/fitting/
-drwxrwxr-x   0 fuji      (1000) fuji      (1000)        0 2021-07-24 16:50:28.165629 bfit-4.9.8/bfit/fitting/FastNumericalIntegration_src/
--rw-rw-r--   0 fuji      (1000) fuji      (1000)    15552 2019-11-12 04:51:09.000000 bfit-4.9.8/bfit/fitting/FastNumericalIntegration_src/DEIntegrationConstants.h
--rw-rw-r--   0 fuji      (1000) fuji      (1000)     7198 2019-11-12 04:51:13.000000 bfit-4.9.8/bfit/fitting/FastNumericalIntegration_src/DEIntegrator.h
--rw-rw-r--   0 fuji      (1000) fuji      (1000)     1553 2019-09-13 17:55:54.000000 bfit-4.9.8/bfit/fitting/FastNumericalIntegration_src/integration_fns.cpp
--rw-rw-r--   0 fuji      (1000) fuji      (1000)      521 2019-09-13 17:54:27.000000 bfit-4.9.8/bfit/fitting/FastNumericalIntegration_src/integration_fns.h
--rw-r--r--   0 fuji      (1000) fuji      (1000)      292 2020-11-18 10:08:57.000000 bfit-4.9.8/bfit/fitting/__init__.py
--rw-r--r--   0 fuji      (1000) fuji      (1000)    14322 2021-02-25 19:21:01.000000 bfit-4.9.8/bfit/fitting/decay_31mg.py
--rw-r--r--   0 fuji      (1000) fuji      (1000)    17862 2021-03-16 21:15:49.000000 bfit-4.9.8/bfit/fitting/fit_bdata.py
--rw-r--r--   0 fuji      (1000) fuji      (1000)    21536 2021-07-23 19:38:20.000000 bfit-4.9.8/bfit/fitting/fitter.py
--rw-rw-r--   0 fuji      (1000) fuji      (1000)      892 2020-11-18 10:09:00.000000 bfit-4.9.8/bfit/fitting/fitter_curve_fit.py
--rw-rw-r--   0 fuji      (1000) fuji      (1000)      944 2020-11-18 10:08:59.000000 bfit-4.9.8/bfit/fitting/fitter_migrad_hesse.py
--rw-rw-r--   0 fuji      (1000) fuji      (1000)      943 2020-11-18 10:08:59.000000 bfit-4.9.8/bfit/fitting/fitter_migrad_minos.py
--rw-rw-r--   0 fuji      (1000) fuji      (1000)     8981 2021-05-14 21:33:21.000000 bfit-4.9.8/bfit/fitting/functions.py
--rw-rw-r--   0 fuji      (1000) fuji      (1000)     2834 2020-11-18 10:08:58.000000 bfit-4.9.8/bfit/fitting/global_bdata_fitter.py
--rw-rw-r--   0 fuji      (1000) fuji      (1000)    32136 2021-05-14 21:33:21.000000 bfit-4.9.8/bfit/fitting/global_fitter.py
--rw-rw-r--   0 fuji      (1000) fuji      (1000)   911070 2021-07-22 15:38:00.000000 bfit-4.9.8/bfit/fitting/integrator.cpp
--rw-rw-r--   0 fuji      (1000) fuji      (1000)     4945 2021-02-19 20:31:57.000000 bfit-4.9.8/bfit/fitting/integrator.pyx
--rw-rw-r--   0 fuji      (1000) fuji      (1000)     5742 2021-02-04 01:46:20.000000 bfit-4.9.8/bfit/fitting/leastsquares.py
--rw-rw-r--   0 fuji      (1000) fuji      (1000)    10321 2021-05-14 21:33:21.000000 bfit-4.9.8/bfit/fitting/minuit.py
-drwxrwxr-x   0 fuji      (1000) fuji      (1000)        0 2021-07-24 16:50:28.189629 bfit-4.9.8/bfit/gui/
--rw-rw-r--   0 fuji      (1000) fuji      (1000)       17 2019-02-20 23:41:35.000000 bfit-4.9.8/bfit/gui/__init__.py
--rwxrwxr-x   0 fuji      (1000) fuji      (1000)    80665 2021-07-24 16:45:25.000000 bfit-4.9.8/bfit/gui/bfit.py
--rw-rw-r--   0 fuji      (1000) fuji      (1000)     5234 2021-05-14 21:33:21.000000 bfit-4.9.8/bfit/gui/calculator_nmr_B1.py
--rw-rw-r--   0 fuji      (1000) fuji      (1000)     6973 2021-05-14 21:33:21.000000 bfit-4.9.8/bfit/gui/calculator_nmr_atten.py
--rw-rw-r--   0 fuji      (1000) fuji      (1000)     4710 2021-05-14 21:33:21.000000 bfit-4.9.8/bfit/gui/calculator_nqr_B0.py
--rw-rw-r--   0 fuji      (1000) fuji      (1000)     8420 2020-11-19 07:49:46.000000 bfit-4.9.8/bfit/gui/popup_add_param.py
--rw-rw-r--   0 fuji      (1000) fuji      (1000)    12987 2021-05-14 21:33:21.000000 bfit-4.9.8/bfit/gui/popup_deadtime.py
--rw-r--r--   0 fuji      (1000) fuji      (1000)     3325 2020-11-23 09:26:35.000000 bfit-4.9.8/bfit/gui/popup_drawstyle.py
--rw-rw-r--   0 fuji      (1000) fuji      (1000)    11992 2021-06-07 19:14:21.000000 bfit-4.9.8/bfit/gui/popup_fit_constraints.py
--rw-rw-r--   0 fuji      (1000) fuji      (1000)    10892 2021-04-23 18:56:19.000000 bfit-4.9.8/bfit/gui/popup_fit_results.py
--rw-rw-r--   0 fuji      (1000) fuji      (1000)     5127 2021-02-05 00:22:39.000000 bfit-4.9.8/bfit/gui/popup_ongoing_process.py
--rw-r--r--   0 fuji      (1000) fuji      (1000)    10481 2021-03-09 19:52:11.000000 bfit-4.9.8/bfit/gui/popup_param.py
--rw-r--r--   0 fuji      (1000) fuji      (1000)     2405 2020-11-23 09:26:33.000000 bfit-4.9.8/bfit/gui/popup_redraw_period.py
--rw-rw-r--   0 fuji      (1000) fuji      (1000)     5083 2021-05-14 21:33:21.000000 bfit-4.9.8/bfit/gui/popup_set_histograms.py
--rw-r--r--   0 fuji      (1000) fuji      (1000)     2445 2020-11-23 09:26:32.000000 bfit-4.9.8/bfit/gui/popup_set_ppm_reference.py
--rw-r--r--   0 fuji      (1000) fuji      (1000)     3937 2020-11-18 10:09:38.000000 bfit-4.9.8/bfit/gui/popup_show_param.py
--rw-r--r--   0 fuji      (1000) fuji      (1000)     2541 2020-11-18 13:55:18.000000 bfit-4.9.8/bfit/gui/popup_terminal.py
--rw-rw-r--   0 fuji      (1000) fuji      (1000)     3443 2021-06-07 19:14:21.000000 bfit-4.9.8/bfit/gui/popup_units.py
--rw-rw-r--   0 fuji      (1000) fuji      (1000)    48231 2021-05-14 21:33:21.000000 bfit-4.9.8/bfit/gui/tab_fetch_files.py
--rw-rw-r--   0 fuji      (1000) fuji      (1000)    54464 2021-07-24 16:34:21.000000 bfit-4.9.8/bfit/gui/tab_fileviewer.py
--rw-rw-r--   0 fuji      (1000) fuji      (1000)   106724 2021-07-24 16:43:30.000000 bfit-4.9.8/bfit/gui/tab_fit_files.py
--rw-r--r--   0 fuji      (1000) fuji      (1000)    13796 2021-05-07 20:22:56.000000 bfit-4.9.8/bfit/gui/template_fit_popup.py
-drwxrwxr-x   0 fuji      (1000) fuji      (1000)        0 2021-07-24 16:50:28.337630 bfit-4.9.8/bfit/test/
--rw-rw-r--   0 fuji      (1000) fuji      (1000)       13 2021-02-03 18:53:47.000000 bfit-4.9.8/bfit/test/__init__.py
--rw-rw-r--   0 fuji      (1000) fuji      (1000)      782 2021-05-14 21:33:21.000000 bfit-4.9.8/bfit/test/test_calculator_nmr_B1.py
--rw-rw-r--   0 fuji      (1000) fuji      (1000)     1192 2021-05-14 21:33:21.000000 bfit-4.9.8/bfit/test/test_calculator_nmr_atten.py
--rw-rw-r--   0 fuji      (1000) fuji      (1000)      834 2021-05-14 21:33:21.000000 bfit-4.9.8/bfit/test/test_calculator_nqr_B0.py
--rw-rw-r--   0 fuji      (1000) fuji      (1000)     4596 2021-06-07 19:14:21.000000 bfit-4.9.8/bfit/test/test_constrained_fit.py
--rw-rw-r--   0 fuji      (1000) fuji      (1000)     2369 2021-05-14 21:33:21.000000 bfit-4.9.8/bfit/test/test_deadtime.py
--rw-rw-r--   0 fuji      (1000) fuji      (1000)     4110 2021-05-14 21:33:21.000000 bfit-4.9.8/bfit/test/test_export_data.py
--rw-rw-r--   0 fuji      (1000) fuji      (1000)     4042 2021-05-14 21:33:21.000000 bfit-4.9.8/bfit/test/test_export_fits.py
--rw-rw-r--   0 fuji      (1000) fuji      (1000)     7032 2021-05-14 21:33:21.000000 bfit-4.9.8/bfit/test/test_export_param.py
--rw-rw-r--   0 fuji      (1000) fuji      (1000)     1463 2021-05-14 21:33:21.000000 bfit-4.9.8/bfit/test/test_fit_model.py
--rw-rw-r--   0 fuji      (1000) fuji      (1000)     5231 2021-05-14 21:33:21.000000 bfit-4.9.8/bfit/test/test_functions.py
--rw-rw-r--   0 fuji      (1000) fuji      (1000)     6124 2021-05-14 21:33:21.000000 bfit-4.9.8/bfit/test/test_global_fitter.py
--rw-rw-r--   0 fuji      (1000) fuji      (1000)     2944 2021-05-14 21:33:21.000000 bfit-4.9.8/bfit/test/test_leastsquares.py
--rw-rw-r--   0 fuji      (1000) fuji      (1000)     3900 2021-05-14 21:33:21.000000 bfit-4.9.8/bfit/test/test_minuit.py
--rw-rw-r--   0 fuji      (1000) fuji      (1000)     4415 2021-05-14 21:33:21.000000 bfit-4.9.8/bfit/test/test_numeric_integration.py
--rw-rw-r--   0 fuji      (1000) fuji      (1000)     6150 2021-05-14 21:33:21.000000 bfit-4.9.8/bfit/test/test_save_load_state.py
--rw-rw-r--   0 fuji      (1000) fuji      (1000)     4812 2021-06-07 19:14:21.000000 bfit-4.9.8/bfit/test/test_tab1_fileviewer.py
--rw-rw-r--   0 fuji      (1000) fuji      (1000)     3891 2021-05-14 21:33:21.000000 bfit-4.9.8/bfit/test/test_tab2_fetch_files.py
--rw-rw-r--   0 fuji      (1000) fuji      (1000)    14127 2021-05-14 21:33:21.000000 bfit-4.9.8/bfit/test/test_tab3_fit_files.py
--rw-rw-r--   0 fuji      (1000) fuji      (1000)     2390 2021-06-07 19:14:21.000000 bfit-4.9.8/bfit/test/test_units.py
-drwxrwxr-x   0 fuji      (1000) fuji      (1000)        0 2021-07-24 16:50:27.981628 bfit-4.9.8/bfit.egg-info/
--rw-r--r--   0 fuji      (1000) fuji      (1000)     8784 2021-07-24 16:50:27.000000 bfit-4.9.8/bfit.egg-info/PKG-INFO
--rw-r--r--   0 fuji      (1000) fuji      (1000)     2527 2021-07-24 16:50:27.000000 bfit-4.9.8/bfit.egg-info/SOURCES.txt
--rw-r--r--   0 fuji      (1000) fuji      (1000)        1 2021-07-24 16:50:27.000000 bfit-4.9.8/bfit.egg-info/dependency_links.txt
--rw-r--r--   0 fuji      (1000) fuji      (1000)       36 2021-07-24 16:50:27.000000 bfit-4.9.8/bfit.egg-info/entry_points.txt
--rw-r--r--   0 fuji      (1000) fuji      (1000)      172 2021-07-24 16:50:27.000000 bfit-4.9.8/bfit.egg-info/requires.txt
--rw-r--r--   0 fuji      (1000) fuji      (1000)        5 2021-07-24 16:50:27.000000 bfit-4.9.8/bfit.egg-info/top_level.txt
--rw-rw-r--   0 fuji      (1000) fuji      (1000)       38 2021-07-24 16:50:28.349630 bfit-4.9.8/setup.cfg
--rw-rw-r--   0 fuji      (1000) fuji      (1000)     1981 2021-07-24 16:49:55.000000 bfit-4.9.8/setup.py
+drwxrwxr-x   0 fuji      (1000) fuji      (1000)        0 2021-07-24 21:22:36.512224 bfit-4.9.9/
+-rw-rw-r--   0 fuji      (1000) fuji      (1000)    35149 2018-09-11 20:25:17.000000 bfit-4.9.9/LICENSE
+-rw-r--r--   0 fuji      (1000) fuji      (1000)      212 2021-02-02 03:05:01.000000 bfit-4.9.9/MANIFEST.in
+-rw-rw-r--   0 fuji      (1000) fuji      (1000)     8784 2021-07-24 21:22:36.512224 bfit-4.9.9/PKG-INFO
+-rw-rw-r--   0 fuji      (1000) fuji      (1000)     8078 2021-06-25 18:16:44.000000 bfit-4.9.9/README.md
+drwxrwxr-x   0 fuji      (1000) fuji      (1000)        0 2021-07-24 21:22:36.504223 bfit-4.9.9/bfit/
+-rw-rw-r--   0 fuji      (1000) fuji      (1000)     4468 2021-07-24 21:22:00.000000 bfit-4.9.9/bfit/__init__.py
+-rw-r--r--   0 fuji      (1000) fuji      (1000)       67 2020-11-24 12:50:02.000000 bfit-4.9.9/bfit/__main__.py
+drwxrwxr-x   0 fuji      (1000) fuji      (1000)        0 2021-07-24 21:22:36.508224 bfit-4.9.9/bfit/backend/
+-rw-r--r--   0 fuji      (1000) fuji      (1000)     4345 2020-11-18 10:08:31.000000 bfit-4.9.9/bfit/backend/ConstrainedFunction.py
+-rw-r--r--   0 fuji      (1000) fuji      (1000)    23967 2020-11-18 10:08:29.000000 bfit-4.9.9/bfit/backend/FunctionPlacer.py
+-rw-rw-r--   0 fuji      (1000) fuji      (1000)     3167 2020-11-18 10:08:27.000000 bfit-4.9.9/bfit/backend/ParameterFunction.py
+-rw-rw-r--   0 fuji      (1000) fuji      (1000)    15162 2021-06-23 20:31:49.000000 bfit-4.9.9/bfit/backend/PltTracker.py
+-rw-r--r--   0 fuji      (1000) fuji      (1000)       98 2020-11-18 10:08:28.000000 bfit-4.9.9/bfit/backend/__init__.py
+-rw-rw-r--   0 fuji      (1000) fuji      (1000)      475 2020-11-23 09:31:15.000000 bfit-4.9.9/bfit/backend/colors.py
+-rw-rw-r--   0 fuji      (1000) fuji      (1000)      732 2020-11-18 10:08:30.000000 bfit-4.9.9/bfit/backend/entry_color_set.py
+-rw-rw-r--   0 fuji      (1000) fuji      (1000)     9684 2021-07-24 16:15:01.000000 bfit-4.9.9/bfit/backend/fitdata.py
+-rw-rw-r--   0 fuji      (1000) fuji      (1000)      267 2019-07-26 16:41:48.000000 bfit-4.9.9/bfit/backend/raise_window.py
+drwxrwxr-x   0 fuji      (1000) fuji      (1000)        0 2021-07-24 21:22:36.508224 bfit-4.9.9/bfit/data/
+-rw-rw-r--   0 fuji      (1000) fuji      (1000)     5282 2018-09-07 03:00:01.000000 bfit-4.9.9/bfit/data/icon.gif
+-rw-rw-r--   0 fuji      (1000) fuji      (1000)      314 2020-11-19 07:43:51.000000 bfit-4.9.9/bfit/data/nmr_antenna_data.csv
+drwxrwxr-x   0 fuji      (1000) fuji      (1000)        0 2021-07-24 21:22:36.508224 bfit-4.9.9/bfit/fitting/
+drwxrwxr-x   0 fuji      (1000) fuji      (1000)        0 2021-07-24 21:22:36.508224 bfit-4.9.9/bfit/fitting/FastNumericalIntegration_src/
+-rw-rw-r--   0 fuji      (1000) fuji      (1000)    15552 2019-11-12 04:51:09.000000 bfit-4.9.9/bfit/fitting/FastNumericalIntegration_src/DEIntegrationConstants.h
+-rw-rw-r--   0 fuji      (1000) fuji      (1000)     7198 2019-11-12 04:51:13.000000 bfit-4.9.9/bfit/fitting/FastNumericalIntegration_src/DEIntegrator.h
+-rw-rw-r--   0 fuji      (1000) fuji      (1000)     1553 2019-09-13 17:55:54.000000 bfit-4.9.9/bfit/fitting/FastNumericalIntegration_src/integration_fns.cpp
+-rw-rw-r--   0 fuji      (1000) fuji      (1000)      521 2019-09-13 17:54:27.000000 bfit-4.9.9/bfit/fitting/FastNumericalIntegration_src/integration_fns.h
+-rw-r--r--   0 fuji      (1000) fuji      (1000)      292 2020-11-18 10:08:57.000000 bfit-4.9.9/bfit/fitting/__init__.py
+-rw-r--r--   0 fuji      (1000) fuji      (1000)    14322 2021-02-25 19:21:01.000000 bfit-4.9.9/bfit/fitting/decay_31mg.py
+-rw-r--r--   0 fuji      (1000) fuji      (1000)    17862 2021-03-16 21:15:49.000000 bfit-4.9.9/bfit/fitting/fit_bdata.py
+-rw-r--r--   0 fuji      (1000) fuji      (1000)    21536 2021-07-23 19:38:20.000000 bfit-4.9.9/bfit/fitting/fitter.py
+-rw-rw-r--   0 fuji      (1000) fuji      (1000)      892 2020-11-18 10:09:00.000000 bfit-4.9.9/bfit/fitting/fitter_curve_fit.py
+-rw-rw-r--   0 fuji      (1000) fuji      (1000)      944 2020-11-18 10:08:59.000000 bfit-4.9.9/bfit/fitting/fitter_migrad_hesse.py
+-rw-rw-r--   0 fuji      (1000) fuji      (1000)      943 2020-11-18 10:08:59.000000 bfit-4.9.9/bfit/fitting/fitter_migrad_minos.py
+-rw-rw-r--   0 fuji      (1000) fuji      (1000)     8981 2021-05-14 21:33:21.000000 bfit-4.9.9/bfit/fitting/functions.py
+-rw-rw-r--   0 fuji      (1000) fuji      (1000)     2834 2020-11-18 10:08:58.000000 bfit-4.9.9/bfit/fitting/global_bdata_fitter.py
+-rw-rw-r--   0 fuji      (1000) fuji      (1000)    32136 2021-05-14 21:33:21.000000 bfit-4.9.9/bfit/fitting/global_fitter.py
+-rw-rw-r--   0 fuji      (1000) fuji      (1000)   911070 2021-07-22 15:38:00.000000 bfit-4.9.9/bfit/fitting/integrator.cpp
+-rw-rw-r--   0 fuji      (1000) fuji      (1000)     4945 2021-02-19 20:31:57.000000 bfit-4.9.9/bfit/fitting/integrator.pyx
+-rw-rw-r--   0 fuji      (1000) fuji      (1000)     5742 2021-02-04 01:46:20.000000 bfit-4.9.9/bfit/fitting/leastsquares.py
+-rw-rw-r--   0 fuji      (1000) fuji      (1000)    10321 2021-05-14 21:33:21.000000 bfit-4.9.9/bfit/fitting/minuit.py
+drwxrwxr-x   0 fuji      (1000) fuji      (1000)        0 2021-07-24 21:22:36.512224 bfit-4.9.9/bfit/gui/
+-rw-rw-r--   0 fuji      (1000) fuji      (1000)       17 2019-02-20 23:41:35.000000 bfit-4.9.9/bfit/gui/__init__.py
+-rwxrwxr-x   0 fuji      (1000) fuji      (1000)    80665 2021-07-24 16:45:25.000000 bfit-4.9.9/bfit/gui/bfit.py
+-rw-rw-r--   0 fuji      (1000) fuji      (1000)     5234 2021-05-14 21:33:21.000000 bfit-4.9.9/bfit/gui/calculator_nmr_B1.py
+-rw-rw-r--   0 fuji      (1000) fuji      (1000)     6973 2021-05-14 21:33:21.000000 bfit-4.9.9/bfit/gui/calculator_nmr_atten.py
+-rw-rw-r--   0 fuji      (1000) fuji      (1000)     4710 2021-05-14 21:33:21.000000 bfit-4.9.9/bfit/gui/calculator_nqr_B0.py
+-rw-rw-r--   0 fuji      (1000) fuji      (1000)     8420 2020-11-19 07:49:46.000000 bfit-4.9.9/bfit/gui/popup_add_param.py
+-rw-rw-r--   0 fuji      (1000) fuji      (1000)    12987 2021-05-14 21:33:21.000000 bfit-4.9.9/bfit/gui/popup_deadtime.py
+-rw-r--r--   0 fuji      (1000) fuji      (1000)     3325 2020-11-23 09:26:35.000000 bfit-4.9.9/bfit/gui/popup_drawstyle.py
+-rw-rw-r--   0 fuji      (1000) fuji      (1000)    11992 2021-06-07 19:14:21.000000 bfit-4.9.9/bfit/gui/popup_fit_constraints.py
+-rw-rw-r--   0 fuji      (1000) fuji      (1000)    10892 2021-04-23 18:56:19.000000 bfit-4.9.9/bfit/gui/popup_fit_results.py
+-rw-rw-r--   0 fuji      (1000) fuji      (1000)     5127 2021-02-05 00:22:39.000000 bfit-4.9.9/bfit/gui/popup_ongoing_process.py
+-rw-r--r--   0 fuji      (1000) fuji      (1000)    10481 2021-03-09 19:52:11.000000 bfit-4.9.9/bfit/gui/popup_param.py
+-rw-r--r--   0 fuji      (1000) fuji      (1000)     2405 2020-11-23 09:26:33.000000 bfit-4.9.9/bfit/gui/popup_redraw_period.py
+-rw-rw-r--   0 fuji      (1000) fuji      (1000)     5083 2021-05-14 21:33:21.000000 bfit-4.9.9/bfit/gui/popup_set_histograms.py
+-rw-r--r--   0 fuji      (1000) fuji      (1000)     2445 2020-11-23 09:26:32.000000 bfit-4.9.9/bfit/gui/popup_set_ppm_reference.py
+-rw-r--r--   0 fuji      (1000) fuji      (1000)     3937 2020-11-18 10:09:38.000000 bfit-4.9.9/bfit/gui/popup_show_param.py
+-rw-r--r--   0 fuji      (1000) fuji      (1000)     2541 2020-11-18 13:55:18.000000 bfit-4.9.9/bfit/gui/popup_terminal.py
+-rw-rw-r--   0 fuji      (1000) fuji      (1000)     3443 2021-06-07 19:14:21.000000 bfit-4.9.9/bfit/gui/popup_units.py
+-rw-rw-r--   0 fuji      (1000) fuji      (1000)    48231 2021-05-14 21:33:21.000000 bfit-4.9.9/bfit/gui/tab_fetch_files.py
+-rw-rw-r--   0 fuji      (1000) fuji      (1000)    54680 2021-07-24 20:30:11.000000 bfit-4.9.9/bfit/gui/tab_fileviewer.py
+-rw-rw-r--   0 fuji      (1000) fuji      (1000)   106724 2021-07-24 16:43:30.000000 bfit-4.9.9/bfit/gui/tab_fit_files.py
+-rw-r--r--   0 fuji      (1000) fuji      (1000)    13796 2021-05-07 20:22:56.000000 bfit-4.9.9/bfit/gui/template_fit_popup.py
+drwxrwxr-x   0 fuji      (1000) fuji      (1000)        0 2021-07-24 21:22:36.512224 bfit-4.9.9/bfit/test/
+-rw-rw-r--   0 fuji      (1000) fuji      (1000)       13 2021-02-03 18:53:47.000000 bfit-4.9.9/bfit/test/__init__.py
+-rw-rw-r--   0 fuji      (1000) fuji      (1000)      782 2021-05-14 21:33:21.000000 bfit-4.9.9/bfit/test/test_calculator_nmr_B1.py
+-rw-rw-r--   0 fuji      (1000) fuji      (1000)     1192 2021-05-14 21:33:21.000000 bfit-4.9.9/bfit/test/test_calculator_nmr_atten.py
+-rw-rw-r--   0 fuji      (1000) fuji      (1000)      834 2021-05-14 21:33:21.000000 bfit-4.9.9/bfit/test/test_calculator_nqr_B0.py
+-rw-rw-r--   0 fuji      (1000) fuji      (1000)     4596 2021-06-07 19:14:21.000000 bfit-4.9.9/bfit/test/test_constrained_fit.py
+-rw-rw-r--   0 fuji      (1000) fuji      (1000)     2369 2021-05-14 21:33:21.000000 bfit-4.9.9/bfit/test/test_deadtime.py
+-rw-rw-r--   0 fuji      (1000) fuji      (1000)     4110 2021-05-14 21:33:21.000000 bfit-4.9.9/bfit/test/test_export_data.py
+-rw-rw-r--   0 fuji      (1000) fuji      (1000)     4042 2021-05-14 21:33:21.000000 bfit-4.9.9/bfit/test/test_export_fits.py
+-rw-rw-r--   0 fuji      (1000) fuji      (1000)     7032 2021-05-14 21:33:21.000000 bfit-4.9.9/bfit/test/test_export_param.py
+-rw-rw-r--   0 fuji      (1000) fuji      (1000)     1463 2021-05-14 21:33:21.000000 bfit-4.9.9/bfit/test/test_fit_model.py
+-rw-rw-r--   0 fuji      (1000) fuji      (1000)     5231 2021-05-14 21:33:21.000000 bfit-4.9.9/bfit/test/test_functions.py
+-rw-rw-r--   0 fuji      (1000) fuji      (1000)     6124 2021-05-14 21:33:21.000000 bfit-4.9.9/bfit/test/test_global_fitter.py
+-rw-rw-r--   0 fuji      (1000) fuji      (1000)     2944 2021-05-14 21:33:21.000000 bfit-4.9.9/bfit/test/test_leastsquares.py
+-rw-rw-r--   0 fuji      (1000) fuji      (1000)     3900 2021-05-14 21:33:21.000000 bfit-4.9.9/bfit/test/test_minuit.py
+-rw-rw-r--   0 fuji      (1000) fuji      (1000)     4415 2021-05-14 21:33:21.000000 bfit-4.9.9/bfit/test/test_numeric_integration.py
+-rw-rw-r--   0 fuji      (1000) fuji      (1000)     6150 2021-05-14 21:33:21.000000 bfit-4.9.9/bfit/test/test_save_load_state.py
+-rw-rw-r--   0 fuji      (1000) fuji      (1000)     4812 2021-06-07 19:14:21.000000 bfit-4.9.9/bfit/test/test_tab1_fileviewer.py
+-rw-rw-r--   0 fuji      (1000) fuji      (1000)     3891 2021-05-14 21:33:21.000000 bfit-4.9.9/bfit/test/test_tab2_fetch_files.py
+-rw-rw-r--   0 fuji      (1000) fuji      (1000)    14127 2021-05-14 21:33:21.000000 bfit-4.9.9/bfit/test/test_tab3_fit_files.py
+-rw-rw-r--   0 fuji      (1000) fuji      (1000)     2390 2021-06-07 19:14:21.000000 bfit-4.9.9/bfit/test/test_units.py
+drwxrwxr-x   0 fuji      (1000) fuji      (1000)        0 2021-07-24 21:22:36.504223 bfit-4.9.9/bfit.egg-info/
+-rw-r--r--   0 fuji      (1000) fuji      (1000)     8784 2021-07-24 21:22:36.000000 bfit-4.9.9/bfit.egg-info/PKG-INFO
+-rw-r--r--   0 fuji      (1000) fuji      (1000)     2527 2021-07-24 21:22:36.000000 bfit-4.9.9/bfit.egg-info/SOURCES.txt
+-rw-r--r--   0 fuji      (1000) fuji      (1000)        1 2021-07-24 21:22:36.000000 bfit-4.9.9/bfit.egg-info/dependency_links.txt
+-rw-r--r--   0 fuji      (1000) fuji      (1000)       36 2021-07-24 21:22:36.000000 bfit-4.9.9/bfit.egg-info/entry_points.txt
+-rw-r--r--   0 fuji      (1000) fuji      (1000)      172 2021-07-24 21:22:36.000000 bfit-4.9.9/bfit.egg-info/requires.txt
+-rw-r--r--   0 fuji      (1000) fuji      (1000)        5 2021-07-24 21:22:36.000000 bfit-4.9.9/bfit.egg-info/top_level.txt
+-rw-rw-r--   0 fuji      (1000) fuji      (1000)       38 2021-07-24 21:22:36.512224 bfit-4.9.9/setup.cfg
+-rw-rw-r--   0 fuji      (1000) fuji      (1000)     1981 2021-07-24 21:22:10.000000 bfit-4.9.9/setup.py
```

### Comparing `bfit-4.9.8/LICENSE` & `bfit-4.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `bfit-4.9.8/PKG-INFO` & `bfit-4.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bfit
-Version: 4.9.8
+Version: 4.9.9
 Summary: β-NMR and β-NQR Data Analysis
 Home-page: https://github.com/dfujim/bfit
 Author: Derek Fujimoto
 Author-email: fujimoto@phas.ubc.ca
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bfit Version: 4.9.8 Summary: Î²-NMR and Î²-NQR Data
+Metadata-Version: 2.1 Name: bfit Version: 4.9.9 Summary: Î²-NMR and Î²-NQR Data
 Analysis Home-page: https://github.com/dfujim/bfit Author: Derek Fujimoto
 Author-email: fujimoto@phas.ubc.ca License: UNKNOWN Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Cython Classifier: License :: OSI Approved
 :: GNU Lesser General Public License v3 (LGPLv3) Classifier: Operating System
 :: POSIX :: Linux Classifier: Operating System :: MacOS Classifier: Development
```

### Comparing `bfit-4.9.8/README.md` & `bfit-4.9.9/README.md`

 * *Files identical despite different names*

### Comparing `bfit-4.9.8/bfit/__init__.py` & `bfit-4.9.9/bfit/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import logging, os, sys, argparse, subprocess, requests, json, code
 from logging.handlers import RotatingFileHandler
 from textwrap import dedent
 from pkg_resources import parse_version 
 from tkinter import messagebox
 
 __all__ = ['gui','fitting','backend','test']
-__version__ = '4.9.8'
+__version__ = '4.9.9'
 __author__ = 'Derek Fujimoto'
 logger_name = 'bfit'
 icon_path = os.path.join(os.path.dirname(__file__),'data','icon.gif')
 
 __all__.extend(("lorentzian", 
                 "bilorentzian", 
                 "gaussian",
```

### Comparing `bfit-4.9.8/bfit/backend/ConstrainedFunction.py` & `bfit-4.9.9/bfit/backend/ConstrainedFunction.py`

 * *Files identical despite different names*

### Comparing `bfit-4.9.8/bfit/backend/FunctionPlacer.py` & `bfit-4.9.9/bfit/backend/FunctionPlacer.py`

 * *Files identical despite different names*

### Comparing `bfit-4.9.8/bfit/backend/ParameterFunction.py` & `bfit-4.9.9/bfit/backend/ParameterFunction.py`

 * *Files identical despite different names*

### Comparing `bfit-4.9.8/bfit/backend/PltTracker.py` & `bfit-4.9.9/bfit/backend/PltTracker.py`

 * *Files identical despite different names*

### Comparing `bfit-4.9.8/bfit/backend/entry_color_set.py` & `bfit-4.9.9/bfit/backend/entry_color_set.py`

 * *Files identical despite different names*

### Comparing `bfit-4.9.8/bfit/backend/fitdata.py` & `bfit-4.9.9/bfit/backend/fitdata.py`

 * *Files identical despite different names*

### Comparing `bfit-4.9.8/bfit/data/icon.gif` & `bfit-4.9.9/bfit/data/icon.gif`

 * *Files identical despite different names*

### Comparing `bfit-4.9.8/bfit/fitting/FastNumericalIntegration_src/DEIntegrationConstants.h` & `bfit-4.9.9/bfit/fitting/FastNumericalIntegration_src/DEIntegrationConstants.h`

 * *Files identical despite different names*

### Comparing `bfit-4.9.8/bfit/fitting/FastNumericalIntegration_src/DEIntegrator.h` & `bfit-4.9.9/bfit/fitting/FastNumericalIntegration_src/DEIntegrator.h`

 * *Files identical despite different names*

### Comparing `bfit-4.9.8/bfit/fitting/FastNumericalIntegration_src/integration_fns.cpp` & `bfit-4.9.9/bfit/fitting/FastNumericalIntegration_src/integration_fns.cpp`

 * *Files identical despite different names*

### Comparing `bfit-4.9.8/bfit/fitting/FastNumericalIntegration_src/integration_fns.h` & `bfit-4.9.9/bfit/fitting/FastNumericalIntegration_src/integration_fns.h`

 * *Files identical despite different names*

### Comparing `bfit-4.9.8/bfit/fitting/decay_31mg.py` & `bfit-4.9.9/bfit/fitting/decay_31mg.py`

 * *Files identical despite different names*

### Comparing `bfit-4.9.8/bfit/fitting/fit_bdata.py` & `bfit-4.9.9/bfit/fitting/fit_bdata.py`

 * *Files identical despite different names*

### Comparing `bfit-4.9.8/bfit/fitting/fitter.py` & `bfit-4.9.9/bfit/fitting/fitter.py`

 * *Files identical despite different names*

### Comparing `bfit-4.9.8/bfit/fitting/fitter_curve_fit.py` & `bfit-4.9.9/bfit/fitting/fitter_curve_fit.py`

 * *Files identical despite different names*

### Comparing `bfit-4.9.8/bfit/fitting/fitter_migrad_hesse.py` & `bfit-4.9.9/bfit/fitting/fitter_migrad_hesse.py`

 * *Files identical despite different names*

### Comparing `bfit-4.9.8/bfit/fitting/fitter_migrad_minos.py` & `bfit-4.9.9/bfit/fitting/fitter_migrad_minos.py`

 * *Files identical despite different names*

### Comparing `bfit-4.9.8/bfit/fitting/functions.py` & `bfit-4.9.9/bfit/fitting/functions.py`

 * *Files identical despite different names*

### Comparing `bfit-4.9.8/bfit/fitting/global_bdata_fitter.py` & `bfit-4.9.9/bfit/fitting/global_bdata_fitter.py`

 * *Files identical despite different names*

### Comparing `bfit-4.9.8/bfit/fitting/global_fitter.py` & `bfit-4.9.9/bfit/fitting/global_fitter.py`

 * *Files identical despite different names*

### Comparing `bfit-4.9.8/bfit/fitting/integrator.cpp` & `bfit-4.9.9/bfit/fitting/integrator.cpp`

 * *Files identical despite different names*

### Comparing `bfit-4.9.8/bfit/fitting/integrator.pyx` & `bfit-4.9.9/bfit/fitting/integrator.pyx`

 * *Files identical despite different names*

### Comparing `bfit-4.9.8/bfit/fitting/leastsquares.py` & `bfit-4.9.9/bfit/fitting/leastsquares.py`

 * *Files identical despite different names*

### Comparing `bfit-4.9.8/bfit/fitting/minuit.py` & `bfit-4.9.9/bfit/fitting/minuit.py`

 * *Files identical despite different names*

### Comparing `bfit-4.9.8/bfit/gui/bfit.py` & `bfit-4.9.9/bfit/gui/bfit.py`

 * *Files identical despite different names*

### Comparing `bfit-4.9.8/bfit/gui/calculator_nmr_B1.py` & `bfit-4.9.9/bfit/gui/calculator_nmr_B1.py`

 * *Files identical despite different names*

### Comparing `bfit-4.9.8/bfit/gui/calculator_nmr_atten.py` & `bfit-4.9.9/bfit/gui/calculator_nmr_atten.py`

 * *Files identical despite different names*

### Comparing `bfit-4.9.8/bfit/gui/calculator_nqr_B0.py` & `bfit-4.9.9/bfit/gui/calculator_nqr_B0.py`

 * *Files identical despite different names*

### Comparing `bfit-4.9.8/bfit/gui/popup_add_param.py` & `bfit-4.9.9/bfit/gui/popup_add_param.py`

 * *Files identical despite different names*

### Comparing `bfit-4.9.8/bfit/gui/popup_deadtime.py` & `bfit-4.9.9/bfit/gui/popup_deadtime.py`

 * *Files identical despite different names*

### Comparing `bfit-4.9.8/bfit/gui/popup_drawstyle.py` & `bfit-4.9.9/bfit/gui/popup_drawstyle.py`

 * *Files identical despite different names*

### Comparing `bfit-4.9.8/bfit/gui/popup_fit_constraints.py` & `bfit-4.9.9/bfit/gui/popup_fit_constraints.py`

 * *Files identical despite different names*

### Comparing `bfit-4.9.8/bfit/gui/popup_fit_results.py` & `bfit-4.9.9/bfit/gui/popup_fit_results.py`

 * *Files identical despite different names*

### Comparing `bfit-4.9.8/bfit/gui/popup_ongoing_process.py` & `bfit-4.9.9/bfit/gui/popup_ongoing_process.py`

 * *Files identical despite different names*

### Comparing `bfit-4.9.8/bfit/gui/popup_param.py` & `bfit-4.9.9/bfit/gui/popup_param.py`

 * *Files identical despite different names*

### Comparing `bfit-4.9.8/bfit/gui/popup_redraw_period.py` & `bfit-4.9.9/bfit/gui/popup_redraw_period.py`

 * *Files identical despite different names*

### Comparing `bfit-4.9.8/bfit/gui/popup_set_histograms.py` & `bfit-4.9.9/bfit/gui/popup_set_histograms.py`

 * *Files identical despite different names*

### Comparing `bfit-4.9.8/bfit/gui/popup_set_ppm_reference.py` & `bfit-4.9.9/bfit/gui/popup_set_ppm_reference.py`

 * *Files identical despite different names*

### Comparing `bfit-4.9.8/bfit/gui/popup_show_param.py` & `bfit-4.9.9/bfit/gui/popup_show_param.py`

 * *Files identical despite different names*

### Comparing `bfit-4.9.8/bfit/gui/popup_terminal.py` & `bfit-4.9.9/bfit/gui/popup_terminal.py`

 * *Files identical despite different names*

### Comparing `bfit-4.9.8/bfit/gui/popup_units.py` & `bfit-4.9.9/bfit/gui/popup_units.py`

 * *Files identical despite different names*

### Comparing `bfit-4.9.8/bfit/gui/tab_fetch_files.py` & `bfit-4.9.9/bfit/gui/tab_fetch_files.py`

 * *Files identical despite different names*

### Comparing `bfit-4.9.8/bfit/gui/tab_fileviewer.py` & `bfit-4.9.9/bfit/gui/tab_fileviewer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1432,15 +1432,20 @@
                     return 
             else:
                 current_run2 = current_run
                 
             # update only in stack mode
             draw_style = self.bfit.draw_style.get()
             self.bfit.draw_style.set('stack')
-            self.bfit.plt.autoscale('periodic', False)
+            
+            # don't update figure limits
+            if self.data.mode in ('20', '2h'):
+                self.bfit.plt.autoscale('periodic', False)
+                
+            # draw
             self.draw(figstyle='periodic', quiet=True)
             draw_style = self.bfit.draw_style.set(draw_style)
             
             # reset year and run 
             do_quiet = (current_run2 != run) or (current_year != year)
             
             self.year.set(current_year)
@@ -1459,14 +1464,16 @@
         else:
             # check if window already removed 
             if self.bfit.plt.active['periodic'] != 0:
                 
                 # remove window
                 fig = self.bfit.plt.gcf('periodic')
                 fig.canvas.manager.set_window_title('Figure %d (Inspect)'%fig.number)
+                
+                self.bfit.plt.autoscale('periodic', True)
                 del self.bfit.plt.plots['periodic'][0]
                 self.bfit.plt.active['periodic'] = 0
             
 # =========================================================================== #
 def num_prefix(val):
     if val > 1e9: return (val/1e9, 'G')
     if val > 1e6: return (val/1e6, 'M')
```

### Comparing `bfit-4.9.8/bfit/gui/tab_fit_files.py` & `bfit-4.9.9/bfit/gui/tab_fit_files.py`

 * *Files identical despite different names*

### Comparing `bfit-4.9.8/bfit/gui/template_fit_popup.py` & `bfit-4.9.9/bfit/gui/template_fit_popup.py`

 * *Files identical despite different names*

### Comparing `bfit-4.9.8/bfit/test/test_calculator_nmr_B1.py` & `bfit-4.9.9/bfit/test/test_calculator_nmr_B1.py`

 * *Files identical despite different names*

### Comparing `bfit-4.9.8/bfit/test/test_calculator_nmr_atten.py` & `bfit-4.9.9/bfit/test/test_calculator_nmr_atten.py`

 * *Files identical despite different names*

### Comparing `bfit-4.9.8/bfit/test/test_calculator_nqr_B0.py` & `bfit-4.9.9/bfit/test/test_calculator_nqr_B0.py`

 * *Files identical despite different names*

### Comparing `bfit-4.9.8/bfit/test/test_constrained_fit.py` & `bfit-4.9.9/bfit/test/test_constrained_fit.py`

 * *Files identical despite different names*

### Comparing `bfit-4.9.8/bfit/test/test_deadtime.py` & `bfit-4.9.9/bfit/test/test_deadtime.py`

 * *Files identical despite different names*

### Comparing `bfit-4.9.8/bfit/test/test_export_data.py` & `bfit-4.9.9/bfit/test/test_export_data.py`

 * *Files identical despite different names*

### Comparing `bfit-4.9.8/bfit/test/test_export_fits.py` & `bfit-4.9.9/bfit/test/test_export_fits.py`

 * *Files identical despite different names*

### Comparing `bfit-4.9.8/bfit/test/test_export_param.py` & `bfit-4.9.9/bfit/test/test_export_param.py`

 * *Files identical despite different names*

### Comparing `bfit-4.9.8/bfit/test/test_fit_model.py` & `bfit-4.9.9/bfit/test/test_fit_model.py`

 * *Files identical despite different names*

### Comparing `bfit-4.9.8/bfit/test/test_functions.py` & `bfit-4.9.9/bfit/test/test_functions.py`

 * *Files identical despite different names*

### Comparing `bfit-4.9.8/bfit/test/test_global_fitter.py` & `bfit-4.9.9/bfit/test/test_global_fitter.py`

 * *Files identical despite different names*

### Comparing `bfit-4.9.8/bfit/test/test_leastsquares.py` & `bfit-4.9.9/bfit/test/test_leastsquares.py`

 * *Files identical despite different names*

### Comparing `bfit-4.9.8/bfit/test/test_minuit.py` & `bfit-4.9.9/bfit/test/test_minuit.py`

 * *Files identical despite different names*

### Comparing `bfit-4.9.8/bfit/test/test_numeric_integration.py` & `bfit-4.9.9/bfit/test/test_numeric_integration.py`

 * *Files identical despite different names*

### Comparing `bfit-4.9.8/bfit/test/test_save_load_state.py` & `bfit-4.9.9/bfit/test/test_save_load_state.py`

 * *Files identical despite different names*

### Comparing `bfit-4.9.8/bfit/test/test_tab1_fileviewer.py` & `bfit-4.9.9/bfit/test/test_tab1_fileviewer.py`

 * *Files identical despite different names*

### Comparing `bfit-4.9.8/bfit/test/test_tab2_fetch_files.py` & `bfit-4.9.9/bfit/test/test_tab2_fetch_files.py`

 * *Files identical despite different names*

### Comparing `bfit-4.9.8/bfit/test/test_tab3_fit_files.py` & `bfit-4.9.9/bfit/test/test_tab3_fit_files.py`

 * *Files identical despite different names*

### Comparing `bfit-4.9.8/bfit/test/test_units.py` & `bfit-4.9.9/bfit/test/test_units.py`

 * *Files identical despite different names*

### Comparing `bfit-4.9.8/bfit.egg-info/PKG-INFO` & `bfit-4.9.9/bfit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bfit
-Version: 4.9.8
+Version: 4.9.9
 Summary: β-NMR and β-NQR Data Analysis
 Home-page: https://github.com/dfujim/bfit
 Author: Derek Fujimoto
 Author-email: fujimoto@phas.ubc.ca
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bfit Version: 4.9.8 Summary: Î²-NMR and Î²-NQR Data
+Metadata-Version: 2.1 Name: bfit Version: 4.9.9 Summary: Î²-NMR and Î²-NQR Data
 Analysis Home-page: https://github.com/dfujim/bfit Author: Derek Fujimoto
 Author-email: fujimoto@phas.ubc.ca License: UNKNOWN Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Cython Classifier: License :: OSI Approved
 :: GNU Lesser General Public License v3 (LGPLv3) Classifier: Operating System
 :: POSIX :: Linux Classifier: Operating System :: MacOS Classifier: Development
```

### Comparing `bfit-4.9.8/bfit.egg-info/SOURCES.txt` & `bfit-4.9.9/bfit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bfit-4.9.8/setup.py` & `bfit-4.9.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
                 include_dirs=["./bfit/fitting/FastNumericalIntegration_src",numpy.get_include()],
                 libraries=["m"],
                 extra_compile_args=["-ffast-math"]
                 )
 
 setuptools.setup(
     name="bfit",
-    version="4.9.8",
+    version="4.9.9",
     author="Derek Fujimoto",
     author_email="fujimoto@phas.ubc.ca",
     description="β-NMR and β-NQR Data Analysis",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/dfujim/bfit",
     packages=setuptools.find_packages(),
```

