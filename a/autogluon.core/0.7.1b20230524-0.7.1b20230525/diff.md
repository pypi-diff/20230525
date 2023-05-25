# Comparing `tmp/autogluon.core-0.7.1b20230524.tar.gz` & `tmp/autogluon.core-0.7.1b20230525.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon.core-0.7.1b20230524.tar", last modified: Wed May 24 09:04:15 2023, max compression
+gzip compressed data, was "autogluon.core-0.7.1b20230525.tar", last modified: Thu May 25 09:03:59 2023, max compression
```

## Comparing `autogluon.core-0.7.1b20230524.tar` & `autogluon.core-0.7.1b20230525.tar`

### file list

```diff
@@ -1,121 +1,120 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:04:15.603127 autogluon.core-0.7.1b20230524/
--rw-r--r--   0 runner    (1001) docker     (123)    12631 2023-05-24 09:04:15.603127 autogluon.core-0.7.1b20230524/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 09:04:15.603127 autogluon.core-0.7.1b20230524/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-05-24 09:03:54.000000 autogluon.core-0.7.1b20230524/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:04:15.591126 autogluon.core-0.7.1b20230524/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:04:15.591126 autogluon.core-0.7.1b20230524/src/autogluon/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-24 09:03:54.000000 autogluon.core-0.7.1b20230524/src/autogluon/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:04:15.591126 autogluon.core-0.7.1b20230524/src/autogluon/core/
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-05-24 09:03:54.000000 autogluon.core-0.7.1b20230524/src/autogluon/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6511 2023-05-24 09:03:54.000000 autogluon.core-0.7.1b20230524/src/autogluon/core/_setup_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:04:15.591126 autogluon.core-0.7.1b20230524/src/autogluon/core/augmentation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 09:03:54.000000 autogluon.core-0.7.1b20230524/src/autogluon/core/augmentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9764 2023-05-24 09:03:54.000000 autogluon.core-0.7.1b20230524/src/autogluon/core/augmentation/distill_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:04:15.595126 autogluon.core-0.7.1b20230524/src/autogluon/core/calibrate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 09:03:54.000000 autogluon.core-0.7.1b20230524/src/autogluon/core/calibrate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-05-24 09:03:54.000000 autogluon.core-0.7.1b20230524/src/autogluon/core/calibrate/conformity_score.py
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-05-24 09:03:54.000000 autogluon.core-0.7.1b20230524/src/autogluon/core/calibrate/temperature_scaling.py
--rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-05-24 09:03:54.000000 autogluon.core-0.7.1b20230524/src/autogluon/core/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:04:15.595126 autogluon.core-0.7.1b20230524/src/autogluon/core/data/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-24 09:03:54.000000 autogluon.core-0.7.1b20230524/src/autogluon/core/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-05-24 09:03:54.000000 autogluon.core-0.7.1b20230524/src/autogluon/core/data/cleaner.py
--rw-r--r--   0 runner    (1001) docker     (123)    14331 2023-05-24 09:03:54.000000 autogluon.core-0.7.1b20230524/src/autogluon/core/data/label_cleaner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-05-24 09:03:54.000000 autogluon.core-0.7.1b20230524/src/autogluon/core/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:04:15.595126 autogluon.core-0.7.1b20230524/src/autogluon/core/hpo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 09:03:54.000000 autogluon.core-0.7.1b20230524/src/autogluon/core/hpo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-24 09:03:54.000000 autogluon.core-0.7.1b20230524/src/autogluon/core/hpo/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-24 09:03:54.000000 autogluon.core-0.7.1b20230524/src/autogluon/core/hpo/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    29675 2023-05-24 09:03:54.000000 autogluon.core-0.7.1b20230524/src/autogluon/core/hpo/executors.py
--rw-r--r--   0 runner    (1001) docker     (123)    23977 2023-05-24 09:03:54.000000 autogluon.core-0.7.1b20230524/src/autogluon/core/hpo/ray_hpo.py
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-05-24 09:03:54.000000 autogluon.core-0.7.1b20230524/src/autogluon/core/hpo/ray_tune_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-05-24 09:03:54.000000 autogluon.core-0.7.1b20230524/src/autogluon/core/hpo/ray_tune_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-05-24 09:03:54.000000 autogluon.core-0.7.1b20230524/src/autogluon/core/hpo/ray_tune_scheduler_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-05-24 09:03:54.000000 autogluon.core-0.7.1b20230524/src/autogluon/core/hpo/ray_tune_searcher_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-05-24 09:03:54.000000 autogluon.core-0.7.1b20230524/src/autogluon/core/hpo/space_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:04:15.595126 autogluon.core-0.7.1b20230524/src/autogluon/core/learner/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-24 09:03:54.000000 autogluon.core-0.7.1b20230524/src/autogluon/core/learner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-05-24 09:03:54.000000 autogluon.core-0.7.1b20230524/src/autogluon/core/learner/abstract_learner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:04:15.595126 autogluon.core-0.7.1b20230524/src/autogluon/core/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)    23243 2023-05-24 09:03:54.000000 autogluon.core-0.7.1b20230524/src/autogluon/core/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18113 2023-05-24 09:03:54.000000 autogluon.core-0.7.1b20230524/src/autogluon/core/metrics/classification_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-05-24 09:03:54.000000 autogluon.core-0.7.1b20230524/src/autogluon/core/metrics/quantile_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-05-24 09:03:54.000000 autogluon.core-0.7.1b20230524/src/autogluon/core/metrics/softclass_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:04:15.595126 autogluon.core-0.7.1b20230524/src/autogluon/core/models/
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-24 09:03:54.000000 autogluon.core-0.7.1b20230524/src/autogluon/core/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-05-24 09:03:54.000000 autogluon.core-0.7.1b20230524/src/autogluon/core/models/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:04:15.595126 autogluon.core-0.7.1b20230524/src/autogluon/core/models/abstract/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 09:03:54.000000 autogluon.core-0.7.1b20230524/src/autogluon/core/models/abstract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-05-24 09:03:54.000000 autogluon.core-0.7.1b20230524/src/autogluon/core/models/abstract/_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)    94023 2023-05-24 09:03:54.000000 autogluon.core-0.7.1b20230524/src/autogluon/core/models/abstract/abstract_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-05-24 09:03:54.000000 autogluon.core-0.7.1b20230524/src/autogluon/core/models/abstract/abstract_nn_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-05-24 09:03:54.000000 autogluon.core-0.7.1b20230524/src/autogluon/core/models/abstract/model_trial.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:04:15.599127 autogluon.core-0.7.1b20230524/src/autogluon/core/models/dummy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 09:03:54.000000 autogluon.core-0.7.1b20230524/src/autogluon/core/models/dummy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-05-24 09:03:54.000000 autogluon.core-0.7.1b20230524/src/autogluon/core/models/dummy/_dummy_quantile_regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-24 09:03:54.000000 autogluon.core-0.7.1b20230524/src/autogluon/core/models/dummy/dummy_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:04:15.599127 autogluon.core-0.7.1b20230524/src/autogluon/core/models/ensemble/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 09:03:54.000000 autogluon.core-0.7.1b20230524/src/autogluon/core/models/ensemble/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    59425 2023-05-24 09:03:54.000000 autogluon.core-0.7.1b20230524/src/autogluon/core/models/ensemble/bagged_ensemble_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    40465 2023-05-24 09:03:54.000000 autogluon.core-0.7.1b20230524/src/autogluon/core/models/ensemble/fold_fitting_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-05-24 09:03:54.000000 autogluon.core-0.7.1b20230524/src/autogluon/core/models/ensemble/ray_parallel_fold_fitting_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)    12762 2023-05-24 09:03:54.000000 autogluon.core-0.7.1b20230524/src/autogluon/core/models/ensemble/stacker_ensemble_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-05-24 09:03:54.000000 autogluon.core-0.7.1b20230524/src/autogluon/core/models/ensemble/weighted_ensemble_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:04:15.599127 autogluon.core-0.7.1b20230524/src/autogluon/core/models/greedy_ensemble/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 09:03:54.000000 autogluon.core-0.7.1b20230524/src/autogluon/core/models/greedy_ensemble/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-05-24 09:03:54.000000 autogluon.core-0.7.1b20230524/src/autogluon/core/models/greedy_ensemble/ensemble_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     6908 2023-05-24 09:03:54.000000 autogluon.core-0.7.1b20230524/src/autogluon/core/models/greedy_ensemble/greedy_weighted_ensemble_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:04:15.599127 autogluon.core-0.7.1b20230524/src/autogluon/core/pseudolabeling/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 09:03:54.000000 autogluon.core-0.7.1b20230524/src/autogluon/core/pseudolabeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-24 09:03:54.000000 autogluon.core-0.7.1b20230524/src/autogluon/core/pseudolabeling/pseudolabeling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:04:15.599127 autogluon.core-0.7.1b20230524/src/autogluon/core/ray/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 09:03:54.000000 autogluon.core-0.7.1b20230524/src/autogluon/core/ray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14720 2023-05-24 09:03:54.000000 autogluon.core-0.7.1b20230524/src/autogluon/core/ray/resources_calculator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:04:15.599127 autogluon.core-0.7.1b20230524/src/autogluon/core/scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-24 09:03:54.000000 autogluon.core-0.7.1b20230524/src/autogluon/core/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-24 09:03:54.000000 autogluon.core-0.7.1b20230524/src/autogluon/core/scheduler/reporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5782 2023-05-24 09:03:54.000000 autogluon.core-0.7.1b20230524/src/autogluon/core/scheduler/scheduler_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    15079 2023-05-24 09:03:54.000000 autogluon.core-0.7.1b20230524/src/autogluon/core/scheduler/seq_scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:04:15.599127 autogluon.core-0.7.1b20230524/src/autogluon/core/searcher/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-24 09:03:54.000000 autogluon.core-0.7.1b20230524/src/autogluon/core/searcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-05-24 09:03:54.000000 autogluon.core-0.7.1b20230524/src/autogluon/core/searcher/dummy_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-24 09:03:54.000000 autogluon.core-0.7.1b20230524/src/autogluon/core/searcher/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-05-24 09:03:54.000000 autogluon.core-0.7.1b20230524/src/autogluon/core/searcher/local_grid_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     3025 2023-05-24 09:03:54.000000 autogluon.core-0.7.1b20230524/src/autogluon/core/searcher/local_random_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     9740 2023-05-24 09:03:54.000000 autogluon.core-0.7.1b20230524/src/autogluon/core/searcher/local_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-05-24 09:03:54.000000 autogluon.core-0.7.1b20230524/src/autogluon/core/searcher/searcher_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-24 09:03:54.000000 autogluon.core-0.7.1b20230524/src/autogluon/core/space.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:04:15.599127 autogluon.core-0.7.1b20230524/src/autogluon/core/task/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 09:03:54.000000 autogluon.core-0.7.1b20230524/src/autogluon/core/task/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:04:15.599127 autogluon.core-0.7.1b20230524/src/autogluon/core/task/base/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-24 09:03:54.000000 autogluon.core-0.7.1b20230524/src/autogluon/core/task/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6547 2023-05-24 09:03:54.000000 autogluon.core-0.7.1b20230524/src/autogluon/core/task/base/base_task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:04:15.599127 autogluon.core-0.7.1b20230524/src/autogluon/core/trainer/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-24 09:03:54.000000 autogluon.core-0.7.1b20230524/src/autogluon/core/trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   169588 2023-05-24 09:03:54.000000 autogluon.core-0.7.1b20230524/src/autogluon/core/trainer/abstract_trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-05-24 09:03:54.000000 autogluon.core-0.7.1b20230524/src/autogluon/core/trainer/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:04:15.603127 autogluon.core-0.7.1b20230524/src/autogluon/core/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-24 09:03:54.000000 autogluon.core-0.7.1b20230524/src/autogluon/core/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-05-24 09:03:54.000000 autogluon.core-0.7.1b20230524/src/autogluon/core/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4669 2023-05-24 09:03:54.000000 autogluon.core-0.7.1b20230524/src/autogluon/core/utils/early_stopping.py
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-24 09:03:54.000000 autogluon.core-0.7.1b20230524/src/autogluon/core/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    36124 2023-05-24 09:03:54.000000 autogluon.core-0.7.1b20230524/src/autogluon/core/utils/feature_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-05-24 09:03:54.000000 autogluon.core-0.7.1b20230524/src/autogluon/core/utils/files.py
--rw-r--r--   0 runner    (1001) docker     (123)     9624 2023-05-24 09:03:54.000000 autogluon.core-0.7.1b20230524/src/autogluon/core/utils/infer_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:04:15.603127 autogluon.core-0.7.1b20230524/src/autogluon/core/utils/loaders/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-24 09:03:54.000000 autogluon.core-0.7.1b20230524/src/autogluon/core/utils/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-05-24 09:03:54.000000 autogluon.core-0.7.1b20230524/src/autogluon/core/utils/miscs.py
--rw-r--r--   0 runner    (1001) docker     (123)    11996 2023-05-24 09:03:54.000000 autogluon.core-0.7.1b20230524/src/autogluon/core/utils/plots.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:04:15.603127 autogluon.core-0.7.1b20230524/src/autogluon/core/utils/savers/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-24 09:03:54.000000 autogluon.core-0.7.1b20230524/src/autogluon/core/utils/savers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-05-24 09:03:54.000000 autogluon.core-0.7.1b20230524/src/autogluon/core/utils/time.py
--rw-r--r--   0 runner    (1001) docker     (123)    49348 2023-05-24 09:03:54.000000 autogluon.core-0.7.1b20230524/src/autogluon/core/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-05-24 09:03:54.000000 autogluon.core-0.7.1b20230524/src/autogluon/core/utils/version_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-24 09:04:15.000000 autogluon.core-0.7.1b20230524/src/autogluon/core/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:04:15.591126 autogluon.core-0.7.1b20230524/src/autogluon.core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12631 2023-05-24 09:04:15.000000 autogluon.core-0.7.1b20230524/src/autogluon.core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-05-24 09:04:15.000000 autogluon.core-0.7.1b20230524/src/autogluon.core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 09:04:15.000000 autogluon.core-0.7.1b20230524/src/autogluon.core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-24 09:04:15.000000 autogluon.core-0.7.1b20230524/src/autogluon.core.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-24 09:04:15.000000 autogluon.core-0.7.1b20230524/src/autogluon.core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-24 09:04:15.000000 autogluon.core-0.7.1b20230524/src/autogluon.core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 09:04:15.000000 autogluon.core-0.7.1b20230524/src/autogluon.core.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:03:59.485210 autogluon.core-0.7.1b20230525/
+-rw-r--r--   0 runner    (1001) docker     (123)    12631 2023-05-25 09:03:59.485210 autogluon.core-0.7.1b20230525/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 09:03:59.485210 autogluon.core-0.7.1b20230525/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-05-25 09:03:38.000000 autogluon.core-0.7.1b20230525/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:03:59.465210 autogluon.core-0.7.1b20230525/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:03:59.465210 autogluon.core-0.7.1b20230525/src/autogluon/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:03:59.469210 autogluon.core-0.7.1b20230525/src/autogluon/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-05-25 09:03:38.000000 autogluon.core-0.7.1b20230525/src/autogluon/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6556 2023-05-25 09:03:38.000000 autogluon.core-0.7.1b20230525/src/autogluon/core/_setup_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:03:59.469210 autogluon.core-0.7.1b20230525/src/autogluon/core/augmentation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 09:03:38.000000 autogluon.core-0.7.1b20230525/src/autogluon/core/augmentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9764 2023-05-25 09:03:38.000000 autogluon.core-0.7.1b20230525/src/autogluon/core/augmentation/distill_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:03:59.473209 autogluon.core-0.7.1b20230525/src/autogluon/core/calibrate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 09:03:38.000000 autogluon.core-0.7.1b20230525/src/autogluon/core/calibrate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-05-25 09:03:38.000000 autogluon.core-0.7.1b20230525/src/autogluon/core/calibrate/conformity_score.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-05-25 09:03:38.000000 autogluon.core-0.7.1b20230525/src/autogluon/core/calibrate/temperature_scaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-05-25 09:03:38.000000 autogluon.core-0.7.1b20230525/src/autogluon/core/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:03:59.473209 autogluon.core-0.7.1b20230525/src/autogluon/core/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-25 09:03:38.000000 autogluon.core-0.7.1b20230525/src/autogluon/core/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-05-25 09:03:38.000000 autogluon.core-0.7.1b20230525/src/autogluon/core/data/cleaner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14331 2023-05-25 09:03:38.000000 autogluon.core-0.7.1b20230525/src/autogluon/core/data/label_cleaner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-05-25 09:03:38.000000 autogluon.core-0.7.1b20230525/src/autogluon/core/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:03:59.473209 autogluon.core-0.7.1b20230525/src/autogluon/core/hpo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 09:03:38.000000 autogluon.core-0.7.1b20230525/src/autogluon/core/hpo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-25 09:03:38.000000 autogluon.core-0.7.1b20230525/src/autogluon/core/hpo/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-25 09:03:38.000000 autogluon.core-0.7.1b20230525/src/autogluon/core/hpo/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29675 2023-05-25 09:03:38.000000 autogluon.core-0.7.1b20230525/src/autogluon/core/hpo/executors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23977 2023-05-25 09:03:38.000000 autogluon.core-0.7.1b20230525/src/autogluon/core/hpo/ray_hpo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-05-25 09:03:38.000000 autogluon.core-0.7.1b20230525/src/autogluon/core/hpo/ray_tune_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-05-25 09:03:38.000000 autogluon.core-0.7.1b20230525/src/autogluon/core/hpo/ray_tune_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-05-25 09:03:38.000000 autogluon.core-0.7.1b20230525/src/autogluon/core/hpo/ray_tune_scheduler_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-05-25 09:03:38.000000 autogluon.core-0.7.1b20230525/src/autogluon/core/hpo/ray_tune_searcher_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-05-25 09:03:38.000000 autogluon.core-0.7.1b20230525/src/autogluon/core/hpo/space_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:03:59.473209 autogluon.core-0.7.1b20230525/src/autogluon/core/learner/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-25 09:03:38.000000 autogluon.core-0.7.1b20230525/src/autogluon/core/learner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-05-25 09:03:38.000000 autogluon.core-0.7.1b20230525/src/autogluon/core/learner/abstract_learner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:03:59.477209 autogluon.core-0.7.1b20230525/src/autogluon/core/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)    23243 2023-05-25 09:03:38.000000 autogluon.core-0.7.1b20230525/src/autogluon/core/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18113 2023-05-25 09:03:38.000000 autogluon.core-0.7.1b20230525/src/autogluon/core/metrics/classification_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-05-25 09:03:38.000000 autogluon.core-0.7.1b20230525/src/autogluon/core/metrics/quantile_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-05-25 09:03:38.000000 autogluon.core-0.7.1b20230525/src/autogluon/core/metrics/softclass_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:03:59.477209 autogluon.core-0.7.1b20230525/src/autogluon/core/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-25 09:03:38.000000 autogluon.core-0.7.1b20230525/src/autogluon/core/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-05-25 09:03:38.000000 autogluon.core-0.7.1b20230525/src/autogluon/core/models/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:03:59.477209 autogluon.core-0.7.1b20230525/src/autogluon/core/models/abstract/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 09:03:38.000000 autogluon.core-0.7.1b20230525/src/autogluon/core/models/abstract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-05-25 09:03:38.000000 autogluon.core-0.7.1b20230525/src/autogluon/core/models/abstract/_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)    94023 2023-05-25 09:03:38.000000 autogluon.core-0.7.1b20230525/src/autogluon/core/models/abstract/abstract_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-05-25 09:03:38.000000 autogluon.core-0.7.1b20230525/src/autogluon/core/models/abstract/abstract_nn_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-05-25 09:03:38.000000 autogluon.core-0.7.1b20230525/src/autogluon/core/models/abstract/model_trial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:03:59.477209 autogluon.core-0.7.1b20230525/src/autogluon/core/models/dummy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 09:03:38.000000 autogluon.core-0.7.1b20230525/src/autogluon/core/models/dummy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-05-25 09:03:38.000000 autogluon.core-0.7.1b20230525/src/autogluon/core/models/dummy/_dummy_quantile_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-25 09:03:38.000000 autogluon.core-0.7.1b20230525/src/autogluon/core/models/dummy/dummy_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:03:59.477209 autogluon.core-0.7.1b20230525/src/autogluon/core/models/ensemble/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 09:03:38.000000 autogluon.core-0.7.1b20230525/src/autogluon/core/models/ensemble/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59425 2023-05-25 09:03:38.000000 autogluon.core-0.7.1b20230525/src/autogluon/core/models/ensemble/bagged_ensemble_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40465 2023-05-25 09:03:38.000000 autogluon.core-0.7.1b20230525/src/autogluon/core/models/ensemble/fold_fitting_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-05-25 09:03:38.000000 autogluon.core-0.7.1b20230525/src/autogluon/core/models/ensemble/ray_parallel_fold_fitting_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12762 2023-05-25 09:03:38.000000 autogluon.core-0.7.1b20230525/src/autogluon/core/models/ensemble/stacker_ensemble_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-05-25 09:03:38.000000 autogluon.core-0.7.1b20230525/src/autogluon/core/models/ensemble/weighted_ensemble_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:03:59.477209 autogluon.core-0.7.1b20230525/src/autogluon/core/models/greedy_ensemble/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 09:03:38.000000 autogluon.core-0.7.1b20230525/src/autogluon/core/models/greedy_ensemble/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-05-25 09:03:38.000000 autogluon.core-0.7.1b20230525/src/autogluon/core/models/greedy_ensemble/ensemble_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6908 2023-05-25 09:03:38.000000 autogluon.core-0.7.1b20230525/src/autogluon/core/models/greedy_ensemble/greedy_weighted_ensemble_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:03:59.481210 autogluon.core-0.7.1b20230525/src/autogluon/core/pseudolabeling/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 09:03:38.000000 autogluon.core-0.7.1b20230525/src/autogluon/core/pseudolabeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-25 09:03:38.000000 autogluon.core-0.7.1b20230525/src/autogluon/core/pseudolabeling/pseudolabeling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:03:59.481210 autogluon.core-0.7.1b20230525/src/autogluon/core/ray/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 09:03:38.000000 autogluon.core-0.7.1b20230525/src/autogluon/core/ray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14720 2023-05-25 09:03:38.000000 autogluon.core-0.7.1b20230525/src/autogluon/core/ray/resources_calculator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:03:59.481210 autogluon.core-0.7.1b20230525/src/autogluon/core/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-25 09:03:38.000000 autogluon.core-0.7.1b20230525/src/autogluon/core/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-25 09:03:38.000000 autogluon.core-0.7.1b20230525/src/autogluon/core/scheduler/reporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5782 2023-05-25 09:03:38.000000 autogluon.core-0.7.1b20230525/src/autogluon/core/scheduler/scheduler_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15079 2023-05-25 09:03:38.000000 autogluon.core-0.7.1b20230525/src/autogluon/core/scheduler/seq_scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:03:59.481210 autogluon.core-0.7.1b20230525/src/autogluon/core/searcher/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-25 09:03:38.000000 autogluon.core-0.7.1b20230525/src/autogluon/core/searcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-05-25 09:03:38.000000 autogluon.core-0.7.1b20230525/src/autogluon/core/searcher/dummy_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-25 09:03:38.000000 autogluon.core-0.7.1b20230525/src/autogluon/core/searcher/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-05-25 09:03:38.000000 autogluon.core-0.7.1b20230525/src/autogluon/core/searcher/local_grid_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3025 2023-05-25 09:03:38.000000 autogluon.core-0.7.1b20230525/src/autogluon/core/searcher/local_random_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9740 2023-05-25 09:03:38.000000 autogluon.core-0.7.1b20230525/src/autogluon/core/searcher/local_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-05-25 09:03:38.000000 autogluon.core-0.7.1b20230525/src/autogluon/core/searcher/searcher_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-25 09:03:38.000000 autogluon.core-0.7.1b20230525/src/autogluon/core/space.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:03:59.481210 autogluon.core-0.7.1b20230525/src/autogluon/core/task/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 09:03:38.000000 autogluon.core-0.7.1b20230525/src/autogluon/core/task/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:03:59.481210 autogluon.core-0.7.1b20230525/src/autogluon/core/task/base/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-25 09:03:38.000000 autogluon.core-0.7.1b20230525/src/autogluon/core/task/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6547 2023-05-25 09:03:38.000000 autogluon.core-0.7.1b20230525/src/autogluon/core/task/base/base_task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:03:59.485210 autogluon.core-0.7.1b20230525/src/autogluon/core/trainer/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-25 09:03:38.000000 autogluon.core-0.7.1b20230525/src/autogluon/core/trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   169588 2023-05-25 09:03:38.000000 autogluon.core-0.7.1b20230525/src/autogluon/core/trainer/abstract_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-05-25 09:03:38.000000 autogluon.core-0.7.1b20230525/src/autogluon/core/trainer/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:03:59.485210 autogluon.core-0.7.1b20230525/src/autogluon/core/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-25 09:03:38.000000 autogluon.core-0.7.1b20230525/src/autogluon/core/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-05-25 09:03:38.000000 autogluon.core-0.7.1b20230525/src/autogluon/core/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4669 2023-05-25 09:03:38.000000 autogluon.core-0.7.1b20230525/src/autogluon/core/utils/early_stopping.py
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-25 09:03:38.000000 autogluon.core-0.7.1b20230525/src/autogluon/core/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36124 2023-05-25 09:03:38.000000 autogluon.core-0.7.1b20230525/src/autogluon/core/utils/feature_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-05-25 09:03:38.000000 autogluon.core-0.7.1b20230525/src/autogluon/core/utils/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9624 2023-05-25 09:03:38.000000 autogluon.core-0.7.1b20230525/src/autogluon/core/utils/infer_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:03:59.485210 autogluon.core-0.7.1b20230525/src/autogluon/core/utils/loaders/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-25 09:03:38.000000 autogluon.core-0.7.1b20230525/src/autogluon/core/utils/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-05-25 09:03:38.000000 autogluon.core-0.7.1b20230525/src/autogluon/core/utils/miscs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11996 2023-05-25 09:03:38.000000 autogluon.core-0.7.1b20230525/src/autogluon/core/utils/plots.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:03:59.485210 autogluon.core-0.7.1b20230525/src/autogluon/core/utils/savers/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-25 09:03:38.000000 autogluon.core-0.7.1b20230525/src/autogluon/core/utils/savers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-05-25 09:03:38.000000 autogluon.core-0.7.1b20230525/src/autogluon/core/utils/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49348 2023-05-25 09:03:38.000000 autogluon.core-0.7.1b20230525/src/autogluon/core/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-05-25 09:03:38.000000 autogluon.core-0.7.1b20230525/src/autogluon/core/utils/version_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-25 09:03:59.000000 autogluon.core-0.7.1b20230525/src/autogluon/core/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:03:59.469210 autogluon.core-0.7.1b20230525/src/autogluon.core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12631 2023-05-25 09:03:59.000000 autogluon.core-0.7.1b20230525/src/autogluon.core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4028 2023-05-25 09:03:59.000000 autogluon.core-0.7.1b20230525/src/autogluon.core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 09:03:59.000000 autogluon.core-0.7.1b20230525/src/autogluon.core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-25 09:03:59.000000 autogluon.core-0.7.1b20230525/src/autogluon.core.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-25 09:03:59.000000 autogluon.core-0.7.1b20230525/src/autogluon.core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-25 09:03:59.000000 autogluon.core-0.7.1b20230525/src/autogluon.core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 09:03:59.000000 autogluon.core-0.7.1b20230525/src/autogluon.core.egg-info/zip-safe
```

### Comparing `autogluon.core-0.7.1b20230524/PKG-INFO` & `autogluon.core-0.7.1b20230525/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.core
-Version: 0.7.1b20230524
+Version: 0.7.1b20230525
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.core-0.7.1b20230524/setup.py` & `autogluon.core-0.7.1b20230525/setup.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230524/src/autogluon/core/__init__.py` & `autogluon.core-0.7.1b20230525/src/autogluon/core/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230524/src/autogluon/core/_setup_utils.py` & `autogluon.core-0.7.1b20230525/src/autogluon/core/_setup_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,15 +89,15 @@
     with open(version_path, 'w') as f:
         f.write(f'"""This is the {AUTOGLUON} version file."""\n')
         f.write("__version__ = '{}'\n".format(version))
         f.write("__lite__ = {}\n".format(LITE_MODE))
 
 
 def default_setup_args(*, version, submodule):
