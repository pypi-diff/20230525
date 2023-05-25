# Comparing `tmp/autogluon.timeseries-0.7.1b20230523.tar.gz` & `tmp/autogluon.timeseries-0.7.1b20230524.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon.timeseries-0.7.1b20230523.tar", last modified: Tue May 23 09:04:21 2023, max compression
+gzip compressed data, was "autogluon.timeseries-0.7.1b20230524.tar", last modified: Wed May 24 09:04:46 2023, max compression
```

## Comparing `autogluon.timeseries-0.7.1b20230523.tar` & `autogluon.timeseries-0.7.1b20230524.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:04:21.520649 autogluon.timeseries-0.7.1b20230523/
--rw-r--r--   0 runner    (1001) docker     (123)    12593 2023-05-23 09:04:21.520649 autogluon.timeseries-0.7.1b20230523/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 09:04:21.520649 autogluon.timeseries-0.7.1b20230523/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-05-23 09:03:35.000000 autogluon.timeseries-0.7.1b20230523/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:04:21.512649 autogluon.timeseries-0.7.1b20230523/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:04:21.516649 autogluon.timeseries-0.7.1b20230523/src/autogluon/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-23 09:03:35.000000 autogluon.timeseries-0.7.1b20230523/src/autogluon/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:04:21.516649 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-05-23 09:03:35.000000 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:04:21.516649 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/configs/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-23 09:03:35.000000 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-23 09:03:35.000000 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/configs/presets_configs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:04:21.516649 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-23 09:03:35.000000 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37170 2023-05-23 09:03:35.000000 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/dataset/ts_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)    11293 2023-05-23 09:03:35.000000 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10081 2023-05-23 09:03:35.000000 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/learner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:04:21.516649 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/models/
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-05-23 09:03:35.000000 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:04:21.516649 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/models/abstract/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-23 09:03:35.000000 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/models/abstract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19736 2023-05-23 09:03:35.000000 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/models/abstract/abstract_timeseries_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-05-23 09:03:35.000000 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/models/abstract/model_trial.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:04:21.516649 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/models/autogluon_tabular/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-23 09:03:35.000000 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/models/autogluon_tabular/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14835 2023-05-23 09:03:35.000000 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/models/autogluon_tabular/mlforecast.py
--rw-r--r--   0 runner    (1001) docker     (123)    17282 2023-05-23 09:03:35.000000 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/models/autogluon_tabular/tabular_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-23 09:03:35.000000 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/models/autogluon_tabular/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:04:21.516649 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/models/ensemble/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-23 09:03:35.000000 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/models/ensemble/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-05-23 09:03:35.000000 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/models/ensemble/abstract_timeseries_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)     5902 2023-05-23 09:03:35.000000 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/models/ensemble/greedy_ensemble.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:04:21.516649 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/models/gluonts/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-23 09:03:35.000000 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/models/gluonts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18915 2023-05-23 09:03:35.000000 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/models/gluonts/abstract_gluonts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:04:21.520649 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/models/gluonts/mx/
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-23 09:03:35.000000 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/models/gluonts/mx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-05-23 09:03:35.000000 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/models/gluonts/mx/callback.py
--rw-r--r--   0 runner    (1001) docker     (123)    22893 2023-05-23 09:03:35.000000 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/models/gluonts/mx/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:04:21.520649 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/models/gluonts/torch/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-23 09:03:35.000000 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/models/gluonts/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13902 2023-05-23 09:03:35.000000 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/models/gluonts/torch/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:04:21.520649 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/models/local/
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-23 09:03:35.000000 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/models/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9193 2023-05-23 09:03:35.000000 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/models/local/abstract_local_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-05-23 09:03:35.000000 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/models/local/naive.py
--rw-r--r--   0 runner    (1001) docker     (123)    10099 2023-05-23 09:03:35.000000 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/models/local/statsforecast.py
--rw-r--r--   0 runner    (1001) docker     (123)    15257 2023-05-23 09:03:35.000000 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/models/local/statsmodels.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:04:21.520649 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/models/multi_window/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-23 09:03:35.000000 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/models/multi_window/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9000 2023-05-23 09:03:35.000000 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/models/multi_window/multi_window_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    10057 2023-05-23 09:03:35.000000 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/models/presets.py
--rw-r--r--   0 runner    (1001) docker     (123)    46181 2023-05-23 09:03:35.000000 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9252 2023-05-23 09:03:35.000000 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/splitter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:04:21.520649 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/trainer/
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-23 09:03:35.000000 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41222 2023-05-23 09:03:35.000000 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/trainer/abstract_trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-05-23 09:03:35.000000 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/trainer/auto_trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:04:21.520649 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:03:35.000000 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8270 2023-05-23 09:03:35.000000 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/utils/features.py
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-05-23 09:03:35.000000 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/utils/forecast.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-23 09:03:35.000000 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/utils/random.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-23 09:03:35.000000 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/utils/seasonality.py
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-05-23 09:03:35.000000 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/utils/warning_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-23 09:04:21.000000 autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:04:21.516649 autogluon.timeseries-0.7.1b20230523/src/autogluon.timeseries.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12593 2023-05-23 09:04:21.000000 autogluon.timeseries-0.7.1b20230523/src/autogluon.timeseries.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-05-23 09:04:21.000000 autogluon.timeseries-0.7.1b20230523/src/autogluon.timeseries.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 09:04:21.000000 autogluon.timeseries-0.7.1b20230523/src/autogluon.timeseries.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-23 09:04:21.000000 autogluon.timeseries-0.7.1b20230523/src/autogluon.timeseries.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-23 09:04:21.000000 autogluon.timeseries-0.7.1b20230523/src/autogluon.timeseries.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-23 09:04:21.000000 autogluon.timeseries-0.7.1b20230523/src/autogluon.timeseries.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 09:04:21.000000 autogluon.timeseries-0.7.1b20230523/src/autogluon.timeseries.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:04:46.125084 autogluon.timeseries-0.7.1b20230524/
+-rw-r--r--   0 runner    (1001) docker     (123)    12593 2023-05-24 09:04:46.125084 autogluon.timeseries-0.7.1b20230524/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 09:04:46.125084 autogluon.timeseries-0.7.1b20230524/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-05-24 09:03:54.000000 autogluon.timeseries-0.7.1b20230524/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:04:46.113083 autogluon.timeseries-0.7.1b20230524/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:04:46.113083 autogluon.timeseries-0.7.1b20230524/src/autogluon/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-24 09:03:54.000000 autogluon.timeseries-0.7.1b20230524/src/autogluon/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:04:46.117083 autogluon.timeseries-0.7.1b20230524/src/autogluon/timeseries/
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-05-24 09:03:54.000000 autogluon.timeseries-0.7.1b20230524/src/autogluon/timeseries/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:04:46.117083 autogluon.timeseries-0.7.1b20230524/src/autogluon/timeseries/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-24 09:03:54.000000 autogluon.timeseries-0.7.1b20230524/src/autogluon/timeseries/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-24 09:03:54.000000 autogluon.timeseries-0.7.1b20230524/src/autogluon/timeseries/configs/presets_configs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:04:46.117083 autogluon.timeseries-0.7.1b20230524/src/autogluon/timeseries/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-24 09:03:54.000000 autogluon.timeseries-0.7.1b20230524/src/autogluon/timeseries/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37170 2023-05-24 09:03:54.000000 autogluon.timeseries-0.7.1b20230524/src/autogluon/timeseries/dataset/ts_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11293 2023-05-24 09:03:54.000000 autogluon.timeseries-0.7.1b20230524/src/autogluon/timeseries/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10081 2023-05-24 09:03:54.000000 autogluon.timeseries-0.7.1b20230524/src/autogluon/timeseries/learner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:04:46.117083 autogluon.timeseries-0.7.1b20230524/src/autogluon/timeseries/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-24 09:03:54.000000 autogluon.timeseries-0.7.1b20230524/src/autogluon/timeseries/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:04:46.117083 autogluon.timeseries-0.7.1b20230524/src/autogluon/timeseries/models/abstract/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-24 09:03:54.000000 autogluon.timeseries-0.7.1b20230524/src/autogluon/timeseries/models/abstract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19736 2023-05-24 09:03:54.000000 autogluon.timeseries-0.7.1b20230524/src/autogluon/timeseries/models/abstract/abstract_timeseries_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-05-24 09:03:54.000000 autogluon.timeseries-0.7.1b20230524/src/autogluon/timeseries/models/abstract/model_trial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:04:46.121084 autogluon.timeseries-0.7.1b20230524/src/autogluon/timeseries/models/autogluon_tabular/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-24 09:03:54.000000 autogluon.timeseries-0.7.1b20230524/src/autogluon/timeseries/models/autogluon_tabular/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16983 2023-05-24 09:03:54.000000 autogluon.timeseries-0.7.1b20230524/src/autogluon/timeseries/models/autogluon_tabular/direct_tabular.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14835 2023-05-24 09:03:54.000000 autogluon.timeseries-0.7.1b20230524/src/autogluon/timeseries/models/autogluon_tabular/mlforecast.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-24 09:03:54.000000 autogluon.timeseries-0.7.1b20230524/src/autogluon/timeseries/models/autogluon_tabular/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:04:46.121084 autogluon.timeseries-0.7.1b20230524/src/autogluon/timeseries/models/ensemble/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-24 09:03:54.000000 autogluon.timeseries-0.7.1b20230524/src/autogluon/timeseries/models/ensemble/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-05-24 09:03:54.000000 autogluon.timeseries-0.7.1b20230524/src/autogluon/timeseries/models/ensemble/abstract_timeseries_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5902 2023-05-24 09:03:54.000000 autogluon.timeseries-0.7.1b20230524/src/autogluon/timeseries/models/ensemble/greedy_ensemble.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:04:46.121084 autogluon.timeseries-0.7.1b20230524/src/autogluon/timeseries/models/gluonts/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-24 09:03:54.000000 autogluon.timeseries-0.7.1b20230524/src/autogluon/timeseries/models/gluonts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18915 2023-05-24 09:03:54.000000 autogluon.timeseries-0.7.1b20230524/src/autogluon/timeseries/models/gluonts/abstract_gluonts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:04:46.121084 autogluon.timeseries-0.7.1b20230524/src/autogluon/timeseries/models/gluonts/mx/
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-24 09:03:54.000000 autogluon.timeseries-0.7.1b20230524/src/autogluon/timeseries/models/gluonts/mx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-05-24 09:03:54.000000 autogluon.timeseries-0.7.1b20230524/src/autogluon/timeseries/models/gluonts/mx/callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22893 2023-05-24 09:03:54.000000 autogluon.timeseries-0.7.1b20230524/src/autogluon/timeseries/models/gluonts/mx/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:04:46.121084 autogluon.timeseries-0.7.1b20230524/src/autogluon/timeseries/models/gluonts/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-24 09:03:54.000000 autogluon.timeseries-0.7.1b20230524/src/autogluon/timeseries/models/gluonts/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13902 2023-05-24 09:03:54.000000 autogluon.timeseries-0.7.1b20230524/src/autogluon/timeseries/models/gluonts/torch/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:04:46.121084 autogluon.timeseries-0.7.1b20230524/src/autogluon/timeseries/models/local/
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-24 09:03:54.000000 autogluon.timeseries-0.7.1b20230524/src/autogluon/timeseries/models/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9193 2023-05-24 09:03:54.000000 autogluon.timeseries-0.7.1b20230524/src/autogluon/timeseries/models/local/abstract_local_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-05-24 09:03:54.000000 autogluon.timeseries-0.7.1b20230524/src/autogluon/timeseries/models/local/naive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10099 2023-05-24 09:03:54.000000 autogluon.timeseries-0.7.1b20230524/src/autogluon/timeseries/models/local/statsforecast.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15257 2023-05-24 09:03:54.000000 autogluon.timeseries-0.7.1b20230524/src/autogluon/timeseries/models/local/statsmodels.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:04:46.125084 autogluon.timeseries-0.7.1b20230524/src/autogluon/timeseries/models/multi_window/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-24 09:03:54.000000 autogluon.timeseries-0.7.1b20230524/src/autogluon/timeseries/models/multi_window/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9000 2023-05-24 09:03:54.000000 autogluon.timeseries-0.7.1b20230524/src/autogluon/timeseries/models/multi_window/multi_window_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10144 2023-05-24 09:03:54.000000 autogluon.timeseries-0.7.1b20230524/src/autogluon/timeseries/models/presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46186 2023-05-24 09:03:54.000000 autogluon.timeseries-0.7.1b20230524/src/autogluon/timeseries/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9252 2023-05-24 09:03:54.000000 autogluon.timeseries-0.7.1b20230524/src/autogluon/timeseries/splitter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:04:46.125084 autogluon.timeseries-0.7.1b20230524/src/autogluon/timeseries/trainer/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-24 09:03:54.000000 autogluon.timeseries-0.7.1b20230524/src/autogluon/timeseries/trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41222 2023-05-24 09:03:54.000000 autogluon.timeseries-0.7.1b20230524/src/autogluon/timeseries/trainer/abstract_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-05-24 09:03:54.000000 autogluon.timeseries-0.7.1b20230524/src/autogluon/timeseries/trainer/auto_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:04:46.125084 autogluon.timeseries-0.7.1b20230524/src/autogluon/timeseries/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 09:03:54.000000 autogluon.timeseries-0.7.1b20230524/src/autogluon/timeseries/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8270 2023-05-24 09:03:54.000000 autogluon.timeseries-0.7.1b20230524/src/autogluon/timeseries/utils/features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-05-24 09:03:54.000000 autogluon.timeseries-0.7.1b20230524/src/autogluon/timeseries/utils/forecast.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-24 09:03:54.000000 autogluon.timeseries-0.7.1b20230524/src/autogluon/timeseries/utils/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-24 09:03:54.000000 autogluon.timeseries-0.7.1b20230524/src/autogluon/timeseries/utils/seasonality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-05-24 09:03:54.000000 autogluon.timeseries-0.7.1b20230524/src/autogluon/timeseries/utils/warning_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-24 09:04:45.000000 autogluon.timeseries-0.7.1b20230524/src/autogluon/timeseries/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:04:46.113083 autogluon.timeseries-0.7.1b20230524/src/autogluon.timeseries.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12593 2023-05-24 09:04:46.000000 autogluon.timeseries-0.7.1b20230524/src/autogluon.timeseries.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-05-24 09:04:46.000000 autogluon.timeseries-0.7.1b20230524/src/autogluon.timeseries.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 09:04:46.000000 autogluon.timeseries-0.7.1b20230524/src/autogluon.timeseries.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-24 09:04:46.000000 autogluon.timeseries-0.7.1b20230524/src/autogluon.timeseries.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-24 09:04:46.000000 autogluon.timeseries-0.7.1b20230524/src/autogluon.timeseries.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-24 09:04:46.000000 autogluon.timeseries-0.7.1b20230524/src/autogluon.timeseries.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 09:04:46.000000 autogluon.timeseries-0.7.1b20230524/src/autogluon.timeseries.egg-info/zip-safe
```

### Comparing `autogluon.timeseries-0.7.1b20230523/PKG-INFO` & `autogluon.timeseries-0.7.1b20230524/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.timeseries
-Version: 0.7.1b20230523
+Version: 0.7.1b20230524
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.timeseries-0.7.1b20230523/setup.py` & `autogluon.timeseries-0.7.1b20230524/setup.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/__init__.py` & `autogluon.timeseries-0.7.1b20230524/src/autogluon/timeseries/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/configs/presets_configs.py` & `autogluon.timeseries-0.7.1b20230524/src/autogluon/timeseries/configs/presets_configs.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/dataset/ts_dataframe.py` & `autogluon.timeseries-0.7.1b20230524/src/autogluon/timeseries/dataset/ts_dataframe.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/evaluator.py` & `autogluon.timeseries-0.7.1b20230524/src/autogluon/timeseries/evaluator.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/learner.py` & `autogluon.timeseries-0.7.1b20230524/src/autogluon/timeseries/learner.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/models/abstract/abstract_timeseries_model.py` & `autogluon.timeseries-0.7.1b20230524/src/autogluon/timeseries/models/abstract/abstract_timeseries_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/models/abstract/model_trial.py` & `autogluon.timeseries-0.7.1b20230524/src/autogluon/timeseries/models/abstract/model_trial.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/models/autogluon_tabular/mlforecast.py` & `autogluon.timeseries-0.7.1b20230524/src/autogluon/timeseries/models/autogluon_tabular/mlforecast.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/models/autogluon_tabular/tabular_model.py` & `autogluon.timeseries-0.7.1b20230524/src/autogluon/timeseries/models/autogluon_tabular/direct_tabular.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,63 +1,67 @@
 import logging
 import time
 import warnings
