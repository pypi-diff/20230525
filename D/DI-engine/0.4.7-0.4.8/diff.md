# Comparing `tmp/DI-engine-0.4.7.tar.gz` & `tmp/DI-engine-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/niuyazhe/code/opendilab/DI-engine/dist/.tmp-12iumh9g/DI-engine-0.4.7.tar", last modified: Wed Apr 12 15:08:02 2023, max compression
+gzip compressed data, was "/Users/niuyazhe/code/opendilab/DI-engine/dist/.tmp-45z5593t/DI-engine-0.4.8.tar", last modified: Thu May 25 06:04:58 2023, max compression
```

## Comparing `DI-engine-0.4.7.tar` & `DI-engine-0.4.8.tar`

### file list

```diff
@@ -1,1361 +1,1376 @@
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:02.461826 DI-engine-0.4.7/
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:01.595677 DI-engine-0.4.7/DI_engine.egg-info/
--rw-r--r--   0 niuyazhe (1370690143) 453037844    56871 2023-04-12 15:08:01.000000 DI-engine-0.4.7/DI_engine.egg-info/PKG-INFO
--rw-r--r--   0 niuyazhe (1370690143) 453037844    49085 2023-04-12 15:08:01.000000 DI-engine-0.4.7/DI_engine.egg-info/SOURCES.txt
--rw-r--r--   0 niuyazhe (1370690143) 453037844        1 2023-04-12 15:08:01.000000 DI-engine-0.4.7/DI_engine.egg-info/dependency_links.txt
--rw-r--r--   0 niuyazhe (1370690143) 453037844       86 2023-04-12 15:08:01.000000 DI-engine-0.4.7/DI_engine.egg-info/entry_points.txt
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1149 2023-04-12 15:08:01.000000 DI-engine-0.4.7/DI_engine.egg-info/requires.txt
--rw-r--r--   0 niuyazhe (1370690143) 453037844       11 2023-04-12 15:08:01.000000 DI-engine-0.4.7/DI_engine.egg-info/top_level.txt
--rw-r--r--   0 niuyazhe (1370690143) 453037844    11342 2021-07-08 05:53:26.000000 DI-engine-0.4.7/LICENSE
--rw-r--r--   0 niuyazhe (1370690143) 453037844    56871 2023-04-12 15:08:02.461529 DI-engine-0.4.7/PKG-INFO
--rw-r--r--   0 niuyazhe (1370690143) 453037844    55605 2023-04-11 14:03:16.000000 DI-engine-0.4.7/README.md
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:01.596679 DI-engine-0.4.7/ding/
--rw-r--r--   0 niuyazhe (1370690143) 453037844      380 2023-04-11 14:01:01.000000 DI-engine-0.4.7/ding/__init__.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:01.600853 DI-engine-0.4.7/ding/bonus/
--rw-r--r--   0 niuyazhe (1370690143) 453037844       58 2023-04-05 10:04:48.000000 DI-engine-0.4.7/ding/bonus/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    10868 2023-04-05 10:04:48.000000 DI-engine-0.4.7/ding/bonus/config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844      901 2023-01-06 07:07:56.000000 DI-engine-0.4.7/ding/bonus/demo.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     9777 2023-04-11 05:01:52.000000 DI-engine-0.4.7/ding/bonus/model.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     9287 2023-04-11 05:01:52.000000 DI-engine-0.4.7/ding/bonus/ppof.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     9060 2023-04-05 10:04:48.000000 DI-engine-0.4.7/ding/bonus/td3.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844      211 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/compatibility.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:01.604101 DI-engine-0.4.7/ding/config/
--rw-r--r--   0 niuyazhe (1370690143) 453037844      227 2023-01-04 09:44:45.000000 DI-engine-0.4.7/ding/config/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    24354 2023-04-05 10:04:48.000000 DI-engine-0.4.7/ding/config/config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    28073 2023-04-05 10:04:48.000000 DI-engine-0.4.7/ding/config/utils.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:01.606727 DI-engine-0.4.7/ding/data/
--rw-r--r--   0 niuyazhe (1370690143) 453037844      352 2022-12-13 15:12:49.000000 DI-engine-0.4.7/ding/data/__init__.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:01.609015 DI-engine-0.4.7/ding/data/buffer/
--rw-r--r--   0 niuyazhe (1370690143) 453037844      150 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/data/buffer/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     7617 2022-12-11 15:35:39.000000 DI-engine-0.4.7/ding/data/buffer/buffer.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    14785 2022-12-11 15:35:39.000000 DI-engine-0.4.7/ding/data/buffer/deque_buffer.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     4701 2023-02-20 14:45:59.000000 DI-engine-0.4.7/ding/data/buffer/deque_buffer_wrapper.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:01.613970 DI-engine-0.4.7/ding/data/buffer/middleware/
--rw-r--r--   0 niuyazhe (1370690143) 453037844      291 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/data/buffer/middleware/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1064 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/data/buffer/middleware/clone_object.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1648 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/data/buffer/middleware/group_sample.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1496 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/data/buffer/middleware/padding.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     6962 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/data/buffer/middleware/priority.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844      979 2022-08-02 16:56:36.000000 DI-engine-0.4.7/ding/data/buffer/middleware/sample_range_view.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1830 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/data/buffer/middleware/staleness_check.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1887 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/data/buffer/middleware/use_time_check.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:01.614846 DI-engine-0.4.7/ding/data/level_replay/
--rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2022-10-19 09:16:29.000000 DI-engine-0.4.7/ding/data/level_replay/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    13812 2023-01-02 10:31:34.000000 DI-engine-0.4.7/ding/data/level_replay/level_sampler.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     5501 2022-12-13 15:12:49.000000 DI-engine-0.4.7/ding/data/model_loader.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     5008 2023-03-09 12:42:49.000000 DI-engine-0.4.7/ding/data/shm_buffer.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:01.616635 DI-engine-0.4.7/ding/data/storage/
--rw-r--r--   0 niuyazhe (1370690143) 453037844       77 2022-12-13 15:12:49.000000 DI-engine-0.4.7/ding/data/storage/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844      605 2022-12-13 15:12:49.000000 DI-engine-0.4.7/ding/data/storage/file.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844      326 2022-12-13 15:12:49.000000 DI-engine-0.4.7/ding/data/storage/storage.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    11978 2022-12-13 15:12:49.000000 DI-engine-0.4.7/ding/data/storage_loader.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:01.638031 DI-engine-0.4.7/ding/entry/
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1732 2023-03-09 11:08:49.000000 DI-engine-0.4.7/ding/entry/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    11820 2022-12-13 15:12:49.000000 DI-engine-0.4.7/ding/entry/application_entry.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     9797 2022-10-19 09:16:29.000000 DI-engine-0.4.7/ding/entry/application_entry_drex_collect_data.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     6652 2022-10-19 09:16:29.000000 DI-engine-0.4.7/ding/entry/application_entry_trex_collect_data.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    13003 2022-10-19 09:16:29.000000 DI-engine-0.4.7/ding/entry/cli.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     5475 2022-12-13 15:12:49.000000 DI-engine-0.4.7/ding/entry/cli_ditask.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:01.639964 DI-engine-0.4.7/ding/entry/cli_parsers/
--rw-r--r--   0 niuyazhe (1370690143) 453037844      136 2022-07-19 08:28:37.000000 DI-engine-0.4.7/ding/entry/cli_parsers/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     5855 2022-12-13 15:12:49.000000 DI-engine-0.4.7/ding/entry/cli_parsers/k8s_parser.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     5656 2022-12-13 15:12:49.000000 DI-engine-0.4.7/ding/entry/cli_parsers/slurm_parser.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    11742 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/entry/dist_entry.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     5631 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/entry/parallel_entry.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1156 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/entry/predefined_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     6335 2023-03-09 11:08:49.000000 DI-engine-0.4.7/ding/entry/serial_entry.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     4005 2022-10-31 06:23:24.000000 DI-engine-0.4.7/ding/entry/serial_entry_bc.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     8933 2023-03-21 10:44:34.000000 DI-engine-0.4.7/ding/entry/serial_entry_bco.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     3405 2022-10-19 09:16:29.000000 DI-engine-0.4.7/ding/entry/serial_entry_decision_transformer.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    12388 2022-10-19 09:16:29.000000 DI-engine-0.4.7/ding/entry/serial_entry_dqfd.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     8037 2022-12-13 15:12:49.000000 DI-engine-0.4.7/ding/entry/serial_entry_gail.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     8452 2022-10-19 09:16:29.000000 DI-engine-0.4.7/ding/entry/serial_entry_guided_cost.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    10336 2022-10-19 09:16:29.000000 DI-engine-0.4.7/ding/entry/serial_entry_mbrl.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     7979 2022-10-19 09:16:29.000000 DI-engine-0.4.7/ding/entry/serial_entry_ngu.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     4645 2022-10-19 09:16:29.000000 DI-engine-0.4.7/ding/entry/serial_entry_offline.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     4963 2022-12-13 15:12:49.000000 DI-engine-0.4.7/ding/entry/serial_entry_onpolicy.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     4460 2022-10-19 09:16:29.000000 DI-engine-0.4.7/ding/entry/serial_entry_onpolicy_ppg.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     4444 2023-03-09 11:08:49.000000 DI-engine-0.4.7/ding/entry/serial_entry_pc.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     5614 2022-10-19 09:16:29.000000 DI-engine-0.4.7/ding/entry/serial_entry_plr.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     6520 2023-01-06 07:05:23.000000 DI-engine-0.4.7/ding/entry/serial_entry_preference_based_irl.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     4811 2023-01-06 07:05:23.000000 DI-engine-0.4.7/ding/entry/serial_entry_preference_based_irl_onpolicy.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    12314 2022-10-19 09:16:29.000000 DI-engine-0.4.7/ding/entry/serial_entry_r2d3.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     6809 2023-03-09 11:08:49.000000 DI-engine-0.4.7/ding/entry/serial_entry_reward_model_offpolicy.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     6557 2023-03-09 11:08:49.000000 DI-engine-0.4.7/ding/entry/serial_entry_reward_model_onpolicy.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     8837 2022-10-19 09:16:29.000000 DI-engine-0.4.7/ding/entry/serial_entry_sqil.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    10374 2022-10-19 09:16:29.000000 DI-engine-0.4.7/ding/entry/serial_entry_td3_vae.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2342 2022-09-16 15:18:07.000000 DI-engine-0.4.7/ding/entry/utils.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:01.640484 DI-engine-0.4.7/ding/envs/
--rw-r--r--   0 niuyazhe (1370690143) 453037844       74 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/envs/__init__.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:01.642653 DI-engine-0.4.7/ding/envs/common/
--rw-r--r--   0 niuyazhe (1370690143) 453037844      354 2022-10-19 09:16:29.000000 DI-engine-0.4.7/ding/envs/common/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    10829 2022-10-19 09:16:29.000000 DI-engine-0.4.7/ding/envs/common/common_function.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1625 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/envs/common/env_element.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844      986 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/envs/common/env_element_runner.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:01.645161 DI-engine-0.4.7/ding/envs/env/
--rw-r--r--   0 niuyazhe (1370690143) 453037844      386 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/envs/env/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     6902 2023-01-02 16:43:42.000000 DI-engine-0.4.7/ding/envs/env/base_env.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1751 2023-03-09 11:08:49.000000 DI-engine-0.4.7/ding/envs/env/default_wrapper.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     9454 2023-04-05 10:04:48.000000 DI-engine-0.4.7/ding/envs/env/ding_env_wrapper.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     7078 2022-12-13 15:12:49.000000 DI-engine-0.4.7/ding/envs/env/env_implementation_check.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:01.647533 DI-engine-0.4.7/ding/envs/env/tests/
--rw-r--r--   0 niuyazhe (1370690143) 453037844       30 2022-07-19 08:28:37.000000 DI-engine-0.4.7/ding/envs/env/tests/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2216 2022-12-13 15:12:49.000000 DI-engine-0.4.7/ding/envs/env/tests/demo_env.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     7618 2022-12-13 15:12:49.000000 DI-engine-0.4.7/ding/envs/env/tests/test_ding_env_wrapper.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1974 2022-07-19 08:28:37.000000 DI-engine-0.4.7/ding/envs/env/tests/test_env_implementation_check.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:01.650754 DI-engine-0.4.7/ding/envs/env_manager/
--rw-r--r--   0 niuyazhe (1370690143) 453037844      394 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/envs/env_manager/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    21523 2023-04-05 10:04:48.000000 DI-engine-0.4.7/ding/envs/env_manager/base_env_manager.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    24099 2022-12-13 15:12:49.000000 DI-engine-0.4.7/ding/envs/env_manager/env_supervisor.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     4222 2022-12-13 15:12:49.000000 DI-engine-0.4.7/ding/envs/env_manager/envpool_env_manager.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     5793 2022-12-13 15:12:49.000000 DI-engine-0.4.7/ding/envs/env_manager/gym_vector_env_manager.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    36999 2023-03-09 11:08:49.000000 DI-engine-0.4.7/ding/envs/env_manager/subprocess_env_manager.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:01.655304 DI-engine-0.4.7/ding/envs/env_manager/tests/
--rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/envs/env_manager/tests/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     8258 2023-01-02 10:31:34.000000 DI-engine-0.4.7/ding/envs/env_manager/tests/conftest.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     9270 2023-01-02 10:31:34.000000 DI-engine-0.4.7/ding/envs/env_manager/tests/test_base_env_manager.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    18474 2023-01-02 10:31:34.000000 DI-engine-0.4.7/ding/envs/env_manager/tests/test_env_supervisor.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1456 2022-07-19 08:28:37.000000 DI-engine-0.4.7/ding/envs/env_manager/tests/test_envpool_env_manager.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2306 2023-01-02 10:31:34.000000 DI-engine-0.4.7/ding/envs/env_manager/tests/test_gym_vector_env_manager.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844      783 2022-07-19 08:28:37.000000 DI-engine-0.4.7/ding/envs/env_manager/tests/test_shm.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     9590 2023-01-02 10:31:34.000000 DI-engine-0.4.7/ding/envs/env_manager/tests/test_subprocess_env_manager.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:01.656448 DI-engine-0.4.7/ding/envs/env_wrappers/
--rw-r--r--   0 niuyazhe (1370690143) 453037844       28 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/envs/env_wrappers/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    43614 2023-03-21 10:15:23.000000 DI-engine-0.4.7/ding/envs/env_wrappers/env_wrappers.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:01.671253 DI-engine-0.4.7/ding/example/
--rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2023-01-04 06:30:14.000000 DI-engine-0.4.7/ding/example/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1997 2023-03-09 07:52:49.000000 DI-engine-0.4.7/ding/example/c51_nstep.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1509 2023-03-06 03:18:03.000000 DI-engine-0.4.7/ding/example/collect_demo_data.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1747 2023-01-06 07:05:23.000000 DI-engine-0.4.7/ding/example/cql.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2098 2023-01-06 07:05:23.000000 DI-engine-0.4.7/ding/example/d4pg.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1962 2023-01-06 07:05:23.000000 DI-engine-0.4.7/ding/example/ddpg.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     4394 2023-01-06 07:05:23.000000 DI-engine-0.4.7/ding/example/dqn.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1928 2023-01-06 07:05:23.000000 DI-engine-0.4.7/ding/example/dqn_her.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1949 2023-01-06 07:05:23.000000 DI-engine-0.4.7/ding/example/dqn_new_env.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2056 2023-01-06 07:05:23.000000 DI-engine-0.4.7/ding/example/dqn_nstep.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2112 2023-01-06 07:05:23.000000 DI-engine-0.4.7/ding/example/dqn_per.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2028 2023-01-06 07:05:23.000000 DI-engine-0.4.7/ding/example/dqn_rnd.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2131 2023-03-08 06:20:41.000000 DI-engine-0.4.7/ding/example/dt.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1991 2023-01-06 07:05:23.000000 DI-engine-0.4.7/ding/example/iqn_nstep.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1838 2023-01-06 07:05:23.000000 DI-engine-0.4.7/ding/example/pdqn.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2539 2023-01-06 07:05:23.000000 DI-engine-0.4.7/ding/example/ppg_offpolicy.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1807 2023-01-06 07:05:23.000000 DI-engine-0.4.7/ding/example/ppo.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1895 2023-01-06 07:05:23.000000 DI-engine-0.4.7/ding/example/ppo_offpolicy.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2003 2023-01-06 07:05:23.000000 DI-engine-0.4.7/ding/example/qrdqn_nstep.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1934 2023-01-06 07:05:23.000000 DI-engine-0.4.7/ding/example/r2d2.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1998 2023-01-06 07:05:23.000000 DI-engine-0.4.7/ding/example/sac.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     3213 2023-01-06 07:05:23.000000 DI-engine-0.4.7/ding/example/sqil.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     3377 2023-01-06 07:05:23.000000 DI-engine-0.4.7/ding/example/sqil_continuous.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1842 2023-01-06 07:05:23.000000 DI-engine-0.4.7/ding/example/sql.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1866 2023-01-06 07:05:23.000000 DI-engine-0.4.7/ding/example/td3.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2447 2023-01-06 07:05:23.000000 DI-engine-0.4.7/ding/example/trex.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:01.675069 DI-engine-0.4.7/ding/framework/
--rw-r--r--   0 niuyazhe (1370690143) 453037844      361 2022-12-13 15:12:49.000000 DI-engine-0.4.7/ding/framework/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     3247 2023-04-05 10:04:48.000000 DI-engine-0.4.7/ding/framework/context.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     4120 2022-12-13 15:12:49.000000 DI-engine-0.4.7/ding/framework/event_loop.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:01.677778 DI-engine-0.4.7/ding/framework/message_queue/
--rw-r--r--   0 niuyazhe (1370690143) 453037844       69 2022-07-19 08:28:37.000000 DI-engine-0.4.7/ding/framework/message_queue/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1635 2022-07-19 08:28:37.000000 DI-engine-0.4.7/ding/framework/message_queue/mq.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2524 2022-12-13 15:12:49.000000 DI-engine-0.4.7/ding/framework/message_queue/nng.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2385 2022-08-02 16:56:36.000000 DI-engine-0.4.7/ding/framework/message_queue/redis.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:01.681255 DI-engine-0.4.7/ding/framework/middleware/
--rw-r--r--   0 niuyazhe (1370690143) 453037844      244 2023-01-04 09:44:45.000000 DI-engine-0.4.7/ding/framework/middleware/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     3017 2023-01-06 07:05:23.000000 DI-engine-0.4.7/ding/framework/middleware/ckpt_handler.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     8143 2023-02-17 05:18:00.000000 DI-engine-0.4.7/ding/framework/middleware/collector.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    11569 2022-12-13 15:12:49.000000 DI-engine-0.4.7/ding/framework/middleware/distributer.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:01.688577 DI-engine-0.4.7/ding/framework/middleware/functional/
--rw-r--r--   0 niuyazhe (1370690143) 453037844      792 2023-01-04 09:44:45.000000 DI-engine-0.4.7/ding/framework/middleware/functional/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     3242 2023-03-09 11:08:49.000000 DI-engine-0.4.7/ding/framework/middleware/functional/advantage_estimator.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     5426 2023-04-05 10:04:48.000000 DI-engine-0.4.7/ding/framework/middleware/functional/collector.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844      912 2023-04-05 10:04:48.000000 DI-engine-0.4.7/ding/framework/middleware/functional/ctx_helper.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    11619 2023-01-04 09:44:45.000000 DI-engine-0.4.7/ding/framework/middleware/functional/data_processor.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     3968 2022-12-13 15:12:50.000000 DI-engine-0.4.7/ding/framework/middleware/functional/enhancer.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    17448 2023-04-05 10:04:48.000000 DI-engine-0.4.7/ding/framework/middleware/functional/evaluator.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1541 2022-12-13 15:12:50.000000 DI-engine-0.4.7/ding/framework/middleware/functional/explorer.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    21299 2023-04-05 10:04:48.000000 DI-engine-0.4.7/ding/framework/middleware/functional/logger.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2054 2022-12-13 15:12:50.000000 DI-engine-0.4.7/ding/framework/middleware/functional/termination_checker.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1021 2022-12-13 15:12:50.000000 DI-engine-0.4.7/ding/framework/middleware/functional/timer.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     3611 2023-03-10 09:15:22.000000 DI-engine-0.4.7/ding/framework/middleware/functional/trainer.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     3717 2023-02-22 10:35:54.000000 DI-engine-0.4.7/ding/framework/middleware/learner.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:01.695539 DI-engine-0.4.7/ding/framework/middleware/tests/
--rw-r--r--   0 niuyazhe (1370690143) 453037844       76 2023-03-21 10:44:32.000000 DI-engine-0.4.7/ding/framework/middleware/tests/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     3256 2022-12-13 15:12:50.000000 DI-engine-0.4.7/ding/framework/middleware/tests/mock_for_test.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     3213 2023-03-09 11:08:49.000000 DI-engine-0.4.7/ding/framework/middleware/tests/test_advantage_estimator.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2074 2023-01-06 07:05:23.000000 DI-engine-0.4.7/ding/framework/middleware/tests/test_ckpt_handler.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     3049 2023-01-04 09:44:45.000000 DI-engine-0.4.7/ding/framework/middleware/tests/test_collector.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     9202 2023-01-04 09:44:45.000000 DI-engine-0.4.7/ding/framework/middleware/tests/test_data_processor.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     7060 2023-04-05 10:04:48.000000 DI-engine-0.4.7/ding/framework/middleware/tests/test_distributer.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2590 2022-12-13 15:12:50.000000 DI-engine-0.4.7/ding/framework/middleware/tests/test_enhancer.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1200 2022-10-19 12:18:13.000000 DI-engine-0.4.7/ding/framework/middleware/tests/test_evaluator.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844      731 2022-07-19 08:28:37.000000 DI-engine-0.4.7/ding/framework/middleware/tests/test_explorer.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     9113 2023-04-05 10:04:48.000000 DI-engine-0.4.7/ding/framework/middleware/tests/test_logger.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     3379 2023-01-29 05:51:23.000000 DI-engine-0.4.7/ding/framework/middleware/tests/test_trainer.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:01.697838 DI-engine-0.4.7/ding/framework/middleware_v3/
--rw-r--r--   0 niuyazhe (1370690143) 453037844      167 2022-09-01 10:26:16.000000 DI-engine-0.4.7/ding/framework/middleware_v3/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2553 2022-09-04 07:49:02.000000 DI-engine-0.4.7/ding/framework/middleware_v3/ckpt_handler.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     5011 2022-09-01 10:45:00.000000 DI-engine-0.4.7/ding/framework/middleware_v3/collector.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:01.703189 DI-engine-0.4.7/ding/framework/middleware_v3/functional/
--rw-r--r--   0 niuyazhe (1370690143) 453037844      578 2022-09-01 10:26:16.000000 DI-engine-0.4.7/ding/framework/middleware_v3/functional/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2742 2022-09-01 10:26:16.000000 DI-engine-0.4.7/ding/framework/middleware_v3/functional/advantage_estimator.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     5391 2022-09-05 08:12:51.000000 DI-engine-0.4.7/ding/framework/middleware_v3/functional/collector.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844      746 2022-09-01 10:26:16.000000 DI-engine-0.4.7/ding/framework/middleware_v3/functional/ctx_helper.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    10145 2022-09-01 11:15:00.000000 DI-engine-0.4.7/ding/framework/middleware_v3/functional/data_processor.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     3672 2022-09-01 10:26:16.000000 DI-engine-0.4.7/ding/framework/middleware_v3/functional/enhancer.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     7765 2022-09-01 11:07:51.000000 DI-engine-0.4.7/ding/framework/middleware_v3/functional/evaluator.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1408 2022-09-01 10:26:49.000000 DI-engine-0.4.7/ding/framework/middleware_v3/functional/explorer.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844      742 2022-09-01 10:26:16.000000 DI-engine-0.4.7/ding/framework/middleware_v3/functional/termination_checker.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2951 2022-09-01 11:16:03.000000 DI-engine-0.4.7/ding/framework/middleware_v3/functional/trainer.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     3507 2022-09-01 11:09:28.000000 DI-engine-0.4.7/ding/framework/middleware_v3/learner.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:01.708562 DI-engine-0.4.7/ding/framework/middleware_v3/tests/
--rw-r--r--   0 niuyazhe (1370690143) 453037844       76 2023-03-21 10:44:33.000000 DI-engine-0.4.7/ding/framework/middleware_v3/tests/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     3252 2022-09-01 10:26:15.000000 DI-engine-0.4.7/ding/framework/middleware_v3/tests/mock_for_test.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     3198 2022-09-01 10:26:15.000000 DI-engine-0.4.7/ding/framework/middleware_v3/tests/test_advantage_estimator.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1987 2022-09-04 07:49:15.000000 DI-engine-0.4.7/ding/framework/middleware_v3/tests/test_ckpt_handler.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     3122 2022-09-01 10:26:15.000000 DI-engine-0.4.7/ding/framework/middleware_v3/tests/test_collector.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     8230 2022-09-01 10:26:16.000000 DI-engine-0.4.7/ding/framework/middleware_v3/tests/test_data_processor.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2642 2022-09-01 10:26:16.000000 DI-engine-0.4.7/ding/framework/middleware_v3/tests/test_enhancer.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1200 2022-09-01 10:26:15.000000 DI-engine-0.4.7/ding/framework/middleware_v3/tests/test_evaluator.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844      731 2022-09-01 10:26:15.000000 DI-engine-0.4.7/ding/framework/middleware_v3/tests/test_explorer.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     3286 2022-09-01 10:26:16.000000 DI-engine-0.4.7/ding/framework/middleware_v3/tests/test_trainer.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    15133 2022-12-13 15:12:50.000000 DI-engine-0.4.7/ding/framework/parallel.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    14388 2023-04-05 10:04:46.000000 DI-engine-0.4.7/ding/framework/supervisor.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    19497 2023-04-05 10:04:48.000000 DI-engine-0.4.7/ding/framework/task.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:01.709654 DI-engine-0.4.7/ding/framework/wrapper/
--rw-r--r--   0 niuyazhe (1370690143) 453037844       34 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/framework/wrapper/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1922 2022-12-13 15:12:50.000000 DI-engine-0.4.7/ding/framework/wrapper/step_timer.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:01.710757 DI-engine-0.4.7/ding/hpc_rl/
--rw-r--r--   0 niuyazhe (1370690143) 453037844       33 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/hpc_rl/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     5953 2022-12-13 15:12:50.000000 DI-engine-0.4.7/ding/hpc_rl/wrapper.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:01.711333 DI-engine-0.4.7/ding/interaction/
--rw-r--r--   0 niuyazhe (1370690143) 453037844       43 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/interaction/__init__.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:01.714377 DI-engine-0.4.7/ding/interaction/base/
--rw-r--r--   0 niuyazhe (1370690143) 453037844      382 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/interaction/base/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2806 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/interaction/base/app.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     5341 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/interaction/base/common.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     4846 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/interaction/base/network.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2163 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/interaction/base/threading.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:01.715337 DI-engine-0.4.7/ding/interaction/config/
--rw-r--r--   0 niuyazhe (1370690143) 453037844      297 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/interaction/config/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844      432 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/interaction/config/base.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:01.717325 DI-engine-0.4.7/ding/interaction/exception/
--rw-r--r--   0 niuyazhe (1370690143) 453037844      848 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/interaction/exception/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2466 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/interaction/exception/base.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     3512 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/interaction/exception/master.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     3914 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/interaction/exception/slave.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:01.720753 DI-engine-0.4.7/ding/interaction/master/
--rw-r--r--   0 niuyazhe (1370690143) 453037844       27 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/interaction/master/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844      293 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/interaction/master/base.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    17041 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/interaction/master/connection.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    27918 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/interaction/master/master.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     9524 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/interaction/master/task.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:01.722337 DI-engine-0.4.7/ding/interaction/slave/
--rw-r--r--   0 niuyazhe (1370690143) 453037844      105 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/interaction/slave/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     3753 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/interaction/slave/action.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    19857 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/interaction/slave/slave.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:01.723242 DI-engine-0.4.7/ding/interaction/tests/
--rw-r--r--   0 niuyazhe (1370690143) 453037844       94 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/interaction/tests/__init__.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:01.725797 DI-engine-0.4.7/ding/interaction/tests/base/
--rw-r--r--   0 niuyazhe (1370690143) 453037844      318 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/interaction/tests/base/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     6161 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/interaction/tests/base/test_app.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2036 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/interaction/tests/base/test_common.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     6046 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/interaction/tests/base/test_network.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     3324 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/interaction/tests/base/test_threading.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:01.726868 DI-engine-0.4.7/ding/interaction/tests/config/
--rw-r--r--   0 niuyazhe (1370690143) 453037844       45 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/interaction/tests/config/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844      226 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/interaction/tests/config/test_base.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:01.729176 DI-engine-0.4.7/ding/interaction/tests/exception/
--rw-r--r--   0 niuyazhe (1370690143) 453037844      110 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/interaction/tests/exception/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1562 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/interaction/tests/exception/test_base.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2877 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/interaction/tests/exception/test_master.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     3293 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/interaction/tests/exception/test_slave.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:01.731175 DI-engine-0.4.7/ding/interaction/tests/interaction/
--rw-r--r--   0 niuyazhe (1370690143) 453037844       94 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/interaction/tests/interaction/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1401 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/interaction/tests/interaction/bases.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1439 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/interaction/tests/interaction/test_errors.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     4795 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/interaction/tests/interaction/test_simple.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:01.732573 DI-engine-0.4.7/ding/interaction/tests/test_utils/
--rw-r--r--   0 niuyazhe (1370690143) 453037844       94 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/interaction/tests/test_utils/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844      417 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/interaction/tests/test_utils/random.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1099 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/interaction/tests/test_utils/stream.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:01.737183 DI-engine-0.4.7/ding/league/
--rw-r--r--   0 niuyazhe (1370690143) 453037844      345 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/league/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1749 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/league/algorithm.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    13037 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/league/base_league.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     4590 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/league/metric.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     5355 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/league/one_vs_one_league.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    13828 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/league/player.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    10938 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/league/shared_payoff.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     9522 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/league/starcraft_player.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:01.737899 DI-engine-0.4.7/ding/model/
--rw-r--r--   0 niuyazhe (1370690143) 453037844       69 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/model/__init__.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:01.741041 DI-engine-0.4.7/ding/model/common/
--rw-r--r--   0 niuyazhe (1370690143) 453037844      355 2023-04-11 05:01:52.000000 DI-engine-0.4.7/ding/model/common/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    12145 2023-03-09 11:08:49.000000 DI-engine-0.4.7/ding/model/common/encoder.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    59073 2023-04-11 05:01:52.000000 DI-engine-0.4.7/ding/model/common/head.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844      628 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/model/common/utils.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:01.758974 DI-engine-0.4.7/ding/model/template/
--rw-r--r--   0 niuyazhe (1370690143) 453037844      761 2023-03-09 11:08:49.000000 DI-engine-0.4.7/ding/model/template/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     8851 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/model/template/acer.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    18749 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/model/template/atoc.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     8563 2023-03-09 11:08:49.000000 DI-engine-0.4.7/ding/model/template/bc.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    19316 2022-10-19 09:16:29.000000 DI-engine-0.4.7/ding/model/template/collaq.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     7751 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/model/template/coma.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     4713 2022-07-19 08:28:37.000000 DI-engine-0.4.7/ding/model/template/decision_transformer.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    17708 2022-10-19 09:16:29.000000 DI-engine-0.4.7/ding/model/template/ebm.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1790 2022-12-11 15:35:39.000000 DI-engine-0.4.7/ding/model/template/madqn.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    20794 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/model/template/maqac.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    12386 2022-10-19 09:16:29.000000 DI-engine-0.4.7/ding/model/template/mavac.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    10574 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/model/template/ngu.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     9646 2023-03-09 11:08:49.000000 DI-engine-0.4.7/ding/model/template/pdqn.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2793 2022-12-11 15:35:39.000000 DI-engine-0.4.7/ding/model/template/pg.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2389 2022-10-19 09:16:29.000000 DI-engine-0.4.7/ding/model/template/ppg.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     8657 2023-03-09 11:08:49.000000 DI-engine-0.4.7/ding/model/template/procedure_cloning.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    51526 2023-04-05 10:04:48.000000 DI-engine-0.4.7/ding/model/template/q_learning.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    27157 2023-04-05 10:04:48.000000 DI-engine-0.4.7/ding/model/template/qac.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    12226 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/model/template/qac_dist.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     9551 2022-10-19 09:16:29.000000 DI-engine-0.4.7/ding/model/template/qmix.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     7140 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/model/template/qtran.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844      589 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/model/template/sqn.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    15891 2023-02-23 09:45:40.000000 DI-engine-0.4.7/ding/model/template/vac.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    12328 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/model/template/vae.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    12586 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/model/template/wqmix.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:01.760977 DI-engine-0.4.7/ding/model/wrapper/
--rw-r--r--   0 niuyazhe (1370690143) 453037844       90 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/model/wrapper/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    37923 2022-12-13 15:12:50.000000 DI-engine-0.4.7/ding/model/wrapper/model_wrappers.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    21725 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/model/wrapper/test_model_wrappers.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:01.797607 DI-engine-0.4.7/ding/policy/
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1543 2023-03-22 09:00:17.000000 DI-engine-0.4.7/ding/policy/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    11203 2023-04-05 10:04:48.000000 DI-engine-0.4.7/ding/policy/a2c.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    24338 2023-04-05 10:04:48.000000 DI-engine-0.4.7/ding/policy/acer.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    16201 2023-04-05 10:04:48.000000 DI-engine-0.4.7/ding/policy/atoc.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    11919 2023-04-05 10:04:48.000000 DI-engine-0.4.7/ding/policy/base_policy.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    13093 2023-04-05 10:04:48.000000 DI-engine-0.4.7/ding/policy/bc.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    19714 2023-04-05 10:04:48.000000 DI-engine-0.4.7/ding/policy/bdq.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    12526 2023-04-05 10:04:48.000000 DI-engine-0.4.7/ding/policy/c51.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    21034 2023-04-05 10:04:48.000000 DI-engine-0.4.7/ding/policy/collaq.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    18431 2023-04-05 10:04:48.000000 DI-engine-0.4.7/ding/policy/coma.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    12184 2023-03-22 09:00:17.000000 DI-engine-0.4.7/ding/policy/command_mode_policy_instance.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1998 2023-03-22 09:00:17.000000 DI-engine-0.4.7/ding/policy/common_utils.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    37331 2023-04-05 10:04:48.000000 DI-engine-0.4.7/ding/policy/cql.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    15951 2023-04-05 10:04:48.000000 DI-engine-0.4.7/ding/policy/d4pg.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    22393 2023-04-05 10:04:48.000000 DI-engine-0.4.7/ding/policy/ddpg.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    15603 2023-04-05 10:04:48.000000 DI-engine-0.4.7/ding/policy/decision_transformer.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    13749 2023-04-05 10:04:48.000000 DI-engine-0.4.7/ding/policy/dqfd.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    36869 2023-04-05 10:04:48.000000 DI-engine-0.4.7/ding/policy/dqn.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    12436 2023-04-05 10:04:48.000000 DI-engine-0.4.7/ding/policy/fqf.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     6988 2023-04-05 10:04:48.000000 DI-engine-0.4.7/ding/policy/ibc.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     9032 2023-04-05 10:04:48.000000 DI-engine-0.4.7/ding/policy/il.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    23117 2023-04-05 10:04:48.000000 DI-engine-0.4.7/ding/policy/impala.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     9233 2023-04-05 10:04:48.000000 DI-engine-0.4.7/ding/policy/iqn.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    15386 2023-04-05 10:04:48.000000 DI-engine-0.4.7/ding/policy/madqn.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:01.799436 DI-engine-0.4.7/ding/policy/mbpolicy/
--rw-r--r--   0 niuyazhe (1370690143) 453037844       31 2022-07-19 08:28:37.000000 DI-engine-0.4.7/ding/policy/mbpolicy/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    15898 2023-04-05 10:04:48.000000 DI-engine-0.4.7/ding/policy/mbpolicy/mbsac.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1318 2022-08-02 16:56:36.000000 DI-engine-0.4.7/ding/policy/mbpolicy/utils.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    12521 2023-04-05 10:04:48.000000 DI-engine-0.4.7/ding/policy/mdqn.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    28541 2023-04-05 10:04:48.000000 DI-engine-0.4.7/ding/policy/ngu.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    13695 2023-04-05 10:04:48.000000 DI-engine-0.4.7/ding/policy/offppo_collect_traj.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     6878 2023-04-05 10:04:48.000000 DI-engine-0.4.7/ding/policy/pc.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    22366 2023-04-05 10:04:48.000000 DI-engine-0.4.7/ding/policy/pdqn.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     8459 2023-04-05 10:04:48.000000 DI-engine-0.4.7/ding/policy/pg.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2892 2023-03-22 09:00:17.000000 DI-engine-0.4.7/ding/policy/policy_factory.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    55970 2023-04-05 10:04:48.000000 DI-engine-0.4.7/ding/policy/ppg.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    56458 2023-04-05 10:04:48.000000 DI-engine-0.4.7/ding/policy/ppo.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    15076 2023-04-11 05:01:52.000000 DI-engine-0.4.7/ding/policy/ppof.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    20183 2023-04-05 10:04:48.000000 DI-engine-0.4.7/ding/policy/qmix.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     9007 2023-04-05 10:04:48.000000 DI-engine-0.4.7/ding/policy/qrdqn.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    21050 2023-04-05 10:04:48.000000 DI-engine-0.4.7/ding/policy/qtran.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    24622 2023-04-05 10:04:48.000000 DI-engine-0.4.7/ding/policy/r2d2.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    23742 2023-04-05 10:04:48.000000 DI-engine-0.4.7/ding/policy/r2d2_collect_traj.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    24134 2023-04-05 10:04:48.000000 DI-engine-0.4.7/ding/policy/r2d2_gtrxl.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    26516 2023-04-05 10:04:48.000000 DI-engine-0.4.7/ding/policy/r2d3.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    13923 2023-04-05 10:04:48.000000 DI-engine-0.4.7/ding/policy/rainbow.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    56196 2023-04-05 10:04:48.000000 DI-engine-0.4.7/ding/policy/sac.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    12620 2023-04-05 10:04:48.000000 DI-engine-0.4.7/ding/policy/sql.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    14436 2023-04-05 10:04:48.000000 DI-engine-0.4.7/ding/policy/sqn.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     9877 2023-04-05 10:04:48.000000 DI-engine-0.4.7/ding/policy/td3.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    17418 2023-04-05 10:04:48.000000 DI-engine-0.4.7/ding/policy/td3_bc.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    32866 2023-04-05 10:04:48.000000 DI-engine-0.4.7/ding/policy/td3_vae.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    15786 2023-04-05 10:04:48.000000 DI-engine-0.4.7/ding/policy/wqmix.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:01.807449 DI-engine-0.4.7/ding/reward_model/
--rw-r--r--   0 niuyazhe (1370690143) 453037844      670 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/reward_model/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     4914 2023-03-09 11:08:49.000000 DI-engine-0.4.7/ding/reward_model/base_reward_model.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     4791 2023-04-05 10:04:48.000000 DI-engine-0.4.7/ding/reward_model/drex_reward_model.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    13515 2023-04-05 10:04:48.000000 DI-engine-0.4.7/ding/reward_model/gail_irl_model.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     8298 2023-04-05 10:04:48.000000 DI-engine-0.4.7/ding/reward_model/guided_cost_reward_model.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     6595 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/reward_model/her_reward_model.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    16854 2023-04-05 10:04:48.000000 DI-engine-0.4.7/ding/reward_model/icm_reward_model.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    26350 2023-04-05 10:04:48.000000 DI-engine-0.4.7/ding/reward_model/ngu_reward_model.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     9980 2023-04-05 10:04:48.000000 DI-engine-0.4.7/ding/reward_model/pdeil_irl_model.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    12376 2023-04-05 10:04:48.000000 DI-engine-0.4.7/ding/reward_model/pwil_irl_model.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    10439 2023-04-05 10:04:48.000000 DI-engine-0.4.7/ding/reward_model/red_irl_model.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    12103 2023-04-05 10:04:48.000000 DI-engine-0.4.7/ding/reward_model/rnd_reward_model.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    20419 2023-04-05 10:04:48.000000 DI-engine-0.4.7/ding/reward_model/trex_reward_model.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:01.818483 DI-engine-0.4.7/ding/rl_utils/
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1894 2023-04-11 05:01:52.000000 DI-engine-0.4.7/ding/rl_utils/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1700 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/rl_utils/a2c.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     4723 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/rl_utils/acer.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    10256 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/rl_utils/adder.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1127 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/rl_utils/beta_function.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2438 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/rl_utils/coma.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     7580 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/rl_utils/exploration.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2435 2023-01-02 12:59:23.000000 DI-engine-0.4.7/ding/rl_utils/gae.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2782 2022-12-13 15:12:50.000000 DI-engine-0.4.7/ding/rl_utils/isw.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1409 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/rl_utils/ppg.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    12781 2023-02-21 09:28:07.000000 DI-engine-0.4.7/ding/rl_utils/ppo.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1729 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/rl_utils/retrace.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1510 2023-02-12 11:34:47.000000 DI-engine-0.4.7/ding/rl_utils/sampler.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    62641 2023-04-05 10:04:48.000000 DI-engine-0.4.7/ding/rl_utils/td.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     3752 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/rl_utils/upgo.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2266 2023-04-11 05:01:52.000000 DI-engine-0.4.7/ding/rl_utils/value_rescale.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     9477 2022-12-13 15:12:50.000000 DI-engine-0.4.7/ding/rl_utils/vtrace.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:01.827734 DI-engine-0.4.7/ding/torch_utils/
--rw-r--r--   0 niuyazhe (1370690143) 453037844      754 2023-03-09 11:08:49.000000 DI-engine-0.4.7/ding/torch_utils/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844      181 2023-04-11 05:01:52.000000 DI-engine-0.4.7/ding/torch_utils/backend_helper.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    12831 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/torch_utils/checkpoint_helper.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    14581 2023-03-09 11:08:49.000000 DI-engine-0.4.7/ding/torch_utils/data_helper.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844      358 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/torch_utils/dataparallel.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     9024 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/torch_utils/distribution.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:01.830692 DI-engine-0.4.7/ding/torch_utils/loss/
--rw-r--r--   0 niuyazhe (1370690143) 453037844      178 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/torch_utils/loss/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     4196 2023-01-28 12:50:23.000000 DI-engine-0.4.7/ding/torch_utils/loss/contrastive_loss.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2514 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/torch_utils/loss/cross_entropy_loss.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     4820 2023-01-02 10:31:34.000000 DI-engine-0.4.7/ding/torch_utils/loss/multi_logits_loss.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1273 2023-04-11 05:01:52.000000 DI-engine-0.4.7/ding/torch_utils/lr_scheduler.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1648 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/torch_utils/math_helper.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     3278 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/torch_utils/metric.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844      210 2023-04-11 05:01:52.000000 DI-engine-0.4.7/ding/torch_utils/model_helper.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:01.840197 DI-engine-0.4.7/ding/torch_utils/network/
--rw-r--r--   0 niuyazhe (1370690143) 453037844      678 2023-04-11 05:01:52.000000 DI-engine-0.4.7/ding/torch_utils/network/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     3769 2023-04-11 05:01:52.000000 DI-engine-0.4.7/ding/torch_utils/network/activation.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    35769 2022-01-21 07:34:18.000000 DI-engine-0.4.7/ding/torch_utils/network/coverage.xml
--rw-r--r--   0 niuyazhe (1370690143) 453037844    25400 2022-07-19 08:28:37.000000 DI-engine-0.4.7/ding/torch_utils/network/gtrxl.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1808 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/torch_utils/network/gumbel_softmax.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    25613 2022-10-19 09:16:29.000000 DI-engine-0.4.7/ding/torch_utils/network/nn_module.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1264 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/torch_utils/network/normalization.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     4429 2023-04-11 05:01:52.000000 DI-engine-0.4.7/ding/torch_utils/network/popart.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     5688 2022-10-19 09:16:29.000000 DI-engine-0.4.7/ding/torch_utils/network/res_block.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    21848 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/torch_utils/network/resnet.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    13797 2023-04-11 05:01:48.000000 DI-engine-0.4.7/ding/torch_utils/network/rnn.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     3626 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/torch_utils/network/scatter_connection.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1687 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/torch_utils/network/soft_argmax.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     8667 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/torch_utils/network/transformer.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1836 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/torch_utils/nn_test_helper.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    34698 2023-04-11 05:01:52.000000 DI-engine-0.4.7/ding/torch_utils/optimizer_helper.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     3018 2022-08-02 16:56:36.000000 DI-engine-0.4.7/ding/torch_utils/reshape_helper.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:01.858731 DI-engine-0.4.7/ding/utils/
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2609 2023-03-09 11:08:49.000000 DI-engine-0.4.7/ding/utils/__init__.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:01.861996 DI-engine-0.4.7/ding/utils/autolog/
--rw-r--r--   0 niuyazhe (1370690143) 453037844      236 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/utils/autolog/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844      701 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/utils/autolog/base.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     5499 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/utils/autolog/data.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     9391 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/utils/autolog/model.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:01.864211 DI-engine-0.4.7/ding/utils/autolog/tests/
--rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/utils/autolog/tests/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2304 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/utils/autolog/tests/test_data.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    17237 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/utils/autolog/tests/test_model.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     3452 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/utils/autolog/tests/test_time.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     5855 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/utils/autolog/time_ctl.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1407 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/utils/autolog/value.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2264 2023-03-09 11:08:49.000000 DI-engine-0.4.7/ding/utils/bfs_helper.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844      818 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/utils/collection_helper.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     4942 2023-02-13 06:43:00.000000 DI-engine-0.4.7/ding/utils/compression_helper.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844   179593 2021-10-17 09:03:07.000000 DI-engine-0.4.7/ding/utils/coverage.xml
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:01.867339 DI-engine-0.4.7/ding/utils/data/
--rw-r--r--   0 niuyazhe (1370690143) 453037844      284 2023-03-06 03:18:03.000000 DI-engine-0.4.7/ding/utils/data/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1052 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/utils/data/base_dataloader.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    11055 2023-04-11 05:01:52.000000 DI-engine-0.4.7/ding/utils/data/collate_fn.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    17023 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/utils/data/dataloader.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    22901 2023-03-09 11:08:49.000000 DI-engine-0.4.7/ding/utils/data/dataset.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:01.869230 DI-engine-0.4.7/ding/utils/data/structure/
--rw-r--r--   0 niuyazhe (1370690143) 453037844       59 2022-12-13 15:12:50.000000 DI-engine-0.4.7/ding/utils/data/structure/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     5297 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/utils/data/structure/cache.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844      300 2022-12-13 15:12:50.000000 DI-engine-0.4.7/ding/utils/data/structure/lifo_deque.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    19782 2022-10-19 09:16:29.000000 DI-engine-0.4.7/ding/utils/default_helper.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844      650 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/utils/design_helper.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844      344 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/utils/fake_linklink.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1480 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/utils/fast_copy.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    10416 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/utils/file_helper.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2897 2022-10-19 09:16:29.000000 DI-engine-0.4.7/ding/utils/import_helper.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     7063 2022-10-19 09:16:29.000000 DI-engine-0.4.7/ding/utils/k8s_helper.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     5414 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/utils/linklink_dist_helper.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:01.876961 DI-engine-0.4.7/ding/utils/loader/
--rw-r--r--   0 niuyazhe (1370690143) 453037844      783 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/utils/loader/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     4306 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/utils/loader/base.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     3043 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/utils/loader/collection.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844      871 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/utils/loader/dict.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844      369 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/utils/loader/exception.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     3093 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/utils/loader/mapping.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     5747 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/utils/loader/norm.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     6391 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/utils/loader/number.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2228 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/utils/loader/string.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:01.877907 DI-engine-0.4.7/ding/utils/loader/tests/
--rw-r--r--   0 niuyazhe (1370690143) 453037844      111 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/utils/loader/tests/__init__.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:01.883044 DI-engine-0.4.7/ding/utils/loader/tests/loader/
--rw-r--r--   0 niuyazhe (1370690143) 453037844      426 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/utils/loader/tests/loader/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     5225 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/utils/loader/tests/loader/test_base.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     5989 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/utils/loader/tests/loader/test_collection.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1090 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/utils/loader/tests/loader/test_dict.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1914 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/utils/loader/tests/loader/test_mapping.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    11175 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/utils/loader/tests/loader/test_norm.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    21822 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/utils/loader/tests/loader/test_number.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     4119 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/utils/loader/tests/loader/test_string.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     3183 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/utils/loader/tests/loader/test_types.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1478 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/utils/loader/tests/loader/test_utils.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     4334 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/utils/loader/tests/test_cartpole_dqn_serial_config_loader.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1366 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/utils/loader/types.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844      409 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/utils/loader/utils.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2796 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/utils/lock_helper.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     5332 2022-11-14 04:31:11.000000 DI-engine-0.4.7/ding/utils/log_helper.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     4397 2022-10-19 10:55:38.000000 DI-engine-0.4.7/ding/utils/log_writer_helper.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     4657 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/utils/orchestrator_launcher.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1135 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/utils/profiler_helper.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     3999 2022-12-13 15:12:50.000000 DI-engine-0.4.7/ding/utils/pytorch_ddp_dist_helper.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     3853 2023-01-02 16:52:37.000000 DI-engine-0.4.7/ding/utils/registry.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1495 2022-10-19 09:16:29.000000 DI-engine-0.4.7/ding/utils/registry_factory.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1525 2022-08-02 16:56:36.000000 DI-engine-0.4.7/ding/utils/render_helper.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     7572 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/utils/scheduler_helper.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     9207 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/utils/segment_tree.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2855 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/utils/slurm_helper.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1743 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/utils/system_helper.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     4522 2023-03-09 11:08:49.000000 DI-engine-0.4.7/ding/utils/time_helper.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844      956 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/utils/time_helper_base.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1908 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/utils/time_helper_cuda.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844      173 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/utils/type_helper.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:01.883542 DI-engine-0.4.7/ding/worker/
--rw-r--r--   0 niuyazhe (1370690143) 453037844      127 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/worker/__init__.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:01.884681 DI-engine-0.4.7/ding/worker/adapter/
--rw-r--r--   0 niuyazhe (1370690143) 453037844       50 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/worker/adapter/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    13378 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/worker/adapter/learner_aggregator.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:01.892613 DI-engine-0.4.7/ding/worker/collector/
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1080 2022-10-19 09:16:29.000000 DI-engine-0.4.7/ding/worker/collector/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     8862 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/worker/collector/base_parallel_collector.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     7839 2023-04-11 13:59:56.000000 DI-engine-0.4.7/ding/worker/collector/base_serial_collector.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     8544 2022-12-26 08:59:29.000000 DI-engine-0.4.7/ding/worker/collector/base_serial_evaluator.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    15584 2023-04-11 13:59:56.000000 DI-engine-0.4.7/ding/worker/collector/battle_episode_serial_collector.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    12112 2023-03-09 11:08:49.000000 DI-engine-0.4.7/ding/worker/collector/battle_interaction_serial_evaluator.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    16387 2023-04-11 13:59:56.000000 DI-engine-0.4.7/ding/worker/collector/battle_sample_serial_collector.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:01.895072 DI-engine-0.4.7/ding/worker/collector/comm/
--rw-r--r--   0 niuyazhe (1370690143) 453037844      177 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/worker/collector/comm/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     4089 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/worker/collector/comm/base_comm_collector.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     8874 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/worker/collector/comm/flask_fs_collector.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2436 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/worker/collector/comm/utils.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    14757 2023-04-11 13:59:56.000000 DI-engine-0.4.7/ding/worker/collector/episode_serial_collector.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    13972 2023-03-09 11:08:49.000000 DI-engine-0.4.7/ding/worker/collector/interaction_serial_evaluator.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    14421 2022-12-13 15:12:50.000000 DI-engine-0.4.7/ding/worker/collector/marine_parallel_collector.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     9156 2022-12-13 15:12:50.000000 DI-engine-0.4.7/ding/worker/collector/metric_serial_evaluator.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    17601 2023-04-11 13:59:56.000000 DI-engine-0.4.7/ding/worker/collector/sample_serial_collector.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:01.898415 DI-engine-0.4.7/ding/worker/collector/tests/
--rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/worker/collector/tests/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844      698 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/worker/collector/tests/fake_cls_policy.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2804 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/worker/collector/tests/fake_cpong_dqn_config.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:01.900350 DI-engine-0.4.7/ding/worker/collector/tests/speed_test/
--rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/worker/collector/tests/speed_test/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2917 2022-12-13 15:12:50.000000 DI-engine-0.4.7/ding/worker/collector/tests/speed_test/fake_env.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     3034 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/worker/collector/tests/speed_test/fake_policy.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     7399 2023-01-02 10:31:34.000000 DI-engine-0.4.7/ding/worker/collector/tests/speed_test/test_collector_profile.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844      107 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/worker/collector/tests/speed_test/utils.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1705 2023-04-11 13:59:56.000000 DI-engine-0.4.7/ding/worker/collector/tests/test_base_serial_collector.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2277 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/worker/collector/tests/test_episode_serial_collector.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2846 2022-12-13 15:12:50.000000 DI-engine-0.4.7/ding/worker/collector/tests/test_marine_parallel_collector.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     3019 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/worker/collector/tests/test_metric_serial_evaluator.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    11723 2023-04-05 10:04:48.000000 DI-engine-0.4.7/ding/worker/collector/zergling_parallel_collector.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:01.904477 DI-engine-0.4.7/ding/worker/coordinator/
--rw-r--r--   0 niuyazhe (1370690143) 453037844      183 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/worker/coordinator/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     7099 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/worker/coordinator/base_parallel_commander.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2070 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/worker/coordinator/base_serial_commander.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    26271 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/worker/coordinator/comm_coordinator.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    20584 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/worker/coordinator/coordinator.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    16808 2022-12-13 15:12:50.000000 DI-engine-0.4.7/ding/worker/coordinator/one_vs_one_parallel_commander.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     3634 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/worker/coordinator/operator_server.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2675 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/worker/coordinator/resource_manager.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    10871 2022-12-13 15:12:50.000000 DI-engine-0.4.7/ding/worker/coordinator/solo_parallel_commander.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:01.906364 DI-engine-0.4.7/ding/worker/learner/
--rw-r--r--   0 niuyazhe (1370690143) 453037844      252 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/worker/learner/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    20149 2022-12-13 15:12:50.000000 DI-engine-0.4.7/ding/worker/learner/base_learner.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:01.908700 DI-engine-0.4.7/ding/worker/learner/comm/
--rw-r--r--   0 niuyazhe (1370690143) 453037844      165 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/worker/learner/comm/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     4937 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/worker/learner/comm/base_comm_learner.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    15576 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/worker/learner/comm/flask_fs_learner.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2120 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/worker/learner/comm/utils.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    15500 2022-10-19 09:16:29.000000 DI-engine-0.4.7/ding/worker/learner/learner_hook.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:01.913742 DI-engine-0.4.7/ding/worker/replay_buffer/
--rw-r--r--   0 niuyazhe (1370690143) 453037844      206 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/worker/replay_buffer/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    37630 2023-04-05 10:04:48.000000 DI-engine-0.4.7/ding/worker/replay_buffer/advanced_buffer.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     4460 2022-12-11 15:35:39.000000 DI-engine-0.4.7/ding/worker/replay_buffer/base_buffer.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844      800 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/worker/replay_buffer/episode_buffer.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    19279 2022-12-11 15:35:39.000000 DI-engine-0.4.7/ding/worker/replay_buffer/naive_buffer.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    10920 2022-09-30 04:52:24.000000 DI-engine-0.4.7/ding/worker/replay_buffer/utils.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:01.917728 DI-engine-0.4.7/ding/world_model/
--rw-r--r--   0 niuyazhe (1370690143) 453037844      139 2022-07-19 08:28:37.000000 DI-engine-0.4.7/ding/world_model/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    13985 2022-08-02 16:56:36.000000 DI-engine-0.4.7/ding/world_model/base_world_model.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    22524 2022-08-02 16:56:36.000000 DI-engine-0.4.7/ding/world_model/ddppo.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     6228 2022-10-19 09:16:29.000000 DI-engine-0.4.7/ding/world_model/idm.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    11421 2022-08-02 16:56:36.000000 DI-engine-0.4.7/ding/world_model/mbpo.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844      852 2022-07-19 08:28:37.000000 DI-engine-0.4.7/ding/world_model/utils.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:01.918302 DI-engine-0.4.7/dizoo/
--rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2023-03-22 09:07:56.000000 DI-engine-0.4.7/dizoo/__init__.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:01.918513 DI-engine-0.4.7/dizoo/atari/
--rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2022-09-30 04:52:24.000000 DI-engine-0.4.7/dizoo/atari/__init__.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:01.918712 DI-engine-0.4.7/dizoo/atari/config/
--rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2022-09-30 04:52:24.000000 DI-engine-0.4.7/dizoo/atari/config/__init__.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:01.919007 DI-engine-0.4.7/dizoo/atari/config/serial/
--rw-r--r--   0 niuyazhe (1370690143) 453037844      239 2023-03-09 11:08:49.000000 DI-engine-0.4.7/dizoo/atari/config/serial/__init__.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:01.920262 DI-engine-0.4.7/dizoo/atari/config/serial/asterix/
--rw-r--r--   0 niuyazhe (1370690143) 453037844       82 2023-03-09 11:08:49.000000 DI-engine-0.4.7/dizoo/atari/config/serial/asterix/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1913 2023-03-09 11:08:49.000000 DI-engine-0.4.7/dizoo/atari/config/serial/asterix/asterix_mdqn_config.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:01.923986 DI-engine-0.4.7/dizoo/atari/config/serial/enduro/
--rw-r--r--   0 niuyazhe (1370690143) 453037844       76 2022-07-19 08:28:37.000000 DI-engine-0.4.7/dizoo/atari/config/serial/enduro/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1731 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/atari/config/serial/enduro/enduro_dqn_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2976 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/atari/config/serial/enduro/enduro_impala_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1900 2023-03-09 11:08:49.000000 DI-engine-0.4.7/dizoo/atari/config/serial/enduro/enduro_mdqn_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2237 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/atari/config/serial/enduro/enduro_onppo_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1758 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/atari/config/serial/enduro/enduro_qrdqn_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1816 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/atari/config/serial/enduro/enduro_rainbow_config.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:01.940359 DI-engine-0.4.7/dizoo/atari/config/serial/pong/
--rw-r--r--   0 niuyazhe (1370690143) 453037844      233 2022-07-19 08:28:37.000000 DI-engine-0.4.7/dizoo/atari/config/serial/pong/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2064 2022-12-13 15:12:50.000000 DI-engine-0.4.7/dizoo/atari/config/serial/pong/pong_a2c_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2480 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/atari/config/serial/pong/pong_acer_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1742 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/atari/config/serial/pong/pong_c51_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2123 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/atari/config/serial/pong/pong_cql_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2877 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/atari/config/serial/pong/pong_dqfd_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1673 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/atari/config/serial/pong/pong_dqn_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1853 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/atari/config/serial/pong/pong_dqn_envpool_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1707 2023-04-05 10:04:48.000000 DI-engine-0.4.7/dizoo/atari/config/serial/pong/pong_dqn_multi_gpu_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1814 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/atari/config/serial/pong/pong_dqn_render_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1975 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/atari/config/serial/pong/pong_dqn_stdim_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1784 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/atari/config/serial/pong/pong_fqf_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     3109 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/atari/config/serial/pong/pong_gail_dqn_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2735 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/atari/config/serial/pong/pong_impala_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1724 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/atari/config/serial/pong/pong_iqn_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     4989 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/atari/config/serial/pong/pong_ngu_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2137 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/atari/config/serial/pong/pong_onppo_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2615 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/atari/config/serial/pong/pong_ppg_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1726 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/atari/config/serial/pong/pong_qrdqn_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2065 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/atari/config/serial/pong/pong_qrdqn_generation_data_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     3300 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/atari/config/serial/pong/pong_r2d2_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     3011 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/atari/config/serial/pong/pong_r2d2_gtrxl_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     3017 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/atari/config/serial/pong/pong_r2d2_residual_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     6446 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/atari/config/serial/pong/pong_r2d3_offppoexpert_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     6795 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/atari/config/serial/pong/pong_r2d3_r2d2expert_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1729 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/atari/config/serial/pong/pong_rainbow_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2290 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/atari/config/serial/pong/pong_sqil_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1571 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/atari/config/serial/pong/pong_sql_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     4218 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/atari/config/serial/pong/pong_trex_offppo_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     3561 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/atari/config/serial/pong/pong_trex_sql_config.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:01.951523 DI-engine-0.4.7/dizoo/atari/config/serial/qbert/
--rw-r--r--   0 niuyazhe (1370690143) 453037844      146 2022-07-19 08:28:37.000000 DI-engine-0.4.7/dizoo/atari/config/serial/qbert/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2058 2022-12-13 15:12:50.000000 DI-engine-0.4.7/dizoo/atari/config/serial/qbert/qbert_a2c_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2541 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/atari/config/serial/qbert/qbert_acer_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1669 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/atari/config/serial/qbert/qbert_c51_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2076 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/atari/config/serial/qbert/qbert_cql_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2732 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/atari/config/serial/qbert/qbert_dqfd_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1687 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/atari/config/serial/qbert/qbert_dqn_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1844 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/atari/config/serial/qbert/qbert_fqf_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2808 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/atari/config/serial/qbert/qbert_impala_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1650 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/atari/config/serial/qbert/qbert_iqn_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2154 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/atari/config/serial/qbert/qbert_offppo_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2184 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/atari/config/serial/qbert/qbert_onppo_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2459 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/atari/config/serial/qbert/qbert_ppg_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1645 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/atari/config/serial/qbert/qbert_qrdqn_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2073 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/atari/config/serial/qbert/qbert_qrdqn_generation_data_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     3387 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/atari/config/serial/qbert/qbert_r2d2_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2760 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/atari/config/serial/qbert/qbert_r2d2_gtrxl_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1757 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/atari/config/serial/qbert/qbert_rainbow_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2415 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/atari/config/serial/qbert/qbert_sqil_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1684 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/atari/config/serial/qbert/qbert_sql_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     3001 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/atari/config/serial/qbert/qbert_trex_dqn_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     3442 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/atari/config/serial/qbert/qbert_trex_offppo_config.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:01.964896 DI-engine-0.4.7/dizoo/atari/config/serial/spaceinvaders/
--rw-r--r--   0 niuyazhe (1370690143) 453037844      194 2022-07-19 08:28:37.000000 DI-engine-0.4.7/dizoo/atari/config/serial/spaceinvaders/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2266 2022-12-13 15:12:50.000000 DI-engine-0.4.7/dizoo/atari/config/serial/spaceinvaders/spaceinvaders_a2c_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2811 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/atari/config/serial/spaceinvaders/spaceinvaders_acer_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1937 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/atari/config/serial/spaceinvaders/spaceinvaders_c51_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2925 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/atari/config/serial/spaceinvaders/spaceinvaders_dqfd_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2029 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/atari/config/serial/spaceinvaders/spaceinvaders_dqn_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1891 2023-04-05 10:04:48.000000 DI-engine-0.4.7/dizoo/atari/config/serial/spaceinvaders/spaceinvaders_dqn_config_multi_gpu_ddp.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1978 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/atari/config/serial/spaceinvaders/spaceinvaders_dqn_config_multi_gpu_dp.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1939 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/atari/config/serial/spaceinvaders/spaceinvaders_fqf_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     3105 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/atari/config/serial/spaceinvaders/spaceinvaders_impala_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1909 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/atari/config/serial/spaceinvaders/spaceinvaders_iqn_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1979 2023-03-09 11:08:49.000000 DI-engine-0.4.7/dizoo/atari/config/serial/spaceinvaders/spaceinvaders_mdqn_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2395 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/atari/config/serial/spaceinvaders/spaceinvaders_offppo_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2310 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/atari/config/serial/spaceinvaders/spaceinvaders_onppo_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2716 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/atari/config/serial/spaceinvaders/spaceinvaders_ppg_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1912 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/atari/config/serial/spaceinvaders/spaceinvaders_qrdqn_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     3492 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/atari/config/serial/spaceinvaders/spaceinvaders_r2d2_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     3033 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/atari/config/serial/spaceinvaders/spaceinvaders_r2d2_gtrxl_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     3167 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/atari/config/serial/spaceinvaders/spaceinvaders_r2d2_residual_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2031 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/atari/config/serial/spaceinvaders/spaceinvaders_rainbow_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2516 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/atari/config/serial/spaceinvaders/spaceinvaders_sqil_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1827 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/atari/config/serial/spaceinvaders/spaceinvaders_sql_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     4055 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/atari/config/serial/spaceinvaders/spaceinvaders_trex_dqn_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     4554 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/atari/config/serial/spaceinvaders/spaceinvaders_trex_offppo_config.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:01.972164 DI-engine-0.4.7/dizoo/atari/entry/
--rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2022-09-30 04:52:24.000000 DI-engine-0.4.7/dizoo/atari/entry/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     3135 2022-09-30 04:52:24.000000 DI-engine-0.4.7/dizoo/atari/entry/atari_dqn_main.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     3534 2022-09-30 04:52:24.000000 DI-engine-0.4.7/dizoo/atari/entry/atari_ppg_main.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     3272 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/atari/entry/phoenix_fqf_main.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     3272 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/atari/entry/phoenix_iqn_main.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2118 2022-09-30 04:52:24.000000 DI-engine-0.4.7/dizoo/atari/entry/pong_cql_main.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     3743 2022-07-19 08:28:38.000000 DI-engine-0.4.7/dizoo/atari/entry/pong_dqn_envpool_main.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     3260 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/atari/entry/pong_fqf_main.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2151 2022-09-30 04:52:24.000000 DI-engine-0.4.7/dizoo/atari/entry/qbert_cql_main.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     3264 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/atari/entry/qbert_fqf_main.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2185 2022-12-13 15:12:50.000000 DI-engine-0.4.7/dizoo/atari/entry/spaceinvaders_dqn_eval.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     3251 2022-09-30 04:52:24.000000 DI-engine-0.4.7/dizoo/atari/entry/spaceinvaders_dqn_main_multi_gpu_ddp.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     3261 2022-09-30 04:52:24.000000 DI-engine-0.4.7/dizoo/atari/entry/spaceinvaders_dqn_main_multi_gpu_dp.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     3296 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/atari/entry/spaceinvaders_fqf_main.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:01.974573 DI-engine-0.4.7/dizoo/atari/envs/
--rw-r--r--   0 niuyazhe (1370690143) 453037844       44 2022-09-30 04:52:24.000000 DI-engine-0.4.7/dizoo/atari/envs/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     5233 2022-12-13 15:12:50.000000 DI-engine-0.4.7/dizoo/atari/envs/atari_env.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     6246 2022-11-14 04:31:11.000000 DI-engine-0.4.7/dizoo/atari/envs/atari_wrappers.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2440 2022-12-13 15:12:50.000000 DI-engine-0.4.7/dizoo/atari/envs/test_atari_env.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:01.975077 DI-engine-0.4.7/dizoo/beergame/
--rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2023-01-17 12:06:07.000000 DI-engine-0.4.7/dizoo/beergame/__init__.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:01.979485 DI-engine-0.4.7/dizoo/beergame/envs/
--rw-r--r--   0 niuyazhe (1370690143) 453037844     8359 2022-12-13 15:12:50.000000 DI-engine-0.4.7/dizoo/beergame/envs/BGAgent.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844       71 2022-11-14 04:31:11.000000 DI-engine-0.4.7/dizoo/beergame/envs/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     4738 2022-11-14 04:31:11.000000 DI-engine-0.4.7/dizoo/beergame/envs/beergame_core.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     3046 2022-12-13 15:12:50.000000 DI-engine-0.4.7/dizoo/beergame/envs/beergame_env.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    23724 2022-11-14 04:31:11.000000 DI-engine-0.4.7/dizoo/beergame/envs/clBeergame.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2721 2022-11-14 04:31:11.000000 DI-engine-0.4.7/dizoo/beergame/envs/plotting.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    17343 2022-11-14 04:31:11.000000 DI-engine-0.4.7/dizoo/beergame/envs/utils.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:01.980276 DI-engine-0.4.7/dizoo/bitflip/
--rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2022-03-14 08:09:40.000000 DI-engine-0.4.7/dizoo/bitflip/__init__.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:01.982118 DI-engine-0.4.7/dizoo/bitflip/config/
--rw-r--r--   0 niuyazhe (1370690143) 453037844      183 2022-09-30 04:52:24.000000 DI-engine-0.4.7/dizoo/bitflip/config/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2616 2022-09-30 04:52:24.000000 DI-engine-0.4.7/dizoo/bitflip/config/bitflip_her_dqn_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1740 2022-09-30 04:52:24.000000 DI-engine-0.4.7/dizoo/bitflip/config/bitflip_pure_dqn_config.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:01.982927 DI-engine-0.4.7/dizoo/bitflip/entry/
--rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2022-03-14 08:09:40.000000 DI-engine-0.4.7/dizoo/bitflip/entry/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     4350 2022-09-30 04:52:24.000000 DI-engine-0.4.7/dizoo/bitflip/entry/bitflip_dqn_main.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:01.986980 DI-engine-0.4.7/dizoo/bitflip/envs/
--rw-r--r--   0 niuyazhe (1370690143) 453037844       36 2022-09-30 04:52:24.000000 DI-engine-0.4.7/dizoo/bitflip/envs/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     3261 2022-12-13 15:12:50.000000 DI-engine-0.4.7/dizoo/bitflip/envs/bitflip_env.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844      756 2022-09-30 04:52:24.000000 DI-engine-0.4.7/dizoo/bitflip/envs/test_bitfilp_env.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:01.987629 DI-engine-0.4.7/dizoo/box2d/
--rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2022-09-30 04:52:24.000000 DI-engine-0.4.7/dizoo/box2d/__init__.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:01.987856 DI-engine-0.4.7/dizoo/box2d/bipedalwalker/
--rw-r--r--   0 niuyazhe (1370690143) 453037844       47 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/box2d/bipedalwalker/__init__.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:01.993291 DI-engine-0.4.7/dizoo/box2d/bipedalwalker/config/
--rw-r--r--   0 niuyazhe (1370690143) 453037844       96 2022-07-19 08:28:38.000000 DI-engine-0.4.7/dizoo/box2d/bipedalwalker/config/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     3050 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/box2d/bipedalwalker/config/bipedalwalker_bco_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2504 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/box2d/bipedalwalker/config/bipedalwalker_dt_config.py
--rwxr-xr-x   0 niuyazhe (1370690143) 453037844     3504 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/box2d/bipedalwalker/config/bipedalwalker_gail_sac_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2819 2022-12-13 15:12:50.000000 DI-engine-0.4.7/dizoo/box2d/bipedalwalker/config/bipedalwalker_impala_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1837 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/box2d/bipedalwalker/config/bipedalwalker_ppo_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2644 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/box2d/bipedalwalker/config/bipedalwalker_ppopg_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2078 2022-09-30 04:52:24.000000 DI-engine-0.4.7/dizoo/box2d/bipedalwalker/config/bipedalwalker_sac_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2135 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/box2d/bipedalwalker/config/bipedalwalker_td3_config.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:01.994032 DI-engine-0.4.7/dizoo/box2d/bipedalwalker/entry/
--rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/box2d/bipedalwalker/entry/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2181 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/box2d/bipedalwalker/entry/bipedalwalker_ppo_eval.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:01.995691 DI-engine-0.4.7/dizoo/box2d/bipedalwalker/envs/
--rw-r--r--   0 niuyazhe (1370690143) 453037844       48 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/box2d/bipedalwalker/envs/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     3868 2022-12-13 15:12:50.000000 DI-engine-0.4.7/dizoo/box2d/bipedalwalker/envs/bipedalwalker_env.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1034 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/box2d/bipedalwalker/envs/test_bipedalwalker.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:01.996237 DI-engine-0.4.7/dizoo/box2d/carracing/
--rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2023-02-13 06:42:54.000000 DI-engine-0.4.7/dizoo/box2d/carracing/__init__.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:01.997046 DI-engine-0.4.7/dizoo/box2d/carracing/config/
--rw-r--r--   0 niuyazhe (1370690143) 453037844       85 2023-02-13 06:42:54.000000 DI-engine-0.4.7/dizoo/box2d/carracing/config/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1767 2023-02-13 06:42:54.000000 DI-engine-0.4.7/dizoo/box2d/carracing/config/carracing_dqn_config.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:01.998957 DI-engine-0.4.7/dizoo/box2d/carracing/envs/
--rw-r--r--   0 niuyazhe (1370690143) 453037844       41 2023-02-13 06:42:54.000000 DI-engine-0.4.7/dizoo/box2d/carracing/envs/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     5913 2023-02-13 06:42:54.000000 DI-engine-0.4.7/dizoo/box2d/carracing/envs/carracing_env.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1082 2023-02-13 06:42:54.000000 DI-engine-0.4.7/dizoo/box2d/carracing/envs/test_carracing_env.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:01.999446 DI-engine-0.4.7/dizoo/box2d/lunarlander/
--rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/box2d/lunarlander/__init__.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:02.019260 DI-engine-0.4.7/dizoo/box2d/lunarlander/config/
--rw-r--r--   0 niuyazhe (1370690143) 453037844      597 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/box2d/lunarlander/config/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1375 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/box2d/lunarlander/config/lunarlander_a2c_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     3181 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/box2d/lunarlander/config/lunarlander_acer_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2827 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/box2d/lunarlander/config/lunarlander_bco_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1671 2023-04-05 10:04:48.000000 DI-engine-0.4.7/dizoo/box2d/lunarlander/config/lunarlander_c51_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2418 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/box2d/lunarlander/config/lunarlander_cont_ddpg_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1677 2023-04-05 10:04:48.000000 DI-engine-0.4.7/dizoo/box2d/lunarlander/config/lunarlander_cont_sac_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1817 2023-04-05 10:04:48.000000 DI-engine-0.4.7/dizoo/box2d/lunarlander/config/lunarlander_cont_td3_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2269 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/box2d/lunarlander/config/lunarlander_cont_td3_vae_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2484 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/box2d/lunarlander/config/lunarlander_decision_transformer.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2086 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/box2d/lunarlander/config/lunarlander_discrete_sac_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2888 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/box2d/lunarlander/config/lunarlander_dqfd_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2636 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/box2d/lunarlander/config/lunarlander_dqn_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2541 2023-04-05 10:04:48.000000 DI-engine-0.4.7/dizoo/box2d/lunarlander/config/lunarlander_dqn_deque_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     3962 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/box2d/lunarlander/config/lunarlander_gail_dqn_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2272 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/box2d/lunarlander/config/lunarlander_gcl_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     5345 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/box2d/lunarlander/config/lunarlander_ngu_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1502 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/box2d/lunarlander/config/lunarlander_offppo_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1381 2022-12-11 15:35:39.000000 DI-engine-0.4.7/dizoo/box2d/lunarlander/config/lunarlander_pg_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1530 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/box2d/lunarlander/config/lunarlander_qrdqn_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     3325 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/box2d/lunarlander/config/lunarlander_r2d2_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     3056 2022-07-19 08:28:38.000000 DI-engine-0.4.7/dizoo/box2d/lunarlander/config/lunarlander_r2d2_gtrxl_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     6624 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/box2d/lunarlander/config/lunarlander_r2d3_ppoexpert_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     6992 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/box2d/lunarlander/config/lunarlander_r2d3_r2d2expert_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2612 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/box2d/lunarlander/config/lunarlander_rnd_onppo_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2498 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/box2d/lunarlander/config/lunarlander_sqil_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1623 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/box2d/lunarlander/config/lunarlander_sql_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     4289 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/box2d/lunarlander/config/lunarlander_trex_dqn_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     3462 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/box2d/lunarlander/config/lunarlander_trex_offppo_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     8211 2022-09-28 13:14:17.000000 DI-engine-0.4.7/dizoo/box2d/lunarlander/config/t.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:02.021601 DI-engine-0.4.7/dizoo/box2d/lunarlander/entry/
--rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/box2d/lunarlander/entry/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2177 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/box2d/lunarlander/entry/lunarlander_dqn_eval.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2985 2023-02-13 06:56:00.000000 DI-engine-0.4.7/dizoo/box2d/lunarlander/entry/lunarlander_dqn_example.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:02.024178 DI-engine-0.4.7/dizoo/box2d/lunarlander/envs/
--rw-r--r--   0 niuyazhe (1370690143) 453037844       44 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/box2d/lunarlander/envs/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     5535 2022-12-13 15:12:50.000000 DI-engine-0.4.7/dizoo/box2d/lunarlander/envs/lunarlander_env.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1248 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/box2d/lunarlander/envs/test_lunarlander_env.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:02.025100 DI-engine-0.4.7/dizoo/bsuite/
--rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/bsuite/__init__.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:02.025453 DI-engine-0.4.7/dizoo/bsuite/config/
--rw-r--r--   0 niuyazhe (1370690143) 453037844        1 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/bsuite/config/__init__.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:02.028695 DI-engine-0.4.7/dizoo/bsuite/envs/
--rw-r--r--   0 niuyazhe (1370690143) 453037844       34 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/bsuite/envs/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     3752 2022-12-13 15:12:50.000000 DI-engine-0.4.7/dizoo/bsuite/envs/bsuite_env.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1467 2022-12-13 15:12:50.000000 DI-engine-0.4.7/dizoo/bsuite/envs/test_bsuite_env.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:02.030197 DI-engine-0.4.7/dizoo/classic_control/
--rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/classic_control/__init__.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:02.030525 DI-engine-0.4.7/dizoo/classic_control/acrobot/
--rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2023-02-13 06:42:54.000000 DI-engine-0.4.7/dizoo/classic_control/acrobot/__init__.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:02.031610 DI-engine-0.4.7/dizoo/classic_control/acrobot/config/
--rw-r--r--   0 niuyazhe (1370690143) 453037844       79 2023-02-13 06:42:54.000000 DI-engine-0.4.7/dizoo/classic_control/acrobot/config/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1659 2023-02-13 06:42:54.000000 DI-engine-0.4.7/dizoo/classic_control/acrobot/config/acrobot_dqn_config.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:02.033813 DI-engine-0.4.7/dizoo/classic_control/acrobot/envs/
--rw-r--r--   0 niuyazhe (1370690143) 453037844       37 2023-02-13 06:42:54.000000 DI-engine-0.4.7/dizoo/classic_control/acrobot/envs/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     3591 2023-02-13 06:42:54.000000 DI-engine-0.4.7/dizoo/classic_control/acrobot/envs/acrobot_env.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1323 2023-02-13 06:42:54.000000 DI-engine-0.4.7/dizoo/classic_control/acrobot/envs/test_acrobot_env.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:02.034435 DI-engine-0.4.7/dizoo/classic_control/cartpole/
--rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/classic_control/cartpole/__init__.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:02.068754 DI-engine-0.4.7/dizoo/classic_control/cartpole/config/
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2040 2023-03-09 11:08:49.000000 DI-engine-0.4.7/dizoo/classic_control/cartpole/config/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1682 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/classic_control/cartpole/config/cartpole_a2c_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2489 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/classic_control/cartpole/config/cartpole_acer_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1330 2023-02-13 06:42:54.000000 DI-engine-0.4.7/dizoo/classic_control/cartpole/config/cartpole_bc_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2524 2022-10-31 06:23:20.000000 DI-engine-0.4.7/dizoo/classic_control/cartpole/config/cartpole_bco_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1687 2023-01-06 07:05:23.000000 DI-engine-0.4.7/dizoo/classic_control/cartpole/config/cartpole_c51_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1649 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/classic_control/cartpole/config/cartpole_cql_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2585 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/classic_control/cartpole/config/cartpole_decision_transformer.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2849 2023-02-22 06:18:30.000000 DI-engine-0.4.7/dizoo/classic_control/cartpole/config/cartpole_dqfd_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1776 2023-02-22 06:18:46.000000 DI-engine-0.4.7/dizoo/classic_control/cartpole/config/cartpole_dqn_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2701 2022-10-31 06:23:20.000000 DI-engine-0.4.7/dizoo/classic_control/cartpole/config/cartpole_dqn_gail_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1556 2022-07-19 08:28:38.000000 DI-engine-0.4.7/dizoo/classic_control/cartpole/config/cartpole_dqn_rnd_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2055 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/classic_control/cartpole/config/cartpole_dqn_stdim_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     3173 2022-11-14 04:31:11.000000 DI-engine-0.4.7/dizoo/classic_control/cartpole/config/cartpole_drex_dqn_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1813 2022-07-19 08:28:38.000000 DI-engine-0.4.7/dizoo/classic_control/cartpole/config/cartpole_fqf_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2423 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/classic_control/cartpole/config/cartpole_gcl_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2781 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/classic_control/cartpole/config/cartpole_impala_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1649 2023-01-06 07:05:23.000000 DI-engine-0.4.7/dizoo/classic_control/cartpole/config/cartpole_iqn_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1721 2023-03-09 11:08:49.000000 DI-engine-0.4.7/dizoo/classic_control/cartpole/config/cartpole_mdqn_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     4857 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/classic_control/cartpole/config/cartpole_ngu_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1277 2022-12-11 15:35:39.000000 DI-engine-0.4.7/dizoo/classic_control/cartpole/config/cartpole_pg_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2357 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/classic_control/cartpole/config/cartpole_ppg_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1684 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/classic_control/cartpole/config/cartpole_ppo_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1894 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/classic_control/cartpole/config/cartpole_ppo_icm_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1797 2023-01-06 07:05:23.000000 DI-engine-0.4.7/dizoo/classic_control/cartpole/config/cartpole_ppo_offpolicy_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2084 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/classic_control/cartpole/config/cartpole_ppo_stdim_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1383 2022-12-11 15:35:39.000000 DI-engine-0.4.7/dizoo/classic_control/cartpole/config/cartpole_ppopg_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1672 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/classic_control/cartpole/config/cartpole_qrdqn_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1739 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/classic_control/cartpole/config/cartpole_qrdqn_generation_data_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2909 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/classic_control/cartpole/config/cartpole_r2d2_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2775 2022-07-19 08:28:38.000000 DI-engine-0.4.7/dizoo/classic_control/cartpole/config/cartpole_r2d2_gtrxl_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     3219 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/classic_control/cartpole/config/cartpole_r2d2_residual_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1664 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/classic_control/cartpole/config/cartpole_rainbow_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2245 2023-03-09 11:08:49.000000 DI-engine-0.4.7/dizoo/classic_control/cartpole/config/cartpole_rnd_onppo_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1998 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/classic_control/cartpole/config/cartpole_sac_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2258 2023-01-06 07:05:23.000000 DI-engine-0.4.7/dizoo/classic_control/cartpole/config/cartpole_sqil_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1554 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/classic_control/cartpole/config/cartpole_sql_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1702 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/classic_control/cartpole/config/cartpole_sqn_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2845 2023-01-06 07:05:23.000000 DI-engine-0.4.7/dizoo/classic_control/cartpole/config/cartpole_trex_dqn_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2948 2023-02-13 06:42:54.000000 DI-engine-0.4.7/dizoo/classic_control/cartpole/config/cartpole_trex_offppo_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     3044 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/classic_control/cartpole/config/cartpole_trex_onppo_config.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:02.071650 DI-engine-0.4.7/dizoo/classic_control/cartpole/config/parallel/
--rw-r--r--   0 niuyazhe (1370690143) 453037844      109 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/classic_control/cartpole/config/parallel/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2921 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/classic_control/cartpole/config/parallel/cartpole_dqn_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     3286 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/classic_control/cartpole/config/parallel/cartpole_dqn_config_k8s.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:02.082030 DI-engine-0.4.7/dizoo/classic_control/cartpole/entry/
--rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/classic_control/cartpole/entry/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1282 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/classic_control/cartpole/entry/cartpole_c51_deploy.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     3403 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/classic_control/cartpole/entry/cartpole_c51_main.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2217 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/classic_control/cartpole/entry/cartpole_cql_main.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     3391 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/classic_control/cartpole/entry/cartpole_dqn_buffer_main.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2014 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/classic_control/cartpole/entry/cartpole_dqn_eval.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     3857 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/classic_control/cartpole/entry/cartpole_dqn_main.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     3959 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/classic_control/cartpole/entry/cartpole_fqf_main.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     3582 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/classic_control/cartpole/entry/cartpole_ppg_main.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2278 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/classic_control/cartpole/entry/cartpole_ppo_main.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2781 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/classic_control/cartpole/entry/cartpole_ppo_offpolicy_main.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2470 2021-07-16 08:07:45.000000 DI-engine-0.4.7/dizoo/classic_control/cartpole/entry/formatted_total_config.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:02.085971 DI-engine-0.4.7/dizoo/classic_control/cartpole/envs/
--rw-r--r--   0 niuyazhe (1370690143) 453037844       38 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/classic_control/cartpole/envs/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     3774 2022-12-13 15:12:50.000000 DI-engine-0.4.7/dizoo/classic_control/cartpole/envs/cartpole_env.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1327 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/classic_control/cartpole/envs/test_cartpole_env.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1350 2022-07-19 08:28:38.000000 DI-engine-0.4.7/dizoo/classic_control/cartpole/envs/test_cartpole_env_manager.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:02.086937 DI-engine-0.4.7/dizoo/classic_control/mountain_car/
--rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/classic_control/mountain_car/__init__.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:02.089474 DI-engine-0.4.7/dizoo/classic_control/mountain_car/envs/
--rw-r--r--   0 niuyazhe (1370690143) 453037844       37 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/classic_control/mountain_car/envs/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     4679 2022-12-13 15:12:50.000000 DI-engine-0.4.7/dizoo/classic_control/mountain_car/envs/mtcar_env.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1400 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/classic_control/mountain_car/envs/test_mtcar_env.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:02.090246 DI-engine-0.4.7/dizoo/classic_control/pendulum/
--rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/classic_control/pendulum/__init__.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:02.102212 DI-engine-0.4.7/dizoo/classic_control/pendulum/config/
--rw-r--r--   0 niuyazhe (1370690143) 453037844      619 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/classic_control/pendulum/config/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1986 2023-01-04 09:44:45.000000 DI-engine-0.4.7/dizoo/classic_control/pendulum/config/pendulum_bdq_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1866 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/classic_control/pendulum/config/pendulum_cql_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1851 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/classic_control/pendulum/config/pendulum_d4pg_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1763 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/classic_control/pendulum/config/pendulum_ddpg_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1949 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/classic_control/pendulum/config/pendulum_dqn_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1068 2023-03-03 07:55:14.000000 DI-engine-0.4.7/dizoo/classic_control/pendulum/config/pendulum_dt_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1353 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/classic_control/pendulum/config/pendulum_ibc_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1376 2022-11-16 06:44:04.000000 DI-engine-0.4.7/dizoo/classic_control/pendulum/config/pendulum_pg_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1816 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/classic_control/pendulum/config/pendulum_ppo_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1766 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/classic_control/pendulum/config/pendulum_sac_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1347 2022-07-19 08:28:38.000000 DI-engine-0.4.7/dizoo/classic_control/pendulum/config/pendulum_sac_data_generation_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2664 2023-01-06 07:05:23.000000 DI-engine-0.4.7/dizoo/classic_control/pendulum/config/pendulum_sqil_sac_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2234 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/classic_control/pendulum/config/pendulum_td3_bc_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1832 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/classic_control/pendulum/config/pendulum_td3_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2203 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/classic_control/pendulum/config/pendulum_td3_data_generation_config.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:02.107722 DI-engine-0.4.7/dizoo/classic_control/pendulum/entry/
--rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/classic_control/pendulum/entry/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2177 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/classic_control/pendulum/entry/pendulum_cql_ddpg_main.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2266 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/classic_control/pendulum/entry/pendulum_cql_main.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     3083 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/classic_control/pendulum/entry/pendulum_d4pg_main.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     3576 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/classic_control/pendulum/entry/pendulum_ddpg_main.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2178 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/classic_control/pendulum/entry/pendulum_dqn_eval.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2178 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/classic_control/pendulum/entry/pendulum_ppo_main.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2325 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/classic_control/pendulum/entry/pendulum_td3_bc_main.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     3381 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/classic_control/pendulum/entry/pendulum_td3_main.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:02.109524 DI-engine-0.4.7/dizoo/classic_control/pendulum/envs/
--rw-r--r--   0 niuyazhe (1370690143) 453037844       38 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/classic_control/pendulum/envs/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     4943 2022-12-13 15:12:50.000000 DI-engine-0.4.7/dizoo/classic_control/pendulum/envs/pendulum_env.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2226 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/classic_control/pendulum/envs/test_pendulum_env.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:02.110134 DI-engine-0.4.7/dizoo/common/
--rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/common/__init__.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:02.113244 DI-engine-0.4.7/dizoo/common/policy/
--rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/common/policy/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     4317 2023-04-05 10:04:48.000000 DI-engine-0.4.7/dizoo/common/policy/md_dqn.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     8472 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/common/policy/md_ppo.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     4183 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/common/policy/md_rainbow_dqn.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:02.114003 DI-engine-0.4.7/dizoo/competitive_rl/
--rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/competitive_rl/__init__.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:02.116732 DI-engine-0.4.7/dizoo/competitive_rl/envs/
--rw-r--r--   0 niuyazhe (1370690143) 453037844       49 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/competitive_rl/envs/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     6561 2022-12-13 15:12:50.000000 DI-engine-0.4.7/dizoo/competitive_rl/envs/competitive_rl_env.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     8597 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/competitive_rl/envs/competitive_rl_env_wrapper.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2554 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/competitive_rl/envs/test_competitive_rl.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:02.117501 DI-engine-0.4.7/dizoo/d4rl/
--rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/d4rl/__init__.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:02.161731 DI-engine-0.4.7/dizoo/d4rl/config/
--rw-r--r--   0 niuyazhe (1370690143) 453037844      175 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/d4rl/config/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1485 2022-07-19 08:28:38.000000 DI-engine-0.4.7/dizoo/d4rl/config/halfcheetah_expert_cql_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2450 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/d4rl/config/halfcheetah_expert_dt_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1726 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/d4rl/config/halfcheetah_expert_td3bc_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1485 2022-07-19 08:28:38.000000 DI-engine-0.4.7/dizoo/d4rl/config/halfcheetah_medium_cql_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2450 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/d4rl/config/halfcheetah_medium_dt_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1499 2022-07-19 08:28:38.000000 DI-engine-0.4.7/dizoo/d4rl/config/halfcheetah_medium_expert_cql_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2471 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/d4rl/config/halfcheetah_medium_expert_dt_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1746 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/d4rl/config/halfcheetah_medium_expert_td3bc_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1499 2022-07-19 08:28:38.000000 DI-engine-0.4.7/dizoo/d4rl/config/halfcheetah_medium_replay_cql_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2471 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/d4rl/config/halfcheetah_medium_replay_dt_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1746 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/d4rl/config/halfcheetah_medium_replay_td3bc_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1732 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/d4rl/config/halfcheetah_medium_td3bc_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1485 2022-07-19 08:28:38.000000 DI-engine-0.4.7/dizoo/d4rl/config/halfcheetah_random_cql_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2449 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/d4rl/config/halfcheetah_random_dt_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1732 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/d4rl/config/halfcheetah_random_td3bc_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1475 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/d4rl/config/hopper_expert_cql_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2385 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/d4rl/config/hopper_expert_dt_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1722 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/d4rl/config/hopper_expert_td3bc_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1475 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/d4rl/config/hopper_medium_cql_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2385 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/d4rl/config/hopper_medium_dt_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1449 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/d4rl/config/hopper_medium_expert_bc_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1489 2022-07-19 08:28:38.000000 DI-engine-0.4.7/dizoo/d4rl/config/hopper_medium_expert_cql_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2406 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/d4rl/config/hopper_medium_expert_dt_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1458 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/d4rl/config/hopper_medium_expert_ibc_ar_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1342 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/d4rl/config/hopper_medium_expert_ibc_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1348 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/d4rl/config/hopper_medium_expert_ibc_mcmc_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1736 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/d4rl/config/hopper_medium_expert_td3bc_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1489 2022-07-19 08:28:38.000000 DI-engine-0.4.7/dizoo/d4rl/config/hopper_medium_replay_cql_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2406 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/d4rl/config/hopper_medium_replay_dt_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1736 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/d4rl/config/hopper_medium_replay_td3bc_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1722 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/d4rl/config/hopper_medium_td3bc_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1475 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/d4rl/config/hopper_random_cql_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2384 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/d4rl/config/hopper_random_dt_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1722 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/d4rl/config/hopper_random_td3bc_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1448 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/d4rl/config/kitchen_complete_bc_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1453 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/d4rl/config/kitchen_complete_ibc_ar_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1337 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/d4rl/config/kitchen_complete_ibc_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1343 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/d4rl/config/kitchen_complete_ibc_mcmc_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1431 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/d4rl/config/pen_human_bc_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1501 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/d4rl/config/pen_human_ibc_ar_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1324 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/d4rl/config/pen_human_ibc_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1330 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/d4rl/config/pen_human_ibc_mcmc_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1479 2022-07-19 08:28:38.000000 DI-engine-0.4.7/dizoo/d4rl/config/walker2d_expert_cql_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2411 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/d4rl/config/walker2d_expert_dt_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1732 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/d4rl/config/walker2d_expert_td3bc_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1479 2022-07-19 08:28:38.000000 DI-engine-0.4.7/dizoo/d4rl/config/walker2d_medium_cql_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2411 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/d4rl/config/walker2d_medium_dt_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1493 2022-07-19 08:28:38.000000 DI-engine-0.4.7/dizoo/d4rl/config/walker2d_medium_expert_cql_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2432 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/d4rl/config/walker2d_medium_expert_dt_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1740 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/d4rl/config/walker2d_medium_expert_td3bc_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1493 2022-07-19 08:28:38.000000 DI-engine-0.4.7/dizoo/d4rl/config/walker2d_medium_replay_cql_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2432 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/d4rl/config/walker2d_medium_replay_dt_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1740 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/d4rl/config/walker2d_medium_replay_td3bc_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1726 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/d4rl/config/walker2d_medium_td3bc_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1479 2022-07-19 08:28:38.000000 DI-engine-0.4.7/dizoo/d4rl/config/walker2d_random_cql_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2410 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/d4rl/config/walker2d_random_dt_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1726 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/d4rl/config/walker2d_random_td3bc_config.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:02.165231 DI-engine-0.4.7/dizoo/d4rl/entry/
--rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/d4rl/entry/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844      685 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/d4rl/entry/d4rl_cql_main.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1407 2022-07-19 08:28:38.000000 DI-engine-0.4.7/dizoo/d4rl/entry/d4rl_dt_main.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1171 2023-04-05 10:04:48.000000 DI-engine-0.4.7/dizoo/d4rl/entry/d4rl_ibc_main.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844      694 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/d4rl/entry/d4rl_td3_bc_main.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:02.167580 DI-engine-0.4.7/dizoo/d4rl/envs/
--rw-r--r--   0 niuyazhe (1370690143) 453037844       30 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/d4rl/envs/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     3986 2022-12-13 15:12:50.000000 DI-engine-0.4.7/dizoo/d4rl/envs/d4rl_env.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2286 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/d4rl/envs/d4rl_wrappers.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:02.168349 DI-engine-0.4.7/dizoo/dmc2gym/
--rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2022-07-19 08:28:38.000000 DI-engine-0.4.7/dizoo/dmc2gym/__init__.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:02.170371 DI-engine-0.4.7/dizoo/dmc2gym/envs/
--rw-r--r--   0 niuyazhe (1370690143) 453037844       36 2022-07-19 08:28:38.000000 DI-engine-0.4.7/dizoo/dmc2gym/envs/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     8742 2023-03-09 11:08:49.000000 DI-engine-0.4.7/dizoo/dmc2gym/envs/dmc2gym_env.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1645 2023-03-09 11:08:49.000000 DI-engine-0.4.7/dizoo/dmc2gym/envs/test_dmc2gym_env.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:02.171145 DI-engine-0.4.7/dizoo/evogym/
--rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/evogym/__init__.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:02.173220 DI-engine-0.4.7/dizoo/evogym/envs/
--rw-r--r--   0 niuyazhe (1370690143) 453037844       34 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/evogym/envs/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     6926 2022-12-13 15:12:50.000000 DI-engine-0.4.7/dizoo/evogym/envs/evogym_env.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:02.174966 DI-engine-0.4.7/dizoo/gfootball/
--rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/gfootball/__init__.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:02.181602 DI-engine-0.4.7/dizoo/gfootball/entry/
--rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/gfootball/entry/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2523 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/gfootball/entry/gfootball_bc_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2542 2022-10-31 06:23:24.000000 DI-engine-0.4.7/dizoo/gfootball/entry/gfootball_bc_kaggle5th_main.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     4374 2022-10-31 06:23:24.000000 DI-engine-0.4.7/dizoo/gfootball/entry/gfootball_bc_rule_lt0_main.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     4010 2022-10-31 06:23:24.000000 DI-engine-0.4.7/dizoo/gfootball/entry/gfootball_bc_rule_main.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1896 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/gfootball/entry/gfootball_dqn_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2197 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/gfootball/entry/show_dataset.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1884 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/gfootball/entry/test_accuracy.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:02.193227 DI-engine-0.4.7/dizoo/gfootball/envs/
--rw-r--r--   0 niuyazhe (1370690143) 453037844      174 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/gfootball/envs/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2648 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/gfootball/envs/fake_dataset.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    14135 2022-12-13 15:12:50.000000 DI-engine-0.4.7/dizoo/gfootball/envs/gfootball_academy_env.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     8689 2022-12-13 15:12:50.000000 DI-engine-0.4.7/dizoo/gfootball/envs/gfootball_env.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     7430 2022-12-13 15:12:50.000000 DI-engine-0.4.7/dizoo/gfootball/envs/gfootballsp_env.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:02.193903 DI-engine-0.4.7/dizoo/gfootball/model/
--rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/gfootball/model/__init__.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:02.197176 DI-engine-0.4.7/dizoo/gfootball/model/bots/
--rw-r--r--   0 niuyazhe (1370690143) 453037844      120 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/gfootball/model/bots/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1780 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/gfootball/model/bots/kaggle_5th_place_model.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    26957 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/gfootball/model/bots/rule_based_bot_model.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:02.198780 DI-engine-0.4.7/dizoo/gfootball/policy/
--rw-r--r--   0 niuyazhe (1370690143) 453037844       55 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/gfootball/policy/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    15162 2023-04-05 10:04:48.000000 DI-engine-0.4.7/dizoo/gfootball/policy/ppo_lstm.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1268 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/gfootball/replay.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:02.199826 DI-engine-0.4.7/dizoo/gym_anytrading/
--rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/gym_anytrading/__init__.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:02.201216 DI-engine-0.4.7/dizoo/gym_anytrading/config/
--rw-r--r--   0 niuyazhe (1370690143) 453037844       76 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/gym_anytrading/config/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2952 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/gym_anytrading/config/stocks_dqn_config.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:02.205626 DI-engine-0.4.7/dizoo/gym_anytrading/envs/
--rw-r--r--   0 niuyazhe (1370690143) 453037844       90 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/gym_anytrading/envs/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     6412 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/gym_anytrading/envs/stocks_env.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1506 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/gym_anytrading/envs/test_stocks_env.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    10840 2022-12-13 15:12:50.000000 DI-engine-0.4.7/dizoo/gym_anytrading/envs/trading_env.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:02.207267 DI-engine-0.4.7/dizoo/gym_anytrading/worker/
--rw-r--r--   0 niuyazhe (1370690143) 453037844       51 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/gym_anytrading/worker/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     9730 2022-12-13 15:12:50.000000 DI-engine-0.4.7/dizoo/gym_anytrading/worker/trading_serial_evaluator.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:02.208214 DI-engine-0.4.7/dizoo/gym_hybrid/
--rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/gym_hybrid/__init__.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:02.211084 DI-engine-0.4.7/dizoo/gym_hybrid/config/
--rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2022-12-22 08:45:23.000000 DI-engine-0.4.7/dizoo/gym_hybrid/config/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2196 2023-01-02 10:31:34.000000 DI-engine-0.4.7/dizoo/gym_hybrid/config/gym_hybrid_ddpg_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1985 2023-01-02 10:31:34.000000 DI-engine-0.4.7/dizoo/gym_hybrid/config/gym_hybrid_hppo_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2453 2023-04-05 10:04:48.000000 DI-engine-0.4.7/dizoo/gym_hybrid/config/gym_hybrid_mpdqn_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2381 2023-04-05 10:04:48.000000 DI-engine-0.4.7/dizoo/gym_hybrid/config/gym_hybrid_pdqn_config.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:02.214412 DI-engine-0.4.7/dizoo/gym_hybrid/entry/
--rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/gym_hybrid/entry/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2316 2022-12-26 09:01:35.000000 DI-engine-0.4.7/dizoo/gym_hybrid/entry/e.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2196 2023-01-02 10:31:34.000000 DI-engine-0.4.7/dizoo/gym_hybrid/entry/gym_hybrid_ddpg_eval.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     3996 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/gym_hybrid/entry/gym_hybrid_ddpg_main.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:02.218911 DI-engine-0.4.7/dizoo/gym_hybrid/envs/
--rw-r--r--   0 niuyazhe (1370690143) 453037844       41 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/gym_hybrid/envs/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     5940 2023-01-02 10:31:34.000000 DI-engine-0.4.7/dizoo/gym_hybrid/envs/gym_hybrid_env.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1149 2022-11-14 04:31:11.000000 DI-engine-0.4.7/dizoo/gym_hybrid/envs/test_gym_hybrid_env.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:02.220944 DI-engine-0.4.7/dizoo/gym_pybullet_drones/
--rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2022-11-14 04:31:11.000000 DI-engine-0.4.7/dizoo/gym_pybullet_drones/__init__.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:02.224183 DI-engine-0.4.7/dizoo/gym_pybullet_drones/envs/
--rw-r--r--   0 niuyazhe (1370690143) 453037844       58 2023-01-04 09:44:45.000000 DI-engine-0.4.7/dizoo/gym_pybullet_drones/envs/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     9559 2023-03-10 09:15:22.000000 DI-engine-0.4.7/dizoo/gym_pybullet_drones/envs/gym_pybullet_drones_env.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1034 2022-11-14 04:31:11.000000 DI-engine-0.4.7/dizoo/gym_pybullet_drones/envs/test_ding_env.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844      830 2022-11-14 04:31:11.000000 DI-engine-0.4.7/dizoo/gym_pybullet_drones/envs/test_ori_env.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:02.225089 DI-engine-0.4.7/dizoo/gym_soccer/
--rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/gym_soccer/__init__.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:02.226968 DI-engine-0.4.7/dizoo/gym_soccer/envs/
--rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/gym_soccer/envs/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     6247 2022-12-13 15:12:50.000000 DI-engine-0.4.7/dizoo/gym_soccer/envs/gym_soccer_env.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1248 2022-12-13 15:12:50.000000 DI-engine-0.4.7/dizoo/gym_soccer/envs/test_gym_soccer_env.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:02.228073 DI-engine-0.4.7/dizoo/image_classification/
--rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/image_classification/__init__.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:02.230975 DI-engine-0.4.7/dizoo/image_classification/data/
--rw-r--r--   0 niuyazhe (1370690143) 453037844       77 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/image_classification/data/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     4660 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/image_classification/data/dataset.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2207 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/image_classification/data/sampler.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:02.233079 DI-engine-0.4.7/dizoo/image_classification/policy/
--rw-r--r--   0 niuyazhe (1370690143) 453037844       46 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/image_classification/policy/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2955 2023-04-05 10:04:48.000000 DI-engine-0.4.7/dizoo/image_classification/policy/policy.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:02.240376 DI-engine-0.4.7/dizoo/league_demo/
--rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/league_demo/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1805 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/league_demo/demo_league.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     3024 2022-12-13 15:12:50.000000 DI-engine-0.4.7/dizoo/league_demo/game_env.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    16428 2022-12-13 15:12:50.000000 DI-engine-0.4.7/dizoo/league_demo/league_demo_collector.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2768 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/league_demo/league_demo_ppo_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    10209 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/league_demo/league_demo_ppo_main.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1199 2022-07-19 08:28:38.000000 DI-engine-0.4.7/dizoo/league_demo/selfplay_demo_ppo_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     4662 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/league_demo/selfplay_demo_ppo_main.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:02.242679 DI-engine-0.4.7/dizoo/mario/
--rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2023-01-17 12:08:18.000000 DI-engine-0.4.7/dizoo/mario/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1354 2023-01-17 12:08:18.000000 DI-engine-0.4.7/dizoo/mario/mario_dqn_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2787 2023-02-13 06:54:46.000000 DI-engine-0.4.7/dizoo/mario/mario_dqn_example.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     4454 2023-01-17 12:08:18.000000 DI-engine-0.4.7/dizoo/mario/mario_dqn_main.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:02.243384 DI-engine-0.4.7/dizoo/maze/
--rw-r--r--   0 niuyazhe (1370690143) 453037844      100 2023-03-09 11:08:49.000000 DI-engine-0.4.7/dizoo/maze/__init__.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:02.245379 DI-engine-0.4.7/dizoo/maze/envs/
--rw-r--r--   0 niuyazhe (1370690143) 453037844       27 2023-03-09 11:08:49.000000 DI-engine-0.4.7/dizoo/maze/envs/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    13099 2023-03-10 04:24:02.000000 DI-engine-0.4.7/dizoo/maze/envs/maze_env.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844      793 2023-03-09 11:08:49.000000 DI-engine-0.4.7/dizoo/maze/envs/test_maze_env.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:02.246119 DI-engine-0.4.7/dizoo/metadrive/
--rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2023-02-15 07:39:03.000000 DI-engine-0.4.7/dizoo/metadrive/__init__.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:02.248040 DI-engine-0.4.7/dizoo/metadrive/config/
--rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2023-02-15 07:39:03.000000 DI-engine-0.4.7/dizoo/metadrive/config/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     4258 2023-02-23 09:38:44.000000 DI-engine-0.4.7/dizoo/metadrive/config/metadrive_onppo_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     3693 2023-02-15 07:39:03.000000 DI-engine-0.4.7/dizoo/metadrive/config/metadrive_onppo_eval_config.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:02.250265 DI-engine-0.4.7/dizoo/metadrive/env/
--rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2023-02-15 07:39:03.000000 DI-engine-0.4.7/dizoo/metadrive/env/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    15662 2023-03-10 09:15:22.000000 DI-engine-0.4.7/dizoo/metadrive/env/drive_env.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     4010 2023-04-05 10:04:48.000000 DI-engine-0.4.7/dizoo/metadrive/env/drive_utils.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     5709 2023-04-05 10:04:48.000000 DI-engine-0.4.7/dizoo/metadrive/env/drive_wrapper.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:02.250958 DI-engine-0.4.7/dizoo/minigrid/
--rw-r--r--   0 niuyazhe (1370690143) 453037844      750 2023-03-09 11:08:49.000000 DI-engine-0.4.7/dizoo/minigrid/__init__.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:02.255341 DI-engine-0.4.7/dizoo/minigrid/envs/
--rw-r--r--   0 niuyazhe (1370690143) 453037844      323 2023-03-09 11:08:49.000000 DI-engine-0.4.7/dizoo/minigrid/envs/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     7470 2023-03-09 11:08:49.000000 DI-engine-0.4.7/dizoo/minigrid/envs/app_key_to_door_treasure.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     6933 2023-03-10 09:15:22.000000 DI-engine-0.4.7/dizoo/minigrid/envs/minigrid_env.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1163 2023-03-09 11:08:49.000000 DI-engine-0.4.7/dizoo/minigrid/envs/minigrid_wrapper.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     7249 2023-03-09 11:08:49.000000 DI-engine-0.4.7/dizoo/minigrid/envs/noisy_tv.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     3769 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/minigrid/envs/test_minigrid_env.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:02.256214 DI-engine-0.4.7/dizoo/mujoco/
--rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/mujoco/__init__.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:02.324766 DI-engine-0.4.7/dizoo/mujoco/config/
--rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/mujoco/config/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2105 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/mujoco/config/ant_ddpg_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     3352 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/mujoco/config/ant_gail_sac_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2154 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/mujoco/config/ant_onppo_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1705 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/mujoco/config/ant_ppo_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1976 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/mujoco/config/ant_sac_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2009 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/mujoco/config/ant_td3_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2544 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/mujoco/config/ant_trex_onppo_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2829 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/mujoco/config/ant_trex_sac_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2954 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/mujoco/config/halfcheetah_bco_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2057 2023-01-04 09:44:45.000000 DI-engine-0.4.7/dizoo/mujoco/config/halfcheetah_bdq_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2074 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/mujoco/config/halfcheetah_d4pg_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1915 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/mujoco/config/halfcheetah_ddpg_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     3430 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/mujoco/config/halfcheetah_gail_sac_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2814 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/mujoco/config/halfcheetah_gcl_sac_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2335 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/mujoco/config/halfcheetah_onppo_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1991 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/mujoco/config/halfcheetah_sac_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2750 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/mujoco/config/halfcheetah_sqil_sac_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2039 2022-11-14 04:31:11.000000 DI-engine-0.4.7/dizoo/mujoco/config/halfcheetah_td3_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     4130 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/mujoco/config/halfcheetah_trex_onppo_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     3966 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/mujoco/config/halfcheetah_trex_sac_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2847 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/mujoco/config/hopper_bco_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2246 2023-01-04 09:44:45.000000 DI-engine-0.4.7/dizoo/mujoco/config/hopper_bdq_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2093 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/mujoco/config/hopper_cql_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1966 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/mujoco/config/hopper_d4pg_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1857 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/mujoco/config/hopper_ddpg_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     3397 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/mujoco/config/hopper_gail_sac_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2372 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/mujoco/config/hopper_gcl_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2131 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/mujoco/config/hopper_onppo_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1936 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/mujoco/config/hopper_sac_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2610 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/mujoco/config/hopper_sac_data_generation_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2601 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/mujoco/config/hopper_sqil_sac_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2455 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/mujoco/config/hopper_td3_bc_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1969 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/mujoco/config/hopper_td3_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2668 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/mujoco/config/hopper_td3_data_generation_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     3635 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/mujoco/config/hopper_trex_onppo_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     3870 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/mujoco/config/hopper_trex_sac_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2000 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/mujoco/config/walker2d_d4pg_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1879 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/mujoco/config/walker2d_ddpg_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     3579 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/mujoco/config/walker2d_gail_ddpg_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     3425 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/mujoco/config/walker2d_gail_sac_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2432 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/mujoco/config/walker2d_gcl_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2346 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/mujoco/config/walker2d_onppo_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1958 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/mujoco/config/walker2d_sac_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2567 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/mujoco/config/walker2d_sqil_sac_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1991 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/mujoco/config/walker2d_td3_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     3659 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/mujoco/config/walker2d_trex_onppo_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     3894 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/mujoco/config/walker2d_trex_sac_config.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:02.333522 DI-engine-0.4.7/dizoo/mujoco/entry/
--rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/mujoco/entry/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844      983 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/mujoco/entry/mujoco_cql_generation_main.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844      436 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/mujoco/entry/mujoco_cql_main.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2861 2022-11-14 04:31:11.000000 DI-engine-0.4.7/dizoo/mujoco/entry/mujoco_d4pg_main.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1937 2022-11-14 04:31:11.000000 DI-engine-0.4.7/dizoo/mujoco/entry/mujoco_ddpg_eval.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2697 2022-11-14 04:31:11.000000 DI-engine-0.4.7/dizoo/mujoco/entry/mujoco_ddpg_main.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2338 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/mujoco/entry/mujoco_ppo_main.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2290 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/mujoco/entry/mujoco_td3_bc_main.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:02.342247 DI-engine-0.4.7/dizoo/mujoco/envs/
--rw-r--r--   0 niuyazhe (1370690143) 453037844       77 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/mujoco/envs/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     6144 2022-12-13 15:12:50.000000 DI-engine-0.4.7/dizoo/mujoco/envs/mujoco_disc_env.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     8606 2023-01-04 09:44:45.000000 DI-engine-0.4.7/dizoo/mujoco/envs/mujoco_env.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1992 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/mujoco/envs/mujoco_gym_env.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1415 2022-12-13 15:12:50.000000 DI-engine-0.4.7/dizoo/mujoco/envs/mujoco_wrappers.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:02.342914 DI-engine-0.4.7/dizoo/multiagent_mujoco/
--rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/multiagent_mujoco/__init__.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:02.348802 DI-engine-0.4.7/dizoo/multiagent_mujoco/envs/
--rw-r--r--   0 niuyazhe (1370690143) 453037844      185 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/multiagent_mujoco/envs/__init__.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:02.366099 DI-engine-0.4.7/dizoo/multiagent_mujoco/envs/assets/
--rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/multiagent_mujoco/envs/assets/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     8773 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/multiagent_mujoco/envs/assets/coupled_half_cheetah.xml
--rw-r--r--   0 niuyazhe (1370690143) 453037844     8333 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/multiagent_mujoco/envs/assets/manyagent_ant.xml
--rw-r--r--   0 niuyazhe (1370690143) 453037844     5215 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/multiagent_mujoco/envs/assets/manyagent_ant__stage1.xml
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2900 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/multiagent_mujoco/envs/assets/manyagent_swimmer__bckp2.xml
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2570 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/multiagent_mujoco/envs/assets/manyagent_swimmer_bckp.xml
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1852 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/multiagent_mujoco/envs/coupled_half_cheetah.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     5661 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/multiagent_mujoco/envs/manyagent_ant.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     3593 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/multiagent_mujoco/envs/manyagent_swimmer.py
--rwxr-xr-x   0 niuyazhe (1370690143) 453037844     9649 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/multiagent_mujoco/envs/mujoco_multi.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     4066 2022-12-13 15:12:50.000000 DI-engine-0.4.7/dizoo/multiagent_mujoco/envs/multi_mujoco_env.py
--rwxr-xr-x   0 niuyazhe (1370690143) 453037844     2404 2022-03-14 08:09:40.000000 DI-engine-0.4.7/dizoo/multiagent_mujoco/envs/multiagentenv.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    23700 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/multiagent_mujoco/envs/obsk.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:02.367071 DI-engine-0.4.7/dizoo/overcooked/
--rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/overcooked/__init__.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:02.368469 DI-engine-0.4.7/dizoo/overcooked/config/
--rw-r--r--   0 niuyazhe (1370690143) 453037844       68 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/overcooked/config/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2357 2022-07-19 08:28:38.000000 DI-engine-0.4.7/dizoo/overcooked/config/overcooked_ppo_config.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:02.371417 DI-engine-0.4.7/dizoo/overcooked/envs/
--rw-r--r--   0 niuyazhe (1370690143) 453037844       58 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/overcooked/envs/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    12316 2022-12-13 15:12:50.000000 DI-engine-0.4.7/dizoo/overcooked/envs/overcooked_env.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1726 2022-12-13 15:12:50.000000 DI-engine-0.4.7/dizoo/overcooked/envs/test_overcooked_env.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:02.372297 DI-engine-0.4.7/dizoo/petting_zoo/
--rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2022-07-19 08:28:38.000000 DI-engine-0.4.7/dizoo/petting_zoo/__init__.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:02.388217 DI-engine-0.4.7/dizoo/petting_zoo/config/
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1022 2022-12-11 15:35:39.000000 DI-engine-0.4.7/dizoo/petting_zoo/config/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2391 2023-03-01 15:44:29.000000 DI-engine-0.4.7/dizoo/petting_zoo/config/ptz_simple_spread_atoc_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2456 2023-03-01 15:44:29.000000 DI-engine-0.4.7/dizoo/petting_zoo/config/ptz_simple_spread_collaq_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2512 2023-03-01 15:44:29.000000 DI-engine-0.4.7/dizoo/petting_zoo/config/ptz_simple_spread_coma_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2581 2023-03-01 15:44:29.000000 DI-engine-0.4.7/dizoo/petting_zoo/config/ptz_simple_spread_madqn_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2960 2023-03-01 15:44:29.000000 DI-engine-0.4.7/dizoo/petting_zoo/config/ptz_simple_spread_mappo_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     3032 2023-03-01 15:44:29.000000 DI-engine-0.4.7/dizoo/petting_zoo/config/ptz_simple_spread_masac_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2082 2023-03-01 15:44:29.000000 DI-engine-0.4.7/dizoo/petting_zoo/config/ptz_simple_spread_qmix_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2490 2023-03-01 15:44:29.000000 DI-engine-0.4.7/dizoo/petting_zoo/config/ptz_simple_spread_qtran_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2196 2023-03-01 15:44:29.000000 DI-engine-0.4.7/dizoo/petting_zoo/config/ptz_simple_spread_vdn_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     2394 2023-03-01 15:44:29.000000 DI-engine-0.4.7/dizoo/petting_zoo/config/ptz_simple_spread_wqmix_config.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:02.391618 DI-engine-0.4.7/dizoo/petting_zoo/envs/
--rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2022-07-19 08:28:38.000000 DI-engine-0.4.7/dizoo/petting_zoo/envs/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    16736 2023-03-09 11:08:49.000000 DI-engine-0.4.7/dizoo/petting_zoo/envs/petting_zoo_simple_spread_env.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     5416 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/petting_zoo/envs/test_petting_zoo_simple_spread_env.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:02.392653 DI-engine-0.4.7/dizoo/pomdp/
--rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/pomdp/__init__.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:02.395720 DI-engine-0.4.7/dizoo/pomdp/envs/
--rw-r--r--   0 niuyazhe (1370690143) 453037844       37 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/pomdp/envs/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     4022 2022-12-13 15:12:50.000000 DI-engine-0.4.7/dizoo/pomdp/envs/atari_env.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     6746 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/pomdp/envs/atari_wrappers.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1031 2022-12-13 15:12:50.000000 DI-engine-0.4.7/dizoo/pomdp/envs/test_atari_env.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:02.396487 DI-engine-0.4.7/dizoo/procgen/
--rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2023-01-17 12:06:29.000000 DI-engine-0.4.7/dizoo/procgen/__init__.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:02.402975 DI-engine-0.4.7/dizoo/procgen/config/
--rw-r--r--   0 niuyazhe (1370690143) 453037844      118 2022-12-11 15:35:39.000000 DI-engine-0.4.7/dizoo/procgen/config/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1719 2022-12-11 15:35:39.000000 DI-engine-0.4.7/dizoo/procgen/config/bigfish_plr_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1617 2022-12-11 15:35:39.000000 DI-engine-0.4.7/dizoo/procgen/config/bigfish_ppg_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1362 2022-12-11 15:35:39.000000 DI-engine-0.4.7/dizoo/procgen/config/coinrun_dqn_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1616 2022-12-11 15:35:39.000000 DI-engine-0.4.7/dizoo/procgen/config/coinrun_ppg_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1449 2022-12-11 15:35:39.000000 DI-engine-0.4.7/dizoo/procgen/config/coinrun_ppo_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1369 2022-12-11 15:35:39.000000 DI-engine-0.4.7/dizoo/procgen/config/maze_dqn_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1641 2022-12-11 15:35:39.000000 DI-engine-0.4.7/dizoo/procgen/config/maze_ppg_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1447 2022-12-11 15:35:39.000000 DI-engine-0.4.7/dizoo/procgen/config/maze_ppo_config.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:02.405351 DI-engine-0.4.7/dizoo/procgen/envs/
--rw-r--r--   0 niuyazhe (1370690143) 453037844       36 2022-07-19 08:28:38.000000 DI-engine-0.4.7/dizoo/procgen/envs/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     4485 2022-12-13 15:12:50.000000 DI-engine-0.4.7/dizoo/procgen/envs/procgen_env.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844      810 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/procgen/envs/test_coinrun_env.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:02.406083 DI-engine-0.4.7/dizoo/pybullet/
--rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/pybullet/__init__.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:02.408387 DI-engine-0.4.7/dizoo/pybullet/envs/
--rw-r--r--   0 niuyazhe (1370690143) 453037844       38 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/pybullet/envs/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    11254 2022-12-13 15:12:50.000000 DI-engine-0.4.7/dizoo/pybullet/envs/pybullet_env.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1663 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/pybullet/envs/pybullet_wrappers.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:02.409133 DI-engine-0.4.7/dizoo/rocket/
--rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2023-01-17 12:05:32.000000 DI-engine-0.4.7/dizoo/rocket/__init__.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:02.410481 DI-engine-0.4.7/dizoo/rocket/config/
--rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2023-01-17 12:05:45.000000 DI-engine-0.4.7/dizoo/rocket/config/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1818 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/rocket/config/rocket_hover_ppo_config.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1828 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/rocket/config/rocket_landing_ppo_config.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:02.414361 DI-engine-0.4.7/dizoo/rocket/entry/
--rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2023-01-17 12:05:50.000000 DI-engine-0.4.7/dizoo/rocket/entry/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     4039 2023-02-13 06:56:29.000000 DI-engine-0.4.7/dizoo/rocket/entry/rocket_hover_onppo_main_v2.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     3261 2023-02-13 06:57:07.000000 DI-engine-0.4.7/dizoo/rocket/entry/rocket_hover_ppo_main.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     4022 2023-02-13 06:57:32.000000 DI-engine-0.4.7/dizoo/rocket/entry/rocket_landing_onppo_main_v2.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     3236 2023-02-13 06:56:46.000000 DI-engine-0.4.7/dizoo/rocket/entry/rocket_landing_ppo_main.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:02.416877 DI-engine-0.4.7/dizoo/rocket/envs/
--rw-r--r--   0 niuyazhe (1370690143) 453037844       34 2023-01-04 09:44:45.000000 DI-engine-0.4.7/dizoo/rocket/envs/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     4024 2023-03-10 09:15:22.000000 DI-engine-0.4.7/dizoo/rocket/envs/rocket_env.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1391 2023-01-04 09:44:45.000000 DI-engine-0.4.7/dizoo/rocket/envs/test_rocket_env.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:02.417796 DI-engine-0.4.7/dizoo/slime_volley/
--rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/slime_volley/__init__.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:02.418265 DI-engine-0.4.7/dizoo/slime_volley/config/
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1685 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/slime_volley/config/slime_volley_ppo_config.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:02.421559 DI-engine-0.4.7/dizoo/slime_volley/envs/
--rw-r--r--   0 niuyazhe (1370690143) 453037844       46 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/slime_volley/envs/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     7877 2022-12-13 15:12:50.000000 DI-engine-0.4.7/dizoo/slime_volley/envs/slime_volley_env.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1274 2022-12-13 15:12:50.000000 DI-engine-0.4.7/dizoo/slime_volley/envs/test_slime_volley_env.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:02.422809 DI-engine-0.4.7/dizoo/smac/
--rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/smac/__init__.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:02.430979 DI-engine-0.4.7/dizoo/smac/envs/
--rw-r--r--   0 niuyazhe (1370690143) 453037844      194 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/smac/envs/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1666 2022-12-13 15:12:50.000000 DI-engine-0.4.7/dizoo/smac/envs/fake_smac_env.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:02.431894 DI-engine-0.4.7/dizoo/smac/envs/maps/
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:02.455798 DI-engine-0.4.7/dizoo/smac/envs/maps/SMAC_Maps/
--rwxr-xr-x   0 niuyazhe (1370690143) 453037844    14925 2021-08-01 05:19:48.000000 DI-engine-0.4.7/dizoo/smac/envs/maps/SMAC_Maps/10m_vs_11m.SC2Map
--rwxr-xr-x   0 niuyazhe (1370690143) 453037844    16965 2021-08-01 05:19:48.000000 DI-engine-0.4.7/dizoo/smac/envs/maps/SMAC_Maps/1c3s5z.SC2Map
--rwxr-xr-x   0 niuyazhe (1370690143) 453037844    14923 2021-08-01 05:19:48.000000 DI-engine-0.4.7/dizoo/smac/envs/maps/SMAC_Maps/25m.SC2Map
--rwxr-xr-x   0 niuyazhe (1370690143) 453037844    14929 2021-08-01 05:19:48.000000 DI-engine-0.4.7/dizoo/smac/envs/maps/SMAC_Maps/27m_vs_30m.SC2Map
--rwxr-xr-x   0 niuyazhe (1370690143) 453037844    16477 2021-08-01 05:19:48.000000 DI-engine-0.4.7/dizoo/smac/envs/maps/SMAC_Maps/2c_vs_64zg.SC2Map
--rwxr-xr-x   0 niuyazhe (1370690143) 453037844    15539 2021-08-01 05:19:48.000000 DI-engine-0.4.7/dizoo/smac/envs/maps/SMAC_Maps/2m_vs_1z.SC2Map
--rwxr-xr-x   0 niuyazhe (1370690143) 453037844    15692 2021-08-01 05:19:48.000000 DI-engine-0.4.7/dizoo/smac/envs/maps/SMAC_Maps/2s3z.SC2Map
--rwxr-xr-x   0 niuyazhe (1370690143) 453037844    14202 2021-08-01 05:19:48.000000 DI-engine-0.4.7/dizoo/smac/envs/maps/SMAC_Maps/2s_vs_1sc.SC2Map
--rwxr-xr-x   0 niuyazhe (1370690143) 453037844    14920 2021-08-01 05:19:48.000000 DI-engine-0.4.7/dizoo/smac/envs/maps/SMAC_Maps/3m.SC2Map
--rwxr-xr-x   0 niuyazhe (1370690143) 453037844    15697 2021-08-01 05:19:48.000000 DI-engine-0.4.7/dizoo/smac/envs/maps/SMAC_Maps/3s5z.SC2Map
--rwxr-xr-x   0 niuyazhe (1370690143) 453037844    15704 2021-08-01 05:19:48.000000 DI-engine-0.4.7/dizoo/smac/envs/maps/SMAC_Maps/3s5z_vs_3s6z.SC2Map
--rwxr-xr-x   0 niuyazhe (1370690143) 453037844    13995 2021-08-01 05:19:48.000000 DI-engine-0.4.7/dizoo/smac/envs/maps/SMAC_Maps/3s_vs_3z.SC2Map
--rwxr-xr-x   0 niuyazhe (1370690143) 453037844    14000 2021-08-01 05:19:48.000000 DI-engine-0.4.7/dizoo/smac/envs/maps/SMAC_Maps/3s_vs_4z.SC2Map
--rwxr-xr-x   0 niuyazhe (1370690143) 453037844    13998 2021-08-01 05:19:48.000000 DI-engine-0.4.7/dizoo/smac/envs/maps/SMAC_Maps/3s_vs_5z.SC2Map
--rwxr-xr-x   0 niuyazhe (1370690143) 453037844    14930 2021-08-01 05:19:48.000000 DI-engine-0.4.7/dizoo/smac/envs/maps/SMAC_Maps/5m_vs_6m.SC2Map
--rwxr-xr-x   0 niuyazhe (1370690143) 453037844    14342 2021-08-01 05:19:48.000000 DI-engine-0.4.7/dizoo/smac/envs/maps/SMAC_Maps/6h_vs_8z.SC2Map
--rwxr-xr-x   0 niuyazhe (1370690143) 453037844    14922 2021-08-01 05:19:48.000000 DI-engine-0.4.7/dizoo/smac/envs/maps/SMAC_Maps/8m.SC2Map
--rwxr-xr-x   0 niuyazhe (1370690143) 453037844    14927 2021-08-01 05:19:48.000000 DI-engine-0.4.7/dizoo/smac/envs/maps/SMAC_Maps/8m_vs_9m.SC2Map
--rwxr-xr-x   0 niuyazhe (1370690143) 453037844    17411 2021-08-01 05:19:48.000000 DI-engine-0.4.7/dizoo/smac/envs/maps/SMAC_Maps/MMM.SC2Map
--rwxr-xr-x   0 niuyazhe (1370690143) 453037844    17419 2021-08-01 05:19:48.000000 DI-engine-0.4.7/dizoo/smac/envs/maps/SMAC_Maps/MMM2.SC2Map
--rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/smac/envs/maps/SMAC_Maps/__init__.py
--rwxr-xr-x   0 niuyazhe (1370690143) 453037844    16782 2021-08-01 05:19:48.000000 DI-engine-0.4.7/dizoo/smac/envs/maps/SMAC_Maps/bane_vs_bane.SC2Map
--rwxr-xr-x   0 niuyazhe (1370690143) 453037844    18055 2021-08-01 05:19:48.000000 DI-engine-0.4.7/dizoo/smac/envs/maps/SMAC_Maps/corridor.SC2Map
--rw-r--r--   0 niuyazhe (1370690143) 453037844    17080 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/smac/envs/maps/SMAC_Maps/infestor_viper.SC2Map
--rwxr-xr-x   0 niuyazhe (1370690143) 453037844    18133 2021-08-01 05:19:48.000000 DI-engine-0.4.7/dizoo/smac/envs/maps/SMAC_Maps/so_many_baneling.SC2Map
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:02.458210 DI-engine-0.4.7/dizoo/smac/envs/maps/SMAC_Maps_two_player/
--rwxr-xr-x   0 niuyazhe (1370690143) 453037844    14835 2021-08-01 05:19:48.000000 DI-engine-0.4.7/dizoo/smac/envs/maps/SMAC_Maps_two_player/3m.SC2Map
--rwxr-xr-x   0 niuyazhe (1370690143) 453037844    15596 2021-08-01 05:19:48.000000 DI-engine-0.4.7/dizoo/smac/envs/maps/SMAC_Maps_two_player/3s5z.SC2Map
--rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/smac/envs/maps/SMAC_Maps_two_player/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/smac/envs/maps/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    16272 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/smac/envs/smac_action.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844    70855 2022-12-13 15:12:50.000000 DI-engine-0.4.7/dizoo/smac/envs/smac_env.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     5383 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/smac/envs/smac_map.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     9098 2022-09-30 04:52:25.000000 DI-engine-0.4.7/dizoo/smac/envs/smac_reward.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     6050 2022-12-13 15:12:50.000000 DI-engine-0.4.7/dizoo/smac/envs/test_smac_env.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:02.458476 DI-engine-0.4.7/dizoo/sokoban/
--rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2023-01-17 12:06:19.000000 DI-engine-0.4.7/dizoo/sokoban/__init__.py
-drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-04-12 15:08:02.460779 DI-engine-0.4.7/dizoo/sokoban/envs/
--rw-r--r--   0 niuyazhe (1370690143) 453037844       36 2022-10-19 09:16:29.000000 DI-engine-0.4.7/dizoo/sokoban/envs/__init__.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     4021 2022-12-13 15:12:50.000000 DI-engine-0.4.7/dizoo/sokoban/envs/sokoban_env.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844     1658 2022-08-02 16:56:36.000000 DI-engine-0.4.7/dizoo/sokoban/envs/sokoban_wrappers.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844      779 2022-08-02 16:56:36.000000 DI-engine-0.4.7/dizoo/sokoban/envs/test_sokoban_env.py
--rw-r--r--   0 niuyazhe (1370690143) 453037844       38 2023-04-12 15:08:02.461912 DI-engine-0.4.7/setup.cfg
--rw-r--r--   0 niuyazhe (1370690143) 453037844     6130 2023-03-10 09:15:22.000000 DI-engine-0.4.7/setup.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:58.122656 DI-engine-0.4.8/
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.349135 DI-engine-0.4.8/DI_engine.egg-info/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    57242 2023-05-25 06:04:57.000000 DI-engine-0.4.8/DI_engine.egg-info/PKG-INFO
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    49689 2023-05-25 06:04:57.000000 DI-engine-0.4.8/DI_engine.egg-info/SOURCES.txt
+-rw-r--r--   0 niuyazhe (1370690143) 453037844        1 2023-05-25 06:04:57.000000 DI-engine-0.4.8/DI_engine.egg-info/dependency_links.txt
+-rw-r--r--   0 niuyazhe (1370690143) 453037844       86 2023-05-25 06:04:57.000000 DI-engine-0.4.8/DI_engine.egg-info/entry_points.txt
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1135 2023-05-25 06:04:57.000000 DI-engine-0.4.8/DI_engine.egg-info/requires.txt
+-rw-r--r--   0 niuyazhe (1370690143) 453037844       11 2023-05-25 06:04:57.000000 DI-engine-0.4.8/DI_engine.egg-info/top_level.txt
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    11342 2021-07-08 05:53:26.000000 DI-engine-0.4.8/LICENSE
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    57242 2023-05-25 06:04:58.122342 DI-engine-0.4.8/PKG-INFO
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    55976 2023-05-25 03:46:38.000000 DI-engine-0.4.8/README.md
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.349854 DI-engine-0.4.8/ding/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844      380 2023-05-25 03:46:09.000000 DI-engine-0.4.8/ding/__init__.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.357396 DI-engine-0.4.8/ding/bonus/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844       58 2023-04-05 10:04:48.000000 DI-engine-0.4.8/ding/bonus/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    10868 2023-04-05 10:04:48.000000 DI-engine-0.4.8/ding/bonus/config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844      901 2023-01-06 07:07:56.000000 DI-engine-0.4.8/ding/bonus/demo.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     9777 2023-04-11 05:01:52.000000 DI-engine-0.4.8/ding/bonus/model.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     9299 2023-05-12 10:29:30.000000 DI-engine-0.4.8/ding/bonus/ppof.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     9060 2023-04-05 10:04:48.000000 DI-engine-0.4.8/ding/bonus/td3.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844      211 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/compatibility.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.360407 DI-engine-0.4.8/ding/config/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844      227 2023-01-04 09:44:45.000000 DI-engine-0.4.8/ding/config/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    24245 2023-05-12 10:29:30.000000 DI-engine-0.4.8/ding/config/config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    28073 2023-04-05 10:04:48.000000 DI-engine-0.4.8/ding/config/utils.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.364056 DI-engine-0.4.8/ding/data/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844      352 2022-12-13 15:12:49.000000 DI-engine-0.4.8/ding/data/__init__.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.367582 DI-engine-0.4.8/ding/data/buffer/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844      150 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/data/buffer/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     7617 2022-12-11 15:35:39.000000 DI-engine-0.4.8/ding/data/buffer/buffer.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    14785 2022-12-11 15:35:39.000000 DI-engine-0.4.8/ding/data/buffer/deque_buffer.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     4701 2023-02-20 14:45:59.000000 DI-engine-0.4.8/ding/data/buffer/deque_buffer_wrapper.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.374646 DI-engine-0.4.8/ding/data/buffer/middleware/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844      291 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/data/buffer/middleware/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1064 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/data/buffer/middleware/clone_object.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1648 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/data/buffer/middleware/group_sample.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1496 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/data/buffer/middleware/padding.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     6962 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/data/buffer/middleware/priority.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844      979 2022-08-02 16:56:36.000000 DI-engine-0.4.8/ding/data/buffer/middleware/sample_range_view.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1830 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/data/buffer/middleware/staleness_check.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1887 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/data/buffer/middleware/use_time_check.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.375844 DI-engine-0.4.8/ding/data/level_replay/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2022-10-19 09:16:29.000000 DI-engine-0.4.8/ding/data/level_replay/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    13812 2023-01-02 10:31:34.000000 DI-engine-0.4.8/ding/data/level_replay/level_sampler.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     5501 2022-12-13 15:12:49.000000 DI-engine-0.4.8/ding/data/model_loader.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     5008 2023-03-09 12:42:49.000000 DI-engine-0.4.8/ding/data/shm_buffer.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.378376 DI-engine-0.4.8/ding/data/storage/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844       77 2022-12-13 15:12:49.000000 DI-engine-0.4.8/ding/data/storage/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844      605 2022-12-13 15:12:49.000000 DI-engine-0.4.8/ding/data/storage/file.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844      326 2022-12-13 15:12:49.000000 DI-engine-0.4.8/ding/data/storage/storage.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    11978 2022-12-13 15:12:49.000000 DI-engine-0.4.8/ding/data/storage_loader.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.402376 DI-engine-0.4.8/ding/entry/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1732 2023-03-09 11:08:49.000000 DI-engine-0.4.8/ding/entry/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    11820 2022-12-13 15:12:49.000000 DI-engine-0.4.8/ding/entry/application_entry.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     9797 2022-10-19 09:16:29.000000 DI-engine-0.4.8/ding/entry/application_entry_drex_collect_data.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     6652 2022-10-19 09:16:29.000000 DI-engine-0.4.8/ding/entry/application_entry_trex_collect_data.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    13003 2022-10-19 09:16:29.000000 DI-engine-0.4.8/ding/entry/cli.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     5475 2022-12-13 15:12:49.000000 DI-engine-0.4.8/ding/entry/cli_ditask.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.404727 DI-engine-0.4.8/ding/entry/cli_parsers/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844      136 2022-07-19 08:28:37.000000 DI-engine-0.4.8/ding/entry/cli_parsers/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     5855 2022-12-13 15:12:49.000000 DI-engine-0.4.8/ding/entry/cli_parsers/k8s_parser.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     5656 2022-12-13 15:12:49.000000 DI-engine-0.4.8/ding/entry/cli_parsers/slurm_parser.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    11742 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/entry/dist_entry.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     5631 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/entry/parallel_entry.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1156 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/entry/predefined_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     6335 2023-03-09 11:08:49.000000 DI-engine-0.4.8/ding/entry/serial_entry.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     4005 2022-10-31 06:23:24.000000 DI-engine-0.4.8/ding/entry/serial_entry_bc.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     8933 2023-05-12 11:44:20.000000 DI-engine-0.4.8/ding/entry/serial_entry_bco.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     3405 2022-10-19 09:16:29.000000 DI-engine-0.4.8/ding/entry/serial_entry_decision_transformer.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    12388 2022-10-19 09:16:29.000000 DI-engine-0.4.8/ding/entry/serial_entry_dqfd.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     8037 2022-12-13 15:12:49.000000 DI-engine-0.4.8/ding/entry/serial_entry_gail.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     8452 2022-10-19 09:16:29.000000 DI-engine-0.4.8/ding/entry/serial_entry_guided_cost.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    10336 2022-10-19 09:16:29.000000 DI-engine-0.4.8/ding/entry/serial_entry_mbrl.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     7979 2022-10-19 09:16:29.000000 DI-engine-0.4.8/ding/entry/serial_entry_ngu.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     4645 2022-10-19 09:16:29.000000 DI-engine-0.4.8/ding/entry/serial_entry_offline.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     4963 2022-12-13 15:12:49.000000 DI-engine-0.4.8/ding/entry/serial_entry_onpolicy.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     4460 2022-10-19 09:16:29.000000 DI-engine-0.4.8/ding/entry/serial_entry_onpolicy_ppg.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     4444 2023-03-09 11:08:49.000000 DI-engine-0.4.8/ding/entry/serial_entry_pc.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     5614 2022-10-19 09:16:29.000000 DI-engine-0.4.8/ding/entry/serial_entry_plr.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     6520 2023-01-06 07:05:23.000000 DI-engine-0.4.8/ding/entry/serial_entry_preference_based_irl.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     4811 2023-01-06 07:05:23.000000 DI-engine-0.4.8/ding/entry/serial_entry_preference_based_irl_onpolicy.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    12314 2022-10-19 09:16:29.000000 DI-engine-0.4.8/ding/entry/serial_entry_r2d3.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     6809 2023-03-09 11:08:49.000000 DI-engine-0.4.8/ding/entry/serial_entry_reward_model_offpolicy.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     6557 2023-03-09 11:08:49.000000 DI-engine-0.4.8/ding/entry/serial_entry_reward_model_onpolicy.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     8837 2022-10-19 09:16:29.000000 DI-engine-0.4.8/ding/entry/serial_entry_sqil.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    10374 2022-10-19 09:16:29.000000 DI-engine-0.4.8/ding/entry/serial_entry_td3_vae.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2466 2023-05-16 06:06:19.000000 DI-engine-0.4.8/ding/entry/utils.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.405472 DI-engine-0.4.8/ding/envs/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844       74 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/envs/__init__.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.408250 DI-engine-0.4.8/ding/envs/common/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844      354 2022-10-19 09:16:29.000000 DI-engine-0.4.8/ding/envs/common/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    10829 2022-10-19 09:16:29.000000 DI-engine-0.4.8/ding/envs/common/common_function.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1625 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/envs/common/env_element.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844      986 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/envs/common/env_element_runner.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.412668 DI-engine-0.4.8/ding/envs/env/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844      386 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/envs/env/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     6902 2023-01-02 16:43:42.000000 DI-engine-0.4.8/ding/envs/env/base_env.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1751 2023-03-09 11:08:49.000000 DI-engine-0.4.8/ding/envs/env/default_wrapper.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     9454 2023-04-05 10:04:48.000000 DI-engine-0.4.8/ding/envs/env/ding_env_wrapper.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     7078 2022-12-13 15:12:49.000000 DI-engine-0.4.8/ding/envs/env/env_implementation_check.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.415456 DI-engine-0.4.8/ding/envs/env/tests/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844       30 2022-07-19 08:28:37.000000 DI-engine-0.4.8/ding/envs/env/tests/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2216 2022-12-13 15:12:49.000000 DI-engine-0.4.8/ding/envs/env/tests/demo_env.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     7618 2022-12-13 15:12:49.000000 DI-engine-0.4.8/ding/envs/env/tests/test_ding_env_wrapper.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1974 2022-07-19 08:28:37.000000 DI-engine-0.4.8/ding/envs/env/tests/test_env_implementation_check.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.419795 DI-engine-0.4.8/ding/envs/env_manager/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844      394 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/envs/env_manager/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    21523 2023-04-05 10:04:48.000000 DI-engine-0.4.8/ding/envs/env_manager/base_env_manager.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    24099 2022-12-13 15:12:49.000000 DI-engine-0.4.8/ding/envs/env_manager/env_supervisor.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     4222 2022-12-13 15:12:49.000000 DI-engine-0.4.8/ding/envs/env_manager/envpool_env_manager.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     5793 2022-12-13 15:12:49.000000 DI-engine-0.4.8/ding/envs/env_manager/gym_vector_env_manager.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    36999 2023-03-09 11:08:49.000000 DI-engine-0.4.8/ding/envs/env_manager/subprocess_env_manager.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.426887 DI-engine-0.4.8/ding/envs/env_manager/tests/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/envs/env_manager/tests/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     8258 2023-01-02 10:31:34.000000 DI-engine-0.4.8/ding/envs/env_manager/tests/conftest.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     9270 2023-01-02 10:31:34.000000 DI-engine-0.4.8/ding/envs/env_manager/tests/test_base_env_manager.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    18474 2023-01-02 10:31:34.000000 DI-engine-0.4.8/ding/envs/env_manager/tests/test_env_supervisor.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1456 2022-07-19 08:28:37.000000 DI-engine-0.4.8/ding/envs/env_manager/tests/test_envpool_env_manager.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2306 2023-01-02 10:31:34.000000 DI-engine-0.4.8/ding/envs/env_manager/tests/test_gym_vector_env_manager.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844      783 2022-07-19 08:28:37.000000 DI-engine-0.4.8/ding/envs/env_manager/tests/test_shm.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     9590 2023-01-02 10:31:34.000000 DI-engine-0.4.8/ding/envs/env_manager/tests/test_subprocess_env_manager.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.428072 DI-engine-0.4.8/ding/envs/env_wrappers/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844       28 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/envs/env_wrappers/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    43614 2023-03-21 10:15:23.000000 DI-engine-0.4.8/ding/envs/env_wrappers/env_wrappers.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.446475 DI-engine-0.4.8/ding/example/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2023-01-04 06:30:14.000000 DI-engine-0.4.8/ding/example/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1997 2023-03-09 07:52:49.000000 DI-engine-0.4.8/ding/example/c51_nstep.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1509 2023-03-06 03:18:03.000000 DI-engine-0.4.8/ding/example/collect_demo_data.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1747 2023-01-06 07:05:23.000000 DI-engine-0.4.8/ding/example/cql.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2098 2023-01-06 07:05:23.000000 DI-engine-0.4.8/ding/example/d4pg.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1962 2023-01-06 07:05:23.000000 DI-engine-0.4.8/ding/example/ddpg.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     4394 2023-01-06 07:05:23.000000 DI-engine-0.4.8/ding/example/dqn.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1928 2023-01-06 07:05:23.000000 DI-engine-0.4.8/ding/example/dqn_her.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1949 2023-01-06 07:05:23.000000 DI-engine-0.4.8/ding/example/dqn_new_env.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2056 2023-01-06 07:05:23.000000 DI-engine-0.4.8/ding/example/dqn_nstep.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2112 2023-01-06 07:05:23.000000 DI-engine-0.4.8/ding/example/dqn_per.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2028 2023-01-06 07:05:23.000000 DI-engine-0.4.8/ding/example/dqn_rnd.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2131 2023-03-08 06:20:41.000000 DI-engine-0.4.8/ding/example/dt.py
+-rwxr-xr-x   0 niuyazhe (1370690143) 453037844     1715 2023-04-28 08:23:39.000000 DI-engine-0.4.8/ding/example/edac.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1991 2023-01-06 07:05:23.000000 DI-engine-0.4.8/ding/example/iqn_nstep.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1933 2023-05-16 06:06:19.000000 DI-engine-0.4.8/ding/example/mappo.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2149 2023-05-16 06:06:19.000000 DI-engine-0.4.8/ding/example/masac.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1838 2023-01-06 07:05:23.000000 DI-engine-0.4.8/ding/example/pdqn.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2539 2023-01-06 07:05:23.000000 DI-engine-0.4.8/ding/example/ppg_offpolicy.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1807 2023-01-06 07:05:23.000000 DI-engine-0.4.8/ding/example/ppo.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1895 2023-01-06 07:05:23.000000 DI-engine-0.4.8/ding/example/ppo_offpolicy.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     7207 2023-04-28 08:20:00.000000 DI-engine-0.4.8/ding/example/ppo_with_complex_obs.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2003 2023-01-06 07:05:23.000000 DI-engine-0.4.8/ding/example/qrdqn_nstep.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1934 2023-01-06 07:05:23.000000 DI-engine-0.4.8/ding/example/r2d2.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1998 2023-01-06 07:05:23.000000 DI-engine-0.4.8/ding/example/sac.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     3213 2023-01-06 07:05:23.000000 DI-engine-0.4.8/ding/example/sqil.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     3377 2023-01-06 07:05:23.000000 DI-engine-0.4.8/ding/example/sqil_continuous.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1842 2023-01-06 07:05:23.000000 DI-engine-0.4.8/ding/example/sql.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1998 2023-05-24 06:35:10.000000 DI-engine-0.4.8/ding/example/td3.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2447 2023-01-06 07:05:23.000000 DI-engine-0.4.8/ding/example/trex.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.450425 DI-engine-0.4.8/ding/framework/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844      361 2022-12-13 15:12:49.000000 DI-engine-0.4.8/ding/framework/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     3247 2023-04-05 10:04:48.000000 DI-engine-0.4.8/ding/framework/context.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     4120 2022-12-13 15:12:49.000000 DI-engine-0.4.8/ding/framework/event_loop.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.453668 DI-engine-0.4.8/ding/framework/message_queue/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844       69 2022-07-19 08:28:37.000000 DI-engine-0.4.8/ding/framework/message_queue/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1635 2022-07-19 08:28:37.000000 DI-engine-0.4.8/ding/framework/message_queue/mq.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2524 2022-12-13 15:12:49.000000 DI-engine-0.4.8/ding/framework/message_queue/nng.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2385 2022-08-02 16:56:36.000000 DI-engine-0.4.8/ding/framework/message_queue/redis.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.457641 DI-engine-0.4.8/ding/framework/middleware/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844      289 2023-04-28 08:20:00.000000 DI-engine-0.4.8/ding/framework/middleware/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    10316 2023-04-28 08:20:00.000000 DI-engine-0.4.8/ding/framework/middleware/barrier.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     3017 2023-01-06 07:05:23.000000 DI-engine-0.4.8/ding/framework/middleware/ckpt_handler.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     8143 2023-02-17 05:18:00.000000 DI-engine-0.4.8/ding/framework/middleware/collector.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    11569 2022-12-13 15:12:49.000000 DI-engine-0.4.8/ding/framework/middleware/distributer.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.463936 DI-engine-0.4.8/ding/framework/middleware/functional/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844      792 2023-01-04 09:44:45.000000 DI-engine-0.4.8/ding/framework/middleware/functional/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     3341 2023-04-28 08:20:00.000000 DI-engine-0.4.8/ding/framework/middleware/functional/advantage_estimator.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     5444 2023-04-28 08:20:00.000000 DI-engine-0.4.8/ding/framework/middleware/functional/collector.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844      912 2023-04-05 10:04:48.000000 DI-engine-0.4.8/ding/framework/middleware/functional/ctx_helper.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    11619 2023-04-17 17:41:31.000000 DI-engine-0.4.8/ding/framework/middleware/functional/data_processor.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     3968 2022-12-13 15:12:50.000000 DI-engine-0.4.8/ding/framework/middleware/functional/enhancer.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    17448 2023-04-05 10:04:48.000000 DI-engine-0.4.8/ding/framework/middleware/functional/evaluator.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1541 2022-12-13 15:12:50.000000 DI-engine-0.4.8/ding/framework/middleware/functional/explorer.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    21320 2023-05-16 06:06:19.000000 DI-engine-0.4.8/ding/framework/middleware/functional/logger.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2054 2022-12-13 15:12:50.000000 DI-engine-0.4.8/ding/framework/middleware/functional/termination_checker.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1021 2022-12-13 15:12:50.000000 DI-engine-0.4.8/ding/framework/middleware/functional/timer.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     4014 2023-05-16 06:06:19.000000 DI-engine-0.4.8/ding/framework/middleware/functional/trainer.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     3960 2023-05-16 06:06:19.000000 DI-engine-0.4.8/ding/framework/middleware/learner.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.472345 DI-engine-0.4.8/ding/framework/middleware/tests/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844       76 2023-05-12 11:44:17.000000 DI-engine-0.4.8/ding/framework/middleware/tests/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     3256 2022-12-13 15:12:50.000000 DI-engine-0.4.8/ding/framework/middleware/tests/mock_for_test.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     3213 2023-03-09 11:08:49.000000 DI-engine-0.4.8/ding/framework/middleware/tests/test_advantage_estimator.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     4256 2023-04-28 08:20:00.000000 DI-engine-0.4.8/ding/framework/middleware/tests/test_barrier.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2074 2023-01-06 07:05:23.000000 DI-engine-0.4.8/ding/framework/middleware/tests/test_ckpt_handler.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     3049 2023-01-04 09:44:45.000000 DI-engine-0.4.8/ding/framework/middleware/tests/test_collector.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     9202 2023-01-04 09:44:45.000000 DI-engine-0.4.8/ding/framework/middleware/tests/test_data_processor.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     7060 2023-04-05 10:04:48.000000 DI-engine-0.4.8/ding/framework/middleware/tests/test_distributer.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2590 2022-12-13 15:12:50.000000 DI-engine-0.4.8/ding/framework/middleware/tests/test_enhancer.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1200 2022-10-19 12:18:13.000000 DI-engine-0.4.8/ding/framework/middleware/tests/test_evaluator.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844      731 2022-07-19 08:28:37.000000 DI-engine-0.4.8/ding/framework/middleware/tests/test_explorer.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     9113 2023-04-05 10:04:48.000000 DI-engine-0.4.8/ding/framework/middleware/tests/test_logger.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     3379 2023-01-29 05:51:23.000000 DI-engine-0.4.8/ding/framework/middleware/tests/test_trainer.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.474810 DI-engine-0.4.8/ding/framework/middleware_v3/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844      167 2022-09-01 10:26:16.000000 DI-engine-0.4.8/ding/framework/middleware_v3/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2553 2022-09-04 07:49:02.000000 DI-engine-0.4.8/ding/framework/middleware_v3/ckpt_handler.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     5011 2022-09-01 10:45:00.000000 DI-engine-0.4.8/ding/framework/middleware_v3/collector.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.481457 DI-engine-0.4.8/ding/framework/middleware_v3/functional/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844      578 2022-09-01 10:26:16.000000 DI-engine-0.4.8/ding/framework/middleware_v3/functional/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2742 2022-09-01 10:26:16.000000 DI-engine-0.4.8/ding/framework/middleware_v3/functional/advantage_estimator.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     5391 2022-09-05 08:12:51.000000 DI-engine-0.4.8/ding/framework/middleware_v3/functional/collector.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844      746 2022-09-01 10:26:16.000000 DI-engine-0.4.8/ding/framework/middleware_v3/functional/ctx_helper.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    10145 2022-09-01 11:15:00.000000 DI-engine-0.4.8/ding/framework/middleware_v3/functional/data_processor.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     3672 2022-09-01 10:26:16.000000 DI-engine-0.4.8/ding/framework/middleware_v3/functional/enhancer.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     7765 2022-09-01 11:07:51.000000 DI-engine-0.4.8/ding/framework/middleware_v3/functional/evaluator.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1408 2022-09-01 10:26:49.000000 DI-engine-0.4.8/ding/framework/middleware_v3/functional/explorer.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844      742 2022-09-01 10:26:16.000000 DI-engine-0.4.8/ding/framework/middleware_v3/functional/termination_checker.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2951 2022-09-01 11:16:03.000000 DI-engine-0.4.8/ding/framework/middleware_v3/functional/trainer.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     3507 2022-09-01 11:09:28.000000 DI-engine-0.4.8/ding/framework/middleware_v3/learner.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.490782 DI-engine-0.4.8/ding/framework/middleware_v3/tests/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844       76 2023-05-12 11:44:18.000000 DI-engine-0.4.8/ding/framework/middleware_v3/tests/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     3252 2022-09-01 10:26:15.000000 DI-engine-0.4.8/ding/framework/middleware_v3/tests/mock_for_test.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     3198 2022-09-01 10:26:15.000000 DI-engine-0.4.8/ding/framework/middleware_v3/tests/test_advantage_estimator.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1987 2022-09-04 07:49:15.000000 DI-engine-0.4.8/ding/framework/middleware_v3/tests/test_ckpt_handler.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     3122 2022-09-01 10:26:15.000000 DI-engine-0.4.8/ding/framework/middleware_v3/tests/test_collector.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     8230 2022-09-01 10:26:16.000000 DI-engine-0.4.8/ding/framework/middleware_v3/tests/test_data_processor.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2642 2022-09-01 10:26:16.000000 DI-engine-0.4.8/ding/framework/middleware_v3/tests/test_enhancer.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1200 2022-09-01 10:26:15.000000 DI-engine-0.4.8/ding/framework/middleware_v3/tests/test_evaluator.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844      731 2022-09-01 10:26:15.000000 DI-engine-0.4.8/ding/framework/middleware_v3/tests/test_explorer.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     3286 2022-09-01 10:26:16.000000 DI-engine-0.4.8/ding/framework/middleware_v3/tests/test_trainer.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    15872 2023-04-28 08:20:00.000000 DI-engine-0.4.8/ding/framework/parallel.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    14388 2023-04-05 10:04:46.000000 DI-engine-0.4.8/ding/framework/supervisor.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    19922 2023-04-28 08:23:39.000000 DI-engine-0.4.8/ding/framework/task.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.492194 DI-engine-0.4.8/ding/framework/wrapper/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844       34 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/framework/wrapper/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1922 2022-12-13 15:12:50.000000 DI-engine-0.4.8/ding/framework/wrapper/step_timer.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.493896 DI-engine-0.4.8/ding/hpc_rl/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844       33 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/hpc_rl/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     5953 2022-12-13 15:12:50.000000 DI-engine-0.4.8/ding/hpc_rl/wrapper.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.494556 DI-engine-0.4.8/ding/interaction/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844       43 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/interaction/__init__.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.497469 DI-engine-0.4.8/ding/interaction/base/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844      382 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/interaction/base/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2806 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/interaction/base/app.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     5341 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/interaction/base/common.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     4846 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/interaction/base/network.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2163 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/interaction/base/threading.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.498315 DI-engine-0.4.8/ding/interaction/config/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844      297 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/interaction/config/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844      432 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/interaction/config/base.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.500328 DI-engine-0.4.8/ding/interaction/exception/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844      848 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/interaction/exception/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2466 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/interaction/exception/base.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     3512 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/interaction/exception/master.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     3914 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/interaction/exception/slave.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.504395 DI-engine-0.4.8/ding/interaction/master/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844       27 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/interaction/master/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844      293 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/interaction/master/base.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    17041 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/interaction/master/connection.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    27918 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/interaction/master/master.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     9524 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/interaction/master/task.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.505715 DI-engine-0.4.8/ding/interaction/slave/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844      105 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/interaction/slave/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     3753 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/interaction/slave/action.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    19857 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/interaction/slave/slave.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.506294 DI-engine-0.4.8/ding/interaction/tests/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844       94 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/interaction/tests/__init__.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.508721 DI-engine-0.4.8/ding/interaction/tests/base/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844      318 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/interaction/tests/base/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     6161 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/interaction/tests/base/test_app.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2036 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/interaction/tests/base/test_common.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     6046 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/interaction/tests/base/test_network.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     3324 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/interaction/tests/base/test_threading.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.509902 DI-engine-0.4.8/ding/interaction/tests/config/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844       45 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/interaction/tests/config/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844      226 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/interaction/tests/config/test_base.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.512431 DI-engine-0.4.8/ding/interaction/tests/exception/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844      110 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/interaction/tests/exception/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1562 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/interaction/tests/exception/test_base.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2877 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/interaction/tests/exception/test_master.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     3293 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/interaction/tests/exception/test_slave.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.514532 DI-engine-0.4.8/ding/interaction/tests/interaction/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844       94 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/interaction/tests/interaction/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1401 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/interaction/tests/interaction/bases.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1439 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/interaction/tests/interaction/test_errors.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     4795 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/interaction/tests/interaction/test_simple.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.515939 DI-engine-0.4.8/ding/interaction/tests/test_utils/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844       94 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/interaction/tests/test_utils/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844      417 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/interaction/tests/test_utils/random.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1099 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/interaction/tests/test_utils/stream.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.520176 DI-engine-0.4.8/ding/league/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844      345 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/league/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1749 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/league/algorithm.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    13037 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/league/base_league.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     4590 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/league/metric.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     5355 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/league/one_vs_one_league.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    13828 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/league/player.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    10938 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/league/shared_payoff.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     9522 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/league/starcraft_player.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.520802 DI-engine-0.4.8/ding/model/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844       69 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/model/__init__.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.523144 DI-engine-0.4.8/ding/model/common/
+-rwxr-xr-x   0 niuyazhe (1370690143) 453037844      369 2023-04-28 08:23:39.000000 DI-engine-0.4.8/ding/model/common/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    12145 2023-03-09 11:08:49.000000 DI-engine-0.4.8/ding/model/common/encoder.py
+-rwxr-xr-x   0 niuyazhe (1370690143) 453037844    61655 2023-04-28 08:23:39.000000 DI-engine-0.4.8/ding/model/common/head.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844      628 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/model/common/utils.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.544409 DI-engine-0.4.8/ding/model/template/
+-rwxr-xr-x   0 niuyazhe (1370690143) 453037844      791 2023-04-28 08:23:39.000000 DI-engine-0.4.8/ding/model/template/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     8851 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/model/template/acer.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    18749 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/model/template/atoc.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     8563 2023-03-09 11:08:49.000000 DI-engine-0.4.8/ding/model/template/bc.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    19316 2022-10-19 09:16:29.000000 DI-engine-0.4.8/ding/model/template/collaq.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     7751 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/model/template/coma.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     4713 2022-07-19 08:28:37.000000 DI-engine-0.4.8/ding/model/template/decision_transformer.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    17708 2022-10-19 09:16:29.000000 DI-engine-0.4.8/ding/model/template/ebm.py
+-rwxr-xr-x   0 niuyazhe (1370690143) 453037844     9122 2023-04-28 08:23:39.000000 DI-engine-0.4.8/ding/model/template/edac.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1790 2022-12-11 15:35:39.000000 DI-engine-0.4.8/ding/model/template/madqn.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    20794 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/model/template/maqac.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    12386 2022-10-19 09:16:29.000000 DI-engine-0.4.8/ding/model/template/mavac.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    10574 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/model/template/ngu.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     9646 2023-03-09 11:08:49.000000 DI-engine-0.4.8/ding/model/template/pdqn.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2793 2022-12-11 15:35:39.000000 DI-engine-0.4.8/ding/model/template/pg.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2389 2022-10-19 09:16:29.000000 DI-engine-0.4.8/ding/model/template/ppg.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     8657 2023-03-09 11:08:49.000000 DI-engine-0.4.8/ding/model/template/procedure_cloning.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    51526 2023-04-05 10:04:48.000000 DI-engine-0.4.8/ding/model/template/q_learning.py
+-rwxr-xr-x   0 niuyazhe (1370690143) 453037844    27157 2023-04-28 08:23:39.000000 DI-engine-0.4.8/ding/model/template/qac.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    12226 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/model/template/qac_dist.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     9551 2022-10-19 09:16:29.000000 DI-engine-0.4.8/ding/model/template/qmix.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     7140 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/model/template/qtran.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844      589 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/model/template/sqn.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    15891 2023-02-23 09:45:40.000000 DI-engine-0.4.8/ding/model/template/vac.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    12328 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/model/template/vae.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    12586 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/model/template/wqmix.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.547637 DI-engine-0.4.8/ding/model/wrapper/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844       90 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/model/wrapper/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    37923 2022-12-13 15:12:50.000000 DI-engine-0.4.8/ding/model/wrapper/model_wrappers.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    21725 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/model/wrapper/test_model_wrappers.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.589409 DI-engine-0.4.8/ding/policy/
+-rwxr-xr-x   0 niuyazhe (1370690143) 453037844     1572 2023-04-28 08:23:39.000000 DI-engine-0.4.8/ding/policy/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    11203 2023-04-05 10:04:48.000000 DI-engine-0.4.8/ding/policy/a2c.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    24338 2023-04-05 10:04:48.000000 DI-engine-0.4.8/ding/policy/acer.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    16201 2023-04-05 10:04:48.000000 DI-engine-0.4.8/ding/policy/atoc.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    11919 2023-04-05 10:04:48.000000 DI-engine-0.4.8/ding/policy/base_policy.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    13093 2023-04-05 10:04:48.000000 DI-engine-0.4.8/ding/policy/bc.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    19714 2023-04-05 10:04:48.000000 DI-engine-0.4.8/ding/policy/bdq.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    12526 2023-04-05 10:04:48.000000 DI-engine-0.4.8/ding/policy/c51.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    21034 2023-04-05 10:04:48.000000 DI-engine-0.4.8/ding/policy/collaq.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    18431 2023-04-05 10:04:48.000000 DI-engine-0.4.8/ding/policy/coma.py
+-rwxr-xr-x   0 niuyazhe (1370690143) 453037844    12332 2023-04-28 08:23:39.000000 DI-engine-0.4.8/ding/policy/command_mode_policy_instance.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1998 2023-03-22 09:00:17.000000 DI-engine-0.4.8/ding/policy/common_utils.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    37331 2023-04-05 10:04:48.000000 DI-engine-0.4.8/ding/policy/cql.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    15951 2023-04-05 10:04:48.000000 DI-engine-0.4.8/ding/policy/d4pg.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    22393 2023-04-05 10:04:48.000000 DI-engine-0.4.8/ding/policy/ddpg.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    15603 2023-04-05 10:04:48.000000 DI-engine-0.4.8/ding/policy/decision_transformer.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    13749 2023-04-05 10:04:48.000000 DI-engine-0.4.8/ding/policy/dqfd.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    36869 2023-04-05 10:04:48.000000 DI-engine-0.4.8/ding/policy/dqn.py
+-rwxr-xr-x   0 niuyazhe (1370690143) 453037844    14959 2023-04-28 08:23:39.000000 DI-engine-0.4.8/ding/policy/edac.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    12436 2023-04-05 10:04:48.000000 DI-engine-0.4.8/ding/policy/fqf.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     6988 2023-04-05 10:04:48.000000 DI-engine-0.4.8/ding/policy/ibc.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     9032 2023-04-05 10:04:48.000000 DI-engine-0.4.8/ding/policy/il.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    23117 2023-04-05 10:04:48.000000 DI-engine-0.4.8/ding/policy/impala.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     9233 2023-04-05 10:04:48.000000 DI-engine-0.4.8/ding/policy/iqn.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    15386 2023-04-05 10:04:48.000000 DI-engine-0.4.8/ding/policy/madqn.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.592054 DI-engine-0.4.8/ding/policy/mbpolicy/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844       31 2022-07-19 08:28:37.000000 DI-engine-0.4.8/ding/policy/mbpolicy/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    15898 2023-04-05 10:04:48.000000 DI-engine-0.4.8/ding/policy/mbpolicy/mbsac.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1318 2022-08-02 16:56:36.000000 DI-engine-0.4.8/ding/policy/mbpolicy/utils.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    12521 2023-04-05 10:04:48.000000 DI-engine-0.4.8/ding/policy/mdqn.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    28541 2023-04-05 10:04:48.000000 DI-engine-0.4.8/ding/policy/ngu.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    13695 2023-04-05 10:04:48.000000 DI-engine-0.4.8/ding/policy/offppo_collect_traj.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     6878 2023-04-05 10:04:48.000000 DI-engine-0.4.8/ding/policy/pc.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    22366 2023-04-05 10:04:48.000000 DI-engine-0.4.8/ding/policy/pdqn.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     8459 2023-04-05 10:04:48.000000 DI-engine-0.4.8/ding/policy/pg.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2892 2023-03-22 09:00:17.000000 DI-engine-0.4.8/ding/policy/policy_factory.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    55970 2023-04-05 10:04:48.000000 DI-engine-0.4.8/ding/policy/ppg.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    56631 2023-04-28 08:20:00.000000 DI-engine-0.4.8/ding/policy/ppo.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    15605 2023-05-12 10:29:30.000000 DI-engine-0.4.8/ding/policy/ppof.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    20183 2023-04-05 10:04:48.000000 DI-engine-0.4.8/ding/policy/qmix.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     9007 2023-04-05 10:04:48.000000 DI-engine-0.4.8/ding/policy/qrdqn.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    21050 2023-04-05 10:04:48.000000 DI-engine-0.4.8/ding/policy/qtran.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    24622 2023-04-05 10:04:48.000000 DI-engine-0.4.8/ding/policy/r2d2.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    23742 2023-04-05 10:04:48.000000 DI-engine-0.4.8/ding/policy/r2d2_collect_traj.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    24134 2023-04-05 10:04:48.000000 DI-engine-0.4.8/ding/policy/r2d2_gtrxl.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    26516 2023-04-05 10:04:48.000000 DI-engine-0.4.8/ding/policy/r2d3.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    13923 2023-04-05 10:04:48.000000 DI-engine-0.4.8/ding/policy/rainbow.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    56374 2023-05-16 06:06:19.000000 DI-engine-0.4.8/ding/policy/sac.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    12620 2023-04-05 10:04:48.000000 DI-engine-0.4.8/ding/policy/sql.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    14436 2023-04-05 10:04:48.000000 DI-engine-0.4.8/ding/policy/sqn.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     9859 2023-05-24 06:38:02.000000 DI-engine-0.4.8/ding/policy/td3.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    17738 2023-04-28 08:23:39.000000 DI-engine-0.4.8/ding/policy/td3_bc.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    32866 2023-04-05 10:04:48.000000 DI-engine-0.4.8/ding/policy/td3_vae.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    15786 2023-04-05 10:04:48.000000 DI-engine-0.4.8/ding/policy/wqmix.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.600697 DI-engine-0.4.8/ding/reward_model/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844      670 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/reward_model/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     4914 2023-03-09 11:08:49.000000 DI-engine-0.4.8/ding/reward_model/base_reward_model.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     4791 2023-04-05 10:04:48.000000 DI-engine-0.4.8/ding/reward_model/drex_reward_model.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    13515 2023-04-05 10:04:48.000000 DI-engine-0.4.8/ding/reward_model/gail_irl_model.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     8298 2023-04-05 10:04:48.000000 DI-engine-0.4.8/ding/reward_model/guided_cost_reward_model.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     6595 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/reward_model/her_reward_model.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    16854 2023-04-05 10:04:48.000000 DI-engine-0.4.8/ding/reward_model/icm_reward_model.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    26350 2023-04-05 10:04:48.000000 DI-engine-0.4.8/ding/reward_model/ngu_reward_model.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     9980 2023-04-05 10:04:48.000000 DI-engine-0.4.8/ding/reward_model/pdeil_irl_model.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    12376 2023-04-05 10:04:48.000000 DI-engine-0.4.8/ding/reward_model/pwil_irl_model.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    10439 2023-04-05 10:04:48.000000 DI-engine-0.4.8/ding/reward_model/red_irl_model.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    12103 2023-04-05 10:04:48.000000 DI-engine-0.4.8/ding/reward_model/rnd_reward_model.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    20419 2023-04-05 10:04:48.000000 DI-engine-0.4.8/ding/reward_model/trex_reward_model.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.612147 DI-engine-0.4.8/ding/rl_utils/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1894 2023-04-11 05:01:52.000000 DI-engine-0.4.8/ding/rl_utils/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1700 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/rl_utils/a2c.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     4723 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/rl_utils/acer.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    10256 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/rl_utils/adder.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1127 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/rl_utils/beta_function.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2438 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/rl_utils/coma.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     7580 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/rl_utils/exploration.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2435 2023-01-02 12:59:23.000000 DI-engine-0.4.8/ding/rl_utils/gae.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2782 2022-12-13 15:12:50.000000 DI-engine-0.4.8/ding/rl_utils/isw.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1409 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/rl_utils/ppg.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    12781 2023-02-21 09:28:07.000000 DI-engine-0.4.8/ding/rl_utils/ppo.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1729 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/rl_utils/retrace.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1510 2023-02-12 11:34:47.000000 DI-engine-0.4.8/ding/rl_utils/sampler.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    62641 2023-04-05 10:04:48.000000 DI-engine-0.4.8/ding/rl_utils/td.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     3752 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/rl_utils/upgo.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2266 2023-04-11 05:01:52.000000 DI-engine-0.4.8/ding/rl_utils/value_rescale.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     9477 2022-12-13 15:12:50.000000 DI-engine-0.4.8/ding/rl_utils/vtrace.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.621341 DI-engine-0.4.8/ding/torch_utils/
+-rwxr-xr-x   0 niuyazhe (1370690143) 453037844      754 2023-04-28 08:23:39.000000 DI-engine-0.4.8/ding/torch_utils/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844      181 2023-04-11 05:01:52.000000 DI-engine-0.4.8/ding/torch_utils/backend_helper.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    12831 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/torch_utils/checkpoint_helper.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    14707 2023-04-28 08:20:00.000000 DI-engine-0.4.8/ding/torch_utils/data_helper.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844      358 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/torch_utils/dataparallel.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     9024 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/torch_utils/distribution.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.624620 DI-engine-0.4.8/ding/torch_utils/loss/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844      178 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/torch_utils/loss/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     4196 2023-01-28 12:50:23.000000 DI-engine-0.4.8/ding/torch_utils/loss/contrastive_loss.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2514 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/torch_utils/loss/cross_entropy_loss.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     4820 2023-01-02 10:31:34.000000 DI-engine-0.4.8/ding/torch_utils/loss/multi_logits_loss.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1273 2023-04-11 05:01:52.000000 DI-engine-0.4.8/ding/torch_utils/lr_scheduler.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1648 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/torch_utils/math_helper.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     3278 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/torch_utils/metric.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844      210 2023-04-11 05:01:52.000000 DI-engine-0.4.8/ding/torch_utils/model_helper.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.635998 DI-engine-0.4.8/ding/torch_utils/network/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844      692 2023-04-28 08:23:39.000000 DI-engine-0.4.8/ding/torch_utils/network/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     3769 2023-04-11 05:01:52.000000 DI-engine-0.4.8/ding/torch_utils/network/activation.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    35769 2022-01-21 07:34:18.000000 DI-engine-0.4.8/ding/torch_utils/network/coverage.xml
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    25400 2022-07-19 08:28:37.000000 DI-engine-0.4.8/ding/torch_utils/network/gtrxl.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1808 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/torch_utils/network/gumbel_softmax.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    26539 2023-05-16 06:06:19.000000 DI-engine-0.4.8/ding/torch_utils/network/nn_module.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1326 2023-05-12 10:29:30.000000 DI-engine-0.4.8/ding/torch_utils/network/normalization.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     4429 2023-05-12 11:44:16.000000 DI-engine-0.4.8/ding/torch_utils/network/popart.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     5700 2023-05-12 10:29:30.000000 DI-engine-0.4.8/ding/torch_utils/network/res_block.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    21848 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/torch_utils/network/resnet.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    13797 2023-04-11 05:01:48.000000 DI-engine-0.4.8/ding/torch_utils/network/rnn.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     3626 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/torch_utils/network/scatter_connection.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1687 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/torch_utils/network/soft_argmax.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     8667 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/torch_utils/network/transformer.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1836 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/torch_utils/nn_test_helper.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    34698 2023-04-11 05:01:52.000000 DI-engine-0.4.8/ding/torch_utils/optimizer_helper.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     3018 2022-08-02 16:56:36.000000 DI-engine-0.4.8/ding/torch_utils/reshape_helper.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.661605 DI-engine-0.4.8/ding/utils/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2609 2023-03-09 11:08:49.000000 DI-engine-0.4.8/ding/utils/__init__.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.665538 DI-engine-0.4.8/ding/utils/autolog/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844      236 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/utils/autolog/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844      701 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/utils/autolog/base.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     5499 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/utils/autolog/data.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     9391 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/utils/autolog/model.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.668130 DI-engine-0.4.8/ding/utils/autolog/tests/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/utils/autolog/tests/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2304 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/utils/autolog/tests/test_data.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    17237 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/utils/autolog/tests/test_model.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     3452 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/utils/autolog/tests/test_time.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     5855 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/utils/autolog/time_ctl.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1407 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/utils/autolog/value.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2264 2023-03-09 11:08:49.000000 DI-engine-0.4.8/ding/utils/bfs_helper.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844      818 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/utils/collection_helper.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     4942 2023-02-13 06:43:00.000000 DI-engine-0.4.8/ding/utils/compression_helper.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844   179593 2021-10-17 09:03:07.000000 DI-engine-0.4.8/ding/utils/coverage.xml
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.672635 DI-engine-0.4.8/ding/utils/data/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844      284 2023-03-06 03:18:03.000000 DI-engine-0.4.8/ding/utils/data/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1052 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/utils/data/base_dataloader.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    11055 2023-04-11 05:01:52.000000 DI-engine-0.4.8/ding/utils/data/collate_fn.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    17023 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/utils/data/dataloader.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    22901 2023-03-09 11:08:49.000000 DI-engine-0.4.8/ding/utils/data/dataset.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.675670 DI-engine-0.4.8/ding/utils/data/structure/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844       59 2022-12-13 15:12:50.000000 DI-engine-0.4.8/ding/utils/data/structure/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     5297 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/utils/data/structure/cache.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844      300 2022-12-13 15:12:50.000000 DI-engine-0.4.8/ding/utils/data/structure/lifo_deque.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    20830 2023-04-28 08:20:00.000000 DI-engine-0.4.8/ding/utils/default_helper.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844      650 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/utils/design_helper.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844      344 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/utils/fake_linklink.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1480 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/utils/fast_copy.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    10416 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/utils/file_helper.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2897 2022-10-19 09:16:29.000000 DI-engine-0.4.8/ding/utils/import_helper.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     7063 2022-10-19 09:16:29.000000 DI-engine-0.4.8/ding/utils/k8s_helper.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     5414 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/utils/linklink_dist_helper.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.681577 DI-engine-0.4.8/ding/utils/loader/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844      783 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/utils/loader/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     4306 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/utils/loader/base.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     3043 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/utils/loader/collection.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844      871 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/utils/loader/dict.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844      369 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/utils/loader/exception.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     3093 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/utils/loader/mapping.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     5747 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/utils/loader/norm.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     6391 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/utils/loader/number.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2228 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/utils/loader/string.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.682447 DI-engine-0.4.8/ding/utils/loader/tests/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844      111 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/utils/loader/tests/__init__.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.687904 DI-engine-0.4.8/ding/utils/loader/tests/loader/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844      426 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/utils/loader/tests/loader/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     5225 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/utils/loader/tests/loader/test_base.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     5989 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/utils/loader/tests/loader/test_collection.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1090 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/utils/loader/tests/loader/test_dict.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1914 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/utils/loader/tests/loader/test_mapping.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    11175 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/utils/loader/tests/loader/test_norm.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    21822 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/utils/loader/tests/loader/test_number.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     4119 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/utils/loader/tests/loader/test_string.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     3183 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/utils/loader/tests/loader/test_types.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1478 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/utils/loader/tests/loader/test_utils.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     4334 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/utils/loader/tests/test_cartpole_dqn_serial_config_loader.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1366 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/utils/loader/types.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844      409 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/utils/loader/utils.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2796 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/utils/lock_helper.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     5332 2022-11-14 04:31:11.000000 DI-engine-0.4.8/ding/utils/log_helper.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     4397 2022-10-19 10:55:38.000000 DI-engine-0.4.8/ding/utils/log_writer_helper.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     4657 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/utils/orchestrator_launcher.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1135 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/utils/profiler_helper.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     3999 2022-12-13 15:12:50.000000 DI-engine-0.4.8/ding/utils/pytorch_ddp_dist_helper.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     3853 2023-01-02 16:52:37.000000 DI-engine-0.4.8/ding/utils/registry.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1495 2022-10-19 09:16:29.000000 DI-engine-0.4.8/ding/utils/registry_factory.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1525 2022-08-02 16:56:36.000000 DI-engine-0.4.8/ding/utils/render_helper.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     7572 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/utils/scheduler_helper.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     9207 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/utils/segment_tree.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2855 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/utils/slurm_helper.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1743 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/utils/system_helper.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     4522 2023-03-09 11:08:49.000000 DI-engine-0.4.8/ding/utils/time_helper.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844      956 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/utils/time_helper_base.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1908 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/utils/time_helper_cuda.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844      173 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/utils/type_helper.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.688693 DI-engine-0.4.8/ding/worker/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844      127 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/worker/__init__.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.690192 DI-engine-0.4.8/ding/worker/adapter/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844       50 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/worker/adapter/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    13378 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/worker/adapter/learner_aggregator.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.699578 DI-engine-0.4.8/ding/worker/collector/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1080 2022-10-19 09:16:29.000000 DI-engine-0.4.8/ding/worker/collector/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     8862 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/worker/collector/base_parallel_collector.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     7839 2023-04-11 13:59:56.000000 DI-engine-0.4.8/ding/worker/collector/base_serial_collector.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     8544 2022-12-26 08:59:29.000000 DI-engine-0.4.8/ding/worker/collector/base_serial_evaluator.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    15584 2023-04-11 13:59:56.000000 DI-engine-0.4.8/ding/worker/collector/battle_episode_serial_collector.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    12112 2023-03-09 11:08:49.000000 DI-engine-0.4.8/ding/worker/collector/battle_interaction_serial_evaluator.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    16387 2023-04-11 13:59:56.000000 DI-engine-0.4.8/ding/worker/collector/battle_sample_serial_collector.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.702844 DI-engine-0.4.8/ding/worker/collector/comm/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844      177 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/worker/collector/comm/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     4089 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/worker/collector/comm/base_comm_collector.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     8874 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/worker/collector/comm/flask_fs_collector.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2436 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/worker/collector/comm/utils.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    14757 2023-04-11 13:59:56.000000 DI-engine-0.4.8/ding/worker/collector/episode_serial_collector.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    13972 2023-04-18 05:25:05.000000 DI-engine-0.4.8/ding/worker/collector/interaction_serial_evaluator.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    14421 2022-12-13 15:12:50.000000 DI-engine-0.4.8/ding/worker/collector/marine_parallel_collector.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     9156 2022-12-13 15:12:50.000000 DI-engine-0.4.8/ding/worker/collector/metric_serial_evaluator.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    17909 2023-05-16 06:06:19.000000 DI-engine-0.4.8/ding/worker/collector/sample_serial_collector.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.707866 DI-engine-0.4.8/ding/worker/collector/tests/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/worker/collector/tests/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844      698 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/worker/collector/tests/fake_cls_policy.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2804 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/worker/collector/tests/fake_cpong_dqn_config.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.712489 DI-engine-0.4.8/ding/worker/collector/tests/speed_test/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/worker/collector/tests/speed_test/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2917 2022-12-13 15:12:50.000000 DI-engine-0.4.8/ding/worker/collector/tests/speed_test/fake_env.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     3034 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/worker/collector/tests/speed_test/fake_policy.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     7399 2023-01-02 10:31:34.000000 DI-engine-0.4.8/ding/worker/collector/tests/speed_test/test_collector_profile.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844      107 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/worker/collector/tests/speed_test/utils.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1705 2023-04-11 13:59:56.000000 DI-engine-0.4.8/ding/worker/collector/tests/test_base_serial_collector.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2277 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/worker/collector/tests/test_episode_serial_collector.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2846 2022-12-13 15:12:50.000000 DI-engine-0.4.8/ding/worker/collector/tests/test_marine_parallel_collector.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     3019 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/worker/collector/tests/test_metric_serial_evaluator.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1693 2023-05-16 06:06:19.000000 DI-engine-0.4.8/ding/worker/collector/tests/test_sample_serial_collector.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    11723 2023-04-05 10:04:48.000000 DI-engine-0.4.8/ding/worker/collector/zergling_parallel_collector.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.718839 DI-engine-0.4.8/ding/worker/coordinator/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844      183 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/worker/coordinator/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     7099 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/worker/coordinator/base_parallel_commander.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2070 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/worker/coordinator/base_serial_commander.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    26271 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/worker/coordinator/comm_coordinator.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    20584 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/worker/coordinator/coordinator.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    16808 2022-12-13 15:12:50.000000 DI-engine-0.4.8/ding/worker/coordinator/one_vs_one_parallel_commander.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     3634 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/worker/coordinator/operator_server.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2675 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/worker/coordinator/resource_manager.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    10871 2022-12-13 15:12:50.000000 DI-engine-0.4.8/ding/worker/coordinator/solo_parallel_commander.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.721527 DI-engine-0.4.8/ding/worker/learner/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844      252 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/worker/learner/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    20149 2023-05-06 14:21:09.000000 DI-engine-0.4.8/ding/worker/learner/base_learner.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.724404 DI-engine-0.4.8/ding/worker/learner/comm/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844      165 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/worker/learner/comm/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     4937 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/worker/learner/comm/base_comm_learner.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    15576 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/worker/learner/comm/flask_fs_learner.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2120 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/worker/learner/comm/utils.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    15500 2022-10-19 09:16:29.000000 DI-engine-0.4.8/ding/worker/learner/learner_hook.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.728762 DI-engine-0.4.8/ding/worker/replay_buffer/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844      206 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/worker/replay_buffer/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    37630 2023-04-05 10:04:48.000000 DI-engine-0.4.8/ding/worker/replay_buffer/advanced_buffer.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     4460 2022-12-11 15:35:39.000000 DI-engine-0.4.8/ding/worker/replay_buffer/base_buffer.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844      800 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/worker/replay_buffer/episode_buffer.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    19279 2022-12-11 15:35:39.000000 DI-engine-0.4.8/ding/worker/replay_buffer/naive_buffer.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    10920 2022-09-30 04:52:24.000000 DI-engine-0.4.8/ding/worker/replay_buffer/utils.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.732906 DI-engine-0.4.8/ding/world_model/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844      139 2022-07-19 08:28:37.000000 DI-engine-0.4.8/ding/world_model/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    13985 2022-08-02 16:56:36.000000 DI-engine-0.4.8/ding/world_model/base_world_model.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    22524 2022-08-02 16:56:36.000000 DI-engine-0.4.8/ding/world_model/ddppo.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     6228 2022-10-19 09:16:29.000000 DI-engine-0.4.8/ding/world_model/idm.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    11421 2022-08-02 16:56:36.000000 DI-engine-0.4.8/ding/world_model/mbpo.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844      852 2022-07-19 08:28:37.000000 DI-engine-0.4.8/ding/world_model/utils.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.733606 DI-engine-0.4.8/dizoo/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2023-03-22 09:07:56.000000 DI-engine-0.4.8/dizoo/__init__.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.733842 DI-engine-0.4.8/dizoo/atari/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2022-09-30 04:52:24.000000 DI-engine-0.4.8/dizoo/atari/__init__.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.734062 DI-engine-0.4.8/dizoo/atari/config/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2022-09-30 04:52:24.000000 DI-engine-0.4.8/dizoo/atari/config/__init__.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.734279 DI-engine-0.4.8/dizoo/atari/config/serial/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844      239 2023-03-09 11:08:49.000000 DI-engine-0.4.8/dizoo/atari/config/serial/__init__.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.735277 DI-engine-0.4.8/dizoo/atari/config/serial/asterix/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844       82 2023-03-09 11:08:49.000000 DI-engine-0.4.8/dizoo/atari/config/serial/asterix/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1924 2023-05-12 10:29:30.000000 DI-engine-0.4.8/dizoo/atari/config/serial/asterix/asterix_mdqn_config.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.741277 DI-engine-0.4.8/dizoo/atari/config/serial/enduro/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844       76 2022-07-19 08:28:37.000000 DI-engine-0.4.8/dizoo/atari/config/serial/enduro/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1742 2023-05-12 10:29:30.000000 DI-engine-0.4.8/dizoo/atari/config/serial/enduro/enduro_dqn_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2987 2023-05-12 10:29:30.000000 DI-engine-0.4.8/dizoo/atari/config/serial/enduro/enduro_impala_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1911 2023-05-12 10:29:30.000000 DI-engine-0.4.8/dizoo/atari/config/serial/enduro/enduro_mdqn_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2248 2023-05-12 10:29:30.000000 DI-engine-0.4.8/dizoo/atari/config/serial/enduro/enduro_onppo_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1769 2023-05-12 10:29:30.000000 DI-engine-0.4.8/dizoo/atari/config/serial/enduro/enduro_qrdqn_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1827 2023-05-12 10:29:30.000000 DI-engine-0.4.8/dizoo/atari/config/serial/enduro/enduro_rainbow_config.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.762385 DI-engine-0.4.8/dizoo/atari/config/serial/pong/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844      233 2022-07-19 08:28:37.000000 DI-engine-0.4.8/dizoo/atari/config/serial/pong/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2075 2023-05-12 10:29:30.000000 DI-engine-0.4.8/dizoo/atari/config/serial/pong/pong_a2c_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2491 2023-05-12 10:29:30.000000 DI-engine-0.4.8/dizoo/atari/config/serial/pong/pong_acer_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1753 2023-05-12 10:29:30.000000 DI-engine-0.4.8/dizoo/atari/config/serial/pong/pong_c51_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2134 2023-05-12 10:29:30.000000 DI-engine-0.4.8/dizoo/atari/config/serial/pong/pong_cql_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2888 2023-05-12 10:29:30.000000 DI-engine-0.4.8/dizoo/atari/config/serial/pong/pong_dqfd_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1684 2023-05-12 10:29:30.000000 DI-engine-0.4.8/dizoo/atari/config/serial/pong/pong_dqn_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1864 2023-05-12 10:29:30.000000 DI-engine-0.4.8/dizoo/atari/config/serial/pong/pong_dqn_envpool_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1718 2023-05-12 10:29:30.000000 DI-engine-0.4.8/dizoo/atari/config/serial/pong/pong_dqn_multi_gpu_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1825 2023-05-12 10:29:30.000000 DI-engine-0.4.8/dizoo/atari/config/serial/pong/pong_dqn_render_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1986 2023-05-12 10:29:30.000000 DI-engine-0.4.8/dizoo/atari/config/serial/pong/pong_dqn_stdim_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1795 2023-05-12 10:29:30.000000 DI-engine-0.4.8/dizoo/atari/config/serial/pong/pong_fqf_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     3120 2023-05-12 10:29:30.000000 DI-engine-0.4.8/dizoo/atari/config/serial/pong/pong_gail_dqn_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2746 2023-05-12 10:29:30.000000 DI-engine-0.4.8/dizoo/atari/config/serial/pong/pong_impala_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1735 2023-05-12 10:29:30.000000 DI-engine-0.4.8/dizoo/atari/config/serial/pong/pong_iqn_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     5000 2023-05-12 10:29:30.000000 DI-engine-0.4.8/dizoo/atari/config/serial/pong/pong_ngu_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2148 2023-05-12 10:29:30.000000 DI-engine-0.4.8/dizoo/atari/config/serial/pong/pong_onppo_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2626 2023-05-12 10:29:30.000000 DI-engine-0.4.8/dizoo/atari/config/serial/pong/pong_ppg_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1737 2023-05-12 10:29:30.000000 DI-engine-0.4.8/dizoo/atari/config/serial/pong/pong_qrdqn_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2076 2023-05-12 10:29:30.000000 DI-engine-0.4.8/dizoo/atari/config/serial/pong/pong_qrdqn_generation_data_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     3311 2023-05-12 10:29:30.000000 DI-engine-0.4.8/dizoo/atari/config/serial/pong/pong_r2d2_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     3022 2023-05-12 10:29:30.000000 DI-engine-0.4.8/dizoo/atari/config/serial/pong/pong_r2d2_gtrxl_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     3028 2023-05-12 10:29:30.000000 DI-engine-0.4.8/dizoo/atari/config/serial/pong/pong_r2d2_residual_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     6468 2023-05-12 10:29:30.000000 DI-engine-0.4.8/dizoo/atari/config/serial/pong/pong_r2d3_offppoexpert_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     6817 2023-05-12 10:29:30.000000 DI-engine-0.4.8/dizoo/atari/config/serial/pong/pong_r2d3_r2d2expert_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1740 2023-05-12 10:29:30.000000 DI-engine-0.4.8/dizoo/atari/config/serial/pong/pong_rainbow_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2301 2023-05-12 10:29:30.000000 DI-engine-0.4.8/dizoo/atari/config/serial/pong/pong_sqil_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1582 2023-05-12 10:29:30.000000 DI-engine-0.4.8/dizoo/atari/config/serial/pong/pong_sql_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     4229 2023-05-12 10:29:30.000000 DI-engine-0.4.8/dizoo/atari/config/serial/pong/pong_trex_offppo_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     3572 2023-05-12 10:29:30.000000 DI-engine-0.4.8/dizoo/atari/config/serial/pong/pong_trex_sql_config.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.777739 DI-engine-0.4.8/dizoo/atari/config/serial/qbert/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844      146 2022-07-19 08:28:37.000000 DI-engine-0.4.8/dizoo/atari/config/serial/qbert/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2069 2023-05-12 10:29:30.000000 DI-engine-0.4.8/dizoo/atari/config/serial/qbert/qbert_a2c_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2552 2023-05-12 10:29:30.000000 DI-engine-0.4.8/dizoo/atari/config/serial/qbert/qbert_acer_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1680 2023-05-12 10:29:30.000000 DI-engine-0.4.8/dizoo/atari/config/serial/qbert/qbert_c51_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2087 2023-05-12 10:29:30.000000 DI-engine-0.4.8/dizoo/atari/config/serial/qbert/qbert_cql_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2743 2023-05-12 10:29:30.000000 DI-engine-0.4.8/dizoo/atari/config/serial/qbert/qbert_dqfd_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1698 2023-05-12 10:29:30.000000 DI-engine-0.4.8/dizoo/atari/config/serial/qbert/qbert_dqn_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1855 2023-05-12 10:29:30.000000 DI-engine-0.4.8/dizoo/atari/config/serial/qbert/qbert_fqf_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2819 2023-05-12 10:29:30.000000 DI-engine-0.4.8/dizoo/atari/config/serial/qbert/qbert_impala_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1661 2023-05-12 10:29:30.000000 DI-engine-0.4.8/dizoo/atari/config/serial/qbert/qbert_iqn_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2165 2023-05-12 10:29:30.000000 DI-engine-0.4.8/dizoo/atari/config/serial/qbert/qbert_offppo_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2195 2023-05-12 10:29:30.000000 DI-engine-0.4.8/dizoo/atari/config/serial/qbert/qbert_onppo_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2470 2023-05-12 10:29:30.000000 DI-engine-0.4.8/dizoo/atari/config/serial/qbert/qbert_ppg_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1656 2023-05-12 10:29:30.000000 DI-engine-0.4.8/dizoo/atari/config/serial/qbert/qbert_qrdqn_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2084 2023-05-12 10:29:30.000000 DI-engine-0.4.8/dizoo/atari/config/serial/qbert/qbert_qrdqn_generation_data_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     3398 2023-05-12 10:29:30.000000 DI-engine-0.4.8/dizoo/atari/config/serial/qbert/qbert_r2d2_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2771 2023-05-12 10:29:30.000000 DI-engine-0.4.8/dizoo/atari/config/serial/qbert/qbert_r2d2_gtrxl_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1768 2023-05-12 10:29:30.000000 DI-engine-0.4.8/dizoo/atari/config/serial/qbert/qbert_rainbow_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2426 2023-05-12 10:29:30.000000 DI-engine-0.4.8/dizoo/atari/config/serial/qbert/qbert_sqil_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1695 2023-05-12 10:29:30.000000 DI-engine-0.4.8/dizoo/atari/config/serial/qbert/qbert_sql_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     3012 2023-05-12 10:29:30.000000 DI-engine-0.4.8/dizoo/atari/config/serial/qbert/qbert_trex_dqn_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     3453 2023-05-12 10:29:30.000000 DI-engine-0.4.8/dizoo/atari/config/serial/qbert/qbert_trex_offppo_config.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.789758 DI-engine-0.4.8/dizoo/atari/config/serial/spaceinvaders/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844      194 2022-07-19 08:28:37.000000 DI-engine-0.4.8/dizoo/atari/config/serial/spaceinvaders/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2277 2023-05-12 10:29:30.000000 DI-engine-0.4.8/dizoo/atari/config/serial/spaceinvaders/spaceinvaders_a2c_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2822 2023-05-12 10:29:30.000000 DI-engine-0.4.8/dizoo/atari/config/serial/spaceinvaders/spaceinvaders_acer_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1948 2023-05-12 10:29:30.000000 DI-engine-0.4.8/dizoo/atari/config/serial/spaceinvaders/spaceinvaders_c51_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2936 2023-05-12 10:29:30.000000 DI-engine-0.4.8/dizoo/atari/config/serial/spaceinvaders/spaceinvaders_dqfd_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2040 2023-05-12 10:29:30.000000 DI-engine-0.4.8/dizoo/atari/config/serial/spaceinvaders/spaceinvaders_dqn_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1902 2023-05-12 10:29:30.000000 DI-engine-0.4.8/dizoo/atari/config/serial/spaceinvaders/spaceinvaders_dqn_config_multi_gpu_ddp.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1989 2023-05-12 10:29:30.000000 DI-engine-0.4.8/dizoo/atari/config/serial/spaceinvaders/spaceinvaders_dqn_config_multi_gpu_dp.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1950 2023-05-12 10:29:30.000000 DI-engine-0.4.8/dizoo/atari/config/serial/spaceinvaders/spaceinvaders_fqf_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     3116 2023-05-12 10:29:30.000000 DI-engine-0.4.8/dizoo/atari/config/serial/spaceinvaders/spaceinvaders_impala_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1920 2023-05-12 10:29:30.000000 DI-engine-0.4.8/dizoo/atari/config/serial/spaceinvaders/spaceinvaders_iqn_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1990 2023-05-12 10:29:30.000000 DI-engine-0.4.8/dizoo/atari/config/serial/spaceinvaders/spaceinvaders_mdqn_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2406 2023-05-12 10:29:30.000000 DI-engine-0.4.8/dizoo/atari/config/serial/spaceinvaders/spaceinvaders_offppo_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2321 2023-05-12 10:29:30.000000 DI-engine-0.4.8/dizoo/atari/config/serial/spaceinvaders/spaceinvaders_onppo_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2727 2023-05-12 10:29:30.000000 DI-engine-0.4.8/dizoo/atari/config/serial/spaceinvaders/spaceinvaders_ppg_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1923 2023-05-12 10:29:30.000000 DI-engine-0.4.8/dizoo/atari/config/serial/spaceinvaders/spaceinvaders_qrdqn_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     3503 2023-05-12 10:29:30.000000 DI-engine-0.4.8/dizoo/atari/config/serial/spaceinvaders/spaceinvaders_r2d2_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     3044 2023-05-12 10:29:30.000000 DI-engine-0.4.8/dizoo/atari/config/serial/spaceinvaders/spaceinvaders_r2d2_gtrxl_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     3178 2023-05-12 10:29:30.000000 DI-engine-0.4.8/dizoo/atari/config/serial/spaceinvaders/spaceinvaders_r2d2_residual_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2042 2023-05-12 10:29:30.000000 DI-engine-0.4.8/dizoo/atari/config/serial/spaceinvaders/spaceinvaders_rainbow_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2527 2023-05-12 10:29:30.000000 DI-engine-0.4.8/dizoo/atari/config/serial/spaceinvaders/spaceinvaders_sqil_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1838 2023-05-12 10:29:30.000000 DI-engine-0.4.8/dizoo/atari/config/serial/spaceinvaders/spaceinvaders_sql_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     4066 2023-05-12 10:29:30.000000 DI-engine-0.4.8/dizoo/atari/config/serial/spaceinvaders/spaceinvaders_trex_dqn_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     4565 2023-05-12 10:29:30.000000 DI-engine-0.4.8/dizoo/atari/config/serial/spaceinvaders/spaceinvaders_trex_offppo_config.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.798427 DI-engine-0.4.8/dizoo/atari/entry/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2022-09-30 04:52:24.000000 DI-engine-0.4.8/dizoo/atari/entry/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     3135 2022-09-30 04:52:24.000000 DI-engine-0.4.8/dizoo/atari/entry/atari_dqn_main.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     3534 2022-09-30 04:52:24.000000 DI-engine-0.4.8/dizoo/atari/entry/atari_ppg_main.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     3272 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/atari/entry/phoenix_fqf_main.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     3272 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/atari/entry/phoenix_iqn_main.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2118 2022-09-30 04:52:24.000000 DI-engine-0.4.8/dizoo/atari/entry/pong_cql_main.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     3743 2022-07-19 08:28:38.000000 DI-engine-0.4.8/dizoo/atari/entry/pong_dqn_envpool_main.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     3260 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/atari/entry/pong_fqf_main.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2151 2022-09-30 04:52:24.000000 DI-engine-0.4.8/dizoo/atari/entry/qbert_cql_main.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     3264 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/atari/entry/qbert_fqf_main.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2185 2022-12-13 15:12:50.000000 DI-engine-0.4.8/dizoo/atari/entry/spaceinvaders_dqn_eval.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     3251 2022-09-30 04:52:24.000000 DI-engine-0.4.8/dizoo/atari/entry/spaceinvaders_dqn_main_multi_gpu_ddp.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     3261 2022-09-30 04:52:24.000000 DI-engine-0.4.8/dizoo/atari/entry/spaceinvaders_dqn_main_multi_gpu_dp.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     3296 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/atari/entry/spaceinvaders_fqf_main.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.801376 DI-engine-0.4.8/dizoo/atari/envs/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844       44 2022-09-30 04:52:24.000000 DI-engine-0.4.8/dizoo/atari/envs/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     5233 2022-12-13 15:12:50.000000 DI-engine-0.4.8/dizoo/atari/envs/atari_env.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     6246 2022-11-14 04:31:11.000000 DI-engine-0.4.8/dizoo/atari/envs/atari_wrappers.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2440 2022-12-13 15:12:50.000000 DI-engine-0.4.8/dizoo/atari/envs/test_atari_env.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.802091 DI-engine-0.4.8/dizoo/beergame/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2023-01-17 12:06:07.000000 DI-engine-0.4.8/dizoo/beergame/__init__.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.806990 DI-engine-0.4.8/dizoo/beergame/envs/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     8359 2022-12-13 15:12:50.000000 DI-engine-0.4.8/dizoo/beergame/envs/BGAgent.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844       71 2022-11-14 04:31:11.000000 DI-engine-0.4.8/dizoo/beergame/envs/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     4738 2022-11-14 04:31:11.000000 DI-engine-0.4.8/dizoo/beergame/envs/beergame_core.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     3046 2022-12-13 15:12:50.000000 DI-engine-0.4.8/dizoo/beergame/envs/beergame_env.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    23724 2022-11-14 04:31:11.000000 DI-engine-0.4.8/dizoo/beergame/envs/clBeergame.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2721 2022-11-14 04:31:11.000000 DI-engine-0.4.8/dizoo/beergame/envs/plotting.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    17343 2022-11-14 04:31:11.000000 DI-engine-0.4.8/dizoo/beergame/envs/utils.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.807694 DI-engine-0.4.8/dizoo/bitflip/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2022-03-14 08:09:40.000000 DI-engine-0.4.8/dizoo/bitflip/__init__.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.809172 DI-engine-0.4.8/dizoo/bitflip/config/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844      183 2022-09-30 04:52:24.000000 DI-engine-0.4.8/dizoo/bitflip/config/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2616 2022-09-30 04:52:24.000000 DI-engine-0.4.8/dizoo/bitflip/config/bitflip_her_dqn_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1740 2022-09-30 04:52:24.000000 DI-engine-0.4.8/dizoo/bitflip/config/bitflip_pure_dqn_config.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.810040 DI-engine-0.4.8/dizoo/bitflip/entry/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2022-03-14 08:09:40.000000 DI-engine-0.4.8/dizoo/bitflip/entry/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     4350 2022-09-30 04:52:24.000000 DI-engine-0.4.8/dizoo/bitflip/entry/bitflip_dqn_main.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.812256 DI-engine-0.4.8/dizoo/bitflip/envs/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844       36 2022-09-30 04:52:24.000000 DI-engine-0.4.8/dizoo/bitflip/envs/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     3261 2022-12-13 15:12:50.000000 DI-engine-0.4.8/dizoo/bitflip/envs/bitflip_env.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844      756 2022-09-30 04:52:24.000000 DI-engine-0.4.8/dizoo/bitflip/envs/test_bitfilp_env.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.812840 DI-engine-0.4.8/dizoo/box2d/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2022-09-30 04:52:24.000000 DI-engine-0.4.8/dizoo/box2d/__init__.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.813208 DI-engine-0.4.8/dizoo/box2d/bipedalwalker/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844       47 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/box2d/bipedalwalker/__init__.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.820917 DI-engine-0.4.8/dizoo/box2d/bipedalwalker/config/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844       96 2022-07-19 08:28:38.000000 DI-engine-0.4.8/dizoo/box2d/bipedalwalker/config/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     3050 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/box2d/bipedalwalker/config/bipedalwalker_bco_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1834 2023-05-12 10:29:30.000000 DI-engine-0.4.8/dizoo/box2d/bipedalwalker/config/bipedalwalker_ddpg_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2504 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/box2d/bipedalwalker/config/bipedalwalker_dt_config.py
+-rwxr-xr-x   0 niuyazhe (1370690143) 453037844     3504 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/box2d/bipedalwalker/config/bipedalwalker_gail_sac_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2819 2022-12-13 15:12:50.000000 DI-engine-0.4.8/dizoo/box2d/bipedalwalker/config/bipedalwalker_impala_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1837 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/box2d/bipedalwalker/config/bipedalwalker_ppo_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2644 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/box2d/bipedalwalker/config/bipedalwalker_ppopg_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1951 2023-05-12 10:29:30.000000 DI-engine-0.4.8/dizoo/box2d/bipedalwalker/config/bipedalwalker_sac_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2004 2023-05-12 10:29:30.000000 DI-engine-0.4.8/dizoo/box2d/bipedalwalker/config/bipedalwalker_td3_config.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.824514 DI-engine-0.4.8/dizoo/box2d/bipedalwalker/entry/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/box2d/bipedalwalker/entry/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2181 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/box2d/bipedalwalker/entry/bipedalwalker_ppo_eval.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.826225 DI-engine-0.4.8/dizoo/box2d/bipedalwalker/envs/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844       48 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/box2d/bipedalwalker/envs/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     3868 2022-12-13 15:12:50.000000 DI-engine-0.4.8/dizoo/box2d/bipedalwalker/envs/bipedalwalker_env.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1034 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/box2d/bipedalwalker/envs/test_bipedalwalker.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.826763 DI-engine-0.4.8/dizoo/box2d/carracing/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2023-02-13 06:42:54.000000 DI-engine-0.4.8/dizoo/box2d/carracing/__init__.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.827588 DI-engine-0.4.8/dizoo/box2d/carracing/config/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844       85 2023-02-13 06:42:54.000000 DI-engine-0.4.8/dizoo/box2d/carracing/config/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1767 2023-02-13 06:42:54.000000 DI-engine-0.4.8/dizoo/box2d/carracing/config/carracing_dqn_config.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.829372 DI-engine-0.4.8/dizoo/box2d/carracing/envs/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844       41 2023-02-13 06:42:54.000000 DI-engine-0.4.8/dizoo/box2d/carracing/envs/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     5913 2023-02-13 06:42:54.000000 DI-engine-0.4.8/dizoo/box2d/carracing/envs/carracing_env.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1082 2023-02-13 06:42:54.000000 DI-engine-0.4.8/dizoo/box2d/carracing/envs/test_carracing_env.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.829824 DI-engine-0.4.8/dizoo/box2d/lunarlander/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/box2d/lunarlander/__init__.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.847409 DI-engine-0.4.8/dizoo/box2d/lunarlander/config/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844      597 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/box2d/lunarlander/config/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1375 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/box2d/lunarlander/config/lunarlander_a2c_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     3181 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/box2d/lunarlander/config/lunarlander_acer_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2827 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/box2d/lunarlander/config/lunarlander_bco_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1671 2023-04-05 10:04:48.000000 DI-engine-0.4.8/dizoo/box2d/lunarlander/config/lunarlander_c51_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2418 2023-05-12 10:29:23.000000 DI-engine-0.4.8/dizoo/box2d/lunarlander/config/lunarlander_cont_ddpg_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1677 2023-05-12 10:29:23.000000 DI-engine-0.4.8/dizoo/box2d/lunarlander/config/lunarlander_cont_sac_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1817 2023-05-12 10:29:23.000000 DI-engine-0.4.8/dizoo/box2d/lunarlander/config/lunarlander_cont_td3_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2269 2023-05-12 10:29:23.000000 DI-engine-0.4.8/dizoo/box2d/lunarlander/config/lunarlander_cont_td3_vae_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2484 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/box2d/lunarlander/config/lunarlander_decision_transformer.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2086 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/box2d/lunarlander/config/lunarlander_discrete_sac_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2888 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/box2d/lunarlander/config/lunarlander_dqfd_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2636 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/box2d/lunarlander/config/lunarlander_dqn_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2541 2023-04-05 10:04:48.000000 DI-engine-0.4.8/dizoo/box2d/lunarlander/config/lunarlander_dqn_deque_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     3962 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/box2d/lunarlander/config/lunarlander_gail_dqn_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2272 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/box2d/lunarlander/config/lunarlander_gcl_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     5345 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/box2d/lunarlander/config/lunarlander_ngu_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1502 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/box2d/lunarlander/config/lunarlander_offppo_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1381 2022-12-11 15:35:39.000000 DI-engine-0.4.8/dizoo/box2d/lunarlander/config/lunarlander_pg_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1530 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/box2d/lunarlander/config/lunarlander_qrdqn_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     3325 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/box2d/lunarlander/config/lunarlander_r2d2_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     3056 2022-07-19 08:28:38.000000 DI-engine-0.4.8/dizoo/box2d/lunarlander/config/lunarlander_r2d2_gtrxl_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     6624 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/box2d/lunarlander/config/lunarlander_r2d3_ppoexpert_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     6992 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/box2d/lunarlander/config/lunarlander_r2d3_r2d2expert_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2612 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/box2d/lunarlander/config/lunarlander_rnd_onppo_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2498 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/box2d/lunarlander/config/lunarlander_sqil_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1623 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/box2d/lunarlander/config/lunarlander_sql_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     4289 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/box2d/lunarlander/config/lunarlander_trex_dqn_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     3462 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/box2d/lunarlander/config/lunarlander_trex_offppo_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     8211 2022-09-28 13:14:17.000000 DI-engine-0.4.8/dizoo/box2d/lunarlander/config/t.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.849208 DI-engine-0.4.8/dizoo/box2d/lunarlander/entry/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/box2d/lunarlander/entry/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2177 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/box2d/lunarlander/entry/lunarlander_dqn_eval.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2985 2023-02-13 06:56:00.000000 DI-engine-0.4.8/dizoo/box2d/lunarlander/entry/lunarlander_dqn_example.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.851112 DI-engine-0.4.8/dizoo/box2d/lunarlander/envs/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844       44 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/box2d/lunarlander/envs/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     5535 2022-12-13 15:12:50.000000 DI-engine-0.4.8/dizoo/box2d/lunarlander/envs/lunarlander_env.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1248 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/box2d/lunarlander/envs/test_lunarlander_env.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.851671 DI-engine-0.4.8/dizoo/bsuite/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/bsuite/__init__.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.852012 DI-engine-0.4.8/dizoo/bsuite/config/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844        1 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/bsuite/config/__init__.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.854487 DI-engine-0.4.8/dizoo/bsuite/envs/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844       34 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/bsuite/envs/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     3752 2022-12-13 15:12:50.000000 DI-engine-0.4.8/dizoo/bsuite/envs/bsuite_env.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1467 2022-12-13 15:12:50.000000 DI-engine-0.4.8/dizoo/bsuite/envs/test_bsuite_env.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.855282 DI-engine-0.4.8/dizoo/classic_control/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/classic_control/__init__.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.855632 DI-engine-0.4.8/dizoo/classic_control/acrobot/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2023-02-13 06:42:54.000000 DI-engine-0.4.8/dizoo/classic_control/acrobot/__init__.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.856529 DI-engine-0.4.8/dizoo/classic_control/acrobot/config/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844       79 2023-02-13 06:42:54.000000 DI-engine-0.4.8/dizoo/classic_control/acrobot/config/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1659 2023-02-13 06:42:54.000000 DI-engine-0.4.8/dizoo/classic_control/acrobot/config/acrobot_dqn_config.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.858751 DI-engine-0.4.8/dizoo/classic_control/acrobot/envs/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844       37 2023-02-13 06:42:54.000000 DI-engine-0.4.8/dizoo/classic_control/acrobot/envs/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     3591 2023-02-13 06:42:54.000000 DI-engine-0.4.8/dizoo/classic_control/acrobot/envs/acrobot_env.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1323 2023-02-13 06:42:54.000000 DI-engine-0.4.8/dizoo/classic_control/acrobot/envs/test_acrobot_env.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.859323 DI-engine-0.4.8/dizoo/classic_control/cartpole/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/classic_control/cartpole/__init__.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.884921 DI-engine-0.4.8/dizoo/classic_control/cartpole/config/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2040 2023-03-09 11:08:49.000000 DI-engine-0.4.8/dizoo/classic_control/cartpole/config/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1682 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/classic_control/cartpole/config/cartpole_a2c_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2489 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/classic_control/cartpole/config/cartpole_acer_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1330 2023-02-13 06:42:54.000000 DI-engine-0.4.8/dizoo/classic_control/cartpole/config/cartpole_bc_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2524 2022-10-31 06:23:20.000000 DI-engine-0.4.8/dizoo/classic_control/cartpole/config/cartpole_bco_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1687 2023-01-06 07:05:23.000000 DI-engine-0.4.8/dizoo/classic_control/cartpole/config/cartpole_c51_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1649 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/classic_control/cartpole/config/cartpole_cql_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2585 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/classic_control/cartpole/config/cartpole_decision_transformer.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2849 2023-02-22 06:18:30.000000 DI-engine-0.4.8/dizoo/classic_control/cartpole/config/cartpole_dqfd_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1776 2023-02-22 06:18:46.000000 DI-engine-0.4.8/dizoo/classic_control/cartpole/config/cartpole_dqn_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2701 2022-10-31 06:23:20.000000 DI-engine-0.4.8/dizoo/classic_control/cartpole/config/cartpole_dqn_gail_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1556 2022-07-19 08:28:38.000000 DI-engine-0.4.8/dizoo/classic_control/cartpole/config/cartpole_dqn_rnd_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2055 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/classic_control/cartpole/config/cartpole_dqn_stdim_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     3173 2022-11-14 04:31:11.000000 DI-engine-0.4.8/dizoo/classic_control/cartpole/config/cartpole_drex_dqn_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1813 2022-07-19 08:28:38.000000 DI-engine-0.4.8/dizoo/classic_control/cartpole/config/cartpole_fqf_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2423 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/classic_control/cartpole/config/cartpole_gcl_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2781 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/classic_control/cartpole/config/cartpole_impala_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1649 2023-01-06 07:05:23.000000 DI-engine-0.4.8/dizoo/classic_control/cartpole/config/cartpole_iqn_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1721 2023-03-09 11:08:49.000000 DI-engine-0.4.8/dizoo/classic_control/cartpole/config/cartpole_mdqn_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     4857 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/classic_control/cartpole/config/cartpole_ngu_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1277 2022-12-11 15:35:39.000000 DI-engine-0.4.8/dizoo/classic_control/cartpole/config/cartpole_pg_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2357 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/classic_control/cartpole/config/cartpole_ppg_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1684 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/classic_control/cartpole/config/cartpole_ppo_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1894 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/classic_control/cartpole/config/cartpole_ppo_icm_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1797 2023-01-06 07:05:23.000000 DI-engine-0.4.8/dizoo/classic_control/cartpole/config/cartpole_ppo_offpolicy_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2084 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/classic_control/cartpole/config/cartpole_ppo_stdim_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1383 2022-12-11 15:35:39.000000 DI-engine-0.4.8/dizoo/classic_control/cartpole/config/cartpole_ppopg_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1672 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/classic_control/cartpole/config/cartpole_qrdqn_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1739 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/classic_control/cartpole/config/cartpole_qrdqn_generation_data_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2909 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/classic_control/cartpole/config/cartpole_r2d2_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2775 2022-07-19 08:28:38.000000 DI-engine-0.4.8/dizoo/classic_control/cartpole/config/cartpole_r2d2_gtrxl_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     3219 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/classic_control/cartpole/config/cartpole_r2d2_residual_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1664 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/classic_control/cartpole/config/cartpole_rainbow_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2245 2023-03-09 11:08:49.000000 DI-engine-0.4.8/dizoo/classic_control/cartpole/config/cartpole_rnd_onppo_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1998 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/classic_control/cartpole/config/cartpole_sac_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2258 2023-01-06 07:05:23.000000 DI-engine-0.4.8/dizoo/classic_control/cartpole/config/cartpole_sqil_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1554 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/classic_control/cartpole/config/cartpole_sql_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1702 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/classic_control/cartpole/config/cartpole_sqn_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2845 2023-01-06 07:05:23.000000 DI-engine-0.4.8/dizoo/classic_control/cartpole/config/cartpole_trex_dqn_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2948 2023-02-13 06:42:54.000000 DI-engine-0.4.8/dizoo/classic_control/cartpole/config/cartpole_trex_offppo_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     3044 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/classic_control/cartpole/config/cartpole_trex_onppo_config.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.886036 DI-engine-0.4.8/dizoo/classic_control/cartpole/config/parallel/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844      109 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/classic_control/cartpole/config/parallel/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2921 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/classic_control/cartpole/config/parallel/cartpole_dqn_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     3286 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/classic_control/cartpole/config/parallel/cartpole_dqn_config_k8s.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.891040 DI-engine-0.4.8/dizoo/classic_control/cartpole/entry/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/classic_control/cartpole/entry/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1282 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/classic_control/cartpole/entry/cartpole_c51_deploy.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     3403 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/classic_control/cartpole/entry/cartpole_c51_main.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2217 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/classic_control/cartpole/entry/cartpole_cql_main.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     3391 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/classic_control/cartpole/entry/cartpole_dqn_buffer_main.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2014 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/classic_control/cartpole/entry/cartpole_dqn_eval.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     3857 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/classic_control/cartpole/entry/cartpole_dqn_main.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     3959 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/classic_control/cartpole/entry/cartpole_fqf_main.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     3582 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/classic_control/cartpole/entry/cartpole_ppg_main.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2278 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/classic_control/cartpole/entry/cartpole_ppo_main.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2781 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/classic_control/cartpole/entry/cartpole_ppo_offpolicy_main.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2470 2021-07-16 08:07:45.000000 DI-engine-0.4.8/dizoo/classic_control/cartpole/entry/formatted_total_config.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.893052 DI-engine-0.4.8/dizoo/classic_control/cartpole/envs/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844       38 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/classic_control/cartpole/envs/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     3774 2022-12-13 15:12:50.000000 DI-engine-0.4.8/dizoo/classic_control/cartpole/envs/cartpole_env.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1327 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/classic_control/cartpole/envs/test_cartpole_env.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1350 2022-07-19 08:28:38.000000 DI-engine-0.4.8/dizoo/classic_control/cartpole/envs/test_cartpole_env_manager.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.893644 DI-engine-0.4.8/dizoo/classic_control/mountain_car/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/classic_control/mountain_car/__init__.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.894863 DI-engine-0.4.8/dizoo/classic_control/mountain_car/envs/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844       37 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/classic_control/mountain_car/envs/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     4679 2022-12-13 15:12:50.000000 DI-engine-0.4.8/dizoo/classic_control/mountain_car/envs/mtcar_env.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1400 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/classic_control/mountain_car/envs/test_mtcar_env.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.895221 DI-engine-0.4.8/dizoo/classic_control/pendulum/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/classic_control/pendulum/__init__.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.904263 DI-engine-0.4.8/dizoo/classic_control/pendulum/config/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844      619 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/classic_control/pendulum/config/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1986 2023-01-04 09:44:45.000000 DI-engine-0.4.8/dizoo/classic_control/pendulum/config/pendulum_bdq_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1866 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/classic_control/pendulum/config/pendulum_cql_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1851 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/classic_control/pendulum/config/pendulum_d4pg_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1763 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/classic_control/pendulum/config/pendulum_ddpg_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1949 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/classic_control/pendulum/config/pendulum_dqn_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1068 2023-03-03 07:55:14.000000 DI-engine-0.4.8/dizoo/classic_control/pendulum/config/pendulum_dt_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1353 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/classic_control/pendulum/config/pendulum_ibc_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1376 2022-11-16 06:44:04.000000 DI-engine-0.4.8/dizoo/classic_control/pendulum/config/pendulum_pg_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1816 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/classic_control/pendulum/config/pendulum_ppo_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1766 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/classic_control/pendulum/config/pendulum_sac_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1347 2022-07-19 08:28:38.000000 DI-engine-0.4.8/dizoo/classic_control/pendulum/config/pendulum_sac_data_generation_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2664 2023-01-06 07:05:23.000000 DI-engine-0.4.8/dizoo/classic_control/pendulum/config/pendulum_sqil_sac_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2234 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/classic_control/pendulum/config/pendulum_td3_bc_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1832 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/classic_control/pendulum/config/pendulum_td3_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2203 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/classic_control/pendulum/config/pendulum_td3_data_generation_config.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.910113 DI-engine-0.4.8/dizoo/classic_control/pendulum/entry/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/classic_control/pendulum/entry/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2177 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/classic_control/pendulum/entry/pendulum_cql_ddpg_main.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2266 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/classic_control/pendulum/entry/pendulum_cql_main.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     3083 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/classic_control/pendulum/entry/pendulum_d4pg_main.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     3576 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/classic_control/pendulum/entry/pendulum_ddpg_main.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2178 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/classic_control/pendulum/entry/pendulum_dqn_eval.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2178 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/classic_control/pendulum/entry/pendulum_ppo_main.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2325 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/classic_control/pendulum/entry/pendulum_td3_bc_main.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     3381 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/classic_control/pendulum/entry/pendulum_td3_main.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.911858 DI-engine-0.4.8/dizoo/classic_control/pendulum/envs/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844       38 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/classic_control/pendulum/envs/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     4943 2022-12-13 15:12:50.000000 DI-engine-0.4.8/dizoo/classic_control/pendulum/envs/pendulum_env.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2226 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/classic_control/pendulum/envs/test_pendulum_env.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.912515 DI-engine-0.4.8/dizoo/common/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/common/__init__.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.915186 DI-engine-0.4.8/dizoo/common/policy/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/common/policy/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     4317 2023-04-05 10:04:48.000000 DI-engine-0.4.8/dizoo/common/policy/md_dqn.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     8472 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/common/policy/md_ppo.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     4183 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/common/policy/md_rainbow_dqn.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.915909 DI-engine-0.4.8/dizoo/competitive_rl/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/competitive_rl/__init__.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.918654 DI-engine-0.4.8/dizoo/competitive_rl/envs/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844       49 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/competitive_rl/envs/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     6561 2022-12-13 15:12:50.000000 DI-engine-0.4.8/dizoo/competitive_rl/envs/competitive_rl_env.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     8597 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/competitive_rl/envs/competitive_rl_env_wrapper.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2554 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/competitive_rl/envs/test_competitive_rl.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.919507 DI-engine-0.4.8/dizoo/d4rl/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/d4rl/__init__.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.951248 DI-engine-0.4.8/dizoo/d4rl/config/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844      175 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/d4rl/config/__init__.py
+-rwxr-xr-x   0 niuyazhe (1370690143) 453037844     1485 2023-04-28 08:23:39.000000 DI-engine-0.4.8/dizoo/d4rl/config/halfcheetah_expert_cql_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2450 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/d4rl/config/halfcheetah_expert_dt_config.py
+-rwxr-xr-x   0 niuyazhe (1370690143) 453037844     1750 2023-05-16 06:06:19.000000 DI-engine-0.4.8/dizoo/d4rl/config/halfcheetah_expert_td3bc_config.py
+-rwxr-xr-x   0 niuyazhe (1370690143) 453037844     1485 2023-04-28 08:23:39.000000 DI-engine-0.4.8/dizoo/d4rl/config/halfcheetah_medium_cql_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2450 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/d4rl/config/halfcheetah_medium_dt_config.py
+-rwxr-xr-x   0 niuyazhe (1370690143) 453037844     1495 2023-04-28 08:23:39.000000 DI-engine-0.4.8/dizoo/d4rl/config/halfcheetah_medium_edac_config.py
+-rwxr-xr-x   0 niuyazhe (1370690143) 453037844     1499 2023-04-28 08:23:39.000000 DI-engine-0.4.8/dizoo/d4rl/config/halfcheetah_medium_expert_cql_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2471 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/d4rl/config/halfcheetah_medium_expert_dt_config.py
+-rwxr-xr-x   0 niuyazhe (1370690143) 453037844     1514 2023-04-28 08:23:39.000000 DI-engine-0.4.8/dizoo/d4rl/config/halfcheetah_medium_expert_edac_config.py
+-rwxr-xr-x   0 niuyazhe (1370690143) 453037844     1765 2023-05-16 06:06:19.000000 DI-engine-0.4.8/dizoo/d4rl/config/halfcheetah_medium_expert_td3bc_config.py
+-rwxr-xr-x   0 niuyazhe (1370690143) 453037844     1499 2023-04-28 08:23:39.000000 DI-engine-0.4.8/dizoo/d4rl/config/halfcheetah_medium_replay_cql_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2471 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/d4rl/config/halfcheetah_medium_replay_dt_config.py
+-rwxr-xr-x   0 niuyazhe (1370690143) 453037844     1764 2023-05-16 06:06:19.000000 DI-engine-0.4.8/dizoo/d4rl/config/halfcheetah_medium_replay_td3bc_config.py
+-rwxr-xr-x   0 niuyazhe (1370690143) 453037844     1750 2023-05-16 06:06:19.000000 DI-engine-0.4.8/dizoo/d4rl/config/halfcheetah_medium_td3bc_config.py
+-rwxr-xr-x   0 niuyazhe (1370690143) 453037844     1485 2023-04-28 08:23:39.000000 DI-engine-0.4.8/dizoo/d4rl/config/halfcheetah_random_cql_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2449 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/d4rl/config/halfcheetah_random_dt_config.py
+-rwxr-xr-x   0 niuyazhe (1370690143) 453037844     1750 2023-05-16 06:06:19.000000 DI-engine-0.4.8/dizoo/d4rl/config/halfcheetah_random_td3bc_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1475 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/d4rl/config/hopper_expert_cql_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2385 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/d4rl/config/hopper_expert_dt_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1621 2023-05-16 06:06:19.000000 DI-engine-0.4.8/dizoo/d4rl/config/hopper_expert_td3bc_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1475 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/d4rl/config/hopper_medium_cql_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2385 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/d4rl/config/hopper_medium_dt_config.py
+-rwxr-xr-x   0 niuyazhe (1370690143) 453037844     1485 2023-04-28 08:23:39.000000 DI-engine-0.4.8/dizoo/d4rl/config/hopper_medium_edac_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1449 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/d4rl/config/hopper_medium_expert_bc_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1489 2022-07-19 08:28:38.000000 DI-engine-0.4.8/dizoo/d4rl/config/hopper_medium_expert_cql_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2406 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/d4rl/config/hopper_medium_expert_dt_config.py
+-rwxr-xr-x   0 niuyazhe (1370690143) 453037844     1500 2023-04-28 08:23:39.000000 DI-engine-0.4.8/dizoo/d4rl/config/hopper_medium_expert_edac_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1458 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/d4rl/config/hopper_medium_expert_ibc_ar_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1342 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/d4rl/config/hopper_medium_expert_ibc_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1348 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/d4rl/config/hopper_medium_expert_ibc_mcmc_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1635 2023-05-16 06:06:19.000000 DI-engine-0.4.8/dizoo/d4rl/config/hopper_medium_expert_td3bc_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1489 2022-07-19 08:28:38.000000 DI-engine-0.4.8/dizoo/d4rl/config/hopper_medium_replay_cql_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2406 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/d4rl/config/hopper_medium_replay_dt_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1635 2023-05-16 06:06:19.000000 DI-engine-0.4.8/dizoo/d4rl/config/hopper_medium_replay_td3bc_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1621 2023-05-16 06:06:19.000000 DI-engine-0.4.8/dizoo/d4rl/config/hopper_medium_td3bc_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1475 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/d4rl/config/hopper_random_cql_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2384 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/d4rl/config/hopper_random_dt_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1740 2023-05-16 06:06:19.000000 DI-engine-0.4.8/dizoo/d4rl/config/hopper_random_td3bc_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1448 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/d4rl/config/kitchen_complete_bc_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1453 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/d4rl/config/kitchen_complete_ibc_ar_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1337 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/d4rl/config/kitchen_complete_ibc_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1343 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/d4rl/config/kitchen_complete_ibc_mcmc_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1431 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/d4rl/config/pen_human_bc_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1501 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/d4rl/config/pen_human_ibc_ar_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1324 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/d4rl/config/pen_human_ibc_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1330 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/d4rl/config/pen_human_ibc_mcmc_config.py
+-rwxr-xr-x   0 niuyazhe (1370690143) 453037844     1479 2023-04-28 08:23:39.000000 DI-engine-0.4.8/dizoo/d4rl/config/walker2d_expert_cql_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2411 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/d4rl/config/walker2d_expert_dt_config.py
+-rwxr-xr-x   0 niuyazhe (1370690143) 453037844     1750 2023-05-16 06:06:19.000000 DI-engine-0.4.8/dizoo/d4rl/config/walker2d_expert_td3bc_config.py
+-rwxr-xr-x   0 niuyazhe (1370690143) 453037844     1479 2023-04-28 08:23:39.000000 DI-engine-0.4.8/dizoo/d4rl/config/walker2d_medium_cql_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2411 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/d4rl/config/walker2d_medium_dt_config.py
+-rwxr-xr-x   0 niuyazhe (1370690143) 453037844     1493 2023-04-28 08:23:39.000000 DI-engine-0.4.8/dizoo/d4rl/config/walker2d_medium_expert_cql_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2432 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/d4rl/config/walker2d_medium_expert_dt_config.py
+-rwxr-xr-x   0 niuyazhe (1370690143) 453037844     1758 2023-05-16 06:06:19.000000 DI-engine-0.4.8/dizoo/d4rl/config/walker2d_medium_expert_td3bc_config.py
+-rwxr-xr-x   0 niuyazhe (1370690143) 453037844     1493 2023-04-28 08:23:39.000000 DI-engine-0.4.8/dizoo/d4rl/config/walker2d_medium_replay_cql_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2432 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/d4rl/config/walker2d_medium_replay_dt_config.py
+-rwxr-xr-x   0 niuyazhe (1370690143) 453037844     1758 2023-05-16 06:06:19.000000 DI-engine-0.4.8/dizoo/d4rl/config/walker2d_medium_replay_td3bc_config.py
+-rwxr-xr-x   0 niuyazhe (1370690143) 453037844     1744 2023-05-16 06:06:19.000000 DI-engine-0.4.8/dizoo/d4rl/config/walker2d_medium_td3bc_config.py
+-rwxr-xr-x   0 niuyazhe (1370690143) 453037844     1479 2023-04-28 08:23:39.000000 DI-engine-0.4.8/dizoo/d4rl/config/walker2d_random_cql_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2410 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/d4rl/config/walker2d_random_dt_config.py
+-rwxr-xr-x   0 niuyazhe (1370690143) 453037844     1744 2023-05-16 06:06:19.000000 DI-engine-0.4.8/dizoo/d4rl/config/walker2d_random_td3bc_config.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.954886 DI-engine-0.4.8/dizoo/d4rl/entry/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/d4rl/entry/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844      685 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/d4rl/entry/d4rl_cql_main.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1407 2022-07-19 08:28:38.000000 DI-engine-0.4.8/dizoo/d4rl/entry/d4rl_dt_main.py
+-rwxr-xr-x   0 niuyazhe (1370690143) 453037844      689 2023-04-28 08:23:39.000000 DI-engine-0.4.8/dizoo/d4rl/entry/d4rl_edac_main.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1171 2023-04-05 10:04:48.000000 DI-engine-0.4.8/dizoo/d4rl/entry/d4rl_ibc_main.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844      694 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/d4rl/entry/d4rl_td3_bc_main.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.956777 DI-engine-0.4.8/dizoo/d4rl/envs/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844       30 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/d4rl/envs/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     3986 2022-12-13 15:12:50.000000 DI-engine-0.4.8/dizoo/d4rl/envs/d4rl_env.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2286 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/d4rl/envs/d4rl_wrappers.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.957353 DI-engine-0.4.8/dizoo/dmc2gym/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2022-07-19 08:28:38.000000 DI-engine-0.4.8/dizoo/dmc2gym/__init__.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.959220 DI-engine-0.4.8/dizoo/dmc2gym/envs/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844       36 2022-07-19 08:28:38.000000 DI-engine-0.4.8/dizoo/dmc2gym/envs/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     8742 2023-03-09 11:08:49.000000 DI-engine-0.4.8/dizoo/dmc2gym/envs/dmc2gym_env.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1645 2023-03-09 11:08:49.000000 DI-engine-0.4.8/dizoo/dmc2gym/envs/test_dmc2gym_env.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.959957 DI-engine-0.4.8/dizoo/evogym/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/evogym/__init__.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.961018 DI-engine-0.4.8/dizoo/evogym/envs/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844       34 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/evogym/envs/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     6926 2022-12-13 15:12:50.000000 DI-engine-0.4.8/dizoo/evogym/envs/evogym_env.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.962051 DI-engine-0.4.8/dizoo/gfootball/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/gfootball/__init__.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.967723 DI-engine-0.4.8/dizoo/gfootball/entry/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/gfootball/entry/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2523 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/gfootball/entry/gfootball_bc_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2542 2022-10-31 06:23:24.000000 DI-engine-0.4.8/dizoo/gfootball/entry/gfootball_bc_kaggle5th_main.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     4374 2022-10-31 06:23:24.000000 DI-engine-0.4.8/dizoo/gfootball/entry/gfootball_bc_rule_lt0_main.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     4010 2022-10-31 06:23:24.000000 DI-engine-0.4.8/dizoo/gfootball/entry/gfootball_bc_rule_main.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1896 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/gfootball/entry/gfootball_dqn_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2197 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/gfootball/entry/show_dataset.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1884 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/gfootball/entry/test_accuracy.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.971506 DI-engine-0.4.8/dizoo/gfootball/envs/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844      174 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/gfootball/envs/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2648 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/gfootball/envs/fake_dataset.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    14135 2022-12-13 15:12:50.000000 DI-engine-0.4.8/dizoo/gfootball/envs/gfootball_academy_env.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     8689 2022-12-13 15:12:50.000000 DI-engine-0.4.8/dizoo/gfootball/envs/gfootball_env.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     7430 2022-12-13 15:12:50.000000 DI-engine-0.4.8/dizoo/gfootball/envs/gfootballsp_env.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.972268 DI-engine-0.4.8/dizoo/gfootball/model/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/gfootball/model/__init__.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.974019 DI-engine-0.4.8/dizoo/gfootball/model/bots/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844      120 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/gfootball/model/bots/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1780 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/gfootball/model/bots/kaggle_5th_place_model.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    26957 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/gfootball/model/bots/rule_based_bot_model.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.975327 DI-engine-0.4.8/dizoo/gfootball/policy/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844       55 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/gfootball/policy/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    15162 2023-04-05 10:04:48.000000 DI-engine-0.4.8/dizoo/gfootball/policy/ppo_lstm.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1268 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/gfootball/replay.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.976212 DI-engine-0.4.8/dizoo/gym_anytrading/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/gym_anytrading/__init__.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.977071 DI-engine-0.4.8/dizoo/gym_anytrading/config/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844       76 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/gym_anytrading/config/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2952 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/gym_anytrading/config/stocks_dqn_config.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.980149 DI-engine-0.4.8/dizoo/gym_anytrading/envs/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844       90 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/gym_anytrading/envs/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     6412 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/gym_anytrading/envs/stocks_env.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1506 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/gym_anytrading/envs/test_stocks_env.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    10840 2022-12-13 15:12:50.000000 DI-engine-0.4.8/dizoo/gym_anytrading/envs/trading_env.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.981169 DI-engine-0.4.8/dizoo/gym_anytrading/worker/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844       51 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/gym_anytrading/worker/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     9730 2022-12-13 15:12:50.000000 DI-engine-0.4.8/dizoo/gym_anytrading/worker/trading_serial_evaluator.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.981621 DI-engine-0.4.8/dizoo/gym_hybrid/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/gym_hybrid/__init__.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.983436 DI-engine-0.4.8/dizoo/gym_hybrid/config/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2022-12-22 08:45:23.000000 DI-engine-0.4.8/dizoo/gym_hybrid/config/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2196 2023-01-02 10:31:34.000000 DI-engine-0.4.8/dizoo/gym_hybrid/config/gym_hybrid_ddpg_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1985 2023-01-02 10:31:34.000000 DI-engine-0.4.8/dizoo/gym_hybrid/config/gym_hybrid_hppo_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2453 2023-04-05 10:04:48.000000 DI-engine-0.4.8/dizoo/gym_hybrid/config/gym_hybrid_mpdqn_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2381 2023-05-25 03:46:54.000000 DI-engine-0.4.8/dizoo/gym_hybrid/config/gym_hybrid_pdqn_config.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.985992 DI-engine-0.4.8/dizoo/gym_hybrid/entry/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/gym_hybrid/entry/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2316 2022-12-26 09:01:35.000000 DI-engine-0.4.8/dizoo/gym_hybrid/entry/e.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2196 2023-01-02 10:31:34.000000 DI-engine-0.4.8/dizoo/gym_hybrid/entry/gym_hybrid_ddpg_eval.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     3996 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/gym_hybrid/entry/gym_hybrid_ddpg_main.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.989295 DI-engine-0.4.8/dizoo/gym_hybrid/envs/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844       41 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/gym_hybrid/envs/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     5947 2023-05-22 11:42:05.000000 DI-engine-0.4.8/dizoo/gym_hybrid/envs/gym_hybrid_env.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1149 2022-11-14 04:31:11.000000 DI-engine-0.4.8/dizoo/gym_hybrid/envs/test_gym_hybrid_env.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.989927 DI-engine-0.4.8/dizoo/gym_pybullet_drones/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2022-11-14 04:31:11.000000 DI-engine-0.4.8/dizoo/gym_pybullet_drones/__init__.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.992053 DI-engine-0.4.8/dizoo/gym_pybullet_drones/envs/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844       58 2023-01-04 09:44:45.000000 DI-engine-0.4.8/dizoo/gym_pybullet_drones/envs/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     9559 2023-03-10 09:15:22.000000 DI-engine-0.4.8/dizoo/gym_pybullet_drones/envs/gym_pybullet_drones_env.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1034 2022-11-14 04:31:11.000000 DI-engine-0.4.8/dizoo/gym_pybullet_drones/envs/test_ding_env.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844      830 2022-11-14 04:31:11.000000 DI-engine-0.4.8/dizoo/gym_pybullet_drones/envs/test_ori_env.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.992639 DI-engine-0.4.8/dizoo/gym_soccer/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/gym_soccer/__init__.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.993454 DI-engine-0.4.8/dizoo/gym_soccer/envs/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/gym_soccer/envs/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     6247 2022-12-13 15:12:50.000000 DI-engine-0.4.8/dizoo/gym_soccer/envs/gym_soccer_env.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1248 2022-12-13 15:12:50.000000 DI-engine-0.4.8/dizoo/gym_soccer/envs/test_gym_soccer_env.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.994280 DI-engine-0.4.8/dizoo/image_classification/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/image_classification/__init__.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.995864 DI-engine-0.4.8/dizoo/image_classification/data/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844       77 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/image_classification/data/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     4660 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/image_classification/data/dataset.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2207 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/image_classification/data/sampler.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:57.997181 DI-engine-0.4.8/dizoo/image_classification/policy/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844       46 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/image_classification/policy/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2955 2023-04-05 10:04:48.000000 DI-engine-0.4.8/dizoo/image_classification/policy/policy.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:58.001431 DI-engine-0.4.8/dizoo/league_demo/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/league_demo/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1805 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/league_demo/demo_league.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     3024 2022-12-13 15:12:50.000000 DI-engine-0.4.8/dizoo/league_demo/game_env.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    16428 2022-12-13 15:12:50.000000 DI-engine-0.4.8/dizoo/league_demo/league_demo_collector.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2768 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/league_demo/league_demo_ppo_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    10209 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/league_demo/league_demo_ppo_main.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1199 2022-07-19 08:28:38.000000 DI-engine-0.4.8/dizoo/league_demo/selfplay_demo_ppo_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     4662 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/league_demo/selfplay_demo_ppo_main.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:58.003738 DI-engine-0.4.8/dizoo/mario/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2023-01-17 12:08:18.000000 DI-engine-0.4.8/dizoo/mario/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1354 2023-01-17 12:08:18.000000 DI-engine-0.4.8/dizoo/mario/mario_dqn_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2787 2023-02-13 06:54:46.000000 DI-engine-0.4.8/dizoo/mario/mario_dqn_example.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     4454 2023-01-17 12:08:18.000000 DI-engine-0.4.8/dizoo/mario/mario_dqn_main.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:58.004507 DI-engine-0.4.8/dizoo/maze/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844      100 2023-03-09 11:08:49.000000 DI-engine-0.4.8/dizoo/maze/__init__.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:58.006889 DI-engine-0.4.8/dizoo/maze/envs/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844       27 2023-03-09 11:08:49.000000 DI-engine-0.4.8/dizoo/maze/envs/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    13099 2023-03-10 04:24:02.000000 DI-engine-0.4.8/dizoo/maze/envs/maze_env.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844      793 2023-03-09 11:08:49.000000 DI-engine-0.4.8/dizoo/maze/envs/test_maze_env.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:58.007504 DI-engine-0.4.8/dizoo/metadrive/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2023-02-15 07:39:03.000000 DI-engine-0.4.8/dizoo/metadrive/__init__.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:58.009168 DI-engine-0.4.8/dizoo/metadrive/config/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2023-02-15 07:39:03.000000 DI-engine-0.4.8/dizoo/metadrive/config/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     4258 2023-02-23 09:38:44.000000 DI-engine-0.4.8/dizoo/metadrive/config/metadrive_onppo_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     3693 2023-02-15 07:39:03.000000 DI-engine-0.4.8/dizoo/metadrive/config/metadrive_onppo_eval_config.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:58.011935 DI-engine-0.4.8/dizoo/metadrive/env/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2023-02-15 07:39:03.000000 DI-engine-0.4.8/dizoo/metadrive/env/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    15662 2023-03-10 09:15:22.000000 DI-engine-0.4.8/dizoo/metadrive/env/drive_env.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     4010 2023-04-05 10:04:48.000000 DI-engine-0.4.8/dizoo/metadrive/env/drive_utils.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     5709 2023-04-05 10:04:48.000000 DI-engine-0.4.8/dizoo/metadrive/env/drive_wrapper.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:58.012760 DI-engine-0.4.8/dizoo/minigrid/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844      750 2023-03-09 11:08:49.000000 DI-engine-0.4.8/dizoo/minigrid/__init__.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:58.016458 DI-engine-0.4.8/dizoo/minigrid/envs/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844      323 2023-03-09 11:08:49.000000 DI-engine-0.4.8/dizoo/minigrid/envs/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     7470 2023-03-09 11:08:49.000000 DI-engine-0.4.8/dizoo/minigrid/envs/app_key_to_door_treasure.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     6933 2023-03-10 09:15:22.000000 DI-engine-0.4.8/dizoo/minigrid/envs/minigrid_env.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1163 2023-03-09 11:08:49.000000 DI-engine-0.4.8/dizoo/minigrid/envs/minigrid_wrapper.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     7249 2023-03-09 11:08:49.000000 DI-engine-0.4.8/dizoo/minigrid/envs/noisy_tv.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     3769 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/minigrid/envs/test_minigrid_env.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:58.017004 DI-engine-0.4.8/dizoo/mujoco/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/mujoco/__init__.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:58.043610 DI-engine-0.4.8/dizoo/mujoco/config/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/mujoco/config/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2105 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/mujoco/config/ant_ddpg_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     3352 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/mujoco/config/ant_gail_sac_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2154 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/mujoco/config/ant_onppo_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1705 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/mujoco/config/ant_ppo_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1976 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/mujoco/config/ant_sac_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2009 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/mujoco/config/ant_td3_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2544 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/mujoco/config/ant_trex_onppo_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2829 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/mujoco/config/ant_trex_sac_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2954 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/mujoco/config/halfcheetah_bco_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2057 2023-01-04 09:44:45.000000 DI-engine-0.4.8/dizoo/mujoco/config/halfcheetah_bdq_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2074 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/mujoco/config/halfcheetah_d4pg_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1915 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/mujoco/config/halfcheetah_ddpg_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     3430 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/mujoco/config/halfcheetah_gail_sac_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2814 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/mujoco/config/halfcheetah_gcl_sac_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2335 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/mujoco/config/halfcheetah_onppo_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1991 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/mujoco/config/halfcheetah_sac_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2750 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/mujoco/config/halfcheetah_sqil_sac_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2039 2022-11-14 04:31:11.000000 DI-engine-0.4.8/dizoo/mujoco/config/halfcheetah_td3_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     4130 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/mujoco/config/halfcheetah_trex_onppo_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     3966 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/mujoco/config/halfcheetah_trex_sac_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2847 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/mujoco/config/hopper_bco_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2246 2023-01-04 09:44:45.000000 DI-engine-0.4.8/dizoo/mujoco/config/hopper_bdq_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2093 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/mujoco/config/hopper_cql_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1966 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/mujoco/config/hopper_d4pg_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1857 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/mujoco/config/hopper_ddpg_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     3397 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/mujoco/config/hopper_gail_sac_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2372 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/mujoco/config/hopper_gcl_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2131 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/mujoco/config/hopper_onppo_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1936 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/mujoco/config/hopper_sac_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2610 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/mujoco/config/hopper_sac_data_generation_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2601 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/mujoco/config/hopper_sqil_sac_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2455 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/mujoco/config/hopper_td3_bc_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1969 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/mujoco/config/hopper_td3_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2668 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/mujoco/config/hopper_td3_data_generation_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     3635 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/mujoco/config/hopper_trex_onppo_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     3870 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/mujoco/config/hopper_trex_sac_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2000 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/mujoco/config/walker2d_d4pg_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1879 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/mujoco/config/walker2d_ddpg_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     3579 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/mujoco/config/walker2d_gail_ddpg_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     3425 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/mujoco/config/walker2d_gail_sac_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2432 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/mujoco/config/walker2d_gcl_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2346 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/mujoco/config/walker2d_onppo_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1958 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/mujoco/config/walker2d_sac_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2567 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/mujoco/config/walker2d_sqil_sac_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1991 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/mujoco/config/walker2d_td3_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     3659 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/mujoco/config/walker2d_trex_onppo_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     3894 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/mujoco/config/walker2d_trex_sac_config.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:58.047762 DI-engine-0.4.8/dizoo/mujoco/entry/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/mujoco/entry/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844      983 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/mujoco/entry/mujoco_cql_generation_main.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844      436 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/mujoco/entry/mujoco_cql_main.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2861 2022-11-14 04:31:11.000000 DI-engine-0.4.8/dizoo/mujoco/entry/mujoco_d4pg_main.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1937 2022-11-14 04:31:11.000000 DI-engine-0.4.8/dizoo/mujoco/entry/mujoco_ddpg_eval.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2697 2022-11-14 04:31:11.000000 DI-engine-0.4.8/dizoo/mujoco/entry/mujoco_ddpg_main.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2338 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/mujoco/entry/mujoco_ppo_main.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2290 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/mujoco/entry/mujoco_td3_bc_main.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:58.049955 DI-engine-0.4.8/dizoo/mujoco/envs/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844       77 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/mujoco/envs/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     6144 2022-12-13 15:12:50.000000 DI-engine-0.4.8/dizoo/mujoco/envs/mujoco_disc_env.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     8606 2023-01-04 09:44:45.000000 DI-engine-0.4.8/dizoo/mujoco/envs/mujoco_env.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1992 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/mujoco/envs/mujoco_gym_env.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1415 2022-12-13 15:12:50.000000 DI-engine-0.4.8/dizoo/mujoco/envs/mujoco_wrappers.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:58.050527 DI-engine-0.4.8/dizoo/multiagent_mujoco/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/multiagent_mujoco/__init__.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:58.055828 DI-engine-0.4.8/dizoo/multiagent_mujoco/envs/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844      185 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/multiagent_mujoco/envs/__init__.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:58.059840 DI-engine-0.4.8/dizoo/multiagent_mujoco/envs/assets/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/multiagent_mujoco/envs/assets/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     8773 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/multiagent_mujoco/envs/assets/coupled_half_cheetah.xml
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     8333 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/multiagent_mujoco/envs/assets/manyagent_ant.xml
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     5215 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/multiagent_mujoco/envs/assets/manyagent_ant__stage1.xml
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2900 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/multiagent_mujoco/envs/assets/manyagent_swimmer__bckp2.xml
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2570 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/multiagent_mujoco/envs/assets/manyagent_swimmer_bckp.xml
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1852 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/multiagent_mujoco/envs/coupled_half_cheetah.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     5661 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/multiagent_mujoco/envs/manyagent_ant.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     3593 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/multiagent_mujoco/envs/manyagent_swimmer.py
+-rwxr-xr-x   0 niuyazhe (1370690143) 453037844     9649 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/multiagent_mujoco/envs/mujoco_multi.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     4066 2022-12-13 15:12:50.000000 DI-engine-0.4.8/dizoo/multiagent_mujoco/envs/multi_mujoco_env.py
+-rwxr-xr-x   0 niuyazhe (1370690143) 453037844     2404 2022-03-14 08:09:40.000000 DI-engine-0.4.8/dizoo/multiagent_mujoco/envs/multiagentenv.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    23700 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/multiagent_mujoco/envs/obsk.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:58.060348 DI-engine-0.4.8/dizoo/overcooked/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/overcooked/__init__.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:58.061210 DI-engine-0.4.8/dizoo/overcooked/config/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844       68 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/overcooked/config/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2357 2022-07-19 08:28:38.000000 DI-engine-0.4.8/dizoo/overcooked/config/overcooked_ppo_config.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:58.063261 DI-engine-0.4.8/dizoo/overcooked/envs/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844       58 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/overcooked/envs/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    12316 2022-12-13 15:12:50.000000 DI-engine-0.4.8/dizoo/overcooked/envs/overcooked_env.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1726 2022-12-13 15:12:50.000000 DI-engine-0.4.8/dizoo/overcooked/envs/test_overcooked_env.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:58.064108 DI-engine-0.4.8/dizoo/petting_zoo/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2022-07-19 08:28:38.000000 DI-engine-0.4.8/dizoo/petting_zoo/__init__.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:58.070983 DI-engine-0.4.8/dizoo/petting_zoo/config/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1022 2022-12-11 15:35:39.000000 DI-engine-0.4.8/dizoo/petting_zoo/config/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2391 2023-03-01 15:44:29.000000 DI-engine-0.4.8/dizoo/petting_zoo/config/ptz_simple_spread_atoc_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2456 2023-03-01 15:44:29.000000 DI-engine-0.4.8/dizoo/petting_zoo/config/ptz_simple_spread_collaq_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2512 2023-03-01 15:44:29.000000 DI-engine-0.4.8/dizoo/petting_zoo/config/ptz_simple_spread_coma_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2581 2023-03-01 15:44:29.000000 DI-engine-0.4.8/dizoo/petting_zoo/config/ptz_simple_spread_madqn_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2960 2023-03-01 15:44:29.000000 DI-engine-0.4.8/dizoo/petting_zoo/config/ptz_simple_spread_mappo_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2544 2023-05-16 06:06:19.000000 DI-engine-0.4.8/dizoo/petting_zoo/config/ptz_simple_spread_masac_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2082 2023-03-01 15:44:29.000000 DI-engine-0.4.8/dizoo/petting_zoo/config/ptz_simple_spread_qmix_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2490 2023-03-01 15:44:29.000000 DI-engine-0.4.8/dizoo/petting_zoo/config/ptz_simple_spread_qtran_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2196 2023-03-01 15:44:29.000000 DI-engine-0.4.8/dizoo/petting_zoo/config/ptz_simple_spread_vdn_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     2394 2023-03-01 15:44:29.000000 DI-engine-0.4.8/dizoo/petting_zoo/config/ptz_simple_spread_wqmix_config.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:58.073034 DI-engine-0.4.8/dizoo/petting_zoo/envs/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2022-07-19 08:28:38.000000 DI-engine-0.4.8/dizoo/petting_zoo/envs/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    16796 2023-05-16 06:06:19.000000 DI-engine-0.4.8/dizoo/petting_zoo/envs/petting_zoo_simple_spread_env.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     5552 2023-05-16 06:06:19.000000 DI-engine-0.4.8/dizoo/petting_zoo/envs/test_petting_zoo_simple_spread_env.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:58.073592 DI-engine-0.4.8/dizoo/pomdp/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/pomdp/__init__.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:58.075760 DI-engine-0.4.8/dizoo/pomdp/envs/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844       37 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/pomdp/envs/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     4022 2022-12-13 15:12:50.000000 DI-engine-0.4.8/dizoo/pomdp/envs/atari_env.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     6746 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/pomdp/envs/atari_wrappers.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1031 2022-12-13 15:12:50.000000 DI-engine-0.4.8/dizoo/pomdp/envs/test_atari_env.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:58.076145 DI-engine-0.4.8/dizoo/procgen/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2023-01-17 12:06:29.000000 DI-engine-0.4.8/dizoo/procgen/__init__.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:58.080138 DI-engine-0.4.8/dizoo/procgen/config/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844      118 2022-12-11 15:35:39.000000 DI-engine-0.4.8/dizoo/procgen/config/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1719 2022-12-11 15:35:39.000000 DI-engine-0.4.8/dizoo/procgen/config/bigfish_plr_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1617 2022-12-11 15:35:39.000000 DI-engine-0.4.8/dizoo/procgen/config/bigfish_ppg_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1362 2022-12-11 15:35:39.000000 DI-engine-0.4.8/dizoo/procgen/config/coinrun_dqn_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1616 2022-12-11 15:35:39.000000 DI-engine-0.4.8/dizoo/procgen/config/coinrun_ppg_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1449 2022-12-11 15:35:39.000000 DI-engine-0.4.8/dizoo/procgen/config/coinrun_ppo_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1369 2022-12-11 15:35:39.000000 DI-engine-0.4.8/dizoo/procgen/config/maze_dqn_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1641 2022-12-11 15:35:39.000000 DI-engine-0.4.8/dizoo/procgen/config/maze_ppg_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1447 2022-12-11 15:35:39.000000 DI-engine-0.4.8/dizoo/procgen/config/maze_ppo_config.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:58.081709 DI-engine-0.4.8/dizoo/procgen/envs/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844       36 2022-07-19 08:28:38.000000 DI-engine-0.4.8/dizoo/procgen/envs/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     4485 2022-12-13 15:12:50.000000 DI-engine-0.4.8/dizoo/procgen/envs/procgen_env.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844      810 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/procgen/envs/test_coinrun_env.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:58.082305 DI-engine-0.4.8/dizoo/pybullet/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/pybullet/__init__.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:58.083870 DI-engine-0.4.8/dizoo/pybullet/envs/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844       38 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/pybullet/envs/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    11254 2022-12-13 15:12:50.000000 DI-engine-0.4.8/dizoo/pybullet/envs/pybullet_env.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1663 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/pybullet/envs/pybullet_wrappers.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:58.084477 DI-engine-0.4.8/dizoo/rocket/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2023-01-17 12:05:32.000000 DI-engine-0.4.8/dizoo/rocket/__init__.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:58.085716 DI-engine-0.4.8/dizoo/rocket/config/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2023-01-17 12:05:45.000000 DI-engine-0.4.8/dizoo/rocket/config/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1818 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/rocket/config/rocket_hover_ppo_config.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1828 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/rocket/config/rocket_landing_ppo_config.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:58.088666 DI-engine-0.4.8/dizoo/rocket/entry/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2023-01-17 12:05:50.000000 DI-engine-0.4.8/dizoo/rocket/entry/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     4039 2023-02-13 06:56:29.000000 DI-engine-0.4.8/dizoo/rocket/entry/rocket_hover_onppo_main_v2.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     3261 2023-02-13 06:57:07.000000 DI-engine-0.4.8/dizoo/rocket/entry/rocket_hover_ppo_main.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     4022 2023-02-13 06:57:32.000000 DI-engine-0.4.8/dizoo/rocket/entry/rocket_landing_onppo_main_v2.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     3236 2023-02-13 06:56:46.000000 DI-engine-0.4.8/dizoo/rocket/entry/rocket_landing_ppo_main.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:58.090717 DI-engine-0.4.8/dizoo/rocket/envs/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844       34 2023-01-04 09:44:45.000000 DI-engine-0.4.8/dizoo/rocket/envs/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     4024 2023-03-10 09:15:22.000000 DI-engine-0.4.8/dizoo/rocket/envs/rocket_env.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1391 2023-01-04 09:44:45.000000 DI-engine-0.4.8/dizoo/rocket/envs/test_rocket_env.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:58.091381 DI-engine-0.4.8/dizoo/slime_volley/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/slime_volley/__init__.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:58.091604 DI-engine-0.4.8/dizoo/slime_volley/config/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1685 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/slime_volley/config/slime_volley_ppo_config.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:58.093549 DI-engine-0.4.8/dizoo/slime_volley/envs/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844       46 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/slime_volley/envs/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     7877 2022-12-13 15:12:50.000000 DI-engine-0.4.8/dizoo/slime_volley/envs/slime_volley_env.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1274 2022-12-13 15:12:50.000000 DI-engine-0.4.8/dizoo/slime_volley/envs/test_slime_volley_env.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:58.094269 DI-engine-0.4.8/dizoo/smac/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/smac/__init__.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:58.098958 DI-engine-0.4.8/dizoo/smac/envs/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844      194 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/smac/envs/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1666 2022-12-13 15:12:50.000000 DI-engine-0.4.8/dizoo/smac/envs/fake_smac_env.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:58.099377 DI-engine-0.4.8/dizoo/smac/envs/maps/
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:58.116727 DI-engine-0.4.8/dizoo/smac/envs/maps/SMAC_Maps/
+-rwxr-xr-x   0 niuyazhe (1370690143) 453037844    14925 2021-08-01 05:19:48.000000 DI-engine-0.4.8/dizoo/smac/envs/maps/SMAC_Maps/10m_vs_11m.SC2Map
+-rwxr-xr-x   0 niuyazhe (1370690143) 453037844    16965 2021-08-01 05:19:48.000000 DI-engine-0.4.8/dizoo/smac/envs/maps/SMAC_Maps/1c3s5z.SC2Map
+-rwxr-xr-x   0 niuyazhe (1370690143) 453037844    14923 2021-08-01 05:19:48.000000 DI-engine-0.4.8/dizoo/smac/envs/maps/SMAC_Maps/25m.SC2Map
+-rwxr-xr-x   0 niuyazhe (1370690143) 453037844    14929 2021-08-01 05:19:48.000000 DI-engine-0.4.8/dizoo/smac/envs/maps/SMAC_Maps/27m_vs_30m.SC2Map
+-rwxr-xr-x   0 niuyazhe (1370690143) 453037844    16477 2021-08-01 05:19:48.000000 DI-engine-0.4.8/dizoo/smac/envs/maps/SMAC_Maps/2c_vs_64zg.SC2Map
+-rwxr-xr-x   0 niuyazhe (1370690143) 453037844    15539 2021-08-01 05:19:48.000000 DI-engine-0.4.8/dizoo/smac/envs/maps/SMAC_Maps/2m_vs_1z.SC2Map
+-rwxr-xr-x   0 niuyazhe (1370690143) 453037844    15692 2021-08-01 05:19:48.000000 DI-engine-0.4.8/dizoo/smac/envs/maps/SMAC_Maps/2s3z.SC2Map
+-rwxr-xr-x   0 niuyazhe (1370690143) 453037844    14202 2021-08-01 05:19:48.000000 DI-engine-0.4.8/dizoo/smac/envs/maps/SMAC_Maps/2s_vs_1sc.SC2Map
+-rwxr-xr-x   0 niuyazhe (1370690143) 453037844    14920 2021-08-01 05:19:48.000000 DI-engine-0.4.8/dizoo/smac/envs/maps/SMAC_Maps/3m.SC2Map
+-rwxr-xr-x   0 niuyazhe (1370690143) 453037844    15697 2021-08-01 05:19:48.000000 DI-engine-0.4.8/dizoo/smac/envs/maps/SMAC_Maps/3s5z.SC2Map
+-rwxr-xr-x   0 niuyazhe (1370690143) 453037844    15704 2021-08-01 05:19:48.000000 DI-engine-0.4.8/dizoo/smac/envs/maps/SMAC_Maps/3s5z_vs_3s6z.SC2Map
+-rwxr-xr-x   0 niuyazhe (1370690143) 453037844    13995 2021-08-01 05:19:48.000000 DI-engine-0.4.8/dizoo/smac/envs/maps/SMAC_Maps/3s_vs_3z.SC2Map
+-rwxr-xr-x   0 niuyazhe (1370690143) 453037844    14000 2021-08-01 05:19:48.000000 DI-engine-0.4.8/dizoo/smac/envs/maps/SMAC_Maps/3s_vs_4z.SC2Map
+-rwxr-xr-x   0 niuyazhe (1370690143) 453037844    13998 2021-08-01 05:19:48.000000 DI-engine-0.4.8/dizoo/smac/envs/maps/SMAC_Maps/3s_vs_5z.SC2Map
+-rwxr-xr-x   0 niuyazhe (1370690143) 453037844    14930 2021-08-01 05:19:48.000000 DI-engine-0.4.8/dizoo/smac/envs/maps/SMAC_Maps/5m_vs_6m.SC2Map
+-rwxr-xr-x   0 niuyazhe (1370690143) 453037844    14342 2021-08-01 05:19:48.000000 DI-engine-0.4.8/dizoo/smac/envs/maps/SMAC_Maps/6h_vs_8z.SC2Map
+-rwxr-xr-x   0 niuyazhe (1370690143) 453037844    14922 2021-08-01 05:19:48.000000 DI-engine-0.4.8/dizoo/smac/envs/maps/SMAC_Maps/8m.SC2Map
+-rwxr-xr-x   0 niuyazhe (1370690143) 453037844    14927 2021-08-01 05:19:48.000000 DI-engine-0.4.8/dizoo/smac/envs/maps/SMAC_Maps/8m_vs_9m.SC2Map
+-rwxr-xr-x   0 niuyazhe (1370690143) 453037844    17411 2021-08-01 05:19:48.000000 DI-engine-0.4.8/dizoo/smac/envs/maps/SMAC_Maps/MMM.SC2Map
+-rwxr-xr-x   0 niuyazhe (1370690143) 453037844    17419 2021-08-01 05:19:48.000000 DI-engine-0.4.8/dizoo/smac/envs/maps/SMAC_Maps/MMM2.SC2Map
+-rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/smac/envs/maps/SMAC_Maps/__init__.py
+-rwxr-xr-x   0 niuyazhe (1370690143) 453037844    16782 2021-08-01 05:19:48.000000 DI-engine-0.4.8/dizoo/smac/envs/maps/SMAC_Maps/bane_vs_bane.SC2Map
+-rwxr-xr-x   0 niuyazhe (1370690143) 453037844    18055 2021-08-01 05:19:48.000000 DI-engine-0.4.8/dizoo/smac/envs/maps/SMAC_Maps/corridor.SC2Map
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    17080 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/smac/envs/maps/SMAC_Maps/infestor_viper.SC2Map
+-rwxr-xr-x   0 niuyazhe (1370690143) 453037844    18133 2021-08-01 05:19:48.000000 DI-engine-0.4.8/dizoo/smac/envs/maps/SMAC_Maps/so_many_baneling.SC2Map
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:58.118663 DI-engine-0.4.8/dizoo/smac/envs/maps/SMAC_Maps_two_player/
+-rwxr-xr-x   0 niuyazhe (1370690143) 453037844    14835 2021-08-01 05:19:48.000000 DI-engine-0.4.8/dizoo/smac/envs/maps/SMAC_Maps_two_player/3m.SC2Map
+-rwxr-xr-x   0 niuyazhe (1370690143) 453037844    15596 2021-08-01 05:19:48.000000 DI-engine-0.4.8/dizoo/smac/envs/maps/SMAC_Maps_two_player/3s5z.SC2Map
+-rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/smac/envs/maps/SMAC_Maps_two_player/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/smac/envs/maps/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    16272 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/smac/envs/smac_action.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844    70855 2022-12-13 15:12:50.000000 DI-engine-0.4.8/dizoo/smac/envs/smac_env.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     5383 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/smac/envs/smac_map.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     9098 2022-09-30 04:52:25.000000 DI-engine-0.4.8/dizoo/smac/envs/smac_reward.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     6050 2022-12-13 15:12:50.000000 DI-engine-0.4.8/dizoo/smac/envs/test_smac_env.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:58.119039 DI-engine-0.4.8/dizoo/sokoban/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844        0 2023-01-17 12:06:19.000000 DI-engine-0.4.8/dizoo/sokoban/__init__.py
+drwxr-xr-x   0 niuyazhe (1370690143) 453037844        0 2023-05-25 06:04:58.121357 DI-engine-0.4.8/dizoo/sokoban/envs/
+-rw-r--r--   0 niuyazhe (1370690143) 453037844       36 2022-10-19 09:16:29.000000 DI-engine-0.4.8/dizoo/sokoban/envs/__init__.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     4021 2022-12-13 15:12:50.000000 DI-engine-0.4.8/dizoo/sokoban/envs/sokoban_env.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     1658 2022-08-02 16:56:36.000000 DI-engine-0.4.8/dizoo/sokoban/envs/sokoban_wrappers.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844      779 2022-08-02 16:56:36.000000 DI-engine-0.4.8/dizoo/sokoban/envs/test_sokoban_env.py
+-rw-r--r--   0 niuyazhe (1370690143) 453037844       38 2023-05-25 06:04:58.122790 DI-engine-0.4.8/setup.cfg
+-rw-r--r--   0 niuyazhe (1370690143) 453037844     6010 2023-05-16 06:07:58.000000 DI-engine-0.4.8/setup.py
```

### Comparing `DI-engine-0.4.7/DI_engine.egg-info/PKG-INFO` & `DI-engine-0.4.8/DI_engine.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DI-engine
-Version: 0.4.7
+Version: 0.4.8
 Summary: Decision AI Engine
 Home-page: https://github.com/opendilab/DI-engine
 Author: OpenDILab Contributors
 Author-email: opendilab@pjlab.org.cn
 License: Apache License, Version 2.0
 Keywords: Decision AI Engine
 Classifier: Development Status :: 5 - Production/Stable
@@ -66,15 +66,15 @@
 [![GitHub forks](https://img.shields.io/github/forks/opendilab/DI-engine)](https://github.com/opendilab/DI-engine/network)
 ![GitHub commit activity](https://img.shields.io/github/commit-activity/m/opendilab/DI-engine)
 [![GitHub issues](https://img.shields.io/github/issues/opendilab/DI-engine)](https://github.com/opendilab/DI-engine/issues)
 [![GitHub pulls](https://img.shields.io/github/issues-pr/opendilab/DI-engine)](https://github.com/opendilab/DI-engine/pulls)
 [![Contributors](https://img.shields.io/github/contributors/opendilab/DI-engine)](https://github.com/opendilab/DI-engine/graphs/contributors)
 [![GitHub license](https://img.shields.io/github/license/opendilab/DI-engine)](https://github.com/opendilab/DI-engine/blob/master/LICENSE)
 
-Updated on 2023.04.11 DI-engine-v0.4.7
+Updated on 2023.05.25 DI-engine-v0.4.8
 
 
 ## Introduction to DI-engine
 [Documentation](https://di-engine-docs.readthedocs.io/en/latest/) | [中文文档](https://di-engine-docs.readthedocs.io/zh_CN/latest/) | [Tutorials](https://di-engine-docs.readthedocs.io/en/latest/01_quickstart/index.html) | [Feature](#feature) | [Task & Middleware](https://di-engine-docs.readthedocs.io/en/latest/03_system/index.html) | [TreeTensor](#general-data-container-treetensor) | [Roadmap](https://github.com/opendilab/DI-engine/issues/548)
 
 **DI-engine** is a generalized decision intelligence engine for PyTorch and JAX. 
 
@@ -286,14 +286,15 @@
 |  46  |         [MBPO](https://arxiv.org/pdf/1906.08253.pdf)         | ![mbrl](https://img.shields.io/badge/-ModelBasedRL-lightblue) | [MBPO doc](https://di-engine-docs.readthedocs.io/en/latest/12_policies/mbpo.html)<br>[world_model/mbpo](https://github.com/opendilab/DI-engine/blob/main/ding/world_model/mbpo.py) |        python3 -u pendulum_sac_mbpo_config.py    |
 |  47  |         [DDPPO](https://openreview.net/forum?id=rzvOQrnclO0)         | ![mbrl](https://img.shields.io/badge/-ModelBasedRL-lightblue) | [world_model/ddppo](https://github.com/opendilab/DI-engine/blob/main/ding/world_model/ddppo.py) |        python3 -u pendulum_mbsac_ddppo_config.py    |
 |  48  |         [PER](https://arxiv.org/pdf/1511.05952.pdf)          |   ![other](https://img.shields.io/badge/-other-lightgrey)    | [worker/replay_buffer](https://github.com/opendilab/DI-engine/blob/main/ding/worker/replay_buffer/advanced_buffer.py) |                        `rainbow demo`                        |
 |  49  |         [GAE](https://arxiv.org/pdf/1506.02438.pdf)          |   ![other](https://img.shields.io/badge/-other-lightgrey)    | [rl_utils/gae](https://github.com/opendilab/DI-engine/blob/main/ding/rl_utils/gae.py) |                          `ppo demo`                          |
 |  50  |         [ST-DIM](https://arxiv.org/pdf/1906.08226.pdf)          |   ![other](https://img.shields.io/badge/-other-lightgrey)    | [torch_utils/loss/contrastive_loss](https://github.com/opendilab/DI-engine/blob/main/ding/torch_utils/loss/contrastive_loss.py) |        ding -m serial -c cartpole_dqn_stdim_config.py -s 0       |
 |  51  |         [PLR](https://arxiv.org/pdf/2010.03934.pdf)          |   ![other](https://img.shields.io/badge/-other-lightgrey)    | [PLR doc](https://di-engine-docs.readthedocs.io/en/latest/12_policies/plr.html)<br>[data/level_replay/level_sampler](https://github.com/opendilab/DI-engine/blob/main/ding/data/level_replay/level_sampler.py) |        python3 -u bigfish_plr_config.py -s 0       |
 |  52  |         [PCGrad](https://arxiv.org/pdf/2001.06782.pdf)          |   ![other](https://img.shields.io/badge/-other-lightgrey)    | [torch_utils/optimizer_helper/PCGrad](https://github.com/opendilab/DI-engine/blob/main/ding/data/torch_utils/optimizer_helper.py) |        python3 -u multi_mnist_pcgrad_main.py -s 0       |
+|  53  |         [edac](https://arxiv.org/pdf/2110.01548.pdf)          | ![offline](https://img.shields.io/badge/-offlineRL-darkblue) | [EDAC doc](https://di-engine-docs.readthedocs.io/en/latest/12_policies/edac.html)<br>[policy/edac](https://github.com/opendilab/DI-engine/blob/main/ding/policy/edac.py) |                 python3 -u d4rl_edac_main.py                  |
 </details>
 
 
 ### Environment Versatility
 <details open>
 <summary>(Click to Collapse)</summary>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: DI-engine Version: 0.4.7 Summary: Decision AI
+Metadata-Version: 2.1 Name: DI-engine Version: 0.4.8 Summary: Decision AI
 Engine Home-page: https://github.com/opendilab/DI-engine Author: OpenDILab
 Contributors Author-email: opendilab@pjlab.org.cn License: Apache License,
 Version 2.0 Keywords: Decision AI Engine Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Science/Research Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Operating System
 :: POSIX :: Linux Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X Classifier: Programming
@@ -48,16 +48,16 @@
 commit-activity/m/opendilab/DI-engine) [![GitHub issues](https://
 img.shields.io/github/issues/opendilab/DI-engine)](https://github.com/
 opendilab/DI-engine/issues) [![GitHub pulls](https://img.shields.io/github/
 issues-pr/opendilab/DI-engine)](https://github.com/opendilab/DI-engine/pulls)
 [![Contributors](https://img.shields.io/github/contributors/opendilab/DI-
 engine)](https://github.com/opendilab/DI-engine/graphs/contributors) [![GitHub
 license](https://img.shields.io/github/license/opendilab/DI-engine)](https://
-github.com/opendilab/DI-engine/blob/master/LICENSE) Updated on 2023.04.11 DI-
-engine-v0.4.7 ## Introduction to DI-engine [Documentation](https://di-engine-
+github.com/opendilab/DI-engine/blob/master/LICENSE) Updated on 2023.05.25 DI-
+engine-v0.4.8 ## Introduction to DI-engine [Documentation](https://di-engine-
 docs.readthedocs.io/en/latest/) | [ä¸­æææ¡£](https://di-engine-
 docs.readthedocs.io/zh_CN/latest/) | [Tutorials](https://di-engine-
 docs.readthedocs.io/en/latest/01_quickstart/index.html) | [Feature](#feature) |
 [Task & Middleware](https://di-engine-docs.readthedocs.io/en/latest/03_system/
 index.html) | [TreeTensor](#general-data-container-treetensor) | [Roadmap]
 (https://github.com/opendilab/DI-engine/issues/548) **DI-engine** is a
 generalized decision intelligence engine for PyTorch and JAX. It provides
@@ -454,19 +454,24 @@
 [PLR doc](https://di-engine-docs.readthedocs.io/en/latest/12_policies/plr.html)
 [data/level_replay/level_sampler](https://github.com/opendilab/DI-engine/blob/
 main/ding/data/level_replay/level_sampler.py) | python3 -
 u bigfish_plr_config.py -s 0 | | 52 | [PCGrad](https://arxiv.org/pdf/
 2001.06782.pdf) | ![other](https://img.shields.io/badge/-other-lightgrey) |
 [torch_utils/optimizer_helper/PCGrad](https://github.com/opendilab/DI-engine/
 blob/main/ding/data/torch_utils/optimizer_helper.py) | python3 -
-u multi_mnist_pcgrad_main.py -s 0 |  ### Environment Versatility  (Click to
-Collapse) | No | Environment | Label | Visualization | Code and Doc Links | | :
---: | :--------------------------------------: | :-----------------------------
-----: | :--------------------------------:|:-----------------------------------
-----------------------: | | 1 | [Atari](https://github.com/openai/gym/tree/
+u multi_mnist_pcgrad_main.py -s 0 | | 53 | [edac](https://arxiv.org/pdf/
+2110.01548.pdf) | ![offline](https://img.shields.io/badge/-offlineRL-darkblue)
+| [EDAC doc](https://di-engine-docs.readthedocs.io/en/latest/12_policies/
+edac.html)
+[policy/edac](https://github.com/opendilab/DI-engine/blob/main/ding/policy/
+edac.py) | python3 -u d4rl_edac_main.py |  ### Environment Versatility  (Click
+to Collapse) | No | Environment | Label | Visualization | Code and Doc Links |
+| :--: | :--------------------------------------: | :--------------------------
+-------: | :--------------------------------:|:--------------------------------
+-------------------------: | | 1 | [Atari](https://github.com/openai/gym/tree/
 master/gym/envs/atari) | ![discrete](https://img.shields.io/badge/-discrete-
 brightgreen) | ![original](./dizoo/atari/atari.gif) | [dizoo link](https://
 github.com/opendilab/DI-engine/tree/main/dizoo/atari/envs)
 [env tutorial](https://di-engine-docs.readthedocs.io/en/latest/13_envs/
 atari.html)
 [ç¯å¢æå](https://di-engine-docs.readthedocs.io/zh_CN/latest/13_envs/
 atari_zh.html) | | 2 | [box2d/bipedalwalker](https://github.com/openai/gym/
```

### Comparing `DI-engine-0.4.7/DI_engine.egg-info/SOURCES.txt` & `DI-engine-0.4.8/DI_engine.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -112,19 +112,23 @@
 ding/example/dqn.py
 ding/example/dqn_her.py
 ding/example/dqn_new_env.py
 ding/example/dqn_nstep.py
 ding/example/dqn_per.py
 ding/example/dqn_rnd.py
 ding/example/dt.py
+ding/example/edac.py
 ding/example/iqn_nstep.py
+ding/example/mappo.py
+ding/example/masac.py
 ding/example/pdqn.py
 ding/example/ppg_offpolicy.py
 ding/example/ppo.py
 ding/example/ppo_offpolicy.py
+ding/example/ppo_with_complex_obs.py
 ding/example/qrdqn_nstep.py
 ding/example/r2d2.py
 ding/example/sac.py
 ding/example/sqil.py
 ding/example/sqil_continuous.py
 ding/example/sql.py
 ding/example/td3.py
@@ -136,14 +140,15 @@
 ding/framework/supervisor.py
 ding/framework/task.py
 ding/framework/message_queue/__init__.py
 ding/framework/message_queue/mq.py
 ding/framework/message_queue/nng.py
 ding/framework/message_queue/redis.py
 ding/framework/middleware/__init__.py
+ding/framework/middleware/barrier.py
 ding/framework/middleware/ckpt_handler.py
 ding/framework/middleware/collector.py
 ding/framework/middleware/distributer.py
 ding/framework/middleware/learner.py
 ding/framework/middleware/functional/__init__.py
 ding/framework/middleware/functional/advantage_estimator.py
 ding/framework/middleware/functional/collector.py
@@ -155,14 +160,15 @@
 ding/framework/middleware/functional/logger.py
 ding/framework/middleware/functional/termination_checker.py
 ding/framework/middleware/functional/timer.py
 ding/framework/middleware/functional/trainer.py
 ding/framework/middleware/tests/__init__.py
 ding/framework/middleware/tests/mock_for_test.py
 ding/framework/middleware/tests/test_advantage_estimator.py
+ding/framework/middleware/tests/test_barrier.py
 ding/framework/middleware/tests/test_ckpt_handler.py
 ding/framework/middleware/tests/test_collector.py
 ding/framework/middleware/tests/test_data_processor.py
 ding/framework/middleware/tests/test_distributer.py
 ding/framework/middleware/tests/test_enhancer.py
 ding/framework/middleware/tests/test_evaluator.py
 ding/framework/middleware/tests/test_explorer.py
@@ -252,14 +258,15 @@
 ding/model/template/acer.py
 ding/model/template/atoc.py
 ding/model/template/bc.py
 ding/model/template/collaq.py
 ding/model/template/coma.py
 ding/model/template/decision_transformer.py
 ding/model/template/ebm.py
+ding/model/template/edac.py
 ding/model/template/madqn.py
 ding/model/template/maqac.py
 ding/model/template/mavac.py
 ding/model/template/ngu.py
 ding/model/template/pdqn.py
 ding/model/template/pg.py
 ding/model/template/ppg.py
@@ -290,14 +297,15 @@
 ding/policy/common_utils.py
 ding/policy/cql.py
 ding/policy/d4pg.py
 ding/policy/ddpg.py
 ding/policy/decision_transformer.py
 ding/policy/dqfd.py
 ding/policy/dqn.py
+ding/policy/edac.py
 ding/policy/fqf.py
 ding/policy/ibc.py
 ding/policy/il.py
 ding/policy/impala.py
 ding/policy/iqn.py
 ding/policy/madqn.py
 ding/policy/mdqn.py
@@ -483,14 +491,15 @@
 ding/worker/collector/tests/__init__.py
 ding/worker/collector/tests/fake_cls_policy.py
 ding/worker/collector/tests/fake_cpong_dqn_config.py
 ding/worker/collector/tests/test_base_serial_collector.py
 ding/worker/collector/tests/test_episode_serial_collector.py
 ding/worker/collector/tests/test_marine_parallel_collector.py
 ding/worker/collector/tests/test_metric_serial_evaluator.py
+ding/worker/collector/tests/test_sample_serial_collector.py
 ding/worker/collector/tests/speed_test/__init__.py
 ding/worker/collector/tests/speed_test/fake_env.py
 ding/worker/collector/tests/speed_test/fake_policy.py
 ding/worker/collector/tests/speed_test/test_collector_profile.py
 ding/worker/collector/tests/speed_test/utils.py
 ding/worker/coordinator/__init__.py
 ding/worker/coordinator/base_parallel_commander.py
@@ -644,14 +653,15 @@
 dizoo/bitflip/envs/__init__.py
 dizoo/bitflip/envs/bitflip_env.py
 dizoo/bitflip/envs/test_bitfilp_env.py
 dizoo/box2d/__init__.py
 dizoo/box2d/bipedalwalker/__init__.py
 dizoo/box2d/bipedalwalker/config/__init__.py
 dizoo/box2d/bipedalwalker/config/bipedalwalker_bco_config.py
+dizoo/box2d/bipedalwalker/config/bipedalwalker_ddpg_config.py
 dizoo/box2d/bipedalwalker/config/bipedalwalker_dt_config.py
 dizoo/box2d/bipedalwalker/config/bipedalwalker_gail_sac_config.py
 dizoo/box2d/bipedalwalker/config/bipedalwalker_impala_config.py
 dizoo/box2d/bipedalwalker/config/bipedalwalker_ppo_config.py
 dizoo/box2d/bipedalwalker/config/bipedalwalker_ppopg_config.py
 dizoo/box2d/bipedalwalker/config/bipedalwalker_sac_config.py
 dizoo/box2d/bipedalwalker/config/bipedalwalker_td3_config.py
@@ -822,32 +832,36 @@
 dizoo/d4rl/__init__.py
 dizoo/d4rl/config/__init__.py
 dizoo/d4rl/config/halfcheetah_expert_cql_config.py
 dizoo/d4rl/config/halfcheetah_expert_dt_config.py
 dizoo/d4rl/config/halfcheetah_expert_td3bc_config.py
 dizoo/d4rl/config/halfcheetah_medium_cql_config.py
 dizoo/d4rl/config/halfcheetah_medium_dt_config.py
+dizoo/d4rl/config/halfcheetah_medium_edac_config.py
 dizoo/d4rl/config/halfcheetah_medium_expert_cql_config.py
 dizoo/d4rl/config/halfcheetah_medium_expert_dt_config.py
+dizoo/d4rl/config/halfcheetah_medium_expert_edac_config.py
 dizoo/d4rl/config/halfcheetah_medium_expert_td3bc_config.py
 dizoo/d4rl/config/halfcheetah_medium_replay_cql_config.py
 dizoo/d4rl/config/halfcheetah_medium_replay_dt_config.py
 dizoo/d4rl/config/halfcheetah_medium_replay_td3bc_config.py
 dizoo/d4rl/config/halfcheetah_medium_td3bc_config.py
 dizoo/d4rl/config/halfcheetah_random_cql_config.py
 dizoo/d4rl/config/halfcheetah_random_dt_config.py
 dizoo/d4rl/config/halfcheetah_random_td3bc_config.py
 dizoo/d4rl/config/hopper_expert_cql_config.py
 dizoo/d4rl/config/hopper_expert_dt_config.py
 dizoo/d4rl/config/hopper_expert_td3bc_config.py
 dizoo/d4rl/config/hopper_medium_cql_config.py
 dizoo/d4rl/config/hopper_medium_dt_config.py
+dizoo/d4rl/config/hopper_medium_edac_config.py
 dizoo/d4rl/config/hopper_medium_expert_bc_config.py
 dizoo/d4rl/config/hopper_medium_expert_cql_config.py
 dizoo/d4rl/config/hopper_medium_expert_dt_config.py
+dizoo/d4rl/config/hopper_medium_expert_edac_config.py
 dizoo/d4rl/config/hopper_medium_expert_ibc_ar_config.py
 dizoo/d4rl/config/hopper_medium_expert_ibc_config.py
 dizoo/d4rl/config/hopper_medium_expert_ibc_mcmc_config.py
 dizoo/d4rl/config/hopper_medium_expert_td3bc_config.py
 dizoo/d4rl/config/hopper_medium_replay_cql_config.py
 dizoo/d4rl/config/hopper_medium_replay_dt_config.py
 dizoo/d4rl/config/hopper_medium_replay_td3bc_config.py
@@ -877,14 +891,15 @@
 dizoo/d4rl/config/walker2d_medium_td3bc_config.py
 dizoo/d4rl/config/walker2d_random_cql_config.py
 dizoo/d4rl/config/walker2d_random_dt_config.py
 dizoo/d4rl/config/walker2d_random_td3bc_config.py
 dizoo/d4rl/entry/__init__.py
 dizoo/d4rl/entry/d4rl_cql_main.py
 dizoo/d4rl/entry/d4rl_dt_main.py
+dizoo/d4rl/entry/d4rl_edac_main.py
 dizoo/d4rl/entry/d4rl_ibc_main.py
 dizoo/d4rl/entry/d4rl_td3_bc_main.py
 dizoo/d4rl/envs/__init__.py
 dizoo/d4rl/envs/d4rl_env.py
 dizoo/d4rl/envs/d4rl_wrappers.py
 dizoo/dmc2gym/__init__.py
 dizoo/dmc2gym/envs/__init__.py
```

### Comparing `DI-engine-0.4.7/DI_engine.egg-info/requires.txt` & `DI-engine-0.4.8/DI_engine.egg-info/requires.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 setuptools<=66.1.1
 gym==0.25.1
-torch<=1.12.1,>=1.1.0
 numpy>=1.18.0
 pandas
 tensorboardX>=2.2
 requests>=2.25.1
 pyyaml
 easydict==1.9
 protobuf
@@ -22,15 +21,15 @@
 readerwriterlock
 enum_tools
 trueskill
 h5py
 mpire>=2.3.5
 pynng
 redis
-pettingzoo
+pettingzoo<=1.22.3
 DI-treetensor>=0.3.0
 DI-toolkit>=0.0.2
 hbutils>=0.5.0
 wandb
 matplotlib
 MarkupSafe==2.0.1
 h5py
```

### Comparing `DI-engine-0.4.7/LICENSE` & `DI-engine-0.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/PKG-INFO` & `DI-engine-0.4.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DI-engine
-Version: 0.4.7
+Version: 0.4.8
 Summary: Decision AI Engine
 Home-page: https://github.com/opendilab/DI-engine
 Author: OpenDILab Contributors
 Author-email: opendilab@pjlab.org.cn
 License: Apache License, Version 2.0
 Keywords: Decision AI Engine
 Classifier: Development Status :: 5 - Production/Stable
@@ -66,15 +66,15 @@
 [![GitHub forks](https://img.shields.io/github/forks/opendilab/DI-engine)](https://github.com/opendilab/DI-engine/network)
 ![GitHub commit activity](https://img.shields.io/github/commit-activity/m/opendilab/DI-engine)
 [![GitHub issues](https://img.shields.io/github/issues/opendilab/DI-engine)](https://github.com/opendilab/DI-engine/issues)
 [![GitHub pulls](https://img.shields.io/github/issues-pr/opendilab/DI-engine)](https://github.com/opendilab/DI-engine/pulls)
 [![Contributors](https://img.shields.io/github/contributors/opendilab/DI-engine)](https://github.com/opendilab/DI-engine/graphs/contributors)
 [![GitHub license](https://img.shields.io/github/license/opendilab/DI-engine)](https://github.com/opendilab/DI-engine/blob/master/LICENSE)
 
-Updated on 2023.04.11 DI-engine-v0.4.7
+Updated on 2023.05.25 DI-engine-v0.4.8
 
 
 ## Introduction to DI-engine
 [Documentation](https://di-engine-docs.readthedocs.io/en/latest/) | [中文文档](https://di-engine-docs.readthedocs.io/zh_CN/latest/) | [Tutorials](https://di-engine-docs.readthedocs.io/en/latest/01_quickstart/index.html) | [Feature](#feature) | [Task & Middleware](https://di-engine-docs.readthedocs.io/en/latest/03_system/index.html) | [TreeTensor](#general-data-container-treetensor) | [Roadmap](https://github.com/opendilab/DI-engine/issues/548)
 
 **DI-engine** is a generalized decision intelligence engine for PyTorch and JAX. 
 
@@ -286,14 +286,15 @@
 |  46  |         [MBPO](https://arxiv.org/pdf/1906.08253.pdf)         | ![mbrl](https://img.shields.io/badge/-ModelBasedRL-lightblue) | [MBPO doc](https://di-engine-docs.readthedocs.io/en/latest/12_policies/mbpo.html)<br>[world_model/mbpo](https://github.com/opendilab/DI-engine/blob/main/ding/world_model/mbpo.py) |        python3 -u pendulum_sac_mbpo_config.py    |
 |  47  |         [DDPPO](https://openreview.net/forum?id=rzvOQrnclO0)         | ![mbrl](https://img.shields.io/badge/-ModelBasedRL-lightblue) | [world_model/ddppo](https://github.com/opendilab/DI-engine/blob/main/ding/world_model/ddppo.py) |        python3 -u pendulum_mbsac_ddppo_config.py    |
 |  48  |         [PER](https://arxiv.org/pdf/1511.05952.pdf)          |   ![other](https://img.shields.io/badge/-other-lightgrey)    | [worker/replay_buffer](https://github.com/opendilab/DI-engine/blob/main/ding/worker/replay_buffer/advanced_buffer.py) |                        `rainbow demo`                        |
 |  49  |         [GAE](https://arxiv.org/pdf/1506.02438.pdf)          |   ![other](https://img.shields.io/badge/-other-lightgrey)    | [rl_utils/gae](https://github.com/opendilab/DI-engine/blob/main/ding/rl_utils/gae.py) |                          `ppo demo`                          |
 |  50  |         [ST-DIM](https://arxiv.org/pdf/1906.08226.pdf)          |   ![other](https://img.shields.io/badge/-other-lightgrey)    | [torch_utils/loss/contrastive_loss](https://github.com/opendilab/DI-engine/blob/main/ding/torch_utils/loss/contrastive_loss.py) |        ding -m serial -c cartpole_dqn_stdim_config.py -s 0       |
 |  51  |         [PLR](https://arxiv.org/pdf/2010.03934.pdf)          |   ![other](https://img.shields.io/badge/-other-lightgrey)    | [PLR doc](https://di-engine-docs.readthedocs.io/en/latest/12_policies/plr.html)<br>[data/level_replay/level_sampler](https://github.com/opendilab/DI-engine/blob/main/ding/data/level_replay/level_sampler.py) |        python3 -u bigfish_plr_config.py -s 0       |
 |  52  |         [PCGrad](https://arxiv.org/pdf/2001.06782.pdf)          |   ![other](https://img.shields.io/badge/-other-lightgrey)    | [torch_utils/optimizer_helper/PCGrad](https://github.com/opendilab/DI-engine/blob/main/ding/data/torch_utils/optimizer_helper.py) |        python3 -u multi_mnist_pcgrad_main.py -s 0       |
+|  53  |         [edac](https://arxiv.org/pdf/2110.01548.pdf)          | ![offline](https://img.shields.io/badge/-offlineRL-darkblue) | [EDAC doc](https://di-engine-docs.readthedocs.io/en/latest/12_policies/edac.html)<br>[policy/edac](https://github.com/opendilab/DI-engine/blob/main/ding/policy/edac.py) |                 python3 -u d4rl_edac_main.py                  |
 </details>
 
 
 ### Environment Versatility
 <details open>
 <summary>(Click to Collapse)</summary>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: DI-engine Version: 0.4.7 Summary: Decision AI
+Metadata-Version: 2.1 Name: DI-engine Version: 0.4.8 Summary: Decision AI
 Engine Home-page: https://github.com/opendilab/DI-engine Author: OpenDILab
 Contributors Author-email: opendilab@pjlab.org.cn License: Apache License,
 Version 2.0 Keywords: Decision AI Engine Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Science/Research Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Operating System
 :: POSIX :: Linux Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X Classifier: Programming
@@ -48,16 +48,16 @@
 commit-activity/m/opendilab/DI-engine) [![GitHub issues](https://
 img.shields.io/github/issues/opendilab/DI-engine)](https://github.com/
 opendilab/DI-engine/issues) [![GitHub pulls](https://img.shields.io/github/
 issues-pr/opendilab/DI-engine)](https://github.com/opendilab/DI-engine/pulls)
 [![Contributors](https://img.shields.io/github/contributors/opendilab/DI-
 engine)](https://github.com/opendilab/DI-engine/graphs/contributors) [![GitHub
 license](https://img.shields.io/github/license/opendilab/DI-engine)](https://
-github.com/opendilab/DI-engine/blob/master/LICENSE) Updated on 2023.04.11 DI-
-engine-v0.4.7 ## Introduction to DI-engine [Documentation](https://di-engine-
+github.com/opendilab/DI-engine/blob/master/LICENSE) Updated on 2023.05.25 DI-
+engine-v0.4.8 ## Introduction to DI-engine [Documentation](https://di-engine-
 docs.readthedocs.io/en/latest/) | [ä¸­æææ¡£](https://di-engine-
 docs.readthedocs.io/zh_CN/latest/) | [Tutorials](https://di-engine-
 docs.readthedocs.io/en/latest/01_quickstart/index.html) | [Feature](#feature) |
 [Task & Middleware](https://di-engine-docs.readthedocs.io/en/latest/03_system/
 index.html) | [TreeTensor](#general-data-container-treetensor) | [Roadmap]
 (https://github.com/opendilab/DI-engine/issues/548) **DI-engine** is a
 generalized decision intelligence engine for PyTorch and JAX. It provides
@@ -454,19 +454,24 @@
 [PLR doc](https://di-engine-docs.readthedocs.io/en/latest/12_policies/plr.html)
 [data/level_replay/level_sampler](https://github.com/opendilab/DI-engine/blob/
 main/ding/data/level_replay/level_sampler.py) | python3 -
 u bigfish_plr_config.py -s 0 | | 52 | [PCGrad](https://arxiv.org/pdf/
 2001.06782.pdf) | ![other](https://img.shields.io/badge/-other-lightgrey) |
 [torch_utils/optimizer_helper/PCGrad](https://github.com/opendilab/DI-engine/
 blob/main/ding/data/torch_utils/optimizer_helper.py) | python3 -
-u multi_mnist_pcgrad_main.py -s 0 |  ### Environment Versatility  (Click to
-Collapse) | No | Environment | Label | Visualization | Code and Doc Links | | :
---: | :--------------------------------------: | :-----------------------------
-----: | :--------------------------------:|:-----------------------------------
-----------------------: | | 1 | [Atari](https://github.com/openai/gym/tree/
+u multi_mnist_pcgrad_main.py -s 0 | | 53 | [edac](https://arxiv.org/pdf/
+2110.01548.pdf) | ![offline](https://img.shields.io/badge/-offlineRL-darkblue)
+| [EDAC doc](https://di-engine-docs.readthedocs.io/en/latest/12_policies/
+edac.html)
+[policy/edac](https://github.com/opendilab/DI-engine/blob/main/ding/policy/
+edac.py) | python3 -u d4rl_edac_main.py |  ### Environment Versatility  (Click
+to Collapse) | No | Environment | Label | Visualization | Code and Doc Links |
+| :--: | :--------------------------------------: | :--------------------------
+-------: | :--------------------------------:|:--------------------------------
+-------------------------: | | 1 | [Atari](https://github.com/openai/gym/tree/
 master/gym/envs/atari) | ![discrete](https://img.shields.io/badge/-discrete-
 brightgreen) | ![original](./dizoo/atari/atari.gif) | [dizoo link](https://
 github.com/opendilab/DI-engine/tree/main/dizoo/atari/envs)
 [env tutorial](https://di-engine-docs.readthedocs.io/en/latest/13_envs/
 atari.html)
 [ç¯å¢æå](https://di-engine-docs.readthedocs.io/zh_CN/latest/13_envs/
 atari_zh.html) | | 2 | [box2d/bipedalwalker](https://github.com/openai/gym/
```

### Comparing `DI-engine-0.4.7/README.md` & `DI-engine-0.4.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 [![GitHub forks](https://img.shields.io/github/forks/opendilab/DI-engine)](https://github.com/opendilab/DI-engine/network)
 ![GitHub commit activity](https://img.shields.io/github/commit-activity/m/opendilab/DI-engine)
 [![GitHub issues](https://img.shields.io/github/issues/opendilab/DI-engine)](https://github.com/opendilab/DI-engine/issues)
 [![GitHub pulls](https://img.shields.io/github/issues-pr/opendilab/DI-engine)](https://github.com/opendilab/DI-engine/pulls)
 [![Contributors](https://img.shields.io/github/contributors/opendilab/DI-engine)](https://github.com/opendilab/DI-engine/graphs/contributors)
 [![GitHub license](https://img.shields.io/github/license/opendilab/DI-engine)](https://github.com/opendilab/DI-engine/blob/master/LICENSE)
 
-Updated on 2023.04.11 DI-engine-v0.4.7
+Updated on 2023.05.25 DI-engine-v0.4.8
 
 
 ## Introduction to DI-engine
 [Documentation](https://di-engine-docs.readthedocs.io/en/latest/) | [中文文档](https://di-engine-docs.readthedocs.io/zh_CN/latest/) | [Tutorials](https://di-engine-docs.readthedocs.io/en/latest/01_quickstart/index.html) | [Feature](#feature) | [Task & Middleware](https://di-engine-docs.readthedocs.io/en/latest/03_system/index.html) | [TreeTensor](#general-data-container-treetensor) | [Roadmap](https://github.com/opendilab/DI-engine/issues/548)
 
 **DI-engine** is a generalized decision intelligence engine for PyTorch and JAX. 
 
@@ -248,14 +248,15 @@
 |  46  |         [MBPO](https://arxiv.org/pdf/1906.08253.pdf)         | ![mbrl](https://img.shields.io/badge/-ModelBasedRL-lightblue) | [MBPO doc](https://di-engine-docs.readthedocs.io/en/latest/12_policies/mbpo.html)<br>[world_model/mbpo](https://github.com/opendilab/DI-engine/blob/main/ding/world_model/mbpo.py) |        python3 -u pendulum_sac_mbpo_config.py    |
 |  47  |         [DDPPO](https://openreview.net/forum?id=rzvOQrnclO0)         | ![mbrl](https://img.shields.io/badge/-ModelBasedRL-lightblue) | [world_model/ddppo](https://github.com/opendilab/DI-engine/blob/main/ding/world_model/ddppo.py) |        python3 -u pendulum_mbsac_ddppo_config.py    |
 |  48  |         [PER](https://arxiv.org/pdf/1511.05952.pdf)          |   ![other](https://img.shields.io/badge/-other-lightgrey)    | [worker/replay_buffer](https://github.com/opendilab/DI-engine/blob/main/ding/worker/replay_buffer/advanced_buffer.py) |                        `rainbow demo`                        |
 |  49  |         [GAE](https://arxiv.org/pdf/1506.02438.pdf)          |   ![other](https://img.shields.io/badge/-other-lightgrey)    | [rl_utils/gae](https://github.com/opendilab/DI-engine/blob/main/ding/rl_utils/gae.py) |                          `ppo demo`                          |
 |  50  |         [ST-DIM](https://arxiv.org/pdf/1906.08226.pdf)          |   ![other](https://img.shields.io/badge/-other-lightgrey)    | [torch_utils/loss/contrastive_loss](https://github.com/opendilab/DI-engine/blob/main/ding/torch_utils/loss/contrastive_loss.py) |        ding -m serial -c cartpole_dqn_stdim_config.py -s 0       |
 |  51  |         [PLR](https://arxiv.org/pdf/2010.03934.pdf)          |   ![other](https://img.shields.io/badge/-other-lightgrey)    | [PLR doc](https://di-engine-docs.readthedocs.io/en/latest/12_policies/plr.html)<br>[data/level_replay/level_sampler](https://github.com/opendilab/DI-engine/blob/main/ding/data/level_replay/level_sampler.py) |        python3 -u bigfish_plr_config.py -s 0       |
 |  52  |         [PCGrad](https://arxiv.org/pdf/2001.06782.pdf)          |   ![other](https://img.shields.io/badge/-other-lightgrey)    | [torch_utils/optimizer_helper/PCGrad](https://github.com/opendilab/DI-engine/blob/main/ding/data/torch_utils/optimizer_helper.py) |        python3 -u multi_mnist_pcgrad_main.py -s 0       |
+|  53  |         [edac](https://arxiv.org/pdf/2110.01548.pdf)          | ![offline](https://img.shields.io/badge/-offlineRL-darkblue) | [EDAC doc](https://di-engine-docs.readthedocs.io/en/latest/12_policies/edac.html)<br>[policy/edac](https://github.com/opendilab/DI-engine/blob/main/ding/policy/edac.py) |                 python3 -u d4rl_edac_main.py                  |
 </details>
 
 
 ### Environment Versatility
 <details open>
 <summary>(Click to Collapse)</summary>
```

#### html2text {}

```diff
@@ -31,16 +31,16 @@
 commit-activity/m/opendilab/DI-engine) [![GitHub issues](https://
 img.shields.io/github/issues/opendilab/DI-engine)](https://github.com/
 opendilab/DI-engine/issues) [![GitHub pulls](https://img.shields.io/github/
 issues-pr/opendilab/DI-engine)](https://github.com/opendilab/DI-engine/pulls)
 [![Contributors](https://img.shields.io/github/contributors/opendilab/DI-
 engine)](https://github.com/opendilab/DI-engine/graphs/contributors) [![GitHub
 license](https://img.shields.io/github/license/opendilab/DI-engine)](https://
-github.com/opendilab/DI-engine/blob/master/LICENSE) Updated on 2023.04.11 DI-
-engine-v0.4.7 ## Introduction to DI-engine [Documentation](https://di-engine-
+github.com/opendilab/DI-engine/blob/master/LICENSE) Updated on 2023.05.25 DI-
+engine-v0.4.8 ## Introduction to DI-engine [Documentation](https://di-engine-
 docs.readthedocs.io/en/latest/) | [ä¸­æææ¡£](https://di-engine-
 docs.readthedocs.io/zh_CN/latest/) | [Tutorials](https://di-engine-
 docs.readthedocs.io/en/latest/01_quickstart/index.html) | [Feature](#feature) |
 [Task & Middleware](https://di-engine-docs.readthedocs.io/en/latest/03_system/
 index.html) | [TreeTensor](#general-data-container-treetensor) | [Roadmap]
 (https://github.com/opendilab/DI-engine/issues/548) **DI-engine** is a
 generalized decision intelligence engine for PyTorch and JAX. It provides
@@ -437,19 +437,24 @@
 [PLR doc](https://di-engine-docs.readthedocs.io/en/latest/12_policies/plr.html)
 [data/level_replay/level_sampler](https://github.com/opendilab/DI-engine/blob/
 main/ding/data/level_replay/level_sampler.py) | python3 -
 u bigfish_plr_config.py -s 0 | | 52 | [PCGrad](https://arxiv.org/pdf/
 2001.06782.pdf) | ![other](https://img.shields.io/badge/-other-lightgrey) |
 [torch_utils/optimizer_helper/PCGrad](https://github.com/opendilab/DI-engine/
 blob/main/ding/data/torch_utils/optimizer_helper.py) | python3 -
-u multi_mnist_pcgrad_main.py -s 0 |  ### Environment Versatility  (Click to
-Collapse) | No | Environment | Label | Visualization | Code and Doc Links | | :
---: | :--------------------------------------: | :-----------------------------
-----: | :--------------------------------:|:-----------------------------------
-----------------------: | | 1 | [Atari](https://github.com/openai/gym/tree/
+u multi_mnist_pcgrad_main.py -s 0 | | 53 | [edac](https://arxiv.org/pdf/
+2110.01548.pdf) | ![offline](https://img.shields.io/badge/-offlineRL-darkblue)
+| [EDAC doc](https://di-engine-docs.readthedocs.io/en/latest/12_policies/
+edac.html)
+[policy/edac](https://github.com/opendilab/DI-engine/blob/main/ding/policy/
+edac.py) | python3 -u d4rl_edac_main.py |  ### Environment Versatility  (Click
+to Collapse) | No | Environment | Label | Visualization | Code and Doc Links |
+| :--: | :--------------------------------------: | :--------------------------
+-------: | :--------------------------------:|:--------------------------------
+-------------------------: | | 1 | [Atari](https://github.com/openai/gym/tree/
 master/gym/envs/atari) | ![discrete](https://img.shields.io/badge/-discrete-
 brightgreen) | ![original](./dizoo/atari/atari.gif) | [dizoo link](https://
 github.com/opendilab/DI-engine/tree/main/dizoo/atari/envs)
 [env tutorial](https://di-engine-docs.readthedocs.io/en/latest/13_envs/
 atari.html)
 [ç¯å¢æå](https://di-engine-docs.readthedocs.io/zh_CN/latest/13_envs/
 atari_zh.html) | | 2 | [box2d/bipedalwalker](https://github.com/openai/gym/
```

### Comparing `DI-engine-0.4.7/ding/bonus/config.py` & `DI-engine-0.4.8/ding/bonus/config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/bonus/demo.py` & `DI-engine-0.4.8/ding/bonus/demo.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/bonus/model.py` & `DI-engine-0.4.8/ding/bonus/model.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/bonus/ppof.py` & `DI-engine-0.4.8/ding/bonus/ppof.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,15 +87,15 @@
             action_shape = int(action_space.n)
         elif isinstance(action_space, (gym.spaces.Tuple, gymnasium.spaces.Tuple)):
             action_shape = get_hybrid_shape(action_space)
         else:
             action_shape = action_space.shape
 
         # Three types of value normalization is supported currently
-        assert self.cfg.value_norm in ['popart', 'value_rescale', 'symlog']
+        assert self.cfg.value_norm in ['popart', 'value_rescale', 'symlog', 'baseline']
         if model is None:
             if self.cfg.value_norm != 'popart':
                 model = PPOFModel(
                     self.env.observation_space.shape,
                     action_shape,
                     action_space=self.cfg.action_space,
                     **self.cfg.model
```

### Comparing `DI-engine-0.4.7/ding/bonus/td3.py` & `DI-engine-0.4.8/ding/bonus/td3.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/config/config.py` & `DI-engine-0.4.8/ding/config/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -302,15 +302,15 @@
     model=dict(),
     learn=dict(learner=dict()),
     collect=dict(collector=dict()),
     eval=dict(evaluator=dict()),
     other=dict(replay_buffer=dict()),
 )
 policy_config_template = EasyDict(policy_config_template)
-env_config_template = dict(manager=dict(), stop_value=int(1e10))
+env_config_template = dict(manager=dict(), stop_value=int(1e10), n_evaluator_episode=4)
 env_config_template = EasyDict(env_config_template)
 
 
 def save_project_state(exp_name: str) -> None:
 
     def _fn(cmd: str):
         return subprocess.run(cmd, shell=True, stdout=subprocess.PIPE).stdout.strip().decode("utf-8")
@@ -447,22 +447,20 @@
     if create_cfg is not None or buffer is not None:
         policy_config.other.replay_buffer = compile_buffer_config(policy_config, cfg, buffer)
     default_config = EasyDict({'env': env_config, 'policy': policy_config})
     if len(reward_model_config) > 0:
         default_config['reward_model'] = reward_model_config
     if len(world_model_config) > 0:
         default_config['world_model'] = world_model_config
-    stop_value_flag = 'stop_value' in cfg.env
     cfg = deep_merge_dicts(default_config, cfg)
     cfg.seed = seed
     # check important key in config
     if evaluator in [InteractionSerialEvaluator, BattleInteractionSerialEvaluator]:  # env interaction evaluation
-        if stop_value_flag:  # data generation task doesn't need these fields
-            cfg.policy.eval.evaluator.n_episode = cfg.env.n_evaluator_episode
-            cfg.policy.eval.evaluator.stop_value = cfg.env.stop_value
+        cfg.policy.eval.evaluator.stop_value = cfg.env.stop_value
+        cfg.policy.eval.evaluator.n_episode = cfg.env.n_evaluator_episode
     if 'exp_name' not in cfg:
         cfg.exp_name = 'default_experiment'
     if save_cfg:
         if os.path.exists(cfg.exp_name) and renew_dir:
             cfg.exp_name += datetime.datetime.now().strftime("_%y%m%d_%H%M%S")
         try:
             os.makedirs(cfg.exp_name)
```

### Comparing `DI-engine-0.4.7/ding/config/utils.py` & `DI-engine-0.4.8/ding/config/utils.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/data/buffer/buffer.py` & `DI-engine-0.4.8/ding/data/buffer/buffer.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/data/buffer/deque_buffer.py` & `DI-engine-0.4.8/ding/data/buffer/deque_buffer.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/data/buffer/deque_buffer_wrapper.py` & `DI-engine-0.4.8/ding/data/buffer/deque_buffer_wrapper.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/data/buffer/middleware/clone_object.py` & `DI-engine-0.4.8/ding/data/buffer/middleware/clone_object.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/data/buffer/middleware/group_sample.py` & `DI-engine-0.4.8/ding/data/buffer/middleware/group_sample.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/data/buffer/middleware/padding.py` & `DI-engine-0.4.8/ding/data/buffer/middleware/padding.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/data/buffer/middleware/priority.py` & `DI-engine-0.4.8/ding/data/buffer/middleware/priority.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/data/buffer/middleware/sample_range_view.py` & `DI-engine-0.4.8/ding/data/buffer/middleware/sample_range_view.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/data/buffer/middleware/staleness_check.py` & `DI-engine-0.4.8/ding/data/buffer/middleware/staleness_check.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/data/buffer/middleware/use_time_check.py` & `DI-engine-0.4.8/ding/data/buffer/middleware/use_time_check.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/data/level_replay/level_sampler.py` & `DI-engine-0.4.8/ding/data/level_replay/level_sampler.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/data/model_loader.py` & `DI-engine-0.4.8/ding/data/model_loader.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/data/shm_buffer.py` & `DI-engine-0.4.8/ding/data/shm_buffer.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/data/storage/file.py` & `DI-engine-0.4.8/ding/data/storage/file.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/data/storage_loader.py` & `DI-engine-0.4.8/ding/data/storage_loader.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/entry/__init__.py` & `DI-engine-0.4.8/ding/entry/__init__.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/entry/application_entry.py` & `DI-engine-0.4.8/ding/entry/application_entry.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/entry/application_entry_drex_collect_data.py` & `DI-engine-0.4.8/ding/entry/application_entry_drex_collect_data.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/entry/application_entry_trex_collect_data.py` & `DI-engine-0.4.8/ding/entry/application_entry_trex_collect_data.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/entry/cli.py` & `DI-engine-0.4.8/ding/entry/cli.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/entry/cli_ditask.py` & `DI-engine-0.4.8/ding/entry/cli_ditask.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/entry/cli_parsers/k8s_parser.py` & `DI-engine-0.4.8/ding/entry/cli_parsers/k8s_parser.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/entry/cli_parsers/slurm_parser.py` & `DI-engine-0.4.8/ding/entry/cli_parsers/slurm_parser.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/entry/dist_entry.py` & `DI-engine-0.4.8/ding/entry/dist_entry.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/entry/parallel_entry.py` & `DI-engine-0.4.8/ding/entry/parallel_entry.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/entry/predefined_config.py` & `DI-engine-0.4.8/ding/entry/predefined_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/entry/serial_entry.py` & `DI-engine-0.4.8/ding/entry/serial_entry.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/entry/serial_entry_bc.py` & `DI-engine-0.4.8/ding/entry/serial_entry_bc.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/entry/serial_entry_bco.py` & `DI-engine-0.4.8/ding/entry/serial_entry_bco.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/entry/serial_entry_decision_transformer.py` & `DI-engine-0.4.8/ding/entry/serial_entry_decision_transformer.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/entry/serial_entry_dqfd.py` & `DI-engine-0.4.8/ding/entry/serial_entry_dqfd.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/entry/serial_entry_gail.py` & `DI-engine-0.4.8/ding/entry/serial_entry_gail.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/entry/serial_entry_guided_cost.py` & `DI-engine-0.4.8/ding/entry/serial_entry_guided_cost.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/entry/serial_entry_mbrl.py` & `DI-engine-0.4.8/ding/entry/serial_entry_mbrl.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/entry/serial_entry_ngu.py` & `DI-engine-0.4.8/ding/entry/serial_entry_ngu.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/entry/serial_entry_offline.py` & `DI-engine-0.4.8/ding/entry/serial_entry_offline.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/entry/serial_entry_onpolicy.py` & `DI-engine-0.4.8/ding/entry/serial_entry_onpolicy.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/entry/serial_entry_onpolicy_ppg.py` & `DI-engine-0.4.8/ding/entry/serial_entry_onpolicy_ppg.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/entry/serial_entry_pc.py` & `DI-engine-0.4.8/ding/entry/serial_entry_pc.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/entry/serial_entry_plr.py` & `DI-engine-0.4.8/ding/entry/serial_entry_plr.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/entry/serial_entry_preference_based_irl.py` & `DI-engine-0.4.8/ding/entry/serial_entry_preference_based_irl.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/entry/serial_entry_preference_based_irl_onpolicy.py` & `DI-engine-0.4.8/ding/entry/serial_entry_preference_based_irl_onpolicy.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/entry/serial_entry_r2d3.py` & `DI-engine-0.4.8/ding/entry/serial_entry_r2d3.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/entry/serial_entry_reward_model_offpolicy.py` & `DI-engine-0.4.8/ding/entry/serial_entry_reward_model_offpolicy.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/entry/serial_entry_reward_model_onpolicy.py` & `DI-engine-0.4.8/ding/entry/serial_entry_reward_model_onpolicy.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/entry/serial_entry_sqil.py` & `DI-engine-0.4.8/ding/entry/serial_entry_sqil.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/entry/serial_entry_td3_vae.py` & `DI-engine-0.4.8/ding/entry/serial_entry_td3_vae.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/entry/utils.py` & `DI-engine-0.4.8/ding/entry/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -55,12 +55,14 @@
         action_space = collector_env.action_space
         random_policy = PolicyFactory.get_random_policy(policy.collect_mode, action_space=action_space)
         collector.reset_policy(random_policy)
     collect_kwargs = commander.step()
     if policy_cfg.collect.collector.type == 'episode':
         new_data = collector.collect(n_episode=policy_cfg.random_collect_size, policy_kwargs=collect_kwargs)
     else:
-        new_data = collector.collect(n_sample=policy_cfg.random_collect_size, policy_kwargs=collect_kwargs)
+        new_data = collector.collect(
+            n_sample=policy_cfg.random_collect_size, record_random_collect=False, policy_kwargs=collect_kwargs
+        )  # 'record_random_collect=False' means random collect without output log
     if postprocess_data_fn is not None:
         new_data = postprocess_data_fn(new_data)
     replay_buffer.push(new_data, cur_collector_envstep=0)
     collector.reset_policy(policy.collect_mode)
```

### Comparing `DI-engine-0.4.7/ding/envs/common/common_function.py` & `DI-engine-0.4.8/ding/envs/common/common_function.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/envs/common/env_element.py` & `DI-engine-0.4.8/ding/envs/common/env_element.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/envs/common/env_element_runner.py` & `DI-engine-0.4.8/ding/envs/common/env_element_runner.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/envs/env/base_env.py` & `DI-engine-0.4.8/ding/envs/env/base_env.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/envs/env/default_wrapper.py` & `DI-engine-0.4.8/ding/envs/env/default_wrapper.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/envs/env/ding_env_wrapper.py` & `DI-engine-0.4.8/ding/envs/env/ding_env_wrapper.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/envs/env/env_implementation_check.py` & `DI-engine-0.4.8/ding/envs/env/env_implementation_check.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/envs/env/tests/demo_env.py` & `DI-engine-0.4.8/ding/envs/env/tests/demo_env.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/envs/env/tests/test_ding_env_wrapper.py` & `DI-engine-0.4.8/ding/envs/env/tests/test_ding_env_wrapper.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/envs/env/tests/test_env_implementation_check.py` & `DI-engine-0.4.8/ding/envs/env/tests/test_env_implementation_check.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/envs/env_manager/base_env_manager.py` & `DI-engine-0.4.8/ding/envs/env_manager/base_env_manager.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/envs/env_manager/env_supervisor.py` & `DI-engine-0.4.8/ding/envs/env_manager/env_supervisor.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/envs/env_manager/envpool_env_manager.py` & `DI-engine-0.4.8/ding/envs/env_manager/envpool_env_manager.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/envs/env_manager/gym_vector_env_manager.py` & `DI-engine-0.4.8/ding/envs/env_manager/gym_vector_env_manager.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/envs/env_manager/subprocess_env_manager.py` & `DI-engine-0.4.8/ding/envs/env_manager/subprocess_env_manager.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/envs/env_manager/tests/conftest.py` & `DI-engine-0.4.8/ding/envs/env_manager/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/envs/env_manager/tests/test_base_env_manager.py` & `DI-engine-0.4.8/ding/envs/env_manager/tests/test_base_env_manager.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/envs/env_manager/tests/test_env_supervisor.py` & `DI-engine-0.4.8/ding/envs/env_manager/tests/test_env_supervisor.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/envs/env_manager/tests/test_envpool_env_manager.py` & `DI-engine-0.4.8/ding/envs/env_manager/tests/test_envpool_env_manager.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/envs/env_manager/tests/test_gym_vector_env_manager.py` & `DI-engine-0.4.8/ding/envs/env_manager/tests/test_gym_vector_env_manager.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/envs/env_manager/tests/test_shm.py` & `DI-engine-0.4.8/ding/envs/env_manager/tests/test_shm.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/envs/env_manager/tests/test_subprocess_env_manager.py` & `DI-engine-0.4.8/ding/envs/env_manager/tests/test_subprocess_env_manager.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/envs/env_wrappers/env_wrappers.py` & `DI-engine-0.4.8/ding/envs/env_wrappers/env_wrappers.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/example/c51_nstep.py` & `DI-engine-0.4.8/ding/example/c51_nstep.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/example/collect_demo_data.py` & `DI-engine-0.4.8/ding/example/collect_demo_data.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/example/cql.py` & `DI-engine-0.4.8/ding/example/cql.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/example/d4pg.py` & `DI-engine-0.4.8/ding/example/d4pg.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/example/ddpg.py` & `DI-engine-0.4.8/ding/example/ddpg.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/example/dqn.py` & `DI-engine-0.4.8/ding/example/dqn.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/example/dqn_her.py` & `DI-engine-0.4.8/ding/example/dqn_her.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/example/dqn_new_env.py` & `DI-engine-0.4.8/ding/example/dqn_new_env.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/example/dqn_nstep.py` & `DI-engine-0.4.8/ding/example/dqn_nstep.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/example/dqn_per.py` & `DI-engine-0.4.8/ding/example/dqn_per.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/example/dqn_rnd.py` & `DI-engine-0.4.8/ding/example/dqn_rnd.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/example/dt.py` & `DI-engine-0.4.8/ding/example/dt.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/example/iqn_nstep.py` & `DI-engine-0.4.8/ding/example/iqn_nstep.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/example/pdqn.py` & `DI-engine-0.4.8/ding/example/pdqn.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/example/ppg_offpolicy.py` & `DI-engine-0.4.8/ding/example/ppg_offpolicy.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/example/ppo.py` & `DI-engine-0.4.8/ding/example/ppo.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/example/ppo_offpolicy.py` & `DI-engine-0.4.8/ding/example/ppo_offpolicy.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/example/qrdqn_nstep.py` & `DI-engine-0.4.8/ding/example/qrdqn_nstep.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/example/r2d2.py` & `DI-engine-0.4.8/ding/example/r2d2.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/example/sac.py` & `DI-engine-0.4.8/ding/example/sac.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/example/sqil.py` & `DI-engine-0.4.8/ding/example/sqil.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/example/sqil_continuous.py` & `DI-engine-0.4.8/ding/example/sqil_continuous.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/example/sql.py` & `DI-engine-0.4.8/ding/example/sql.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/example/td3.py` & `DI-engine-0.4.8/ding/example/td3.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,44 +1,47 @@
-import gym
 from ditk import logging
-from ding.model.template.qac import QAC
+from ding.model import QAC
 from ding.policy import TD3Policy
-from ding.envs import DingEnvWrapper, BaseEnvManagerV2
+from ding.envs import BaseEnvManagerV2
 from ding.data import DequeBuffer
 from ding.config import compile_config
-from ding.framework import task
+from ding.framework import task, ding_init
 from ding.framework.context import OnlineRLContext
-from ding.framework.middleware import OffPolicyLearner, StepCollector, interaction_evaluator, data_pusher, CkptSaver
+from ding.framework.middleware import data_pusher, StepCollector, interaction_evaluator, \
+    CkptSaver, OffPolicyLearner, termination_checker, online_logger
 from ding.utils import set_pkg_seed
 from dizoo.classic_control.pendulum.envs.pendulum_env import PendulumEnv
 from dizoo.classic_control.pendulum.config.pendulum_td3_config import main_config, create_config
 
 
 def main():
     logging.getLogger().setLevel(logging.INFO)
     cfg = compile_config(main_config, create_cfg=create_config, auto=True)
+    ding_init(cfg)
     with task.start(async_mode=False, ctx=OnlineRLContext()):
         collector_env = BaseEnvManagerV2(
             env_fn=[lambda: PendulumEnv(cfg.env) for _ in range(cfg.env.collector_env_num)], cfg=cfg.env.manager
         )
         evaluator_env = BaseEnvManagerV2(
             env_fn=[lambda: PendulumEnv(cfg.env) for _ in range(cfg.env.evaluator_env_num)], cfg=cfg.env.manager
         )
 
         set_pkg_seed(cfg.seed, use_cuda=cfg.policy.cuda)
 
         model = QAC(**cfg.policy.model)
         buffer_ = DequeBuffer(size=cfg.policy.other.replay_buffer.replay_buffer_size)
-        policy = TD3Policy(cfg.policy, model)
+        policy = TD3Policy(cfg.policy, model=model)
 
         task.use(interaction_evaluator(cfg, policy.eval_mode, evaluator_env))
         task.use(
             StepCollector(cfg, policy.collect_mode, collector_env, random_collect_size=cfg.policy.random_collect_size)
         )
         task.use(data_pusher(cfg, buffer_))
         task.use(OffPolicyLearner(cfg, policy.learn_mode, buffer_))
         task.use(CkptSaver(policy, cfg.exp_name, train_freq=100))
+        task.use(termination_checker(max_train_iter=10000))
+        task.use(online_logger())
         task.run()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `DI-engine-0.4.7/ding/example/trex.py` & `DI-engine-0.4.8/ding/example/trex.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/framework/context.py` & `DI-engine-0.4.8/ding/framework/context.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/framework/event_loop.py` & `DI-engine-0.4.8/ding/framework/event_loop.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/framework/message_queue/mq.py` & `DI-engine-0.4.8/ding/framework/message_queue/mq.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/framework/message_queue/nng.py` & `DI-engine-0.4.8/ding/framework/message_queue/nng.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/framework/message_queue/redis.py` & `DI-engine-0.4.8/ding/framework/message_queue/redis.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/framework/middleware/ckpt_handler.py` & `DI-engine-0.4.8/ding/framework/middleware/ckpt_handler.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/framework/middleware/collector.py` & `DI-engine-0.4.8/ding/framework/middleware/collector.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/framework/middleware/distributer.py` & `DI-engine-0.4.8/ding/framework/middleware/distributer.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/framework/middleware/functional/__init__.py` & `DI-engine-0.4.8/ding/framework/middleware/functional/__init__.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/framework/middleware/functional/advantage_estimator.py` & `DI-engine-0.4.8/ding/framework/middleware/functional/advantage_estimator.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,35 +36,35 @@
                 Each element should contain the following keys: `obs`, `next_obs`, `reward`, `done`.
             - trajectory_end_idx: (:obj:`treetensor.torch.IntTensor`):
                 The indices that define the end of trajectories, \
                 which should be shorter than the length of `ctx.trajectories`.
         Output of ctx:
             - train_data (:obj:`List[treetensor.torch.Tensor]`): The processed data if `buffer_` is None.
         """
-        data = ctx.trajectories  # list
-        data = ttorch_collate(data)
+        cuda = cfg.policy.cuda and torch.cuda.is_available()
+        data = ctx.trajectories  # List
+        data = ttorch_collate(data)  # ttorch.Tensor
         with torch.no_grad():
-            if cfg.policy.cuda:
+            if cuda:
                 data = data.cuda()
-            value = model.forward(data.obs, mode='compute_critic')['value']
-            next_value = model.forward(data.next_obs, mode='compute_critic')['value']
+            value = model.forward(data.obs.to(dtype=ttorch.float32), mode='compute_critic')['value']
+            next_value = model.forward(data.next_obs.to(dtype=ttorch.float32), mode='compute_critic')['value']
             data.value = value
 
-        traj_flag = data.done.clone()
-        traj_flag[ctx.trajectory_end_idx] = True
-        data.traj_flag = traj_flag
+            traj_flag = data.done.clone()
+            traj_flag[ctx.trajectory_end_idx] = True
+            data.traj_flag = traj_flag
 
-        # done is bool type when acquired from env.step
-        data_ = gae_data(data.value, next_value, data.reward, data.done.float(), traj_flag.float())
-        data.adv = gae(data_, cfg.policy.collect.discount_factor, cfg.policy.collect.gae_lambda)
-        if cfg.policy.get("cuda", False):
-            data = data.cpu()
+            # done is bool type when acquired from env.step
+            data_ = gae_data(data.value, next_value, data.reward, data.done.float(), traj_flag.float())
+            data.adv = gae(data_, cfg.policy.collect.discount_factor, cfg.policy.collect.gae_lambda)
         if buffer_ is None:
             ctx.train_data = data
         else:
+            data = data.cpu()
             data = ttorch.split(data, 1)
             for d in data:
                 buffer_.push(d)
         ctx.trajectories = None
 
     return _gae
```

### Comparing `DI-engine-0.4.7/ding/framework/middleware/functional/collector.py` & `DI-engine-0.4.8/ding/framework/middleware/functional/collector.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,16 +66,17 @@
             - inference_output (:obj:`Dict[int, Dict]`): The dict of which the key is env_id (int), \
                 and the value is inference result (Dict).
         """
 
         if env.closed:
             env.launch()
 
-        obs = ttorch.as_tensor(env.ready_obs).to(dtype=ttorch.float32)
+        obs = ttorch.as_tensor(env.ready_obs)
         ctx.obs = obs
+        obs = obs.to(dtype=ttorch.float32)
         # TODO mask necessary rollout
 
         obs = {i: obs[i] for i in range(get_shape0(obs))}  # TBD
         inference_output = policy.forward(obs, **ctx.collect_kwargs)
         ctx.action = [to_ndarray(v['action']) for v in inference_output.values()]  # TBD
         ctx.inference_output = inference_output
```

### Comparing `DI-engine-0.4.7/ding/framework/middleware/functional/ctx_helper.py` & `DI-engine-0.4.8/ding/framework/middleware/functional/ctx_helper.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/framework/middleware/functional/data_processor.py` & `DI-engine-0.4.8/ding/framework/middleware/functional/data_processor.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/framework/middleware/functional/enhancer.py` & `DI-engine-0.4.8/ding/framework/middleware/functional/enhancer.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/framework/middleware/functional/evaluator.py` & `DI-engine-0.4.8/ding/framework/middleware/functional/evaluator.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/framework/middleware/functional/explorer.py` & `DI-engine-0.4.8/ding/framework/middleware/functional/explorer.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/framework/middleware/functional/logger.py` & `DI-engine-0.4.8/ding/framework/middleware/functional/logger.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,15 @@
         if ctx.train_output is not None and ctx.train_iter - last_train_show_iter >= train_show_freq:
             last_train_show_iter = ctx.train_iter
             if isinstance(ctx.train_output, List):
                 output = ctx.train_output.pop()  # only use latest output
             else:
                 output = ctx.train_output
             for k, v in output.items():
-                if k in ['priority']:
+                if k in ['priority', 'td_error_priority']:
                     continue
                 if "[scalars]" in k:
                     new_k = k.split(']')[-1]
                     raise NotImplementedError
                 elif "[histogram]" in k:
                     new_k = k.split(']')[-1]
                     writer.add_histogram(new_k, v, ctx.env_step)
```

### Comparing `DI-engine-0.4.7/ding/framework/middleware/functional/termination_checker.py` & `DI-engine-0.4.8/ding/framework/middleware/functional/termination_checker.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/framework/middleware/functional/timer.py` & `DI-engine-0.4.8/ding/framework/middleware/functional/timer.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/framework/middleware/functional/trainer.py` & `DI-engine-0.4.8/ding/framework/middleware/functional/trainer.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 from typing import TYPE_CHECKING, Callable, Union
 from easydict import EasyDict
+import treetensor.torch as ttorch
 from ditk import logging
 import numpy as np
 from ding.policy import Policy
 from ding.framework import task, OfflineRLContext, OnlineRLContext
 
 
-def trainer(cfg: EasyDict, policy: Policy) -> Callable:
+def trainer(cfg: EasyDict, policy: Policy, log_freq: int = 100) -> Callable:
     """
     Overview:
         The middleware that executes a single training process.
     Arguments:
         - cfg (:obj:`EasyDict`): Config.
         - policy (:obj:`Policy`): The policy to be trained in step-by-step mode.
+        - log_freq (:obj:`int`): The frequency (iteration) of showing log.
     """
 
     def _train(ctx: Union["OnlineRLContext", "OfflineRLContext"]):
         """
         Input of ctx:
             - train_data (:obj:`Dict`): The data used to update the network. It will train only if \
                 the data is not empty.
@@ -24,17 +26,17 @@
                 it reachs certain values.
         Output of ctx:
             - train_output (:obj:`Dict`): The training output in the Dict format, including loss info.
         """
 
         if ctx.train_data is None:
             return
+        data = ctx.train_data
         train_output = policy.forward(ctx.train_data)
-        #if ctx.train_iter % cfg.policy.learn.learner.hook.log_show_after_iter == 0:
-        if True:
+        if ctx.train_iter % log_freq == 0:
             if isinstance(ctx, OnlineRLContext):
                 logging.info(
                     'Training: Train Iter({})\tEnv Step({})\tLoss({:.3f})'.format(
                         ctx.train_iter, ctx.env_step, train_output['total_loss']
                     )
                 )
             elif isinstance(ctx, OfflineRLContext):
@@ -45,21 +47,21 @@
                 raise TypeError("not supported ctx type: {}".format(type(ctx)))
         ctx.train_iter += 1
         ctx.train_output = train_output
 
     return _train
 
 
-def multistep_trainer(policy: Policy, log_freq: int) -> Callable:
+def multistep_trainer(policy: Policy, log_freq: int = 100) -> Callable:
     """
     Overview:
         The middleware that executes training for a target num of steps.
     Arguments:
         - policy (:obj:`Policy`): The policy specialized for multi-step training.
-        - int (:obj:`int`): The frequency (iteration) of showing log.
+        - log_freq (:obj:`int`): The frequency (iteration) of showing log.
     """
     last_log_iter = -1
 
     def _train(ctx: Union["OnlineRLContext", "OfflineRLContext"]):
         """
         Input of ctx:
             - train_data: The data used to update the network.
@@ -68,15 +70,20 @@
                 The log will be printed if it reachs certain values.
         Output of ctx:
             - train_output (:obj:`List[Dict]`): The training output listed by steps.
         """
 
         if ctx.train_data is None:  # no enough data from data fetcher
             return
-        data = ctx.train_data.to(policy._device)
+        if hasattr(policy, "_device"):  # For ppof policy
+            data = ctx.train_data.to(policy._device)
+        elif hasattr(policy, "get_attribute"):  # For other policy
+            data = ctx.train_data.to(policy.get_attribute("device"))
+        else:
+            assert AttributeError("Policy should have attribution '_device'.")
         train_output = policy.forward(data)
         nonlocal last_log_iter
         if ctx.train_iter - last_log_iter >= log_freq:
             loss = np.mean([o['total_loss'] for o in train_output])
             if isinstance(ctx, OfflineRLContext):
                 logging.info('Training: Train Iter({})\tLoss({:.3f})'.format(ctx.train_iter, loss))
             else:
```

### Comparing `DI-engine-0.4.7/ding/framework/middleware/learner.py` & `DI-engine-0.4.8/ding/framework/middleware/learner.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 
 from ding.framework import task
 from ding.data import Buffer
 from .functional import trainer, offpolicy_data_fetcher, reward_estimator, her_data_enhancer
 
 if TYPE_CHECKING:
     from ding.framework import Context, OnlineRLContext
+    from ding.policy import Policy
+    from ding.reward_model import BaseRewardModel
 
 
 class OffPolicyLearner:
     """
     Overview:
         The class of the off-policy learner, including data fetching and model training. Use \
             the `__call__` method to execute the whole learning process.
@@ -21,25 +23,27 @@
         if task.router.is_active and not task.has_role(task.role.LEARNER):
             return task.void()
         return super(OffPolicyLearner, cls).__new__(cls)
 
     def __init__(
             self,
             cfg: EasyDict,
-            policy,
+            policy: 'Policy',
             buffer_: Union[Buffer, List[Tuple[Buffer, float]], Dict[str, Buffer]],
-            reward_model=None
+            reward_model: Optional['BaseRewardModel'] = None,
+            log_freq: int = 100,
     ) -> None:
         """
         Arguments:
             - cfg (:obj:`EasyDict`): Config.
             - policy (:obj:`Policy`): The policy to be trained.
-            - buffer\_ (:obj:`Buffer`): The replay buffer to store the data for training.
-            - reward_model (:obj:`nn.Module`): Additional reward estimator likes RND, ICM, etc. \
+            - buffer (:obj:`Buffer`): The replay buffer to store the data for training.
+            - reward_model (:obj:`BaseRewardModel`): Additional reward estimator likes RND, ICM, etc. \
                 default to None.
+            - log_freq (:obj:`int`): The frequency (iteration) of showing log.
         """
         self.cfg = cfg
         self._fetcher = task.wrap(offpolicy_data_fetcher(cfg, buffer_))
         self._trainer = task.wrap(trainer(cfg, policy))
         if reward_model is not None:
             self._reward_estimator = task.wrap(reward_estimator(cfg, reward_model))
         else:
```

### Comparing `DI-engine-0.4.7/ding/framework/middleware/tests/mock_for_test.py` & `DI-engine-0.4.8/ding/framework/middleware/tests/mock_for_test.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/framework/middleware/tests/test_advantage_estimator.py` & `DI-engine-0.4.8/ding/framework/middleware/tests/test_advantage_estimator.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/framework/middleware/tests/test_ckpt_handler.py` & `DI-engine-0.4.8/ding/framework/middleware/tests/test_ckpt_handler.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/framework/middleware/tests/test_collector.py` & `DI-engine-0.4.8/ding/framework/middleware/tests/test_collector.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/framework/middleware/tests/test_data_processor.py` & `DI-engine-0.4.8/ding/framework/middleware/tests/test_data_processor.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/framework/middleware/tests/test_distributer.py` & `DI-engine-0.4.8/ding/framework/middleware/tests/test_distributer.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/framework/middleware/tests/test_enhancer.py` & `DI-engine-0.4.8/ding/framework/middleware/tests/test_enhancer.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/framework/middleware/tests/test_evaluator.py` & `DI-engine-0.4.8/ding/framework/middleware/tests/test_evaluator.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/framework/middleware/tests/test_explorer.py` & `DI-engine-0.4.8/ding/framework/middleware/tests/test_explorer.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/framework/middleware/tests/test_logger.py` & `DI-engine-0.4.8/ding/framework/middleware/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/framework/middleware/tests/test_trainer.py` & `DI-engine-0.4.8/ding/framework/middleware/tests/test_trainer.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/framework/middleware_v3/ckpt_handler.py` & `DI-engine-0.4.8/ding/framework/middleware_v3/ckpt_handler.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/framework/middleware_v3/collector.py` & `DI-engine-0.4.8/ding/framework/middleware_v3/collector.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/framework/middleware_v3/functional/__init__.py` & `DI-engine-0.4.8/ding/framework/middleware_v3/functional/__init__.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/framework/middleware_v3/functional/advantage_estimator.py` & `DI-engine-0.4.8/ding/framework/middleware_v3/functional/advantage_estimator.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/framework/middleware_v3/functional/collector.py` & `DI-engine-0.4.8/ding/framework/middleware_v3/functional/collector.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/framework/middleware_v3/functional/ctx_helper.py` & `DI-engine-0.4.8/ding/framework/middleware_v3/functional/ctx_helper.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/framework/middleware_v3/functional/data_processor.py` & `DI-engine-0.4.8/ding/framework/middleware_v3/functional/data_processor.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/framework/middleware_v3/functional/enhancer.py` & `DI-engine-0.4.8/ding/framework/middleware_v3/functional/enhancer.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/framework/middleware_v3/functional/evaluator.py` & `DI-engine-0.4.8/ding/framework/middleware_v3/functional/evaluator.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/framework/middleware_v3/functional/explorer.py` & `DI-engine-0.4.8/ding/framework/middleware_v3/functional/explorer.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/framework/middleware_v3/functional/termination_checker.py` & `DI-engine-0.4.8/ding/framework/middleware_v3/functional/termination_checker.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/framework/middleware_v3/functional/trainer.py` & `DI-engine-0.4.8/ding/framework/middleware_v3/functional/trainer.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/framework/middleware_v3/learner.py` & `DI-engine-0.4.8/ding/framework/middleware_v3/learner.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/framework/middleware_v3/tests/mock_for_test.py` & `DI-engine-0.4.8/ding/framework/middleware_v3/tests/mock_for_test.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/framework/middleware_v3/tests/test_advantage_estimator.py` & `DI-engine-0.4.8/ding/framework/middleware_v3/tests/test_advantage_estimator.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/framework/middleware_v3/tests/test_ckpt_handler.py` & `DI-engine-0.4.8/ding/framework/middleware_v3/tests/test_ckpt_handler.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/framework/middleware_v3/tests/test_collector.py` & `DI-engine-0.4.8/ding/framework/middleware_v3/tests/test_collector.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/framework/middleware_v3/tests/test_data_processor.py` & `DI-engine-0.4.8/ding/framework/middleware_v3/tests/test_data_processor.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/framework/middleware_v3/tests/test_enhancer.py` & `DI-engine-0.4.8/ding/framework/middleware_v3/tests/test_enhancer.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/framework/middleware_v3/tests/test_evaluator.py` & `DI-engine-0.4.8/ding/framework/middleware_v3/tests/test_evaluator.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/framework/middleware_v3/tests/test_explorer.py` & `DI-engine-0.4.8/ding/framework/middleware_v3/tests/test_explorer.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/framework/middleware_v3/tests/test_trainer.py` & `DI-engine-0.4.8/ding/framework/middleware_v3/tests/test_trainer.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/framework/parallel.py` & `DI-engine-0.4.8/ding/framework/parallel.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,17 @@
         self.auto_recover = auto_recover
         self.max_retries = max_retries
         self._mq = MQ_REGISTRY.get(mq_type)(**kwargs)
         time.sleep(self.local_id * self.startup_interval)
         self._listener = Thread(target=self.listen, name="mq_listener", daemon=True)
         self._listener.start()
 
+        self.mq_type = mq_type
+        self.barrier_runtime = Parallel.get_barrier_runtime()(self.node_id)
+
     @classmethod
     def runner(
             cls,
             n_parallel_workers: int,
             mq_type: str = "nng",
             attach_to: Optional[List[str]] = None,
             protocol: str = "ipc",
@@ -368,14 +371,26 @@
             ip = s.getsockname()[0]
         except Exception:
             ip = '127.0.0.1'
         finally:
             s.close()
         return ip
 
+    def get_attch_to_len(self) -> int:
+        """
+        Overview:
+            Get the length of the 'attach_to' list of message queue.
+        Returns:
+            int: the length of the self._mq.attach_to. Returns 0 if self._mq is not initialized
+        """
+        if self._mq:
+            if hasattr(self._mq, 'attach_to'):
+                return len(self._mq.attach_to)
+        return 0
+
     def __enter__(self) -> "Parallel":
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.stop()
 
     def stop(self):
@@ -385,7 +400,13 @@
         if self._mq:
             self._mq.stop()
             self._mq = None
         if self._listener:
             self._listener.join(timeout=1)
             self._listener = None
         self._event_loop.stop()
+
+    @classmethod
+    def get_barrier_runtime(cls):
+        # We get the BarrierRuntime object in the closure to avoid circular import.
+        from ding.framework.middleware.barrier import BarrierRuntime
+        return BarrierRuntime
```

### Comparing `DI-engine-0.4.7/ding/framework/supervisor.py` & `DI-engine-0.4.8/ding/framework/supervisor.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/framework/task.py` & `DI-engine-0.4.8/ding/framework/task.py`

 * *Files 2% similar despite different names*

```diff
@@ -532,9 +532,21 @@
 
     def _activate_async(self):
         if not self._thread_pool:
             self._thread_pool = concurrent.futures.ThreadPoolExecutor(max_workers=self.n_async_workers)
         if not self._async_loop:
             self._async_loop = asyncio.new_event_loop()
 
+    def get_attch_to_len(self) -> int:
+        """
+        Overview:
+            Get the length of the 'attach_to' list in Parallel._mq.
+        Returns:
+            int: the length of the Parallel._mq.
+        """
+        if self.router.is_active:
+            return self.router.get_attch_to_len()
+        else:
+            raise RuntimeError("The router is inactive, failed to be obtained the length of 'attch_to' list.")
+
 
 task = Task()
```

### Comparing `DI-engine-0.4.7/ding/framework/wrapper/step_timer.py` & `DI-engine-0.4.8/ding/framework/wrapper/step_timer.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/hpc_rl/wrapper.py` & `DI-engine-0.4.8/ding/hpc_rl/wrapper.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/interaction/base/app.py` & `DI-engine-0.4.8/ding/interaction/base/app.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/interaction/base/common.py` & `DI-engine-0.4.8/ding/interaction/base/common.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/interaction/base/network.py` & `DI-engine-0.4.8/ding/interaction/base/network.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/interaction/base/threading.py` & `DI-engine-0.4.8/ding/interaction/base/threading.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/interaction/exception/__init__.py` & `DI-engine-0.4.8/ding/interaction/exception/__init__.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/interaction/exception/base.py` & `DI-engine-0.4.8/ding/interaction/exception/base.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/interaction/exception/master.py` & `DI-engine-0.4.8/ding/interaction/exception/master.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/interaction/exception/slave.py` & `DI-engine-0.4.8/ding/interaction/exception/slave.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/interaction/master/connection.py` & `DI-engine-0.4.8/ding/interaction/master/connection.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/interaction/master/master.py` & `DI-engine-0.4.8/ding/interaction/master/master.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/interaction/master/task.py` & `DI-engine-0.4.8/ding/interaction/master/task.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/interaction/slave/action.py` & `DI-engine-0.4.8/ding/interaction/slave/action.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/interaction/slave/slave.py` & `DI-engine-0.4.8/ding/interaction/slave/slave.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/interaction/tests/base/test_app.py` & `DI-engine-0.4.8/ding/interaction/tests/base/test_app.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/interaction/tests/base/test_common.py` & `DI-engine-0.4.8/ding/interaction/tests/base/test_common.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/interaction/tests/base/test_network.py` & `DI-engine-0.4.8/ding/interaction/tests/base/test_network.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/interaction/tests/base/test_threading.py` & `DI-engine-0.4.8/ding/interaction/tests/base/test_threading.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/interaction/tests/exception/test_base.py` & `DI-engine-0.4.8/ding/interaction/tests/exception/test_base.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/interaction/tests/exception/test_master.py` & `DI-engine-0.4.8/ding/interaction/tests/exception/test_master.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/interaction/tests/exception/test_slave.py` & `DI-engine-0.4.8/ding/interaction/tests/exception/test_slave.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/interaction/tests/interaction/bases.py` & `DI-engine-0.4.8/ding/interaction/tests/interaction/bases.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/interaction/tests/interaction/test_errors.py` & `DI-engine-0.4.8/ding/interaction/tests/interaction/test_errors.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/interaction/tests/interaction/test_simple.py` & `DI-engine-0.4.8/ding/interaction/tests/interaction/test_simple.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/interaction/tests/test_utils/stream.py` & `DI-engine-0.4.8/ding/interaction/tests/test_utils/stream.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/league/algorithm.py` & `DI-engine-0.4.8/ding/league/algorithm.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/league/base_league.py` & `DI-engine-0.4.8/ding/league/base_league.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/league/metric.py` & `DI-engine-0.4.8/ding/league/metric.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/league/one_vs_one_league.py` & `DI-engine-0.4.8/ding/league/one_vs_one_league.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/league/player.py` & `DI-engine-0.4.8/ding/league/player.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/league/shared_payoff.py` & `DI-engine-0.4.8/ding/league/shared_payoff.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/league/starcraft_player.py` & `DI-engine-0.4.8/ding/league/starcraft_player.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/model/common/encoder.py` & `DI-engine-0.4.8/ding/model/common/encoder.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/model/common/head.py` & `DI-engine-0.4.8/ding/model/common/head.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import math
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from torch.distributions import Normal, Independent
 
-from ding.torch_utils import fc_block, noise_block, NoiseLinearLayer, MLP, PopArt
+from ding.torch_utils import fc_block, noise_block, NoiseLinearLayer, MLP, PopArt, conv1d_block
 from ding.rl_utils import beta_function_map
 from ding.utils import lists_to_dicts, SequenceType
 
 
 class DiscreteHead(nn.Module):
     """
         Overview:
@@ -1312,14 +1312,87 @@
             >>> torch.Size([4, 3])
             >>> outputs['logit'][2].shape
             >>> torch.Size([4, 5])
         """
         return lists_to_dicts([m(x) for m in self.pred])
 
 
+class EnsembleHead(nn.Module):
+    """
+    Overview:
+        The ``EnsembleHead`` used to output action Q-value for Q-ensemble. \
+        Input is a (:obj:`torch.Tensor`) of shape ''(B, N * ensemble_num, 1)'' and returns a (:obj:`Dict`) containing \
+        output ``pred``.
+    Interfaces:
+        ``__init__``, ``forward``.
+    """
+
+    def __init__(
+            self,
+            input_size: int,
+            output_size: int,
+            hidden_size: int,
+            layer_num: int,
+            ensemble_num: int,
+            activation: Optional[nn.Module] = nn.ReLU(),
+            norm_type: Optional[str] = None
+    ) -> None:
+        super(EnsembleHead, self).__init__()
+        d = input_size
+        layers = []
+        for _ in range(layer_num):
+            layers.append(
+                conv1d_block(
+                    d * ensemble_num,
+                    hidden_size * ensemble_num,
+                    kernel_size=1,
+                    stride=1,
+                    groups=ensemble_num,
+                    activation=activation,
+                    norm_type=norm_type
+                )
+            )
+            d = hidden_size
+
+        # Adding activation for last layer will lead to train fail
+        layers.append(
+            conv1d_block(
+                hidden_size * ensemble_num,
+                output_size * ensemble_num,
+                kernel_size=1,
+                stride=1,
+                groups=ensemble_num,
+                activation=None,
+                norm_type=None
+            )
+        )
+        self.pred = nn.Sequential(*layers)
+
+    def forward(self, x: torch.Tensor) -> Dict:
+        """
+        Overview:
+            Use encoded embedding tensor to run MLP with ``EnsembleHead`` and return the prediction dictionary.
+        Arguments:
+            - x (:obj:`torch.Tensor`): Tensor containing input embedding.
+        Returns:
+            - outputs (:obj:`Dict`): Dict containing keyword ``pred`` (:obj:`torch.Tensor`).
+        Shapes:
+            - x: :math:`(B, N * ensemble_num, 1)`, where ``B = batch_size`` and ``N = hidden_size``.
+            - pred: :math:`(B, M * ensemble_num, 1)`, where ``M = output_size``.
+        Examples:
+            >>> head = EnsembleHead(64 * 10, 64 * 10)
+            >>> inputs = torch.randn(4, 64 * 10, 1) `
+            >>> outputs = head(inputs)
+            >>> assert isinstance(outputs, dict)
+            >>> assert outputs['pred'].shape == torch.Size([10, 64 * 10])
+        """
+        x = self.pred(x).squeeze(-1)
+        return {'pred': x}
+
+
 def independent_normal_dist(logits: Union[List, Dict]) -> torch.distributions.Distribution:
     if isinstance(logits, (list, tuple)):
         return Independent(Normal(*logits), 1)
     elif isinstance(logits, dict):
         return Independent(Normal(logits['mu'], logits['sigma']), 1)
     else:
         raise TypeError("invalid logits type: {}".format(type(logits)))
@@ -1337,8 +1410,9 @@
     'attention_policy': AttentionPolicyHead,
     # continuous
     'regression': RegressionHead,
     'reparameterization': ReparameterizationHead,
     'popart': PopArtVHead,
     # multi
     'multi': MultiHead,
+    'ensemble': EnsembleHead,
 }
```

### Comparing `DI-engine-0.4.7/ding/model/common/utils.py` & `DI-engine-0.4.8/ding/model/common/utils.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/model/template/__init__.py` & `DI-engine-0.4.8/ding/model/template/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,7 +19,8 @@
 from .ngu import NGU
 from .qac_dist import QACDIST
 from .maqac import MAQAC, ContinuousMAQAC
 from .madqn import MADQN
 from .vae import VanillaVAE
 from .decision_transformer import DecisionTransformer
 from .procedure_cloning import ProcedureCloningMCTS, ProcedureCloningBFS
+from .edac import QACEnsemble
```

### Comparing `DI-engine-0.4.7/ding/model/template/acer.py` & `DI-engine-0.4.8/ding/model/template/acer.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/model/template/atoc.py` & `DI-engine-0.4.8/ding/model/template/atoc.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/model/template/bc.py` & `DI-engine-0.4.8/ding/model/template/bc.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/model/template/collaq.py` & `DI-engine-0.4.8/ding/model/template/collaq.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/model/template/coma.py` & `DI-engine-0.4.8/ding/model/template/coma.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/model/template/decision_transformer.py` & `DI-engine-0.4.8/ding/model/template/decision_transformer.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/model/template/ebm.py` & `DI-engine-0.4.8/ding/model/template/ebm.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/model/template/madqn.py` & `DI-engine-0.4.8/ding/model/template/madqn.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/model/template/maqac.py` & `DI-engine-0.4.8/ding/model/template/maqac.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/model/template/mavac.py` & `DI-engine-0.4.8/ding/model/template/mavac.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/model/template/ngu.py` & `DI-engine-0.4.8/ding/model/template/ngu.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/model/template/pdqn.py` & `DI-engine-0.4.8/ding/model/template/pdqn.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/model/template/pg.py` & `DI-engine-0.4.8/ding/model/template/pg.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/model/template/ppg.py` & `DI-engine-0.4.8/ding/model/template/ppg.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/model/template/procedure_cloning.py` & `DI-engine-0.4.8/ding/model/template/procedure_cloning.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/model/template/q_learning.py` & `DI-engine-0.4.8/ding/model/template/q_learning.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/model/template/qac.py` & `DI-engine-0.4.8/ding/model/template/qac.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/model/template/qac_dist.py` & `DI-engine-0.4.8/ding/model/template/qac_dist.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/model/template/qmix.py` & `DI-engine-0.4.8/ding/model/template/qmix.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/model/template/qtran.py` & `DI-engine-0.4.8/ding/model/template/qtran.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/model/template/sqn.py` & `DI-engine-0.4.8/ding/model/template/sqn.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/model/template/vac.py` & `DI-engine-0.4.8/ding/model/template/vac.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/model/template/vae.py` & `DI-engine-0.4.8/ding/model/template/vae.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/model/template/wqmix.py` & `DI-engine-0.4.8/ding/model/template/wqmix.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/model/wrapper/model_wrappers.py` & `DI-engine-0.4.8/ding/model/wrapper/model_wrappers.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/model/wrapper/test_model_wrappers.py` & `DI-engine-0.4.8/ding/model/wrapper/test_model_wrappers.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/policy/__init__.py` & `DI-engine-0.4.8/ding/policy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from .td3_bc import TD3BCPolicy
 
 from .pg import PGPolicy
 from .a2c import A2CPolicy
 from .ppo import PPOPolicy, PPOPGPolicy, PPOOffPolicy
 from .sac import SACPolicy, SACDiscretePolicy, SQILSACPolicy
 from .cql import CQLPolicy, CQLDiscretePolicy
+from .edac import EDACPolicy
 from .impala import IMPALAPolicy
 from .ngu import NGUPolicy
 from .r2d2 import R2D2Policy
 from .r2d2_gtrxl import R2D2GTrXLPolicy
 from .ppg import PPGPolicy, PPGOffPolicy
 from .sqn import SQNPolicy
 from .bdq import BDQPolicy
```

### Comparing `DI-engine-0.4.7/ding/policy/a2c.py` & `DI-engine-0.4.8/ding/policy/a2c.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/policy/acer.py` & `DI-engine-0.4.8/ding/policy/acer.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/policy/atoc.py` & `DI-engine-0.4.8/ding/policy/atoc.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/policy/base_policy.py` & `DI-engine-0.4.8/ding/policy/base_policy.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/policy/bc.py` & `DI-engine-0.4.8/ding/policy/bc.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/policy/bdq.py` & `DI-engine-0.4.8/ding/policy/bdq.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/policy/c51.py` & `DI-engine-0.4.8/ding/policy/c51.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/policy/collaq.py` & `DI-engine-0.4.8/ding/policy/collaq.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/policy/coma.py` & `DI-engine-0.4.8/ding/policy/coma.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/policy/command_mode_policy_instance.py` & `DI-engine-0.4.8/ding/policy/command_mode_policy_instance.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,15 @@
 from .d4pg import D4PGPolicy
 from .cql import CQLPolicy, CQLDiscretePolicy
 from .decision_transformer import DTPolicy
 from .pdqn import PDQNPolicy
 from .sac import SQILSACPolicy
 from .madqn import MADQNPolicy
 from .bdq import BDQPolicy
+from .edac import EDACPolicy
 
 
 class EpsCommandModePolicy(CommandModePolicy):
 
     def _init_command(self) -> None:
         r"""
         Overview:
@@ -377,14 +378,19 @@
 
 
 @POLICY_REGISTRY.register('ibc_command')
 class IBCCommandModePolicy(IBCPolicy, DummyCommandModePolicy):
     pass
 
 
+@POLICY_REGISTRY.register('edac_command')
+class EDACCommandModelPolicy(EDACPolicy, DummyCommandModePolicy):
+    pass
+
+
 @POLICY_REGISTRY.register('bc_command')
 class BCCommandModePolicy(BehaviourCloningPolicy, DummyCommandModePolicy):
 
     def _init_command(self) -> None:
         r"""
         Overview:
             Command mode init method. Called by ``self.__init__``.
```

### Comparing `DI-engine-0.4.7/ding/policy/common_utils.py` & `DI-engine-0.4.8/ding/policy/common_utils.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/policy/cql.py` & `DI-engine-0.4.8/ding/policy/cql.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/policy/d4pg.py` & `DI-engine-0.4.8/ding/policy/d4pg.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/policy/ddpg.py` & `DI-engine-0.4.8/ding/policy/ddpg.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/policy/decision_transformer.py` & `DI-engine-0.4.8/ding/policy/decision_transformer.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/policy/dqfd.py` & `DI-engine-0.4.8/ding/policy/dqfd.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/policy/dqn.py` & `DI-engine-0.4.8/ding/policy/dqn.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/policy/fqf.py` & `DI-engine-0.4.8/ding/policy/fqf.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/policy/ibc.py` & `DI-engine-0.4.8/ding/policy/ibc.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/policy/il.py` & `DI-engine-0.4.8/ding/policy/il.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/policy/impala.py` & `DI-engine-0.4.8/ding/policy/impala.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/policy/iqn.py` & `DI-engine-0.4.8/ding/policy/iqn.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/policy/madqn.py` & `DI-engine-0.4.8/ding/policy/madqn.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/policy/mbpolicy/mbsac.py` & `DI-engine-0.4.8/ding/policy/mbpolicy/mbsac.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/policy/mbpolicy/utils.py` & `DI-engine-0.4.8/ding/policy/mbpolicy/utils.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/policy/mdqn.py` & `DI-engine-0.4.8/ding/policy/mdqn.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/policy/ngu.py` & `DI-engine-0.4.8/ding/policy/ngu.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/policy/offppo_collect_traj.py` & `DI-engine-0.4.8/ding/policy/offppo_collect_traj.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/policy/pc.py` & `DI-engine-0.4.8/ding/policy/pc.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/policy/pdqn.py` & `DI-engine-0.4.8/ding/policy/pdqn.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/policy/pg.py` & `DI-engine-0.4.8/ding/policy/pg.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/policy/policy_factory.py` & `DI-engine-0.4.8/ding/policy/policy_factory.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/policy/ppg.py` & `DI-engine-0.4.8/ding/policy/ppg.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/policy/ppo.py` & `DI-engine-0.4.8/ding/policy/ppo.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import List, Dict, Any, Tuple, Union
 from collections import namedtuple
 import torch
 import copy
 import numpy as np
 
-from ding.torch_utils import Adam, to_device, unsqueeze, ContrastiveLoss
+from ding.torch_utils import Adam, to_device, to_dtype, unsqueeze, ContrastiveLoss
 from ding.rl_utils import ppo_data, ppo_error, ppo_policy_error, ppo_policy_data, get_gae_with_default_last_value, \
     v_nstep_td_data, v_nstep_td_error, get_nstep_return_data, get_train_sample, gae, gae_data, ppo_error_continuous, \
     get_gae, ppo_policy_error_continuous
 from ding.model import model_wrap
 from ding.utils import POLICY_REGISTRY, split_data_generator, RunningMeanStd
 from ding.utils.data import default_collate, default_decollate
 from .base_policy import Policy
@@ -153,14 +153,17 @@
             - info_dict (:obj:`Dict[str, Any]`):
               Including current lr, total_loss, policy_loss, value_loss, entropy_loss, \
                         adv_abs_max, approx_kl, clipfrac
         """
         data = default_preprocess_learn(data, ignore_done=self._cfg.learn.ignore_done, use_nstep=False)
         if self._cuda:
             data = to_device(data, self._device)
+        data['obs'] = to_dtype(data['obs'], torch.float32)
+        if 'next_obs' in data:
+            data['next_obs'] = to_dtype(data['next_obs'], torch.float32)
         # ====================
         # PPO forward
         # ====================
         return_infos = []
         self._learn_model.train()
 
         for epoch in range(self._cfg.learn.epoch_per_collect):
```

### Comparing `DI-engine-0.4.7/ding/policy/ppof.py` & `DI-engine-0.4.8/ding/policy/ppof.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         batch_size=64,
         learning_rate=3e-4,
         weight_decay=0,
         value_weight=0.5,
         entropy_weight=0.01,
         clip_ratio=0.2,
         adv_norm=True,
-        value_norm='symlog',
+        value_norm='baseline',
         ppo_param_init=True,
         grad_norm=0.5,
         # collect
         n_sample=128,
         unroll_len=1,
         # eval
         deterministic_eval=True,
@@ -150,16 +150,17 @@
             with torch.no_grad():
                 # get the value dictionary
                 # In popart, the dictionary has two keys: 'pred' and 'unnormalized_pred'
                 value = self._model.compute_critic(data.obs)
                 next_value = self._model.compute_critic(data.next_obs)
                 reward = data.reward
 
-                assert self._cfg.value_norm in ['popart', 'value_rescale', 'symlog'],\
-                    'Not supported value normalization! Value normalization supported: popart, value rescale, symlog'
+                assert self._cfg.value_norm in ['popart', 'value_rescale', 'symlog', 'baseline'],\
+                    'Not supported value normalization! Value normalization supported: \
+                        popart, value rescale, symlog, baseline'
 
                 if self._cfg.value_norm == 'popart':
                     unnormalized_value = value['unnormalized_pred']
                     unnormalized_next_value = value['unnormalized_pred']
 
                     mu = self._model.critic_head.popart.mu
                     sigma = self._model.critic_head.popart.sigma
@@ -169,14 +170,17 @@
                     next_value = next_value['pred']
                 elif self._cfg.value_norm == 'value_rescale':
                     value = value_inv_transform(value['pred'])
                     next_value = value_inv_transform(next_value['pred'])
                 elif self._cfg.value_norm == 'symlog':
                     value = inv_symlog(value['pred'])
                     next_value = inv_symlog(next_value['pred'])
+                elif self._cfg.value_norm == 'baseline':
+                    value = value['pred'] * self._running_mean_std.std
+                    next_value = next_value['pred'] * self._running_mean_std.std
 
                 traj_flag = data.get('traj_flag', None)  # traj_flag indicates termination of trajectory
                 adv_data = gae_data(value, next_value, reward, data.done, traj_flag)
                 data.adv = gae(adv_data, self._cfg.discount_factor, self._cfg.gae_lambda)
 
                 unnormalized_returns = value + data.adv  # In popart, this return is normalized
 
@@ -184,14 +188,18 @@
                     self._model.critic_head.popart.update_parameters((data.reward).unsqueeze(1))
                 elif self._cfg.value_norm == 'value_rescale':
                     value = value_transform(value)
                     unnormalized_returns = value_transform(unnormalized_returns)
                 elif self._cfg.value_norm == 'symlog':
                     value = symlog(value)
                     unnormalized_returns = symlog(unnormalized_returns)
+                elif self._cfg.value_norm == 'baseline':
+                    value /= self._running_mean_std.std
+                    unnormalized_returns /= self._running_mean_std.std
+                    self._running_mean_std.update(unnormalized_returns.cpu().numpy())
                 data.value = value
                 data.return_ = unnormalized_returns
 
             # inner training loop
             split_data = ttorch.split(data, self._cfg.batch_size)
             random.shuffle(list(split_data))
             for batch in split_data:
```

### Comparing `DI-engine-0.4.7/ding/policy/qmix.py` & `DI-engine-0.4.8/ding/policy/qmix.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/policy/qrdqn.py` & `DI-engine-0.4.8/ding/policy/qrdqn.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/policy/qtran.py` & `DI-engine-0.4.8/ding/policy/qtran.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/policy/r2d2.py` & `DI-engine-0.4.8/ding/policy/r2d2.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/policy/r2d2_collect_traj.py` & `DI-engine-0.4.8/ding/policy/r2d2_collect_traj.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/policy/r2d2_gtrxl.py` & `DI-engine-0.4.8/ding/policy/r2d2_gtrxl.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/policy/r2d3.py` & `DI-engine-0.4.8/ding/policy/r2d3.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/policy/rainbow.py` & `DI-engine-0.4.8/ding/policy/rainbow.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/policy/sac.py` & `DI-engine-0.4.8/ding/policy/sac.py`

 * *Files 1% similar despite different names*

```diff
@@ -313,14 +313,17 @@
                 self._alpha.data = torch.where(self._alpha > 0, self._alpha,
                                                torch.zeros_like(self._alpha)).requires_grad_()
         loss_dict['total_loss'] = sum(loss_dict.values())
 
         # target update
         self._target_model.update(self._learn_model.state_dict())
         return {
+            'total_loss': loss_dict['total_loss'].item(),
+            'policy_loss': loss_dict['policy_loss'].item(),
+            'critic_loss': loss_dict['critic_loss'].item(),
             'cur_lr_q': self._optimizer_q.defaults['lr'],
             'cur_lr_p': self._optimizer_policy.defaults['lr'],
             'priority': td_error_per_sample.abs().tolist(),
             'td_error': td_error_per_sample.detach().mean().item(),
             'alpha': self._alpha.item(),
             'q_value_1': target_q_value[0].detach().mean().item(),
             'q_value_2': target_q_value[1].detach().mean().item(),
```

### Comparing `DI-engine-0.4.7/ding/policy/sql.py` & `DI-engine-0.4.8/ding/policy/sql.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/policy/sqn.py` & `DI-engine-0.4.8/ding/policy/sqn.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/policy/td3.py` & `DI-engine-0.4.8/ding/policy/td3.py`

 * *Files 0% similar despite different names*

```diff
@@ -152,8 +152,8 @@
                 # (int) Maximum size of replay buffer.
                 replay_buffer_size=100000,
             ),
         ),
     )
 
     def monitor_vars(self) -> List[str]:
-        return ["q_value", "target q_value", "loss", "lr", "entropy", "target_q_value", "td_error"]
+        return ["q_value", "loss", "lr", "entropy", "target_q_value", "td_error"]
```

### Comparing `DI-engine-0.4.7/ding/policy/td3_bc.py` & `DI-engine-0.4.8/ding/policy/td3_bc.py`

 * *Files 1% similar despite different names*

```diff
@@ -194,14 +194,17 @@
         self._optimizer_critic = Adam(
             self._model.critic.parameters(),
             lr=self._cfg.learn.learning_rate_critic,
             grad_clip_type='clip_norm',
             clip_value=1.0,
         )
 
+        self.noise_sigma = self._cfg.learn.noise_sigma
+        self.noise_range = self._cfg.learn.noise_range
+
     def _forward_learn(self, data: dict) -> Dict[str, Any]:
         r"""
         Overview:
             Forward and backward function of learn mode.
         Arguments:
             - data (:obj:`dict`): Dict type data, including at least ['obs', 'action', 'reward', 'next_obs']
         Returns:
@@ -233,14 +236,17 @@
             q_value_dict['q_value'] = q_value[0].mean()
             q_value_dict['q_value_twin'] = q_value[1].mean()
         else:
             q_value_dict['q_value'] = q_value.mean()
         # target q value.
         with torch.no_grad():
             next_action = self._target_model.forward(next_obs, mode='compute_actor')['action']
+            noise = (torch.randn_like(next_action) *
+                     self.noise_sigma).clamp(self.noise_range['min'], self.noise_range['max'])
+            next_action = (next_action + noise).clamp(-1, 1)
             next_data = {'obs': next_obs, 'action': next_action}
             target_q_value = self._target_model.forward(next_data, mode='compute_critic')['q_value']
         if self._twin_critic:
             # TD3: two critic networks
             target_q_value = torch.min(target_q_value[0], target_q_value[1])  # find min one as target q value
             # critic network1
             td_data = v_1step_td_data(q_value[0], target_q_value, reward, data['done'], data['weight'])
```

### Comparing `DI-engine-0.4.7/ding/policy/td3_vae.py` & `DI-engine-0.4.8/ding/policy/td3_vae.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/policy/wqmix.py` & `DI-engine-0.4.8/ding/policy/wqmix.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/reward_model/__init__.py` & `DI-engine-0.4.8/ding/reward_model/__init__.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/reward_model/base_reward_model.py` & `DI-engine-0.4.8/ding/reward_model/base_reward_model.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/reward_model/drex_reward_model.py` & `DI-engine-0.4.8/ding/reward_model/drex_reward_model.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/reward_model/gail_irl_model.py` & `DI-engine-0.4.8/ding/reward_model/gail_irl_model.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/reward_model/guided_cost_reward_model.py` & `DI-engine-0.4.8/ding/reward_model/guided_cost_reward_model.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/reward_model/her_reward_model.py` & `DI-engine-0.4.8/ding/reward_model/her_reward_model.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/reward_model/icm_reward_model.py` & `DI-engine-0.4.8/ding/reward_model/icm_reward_model.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/reward_model/ngu_reward_model.py` & `DI-engine-0.4.8/ding/reward_model/ngu_reward_model.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/reward_model/pdeil_irl_model.py` & `DI-engine-0.4.8/ding/reward_model/pdeil_irl_model.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/reward_model/pwil_irl_model.py` & `DI-engine-0.4.8/ding/reward_model/pwil_irl_model.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/reward_model/red_irl_model.py` & `DI-engine-0.4.8/ding/reward_model/red_irl_model.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/reward_model/rnd_reward_model.py` & `DI-engine-0.4.8/ding/reward_model/rnd_reward_model.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/reward_model/trex_reward_model.py` & `DI-engine-0.4.8/ding/reward_model/trex_reward_model.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/rl_utils/__init__.py` & `DI-engine-0.4.8/ding/rl_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/rl_utils/a2c.py` & `DI-engine-0.4.8/ding/rl_utils/a2c.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/rl_utils/acer.py` & `DI-engine-0.4.8/ding/rl_utils/acer.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/rl_utils/adder.py` & `DI-engine-0.4.8/ding/rl_utils/adder.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/rl_utils/beta_function.py` & `DI-engine-0.4.8/ding/rl_utils/beta_function.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/rl_utils/coma.py` & `DI-engine-0.4.8/ding/rl_utils/coma.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/rl_utils/exploration.py` & `DI-engine-0.4.8/ding/rl_utils/exploration.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/rl_utils/gae.py` & `DI-engine-0.4.8/ding/rl_utils/gae.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/rl_utils/isw.py` & `DI-engine-0.4.8/ding/rl_utils/isw.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/rl_utils/ppg.py` & `DI-engine-0.4.8/ding/rl_utils/ppg.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/rl_utils/ppo.py` & `DI-engine-0.4.8/ding/rl_utils/ppo.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/rl_utils/retrace.py` & `DI-engine-0.4.8/ding/rl_utils/retrace.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/rl_utils/sampler.py` & `DI-engine-0.4.8/ding/rl_utils/sampler.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/rl_utils/td.py` & `DI-engine-0.4.8/ding/rl_utils/td.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/rl_utils/upgo.py` & `DI-engine-0.4.8/ding/rl_utils/upgo.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/rl_utils/value_rescale.py` & `DI-engine-0.4.8/ding/rl_utils/value_rescale.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/rl_utils/vtrace.py` & `DI-engine-0.4.8/ding/rl_utils/vtrace.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/torch_utils/__init__.py` & `DI-engine-0.4.8/ding/torch_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/torch_utils/checkpoint_helper.py` & `DI-engine-0.4.8/ding/torch_utils/checkpoint_helper.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/torch_utils/data_helper.py` & `DI-engine-0.4.8/ding/torch_utils/data_helper.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 from threading import Thread
 from queue import Queue
 
 import numpy as np
 import torch
 import treetensor.torch as ttorch
 
+from ding.utils.default_helper import get_shape0
+
 
 def to_device(item: Any, device: str, ignore_keys: list = []) -> Any:
     """
     Overview:
         Transfer data to certain device
     Arguments:
         - item (:obj:`Any`): the item to be transferred
@@ -276,35 +278,46 @@
         return {k: tensor_to_list(v) for k, v in item.items()}
     elif np.isscalar(item):
         return item
     else:
         raise TypeError("not support item type: {}".format(type(item)))
 
 
-def to_item(data):
+def to_item(data: Any, ignore_error: bool = True) -> Any:
     """
     Overview:
         Transform data into python native scalar (i.e. data item), keep other data types unchanged.
     Arguments:
         - data (:obj:`Any`): The data that needs to be transformed.
+        - ignore_error (:obj:`bool`): Whether to ignore the error when the data type is not supported. That is to \
+            say, only the data can be transformed into a python native scalar will be returned.
     Returns:
         - data (:obj:`Any`): Transformed data.
     """
     if data is None:
         return data
     elif isinstance(data, bool) or isinstance(data, str):
         return data
     elif np.isscalar(data):
         return data
     elif isinstance(data, np.ndarray) or isinstance(data, torch.Tensor) or isinstance(data, ttorch.Tensor):
         return data.item()
     elif isinstance(data, list) or isinstance(data, tuple):
         return [to_item(d) for d in data]
     elif isinstance(data, dict):
-        return {k: to_item(v) for k, v in data.items()}
+        new_data = {}
+        for k, v in data.items():
+            if ignore_error:
+                try:
+                    new_data[k] = to_item(v)
+                except ValueError:
+                    pass
+            else:
+                new_data[k] = to_item(v)
+        return new_data
     else:
         raise TypeError("not support data type: {}".format(data))
 
 
 def same_shape(data: list) -> bool:
     r"""
     Overview:
@@ -441,24 +454,7 @@
     for _ in range(num):
         data = copy.deepcopy(template)
         data['null'] = True
         data['done'] = True
         data['reward'].zero_()
         ret.append(data)
     return ret
-
-
-def get_shape0(data):
-    if isinstance(data, torch.Tensor):
-        return data.shape[0]
-    elif isinstance(data, ttorch.Tensor):
-
-        def fn(t):
-            item = list(t.values())[0]
-            if np.isscalar(item[0]):
-                return item[0]
-            else:
-                return fn(item)
-
-        return fn(data.shape)
-    else:
-        raise TypeError("not support type: {}".format(data))
```

### Comparing `DI-engine-0.4.7/ding/torch_utils/distribution.py` & `DI-engine-0.4.8/ding/torch_utils/distribution.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/torch_utils/loss/contrastive_loss.py` & `DI-engine-0.4.8/ding/torch_utils/loss/contrastive_loss.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/torch_utils/loss/cross_entropy_loss.py` & `DI-engine-0.4.8/ding/torch_utils/loss/cross_entropy_loss.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/torch_utils/loss/multi_logits_loss.py` & `DI-engine-0.4.8/ding/torch_utils/loss/multi_logits_loss.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/torch_utils/lr_scheduler.py` & `DI-engine-0.4.8/ding/torch_utils/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/torch_utils/math_helper.py` & `DI-engine-0.4.8/ding/torch_utils/math_helper.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/torch_utils/metric.py` & `DI-engine-0.4.8/ding/torch_utils/metric.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/torch_utils/network/__init__.py` & `DI-engine-0.4.8/ding/torch_utils/network/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from .activation import build_activation, Swish
 from .res_block import ResBlock, ResFCBlock
 from .nn_module import fc_block, conv2d_block, one_hot, deconv2d_block, BilinearUpsample, NearestUpsample, \
-    binary_encode, NoiseLinearLayer, noise_block, MLP, Flatten, normed_linear, normed_conv2d
+    binary_encode, NoiseLinearLayer, noise_block, MLP, Flatten, normed_linear, normed_conv2d, conv1d_block
 from .normalization import build_normalization
 from .rnn import get_lstm, sequence_mask
 from .soft_argmax import SoftArgmax
 from .transformer import Transformer, ScaledDotProductAttention
 from .scatter_connection import ScatterConnection
 from .resnet import resnet18, ResNet
 from .gumbel_softmax import GumbelSoftmax
```

### Comparing `DI-engine-0.4.7/ding/torch_utils/network/activation.py` & `DI-engine-0.4.8/ding/torch_utils/network/activation.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/torch_utils/network/coverage.xml` & `DI-engine-0.4.8/ding/torch_utils/network/coverage.xml`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/torch_utils/network/gtrxl.py` & `DI-engine-0.4.8/ding/torch_utils/network/gtrxl.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/torch_utils/network/gumbel_softmax.py` & `DI-engine-0.4.8/ding/torch_utils/network/gumbel_softmax.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/torch_utils/network/nn_module.py` & `DI-engine-0.4.8/ding/torch_utils/network/nn_module.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,15 +86,15 @@
         - stride (:obj:`int`): Stride of the convolution
         - padding (:obj:`int`): Zero-padding added to both sides of the input
         - dilation (:obj:`int`): Spacing between kernel elements
         - groups (:obj:`int`): Number of blocked connections from input channels to output channels
         - activation (:obj:`nn.Module`): the optional activation function
         - norm_type (:obj:`str`): type of the normalization
     Returns:
-        - block (:obj:`nn.Sequential`): a sequential list containing the torch layers of the 1 dim convlution layer
+        - block (:obj:`nn.Sequential`): a sequential list containing the torch layers of the 1 dim convolution layer
 
     .. note::
 
         Conv1d (https://pytorch.org/docs/stable/generated/torch.nn.Conv1d.html#torch.nn.Conv1d)
     """
     block = []
     block.append(nn.Conv1d(in_channels, out_channels, kernel_size, stride, padding, dilation, groups))
@@ -112,31 +112,34 @@
         stride: int = 1,
         padding: int = 0,
         dilation: int = 1,
         groups: int = 1,
         pad_type: str = 'zero',
         activation: nn.Module = None,
         norm_type: str = None,
+        num_groups_for_gn: int = 1,
         bias: bool = True
 ) -> nn.Sequential:
     r"""
     Overview:
         Create a 2-dim convolution layer with activation and normalization.
     Arguments:
-        - in_channels (:obj:`int`): Number of channels in the input tensor
-        - out_channels (:obj:`int`): Number of channels in the output tensor
-        - kernel_size (:obj:`int`): Size of the convolving kernel
-        - stride (:obj:`int`): Stride of the convolution
-        - padding (:obj:`int`): Zero-padding added to both sides of the input
-        - dilation (:obj:`int`): Spacing between kernel elements
-        - groups (:obj:`int`): Number of blocked connections from input channels to output channels
-        - pad_type (:obj:`str`): the way to add padding, include ['zero', 'reflect', 'replicate'], default: None
-        - activation (:obj:`nn.Module`): the optional activation function
-        - norm_type (:obj:`str`): type of the normalization, default set to None, now support ['BN', 'IN', 'SyncBN']
-        - bias (:obj:`bool`): whether adds a learnable bias to the nn.Conv2d. default set to True
+        - in_channels (:obj:`int`): Number of channels in the input tensor.
+        - out_channels (:obj:`int`): Number of channels in the output tensor.
+        - kernel_size (:obj:`int`): Size of the convolving kernel.
+        - stride (:obj:`int`): Stride of the convolution.
+        - padding (:obj:`int`): Zero-padding added to both sides of the input.
+        - dilation (:obj:`int`): Spacing between kernel elements.
+        - groups (:obj:`int`): Number of blocked connections from input channels to output channels.
+        - pad_type (:obj:`str`): the way to add padding, include ['zero', 'reflect', 'replicate'], default: None.
+        - activation (:obj:`nn.Module`): the optional activation function.
+        - norm_type (:obj:`str`): The type of the normalization, now support ['BN', 'LN', 'IN', 'GN', 'SyncBN'],
+            default set to None, which means no normalization.
+        - num_groups_for_gn (:obj:`int`): Number of groups for GroupNorm.
+        - bias (:obj:`bool`): whether adds a learnable bias to the nn.Conv2d. Default set to True.
     Returns:
         - block (:obj:`nn.Sequential`): a sequential list containing the torch layers of the 2 dim convlution layer
 
     .. note::
 
         Conv2d (https://pytorch.org/docs/stable/generated/torch.nn.Conv2d.html#torch.nn.Conv2d)
     """
@@ -159,15 +162,27 @@
             padding=padding,
             dilation=dilation,
             groups=groups,
             bias=bias
         )
     )
     if norm_type is not None:
-        block.append(build_normalization(norm_type, dim=2)(out_channels))
+        if norm_type == 'LN':
+            # LN is implemented as GroupNorm with 1 group.
+            block.append(nn.GroupNorm(1, out_channels))
+        elif norm_type == 'GN':
+            block.append(nn.GroupNorm(num_groups_for_gn, out_channels))
+        elif norm_type in ['BN', 'IN', 'SyncBN']:
+            block.append(build_normalization(norm_type, dim=2)(out_channels))
+        else:
+            raise KeyError(
+                "Invalid value in norm_type: {}. The valid norm_type are "
+                "BN, LN, IN, GN and SyncBN.".format(norm_type)
+            )
+
     if activation is not None:
         block.append(activation)
     return sequential_pack(block)
 
 
 def deconv2d_block(
         in_channels: int,
@@ -178,27 +193,27 @@
         output_padding: int = 0,
         groups: int = 1,
         activation: int = None,
         norm_type: int = None
 ) -> nn.Sequential:
     r"""
     Overview:
-        Create a 2-dim transopse convlution layer with activation and normalization
+        Create a 2-dim transpose convolution layer with activation and normalization
     Arguments:
         - in_channels (:obj:`int`): Number of channels in the input tensor
         - out_channels (:obj:`int`): Number of channels in the output tensor
         - kernel_size (:obj:`int`): Size of the convolving kernel
         - stride (:obj:`int`): Stride of the convolution
         - padding (:obj:`int`): Zero-padding added to both sides of the input
         - pad_type (:obj:`str`): the way to add padding, include ['zero', 'reflect', 'replicate']
         - activation (:obj:`nn.Module`): the optional activation function
         - norm_type (:obj:`str`): type of the normalization
     Returns:
         - block (:obj:`nn.Sequential`): a sequential list containing the torch layers of the 2-dim \
-            transpose convlution layer
+            transpose convolution layer
 
     .. note::
 
         ConvTranspose2d (https://pytorch.org/docs/master/generated/torch.nn.ConvTranspose2d.html)
     """
     block = []
     block.append(
@@ -310,37 +325,40 @@
     out_channels: int,
     layer_num: int,
     layer_fn: Callable = None,
     activation: nn.Module = None,
     norm_type: str = None,
     use_dropout: bool = False,
     dropout_probability: float = 0.5,
-    output_activation: nn.Module = None,
-    output_norm_type: str = None,
+    output_activation: bool = True,
+    output_norm: bool = True,
     last_linear_layer_init_zero: bool = False
 ):
     r"""
     Overview:
         create a multi-layer perceptron using fully-connected blocks with activation, normalization and dropout,
         optional normalization can be done to the dim 1 (across the channels).
         x -> fc -> norm -> act -> dropout -> out
     Arguments:
         - in_channels (:obj:`int`): Number of channels in the input tensor.
         - hidden_channels (:obj:`int`): Number of channels in the hidden tensor.
         - out_channels (:obj:`int`): Number of channels in the output tensor.
         - layer_num (:obj:`int`): Number of layers.
-        - layer_fn (:obj:`Callable`): layer function.
-        - activation (:obj:`nn.Module`): the optional activation function.
-        - norm_type (:obj:`str`): type of the normalization.
-        - use_dropout (:obj:`bool`): whether to use dropout in the fully-connected block.
-        - dropout_probability (:obj:`float`): probability of an element to be zeroed in the dropout. Default: 0.5.
-        - output_activation (:obj:`nn.Module`): the optional activation function in the last layer.
-        - output_norm_type (:obj:`str`): type of the normalization in the last layer.
-        - last_linear_layer_init_zero (:obj:`bool`): zero initialization for the last linear layer (including w and b),
-            which can provide stable zero outputs in the beginning.
+        - layer_fn (:obj:`Callable`): Layer function.
+        - activation (:obj:`nn.Module`): The optional activation function.
+        - norm_type (:obj:`str`): The type of the normalization.
+        - use_dropout (:obj:`bool`): Whether to use dropout in the fully-connected block.
+        - dropout_probability (:obj:`float`): The probability of an element to be zeroed in the dropout. Default: 0.5.
+        - output_activation (:obj:`bool`): Whether to use activation in the output layer. If True,
+            we use the same activation as front layers. Default: True.
+        - output_norm (:obj:`bool`): Whether to use normalization in the output layer. If True,
+            we use the same normalization as front layers. Default: True.
+        - last_linear_layer_init_zero (:obj:`bool`): Whether to use zero initializations for the last linear layer
+            (including w and b), which can provide stable zero outputs in the beginning,
+            usually used in the policy network in RL settings.
     Returns:
         - block (:obj:`nn.Sequential`): a sequential list containing the torch layers of the fully-connected block.
 
     .. note::
 
         you can refer to nn.linear (https://pytorch.org/docs/master/generated/torch.nn.Linear.html).
     """
@@ -357,38 +375,39 @@
         if norm_type is not None:
             block.append(build_normalization(norm_type, dim=1)(out_channels))
         if activation is not None:
             block.append(activation)
         if use_dropout:
             block.append(nn.Dropout(dropout_probability))
 
-    # the last layer
+    # The last layer
     in_channels = channels[-2]
     out_channels = channels[-1]
-    if output_activation is None and output_norm_type is None:
-        #  the last layer use the same norm and activation as front layers
-        block.append(layer_fn(in_channels, out_channels))
+    block.append(layer_fn(in_channels, out_channels))
+    """
+    In the final layer of a neural network, whether to use normalization and activation are typically determined
+    based on user specifications. These specifications depend on the problem at hand and the desired properties of
+    the model's output.
+    """
+    if output_norm is True:
+        # The last layer uses the same norm as front layers.
         if norm_type is not None:
             block.append(build_normalization(norm_type, dim=1)(out_channels))
+    if output_activation is True:
+        # The last layer uses the same activation as front layers.
         if activation is not None:
             block.append(activation)
-        if use_dropout:
-            block.append(nn.Dropout(dropout_probability))
-    else:
-        #  the last layer use the specific norm and activation
-        block.append(layer_fn(in_channels, out_channels))
-        if output_norm_type is not None:
-            block.append(build_normalization(output_norm_type, dim=1)(out_channels))
-        if output_activation is not None:
-            block.append(output_activation)
-        if use_dropout:
-            block.append(nn.Dropout(dropout_probability))
-        if last_linear_layer_init_zero:
-            block[-2].weight.data.fill_(0)
-            block[-2].bias.data.fill_(0)
+
+    if last_linear_layer_init_zero:
+        # Locate the last linear layer and initialize its weights and biases to 0.
+        for _, layer in enumerate(reversed(block)):
+            if isinstance(layer, nn.Linear):
+                nn.init.zeros_(layer.weight)
+                nn.init.zeros_(layer.bias)
+                break
 
     return sequential_pack(block)
 
 
 class ChannelShuffle(nn.Module):
     r"""
     Overview:
@@ -478,15 +497,15 @@
     else:
         return ret.reshape(*old_shape, num)
 
 
 class NearestUpsample(nn.Module):
     r"""
     Overview:
-        Upsamples the input to the given member varible scale_factor using mode nearest
+        Upsamples the input to the given member variable scale_factor using mode nearest
     Interface:
         forward
     """
 
     def __init__(self, scale_factor: Union[float, List[float]]) -> None:
         r"""
         Overview:
@@ -508,15 +527,15 @@
         """
         return F.interpolate(x, scale_factor=self.scale_factor, mode='nearest')
 
 
 class BilinearUpsample(nn.Module):
     r"""
     Overview:
-        Upsamples the input to the given member varible scale_factor using mode biliner
+        Upsamples the input to the given member variable scale_factor using mode bilinear
     Interface:
         forward
     """
 
     def __init__(self, scale_factor: Union[float, List[float]]) -> None:
         r"""
         Overview:
@@ -593,15 +612,15 @@
         x = torch.randn(size)
         x = x.sign().mul(x.abs().sqrt())
         return x
 
     def reset_noise(self):
         r"""
         Overview:
-            Reset noise settinngs in the layer.
+            Reset noise settings in the layer.
         """
         is_cuda = self.weight_mu.is_cuda
         in_noise = self._scale_noise(self.in_channels).to(torch.device("cuda" if is_cuda else "cpu"))
         out_noise = self._scale_noise(self.out_channels).to(torch.device("cuda" if is_cuda else "cpu"))
         self.weight_eps = out_noise.ger(in_noise)
         self.bias_eps = out_noise
 
@@ -655,15 +674,15 @@
     Arguments:
         - in_channels (:obj:`int`): Number of channels in the input tensor
         - out_channels (:obj:`int`): Number of channels in the output tensor
         - activation (:obj:`str`): the optional activation function
         - norm_type (:obj:`str`): type of the normalization
         - use_dropout (:obj:`bool`) : whether to use dropout in the fully-connected block
         - dropout_probability (:obj:`float`) : probability of an element to be zeroed in the dropout. Default: 0.5
-        - simga0 (:obj:`float`): the sigma0 is the defalut noise volumn when init NoiseLinearLayer
+        - simga0 (:obj:`float`): the sigma0 is the default noise volume when init NoiseLinearLayer
     Returns:
         - block (:obj:`nn.Sequential`): a sequential list containing the torch layers of the fully-connected block
 
     .. note::
 
         you can refer to nn.linear (https://pytorch.org/docs/master/generated/torch.nn.Linear.html)
     """
```

### Comparing `DI-engine-0.4.7/ding/torch_utils/network/normalization.py` & `DI-engine-0.4.8/ding/torch_utils/network/normalization.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,34 +3,36 @@
 
 
 def build_normalization(norm_type: str, dim: Optional[int] = None) -> nn.Module:
     r"""
     Overview:
         Build the corresponding normalization module
     Arguments:
-        - norm_type (:obj:`str`): type of the normaliztion, now support ['BN', 'IN', 'SyncBN', 'AdaptiveIN']
+        - norm_type (:obj:`str`): type of the normaliztion, now support ['BN', 'LN', 'IN', 'SyncBN']
         - dim (:obj:`int`): dimension of the normalization, when norm_type is in [BN, IN]
     Returns:
         - norm_func (:obj:`nn.Module`): the corresponding batch normalization function
 
     .. note::
         For beginers, you can refer to <https://zhuanlan.zhihu.com/p/34879333> to learn more about batch normalization.
     """
     if dim is None:
         key = norm_type
     else:
-        if norm_type in ['BN', 'IN', 'SyncBN']:
+        if norm_type in ['BN', 'IN']:
             key = norm_type + str(dim)
-        elif norm_type in ['LN']:
+        elif norm_type in ['LN', 'SyncBN']:
             key = norm_type
         else:
             raise NotImplementedError("not support indicated dim when creates {}".format(norm_type))
     norm_func = {
         'BN1': nn.BatchNorm1d,
         'BN2': nn.BatchNorm2d,
         'LN': nn.LayerNorm,
+        'IN1': nn.InstanceNorm1d,
         'IN2': nn.InstanceNorm2d,
+        'SyncBN': nn.SyncBatchNorm,
     }
     if key in norm_func.keys():
         return norm_func[key]
     else:
         raise KeyError("invalid norm type: {}".format(key))
```

### Comparing `DI-engine-0.4.7/ding/torch_utils/network/popart.py` & `DI-engine-0.4.8/ding/torch_utils/network/popart.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/torch_utils/network/res_block.py` & `DI-engine-0.4.8/ding/torch_utils/network/res_block.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         """
         Overview:
             Init the 2D convolution residual block.
         Arguments:
             - in_channels (:obj:`int`): Number of channels in the input tensor.
             - activation (:obj:`nn.Module`): the optional activation function.
             - norm_type (:obj:`str`): type of the normalization, default set to 'BN'(Batch Normalization), \
-                supports ['BN', 'IN', 'SyncBN', None].
+                supports ['BN', 'LN', 'IN', 'GN', 'SyncBN', None].
             - res_type (:obj:`str`): type of residual block, supports ['basic', 'bottleneck', 'downsample']
             - bias (:obj:`bool`): whether adds a learnable bias to the conv2d_block. default set to True.
             - out_channels (:obj:`int`): Number of channels in the output tensor, default set to None,
                 which means out_channels = in_channels.
         """
         super(ResBlock, self).__init__()
         self.act = activation
@@ -97,23 +97,23 @@
         elif self.res_type == 'downsample':
             identity = self.conv3(identity)
         x = self.act(x + identity)
         return x
 
 
 class ResFCBlock(nn.Module):
-    r'''
+    r"""
     Overview:
         Residual Block with 2 fully connected layers.
         x -> fc1 -> norm -> act -> fc2 -> norm -> act -> out
         \_____________________________________/+
 
     Interfaces:
         forward
-    '''
+    """
 
     def __init__(self, in_channels: int, activation: nn.Module = nn.ReLU(), norm_type: str = 'BN'):
         r"""
         Overview:
             Init the fully connected layer residual block.
         Arguments:
             - in_channels (:obj:`int`): The number of channels in the input tensor.
```

### Comparing `DI-engine-0.4.7/ding/torch_utils/network/resnet.py` & `DI-engine-0.4.8/ding/torch_utils/network/resnet.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/torch_utils/network/rnn.py` & `DI-engine-0.4.8/ding/torch_utils/network/rnn.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/torch_utils/network/scatter_connection.py` & `DI-engine-0.4.8/ding/torch_utils/network/scatter_connection.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/torch_utils/network/soft_argmax.py` & `DI-engine-0.4.8/ding/torch_utils/network/soft_argmax.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/torch_utils/network/transformer.py` & `DI-engine-0.4.8/ding/torch_utils/network/transformer.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/torch_utils/nn_test_helper.py` & `DI-engine-0.4.8/ding/torch_utils/nn_test_helper.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/torch_utils/optimizer_helper.py` & `DI-engine-0.4.8/ding/torch_utils/optimizer_helper.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/torch_utils/reshape_helper.py` & `DI-engine-0.4.8/ding/torch_utils/reshape_helper.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/utils/__init__.py` & `DI-engine-0.4.8/ding/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/utils/autolog/base.py` & `DI-engine-0.4.8/ding/utils/autolog/base.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/utils/autolog/data.py` & `DI-engine-0.4.8/ding/utils/autolog/data.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/utils/autolog/model.py` & `DI-engine-0.4.8/ding/utils/autolog/model.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/utils/autolog/tests/test_data.py` & `DI-engine-0.4.8/ding/utils/autolog/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/utils/autolog/tests/test_model.py` & `DI-engine-0.4.8/ding/utils/autolog/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/utils/autolog/tests/test_time.py` & `DI-engine-0.4.8/ding/utils/autolog/tests/test_time.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/utils/autolog/time_ctl.py` & `DI-engine-0.4.8/ding/utils/autolog/time_ctl.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/utils/autolog/value.py` & `DI-engine-0.4.8/ding/utils/autolog/value.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/utils/bfs_helper.py` & `DI-engine-0.4.8/ding/utils/bfs_helper.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/utils/collection_helper.py` & `DI-engine-0.4.8/ding/utils/collection_helper.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/utils/compression_helper.py` & `DI-engine-0.4.8/ding/utils/compression_helper.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/utils/coverage.xml` & `DI-engine-0.4.8/ding/utils/coverage.xml`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/utils/data/base_dataloader.py` & `DI-engine-0.4.8/ding/utils/data/base_dataloader.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/utils/data/collate_fn.py` & `DI-engine-0.4.8/ding/utils/data/collate_fn.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/utils/data/dataloader.py` & `DI-engine-0.4.8/ding/utils/data/dataloader.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/utils/data/dataset.py` & `DI-engine-0.4.8/ding/utils/data/dataset.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/utils/data/structure/cache.py` & `DI-engine-0.4.8/ding/utils/data/structure/cache.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/utils/default_helper.py` & `DI-engine-0.4.8/ding/utils/default_helper.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,45 @@
 from typing import Union, Mapping, List, NamedTuple, Tuple, Callable, Optional, Any, Dict
 import copy
 from ditk import logging
 import random
 from functools import lru_cache  # in python3.9, we can change to cache
 import numpy as np
 import torch
+import treetensor.torch as ttorch
+
+
+def get_shape0(data: Union[List, Dict, torch.Tensor, ttorch.Tensor]) -> int:
+    """
+    Overview:
+        Get shape[0] of data's torch tensor or treetensor
+    Arguments:
+        - data (:obj:`Union[List,Dict,torch.Tensor,ttorch.Tensor]`): data to be analysed
+    Returns:
+        - shape[0] (:obj:`int`): first dimension length of data, usually the batchsize.
+    """
+    if isinstance(data, list) or isinstance(data, tuple):
+        return get_shape0(data[0])
+    elif isinstance(data, dict):
+        for k, v in data.items():
+            return get_shape0(v)
+    elif isinstance(data, torch.Tensor):
+        return data.shape[0]
+    elif isinstance(data, ttorch.Tensor):
+
+        def fn(t):
+            item = list(t.values())[0]
+            if np.isscalar(item[0]):
+                return item[0]
+            else:
+                return fn(item)
+
+        return fn(data.shape)
+    else:
+        raise TypeError("Error in getting shape0, not support type: {}".format(data))
 
 
 def lists_to_dicts(
         data: Union[List[Union[dict, NamedTuple]], Tuple[Union[dict, NamedTuple]]],
         recursive: bool = False,
 ) -> Union[Mapping[object, object], NamedTuple]:
     r"""
@@ -426,24 +457,24 @@
     length = []
     for k, v in data.items():
         if v is None:
             continue
         elif k in ['prev_state', 'prev_actor_state', 'prev_critic_state']:
             length.append(len(v))
         elif isinstance(v, list) or isinstance(v, tuple):
-            length.append(len(v[0]))
+            length.append(get_shape0(v[0]))
         elif isinstance(v, dict):
             length.append(len(v[list(v.keys())[0]]))
         else:
             length.append(len(v))
     assert len(length) > 0
     # assert len(set(length)) == 1, "data values must have the same length: {}".format(length)
     # if continuous action, data['logit'] is list of length 2
     length = length[0]
-    assert split_size >= 1 and split_size <= length
+    assert split_size >= 1 and split_size <= length, f'{split_size}_{length}'
     if shuffle:
         indices = np.random.permutation(length)
     else:
         indices = np.arange(length)
     for i in range(0, length, split_size):
         if i + split_size > length:
             i = length - split_size
```

### Comparing `DI-engine-0.4.7/ding/utils/design_helper.py` & `DI-engine-0.4.8/ding/utils/design_helper.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/utils/fast_copy.py` & `DI-engine-0.4.8/ding/utils/fast_copy.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/utils/file_helper.py` & `DI-engine-0.4.8/ding/utils/file_helper.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/utils/import_helper.py` & `DI-engine-0.4.8/ding/utils/import_helper.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/utils/k8s_helper.py` & `DI-engine-0.4.8/ding/utils/k8s_helper.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/utils/linklink_dist_helper.py` & `DI-engine-0.4.8/ding/utils/linklink_dist_helper.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/utils/loader/__init__.py` & `DI-engine-0.4.8/ding/utils/loader/__init__.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/utils/loader/base.py` & `DI-engine-0.4.8/ding/utils/loader/base.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/utils/loader/collection.py` & `DI-engine-0.4.8/ding/utils/loader/collection.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/utils/loader/dict.py` & `DI-engine-0.4.8/ding/utils/loader/dict.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/utils/loader/mapping.py` & `DI-engine-0.4.8/ding/utils/loader/mapping.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/utils/loader/norm.py` & `DI-engine-0.4.8/ding/utils/loader/norm.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/utils/loader/number.py` & `DI-engine-0.4.8/ding/utils/loader/number.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/utils/loader/string.py` & `DI-engine-0.4.8/ding/utils/loader/string.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/utils/loader/tests/loader/test_base.py` & `DI-engine-0.4.8/ding/utils/loader/tests/loader/test_base.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/utils/loader/tests/loader/test_collection.py` & `DI-engine-0.4.8/ding/utils/loader/tests/loader/test_collection.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/utils/loader/tests/loader/test_dict.py` & `DI-engine-0.4.8/ding/utils/loader/tests/loader/test_dict.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/utils/loader/tests/loader/test_mapping.py` & `DI-engine-0.4.8/ding/utils/loader/tests/loader/test_mapping.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/utils/loader/tests/loader/test_norm.py` & `DI-engine-0.4.8/ding/utils/loader/tests/loader/test_norm.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/utils/loader/tests/loader/test_number.py` & `DI-engine-0.4.8/ding/utils/loader/tests/loader/test_number.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/utils/loader/tests/loader/test_string.py` & `DI-engine-0.4.8/ding/utils/loader/tests/loader/test_string.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/utils/loader/tests/loader/test_types.py` & `DI-engine-0.4.8/ding/utils/loader/tests/loader/test_types.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/utils/loader/tests/loader/test_utils.py` & `DI-engine-0.4.8/ding/utils/loader/tests/loader/test_utils.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/utils/loader/tests/test_cartpole_dqn_serial_config_loader.py` & `DI-engine-0.4.8/ding/utils/loader/tests/test_cartpole_dqn_serial_config_loader.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/utils/loader/types.py` & `DI-engine-0.4.8/ding/utils/loader/types.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/utils/lock_helper.py` & `DI-engine-0.4.8/ding/utils/lock_helper.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/utils/log_helper.py` & `DI-engine-0.4.8/ding/utils/log_helper.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/utils/log_writer_helper.py` & `DI-engine-0.4.8/ding/utils/log_writer_helper.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/utils/orchestrator_launcher.py` & `DI-engine-0.4.8/ding/utils/orchestrator_launcher.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/utils/profiler_helper.py` & `DI-engine-0.4.8/ding/utils/profiler_helper.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/utils/pytorch_ddp_dist_helper.py` & `DI-engine-0.4.8/ding/utils/pytorch_ddp_dist_helper.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/utils/registry.py` & `DI-engine-0.4.8/ding/utils/registry.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/utils/registry_factory.py` & `DI-engine-0.4.8/ding/utils/registry_factory.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/utils/render_helper.py` & `DI-engine-0.4.8/ding/utils/render_helper.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/utils/scheduler_helper.py` & `DI-engine-0.4.8/ding/utils/scheduler_helper.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/utils/segment_tree.py` & `DI-engine-0.4.8/ding/utils/segment_tree.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/utils/slurm_helper.py` & `DI-engine-0.4.8/ding/utils/slurm_helper.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/utils/system_helper.py` & `DI-engine-0.4.8/ding/utils/system_helper.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/utils/time_helper.py` & `DI-engine-0.4.8/ding/utils/time_helper.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/utils/time_helper_base.py` & `DI-engine-0.4.8/ding/utils/time_helper_base.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/utils/time_helper_cuda.py` & `DI-engine-0.4.8/ding/utils/time_helper_cuda.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/worker/adapter/learner_aggregator.py` & `DI-engine-0.4.8/ding/worker/adapter/learner_aggregator.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/worker/collector/__init__.py` & `DI-engine-0.4.8/ding/worker/collector/__init__.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/worker/collector/base_parallel_collector.py` & `DI-engine-0.4.8/ding/worker/collector/base_parallel_collector.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/worker/collector/base_serial_collector.py` & `DI-engine-0.4.8/ding/worker/collector/base_serial_collector.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/worker/collector/base_serial_evaluator.py` & `DI-engine-0.4.8/ding/worker/collector/base_serial_evaluator.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/worker/collector/battle_episode_serial_collector.py` & `DI-engine-0.4.8/ding/worker/collector/battle_episode_serial_collector.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/worker/collector/battle_interaction_serial_evaluator.py` & `DI-engine-0.4.8/ding/worker/collector/battle_interaction_serial_evaluator.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/worker/collector/battle_sample_serial_collector.py` & `DI-engine-0.4.8/ding/worker/collector/battle_sample_serial_collector.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/worker/collector/comm/base_comm_collector.py` & `DI-engine-0.4.8/ding/worker/collector/comm/base_comm_collector.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/worker/collector/comm/flask_fs_collector.py` & `DI-engine-0.4.8/ding/worker/collector/comm/flask_fs_collector.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/worker/collector/comm/utils.py` & `DI-engine-0.4.8/ding/worker/collector/comm/utils.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/worker/collector/episode_serial_collector.py` & `DI-engine-0.4.8/ding/worker/collector/episode_serial_collector.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/worker/collector/interaction_serial_evaluator.py` & `DI-engine-0.4.8/ding/worker/collector/interaction_serial_evaluator.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/worker/collector/marine_parallel_collector.py` & `DI-engine-0.4.8/ding/worker/collector/marine_parallel_collector.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/worker/collector/metric_serial_evaluator.py` & `DI-engine-0.4.8/ding/worker/collector/metric_serial_evaluator.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/worker/collector/sample_serial_collector.py` & `DI-engine-0.4.8/ding/worker/collector/sample_serial_collector.py`

 * *Files 1% similar despite different names*

```diff
@@ -196,24 +196,26 @@
         self.close()
 
     def collect(
             self,
             n_sample: Optional[int] = None,
             train_iter: int = 0,
             drop_extra: bool = True,
+            record_random_collect: bool = True,
             policy_kwargs: Optional[dict] = None,
             level_seeds: Optional[List] = None,
     ) -> List[Any]:
         """
         Overview:
             Collect `n_sample` data with policy_kwargs, which is already trained `train_iter` iterations.
         Arguments:
             - n_sample (:obj:`int`): The number of collecting data sample.
             - train_iter (:obj:`int`): The number of training iteration when calling collect method.
             - drop_extra (:obj:`bool`): Whether to drop extra return_data more than `n_sample`.
+            - record_random_collect (:obj:`bool`) :Whether to output logs of random collect.
             - policy_kwargs (:obj:`dict`): The keyword args for policy forward.
             - level_seeds (:obj:`dict`): Used in PLR, represents the seed of the environment that \
                 generate the data
         Returns:
             - return_data (:obj:`List`): A list containing training samples.
         """
         if n_sample is None:
@@ -310,15 +312,18 @@
                         'train_sample': self._env_info[env_id]['train_sample'],
                     }
                     self._episode_info.append(info)
                     # Env reset is done by env_manager automatically
                     self._policy.reset([env_id])
                     self._reset_stat(env_id)
         # log
-        self._output_log(train_iter)
+        if record_random_collect:  # default is true, but when random collect, record_random_collect is False
+            self._output_log(train_iter)
+        else:
+            self._episode_info.clear()
         # on-policy reset
         if self._on_policy:
             for env_id in range(self._env_num):
                 self._reset_stat(env_id)
 
         if drop_extra:
             return return_data[:n_sample]
```

### Comparing `DI-engine-0.4.7/ding/worker/collector/tests/fake_cls_policy.py` & `DI-engine-0.4.8/ding/worker/collector/tests/fake_cls_policy.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/worker/collector/tests/fake_cpong_dqn_config.py` & `DI-engine-0.4.8/ding/worker/collector/tests/fake_cpong_dqn_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/worker/collector/tests/speed_test/fake_env.py` & `DI-engine-0.4.8/ding/worker/collector/tests/speed_test/fake_env.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/worker/collector/tests/speed_test/fake_policy.py` & `DI-engine-0.4.8/ding/worker/collector/tests/speed_test/fake_policy.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/worker/collector/tests/speed_test/test_collector_profile.py` & `DI-engine-0.4.8/ding/worker/collector/tests/speed_test/test_collector_profile.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/worker/collector/tests/test_base_serial_collector.py` & `DI-engine-0.4.8/ding/worker/collector/tests/test_base_serial_collector.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/worker/collector/tests/test_episode_serial_collector.py` & `DI-engine-0.4.8/ding/worker/collector/tests/test_episode_serial_collector.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/worker/collector/tests/test_marine_parallel_collector.py` & `DI-engine-0.4.8/ding/worker/collector/tests/test_marine_parallel_collector.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/worker/collector/tests/test_metric_serial_evaluator.py` & `DI-engine-0.4.8/ding/worker/collector/tests/test_metric_serial_evaluator.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/worker/collector/zergling_parallel_collector.py` & `DI-engine-0.4.8/ding/worker/collector/zergling_parallel_collector.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/worker/coordinator/base_parallel_commander.py` & `DI-engine-0.4.8/ding/worker/coordinator/base_parallel_commander.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/worker/coordinator/base_serial_commander.py` & `DI-engine-0.4.8/ding/worker/coordinator/base_serial_commander.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/worker/coordinator/comm_coordinator.py` & `DI-engine-0.4.8/ding/worker/coordinator/comm_coordinator.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/worker/coordinator/coordinator.py` & `DI-engine-0.4.8/ding/worker/coordinator/coordinator.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/worker/coordinator/one_vs_one_parallel_commander.py` & `DI-engine-0.4.8/ding/worker/coordinator/one_vs_one_parallel_commander.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/worker/coordinator/operator_server.py` & `DI-engine-0.4.8/ding/worker/coordinator/operator_server.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/worker/coordinator/resource_manager.py` & `DI-engine-0.4.8/ding/worker/coordinator/resource_manager.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/worker/coordinator/solo_parallel_commander.py` & `DI-engine-0.4.8/ding/worker/coordinator/solo_parallel_commander.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/worker/learner/base_learner.py` & `DI-engine-0.4.8/ding/worker/learner/base_learner.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/worker/learner/comm/base_comm_learner.py` & `DI-engine-0.4.8/ding/worker/learner/comm/base_comm_learner.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/worker/learner/comm/flask_fs_learner.py` & `DI-engine-0.4.8/ding/worker/learner/comm/flask_fs_learner.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/worker/learner/comm/utils.py` & `DI-engine-0.4.8/ding/worker/learner/comm/utils.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/worker/learner/learner_hook.py` & `DI-engine-0.4.8/ding/worker/learner/learner_hook.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/worker/replay_buffer/advanced_buffer.py` & `DI-engine-0.4.8/ding/worker/replay_buffer/advanced_buffer.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/worker/replay_buffer/base_buffer.py` & `DI-engine-0.4.8/ding/worker/replay_buffer/base_buffer.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/worker/replay_buffer/episode_buffer.py` & `DI-engine-0.4.8/ding/worker/replay_buffer/episode_buffer.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/worker/replay_buffer/naive_buffer.py` & `DI-engine-0.4.8/ding/worker/replay_buffer/naive_buffer.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/worker/replay_buffer/utils.py` & `DI-engine-0.4.8/ding/worker/replay_buffer/utils.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/world_model/base_world_model.py` & `DI-engine-0.4.8/ding/world_model/base_world_model.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/world_model/ddppo.py` & `DI-engine-0.4.8/ding/world_model/ddppo.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/world_model/idm.py` & `DI-engine-0.4.8/ding/world_model/idm.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/world_model/mbpo.py` & `DI-engine-0.4.8/ding/world_model/mbpo.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/ding/world_model/utils.py` & `DI-engine-0.4.8/ding/world_model/utils.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/atari/config/serial/asterix/asterix_mdqn_config.py` & `DI-engine-0.4.8/dizoo/atari/config/serial/asterix/asterix_mdqn_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 asterix_mdqn_config = dict(
     exp_name='asterix_mdqn_seed0',
     env=dict(
         collector_env_num=8,
         evaluator_env_num=8,
         n_evaluator_episode=8,
         stop_value=20000,
-        env_id='Asterix-v0',
+        env_id='AsterixNoFrameskip-v0',
         #'ALE/SpaceInvaders-v5' is available. But special setting is needed after gym make.
         frame_stack=4,
     ),
     policy=dict(
         cuda=True,
         priority=False,
         model=dict(
```

### Comparing `DI-engine-0.4.7/dizoo/atari/config/serial/enduro/enduro_dqn_config.py` & `DI-engine-0.4.8/dizoo/atari/config/serial/enduro/enduro_dqn_config.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 enduro_dqn_config = dict(
     exp_name='enduro_dqn_seed0',
     env=dict(
         collector_env_num=8,
         evaluator_env_num=8,
         n_evaluator_episode=8,
         stop_value=int(1e10),
-        env_id='Enduro-v4',
+        env_id='EnduroNoFrameskip-v4',
         #'ALE/Enduro-v5' is available. But special setting is needed after gym make.
         frame_stack=4,
     ),
     policy=dict(
         cuda=True,
         priority=False,
         model=dict(
```

### Comparing `DI-engine-0.4.7/dizoo/atari/config/serial/enduro/enduro_impala_config.py` & `DI-engine-0.4.8/dizoo/atari/config/serial/enduro/enduro_impala_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 enduro_impala_config = dict(
     exp_name='enduro_impala_seed0',
     env=dict(
         collector_env_num=16,
         evaluator_env_num=8,
         n_evaluator_episode=8,
         stop_value=10000000000,
-        env_id='Enduro-v4',
+        env_id='EnduroNoFrameskip-v4',
         #'ALE/Enduro-v5' is available. But special setting is needed after gym make.
         frame_stack=4
     ),
     policy=dict(
         cuda=True,
         # (int) the trajectory length to calculate v-trace target
         unroll_len=64,
```

### Comparing `DI-engine-0.4.7/dizoo/atari/config/serial/enduro/enduro_mdqn_config.py` & `DI-engine-0.4.8/dizoo/atari/config/serial/enduro/enduro_mdqn_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 enduro_mdqn_config = dict(
     exp_name='enduro_mdqn_seed0',
     env=dict(
         collector_env_num=8,
         evaluator_env_num=8,
         n_evaluator_episode=8,
         stop_value=int(1e10),
-        env_id='Enduro-v4',
+        env_id='EnduroNoFrameskip-v4',
         #'ALE/Enduro-v5' is available. But special setting is needed after gym make.
         frame_stack=4,
     ),
     policy=dict(
         cuda=True,
         priority=False,
         model=dict(
```

### Comparing `DI-engine-0.4.7/dizoo/atari/config/serial/enduro/enduro_onppo_config.py` & `DI-engine-0.4.8/dizoo/atari/config/serial/enduro/enduro_onppo_config.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 enduro_onppo_config = dict(
     exp_name='enduro_onppo_seed0',
     env=dict(
         collector_env_num=64,
         evaluator_env_num=8,
         n_evaluator_episode=8,
         stop_value=10000000000,
-        env_id='Enduro-v4',
+        env_id='EnduroNoFrameskip-v4',
         #'ALE/Enduro-v5' is available. But special setting is needed after gym make.
         frame_stack=4,
         manager=dict(shared_memory=False, )
     ),
     policy=dict(
         cuda=True,
         model=dict(
```

### Comparing `DI-engine-0.4.7/dizoo/atari/config/serial/enduro/enduro_qrdqn_config.py` & `DI-engine-0.4.8/dizoo/atari/config/serial/enduro/enduro_qrdqn_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 enduro_qrdqn_config = dict(
     exp_name='enduro_qrdqn_seed0',
     env=dict(
         collector_env_num=8,
         evaluator_env_num=8,
         n_evaluator_episode=8,
         stop_value=10000000000,
-        env_id='Enduro-v4',
+        env_id='EnduroNoFrameskip-v4',
         #'ALE/Enduro-v5' is available. But special setting is needed after gym make.
         frame_stack=4,
     ),
     policy=dict(
         cuda=True,
         priority=False,
         model=dict(
```

### Comparing `DI-engine-0.4.7/dizoo/atari/config/serial/enduro/enduro_rainbow_config.py` & `DI-engine-0.4.8/dizoo/atari/config/serial/enduro/enduro_rainbow_config.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 enduro_rainbow_config = dict(
     exp_name='enduro_rainbow_seed0',
     env=dict(
         collector_env_num=8,
         evaluator_env_num=8,
         n_evaluator_episode=8,
         stop_value=10000000000,
-        env_id='Enduro-v4',
+        env_id='EnduroNoFrameskip-v4',
         #'ALE/Enduro-v5' is available. But special setting is needed after gym make.
         frame_stack=4
     ),
     policy=dict(
         cuda=True,
         priority=True,
         model=dict(
```

### Comparing `DI-engine-0.4.7/dizoo/atari/config/serial/pong/pong_a2c_config.py` & `DI-engine-0.4.8/dizoo/atari/config/serial/pong/pong_a2c_config.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 pong_a2c_config = dict(
     exp_name='pong_a2c_seed0',
     env=dict(
         collector_env_num=8,
         evaluator_env_num=8,
         n_evaluator_episode=8,
         stop_value=20,
-        env_id='Pong-v4',
+        env_id='PongNoFrameskip-v4',
         #'ALE/Pong-v5' is available. But special setting is needed after gym make.
         frame_stack=4,
     ),
     policy=dict(
         cuda=True,
         model=dict(
             obs_shape=[4, 84, 84],
```

### Comparing `DI-engine-0.4.7/dizoo/atari/config/serial/pong/pong_acer_config.py` & `DI-engine-0.4.8/dizoo/atari/config/serial/pong/pong_acer_config.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 pong_acer_config = dict(
     env=dict(
         collector_env_num=8,
         evaluator_env_num=8,
         n_evaluator_episode=8,
         stop_value=20,
-        env_id='Pong-v4',
+        env_id='PongNoFrameskip-v4',
         #'ALE/Pong-v5' is available. But special setting is needed after gym make.
         frame_stack=4,
     ),
     policy=dict(
         cuda=True,
         priority=False,
         model=dict(
```

### Comparing `DI-engine-0.4.7/dizoo/atari/config/serial/pong/pong_c51_config.py` & `DI-engine-0.4.8/dizoo/atari/config/serial/pong/pong_c51_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 pong_c51_config = dict(
     exp_name='pong_c51_seed0',
     env=dict(
         collector_env_num=8,
         evaluator_env_num=8,
         n_evaluator_episode=8,
         stop_value=20,
-        env_id='Pong-v4',
+        env_id='PongNoFrameskip-v4',
         #'ALE/Pong-v5' is available. But special setting is needed after gym make.
         frame_stack=4,
     ),
     policy=dict(
         cuda=True,
         priority=False,
         model=dict(
```

### Comparing `DI-engine-0.4.7/dizoo/atari/config/serial/pong/pong_cql_config.py` & `DI-engine-0.4.8/dizoo/atari/config/serial/pong/pong_cql_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 pong_cql_config = dict(
     exp_name='pong_cql_seed0',
     env=dict(
         collector_env_num=8,
         evaluator_env_num=8,
         n_evaluator_episode=8,
         stop_value=20,
-        env_id='Pong-v4',
+        env_id='PongNoFrameskip-v4',
         #'ALE/Pong-v5' is available. But special setting is needed after gym make.
         frame_stack=4,
     ),
     policy=dict(
         cuda=True,
         priority=False,
         model=dict(
```

### Comparing `DI-engine-0.4.7/dizoo/atari/config/serial/pong/pong_dqfd_config.py` & `DI-engine-0.4.8/dizoo/atari/config/serial/pong/pong_dqfd_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 pong_dqfd_config = dict(
     exp_name='pong_dqfd_seed0',
     env=dict(
         collector_env_num=8,
         evaluator_env_num=8,
         n_evaluator_episode=8,
         stop_value=20,
-        env_id='Pong-v4',
+        env_id='PongNoFrameskip-v4',
         #'ALE/Pong-v5' is available. But special setting is needed after gym make.
         frame_stack=4,
     ),
     policy=dict(
         cuda=True,
         priority=True,
         model=dict(
```

### Comparing `DI-engine-0.4.7/dizoo/atari/config/serial/pong/pong_dqn_config.py` & `DI-engine-0.4.8/dizoo/atari/config/serial/pong/pong_dqn_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 pong_dqn_config = dict(
     exp_name='pong_dqn_seed0',
     env=dict(
         collector_env_num=8,
         evaluator_env_num=8,
         n_evaluator_episode=8,
         stop_value=20,
-        env_id='Pong-v4',
+        env_id='PongNoFrameskip-v4',
         #'ALE/Pong-v5' is available. But special setting is needed after gym make.
         frame_stack=4,
     ),
     policy=dict(
         cuda=True,
         priority=False,
         model=dict(
```

### Comparing `DI-engine-0.4.7/dizoo/atari/config/serial/pong/pong_dqn_envpool_config.py` & `DI-engine-0.4.8/dizoo/atari/config/serial/pong/pong_dqn_envpool_config.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     env=dict(
         collector_env_num=8,
         collector_batch_size=8,
         evaluator_env_num=8,
         evaluator_batch_size=8,
         n_evaluator_episode=8,
         stop_value=20,
-        env_id='Pong-v4',
+        env_id='PongNoFrameskip-v4',
         #'ALE/Pong-v5' is available. But special setting is needed after gym make.
         frame_stack=4,
     ),
     policy=dict(
         cuda=True,
         priority=False,
         model=dict(
```

### Comparing `DI-engine-0.4.7/dizoo/atari/config/serial/pong/pong_dqn_multi_gpu_config.py` & `DI-engine-0.4.8/dizoo/atari/config/serial/pong/pong_dqn_multi_gpu_config.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 pong_dqn_config = dict(
     exp_name='pong_dqn_multi_gpu_seed0',
     env=dict(
         collector_env_num=4,
         evaluator_env_num=4,
         n_evaluator_episode=8,
         stop_value=20,
-        env_id='Pong-v4',
+        env_id='PongNoFrameskip-v4',
         #'ALE/Pong-v5' is available. But special setting is needed after gym make.
         frame_stack=4,
     ),
     policy=dict(
         cuda=True,
         priority=False,
         multi_gpu=True,
```

### Comparing `DI-engine-0.4.7/dizoo/atari/config/serial/pong/pong_dqn_render_config.py` & `DI-engine-0.4.8/dizoo/atari/config/serial/pong/pong_dqn_render_config.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 pong_dqn_config = dict(
     exp_name='pong_dqn_render_seed0',
     env=dict(
         collector_env_num=8,
         evaluator_env_num=8,
         n_evaluator_episode=8,
         stop_value=20,
-        env_id='Pong-v4',
+        env_id='PongNoFrameskip-v4',
         #'ALE/Pong-v5' is available. But special setting is needed after gym make.
         frame_stack=4,
     ),
     policy=dict(
         cuda=True,
         priority=False,
         model=dict(
```

### Comparing `DI-engine-0.4.7/dizoo/atari/config/serial/pong/pong_dqn_stdim_config.py` & `DI-engine-0.4.8/dizoo/atari/config/serial/pong/pong_dqn_stdim_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 pong_dqn_stdim_config = dict(
     exp_name='pong_dqn_stdim_seed0',
     env=dict(
         collector_env_num=8,
         evaluator_env_num=8,
         n_evaluator_episode=8,
         stop_value=20,
-        env_id='Pong-v4',
+        env_id='PongNoFrameskip-v4',
         #'ALE/Pong-v5' is available. But special setting is needed after gym make.
         frame_stack=4,
     ),
     policy=dict(
         cuda=True,
         priority=False,
         model=dict(
```

### Comparing `DI-engine-0.4.7/dizoo/atari/config/serial/pong/pong_fqf_config.py` & `DI-engine-0.4.8/dizoo/atari/config/serial/pong/pong_fqf_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 pong_fqf_config = dict(
     exp_name='pong_fqf_seed0',
     env=dict(
         collector_env_num=8,
         evaluator_env_num=8,
         n_evaluator_episode=8,
         stop_value=10000000000,
-        env_id='Pong-v4',
+        env_id='PongNoFrameskip-v4',
         #'ALE/Pong-v5' is available. But special setting is needed after gym make.
         frame_stack=4,
     ),
     policy=dict(
         cuda=True,
         priority=False,
         model=dict(
```

### Comparing `DI-engine-0.4.7/dizoo/atari/config/serial/pong/pong_gail_dqn_config.py` & `DI-engine-0.4.8/dizoo/atari/config/serial/pong/pong_gail_dqn_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 pong_dqn_gail_config = dict(
     exp_name='pong_gail_dqn_seed0',
     env=dict(
         collector_env_num=8,
         evaluator_env_num=8,
         n_evaluator_episode=8,
         stop_value=20,
-        env_id='Pong-v4',
+        env_id='PongNoFrameskip-v4',
         #'ALE/Pong-v5' is available. But special setting is needed after gym make.
         frame_stack=4,
     ),
     reward_model=dict(
         type='gail',
         input_size=[4, 84, 84],
         hidden_size=128,
```

### Comparing `DI-engine-0.4.7/dizoo/atari/config/serial/pong/pong_impala_config.py` & `DI-engine-0.4.8/dizoo/atari/config/serial/pong/pong_impala_config.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 pong_impala_config = dict(
     exp_name='pong_impala_seed0',
     env=dict(
         collector_env_num=8,
         evaluator_env_num=8,
         n_evaluator_episode=8,
         stop_value=20,
-        env_id='Pong-v4',
+        env_id='PongNoFrameskip-v4',
         #'ALE/Pong-v5' is available. But special setting is needed after gym make.
         frame_stack=4,
     ),
     policy=dict(
         cuda=True,
         priority=False,
         # (int) the trajectory length to calculate v-trace target
```

### Comparing `DI-engine-0.4.7/dizoo/atari/config/serial/pong/pong_iqn_config.py` & `DI-engine-0.4.8/dizoo/atari/config/serial/qbert/qbert_dqn_config.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,62 +1,59 @@
 from easydict import EasyDict
 
-pong_iqn_config = dict(
-    exp_name='pong_iqn_seed0',
+qbert_dqn_config = dict(
+    exp_name='qbert_dqn_seed0',
     env=dict(
         collector_env_num=8,
         evaluator_env_num=8,
         n_evaluator_episode=8,
-        stop_value=20,
-        env_id='Pong-v4',
-        #'ALE/Pong-v5' is available. But special setting is needed after gym make.
-        frame_stack=4,
+        stop_value=30000,
+        env_id='QbertNoFrameskip-v4',
+        #'ALE/Qbert-v5' is available. But special setting is needed after gym make.
+        frame_stack=4
     ),
     policy=dict(
         cuda=True,
         priority=False,
         model=dict(
             obs_shape=[4, 84, 84],
             action_shape=6,
             encoder_hidden_size_list=[128, 128, 512],
-            num_quantiles=32,
         ),
         nstep=3,
         discount_factor=0.99,
-        kappa=1.0,
         learn=dict(
             update_per_collect=10,
             batch_size=32,
             learning_rate=0.0001,
             target_update_freq=500,
         ),
         collect=dict(n_sample=100, ),
         eval=dict(evaluator=dict(eval_freq=4000, )),
         other=dict(
             eps=dict(
                 type='exp',
                 start=1.,
                 end=0.05,
-                decay=250000,
+                decay=1000000,
             ),
-            replay_buffer=dict(replay_buffer_size=100000, ),
+            replay_buffer=dict(replay_buffer_size=400000, ),
         ),
     ),
 )
-pong_iqn_config = EasyDict(pong_iqn_config)
-main_config = pong_iqn_config
-
-pong_iqn_create_config = dict(
+qbert_dqn_config = EasyDict(qbert_dqn_config)
+main_config = qbert_dqn_config
+qbert_dqn_create_config = dict(
     env=dict(
         type='atari',
         import_names=['dizoo.atari.envs.atari_env'],
     ),
     env_manager=dict(type='subprocess'),
-    policy=dict(type='iqn'),
+    policy=dict(type='dqn'),
 )
-pong_iqn_create_config = EasyDict(pong_iqn_create_config)
-create_config = pong_iqn_create_config
+qbert_dqn_create_config = EasyDict(qbert_dqn_create_config)
+create_config = qbert_dqn_create_config
 
 if __name__ == '__main__':
-    # or you can enter `ding -m serial -c pong_iqn_config.py -s 0`
+    # or you can enter ding -m serial -c qbert_dqn_config.py -s 0
     from ding.entry import serial_pipeline
     serial_pipeline((main_config, create_config), seed=0)
```

### Comparing `DI-engine-0.4.7/dizoo/atari/config/serial/pong/pong_ngu_config.py` & `DI-engine-0.4.8/dizoo/atari/config/serial/pong/pong_ngu_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 nstep = 5
 pong_ppo_rnd_config = dict(
     exp_name='pong_ngu_seed0',
     env=dict(
         collector_env_num=collector_env_num,
         evaluator_env_num=evaluator_env_num,
         n_evaluator_episode=evaluator_env_num,
-        env_id='Pong-v4',
+        env_id='PongNoFrameskip-v4',
         #'ALE/Pong-v5' is available. But special setting is needed after gym make.
         obs_plus_prev_action_reward=True,  # use specific env wrapper for ngu policy
         stop_value=20,
         frame_stack=4,
     ),
     rnd_reward_model=dict(
         intrinsic_reward_type='add',
```

### Comparing `DI-engine-0.4.7/dizoo/atari/config/serial/pong/pong_onppo_config.py` & `DI-engine-0.4.8/dizoo/atari/config/serial/pong/pong_onppo_config.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 pong_onppo_config = dict(
     env=dict(
         collector_env_num=8,
         evaluator_env_num=8,
         n_evaluator_episode=8,
         stop_value=20,
-        env_id='Pong-v4',
+        env_id='PongNoFrameskip-v4',
         #'ALE/Pong-v5' is available. But special setting is needed after gym make.
         frame_stack=4,
     ),
     policy=dict(
         cuda=True,
         recompute_adv=True,
         action_space='discrete',
```

### Comparing `DI-engine-0.4.7/dizoo/atari/config/serial/pong/pong_ppg_config.py` & `DI-engine-0.4.8/dizoo/atari/config/serial/pong/pong_ppg_config.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 pong_ppg_config = dict(
     exp_name='pong_ppg_seed0',
     env=dict(
         collector_env_num=8,
         evaluator_env_num=8,
         n_evaluator_episode=8,
         stop_value=20,
-        env_id='Pong-v4',
+        env_id='PongNoFrameskip-v4',
         #'ALE/Pong-v5' is available. But special setting is needed after gym make.
         frame_stack=4,
     ),
     policy=dict(
         cuda=True,
         model=dict(
             obs_shape=[4, 84, 84],
```

### Comparing `DI-engine-0.4.7/dizoo/atari/config/serial/pong/pong_qrdqn_config.py` & `DI-engine-0.4.8/dizoo/atari/config/serial/pong/pong_qrdqn_config.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 pong_qrdqn_config = dict(
     exp_name='pong_qrdqn_seed0',
     env=dict(
         collector_env_num=8,
         evaluator_env_num=8,
         n_evaluator_episode=8,
         stop_value=20,
-        env_id='Pong-v4',
+        env_id='PongNoFrameskip-v4',
         #'ALE/Pong-v5' is available. But special setting is needed after gym make.
         frame_stack=4,
     ),
     policy=dict(
         cuda=True,
         priority=False,
         model=dict(
```

### Comparing `DI-engine-0.4.7/dizoo/atari/config/serial/pong/pong_qrdqn_generation_data_config.py` & `DI-engine-0.4.8/dizoo/atari/config/serial/pong/pong_qrdqn_generation_data_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 pong_qrdqn_config = dict(
     exp_name='pong_qrdqn_generation_data_seed0',
     env=dict(
         collector_env_num=8,
         evaluator_env_num=8,
         n_evaluator_episode=8,
         stop_value=20,
-        env_id='Pong-v4',
+        env_id='PongNoFrameskip-v4',
         #'ALE/Pong-v5' is available. But special setting is needed after gym make.
         frame_stack=4,
     ),
     policy=dict(
         cuda=True,
         priority=False,
         model=dict(
```

### Comparing `DI-engine-0.4.7/dizoo/atari/config/serial/pong/pong_r2d2_config.py` & `DI-engine-0.4.8/dizoo/atari/config/serial/pong/pong_r2d2_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 pong_r2d2_config = dict(
     exp_name='pong_r2d2_seed0',
     env=dict(
         collector_env_num=collector_env_num,
         evaluator_env_num=evaluator_env_num,
         n_evaluator_episode=evaluator_env_num,
         stop_value=20,
-        env_id='Pong-v4',
+        env_id='PongNoFrameskip-v4',
         #'ALE/Pong-v5' is available. But special setting is needed after gym make.
         frame_stack=4,
     ),
     policy=dict(
         cuda=True,
         priority=True,
         priority_IS_weight=True,
```

### Comparing `DI-engine-0.4.7/dizoo/atari/config/serial/pong/pong_r2d2_gtrxl_config.py` & `DI-engine-0.4.8/dizoo/atari/config/serial/pong/pong_r2d2_gtrxl_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 pong_r2d2_gtrxl_config = dict(
     exp_name='pong_r2d2_gtrxl_seed0',
     env=dict(
         collector_env_num=collector_env_num,
         evaluator_env_num=evaluator_env_num,
         n_evaluator_episode=5,
         stop_value=20,
-        env_id='Pong-v4',
+        env_id='PongNoFrameskip-v4',
         #'ALE/Pong-v5' is available. But special setting is needed after gym make.
         frame_stack=4,
     ),
     policy=dict(
         cuda=True,
         on_policy=False,
         priority=True,
```

### Comparing `DI-engine-0.4.7/dizoo/atari/config/serial/pong/pong_r2d2_residual_config.py` & `DI-engine-0.4.8/dizoo/atari/config/serial/pong/pong_r2d2_residual_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 pong_r2d2_residual_config = dict(
     exp_name='pong_r2d2_residual_seed0',
     env=dict(
         collector_env_num=collector_env_num,
         evaluator_env_num=evaluator_env_num,
         n_evaluator_episode=evaluator_env_num,
         stop_value=20,
-        env_id='Pong-v4',
+        env_id='PongNoFrameskip-v4',
         #'ALE/Pong-v5' is available. But special setting is needed after gym make.
         frame_stack=4,
     ),
     policy=dict(
         cuda=True,
         priority=True,
         priority_IS_weight=True,
```

### Comparing `DI-engine-0.4.7/dizoo/atari/config/serial/pong/pong_r2d3_offppoexpert_config.py` & `DI-engine-0.4.8/dizoo/atari/config/serial/pong/pong_r2d3_offppoexpert_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 pong_r2d3_config = dict(
     exp_name='pong_r2d3_offppo-expert_seed0',
     env=dict(
         collector_env_num=collector_env_num,
         evaluator_env_num=evaluator_env_num,
         n_evaluator_episode=evaluator_env_num,
         stop_value=20,
-        env_id='Pong-v4',
+        env_id='PongNoFrameskip-v4',
         #'ALE/Pong-v5' is available. But special setting is needed after gym make.
         frame_stack=4,
     ),
     policy=dict(
         cuda=True,
         priority=True,
         priority_IS_weight=True,
@@ -97,15 +97,15 @@
 expert_pong_r2d3_config = dict(
     exp_name='expert_pong_r2d3_offppo-expert_seed0',
     env=dict(
         collector_env_num=collector_env_num,
         evaluator_env_num=evaluator_env_num,
         n_evaluator_episode=evaluator_env_num,
         stop_value=20,
-        env_id='Pong-v4',
+        env_id='PongNoFrameskip-v4',
         #'ALE/Pong-v5' is available. But special setting is needed after gym make.
         frame_stack=4,
     ),
     policy=dict(
         cuda=True,
         priority=True,
         priority_IS_weight=True,
```

### Comparing `DI-engine-0.4.7/dizoo/atari/config/serial/pong/pong_r2d3_r2d2expert_config.py` & `DI-engine-0.4.8/dizoo/atari/config/serial/pong/pong_r2d3_r2d2expert_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 pong_r2d3_config = dict(
     exp_name='pong_r2d3_r2d2expert_k0_pho1-4_rbs2e4_ds5e3_seed0',
     env=dict(
         collector_env_num=collector_env_num,
         evaluator_env_num=evaluator_env_num,
         n_evaluator_episode=evaluator_env_num,
         stop_value=20,
-        env_id='Pong-v4',
+        env_id='PongNoFrameskip-v4',
         #'ALE/Pong-v5' is available. But special setting is needed after gym make.
         frame_stack=4,
     ),
     policy=dict(
         cuda=True,
         priority=True,
         priority_IS_weight=True,
@@ -101,15 +101,15 @@
 expert_pong_r2d3_config = dict(
     exp_name='expert_pong_r2d3_r2d2expert_seed0',
     env=dict(
         collector_env_num=collector_env_num,
         evaluator_env_num=evaluator_env_num,
         n_evaluator_episode=evaluator_env_num,
         stop_value=20,
-        env_id='Pong-v4',
+        env_id='PongNoFrameskip-v4',
         #'ALE/Pong-v5' is available. But special setting is needed after gym make.
         frame_stack=4,
     ),
     policy=dict(
         cuda=True,
         priority=True,
         priority_IS_weight=True,
```

### Comparing `DI-engine-0.4.7/dizoo/atari/config/serial/pong/pong_rainbow_config.py` & `DI-engine-0.4.8/dizoo/atari/config/serial/pong/pong_rainbow_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 pong_rainbow_config = dict(
     env=dict(
         exp_name='pong_rainbow_seed0',
         collector_env_num=8,
         evaluator_env_num=8,
         n_evaluator_episode=8,
         stop_value=20,
-        env_id='Pong-v4',
+        env_id='PongNoFrameskip-v4',
         #'ALE/Pong-v5' is available. But special setting is needed after gym make.
         frame_stack=4,
     ),
     policy=dict(
         cuda=True,
         priority=False,
         priority_IS_weight=False,
```

### Comparing `DI-engine-0.4.7/dizoo/atari/config/serial/pong/pong_sqil_config.py` & `DI-engine-0.4.8/dizoo/atari/config/serial/pong/pong_sqil_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 pong_sqil_config = dict(
     exp_name='pong_sqil_seed0',
     env=dict(
         collector_env_num=8,
         evaluator_env_num=8,
         n_evaluator_episode=8,
         stop_value=20,
-        env_id='Pong-v4',
+        env_id='PongNoFrameskip-v4',
         #'ALE/Pong-v5' is available. But special setting is needed after gym make.
         frame_stack=4,
     ),
     policy=dict(
         cuda=True,
         priority=True,
         model=dict(
```

### Comparing `DI-engine-0.4.7/dizoo/atari/config/serial/pong/pong_sql_config.py` & `DI-engine-0.4.8/dizoo/atari/config/serial/pong/pong_sql_config.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 pong_sql_config = dict(
     exp_name='pong_sql_seed0',
     env=dict(
         collector_env_num=8,
         evaluator_env_num=8,
         n_evaluator_episode=8,
         stop_value=20,
-        env_id='Pong-v4',
+        env_id='PongNoFrameskip-v4',
         #'ALE/Pong-v5' is available. But special setting is needed after gym make.
         frame_stack=4,
     ),
     policy=dict(
         cuda=True,
         priority=False,
         model=dict(
```

### Comparing `DI-engine-0.4.7/dizoo/atari/config/serial/pong/pong_trex_offppo_config.py` & `DI-engine-0.4.8/dizoo/atari/config/serial/pong/pong_trex_offppo_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 pong_trex_ppo_config = dict(
     exp_name='pong_trex_offppo_seed0',
     env=dict(
         collector_env_num=4,
         evaluator_env_num=4,
         n_evaluator_episode=8,
         stop_value=20,
-        env_id='Pong-v4',
+        env_id='PongNoFrameskip-v4',
         #'ALE/Pong-v5' is available. But special setting is needed after gym make.
         frame_stack=4,
     ),
     reward_model=dict(
         type='trex',
         min_snippet_length=50,
         max_snippet_length=100,
```

### Comparing `DI-engine-0.4.7/dizoo/atari/config/serial/pong/pong_trex_sql_config.py` & `DI-engine-0.4.8/dizoo/atari/config/serial/pong/pong_trex_sql_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 pong_trex_sql_config = dict(
     exp_name='pong_trex_sql_seed0',
     env=dict(
         collector_env_num=8,
         evaluator_env_num=8,
         n_evaluator_episode=8,
         stop_value=20,
-        env_id='Pong-v4',
+        env_id='PongNoFrameskip-v4',
         #'ALE/Pong-v5' is available. But special setting is needed after gym make.
         frame_stack=4,
     ),
     reward_model=dict(
         type='trex',
         min_snippet_length=50,
         max_snippet_length=100,
```

### Comparing `DI-engine-0.4.7/dizoo/atari/config/serial/qbert/qbert_a2c_config.py` & `DI-engine-0.4.8/dizoo/atari/config/serial/qbert/qbert_a2c_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 qbert_a2c_config = dict(
     exp_name='qbert_a2c_seed0',
     env=dict(
         collector_env_num=16,
         evaluator_env_num=8,
         n_evaluator_episode=8,
         stop_value=1000000,
-        env_id='Qbert-v4',
+        env_id='QbertNoFrameskip-v4',
         #'ALE/Qbert-v5' is available. But special setting is needed after gym make.
         frame_stack=4
     ),
     policy=dict(
         cuda=True,
         model=dict(
             obs_shape=[4, 84, 84],
```

### Comparing `DI-engine-0.4.7/dizoo/atari/config/serial/qbert/qbert_acer_config.py` & `DI-engine-0.4.8/dizoo/atari/config/serial/qbert/qbert_acer_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 qbert_acer_config = dict(
     exp_name='qbert_acer_seed0',
     env=dict(
         collector_env_num=16,
         evaluator_env_num=8,
         n_evaluator_episode=8,
         stop_value=int(1e6),
-        env_id='Qbert-v4',
+        env_id='QbertNoFrameskip-v4',
         #'ALE/Qbert-v5' is available. But special setting is needed after gym make.
         frame_stack=4,
         manager=dict(shared_memory=False, )
     ),
     policy=dict(
         cuda=True,
         priority=False,
```

### Comparing `DI-engine-0.4.7/dizoo/atari/config/serial/qbert/qbert_c51_config.py` & `DI-engine-0.4.8/dizoo/atari/config/serial/qbert/qbert_qrdqn_config.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 from easydict import EasyDict
 
-qbert_c51_config = dict(
-    exp_name='qbert_c51_seed0',
+qbert_qrdqn_config = dict(
+    exp_name='qbert_qrdqn_seed0',
     env=dict(
         collector_env_num=8,
         evaluator_env_num=8,
         n_evaluator_episode=8,
         stop_value=30000,
-        env_id='Qbert-v4',
+        env_id='QbertNoFrameskip-v4',
         #'ALE/Qbert-v5' is available. But special setting is needed after gym make.
         frame_stack=4
     ),
     policy=dict(
         cuda=True,
         priority=True,
         model=dict(
             obs_shape=[4, 84, 84],
             action_shape=6,
             encoder_hidden_size_list=[128, 128, 512],
-            v_min=-10,
-            v_max=10,
-            n_atom=51,
+            num_quantiles=64,
         ),
         nstep=3,
         discount_factor=0.99,
         learn=dict(
             update_per_collect=10,
             batch_size=32,
             learning_rate=0.0001,
@@ -39,23 +37,23 @@
                 end=0.05,
                 decay=1000000,
             ),
             replay_buffer=dict(replay_buffer_size=400000, ),
         ),
     ),
 )
-main_config = EasyDict(qbert_c51_config)
+main_config = EasyDict(qbert_qrdqn_config)
 
-qbert_c51_create_config = dict(
+qbert_qrdqn_create_config = dict(
     env=dict(
         type='atari',
         import_names=['dizoo.atari.envs.atari_env'],
     ),
     env_manager=dict(type='subprocess'),
-    policy=dict(type='c51'),
+    policy=dict(type='qrdqn'),
 )
-create_config = EasyDict(qbert_c51_create_config)
+create_config = EasyDict(qbert_qrdqn_create_config)
 
 if __name__ == '__main__':
-    # or you can enter ding -m serial -c qbert_c51_config.py -s 0
+    # or you can enter ding -m serial -c qbert_qrdqn_config.py -s 0
     from ding.entry import serial_pipeline
     serial_pipeline((main_config, create_config), seed=0)
```

### Comparing `DI-engine-0.4.7/dizoo/atari/config/serial/qbert/qbert_cql_config.py` & `DI-engine-0.4.8/dizoo/atari/config/serial/qbert/qbert_cql_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 qbert_cql_config = dict(
     exp_name='qbert_cql_seed0',
     env=dict(
         collector_env_num=8,
         evaluator_env_num=8,
         n_evaluator_episode=8,
         stop_value=30000,
-        env_id='Qbert-v4',
+        env_id='QbertNoFrameskip-v4',
         #'ALE/Qbert-v5' is available. But special setting is needed after gym make.
         frame_stack=4
     ),
     policy=dict(
         cuda=True,
         priority=False,
         model=dict(
```

### Comparing `DI-engine-0.4.7/dizoo/atari/config/serial/qbert/qbert_dqfd_config.py` & `DI-engine-0.4.8/dizoo/atari/config/serial/qbert/qbert_dqfd_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 qbert_dqfd_config = dict(
     exp_name='qbert_dqfd_seed0',
     env=dict(
         collector_env_num=8,
         evaluator_env_num=8,
         n_evaluator_episode=8,
         stop_value=30000,
-        env_id='Qbert-v4',
+        env_id='QbertNoFrameskip-v4',
         #'ALE/Qbert-v5' is available. But special setting is needed after gym make.
         frame_stack=4
     ),
     policy=dict(
         cuda=True,
         priority=True,
         model=dict(
```

### Comparing `DI-engine-0.4.7/dizoo/atari/config/serial/qbert/qbert_dqn_config.py` & `DI-engine-0.4.8/dizoo/box2d/carracing/config/carracing_dqn_config.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,59 +1,63 @@
 from easydict import EasyDict
 
-qbert_dqn_config = dict(
-    exp_name='qbert_dqn_seed0',
+nstep = 3
+carracing_dqn_config = dict(
+    exp_name='carracing_dqn_seed0',
     env=dict(
         collector_env_num=8,
         evaluator_env_num=8,
+        env_id='CarRacing-v2',
+        continuous=False,
         n_evaluator_episode=8,
-        stop_value=30000,
-        env_id='Qbert-v4',
-        #'ALE/Qbert-v5' is available. But special setting is needed after gym make.
-        frame_stack=4
+        stop_value=900,
+        # replay_path='./carracing_dqn_seed0/video',
     ),
     policy=dict(
         cuda=True,
-        priority=False,
+        # load_path='carracing_dqn_seed0/ckpt/ckpt_best.pth.tar',
         model=dict(
-            obs_shape=[4, 84, 84],
-            action_shape=6,
-            encoder_hidden_size_list=[128, 128, 512],
+            obs_shape=[3, 96, 96],
+            action_shape=5,
+            encoder_hidden_size_list=[64, 64, 128],
+            dueling=True,
         ),
-        nstep=3,
         discount_factor=0.99,
+        nstep=nstep,
         learn=dict(
             update_per_collect=10,
-            batch_size=32,
+            batch_size=64,
             learning_rate=0.0001,
-            target_update_freq=500,
+            target_update_freq=100,
+        ),
+        collect=dict(
+            n_sample=64,
         ),
-        collect=dict(n_sample=100, ),
-        eval=dict(evaluator=dict(eval_freq=4000, )),
         other=dict(
             eps=dict(
                 type='exp',
-                start=1.,
-                end=0.05,
-                decay=1000000,
+                start=0.95,
+                end=0.1,
+                decay=50000,
             ),
-            replay_buffer=dict(replay_buffer_size=400000, ),
+            replay_buffer=dict(replay_buffer_size=100000, )
         ),
     ),
 )
-qbert_dqn_config = EasyDict(qbert_dqn_config)
-main_config = qbert_dqn_config
-qbert_dqn_create_config = dict(
+carracing_dqn_config = EasyDict(carracing_dqn_config)
+main_config = carracing_dqn_config
+
+carracing_dqn_create_config = dict(
     env=dict(
-        type='atari',
-        import_names=['dizoo.atari.envs.atari_env'],
+        type='carracing',
+        import_names=['dizoo.box2d.carracing.envs.carracing_env'],
     ),
     env_manager=dict(type='subprocess'),
     policy=dict(type='dqn'),
 )
-qbert_dqn_create_config = EasyDict(qbert_dqn_create_config)
-create_config = qbert_dqn_create_config
+carracing_dqn_create_config = EasyDict(carracing_dqn_create_config)
+create_config = carracing_dqn_create_config
 
-if __name__ == '__main__':
-    # or you can enter ding -m serial -c qbert_dqn_config.py -s 0
+if __name__ == "__main__":
+    # or you can enter `ding -m serial -c carracing_dqn_config.py -s 0`
     from ding.entry import serial_pipeline
-    serial_pipeline((main_config, create_config), seed=0)
+    serial_pipeline([main_config, create_config], seed=0)
```

### Comparing `DI-engine-0.4.7/dizoo/atari/config/serial/qbert/qbert_fqf_config.py` & `DI-engine-0.4.8/dizoo/atari/config/serial/qbert/qbert_fqf_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 qbert_fqf_config = dict(
     exp_name='qbert_fqf_seed0',
     env=dict(
         collector_env_num=8,
         evaluator_env_num=8,
         n_evaluator_episode=8,
         stop_value=10000000000,
-        env_id='Qbert-v4',
+        env_id='QbertNoFrameskip-v4',
         #'ALE/Qbert-v5' is available. But special setting is needed after gym make.
         frame_stack=4,
     ),
     policy=dict(
         cuda=True,
         priority=False,
         model=dict(
```

### Comparing `DI-engine-0.4.7/dizoo/atari/config/serial/qbert/qbert_impala_config.py` & `DI-engine-0.4.8/dizoo/atari/config/serial/qbert/qbert_impala_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 qbert_impala_config = dict(
     exp_name='qbert_impala_seed0',
     env=dict(
         collector_env_num=8,
         evaluator_env_num=8,
         n_evaluator_episode=8,
         stop_value=10000000000,
-        env_id='Qbert-v4',
+        env_id='QbertNoFrameskip-v4',
         #'ALE/Qbert-v5' is available. But special setting is needed after gym make.
         frame_stack=4
     ),
     policy=dict(
         cuda=True,
         # (int) the trajectory length to calculate v-trace target
         unroll_len=32,
```

### Comparing `DI-engine-0.4.7/dizoo/atari/config/serial/qbert/qbert_iqn_config.py` & `DI-engine-0.4.8/dizoo/atari/config/serial/qbert/qbert_iqn_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 qbert_iqn_config = dict(
     exp_name='qbert_dqn_seed0',
     env=dict(
         collector_env_num=8,
         evaluator_env_num=8,
         n_evaluator_episode=8,
         stop_value=30000,
-        env_id='Qbert-v4',
+        env_id='QbertNoFrameskip-v4',
         #'ALE/Qbert-v5' is available. But special setting is needed after gym make.
         frame_stack=4
     ),
     policy=dict(
         cuda=True,
         priority=True,
         model=dict(
```

### Comparing `DI-engine-0.4.7/dizoo/atari/config/serial/qbert/qbert_offppo_config.py` & `DI-engine-0.4.8/dizoo/atari/config/serial/qbert/qbert_offppo_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 qbert_offppo_config = dict(
     exp_name='qbert_offppo_seed0',
     env=dict(
         collector_env_num=16,
         evaluator_env_num=8,
         n_evaluator_episode=8,
         stop_value=10000000000,
-        env_id='Qbert-v4',
+        env_id='QbertNoFrameskip-v4',
         #'ALE/Qbert-v5' is available. But special setting is needed after gym make.
         frame_stack=4
     ),
     policy=dict(
         cuda=True,
         model=dict(
             obs_shape=[4, 84, 84],
```

### Comparing `DI-engine-0.4.7/dizoo/atari/config/serial/qbert/qbert_onppo_config.py` & `DI-engine-0.4.8/dizoo/atari/config/serial/qbert/qbert_onppo_config.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 qbert_onppo_config = dict(
     exp_name='enduro_onppo_seed0',
     env=dict(
         collector_env_num=16,
         evaluator_env_num=8,
         n_evaluator_episode=8,
         stop_value=int(1e10),
-        env_id='Qbert-v4',
+        env_id='QbertNoFrameskip-v4',
         #'ALE/Qbert-v5' is available. But special setting is needed after gym make.
         frame_stack=4
     ),
     policy=dict(
         cuda=True,
         recompute_adv=True,
         action_space='discrete',
```

### Comparing `DI-engine-0.4.7/dizoo/atari/config/serial/qbert/qbert_ppg_config.py` & `DI-engine-0.4.8/dizoo/atari/config/serial/qbert/qbert_ppg_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 qbert_ppg_config = dict(
     exp_name='qbert_ppg_seed0',
     env=dict(
         collector_env_num=8,
         evaluator_env_num=8,
         n_evaluator_episode=8,
         stop_value=1000000,
-        env_id='Qbert-v4',
+        env_id='QbertNoFrameskip-v4',
         #'ALE/Qbert-v5' is available. But special setting is needed after gym make.
         frame_stack=4
     ),
     policy=dict(
         cuda=True,
         model=dict(
             obs_shape=[4, 84, 84],
```

### Comparing `DI-engine-0.4.7/dizoo/atari/config/serial/qbert/qbert_qrdqn_config.py` & `DI-engine-0.4.8/dizoo/atari/config/serial/qbert/qbert_sql_config.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,59 +1,59 @@
 from easydict import EasyDict
 
-qbert_qrdqn_config = dict(
-    exp_name='qbert_qrdqn_seed0',
+qbert_sql_config = dict(
+    exp_name='qbert_sql_seed0',
     env=dict(
         collector_env_num=8,
         evaluator_env_num=8,
         n_evaluator_episode=8,
         stop_value=30000,
-        env_id='Qbert-v4',
+        env_id='QbertNoFrameskip-v4',
         #'ALE/Qbert-v5' is available. But special setting is needed after gym make.
         frame_stack=4
     ),
     policy=dict(
         cuda=True,
-        priority=True,
+        priority=False,
         model=dict(
             obs_shape=[4, 84, 84],
             action_shape=6,
             encoder_hidden_size_list=[128, 128, 512],
-            num_quantiles=64,
         ),
         nstep=3,
         discount_factor=0.99,
         learn=dict(
             update_per_collect=10,
             batch_size=32,
             learning_rate=0.0001,
             target_update_freq=500,
         ),
-        collect=dict(n_sample=100, ),
+        collect=dict(n_sample=100),
         eval=dict(evaluator=dict(eval_freq=4000, )),
         other=dict(
             eps=dict(
                 type='exp',
                 start=1.,
                 end=0.05,
-                decay=1000000,
+                decay=500000,
             ),
             replay_buffer=dict(replay_buffer_size=400000, ),
         ),
     ),
 )
-main_config = EasyDict(qbert_qrdqn_config)
-
-qbert_qrdqn_create_config = dict(
+qbert_sql_config = EasyDict(qbert_sql_config)
+main_config = qbert_sql_config
+qbert_sql_create_config = dict(
     env=dict(
         type='atari',
         import_names=['dizoo.atari.envs.atari_env'],
     ),
     env_manager=dict(type='subprocess'),
-    policy=dict(type='qrdqn'),
+    policy=dict(type='sql'),
 )
-create_config = EasyDict(qbert_qrdqn_create_config)
+qbert_sql_create_config = EasyDict(qbert_sql_create_config)
+create_config = qbert_sql_create_config
 
 if __name__ == '__main__':
-    # or you can enter ding -m serial -c qbert_qrdqn_config.py -s 0
+    # or you can enter ding -m serial -c qbert_sql_config.py -s 0
     from ding.entry import serial_pipeline
     serial_pipeline((main_config, create_config), seed=0)
```

### Comparing `DI-engine-0.4.7/dizoo/atari/config/serial/qbert/qbert_qrdqn_generation_data_config.py` & `DI-engine-0.4.8/dizoo/atari/config/serial/qbert/qbert_qrdqn_generation_data_config.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 qbert_qrdqn_config = dict(
     exp_name='qbert_qrdqn_generation_data_seed0',
     env=dict(
         collector_env_num=8,
         evaluator_env_num=8,
         n_evaluator_episode=8,
         stop_value=30000,
-        env_id='Qbert-v4',
+        env_id='QbertNoFrameskip-v4',
         #'ALE/Qbert-v5' is available. But special setting is needed after gym make.
         frame_stack=4
     ),
     policy=dict(
         cuda=True,
         priority=False,
         model=dict(
```

### Comparing `DI-engine-0.4.7/dizoo/atari/config/serial/qbert/qbert_r2d2_config.py` & `DI-engine-0.4.8/dizoo/atari/config/serial/qbert/qbert_r2d2_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 qbert_r2d2_config = dict(
     exp_name='qbert_r2d2_seed0',
     env=dict(
         collector_env_num=collector_env_num,
         evaluator_env_num=evaluator_env_num,
         n_evaluator_episode=evaluator_env_num,
         stop_value=int(1e6),
-        env_id='Qbert-v4',
+        env_id='QbertNoFrameskip-v4',
         #'ALE/Qbert-v5' is available. But special setting is needed after gym make.
         frame_stack=4
     ),
     policy=dict(
         cuda=True,
         priority=True,
         priority_IS_weight=True,
```

### Comparing `DI-engine-0.4.7/dizoo/atari/config/serial/qbert/qbert_r2d2_gtrxl_config.py` & `DI-engine-0.4.8/dizoo/atari/config/serial/qbert/qbert_r2d2_gtrxl_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 qbert_r2d2_gtrxl_config = dict(
     exp_name='qbert_r2d2_gtrxl_seed0',
     env=dict(
         collector_env_num=8,
         evaluator_env_num=8,
         n_evaluator_episode=8,
         stop_value=10000000000,
-        env_id='Qbert-v4',
+        env_id='QbertNoFrameskip-v4',
         #'ALE/Qbert-v5' is available. But special setting is needed after gym make.
         frame_stack=4
     ),
     policy=dict(
         cuda=True,
         priority=True,
         priority_IS_weight=True,
```

### Comparing `DI-engine-0.4.7/dizoo/atari/config/serial/qbert/qbert_rainbow_config.py` & `DI-engine-0.4.8/dizoo/atari/config/serial/qbert/qbert_rainbow_config.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 qbert_rainbow_config = dict(
     exp_name='qbert_rainbow_seed0',
     env=dict(
         collector_env_num=8,
         evaluator_env_num=8,
         n_evaluator_episode=8,
         stop_value=30000,
-        env_id='Qbert-v4',
+        env_id='QbertNoFrameskip-v4',
         #'ALE/Qbert-v5' is available. But special setting is needed after gym make.
         frame_stack=4
     ),
     policy=dict(
         cuda=True,
         priority=False,
         priority_IS_weight=False,
```

### Comparing `DI-engine-0.4.7/dizoo/atari/config/serial/qbert/qbert_sqil_config.py` & `DI-engine-0.4.8/dizoo/atari/config/serial/qbert/qbert_sqil_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 qbert_sqil_config = dict(
     exp_name='qbert_sqil_seed0',
     env=dict(
         collector_env_num=8,
         evaluator_env_num=8,
         n_evaluator_episode=8,
         stop_value=30000,
-        env_id='Qbert-v4',
+        env_id='QbertNoFrameskip-v4',
         #'ALE/Qbert-v5' is available. But special setting is needed after gym make.
         frame_stack=4
     ),
     policy=dict(
         cuda=True,
         priority=True,
         model=dict(
```

### Comparing `DI-engine-0.4.7/dizoo/atari/config/serial/qbert/qbert_sql_config.py` & `DI-engine-0.4.8/dizoo/mario/mario_dqn_config.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,59 +1,49 @@
 from easydict import EasyDict
 
-qbert_sql_config = dict(
-    exp_name='qbert_sql_seed0',
+mario_dqn_config = dict(
+    exp_name='mario_dqn_seed0',
     env=dict(
         collector_env_num=8,
         evaluator_env_num=8,
         n_evaluator_episode=8,
-        stop_value=30000,
-        env_id='Qbert-v4',
-        #'ALE/Qbert-v5' is available. But special setting is needed after gym make.
-        frame_stack=4
+        stop_value=100000,
+        replay_path='mario_dqn_seed0/video',
     ),
     policy=dict(
         cuda=True,
-        priority=False,
         model=dict(
             obs_shape=[4, 84, 84],
-            action_shape=6,
-            encoder_hidden_size_list=[128, 128, 512],
+            action_shape=2,
+            encoder_hidden_size_list=[128, 128, 256],
+            dueling=True,
         ),
         nstep=3,
         discount_factor=0.99,
         learn=dict(
             update_per_collect=10,
             batch_size=32,
             learning_rate=0.0001,
             target_update_freq=500,
         ),
-        collect=dict(n_sample=100),
-        eval=dict(evaluator=dict(eval_freq=4000, )),
+        collect=dict(n_sample=96, ),
+        eval=dict(evaluator=dict(eval_freq=2000, )),
         other=dict(
             eps=dict(
                 type='exp',
                 start=1.,
                 end=0.05,
-                decay=500000,
+                decay=250000,
             ),
-            replay_buffer=dict(replay_buffer_size=400000, ),
+            replay_buffer=dict(replay_buffer_size=100000, ),
         ),
     ),
 )
-qbert_sql_config = EasyDict(qbert_sql_config)
-main_config = qbert_sql_config
-qbert_sql_create_config = dict(
-    env=dict(
-        type='atari',
-        import_names=['dizoo.atari.envs.atari_env'],
-    ),
+mario_dqn_config = EasyDict(mario_dqn_config)
+main_config = mario_dqn_config
+mario_dqn_create_config = dict(
     env_manager=dict(type='subprocess'),
-    policy=dict(type='sql'),
+    policy=dict(type='dqn'),
 )
-qbert_sql_create_config = EasyDict(qbert_sql_create_config)
-create_config = qbert_sql_create_config
-
-if __name__ == '__main__':
-    # or you can enter ding -m serial -c qbert_sql_config.py -s 0
-    from ding.entry import serial_pipeline
-    serial_pipeline((main_config, create_config), seed=0)
+mario_dqn_create_config = EasyDict(mario_dqn_create_config)
+create_config = mario_dqn_create_config
+# you can run `python3 -u mario_dqn_main.py`
```

### Comparing `DI-engine-0.4.7/dizoo/atari/config/serial/qbert/qbert_trex_dqn_config.py` & `DI-engine-0.4.8/dizoo/atari/config/serial/qbert/qbert_trex_dqn_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 qbert_trex_dqn_config = dict(
     exp_name='qbert_trex_dqn_seed0',
     env=dict(
         collector_env_num=8,
         evaluator_env_num=8,
         n_evaluator_episode=8,
         stop_value=30000,
-        env_id='Qbert-v4',
+        env_id='QbertNoFrameskip-v4',
         #'ALE/Qbert-v5' is available. But special setting is needed after gym make.
         frame_stack=4
     ),
     reward_model=dict(
         type='trex',
         min_snippet_length=30,
         max_snippet_length=100,
```

### Comparing `DI-engine-0.4.7/dizoo/atari/config/serial/qbert/qbert_trex_offppo_config.py` & `DI-engine-0.4.8/dizoo/atari/config/serial/qbert/qbert_trex_offppo_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 qbert_trex_ppo_config = dict(
     exp_name='qbert_trex_offppo_seed0',
     env=dict(
         collector_env_num=16,
         evaluator_env_num=8,
         n_evaluator_episode=8,
         stop_value=10000000000,
-        env_id='Qbert-v4',
+        env_id='QbertNoFrameskip-v4',
         #'ALE/Qbert-v5' is available. But special setting is needed after gym make.
         frame_stack=4
     ),
     reward_model=dict(
         type='trex',
         min_snippet_length=30,
         max_snippet_length=100,
```

### Comparing `DI-engine-0.4.7/dizoo/atari/config/serial/spaceinvaders/spaceinvaders_a2c_config.py` & `DI-engine-0.4.8/dizoo/atari/config/serial/spaceinvaders/spaceinvaders_a2c_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 spaceinvaders_a2c_config = dict(
     exp_name='spaceinvaders_a2c_seed0',
     env=dict(
         collector_env_num=16,
         evaluator_env_num=8,
         n_evaluator_episode=8,
         stop_value=10000000000,
-        env_id='SpaceInvaders-v4',
+        env_id='SpaceInvadersNoFrameskip-v4',
         #'ALE/SpaceInvaders-v5' is available. But special setting is needed after gym make.
         frame_stack=4,
     ),
     policy=dict(
         cuda=True,
         model=dict(
             obs_shape=[4, 84, 84],
```

### Comparing `DI-engine-0.4.7/dizoo/atari/config/serial/spaceinvaders/spaceinvaders_acer_config.py` & `DI-engine-0.4.8/dizoo/atari/config/serial/spaceinvaders/spaceinvaders_acer_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 spaceinvaders_acer_config = dict(
     exp_name='spaceinvaders_acer_seed0',
     env=dict(
         collector_env_num=16,
         evaluator_env_num=8,
         n_evaluator_episode=8,
         stop_value=int(1e6),
-        env_id='SpaceInvaders-v4',
+        env_id='SpaceInvadersNoFrameskip-v4',
         #'ALE/SpaceInvaders-v5' is available. But special setting is needed after gym make.
         frame_stack=4,
         manager=dict(shared_memory=False, )
     ),
     policy=dict(
         cuda=True,
         priority=False,
```

### Comparing `DI-engine-0.4.7/dizoo/atari/config/serial/spaceinvaders/spaceinvaders_c51_config.py` & `DI-engine-0.4.8/dizoo/atari/config/serial/spaceinvaders/spaceinvaders_c51_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 spaceinvaders_c51_config = dict(
     exp_name='spaceinvaders_c51_seed0',
     env=dict(
         collector_env_num=8,
         evaluator_env_num=8,
         n_evaluator_episode=8,
         stop_value=10000000000,
-        env_id='SpaceInvaders-v4',
+        env_id='SpaceInvadersNoFrameskip-v4',
         #'ALE/SpaceInvaders-v5' is available. But special setting is needed after gym make.
         frame_stack=4,
         manager=dict(shared_memory=False, )
     ),
     policy=dict(
         cuda=True,
         priority=False,
```

### Comparing `DI-engine-0.4.7/dizoo/atari/config/serial/spaceinvaders/spaceinvaders_dqfd_config.py` & `DI-engine-0.4.8/dizoo/atari/config/serial/spaceinvaders/spaceinvaders_dqfd_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 spaceinvaders_dqfd_config = dict(
     exp_name='spaceinvaders_dqfd_seed0',
     env=dict(
         collector_env_num=8,
         evaluator_env_num=8,
         n_evaluator_episode=8,
         stop_value=10000000000,
-        env_id='SpaceInvaders-v4',
+        env_id='SpaceInvadersNoFrameskip-v4',
         #'ALE/SpaceInvaders-v5' is available. But special setting is needed after gym make.
         frame_stack=4,
     ),
     policy=dict(
         cuda=True,
         priority=True,
         model=dict(
```

### Comparing `DI-engine-0.4.7/dizoo/atari/config/serial/spaceinvaders/spaceinvaders_dqn_config.py` & `DI-engine-0.4.8/dizoo/atari/config/serial/spaceinvaders/spaceinvaders_dqn_config.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 spaceinvaders_dqn_config = dict(
     exp_name='spaceinvaders_dqn_seed0',
     env=dict(
         collector_env_num=8,
         evaluator_env_num=8,
         n_evaluator_episode=8,
         stop_value=10000000000,
-        env_id='SpaceInvaders-v4',
+        env_id='SpaceInvadersNoFrameskip-v4',
         #'ALE/SpaceInvaders-v5' is available. But special setting is needed after gym make.
         frame_stack=4,
         manager=dict(shared_memory=False, ),
         # The path to save the game replay
         replay_path='./spaceinvaders_dqn_seed0/video',
     ),
     policy=dict(
```

### Comparing `DI-engine-0.4.7/dizoo/atari/config/serial/spaceinvaders/spaceinvaders_dqn_config_multi_gpu_ddp.py` & `DI-engine-0.4.8/dizoo/atari/config/serial/spaceinvaders/spaceinvaders_dqn_config_multi_gpu_ddp.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 spaceinvaders_dqn_config = dict(
     exp_name='spaceinvaders_dqn_multi_gpu_ddp_seed0',
     env=dict(
         collector_env_num=8,
         evaluator_env_num=8,
         n_evaluator_episode=8,
         stop_value=10000000000,
-        env_id='SpaceInvaders-v4',
+        env_id='SpaceInvadersNoFrameskip-v4',
         #'ALE/SpaceInvaders-v5' is available. But special setting is needed after gym make.
         frame_stack=4,
         manager=dict(shared_memory=False, )
     ),
     policy=dict(
         cuda=True,
         multi_gpu=True,
```

### Comparing `DI-engine-0.4.7/dizoo/atari/config/serial/spaceinvaders/spaceinvaders_dqn_config_multi_gpu_dp.py` & `DI-engine-0.4.8/dizoo/atari/config/serial/spaceinvaders/spaceinvaders_dqn_config_multi_gpu_dp.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 spaceinvaders_dqn_config = dict(
     exp_name='spaceinvaders_dqn_multi_gpu_dp_seed0',
     env=dict(
         collector_env_num=8,
         evaluator_env_num=8,
         n_evaluator_episode=8,
         stop_value=10000000000,
-        env_id='SpaceInvaders-v4',
+        env_id='SpaceInvadersNoFrameskip-v4',
         #'ALE/SpaceInvaders-v5' is available. But special setting is needed after gym make.
         frame_stack=4,
         manager=dict(shared_memory=False, )
     ),
     policy=dict(
         cuda=True,
         priority=False,
```

### Comparing `DI-engine-0.4.7/dizoo/atari/config/serial/spaceinvaders/spaceinvaders_fqf_config.py` & `DI-engine-0.4.8/dizoo/atari/config/serial/spaceinvaders/spaceinvaders_fqf_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 spaceinvaders_fqf_config = dict(
     exp_name='spaceinvaders_fqf_seed0',
     env=dict(
         collector_env_num=8,
         evaluator_env_num=8,
         n_evaluator_episode=8,
         stop_value=10000000000,
-        env_id='SpaceInvaders-v4',
+        env_id='SpaceInvadersNoFrameskip-v4',
         #'ALE/SpaceInvaders-v5' is available. But special setting is needed after gym make.
         frame_stack=4,
     ),
     policy=dict(
         cuda=True,
         priority=False,
         model=dict(
```

### Comparing `DI-engine-0.4.7/dizoo/atari/config/serial/spaceinvaders/spaceinvaders_impala_config.py` & `DI-engine-0.4.8/dizoo/atari/config/serial/spaceinvaders/spaceinvaders_impala_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 spaceinvaders_impala_config = dict(
     exp_name='spaceinvaders_impala_seed0',
     env=dict(
         collector_env_num=8,
         evaluator_env_num=8,
         n_evaluator_episode=8,
         stop_value=10000000000,
-        env_id='SpaceInvaders-v4',
+        env_id='SpaceInvadersNoFrameskip-v4',
         #'ALE/SpaceInvaders-v5' is available. But special setting is needed after gym make.
         frame_stack=4,
         manager=dict(shared_memory=False, )
     ),
     policy=dict(
         cuda=True,
         # (int) the trajectory length to calculate v-trace target
```

### Comparing `DI-engine-0.4.7/dizoo/atari/config/serial/spaceinvaders/spaceinvaders_iqn_config.py` & `DI-engine-0.4.8/dizoo/atari/config/serial/spaceinvaders/spaceinvaders_iqn_config.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 spaceinvaders_iqn_config = dict(
     exp_name='spaceinvaders_iqn_seed0',
     env=dict(
         collector_env_num=8,
         evaluator_env_num=8,
         n_evaluator_episode=8,
         stop_value=10000000000,
-        env_id='SpaceInvaders-v4',
+        env_id='SpaceInvadersNoFrameskip-v4',
         #'ALE/SpaceInvaders-v5' is available. But special setting is needed after gym make.
         frame_stack=4,
         manager=dict(shared_memory=False, )
     ),
     policy=dict(
         cuda=True,
         priority=False,
```

### Comparing `DI-engine-0.4.7/dizoo/atari/config/serial/spaceinvaders/spaceinvaders_mdqn_config.py` & `DI-engine-0.4.8/dizoo/atari/config/serial/spaceinvaders/spaceinvaders_mdqn_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 spaceinvaders_mdqn_config = dict(
     exp_name='spaceinvaders_mdqn_seed0',
     env=dict(
         collector_env_num=8,
         evaluator_env_num=8,
         n_evaluator_episode=8,
         stop_value=10000,
-        env_id='SpaceInvaders-v0',
+        env_id='SpaceInvadersNoFrameskip-v0',
         #'ALE/SpaceInvaders-v5' is available. But special setting is needed after gym make.
         frame_stack=4,
     ),
     policy=dict(
         cuda=True,
         priority=False,
         model=dict(
```

### Comparing `DI-engine-0.4.7/dizoo/atari/config/serial/spaceinvaders/spaceinvaders_offppo_config.py` & `DI-engine-0.4.8/dizoo/atari/config/serial/spaceinvaders/spaceinvaders_offppo_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 spaceinvaders_ppo_config = dict(
     exp_name='spaceinvaders_offppo_seed0',
     env=dict(
         collector_env_num=16,
         evaluator_env_num=8,
         n_evaluator_episode=8,
         stop_value=10000000000,
-        env_id='SpaceInvaders-v4',
+        env_id='SpaceInvadersNoFrameskip-v4',
         #'ALE/SpaceInvaders-v5' is available. But special setting is needed after gym make.
         frame_stack=4,
         manager=dict(shared_memory=False, )
     ),
     policy=dict(
         cuda=True,
         model=dict(
```

### Comparing `DI-engine-0.4.7/dizoo/atari/config/serial/spaceinvaders/spaceinvaders_onppo_config.py` & `DI-engine-0.4.8/dizoo/atari/config/serial/spaceinvaders/spaceinvaders_onppo_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 spaceinvaders_ppo_config = dict(
     exp_name='spaceinvaders_onppo_seed0',
     env=dict(
         collector_env_num=16,
         evaluator_env_num=8,
         n_evaluator_episode=8,
         stop_value=int(1e10),
-        env_id='SpaceInvaders-v4',
+        env_id='SpaceInvadersNoFrameskip-v4',
         #'ALE/SpaceInvaders-v5' is available. But special setting is needed after gym make.
         frame_stack=4,
         manager=dict(shared_memory=False, )
     ),
     policy=dict(
         cuda=True,
         recompute_adv=True,
```

### Comparing `DI-engine-0.4.7/dizoo/atari/config/serial/spaceinvaders/spaceinvaders_ppg_config.py` & `DI-engine-0.4.8/dizoo/atari/config/serial/spaceinvaders/spaceinvaders_ppg_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 spaceinvaders_ppg_config = dict(
     exp_name='spaceinvaders_ppg_seed0',
     env=dict(
         collector_env_num=16,
         evaluator_env_num=8,
         n_evaluator_episode=8,
         stop_value=10000000000,
-        env_id='SpaceInvaders-v4',
+        env_id='SpaceInvadersNoFrameskip-v4',
         #'ALE/SpaceInvaders-v5' is available. But special setting is needed after gym make.
         frame_stack=4,
         manager=dict(shared_memory=False, )
     ),
     policy=dict(
         cuda=True,
         model=dict(
```

### Comparing `DI-engine-0.4.7/dizoo/atari/config/serial/spaceinvaders/spaceinvaders_qrdqn_config.py` & `DI-engine-0.4.8/dizoo/atari/config/serial/spaceinvaders/spaceinvaders_qrdqn_config.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 spaceinvaders_qrdqn_config = dict(
     exp_name='spaceinvaders_qrdqn_seed0',
     env=dict(
         collector_env_num=8,
         evaluator_env_num=8,
         n_evaluator_episode=8,
         stop_value=10000000000,
-        env_id='SpaceInvaders-v4',
+        env_id='SpaceInvadersNoFrameskip-v4',
         #'ALE/SpaceInvaders-v5' is available. But special setting is needed after gym make.
         frame_stack=4,
         manager=dict(shared_memory=False, )
     ),
     policy=dict(
         cuda=True,
         priority=False,
```

### Comparing `DI-engine-0.4.7/dizoo/atari/config/serial/spaceinvaders/spaceinvaders_r2d2_config.py` & `DI-engine-0.4.8/dizoo/atari/config/serial/spaceinvaders/spaceinvaders_r2d2_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 spaceinvaders_r2d2_config = dict(
     exp_name='spaceinvaders_r2d2_seed0',
     env=dict(
         collector_env_num=collector_env_num,
         evaluator_env_num=evaluator_env_num,
         n_evaluator_episode=8,
         stop_value=int(1e6),
-        env_id='SpaceInvaders-v4',
+        env_id='SpaceInvadersNoFrameskip-v4',
         #'ALE/SpaceInvaders-v5' is available. But special setting is needed after gym make.
         frame_stack=4,
         manager=dict(shared_memory=False, )
     ),
     policy=dict(
         cuda=True,
         priority=True,
```

### Comparing `DI-engine-0.4.7/dizoo/atari/config/serial/spaceinvaders/spaceinvaders_r2d2_gtrxl_config.py` & `DI-engine-0.4.8/dizoo/atari/config/serial/spaceinvaders/spaceinvaders_r2d2_gtrxl_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 spaceinvaders_r2d2_gtrxl_config = dict(
     exp_name='spaceinvaders_r2d2_gtrxl_seed0',
     env=dict(
         collector_env_num=8,
         evaluator_env_num=8,
         n_evaluator_episode=8,
         stop_value=10000000000,
-        env_id='SpaceInvaders-v4',
+        env_id='SpaceInvadersNoFrameskip-v4',
         #'ALE/SpaceInvaders-v5' is available. But special setting is needed after gym make.
         frame_stack=4,
         manager=dict(shared_memory=False)
     ),
     policy=dict(
         cuda=True,
         priority=True,
```

### Comparing `DI-engine-0.4.7/dizoo/atari/config/serial/spaceinvaders/spaceinvaders_r2d2_residual_config.py` & `DI-engine-0.4.8/dizoo/atari/config/serial/spaceinvaders/spaceinvaders_r2d2_residual_config.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 spaceinvaders_r2d2_residual_config = dict(
     exp_name='spaceinvaders_r2d2_residual_link_seed0',
     env=dict(
         collector_env_num=collector_env_num,
         evaluator_env_num=evaluator_env_num,
         n_evaluator_episode=8,
         stop_value=10000000000,
-        env_id='SpaceInvaders-v4',
+        env_id='SpaceInvadersNoFrameskip-v4',
         #'ALE/SpaceInvaders-v5' is available. But special setting is needed after gym make.
         frame_stack=4,
         manager=dict(shared_memory=False, )
     ),
     policy=dict(
         cuda=True,
         priority=False,
```

### Comparing `DI-engine-0.4.7/dizoo/atari/config/serial/spaceinvaders/spaceinvaders_rainbow_config.py` & `DI-engine-0.4.8/dizoo/atari/config/serial/spaceinvaders/spaceinvaders_rainbow_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 spaceinvaders_rainbow_config = dict(
     exp_name='spaceinvaders_rainbow_seed0',
     env=dict(
         collector_env_num=8,
         evaluator_env_num=8,
         n_evaluator_episode=8,
         stop_value=10000000000,
-        env_id='SpaceInvaders-v4',
+        env_id='SpaceInvadersNoFrameskip-v4',
         #'ALE/SpaceInvaders-v5' is available. But special setting is needed after gym make.
         frame_stack=4,
         manager=dict(shared_memory=False, )
     ),
     policy=dict(
         cuda=True,
         priority=False,
```

### Comparing `DI-engine-0.4.7/dizoo/atari/config/serial/spaceinvaders/spaceinvaders_sqil_config.py` & `DI-engine-0.4.8/dizoo/atari/config/serial/spaceinvaders/spaceinvaders_sqil_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 spaceinvaders_sqil_config = dict(
     exp_name='spaceinvaders_sqil_seed0',
     env=dict(
         collector_env_num=8,
         evaluator_env_num=8,
         n_evaluator_episode=8,
         stop_value=10000000000,
-        env_id='SpaceInvaders-v4',
+        env_id='SpaceInvadersNoFrameskip-v4',
         #'ALE/SpaceInvaders-v5' is available. But special setting is needed after gym make.
         frame_stack=4,
     ),
     policy=dict(
         cuda=True,
         priority=True,
         model=dict(
```

### Comparing `DI-engine-0.4.7/dizoo/atari/config/serial/spaceinvaders/spaceinvaders_sql_config.py` & `DI-engine-0.4.8/dizoo/atari/config/serial/spaceinvaders/spaceinvaders_sql_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 spaceinvaders_sql_config = dict(
     exp_name='spaceinvaders_sql_seed0',
     env=dict(
         collector_env_num=8,
         evaluator_env_num=8,
         n_evaluator_episode=8,
         stop_value=10000000000,
-        env_id='SpaceInvaders-v4',
+        env_id='SpaceInvadersNoFrameskip-v4',
         #'ALE/SpaceInvaders-v5' is available. But special setting is needed after gym make.
         frame_stack=4,
         manager=dict(shared_memory=False, reset_inplace=True)
     ),
     policy=dict(
         cuda=True,
         priority=False,
```

### Comparing `DI-engine-0.4.7/dizoo/atari/config/serial/spaceinvaders/spaceinvaders_trex_dqn_config.py` & `DI-engine-0.4.8/dizoo/atari/config/serial/spaceinvaders/spaceinvaders_trex_dqn_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 spaceinvaders_trex_dqn_config = dict(
     exp_name='spaceinvaders_trex_dqn_seed0',
     env=dict(
         collector_env_num=8,
         evaluator_env_num=8,
         n_evaluator_episode=8,
         stop_value=10000000000,
-        env_id='SpaceInvaders-v4',
+        env_id='SpaceInvadersNoFrameskip-v4',
         #'ALE/SpaceInvaders-v5' is available. But special setting is needed after gym make.
         frame_stack=4,
         manager=dict(shared_memory=False, )
     ),
     reward_model=dict(
         type='trex',
         min_snippet_length=50,
```

### Comparing `DI-engine-0.4.7/dizoo/atari/config/serial/spaceinvaders/spaceinvaders_trex_offppo_config.py` & `DI-engine-0.4.8/dizoo/atari/config/serial/spaceinvaders/spaceinvaders_trex_offppo_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 spaceinvaders_trex_ppo_config = dict(
     exp_name='spaceinvaders_trex_offppo_seed0',
     env=dict(
         collector_env_num=16,
         evaluator_env_num=8,
         n_evaluator_episode=8,
         stop_value=10000000000,
-        env_id='SpaceInvaders-v4',
+        env_id='SpaceInvadersNoFrameskip-v4',
         #'ALE/SpaceInvaders-v5' is available. But special setting is needed after gym make.
         frame_stack=4,
         manager=dict(shared_memory=False, )
     ),
     reward_model=dict(
         type='trex',
         min_snippet_length=30,
```

### Comparing `DI-engine-0.4.7/dizoo/atari/entry/atari_dqn_main.py` & `DI-engine-0.4.8/dizoo/atari/entry/atari_dqn_main.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/atari/entry/atari_ppg_main.py` & `DI-engine-0.4.8/dizoo/atari/entry/atari_ppg_main.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/atari/entry/phoenix_fqf_main.py` & `DI-engine-0.4.8/dizoo/atari/entry/phoenix_fqf_main.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/atari/entry/phoenix_iqn_main.py` & `DI-engine-0.4.8/dizoo/atari/entry/phoenix_iqn_main.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/atari/entry/pong_cql_main.py` & `DI-engine-0.4.8/dizoo/atari/entry/pong_cql_main.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/atari/entry/pong_dqn_envpool_main.py` & `DI-engine-0.4.8/dizoo/atari/entry/pong_dqn_envpool_main.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/atari/entry/pong_fqf_main.py` & `DI-engine-0.4.8/dizoo/atari/entry/pong_fqf_main.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/atari/entry/qbert_cql_main.py` & `DI-engine-0.4.8/dizoo/atari/entry/qbert_cql_main.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/atari/entry/qbert_fqf_main.py` & `DI-engine-0.4.8/dizoo/atari/entry/qbert_fqf_main.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/atari/entry/spaceinvaders_dqn_eval.py` & `DI-engine-0.4.8/dizoo/atari/entry/spaceinvaders_dqn_eval.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/atari/entry/spaceinvaders_dqn_main_multi_gpu_ddp.py` & `DI-engine-0.4.8/dizoo/atari/entry/spaceinvaders_dqn_main_multi_gpu_ddp.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/atari/entry/spaceinvaders_dqn_main_multi_gpu_dp.py` & `DI-engine-0.4.8/dizoo/atari/entry/spaceinvaders_dqn_main_multi_gpu_dp.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/atari/entry/spaceinvaders_fqf_main.py` & `DI-engine-0.4.8/dizoo/atari/entry/spaceinvaders_fqf_main.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/atari/envs/atari_env.py` & `DI-engine-0.4.8/dizoo/atari/envs/atari_env.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/atari/envs/atari_wrappers.py` & `DI-engine-0.4.8/dizoo/atari/envs/atari_wrappers.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/atari/envs/test_atari_env.py` & `DI-engine-0.4.8/dizoo/atari/envs/test_atari_env.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/beergame/envs/BGAgent.py` & `DI-engine-0.4.8/dizoo/beergame/envs/BGAgent.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/beergame/envs/beergame_core.py` & `DI-engine-0.4.8/dizoo/beergame/envs/beergame_core.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/beergame/envs/beergame_env.py` & `DI-engine-0.4.8/dizoo/beergame/envs/beergame_env.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/beergame/envs/clBeergame.py` & `DI-engine-0.4.8/dizoo/beergame/envs/clBeergame.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/beergame/envs/plotting.py` & `DI-engine-0.4.8/dizoo/beergame/envs/plotting.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/beergame/envs/utils.py` & `DI-engine-0.4.8/dizoo/beergame/envs/utils.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/bitflip/config/bitflip_her_dqn_config.py` & `DI-engine-0.4.8/dizoo/bitflip/config/bitflip_her_dqn_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/bitflip/config/bitflip_pure_dqn_config.py` & `DI-engine-0.4.8/dizoo/bitflip/config/bitflip_pure_dqn_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/bitflip/entry/bitflip_dqn_main.py` & `DI-engine-0.4.8/dizoo/bitflip/entry/bitflip_dqn_main.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/bitflip/envs/bitflip_env.py` & `DI-engine-0.4.8/dizoo/bitflip/envs/bitflip_env.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/bitflip/envs/test_bitfilp_env.py` & `DI-engine-0.4.8/dizoo/bitflip/envs/test_bitfilp_env.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/box2d/bipedalwalker/config/bipedalwalker_bco_config.py` & `DI-engine-0.4.8/dizoo/box2d/bipedalwalker/config/bipedalwalker_bco_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/box2d/bipedalwalker/config/bipedalwalker_dt_config.py` & `DI-engine-0.4.8/dizoo/box2d/bipedalwalker/config/bipedalwalker_dt_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/box2d/bipedalwalker/config/bipedalwalker_gail_sac_config.py` & `DI-engine-0.4.8/dizoo/box2d/bipedalwalker/config/bipedalwalker_gail_sac_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/box2d/bipedalwalker/config/bipedalwalker_impala_config.py` & `DI-engine-0.4.8/dizoo/box2d/bipedalwalker/config/bipedalwalker_impala_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/box2d/bipedalwalker/config/bipedalwalker_ppo_config.py` & `DI-engine-0.4.8/dizoo/box2d/bipedalwalker/config/bipedalwalker_ppo_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/box2d/bipedalwalker/config/bipedalwalker_ppopg_config.py` & `DI-engine-0.4.8/dizoo/box2d/bipedalwalker/config/bipedalwalker_ppopg_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/box2d/bipedalwalker/config/bipedalwalker_sac_config.py` & `DI-engine-0.4.8/dizoo/box2d/bipedalwalker/config/bipedalwalker_sac_config.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,68 +1,63 @@
 from easydict import EasyDict
 
 bipedalwalker_sac_config = dict(
-    exp_name='bipedalwalker_sac_seed0',
+    exp_name='bipedalwalker_sac_config0',
     env=dict(
         env_id='BipedalWalker-v3',
         collector_env_num=8,
         evaluator_env_num=5,
         # (bool) Scale output action into legal range.
         act_scale=True,
         n_evaluator_episode=5,
-        stop_value=300,
         rew_clip=True,
-        # The path to save the game replay
-        replay_path=None,
     ),
     policy=dict(
-        cuda=False,
-        priority=False,
-        random_collect_size=1000,
+        cuda=True,
+        random_collect_size=10000,
         model=dict(
             obs_shape=24,
             action_shape=4,
             twin_critic=True,
             action_space='reparameterization',
             actor_head_hidden_size=128,
             critic_head_hidden_size=128,
         ),
         learn=dict(
-            update_per_collect=1,
-            batch_size=128,
-            learning_rate_q=0.001,
-            learning_rate_policy=0.001,
+            update_per_collect=64,
+            batch_size=256,
+            learning_rate_q=0.0003,
+            learning_rate_policy=0.0003,
             learning_rate_alpha=0.0003,
-            ignore_done=True,
             target_theta=0.005,
             discount_factor=0.99,
             auto_alpha=True,
-            value_network=False,
+            learner=dict(
+                hook=dict(log_show_after_iter=1000, )
+            )
         ),
         collect=dict(
-            n_sample=128,
-            unroll_len=1,
+            n_sample=64,
         ),
-        other=dict(replay_buffer=dict(replay_buffer_size=100000, ), ),
+        other=dict(replay_buffer=dict(replay_buffer_size=300000, ), ),
     ),
 )
 bipedalwalker_sac_config = EasyDict(bipedalwalker_sac_config)
 main_config = bipedalwalker_sac_config
 bipedalwalker_sac_create_config = dict(
     env=dict(
         type='bipedalwalker',
         import_names=['dizoo.box2d.bipedalwalker.envs.bipedalwalker_env'],
     ),
     env_manager=dict(type='subprocess'),
     policy=dict(
         type='sac',
-        import_names=['ding.policy.sac'],
     ),
     replay_buffer=dict(type='naive', ),
 )
 bipedalwalker_sac_create_config = EasyDict(bipedalwalker_sac_create_config)
 create_config = bipedalwalker_sac_create_config
 
 if __name__ == "__main__":
     # or you can enter `ding -m serial -c bipedalwalker_sac_config.py -s 0`
     from ding.entry import serial_pipeline
-    serial_pipeline([main_config, create_config], seed=0)
+    serial_pipeline([main_config, create_config], seed=0, max_env_step=int(1e5))
```

### Comparing `DI-engine-0.4.7/dizoo/box2d/bipedalwalker/config/bipedalwalker_td3_config.py` & `DI-engine-0.4.8/dizoo/box2d/bipedalwalker/config/bipedalwalker_td3_config.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,57 +1,53 @@
 from easydict import EasyDict
 
 bipedalwalker_td3_config = dict(
     exp_name='bipedalwalker_td3_seed0',
     env=dict(
         env_id='BipedalWalker-v3',
-        collector_env_num=1,
+        collector_env_num=8,
         evaluator_env_num=5,
         # (bool) Scale output action into legal range.
         act_scale=True,
         n_evaluator_episode=5,
-        stop_value=300,
         rew_clip=True,
-        # The path to save the game replay
-        replay_path=None,
     ),
     policy=dict(
         cuda=True,
-        priority=False,
+        random_collect_size=10000,
         model=dict(
             obs_shape=24,
             action_shape=4,
             twin_critic=True,
+            action_space='regression',
             actor_head_hidden_size=400,
             critic_head_hidden_size=400,
-            action_space='regression',
         ),
         learn=dict(
-            update_per_collect=4,
-            discount_factor=0.99,
-            batch_size=128,
-            learning_rate_actor=0.001,
-            learning_rate_critic=0.001,
+            update_per_collect=64,
+            batch_size=256,
+            learning_rate_actor=0.0003,
+            learning_rate_critic=0.0003,
             target_theta=0.005,
-            ignore_done=False,
+            discount_factor=0.99,
             actor_update_freq=2,
             noise=True,
             noise_sigma=0.2,
             noise_range=dict(
                 min=-0.5,
                 max=0.5,
             ),
+            learner=dict(
+                hook=dict(log_show_after_iter=1000, )
+            )
         ),
         collect=dict(
-            n_sample=256,
-            noise_sigma=0.1,
-            collector=dict(collect_print_freq=1000, ),
+            n_sample=64,
         ),
-        eval=dict(evaluator=dict(eval_freq=100, ), ),
-        other=dict(replay_buffer=dict(replay_buffer_size=50000, ), ),
+        other=dict(replay_buffer=dict(replay_buffer_size=300000, ), ),
     ),
 )
 bipedalwalker_td3_config = EasyDict(bipedalwalker_td3_config)
 main_config = bipedalwalker_td3_config
 
 bipedalwalker_td3_create_config = dict(
     env=dict(
@@ -63,8 +59,8 @@
 )
 bipedalwalker_td3_create_config = EasyDict(bipedalwalker_td3_create_config)
 create_config = bipedalwalker_td3_create_config
 
 if __name__ == "__main__":
     # or you can enter `ding -m serial -c bipedalwalker_td3_config.py -s 0`
     from ding.entry import serial_pipeline
-    serial_pipeline([main_config, create_config], seed=0)
+    serial_pipeline([main_config, create_config], seed=0, max_env_step=int(1e5))
```

### Comparing `DI-engine-0.4.7/dizoo/box2d/bipedalwalker/entry/bipedalwalker_ppo_eval.py` & `DI-engine-0.4.8/dizoo/box2d/bipedalwalker/entry/bipedalwalker_ppo_eval.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/box2d/bipedalwalker/envs/bipedalwalker_env.py` & `DI-engine-0.4.8/dizoo/box2d/bipedalwalker/envs/bipedalwalker_env.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/box2d/bipedalwalker/envs/test_bipedalwalker.py` & `DI-engine-0.4.8/dizoo/box2d/bipedalwalker/envs/test_bipedalwalker.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/box2d/carracing/config/carracing_dqn_config.py` & `DI-engine-0.4.8/dizoo/classic_control/acrobot/config/acrobot_dqn_config.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,63 +1,55 @@
 from easydict import EasyDict
 
-nstep = 3
-carracing_dqn_config = dict(
-    exp_name='carracing_dqn_seed0',
+acrobot_dqn_config = dict(
+    exp_name='acrobot_dqn_seed0',
     env=dict(
         collector_env_num=8,
         evaluator_env_num=8,
-        env_id='CarRacing-v2',
-        continuous=False,
         n_evaluator_episode=8,
-        stop_value=900,
-        # replay_path='./carracing_dqn_seed0/video',
+        stop_value=-60,
+        env_id='Acrobot-v1',
+        replay_path='acrobot_dqn_seed0/video',
     ),
     policy=dict(
         cuda=True,
-        # load_path='carracing_dqn_seed0/ckpt/ckpt_best.pth.tar',
         model=dict(
-            obs_shape=[3, 96, 96],
-            action_shape=5,
-            encoder_hidden_size_list=[64, 64, 128],
+            obs_shape=6,
+            action_shape=3,
+            encoder_hidden_size_list=[256, 256],
             dueling=True,
         ),
+        nstep=3,
         discount_factor=0.99,
-        nstep=nstep,
         learn=dict(
             update_per_collect=10,
-            batch_size=64,
+            batch_size=128,
             learning_rate=0.0001,
-            target_update_freq=100,
-        ),
-        collect=dict(
-            n_sample=64,
+            target_update_freq=250,
         ),
+        collect=dict(n_sample=96, ),
+        eval=dict(evaluator=dict(eval_freq=2000, )),
         other=dict(
             eps=dict(
                 type='exp',
-                start=0.95,
-                end=0.1,
-                decay=50000,
+                start=1.,
+                end=0.05,
+                decay=250000,
             ),
-            replay_buffer=dict(replay_buffer_size=100000, )
+            replay_buffer=dict(replay_buffer_size=100000, ),
         ),
     ),
 )
-carracing_dqn_config = EasyDict(carracing_dqn_config)
-main_config = carracing_dqn_config
-
-carracing_dqn_create_config = dict(
-    env=dict(
-        type='carracing',
-        import_names=['dizoo.box2d.carracing.envs.carracing_env'],
-    ),
+acrobot_dqn_config = EasyDict(acrobot_dqn_config)
+main_config = acrobot_dqn_config
+acrobot_dqn_create_config = dict(
+    env=dict(type='acrobot', import_names=['dizoo.classic_control.acrobot.envs.acrobot_env']),
     env_manager=dict(type='subprocess'),
     policy=dict(type='dqn'),
+    replay_buffer=dict(type='deque', import_names=['ding.data.buffer.deque_buffer_wrapper']),
 )
-carracing_dqn_create_config = EasyDict(carracing_dqn_create_config)
-create_config = carracing_dqn_create_config
+acrobot_dqn_create_config = EasyDict(acrobot_dqn_create_config)
+create_config = acrobot_dqn_create_config
 
 if __name__ == "__main__":
-    # or you can enter `ding -m serial -c carracing_dqn_config.py -s 0`
     from ding.entry import serial_pipeline
-    serial_pipeline([main_config, create_config], seed=0)
+    serial_pipeline((main_config, create_config), seed=0)
```

### Comparing `DI-engine-0.4.7/dizoo/box2d/carracing/envs/carracing_env.py` & `DI-engine-0.4.8/dizoo/box2d/carracing/envs/carracing_env.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/box2d/carracing/envs/test_carracing_env.py` & `DI-engine-0.4.8/dizoo/box2d/carracing/envs/test_carracing_env.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/box2d/lunarlander/config/__init__.py` & `DI-engine-0.4.8/dizoo/box2d/lunarlander/config/__init__.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/box2d/lunarlander/config/lunarlander_a2c_config.py` & `DI-engine-0.4.8/dizoo/box2d/lunarlander/config/lunarlander_a2c_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/box2d/lunarlander/config/lunarlander_acer_config.py` & `DI-engine-0.4.8/dizoo/box2d/lunarlander/config/lunarlander_acer_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/box2d/lunarlander/config/lunarlander_bco_config.py` & `DI-engine-0.4.8/dizoo/box2d/lunarlander/config/lunarlander_bco_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/box2d/lunarlander/config/lunarlander_c51_config.py` & `DI-engine-0.4.8/dizoo/box2d/lunarlander/config/lunarlander_c51_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/box2d/lunarlander/config/lunarlander_cont_ddpg_config.py` & `DI-engine-0.4.8/dizoo/box2d/lunarlander/config/lunarlander_cont_ddpg_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/box2d/lunarlander/config/lunarlander_cont_sac_config.py` & `DI-engine-0.4.8/dizoo/box2d/lunarlander/config/lunarlander_cont_sac_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/box2d/lunarlander/config/lunarlander_cont_td3_config.py` & `DI-engine-0.4.8/dizoo/box2d/lunarlander/config/lunarlander_cont_td3_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/box2d/lunarlander/config/lunarlander_cont_td3_vae_config.py` & `DI-engine-0.4.8/dizoo/box2d/lunarlander/config/lunarlander_cont_td3_vae_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/box2d/lunarlander/config/lunarlander_decision_transformer.py` & `DI-engine-0.4.8/dizoo/box2d/lunarlander/config/lunarlander_decision_transformer.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/box2d/lunarlander/config/lunarlander_discrete_sac_config.py` & `DI-engine-0.4.8/dizoo/box2d/lunarlander/config/lunarlander_discrete_sac_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/box2d/lunarlander/config/lunarlander_dqfd_config.py` & `DI-engine-0.4.8/dizoo/box2d/lunarlander/config/lunarlander_dqfd_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/box2d/lunarlander/config/lunarlander_dqn_config.py` & `DI-engine-0.4.8/dizoo/box2d/lunarlander/config/lunarlander_dqn_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/box2d/lunarlander/config/lunarlander_dqn_deque_config.py` & `DI-engine-0.4.8/dizoo/box2d/lunarlander/config/lunarlander_dqn_deque_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/box2d/lunarlander/config/lunarlander_gail_dqn_config.py` & `DI-engine-0.4.8/dizoo/box2d/lunarlander/config/lunarlander_gail_dqn_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/box2d/lunarlander/config/lunarlander_gcl_config.py` & `DI-engine-0.4.8/dizoo/box2d/lunarlander/config/lunarlander_gcl_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/box2d/lunarlander/config/lunarlander_ngu_config.py` & `DI-engine-0.4.8/dizoo/box2d/lunarlander/config/lunarlander_ngu_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/box2d/lunarlander/config/lunarlander_offppo_config.py` & `DI-engine-0.4.8/dizoo/box2d/lunarlander/config/lunarlander_offppo_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/box2d/lunarlander/config/lunarlander_pg_config.py` & `DI-engine-0.4.8/dizoo/box2d/lunarlander/config/lunarlander_pg_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/box2d/lunarlander/config/lunarlander_qrdqn_config.py` & `DI-engine-0.4.8/dizoo/box2d/lunarlander/config/lunarlander_qrdqn_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/box2d/lunarlander/config/lunarlander_r2d2_config.py` & `DI-engine-0.4.8/dizoo/box2d/lunarlander/config/lunarlander_r2d2_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/box2d/lunarlander/config/lunarlander_r2d2_gtrxl_config.py` & `DI-engine-0.4.8/dizoo/box2d/lunarlander/config/lunarlander_r2d2_gtrxl_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/box2d/lunarlander/config/lunarlander_r2d3_ppoexpert_config.py` & `DI-engine-0.4.8/dizoo/box2d/lunarlander/config/lunarlander_r2d3_ppoexpert_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/box2d/lunarlander/config/lunarlander_r2d3_r2d2expert_config.py` & `DI-engine-0.4.8/dizoo/box2d/lunarlander/config/lunarlander_r2d3_r2d2expert_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/box2d/lunarlander/config/lunarlander_rnd_onppo_config.py` & `DI-engine-0.4.8/dizoo/box2d/lunarlander/config/lunarlander_rnd_onppo_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/box2d/lunarlander/config/lunarlander_sqil_config.py` & `DI-engine-0.4.8/dizoo/box2d/lunarlander/config/lunarlander_sqil_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/box2d/lunarlander/config/lunarlander_sql_config.py` & `DI-engine-0.4.8/dizoo/box2d/lunarlander/config/lunarlander_sql_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/box2d/lunarlander/config/lunarlander_trex_dqn_config.py` & `DI-engine-0.4.8/dizoo/box2d/lunarlander/config/lunarlander_trex_dqn_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/box2d/lunarlander/config/lunarlander_trex_offppo_config.py` & `DI-engine-0.4.8/dizoo/box2d/lunarlander/config/lunarlander_trex_offppo_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/box2d/lunarlander/config/t.py` & `DI-engine-0.4.8/dizoo/box2d/lunarlander/config/t.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/box2d/lunarlander/entry/lunarlander_dqn_eval.py` & `DI-engine-0.4.8/dizoo/box2d/lunarlander/entry/lunarlander_dqn_eval.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/box2d/lunarlander/entry/lunarlander_dqn_example.py` & `DI-engine-0.4.8/dizoo/box2d/lunarlander/entry/lunarlander_dqn_example.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/box2d/lunarlander/envs/lunarlander_env.py` & `DI-engine-0.4.8/dizoo/box2d/lunarlander/envs/lunarlander_env.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/box2d/lunarlander/envs/test_lunarlander_env.py` & `DI-engine-0.4.8/dizoo/box2d/lunarlander/envs/test_lunarlander_env.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/bsuite/envs/bsuite_env.py` & `DI-engine-0.4.8/dizoo/bsuite/envs/bsuite_env.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/bsuite/envs/test_bsuite_env.py` & `DI-engine-0.4.8/dizoo/bsuite/envs/test_bsuite_env.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/classic_control/acrobot/config/acrobot_dqn_config.py` & `DI-engine-0.4.8/dizoo/procgen/config/coinrun_dqn_config.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,55 +1,51 @@
 from easydict import EasyDict
 
-acrobot_dqn_config = dict(
-    exp_name='acrobot_dqn_seed0',
+coinrun_dqn_config = dict(
     env=dict(
-        collector_env_num=8,
-        evaluator_env_num=8,
-        n_evaluator_episode=8,
-        stop_value=-60,
-        env_id='Acrobot-v1',
-        replay_path='acrobot_dqn_seed0/video',
+        env_id='coinrun',
+        collector_env_num=4,
+        evaluator_env_num=4,
+        n_evaluator_episode=4,
+        stop_value=10,
     ),
     policy=dict(
-        cuda=True,
+        cuda=False,
         model=dict(
-            obs_shape=6,
-            action_shape=3,
-            encoder_hidden_size_list=[256, 256],
-            dueling=True,
+            obs_shape=[3, 64, 64],
+            action_shape=15,
+            encoder_hidden_size_list=[128, 128, 512],
+            dueling=False,
         ),
-        nstep=3,
         discount_factor=0.99,
         learn=dict(
-            update_per_collect=10,
-            batch_size=128,
-            learning_rate=0.0001,
-            target_update_freq=250,
+            update_per_collect=20,
+            batch_size=32,
+            learning_rate=0.0005,
+            target_update_freq=500,
         ),
-        collect=dict(n_sample=96, ),
-        eval=dict(evaluator=dict(eval_freq=2000, )),
+        collect=dict(n_sample=100, ),
+        eval=dict(evaluator=dict(eval_freq=5000, )),
         other=dict(
             eps=dict(
                 type='exp',
                 start=1.,
                 end=0.05,
                 decay=250000,
             ),
             replay_buffer=dict(replay_buffer_size=100000, ),
         ),
     ),
 )
-acrobot_dqn_config = EasyDict(acrobot_dqn_config)
-main_config = acrobot_dqn_config
-acrobot_dqn_create_config = dict(
-    env=dict(type='acrobot', import_names=['dizoo.classic_control.acrobot.envs.acrobot_env']),
-    env_manager=dict(type='subprocess'),
+coinrun_dqn_config = EasyDict(coinrun_dqn_config)
+main_config = coinrun_dqn_config
+
+coinrun_dqn_create_config = dict(
+    env=dict(
+        type='procgen',
+        import_names=['dizoo.procgen.envs.procgen_env'],
+    ),
+    env_manager=dict(type='subprocess', ),
     policy=dict(type='dqn'),
-    replay_buffer=dict(type='deque', import_names=['ding.data.buffer.deque_buffer_wrapper']),
 )
-acrobot_dqn_create_config = EasyDict(acrobot_dqn_create_config)
-create_config = acrobot_dqn_create_config
-
-if __name__ == "__main__":
-    from ding.entry import serial_pipeline
-    serial_pipeline((main_config, create_config), seed=0)
+coinrun_dqn_create_config = EasyDict(coinrun_dqn_create_config)
+create_config = coinrun_dqn_create_config
```

### Comparing `DI-engine-0.4.7/dizoo/classic_control/acrobot/envs/acrobot_env.py` & `DI-engine-0.4.8/dizoo/classic_control/acrobot/envs/acrobot_env.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/classic_control/acrobot/envs/test_acrobot_env.py` & `DI-engine-0.4.8/dizoo/classic_control/acrobot/envs/test_acrobot_env.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/classic_control/cartpole/config/__init__.py` & `DI-engine-0.4.8/dizoo/classic_control/cartpole/config/__init__.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/classic_control/cartpole/config/cartpole_a2c_config.py` & `DI-engine-0.4.8/dizoo/classic_control/cartpole/config/cartpole_a2c_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/classic_control/cartpole/config/cartpole_acer_config.py` & `DI-engine-0.4.8/dizoo/classic_control/cartpole/config/cartpole_acer_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/classic_control/cartpole/config/cartpole_bc_config.py` & `DI-engine-0.4.8/dizoo/classic_control/cartpole/config/cartpole_bc_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/classic_control/cartpole/config/cartpole_bco_config.py` & `DI-engine-0.4.8/dizoo/classic_control/cartpole/config/cartpole_bco_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/classic_control/cartpole/config/cartpole_c51_config.py` & `DI-engine-0.4.8/dizoo/classic_control/cartpole/config/cartpole_c51_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/classic_control/cartpole/config/cartpole_cql_config.py` & `DI-engine-0.4.8/dizoo/classic_control/cartpole/config/cartpole_cql_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/classic_control/cartpole/config/cartpole_decision_transformer.py` & `DI-engine-0.4.8/dizoo/classic_control/cartpole/config/cartpole_decision_transformer.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/classic_control/cartpole/config/cartpole_dqfd_config.py` & `DI-engine-0.4.8/dizoo/classic_control/cartpole/config/cartpole_dqfd_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/classic_control/cartpole/config/cartpole_dqn_config.py` & `DI-engine-0.4.8/dizoo/classic_control/cartpole/config/cartpole_dqn_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/classic_control/cartpole/config/cartpole_dqn_gail_config.py` & `DI-engine-0.4.8/dizoo/classic_control/cartpole/config/cartpole_dqn_gail_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/classic_control/cartpole/config/cartpole_dqn_rnd_config.py` & `DI-engine-0.4.8/dizoo/classic_control/cartpole/config/cartpole_dqn_rnd_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/classic_control/cartpole/config/cartpole_dqn_stdim_config.py` & `DI-engine-0.4.8/dizoo/classic_control/cartpole/config/cartpole_dqn_stdim_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/classic_control/cartpole/config/cartpole_drex_dqn_config.py` & `DI-engine-0.4.8/dizoo/classic_control/cartpole/config/cartpole_drex_dqn_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/classic_control/cartpole/config/cartpole_fqf_config.py` & `DI-engine-0.4.8/dizoo/classic_control/cartpole/config/cartpole_fqf_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/classic_control/cartpole/config/cartpole_gcl_config.py` & `DI-engine-0.4.8/dizoo/classic_control/cartpole/config/cartpole_gcl_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/classic_control/cartpole/config/cartpole_impala_config.py` & `DI-engine-0.4.8/dizoo/classic_control/cartpole/config/cartpole_impala_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/classic_control/cartpole/config/cartpole_iqn_config.py` & `DI-engine-0.4.8/dizoo/classic_control/cartpole/config/cartpole_iqn_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/classic_control/cartpole/config/cartpole_mdqn_config.py` & `DI-engine-0.4.8/dizoo/classic_control/cartpole/config/cartpole_mdqn_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/classic_control/cartpole/config/cartpole_ngu_config.py` & `DI-engine-0.4.8/dizoo/classic_control/cartpole/config/cartpole_ngu_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/classic_control/cartpole/config/cartpole_pg_config.py` & `DI-engine-0.4.8/dizoo/classic_control/cartpole/config/cartpole_pg_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/classic_control/cartpole/config/cartpole_ppg_config.py` & `DI-engine-0.4.8/dizoo/classic_control/cartpole/config/cartpole_ppg_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/classic_control/cartpole/config/cartpole_ppo_config.py` & `DI-engine-0.4.8/dizoo/classic_control/cartpole/config/cartpole_ppo_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/classic_control/cartpole/config/cartpole_ppo_icm_config.py` & `DI-engine-0.4.8/dizoo/classic_control/cartpole/config/cartpole_ppo_icm_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/classic_control/cartpole/config/cartpole_ppo_offpolicy_config.py` & `DI-engine-0.4.8/dizoo/classic_control/cartpole/config/cartpole_ppo_offpolicy_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/classic_control/cartpole/config/cartpole_ppo_stdim_config.py` & `DI-engine-0.4.8/dizoo/classic_control/cartpole/config/cartpole_ppo_stdim_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/classic_control/cartpole/config/cartpole_ppopg_config.py` & `DI-engine-0.4.8/dizoo/classic_control/cartpole/config/cartpole_ppopg_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/classic_control/cartpole/config/cartpole_qrdqn_config.py` & `DI-engine-0.4.8/dizoo/classic_control/cartpole/config/cartpole_qrdqn_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/classic_control/cartpole/config/cartpole_qrdqn_generation_data_config.py` & `DI-engine-0.4.8/dizoo/classic_control/cartpole/config/cartpole_qrdqn_generation_data_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/classic_control/cartpole/config/cartpole_r2d2_config.py` & `DI-engine-0.4.8/dizoo/classic_control/cartpole/config/cartpole_r2d2_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/classic_control/cartpole/config/cartpole_r2d2_gtrxl_config.py` & `DI-engine-0.4.8/dizoo/classic_control/cartpole/config/cartpole_r2d2_gtrxl_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/classic_control/cartpole/config/cartpole_r2d2_residual_config.py` & `DI-engine-0.4.8/dizoo/classic_control/cartpole/config/cartpole_r2d2_residual_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/classic_control/cartpole/config/cartpole_rainbow_config.py` & `DI-engine-0.4.8/dizoo/classic_control/cartpole/config/cartpole_rainbow_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/classic_control/cartpole/config/cartpole_rnd_onppo_config.py` & `DI-engine-0.4.8/dizoo/classic_control/cartpole/config/cartpole_rnd_onppo_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/classic_control/cartpole/config/cartpole_sac_config.py` & `DI-engine-0.4.8/dizoo/classic_control/cartpole/config/cartpole_sac_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/classic_control/cartpole/config/cartpole_sqil_config.py` & `DI-engine-0.4.8/dizoo/classic_control/cartpole/config/cartpole_sqil_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/classic_control/cartpole/config/cartpole_sql_config.py` & `DI-engine-0.4.8/dizoo/classic_control/cartpole/config/cartpole_sql_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/classic_control/cartpole/config/cartpole_sqn_config.py` & `DI-engine-0.4.8/dizoo/classic_control/cartpole/config/cartpole_sqn_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/classic_control/cartpole/config/cartpole_trex_dqn_config.py` & `DI-engine-0.4.8/dizoo/classic_control/cartpole/config/cartpole_trex_dqn_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/classic_control/cartpole/config/cartpole_trex_offppo_config.py` & `DI-engine-0.4.8/dizoo/classic_control/cartpole/config/cartpole_trex_offppo_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/classic_control/cartpole/config/cartpole_trex_onppo_config.py` & `DI-engine-0.4.8/dizoo/classic_control/cartpole/config/cartpole_trex_onppo_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/classic_control/cartpole/config/parallel/cartpole_dqn_config.py` & `DI-engine-0.4.8/dizoo/classic_control/cartpole/config/parallel/cartpole_dqn_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/classic_control/cartpole/config/parallel/cartpole_dqn_config_k8s.py` & `DI-engine-0.4.8/dizoo/classic_control/cartpole/config/parallel/cartpole_dqn_config_k8s.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/classic_control/cartpole/entry/cartpole_c51_deploy.py` & `DI-engine-0.4.8/dizoo/classic_control/cartpole/entry/cartpole_c51_deploy.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/classic_control/cartpole/entry/cartpole_c51_main.py` & `DI-engine-0.4.8/dizoo/classic_control/cartpole/entry/cartpole_c51_main.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/classic_control/cartpole/entry/cartpole_cql_main.py` & `DI-engine-0.4.8/dizoo/classic_control/cartpole/entry/cartpole_cql_main.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/classic_control/cartpole/entry/cartpole_dqn_buffer_main.py` & `DI-engine-0.4.8/dizoo/classic_control/cartpole/entry/cartpole_dqn_buffer_main.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/classic_control/cartpole/entry/cartpole_dqn_eval.py` & `DI-engine-0.4.8/dizoo/classic_control/cartpole/entry/cartpole_dqn_eval.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/classic_control/cartpole/entry/cartpole_dqn_main.py` & `DI-engine-0.4.8/dizoo/classic_control/cartpole/entry/cartpole_dqn_main.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/classic_control/cartpole/entry/cartpole_fqf_main.py` & `DI-engine-0.4.8/dizoo/classic_control/cartpole/entry/cartpole_fqf_main.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/classic_control/cartpole/entry/cartpole_ppg_main.py` & `DI-engine-0.4.8/dizoo/classic_control/cartpole/entry/cartpole_ppg_main.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/classic_control/cartpole/entry/cartpole_ppo_main.py` & `DI-engine-0.4.8/dizoo/classic_control/cartpole/entry/cartpole_ppo_main.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/classic_control/cartpole/entry/cartpole_ppo_offpolicy_main.py` & `DI-engine-0.4.8/dizoo/classic_control/cartpole/entry/cartpole_ppo_offpolicy_main.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/classic_control/cartpole/entry/formatted_total_config.py` & `DI-engine-0.4.8/dizoo/classic_control/cartpole/entry/formatted_total_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/classic_control/cartpole/envs/cartpole_env.py` & `DI-engine-0.4.8/dizoo/classic_control/cartpole/envs/cartpole_env.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/classic_control/cartpole/envs/test_cartpole_env.py` & `DI-engine-0.4.8/dizoo/classic_control/cartpole/envs/test_cartpole_env.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/classic_control/cartpole/envs/test_cartpole_env_manager.py` & `DI-engine-0.4.8/dizoo/classic_control/cartpole/envs/test_cartpole_env_manager.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/classic_control/mountain_car/envs/mtcar_env.py` & `DI-engine-0.4.8/dizoo/classic_control/mountain_car/envs/mtcar_env.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/classic_control/mountain_car/envs/test_mtcar_env.py` & `DI-engine-0.4.8/dizoo/classic_control/mountain_car/envs/test_mtcar_env.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/classic_control/pendulum/config/__init__.py` & `DI-engine-0.4.8/dizoo/classic_control/pendulum/config/__init__.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/classic_control/pendulum/config/pendulum_bdq_config.py` & `DI-engine-0.4.8/dizoo/classic_control/pendulum/config/pendulum_bdq_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/classic_control/pendulum/config/pendulum_cql_config.py` & `DI-engine-0.4.8/dizoo/classic_control/pendulum/config/pendulum_cql_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/classic_control/pendulum/config/pendulum_d4pg_config.py` & `DI-engine-0.4.8/dizoo/classic_control/pendulum/config/pendulum_d4pg_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/classic_control/pendulum/config/pendulum_ddpg_config.py` & `DI-engine-0.4.8/dizoo/classic_control/pendulum/config/pendulum_ddpg_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/classic_control/pendulum/config/pendulum_dqn_config.py` & `DI-engine-0.4.8/dizoo/classic_control/pendulum/config/pendulum_dqn_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/classic_control/pendulum/config/pendulum_dt_config.py` & `DI-engine-0.4.8/dizoo/classic_control/pendulum/config/pendulum_dt_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/classic_control/pendulum/config/pendulum_ibc_config.py` & `DI-engine-0.4.8/dizoo/classic_control/pendulum/config/pendulum_ibc_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/classic_control/pendulum/config/pendulum_pg_config.py` & `DI-engine-0.4.8/dizoo/classic_control/pendulum/config/pendulum_pg_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/classic_control/pendulum/config/pendulum_ppo_config.py` & `DI-engine-0.4.8/dizoo/classic_control/pendulum/config/pendulum_ppo_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/classic_control/pendulum/config/pendulum_sac_config.py` & `DI-engine-0.4.8/dizoo/classic_control/pendulum/config/pendulum_sac_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/classic_control/pendulum/config/pendulum_sac_data_generation_config.py` & `DI-engine-0.4.8/dizoo/classic_control/pendulum/config/pendulum_sac_data_generation_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/classic_control/pendulum/config/pendulum_sqil_sac_config.py` & `DI-engine-0.4.8/dizoo/classic_control/pendulum/config/pendulum_sqil_sac_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/classic_control/pendulum/config/pendulum_td3_bc_config.py` & `DI-engine-0.4.8/dizoo/classic_control/pendulum/config/pendulum_td3_bc_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/classic_control/pendulum/config/pendulum_td3_config.py` & `DI-engine-0.4.8/dizoo/classic_control/pendulum/config/pendulum_td3_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/classic_control/pendulum/config/pendulum_td3_data_generation_config.py` & `DI-engine-0.4.8/dizoo/classic_control/pendulum/config/pendulum_td3_data_generation_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/classic_control/pendulum/entry/pendulum_cql_ddpg_main.py` & `DI-engine-0.4.8/dizoo/classic_control/pendulum/entry/pendulum_cql_ddpg_main.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/classic_control/pendulum/entry/pendulum_cql_main.py` & `DI-engine-0.4.8/dizoo/classic_control/pendulum/entry/pendulum_cql_main.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/classic_control/pendulum/entry/pendulum_d4pg_main.py` & `DI-engine-0.4.8/dizoo/classic_control/pendulum/entry/pendulum_d4pg_main.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/classic_control/pendulum/entry/pendulum_ddpg_main.py` & `DI-engine-0.4.8/dizoo/classic_control/pendulum/entry/pendulum_ddpg_main.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/classic_control/pendulum/entry/pendulum_dqn_eval.py` & `DI-engine-0.4.8/dizoo/classic_control/pendulum/entry/pendulum_dqn_eval.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/classic_control/pendulum/entry/pendulum_ppo_main.py` & `DI-engine-0.4.8/dizoo/classic_control/pendulum/entry/pendulum_ppo_main.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/classic_control/pendulum/entry/pendulum_td3_bc_main.py` & `DI-engine-0.4.8/dizoo/classic_control/pendulum/entry/pendulum_td3_bc_main.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/classic_control/pendulum/entry/pendulum_td3_main.py` & `DI-engine-0.4.8/dizoo/classic_control/pendulum/entry/pendulum_td3_main.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/classic_control/pendulum/envs/pendulum_env.py` & `DI-engine-0.4.8/dizoo/classic_control/pendulum/envs/pendulum_env.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/classic_control/pendulum/envs/test_pendulum_env.py` & `DI-engine-0.4.8/dizoo/classic_control/pendulum/envs/test_pendulum_env.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/common/policy/md_dqn.py` & `DI-engine-0.4.8/dizoo/common/policy/md_dqn.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/common/policy/md_ppo.py` & `DI-engine-0.4.8/dizoo/common/policy/md_ppo.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/common/policy/md_rainbow_dqn.py` & `DI-engine-0.4.8/dizoo/common/policy/md_rainbow_dqn.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/competitive_rl/envs/competitive_rl_env.py` & `DI-engine-0.4.8/dizoo/competitive_rl/envs/competitive_rl_env.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/competitive_rl/envs/competitive_rl_env_wrapper.py` & `DI-engine-0.4.8/dizoo/competitive_rl/envs/competitive_rl_env_wrapper.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/competitive_rl/envs/test_competitive_rl.py` & `DI-engine-0.4.8/dizoo/competitive_rl/envs/test_competitive_rl.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/d4rl/config/halfcheetah_expert_cql_config.py` & `DI-engine-0.4.8/dizoo/d4rl/config/hopper_expert_cql_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # You can conduct Experiments on D4RL with this config file through the following command:
 # cd ../entry && python d4rl_cql_main.py
 from easydict import EasyDict
 
 main_config = dict(
-    exp_name="halfcheetah_expert_cql_seed0",
+    exp_name="hopper_expert_cql_seed0",
     env=dict(
-        env_id='halfcheetah-expert-v0',
+        env_id='hopper-expert-v0',
         collector_env_num=1,
         evaluator_env_num=8,
         use_act_scale=True,
         n_evaluator_episode=8,
         stop_value=6000,
     ),
     policy=dict(
```

### Comparing `DI-engine-0.4.7/dizoo/d4rl/config/halfcheetah_expert_dt_config.py` & `DI-engine-0.4.8/dizoo/d4rl/config/halfcheetah_expert_dt_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/d4rl/config/halfcheetah_expert_td3bc_config.py` & `DI-engine-0.4.8/dizoo/d4rl/config/halfcheetah_medium_expert_td3bc_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 # You can conduct Experiments on D4RL with this config file through the following command:
 # cd ../entry && python d4rl_td3_bc_main.py
 from easydict import EasyDict
 
 main_config = dict(
-    exp_name='walker2d_expert_td3-bc_seed0',
+    exp_name='halfcheetah_medium_expert_td3-bc_seed0',
     env=dict(
-        env_id='walker2d-expert-v0',
+        env_id='halfcheetah-medium-expert-v2',
         norm_obs=dict(
-            use_norm=True, 
+            use_norm=True,
             offline_stats=dict(use_offline_stats=True, ),
         ),
         collector_env_num=1,
         evaluator_env_num=8,
         use_act_scale=True,
         n_evaluator_episode=8,
-        stop_value=6000,
+        stop_value=13000,
     ),
     policy=dict(
+        cuda=True,
         model=dict(
-            obs_shape=11,
-            action_shape=3,
+            obs_shape=17,
+            action_shape=6,
         ),
         learn=dict(
             train_epoch=30000,
             batch_size=256,
             learning_rate_actor=0.0003,
             learning_rate_critic=0.0003,
             actor_update_freq=2,
```

### Comparing `DI-engine-0.4.7/dizoo/d4rl/config/halfcheetah_medium_cql_config.py` & `DI-engine-0.4.8/dizoo/d4rl/config/halfcheetah_medium_expert_cql_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # You can conduct Experiments on D4RL with this config file through the following command:
 # cd ../entry && python d4rl_cql_main.py
 from easydict import EasyDict
 
 main_config = dict(
-    exp_name="halfcheetah_medium_cql_seed0",
+    exp_name="halfcheetah_medium_expert_cql_seed0",
     env=dict(
-        env_id='halfcheetah-medium-v0',
+        env_id='halfcheetah-medium-expert-v2',
         collector_env_num=1,
         evaluator_env_num=8,
         use_act_scale=True,
         n_evaluator_episode=8,
         stop_value=6000,
     ),
     policy=dict(
         cuda=True,
         model=dict(
-            obs_shape=11,
-            action_shape=3,
+            obs_shape=17,
+            action_shape=6,
         ),
         learn=dict(
             data_path=None,
             train_epoch=30000,
             batch_size=256,
             learning_rate_q=3e-4,
             learning_rate_policy=1e-4,
```

### Comparing `DI-engine-0.4.7/dizoo/d4rl/config/halfcheetah_medium_dt_config.py` & `DI-engine-0.4.8/dizoo/d4rl/config/halfcheetah_medium_dt_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/d4rl/config/halfcheetah_medium_expert_cql_config.py` & `DI-engine-0.4.8/dizoo/d4rl/config/hopper_medium_expert_cql_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # You can conduct Experiments on D4RL with this config file through the following command:
 # cd ../entry && python d4rl_cql_main.py
 from easydict import EasyDict
 
 main_config = dict(
-    exp_name="halfcheetah_medium_expert_cql_seed0",
+    exp_name="hopper_medium_expert_cql_seed0",
     env=dict(
-        env_id='halfcheetah-medium-expert-v0',
+        env_id='hopper-medium-expert-v0',
         collector_env_num=1,
         evaluator_env_num=8,
         use_act_scale=True,
         n_evaluator_episode=8,
         stop_value=6000,
     ),
     policy=dict(
```

### Comparing `DI-engine-0.4.7/dizoo/d4rl/config/halfcheetah_medium_expert_dt_config.py` & `DI-engine-0.4.8/dizoo/d4rl/config/halfcheetah_medium_expert_dt_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/d4rl/config/halfcheetah_medium_expert_td3bc_config.py` & `DI-engine-0.4.8/dizoo/d4rl/config/hopper_medium_expert_td3bc_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 # You can conduct Experiments on D4RL with this config file through the following command:
 # cd ../entry && python d4rl_td3_bc_main.py
 from easydict import EasyDict
 
 main_config = dict(
-    exp_name='halfcheetah_medium_expert_td3-bc_seed0',
+    exp_name='hopper_medium_expert_td3-bc_seed0',
     env=dict(
-        env_id='halfcheetah-medium-expert-v0',
-        norm_obs=dict(
-            use_norm=True, 
-            offline_stats=dict(use_offline_stats=True, ),
-        ),
+        env_id='hopper-medium-expert-v2',
         collector_env_num=1,
         evaluator_env_num=8,
         use_act_scale=True,
         n_evaluator_episode=8,
         stop_value=6000,
     ),
     policy=dict(
+        cuda=True,
         model=dict(
             obs_shape=11,
             action_shape=3,
         ),
         learn=dict(
             train_epoch=30000,
             batch_size=256,
```

### Comparing `DI-engine-0.4.7/dizoo/d4rl/config/halfcheetah_medium_replay_cql_config.py` & `DI-engine-0.4.8/dizoo/d4rl/config/halfcheetah_medium_replay_cql_config.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # You can conduct Experiments on D4RL with this config file through the following command:
 # cd ../entry && python d4rl_cql_main.py
 from easydict import EasyDict
 
 main_config = dict(
     exp_name="halfcheetah_medium_replay_cql_seed0",
     env=dict(
-        env_id='halfcheetah-medium-replay-v0',
+        env_id='halfcheetah-medium-replay-v2',
         collector_env_num=1,
         evaluator_env_num=8,
         use_act_scale=True,
         n_evaluator_episode=8,
         stop_value=6000,
     ),
     policy=dict(
         cuda=True,
         model=dict(
-            obs_shape=11,
-            action_shape=3,
+            obs_shape=17,
+            action_shape=6,
         ),
         learn=dict(
             data_path=None,
             train_epoch=30000,
             batch_size=256,
             learning_rate_q=3e-4,
             learning_rate_policy=1e-4,
```

### Comparing `DI-engine-0.4.7/dizoo/d4rl/config/halfcheetah_medium_replay_dt_config.py` & `DI-engine-0.4.8/dizoo/d4rl/config/halfcheetah_medium_replay_dt_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/d4rl/config/halfcheetah_medium_replay_td3bc_config.py` & `DI-engine-0.4.8/dizoo/d4rl/config/halfcheetah_medium_replay_td3bc_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 # You can conduct Experiments on D4RL with this config file through the following command:
 # cd ../entry && python d4rl_td3_bc_main.py
 from easydict import EasyDict
 
 main_config = dict(
     exp_name='halfcheetah_medium_replay_td3-bc_seed0',
     env=dict(
-        env_id='halfcheetah-medium-replay-v0',
+        env_id='halfcheetah-medium-replay-v2',
         norm_obs=dict(
-            use_norm=True, 
+            use_norm=True,
             offline_stats=dict(use_offline_stats=True, ),
         ),
         collector_env_num=1,
         evaluator_env_num=8,
         use_act_scale=True,
         n_evaluator_episode=8,
         stop_value=6000,
     ),
     policy=dict(
+        cuda=True,
         model=dict(
-            obs_shape=11,
-            action_shape=3,
+            obs_shape=17,
+            action_shape=6,
         ),
         learn=dict(
             train_epoch=30000,
             batch_size=256,
             learning_rate_actor=0.0003,
             learning_rate_critic=0.0003,
             actor_update_freq=2,
```

### Comparing `DI-engine-0.4.7/dizoo/d4rl/config/halfcheetah_medium_td3bc_config.py` & `DI-engine-0.4.8/dizoo/d4rl/config/halfcheetah_medium_td3bc_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 # You can conduct Experiments on D4RL with this config file through the following command:
 # cd ../entry && python d4rl_td3_bc_main.py
 from easydict import EasyDict
 
 main_config = dict(
     exp_name='halfcheetah_medium_td3-bc_seed0',
     env=dict(
-        env_id='halfcheetah-medium-v0',
+        env_id='halfcheetah-medium-v2',
         norm_obs=dict(
-            use_norm=True, 
+            use_norm=True,
             offline_stats=dict(use_offline_stats=True, ),
         ),
         collector_env_num=1,
         evaluator_env_num=8,
         use_act_scale=True,
         n_evaluator_episode=8,
-        stop_value=6000,
+        stop_value=7600,
     ),
     policy=dict(
+        cuda=True,
         model=dict(
-            obs_shape=11,
-            action_shape=3,
+            obs_shape=17,
+            action_shape=6,
         ),
         learn=dict(
             train_epoch=30000,
             batch_size=256,
             learning_rate_actor=0.0003,
             learning_rate_critic=0.0003,
             actor_update_freq=2,
```

### Comparing `DI-engine-0.4.7/dizoo/d4rl/config/halfcheetah_random_cql_config.py` & `DI-engine-0.4.8/dizoo/d4rl/config/hopper_random_cql_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # You can conduct Experiments on D4RL with this config file through the following command:
 # cd ../entry && python d4rl_cql_main.py
 from easydict import EasyDict
 
 main_config = dict(
-    exp_name="halfcheetah_expert_cql_seed0",
+    exp_name="hopper_expert_cql_seed0",
     env=dict(
-        env_id='halfcheetah-expert-v0',
+        env_id='hopper-expert-v0',
         collector_env_num=1,
         evaluator_env_num=8,
         use_act_scale=True,
         n_evaluator_episode=8,
         stop_value=6000,
     ),
     policy=dict(
```

### Comparing `DI-engine-0.4.7/dizoo/d4rl/config/halfcheetah_random_dt_config.py` & `DI-engine-0.4.8/dizoo/d4rl/config/halfcheetah_random_dt_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/d4rl/config/halfcheetah_random_td3bc_config.py` & `DI-engine-0.4.8/dizoo/d4rl/config/halfcheetah_random_td3bc_config.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 # You can conduct Experiments on D4RL with this config file through the following command:
 # cd ../entry && python d4rl_td3_bc_main.py
 from easydict import EasyDict
 
 main_config = dict(
     exp_name='halfcheetah_random_td3-bc_seed0',
     env=dict(
-        env_id='halfcheetah-random-v0',
+        env_id='halfcheetah-random-v2',
         norm_obs=dict(
-            use_norm=True, 
+            use_norm=True,
             offline_stats=dict(use_offline_stats=True, ),
         ),
         collector_env_num=1,
         evaluator_env_num=8,
         use_act_scale=True,
         n_evaluator_episode=8,
         stop_value=6000,
     ),
     policy=dict(
+        cuda=True,
         model=dict(
-            obs_shape=11,
-            action_shape=3,
+            obs_shape=17,
+            action_shape=6,
         ),
         learn=dict(
             train_epoch=30000,
             batch_size=256,
             learning_rate_actor=0.0003,
             learning_rate_critic=0.0003,
             actor_update_freq=2,
```

### Comparing `DI-engine-0.4.7/dizoo/d4rl/config/hopper_expert_cql_config.py` & `DI-engine-0.4.8/dizoo/d4rl/config/hopper_medium_cql_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # You can conduct Experiments on D4RL with this config file through the following command:
 # cd ../entry && python d4rl_cql_main.py
 from easydict import EasyDict
 
 main_config = dict(
-    exp_name="hopper_expert_cql_seed0",
+    exp_name="hopper_medium_cql_seed0",
     env=dict(
-        env_id='hopper-expert-v0',
+        env_id='hopper-medium-v0',
         collector_env_num=1,
         evaluator_env_num=8,
         use_act_scale=True,
         n_evaluator_episode=8,
         stop_value=6000,
     ),
     policy=dict(
```

### Comparing `DI-engine-0.4.7/dizoo/d4rl/config/hopper_expert_dt_config.py` & `DI-engine-0.4.8/dizoo/d4rl/config/hopper_expert_dt_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/d4rl/config/hopper_expert_td3bc_config.py` & `DI-engine-0.4.8/dizoo/d4rl/config/hopper_expert_td3bc_config.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 # You can conduct Experiments on D4RL with this config file through the following command:
 # cd ../entry && python d4rl_td3_bc_main.py
 from easydict import EasyDict
 
 main_config = dict(
     exp_name='hopper_expert_td3-bc_seed0',
     env=dict(
-        env_id='hopper-expert-v0',
-        norm_obs=dict(
-            use_norm=True, 
-            offline_stats=dict(use_offline_stats=True, ),
-        ),
+        env_id='hopper-expert-v2',
         collector_env_num=1,
         evaluator_env_num=8,
         use_act_scale=True,
         n_evaluator_episode=8,
         stop_value=6000,
     ),
     policy=dict(
+        cuda=True,
         model=dict(
             obs_shape=11,
             action_shape=3,
         ),
         learn=dict(
             train_epoch=30000,
             batch_size=256,
```

### Comparing `DI-engine-0.4.7/dizoo/d4rl/config/hopper_medium_cql_config.py` & `DI-engine-0.4.8/dizoo/d4rl/config/halfcheetah_medium_cql_config.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # You can conduct Experiments on D4RL with this config file through the following command:
 # cd ../entry && python d4rl_cql_main.py
 from easydict import EasyDict
 
 main_config = dict(
-    exp_name="hopper_medium_cql_seed0",
+    exp_name="halfcheetah_medium_cql_seed0",
     env=dict(
-        env_id='hopper-medium-v0',
+        env_id='halfcheetah-medium-v2',
         collector_env_num=1,
         evaluator_env_num=8,
         use_act_scale=True,
         n_evaluator_episode=8,
         stop_value=6000,
     ),
     policy=dict(
         cuda=True,
         model=dict(
-            obs_shape=11,
-            action_shape=3,
+            obs_shape=17,
+            action_shape=6,
         ),
         learn=dict(
             data_path=None,
             train_epoch=30000,
             batch_size=256,
             learning_rate_q=3e-4,
             learning_rate_policy=1e-4,
```

### Comparing `DI-engine-0.4.7/dizoo/d4rl/config/hopper_medium_dt_config.py` & `DI-engine-0.4.8/dizoo/d4rl/config/hopper_medium_dt_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/d4rl/config/hopper_medium_expert_bc_config.py` & `DI-engine-0.4.8/dizoo/d4rl/config/hopper_medium_expert_bc_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/d4rl/config/hopper_medium_expert_cql_config.py` & `DI-engine-0.4.8/dizoo/d4rl/config/hopper_medium_replay_cql_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # You can conduct Experiments on D4RL with this config file through the following command:
 # cd ../entry && python d4rl_cql_main.py
 from easydict import EasyDict
 
 main_config = dict(
-    exp_name="hopper_medium_expert_cql_seed0",
+    exp_name="hopper_medium_replay_cql_seed0",
     env=dict(
-        env_id='hopper-medium-expert-v0',
+        env_id='hopper-medium-replay-v0',
         collector_env_num=1,
         evaluator_env_num=8,
         use_act_scale=True,
         n_evaluator_episode=8,
         stop_value=6000,
     ),
     policy=dict(
```

### Comparing `DI-engine-0.4.7/dizoo/d4rl/config/hopper_medium_expert_dt_config.py` & `DI-engine-0.4.8/dizoo/d4rl/config/hopper_medium_expert_dt_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/d4rl/config/hopper_medium_expert_ibc_ar_config.py` & `DI-engine-0.4.8/dizoo/d4rl/config/hopper_medium_expert_ibc_ar_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/d4rl/config/hopper_medium_expert_ibc_config.py` & `DI-engine-0.4.8/dizoo/d4rl/config/hopper_medium_expert_ibc_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/d4rl/config/hopper_medium_expert_ibc_mcmc_config.py` & `DI-engine-0.4.8/dizoo/d4rl/config/hopper_medium_expert_ibc_mcmc_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/d4rl/config/hopper_medium_expert_td3bc_config.py` & `DI-engine-0.4.8/dizoo/d4rl/config/hopper_medium_td3bc_config.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 # You can conduct Experiments on D4RL with this config file through the following command:
 # cd ../entry && python d4rl_td3_bc_main.py
 from easydict import EasyDict
 
 main_config = dict(
-    exp_name='hopper_medium_expert_td3-bc_seed0',
+    exp_name='hopper_medium_td3-bc_seed0',
     env=dict(
-        env_id='hopper-medium-expert-v0',
-        norm_obs=dict(
-            use_norm=True, 
-            offline_stats=dict(use_offline_stats=True, ),
-        ),
+        env_id='hopper-medium-v2',
         collector_env_num=1,
         evaluator_env_num=8,
         use_act_scale=True,
         n_evaluator_episode=8,
         stop_value=6000,
     ),
     policy=dict(
+        cuda=True,
         model=dict(
             obs_shape=11,
             action_shape=3,
         ),
         learn=dict(
             train_epoch=30000,
             batch_size=256,
```

### Comparing `DI-engine-0.4.7/dizoo/d4rl/config/hopper_medium_replay_cql_config.py` & `DI-engine-0.4.8/dizoo/d4rl/config/walker2d_medium_replay_cql_config.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # You can conduct Experiments on D4RL with this config file through the following command:
 # cd ../entry && python d4rl_cql_main.py
 from easydict import EasyDict
 
 main_config = dict(
-    exp_name="hopper_medium_replay_cql_seed0",
+    exp_name="walker2d_medium_replay_cql_seed0",
     env=dict(
-        env_id='hopper-medium-replay-v0',
+        env_id='walker2d-medium-replay-v2',
         collector_env_num=1,
         evaluator_env_num=8,
         use_act_scale=True,
         n_evaluator_episode=8,
         stop_value=6000,
     ),
     policy=dict(
         cuda=True,
         model=dict(
-            obs_shape=11,
-            action_shape=3,
+            obs_shape=17,
+            action_shape=6,
         ),
         learn=dict(
             data_path=None,
             train_epoch=30000,
             batch_size=256,
             learning_rate_q=3e-4,
             learning_rate_policy=1e-4,
```

### Comparing `DI-engine-0.4.7/dizoo/d4rl/config/hopper_medium_replay_dt_config.py` & `DI-engine-0.4.8/dizoo/d4rl/config/hopper_medium_replay_dt_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/d4rl/config/hopper_medium_replay_td3bc_config.py` & `DI-engine-0.4.8/dizoo/d4rl/config/hopper_random_td3bc_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 # You can conduct Experiments on D4RL with this config file through the following command:
 # cd ../entry && python d4rl_td3_bc_main.py
 from easydict import EasyDict
 
 main_config = dict(
-    exp_name='hopper_medium_replay_td3-bc_seed0',
+    exp_name='hopper_random_td3-bc_seed0',
     env=dict(
-        env_id='hopper-medium-replay-v0',
+        env_id='hopper-random-v0',
         norm_obs=dict(
-            use_norm=True, 
+            use_norm=True,
             offline_stats=dict(use_offline_stats=True, ),
         ),
         collector_env_num=1,
         evaluator_env_num=8,
         use_act_scale=True,
         n_evaluator_episode=8,
         stop_value=6000,
     ),
     policy=dict(
+        cuda=True,
         model=dict(
             obs_shape=11,
             action_shape=3,
         ),
         learn=dict(
             train_epoch=30000,
             batch_size=256,
```

### Comparing `DI-engine-0.4.7/dizoo/d4rl/config/hopper_medium_td3bc_config.py` & `DI-engine-0.4.8/dizoo/d4rl/config/hopper_medium_replay_td3bc_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 # You can conduct Experiments on D4RL with this config file through the following command:
 # cd ../entry && python d4rl_td3_bc_main.py
 from easydict import EasyDict
 
 main_config = dict(
-    exp_name='hopper_medium_td3-bc_seed0',
+    exp_name='hopper_medium_replay_td3-bc_seed0',
     env=dict(
-        env_id='hopper-medium-v0',
-        norm_obs=dict(
-            use_norm=True, 
-            offline_stats=dict(use_offline_stats=True, ),
-        ),
+        env_id='hopper-medium-replay-v2',
         collector_env_num=1,
         evaluator_env_num=8,
         use_act_scale=True,
         n_evaluator_episode=8,
         stop_value=6000,
     ),
     policy=dict(
+        cuda=True,
         model=dict(
             obs_shape=11,
             action_shape=3,
         ),
         learn=dict(
             train_epoch=30000,
             batch_size=256,
```

### Comparing `DI-engine-0.4.7/dizoo/d4rl/config/hopper_random_cql_config.py` & `DI-engine-0.4.8/dizoo/d4rl/config/halfcheetah_expert_cql_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # You can conduct Experiments on D4RL with this config file through the following command:
 # cd ../entry && python d4rl_cql_main.py
 from easydict import EasyDict
 
 main_config = dict(
-    exp_name="hopper_expert_cql_seed0",
+    exp_name="halfcheetah_expert_cql_seed0",
     env=dict(
-        env_id='hopper-expert-v0',
+        env_id='halfcheetah-expert-v2',
         collector_env_num=1,
         evaluator_env_num=8,
         use_act_scale=True,
         n_evaluator_episode=8,
         stop_value=6000,
     ),
     policy=dict(
         cuda=True,
         model=dict(
-            obs_shape=11,
-            action_shape=3,
+            obs_shape=17,
+            action_shape=6,
         ),
         learn=dict(
             data_path=None,
             train_epoch=30000,
             batch_size=256,
             learning_rate_q=3e-4,
             learning_rate_policy=1e-4,
```

### Comparing `DI-engine-0.4.7/dizoo/d4rl/config/hopper_random_dt_config.py` & `DI-engine-0.4.8/dizoo/d4rl/config/hopper_random_dt_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/d4rl/config/hopper_random_td3bc_config.py` & `DI-engine-0.4.8/dizoo/d4rl/config/walker2d_medium_replay_td3bc_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 # You can conduct Experiments on D4RL with this config file through the following command:
 # cd ../entry && python d4rl_td3_bc_main.py
 from easydict import EasyDict
 
 main_config = dict(
-    exp_name='hopper_random_td3-bc_seed0',
+    exp_name='walker2d_medium_replay_td3-bc_seed0',
     env=dict(
-        env_id='hopper-random-v0',
+        env_id='walker2d-medium-replay-v2',
         norm_obs=dict(
-            use_norm=True, 
+            use_norm=True,
             offline_stats=dict(use_offline_stats=True, ),
         ),
         collector_env_num=1,
         evaluator_env_num=8,
         use_act_scale=True,
         n_evaluator_episode=8,
         stop_value=6000,
     ),
     policy=dict(
+        cuda=True,
         model=dict(
-            obs_shape=11,
-            action_shape=3,
+            obs_shape=17,
+            action_shape=6,
         ),
         learn=dict(
             train_epoch=30000,
             batch_size=256,
             learning_rate_actor=0.0003,
             learning_rate_critic=0.0003,
             actor_update_freq=2,
```

### Comparing `DI-engine-0.4.7/dizoo/d4rl/config/kitchen_complete_bc_config.py` & `DI-engine-0.4.8/dizoo/d4rl/config/kitchen_complete_bc_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/d4rl/config/kitchen_complete_ibc_ar_config.py` & `DI-engine-0.4.8/dizoo/d4rl/config/kitchen_complete_ibc_ar_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/d4rl/config/kitchen_complete_ibc_config.py` & `DI-engine-0.4.8/dizoo/d4rl/config/kitchen_complete_ibc_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/d4rl/config/kitchen_complete_ibc_mcmc_config.py` & `DI-engine-0.4.8/dizoo/d4rl/config/kitchen_complete_ibc_mcmc_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/d4rl/config/pen_human_bc_config.py` & `DI-engine-0.4.8/dizoo/d4rl/config/pen_human_bc_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/d4rl/config/pen_human_ibc_ar_config.py` & `DI-engine-0.4.8/dizoo/d4rl/config/pen_human_ibc_ar_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/d4rl/config/pen_human_ibc_config.py` & `DI-engine-0.4.8/dizoo/d4rl/config/pen_human_ibc_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/d4rl/config/pen_human_ibc_mcmc_config.py` & `DI-engine-0.4.8/dizoo/d4rl/config/pen_human_ibc_mcmc_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/d4rl/config/walker2d_expert_cql_config.py` & `DI-engine-0.4.8/dizoo/d4rl/config/walker2d_medium_cql_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # You can conduct Experiments on D4RL with this config file through the following command:
 # cd ../entry && python d4rl_cql_main.py
 from easydict import EasyDict
 
 main_config = dict(
-    exp_name="walker2d_expert_cql_seed0",
+    exp_name="walker2d_medium_cql_seed0",
     env=dict(
-        env_id='walker2d-expert-v0',
+        env_id='walker2d-medium-v2',
         collector_env_num=1,
         evaluator_env_num=8,
         use_act_scale=True,
         n_evaluator_episode=8,
         stop_value=6000,
     ),
     policy=dict(
         cuda=True,
         model=dict(
-            obs_shape=11,
-            action_shape=3,
+            obs_shape=17,
+            action_shape=6,
         ),
         learn=dict(
             data_path=None,
             train_epoch=30000,
             batch_size=256,
             learning_rate_q=3e-4,
             learning_rate_policy=1e-4,
```

### Comparing `DI-engine-0.4.7/dizoo/d4rl/config/walker2d_expert_dt_config.py` & `DI-engine-0.4.8/dizoo/d4rl/config/walker2d_expert_dt_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/d4rl/config/walker2d_expert_td3bc_config.py` & `DI-engine-0.4.8/dizoo/d4rl/config/halfcheetah_random_cql_config.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,64 +1,55 @@
 # You can conduct Experiments on D4RL with this config file through the following command:
-# cd ../entry && python d4rl_td3_bc_main.py
+# cd ../entry && python d4rl_cql_main.py
 from easydict import EasyDict
 
 main_config = dict(
-    exp_name='halfcheetah_expert_td3-bc_seed0',
+    exp_name="halfcheetah_expert_cql_seed0",
     env=dict(
-        env_id='halfcheetah-expert-v0',
-        norm_obs=dict(
-            use_norm=True, 
-            offline_stats=dict(use_offline_stats=True, ),
-        ),
+        env_id='halfcheetah-expert-v2',
         collector_env_num=1,
         evaluator_env_num=8,
         use_act_scale=True,
         n_evaluator_episode=8,
         stop_value=6000,
     ),
     policy=dict(
+        cuda=True,
         model=dict(
-            obs_shape=11,
-            action_shape=3,
+            obs_shape=17,
+            action_shape=6,
         ),
         learn=dict(
+            data_path=None,
             train_epoch=30000,
             batch_size=256,
-            learning_rate_actor=0.0003,
-            learning_rate_critic=0.0003,
-            actor_update_freq=2,
-            noise=True,
-            noise_sigma=0.2,
-            noise_range={
-                'min': -0.5,
-                'max': 0.5
-            },
-            alpha=2.5,
-        ),
-        collect=dict(
-            data_type='d4rl',
-            data_path=None,
+            learning_rate_q=3e-4,
+            learning_rate_policy=1e-4,
+            learning_rate_alpha=1e-4,
+            alpha=0.2,
+            auto_alpha=False,
+            lagrange_thresh=-1.0,
+            min_q_weight=5.0,
         ),
-        eval=dict(evaluator=dict(eval_freq=10000, )),
+        collect=dict(data_type='d4rl', ),
+        eval=dict(evaluator=dict(eval_freq=500, )),
         other=dict(replay_buffer=dict(replay_buffer_size=2000000, ), ),
     ),
 )
+
 main_config = EasyDict(main_config)
 main_config = main_config
+
 create_config = dict(
     env=dict(
         type='d4rl',
         import_names=['dizoo.d4rl.envs.d4rl_env'],
     ),
-    env_manager=dict(
-        cfg_type='BaseEnvManagerDict',
-        type='base',
-    ),
+    env_manager=dict(type='base'),
     policy=dict(
-        type='td3_bc',
-        import_names=['ding.policy.td3_bc'],
+        type='cql',
+        import_names=['ding.policy.cql'],
     ),
     replay_buffer=dict(type='naive', ),
 )
 create_config = EasyDict(create_config)
 create_config = create_config
```

### Comparing `DI-engine-0.4.7/dizoo/d4rl/config/walker2d_medium_cql_config.py` & `DI-engine-0.4.8/dizoo/d4rl/config/walker2d_expert_cql_config.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # You can conduct Experiments on D4RL with this config file through the following command:
 # cd ../entry && python d4rl_cql_main.py
 from easydict import EasyDict
 
 main_config = dict(
-    exp_name="walker2d_medium_cql_seed0",
+    exp_name="walker2d_expert_cql_seed0",
     env=dict(
-        env_id='walker2d-medium-v0',
+        env_id='walker2d-expert-v2',
         collector_env_num=1,
         evaluator_env_num=8,
         use_act_scale=True,
         n_evaluator_episode=8,
         stop_value=6000,
     ),
     policy=dict(
         cuda=True,
         model=dict(
-            obs_shape=11,
-            action_shape=3,
+            obs_shape=17,
+            action_shape=6,
         ),
         learn=dict(
             data_path=None,
             train_epoch=30000,
             batch_size=256,
             learning_rate_q=3e-4,
             learning_rate_policy=1e-4,
```

### Comparing `DI-engine-0.4.7/dizoo/d4rl/config/walker2d_medium_dt_config.py` & `DI-engine-0.4.8/dizoo/d4rl/config/walker2d_medium_dt_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/d4rl/config/walker2d_medium_expert_cql_config.py` & `DI-engine-0.4.8/dizoo/d4rl/config/walker2d_medium_expert_cql_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # You can conduct Experiments on D4RL with this config file through the following command:
 # cd ../entry && python d4rl_cql_main.py
 from easydict import EasyDict
 
 main_config = dict(
     exp_name="walker2d_medium_expert_cql_seed0",
     env=dict(
-        env_id='walker2d-medium-expert-v0',
+        env_id='walker2d-medium-expert-v2',
         collector_env_num=1,
         evaluator_env_num=8,
         use_act_scale=True,
         n_evaluator_episode=8,
         stop_value=6000,
     ),
     policy=dict(
         cuda=True,
         model=dict(
-            obs_shape=11,
-            action_shape=3,
+            obs_shape=17,
+            action_shape=6,
         ),
         learn=dict(
             data_path=None,
             train_epoch=30000,
             batch_size=256,
             learning_rate_q=3e-4,
             learning_rate_policy=1e-4,
```

### Comparing `DI-engine-0.4.7/dizoo/d4rl/config/walker2d_medium_expert_dt_config.py` & `DI-engine-0.4.8/dizoo/d4rl/config/walker2d_medium_expert_dt_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/d4rl/config/walker2d_medium_expert_td3bc_config.py` & `DI-engine-0.4.8/dizoo/d4rl/config/walker2d_medium_expert_td3bc_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 # You can conduct Experiments on D4RL with this config file through the following command:
 # cd ../entry && python d4rl_td3_bc_main.py
 from easydict import EasyDict
 
 main_config = dict(
     exp_name='walker2d_medium_expert_td3-bc_seed0',
     env=dict(
-        env_id='walker2d-medium-expert-v0',
+        env_id='walker2d-medium-expert-v2',
         norm_obs=dict(
-            use_norm=True, 
+            use_norm=True,
             offline_stats=dict(use_offline_stats=True, ),
         ),
         collector_env_num=1,
         evaluator_env_num=8,
         use_act_scale=True,
         n_evaluator_episode=8,
         stop_value=6000,
     ),
     policy=dict(
+        cuda=True,
         model=dict(
-            obs_shape=11,
-            action_shape=3,
+            obs_shape=17,
+            action_shape=6,
         ),
         learn=dict(
             train_epoch=30000,
             batch_size=256,
             learning_rate_actor=0.0003,
             learning_rate_critic=0.0003,
             actor_update_freq=2,
```

### Comparing `DI-engine-0.4.7/dizoo/d4rl/config/walker2d_medium_replay_cql_config.py` & `DI-engine-0.4.8/dizoo/d4rl/config/halfcheetah_expert_td3bc_config.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,55 +1,65 @@
 # You can conduct Experiments on D4RL with this config file through the following command:
-# cd ../entry && python d4rl_cql_main.py
+# cd ../entry && python d4rl_td3_bc_main.py
 from easydict import EasyDict
 
 main_config = dict(
-    exp_name="walker2d_medium_replay_cql_seed0",
+    exp_name='halfcheetah_expert_td3-bc_seed0',
     env=dict(
-        env_id='walker2d-medium-replay-v0',
+        env_id='halfcheetah-expert-v2',
+        norm_obs=dict(
+            use_norm=True,
+            offline_stats=dict(use_offline_stats=True, ),
+        ),
         collector_env_num=1,
         evaluator_env_num=8,
         use_act_scale=True,
         n_evaluator_episode=8,
         stop_value=6000,
     ),
     policy=dict(
         cuda=True,
         model=dict(
-            obs_shape=11,
-            action_shape=3,
+            obs_shape=17,
+            action_shape=6,
         ),
         learn=dict(
-            data_path=None,
             train_epoch=30000,
             batch_size=256,
-            learning_rate_q=3e-4,
-            learning_rate_policy=1e-4,
-            learning_rate_alpha=1e-4,
-            alpha=0.2,
-            auto_alpha=False,
-            lagrange_thresh=-1.0,
-            min_q_weight=5.0,
+            learning_rate_actor=0.0003,
+            learning_rate_critic=0.0003,
+            actor_update_freq=2,
+            noise=True,
+            noise_sigma=0.2,
+            noise_range={
+                'min': -0.5,
+                'max': 0.5
+            },
+            alpha=2.5,
+        ),
+        collect=dict(
+            data_type='d4rl',
+            data_path=None,
         ),
-        collect=dict(data_type='d4rl', ),
-        eval=dict(evaluator=dict(eval_freq=500, )),
+        eval=dict(evaluator=dict(eval_freq=10000, )),
         other=dict(replay_buffer=dict(replay_buffer_size=2000000, ), ),
     ),
 )
-
 main_config = EasyDict(main_config)
 main_config = main_config
-
 create_config = dict(
     env=dict(
         type='d4rl',
         import_names=['dizoo.d4rl.envs.d4rl_env'],
     ),
-    env_manager=dict(type='base'),
+    env_manager=dict(
+        cfg_type='BaseEnvManagerDict',
+        type='base',
+    ),
     policy=dict(
-        type='cql',
-        import_names=['ding.policy.cql'],
+        type='td3_bc',
+        import_names=['ding.policy.td3_bc'],
     ),
     replay_buffer=dict(type='naive', ),
 )
 create_config = EasyDict(create_config)
 create_config = create_config
```

### Comparing `DI-engine-0.4.7/dizoo/d4rl/config/walker2d_medium_replay_dt_config.py` & `DI-engine-0.4.8/dizoo/d4rl/config/walker2d_medium_replay_dt_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/d4rl/config/walker2d_medium_replay_td3bc_config.py` & `DI-engine-0.4.8/dizoo/d4rl/config/walker2d_random_td3bc_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 # You can conduct Experiments on D4RL with this config file through the following command:
 # cd ../entry && python d4rl_td3_bc_main.py
 from easydict import EasyDict
 
 main_config = dict(
-    exp_name='walker2d_medium_replay_td3-bc_seed0',
+    exp_name='walker2d_random_td3-bc_seed0',
     env=dict(
-        env_id='walker2d-medium-replay-v0',
+        env_id='walker2d-random-v2',
         norm_obs=dict(
-            use_norm=True, 
+            use_norm=True,
             offline_stats=dict(use_offline_stats=True, ),
         ),
         collector_env_num=1,
         evaluator_env_num=8,
         use_act_scale=True,
         n_evaluator_episode=8,
         stop_value=6000,
     ),
     policy=dict(
+        cuda=True,
         model=dict(
-            obs_shape=11,
-            action_shape=3,
+            obs_shape=17,
+            action_shape=6,
         ),
         learn=dict(
             train_epoch=30000,
             batch_size=256,
             learning_rate_actor=0.0003,
             learning_rate_critic=0.0003,
             actor_update_freq=2,
```

### Comparing `DI-engine-0.4.7/dizoo/d4rl/config/walker2d_medium_td3bc_config.py` & `DI-engine-0.4.8/dizoo/d4rl/config/walker2d_medium_td3bc_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 # You can conduct Experiments on D4RL with this config file through the following command:
 # cd ../entry && python d4rl_td3_bc_main.py
 from easydict import EasyDict
 
 main_config = dict(
     exp_name='walker2d_medium_td3-bc_seed0',
     env=dict(
-        env_id='walker2d-medium-v0',
+        env_id='walker2d-medium-v2',
         norm_obs=dict(
-            use_norm=True, 
+            use_norm=True,
             offline_stats=dict(use_offline_stats=True, ),
         ),
         collector_env_num=1,
         evaluator_env_num=8,
         use_act_scale=True,
         n_evaluator_episode=8,
         stop_value=6000,
     ),
     policy=dict(
+        cuda=True,
         model=dict(
-            obs_shape=11,
-            action_shape=3,
+            obs_shape=17,
+            action_shape=6,
         ),
         learn=dict(
             train_epoch=30000,
             batch_size=256,
             learning_rate_actor=0.0003,
             learning_rate_critic=0.0003,
             actor_update_freq=2,
```

### Comparing `DI-engine-0.4.7/dizoo/d4rl/config/walker2d_random_cql_config.py` & `DI-engine-0.4.8/dizoo/d4rl/config/walker2d_random_cql_config.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # You can conduct Experiments on D4RL with this config file through the following command:
 # cd ../entry && python d4rl_cql_main.py
 from easydict import EasyDict
 
 main_config = dict(
     exp_name="walker2d_expert_cql_seed0",
     env=dict(
-        env_id='walker2d-expert-v0',
+        env_id='walker2d-expert-v2',
         collector_env_num=1,
         evaluator_env_num=8,
         use_act_scale=True,
         n_evaluator_episode=8,
         stop_value=6000,
     ),
     policy=dict(
         cuda=True,
         model=dict(
-            obs_shape=11,
-            action_shape=3,
+            obs_shape=17,
+            action_shape=6,
         ),
         learn=dict(
             data_path=None,
             train_epoch=30000,
             batch_size=256,
             learning_rate_q=3e-4,
             learning_rate_policy=1e-4,
```

### Comparing `DI-engine-0.4.7/dizoo/d4rl/config/walker2d_random_dt_config.py` & `DI-engine-0.4.8/dizoo/d4rl/config/walker2d_random_dt_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/d4rl/config/walker2d_random_td3bc_config.py` & `DI-engine-0.4.8/dizoo/d4rl/config/walker2d_expert_td3bc_config.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 # You can conduct Experiments on D4RL with this config file through the following command:
 # cd ../entry && python d4rl_td3_bc_main.py
 from easydict import EasyDict
 
 main_config = dict(
-    exp_name='walker2d_random_td3-bc_seed0',
+    exp_name='halfcheetah_expert_td3-bc_seed0',
     env=dict(
-        env_id='walker2d-random-v0',
+        env_id='halfcheetah-expert-v2',
         norm_obs=dict(
-            use_norm=True, 
+            use_norm=True,
             offline_stats=dict(use_offline_stats=True, ),
         ),
         collector_env_num=1,
         evaluator_env_num=8,
         use_act_scale=True,
         n_evaluator_episode=8,
         stop_value=6000,
     ),
     policy=dict(
+        cuda=True,
         model=dict(
-            obs_shape=11,
-            action_shape=3,
+            obs_shape=17,
+            action_shape=6,
         ),
         learn=dict(
             train_epoch=30000,
             batch_size=256,
             learning_rate_actor=0.0003,
             learning_rate_critic=0.0003,
             actor_update_freq=2,
```

### Comparing `DI-engine-0.4.7/dizoo/d4rl/entry/d4rl_cql_main.py` & `DI-engine-0.4.8/dizoo/d4rl/entry/d4rl_cql_main.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/d4rl/entry/d4rl_dt_main.py` & `DI-engine-0.4.8/dizoo/d4rl/entry/d4rl_dt_main.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/d4rl/entry/d4rl_ibc_main.py` & `DI-engine-0.4.8/dizoo/d4rl/entry/d4rl_ibc_main.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/d4rl/entry/d4rl_td3_bc_main.py` & `DI-engine-0.4.8/dizoo/d4rl/entry/d4rl_td3_bc_main.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/d4rl/envs/d4rl_env.py` & `DI-engine-0.4.8/dizoo/d4rl/envs/d4rl_env.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/d4rl/envs/d4rl_wrappers.py` & `DI-engine-0.4.8/dizoo/d4rl/envs/d4rl_wrappers.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/dmc2gym/envs/dmc2gym_env.py` & `DI-engine-0.4.8/dizoo/dmc2gym/envs/dmc2gym_env.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/dmc2gym/envs/test_dmc2gym_env.py` & `DI-engine-0.4.8/dizoo/dmc2gym/envs/test_dmc2gym_env.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/evogym/envs/evogym_env.py` & `DI-engine-0.4.8/dizoo/evogym/envs/evogym_env.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/gfootball/entry/gfootball_bc_config.py` & `DI-engine-0.4.8/dizoo/gfootball/entry/gfootball_bc_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/gfootball/entry/gfootball_bc_kaggle5th_main.py` & `DI-engine-0.4.8/dizoo/gfootball/entry/gfootball_bc_kaggle5th_main.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/gfootball/entry/gfootball_bc_rule_lt0_main.py` & `DI-engine-0.4.8/dizoo/gfootball/entry/gfootball_bc_rule_lt0_main.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/gfootball/entry/gfootball_bc_rule_main.py` & `DI-engine-0.4.8/dizoo/gfootball/entry/gfootball_bc_rule_main.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/gfootball/entry/gfootball_dqn_config.py` & `DI-engine-0.4.8/dizoo/gfootball/entry/gfootball_dqn_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/gfootball/entry/show_dataset.py` & `DI-engine-0.4.8/dizoo/gfootball/entry/show_dataset.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/gfootball/entry/test_accuracy.py` & `DI-engine-0.4.8/dizoo/gfootball/entry/test_accuracy.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/gfootball/envs/fake_dataset.py` & `DI-engine-0.4.8/dizoo/gfootball/envs/fake_dataset.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/gfootball/envs/gfootball_academy_env.py` & `DI-engine-0.4.8/dizoo/gfootball/envs/gfootball_academy_env.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/gfootball/envs/gfootball_env.py` & `DI-engine-0.4.8/dizoo/gfootball/envs/gfootball_env.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/gfootball/envs/gfootballsp_env.py` & `DI-engine-0.4.8/dizoo/gfootball/envs/gfootballsp_env.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/gfootball/model/bots/kaggle_5th_place_model.py` & `DI-engine-0.4.8/dizoo/gfootball/model/bots/kaggle_5th_place_model.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/gfootball/model/bots/rule_based_bot_model.py` & `DI-engine-0.4.8/dizoo/gfootball/model/bots/rule_based_bot_model.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/gfootball/policy/ppo_lstm.py` & `DI-engine-0.4.8/dizoo/gfootball/policy/ppo_lstm.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/gfootball/replay.py` & `DI-engine-0.4.8/dizoo/gfootball/replay.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/gym_anytrading/config/stocks_dqn_config.py` & `DI-engine-0.4.8/dizoo/gym_anytrading/config/stocks_dqn_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/gym_anytrading/envs/stocks_env.py` & `DI-engine-0.4.8/dizoo/gym_anytrading/envs/stocks_env.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/gym_anytrading/envs/test_stocks_env.py` & `DI-engine-0.4.8/dizoo/gym_anytrading/envs/test_stocks_env.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/gym_anytrading/envs/trading_env.py` & `DI-engine-0.4.8/dizoo/gym_anytrading/envs/trading_env.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/gym_anytrading/worker/trading_serial_evaluator.py` & `DI-engine-0.4.8/dizoo/gym_anytrading/worker/trading_serial_evaluator.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/gym_hybrid/config/gym_hybrid_ddpg_config.py` & `DI-engine-0.4.8/dizoo/gym_hybrid/config/gym_hybrid_ddpg_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/gym_hybrid/config/gym_hybrid_hppo_config.py` & `DI-engine-0.4.8/dizoo/gym_hybrid/config/gym_hybrid_hppo_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/gym_hybrid/config/gym_hybrid_mpdqn_config.py` & `DI-engine-0.4.8/dizoo/gym_hybrid/config/gym_hybrid_mpdqn_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/gym_hybrid/config/gym_hybrid_pdqn_config.py` & `DI-engine-0.4.8/dizoo/gym_hybrid/config/gym_hybrid_pdqn_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/gym_hybrid/entry/e.py` & `DI-engine-0.4.8/dizoo/gym_hybrid/entry/e.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/gym_hybrid/entry/gym_hybrid_ddpg_eval.py` & `DI-engine-0.4.8/dizoo/gym_hybrid/entry/gym_hybrid_ddpg_eval.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/gym_hybrid/entry/gym_hybrid_ddpg_main.py` & `DI-engine-0.4.8/dizoo/gym_hybrid/entry/gym_hybrid_ddpg_main.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/gym_hybrid/envs/gym_hybrid_env.py` & `DI-engine-0.4.8/dizoo/gym_hybrid/envs/gym_hybrid_env.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,40 +84,40 @@
                 # rotation_value. Following line can be omitted, because in the affine_transform function,
                 # we have already done the clip(-1,1) operation
                 action['action_args'][1] = affine_transform(action['action_args'][1], min_val=-1, max_val=1)
                 action = [action['action_type'], action['action_args']]
         if self._save_replay:
             self._frames.append(self._env.render(mode='rgb_array'))
         obs, rew, done, info = self._env.step(action)
-        self._eval_episode_return += rew
-        if done:
-            info['eval_episode_return'] = self._eval_episode_return
-            if self._save_replay:
-                if self._env_id == 'HardMove-v0':
-                    self._env_id = f'hardmove_n{self._cfg.num_actuators}'
-                path = os.path.join(
-                    self._replay_path, '{}_episode_{}.gif'.format(self._env_id, self._save_replay_count)
-                )
-                self.display_frames_as_gif(self._frames, path)
-                self._frames = []
-                self._save_replay_count += 1
 
         obs = to_ndarray(obs)
         if isinstance(obs, list):  # corner case
             for i in range(len(obs)):
                 if len(obs[i].shape) == 0:
                     obs[i] = np.array([obs[i]])
             obs = np.concatenate(obs)
         assert isinstance(obs, np.ndarray) and obs.shape == (10, )
         obs = obs.astype(np.float32)
 
         rew = to_ndarray([rew])  # wrapped to be transferred to a numpy array with shape (1,)
         if isinstance(rew, list):
             rew = rew[0]
         assert isinstance(rew, np.ndarray) and rew.shape == (1, )
+        self._eval_episode_return += rew.item()
+        if done:
+            info['eval_episode_return'] = self._eval_episode_return
+            if self._save_replay:
+                if self._env_id == 'HardMove-v0':
+                    self._env_id = f'hardmove_n{self._cfg.num_actuators}'
+                path = os.path.join(
+                    self._replay_path, '{}_episode_{}.gif'.format(self._env_id, self._save_replay_count)
+                )
+                self.display_frames_as_gif(self._frames, path)
+                self._frames = []
+                self._save_replay_count += 1
         info['action_args_mask'] = np.array([[1, 0], [0, 1], [0, 0]])
         return BaseEnvTimestep(obs, rew, done, info)
 
     def random_action(self) -> Dict:
         # action_type: 0, 1, 2
         # action_args:
         #   - acceleration_value: [0, 1]
```

### Comparing `DI-engine-0.4.7/dizoo/gym_hybrid/envs/test_gym_hybrid_env.py` & `DI-engine-0.4.8/dizoo/gym_hybrid/envs/test_gym_hybrid_env.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/gym_pybullet_drones/envs/gym_pybullet_drones_env.py` & `DI-engine-0.4.8/dizoo/gym_pybullet_drones/envs/gym_pybullet_drones_env.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/gym_pybullet_drones/envs/test_ding_env.py` & `DI-engine-0.4.8/dizoo/gym_pybullet_drones/envs/test_ding_env.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/gym_pybullet_drones/envs/test_ori_env.py` & `DI-engine-0.4.8/dizoo/gym_pybullet_drones/envs/test_ori_env.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/gym_soccer/envs/gym_soccer_env.py` & `DI-engine-0.4.8/dizoo/gym_soccer/envs/gym_soccer_env.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/gym_soccer/envs/test_gym_soccer_env.py` & `DI-engine-0.4.8/dizoo/gym_soccer/envs/test_gym_soccer_env.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/image_classification/data/dataset.py` & `DI-engine-0.4.8/dizoo/image_classification/data/dataset.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/image_classification/data/sampler.py` & `DI-engine-0.4.8/dizoo/image_classification/data/sampler.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/image_classification/policy/policy.py` & `DI-engine-0.4.8/dizoo/image_classification/policy/policy.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/league_demo/demo_league.py` & `DI-engine-0.4.8/dizoo/league_demo/demo_league.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/league_demo/game_env.py` & `DI-engine-0.4.8/dizoo/league_demo/game_env.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/league_demo/league_demo_collector.py` & `DI-engine-0.4.8/dizoo/league_demo/league_demo_collector.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/league_demo/league_demo_ppo_config.py` & `DI-engine-0.4.8/dizoo/league_demo/league_demo_ppo_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/league_demo/league_demo_ppo_main.py` & `DI-engine-0.4.8/dizoo/league_demo/league_demo_ppo_main.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/league_demo/selfplay_demo_ppo_config.py` & `DI-engine-0.4.8/dizoo/league_demo/selfplay_demo_ppo_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/league_demo/selfplay_demo_ppo_main.py` & `DI-engine-0.4.8/dizoo/league_demo/selfplay_demo_ppo_main.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/mario/mario_dqn_config.py` & `DI-engine-0.4.8/dizoo/atari/config/serial/pong/pong_iqn_config.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,49 +1,62 @@
 from easydict import EasyDict
 
-mario_dqn_config = dict(
-    exp_name='mario_dqn_seed0',
+pong_iqn_config = dict(
+    exp_name='pong_iqn_seed0',
     env=dict(
         collector_env_num=8,
         evaluator_env_num=8,
         n_evaluator_episode=8,
-        stop_value=100000,
-        replay_path='mario_dqn_seed0/video',
+        stop_value=20,
+        env_id='PongNoFrameskip-v4',
+        #'ALE/Pong-v5' is available. But special setting is needed after gym make.
+        frame_stack=4,
     ),
     policy=dict(
         cuda=True,
+        priority=False,
         model=dict(
             obs_shape=[4, 84, 84],
-            action_shape=2,
-            encoder_hidden_size_list=[128, 128, 256],
-            dueling=True,
+            action_shape=6,
+            encoder_hidden_size_list=[128, 128, 512],
+            num_quantiles=32,
         ),
         nstep=3,
         discount_factor=0.99,
+        kappa=1.0,
         learn=dict(
             update_per_collect=10,
             batch_size=32,
             learning_rate=0.0001,
             target_update_freq=500,
         ),
-        collect=dict(n_sample=96, ),
-        eval=dict(evaluator=dict(eval_freq=2000, )),
+        collect=dict(n_sample=100, ),
+        eval=dict(evaluator=dict(eval_freq=4000, )),
         other=dict(
             eps=dict(
                 type='exp',
                 start=1.,
                 end=0.05,
                 decay=250000,
             ),
             replay_buffer=dict(replay_buffer_size=100000, ),
         ),
     ),
 )
-mario_dqn_config = EasyDict(mario_dqn_config)
-main_config = mario_dqn_config
-mario_dqn_create_config = dict(
+pong_iqn_config = EasyDict(pong_iqn_config)
+main_config = pong_iqn_config
+
+pong_iqn_create_config = dict(
+    env=dict(
+        type='atari',
+        import_names=['dizoo.atari.envs.atari_env'],
+    ),
     env_manager=dict(type='subprocess'),
-    policy=dict(type='dqn'),
+    policy=dict(type='iqn'),
 )
-mario_dqn_create_config = EasyDict(mario_dqn_create_config)
-create_config = mario_dqn_create_config
-# you can run `python3 -u mario_dqn_main.py`
+pong_iqn_create_config = EasyDict(pong_iqn_create_config)
+create_config = pong_iqn_create_config
+
+if __name__ == '__main__':
+    # or you can enter `ding -m serial -c pong_iqn_config.py -s 0`
+    from ding.entry import serial_pipeline
+    serial_pipeline((main_config, create_config), seed=0)
```

### Comparing `DI-engine-0.4.7/dizoo/mario/mario_dqn_example.py` & `DI-engine-0.4.8/dizoo/mario/mario_dqn_example.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/mario/mario_dqn_main.py` & `DI-engine-0.4.8/dizoo/mario/mario_dqn_main.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/maze/envs/maze_env.py` & `DI-engine-0.4.8/dizoo/maze/envs/maze_env.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/maze/envs/test_maze_env.py` & `DI-engine-0.4.8/dizoo/maze/envs/test_maze_env.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/metadrive/config/metadrive_onppo_config.py` & `DI-engine-0.4.8/dizoo/metadrive/config/metadrive_onppo_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/metadrive/config/metadrive_onppo_eval_config.py` & `DI-engine-0.4.8/dizoo/metadrive/config/metadrive_onppo_eval_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/metadrive/env/drive_env.py` & `DI-engine-0.4.8/dizoo/metadrive/env/drive_env.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/metadrive/env/drive_utils.py` & `DI-engine-0.4.8/dizoo/metadrive/env/drive_utils.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/metadrive/env/drive_wrapper.py` & `DI-engine-0.4.8/dizoo/metadrive/env/drive_wrapper.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/minigrid/__init__.py` & `DI-engine-0.4.8/dizoo/minigrid/__init__.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/minigrid/envs/app_key_to_door_treasure.py` & `DI-engine-0.4.8/dizoo/minigrid/envs/app_key_to_door_treasure.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/minigrid/envs/minigrid_env.py` & `DI-engine-0.4.8/dizoo/minigrid/envs/minigrid_env.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/minigrid/envs/minigrid_wrapper.py` & `DI-engine-0.4.8/dizoo/minigrid/envs/minigrid_wrapper.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/minigrid/envs/noisy_tv.py` & `DI-engine-0.4.8/dizoo/minigrid/envs/noisy_tv.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/minigrid/envs/test_minigrid_env.py` & `DI-engine-0.4.8/dizoo/minigrid/envs/test_minigrid_env.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/mujoco/config/ant_ddpg_config.py` & `DI-engine-0.4.8/dizoo/mujoco/config/ant_ddpg_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/mujoco/config/ant_gail_sac_config.py` & `DI-engine-0.4.8/dizoo/mujoco/config/ant_gail_sac_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/mujoco/config/ant_onppo_config.py` & `DI-engine-0.4.8/dizoo/mujoco/config/ant_onppo_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/mujoco/config/ant_ppo_config.py` & `DI-engine-0.4.8/dizoo/mujoco/config/ant_ppo_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/mujoco/config/ant_sac_config.py` & `DI-engine-0.4.8/dizoo/mujoco/config/ant_sac_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/mujoco/config/ant_td3_config.py` & `DI-engine-0.4.8/dizoo/mujoco/config/ant_td3_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/mujoco/config/ant_trex_onppo_config.py` & `DI-engine-0.4.8/dizoo/mujoco/config/ant_trex_onppo_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/mujoco/config/ant_trex_sac_config.py` & `DI-engine-0.4.8/dizoo/mujoco/config/ant_trex_sac_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/mujoco/config/halfcheetah_bco_config.py` & `DI-engine-0.4.8/dizoo/mujoco/config/halfcheetah_bco_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/mujoco/config/halfcheetah_bdq_config.py` & `DI-engine-0.4.8/dizoo/mujoco/config/halfcheetah_bdq_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/mujoco/config/halfcheetah_d4pg_config.py` & `DI-engine-0.4.8/dizoo/mujoco/config/halfcheetah_d4pg_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/mujoco/config/halfcheetah_ddpg_config.py` & `DI-engine-0.4.8/dizoo/mujoco/config/halfcheetah_ddpg_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/mujoco/config/halfcheetah_gail_sac_config.py` & `DI-engine-0.4.8/dizoo/mujoco/config/halfcheetah_gail_sac_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/mujoco/config/halfcheetah_gcl_sac_config.py` & `DI-engine-0.4.8/dizoo/mujoco/config/halfcheetah_gcl_sac_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/mujoco/config/halfcheetah_onppo_config.py` & `DI-engine-0.4.8/dizoo/mujoco/config/halfcheetah_onppo_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/mujoco/config/halfcheetah_sac_config.py` & `DI-engine-0.4.8/dizoo/mujoco/config/halfcheetah_sac_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/mujoco/config/halfcheetah_sqil_sac_config.py` & `DI-engine-0.4.8/dizoo/mujoco/config/halfcheetah_sqil_sac_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/mujoco/config/halfcheetah_td3_config.py` & `DI-engine-0.4.8/dizoo/mujoco/config/halfcheetah_td3_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/mujoco/config/halfcheetah_trex_onppo_config.py` & `DI-engine-0.4.8/dizoo/mujoco/config/halfcheetah_trex_onppo_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/mujoco/config/halfcheetah_trex_sac_config.py` & `DI-engine-0.4.8/dizoo/mujoco/config/halfcheetah_trex_sac_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/mujoco/config/hopper_bco_config.py` & `DI-engine-0.4.8/dizoo/mujoco/config/hopper_bco_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/mujoco/config/hopper_bdq_config.py` & `DI-engine-0.4.8/dizoo/mujoco/config/hopper_bdq_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/mujoco/config/hopper_cql_config.py` & `DI-engine-0.4.8/dizoo/mujoco/config/hopper_cql_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/mujoco/config/hopper_d4pg_config.py` & `DI-engine-0.4.8/dizoo/mujoco/config/hopper_d4pg_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/mujoco/config/hopper_ddpg_config.py` & `DI-engine-0.4.8/dizoo/mujoco/config/hopper_ddpg_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/mujoco/config/hopper_gail_sac_config.py` & `DI-engine-0.4.8/dizoo/mujoco/config/hopper_gail_sac_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/mujoco/config/hopper_gcl_config.py` & `DI-engine-0.4.8/dizoo/mujoco/config/hopper_gcl_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/mujoco/config/hopper_onppo_config.py` & `DI-engine-0.4.8/dizoo/mujoco/config/hopper_onppo_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/mujoco/config/hopper_sac_config.py` & `DI-engine-0.4.8/dizoo/mujoco/config/hopper_sac_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/mujoco/config/hopper_sac_data_generation_config.py` & `DI-engine-0.4.8/dizoo/mujoco/config/hopper_sac_data_generation_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/mujoco/config/hopper_sqil_sac_config.py` & `DI-engine-0.4.8/dizoo/mujoco/config/hopper_sqil_sac_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/mujoco/config/hopper_td3_bc_config.py` & `DI-engine-0.4.8/dizoo/mujoco/config/hopper_td3_bc_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/mujoco/config/hopper_td3_config.py` & `DI-engine-0.4.8/dizoo/mujoco/config/hopper_td3_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/mujoco/config/hopper_td3_data_generation_config.py` & `DI-engine-0.4.8/dizoo/mujoco/config/hopper_td3_data_generation_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/mujoco/config/hopper_trex_onppo_config.py` & `DI-engine-0.4.8/dizoo/mujoco/config/hopper_trex_onppo_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/mujoco/config/hopper_trex_sac_config.py` & `DI-engine-0.4.8/dizoo/mujoco/config/hopper_trex_sac_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/mujoco/config/walker2d_d4pg_config.py` & `DI-engine-0.4.8/dizoo/mujoco/config/walker2d_d4pg_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/mujoco/config/walker2d_ddpg_config.py` & `DI-engine-0.4.8/dizoo/mujoco/config/walker2d_ddpg_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/mujoco/config/walker2d_gail_ddpg_config.py` & `DI-engine-0.4.8/dizoo/mujoco/config/walker2d_gail_ddpg_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/mujoco/config/walker2d_gail_sac_config.py` & `DI-engine-0.4.8/dizoo/mujoco/config/walker2d_gail_sac_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/mujoco/config/walker2d_gcl_config.py` & `DI-engine-0.4.8/dizoo/mujoco/config/walker2d_gcl_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/mujoco/config/walker2d_onppo_config.py` & `DI-engine-0.4.8/dizoo/mujoco/config/walker2d_onppo_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/mujoco/config/walker2d_sac_config.py` & `DI-engine-0.4.8/dizoo/mujoco/config/walker2d_sac_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/mujoco/config/walker2d_sqil_sac_config.py` & `DI-engine-0.4.8/dizoo/mujoco/config/walker2d_sqil_sac_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/mujoco/config/walker2d_td3_config.py` & `DI-engine-0.4.8/dizoo/mujoco/config/walker2d_td3_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/mujoco/config/walker2d_trex_onppo_config.py` & `DI-engine-0.4.8/dizoo/mujoco/config/walker2d_trex_onppo_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/mujoco/config/walker2d_trex_sac_config.py` & `DI-engine-0.4.8/dizoo/mujoco/config/walker2d_trex_sac_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/mujoco/entry/mujoco_cql_generation_main.py` & `DI-engine-0.4.8/dizoo/mujoco/entry/mujoco_cql_generation_main.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/mujoco/entry/mujoco_d4pg_main.py` & `DI-engine-0.4.8/dizoo/mujoco/entry/mujoco_d4pg_main.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/mujoco/entry/mujoco_ddpg_eval.py` & `DI-engine-0.4.8/dizoo/mujoco/entry/mujoco_ddpg_eval.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/mujoco/entry/mujoco_ddpg_main.py` & `DI-engine-0.4.8/dizoo/mujoco/entry/mujoco_ddpg_main.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/mujoco/entry/mujoco_ppo_main.py` & `DI-engine-0.4.8/dizoo/mujoco/entry/mujoco_ppo_main.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/mujoco/entry/mujoco_td3_bc_main.py` & `DI-engine-0.4.8/dizoo/mujoco/entry/mujoco_td3_bc_main.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/mujoco/envs/mujoco_disc_env.py` & `DI-engine-0.4.8/dizoo/mujoco/envs/mujoco_disc_env.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/mujoco/envs/mujoco_env.py` & `DI-engine-0.4.8/dizoo/mujoco/envs/mujoco_env.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/mujoco/envs/mujoco_gym_env.py` & `DI-engine-0.4.8/dizoo/mujoco/envs/mujoco_gym_env.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/mujoco/envs/mujoco_wrappers.py` & `DI-engine-0.4.8/dizoo/mujoco/envs/mujoco_wrappers.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/multiagent_mujoco/envs/assets/coupled_half_cheetah.xml` & `DI-engine-0.4.8/dizoo/multiagent_mujoco/envs/assets/coupled_half_cheetah.xml`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/multiagent_mujoco/envs/assets/manyagent_ant.xml` & `DI-engine-0.4.8/dizoo/multiagent_mujoco/envs/assets/manyagent_ant.xml`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/multiagent_mujoco/envs/assets/manyagent_ant__stage1.xml` & `DI-engine-0.4.8/dizoo/multiagent_mujoco/envs/assets/manyagent_ant__stage1.xml`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/multiagent_mujoco/envs/assets/manyagent_swimmer__bckp2.xml` & `DI-engine-0.4.8/dizoo/multiagent_mujoco/envs/assets/manyagent_swimmer__bckp2.xml`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/multiagent_mujoco/envs/assets/manyagent_swimmer_bckp.xml` & `DI-engine-0.4.8/dizoo/multiagent_mujoco/envs/assets/manyagent_swimmer_bckp.xml`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/multiagent_mujoco/envs/coupled_half_cheetah.py` & `DI-engine-0.4.8/dizoo/multiagent_mujoco/envs/coupled_half_cheetah.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/multiagent_mujoco/envs/manyagent_ant.py` & `DI-engine-0.4.8/dizoo/multiagent_mujoco/envs/manyagent_ant.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/multiagent_mujoco/envs/manyagent_swimmer.py` & `DI-engine-0.4.8/dizoo/multiagent_mujoco/envs/manyagent_swimmer.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/multiagent_mujoco/envs/mujoco_multi.py` & `DI-engine-0.4.8/dizoo/multiagent_mujoco/envs/mujoco_multi.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/multiagent_mujoco/envs/multi_mujoco_env.py` & `DI-engine-0.4.8/dizoo/multiagent_mujoco/envs/multi_mujoco_env.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/multiagent_mujoco/envs/multiagentenv.py` & `DI-engine-0.4.8/dizoo/multiagent_mujoco/envs/multiagentenv.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/multiagent_mujoco/envs/obsk.py` & `DI-engine-0.4.8/dizoo/multiagent_mujoco/envs/obsk.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/overcooked/config/overcooked_ppo_config.py` & `DI-engine-0.4.8/dizoo/overcooked/config/overcooked_ppo_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/overcooked/envs/overcooked_env.py` & `DI-engine-0.4.8/dizoo/overcooked/envs/overcooked_env.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/overcooked/envs/test_overcooked_env.py` & `DI-engine-0.4.8/dizoo/overcooked/envs/test_overcooked_env.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/petting_zoo/config/__init__.py` & `DI-engine-0.4.8/dizoo/petting_zoo/config/__init__.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/petting_zoo/config/ptz_simple_spread_atoc_config.py` & `DI-engine-0.4.8/dizoo/petting_zoo/config/ptz_simple_spread_atoc_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/petting_zoo/config/ptz_simple_spread_collaq_config.py` & `DI-engine-0.4.8/dizoo/petting_zoo/config/ptz_simple_spread_collaq_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/petting_zoo/config/ptz_simple_spread_coma_config.py` & `DI-engine-0.4.8/dizoo/petting_zoo/config/ptz_simple_spread_coma_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/petting_zoo/config/ptz_simple_spread_madqn_config.py` & `DI-engine-0.4.8/dizoo/petting_zoo/config/ptz_simple_spread_madqn_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/petting_zoo/config/ptz_simple_spread_mappo_config.py` & `DI-engine-0.4.8/dizoo/petting_zoo/config/ptz_simple_spread_mappo_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/petting_zoo/config/ptz_simple_spread_masac_config.py` & `DI-engine-0.4.8/dizoo/petting_zoo/config/ptz_simple_spread_masac_config.py`

 * *Files 16% similar despite different names*

```diff
@@ -20,51 +20,39 @@
         n_evaluator_episode=evaluator_env_num,
         stop_value=0,
     ),
     policy=dict(
         cuda=True,
         on_policy=False,
         multi_agent=True,
-        # priority=True,
-        # priority_IS_weight=False,
-        random_collect_size=0,
+        random_collect_size=5000,
         model=dict(
             agent_obs_shape=2 + 2 + n_landmark * 2 + (n_agent - 1) * 2 + (n_agent - 1) * 2,
             global_obs_shape=2 + 2 + n_landmark * 2 + (n_agent - 1) * 2 + (n_agent - 1) * 2 + n_agent * (2 + 2) +
             n_landmark * 2 + n_agent * (n_agent - 1) * 2,
             action_shape=5,
-            # SAC concerned
             twin_critic=True,
-            actor_head_hidden_size=256,
-            critic_head_hidden_size=256,
         ),
         learn=dict(
             update_per_collect=50,
             batch_size=320,
-            # ==============================================================
-            # The following configs is algorithm-specific
-            # ==============================================================
             # learning_rates
             learning_rate_q=5e-4,
             learning_rate_policy=5e-4,
             learning_rate_alpha=5e-5,
             target_theta=0.005,
             discount_factor=0.99,
             alpha=0.2,
             auto_alpha=True,
-            log_space=True,
-            ignore_down=False,
             target_entropy=-2,
         ),
         collect=dict(
             n_sample=1600,
-            unroll_len=1,
             env_num=collector_env_num,
         ),
-        command=dict(),
         eval=dict(
             env_num=evaluator_env_num,
             evaluator=dict(eval_freq=50, ),
         ),
         other=dict(
             eps=dict(
                 type='linear',
```

### Comparing `DI-engine-0.4.7/dizoo/petting_zoo/config/ptz_simple_spread_qmix_config.py` & `DI-engine-0.4.8/dizoo/petting_zoo/config/ptz_simple_spread_qmix_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/petting_zoo/config/ptz_simple_spread_qtran_config.py` & `DI-engine-0.4.8/dizoo/petting_zoo/config/ptz_simple_spread_qtran_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/petting_zoo/config/ptz_simple_spread_vdn_config.py` & `DI-engine-0.4.8/dizoo/petting_zoo/config/ptz_simple_spread_vdn_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/petting_zoo/config/ptz_simple_spread_wqmix_config.py` & `DI-engine-0.4.8/dizoo/petting_zoo/config/ptz_simple_spread_wqmix_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/petting_zoo/envs/petting_zoo_simple_spread_env.py` & `DI-engine-0.4.8/dizoo/petting_zoo/envs/petting_zoo_simple_spread_env.py`

 * *Files 1% similar despite different names*

```diff
@@ -176,14 +176,15 @@
                 action[agent] = affine_transform(
                     action[agent], min_val=self.action_space[agent].low, max_val=self.action_space[agent].high
                 )
 
         obs, rew, done, trunc, info = self._env.step(action)
         obs_n = self._process_obs(obs)
         rew_n = np.array([sum([rew[agent] for agent in self._agents])])
+        rew_n = rew_n.astype(np.float32)
         # collide_sum = 0
         # for i in range(self._num_agents):
         #     collide_sum += info['n'][i][1]
         # collide_penalty = self._cfg.get('collide_penal', self._num_agent)
         # rew_n += collide_sum * (1.0 - collide_penalty)
         # rew_n = rew_n / (self._cfg.get('max_cycles', 25) * self._num_agent)
         self._eval_episode_return += rew_n.item()
@@ -267,15 +268,15 @@
                 np.zeros((self._num_agents,
                           (self._num_agents - 1) * 2), np.float32),  # Other agents' position(0-padding)
                 obs[:, -(self._num_agents - 1) * 2:]  # communication
             ],
             1
         )
         # action_mask: All actions are of use(either 1 for discrete or 5 for continuous). Thus all 1.
-        ret['action_mask'] = np.ones((self._num_agents, *self._action_dim))
+        ret['action_mask'] = np.ones((self._num_agents, *self._action_dim)).astype(np.float32)
         return ret
 
     def _process_action(self, action: 'torch.Tensor') -> Dict[str, np.ndarray]:  # noqa
         dict_action = {}
         for i, agent in enumerate(self._agents):
             agent_action = action[i]
             if agent_action.shape == (1, ):
```

### Comparing `DI-engine-0.4.7/dizoo/petting_zoo/envs/test_petting_zoo_simple_spread_env.py` & `DI-engine-0.4.8/dizoo/petting_zoo/envs/test_petting_zoo_simple_spread_env.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
+from easydict import EasyDict
+import pytest
 import numpy as np
 import pettingzoo
 from ding.utils import import_module
-from easydict import EasyDict
-import pytest
 
-from dizoo.petting_zoo.envs.petting_zoo_env import PettingZooEnv
+from dizoo.petting_zoo.envs.petting_zoo_simple_spread_env import PettingZooEnv
 
 
 @pytest.mark.envtest
 class TestPettingZooEnv:
 
     def test_agent_obs_only(self):
         n_agent = 5
@@ -35,14 +35,15 @@
             random_action = np.array([random_action[agent] for agent in random_action])
             timestep = env.step(random_action)
             print(timestep)
             assert isinstance(timestep.obs, np.ndarray), timestep.obs
             assert timestep.obs.shape == (n_agent, 2 + 2 + (n_agent - 1) * 2 + n_agent * 2 + (n_agent - 1) * 2)
             assert isinstance(timestep.done, bool), timestep.done
             assert isinstance(timestep.reward, np.ndarray), timestep.reward
+            assert timestep.reward.dtype == np.float32
         print(env.observation_space, env.action_space, env.reward_space)
         env.close()
 
     def test_dict_obs(self):
         n_agent = 5
         n_landmark = n_agent
         env = PettingZooEnv(
@@ -76,14 +77,15 @@
             assert timestep.obs['global_state'].shape == (
                 n_agent * (2 + 2) + n_landmark * 2 + n_agent * (n_agent - 1) * 2,
             )
             assert timestep.obs['agent_alone_state'].shape == (n_agent, 2 + 2 + n_landmark * 2 + (n_agent - 1) * 2)
             assert timestep.obs['agent_alone_padding_state'].shape == (
                 n_agent, 2 + 2 + n_landmark * 2 + (n_agent - 1) * 2 + (n_agent - 1) * 2
             )
+            assert timestep.obs['action_mask'].dtype == np.float32
             assert isinstance(timestep.done, bool), timestep.done
             assert isinstance(timestep.reward, np.ndarray), timestep.reward
         print(env.observation_space, env.action_space, env.reward_space)
         env.close()
 
     def test_agent_specific_global_state(self):
         n_agent = 5
```

### Comparing `DI-engine-0.4.7/dizoo/pomdp/envs/atari_env.py` & `DI-engine-0.4.8/dizoo/pomdp/envs/atari_env.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/pomdp/envs/atari_wrappers.py` & `DI-engine-0.4.8/dizoo/pomdp/envs/atari_wrappers.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/pomdp/envs/test_atari_env.py` & `DI-engine-0.4.8/dizoo/pomdp/envs/test_atari_env.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/procgen/config/bigfish_plr_config.py` & `DI-engine-0.4.8/dizoo/procgen/config/bigfish_plr_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/procgen/config/bigfish_ppg_config.py` & `DI-engine-0.4.8/dizoo/procgen/config/bigfish_ppg_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/procgen/config/coinrun_dqn_config.py` & `DI-engine-0.4.8/dizoo/procgen/config/maze_dqn_config.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from easydict import EasyDict
 
-coinrun_dqn_config = dict(
+maze_dqn_config = dict(
     env=dict(
-        env_id='coinrun',
         collector_env_num=4,
+        env_id='maze',
         evaluator_env_num=4,
         n_evaluator_episode=4,
         stop_value=10,
     ),
     policy=dict(
         cuda=False,
         model=dict(
@@ -18,34 +18,35 @@
         ),
         discount_factor=0.99,
         learn=dict(
             update_per_collect=20,
             batch_size=32,
             learning_rate=0.0005,
             target_update_freq=500,
+            discount_factor=0.99,
         ),
         collect=dict(n_sample=100, ),
         eval=dict(evaluator=dict(eval_freq=5000, )),
         other=dict(
             eps=dict(
                 type='exp',
                 start=1.,
                 end=0.05,
                 decay=250000,
             ),
             replay_buffer=dict(replay_buffer_size=100000, ),
         ),
     ),
 )
-coinrun_dqn_config = EasyDict(coinrun_dqn_config)
-main_config = coinrun_dqn_config
+maze_dqn_config = EasyDict(maze_dqn_config)
+main_config = maze_dqn_config
 
-coinrun_dqn_create_config = dict(
+maze_dqn_create_config = dict(
     env=dict(
         type='procgen',
         import_names=['dizoo.procgen.envs.procgen_env'],
     ),
     env_manager=dict(type='subprocess', ),
     policy=dict(type='dqn'),
 )
-coinrun_dqn_create_config = EasyDict(coinrun_dqn_create_config)
-create_config = coinrun_dqn_create_config
+maze_dqn_create_config = EasyDict(maze_dqn_create_config)
+create_config = maze_dqn_create_config
```

### Comparing `DI-engine-0.4.7/dizoo/procgen/config/coinrun_ppg_config.py` & `DI-engine-0.4.8/dizoo/procgen/config/coinrun_ppg_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/procgen/config/coinrun_ppo_config.py` & `DI-engine-0.4.8/dizoo/procgen/config/coinrun_ppo_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/procgen/config/maze_ppg_config.py` & `DI-engine-0.4.8/dizoo/procgen/config/maze_ppg_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/procgen/config/maze_ppo_config.py` & `DI-engine-0.4.8/dizoo/procgen/config/maze_ppo_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/procgen/envs/procgen_env.py` & `DI-engine-0.4.8/dizoo/procgen/envs/procgen_env.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/procgen/envs/test_coinrun_env.py` & `DI-engine-0.4.8/dizoo/procgen/envs/test_coinrun_env.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/pybullet/envs/pybullet_env.py` & `DI-engine-0.4.8/dizoo/pybullet/envs/pybullet_env.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/pybullet/envs/pybullet_wrappers.py` & `DI-engine-0.4.8/dizoo/pybullet/envs/pybullet_wrappers.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/rocket/config/rocket_hover_ppo_config.py` & `DI-engine-0.4.8/dizoo/rocket/config/rocket_hover_ppo_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/rocket/config/rocket_landing_ppo_config.py` & `DI-engine-0.4.8/dizoo/rocket/config/rocket_landing_ppo_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/rocket/entry/rocket_hover_onppo_main_v2.py` & `DI-engine-0.4.8/dizoo/rocket/entry/rocket_hover_onppo_main_v2.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/rocket/entry/rocket_hover_ppo_main.py` & `DI-engine-0.4.8/dizoo/rocket/entry/rocket_hover_ppo_main.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/rocket/entry/rocket_landing_onppo_main_v2.py` & `DI-engine-0.4.8/dizoo/rocket/entry/rocket_landing_onppo_main_v2.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/rocket/entry/rocket_landing_ppo_main.py` & `DI-engine-0.4.8/dizoo/rocket/entry/rocket_landing_ppo_main.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/rocket/envs/rocket_env.py` & `DI-engine-0.4.8/dizoo/rocket/envs/rocket_env.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/rocket/envs/test_rocket_env.py` & `DI-engine-0.4.8/dizoo/rocket/envs/test_rocket_env.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/slime_volley/config/slime_volley_ppo_config.py` & `DI-engine-0.4.8/dizoo/slime_volley/config/slime_volley_ppo_config.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/slime_volley/envs/slime_volley_env.py` & `DI-engine-0.4.8/dizoo/slime_volley/envs/slime_volley_env.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/slime_volley/envs/test_slime_volley_env.py` & `DI-engine-0.4.8/dizoo/slime_volley/envs/test_slime_volley_env.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/smac/envs/fake_smac_env.py` & `DI-engine-0.4.8/dizoo/smac/envs/fake_smac_env.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/smac/envs/maps/SMAC_Maps/10m_vs_11m.SC2Map` & `DI-engine-0.4.8/dizoo/smac/envs/maps/SMAC_Maps/10m_vs_11m.SC2Map`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/smac/envs/maps/SMAC_Maps/1c3s5z.SC2Map` & `DI-engine-0.4.8/dizoo/smac/envs/maps/SMAC_Maps/1c3s5z.SC2Map`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/smac/envs/maps/SMAC_Maps/25m.SC2Map` & `DI-engine-0.4.8/dizoo/smac/envs/maps/SMAC_Maps/25m.SC2Map`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/smac/envs/maps/SMAC_Maps/27m_vs_30m.SC2Map` & `DI-engine-0.4.8/dizoo/smac/envs/maps/SMAC_Maps/27m_vs_30m.SC2Map`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/smac/envs/maps/SMAC_Maps/2c_vs_64zg.SC2Map` & `DI-engine-0.4.8/dizoo/smac/envs/maps/SMAC_Maps/2c_vs_64zg.SC2Map`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/smac/envs/maps/SMAC_Maps/2m_vs_1z.SC2Map` & `DI-engine-0.4.8/dizoo/smac/envs/maps/SMAC_Maps/2m_vs_1z.SC2Map`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/smac/envs/maps/SMAC_Maps/2s3z.SC2Map` & `DI-engine-0.4.8/dizoo/smac/envs/maps/SMAC_Maps/2s3z.SC2Map`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/smac/envs/maps/SMAC_Maps/2s_vs_1sc.SC2Map` & `DI-engine-0.4.8/dizoo/smac/envs/maps/SMAC_Maps/2s_vs_1sc.SC2Map`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/smac/envs/maps/SMAC_Maps/3m.SC2Map` & `DI-engine-0.4.8/dizoo/smac/envs/maps/SMAC_Maps/3m.SC2Map`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/smac/envs/maps/SMAC_Maps/3s5z.SC2Map` & `DI-engine-0.4.8/dizoo/smac/envs/maps/SMAC_Maps/3s5z.SC2Map`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/smac/envs/maps/SMAC_Maps/3s5z_vs_3s6z.SC2Map` & `DI-engine-0.4.8/dizoo/smac/envs/maps/SMAC_Maps/3s5z_vs_3s6z.SC2Map`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/smac/envs/maps/SMAC_Maps/3s_vs_3z.SC2Map` & `DI-engine-0.4.8/dizoo/smac/envs/maps/SMAC_Maps/3s_vs_3z.SC2Map`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/smac/envs/maps/SMAC_Maps/3s_vs_4z.SC2Map` & `DI-engine-0.4.8/dizoo/smac/envs/maps/SMAC_Maps/3s_vs_4z.SC2Map`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/smac/envs/maps/SMAC_Maps/3s_vs_5z.SC2Map` & `DI-engine-0.4.8/dizoo/smac/envs/maps/SMAC_Maps/3s_vs_5z.SC2Map`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/smac/envs/maps/SMAC_Maps/5m_vs_6m.SC2Map` & `DI-engine-0.4.8/dizoo/smac/envs/maps/SMAC_Maps/5m_vs_6m.SC2Map`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/smac/envs/maps/SMAC_Maps/6h_vs_8z.SC2Map` & `DI-engine-0.4.8/dizoo/smac/envs/maps/SMAC_Maps/6h_vs_8z.SC2Map`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/smac/envs/maps/SMAC_Maps/8m.SC2Map` & `DI-engine-0.4.8/dizoo/smac/envs/maps/SMAC_Maps/8m.SC2Map`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/smac/envs/maps/SMAC_Maps/8m_vs_9m.SC2Map` & `DI-engine-0.4.8/dizoo/smac/envs/maps/SMAC_Maps/8m_vs_9m.SC2Map`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/smac/envs/maps/SMAC_Maps/MMM.SC2Map` & `DI-engine-0.4.8/dizoo/smac/envs/maps/SMAC_Maps/MMM.SC2Map`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/smac/envs/maps/SMAC_Maps/MMM2.SC2Map` & `DI-engine-0.4.8/dizoo/smac/envs/maps/SMAC_Maps/MMM2.SC2Map`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/smac/envs/maps/SMAC_Maps/bane_vs_bane.SC2Map` & `DI-engine-0.4.8/dizoo/smac/envs/maps/SMAC_Maps/bane_vs_bane.SC2Map`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/smac/envs/maps/SMAC_Maps/corridor.SC2Map` & `DI-engine-0.4.8/dizoo/smac/envs/maps/SMAC_Maps/corridor.SC2Map`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/smac/envs/maps/SMAC_Maps/infestor_viper.SC2Map` & `DI-engine-0.4.8/dizoo/smac/envs/maps/SMAC_Maps/infestor_viper.SC2Map`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/smac/envs/maps/SMAC_Maps/so_many_baneling.SC2Map` & `DI-engine-0.4.8/dizoo/smac/envs/maps/SMAC_Maps/so_many_baneling.SC2Map`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/smac/envs/maps/SMAC_Maps_two_player/3m.SC2Map` & `DI-engine-0.4.8/dizoo/smac/envs/maps/SMAC_Maps_two_player/3m.SC2Map`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/smac/envs/maps/SMAC_Maps_two_player/3s5z.SC2Map` & `DI-engine-0.4.8/dizoo/smac/envs/maps/SMAC_Maps_two_player/3s5z.SC2Map`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/smac/envs/smac_action.py` & `DI-engine-0.4.8/dizoo/smac/envs/smac_action.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/smac/envs/smac_env.py` & `DI-engine-0.4.8/dizoo/smac/envs/smac_env.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/smac/envs/smac_map.py` & `DI-engine-0.4.8/dizoo/smac/envs/smac_map.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/smac/envs/smac_reward.py` & `DI-engine-0.4.8/dizoo/smac/envs/smac_reward.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/smac/envs/test_smac_env.py` & `DI-engine-0.4.8/dizoo/smac/envs/test_smac_env.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/sokoban/envs/sokoban_env.py` & `DI-engine-0.4.8/dizoo/sokoban/envs/sokoban_env.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/sokoban/envs/sokoban_wrappers.py` & `DI-engine-0.4.8/dizoo/sokoban/envs/sokoban_wrappers.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/dizoo/sokoban/envs/test_sokoban_env.py` & `DI-engine-0.4.8/dizoo/sokoban/envs/test_sokoban_env.py`

 * *Files identical despite different names*

### Comparing `DI-engine-0.4.7/setup.py` & `DI-engine-0.4.8/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         package_name: ['*.yaml', '*.xml', '*cfg', '*SC2Map']
         for package_name in find_packages(include=('ding.*'))
     },
     python_requires=">=3.7",
     install_requires=[
         'setuptools<=66.1.1',
         'gym==0.25.1',  # pypy incompatible; some environmrnt only support gym==0.22.0
-        'torch>=1.1.0, <=1.12.1',  # If encountering pytorch errors, you need to do something like https://github.com/opendilab/DI-engine/discussions/81
+        #'torch>=1.1.0',
         'numpy>=1.18.0',
         'pandas',
         'tensorboardX>=2.2',
         'requests>=2.25.1',
         'pyyaml',
         'easydict==1.9',
         'protobuf',
@@ -74,15 +74,15 @@
         'readerwriterlock',
         'enum_tools',
         'trueskill',
         'h5py',
         'mpire>=2.3.5',
         'pynng',
         'redis',
-        'pettingzoo',
+        'pettingzoo<=1.22.3',
         'DI-treetensor>=0.3.0',
         'DI-toolkit>=0.0.2',
         'hbutils>=0.5.0',
         'wandb',
         'matplotlib',
         'MarkupSafe==2.0.1',  # compatibility
         'h5py',
```