-    from setuptools import find_packages
+    from setuptools import find_namespace_packages
     long_description = open(os.path.join(AUTOGLUON_ROOT_PATH, 'README.md')).read()
     if submodule is None:
         name = PACKAGE_NAME
     else:
         name = f'{PACKAGE_NAME}.{submodule}'
     setup_args = dict(
         name=name,
@@ -107,15 +107,15 @@
         description='AutoML for Image, Text, and Tabular Data',
         long_description=long_description,
         long_description_content_type='text/markdown',
         license='Apache-2.0',
         license_files=('../LICENSE', '../NOTICE'),
 
         # Package info
-        packages=find_packages('src'),
+        packages=find_namespace_packages('src', include=['autogluon.*']),
         package_dir={'': 'src'},
         namespace_packages=[AUTOGLUON],
         zip_safe=True,
         include_package_data=True,
         python_requires=PYTHON_REQUIRES,
         package_data={AUTOGLUON: [
             'LICENSE',
```

### Comparing `autogluon.core-0.7.1b20230524/src/autogluon/core/augmentation/distill_utils.py` & `autogluon.core-0.7.1b20230525/src/autogluon/core/augmentation/distill_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230524/src/autogluon/core/calibrate/conformity_score.py` & `autogluon.core-0.7.1b20230525/src/autogluon/core/calibrate/conformity_score.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230524/src/autogluon/core/calibrate/temperature_scaling.py` & `autogluon.core-0.7.1b20230525/src/autogluon/core/calibrate/temperature_scaling.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230524/src/autogluon/core/constants.py` & `autogluon.core-0.7.1b20230525/src/autogluon/core/constants.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230524/src/autogluon/core/data/cleaner.py` & `autogluon.core-0.7.1b20230525/src/autogluon/core/data/cleaner.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230524/src/autogluon/core/data/label_cleaner.py` & `autogluon.core-0.7.1b20230525/src/autogluon/core/data/label_cleaner.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230524/src/autogluon/core/dataset.py` & `autogluon.core-0.7.1b20230525/src/autogluon/core/dataset.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230524/src/autogluon/core/hpo/executors.py` & `autogluon.core-0.7.1b20230525/src/autogluon/core/hpo/executors.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230524/src/autogluon/core/hpo/ray_hpo.py` & `autogluon.core-0.7.1b20230525/src/autogluon/core/hpo/ray_hpo.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230524/src/autogluon/core/hpo/ray_tune_scheduler.py` & `autogluon.core-0.7.1b20230525/src/autogluon/core/hpo/ray_tune_scheduler.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230524/src/autogluon/core/hpo/ray_tune_scheduler_factory.py` & `autogluon.core-0.7.1b20230525/src/autogluon/core/hpo/ray_tune_scheduler_factory.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230524/src/autogluon/core/hpo/ray_tune_searcher_factory.py` & `autogluon.core-0.7.1b20230525/src/autogluon/core/hpo/ray_tune_searcher_factory.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230524/src/autogluon/core/hpo/space_converter.py` & `autogluon.core-0.7.1b20230525/src/autogluon/core/hpo/space_converter.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230524/src/autogluon/core/learner/abstract_learner.py` & `autogluon.core-0.7.1b20230525/src/autogluon/core/learner/abstract_learner.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230524/src/autogluon/core/metrics/__init__.py` & `autogluon.core-0.7.1b20230525/src/autogluon/core/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230524/src/autogluon/core/metrics/classification_metrics.py` & `autogluon.core-0.7.1b20230525/src/autogluon/core/metrics/classification_metrics.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230524/src/autogluon/core/metrics/quantile_metrics.py` & `autogluon.core-0.7.1b20230525/src/autogluon/core/metrics/quantile_metrics.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230524/src/autogluon/core/metrics/softclass_metrics.py` & `autogluon.core-0.7.1b20230525/src/autogluon/core/metrics/softclass_metrics.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230524/src/autogluon/core/models/_utils.py` & `autogluon.core-0.7.1b20230525/src/autogluon/core/models/_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230524/src/autogluon/core/models/abstract/_tags.py` & `autogluon.core-0.7.1b20230525/src/autogluon/core/models/abstract/_tags.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230524/src/autogluon/core/models/abstract/abstract_model.py` & `autogluon.core-0.7.1b20230525/src/autogluon/core/models/abstract/abstract_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230524/src/autogluon/core/models/abstract/abstract_nn_model.py` & `autogluon.core-0.7.1b20230525/src/autogluon/core/models/abstract/abstract_nn_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230524/src/autogluon/core/models/abstract/model_trial.py` & `autogluon.core-0.7.1b20230525/src/autogluon/core/models/abstract/model_trial.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230524/src/autogluon/core/models/dummy/_dummy_quantile_regressor.py` & `autogluon.core-0.7.1b20230525/src/autogluon/core/models/dummy/_dummy_quantile_regressor.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230524/src/autogluon/core/models/dummy/dummy_model.py` & `autogluon.core-0.7.1b20230525/src/autogluon/core/models/dummy/dummy_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230524/src/autogluon/core/models/ensemble/bagged_ensemble_model.py` & `autogluon.core-0.7.1b20230525/src/autogluon/core/models/ensemble/bagged_ensemble_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230524/src/autogluon/core/models/ensemble/fold_fitting_strategy.py` & `autogluon.core-0.7.1b20230525/src/autogluon/core/models/ensemble/fold_fitting_strategy.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230524/src/autogluon/core/models/ensemble/ray_parallel_fold_fitting_strategy.py` & `autogluon.core-0.7.1b20230525/src/autogluon/core/models/ensemble/ray_parallel_fold_fitting_strategy.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230524/src/autogluon/core/models/ensemble/stacker_ensemble_model.py` & `autogluon.core-0.7.1b20230525/src/autogluon/core/models/ensemble/stacker_ensemble_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230524/src/autogluon/core/models/ensemble/weighted_ensemble_model.py` & `autogluon.core-0.7.1b20230525/src/autogluon/core/models/ensemble/weighted_ensemble_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230524/src/autogluon/core/models/greedy_ensemble/ensemble_selection.py` & `autogluon.core-0.7.1b20230525/src/autogluon/core/models/greedy_ensemble/ensemble_selection.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230524/src/autogluon/core/models/greedy_ensemble/greedy_weighted_ensemble_model.py` & `autogluon.core-0.7.1b20230525/src/autogluon/core/models/greedy_ensemble/greedy_weighted_ensemble_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230524/src/autogluon/core/pseudolabeling/pseudolabeling.py` & `autogluon.core-0.7.1b20230525/src/autogluon/core/pseudolabeling/pseudolabeling.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230524/src/autogluon/core/ray/resources_calculator.py` & `autogluon.core-0.7.1b20230525/src/autogluon/core/ray/resources_calculator.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230524/src/autogluon/core/scheduler/scheduler_factory.py` & `autogluon.core-0.7.1b20230525/src/autogluon/core/scheduler/scheduler_factory.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230524/src/autogluon/core/scheduler/seq_scheduler.py` & `autogluon.core-0.7.1b20230525/src/autogluon/core/scheduler/seq_scheduler.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230524/src/autogluon/core/searcher/dummy_searcher.py` & `autogluon.core-0.7.1b20230525/src/autogluon/core/searcher/dummy_searcher.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230524/src/autogluon/core/searcher/local_grid_searcher.py` & `autogluon.core-0.7.1b20230525/src/autogluon/core/searcher/local_grid_searcher.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230524/src/autogluon/core/searcher/local_random_searcher.py` & `autogluon.core-0.7.1b20230525/src/autogluon/core/searcher/local_random_searcher.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230524/src/autogluon/core/searcher/local_searcher.py` & `autogluon.core-0.7.1b20230525/src/autogluon/core/searcher/local_searcher.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230524/src/autogluon/core/searcher/searcher_factory.py` & `autogluon.core-0.7.1b20230525/src/autogluon/core/searcher/searcher_factory.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230524/src/autogluon/core/space.py` & `autogluon.core-0.7.1b20230525/src/autogluon/core/space.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230524/src/autogluon/core/task/base/base_task.py` & `autogluon.core-0.7.1b20230525/src/autogluon/core/task/base/base_task.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230524/src/autogluon/core/trainer/abstract_trainer.py` & `autogluon.core-0.7.1b20230525/src/autogluon/core/trainer/abstract_trainer.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230524/src/autogluon/core/trainer/utils.py` & `autogluon.core-0.7.1b20230525/src/autogluon/core/trainer/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230524/src/autogluon/core/utils/decorators.py` & `autogluon.core-0.7.1b20230525/src/autogluon/core/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230524/src/autogluon/core/utils/early_stopping.py` & `autogluon.core-0.7.1b20230525/src/autogluon/core/utils/early_stopping.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230524/src/autogluon/core/utils/feature_selection.py` & `autogluon.core-0.7.1b20230525/src/autogluon/core/utils/feature_selection.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230524/src/autogluon/core/utils/files.py` & `autogluon.core-0.7.1b20230525/src/autogluon/core/utils/files.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230524/src/autogluon/core/utils/infer_utils.py` & `autogluon.core-0.7.1b20230525/src/autogluon/core/utils/infer_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230524/src/autogluon/core/utils/miscs.py` & `autogluon.core-0.7.1b20230525/src/autogluon/core/utils/miscs.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230524/src/autogluon/core/utils/plots.py` & `autogluon.core-0.7.1b20230525/src/autogluon/core/utils/plots.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230524/src/autogluon/core/utils/time.py` & `autogluon.core-0.7.1b20230525/src/autogluon/core/utils/time.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230524/src/autogluon/core/utils/utils.py` & `autogluon.core-0.7.1b20230525/src/autogluon/core/utils/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230524/src/autogluon/core/utils/version_utils.py` & `autogluon.core-0.7.1b20230525/src/autogluon/core/utils/version_utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,72 +1,50 @@
-import autogluon
-import importlib
 import pkgutil
-import pkg_resources
 import platform
+import re
 import sys
-
 from datetime import datetime
+from importlib.metadata import version, distribution
 
+import autogluon
 from autogluon.common.utils.nvutil import cudaInit, cudaSystemGetNVMLVersion
 from autogluon.common.utils.resource_utils import ResourceManager
 
-# We don't include test dependency here
-autogluon_extras_dict = {
-    'autogluon.core': ('all',),
-    'autogluon.common': (),
-    'autogluon.features': (),
-    'autogluon.timeseries': (),
-    'autogluon.tabular': ('all',),
-}
-
-# This is needed because some module are different in its import name and pip install name
-import_name_dict = {
-    'pillow': 'PIL',
-    'pytorch-lightning': 'pytorch_lightning',
-    'scikit-image': 'skimage',
-    'scikit-learn': 'sklearn',
-    'smart-open': 'smart_open',
-    'timm-clean': 'timm',
-}
-
 
 def _get_autogluon_versions():
     """Retrieve version of all autogluon subpackages and its dependencies"""
     versions = dict()
     for pkg in list(pkgutil.iter_modules(autogluon.__path__, autogluon.__name__ + '.')):
-        if pkg.name == 'autogluon.version':  # autogluon.version will be recognized as a submodule by pkgutil. We don't need it
+        # The following packages will be recognized as a submodule by pkgutil -exclude them.
+        if pkg.name in ['autogluon.version', 'autogluon.setup', 'autogluon._internal_']:
             continue
         try:
-            module = importlib.import_module(pkg.name)
-            versions[pkg.name] = module.__version__
-            versions.update(_get_dependency_versions(pkg.name, autogluon_extras_dict.get(pkg.name, ())))
+            versions[pkg.name] = version(pkg.name)
+            versions.update(_get_dependency_versions(pkg.name))
         except ImportError:
             versions[pkg.name] = None
     return versions
 
 
-def _get_dependency_versions(package, extras=()):
+def _get_dependency_versions(package):
     """Retrieve direct dependency of the given package
 
     Args:
         package (str): name of the package
-        extras (tuple, optional): extras in package dependency. Defaults to ().
     """
-    package = pkg_resources.working_set.by_key[package]
-    dependencies = [str(r.key) for r in package.requires(extras=extras)]
+    # Get all requires for the package
+    dependencies = distribution(package).requires
+    # Filter-out test dependencies
+    dependencies = [req for req in dependencies if not bool(re.search('extra.*test', req))]
+    # keep only package name
+    dependencies = [re.findall('[a-zA-Z0-9_\\-]+', req)[0].strip() for req in dependencies]
     versions = dict()
     for dependency in dependencies:
-        dependency = import_name_dict.get(dependency, dependency)
         try:
-            module = importlib.import_module(dependency)
-            version = getattr(module, "__version__", None)
-            if version is None:
-                version = getattr(module, "__VERSION__", None)
-            versions[dependency] = version
+            versions[dependency] = version(dependency)
         except ImportError:
             versions[dependency] = None
     return versions
 
 
 def _get_sys_info():
     """Retrieve system information"""
@@ -102,15 +80,15 @@
     It comprises info about hosting operation system, autogluon subpackage versions,
     and versions of other installed relative packages.
     """
     sys_info = _get_sys_info()
     versions = _get_autogluon_versions()
     sorted_keys = sorted(versions.keys(), key=lambda x: x.lower())
 
-    maxlen = max(len(x) for x in versions)
+    maxlen = 0 if len(versions) == 0 else max(len(x) for x in versions)
     print("\nINSTALLED VERSIONS")
     print("------------------")
     for k, v in sys_info.items():
         print(f"{k:<{maxlen}}: {v}")
     print("")
     for k in sorted_keys:
         print(f"{k:<{maxlen}}: {versions[k]}")
```

### Comparing `autogluon.core-0.7.1b20230524/src/autogluon.core.egg-info/PKG-INFO` & `autogluon.core-0.7.1b20230525/src/autogluon.core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.core
-Version: 0.7.1b20230524
+Version: 0.7.1b20230525
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.core-0.7.1b20230524/src/autogluon.core.egg-info/SOURCES.txt` & `autogluon.core-0.7.1b20230525/src/autogluon.core.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 setup.py
-src/autogluon/__init__.py
 src/autogluon.core.egg-info/PKG-INFO
 src/autogluon.core.egg-info/SOURCES.txt
 src/autogluon.core.egg-info/dependency_links.txt
 src/autogluon.core.egg-info/namespace_packages.txt
 src/autogluon.core.egg-info/requires.txt
 src/autogluon.core.egg-info/top_level.txt
 src/autogluon.core.egg-info/zip-safe
```