-from typing import Any, Callable, Dict, List, Optional, Tuple
+from typing import Any, Callable, Dict, List, Optional, Tuple, Union
 
 import numpy as np
 import pandas as pd
 
 # TODO: Drop GluonTS dependency
 from gluonts.time_feature import get_lags_for_frequency, time_features_from_frequency_str
 from joblib.parallel import Parallel, delayed
 
 import autogluon.core as ag
 from autogluon.tabular import TabularPredictor
 from autogluon.timeseries.dataset.ts_dataframe import ITEMID, TIMESTAMP, TimeSeriesDataFrame
 from autogluon.timeseries.models.abstract import AbstractTimeSeriesModel
+from autogluon.timeseries.utils.forecast import get_forecast_horizon_index_ts_dataframe
 
 logger = logging.getLogger(__name__)
 
 
-class AutoGluonTabularModel(AbstractTimeSeriesModel):
+class DirectTabularModel(AbstractTimeSeriesModel):
     """Predict future time series values using autogluon.tabular.TabularPredictor.
 
-    The forecasting is converted to a tabular problem using the following features:
+    A single predictor is used to forecast all future time series values using the following features:
 
     - lag features (observed time series values) based on ``freq`` of the data
     - time features (e.g., day of the week) based on the timestamp of the measurement
     - lagged known and past covariates (if available)
     - static features of each item (if available)
 
-    Quantiles are obtained by assuming that the residuals follow zero-mean normal distribution, scale of which is
-    estimated from the empirical distribution of the residuals.
+    Features not known during the forecast horizon (e.g., future target values) are replaced by NaNs.
+
+    If ``eval_metric=="mean_wQuantileLoss"``, the TabularPredictor will be trained with ``"quantile"`` problem type.
+    Otherwise, TabularPredictor will be trained with ``"regression"`` problem type, and dummy quantiles will be
+    obtained by assuming that the residuals follow zero-mean normal distribution.
 
 
     Other Parameters
     ----------------
-    max_train_size : int, default = 1_000_000
+    max_num_samples : int, default = 1_000_000
         Maximum number of rows in the training and validation sets. If the number of rows in train or validation data
-        exceeds ``max_train_size``, then ``max_train_size`` many rows are subsampled from the dataframe.
+        exceeds ``max_num_samples``, then ``max_num_samples`` many rows are subsampled from the dataframe.
     tabular_hyperparameters : Dict[Dict[str, Any]], optional
         Hyperparameters dictionary passed to `TabularPredictor.fit`. Contains the names of models that should be fit.
-        Defaults to ``{"CAT": {}, "GBM" :{}}``.
+        Defaults to ``{"GBM" :{}}``.
     """
 
