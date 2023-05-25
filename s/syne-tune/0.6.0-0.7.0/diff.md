# Comparing `tmp/syne_tune-0.6.0.tar.gz` & `tmp/syne_tune-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syne_tune-0.6.0.tar", last modified: Mon May  8 09:47:34 2023, max compression
+gzip compressed data, was "syne_tune-0.7.0.tar", last modified: Thu May 25 13:19:49 2023, max compression
```

## Comparing `syne_tune-0.6.0.tar` & `syne_tune-0.7.0.tar`

### file list

```diff
@@ -1,291 +1,303 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:47:34.953970 syne_tune-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-05-08 09:47:22.000000 syne_tune-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-08 09:47:22.000000 syne_tune-0.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-08 09:47:22.000000 syne_tune-0.6.0/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)    19009 2023-05-08 09:47:34.953970 syne_tune-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18216 2023-05-08 09:47:22.000000 syne_tune-0.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-08 09:47:34.953970 syne_tune-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-05-08 09:47:23.000000 syne_tune-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:47:34.929970 syne_tune-0.6.0/syne_tune/
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:47:34.929970 syne_tune-0.6.0/syne_tune/backend/
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15659 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/backend/local_backend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:47:34.933970 syne_tune-0.6.0/syne_tune/backend/python_backend/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/backend/python_backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/backend/python_backend/python_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/backend/python_backend/python_entrypoint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:47:34.933970 syne_tune-0.6.0/syne_tune/backend/sagemaker_backend/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/backend/sagemaker_backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/backend/sagemaker_backend/custom_framework.py
--rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/backend/sagemaker_backend/instance-types-cost.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/backend/sagemaker_backend/instance_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    24042 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/backend/sagemaker_backend/sagemaker_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    21131 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/backend/sagemaker_backend/sagemaker_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:47:34.933970 syne_tune-0.6.0/syne_tune/backend/simulator_backend/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/backend/simulator_backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/backend/simulator_backend/events.py
--rw-r--r--   0 runner    (1001) docker     (123)    22590 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/backend/simulator_backend/simulator_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     6643 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/backend/simulator_backend/simulator_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/backend/simulator_backend/time_keeper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/backend/time_keeper.py
--rw-r--r--   0 runner    (1001) docker     (123)    14202 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/backend/trial_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/backend/trial_status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:47:34.933970 syne_tune-0.6.0/syne_tune/blackbox_repository/
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/blackbox_repository/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9224 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/blackbox_repository/blackbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     9231 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/blackbox_repository/blackbox_offline.py
--rw-r--r--   0 runner    (1001) docker     (123)    22192 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/blackbox_repository/blackbox_surrogate.py
--rw-r--r--   0 runner    (1001) docker     (123)    17442 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/blackbox_repository/blackbox_tabular.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:47:34.933970 syne_tune-0.6.0/syne_tune/blackbox_repository/conversion_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/blackbox_repository/conversion_scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/blackbox_repository/conversion_scripts/blackbox_recipe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/blackbox_repository/conversion_scripts/recipes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:47:34.933970 syne_tune-0.6.0/syne_tune/blackbox_repository/conversion_scripts/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/blackbox_repository/conversion_scripts/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7925 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/blackbox_repository/conversion_scripts/scripts/fcnet_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     5606 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/blackbox_repository/conversion_scripts/scripts/icml2020_import.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:47:34.933970 syne_tune-0.6.0/syne_tune/blackbox_repository/conversion_scripts/scripts/lcbench/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/blackbox_repository/conversion_scripts/scripts/lcbench/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10223 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/blackbox_repository/conversion_scripts/scripts/lcbench/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5128 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/blackbox_repository/conversion_scripts/scripts/lcbench/lcbench.py
--rw-r--r--   0 runner    (1001) docker     (123)    10468 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/blackbox_repository/conversion_scripts/scripts/nasbench201_import.py
--rw-r--r--   0 runner    (1001) docker     (123)    11750 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/blackbox_repository/conversion_scripts/scripts/pd1_import.py
--rw-r--r--   0 runner    (1001) docker     (123)    17778 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/blackbox_repository/conversion_scripts/scripts/yahpo_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     4770 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/blackbox_repository/conversion_scripts/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8211 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/blackbox_repository/repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/blackbox_repository/serialize.py
--rw-r--r--   0 runner    (1001) docker     (123)    18952 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/blackbox_repository/simulated_tabular_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/blackbox_repository/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:47:34.933970 syne_tune-0.6.0/syne_tune/callbacks/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22237 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/callbacks/hyperband_remove_checkpoints_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)     6937 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/callbacks/hyperband_remove_checkpoints_score.py
--rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/callbacks/remove_checkpoints_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)     6940 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/callbacks/tensorboard_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)    43889 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/config_space.py
--rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:47:34.933970 syne_tune-0.6.0/syne_tune/experiments/
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/experiments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17083 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/experiments/experiment_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/experiments/results_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/num_gpu.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:47:34.937970 syne_tune-0.6.0/syne_tune/optimizer/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36483 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/baselines.py
--rw-r--r--   0 runner    (1001) docker     (123)    12102 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:47:34.937970 syne_tune-0.6.0/syne_tune/optimizer/schedulers/
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17051 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/fifo.py
--rw-r--r--   0 runner    (1001) docker     (123)    59571 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/hyperband.py
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/hyperband_checkpoint_removal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4329 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/hyperband_cost_promotion.py
--rw-r--r--   0 runner    (1001) docker     (123)    12528 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/hyperband_pasha.py
--rw-r--r--   0 runner    (1001) docker     (123)    11942 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/hyperband_promotion.py
--rw-r--r--   0 runner    (1001) docker     (123)     5320 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/hyperband_rush.py
--rw-r--r--   0 runner    (1001) docker     (123)    15115 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/hyperband_stopping.py
--rw-r--r--   0 runner    (1001) docker     (123)     5565 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/median_stopping_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/multi_fidelity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:47:34.937970 syne_tune-0.6.0/syne_tune/optimizer/schedulers/multiobjective/
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/multiobjective/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7697 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/multiobjective/linear_scalarizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11212 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/multiobjective/moasha.py
--rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/multiobjective/multi_objective_regularized_evolution.py
--rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/multiobjective/multiobjective_priority.py
--rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/multiobjective/non_dominated_priority.py
--rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/multiobjective/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:47:34.937970 syne_tune-0.6.0/syne_tune/optimizer/schedulers/neuralbands/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/neuralbands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/neuralbands/networks.py
--rw-r--r--   0 runner    (1001) docker     (123)    13166 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/neuralbands/neuralband.py
--rw-r--r--   0 runner    (1001) docker     (123)    22189 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/neuralbands/neuralband_supplement.py
--rw-r--r--   0 runner    (1001) docker     (123)    15111 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/pbt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/random_seeds.py
--rw-r--r--   0 runner    (1001) docker     (123)     8676 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/ray_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/remove_checkpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     4899 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/scheduler_searcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:47:34.941970 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:47:34.941970 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:47:34.941970 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/datatypes/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/datatypes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/datatypes/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/datatypes/config_ext.py
--rw-r--r--   0 runner    (1001) docker     (123)    13227 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/datatypes/tuning_job_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:47:34.941970 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     6108 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/custom_op.py
--rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)    40693 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gluon.py
--rw-r--r--   0 runner    (1001) docker     (123)    14767 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gluon_blocks_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    11243 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gp_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gp_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     8115 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gpr_mcmc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:47:34.941970 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13474 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/gp_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/likelihood.py
--rw-r--r--   0 runner    (1001) docker     (123)    15300 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/posterior_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    19410 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:47:34.941970 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/independent/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/independent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5096 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/independent/gpind_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    11496 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/independent/likelihood.py
--rw-r--r--   0 runner    (1001) docker     (123)    10699 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/independent/posterior_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:47:34.941970 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10740 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6635 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/cross_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)    13361 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/exponential_decay.py
--rw-r--r--   0 runner    (1001) docker     (123)     4869 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/fabolas.py
--rw-r--r--   0 runner    (1001) docker     (123)    10162 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/freeze_thaw.py
--rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/product_kernel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/range_kernel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:47:34.945970 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18991 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/freeze_thaw.py
--rw-r--r--   0 runner    (1001) docker     (123)     4068 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/gpiss_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    42009 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/issm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7009 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/likelihood.py
--rw-r--r--   0 runner    (1001) docker     (123)     5704 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/model_params.py
--rw-r--r--   0 runner    (1001) docker     (123)    27024 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/posterior_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     9563 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/likelihood.py
--rw-r--r--   0 runner    (1001) docker     (123)     4394 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/mean.py
--rw-r--r--   0 runner    (1001) docker     (123)    13024 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/optimization_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16413 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/posterior_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    13238 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/posterior_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/slice.py
--rw-r--r--   0 runner    (1001) docker     (123)    10095 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/target_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)    11507 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/warping.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:47:34.945970 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:47:34.945970 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6595 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/cost_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    15944 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/linear_cost_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    14332 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/sklearn_cost_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5928 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost_fifo_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/gp_mcmc_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    20255 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/gp_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    17363 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/gpiss_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4499 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/kernel_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    14930 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/meanstd_acqfunc.py
--rw-r--r--   0 runner    (1001) docker     (123)    21050 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/meanstd_acqfunc_impl.py
--rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/model_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/model_skipopt.py
--rw-r--r--   0 runner    (1001) docker     (123)    18366 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/model_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    13847 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/subsample_state_multi_fidelity.py
--rw-r--r--   0 runner    (1001) docker     (123)     5486 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/subsample_state_single_fidelity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:47:34.945970 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12602 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/base_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)    15826 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/bo_algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)    13194 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/bo_algorithm_components.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/defaults.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:47:34.945970 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6840 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/comparison_gpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/debug_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     7781 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/test_objects.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:47:34.945970 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bore/
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10866 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bore/bore.py
--rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bore/de.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bore/gp_classififer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bore/mlp_classififer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bore/multi_fidelity_bore.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:47:34.945970 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/botorch/
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/botorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11845 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/botorch/botorch_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bracket_distribution.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:47:34.945970 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/constrained/
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/constrained/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/constrained/constrained_gp_fifo_searcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:47:34.945970 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/cost_aware/
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/cost_aware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/cost_aware/cost_aware_gp_fifo_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     6690 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/cost_aware/cost_aware_gp_multifidelity_searcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:47:34.949970 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/dyhpo/
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/dyhpo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18590 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/dyhpo/dyhpo_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    10575 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/dyhpo/hyperband_dyhpo.py
--rw-r--r--   0 runner    (1001) docker     (123)    15795 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/gp_fifo_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    13455 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/gp_multifidelity_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    42280 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/gp_searcher_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     9020 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/gp_searcher_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:47:34.949970 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/hypertune/
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/hypertune/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/hypertune/hypertune_bracket_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     4270 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/hypertune/hypertune_searcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:47:34.949970 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/kde/
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/kde/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17166 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/kde/kde_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     5089 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/kde/multi_fidelity_kde_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    34657 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/model_based_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    15391 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/random_grid_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     6314 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/regularized_evolution.py
--rw-r--r--   0 runner    (1001) docker     (123)    14507 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    14811 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/searcher_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/searcher_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)     6798 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/searcher_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:47:34.949970 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     6267 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/utils/default_arguments.py
--rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/utils/exclusion_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    12859 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/utils/hp_ranges.py
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/utils/hp_ranges_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    31161 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/utils/hp_ranges_impl.py
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/utils/scaling.py
--rw-r--r--   0 runner    (1001) docker     (123)     5835 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/utils/warmstarting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:47:34.949970 syne_tune-0.6.0/syne_tune/optimizer/schedulers/synchronous/
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/synchronous/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34062 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/synchronous/dehb.py
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/synchronous/dehb_bracket.py
--rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/synchronous/dehb_bracket_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    19672 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/synchronous/hyperband.py
--rw-r--r--   0 runner    (1001) docker     (123)    10044 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/synchronous/hyperband_bracket.py
--rw-r--r--   0 runner    (1001) docker     (123)     7689 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/synchronous/hyperband_bracket_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    12482 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/synchronous/hyperband_impl.py
--rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/synchronous/hyperband_rung_system.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:47:34.949970 syne_tune-0.6.0/syne_tune/optimizer/schedulers/transfer_learning/
--rw-r--r--   0 runner    (1001) docker     (123)     7229 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/transfer_learning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6999 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/transfer_learning/bounding_box.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:47:34.949970 syne_tune-0.6.0/syne_tune/optimizer/schedulers/transfer_learning/quantile_based/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/transfer_learning/quantile_based/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/transfer_learning/quantile_based/normalization_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     7282 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/transfer_learning/quantile_based/quantile_based_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     4499 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/transfer_learning/rush.py
--rw-r--r--   0 runner    (1001) docker     (123)     8320 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/transfer_learning/zero_shot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:47:34.949970 syne_tune-0.6.0/syne_tune/optimizer/schedulers/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/utils/simple_profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/optimizer/schedulers/utils/successive_halving.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:47:34.949970 syne_tune-0.6.0/syne_tune/remote/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/remote/estimators.py
--rw-r--r--   0 runner    (1001) docker     (123)    14281 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/remote/remote_launcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/remote/remote_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/remote/remote_metrics_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)     6366 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     5787 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/results_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)     9002 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/stopping_criterion.py
--rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/try_import.py
--rw-r--r--   0 runner    (1001) docker     (123)    31764 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/tuner.py
--rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/tuner_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)    10789 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/tuning_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    10441 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:47:34.953970 syne_tune-0.6.0/syne_tune/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/utils/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/utils/config_as_json.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/utils/parse_bool.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-08 09:47:23.000000 syne_tune-0.6.0/syne_tune/version
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:47:34.929970 syne_tune-0.6.0/syne_tune.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19009 2023-05-08 09:47:34.000000 syne_tune-0.6.0/syne_tune.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14803 2023-05-08 09:47:34.000000 syne_tune-0.6.0/syne_tune.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 09:47:34.000000 syne_tune-0.6.0/syne_tune.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-08 09:47:34.000000 syne_tune-0.6.0/syne_tune.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-08 09:47:34.000000 syne_tune-0.6.0/syne_tune.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:19:49.343604 syne_tune-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-05-25 13:19:34.000000 syne_tune-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-25 13:19:34.000000 syne_tune-0.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-25 13:19:34.000000 syne_tune-0.7.0/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)    19123 2023-05-25 13:19:49.343604 syne_tune-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18283 2023-05-25 13:19:34.000000 syne_tune-0.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-25 13:19:49.343604 syne_tune-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-05-25 13:19:34.000000 syne_tune-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:19:49.319603 syne_tune-0.7.0/syne_tune/
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:19:49.319603 syne_tune-0.7.0/syne_tune/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15659 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/backend/local_backend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:19:49.319603 syne_tune-0.7.0/syne_tune/backend/python_backend/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/backend/python_backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/backend/python_backend/python_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/backend/python_backend/python_entrypoint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:19:49.319603 syne_tune-0.7.0/syne_tune/backend/sagemaker_backend/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/backend/sagemaker_backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/backend/sagemaker_backend/custom_framework.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/backend/sagemaker_backend/instance-types-cost.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/backend/sagemaker_backend/instance_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24042 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/backend/sagemaker_backend/sagemaker_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21131 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/backend/sagemaker_backend/sagemaker_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:19:49.319603 syne_tune-0.7.0/syne_tune/backend/simulator_backend/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/backend/simulator_backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/backend/simulator_backend/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22590 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/backend/simulator_backend/simulator_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6643 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/backend/simulator_backend/simulator_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/backend/simulator_backend/time_keeper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/backend/time_keeper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14202 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/backend/trial_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/backend/trial_status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:19:49.323603 syne_tune-0.7.0/syne_tune/blackbox_repository/
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/blackbox_repository/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9224 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/blackbox_repository/blackbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9231 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/blackbox_repository/blackbox_offline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22192 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/blackbox_repository/blackbox_surrogate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17442 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/blackbox_repository/blackbox_tabular.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:19:49.323603 syne_tune-0.7.0/syne_tune/blackbox_repository/conversion_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/blackbox_repository/conversion_scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/blackbox_repository/conversion_scripts/blackbox_recipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/blackbox_repository/conversion_scripts/recipes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:19:49.323603 syne_tune-0.7.0/syne_tune/blackbox_repository/conversion_scripts/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/blackbox_repository/conversion_scripts/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7925 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/blackbox_repository/conversion_scripts/scripts/fcnet_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5606 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/blackbox_repository/conversion_scripts/scripts/icml2020_import.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:19:49.323603 syne_tune-0.7.0/syne_tune/blackbox_repository/conversion_scripts/scripts/lcbench/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/blackbox_repository/conversion_scripts/scripts/lcbench/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10223 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/blackbox_repository/conversion_scripts/scripts/lcbench/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5128 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/blackbox_repository/conversion_scripts/scripts/lcbench/lcbench.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10468 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/blackbox_repository/conversion_scripts/scripts/nasbench201_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11750 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/blackbox_repository/conversion_scripts/scripts/pd1_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17778 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/blackbox_repository/conversion_scripts/scripts/yahpo_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4770 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/blackbox_repository/conversion_scripts/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8211 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/blackbox_repository/repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/blackbox_repository/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18952 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/blackbox_repository/simulated_tabular_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/blackbox_repository/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:19:49.323603 syne_tune-0.7.0/syne_tune/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22237 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/callbacks/hyperband_remove_checkpoints_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6937 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/callbacks/hyperband_remove_checkpoints_score.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/callbacks/remove_checkpoints_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6940 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/callbacks/tensorboard_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43893 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/config_space.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:19:49.323603 syne_tune-0.7.0/syne_tune/experiments/
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/experiments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5633 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/experiments/aggregate_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17083 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/experiments/experiment_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14601 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/experiments/plot_per_trial.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29593 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/experiments/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17712 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/experiments/results_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/num_gpu.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:19:49.323603 syne_tune-0.7.0/syne_tune/optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37757 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/baselines.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12102 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:19:49.327603 syne_tune-0.7.0/syne_tune/optimizer/schedulers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17051 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/fifo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59571 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/hyperband.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/hyperband_checkpoint_removal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4329 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/hyperband_cost_promotion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12528 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/hyperband_pasha.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11942 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/hyperband_promotion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5320 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/hyperband_rush.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15115 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/hyperband_stopping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5565 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/median_stopping_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/multi_fidelity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:19:49.327603 syne_tune-0.7.0/syne_tune/optimizer/schedulers/multiobjective/
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/multiobjective/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7697 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/multiobjective/linear_scalarizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11212 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/multiobjective/moasha.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/multiobjective/multi_objective_regularized_evolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/multiobjective/multiobjective_priority.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/multiobjective/non_dominated_priority.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8564 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/multiobjective/nsga2_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/multiobjective/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:19:49.327603 syne_tune-0.7.0/syne_tune/optimizer/schedulers/neuralbands/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/neuralbands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/neuralbands/networks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13166 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/neuralbands/neuralband.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22189 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/neuralbands/neuralband_supplement.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15111 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/pbt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/random_seeds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8676 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/ray_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/remove_checkpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4899 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/scheduler_searcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:19:49.331603 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:19:49.331603 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:19:49.331603 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/datatypes/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/datatypes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/datatypes/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/datatypes/config_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13227 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/datatypes/tuning_job_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:19:49.331603 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6108 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/custom_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40693 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gluon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14767 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gluon_blocks_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11243 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gp_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gp_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8115 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gpr_mcmc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:19:49.331603 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13474 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/gp_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/likelihood.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15300 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/posterior_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19410 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:19:49.331603 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/independent/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/independent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5096 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/independent/gpind_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11496 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/independent/likelihood.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10699 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/independent/posterior_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:19:49.335604 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10740 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6635 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/cross_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13361 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/exponential_decay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4869 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/fabolas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10162 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/freeze_thaw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/product_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/range_kernel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:19:49.335604 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18991 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/freeze_thaw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4068 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/gpiss_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42009 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/issm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7009 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/likelihood.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5704 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/model_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27009 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/posterior_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9563 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/likelihood.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4394 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/mean.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13024 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/optimization_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16368 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/posterior_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13238 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/posterior_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/slice.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10095 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/target_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11507 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/warping.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:19:49.335604 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:19:49.335604 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6595 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/cost_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15944 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/linear_cost_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14332 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/sklearn_cost_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5848 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost_fifo_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6919 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/estimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/gp_mcmc_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18163 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/gp_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17447 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/gpiss_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4499 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/kernel_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15047 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/meanstd_acqfunc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21176 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/meanstd_acqfunc_impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/model_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/model_skipopt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16104 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/model_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/sklearn_estimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/sklearn_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13847 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/subsample_state_multi_fidelity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5486 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/subsample_state_single_fidelity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:19:49.335604 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/sklearn/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/sklearn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/sklearn/estimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/sklearn/predictor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:19:49.339604 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12949 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/base_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16077 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/bo_algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13322 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/bo_algorithm_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/defaults.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:19:49.339604 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/comparison_gpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/debug_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7781 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/test_objects.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:19:49.339604 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bore/
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10866 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bore/bore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bore/de.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bore/gp_classififer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bore/mlp_classififer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bore/multi_fidelity_bore.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:19:49.339604 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/botorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/botorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11845 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/botorch/botorch_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bracket_distribution.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:19:49.339604 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/constrained/
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/constrained/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/constrained/constrained_gp_fifo_searcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:19:49.339604 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/cost_aware/
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/cost_aware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6762 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/cost_aware/cost_aware_gp_fifo_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6610 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/cost_aware/cost_aware_gp_multifidelity_searcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:19:49.339604 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/dyhpo/
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/dyhpo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18542 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/dyhpo/dyhpo_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10575 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/dyhpo/hyperband_dyhpo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15779 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/gp_fifo_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13439 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/gp_multifidelity_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42012 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/gp_searcher_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9020 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/gp_searcher_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:19:49.339604 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/hypertune/
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/hypertune/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/hypertune/hypertune_bracket_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4270 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/hypertune/hypertune_searcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:19:49.339604 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/kde/
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/kde/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17166 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/kde/kde_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5089 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/kde/multi_fidelity_kde_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34597 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/model_based_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15488 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/random_grid_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6550 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/regularized_evolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14507 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14811 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/searcher_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/searcher_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6798 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/searcher_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:19:49.339604 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6267 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/utils/default_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/utils/exclusion_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12859 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/utils/hp_ranges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/utils/hp_ranges_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31161 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/utils/hp_ranges_impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/utils/scaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5835 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/utils/warmstarting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:19:49.343604 syne_tune-0.7.0/syne_tune/optimizer/schedulers/synchronous/
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/synchronous/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34062 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/synchronous/dehb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/synchronous/dehb_bracket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/synchronous/dehb_bracket_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19672 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/synchronous/hyperband.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10044 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/synchronous/hyperband_bracket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7689 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/synchronous/hyperband_bracket_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12482 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/synchronous/hyperband_impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/synchronous/hyperband_rung_system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:19:49.343604 syne_tune-0.7.0/syne_tune/optimizer/schedulers/transfer_learning/
+-rw-r--r--   0 runner    (1001) docker     (123)     7229 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/transfer_learning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6999 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/transfer_learning/bounding_box.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:19:49.343604 syne_tune-0.7.0/syne_tune/optimizer/schedulers/transfer_learning/quantile_based/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/transfer_learning/quantile_based/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/transfer_learning/quantile_based/normalization_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7282 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/transfer_learning/quantile_based/quantile_based_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4499 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/transfer_learning/rush.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8320 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/transfer_learning/zero_shot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:19:49.343604 syne_tune-0.7.0/syne_tune/optimizer/schedulers/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/utils/simple_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/utils/successive_halving.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:19:49.343604 syne_tune-0.7.0/syne_tune/remote/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/remote/estimators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14281 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/remote/remote_launcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/remote/remote_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/remote/remote_metrics_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/remote/scheduling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6366 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5787 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/results_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9002 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/stopping_criterion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/try_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31764 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/tuner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/tuner_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10789 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/tuning_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10441 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:19:49.343604 syne_tune-0.7.0/syne_tune/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/utils/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/utils/config_as_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/utils/parse_bool.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/version
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:19:49.319603 syne_tune-0.7.0/syne_tune.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19123 2023-05-25 13:19:49.000000 syne_tune-0.7.0/syne_tune.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15453 2023-05-25 13:19:49.000000 syne_tune-0.7.0/syne_tune.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 13:19:49.000000 syne_tune-0.7.0/syne_tune.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-05-25 13:19:49.000000 syne_tune-0.7.0/syne_tune.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-25 13:19:49.000000 syne_tune-0.7.0/syne_tune.egg-info/top_level.txt
```

### Comparing `syne_tune-0.6.0/LICENSE` & `syne_tune-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/PKG-INFO` & `syne_tune-0.7.0/syne_tune.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 Metadata-Version: 2.1
-Name: syne_tune
-Version: 0.6.0
+Name: syne-tune
+Version: 0.7.0
 Summary: Distributed Hyperparameter Optimization on SageMaker
 Author: AWS
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
-Provides-Extra: raytune
-Provides-Extra: bore
-Provides-Extra: kde
 Provides-Extra: gpsearchers