+    # TODO: Implemented detrending/differencing to allow extrapolation.
+
     default_tabular_hyperparameters = {
-        "CAT": {},
         "GBM": {},
     }
 
     PREDICTION_BATCH_SIZE = 100_000
 
     TIMESERIES_METRIC_TO_TABULAR_METRIC = {
         "MASE": "mean_absolute_error",
         "MAPE": "mean_absolute_percentage_error",
         "sMAPE": "mean_absolute_percentage_error",
-        "mean_wQuantileLoss": "mean_absolute_error",
         "MSE": "mean_squared_error",
         "RMSE": "root_mean_squared_error",
     }
 
     def __init__(
         self,
         freq: Optional[str] = None,
@@ -77,19 +81,32 @@
             hyperparameters=hyperparameters,
             **kwargs,
         )
         self._target_lag_indices: np.array = None
         self._known_covariates_lag_indices: np.array = None
         self._past_covariates_lag_indices: np.array = None
         self._time_features: List[Callable] = None
-        self._available_features: pd.Index = None
-        self.quantile_adjustments: Dict[str, float] = {}
-
+        self.is_quantile_model = self.eval_metric == "mean_wQuantileLoss"
+        if 0.5 not in self.quantile_levels:
+            self.must_drop_median = True
+            self.quantile_levels = sorted(set([0.5] + self.quantile_levels))
+        else:
+            self.must_drop_median = False
+        self.residuals_std = 1.0
         self.tabular_predictor: TabularPredictor = None
 