-Provides-Extra: benchmarks
-Provides-Extra: blackbox-repository
-Provides-Extra: aws
-Provides-Extra: yahpo
+Provides-Extra: kde
 Provides-Extra: dev
+Provides-Extra: aws
 Provides-Extra: moo
+Provides-Extra: visual
+Provides-Extra: blackbox-repository
+Provides-Extra: benchmarks
+Provides-Extra: yahpo
+Provides-Extra: raytune
+Provides-Extra: botorch
+Provides-Extra: bore
 Provides-Extra: extra
 License-File: LICENSE
 License-File: NOTICE
 
 # Syne Tune: Large-Scale and Reproducible Hyperparameter Optimization
 
 [![release](https://img.shields.io/github/v/release/awslabs/syne-tune)](https://pypi.org/project/syne-tune/)
@@ -86,20 +88,20 @@
 from syne_tune import Reporter
 from argparse import ArgumentParser
 
 if __name__ == '__main__':
     root = logging.getLogger()
     root.setLevel(logging.INFO)
     parser = ArgumentParser()
-    parser.add_argument('--steps', type=int)
+    parser.add_argument('--epochs', type=int)
     parser.add_argument('--width', type=float)
     parser.add_argument('--height', type=float)
     args, _ = parser.parse_known_args()
     report = Reporter()
-    for step in range(args.steps):
+    for step in range(args.epochs):
         time.sleep(0.1)
         dummy_score = 1.0 / (0.1 + args.width * step / 100) + args.height * 0.1
         # Feed the score back to Syne Tune.
         report(epoch=step + 1, mean_loss=dummy_score)
 ```
 
 Once you have a script reporting metric, you can launch a tuning as-follow:
@@ -115,15 +117,15 @@
 config_space = {
     'width': randint(1, 20),
     'height': randint(1, 20),
     'epochs': 100,
 }
 
 tuner = Tuner(
-    trial_backend=LocalBackend(entry_point='train_height.py'),
+    trial_backend=LocalBackend(entry_point='train_height_simple.py'),
     scheduler=ASHA(
         config_space,
         metric='mean_loss',
         resource_attr='epoch',
         max_resource_attr="epochs",
         search_options={'debug_log': False},
     ),
@@ -171,14 +173,15 @@
 
 ## Supported multi-objective optimization methods
 
 Method | Reference | Searcher | Asynchronous? | Multi-fidelity? | Transfer?
 :--- | :---: | :---: | :---: | :---: | :---: 
 Constrained Bayesian Optimization | Gardner, et al. (2014) | model-based | yes | no | no
 MOASHA | Schmucker, et al. (2021) | random | yes | yes | no
+NSGA-2 | Deb, et al. (2002) | evolutionary | no | no | no
 
 HPO methods listed can be used in a multi-objective setting by scalarization or non-dominated sorting. See [multiobjective_priority.py](syne_tune/optimizers/schedulers/multiobjective/multiobjective_priority.py) for details.
 
 ## Examples
 
 You will find many examples in the [examples/](examples/) folder illustrating
 different functionalities provided by Syne Tune. For example:
```

### Comparing `syne_tune-0.6.0/README.md` & `syne_tune-0.7.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -60,20 +60,20 @@
 from syne_tune import Reporter
 from argparse import ArgumentParser
 
 if __name__ == '__main__':
     root = logging.getLogger()
     root.setLevel(logging.INFO)
     parser = ArgumentParser()
-    parser.add_argument('--steps', type=int)
+    parser.add_argument('--epochs', type=int)
     parser.add_argument('--width', type=float)
     parser.add_argument('--height', type=float)
     args, _ = parser.parse_known_args()
     report = Reporter()
-    for step in range(args.steps):
+    for step in range(args.epochs):
         time.sleep(0.1)
         dummy_score = 1.0 / (0.1 + args.width * step / 100) + args.height * 0.1
         # Feed the score back to Syne Tune.
         report(epoch=step + 1, mean_loss=dummy_score)
 ```
 
 Once you have a script reporting metric, you can launch a tuning as-follow:
@@ -89,15 +89,15 @@
 config_space = {
     'width': randint(1, 20),
     'height': randint(1, 20),
     'epochs': 100,
 }
 
 tuner = Tuner(
-    trial_backend=LocalBackend(entry_point='train_height.py'),
+    trial_backend=LocalBackend(entry_point='train_height_simple.py'),
     scheduler=ASHA(
         config_space,
         metric='mean_loss',
         resource_attr='epoch',
         max_resource_attr="epochs",
         search_options={'debug_log': False},
     ),
@@ -145,14 +145,15 @@
 
 ## Supported multi-objective optimization methods
 
 Method | Reference | Searcher | Asynchronous? | Multi-fidelity? | Transfer?
 :--- | :---: | :---: | :---: | :---: | :---: 
 Constrained Bayesian Optimization | Gardner, et al. (2014) | model-based | yes | no | no
 MOASHA | Schmucker, et al. (2021) | random | yes | yes | no
+NSGA-2 | Deb, et al. (2002) | evolutionary | no | no | no
 
 HPO methods listed can be used in a multi-objective setting by scalarization or non-dominated sorting. See [multiobjective_priority.py](syne_tune/optimizers/schedulers/multiobjective/multiobjective_priority.py) for details.
 
 ## Examples
 
 You will find many examples in the [examples/](examples/) folder illustrating
 different functionalities provided by Syne Tune. For example:
```

### Comparing `syne_tune-0.6.0/setup.py` & `syne_tune-0.7.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,26 +35,28 @@
 required_yahpo = load_requirements(
     "syne_tune/blackbox_repository/conversion_scripts/scripts/requirements-yahpo.txt"
 )
 required_benchmarks = load_benchmark_requirements()
 required_dev = load_requirements("requirements-dev.txt")
 required_aws = load_requirements("requirements-aws.txt")
 required_moo = load_requirements("requirements-moo.txt")
+required_visual = load_requirements("requirements-visual.txt")
 
 long_description = (Path(__file__).parent / "README.md").read_text()
 required_extra = (
-    required_ray
-    + required_gpsearchers
-    + required_benchmarks
-    + required_blackbox_repository
+    required_gpsearchers
     + required_kde
     + required_dev
     + required_aws
-    + required_yahpo
     + required_moo
+    + required_visual
+    + required_blackbox_repository
+    + required_benchmarks
+    + required_yahpo
+    + required_ray
 )
 
 # Botorch only supports python version >= 3.8
 if sys.version_info >= (3, 8):
     required_extra += required_botorch
 
 setup(
@@ -67,24 +69,26 @@
     packages=find_packages(
         include=[
             "syne_tune",
             "syne_tune.*",
         ]
     ),
     extras_require={
-        "raytune": required_ray,
-        "bore": required_bore,
-        "kde": required_kde,
         "gpsearchers": required_gpsearchers,
-        "benchmarks": required_benchmarks,
-        "blackbox-repository": required_blackbox_repository,
-        "aws": required_aws,
-        "yahpo": required_yahpo,
+        "kde": required_kde,
         "dev": required_dev,
+        "aws": required_aws,
         "moo": required_moo,
+        "visual": required_visual,
+        "blackbox-repository": required_blackbox_repository,
+        "benchmarks": required_benchmarks,
+        "yahpo": required_yahpo,
+        "raytune": required_ray,
+        "botorch": required_botorch,
+        "bore": required_bore,
         "extra": required_extra,
     },
     install_requires=required_core,
     include_package_data=True,
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
```

### Comparing `syne_tune-0.6.0/syne_tune/__init__.py` & `syne_tune-0.7.0/syne_tune/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/backend/__init__.py` & `syne_tune-0.7.0/syne_tune/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/backend/local_backend.py` & `syne_tune-0.7.0/syne_tune/backend/local_backend.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/backend/python_backend/__init__.py` & `syne_tune-0.7.0/syne_tune/backend/python_backend/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/backend/python_backend/python_backend.py` & `syne_tune-0.7.0/syne_tune/backend/python_backend/python_backend.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/backend/python_backend/python_entrypoint.py` & `syne_tune-0.7.0/syne_tune/backend/python_backend/python_entrypoint.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/backend/sagemaker_backend/__init__.py` & `syne_tune-0.7.0/syne_tune/backend/sagemaker_backend/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/backend/sagemaker_backend/custom_framework.py` & `syne_tune-0.7.0/syne_tune/backend/sagemaker_backend/custom_framework.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/backend/sagemaker_backend/instance-types-cost.csv` & `syne_tune-0.7.0/syne_tune/backend/sagemaker_backend/instance-types-cost.csv`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/backend/sagemaker_backend/instance_info.py` & `syne_tune-0.7.0/syne_tune/backend/sagemaker_backend/instance_info.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/backend/sagemaker_backend/sagemaker_backend.py` & `syne_tune-0.7.0/syne_tune/backend/sagemaker_backend/sagemaker_backend.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/backend/sagemaker_backend/sagemaker_utils.py` & `syne_tune-0.7.0/syne_tune/backend/sagemaker_backend/sagemaker_utils.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/backend/simulator_backend/__init__.py` & `syne_tune-0.7.0/syne_tune/backend/simulator_backend/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/backend/simulator_backend/events.py` & `syne_tune-0.7.0/syne_tune/backend/simulator_backend/events.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/backend/simulator_backend/simulator_backend.py` & `syne_tune-0.7.0/syne_tune/backend/simulator_backend/simulator_backend.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/backend/simulator_backend/simulator_callback.py` & `syne_tune-0.7.0/syne_tune/backend/simulator_backend/simulator_callback.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/backend/simulator_backend/time_keeper.py` & `syne_tune-0.7.0/syne_tune/backend/simulator_backend/time_keeper.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/backend/time_keeper.py` & `syne_tune-0.7.0/syne_tune/backend/time_keeper.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/backend/trial_backend.py` & `syne_tune-0.7.0/syne_tune/backend/trial_backend.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/backend/trial_status.py` & `syne_tune-0.7.0/syne_tune/backend/trial_status.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/blackbox_repository/__init__.py` & `syne_tune-0.7.0/syne_tune/blackbox_repository/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/blackbox_repository/blackbox.py` & `syne_tune-0.7.0/syne_tune/blackbox_repository/blackbox.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/blackbox_repository/blackbox_offline.py` & `syne_tune-0.7.0/syne_tune/blackbox_repository/blackbox_offline.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/blackbox_repository/blackbox_surrogate.py` & `syne_tune-0.7.0/syne_tune/blackbox_repository/blackbox_surrogate.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/blackbox_repository/blackbox_tabular.py` & `syne_tune-0.7.0/syne_tune/blackbox_repository/blackbox_tabular.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/blackbox_repository/conversion_scripts/__init__.py` & `syne_tune-0.7.0/syne_tune/blackbox_repository/conversion_scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/blackbox_repository/conversion_scripts/blackbox_recipe.py` & `syne_tune-0.7.0/syne_tune/blackbox_repository/conversion_scripts/blackbox_recipe.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/blackbox_repository/conversion_scripts/recipes.py` & `syne_tune-0.7.0/syne_tune/blackbox_repository/conversion_scripts/recipes.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/blackbox_repository/conversion_scripts/scripts/__init__.py` & `syne_tune-0.7.0/syne_tune/blackbox_repository/conversion_scripts/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/blackbox_repository/conversion_scripts/scripts/fcnet_import.py` & `syne_tune-0.7.0/syne_tune/blackbox_repository/conversion_scripts/scripts/fcnet_import.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/blackbox_repository/conversion_scripts/scripts/icml2020_import.py` & `syne_tune-0.7.0/syne_tune/blackbox_repository/conversion_scripts/scripts/icml2020_import.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/blackbox_repository/conversion_scripts/scripts/lcbench/__init__.py` & `syne_tune-0.7.0/syne_tune/blackbox_repository/conversion_scripts/scripts/lcbench/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/blackbox_repository/conversion_scripts/scripts/lcbench/api.py` & `syne_tune-0.7.0/syne_tune/blackbox_repository/conversion_scripts/scripts/lcbench/api.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/blackbox_repository/conversion_scripts/scripts/lcbench/lcbench.py` & `syne_tune-0.7.0/syne_tune/blackbox_repository/conversion_scripts/scripts/lcbench/lcbench.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/blackbox_repository/conversion_scripts/scripts/nasbench201_import.py` & `syne_tune-0.7.0/syne_tune/blackbox_repository/conversion_scripts/scripts/nasbench201_import.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/blackbox_repository/conversion_scripts/scripts/pd1_import.py` & `syne_tune-0.7.0/syne_tune/blackbox_repository/conversion_scripts/scripts/pd1_import.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/blackbox_repository/conversion_scripts/scripts/yahpo_import.py` & `syne_tune-0.7.0/syne_tune/blackbox_repository/conversion_scripts/scripts/yahpo_import.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/blackbox_repository/conversion_scripts/utils.py` & `syne_tune-0.7.0/syne_tune/blackbox_repository/conversion_scripts/utils.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/blackbox_repository/repository.py` & `syne_tune-0.7.0/syne_tune/blackbox_repository/repository.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/blackbox_repository/serialize.py` & `syne_tune-0.7.0/syne_tune/blackbox_repository/serialize.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/blackbox_repository/simulated_tabular_backend.py` & `syne_tune-0.7.0/syne_tune/blackbox_repository/simulated_tabular_backend.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/blackbox_repository/utils.py` & `syne_tune-0.7.0/syne_tune/blackbox_repository/utils.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/callbacks/__init__.py` & `syne_tune-0.7.0/syne_tune/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/callbacks/hyperband_remove_checkpoints_callback.py` & `syne_tune-0.7.0/syne_tune/callbacks/hyperband_remove_checkpoints_callback.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/callbacks/hyperband_remove_checkpoints_score.py` & `syne_tune-0.7.0/syne_tune/callbacks/hyperband_remove_checkpoints_score.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/callbacks/remove_checkpoints_callback.py` & `syne_tune-0.7.0/syne_tune/callbacks/remove_checkpoints_callback.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/callbacks/tensorboard_callback.py` & `syne_tune-0.7.0/syne_tune/callbacks/tensorboard_callback.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/config_space.py` & `syne_tune-0.7.0/syne_tune/config_space.py`

 * *Files 0% similar despite different names*

```diff
@@ -1080,16 +1080,16 @@
     """
     Counts the number of distinct configurations in the configuration space
     ``config_space``. If this is infinite (due to real-valued parameters) or
     larger than ``upper_limit``, None is returned.
 
     :param config_space: Configuration space
     :param upper_limit: See above. Defaults to :code:`2**20`
-    :return: Number of distinct configurations; or None if infinite or more than
-        ``upper_limit``
+    :return: Number of distinct configurations; or ``None`` if infinite or
+        more than ``upper_limit``
     """
     assert upper_limit > 1
     size = 1
     for name, domain in config_space.items():
         if isinstance(domain, Domain):
             domain_size = len(domain)
             if domain_size == 0 or domain_size > upper_limit:
```

### Comparing `syne_tune-0.6.0/syne_tune/constants.py` & `syne_tune-0.7.0/syne_tune/constants.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/experiments/__init__.py` & `syne_tune-0.7.0/syne_tune/experiments/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,15 +13,31 @@
 from syne_tune.experiments.experiment_result import (
     ExperimentResult,
     load_experiment,
     get_metadata,
     list_experiments,
     load_experiments_df,
 )
+from syne_tune.experiments.plotting import (
+    ComparativeResults,
+    PlotParameters,
+    SubplotParameters,
+    ShowTrialParameters,
+)
+from syne_tune.experiments.plot_per_trial import (
+    TrialsOfExperimentResults,
+    MultiFidelityParameters,
+)
 
 __all__ = [
     "ExperimentResult",
     "load_experiment",
     "get_metadata",
     "list_experiments",
     "load_experiments_df",
+    "ComparativeResults",
+    "PlotParameters",
+    "SubplotParameters",
+    "ShowTrialParameters",
+    "TrialsOfExperimentResults",
+    "MultiFidelityParameters",
 ]
```

### Comparing `syne_tune-0.6.0/syne_tune/experiments/experiment_result.py` & `syne_tune-0.7.0/syne_tune/experiments/experiment_result.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/experiments/results_utils.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/cost_aware/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,26 +6,27 @@
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # or in the "license" file accompanying this file. This file is distributed
 # on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either
 # express or implied. See the License for the specific language governing
 # permissions and limitations under the License.
-from typing import Optional
+from syne_tune.try_import import try_import_gpsearchers_message
 
-from syne_tune.constants import (
-    ST_METADATA_FILENAME,
-    ST_RESULTS_DATAFRAME_FILENAME,
-)
-from syne_tune.util import experiment_path, s3_experiment_path
+__all__ = []
 
-
-def sync_from_s3_command(experiment_name: str, s3_bucket: Optional[str] = None) -> str:
-    s3_source_path = s3_experiment_path(
-        s3_bucket=s3_bucket, experiment_name=experiment_name
+try:
+    from syne_tune.optimizer.schedulers.searchers.cost_aware.cost_aware_gp_fifo_searcher import (  # noqa: F401
+        CostAwareGPFIFOSearcher,
+    )
+    from syne_tune.optimizer.schedulers.searchers.cost_aware.cost_aware_gp_multifidelity_searcher import (  # noqa: F401
+        CostAwareGPMultiFidelitySearcher,
     )
-    target_path = str(experiment_path() / experiment_name)
-    return (
-        f'aws s3 sync {s3_source_path} {target_path} --exclude "*" '
-        f'--include "*{ST_METADATA_FILENAME}" '
-        f'--include "*{ST_RESULTS_DATAFRAME_FILENAME}"'
+
+    __all__.extend(
+        [
+            "CostAwareGPFIFOSearcher",
+            "CostAwareGPMultiFidelitySearcher",
+        ]
     )
+except ImportError:
+    print(try_import_gpsearchers_message())
```

### Comparing `syne_tune-0.6.0/syne_tune/num_gpu.py` & `syne_tune-0.7.0/syne_tune/num_gpu.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/__init__.py` & `syne_tune-0.7.0/syne_tune/optimizer/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/baselines.py` & `syne_tune-0.7.0/syne_tune/optimizer/baselines.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 from syne_tune.optimizer.schedulers.multiobjective import MOASHA
 from syne_tune.optimizer.schedulers.searchers.regularized_evolution import (
     RegularizedEvolution,
 )
 from syne_tune.optimizer.schedulers.multiobjective.multi_objective_regularized_evolution import (
     MultiObjectiveRegularizedEvolution,
 )
+from syne_tune.optimizer.schedulers.multiobjective.nsga2_searcher import NSGA2Searcher
 from syne_tune.optimizer.schedulers.synchronous import (
     SynchronousGeometricHyperbandScheduler,
     GeometricDifferentialEvolutionHyperbandScheduler,
 )
 from syne_tune.optimizer.schedulers.transfer_learning import (
     TransferLearningTaskEvaluations,
 )
@@ -774,14 +775,53 @@
                 random_seed=random_seed,
             ),
             random_seed=random_seed,
             **kwargs,
         )
 
 
+class NSGA2(FIFOScheduler):
+    """
+
+    See :class:`~syne_tune.optimizer.schedulers.searchers.RandomSearcher`
+    for ``kwargs["search_options"]`` parameters.
+
+    :param config_space: Configuration space for evaluation function
+    :param metric: Name of metric to optimize
+    :param population_size: The size of the population for NSGA-2
+    :param random_seed: Random seed, optional
+    :param kwargs: Additional arguments to
+        :class:`~syne_tune.optimizer.schedulers.FIFOScheduler`
+    """
+
+    def __init__(
+        self,
+        config_space: Dict[str, Any],
+        metric: List[str],
+        mode: Union[List[str], str] = "min",
+        population_size: int = 20,
+        random_seed: Optional[int] = None,
+        **kwargs,
+    ):
+        super(NSGA2, self).__init__(
+            config_space=config_space,
+            metric=metric,
+            mode=mode,
+            searcher=NSGA2Searcher(
+                config_space=config_space,
+                metric=metric,
+                mode=mode,
+                population_size=population_size,
+                random_seed=random_seed,
+            ),
+            random_seed=random_seed,
+            **kwargs,
+        )
+
+
 class ConstrainedBayesianOptimization(FIFOScheduler):
     """Constrained Bayesian Optimization.
 
     See :class:`~syne_tune.optimizer.schedulers.searchers.constrained.ConstrainedGPFIFOSearcher`
     for ``kwargs["search_options"]`` parameters.
 
     :param config_space: Configuration space for evaluation function
```

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/scheduler.py` & `syne_tune-0.7.0/syne_tune/optimizer/scheduler.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/__init__.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/fifo.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/fifo.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/hyperband.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/hyperband.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/hyperband_checkpoint_removal.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/hyperband_checkpoint_removal.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/hyperband_cost_promotion.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/hyperband_cost_promotion.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/hyperband_pasha.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/hyperband_pasha.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/hyperband_promotion.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/hyperband_promotion.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/hyperband_rush.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/hyperband_rush.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/hyperband_stopping.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/hyperband_stopping.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/median_stopping_rule.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/median_stopping_rule.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/multi_fidelity.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/multi_fidelity.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/multiobjective/__init__.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/multiobjective/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/multiobjective/linear_scalarizer.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/multiobjective/linear_scalarizer.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/multiobjective/moasha.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/multiobjective/moasha.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/multiobjective/multi_objective_regularized_evolution.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/multiobjective/multi_objective_regularized_evolution.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/multiobjective/multiobjective_priority.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/multiobjective/multiobjective_priority.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/multiobjective/non_dominated_priority.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/multiobjective/non_dominated_priority.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/multiobjective/utils.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/multiobjective/utils.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/neuralbands/__init__.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/neuralbands/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/neuralbands/networks.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/neuralbands/networks.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/neuralbands/neuralband.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/neuralbands/neuralband.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/neuralbands/neuralband_supplement.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/neuralbands/neuralband_supplement.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/pbt.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/pbt.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/random_seeds.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/random_seeds.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/ray_scheduler.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/ray_scheduler.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/remove_checkpoints.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/remove_checkpoints.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/scheduler_searcher.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/scheduler_searcher.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/__init__.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/__init__.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/datatypes/__init__.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/datatypes/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/datatypes/common.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/datatypes/common.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/datatypes/config_ext.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/datatypes/config_ext.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/datatypes/tuning_job_state.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/datatypes/tuning_job_state.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/__init__.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/constants.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/constants.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/custom_op.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/custom_op.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/distribution.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/distribution.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gluon.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gluon.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gluon_blocks_helpers.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gluon_blocks_helpers.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gp_model.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gp_model.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gp_regression.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gp_regression.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gpr_mcmc.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gpr_mcmc.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/__init__.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/gp_model.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/gp_model.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/likelihood.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/likelihood.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/posterior_state.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/posterior_state.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/utils.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/utils.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/independent/__init__.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/independent/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/independent/gpind_model.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/independent/gpind_model.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/independent/likelihood.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/independent/likelihood.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/independent/posterior_state.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/independent/posterior_state.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/__init__.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/base.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/base.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/cross_validation.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/cross_validation.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/exponential_decay.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/exponential_decay.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/fabolas.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/fabolas.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/freeze_thaw.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/freeze_thaw.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/product_kernel.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/product_kernel.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/range_kernel.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/range_kernel.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/__init__.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/freeze_thaw.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/freeze_thaw.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/gpiss_model.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/gpiss_model.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/issm.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/issm.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/likelihood.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/likelihood.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/model_params.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/model_params.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/posterior_state.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/posterior_state.py`

 * *Files 1% similar despite different names*

```diff
@@ -180,20 +180,20 @@
         self,
         input: np.ndarray,
         head_gradients: Dict[str, np.ndarray],
         mean_data: float,
         std_data: float,
     ) -> np.ndarray:
         """
-        Implements SurrogateModel.backward_gradient, see comments there.
-        This is for a single posterior state. If the SurrogateModel uses
+        Implements Predictor.backward_gradient, see comments there.
+        This is for a single posterior state. If the Predictor uses
         MCMC, have to call this for every sample.
 
         :param input: Single input point x, shape (d,)
-        :param head_gradients: See SurrogateModel.backward_gradient
+        :param head_gradients: See Predictor.backward_gradient
         :param mean_data: Mean used to normalize targets
         :param std_data: Stddev used to normalize targets
         :return:
         """
         test_feature = np.reshape(input, (1, -1))
 
         def diff_test_feature(test_feature_array):
```

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/likelihood.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/likelihood.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/mean.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/mean.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/optimization_utils.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/optimization_utils.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/posterior_state.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/posterior_state.py`

 * *Files 4% similar despite different names*

```diff
@@ -88,20 +88,20 @@
         self,
         input: np.ndarray,
         head_gradients: Dict[str, np.ndarray],
         mean_data: float,
         std_data: float,
     ) -> np.ndarray:
         """
-        Implements SurrogateModel.backward_gradient, see comments there.
-        This is for a single posterior state. If the SurrogateModel uses
+        Implements Predictor.backward_gradient, see comments there.
+        This is for a single posterior state. If the Predictor uses
         MCMC, have to call this for every sample.
 
         :param input: Single input point x, shape (d,)
-        :param head_gradients: See SurrogateModel.backward_gradient
+        :param head_gradients: See Predictor.backward_gradient
         :param mean_data: Mean used to normalize targets
         :param std_data: Stddev used to normalize targets
         :return:
         """
         raise NotImplementedError
 
 
@@ -240,24 +240,24 @@
         self,
         input: np.ndarray,
         head_gradients: Dict[str, np.ndarray],
         mean_data: float,
         std_data: float,
     ) -> np.ndarray:
         """
-        Implements SurrogateModel.backward_gradient, see comments there.
-        This is for a single posterior state. If the SurrogateModel uses
+        Implements Predictor.backward_gradient, see comments there.
+        This is for a single posterior state. If the Predictor uses
         MCMC, have to call this for every sample.
 
         The posterior represented here is based on normalized data, while
         the acquisition function is based on the de-normalized predictive
         distribution, which is why we need 'mean_data', 'std_data' here.
 
         :param input: Single input point x, shape (d,)
-        :param head_gradients: See SurrogateModel.backward_gradient
+        :param head_gradients: See Predictor.backward_gradient
         :param mean_data: Mean used to normalize targets
         :param std_data: Stddev used to normalize targets
         :return:
         """
 
         def predict_func(test_feature_array):
             return self.predict(test_feature_array)
@@ -290,25 +290,25 @@
     predict_func: Callable[[np.ndarray], Tuple[np.ndarray, np.ndarray]],
     input: np.ndarray,
     head_gradients: Dict[str, np.ndarray],
     mean_data: float,
     std_data: float,
 ) -> np.ndarray:
     """
-    Implements SurrogateModel.backward_gradient, see comments there.
-    This is for a single posterior state. If the SurrogateModel uses
+    Implements Predictor.backward_gradient, see comments there.
+    This is for a single posterior state. If the Predictor uses
     MCMC, have to call this for every sample.
 
     The posterior represented here is based on normalized data, while
     the acquisition function is based on the de-normalized predictive
     distribution, which is why we need 'mean_data', 'std_data' here.
 
     :param predict_func: Function mapping input x to mean, variance
     :param input: Single input point x, shape (d,)
-    :param head_gradients: See SurrogateModel.backward_gradient
+    :param head_gradients: See Predictor.backward_gradient
     :param mean_data: Mean used to normalize targets
     :param std_data: Stddev used to normalize targets
     :return:
     """
     test_feature = np.reshape(input, (1, -1))
     assert "mean" in head_gradients, "Need head_gradients['mean'] for backward_gradient"
     has_std = "std" in head_gradients
```

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/posterior_utils.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/posterior_utils.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/slice.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/slice.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/target_transform.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/target_transform.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/warping.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/warping.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/__init__.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/__init__.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/cost_model.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/cost_model.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/linear_cost_model.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/linear_cost_model.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/sklearn_cost_model.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/sklearn_cost_model.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost_fifo_model.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost_fifo_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,34 +10,32 @@
 # on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either
 # express or implied. See the License for the specific language governing
 # permissions and limitations under the License.
 from typing import Dict, List, Set
 import numpy as np
 import logging
 
-from syne_tune.optimizer.schedulers.searchers.bayesopt.models.model_transformer import (
-    TransformerModelFactory,
-)
+from syne_tune.optimizer.schedulers.searchers.bayesopt.models.estimator import Estimator
 from syne_tune.optimizer.schedulers.searchers.bayesopt.models.model_base import (
-    BaseSurrogateModel,
+    BasePredictor,
 )
 from syne_tune.optimizer.schedulers.searchers.bayesopt.models.cost.cost_model import (
     CostModel,
 )
 from syne_tune.optimizer.schedulers.searchers.bayesopt.datatypes.tuning_job_state import (
     TuningJobState,
 )
 from syne_tune.optimizer.schedulers.searchers.bayesopt.tuning_algorithms.base_classes import (
-    SurrogateModel,
+    Predictor,
 )
 
 logger = logging.getLogger(__name__)
 
 
-class CostFixedResourceSurrogateModel(BaseSurrogateModel):
+class CostFixedResourcePredictor(BasePredictor):
     """
     Wraps cost model :math:`c(x, r)` of :class:`CostModel` to be used as
     surrogate model, where predictions are done at r = ``fixed_resource``.
 
     Note: For random cost models, we approximate expectations in ``predict``
     by resampling ``num_samples`` times (should be 1 for deterministic cost
     models).
@@ -111,15 +109,15 @@
 
     # We currently do not support cost models for the primary metric to be
     # optimized
     def current_best(self) -> List[np.ndarray]:
         raise NotImplementedError()
 
 
-class CostSurrogateModelFactory(TransformerModelFactory):
+class CostEstimator(Estimator):
     """
     The name of the cost metric is ``model.cost_metric_name``.
 
     :param model: CostModel to be wrapped
     :param fixed_resource: :math:`c(x, r)` is predicted for this resource level r
     :param num_samples: Number of samples drawn in :meth:`predict`. Use this for
         random cost models only
@@ -141,20 +139,20 @@
     def fixed_resource(self) -> int:
         return self._fixed_resource
 
     def set_fixed_resource(self, resource: int):
         assert resource >= 1, "Must be positive integer"
         self._fixed_resource = resource
 
-    def model(self, state: TuningJobState, fit_params: bool) -> SurrogateModel:
+    def fit_from_state(self, state: TuningJobState, update_params: bool) -> Predictor:
         """
         Models of type :class:`CostModel` do not have hyperparameters to be
-        fit, so ``fit_params`` is ignored here (TODO?).
+        fit, so ``update_params`` is ignored here.
 
         """
         self._model.update(state)
-        return CostFixedResourceSurrogateModel(
+        return CostFixedResourcePredictor(
             state=state,
             model=self._model,
             fixed_resource=self._fixed_resource,
             num_samples=self._num_samples,
         )
```

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/gp_mcmc_model.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/gp_mcmc_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,28 +16,28 @@
 from syne_tune.optimizer.schedulers.searchers.bayesopt.gpautograd.gpr_mcmc import (
     GPRegressionMCMC,
 )
 from syne_tune.optimizer.schedulers.searchers.utils.hp_ranges import (
     HyperparameterRanges,
 )
 from syne_tune.optimizer.schedulers.searchers.bayesopt.models.gp_model import (
-    GaussProcModelFactory,
+    GaussProcEstimator,
 )
 from syne_tune.optimizer.schedulers.searchers.bayesopt.utils.debug_log import (
     DebugLogPrinter,
 )
 from syne_tune.optimizer.schedulers.searchers.bayesopt.datatypes.common import (
     INTERNAL_METRIC_NAME,
 )
 from syne_tune.optimizer.schedulers.searchers.utils.common import ConfigurationFilter
 
 logger = logging.getLogger(__name__)
 
 
-class GaussProcMCMCModelFactory(GaussProcModelFactory):
+class GaussProcMCMCEstimator(GaussProcEstimator):
     """
     We support pending evaluations via fantasizing. Note that state does
     not contain the fantasy values, but just the pending configs. Fantasy
     values are sampled here.
 
     We draw one fantasy sample per MCMC sample here. This could be extended
     by sampling ``> 1`` fantasy samples for each MCMC sample.
```

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/gp_model.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/gp_model.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,21 +9,21 @@
 # or in the "license" file accompanying this file. This file is distributed
 # on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either
 # express or implied. See the License for the specific language governing
 # permissions and limitations under the License.
 from typing import Dict, List, Optional, Union
 import numpy as np
 import logging
-from dataclasses import dataclass
 
-from syne_tune.optimizer.schedulers.searchers.bayesopt.models.model_transformer import (
-    TransformerModelFactory,
+from syne_tune.optimizer.schedulers.searchers.bayesopt.models.estimator import (
+    Estimator,
+    transform_state_to_data,
 )
 from syne_tune.optimizer.schedulers.searchers.bayesopt.models.model_base import (
-    BaseSurrogateModel,
+    BasePredictor,
 )
 from syne_tune.optimizer.schedulers.searchers.bayesopt.datatypes.common import (
     FantasizedPendingEvaluation,
     INTERNAL_METRIC_NAME,
 )
 from syne_tune.optimizer.schedulers.searchers.utils.common import ConfigurationFilter
 from syne_tune.optimizer.schedulers.searchers.bayesopt.datatypes.tuning_job_state import (
@@ -45,15 +45,15 @@
     HyperTuneIndependentGPModel,
     HyperTuneJointGPModel,
 )
 from syne_tune.optimizer.schedulers.searchers.bayesopt.gpautograd.posterior_state import (
     PosteriorState,
 )
 from syne_tune.optimizer.schedulers.searchers.bayesopt.tuning_algorithms.base_classes import (
-    SurrogateModel,
+    Predictor,
 )
 from syne_tune.optimizer.schedulers.searchers.bayesopt.utils.debug_log import (
     DebugLogPrinter,
 )
 
 logger = logging.getLogger(__name__)
 
@@ -63,15 +63,15 @@
     GPRegressionMCMC,
     IndependentGPPerResourceModel,
     HyperTuneIndependentGPModel,
     HyperTuneJointGPModel,
 ]
 
 
-class GaussProcSurrogateModel(BaseSurrogateModel):
+class GaussProcPredictor(BasePredictor):
     """
     Gaussian process surrogate model, where model parameters are either fit by
     marginal likelihood maximization
     (e.g., :class:`~syne_tune.optimizer.schedulers.searchers.bayesopt.gpautograd.gp_regression.GaussianProcessRegression`),
     or integrated out by MCMC sampling
     (e.g., :class:`~syne_tune.optimizer.schedulers.searchers.bayesopt.gpautograd.gpr_mcmc.GPRegressionMCMC`).
 
@@ -143,15 +143,20 @@
         ), "Cannot run backward_gradient without a posterior state"
         assert len(poster_states) == len(
             head_gradients
         ), "len(posterior_states) = {} != {} = len(head_gradients)".format(
             len(poster_states), len(head_gradients)
         )
         return [
-            poster_state.backward_gradient(input, head_gradient, self.mean, self.std)
+            poster_state.backward_gradient(
+                input=input,
+                head_gradients=head_gradient,
+                mean_data=self.mean,
+                std_data=self.std,
+            )
             for poster_state, head_gradient in zip(poster_states, head_gradients)
         ]
 
     def does_mcmc(self):
         return isinstance(self._gpmodel, GPRegressionMCMC)
 
     @property
@@ -167,85 +172,29 @@
         )
         if hp_ranges.is_attribute_fixed():
             error_msg += f" with resource attribute '{hp_ranges.name_last_pos}' == {hp_ranges.value_for_last_pos}"
         assert candidates, error_msg
         return candidates
 
 
-@dataclass
-class InternalCandidateEvaluations:
-    features: np.ndarray
-    targets: np.ndarray
-    mean: float
-    std: float
-
-
-# Note: If state.pending_evaluations is not empty, it must contain entries
-# of type FantasizedPendingEvaluation, which contain the fantasy samples. This
-# is the case only for internal states.
-def get_internal_candidate_evaluations(
-    state: TuningJobState,
-    active_metric: str,
-    normalize_targets: bool,
-    num_fantasy_samples: int,
-) -> InternalCandidateEvaluations:
-    candidates, evaluation_values = state.observed_data_for_metric(
-        metric_name=active_metric
-    )
-    hp_ranges = state.hp_ranges
-    features = hp_ranges.to_ndarray_matrix(candidates)
-    # Normalize
-    # Note: The fantasy values in state.pending_evaluations are sampled
-    # from the model fit to normalized targets, so they are already
-    # normalized
-    targets = np.vstack(evaluation_values).reshape((-1, 1))
-    mean = 0.0
-    std = 1.0
-    if normalize_targets:
-        std = max(np.std(targets).item(), 1e-9)
-        mean = np.mean(targets).item()
-        targets = (targets - mean) / std
-    if state.pending_evaluations:
-        # In this case, y becomes a matrix, where the observed values are
-        # broadcast
-        cand_lst = [
-            hp_ranges.to_ndarray(config) for config in state.pending_configurations()
-        ]
-        fanta_lst = []
-        for pending_eval in state.pending_evaluations:
-            assert isinstance(
-                pending_eval, FantasizedPendingEvaluation
-            ), "state.pending_evaluations has to contain FantasizedPendingEvaluation"
-            fantasies = pending_eval.fantasies[active_metric]
-            assert (
-                fantasies.size == num_fantasy_samples
-            ), "All state.pending_evaluations entries must have length {}".format(
-                num_fantasy_samples
-            )
-            fanta_lst.append(fantasies.reshape((1, -1)))
-        targets = np.vstack([targets * np.ones((1, num_fantasy_samples))] + fanta_lst)
-        features = np.vstack([features] + cand_lst)
-    return InternalCandidateEvaluations(features, targets, mean, std)
-
-
-class GaussProcModelFactory(TransformerModelFactory):
+class GaussProcEstimator(Estimator):
     """
     We support pending evaluations via fantasizing. Note that state does
     not contain the fantasy values, but just the pending configs. Fantasy
     values are sampled here.
 
     :param gpmodel: Internal model
     :param active_metric: Name of the metric to optimize.
     :param normalize_targets: Normalize observed target values?
     :param debug_log: DebugLogPrinter (optional)
     :param filter_observed_data: Filter for observed data before
         computing incumbent
     :param no_fantasizing: If True, pending evaluations in the state are
         simply ignored, fantasizing is not done (not recommended)
-    :param hp_ranges_for_prediction: If given, :class:`GaussProcSurrogateModel`
+    :param hp_ranges_for_prediction: If given, :class:`GaussProcPredictor`
         should use this instead of ``state.hp_ranges``
     """
 
     def __init__(
         self,
         gpmodel: GPModel,
         active_metric: str,
@@ -269,20 +218,20 @@
     def debug_log(self) -> Optional[DebugLogPrinter]:
         return self._debug_log
 
     @property
     def gpmodel(self) -> GPModel:
         return self._gpmodel
 
-    def model(self, state: TuningJobState, fit_params: bool) -> SurrogateModel:
+    def fit_from_state(self, state: TuningJobState, update_params: bool) -> Predictor:
         """
-        Parameters of ``self._gpmodel`` are optimized iff ``fit_params``. This
+        Parameters of ``self._gpmodel`` are optimized iff ``update_params``. This
         requires ``state`` to contain labeled examples.
 
-        If self.state.pending_evaluations is not empty, we proceed as follows:
+        If ``self.state.pending_evaluations`` is not empty, we proceed as follows:
 
         * Compute posterior for state without pending evals
         * Draw fantasy values for pending evals
         * Recompute posterior (without fitting)
 
         """
         if self._debug_log is not None:
@@ -292,24 +241,24 @@
         if state.pending_evaluations:
             no_pending_state = TuningJobState(
                 hp_ranges=state.hp_ranges,
                 config_for_trial=state.config_for_trial,
                 trials_evaluations=state.trials_evaluations,
                 failed_trials=state.failed_trials,
             )
-        self._posterior_for_state(no_pending_state, fit_params=fit_params)
+        self._posterior_for_state(no_pending_state, update_params=update_params)
         if state.pending_evaluations and not self._no_fantasizing:
             # Sample fantasy values for pending evaluations
             state_with_fantasies = self._draw_fantasy_values(state)
             # Compute posterior for state with pending evals
-            self._posterior_for_state(state_with_fantasies, fit_params=False)
+            self._posterior_for_state(state_with_fantasies, update_params=False)
             fantasy_samples = state_with_fantasies.pending_evaluations
         else:
             fantasy_samples = []
-        return GaussProcSurrogateModel(
+        return GaussProcPredictor(
             state=state,
             active_metric=self.active_metric,
             gpmodel=self._gpmodel,
             fantasy_samples=fantasy_samples,
             normalize_mean=self._mean,
             normalize_std=self._std,
             filter_observed_data=self._filter_observed_data,
@@ -318,43 +267,43 @@
 
     def _get_num_fantasy_samples(self) -> int:
         raise NotImplementedError()
 
     def _posterior_for_state(
         self,
         state: TuningJobState,
-        fit_params: bool,
+        update_params: bool,
     ):
         """
         Computes posterior for state.
         If ``fit_params`` and ``state.pending_evaluations`` is empty, we first
         optimize the model parameters.
         If ``state.pending_evaluations`` are given, these must be of type
         :class:`~syne_tune.optimizer.schedulers.searchers.bayesopt.datatypes.common.FantasizedPendingEvaluations`,
         i.e. the fantasy values must have been sampled.
         """
         assert state.num_observed_cases(self.active_metric) > 0, (
             "Cannot compute posterior: state has no labeled datapoints "
             + f"for metric {self.active_metric}"
         )
-        internal_candidate_evaluations = get_internal_candidate_evaluations(
+        internal_candidate_evaluations = transform_state_to_data(
             state,
             self.active_metric,
             self.normalize_targets,
             self._get_num_fantasy_samples(),
         )
         features = internal_candidate_evaluations.features
         targets = internal_candidate_evaluations.targets
         assert features.shape[0] == targets.shape[0]
         self._mean = internal_candidate_evaluations.mean
         self._std = internal_candidate_evaluations.std
 
-        fit_params = fit_params and (not state.pending_evaluations)
+        update_params = update_params and (not state.pending_evaluations)
         data = {"features": features, "targets": targets}
-        if not fit_params:
+        if not update_params:
             if self._debug_log is not None:
                 logger.info("Recomputing posterior state")
             self._gpmodel.recompute_states(data)
         else:
             if self._debug_log is not None:
                 logger.info(f"Fitting surrogate model for {self.active_metric}")
             self._gpmodel.fit(data)
@@ -438,15 +387,15 @@
             if scheduler.rung_levels[-1] == max_resource_level:
                 rung_levels = scheduler.rung_levels
             else:
                 rung_levels = scheduler.rung_levels + [max_resource_level]
             self._gpmodel.create_likelihood(rung_levels)
 
 
-class GaussProcEmpiricalBayesModelFactory(GaussProcModelFactory):
+class GaussProcEmpiricalBayesEstimator(GaussProcEstimator):
     """
     We support pending evaluations via fantasizing. Note that state does
     not contain the fantasy values, but just the pending configs. Fantasy
     values are sampled here.
 
     :param gpmodel: :class:`GaussianProcessRegression` model
     :param num_fantasy_samples: See above
```

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/gpiss_model.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/gpiss_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,19 +10,17 @@
 # on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either
 # express or implied. See the License for the specific language governing
 # permissions and limitations under the License.
 from typing import Dict, List, Optional
 import numpy as np
 import logging
 
-from syne_tune.optimizer.schedulers.searchers.bayesopt.models.model_transformer import (
-    TransformerModelFactory,
-)
+from syne_tune.optimizer.schedulers.searchers.bayesopt.models.estimator import Estimator
 from syne_tune.optimizer.schedulers.searchers.bayesopt.models.model_base import (
-    BaseSurrogateModel,
+    BasePredictor,
 )
 from syne_tune.optimizer.schedulers.searchers.bayesopt.datatypes.config_ext import (
     ExtendedConfiguration,
 )
 from syne_tune.optimizer.schedulers.searchers.bayesopt.datatypes.tuning_job_state import (
     TuningJobState,
 )
@@ -33,28 +31,28 @@
     prepare_data,
     prepare_data_with_pending,
 )
 from syne_tune.optimizer.schedulers.searchers.bayesopt.gpautograd.learncurve.posterior_state import (
     GaussProcAdditivePosteriorState,
 )
 from syne_tune.optimizer.schedulers.searchers.bayesopt.tuning_algorithms.base_classes import (
-    SurrogateModel,
+    Predictor,
 )
 from syne_tune.optimizer.schedulers.searchers.bayesopt.datatypes.common import (
     FantasizedPendingEvaluation,
 )
 from syne_tune.optimizer.schedulers.searchers.utils.common import ConfigurationFilter
 from syne_tune.optimizer.schedulers.searchers.bayesopt.utils.debug_log import (
     DebugLogPrinter,
 )
 
 logger = logging.getLogger(__name__)
 
 
-class GaussProcAdditiveSurrogateModel(BaseSurrogateModel):
+class GaussProcAdditivePredictor(BasePredictor):
     """
     Gaussian Process additive surrogate model, where model parameters are
     fit by marginal likelihood maximization.
 
     Note: :meth:`predict_mean_current_candidates` calls :meth:`predict` for all
     observed and pending extended configs. This may not be exactly
     correct, because :meth:`predict` is not meant to be used for configs
@@ -121,27 +119,32 @@
         ), "Cannot run backward_gradient without a posterior state"
         assert len(poster_states) == len(
             head_gradients
         ), "len(posterior_states) = {} != {} = len(head_gradients)".format(
             len(poster_states), len(head_gradients)
         )
         return [
-            poster_state.backward_gradient(input, head_gradient, self.mean, self.std)
+            poster_state.backward_gradient(
+                input=input,
+                head_gradients=head_gradient,
+                mean_data=self.mean,
+                std_data=self.std,
+            )
             for poster_state, head_gradient in zip(poster_states, head_gradients)
         ]
 
     def does_mcmc(self):
         return False
 
     @property
     def posterior_states(self) -> Optional[List[GaussProcAdditivePosteriorState]]:
         return self._gpmodel.states
 
 
-class GaussProcAdditiveModelFactory(TransformerModelFactory):
+class GaussProcAdditiveEstimator(Estimator):
     """
     If ``num_fantasy_samples > 0``, we draw this many fantasy targets
     independently, while each sample is dependent over all pending
     evaluations. If ``num_fantasy_samples == 0``, pending evaluations
     in ``state`` are ignored.
 
     :param gpmodel: GaussianProcessLearningCurveModel
@@ -185,32 +188,32 @@
 
     def get_params(self):
         return self._gpmodel.get_params()
 
     def set_params(self, param_dict):
         self._gpmodel.set_params(param_dict)
 
-    def model(self, state: TuningJobState, fit_params: bool) -> SurrogateModel:
+    def fit_from_state(self, state: TuningJobState, update_params: bool) -> Predictor:
         assert state.num_observed_cases(self.active_metric) > 0, (
             "Cannot compute posterior: state has no labeled datapoints "
             + f"for metric {self.active_metric}"
         )
         if self._debug_log is not None:
             self._debug_log.set_state(state)
         do_fantasizing = state.pending_evaluations and self.num_fantasy_samples > 0
 
         # [1] Fit model and compute posterior state, ignoring pending evals
         data = prepare_data(
-            state,
-            self._config_space_ext,
-            self.active_metric,
+            state=state,
+            config_space_ext=self._config_space_ext,
+            active_metric=self.active_metric,
             normalize_targets=self.normalize_targets,
             do_fantasizing=False,
         )
-        if fit_params:
+        if update_params:
             logger.info(f"Fitting surrogate model for {self.active_metric}")
             self._gpmodel.fit(data)
         elif not do_fantasizing:
             # Only if part below is skipped
             logger.info("Recomputing posterior state")
             self._gpmodel.recompute_states(data)
         if self._debug_log is not None:
@@ -238,26 +241,26 @@
                 normalize_targets=self.normalize_targets,
                 do_fantasizing=True,
             )
             self._gpmodel.recompute_states(data)
         else:
             fantasy_samples = []
 
-        return GaussProcAdditiveSurrogateModel(
+        return GaussProcAdditivePredictor(
             state=state,
             gpmodel=self._gpmodel,
             fantasy_samples=fantasy_samples,
             active_metric=self.active_metric,
             filter_observed_data=self._filter_observed_data,
             **extra_kwargs,
         )
 
-    def model_for_fantasy_samples(
+    def predictor_for_fantasy_samples(
         self, state: TuningJobState, fantasy_samples: List[FantasizedPendingEvaluation]
-    ) -> SurrogateModel:
+    ) -> Predictor:
         """
         Same as ``model`` with ``fit_params=False``, but ``fantasy_samples`` are
         passed in, rather than sampled here.
 
         :param state: See ``model``
         :param fantasy_samples: See above
         :return: See ``model``
@@ -290,15 +293,15 @@
             extra_kwargs = {
                 "normalize_mean": data["mean_targets"],
                 "normalize_std": data["std_targets"],
             }
         else:
             extra_kwargs = dict()
 
-        return GaussProcAdditiveSurrogateModel(
+        return GaussProcAdditivePredictor(
             state=state,
             gpmodel=self._gpmodel,
             fantasy_samples=fantasy_samples,
             active_metric=self.active_metric,
             filter_observed_data=self._filter_observed_data,
             **extra_kwargs,
         )
@@ -306,15 +309,15 @@
     def configure_scheduler(self, scheduler):
         from syne_tune.optimizer.schedulers.multi_fidelity import (
             MultiFidelitySchedulerMixin,
         )
 
         assert isinstance(
             scheduler, MultiFidelitySchedulerMixin
-        ), "GaussProcAdditiveModelFactory requires MultiFidelitySchedulerMixin scheduler"
+        ), "GaussProcAdditiveEstimator requires MultiFidelitySchedulerMixin scheduler"
         assert scheduler.searcher_data == "all", (
             "For an additive Gaussian learning curve model (model='gp_issm' or "
             "model='gp_expdecay' in search_options), you need to set "
             "searcher_data='all' when creating the multi-fidelity scheduler"
         )
 
     def _draw_fantasy_values(self, state: TuningJobState) -> TuningJobState:
```

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/kernel_factory.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/kernel_factory.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/meanstd_acqfunc_impl.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/meanstd_acqfunc_impl.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,50 +21,50 @@
 from syne_tune.optimizer.schedulers.searchers.bayesopt.models.meanstd_acqfunc import (
     MeanStdAcquisitionFunction,
     HeadWithGradient,
     SamplePredictionsPerOutput,
     CurrentBestProvider,
 )
 from syne_tune.optimizer.schedulers.searchers.bayesopt.models.model_base import (
-    BaseSurrogateModel,
+    BasePredictor,
 )
 from syne_tune.optimizer.schedulers.searchers.bayesopt.tuning_algorithms.base_classes import (
-    SurrogateOutputModel,
-    SurrogateModel,
+    OutputPredictor,
+    Predictor,
 )
 
 logger = logging.getLogger(__name__)
 
 
 MIN_COST = 1e-12  # For numerical stability when dividing EI / cost
 
 MIN_STD_CONSTRAINT = (
     1e-12  # For numerical stability when computing the constraint probability in CEI
 )
 
 
-def _extract_active_and_secondary_metric(model_output_names, active_metric):
+def _extract_active_and_secondary_metric(predictor_output_names, active_metric):
     """
-    Returns the active metric and the secondary metric (such as the cost or constraint metric) from model_output_names.
+    Returns the active metric and the secondary metric (such as the cost or constraint metric) from predictor_output_names.
     """
-    assert len(model_output_names) == 2, (
-        f"The model should consist of exactly 2 outputs, "
-        f"while the current outputs are {model_output_names}"
+    assert len(predictor_output_names) == 2, (
+        f"The predictor should consist of exactly 2 outputs, "
+        f"while the current outputs are {predictor_output_names}"
     )
-    assert active_metric in model_output_names, (
+    assert active_metric in predictor_output_names, (
         f"{active_metric} is not a valid metric. "
         f"The metric name must match one of the following metrics "
-        f"in the model output: {model_output_names}"
+        f"in the predictor output: {predictor_output_names}"
     )
-    if model_output_names[0] == active_metric:
-        secondary_metric = model_output_names[1]
+    if predictor_output_names[0] == active_metric:
+        secondary_metric = predictor_output_names[1]
     else:
-        secondary_metric = model_output_names[0]
+        secondary_metric = predictor_output_names[0]
     logger.debug(
-        f"There are two metrics in the output: {model_output_names}. "
+        f"There are two metrics in the output: {predictor_output_names}. "
         f"The metric to optimize was set to '{active_metric}'. "
         f"The secondary metric is assumed to be '{secondary_metric}'"
     )
     return active_metric, secondary_metric
 
 
 def _postprocess_gradient(grad: np.ndarray, nf: int) -> np.ndarray:
@@ -79,21 +79,21 @@
     """
     Minus expected improvement acquisition function
     (minus because the convention is to always minimize acquisition functions)
     """
 
     def __init__(
         self,
-        model: SurrogateOutputModel,
+        predictor: OutputPredictor,
         active_metric: str = None,
         jitter: float = 0.01,
         debug_collect_stats: bool = False,
     ):
-        assert isinstance(model, SurrogateModel)
-        super().__init__(model, active_metric)
+        assert isinstance(predictor, Predictor)
+        super().__init__(predictor, active_metric)
         self.jitter = jitter
         if debug_collect_stats:
             self._debug_data = {"absdiff": [], "std": [], "u": []}
         else:
             self._debug_data = None
 
     def _head_needs_current_best(self) -> bool:
@@ -165,18 +165,18 @@
 
     .. math::
 
        h(\mu, \sigma) = \mu - \kappa * \sigma
     """
 
     def __init__(
-        self, model: SurrogateOutputModel, kappa: float, active_metric: str = None
+        self, predictor: OutputPredictor, kappa: float, active_metric: str = None
     ):
-        super().__init__(model, active_metric)
-        assert isinstance(model, SurrogateModel)
+        super().__init__(predictor, active_metric)
+        assert isinstance(predictor, Predictor)
         assert kappa > 0, "kappa must be positive"
         self.kappa = kappa
 
     def _head_needs_current_best(self) -> bool:
         return False
 
     def _compute_head(
@@ -225,48 +225,48 @@
         | https://arxiv.org/abs/2003.10870
 
     Note: two metrics are expected in the model output: the main objective and the cost.
     The main objective needs to be indicated as ``active_metric`` when initializing
     :class:`EIpuAcquisitionFunction`.
     The cost is automatically assumed to be the other metric.
 
-    :param model: Surrogate models for main objective and cost
+    :param predictor: Predictors for main objective and cost
     :param active_metric: Name of main objective
     :param exponent_cost: Exponent for cost in denominator. Defaults to 1
     :param jitter: Jitter factor, must be positive. Defaults to 0.01
     """
 
     def __init__(
         self,
-        model: SurrogateOutputModel,
+        predictor: OutputPredictor,
         active_metric: Optional[str] = None,
         exponent_cost: float = 1.0,
         jitter: float = 0.01,
     ):
-        super().__init__(model, active_metric)
+        super().__init__(predictor, active_metric)
         assert (
             0 < exponent_cost <= 1
         ), f"exponent_cost = {exponent_cost} must lie in (0, 1]"
         self.jitter = jitter
         self.exponent_cost = exponent_cost
         self.active_metric, self.cost_metric = _extract_active_and_secondary_metric(
-            self.model_output_names, active_metric
+            self.predictor_output_names, active_metric
         )
 
     def _head_needs_current_best(self) -> bool:
         return True
 
     def _output_to_keys_predict(self) -> Dict[str, Set[str]]:
         """
         The cost model may be deterministic, as the acquisition function
         only needs the mean.
         """
         return {
-            self.model_output_names[0]: {"mean", "std"},
-            self.model_output_names[1]: {"mean"},
+            self.predictor_output_names[0]: {"mean", "std"},
+            self.predictor_output_names[1]: {"mean"},
         }
 
     def _compute_head(
         self,
         output_to_predictions: SamplePredictionsPerOutput,
         current_best: Optional[np.ndarray],
     ) -> np.ndarray:
@@ -285,16 +285,16 @@
     def _compute_head_and_gradient(
         self,
         output_to_predictions: SamplePredictionsPerOutput,
         current_best: Optional[np.ndarray],
     ) -> HeadWithGradient:
         """
         Returns minus cost-aware expected improvement and, for each output
-        model, the gradients with respect to the mean and standard deviation of
-        that model.
+        predictor, the gradients with respect to the mean and standard deviation of
+        that predictor.
         """
         assert current_best is not None
         mean, std = self._extract_mean_and_std(output_to_predictions)
         pred_cost = self._extract_positive_cost(output_to_predictions)
         nf_active = mean.size
         nf_cost = pred_cost.size
 
@@ -317,26 +317,26 @@
         }
         return HeadWithGradient(hval=-np.mean(f_acqu), gradient=gradient)
 
     def _extract_positive_cost(self, output_to_predictions):
         pred_cost = output_to_predictions[self.cost_metric]["mean"]
         if np.any(pred_cost) < 0.0:
             logger.warning(
-                f"The model for {self.cost_metric} predicted some negative cost. "
+                f"The predictor for {self.cost_metric} predicted some negative cost. "
                 f"Capping the minimum cost at {MIN_COST}."
             )
         pred_cost = np.maximum(
             pred_cost, MIN_COST
         )  # ensure that the predicted cost/run-time is positive
         return pred_cost
 
 
 class ConstraintCurrentBestProvider(CurrentBestProvider):
     """
-    Here, ``current_best`` depends on two models, for active and constraint metric.
+    Here, ``current_best`` depends on two predictors, for active and constraint metric.
     """
 
     def __init__(self, current_best_list: List[np.ndarray], num_samples_active: int):
         list_size = len(current_best_list)
         assert list_size > 0 and list_size % num_samples_active == 0
         self._active_and_constraint_current_best = [
             v.reshape((1, -1)) for v in current_best_list
@@ -374,32 +374,34 @@
         | ICML 2014
     and
 
         | Gelbart et al.
         | Bayesian Optimization with Unknown Constraints
         | UAI 2014.
 
-    :param model: Surrogate models for main objective and cost
+    :param predictor: Predictors for main objective and cost
     :param active_metric: Name of main objective
     :param jitter: Jitter factor, must be positive. Defaults to 0.01
     """
 
     def __init__(
         self,
-        model: SurrogateOutputModel,
+        predictor: OutputPredictor,
         active_metric: Optional[str] = None,
         jitter: float = 0.01,
     ):
-        super().__init__(model, active_metric)
+        super().__init__(predictor, active_metric)
         self.jitter = jitter
         self._feasible_best_list = None
         (
             self.active_metric,
             self.constraint_metric,
-        ) = _extract_active_and_secondary_metric(self.model_output_names, active_metric)
+        ) = _extract_active_and_secondary_metric(
+            self.predictor_output_names, active_metric
+        )
 
     def _head_needs_current_best(self) -> bool:
         return True
 
     def _compute_head(
         self,
         output_to_predictions: SamplePredictionsPerOutput,
@@ -429,16 +431,16 @@
 
     def _compute_head_and_gradient(
         self,
         output_to_predictions: SamplePredictionsPerOutput,
         current_best: Optional[np.ndarray],
     ) -> HeadWithGradient:
         """
-        Returns minus cost-aware expected improvement (- CEI) and, for each output model, the gradients
-        with respect to the mean and standard deviation of that model.
+        Returns minus cost-aware expected improvement (- CEI) and, for each output predictor, the gradients
+        with respect to the mean and standard deviation of that predictor.
         """
         assert current_best is not None
         mean, std = self._extract_mean_and_std(output_to_predictions)
         mean_constr, std_constr = self._extract_mean_and_std(
             output_to_predictions, metric=self.constraint_metric
         )
         nf_mean = mean.size
@@ -490,27 +492,27 @@
             self.constraint_metric: dict(
                 mean=dh_dmean_constraint, std=dh_dstd_constraint
             ),
         }
         return HeadWithGradient(hval=-np.mean(f_acqu), gradient=gradient)
 
     def _get_current_bests_internal(
-        self, model: SurrogateOutputModel
+        self, predictor: OutputPredictor
     ) -> CurrentBestProvider:
-        active_model = model[self.active_metric]
-        assert isinstance(active_model, BaseSurrogateModel)
-        all_means_active = active_model.predict_mean_current_candidates()
+        active_predictor = predictor[self.active_metric]
+        assert isinstance(active_predictor, BasePredictor)
+        all_means_active = active_predictor.predict_mean_current_candidates()
         num_samples_active = len(all_means_active)
-        constraint_model = model[self.constraint_metric]
-        assert isinstance(constraint_model, BaseSurrogateModel)
-        all_means_constraint = constraint_model.predict_mean_current_candidates()
+        constraint_predictor = predictor[self.constraint_metric]
+        assert isinstance(constraint_predictor, BasePredictor)
+        all_means_constraint = constraint_predictor.predict_mean_current_candidates()
         common_shape = all_means_active[0].shape
         assert all(
             x.shape == common_shape for x in all_means_constraint
-        ), "Shape mismatch between models for predict_mean_current_candidates"
+        ), "Shape mismatch between predictors for predict_mean_current_candidates"
         current_best_list = []
         for means_constraint, means_active in itertools.product(
             all_means_constraint, all_means_active
         ):
             # Remove all infeasible candidates (i.e., where means_constraint
             # is >= 0)
             means_active[means_constraint >= 0] = np.nan
```

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/model_base.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/model_base.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,25 +14,25 @@
 import numpy as np
 import logging
 
 from syne_tune.optimizer.schedulers.searchers.bayesopt.datatypes.tuning_job_state import (
     TuningJobState,
 )
 from syne_tune.optimizer.schedulers.searchers.bayesopt.tuning_algorithms.base_classes import (
-    SurrogateModel,
+    Predictor,
 )
 from syne_tune.optimizer.schedulers.searchers.utils.common import ConfigurationFilter
 
 logger = logging.getLogger(__name__)
 
 
-class BaseSurrogateModel(SurrogateModel):
+class BasePredictor(Predictor):
     """
     Base class for (most)
-    :class:`~syne_tune.optimizer.schedulers.searchers.bayesopt.tuning_algorithms.base_classes.SurrogateModel`
+    :class:`~syne_tune.optimizer.schedulers.searchers.bayesopt.tuning_algorithms.base_classes.Predictor`
     implementations, provides common code.
     """
 
     def __init__(
         self,
         state: TuningJobState,
         active_metric: Optional[str] = None,
```

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/model_skipopt.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/model_skipopt.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/model_transformer.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/model_transformer.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,28 +12,28 @@
 # permissions and limitations under the License.
 from typing import Dict, Optional, Callable, Union
 import logging
 import copy
 
 from numpy.random import RandomState
 
+from syne_tune.optimizer.schedulers.searchers.bayesopt.models.estimator import (
+    Estimator,
+    OutputEstimator,
+)
 from syne_tune.optimizer.schedulers.searchers.bayesopt.tuning_algorithms.base_classes import (
-    SurrogateModel,
-    SurrogateOutputModel,
+    OutputPredictor,
 )
 from syne_tune.optimizer.schedulers.searchers.bayesopt.datatypes.tuning_job_state import (
     TuningJobState,
 )
 from syne_tune.optimizer.schedulers.searchers.bayesopt.models.model_skipopt import (
     SkipOptimizationPredicate,
     NeverSkipPredicate,
 )
-from syne_tune.optimizer.schedulers.searchers.bayesopt.utils.debug_log import (
-    DebugLogPrinter,
-)
 from syne_tune.optimizer.schedulers.searchers.bayesopt.datatypes.common import (
     PendingEvaluation,
     TrialEvaluations,
     dictionarize_objective,
     INTERNAL_METRIC_NAME,
 )
 from syne_tune.optimizer.schedulers.searchers.utils.common import Configuration
@@ -43,72 +43,17 @@
 
 def _assert_same_keys(dict1, dict2):
     assert set(dict1.keys()) == set(
         dict2.keys()
     ), f"{list(dict1.keys())} and {list(dict2.keys())} need to be the same keys. "
 
 
-class TransformerModelFactory:
-    """
-    Interface for model factories used in :class:`ModelStateTransformer`. A model
-    factory provides access to tunable model parameters, and :meth:`model` creates
-    :class:`~syne_tune.optimizer.schedulers.searchers.bayesopt.tuning_algorithms.base_classes.SurrogateModel`
-    instances.
-    """
-
-    def get_params(self) -> Dict:
-        """
-        :return: Current tunable model parameters
-        """
-        raise NotImplementedError()
-
-    def set_params(self, param_dict: Dict):
-        """
-        :param param_dict: New model parameters
-        """
-        raise NotImplementedError()
-
-    def model(self, state: TuningJobState, fit_params: bool) -> SurrogateModel:
-        """
-        Creates a
-        :class:`~syne_tune.optimizer.schedulers.searchers.bayesopt.tuning_algorithms.base_classes.SurrogateModel`
-        object based on data in ``state``. This involves fitting model parameters
-        if ``fit_params == True``. Otherwise, the current model parameters are not
-        changed (so may be stale, given that ``state`` has changed). The idea is that
-        often, model fitting is much more expensive than just creating the final
-        :class:`SurrogateModel` (posterior state). It then makes sense to partly
-        work with stale model parameters.
-
-        :param state: Current data model parameters are to be fit on, and the
-            posterior state is to be computed from
-        :param fit_params: See above
-        :return: Fitted model, wrapping the posterior state for predictions
-        """
-        raise NotImplementedError()
-
-    @property
-    def debug_log(self) -> Optional[DebugLogPrinter]:
-        return None
-
-    def configure_scheduler(self, scheduler):
-        """
-        Called by :meth:`configure_scheduler` of searchers which make use of a
-        class:``TransformerModelFactory``. Allows the factory to depend on
-        parameters of the scheduler.
-
-        :param scheduler: Scheduler object
-        """
-        pass
-
-
-# Convenience types allowing for multi-output HPO. These are used for methods that work both in the standard case
-# of a single output model and in the multi-output case
-TransformerOutputModelFactory = Union[
-    TransformerModelFactory, Dict[str, TransformerModelFactory]
-]
+# Convenience type allowing for multi-output HPO. These are used for methods
+# that work both in the standard case of a single output model and in the
+# multi-output case
 
 SkipOptimizationOutputPredicate = Union[
     SkipOptimizationPredicate, Dict[str, SkipOptimizationPredicate]
 ]
 
 
 class StateForModelConverter:
@@ -137,16 +82,16 @@
     """
     This class maintains the
     :class:`~syne_tune.optimizer.schedulers.searchers.bayesopt.datatypes.tuning_job_state.TuningJobState`
     object alongside an HPO experiment, and manages the reaction to changes of
     this state. In particular, it provides a fitted surrogate model on demand,
     which encapsulates the GP posterior.
 
-    The state transformer is generic, it uses :class:`TransformerModelFactory`
-    for anything specific to the model type.
+    The state transformer is generic, it uses :class:`Estimator` for anything specific
+    to the model type.
 
     ``skip_optimization`` is a predicate depending on the state, determining
     what is done at the next recent call of ``model``. If ``False``, the model
     parameters are refit, otherwise the current ones are not changed (which
     is usually faster, but risks stale-ness).
 
     We also track the observed data ``state.trials_evaluations``. If this
@@ -156,80 +101,80 @@
     not on other fields (e.g., pending evaluations).
 
     If given, ``state_converter`` maps the state to another one which is then
     passed to the model for fitting and predictions. One important use case is
     filtering down data when model fitting is superlinear. Another is to convert
     multi-fidelity setups to be used with single-fidelity models inside.
 
-    Note that ``model_factory`` and ``skip_optimization`` can also be a dictionary mapping
+    Note that ``estimator`` and ``skip_optimization`` can also be a dictionary mapping
     output names to models. In that case, the state is shared but the models for each
     output metric are updated independently.
 
-    :param model_factory: Factory for surrogate models, given tuning job state
+    :param estimator: Surrogate model(s)
     :param init_state: Initial tuning job state
     :param skip_optimization: Skip optimization predicate (see above). Defaults to
         ``None`` (fitting is never skipped)
     :param state_converter: See above, optional
     """
 
     def __init__(
         self,
-        model_factory: TransformerOutputModelFactory,
+        estimator: OutputEstimator,
         init_state: TuningJobState,
         skip_optimization: Optional[SkipOptimizationOutputPredicate] = None,
         state_converter: Optional[StateForModelConverter] = None,
     ):
         self._use_single_model = False
-        if isinstance(model_factory, TransformerModelFactory):
+        if isinstance(estimator, Estimator):
             self._use_single_model = True
         if not self._use_single_model:
-            assert isinstance(model_factory, Dict), (
-                f"{model_factory} is not an instance of TransformerModelFactory. "
+            assert isinstance(estimator, dict), (
+                f"{estimator} is not an instance of Estimator. "
                 f"It is assumed that we are in the multi-output case and that it "
                 f"must be a Dict. No other types are supported. "
             )
-            _assert_same_keys(model_factory, skip_optimization)
+            _assert_same_keys(estimator, skip_optimization)
             # Default: Always refit model parameters for each output model
             if skip_optimization is None:
                 skip_optimization = {
                     output_name: NeverSkipPredicate()
-                    for output_name in model_factory.keys()
+                    for output_name in estimator.keys()
                 }
             else:
                 assert isinstance(skip_optimization, Dict), (
                     f"{skip_optimization} must be a Dict, consistently "
-                    f"with {model_factory}."
+                    f"with {estimator}."
                 )
                 skip_optimization = {
                     output_name: skip_optimization[output_name]
                     if skip_optimization.get(output_name) is not None
                     else NeverSkipPredicate()
-                    for output_name in model_factory.keys()
+                    for output_name in estimator.keys()
                 }
             # debug_log is shared by all output models
-            self._debug_log = next(iter(model_factory.values())).debug_log
+            self._debug_log = next(iter(estimator.values())).debug_log
         else:
             if skip_optimization is None:
                 # Default: Always refit model parameters
                 skip_optimization = NeverSkipPredicate()
             assert isinstance(skip_optimization, SkipOptimizationPredicate)
-            self._debug_log = model_factory.debug_log
-            # Make model_factory and skip_optimization single-key dictionaries
+            self._debug_log = estimator.debug_log
+            # Make ``estimator`` and ``skip_optimization`` single-key dictionaries
             # for convenience, so that we can treat the single model and multi-model case in the same way
-            model_factory = dictionarize_objective(model_factory)
+            estimator = dictionarize_objective(estimator)
             skip_optimization = dictionarize_objective(skip_optimization)
-        self._model_factory = model_factory
+        self._estimator = estimator
         self._skip_optimization = skip_optimization
         self._state_converter = state_converter
         self._state = copy.copy(init_state)
-        # SurrogateOutputModel computed on demand
-        self._model: Optional[SurrogateOutputModel] = None
+        # OutputPredictor computed on demand
+        self._predictor: Optional[OutputPredictor] = None
         # Observed data for which model parameters were re-fit most
         # recently, separately for each model
-        self._num_evaluations = {output_name: 0 for output_name in model_factory.keys()}
+        self._num_evaluations = {output_name: 0 for output_name in estimator.keys()}
 
     @property
     def state(self) -> TuningJobState:
         return self._state
 
     def _unwrap_from_dict(self, x):
         if self._use_single_model:
@@ -238,49 +183,49 @@
             return x
 
     @property
     def use_single_model(self) -> bool:
         return self._use_single_model
 
     @property
-    def model_factory(self) -> TransformerOutputModelFactory:
-        return self._unwrap_from_dict(self._model_factory)
+    def estimator(self) -> OutputEstimator:
+        return self._unwrap_from_dict(self._estimator)
 
     @property
     def skip_optimization(self) -> SkipOptimizationOutputPredicate:
         return self._unwrap_from_dict(self._skip_optimization)
 
-    def model(self, **kwargs) -> SurrogateOutputModel:
+    def fit(self, **kwargs) -> OutputPredictor:
         """
-        If skip_optimization is given, it overrides the ``self._skip_optimization``
+        If ``skip_optimization`` is given, it overrides the ``self._skip_optimization``
         predicate.
 
         :return: Fitted surrogate model for current state in the standard single
             model case; in the multi-model case, it returns a dictionary mapping
             output names to surrogate model instances for current state (shared
             across models).
         """
-        if self._model is None:
+        if self._predictor is None:
             skip_optimization = kwargs.get("skip_optimization")
-            self._compute_model(skip_optimization=skip_optimization)
-        return self._unwrap_from_dict(self._model)
+            self._compute_predictor(skip_optimization=skip_optimization)
+        return self._unwrap_from_dict(self._predictor)
 
     def get_params(self):
         params = {
-            output_name: output_model.get_params()
-            for output_name, output_model in self._model_factory.items()
+            output_name: output_estimator.get_params()
+            for output_name, output_estimator in self._estimator.items()
         }
         return self._unwrap_from_dict(params)
 
     def set_params(self, param_dict):
         if self._use_single_model:
             param_dict = dictionarize_objective(param_dict)
-        _assert_same_keys(self._model_factory, param_dict)
-        for output_name in self._model_factory:
-            self._model_factory[output_name].set_params(param_dict[output_name])
+        _assert_same_keys(self._estimator, param_dict)
+        for output_name in self._estimator:
+            self._estimator[output_name].set_params(param_dict[output_name])
 
     def append_trial(
         self,
         trial_id: str,
         config: Optional[Configuration] = None,
         resource: Optional[int] = None,
     ):
@@ -289,15 +234,15 @@
 
         :param trial_id: ID of trial
         :param config: Must be given if this trial does not yet feature in the
             state
         :param resource: Must be given in the multi-fidelity case, to specify
             at which resource level the evaluation is pending
         """
-        self._model = None  # Invalidate
+        self._predictor = None  # Invalidate
         self._state.append_pending(trial_id, config=config, resource=resource)
 
     def drop_pending_evaluation(
         self, trial_id: str, resource: Optional[int] = None
     ) -> bool:
         """
         Drop pending evaluation from state. If it is not listed as pending,
@@ -370,38 +315,38 @@
         # Assign / append new labels
         metrics = self._state.metrics_for_trial(trial_id, config=config)
         for name, new_labels in data.metrics.items():
             if name not in metrics or not isinstance(new_labels, dict):
                 metrics[name] = new_labels
             else:
                 metrics[name].update(new_labels)
-        self._model = None  # Invalidate
+        self._predictor = None  # Invalidate
 
     def filter_pending_evaluations(
         self, filter_pred: Callable[[PendingEvaluation], bool]
     ):
         """
         Filters ``state.pending_evaluations`` with ``filter_pred``.
 
         :param filter_pred: Filtering predicate
         """
         new_pending_evaluations = list(
             filter(filter_pred, self._state.pending_evaluations)
         )
         if len(new_pending_evaluations) != len(self._state.pending_evaluations):
-            self._model = None  # Invalidate
+            self._predictor = None  # Invalidate
             del self._state.pending_evaluations[:]
             self._state.pending_evaluations.extend(new_pending_evaluations)
 
     def mark_trial_failed(self, trial_id: str):
         failed_trials = self._state.failed_trials
         if trial_id not in failed_trials:
             failed_trials.append(trial_id)
 
-    def _compute_model(self, skip_optimization=None):
+    def _compute_predictor(self, skip_optimization=None):
         if skip_optimization is None:
             skip_optimization = dict()
             for (
                 output_name,
                 output_skip_optimization,
             ) in self._skip_optimization.items():
                 skip_optimization[output_name] = output_skip_optimization(self._state)
@@ -410,34 +355,34 @@
         if self._debug_log is not None:
             for output_name, skip_opt in skip_optimization.items():
                 if skip_opt:
                     logger.info(
                         f"Skipping the refitting of model parameters for {output_name}"
                     )
 
-        _assert_same_keys(skip_optimization, self._model_factory)
+        _assert_same_keys(skip_optimization, self._estimator)
         state_for_model = (
             self._state
             if self._state_converter is None
             else self._state_converter(self._state)
         )
-        output_models = dict()
+        output_predictors = dict()
         for output_name, output_skip_optimization in skip_optimization.items():
-            fit_params = not output_skip_optimization
-            if fit_params:
+            update_params = not output_skip_optimization
+            if update_params:
                 # Did the labeled data really change since the last recent refit?
                 # If not, skip the refitting
                 num_evaluations = self._state.num_observed_cases(output_name)
                 if num_evaluations == self._num_evaluations[output_name]:
-                    fit_params = False
+                    update_params = False
                     if self._debug_log is not None:
                         logger.info(
                             f"Skipping the refitting of model parameters for {output_name}, "
                             f"since the labeled data did not change since the last recent fit"
                         )
                 else:
                     # Model will be refitted: Update
                     self._num_evaluations[output_name] = num_evaluations
-            output_models[output_name] = self._model_factory[output_name].model(
-                state=state_for_model, fit_params=fit_params
-            )
-        self._model = output_models
+            output_predictors[output_name] = self._estimator[
+                output_name
+            ].fit_from_state(state=state_for_model, update_params=update_params)
+        self._predictor = output_predictors
```

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/subsample_state_multi_fidelity.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/subsample_state_multi_fidelity.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/subsample_state_single_fidelity.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/subsample_state_single_fidelity.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/__init__.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/sklearn/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/base_classes.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/base_classes.py`

 * *Files 12% similar despite different names*

```diff
@@ -33,47 +33,50 @@
 from syne_tune.optimizer.schedulers.searchers.utils.common import Configuration
 from syne_tune.optimizer.schedulers.searchers.utils.exclusion_list import ExclusionList
 from syne_tune.optimizer.schedulers.searchers.utils.hp_ranges import (
     HyperparameterRanges,
 )
 
 
-def assign_active_metric(model, active_metric):
-    """Checks that active_metric is provided when model consists of multiple output models.
-    Otherwise, just sets active_metric to the only model output name available.
+def assign_active_metric(predictor, active_metric):
+    """Checks that active_metric is provided when predictor consists of multiple output predictors.
+    Otherwise, just sets active_metric to the only predictor output name available.
     """
-    model_output_names = sorted(model.keys())
-    num_output_models = len(model_output_names)
-    if num_output_models == 1:
+    predictor_output_names = sorted(predictor.keys())
+    num_output_predictors = len(predictor_output_names)
+    if num_output_predictors == 1:
         if active_metric is not None:
-            assert active_metric == model_output_names[0], (
-                "Only a single output model is given. "
-                "Active metric must be set to that output model."
+            assert active_metric == predictor_output_names[0], (
+                "Only a single output predictor is given. "
+                "Active metric must be set to that output predictor."
             )
-        active_metric = model_output_names[0]
+        active_metric = predictor_output_names[0]
     else:
         assert active_metric is not None, (
-            f"As model has {num_output_models}, active metric cannot be None. "
-            f"Please set active_metric to one of the model output names: "
-            f"{model_output_names}."
+            f"As predictor has {num_output_predictors}, active metric cannot be None. "
+            f"Please set active_metric to one of the predictor output names: "
+            f"{predictor_output_names}."
         )
-        assert active_metric in model_output_names
+        assert active_metric in predictor_output_names
     return active_metric
 
 
 class NextCandidatesAlgorithm:
     def next_candidates(self) -> List[Configuration]:
         raise NotImplementedError
 
 
-class SurrogateModel:
+class Predictor:
     """
-    Base class of surrogate models for Bayesian optimization. A surrogate model
-    supports marginal predictions feeding into an acquisition function, as well
-    as suppport to compute gradients of an acquisition function w.r.t. inputs.
+    Base class for probabilistic predictors used in Bayesian optimization. They
+    support marginal predictions feeding into an acquisition function, as well
+    as computing gradients of an acquisition function w.r.t. inputs.
+
+    In general, a predictor is created by an estimator. It wraps a posterior
+    state, which allows for probabilistic predictions on arbitrary inputs.
 
     :param state: Tuning job state
     :param active_metric: Name of internal objective
     """
 
     def __init__(self, state: TuningJobState, active_metric: Optional[str] = None):
         self.state = state
@@ -98,15 +101,15 @@
     def predict(self, inputs: np.ndarray) -> List[Dict[str, np.ndarray]]:
         """
         Returns signals which are statistics of the predictive distribution at
         input points ``inputs``. By default:
 
         * "mean": Predictive means. If the model supports fantasizing with a
             number ``nf`` of fantasies, this has shape ``(n, nf)``, otherwise ``(n,)``
-        - "std": Predictive stddevs, shape ``(n,)``
+        * "std": Predictive stddevs, shape ``(n,)``
 
         If the hyperparameters of the surrogate model are being optimized (e.g.,
         by empirical Bayes), the returned list has length 1. If its
         hyperparameters are averaged over by MCMC, the returned list has one
         entry per MCMC sample.
 
         :param inputs: Input points, shape ``(n, d)``
@@ -170,153 +173,156 @@
         :param input: Single input point :math:`x`, shape ``(d,)``
         :param head_gradients: See above
         :return: Gradient :math:`\nabla f(x)` (several if MCMC is used)
         """
         raise NotImplementedError
 
 
-# Useful type that allows for a dictionary mapping each output name to a SurrogateModel.
+# Useful type that allows for a dictionary mapping each output name to a Predictor.
 # This is needed for multi-output BO methods such as constrained BO, where each output
-# is associated to a model. This type includes the Union with the standard
-# SurrogateModel type for backward compatibility.
-SurrogateOutputModel = Union[SurrogateModel, Dict[str, SurrogateModel]]
+# is associated to a predictor. This type includes the Union with the standard
+# Predictor type for backward compatibility.
+OutputPredictor = Union[Predictor, Dict[str, Predictor]]
 
 
 class ScoringFunction:
     """
     Class to score candidates. As opposed to acquisition functions, scores do
     not support gradient computation. Note that scores are always minimized.
     """
 
+    def __init__(
+        self, predictor: OutputPredictor = None, active_metric: Optional[str] = None
+    ):
+        self.predictor = predictor
+        if active_metric is None:
+            active_metric = INTERNAL_METRIC_NAME
+        self.active_metric = active_metric
+
     def score(
         self,
         candidates: Iterable[Configuration],
-        model: Optional[SurrogateOutputModel] = None,
+        predictor: Optional[OutputPredictor] = None,
     ) -> List[float]:
         """
         :param candidates: Configurations for which scores are to be computed
-        :param model: Overrides default surrogate model
+        :param predictor: Overrides default  predictor
         :return: List of score values, length of ``candidates``
         """
         raise NotImplementedError
 
 
 class AcquisitionFunction(ScoringFunction):
     """
     Base class for acquisition functions :math:`f(x)`.
 
-    :param model: Surrogate model providing predictive statistics (e.g.,
-        mean, variance)
+    :param predictor: Predictor(s) from surrogate model
     :param active_metric: Name of internal metric
     """
 
-    def __init__(
-        self, model: SurrogateOutputModel, active_metric: Optional[str] = None
-    ):
-        self.model = model
-        if active_metric is None:
-            active_metric = INTERNAL_METRIC_NAME
-        self.active_metric = active_metric
-
     def compute_acq(
-        self, inputs: np.ndarray, model: Optional[SurrogateOutputModel] = None
+        self, inputs: np.ndarray, predictor: Optional[OutputPredictor] = None
     ) -> np.ndarray:
         """
         Note: If inputs has shape ``(d,)``, it is taken to be ``(1, d)``
 
         :param inputs: Encoded input points, shape ``(n, d)``
-        :param model: If given, overrides ``self.model``
+        :param predictor: If given, overrides ``self.predictor``
         :return: Acquisition function values, shape ``(n,)``
         """
         raise NotImplementedError
 
     def compute_acq_with_gradient(
-        self, input: np.ndarray, model: Optional[SurrogateOutputModel] = None
+        self, input: np.ndarray, predictor: Optional[OutputPredictor] = None
     ) -> Tuple[float, np.ndarray]:
         """
         For a single input point :math:`x`, compute acquisition function value
         :math:`f(x)` and gradient :math:`\nabla f(x)`.
 
         :param input: Single input point :math:`x`, shape ``(d,)``
-        :param model: If given, overrides ``self.model``
+        :param predictor: If given, overrides ``self.predictor``
         :return: :math:`(f(x), \nabla f(x))`
         """
         raise NotImplementedError
 
     def score(
         self,
         candidates: Iterable[Configuration],
-        model: Optional[SurrogateOutputModel] = None,
+        predictor: Optional[OutputPredictor] = None,
     ) -> List[float]:
-        if model is None:
-            model = self.model
-        if isinstance(model, dict):
-            active_model = model[self.active_metric]
+        if predictor is None:
+            predictor = self.predictor
+        if isinstance(predictor, dict):
+            active_predictor = predictor[self.active_metric]
         else:
-            active_model = model
-        hp_ranges = active_model.hp_ranges_for_prediction()
+            active_predictor = predictor
+        hp_ranges = active_predictor.hp_ranges_for_prediction()
         inputs = hp_ranges.to_ndarray_matrix(candidates)
-        return list(self.compute_acq(inputs, model=model))
+        return list(self.compute_acq(inputs, predictor=predictor))
 
 
 AcquisitionClassAndArgs = Union[
     Type[AcquisitionFunction], Tuple[Type[AcquisitionFunction], Dict[str, Any]]
 ]
 
+ScoringClassAndArgs = Union[
+    Type[ScoringFunction], Tuple[Type[ScoringFunction], Dict[str, Any]]
+]
+
 
 def unwrap_acquisition_class_and_kwargs(
     acquisition_class: AcquisitionClassAndArgs,
 ) -> (Type[AcquisitionFunction], Dict[str, Any]):
     if isinstance(acquisition_class, tuple):
         return acquisition_class
     else:
         return acquisition_class, dict()
 
 
 class LocalOptimizer:
     """
     Class that tries to find a local candidate with a better score, typically
     using a local optimization method such as L-BFGS. It would normally
-    encapsulate an acquisition function and model.
+    encapsulate an acquisition function and predictor.
 
     ``acquisition_class`` contains the type of the acquisition function
     (subclass of :class:`AcquisitionFunction`). It can also be a tuple of the
     form ``(type, kwargs)``, where ``kwargs`` are extra arguments to the class
     constructor.
 
     :param hp_ranges: Feature generator for configurations
-    :param model: Surrogate model for acquisition function
+    :param predictor: Predictor(s) for acquisition function
     :param acquisition_class: See above
     :param active_metric: Name of internal metric
     """
 
     def __init__(
         self,
         hp_ranges: HyperparameterRanges,
-        model: SurrogateOutputModel,
+        predictor: OutputPredictor,
         acquisition_class: AcquisitionClassAndArgs,
         active_metric: Optional[str] = None,
     ):
         self.hp_ranges = hp_ranges
-        self.model = model
+        self.predictor = predictor
         if active_metric is None:
             active_metric = INTERNAL_METRIC_NAME
-        if isinstance(model, dict):
-            self.active_metric = assign_active_metric(model, active_metric)
+        if isinstance(predictor, dict):
+            self.active_metric = assign_active_metric(predictor, active_metric)
         else:
             self.active_metric = active_metric
         self.acquisition_class = acquisition_class
 
     def optimize(
-        self, candidate: Configuration, model: Optional[SurrogateOutputModel] = None
+        self, candidate: Configuration, predictor: Optional[OutputPredictor] = None
     ) -> Configuration:
         """Run local optimization, starting from ``candidate``
 
         :param candidate: Starting point
-        :param model: Overrides ``self.model``
+        :param predictor: Overrides ``self.predictor``
         :return: Configuration found by local optimization
         """
         raise NotImplementedError
 
 
 class CandidateGenerator:
     """
```

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/bo_algorithm.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/bo_algorithm.py`

 * *Files 22% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from syne_tune.optimizer.schedulers.searchers.bayesopt.models.model_transformer import (
     ModelStateTransformer,
 )
 from syne_tune.optimizer.schedulers.searchers.bayesopt.tuning_algorithms.base_classes import (
     NextCandidatesAlgorithm,
     ScoringFunction,
     LocalOptimizer,
-    SurrogateModel,
+    Predictor,
     CandidateGenerator,
 )
 from syne_tune.optimizer.schedulers.searchers.bayesopt.tuning_algorithms.bo_algorithm_components import (
     LBFGSOptimizeAcquisition,
     generate_unique_candidates,
     DuplicateDetector,
 )
@@ -106,18 +106,18 @@
     greedy_batch_selection: bool
     duplicate_detector: DuplicateDetector
     num_initial_candidates_for_batch: Optional[int] = None
     sample_unique_candidates: bool = False
     debug_log: Optional[DebugLogPrinter] = None
 
     # Note: For greedy batch selection (num_outer_iterations > 1), the
-    # underlying SurrrogateModel changes with each new pending candidate. The
-    # model changes are managed by pending_candidate_state_transformer. The
-    # model has to be passed to both initial_candidates_scorer and
-    # local_optimizer.
+    # underlying ``Predictor`` changes with each new pending candidate. The
+    # model changes are managed by ``pending_candidate_state_transformer``. The
+    # model has to be passed to both ``initial_candidates_scorer`` and
+    # ``local_optimizer``.
     def next_candidates(self) -> List[Configuration]:
         if self.greedy_batch_selection:
             # Select batch greedily, one candidate at a time, updating the
             # model in between
             num_outer_iterations = self.num_requested_candidates
             num_inner_candidates = 1
         else:
@@ -144,15 +144,15 @@
                 try:
                     next_trial_id = max(next_trial_id, int(trial_id))
                 except ValueError:
                     pass
             next_trial_id += 1
         candidates = []
         just_added = True
-        model = None  # SurrogateModel, if num_outer_iterations > 1
+        predictor = None  # Predictor, if num_outer_iterations > 1
         for outer_iter in range(num_outer_iterations):
             if just_added:
                 if self.exclusion_candidates.config_space_exhausted():
                     logger.warning(
                         "All entries of finite config space (size "
                         + f"{self.exclusion_candidates.configspace_size}) have been selected. Returning "
                         + f"{len(candidates)} configs instead of {self.num_requested_candidates}"
@@ -165,15 +165,15 @@
                 and outer_iter > 0
             ):
                 num_initial_candidates = self.num_initial_candidates_for_batch
             else:
                 num_initial_candidates = self.num_initial_candidates
             inner_candidates = self._get_next_candidates(
                 num_inner_candidates,
-                model=model,
+                predictor=predictor,
                 num_initial_candidates=num_initial_candidates,
             )
             candidates.extend(inner_candidates)
             if outer_iter < num_outer_iterations - 1 and len(inner_candidates) > 0:
                 just_added = True
                 # This is not the last outer iteration
                 for cand in inner_candidates:
@@ -182,15 +182,15 @@
                 # Note: We suppress fit_hyperpars for models obtained during
                 # batch selection
                 for candidate in inner_candidates:
                     self.pending_candidate_state_transformer.append_trial(
                         trial_id=str(next_trial_id), config=candidate
                     )
                     next_trial_id += 1
-                model = self.pending_candidate_state_transformer.model(
+                predictor = self.pending_candidate_state_transformer.fit(
                     skip_optimization=True
                 )
             if (
                 len(inner_candidates) < num_inner_candidates
                 and len(candidates) < self.num_requested_candidates
             ):
                 logger.warning(
@@ -201,15 +201,15 @@
                 break
 
         return candidates
 
     def _get_next_candidates(
         self,
         num_candidates: int,
-        model: Optional[SurrogateModel],
+        predictor: Optional[Predictor],
         num_initial_candidates: Optional[int] = None,
     ):
         if num_initial_candidates is None:
             num_initial_candidates = self.num_initial_candidates
         # generate a random candidates among which to pick the ones to be
         # locally optimized
         logger.info(
@@ -230,88 +230,90 @@
                 self.initial_candidates_generator.generate_candidates_en_bulk(
                     num_initial_candidates, exclusion_list=self.exclusion_candidates
                 )
             )
         logger.info("BayesOpt Algorithm: Scoring (and reordering) candidates.")
         if self.debug_log is not None:
             candidates_and_scores = _order_candidates(
-                initial_candidates,
-                self.initial_candidates_scorer,
-                model=model,
+                candidates=initial_candidates,
+                scoring_function=self.initial_candidates_scorer,
+                predictor=predictor,
                 with_scores=True,
             )
             initial_candidates = [cand for score, cand in candidates_and_scores]
             config = initial_candidates[0]
             top_scores = np.array([x for x, _ in candidates_and_scores[:5]])
             self.debug_log.set_init_config(config, top_scores)
         else:
             initial_candidates = _order_candidates(
-                initial_candidates, self.initial_candidates_scorer, model=model
+                candidates=initial_candidates,
+                scoring_function=self.initial_candidates_scorer,
+                predictor=predictor,
             )
         candidates_with_optimization = _lazily_locally_optimize(
-            initial_candidates,
-            self.local_optimizer,
+            candidates=initial_candidates,
+            local_optimizer=self.local_optimizer,
             hp_ranges=self.exclusion_candidates.hp_ranges,
-            model=model,
+            predictor=predictor,
         )
         logger.info("BayesOpt Algorithm: Selecting final set of candidates.")
         if self.debug_log is not None and isinstance(
             self.local_optimizer, LBFGSOptimizeAcquisition
         ):
             # We would like to get num_evaluations from the first run (usually
             # the only one). This requires peeking at the first entry of the
             # iterator
             peek = candidates_with_optimization.__next__()
             self.debug_log.set_num_evaluations(self.local_optimizer.num_evaluations)
             candidates_with_optimization = itertools.chain(
                 [peek], candidates_with_optimization
             )
         candidates = _pick_from_locally_optimized(
-            candidates_with_optimization,
-            self.exclusion_candidates,
-            num_candidates,
-            self.duplicate_detector,
+            candidates_with_optimization=candidates_with_optimization,
+            exclusion_candidates=self.exclusion_candidates,
+            num_candidates=num_candidates,
+            duplicate_detector=self.duplicate_detector,
         )
         return candidates
 
 
 def _order_candidates(
     candidates: List[Configuration],
     scoring_function: ScoringFunction,
-    model: Optional[SurrogateModel],
+    predictor: Optional[Predictor],
     with_scores: bool = False,
 ):
     if len(candidates) == 0:
         return []
     # scored in batch as this can be more efficient
-    scores = scoring_function.score(candidates, model=model)
+    scores = scoring_function.score(candidates, predictor=predictor)
     sorted_list = sorted(zip(scores, candidates), key=lambda x: x[0])
     if with_scores:
         return sorted_list
     else:
         return [cand for score, cand in sorted_list]
 
 
 def _lazily_locally_optimize(
     candidates: List[Configuration],
     local_optimizer: LocalOptimizer,
     hp_ranges: HyperparameterRanges,
-    model: Optional[SurrogateModel],
+    predictor: Optional[Predictor],
 ) -> Iterator[Tuple[Configuration, Configuration]]:
     """
     Due to local deduplication we do not know in advance how many candidates
     we have to locally optimize, hence this helper to create a lazy generator
     of locally optimized candidates.
     Note that ``candidates`` may contain duplicates, but such are skipped here.
     """
     considered_already = ExclusionList(hp_ranges)
     for cand in candidates:
         if not considered_already.contains(cand):
             considered_already.add(cand)
-            yield cand, local_optimizer.optimize(cand, model=model)
+            yield cand, local_optimizer.optimize(cand, predictor=predictor)
 
 
 # Note: If ``duplicate_detector`` is at least :class:`DuplicateDetectorIdentical`,
 # it will filter out candidates in exclusion_candidates here. Such can in
 # principle arise if ``sample_unique_candidates == False``. This does not work
 # if ``duplicate_detector`` is of type :class:`DuplicateDetectorNoDetection`.
 def _pick_from_locally_optimized(
```

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/bo_algorithm_components.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/bo_algorithm_components.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,18 +13,18 @@
 from typing import Iterable, List, Optional, Iterator
 import numpy as np
 from scipy.optimize import fmin_l_bfgs_b
 import logging
 from numpy.random import RandomState
 
 from syne_tune.optimizer.schedulers.searchers.bayesopt.tuning_algorithms.base_classes import (
-    SurrogateModel,
+    Predictor,
     ScoringFunction,
     LocalOptimizer,
-    SurrogateOutputModel,
+    OutputPredictor,
     AcquisitionClassAndArgs,
     unwrap_acquisition_class_and_kwargs,
     CandidateGenerator,
 )
 from syne_tune.optimizer.schedulers.searchers.utils.common import Configuration
 from syne_tune.optimizer.schedulers.searchers.utils.exclusion_list import ExclusionList
 from syne_tune.optimizer.schedulers.searchers.utils.hp_ranges import (
@@ -38,34 +38,37 @@
     """
     Note: This is *not* Thompson sampling, but rather a variant called
     "independent Thompson sampling", where means and variances are drawn
     from the marginal rather than the joint distribution. This is cheap,
     but incorrect. In fact, the larger the number of candidates, the more
     likely the winning configuration is arising from pure chance.
 
-    :param model: Surrogate model for statistics of predictive distribution
+    :param predictor: Surrogate predictor for statistics of predictive distribution
     :param random_state: PRN generator
     """
 
     def __init__(
-        self, model: SurrogateModel, random_state: Optional[RandomState] = None
+        self,
+        predictor: OutputPredictor = None,
+        active_metric: Optional[str] = None,
+        random_state: Optional[RandomState] = None,
     ):
-        self.model = model
+        super().__init__(predictor, active_metric)
         if random_state is None:
             random_state = RandomState(31415629)
         self.random_state = random_state
 
     def score(
         self,
         candidates: Iterable[Configuration],
-        model: Optional[SurrogateModel] = None,
+        predictor: Optional[Predictor] = None,
     ) -> List[float]:
-        if model is None:
-            model = self.model
-        predictions_list = model.predict_candidates(candidates)
+        if predictor is None:
+            predictor = self.predictor
+        predictions_list = predictor.predict_candidates(candidates)
         scores = []
         # If the model supports fantasizing, posterior_means is a matrix. In
         # that case, samples are drawn for every column, then averaged (why
         # we need np.mean)
         for predictions in predictions_list:
             posterior_means = predictions["mean"]
             posterior_stds = predictions["std"]
@@ -77,33 +80,33 @@
         return list(np.mean(np.array(scores), axis=0))
 
 
 class LBFGSOptimizeAcquisition(LocalOptimizer):
     def __init__(
         self,
         hp_ranges: HyperparameterRanges,
-        model: SurrogateOutputModel,
+        predictor: OutputPredictor,
         acquisition_class: AcquisitionClassAndArgs,
         active_metric: str = None,
     ):
-        super().__init__(hp_ranges, model, acquisition_class, active_metric)
+        super().__init__(hp_ranges, predictor, acquisition_class, active_metric)
         # Number criterion evaluations in last recent optimize call
         self.num_evaluations = None
 
     def optimize(
-        self, candidate: Configuration, model: Optional[SurrogateOutputModel] = None
+        self, candidate: Configuration, predictor: Optional[OutputPredictor] = None
     ) -> Configuration:
         # Before local minimization, the model for this state_id should have been fitted.
-        if model is None:
-            model = self.model
+        if predictor is None:
+            predictor = self.predictor
         acquisition_class, acquisition_kwargs = unwrap_acquisition_class_and_kwargs(
             self.acquisition_class
         )
         acquisition_function = acquisition_class(
-            model, self.active_metric, **acquisition_kwargs
+            predictor, self.active_metric, **acquisition_kwargs
         )
 
         x0 = self.hp_ranges.to_ndarray(candidate)
         bounds = self.hp_ranges.get_ndarray_bounds()
         n_evaluations = [0]  # wrapped in list to allow access from function
 
         # unwrap 2d arrays
@@ -134,15 +137,15 @@
             )
             result = self.hp_ranges.from_ndarray(optimized_x.flatten())
             return result
 
 
 class NoOptimization(LocalOptimizer):
     def optimize(
-        self, candidate: Configuration, model: Optional[SurrogateModel] = None
+        self, candidate: Configuration, predictor: Optional[Predictor] = None
     ) -> Configuration:
         return candidate
 
 
 MAX_RETRIES_CANDIDATES_EN_BULK = 20
 MAX_RETRIES_ON_DUPLICATES = 10000
```

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/defaults.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/defaults.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/__init__.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/comparison_gpy.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/comparison_gpy.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,16 +23,16 @@
 from syne_tune.optimizer.schedulers.searchers.utils.common import Configuration
 from syne_tune.optimizer.schedulers.searchers.utils.hp_ranges_factory import (
     make_hyperparameter_ranges,
 )
 from syne_tune.optimizer.schedulers.searchers.bayesopt.datatypes.tuning_job_state import (
     TuningJobState,
 )
-from syne_tune.optimizer.schedulers.searchers.bayesopt.models.gp_model import (
-    get_internal_candidate_evaluations,
+from syne_tune.optimizer.schedulers.searchers.bayesopt.models.estimator import (
+    transform_state_to_data,
 )
 
 
 class ThreeHumpCamel:
     @property
     def search_space(self):
         return [{"min": -5.0, "max": 5.0}, {"min": -5.0, "max": 5.0}]
@@ -141,15 +141,15 @@
 def expand_data(data: Dict[str, Any]) -> Dict[str, Any]:
     """
     Appends derived entries to data dict, which have non-elementary types.
     """
     if "state" not in data:
         data = copy.copy(data)
         state = data_to_state(data)
-        data_internal = get_internal_candidate_evaluations(
+        data_internal = transform_state_to_data(
             state,
             active_metric=INTERNAL_METRIC_NAME,
             normalize_targets=True,
             num_fantasy_samples=20,
         )
         data["state"] = state
         data["train_inputs"] = data_internal.features
```

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/debug_log.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/debug_log.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/test_objects.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/test_objects.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bore/__init__.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bore/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bore/bore.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bore/bore.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bore/de.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bore/de.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bore/gp_classififer.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bore/gp_classififer.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bore/mlp_classififer.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bore/mlp_classififer.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bore/multi_fidelity_bore.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bore/multi_fidelity_bore.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/botorch/__init__.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/botorch/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/botorch/botorch_searcher.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/botorch/botorch_searcher.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/bracket_distribution.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bracket_distribution.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/constrained/__init__.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/constrained/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/constrained/constrained_gp_fifo_searcher.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/constrained/constrained_gp_fifo_searcher.py`

 * *Files 3% similar despite different names*

```diff
@@ -98,19 +98,19 @@
         if self.debug_log is not None:
             logger.info(f"constraint_val = {constr_val}")
 
     def clone_from_state(self, state):
         # Create clone with mutable state taken from 'state'
         init_state = decode_state(state["state"], self._hp_ranges_in_state())
         output_skip_optimization = state["skip_optimization"]
-        output_model_factory = self.state_transformer.model_factory
+        output_estimator = self.state_transformer.estimator
         # Call internal constructor
         new_searcher = ConstrainedGPFIFOSearcher(
             **self._new_searcher_kwargs_for_clone(),
-            output_model_factory=output_model_factory,
+            output_estimator=output_estimator,
             init_state=init_state,
             output_skip_optimization=output_skip_optimization,
             constraint_attr=self._constraint_attr,
         )
         new_searcher._restore_from_state(state)
         # Invalidate self (must not be used afterwards)
         self.state_transformer = None
```

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/cost_aware/__init__.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/dyhpo/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -11,22 +11,14 @@
 # express or implied. See the License for the specific language governing
 # permissions and limitations under the License.
 from syne_tune.try_import import try_import_gpsearchers_message
 
 __all__ = []
 
 try:
-    from syne_tune.optimizer.schedulers.searchers.cost_aware.cost_aware_gp_fifo_searcher import (  # noqa: F401
-        CostAwareGPFIFOSearcher,
-    )
-    from syne_tune.optimizer.schedulers.searchers.cost_aware.cost_aware_gp_multifidelity_searcher import (  # noqa: F401
-        CostAwareGPMultiFidelitySearcher,
+    from syne_tune.optimizer.schedulers.searchers.dyhpo.dyhpo_searcher import (  # noqa: F401
+        DynamicHPOSearcher,
     )
 
-    __all__.extend(
-        [
-            "CostAwareGPFIFOSearcher",
-            "CostAwareGPMultiFidelitySearcher",
-        ]
-    )
+    __all__.append("DynamicHPOSearcher")
 except ImportError:
     print(try_import_gpsearchers_message())
```

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/cost_aware/cost_aware_gp_fifo_searcher.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/cost_aware/cost_aware_gp_fifo_searcher.py`

 * *Files 7% similar despite different names*

```diff
@@ -40,23 +40,23 @@
     call
     :meth:`~syne_tune.optimizer.schedulers.searchers.GPFIFOSearcher._create_internal`
     passing factory and ``skip_optimization`` predicate for the ``INTERNAL_METRIC_NAME``
     model, then replace the state transformer by a multi-model one.
     """
 
     def _call_create_internal(self, kwargs_int):
-        output_model_factory = kwargs_int.pop("output_model_factory")
+        output_estimator = kwargs_int.pop("output_estimator")
         output_skip_optimization = kwargs_int.pop("output_skip_optimization")
-        kwargs_int["model_factory"] = output_model_factory[INTERNAL_METRIC_NAME]
+        kwargs_int["estimator"] = output_estimator[INTERNAL_METRIC_NAME]
         kwargs_int["skip_optimization"] = output_skip_optimization[INTERNAL_METRIC_NAME]
         self._create_internal(**kwargs_int)
         # Replace ``state_transformer``
         init_state = self.state_transformer.state
         self.state_transformer = ModelStateTransformer(
-            model_factory=output_model_factory,
+            estimator=output_estimator,
             init_state=init_state,
             skip_optimization=output_skip_optimization,
         )
 
 
 class CostAwareGPFIFOSearcher(MultiModelGPFIFOSearcher):
     """
@@ -136,19 +136,19 @@
         self._copy_kwargs_to_kwargs_int(kwargs_int, kwargs)
         return kwargs_int
 
     def clone_from_state(self, state):
         # Create clone with mutable state taken from 'state'
         init_state = decode_state(state["state"], self._hp_ranges_in_state())
         output_skip_optimization = state["skip_optimization"]
-        output_model_factory = self.state_transformer.model_factory
+        output_estimator = self.state_transformer.estimator
         # Call internal constructor
         new_searcher = CostAwareGPFIFOSearcher(
             **self._new_searcher_kwargs_for_clone(),
-            output_model_factory=output_model_factory,
+            output_estimator=output_estimator,
             init_state=init_state,
             output_skip_optimization=output_skip_optimization,
         )
         new_searcher._restore_from_state(state)
         # Invalidate self (must not be used afterwards)
         self.state_transformer = None
         return new_searcher
```

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/cost_aware/cost_aware_gp_multifidelity_searcher.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/cost_aware/cost_aware_gp_multifidelity_searcher.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from syne_tune.optimizer.schedulers.searchers.utils.default_arguments import (
     check_and_merge_defaults,
 )
 from syne_tune.optimizer.schedulers.searchers.bayesopt.models.model_transformer import (
     ModelStateTransformer,
 )
 from syne_tune.optimizer.schedulers.searchers.bayesopt.models.cost_fifo_model import (
-    CostSurrogateModelFactory,
+    CostEstimator,
 )
 from syne_tune.optimizer.schedulers.searchers.bayesopt.datatypes.common import (
     INTERNAL_METRIC_NAME,
     INTERNAL_COST_NAME,
 )
 
 logger = logging.getLogger(__name__)
@@ -45,23 +45,23 @@
     We first call
     :meth:`~syne_tune.optimizer.schedulers.searchers.GPMultiFidelitySearcher._create_internal`
     passing factory and ``skip_optimization`` predicate for the ``INTERNAL_METRIC_NAME``
     model, then replace the state transformer by a multi-model one.
     """
 
     def _call_create_internal(self, kwargs_int):
-        output_model_factory = kwargs_int.pop("output_model_factory")
+        output_estimator = kwargs_int.pop("output_estimator")
         output_skip_optimization = kwargs_int.pop("output_skip_optimization")
-        kwargs_int["model_factory"] = output_model_factory[INTERNAL_METRIC_NAME]
+        kwargs_int["estimator"] = output_estimator[INTERNAL_METRIC_NAME]
         kwargs_int["skip_optimization"] = output_skip_optimization[INTERNAL_METRIC_NAME]
         super()._call_create_internal(kwargs_int)
         # Replace ``state_transformer``
         init_state = self.state_transformer.state
         self.state_transformer = ModelStateTransformer(
-            model_factory=output_model_factory,
+            estimator=output_estimator,
             init_state=init_state,
             skip_optimization=output_skip_optimization,
         )
 
 
 class CostAwareGPMultiFidelitySearcher(MultiModelGPMultiFidelitySearcher):
     """
@@ -123,27 +123,27 @@
     def _fix_resource_attribute(self, **kwargs):
         if self.resource_for_acquisition is not None:
             super()._fix_resource_attribute(**kwargs)
             fixed_resource = self.config_space_ext.hp_ranges_ext.value_for_last_pos
         else:
             # Cost at r_max
             fixed_resource = self.config_space_ext.resource_attr_range[1]
-        cost_model_factory = self.state_transformer.model_factory[INTERNAL_COST_NAME]
-        assert isinstance(cost_model_factory, CostSurrogateModelFactory)
-        cost_model_factory.set_fixed_resource(fixed_resource)
+        cost_estimator = self.state_transformer.estimator[INTERNAL_COST_NAME]
+        assert isinstance(cost_estimator, CostEstimator)
+        cost_estimator.set_fixed_resource(fixed_resource)
 
     def clone_from_state(self, state):
         # Create clone with mutable state taken from 'state'
         init_state = decode_state(state["state"], self._hp_ranges_in_state())
         output_skip_optimization = state["skip_optimization"]
-        output_model_factory = self.state_transformer.model_factory
+        output_estimator = self.state_transformer.estimator
         # Call internal constructor
         new_searcher = CostAwareGPMultiFidelitySearcher(
             **self._new_searcher_kwargs_for_clone(),
-            output_model_factory=output_model_factory,
+            output_estimator=output_estimator,
             init_state=init_state,
             output_skip_optimization=output_skip_optimization,
             config_space_ext=self.config_space_ext,
             resource_for_acquisition=self.resource_for_acquisition,
         )
         new_searcher._restore_from_state(state)
         # Invalidate self (must not be used afterwards)
```

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/dyhpo/__init__.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/hypertune/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,14 +11,14 @@
 # express or implied. See the License for the specific language governing
 # permissions and limitations under the License.
 from syne_tune.try_import import try_import_gpsearchers_message
 
 __all__ = []
 
 try:
-    from syne_tune.optimizer.schedulers.searchers.dyhpo.dyhpo_searcher import (  # noqa: F401
-        DynamicHPOSearcher,
+    from syne_tune.optimizer.schedulers.searchers.hypertune.hypertune_searcher import (  # noqa: F401
+        HyperTuneSearcher,
     )
 
-    __all__.append("DynamicHPOSearcher")
+    __all__.append("HyperTuneSearcher")
 except ImportError:
     print(try_import_gpsearchers_message())
```

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/dyhpo/dyhpo_searcher.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/dyhpo/dyhpo_searcher.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 from syne_tune.optimizer.schedulers.searchers.utils.common import (
     Configuration,
 )
 from syne_tune.optimizer.schedulers.searchers.bayesopt.tuning_algorithms.base_classes import (
     CandidateGenerator,
 )
 from syne_tune.optimizer.schedulers.searchers.bayesopt.models.model_base import (
-    BaseSurrogateModel,
+    BasePredictor,
 )
 from syne_tune.optimizer.schedulers.searchers.bayesopt.datatypes.tuning_job_state import (
     TuningJobState,
 )
 
 # DEBUG:
 from syne_tune.optimizer.schedulers.searchers.bayesopt.models.meanstd_acqfunc_impl import (
@@ -122,33 +122,33 @@
         ]
 
     def _scores_for_resource(
         self,
         resource: int,
         start: int,
         end: int,
-        model: BaseSurrogateModel,
+        predictor: BasePredictor,
         sorted_ind: np.ndarray,
         configs_all: List[Dict[str, Any]],
     ) -> (List[float], np.ndarray):
         def my_filter_observed_data(config: Configuration) -> bool:
             return self.config_space_ext.get_resource(config) == resource
 
         # If there is data at level ``resource``, the incumbent in EI
         # should only be computed over this. If there is no data at level
         # ``resource``, the incumbent is computed over all data
-        state = model.state
+        state = predictor.state
         if state.num_observed_cases(resource=resource) > 0:
             filter_observed_data = my_filter_observed_data
         else:
             filter_observed_data = None
-        model.set_filter_observed_data(filter_observed_data)
+        predictor.set_filter_observed_data(filter_observed_data)
         candidates_scorer = create_initial_candidates_scorer(
             initial_scoring="acq_func",
-            model=model,
+            predictor=predictor,
             acquisition_class=self.acquisition_class,
             random_state=self.random_state,
         )
         ind_for_resource = sorted_ind[start:end]
         scores_for_resource = candidates_scorer.score(
             [configs_all[pos] for pos in ind_for_resource]
         )
@@ -211,17 +211,16 @@
         # the incumbent is the best value at the same level, not overall. This
         # is why we compute the score values in chunks for the same :math:`r`
         # value
         if skip_optimization:
             kwargs = dict(skip_optimization=skip_optimization)
         else:
             kwargs = dict()
-        # Note: Asking for the model triggers the posterior computation
-        model = self.state_transformer.model(**kwargs)
-        # Note: ``model.state`` can have fewer observations than
+        predictor = self.state_transformer.fit(**kwargs)
+        # Note: ``predictor.state`` can have fewer observations than
         # ``self.state_transformer.state`` used above, because the former can
         # be filtered down
         resources_all = np.array(resources_all)
         sorted_ind = np.argsort(resources_all)
         resources_all = resources_all[sorted_ind]
         # Find positions where resource value changes
         change_pos = (
@@ -233,15 +232,15 @@
         for start, end in zip(change_pos[:-1], change_pos[1:]):
             resource = resources_all[start]
             assert resources_all[end - 1] == resource
             scores_for_resource, ind_for_resource = self._scores_for_resource(
                 resource=resource,
                 start=start,
                 end=end,
-                model=model,
+                predictor=predictor,
                 sorted_ind=sorted_ind,
                 configs_all=configs_all,
             )
             scores[ind_for_resource] = scores_for_resource
             # DEBUG:
             # _debug_print_info(resource, scores_for_resource, candidates_scorer)
```

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/dyhpo/hyperband_dyhpo.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/dyhpo/hyperband_dyhpo.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/gp_fifo_searcher.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/gp_fifo_searcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -278,19 +278,19 @@
         """
         self._create_internal(**kwargs_int)
 
     def clone_from_state(self, state):
         # Create clone with mutable state taken from 'state'
         init_state = decode_state(state["state"], self._hp_ranges_in_state())
         skip_optimization = state["skip_optimization"]
-        model_factory = self.state_transformer.model_factory
+        estimator = self.state_transformer.estimator
         # Call internal constructor
         new_searcher = GPFIFOSearcher(
             **self._new_searcher_kwargs_for_clone(),
-            model_factory=model_factory,
+            estimator=estimator,
             init_state=init_state,
             skip_optimization=skip_optimization,
         )
         new_searcher._restore_from_state(state)
         # Invalidate self (must not be used afterwards)
         self.state_transformer = None
         return new_searcher
```

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/gp_multifidelity_searcher.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/gp_multifidelity_searcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -266,19 +266,19 @@
         resource = kwargs[self._resource_attr]
         self.state_transformer.remove_observed_case(trial_id, key=str(resource))
 
     def clone_from_state(self, state):
         # Create clone with mutable state taken from 'state'
         init_state = decode_state(state["state"], self._hp_ranges_in_state())
         skip_optimization = state["skip_optimization"]
-        model_factory = self.state_transformer.model_factory
+        estimator = self.state_transformer.estimator
         # Call internal constructor
         new_searcher = GPMultiFidelitySearcher(
             **self._new_searcher_kwargs_for_clone(),
-            model_factory=model_factory,
+            estimator=estimator,
             init_state=init_state,
             skip_optimization=skip_optimization,
             config_space_ext=self.config_space_ext,
             resource_for_acquisition=self.resource_for_acquisition,
         )
         new_searcher._restore_from_state(state)
         # Invalidate self (must not be used afterwards)
```

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/gp_searcher_factory.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/gp_searcher_factory.py`

 * *Files 6% similar despite different names*

```diff
@@ -71,21 +71,21 @@
     BoxCoxTargetTransform,
 )
 from syne_tune.optimizer.schedulers.searchers.bayesopt.models.model_skipopt import (
     SkipNoMaxResourcePredicate,
     SkipPeriodicallyPredicate,
 )
 from syne_tune.optimizer.schedulers.searchers.bayesopt.models.gp_model import (
-    GaussProcEmpiricalBayesModelFactory,
+    GaussProcEmpiricalBayesEstimator,
 )
 from syne_tune.optimizer.schedulers.searchers.bayesopt.models.gpiss_model import (
-    GaussProcAdditiveModelFactory,
+    GaussProcAdditiveEstimator,
 )
 from syne_tune.optimizer.schedulers.searchers.bayesopt.models.cost_fifo_model import (
-    CostSurrogateModelFactory,
+    CostEstimator,
 )
 from syne_tune.optimizer.schedulers.searchers.bayesopt.models.meanstd_acqfunc_impl import (
     EIAcquisitionFunction,
     CEIAcquisitionFunction,
     EIpuAcquisitionFunction,
 )
 from syne_tune.optimizer.schedulers.searchers.bayesopt.tuning_algorithms.defaults import (
@@ -207,34 +207,34 @@
         "target_transform": target_transform,
         "optimization_config": optimization_config,
         "debug_log": debug_log,
         "filter_observed_data": filter_observed_data,
     }
 
 
-def _create_gp_model_factory(
+def _create_gp_estimator(
     gpmodel,
     result: Dict[str, Any],
     hp_ranges_for_prediction: Optional[HyperparameterRanges],
     active_metric: Optional[str],
     **kwargs,
 ):
     filter_observed_data = result["filter_observed_data"]
-    model_factory = GaussProcEmpiricalBayesModelFactory(
+    estimator = GaussProcEmpiricalBayesEstimator(
         active_metric=active_metric,
         gpmodel=gpmodel,
         num_fantasy_samples=kwargs["num_fantasy_samples"],
         normalize_targets=kwargs.get("normalize_targets", True),
         debug_log=result["debug_log"],
         filter_observed_data=filter_observed_data,
         no_fantasizing=kwargs.get("no_fantasizing", False),
         hp_ranges_for_prediction=hp_ranges_for_prediction,
     )
     return {
-        "model_factory": model_factory,
+        "estimator": estimator,
         "filter_observed_data": filter_observed_data,
     }
 
 
 def _create_gp_standard_model(
     hp_ranges: HyperparameterRanges,
     active_metric: Optional[str],
@@ -272,15 +272,15 @@
             hypertune_distribution_args=hypertune_distribution_args,
             **common_kwargs,
         )
         hp_ranges_for_prediction = hp_ranges
     else:
         gpmodel = GaussianProcessRegression(**common_kwargs)
         hp_ranges_for_prediction = None
-    return _create_gp_model_factory(
+    return _create_gp_estimator(
         gpmodel=gpmodel,
         result=result,
         hp_ranges_for_prediction=hp_ranges_for_prediction,
         active_metric=active_metric,
         **kwargs,
     )
 
@@ -317,15 +317,15 @@
             hypertune_distribution_args=hypertune_distribution_args,
             **common_kwargs,
         )
         hp_ranges_for_prediction = hp_ranges
     else:
         gpmodel = IndependentGPPerResourceModel(**common_kwargs)
         hp_ranges_for_prediction = None
-    return _create_gp_model_factory(
+    return _create_gp_estimator(
         gpmodel=gpmodel,
         result=result,
         hp_ranges_for_prediction=hp_ranges_for_prediction,
         active_metric=active_metric,
         **kwargs,
     )
 
@@ -357,25 +357,25 @@
         optimization_config=result["optimization_config"],
         random_seed=random_seed,
         fit_reset_params=not result["opt_warmstart"],
     )
     filter_observed_data = result["filter_observed_data"]
     no_fantasizing = kwargs.get("no_fantasizing", False)
     num_fantasy_samples = 0 if no_fantasizing else kwargs["num_fantasy_samples"]
-    model_factory = GaussProcAdditiveModelFactory(
+    estimator = GaussProcAdditiveEstimator(
         gpmodel=gpmodel,
         num_fantasy_samples=num_fantasy_samples,
         active_metric=active_metric,
         config_space_ext=config_space_ext,
         debug_log=result["debug_log"],
         filter_observed_data=filter_observed_data,
         normalize_targets=kwargs.get("normalize_targets", True),
     )
     return {
-        "model_factory": model_factory,
+        "estimator": estimator,
         "filter_observed_data": filter_observed_data,
     }
 
 
 def _create_state_converter(
     model: str,
     is_hyperband: bool,
@@ -652,43 +652,43 @@
     assert (
         kwargs["scheduler"] == "fifo"
     ), "This factory needs scheduler = 'fifo' (instead of '{}')".format(
         kwargs["scheduler"]
     )
     # Common objects
     result = _create_common_objects(**kwargs)
-    model_factory = result.pop("model_factory")
+    estimator = result.pop("estimator")
     skip_optimization = result.pop("skip_optimization")
-    # We need two model factories: one for active metric (model_factory),
-    # the other for constraint metric (model_factory_constraint)
+    # We need two model factories: one for active metric (estimator),
+    # the other for constraint metric (estimator_constraint)
     random_seed, _kwargs = extract_random_seed(**kwargs)
-    model_factory_constraint = _create_gp_standard_model(
+    estimator_constraint = _create_gp_standard_model(
         hp_ranges=result["hp_ranges"],
         active_metric=INTERNAL_CONSTRAINT_NAME,
         random_seed=random_seed,
         is_hyperband=False,
         **_kwargs,
-    )["model_factory"]
+    )["estimator"]
     # Sharing debug_log attribute across models
-    model_factory_constraint._debug_log = model_factory._debug_log
+    estimator_constraint._debug_log = estimator._debug_log
     # The same skip_optimization strategy applies to both models
     skip_optimization_constraint = skip_optimization
 
-    output_model_factory = {
-        INTERNAL_METRIC_NAME: model_factory,
-        INTERNAL_CONSTRAINT_NAME: model_factory_constraint,
+    output_estimator = {
+        INTERNAL_METRIC_NAME: estimator,
+        INTERNAL_CONSTRAINT_NAME: estimator_constraint,
     }
     output_skip_optimization = {
         INTERNAL_METRIC_NAME: skip_optimization,
         INTERNAL_CONSTRAINT_NAME: skip_optimization_constraint,
     }
 
     return dict(
         result,
-        output_model_factory=output_model_factory,
+        output_estimator=output_estimator,
         output_skip_optimization=output_skip_optimization,
         acquisition_class=CEIAcquisitionFunction,
     )
 
 
 def cost_aware_coarse_gp_fifo_searcher_factory(**kwargs) -> Dict[str, Any]:
     """
@@ -706,45 +706,45 @@
     assert (
         kwargs["scheduler"] == "fifo"
     ), "This factory needs scheduler = 'fifo' (instead of '{}')".format(
         kwargs["scheduler"]
     )
     # Common objects
     result = _create_common_objects(**kwargs)
-    model_factory = result.pop("model_factory")
+    estimator = result.pop("estimator")
     skip_optimization = result.pop("skip_optimization")
-    # We need two model factories: one for active metric (model_factory),
-    # the other for cost metric (model_factory_cost)
+    # We need two model factories: one for active metric (estimator),
+    # the other for cost metric (estimator_cost)
     random_seed, _kwargs = extract_random_seed(**kwargs)
-    model_factory_cost = _create_gp_standard_model(
+    estimator_cost = _create_gp_standard_model(
         hp_ranges=result["hp_ranges"],
         active_metric=INTERNAL_COST_NAME,
         random_seed=random_seed,
         is_hyperband=False,
         **_kwargs,
-    )["model_factory"]
+    )["estimator"]
     # Sharing debug_log attribute across models
-    model_factory_cost._debug_log = model_factory._debug_log
+    estimator_cost._debug_log = estimator._debug_log
     exponent_cost = kwargs.get("exponent_cost", 1.0)
     acquisition_class = (EIpuAcquisitionFunction, dict(exponent_cost=exponent_cost))
     # The same skip_optimization strategy applies to both models
     skip_optimization_cost = skip_optimization
 
-    output_model_factory = {
-        INTERNAL_METRIC_NAME: model_factory,
-        INTERNAL_COST_NAME: model_factory_cost,
+    output_estimator = {
+        INTERNAL_METRIC_NAME: estimator,
+        INTERNAL_COST_NAME: estimator_cost,
     }
     output_skip_optimization = {
         INTERNAL_METRIC_NAME: skip_optimization,
         INTERNAL_COST_NAME: skip_optimization_cost,
     }
 
     return dict(
         result,
-        output_model_factory=output_model_factory,
+        output_estimator=output_estimator,
         output_skip_optimization=output_skip_optimization,
         acquisition_class=acquisition_class,
     )
 
 
 def cost_aware_fine_gp_fifo_searcher_factory(**kwargs) -> Dict[str, Any]:
     """
@@ -776,38 +776,38 @@
         "If search_options['resource_attr'] is given, the maximum "
         + "resource level has to be specified in "
         + "search_options['max_epochs'], or (simpler) as max_t when "
         + "creating FIFOScheduler"
     )
     # Common objects
     result = _create_common_objects(**kwargs)
-    model_factory = result.pop("model_factory")
+    estimator = result.pop("estimator")
     skip_optimization = result.pop("skip_optimization")
-    # We need two model factories: one for active metric (model_factory),
-    # the other for cost metric (model_factory_cost)
-    model_factory_cost = CostSurrogateModelFactory(
+    # We need two model factories: one for active metric (estimator),
+    # the other for cost metric (estimator_cost)
+    estimator_cost = CostEstimator(
         model=kwargs["cost_model"], fixed_resource=fixed_resource, num_samples=1
     )
     exponent_cost = kwargs.get("exponent_cost", 1.0)
     acquisition_class = (EIpuAcquisitionFunction, dict(exponent_cost=exponent_cost))
     # The same skip_optimization strategy applies to both models
     skip_optimization_cost = skip_optimization
 
-    output_model_factory = {
-        INTERNAL_METRIC_NAME: model_factory,
-        INTERNAL_COST_NAME: model_factory_cost,
+    output_estimator = {
+        INTERNAL_METRIC_NAME: estimator,
+        INTERNAL_COST_NAME: estimator_cost,
     }
     output_skip_optimization = {
         INTERNAL_METRIC_NAME: skip_optimization,
         INTERNAL_COST_NAME: skip_optimization_cost,
     }
 
     return dict(
         result,
-        output_model_factory=output_model_factory,
+        output_estimator=output_estimator,
         output_skip_optimization=output_skip_optimization,
         acquisition_class=acquisition_class,
         resource_attr=kwargs["resource_attr"],
     )
 
 
 def cost_aware_gp_multifidelity_searcher_factory(**kwargs) -> Dict[str, Any]:
@@ -834,42 +834,42 @@
     cost_model = kwargs.get("cost_model")
     assert cost_model is not None, (
         "If search_options['resource_attr'] is given, a CostModel has "
         + "to be specified in search_options['cost_model']"
     )
     # Common objects
     result = _create_common_objects(**kwargs)
-    model_factory = result.pop("model_factory")
+    estimator = result.pop("estimator")
     skip_optimization = result.pop("skip_optimization")
-    # We need two model factories: one for active metric (model_factory),
-    # the other for cost metric (model_factory_cost)
-    model_factory_cost = CostSurrogateModelFactory(
+    # We need two model factories: one for active metric (estimator),
+    # the other for cost metric (estimator_cost)
+    estimator_cost = CostEstimator(
         model=kwargs["cost_model"], fixed_resource=kwargs["max_epochs"], num_samples=1
     )
     exponent_cost = kwargs.get("exponent_cost", 1.0)
     acquisition_class = (EIpuAcquisitionFunction, dict(exponent_cost=exponent_cost))
     # The same skip_optimization strategy applies to both models
     skip_optimization_cost = skip_optimization
 
-    output_model_factory = {
-        INTERNAL_METRIC_NAME: model_factory,
-        INTERNAL_COST_NAME: model_factory_cost,
+    output_estimator = {
+        INTERNAL_METRIC_NAME: estimator,
+        INTERNAL_COST_NAME: estimator_cost,
     }
     output_skip_optimization = {
         INTERNAL_METRIC_NAME: skip_optimization,
         INTERNAL_COST_NAME: skip_optimization_cost,
     }
 
     resource_for_acquisition = resource_for_acquisition_factory(
         kwargs, result["hp_ranges"]
     )
     return dict(
         result,
         resource_attr=kwargs["resource_attr"],
-        output_model_factory=output_model_factory,
+        output_estimator=output_estimator,
         output_skip_optimization=output_skip_optimization,
         resource_for_acquisition=resource_for_acquisition,
         acquisition_class=acquisition_class,
     )
 
 
 def _common_defaults(
```

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/gp_searcher_utils.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/gp_searcher_utils.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/hypertune/__init__.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/kde/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,19 +6,27 @@
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # or in the "license" file accompanying this file. This file is distributed
 # on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either
 # express or implied. See the License for the specific language governing
 # permissions and limitations under the License.
-from syne_tune.try_import import try_import_gpsearchers_message
+from syne_tune.try_import import try_import_kde_message
 
 __all__ = []
 
 try:
-    from syne_tune.optimizer.schedulers.searchers.hypertune.hypertune_searcher import (  # noqa: F401
-        HyperTuneSearcher,
+    from syne_tune.optimizer.schedulers.searchers.kde.kde_searcher import (  # noqa: F401
+        KernelDensityEstimator,
+    )
+    from syne_tune.optimizer.schedulers.searchers.kde.multi_fidelity_kde_searcher import (  # noqa: F401
+        MultiFidelityKernelDensityEstimator,
     )
 
-    __all__.append("HyperTuneSearcher")
+    __all__.extend(
+        [
+            "KernelDensityEstimator",
+            "MultiFidelityKernelDensityEstimator",
+        ]
+    )
 except ImportError:
-    print(try_import_gpsearchers_message())
+    print(try_import_kde_message())
```

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/hypertune/hypertune_bracket_distribution.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/hypertune/hypertune_bracket_distribution.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # or in the "license" file accompanying this file. This file is distributed
 # on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either
 # express or implied. See the License for the specific language governing
 import numpy as np
 import logging
 
 from syne_tune.optimizer.schedulers.searchers.bayesopt.models.gp_model import (
-    GaussProcModelFactory,
+    GaussProcEstimator,
 )
 from syne_tune.optimizer.schedulers.searchers.bayesopt.gpautograd.hypertune.gp_model import (
     HyperTuneIndependentGPModel,
     HyperTuneJointGPModel,
 )
 from syne_tune.optimizer.schedulers.searchers.bracket_distribution import (
     DefaultHyperbandBracketDistribution,
@@ -52,22 +52,22 @@
             + "SynchronousHyperbandScheduler scheduler"
         )
         self._searcher = scheduler.searcher
         assert isinstance(self._searcher, GPMultiFidelitySearcher)
 
     def __call__(self) -> np.ndarray:
         distribution = super().__call__()
-        model_factory = self._searcher.state_transformer.model_factory
+        estimator = self._searcher.state_transformer.estimator
         err_msg = (
-            "Hyper-Tune requires GaussProcModelFactory model factory with "
+            "Hyper-Tune requires GaussProcEstimator estimator with "
             "HyperTuneIndependentGPModel or HyperTuneJointGPModel model. Use "
             "searcher = 'hypertune'"
         )
-        assert isinstance(model_factory, GaussProcModelFactory), err_msg
-        gpmodel = model_factory.gpmodel
+        assert isinstance(estimator, GaussProcEstimator), err_msg
+        gpmodel = estimator.gpmodel
         assert isinstance(
             gpmodel, (HyperTuneIndependentGPModel, HyperTuneJointGPModel)
         ), err_msg
         ht_distribution = gpmodel.hypertune_bracket_distribution()
         if ht_distribution is not None:
             # The Hyper-Tune distribution may not be over all brackets.
             # In that case, we keep the tail of the default distribution
```

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/hypertune/hypertune_searcher.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/hypertune/hypertune_searcher.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/kde/kde_searcher.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/kde/kde_searcher.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/kde/multi_fidelity_kde_searcher.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/kde/multi_fidelity_kde_searcher.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/model_based_searcher.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/model_based_searcher.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,23 +31,25 @@
     TuningJobState,
 )
 from syne_tune.optimizer.schedulers.searchers.bayesopt.models.model_skipopt import (
     SkipOptimizationPredicate,
     AlwaysSkipPredicate,
 )
 from syne_tune.optimizer.schedulers.searchers.bayesopt.models.model_transformer import (
-    TransformerOutputModelFactory,
     ModelStateTransformer,
     StateForModelConverter,
 )
+from syne_tune.optimizer.schedulers.searchers.bayesopt.models.estimator import (
+    OutputEstimator,
+)
 from syne_tune.optimizer.schedulers.searchers.bayesopt.tuning_algorithms.base_classes import (
     AcquisitionClassAndArgs,
     LocalOptimizer,
     ScoringFunction,
-    SurrogateOutputModel,
+    OutputPredictor,
     unwrap_acquisition_class_and_kwargs,
     CandidateGenerator,
 )
 from syne_tune.optimizer.schedulers.searchers.bayesopt.tuning_algorithms.bo_algorithm import (
     BayesianOptimizationAlgorithm,
 )
 from syne_tune.optimizer.schedulers.searchers.bayesopt.tuning_algorithms.bo_algorithm_components import (
@@ -110,15 +112,15 @@
     Note that this works because :attr:`random_state` is only used in the internal
     random searcher until meth:`_get_config_modelbased` is first called.
     """
 
     def _create_internal(
         self,
         hp_ranges: HyperparameterRanges,
-        model_factory: TransformerOutputModelFactory,
+        estimator: OutputEstimator,
         acquisition_class: AcquisitionClassAndArgs,
         map_reward: Optional[MapReward] = None,
         init_state: TuningJobState = None,
         local_minimizer_class: Type[LocalOptimizer] = None,
         skip_optimization: SkipOptimizationPredicate = None,
         num_initial_candidates: int = DEFAULT_NUM_INITIAL_CANDIDATES,
         num_initial_random_choices: int = DEFAULT_NUM_INITIAL_RANDOM_EVALUATIONS,
@@ -150,31 +152,31 @@
         else:
             self.local_minimizer_class = (
                 DEFAULT_LOCAL_OPTIMIZER_CLASS
                 if local_minimizer_class is None
                 else local_minimizer_class
             )
         self.acquisition_class = acquisition_class
-        if isinstance(model_factory, dict):
-            model_factory_main = model_factory[INTERNAL_METRIC_NAME]
+        if isinstance(estimator, dict):
+            estimator_main = estimator[INTERNAL_METRIC_NAME]
         else:
-            model_factory_main = model_factory
-        self._debug_log = model_factory_main.debug_log
+            estimator_main = estimator
+        self._debug_log = estimator_main.debug_log
         self.initial_scoring = check_initial_candidates_scorer(initial_scoring)
         self.skip_local_optimization = skip_local_optimization
         # Create state transformer
         # Initial state is empty (note that the state is mutable).
         # If there is a state converter, it uses the same random state as the searcher
         # here
         if state_converter is not None:
             state_converter.set_random_state(self.random_state)
         if init_state is None:
             init_state = TuningJobState.empty_state(self._hp_ranges_in_state())
         self.state_transformer = ModelStateTransformer(
-            model_factory=model_factory,
+            estimator=estimator,
             init_state=init_state,
             skip_optimization=skip_optimization,
             state_converter=state_converter,
         )
         self._cost_attr = cost_attr
         self._resource_attr = resource_attr
         self._filter_observed_data = filter_observed_data
@@ -479,30 +481,30 @@
                 restrict_configurations=self._restrict_configurations,
             )
             self._random_searcher.set_random_state(self.random_state)
 
 
 def create_initial_candidates_scorer(
     initial_scoring: str,
-    model: SurrogateOutputModel,
+    predictor: OutputPredictor,
     acquisition_class: AcquisitionClassAndArgs,
     random_state: np.random.RandomState,
     active_metric: str = INTERNAL_METRIC_NAME,
 ) -> ScoringFunction:
     if initial_scoring == "thompson_indep":
-        if isinstance(model, dict):
-            assert active_metric in model
-            model = model[active_metric]
-        return IndependentThompsonSampling(model, random_state=random_state)
+        if isinstance(predictor, dict):
+            assert active_metric in predictor
+            predictor = predictor[active_metric]
+        return IndependentThompsonSampling(predictor, random_state=random_state)
     else:
         acquisition_class, acquisition_kwargs = unwrap_acquisition_class_and_kwargs(
             acquisition_class
         )
         return acquisition_class(
-            model, active_metric=active_metric, **acquisition_kwargs
+            predictor, active_metric=active_metric, **acquisition_kwargs
         )
 
 
 class BayesianOptimizationSearcher(ModelBasedSearcher):
     """Common Code for searchers using Bayesian optimization
 
     We implement Bayesian optimization, based on a model factory which
@@ -531,22 +533,22 @@
             TrialSchedulerWithSearcher,
         )
 
         assert isinstance(
             scheduler, TrialSchedulerWithSearcher
         ), "This searcher requires TrialSchedulerWithSearcher scheduler"
         super().configure_scheduler(scheduler)
-        # Allow model factory to depend on ``scheduler`` as well
-        model_factory = self.state_transformer.model_factory
-        if isinstance(model_factory, dict):
-            model_factories = list(model_factory.values())
+        # Allow estimator(s) to depend on ``scheduler`` as well
+        estimator = self.state_transformer.estimator
+        if isinstance(estimator, dict):
+            estimators = list(estimator.values())
         else:
-            model_factories = [model_factory]
-        for model_factory in model_factories:
-            model_factory.configure_scheduler(scheduler)
+            estimators = [estimator]
+        for estimator in estimators:
+            estimator.configure_scheduler(scheduler)
 
     def register_pending(
         self, trial_id: str, config: Optional[Dict[str, Any]] = None, milestone=None
     ):
         """
         Registers trial as pending. This means the corresponding evaluation
         task is running. Once it finishes, update is called for this trial.
@@ -613,31 +615,30 @@
                 for pos, config in enumerate(self._restrict_configurations)
                 if pos not in remove_pos
             ]
 
     def _get_config_modelbased(
         self, exclusion_candidates, **kwargs
     ) -> Optional[Configuration]:
-        # Obtain current :class:`SurrogateModel` from state transformer. Based on
+        # Obtain current :class:`Predictor` from state transformer. Based on
         # this, the BO algorithm components can be constructed
-        # Note: Asking for the model triggers the posterior computation
-        model = self.state_transformer.model()
+        predictor = self.state_transformer.fit()
         # Select and fix target resource attribute (relevant in subclasses)
         self._fix_resource_attribute(**kwargs)
         # Create BO algorithm
         random_generator = self._create_random_generator()
         initial_candidates_scorer = create_initial_candidates_scorer(
             initial_scoring=self.initial_scoring,
-            model=model,
+            predictor=predictor,
             acquisition_class=self.acquisition_class,
             random_state=self.random_state,
         )
         local_optimizer = self.local_minimizer_class(
             hp_ranges=self._hp_ranges_for_prediction(),
-            model=model,
+            predictor=predictor,
             acquisition_class=self.acquisition_class,
             active_metric=INTERNAL_METRIC_NAME,
         )
         bo_algorithm = BayesianOptimizationAlgorithm(
             initial_candidates_generator=random_generator,
             initial_candidates_scorer=initial_candidates_scorer,
             num_initial_candidates=self.num_initial_candidates,
@@ -715,42 +716,42 @@
                         # duplicates in the same batch
                         exclusion_candidates.add(config)
                     else:
                         break  # Space exhausted
             if not pick_random:
                 # Model-based decision for remaining ones
                 num_requested_candidates = batch_size - len(configs)
-                model = self.state_transformer.model()
+                predictor = self.state_transformer.fit()
                 # Select and fix target resource attribute (relevant in subclasses)
                 self._fix_resource_attribute(**kwargs)
                 # Create BO algorithm
                 random_generator = self._create_random_generator()
                 initial_candidates_scorer = create_initial_candidates_scorer(
                     initial_scoring=self.initial_scoring,
-                    model=model,
+                    predictor=predictor,
                     acquisition_class=self.acquisition_class,
                     random_state=self.random_state,
                 )
                 local_optimizer = self.local_minimizer_class(
                     hp_ranges=self._hp_ranges_for_prediction(),
-                    model=model,
+                    predictor=predictor,
                     acquisition_class=self.acquisition_class,
                     active_metric=INTERNAL_METRIC_NAME,
                 )
                 pending_candidate_state_transformer = None
                 if num_requested_candidates > 1:
                     # Internally, if num_requested_candidates > 1, the candidates are
                     # selected greedily. This needs model updates after each greedy
                     # selection, because of one more pending evaluation.
                     # We need a copy of the state here, since
                     # ``pending_candidate_state_transformer`` modifies the state (it
                     # appends pending trials)
                     temporary_state = copy.deepcopy(self.state_transformer.state)
                     pending_candidate_state_transformer = ModelStateTransformer(
-                        model_factory=self.state_transformer.model_factory,
+                        estimator=self.state_transformer.estimator,
                         init_state=temporary_state,
                         skip_optimization=AlwaysSkipPredicate(),
                     )
                 bo_algorithm = BayesianOptimizationAlgorithm(
                     initial_candidates_generator=random_generator,
                     initial_candidates_scorer=initial_candidates_scorer,
                     num_initial_candidates=self.num_initial_candidates,
@@ -780,15 +781,15 @@
         # Mark config as failed (which means it will be blacklisted in
         # future get_config calls)
         self.state_transformer.mark_trial_failed(trial_id)
 
     def _new_searcher_kwargs_for_clone(self) -> Dict[str, Any]:
         """
         Helper method for ``clone_from_state``. Args need to be extended
-        by ``model_factory``, ``init_state``, ``skip_optimization``, and others
+        by ``estimator``, ``init_state``, ``skip_optimization``, and others
         args becoming relevant in subclasses only.
 
         :return: kwargs for creating new searcher object in ``clone_from_state``
         """
         return dict(
             config_space=self.config_space,
             metric=self._metric,
```

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/random_grid_searcher.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/random_grid_searcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,15 +74,17 @@
         # Debug log printing (switched off by default)
         if isinstance(debug_log, bool):
             if debug_log:
                 self._debug_log = DebugLogPrinter()
             else:
                 self._debug_log = None
         else:
-            assert isinstance(debug_log, DebugLogPrinter)
+            assert isinstance(
+                debug_log, DebugLogPrinter
+            ), f"debug_log = {debug_log} must either be bool or DebugLogPrinter"
             self._debug_log = debug_log
 
     def configure_scheduler(self, scheduler):
         from syne_tune.optimizer.schedulers.multi_fidelity import (
             MultiFidelitySchedulerMixin,
         )
```

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/regularized_evolution.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/regularized_evolution.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import logging
 
 from collections import deque
 from typing import Optional, List, Dict, Any
 from dataclasses import dataclass
 
 from syne_tune.optimizer.schedulers.searchers import StochasticSearcher
-from syne_tune.config_space import Domain
+from syne_tune.config_space import config_space_size, Domain
 from syne_tune.optimizer.schedulers.searchers.utils import make_hyperparameter_ranges
 from syne_tune.optimizer.schedulers.searchers.searcher_base import (
     sample_random_configuration,
 )
 
 logger = logging.getLogger(__name__)
 
@@ -67,55 +67,58 @@
         population_size: int = 100,
         sample_size: int = 10,
         **kwargs,
     ):
         super(RegularizedEvolution, self).__init__(
             config_space, metric, points_to_evaluate=points_to_evaluate, **kwargs
         )
+        assert (
+            config_space_size(config_space) != 1
+        ), "config_space has size 1, does not offer any diversity"
         self.mode = mode
         self.population_size = population_size
         self.sample_size = sample_size
         self.population = deque()
         self.num_sample_try = 1000  # number of times allowed to sample a mutation
         self._hp_ranges = make_hyperparameter_ranges(self.config_space)
         allow_duplicates = kwargs.get("allow_duplicates")
         if allow_duplicates is not None and (not allow_duplicates):
             logger.warning(
                 "This class does not support allow_duplicates argument. Sampling is with replacement"
             )
         if kwargs.get("restrict_configurations") is not None:
             logger.warning("This class does not support restrict_configurations")
+        self._non_constant_hps = [
+            name
+            for name, domain in config_space.items()
+            if isinstance(domain, Domain) and len(domain) != 1
+        ]
 
     def _mutate_config(self, config: Dict[str, Any]) -> Dict[str, Any]:
         child_config = copy.deepcopy(config)
-
-        # sample mutation until a different configuration is found
-        for sample_try in range(self.num_sample_try):
-            if child_config == config:
-                # sample a random hyperparameter to mutate
-                hps = [
-                    (k, v)
-                    for k, v in self.config_space.items()
-                    if isinstance(v, Domain) and len(v) > 1
-                ]
-                assert (
-                    len(hps) >= 0
-                ), "all hyperparameters only have a single value, cannot perform mutations."
-                hp_name, hp = hps[self.random_state.randint(len(hps))]
-
-                # mutate the value by sampling
-                child_config[hp_name] = hp.sample(random_state=self.random_state)
+        config_ms = self._hp_ranges.config_to_match_string(config)
+        # Sample mutation until a different configuration is found
+        config_is_mutated = False
+        for _ in range(self.num_sample_try):
+            if self._hp_ranges.config_to_match_string(child_config) == config_ms:
+                # Sample a random hyperparameter to mutate
+                hp_name = self.random_state.choice(self._non_constant_hps, 1).item()
+                # Mutate the value by sampling
+                child_config[hp_name] = self.config_space[hp_name].sample(
+                    random_state=self.random_state
+                )
             else:
+                config_is_mutated = True
                 break
-        if sample_try == self.num_sample_try:
+        if not config_is_mutated:
             logger.info(
-                f"Did not manage to sample a different configuration with {self.num_sample_try}, "
-                f"sampling at random"
+                "Did not manage to sample a different configuration with "
+                f"{self.num_sample_try}, sampling at random"
             )
-            return self._sample_random_config()
+            child_config = self._sample_random_config()
 
         return child_config
 
     def _sample_random_config(self) -> Dict[str, Any]:
         return sample_random_configuration(self._hp_ranges, self.random_state)
 
     def get_config(self, **kwargs) -> Optional[dict]:
```

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/searcher.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/searcher.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/searcher_base.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/searcher_base.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/searcher_callback.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/searcher_callback.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/searcher_factory.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/searcher_factory.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/utils/__init__.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/utils/common.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/utils/common.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/utils/default_arguments.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/utils/default_arguments.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/utils/exclusion_list.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/utils/exclusion_list.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/utils/hp_ranges.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/utils/hp_ranges.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/utils/hp_ranges_factory.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/utils/hp_ranges_factory.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/utils/hp_ranges_impl.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/utils/hp_ranges_impl.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/utils/scaling.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/utils/scaling.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/searchers/utils/warmstarting.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/utils/warmstarting.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/synchronous/__init__.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/synchronous/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/synchronous/dehb.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/synchronous/dehb.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/synchronous/dehb_bracket.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/synchronous/dehb_bracket.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/synchronous/dehb_bracket_manager.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/synchronous/dehb_bracket_manager.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/synchronous/hyperband.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/synchronous/hyperband.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/synchronous/hyperband_bracket.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/synchronous/hyperband_bracket.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/synchronous/hyperband_bracket_manager.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/synchronous/hyperband_bracket_manager.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/synchronous/hyperband_impl.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/synchronous/hyperband_impl.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/synchronous/hyperband_rung_system.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/synchronous/hyperband_rung_system.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/transfer_learning/__init__.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/transfer_learning/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/transfer_learning/bounding_box.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/transfer_learning/bounding_box.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/transfer_learning/quantile_based/__init__.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/transfer_learning/quantile_based/normalization_transforms.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/transfer_learning/quantile_based/normalization_transforms.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/transfer_learning/quantile_based/quantile_based_searcher.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/transfer_learning/quantile_based/quantile_based_searcher.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/transfer_learning/rush.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/transfer_learning/rush.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/transfer_learning/zero_shot.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/transfer_learning/zero_shot.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/utils/__init__.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/transfer_learning/quantile_based/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/utils/simple_profiler.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/utils/simple_profiler.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/optimizer/schedulers/utils/successive_halving.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/utils/successive_halving.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/remote/__init__.py` & `syne_tune-0.7.0/syne_tune/optimizer/schedulers/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/remote/estimators.py` & `syne_tune-0.7.0/syne_tune/remote/estimators.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/remote/remote_launcher.py` & `syne_tune-0.7.0/syne_tune/remote/remote_launcher.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/remote/remote_main.py` & `syne_tune-0.7.0/syne_tune/remote/remote_main.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/remote/remote_metrics_callback.py` & `syne_tune-0.7.0/syne_tune/remote/remote_metrics_callback.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/report.py` & `syne_tune-0.7.0/syne_tune/report.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/results_callback.py` & `syne_tune-0.7.0/syne_tune/results_callback.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/stopping_criterion.py` & `syne_tune-0.7.0/syne_tune/stopping_criterion.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/try_import.py` & `syne_tune-0.7.0/syne_tune/try_import.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/tuner.py` & `syne_tune-0.7.0/syne_tune/tuner.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/tuner_callback.py` & `syne_tune-0.7.0/syne_tune/tuner_callback.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/tuning_status.py` & `syne_tune-0.7.0/syne_tune/tuning_status.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/util.py` & `syne_tune-0.7.0/syne_tune/util.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/utils/__init__.py` & `syne_tune-0.7.0/syne_tune/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/utils/checkpoint.py` & `syne_tune-0.7.0/syne_tune/utils/checkpoint.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/utils/config_as_json.py` & `syne_tune-0.7.0/syne_tune/utils/config_as_json.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune/utils/parse_bool.py` & `syne_tune-0.7.0/syne_tune/utils/parse_bool.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.6.0/syne_tune.egg-info/PKG-INFO` & `syne_tune-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 Metadata-Version: 2.1
-Name: syne-tune
-Version: 0.6.0
+Name: syne_tune
+Version: 0.7.0
 Summary: Distributed Hyperparameter Optimization on SageMaker
 Author: AWS
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
-Provides-Extra: raytune
-Provides-Extra: bore
-Provides-Extra: kde
 Provides-Extra: gpsearchers
-Provides-Extra: benchmarks
-Provides-Extra: blackbox-repository
-Provides-Extra: aws
-Provides-Extra: yahpo
+Provides-Extra: kde
 Provides-Extra: dev
+Provides-Extra: aws
 Provides-Extra: moo
+Provides-Extra: visual
+Provides-Extra: blackbox-repository
+Provides-Extra: benchmarks
+Provides-Extra: yahpo
+Provides-Extra: raytune
+Provides-Extra: botorch
+Provides-Extra: bore
 Provides-Extra: extra
 License-File: LICENSE
 License-File: NOTICE
 
 # Syne Tune: Large-Scale and Reproducible Hyperparameter Optimization
 
 [![release](https://img.shields.io/github/v/release/awslabs/syne-tune)](https://pypi.org/project/syne-tune/)
@@ -86,20 +88,20 @@
 from syne_tune import Reporter
 from argparse import ArgumentParser
 
 if __name__ == '__main__':
     root = logging.getLogger()
     root.setLevel(logging.INFO)
     parser = ArgumentParser()
-    parser.add_argument('--steps', type=int)
+    parser.add_argument('--epochs', type=int)
     parser.add_argument('--width', type=float)
     parser.add_argument('--height', type=float)
     args, _ = parser.parse_known_args()
     report = Reporter()
-    for step in range(args.steps):
+    for step in range(args.epochs):
         time.sleep(0.1)
         dummy_score = 1.0 / (0.1 + args.width * step / 100) + args.height * 0.1
         # Feed the score back to Syne Tune.
         report(epoch=step + 1, mean_loss=dummy_score)
 ```
 
 Once you have a script reporting metric, you can launch a tuning as-follow:
@@ -115,15 +117,15 @@
 config_space = {
     'width': randint(1, 20),
     'height': randint(1, 20),
     'epochs': 100,
 }
 
 tuner = Tuner(
-    trial_backend=LocalBackend(entry_point='train_height.py'),
+    trial_backend=LocalBackend(entry_point='train_height_simple.py'),
     scheduler=ASHA(
         config_space,
         metric='mean_loss',
         resource_attr='epoch',
         max_resource_attr="epochs",
         search_options={'debug_log': False},
     ),
@@ -171,14 +173,15 @@
 
 ## Supported multi-objective optimization methods
 
 Method | Reference | Searcher | Asynchronous? | Multi-fidelity? | Transfer?
 :--- | :---: | :---: | :---: | :---: | :---: 
 Constrained Bayesian Optimization | Gardner, et al. (2014) | model-based | yes | no | no
 MOASHA | Schmucker, et al. (2021) | random | yes | yes | no
+NSGA-2 | Deb, et al. (2002) | evolutionary | no | no | no
 
 HPO methods listed can be used in a multi-objective setting by scalarization or non-dominated sorting. See [multiobjective_priority.py](syne_tune/optimizers/schedulers/multiobjective/multiobjective_priority.py) for details.
 
 ## Examples
 
 You will find many examples in the [examples/](examples/) folder illustrating
 different functionalities provided by Syne Tune. For example:
```

### Comparing `syne_tune-0.6.0/syne_tune.egg-info/SOURCES.txt` & `syne_tune-0.7.0/syne_tune.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,18 @@
 syne_tune/blackbox_repository/conversion_scripts/scripts/lcbench/lcbench.py
 syne_tune/callbacks/__init__.py
 syne_tune/callbacks/hyperband_remove_checkpoints_callback.py
 syne_tune/callbacks/hyperband_remove_checkpoints_score.py
 syne_tune/callbacks/remove_checkpoints_callback.py
 syne_tune/callbacks/tensorboard_callback.py
 syne_tune/experiments/__init__.py
+syne_tune/experiments/aggregate_results.py
 syne_tune/experiments/experiment_result.py
+syne_tune/experiments/plot_per_trial.py
+syne_tune/experiments/plotting.py
 syne_tune/experiments/results_utils.py
 syne_tune/optimizer/__init__.py
 syne_tune/optimizer/baselines.py
 syne_tune/optimizer/scheduler.py
 syne_tune/optimizer/schedulers/__init__.py
 syne_tune/optimizer/schedulers/fifo.py
 syne_tune/optimizer/schedulers/hyperband.py
@@ -92,14 +95,15 @@
 syne_tune/optimizer/schedulers/scheduler_searcher.py
 syne_tune/optimizer/schedulers/multiobjective/__init__.py
 syne_tune/optimizer/schedulers/multiobjective/linear_scalarizer.py
 syne_tune/optimizer/schedulers/multiobjective/moasha.py
 syne_tune/optimizer/schedulers/multiobjective/multi_objective_regularized_evolution.py
 syne_tune/optimizer/schedulers/multiobjective/multiobjective_priority.py
 syne_tune/optimizer/schedulers/multiobjective/non_dominated_priority.py
+syne_tune/optimizer/schedulers/multiobjective/nsga2_searcher.py
 syne_tune/optimizer/schedulers/multiobjective/utils.py
 syne_tune/optimizer/schedulers/neuralbands/__init__.py
 syne_tune/optimizer/schedulers/neuralbands/networks.py
 syne_tune/optimizer/schedulers/neuralbands/neuralband.py
 syne_tune/optimizer/schedulers/neuralbands/neuralband_supplement.py
 syne_tune/optimizer/schedulers/searchers/__init__.py
 syne_tune/optimizer/schedulers/searchers/bracket_distribution.py
@@ -158,29 +162,35 @@
 syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/gpiss_model.py
 syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/issm.py
 syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/likelihood.py
 syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/model_params.py
 syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/posterior_state.py
 syne_tune/optimizer/schedulers/searchers/bayesopt/models/__init__.py
 syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost_fifo_model.py
+syne_tune/optimizer/schedulers/searchers/bayesopt/models/estimator.py
 syne_tune/optimizer/schedulers/searchers/bayesopt/models/gp_mcmc_model.py
 syne_tune/optimizer/schedulers/searchers/bayesopt/models/gp_model.py
 syne_tune/optimizer/schedulers/searchers/bayesopt/models/gpiss_model.py
 syne_tune/optimizer/schedulers/searchers/bayesopt/models/kernel_factory.py
 syne_tune/optimizer/schedulers/searchers/bayesopt/models/meanstd_acqfunc.py
 syne_tune/optimizer/schedulers/searchers/bayesopt/models/meanstd_acqfunc_impl.py
 syne_tune/optimizer/schedulers/searchers/bayesopt/models/model_base.py
 syne_tune/optimizer/schedulers/searchers/bayesopt/models/model_skipopt.py
 syne_tune/optimizer/schedulers/searchers/bayesopt/models/model_transformer.py
+syne_tune/optimizer/schedulers/searchers/bayesopt/models/sklearn_estimator.py
+syne_tune/optimizer/schedulers/searchers/bayesopt/models/sklearn_predictor.py
 syne_tune/optimizer/schedulers/searchers/bayesopt/models/subsample_state_multi_fidelity.py
 syne_tune/optimizer/schedulers/searchers/bayesopt/models/subsample_state_single_fidelity.py
 syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/__init__.py
 syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/cost_model.py
 syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/linear_cost_model.py
 syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/sklearn_cost_model.py
+syne_tune/optimizer/schedulers/searchers/bayesopt/sklearn/__init__.py
+syne_tune/optimizer/schedulers/searchers/bayesopt/sklearn/estimator.py
+syne_tune/optimizer/schedulers/searchers/bayesopt/sklearn/predictor.py
 syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/__init__.py
 syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/base_classes.py
 syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/bo_algorithm.py
 syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/bo_algorithm_components.py
 syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/defaults.py
 syne_tune/optimizer/schedulers/searchers/bayesopt/utils/__init__.py
 syne_tune/optimizer/schedulers/searchers/bayesopt/utils/comparison_gpy.py
@@ -237,11 +247,12 @@
 syne_tune/optimizer/schedulers/utils/simple_profiler.py
 syne_tune/optimizer/schedulers/utils/successive_halving.py
 syne_tune/remote/__init__.py
 syne_tune/remote/estimators.py
 syne_tune/remote/remote_launcher.py
 syne_tune/remote/remote_main.py
 syne_tune/remote/remote_metrics_callback.py
+syne_tune/remote/scheduling.py
 syne_tune/utils/__init__.py
 syne_tune/utils/checkpoint.py
 syne_tune/utils/config_as_json.py
 syne_tune/utils/parse_bool.py
```

### Comparing `syne_tune-0.6.0/syne_tune.egg-info/requires.txt` & `syne_tune-0.7.0/syne_tune.egg-info/requires.txt`

 * *Files 14% similar despite different names*

```diff
@@ -8,18 +8,20 @@
 boto3
 sagemaker>=2.112.0
 PyYaml
 ujson
 s3fs
 
 [benchmarks]
-filelock
 torch
-tqdm
 torchvision
+transformers
+tqdm
+datasets==1.8.0
+filelock
 
 [blackbox-repository]
 numpy<1.24.0,>=1.16.0
 pandas
 fastparquet==0.8.1
 s3fs
 scikit-learn
@@ -28,14 +30,17 @@
 
 [bore]
 numpy<1.24.0,>=1.16.0
 xgboost
 scikit-learn
 GPy==1.12.0
 
+[botorch]
+botorch>=0.7.2
+
 [dev]
 pytest
 pytest-cov~=4.0.0
 pytest-timeout
 black==22.3.0
 flake8
 sphinx
@@ -43,29 +48,16 @@
 sphinx-autodoc-typehints
 myst-parser
 sphinx_copybutton
 sphinxcontrib-bibtex
 sphinxcontrib.jquery
 
 [extra]
-ray[tune]>=2.0.0
-scikit-learn
-scikit-optimize
 scipy>=1.3.3
 autograd>=1.3
-filelock
-torch
-tqdm
-torchvision
-numpy<1.24.0,>=1.16.0
-pandas
-fastparquet==0.8.1
-s3fs
-xgboost
-h5py
 statsmodels
 pytest
 pytest-cov~=4.0.0
 pytest-timeout
 black==22.3.0
 flake8
 sphinx
@@ -75,18 +67,34 @@
 sphinx_copybutton
 sphinxcontrib-bibtex
 sphinxcontrib.jquery
 boto3
 sagemaker>=2.112.0
 PyYaml
 ujson
+s3fs
+pymoo>=0.6.0
+matplotlib
+numpy<1.24.0,>=1.16.0
+pandas
+fastparquet==0.8.1
+scikit-learn
+xgboost
+h5py
+torch
+torchvision
+transformers
+tqdm
+datasets==1.8.0
+filelock
 onnxruntime>=1.10.0
 configspace
 yahpo-gym
-pymoo>=0.6.0
+ray[tune]>=2.0.0
+scikit-optimize
 botorch>=0.7.2
 
 [gpsearchers]
 scipy>=1.3.3
 autograd>=1.3
 
 [kde]
@@ -96,13 +104,16 @@
 pymoo>=0.6.0
 
 [raytune]
 ray[tune]>=2.0.0
 scikit-learn
 scikit-optimize
 
+[visual]
+matplotlib
+
 [yahpo]
 onnxruntime>=1.10.0
 pyyaml
 configspace
 pandas
 yahpo-gym
```