+    def _normalize_targets(self, data: TimeSeriesDataFrame, min_scale=1e-5) -> Tuple[TimeSeriesDataFrame, pd.Series]:
+        """Normalize data such that each the average absolute value of each time series is equal to 1."""
+        # TODO: Implement other scalers (min/max)?
+        # TODO: Don't include validation data when computing the scale
+        scale_per_item = data.abs().groupby(level=ITEMID, sort=False)[self.target].mean().clip(lower=min_scale)
+        normalized_data = data.copy()
+        normalized_data[self.target] = normalized_data[self.target] / scale_per_item
+        return normalized_data, scale_per_item
+
     def _get_features_dataframe(
         self,
         data: TimeSeriesDataFrame,
         max_rows_per_item: Optional[int] = None,
     ) -> pd.DataFrame:
         """Generate a feature matrix used by TabularPredictor.
 
@@ -264,137 +281,117 @@
         return features
 
     def _fit(
         self,
         train_data: TimeSeriesDataFrame,
         val_data: Optional[TimeSeriesDataFrame] = None,
         time_limit: int = None,
+        verbosity: int = 2,
         **kwargs,
     ) -> None:
         self._check_fit_params()
         start_time = time.time()
         if self.tabular_predictor is not None:
             raise AssertionError(f"{self.name} predictor has already been fit!")
-        verbosity = kwargs.get("verbosity", 2)
         self._target_lag_indices = np.array(get_lags_for_frequency(train_data.freq), dtype=np.int64)
         self._past_covariates_lag_indices = self._target_lag_indices
         self._known_covariates_lag_indices = np.concatenate([[0], self._target_lag_indices])
         self._time_features = time_features_from_frequency_str(train_data.freq)
 
         train_data, _ = self._normalize_targets(train_data)
-        train_df = self._get_features_dataframe(train_data)
-        # Remove features that are completely missing in the training set
-        train_df.dropna(axis=1, how="all", inplace=True)
-        self._available_features = train_df.columns
+        # Do not use external val_data as tuning_data to avoid overfitting
+        train_subset, val_subset = train_data.train_test_split(self.prediction_length)
+        train_df = self._get_features_dataframe(train_subset)
+        val_df = self._get_features_dataframe(val_subset, max_rows_per_item=self.prediction_length)
 
         model_params = self._get_model_params()
         tabular_hyperparameters = model_params.get("tabular_hyperparameters", self.default_tabular_hyperparameters)
-        max_train_size = model_params.get("max_train_size", 1_000_000)
+        max_num_samples = model_params.get("max_num_samples", 1_000_000)
 
-        if len(train_df) > max_train_size:
-            train_df = train_df.sample(max_train_size)
+        if len(train_df) > max_num_samples:
+            train_df = train_df.sample(max_num_samples)
         logger.debug(f"Generated training dataframe with shape {train_df.shape}")
 
-        if val_data is not None:
-            if val_data.freq != train_data.freq:
-                raise ValueError(
-                    f"train_data and val_data must have the same freq (received {train_data.freq} and {val_data.freq})"
-                )
-            val_data, _ = self._normalize_targets(val_data)
-            val_df = self._get_features_dataframe(val_data, max_rows_per_item=self.prediction_length)
-            val_df = val_df[self._available_features]
-
-            if len(val_df) > max_train_size:
-                val_df = val_df.sample(max_train_size)
-
-            logger.debug(f"Generated validation dataframe with shape {val_df.shape}")
-        else:
-            logger.warning(
-                f"No val_data was provided to {self.name}. "
-                "TabularPredictor will generate a validation set without respecting the temporal ordering."
-            )
-            val_df = None
-
         time_elapsed = time.time() - start_time
         autogluon_logger = logging.getLogger("autogluon")
         logging_level = autogluon_logger.level
 
+        if self.is_quantile_model:
+            predictor_init_kwargs = {
+                "problem_type": ag.constants.QUANTILE,
+                "eval_metric": "pinball_loss",
+                "quantile_levels": self.quantile_levels,
+            }
+        else:
+            predictor_init_kwargs = {
+                "problem_type": ag.constants.REGRESSION,
+                "eval_metric": self.TIMESERIES_METRIC_TO_TABULAR_METRIC.get(self.eval_metric),
+            }
+
         self.tabular_predictor = TabularPredictor(
             path=self.path,
             label=self.target,
-            problem_type=ag.constants.REGRESSION,
-            eval_metric=self.TIMESERIES_METRIC_TO_TABULAR_METRIC.get(self.eval_metric),
+            **predictor_init_kwargs,
         )
 
         with warnings.catch_warnings():
             warnings.simplefilter("ignore")
             self.tabular_predictor.fit(
                 train_data=train_df,
                 tuning_data=val_df,
                 time_limit=time_limit - time_elapsed if time_limit else None,
                 hyperparameters=tabular_hyperparameters,
                 verbosity=verbosity - 2,
             )
-        residuals = (train_df[self.target] - self.tabular_predictor.predict(train_df)).values
-        for q in self.quantile_levels:
-            self.quantile_adjustments[q] = np.quantile(residuals, q)
-        # Logger level is changed inside .fit(), restore to the initial value
-        autogluon_logger.setLevel(logging_level)
 
-    def _extend_index(self, data: TimeSeriesDataFrame) -> TimeSeriesDataFrame:
-        """Add self.prediction_length many time steps with dummy values to each timeseries in the dataset."""
+        if not self.is_quantile_model:
+            residuals = (train_df[self.target] - self.tabular_predictor.predict(train_df)).values
+            self.residuals_std = np.sqrt(np.mean(residuals**2))
 
-        def extend_single_time_series(group):
-            offset = pd.tseries.frequencies.to_offset(data.freq)
-            cutoff = group.index.get_level_values(TIMESTAMP)[-1]
-            new_index = pd.date_range(cutoff + offset, freq=offset, periods=self.prediction_length).rename(TIMESTAMP)
-            new_values = np.full([self.prediction_length], fill_value=np.nan)
-            new_df = pd.DataFrame(new_values, index=new_index, columns=[self.target])
-            return pd.concat([group.droplevel(ITEMID), new_df])
-
-        extended_data = data.groupby(level=ITEMID, sort=False).apply(extend_single_time_series)
-        extended_data.static_features = data.static_features
-        return extended_data
-
-    def predict(self, data: TimeSeriesDataFrame, quantile_levels: List[float] = None, **kwargs) -> TimeSeriesDataFrame:
-        self._check_predict_inputs(data=data, quantile_levels=quantile_levels)
-        if quantile_levels is None:
-            quantile_levels = self.quantile_levels
+        # Logger level is changed inside .fit(), restore to the initial value
+        autogluon_logger.setLevel(logging_level)
 
+    def _postprocess_predictions(self, predictions: Union[pd.DataFrame, pd.Series]) -> pd.DataFrame:
+        """Convert output of TabularPredictor to a dataframe with 'mean' and quantile forecast columns."""
+        from scipy.stats import norm
+
+        if self.is_quantile_model:
+            # Ensure that quantiles are monotonic
+            predictions.values.sort(axis=1)
+            predictions.columns = [str(q) for q in predictions.columns]
+            predictions["mean"] = predictions["0.5"]
+        else:
+            predictions = predictions.rename("mean").to_frame()
+            for q in self.quantile_levels:
+                predictions[str(q)] = predictions["mean"] + norm.ppf(q) * self.residuals_std
+
+        column_order = ["mean"] + [col for col in predictions.columns if col != "mean"]
+        return predictions[column_order]
+
+    def predict(
+        self, data: TimeSeriesDataFrame, known_covariates: Optional[TimeSeriesDataFrame] = None, **kwargs
+    ) -> TimeSeriesDataFrame:
         data, scale_per_item = self._normalize_targets(data)
-        data_extended = self._extend_index(data)
+        if known_covariates is not None:
+            data_future = known_covariates.copy()
+            data_future[self.target] = np.nan
+        else:
+            future_index = get_forecast_horizon_index_ts_dataframe(data, self.prediction_length)
+            data_future = pd.DataFrame(columns=[self.target], index=future_index)
+        data_extended = pd.concat([data, data_future])
+        data_extended.static_features = data.static_features
+
         features = self._get_features_dataframe(data_extended, max_rows_per_item=self.prediction_length)
-        features = features[self._available_features]
 
         # Predict for batches (instead of using full dataset) to avoid high memory usage
         batches = features.groupby(np.arange(len(features)) // self.PREDICTION_BATCH_SIZE, sort=False)
         predictions = pd.concat([self.tabular_predictor.predict(batch) for _, batch in batches])
+        predictions.set_index(data_future.index, inplace=True)
 
-        predictions = predictions.rename("mean").to_frame()
-        preds_index = data_extended.slice_by_timestep(-self.prediction_length, None).index
-        predictions.set_index(preds_index, inplace=True)
-
-        for q in quantile_levels:
-            predictions[str(q)] = predictions["mean"] + self.quantile_adjustments[q]
-
-        predictions = self._rescale_targets(predictions, scale_per_item)
-        return TimeSeriesDataFrame(predictions).loc[data.item_ids]
-
-    def _normalize_targets(self, data: TimeSeriesDataFrame, min_scale=1e-5) -> Tuple[TimeSeriesDataFrame, pd.Series]:
-        """Normalize data such that each the average absolute value of each time series is equal to 1."""
-        # TODO: Implement other scalers (min/max)?
-        # TODO: Don't include validation data when computing the scale
-        scale_per_item = data.abs().groupby(level=ITEMID, sort=False)[self.target].mean().clip(lower=min_scale)
-        normalized_data = data.copy()
-        for col in normalized_data.columns:
-            normalized_data[col] = normalized_data[col] / scale_per_item
-        return normalized_data, scale_per_item
+        predictions = self._postprocess_predictions(predictions)
 
-    def _rescale_targets(self, normalized_data: TimeSeriesDataFrame, scale_per_item: pd.Series) -> TimeSeriesDataFrame:
-        """Scale all columns in the normalized dataframe back to original scale (inplace)."""
-        data = normalized_data
-        for col in data.columns:
-            data[col] = data[col] * scale_per_item
-        return data
+        for col in predictions.columns:
+            predictions[col] = predictions[col] * scale_per_item
+        return TimeSeriesDataFrame(predictions).reindex(data.item_ids, level=ITEMID)
 
     def _more_tags(self) -> dict:
         return {"can_refit_full": True}
```

### Comparing `autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/models/autogluon_tabular/utils.py` & `autogluon.timeseries-0.7.1b20230524/src/autogluon/timeseries/models/autogluon_tabular/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/models/ensemble/abstract_timeseries_ensemble.py` & `autogluon.timeseries-0.7.1b20230524/src/autogluon/timeseries/models/ensemble/abstract_timeseries_ensemble.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/models/ensemble/greedy_ensemble.py` & `autogluon.timeseries-0.7.1b20230524/src/autogluon/timeseries/models/ensemble/greedy_ensemble.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/models/gluonts/abstract_gluonts.py` & `autogluon.timeseries-0.7.1b20230524/src/autogluon/timeseries/models/gluonts/abstract_gluonts.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/models/gluonts/mx/__init__.py` & `autogluon.timeseries-0.7.1b20230524/src/autogluon/timeseries/models/gluonts/mx/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/models/gluonts/mx/callback.py` & `autogluon.timeseries-0.7.1b20230524/src/autogluon/timeseries/models/gluonts/mx/callback.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/models/gluonts/mx/models.py` & `autogluon.timeseries-0.7.1b20230524/src/autogluon/timeseries/models/gluonts/mx/models.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/models/gluonts/torch/models.py` & `autogluon.timeseries-0.7.1b20230524/src/autogluon/timeseries/models/gluonts/torch/models.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/models/local/__init__.py` & `autogluon.timeseries-0.7.1b20230524/src/autogluon/timeseries/models/local/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/models/local/abstract_local_model.py` & `autogluon.timeseries-0.7.1b20230524/src/autogluon/timeseries/models/local/abstract_local_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/models/local/naive.py` & `autogluon.timeseries-0.7.1b20230524/src/autogluon/timeseries/models/local/naive.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/models/local/statsforecast.py` & `autogluon.timeseries-0.7.1b20230524/src/autogluon/timeseries/models/local/statsforecast.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/models/local/statsmodels.py` & `autogluon.timeseries-0.7.1b20230524/src/autogluon/timeseries/models/local/statsmodels.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/models/multi_window/multi_window_model.py` & `autogluon.timeseries-0.7.1b20230524/src/autogluon/timeseries/models/multi_window/multi_window_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/models/presets.py` & `autogluon.timeseries-0.7.1b20230524/src/autogluon/timeseries/models/presets.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 from autogluon.common import space
 from autogluon.core import constants
 
 from . import (
     ARIMAModel,
     AutoARIMAModel,
     AutoETSModel,
-    AutoGluonTabularModel,
     DeepARModel,
+    DirectTabularModel,
     DynamicOptimizedThetaModel,
     ETSModel,
     NaiveModel,
     RecursiveTabularModel,
     SeasonalNaiveModel,
     SimpleFeedForwardModel,
     TemporalFusionTransformerModel,
@@ -29,16 +29,16 @@
 logger = logging.getLogger(__name__)
 
 # define the model zoo with their aliases
 MODEL_TYPES = dict(
     SimpleFeedForward=SimpleFeedForwardModel,
     DeepAR=DeepARModel,
     TemporalFusionTransformer=TemporalFusionTransformerModel,
-    AutoGluonTabular=AutoGluonTabularModel,
     RecursiveTabular=RecursiveTabularModel,
+    DirectTabular=DirectTabularModel,
     Naive=NaiveModel,
     SeasonalNaive=SeasonalNaiveModel,
     AutoETS=AutoETSModel,
     AutoARIMA=AutoARIMAModel,
     DynamicOptimizedTheta=DynamicOptimizedThetaModel,
     Theta=ThetaModel,
     ARIMA=ARIMAModel,
@@ -70,15 +70,15 @@
 DEFAULT_MODEL_PRIORITY = dict(
     Naive=100,
     SeasonalNaive=100,
     ETS=90,
     Theta=90,
     RecursiveTabular=80,
     ARIMA=70,
-    AutoGluonTabular=70,
+    DirectTabular=70,
     DeepAR=60,
     TemporalFusionTransformer=50,
     SimpleFeedForward=40,
     AutoARIMA=50,
     AutoETS=70,
     DynamicOptimizedTheta=60,
     # Models below are not included in any presets
@@ -112,25 +112,27 @@
             "Naive": {},
             "SeasonalNaive": {},
             "ARIMA": {},
             "ETS": {},
             "AutoETS": {},
             "Theta": {},
             "RecursiveTabular": {},
+            "DirectTabular": {},
             "DeepAR": {},
         },
         "high_quality": {
             "Naive": {},
             "SeasonalNaive": {},
             "ARIMA": {},
             "ETS": {},
             "AutoETS": {},
             "AutoARIMA": {},
             "Theta": {},
             "RecursiveTabular": {},
+            "DirectTabular": {},
             "DeepAR": {},
             "SimpleFeedForward": {},
             "TemporalFusionTransformer": {},
         },
         "best_quality": {
             "Naive": {},
             "SeasonalNaive": {},
@@ -142,14 +144,15 @@
             "Theta": {},
             "RecursiveTabular": {
                 "tabular_hyperparameters": {
                     "NN_TORCH": {"proc.impute_strategy": "constant"},
                     "GBM": [{}, {"extra_trees": True, "ag_args": {"name_suffix": "XT"}}],
                 },
             },
+            "DirectTabular": {},
             "DeepAR": {
                 "num_layers": space.Int(1, 3, default=2),
                 "hidden_size": space.Int(40, 80, default=40),
             },
             "SimpleFeedForward": {
                 "hidden_dimensions": space.Categorical([40], [40, 40], [120]),
             },
```

### Comparing `autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/predictor.py` & `autogluon.timeseries-0.7.1b20230524/src/autogluon/timeseries/predictor.py`

 * *Files 0% similar despite different names*

```diff
@@ -145,15 +145,15 @@
         self.known_covariates_names = known_covariates_names
 
         self.prediction_length = prediction_length
         self.eval_metric = eval_metric
         self.eval_metric_seasonal_period = eval_metric_seasonal_period
         if quantile_levels is None:
             quantile_levels = [0.1, 0.2, 0.3, 0.4, 0.5, 0.6, 0.7, 0.8, 0.9]
-        self.quantile_levels = quantile_levels
+        self.quantile_levels = sorted(quantile_levels)
 
         if validation_splitter is not None:
             warnings.warn(
                 "`validation_splitter` argument has been deprecated as of v0.8.0. "
                 "Please use the `num_val_windows` argument of `TimeSeriesPredictor.fit` instead."
             )
         if quantiles is not None:
@@ -361,15 +361,15 @@
             statistical models.
             Any user-specified arguments in :meth:`~autogluon.timeseries.TimeSeriesPredictor.fit` will
             override the values used by presets.
 
             Available presets:
 
             - ``"fast_training"``: fit simple "local" statistical models (``ETS``, ``ARIMA``, ``Theta``, ``Naive``, ``SeasonalNaive``). These models are fast to train, but cannot capture more complex patterns in the data.
-            - ``"medium_quality"``: all models mentioned above + tree-based model ``AutoGluonTabular`` + deep learning model ``DeepAR``. Default setting that produces good forecasts with reasonable training time.
+            - ``"medium_quality"``: all models mentioned above + tree-based model ``DirectTabular`` + deep learning model ``DeepAR``. Default setting that produces good forecasts with reasonable training time.
             - ``"high_quality"``: all models mentioned above + hyperparameter optimization for local statistical models + deep learning models ``TemporalFusionTransformerMXNet`` (if MXNet is available) and ``SimpleFeedForward``. Usually more accurate than ``medium_quality``, but takes longer to train.
             - ``"best_quality"``: all models mentioned above + deep learning model ``TransformerMXNet`` (if MXNet is available) + hyperparameter optimization for deep learning models. Usually better than ``high_quality``, but takes much longer to train.
 
             Details for these presets can be found in ``autogluon/timeseries/configs/presets_configs.py``. If not
             provided, user-provided values for ``hyperparameters`` and ``hyperparameter_tune_kwargs`` will be used
             (defaulting to their default values specified below).
         hyperparameters : str or dict, default = "medium_quality"
```

### Comparing `autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/splitter.py` & `autogluon.timeseries-0.7.1b20230524/src/autogluon/timeseries/splitter.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/trainer/abstract_trainer.py` & `autogluon.timeseries-0.7.1b20230524/src/autogluon/timeseries/trainer/abstract_trainer.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/trainer/auto_trainer.py` & `autogluon.timeseries-0.7.1b20230524/src/autogluon/timeseries/trainer/auto_trainer.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/utils/features.py` & `autogluon.timeseries-0.7.1b20230524/src/autogluon/timeseries/utils/features.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/utils/forecast.py` & `autogluon.timeseries-0.7.1b20230524/src/autogluon/timeseries/utils/forecast.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/utils/seasonality.py` & `autogluon.timeseries-0.7.1b20230524/src/autogluon/timeseries/utils/seasonality.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230523/src/autogluon/timeseries/utils/warning_filters.py` & `autogluon.timeseries-0.7.1b20230524/src/autogluon/timeseries/utils/warning_filters.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230523/src/autogluon.timeseries.egg-info/PKG-INFO` & `autogluon.timeseries-0.7.1b20230524/src/autogluon.timeseries.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.timeseries
-Version: 0.7.1b20230523
+Version: 0.7.1b20230524
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.timeseries-0.7.1b20230523/src/autogluon.timeseries.egg-info/SOURCES.txt` & `autogluon.timeseries-0.7.1b20230524/src/autogluon.timeseries.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -19,16 +19,16 @@
 src/autogluon/timeseries/dataset/ts_dataframe.py
 src/autogluon/timeseries/models/__init__.py
 src/autogluon/timeseries/models/presets.py
 src/autogluon/timeseries/models/abstract/__init__.py
 src/autogluon/timeseries/models/abstract/abstract_timeseries_model.py
 src/autogluon/timeseries/models/abstract/model_trial.py
 src/autogluon/timeseries/models/autogluon_tabular/__init__.py
+src/autogluon/timeseries/models/autogluon_tabular/direct_tabular.py
 src/autogluon/timeseries/models/autogluon_tabular/mlforecast.py
-src/autogluon/timeseries/models/autogluon_tabular/tabular_model.py
 src/autogluon/timeseries/models/autogluon_tabular/utils.py
 src/autogluon/timeseries/models/ensemble/__init__.py
 src/autogluon/timeseries/models/ensemble/abstract_timeseries_ensemble.py
 src/autogluon/timeseries/models/ensemble/greedy_ensemble.py
 src/autogluon/timeseries/models/gluonts/__init__.py
 src/autogluon/timeseries/models/gluonts/abstract_gluonts.py
 src/autogluon/timeseries/models/gluonts/mx/__init__.py
```

